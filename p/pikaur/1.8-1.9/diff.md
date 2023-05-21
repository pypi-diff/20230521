# Comparing `tmp/pikaur-1.8.tar.gz` & `tmp/pikaur-1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pikaur-1.8.tar", last modified: Wed Sep  8 22:15:29 2021, max compression
+gzip compressed data, was "pikaur-1.9.tar", last modified: Tue Dec 14 18:24:16 2021, max compression
```

## Comparing `pikaur-1.8.tar` & `pikaur-1.9.tar`

### file list

```diff
@@ -1,48 +1,48 @@
-drwxr-xr-x   0 lie       (1000) lie       (1000)        0 2021-09-08 22:15:29.435965 pikaur-1.8/
--rw-r--r--   0 lie       (1000) lie       (1000)    35147 2018-04-26 23:34:19.000000 pikaur-1.8/LICENSE
--rw-r--r--   0 lie       (1000) lie       (1000)    13770 2021-09-08 22:15:29.435965 pikaur-1.8/PKG-INFO
--rw-r--r--   0 lie       (1000) lie       (1000)    12667 2021-08-25 20:02:25.000000 pikaur-1.8/README.md
-drwxr-xr-x   0 lie       (1000) lie       (1000)        0 2021-09-08 22:15:29.435965 pikaur-1.8/pikaur/
--rw-r--r--   0 lie       (1000) lie       (1000)      661 2018-07-05 16:16:12.000000 pikaur-1.8/pikaur/__init__.py
--rw-r--r--   0 lie       (1000) lie       (1000)       63 2019-12-03 22:50:30.000000 pikaur-1.8/pikaur/__main__.py
--rw-r--r--   0 lie       (1000) lie       (1000)    12324 2019-07-26 03:48:53.000000 pikaur-1.8/pikaur/argparse.py
--rw-r--r--   0 lie       (1000) lie       (1000)    12728 2021-07-28 15:28:22.000000 pikaur-1.8/pikaur/args.py
--rw-r--r--   0 lie       (1000) lie       (1000)     6616 2020-09-24 16:58:18.000000 pikaur-1.8/pikaur/aur.py
--rw-r--r--   0 lie       (1000) lie       (1000)    13393 2021-06-24 21:06:36.000000 pikaur-1.8/pikaur/aur_deps.py
--rw-r--r--   0 lie       (1000) lie       (1000)    29292 2021-06-05 13:58:34.000000 pikaur-1.8/pikaur/build.py
--rw-r--r--   0 lie       (1000) lie       (1000)    11933 2021-09-08 22:12:56.000000 pikaur-1.8/pikaur/config.py
--rw-r--r--   0 lie       (1000) lie       (1000)     6343 2019-07-26 03:48:53.000000 pikaur-1.8/pikaur/conflicts.py
--rw-r--r--   0 lie       (1000) lie       (1000)    11319 2021-08-25 20:04:13.000000 pikaur-1.8/pikaur/core.py
--rw-r--r--   0 lie       (1000) lie       (1000)     2033 2020-03-24 19:00:04.000000 pikaur-1.8/pikaur/exceptions.py
--rw-r--r--   0 lie       (1000) lie       (1000)     1285 2021-08-25 19:58:48.000000 pikaur-1.8/pikaur/filelock.py
--rw-r--r--   0 lie       (1000) lie       (1000)     1800 2021-05-10 18:22:13.000000 pikaur-1.8/pikaur/getpkgbuild_cli.py
--rw-r--r--   0 lie       (1000) lie       (1000)     3793 2020-03-24 18:57:17.000000 pikaur-1.8/pikaur/help_cli.py
--rw-r--r--   0 lie       (1000) lie       (1000)      330 2018-07-05 16:26:09.000000 pikaur-1.8/pikaur/i18n.py
--rw-r--r--   0 lie       (1000) lie       (1000)     3246 2021-06-12 11:19:00.000000 pikaur-1.8/pikaur/info_cli.py
--rw-r--r--   0 lie       (1000) lie       (1000)    43211 2021-06-23 13:54:11.000000 pikaur-1.8/pikaur/install_cli.py
--rw-r--r--   0 lie       (1000) lie       (1000)    24793 2021-06-05 13:50:12.000000 pikaur-1.8/pikaur/install_info_fetcher.py
--rw-r--r--   0 lie       (1000) lie       (1000)    11406 2021-08-25 20:02:04.000000 pikaur-1.8/pikaur/main.py
--rw-r--r--   0 lie       (1000) lie       (1000)     4552 2020-07-02 04:34:15.000000 pikaur-1.8/pikaur/makepkg_config.py
--rw-r--r--   0 lie       (1000) lie       (1000)     5716 2021-08-25 19:55:37.000000 pikaur-1.8/pikaur/news.py
--rw-r--r--   0 lie       (1000) lie       (1000)    22623 2021-07-27 22:37:23.000000 pikaur-1.8/pikaur/pacman.py
--rw-r--r--   0 lie       (1000) lie       (1000)      153 2020-03-24 19:07:08.000000 pikaur-1.8/pikaur/pacman_i18n.py
--rw-r--r--   0 lie       (1000) lie       (1000)    13597 2021-09-04 16:12:53.000000 pikaur-1.8/pikaur/pikspect.py
--rw-r--r--   0 lie       (1000) lie       (1000)     3801 2021-08-24 20:40:33.000000 pikaur-1.8/pikaur/pprint.py
--rw-r--r--   0 lie       (1000) lie       (1000)    23508 2020-11-29 00:20:14.000000 pikaur-1.8/pikaur/print_department.py
--rw-r--r--   0 lie       (1000) lie       (1000)     1897 2021-07-27 22:04:00.000000 pikaur-1.8/pikaur/progressbar.py
--rw-r--r--   0 lie       (1000) lie       (1000)     7158 2021-08-25 22:44:28.000000 pikaur-1.8/pikaur/prompt.py
--rw-r--r--   0 lie       (1000) lie       (1000)     2159 2018-07-25 03:24:33.000000 pikaur-1.8/pikaur/replacements.py
--rw-r--r--   0 lie       (1000) lie       (1000)     6309 2021-06-12 10:08:24.000000 pikaur-1.8/pikaur/search_cli.py
--rw-r--r--   0 lie       (1000) lie       (1000)     5055 2020-01-20 21:45:29.000000 pikaur-1.8/pikaur/srcinfo.py
--rw-r--r--   0 lie       (1000) lie       (1000)     4751 2020-01-20 21:45:29.000000 pikaur-1.8/pikaur/updates.py
--rw-r--r--   0 lie       (1000) lie       (1000)     3713 2021-08-25 20:07:15.000000 pikaur-1.8/pikaur/urllib.py
--rw-r--r--   0 lie       (1000) lie       (1000)     6446 2021-06-30 12:32:22.000000 pikaur-1.8/pikaur/version.py
-drwxr-xr-x   0 lie       (1000) lie       (1000)        0 2021-09-08 22:15:29.435965 pikaur-1.8/pikaur.egg-info/
--rw-r--r--   0 lie       (1000) lie       (1000)    13770 2021-09-08 22:15:29.000000 pikaur-1.8/pikaur.egg-info/PKG-INFO
--rw-r--r--   0 lie       (1000) lie       (1000)      864 2021-09-08 22:15:29.000000 pikaur-1.8/pikaur.egg-info/SOURCES.txt
--rw-r--r--   0 lie       (1000) lie       (1000)        1 2021-09-08 22:15:29.000000 pikaur-1.8/pikaur.egg-info/dependency_links.txt
--rw-r--r--   0 lie       (1000) lie       (1000)       45 2021-09-08 22:15:29.000000 pikaur-1.8/pikaur.egg-info/entry_points.txt
--rw-r--r--   0 lie       (1000) lie       (1000)        7 2021-09-08 22:15:29.000000 pikaur-1.8/pikaur.egg-info/requires.txt
--rw-r--r--   0 lie       (1000) lie       (1000)        7 2021-09-08 22:15:29.000000 pikaur-1.8/pikaur.egg-info/top_level.txt
--rw-r--r--   0 lie       (1000) lie       (1000)       38 2021-09-08 22:15:29.435965 pikaur-1.8/setup.cfg
--rw-r--r--   0 lie       (1000) lie       (1000)     2009 2021-09-08 22:12:56.000000 pikaur-1.8/setup.py
+drwxr-xr-x   0 lie       (1000) lie       (1000)        0 2021-12-14 18:24:16.698794 pikaur-1.9/
+-rw-r--r--   0 lie       (1000) lie       (1000)    35147 2018-04-26 23:34:19.000000 pikaur-1.9/LICENSE
+-rw-r--r--   0 lie       (1000) lie       (1000)    13770 2021-12-14 18:24:16.698794 pikaur-1.9/PKG-INFO
+-rw-r--r--   0 lie       (1000) lie       (1000)    12667 2021-12-01 23:52:41.000000 pikaur-1.9/README.md
+drwxr-xr-x   0 lie       (1000) lie       (1000)        0 2021-12-14 18:24:16.698794 pikaur-1.9/pikaur/
+-rw-r--r--   0 lie       (1000) lie       (1000)      661 2018-07-05 16:16:12.000000 pikaur-1.9/pikaur/__init__.py
+-rw-r--r--   0 lie       (1000) lie       (1000)       63 2019-12-03 22:50:30.000000 pikaur-1.9/pikaur/__main__.py
+-rw-r--r--   0 lie       (1000) lie       (1000)    12324 2019-07-26 03:48:53.000000 pikaur-1.9/pikaur/argparse.py
+-rw-r--r--   0 lie       (1000) lie       (1000)    12654 2021-11-20 18:38:16.000000 pikaur-1.9/pikaur/args.py
+-rw-r--r--   0 lie       (1000) lie       (1000)     6815 2021-09-22 16:55:28.000000 pikaur-1.9/pikaur/aur.py
+-rw-r--r--   0 lie       (1000) lie       (1000)    13393 2021-06-24 21:06:36.000000 pikaur-1.9/pikaur/aur_deps.py
+-rw-r--r--   0 lie       (1000) lie       (1000)    29850 2021-12-01 23:48:08.000000 pikaur-1.9/pikaur/build.py
+-rw-r--r--   0 lie       (1000) lie       (1000)    11933 2021-12-14 18:13:47.000000 pikaur-1.9/pikaur/config.py
+-rw-r--r--   0 lie       (1000) lie       (1000)     6343 2019-07-26 03:48:53.000000 pikaur-1.9/pikaur/conflicts.py
+-rw-r--r--   0 lie       (1000) lie       (1000)    11402 2021-12-02 07:02:22.000000 pikaur-1.9/pikaur/core.py
+-rw-r--r--   0 lie       (1000) lie       (1000)     2033 2020-03-24 19:00:04.000000 pikaur-1.9/pikaur/exceptions.py
+-rw-r--r--   0 lie       (1000) lie       (1000)     1285 2021-08-25 19:58:48.000000 pikaur-1.9/pikaur/filelock.py
+-rw-r--r--   0 lie       (1000) lie       (1000)     1800 2021-05-10 18:22:13.000000 pikaur-1.9/pikaur/getpkgbuild_cli.py
+-rw-r--r--   0 lie       (1000) lie       (1000)     3836 2021-09-22 17:04:52.000000 pikaur-1.9/pikaur/help_cli.py
+-rw-r--r--   0 lie       (1000) lie       (1000)      330 2018-07-05 16:26:09.000000 pikaur-1.9/pikaur/i18n.py
+-rw-r--r--   0 lie       (1000) lie       (1000)     3210 2021-09-22 17:04:06.000000 pikaur-1.9/pikaur/info_cli.py
+-rw-r--r--   0 lie       (1000) lie       (1000)    43629 2021-12-02 07:08:07.000000 pikaur-1.9/pikaur/install_cli.py
+-rw-r--r--   0 lie       (1000) lie       (1000)    25025 2021-12-02 07:07:37.000000 pikaur-1.9/pikaur/install_info_fetcher.py
+-rw-r--r--   0 lie       (1000) lie       (1000)    11477 2021-09-22 17:03:04.000000 pikaur-1.9/pikaur/main.py
+-rw-r--r--   0 lie       (1000) lie       (1000)     4552 2020-07-02 04:34:15.000000 pikaur-1.9/pikaur/makepkg_config.py
+-rw-r--r--   0 lie       (1000) lie       (1000)     5716 2021-08-25 19:55:37.000000 pikaur-1.9/pikaur/news.py
+-rw-r--r--   0 lie       (1000) lie       (1000)    22666 2021-10-23 17:27:56.000000 pikaur-1.9/pikaur/pacman.py
+-rw-r--r--   0 lie       (1000) lie       (1000)      153 2020-03-24 19:07:08.000000 pikaur-1.9/pikaur/pacman_i18n.py
+-rw-r--r--   0 lie       (1000) lie       (1000)    13587 2021-09-22 16:58:47.000000 pikaur-1.9/pikaur/pikspect.py
+-rw-r--r--   0 lie       (1000) lie       (1000)     3801 2021-08-24 20:40:33.000000 pikaur-1.9/pikaur/pprint.py
+-rw-r--r--   0 lie       (1000) lie       (1000)    24653 2021-11-25 05:20:58.000000 pikaur-1.9/pikaur/print_department.py
+-rw-r--r--   0 lie       (1000) lie       (1000)     1897 2021-07-27 22:04:00.000000 pikaur-1.9/pikaur/progressbar.py
+-rw-r--r--   0 lie       (1000) lie       (1000)     7176 2021-09-22 17:07:40.000000 pikaur-1.9/pikaur/prompt.py
+-rw-r--r--   0 lie       (1000) lie       (1000)     2159 2018-07-25 03:24:33.000000 pikaur-1.9/pikaur/replacements.py
+-rw-r--r--   0 lie       (1000) lie       (1000)     6306 2021-09-22 17:11:37.000000 pikaur-1.9/pikaur/search_cli.py
+-rw-r--r--   0 lie       (1000) lie       (1000)     5563 2021-12-02 07:25:21.000000 pikaur-1.9/pikaur/srcinfo.py
+-rw-r--r--   0 lie       (1000) lie       (1000)     4751 2020-01-20 21:45:29.000000 pikaur-1.9/pikaur/updates.py
+-rw-r--r--   0 lie       (1000) lie       (1000)     3713 2021-08-25 20:07:15.000000 pikaur-1.9/pikaur/urllib.py
+-rw-r--r--   0 lie       (1000) lie       (1000)     6446 2021-06-30 12:32:22.000000 pikaur-1.9/pikaur/version.py
+drwxr-xr-x   0 lie       (1000) lie       (1000)        0 2021-12-14 18:24:16.698794 pikaur-1.9/pikaur.egg-info/
+-rw-r--r--   0 lie       (1000) lie       (1000)    13770 2021-12-14 18:24:16.000000 pikaur-1.9/pikaur.egg-info/PKG-INFO
+-rw-r--r--   0 lie       (1000) lie       (1000)      864 2021-12-14 18:24:16.000000 pikaur-1.9/pikaur.egg-info/SOURCES.txt
+-rw-r--r--   0 lie       (1000) lie       (1000)        1 2021-12-14 18:24:16.000000 pikaur-1.9/pikaur.egg-info/dependency_links.txt
+-rw-r--r--   0 lie       (1000) lie       (1000)       45 2021-12-14 18:24:16.000000 pikaur-1.9/pikaur.egg-info/entry_points.txt
+-rw-r--r--   0 lie       (1000) lie       (1000)        7 2021-12-14 18:24:16.000000 pikaur-1.9/pikaur.egg-info/requires.txt
+-rw-r--r--   0 lie       (1000) lie       (1000)        7 2021-12-14 18:24:16.000000 pikaur-1.9/pikaur.egg-info/top_level.txt
+-rw-r--r--   0 lie       (1000) lie       (1000)       38 2021-12-14 18:24:16.698794 pikaur-1.9/setup.cfg
+-rw-r--r--   0 lie       (1000) lie       (1000)     2009 2021-12-14 18:13:47.000000 pikaur-1.9/setup.py
```

### Comparing `pikaur-1.8/LICENSE` & `pikaur-1.9/LICENSE`

 * *Files identical despite different names*

### Comparing `pikaur-1.8/PKG-INFO` & `pikaur-1.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pikaur
-Version: 1.8
+Version: 1.9
 Summary: AUR helper with minimal dependencies
 Home-page: https://github.com/actionless/pikaur
 Author: Yauheni Kirylau
 Author-email: actionless.loveless@gmail.com
 License: UNKNOWN
 Keywords: arch linux aur helper
 Platform: UNKNOWN
```

### Comparing `pikaur-1.8/README.md` & `pikaur-1.9/README.md`

 * *Files identical despite different names*

### Comparing `pikaur-1.8/pikaur/__init__.py` & `pikaur-1.9/pikaur/__init__.py`

 * *Files identical despite different names*

### Comparing `pikaur-1.8/pikaur/argparse.py` & `pikaur-1.9/pikaur/argparse.py`

 * *Files identical despite different names*

### Comparing `pikaur-1.8/pikaur/args.py` & `pikaur-1.9/pikaur/args.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 """ This file is licensed under GPLv3, see https://www.gnu.org/licenses/ """
 
 import sys
-from argparse import Namespace  # pylint: disable=no-name-in-module
-from pprint import pprint  # pylint: disable=no-name-in-module
+from argparse import Namespace
+from pprint import pprint
 from typing import Any, List, NoReturn, Optional, Tuple, Union
 
 from .argparse import ArgumentParserWithUnknowns
 from .config import PikaurConfig
 from .i18n import _, _n
```

### Comparing `pikaur-1.8/pikaur/aur.py` & `pikaur-1.9/pikaur/aur.py`

 * *Files 2% similar despite different names*

```diff
@@ -68,14 +68,20 @@
                     'conflicts',
                     'replaces',
                     'provides',
                 ]
             }
         )
 
+    def __repr__(self) -> str:
+        return (
+            f'<{self.__class__.__name__} "{self.name}" '
+            f'{self.version}>'
+        )
+
 
 def construct_aur_rpc_url_from_uri(uri: str) -> str:
     url = AUR_BASE_URL + '/rpc/?' + uri
     return url
 
 
 def construct_aur_rpc_url_from_params(params: Dict[str, Union[str, int]]) -> str:
@@ -168,26 +174,27 @@
             ]
             pool.close()
             results = [request.get() for request in requests]
             pool.join()
             for result in results:
                 for aur_pkg in result:
                     _AUR_PKGS_FIND_CACHE[aur_pkg.name] = aur_pkg
-                    json_results.append(aur_pkg)
+                    if aur_pkg.name in package_names:
+                        json_results.append(aur_pkg)
 
     found_aur_packages = [
         result.name for result in json_results
     ]
-    not_found_packages: List[str] = []
-    if num_packages != len(found_aur_packages):
-        not_found_packages = [
+    not_found_packages: List[str] = (
+        [] if num_packages == len(found_aur_packages)
+        else [
             package for package in package_names
             if package not in found_aur_packages
         ]
-
+    )
     return json_results, not_found_packages
 
 
 def get_repo_url(package_base_name: str) -> str:
     return f'{AUR_BASE_URL}/{package_base_name}.git'
```

### Comparing `pikaur-1.8/pikaur/aur_deps.py` & `pikaur-1.9/pikaur/aur_deps.py`

 * *Files identical despite different names*

### Comparing `pikaur-1.8/pikaur/build.py` & `pikaur-1.9/pikaur/build.py`

 * *Files 2% similar despite different names*

```diff
@@ -267,15 +267,15 @@
         self.prepare_build_destination()
         if (
                 self._source_repo_updated
         ) or (
             not (is_devel_pkg(self.package_base) and check_dev_pkgs)
         ):
             return
-        print_stdout('{} {}...'.format(
+        print_stdout('{} {}...'.format(  # pylint: disable=consider-using-f-string
             color_line('::', 15),
             _n(
                 "Downloading the latest sources for a devel package {}",
                 "Downloading the latest sources for devel packages {}",
                 len(self.package_names)
             ).format(
                 bold_line(', '.join(self.package_names))
@@ -382,24 +382,24 @@
             all_package_builds: Dict[str, 'PackageBuild']
     ) -> None:
 
         self.get_deps(all_package_builds)
         if not self.built_deps_to_install:
             return
 
-        print_stderr('{} {}:'.format(
+        print_stderr('{} {}:'.format(  # pylint: disable=consider-using-f-string
             color_line('::', 13),
             _("Installing already built dependencies for {}").format(
                 bold_line(', '.join(self.package_names)))
         ))
 
         try:
             update_self_deps = False
             for pkg_name, pkg_build in all_package_builds.items():
-                if pkg_name in self.built_deps_to_install.keys():
+                if pkg_name in self.built_deps_to_install:
                     pkg_build.install_built_deps(all_package_builds)
                     update_self_deps = True
             if update_self_deps:
                 self.get_deps(all_package_builds)
             install_built_deps(
                 deps_names_and_paths=self.built_deps_to_install,
                 resolved_conflicts=self.resolved_conflicts
@@ -448,15 +448,15 @@
     def check_if_already_built(self) -> bool:
         self.get_latest_dev_sources()
         self._set_built_package_path()
         if (
                 not self.args.rebuild and
                 len(self.built_packages_paths) == len(self.package_names)
         ):
-            print_stderr("{} {}\n".format(
+            print_stderr("{} {}\n".format(  # pylint: disable=consider-using-f-string
                 color_line("::", 10),
                 _n(
                     "Package {pkg} is already built. Pass '--rebuild' flag to force the build.",
                     "Packages {pkg} are already built. Pass '--rebuild' flag to force the build.",
                     len(self.package_names)
                 ).format(
                     pkg=bold_line(", ".join(self.package_names))
@@ -525,15 +525,15 @@
         if filter_built:
             self._filter_built_deps(all_package_builds)
 
     def _install_repo_deps(self) -> None:
         if not self.all_deps_to_install:
             return
 
-        print_stderr('{} {}:'.format(
+        print_stderr('{} {}:'.format(  # pylint: disable=consider-using-f-string
             color_line('::', 13),
             _("Installing repository dependencies for {}").format(
                 bold_line(', '.join(self.package_names)))
         ))
 
         retry_interactive_command_or_exit(
             sudo(
@@ -595,15 +595,15 @@
                 )
             )
             if not ask_to_continue():
                 raise SysExit(125)
         if not deps_packages_installed or self.args.keepbuilddeps:
             return
 
-        print_stderr('{} {}:'.format(
+        print_stderr('{} {}:'.format(  # pylint: disable=consider-using-f-string
             color_line('::', 13),
             _("Removing already installed dependencies for {}").format(
                 bold_line(', '.join(self.package_names)))
         ))
         retry_interactive_command_or_exit(
             sudo(
                 # pacman --remove flag conflicts with some --sync options:
@@ -643,29 +643,32 @@
     def build_with_makepkg(self) -> bool:  # pylint: disable=too-many-branches,too-many-statements
         makepkg_args = []
         if not self.args.needed:
             makepkg_args.append('--force')
         if not color_enabled():
             makepkg_args.append('--nocolor')
 
-        print_stderr('\n{} {}:'.format(
+        print_stderr('\n{} {}:'.format(  # pylint: disable=consider-using-f-string
             color_line('::', 13),
             _('Starting the build')
         ))
         build_succeeded = False
         skip_pgp_check = False
         skip_file_checksums = False
+        skip_check = False
         while True:
             cmd_args = MakePkgCommand.get() + makepkg_args
             if skip_pgp_check:
                 cmd_args += ['--skippgpcheck']
             if skip_file_checksums:
                 cmd_args += ['--skipchecksums']
             if self.skip_carch_check:
                 cmd_args += ['--ignorearch']
+            if skip_check:
+                cmd_args += ['--nocheck']
             cmd_args = isolate_root_cmd(cmd_args, cwd=self.build_dir)
             spawn_kwargs: Dict[str, Any] = {}
             if self.args.hide_build_log:
                 spawn_kwargs = dict(
                     stdout=subprocess.PIPE,
                     stderr=subprocess.PIPE
                 )
@@ -683,44 +686,48 @@
                 ' '.join(cmd_args)
             ), 9))
             if PikaurConfig().build.SkipFailedBuild.get_bool():
                 answer = _("s")
             elif self.args.noconfirm:
                 answer = _("a")
             else:  # pragma: no cover
-                prompt = '{} {}\n{}\n> '.format(
+                prompt = '{} {}\n{}\n> '.format(  # pylint: disable=consider-using-f-string
                     color_line('::', 11),
                     _("Try recovering?"),
                     "\n".join((
                         _("[R] retry build"),
                         _("[p] PGP check skip"),
                         _("[c] checksums skip"),
+                        _("[f] check() skip"),
                         _("[i] ignore architecture"),
                         _("[d] delete build dir and try again"),
                         _("[e] edit PKGBUILD"),
                         "-" * 24,
                         _("[s] skip building this package"),
                         _("[a] abort building all the packages"),
                     ))
                 )
                 answer = get_input(
                     prompt,
-                    _('r').upper() + _('p') + _('c') + _('i') + _('d') + _('e') +
+                    _('r').upper() + _('p') + _('c') + _('f') + _('i') + _('d') + _('e') +
                     _('s') + _('a')
                 )
 
             answer = answer.lower()[0]
             if answer == _("r"):  # pragma: no cover
                 continue
             if answer == _("p"):  # pragma: no cover
                 skip_pgp_check = True
                 continue
             if answer == _("c"):  # pragma: no cover
                 skip_file_checksums = True
                 continue
+            if answer == _("f"):  # pragma: no cover
+                skip_check = True
+                continue
             if answer == _("i"):  # pragma: no cover
                 self.skip_carch_check = True
                 continue
             if answer == _("d"):  # pragma: no cover
                 self.prepare_build_destination(flush=True)
                 continue
             if answer == _('e'):  # pragma: no cover
```

### Comparing `pikaur-1.8/pikaur/config.py` & `pikaur-1.9/pikaur/config.py`

 * *Files 0% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 
 DEFAULT_CONFIG_ENCODING = 'utf-8'
 
 
 RUNNING_AS_ROOT = os.geteuid() == 0
 
 
-VERSION = '1.8-dev'
+VERSION = '1.9-dev'
 
 _USER_CACHE_HOME = os.environ.get(
     "XDG_CACHE_HOME",
     os.path.join(Path.home(), ".cache/")
 )
 if RUNNING_AS_ROOT:
     CACHE_ROOT = '/var/cache/pikaur'
```

### Comparing `pikaur-1.8/pikaur/conflicts.py` & `pikaur-1.9/pikaur/conflicts.py`

 * *Files identical despite different names*

### Comparing `pikaur-1.8/pikaur/core.py` & `pikaur-1.9/pikaur/core.py`

 * *Files 1% similar despite different names*

```diff
@@ -88,14 +88,15 @@
 
 
 class InstallInfo(DataType):
     name: str
     current_version: str
     new_version: str
     description: Optional[str] = None
+    maintainer: Optional[str] = None
     repository: Optional[str] = None
     devel_pkg_age_days: Optional[int] = None
     package: Union['pyalpm.Package', 'AURPackageInfo']
     provided_by: Optional[List[Union['pyalpm.Package', 'AURPackageInfo']]] = None
     required_by: Optional[List['InstallInfo']] = None
     members_of: Optional[List[str]] = None
     replaces: Optional[List[str]] = None
@@ -361,12 +362,12 @@
         privilege_escalation_tool = PikaurConfig().misc.PrivilegeEscalationTool.get_str()
         dep_names = ["fakeroot", ] + (
             [privilege_escalation_tool] if not running_as_root() else []
         )
 
     for dep_bin in dep_names:
         if not shutil.which(dep_bin):
-            print_error("'{}' {}.".format(
+            print_error("'{}' {}.".format(  # pylint: disable=consider-using-f-string
                 bold_line(dep_bin),
-                "executable not found"
+                _("executable not found")
             ))
             sys.exit(2)
```

### Comparing `pikaur-1.8/pikaur/exceptions.py` & `pikaur-1.9/pikaur/exceptions.py`

 * *Files identical despite different names*

### Comparing `pikaur-1.8/pikaur/filelock.py` & `pikaur-1.9/pikaur/filelock.py`

 * *Files identical despite different names*

### Comparing `pikaur-1.8/pikaur/getpkgbuild_cli.py` & `pikaur-1.9/pikaur/getpkgbuild_cli.py`

 * *Files identical despite different names*

### Comparing `pikaur-1.8/pikaur/help_cli.py` & `pikaur-1.9/pikaur/help_cli.py`

 * *Files 2% similar despite different names*

```diff
@@ -7,15 +7,15 @@
     get_pikaur_long_opts,
 )
 from .core import spawn
 
 
 def _format_options_help(options: List[Tuple[str, str, str]]) -> str:
     return '\n'.join([
-        '{:>5} {:<16} {}'.format(
+        '{:>5} {:<16} {}'.format(  # pylint: disable=consider-using-f-string
             short_opt and (short_opt + ',') or '',
             long_opt or '',
             descr if ((len(short_opt) + len(long_opt)) < 16) else f"\n{23 * ' '}{descr}"
         )
         for short_opt, long_opt, descr in options
     ])
```

### Comparing `pikaur-1.8/pikaur/info_cli.py` & `pikaur-1.9/pikaur/info_cli.py`

 * *Files 4% similar despite different names*

```diff
@@ -81,18 +81,16 @@
         pkg_info_lines = []
         for key, display_name in INFO_FIELDS.items():
             value = getattr(aur_pkg, key, None)
             if key in ['firstsubmitted', 'lastmodified', 'outofdate'] and value:
                 value = datetime.fromtimestamp(value).strftime('%c')
             elif isinstance(value, list):
                 value = ', '.join(value) or _("None")
-            pkg_info_lines.append('{key}: {value}'.format(
-                key=bold_line(_rightpad(display_name, longest_field_length + 1)),
-                value=value
-            ))
+            key_display = bold_line(_rightpad(display_name, longest_field_length + 1))
+            pkg_info_lines.append(f'{key_display}: {value}')
         print(
             _decorate_aur_info_output('\n'.join(pkg_info_lines)) +
             ('\n' if i + 1 < num_found else '')
         )
 
 
 def _rightpad(text: str, num: int) -> str:
```

### Comparing `pikaur-1.8/pikaur/install_cli.py` & `pikaur-1.9/pikaur/install_cli.py`

 * *Files 1% similar despite different names*

```diff
@@ -144,15 +144,15 @@
                 return
 
             if self.args.refresh:
                 PackageDB.discard_repo_cache()
                 print_stdout()
 
         if self.args.sysupgrade and not self.args.repo:
-            print_stderr('{} {}'.format(
+            print_stderr('{} {}'.format(  # pylint: disable=consider-using-f-string
                 color_line('::', 12),
                 bold_line(_("Starting full AUR upgrade..."))
             ))
         if self.args.aur:
             self.not_found_repo_pkgs_names = self.install_package_names
             self.install_package_names = []
         if self.args.pkgbuild:
@@ -198,15 +198,15 @@
         self.not_found_repo_pkgs_names = []
         self.pkgbuilds_packagelists = {
             path: [] for path in
             self.args.positional or ['PKGBUILD']
         }
 
     def aur_pkg_not_found_prompt(self, pkg_name: str) -> None:  # pragma: no cover
-        prompt = '{} {}\n{}\n{}\n{}\n> '.format(
+        prompt = '{} {}\n{}\n{}\n{}\n> '.format(  # pylint: disable=consider-using-f-string
             color_line('::', 11),
             _("Try recovering {pkg_name}?").format(pkg_name=bold_line(pkg_name)),
             _("[e] edit PKGBUILD"),
             _("[s] skip this package"),
             _("[A] abort")
         )
         answer = get_input(prompt, _('e') + _('s') + _('a').upper())
@@ -317,15 +317,15 @@
                 self.install_info.new_repo_deps_install_info or
                 self.install_info.thirdparty_repo_packages_install_info or
                 self.install_info.aur_updates_install_info
         ):
             if not self.args.aur and self.args.sysupgrade:
                 self.install_repo_packages()
             else:
-                print_stdout('{} {}'.format(
+                print_stdout('{} {}'.format(  # pylint: disable=consider-using-f-string
                     color_line('::', 10),
                     _("Nothing to do."),
                 ))
             raise SysExit(0)
 
     def _ignore_package(self, pkg_name: str) -> None:
         self.manually_excluded_packages_names.append(pkg_name)
@@ -383,15 +383,15 @@
             print_stdout(pretty_format_sysupgrade(
                 install_info=self.install_info,
                 verbose=verbose
             ))
 
         def _confirm_sysupgrade(verbose=False) -> str:
             _print_sysupgrade(verbose=verbose)
-            prompt = '{} {}\n{} {}\n>> '.format(
+            prompt = '{} {}\n{} {}\n>> '.format(  # pylint: disable=consider-using-f-string
                 color_line('::', 12),
                 bold_line(_('Proceed with installation? [Y/n] ')),
                 color_line('::', 12),
                 bold_line(_('[v]iew package details   [m]anually select packages')))
 
             answer = get_input(prompt, _('y').upper() + _('n') + _('v') + _('m'))
 
@@ -522,15 +522,15 @@
                     9
                 ))
                 print_stderr(err.result.stdout_text)
                 print_stderr(err.result.stderr_text)
                 if self.args.noconfirm:
                     answer = _("a")
                 else:  # pragma: no cover
-                    prompt = '{} {}\n> '.format(
+                    prompt = '{} {}\n> '.format(  # pylint: disable=consider-using-f-string
                         color_line('::', 11),
                         '\n'.join((
                             _("Try recovering?"),
                             _("[c] git checkout -- '*'"),
                             # _("[c] git checkout -- '*' ; git clean -f -d -x"),
                             _("[r] remove dir and clone again"),
                             _("[p] git stash && ... && git stash pop"),
@@ -614,15 +614,15 @@
                     print_stderr(color_line(
                         _("New packages '{new}' and '{other}' are in conflict.").format(
                             new=new_pkg_name, other=pkg_conflict),
                         9))
                     raise SysExit(131)
         for new_pkg_name, new_pkg_conflicts in self.found_conflicts.items():
             for pkg_conflict in new_pkg_conflicts:
-                answer = ask_to_continue('{} {}'.format(
+                answer = ask_to_continue('{} {}'.format(  # pylint: disable=consider-using-f-string
                     color_line('::', 11),
                     bold_line(_(
                         "{new} and {installed} are in conflict. Remove {installed}?"
                     ).format(
                         new=new_pkg_name, installed=pkg_conflict
                     ))
                 ), default_yes=False)
@@ -633,15 +633,15 @@
     def ask_to_edit_file(
             self, filename: str, package_build: PackageBuild
     ) -> bool:  # pragma: no cover
         noedit = not self.args.edit and (
             self.args.noedit
         )
         if noedit or self.args.noconfirm:
-            print_stderr('{} {}'.format(
+            print_stderr('{} {}'.format(  # pylint: disable=consider-using-f-string
                 color_line('::', 11),
                 _("Skipping review of {file} for {name} package ({flag})").format(
                     file=filename,
                     name=', '.join(package_build.package_names),
                     flag=(noedit and '--noedit') or
                     (self.args.noconfirm and '--noconfirm')),
             ))
@@ -791,14 +791,15 @@
                 if install_file_name:
                     self.ask_to_edit_file(install_file_name, pkg_build)
 
             pkg_build.check_pkg_arch()
             pkg_build.reviewed = True
 
     def handle_pkgbuild_changed(self, pkg_build: PackageBuild) -> None:
+        debug(f'handle pkgbuild changed {pkg_build=}')
         for pkg_name in pkg_build.package_names:
             self.discard_install_info(pkg_name, ignore=False)
         src_info = SrcInfo(pkgbuild_path=pkg_build.pkgbuild_path)
         old_srcinfo_hash = hash_file(src_info.path)
         src_info.regenerate()
         new_srcinfo_hash = hash_file(src_info.path)
 
@@ -860,15 +861,16 @@
                 print_stderr(
                     color_line(_("Can't build '{name}'.").format(name=pkg_name) + '\n', 9)
                 )
                 # if not ask_to_continue():
                 #     raise SysExit(125)
                 for _pkg_name in pkg_build.package_names:
                     failed_to_build_package_names.append(_pkg_name)
-                    packages_to_be_built.remove(_pkg_name)
+                    if _pkg_name in packages_to_be_built:
+                        packages_to_be_built.remove(_pkg_name)
                     self.discard_install_info(_pkg_name)
                     for remaining_aur_pkg_name in packages_to_be_built[:]:
                         if remaining_aur_pkg_name not in self.all_aur_packages_names:
                             packages_to_be_built.remove(remaining_aur_pkg_name)
             except DependencyNotBuiltYet as exc:
                 index += 1
                 for _pkg_name in pkg_build.package_names:
```

### Comparing `pikaur-1.8/pikaur/install_info_fetcher.py` & `pikaur-1.9/pikaur/install_info_fetcher.py`

 * *Files 1% similar despite different names*

```diff
@@ -370,14 +370,19 @@
             f"    {self.aur_updates_install_info=}\n"
             f"    {aur_packages_names_to_versions=}"
         )
         local_pkgs = PackageDB.get_local_dict()
         aur_pkg_list, not_found_aur_pkgs = find_aur_packages(
             list(aur_packages_names_to_versions.keys())
         )
+        debug(
+            f"found AUR pkgs:\n"
+            f"    {aur_pkg_list=}\n"
+            f"    {not_found_aur_pkgs=}\n"
+        )
         aur_pkgs = {}
         for aur_pkg in aur_pkg_list:
             if aur_packages_names_to_versions[aur_pkg.name](aur_pkg.version):
                 aur_pkgs[aur_pkg.name] = aur_pkg
             else:
                 not_found_aur_pkgs.append(aur_packages_names_to_versions[aur_pkg.name].line)
         if not_found_aur_pkgs:
@@ -397,14 +402,15 @@
                 continue
             local_pkg = local_pkgs.get(pkg_name)
             aur_updates_install_info_by_name[pkg_name] = InstallInfo(
                 name=pkg_name,
                 current_version=local_pkg.version if local_pkg else ' ',
                 new_version=aur_pkg.version,
                 description=aur_pkg.desc,
+                maintainer=aur_pkg.maintainer,
                 package=aur_pkg,
             )
         for pkg_name in list(aur_updates_install_info_by_name.keys())[:]:
             if (
                     self.package_is_manually_excluded(pkg_name)
             ) or (
                 self.package_is_ignored(pkg_name)
@@ -482,14 +488,15 @@
             aur_pkg = aur_pkgs[pkg_name]
             local_pkg = local_pkgs.get(pkg_name)
             self.aur_deps_install_info.append(InstallInfo(
                 name=pkg_name,
                 current_version=local_pkg.version if local_pkg else ' ',
                 new_version=aur_pkg.version,
                 description=aur_pkg.desc,
+                maintainer=aur_pkg.maintainer,
                 package=aur_pkg,
             ))
 
     def mark_dependent(self) -> None:  # pylint: disable=too-many-locals
         """
         update packages' install info to show deps in prompt:
         """
```

### Comparing `pikaur-1.8/pikaur/main.py` & `pikaur-1.9/pikaur/main.py`

 * *Files 2% similar despite different names*

```diff
@@ -125,16 +125,16 @@
     args = parse_args()
     if not args.repo:
         for directory, message, minimal_clean_level in (
                 (BUILD_CACHE_PATH, _("Build directory"), 1, ),
                 (PACKAGE_CACHE_PATH, _("Packages directory"), 2, ),
         ):
             if minimal_clean_level <= args.clean and os.path.exists(directory):
-                print_stdout('\n' + "{}: {}".format(message, directory))
-                if ask_to_continue(text='{} {}'.format(
+                print_stdout(f"\n{message}: {directory}")
+                if ask_to_continue(text='{} {}'.format(  # pylint: disable=consider-using-f-string
                         color_line('::', 12),
                         bold_line(_("Do you want to remove all files?"))
                 )):
                     remove_dir(directory)
     if not args.aur:
         raise SysExit(
             interactive_spawn(sudo(
@@ -290,15 +290,15 @@
         return
     if not os.path.exists(DATA_ROOT):
         os.makedirs(DATA_ROOT)
     shutil.move(_OLD_AUR_REPOS_CACHE_PATH, AUR_REPOS_CACHE_PATH)
 
     print_stderr()
     print_warning(
-        _("AUR repos dir has been moved from '{old}' to '{new}'.".format(
+        _("AUR repos dir has been moved from '{old}' to '{new}'.".format(  # pylint: disable=consider-using-f-string
             old=_OLD_AUR_REPOS_CACHE_PATH,
             new=AUR_REPOS_CACHE_PATH
         ))
     )
     print_stderr()
```

### Comparing `pikaur-1.8/pikaur/makepkg_config.py` & `pikaur-1.9/pikaur/makepkg_config.py`

 * *Files identical despite different names*

### Comparing `pikaur-1.8/pikaur/news.py` & `pikaur-1.9/pikaur/news.py`

 * *Files identical despite different names*

### Comparing `pikaur-1.8/pikaur/pacman.py` & `pikaur-1.9/pikaur/pacman.py`

 * *Files 0% similar despite different names*

```diff
@@ -331,15 +331,15 @@
             cls, package_source: PackageSource
     ) -> Dict[str, List[ProvidedDependency]]:
 
         if not cls._provided_dict_cache.get(package_source):
             provided_pkg_names = super()._get_provided_dict(package_source)
             if package_source == PackageSource.REPO:
                 for _what_provides, provided_pkgs in provided_pkg_names.items():
-                    provided_pkgs.sort(key=lambda p: "{}{}".format(
+                    provided_pkgs.sort(key=lambda p: "{}{}".format(  # pylint: disable=consider-using-f-string
                         cls.get_repo_priority(p.package.db.name),
                         p.package.name
                     ))
             cls._provided_dict_cache[package_source] = provided_pkg_names
         return cls._provided_dict_cache[package_source]
 
     @classmethod
```

### Comparing `pikaur-1.8/pikaur/pikspect.py` & `pikaur-1.9/pikaur/pikspect.py`

 * *Files 2% similar despite different names*

```diff
@@ -355,15 +355,15 @@
     class YesNo:
         ANSWER_Y = _p("Y")
         ANSWER_N = _p("N")
         QUESTION_YN_YES = _p("[Y/n]")
         QUESTION_YN_NO = _p("[y/N]")
 
     def format_pacman_question(message: str, question=YesNo.QUESTION_YN_YES) -> str:
-        return bold_line(" {} {} ".format(_p(message), question))
+        return bold_line(f" {_p(message)} {question} ")
 
     class Questions:
         PROCEED = [
             format_pacman_question('Proceed with installation?'),
             format_pacman_question('Proceed with download?'),
         ]
         REMOVE = format_pacman_question('Do you want to remove these packages?')
```

### Comparing `pikaur-1.8/pikaur/pprint.py` & `pikaur-1.9/pikaur/pprint.py`

 * *Files identical despite different names*

### Comparing `pikaur-1.8/pikaur/print_department.py` & `pikaur-1.9/pikaur/print_department.py`

 * *Files 8% similar despite different names*

```diff
@@ -22,14 +22,15 @@
 if TYPE_CHECKING:
     # pylint: disable=unused-import,cyclic-import
     from .install_info_fetcher import InstallInfoFetcher  # noqa
 
 
 GROUP_COLOR = 4
 REPLACEMENTS_COLOR = 14
+ORPHANED_COLOR = 9
 
 
 AnyPackage = Union[AURPackageInfo, pyalpm.Package]
 
 
 def print_version(pacman_version: str, pyalpm_version: str, quiet=False) -> None:
     if quiet:
@@ -124,15 +125,15 @@
     _bold_line = bold_line
     if not color:
         _color_line = lambda line, *args, **kwargs: line  # noqa
         _bold_line = lambda line: line  # noqa
 
     SortKey = Union[Tuple, str]
 
-    def pretty_format(pkg_update: 'InstallInfo') -> Tuple[str, SortKey]:  # pylint:disable=too-many-locals
+    def pretty_format(pkg_update: 'InstallInfo') -> Tuple[str, SortKey]:  # pylint:disable=too-many-locals,R0912
         common_version, diff_weight = get_common_version(
             pkg_update.current_version or '', pkg_update.new_version or ''
         )
         user_config = PikaurConfig()
         color_config = user_config.colors
         version_color = color_config.Version.get_int()
         old_color = color_config.VersionDiffOld.get_int()
@@ -153,28 +154,28 @@
             )
 
         pkg_name = pkg_update.name
         pkg_len = len(pkg_update.name)
 
         pkg_name = _bold_line(pkg_name)
         if (print_repo or verbose) and pkg_update.repository:
-            pkg_name = '{}{}'.format(
+            pkg_name = '{}{}'.format(  # pylint: disable=consider-using-f-string
                 pretty_format_repo_name(pkg_update.repository, color=color),
                 pkg_name
             )
             pkg_len += len(pkg_update.repository) + 1
         elif print_repo:
-            pkg_name = '{}{}'.format(
+            pkg_name = '{}{}'.format(  # pylint: disable=consider-using-f-string
                 _color_line('aur/', 9),
                 pkg_name
             )
             pkg_len += len('aur/')
 
         if pkg_update.required_by:
-            required_by = ' ({})'.format(
+            required_by = ' ({})'.format(  # pylint: disable=consider-using-f-string
                 _('for {pkg}').format(
                     pkg=', '.join([p.package.name for p in pkg_update.required_by])
                 )
             )
             pkg_len += len(required_by)
             dep_color = 3
             required_by = _color_line(' ({})', dep_color).format(
@@ -182,36 +183,36 @@
                     pkg=_color_line(', ', dep_color).join([
                         _color_line(p.package.name, dep_color + 8) for p in pkg_update.required_by
                     ]) + _color_line('', dep_color, reset=False),
                 )
             )
             pkg_name += required_by
         if pkg_update.provided_by:
-            provided_by = ' ({})'.format(
+            provided_by = ' ({})'.format(  # pylint: disable=consider-using-f-string
                 ' # '.join([p.name for p in pkg_update.provided_by])
             )
             pkg_len += len(provided_by)
             pkg_name += _color_line(provided_by, 2)
         if pkg_update.members_of:
-            members_of = ' ({})'.format(
+            members_of = ' ({})'.format(  # pylint: disable=consider-using-f-string
                 _n('{grp} group', '{grp} groups', len(pkg_update.members_of)).format(
                     grp=', '.join(g for g in pkg_update.members_of),
                 )
             )
             pkg_len += len(members_of)
             members_of = _color_line(' ({})', GROUP_COLOR).format(
                 _n('{grp} group', '{grp} groups', len(pkg_update.members_of)).format(
                     grp=_color_line(', ', GROUP_COLOR).join(
                         [_color_line(g, GROUP_COLOR + 8) for g in pkg_update.members_of]
                     ) + _color_line('', GROUP_COLOR, reset=False),
                 )
             )
             pkg_name += _color_line(members_of, GROUP_COLOR)
         if pkg_update.replaces:
-            replaces = ' (replaces {})'.format(
+            replaces = ' (replaces {})'.format(  # pylint: disable=consider-using-f-string
                 ', '.join(g for g in pkg_update.replaces)
             )
             pkg_len += len(replaces)
             pkg_name += _color_line(replaces, REPLACEMENTS_COLOR)
             if not color:
                 pkg_name = f'# {pkg_name}'
 
@@ -222,21 +223,29 @@
         ):
             pkg_size = f'{pkg_update.package.size/1024/1024:.2f} MiB'
 
         days_old = ''
         if pkg_update.devel_pkg_age_days:
             days_old = ' ' + _('({} days old)').format(pkg_update.devel_pkg_age_days)
 
+        if (
+                isinstance(pkg_update.package, AURPackageInfo) and
+                pkg_update.package.maintainer is None
+        ):
+            orphaned = f" [{_('orphaned')}]"
+            pkg_len += len(orphaned)
+            pkg_name += _color_line(orphaned, ORPHANED_COLOR)
+
         out_of_date = ''
         if (
                 isinstance(pkg_update.package, AURPackageInfo) and
                 pkg_update.package.outofdate is not None
         ):
             out_of_date = _color_line(
-                " [{}: {}]".format(
+                " [{}: {}]".format(  # pylint: disable=consider-using-f-string
                     _("outofdate"),
                     datetime.fromtimestamp(pkg_update.package.outofdate).strftime('%Y/%m/%d')
                 ),
                 color_config.VersionDiffOld.get_int()
             )
 
         return (
@@ -328,101 +337,101 @@
     if not color:
         _color_line = lambda line, *args: line  # noqa
         _bold_line = lambda line: line  # noqa
 
     result = []
 
     if repo_replacements:
-        result.append('\n{} {}'.format(
+        result.append('\n{} {}'.format(  # pylint: disable=consider-using-f-string
             _color_line('::', 12),
             _bold_line(_n(
                 "Repository package suggested as a replacement:",
                 "Repository packages suggested as a replacement:",
                 len(repo_replacements)))
         ))
         result.append(pretty_format_upgradeable(
             repo_replacements,
             verbose=verbose, color=color,
             print_repo=PikaurConfig().sync.AlwaysShowPkgOrigin.get_bool()
         ))
     if thirdparty_repo_replacements:
-        result.append('\n{} {}'.format(
+        result.append('\n{} {}'.format(  # pylint: disable=consider-using-f-string
             _color_line('::', 12),
             _bold_line(_n(
                 "Third-party repository package suggested as a replacement:",
                 "Third-party repository packages suggested as a replacement:",
                 len(repo_packages_updates)))
         ))
         result.append(pretty_format_upgradeable(
             thirdparty_repo_replacements,
             verbose=verbose, color=color,
             print_repo=PikaurConfig().sync.AlwaysShowPkgOrigin.get_bool()
         ))
 
     if repo_packages_updates:
-        result.append('\n{} {}'.format(
+        result.append('\n{} {}'.format(  # pylint: disable=consider-using-f-string
             _color_line('::', 12),
             _bold_line(_n(
                 "Repository package will be installed:",
                 "Repository packages will be installed:",
                 len(repo_packages_updates)))
         ))
         result.append(pretty_format_upgradeable(
             repo_packages_updates,
             verbose=verbose, color=color,
             print_repo=PikaurConfig().sync.AlwaysShowPkgOrigin.get_bool()
         ))
     if new_repo_deps:
-        result.append('\n{} {}'.format(
+        result.append('\n{} {}'.format(  # pylint: disable=consider-using-f-string
             _color_line('::', 11),
             _bold_line(_n("New dependency will be installed from repository:",
                           "New dependencies will be installed from repository:",
                           len(new_repo_deps)))
         ))
         result.append(pretty_format_upgradeable(
             new_repo_deps,
             verbose=verbose, color=color,
             print_repo=PikaurConfig().sync.AlwaysShowPkgOrigin.get_bool()
         ))
     if thirdparty_repo_packages_updates:
-        result.append('\n{} {}'.format(
+        result.append('\n{} {}'.format(  # pylint: disable=consider-using-f-string
             _color_line('::', 12),
             _bold_line(_n("Third-party repository package will be installed:",
                           "Third-party repository packages will be installed:",
                           len(thirdparty_repo_packages_updates)))
         ))
         result.append(pretty_format_upgradeable(
             thirdparty_repo_packages_updates,
             verbose=verbose, color=color, print_repo=True
         ))
     if new_thirdparty_repo_deps:
-        result.append('\n{} {}'.format(
+        result.append('\n{} {}'.format(  # pylint: disable=consider-using-f-string
             _color_line('::', 11),
             _bold_line(_n("New dependency will be installed from third-party repository:",
                           "New dependencies will be installed from third-party repository:",
                           len(new_thirdparty_repo_deps)))
         ))
         result.append(pretty_format_upgradeable(
             new_thirdparty_repo_deps,
             verbose=verbose, color=color,
             print_repo=PikaurConfig().sync.AlwaysShowPkgOrigin.get_bool()
         ))
     if aur_updates:
-        result.append('\n{} {}'.format(
+        result.append('\n{} {}'.format(  # pylint: disable=consider-using-f-string
             _color_line('::', 14),
             _bold_line(_n("AUR package will be installed:",
                           "AUR packages will be installed:",
                           len(aur_updates)))
         ))
         result.append(pretty_format_upgradeable(
             aur_updates,
             verbose=verbose, color=color, print_repo=False
         ))
     if new_aur_deps:
-        result.append('\n{} {}'.format(
+        result.append('\n{} {}'.format(  # pylint: disable=consider-using-f-string
             _color_line('::', 11),
             _bold_line(_n("New dependency will be installed from AUR:",
                           "New dependencies will be installed from AUR:",
                           len(new_aur_deps)))
         ))
         result.append(pretty_format_upgradeable(
             new_aur_deps,
@@ -440,15 +449,15 @@
         raise TypeError("Either 'package_name' or 'install_info' should be specified")
     install_info = install_info or InstallInfo(
         name=package_name,
         current_version='',
         new_version='',
         package=None,
     )
-    print_stderr('{} {}'.format(
+    print_stderr('{} {}'.format(  # pylint: disable=consider-using-f-string
         color_line('::', 11),
         _("Ignoring package update {}").format(
             pretty_format_upgradeable(
                 [install_info],
                 template="{pkg_name} ({current_version} => {new_version})"
             ))
         if (install_info.current_version and install_info.new_version) else
@@ -579,15 +588,17 @@
 
             repo = color_line('aur/', 9)
             if isinstance(package, pyalpm.Package):
                 repo = pretty_format_repo_name(package.db.name)
 
             groups = ''
             if getattr(package, 'groups', None):
-                groups = color_line('({}) '.format(' '.join(package.groups)), GROUP_COLOR)
+                groups = color_line('({}) '.format(  # pylint: disable=consider-using-f-string
+                    ' '.join(package.groups)
+                ), GROUP_COLOR)
 
             installed = ''
             if pkg_name in local_pkgs_names:
                 if package.version != local_pkgs_versions[pkg_name]:
                     installed = color_line(_("[installed: {version}]").format(
                         version=local_pkgs_versions[pkg_name],
                     ) + ' ', 14)
@@ -598,47 +609,44 @@
             if (
                     isinstance(package, AURPackageInfo)
             ) and (
                 package.numvotes is not None
             ) and (
                 package.popularity is not None
             ):
-                rating = color_line('({}, {:.2f})'.format(
-                    package.numvotes,
-                    package.popularity
-                ), 3)
+                rating = color_line(f'({package.numvotes}, {package.popularity:.2f})', 3)
 
             color_config = user_config.colors
             version_color = color_config.Version.get_int()
             version = package.version
 
             if isinstance(package, AURPackageInfo) and package.outofdate is not None:
                 version_color = color_config.VersionDiffOld.get_int()
-                version = "{} [{}: {}]".format(
+                version = "{} [{}: {}]".format(  # pylint: disable=consider-using-f-string
                     package.version,
                     _("outofdate"),
                     datetime.fromtimestamp(package.outofdate).strftime('%Y/%m/%d')
                 )
 
             last_updated = ""
             if user_config.ui.DisplayLastUpdated.get_bool():
                 last_update_date = None
 
                 if isinstance(package, pyalpm.Package):
                     last_update_date = package.builddate
                 if isinstance(package, AURPackageInfo):
                     last_update_date = package.lastmodified
 
-                last_updated = color_line(' (last updated: {})'.format(
+                last_updated = color_line(' (last updated: {})'.format(  # pylint: disable=consider-using-f-string
                     datetime.fromtimestamp(last_update_date).strftime('%Y/%m/%d')
                     if last_update_date is not None
                     else 'unknown'
                 ), 8)
 
-            print("{}{}{} {} {}{}{}{}".format(
+            print("{}{}{} {} {}{}{}{}".format(  # pylint: disable=consider-using-f-string
                 idx,
                 repo,
                 bold_line(pkg_name),
                 color_line(version, version_color),
                 groups,
                 installed,
                 rating,
```

### Comparing `pikaur-1.8/pikaur/progressbar.py` & `pikaur-1.9/pikaur/progressbar.py`

 * *Files identical despite different names*

### Comparing `pikaur-1.8/pikaur/prompt.py` & `pikaur-1.9/pikaur/prompt.py`

 * *Files 5% similar despite different names*

```diff
@@ -61,27 +61,27 @@
         return ' '
     except Exception:
         return ' '
     finally:
         tty.tcsetattr(  # type: ignore[attr-defined]
             sys.stdin.fileno(), tty.TCSADRAIN, previous_tty_settings  # type: ignore[attr-defined]
         )
-        sys.stdout.write('{}\r\n'.format(answer))
+        sys.stdout.write(f'{answer}\r\n')
         tty.tcdrain(sys.stdin.fileno())  # type: ignore[attr-defined]
 
 
 def split_last_line(text: str) -> str:
     all_lines = text.split('\n')
     n_lines = len(all_lines)
     last_line = all_lines[n_lines - 1]
     term_width = get_term_width()
     if len(last_line) < term_width:
         return text
     prev_lines = all_lines[:n_lines - 1]
-    last_line = "{}\n{}".format(
+    last_line = "{}\n{}".format(  # pylint: disable=consider-using-f-string
         range_printable(last_line, 0, term_width),
         range_printable(last_line, term_width)
     )
     return '\n'.join(prev_lines + [last_line])
 
 
 def _debug(message, *args, **kwargs):
@@ -164,21 +164,19 @@
 
 def ask_to_continue(text: str = None, default_yes: bool = True) -> bool:
     args = parse_args()
     if text is None:
         text = _('Do you want to proceed?')
 
     if args.noconfirm:
-        print_stderr('{} {}'.format(
-            text,
-            _("[Y]es (--noconfirm)") if default_yes else _("[N]o (--noconfirm)")
-        ))
+        default_option = ("[Y]es (--noconfirm)") if default_yes else _("[N]o (--noconfirm)")
+        print_stderr(f'{text} {default_option}')
         return default_yes
 
-    prompt = text + (' [%s/%s] ' % (Y_UP, N) if default_yes else ' [%s/%s] ' % (Y, N_UP))
+    prompt = text + (f' [{Y_UP}/{N}] ' if default_yes else f' [{Y}/{N_UP}] ')
     answers = Y_UP + N if default_yes else Y + N_UP
 
     answer = get_input(prompt, answers)
     return (answer == Y) or (default_yes and answer == '')
 
 
 def retry_interactive_command(
```

### Comparing `pikaur-1.8/pikaur/replacements.py` & `pikaur-1.9/pikaur/replacements.py`

 * *Files identical despite different names*

### Comparing `pikaur-1.8/pikaur/search_cli.py` & `pikaur-1.9/pikaur/search_cli.py`

 * *Files 1% similar despite different names*

```diff
@@ -157,15 +157,15 @@
         for request_repo in requests_repo:
             pkgs_found = request_repo.get()
             if pkgs_found:
                 result_repo.append(pkgs_found)
         try:
             result_aur = request_aur.get() if request_aur else None
         except AURError as exc:
-            print_stderr('AUR returned error: {}'.format(exc))
+            print_stderr(f'_("AUR returned error:") {exc}')
             raise SysExit(121) from exc
         pool.join()
 
     if not args.quiet:
         sys.stderr.write('\n')
 
     repo_result = (
```

### Comparing `pikaur-1.8/pikaur/srcinfo.py` & `pikaur-1.9/pikaur/srcinfo.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,13 +1,15 @@
 """ This file is licensed under GPLv3, see https://www.gnu.org/licenses/ """
 
 import os
+import shutil
 from typing import List, Dict, Optional
 
-from .core import open_file, spawn, isolate_root_cmd, dirname
+from .config import BUILD_CACHE_PATH, CACHE_ROOT
+from .core import open_file, spawn, isolate_root_cmd, dirname, running_as_root
 from .version import VersionMatcher
 from .makepkg_config import MakepkgConfig, MakePkgCommand
 from .pprint import print_stderr, print_error
 from .i18n import _
 from .exceptions import SysExit
 
 
@@ -114,29 +116,35 @@
         return self._get_build_depends('makedepends')
 
     def get_build_checkdepends(self) -> Dict[str, VersionMatcher]:
         return self._get_build_depends('checkdepends')
 
     def get_version(self) -> str:
         epoch = self.get_value('epoch')
+        epoch_display = (epoch + ':') if epoch else ''
         version = self.get_value('pkgver')
         release = self.get_value('pkgrel')
-        return '{}{}-{}'.format(
-            (epoch + ':') if epoch else '',
-            version,
-            release
-        )
+        return f'{epoch_display}{version}-{release}'
 
     def regenerate(self) -> None:
+        working_directory = self.repo_path
+        if running_as_root() and not self.repo_path.startswith(CACHE_ROOT):
+            working_directory = os.path.join(
+                BUILD_CACHE_PATH,
+                '_info_' + (self.get_value('pkgbase') or 'unknown')
+            )
+            if not os.path.exists(working_directory):
+                os.mkdir(working_directory)
+            shutil.copy(self.pkgbuild_path, working_directory)
         result = spawn(
             isolate_root_cmd(
                 MakePkgCommand.get() + ['--printsrcinfo'] +
                 ['-p', os.path.basename(self.pkgbuild_path)],
-                cwd=self.repo_path
-            ), cwd=self.repo_path
+                cwd=working_directory
+            ), cwd=working_directory
         )
         if result.returncode != 0:
             print_error(_("failed to generate .SRCINFO from {}:").format(self.pkgbuild_path))
             print_stderr(result.stderr_text)
             raise SysExit(5)
         with open_file(self.path, 'w') as srcinfo_file:
             srcinfo_file.write(result.stdout_text)
```

### Comparing `pikaur-1.8/pikaur/updates.py` & `pikaur-1.9/pikaur/updates.py`

 * *Files identical despite different names*

### Comparing `pikaur-1.8/pikaur/urllib.py` & `pikaur-1.9/pikaur/urllib.py`

 * *Files identical despite different names*

### Comparing `pikaur-1.8/pikaur/version.py` & `pikaur-1.9/pikaur/version.py`

 * *Files identical despite different names*

### Comparing `pikaur-1.8/pikaur.egg-info/PKG-INFO` & `pikaur-1.9/pikaur.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pikaur
-Version: 1.8
+Version: 1.9
 Summary: AUR helper with minimal dependencies
 Home-page: https://github.com/actionless/pikaur
 Author: Yauheni Kirylau
 Author-email: actionless.loveless@gmail.com
 License: UNKNOWN
 Keywords: arch linux aur helper
 Platform: UNKNOWN
```

### Comparing `pikaur-1.8/pikaur.egg-info/SOURCES.txt` & `pikaur-1.9/pikaur.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pikaur-1.8/setup.py` & `pikaur-1.9/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -12,15 +12,15 @@
 HERE = path.abspath(path.dirname(__file__))
 
 with codecs.open(path.join(HERE, 'README.md'), encoding='utf-8') as f:
     LONG_DESCRIPTION = f.read()
 
 SETUP_ARGS: Dict[str, Any] = dict(
     name='pikaur',  # Required
-    version='1.8',  # Required
+    version='1.9',  # Required
     description='AUR helper with minimal dependencies',  # Required
     long_description=LONG_DESCRIPTION,  # Optional
     url='https://github.com/actionless/pikaur',  # Optional
     author='Yauheni Kirylau',  # Optional
     author_email='actionless.loveless@gmail.com',  # Optional
     classifiers=[
         'Development Status :: 5 - Production/Stable',
```

