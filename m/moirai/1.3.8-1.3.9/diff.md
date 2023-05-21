# Comparing `tmp/moirai-1.3.8.tar.gz` & `tmp/moirai-1.3.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/moirai-1.3.8.tar", last modified: Fri Jul 12 16:54:10 2019, max compression
+gzip compressed data, was "dist/moirai-1.3.9.tar", last modified: Wed Nov  6 13:25:19 2019, max compression
```

## Comparing `moirai-1.3.8.tar` & `moirai-1.3.9.tar`

### file list

```diff
@@ -1,39 +1,39 @@
-drwx------   0 Alan       (501) staff       (20)        0 2019-07-12 16:54:10.000000 moirai-1.3.8/
--rw-------   0 Alan       (501) staff       (20)     1061 2016-09-29 20:53:48.000000 moirai-1.3.8/LICENSE
--rw-------   0 Alan       (501) staff       (20)       34 2016-10-27 12:28:11.000000 moirai-1.3.8/MANIFEST.in
--rw-------   0 Alan       (501) staff       (20)     4152 2019-07-12 16:54:10.000000 moirai-1.3.8/PKG-INFO
--rw-------   0 Alan       (501) staff       (20)     2862 2018-08-20 12:17:11.000000 moirai-1.3.8/README.md
-drwx------   0 Alan       (501) staff       (20)        0 2019-07-12 16:54:10.000000 moirai-1.3.8/moirai/
--rw-------   0 Alan       (501) staff       (20)     1388 2019-07-12 16:53:58.000000 moirai-1.3.8/moirai/__init__.py
--rwx------   0 Alan       (501) staff       (20)     1189 2018-08-17 14:42:30.000000 moirai-1.3.8/moirai/__main__.py
--rwx------   0 Alan       (501) staff       (20)     5429 2019-02-12 14:18:45.000000 moirai-1.3.8/moirai/abstract_process_handler.py
-drwx------   0 Alan       (501) staff       (20)        0 2019-07-12 16:54:10.000000 moirai-1.3.8/moirai/database/
--rwx------   0 Alan       (501) staff       (20)     2482 2018-08-17 14:45:59.000000 moirai-1.3.8/moirai/database/__init__.py
--rwx------   0 Alan       (501) staff       (20)     8276 2019-07-12 16:42:35.000000 moirai-1.3.8/moirai/database/mongodb.py
--rwx------   0 Alan       (501) staff       (20)    15479 2019-07-12 16:42:35.000000 moirai-1.3.8/moirai/database/mysql.py
--rwx------   0 Alan       (501) staff       (20)     3699 2018-08-20 11:34:41.000000 moirai-1.3.8/moirai/decorators.py
-drwx------   0 Alan       (501) staff       (20)        0 2019-07-12 16:54:10.000000 moirai-1.3.8/moirai/hardware/
--rwx------   0 Alan       (501) staff       (20)     4168 2019-02-12 14:18:45.000000 moirai-1.3.8/moirai/hardware/__init__.py
--rwx------   0 Alan       (501) staff       (20)     2706 2019-02-12 14:18:45.000000 moirai-1.3.8/moirai/hardware/cmd_processor.py
--rwx------   0 Alan       (501) staff       (20)     4753 2019-02-27 17:43:34.000000 moirai-1.3.8/moirai/hardware/configured_hardware.py
--rwx------   0 Alan       (501) staff       (20)     9541 2019-03-06 22:45:59.000000 moirai-1.3.8/moirai/hardware/controller.py
--rwx------   0 Alan       (501) staff       (20)     6085 2019-03-06 22:45:59.000000 moirai-1.3.8/moirai/hardware/free.py
--rwx------   0 Alan       (501) staff       (20)     4963 2019-07-12 16:42:35.000000 moirai-1.3.8/moirai/hardware/model_simulation.py
--rwx------   0 Alan       (501) staff       (20)     6810 2019-03-06 22:45:59.000000 moirai-1.3.8/moirai/hardware/pid.py
--rwx------   0 Alan       (501) staff       (20)     4583 2019-03-06 22:45:59.000000 moirai-1.3.8/moirai/hardware/system_response_tests.py
--rwx------   0 Alan       (501) staff       (20)     1876 2018-08-17 14:44:22.000000 moirai-1.3.8/moirai/hardware/timer.py
--rwx------   0 Alan       (501) staff       (20)    13506 2019-03-09 19:22:44.000000 moirai-1.3.8/moirai/installer.py
--rwx------   0 Alan       (501) staff       (20)     8367 2019-07-12 16:53:58.000000 moirai-1.3.8/moirai/moirai.py
-drwx------   0 Alan       (501) staff       (20)        0 2019-07-12 16:54:10.000000 moirai-1.3.8/moirai/webapi/
--rwx------   0 Alan       (501) staff       (20)     2230 2018-08-20 12:17:11.000000 moirai-1.3.8/moirai/webapi/__init__.py
--rwx------   0 Alan       (501) staff       (20)    25992 2019-03-06 22:45:59.000000 moirai-1.3.8/moirai/webapi/api.py
--rwx------   0 Alan       (501) staff       (20)     1941 2018-08-20 11:50:24.000000 moirai-1.3.8/moirai/webapi/cmd_processor.py
-drwx------   0 Alan       (501) staff       (20)        0 2019-07-12 16:54:10.000000 moirai-1.3.8/moirai.egg-info/
--rw-------   0 Alan       (501) staff       (20)     4152 2019-07-12 16:54:09.000000 moirai-1.3.8/moirai.egg-info/PKG-INFO
--rw-------   0 Alan       (501) staff       (20)      798 2019-07-12 16:54:09.000000 moirai-1.3.8/moirai.egg-info/SOURCES.txt
--rw-------   0 Alan       (501) staff       (20)        1 2019-07-12 16:54:09.000000 moirai-1.3.8/moirai.egg-info/dependency_links.txt
--rw-------   0 Alan       (501) staff       (20)       48 2019-07-12 16:54:09.000000 moirai-1.3.8/moirai.egg-info/entry_points.txt
--rw-------   0 Alan       (501) staff       (20)       63 2019-07-12 16:54:09.000000 moirai-1.3.8/moirai.egg-info/requires.txt
--rw-------   0 Alan       (501) staff       (20)        7 2019-07-12 16:54:09.000000 moirai-1.3.8/moirai.egg-info/top_level.txt
--rw-------   0 Alan       (501) staff       (20)       79 2019-07-12 16:54:10.000000 moirai-1.3.8/setup.cfg
--rwx------   0 Alan       (501) staff       (20)     3318 2019-03-06 22:45:59.000000 moirai-1.3.8/setup.py
+drwx------   0 Alan       (501) staff       (20)        0 2019-11-06 13:25:19.000000 moirai-1.3.9/
+-rw-------   0 Alan       (501) staff       (20)     1061 2016-09-29 20:53:48.000000 moirai-1.3.9/LICENSE
+-rw-------   0 Alan       (501) staff       (20)       34 2016-10-27 12:28:11.000000 moirai-1.3.9/MANIFEST.in
+-rw-------   0 Alan       (501) staff       (20)     4152 2019-11-06 13:25:19.000000 moirai-1.3.9/PKG-INFO
+-rw-------   0 Alan       (501) staff       (20)     2862 2018-08-20 12:17:11.000000 moirai-1.3.9/README.md
+drwx------   0 Alan       (501) staff       (20)        0 2019-11-06 13:25:19.000000 moirai-1.3.9/moirai/
+-rw-------   0 Alan       (501) staff       (20)     1388 2019-11-06 13:24:49.000000 moirai-1.3.9/moirai/__init__.py
+-rwx------   0 Alan       (501) staff       (20)     1189 2018-08-17 14:42:30.000000 moirai-1.3.9/moirai/__main__.py
+-rwx------   0 Alan       (501) staff       (20)     5429 2019-02-12 14:18:45.000000 moirai-1.3.9/moirai/abstract_process_handler.py
+drwx------   0 Alan       (501) staff       (20)        0 2019-11-06 13:25:19.000000 moirai-1.3.9/moirai/database/
+-rwx------   0 Alan       (501) staff       (20)     2482 2018-08-17 14:45:59.000000 moirai-1.3.9/moirai/database/__init__.py
+-rwx------   0 Alan       (501) staff       (20)     8276 2019-07-12 16:42:35.000000 moirai-1.3.9/moirai/database/mongodb.py
+-rwx------   0 Alan       (501) staff       (20)    15479 2019-07-12 16:42:35.000000 moirai-1.3.9/moirai/database/mysql.py
+-rwx------   0 Alan       (501) staff       (20)     3699 2018-08-20 11:34:41.000000 moirai-1.3.9/moirai/decorators.py
+drwx------   0 Alan       (501) staff       (20)        0 2019-11-06 13:25:19.000000 moirai-1.3.9/moirai/hardware/
+-rwx------   0 Alan       (501) staff       (20)     4168 2019-02-12 14:18:45.000000 moirai-1.3.9/moirai/hardware/__init__.py
+-rwx------   0 Alan       (501) staff       (20)     2706 2019-02-12 14:18:45.000000 moirai-1.3.9/moirai/hardware/cmd_processor.py
+-rwx------   0 Alan       (501) staff       (20)     4753 2019-02-27 17:43:34.000000 moirai-1.3.9/moirai/hardware/configured_hardware.py
+-rwx------   0 Alan       (501) staff       (20)     9541 2019-03-06 22:45:59.000000 moirai-1.3.9/moirai/hardware/controller.py
+-rwx------   0 Alan       (501) staff       (20)     6085 2019-03-06 22:45:59.000000 moirai-1.3.9/moirai/hardware/free.py
+-rwx------   0 Alan       (501) staff       (20)     4963 2019-07-12 16:42:35.000000 moirai-1.3.9/moirai/hardware/model_simulation.py
+-rwx------   0 Alan       (501) staff       (20)     6810 2019-03-06 22:45:59.000000 moirai-1.3.9/moirai/hardware/pid.py
+-rwx------   0 Alan       (501) staff       (20)     4624 2019-11-06 13:23:28.000000 moirai-1.3.9/moirai/hardware/system_response_tests.py
+-rwx------   0 Alan       (501) staff       (20)     1876 2018-08-17 14:44:22.000000 moirai-1.3.9/moirai/hardware/timer.py
+-rwx------   0 Alan       (501) staff       (20)    13506 2019-03-09 19:22:44.000000 moirai-1.3.9/moirai/installer.py
+-rwx------   0 Alan       (501) staff       (20)     8367 2019-07-12 16:53:58.000000 moirai-1.3.9/moirai/moirai.py
+drwx------   0 Alan       (501) staff       (20)        0 2019-11-06 13:25:19.000000 moirai-1.3.9/moirai/webapi/
+-rwx------   0 Alan       (501) staff       (20)     2230 2018-08-20 12:17:11.000000 moirai-1.3.9/moirai/webapi/__init__.py
+-rwx------   0 Alan       (501) staff       (20)    25992 2019-03-06 22:45:59.000000 moirai-1.3.9/moirai/webapi/api.py
+-rwx------   0 Alan       (501) staff       (20)     1941 2018-08-20 11:50:24.000000 moirai-1.3.9/moirai/webapi/cmd_processor.py
+drwx------   0 Alan       (501) staff       (20)        0 2019-11-06 13:25:19.000000 moirai-1.3.9/moirai.egg-info/
+-rw-------   0 Alan       (501) staff       (20)     4152 2019-11-06 13:25:19.000000 moirai-1.3.9/moirai.egg-info/PKG-INFO
+-rw-------   0 Alan       (501) staff       (20)      798 2019-11-06 13:25:19.000000 moirai-1.3.9/moirai.egg-info/SOURCES.txt
+-rw-------   0 Alan       (501) staff       (20)        1 2019-11-06 13:25:19.000000 moirai-1.3.9/moirai.egg-info/dependency_links.txt
+-rw-------   0 Alan       (501) staff       (20)       48 2019-11-06 13:25:19.000000 moirai-1.3.9/moirai.egg-info/entry_points.txt
+-rw-------   0 Alan       (501) staff       (20)       63 2019-11-06 13:25:19.000000 moirai-1.3.9/moirai.egg-info/requires.txt
+-rw-------   0 Alan       (501) staff       (20)        7 2019-11-06 13:25:19.000000 moirai-1.3.9/moirai.egg-info/top_level.txt
+-rw-------   0 Alan       (501) staff       (20)       79 2019-11-06 13:25:19.000000 moirai-1.3.9/setup.cfg
+-rwx------   0 Alan       (501) staff       (20)     3318 2019-03-06 22:45:59.000000 moirai-1.3.9/setup.py
```

### Comparing `moirai-1.3.8/LICENSE` & `moirai-1.3.9/LICENSE`

 * *Files identical despite different names*

### Comparing `moirai-1.3.8/PKG-INFO` & `moirai-1.3.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: moirai
-Version: 1.3.8
+Version: 1.3.9
 Summary: Digital Control Manager Backend
 Home-page: https://www.github.com/acristoffers/moirai
 Author: Álan Crístoffer
 Author-email: acristoffers@gmail.com
 License: MIT
 Description: # moirai
```

### Comparing `moirai-1.3.8/README.md` & `moirai-1.3.9/README.md`

 * *Files identical despite different names*

### Comparing `moirai-1.3.8/moirai/__init__.py` & `moirai-1.3.9/moirai/__init__.py`

 * *Files 18% similar despite different names*

```diff
@@ -20,11 +20,11 @@
 # OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN
 # THE SOFTWARE.
 
 __author__ = 'Álan Crístoffer'
 __copyright__ = 'Copyright 2016, Álan Crístoffer'
 __credits__ = ['Álan Crístoffer']
 __license__ = 'MIT'
-__version__ = '1.3.8'
+__version__ = '1.3.9'
 __maintainer__ = 'Álan Crístoffer'
 __email__ = 'acristoffers@gmail.com'
 __status__ = 'Development'
```

### Comparing `moirai-1.3.8/moirai/__main__.py` & `moirai-1.3.9/moirai/__main__.py`

 * *Files identical despite different names*

### Comparing `moirai-1.3.8/moirai/abstract_process_handler.py` & `moirai-1.3.9/moirai/abstract_process_handler.py`

 * *Files identical despite different names*

### Comparing `moirai-1.3.8/moirai/database/__init__.py` & `moirai-1.3.9/moirai/database/__init__.py`

 * *Files identical despite different names*

### Comparing `moirai-1.3.8/moirai/database/mongodb.py` & `moirai-1.3.9/moirai/database/mongodb.py`

 * *Files identical despite different names*

### Comparing `moirai-1.3.8/moirai/database/mysql.py` & `moirai-1.3.9/moirai/database/mysql.py`

 * *Files identical despite different names*

### Comparing `moirai-1.3.8/moirai/decorators.py` & `moirai-1.3.9/moirai/decorators.py`

 * *Files identical despite different names*

### Comparing `moirai-1.3.8/moirai/hardware/__init__.py` & `moirai-1.3.9/moirai/hardware/__init__.py`

 * *Files identical despite different names*

### Comparing `moirai-1.3.8/moirai/hardware/cmd_processor.py` & `moirai-1.3.9/moirai/hardware/cmd_processor.py`

 * *Files identical despite different names*

### Comparing `moirai-1.3.8/moirai/hardware/configured_hardware.py` & `moirai-1.3.9/moirai/hardware/configured_hardware.py`

 * *Files identical despite different names*

### Comparing `moirai-1.3.8/moirai/hardware/controller.py` & `moirai-1.3.9/moirai/hardware/controller.py`

 * *Files identical despite different names*

### Comparing `moirai-1.3.8/moirai/hardware/free.py` & `moirai-1.3.9/moirai/hardware/free.py`

 * *Files identical despite different names*

### Comparing `moirai-1.3.8/moirai/hardware/model_simulation.py` & `moirai-1.3.9/moirai/hardware/model_simulation.py`

 * *Files identical despite different names*

### Comparing `moirai-1.3.8/moirai/hardware/pid.py` & `moirai-1.3.9/moirai/hardware/pid.py`

 * *Files identical despite different names*

### Comparing `moirai-1.3.8/moirai/hardware/system_response_tests.py` & `moirai-1.3.9/moirai/hardware/system_response_tests.py`

 * *Files 6% similar despite different names*

```diff
@@ -47,15 +47,16 @@
         code = compile('y=%s' % lock['expression'], '_string_', 'exec')
 
         def f(code=code, lock=lock):
             value = self.hardware.read(lock['sensor'])
             scope = {'x': value}
             exec(code, None, scope)
             if scope['y']:
-                self.hardware.write(lock['actuator'], lock['actuatorValue'])
+                value = float(lock['actuatorValue'])
+                self.hardware.write(lock['actuator'], value)
                 self.db.set_setting('test_error', 'Interlock')
                 raise Exception('Interlock')
 
         return f
 
     def run(self):
         self.db.set_setting('current_test', self.test['name'])
@@ -67,15 +68,15 @@
         for o in self.test['fixedOutputs']:
             self.hardware.write(o['alias'], o['value'])
 
         run_time = self.test['points'][-1]['x']
         interval = self.test['logRate']
         t = Timer(run_time, interval)
         ports = self.test['output']  # Can be a list.
-        ports = [ports] if type(ports) == str else ports
+        ports = [ports] if isinstance(ports, str) else ports
         start_time = datetime.datetime.utcnow()
         last_port_value = 0
         t_elapsed = 0
         graph_id = self.db.save_test(self.test['name'], start_time)
 
         try:
             while self.db.get_setting('current_test') is not None:
```

### Comparing `moirai-1.3.8/moirai/hardware/timer.py` & `moirai-1.3.9/moirai/hardware/timer.py`

 * *Files identical despite different names*

### Comparing `moirai-1.3.8/moirai/installer.py` & `moirai-1.3.9/moirai/installer.py`

 * *Files identical despite different names*

### Comparing `moirai-1.3.8/moirai/moirai.py` & `moirai-1.3.9/moirai/moirai.py`

 * *Files identical despite different names*

### Comparing `moirai-1.3.8/moirai/webapi/__init__.py` & `moirai-1.3.9/moirai/webapi/__init__.py`

 * *Files identical despite different names*

### Comparing `moirai-1.3.8/moirai/webapi/api.py` & `moirai-1.3.9/moirai/webapi/api.py`

 * *Files identical despite different names*

### Comparing `moirai-1.3.8/moirai/webapi/cmd_processor.py` & `moirai-1.3.9/moirai/webapi/cmd_processor.py`

 * *Files identical despite different names*

### Comparing `moirai-1.3.8/moirai.egg-info/PKG-INFO` & `moirai-1.3.9/moirai.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: moirai
-Version: 1.3.8
+Version: 1.3.9
 Summary: Digital Control Manager Backend
 Home-page: https://www.github.com/acristoffers/moirai
 Author: Álan Crístoffer
 Author-email: acristoffers@gmail.com
 License: MIT
 Description: # moirai
```

### Comparing `moirai-1.3.8/moirai.egg-info/SOURCES.txt` & `moirai-1.3.9/moirai.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `moirai-1.3.8/setup.py` & `moirai-1.3.9/setup.py`

 * *Files identical despite different names*

