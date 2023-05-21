# Comparing `tmp/QtLogger-1.0.2-py3-none-any.whl.zip` & `tmp/QtLogger-1.0.3-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,11 +1,11 @@
-Zip file size: 6174 bytes, number of entries: 9
+Zip file size: 6176 bytes, number of entries: 9
 -rw-rw-rw-  2.0 fat       28 b- defN 23-Apr-17 16:09 QtLogger/__init__.py
 -rw-rw-rw-  2.0 fat     2561 b- defN 23-May-20 09:53 QtLogger/__main__.py
--rw-rw-rw-  2.0 fat     9748 b- defN 23-May-20 09:55 QtLogger/base.py
+-rw-rw-rw-  2.0 fat     9761 b- defN 23-May-21 12:13 QtLogger/base.py
 -rw-rw-rw-  2.0 fat      152 b- defN 23-Apr-18 07:00 QtLogger/exceptions.py
 -rw-rw-rw-  2.0 fat      180 b- defN 23-Apr-18 07:21 QtLogger/warnings.py
--rw-rw-rw-  2.0 fat     1973 b- defN 23-May-20 10:23 QtLogger-1.0.2.dist-info/METADATA
--rw-rw-rw-  2.0 fat       92 b- defN 23-May-20 10:23 QtLogger-1.0.2.dist-info/WHEEL
--rw-rw-rw-  2.0 fat        9 b- defN 23-May-20 10:23 QtLogger-1.0.2.dist-info/top_level.txt
-?rw-rw-r--  2.0 fat      680 b- defN 23-May-20 10:23 QtLogger-1.0.2.dist-info/RECORD
-9 files, 15423 bytes uncompressed, 5008 bytes compressed:  67.5%
+-rw-rw-rw-  2.0 fat     1973 b- defN 23-May-21 12:14 QtLogger-1.0.3.dist-info/METADATA
+-rw-rw-rw-  2.0 fat       92 b- defN 23-May-21 12:14 QtLogger-1.0.3.dist-info/WHEEL
+-rw-rw-rw-  2.0 fat        9 b- defN 23-May-21 12:14 QtLogger-1.0.3.dist-info/top_level.txt
+?rw-rw-r--  2.0 fat      680 b- defN 23-May-21 12:14 QtLogger-1.0.3.dist-info/RECORD
+9 files, 15436 bytes uncompressed, 5010 bytes compressed:  67.5%
```

## zipnote {}

```diff
@@ -9,20 +9,20 @@
 
 Filename: QtLogger/exceptions.py
 Comment: 
 
 Filename: QtLogger/warnings.py
 Comment: 
 
-Filename: QtLogger-1.0.2.dist-info/METADATA
+Filename: QtLogger-1.0.3.dist-info/METADATA
 Comment: 
 
-Filename: QtLogger-1.0.2.dist-info/WHEEL
+Filename: QtLogger-1.0.3.dist-info/WHEEL
 Comment: 
 
-Filename: QtLogger-1.0.2.dist-info/top_level.txt
+Filename: QtLogger-1.0.3.dist-info/top_level.txt
 Comment: 
 
-Filename: QtLogger-1.0.2.dist-info/RECORD
+Filename: QtLogger-1.0.3.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## QtLogger/base.py

```diff
@@ -58,15 +58,15 @@
         self._setup_ui()
 
 
     def _setup_ui(self):
         self.lay = QGridLayout(self)
         self.logger_view = QTextEdit(self)
         self.logger_view.setReadOnly(True)
-        self.logger_view.setLineWrapMode(QTextEdit.NoWrap)
+        self.logger_view.setLineWrapMode(QTextEdit.LineWrapMode.NoWrap)
 
         # Highlight things like these
         # [DEBUG]-[time]-[module]: message <--- This one is purple
         # [INFO]-[time]-[module]: message <--- This one is blue
         # [WARNING]-[time]-[module]: message <--- This one is yellow
         # [ERROR]-[time]-[module]: message <--- This one is red
         # [SUCCESS]-[time]-[module]: message <--- This one is green
```

## Comparing `QtLogger-1.0.2.dist-info/METADATA` & `QtLogger-1.0.3.dist-info/METADATA`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: QtLogger
-Version: 1.0.2
+Version: 1.0.3
 Summary: A simple logger for PyQt6 that also has a nice UI
 Home-page: https://github.com/Advik-B/PyQt-Logger
 Author: Advik
 Author-email: <advik.b@gmail.com>
 Keywords: Logger,Qt,PyQt,Qt6,PyQt6,QtLogger
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
```

