# Comparing `tmp/veilcord-0.0.0.5.tar.gz` & `tmp/veilcord-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "veilcord-0.0.0.5.tar", last modified: Fri May 19 23:27:43 2023, max compression
+gzip compressed data, was "veilcord-0.0.2.tar", last modified: Sat May 20 22:11:22 2023, max compression
```

## Comparing `veilcord-0.0.0.5.tar` & `veilcord-0.0.2.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxrwx   0        0        0        0 2023-05-19 23:27:43.655725 veilcord-0.0.0.5/
--rw-rw-rw-   0        0        0     1085 2023-05-08 01:47:46.000000 veilcord-0.0.0.5/LICENSE
--rw-rw-rw-   0        0        0     1926 2023-05-19 23:27:43.655725 veilcord-0.0.0.5/PKG-INFO
--rw-rw-rw-   0        0        0      748 2023-05-17 01:51:11.000000 veilcord-0.0.0.5/README.md
--rw-rw-rw-   0        0        0       86 2023-05-08 02:01:12.000000 veilcord-0.0.0.5/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-05-19 23:27:43.655725 veilcord-0.0.0.5/setup.cfg
--rw-rw-rw-   0        0        0     1603 2023-05-19 23:27:09.000000 veilcord-0.0.0.5/setup.py
-drwxrwxrwx   0        0        0        0 2023-05-19 23:27:43.649379 veilcord-0.0.0.5/veilcord/
--rw-rw-rw-   0        0        0    13742 2023-05-19 23:27:30.000000 veilcord-0.0.0.5/veilcord/__init__.py
--rw-rw-rw-   0        0        0    10092 2023-05-19 23:26:56.000000 veilcord-0.0.0.5/veilcord/verification.py
-drwxrwxrwx   0        0        0        0 2023-05-19 23:27:43.654727 veilcord-0.0.0.5/veilcord.egg-info/
--rw-rw-rw-   0        0        0     1926 2023-05-19 23:27:43.000000 veilcord-0.0.0.5/veilcord.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      246 2023-05-19 23:27:43.000000 veilcord-0.0.0.5/veilcord.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-19 23:27:43.000000 veilcord-0.0.0.5/veilcord.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       38 2023-05-19 23:27:43.000000 veilcord-0.0.0.5/veilcord.egg-info/requires.txt
--rw-rw-rw-   0        0        0        9 2023-05-19 23:27:43.000000 veilcord-0.0.0.5/veilcord.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-05-20 22:11:22.905793 veilcord-0.0.2/
+-rw-rw-rw-   0        0        0     1085 2023-05-20 20:15:11.000000 veilcord-0.0.2/LICENSE
+-rw-rw-rw-   0        0        0     2826 2023-05-20 22:11:22.905793 veilcord-0.0.2/PKG-INFO
+-rw-rw-rw-   0        0        0     1598 2023-05-20 14:17:39.000000 veilcord-0.0.2/README.md
+-rw-rw-rw-   0        0        0       86 2023-05-08 02:01:12.000000 veilcord-0.0.2/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-05-20 22:11:22.905793 veilcord-0.0.2/setup.cfg
+-rw-rw-rw-   0        0        0     1753 2023-05-20 22:10:30.000000 veilcord-0.0.2/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-20 22:11:22.898575 veilcord-0.0.2/veilcord/
+-rw-rw-rw-   0        0        0     9187 2023-05-20 22:10:32.000000 veilcord-0.0.2/veilcord/__init__.py
+-rw-rw-rw-   0        0        0    13660 2023-05-20 22:05:34.000000 veilcord-0.0.2/veilcord/__main__.py
+drwxrwxrwx   0        0        0        0 2023-05-20 22:11:22.904796 veilcord-0.0.2/veilcord.egg-info/
+-rw-rw-rw-   0        0        0     2826 2023-05-20 22:11:22.000000 veilcord-0.0.2/veilcord.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      242 2023-05-20 22:11:22.000000 veilcord-0.0.2/veilcord.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-20 22:11:22.000000 veilcord-0.0.2/veilcord.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       95 2023-05-20 22:11:22.000000 veilcord-0.0.2/veilcord.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        9 2023-05-20 22:11:22.000000 veilcord-0.0.2/veilcord.egg-info/top_level.txt
```

### Comparing `veilcord-0.0.0.5/LICENSE` & `veilcord-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `veilcord-0.0.0.5/PKG-INFO` & `veilcord-0.0.2/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: veilcord
-Version: 0.0.0.5
+Version: 0.0.2
 Summary: VeilCord // vast#1337
 Home-page: http://pypi.python.org/pypi/veilcord
 Author: vast#1337
 Author-email: vastcord@proton.me
 License: MIT
 Project-URL: Homepage, https://github.com/imvast/veilcord
 Project-URL: Suggestions, https://github.com/imvast/veilcord/issues
@@ -13,45 +13,71 @@
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Natural Language :: English
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
 Classifier: Topic :: Scientific/Engineering
 Classifier: Topic :: Scientific/Engineering :: Information Analysis
 Classifier: Topic :: Scientific/Engineering :: Mathematics
 Classifier: Topic :: Scientific/Engineering :: Visualization
 Classifier: Topic :: Software Development :: Libraries
 Classifier: Topic :: Utilities
 Requires-Python: ~=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # VeilCord.
-<img src="https://img.shields.io/pypi/v/terminut?style=for-the-badge&logo=python">
+<img src="https://img.shields.io/pypi/v/veilcord?style=for-the-badge&logo=python">
 <img alt="followers" src="https://img.shields.io/github/followers/imvast?color=f429ff&style=for-the-badge&logo=github&label=Follow"/>
 
 ```less
               > Custom Discord Tools Going To Be Used For My Projects
                     And Available To Anyone Else Who Wants To Use <
 ```
 
 ---
 
 ### Installation
 ```yaml
 ! package NOT FULLY available for non-personal use !
 ```
 
-### Usage
+### Example Usage
 ```py
-# default shit if u want to only import for ease - auto switches #
+from veilcord import VeilCord
 
-import veilcord
+veilcord = VeilCord(
+    session = None, # for custom tls_client sessions
+    device_type = "browser", # types : browser, mobile, app
+    user_agent = None # for custom user agent
+)
+
+# GETTING X-Super-Properties
+xsup = veilcord.generateXProp()
+print(f"(+) Retrieved XSup: {xsup}")
+
+# GETTING ALL THE COOKIES AND FINGERPRINT
+cookies = veilcord.getFingerprint(xsup)
+print(f"(+) Retrieved Fingerprint: {cookies[0]}")
+# returns a set.  [0] - Fingerprint  |  [1] - COOKIESJAR
+
+
+# GET THE NEW SESSION ID BS
+token = ""
+sessionid = veilcord.getSession(
+      token = token, # obv the token 
+      type = 1, # type : 1 - web | 2 - app
+      keepAlive = False # keep the session alive | only needed if ur code is slow (avg. session is live for ~40 seconds.)
+)
+print(f"(+) Got Session ID: {sessionid}")
 
+# close the session, if keepAlive is enabled.
+# veilcord.closeSession(token)
 
 ```
 
 ---
 
-## * [vast#1337](https://discord.com/users/852976920148967485) | [imvast@github](https://github.com/imvast) | [vast.gay](https://vast.gay) *
+## * [vast#1337](https://discord.com/users/1109124745477246988) | [imvast@github](https://github.com/imvast) | [vast.gay](https://vast.gay) *
```

### Comparing `veilcord-0.0.0.5/setup.py` & `veilcord-0.0.2/setup.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 #! /usr/bin/env python
 
 from setuptools import setup, find_packages
 
-vers = "0.0.0.5"
+vers = "0.0.2"
     
 setup(name="veilcord",
       version=vers,
       description="VeilCord // vast#1337",
       long_description_content_type="text/markdown",
       long_description=open("README.md", encoding="utf-8").read(),
       packages=find_packages(exclude=['tests']),
@@ -20,14 +20,15 @@
           "License :: OSI Approved :: MIT License",
           "Natural Language :: English",
           "Programming Language :: Python",
           "Programming Language :: Python :: 3",
           "Programming Language :: Python :: 3.7",
           "Programming Language :: Python :: 3.8",
           "Programming Language :: Python :: 3.9",
+          "Programming Language :: Python :: 3.10",
           "Topic :: Scientific/Engineering",
           "Topic :: Scientific/Engineering :: Information Analysis",
           "Topic :: Scientific/Engineering :: Mathematics",
           "Topic :: Scientific/Engineering :: Visualization",
           "Topic :: Software Development :: Libraries",
           "Topic :: Utilities",
       ],
@@ -36,10 +37,13 @@
         'Suggestions': 'https://github.com/imvast/veilcord/issues',
       },
     
       python_requires="~=3.7",
 
       install_requires=[
           "terminut>=0.0.0.869",
-          "tls_client>=0.2.1"
+          "colorama>=0.4.6",
+          "requests>=2.30.0",
+          "tls_client>=0.2.1",
+          "websocket-client>=1.5.1"
       ]
 )
```

### Comparing `veilcord-0.0.0.5/veilcord.egg-info/PKG-INFO` & `veilcord-0.0.2/veilcord.egg-info/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: veilcord
-Version: 0.0.0.5
+Version: 0.0.2
 Summary: VeilCord // vast#1337
 Home-page: http://pypi.python.org/pypi/veilcord
 Author: vast#1337
 Author-email: vastcord@proton.me
 License: MIT
 Project-URL: Homepage, https://github.com/imvast/veilcord
 Project-URL: Suggestions, https://github.com/imvast/veilcord/issues
@@ -13,45 +13,71 @@
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Natural Language :: English
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
 Classifier: Topic :: Scientific/Engineering
 Classifier: Topic :: Scientific/Engineering :: Information Analysis
 Classifier: Topic :: Scientific/Engineering :: Mathematics
 Classifier: Topic :: Scientific/Engineering :: Visualization
 Classifier: Topic :: Software Development :: Libraries
 Classifier: Topic :: Utilities
 Requires-Python: ~=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # VeilCord.
-<img src="https://img.shields.io/pypi/v/terminut?style=for-the-badge&logo=python">
+<img src="https://img.shields.io/pypi/v/veilcord?style=for-the-badge&logo=python">
 <img alt="followers" src="https://img.shields.io/github/followers/imvast?color=f429ff&style=for-the-badge&logo=github&label=Follow"/>
 
 ```less
               > Custom Discord Tools Going To Be Used For My Projects
                     And Available To Anyone Else Who Wants To Use <
 ```
 
 ---
 
 ### Installation
 ```yaml
 ! package NOT FULLY available for non-personal use !
 ```
 
-### Usage
+### Example Usage
 ```py
-# default shit if u want to only import for ease - auto switches #
+from veilcord import VeilCord
 
-import veilcord
+veilcord = VeilCord(
+    session = None, # for custom tls_client sessions
+    device_type = "browser", # types : browser, mobile, app
+    user_agent = None # for custom user agent
+)
+
+# GETTING X-Super-Properties
+xsup = veilcord.generateXProp()
+print(f"(+) Retrieved XSup: {xsup}")
+
+# GETTING ALL THE COOKIES AND FINGERPRINT
+cookies = veilcord.getFingerprint(xsup)
+print(f"(+) Retrieved Fingerprint: {cookies[0]}")
+# returns a set.  [0] - Fingerprint  |  [1] - COOKIESJAR
+
+
+# GET THE NEW SESSION ID BS
+token = ""
+sessionid = veilcord.getSession(
+      token = token, # obv the token 
+      type = 1, # type : 1 - web | 2 - app
+      keepAlive = False # keep the session alive | only needed if ur code is slow (avg. session is live for ~40 seconds.)
+)
+print(f"(+) Got Session ID: {sessionid}")
 
+# close the session, if keepAlive is enabled.
+# veilcord.closeSession(token)
 
 ```
 
 ---
 
-## * [vast#1337](https://discord.com/users/852976920148967485) | [imvast@github](https://github.com/imvast) | [vast.gay](https://vast.gay) *
+## * [vast#1337](https://discord.com/users/1109124745477246988) | [imvast@github](https://github.com/imvast) | [vast.gay](https://vast.gay) *
```

