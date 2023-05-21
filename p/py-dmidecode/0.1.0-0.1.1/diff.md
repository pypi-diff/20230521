# Comparing `tmp/py-dmidecode-0.1.0.tar.gz` & `tmp/py_dmidecode-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/py-dmidecode-0.1.0.tar", last modified: Thu Oct 10 06:50:46 2019, max compression
+gzip compressed data, was "py_dmidecode-0.1.1.tar", max compression
```

## Comparing `py-dmidecode-0.1.0.tar` & `py_dmidecode-0.1.1.tar`

### file list

```diff
@@ -1,11 +1,6 @@
-drwxr-xr-x   0 zaibon    (1000) zaibon    (1000)        0 2019-10-10 06:50:46.000000 py-dmidecode-0.1.0/
--rw-r--r--   0 zaibon    (1000) zaibon    (1000)     2071 2019-10-10 06:50:46.000000 py-dmidecode-0.1.0/PKG-INFO
--rw-r--r--   0 zaibon    (1000) zaibon    (1000)      941 2019-10-10 06:43:31.000000 py-dmidecode-0.1.0/README.md
--rw-r--r--   0 zaibon    (1000) zaibon    (1000)     7109 2019-10-10 06:43:56.000000 py-dmidecode-0.1.0/dmidecode.py
-drwxr-xr-x   0 zaibon    (1000) zaibon    (1000)        0 2019-10-10 06:50:46.000000 py-dmidecode-0.1.0/py_dmidecode.egg-info/
--rw-r--r--   0 zaibon    (1000) zaibon    (1000)     2071 2019-10-10 06:50:46.000000 py-dmidecode-0.1.0/py_dmidecode.egg-info/PKG-INFO
--rw-r--r--   0 zaibon    (1000) zaibon    (1000)      175 2019-10-10 06:50:46.000000 py-dmidecode-0.1.0/py_dmidecode.egg-info/SOURCES.txt
--rw-r--r--   0 zaibon    (1000) zaibon    (1000)        1 2019-10-10 06:50:46.000000 py-dmidecode-0.1.0/py_dmidecode.egg-info/dependency_links.txt
--rw-r--r--   0 zaibon    (1000) zaibon    (1000)       10 2019-10-10 06:50:46.000000 py-dmidecode-0.1.0/py_dmidecode.egg-info/top_level.txt
--rw-r--r--   0 zaibon    (1000) zaibon    (1000)       38 2019-10-10 06:50:46.000000 py-dmidecode-0.1.0/setup.cfg
--rw-r--r--   0 zaibon    (1000) zaibon    (1000)     1826 2019-10-10 06:50:32.000000 py-dmidecode-0.1.0/setup.py
+-rw-r--r--   0        0        0    11357 2019-10-06 18:35:46.000000 py_dmidecode-0.1.1/LICENSE
+-rw-r--r--   0        0        0      945 2023-05-21 17:58:12.203993 py_dmidecode-0.1.1/README.md
+-rw-r--r--   0        0        0        0 2023-05-21 17:58:12.204299 py_dmidecode-0.1.1/py_dmidecode/__init__.py
+-rw-r--r--   0        0        0     7166 2023-05-21 17:58:12.211247 py_dmidecode-0.1.1/py_dmidecode/dmidecode.py
+-rw-r--r--   0        0        0     1184 2023-05-21 17:59:04.926462 py_dmidecode-0.1.1/pyproject.toml
+-rw-r--r--   0        0        0     2090 1970-01-01 00:00:00.000000 py_dmidecode-0.1.1/PKG-INFO
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `py-dmidecode-0.1.0/PKG-INFO` & `py_dmidecode-0.1.1/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,54 +1,63 @@
 Metadata-Version: 2.1
 Name: py-dmidecode
-Version: 0.1.0
-Summary: python lib that parse the output of dmidecode 
+Version: 0.1.1
+Summary: python library to parse the output of dmidecode
 Home-page: https://github.com/zaibon/py-dmidecode
-Author: Christophe de Carvalho
-License: UNKNOWN
-Project-URL: Bug Reports, https://github.com/zaibon/py-dmidecode/issues
-Project-URL: Source, https://github.com/zaibon/py-dmidecode/
-Description: # py-dmidecode
-        
-        Small tool that parses ouput of dmidecode command
-        
-        ## How to use
-        ```python
-        from dmidecode import DMIDecode
-        import subprocess
-        
-        # create parsing instance by passing dmidecode output
-        dmi = DMIDecode()
-        
-        # some of the pre-defined queries
-        print('Manufacturer:\t', dmi.manufacturer())
-        print('Model:\t\t', dmi.model())
-        print('Firmware:\t', dmi.firmware())
-        print('Serial number:\t', dmi.serial_number())
-        print('Processor type:\t', dmi.cpu_type())
-        print('Number of CPUs:\t', dmi.cpu_num())
-        print('Cores count:\t', dmi.total_enabled_cores())
-        print('Total RAM:\t{} GB'.format(dmi.total_ram()))
-        ```
-        
-        Alternatively instead of running dmidecode locally you can use DMIParse by passing dmidecode output as an argument:
-        ```python
-        from dmidecode import DMIParse
-        dmi = DMIParse(raw)
-        ```
-        
-        Other information can be easily retrieved by analyzing dmi.data and module code.
-        
-        ## Possible limitations
-        Tested with dmidecode versions 2.11, 2.12 and 3.2
-        
 Keywords: system development
-Platform: UNKNOWN
+Author: Christophe de Carvalho
+Author-email: christophe.dcpm@gmail.com
+Requires-Python: >=3.8.1,<4.0
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
-Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.4
-Classifier: Programming Language :: Python :: 3.5
-Classifier: Programming Language :: Python :: 3.6
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Topic :: Software Development :: Libraries :: Python Modules
+Project-URL: Bug Tracker, https://github.com/zaibon/py-dmidecode/issues
+Project-URL: Repository, https://github.com/zaibon/py-dmidecode
 Description-Content-Type: text/markdown
+
+# py-dmidecode
+
+Small tool that parses output of dmidecode command
+
+## How to use
+
+```python
+from dmidecode import DMIDecode
+import subprocess
+
+# create parsing instance by passing dmidecode output
+dmi = DMIDecode()
+
+# some of the pre-defined queries
+print('Manufacturer:\t', dmi.manufacturer())
+print('Model:\t\t', dmi.model())
+print('Firmware:\t', dmi.firmware())
+print('Serial number:\t', dmi.serial_number())
+print('Processor type:\t', dmi.cpu_type())
+print('Number of CPUs:\t', dmi.cpu_num())
+print('Cores count:\t', dmi.total_enabled_cores())
+print('Total RAM:\t{} GB'.format(dmi.total_ram()))
+```
+
+Alternatively instead of running dmidecode locally you can use DMIParse by passing dmidecode output as an argument:
+
+```python
+from dmidecode import DMIParse
+dmi = DMIParse(raw)
+```
+
+Other information can be easily retrieved by analyzing dmi.data and module code.
+
+## Possible limitations
+
+Tested with dmidecode versions 2.11, 2.12 and 3.2
+
```

### Comparing `py-dmidecode-0.1.0/README.md` & `py_dmidecode-0.1.1/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 # py-dmidecode
 
-Small tool that parses ouput of dmidecode command
+Small tool that parses output of dmidecode command
 
 ## How to use
+
 ```python
 from dmidecode import DMIDecode
 import subprocess
 
 # create parsing instance by passing dmidecode output
 dmi = DMIDecode()
 
@@ -18,16 +19,18 @@
 print('Processor type:\t', dmi.cpu_type())
 print('Number of CPUs:\t', dmi.cpu_num())
 print('Cores count:\t', dmi.total_enabled_cores())
 print('Total RAM:\t{} GB'.format(dmi.total_ram()))
 ```
 
 Alternatively instead of running dmidecode locally you can use DMIParse by passing dmidecode output as an argument:
+
 ```python
 from dmidecode import DMIParse
 dmi = DMIParse(raw)
 ```
 
 Other information can be easily retrieved by analyzing dmi.data and module code.
 
 ## Possible limitations
+
 Tested with dmidecode versions 2.11, 2.12 and 3.2
```

### Comparing `py-dmidecode-0.1.0/dmidecode.py` & `py_dmidecode-0.1.1/py_dmidecode/dmidecode.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,17 +4,17 @@
 
 class DMIParse:
     """
     dmidecode information parsing object
     requires dmidecode output as input string
     """
 
-    def __init__(self, str, default="n/a"):
+    def __init__(self, dmidecode_output, default="n/a"):
         self.default = default
-        self.data = self.dmidecode_parse(str)
+        self.data = self.dmidecode_parse(dmidecode_output)
 
     def get(self, type_id):
         if isinstance(type_id, str):
             for type_num, type_str in self.type2str.items():
                 if type_str == type_id:
                     type_id = type_num
 
@@ -144,15 +144,14 @@
 
             #  Loop over the rest of the record, gathering values
             for i in range(2, len(record_element), 1):
                 if i >= len(record_element):
                     break
                 #  Check whether we are inside a \t\t block
                 if in_block_elemet != "":
-
                     in_block_data = DMIDecode.in_block_re.findall(record_element[1])
 
                     if in_block_data:
                         if not in_block_list:
                             in_block_list = in_block_data[0][0]
                         else:
                             in_block_list = in_block_list + "\t\t"
@@ -178,24 +177,24 @@
                 if record_data2:
                     #  This is an array of data - let the loop know we are
                     #  inside an array block
                     in_block_elemet = record_data2[0][0]
                     continue
         return data
 
-    def size_to_gb(self, str):
+    def size_to_gb(self, value):
         """Convert dmidecode memory size description to GB"""
-        nb = re.search("[0-9]+", str)
+        nb = re.search("[0-9]+", value)
         if nb:
-            nb = int(re.search("[0-9]+", str).group())
+            nb = int(re.search("[0-9]+", value).group())
         else:
             return 0
-        if "MB" in str:
+        if "MB" in value:
             return nb / 1024 if nb else 0
-        elif "GB" in str:
+        elif "GB" in value:
             return nb
         else:
             return 0
 
 
 class DMIDecode(DMIParse):
     """Wrapper over DMIParse which runs dmidecode locally"""
@@ -203,13 +202,13 @@
     def __init__(self, command="dmidecode"):
         self.dmidecode = command
         raw = self._run()
         super().__init__(raw)
 
     def _run(self):
         # let subprocess merge stderr with stdout
-        proc = subprocess.Popen(self.dmidecode, stderr=subprocess.STDOUT, stdout=subprocess.PIPE)
-        stdout, stderr = proc.communicate()
-        if proc.returncode > 0:
-            raise RuntimeError("{} failed with an error:\n{}".format(self.dmidecode, stdout.decode()))
-        else:
-            return stdout.decode()
+        with subprocess.Popen(self.dmidecode, stderr=subprocess.STDOUT, stdout=subprocess.PIPE) as proc:
+            stdout, _ = proc.communicate()
+            if proc.returncode > 0:
+                raise RuntimeError("{} failed with an error:\n{}".format(self.dmidecode, stdout.decode()))
+            else:
+                return stdout.decode()
```

