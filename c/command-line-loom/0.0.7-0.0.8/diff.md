# Comparing `tmp/command_line_loom-0.0.7.tar.gz` & `tmp/command_line_loom-0.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "command_line_loom-0.0.7.tar", max compression
+gzip compressed data, was "command_line_loom-0.0.8.tar", max compression
```

## Comparing `command_line_loom-0.0.7.tar` & `command_line_loom-0.0.8.tar`

### file list

```diff
@@ -1,17 +1,17 @@
--rw-r--r--   0        0        0     1070 2023-05-18 18:19:49.972930 command_line_loom-0.0.7/LICENSE
--rw-r--r--   0        0        0     1899 2023-05-21 13:57:05.105476 command_line_loom-0.0.7/README.md
--rw-r--r--   0        0        0        7 2023-05-19 13:37:16.686088 command_line_loom-0.0.7/cll/__init__.py
--rw-r--r--   0        0        0     1555 2023-05-19 13:37:16.690088 command_line_loom-0.0.7/cll/__main__.py
--rw-r--r--   0        0        0     7645 2023-05-19 21:14:40.199467 command_line_loom-0.0.7/cll/app.py
--rw-r--r--   0        0        0     7381 2023-05-20 21:23:31.452227 command_line_loom-0.0.7/cll/config.py
--rw-r--r--   0        0        0      217 2023-05-19 13:37:16.690088 command_line_loom-0.0.7/cll/data_structs/__init__.py
--rw-r--r--   0        0        0    13252 2023-05-21 13:07:37.864187 command_line_loom-0.0.7/cll/data_structs/data_structs.py
--rw-r--r--   0        0        0    11176 2023-05-21 13:19:09.623216 command_line_loom-0.0.7/cll/data_structs/loom_index.py
--rw-r--r--   0        0        0     2493 2023-05-19 17:01:41.546225 command_line_loom-0.0.7/cll/data_structs/node.py
--rwxr-xr-x   0        0        0     4162 2023-05-21 14:03:25.003785 command_line_loom-0.0.7/cll/encoder.py
--rw-r--r--   0        0        0     1025 2023-05-19 13:37:16.690088 command_line_loom-0.0.7/cll/io.py
--rw-r--r--   0        0        0     2381 2023-05-19 21:14:40.203467 command_line_loom-0.0.7/cll/store.py
--rw-r--r--   0        0        0     7963 2023-05-19 21:14:40.203467 command_line_loom-0.0.7/cll/templater.py
--rw-r--r--   0        0        0    19070 2023-05-21 14:09:35.940621 command_line_loom-0.0.7/cll/tree.py
--rw-r--r--   0        0        0     1052 2023-05-21 14:17:02.082261 command_line_loom-0.0.7/pyproject.toml
--rw-r--r--   0        0        0     2913 1970-01-01 00:00:00.000000 command_line_loom-0.0.7/PKG-INFO
+-rw-r--r--   0        0        0     1070 2023-05-18 18:19:49.972930 command_line_loom-0.0.8/LICENSE
+-rw-r--r--   0        0        0     1899 2023-05-21 13:57:05.105476 command_line_loom-0.0.8/README.md
+-rw-r--r--   0        0        0        7 2023-05-19 13:37:16.686088 command_line_loom-0.0.8/cll/__init__.py
+-rw-r--r--   0        0        0     1555 2023-05-19 13:37:16.690088 command_line_loom-0.0.8/cll/__main__.py
+-rw-r--r--   0        0        0     7645 2023-05-19 21:14:40.199467 command_line_loom-0.0.8/cll/app.py
+-rw-r--r--   0        0        0     7381 2023-05-20 21:23:31.452227 command_line_loom-0.0.8/cll/config.py
+-rw-r--r--   0        0        0      217 2023-05-19 13:37:16.690088 command_line_loom-0.0.8/cll/data_structs/__init__.py
+-rw-r--r--   0        0        0    13252 2023-05-21 13:07:37.864187 command_line_loom-0.0.8/cll/data_structs/data_structs.py
+-rw-r--r--   0        0        0    11176 2023-05-21 13:19:09.623216 command_line_loom-0.0.8/cll/data_structs/loom_index.py
+-rw-r--r--   0        0        0     2493 2023-05-19 17:01:41.546225 command_line_loom-0.0.8/cll/data_structs/node.py
+-rwxr-xr-x   0        0        0     4162 2023-05-21 14:03:25.003785 command_line_loom-0.0.8/cll/encoder.py
+-rw-r--r--   0        0        0     1025 2023-05-19 13:37:16.690088 command_line_loom-0.0.8/cll/io.py
+-rw-r--r--   0        0        0     2381 2023-05-19 21:14:40.203467 command_line_loom-0.0.8/cll/store.py
+-rw-r--r--   0        0        0     7963 2023-05-19 21:14:40.203467 command_line_loom-0.0.8/cll/templater.py
+-rw-r--r--   0        0        0    19129 2023-05-21 14:31:44.323307 command_line_loom-0.0.8/cll/tree.py
+-rw-r--r--   0        0        0     1052 2023-05-21 14:32:03.535097 command_line_loom-0.0.8/pyproject.toml
+-rw-r--r--   0        0        0     2913 1970-01-01 00:00:00.000000 command_line_loom-0.0.8/PKG-INFO
```

### Comparing `command_line_loom-0.0.7/LICENSE` & `command_line_loom-0.0.8/LICENSE`

 * *Files identical despite different names*

### Comparing `command_line_loom-0.0.7/README.md` & `command_line_loom-0.0.8/README.md`

 * *Files identical despite different names*

### Comparing `command_line_loom-0.0.7/cll/__main__.py` & `command_line_loom-0.0.8/cll/__main__.py`

 * *Files identical despite different names*

### Comparing `command_line_loom-0.0.7/cll/app.py` & `command_line_loom-0.0.8/cll/app.py`

 * *Files identical despite different names*

### Comparing `command_line_loom-0.0.7/cll/config.py` & `command_line_loom-0.0.8/cll/config.py`

 * *Files identical despite different names*

### Comparing `command_line_loom-0.0.7/cll/data_structs/data_structs.py` & `command_line_loom-0.0.8/cll/data_structs/data_structs.py`

 * *Files identical despite different names*

### Comparing `command_line_loom-0.0.7/cll/data_structs/loom_index.py` & `command_line_loom-0.0.8/cll/data_structs/loom_index.py`

 * *Files identical despite different names*

### Comparing `command_line_loom-0.0.7/cll/data_structs/node.py` & `command_line_loom-0.0.8/cll/data_structs/node.py`

 * *Files identical despite different names*

### Comparing `command_line_loom-0.0.7/cll/encoder.py` & `command_line_loom-0.0.8/cll/encoder.py`

 * *Files identical despite different names*

### Comparing `command_line_loom-0.0.7/cll/io.py` & `command_line_loom-0.0.8/cll/io.py`

 * *Files identical despite different names*

### Comparing `command_line_loom-0.0.7/cll/store.py` & `command_line_loom-0.0.8/cll/store.py`

 * *Files identical despite different names*

### Comparing `command_line_loom-0.0.7/cll/templater.py` & `command_line_loom-0.0.8/cll/templater.py`

 * *Files identical despite different names*

### Comparing `command_line_loom-0.0.7/cll/tree.py` & `command_line_loom-0.0.8/cll/tree.py`

 * *Files 0% similar despite different names*

```diff
@@ -525,15 +525,15 @@
         indexes = indexes.split(" ")
     return [int(index) if index.isdigit() else index for index in indexes]
 
 
 @cli.command()
 @cli.command(name="del", hidden=True)
 def delete(ctx: Context, indexes: Annotated[Optional[str], Argument()] = None, all: bool = False):
-    "(del) delete some nodes (space separated) (last one by default)"
+    "(del) delete some nodes (space separated) (last one by default) (and subnodes if --all)"
     if not indexes:
         indexes = [ctx.obj.tree.index.path[-1].index]
     else:
         indexes = parse_indexes(indexes)
     ctx.obj.tree.index.delete(indexes, all=all)
 
 
@@ -545,15 +545,15 @@
     ctx.obj.tree.index.cherry_pick(indexes)
     path_with_current(ctx)
 
 
 @cli.command()
 @cli.command(name="hh", hidden=True)
 def hoist(ctx: Context, target: Annotated[Optional[str], Argument()] = None):
-    "Copies the node and all downstreams to a new root."
+    "(hh) Copies the node and all downstreams to a new root (or to a target if specified)."
     index = ctx.obj.tree.index.path[-1].index
     ctx.obj.tree.index.hoist(index, target)
     path_with_current(ctx)
 
 
 @cli.command()
 def dump(ctx: Context):
```

### Comparing `command_line_loom-0.0.7/pyproject.toml` & `command_line_loom-0.0.8/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "command-line-loom"
-version = "0.0.7"
+version = "0.0.8"
 description = ""
 authors = ["fergus <fergusfettes@gmail.com>"]
 homepage = "https://github.com/fergusfettes/command-line-loom"
 readme = "README.md"
 packages = [{include = "cll"}]
 
 [tool.poetry.dependencies]
```

### Comparing `command_line_loom-0.0.7/PKG-INFO` & `command_line_loom-0.0.8/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: command-line-loom
-Version: 0.0.7
+Version: 0.0.8
 Summary: 
 Home-page: https://github.com/fergusfettes/command-line-loom
 Author: fergus
 Author-email: fergusfettes@gmail.com
 Requires-Python: >=3.8.1,<3.12
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
```

