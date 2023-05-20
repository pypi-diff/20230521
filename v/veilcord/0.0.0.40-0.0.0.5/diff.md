# Comparing `tmp/veilcord-0.0.0.40.tar.gz` & `tmp/veilcord-0.0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "veilcord-0.0.0.40.tar", last modified: Sat May 20 14:15:23 2023, max compression
+gzip compressed data, was "veilcord-0.0.0.5.tar", last modified: Fri May 19 23:27:43 2023, max compression
```

## Comparing `veilcord-0.0.0.40.tar` & `veilcord-0.0.0.5.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxrwx   0        0        0        0 2023-05-20 14:15:23.028887 veilcord-0.0.0.40/
--rw-rw-rw-   0        0        0     1085 2023-05-08 01:47:46.000000 veilcord-0.0.0.40/LICENSE
--rw-rw-rw-   0        0        0     2777 2023-05-20 14:15:23.028887 veilcord-0.0.0.40/PKG-INFO
--rw-rw-rw-   0        0        0     1598 2023-05-20 13:55:32.000000 veilcord-0.0.0.40/README.md
--rw-rw-rw-   0        0        0       86 2023-05-08 02:01:12.000000 veilcord-0.0.0.40/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-05-20 14:15:23.028887 veilcord-0.0.0.40/setup.cfg
--rw-rw-rw-   0        0        0     1604 2023-05-20 14:15:10.000000 veilcord-0.0.0.40/setup.py
-drwxrwxrwx   0        0        0        0 2023-05-20 14:15:23.013019 veilcord-0.0.0.40/veilcord/
--rw-rw-rw-   0        0        0    13571 2023-05-20 14:14:51.000000 veilcord-0.0.0.40/veilcord/__init__.py
--rw-rw-rw-   0        0        0    16550 2023-05-20 13:52:30.000000 veilcord-0.0.0.40/veilcord/v2.py
-drwxrwxrwx   0        0        0        0 2023-05-20 14:15:23.027890 veilcord-0.0.0.40/veilcord.egg-info/
--rw-rw-rw-   0        0        0     2777 2023-05-20 14:15:22.000000 veilcord-0.0.0.40/veilcord.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      236 2023-05-20 14:15:22.000000 veilcord-0.0.0.40/veilcord.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-20 14:15:22.000000 veilcord-0.0.0.40/veilcord.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       38 2023-05-20 14:15:22.000000 veilcord-0.0.0.40/veilcord.egg-info/requires.txt
--rw-rw-rw-   0        0        0        9 2023-05-20 14:15:22.000000 veilcord-0.0.0.40/veilcord.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-05-19 23:27:43.655725 veilcord-0.0.0.5/
+-rw-rw-rw-   0        0        0     1085 2023-05-08 01:47:46.000000 veilcord-0.0.0.5/LICENSE
+-rw-rw-rw-   0        0        0     1926 2023-05-19 23:27:43.655725 veilcord-0.0.0.5/PKG-INFO
+-rw-rw-rw-   0        0        0      748 2023-05-17 01:51:11.000000 veilcord-0.0.0.5/README.md
+-rw-rw-rw-   0        0        0       86 2023-05-08 02:01:12.000000 veilcord-0.0.0.5/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-05-19 23:27:43.655725 veilcord-0.0.0.5/setup.cfg
+-rw-rw-rw-   0        0        0     1603 2023-05-19 23:27:09.000000 veilcord-0.0.0.5/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-19 23:27:43.649379 veilcord-0.0.0.5/veilcord/
+-rw-rw-rw-   0        0        0    13742 2023-05-19 23:27:30.000000 veilcord-0.0.0.5/veilcord/__init__.py
+-rw-rw-rw-   0        0        0    10092 2023-05-19 23:26:56.000000 veilcord-0.0.0.5/veilcord/verification.py
+drwxrwxrwx   0        0        0        0 2023-05-19 23:27:43.654727 veilcord-0.0.0.5/veilcord.egg-info/
+-rw-rw-rw-   0        0        0     1926 2023-05-19 23:27:43.000000 veilcord-0.0.0.5/veilcord.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      246 2023-05-19 23:27:43.000000 veilcord-0.0.0.5/veilcord.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-19 23:27:43.000000 veilcord-0.0.0.5/veilcord.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       38 2023-05-19 23:27:43.000000 veilcord-0.0.0.5/veilcord.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        9 2023-05-19 23:27:43.000000 veilcord-0.0.0.5/veilcord.egg-info/top_level.txt
```

### Comparing `veilcord-0.0.0.40/LICENSE` & `veilcord-0.0.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `veilcord-0.0.0.40/PKG-INFO` & `veilcord-0.0.0.5/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: veilcord
-Version: 0.0.0.40
+Version: 0.0.0.5
 Summary: VeilCord // vast#1337
 Home-page: http://pypi.python.org/pypi/veilcord
 Author: vast#1337
 Author-email: vastcord@proton.me
 License: MIT
 Project-URL: Homepage, https://github.com/imvast/veilcord
 Project-URL: Suggestions, https://github.com/imvast/veilcord/issues
@@ -24,59 +24,34 @@
 Classifier: Topic :: Software Development :: Libraries
 Classifier: Topic :: Utilities
 Requires-Python: ~=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # VeilCord.
-<img src="https://img.shields.io/pypi/v/veilcord?style=for-the-badge&logo=python">
+<img src="https://img.shields.io/pypi/v/terminut?style=for-the-badge&logo=python">
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
 
-### Example Usage
+### Usage
 ```py
-from veilcord import VeilCord
+# default shit if u want to only import for ease - auto switches #
 
-veilcord = VeilCord(
-    session = None, # for custom tls_client sessions
-    device_type = "browser", # types : browser, mobile, app
-    user_agent = None # for custom user agent
-)
-
-# GETTING X-Super-Properties
-xsup = veilcord.generateXProp()
-print(f"(+) Retrieved XSup: {xsup}")
-
-# GETTING ALL THE COOKIES AND FINGERPRINT
-cookies = veilcord.getFingerprint(xsup)
-print(f"(+) Retrieved Fingerprint: {cookies[0]}")
-# returns a set.  [0] - Fingerprint  |  [1] - COOKIESJAR
-
-
-# GET THE NEW SESSION ID BS
-token = ""
-sessionid = veilcord.getSession(
-      token = token, # obv the token 
-      type = 2, # type : 1 - web | 2 - app
-      keepAlive = False # keep the session alive | only needed if ur code is slow (avg. session is live for ~40 seconds.)
-)
-print(f"(+) Got Session ID: {sessionid}")
+import veilcord
 
-# close the session, if keepAlive is enabled.
-# veilcord.closeSession(token)
 
 ```
 
 ---
 
-## * [vast#1337](https://discord.com/users/1109124745477246988) | [imvast@github](https://github.com/imvast) | [vast.gay](https://vast.gay) *
+## * [vast#1337](https://discord.com/users/852976920148967485) | [imvast@github](https://github.com/imvast) | [vast.gay](https://vast.gay) *
```

### Comparing `veilcord-0.0.0.40/setup.py` & `veilcord-0.0.0.5/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 #! /usr/bin/env python
 
 from setuptools import setup, find_packages
 
-vers = "0.0.0.40"
+vers = "0.0.0.5"
     
 setup(name="veilcord",
       version=vers,
       description="VeilCord // vast#1337",
       long_description_content_type="text/markdown",
       long_description=open("README.md", encoding="utf-8").read(),
       packages=find_packages(exclude=['tests']),
```

### Comparing `veilcord-0.0.0.40/veilcord/__init__.py` & `veilcord-0.0.0.5/veilcord/__init__.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,25 +1,36 @@
-from .v2            import *
-from terminut       import printf as print
-from colorama       import Fore
-from os             import system
-from requests       import get
-
+from .verification import *
+from terminut import printf as print
+from re import search
+from colorama import Fore
 
 __author__ = "github.com/imvast"                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                   ;_0110001001101111011011110110110001110101011100110110010101100100011000100110010101100110011011110111001001100101=False
-__title__ = 'VeilCord'                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                           ;print("MADE BY VAST DONT CHANGE CREDITS U QUEER") if __author__ != "github.com/imvast" else None                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                     
-__version__ = '0.0.0.40'
 if _0110001001101111011011110110110001110101011100110110010101100100011000100110010101100110011011110111001001100101==False:print("(*) Welcome. This was made by github.com/imvast.",showTimestamp=False)                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                               ;_0110001001101111011011110110110001110101011100110110010101100100011000100110010101100110011011110111001001100101=True
 
+__title__ = 'VeilCord'                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                           ;print("MADE BY VAST DONT CHANGE CREDITS U QUEER") if __author__ != "github.com/imvast" else None                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                     
+__version__ = '0.0.0.5a'
 
-response = get('https://pypi.org/project/veilcord/').text
-CURRENT_VERSION = str(response.split('<h1 class="package-header__name">\n        veilcord ')[1].split('\n')[0])
+CURRENT_VERSION = '0.0.0.69'
 
 
 if __version__ < CURRENT_VERSION:
     print(
         f"[VeilCord] Version Out-of-Date. Please upgrade by using: \"python.exe -m pip install -U veilcord\"", 
         mainCol=Fore.RED,
         showTimestamp=False
     )
-    system('python.exe -m pip install -U veilcord  -q')
-    
+
+
+def getCode(invite):
+    """Extracts the code from a Discord invite link"""
+    code_regex = r"(?:(?:http:\/\/|https:\/\/)?discord\.gg\/|discordapp\.com\/invite\/|discord\.com\/invite\/)?([a-zA-Z0-9-]+)"
+    match = search(code_regex, invite)
+    if match:
+        try:
+            return match.group(1)
+        except:
+            return match.group(0)
+    else:
+        return None
+    
+def getBuildNum():
+    pass
```

### Comparing `veilcord-0.0.0.40/veilcord.egg-info/PKG-INFO` & `veilcord-0.0.0.5/veilcord.egg-info/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: veilcord
-Version: 0.0.0.40
+Version: 0.0.0.5
 Summary: VeilCord // vast#1337
 Home-page: http://pypi.python.org/pypi/veilcord
 Author: vast#1337
 Author-email: vastcord@proton.me
 License: MIT
 Project-URL: Homepage, https://github.com/imvast/veilcord
 Project-URL: Suggestions, https://github.com/imvast/veilcord/issues
@@ -24,59 +24,34 @@
 Classifier: Topic :: Software Development :: Libraries
 Classifier: Topic :: Utilities
 Requires-Python: ~=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # VeilCord.
-<img src="https://img.shields.io/pypi/v/veilcord?style=for-the-badge&logo=python">
+<img src="https://img.shields.io/pypi/v/terminut?style=for-the-badge&logo=python">
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
 
-### Example Usage
+### Usage
 ```py
-from veilcord import VeilCord
+# default shit if u want to only import for ease - auto switches #
 
-veilcord = VeilCord(
-    session = None, # for custom tls_client sessions
-    device_type = "browser", # types : browser, mobile, app
-    user_agent = None # for custom user agent
-)
-
-# GETTING X-Super-Properties
-xsup = veilcord.generateXProp()
-print(f"(+) Retrieved XSup: {xsup}")
-
-# GETTING ALL THE COOKIES AND FINGERPRINT
-cookies = veilcord.getFingerprint(xsup)
-print(f"(+) Retrieved Fingerprint: {cookies[0]}")
-# returns a set.  [0] - Fingerprint  |  [1] - COOKIESJAR
-
-
-# GET THE NEW SESSION ID BS
-token = ""
-sessionid = veilcord.getSession(
-      token = token, # obv the token 
-      type = 2, # type : 1 - web | 2 - app
-      keepAlive = False # keep the session alive | only needed if ur code is slow (avg. session is live for ~40 seconds.)
-)
-print(f"(+) Got Session ID: {sessionid}")
+import veilcord
 
-# close the session, if keepAlive is enabled.
-# veilcord.closeSession(token)
 
 ```
 
 ---
 
-## * [vast#1337](https://discord.com/users/1109124745477246988) | [imvast@github](https://github.com/imvast) | [vast.gay](https://vast.gay) *
+## * [vast#1337](https://discord.com/users/852976920148967485) | [imvast@github](https://github.com/imvast) | [vast.gay](https://vast.gay) *
```

