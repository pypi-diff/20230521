# Comparing `tmp/mkdocs_entangled_plugin-0.2.0.tar.gz` & `tmp/mkdocs_entangled_plugin-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mkdocs_entangled_plugin-0.2.0.tar", max compression
+gzip compressed data, was "mkdocs_entangled_plugin-0.3.0.tar", max compression
```

## Comparing `mkdocs_entangled_plugin-0.2.0.tar` & `mkdocs_entangled_plugin-0.3.0.tar`

### file list

```diff
@@ -1,11 +1,11 @@
--rw-r--r--   0        0        0    11357 2023-05-03 23:56:27.577268 mkdocs_entangled_plugin-0.2.0/LICENSE
--rw-r--r--   0        0        0     1462 2023-05-03 23:56:27.577268 mkdocs_entangled_plugin-0.2.0/README.md
--rw-r--r--   0        0        0       67 2023-05-03 23:56:27.581268 mkdocs_entangled_plugin-0.2.0/mkdocs_entangled/__init__.py
--rw-r--r--   0        0        0       79 2023-05-03 23:56:27.581268 mkdocs_entangled_plugin-0.2.0/mkdocs_entangled/config.py
--rw-r--r--   0        0        0     3191 2023-05-03 23:56:27.581268 mkdocs_entangled_plugin-0.2.0/mkdocs_entangled/mawk.py
--rw-r--r--   0        0        0     3007 2023-05-03 23:56:27.581268 mkdocs_entangled_plugin-0.2.0/mkdocs_entangled/on_page_markdown.py
--rw-r--r--   0        0        0      474 2023-05-03 23:56:27.581268 mkdocs_entangled_plugin-0.2.0/mkdocs_entangled/plugin.py
--rw-r--r--   0        0        0     2892 2023-05-03 23:56:27.581268 mkdocs_entangled_plugin-0.2.0/mkdocs_entangled/properties.py
--rw-r--r--   0        0        0        0 2023-05-03 23:56:27.581268 mkdocs_entangled_plugin-0.2.0/mkdocs_entangled/py.typed
--rw-r--r--   0        0        0      814 2023-05-03 23:56:27.581268 mkdocs_entangled_plugin-0.2.0/pyproject.toml
--rw-r--r--   0        0        0     2158 1970-01-01 00:00:00.000000 mkdocs_entangled_plugin-0.2.0/PKG-INFO
+-rw-r--r--   0        0        0    11357 2023-05-20 22:54:50.985888 mkdocs_entangled_plugin-0.3.0/LICENSE
+-rw-r--r--   0        0        0     2033 2023-05-20 22:54:50.985888 mkdocs_entangled_plugin-0.3.0/README.md
+-rw-r--r--   0        0        0       67 2023-05-20 22:54:50.989888 mkdocs_entangled_plugin-0.3.0/mkdocs_entangled/__init__.py
+-rw-r--r--   0        0        0       79 2023-05-20 22:54:50.989888 mkdocs_entangled_plugin-0.3.0/mkdocs_entangled/config.py
+-rw-r--r--   0        0        0     3191 2023-05-20 22:54:50.989888 mkdocs_entangled_plugin-0.3.0/mkdocs_entangled/mawk.py
+-rw-r--r--   0        0        0     1919 2023-05-20 22:54:50.989888 mkdocs_entangled_plugin-0.3.0/mkdocs_entangled/on_page_markdown.py
+-rw-r--r--   0        0        0      706 2023-05-20 22:54:50.989888 mkdocs_entangled_plugin-0.3.0/mkdocs_entangled/plugin.py
+-rw-r--r--   0        0        0     2892 2023-05-20 22:54:50.989888 mkdocs_entangled_plugin-0.3.0/mkdocs_entangled/properties.py
+-rw-r--r--   0        0        0        0 2023-05-20 22:54:50.989888 mkdocs_entangled_plugin-0.3.0/mkdocs_entangled/py.typed
+-rw-r--r--   0        0        0      952 2023-05-20 22:54:50.989888 mkdocs_entangled_plugin-0.3.0/pyproject.toml
+-rw-r--r--   0        0        0     2588 1970-01-01 00:00:00.000000 mkdocs_entangled_plugin-0.3.0/PKG-INFO
```

### Comparing `mkdocs_entangled_plugin-0.2.0/LICENSE` & `mkdocs_entangled_plugin-0.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `mkdocs_entangled_plugin-0.2.0/mkdocs_entangled/mawk.py` & `mkdocs_entangled_plugin-0.3.0/mkdocs_entangled/mawk.py`

 * *Files identical despite different names*

### Comparing `mkdocs_entangled_plugin-0.2.0/mkdocs_entangled/on_page_markdown.py` & `mkdocs_entangled_plugin-0.3.0/mkdocs_entangled/on_page_markdown.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,30 +1,22 @@
 from typing import Optional
 from dataclasses import dataclass
-from pathlib import Path
 import re
-import tempfile
-import subprocess
-import sys
 
 from mkdocs.config.defaults import MkDocsConfig
 from mkdocs.structure.pages import Page
 from mkdocs.structure.files import Files
 
-from .config import EntangledConfig
-from .properties import read_properties, Id, Attribute, Class
+from .properties import read_properties, Id, Attribute
 from . import mawk
 
 
 @dataclass
 class EntangledFilter(mawk.RuleSet):
     add_title: bool = True
-    build_artifacts: bool = True
-
-    _collect_make_script: bool = False
     _ignore: bool = False
 
     @mawk.on_match(r"~~~markdown")
     def start_ignore(self, m):
         self._ignore = True
         return [m[0]]
     
@@ -54,39 +46,19 @@
                 title = f"file: {filenames[0]}"
             elif len(ids) > 1 or len(filenames) > 1:
                 title = f"error: ambiguous code block title"
 
             if title is not None:
                 props.append(Attribute("title", title))
         
-        if self.build_artifacts and Class("build-artifact") in props:
-            self._collect_make_script = True
-            self._make_script: list[str] = []
-            self._make_props = props
-            self._indent = indent
-
         prop_str = " ".join(str(p) for p in props)
         return [f"{indent}``` {{{prop_str}}}"]
 
     @mawk.on_match(r"\s*```\s*$")
     def close_code_block(self, m: re.Match) -> Optional[list[str]]:
-        if not self._ignore and self._collect_make_script:
-            self._collect_make_script = False
-            script = "\n".join(self._make_script)
-            with tempfile.TemporaryDirectory() as _tmpdir:
-                tmpdir = Path(_tmpdir)
-                with open(tmpdir / "Makefile", "w") as makefile:
-                    makefile.write(script)
-                subprocess.run(["make", "-f", str(tmpdir / "Makefile")])
-        return None
-
-    @mawk.always
-    def add_line_to_script(self, line: str) -> Optional[list[str]]:
-        if not self._ignore and self._collect_make_script:
-            self._make_script.append(line.removeprefix(self._indent))
         return None
 
 
 def on_page_markdown(markdown: str, *, page: Page, config: MkDocsConfig, files: Files) -> str:
     result = EntangledFilter().run(markdown)
     return result
```

### Comparing `mkdocs_entangled_plugin-0.2.0/mkdocs_entangled/properties.py` & `mkdocs_entangled_plugin-0.3.0/mkdocs_entangled/properties.py`

 * *Files identical despite different names*

### Comparing `mkdocs_entangled_plugin-0.2.0/pyproject.toml` & `mkdocs_entangled_plugin-0.3.0/pyproject.toml`

 * *Files 11% similar despite different names*

```diff
@@ -1,24 +1,26 @@
 [tool.poetry]
 name = "mkdocs-entangled-plugin"
-version = "0.2.0"
+version = "0.3.0"
 description = "Plugin for MkDocs helping with rendering Entangled (entangled.github.io) projects."
 readme = "README.md"
 authors = ["Johan Hidding <j.hidding@esciencecenter.nl>"]
 license = "Apache 2.0"
 packages = [
     { include = "mkdocs_entangled" }
 ]
 
 [tool.poetry.plugins."mkdocs.plugins"]
 entangled = "mkdocs_entangled:EntangledPlugin"
 
 [tool.poetry.dependencies]
-python = ">=3.7"
+python = "^3.11"
 mkdocs = "^1.4.2"
+# entangled-cli = {path = "../entangled.py", extras = ["rich"], develop = true}
+entangled-cli = {extras = ["rich"], version = "^2.0.0a3"}
 
 [tool.poetry.dev-dependencies]
 mypy = "^1.2.0"
 pytest = "^7.3.0"
 pytest-mypy = "^0.10.3"
 mkdocs-material = "^9.1.6"
 twine = "^4.0.2"
```

### Comparing `mkdocs_entangled_plugin-0.2.0/PKG-INFO` & `mkdocs_entangled_plugin-0.3.0/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,22 +1,19 @@
 Metadata-Version: 2.1
 Name: mkdocs-entangled-plugin
-Version: 0.2.0
+Version: 0.3.0
 Summary: Plugin for MkDocs helping with rendering Entangled (entangled.github.io) projects.
 License: Apache 2.0
 Author: Johan Hidding
 Author-email: j.hidding@esciencecenter.nl
-Requires-Python: >=3.7
+Requires-Python: >=3.11,<4.0
 Classifier: License :: Other/Proprietary License
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.7
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
-Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
+Requires-Dist: entangled-cli[rich] (>=2.0.0a3,<3.0.0)
 Requires-Dist: mkdocs (>=1.4.2,<2.0.0)
 Description-Content-Type: text/markdown
 
 # Welcome to MkDocs Entangled Plugin
 Using this plugin, you can make your Entangled documents look better.
 
 ## Install
@@ -29,27 +26,33 @@
 
 markdown_extensions:
   - pymdownx.superfences
   - pymdownx.tabbed:
       alternate_style: true 
 ```
 
-## Annotates codeblocks
+## Components
+This plugin bundles functionality for literate programming with Entangled.
+
+- Annotate code blocks with titles.
+- Build artifacts using Make.
+
+### Annotate code blocks
 The default markdown syntax that Entangled supports has fenced code blocks as follows
 
 ~~~markdown
-``` {.python file=hello_world.py}
+``` {.python file=examples/hello_world.py}
 if __name__ == "__main__":
     <<hello-world>>
 ```
 ~~~
 
 Which renders like this:
 
-``` {.python file=hello_world.py}
+``` {.python file=examples/hello_world.py}
 if __name__ == "__main__":
     <<hello-world>>
 ```
 
 Or named code blocks
 
 ~~~markdown
@@ -57,47 +60,63 @@
 print("Hello, World!")
 ```
 ~~~
 
 that render like this:
 
 ``` {.python #hello-world}
-print("Hello, World!")
+print("Hello, Universe!")
 ```
 
-## Build Artifacts
+### Build Artifacts
 
 Build artifacts by specifying a Makefile.
 
 ~~~markdown
 === "Figure 1"
 
     ![](fig/plot.svg)
 
-=== "Makefile"
+=== "Source"
+
+    ``` {.gnuplot file=examples/plot.gp}
+    # enter your plotting commands here
+    ```
 
     ``` {.make .build-artifact}
     .RECIPEPREFIX = >
   
-    docs/fig/plot.svg:
+    docs/fig/plot.svg: examples/plot.gp
     > mkdir -p $(@D)
-    > gnuplot -e "set term svg; plot sin(x)" > $@
+    > gnuplot $^ > $@
     ```
 ~~~
 
 === "Figure 1"
 
     ![](fig/plot.svg)
 
-=== "Makefile"
+=== "Source"
+
+    ``` {.gnuplot file=examples/plot.gp}
+    set term svg background rgb 'white' size 700, 500
+    sinc(r) = sin(pi*r) / (pi*r)
+    set isosamples 50, 50
+    set hidden3d
+    set xrange [-4:4]
+    set yrange [-4:4]
+    set xyplane 0
+    set title "Sinc function"
+    splot sinc(sqrt(x**2 + y**2)) t'' lc rgb '#5533cc'
+    ```
 
     ``` {.make .build-artifact}
     .RECIPEPREFIX = >
   
-    docs/fig/plot.svg:
+    docs/fig/plot.svg: examples/plot.gp
     > mkdir -p $(@D)
-    > gnuplot -e "set term svg; plot sin(x)" > $@
+    > gnuplot $^ > $@
     ```
 
 ## License
 Licensed under the Apache-2 license agreement: see LICENSE
```

