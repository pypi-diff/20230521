# Comparing `tmp/metron_tagger-1.4.3.tar.gz` & `tmp/metron_tagger-1.4.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "metron_tagger-1.4.3.tar", max compression
+gzip compressed data, was "metron_tagger-1.4.4.tar", max compression
```

## Comparing `metron_tagger-1.4.3.tar` & `metron_tagger-1.4.4.tar`

### file list

```diff
@@ -1,24 +1,23 @@
--rw-r--r--   0        0        0    35149 2022-10-24 13:42:58.896643 metron_tagger-1.4.3/LICENSE
--rw-r--r--   0        0        0     2814 2022-10-24 13:42:58.896643 metron_tagger-1.4.3/README.rst
--rw-r--r--   0        0        0       74 2022-10-24 13:42:58.896643 metron_tagger-1.4.3/metrontagger/__init__.py
--rw-r--r--   0        0        0     1328 2022-10-24 13:42:58.900643 metron_tagger-1.4.3/metrontagger/cli.py
--rw-r--r--   0        0        0     7175 2022-10-24 13:42:58.900643 metron_tagger-1.4.3/metrontagger/filerenamer.py
--rw-r--r--   0        0        0     3270 2022-10-24 13:42:58.900643 metron_tagger-1.4.3/metrontagger/filesorter.py
--rw-r--r--   0        0        0     2574 2022-10-24 13:42:58.900643 metron_tagger-1.4.3/metrontagger/options.py
--rwxr-xr-x   0        0        0     8621 2022-10-24 13:42:58.900643 metron_tagger-1.4.3/metrontagger/run.py
--rw-r--r--   0        0        0     4753 2022-10-24 13:42:58.900643 metron_tagger-1.4.3/metrontagger/settings.py
--rw-r--r--   0        0        0      129 2022-10-24 13:42:58.900643 metron_tagger-1.4.3/metrontagger/styles.py
--rw-r--r--   0        0        0     9120 2022-10-24 13:42:58.900643 metron_tagger-1.4.3/metrontagger/talker.py
--rw-r--r--   0        0        0     1492 2022-10-24 13:42:58.900643 metron_tagger-1.4.3/metrontagger/utils.py
--rw-r--r--   0        0        0     2039 2022-10-24 13:42:58.900643 metron_tagger-1.4.3/pyproject.toml
--rw-r--r--   0        0        0        0 2022-10-24 13:42:58.900643 metron_tagger-1.4.3/tests/__init__.py
--rw-r--r--   0        0        0     2029 2022-10-24 13:42:58.900643 metron_tagger-1.4.3/tests/conftest.py
--rw-r--r--   0        0        0     1212 2022-10-24 13:42:58.900643 metron_tagger-1.4.3/tests/test_filerenamer.py
--rw-r--r--   0        0        0     2600 2022-10-24 13:42:58.900643 metron_tagger-1.4.3/tests/test_filesorter.py
--rw-r--r--   0        0        0     6621 2022-10-24 13:42:58.900643 metron_tagger-1.4.3/tests/test_metron_tagger.py
--rw-r--r--   0        0        0     1158 2022-10-24 13:42:58.900643 metron_tagger-1.4.3/tests/test_options.py
--rw-r--r--   0        0        0     1279 2022-10-24 13:42:58.900643 metron_tagger-1.4.3/tests/test_settings.py
--rw-r--r--   0        0        0     9347 2022-10-24 13:42:58.900643 metron_tagger-1.4.3/tests/test_talker.py
--rw-r--r--   0        0        0     2094 2022-10-24 13:42:58.900643 metron_tagger-1.4.3/tests/test_utils.py
--rw-r--r--   0        0        0     3776 1970-01-01 00:00:00.000000 metron_tagger-1.4.3/setup.py
--rw-r--r--   0        0        0     4391 1970-01-01 00:00:00.000000 metron_tagger-1.4.3/PKG-INFO
+-rw-r--r--   0        0        0    35149 2023-05-21 13:46:38.407701 metron_tagger-1.4.4/LICENSE
+-rw-r--r--   0        0        0     2814 2023-05-21 13:46:38.407701 metron_tagger-1.4.4/README.rst
+-rw-r--r--   0        0        0       74 2023-05-21 13:46:38.407701 metron_tagger-1.4.4/metrontagger/__init__.py
+-rw-r--r--   0        0        0     1328 2023-05-21 13:46:38.407701 metron_tagger-1.4.4/metrontagger/cli.py
+-rw-r--r--   0        0        0     7090 2023-05-21 13:46:38.407701 metron_tagger-1.4.4/metrontagger/filerenamer.py
+-rw-r--r--   0        0        0     3270 2023-05-21 13:46:38.407701 metron_tagger-1.4.4/metrontagger/filesorter.py
+-rw-r--r--   0        0        0     2574 2023-05-21 13:46:38.407701 metron_tagger-1.4.4/metrontagger/options.py
+-rwxr-xr-x   0        0        0     8599 2023-05-21 13:46:38.407701 metron_tagger-1.4.4/metrontagger/run.py
+-rw-r--r--   0        0        0     4753 2023-05-21 13:46:38.407701 metron_tagger-1.4.4/metrontagger/settings.py
+-rw-r--r--   0        0        0      129 2023-05-21 13:46:38.407701 metron_tagger-1.4.4/metrontagger/styles.py
+-rw-r--r--   0        0        0     9460 2023-05-21 13:46:38.407701 metron_tagger-1.4.4/metrontagger/talker.py
+-rw-r--r--   0        0        0     1492 2023-05-21 13:46:38.407701 metron_tagger-1.4.4/metrontagger/utils.py
+-rw-r--r--   0        0        0     2039 2023-05-21 13:46:38.407701 metron_tagger-1.4.4/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-05-21 13:46:38.407701 metron_tagger-1.4.4/tests/__init__.py
+-rw-r--r--   0        0        0     2029 2023-05-21 13:46:38.407701 metron_tagger-1.4.4/tests/conftest.py
+-rw-r--r--   0        0        0     1212 2023-05-21 13:46:38.407701 metron_tagger-1.4.4/tests/test_filerenamer.py
+-rw-r--r--   0        0        0     2600 2023-05-21 13:46:38.407701 metron_tagger-1.4.4/tests/test_filesorter.py
+-rw-r--r--   0        0        0     6621 2023-05-21 13:46:38.407701 metron_tagger-1.4.4/tests/test_metron_tagger.py
+-rw-r--r--   0        0        0     1158 2023-05-21 13:46:38.407701 metron_tagger-1.4.4/tests/test_options.py
+-rw-r--r--   0        0        0     1279 2023-05-21 13:46:38.407701 metron_tagger-1.4.4/tests/test_settings.py
+-rw-r--r--   0        0        0     9347 2023-05-21 13:46:38.411701 metron_tagger-1.4.4/tests/test_talker.py
+-rw-r--r--   0        0        0     2094 2023-05-21 13:46:38.411701 metron_tagger-1.4.4/tests/test_utils.py
+-rw-r--r--   0        0        0     4290 1970-01-01 00:00:00.000000 metron_tagger-1.4.4/PKG-INFO
```

### Comparing `metron_tagger-1.4.3/LICENSE` & `metron_tagger-1.4.4/LICENSE`

 * *Files identical despite different names*

### Comparing `metron_tagger-1.4.3/README.rst` & `metron_tagger-1.4.4/README.rst`

 * *Files identical despite different names*

### Comparing `metron_tagger-1.4.3/metrontagger/cli.py` & `metron_tagger-1.4.4/metrontagger/cli.py`

 * *Files identical despite different names*

### Comparing `metron_tagger-1.4.3/metrontagger/filerenamer.py` & `metron_tagger-1.4.4/metrontagger/filerenamer.py`

 * *Files 4% similar despite different names*

```diff
@@ -159,18 +159,15 @@
 
         if self.smart_cleanup:
             new_name = self.smart_cleanup_string(new_name)
 
         ext = filename.suffix
         new_name += ext
 
-        # some tweaks to keep various filesystems happy
-        new_name = cleanup_string(new_name)
-
-        return new_name
+        return cleanup_string(new_name)
 
     def rename_file(self, comic: Path) -> Optional[Path]:
         new_name = self.determine_name(comic)
         if not new_name:
             return None
 
         if new_name == comic.name:
```

### Comparing `metron_tagger-1.4.3/metrontagger/filesorter.py` & `metron_tagger-1.4.4/metrontagger/filesorter.py`

 * *Files identical despite different names*

### Comparing `metron_tagger-1.4.3/metrontagger/options.py` & `metron_tagger-1.4.4/metrontagger/options.py`

 * *Files identical despite different names*

### Comparing `metron_tagger-1.4.3/metrontagger/run.py` & `metron_tagger-1.4.4/metrontagger/run.py`

 * *Files 2% similar despite different names*

```diff
@@ -127,15 +127,15 @@
             "\nShowing files without metadata:\n-------------------------------",
             style=Styles.TITLE,
         )
         for comic in file_list:
             comic_archive = Comic(comic)
             if comic_archive.has_metadata():
                 continue
-            questionary.print(f"no metadata in '{comic.name}'", style=Styles.SUCCESS)
+            questionary.print(f"{comic}", style=Styles.SUCCESS)
 
     @staticmethod
     def _delete_metadata(file_list: List[Path]) -> None:
         questionary.print("\nRemoving metadata:\n-----------------", style=Styles.TITLE)
         for comic in file_list:
             comic_archive = Comic(comic)
             if comic_archive.has_metadata():
```

### Comparing `metron_tagger-1.4.3/metrontagger/settings.py` & `metron_tagger-1.4.4/metrontagger/settings.py`

 * *Files identical despite different names*

### Comparing `metron_tagger-1.4.3/metrontagger/talker.py` & `metron_tagger-1.4.4/metrontagger/talker.py`

 * *Files 6% similar despite different names*

```diff
@@ -3,14 +3,15 @@
 from typing import List, Optional, Tuple
 
 import mokkari
 import questionary
 from darkseid.comic import Comic
 from darkseid.issue_string import IssueString
 from darkseid.metadata import Basic, Credit, Metadata, Role, Series
+from mokkari.exceptions import ApiError
 from mokkari.issue import CreditsSchema, IssueSchema, RolesSchema
 
 from metrontagger import __version__
 from metrontagger.settings import MetronTaggerSettings
 from metrontagger.styles import Styles
 from metrontagger.utils import create_query_params
 
@@ -39,15 +40,15 @@
 
     def add_multiple_match(self, multi_match: MultipleMatch) -> None:
         self.multiple_matches.append(multi_match)
 
 
 class Talker:
     def __init__(self, username: str, password: str) -> None:
-        self.api = mokkari.api(username, password)
+        self.api = mokkari.api(username, password, user_agent=f"Metron-Tagger/{__version__}")
         self.match_results = OnlineMatchResults()
 
     @staticmethod
     def _create_choice_list(match_set: List[IssueSchema]) -> List[questionary.Choice]:
         issue_lst = []
         for i in match_set:
             c = questionary.Choice(title=f"{i.issue_name} ({i.cover_date})", value=i.id)
@@ -123,17 +124,22 @@
             for match_set in self.match_results.multiple_matches:
                 if issue_id := self._select_choice_from_matches(
                     match_set.filename, match_set.matches
                 ):
                     self._write_issue_md(match_set.filename, issue_id)
 
     def _write_issue_md(self, filename: Path, issue_id: int) -> None:
+        # sourcery skip: extract-method, inline-immediately-returned-variable
         success = False
-
-        if resp := self.api.issue(issue_id):
+        resp = None
+        try:
+            resp = self.api.issue(issue_id)
+        except ApiError as e:
+            questionary.print(f"Failed to retrieve data: {repr(e)}", style=Styles.ERROR)
+        if resp is not None:
             ca = Comic(filename)
             meta_data = Metadata()
             meta_data.set_default_page_list(ca.get_number_of_pages())
             md = self._map_resp_to_metadata(resp)
             md.overlay(meta_data)
             success = ca.write_metadata(md)
```

### Comparing `metron_tagger-1.4.3/metrontagger/utils.py` & `metron_tagger-1.4.4/metrontagger/utils.py`

 * *Files identical despite different names*

### Comparing `metron_tagger-1.4.3/pyproject.toml` & `metron_tagger-1.4.4/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "metron-tagger"
-version = "1.4.3"
+version = "1.4.4"
 description = "A program to write metadata from metron.cloud to a comic archive"
 authors = ["Brian Pepple <bdpepple@gmail.com>"]
 license = "GPL-3.0-or-later"
 maintainers = ["Brian Pepple <bdpepple@gmail.com>"]
 readme = "README.rst"
 packages = [
 	{ include = "metrontagger" },
@@ -28,15 +28,15 @@
   "Operating System :: POSIX :: Linux",
   "Operating System :: Microsoft :: Windows",
 ]
 keywords=["comics", "comic", "metadata", "tagging", "tagger"]
 
 [tool.poetry.dependencies]
 python = "^3.9"
-mokkari = "^2.3.3"
+mokkari = "^2.5.0"
 questionary = "^1.10.0"
 pyxdg = "^0.28"
 darkseid = "^2.0.1"
 
 [tool.poetry.dev-dependencies]
 pytest-cov = "^2.12.1"
 flake8 = "^3.9.2"
```

### Comparing `metron_tagger-1.4.3/tests/conftest.py` & `metron_tagger-1.4.4/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `metron_tagger-1.4.3/tests/test_filerenamer.py` & `metron_tagger-1.4.4/tests/test_filerenamer.py`

 * *Files identical despite different names*

### Comparing `metron_tagger-1.4.3/tests/test_filesorter.py` & `metron_tagger-1.4.4/tests/test_filesorter.py`

 * *Files identical despite different names*

### Comparing `metron_tagger-1.4.3/tests/test_metron_tagger.py` & `metron_tagger-1.4.4/tests/test_metron_tagger.py`

 * *Files identical despite different names*

### Comparing `metron_tagger-1.4.3/tests/test_options.py` & `metron_tagger-1.4.4/tests/test_options.py`

 * *Files identical despite different names*

### Comparing `metron_tagger-1.4.3/tests/test_settings.py` & `metron_tagger-1.4.4/tests/test_settings.py`

 * *Files identical despite different names*

### Comparing `metron_tagger-1.4.3/tests/test_talker.py` & `metron_tagger-1.4.4/tests/test_talker.py`

 * *Files identical despite different names*

### Comparing `metron_tagger-1.4.3/tests/test_utils.py` & `metron_tagger-1.4.4/tests/test_utils.py`

 * *Files identical despite different names*

### Comparing `metron_tagger-1.4.3/PKG-INFO` & `metron_tagger-1.4.4/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: metron-tagger
-Version: 1.4.3
+Version: 1.4.4
 Summary: A program to write metadata from metron.cloud to a comic archive
 License: GPL-3.0-or-later
 Keywords: comics,comic,metadata,tagging,tagger
 Author: Brian Pepple
 Author-email: bdpepple@gmail.com
 Maintainer: Brian Pepple
 Maintainer-email: bdpepple@gmail.com
@@ -19,20 +19,18 @@
 Classifier: Operating System :: POSIX
 Classifier: Operating System :: POSIX :: BSD
 Classifier: Operating System :: POSIX :: Linux
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
-Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.9
 Classifier: Topic :: Other/Nonlisted Topic
 Classifier: Topic :: Utilities
 Requires-Dist: darkseid (>=2.0.1,<3.0.0)
-Requires-Dist: mokkari (>=2.3.3,<3.0.0)
+Requires-Dist: mokkari (>=2.5.0,<3.0.0)
 Requires-Dist: pyxdg (>=0.28,<0.29)
 Requires-Dist: questionary (>=1.10.0,<2.0.0)
 Project-URL: Bug Tracker, https://github.com/Metron-Project/metron-tagger/issues
 Project-URL: Homepage, https://github.com/Metron-Project/metron-tagger
 Description-Content-Type: text/x-rst
 
 =============
```

