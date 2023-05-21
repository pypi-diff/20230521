# Comparing `tmp/aio.api.github-0.2.0.tar.gz` & `tmp/aio.api.github-0.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aio.api.github-0.2.0.tar", last modified: Fri Feb  3 14:57:01 2023, max compression
+gzip compressed data, was "aio.api.github-0.2.2.tar", last modified: Sun May 21 17:27:43 2023, max compression
```

## Comparing `aio.api.github-0.2.0.tar` & `aio.api.github-0.2.2.tar`

### file list

```diff
@@ -1,36 +1,37 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-03 14:57:01.822353 aio.api.github-0.2.0/
--rw-r--r--   0 runner    (1001) docker     (123)       12 2023-02-03 14:57:01.000000 aio.api.github-0.2.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)      395 2023-02-03 14:57:01.822353 aio.api.github-0.2.0/PKG-INFO
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-03 14:57:01.818353 aio.api.github-0.2.0/aio/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-03 14:57:01.818353 aio.api.github-0.2.0/aio/api/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-03 14:57:01.822353 aio.api.github-0.2.0/aio/api/github/
--rw-r--r--   0 runner    (1001) docker     (123)     1601 2023-02-03 14:57:01.000000 aio.api.github-0.2.0/aio/api/github/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-03 14:57:01.822353 aio.api.github-0.2.0/aio/api/github/abstract/
--rw-r--r--   0 runner    (1001) docker     (123)      642 2023-02-03 14:57:01.000000 aio.api.github-0.2.0/aio/api/github/abstract/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3473 2023-02-03 14:57:01.000000 aio.api.github-0.2.0/aio/api/github/abstract/api.py
--rw-r--r--   0 runner    (1001) docker     (123)     1258 2023-02-03 14:57:01.000000 aio.api.github-0.2.0/aio/api/github/abstract/base.py
--rw-r--r--   0 runner    (1001) docker     (123)      608 2023-02-03 14:57:01.000000 aio.api.github-0.2.0/aio/api/github/abstract/commit.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-03 14:57:01.822353 aio.api.github-0.2.0/aio/api/github/abstract/issues/
--rw-r--r--   0 runner    (1001) docker     (123)      298 2023-02-03 14:57:01.000000 aio.api.github-0.2.0/aio/api/github/abstract/issues/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3908 2023-02-03 14:57:01.000000 aio.api.github-0.2.0/aio/api/github/abstract/issues/issues.py
--rw-r--r--   0 runner    (1001) docker     (123)     7235 2023-02-03 14:57:01.000000 aio.api.github-0.2.0/aio/api/github/abstract/issues/tracker.py
--rw-r--r--   0 runner    (1001) docker     (123)     3148 2023-02-03 14:57:01.000000 aio.api.github-0.2.0/aio/api/github/abstract/iterator.py
--rw-r--r--   0 runner    (1001) docker     (123)      319 2023-02-03 14:57:01.000000 aio.api.github-0.2.0/aio/api/github/abstract/label.py
--rw-r--r--   0 runner    (1001) docker     (123)      942 2023-02-03 14:57:01.000000 aio.api.github-0.2.0/aio/api/github/abstract/release.py
--rw-r--r--   0 runner    (1001) docker     (123)     5706 2023-02-03 14:57:01.000000 aio.api.github-0.2.0/aio/api/github/abstract/repo.py
--rw-r--r--   0 runner    (1001) docker     (123)      543 2023-02-03 14:57:01.000000 aio.api.github-0.2.0/aio/api/github/abstract/tag.py
--rw-r--r--   0 runner    (1001) docker     (123)     1825 2023-02-03 14:57:01.000000 aio.api.github-0.2.0/aio/api/github/api.py
--rw-r--r--   0 runner    (1001) docker     (123)      210 2023-02-03 14:57:01.000000 aio.api.github-0.2.0/aio/api/github/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)    14153 2023-02-03 14:57:01.000000 aio.api.github-0.2.0/aio/api/github/interface.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-03 14:57:01.000000 aio.api.github-0.2.0/aio/api/github/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)      322 2023-02-03 14:57:01.000000 aio.api.github-0.2.0/aio/api/github/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-03 14:57:01.818353 aio.api.github-0.2.0/aio.api.github.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      395 2023-02-03 14:57:01.000000 aio.api.github-0.2.0/aio.api.github.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      852 2023-02-03 14:57:01.000000 aio.api.github-0.2.0/aio.api.github.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-02-03 14:57:01.000000 aio.api.github-0.2.0/aio.api.github.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-02-03 14:57:01.000000 aio.api.github-0.2.0/aio.api.github.egg-info/namespace_packages.txt
--rw-r--r--   0 runner    (1001) docker     (123)       75 2023-02-03 14:57:01.000000 aio.api.github-0.2.0/aio.api.github.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        4 2023-02-03 14:57:01.000000 aio.api.github-0.2.0/aio.api.github.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      625 2023-02-03 14:57:01.000000 aio.api.github-0.2.0/backend_shim.py
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-02-03 14:57:01.822353 aio.api.github-0.2.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1038 2023-02-03 14:57:01.000000 aio.api.github-0.2.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 17:27:43.696289 aio.api.github-0.2.2/
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-05-21 17:27:43.000000 aio.api.github-0.2.2/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)      394 2023-05-21 17:27:43.696289 aio.api.github-0.2.2/PKG-INFO
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 17:27:43.692289 aio.api.github-0.2.2/aio/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 17:27:43.692289 aio.api.github-0.2.2/aio/api/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 17:27:43.696289 aio.api.github-0.2.2/aio/api/github/
+-rw-r--r--   0 runner    (1001) docker     (123)     1761 2023-05-21 17:27:43.000000 aio.api.github-0.2.2/aio/api/github/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 17:27:43.696289 aio.api.github-0.2.2/aio/api/github/abstract/
+-rw-r--r--   0 runner    (1001) docker     (123)      692 2023-05-21 17:27:43.000000 aio.api.github-0.2.2/aio/api/github/abstract/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3473 2023-05-21 17:27:43.000000 aio.api.github-0.2.2/aio/api/github/abstract/api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1345 2023-05-21 17:27:43.000000 aio.api.github-0.2.2/aio/api/github/abstract/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)      608 2023-05-21 17:27:43.000000 aio.api.github-0.2.2/aio/api/github/abstract/commit.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 17:27:43.696289 aio.api.github-0.2.2/aio/api/github/abstract/issues/
+-rw-r--r--   0 runner    (1001) docker     (123)      298 2023-05-21 17:27:43.000000 aio.api.github-0.2.2/aio/api/github/abstract/issues/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3908 2023-05-21 17:27:43.000000 aio.api.github-0.2.2/aio/api/github/abstract/issues/issues.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7235 2023-05-21 17:27:43.000000 aio.api.github-0.2.2/aio/api/github/abstract/issues/tracker.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3148 2023-05-21 17:27:43.000000 aio.api.github-0.2.2/aio/api/github/abstract/iterator.py
+-rw-r--r--   0 runner    (1001) docker     (123)      319 2023-05-21 17:27:43.000000 aio.api.github-0.2.2/aio/api/github/abstract/label.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4242 2023-05-21 17:27:43.000000 aio.api.github-0.2.2/aio/api/github/abstract/release.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6237 2023-05-21 17:27:43.000000 aio.api.github-0.2.2/aio/api/github/abstract/repo.py
+-rw-r--r--   0 runner    (1001) docker     (123)      543 2023-05-21 17:27:43.000000 aio.api.github-0.2.2/aio/api/github/abstract/tag.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2069 2023-05-21 17:27:43.000000 aio.api.github-0.2.2/aio/api/github/api.py
+-rw-r--r--   0 runner    (1001) docker     (123)      210 2023-05-21 17:27:43.000000 aio.api.github-0.2.2/aio/api/github/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14600 2023-05-21 17:27:43.000000 aio.api.github-0.2.2/aio/api/github/interface.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-21 17:27:43.000000 aio.api.github-0.2.2/aio/api/github/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)      147 2023-05-21 17:27:43.000000 aio.api.github-0.2.2/aio/api/github/typing.py
+-rw-r--r--   0 runner    (1001) docker     (123)      322 2023-05-21 17:27:43.000000 aio.api.github-0.2.2/aio/api/github/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 17:27:43.696289 aio.api.github-0.2.2/aio.api.github.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      394 2023-05-21 17:27:43.000000 aio.api.github-0.2.2/aio.api.github.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      877 2023-05-21 17:27:43.000000 aio.api.github-0.2.2/aio.api.github.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-21 17:27:43.000000 aio.api.github-0.2.2/aio.api.github.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-21 17:27:43.000000 aio.api.github-0.2.2/aio.api.github.egg-info/namespace_packages.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       76 2023-05-21 17:27:43.000000 aio.api.github-0.2.2/aio.api.github.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        4 2023-05-21 17:27:43.000000 aio.api.github-0.2.2/aio.api.github.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      625 2023-05-21 17:27:43.000000 aio.api.github-0.2.2/backend_shim.py
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-21 17:27:43.696289 aio.api.github-0.2.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1038 2023-05-21 17:27:43.000000 aio.api.github-0.2.2/setup.py
```

### Comparing `aio.api.github-0.2.0/aio/api/github/__init__.py` & `aio.api.github-0.2.2/aio/api/github/__init__.py`

 * *Files 6% similar despite different names*

```diff
@@ -8,38 +8,41 @@
     GithubAPI,
     GithubCommit,
     GithubIssue,
     GithubIssues,
     GithubIterator,
     GithubLabel,
     GithubRelease,
+    GithubReleaseAssets,
     GithubRepo,
     GithubTag)
 from .abstract import (
     AGithubAPI,
     AGithubCommit,
     AGithubIssue,
     AGithubIssues,
     AGithubIssuesTracker,
     AGithubIterator,
     AGithubLabel,
     AGithubRelease,
+    AGithubReleaseAssets,
     AGithubRepo,
     AGithubTag,
     AGithubTrackedIssue,
     AGithubTrackedIssues)
 from .interface import (
     IGithubAPI,
     IGithubCommit,
     IGithubIssue,
     IGithubIssues,
     IGithubIssuesTracker,
     IGithubIterator,
     IGithubLabel,
     IGithubRelease,
+    IGithubReleaseAssets,
     IGithubRepo,
     IGithubTag,
     IGithubTrackedIssue,
     IGithubTrackedIssues)
 
 
 __all__ = (
@@ -48,35 +51,38 @@
     "AGithubCommit",
     "AGithubIssue",
     "AGithubIssuesTracker",
     "AGithubIssues",
     "AGithubIterator",
     "AGithubLabel",
     "AGithubRelease",
+    "AGithubReleaseAssets",
     "AGithubRepo",
     "AGithubTag",
     "AGithubTrackedIssue",
     "AGithubTrackedIssues",
     "exceptions",
     "GithubAPI",
     "GithubCommit",
     "GithubLabel",
     "GithubIssue",
     "GithubIssues",
     "GithubIterator",
     "GithubRelease",
+    "GithubReleaseAssets",
     "GithubRepo",
     "GithubTag",
     "IGithubAPI",
     "IGithubCommit",
     "IGithubIssue",
     "IGithubIssues",
     "IGithubIssuesTracker",
     "IGithubIterator",
     "IGithubLabel",
     "IGithubRelease",
+    "IGithubReleaseAssets",
     "IGithubRepo",
     "IGithubTag",
     "IGithubTrackedIssue",
     "IGithubTrackedIssues",
     "interface",
     "utils")
```

### Comparing `aio.api.github-0.2.0/aio/api/github/abstract/__init__.py` & `aio.api.github-0.2.2/aio/api/github/abstract/__init__.py`

 * *Files 14% similar despite different names*

```diff
@@ -5,25 +5,26 @@
     AGithubIssue,
     AGithubIssues,
     AGithubIssuesTracker,
     AGithubTrackedIssue,
     AGithubTrackedIssues)
 from .iterator import AGithubIterator
 from .label import AGithubLabel
-from .release import AGithubRelease
+from .release import AGithubRelease, AGithubReleaseAssets
 from .repo import AGithubRepo
 from .tag import AGithubTag
 
 
 __all__ = (
     "AGithubAPI",
     "AGithubCommit",
     "AGithubIssue",
     "AGithubIssues",
     "AGithubIssuesTracker",
     "AGithubIterator",
     "AGithubLabel",
     "AGithubRelease",
+    "AGithubReleaseAssets",
     "AGithubRepo",
     "AGithubTag",
     "AGithubTrackedIssue",
     "AGithubTrackedIssues")
```

### Comparing `aio.api.github-0.2.0/aio/api/github/abstract/api.py` & `aio.api.github-0.2.2/aio/api/github/abstract/api.py`

 * *Files identical despite different names*

### Comparing `aio.api.github-0.2.0/aio/api/github/abstract/base.py` & `aio.api.github-0.2.2/aio/api/github/abstract/base.py`

 * *Files 7% similar despite different names*

```diff
@@ -7,16 +7,16 @@
 UNSET = object()
 
 
 class GithubEntity:
     """Base Github entity class."""
 
     def __init__(self, github: interface.IGithubAPI, data: Dict) -> None:
-        self._github = github
         self.data = data
+        self._github = github
 
     @property
     def github(self) -> "interface.IGithubAPI":
         """Github API."""
         return self._github
 
     @property
@@ -35,14 +35,18 @@
         return self.__data__.get(k, lambda x: x)(v)
 
 
 class GithubRepoEntity(GithubEntity):
     """Base Github repo entity class."""
 
     def __init__(self, repo: interface.IGithubRepo, data: Dict) -> None:
-        self.repo = repo
         self.data = data
+        self._repo = repo
 
     @property
     def github(self) -> interface.IGithubAPI:
         """Github API."""
         return self.repo.github
+
+    @property
+    def repo(self) -> interface.IGithubRepo:
+        return self._repo
```

### Comparing `aio.api.github-0.2.0/aio/api/github/abstract/commit.py` & `aio.api.github-0.2.2/aio/api/github/abstract/commit.py`

 * *Files identical despite different names*

### Comparing `aio.api.github-0.2.0/aio/api/github/abstract/issues/issues.py` & `aio.api.github-0.2.2/aio/api/github/abstract/issues/issues.py`

 * *Files identical despite different names*

### Comparing `aio.api.github-0.2.0/aio/api/github/abstract/issues/tracker.py` & `aio.api.github-0.2.2/aio/api/github/abstract/issues/tracker.py`

 * *Files identical despite different names*

### Comparing `aio.api.github-0.2.0/aio/api/github/abstract/iterator.py` & `aio.api.github-0.2.2/aio/api/github/abstract/iterator.py`

 * *Files identical despite different names*

### Comparing `aio.api.github-0.2.0/aio/api/github/abstract/repo.py` & `aio.api.github-0.2.2/aio/api/github/abstract/repo.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,21 +1,25 @@
 
+import logging
 import pathlib
 from datetime import datetime
 from functools import cached_property, partial
 from typing import Any, Dict, Optional, Type
 
 import gidgethub
 
 import abstracts
 
 from aio.api.github import exceptions, interface, utils
 from . import base
 
 
+logger = logging.getLogger(__name__)
+
+
 class AGithubRepo(metaclass=abstracts.Abstraction):
     """A Github repo."""
 
     def __init__(self, github: "interface.IGithubAPI", name: str) -> None:
         self._github = github
         self._name = name
 
@@ -59,44 +63,51 @@
             query,
             inflate=partial(self.github.commit_class, self))
 
     async def create_release(
             self,
             commitish: str,
             tag_name: str,
+            dry_run: bool = False,
             body: Optional[str] = None,
             latest: Optional[bool] = False,
             generate_release_notes: Optional[bool] = False) -> (
-                Dict[str, str | Dict]):
-        if await self.tag_exists(tag_name):
+                "interface.IGithubRelease"):
+        if await self.tag_exists(tag_name) and not dry_run:
             raise exceptions.TagExistsError(
                 f"Cannot create tag, already exists: {tag_name}")
         url_vars: Dict[str, bool | str] = dict(
             tag_name=tag_name,
             name=tag_name,
             target_commitish=commitish,
             make_latest=("true" if latest else "false"))
         if body is not None:
             url_vars["body"] = body
         if generate_release_notes is not None:
             url_vars["generate_release_notes"] = generate_release_notes
-        return await self.post("releases", url_vars)
+        logger.debug(
+            f"Create {'DRY RUN ' if dry_run else ''}release "
+            f"({tag_name}):\n  {url_vars}")
+        return await self.release(tag_name, url_vars, dry_run=dry_run)
 
     async def getitem(self, query: str) -> Any:
         """Call the `gidgethub.getitem` api for this repo."""
         return await self.github.getitem(self.github_endpoint(query))
 
     def getiter(self, query: str, **kwargs) -> "interface.IGithubIterator":
         """Return a `GithubIterator` wrapping `gidgethub.getiter` for this
         repo."""
         return self.github.getiter(self.github_endpoint(query), **kwargs)
 
     def github_endpoint(self, rel_path: str) -> str:
         """Github API path for provided relative path."""
-        return str(self.github_path.joinpath(rel_path))
+        return (
+            rel_path
+            if rel_path.startswith("https://")
+            else str(self.github_path.joinpath(rel_path)))
 
     async def highest_release(
             self,
             since: Optional[datetime] = None) -> Optional[
                 "interface.IGithubRelease"]:
         highest_release = None
 
@@ -131,15 +142,21 @@
             query: str,
             data: Optional[Dict] = None, **kwargs) -> Any:
         return await self.github.post(
             self.github_endpoint(query),
             data=data,
             **kwargs)
 
-    async def release(self, name: str) -> "interface.IGithubRelease":
+    async def release(
+            self,
+            name: str,
+            data: dict = None,
+            dry_run: bool = False) -> "interface.IGithubRelease":
+        if data:
+            return await self.github.release_class.create(self, data, dry_run)
         return self.github.release_class(
             self,
             await self.getitem(f"releases/tags/{name}"))
 
     def releases(self) -> "interface.IGithubIterator":
         """Iterate releases for this repo."""
         # TODO: make per_page configurable
```

### Comparing `aio.api.github-0.2.0/aio/api/github/abstract/tag.py` & `aio.api.github-0.2.2/aio/api/github/abstract/tag.py`

 * *Files identical despite different names*

### Comparing `aio.api.github-0.2.0/aio/api/github/api.py` & `aio.api.github-0.2.2/aio/api/github/api.py`

 * *Files 11% similar despite different names*

```diff
@@ -9,16 +9,18 @@
     AGithubAPI,
     AGithubCommit,
     AGithubIssue,
     AGithubIssues,
     AGithubIterator,
     AGithubLabel,
     AGithubRelease,
+    AGithubReleaseAssets,
     AGithubRepo,
     AGithubTag)
+from . import interface
 
 
 @abstracts.implementer(AGithubCommit)
 class GithubCommit:
     pass
 
 
@@ -40,14 +42,22 @@
 @abstracts.implementer(AGithubLabel)
 class GithubLabel:
     pass
 
 
 @abstracts.implementer(AGithubRelease)
 class GithubRelease:
+
+    @property
+    def assets_class(self) -> Type["interface.IGithubReleaseAssets"]:
+        return GithubReleaseAssets
+
+
+@abstracts.implementer(AGithubReleaseAssets)
+class GithubReleaseAssets:
     pass
 
 
 @abstracts.implementer(AGithubRepo)
 class GithubRepo:
     pass
```

### Comparing `aio.api.github-0.2.0/aio/api/github/interface.py` & `aio.api.github-0.2.2/aio/api/github/interface.py`

 * *Files 1% similar despite different names*

```diff
@@ -19,23 +19,40 @@
     pass
 
 
 class IGithubRelease(metaclass=abstracts.Interface):
 
     @property  # type:ignore
     @abstracts.interfacemethod
+    def repo(self) -> str:
+        raise NotImplementedError
+
+    @property  # type:ignore
+    @abstracts.interfacemethod
     def tag_name(self) -> str:
         raise NotImplementedError
 
     @property  # type:ignore
     @abstracts.interfacemethod
+    def upload_url(self) -> str:
+        raise NotImplementedError
+
+    @property  # type:ignore
+    @abstracts.interfacemethod
     def version(self) -> Optional[version.Version]:
         raise NotImplementedError
 
 
+class IGithubReleaseAssets(metaclass=abstracts.Interface):
+
+    @abstracts.interfacemethod
+    def __init__(self, release: "IGithubRelease", name: str) -> None:
+        raise NotImplementedError
+
+
 class IGithubTag(metaclass=abstracts.Interface):
     pass
 
 
 class IGithubIterator(metaclass=abstracts.Interface):
 
     @abstracts.interfacemethod
```

### Comparing `aio.api.github-0.2.0/aio.api.github.egg-info/SOURCES.txt` & `aio.api.github-0.2.2/aio.api.github.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -8,14 +8,15 @@
 aio.api.github.egg-info/requires.txt
 aio.api.github.egg-info/top_level.txt
 aio/api/github/__init__.py
 aio/api/github/api.py
 aio/api/github/exceptions.py
 aio/api/github/interface.py
 aio/api/github/py.typed
+aio/api/github/typing.py
 aio/api/github/utils.py
 aio/api/github/abstract/__init__.py
 aio/api/github/abstract/api.py
 aio/api/github/abstract/base.py
 aio/api/github/abstract/commit.py
 aio/api/github/abstract/iterator.py
 aio/api/github/abstract/label.py
```

### Comparing `aio.api.github-0.2.0/backend_shim.py` & `aio.api.github-0.2.2/backend_shim.py`

 * *Files identical despite different names*

