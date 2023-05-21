# Comparing `tmp/plugget-0.0.6.tar.gz` & `tmp/plugget-0.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "plugget-0.0.6.tar", last modified: Sat May 20 10:22:57 2023, max compression
+gzip compressed data, was "plugget-0.0.7.tar", last modified: Sun May 21 13:05:54 2023, max compression
```

## Comparing `plugget-0.0.6.tar` & `plugget-0.0.7.tar`

### file list

```diff
@@ -1,44 +1,44 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 10:22:57.249890 plugget-0.0.6/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 10:22:57.245890 plugget-0.0.6/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 10:22:57.245890 plugget-0.0.6/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)     1084 2023-05-20 10:22:45.000000 plugget-0.0.6/.github/workflows/python-publish.yml
--rw-r--r--   0 runner    (1001) docker     (123)     3077 2023-05-20 10:22:45.000000 plugget-0.0.6/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)     2322 2023-05-20 10:22:57.249890 plugget-0.0.6/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1834 2023-05-20 10:22:45.000000 plugget-0.0.6/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 10:22:57.245890 plugget-0.0.6/plugget/
--rw-r--r--   0 runner    (1001) docker     (123)       64 2023-05-20 10:22:45.000000 plugget-0.0.6/plugget/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 10:22:57.245890 plugget-0.0.6/plugget/actions/
--rw-r--r--   0 runner    (1001) docker     (123)     1547 2023-05-20 10:22:45.000000 plugget-0.0.6/plugget/actions/_template.py
--rw-r--r--   0 runner    (1001) docker     (123)     3621 2023-05-20 10:22:45.000000 plugget-0.0.6/plugget/actions/blender_addon.py
--rw-r--r--   0 runner    (1001) docker     (123)     1958 2023-05-20 10:22:45.000000 plugget-0.0.6/plugget/actions/blender_pip.py
--rw-r--r--   0 runner    (1001) docker     (123)     3683 2023-05-20 10:22:45.000000 plugget-0.0.6/plugget/actions/krita_pip.py
--rw-r--r--   0 runner    (1001) docker     (123)     3624 2023-05-20 10:22:45.000000 plugget-0.0.6/plugget/actions/krita_plugin.py
--rw-r--r--   0 runner    (1001) docker     (123)     2286 2023-05-20 10:22:45.000000 plugget-0.0.6/plugget/actions/max_macroscript.py
--rw-r--r--   0 runner    (1001) docker     (123)     3220 2023-05-20 10:22:45.000000 plugget-0.0.6/plugget/actions/unreal_pip.py
--rw-r--r--   0 runner    (1001) docker     (123)     1984 2023-05-20 10:22:45.000000 plugget-0.0.6/plugget/actions/unreal_plugin.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 10:22:57.245890 plugget-0.0.6/plugget/apps/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-20 10:22:45.000000 plugget-0.0.6/plugget/apps/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3355 2023-05-20 10:22:45.000000 plugget-0.0.6/plugget/apps/blender.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 10:22:57.245890 plugget-0.0.6/plugget/commands/
--rw-r--r--   0 runner    (1001) docker     (123)     9558 2023-05-20 10:22:45.000000 plugget-0.0.6/plugget/commands/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 10:22:57.249890 plugget-0.0.6/plugget/data/
--rw-r--r--   0 runner    (1001) docker     (123)      121 2023-05-20 10:22:45.000000 plugget-0.0.6/plugget/data/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    13655 2023-05-20 10:22:45.000000 plugget-0.0.6/plugget/data/package.py
--rw-r--r--   0 runner    (1001) docker     (123)     1469 2023-05-20 10:22:45.000000 plugget-0.0.6/plugget/data/packages_meta.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 10:22:57.249890 plugget-0.0.6/plugget/github/
--rw-r--r--   0 runner    (1001) docker     (123)     2670 2023-05-20 10:22:45.000000 plugget-0.0.6/plugget/github/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1825 2023-05-20 10:22:45.000000 plugget-0.0.6/plugget/github/async.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 10:22:57.249890 plugget-0.0.6/plugget/gumroad/
--rw-r--r--   0 runner    (1001) docker     (123)      858 2023-05-20 10:22:45.000000 plugget-0.0.6/plugget/gumroad/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2008 2023-05-20 10:22:45.000000 plugget-0.0.6/plugget/settings.py
--rw-r--r--   0 runner    (1001) docker     (123)      207 2023-05-20 10:22:45.000000 plugget-0.0.6/plugget/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 10:22:57.245890 plugget-0.0.6/plugget.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2322 2023-05-20 10:22:57.000000 plugget-0.0.6/plugget.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      800 2023-05-20 10:22:57.000000 plugget-0.0.6/plugget.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-20 10:22:57.000000 plugget-0.0.6/plugget.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       57 2023-05-20 10:22:57.000000 plugget-0.0.6/plugget.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-05-20 10:22:57.000000 plugget-0.0.6/plugget.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      967 2023-05-20 10:22:45.000000 plugget-0.0.6/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       19 2023-05-20 10:22:45.000000 plugget-0.0.6/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-20 10:22:57.249890 plugget-0.0.6/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1182 2023-05-20 10:22:45.000000 plugget-0.0.6/testcode.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 13:05:54.889620 plugget-0.0.7/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 13:05:54.877620 plugget-0.0.7/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 13:05:54.881620 plugget-0.0.7/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)     1084 2023-05-21 13:05:38.000000 plugget-0.0.7/.github/workflows/python-publish.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     3077 2023-05-21 13:05:38.000000 plugget-0.0.7/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)     2322 2023-05-21 13:05:54.889620 plugget-0.0.7/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1834 2023-05-21 13:05:38.000000 plugget-0.0.7/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 13:05:54.881620 plugget-0.0.7/plugget/
+-rw-r--r--   0 runner    (1001) docker     (123)       64 2023-05-21 13:05:38.000000 plugget-0.0.7/plugget/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 13:05:54.885620 plugget-0.0.7/plugget/actions/
+-rw-r--r--   0 runner    (1001) docker     (123)     1547 2023-05-21 13:05:38.000000 plugget-0.0.7/plugget/actions/_template.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3712 2023-05-21 13:05:38.000000 plugget-0.0.7/plugget/actions/blender_addon.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2124 2023-05-21 13:05:38.000000 plugget-0.0.7/plugget/actions/blender_pip.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3696 2023-05-21 13:05:38.000000 plugget-0.0.7/plugget/actions/krita_pip.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3624 2023-05-21 13:05:38.000000 plugget-0.0.7/plugget/actions/krita_plugin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2286 2023-05-21 13:05:38.000000 plugget-0.0.7/plugget/actions/max_macroscript.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3233 2023-05-21 13:05:38.000000 plugget-0.0.7/plugget/actions/unreal_pip.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1984 2023-05-21 13:05:38.000000 plugget-0.0.7/plugget/actions/unreal_plugin.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 13:05:54.885620 plugget-0.0.7/plugget/apps/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-21 13:05:38.000000 plugget-0.0.7/plugget/apps/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3355 2023-05-21 13:05:38.000000 plugget-0.0.7/plugget/apps/blender.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 13:05:54.885620 plugget-0.0.7/plugget/commands/
+-rw-r--r--   0 runner    (1001) docker     (123)     9750 2023-05-21 13:05:38.000000 plugget-0.0.7/plugget/commands/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 13:05:54.889620 plugget-0.0.7/plugget/data/
+-rw-r--r--   0 runner    (1001) docker     (123)      121 2023-05-21 13:05:38.000000 plugget-0.0.7/plugget/data/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13655 2023-05-21 13:05:38.000000 plugget-0.0.7/plugget/data/package.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1383 2023-05-21 13:05:38.000000 plugget-0.0.7/plugget/data/packages_meta.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 13:05:54.889620 plugget-0.0.7/plugget/github/
+-rw-r--r--   0 runner    (1001) docker     (123)     2670 2023-05-21 13:05:38.000000 plugget-0.0.7/plugget/github/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1825 2023-05-21 13:05:38.000000 plugget-0.0.7/plugget/github/async.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 13:05:54.889620 plugget-0.0.7/plugget/gumroad/
+-rw-r--r--   0 runner    (1001) docker     (123)      858 2023-05-21 13:05:38.000000 plugget-0.0.7/plugget/gumroad/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2008 2023-05-21 13:05:38.000000 plugget-0.0.7/plugget/settings.py
+-rw-r--r--   0 runner    (1001) docker     (123)      207 2023-05-21 13:05:38.000000 plugget-0.0.7/plugget/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 13:05:54.881620 plugget-0.0.7/plugget.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2322 2023-05-21 13:05:54.000000 plugget-0.0.7/plugget.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      800 2023-05-21 13:05:54.000000 plugget-0.0.7/plugget.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-21 13:05:54.000000 plugget-0.0.7/plugget.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       57 2023-05-21 13:05:54.000000 plugget-0.0.7/plugget.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-05-21 13:05:54.000000 plugget-0.0.7/plugget.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      967 2023-05-21 13:05:38.000000 plugget-0.0.7/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       19 2023-05-21 13:05:38.000000 plugget-0.0.7/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-21 13:05:54.889620 plugget-0.0.7/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1182 2023-05-21 13:05:38.000000 plugget-0.0.7/testcode.py
```

### Comparing `plugget-0.0.6/.github/workflows/python-publish.yml` & `plugget-0.0.7/.github/workflows/python-publish.yml`

 * *Files identical despite different names*

### Comparing `plugget-0.0.6/.gitignore` & `plugget-0.0.7/.gitignore`

 * *Files identical despite different names*

### Comparing `plugget-0.0.6/PKG-INFO` & `plugget-0.0.7/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: plugget
-Version: 0.0.6
+Version: 0.0.7
 Summary: detect which app the python interpreter is running in
 Author: Hannes
 Project-URL: Homepage, https://github.com/hannesdelbeke/plugget
 Project-URL: Source, https://github.com/hannesdelbeke/plugget
 Keywords: plugin,addon,add-on,extension,package,manager,resource,studio,dcc,app,application,pipeline,blender,krita,max
 Classifier: Programming Language :: Python :: 3.7
 Requires-Python: >=3.4
```

### Comparing `plugget-0.0.6/README.md` & `plugget-0.0.7/README.md`

 * *Files identical despite different names*

### Comparing `plugget-0.0.6/plugget/actions/_template.py` & `plugget-0.0.7/plugget/actions/_template.py`

 * *Files identical despite different names*

### Comparing `plugget-0.0.6/plugget/actions/blender_addon.py` & `plugget-0.0.7/plugget/actions/blender_addon.py`

 * *Files 5% similar despite different names*

```diff
@@ -76,14 +76,16 @@
         # check if plugin folder was copied, by checking if any files are in new_plugin_path
         # new_addon_path = local_addons_dir / addon_path.name
         # if not any(new_addon_path.iterdir()):
         #     logging.warning(f"Failed to install plugin {addon_path.name}")
         #     return False
 
     package.installed_paths |= {local_addons_dir / x.name for x in addon_paths}  # todo might want a dict later
+    # todo support renaming the addon in the config file
+    #  also delete renamed folder
 
 
 def uninstall(package: "plugget.data.Package", **kwargs):
     """uninstall plugin by name"""
     # todo make plugin name an action kwarg
 
     for p in package.installed_paths:
```

### Comparing `plugget-0.0.6/plugget/actions/blender_pip.py` & `plugget-0.0.7/plugget/actions/blender_pip.py`

 * *Files 5% similar despite different names*

```diff
@@ -21,15 +21,19 @@
 def install(package: "plugget.data.Package", **kwargs):
     blender_user_site_packages = Path(str(bpy.utils.script_path_user())) / "modules"  # appdata
 
     for p in get_requirements(package):
         if p.exists():
             print("requirements.txt found, installing requirements")
             # todo blender pip
-            subprocess.run(["pip", "install", "-r", package.clone_dir / p, '-t', blender_user_site_packages])
+            try:
+                # todo python -m pip
+                subprocess.run(["pip", "install", "-r", package.clone_dir / p, '-t', blender_user_site_packages, "--no-user"])
+            except subprocess.CalledProcessError as e:
+                logging.error(e.output)
         else:
             logging.warning(f"expected requirements.txt not found: '{p}'")
     importlib.invalidate_caches()
 
 
 def uninstall(package: "plugget.data.Package", dependencies=False, **kwargs):
     # this method runs on uninstall, then the manifest is removed from installed packages
```

### Comparing `plugget-0.0.6/plugget/actions/krita_pip.py` & `plugget-0.0.7/plugget/actions/krita_pip.py`

 * *Files 2% similar despite different names*

```diff
@@ -56,15 +56,15 @@
 
 def install(package: "plugget.data.Package", **kwargs):
     print("check for requirements")
 
     for p in get_requirements(package):
         if p.exists():
             print("requirements.txt found, installing requirements")
-            subprocess.run(["pip", "install", "-r", package.clone_dir / p, '-t', path])
+            subprocess.run(["pip", "install", "-r", package.clone_dir / p, '-t', path, "--no-user"])
         else:
             logging.warning(f"expected requirements.txt not found: '{p}'")
     importlib.invalidate_caches()
 
 
 # def install(package: "plugget.data.Package", **kwargs):
 #     # Use the Python executable to run the pip install command
```

### Comparing `plugget-0.0.6/plugget/actions/krita_plugin.py` & `plugget-0.0.7/plugget/actions/krita_plugin.py`

 * *Files identical despite different names*

### Comparing `plugget-0.0.6/plugget/actions/max_macroscript.py` & `plugget-0.0.7/plugget/actions/max_macroscript.py`

 * *Files identical despite different names*

### Comparing `plugget-0.0.6/plugget/actions/unreal_pip.py` & `plugget-0.0.7/plugget/actions/unreal_pip.py`

 * *Files 1% similar despite different names*

```diff
@@ -47,15 +47,15 @@
 
 def install(package: "plugget.data.Package", **kwargs):
     print("check for requirements")
 
     for p in get_requirements(package):
         if p.exists():
             print("requirements.txt found, installing requirements")
-            subprocess.run(["pip", "install", "-r", package.clone_dir / p, '-t', project_site_dir])
+            subprocess.run(["pip", "install", "-r", package.clone_dir / p, '-t', project_site_dir, "--no-user"])
         else:
             logging.warning(f"expected requirements.txt not found: '{p}'")
     importlib.invalidate_caches()
 
     # # check if files were copied: package.clone_dir / p
     # if not (package.clone_dir / p).exists():
     #     raise FileNotFoundError(f"expected file not found: '{p}'")
```

### Comparing `plugget-0.0.6/plugget/actions/unreal_plugin.py` & `plugget-0.0.7/plugget/actions/unreal_plugin.py`

 * *Files identical despite different names*

### Comparing `plugget-0.0.6/plugget/apps/blender.py` & `plugget-0.0.7/plugget/apps/blender.py`

 * *Files identical despite different names*

### Comparing `plugget-0.0.6/plugget/commands/__init__.py` & `plugget-0.0.7/plugget/commands/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 """
 Plugget is a plugin-manager for various applications.
 """
 import logging
 import subprocess
 import datetime
 import pprint
+import os
 
 from plugget.utils import rmdir
 from plugget.data import Package, PackagesMeta
 from plugget import settings
 
 from pathlib import Path
 
@@ -30,21 +31,24 @@
 
 
 def _clone_manifest_repo(source_url) -> "pathlib.Path":
     """clone git repo containing plugget manifests, from a git URL"""
     source_name = source_url.split("/")[-1].split(".")[0]
     source_dir = settings.TEMP_PLUGGET / source_name
 
-    # CACHING: check when repo was last updated
-    if (source_dir / "_LAST_UPDATED").exists():
-        with open(source_dir / "_LAST_UPDATED", "r") as f:
-            last_updated = datetime.datetime.strptime(f.read(), "%Y-%m-%d %H:%M:%S")
-        if last_updated > datetime.datetime.now() - datetime.timedelta(days=1):
-            print("using cached manifest repo, last updated less than a day ago")
-            return source_dir
+    # by default disable caching for now, it hinders debugging
+    # great for instant search results though
+    if os.environ['PLUGGET_USE_CACHE'] == 1:
+        # CACHING: check when repo was last updated
+        if (source_dir / "_LAST_UPDATED").exists():
+            with open(source_dir / "_LAST_UPDATED", "r") as f:
+                last_updated = datetime.datetime.strptime(f.read(), "%Y-%m-%d %H:%M:%S")
+            if last_updated > datetime.datetime.now() - datetime.timedelta(days=1):
+                print("using cached manifest repo, last updated less than a day ago")
+                return source_dir
 
     # remove old manifest repo
     rmdir(source_dir)  # todo catch if this failed
     # check if dir exists
     if source_dir.exists():
         raise Exception(f"Failed to remove source_dir {source_dir}")
```

### Comparing `plugget-0.0.6/plugget/data/package.py` & `plugget-0.0.7/plugget/data/package.py`

 * *Files identical despite different names*

### Comparing `plugget-0.0.6/plugget/data/packages_meta.py` & `plugget-0.0.7/plugget/data/packages_meta.py`

 * *Files 6% similar despite different names*

```diff
@@ -29,14 +29,12 @@
         return [x.version for x in self.packages]
 
     def __getattr__(self, attr):
         """__getattr__ is called when the attr is not found on the instance
         try get the attr from the latest package, e.g. package_meta.install() == package_meta.latest.install()"""
         return getattr(self.latest, attr)
 
-    def get_version(self, version:str) -> "plugget.data.package.Package":
+    def get_version(self, version:str) -> "plugget.data.package.Package | None":
         """get package with matching version from self.packages"""
         match = [x for x in self.packages if version == x.version]
         if match:
-            return match[0]
-        else:
-            logging.warning(f"could not find package of version '{version}'")
+            return match[0]
```

### Comparing `plugget-0.0.6/plugget/github/__init__.py` & `plugget-0.0.7/plugget/github/__init__.py`

 * *Files identical despite different names*

### Comparing `plugget-0.0.6/plugget/github/async.py` & `plugget-0.0.7/plugget/github/async.py`

 * *Files identical despite different names*

### Comparing `plugget-0.0.6/plugget/gumroad/__init__.py` & `plugget-0.0.7/plugget/gumroad/__init__.py`

 * *Files identical despite different names*

### Comparing `plugget-0.0.6/plugget/settings.py` & `plugget-0.0.7/plugget/settings.py`

 * *Files identical despite different names*

### Comparing `plugget-0.0.6/plugget.egg-info/PKG-INFO` & `plugget-0.0.7/plugget.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: plugget
-Version: 0.0.6
+Version: 0.0.7
 Summary: detect which app the python interpreter is running in
 Author: Hannes
 Project-URL: Homepage, https://github.com/hannesdelbeke/plugget
 Project-URL: Source, https://github.com/hannesdelbeke/plugget
 Keywords: plugin,addon,add-on,extension,package,manager,resource,studio,dcc,app,application,pipeline,blender,krita,max
 Classifier: Programming Language :: Python :: 3.7
 Requires-Python: >=3.4
```

### Comparing `plugget-0.0.6/plugget.egg-info/SOURCES.txt` & `plugget-0.0.7/plugget.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `plugget-0.0.6/pyproject.toml` & `plugget-0.0.7/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -19,15 +19,15 @@
 #license = { file = "LICENSE" }
 classifiers = [
     "Programming Language :: Python :: 3.7",
 ]
 #dynamic = ["dependencies"]
 dependencies = ['importlib-metadata; python_version<"3.7"', "detect-app"]
 #dynamic = ["version"]
-version = "0.0.6"
+version = "0.0.7"
 
 #[project.optional-dependencies]
 #yaml = ["pyyaml"]
 
 #[project.scripts]
 #my-script = "my_package.module:function"
```

### Comparing `plugget-0.0.6/testcode.py` & `plugget-0.0.7/testcode.py`

 * *Files identical despite different names*

