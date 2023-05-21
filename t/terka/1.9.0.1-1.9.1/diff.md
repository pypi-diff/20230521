# Comparing `tmp/terka-1.9.0.1.tar.gz` & `tmp/terka-1.9.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "terka-1.9.0.1.tar", last modified: Sun May 14 20:46:02 2023, max compression
+gzip compressed data, was "terka-1.9.1.tar", last modified: Mon May 15 19:30:56 2023, max compression
```

## Comparing `terka-1.9.0.1.tar` & `terka-1.9.1.tar`

### file list

```diff
@@ -1,46 +1,56 @@
-drwxr-xr-x   0 am        (1000) am        (1000)        0 2023-05-14 20:46:02.137953 terka-1.9.0.1/
--rw-r--r--   0 am        (1000) am        (1000)      294 2023-05-14 20:46:02.137953 terka-1.9.0.1/PKG-INFO
--rw-r--r--   0 am        (1000) am        (1000)       38 2023-05-14 20:46:02.137953 terka-1.9.0.1/setup.cfg
--rw-r--r--   0 am        (1000) am        (1000)      912 2023-05-14 20:45:49.000000 terka-1.9.0.1/setup.py
-drwxr-xr-x   0 am        (1000) am        (1000)        0 2023-05-14 20:46:02.133953 terka-1.9.0.1/terka/
--rw-r--r--   0 am        (1000) am        (1000)        0 2023-05-11 20:48:24.000000 terka-1.9.0.1/terka/__init__.py
-drwxr-xr-x   0 am        (1000) am        (1000)        0 2023-05-14 20:46:02.133953 terka-1.9.0.1/terka/adapters/
--rw-r--r--   0 am        (1000) am        (1000)        0 2023-05-11 20:48:24.000000 terka-1.9.0.1/terka/adapters/__init__.py
--rw-r--r--   0 am        (1000) am        (1000)    16361 2023-05-11 20:48:24.000000 terka-1.9.0.1/terka/adapters/orm.py
--rw-r--r--   0 am        (1000) am        (1000)     6150 2023-05-11 20:48:24.000000 terka-1.9.0.1/terka/adapters/repository.py
-drwxr-xr-x   0 am        (1000) am        (1000)        0 2023-05-14 20:46:02.137953 terka-1.9.0.1/terka/domain/
--rw-r--r--   0 am        (1000) am        (1000)        0 2023-05-11 20:48:24.000000 terka-1.9.0.1/terka/domain/__init__.py
--rw-r--r--   0 am        (1000) am        (1000)      576 2023-05-11 20:48:24.000000 terka-1.9.0.1/terka/domain/collaborators.py
--rw-r--r--   0 am        (1000) am        (1000)    41811 2023-05-14 20:36:38.000000 terka-1.9.0.1/terka/domain/commands.py
--rw-r--r--   0 am        (1000) am        (1000)     1643 2023-05-11 20:48:24.000000 terka-1.9.0.1/terka/domain/commentary.py
--rw-r--r--   0 am        (1000) am        (1000)      102 2023-05-11 20:48:24.000000 terka-1.9.0.1/terka/domain/element.py
--rw-r--r--   0 am        (1000) am        (1000)     1513 2023-05-11 20:48:24.000000 terka-1.9.0.1/terka/domain/epic.py
--rw-r--r--   0 am        (1000) am        (1000)     1440 2023-05-11 20:48:24.000000 terka-1.9.0.1/terka/domain/event_history.py
-drwxr-xr-x   0 am        (1000) am        (1000)        0 2023-05-14 20:46:02.137953 terka-1.9.0.1/terka/domain/external_connectors/
--rw-r--r--   0 am        (1000) am        (1000)        0 2023-05-11 20:48:24.000000 terka-1.9.0.1/terka/domain/external_connectors/__init__.py
--rw-r--r--   0 am        (1000) am        (1000)      265 2023-05-11 20:48:24.000000 terka-1.9.0.1/terka/domain/external_connectors/asana.py
--rw-r--r--   0 am        (1000) am        (1000)      892 2023-05-11 20:48:24.000000 terka-1.9.0.1/terka/domain/project.py
--rw-r--r--   0 am        (1000) am        (1000)     2244 2023-05-11 20:48:24.000000 terka-1.9.0.1/terka/domain/sprint.py
--rw-r--r--   0 am        (1000) am        (1000)     1495 2023-05-11 20:48:24.000000 terka-1.9.0.1/terka/domain/story.py
--rw-r--r--   0 am        (1000) am        (1000)      639 2023-05-11 20:48:24.000000 terka-1.9.0.1/terka/domain/tag.py
--rw-r--r--   0 am        (1000) am        (1000)     2082 2023-05-11 20:48:24.000000 terka-1.9.0.1/terka/domain/task.py
--rw-r--r--   0 am        (1000) am        (1000)      530 2023-05-11 20:48:24.000000 terka-1.9.0.1/terka/domain/time_tracker.py
--rw-r--r--   0 am        (1000) am        (1000)      338 2023-05-11 20:48:24.000000 terka-1.9.0.1/terka/domain/user.py
-drwxr-xr-x   0 am        (1000) am        (1000)        0 2023-05-14 20:46:02.137953 terka-1.9.0.1/terka/entrypoints/
--rw-r--r--   0 am        (1000) am        (1000)        0 2023-05-11 20:48:24.000000 terka-1.9.0.1/terka/entrypoints/__init__.py
--rw-r--r--   0 am        (1000) am        (1000)     6345 2023-05-14 20:37:14.000000 terka-1.9.0.1/terka/entrypoints/cli.py
-drwxr-xr-x   0 am        (1000) am        (1000)        0 2023-05-14 20:46:02.137953 terka-1.9.0.1/terka/service_layer/
--rw-r--r--   0 am        (1000) am        (1000)        0 2023-05-11 20:48:24.000000 terka-1.9.0.1/terka/service_layer/__init__.py
--rw-r--r--   0 am        (1000) am        (1000)    32008 2023-05-14 20:45:39.000000 terka-1.9.0.1/terka/service_layer/printer.py
--rw-r--r--   0 am        (1000) am        (1000)     6558 2023-05-14 20:27:18.000000 terka-1.9.0.1/terka/service_layer/services.py
--rw-r--r--   0 am        (1000) am        (1000)     3882 2023-05-11 20:48:24.000000 terka-1.9.0.1/terka/service_layer/ui.py
--rw-r--r--   0 am        (1000) am        (1000)      698 2023-05-11 20:48:24.000000 terka-1.9.0.1/terka/service_layer/vertical_layout.css
--rw-r--r--   0 am        (1000) am        (1000)     2382 2023-05-11 20:48:24.000000 terka-1.9.0.1/terka/service_layer/views.py
--rw-r--r--   0 am        (1000) am        (1000)     7800 2023-05-14 20:38:48.000000 terka-1.9.0.1/terka/utils.py
-drwxr-xr-x   0 am        (1000) am        (1000)        0 2023-05-14 20:46:02.133953 terka-1.9.0.1/terka.egg-info/
--rw-r--r--   0 am        (1000) am        (1000)      294 2023-05-14 20:46:02.000000 terka-1.9.0.1/terka.egg-info/PKG-INFO
--rw-r--r--   0 am        (1000) am        (1000)      969 2023-05-14 20:46:02.000000 terka-1.9.0.1/terka.egg-info/SOURCES.txt
--rw-r--r--   0 am        (1000) am        (1000)        1 2023-05-14 20:46:02.000000 terka-1.9.0.1/terka.egg-info/dependency_links.txt
--rw-r--r--   0 am        (1000) am        (1000)       53 2023-05-14 20:46:02.000000 terka-1.9.0.1/terka.egg-info/entry_points.txt
--rw-r--r--   0 am        (1000) am        (1000)       59 2023-05-14 20:46:02.000000 terka-1.9.0.1/terka.egg-info/requires.txt
--rw-r--r--   0 am        (1000) am        (1000)        6 2023-05-14 20:46:02.000000 terka-1.9.0.1/terka.egg-info/top_level.txt
+drwxr-xr-x   0 am        (1000) am        (1000)        0 2023-05-15 19:30:56.252260 terka-1.9.1/
+-rw-r--r--   0 am        (1000) am        (1000)    11357 2023-05-11 20:48:24.000000 terka-1.9.1/LICENSE
+-rw-r--r--   0 am        (1000) am        (1000)     1471 2023-05-15 19:30:56.252260 terka-1.9.1/PKG-INFO
+-rw-r--r--   0 am        (1000) am        (1000)     1156 2023-05-15 18:52:47.000000 terka-1.9.1/README.md
+-rw-r--r--   0 am        (1000) am        (1000)       38 2023-05-15 19:30:56.252260 terka-1.9.1/setup.cfg
+-rw-r--r--   0 am        (1000) am        (1000)      937 2023-05-15 18:51:36.000000 terka-1.9.1/setup.py
+drwxr-xr-x   0 am        (1000) am        (1000)        0 2023-05-15 19:30:56.244260 terka-1.9.1/terka/
+-rw-r--r--   0 am        (1000) am        (1000)        0 2023-05-11 20:48:24.000000 terka-1.9.1/terka/__init__.py
+drwxr-xr-x   0 am        (1000) am        (1000)        0 2023-05-15 19:30:56.248260 terka-1.9.1/terka/adapters/
+-rw-r--r--   0 am        (1000) am        (1000)        0 2023-05-11 20:48:24.000000 terka-1.9.1/terka/adapters/__init__.py
+-rw-r--r--   0 am        (1000) am        (1000)    16361 2023-05-11 20:48:24.000000 terka-1.9.1/terka/adapters/orm.py
+-rw-r--r--   0 am        (1000) am        (1000)     6150 2023-05-11 20:48:24.000000 terka-1.9.1/terka/adapters/repository.py
+drwxr-xr-x   0 am        (1000) am        (1000)        0 2023-05-15 19:30:56.248260 terka-1.9.1/terka/domain/
+-rw-r--r--   0 am        (1000) am        (1000)        0 2023-05-11 20:48:24.000000 terka-1.9.1/terka/domain/__init__.py
+-rw-r--r--   0 am        (1000) am        (1000)      576 2023-05-11 20:48:24.000000 terka-1.9.1/terka/domain/collaborators.py
+-rw-r--r--   0 am        (1000) am        (1000)    41811 2023-05-15 18:39:55.000000 terka-1.9.1/terka/domain/commands.py
+-rw-r--r--   0 am        (1000) am        (1000)     1643 2023-05-11 20:48:24.000000 terka-1.9.1/terka/domain/commentary.py
+-rw-r--r--   0 am        (1000) am        (1000)      102 2023-05-11 20:48:24.000000 terka-1.9.1/terka/domain/element.py
+-rw-r--r--   0 am        (1000) am        (1000)     1513 2023-05-11 20:48:24.000000 terka-1.9.1/terka/domain/epic.py
+-rw-r--r--   0 am        (1000) am        (1000)     1440 2023-05-11 20:48:24.000000 terka-1.9.1/terka/domain/event_history.py
+drwxr-xr-x   0 am        (1000) am        (1000)        0 2023-05-15 19:30:56.248260 terka-1.9.1/terka/domain/external_connectors/
+-rw-r--r--   0 am        (1000) am        (1000)        0 2023-05-11 20:48:24.000000 terka-1.9.1/terka/domain/external_connectors/__init__.py
+-rw-r--r--   0 am        (1000) am        (1000)      265 2023-05-11 20:48:24.000000 terka-1.9.1/terka/domain/external_connectors/asana.py
+-rw-r--r--   0 am        (1000) am        (1000)      892 2023-05-11 20:48:24.000000 terka-1.9.1/terka/domain/project.py
+-rw-r--r--   0 am        (1000) am        (1000)     2244 2023-05-11 20:48:24.000000 terka-1.9.1/terka/domain/sprint.py
+-rw-r--r--   0 am        (1000) am        (1000)     1495 2023-05-11 20:48:24.000000 terka-1.9.1/terka/domain/story.py
+-rw-r--r--   0 am        (1000) am        (1000)      639 2023-05-11 20:48:24.000000 terka-1.9.1/terka/domain/tag.py
+-rw-r--r--   0 am        (1000) am        (1000)     2082 2023-05-11 20:48:24.000000 terka-1.9.1/terka/domain/task.py
+-rw-r--r--   0 am        (1000) am        (1000)      530 2023-05-11 20:48:24.000000 terka-1.9.1/terka/domain/time_tracker.py
+-rw-r--r--   0 am        (1000) am        (1000)      338 2023-05-11 20:48:24.000000 terka-1.9.1/terka/domain/user.py
+drwxr-xr-x   0 am        (1000) am        (1000)        0 2023-05-15 19:30:56.248260 terka-1.9.1/terka/entrypoints/
+-rw-r--r--   0 am        (1000) am        (1000)        0 2023-05-11 20:48:24.000000 terka-1.9.1/terka/entrypoints/__init__.py
+-rw-r--r--   0 am        (1000) am        (1000)     6527 2023-05-15 18:39:55.000000 terka-1.9.1/terka/entrypoints/cli.py
+drwxr-xr-x   0 am        (1000) am        (1000)        0 2023-05-15 19:30:56.248260 terka-1.9.1/terka/service_layer/
+-rw-r--r--   0 am        (1000) am        (1000)        0 2023-05-11 20:48:24.000000 terka-1.9.1/terka/service_layer/__init__.py
+-rw-r--r--   0 am        (1000) am        (1000)    32008 2023-05-14 20:45:39.000000 terka-1.9.1/terka/service_layer/printer.py
+-rw-r--r--   0 am        (1000) am        (1000)     6558 2023-05-14 20:27:18.000000 terka-1.9.1/terka/service_layer/services.py
+-rw-r--r--   0 am        (1000) am        (1000)     3882 2023-05-11 20:48:24.000000 terka-1.9.1/terka/service_layer/ui.py
+-rw-r--r--   0 am        (1000) am        (1000)      698 2023-05-11 20:48:24.000000 terka-1.9.1/terka/service_layer/vertical_layout.css
+-rw-r--r--   0 am        (1000) am        (1000)     2382 2023-05-11 20:48:24.000000 terka-1.9.1/terka/service_layer/views.py
+-rw-r--r--   0 am        (1000) am        (1000)     7800 2023-05-14 20:38:48.000000 terka-1.9.1/terka/utils.py
+drwxr-xr-x   0 am        (1000) am        (1000)        0 2023-05-15 19:30:56.244260 terka-1.9.1/terka.egg-info/
+-rw-r--r--   0 am        (1000) am        (1000)     1471 2023-05-15 19:30:56.000000 terka-1.9.1/terka.egg-info/PKG-INFO
+-rw-r--r--   0 am        (1000) am        (1000)     1122 2023-05-15 19:30:56.000000 terka-1.9.1/terka.egg-info/SOURCES.txt
+-rw-r--r--   0 am        (1000) am        (1000)        1 2023-05-15 19:30:56.000000 terka-1.9.1/terka.egg-info/dependency_links.txt
+-rw-r--r--   0 am        (1000) am        (1000)       53 2023-05-15 19:30:56.000000 terka-1.9.1/terka.egg-info/entry_points.txt
+-rw-r--r--   0 am        (1000) am        (1000)       77 2023-05-15 19:30:56.000000 terka-1.9.1/terka.egg-info/requires.txt
+-rw-r--r--   0 am        (1000) am        (1000)       12 2023-05-15 19:30:56.000000 terka-1.9.1/terka.egg-info/top_level.txt
+drwxr-xr-x   0 am        (1000) am        (1000)        0 2023-05-15 19:30:56.252260 terka-1.9.1/tests/
+-rw-r--r--   0 am        (1000) am        (1000)        0 2023-05-11 20:48:24.000000 terka-1.9.1/tests/__init__.py
+-rw-r--r--   0 am        (1000) am        (1000)      424 2023-05-11 20:48:24.000000 terka-1.9.1/tests/conftest.py
+-rw-r--r--   0 am        (1000) am        (1000)       43 2023-05-11 20:48:24.000000 terka-1.9.1/tests/test_commands.py
+-rw-r--r--   0 am        (1000) am        (1000)     2818 2023-05-11 20:48:24.000000 terka-1.9.1/tests/test_orm.py
+-rw-r--r--   0 am        (1000) am        (1000)      956 2023-05-11 20:48:24.000000 terka-1.9.1/tests/test_task.py
+-rw-r--r--   0 am        (1000) am        (1000)     1281 2023-05-11 20:48:24.000000 terka-1.9.1/tests/test_user.py
+-rw-r--r--   0 am        (1000) am        (1000)      265 2023-05-11 20:48:24.000000 terka-1.9.1/tests/test_utils.py
```

### Comparing `terka-1.9.0.1/setup.py` & `terka-1.9.1/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,30 +1,32 @@
 import pathlib
 from setuptools import setup, find_packages
 
-HERE = pathlib.Path(__file__).parent
-# README = (HERE.parent / "README.md").read_text()
+HERE = pathlib.Path(__file__)
+README = (HERE.parent / "README.md").read_text()
 
 setup(
     name="terka",
-    version="1.9.0.1",
+    version="1.9.1",
     description="CLI utility for creating and managing tasks in a terminal",
-    # long_description=README,
+    long_description=README,
     long_description_content_type="text/markdown",
     author="Andrei Markin",
     author_email="andrey.markin.ppc@gmail.com",
     license="Apache 2.0",
     url="https://github.com/AndreyMarkinPPC/terka",
     packages=find_packages(),
     include_package_data=True,
     package_data={"": ["service_layer/*.css"]},
     install_requires=[
-        "sqlalchemy==1.4.0", "pyaml", "rich", "textual==0.5.0", "plotext==5.2.8"
+        "sqlalchemy==1.4.0",
+        "pyaml",
+        "rich",
+        "textual==0.5.0",
+        "plotext==5.2.8",
+        "pandas",
+        "matplotlib",
     ],
     setup_requires=["pytest-runner"],
     tests_requires=["pytest"],
-    entry_points={
-        "console_scripts": [
-            "terka=terka.entrypoints.cli:main"
-        ]
-    }
+    entry_points={"console_scripts": ["terka=terka.entrypoints.cli:main"]},
 )
```

### Comparing `terka-1.9.0.1/terka/adapters/orm.py` & `terka-1.9.1/terka/adapters/orm.py`

 * *Files identical despite different names*

### Comparing `terka-1.9.0.1/terka/adapters/repository.py` & `terka-1.9.1/terka/adapters/repository.py`

 * *Files identical despite different names*

### Comparing `terka-1.9.0.1/terka/domain/collaborators.py` & `terka-1.9.1/terka/domain/collaborators.py`

 * *Files identical despite different names*

### Comparing `terka-1.9.0.1/terka/domain/commands.py` & `terka-1.9.1/terka/domain/commands.py`

 * *Files identical despite different names*

### Comparing `terka-1.9.0.1/terka/domain/commentary.py` & `terka-1.9.1/terka/domain/commentary.py`

 * *Files identical despite different names*

### Comparing `terka-1.9.0.1/terka/domain/epic.py` & `terka-1.9.1/terka/domain/epic.py`

 * *Files identical despite different names*

### Comparing `terka-1.9.0.1/terka/domain/event_history.py` & `terka-1.9.1/terka/domain/event_history.py`

 * *Files identical despite different names*

### Comparing `terka-1.9.0.1/terka/domain/project.py` & `terka-1.9.1/terka/domain/project.py`

 * *Files identical despite different names*

### Comparing `terka-1.9.0.1/terka/domain/sprint.py` & `terka-1.9.1/terka/domain/sprint.py`

 * *Files identical despite different names*

### Comparing `terka-1.9.0.1/terka/domain/story.py` & `terka-1.9.1/terka/domain/story.py`

 * *Files identical despite different names*

### Comparing `terka-1.9.0.1/terka/domain/tag.py` & `terka-1.9.1/terka/domain/tag.py`

 * *Files identical despite different names*

### Comparing `terka-1.9.0.1/terka/domain/task.py` & `terka-1.9.1/terka/domain/task.py`

 * *Files identical despite different names*

### Comparing `terka-1.9.0.1/terka/domain/time_tracker.py` & `terka-1.9.1/terka/domain/time_tracker.py`

 * *Files identical despite different names*

### Comparing `terka-1.9.0.1/terka/entrypoints/cli.py` & `terka-1.9.1/terka/entrypoints/cli.py`

 * *Files 1% similar despite different names*

```diff
@@ -120,14 +120,18 @@
                         case [project, name]:
                             task_dict = {"name": name, "project": project}
                         case [name]:
                             task_dict = {"name": name}
                         case _:
                             raise Exception("Unknown format")
                     task_dict = update_task_dict(task_dict, repo)
+                    if entity.startswith("s/"):
+                        entity = "stories"
+                    elif entity.startswith("e/"):
+                        entity = "epics"
                     command_handler.execute(command, entity, task_dict)
             exit()
         is_interactive = False
         if not command and not entity:
             is_interactive = True
             interactive_message = (
                 f"[green]>>> Running terka in an interactive mode[/green]"
```

### Comparing `terka-1.9.0.1/terka/service_layer/printer.py` & `terka-1.9.1/terka/service_layer/printer.py`

 * *Files identical despite different names*

### Comparing `terka-1.9.0.1/terka/service_layer/services.py` & `terka-1.9.1/terka/service_layer/services.py`

 * *Files identical despite different names*

### Comparing `terka-1.9.0.1/terka/service_layer/ui.py` & `terka-1.9.1/terka/service_layer/ui.py`

 * *Files identical despite different names*

### Comparing `terka-1.9.0.1/terka/service_layer/vertical_layout.css` & `terka-1.9.1/terka/service_layer/vertical_layout.css`

 * *Files identical despite different names*

### Comparing `terka-1.9.0.1/terka/service_layer/views.py` & `terka-1.9.1/terka/service_layer/views.py`

 * *Files identical despite different names*

### Comparing `terka-1.9.0.1/terka/utils.py` & `terka-1.9.1/terka/utils.py`

 * *Files identical despite different names*

### Comparing `terka-1.9.0.1/terka.egg-info/SOURCES.txt` & `terka-1.9.1/terka.egg-info/SOURCES.txt`

 * *Files 21% similar despite different names*

```diff
@@ -1,7 +1,9 @@
+LICENSE
+README.md
 setup.py
 terka/__init__.py
 terka/utils.py
 terka.egg-info/PKG-INFO
 terka.egg-info/SOURCES.txt
 terka.egg-info/dependency_links.txt
 terka.egg-info/entry_points.txt
@@ -29,8 +31,15 @@
 terka/entrypoints/__init__.py
 terka/entrypoints/cli.py
 terka/service_layer/__init__.py
 terka/service_layer/printer.py
 terka/service_layer/services.py
 terka/service_layer/ui.py
 terka/service_layer/vertical_layout.css
-terka/service_layer/views.py
+terka/service_layer/views.py
+tests/__init__.py
+tests/conftest.py
+tests/test_commands.py
+tests/test_orm.py
+tests/test_task.py
+tests/test_user.py
+tests/test_utils.py
```

