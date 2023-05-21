# Comparing `tmp/facere_sensum-0.0.1.tar.gz` & `tmp/facere_sensum-0.0.2.tar.gz`

## Comparing `facere_sensum-0.0.1.tar` & `facere_sensum-0.0.2.tar`

### file list

```diff
@@ -1,7 +1,15 @@
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 facere_sensum-0.0.1/src/facere-sensum/__init__.py
--rw-r--r--   0        0        0       17 2020-02-02 00:00:00.000000 facere_sensum-0.0.1/src/facere-sensum/facere-sensum.py
--rw-r--r--   0        0        0     1799 2020-02-02 00:00:00.000000 facere_sensum-0.0.1/.gitignore
--rw-r--r--   0        0        0     1068 2020-02-02 00:00:00.000000 facere_sensum-0.0.1/LICENSE
--rw-r--r--   0        0        0       42 2020-02-02 00:00:00.000000 facere_sensum-0.0.1/README.md
--rw-r--r--   0        0        0      659 2020-02-02 00:00:00.000000 facere_sensum-0.0.1/pyproject.toml
--rw-r--r--   0        0        0      546 2020-02-02 00:00:00.000000 facere_sensum-0.0.1/PKG-INFO
+-rw-r--r--   0        0        0      139 2020-02-02 00:00:00.000000 facere_sensum-0.0.2/log.csv
+-rw-r--r--   0        0        0       31 2020-02-02 00:00:00.000000 facere_sensum-0.0.2/requirements.txt
+-rw-r--r--   0        0        0      606 2020-02-02 00:00:00.000000 facere_sensum-0.0.2/.github/workflows/lints.yaml
+-rw-r--r--   0        0        0      405 2020-02-02 00:00:00.000000 facere_sensum-0.0.2/.github/workflows/test.yaml
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 facere_sensum-0.0.2/src/facere_sensum/__init__.py
+-rw-r--r--   0        0        0     3531 2020-02-02 00:00:00.000000 facere_sensum-0.0.2/src/facere_sensum/facere_sensum.py
+-rw-r--r--   0        0        0      390 2020-02-02 00:00:00.000000 facere_sensum-0.0.2/src/facere_sensum/test.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 facere_sensum-0.0.2/test/__init__.py
+-rw-r--r--   0        0        0      276 2020-02-02 00:00:00.000000 facere_sensum-0.0.2/test/ref.csv
+-rw-r--r--   0        0        0     1372 2020-02-02 00:00:00.000000 facere_sensum-0.0.2/test/test.py
+-rw-r--r--   0        0        0     1799 2020-02-02 00:00:00.000000 facere_sensum-0.0.2/.gitignore
+-rw-r--r--   0        0        0     1068 2020-02-02 00:00:00.000000 facere_sensum-0.0.2/LICENSE
+-rw-r--r--   0        0        0     4688 2020-02-02 00:00:00.000000 facere_sensum-0.0.2/README.md
+-rw-r--r--   0        0        0      777 2020-02-02 00:00:00.000000 facere_sensum-0.0.2/pyproject.toml
+-rw-r--r--   0        0        0     5192 2020-02-02 00:00:00.000000 facere_sensum-0.0.2/PKG-INFO
```

### Comparing `facere_sensum-0.0.1/.gitignore` & `facere_sensum-0.0.2/.gitignore`

 * *Files identical despite different names*

### Comparing `facere_sensum-0.0.1/LICENSE` & `facere_sensum-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `facere_sensum-0.0.1/pyproject.toml` & `facere_sensum-0.0.2/pyproject.toml`

 * *Files 24% similar despite different names*

```diff
@@ -1,25 +1,31 @@
-[build-system]
-requires = ["hatchling"]
-build-backend = "hatchling.build"
-
-[project]
-name = "facere-sensum"
-dynamic = ["version"]
-authors = [
-  { name = "Serge Lunev" },
-]
-description = "facere-sensum: make sense of the turmoil"
-readme = "README.md"
-requires-python = ">=3.11"
-classifiers = [
-    "Programming Language :: Python :: 3",
-    "License :: OSI Approved :: MIT License",
-    "Operating System :: OS Independent",
-]
-
-[project.urls]
-"Homepage" = "https://github.com/lunarserge/facere-sensum"
-"Bug Tracker" = "https://github.com/lunarserge/facere-sensum/issues"
-
-[tool.hatch.version]
-path = "src/facere-sensum/facere-sensum.py"
+[build-system]
+requires = ["hatchling"]
+build-backend = "hatchling.build"
+
+[project]
+name = "facere-sensum"
+dynamic = ["version"]
+authors = [
+  { name = "Serge Lunev" },
+]
+description = "facere-sensum: make sense of the turmoil"
+readme = "README.md"
+requires-python = ">=3.11"
+classifiers = [
+    "Programming Language :: Python :: 3",
+    "License :: OSI Approved :: MIT License",
+    "Operating System :: OS Independent",
+]
+
+[project.urls]
+"Homepage" = "https://github.com/lunarserge/facere-sensum"
+"Bug Tracker" = "https://github.com/lunarserge/facere-sensum/issues"
+
+[project.scripts]
+facere-sensum = "facere_sensum.facere_sensum:main"
+
+[tool.hatch.version]
+path = "src/facere_sensum/facere_sensum.py"
+
+[tool.setuptools.dynamic]
+dependencies = {file = ["requirements.txt"]}
```

