# Comparing `tmp/lantana-2.6.5.tar.gz` & `tmp/lantana-2.6.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\lantana-2.6.5.tar", last modified: Sun May 21 06:06:09 2023, max compression
+gzip compressed data, was "dist\lantana-2.6.6.tar", last modified: Sun May 21 07:10:25 2023, max compression
```

## Comparing `lantana-2.6.5.tar` & `lantana-2.6.6.tar`

### file list

```diff
@@ -1,37 +1,45 @@
-drwxrwxrwx   0        0        0        0 2023-05-21 06:06:09.000000 lantana-2.6.5/
-drwxrwxrwx   0        0        0        0 2023-05-21 06:06:09.000000 lantana-2.6.5/lantana/
--rw-rw-rw-   0        0        0      547 2022-10-28 12:09:36.000000 lantana-2.6.5/lantana/404.html
--rw-rw-rw-   0        0        0     9850 2023-03-05 11:52:40.000000 lantana-2.6.5/lantana/base.html
--rw-rw-rw-   0        0        0      306 2022-10-28 12:09:36.000000 lantana-2.6.5/lantana/breadcrumb.html
-drwxrwxrwx   0        0        0        0 2023-05-21 06:06:09.000000 lantana-2.6.5/lantana/css/
--rw-rw-rw-   0        0        0     2705 2023-03-05 11:56:33.000000 lantana-2.6.5/lantana/css/theme.css
-drwxrwxrwx   0        0        0        0 2023-05-21 06:06:09.000000 lantana-2.6.5/lantana/extensions/
--rw-rw-rw-   0        0        0     3125 2023-03-08 12:20:00.000000 lantana-2.6.5/lantana/extensions/mdx_cards.py
--rw-rw-rw-   0        0        0     1996 2022-11-27 08:35:47.000000 lantana-2.6.5/lantana/extensions/mdx_embedly.py
--rw-rw-rw-   0        0        0     2138 2023-03-08 08:22:38.000000 lantana-2.6.5/lantana/extensions/mdx_wsid.py
--rw-rw-rw-   0        0        0        0 2022-10-28 12:09:36.000000 lantana-2.6.5/lantana/extensions/__init__.py
--rw-rw-rw-   0        0        0     1784 2022-10-28 12:09:36.000000 lantana-2.6.5/lantana/favicon.png
--rw-rw-rw-   0        0        0     4486 2022-10-28 12:09:36.000000 lantana-2.6.5/lantana/favicon.svg
-drwxrwxrwx   0        0        0        0 2023-05-21 06:06:09.000000 lantana-2.6.5/lantana/js/
--rw-rw-rw-   0        0        0     5746 2023-03-05 11:57:02.000000 lantana-2.6.5/lantana/js/theme.js
--rw-rw-rw-   0        0        0     5285 2023-01-15 11:10:45.000000 lantana-2.6.5/lantana/main.html
--rw-rw-rw-   0        0        0      360 2023-02-09 08:21:12.000000 lantana-2.6.5/lantana/mkdocs_theme.yml
--rw-rw-rw-   0        0        0      843 2023-03-04 05:20:30.000000 lantana-2.6.5/lantana/nav.html
--rw-rw-rw-   0        0        0      536 2022-11-07 12:37:39.000000 lantana-2.6.5/lantana/sitemap.html
--rw-rw-rw-   0        0        0     1994 2023-05-21 06:06:01.000000 lantana-2.6.5/lantana/statics.html
--rw-rw-rw-   0        0        0      368 2023-02-16 13:48:35.000000 lantana-2.6.5/lantana/toc.html
--rw-rw-rw-   0        0        0        0 2022-10-28 12:09:36.000000 lantana-2.6.5/lantana/__init__.py
--rw-rw-rw-   0        0        0     2682 2022-12-01 09:12:15.000000 lantana-2.6.5/lantana/__main__.py
-drwxrwxrwx   0        0        0        0 2023-05-21 06:06:09.000000 lantana-2.6.5/lantana.egg-info/
--rw-rw-rw-   0        0        0        1 2023-05-21 06:06:09.000000 lantana-2.6.5/lantana.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      279 2023-05-21 06:06:09.000000 lantana-2.6.5/lantana.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0        2 2023-05-21 06:06:09.000000 lantana-2.6.5/lantana.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0      266 2023-05-21 06:06:09.000000 lantana-2.6.5/lantana.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      224 2023-05-21 06:06:09.000000 lantana-2.6.5/lantana.egg-info/requires.txt
--rw-rw-rw-   0        0        0      676 2023-05-21 06:06:09.000000 lantana-2.6.5/lantana.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        8 2023-05-21 06:06:09.000000 lantana-2.6.5/lantana.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      124 2022-10-28 12:09:36.000000 lantana-2.6.5/MANIFEST.in
--rw-rw-rw-   0        0        0      266 2023-05-21 06:06:09.000000 lantana-2.6.5/PKG-INFO
--rw-rw-rw-   0        0        0     1212 2023-03-04 05:20:30.000000 lantana-2.6.5/README.md
--rw-rw-rw-   0        0        0       42 2023-05-21 06:06:09.000000 lantana-2.6.5/setup.cfg
--rw-rw-rw-   0        0        0     1129 2023-05-21 06:05:46.000000 lantana-2.6.5/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-21 07:10:25.000000 lantana-2.6.6/
+drwxrwxrwx   0        0        0        0 2023-05-21 07:10:24.000000 lantana-2.6.6/lantana/
+-rw-rw-rw-   0        0        0      547 2022-10-28 12:09:36.000000 lantana-2.6.6/lantana/404.html
+-rw-rw-rw-   0        0        0     8998 2023-05-21 07:10:20.000000 lantana-2.6.6/lantana/base.html
+-rw-rw-rw-   0        0        0      306 2022-10-28 12:09:36.000000 lantana-2.6.6/lantana/breadcrumb.html
+drwxrwxrwx   0        0        0        0 2023-05-21 07:10:25.000000 lantana-2.6.6/lantana/css/
+-rw-rw-rw-   0        0        0   210062 2023-05-21 06:29:23.000000 lantana-2.6.6/lantana/css/bootstrap-dark.min.css
+-rw-rw-rw-   0        0        0    83555 2023-05-21 06:33:38.000000 lantana-2.6.6/lantana/css/bootstrap-icons.min.css
+-rw-rw-rw-   0        0        0   155850 2023-05-21 06:31:31.000000 lantana-2.6.6/lantana/css/bootstrap.min.css
+-rw-rw-rw-   0        0        0     1152 2023-05-21 06:34:35.000000 lantana-2.6.6/lantana/css/default.min.css
+-rw-rw-rw-   0        0        0     2705 2023-03-05 11:56:33.000000 lantana-2.6.6/lantana/css/theme.css
+-rw-rw-rw-   0        0        0     1927 2023-05-21 06:35:24.000000 lantana-2.6.6/lantana/css/vs.min.css
+drwxrwxrwx   0        0        0        0 2023-05-21 07:10:25.000000 lantana-2.6.6/lantana/extensions/
+-rw-rw-rw-   0        0        0     3125 2023-03-08 12:20:00.000000 lantana-2.6.6/lantana/extensions/mdx_cards.py
+-rw-rw-rw-   0        0        0     1996 2022-11-27 08:35:47.000000 lantana-2.6.6/lantana/extensions/mdx_embedly.py
+-rw-rw-rw-   0        0        0     2138 2023-03-08 08:22:38.000000 lantana-2.6.6/lantana/extensions/mdx_wsid.py
+-rw-rw-rw-   0        0        0        0 2022-10-28 12:09:36.000000 lantana-2.6.6/lantana/extensions/__init__.py
+-rw-rw-rw-   0        0        0     1784 2022-10-28 12:09:36.000000 lantana-2.6.6/lantana/favicon.png
+-rw-rw-rw-   0        0        0     4486 2022-10-28 12:09:36.000000 lantana-2.6.6/lantana/favicon.svg
+drwxrwxrwx   0        0        0        0 2023-05-21 07:10:25.000000 lantana-2.6.6/lantana/js/
+-rw-rw-rw-   0        0        0    78749 2023-05-21 06:58:58.000000 lantana-2.6.6/lantana/js/bootstrap.bundle.min.js
+-rw-rw-rw-   0        0        0   126355 2023-05-21 06:59:30.000000 lantana-2.6.6/lantana/js/highlight.min.js
+-rw-rw-rw-   0        0        0    72535 2023-05-21 06:58:42.000000 lantana-2.6.6/lantana/js/jquery-3.6.1.slim.min.js
+-rw-rw-rw-   0        0        0     5746 2023-03-05 11:57:02.000000 lantana-2.6.6/lantana/js/theme.js
+-rw-rw-rw-   0        0        0     5285 2023-01-15 11:10:45.000000 lantana-2.6.6/lantana/main.html
+-rw-rw-rw-   0        0        0      360 2023-02-09 08:21:12.000000 lantana-2.6.6/lantana/mkdocs_theme.yml
+-rw-rw-rw-   0        0        0      843 2023-03-04 05:20:30.000000 lantana-2.6.6/lantana/nav.html
+-rw-rw-rw-   0        0        0      536 2022-11-07 12:37:39.000000 lantana-2.6.6/lantana/sitemap.html
+-rw-rw-rw-   0        0        0     1994 2023-05-21 07:00:03.000000 lantana-2.6.6/lantana/statics.html
+-rw-rw-rw-   0        0        0      368 2023-02-16 13:48:35.000000 lantana-2.6.6/lantana/toc.html
+-rw-rw-rw-   0        0        0        0 2022-10-28 12:09:36.000000 lantana-2.6.6/lantana/__init__.py
+-rw-rw-rw-   0        0        0     2682 2022-12-01 09:12:15.000000 lantana-2.6.6/lantana/__main__.py
+drwxrwxrwx   0        0        0        0 2023-05-21 07:10:25.000000 lantana-2.6.6/lantana.egg-info/
+-rw-rw-rw-   0        0        0        1 2023-05-21 07:10:24.000000 lantana-2.6.6/lantana.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      279 2023-05-21 07:10:24.000000 lantana-2.6.6/lantana.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0        2 2023-05-21 07:10:24.000000 lantana-2.6.6/lantana.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0      266 2023-05-21 07:10:24.000000 lantana-2.6.6/lantana.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      224 2023-05-21 07:10:24.000000 lantana-2.6.6/lantana.egg-info/requires.txt
+-rw-rw-rw-   0        0        0      927 2023-05-21 07:10:24.000000 lantana-2.6.6/lantana.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        8 2023-05-21 07:10:24.000000 lantana-2.6.6/lantana.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      124 2022-10-28 12:09:36.000000 lantana-2.6.6/MANIFEST.in
+-rw-rw-rw-   0        0        0      266 2023-05-21 07:10:25.000000 lantana-2.6.6/PKG-INFO
+-rw-rw-rw-   0        0        0     1212 2023-03-04 05:20:30.000000 lantana-2.6.6/README.md
+-rw-rw-rw-   0        0        0       42 2023-05-21 07:10:25.000000 lantana-2.6.6/setup.cfg
+-rw-rw-rw-   0        0        0     1129 2023-05-21 07:00:00.000000 lantana-2.6.6/setup.py
```

### Comparing `lantana-2.6.5/lantana/404.html` & `lantana-2.6.6/lantana/404.html`

 * *Files identical despite different names*

### Comparing `lantana-2.6.5/lantana/base.html` & `lantana-2.6.6/lantana/base.html`

 * *Files 8% similar despite different names*

```diff
@@ -41,40 +41,31 @@
     <title>{% if page.title %}{{ page.title }} | {% endif %}{{ config.site_name }}</title>
   {% endif %}
 
   {% if config.favicon %}
     <link rel="favicon" href="{{ config.favicon|url }}">
   {% endif %}
 
-  {% if config.google_analytics %}
-    <script async async src="https://www.googletagmanager.com/gtag/js?id={{config.google_analytics}}"></script>
-    <script async>
-        window.dataLayer = window.dataLayer || [];
-        function gtag(){dataLayer.push(arguments);}
-        gtag('js', new Date());
-        gtag('config', '{{config.google_analytics}}');
-    </script>
-  {% endif %}
-  <link href="https://cdn.jsdelivr.net/npm/bootstrap-dark-5@1.1.3/dist/css/bootstrap-dark.min.css" rel="stylesheet" media="not print">
-  <link href="https://cdn.jsdelivr.net/npm/bootstrap@5.0.2/dist/css/bootstrap.min.css" rel="stylesheet" media="print">
-  <link rel="stylesheet" href="https://cdn.jsdelivr.net/npm/bootstrap-icons@1.10.2/font/bootstrap-icons.css">
-  <link rel="stylesheet" href="//cdn.jsdelivr.net/gh/highlightjs/cdn-release@11.6.0/build/styles/default.min.css">
-  <link rel="stylesheet" href="https://cdn.jsdelivr.net/npm/pygments-rouge-css@0.1.0/vs.min.css">
+  <link rel="stylesheet" href="{{ "css/bootstrap.min.css"|url }}" media="print">
+  <link rel="stylesheet" href="{{ "css/bootstrap-dark.min.css"|url }}" media="not print">
+  <link rel="stylesheet" href="https://cdn.jsdelivr.net/npm/bootstrap-icons@1.8.0/font/bootstrap-icons.css">
+  <link rel="stylesheet" href="{{ "css/default.min.css"|url }}">
+  <link rel="stylesheet" href="{{ "css/vs.min.css"|url }}">
   <link rel="stylesheet" href="{{ "css/theme.css"|url }}">
   {% for path in config.extra_css %}
     <link href="{{ path|url }}" rel="stylesheet">
   {% endfor %}
   {% for path2 in page.extra_css %}
     <link href="{{ path2|url }}" rel="stylesheet">
   {% endfor %}
   
   <script async>var base_url = '{{ base_url }}';</script>
-  <script src="https://code.jquery.com/jquery-3.6.1.slim.min.js" integrity="sha256-w8CvhFs7iHNVUtnSP0YKEg00p9Ih13rlL9zGqvLdePA=" crossorigin="anonymous"></script>
-  <script src="https://cdn.jsdelivr.net/npm/bootstrap@5.0.2/dist/js/bootstrap.bundle.min.js" integrity="sha384-MrcW6ZMFYlzcLA8Nl+NtUVF0sA7MsXsP1UyJoMp4YLEuNSfAP+JcXn/tWtIaxVXM" crossorigin="anonymous"></script>
-  <script async src="//cdn.jsdelivr.net/gh/highlightjs/cdn-release@11.6.0/build/highlight.min.js"></script>
+  <script src="{{ "js/jquery-3.6.1.slim.min.js"|url }}"></script>
+  <script src="{{ "js/bootstrap.bundle.min.js"|url }}"></script>
+  <script async src="{{ "js/highlight.min.js"|url }}"></script>
 
   {% block extrahead %}
   {% endblock %}
 </head>
 <body>
   {% if not config.disable_header %}
     <header>
```

#### html2text {}

```diff
@@ -16,25 +16,28 @@
 
 
  {% endif %} {% if page and page.meta.image %}
  {% else %}
  {% endif %} {% endif %} {% if config.site_short_name %}
 {% else %}
 {% endif %} {% if config.favicon %}
- {% endif %} {% if config.google_analytics %}
  {% endif %}
+ootstrap.min.css"|url }}" media="print">
+ootstrap-dark.min.css"|url }}" media="not print">
 
-
-
-
-
+efault.min.css"|url }}">
+s.min.css"|url }}">
 heme.css"|url }}"> {% for path in config.extra_css %}
  {% endfor %} {% for path2 in page.extra_css %}
  {% endfor %}
- {% block extrahead %} {% endblock %}
+
+query-3.6.1.slim.min.js"|url }}">
+ootstrap.bundle.min.js"|url }}">
+ighlight.min.js"|url }}">
+{% block extrahead %} {% endblock %}
 {% if not config.disable_header %}
 |url }}"> {% if config.logo %} [{{ config.site_name }}] {% endif%} {% if
 config.header_name %} {{ config.header_name }} {% else %} {{ config.site_name
 }} {% endif %}
 {% if config.visible_search!=false %} [Unknown INPUT type]    {% endif %}
 
 {% if page and page.meta.disable_nav %}  {% else %}  {% endif %} {% if
```

### Comparing `lantana-2.6.5/lantana/css/theme.css` & `lantana-2.6.6/lantana/css/theme.css`

 * *Files identical despite different names*

### Comparing `lantana-2.6.5/lantana/extensions/mdx_cards.py` & `lantana-2.6.6/lantana/extensions/mdx_cards.py`

 * *Files identical despite different names*

### Comparing `lantana-2.6.5/lantana/extensions/mdx_embedly.py` & `lantana-2.6.6/lantana/extensions/mdx_embedly.py`

 * *Files identical despite different names*

### Comparing `lantana-2.6.5/lantana/extensions/mdx_wsid.py` & `lantana-2.6.6/lantana/extensions/mdx_wsid.py`

 * *Files identical despite different names*

### Comparing `lantana-2.6.5/lantana/favicon.png` & `lantana-2.6.6/lantana/favicon.png`

 * *Files identical despite different names*

### Comparing `lantana-2.6.5/lantana/favicon.svg` & `lantana-2.6.6/lantana/favicon.svg`

 * *Files identical despite different names*

### Comparing `lantana-2.6.5/lantana/js/theme.js` & `lantana-2.6.6/lantana/js/theme.js`

 * *Files identical despite different names*

### Comparing `lantana-2.6.5/lantana/main.html` & `lantana-2.6.6/lantana/main.html`

 * *Files identical despite different names*

### Comparing `lantana-2.6.5/lantana/nav.html` & `lantana-2.6.6/lantana/nav.html`

 * *Files identical despite different names*

### Comparing `lantana-2.6.5/lantana/sitemap.html` & `lantana-2.6.6/lantana/sitemap.html`

 * *Files identical despite different names*

### Comparing `lantana-2.6.5/lantana/statics.html` & `lantana-2.6.6/lantana/statics.html`

 * *Files 0% similar despite different names*

```diff
@@ -35,15 +35,15 @@
       <tr>
         <th scope="row">リポジトリ</th>
         <td colspan="2"><a href="{{ config.repo_url }}">{% if config.repo_name %}{{ config.repo_name }}{% else %}{{ config.repo_url }}{% endif %}</a></td>
       </tr>
       {% endif %}
       <tr>
         <th scope="row">Lantanaのバージョン</th>
-        <td>WSOFT Lantana v2.6.5(tapioca)</td>
+        <td>WSOFT Lantana v2.6.6(tapioca)</td>
       </tr>
       <tr>
         <th scope="row">MkDocsのバージョン</th>
         <td>{{ mkdocs_version }}</td>
       </tr>
     </tbody>
   </table>
```

#### html2text {}

```diff
@@ -6,15 +6,15 @@
                                         }}
 è¨äºã®ç·æ°          {{ ns.cnt }}
 ãµã¤ãã®æçµæ{{ build_date_utc }}
 ãµã¤ãã®ä½è    {{ config.author }}
                                         {%_if_config.repo_name_%}{
 ãªãã¸ããª          {_config.repo_name_}}{%_else_%}{
                                         {_config.repo_url_}}{%_endif_%}
-Lantanaã®ãã¼ã¸ã§ã�WSOFT Lantana v2.6.5
+Lantanaã®ãã¼ã¸ã§ã�WSOFT Lantana v2.6.6
                                         (tapioca)
 MkDocsã®ãã¼ã¸ã§ã{{ mkdocs_version }}
 Lantana
 Copyright 2022 WSOFT. All rights reserved.
 Lantanaã¯MkDocsããã®ä»ã®ãªã¼ãã³ã½ã¼ã¹
 ã½ããã¦ã§ã¢ã«ãã£ã¦å®ç¾ãã¾ããã
 Lantanaã®ãã¼ã ãã¼ã¸/GitHubãªãã¸ããª/WSOFTã®ãµã¤ã
```

### Comparing `lantana-2.6.5/lantana/__main__.py` & `lantana-2.6.6/lantana/__main__.py`

 * *Files identical despite different names*

### Comparing `lantana-2.6.5/README.md` & `lantana-2.6.6/README.md`

 * *Files identical despite different names*

### Comparing `lantana-2.6.5/setup.py` & `lantana-2.6.6/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from setuptools import setup, find_packages
 
-VERSION = '2.6.5'
+VERSION = '2.6.6'
 
 setup(
     name="lantana",
     version=VERSION,
     url='http://wsoft-project.github.io/lantana/',
     license='MIT',
     description='Bootstrap theme for MkDocs',
```

