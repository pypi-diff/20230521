# Comparing `tmp/aa-charlink-0.3.0.tar.gz` & `tmp/aa-charlink-0.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aa-charlink-0.3.0.tar", last modified: Sun Apr 30 13:58:52 2023, max compression
+gzip compressed data, was "aa-charlink-0.4.0.tar", last modified: Sun May 21 17:42:15 2023, max compression
```

## Comparing `aa-charlink-0.3.0.tar` & `aa-charlink-0.4.0.tar`

### file list

```diff
@@ -1,41 +1,49 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-30 13:58:52.172855 aa-charlink-0.3.0/
--rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-04-30 13:58:37.000000 aa-charlink-0.3.0/LICENSE
--rwxr-xr-x   0 runner    (1001) docker     (123)      197 2023-04-30 13:58:37.000000 aa-charlink-0.3.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     2625 2023-04-30 13:58:52.172855 aa-charlink-0.3.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1452 2023-04-30 13:58:37.000000 aa-charlink-0.3.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-30 13:58:52.168855 aa-charlink-0.3.0/aa_charlink.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2625 2023-04-30 13:58:52.000000 aa-charlink-0.3.0/aa_charlink.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      841 2023-04-30 13:58:52.000000 aa-charlink-0.3.0/aa_charlink.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-30 13:58:52.000000 aa-charlink-0.3.0/aa_charlink.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-30 13:58:51.000000 aa-charlink-0.3.0/aa_charlink.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       18 2023-04-30 13:58:52.000000 aa-charlink-0.3.0/aa_charlink.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-04-30 13:58:52.000000 aa-charlink-0.3.0/aa_charlink.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-30 13:58:52.168855 aa-charlink-0.3.0/charlink/
--rwxr-xr-x   0 runner    (1001) docker     (123)      127 2023-04-30 13:58:37.000000 aa-charlink-0.3.0/charlink/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1451 2023-04-30 13:58:37.000000 aa-charlink-0.3.0/charlink/app_imports.py
--rw-r--r--   0 runner    (1001) docker     (123)      108 2023-04-30 13:58:37.000000 aa-charlink-0.3.0/charlink/app_settings.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      148 2023-04-30 13:58:37.000000 aa-charlink-0.3.0/charlink/apps.py
--rw-r--r--   0 runner    (1001) docker     (123)      468 2023-04-30 13:58:37.000000 aa-charlink-0.3.0/charlink/auth_hooks.py
--rw-r--r--   0 runner    (1001) docker     (123)      494 2023-04-30 13:58:37.000000 aa-charlink-0.3.0/charlink/decorators.py
--rw-r--r--   0 runner    (1001) docker     (123)      746 2023-04-30 13:58:37.000000 aa-charlink-0.3.0/charlink/forms.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-30 13:58:52.168855 aa-charlink-0.3.0/charlink/imports/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-30 13:58:37.000000 aa-charlink-0.3.0/charlink/imports/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-30 13:58:52.172855 aa-charlink-0.3.0/charlink/imports/allianceauth/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-30 13:58:37.000000 aa-charlink-0.3.0/charlink/imports/allianceauth/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1229 2023-04-30 13:58:37.000000 aa-charlink-0.3.0/charlink/imports/allianceauth/corputils.py
--rw-r--r--   0 runner    (1001) docker     (123)      662 2023-04-30 13:58:37.000000 aa-charlink-0.3.0/charlink/imports/corptools.py
--rw-r--r--   0 runner    (1001) docker     (123)     1162 2023-04-30 13:58:37.000000 aa-charlink-0.3.0/charlink/imports/memberaudit.py
--rw-r--r--   0 runner    (1001) docker     (123)      687 2023-04-30 13:58:37.000000 aa-charlink-0.3.0/charlink/imports/miningtaxes.py
--rw-r--r--   0 runner    (1001) docker     (123)     1689 2023-04-30 13:58:37.000000 aa-charlink-0.3.0/charlink/imports/moonmining.py
--rw-r--r--   0 runner    (1001) docker     (123)      820 2023-04-30 13:58:37.000000 aa-charlink-0.3.0/charlink/imports/moonstuff.py
--rw-r--r--   0 runner    (1001) docker     (123)     4419 2023-04-30 13:58:37.000000 aa-charlink-0.3.0/charlink/imports/structures.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-30 13:58:52.172855 aa-charlink-0.3.0/charlink/migrations/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-30 13:58:37.000000 aa-charlink-0.3.0/charlink/migrations/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       29 2023-04-30 13:58:37.000000 aa-charlink-0.3.0/charlink/models.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-30 13:58:52.164855 aa-charlink-0.3.0/charlink/templates/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-30 13:58:52.172855 aa-charlink-0.3.0/charlink/templates/charlink/
--rw-r--r--   0 runner    (1001) docker     (123)     3082 2023-04-30 13:58:37.000000 aa-charlink-0.3.0/charlink/templates/charlink/charlink.html
--rw-r--r--   0 runner    (1001) docker     (123)      185 2023-04-30 13:58:37.000000 aa-charlink-0.3.0/charlink/urls.py
--rw-r--r--   0 runner    (1001) docker     (123)     3220 2023-04-30 13:58:37.000000 aa-charlink-0.3.0/charlink/views.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      104 2023-04-30 13:58:37.000000 aa-charlink-0.3.0/pyproject.toml
--rwxr-xr-x   0 runner    (1001) docker     (123)     1577 2023-04-30 13:58:52.172855 aa-charlink-0.3.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 17:42:15.984414 aa-charlink-0.4.0/
+-rwxr-xr-x   0 runner    (1001) docker     (123)    35149 2023-05-21 17:42:03.000000 aa-charlink-0.4.0/LICENSE
+-rwxr-xr-x   0 runner    (1001) docker     (123)      197 2023-05-21 17:42:03.000000 aa-charlink-0.4.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     3532 2023-05-21 17:42:15.984414 aa-charlink-0.4.0/PKG-INFO
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2359 2023-05-21 17:42:03.000000 aa-charlink-0.4.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 17:42:15.980413 aa-charlink-0.4.0/aa_charlink.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3532 2023-05-21 17:42:15.000000 aa-charlink-0.4.0/aa_charlink.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1117 2023-05-21 17:42:15.000000 aa-charlink-0.4.0/aa_charlink.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-21 17:42:15.000000 aa-charlink-0.4.0/aa_charlink.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-21 17:42:15.000000 aa-charlink-0.4.0/aa_charlink.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       18 2023-05-21 17:42:15.000000 aa-charlink-0.4.0/aa_charlink.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-05-21 17:42:15.000000 aa-charlink-0.4.0/aa_charlink.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 17:42:15.984414 aa-charlink-0.4.0/charlink/
+-rwxr-xr-x   0 runner    (1001) docker     (123)      127 2023-05-21 17:42:03.000000 aa-charlink-0.4.0/charlink/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1451 2023-05-21 17:42:03.000000 aa-charlink-0.4.0/charlink/app_imports.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      108 2023-05-21 17:42:03.000000 aa-charlink-0.4.0/charlink/app_settings.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      148 2023-05-21 17:42:03.000000 aa-charlink-0.4.0/charlink/apps.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      468 2023-05-21 17:42:03.000000 aa-charlink-0.4.0/charlink/auth_hooks.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      494 2023-05-21 17:42:03.000000 aa-charlink-0.4.0/charlink/decorators.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      746 2023-05-21 17:42:03.000000 aa-charlink-0.4.0/charlink/forms.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 17:42:15.984414 aa-charlink-0.4.0/charlink/imports/
+-rwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 17:42:03.000000 aa-charlink-0.4.0/charlink/imports/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 17:42:15.984414 aa-charlink-0.4.0/charlink/imports/allianceauth/
+-rwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 17:42:03.000000 aa-charlink-0.4.0/charlink/imports/allianceauth/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1229 2023-05-21 17:42:03.000000 aa-charlink-0.4.0/charlink/imports/allianceauth/corputils.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      662 2023-05-21 17:42:03.000000 aa-charlink-0.4.0/charlink/imports/corptools.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1162 2023-05-21 17:42:03.000000 aa-charlink-0.4.0/charlink/imports/memberaudit.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      687 2023-05-21 17:42:03.000000 aa-charlink-0.4.0/charlink/imports/miningtaxes.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1689 2023-05-21 17:42:03.000000 aa-charlink-0.4.0/charlink/imports/moonmining.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      820 2023-05-21 17:42:03.000000 aa-charlink-0.4.0/charlink/imports/moonstuff.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     4419 2023-05-21 17:42:03.000000 aa-charlink-0.4.0/charlink/imports/structures.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 17:42:15.984414 aa-charlink-0.4.0/charlink/migrations/
+-rw-r--r--   0 runner    (1001) docker     (123)      810 2023-05-21 17:42:03.000000 aa-charlink-0.4.0/charlink/migrations/0001_initial.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 17:42:03.000000 aa-charlink-0.4.0/charlink/migrations/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      435 2023-05-21 17:42:03.000000 aa-charlink-0.4.0/charlink/models.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 17:42:15.980413 aa-charlink-0.4.0/charlink/templates/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 17:42:15.984414 aa-charlink-0.4.0/charlink/templates/charlink/
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3656 2023-05-21 17:42:03.000000 aa-charlink-0.4.0/charlink/templates/charlink/audit.html
+-rw-r--r--   0 runner    (1001) docker     (123)     1507 2023-05-21 17:42:03.000000 aa-charlink-0.4.0/charlink/templates/charlink/base_audit.html
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3565 2023-05-21 17:42:03.000000 aa-charlink-0.4.0/charlink/templates/charlink/charlink.html
+-rw-r--r--   0 runner    (1001) docker     (123)     2258 2023-05-21 17:42:03.000000 aa-charlink-0.4.0/charlink/templates/charlink/search.html
+-rw-r--r--   0 runner    (1001) docker     (123)     1616 2023-05-21 17:42:03.000000 aa-charlink-0.4.0/charlink/templates/charlink/user_audit.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 17:42:15.984414 aa-charlink-0.4.0/charlink/templatetags/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-21 17:42:03.000000 aa-charlink-0.4.0/charlink/templatetags/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      346 2023-05-21 17:42:03.000000 aa-charlink-0.4.0/charlink/templatetags/charlinkutils.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      429 2023-05-21 17:42:03.000000 aa-charlink-0.4.0/charlink/urls.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     7398 2023-05-21 17:42:03.000000 aa-charlink-0.4.0/charlink/views.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      104 2023-05-21 17:42:03.000000 aa-charlink-0.4.0/pyproject.toml
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1577 2023-05-21 17:42:15.984414 aa-charlink-0.4.0/setup.cfg
```

### Comparing `aa-charlink-0.3.0/LICENSE` & `aa-charlink-0.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `aa-charlink-0.3.0/charlink/app_imports.py` & `aa-charlink-0.4.0/charlink/app_imports.py`

 * *Files identical despite different names*

### Comparing `aa-charlink-0.3.0/charlink/forms.py` & `aa-charlink-0.4.0/charlink/forms.py`

 * *Files identical despite different names*

### Comparing `aa-charlink-0.3.0/charlink/imports/allianceauth/corputils.py` & `aa-charlink-0.4.0/charlink/imports/allianceauth/corputils.py`

 * *Files identical despite different names*

### Comparing `aa-charlink-0.3.0/charlink/imports/corptools.py` & `aa-charlink-0.4.0/charlink/imports/corptools.py`

 * *Files identical despite different names*

### Comparing `aa-charlink-0.3.0/charlink/imports/memberaudit.py` & `aa-charlink-0.4.0/charlink/imports/memberaudit.py`

 * *Files identical despite different names*

### Comparing `aa-charlink-0.3.0/charlink/imports/miningtaxes.py` & `aa-charlink-0.4.0/charlink/imports/miningtaxes.py`

 * *Files identical despite different names*

### Comparing `aa-charlink-0.3.0/charlink/imports/moonmining.py` & `aa-charlink-0.4.0/charlink/imports/moonmining.py`

 * *Files identical despite different names*

### Comparing `aa-charlink-0.3.0/charlink/imports/moonstuff.py` & `aa-charlink-0.4.0/charlink/imports/moonstuff.py`

 * *Files identical despite different names*

### Comparing `aa-charlink-0.3.0/charlink/imports/structures.py` & `aa-charlink-0.4.0/charlink/imports/structures.py`

 * *Files identical despite different names*

### Comparing `aa-charlink-0.3.0/charlink/templates/charlink/charlink.html` & `aa-charlink-0.4.0/charlink/templates/charlink/charlink.html`

 * *Files 14% similar despite different names*

```diff
@@ -14,14 +14,24 @@
         }
     </style>
 {% endblock extra_css %}
 
 {% block content %}
     <div class="col-lg-12">
         <h1 class="page-header text-center">Character Linking</h1>
+        {% if is_auditor %}
+            <div class="panel panel-warning text-center">
+                <div class="panel-heading">
+                    <h3 class="panel-title text-center">Admin Section</h3>
+                </div>
+                <div class="panel-body">
+                    <a href="{% url 'charlink:audit' %}" class="btn btn-success">Auditing&nbsp;&nbsp;<i class="fas fa-external-link-alt fa-xs"></i></a>
+                </div>
+            </div>
+        {% endif %}
         <div class="panel panel-primary text-center">
             <div class="panel-heading">
                 <h3 class="panel-title text-center">Login Form</h3>
             </div>
             <div class="panel-body">
                 <p>Select the apps you want to link from the list. You will be redirected to eveonline website to authenticate and provide the token with all the scopes needed.</p>
                 <br>
```

#### html2text {}

```diff
@@ -1,11 +1,15 @@
 {% extends 'allianceauth/base.html' %} {% load bootstrap %} {% block page_title
 %}Charlink{% endblock page_title %} {% block extra_css %}
  {% endblock extra_css %} {% block content %}
 ****** Character Linking ******
+{% if is_auditor %}
+**** Admin Section ****
+Auditing  
+{% endif %}
 **** Login Form ****
 Select the apps you want to link from the list. You will be redirected to
 eveonline website to authenticate and provide the token with all the scopes
 needed.
 
 {% csrf_token %} {{ form|bootstrap }} Login
 **** Linked Characters ****
```

### Comparing `aa-charlink-0.3.0/setup.cfg` & `aa-charlink-0.4.0/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 [bumpversion]
-current_version = 0.3.0
+current_version = 0.4.0
 parse = (?P<major>\d+)\.(?P<minor>\d+)\.(?P<patch>\d+)(b(?P<beta>\d+))?
 serialize = 
 	{major}.{minor}.{patch}b{beta}
 	{major}.{minor}.{patch}
 commit = True
 tag = True
 sign_tags = True
```

