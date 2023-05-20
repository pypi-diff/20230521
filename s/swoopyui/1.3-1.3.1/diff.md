# Comparing `tmp/swoopyui-1.3.tar.gz` & `tmp/swoopyui-1.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "swoopyui-1.3.tar", last modified: Sat May 20 13:26:18 2023, max compression
+gzip compressed data, was "swoopyui-1.3.1.tar", last modified: Sat May 20 23:05:00 2023, max compression
```

## Comparing `swoopyui-1.3.tar` & `swoopyui-1.3.1.tar`

### file list

```diff
@@ -1,38 +1,38 @@
-drwxr-xr-x   0 yousifaladwani   (501) staff       (20)        0 2023-05-20 13:26:18.307115 swoopyui-1.3/
--rw-r--r--   0 yousifaladwani   (501) staff       (20)     1060 2023-05-09 17:18:40.000000 swoopyui-1.3/LICENSE
--rw-r--r--   0 yousifaladwani   (501) staff       (20)      125 2023-05-20 08:58:40.000000 swoopyui-1.3/MANIFEST.in
--rw-r--r--   0 yousifaladwani   (501) staff       (20)     1562 2023-05-20 13:26:18.306967 swoopyui-1.3/PKG-INFO
--rw-r--r--   0 yousifaladwani   (501) staff       (20)     1156 2023-05-20 13:25:27.000000 swoopyui-1.3/README.md
--rw-r--r--   0 yousifaladwani   (501) staff       (20)      103 2023-05-07 15:22:15.000000 swoopyui-1.3/pyproject.toml
--rw-r--r--   0 yousifaladwani   (501) staff       (20)       38 2023-05-20 13:26:18.307159 swoopyui-1.3/setup.cfg
--rw-r--r--   0 yousifaladwani   (501) staff       (20)      762 2023-05-20 13:26:07.000000 swoopyui-1.3/setup.py
-drwxr-xr-x   0 yousifaladwani   (501) staff       (20)        0 2023-05-20 13:26:18.303586 swoopyui-1.3/swoopyui/
-drwxr-xr-x   0 yousifaladwani   (501) staff       (20)        0 2023-05-20 13:26:18.304571 swoopyui-1.3/swoopyui/UIkits/
--rw-r--r--   0 yousifaladwani   (501) staff       (20)        0 2023-05-20 12:59:35.000000 swoopyui-1.3/swoopyui/UIkits/__init__.py
--rw-r--r--   0 yousifaladwani   (501) staff       (20)      301 2023-05-20 12:59:35.000000 swoopyui-1.3/swoopyui/__init__.py
-drwxr-xr-x   0 yousifaladwani   (501) staff       (20)        0 2023-05-20 13:26:18.304870 swoopyui-1.3/swoopyui/assets/
--rw-r--r--   0 yousifaladwani   (501) staff       (20)        0 2023-05-20 12:59:35.000000 swoopyui-1.3/swoopyui/assets/__init__.py
--rw-r--r--   0 yousifaladwani   (501) staff       (20)   442407 2023-05-20 12:59:35.000000 swoopyui-1.3/swoopyui/assets/swoopyui.zip
--rw-r--r--   0 yousifaladwani   (501) staff       (20)      632 2023-05-20 12:59:35.000000 swoopyui-1.3/swoopyui/protocol.py
--rw-r--r--   0 yousifaladwani   (501) staff       (20)     3313 2023-05-20 12:59:35.000000 swoopyui-1.3/swoopyui/swoopyui.py
-drwxr-xr-x   0 yousifaladwani   (501) staff       (20)        0 2023-05-20 13:26:18.305872 swoopyui-1.3/swoopyui/tools/
--rw-r--r--   0 yousifaladwani   (501) staff       (20)        0 2023-05-20 12:59:35.000000 swoopyui-1.3/swoopyui/tools/__init__.py
--rw-r--r--   0 yousifaladwani   (501) staff       (20)      146 2023-05-20 12:59:35.000000 swoopyui-1.3/swoopyui/tools/on_action.py
--rw-r--r--   0 yousifaladwani   (501) staff       (20)      815 2023-05-20 12:59:35.000000 swoopyui-1.3/swoopyui/tools/run_swiftUI.py
--rw-r--r--   0 yousifaladwani   (501) staff       (20)      266 2023-05-20 12:59:35.000000 swoopyui-1.3/swoopyui/tools/run_target.py
--rw-r--r--   0 yousifaladwani   (501) staff       (20)      351 2023-05-20 12:59:35.000000 swoopyui-1.3/swoopyui/tools/unzip_assets.py
--rw-r--r--   0 yousifaladwani   (501) staff       (20)     2165 2023-05-20 12:59:35.000000 swoopyui-1.3/swoopyui/view.py
-drwxr-xr-x   0 yousifaladwani   (501) staff       (20)        0 2023-05-20 13:26:18.306753 swoopyui-1.3/swoopyui/views/
--rw-r--r--   0 yousifaladwani   (501) staff       (20)        0 2023-05-20 12:59:35.000000 swoopyui-1.3/swoopyui/views/__init__.py
--rw-r--r--   0 yousifaladwani   (501) staff       (20)     4068 2023-05-20 12:59:35.000000 swoopyui-1.3/swoopyui/views/button.py
--rw-r--r--   0 yousifaladwani   (501) staff       (20)     2817 2023-05-20 12:59:35.000000 swoopyui-1.3/swoopyui/views/navigationlink.py
--rw-r--r--   0 yousifaladwani   (501) staff       (20)     2948 2023-05-20 12:59:35.000000 swoopyui-1.3/swoopyui/views/navigationstack.py
--rw-r--r--   0 yousifaladwani   (501) staff       (20)     2982 2023-05-20 12:59:35.000000 swoopyui-1.3/swoopyui/views/navigationview.py
--rw-r--r--   0 yousifaladwani   (501) staff       (20)     2515 2023-05-20 12:59:35.000000 swoopyui-1.3/swoopyui/views/text.py
--rw-r--r--   0 yousifaladwani   (501) staff       (20)     4432 2023-05-20 12:59:35.000000 swoopyui-1.3/swoopyui/views/textfield.py
-drwxr-xr-x   0 yousifaladwani   (501) staff       (20)        0 2023-05-20 13:26:18.304258 swoopyui-1.3/swoopyui.egg-info/
--rw-r--r--   0 yousifaladwani   (501) staff       (20)     1562 2023-05-20 13:26:18.000000 swoopyui-1.3/swoopyui.egg-info/PKG-INFO
--rw-r--r--   0 yousifaladwani   (501) staff       (20)      725 2023-05-20 13:26:18.000000 swoopyui-1.3/swoopyui.egg-info/SOURCES.txt
--rw-r--r--   0 yousifaladwani   (501) staff       (20)        1 2023-05-20 13:26:18.000000 swoopyui-1.3/swoopyui.egg-info/dependency_links.txt
--rw-r--r--   0 yousifaladwani   (501) staff       (20)       15 2023-05-20 13:26:18.000000 swoopyui-1.3/swoopyui.egg-info/requires.txt
--rw-r--r--   0 yousifaladwani   (501) staff       (20)        9 2023-05-20 13:26:18.000000 swoopyui-1.3/swoopyui.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 23:05:00.515981 swoopyui-1.3.1/
+-rw-r--r--   0 runner    (1001) docker     (123)     1060 2023-05-20 23:04:49.000000 swoopyui-1.3.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      125 2023-05-20 23:04:49.000000 swoopyui-1.3.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     1721 2023-05-20 23:05:00.515981 swoopyui-1.3.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1313 2023-05-20 23:04:49.000000 swoopyui-1.3.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      103 2023-05-20 23:04:49.000000 swoopyui-1.3.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-20 23:05:00.515981 swoopyui-1.3.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      764 2023-05-20 23:04:49.000000 swoopyui-1.3.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 23:05:00.515981 swoopyui-1.3.1/swoopyui/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 23:05:00.515981 swoopyui-1.3.1/swoopyui/UIkits/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-20 23:04:49.000000 swoopyui-1.3.1/swoopyui/UIkits/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      301 2023-05-20 23:04:49.000000 swoopyui-1.3.1/swoopyui/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 23:05:00.515981 swoopyui-1.3.1/swoopyui/assets/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-20 23:04:49.000000 swoopyui-1.3.1/swoopyui/assets/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)   280787 2023-05-20 23:04:49.000000 swoopyui-1.3.1/swoopyui/assets/swoopyui.zip
+-rw-r--r--   0 runner    (1001) docker     (123)      632 2023-05-20 23:04:49.000000 swoopyui-1.3.1/swoopyui/protocol.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3440 2023-05-20 23:04:49.000000 swoopyui-1.3.1/swoopyui/swoopyui.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 23:05:00.515981 swoopyui-1.3.1/swoopyui/tools/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-20 23:04:49.000000 swoopyui-1.3.1/swoopyui/tools/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      146 2023-05-20 23:04:49.000000 swoopyui-1.3.1/swoopyui/tools/on_action.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1027 2023-05-20 23:04:49.000000 swoopyui-1.3.1/swoopyui/tools/run_swiftUI.py
+-rw-r--r--   0 runner    (1001) docker     (123)      266 2023-05-20 23:04:49.000000 swoopyui-1.3.1/swoopyui/tools/run_target.py
+-rw-r--r--   0 runner    (1001) docker     (123)      351 2023-05-20 23:04:49.000000 swoopyui-1.3.1/swoopyui/tools/unzip_assets.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2165 2023-05-20 23:04:49.000000 swoopyui-1.3.1/swoopyui/view.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 23:05:00.515981 swoopyui-1.3.1/swoopyui/views/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-20 23:04:49.000000 swoopyui-1.3.1/swoopyui/views/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4171 2023-05-20 23:04:49.000000 swoopyui-1.3.1/swoopyui/views/button.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2906 2023-05-20 23:04:49.000000 swoopyui-1.3.1/swoopyui/views/navigationlink.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3015 2023-05-20 23:04:49.000000 swoopyui-1.3.1/swoopyui/views/navigationstack.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2982 2023-05-20 23:04:49.000000 swoopyui-1.3.1/swoopyui/views/navigationview.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2391 2023-05-20 23:04:49.000000 swoopyui-1.3.1/swoopyui/views/text.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4432 2023-05-20 23:04:49.000000 swoopyui-1.3.1/swoopyui/views/textfield.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 23:05:00.515981 swoopyui-1.3.1/swoopyui.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1721 2023-05-20 23:05:00.000000 swoopyui-1.3.1/swoopyui.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      725 2023-05-20 23:05:00.000000 swoopyui-1.3.1/swoopyui.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-20 23:05:00.000000 swoopyui-1.3.1/swoopyui.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       15 2023-05-20 23:05:00.000000 swoopyui-1.3.1/swoopyui.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-05-20 23:05:00.000000 swoopyui-1.3.1/swoopyui.egg-info/top_level.txt
```

### Comparing `swoopyui-1.3/LICENSE` & `swoopyui-1.3.1/LICENSE`

 * *Files identical despite different names*

### Comparing `swoopyui-1.3/PKG-INFO` & `swoopyui-1.3.1/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: swoopyui
-Version: 1.3
+Version: 1.3.1
 Summary: A python library that allow you to build swiftUI apps using python.
 Home-page: https://github.com/SKbarbon/swoopyui
 Author: SKbarbon
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: MacOS :: MacOS X
 Classifier: Operating System :: Microsoft :: Windows
 Description-Content-Type: text/markdown
@@ -14,14 +14,20 @@
 A simple python library that allow you to build swiftUI apps using python.
 
 ## How does it work ?
 This library works by running python and swift at the same time!. It start a python localhost at the background and run swiftUI app that show the fron-end by communicating with python back-end host. But you should NOT worry about all of that, becuase the library always making sure that everything stay easy, simple and pythonic.
 
 ## installation
 
+Enter this on terminal to install this package:
+
+```zsh
+pip install swoopyui --upgrade
+```
+
 
 ## usage and examples
 To make sure that you are not OVERTHINKING about the ease of this, Check this simple `hello, world` app:
 
 ```python
 from swoopyui import View, Text, app
 
@@ -29,17 +35,18 @@
     view.add(Text("Hello, world!"))
 
 app(target=main, base_name=__name__)
 ```
 
 Are you ok now 🙃 ? fine lets start:
 
-- If you here now, the docs are on the way soon 🙂..
+- [The docs](https://github.com/SKbarbon/swoopyui/wiki)
 
-## help and contribute wanted ⚠️!!
+## ⚠️ help and contribute wanted!!
 Hi, read the docs, be master at this, it will be quick and easy..
 
 I want help with:
 - Supporting iOS, we need to support iOS and iPadOS, so if you can help with this.
 - Find a way to pack this library into `.app`, and fix the problem with most of packing packages.
+- Add a secure connection strategy between the host and client.
 
 Thanks, good luck..
```

### Comparing `swoopyui-1.3/README.md` & `swoopyui-1.3.1/README.md`

 * *Files 13% similar despite different names*

```diff
@@ -2,14 +2,20 @@
 A simple python library that allow you to build swiftUI apps using python.
 
 ## How does it work ?
 This library works by running python and swift at the same time!. It start a python localhost at the background and run swiftUI app that show the fron-end by communicating with python back-end host. But you should NOT worry about all of that, becuase the library always making sure that everything stay easy, simple and pythonic.
 
 ## installation
 
+Enter this on terminal to install this package:
+
+```zsh
+pip install swoopyui --upgrade
+```
+
 
 ## usage and examples
 To make sure that you are not OVERTHINKING about the ease of this, Check this simple `hello, world` app:
 
 ```python
 from swoopyui import View, Text, app
 
@@ -17,17 +23,18 @@
     view.add(Text("Hello, world!"))
 
 app(target=main, base_name=__name__)
 ```
 
 Are you ok now 🙃 ? fine lets start:
 
-- If you here now, the docs are on the way soon 🙂..
+- [The docs](https://github.com/SKbarbon/swoopyui/wiki)
 
-## help and contribute wanted ⚠️!!
+## ⚠️ help and contribute wanted!!
 Hi, read the docs, be master at this, it will be quick and easy..
 
 I want help with:
 - Supporting iOS, we need to support iOS and iPadOS, so if you can help with this.
 - Find a way to pack this library into `.app`, and fix the problem with most of packing packages.
+- Add a secure connection strategy between the host and client.
 
 Thanks, good luck..
```

### Comparing `swoopyui-1.3/setup.py` & `swoopyui-1.3.1/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup, find_packages
 
 with open("README.md", encoding="utf-8") as f:
     long_des = str(f.read())
 
 setup(
     name='swoopyui',
-    version='1.3',
+    version='1.3.1',
     author='SKbarbon',
     description='A python library that allow you to build swiftUI apps using python.',
     long_description=long_des,
     long_description_content_type='text/markdown',
     url='https://github.com/SKbarbon/swoopyui',
     install_requires=["flask", "requests"],
     packages=find_packages(),
```

### Comparing `swoopyui-1.3/swoopyui/protocol.py` & `swoopyui-1.3.1/swoopyui/protocol.py`

 * *Files identical despite different names*

### Comparing `swoopyui-1.3/swoopyui/swoopyui.py` & `swoopyui-1.3.1/swoopyui/swoopyui.py`

 * *Files 4% similar despite different names*

```diff
@@ -68,15 +68,18 @@
             if update_name == "on_view_action":
                 self.__main_view.manage_on_view_action(json_data.get("update_content"))
             return ""
 
         
         @flask_app.route("/close_the_app")
         def close_the_app ():
-            shutil.rmtree(self.current_tmp_dir)
+            # Remove the temporary dir
+            if os.path.isdir (self.current_tmp_dir):
+                shutil.rmtree(self.current_tmp_dir)
+            # exit the script.
             os._exit(0)
 
         with socketserver.TCPServer(("localhost", 0), None) as s:
             free_port = s.server_address[1]
         
         self.current_tmp_dir = tempfile.mkdtemp()
         threading.Thread(target=run_swiftUI_on_new_process, args=[free_port, self.current_tmp_dir]).start()
```

### Comparing `swoopyui-1.3/swoopyui/tools/run_swiftUI.py` & `swoopyui-1.3.1/swoopyui/tools/run_swiftUI.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,24 +1,30 @@
 import subprocess
 import os
 import shutil
 from .unzip_assets import unzip_file
 
 def run_swiftUI_app(port, tmp_dir):
+    # get the current temporary folder.
     temp_dir = tmp_dir
-    print(f"tmp exist: {os.path.isdir(temp_dir)}")
 
+    # Prepare paths
     zip_path = str(__file__).replace("tools/run_swiftUI.py", "assets/swoopyui.zip")
     new_app_path = os.path.join(temp_dir, "swoopyui.app/")
 
+    # unzip the app on the temporary folder
     unzip_file(zip_path=zip_path, destination_path=temp_dir)
 
+    # prepare the commands
     executable_of_the_app = os.path.join(new_app_path, "Contents/MacOS/swoopyui")
     chmod_command = ["chmod", "+x", executable_of_the_app]
 
+    # run the `chmod` command
     subprocess.run(chmod_command, stdout=subprocess.DEVNULL, stderr=subprocess.DEVNULL)
 
+    # run the command the will start the swiftUI app
     run_command = [executable_of_the_app, str(port)]
     subprocess.run(run_command, stdout=subprocess.DEVNULL, stderr=subprocess.DEVNULL)
 
-    print(temp_dir)
-    shutil.rmtree(temp_dir)
+    # Remove the temporary dir.
+    if os.path.isdir (temp_dir):
+        shutil.rmtree(temp_dir)
```

### Comparing `swoopyui-1.3/swoopyui/view.py` & `swoopyui-1.3.1/swoopyui/view.py`

 * *Files identical despite different names*

### Comparing `swoopyui-1.3/swoopyui/views/button.py` & `swoopyui-1.3.1/swoopyui/views/button.py`

 * *Files 12% similar despite different names*

```diff
@@ -44,14 +44,15 @@
         if self.__mother_view == None:
             self.__mother_view = mother_view
         
         if self.__parent_view == None:
             self.__parent_view = parent
     
     def add (self, *sub_view):
+        """Add new subviews to present the button. If there is no subviews the `text` will be used."""
         if self.__mother_view == None:
             raise Exception("Cannot add sub-views while this view not have an active mother view.")
         
         for subv in sub_view:
             subv.respown (new_id=self.__mother_view.get_new_view_id(), mother_view=self.__mother_view, parent=self)
             self.__mother_view.sub_views_history.append(subv)
             self.__subviews.append(subv)
```

### Comparing `swoopyui-1.3/swoopyui/views/navigationlink.py` & `swoopyui-1.3.1/swoopyui/views/navigationlink.py`

 * *Files 5% similar despite different names*

```diff
@@ -39,14 +39,15 @@
         if self.__mother_view == None:
             self.__mother_view = mother_view
         
         if self.__parent_view == None:
             self.__parent_view = parent
     
     def add (self, *sub_view):
+        """This will add a subview to the page that this NavigationLink is linked to."""
         if self.__mother_view == None:
             raise Exception("Cannot add sub-views while this view not have an active mother view.")
         
         for subv in sub_view:
             subv.respown (new_id=self.__mother_view.get_new_view_id(), mother_view=self.__mother_view, parent=self)
             self.__mother_view.sub_views_history.append(subv)
             self.__subviews.append(subv)
```

### Comparing `swoopyui-1.3/swoopyui/views/navigationstack.py` & `swoopyui-1.3.1/swoopyui/views/navigationstack.py`

 * *Files 3% similar despite different names*

```diff
@@ -41,14 +41,15 @@
         if self.__mother_view == None:
             self.__mother_view = mother_view
         
         if self.__parent_view == None:
             self.__parent_view = parent
     
     def add (self, *sub_view):
+        """Add a new subview to be inside this NavigationStack."""
         if self.__mother_view == None:
             raise Exception("Cannot add sub-views while this view not have an active mother view.")
         
         for subv in sub_view:
             subv.respown (new_id=self.__mother_view.get_new_view_id(), mother_view=self.__mother_view, parent=self)
             self.__mother_view.sub_views_history.append(subv)
             self.__subviews.append(subv)
```

### Comparing `swoopyui-1.3/swoopyui/views/navigationview.py` & `swoopyui-1.3.1/swoopyui/views/navigationview.py`

 * *Files identical despite different names*

### Comparing `swoopyui-1.3/swoopyui/views/text.py` & `swoopyui-1.3.1/swoopyui/views/text.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,31 +1,29 @@
 from ..tools.on_action import on_view_action
 
 
 class Text (object):
-    def __init__(self, text, foreground_color="black", background_color="white", on_hover=None) -> None:
+    def __init__(self, text, foreground_color="primary", on_hover=None) -> None:
         self.__last_view_id = None # This is used becuase swiftUI will not know that this updated without it
         self.__id = None
         self.__mother_view = None
         self.__parent_view = None
 
         self.__text = text
         self.__foreground_color = foreground_color
-        self.__background_color = background_color
         self.on_hover = on_hover
     
 
     def get_dict_content (self):
         return {
             "last_view_id" : self.__last_view_id,
             "view_id" : self.__id,
             "vname" : "Text",
             "text" : self.__text,
-            "fgcolor" : self.__foreground_color,
-            "bgcolor" : self.__background_color
+            "fgcolor" : self.__foreground_color
         }
 
     def respown (self, new_id=None, mother_view=None, parent=None):
         if new_id == None: return
         if mother_view == None: return
         if parent == None: return
```

### Comparing `swoopyui-1.3/swoopyui/views/textfield.py` & `swoopyui-1.3.1/swoopyui/views/textfield.py`

 * *Files 0% similar despite different names*

```diff
@@ -20,15 +20,15 @@
         self.on_submit = on_submit
 
     def get_dict_content (self):
         return {
             "last_view_id" : self.__last_view_id,
             "view_id" : self.__id,
             "vname" : "TextField",
-            "Text" : self.text,
+            "text" : self.text,
             "placeholder" : self.placeholder,
             "width" : self.width,
             "height" : self.height,
             "fgcolor" : self.foreground_color
         }
     
     def respown (self, new_id=None, mother_view=None, parent=None):
```

### Comparing `swoopyui-1.3/swoopyui.egg-info/PKG-INFO` & `swoopyui-1.3.1/swoopyui.egg-info/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: swoopyui
-Version: 1.3
+Version: 1.3.1
 Summary: A python library that allow you to build swiftUI apps using python.
 Home-page: https://github.com/SKbarbon/swoopyui
 Author: SKbarbon
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: MacOS :: MacOS X
 Classifier: Operating System :: Microsoft :: Windows
 Description-Content-Type: text/markdown
@@ -14,14 +14,20 @@
 A simple python library that allow you to build swiftUI apps using python.
 
 ## How does it work ?
 This library works by running python and swift at the same time!. It start a python localhost at the background and run swiftUI app that show the fron-end by communicating with python back-end host. But you should NOT worry about all of that, becuase the library always making sure that everything stay easy, simple and pythonic.
 
 ## installation
 
+Enter this on terminal to install this package:
+
+```zsh
+pip install swoopyui --upgrade
+```
+
 
 ## usage and examples
 To make sure that you are not OVERTHINKING about the ease of this, Check this simple `hello, world` app:
 
 ```python
 from swoopyui import View, Text, app
 
@@ -29,17 +35,18 @@
     view.add(Text("Hello, world!"))
 
 app(target=main, base_name=__name__)
 ```
 
 Are you ok now 🙃 ? fine lets start:
 
-- If you here now, the docs are on the way soon 🙂..
+- [The docs](https://github.com/SKbarbon/swoopyui/wiki)
 
-## help and contribute wanted ⚠️!!
+## ⚠️ help and contribute wanted!!
 Hi, read the docs, be master at this, it will be quick and easy..
 
 I want help with:
 - Supporting iOS, we need to support iOS and iPadOS, so if you can help with this.
 - Find a way to pack this library into `.app`, and fix the problem with most of packing packages.
+- Add a secure connection strategy between the host and client.
 
 Thanks, good luck..
```

### Comparing `swoopyui-1.3/swoopyui.egg-info/SOURCES.txt` & `swoopyui-1.3.1/swoopyui.egg-info/SOURCES.txt`

 * *Files identical despite different names*

