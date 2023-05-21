# Comparing `tmp/kojo-0.16.0.tar.gz` & `tmp/kojo-0.17.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "kojo-0.16.0.tar", last modified: Fri May  5 12:16:04 2023, max compression
+gzip compressed data, was "dist/kojo-0.17.0.tar", last modified: Sun May 21 11:07:53 2023, max compression
```

## Comparing `kojo-0.16.0.tar` & `kojo-0.17.0.tar`

### file list

```diff
@@ -1,12 +1,12 @@
-drwxrwxr-x   0 olaf      (1000) olaf      (1000)        0 2023-05-05 12:16:04.481533 kojo-0.16.0/
--rw-rw-r--   0 olaf      (1000) olaf      (1000)      612 2023-05-05 12:16:04.481533 kojo-0.16.0/PKG-INFO
-drwxrwxr-x   0 olaf      (1000) olaf      (1000)        0 2023-05-05 12:16:04.481533 kojo-0.16.0/kojo/
--rw-rw-r--   0 olaf      (1000) olaf      (1000)      142 2023-04-27 08:51:59.007066 kojo-0.16.0/kojo/__init__.py
--rw-rw-r--   0 olaf      (1000) olaf      (1000)      454 2023-04-27 08:31:58.877706 kojo-0.16.0/kojo/duplicatefinder.py
--rw-rw-r--   0 olaf      (1000) olaf      (1000)     2197 2023-05-05 11:59:44.265339 kojo-0.16.0/kojo/io.py
--rw-rw-r--   0 olaf      (1000) olaf      (1000)     3455 2023-05-02 12:01:05.544818 kojo-0.16.0/kojo/item.py
--rw-rw-r--   0 olaf      (1000) olaf      (1000)      947 2023-04-28 09:56:03.337703 kojo-0.16.0/kojo/jsonschemavalidator.py
--rw-rw-r--   0 olaf      (1000) olaf      (1000)     1110 2023-05-05 12:13:22.078434 kojo-0.16.0/kojo/process.py
--rw-rw-r--   0 olaf      (1000) olaf      (1000)     1844 2023-04-27 08:31:58.877706 kojo-0.16.0/kojo/propertiesconverter.py
--rw-rw-r--   0 olaf      (1000) olaf      (1000)       39 2023-04-27 08:31:58.877706 kojo-0.16.0/setup.cfg
--rw-rw-r--   0 olaf      (1000) olaf      (1000)      743 2023-05-05 12:12:53.250550 kojo-0.16.0/setup.py
+drwxr-xr-x   0 olaf       (501) staff       (20)        0 2023-05-21 11:07:53.000000 kojo-0.17.0/
+drwxr-xr-x   0 olaf       (501) staff       (20)        0 2023-05-21 11:07:53.000000 kojo-0.17.0/kojo/
+-rw-r--r--   0 olaf       (501) staff       (20)      454 2023-05-20 06:51:50.000000 kojo-0.17.0/kojo/duplicatefinder.py
+-rw-r--r--   0 olaf       (501) staff       (20)     2188 2023-05-20 19:17:09.000000 kojo-0.17.0/kojo/io.py
+-rw-r--r--   0 olaf       (501) staff       (20)      142 2023-05-20 06:51:50.000000 kojo-0.17.0/kojo/__init__.py
+-rw-r--r--   0 olaf       (501) staff       (20)      947 2023-05-20 06:51:50.000000 kojo-0.17.0/kojo/jsonschemavalidator.py
+-rw-r--r--   0 olaf       (501) staff       (20)     1314 2023-05-21 10:39:01.000000 kojo-0.17.0/kojo/process.py
+-rw-r--r--   0 olaf       (501) staff       (20)     1844 2023-05-20 06:51:50.000000 kojo-0.17.0/kojo/propertiesconverter.py
+-rw-r--r--   0 olaf       (501) staff       (20)     4108 2023-05-20 07:57:15.000000 kojo-0.17.0/kojo/item.py
+-rw-r--r--   0 olaf       (501) staff       (20)      561 2023-05-21 11:07:53.000000 kojo-0.17.0/PKG-INFO
+-rw-r--r--   0 olaf       (501) staff       (20)      693 2023-05-21 11:02:26.000000 kojo-0.17.0/setup.py
+-rw-r--r--   0 olaf       (501) staff       (20)       39 2023-05-20 06:51:50.000000 kojo-0.17.0/setup.cfg
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive
+POSIX tar archive (GNU)
```

### Comparing `kojo-0.16.0/PKG-INFO` & `kojo-0.17.0/PKG-INFO`

 * *Files 17% similar despite different names*

```diff
@@ -1,16 +1,15 @@
 Metadata-Version: 1.1
 Name: kojo
-Version: 0.16.0
+Version: 0.17.0
 Summary: A library to transform data through a pipeline
 Home-page: https://gitlab.com/filchos/kojo
 Author: Olaf Schneider
 Author-email: mail@olafschneider.com
 License: GNU GPLv3
-Download-URL: https://gitlab.com/filchos/kojo/-/archive/0.16.0/kojo-0.16.0.tar.gz
+Download-URL: https://gitlab.com/filchos/kojo/-/archive/0.17.0/kojo-0.17.0.tar.gz
 Description: UNKNOWN
 Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.10
```

### Comparing `kojo-0.16.0/kojo/io.py` & `kojo-0.17.0/kojo/io.py`

 * *Files 6% similar despite different names*

```diff
@@ -38,15 +38,15 @@
 
 class CSVWriter:
     def write(self, iterator, filename):
         keys = []
         iter0, iter1 = itertools.tee(iterator, 2)
 
         for item in iter0:
-            k = list(filter(lambda k: k not in keys, item.keys()))
+            k = [k for k in item.keys() if k not in keys]
             keys += k
 
         with open(filename, "w") as file:
             writer = csv.writer(file)
             writer.writerow(keys)
 
             for item in iter1:
```

### Comparing `kojo-0.16.0/kojo/item.py` & `kojo-0.17.0/kojo/item.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 import copy
+import json
 import logging
 
 
 def flatten(item, prefix=""):
     flat_dict = {}
     for k, v in item.items():
         kk = k
@@ -118,7 +119,29 @@
         return item
 
     def flatten(self):
         item = Item(flatten(self))
         item.log = self.log.clone()
         item.meta = copy.copy(self.meta)
         return item
+
+    def to_json(self):
+        obj = {"data": dict(self), "logEntries": [], "meta": self.meta}
+        for entry in self.log.entries:
+            obj["logEntries"].append(
+                {
+                    "level": entry.level,
+                    "message": entry.message,
+                    "details": entry.details,
+                }
+            )
+        return json.dumps(obj)
+
+
+def from_json(j):
+    obj = json.loads(j)
+    item = Item(obj["data"])
+    item.log = ItemLog()
+    for entry in obj["logEntries"]:
+        item.log.log(entry["level"], entry["message"], **entry["details"])
+    item.meta = obj["meta"]
+    return item
```

### Comparing `kojo-0.16.0/kojo/jsonschemavalidator.py` & `kojo-0.17.0/kojo/jsonschemavalidator.py`

 * *Files identical despite different names*

### Comparing `kojo-0.16.0/kojo/propertiesconverter.py` & `kojo-0.17.0/kojo/propertiesconverter.py`

 * *Files identical despite different names*

### Comparing `kojo-0.16.0/setup.py` & `kojo-0.17.0/setup.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,23 +1,22 @@
 #!/usr/bin/env python
 
 from distutils.core import setup
 
 setup(
     name="kojo",
     packages=["kojo"],
-    version="0.16.0",
+    version="0.17.0",
     license="GNU GPLv3",
     description="A library to transform data through a pipeline",
     author="Olaf Schneider",
     author_email="mail@olafschneider.com",
     url="https://gitlab.com/filchos/kojo",
-    download_url="https://gitlab.com/filchos/kojo/-/archive/0.16.0/kojo-0.16.0.tar.gz",
+    download_url="https://gitlab.com/filchos/kojo/-/archive/0.17.0/kojo-0.17.0.tar.gz",
     install_requires=["jsonschema"],
     classifiers=[
         "Development Status :: 3 - Alpha",
         "Intended Audience :: Developers",
         "License :: OSI Approved :: GNU General Public License v3 (GPLv3)",
         "Programming Language :: Python :: 3",
-        "Programming Language :: Python :: 3.10",
     ],
 )
```

