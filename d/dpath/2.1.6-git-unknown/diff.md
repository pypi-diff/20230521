# Comparing `tmp/dpath-2.1.6.tar.gz` & `tmp/dpath-git-unknown.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dpath-2.1.6.tar", last modified: Sun May 21 21:35:30 2023, max compression
+gzip compressed data, was "dist/dpath-git-unknown.tar", last modified: Sat Oct  5 11:55:20 2013, max compression
```

## Comparing `dpath-2.1.6.tar` & `dpath-git-unknown.tar`

### file list

```diff
@@ -1,36 +1,10 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 21:35:30.750834 dpath-2.1.6/
--rw-r--r--   0 runner    (1001) docker     (123)     1138 2023-05-21 21:35:24.000000 dpath-2.1.6/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (123)       83 2023-05-21 21:35:24.000000 dpath-2.1.6/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)    15654 2023-05-21 21:35:30.750834 dpath-2.1.6/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    14680 2023-05-21 21:35:24.000000 dpath-2.1.6/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 21:35:30.750834 dpath-2.1.6/dpath/
--rw-r--r--   0 runner    (1001) docker     (123)    12029 2023-05-21 21:35:24.000000 dpath-2.1.6/dpath/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      433 2023-05-21 21:35:24.000000 dpath-2.1.6/dpath/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)       32 2023-05-21 21:35:24.000000 dpath-2.1.6/dpath/options.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-21 21:35:24.000000 dpath-2.1.6/dpath/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    13241 2023-05-21 21:35:24.000000 dpath-2.1.6/dpath/segments.py
--rw-r--r--   0 runner    (1001) docker     (123)     2348 2023-05-21 21:35:24.000000 dpath-2.1.6/dpath/types.py
--rw-r--r--   0 runner    (1001) docker     (123)     1371 2023-05-21 21:35:24.000000 dpath-2.1.6/dpath/util.py
--rw-r--r--   0 runner    (1001) docker     (123)       18 2023-05-21 21:35:24.000000 dpath-2.1.6/dpath/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 21:35:30.750834 dpath-2.1.6/dpath.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    15654 2023-05-21 21:35:30.000000 dpath-2.1.6/dpath.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      596 2023-05-21 21:35:30.000000 dpath-2.1.6/dpath.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-21 21:35:30.000000 dpath-2.1.6/dpath.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-05-21 21:35:30.000000 dpath-2.1.6/dpath.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-21 21:35:30.750834 dpath-2.1.6/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2063 2023-05-21 21:35:24.000000 dpath-2.1.6/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 21:35:30.750834 dpath-2.1.6/tests/
--rw-r--r--   0 runner    (1001) docker     (123)       69 2023-05-21 21:35:24.000000 dpath-2.1.6/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1577 2023-05-21 21:35:24.000000 dpath-2.1.6/tests/test_broken_afilter.py
--rw-r--r--   0 runner    (1001) docker     (123)      947 2023-05-21 21:35:24.000000 dpath-2.1.6/tests/test_delete.py
--rw-r--r--   0 runner    (1001) docker     (123)     4937 2023-05-21 21:35:24.000000 dpath-2.1.6/tests/test_get_values.py
--rw-r--r--   0 runner    (1001) docker     (123)     4142 2023-05-21 21:35:24.000000 dpath-2.1.6/tests/test_merge.py
--rw-r--r--   0 runner    (1001) docker     (123)     2676 2023-05-21 21:35:24.000000 dpath-2.1.6/tests/test_new.py
--rw-r--r--   0 runner    (1001) docker     (123)      429 2023-05-21 21:35:24.000000 dpath-2.1.6/tests/test_path_get.py
--rw-r--r--   0 runner    (1001) docker     (123)      769 2023-05-21 21:35:24.000000 dpath-2.1.6/tests/test_path_paths.py
--rw-r--r--   0 runner    (1001) docker     (123)      203 2023-05-21 21:35:24.000000 dpath-2.1.6/tests/test_paths.py
--rw-r--r--   0 runner    (1001) docker     (123)     5589 2023-05-21 21:35:24.000000 dpath-2.1.6/tests/test_search.py
--rw-r--r--   0 runner    (1001) docker     (123)    10458 2023-05-21 21:35:24.000000 dpath-2.1.6/tests/test_segments.py
--rw-r--r--   0 runner    (1001) docker     (123)     1640 2023-05-21 21:35:24.000000 dpath-2.1.6/tests/test_set.py
--rw-r--r--   0 runner    (1001) docker     (123)     3515 2023-05-21 21:35:24.000000 dpath-2.1.6/tests/test_types.py
--rw-r--r--   0 runner    (1001) docker     (123)      686 2023-05-21 21:35:24.000000 dpath-2.1.6/tests/test_unicode.py
+drwxrwxr-x   0 bamboo    (1003) bamboo    (1003)        0 2013-10-05 11:55:20.000000 dpath-git-unknown/
+-rw-rw-r--   0 bamboo    (1003) bamboo    (1003)     8218 2013-10-05 11:55:15.000000 dpath-git-unknown/README
+-rw-rw-r--   0 bamboo    (1003) bamboo    (1003)     1860 2013-10-05 11:55:14.000000 dpath-git-unknown/setup.py
+-rw-rw-r--   0 bamboo    (1003) bamboo    (1003)     1605 2013-10-05 11:55:20.000000 dpath-git-unknown/PKG-INFO
+drwxrwxr-x   0 bamboo    (1003) bamboo    (1003)        0 2013-10-05 11:55:20.000000 dpath-git-unknown/dpath/
+-rw-rw-r--   0 bamboo    (1003) bamboo    (1003)      430 2013-10-05 11:55:14.000000 dpath-git-unknown/dpath/exceptions.py
+-rw-rw-r--   0 bamboo    (1003) bamboo    (1003)       66 2013-10-05 11:55:14.000000 dpath-git-unknown/dpath/version.py
+-rw-rw-r--   0 bamboo    (1003) bamboo    (1003)     6350 2013-10-05 11:55:14.000000 dpath-git-unknown/dpath/util.py
+-rw-rw-r--   0 bamboo    (1003) bamboo    (1003)     8732 2013-10-05 11:55:14.000000 dpath-git-unknown/dpath/path.py
+-rw-rw-r--   0 bamboo    (1003) bamboo    (1003)        0 2013-10-05 11:55:14.000000 dpath-git-unknown/dpath/__init__.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive
+POSIX tar archive (GNU)
```

### Comparing `dpath-2.1.6/setup.py` & `dpath-git-unknown/setup.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,55 +1,43 @@
-import os
-from setuptools import setup
-
+from distutils.core import setup
 import dpath.version
-
-long_description = open(
-    os.path.join(
-        os.path.dirname(__file__),
-        'README.rst'
-    )
-).read()
+import os
+import sys
 
 if __name__ == "__main__":
     setup(
         name="dpath",
-        url="https://github.com/dpath-maintainers/dpath-python",
+        url="https://www.github.com/akesterson/dpath-python",
         version=dpath.version.VERSION,
         description="Filesystem-like pathing and searching for dictionaries",
-        long_description=long_description,
+        long_description="""
+DPath is a library that allows you to access dictionaries similar to using find over a filesystem. The proper documentation is maintained on GitHub: https://github.com/akesterson/dpath-python
+
+Version 1.2 introduces a number of fixes against 1.1:
+
+    * List handling has been completely redone. Various builds of 1.1 had fundamentally broken list handling. 1.2 handles list insertions, deletions, and searches as expected.
+
+    * The backend path library has been improved to include type information with each path component, so the issue of lists mysteriously being transformed into dictionaries will no longer happen
+
+    * The merge function's filtering has been fixed; before, it was broken, as directory nodes were merged in before filtering leaf nodes, making the filters essentially useless.
+
+    * The unit test suite has been expanded.
+""",
         author=("Caleb Case, "
                 "Andrew Kesterson"),
         author_email="calebcase@gmail.com, andrew@aklabs.net",
         license="MIT",
         install_requires=[],
         scripts=[],
         packages=["dpath"],
         data_files=[],
-        package_data={"dpath": ["py.typed"]},
-
-        # Type hints are great.
-        # Function annotations were added in Python 3.0.
-        # Typing module was added in Python 3.5.
-        # Variable annotations were added in Python 3.6.
-        # Python versions that are >=3.6 are more popular.
-        #   (Source: https://github.com/hugovk/pypi-tools/blob/master/README.md)
-        #
-        # Conclusion: In order to accommodate type hinting support must be limited to Python versions >=3.6.
-        # 3.6 was dropped because of EOL and this issue: https://github.com/actions/setup-python/issues/544
-        python_requires=">=3.7",
         classifiers=[
             'Development Status :: 5 - Production/Stable',
             'Environment :: Console',
             'Intended Audience :: Developers',
             'License :: OSI Approved :: MIT License',
             'Natural Language :: English',
-            'Programming Language :: Python :: 3',
-            'Programming Language :: Python :: 3.7',
-            'Programming Language :: Python :: 3.8',
-            'Programming Language :: Python :: 3.9',
-            'Programming Language :: Python :: 3.10',
-            'Programming Language :: Python :: 3.11',
+            'Programming Language :: Python :: 2.7',
             'Topic :: Software Development :: Libraries :: Python Modules',
-            'Typing :: Typed',
         ],
     )
+
```

