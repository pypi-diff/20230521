# Comparing `tmp/mcmc_statphys-0.4.2.tar.gz` & `tmp/mcmc_statphys-0.4.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mcmc_statphys-0.4.2.tar", last modified: Sun May 21 04:42:21 2023, max compression
+gzip compressed data, was "mcmc_statphys-0.4.3.tar", last modified: Sun May 21 09:27:48 2023, max compression
```

## Comparing `mcmc_statphys-0.4.2.tar` & `mcmc_statphys-0.4.3.tar`

### file list

```diff
@@ -1,50 +1,50 @@
-drwxrwxrwx   0        0        0        0 2023-05-21 04:42:21.069191 mcmc_statphys-0.4.2/
--rw-rw-rw-   0        0        0      170 2023-05-14 13:37:58.000000 mcmc_statphys-0.4.2/AUTHORS.rst
--rw-rw-rw-   0        0        0     3726 2023-05-18 15:41:51.000000 mcmc_statphys-0.4.2/CONTRIBUTING.rst
--rw-rw-rw-   0        0        0     1592 2023-05-21 04:30:43.000000 mcmc_statphys-0.4.2/HISTORY.rst
--rw-rw-rw-   0        0        0     1089 2023-05-14 13:37:58.000000 mcmc_statphys-0.4.2/LICENSE
--rw-rw-rw-   0        0        0      273 2023-05-14 13:37:58.000000 mcmc_statphys-0.4.2/MANIFEST.in
--rw-rw-rw-   0        0        0     4623 2023-05-21 04:42:21.070186 mcmc_statphys-0.4.2/PKG-INFO
--rw-rw-rw-   0        0        0     2193 2023-05-18 15:41:51.000000 mcmc_statphys-0.4.2/README.rst
-drwxrwxrwx   0        0        0        0 2023-05-21 04:42:20.783689 mcmc_statphys-0.4.2/docs/
--rw-rw-rw-   0        0        0      634 2023-05-14 13:37:58.000000 mcmc_statphys-0.4.2/docs/Makefile
--rw-rw-rw-   0        0        0       29 2023-05-14 13:37:58.000000 mcmc_statphys-0.4.2/docs/authors.rst
--rw-rw-rw-   0        0        0     4923 2023-05-21 04:30:43.000000 mcmc_statphys-0.4.2/docs/conf.py
--rw-rw-rw-   0        0        0       34 2023-05-14 13:37:58.000000 mcmc_statphys-0.4.2/docs/contributing.rst
--rw-rw-rw-   0        0        0       29 2023-05-14 13:37:58.000000 mcmc_statphys-0.4.2/docs/history.rst
-drwxrwxrwx   0        0        0        0 2023-05-21 04:42:20.786682 mcmc_statphys-0.4.2/docs/img/
--rw-rw-rw-   0        0        0    12977 2023-05-17 14:16:19.000000 mcmc_statphys-0.4.2/docs/img/energy-73cbe80ef4b811ed9b0400e04c6807cc.png
--rw-rw-rw-   0        0        0      333 2023-05-16 16:00:10.000000 mcmc_statphys-0.4.2/docs/index.rst
--rw-rw-rw-   0        0        0     1209 2023-05-14 13:37:58.000000 mcmc_statphys-0.4.2/docs/installation.rst
--rwxrwxrwx   0        0        0      811 2023-05-14 13:37:58.000000 mcmc_statphys-0.4.2/docs/make.bat
--rw-rw-rw-   0        0        0    10277 2023-05-21 04:30:43.000000 mcmc_statphys-0.4.2/docs/modules.rst
--rw-rw-rw-   0        0        0       28 2023-05-14 13:37:58.000000 mcmc_statphys-0.4.2/docs/readme.rst
--rw-rw-rw-   0        0        0    17406 2023-05-21 04:30:43.000000 mcmc_statphys-0.4.2/docs/usage.rst
-drwxrwxrwx   0        0        0        0 2023-05-21 04:42:20.820930 mcmc_statphys-0.4.2/mcmc_statphys/
--rw-rw-rw-   0        0        0      247 2023-05-21 04:30:43.000000 mcmc_statphys-0.4.2/mcmc_statphys/__init__.py
--rw-rw-rw-   0        0        0    14945 2023-05-21 04:30:43.000000 mcmc_statphys-0.4.2/mcmc_statphys/algorithm.py
--rw-rw-rw-   0        0        0     2582 2023-05-20 10:32:21.000000 mcmc_statphys-0.4.2/mcmc_statphys/analysis.py
--rw-rw-rw-   0        0        0      434 2023-05-14 12:02:25.000000 mcmc_statphys-0.4.2/mcmc_statphys/cli.py
--rw-rw-rw-   0        0        0     5788 2023-05-21 04:30:43.000000 mcmc_statphys-0.4.2/mcmc_statphys/draw.py
--rw-rw-rw-   0        0        0     8776 2023-05-21 04:30:43.000000 mcmc_statphys-0.4.2/mcmc_statphys/model.py
-drwxrwxrwx   0        0        0        0 2023-05-21 04:42:20.934555 mcmc_statphys-0.4.2/mcmc_statphys.egg-info/
--rw-rw-rw-   0        0        0     4623 2023-05-21 04:42:20.000000 mcmc_statphys-0.4.2/mcmc_statphys.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      914 2023-05-21 04:42:20.000000 mcmc_statphys-0.4.2/mcmc_statphys.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-21 04:42:20.000000 mcmc_statphys-0.4.2/mcmc_statphys.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       57 2023-05-21 04:42:20.000000 mcmc_statphys-0.4.2/mcmc_statphys.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0        2 2023-05-14 13:46:13.000000 mcmc_statphys-0.4.2/mcmc_statphys.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0       11 2023-05-21 04:42:20.000000 mcmc_statphys-0.4.2/mcmc_statphys.egg-info/requires.txt
--rw-rw-rw-   0        0        0       14 2023-05-21 04:42:20.000000 mcmc_statphys-0.4.2/mcmc_statphys.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      520 2023-05-21 04:42:21.077172 mcmc_statphys-0.4.2/setup.cfg
--rw-rw-rw-   0        0        0     1556 2023-05-21 04:30:43.000000 mcmc_statphys-0.4.2/setup.py
-drwxrwxrwx   0        0        0        0 2023-05-21 04:42:20.968465 mcmc_statphys-0.4.2/tests/
--rw-rw-rw-   0        0        0       44 2023-05-14 13:37:58.000000 mcmc_statphys-0.4.2/tests/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-21 04:42:21.067194 mcmc_statphys-0.4.2/tests/one/
--rw-rw-rw-   0        0        0      229 2023-05-21 04:30:43.000000 mcmc_statphys-0.4.2/tests/one/__init__.py
--rw-rw-rw-   0        0        0    14945 2023-05-21 04:30:43.000000 mcmc_statphys-0.4.2/tests/one/algorithm.py
--rw-rw-rw-   0        0        0     1406 2023-05-21 04:30:43.000000 mcmc_statphys-0.4.2/tests/one/analysis.py
--rw-rw-rw-   0        0        0      434 2023-05-21 04:30:43.000000 mcmc_statphys-0.4.2/tests/one/cli.py
--rw-rw-rw-   0        0        0     5788 2023-05-21 04:30:43.000000 mcmc_statphys-0.4.2/tests/one/draw.py
--rw-rw-rw-   0        0        0     8776 2023-05-21 04:30:43.000000 mcmc_statphys-0.4.2/tests/one/model.py
--rw-rw-rw-   0        0        0     2891 2023-05-21 04:30:43.000000 mcmc_statphys-0.4.2/tests/test.ipynb
--rw-rw-rw-   0        0        0      952 2023-05-18 15:41:51.000000 mcmc_statphys-0.4.2/tests/test_mcmc_statphys.py
+drwxrwxrwx   0        0        0        0 2023-05-21 09:27:48.245245 mcmc_statphys-0.4.3/
+-rw-rw-rw-   0        0        0      170 2023-05-14 13:37:58.000000 mcmc_statphys-0.4.3/AUTHORS.rst
+-rw-rw-rw-   0        0        0     3726 2023-05-18 15:41:51.000000 mcmc_statphys-0.4.3/CONTRIBUTING.rst
+-rw-rw-rw-   0        0        0     1592 2023-05-21 04:30:43.000000 mcmc_statphys-0.4.3/HISTORY.rst
+-rw-rw-rw-   0        0        0     1089 2023-05-14 13:37:58.000000 mcmc_statphys-0.4.3/LICENSE
+-rw-rw-rw-   0        0        0      273 2023-05-14 13:37:58.000000 mcmc_statphys-0.4.3/MANIFEST.in
+-rw-rw-rw-   0        0        0     4623 2023-05-21 09:27:48.245245 mcmc_statphys-0.4.3/PKG-INFO
+-rw-rw-rw-   0        0        0     2193 2023-05-18 15:41:51.000000 mcmc_statphys-0.4.3/README.rst
+drwxrwxrwx   0        0        0        0 2023-05-21 09:27:48.150984 mcmc_statphys-0.4.3/docs/
+-rw-rw-rw-   0        0        0      634 2023-05-14 13:37:58.000000 mcmc_statphys-0.4.3/docs/Makefile
+-rw-rw-rw-   0        0        0       29 2023-05-14 13:37:58.000000 mcmc_statphys-0.4.3/docs/authors.rst
+-rw-rw-rw-   0        0        0     4923 2023-05-21 09:26:39.000000 mcmc_statphys-0.4.3/docs/conf.py
+-rw-rw-rw-   0        0        0       34 2023-05-14 13:37:58.000000 mcmc_statphys-0.4.3/docs/contributing.rst
+-rw-rw-rw-   0        0        0       29 2023-05-14 13:37:58.000000 mcmc_statphys-0.4.3/docs/history.rst
+drwxrwxrwx   0        0        0        0 2023-05-21 09:27:48.152979 mcmc_statphys-0.4.3/docs/img/
+-rw-rw-rw-   0        0        0    12977 2023-05-17 14:16:19.000000 mcmc_statphys-0.4.3/docs/img/energy-73cbe80ef4b811ed9b0400e04c6807cc.png
+-rw-rw-rw-   0        0        0      333 2023-05-16 16:00:10.000000 mcmc_statphys-0.4.3/docs/index.rst
+-rw-rw-rw-   0        0        0     1209 2023-05-14 13:37:58.000000 mcmc_statphys-0.4.3/docs/installation.rst
+-rwxrwxrwx   0        0        0      811 2023-05-14 13:37:58.000000 mcmc_statphys-0.4.3/docs/make.bat
+-rw-rw-rw-   0        0        0    10277 2023-05-21 04:30:43.000000 mcmc_statphys-0.4.3/docs/modules.rst
+-rw-rw-rw-   0        0        0       28 2023-05-14 13:37:58.000000 mcmc_statphys-0.4.3/docs/readme.rst
+-rw-rw-rw-   0        0        0    17406 2023-05-21 04:30:43.000000 mcmc_statphys-0.4.3/docs/usage.rst
+drwxrwxrwx   0        0        0        0 2023-05-21 09:27:48.167939 mcmc_statphys-0.4.3/mcmc_statphys/
+-rw-rw-rw-   0        0        0      247 2023-05-21 09:26:39.000000 mcmc_statphys-0.4.3/mcmc_statphys/__init__.py
+-rw-rw-rw-   0        0        0    14689 2023-05-21 09:26:19.000000 mcmc_statphys-0.4.3/mcmc_statphys/algorithm.py
+-rw-rw-rw-   0        0        0     2582 2023-05-20 10:32:21.000000 mcmc_statphys-0.4.3/mcmc_statphys/analysis.py
+-rw-rw-rw-   0        0        0      434 2023-05-14 12:02:25.000000 mcmc_statphys-0.4.3/mcmc_statphys/cli.py
+-rw-rw-rw-   0        0        0     5788 2023-05-21 04:30:43.000000 mcmc_statphys-0.4.3/mcmc_statphys/draw.py
+-rw-rw-rw-   0        0        0     8776 2023-05-21 04:30:43.000000 mcmc_statphys-0.4.3/mcmc_statphys/model.py
+drwxrwxrwx   0        0        0        0 2023-05-21 09:27:48.211822 mcmc_statphys-0.4.3/mcmc_statphys.egg-info/
+-rw-rw-rw-   0        0        0     4623 2023-05-21 09:27:47.000000 mcmc_statphys-0.4.3/mcmc_statphys.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      914 2023-05-21 09:27:48.000000 mcmc_statphys-0.4.3/mcmc_statphys.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-21 09:27:47.000000 mcmc_statphys-0.4.3/mcmc_statphys.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       57 2023-05-21 09:27:47.000000 mcmc_statphys-0.4.3/mcmc_statphys.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0        2 2023-05-14 13:46:13.000000 mcmc_statphys-0.4.3/mcmc_statphys.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0       11 2023-05-21 09:27:47.000000 mcmc_statphys-0.4.3/mcmc_statphys.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       14 2023-05-21 09:27:47.000000 mcmc_statphys-0.4.3/mcmc_statphys.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      520 2023-05-21 09:27:48.249237 mcmc_statphys-0.4.3/setup.cfg
+-rw-rw-rw-   0        0        0     1556 2023-05-21 09:26:39.000000 mcmc_statphys-0.4.3/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-21 09:27:48.228776 mcmc_statphys-0.4.3/tests/
+-rw-rw-rw-   0        0        0       44 2023-05-14 13:37:58.000000 mcmc_statphys-0.4.3/tests/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-21 09:27:48.243250 mcmc_statphys-0.4.3/tests/one/
+-rw-rw-rw-   0        0        0      229 2023-05-21 04:30:43.000000 mcmc_statphys-0.4.3/tests/one/__init__.py
+-rw-rw-rw-   0        0        0    14945 2023-05-21 04:30:43.000000 mcmc_statphys-0.4.3/tests/one/algorithm.py
+-rw-rw-rw-   0        0        0     1406 2023-05-21 04:30:43.000000 mcmc_statphys-0.4.3/tests/one/analysis.py
+-rw-rw-rw-   0        0        0      434 2023-05-21 04:30:43.000000 mcmc_statphys-0.4.3/tests/one/cli.py
+-rw-rw-rw-   0        0        0     5788 2023-05-21 04:30:43.000000 mcmc_statphys-0.4.3/tests/one/draw.py
+-rw-rw-rw-   0        0        0     8776 2023-05-21 04:30:43.000000 mcmc_statphys-0.4.3/tests/one/model.py
+-rw-rw-rw-   0        0        0     2891 2023-05-21 04:30:43.000000 mcmc_statphys-0.4.3/tests/test.ipynb
+-rw-rw-rw-   0        0        0      952 2023-05-18 15:41:51.000000 mcmc_statphys-0.4.3/tests/test_mcmc_statphys.py
```

### Comparing `mcmc_statphys-0.4.2/CONTRIBUTING.rst` & `mcmc_statphys-0.4.3/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `mcmc_statphys-0.4.2/HISTORY.rst` & `mcmc_statphys-0.4.3/HISTORY.rst`

 * *Files identical despite different names*

### Comparing `mcmc_statphys-0.4.2/LICENSE` & `mcmc_statphys-0.4.3/LICENSE`

 * *Files identical despite different names*

### Comparing `mcmc_statphys-0.4.2/PKG-INFO` & `mcmc_statphys-0.4.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mcmc_statphys
-Version: 0.4.2
+Version: 0.4.3
 Summary: A library project of Monte Carlo simulation algorithms for some statistical physics models (in particular, the Ising model and its variants).
 Home-page: https://github.com/uynajgi/mcmc_statphys
 Author: Uynaj GI
 Author-email: suquan12148@outlook.com
 License: MIT license
 Keywords: mcmc_statphys
 Classifier: Development Status :: 2 - Pre-Alpha
```

### Comparing `mcmc_statphys-0.4.2/README.rst` & `mcmc_statphys-0.4.3/README.rst`

 * *Files identical despite different names*

### Comparing `mcmc_statphys-0.4.2/docs/Makefile` & `mcmc_statphys-0.4.3/docs/Makefile`

 * *Files identical despite different names*

### Comparing `mcmc_statphys-0.4.2/docs/conf.py` & `mcmc_statphys-0.4.3/docs/conf.py`

 * *Files 0% similar despite different names*

```diff
@@ -52,15 +52,15 @@
 author = "Uynaj GI"
 
 # The version info for the project you're documenting, acts as replacement
 # for |version| and |release|, also used in various other places throughout
 # the built documents.
 #
 # The short X.Y version.
-version = '0.4.2'
+version = '0.4.3'
 # The full version, including alpha/beta/rc tags.
 release = version
 
 # The language for content autogenerated by Sphinx. Refer to documentation
 # for a list of supported languages.
 #
 # This is also used if you do content translation via gettext catalogs.
```

### Comparing `mcmc_statphys-0.4.2/docs/img/energy-73cbe80ef4b811ed9b0400e04c6807cc.png` & `mcmc_statphys-0.4.3/docs/img/energy-73cbe80ef4b811ed9b0400e04c6807cc.png`

 * *Files identical despite different names*

### Comparing `mcmc_statphys-0.4.2/docs/installation.rst` & `mcmc_statphys-0.4.3/docs/installation.rst`

 * *Files identical despite different names*

### Comparing `mcmc_statphys-0.4.2/docs/make.bat` & `mcmc_statphys-0.4.3/docs/make.bat`

 * *Files identical despite different names*

### Comparing `mcmc_statphys-0.4.2/docs/modules.rst` & `mcmc_statphys-0.4.3/docs/modules.rst`

 * *Files identical despite different names*

### Comparing `mcmc_statphys-0.4.2/docs/usage.rst` & `mcmc_statphys-0.4.3/docs/usage.rst`

 * *Files identical despite different names*

### Comparing `mcmc_statphys-0.4.2/mcmc_statphys/algorithm.py` & `mcmc_statphys-0.4.3/tests/one/algorithm.py`

 * *Files identical despite different names*

### Comparing `mcmc_statphys-0.4.2/mcmc_statphys/analysis.py` & `mcmc_statphys-0.4.3/mcmc_statphys/analysis.py`

 * *Files identical despite different names*

### Comparing `mcmc_statphys-0.4.2/mcmc_statphys/draw.py` & `mcmc_statphys-0.4.3/mcmc_statphys/draw.py`

 * *Files identical despite different names*

### Comparing `mcmc_statphys-0.4.2/mcmc_statphys/model.py` & `mcmc_statphys-0.4.3/mcmc_statphys/model.py`

 * *Files identical despite different names*

### Comparing `mcmc_statphys-0.4.2/mcmc_statphys.egg-info/PKG-INFO` & `mcmc_statphys-0.4.3/mcmc_statphys.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mcmc-statphys
-Version: 0.4.2
+Version: 0.4.3
 Summary: A library project of Monte Carlo simulation algorithms for some statistical physics models (in particular, the Ising model and its variants).
 Home-page: https://github.com/uynajgi/mcmc_statphys
 Author: Uynaj GI
 Author-email: suquan12148@outlook.com
 License: MIT license
 Keywords: mcmc_statphys
 Classifier: Development Status :: 2 - Pre-Alpha
```

### Comparing `mcmc_statphys-0.4.2/mcmc_statphys.egg-info/SOURCES.txt` & `mcmc_statphys-0.4.3/mcmc_statphys.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mcmc_statphys-0.4.2/setup.cfg` & `mcmc_statphys-0.4.3/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 [bumpversion]
-current_version = 0.4.2
+current_version = 0.4.3
 commit = True
 tag = True
 
 [bumpversion:file:setup.py]
 search = version='{current_version}'
 replace = version='{new_version}'
```

### Comparing `mcmc_statphys-0.4.2/setup.py` & `mcmc_statphys-0.4.3/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -40,10 +40,10 @@
     include_package_data=True,
     keywords='mcmc_statphys',
     name='mcmc_statphys',
     packages=find_packages(include=['mcmc_statphys', 'mcmc_statphys.*']),
     test_suite='tests',
     tests_require=test_requirements,
     url='https://github.com/uynajgi/mcmc_statphys',
-    version='0.4.2',
+    version='0.4.3',
     zip_safe=False,
 )
```

### Comparing `mcmc_statphys-0.4.2/tests/one/algorithm.py` & `mcmc_statphys-0.4.3/mcmc_statphys/algorithm.py`

 * *Files 3% similar despite different names*

```diff
@@ -314,16 +314,14 @@
             if self.parameter == "T":
                 if self.model.type == "ising" or self.model.type == "potts":
                     self.model.H = self.H0
                 self.equil_sample(param, max_iter=max_iter, uid=uid)
             elif self.parameter == "H":
                 self.model.H = param
                 self.equil_sample(self.T0, max_iter=max_iter, uid=uid)
-            param_lst.set_description("{parameter} = {param}".format(
-                parameter=self.parameter, param=param))
         uid_param_dict: Dict = {
             "uid": uid_lst,
             "{param}".format(param=self.parameter): param_lst,
         }
         return uid_param_dict
 
 
@@ -395,14 +393,12 @@
             if self.parameter == "T":
                 if self.model.type == "ising" or self.model.type == "potts":
                     self.model.H = self.H0
                 self.equil_sample(param, max_iter=max_iter, uid=uid)
             elif self.parameter == "H":
                 self.model.H = param
                 self.equil_sample(self.T0, max_iter=max_iter, uid=uid)
-            param_lst.set_description("{parameter} = {param}".format(
-                parameter=self.parameter, param=param))
         uid_param_dict: Dict = {
             "uid": uid_lst,
             "{param}".format(param=self.parameter): param_lst,
         }
         return uid_param_dict
```

### Comparing `mcmc_statphys-0.4.2/tests/one/analysis.py` & `mcmc_statphys-0.4.3/tests/one/analysis.py`

 * *Files identical despite different names*

### Comparing `mcmc_statphys-0.4.2/tests/one/draw.py` & `mcmc_statphys-0.4.3/tests/one/draw.py`

 * *Files identical despite different names*

### Comparing `mcmc_statphys-0.4.2/tests/one/model.py` & `mcmc_statphys-0.4.3/tests/one/model.py`

 * *Files identical despite different names*

### Comparing `mcmc_statphys-0.4.2/tests/test.ipynb` & `mcmc_statphys-0.4.3/tests/test.ipynb`

 * *Files identical despite different names*

### Comparing `mcmc_statphys-0.4.2/tests/test_mcmc_statphys.py` & `mcmc_statphys-0.4.3/tests/test_mcmc_statphys.py`

 * *Files identical despite different names*

