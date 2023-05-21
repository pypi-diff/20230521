# Comparing `tmp/copyright_claim-0.0.4.tar.gz` & `tmp/copyright_claim-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "copyright_claim-0.0.4.tar", max compression
+gzip compressed data, was "copyright_claim-0.0.5.tar", max compression
```

## Comparing `copyright_claim-0.0.4.tar` & `copyright_claim-0.0.5.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rw-r--r--   0        0        0     3758 2023-05-19 18:33:40.377872 copyright_claim-0.0.4/README.md
--rw-r--r--   0        0        0      114 2023-05-18 22:59:56.420566 copyright_claim-0.0.4/copyright_claim/__init__.py
--rw-r--r--   0        0        0     8128 2023-05-19 17:36:55.654300 copyright_claim-0.0.4/copyright_claim/copyright_claim.py
--rw-r--r--   0        0        0      311 2023-05-19 15:15:17.230093 copyright_claim-0.0.4/copyright_claim/dummy_copyright_claim.txt
--rw-r--r--   0        0        0      535 2023-05-19 18:34:02.713896 copyright_claim-0.0.4/pyproject.toml
--rw-r--r--   0        0        0     4397 1970-01-01 00:00:00.000000 copyright_claim-0.0.4/PKG-INFO
+-rw-r--r--   0        0        0     3758 2023-05-19 18:33:40.377872 copyright_claim-0.0.5/README.md
+-rw-r--r--   0        0        0      114 2023-05-18 22:59:56.420566 copyright_claim-0.0.5/copyright_claim/__init__.py
+-rw-r--r--   0        0        0     8122 2023-05-21 08:14:47.168155 copyright_claim-0.0.5/copyright_claim/copyright_claim.py
+-rw-r--r--   0        0        0      311 2023-05-19 15:15:17.230093 copyright_claim-0.0.5/copyright_claim/dummy_copyright_claim.txt
+-rw-r--r--   0        0        0      535 2023-05-21 08:24:48.158502 copyright_claim-0.0.5/pyproject.toml
+-rw-r--r--   0        0        0     4397 1970-01-01 00:00:00.000000 copyright_claim-0.0.5/PKG-INFO
```

### Comparing `copyright_claim-0.0.4/README.md` & `copyright_claim-0.0.5/README.md`

 * *Files identical despite different names*

### Comparing `copyright_claim-0.0.4/copyright_claim/copyright_claim.py` & `copyright_claim-0.0.5/copyright_claim/copyright_claim.py`

 * *Files 2% similar despite different names*

```diff
@@ -49,15 +49,15 @@
 
     Args:
         file_path (str): The path to the file to be treated.
         claim_path (str): The path to a file containing the claim text
             string.
         start_string (str, optional): A string to mark the beginning of
             the copyright claim block. Defaults to "COPYRIGHT CLAIM".
-        end_string (str, optional): A string to mark the beginning of
+        end_string (str, optional): A string to mark the end of
             the copyright claim block. Defaults to "END OF COPYRIGHT
             CLAIM".
         comment_symbol (str, optional): The symbol that marks comment
             lines in the treated files. Defaults to "# ".
     """
 
     with open(claim_path, "r") as claim_file:
@@ -133,15 +133,15 @@
     print(pkgutil.get_data(__name__, "dummy_copyright_claim.txt").decode())
 
 
 def main():
     "Wraps everything to form a terminal command."
     # Argument parsing.
     parser = argparse.ArgumentParser(
-        prog="copyright_claim",
+        prog="copyright-claim",
         description="Adds and removes copyright claims at the beginning of text files.",
     )
     parser.add_argument(
         "mode",
         choices=["add", "remove", "dummy"],
         help='Choose "add" if you want to add the claim, "remove" if you '
         + 'want to remove it. The "dummy" option simply outputs our dummy '
```

### Comparing `copyright_claim-0.0.4/pyproject.toml` & `copyright_claim-0.0.5/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "copyright-claim"
-version = "0.0.4"
+version = "0.0.5"
 description = "Adds and removes copyright claims at the beginning of text files."
 authors = ["Gaël Cousin <gcousin333@gmail.com>"]
 license = "BSD-2-Clause License"
 readme = "README.md"
 packages = [{include = "copyright_claim"}]
 
 [tool.poetry.dependencies]
```

### Comparing `copyright_claim-0.0.4/PKG-INFO` & `copyright_claim-0.0.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: copyright-claim
-Version: 0.0.4
+Version: 0.0.5
 Summary: Adds and removes copyright claims at the beginning of text files.
 License: BSD-2-Clause License
 Author: Gaël Cousin
 Author-email: gcousin333@gmail.com
 Requires-Python: >=3.7,<4.0
 Classifier: License :: Other/Proprietary License
 Classifier: Programming Language :: Python :: 3
```

