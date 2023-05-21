# Comparing `tmp/cz_conventional_gitmoji-0.1.3.tar.gz` & `tmp/cz_conventional_gitmoji-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cz_conventional_gitmoji-0.1.3.tar", max compression
+gzip compressed data, was "cz_conventional_gitmoji-0.2.0.tar", max compression
```

## Comparing `cz_conventional_gitmoji-0.1.3.tar` & `cz_conventional_gitmoji-0.2.0.tar`

### file list

```diff
@@ -1,13 +1,13 @@
--rw-r--r--   0        0        0     2506 2022-12-25 17:16:10.733756 cz_conventional_gitmoji-0.1.3/README.md
--rw-r--r--   0        0        0     2371 2023-05-02 09:19:44.196072 cz_conventional_gitmoji-0.1.3/pyproject.toml
--rw-r--r--   0        0        0       85 2022-12-22 20:59:18.556559 cz_conventional_gitmoji-0.1.3/src/cz_gitmoji/__init__.py
--rw-r--r--   0        0        0     1285 2022-12-22 20:59:18.556559 cz_conventional_gitmoji-0.1.3/src/cz_gitmoji/conventional_gitmojis_info.txt
--rw-r--r--   0        0        0    13515 2022-12-27 13:40:50.852366 cz_conventional_gitmoji-0.1.3/src/cz_gitmoji/main.py
--rw-r--r--   0        0        0        0 2022-12-22 20:59:18.556559 cz_conventional_gitmoji-0.1.3/src/gitmojify/__init__.py
--rw-r--r--   0        0        0     1669 2022-12-27 01:28:48.481457 cz_conventional_gitmoji-0.1.3/src/gitmojify/mojify.py
--rw-r--r--   0        0        0        0 2022-12-22 20:59:18.556559 cz_conventional_gitmoji-0.1.3/src/shared/__init__.py
--rw-r--r--   0        0        0     2667 2022-12-23 22:03:29.325029 cz_conventional_gitmoji-0.1.3/src/shared/gitmojis.py
--rw-r--r--   0        0        0      406 2022-12-22 20:59:18.556559 cz_conventional_gitmoji-0.1.3/src/shared/model.py
--rw-r--r--   0        0        0    10608 2022-12-27 01:28:48.481457 cz_conventional_gitmoji-0.1.3/src/shared/spec.py
--rw-r--r--   0        0        0      817 2022-12-27 01:28:48.481457 cz_conventional_gitmoji-0.1.3/src/shared/utils.py
--rw-r--r--   0        0        0     3362 1970-01-01 00:00:00.000000 cz_conventional_gitmoji-0.1.3/PKG-INFO
+-rw-r--r--   0        0        0     2506 2023-05-21 14:39:38.339405 cz_conventional_gitmoji-0.2.0/README.md
+-rw-r--r--   0        0        0     2464 2023-05-21 14:39:38.339405 cz_conventional_gitmoji-0.2.0/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-05-21 14:39:38.339405 cz_conventional_gitmoji-0.2.0/src/cz_gitmoji/__init__.py
+-rw-r--r--   0        0        0     1285 2023-05-21 14:39:38.339405 cz_conventional_gitmoji-0.2.0/src/cz_gitmoji/conventional_gitmojis_info.txt
+-rw-r--r--   0        0        0    13515 2023-05-21 14:39:38.339405 cz_conventional_gitmoji-0.2.0/src/cz_gitmoji/main.py
+-rw-r--r--   0        0        0        0 2023-05-21 14:39:38.339405 cz_conventional_gitmoji-0.2.0/src/gitmojify/__init__.py
+-rw-r--r--   0        0        0     1669 2023-05-21 14:39:38.339405 cz_conventional_gitmoji-0.2.0/src/gitmojify/mojify.py
+-rw-r--r--   0        0        0        0 2023-05-21 14:39:38.339405 cz_conventional_gitmoji-0.2.0/src/shared/__init__.py
+-rw-r--r--   0        0        0     2667 2023-05-21 14:39:38.339405 cz_conventional_gitmoji-0.2.0/src/shared/gitmojis.py
+-rw-r--r--   0        0        0      406 2023-05-21 14:39:38.339405 cz_conventional_gitmoji-0.2.0/src/shared/model.py
+-rw-r--r--   0        0        0    10608 2023-05-21 14:39:38.339405 cz_conventional_gitmoji-0.2.0/src/shared/spec.py
+-rw-r--r--   0        0        0      817 2023-05-21 14:39:38.339405 cz_conventional_gitmoji-0.2.0/src/shared/utils.py
+-rw-r--r--   0        0        0     3361 1970-01-01 00:00:00.000000 cz_conventional_gitmoji-0.2.0/PKG-INFO
```

### Comparing `cz_conventional_gitmoji-0.1.3/README.md` & `cz_conventional_gitmoji-0.2.0/README.md`

 * *Files identical despite different names*

### Comparing `cz_conventional_gitmoji-0.1.3/pyproject.toml` & `cz_conventional_gitmoji-0.2.0/pyproject.toml`

 * *Files 3% similar despite different names*

```diff
@@ -1,39 +1,42 @@
 [tool.poetry]
 name = "cz-conventional-gitmoji"
-version = "0.1.3"
+version = "0.2.0"
 description = "A commitizen plugin that combines gitmoji and conventional."
 authors = ["ljnsn <82611987+ljnsn@users.noreply.github.com>"]
 license = "MIT"
 readme = "README.md"
 packages = [
   {include = "shared", from = "src"},
   {include = "cz_gitmoji", from = "src"},
   {include = "gitmojify", from = "src"}
 ]
 repository = "https://github.com/ljnsn/cz-conventional-gitmoji"
 
+[tool.poetry.plugins."commitizen.plugin"]
+cz_gitmoji = "cz_gitmoji.main:CommitizenGitmojiCz"
+
 [tool.poetry.scripts]
 gitmojify = "gitmojify.mojify:run"
 
 [tool.poetry.dependencies]
 python = "^3.7"
-commitizen = "^2.42.0"
+commitizen = "^3.2.2"
 attrs = "^23.1.0"
 
 [tool.poetry.group.dev.dependencies]
 black = ">=22.12,<24.0"
 pytest = "^7.2.0"
 pytest-cov = "^4.0.0"
 coverage = {extras = ["toml"], version = "^7.0.1"}
-ruff = ">=0.0.246,<0.0.264"
+ruff = ">=0.0.246,<0.0.270"
 
 [tool.commitizen]
 name = "cz_gitmoji"
-version = "0.1.3"
+version = "0.2.0"
 bump_message = "🔖 bump(release): v$current_version → v$new_version"
 tag_format = "v$version"
 version_files = ["pyproject.toml:^version"]
 update_changelog_on_bump = true
 
 [tool.black]
 target-version = ["py37", "py38", "py39", "py310", "py311"]
```

### Comparing `cz_conventional_gitmoji-0.1.3/src/cz_gitmoji/conventional_gitmojis_info.txt` & `cz_conventional_gitmoji-0.2.0/src/cz_gitmoji/conventional_gitmojis_info.txt`

 * *Files identical despite different names*

### Comparing `cz_conventional_gitmoji-0.1.3/src/cz_gitmoji/main.py` & `cz_conventional_gitmoji-0.2.0/src/cz_gitmoji/main.py`

 * *Files identical despite different names*

### Comparing `cz_conventional_gitmoji-0.1.3/src/gitmojify/mojify.py` & `cz_conventional_gitmoji-0.2.0/src/gitmojify/mojify.py`

 * *Files identical despite different names*

### Comparing `cz_conventional_gitmoji-0.1.3/src/shared/gitmojis.py` & `cz_conventional_gitmoji-0.2.0/src/shared/gitmojis.py`

 * *Files identical despite different names*

### Comparing `cz_conventional_gitmoji-0.1.3/src/shared/spec.py` & `cz_conventional_gitmoji-0.2.0/src/shared/spec.py`

 * *Files identical despite different names*

### Comparing `cz_conventional_gitmoji-0.1.3/src/shared/utils.py` & `cz_conventional_gitmoji-0.2.0/src/shared/utils.py`

 * *Files identical despite different names*

### Comparing `cz_conventional_gitmoji-0.1.3/PKG-INFO` & `cz_conventional_gitmoji-0.2.0/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 Metadata-Version: 2.1
 Name: cz-conventional-gitmoji
-Version: 0.1.3
+Version: 0.2.0
 Summary: A commitizen plugin that combines gitmoji and conventional.
 Home-page: https://github.com/ljnsn/cz-conventional-gitmoji
 License: MIT
 Author: ljnsn
 Author-email: 82611987+ljnsn@users.noreply.github.com
 Requires-Python: >=3.7,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: attrs (>=23.1.0,<24.0.0)
-Requires-Dist: commitizen (>=2.42.0,<3.0.0)
+Requires-Dist: commitizen (>=3.2.2,<4.0.0)
 Project-URL: Repository, https://github.com/ljnsn/cz-conventional-gitmoji
 Description-Content-Type: text/markdown
 
 # cz-conventional-gitmoji
 
 A [commitizen](https://github.com/commitizen-tools/commitizen) plugin that combines [gitmoji](https://gitmoji.dev/) and [conventional commits](https://www.conventionalcommits.org/en/v1.0.0/).
```

