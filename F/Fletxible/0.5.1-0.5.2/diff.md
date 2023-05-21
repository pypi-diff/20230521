# Comparing `tmp/Fletxible-0.5.1.tar.gz` & `tmp/Fletxible-0.5.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "Fletxible-0.5.1.tar", last modified: Thu May 18 15:53:22 2023, max compression
+gzip compressed data, was "Fletxible-0.5.2.tar", last modified: Sun May 21 13:02:35 2023, max compression
```

## Comparing `Fletxible-0.5.1.tar` & `Fletxible-0.5.2.tar`

### file list

```diff
@@ -1,25 +1,27 @@
-drwxr-xr-x   0 ahmad      (501) staff       (20)        0 2023-05-18 15:53:22.880722 Fletxible-0.5.1/
-drwxr-xr-x   0 ahmad      (501) staff       (20)        0 2023-05-18 15:53:22.875948 Fletxible-0.5.1/Fletxible.egg-info/
--rw-r--r--   0 ahmad      (501) staff       (20)      830 2023-05-18 15:53:22.000000 Fletxible-0.5.1/Fletxible.egg-info/PKG-INFO
--rw-r--r--   0 ahmad      (501) staff       (20)      391 2023-05-18 15:53:22.000000 Fletxible-0.5.1/Fletxible.egg-info/SOURCES.txt
--rw-r--r--   0 ahmad      (501) staff       (20)        1 2023-05-18 15:53:22.000000 Fletxible-0.5.1/Fletxible.egg-info/dependency_links.txt
--rw-r--r--   0 ahmad      (501) staff       (20)       50 2023-05-18 15:53:22.000000 Fletxible-0.5.1/Fletxible.egg-info/entry_points.txt
--rw-r--r--   0 ahmad      (501) staff       (20)       37 2023-05-18 15:53:22.000000 Fletxible-0.5.1/Fletxible.egg-info/requires.txt
--rw-r--r--   0 ahmad      (501) staff       (20)        6 2023-05-18 15:53:22.000000 Fletxible-0.5.1/Fletxible.egg-info/top_level.txt
--rw-r--r--   0 ahmad      (501) staff       (20)     1079 2023-04-29 15:25:05.000000 Fletxible-0.5.1/LICENSE
--rw-r--r--   0 ahmad      (501) staff       (20)      830 2023-05-18 15:53:22.880470 Fletxible-0.5.1/PKG-INFO
--rw-r--r--   0 ahmad      (501) staff       (20)     4106 2023-05-01 16:06:19.000000 Fletxible-0.5.1/README.md
-drwxr-xr-x   0 ahmad      (501) staff       (20)        0 2023-05-18 15:53:22.879326 Fletxible-0.5.1/logic/
--rw-r--r--   0 ahmad      (501) staff       (20)        0 2023-05-01 13:39:08.000000 Fletxible-0.5.1/logic/__init__.py
--rw-r--r--   0 ahmad      (501) staff       (20)     2251 2023-05-17 15:53:13.000000 Fletxible-0.5.1/logic/cli.py
--rw-r--r--   0 ahmad      (501) staff       (20)     7170 2023-05-17 15:50:13.000000 Fletxible-0.5.1/logic/controls.py
--rw-r--r--   0 ahmad      (501) staff       (20)      891 2023-05-18 14:26:31.000000 Fletxible-0.5.1/logic/main.py
--rw-r--r--   0 ahmad      (501) staff       (20)       68 2023-05-18 15:36:10.000000 Fletxible-0.5.1/logic/mapped.py
--rw-r--r--   0 ahmad      (501) staff       (20)      335 2023-05-18 15:36:10.000000 Fletxible-0.5.1/logic/route.py
--rw-r--r--   0 ahmad      (501) staff       (20)     6505 2023-05-16 19:07:50.000000 Fletxible-0.5.1/logic/script.py
--rw-r--r--   0 ahmad      (501) staff       (20)      908 2023-05-17 15:50:39.000000 Fletxible-0.5.1/logic/styles.py
--rw-r--r--   0 ahmad      (501) staff       (20)     5929 2023-05-18 15:36:06.000000 Fletxible-0.5.1/logic/utilities.py
--rw-r--r--   0 ahmad      (501) staff       (20)       38 2023-05-18 15:53:22.880794 Fletxible-0.5.1/setup.cfg
--rw-r--r--   0 ahmad      (501) staff       (20)     1110 2023-05-18 15:52:37.000000 Fletxible-0.5.1/setup.py
-drwxr-xr-x   0 ahmad      (501) staff       (20)        0 2023-05-18 15:53:22.879823 Fletxible-0.5.1/tests/
--rw-r--r--   0 ahmad      (501) staff       (20)        5 2023-05-01 14:25:50.000000 Fletxible-0.5.1/tests/test_route.py
+drwxr-xr-x   0 ahmad      (501) staff       (20)        0 2023-05-21 13:02:35.025517 Fletxible-0.5.2/
+drwxr-xr-x   0 ahmad      (501) staff       (20)        0 2023-05-21 13:02:35.020273 Fletxible-0.5.2/Fletxible.egg-info/
+-rw-r--r--   0 ahmad      (501) staff       (20)      830 2023-05-21 13:02:34.000000 Fletxible-0.5.2/Fletxible.egg-info/PKG-INFO
+-rw-r--r--   0 ahmad      (501) staff       (20)      429 2023-05-21 13:02:34.000000 Fletxible-0.5.2/Fletxible.egg-info/SOURCES.txt
+-rw-r--r--   0 ahmad      (501) staff       (20)        1 2023-05-21 13:02:34.000000 Fletxible-0.5.2/Fletxible.egg-info/dependency_links.txt
+-rw-r--r--   0 ahmad      (501) staff       (20)       86 2023-05-21 13:02:34.000000 Fletxible-0.5.2/Fletxible.egg-info/entry_points.txt
+-rw-r--r--   0 ahmad      (501) staff       (20)       37 2023-05-21 13:02:34.000000 Fletxible-0.5.2/Fletxible.egg-info/requires.txt
+-rw-r--r--   0 ahmad      (501) staff       (20)        6 2023-05-21 13:02:34.000000 Fletxible-0.5.2/Fletxible.egg-info/top_level.txt
+-rw-r--r--   0 ahmad      (501) staff       (20)     1079 2023-04-29 15:25:05.000000 Fletxible-0.5.2/LICENSE
+-rw-r--r--   0 ahmad      (501) staff       (20)      830 2023-05-21 13:02:35.025266 Fletxible-0.5.2/PKG-INFO
+-rw-r--r--   0 ahmad      (501) staff       (20)     4106 2023-05-01 16:06:19.000000 Fletxible-0.5.2/README.md
+drwxr-xr-x   0 ahmad      (501) staff       (20)        0 2023-05-21 13:02:35.023949 Fletxible-0.5.2/logic/
+-rw-r--r--   0 ahmad      (501) staff       (20)        0 2023-05-20 17:37:40.000000 Fletxible-0.5.2/logic/__init__.py
+-rw-r--r--   0 ahmad      (501) staff       (20)     2201 2023-05-21 12:36:22.000000 Fletxible-0.5.2/logic/build.py
+-rw-r--r--   0 ahmad      (501) staff       (20)     2251 2023-05-17 15:53:13.000000 Fletxible-0.5.2/logic/cli.py
+-rw-r--r--   0 ahmad      (501) staff       (20)     7832 2023-05-21 08:03:38.000000 Fletxible-0.5.2/logic/controls.py
+-rw-r--r--   0 ahmad      (501) staff       (20)      909 2023-05-21 12:43:58.000000 Fletxible-0.5.2/logic/main.py
+-rw-r--r--   0 ahmad      (501) staff       (20)       95 2023-05-21 08:59:30.000000 Fletxible-0.5.2/logic/mapped.py
+-rw-r--r--   0 ahmad      (501) staff       (20)      531 2023-05-21 10:41:00.000000 Fletxible-0.5.2/logic/route.py
+-rw-r--r--   0 ahmad      (501) staff       (20)     6629 2023-05-21 08:58:38.000000 Fletxible-0.5.2/logic/script.py
+-rw-r--r--   0 ahmad      (501) staff       (20)      908 2023-05-21 08:03:38.000000 Fletxible-0.5.2/logic/styles.py
+-rw-r--r--   0 ahmad      (501) staff       (20)    12162 2023-05-21 08:59:39.000000 Fletxible-0.5.2/logic/utilities.py
+-rw-r--r--   0 ahmad      (501) staff       (20)       38 2023-05-21 13:02:35.025595 Fletxible-0.5.2/setup.cfg
+-rw-r--r--   0 ahmad      (501) staff       (20)     1182 2023-05-21 12:43:45.000000 Fletxible-0.5.2/setup.py
+drwxr-xr-x   0 ahmad      (501) staff       (20)        0 2023-05-21 13:02:35.024632 Fletxible-0.5.2/tests/
+-rw-r--r--   0 ahmad      (501) staff       (20)     1049 2023-05-21 07:43:28.000000 Fletxible-0.5.2/tests/test_controls.py
+-rw-r--r--   0 ahmad      (501) staff       (20)        5 2023-05-01 14:25:50.000000 Fletxible-0.5.2/tests/test_route.py
```

### Comparing `Fletxible-0.5.1/Fletxible.egg-info/PKG-INFO` & `Fletxible-0.5.2/Fletxible.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Fletxible
-Version: 0.5.1
+Version: 0.5.2
 Summary: Web Boilerplate for Flet Library
 Home-page: https://github.com/LineIndent/fletxible
 Author: S. Ahmad P. Hakimi
 Author-email: pourhakimi@pm.me
 Keywords: python web template,web application,development
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `Fletxible-0.5.1/LICENSE` & `Fletxible-0.5.2/LICENSE`

 * *Files identical despite different names*

### Comparing `Fletxible-0.5.1/PKG-INFO` & `Fletxible-0.5.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Fletxible
-Version: 0.5.1
+Version: 0.5.2
 Summary: Web Boilerplate for Flet Library
 Home-page: https://github.com/LineIndent/fletxible
 Author: S. Ahmad P. Hakimi
 Author-email: pourhakimi@pm.me
 Keywords: python web template,web application,development
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `Fletxible-0.5.1/README.md` & `Fletxible-0.5.2/README.md`

 * *Files identical despite different names*

### Comparing `Fletxible-0.5.1/logic/cli.py` & `Fletxible-0.5.2/logic/cli.py`

 * *Files identical despite different names*

### Comparing `Fletxible-0.5.1/logic/controls.py` & `Fletxible-0.5.2/logic/controls.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,24 +1,49 @@
 import flet as ft
 import asyncio
-from styles import admonitions_color_scheme
+from logic.styles import admonitions_color_scheme
 
 
 def title(title):
     return ft.Text(value=title, size=21, weight="bold")
 
 
 def subtitle(title, key=None):
     return ft.Text(value=title, size=17, weight="w700", key=key)
 
 
 def text(title):
     return ft.Text(value=title, size=12, weight="w400")
 
 
+def generate_right_rail(number: int, title: list, funcOne: list, funcTwo: list):
+    rail_list: list = [
+        ft.Divider(height=10, color="transparent"),
+    ]
+
+    if number != 0:
+        for index in range(number):
+            rail_list.append(
+                ft.Container(
+                    content=ft.Text(
+                        title[index],
+                        size=12,
+                        color=ft.colors.with_opacity(0.55, "white10"),
+                    ),
+                    on_click=funcOne[index],
+                    on_hover=funcTwo[index],
+                )
+            )
+
+        return rail_list
+
+    else:
+        pass
+
+
 class CodeBlock(ft.UserControl):
     def __init__(self, title):
         #
         self.title = title
 
         #
         self._hovered: bool | None = None
```

### Comparing `Fletxible-0.5.1/logic/main.py` & `Fletxible-0.5.2/logic/main.py`

 * *Files 0% similar despite different names*

```diff
@@ -26,13 +26,14 @@
 
         else:
             for nav in page.views[-1].controls[:]:
                 nav.content.show_navigation()
 
     # Page events ...
     page.on_resize = resize_event
+    page.update()
     resize_event(None)
     page.update()
 
 
 if __name__ == "__main__":
     ft.flet.app(target=main)
```

### Comparing `Fletxible-0.5.1/logic/script.py` & `Fletxible-0.5.2/logic/script.py`

 * *Files 2% similar despite different names*

```diff
@@ -8,15 +8,14 @@
     set_app_route_method,
     set_app_default_pages,
     navigation_example_method,
 )
 
 #
 route_keys: dict = {}
-control_keys: list = []
 
 
 def open_yaml_script() -> dict:
     # Load the YAML file
     with open("flet_config.yml", "r") as file:
         docs = yaml.safe_load(file)
 
@@ -76,15 +75,14 @@
     os.remove("./logic/temp_route.txt")
 
 
 def set_default_methods_script(docs: dict):
     # Loop over the nav list and create/update files
     # 1. Temp. list to store the filepaths in + the modules dict
     file_list: list = []
-    # route_keys: dict = {}
 
     # 2. Loop through navigation tree and append the file_list with the filepaths
     for page in docs["nav"]:
         for key in page:
             filename = f"{page[key]}"
             filepath = os.path.join("pages", filename)
             file_list.append(filepath)
@@ -197,15 +195,19 @@
     # several step. First, adding the default method into each page
     try:
         route_keys: dict = set_default_methods_script(docs)
 
         for keys, __ in route_keys.items():
             page.views.append(route_keys[keys].loader.load_module().View())
 
-        page.go("/index")
+        # Set's the index.py page as the first page.
+        index = -1
+        current = 1
+        page.views[index], page.views[current] = page.views[current], page.views[index]
+        page.update()
 
     except Exception as e:
         print(e)
 
     # Map out the .yml file into a python dict
     try:
         map_yaml("flet_config.yml", "./logic/mapped.py")
```

### Comparing `Fletxible-0.5.1/logic/styles.py` & `Fletxible-0.5.2/logic/styles.py`

 * *Files identical despite different names*

### Comparing `Fletxible-0.5.1/setup.py` & `Fletxible-0.5.2/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,23 +1,26 @@
 from setuptools import setup
 
 setup(
     name="Fletxible",
-    version="0.5.1",
+    version="0.5.2",
     author="S. Ahmad P. Hakimi",
     author_email="pourhakimi@pm.me",
     description="Web Boilerplate for Flet Library",
     long_description="Fletxible is a Python web boilerplate project designed to provide a solid foundation for building web applications with Python and Flet. The project comes pre-configured with a range of tools and features to make it easy for developers to get started building their applications, without the need to spend time setting up infrastructure or configuring tools.",
     long_description_content_type="text/markdown",
     url="https://github.com/LineIndent/fletxible",
     packages=["logic"],
     install_requires=["click>=8.1.3", "flet>=0.7.1", "PyYAML>=6.0"],
     classifiers=[
         "Programming Language :: Python :: 3",
         "License :: OSI Approved :: MIT License",
         "Operating System :: OS Independent",
     ],
     entry_points={
-        "console_scripts": ["fletxible-init=logic.cli:init"],
+        "console_scripts": [
+            "fletxible-init=logic.cli:init",
+            "fletxible-build=logic.build:build",
+        ],
     },
     keywords=["python web template", "web application", "development"],
 )
```

