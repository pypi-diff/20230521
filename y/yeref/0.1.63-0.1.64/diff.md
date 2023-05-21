# Comparing `tmp/yeref-0.1.63.tar.gz` & `tmp/yeref-0.1.64.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "yeref-0.1.63.tar", last modified: Fri May 19 10:28:48 2023, max compression
+gzip compressed data, was "yeref-0.1.64.tar", last modified: Sun May 21 09:29:11 2023, max compression
```

## Comparing `yeref-0.1.63.tar` & `yeref-0.1.64.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxr-xr-x   0 mark       (501) staff       (20)        0 2023-05-19 10:28:48.622886 yeref-0.1.63/
--rw-r--r--   0 mark       (501) staff       (20)       85 2023-05-19 10:28:48.623379 yeref-0.1.63/PKG-INFO
--rw-r--r--   0 mark       (501) staff       (20)       38 2023-05-19 10:28:48.624108 yeref-0.1.63/setup.cfg
--rw-r--r--   0 mark       (501) staff       (20)     1351 2023-05-19 10:28:37.000000 yeref-0.1.63/setup.py
-drwxr-xr-x   0 mark       (501) staff       (20)        0 2023-05-19 10:28:48.614916 yeref-0.1.63/yeref/
--rw-r--r--   0 mark       (501) staff       (20)       39 2023-04-21 17:52:00.000000 yeref-0.1.63/yeref/__init__.py
--rw-r--r--   0 mark       (501) staff       (20)   511251 2023-05-09 14:24:53.000000 yeref-0.1.63/yeref/l_.py
--rw-r--r--   0 mark       (501) staff       (20)   204234 2023-05-19 10:27:02.000000 yeref-0.1.63/yeref/yeref.py
-drwxr-xr-x   0 mark       (501) staff       (20)        0 2023-05-19 10:28:48.621580 yeref-0.1.63/yeref.egg-info/
--rw-r--r--   0 mark       (501) staff       (20)       85 2023-05-19 10:28:48.000000 yeref-0.1.63/yeref.egg-info/PKG-INFO
--rw-r--r--   0 mark       (501) staff       (20)      179 2023-05-19 10:28:48.000000 yeref-0.1.63/yeref.egg-info/SOURCES.txt
--rw-r--r--   0 mark       (501) staff       (20)        1 2023-05-19 10:28:48.000000 yeref-0.1.63/yeref.egg-info/dependency_links.txt
--rw-r--r--   0 mark       (501) staff       (20)        6 2023-05-19 10:28:48.000000 yeref-0.1.63/yeref.egg-info/top_level.txt
+drwxr-xr-x   0 mark       (501) staff       (20)        0 2023-05-21 09:29:11.973799 yeref-0.1.64/
+-rw-r--r--   0 mark       (501) staff       (20)       85 2023-05-21 09:29:11.974235 yeref-0.1.64/PKG-INFO
+-rw-r--r--   0 mark       (501) staff       (20)       38 2023-05-21 09:29:11.975784 yeref-0.1.64/setup.cfg
+-rw-r--r--   0 mark       (501) staff       (20)     1351 2023-05-21 09:28:57.000000 yeref-0.1.64/setup.py
+drwxr-xr-x   0 mark       (501) staff       (20)        0 2023-05-21 09:29:11.965920 yeref-0.1.64/yeref/
+-rw-r--r--   0 mark       (501) staff       (20)       39 2023-04-21 17:52:00.000000 yeref-0.1.64/yeref/__init__.py
+-rw-r--r--   0 mark       (501) staff       (20)   511251 2023-05-09 14:24:53.000000 yeref-0.1.64/yeref/l_.py
+-rw-r--r--   0 mark       (501) staff       (20)   204714 2023-05-21 07:57:19.000000 yeref-0.1.64/yeref/yeref.py
+drwxr-xr-x   0 mark       (501) staff       (20)        0 2023-05-21 09:29:11.973045 yeref-0.1.64/yeref.egg-info/
+-rw-r--r--   0 mark       (501) staff       (20)       85 2023-05-21 09:29:11.000000 yeref-0.1.64/yeref.egg-info/PKG-INFO
+-rw-r--r--   0 mark       (501) staff       (20)      179 2023-05-21 09:29:11.000000 yeref-0.1.64/yeref.egg-info/SOURCES.txt
+-rw-r--r--   0 mark       (501) staff       (20)        1 2023-05-21 09:29:11.000000 yeref-0.1.64/yeref.egg-info/dependency_links.txt
+-rw-r--r--   0 mark       (501) staff       (20)        6 2023-05-21 09:29:11.000000 yeref-0.1.64/yeref.egg-info/top_level.txt
```

### Comparing `yeref-0.1.63/setup.py` & `yeref-0.1.64/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup
 
 setup(
       name='yeref',
-      version='0.1.63',
+      version='0.1.64',
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
 
-# python3 -m pip install --force-reinstall /Users/mark/PycharmProjects/AUTOBOT/yeref/dist/yeref-0.1.63-py3-none-any.whl
+# python3 -m pip install --force-reinstall /Users/mark/PycharmProjects/AUTOBOT/yeref/dist/yeref-0.1.64-py3-none-any.whl
 
 # python3 -m pip install --upgrade yeref
 
 # pip install --force-reinstall -v "yeref==0.1.30"
 # pip install https://github.com/aiogram/aiogram/archive/refs/heads/dev-3.x.zip
 # pip show aiogram
 # ARCHFLAGS="-arch x86_64" pip install pycurl
```

### Comparing `yeref-0.1.63/yeref/l_.py` & `yeref-0.1.64/yeref/l_.py`

 * *Files identical despite different names*

### Comparing `yeref-0.1.63/yeref/yeref.py` & `yeref-0.1.64/yeref/yeref.py`

 * *Files 0% similar despite different names*

```diff
@@ -218,40 +218,14 @@
 
 
 async def db_bot_create(db):
     con = sqlite3.connect(db, timeout=10)
     try:
         cur = con.cursor()
 
-        # USER
-        cur.execute(f'''CREATE TABLE IF NOT EXISTS USER ( 
-            USER_ID         INTEGER     PRIMARY KEY AUTOINCREMENT
-                                        UNIQUE
-                                        NOT NULL,
-            USER_TID        BIGINT      UNIQUE
-                                        NOT NULL,
-            USER_USERNAME   VARCHAR,
-            USER_FULLNAME   VARCHAR,
-
-            USER_VARS       VARCHAR     DEFAULT '{USER_VARS_}',
-            USER_LSTS       VARCHAR     DEFAULT '{USER_LSTS_}'
-        )''')
-
-        # USERBAN
-        cur.execute('''CREATE TABLE IF NOT EXISTS USERBAN ( 
-            USERBAN_ID          INTEGER     PRIMARY KEY AUTOINCREMENT
-                                            UNIQUE
-                                            NOT NULL,
-            USERBAN_TID         BIGINT      UNIQUE,
-            USERBAN_USERNAME    VARCHAR     UNIQUE,
-            USERBAN_FULLNAME    VARCHAR,
-            USERBAN_BAN         VARCHAR, 
-            USERBAN_DT          VARCHAR
-        )''')
-
         # TRG
         cur.execute('''CREATE TABLE IF NOT EXISTS TRG ( 
             TRG_ID          INTEGER     PRIMARY KEY AUTOINCREMENT
                                         UNIQUE
                                         NOT NULL,
             TRG_VID         VARCHAR     UNIQUE NOT NULL,
             TRG_TYPE        VARCHAR,
@@ -284,28 +258,67 @@
                                         UNIQUE
                                         NOT NULL,
             MSG_VID         VARCHAR     UNIQUE NOT NULL,
             MSG_TYPE        VARCHAR,
             MSG_TEXT        VARCHAR,
             MSG_MEDIA       VARCHAR,
             MSG_BUTTONS     VARCHAR,
+            
             MSG_CHKBOX      VARCHAR,
             MSG_TEXTF       VARCHAR,
+            MSG_FILENAME    VARCHAR,      
             MSG_BUTTONSF    VARCHAR,
-            MSG_FILENAME    VARCHAR,
-
-            MSG_STATUS      VARCHAR,
-            MSG_LZ          VARCHAR,
-            MSG_DT          VARCHAR,
+            MSG_LC          VARCHAR,
+            MSG_TRANSLATED  INTEGER     DEFAULT 0,
 
             MSG_NEXTID      VARCHAR,
             MSG_NEXTTYPE    VARCHAR,
             MSG_USERS       VARCHAR
         )''')
 
+        # LANG
+        cur.execute('''CREATE TABLE IF NOT EXISTS LANG ( 
+            LANG_ID         INTEGER     PRIMARY KEY AUTOINCREMENT
+                                        UNIQUE
+                                        NOT NULL,
+            MSG_ID          INTEGER,
+            MSG_LC          VARCHAR,
+            
+            MSG_TEXT        VARCHAR,
+            MSG_BUTTONS     VARCHAR,
+            MSG_TEXTF       VARCHAR,
+            MSG_BUTTONSF    VARCHAR
+        )''')
+
+        # USER
+        cur.execute(f'''CREATE TABLE IF NOT EXISTS USER ( 
+            USER_ID         INTEGER     PRIMARY KEY AUTOINCREMENT
+                                        UNIQUE
+                                        NOT NULL,
+            USER_TID        BIGINT      UNIQUE
+                                        NOT NULL,
+            USER_USERNAME   VARCHAR,
+            USER_FULLNAME   VARCHAR,
+
+            USER_VARS       VARCHAR     DEFAULT '{USER_VARS_}',
+            USER_LSTS       VARCHAR     DEFAULT '{USER_LSTS_}'
+        )''')
+
+        # USERBAN
+        cur.execute('''CREATE TABLE IF NOT EXISTS USERBAN ( 
+            USERBAN_ID          INTEGER     PRIMARY KEY AUTOINCREMENT
+                                            UNIQUE
+                                            NOT NULL,
+            USERBAN_TID         BIGINT      UNIQUE,
+            USERBAN_USERNAME    VARCHAR     UNIQUE,
+            USERBAN_FULLNAME    VARCHAR,
+            USERBAN_BAN         VARCHAR, 
+            USERBAN_DT          VARCHAR
+        )''')
+
         con.commit()
         cur.close()
     except Exception as e:
         logger.info(log_ % str(e))
         await asyncio.sleep(round(random.uniform(0, 1), 2))
     finally:
         con.close()
```

