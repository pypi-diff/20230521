# Comparing `tmp/awesomeversion-22.9.0.tar.gz` & `tmp/awesomeversion-23.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "awesomeversion-22.9.0.tar", max compression
+gzip compressed data, was "awesomeversion-23.5.0.tar", max compression
```

## Comparing `awesomeversion-22.9.0.tar` & `awesomeversion-23.5.0.tar`

### file list

```diff
@@ -1,18 +1,17 @@
--rw-r--r--   0        0        0     1076 2022-09-15 10:13:24.918257 awesomeversion-22.9.0/LICENCE.md
--rw-r--r--   0        0        0     3192 2022-09-15 10:13:24.918257 awesomeversion-22.9.0/README.md
--rw-r--r--   0        0        0      536 2022-09-15 10:13:24.918257 awesomeversion-22.9.0/awesomeversion/__init__.py
--rw-r--r--   0        0        0    16876 2022-09-15 10:13:24.918257 awesomeversion-22.9.0/awesomeversion/awesomeversion.py
--rw-r--r--   0        0        0       57 2022-09-15 10:13:24.918257 awesomeversion-22.9.0/awesomeversion/comparehandlers/__init__.py
--rw-r--r--   0        0        0      849 2022-09-15 10:13:24.918257 awesomeversion-22.9.0/awesomeversion/comparehandlers/container.py
--rw-r--r--   0        0        0     1835 2022-09-15 10:13:24.922257 awesomeversion-22.9.0/awesomeversion/comparehandlers/modifier.py
--rw-r--r--   0        0        0     2557 2022-09-15 10:13:24.922257 awesomeversion-22.9.0/awesomeversion/comparehandlers/sections.py
--rw-r--r--   0        0        0      478 2022-09-15 10:13:24.922257 awesomeversion-22.9.0/awesomeversion/comparehandlers/simple.py
--rw-r--r--   0        0        0      360 2022-09-15 10:13:24.922257 awesomeversion-22.9.0/awesomeversion/exceptions.py
--rw-r--r--   0        0        0        0 2022-09-15 10:13:24.922257 awesomeversion-22.9.0/awesomeversion/py.typed
--rw-r--r--   0        0        0     2323 2022-09-15 10:13:24.922257 awesomeversion-22.9.0/awesomeversion/strategy.py
--rw-r--r--   0        0        0      499 2022-09-15 10:13:24.922257 awesomeversion-22.9.0/awesomeversion/typing.py
--rw-r--r--   0        0        0        0 2022-09-15 10:13:24.922257 awesomeversion-22.9.0/awesomeversion/utils/__init__.py
--rw-r--r--   0        0        0     1126 2022-09-15 10:13:24.922257 awesomeversion-22.9.0/awesomeversion/utils/regex.py
--rw-r--r--   0        0        0     1315 2022-09-15 10:13:38.631431 awesomeversion-22.9.0/pyproject.toml
--rw-r--r--   0        0        0     4077 1970-01-01 00:00:00.000000 awesomeversion-22.9.0/setup.py
--rw-r--r--   0        0        0     4223 1970-01-01 00:00:00.000000 awesomeversion-22.9.0/PKG-INFO
+-rw-r--r--   0        0        0     1076 2023-05-21 11:01:16.699400 awesomeversion-23.5.0/LICENCE.md
+-rw-r--r--   0        0        0     7896 2023-05-21 11:01:16.699400 awesomeversion-23.5.0/README.md
+-rw-r--r--   0        0        0      536 2023-05-21 11:01:16.699400 awesomeversion-23.5.0/awesomeversion/__init__.py
+-rw-r--r--   0        0        0    17492 2023-05-21 11:01:16.699400 awesomeversion-23.5.0/awesomeversion/awesomeversion.py
+-rw-r--r--   0        0        0       57 2023-05-21 11:01:16.699400 awesomeversion-23.5.0/awesomeversion/comparehandlers/__init__.py
+-rw-r--r--   0        0        0      849 2023-05-21 11:01:16.699400 awesomeversion-23.5.0/awesomeversion/comparehandlers/container.py
+-rw-r--r--   0        0        0     1835 2023-05-21 11:01:16.699400 awesomeversion-23.5.0/awesomeversion/comparehandlers/modifier.py
+-rw-r--r--   0        0        0     2557 2023-05-21 11:01:16.699400 awesomeversion-23.5.0/awesomeversion/comparehandlers/sections.py
+-rw-r--r--   0        0        0      478 2023-05-21 11:01:16.699400 awesomeversion-23.5.0/awesomeversion/comparehandlers/simple.py
+-rw-r--r--   0        0        0      360 2023-05-21 11:01:16.699400 awesomeversion-23.5.0/awesomeversion/exceptions.py
+-rw-r--r--   0        0        0        0 2023-05-21 11:01:16.699400 awesomeversion-23.5.0/awesomeversion/py.typed
+-rw-r--r--   0        0        0     2323 2023-05-21 11:01:16.699400 awesomeversion-23.5.0/awesomeversion/strategy.py
+-rw-r--r--   0        0        0      499 2023-05-21 11:01:16.699400 awesomeversion-23.5.0/awesomeversion/typing.py
+-rw-r--r--   0        0        0        0 2023-05-21 11:01:16.699400 awesomeversion-23.5.0/awesomeversion/utils/__init__.py
+-rw-r--r--   0        0        0     1126 2023-05-21 11:01:16.699400 awesomeversion-23.5.0/awesomeversion/utils/regex.py
+-rw-r--r--   0        0        0     1337 2023-05-21 11:01:33.595716 awesomeversion-23.5.0/pyproject.toml
+-rw-r--r--   0        0        0     8978 1970-01-01 00:00:00.000000 awesomeversion-23.5.0/PKG-INFO
```

### Comparing `awesomeversion-22.9.0/LICENCE.md` & `awesomeversion-23.5.0/LICENCE.md`

 * *Files identical despite different names*

### Comparing `awesomeversion-22.9.0/awesomeversion/__init__.py` & `awesomeversion-23.5.0/awesomeversion/__init__.py`

 * *Files identical despite different names*

### Comparing `awesomeversion-22.9.0/awesomeversion/awesomeversion.py` & `awesomeversion-23.5.0/awesomeversion/awesomeversion.py`

 * *Files 5% similar despite different names*

```diff
@@ -142,15 +142,15 @@
             self._version = self._version[:-1]
 
         super().__init__(self._version)
 
     def __enter__(self) -> AwesomeVersion:
         return self
 
-    def __exit__(self, *_: Any, **__: Any) -> bool:
+    def __exit__(self, *_: Any, **__: Any) -> None:
         pass
 
     def __repr__(self) -> str:
         return f"<AwesomeVersion {self.strategy.value} '{self.string}'>"
 
     def __str__(self) -> str:
         return str(self._version)
@@ -219,14 +219,26 @@
                 "minor": self.minor != compareto.minor,
                 "patch": self.patch != compareto.patch,
                 "modifier": self.modifier != compareto.modifier,
                 "strategy": self.strategy != compareto.strategy,
             }
         )
 
+    def in_range(self, lowest: VersionType, highest: VersionType) -> bool:
+        """Check if version is in range."""
+        if isinstance(lowest, (str, float, int)):
+            lowest = AwesomeVersion(lowest)
+        if isinstance(highest, (str, float, int)):
+            highest = AwesomeVersion(highest)
+        if not isinstance(lowest, AwesomeVersion):
+            raise AwesomeVersionCompareException("Lowest version is not valid")
+        if not isinstance(highest, AwesomeVersion):
+            raise AwesomeVersionCompareException("Highest version is not valid")
+        return lowest <= self <= highest
+
     def section(self, idx: int) -> int:
         """Return the value of the specified section of the version."""
         if self.sections >= (idx + 1):
             match = RE_DIGIT.match(self.string.split(".")[idx] or "")
             if match and match.groups():
                 return int(match.group(1) or 0)
         return 0
```

### Comparing `awesomeversion-22.9.0/awesomeversion/comparehandlers/container.py` & `awesomeversion-23.5.0/awesomeversion/comparehandlers/container.py`

 * *Files identical despite different names*

### Comparing `awesomeversion-22.9.0/awesomeversion/comparehandlers/modifier.py` & `awesomeversion-23.5.0/awesomeversion/comparehandlers/modifier.py`

 * *Files identical despite different names*

### Comparing `awesomeversion-22.9.0/awesomeversion/comparehandlers/sections.py` & `awesomeversion-23.5.0/awesomeversion/comparehandlers/sections.py`

 * *Files identical despite different names*

### Comparing `awesomeversion-22.9.0/awesomeversion/strategy.py` & `awesomeversion-23.5.0/awesomeversion/strategy.py`

 * *Files identical despite different names*

### Comparing `awesomeversion-22.9.0/awesomeversion/utils/regex.py` & `awesomeversion-23.5.0/awesomeversion/utils/regex.py`

 * *Files identical despite different names*

### Comparing `awesomeversion-22.9.0/pyproject.toml` & `awesomeversion-23.5.0/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -14,34 +14,34 @@
 include = ["awesomeversion", "awesomeversion.*", "LICENCE.md"]
 keywords = ["calver", "semver", "0ver", "version", "pep440", "buildver"]
 license = "MIT"
 maintainers = ["Ludeeus <ludeeus@ludeeus.dev>"]
 name = "awesomeversion"
 readme = "README.md"
 repository = "https://github.com/ludeeus/awesomeversion"
-version = "22.9.0"
+version = "23.5.0"
 
 [tool.poetry.dependencies]
 python = "^3.7"
 
 [tool.poetry.dev-dependencies]
-black = "^22.8"
-isort = "^5.10.1"
-mypy = "^0.971"
+black = "^23.3"
+isort = "^5.11.5"
+mypy = "^1.3"
 pylint = "^2.13.9"
-pytest = "^7.1.3"
-pytest-cov = "^3.0.0"
+pytest = "^7.3.1"
+pytest-cov = "^4.0.0"
 
 [tool.isort]
 combine_as_imports = true
 force_sort_within_sections = true
 profile = "black"
 
 [tool.pylint.'MESSAGES CONTROL']
-disable = "unsubscriptable-object,duplicate-code"
+disable = "unsubscriptable-object,duplicate-code,too-many-public-methods"
 
 
 [tool.coverage.run]
 source = ["awesomeversion"]
 omit = ["setup.py", "tests/*"]
 
 [tool.coverage.report]
```

