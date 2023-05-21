# Comparing `tmp/ersciyt-1.87.tar.gz` & `tmp/ersciyt-1.88.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ersciyt-1.87.tar", last modified: Thu May 18 23:46:40 2023, max compression
+gzip compressed data, was "ersciyt-1.88.tar", last modified: Sun May 21 04:57:48 2023, max compression
```

## Comparing `ersciyt-1.87.tar` & `ersciyt-1.88.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-18 23:46:40.046178 ersciyt-1.87/
--rw-r--r--   0 root         (0) root         (0)    35149 2023-05-18 23:46:34.000000 ersciyt-1.87/LICENSE
--rw-r--r--   0 root         (0) root         (0)       69 2023-05-18 23:46:34.000000 ersciyt-1.87/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)      778 2023-05-18 23:46:40.046178 ersciyt-1.87/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      517 2023-05-18 23:46:34.000000 ersciyt-1.87/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-18 23:46:40.044178 ersciyt-1.87/ersciyt/
--rw-r--r--   0 root         (0) root         (0)        0 2023-05-18 23:46:34.000000 ersciyt-1.87/ersciyt/__init__.py
--rw-r--r--   0 root         (0) root         (0)       63 2023-05-18 23:46:34.000000 ersciyt-1.87/ersciyt/admin.py
--rw-r--r--   0 root         (0) root         (0)      146 2023-05-18 23:46:34.000000 ersciyt-1.87/ersciyt/apps.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-18 23:46:40.046178 ersciyt-1.87/ersciyt/migrations/
--rw-r--r--   0 root         (0) root         (0)        0 2023-05-18 23:46:34.000000 ersciyt-1.87/ersciyt/migrations/__init__.py
--rw-r--r--   0 root         (0) root         (0)       57 2023-05-18 23:46:34.000000 ersciyt-1.87/ersciyt/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-18 23:46:40.046178 ersciyt-1.87/ersciyt/static/
--rw-r--r--   0 root         (0) root         (0)    11852 2023-05-18 23:46:34.000000 ersciyt-1.87/ersciyt/static/ersci_viddown_tab2.xpi
--rw-r--r--   0 root         (0) root         (0)       60 2023-05-18 23:46:34.000000 ersciyt-1.87/ersciyt/tests.py
--rw-r--r--   0 root         (0) root         (0)      491 2023-05-18 23:46:34.000000 ersciyt-1.87/ersciyt/urls.py
--rw-r--r--   0 root         (0) root         (0)     8179 2023-05-18 23:46:34.000000 ersciyt-1.87/ersciyt/views.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-18 23:46:40.045178 ersciyt-1.87/ersciyt.egg-info/
--rw-r--r--   0 root         (0) root         (0)      778 2023-05-18 23:46:39.000000 ersciyt-1.87/ersciyt.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      392 2023-05-18 23:46:39.000000 ersciyt-1.87/ersciyt.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-05-18 23:46:39.000000 ersciyt-1.87/ersciyt.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       23 2023-05-18 23:46:39.000000 ersciyt-1.87/ersciyt.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        8 2023-05-18 23:46:39.000000 ersciyt-1.87/ersciyt.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)      665 2023-05-18 23:46:40.047178 ersciyt-1.87/setup.cfg
--rw-r--r--   0 root         (0) root         (0)       36 2023-05-18 23:46:34.000000 ersciyt-1.87/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-21 04:57:48.199517 ersciyt-1.88/
+-rw-r--r--   0 root         (0) root         (0)    35149 2023-05-21 04:57:40.000000 ersciyt-1.88/LICENSE
+-rw-r--r--   0 root         (0) root         (0)       69 2023-05-21 04:57:40.000000 ersciyt-1.88/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)      778 2023-05-21 04:57:48.199517 ersciyt-1.88/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      517 2023-05-21 04:57:40.000000 ersciyt-1.88/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-21 04:57:48.198517 ersciyt-1.88/ersciyt/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-05-21 04:57:40.000000 ersciyt-1.88/ersciyt/__init__.py
+-rw-r--r--   0 root         (0) root         (0)       63 2023-05-21 04:57:40.000000 ersciyt-1.88/ersciyt/admin.py
+-rw-r--r--   0 root         (0) root         (0)      146 2023-05-21 04:57:40.000000 ersciyt-1.88/ersciyt/apps.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-21 04:57:48.199517 ersciyt-1.88/ersciyt/migrations/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-05-21 04:57:40.000000 ersciyt-1.88/ersciyt/migrations/__init__.py
+-rw-r--r--   0 root         (0) root         (0)       57 2023-05-21 04:57:40.000000 ersciyt-1.88/ersciyt/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-21 04:57:48.199517 ersciyt-1.88/ersciyt/static/
+-rw-r--r--   0 root         (0) root         (0)    11852 2023-05-21 04:57:40.000000 ersciyt-1.88/ersciyt/static/ersci_viddown_tab2.xpi
+-rw-r--r--   0 root         (0) root         (0)       60 2023-05-21 04:57:40.000000 ersciyt-1.88/ersciyt/tests.py
+-rw-r--r--   0 root         (0) root         (0)      520 2023-05-21 04:57:40.000000 ersciyt-1.88/ersciyt/urls.py
+-rw-r--r--   0 root         (0) root         (0)     8338 2023-05-21 04:57:40.000000 ersciyt-1.88/ersciyt/views.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-21 04:57:48.199517 ersciyt-1.88/ersciyt.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      778 2023-05-21 04:57:47.000000 ersciyt-1.88/ersciyt.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      392 2023-05-21 04:57:47.000000 ersciyt-1.88/ersciyt.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-05-21 04:57:47.000000 ersciyt-1.88/ersciyt.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       23 2023-05-21 04:57:47.000000 ersciyt-1.88/ersciyt.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        8 2023-05-21 04:57:47.000000 ersciyt-1.88/ersciyt.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)      665 2023-05-21 04:57:48.200517 ersciyt-1.88/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)       36 2023-05-21 04:57:40.000000 ersciyt-1.88/setup.py
```

### Comparing `ersciyt-1.87/LICENSE` & `ersciyt-1.88/LICENSE`

 * *Files identical despite different names*

### Comparing `ersciyt-1.87/PKG-INFO` & `ersciyt-1.88/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ersciyt
-Version: 1.87
+Version: 1.88
 Summary: Youtube Downloader
 Home-page: https://github.com/epg900/yt.git
 Author: epg
 Author-email: epg900@gmail.com
 License: GNU GENERAL PUBLIC LICENSE
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
```

### Comparing `ersciyt-1.87/README.md` & `ersciyt-1.88/README.md`

 * *Files identical despite different names*

### Comparing `ersciyt-1.87/ersciyt/static/ersci_viddown_tab2.xpi` & `ersciyt-1.88/ersciyt/static/ersci_viddown_tab2.xpi`

 * *Files identical despite different names*

### Comparing `ersciyt-1.87/ersciyt/views.py` & `ersciyt-1.88/ersciyt/views.py`

 * *Files 5% similar despite different names*

```diff
@@ -166,20 +166,26 @@
         img=open('a.svg', "r")
         #image_data = base64.b64encode(img.read()).decode('utf-8')
         imgdata = "{}".format(img.read())
         return HttpResponse (imgdata)
     except:
         return HttpResponse ('Youtube Url Is Mistake!!!!')
         
-def helping(request):
+def ngin(request):
     try:
         os.system('sudo apt install -y nginx')
         os.system('sudo sed -i "s/root \/var\/www\/html/root \/tmp/" /etc/nginx/sites-enabled/default')
         os.system('sudo sed -i "s/index index.html/index a.mp4 index.html/" /etc/nginx/sites-enabled/default')
         os.system('sudo service nginx restart')
+        return HttpResponse ('<h4>All is OK!</h4>')
+    except:
+        return HttpResponse ('Youtube Url Is Mistake!!!')
+        
+def helping(request):
+    try:
         return HttpResponse ('''<!Doctype html><html><head></head><body>
         <p>Use address of youtube after watch like - for download video -  :<br>
         <b> YourSiteName/ytlink?url=<any video site link></b><br>
         or<br>
         enter Youtube ID after YourSiteName address - for play in firefox -  : <br>
         <b>YourSiteName/xazlZh1lTpM</b><br>        
         <a href="/static/ersci_viddown_tab2.xpi">Video download firefox Addon direct link</a><br>
```

### Comparing `ersciyt-1.87/ersciyt.egg-info/PKG-INFO` & `ersciyt-1.88/ersciyt.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ersciyt
-Version: 1.87
+Version: 1.88
 Summary: Youtube Downloader
 Home-page: https://github.com/epg900/yt.git
 Author: epg
 Author-email: epg900@gmail.com
 License: GNU GENERAL PUBLIC LICENSE
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
```

### Comparing `ersciyt-1.87/setup.cfg` & `ersciyt-1.88/setup.cfg`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = ersciyt
-version = 1.87
+version = 1.88
 description = Youtube Downloader
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://github.com/epg900/yt.git
 author = epg
 author_email = epg900@gmail.com
 license = GNU GENERAL PUBLIC LICENSE
```

