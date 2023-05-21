# Comparing `tmp/pysolarmanv5-2.5.0.tar.gz` & `tmp/pysolarmanv5-3.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pysolarmanv5-2.5.0.tar", last modified: Wed May 10 00:00:49 2023, max compression
+gzip compressed data, was "pysolarmanv5-3.0.0.tar", last modified: Sun May 21 20:43:59 2023, max compression
```

## Comparing `pysolarmanv5-2.5.0.tar` & `pysolarmanv5-3.0.0.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 jmccrohan  (1000) jmccrohan  (1000)        0 2023-05-10 00:00:49.141669 pysolarmanv5-2.5.0/
--rw-r--r--   0 jmccrohan  (1000) jmccrohan  (1000)     1083 2023-05-09 23:59:31.000000 pysolarmanv5-2.5.0/LICENSE
--rw-r--r--   0 jmccrohan  (1000) jmccrohan  (1000)     4134 2023-05-10 00:00:49.141669 pysolarmanv5-2.5.0/PKG-INFO
--rw-r--r--   0 jmccrohan  (1000) jmccrohan  (1000)     3327 2023-05-09 23:59:31.000000 pysolarmanv5-2.5.0/README.md
--rw-r--r--   0 jmccrohan  (1000) jmccrohan  (1000)     1038 2023-05-09 23:59:31.000000 pysolarmanv5-2.5.0/pyproject.toml
-drwxr-xr-x   0 jmccrohan  (1000) jmccrohan  (1000)        0 2023-05-10 00:00:49.141669 pysolarmanv5-2.5.0/pysolarmanv5/
--rw-r--r--   0 jmccrohan  (1000) jmccrohan  (1000)      358 2023-05-09 23:59:31.000000 pysolarmanv5-2.5.0/pysolarmanv5/__init__.py
--rw-r--r--   0 jmccrohan  (1000) jmccrohan  (1000)    26107 2023-05-09 23:59:31.000000 pysolarmanv5-2.5.0/pysolarmanv5/pysolarmanv5.py
--rw-r--r--   0 jmccrohan  (1000) jmccrohan  (1000)    17728 2023-05-09 23:59:31.000000 pysolarmanv5-2.5.0/pysolarmanv5/pysolarmanv5_async.py
-drwxr-xr-x   0 jmccrohan  (1000) jmccrohan  (1000)        0 2023-05-10 00:00:49.141669 pysolarmanv5-2.5.0/pysolarmanv5.egg-info/
--rw-r--r--   0 jmccrohan  (1000) jmccrohan  (1000)     4134 2023-05-10 00:00:49.000000 pysolarmanv5-2.5.0/pysolarmanv5.egg-info/PKG-INFO
--rw-r--r--   0 jmccrohan  (1000) jmccrohan  (1000)      360 2023-05-10 00:00:49.000000 pysolarmanv5-2.5.0/pysolarmanv5.egg-info/SOURCES.txt
--rw-r--r--   0 jmccrohan  (1000) jmccrohan  (1000)        1 2023-05-10 00:00:49.000000 pysolarmanv5-2.5.0/pysolarmanv5.egg-info/dependency_links.txt
--rw-r--r--   0 jmccrohan  (1000) jmccrohan  (1000)       35 2023-05-10 00:00:49.000000 pysolarmanv5-2.5.0/pysolarmanv5.egg-info/requires.txt
--rw-r--r--   0 jmccrohan  (1000) jmccrohan  (1000)       13 2023-05-10 00:00:49.000000 pysolarmanv5-2.5.0/pysolarmanv5.egg-info/top_level.txt
--rw-r--r--   0 jmccrohan  (1000) jmccrohan  (1000)       38 2023-05-10 00:00:49.141669 pysolarmanv5-2.5.0/setup.cfg
-drwxr-xr-x   0 jmccrohan  (1000) jmccrohan  (1000)        0 2023-05-10 00:00:49.141669 pysolarmanv5-2.5.0/tests/
--rw-r--r--   0 jmccrohan  (1000) jmccrohan  (1000)     1329 2023-05-09 23:59:31.000000 pysolarmanv5-2.5.0/tests/test_aio_solarman.py
--rw-r--r--   0 jmccrohan  (1000) jmccrohan  (1000)     1061 2023-05-09 23:59:31.000000 pysolarmanv5-2.5.0/tests/test_solarman.py
+drwxr-xr-x   0 jmccrohan  (1000) jmccrohan  (1000)        0 2023-05-21 20:43:59.321368 pysolarmanv5-3.0.0/
+-rw-r--r--   0 jmccrohan  (1000) jmccrohan  (1000)     1083 2023-05-21 20:42:53.000000 pysolarmanv5-3.0.0/LICENSE
+-rw-r--r--   0 jmccrohan  (1000) jmccrohan  (1000)     4134 2023-05-21 20:43:59.321368 pysolarmanv5-3.0.0/PKG-INFO
+-rw-r--r--   0 jmccrohan  (1000) jmccrohan  (1000)     3327 2023-05-21 20:42:53.000000 pysolarmanv5-3.0.0/README.md
+-rw-r--r--   0 jmccrohan  (1000) jmccrohan  (1000)     1038 2023-05-21 20:42:53.000000 pysolarmanv5-3.0.0/pyproject.toml
+drwxr-xr-x   0 jmccrohan  (1000) jmccrohan  (1000)        0 2023-05-21 20:43:59.317368 pysolarmanv5-3.0.0/pysolarmanv5/
+-rw-r--r--   0 jmccrohan  (1000) jmccrohan  (1000)      358 2023-05-21 20:42:53.000000 pysolarmanv5-3.0.0/pysolarmanv5/__init__.py
+-rw-r--r--   0 jmccrohan  (1000) jmccrohan  (1000)    26335 2023-05-21 20:42:53.000000 pysolarmanv5-3.0.0/pysolarmanv5/pysolarmanv5.py
+-rw-r--r--   0 jmccrohan  (1000) jmccrohan  (1000)    17728 2023-05-21 20:42:53.000000 pysolarmanv5-3.0.0/pysolarmanv5/pysolarmanv5_async.py
+drwxr-xr-x   0 jmccrohan  (1000) jmccrohan  (1000)        0 2023-05-21 20:43:59.321368 pysolarmanv5-3.0.0/pysolarmanv5.egg-info/
+-rw-r--r--   0 jmccrohan  (1000) jmccrohan  (1000)     4134 2023-05-21 20:43:59.000000 pysolarmanv5-3.0.0/pysolarmanv5.egg-info/PKG-INFO
+-rw-r--r--   0 jmccrohan  (1000) jmccrohan  (1000)      360 2023-05-21 20:43:59.000000 pysolarmanv5-3.0.0/pysolarmanv5.egg-info/SOURCES.txt
+-rw-r--r--   0 jmccrohan  (1000) jmccrohan  (1000)        1 2023-05-21 20:43:59.000000 pysolarmanv5-3.0.0/pysolarmanv5.egg-info/dependency_links.txt
+-rw-r--r--   0 jmccrohan  (1000) jmccrohan  (1000)       35 2023-05-21 20:43:59.000000 pysolarmanv5-3.0.0/pysolarmanv5.egg-info/requires.txt
+-rw-r--r--   0 jmccrohan  (1000) jmccrohan  (1000)       13 2023-05-21 20:43:59.000000 pysolarmanv5-3.0.0/pysolarmanv5.egg-info/top_level.txt
+-rw-r--r--   0 jmccrohan  (1000) jmccrohan  (1000)       38 2023-05-21 20:43:59.321368 pysolarmanv5-3.0.0/setup.cfg
+drwxr-xr-x   0 jmccrohan  (1000) jmccrohan  (1000)        0 2023-05-21 20:43:59.321368 pysolarmanv5-3.0.0/tests/
+-rw-r--r--   0 jmccrohan  (1000) jmccrohan  (1000)     1329 2023-05-21 20:42:53.000000 pysolarmanv5-3.0.0/tests/test_aio_solarman.py
+-rw-r--r--   0 jmccrohan  (1000) jmccrohan  (1000)     1061 2023-05-21 20:42:53.000000 pysolarmanv5-3.0.0/tests/test_solarman.py
```

### Comparing `pysolarmanv5-2.5.0/LICENSE` & `pysolarmanv5-3.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `pysolarmanv5-2.5.0/PKG-INFO` & `pysolarmanv5-3.0.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pysolarmanv5
-Version: 2.5.0
+Version: 3.0.0
 Summary: A Python library for interacting with Solarman (IGEN-Tech) v5 based Solar Data Loggers
 Author-email: Jonathan McCrohan <jmccrohan@gmail.com>
 License: MIT License
 Project-URL: homepage, https://github.com/jmccrohan/pysolarmanv5
 Project-URL: repository, https://github.com/jmccrohan/pysolarmanv5
 Project-URL: documentation, https://pysolarmanv5.readthedocs.io/
 Project-URL: changelog, https://pysolarmanv5.readthedocs.io/en/latest/changelog.html
```

### Comparing `pysolarmanv5-2.5.0/README.md` & `pysolarmanv5-3.0.0/README.md`

 * *Files identical despite different names*

### Comparing `pysolarmanv5-2.5.0/pyproject.toml` & `pysolarmanv5-3.0.0/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "pysolarmanv5"
-version = "2.5.0"
+version = "3.0.0"
 description = "A Python library for interacting with Solarman (IGEN-Tech) v5 based Solar Data Loggers"
 readme = "README.md"
 requires-python = ">=3.8"
 license = {text = "MIT License"}
 authors = [{name = "Jonathan McCrohan", email = "jmccrohan@gmail.com"}]
 keywords = ["solarman", "igen-tech", "modbus", "solar", "inverter", "solarmanv5"]
 classifiers = [
```

### Comparing `pysolarmanv5-2.5.0/pysolarmanv5/pysolarmanv5.py` & `pysolarmanv5-3.0.0/pysolarmanv5/pysolarmanv5.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,21 +1,25 @@
 """pysolarmanv5.py"""
 import queue
 import struct
 import socket
 import logging
-import select
+import selectors
+import platform
 from threading import Thread, Event
 from multiprocessing import Queue
 from typing import Any
 from random import randrange
 
 from umodbus.client.serial import rtu
 
 
+_WIN_PLATFORM = True if platform.system() == 'Windows' else False
+
+
 class V5FrameError(Exception):
     """V5 Frame Validation Error"""
 
     pass
 
 
 class NoSocketAvailableError(Exception):
@@ -100,15 +104,15 @@
 
         if self.verbose:
             self.log.setLevel("DEBUG")
 
         self._v5_frame_def()
 
         self.sock: socket.socket = None  # noqa
-        self._poll: select.poll = None  # noqa
+        self._poll: selectors.BaseSelector = None  # noqa
         self._sock_fd: int = None  # noqa
         self._auto_reconnect = False
         self._data_queue: Queue = None  # noqa
         self._data_wanted: Event = None  # noqa
         self._reader_exit: Event = None  # noqa
         self._reader_thr: Thread = None  # noqa
         self._socket_setup(kwargs.get("socket"), kwargs.get("auto_reconnect", False))
@@ -279,17 +283,17 @@
         except TimeoutError:
             raise
 
         self.log.debug("RECD: " + v5_response.hex(" "))
         return v5_response
 
     def _data_receiver(self):
-        self._poll.register(self.sock.fileno(), select.POLLIN)
+        self._poll.register(self.sock.fileno(), selectors.EVENT_READ)
         while True:
-            events = self._poll.poll(500)
+            events = self._poll.select(.500)
             if self._reader_exit.is_set():
                 return
             for event in events:
                 # We are registered only for inbound data on a single socket,
                 # so there is no need to check the (fileno, mask) tuples
                 data = self.sock.recv(1024)
                 if data == b"":
@@ -342,20 +346,20 @@
         """
         Disconnect the socket and set a signal for the reader thread to exit
 
         :return: None
 
         """
         self._data_wanted.clear()
+        self._reader_exit.set()
         try:
             self.sock.send(b"")
             self.sock.close()
         except OSError:
             pass
-        self._reader_exit.set()
         self._reader_thr.join(0.5)
         self._poll.unregister(self._sock_fd)
 
     def _send_receive_modbus_frame(self, mb_request_frame):
         """Encodes mb_frame, sends/receives v5_frame, decodes response
 
         :param mb_request_frame: Modbus RTU frame to transmit
@@ -394,15 +398,18 @@
 
     def _socket_setup(self, sock: Any, auto_reconnect: bool):
         """Socket setup method"""
         if isinstance(sock, socket.socket) or sock is None:
             self.sock = sock if sock else self._create_socket()
             if self.sock is None:
                 raise NoSocketAvailableError("No socket available")
-            self._poll = select.poll()
+            if _WIN_PLATFORM:
+                self._poll = selectors.DefaultSelector()
+            else:
+                self._poll = selectors.PollSelector()
             self._sock_fd = self.sock.fileno()
             self._auto_reconnect = False if sock else auto_reconnect
             self._data_queue = Queue(maxsize=1)
             self._data_wanted = Event()
             self._reader_exit = Event()
             self._reader_thr = Thread(target=self._data_receiver, daemon=True)
             self._reader_thr.start()
```

### Comparing `pysolarmanv5-2.5.0/pysolarmanv5/pysolarmanv5_async.py` & `pysolarmanv5-3.0.0/pysolarmanv5/pysolarmanv5_async.py`

 * *Files identical despite different names*

### Comparing `pysolarmanv5-2.5.0/pysolarmanv5.egg-info/PKG-INFO` & `pysolarmanv5-3.0.0/pysolarmanv5.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pysolarmanv5
-Version: 2.5.0
+Version: 3.0.0
 Summary: A Python library for interacting with Solarman (IGEN-Tech) v5 based Solar Data Loggers
 Author-email: Jonathan McCrohan <jmccrohan@gmail.com>
 License: MIT License
 Project-URL: homepage, https://github.com/jmccrohan/pysolarmanv5
 Project-URL: repository, https://github.com/jmccrohan/pysolarmanv5
 Project-URL: documentation, https://pysolarmanv5.readthedocs.io/
 Project-URL: changelog, https://pysolarmanv5.readthedocs.io/en/latest/changelog.html
```

### Comparing `pysolarmanv5-2.5.0/tests/test_aio_solarman.py` & `pysolarmanv5-3.0.0/tests/test_aio_solarman.py`

 * *Files identical despite different names*

### Comparing `pysolarmanv5-2.5.0/tests/test_solarman.py` & `pysolarmanv5-3.0.0/tests/test_solarman.py`

 * *Files identical despite different names*

