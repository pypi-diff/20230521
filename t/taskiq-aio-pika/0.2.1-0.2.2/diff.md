# Comparing `tmp/taskiq_aio_pika-0.2.1.tar.gz` & `tmp/taskiq_aio_pika-0.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "taskiq_aio_pika-0.2.1.tar", max compression
+gzip compressed data, was "taskiq_aio_pika-0.2.2.tar", max compression
```

## Comparing `taskiq_aio_pika-0.2.1.tar` & `taskiq_aio_pika-0.2.2.tar`

### file list

```diff
@@ -1,5 +1,5 @@
--rw-r--r--   0        0        0     3262 2023-05-12 13:53:36.937843 taskiq_aio_pika-0.2.1/README.md
--rw-r--r--   0        0        0     1536 2023-05-12 13:53:36.941843 taskiq_aio_pika-0.2.1/pyproject.toml
--rw-r--r--   0        0        0      118 2023-05-12 13:53:36.941843 taskiq_aio_pika-0.2.1/taskiq_aio_pika/__init__.py
--rw-r--r--   0        0        0     8864 2023-05-12 13:53:36.941843 taskiq_aio_pika-0.2.1/taskiq_aio_pika/broker.py
--rw-r--r--   0        0        0     4429 1970-01-01 00:00:00.000000 taskiq_aio_pika-0.2.1/PKG-INFO
+-rw-r--r--   0        0        0     4517 2023-05-21 16:19:07.936297 taskiq_aio_pika-0.2.2/README.md
+-rw-r--r--   0        0        0     1536 2023-05-21 16:19:07.936297 taskiq_aio_pika-0.2.2/pyproject.toml
+-rw-r--r--   0        0        0      118 2023-05-21 16:19:07.936297 taskiq_aio_pika-0.2.2/taskiq_aio_pika/__init__.py
+-rw-r--r--   0        0        0    10305 2023-05-21 16:19:07.936297 taskiq_aio_pika-0.2.2/taskiq_aio_pika/broker.py
+-rw-r--r--   0        0        0     5384 1970-01-01 00:00:00.000000 taskiq_aio_pika-0.2.2/PKG-INFO
```

### Comparing `taskiq_aio_pika-0.2.1/pyproject.toml` & `taskiq_aio_pika-0.2.2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "taskiq-aio-pika"
-version = "0.2.1"
+version = "0.2.2"
 description = "RabbitMQ broker for taskiq"
 authors = ["Pavel Kirilin <win10@list.ru>"]
 readme = "README.md"
 classifiers = [
     "Programming Language :: Python",
     "Programming Language :: Python :: 3",
     "Programming Language :: Python :: 3 :: Only",
```

### Comparing `taskiq_aio_pika-0.2.1/taskiq_aio_pika/broker.py` & `taskiq_aio_pika-0.2.2/taskiq_aio_pika/broker.py`

 * *Files 13% similar despite different names*

```diff
@@ -49,14 +49,15 @@
         dead_letter_queue_name: Optional[str] = None,
         delay_queue_name: Optional[str] = None,
         declare_exchange: bool = True,
         declare_queues: bool = True,
         routing_key: str = "#",
         exchange_type: ExchangeType = ExchangeType.TOPIC,
         max_priority: Optional[int] = None,
+        delayed_message_exchange_plugin: bool = False,
         **connection_kwargs: Any,
     ) -> None:
         """
         Construct a new broker.
 
         :param url: url to rabbitmq. If None,
             the default "amqp://guest:guest@localhost:5672" is used.
@@ -75,14 +76,16 @@
             if it doesn't exist.
         :param declare_queues: whether you want to declare queues even on
             client side. May be useful for message persistance.
         :param routing_key: that used to bind that queue to the exchange.
         :param exchange_type: type of the exchange.
             Used only if `declare_exchange` is True.
         :param max_priority: maximum priority value for messages.
+        :param delayed_message_exchange_plugin: turn on or disable
+            delayed-message-exchange rabbitmq plugin.
         :param connection_kwargs: additional keyword arguments,
             for connect_robust method of aio-pika.
         """
         super().__init__(result_backend, task_id_generator)
 
         self.url = url
         self._loop = loop
@@ -91,23 +94,26 @@
         self._exchange_type = exchange_type
         self._qos = qos
         self._declare_exchange = declare_exchange
         self._declare_queues = declare_queues
         self._queue_name = queue_name
         self._routing_key = routing_key
         self._max_priority = max_priority
+        self._delayed_message_exchange_plugin = delayed_message_exchange_plugin
 
         self._dead_letter_queue_name = f"{queue_name}.dead_letter"
         if dead_letter_queue_name:
             self._dead_letter_queue_name = dead_letter_queue_name
 
         self._delay_queue_name = f"{queue_name}.delay"
         if delay_queue_name:
             self._delay_queue_name = delay_queue_name
 
+        self._delay_plugin_exchange_name = f"{exchange_name}.plugin_delay"
+
         self.read_conn: Optional[AbstractRobustConnection] = None
         self.write_conn: Optional[AbstractRobustConnection] = None
         self.write_channel: Optional[AbstractChannel] = None
         self.read_channel: Optional[AbstractChannel] = None
 
     async def startup(self) -> None:  # noqa: WPS217
         """Create exchange and queue on startup."""
@@ -128,17 +134,39 @@
             self.read_channel = await self.read_conn.channel()
 
         if self._declare_exchange:
             await self.write_channel.declare_exchange(
                 self._exchange_name,
                 type=self._exchange_type,
             )
+
+        if self._delayed_message_exchange_plugin:
+            await self.write_channel.declare_exchange(
+                self._delay_plugin_exchange_name,
+                type=ExchangeType.X_DELAYED_MESSAGE,
+                arguments={
+                    "x-delayed-type": "direct",
+                },
+            )
+
         if self._declare_queues:
             await self.declare_queues(self.write_channel)
 
+    async def shutdown(self) -> None:
+        """Close all connections on shutdown."""
+        await super().shutdown()
+        if self.write_channel:
+            await self.write_channel.close()
+        if self.read_channel:
+            await self.read_channel.close()
+        if self.write_conn:
+            await self.write_conn.close()
+        if self.read_conn:
+            await self.read_conn.close()
+
     async def declare_queues(
         self,
         channel: AbstractChannel,
     ) -> AbstractQueue:
         """
         This function is used to declare queues.
 
@@ -159,22 +187,32 @@
         }
         if self._max_priority is not None:
             args["x-max-priority"] = self._max_priority
         queue = await channel.declare_queue(
             self._queue_name,
             arguments=args,
         )
-        await channel.declare_queue(
-            self._delay_queue_name,
-            arguments={
-                "x-dead-letter-exchange": "",
-                "x-dead-letter-routing-key": self._queue_name,
-            },
+        if self._delayed_message_exchange_plugin:
+            await queue.bind(
+                exchange=self._delay_plugin_exchange_name,
+                routing_key=self._routing_key,
+            )
+        else:
+            await channel.declare_queue(
+                self._delay_queue_name,
+                arguments={
+                    "x-dead-letter-exchange": "",
+                    "x-dead-letter-routing-key": self._queue_name,
+                },
+            )
+
+        await queue.bind(
+            exchange=self._exchange_name,
+            routing_key=self._routing_key,
         )
-        await queue.bind(exchange=self._exchange_name, routing_key=self._routing_key)
         return queue
 
     async def kick(self, message: BrokerMessage) -> None:
         """
         Send message to the exchange.
 
         This function constructs rmq message
@@ -185,36 +223,52 @@
         as the task_name.
 
         :raises ValueError: if startup wasn't called.
         :param message: message to send.
         """
         if self.write_channel is None:
             raise ValueError("Please run startup before kicking.")
-        priority = parse_val(int, message.labels.get("priority"))
-        rmq_msg = Message(
-            body=message.message,
-            headers={
+
+        message_base_params: dict[str, Any] = {
+            "body": message.message,
+            "headers": {
                 "task_id": message.task_id,
                 "task_name": message.task_name,
                 **message.labels,
             },
-            delivery_mode=DeliveryMode.PERSISTENT,
-            priority=priority,
+            "delivery_mode": DeliveryMode.PERSISTENT,
+        }
+
+        message_base_params["priority"] = parse_val(
+            int,
+            message.labels.get("priority"),
         )
-        delay = parse_val(int, message.labels.get("delay"))
+
+        delay: Optional[int] = parse_val(int, message.labels.get("delay"))
+        rmq_message: Message = Message(**message_base_params)
+
         if delay is None:
             exchange = await self.write_channel.get_exchange(
                 self._exchange_name,
                 ensure=False,
             )
-            await exchange.publish(rmq_msg, routing_key=message.task_name)
+            await exchange.publish(rmq_message, routing_key=message.task_name)
+        elif self._delayed_message_exchange_plugin:
+            rmq_message.headers["x-delay"] = delay * 1000
+            exchange = await self.write_channel.get_exchange(
+                self._delay_plugin_exchange_name,
+            )
+            await exchange.publish(
+                rmq_message,
+                routing_key=self._routing_key,
+            )
         else:
-            rmq_msg.expiration = timedelta(seconds=delay)
+            rmq_message.expiration = timedelta(seconds=delay)
             await self.write_channel.default_exchange.publish(
-                rmq_msg,
+                rmq_message,
                 routing_key=self._delay_queue_name,
             )
 
     async def listen(self) -> AsyncGenerator[bytes, None]:
         """
         Listen to queue.
 
@@ -228,19 +282,7 @@
             raise ValueError("Call startup before starting listening.")
         await self.read_channel.set_qos(prefetch_count=self._qos)
         queue = await self.declare_queues(self.read_channel)
         async with queue.iterator() as iterator:
             async for message in iterator:
                 async with message.process():
                     yield message.body
-
-    async def shutdown(self) -> None:
-        """Close all connections on shutdown."""
-        await super().shutdown()
-        if self.write_channel:
-            await self.write_channel.close()
-        if self.read_channel:
-            await self.read_channel.close()
-        if self.write_conn:
-            await self.write_conn.close()
-        if self.read_conn:
-            await self.read_conn.close()
```

### Comparing `taskiq_aio_pika-0.2.1/PKG-INFO` & `taskiq_aio_pika-0.2.2/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,30 +1,24 @@
 Metadata-Version: 2.1
 Name: taskiq-aio-pika
-Version: 0.2.1
+Version: 0.2.2
 Summary: RabbitMQ broker for taskiq
 Home-page: https://github.com/taskiq-python/taskiq-aio-pika
 Keywords: taskiq,tasks,distributed,async,aio-pika
 Author: Pavel Kirilin
 Author-email: win10@list.ru
 Requires-Python: >=3.7,<4.0
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
-Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3 :: Only
-Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.11
-Classifier: Programming Language :: Python :: 3.7
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
 Requires-Dist: aio-pika (>=9.0,<10.0)
 Requires-Dist: taskiq (>=0,<1)
 Project-URL: Repository, https://github.com/taskiq-python/taskiq-aio-pika
 Description-Content-Type: text/markdown
 
 # AioPika broker for taskiq
 
@@ -44,17 +38,21 @@
 
 ## Non-obvious things
 
 You can send delayed messages and set priorities to messages using labels.
 
 ## Delays
 
+### **Default retries**
+
 To send delayed message, you have to specify
 delay label. You can do it with `task` decorator,
-or by using kicker. For example:
+or by using kicker.  
+In this type of delay we are using additional queue with `expiration` parameter and after with time message will be deleted from `delay` queue and sent to the main taskiq queue.
+For example:
 
 ```python
 broker = AioPikaBroker()
 
 @broker.task(delay=3)
 async def delayed_task() -> int:
     return 1
@@ -72,14 +70,44 @@
     # This message is going to be send immediately. Since we deleted the label.
     await delayed_task.kicker().with_labels(delay=None).kiq()
 
     # Of course the delay is managed by rabbitmq, so you don't
     # have to wait delay period before message is going to be sent.
 ```
 
+### **Retries with `rabbitmq-delayed-message-exchange` plugin**
+
+To send delayed message you can install `rabbitmq-delayed-message-exchange`
+plugin https://github.com/rabbitmq/rabbitmq-delayed-message-exchange.
+
+And you need to configure you broker.
+There is `delayed_message_exchange_plugin` `AioPikaBroker` parameter and it must be `True` to turn on delayed message functionality.  
+
+The delay plugin can handle tasks with different delay times well, and the delay based on dead letter queue is suitable for tasks with the same delay time.  
+For example:
+
+```python
+broker = AioPikaBroker(
+    delayed_message_exchange_plugin=True,
+)
+
+@broker.task(delay=3)
+async def delayed_task() -> int:
+    return 1
+
+async def main():
+    await broker.startup()
+    # This message will be received by workers
+    # After 3 seconds delay.
+    await delayed_task.kiq()
+
+    # This message is going to be received after the delay in 4 seconds.
+    # Since we overriden the `delay` label using kicker.
+    await delayed_task.kicker().with_labels(delay=4).kiq()
+```
 
 ## Priorities
 
 You can define priorities for messages using `priority` label.
 Messages with higher priorities are delivered faster.
 But to use priorities you need to define `max_priority` of the main queue, by passing `max_priority` parameter in broker's init.
 This parameter sets maximum priority for the queue and
```

