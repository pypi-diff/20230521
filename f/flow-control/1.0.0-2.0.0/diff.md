# Comparing `tmp/flow_control-1.0.0.tar.gz` & `tmp/flow_control-2.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\flow_control-1.0.0.tar", last modified: Fri Jan 10 13:42:59 2020, max compression
+gzip compressed data, was "flow_control-2.0.0.tar", last modified: Sun May 21 12:37:39 2023, max compression
```

## Comparing `flow_control-1.0.0.tar` & `flow_control-2.0.0.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxrwxrwx   0        0        0        0 2020-01-10 13:42:59.000000 flow_control-1.0.0/
--rw-rw-rw-   0        0        0     2191 2020-01-10 13:42:59.000000 flow_control-1.0.0/PKG-INFO
--rw-rw-rw-   0        0        0     1412 2020-01-10 13:13:14.000000 flow_control-1.0.0/README.md
-drwxrwxrwx   0        0        0        0 2020-01-10 13:42:59.000000 flow_control-1.0.0/flow_control/
--rw-rw-rw-   0        0        0       98 2020-01-10 12:52:22.000000 flow_control-1.0.0/flow_control/__init__.py
--rw-rw-rw-   0        0        0     2269 2020-01-10 12:52:22.000000 flow_control-1.0.0/flow_control/controller.py
--rw-rw-rw-   0        0        0      935 2020-01-10 13:35:09.000000 flow_control-1.0.0/flow_control/test.py
-drwxrwxrwx   0        0        0        0 2020-01-10 13:42:59.000000 flow_control-1.0.0/flow_control.egg-info/
--rw-rw-rw-   0        0        0     2191 2020-01-10 13:42:58.000000 flow_control-1.0.0/flow_control.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      235 2020-01-10 13:42:58.000000 flow_control-1.0.0/flow_control.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2020-01-10 13:42:58.000000 flow_control-1.0.0/flow_control.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       13 2020-01-10 13:42:58.000000 flow_control-1.0.0/flow_control.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2020-01-10 13:42:59.000000 flow_control-1.0.0/setup.cfg
--rw-rw-rw-   0        0        0      739 2020-01-10 13:16:32.000000 flow_control-1.0.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-21 12:37:39.314151 flow_control-2.0.0/
+-rw-rw-rw-   0        0        0     1951 2023-05-21 12:37:39.313150 flow_control-2.0.0/PKG-INFO
+-rw-rw-rw-   0        0        0     1485 2023-05-21 12:35:36.000000 flow_control-2.0.0/README.md
+drwxrwxrwx   0        0        0        0 2023-05-21 12:37:39.303141 flow_control-2.0.0/flow_control/
+-rw-rw-rw-   0        0        0      205 2023-05-21 12:18:13.000000 flow_control-2.0.0/flow_control/__init__.py
+-rw-rw-rw-   0        0        0     3894 2023-05-21 12:18:13.000000 flow_control-2.0.0/flow_control/controller.py
+-rw-rw-rw-   0        0        0     1891 2023-05-21 12:25:45.000000 flow_control-2.0.0/flow_control/test.py
+drwxrwxrwx   0        0        0        0 2023-05-21 12:37:39.312149 flow_control-2.0.0/flow_control.egg-info/
+-rw-rw-rw-   0        0        0     1951 2023-05-21 12:37:38.000000 flow_control-2.0.0/flow_control.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      235 2023-05-21 12:37:39.000000 flow_control-2.0.0/flow_control.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-21 12:37:38.000000 flow_control-2.0.0/flow_control.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       13 2023-05-21 12:37:38.000000 flow_control-2.0.0/flow_control.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-05-21 12:37:39.314151 flow_control-2.0.0/setup.cfg
+-rw-rw-rw-   0        0        0      739 2023-05-21 11:54:56.000000 flow_control-2.0.0/setup.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `flow_control-1.0.0/PKG-INFO` & `flow_control-2.0.0/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,53 +1,53 @@
 Metadata-Version: 2.1
 Name: flow_control
-Version: 1.0.0
+Version: 2.0.0
 Summary: A flow control packages,control QPS
 Home-page: https://github.com/mt6979/flow_control
 Author: liuyancong
 Author-email: 1437255447@qq.com
 License: UNKNOWN
-Description: #                                                             Flow Control
-        
-        - 功能 
-          - 这个packages可以控制每秒一个函数或者语句的调用次数，可以设置访问次数和时间间隔，
-          - 访问限制 访问次数/时间间隔
-        
-        - 使用方法(单进程情况下使用FlowControl 类，多进程情况下使用ProcessFlowControl类)
-        
-          ```Python
-          #encoding=utf-8
-          import os
-          import threading
-          
-          from datetime import datetime
-          from flow_control.controller import FlowControl
-          from flow_control.controller import ProcessFlowControl
-          from threading import Thread
-        
-          
-          
-          def work(flowcontrol):
-              while True:
-                  if flowcontrol.get():
-                      print("{}--{}--{}".format(os.getpid(), threading.currentThread().ident, datetime.now()))
-          
-          flow_control = FlowControl(num=1, interval=1)
-          Thread(target=work, args=(flow_control,)).start()
-          work(flow_control)
-          ```
-        
-          
-        
-          
-        
-          - 创建一个FlowControl (单进程情况下)或者 ProcessFlowControl(多进程情况下) 对象，参数为(num=访问次数,interval=时间间隔)，
-          - num的类型应该为int类型，interval应该为int或者float类型
-          - 然后调用该对象的 get方法
-          - 如果get方法返回 True，则说明可以未达到流控限制，如果返回False则说明函数调用次数或者访问次数已经 达到流控限制，应该拒绝调用或访问
-        
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
-Requires-Python: >=3.5
+Requires-Python: >=2.7
 Description-Content-Type: text/markdown
+
+#                                                             Flow Control
+
+- 功能 
+  - 这个packages可以控制间隔固定的时间一个函数或者语句的调用次数(QPS)，可以设置访问次数和时间间隔，
+  - 访问限制 访问次数/时间间隔
+
+- 使用方法(单进程情况下使用FlowControl 类，多进程情况下使用ProcessFlowControl类)
+
+  ```Python
+  # encoding=utf-8
+  import os
+  import threading
+  
+  from datetime import datetime
+  from flow_control.controller import FlowController
+  from flow_control.controller import ProcessFlowController
+  from flow_control.controller import AverageFlowControl
+  from flow_control.controller import AverageProcessFlowControl
+  from threading import Thread
+
+  
+  
+  def work(flowcontrol):
+      while True:
+          if flowcontrol.get():
+              print("{}--{}--{}".format(os.getpid(), threading.currentThread().ident, datetime.now()))
+  
+  flow_control = AverageFlowControl(num=0.5, interval=1)
+  Thread(target=work, args=(flow_control,)).start()
+  work(flow_control)
+  ```
+
+
+  - 创建一个FlowControl (单进程情况下)或者 ProcessFlowControl(多进程情况下) 对象，参数为(num=访问次数,interval=时间间隔)，
+  - 然后调用该对象的 get方法
+  - 如果get方法返回 True，则说明可以未达到流控限制，如果返回False则说明函数调用次数或者访问次数已经 达到流控限制，应该拒绝调用或访问
+
+
```

### Comparing `flow_control-1.0.0/README.md` & `flow_control-2.0.0/README.md`

 * *Files 12% similar despite different names*

```diff
@@ -1,38 +1,36 @@
 #                                                             Flow Control
 
 - 功能 
-  - 这个packages可以控制每秒一个函数或者语句的调用次数，可以设置访问次数和时间间隔，
+  - 这个packages可以控制间隔固定的时间一个函数或者语句的调用次数(QPS)，可以设置访问次数和时间间隔，
   - 访问限制 访问次数/时间间隔
 
 - 使用方法(单进程情况下使用FlowControl 类，多进程情况下使用ProcessFlowControl类)
 
   ```Python
-  #encoding=utf-8
+  # encoding=utf-8
   import os
   import threading
   
   from datetime import datetime
-  from flow_control.controller import FlowControl
-  from flow_control.controller import ProcessFlowControl
+  from flow_control.controller import FlowController
+  from flow_control.controller import ProcessFlowController
+  from flow_control.controller import AverageFlowControl
+  from flow_control.controller import AverageProcessFlowControl
   from threading import Thread
 
   
   
   def work(flowcontrol):
       while True:
           if flowcontrol.get():
               print("{}--{}--{}".format(os.getpid(), threading.currentThread().ident, datetime.now()))
   
-  flow_control = FlowControl(num=1, interval=1)
+  flow_control = AverageFlowControl(num=0.5, interval=1)
   Thread(target=work, args=(flow_control,)).start()
   work(flow_control)
   ```
 
-  
-
-  
 
   - 创建一个FlowControl (单进程情况下)或者 ProcessFlowControl(多进程情况下) 对象，参数为(num=访问次数,interval=时间间隔)，
-  - num的类型应该为int类型，interval应该为int或者float类型
   - 然后调用该对象的 get方法
   - 如果get方法返回 True，则说明可以未达到流控限制，如果返回False则说明函数调用次数或者访问次数已经 达到流控限制，应该拒绝调用或访问
```

### Comparing `flow_control-1.0.0/flow_control.egg-info/PKG-INFO` & `flow_control-2.0.0/flow_control.egg-info/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,53 +1,53 @@
 Metadata-Version: 2.1
 Name: flow-control
-Version: 1.0.0
+Version: 2.0.0
 Summary: A flow control packages,control QPS
 Home-page: https://github.com/mt6979/flow_control
 Author: liuyancong
 Author-email: 1437255447@qq.com
 License: UNKNOWN
-Description: #                                                             Flow Control
-        
-        - 功能 
-          - 这个packages可以控制每秒一个函数或者语句的调用次数，可以设置访问次数和时间间隔，
-          - 访问限制 访问次数/时间间隔
-        
-        - 使用方法(单进程情况下使用FlowControl 类，多进程情况下使用ProcessFlowControl类)
-        
-          ```Python
-          #encoding=utf-8
-          import os
-          import threading
-          
-          from datetime import datetime
-          from flow_control.controller import FlowControl
-          from flow_control.controller import ProcessFlowControl
-          from threading import Thread
-        
-          
-          
-          def work(flowcontrol):
-              while True:
-                  if flowcontrol.get():
-                      print("{}--{}--{}".format(os.getpid(), threading.currentThread().ident, datetime.now()))
-          
-          flow_control = FlowControl(num=1, interval=1)
-          Thread(target=work, args=(flow_control,)).start()
-          work(flow_control)
-          ```
-        
-          
-        
-          
-        
-          - 创建一个FlowControl (单进程情况下)或者 ProcessFlowControl(多进程情况下) 对象，参数为(num=访问次数,interval=时间间隔)，
-          - num的类型应该为int类型，interval应该为int或者float类型
-          - 然后调用该对象的 get方法
-          - 如果get方法返回 True，则说明可以未达到流控限制，如果返回False则说明函数调用次数或者访问次数已经 达到流控限制，应该拒绝调用或访问
-        
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
-Requires-Python: >=3.5
+Requires-Python: >=2.7
 Description-Content-Type: text/markdown
+
+#                                                             Flow Control
+
+- 功能 
+  - 这个packages可以控制间隔固定的时间一个函数或者语句的调用次数(QPS)，可以设置访问次数和时间间隔，
+  - 访问限制 访问次数/时间间隔
+
+- 使用方法(单进程情况下使用FlowControl 类，多进程情况下使用ProcessFlowControl类)
+
+  ```Python
+  # encoding=utf-8
+  import os
+  import threading
+  
+  from datetime import datetime
+  from flow_control.controller import FlowController
+  from flow_control.controller import ProcessFlowController
+  from flow_control.controller import AverageFlowControl
+  from flow_control.controller import AverageProcessFlowControl
+  from threading import Thread
+
+  
+  
+  def work(flowcontrol):
+      while True:
+          if flowcontrol.get():
+              print("{}--{}--{}".format(os.getpid(), threading.currentThread().ident, datetime.now()))
+  
+  flow_control = AverageFlowControl(num=0.5, interval=1)
+  Thread(target=work, args=(flow_control,)).start()
+  work(flow_control)
+  ```
+
+
+  - 创建一个FlowControl (单进程情况下)或者 ProcessFlowControl(多进程情况下) 对象，参数为(num=访问次数,interval=时间间隔)，
+  - 然后调用该对象的 get方法
+  - 如果get方法返回 True，则说明可以未达到流控限制，如果返回False则说明函数调用次数或者访问次数已经 达到流控限制，应该拒绝调用或访问
+
+
```

### Comparing `flow_control-1.0.0/setup.py` & `flow_control-2.0.0/setup.py`

 * *Files 21% similar despite different names*

```diff
@@ -2,22 +2,22 @@
 import setuptools
 
 with open("README.md", "r",encoding='utf-8') as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="flow_control", # Replace with your own username
-    version="1.0.0",
+    version="2.0.0",
     author="liuyancong",
     author_email="1437255447@qq.com",
     description="A flow control packages,control QPS",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/mt6979/flow_control",
     packages=setuptools.find_packages(),
     classifiers=[
         "Programming Language :: Python :: 3",
         "License :: OSI Approved :: MIT License",
         "Operating System :: OS Independent",
     ],
-    python_requires='>=3.5',
+    python_requires='>=2.7',
 )
```

