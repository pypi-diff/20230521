# Comparing `tmp/pyloobins-0.1.6.tar.gz` & `tmp/pyloobins-0.1.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyloobins-0.1.6.tar", max compression
+gzip compressed data, was "pyloobins-0.1.7.tar", max compression
```

## Comparing `pyloobins-0.1.6.tar` & `pyloobins-0.1.7.tar`

### file list

```diff
@@ -1,34 +1,34 @@
--rw-r--r--   0        0        0    35149 2023-04-11 23:56:04.085551 pyloobins-0.1.6/LICENSE
--rw-r--r--   0        0        0      885 2023-05-01 23:30:07.408912 pyloobins-0.1.6/LOOBins/GetFileInfo.yml
--rw-r--r--   0        0        0     1412 2023-05-01 23:30:07.409275 pyloobins-0.1.6/LOOBins/SetFile.yml
--rw-r--r--   0        0        0     1410 2023-05-17 23:34:53.847985 pyloobins-0.1.6/LOOBins/csrutil.yml
--rw-r--r--   0        0        0     2449 2023-05-08 00:30:49.737329 pyloobins-0.1.6/LOOBins/ditto.yml
--rw-r--r--   0        0        0     1644 2023-05-20 14:12:36.410173 pyloobins-0.1.6/LOOBins/dns-sd.yml
--rw-r--r--   0        0        0     3545 2023-05-01 23:30:07.409751 pyloobins-0.1.6/LOOBins/dscl.yml
--rw-r--r--   0        0        0     2138 2023-05-01 23:30:07.409978 pyloobins-0.1.6/LOOBins/ioreg.yml
--rw-r--r--   0        0        0     1538 2023-05-01 01:46:27.775139 pyloobins-0.1.6/LOOBins/last.yml
--rw-r--r--   0        0        0     1869 2023-05-17 23:34:53.848702 pyloobins-0.1.6/LOOBins/lsregister.yml
--rw-r--r--   0        0        0     1763 2023-05-14 23:57:44.222650 pyloobins-0.1.6/LOOBins/mdfind.yml
--rw-r--r--   0        0        0     4420 2023-05-01 23:30:07.410858 pyloobins-0.1.6/LOOBins/networksetup.yml
--rw-r--r--   0        0        0      868 2023-05-15 00:11:31.657614 pyloobins-0.1.6/LOOBins/open.yml
--rw-r--r--   0        0        0     1229 2023-05-15 23:03:47.041630 pyloobins-0.1.6/LOOBins/osacompile.yml
--rw-r--r--   0        0        0     3237 2023-05-01 23:30:07.411097 pyloobins-0.1.6/LOOBins/osascript.yml
--rw-r--r--   0        0        0     1263 2023-05-01 23:30:07.411462 pyloobins-0.1.6/LOOBins/pbpaste.yml
--rw-r--r--   0        0        0     1259 2023-05-11 01:22:04.795362 pyloobins-0.1.6/LOOBins/plutil.yml
--rw-r--r--   0        0        0     1249 2023-05-17 23:34:53.848926 pyloobins-0.1.6/LOOBins/profiles.yml
--rw-r--r--   0        0        0     1051 2023-05-01 01:46:27.801548 pyloobins-0.1.6/LOOBins/screencapture.yml
--rw-r--r--   0        0        0     2458 2023-05-01 01:46:27.474479 pyloobins-0.1.6/LOOBins/security.yml
--rw-r--r--   0        0        0      840 2023-05-01 23:30:07.411670 pyloobins-0.1.6/LOOBins/softwareupdate.yml
--rw-r--r--   0        0        0      790 2023-05-01 23:30:07.411980 pyloobins-0.1.6/LOOBins/sysctl.yml
--rw-r--r--   0        0        0     1158 2023-05-18 14:49:43.472269 pyloobins-0.1.6/LOOBins/tclsh.yml
--rw-r--r--   0        0        0     1993 2023-05-11 01:17:33.005665 pyloobins-0.1.6/LOOBins/textutil.yml
--rw-r--r--   0        0        0     2034 2023-05-06 18:13:38.210711 pyloobins-0.1.6/LOOBins/tmutil.yml
--rw-r--r--   0        0        0     1636 2023-04-23 17:34:43.219172 pyloobins-0.1.6/LOOBins/xattr.yml
--rw-r--r--   0        0        0      559 2023-05-09 23:38:24.844556 pyloobins-0.1.6/README.md
--rw-r--r--   0        0        0     1212 2023-05-20 14:54:20.754666 pyloobins-0.1.6/pyproject.toml
--rw-r--r--   0        0        0        0 2023-04-07 02:06:55.452190 pyloobins-0.1.6/src/pyloobins/__init__.py
--rw-r--r--   0        0        0     2187 2023-05-20 14:54:20.754917 pyloobins-0.1.6/src/pyloobins/cli.py
--rw-r--r--   0        0        0     4015 2023-05-15 23:42:52.127853 pyloobins-0.1.6/src/pyloobins/models.py
--rw-r--r--   0        0        0     1311 2023-05-01 23:30:07.412430 pyloobins-0.1.6/src/pyloobins/templates/loobin.md.j2
--rw-r--r--   0        0        0     2761 2023-05-20 14:54:20.755132 pyloobins-0.1.6/src/pyloobins/util.py
--rw-r--r--   0        0        0     1442 1970-01-01 00:00:00.000000 pyloobins-0.1.6/PKG-INFO
+-rw-r--r--   0        0        0    35149 2023-04-11 23:56:04.085551 pyloobins-0.1.7/LICENSE
+-rw-r--r--   0        0        0      885 2023-05-01 23:30:07.408912 pyloobins-0.1.7/LOOBins/GetFileInfo.yml
+-rw-r--r--   0        0        0     1412 2023-05-01 23:30:07.409275 pyloobins-0.1.7/LOOBins/SetFile.yml
+-rw-r--r--   0        0        0     1410 2023-05-17 23:34:53.847985 pyloobins-0.1.7/LOOBins/csrutil.yml
+-rw-r--r--   0        0        0     2449 2023-05-08 00:30:49.737329 pyloobins-0.1.7/LOOBins/ditto.yml
+-rw-r--r--   0        0        0     1644 2023-05-20 14:12:36.410173 pyloobins-0.1.7/LOOBins/dns-sd.yml
+-rw-r--r--   0        0        0     3545 2023-05-01 23:30:07.409751 pyloobins-0.1.7/LOOBins/dscl.yml
+-rw-r--r--   0        0        0     2138 2023-05-01 23:30:07.409978 pyloobins-0.1.7/LOOBins/ioreg.yml
+-rw-r--r--   0        0        0     1538 2023-05-01 01:46:27.775139 pyloobins-0.1.7/LOOBins/last.yml
+-rw-r--r--   0        0        0     1869 2023-05-17 23:34:53.848702 pyloobins-0.1.7/LOOBins/lsregister.yml
+-rw-r--r--   0        0        0     1763 2023-05-14 23:57:44.222650 pyloobins-0.1.7/LOOBins/mdfind.yml
+-rw-r--r--   0        0        0     4420 2023-05-01 23:30:07.410858 pyloobins-0.1.7/LOOBins/networksetup.yml
+-rw-r--r--   0        0        0      868 2023-05-15 00:11:31.657614 pyloobins-0.1.7/LOOBins/open.yml
+-rw-r--r--   0        0        0     1229 2023-05-15 23:03:47.041630 pyloobins-0.1.7/LOOBins/osacompile.yml
+-rw-r--r--   0        0        0     3237 2023-05-01 23:30:07.411097 pyloobins-0.1.7/LOOBins/osascript.yml
+-rw-r--r--   0        0        0     1263 2023-05-01 23:30:07.411462 pyloobins-0.1.7/LOOBins/pbpaste.yml
+-rw-r--r--   0        0        0     1259 2023-05-11 01:22:04.795362 pyloobins-0.1.7/LOOBins/plutil.yml
+-rw-r--r--   0        0        0     1249 2023-05-17 23:34:53.848926 pyloobins-0.1.7/LOOBins/profiles.yml
+-rw-r--r--   0        0        0     1051 2023-05-01 01:46:27.801548 pyloobins-0.1.7/LOOBins/screencapture.yml
+-rw-r--r--   0        0        0     2458 2023-05-01 01:46:27.474479 pyloobins-0.1.7/LOOBins/security.yml
+-rw-r--r--   0        0        0      840 2023-05-01 23:30:07.411670 pyloobins-0.1.7/LOOBins/softwareupdate.yml
+-rw-r--r--   0        0        0      790 2023-05-01 23:30:07.411980 pyloobins-0.1.7/LOOBins/sysctl.yml
+-rw-r--r--   0        0        0     1158 2023-05-18 14:49:43.472269 pyloobins-0.1.7/LOOBins/tclsh.yml
+-rw-r--r--   0        0        0     1993 2023-05-11 01:17:33.005665 pyloobins-0.1.7/LOOBins/textutil.yml
+-rw-r--r--   0        0        0     2034 2023-05-06 18:13:38.210711 pyloobins-0.1.7/LOOBins/tmutil.yml
+-rw-r--r--   0        0        0     1636 2023-04-23 17:34:43.219172 pyloobins-0.1.7/LOOBins/xattr.yml
+-rw-r--r--   0        0        0      972 2023-05-20 18:41:59.143590 pyloobins-0.1.7/docs/pyloobins/README.md
+-rw-r--r--   0        0        0     1227 2023-05-20 18:41:59.143868 pyloobins-0.1.7/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-04-07 02:06:55.452190 pyloobins-0.1.7/src/pyloobins/__init__.py
+-rw-r--r--   0        0        0     2182 2023-05-20 18:41:59.144041 pyloobins-0.1.7/src/pyloobins/cli.py
+-rw-r--r--   0        0        0     4015 2023-05-15 23:42:52.127853 pyloobins-0.1.7/src/pyloobins/models.py
+-rw-r--r--   0        0        0     1311 2023-05-01 23:30:07.412430 pyloobins-0.1.7/src/pyloobins/templates/loobin.md.j2
+-rw-r--r--   0        0        0     2761 2023-05-20 14:54:20.755132 pyloobins-0.1.7/src/pyloobins/util.py
+-rw-r--r--   0        0        0     1855 1970-01-01 00:00:00.000000 pyloobins-0.1.7/PKG-INFO
```

### Comparing `pyloobins-0.1.6/LICENSE` & `pyloobins-0.1.7/LICENSE`

 * *Files identical despite different names*

### Comparing `pyloobins-0.1.6/LOOBins/GetFileInfo.yml` & `pyloobins-0.1.7/LOOBins/GetFileInfo.yml`

 * *Files identical despite different names*

### Comparing `pyloobins-0.1.6/LOOBins/SetFile.yml` & `pyloobins-0.1.7/LOOBins/SetFile.yml`

 * *Files identical despite different names*

### Comparing `pyloobins-0.1.6/LOOBins/csrutil.yml` & `pyloobins-0.1.7/LOOBins/csrutil.yml`

 * *Files identical despite different names*

### Comparing `pyloobins-0.1.6/LOOBins/ditto.yml` & `pyloobins-0.1.7/LOOBins/ditto.yml`

 * *Files identical despite different names*

### Comparing `pyloobins-0.1.6/LOOBins/dns-sd.yml` & `pyloobins-0.1.7/LOOBins/dns-sd.yml`

 * *Files identical despite different names*

### Comparing `pyloobins-0.1.6/LOOBins/dscl.yml` & `pyloobins-0.1.7/LOOBins/dscl.yml`

 * *Files identical despite different names*

### Comparing `pyloobins-0.1.6/LOOBins/ioreg.yml` & `pyloobins-0.1.7/LOOBins/ioreg.yml`

 * *Files identical despite different names*

### Comparing `pyloobins-0.1.6/LOOBins/last.yml` & `pyloobins-0.1.7/LOOBins/last.yml`

 * *Files identical despite different names*

### Comparing `pyloobins-0.1.6/LOOBins/lsregister.yml` & `pyloobins-0.1.7/LOOBins/lsregister.yml`

 * *Files identical despite different names*

### Comparing `pyloobins-0.1.6/LOOBins/mdfind.yml` & `pyloobins-0.1.7/LOOBins/mdfind.yml`

 * *Files identical despite different names*

### Comparing `pyloobins-0.1.6/LOOBins/networksetup.yml` & `pyloobins-0.1.7/LOOBins/networksetup.yml`

 * *Files identical despite different names*

### Comparing `pyloobins-0.1.6/LOOBins/open.yml` & `pyloobins-0.1.7/LOOBins/open.yml`

 * *Files identical despite different names*

### Comparing `pyloobins-0.1.6/LOOBins/osacompile.yml` & `pyloobins-0.1.7/LOOBins/osacompile.yml`

 * *Files identical despite different names*

### Comparing `pyloobins-0.1.6/LOOBins/osascript.yml` & `pyloobins-0.1.7/LOOBins/osascript.yml`

 * *Files identical despite different names*

### Comparing `pyloobins-0.1.6/LOOBins/pbpaste.yml` & `pyloobins-0.1.7/LOOBins/pbpaste.yml`

 * *Files identical despite different names*

### Comparing `pyloobins-0.1.6/LOOBins/plutil.yml` & `pyloobins-0.1.7/LOOBins/plutil.yml`

 * *Files identical despite different names*

### Comparing `pyloobins-0.1.6/LOOBins/profiles.yml` & `pyloobins-0.1.7/LOOBins/profiles.yml`

 * *Files identical despite different names*

### Comparing `pyloobins-0.1.6/LOOBins/screencapture.yml` & `pyloobins-0.1.7/LOOBins/screencapture.yml`

 * *Files identical despite different names*

### Comparing `pyloobins-0.1.6/LOOBins/security.yml` & `pyloobins-0.1.7/LOOBins/security.yml`

 * *Files identical despite different names*

### Comparing `pyloobins-0.1.6/LOOBins/softwareupdate.yml` & `pyloobins-0.1.7/LOOBins/softwareupdate.yml`

 * *Files identical despite different names*

### Comparing `pyloobins-0.1.6/LOOBins/sysctl.yml` & `pyloobins-0.1.7/LOOBins/sysctl.yml`

 * *Files identical despite different names*

### Comparing `pyloobins-0.1.6/LOOBins/tclsh.yml` & `pyloobins-0.1.7/LOOBins/tclsh.yml`

 * *Files identical despite different names*

### Comparing `pyloobins-0.1.6/LOOBins/textutil.yml` & `pyloobins-0.1.7/LOOBins/textutil.yml`

 * *Files identical despite different names*

### Comparing `pyloobins-0.1.6/LOOBins/tmutil.yml` & `pyloobins-0.1.7/LOOBins/tmutil.yml`

 * *Files identical despite different names*

### Comparing `pyloobins-0.1.6/LOOBins/xattr.yml` & `pyloobins-0.1.7/LOOBins/xattr.yml`

 * *Files identical despite different names*

### Comparing `pyloobins-0.1.6/pyproject.toml` & `pyloobins-0.1.7/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 [tool.poetry]
 name = "PyLOOBins"
-version = "0.1.6"
+version = "0.1.7"
 description = "Python package for managing the LOOBins model and schema."
 authors = ["infosecB <brendan@infosecb.com>"]
-readme = "README.md"
+readme = "docs/pyloobins/README.md"
 packages = [{include = "pyloobins", from = "src"}]
 include = ["LOOBins/*.yml"]
 homepage = "https://loobins.io/"
 repository = "https://github.com/infosecB/LOOBins"
 keywords = ["cybersecurity", "cli", "lol"]
 license = "GPL-3.0-or-later"
```

### Comparing `pyloobins-0.1.6/src/pyloobins/cli.py` & `pyloobins-0.1.7/src/pyloobins/cli.py`

 * *Files 5% similar despite different names*

```diff
@@ -10,18 +10,18 @@
 @click.group()
 def cli():
     """Create, validate, and view LOOBin objects."""
 
 
 @cli.command()
 @click.option(
-    "--file",
+    "--path",
     type=str,
     required=True,
-    help="File location of the LOOBin YAML file to validate.",
+    help="The path of the LOOBin YAML file to validate.",
 )
 def validate(file: str) -> None:
     """Validate a LOOBin YAML file."""
     if validate_loobin(yml_path=file):
         print(f"LOOBin at {file} is valid.")
         sys.exit(0)
     else:
```

### Comparing `pyloobins-0.1.6/src/pyloobins/models.py` & `pyloobins-0.1.7/src/pyloobins/models.py`

 * *Files identical despite different names*

### Comparing `pyloobins-0.1.6/src/pyloobins/templates/loobin.md.j2` & `pyloobins-0.1.7/src/pyloobins/templates/loobin.md.j2`

 * *Files identical despite different names*

### Comparing `pyloobins-0.1.6/src/pyloobins/util.py` & `pyloobins-0.1.7/src/pyloobins/util.py`

 * *Files identical despite different names*

### Comparing `pyloobins-0.1.6/PKG-INFO` & `pyloobins-0.1.7/PKG-INFO`

 * *Files 26% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyloobins
-Version: 0.1.6
+Version: 0.1.7
 Summary: Python package for managing the LOOBins model and schema.
 Home-page: https://loobins.io/
 License: GPL-3.0-or-later
 Keywords: cybersecurity,cli,lol
 Author: infosecB
 Author-email: brendan@infosecb.com
 Requires-Python: >=3.8,<4.0
@@ -17,14 +17,48 @@
 Requires-Dist: click (>=8.1.3,<9.0.0)
 Requires-Dist: jinja2 (>=3.1.2,<4.0.0)
 Requires-Dist: pydantic (>=1.10.5,<2.0.0)
 Requires-Dist: pyyaml (>=6.0,<7.0)
 Project-URL: Repository, https://github.com/infosecB/LOOBins
 Description-Content-Type: text/markdown
 
-# LOOBins
-[https://loobins.io](https://loobins.io)
+# PyLOOBins
+PyLOOBins is a Python SDK and command-line utility for interacting with LOOBins.
 
-**L**iving **O**ff the **O**rchard: macOS Binaries (LOOBins) is designed to provide detailed information on various built-in macOS binaries and how they can be used by threat actors for malicious purposes. This list does not include overlapping Unix binaries that are detailed in [GTFOBins](https://gtfobins.github.io).
+You can download PyLOOBins from PyPI by running the following command:
+`pip install pyloobins`
 
-We are in active development and welcome contributions. Please see [our guidelines](https://github.com/infosecB/LOOBins/blob/main/CONTRIBUTING.md) if you are interesting in helping out!
+PyLOOBins requires Python 3.8 or later.
+
+## Usage
+### Command-line
+
+You can run `pyloobins --help` to see the available commands and options.
+
+```
+>>> pyloobins --help
+
+Usage: pyloobins [OPTIONS] COMMAND [ARGS]...
+
+  Create, validate, and view LOOBin objects.
+
+Options:
+  --help  Show this message and exit.
+
+Commands:
+  create    Create a YAML template file for a new LOOBin.
+  get       Get a LOOBin object.
+  validate  Validate a LOOBin YAML file.
+```
+
+You can run `pyloobins <command> --help` to see the available options for a specific command.
+```
+>>> pyloobins validate --help
+Usage: pyloobins validate [OPTIONS]
+
+  Validate a LOOBin YAML file.
+
+Options:
+  --path TEXT  The path of the LOOBin YAML file to validate.  [required]
+  --help       Show this message and exit.
+```
```

