# Comparing `tmp/Flask-RESTful-0.3.8.tar.gz` & `tmp/Flask-RESTful-0.3.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/Flask-RESTful-0.3.8.tar", last modified: Thu Feb  6 13:49:36 2020, max compression
+gzip compressed data, was "dist/Flask-RESTful-0.3.9.tar", last modified: Mon May 17 19:23:11 2021, max compression
```

## Comparing `Flask-RESTful-0.3.8.tar` & `Flask-RESTful-0.3.9.tar`

### file list

```diff
@@ -1,64 +1,65 @@
-drwxr-xr-x   0 josh       (501) staff       (20)        0 2020-02-06 13:49:36.111270 Flask-RESTful-0.3.8/
--rw-r--r--   0 josh       (501) staff       (20)     1992 2017-05-31 12:02:31.000000 Flask-RESTful-0.3.8/AUTHORS.md
-drwxr-xr-x   0 josh       (501) staff       (20)        0 2020-02-06 13:49:36.089984 Flask-RESTful-0.3.8/Flask_RESTful.egg-info/
--rw-r--r--   0 josh       (501) staff       (20)      770 2020-02-06 13:49:36.000000 Flask-RESTful-0.3.8/Flask_RESTful.egg-info/PKG-INFO
--rw-r--r--   0 josh       (501) staff       (20)     1238 2020-02-06 13:49:36.000000 Flask-RESTful-0.3.8/Flask_RESTful.egg-info/SOURCES.txt
--rw-r--r--   0 josh       (501) staff       (20)        1 2020-02-06 13:49:36.000000 Flask-RESTful-0.3.8/Flask_RESTful.egg-info/dependency_links.txt
--rw-r--r--   0 josh       (501) staff       (20)        1 2018-03-29 18:50:14.000000 Flask-RESTful-0.3.8/Flask_RESTful.egg-info/not-zip-safe
--rw-r--r--   0 josh       (501) staff       (20)       58 2020-02-06 13:49:36.000000 Flask-RESTful-0.3.8/Flask_RESTful.egg-info/requires.txt
--rw-r--r--   0 josh       (501) staff       (20)       14 2020-02-06 13:49:36.000000 Flask-RESTful-0.3.8/Flask_RESTful.egg-info/top_level.txt
--rw-r--r--   0 josh       (501) staff       (20)     1485 2016-12-28 15:23:58.000000 Flask-RESTful-0.3.8/LICENSE
--rw-r--r--   0 josh       (501) staff       (20)      344 2016-12-28 15:23:58.000000 Flask-RESTful-0.3.8/MANIFEST.in
--rw-r--r--   0 josh       (501) staff       (20)     4845 2020-02-06 13:45:04.000000 Flask-RESTful-0.3.8/Makefile
--rw-r--r--   0 josh       (501) staff       (20)      770 2020-02-06 13:49:36.111480 Flask-RESTful-0.3.8/PKG-INFO
--rw-r--r--   0 josh       (501) staff       (20)      596 2018-03-29 18:45:50.000000 Flask-RESTful-0.3.8/README.md
-drwxr-xr-x   0 josh       (501) staff       (20)        0 2020-02-06 13:49:36.093338 Flask-RESTful-0.3.8/docs/
--rw-r--r--   0 josh       (501) staff       (20)     5592 2016-12-28 15:23:56.000000 Flask-RESTful-0.3.8/docs/Makefile
-drwxr-xr-x   0 josh       (501) staff       (20)        0 2020-02-06 13:49:36.101545 Flask-RESTful-0.3.8/docs/_static/
--rw-r--r--   0 josh       (501) staff       (20)    20913 2016-12-28 15:23:56.000000 Flask-RESTful-0.3.8/docs/_static/flask-restful-small.png
--rw-r--r--   0 josh       (501) staff       (20)    17865 2016-12-28 15:23:56.000000 Flask-RESTful-0.3.8/docs/_static/flask-restful.png
-drwxr-xr-x   0 josh       (501) staff       (20)        0 2020-02-06 13:49:36.102235 Flask-RESTful-0.3.8/docs/_templates/
--rw-r--r--   0 josh       (501) staff       (20)      617 2016-12-28 15:23:56.000000 Flask-RESTful-0.3.8/docs/_templates/sidebarintro.html
--rw-r--r--   0 josh       (501) staff       (20)      182 2016-12-28 15:23:56.000000 Flask-RESTful-0.3.8/docs/_templates/sidebarlogo.html
--rw-r--r--   0 josh       (501) staff       (20)      579 2016-12-28 15:23:56.000000 Flask-RESTful-0.3.8/docs/api.rst
--rw-r--r--   0 josh       (501) staff       (20)     9184 2017-09-20 13:10:34.000000 Flask-RESTful-0.3.8/docs/conf.py
--rw-r--r--   0 josh       (501) staff       (20)      629 2016-12-28 15:23:56.000000 Flask-RESTful-0.3.8/docs/contents.rst.inc
--rw-r--r--   0 josh       (501) staff       (20)     9585 2020-02-06 13:42:49.000000 Flask-RESTful-0.3.8/docs/extending.rst
--rw-r--r--   0 josh       (501) staff       (20)     9422 2020-02-06 13:42:49.000000 Flask-RESTful-0.3.8/docs/fields.rst
--rw-r--r--   0 josh       (501) staff       (20)      403 2016-12-28 15:23:56.000000 Flask-RESTful-0.3.8/docs/index.rst
--rw-r--r--   0 josh       (501) staff       (20)      622 2018-12-18 12:49:18.000000 Flask-RESTful-0.3.8/docs/installation.rst
--rw-r--r--   0 josh       (501) staff       (20)     9789 2020-02-06 13:42:49.000000 Flask-RESTful-0.3.8/docs/intermediate-usage.rst
--rw-r--r--   0 josh       (501) staff       (20)     5110 2016-12-28 15:23:56.000000 Flask-RESTful-0.3.8/docs/make.bat
--rw-r--r--   0 josh       (501) staff       (20)    10866 2018-12-18 12:49:18.000000 Flask-RESTful-0.3.8/docs/quickstart.rst
--rw-r--r--   0 josh       (501) staff       (20)     8239 2017-04-02 21:29:53.000000 Flask-RESTful-0.3.8/docs/reqparse.rst
--rw-r--r--   0 josh       (501) staff       (20)      903 2020-02-06 13:42:49.000000 Flask-RESTful-0.3.8/docs/testing.rst
-drwxr-xr-x   0 josh       (501) staff       (20)        0 2020-02-06 13:49:36.103109 Flask-RESTful-0.3.8/examples/
--rw-r--r--   0 josh       (501) staff       (20)     1432 2016-12-28 15:23:58.000000 Flask-RESTful-0.3.8/examples/todo.py
--rw-r--r--   0 josh       (501) staff       (20)     1332 2016-12-28 15:23:58.000000 Flask-RESTful-0.3.8/examples/todo_simple.py
--rw-r--r--   0 josh       (501) staff       (20)     1167 2016-12-28 15:23:58.000000 Flask-RESTful-0.3.8/examples/xml_representation.py
-drwxr-xr-x   0 josh       (501) staff       (20)        0 2020-02-06 13:49:36.104813 Flask-RESTful-0.3.8/flask_restful/
--rw-r--r--   0 josh       (501) staff       (20)    27927 2020-02-06 13:42:49.000000 Flask-RESTful-0.3.8/flask_restful/__init__.py
--rw-r--r--   0 josh       (501) staff       (20)       45 2020-02-06 13:47:56.000000 Flask-RESTful-0.3.8/flask_restful/__version__.py
--rw-r--r--   0 josh       (501) staff       (20)    13069 2017-09-20 13:10:28.000000 Flask-RESTful-0.3.8/flask_restful/fields.py
--rw-r--r--   0 josh       (501) staff       (20)     9114 2017-04-02 21:29:53.000000 Flask-RESTful-0.3.8/flask_restful/inputs.py
-drwxr-xr-x   0 josh       (501) staff       (20)        0 2020-02-06 13:49:36.105349 Flask-RESTful-0.3.8/flask_restful/representations/
--rw-r--r--   0 josh       (501) staff       (20)        1 2016-12-28 15:23:58.000000 Flask-RESTful-0.3.8/flask_restful/representations/__init__.py
--rw-r--r--   0 josh       (501) staff       (20)      873 2017-05-31 11:48:12.000000 Flask-RESTful-0.3.8/flask_restful/representations/json.py
--rw-r--r--   0 josh       (501) staff       (20)    14681 2020-02-06 13:42:49.000000 Flask-RESTful-0.3.8/flask_restful/reqparse.py
-drwxr-xr-x   0 josh       (501) staff       (20)        0 2020-02-06 13:49:36.106188 Flask-RESTful-0.3.8/flask_restful/utils/
--rw-r--r--   0 josh       (501) staff       (20)      723 2020-02-06 13:42:49.000000 Flask-RESTful-0.3.8/flask_restful/utils/__init__.py
--rw-r--r--   0 josh       (501) staff       (20)     2084 2016-12-28 15:23:58.000000 Flask-RESTful-0.3.8/flask_restful/utils/cors.py
--rw-r--r--   0 josh       (501) staff       (20)      996 2016-12-28 15:23:58.000000 Flask-RESTful-0.3.8/flask_restful/utils/crypto.py
--rw-r--r--   0 josh       (501) staff       (20)       70 2020-02-06 13:49:36.112238 Flask-RESTful-0.3.8/setup.cfg
--rwxr-xr-x   0 josh       (501) staff       (20)     1581 2020-02-06 13:42:49.000000 Flask-RESTful-0.3.8/setup.py
-drwxr-xr-x   0 josh       (501) staff       (20)        0 2020-02-06 13:49:36.110766 Flask-RESTful-0.3.8/tests/
--rw-r--r--   0 josh       (501) staff       (20)       79 2016-12-28 15:23:58.000000 Flask-RESTful-0.3.8/tests/README.md
--rw-r--r--   0 josh       (501) staff       (20)      340 2016-12-28 15:23:58.000000 Flask-RESTful-0.3.8/tests/__init__.py
--rw-r--r--   0 josh       (501) staff       (20)       41 2016-12-28 15:23:58.000000 Flask-RESTful-0.3.8/tests/requirements.txt
--rw-r--r--   0 josh       (501) staff       (20)     7668 2016-12-28 15:23:58.000000 Flask-RESTful-0.3.8/tests/test_accept.py
--rw-r--r--   0 josh       (501) staff       (20)    37604 2020-02-06 13:42:49.000000 Flask-RESTful-0.3.8/tests/test_api.py
--rw-r--r--   0 josh       (501) staff       (20)     7991 2016-12-28 15:23:58.000000 Flask-RESTful-0.3.8/tests/test_api_with_blueprint.py
--rw-r--r--   0 josh       (501) staff       (20)     3113 2018-12-18 12:49:18.000000 Flask-RESTful-0.3.8/tests/test_cors.py
--rw-r--r--   0 josh       (501) staff       (20)    18877 2017-09-20 13:10:04.000000 Flask-RESTful-0.3.8/tests/test_fields.py
--rw-r--r--   0 josh       (501) staff       (20)    12433 2018-03-29 18:51:59.000000 Flask-RESTful-0.3.8/tests/test_inputs.py
--rw-r--r--   0 josh       (501) staff       (20)    34432 2020-02-06 13:42:49.000000 Flask-RESTful-0.3.8/tests/test_reqparse.py
+drwxr-xr-x   0 josh       (501) staff       (20)        0 2021-05-17 19:23:11.894755 Flask-RESTful-0.3.9/
+-rw-r--r--   0 josh       (501) staff       (20)     1992 2017-05-31 12:02:31.000000 Flask-RESTful-0.3.9/AUTHORS.md
+drwxr-xr-x   0 josh       (501) staff       (20)        0 2021-05-17 19:23:11.876650 Flask-RESTful-0.3.9/Flask_RESTful.egg-info/
+-rw-r--r--   0 josh       (501) staff       (20)      770 2021-05-17 19:23:11.000000 Flask-RESTful-0.3.9/Flask_RESTful.egg-info/PKG-INFO
+-rw-r--r--   0 josh       (501) staff       (20)     1259 2021-05-17 19:23:11.000000 Flask-RESTful-0.3.9/Flask_RESTful.egg-info/SOURCES.txt
+-rw-r--r--   0 josh       (501) staff       (20)        1 2021-05-17 19:23:11.000000 Flask-RESTful-0.3.9/Flask_RESTful.egg-info/dependency_links.txt
+-rw-r--r--   0 josh       (501) staff       (20)        1 2018-03-29 18:50:14.000000 Flask-RESTful-0.3.9/Flask_RESTful.egg-info/not-zip-safe
+-rw-r--r--   0 josh       (501) staff       (20)       58 2021-05-17 19:23:11.000000 Flask-RESTful-0.3.9/Flask_RESTful.egg-info/requires.txt
+-rw-r--r--   0 josh       (501) staff       (20)       14 2021-05-17 19:23:11.000000 Flask-RESTful-0.3.9/Flask_RESTful.egg-info/top_level.txt
+-rw-r--r--   0 josh       (501) staff       (20)     1485 2016-12-28 15:23:58.000000 Flask-RESTful-0.3.9/LICENSE
+-rw-r--r--   0 josh       (501) staff       (20)      344 2016-12-28 15:23:58.000000 Flask-RESTful-0.3.9/MANIFEST.in
+-rw-r--r--   0 josh       (501) staff       (20)     4845 2021-05-17 19:18:29.000000 Flask-RESTful-0.3.9/Makefile
+-rw-r--r--   0 josh       (501) staff       (20)      770 2021-05-17 19:23:11.894976 Flask-RESTful-0.3.9/PKG-INFO
+-rw-r--r--   0 josh       (501) staff       (20)      596 2018-03-29 18:45:50.000000 Flask-RESTful-0.3.9/README.md
+drwxr-xr-x   0 josh       (501) staff       (20)        0 2021-05-17 19:23:11.881199 Flask-RESTful-0.3.9/docs/
+-rw-r--r--   0 josh       (501) staff       (20)    20480 2021-05-17 19:16:30.000000 Flask-RESTful-0.3.9/docs/.fields.rst.swp
+-rw-r--r--   0 josh       (501) staff       (20)     5592 2016-12-28 15:23:56.000000 Flask-RESTful-0.3.9/docs/Makefile
+drwxr-xr-x   0 josh       (501) staff       (20)        0 2021-05-17 19:23:11.882306 Flask-RESTful-0.3.9/docs/_static/
+-rw-r--r--   0 josh       (501) staff       (20)    20913 2016-12-28 15:23:56.000000 Flask-RESTful-0.3.9/docs/_static/flask-restful-small.png
+-rw-r--r--   0 josh       (501) staff       (20)    17865 2016-12-28 15:23:56.000000 Flask-RESTful-0.3.9/docs/_static/flask-restful.png
+drwxr-xr-x   0 josh       (501) staff       (20)        0 2021-05-17 19:23:11.883255 Flask-RESTful-0.3.9/docs/_templates/
+-rw-r--r--   0 josh       (501) staff       (20)      617 2016-12-28 15:23:56.000000 Flask-RESTful-0.3.9/docs/_templates/sidebarintro.html
+-rw-r--r--   0 josh       (501) staff       (20)      182 2016-12-28 15:23:56.000000 Flask-RESTful-0.3.9/docs/_templates/sidebarlogo.html
+-rw-r--r--   0 josh       (501) staff       (20)      579 2016-12-28 15:23:56.000000 Flask-RESTful-0.3.9/docs/api.rst
+-rw-r--r--   0 josh       (501) staff       (20)     9184 2017-09-20 13:10:34.000000 Flask-RESTful-0.3.9/docs/conf.py
+-rw-r--r--   0 josh       (501) staff       (20)      629 2016-12-28 15:23:56.000000 Flask-RESTful-0.3.9/docs/contents.rst.inc
+-rw-r--r--   0 josh       (501) staff       (20)     9585 2020-02-06 13:42:49.000000 Flask-RESTful-0.3.9/docs/extending.rst
+-rw-r--r--   0 josh       (501) staff       (20)     9422 2021-05-17 19:16:30.000000 Flask-RESTful-0.3.9/docs/fields.rst
+-rw-r--r--   0 josh       (501) staff       (20)      403 2016-12-28 15:23:56.000000 Flask-RESTful-0.3.9/docs/index.rst
+-rw-r--r--   0 josh       (501) staff       (20)      622 2018-12-18 12:49:18.000000 Flask-RESTful-0.3.9/docs/installation.rst
+-rw-r--r--   0 josh       (501) staff       (20)     9785 2021-05-17 19:16:30.000000 Flask-RESTful-0.3.9/docs/intermediate-usage.rst
+-rw-r--r--   0 josh       (501) staff       (20)     5110 2016-12-28 15:23:56.000000 Flask-RESTful-0.3.9/docs/make.bat
+-rw-r--r--   0 josh       (501) staff       (20)    10866 2018-12-18 12:49:18.000000 Flask-RESTful-0.3.9/docs/quickstart.rst
+-rw-r--r--   0 josh       (501) staff       (20)     8239 2017-04-02 21:29:53.000000 Flask-RESTful-0.3.9/docs/reqparse.rst
+-rw-r--r--   0 josh       (501) staff       (20)      903 2020-02-06 13:42:49.000000 Flask-RESTful-0.3.9/docs/testing.rst
+drwxr-xr-x   0 josh       (501) staff       (20)        0 2021-05-17 19:23:11.884793 Flask-RESTful-0.3.9/examples/
+-rw-r--r--   0 josh       (501) staff       (20)     1432 2016-12-28 15:23:58.000000 Flask-RESTful-0.3.9/examples/todo.py
+-rw-r--r--   0 josh       (501) staff       (20)     1332 2016-12-28 15:23:58.000000 Flask-RESTful-0.3.9/examples/todo_simple.py
+-rw-r--r--   0 josh       (501) staff       (20)     1167 2016-12-28 15:23:58.000000 Flask-RESTful-0.3.9/examples/xml_representation.py
+drwxr-xr-x   0 josh       (501) staff       (20)        0 2021-05-17 19:23:11.887369 Flask-RESTful-0.3.9/flask_restful/
+-rw-r--r--   0 josh       (501) staff       (20)    27859 2021-05-17 19:16:30.000000 Flask-RESTful-0.3.9/flask_restful/__init__.py
+-rw-r--r--   0 josh       (501) staff       (20)       45 2021-05-17 19:21:14.000000 Flask-RESTful-0.3.9/flask_restful/__version__.py
+-rw-r--r--   0 josh       (501) staff       (20)    13018 2021-05-17 19:16:30.000000 Flask-RESTful-0.3.9/flask_restful/fields.py
+-rw-r--r--   0 josh       (501) staff       (20)     9118 2021-05-17 19:16:30.000000 Flask-RESTful-0.3.9/flask_restful/inputs.py
+drwxr-xr-x   0 josh       (501) staff       (20)        0 2021-05-17 19:23:11.887954 Flask-RESTful-0.3.9/flask_restful/representations/
+-rw-r--r--   0 josh       (501) staff       (20)        1 2016-12-28 15:23:58.000000 Flask-RESTful-0.3.9/flask_restful/representations/__init__.py
+-rw-r--r--   0 josh       (501) staff       (20)      873 2017-05-31 11:48:12.000000 Flask-RESTful-0.3.9/flask_restful/representations/json.py
+-rw-r--r--   0 josh       (501) staff       (20)    14681 2020-02-06 13:42:49.000000 Flask-RESTful-0.3.9/flask_restful/reqparse.py
+drwxr-xr-x   0 josh       (501) staff       (20)        0 2021-05-17 19:23:11.889202 Flask-RESTful-0.3.9/flask_restful/utils/
+-rw-r--r--   0 josh       (501) staff       (20)      723 2020-02-06 13:42:49.000000 Flask-RESTful-0.3.9/flask_restful/utils/__init__.py
+-rw-r--r--   0 josh       (501) staff       (20)     2084 2016-12-28 15:23:58.000000 Flask-RESTful-0.3.9/flask_restful/utils/cors.py
+-rw-r--r--   0 josh       (501) staff       (20)      996 2016-12-28 15:23:58.000000 Flask-RESTful-0.3.9/flask_restful/utils/crypto.py
+-rw-r--r--   0 josh       (501) staff       (20)       70 2021-05-17 19:23:11.895683 Flask-RESTful-0.3.9/setup.cfg
+-rwxr-xr-x   0 josh       (501) staff       (20)     1581 2020-02-06 13:42:49.000000 Flask-RESTful-0.3.9/setup.py
+drwxr-xr-x   0 josh       (501) staff       (20)        0 2021-05-17 19:23:11.894253 Flask-RESTful-0.3.9/tests/
+-rw-r--r--   0 josh       (501) staff       (20)       79 2016-12-28 15:23:58.000000 Flask-RESTful-0.3.9/tests/README.md
+-rw-r--r--   0 josh       (501) staff       (20)      340 2016-12-28 15:23:58.000000 Flask-RESTful-0.3.9/tests/__init__.py
+-rw-r--r--   0 josh       (501) staff       (20)       41 2016-12-28 15:23:58.000000 Flask-RESTful-0.3.9/tests/requirements.txt
+-rw-r--r--   0 josh       (501) staff       (20)     7700 2021-05-17 19:16:30.000000 Flask-RESTful-0.3.9/tests/test_accept.py
+-rw-r--r--   0 josh       (501) staff       (20)    37608 2021-05-17 19:16:30.000000 Flask-RESTful-0.3.9/tests/test_api.py
+-rw-r--r--   0 josh       (501) staff       (20)     7982 2021-05-17 19:16:30.000000 Flask-RESTful-0.3.9/tests/test_api_with_blueprint.py
+-rw-r--r--   0 josh       (501) staff       (20)     3129 2021-05-17 19:16:30.000000 Flask-RESTful-0.3.9/tests/test_cors.py
+-rw-r--r--   0 josh       (501) staff       (20)    18817 2021-05-17 19:16:30.000000 Flask-RESTful-0.3.9/tests/test_fields.py
+-rw-r--r--   0 josh       (501) staff       (20)    12433 2018-03-29 18:51:59.000000 Flask-RESTful-0.3.9/tests/test_inputs.py
+-rw-r--r--   0 josh       (501) staff       (20)    34333 2021-05-17 19:16:30.000000 Flask-RESTful-0.3.9/tests/test_reqparse.py
```

### Comparing `Flask-RESTful-0.3.8/AUTHORS.md` & `Flask-RESTful-0.3.9/AUTHORS.md`

 * *Files identical despite different names*

### Comparing `Flask-RESTful-0.3.8/Flask_RESTful.egg-info/PKG-INFO` & `Flask-RESTful-0.3.9/Flask_RESTful.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Flask-RESTful
-Version: 0.3.8
+Version: 0.3.9
 Summary: Simple framework for creating REST APIs
 Home-page: https://www.github.com/flask-restful/flask-restful/
 Author: Twilio API Team
 Author-email: help@twilio.com
 License: BSD
 Description: UNKNOWN
 Platform: any
```

### Comparing `Flask-RESTful-0.3.8/Flask_RESTful.egg-info/SOURCES.txt` & `Flask-RESTful-0.3.9/Flask_RESTful.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -7,14 +7,15 @@
 setup.py
 Flask_RESTful.egg-info/PKG-INFO
 Flask_RESTful.egg-info/SOURCES.txt
 Flask_RESTful.egg-info/dependency_links.txt
 Flask_RESTful.egg-info/not-zip-safe
 Flask_RESTful.egg-info/requires.txt
 Flask_RESTful.egg-info/top_level.txt
+docs/.fields.rst.swp
 docs/Makefile
 docs/api.rst
 docs/conf.py
 docs/contents.rst.inc
 docs/extending.rst
 docs/fields.rst
 docs/index.rst
```

### Comparing `Flask-RESTful-0.3.8/LICENSE` & `Flask-RESTful-0.3.9/LICENSE`

 * *Files identical despite different names*

### Comparing `Flask-RESTful-0.3.8/Makefile` & `Flask-RESTful-0.3.9/Makefile`

 * *Files identical despite different names*

### Comparing `Flask-RESTful-0.3.8/PKG-INFO` & `Flask-RESTful-0.3.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Flask-RESTful
-Version: 0.3.8
+Version: 0.3.9
 Summary: Simple framework for creating REST APIs
 Home-page: https://www.github.com/flask-restful/flask-restful/
 Author: Twilio API Team
 Author-email: help@twilio.com
 License: BSD
 Description: UNKNOWN
 Platform: any
```

### Comparing `Flask-RESTful-0.3.8/README.md` & `Flask-RESTful-0.3.9/README.md`

 * *Files identical despite different names*

### Comparing `Flask-RESTful-0.3.8/docs/Makefile` & `Flask-RESTful-0.3.9/docs/Makefile`

 * *Files identical despite different names*

### Comparing `Flask-RESTful-0.3.8/docs/_static/flask-restful-small.png` & `Flask-RESTful-0.3.9/docs/_static/flask-restful-small.png`

 * *Files identical despite different names*

### Comparing `Flask-RESTful-0.3.8/docs/_static/flask-restful.png` & `Flask-RESTful-0.3.9/docs/_static/flask-restful.png`

 * *Files identical despite different names*

### Comparing `Flask-RESTful-0.3.8/docs/_templates/sidebarintro.html` & `Flask-RESTful-0.3.9/docs/_templates/sidebarintro.html`

 * *Files identical despite different names*

### Comparing `Flask-RESTful-0.3.8/docs/api.rst` & `Flask-RESTful-0.3.9/docs/api.rst`

 * *Files identical despite different names*

### Comparing `Flask-RESTful-0.3.8/docs/conf.py` & `Flask-RESTful-0.3.9/docs/conf.py`

 * *Files identical despite different names*

### Comparing `Flask-RESTful-0.3.8/docs/contents.rst.inc` & `Flask-RESTful-0.3.9/docs/contents.rst.inc`

 * *Files identical despite different names*

### Comparing `Flask-RESTful-0.3.8/docs/extending.rst` & `Flask-RESTful-0.3.9/docs/extending.rst`

 * *Files identical despite different names*

### Comparing `Flask-RESTful-0.3.8/docs/fields.rst` & `Flask-RESTful-0.3.9/docs/fields.rst`

 * *Files 0% similar despite different names*

```diff
@@ -108,15 +108,15 @@
 bit-field whose individual bits represent distinct values.  You can use fields
 to multiplex a single attribute to multiple output values.
 
 
 This example assumes that bit 1 in the ``flags`` attribute signifies a
 "Normal" or "Urgent" item, and bit 2 signifies "Read" or "Unread".  These
 items might be easy to store in a bitfield, but for a human readable output
-it's nice to convert them to seperate string fields. ::
+it's nice to convert them to separate string fields. ::
 
     class UrgentItem(fields.Raw):
         def format(self, value):
             return "Urgent" if value & 0x01 else "Normal"
 
     class UnreadItem(fields.Raw):
         def format(self, value):
```

### Comparing `Flask-RESTful-0.3.8/docs/installation.rst` & `Flask-RESTful-0.3.9/docs/installation.rst`

 * *Files identical despite different names*

### Comparing `Flask-RESTful-0.3.8/docs/intermediate-usage.rst` & `Flask-RESTful-0.3.9/docs/intermediate-usage.rst`

 * *Files 0% similar despite different names*

```diff
@@ -210,15 +210,15 @@
         'email': fields.String,
         'user_priority': fields.Integer,
         'custom_greeting': fields.FormattedString('Hey there {username}!'),
         'date_created': fields.DateTime,
         'date_updated': fields.DateTime,
         'links': fields.Nested({
             'friends': fields.Url('user_friends', absolute=True),
-            'posts': fields.Url('user_friends', absolute=True),
+            'posts': fields.Url('user_posts', absolute=True),
         }),
     }
 
 First up, there's :class:`fields.FormattedString`. ::
 
     'custom_greeting': fields.FormattedString('Hey there {username}!'),
 
@@ -237,15 +237,15 @@
 we want to create a ``links`` sub-object to contain urls of related objects.
 Note that we passed `fields.Nested` another dict which is built in such a
 way that it would be an acceptable argument to :func:`marshal` by itself.
 
 Finally, we used the :class:`fields.Url` field type. ::
 
         'friends': fields.Url('user_friends', absolute=True),
-        'posts': fields.Url('user_friends', absolute=True),
+        'posts': fields.Url('user_posts', absolute=True),
 
 It takes as its first parameter the name of the endpoint associated with the
 urls of the objects in the ``links`` sub-object.  Passing ``absolute=True``
 ensures that the generated urls will have the hostname included.
 
 
 Passing Constructor Parameters Into Resources
```

### Comparing `Flask-RESTful-0.3.8/docs/make.bat` & `Flask-RESTful-0.3.9/docs/make.bat`

 * *Files identical despite different names*

### Comparing `Flask-RESTful-0.3.8/docs/quickstart.rst` & `Flask-RESTful-0.3.9/docs/quickstart.rst`

 * *Files identical despite different names*

### Comparing `Flask-RESTful-0.3.8/docs/reqparse.rst` & `Flask-RESTful-0.3.9/docs/reqparse.rst`

 * *Files identical despite different names*

### Comparing `Flask-RESTful-0.3.8/docs/testing.rst` & `Flask-RESTful-0.3.9/docs/testing.rst`

 * *Files identical despite different names*

### Comparing `Flask-RESTful-0.3.8/examples/todo.py` & `Flask-RESTful-0.3.9/examples/todo.py`

 * *Files identical despite different names*

### Comparing `Flask-RESTful-0.3.8/examples/todo_simple.py` & `Flask-RESTful-0.3.9/examples/todo_simple.py`

 * *Files identical despite different names*

### Comparing `Flask-RESTful-0.3.8/examples/xml_representation.py` & `Flask-RESTful-0.3.9/examples/xml_representation.py`

 * *Files identical despite different names*

### Comparing `Flask-RESTful-0.3.8/flask_restful/__init__.py` & `Flask-RESTful-0.3.9/flask_restful/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -7,15 +7,14 @@
 from flask.signals import got_request_exception
 from werkzeug.datastructures import Headers
 from werkzeug.exceptions import HTTPException, MethodNotAllowed, NotFound, NotAcceptable, InternalServerError
 from werkzeug.wrappers import Response as ResponseBase
 from flask_restful.utils import http_status_message, unpack, OrderedDict
 from flask_restful.representations.json import output_json
 import sys
-from flask.helpers import _endpoint_from_view_func
 from types import MethodType
 import operator
 try:
     from collections.abc import Mapping
 except ImportError:
     from collections import Mapping
 
@@ -152,15 +151,15 @@
 
         if callable(rule):
             rule = rule(blueprint_setup.url_prefix)
         elif blueprint_setup.url_prefix:
             rule = blueprint_setup.url_prefix + rule
         options.setdefault('subdomain', blueprint_setup.subdomain)
         if endpoint is None:
-            endpoint = _endpoint_from_view_func(view_func)
+            endpoint = view_func.__name__
         defaults = blueprint_setup.url_defaults
         if 'defaults' in options:
             defaults = dict(defaults, **options.pop('defaults'))
         blueprint_setup.app.add_url_rule(rule, '%s.%s' % (blueprint_setup.blueprint.name, endpoint),
                                          view_func, defaults=defaults, **options)
 
     def _deferred_blueprint_init(self, setup_state):
```

### Comparing `Flask-RESTful-0.3.8/flask_restful/fields.py` & `Flask-RESTful-0.3.9/flask_restful/fields.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,20 +1,17 @@
-from datetime import datetime
 from calendar import timegm
-import pytz
 from decimal import Decimal as MyDecimal, ROUND_HALF_EVEN
 from email.utils import formatdate
 import six
 try:
     from urlparse import urlparse, urlunparse
 except ImportError:
     # python3
     from urllib.parse import urlparse, urlunparse
-
-from flask_restful import inputs, marshal
+from flask_restful import marshal
 from flask import url_for, request
 
 __all__ = ["String", "FormattedString", "Url", "DateTime", "Float",
            "Integer", "Arbitrary", "Nested", "List", "Raw", "Boolean",
            "Fixed", "Price"]
```

### Comparing `Flask-RESTful-0.3.8/flask_restful/inputs.py` & `Flask-RESTful-0.3.9/flask_restful/inputs.py`

 * *Files 0% similar despite different names*

```diff
@@ -265,15 +265,15 @@
     :type datetime_str: str
     :return: A datetime
     """
     return datetime.fromtimestamp(mktime_tz(parsedate_tz(datetime_str)), pytz.utc)
 
 
 def datetime_from_iso8601(datetime_str):
-    """Turns an ISO8601 formatted date into a datetime object.
+    """Turns an ISO8601 formatted datetime into a datetime object.
 
     Example::
 
         inputs.datetime_from_iso8601("2012-01-01T23:30:00+02:00")
 
     :param datetime_str: The ISO8601-complying string to transform
     :type datetime_str: str
```

### Comparing `Flask-RESTful-0.3.8/flask_restful/representations/json.py` & `Flask-RESTful-0.3.9/flask_restful/representations/json.py`

 * *Files identical despite different names*

### Comparing `Flask-RESTful-0.3.8/flask_restful/reqparse.py` & `Flask-RESTful-0.3.9/flask_restful/reqparse.py`

 * *Files identical despite different names*

### Comparing `Flask-RESTful-0.3.8/flask_restful/utils/__init__.py` & `Flask-RESTful-0.3.9/flask_restful/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `Flask-RESTful-0.3.8/flask_restful/utils/cors.py` & `Flask-RESTful-0.3.9/flask_restful/utils/cors.py`

 * *Files identical despite different names*

### Comparing `Flask-RESTful-0.3.8/flask_restful/utils/crypto.py` & `Flask-RESTful-0.3.9/flask_restful/utils/crypto.py`

 * *Files identical despite different names*

### Comparing `Flask-RESTful-0.3.8/setup.py` & `Flask-RESTful-0.3.9/setup.py`

 * *Files identical despite different names*

### Comparing `Flask-RESTful-0.3.8/tests/test_accept.py` & `Flask-RESTful-0.3.9/tests/test_accept.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,12 +1,11 @@
 import unittest
 from flask import Flask
 import flask_restful
 from werkzeug import exceptions
-from nose.tools import assert_equals
 
 
 
 class AcceptTestCase(unittest.TestCase):
 
     def test_accept_default_application_json(self):
 
@@ -17,16 +16,16 @@
         app = Flask(__name__)
         api = flask_restful.Api(app)
 
         api.add_resource(Foo, '/')
 
         with app.test_client() as client:
             res = client.get('/', headers=[('Accept', 'application/json')])
-            assert_equals(res.status_code, 200)
-            assert_equals(res.content_type, 'application/json')
+            self.assertEqual(res.status_code, 200)
+            self.assertEqual(res.content_type, 'application/json')
 
 
     def test_accept_no_default_match_acceptable(self):
 
         class Foo(flask_restful.Resource):
             def get(self):
                 return "data"
@@ -34,16 +33,16 @@
         app = Flask(__name__)
         api = flask_restful.Api(app, default_mediatype=None)
 
         api.add_resource(Foo, '/')
 
         with app.test_client() as client:
             res = client.get('/', headers=[('Accept', 'application/json')])
-            assert_equals(res.status_code, 200)
-            assert_equals(res.content_type, 'application/json')
+            self.assertEqual(res.status_code, 200)
+            self.assertEqual(res.content_type, 'application/json')
 
 
     def test_accept_default_override_accept(self):
 
         class Foo(flask_restful.Resource):
             def get(self):
                 return "data"
@@ -51,16 +50,16 @@
         app = Flask(__name__)
         api = flask_restful.Api(app)
 
         api.add_resource(Foo, '/')
 
         with app.test_client() as client:
             res = client.get('/', headers=[('Accept', 'text/plain')])
-            assert_equals(res.status_code, 200)
-            assert_equals(res.content_type, 'application/json')
+            self.assertEqual(res.status_code, 200)
+            self.assertEqual(res.content_type, 'application/json')
 
 
     def test_accept_default_any_pick_first(self):
 
         class Foo(flask_restful.Resource):
             def get(self):
                 return "data"
@@ -73,16 +72,16 @@
             resp = app.make_response((str(data), status_code, headers))
             return resp
 
         api.add_resource(Foo, '/')
 
         with app.test_client() as client:
             res = client.get('/', headers=[('Accept', '*/*')])
-            assert_equals(res.status_code, 200)
-            assert_equals(res.content_type, 'application/json')
+            self.assertEqual(res.status_code, 200)
+            self.assertEqual(res.content_type, 'application/json')
 
 
     def test_accept_no_default_no_match_not_acceptable(self):
 
         class Foo(flask_restful.Resource):
             def get(self):
                 return "data"
@@ -90,16 +89,16 @@
         app = Flask(__name__)
         api = flask_restful.Api(app, default_mediatype=None)
 
         api.add_resource(Foo, '/')
 
         with app.test_client() as client:
             res = client.get('/', headers=[('Accept', 'text/plain')])
-            assert_equals(res.status_code, 406)
-            assert_equals(res.content_type, 'application/json')
+            self.assertEqual(res.status_code, 406)
+            self.assertEqual(res.content_type, 'application/json')
 
 
     def test_accept_no_default_custom_repr_match(self):
 
         class Foo(flask_restful.Resource):
             def get(self):
                 return "data"
@@ -113,16 +112,16 @@
             resp = app.make_response((str(data), status_code, headers))
             return resp
 
         api.add_resource(Foo, '/')
 
         with app.test_client() as client:
             res = client.get('/', headers=[('Accept', 'text/plain')])
-            assert_equals(res.status_code, 200)
-            assert_equals(res.content_type, 'text/plain')
+            self.assertEqual(res.status_code, 200)
+            self.assertEqual(res.content_type, 'text/plain')
 
 
     def test_accept_no_default_custom_repr_not_acceptable(self):
 
         class Foo(flask_restful.Resource):
             def get(self):
                 return "data"
@@ -136,16 +135,16 @@
             resp = app.make_response((str(data), status_code, headers))
             return resp
 
         api.add_resource(Foo, '/')
 
         with app.test_client() as client:
             res = client.get('/', headers=[('Accept', 'application/json')])
-            assert_equals(res.status_code, 406)
-            assert_equals(res.content_type, 'text/plain')
+            self.assertEqual(res.status_code, 406)
+            self.assertEqual(res.content_type, 'text/plain')
 
 
     def test_accept_no_default_match_q0_not_acceptable(self):
         """
         q=0 should be considered NotAcceptable,
         but this depends on werkzeug >= 1.0 which is not yet released
         so this test is expected to fail until we depend on werkzeug >= 1.0
@@ -157,16 +156,16 @@
         app = Flask(__name__)
         api = flask_restful.Api(app, default_mediatype=None)
 
         api.add_resource(Foo, '/')
 
         with app.test_client() as client:
             res = client.get('/', headers=[('Accept', 'application/json; q=0')])
-            assert_equals(res.status_code, 406)
-            assert_equals(res.content_type, 'application/json')
+            self.assertEqual(res.status_code, 406)
+            self.assertEqual(res.content_type, 'application/json')
 
     def test_accept_no_default_accept_highest_quality_of_two(self):
         class Foo(flask_restful.Resource):
             def get(self):
                 return "data"
 
         app = Flask(__name__)
@@ -177,16 +176,16 @@
             resp = app.make_response((str(data), status_code, headers))
             return resp
 
         api.add_resource(Foo, '/')
 
         with app.test_client() as client:
             res = client.get('/', headers=[('Accept', 'application/json; q=0.1, text/plain; q=1.0')])
-            assert_equals(res.status_code, 200)
-            assert_equals(res.content_type, 'text/plain')
+            self.assertEqual(res.status_code, 200)
+            self.assertEqual(res.content_type, 'text/plain')
 
 
     def test_accept_no_default_accept_highest_quality_of_three(self):
         class Foo(flask_restful.Resource):
             def get(self):
                 return "data"
 
@@ -199,16 +198,16 @@
             resp = app.make_response((str(data), status_code, headers))
             return resp
 
         api.add_resource(Foo, '/')
 
         with app.test_client() as client:
             res = client.get('/', headers=[('Accept', 'application/json; q=0.1, text/plain; q=0.3, text/html; q=0.2')])
-            assert_equals(res.status_code, 200)
-            assert_equals(res.content_type, 'text/plain')
+            self.assertEqual(res.status_code, 200)
+            self.assertEqual(res.content_type, 'text/plain')
 
 
     def test_accept_no_default_no_representations(self):
 
         class Foo(flask_restful.Resource):
             def get(self):
                 return "data"
@@ -217,16 +216,16 @@
         api = flask_restful.Api(app, default_mediatype=None)
         api.representations = {}
 
         api.add_resource(Foo, '/')
 
         with app.test_client() as client:
             res = client.get('/', headers=[('Accept', 'text/plain')])
-            assert_equals(res.status_code, 406)
-            assert_equals(res.content_type, 'text/plain')
+            self.assertEqual(res.status_code, 406)
+            self.assertEqual(res.content_type, 'text/plain')
 
     def test_accept_invalid_default_no_representations(self):
 
         class Foo(flask_restful.Resource):
             def get(self):
                 return "data"
 
@@ -234,8 +233,8 @@
         api = flask_restful.Api(app, default_mediatype='nonexistant/mediatype')
         api.representations = {}
 
         api.add_resource(Foo, '/')
 
         with app.test_client() as client:
             res = client.get('/', headers=[('Accept', 'text/plain')])
-            assert_equals(res.status_code, 500)
+            self.assertEqual(res.status_code, 500)
```

### Comparing `Flask-RESTful-0.3.8/tests/test_api.py` & `Flask-RESTful-0.3.9/tests/test_api.py`

 * *Files 2% similar despite different names*

```diff
@@ -12,21 +12,20 @@
 from werkzeug.exceptions import HTTPException, Unauthorized, BadRequest, NotFound, _aborter
 from werkzeug.http import quote_etag, unquote_etag
 from flask_restful.utils import http_status_message, unpack
 import flask_restful
 import flask_restful.fields
 from flask_restful import OrderedDict
 from json import dumps, loads, JSONEncoder
-#noinspection PyUnresolvedReferences
-from nose.tools import assert_equals, assert_true, assert_false  # you need it for tests in form of continuations
+from nose.tools import assert_equal  # you need it for tests in form of continuations
 import six
 
 
 def check_unpack(expected, value):
-    assert_equals(expected, value)
+    assert_equal(expected, value)
 
 
 def test_unpack():
     yield check_unpack, ("hey", 200, {}), unpack("hey")
     yield check_unpack, (("hey",), 200, {}), unpack(("hey",))
     yield check_unpack, ("hey", 201, {}), unpack(("hey", 201))
     yield check_unpack, ("hey", 201, "foo"), unpack(("hey", 201, "foo"))
@@ -48,91 +47,91 @@
     def get(self):
         raise BadMojoError("It burns..")
 
 
 class APITestCase(unittest.TestCase):
 
     def test_http_code(self):
-        self.assertEquals(http_status_message(200), 'OK')
-        self.assertEquals(http_status_message(404), 'Not Found')
+        self.assertEqual(http_status_message(200), 'OK')
+        self.assertEqual(http_status_message(404), 'Not Found')
 
     def test_unauthorized_no_challenge_by_default(self):
         app = Flask(__name__)
         api = flask_restful.Api(app)
         response = Mock()
         response.headers = {}
         with app.test_request_context('/foo'):
             response = api.unauthorized(response)
-        assert_false('WWW-Authenticate' in response.headers)
+        self.assertFalse('WWW-Authenticate' in response.headers)
 
     def test_unauthorized(self):
         app = Flask(__name__)
         api = flask_restful.Api(app, serve_challenge_on_401=True)
         response = Mock()
         response.headers = {}
         with app.test_request_context('/foo'):
             response = api.unauthorized(response)
-        self.assertEquals(response.headers['WWW-Authenticate'],
+        self.assertEqual(response.headers['WWW-Authenticate'],
                           'Basic realm="flask-restful"')
 
     def test_unauthorized_custom_realm(self):
         app = Flask(__name__)
         app.config['HTTP_BASIC_AUTH_REALM'] = 'Foo'
         api = flask_restful.Api(app, serve_challenge_on_401=True)
         response = Mock()
         response.headers = {}
         with app.test_request_context('/foo'):
             response = api.unauthorized(response)
-        self.assertEquals(response.headers['WWW-Authenticate'], 'Basic realm="Foo"')
+        self.assertEqual(response.headers['WWW-Authenticate'], 'Basic realm="Foo"')
 
     def test_handle_error_401_sends_challege_default_realm(self):
         app = Flask(__name__)
         api = flask_restful.Api(app, serve_challenge_on_401=True)
         exception = HTTPException()
         exception.code = 401
         exception.data = {'foo': 'bar'}
 
         with app.test_request_context('/foo'):
             resp = api.handle_error(exception)
-            self.assertEquals(resp.status_code, 401)
-            self.assertEquals(resp.headers['WWW-Authenticate'],
+            self.assertEqual(resp.status_code, 401)
+            self.assertEqual(resp.headers['WWW-Authenticate'],
                               'Basic realm="flask-restful"')
 
     def test_handle_error_401_sends_challege_configured_realm(self):
         app = Flask(__name__)
         app.config['HTTP_BASIC_AUTH_REALM'] = 'test-realm'
         api = flask_restful.Api(app, serve_challenge_on_401=True)
 
         with app.test_request_context('/foo'):
             resp = api.handle_error(Unauthorized())
-            self.assertEquals(resp.status_code, 401)
-            self.assertEquals(resp.headers['WWW-Authenticate'],
+            self.assertEqual(resp.status_code, 401)
+            self.assertEqual(resp.headers['WWW-Authenticate'],
                               'Basic realm="test-realm"')
 
     def test_handle_error_does_not_swallow_exceptions(self):
         app = Flask(__name__)
         api = flask_restful.Api(app)
         exception = BadRequest('x')
 
         with app.test_request_context('/foo'):
             resp = api.handle_error(exception)
-            self.assertEquals(resp.status_code, 400)
-            self.assertEquals(resp.get_data(), b'{"message": "x"}\n')
+            self.assertEqual(resp.status_code, 400)
+            self.assertEqual(resp.get_data(), b'{"message": "x"}\n')
 
 
     def test_handle_error_does_not_swallow_custom_exceptions(self):
         app = Flask(__name__)
         errors = {'BadMojoError': {'status': 409, 'message': 'go away'}}
         api = flask_restful.Api(app, errors=errors)
         api.add_resource(HelloBomb, '/bomb')
 
         app = app.test_client()
         resp = app.get('/bomb')
-        self.assertEquals(resp.status_code, 409)
-        self.assertEquals(resp.content_type, api.default_mediatype)
+        self.assertEqual(resp.status_code, 409)
+        self.assertEqual(resp.content_type, api.default_mediatype)
         resp_dict = json.loads(resp.data.decode())
         self.assertEqual(resp_dict.get('status'), 409)
         self.assertEqual(resp_dict.get('message'), 'go away')
 
     def test_handle_error_does_not_swallow_abort_response(self):
 
         class HelloBombAbort(flask_restful.Resource):
@@ -144,151 +143,151 @@
         api.add_resource(HelloBombAbort, '/bomb')
 
         app = app.test_client()
         resp = app.get('/bomb')
 
         resp_dict = json.loads(resp.data.decode())
 
-        self.assertEquals(resp.status_code, 403)
+        self.assertEqual(resp.status_code, 403)
         self.assertDictEqual(resp_dict, {})
 
     def test_marshal(self):
         fields = OrderedDict([('foo', flask_restful.fields.Raw)])
         marshal_dict = OrderedDict([('foo', 'bar'), ('bat', 'baz')])
         output = flask_restful.marshal(marshal_dict, fields)
-        self.assertEquals(output, {'foo': 'bar'})
+        self.assertEqual(output, {'foo': 'bar'})
 
     def test_marshal_with_envelope(self):
         fields = OrderedDict([('foo', flask_restful.fields.Raw)])
         marshal_dict = OrderedDict([('foo', 'bar'), ('bat', 'baz')])
         output = flask_restful.marshal(marshal_dict, fields, envelope='hey')
-        self.assertEquals(output, {'hey': {'foo': 'bar'}})
+        self.assertEqual(output, {'hey': {'foo': 'bar'}})
 
     def test_marshal_decorator(self):
         fields = OrderedDict([('foo', flask_restful.fields.Raw)])
 
         @flask_restful.marshal_with(fields)
         def try_me():
             return OrderedDict([('foo', 'bar'), ('bat', 'baz')])
-        self.assertEquals(try_me(), {'foo': 'bar'})
+        self.assertEqual(try_me(), {'foo': 'bar'})
 
     def test_marshal_decorator_with_envelope(self):
         fields = OrderedDict([('foo', flask_restful.fields.Raw)])
 
         @flask_restful.marshal_with(fields, envelope='hey')
         def try_me():
             return OrderedDict([('foo', 'bar'), ('bat', 'baz')])
 
-        self.assertEquals(try_me(), {'hey': {'foo': 'bar'}})
+        self.assertEqual(try_me(), {'hey': {'foo': 'bar'}})
 
     def test_marshal_decorator_tuple(self):
         fields = OrderedDict([('foo', flask_restful.fields.Raw)])
 
         @flask_restful.marshal_with(fields)
         def try_me():
             return OrderedDict([('foo', 'bar'), ('bat', 'baz')]), 200, {'X-test': 123}
-        self.assertEquals(try_me(), ({'foo': 'bar'}, 200, {'X-test': 123}))
+        self.assertEqual(try_me(), ({'foo': 'bar'}, 200, {'X-test': 123}))
 
     def test_marshal_decorator_tuple_with_envelope(self):
         fields = OrderedDict([('foo', flask_restful.fields.Raw)])
 
         @flask_restful.marshal_with(fields, envelope='hey')
         def try_me():
             return OrderedDict([('foo', 'bar'), ('bat', 'baz')]), 200, {'X-test': 123}
 
-        self.assertEquals(try_me(), ({'hey': {'foo': 'bar'}}, 200, {'X-test': 123}))
+        self.assertEqual(try_me(), ({'hey': {'foo': 'bar'}}, 200, {'X-test': 123}))
 
     def test_marshal_field_decorator(self):
         field = flask_restful.fields.Raw
 
         @flask_restful.marshal_with_field(field)
         def try_me():
             return 'foo'
-        self.assertEquals(try_me(), 'foo')
+        self.assertEqual(try_me(), 'foo')
 
     def test_marshal_field_decorator_tuple(self):
         field = flask_restful.fields.Raw
 
         @flask_restful.marshal_with_field(field)
         def try_me():
             return 'foo', 200, {'X-test': 123}
-        self.assertEquals(('foo', 200, {'X-test': 123}), try_me())
+        self.assertEqual(('foo', 200, {'X-test': 123}), try_me())
 
     def test_marshal_field(self):
         fields = OrderedDict({'foo': flask_restful.fields.Raw()})
         marshal_fields = OrderedDict([('foo', 'bar'), ('bat', 'baz')])
         output = flask_restful.marshal(marshal_fields, fields)
-        self.assertEquals(output, {'foo': 'bar'})
+        self.assertEqual(output, {'foo': 'bar'})
 
     def test_marshal_tuple(self):
         fields = OrderedDict({'foo': flask_restful.fields.Raw})
         marshal_fields = OrderedDict([('foo', 'bar'), ('bat', 'baz')])
         output = flask_restful.marshal((marshal_fields,), fields)
-        self.assertEquals(output, [{'foo': 'bar'}])
+        self.assertEqual(output, [{'foo': 'bar'}])
 
     def test_marshal_tuple_with_envelope(self):
         fields = OrderedDict({'foo': flask_restful.fields.Raw})
         marshal_fields = OrderedDict([('foo', 'bar'), ('bat', 'baz')])
         output = flask_restful.marshal((marshal_fields,), fields, envelope='hey')
-        self.assertEquals(output, {'hey': [{'foo': 'bar'}]})
+        self.assertEqual(output, {'hey': [{'foo': 'bar'}]})
 
     def test_marshal_nested(self):
         fields = OrderedDict([
             ('foo', flask_restful.fields.Raw),
             ('fee', flask_restful.fields.Nested({
                 'fye': flask_restful.fields.String,
             }))
         ])
 
         marshal_fields = OrderedDict([('foo', 'bar'), ('bat', 'baz'), ('fee', {'fye': 'fum'})])
         output = flask_restful.marshal(marshal_fields, fields)
         expected = OrderedDict([('foo', 'bar'), ('fee', OrderedDict([('fye', 'fum')]))])
-        self.assertEquals(output, expected)
+        self.assertEqual(output, expected)
 
     def test_marshal_nested_with_non_null(self):
         fields = OrderedDict([
             ('foo', flask_restful.fields.Raw),
             ('fee', flask_restful.fields.Nested(
                 OrderedDict([
                     ('fye', flask_restful.fields.String),
                     ('blah', flask_restful.fields.String)
                 ]), allow_null=False))
         ])
         marshal_fields = [OrderedDict([('foo', 'bar'), ('bat', 'baz'), ('fee', None)])]
         output = flask_restful.marshal(marshal_fields, fields)
         expected = [OrderedDict([('foo', 'bar'), ('fee', OrderedDict([('fye', None), ('blah', None)]))])]
-        self.assertEquals(output, expected)
+        self.assertEqual(output, expected)
 
     def test_marshal_nested_with_null(self):
         fields = OrderedDict([
             ('foo', flask_restful.fields.Raw),
             ('fee', flask_restful.fields.Nested(
                 OrderedDict([
                     ('fye', flask_restful.fields.String),
                     ('blah', flask_restful.fields.String)
                 ]), allow_null=True))
         ])
         marshal_fields = OrderedDict([('foo', 'bar'), ('bat', 'baz'), ('fee', None)])
         output = flask_restful.marshal(marshal_fields, fields)
         expected = OrderedDict([('foo', 'bar'), ('fee', None)])
-        self.assertEquals(output, expected)
+        self.assertEqual(output, expected)
 
     def test_allow_null_presents_data(self):
         fields = OrderedDict([
             ('foo', flask_restful.fields.Raw),
             ('fee', flask_restful.fields.Nested(
                 OrderedDict([
                     ('fye', flask_restful.fields.String),
                     ('blah', flask_restful.fields.String)
                 ]), allow_null=True))
         ])
         marshal_fields = OrderedDict([('foo', 'bar'), ('bat', 'baz'), ('fee', {'blah': 'cool'})])
         output = flask_restful.marshal(marshal_fields, fields)
         expected = OrderedDict([('foo', 'bar'), ('fee', OrderedDict([('fye', None), ('blah', 'cool')]))])
-        self.assertEquals(output, expected)
+        self.assertEqual(output, expected)
 
     def test_marshal_nested_property(self):
         class TestObject(object):
             @property
             def fee(self):
                 return {'blah': 'cool'}
         fields = OrderedDict([
@@ -300,128 +299,128 @@
                 ]), allow_null=True))
         ])
         obj = TestObject()
         obj.foo = 'bar'
         obj.bat = 'baz'
         output = flask_restful.marshal([obj], fields)
         expected = [OrderedDict([('foo', 'bar'), ('fee', OrderedDict([('fye', None), ('blah', 'cool')]))])]
-        self.assertEquals(output, expected)
+        self.assertEqual(output, expected)
 
     def test_marshal_list(self):
         fields = OrderedDict([
             ('foo', flask_restful.fields.Raw),
             ('fee', flask_restful.fields.List(flask_restful.fields.String))
         ])
         marshal_fields = OrderedDict([('foo', 'bar'), ('bat', 'baz'), ('fee', ['fye', 'fum'])])
         output = flask_restful.marshal(marshal_fields, fields)
         expected = OrderedDict([('foo', 'bar'), ('fee', (['fye', 'fum']))])
-        self.assertEquals(output, expected)
+        self.assertEqual(output, expected)
 
     def test_marshal_list_of_nesteds(self):
         fields = OrderedDict([
             ('foo', flask_restful.fields.Raw),
             ('fee', flask_restful.fields.List(flask_restful.fields.Nested({
                 'fye': flask_restful.fields.String
             })))
         ])
         marshal_fields = OrderedDict([('foo', 'bar'), ('bat', 'baz'), ('fee', {'fye': 'fum'})])
         output = flask_restful.marshal(marshal_fields, fields)
         expected = OrderedDict([('foo', 'bar'), ('fee', [OrderedDict([('fye', 'fum')])])])
-        self.assertEquals(output, expected)
+        self.assertEqual(output, expected)
 
     def test_marshal_list_of_lists(self):
         fields = OrderedDict([
             ('foo', flask_restful.fields.Raw),
             ('fee', flask_restful.fields.List(flask_restful.fields.List(
                 flask_restful.fields.String)))
         ])
         marshal_fields = OrderedDict([('foo', 'bar'), ('bat', 'baz'), ('fee', [['fye'], ['fum']])])
         output = flask_restful.marshal(marshal_fields, fields)
         expected = OrderedDict([('foo', 'bar'), ('fee', [['fye'], ['fum']])])
-        self.assertEquals(output, expected)
+        self.assertEqual(output, expected)
 
     def test_marshal_nested_dict(self):
         fields = OrderedDict([
             ('foo', flask_restful.fields.Raw),
             ('bar', OrderedDict([
                 ('a', flask_restful.fields.Raw),
                 ('b', flask_restful.fields.Raw),
             ])),
         ])
         marshal_fields = OrderedDict([('foo', 'foo-val'), ('bar', 'bar-val'), ('bat', 'bat-val'),
                                       ('a', 1), ('b', 2), ('c', 3)])
         output = flask_restful.marshal(marshal_fields, fields)
         expected = OrderedDict([('foo', 'foo-val'), ('bar', OrderedDict([('a', 1), ('b', 2)]))])
-        self.assertEquals(output, expected)
+        self.assertEqual(output, expected)
 
     def test_api_representation(self):
         app = Mock()
         api = flask_restful.Api(app)
 
         @api.representation('foo')
         def foo():
             pass
 
-        self.assertEquals(api.representations['foo'], foo)
+        self.assertEqual(api.representations['foo'], foo)
 
     def test_api_base(self):
         app = Mock()
         app.configure_mock(**{'record.side_effect': AttributeError})
         api = flask_restful.Api(app)
-        self.assertEquals(api.urls, {})
-        self.assertEquals(api.prefix, '')
-        self.assertEquals(api.default_mediatype, 'application/json')
+        self.assertEqual(api.urls, {})
+        self.assertEqual(api.prefix, '')
+        self.assertEqual(api.default_mediatype, 'application/json')
 
     def test_api_delayed_initialization(self):
         app = Flask(__name__)
         api = flask_restful.Api()
         api.add_resource(HelloWorld, '/', endpoint="hello")
         api.init_app(app)
         with app.test_client() as client:
-            self.assertEquals(client.get('/').status_code, 200)
+            self.assertEqual(client.get('/').status_code, 200)
 
     def test_api_prefix(self):
         app = Mock()
         app.configure_mock(**{'record.side_effect': AttributeError})
         api = flask_restful.Api(app, prefix='/foo')
-        self.assertEquals(api.prefix, '/foo')
+        self.assertEqual(api.prefix, '/foo')
 
     def test_handle_server_error(self):
         app = Flask(__name__)
         api = flask_restful.Api(app)
 
         with app.test_request_context("/foo"):
             resp = api.handle_error(Exception())
-            self.assertEquals(resp.status_code, 500)
-            self.assertEquals(resp.data.decode(), dumps({
+            self.assertEqual(resp.status_code, 500)
+            self.assertEqual(resp.data.decode(), dumps({
                 "message": "Internal Server Error"
             }) + "\n")
 
     def test_handle_error_with_code(self):
         app = Flask(__name__)
         api = flask_restful.Api(app, serve_challenge_on_401=True)
 
         exception = Exception()
         exception.code = "Not an integer"
         exception.data = {'foo': 'bar'}
 
         with app.test_request_context("/foo"):
             resp = api.handle_error(exception)
-            self.assertEquals(resp.status_code, 500)
-            self.assertEquals(resp.data.decode(), dumps({"foo": "bar"}) + "\n")
+            self.assertEqual(resp.status_code, 500)
+            self.assertEqual(resp.data.decode(), dumps({"foo": "bar"}) + "\n")
 
     def test_handle_auth(self):
         app = Flask(__name__)
         api = flask_restful.Api(app, serve_challenge_on_401=True)
 
         with app.test_request_context("/foo"):
             resp = api.handle_error(Unauthorized())
-            self.assertEquals(resp.status_code, 401)
+            self.assertEqual(resp.status_code, 401)
             expected_data = dumps({'message': Unauthorized.description}) + "\n"
-            self.assertEquals(resp.data.decode(), expected_data)
+            self.assertEqual(resp.data.decode(), expected_data)
 
             self.assertTrue('WWW-Authenticate' in resp.headers)
 
     def test_handle_api_error(self):
         app = Flask(__name__)
         api = flask_restful.Api(app)
 
@@ -429,35 +428,37 @@
             def get(self):
                 flask.abort(404)
 
         api.add_resource(Test(), '/api', endpoint='api')
         app = app.test_client()
 
         resp = app.get("/api")
-        assert_equals(resp.status_code, 404)
-        assert_equals('application/json', resp.headers['Content-Type'])
+        self.assertEqual(resp.status_code, 404)
+        self.assertEqual('application/json', resp.headers['Content-Type'])
         data = loads(resp.data.decode())
-        assert_true('message' in data)
+        self.assertTrue('message' in data)
 
     def test_handle_non_api_error(self):
         app = Flask(__name__)
         flask_restful.Api(app)
         app = app.test_client()
 
         resp = app.get("/foo")
-        self.assertEquals(resp.status_code, 404)
-        self.assertEquals('text/html', resp.headers['Content-Type'])
+        self.assertEqual(resp.status_code, 404)
+        # in newer versions of werkzeug this is `text/html; charset=utf8`
+        content_type, _, _ = resp.headers['Content-Type'].partition(';')
+        self.assertEqual('text/html', content_type)
 
     def test_non_api_error_404_catchall(self):
         app = Flask(__name__)
         api = flask_restful.Api(app, catch_all_404s=True)
         app = app.test_client()
 
         resp = app.get("/foo")
-        self.assertEquals(api.default_mediatype, resp.headers['Content-Type'])
+        self.assertEqual(api.default_mediatype, resp.headers['Content-Type'])
 
     def test_handle_error_signal(self):
         if not signals_available:
             # This test requires the blinker lib to run.
             print("Can't test signals without signal support")
             return
         app = Flask(__name__)
@@ -470,27 +471,27 @@
         def record(sender, exception):
             recorded.append(exception)
 
         got_request_exception.connect(record, app)
         try:
             with app.test_request_context("/foo"):
                 api.handle_error(exception)
-                self.assertEquals(len(recorded), 1)
+                self.assertEqual(len(recorded), 1)
                 self.assertTrue(exception is recorded[0])
         finally:
             got_request_exception.disconnect(record, app)
 
     def test_handle_error(self):
         app = Flask(__name__)
         api = flask_restful.Api(app)
 
         with app.test_request_context("/foo"):
             resp = api.handle_error(BadRequest())
-            self.assertEquals(resp.status_code, 400)
-            self.assertEquals(resp.data.decode(), dumps({
+            self.assertEqual(resp.status_code, 400)
+            self.assertEqual(resp.data.decode(), dumps({
                 'message': BadRequest.description,
             }) + "\n")
 
     def test_error_router_falls_back_to_original(self):
         """Verify that if an exception occurs in the Flask-RESTful error handler,
         the error_router will call the original flask error handler instead.
         """
@@ -509,34 +510,34 @@
     def test_media_types(self):
         app = Flask(__name__)
         api = flask_restful.Api(app)
 
         with app.test_request_context("/foo", headers={
             'Accept': 'application/json'
         }):
-            self.assertEquals(api.mediatypes(), ['application/json'])
+            self.assertEqual(api.mediatypes(), ['application/json'])
 
     def test_media_types_method(self):
         app = Flask(__name__)
         api = flask_restful.Api(app)
 
         with app.test_request_context("/foo", headers={
             'Accept': 'application/xml; q=.5'
         }):
-            self.assertEquals(api.mediatypes_method()(Mock()),
+            self.assertEqual(api.mediatypes_method()(Mock()),
                               ['application/xml', 'application/json'])
 
     def test_media_types_q(self):
         app = Flask(__name__)
         api = flask_restful.Api(app)
 
         with app.test_request_context("/foo", headers={
             'Accept': 'application/json; q=1, application/xml; q=.5'
         }):
-            self.assertEquals(api.mediatypes(),
+            self.assertEqual(api.mediatypes(),
                               ['application/json', 'application/xml'])
 
     def test_decorator(self):
         def return_zero(func):
             return 0
 
         app = Mock(flask.Flask)
@@ -584,17 +585,17 @@
                 return 'foo1'
 
         api.add_resource(Foo1, '/foo', endpoint='bar')
         api.add_resource(Foo1, '/foo/toto', endpoint='blah')
 
         with app.test_client() as client:
             foo1 = client.get('/foo')
-            self.assertEquals(foo1.data, b'"foo1"\n')
+            self.assertEqual(foo1.data, b'"foo1"\n')
             foo2 = client.get('/foo/toto')
-            self.assertEquals(foo2.data, b'"foo1"\n')
+            self.assertEqual(foo2.data, b'"foo1"\n')
 
     def test_add_resource(self):
         app = Mock(flask.Flask)
         app.view_functions = {}
         api = flask_restful.Api(app)
         api.output = Mock()
         api.add_resource(views.MethodView, '/foo')
@@ -640,43 +641,43 @@
 
         api.add_resource(Foo, '/foo',
                 resource_class_args=('wonderful',),
                 resource_class_kwargs={'secret_state': 'slurm'})
 
         with app.test_client() as client:
             foo = client.get('/foo')
-            self.assertEquals(foo.data, b'"wonderful slurm"\n')
+            self.assertEqual(foo.data, b'"wonderful slurm"\n')
 
     def test_output_unpack(self):
 
         def make_empty_response():
             return {'foo': 'bar'}
 
         app = Flask(__name__)
         api = flask_restful.Api(app)
 
         with app.test_request_context("/foo"):
             wrapper = api.output(make_empty_response)
             resp = wrapper()
-            self.assertEquals(resp.status_code, 200)
-            self.assertEquals(resp.data.decode(), '{"foo": "bar"}\n')
+            self.assertEqual(resp.status_code, 200)
+            self.assertEqual(resp.data.decode(), '{"foo": "bar"}\n')
 
     def test_output_func(self):
 
         def make_empty_response():
             return flask.make_response('')
 
         app = Flask(__name__)
         api = flask_restful.Api(app)
 
         with app.test_request_context("/foo"):
             wrapper = api.output(make_empty_response)
             resp = wrapper()
-            self.assertEquals(resp.status_code, 200)
-            self.assertEquals(resp.data.decode(), '')
+            self.assertEqual(resp.status_code, 200)
+            self.assertEqual(resp.data.decode(), '')
 
     def test_resource(self):
         app = Flask(__name__)
         resource = flask_restful.Resource()
         resource.get = Mock()
         with app.test_request_context("/foo"):
             resource.dispatch_request()
@@ -703,15 +704,15 @@
 
             def get(self):
                 return 'hello'
 
         with app.test_request_context("/foo", headers={'Accept': 'text/plain'}):
             resource = Foo()
             resp = resource.dispatch_request()
-            self.assertEquals(resp.data.decode(), 'hello')
+            self.assertEqual(resp.data.decode(), 'hello')
 
     def test_resource_error(self):
         app = Flask(__name__)
         resource = flask_restful.Resource()
         with app.test_request_context("/foo"):
             self.assertRaises(AssertionError, lambda: resource.dispatch_request())
 
@@ -722,29 +723,29 @@
             self.assertRaises(AssertionError, lambda: resource.dispatch_request())
 
     def test_abort_data(self):
         try:
             flask_restful.abort(404, foo='bar')
             assert False  # We should never get here
         except Exception as e:
-            self.assertEquals(e.data, {'foo': 'bar'})
+            self.assertEqual(e.data, {'foo': 'bar'})
 
     def test_abort_no_data(self):
         try:
             flask_restful.abort(404)
             assert False  # We should never get here
         except Exception as e:
-            self.assertEquals(False, hasattr(e, "data"))
+            self.assertEqual(False, hasattr(e, "data"))
 
     def test_abort_custom_message(self):
         try:
             flask_restful.abort(404, message="no user")
             assert False  # We should never get here
         except Exception as e:
-            assert_equals(e.data['message'], "no user")
+            self.assertEqual(e.data['message'], "no user")
 
     def test_abort_type(self):
         self.assertRaises(HTTPException, lambda: flask_restful.abort(404))
 
     def test_endpoints(self):
         app = Flask(__name__)
         api = flask_restful.Api(app)
@@ -776,20 +777,20 @@
 
     def test_fr_405(self):
         app = Flask(__name__)
         api = flask_restful.Api(app)
         api.add_resource(HelloWorld, '/ids/<int:id>', endpoint="hello")
         app = app.test_client()
         resp = app.post('/ids/3')
-        self.assertEquals(resp.status_code, 405)
-        self.assertEquals(resp.content_type, api.default_mediatype)
+        self.assertEqual(resp.status_code, 405)
+        self.assertEqual(resp.content_type, api.default_mediatype)
         # Allow can be of the form 'GET, PUT, POST'
         allow = ', '.join(set(resp.headers.get_all('Allow')))
         allow = set(method.strip() for method in allow.split(','))
-        self.assertEquals(allow,
+        self.assertEqual(allow,
                           {'HEAD', 'OPTIONS'}.union(HelloWorld.methods))
 
     def test_exception_header_forwarded(self):
         """Test that HTTPException's headers are extended properly"""
         app = Flask(__name__)
         app.config['DEBUG'] = True
         api = flask_restful.Api(app)
@@ -810,15 +811,15 @@
                 flask_abort(304, etag='myETag')
 
         api.add_resource(Foo1, '/foo')
         _aborter.mapping.update({304: NotModified})
 
         with app.test_client() as client:
             foo = client.get('/foo')
-            self.assertEquals(foo.get_etag(),
+            self.assertEqual(foo.get_etag(),
                               unquote_etag(quote_etag('myETag')))
 
     def test_exception_header_forwarding_doesnt_duplicate_headers(self):
         """Test that HTTPException's headers do not add a duplicate
         Content-Length header
 
         https://github.com/flask-restful/flask-restful/issues/534
@@ -846,18 +847,18 @@
             foo = client.get('/foo')
 
             # Python's dictionaries have random order (as of "new" Pythons,
             # anyway), so we can't verify the actual output here.  We just
             # assert that they're properly prettyprinted.
             lines = foo.data.splitlines()
             lines = [line.decode() for line in lines]
-            self.assertEquals("{", lines[0])
+            self.assertEqual("{", lines[0])
             self.assertTrue(lines[1].startswith('    '))
             self.assertTrue(lines[2].startswith('    '))
-            self.assertEquals("}", lines[3])
+            self.assertEqual("}", lines[3])
 
             # Assert our trailing newline.
             self.assertTrue(foo.data.endswith(b'\n'))
 
     def test_read_json_settings_from_config(self):
         class TestConfig(object):
             RESTFUL_JSON = {'indent': 2,
@@ -875,15 +876,15 @@
         api.add_resource(Foo, '/foo')
 
         with app.test_client() as client:
             data = client.get('/foo').data
 
         expected = b'{\n  "baz": "qux", \n  "foo": "bar"\n}\n'
 
-        self.assertEquals(data, expected)
+        self.assertEqual(data, expected)
 
 
     def test_use_custom_jsonencoder(self):
         class CabageEncoder(JSONEncoder):
             def default(self, obj):
                 return 'cabbage'
 
@@ -900,15 +901,15 @@
 
         api.add_resource(Cabbage, '/cabbage')
 
         with app.test_client() as client:
             data = client.get('/cabbage').data
 
         expected = b'{"frob": "cabbage"}\n'
-        self.assertEquals(data, expected)
+        self.assertEqual(data, expected)
 
     def test_json_with_no_settings(self):
         app = Flask(__name__)
         api = flask_restful.Api(app)
 
         class Foo(flask_restful.Resource):
             def get(self):
@@ -916,46 +917,46 @@
 
         api.add_resource(Foo, '/foo')
 
         with app.test_client() as client:
             data = client.get('/foo').data
 
         expected = b'{"foo": "bar"}\n'
-        self.assertEquals(data, expected)
+        self.assertEqual(data, expected)
 
     def test_redirect(self):
         app = Flask(__name__)
         api = flask_restful.Api(app)
 
         class FooResource(flask_restful.Resource):
             def get(self):
                 return redirect('/')
 
         api.add_resource(FooResource, '/api')
 
         app = app.test_client()
         resp = app.get('/api')
-        self.assertEquals(resp.status_code, 302)
-        self.assertEquals(resp.headers['Location'], 'http://localhost/')
+        self.assertEqual(resp.status_code, 302)
+        self.assertEqual(resp.headers['Location'], 'http://localhost/')
 
     def test_json_float_marshalled(self):
         app = Flask(__name__)
         api = flask_restful.Api(app)
 
         class FooResource(flask_restful.Resource):
             fields = {'foo': flask_restful.fields.Float}
             def get(self):
                 return flask_restful.marshal({"foo": 3.0}, self.fields)
 
         api.add_resource(FooResource, '/api')
 
         app = app.test_client()
         resp = app.get('/api')
-        self.assertEquals(resp.status_code, 200)
-        self.assertEquals(resp.data.decode('utf-8'), '{"foo": 3.0}\n')
+        self.assertEqual(resp.status_code, 200)
+        self.assertEqual(resp.data.decode('utf-8'), '{"foo": 3.0}\n')
 
     def test_custom_error_message(self):
         errors = {
             'FooError': {
                 'message': "api is foobar",
                 'status': 418,
             }
@@ -969,15 +970,15 @@
 
         exception = FooError()
         exception.code = 400
         exception.data = {'message': 'FooError'}
 
         with app.test_request_context("/foo"):
             resp = api.handle_error(exception)
-            self.assertEquals(resp.status_code, 418)
+            self.assertEqual(resp.status_code, 418)
             self.assertEqual(loads(resp.data.decode('utf8')), {"message": "api is foobar", "status": 418})
 
     def test_calling_owns_endpoint_before_api_init(self):
         api = flask_restful.Api()
 
         try:
             api.owns_endpoint('endpoint')
```

### Comparing `Flask-RESTful-0.3.8/tests/test_api_with_blueprint.py` & `Flask-RESTful-0.3.9/tests/test_api_with_blueprint.py`

 * *Files 4% similar despite different names*

```diff
@@ -29,17 +29,17 @@
 class APIWithBlueprintTestCase(unittest.TestCase):
 
     def test_api_base(self):
         blueprint = Blueprint('test', __name__)
         api = flask_restful.Api(blueprint)
         app = Flask(__name__)
         app.register_blueprint(blueprint)
-        self.assertEquals(api.urls, {})
-        self.assertEquals(api.prefix, '')
-        self.assertEquals(api.default_mediatype, 'application/json')
+        self.assertEqual(api.urls, {})
+        self.assertEqual(api.prefix, '')
+        self.assertEqual(api.default_mediatype, 'application/json')
 
     def test_api_delayed_initialization(self):
         blueprint = Blueprint('test', __name__)
         api = flask_restful.Api()
         api.init_app(blueprint)
         app = Flask(__name__)
         app.register_blueprint(blueprint)
@@ -66,60 +66,60 @@
     def test_url_with_api_prefix(self):
         blueprint = Blueprint('test', __name__)
         api = flask_restful.Api(blueprint, prefix='/api')
         api.add_resource(HelloWorld, '/hi', endpoint='hello')
         app = Flask(__name__)
         app.register_blueprint(blueprint)
         with app.test_request_context('/api/hi'):
-            self.assertEquals(request.endpoint, 'test.hello')
+            self.assertEqual(request.endpoint, 'test.hello')
 
     def test_url_with_blueprint_prefix(self):
         blueprint = Blueprint('test', __name__, url_prefix='/bp')
         api = flask_restful.Api(blueprint)
         api.add_resource(HelloWorld, '/hi', endpoint='hello')
         app = Flask(__name__)
         app.register_blueprint(blueprint)
         with app.test_request_context('/bp/hi'):
-            self.assertEquals(request.endpoint, 'test.hello')
+            self.assertEqual(request.endpoint, 'test.hello')
 
     def test_url_with_registration_prefix(self):
         blueprint = Blueprint('test', __name__)
         api = flask_restful.Api(blueprint)
         api.add_resource(HelloWorld, '/hi', endpoint='hello')
         app = Flask(__name__)
         app.register_blueprint(blueprint, url_prefix='/reg')
         with app.test_request_context('/reg/hi'):
-            self.assertEquals(request.endpoint, 'test.hello')
+            self.assertEqual(request.endpoint, 'test.hello')
 
     def test_registration_prefix_overrides_blueprint_prefix(self):
         blueprint = Blueprint('test', __name__, url_prefix='/bp')
         api = flask_restful.Api(blueprint)
         api.add_resource(HelloWorld, '/hi', endpoint='hello')
         app = Flask(__name__)
         app.register_blueprint(blueprint, url_prefix='/reg')
         with app.test_request_context('/reg/hi'):
-            self.assertEquals(request.endpoint, 'test.hello')
+            self.assertEqual(request.endpoint, 'test.hello')
 
     def test_url_with_api_and_blueprint_prefix(self):
         blueprint = Blueprint('test', __name__, url_prefix='/bp')
         api = flask_restful.Api(blueprint, prefix='/api')
         api.add_resource(HelloWorld, '/hi', endpoint='hello')
         app = Flask(__name__)
         app.register_blueprint(blueprint)
         with app.test_request_context('/bp/api/hi'):
-            self.assertEquals(request.endpoint, 'test.hello')
+            self.assertEqual(request.endpoint, 'test.hello')
 
     def test_url_part_order_aeb(self):
         blueprint = Blueprint('test', __name__, url_prefix='/bp')
         api = flask_restful.Api(blueprint, prefix='/api', url_part_order='aeb')
         api.add_resource(HelloWorld, '/hi', endpoint='hello')
         app = Flask(__name__)
         app.register_blueprint(blueprint)
         with app.test_request_context('/api/hi/bp'):
-            self.assertEquals(request.endpoint, 'test.hello')
+            self.assertEqual(request.endpoint, 'test.hello')
 
     def test_error_routing(self):
         blueprint = Blueprint('test', __name__)
         api = flask_restful.Api(blueprint)
         api.add_resource(HelloWorld(), '/hi', endpoint="hello")
         api.add_resource(GoodbyeWorld(404), '/bye', endpoint="bye")
         app = Flask(__name__)
```

### Comparing `Flask-RESTful-0.3.8/tests/test_cors.py` & `Flask-RESTful-0.3.9/tests/test_cors.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,12 +1,11 @@
 import unittest
 from flask import Flask
 import flask_restful
 from flask_restful.utils import cors
-from nose.tools import assert_equals, assert_true
 
 
 class CORSTestCase(unittest.TestCase):
 
     def test_crossdomain(self):
 
         class Foo(flask_restful.Resource):
@@ -16,20 +15,20 @@
 
         app = Flask(__name__)
         api = flask_restful.Api(app)
         api.add_resource(Foo, '/')
 
         with app.test_client() as client:
             res = client.get('/')
-            assert_equals(res.status_code, 200)
-            assert_equals(res.headers['Access-Control-Allow-Origin'], '*')
-            assert_equals(res.headers['Access-Control-Max-Age'], '21600')
-            assert_true('HEAD' in res.headers['Access-Control-Allow-Methods'])
-            assert_true('OPTIONS' in res.headers['Access-Control-Allow-Methods'])
-            assert_true('GET' in res.headers['Access-Control-Allow-Methods'])
+            self.assertEqual(res.status_code, 200)
+            self.assertEqual(res.headers['Access-Control-Allow-Origin'], '*')
+            self.assertEqual(res.headers['Access-Control-Max-Age'], '21600')
+            self.assertTrue('HEAD' in res.headers['Access-Control-Allow-Methods'])
+            self.assertTrue('OPTIONS' in res.headers['Access-Control-Allow-Methods'])
+            self.assertTrue('GET' in res.headers['Access-Control-Allow-Methods'])
 
     def test_access_control_expose_headers(self):
 
         class Foo(flask_restful.Resource):
             @cors.crossdomain(origin='*',
                               expose_headers=['X-My-Header', 'X-Another-Header'])
             def get(self):
@@ -37,17 +36,17 @@
 
         app = Flask(__name__)
         api = flask_restful.Api(app)
         api.add_resource(Foo, '/')
 
         with app.test_client() as client:
             res = client.get('/')
-            assert_equals(res.status_code, 200)
-            assert_true('X-MY-HEADER' in res.headers['Access-Control-Expose-Headers'])
-            assert_true('X-ANOTHER-HEADER' in res.headers['Access-Control-Expose-Headers'])
+            self.assertEqual(res.status_code, 200)
+            self.assertTrue('X-MY-HEADER' in res.headers['Access-Control-Expose-Headers'])
+            self.assertTrue('X-ANOTHER-HEADER' in res.headers['Access-Control-Expose-Headers'])
 
     def test_access_control_allow_methods(self):
 
         class Foo(flask_restful.Resource):
             @cors.crossdomain(origin='*',
                               methods={"HEAD","OPTIONS","GET"})
             def get(self):
@@ -58,29 +57,29 @@
 
         app = Flask(__name__)
         api = flask_restful.Api(app)
         api.add_resource(Foo, '/')
 
         with app.test_client() as client:
             res = client.get('/')
-            assert_equals(res.status_code, 200)
-            assert_true('HEAD' in res.headers['Access-Control-Allow-Methods'])
-            assert_true('OPTIONS' in res.headers['Access-Control-Allow-Methods'])
-            assert_true('GET' in res.headers['Access-Control-Allow-Methods'])
-            assert_true('POST' not in res.headers['Access-Control-Allow-Methods'])
+            self.assertEqual(res.status_code, 200)
+            self.assertTrue('HEAD' in res.headers['Access-Control-Allow-Methods'])
+            self.assertTrue('OPTIONS' in res.headers['Access-Control-Allow-Methods'])
+            self.assertTrue('GET' in res.headers['Access-Control-Allow-Methods'])
+            self.assertTrue('POST' not in res.headers['Access-Control-Allow-Methods'])
 
     def test_no_crossdomain(self):
 
         class Foo(flask_restful.Resource):
             def get(self):
                 return "data"
 
         app = Flask(__name__)
         api = flask_restful.Api(app)
         api.add_resource(Foo, '/')
 
         with app.test_client() as client:
             res = client.get('/')
-            assert_equals(res.status_code, 200)
-            assert_true('Access-Control-Allow-Origin' not in res.headers)
-            assert_true('Access-Control-Allow-Methods' not in res.headers)
-            assert_true('Access-Control-Max-Age' not in res.headers)
+            self.assertEqual(res.status_code, 200)
+            self.assertTrue('Access-Control-Allow-Origin' not in res.headers)
+            self.assertTrue('Access-Control-Allow-Methods' not in res.headers)
+            self.assertTrue('Access-Control-Max-Age' not in res.headers)
```

### Comparing `Flask-RESTful-0.3.8/tests/test_fields.py` & `Flask-RESTful-0.3.9/tests/test_fields.py`

 * *Files 2% similar despite different names*

```diff
@@ -84,30 +84,30 @@
 
     def test_decimal_trash(self):
         self.assertRaises(MarshallingException, lambda: fields.Float().output('a', {'a': 'Foo'}))
 
     def test_basic_dictionary(self):
         obj = {"foo": 3}
         field = fields.String()
-        self.assertEquals(field.output("foo", obj), "3")
+        self.assertEqual(field.output("foo", obj), "3")
 
     def test_no_attribute(self):
         obj = {"bar": 3}
         field = fields.String()
-        self.assertEquals(field.output("foo", obj), None)
+        self.assertEqual(field.output("foo", obj), None)
 
     def test_date_field_invalid(self):
         obj = {"bar": 3}
         field = fields.DateTime()
         self.assertRaises(MarshallingException, lambda: field.output("bar", obj))
 
     def test_attribute(self):
         obj = {"bar": 3}
         field = fields.String(attribute="bar")
-        self.assertEquals(field.output("foo", obj), "3")
+        self.assertEqual(field.output("foo", obj), "3")
 
     def test_formatting_field_none(self):
         obj = {}
         field = fields.FormattedString("/foo/{0[account_sid]}/{0[sid]}/")
         self.assertRaises(MarshallingException, lambda: field.output("foo", obj))
 
     def test_formatting_field_tuple(self):
@@ -117,67 +117,67 @@
 
     def test_formatting_field_dict(self):
         obj = {
             "sid": 3,
             "account_sid": 4,
         }
         field = fields.FormattedString("/foo/{account_sid}/{sid}/")
-        self.assertEquals(field.output("foo", obj), "/foo/4/3/")
+        self.assertEqual(field.output("foo", obj), "/foo/4/3/")
 
     def test_formatting_field(self):
         obj = Mock()
         obj.sid = 3
         obj.account_sid = 4
         field = fields.FormattedString("/foo/{account_sid}/{sid}/")
-        self.assertEquals(field.output("foo", obj), "/foo/4/3/")
+        self.assertEqual(field.output("foo", obj), "/foo/4/3/")
 
     def test_basic_field(self):
         obj = Mock()
         obj.foo = 3
         field = fields.Raw()
-        self.assertEquals(field.output("foo", obj), 3)
+        self.assertEqual(field.output("foo", obj), 3)
 
     def test_raw_field(self):
         obj = Mock()
         obj.foo = 3
         field = fields.Raw()
-        self.assertEquals(field.output("foo", obj), 3)
+        self.assertEqual(field.output("foo", obj), 3)
 
     def test_nested_raw_field(self):
         foo = Mock()
         bar = Mock()
         bar.value = 3
         foo.bar = bar
         field = fields.Raw()
-        self.assertEquals(field.output("bar.value", foo), 3)
+        self.assertEqual(field.output("bar.value", foo), 3)
 
     def test_formatted_string_invalid_obj(self):
         field = fields.FormattedString("{hey}")
         self.assertRaises(MarshallingException, lambda: field.output("hey", None))
 
     def test_formatted_string(self):
         field = fields.FormattedString("{hey}")
-        self.assertEquals("3", field.output("hey", Foo()))
+        self.assertEqual("3", field.output("hey", Foo()))
 
     def test_string_with_attribute(self):
         field = fields.String(attribute="hey")
-        self.assertEquals("3", field.output("foo", Foo()))
+        self.assertEqual("3", field.output("foo", Foo()))
 
     def test_string_with_lambda(self):
         field = fields.String(attribute=lambda x: x.hey)
-        self.assertEquals("3", field.output("foo", Foo()))
+        self.assertEqual("3", field.output("foo", Foo()))
 
     def test_string_with_partial(self):
 
         def f(x, suffix):
             return "%s-%s" % (x.hey, suffix)
 
         p = partial(f, suffix="whatever")
         field = fields.String(attribute=p)
-        self.assertEquals("3-whatever", field.output("foo", Foo()))
+        self.assertEqual("3-whatever", field.output("foo", Foo()))
 
     def test_url_invalid_object(self):
         app = Flask(__name__)
         app.add_url_rule("/<hey>", "foobar", view_func=lambda x: x)
         field = fields.Url("foobar")
 
         with app.test_request_context("/"):
@@ -185,32 +185,32 @@
 
     def test_url(self):
         app = Flask(__name__)
         app.add_url_rule("/<hey>", "foobar", view_func=lambda x: x)
         field = fields.Url("foobar")
 
         with app.test_request_context("/"):
-            self.assertEquals("/3", field.output("hey", Foo()))
+            self.assertEqual("/3", field.output("hey", Foo()))
 
     def test_url_absolute(self):
         app = Flask(__name__)
         app.add_url_rule("/<hey>", "foobar", view_func=lambda x: x)
         field = fields.Url("foobar", absolute=True)
 
         with app.test_request_context("/"):
-            self.assertEquals("http://localhost/3", field.output("hey", Foo()))
+            self.assertEqual("http://localhost/3", field.output("hey", Foo()))
 
     def test_url_absolute_scheme(self):
         """Url.scheme should override current_request.scheme"""
         app = Flask(__name__)
         app.add_url_rule("/<hey>", "foobar", view_func=lambda x: x)
         field = fields.Url("foobar", absolute=True, scheme='https')
 
         with app.test_request_context("/", base_url="http://localhost"):
-            self.assertEquals("https://localhost/3", field.output("hey", Foo()))
+            self.assertEqual("https://localhost/3", field.output("hey", Foo()))
 
     def test_url_without_endpoint_invalid_object(self):
         app = Flask(__name__)
         app.add_url_rule("/<hey>", "foobar", view_func=lambda x: x)
         field = fields.Url()
 
         with app.test_request_context("/hey"):
@@ -218,31 +218,31 @@
 
     def test_url_without_endpoint(self):
         app = Flask(__name__)
         app.add_url_rule("/<hey>", "foobar", view_func=lambda x: x)
         field = fields.Url()
 
         with app.test_request_context("/hey"):
-            self.assertEquals("/3", field.output("hey", Foo()))
+            self.assertEqual("/3", field.output("hey", Foo()))
 
     def test_url_without_endpoint_absolute(self):
         app = Flask(__name__)
         app.add_url_rule("/<hey>", "foobar", view_func=lambda x: x)
         field = fields.Url(absolute=True)
 
         with app.test_request_context("/hey"):
-            self.assertEquals("http://localhost/3", field.output("hey", Foo()))
+            self.assertEqual("http://localhost/3", field.output("hey", Foo()))
 
     def test_url_without_endpoint_absolute_scheme(self):
         app = Flask(__name__)
         app.add_url_rule("/<hey>", "foobar", view_func=lambda x: x)
         field = fields.Url(absolute=True, scheme='https')
 
         with app.test_request_context("/hey", base_url="http://localhost"):
-            self.assertEquals("https://localhost/3", field.output("hey", Foo()))
+            self.assertEqual("https://localhost/3", field.output("hey", Foo()))
 
     def test_url_with_blueprint_invalid_object(self):
         app = Flask(__name__)
         bp = Blueprint("foo", __name__, url_prefix="/foo")
         bp.add_url_rule("/<hey>", "foobar", view_func=lambda x: x)
         app.register_blueprint(bp)
         field = fields.Url()
@@ -254,185 +254,185 @@
         app = Flask(__name__)
         bp = Blueprint("foo", __name__, url_prefix="/foo")
         bp.add_url_rule("/<hey>", "foobar", view_func=lambda x: x)
         app.register_blueprint(bp)
         field = fields.Url()
 
         with app.test_request_context("/foo/hey"):
-            self.assertEquals("/foo/3", field.output("hey", Foo()))
+            self.assertEqual("/foo/3", field.output("hey", Foo()))
 
     def test_url_with_blueprint_absolute(self):
         app = Flask(__name__)
         bp = Blueprint("foo", __name__, url_prefix="/foo")
         bp.add_url_rule("/<hey>", "foobar", view_func=lambda x: x)
         app.register_blueprint(bp)
         field = fields.Url(absolute=True)
 
         with app.test_request_context("/foo/hey"):
-            self.assertEquals("http://localhost/foo/3", field.output("hey", Foo()))
+            self.assertEqual("http://localhost/foo/3", field.output("hey", Foo()))
 
     def test_url_with_blueprint_absolute_scheme(self):
         app = Flask(__name__)
         bp = Blueprint("foo", __name__, url_prefix="/foo")
         bp.add_url_rule("/<hey>", "foobar", view_func=lambda x: x)
         app.register_blueprint(bp)
         field = fields.Url(absolute=True, scheme='https')
 
         with app.test_request_context("/foo/hey", base_url="http://localhost"):
-            self.assertEquals("https://localhost/foo/3", field.output("hey", Foo()))
+            self.assertEqual("https://localhost/foo/3", field.output("hey", Foo()))
 
     def test_url_superclass_kwargs(self):
         app = Flask(__name__)
         app.add_url_rule("/<hey>", "foobar", view_func=lambda x: x)
         field = fields.Url(absolute=True, attribute='hey')
 
         with app.test_request_context("/hey"):
-            self.assertEquals("http://localhost/3", field.output("hey", Foo()))
+            self.assertEqual("http://localhost/3", field.output("hey", Foo()))
 
     def test_int(self):
         field = fields.Integer()
-        self.assertEquals(3, field.output("hey", {'hey': 3}))
+        self.assertEqual(3, field.output("hey", {'hey': 3}))
 
     def test_int_default(self):
         field = fields.Integer(default=1)
-        self.assertEquals(1, field.output("hey", {'hey': None}))
+        self.assertEqual(1, field.output("hey", {'hey': None}))
 
     def test_no_int(self):
         field = fields.Integer()
-        self.assertEquals(0, field.output("hey", {'hey': None}))
+        self.assertEqual(0, field.output("hey", {'hey': None}))
 
     def test_int_decode_error(self):
         field = fields.Integer()
         self.assertRaises(MarshallingException, lambda: field.output("hey", {'hey': 'Explode please I am nowhere looking like an int'}))
 
     def test_float(self):
         field = fields.Float()
-        self.assertEquals(3.0, field.output("hey", {'hey': 3.0}))
+        self.assertEqual(3.0, field.output("hey", {'hey': 3.0}))
 
     def test_float_decode_error(self):
         field = fields.Float()
         self.assertRaises(MarshallingException, lambda: field.output("hey", {'hey': 'Explode!'}))
 
     PI_STR = u'3.14159265358979323846264338327950288419716939937510582097494459230781640628620899862803482534211706798214808651328230664709384460955058223172535940812848111745028410270193852110555964462294895493038196442881097566593344612847564823378678316527120190914564856692346034861'
     PI = Decimal(PI_STR)
 
     def test_arbitrary(self):
         field = fields.Arbitrary()
-        self.assertEquals(self.PI_STR, field.output("hey", {'hey': self.PI}))
+        self.assertEqual(self.PI_STR, field.output("hey", {'hey': self.PI}))
 
     def test_fixed(self):
         field5 = fields.Fixed(5)
         field4 = fields.Fixed(4)
 
-        self.assertEquals('3.14159', field5.output("hey", {'hey': self.PI}))
-        self.assertEquals('3.1416', field4.output("hey", {'hey': self.PI}))
-        self.assertEquals('3.0000', field4.output("hey", {'hey': '3'}))
-        self.assertEquals('3.0000', field4.output("hey", {'hey': '03'}))
-        self.assertEquals('3.0000', field4.output("hey", {'hey': '03.0'}))
+        self.assertEqual('3.14159', field5.output("hey", {'hey': self.PI}))
+        self.assertEqual('3.1416', field4.output("hey", {'hey': self.PI}))
+        self.assertEqual('3.0000', field4.output("hey", {'hey': '3'}))
+        self.assertEqual('3.0000', field4.output("hey", {'hey': '03'}))
+        self.assertEqual('3.0000', field4.output("hey", {'hey': '03.0'}))
 
     def test_zero_fixed(self):
         field = fields.Fixed()
-        self.assertEquals('0.00000', field.output('hey', {'hey': 0}))
+        self.assertEqual('0.00000', field.output('hey', {'hey': 0}))
 
     def test_infinite_fixed(self):
         field = fields.Fixed()
         self.assertRaises(MarshallingException, lambda: field.output("hey", {'hey': '+inf'}))
         self.assertRaises(MarshallingException, lambda: field.output("hey", {'hey': '-inf'}))
 
     def test_advanced_fixed(self):
         field = fields.Fixed()
         self.assertRaises(MarshallingException, lambda: field.output("hey", {'hey': 'NaN'}))
 
     def test_fixed_with_attribute(self):
         field = fields.Fixed(4, attribute="bar")
-        self.assertEquals('3.0000', field.output("foo", {'bar': '3'}))
+        self.assertEqual('3.0000', field.output("foo", {'bar': '3'}))
 
     def test_string(self):
         field = fields.String()
-        self.assertEquals("3", field.output("hey", Foo()))
+        self.assertEqual("3", field.output("hey", Foo()))
 
     def test_string_no_value(self):
         field = fields.String()
-        self.assertEquals(None, field.output("bar", Foo()))
+        self.assertEqual(None, field.output("bar", Foo()))
 
     def test_string_none(self):
         field = fields.String()
-        self.assertEquals(None, field.output("empty", {'empty': None}))
+        self.assertEqual(None, field.output("empty", {'empty': None}))
 
     def test_rfc822_date_field_without_offset(self):
         obj = {"bar": datetime(2011, 8, 22, 20, 58, 45)}
         field = fields.DateTime()
-        self.assertEquals("Mon, 22 Aug 2011 20:58:45 -0000", field.output("bar", obj))
+        self.assertEqual("Mon, 22 Aug 2011 20:58:45 -0000", field.output("bar", obj))
 
     def test_rfc822_date_field_with_offset(self):
         obj = {"bar": datetime(2011, 8, 22, 20, 58, 45, tzinfo=pytz.timezone('CET'))}
         field = fields.DateTime()
-        self.assertEquals("Mon, 22 Aug 2011 19:58:45 -0000", field.output("bar", obj))
+        self.assertEqual("Mon, 22 Aug 2011 19:58:45 -0000", field.output("bar", obj))
 
     def test_iso8601_date_field_without_offset(self):
         obj = {"bar": datetime(2011, 8, 22, 20, 58, 45)}
         field = fields.DateTime(dt_format='iso8601')
-        self.assertEquals("2011-08-22T20:58:45", field.output("bar", obj))
+        self.assertEqual("2011-08-22T20:58:45", field.output("bar", obj))
 
     def test_iso8601_date_field_with_offset(self):
         obj = {"bar": datetime(2011, 8, 22, 20, 58, 45, tzinfo=pytz.timezone('CET'))}
         field = fields.DateTime(dt_format='iso8601')
-        self.assertEquals("2011-08-22T20:58:45+01:00", field.output("bar", obj))
+        self.assertEqual("2011-08-22T20:58:45+01:00", field.output("bar", obj))
 
     def test_unsupported_datetime_format(self):
         obj = {"bar": datetime(2011, 8, 22, 20, 58, 45)}
         field = fields.DateTime(dt_format='raw')
         self.assertRaises(MarshallingException, lambda: field.output('bar', obj))
 
     def test_to_dict(self):
         obj = {"hey": 3}
-        self.assertEquals(obj, fields.to_marshallable_type(obj))
+        self.assertEqual(obj, fields.to_marshallable_type(obj))
 
     def test_to_dict_obj(self):
         obj = {"hey": 3}
-        self.assertEquals(obj, fields.to_marshallable_type(Foo()))
+        self.assertEqual(obj, fields.to_marshallable_type(Foo()))
 
     def test_to_dict_custom_marshal(self):
         obj = {"hey": 3}
-        self.assertEquals(obj, fields.to_marshallable_type(Bar()))
+        self.assertEqual(obj, fields.to_marshallable_type(Bar()))
 
     def test_get_value(self):
-        self.assertEquals(3, fields.get_value("hey", {"hey": 3}))
+        self.assertEqual(3, fields.get_value("hey", {"hey": 3}))
 
     def test_get_value_no_value(self):
-        self.assertEquals(None, fields.get_value("foo", {"hey": 3}))
+        self.assertEqual(None, fields.get_value("foo", {"hey": 3}))
 
     def test_get_value_obj(self):
-        self.assertEquals(3, fields.get_value("hey", Foo()))
+        self.assertEqual(3, fields.get_value("hey", Foo()))
 
     def test_list(self):
         obj = {'list': ['a', 'b', 'c']}
         field = fields.List(fields.String)
-        self.assertEquals(['a', 'b', 'c'], field.output('list', obj))
+        self.assertEqual(['a', 'b', 'c'], field.output('list', obj))
 
     def test_list_from_set(self):
         obj = {'list': set(['a', 'b', 'c'])}
         field = fields.List(fields.String)
-        self.assertEquals(set(['a', 'b', 'c']), set(field.output('list', obj)))
+        self.assertEqual(set(['a', 'b', 'c']), set(field.output('list', obj)))
 
     def test_list_from_object(self):
         class TestObject(object):
             def __init__(self, list):
                 self.list = list
         obj = TestObject(['a', 'b', 'c'])
         field = fields.List(fields.String)
-        self.assertEquals(['a', 'b', 'c'], field.output('list', obj))
+        self.assertEqual(['a', 'b', 'c'], field.output('list', obj))
 
     def test_list_with_attribute(self):
         class TestObject(object):
             def __init__(self, list):
                 self.foo = list
         obj = TestObject(['a', 'b', 'c'])
         field = fields.List(fields.String, attribute='foo')
-        self.assertEquals(['a', 'b', 'c'], field.output('list', obj))
+        self.assertEqual(['a', 'b', 'c'], field.output('list', obj))
 
     def test_list_with_scoped_attribute_on_dict_or_obj(self):
         class TestObject(object):
             def __init__(self, list_):
                 self.bar = list_
 
         class TestEgg(object):
@@ -440,24 +440,24 @@
                 self.attrib = val
 
         eggs = [TestEgg(i) for i in ['a', 'b', 'c']]
         test_obj = TestObject(eggs)
         test_dict = {'bar': [{'attrib': 'a'}, {'attrib':'b'}, {'attrib':'c'}]}
 
         field = fields.List(fields.String(attribute='attrib'), attribute='bar')
-        self.assertEquals(['a', 'b', 'c'], field.output('bar', test_obj))
-        self.assertEquals(['a', 'b', 'c'], field.output('bar', test_dict))
+        self.assertEqual(['a', 'b', 'c'], field.output('bar', test_obj))
+        self.assertEqual(['a', 'b', 'c'], field.output('bar', test_dict))
 
     def test_null_list(self):
         class TestObject(object):
             def __init__(self, list):
                 self.list = list
         obj = TestObject(None)
         field = fields.List(fields.String)
-        self.assertEquals(None, field.output('list', obj))
+        self.assertEqual(None, field.output('list', obj))
 
     def test_indexable_object(self):
         class TestObject(object):
             def __init__(self, foo):
                 self.foo = foo
 
             def __getitem__(self, n):
@@ -465,40 +465,40 @@
                     if n < 3:
                         return n
                     raise IndexError
                 raise TypeError
 
         obj = TestObject("hi")
         field = fields.String(attribute="foo")
-        self.assertEquals("hi", field.output("foo", obj))
+        self.assertEqual("hi", field.output("foo", obj))
 
     def test_list_from_dict_with_attribute(self):
         obj = {'list': [{'a': 1, 'b': 1}, {'a': 2, 'b': 1}, {'a': 3, 'b': 1}]}
         field = fields.List(fields.Integer(attribute='a'))
-        self.assertEquals([1, 2, 3], field.output('list', obj))
+        self.assertEqual([1, 2, 3], field.output('list', obj))
 
     def test_list_of_nested(self):
         obj = {'list': [{'a': 1, 'b': 1}, {'a': 2, 'b': 1}, {'a': 3, 'b': 1}]}
         field = fields.List(fields.Nested({'a': fields.Integer}))
-        self.assertEquals([OrderedDict([('a', 1)]), OrderedDict([('a', 2)]), OrderedDict([('a', 3)])],
+        self.assertEqual([OrderedDict([('a', 1)]), OrderedDict([('a', 2)]), OrderedDict([('a', 3)])],
                           field.output('list', obj))
 
     def test_nested_with_default(self):
         obj = None
         field = fields.Nested({'a': fields.Integer, 'b': fields.String}, default={})
-        self.assertEquals({}, field.output('a', obj))
+        self.assertEqual({}, field.output('a', obj))
 
     def test_list_of_raw(self):
         obj = {'list': [{'a': 1, 'b': 1}, {'a': 2, 'b': 1}, {'a': 3, 'b': 1}]}
         field = fields.List(fields.Raw)
-        self.assertEquals([OrderedDict([('a', 1), ('b', 1), ]),
+        self.assertEqual([OrderedDict([('a', 1), ('b', 1), ]),
                            OrderedDict([('a', 2), ('b', 1), ]),
                            OrderedDict([('a', 3), ('b', 1), ])],
                           field.output('list', obj))
 
         obj = {'list': [1, 2, 'a']}
         field = fields.List(fields.Raw)
-        self.assertEquals([1, 2, 'a'], field.output('list', obj))
+        self.assertEqual([1, 2, 'a'], field.output('list', obj))
 
 
 if __name__ == '__main__':
     unittest.main()
```

### Comparing `Flask-RESTful-0.3.8/tests/test_inputs.py` & `Flask-RESTful-0.3.9/tests/test_inputs.py`

 * *Files identical despite different names*

### Comparing `Flask-RESTful-0.3.8/tests/test_reqparse.py` & `Flask-RESTful-0.3.9/tests/test_reqparse.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 # -*- coding: utf-8 -*-
 import unittest
 from mock import Mock, patch
 from flask import Flask
-from werkzeug import exceptions, MultiDict
+from werkzeug import exceptions
 from werkzeug.wrappers import Request
-from werkzeug.datastructures import FileStorage
+from werkzeug.datastructures import FileStorage, MultiDict
 from flask_restful.reqparse import Argument, RequestParser, Namespace
 import six
 import decimal
 
 import json
 
 
 class ReqParseTestCase(unittest.TestCase):
     def test_default_help(self):
         arg = Argument("foo")
-        self.assertEquals(arg.help, None)
+        self.assertEqual(arg.help, None)
 
     @patch('flask_restful.abort')
     def test_help_with_error_msg(self, abort):
         app = Flask(__name__)
         with app.app_context():
             parser = RequestParser()
             parser.add_argument('foo', choices=('one', 'two'), help='Bad choice: {error_msg}')
@@ -64,309 +64,309 @@
             abort.assert_called_with(400, message='three is not a valid choice')
         app = Flask(__name__)
         with app.app_context():
             self.assertRaises(exceptions.BadRequest, bad_choice)
 
     def test_name(self):
         arg = Argument("foo")
-        self.assertEquals(arg.name, "foo")
+        self.assertEqual(arg.name, "foo")
 
     def test_dest(self):
         arg = Argument("foo", dest="foobar")
-        self.assertEquals(arg.dest, "foobar")
+        self.assertEqual(arg.dest, "foobar")
 
     def test_location_url(self):
         arg = Argument("foo", location="url")
-        self.assertEquals(arg.location, "url")
+        self.assertEqual(arg.location, "url")
 
     def test_location_url_list(self):
         arg = Argument("foo", location=["url"])
-        self.assertEquals(arg.location, ["url"])
+        self.assertEqual(arg.location, ["url"])
 
     def test_location_header(self):
         arg = Argument("foo", location="headers")
-        self.assertEquals(arg.location, "headers")
+        self.assertEqual(arg.location, "headers")
 
     def test_location_json(self):
         arg = Argument("foo", location="json")
-        self.assertEquals(arg.location, "json")
+        self.assertEqual(arg.location, "json")
 
     def test_location_get_json(self):
         arg = Argument("foo", location="get_json")
-        self.assertEquals(arg.location, "get_json")
+        self.assertEqual(arg.location, "get_json")
 
     def test_location_header_list(self):
         arg = Argument("foo", location=["headers"])
-        self.assertEquals(arg.location, ["headers"])
+        self.assertEqual(arg.location, ["headers"])
 
     def test_type(self):
         arg = Argument("foo", type=int)
-        self.assertEquals(arg.type, int)
+        self.assertEqual(arg.type, int)
 
     def test_default(self):
         arg = Argument("foo", default=True)
-        self.assertEquals(arg.default, True)
+        self.assertEqual(arg.default, True)
 
     def test_required(self):
         arg = Argument("foo", required=True)
-        self.assertEquals(arg.required, True)
+        self.assertEqual(arg.required, True)
 
     def test_ignore(self):
         arg = Argument("foo", ignore=True)
-        self.assertEquals(arg.ignore, True)
+        self.assertEqual(arg.ignore, True)
 
     def test_operator(self):
         arg = Argument("foo", operators=[">=", "<=", "="])
-        self.assertEquals(arg.operators, [">=", "<=", "="])
+        self.assertEqual(arg.operators, [">=", "<=", "="])
 
     def test_action_filter(self):
         arg = Argument("foo", action="filter")
-        self.assertEquals(arg.action, u"filter")
+        self.assertEqual(arg.action, u"filter")
 
     def test_action(self):
         arg = Argument("foo", action="append")
-        self.assertEquals(arg.action, u"append")
+        self.assertEqual(arg.action, u"append")
 
     def test_choices(self):
         arg = Argument("foo", choices=[1, 2])
-        self.assertEquals(arg.choices, [1, 2])
+        self.assertEqual(arg.choices, [1, 2])
 
     def test_default_dest(self):
         arg = Argument("foo")
-        self.assertEquals(arg.dest, None)
+        self.assertEqual(arg.dest, None)
 
     def test_default_operators(self):
         arg = Argument("foo")
-        self.assertEquals(arg.operators[0], "=")
-        self.assertEquals(len(arg.operators), 1)
+        self.assertEqual(arg.operators[0], "=")
+        self.assertEqual(len(arg.operators), 1)
 
     @patch('flask_restful.reqparse.six')
     def test_default_type(self, mock_six):
         arg = Argument("foo")
         sentinel = object()
         arg.type(sentinel)
         mock_six.text_type.assert_called_with(sentinel)
 
     def test_default_default(self):
         arg = Argument("foo")
-        self.assertEquals(arg.default, None)
+        self.assertEqual(arg.default, None)
 
     def test_required_default(self):
         arg = Argument("foo")
-        self.assertEquals(arg.required, False)
+        self.assertEqual(arg.required, False)
 
     def test_ignore_default(self):
         arg = Argument("foo")
-        self.assertEquals(arg.ignore, False)
+        self.assertEqual(arg.ignore, False)
 
     def test_action_default(self):
         arg = Argument("foo")
-        self.assertEquals(arg.action, u"store")
+        self.assertEqual(arg.action, u"store")
 
     def test_choices_default(self):
         arg = Argument("foo")
-        self.assertEquals(len(arg.choices), 0)
+        self.assertEqual(len(arg.choices), 0)
 
     def test_source(self):
         req = Mock(['args', 'headers', 'values'])
         req.args = {'foo': 'bar'}
         req.headers = {'baz': 'bat'}
         arg = Argument('foo', location=['args'])
-        self.assertEquals(arg.source(req), MultiDict(req.args))
+        self.assertEqual(arg.source(req), MultiDict(req.args))
 
         arg = Argument('foo', location=['headers'])
-        self.assertEquals(arg.source(req), MultiDict(req.headers))
+        self.assertEqual(arg.source(req), MultiDict(req.headers))
 
     def test_convert_default_type_with_null_input(self):
         arg = Argument('foo')
-        self.assertEquals(arg.convert(None, None), None)
+        self.assertEqual(arg.convert(None, None), None)
 
     def test_convert_with_null_input_when_not_nullable(self):
         arg = Argument('foo', nullable=False)
         self.assertRaises(ValueError, lambda: arg.convert(None, None))
 
     def test_source_bad_location(self):
         req = Mock(['values'])
         arg = Argument('foo', location=['foo'])
         self.assertTrue(len(arg.source(req)) == 0)  # yes, basically you don't find it
 
     def test_source_default_location(self):
         req = Mock(['values'])
         req._get_child_mock = lambda **kwargs: MultiDict()
         arg = Argument('foo')
-        self.assertEquals(arg.source(req), req.values)
+        self.assertEqual(arg.source(req), req.values)
 
     def test_option_case_sensitive(self):
         arg = Argument("foo", choices=["bar", "baz"], case_sensitive=True)
-        self.assertEquals(True, arg.case_sensitive)
+        self.assertEqual(True, arg.case_sensitive)
 
         # Insensitive
         arg = Argument("foo", choices=["bar", "baz"], case_sensitive=False)
-        self.assertEquals(False, arg.case_sensitive)
+        self.assertEqual(False, arg.case_sensitive)
 
         # Default
         arg = Argument("foo", choices=["bar", "baz"])
-        self.assertEquals(True, arg.case_sensitive)
+        self.assertEqual(True, arg.case_sensitive)
 
     def test_viewargs(self):
         req = Request.from_values()
         req.view_args = {"foo": "bar"}
         parser = RequestParser()
         parser.add_argument("foo", location=["view_args"])
         args = parser.parse_args(req)
-        self.assertEquals(args['foo'], "bar")
+        self.assertEqual(args['foo'], "bar")
 
         req = Mock()
         req.values = ()
         req.json = None
         req.view_args = {"foo": "bar"}
         parser = RequestParser()
         parser.add_argument("foo", store_missing=True)
         args = parser.parse_args(req)
-        self.assertEquals(args["foo"], None)
+        self.assertEqual(args["foo"], None)
 
     def test_parse_unicode(self):
         req = Request.from_values("/bubble?foo=barß")
         parser = RequestParser()
         parser.add_argument("foo")
 
         args = parser.parse_args(req)
-        self.assertEquals(args['foo'], u"barß")
+        self.assertEqual(args['foo'], u"barß")
 
     def test_parse_unicode_app(self):
         app = Flask(__name__)
 
         parser = RequestParser()
         parser.add_argument("foo")
 
         with app.test_request_context('/bubble?foo=barß'):
             args = parser.parse_args()
-            self.assertEquals(args['foo'], u"barß")
+            self.assertEqual(args['foo'], u"barß")
 
     def test_json_location(self):
         app = Flask(__name__)
 
         parser = RequestParser()
         parser.add_argument("foo", location="json", store_missing=True)
 
         with app.test_request_context('/bubble', method="post"):
             args = parser.parse_args()
-            self.assertEquals(args['foo'], None)
+            self.assertEqual(args['foo'], None)
 
     def test_get_json_location(self):
         app = Flask(__name__)
 
         parser = RequestParser()
         parser.add_argument("foo", location="json")
 
         with app.test_request_context('/bubble', method="post",
                                       data=json.dumps({"foo": "bar"}),
                                       content_type='application/json'):
             args = parser.parse_args()
-            self.assertEquals(args['foo'], 'bar')
+            self.assertEqual(args['foo'], 'bar')
 
     def test_parse_append_ignore(self):
         req = Request.from_values("/bubble?foo=bar")
 
         parser = RequestParser()
         parser.add_argument("foo", ignore=True, type=int, action="append",
                             store_missing=True),
 
         args = parser.parse_args(req)
-        self.assertEquals(args['foo'], None)
+        self.assertEqual(args['foo'], None)
 
     def test_parse_append_default(self):
         req = Request.from_values("/bubble?")
 
         parser = RequestParser()
         parser.add_argument("foo", action="append", store_missing=True),
 
         args = parser.parse_args(req)
-        self.assertEquals(args['foo'], None)
+        self.assertEqual(args['foo'], None)
 
     def test_parse_append(self):
         req = Request.from_values("/bubble?foo=bar&foo=bat")
 
         parser = RequestParser()
         parser.add_argument("foo", action="append"),
 
         args = parser.parse_args(req)
-        self.assertEquals(args['foo'], ["bar", "bat"])
+        self.assertEqual(args['foo'], ["bar", "bat"])
 
     def test_parse_append_single(self):
         req = Request.from_values("/bubble?foo=bar")
 
         parser = RequestParser()
         parser.add_argument("foo", action="append"),
 
         args = parser.parse_args(req)
-        self.assertEquals(args['foo'], ["bar"])
+        self.assertEqual(args['foo'], ["bar"])
 
     def test_parse_append_many(self):
         req = Request.from_values("/bubble?foo=bar&foo=bar2")
 
         parser = RequestParser()
         parser.add_argument("foo", action="append"),
 
         args = parser.parse_args(req)
-        self.assertEquals(args['foo'], ["bar", "bar2"])
+        self.assertEqual(args['foo'], ["bar", "bar2"])
 
     def test_parse_append_many_location_json(self):
         app = Flask(__name__)
 
         parser = RequestParser()
         parser.add_argument("foo", action='append', location="json")
 
         with app.test_request_context('/bubble', method="post",
                                       data=json.dumps({"foo": ["bar", "bar2"]}),
                                       content_type='application/json'):
             args = parser.parse_args()
-            self.assertEquals(args['foo'], ['bar', 'bar2'])
+            self.assertEqual(args['foo'], ['bar', 'bar2'])
 
     def test_parse_dest(self):
         req = Request.from_values("/bubble?foo=bar")
 
         parser = RequestParser()
         parser.add_argument("foo", dest="bat")
 
         args = parser.parse_args(req)
-        self.assertEquals(args['bat'], "bar")
+        self.assertEqual(args['bat'], "bar")
 
     def test_parse_gte_lte_eq(self):
         req = Request.from_values("/bubble?foo>=bar&foo<=bat&foo=foo")
 
         parser = RequestParser()
         parser.add_argument("foo", operators=[">=", "<=", "="], action="append"),
 
         args = parser.parse_args(req)
-        self.assertEquals(args['foo'], ["bar", "bat", "foo"])
+        self.assertEqual(args['foo'], ["bar", "bat", "foo"])
 
     def test_parse_gte(self):
         req = Request.from_values("/bubble?foo>=bar")
 
         parser = RequestParser()
         parser.add_argument("foo", operators=[">="])
 
         args = parser.parse_args(req)
-        self.assertEquals(args['foo'], "bar")
+        self.assertEqual(args['foo'], "bar")
 
     def test_parse_foo_operators_four_hunderd(self):
         app = Flask(__name__)
         with app.app_context():
             parser = RequestParser()
             parser.add_argument("foo", type=int),
 
             self.assertRaises(exceptions.BadRequest, lambda: parser.parse_args(Request.from_values("/bubble?foo=bar")))
 
     def test_parse_foo_operators_ignore(self):
         parser = RequestParser()
         parser.add_argument("foo", ignore=True, store_missing=True)
 
         args = parser.parse_args(Request.from_values("/bubble"))
-        self.assertEquals(args['foo'], None)
+        self.assertEqual(args['foo'], None)
 
     def test_parse_lte_gte_mock(self):
         mock_type = Mock()
         req = Request.from_values("/bubble?foo<=bar")
 
         parser = RequestParser()
         parser.add_argument("foo", type=mock_type, operators=["<="])
@@ -375,42 +375,42 @@
         mock_type.assert_called_with("bar", "foo", "<=")
 
     def test_parse_lte_gte_append(self):
         parser = RequestParser()
         parser.add_argument("foo", operators=["<=", "="], action="append")
 
         args = parser.parse_args(Request.from_values("/bubble?foo<=bar"))
-        self.assertEquals(args['foo'], ["bar"])
+        self.assertEqual(args['foo'], ["bar"])
 
     def test_parse_lte_gte_missing(self):
         parser = RequestParser()
         parser.add_argument("foo", operators=["<=", "="])
         args = parser.parse_args(Request.from_values("/bubble?foo<=bar"))
-        self.assertEquals(args['foo'], "bar")
+        self.assertEqual(args['foo'], "bar")
 
     def test_parse_eq_other(self):
         parser = RequestParser()
         parser.add_argument("foo"),
         args = parser.parse_args(Request.from_values("/bubble?foo=bar&foo=bat"))
-        self.assertEquals(args['foo'], "bar")
+        self.assertEqual(args['foo'], "bar")
 
     def test_parse_eq(self):
         req = Request.from_values("/bubble?foo=bar")
         parser = RequestParser()
         parser.add_argument("foo"),
         args = parser.parse_args(req)
-        self.assertEquals(args['foo'], "bar")
+        self.assertEqual(args['foo'], "bar")
 
     def test_parse_lte(self):
         req = Request.from_values("/bubble?foo<=bar")
         parser = RequestParser()
         parser.add_argument("foo", operators=["<="])
 
         args = parser.parse_args(req)
-        self.assertEquals(args['foo'], "bar")
+        self.assertEqual(args['foo'], "bar")
 
     def test_parse_required(self):
         app = Flask(__name__)
         with app.app_context():
             req = Request.from_values("/bubble")
 
             parser = RequestParser()
@@ -418,26 +418,26 @@
 
             message = ''
             try:
                 parser.parse_args(req)
             except exceptions.BadRequest as e:
                 message = e.data['message']
 
-            self.assertEquals(message, ({'foo': 'Missing required parameter in '
+            self.assertEqual(message, ({'foo': 'Missing required parameter in '
                                                 'the post body or the query '
                                                 'string'}))
 
             parser = RequestParser()
             parser.add_argument("bar", required=True, location=['values', 'cookies'])
 
             try:
                 parser.parse_args(req)
             except exceptions.BadRequest as e:
                 message = e.data['message']
-            self.assertEquals(message, ({'bar': 'Missing required parameter in '
+            self.assertEqual(message, ({'bar': 'Missing required parameter in '
                                                 'the post body or the query '
                                                 'string or the request\'s '
                                                 'cookies'}))
 
     def test_parse_error_bundling(self):
         app = Flask(__name__)
         app.config['BUNDLE_ERRORS'] = True
@@ -454,15 +454,15 @@
             except exceptions.BadRequest as e:
                 message = e.data['message']
             error_message = {'foo': 'Missing required parameter in the post '
                                     'body or the query string',
                              'bar': 'Missing required parameter in the post '
                                     'body or the query string or the '
                                     'request\'s cookies'}
-            self.assertEquals(message, error_message)
+            self.assertEqual(message, error_message)
 
     def test_parse_error_bundling_w_parser_arg(self):
         app = Flask(__name__)
         app.config['BUNDLE_ERRORS'] = False
         with app.app_context():
             req = Request.from_values("/bubble")
 
@@ -476,61 +476,61 @@
             except exceptions.BadRequest as e:
                 message = e.data['message']
             error_message = {'foo': 'Missing required parameter in the post '
                                     'body or the query string',
                              'bar': 'Missing required parameter in the post '
                              'body or the query string or the request\'s '
                              'cookies'}
-            self.assertEquals(message, error_message)
+            self.assertEqual(message, error_message)
 
     def test_parse_default_append(self):
         req = Request.from_values("/bubble")
         parser = RequestParser()
         parser.add_argument("foo", default="bar", action="append",
                             store_missing=True)
 
         args = parser.parse_args(req)
 
-        self.assertEquals(args['foo'], "bar")
+        self.assertEqual(args['foo'], "bar")
 
     def test_parse_default(self):
         req = Request.from_values("/bubble")
 
         parser = RequestParser()
         parser.add_argument("foo", default="bar", store_missing=True)
 
         args = parser.parse_args(req)
-        self.assertEquals(args['foo'], "bar")
+        self.assertEqual(args['foo'], "bar")
 
     def test_parse_callable_default(self):
         req = Request.from_values("/bubble")
 
         parser = RequestParser()
         parser.add_argument("foo", default=lambda: "bar", store_missing=True)
 
         args = parser.parse_args(req)
-        self.assertEquals(args['foo'], "bar")
+        self.assertEqual(args['foo'], "bar")
 
     def test_parse(self):
         req = Request.from_values("/bubble?foo=bar")
 
         parser = RequestParser()
         parser.add_argument("foo"),
 
         args = parser.parse_args(req)
-        self.assertEquals(args['foo'], "bar")
+        self.assertEqual(args['foo'], "bar")
 
     def test_parse_none(self):
         req = Request.from_values("/bubble")
 
         parser = RequestParser()
         parser.add_argument("foo")
 
         args = parser.parse_args(req)
-        self.assertEquals(args['foo'], None)
+        self.assertEqual(args['foo'], None)
 
     def test_parse_store_missing(self):
         req = Request.from_values("/bubble")
 
         parser = RequestParser()
         parser.add_argument("foo", store_missing=False)
 
@@ -540,15 +540,15 @@
     def test_parse_choices_correct(self):
         req = Request.from_values("/bubble?foo=bat")
 
         parser = RequestParser()
         parser.add_argument("foo", choices=["bat"]),
 
         args = parser.parse_args(req)
-        self.assertEquals(args['foo'], "bat")
+        self.assertEqual(args['foo'], "bat")
 
     def test_parse_choices(self):
         app = Flask(__name__)
         with app.app_context():
             req = Request.from_values("/bubble?foo=bar")
 
             parser = RequestParser()
@@ -569,44 +569,44 @@
     def test_parse_choices_insensitive(self):
         req = Request.from_values("/bubble?foo=BAT")
 
         parser = RequestParser()
         parser.add_argument("foo", choices=["bat"], case_sensitive=False),
 
         args = parser.parse_args(req)
-        self.assertEquals('bat', args.get('foo'))
+        self.assertEqual('bat', args.get('foo'))
 
         # both choices and args are case_insensitive
         req = Request.from_values("/bubble?foo=bat")
 
         parser = RequestParser()
         parser.add_argument("foo", choices=["BAT"], case_sensitive=False),
 
         args = parser.parse_args(req)
-        self.assertEquals('bat', args.get('foo'))
+        self.assertEqual('bat', args.get('foo'))
 
     def test_parse_ignore(self):
         req = Request.from_values("/bubble?foo=bar")
 
         parser = RequestParser()
         parser.add_argument("foo", type=int, ignore=True, store_missing=True),
 
         args = parser.parse_args(req)
-        self.assertEquals(args['foo'], None)
+        self.assertEqual(args['foo'], None)
 
     def test_chaining(self):
         parser = RequestParser()
         self.assertTrue(parser is parser.add_argument("foo"))
 
     def test_namespace_existence(self):
         namespace = Namespace()
         namespace.foo = 'bar'
         namespace['bar'] = 'baz'
-        self.assertEquals(namespace['foo'], 'bar')
-        self.assertEquals(namespace.bar, 'baz')
+        self.assertEqual(namespace['foo'], 'bar')
+        self.assertEqual(namespace.bar, 'baz')
 
     def test_namespace_missing(self):
         namespace = Namespace()
         self.assertRaises(AttributeError, lambda: namespace.spam)
         self.assertRaises(KeyError, lambda: namespace['eggs'])
 
     def test_namespace_configurability(self):
@@ -620,79 +620,79 @@
 
         parser = RequestParser()
         parser.add_argument("foo", location="json")
         with app.test_request_context('/bubble', method="post",
                                       data=json.dumps({"foo": None}),
                                       content_type='application/json'):
             args = parser.parse_args()
-            self.assertEquals(args['foo'], None)
+            self.assertEqual(args['foo'], None)
 
     def test_type_callable(self):
         req = Request.from_values("/bubble?foo=1")
 
         parser = RequestParser()
         parser.add_argument("foo", type=lambda x: x, required=False),
 
         args = parser.parse_args(req)
-        self.assertEquals(args['foo'], "1")
+        self.assertEqual(args['foo'], "1")
 
     def test_type_callable_none(self):
         app = Flask(__name__)
 
         parser = RequestParser()
         parser.add_argument("foo", type=lambda x: x, location="json", required=False),
 
         with app.test_request_context('/bubble', method="post",
                                       data=json.dumps({"foo": None}),
                                       content_type='application/json'):
             try:
                 args = parser.parse_args()
-                self.assertEquals(args['foo'], None)
+                self.assertEqual(args['foo'], None)
             except exceptions.BadRequest:
                 self.fail()
 
     def test_type_decimal(self):
         app = Flask(__name__)
 
         parser = RequestParser()
         parser.add_argument("foo", type=decimal.Decimal, location="json")
 
         with app.test_request_context('/bubble', method='post',
                                       data=json.dumps({"foo": "1.0025"}),
                                       content_type='application/json'):
             args = parser.parse_args()
-            self.assertEquals(args['foo'], decimal.Decimal("1.0025"))
+            self.assertEqual(args['foo'], decimal.Decimal("1.0025"))
 
 
     def test_type_hard_decimal(self):
         app = Flask(__name__)
 
         parser = RequestParser()
         parser.add_argument("foo", type=decimal.Decimal, location="json")
 
         with app.test_request_context('/bubble', method='post',
                                       data=json.dumps({"foo": 89.92}),
                                       content_type='application/json'):
             args = parser.parse_args()
-            self.assertEquals(args['foo'], decimal.Decimal("89.92"))
+            self.assertEqual(args['foo'], decimal.Decimal("89.92"))
 
     def test_type_filestorage(self):
         app = Flask(__name__)
 
         parser = RequestParser()
         parser.add_argument("foo", type=FileStorage, location='files')
 
         fdata = six.b('foo bar baz qux')
         with app.test_request_context('/bubble', method='POST',
                                       data={'foo': (six.BytesIO(fdata), 'baz.txt')}):
             args = parser.parse_args()
 
-            self.assertEquals(args['foo'].name, 'foo')
-            self.assertEquals(args['foo'].filename, 'baz.txt')
-            self.assertEquals(args['foo'].read(), fdata)
+            self.assertEqual(args['foo'].name, 'foo')
+            self.assertEqual(args['foo'].filename, 'baz.txt')
+            self.assertEqual(args['foo'].read(), fdata)
 
     def test_filestorage_custom_type(self):
         def _custom_type(f):
             return FileStorage(stream=f.stream,
                                filename="{0}aaaa".format(f.filename),
                                name="{0}aaaa".format(f.name))
 
@@ -702,25 +702,25 @@
         parser.add_argument("foo", type=_custom_type, location='files')
 
         fdata = six.b('foo bar baz qux')
         with app.test_request_context('/bubble', method='POST',
                                       data={'foo': (six.BytesIO(fdata), 'baz.txt')}):
             args = parser.parse_args()
 
-            self.assertEquals(args['foo'].name, 'fooaaaa')
-            self.assertEquals(args['foo'].filename, 'baz.txtaaaa')
-            self.assertEquals(args['foo'].read(), fdata)
+            self.assertEqual(args['foo'].name, 'fooaaaa')
+            self.assertEqual(args['foo'].filename, 'baz.txtaaaa')
+            self.assertEqual(args['foo'].read(), fdata)
 
     def test_passing_arguments_object(self):
         req = Request.from_values("/bubble?foo=bar")
         parser = RequestParser()
         parser.add_argument(Argument("foo"))
 
         args = parser.parse_args(req)
-        self.assertEquals(args['foo'], u"bar")
+        self.assertEqual(args['foo'], u"bar")
 
     def test_int_choice_types(self):
         app = Flask(__name__)
         parser = RequestParser()
         parser.add_argument("foo", type=int, choices=[1, 2, 3], location='json')
 
         with app.test_request_context(
@@ -763,16 +763,16 @@
 
         # Args added to new parser should not be added to the original
         bar_arg = Argument('bar')
         parser_copy.args.append(bar_arg)
         self.assertFalse(bar_arg in parser.args)
 
         args = parser_copy.parse_args(req)
-        self.assertEquals(args['foo'], 101)
-        self.assertEquals(args['bar'], u'baz')
+        self.assertEqual(args['foo'], 101)
+        self.assertEqual(args['bar'], u'baz')
 
     def test_request_parse_copy_including_settings(self):
         parser = RequestParser(trim=True, bundle_errors=True)
         parser_copy = parser.copy()
 
         self.assertEqual(parser.trim, parser_copy.trim)
         self.assertEqual(parser.bundle_errors, parser_copy.bundle_errors)
@@ -781,29 +781,29 @@
         req = Request.from_values("/bubble?foo=baz")
         parser = RequestParser()
         parser.add_argument('foo', type=int)
         parser_copy = parser.copy()
         parser_copy.replace_argument('foo')
 
         args = parser_copy.parse_args(req)
-        self.assertEquals(args['foo'], u'baz')
+        self.assertEqual(args['foo'], u'baz')
 
     def test_both_json_and_values_location(self):
 
         app = Flask(__name__)
 
         parser = RequestParser()
         parser.add_argument('foo', type=int)
         parser.add_argument('baz', type=int)
         with app.test_request_context('/bubble?foo=1', method="post",
                                       data=json.dumps({"baz": 2}),
                                       content_type='application/json'):
             args = parser.parse_args()
-            self.assertEquals(args['foo'], 1)
-            self.assertEquals(args['baz'], 2)
+            self.assertEqual(args['foo'], 1)
+            self.assertEqual(args['baz'], 2)
 
     def test_not_json_location_and_content_type_json(self):
         app = Flask(__name__)
 
         parser = RequestParser()
         parser.add_argument('foo', location='args')
 
@@ -815,73 +815,73 @@
         req = Request.from_values("/bubble?foo=baz")
         parser = RequestParser()
         parser.add_argument('foo', type=int)
         parser_copy = parser.copy()
         parser_copy.remove_argument('foo')
 
         args = parser_copy.parse_args(req)
-        self.assertEquals(args, {})
+        self.assertEqual(args, {})
 
     def test_strict_parsing_off(self):
         req = Request.from_values("/bubble?foo=baz")
         parser = RequestParser()
         args = parser.parse_args(req)
-        self.assertEquals(args, {})
+        self.assertEqual(args, {})
 
     def test_strict_parsing_on(self):
         req = Request.from_values("/bubble?foo=baz")
         parser = RequestParser()
         self.assertRaises(exceptions.BadRequest, parser.parse_args, req, strict=True)
 
     def test_strict_parsing_off_partial_hit(self):
         req = Request.from_values("/bubble?foo=1&bar=bees&n=22")
         parser = RequestParser()
         parser.add_argument('foo', type=int)
         args = parser.parse_args(req)
-        self.assertEquals(args['foo'], 1)
+        self.assertEqual(args['foo'], 1)
 
     def test_strict_parsing_on_partial_hit(self):
         req = Request.from_values("/bubble?foo=1&bar=bees&n=22")
         parser = RequestParser()
         parser.add_argument('foo', type=int)
         self.assertRaises(exceptions.BadRequest, parser.parse_args, req, strict=True)
 
     def test_trim_argument(self):
         req = Request.from_values("/bubble?foo= 1 &bar=bees&n=22")
         parser = RequestParser()
         parser.add_argument('foo')
         args = parser.parse_args(req)
-        self.assertEquals(args['foo'], ' 1 ')
+        self.assertEqual(args['foo'], ' 1 ')
 
         parser = RequestParser()
         parser.add_argument('foo', trim=True)
         args = parser.parse_args(req)
-        self.assertEquals(args['foo'], '1')
+        self.assertEqual(args['foo'], '1')
 
         parser = RequestParser()
         parser.add_argument('foo', trim=True, type=int)
         args = parser.parse_args(req)
-        self.assertEquals(args['foo'], 1)
+        self.assertEqual(args['foo'], 1)
 
     def test_trim_request_parser(self):
         req = Request.from_values("/bubble?foo= 1 &bar=bees&n=22")
         parser = RequestParser(trim=False)
         parser.add_argument('foo')
         args = parser.parse_args(req)
-        self.assertEquals(args['foo'], ' 1 ')
+        self.assertEqual(args['foo'], ' 1 ')
 
         parser = RequestParser(trim=True)
         parser.add_argument('foo')
         args = parser.parse_args(req)
-        self.assertEquals(args['foo'], '1')
+        self.assertEqual(args['foo'], '1')
 
         parser = RequestParser(trim=True)
         parser.add_argument('foo', type=int)
         args = parser.parse_args(req)
-        self.assertEquals(args['foo'], 1)
+        self.assertEqual(args['foo'], 1)
 
     def test_trim_request_parser_override_by_argument(self):
         parser = RequestParser(trim=True)
         parser.add_argument('foo', trim=False)
 
         self.assertFalse(parser.args[0].trim)
 
@@ -893,41 +893,41 @@
         parser.add_argument("int1", location="json", type=int)
         parser.add_argument("int2", location="json", type=int)
 
         with app.test_request_context('/bubble', method="post",
                                       data=json.dumps({"foo": " bar ", "int1": 1, "int2": " 2 "}),
                                       content_type='application/json'):
             args = parser.parse_args()
-            self.assertEquals(args['foo'], 'bar')
-            self.assertEquals(args['int1'], 1)
-            self.assertEquals(args['int2'], 2)
+            self.assertEqual(args['foo'], 'bar')
+            self.assertEqual(args['int1'], 1)
+            self.assertEqual(args['int2'], 2)
 
     def test_list_argument(self):
         app = Flask(__name__)
 
         parser = RequestParser()
         parser.add_argument('arg1', location='json', type=list)
 
         with app.test_request_context('/bubble', method="post",
                                       data=json.dumps({'arg1': ['foo', 'bar']}),
                                       content_type='application/json'):
             args = parser.parse_args()
-            self.assertEquals(args['arg1'], ['foo', 'bar'])
+            self.assertEqual(args['arg1'], ['foo', 'bar'])
 
     def test_list_argument_dict(self):
         app = Flask(__name__)
 
         parser = RequestParser()
         parser.add_argument('arg1', location='json', type=list)
 
         with app.test_request_context('/bubble', method="post",
                                       data=json.dumps({'arg1': [{'foo': 1, 'bar': 2}]}),
                                       content_type='application/json'):
             args = parser.parse_args()
-            self.assertEquals(args['arg1'], [{'foo': 1, 'bar': 2}])
+            self.assertEqual(args['arg1'], [{'foo': 1, 'bar': 2}])
 
     def test_argument_repr(self):
         arg = Argument('foo')
         try:  # Python 2.6 compatibility
             self.assertIn('foo', arg.__repr__())
         except AttributeError:
             self.assertTrue('foo' in arg.__repr__())
```

