# Comparing `tmp/aksharify-2.2.5.tar.gz` & `tmp/aksharify-2.2.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aksharify-2.2.5.tar", last modified: Sun May 21 09:23:44 2023, max compression
+gzip compressed data, was "aksharify-2.2.7.tar", last modified: Sun May 21 16:11:40 2023, max compression
```

## Comparing `aksharify-2.2.5.tar` & `aksharify-2.2.7.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxrwx   0        0        0        0 2023-05-21 09:23:44.165078 aksharify-2.2.5/
--rw-rw-rw-   0        0        0     1094 2023-05-09 13:06:55.000000 aksharify-2.2.5/LICENSE.md
--rw-rw-rw-   0        0        0     4709 2023-05-21 09:23:44.163038 aksharify-2.2.5/PKG-INFO
--rw-rw-rw-   0        0        0     4193 2023-05-11 14:40:43.000000 aksharify-2.2.5/README.md
--rw-rw-rw-   0        0        0      622 2023-05-21 09:22:31.000000 aksharify-2.2.5/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-05-21 09:23:44.165078 aksharify-2.2.5/setup.cfg
-drwxrwxrwx   0        0        0        0 2023-05-21 09:23:44.086470 aksharify-2.2.5/src/
--rw-rw-rw-   0        0        0        0 2023-05-09 16:00:52.000000 aksharify-2.2.5/src/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-21 09:23:44.158620 aksharify-2.2.5/src/aksharify.egg-info/
--rw-rw-rw-   0        0        0     4709 2023-05-21 09:23:44.000000 aksharify-2.2.5/src/aksharify.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      252 2023-05-21 09:23:44.000000 aksharify-2.2.5/src/aksharify.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-21 09:23:44.000000 aksharify-2.2.5/src/aksharify.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        7 2023-05-21 09:23:44.000000 aksharify-2.2.5/src/aksharify.egg-info/requires.txt
--rw-rw-rw-   0        0        0       19 2023-05-21 09:23:44.000000 aksharify-2.2.5/src/aksharify.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     3169 2023-05-21 08:47:16.000000 aksharify-2.2.5/src/aksharify.py
+drwxrwxrwx   0        0        0        0 2023-05-21 16:11:40.617824 aksharify-2.2.7/
+-rw-rw-rw-   0        0        0     1094 2023-05-09 13:06:55.000000 aksharify-2.2.7/LICENSE.md
+-rw-rw-rw-   0        0        0     4709 2023-05-21 16:11:40.616203 aksharify-2.2.7/PKG-INFO
+-rw-rw-rw-   0        0        0     4193 2023-05-11 14:40:43.000000 aksharify-2.2.7/README.md
+-rw-rw-rw-   0        0        0      622 2023-05-21 16:09:15.000000 aksharify-2.2.7/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-05-21 16:11:40.618964 aksharify-2.2.7/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-05-21 16:11:40.552981 aksharify-2.2.7/src/
+-rw-rw-rw-   0        0        0        0 2023-05-09 16:00:52.000000 aksharify-2.2.7/src/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-21 16:11:40.612457 aksharify-2.2.7/src/aksharify.egg-info/
+-rw-rw-rw-   0        0        0     4709 2023-05-21 16:11:40.000000 aksharify-2.2.7/src/aksharify.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      252 2023-05-21 16:11:40.000000 aksharify-2.2.7/src/aksharify.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-21 16:11:40.000000 aksharify-2.2.7/src/aksharify.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        7 2023-05-21 16:11:40.000000 aksharify-2.2.7/src/aksharify.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       19 2023-05-21 16:11:40.000000 aksharify-2.2.7/src/aksharify.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     3203 2023-05-21 16:03:49.000000 aksharify-2.2.7/src/aksharify.py
```

### Comparing `aksharify-2.2.5/LICENSE.md` & `aksharify-2.2.7/LICENSE.md`

 * *Files identical despite different names*

### Comparing `aksharify-2.2.5/PKG-INFO` & `aksharify-2.2.7/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aksharify
-Version: 2.2.5
+Version: 2.2.7
 Summary: Ascii art module
 Author-email: Prime Patel <primespatel@gmail.com>
 Project-URL: Homepage, https://github.com/primepatel/aksharify
 Project-URL: Bug Tracker, https://github.com/primepatel/aksharify/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: aksharify Version: 2.2.5 Summary: Ascii art module
+Metadata-Version: 2.1 Name: aksharify Version: 2.2.7 Summary: Ascii art module
 Author-email: Prime Patel
 gmail.com> Project-URL: Homepage, https://github.com/primepatel/aksharify
 Project-URL: Bug Tracker, https://github.com/primepatel/aksharify/issues
 Classifier: Programming Language :: Python :: 3 Classifier: License :: OSI
 Approved :: MIT License Classifier: Operating System :: OS Independent
 Requires-Python: >=3.8 Description-Content-Type: text/markdown License-File:
 LICENSE.md  # __Aksharify__ [![Contributors][contributors-shield]]
```

### Comparing `aksharify-2.2.5/README.md` & `aksharify-2.2.7/README.md`

 * *Files identical despite different names*

### Comparing `aksharify-2.2.5/pyproject.toml` & `aksharify-2.2.7/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "aksharify"
-version = "2.2.5"
+version = "2.2.7"
 authors = [
     {name="Prime Patel", email = "primespatel@gmail.com"}
 ]
 description = "Ascii art module"
 readme = "README.md"
 requires-python = ">=3.8"
```

### Comparing `aksharify-2.2.5/src/aksharify.egg-info/PKG-INFO` & `aksharify-2.2.7/src/aksharify.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aksharify
-Version: 2.2.5
+Version: 2.2.7
 Summary: Ascii art module
 Author-email: Prime Patel <primespatel@gmail.com>
 Project-URL: Homepage, https://github.com/primepatel/aksharify
 Project-URL: Bug Tracker, https://github.com/primepatel/aksharify/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: aksharify Version: 2.2.5 Summary: Ascii art module
+Metadata-Version: 2.1 Name: aksharify Version: 2.2.7 Summary: Ascii art module
 Author-email: Prime Patel
 gmail.com> Project-URL: Homepage, https://github.com/primepatel/aksharify
 Project-URL: Bug Tracker, https://github.com/primepatel/aksharify/issues
 Classifier: Programming Language :: Python :: 3 Classifier: License :: OSI
 Approved :: MIT License Classifier: Operating System :: OS Independent
 Requires-Python: >=3.8 Description-Content-Type: text/markdown License-File:
 LICENSE.md  # __Aksharify__ [![Contributors][contributors-shield]]
```

### Comparing `aksharify-2.2.5/src/aksharify.py` & `aksharify-2.2.7/src/aksharify.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,86 +1,88 @@
 from PIL import Image
 
+
 class TextArt:
     def __init__(self, image) -> None:
         self.image = Image.open(image)
         self.w, self.h = self.image.size
         self.ascii_chars = list('01')
         self.ascii_text = ''
         self.ascii_html = ''
 
-    def set_dim(self, width=0, hight=0):
-        if width == 0 and hight != 0:
-            self.w, self.h = int(self.w/self.h * hight), hight
-        elif width != 0 and hight == 0:
-            self.w, self.h = width, int(self.h/self.w * width)
+    def set_dim(self, width=0, height=0):
+        if width != 0 and height == 0:
+            self.w, self.h = width, int((self.h/self.w * width)/2.143)
+        elif width == 0 and height != 0:
+            self.w, self.h = int((self.w/self.h * height)*2.143), height
         else:
-            self.w, self.h = width, hight
+            self.w, self.h = width, height
         self.image = self.image.resize((self.w, self.h))
 
     def binary_to_decimal(self, binary):
         decimal = 0
         l = len(binary)
         for x in binary:
             l -= 1
             decimal += pow(2, l) * int(x)
         return int(decimal)
 
     def span(self, integer, integer_colour):
         return f"<span style='color: rgb{integer_colour};'><b>{integer}</b></span>"
-    
+
     def asciify(self):
         self.ascii_text = ""
         div = 255//(len(self.ascii_chars))
         bwdata = self.image.convert('L').getdata()
         for line_no in range(self.h):
             for pixel in range(line_no*self.w, line_no*self.w + self.w):
-                self.ascii_text += self.ascii_chars[bwdata[pixel]//div -1]
-    
+                self.ascii_text += self.ascii_chars[bwdata[pixel]//div - 1]
+
     def numberify(self, first_char=0):
         for i in self.ascii_chars:
             if not i.isnumeric():
                 raise TypeError
         self.asciify()
         if first_char != 0:
             self.ascii_text = str(first_char) + self.ascii_text[1:]
         return self.ascii_text
-    
+
     def primify(self, prime, asis=True, func=bin):
         if not asis and len(bin(int(prime))) == len(func(self.ascii_text)):
             self.ascii_text = func(int(prime))
         elif len(str(int(prime))) == len(self.ascii_text):
             self.ascii_text = str(prime)
         else:
             print("not primified")
-    
+
     def replace(self, text, position):
-        self.ascii_text = self.ascii_text[:position]+ text + self.ascii_text[position+len(text):]
-    
+        self.ascii_text = self.ascii_text[:position] + \
+            text + self.ascii_text[position+len(text):]
+
     def colorify(self):
         color = self.image.getdata()
-        if self.ascii_text[:2]=="0b":
+        if self.ascii_text[:2] == "0b":
             self.ascii_text = self.ascii_text[2:]
-        file = '<p style="font-family: monospace;">'
+        file = '<p style="font-size: 10px; font-family: monospace;">'
         for line_no in range(self.h):
             for pixel in range(line_no*self.w, line_no*self.w + self.w):
                 file += self.span(self.ascii_text[pixel], color[pixel])
             file += '<br>'
         file += "</p>"
         self.ascii_html = file
-    
+
     def ascii_show(self):
         text = ""
         for line_no in range(self.h):
             text += self.ascii_text[line_no*self.w:line_no*self.w + self.w] + "\n"
         print(text)
 
     def text_output(self, fname):
         text = ""
         for line_no in range(self.h):
             text += self.ascii_text[line_no*self.w:line_no*self.w + self.w] + "\n"
         with open(fname + ".txt", "w") as file:
             file.write(text)
-    
+
     def color_output(self, fname):
         with open(fname + ".html", "w") as file:
-            file.write(self.ascii_html)
+            file.write(self.ascii_html)
```

