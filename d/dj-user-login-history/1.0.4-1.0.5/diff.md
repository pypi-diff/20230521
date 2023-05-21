# Comparing `tmp/dj-user-login-history-1.0.4.tar.gz` & `tmp/dj-user-login-history-1.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dj-user-login-history-1.0.4.tar", last modified: Fri May 19 17:29:39 2023, max compression
+gzip compressed data, was "dj-user-login-history-1.0.5.tar", last modified: Sun May 21 07:13:03 2023, max compression
```

## Comparing `dj-user-login-history-1.0.4.tar` & `dj-user-login-history-1.0.5.tar`

### file list

```diff
@@ -1,26 +1,26 @@
-drwxrwxrwx   0        0        0        0 2023-05-19 17:29:39.634321 dj-user-login-history-1.0.4/
--rw-rw-rw-   0        0        0     1092 2023-03-01 16:30:58.000000 dj-user-login-history-1.0.4/LICENSE
--rw-rw-rw-   0        0        0     2070 2023-05-19 17:29:39.633329 dj-user-login-history-1.0.4/PKG-INFO
--rw-rw-rw-   0        0        0     1576 2023-03-01 16:30:58.000000 dj-user-login-history-1.0.4/README.md
-drwxrwxrwx   0        0        0        0 2023-05-19 17:29:39.595736 dj-user-login-history-1.0.4/dj_user_login_history.egg-info/
--rw-rw-rw-   0        0        0     2070 2023-05-19 17:29:39.000000 dj-user-login-history-1.0.4/dj_user_login_history.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      815 2023-05-19 17:29:39.000000 dj-user-login-history-1.0.4/dj_user_login_history.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-19 17:29:39.000000 dj-user-login-history-1.0.4/dj_user_login_history.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       12 2023-05-19 17:29:39.000000 dj-user-login-history-1.0.4/dj_user_login_history.egg-info/requires.txt
--rw-rw-rw-   0        0        0       39 2023-05-19 17:29:39.000000 dj-user-login-history-1.0.4/dj_user_login_history.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2023-05-19 17:29:39.620546 dj-user-login-history-1.0.4/login_history/
--rw-rw-rw-   0        0        0        0 2023-03-01 16:30:58.000000 dj-user-login-history-1.0.4/login_history/__init__.py
--rw-rw-rw-   0        0        0      573 2023-03-01 16:30:58.000000 dj-user-login-history-1.0.4/login_history/admin.py
--rw-rw-rw-   0        0        0      199 2023-05-19 17:25:11.000000 dj-user-login-history-1.0.4/login_history/apps.py
-drwxrwxrwx   0        0        0        0 2023-05-19 17:29:39.629236 dj-user-login-history-1.0.4/login_history/migrations/
--rw-rw-rw-   0        0        0     1220 2023-03-01 16:30:58.000000 dj-user-login-history-1.0.4/login_history/migrations/0001_initial.py
--rw-rw-rw-   0        0        0      430 2023-03-01 16:30:58.000000 dj-user-login-history-1.0.4/login_history/migrations/0002_loginhistory_is_login.py
--rw-rw-rw-   0        0        0      476 2023-05-19 17:25:33.000000 dj-user-login-history-1.0.4/login_history/migrations/0003_alter_loginhistory_id.py
--rw-rw-rw-   0        0        0        0 2023-03-01 16:30:58.000000 dj-user-login-history-1.0.4/login_history/migrations/__init__.py
--rw-rw-rw-   0        0        0     3426 2023-03-01 16:30:58.000000 dj-user-login-history-1.0.4/login_history/models.py
--rw-rw-rw-   0        0        0     1228 2023-03-01 16:30:58.000000 dj-user-login-history-1.0.4/login_history/settings.py
--rw-rw-rw-   0        0        0       63 2023-03-01 16:30:58.000000 dj-user-login-history-1.0.4/login_history/tests.py
--rw-rw-rw-   0        0        0      100 2023-03-01 16:30:58.000000 dj-user-login-history-1.0.4/login_history/urls.py
--rw-rw-rw-   0        0        0      563 2023-03-01 16:30:58.000000 dj-user-login-history-1.0.4/login_history/views.py
--rw-rw-rw-   0        0        0       42 2023-05-19 17:29:39.634321 dj-user-login-history-1.0.4/setup.cfg
--rw-rw-rw-   0        0        0     1002 2023-05-19 17:29:19.000000 dj-user-login-history-1.0.4/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-21 07:13:03.179280 dj-user-login-history-1.0.5/
+-rw-rw-rw-   0        0        0     1092 2023-03-01 16:30:58.000000 dj-user-login-history-1.0.5/LICENSE
+-rw-rw-rw-   0        0        0     2070 2023-05-21 07:13:03.178248 dj-user-login-history-1.0.5/PKG-INFO
+-rw-rw-rw-   0        0        0     1576 2023-03-01 16:30:58.000000 dj-user-login-history-1.0.5/README.md
+drwxrwxrwx   0        0        0        0 2023-05-21 07:13:03.146225 dj-user-login-history-1.0.5/dj_user_login_history.egg-info/
+-rw-rw-rw-   0        0        0     2070 2023-05-21 07:13:02.000000 dj-user-login-history-1.0.5/dj_user_login_history.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      815 2023-05-21 07:13:03.000000 dj-user-login-history-1.0.5/dj_user_login_history.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-21 07:13:02.000000 dj-user-login-history-1.0.5/dj_user_login_history.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       12 2023-05-21 07:13:02.000000 dj-user-login-history-1.0.5/dj_user_login_history.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       39 2023-05-21 07:13:02.000000 dj-user-login-history-1.0.5/dj_user_login_history.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-05-21 07:13:03.164830 dj-user-login-history-1.0.5/login_history/
+-rw-rw-rw-   0        0        0        0 2023-03-01 16:30:58.000000 dj-user-login-history-1.0.5/login_history/__init__.py
+-rw-rw-rw-   0        0        0      563 2023-05-21 07:10:53.000000 dj-user-login-history-1.0.5/login_history/admin.py
+-rw-rw-rw-   0        0        0      199 2023-05-19 17:25:11.000000 dj-user-login-history-1.0.5/login_history/apps.py
+drwxrwxrwx   0        0        0        0 2023-05-21 07:13:03.174321 dj-user-login-history-1.0.5/login_history/migrations/
+-rw-rw-rw-   0        0        0     1220 2023-03-01 16:30:58.000000 dj-user-login-history-1.0.5/login_history/migrations/0001_initial.py
+-rw-rw-rw-   0        0        0      430 2023-03-01 16:30:58.000000 dj-user-login-history-1.0.5/login_history/migrations/0002_loginhistory_is_login.py
+-rw-rw-rw-   0        0        0      476 2023-05-19 17:25:33.000000 dj-user-login-history-1.0.5/login_history/migrations/0003_alter_loginhistory_id.py
+-rw-rw-rw-   0        0        0        0 2023-03-01 16:30:58.000000 dj-user-login-history-1.0.5/login_history/migrations/__init__.py
+-rw-rw-rw-   0        0        0     3426 2023-03-01 16:30:58.000000 dj-user-login-history-1.0.5/login_history/models.py
+-rw-rw-rw-   0        0        0     1228 2023-03-01 16:30:58.000000 dj-user-login-history-1.0.5/login_history/settings.py
+-rw-rw-rw-   0        0        0       63 2023-03-01 16:30:58.000000 dj-user-login-history-1.0.5/login_history/tests.py
+-rw-rw-rw-   0        0        0      100 2023-03-01 16:30:58.000000 dj-user-login-history-1.0.5/login_history/urls.py
+-rw-rw-rw-   0        0        0      563 2023-03-01 16:30:58.000000 dj-user-login-history-1.0.5/login_history/views.py
+-rw-rw-rw-   0        0        0       42 2023-05-21 07:13:03.179280 dj-user-login-history-1.0.5/setup.cfg
+-rw-rw-rw-   0        0        0     1002 2023-05-21 07:12:28.000000 dj-user-login-history-1.0.5/setup.py
```

### Comparing `dj-user-login-history-1.0.4/LICENSE` & `dj-user-login-history-1.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `dj-user-login-history-1.0.4/PKG-INFO` & `dj-user-login-history-1.0.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dj-user-login-history
-Version: 1.0.4
+Version: 1.0.5
 Summary: Django app which keep track of user login history.
 Home-page: https://github.com/farhad0085/dj-user-login-history
 Author: Farhad Hossain
 Author-email: farhadhossain0085@gmail.com
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

### Comparing `dj-user-login-history-1.0.4/README.md` & `dj-user-login-history-1.0.5/README.md`

 * *Files identical despite different names*

### Comparing `dj-user-login-history-1.0.4/dj_user_login_history.egg-info/PKG-INFO` & `dj-user-login-history-1.0.5/dj_user_login_history.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dj-user-login-history
-Version: 1.0.4
+Version: 1.0.5
 Summary: Django app which keep track of user login history.
 Home-page: https://github.com/farhad0085/dj-user-login-history
 Author: Farhad Hossain
 Author-email: farhadhossain0085@gmail.com
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

### Comparing `dj-user-login-history-1.0.4/dj_user_login_history.egg-info/SOURCES.txt` & `dj-user-login-history-1.0.5/dj_user_login_history.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `dj-user-login-history-1.0.4/login_history/admin.py` & `dj-user-login-history-1.0.5/login_history/admin.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from django.contrib import admin
 from .models import LoginHistory
 
 
 class ReadOnlyLoginHistoryAdmin(admin.ModelAdmin):
     list_display = ['user', 'id', 'date_time', 'ip', 'user_agent', 'is_logged_in', 'get_action_status']
-    list_filter = ['user__username']
+    list_filter = ['user']
 
     def get_action_status(self, obj):
         if obj.is_login:
             return "Login"
         return "Logout"
 
     def has_add_permission(self, request):
```

### Comparing `dj-user-login-history-1.0.4/login_history/migrations/0001_initial.py` & `dj-user-login-history-1.0.5/login_history/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `dj-user-login-history-1.0.4/login_history/models.py` & `dj-user-login-history-1.0.5/login_history/models.py`

 * *Files identical despite different names*

### Comparing `dj-user-login-history-1.0.4/login_history/settings.py` & `dj-user-login-history-1.0.5/login_history/settings.py`

 * *Files identical despite different names*

### Comparing `dj-user-login-history-1.0.4/login_history/views.py` & `dj-user-login-history-1.0.5/login_history/views.py`

 * *Files identical despite different names*

### Comparing `dj-user-login-history-1.0.4/setup.py` & `dj-user-login-history-1.0.5/setup.py`

 * *Files 11% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 
 # The text of the README file
 README = (BASE_PATH / "README.md").read_text()
 
 # This call to setup() does all the work
 setup(
     name="dj-user-login-history",
-    version="1.0.4",
+    version="1.0.5",
     description="Django app which keep track of user login history.",
     long_description=README,
     long_description_content_type="text/markdown",
     url="https://github.com/farhad0085/dj-user-login-history",
     author="Farhad Hossain",
     author_email="farhadhossain0085@gmail.com",
     license="MIT",
```

