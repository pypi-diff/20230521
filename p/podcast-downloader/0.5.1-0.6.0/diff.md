# Comparing `tmp/podcast_downloader-0.5.1.tar.gz` & `tmp/podcast_downloader-0.6.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "podcast_downloader-0.5.1.tar", last modified: Fri May 12 20:08:14 2023, max compression
+gzip compressed data, was "podcast_downloader-0.6.0.tar", last modified: Sun May 21 16:49:31 2023, max compression
```

## Comparing `podcast_downloader-0.5.1.tar` & `podcast_downloader-0.6.0.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 20:08:14.695814 podcast_downloader-0.5.1/
--rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-05-12 20:08:04.000000 podcast_downloader-0.5.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     9787 2023-05-12 20:08:14.695814 podcast_downloader-0.5.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     9200 2023-05-12 20:08:04.000000 podcast_downloader-0.5.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 20:08:14.695814 podcast_downloader-0.5.1/podcast_downloader/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-12 20:08:04.000000 podcast_downloader-0.5.1/podcast_downloader/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8563 2023-05-12 20:08:04.000000 podcast_downloader-0.5.1/podcast_downloader/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3243 2023-05-12 20:08:04.000000 podcast_downloader-0.5.1/podcast_downloader/configuration.py
--rw-r--r--   0 runner    (1001) docker     (123)      968 2023-05-12 20:08:04.000000 podcast_downloader-0.5.1/podcast_downloader/downloaded.py
--rw-r--r--   0 runner    (1001) docker     (123)      651 2023-05-12 20:08:04.000000 podcast_downloader-0.5.1/podcast_downloader/parameters.py
--rw-r--r--   0 runner    (1001) docker     (123)     3238 2023-05-12 20:08:04.000000 podcast_downloader-0.5.1/podcast_downloader/rss.py
--rw-r--r--   0 runner    (1001) docker     (123)      893 2023-05-12 20:08:04.000000 podcast_downloader-0.5.1/podcast_downloader/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 20:08:14.695814 podcast_downloader-0.5.1/podcast_downloader.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     9787 2023-05-12 20:08:14.000000 podcast_downloader-0.5.1/podcast_downloader.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      453 2023-05-12 20:08:14.000000 podcast_downloader-0.5.1/podcast_downloader.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-12 20:08:14.000000 podcast_downloader-0.5.1/podcast_downloader.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       11 2023-05-12 20:08:14.000000 podcast_downloader-0.5.1/podcast_downloader.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       19 2023-05-12 20:08:14.000000 podcast_downloader-0.5.1/podcast_downloader.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-12 20:08:14.695814 podcast_downloader-0.5.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      883 2023-05-12 20:08:04.000000 podcast_downloader-0.5.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 16:49:31.198124 podcast_downloader-0.6.0/
+-rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-05-21 16:49:21.000000 podcast_downloader-0.6.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    11282 2023-05-21 16:49:31.198124 podcast_downloader-0.6.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    10695 2023-05-21 16:49:21.000000 podcast_downloader-0.6.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 16:49:31.194124 podcast_downloader-0.6.0/podcast_downloader/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-21 16:49:21.000000 podcast_downloader-0.6.0/podcast_downloader/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9103 2023-05-21 16:49:21.000000 podcast_downloader-0.6.0/podcast_downloader/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3279 2023-05-21 16:49:21.000000 podcast_downloader-0.6.0/podcast_downloader/configuration.py
+-rw-r--r--   0 runner    (1001) docker     (123)      968 2023-05-21 16:49:21.000000 podcast_downloader-0.6.0/podcast_downloader/downloaded.py
+-rw-r--r--   0 runner    (1001) docker     (123)      651 2023-05-21 16:49:21.000000 podcast_downloader-0.6.0/podcast_downloader/parameters.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3238 2023-05-21 16:49:21.000000 podcast_downloader-0.6.0/podcast_downloader/rss.py
+-rw-r--r--   0 runner    (1001) docker     (123)      893 2023-05-21 16:49:21.000000 podcast_downloader-0.6.0/podcast_downloader/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 16:49:31.198124 podcast_downloader-0.6.0/podcast_downloader.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    11282 2023-05-21 16:49:31.000000 podcast_downloader-0.6.0/podcast_downloader.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      453 2023-05-21 16:49:31.000000 podcast_downloader-0.6.0/podcast_downloader.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-21 16:49:31.000000 podcast_downloader-0.6.0/podcast_downloader.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       11 2023-05-21 16:49:31.000000 podcast_downloader-0.6.0/podcast_downloader.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       19 2023-05-21 16:49:31.000000 podcast_downloader-0.6.0/podcast_downloader.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-21 16:49:31.198124 podcast_downloader-0.6.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      883 2023-05-21 16:49:21.000000 podcast_downloader-0.6.0/setup.py
```

### Comparing `podcast_downloader-0.5.1/LICENSE` & `podcast_downloader-0.6.0/LICENSE`

 * *Files identical despite different names*

### Comparing `podcast_downloader-0.5.1/PKG-INFO` & `podcast_downloader-0.6.0/README.md`

 * *Files 12% similar despite different names*

```diff
@@ -1,23 +1,7 @@
-Metadata-Version: 2.1
-Name: podcast_downloader
-Version: 0.5.1
-Summary: The script for downloading the recent mp3 from given RSS channels
-Home-page: https://github.com/dplocki/podcast-downloader
-Author: Dawid Plocki
-Author-email: dawid.plocki@gmail.com
-Classifier: Environment :: Console
-Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
-Classifier: Natural Language :: English
-Classifier: Operating System :: OS Independent
-Classifier: Programming Language :: Python :: 3.7
-Requires-Python: >=3.6
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
 # Podcast Downloader
 
 ![GitHub](https://img.shields.io/github/license/dplocki/podcast-downloader)
 ![Build Status](https://img.shields.io/endpoint.svg?url=https%3A%2F%2Factions-badge.atrox.dev%2Fdplocki%2Fpodcast-downloader%2Fbadge%3Fref%3Dmaster&style=flat)
 ![PyPI](https://img.shields.io/pypi/v/podcast-downloader)
 
 The Python module for downloading files from given RSS feeds.
@@ -72,48 +56,85 @@
 
 ```
  command line parameters > configuration file > default values
 ```
 
 ### The main options
 
-| Property             | Type       | Required | Default                  | Note |
-|:---------------------|:----------:|:--------:|:------------------------:|:-----|
-| `downloads_limit`    | number     | no       | infinity                 |      |
-| `if_directory_empty` | string     | no       | download_last            | See [In case of empty directory](#in-case-of-empty-directory) |
-| `podcast_extensions` | key-value  | no       | `{".mp3": "audio/mpeg"}` | The file filter |
-| `podcasts`           | subsection | yes      | `[]`                     | See [Podcasts sub category](#podcasts-sub-category) |
+| Property             | Type       | Required | Default                                | Note |
+|:---------------------|:----------:|:--------:|:--------------------------------------:|:-----|
+| `downloads_limit`    | number     | no       | infinity                               |      |
+| `if_directory_empty` | string     | no       | download_last                          | See [In case of empty directory](#in-case-of-empty-directory) |
+| `podcast_extensions` | key-value  | no       | `{".mp3": "audio/mpeg"}`               | The file filter |
+| `podcasts`           | subsection | yes      | `[]`                                   | See [Podcasts sub category](#podcasts-sub-category) |
+| `http_headers`       | key-value  | no       | `{"User-Agent": "podcast-downloader"}` | See [HTTP request headers](#http-request-headers) |
 
 ### Podcasts sub category
 
 `Podcasts` is the part of configuration file where you provide the array of objects with fallowing content:
 
-| Property             | Type      | Required | Default                        | Note |
-|:---------------------|:---------:|:--------:|:------------------------------:|:-----|
-| `name`               | string    | yes      | -                              | The name of channel (used in logger) |
-| `rss_link`           | string    | yes      | -                              | The URL of RSS channel |
-| `path`               | string    | yes      | -                              | The path to directory, for podcast files |
-| `file_name_template` | string    | no       | `%file_name%.%file_extension%` | The template for the downloaded files, more 
-| `disable`            | boolean   | no       | `false`                        | This podcast will be ignored |
-| `podcast_extensions` | key-value | no       | `{".mp3": "audio/mpeg"}`       | The file filter |
-| `if_directory_empty` | string    | no       | `download_last`                | See [In case of empty directory](#in-case-of-empty-directory) |
-| `require_date`       | boolean   | no       | `false`                        | **Deprecated** Is date of podcast should be added into name of file - use the `file_name_template`: `[%publish_date%] %file_name%.%file_extension%"` |
+| Property             | Type       | Required | Default                                | Note |
+|:---------------------|:----------:|:--------:|:--------------------------------------:|:-----|
+| `name`               | string     | yes      | -                                      | The name of channel (used in logger) |
+| `rss_link`           | string     | yes      | -                                      | The URL of RSS channel |
+| `path`               | string     | yes      | -                                      | The path to directory, for podcast files |
+| `file_name_template` | string     | no       | `%file_name%.%file_extension%`         | The template for the downloaded files, more 
+| `disable`            | boolean    | no       | `false`                                | This podcast will be ignored |
+| `podcast_extensions` | key-value  | no       | `{".mp3": "audio/mpeg"}`               | The file filter |
+| `if_directory_empty` | string     | no       | `download_last`                        | See [In case of empty directory](#in-case-of-empty-directory) |
+| `require_date`       | boolean    | no       | `false`                                | **Deprecated** Is date of podcast should be added into name of file - use the `file_name_template`: `[%publish_date%] %file_name%.%file_extension%"` |
+| `http_headers`       | key-value  | no       | `{"User-Agent": "podcast-downloader"}` |      |
 
 ### An example of configuration file
 
 ```json
 {
-    "if_directory_empty": "download_from_4_days",
-    "podcasts": [
-        {
-            "name": "The Skeptic Guide",
-            "rss_link": "http://www.theskepticsguide.org/feed/rss.aspx",
-            "path": "~/podcasts/SGTTU"
-        }
-    ]
+  "if_directory_empty": "download_from_4_days",
+  "podcasts": [
+    {
+      "name": "Python for dummies",
+      "rss_link": "http://python-for-dummies/atom.rss",
+      "path": "~/podcasts/PythonForDummies"
+    },
+    {
+      "name": "The Skeptic Guide",
+      "rss_link": "https://feed.theskepticsguide.org/feed/rss.aspx",
+      "path": "~/podcasts/SGTTU"
+    }
+  ]
+}
+```
+
+### HTTP request headers
+
+There is an option to specify HTTP headers when downloading files.
+You can provide them using the `http_headers` value in the configuration file.
+The option value should be a dictionary where each header is presented as a key-value pair, with the key being the header title and the value being the header value.
+
+Default value: `{"User-Agent": "podcast-downloader"}`. Providing any value for `http_headers` will override the default value.
+
+Podcast `http_headers` will be merged with the global `http_headers`. In case of a conflict (same key name), the vale from podcast sub-configuration will override the global one.
+
+Example:
+
+```json
+{
+  "http_headers": {
+    "User-Agent": "podcast-downloader"
+  },
+  "podcasts": [
+    {
+      "name": "Unu Podcast",
+      "rss_link": "http://www.unupodcast.org/feed.rss",
+      "path": "~/podcasts/unu_podcast",
+      "https_headers": {
+        "User-Agent": "User-Agent: Mozilla/5.0",
+      }
+    }
+  ]
 }
 ```
 
 ## Script arguments
 
 The script accept following command line arguments:
 
@@ -153,18 +174,18 @@
 Podcasts are mostly stored as `*.mp3` files. By default Podcast Downloader will look just for them.
 
 If your podcast support other types of media files, you can precised your own podcast file filter, by providing extension for the file (like `.mp3`), and type of link in RSS feed itself (for `mp3` it is `audio/mpeg`).
 
 If you don't know the type of the file, you can check the RSS file. Seek for `enclosure` tags, should looks like this:
 
 ```xml
-    <enclosure
-        url="https://an.apple.supporter.page/podcast/episode23.m4a"
-        length="14527149"
-        type="audio/x-m4a" />
+  <enclosure
+    url="https://an.apple.supporter.page/podcast/episode23.m4a"
+    length="14527149"
+    type="audio/x-m4a" />
 ```
 
 Notes: the dot on the file extension is require.
 
 ### Example
 
 ```json
```

### Comparing `podcast_downloader-0.5.1/README.md` & `podcast_downloader-0.6.0/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,7 +1,23 @@
+Metadata-Version: 2.1
+Name: podcast_downloader
+Version: 0.6.0
+Summary: The script for downloading the recent mp3 from given RSS channels
+Home-page: https://github.com/dplocki/podcast-downloader
+Author: Dawid Plocki
+Author-email: dawid.plocki@gmail.com
+Classifier: Environment :: Console
+Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
+Classifier: Natural Language :: English
+Classifier: Operating System :: OS Independent
+Classifier: Programming Language :: Python :: 3.7
+Requires-Python: >=3.6
+Description-Content-Type: text/markdown
+License-File: LICENSE
+
 # Podcast Downloader
 
 ![GitHub](https://img.shields.io/github/license/dplocki/podcast-downloader)
 ![Build Status](https://img.shields.io/endpoint.svg?url=https%3A%2F%2Factions-badge.atrox.dev%2Fdplocki%2Fpodcast-downloader%2Fbadge%3Fref%3Dmaster&style=flat)
 ![PyPI](https://img.shields.io/pypi/v/podcast-downloader)
 
 The Python module for downloading files from given RSS feeds.
@@ -56,48 +72,85 @@
 
 ```
  command line parameters > configuration file > default values
 ```
 
 ### The main options
 
-| Property             | Type       | Required | Default                  | Note |
-|:---------------------|:----------:|:--------:|:------------------------:|:-----|
-| `downloads_limit`    | number     | no       | infinity                 |      |
-| `if_directory_empty` | string     | no       | download_last            | See [In case of empty directory](#in-case-of-empty-directory) |
-| `podcast_extensions` | key-value  | no       | `{".mp3": "audio/mpeg"}` | The file filter |
-| `podcasts`           | subsection | yes      | `[]`                     | See [Podcasts sub category](#podcasts-sub-category) |
+| Property             | Type       | Required | Default                                | Note |
+|:---------------------|:----------:|:--------:|:--------------------------------------:|:-----|
+| `downloads_limit`    | number     | no       | infinity                               |      |
+| `if_directory_empty` | string     | no       | download_last                          | See [In case of empty directory](#in-case-of-empty-directory) |
+| `podcast_extensions` | key-value  | no       | `{".mp3": "audio/mpeg"}`               | The file filter |
+| `podcasts`           | subsection | yes      | `[]`                                   | See [Podcasts sub category](#podcasts-sub-category) |
+| `http_headers`       | key-value  | no       | `{"User-Agent": "podcast-downloader"}` | See [HTTP request headers](#http-request-headers) |
 
 ### Podcasts sub category
 
 `Podcasts` is the part of configuration file where you provide the array of objects with fallowing content:
 
-| Property             | Type      | Required | Default                        | Note |
-|:---------------------|:---------:|:--------:|:------------------------------:|:-----|
-| `name`               | string    | yes      | -                              | The name of channel (used in logger) |
-| `rss_link`           | string    | yes      | -                              | The URL of RSS channel |
-| `path`               | string    | yes      | -                              | The path to directory, for podcast files |
-| `file_name_template` | string    | no       | `%file_name%.%file_extension%` | The template for the downloaded files, more 
-| `disable`            | boolean   | no       | `false`                        | This podcast will be ignored |
-| `podcast_extensions` | key-value | no       | `{".mp3": "audio/mpeg"}`       | The file filter |
-| `if_directory_empty` | string    | no       | `download_last`                | See [In case of empty directory](#in-case-of-empty-directory) |
-| `require_date`       | boolean   | no       | `false`                        | **Deprecated** Is date of podcast should be added into name of file - use the `file_name_template`: `[%publish_date%] %file_name%.%file_extension%"` |
+| Property             | Type       | Required | Default                                | Note |
+|:---------------------|:----------:|:--------:|:--------------------------------------:|:-----|
+| `name`               | string     | yes      | -                                      | The name of channel (used in logger) |
+| `rss_link`           | string     | yes      | -                                      | The URL of RSS channel |
+| `path`               | string     | yes      | -                                      | The path to directory, for podcast files |
+| `file_name_template` | string     | no       | `%file_name%.%file_extension%`         | The template for the downloaded files, more 
+| `disable`            | boolean    | no       | `false`                                | This podcast will be ignored |
+| `podcast_extensions` | key-value  | no       | `{".mp3": "audio/mpeg"}`               | The file filter |
+| `if_directory_empty` | string     | no       | `download_last`                        | See [In case of empty directory](#in-case-of-empty-directory) |
+| `require_date`       | boolean    | no       | `false`                                | **Deprecated** Is date of podcast should be added into name of file - use the `file_name_template`: `[%publish_date%] %file_name%.%file_extension%"` |
+| `http_headers`       | key-value  | no       | `{"User-Agent": "podcast-downloader"}` |      |
 
 ### An example of configuration file
 
 ```json
 {
-    "if_directory_empty": "download_from_4_days",
-    "podcasts": [
-        {
-            "name": "The Skeptic Guide",
-            "rss_link": "http://www.theskepticsguide.org/feed/rss.aspx",
-            "path": "~/podcasts/SGTTU"
-        }
-    ]
+  "if_directory_empty": "download_from_4_days",
+  "podcasts": [
+    {
+      "name": "Python for dummies",
+      "rss_link": "http://python-for-dummies/atom.rss",
+      "path": "~/podcasts/PythonForDummies"
+    },
+    {
+      "name": "The Skeptic Guide",
+      "rss_link": "https://feed.theskepticsguide.org/feed/rss.aspx",
+      "path": "~/podcasts/SGTTU"
+    }
+  ]
+}
+```
+
+### HTTP request headers
+
+There is an option to specify HTTP headers when downloading files.
+You can provide them using the `http_headers` value in the configuration file.
+The option value should be a dictionary where each header is presented as a key-value pair, with the key being the header title and the value being the header value.
+
+Default value: `{"User-Agent": "podcast-downloader"}`. Providing any value for `http_headers` will override the default value.
+
+Podcast `http_headers` will be merged with the global `http_headers`. In case of a conflict (same key name), the vale from podcast sub-configuration will override the global one.
+
+Example:
+
+```json
+{
+  "http_headers": {
+    "User-Agent": "podcast-downloader"
+  },
+  "podcasts": [
+    {
+      "name": "Unu Podcast",
+      "rss_link": "http://www.unupodcast.org/feed.rss",
+      "path": "~/podcasts/unu_podcast",
+      "https_headers": {
+        "User-Agent": "User-Agent: Mozilla/5.0",
+      }
+    }
+  ]
 }
 ```
 
 ## Script arguments
 
 The script accept following command line arguments:
 
@@ -137,18 +190,18 @@
 Podcasts are mostly stored as `*.mp3` files. By default Podcast Downloader will look just for them.
 
 If your podcast support other types of media files, you can precised your own podcast file filter, by providing extension for the file (like `.mp3`), and type of link in RSS feed itself (for `mp3` it is `audio/mpeg`).
 
 If you don't know the type of the file, you can check the RSS file. Seek for `enclosure` tags, should looks like this:
 
 ```xml
-    <enclosure
-        url="https://an.apple.supporter.page/podcast/episode23.m4a"
-        length="14527149"
-        type="audio/x-m4a" />
+  <enclosure
+    url="https://an.apple.supporter.page/podcast/episode23.m4a"
+    length="14527149"
+    type="audio/x-m4a" />
 ```
 
 Notes: the dot on the file extension is require.
 
 ### Example
 
 ```json
```

### Comparing `podcast_downloader-0.5.1/podcast_downloader/__main__.py` & `podcast_downloader-0.6.0/podcast_downloader/__main__.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 import os
-from typing import Callable, Dict, Iterable
+from typing import Callable, Dict, Iterable, List, Tuple
 import urllib
 import argparse
 import re
 import time
 import sys
 
 from functools import partial
@@ -28,20 +28,28 @@
     limit_file_name,
     only_last_entity,
     only_entities_from_date,
 )
 
 
 def download_rss_entity_to_path(
-    to_file_name_function: Callable[[RSSEntity], str], path: str, rss_entity: RSSEntity
+    headers: List[Tuple[str, str]],
+    to_file_name_function: Callable[[RSSEntity], str],
+    path: str,
+    rss_entity: RSSEntity,
 ):
     path_to_file = os.path.join(path, to_file_name_function(rss_entity))
 
     try:
-        return urllib.request.urlretrieve(rss_entity.link, path_to_file)
+        request = urllib.request.Request(rss_entity.link, headers=headers)
+
+        with urllib.request.urlopen(request) as response:
+            with open(path_to_file, "wb") as file:
+                file.write(response.read())
+
     except Exception as exception:
         log_error(
             'The podcast file "{}" could not be saved to disk "{}" due to the following error:\n{}',
             rss_entity.link,
             path_to_file,
             exception,
         )
@@ -129,14 +137,15 @@
     import sys
 
     DEFAULT_CONFIGURATION = {
         configuration.CONFIG_DOWNLOADS_LIMIT: sys.maxsize,
         configuration.CONFIG_IF_DIRECTORY_EMPTY: "download_last",
         configuration.CONFIG_PODCAST_EXTENSIONS: {".mp3": "audio/mpeg"},
         configuration.CONFIG_FILE_NAME_TEMPLATE: "%file_name%.%file_extension%",
+        configuration.CONFIG_HTTP_HEADER: {"User-Agent": "podcast-downloader"},
         configuration.CONFIG_PODCASTS: [],
     }
 
     CONFIG_FILE = "~/.podcast_downloader_config.json"
     log('Loading configuration (from file: "{}")', CONFIG_FILE)
 
     CONFIGURATION = merge_parameters_collection(
@@ -169,14 +178,18 @@
             configuration.CONFIG_IF_DIRECTORY_EMPTY,
             CONFIGURATION[configuration.CONFIG_IF_DIRECTORY_EMPTY],
         )
         rss_podcast_extensions = rss_source.get(
             configuration.CONFIG_PODCAST_EXTENSIONS,
             CONFIGURATION[configuration.CONFIG_PODCAST_EXTENSIONS],
         )
+        rss_https_header = merge_parameters_collection(
+            CONFIGURATION[configuration.CONFIG_HTTP_HEADER],
+            rss_source.get(configuration.CONFIG_HTTP_HEADER, {}),
+        )
 
         if rss_disable:
             log('Skipping the "{}"', rss_source_name)
             continue
 
         log('Checking "{}"', rss_source_name)
 
@@ -213,16 +226,19 @@
 
         if missing_files_links:
             to_real_podcast_file_name = compose(
                 partial(limit_file_name, file_length_limit), to_name_function
             )
 
             download_podcast = partial(
-                download_rss_entity_to_path, to_real_podcast_file_name
+                download_rss_entity_to_path,
+                rss_https_header,
+                to_real_podcast_file_name,
             )
+
             for rss_entry in reversed(missing_files_links):
                 wanted_podcast_file_name = to_name_function(rss_entry)
                 if wanted_podcast_file_name in downloaded_files:
                     continue
 
                 if DOWNLOADS_LIMITS == 0:
                     continue
```

### Comparing `podcast_downloader-0.5.1/podcast_downloader/configuration.py` & `podcast_downloader-0.6.0/podcast_downloader/configuration.py`

 * *Files 2% similar despite different names*

```diff
@@ -5,14 +5,15 @@
 
 SECONDS_IN_DAY = 24 * 60 * 60
 
 CONFIG_IF_DIRECTORY_EMPTY = "if_directory_empty"
 CONFIG_DOWNLOADS_LIMIT = "downloads_limit"
 CONFIG_FILE_NAME_TEMPLATE = "file_name_template"
 CONFIG_PODCAST_EXTENSIONS = "podcast_extensions"
+CONFIG_HTTP_HEADER = "http_headers"
 
 CONFIG_PODCASTS = "podcasts"
 CONFIG_PODCASTS_NAME = "name"
 CONFIG_PODCASTS_PATH = "path"
 CONFIG_PODCASTS_RSS_LINK = "rss_link"
 CONFIG_PODCASTS_REQUIRE_DATE = "require_date"
 CONFIG_PODCASTS_DISABLE = "disable"
```

### Comparing `podcast_downloader-0.5.1/podcast_downloader/downloaded.py` & `podcast_downloader-0.6.0/podcast_downloader/downloaded.py`

 * *Files identical despite different names*

### Comparing `podcast_downloader-0.5.1/podcast_downloader/parameters.py` & `podcast_downloader-0.6.0/podcast_downloader/parameters.py`

 * *Files identical despite different names*

### Comparing `podcast_downloader-0.5.1/podcast_downloader/rss.py` & `podcast_downloader-0.6.0/podcast_downloader/rss.py`

 * *Files identical despite different names*

### Comparing `podcast_downloader-0.5.1/podcast_downloader/utils.py` & `podcast_downloader-0.6.0/podcast_downloader/utils.py`

 * *Files identical despite different names*

### Comparing `podcast_downloader-0.5.1/podcast_downloader.egg-info/PKG-INFO` & `podcast_downloader-0.6.0/podcast_downloader.egg-info/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: podcast-downloader
-Version: 0.5.1
+Version: 0.6.0
 Summary: The script for downloading the recent mp3 from given RSS channels
 Home-page: https://github.com/dplocki/podcast-downloader
 Author: Dawid Plocki
 Author-email: dawid.plocki@gmail.com
 Classifier: Environment :: Console
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Natural Language :: English
@@ -72,48 +72,85 @@
 
 ```
  command line parameters > configuration file > default values
 ```
 
 ### The main options
 
-| Property             | Type       | Required | Default                  | Note |
-|:---------------------|:----------:|:--------:|:------------------------:|:-----|
-| `downloads_limit`    | number     | no       | infinity                 |      |
-| `if_directory_empty` | string     | no       | download_last            | See [In case of empty directory](#in-case-of-empty-directory) |
-| `podcast_extensions` | key-value  | no       | `{".mp3": "audio/mpeg"}` | The file filter |
-| `podcasts`           | subsection | yes      | `[]`                     | See [Podcasts sub category](#podcasts-sub-category) |
+| Property             | Type       | Required | Default                                | Note |
+|:---------------------|:----------:|:--------:|:--------------------------------------:|:-----|
+| `downloads_limit`    | number     | no       | infinity                               |      |
+| `if_directory_empty` | string     | no       | download_last                          | See [In case of empty directory](#in-case-of-empty-directory) |
+| `podcast_extensions` | key-value  | no       | `{".mp3": "audio/mpeg"}`               | The file filter |
+| `podcasts`           | subsection | yes      | `[]`                                   | See [Podcasts sub category](#podcasts-sub-category) |
+| `http_headers`       | key-value  | no       | `{"User-Agent": "podcast-downloader"}` | See [HTTP request headers](#http-request-headers) |
 
 ### Podcasts sub category
 
 `Podcasts` is the part of configuration file where you provide the array of objects with fallowing content:
 
-| Property             | Type      | Required | Default                        | Note |
-|:---------------------|:---------:|:--------:|:------------------------------:|:-----|
-| `name`               | string    | yes      | -                              | The name of channel (used in logger) |
-| `rss_link`           | string    | yes      | -                              | The URL of RSS channel |
-| `path`               | string    | yes      | -                              | The path to directory, for podcast files |
-| `file_name_template` | string    | no       | `%file_name%.%file_extension%` | The template for the downloaded files, more 
-| `disable`            | boolean   | no       | `false`                        | This podcast will be ignored |
-| `podcast_extensions` | key-value | no       | `{".mp3": "audio/mpeg"}`       | The file filter |
-| `if_directory_empty` | string    | no       | `download_last`                | See [In case of empty directory](#in-case-of-empty-directory) |
-| `require_date`       | boolean   | no       | `false`                        | **Deprecated** Is date of podcast should be added into name of file - use the `file_name_template`: `[%publish_date%] %file_name%.%file_extension%"` |
+| Property             | Type       | Required | Default                                | Note |
+|:---------------------|:----------:|:--------:|:--------------------------------------:|:-----|
+| `name`               | string     | yes      | -                                      | The name of channel (used in logger) |
+| `rss_link`           | string     | yes      | -                                      | The URL of RSS channel |
+| `path`               | string     | yes      | -                                      | The path to directory, for podcast files |
+| `file_name_template` | string     | no       | `%file_name%.%file_extension%`         | The template for the downloaded files, more 
+| `disable`            | boolean    | no       | `false`                                | This podcast will be ignored |
+| `podcast_extensions` | key-value  | no       | `{".mp3": "audio/mpeg"}`               | The file filter |
+| `if_directory_empty` | string     | no       | `download_last`                        | See [In case of empty directory](#in-case-of-empty-directory) |
+| `require_date`       | boolean    | no       | `false`                                | **Deprecated** Is date of podcast should be added into name of file - use the `file_name_template`: `[%publish_date%] %file_name%.%file_extension%"` |
+| `http_headers`       | key-value  | no       | `{"User-Agent": "podcast-downloader"}` |      |
 
 ### An example of configuration file
 
 ```json
 {
-    "if_directory_empty": "download_from_4_days",
-    "podcasts": [
-        {
-            "name": "The Skeptic Guide",
-            "rss_link": "http://www.theskepticsguide.org/feed/rss.aspx",
-            "path": "~/podcasts/SGTTU"
-        }
-    ]
+  "if_directory_empty": "download_from_4_days",
+  "podcasts": [
+    {
+      "name": "Python for dummies",
+      "rss_link": "http://python-for-dummies/atom.rss",
+      "path": "~/podcasts/PythonForDummies"
+    },
+    {
+      "name": "The Skeptic Guide",
+      "rss_link": "https://feed.theskepticsguide.org/feed/rss.aspx",
+      "path": "~/podcasts/SGTTU"
+    }
+  ]
+}
+```
+
+### HTTP request headers
+
+There is an option to specify HTTP headers when downloading files.
+You can provide them using the `http_headers` value in the configuration file.
+The option value should be a dictionary where each header is presented as a key-value pair, with the key being the header title and the value being the header value.
+
+Default value: `{"User-Agent": "podcast-downloader"}`. Providing any value for `http_headers` will override the default value.
+
+Podcast `http_headers` will be merged with the global `http_headers`. In case of a conflict (same key name), the vale from podcast sub-configuration will override the global one.
+
+Example:
+
+```json
+{
+  "http_headers": {
+    "User-Agent": "podcast-downloader"
+  },
+  "podcasts": [
+    {
+      "name": "Unu Podcast",
+      "rss_link": "http://www.unupodcast.org/feed.rss",
+      "path": "~/podcasts/unu_podcast",
+      "https_headers": {
+        "User-Agent": "User-Agent: Mozilla/5.0",
+      }
+    }
+  ]
 }
 ```
 
 ## Script arguments
 
 The script accept following command line arguments:
 
@@ -153,18 +190,18 @@
 Podcasts are mostly stored as `*.mp3` files. By default Podcast Downloader will look just for them.
 
 If your podcast support other types of media files, you can precised your own podcast file filter, by providing extension for the file (like `.mp3`), and type of link in RSS feed itself (for `mp3` it is `audio/mpeg`).
 
 If you don't know the type of the file, you can check the RSS file. Seek for `enclosure` tags, should looks like this:
 
 ```xml
-    <enclosure
-        url="https://an.apple.supporter.page/podcast/episode23.m4a"
-        length="14527149"
-        type="audio/x-m4a" />
+  <enclosure
+    url="https://an.apple.supporter.page/podcast/episode23.m4a"
+    length="14527149"
+    type="audio/x-m4a" />
 ```
 
 Notes: the dot on the file extension is require.
 
 ### Example
 
 ```json
```

### Comparing `podcast_downloader-0.5.1/setup.py` & `podcast_downloader-0.6.0/setup.py`

 * *Files identical despite different names*

