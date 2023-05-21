# Comparing `tmp/cyberdrop-dl-4.2.39.tar.gz` & `tmp/cyberdrop-dl-4.2.41.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cyberdrop-dl-4.2.39.tar", last modified: Sat May 20 05:00:23 2023, max compression
+gzip compressed data, was "cyberdrop-dl-4.2.41.tar", last modified: Sun May 21 17:04:00 2023, max compression
```

## Comparing `cyberdrop-dl-4.2.39.tar` & `cyberdrop-dl-4.2.41.tar`

### file list

```diff
@@ -1,62 +1,62 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 05:00:23.181701 cyberdrop-dl-4.2.39/
--rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-05-20 05:00:12.000000 cyberdrop-dl-4.2.39/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    18155 2023-05-20 05:00:23.181701 cyberdrop-dl-4.2.39/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    17720 2023-05-20 05:00:12.000000 cyberdrop-dl-4.2.39/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 05:00:23.169701 cyberdrop-dl-4.2.39/cyberdrop_dl/
--rw-r--r--   0 runner    (1001) docker     (123)       23 2023-05-20 05:00:12.000000 cyberdrop-dl-4.2.39/cyberdrop_dl/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 05:00:23.173701 cyberdrop-dl-4.2.39/cyberdrop_dl/base_functions/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-20 05:00:12.000000 cyberdrop-dl-4.2.39/cyberdrop_dl/base_functions/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6624 2023-05-20 05:00:12.000000 cyberdrop-dl-4.2.39/cyberdrop_dl/base_functions/base_functions.py
--rw-r--r--   0 runner    (1001) docker     (123)     3611 2023-05-20 05:00:12.000000 cyberdrop-dl-4.2.39/cyberdrop_dl/base_functions/config_manager.py
--rw-r--r--   0 runner    (1001) docker     (123)     3471 2023-05-20 05:00:12.000000 cyberdrop-dl-4.2.39/cyberdrop_dl/base_functions/config_schema.py
--rw-r--r--   0 runner    (1001) docker     (123)     8468 2023-05-20 05:00:12.000000 cyberdrop-dl-4.2.39/cyberdrop_dl/base_functions/data_classes.py
--rw-r--r--   0 runner    (1001) docker     (123)     1184 2023-05-20 05:00:12.000000 cyberdrop-dl-4.2.39/cyberdrop_dl/base_functions/error_classes.py
--rw-r--r--   0 runner    (1001) docker     (123)     3450 2023-05-20 05:00:12.000000 cyberdrop-dl-4.2.39/cyberdrop_dl/base_functions/sorting_functions.py
--rw-r--r--   0 runner    (1001) docker     (123)    12707 2023-05-20 05:00:12.000000 cyberdrop-dl-4.2.39/cyberdrop_dl/base_functions/sql_helper.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 05:00:23.173701 cyberdrop-dl-4.2.39/cyberdrop_dl/client/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-20 05:00:12.000000 cyberdrop-dl-4.2.39/cyberdrop_dl/client/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10099 2023-05-20 05:00:12.000000 cyberdrop-dl-4.2.39/cyberdrop_dl/client/client.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 05:00:23.177701 cyberdrop-dl-4.2.39/cyberdrop_dl/crawlers/
--rw-r--r--   0 runner    (1001) docker     (123)     2217 2023-05-20 05:00:12.000000 cyberdrop-dl-4.2.39/cyberdrop_dl/crawlers/Anonfiles_Spider.py
--rw-r--r--   0 runner    (1001) docker     (123)     7802 2023-05-20 05:00:12.000000 cyberdrop-dl-4.2.39/cyberdrop_dl/crawlers/Bunkr_Spider.py
--rw-r--r--   0 runner    (1001) docker     (123)     7922 2023-05-20 05:00:12.000000 cyberdrop-dl-4.2.39/cyberdrop_dl/crawlers/Coomeno_Spider.py
--rw-r--r--   0 runner    (1001) docker     (123)    12903 2023-05-20 05:00:12.000000 cyberdrop-dl-4.2.39/cyberdrop_dl/crawlers/CyberFile_Spider.py
--rw-r--r--   0 runner    (1001) docker     (123)     3042 2023-05-20 05:00:12.000000 cyberdrop-dl-4.2.39/cyberdrop_dl/crawlers/Cyberdrop_Spider.py
--rw-r--r--   0 runner    (1001) docker     (123)     3089 2023-05-20 05:00:12.000000 cyberdrop-dl-4.2.39/cyberdrop_dl/crawlers/EHentai_Spider.py
--rw-r--r--   0 runner    (1001) docker     (123)     4239 2023-05-20 05:00:12.000000 cyberdrop-dl-4.2.39/cyberdrop_dl/crawlers/Erome_Spider.py
--rw-r--r--   0 runner    (1001) docker     (123)     4206 2023-05-20 05:00:12.000000 cyberdrop-dl-4.2.39/cyberdrop_dl/crawlers/Fapello_Spider.py
--rw-r--r--   0 runner    (1001) docker     (123)     1890 2023-05-20 05:00:12.000000 cyberdrop-dl-4.2.39/cyberdrop_dl/crawlers/Gfycat_Spider.py
--rw-r--r--   0 runner    (1001) docker     (123)     5069 2023-05-20 05:00:12.000000 cyberdrop-dl-4.2.39/cyberdrop_dl/crawlers/GoFile_Spider.py
--rw-r--r--   0 runner    (1001) docker     (123)     2884 2023-05-20 05:00:12.000000 cyberdrop-dl-4.2.39/cyberdrop_dl/crawlers/HGameCG_Spider.py
--rw-r--r--   0 runner    (1001) docker     (123)     3140 2023-05-20 05:00:12.000000 cyberdrop-dl-4.2.39/cyberdrop_dl/crawlers/ImgBox_Spider.py
--rw-r--r--   0 runner    (1001) docker     (123)     3676 2023-05-20 05:00:12.000000 cyberdrop-dl-4.2.39/cyberdrop_dl/crawlers/LoveFap_Spider.py
--rw-r--r--   0 runner    (1001) docker     (123)     4389 2023-05-20 05:00:12.000000 cyberdrop-dl-4.2.39/cyberdrop_dl/crawlers/NSFWXXX_Spider.py
--rw-r--r--   0 runner    (1001) docker     (123)     2918 2023-05-20 05:00:12.000000 cyberdrop-dl-4.2.39/cyberdrop_dl/crawlers/PimpAndHost_Spider.py
--rw-r--r--   0 runner    (1001) docker     (123)     3362 2023-05-20 05:00:12.000000 cyberdrop-dl-4.2.39/cyberdrop_dl/crawlers/PixelDrain_Spider.py
--rw-r--r--   0 runner    (1001) docker     (123)     3008 2023-05-20 05:00:12.000000 cyberdrop-dl-4.2.39/cyberdrop_dl/crawlers/PostImg_Spider.py
--rw-r--r--   0 runner    (1001) docker     (123)     1499 2023-05-20 05:00:12.000000 cyberdrop-dl-4.2.39/cyberdrop_dl/crawlers/Saint_Spider.py
--rw-r--r--   0 runner    (1001) docker     (123)     9157 2023-05-20 05:00:12.000000 cyberdrop-dl-4.2.39/cyberdrop_dl/crawlers/ShareX_Spider.py
--rw-r--r--   0 runner    (1001) docker     (123)     2186 2023-05-20 05:00:12.000000 cyberdrop-dl-4.2.39/cyberdrop_dl/crawlers/XBunkr_Spider.py
--rw-r--r--   0 runner    (1001) docker     (123)    13919 2023-05-20 05:00:12.000000 cyberdrop-dl-4.2.39/cyberdrop_dl/crawlers/Xenforo_Spider.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-20 05:00:12.000000 cyberdrop-dl-4.2.39/cyberdrop_dl/crawlers/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 05:00:23.181701 cyberdrop-dl-4.2.39/cyberdrop_dl/downloader/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-20 05:00:12.000000 cyberdrop-dl-4.2.39/cyberdrop_dl/downloader/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2924 2023-05-20 05:00:12.000000 cyberdrop-dl-4.2.39/cyberdrop_dl/downloader/downloader_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    18477 2023-05-20 05:00:12.000000 cyberdrop-dl-4.2.39/cyberdrop_dl/downloader/downloaders.py
--rw-r--r--   0 runner    (1001) docker     (123)    12870 2023-05-20 05:00:12.000000 cyberdrop-dl-4.2.39/cyberdrop_dl/downloader/old_downloaders.py
--rw-r--r--   0 runner    (1001) docker     (123)    17463 2023-05-20 05:00:12.000000 cyberdrop-dl-4.2.39/cyberdrop_dl/downloader/progress_definitions.py
--rw-r--r--   0 runner    (1001) docker     (123)    20536 2023-05-20 05:00:12.000000 cyberdrop-dl-4.2.39/cyberdrop_dl/main.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 05:00:23.181701 cyberdrop-dl-4.2.39/cyberdrop_dl/scraper/
--rw-r--r--   0 runner    (1001) docker     (123)     2531 2023-05-20 05:00:12.000000 cyberdrop-dl-4.2.39/cyberdrop_dl/scraper/JDownloader_Integration.py
--rw-r--r--   0 runner    (1001) docker     (123)    20427 2023-05-20 05:00:12.000000 cyberdrop-dl-4.2.39/cyberdrop_dl/scraper/Scraper.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-20 05:00:12.000000 cyberdrop-dl-4.2.39/cyberdrop_dl/scraper/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 05:00:23.173701 cyberdrop-dl-4.2.39/cyberdrop_dl.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    18155 2023-05-20 05:00:23.000000 cyberdrop-dl-4.2.39/cyberdrop_dl.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1933 2023-05-20 05:00:23.000000 cyberdrop-dl-4.2.39/cyberdrop_dl.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-20 05:00:23.000000 cyberdrop-dl-4.2.39/cyberdrop_dl.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       56 2023-05-20 05:00:23.000000 cyberdrop-dl-4.2.39/cyberdrop_dl.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      176 2023-05-20 05:00:23.000000 cyberdrop-dl-4.2.39/cyberdrop_dl.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       13 2023-05-20 05:00:23.000000 cyberdrop-dl-4.2.39/cyberdrop_dl.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       90 2023-05-20 05:00:12.000000 cyberdrop-dl-4.2.39/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      860 2023-05-20 05:00:23.181701 cyberdrop-dl-4.2.39/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-20 05:00:12.000000 cyberdrop-dl-4.2.39/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 17:04:00.951463 cyberdrop-dl-4.2.41/
+-rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-05-21 17:03:46.000000 cyberdrop-dl-4.2.41/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    18155 2023-05-21 17:04:00.951463 cyberdrop-dl-4.2.41/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    17720 2023-05-21 17:03:46.000000 cyberdrop-dl-4.2.41/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 17:04:00.947463 cyberdrop-dl-4.2.41/cyberdrop_dl/
+-rw-r--r--   0 runner    (1001) docker     (123)       23 2023-05-21 17:03:46.000000 cyberdrop-dl-4.2.41/cyberdrop_dl/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 17:04:00.947463 cyberdrop-dl-4.2.41/cyberdrop_dl/base_functions/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-21 17:03:46.000000 cyberdrop-dl-4.2.41/cyberdrop_dl/base_functions/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6659 2023-05-21 17:03:46.000000 cyberdrop-dl-4.2.41/cyberdrop_dl/base_functions/base_functions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3033 2023-05-21 17:03:46.000000 cyberdrop-dl-4.2.41/cyberdrop_dl/base_functions/config_manager.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3471 2023-05-21 17:03:46.000000 cyberdrop-dl-4.2.41/cyberdrop_dl/base_functions/config_schema.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8468 2023-05-21 17:03:46.000000 cyberdrop-dl-4.2.41/cyberdrop_dl/base_functions/data_classes.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1184 2023-05-21 17:03:46.000000 cyberdrop-dl-4.2.41/cyberdrop_dl/base_functions/error_classes.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3450 2023-05-21 17:03:46.000000 cyberdrop-dl-4.2.41/cyberdrop_dl/base_functions/sorting_functions.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12707 2023-05-21 17:03:46.000000 cyberdrop-dl-4.2.41/cyberdrop_dl/base_functions/sql_helper.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 17:04:00.947463 cyberdrop-dl-4.2.41/cyberdrop_dl/client/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-21 17:03:46.000000 cyberdrop-dl-4.2.41/cyberdrop_dl/client/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10099 2023-05-21 17:03:46.000000 cyberdrop-dl-4.2.41/cyberdrop_dl/client/client.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 17:04:00.951463 cyberdrop-dl-4.2.41/cyberdrop_dl/crawlers/
+-rw-r--r--   0 runner    (1001) docker     (123)     2217 2023-05-21 17:03:46.000000 cyberdrop-dl-4.2.41/cyberdrop_dl/crawlers/Anonfiles_Spider.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7802 2023-05-21 17:03:46.000000 cyberdrop-dl-4.2.41/cyberdrop_dl/crawlers/Bunkr_Spider.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7922 2023-05-21 17:03:46.000000 cyberdrop-dl-4.2.41/cyberdrop_dl/crawlers/Coomeno_Spider.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12903 2023-05-21 17:03:46.000000 cyberdrop-dl-4.2.41/cyberdrop_dl/crawlers/CyberFile_Spider.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3042 2023-05-21 17:03:46.000000 cyberdrop-dl-4.2.41/cyberdrop_dl/crawlers/Cyberdrop_Spider.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3089 2023-05-21 17:03:46.000000 cyberdrop-dl-4.2.41/cyberdrop_dl/crawlers/EHentai_Spider.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4239 2023-05-21 17:03:46.000000 cyberdrop-dl-4.2.41/cyberdrop_dl/crawlers/Erome_Spider.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4206 2023-05-21 17:03:46.000000 cyberdrop-dl-4.2.41/cyberdrop_dl/crawlers/Fapello_Spider.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1890 2023-05-21 17:03:46.000000 cyberdrop-dl-4.2.41/cyberdrop_dl/crawlers/Gfycat_Spider.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5069 2023-05-21 17:03:46.000000 cyberdrop-dl-4.2.41/cyberdrop_dl/crawlers/GoFile_Spider.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2884 2023-05-21 17:03:46.000000 cyberdrop-dl-4.2.41/cyberdrop_dl/crawlers/HGameCG_Spider.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3140 2023-05-21 17:03:46.000000 cyberdrop-dl-4.2.41/cyberdrop_dl/crawlers/ImgBox_Spider.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3676 2023-05-21 17:03:46.000000 cyberdrop-dl-4.2.41/cyberdrop_dl/crawlers/LoveFap_Spider.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4389 2023-05-21 17:03:46.000000 cyberdrop-dl-4.2.41/cyberdrop_dl/crawlers/NSFWXXX_Spider.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2918 2023-05-21 17:03:46.000000 cyberdrop-dl-4.2.41/cyberdrop_dl/crawlers/PimpAndHost_Spider.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3362 2023-05-21 17:03:46.000000 cyberdrop-dl-4.2.41/cyberdrop_dl/crawlers/PixelDrain_Spider.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3008 2023-05-21 17:03:46.000000 cyberdrop-dl-4.2.41/cyberdrop_dl/crawlers/PostImg_Spider.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1499 2023-05-21 17:03:46.000000 cyberdrop-dl-4.2.41/cyberdrop_dl/crawlers/Saint_Spider.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9157 2023-05-21 17:03:46.000000 cyberdrop-dl-4.2.41/cyberdrop_dl/crawlers/ShareX_Spider.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2186 2023-05-21 17:03:46.000000 cyberdrop-dl-4.2.41/cyberdrop_dl/crawlers/XBunkr_Spider.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13919 2023-05-21 17:03:46.000000 cyberdrop-dl-4.2.41/cyberdrop_dl/crawlers/Xenforo_Spider.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-21 17:03:46.000000 cyberdrop-dl-4.2.41/cyberdrop_dl/crawlers/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 17:04:00.951463 cyberdrop-dl-4.2.41/cyberdrop_dl/downloader/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-21 17:03:46.000000 cyberdrop-dl-4.2.41/cyberdrop_dl/downloader/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2924 2023-05-21 17:03:46.000000 cyberdrop-dl-4.2.41/cyberdrop_dl/downloader/downloader_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18477 2023-05-21 17:03:46.000000 cyberdrop-dl-4.2.41/cyberdrop_dl/downloader/downloaders.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12870 2023-05-21 17:03:46.000000 cyberdrop-dl-4.2.41/cyberdrop_dl/downloader/old_downloaders.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17463 2023-05-21 17:03:46.000000 cyberdrop-dl-4.2.41/cyberdrop_dl/downloader/progress_definitions.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20536 2023-05-21 17:03:46.000000 cyberdrop-dl-4.2.41/cyberdrop_dl/main.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 17:04:00.951463 cyberdrop-dl-4.2.41/cyberdrop_dl/scraper/
+-rw-r--r--   0 runner    (1001) docker     (123)     2531 2023-05-21 17:03:46.000000 cyberdrop-dl-4.2.41/cyberdrop_dl/scraper/JDownloader_Integration.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20427 2023-05-21 17:03:46.000000 cyberdrop-dl-4.2.41/cyberdrop_dl/scraper/Scraper.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-21 17:03:46.000000 cyberdrop-dl-4.2.41/cyberdrop_dl/scraper/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 17:04:00.947463 cyberdrop-dl-4.2.41/cyberdrop_dl.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    18155 2023-05-21 17:04:00.000000 cyberdrop-dl-4.2.41/cyberdrop_dl.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1933 2023-05-21 17:04:00.000000 cyberdrop-dl-4.2.41/cyberdrop_dl.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-21 17:04:00.000000 cyberdrop-dl-4.2.41/cyberdrop_dl.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       56 2023-05-21 17:04:00.000000 cyberdrop-dl-4.2.41/cyberdrop_dl.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      176 2023-05-21 17:04:00.000000 cyberdrop-dl-4.2.41/cyberdrop_dl.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       13 2023-05-21 17:04:00.000000 cyberdrop-dl-4.2.41/cyberdrop_dl.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       90 2023-05-21 17:03:46.000000 cyberdrop-dl-4.2.41/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      860 2023-05-21 17:04:00.951463 cyberdrop-dl-4.2.41/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-21 17:03:46.000000 cyberdrop-dl-4.2.41/setup.py
```

### Comparing `cyberdrop-dl-4.2.39/LICENSE` & `cyberdrop-dl-4.2.41/LICENSE`

 * *Files identical despite different names*

### Comparing `cyberdrop-dl-4.2.39/PKG-INFO` & `cyberdrop-dl-4.2.41/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cyberdrop-dl
-Version: 4.2.39
+Version: 4.2.41
 Summary: Bulk downloader for multiple file hosts and forum sites
 Home-page: https://github.com/Jules-WinnfieldX/CyberDropDownloader
 Author: Jules-WinnfieldX
 Author-email: JulesWinnfieldII@protonmail.com
 Project-URL: Bug Tracker, https://github.com/Jules-WinnfieldX/CyberDropDownloader/issues
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: cyberdrop-dl Version: 4.2.39 Summary: Bulk
+Metadata-Version: 2.1 Name: cyberdrop-dl Version: 4.2.41 Summary: Bulk
 downloader for multiple file hosts and forum sites Home-page: https://
 github.com/Jules-WinnfieldX/CyberDropDownloader Author: Jules-WinnfieldX
 Author-email: JulesWinnfieldII@protonmail.com Project-URL: Bug Tracker, https:/
 /github.com/Jules-WinnfieldX/CyberDropDownloader/issues Requires-Python: >=3.7
 Description-Content-Type: text/markdown License-File: LICENSE # `cyberdrop-dl`
 **Bulk downloader for multiple file hosts** [![PyPI version](https://
 badge.fury.io/py/cyberdrop-dl.svg)](https://badge.fury.io/py/cyberdrop-dl) [!
```

### Comparing `cyberdrop-dl-4.2.39/README.md` & `cyberdrop-dl-4.2.41/README.md`

 * *Files identical despite different names*

### Comparing `cyberdrop-dl-4.2.39/cyberdrop_dl/base_functions/base_functions.py` & `cyberdrop-dl-4.2.41/cyberdrop_dl/base_functions/base_functions.py`

 * *Files 1% similar despite different names*

```diff
@@ -159,29 +159,29 @@
         """Writes to the error file"""
         if not self.output_errored:
             return
 
         async with aiofiles.open(self.errored_downloads, 'a') as f:
             await f.write("URL,REFERER,REASON\n")
 
-    async def write_unsupported(self, text: str) -> None:
+    async def write_unsupported(self, url: URL, referer: URL, title: str) -> None:
         """Writes to the error file"""
         if not self.output_unsupported:
             return
 
         async with aiofiles.open(self.unsupported, 'a') as f:
-            await f.write("URL,REFERER,REASON\n")
+            await f.write(f"{url},{referer},{title}\n")
 
     async def write_unsupported_header(self):
         """Writes to the error file"""
         if not self.output_unsupported:
             return
 
         async with aiofiles.open(self.unsupported, 'a') as f:
-            await f.write(f"URL,Exception\n")
+            await f.write(f"URL,REFERER,TITLE\n")
 
     async def write_last_post(self, url: URL) -> None:
         """Writes to the error file"""
         if not self.output_last_post:
             return
 
         async with aiofiles.open(self.last_post, 'a') as f:
```

### Comparing `cyberdrop-dl-4.2.39/cyberdrop_dl/base_functions/config_manager.py` & `cyberdrop-dl-4.2.41/cyberdrop_dl/base_functions/config_manager.py`

 * *Files 16% similar despite different names*

```diff
@@ -74,22 +74,14 @@
     return config_data
 
 
 async def document_args(args: Dict) -> None:
     """We document the runtime arguments for debugging and troubleshooting, redacting sensitive information"""
     print_args = copy.deepcopy(args)
 
-    for group in print_args.values():
+    log("Starting Cyberdrop-DL")
+    for group_name, group in print_args.items():
+        args_type = group_name.replace('_', ' ').lower()
         for arg in group:
             if group[arg] is not None and any(s in arg for s in ('api_key', 'password')):
                 group[arg] = '!REDACTED!'
-
-    log("Starting Cyberdrop-DL")
-    log(f"Using authentication arguments: {print_args['Authentication']}", quiet=True)
-    log(f"Using file arguments: {print_args['Files']}", quiet=True)
-    log(f"Using forum option arguments: {print_args['Forum_Options']}", quiet=True)
-    log(f"Using ignore arguments: {print_args['Ignore']}", quiet=True)
-    log(f"Using jdownloader arguments: {print_args['JDownloader']}", quiet=True)
-    log(f"Using progress option arguments: {print_args['Progress_Options']}", quiet=True)
-    log(f"Using ratelimiting arguments: {print_args['Ratelimiting']}", quiet=True)
-    log(f"Using runtime arguments: {print_args['Runtime']}", quiet=True)
-    log(f"Using sorting arguments: {print_args['Sorting']}", quiet=True)
+        log(f"Using {args_type} arguments: {group}", quiet=True)
```

### Comparing `cyberdrop-dl-4.2.39/cyberdrop_dl/base_functions/config_schema.py` & `cyberdrop-dl-4.2.41/cyberdrop_dl/base_functions/config_schema.py`

 * *Files identical despite different names*

### Comparing `cyberdrop-dl-4.2.39/cyberdrop_dl/base_functions/data_classes.py` & `cyberdrop-dl-4.2.41/cyberdrop_dl/base_functions/data_classes.py`

 * *Files identical despite different names*

### Comparing `cyberdrop-dl-4.2.39/cyberdrop_dl/base_functions/error_classes.py` & `cyberdrop-dl-4.2.41/cyberdrop_dl/base_functions/error_classes.py`

 * *Files identical despite different names*

### Comparing `cyberdrop-dl-4.2.39/cyberdrop_dl/base_functions/sorting_functions.py` & `cyberdrop-dl-4.2.41/cyberdrop_dl/base_functions/sorting_functions.py`

 * *Files identical despite different names*

### Comparing `cyberdrop-dl-4.2.39/cyberdrop_dl/base_functions/sql_helper.py` & `cyberdrop-dl-4.2.41/cyberdrop_dl/base_functions/sql_helper.py`

 * *Files identical despite different names*

### Comparing `cyberdrop-dl-4.2.39/cyberdrop_dl/client/client.py` & `cyberdrop-dl-4.2.41/cyberdrop_dl/client/client.py`

 * *Files identical despite different names*

### Comparing `cyberdrop-dl-4.2.39/cyberdrop_dl/crawlers/Anonfiles_Spider.py` & `cyberdrop-dl-4.2.41/cyberdrop_dl/crawlers/Anonfiles_Spider.py`

 * *Files identical despite different names*

### Comparing `cyberdrop-dl-4.2.39/cyberdrop_dl/crawlers/Bunkr_Spider.py` & `cyberdrop-dl-4.2.41/cyberdrop_dl/crawlers/Bunkr_Spider.py`

 * *Files identical despite different names*

### Comparing `cyberdrop-dl-4.2.39/cyberdrop_dl/crawlers/Coomeno_Spider.py` & `cyberdrop-dl-4.2.41/cyberdrop_dl/crawlers/Coomeno_Spider.py`

 * *Files identical despite different names*

### Comparing `cyberdrop-dl-4.2.39/cyberdrop_dl/crawlers/CyberFile_Spider.py` & `cyberdrop-dl-4.2.41/cyberdrop_dl/crawlers/CyberFile_Spider.py`

 * *Files identical despite different names*

### Comparing `cyberdrop-dl-4.2.39/cyberdrop_dl/crawlers/Cyberdrop_Spider.py` & `cyberdrop-dl-4.2.41/cyberdrop_dl/crawlers/Cyberdrop_Spider.py`

 * *Files identical despite different names*

### Comparing `cyberdrop-dl-4.2.39/cyberdrop_dl/crawlers/EHentai_Spider.py` & `cyberdrop-dl-4.2.41/cyberdrop_dl/crawlers/EHentai_Spider.py`

 * *Files identical despite different names*

### Comparing `cyberdrop-dl-4.2.39/cyberdrop_dl/crawlers/Erome_Spider.py` & `cyberdrop-dl-4.2.41/cyberdrop_dl/crawlers/Erome_Spider.py`

 * *Files identical despite different names*

### Comparing `cyberdrop-dl-4.2.39/cyberdrop_dl/crawlers/Fapello_Spider.py` & `cyberdrop-dl-4.2.41/cyberdrop_dl/crawlers/Fapello_Spider.py`

 * *Files identical despite different names*

### Comparing `cyberdrop-dl-4.2.39/cyberdrop_dl/crawlers/Gfycat_Spider.py` & `cyberdrop-dl-4.2.41/cyberdrop_dl/crawlers/Gfycat_Spider.py`

 * *Files identical despite different names*

### Comparing `cyberdrop-dl-4.2.39/cyberdrop_dl/crawlers/GoFile_Spider.py` & `cyberdrop-dl-4.2.41/cyberdrop_dl/crawlers/GoFile_Spider.py`

 * *Files identical despite different names*

### Comparing `cyberdrop-dl-4.2.39/cyberdrop_dl/crawlers/HGameCG_Spider.py` & `cyberdrop-dl-4.2.41/cyberdrop_dl/crawlers/HGameCG_Spider.py`

 * *Files identical despite different names*

### Comparing `cyberdrop-dl-4.2.39/cyberdrop_dl/crawlers/ImgBox_Spider.py` & `cyberdrop-dl-4.2.41/cyberdrop_dl/crawlers/ImgBox_Spider.py`

 * *Files identical despite different names*

### Comparing `cyberdrop-dl-4.2.39/cyberdrop_dl/crawlers/LoveFap_Spider.py` & `cyberdrop-dl-4.2.41/cyberdrop_dl/crawlers/LoveFap_Spider.py`

 * *Files identical despite different names*

### Comparing `cyberdrop-dl-4.2.39/cyberdrop_dl/crawlers/NSFWXXX_Spider.py` & `cyberdrop-dl-4.2.41/cyberdrop_dl/crawlers/NSFWXXX_Spider.py`

 * *Files identical despite different names*

### Comparing `cyberdrop-dl-4.2.39/cyberdrop_dl/crawlers/PimpAndHost_Spider.py` & `cyberdrop-dl-4.2.41/cyberdrop_dl/crawlers/PimpAndHost_Spider.py`

 * *Files identical despite different names*

### Comparing `cyberdrop-dl-4.2.39/cyberdrop_dl/crawlers/PixelDrain_Spider.py` & `cyberdrop-dl-4.2.41/cyberdrop_dl/crawlers/PixelDrain_Spider.py`

 * *Files identical despite different names*

### Comparing `cyberdrop-dl-4.2.39/cyberdrop_dl/crawlers/PostImg_Spider.py` & `cyberdrop-dl-4.2.41/cyberdrop_dl/crawlers/PostImg_Spider.py`

 * *Files identical despite different names*

### Comparing `cyberdrop-dl-4.2.39/cyberdrop_dl/crawlers/Saint_Spider.py` & `cyberdrop-dl-4.2.41/cyberdrop_dl/crawlers/Saint_Spider.py`

 * *Files identical despite different names*

### Comparing `cyberdrop-dl-4.2.39/cyberdrop_dl/crawlers/ShareX_Spider.py` & `cyberdrop-dl-4.2.41/cyberdrop_dl/crawlers/ShareX_Spider.py`

 * *Files identical despite different names*

### Comparing `cyberdrop-dl-4.2.39/cyberdrop_dl/crawlers/XBunkr_Spider.py` & `cyberdrop-dl-4.2.41/cyberdrop_dl/crawlers/XBunkr_Spider.py`

 * *Files identical despite different names*

### Comparing `cyberdrop-dl-4.2.39/cyberdrop_dl/crawlers/Xenforo_Spider.py` & `cyberdrop-dl-4.2.41/cyberdrop_dl/crawlers/Xenforo_Spider.py`

 * *Files identical despite different names*

### Comparing `cyberdrop-dl-4.2.39/cyberdrop_dl/downloader/downloader_utils.py` & `cyberdrop-dl-4.2.41/cyberdrop_dl/downloader/downloader_utils.py`

 * *Files identical despite different names*

### Comparing `cyberdrop-dl-4.2.39/cyberdrop_dl/downloader/downloaders.py` & `cyberdrop-dl-4.2.41/cyberdrop_dl/downloader/downloaders.py`

 * *Files identical despite different names*

### Comparing `cyberdrop-dl-4.2.39/cyberdrop_dl/downloader/old_downloaders.py` & `cyberdrop-dl-4.2.41/cyberdrop_dl/downloader/old_downloaders.py`

 * *Files identical despite different names*

### Comparing `cyberdrop-dl-4.2.39/cyberdrop_dl/downloader/progress_definitions.py` & `cyberdrop-dl-4.2.41/cyberdrop_dl/downloader/progress_definitions.py`

 * *Files identical despite different names*

### Comparing `cyberdrop-dl-4.2.39/cyberdrop_dl/main.py` & `cyberdrop-dl-4.2.41/cyberdrop_dl/main.py`

 * *Files identical despite different names*

### Comparing `cyberdrop-dl-4.2.39/cyberdrop_dl/scraper/JDownloader_Integration.py` & `cyberdrop-dl-4.2.41/cyberdrop_dl/scraper/JDownloader_Integration.py`

 * *Files identical despite different names*

### Comparing `cyberdrop-dl-4.2.39/cyberdrop_dl/scraper/Scraper.py` & `cyberdrop-dl-4.2.41/cyberdrop_dl/scraper/Scraper.py`

 * *Files identical despite different names*

### Comparing `cyberdrop-dl-4.2.39/cyberdrop_dl.egg-info/PKG-INFO` & `cyberdrop-dl-4.2.41/cyberdrop_dl.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cyberdrop-dl
-Version: 4.2.39
+Version: 4.2.41
 Summary: Bulk downloader for multiple file hosts and forum sites
 Home-page: https://github.com/Jules-WinnfieldX/CyberDropDownloader
 Author: Jules-WinnfieldX
 Author-email: JulesWinnfieldII@protonmail.com
 Project-URL: Bug Tracker, https://github.com/Jules-WinnfieldX/CyberDropDownloader/issues
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: cyberdrop-dl Version: 4.2.39 Summary: Bulk
+Metadata-Version: 2.1 Name: cyberdrop-dl Version: 4.2.41 Summary: Bulk
 downloader for multiple file hosts and forum sites Home-page: https://
 github.com/Jules-WinnfieldX/CyberDropDownloader Author: Jules-WinnfieldX
 Author-email: JulesWinnfieldII@protonmail.com Project-URL: Bug Tracker, https:/
 /github.com/Jules-WinnfieldX/CyberDropDownloader/issues Requires-Python: >=3.7
 Description-Content-Type: text/markdown License-File: LICENSE # `cyberdrop-dl`
 **Bulk downloader for multiple file hosts** [![PyPI version](https://
 badge.fury.io/py/cyberdrop-dl.svg)](https://badge.fury.io/py/cyberdrop-dl) [!
```

### Comparing `cyberdrop-dl-4.2.39/cyberdrop_dl.egg-info/SOURCES.txt` & `cyberdrop-dl-4.2.41/cyberdrop_dl.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `cyberdrop-dl-4.2.39/setup.cfg` & `cyberdrop-dl-4.2.41/setup.cfg`

 * *Files identical despite different names*

