# Comparing `tmp/lantana-2.6.4.tar.gz` & `tmp/lantana-2.6.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\lantana-2.6.4.tar", last modified: Sun May 21 05:58:47 2023, max compression
+gzip compressed data, was "dist\lantana-2.6.5.tar", last modified: Sun May 21 06:06:09 2023, max compression
```

## Comparing `lantana-2.6.4.tar` & `lantana-2.6.5.tar`

### file list

```diff
@@ -1,37 +1,37 @@
-drwxrwxrwx   0        0        0        0 2023-05-21 05:58:47.000000 lantana-2.6.4/
-drwxrwxrwx   0        0        0        0 2023-05-21 05:58:47.000000 lantana-2.6.4/lantana/
--rw-rw-rw-   0        0        0      547 2022-10-28 12:09:36.000000 lantana-2.6.4/lantana/404.html
--rw-rw-rw-   0        0        0     9850 2023-03-05 11:52:40.000000 lantana-2.6.4/lantana/base.html
--rw-rw-rw-   0        0        0      306 2022-10-28 12:09:36.000000 lantana-2.6.4/lantana/breadcrumb.html
-drwxrwxrwx   0        0        0        0 2023-05-21 05:58:47.000000 lantana-2.6.4/lantana/css/
--rw-rw-rw-   0        0        0     2705 2023-03-05 11:56:33.000000 lantana-2.6.4/lantana/css/theme.css
-drwxrwxrwx   0        0        0        0 2023-05-21 05:58:47.000000 lantana-2.6.4/lantana/extensions/
--rw-rw-rw-   0        0        0     3125 2023-03-08 12:20:00.000000 lantana-2.6.4/lantana/extensions/mdx_cards.py
--rw-rw-rw-   0        0        0     1996 2022-11-27 08:35:47.000000 lantana-2.6.4/lantana/extensions/mdx_embedly.py
--rw-rw-rw-   0        0        0     2138 2023-03-08 08:22:38.000000 lantana-2.6.4/lantana/extensions/mdx_wsid.py
--rw-rw-rw-   0        0        0        0 2022-10-28 12:09:36.000000 lantana-2.6.4/lantana/extensions/__init__.py
--rw-rw-rw-   0        0        0     1784 2022-10-28 12:09:36.000000 lantana-2.6.4/lantana/favicon.png
--rw-rw-rw-   0        0        0     4486 2022-10-28 12:09:36.000000 lantana-2.6.4/lantana/favicon.svg
-drwxrwxrwx   0        0        0        0 2023-05-21 05:58:47.000000 lantana-2.6.4/lantana/js/
--rw-rw-rw-   0        0        0     5746 2023-03-05 11:57:02.000000 lantana-2.6.4/lantana/js/theme.js
--rw-rw-rw-   0        0        0     5285 2023-01-15 11:10:45.000000 lantana-2.6.4/lantana/main.html
--rw-rw-rw-   0        0        0      360 2023-02-09 08:21:12.000000 lantana-2.6.4/lantana/mkdocs_theme.yml
--rw-rw-rw-   0        0        0      843 2023-03-04 05:20:30.000000 lantana-2.6.4/lantana/nav.html
--rw-rw-rw-   0        0        0      536 2022-11-07 12:37:39.000000 lantana-2.6.4/lantana/sitemap.html
--rw-rw-rw-   0        0        0     1994 2023-03-08 12:20:18.000000 lantana-2.6.4/lantana/statics.html
--rw-rw-rw-   0        0        0      368 2023-02-16 13:48:35.000000 lantana-2.6.4/lantana/toc.html
--rw-rw-rw-   0        0        0        0 2022-10-28 12:09:36.000000 lantana-2.6.4/lantana/__init__.py
--rw-rw-rw-   0        0        0     2682 2022-12-01 09:12:15.000000 lantana-2.6.4/lantana/__main__.py
-drwxrwxrwx   0        0        0        0 2023-05-21 05:58:47.000000 lantana-2.6.4/lantana.egg-info/
--rw-rw-rw-   0        0        0        1 2023-05-21 05:58:47.000000 lantana-2.6.4/lantana.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      279 2023-05-21 05:58:47.000000 lantana-2.6.4/lantana.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0        2 2023-05-21 05:58:47.000000 lantana-2.6.4/lantana.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0      266 2023-05-21 05:58:47.000000 lantana-2.6.4/lantana.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      225 2023-05-21 05:58:47.000000 lantana-2.6.4/lantana.egg-info/requires.txt
--rw-rw-rw-   0        0        0      676 2023-05-21 05:58:47.000000 lantana-2.6.4/lantana.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        8 2023-05-21 05:58:47.000000 lantana-2.6.4/lantana.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      124 2022-10-28 12:09:36.000000 lantana-2.6.4/MANIFEST.in
--rw-rw-rw-   0        0        0      266 2023-05-21 05:58:47.000000 lantana-2.6.4/PKG-INFO
--rw-rw-rw-   0        0        0     1212 2023-03-04 05:20:30.000000 lantana-2.6.4/README.md
--rw-rw-rw-   0        0        0       42 2023-05-21 05:58:47.000000 lantana-2.6.4/setup.cfg
--rw-rw-rw-   0        0        0     1130 2023-05-21 05:58:43.000000 lantana-2.6.4/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-21 06:06:09.000000 lantana-2.6.5/
+drwxrwxrwx   0        0        0        0 2023-05-21 06:06:09.000000 lantana-2.6.5/lantana/
+-rw-rw-rw-   0        0        0      547 2022-10-28 12:09:36.000000 lantana-2.6.5/lantana/404.html
+-rw-rw-rw-   0        0        0     9850 2023-03-05 11:52:40.000000 lantana-2.6.5/lantana/base.html
+-rw-rw-rw-   0        0        0      306 2022-10-28 12:09:36.000000 lantana-2.6.5/lantana/breadcrumb.html
+drwxrwxrwx   0        0        0        0 2023-05-21 06:06:09.000000 lantana-2.6.5/lantana/css/
+-rw-rw-rw-   0        0        0     2705 2023-03-05 11:56:33.000000 lantana-2.6.5/lantana/css/theme.css
+drwxrwxrwx   0        0        0        0 2023-05-21 06:06:09.000000 lantana-2.6.5/lantana/extensions/
+-rw-rw-rw-   0        0        0     3125 2023-03-08 12:20:00.000000 lantana-2.6.5/lantana/extensions/mdx_cards.py
+-rw-rw-rw-   0        0        0     1996 2022-11-27 08:35:47.000000 lantana-2.6.5/lantana/extensions/mdx_embedly.py
+-rw-rw-rw-   0        0        0     2138 2023-03-08 08:22:38.000000 lantana-2.6.5/lantana/extensions/mdx_wsid.py
+-rw-rw-rw-   0        0        0        0 2022-10-28 12:09:36.000000 lantana-2.6.5/lantana/extensions/__init__.py
+-rw-rw-rw-   0        0        0     1784 2022-10-28 12:09:36.000000 lantana-2.6.5/lantana/favicon.png
+-rw-rw-rw-   0        0        0     4486 2022-10-28 12:09:36.000000 lantana-2.6.5/lantana/favicon.svg
+drwxrwxrwx   0        0        0        0 2023-05-21 06:06:09.000000 lantana-2.6.5/lantana/js/
+-rw-rw-rw-   0        0        0     5746 2023-03-05 11:57:02.000000 lantana-2.6.5/lantana/js/theme.js
+-rw-rw-rw-   0        0        0     5285 2023-01-15 11:10:45.000000 lantana-2.6.5/lantana/main.html
+-rw-rw-rw-   0        0        0      360 2023-02-09 08:21:12.000000 lantana-2.6.5/lantana/mkdocs_theme.yml
+-rw-rw-rw-   0        0        0      843 2023-03-04 05:20:30.000000 lantana-2.6.5/lantana/nav.html
+-rw-rw-rw-   0        0        0      536 2022-11-07 12:37:39.000000 lantana-2.6.5/lantana/sitemap.html
+-rw-rw-rw-   0        0        0     1994 2023-05-21 06:06:01.000000 lantana-2.6.5/lantana/statics.html
+-rw-rw-rw-   0        0        0      368 2023-02-16 13:48:35.000000 lantana-2.6.5/lantana/toc.html
+-rw-rw-rw-   0        0        0        0 2022-10-28 12:09:36.000000 lantana-2.6.5/lantana/__init__.py
+-rw-rw-rw-   0        0        0     2682 2022-12-01 09:12:15.000000 lantana-2.6.5/lantana/__main__.py
+drwxrwxrwx   0        0        0        0 2023-05-21 06:06:09.000000 lantana-2.6.5/lantana.egg-info/
+-rw-rw-rw-   0        0        0        1 2023-05-21 06:06:09.000000 lantana-2.6.5/lantana.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      279 2023-05-21 06:06:09.000000 lantana-2.6.5/lantana.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0        2 2023-05-21 06:06:09.000000 lantana-2.6.5/lantana.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0      266 2023-05-21 06:06:09.000000 lantana-2.6.5/lantana.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      224 2023-05-21 06:06:09.000000 lantana-2.6.5/lantana.egg-info/requires.txt
+-rw-rw-rw-   0        0        0      676 2023-05-21 06:06:09.000000 lantana-2.6.5/lantana.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        8 2023-05-21 06:06:09.000000 lantana-2.6.5/lantana.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      124 2022-10-28 12:09:36.000000 lantana-2.6.5/MANIFEST.in
+-rw-rw-rw-   0        0        0      266 2023-05-21 06:06:09.000000 lantana-2.6.5/PKG-INFO
+-rw-rw-rw-   0        0        0     1212 2023-03-04 05:20:30.000000 lantana-2.6.5/README.md
+-rw-rw-rw-   0        0        0       42 2023-05-21 06:06:09.000000 lantana-2.6.5/setup.cfg
+-rw-rw-rw-   0        0        0     1129 2023-05-21 06:05:46.000000 lantana-2.6.5/setup.py
```

### Comparing `lantana-2.6.4/lantana/404.html` & `lantana-2.6.5/lantana/404.html`

 * *Files identical despite different names*

### Comparing `lantana-2.6.4/lantana/base.html` & `lantana-2.6.5/lantana/base.html`

 * *Files identical despite different names*

### Comparing `lantana-2.6.4/lantana/css/theme.css` & `lantana-2.6.5/lantana/css/theme.css`

 * *Files identical despite different names*

### Comparing `lantana-2.6.4/lantana/extensions/mdx_cards.py` & `lantana-2.6.5/lantana/extensions/mdx_cards.py`

 * *Files identical despite different names*

### Comparing `lantana-2.6.4/lantana/extensions/mdx_embedly.py` & `lantana-2.6.5/lantana/extensions/mdx_embedly.py`

 * *Files identical despite different names*

### Comparing `lantana-2.6.4/lantana/extensions/mdx_wsid.py` & `lantana-2.6.5/lantana/extensions/mdx_wsid.py`

 * *Files identical despite different names*

### Comparing `lantana-2.6.4/lantana/favicon.png` & `lantana-2.6.5/lantana/favicon.png`

 * *Files identical despite different names*

### Comparing `lantana-2.6.4/lantana/favicon.svg` & `lantana-2.6.5/lantana/favicon.svg`

 * *Files identical despite different names*

### Comparing `lantana-2.6.4/lantana/js/theme.js` & `lantana-2.6.5/lantana/js/theme.js`

 * *Files identical despite different names*

### Comparing `lantana-2.6.4/lantana/main.html` & `lantana-2.6.5/lantana/main.html`

 * *Files identical despite different names*

### Comparing `lantana-2.6.4/lantana/nav.html` & `lantana-2.6.5/lantana/nav.html`

 * *Files identical despite different names*

### Comparing `lantana-2.6.4/lantana/sitemap.html` & `lantana-2.6.5/lantana/sitemap.html`

 * *Files identical despite different names*

### Comparing `lantana-2.6.4/lantana/statics.html` & `lantana-2.6.5/lantana/statics.html`

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
-        <td>WSOFT Lantana v2.6.2(tapioca)</td>
+        <td>WSOFT Lantana v2.6.5(tapioca)</td>
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
-Lantanaã®ãã¼ã¸ã§ã�WSOFT Lantana v2.6.2
+Lantanaã®ãã¼ã¸ã§ã�WSOFT Lantana v2.6.5
                                         (tapioca)
 MkDocsã®ãã¼ã¸ã§ã{{ mkdocs_version }}
 Lantana
 Copyright 2022 WSOFT. All rights reserved.
 Lantanaã¯MkDocsããã®ä»ã®ãªã¼ãã³ã½ã¼ã¹
 ã½ããã¦ã§ã¢ã«ãã£ã¦å®ç¾ãã¾ããã
 Lantanaã®ãã¼ã ãã¼ã¸/GitHubãªãã¸ããª/WSOFTã®ãµã¤ã
```

### Comparing `lantana-2.6.4/lantana/__main__.py` & `lantana-2.6.5/lantana/__main__.py`

 * *Files identical despite different names*

### Comparing `lantana-2.6.4/lantana.egg-info/SOURCES.txt` & `lantana-2.6.5/lantana.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `lantana-2.6.4/README.md` & `lantana-2.6.5/README.md`

 * *Files identical despite different names*

### Comparing `lantana-2.6.4/setup.py` & `lantana-2.6.5/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 from setuptools import setup, find_packages
 
-VERSION = '2.6.4'
+VERSION = '2.6.5'
 
 setup(
     name="lantana",
     version=VERSION,
     url='http://wsoft-project.github.io/lantana/',
     license='MIT',
     description='Bootstrap theme for MkDocs',
     author='WSOFT',
     author_email='info@wsoft.ws',
     packages=find_packages(),
     include_package_data=True,
-    install_requires=[ 'markdown>=3.4','mkdocs>=1.1','mkdocs-material>=7.0','mkdocs-awesome-pages-plugin>=2.3','mkdocs-macros-plugin>=0.6.3','mkdocs-git-authors-plugin>=0.6.2','mkdocs-mermaid2-plugin>=0.5.0','mkdocs-git-revision-date-plugin>=0.3.1','natsort>=8.3.1'],
+    install_requires=[ 'markdown<3.4','mkdocs>=1.1','mkdocs-material>=7.0','mkdocs-awesome-pages-plugin>=2.3','mkdocs-macros-plugin>=0.6.3','mkdocs-git-authors-plugin>=0.6.2','mkdocs-mermaid2-plugin>=0.5.0','mkdocs-git-revision-date-plugin>=0.3.1','natsort>=8.3.1'],
     python_requires='>=3.5',
     entry_points={
         'mkdocs.themes': [
             'lantana = lantana',
         ],
         "console_scripts":[
             'lantana = lantana.__main__:cli',
```

