# Comparing `tmp/yeref-0.1.64.tar.gz` & `tmp/yeref-0.1.65.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "yeref-0.1.64.tar", last modified: Sun May 21 09:29:11 2023, max compression
+gzip compressed data, was "yeref-0.1.65.tar", last modified: Sun May 21 14:12:47 2023, max compression
```

## Comparing `yeref-0.1.64.tar` & `yeref-0.1.65.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxr-xr-x   0 mark       (501) staff       (20)        0 2023-05-21 09:29:11.973799 yeref-0.1.64/
--rw-r--r--   0 mark       (501) staff       (20)       85 2023-05-21 09:29:11.974235 yeref-0.1.64/PKG-INFO
--rw-r--r--   0 mark       (501) staff       (20)       38 2023-05-21 09:29:11.975784 yeref-0.1.64/setup.cfg
--rw-r--r--   0 mark       (501) staff       (20)     1351 2023-05-21 09:28:57.000000 yeref-0.1.64/setup.py
-drwxr-xr-x   0 mark       (501) staff       (20)        0 2023-05-21 09:29:11.965920 yeref-0.1.64/yeref/
--rw-r--r--   0 mark       (501) staff       (20)       39 2023-04-21 17:52:00.000000 yeref-0.1.64/yeref/__init__.py
--rw-r--r--   0 mark       (501) staff       (20)   511251 2023-05-09 14:24:53.000000 yeref-0.1.64/yeref/l_.py
--rw-r--r--   0 mark       (501) staff       (20)   204714 2023-05-21 07:57:19.000000 yeref-0.1.64/yeref/yeref.py
-drwxr-xr-x   0 mark       (501) staff       (20)        0 2023-05-21 09:29:11.973045 yeref-0.1.64/yeref.egg-info/
--rw-r--r--   0 mark       (501) staff       (20)       85 2023-05-21 09:29:11.000000 yeref-0.1.64/yeref.egg-info/PKG-INFO
--rw-r--r--   0 mark       (501) staff       (20)      179 2023-05-21 09:29:11.000000 yeref-0.1.64/yeref.egg-info/SOURCES.txt
--rw-r--r--   0 mark       (501) staff       (20)        1 2023-05-21 09:29:11.000000 yeref-0.1.64/yeref.egg-info/dependency_links.txt
--rw-r--r--   0 mark       (501) staff       (20)        6 2023-05-21 09:29:11.000000 yeref-0.1.64/yeref.egg-info/top_level.txt
+drwxr-xr-x   0 mark       (501) staff       (20)        0 2023-05-21 14:12:47.548693 yeref-0.1.65/
+-rw-r--r--   0 mark       (501) staff       (20)       85 2023-05-21 14:12:47.548840 yeref-0.1.65/PKG-INFO
+-rw-r--r--   0 mark       (501) staff       (20)       38 2023-05-21 14:12:47.549407 yeref-0.1.65/setup.cfg
+-rw-r--r--   0 mark       (501) staff       (20)     1351 2023-05-21 14:12:35.000000 yeref-0.1.65/setup.py
+drwxr-xr-x   0 mark       (501) staff       (20)        0 2023-05-21 14:12:47.542591 yeref-0.1.65/yeref/
+-rw-r--r--   0 mark       (501) staff       (20)       39 2023-04-21 17:52:00.000000 yeref-0.1.65/yeref/__init__.py
+-rw-r--r--   0 mark       (501) staff       (20)   511251 2023-05-09 14:24:53.000000 yeref-0.1.65/yeref/l_.py
+-rw-r--r--   0 mark       (501) staff       (20)   204673 2023-05-21 14:10:12.000000 yeref-0.1.65/yeref/yeref.py
+drwxr-xr-x   0 mark       (501) staff       (20)        0 2023-05-21 14:12:47.548301 yeref-0.1.65/yeref.egg-info/
+-rw-r--r--   0 mark       (501) staff       (20)       85 2023-05-21 14:12:47.000000 yeref-0.1.65/yeref.egg-info/PKG-INFO
+-rw-r--r--   0 mark       (501) staff       (20)      179 2023-05-21 14:12:47.000000 yeref-0.1.65/yeref.egg-info/SOURCES.txt
+-rw-r--r--   0 mark       (501) staff       (20)        1 2023-05-21 14:12:47.000000 yeref-0.1.65/yeref.egg-info/dependency_links.txt
+-rw-r--r--   0 mark       (501) staff       (20)        6 2023-05-21 14:12:47.000000 yeref-0.1.65/yeref.egg-info/top_level.txt
```

### Comparing `yeref-0.1.64/setup.py` & `yeref-0.1.65/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup
 
 setup(
       name='yeref',
-      version='0.1.64',
+      version='0.1.65',
       description='desc-f',
       author='john smith',
       packages=['yeref'],
       # install_requires=[
       #       "httplib2>=0.20.4",
       #       "moviepy>=1.0.3",
       #       "Pillow>=9.2.0",
@@ -39,15 +39,15 @@
 # python setup.py bdist_wheel
 # endregion
 
 # python -m build
 
 # twine upload dist/*
 
-# python3 -m pip install --force-reinstall /Users/mark/PycharmProjects/AUTOBOT/yeref/dist/yeref-0.1.64-py3-none-any.whl
+# python3 -m pip install --force-reinstall /Users/mark/PycharmProjects/AUTOBOT/yeref/dist/yeref-0.1.65-py3-none-any.whl
 
 # python3 -m pip install --upgrade yeref
 
 # pip install --force-reinstall -v "yeref==0.1.30"
 # pip install https://github.com/aiogram/aiogram/archive/refs/heads/dev-3.x.zip
 # pip show aiogram
 # ARCHFLAGS="-arch x86_64" pip install pycurl
```

### Comparing `yeref-0.1.64/yeref/l_.py` & `yeref-0.1.65/yeref/l_.py`

 * *Files identical despite different names*

### Comparing `yeref-0.1.64/yeref/yeref.py` & `yeref-0.1.65/yeref/yeref.py`

 * *Files 0% similar despite different names*

```diff
@@ -260,16 +260,15 @@
             MSG_VID         VARCHAR     UNIQUE NOT NULL,
             MSG_TYPE        VARCHAR,
             MSG_TEXT        VARCHAR,
             MSG_MEDIA       VARCHAR,
             MSG_BUTTONS     VARCHAR,
             
             MSG_CHKBOX      VARCHAR,
-            MSG_TEXTF       VARCHAR,
-            MSG_FILENAME    VARCHAR,      
+            MSG_TEXTF       VARCHAR,  
             MSG_BUTTONSF    VARCHAR,
             MSG_LC          VARCHAR,
             MSG_TRANSLATED  INTEGER     DEFAULT 0,
 
             MSG_NEXTID      VARCHAR,
             MSG_NEXTTYPE    VARCHAR,
             MSG_USERS       VARCHAR
```

