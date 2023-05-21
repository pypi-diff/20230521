# Comparing `tmp/duckduckgo_search-2.9.5.tar.gz` & `tmp/duckduckgo_search-3.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "duckduckgo_search-2.9.5.tar", last modified: Fri May 12 17:56:15 2023, max compression
+gzip compressed data, was "duckduckgo_search-3.0.2.tar", last modified: Wed May 17 21:50:09 2023, max compression
```

## Comparing `duckduckgo_search-2.9.5.tar` & `duckduckgo_search-3.0.2.tar`

### file list

```diff
@@ -1,38 +1,22 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 17:56:15.447162 duckduckgo_search-2.9.5/
--rwxr-xr-x   0 runner    (1001) docker     (123)     1063 2023-05-12 17:55:58.000000 duckduckgo_search-2.9.5/LICENSE.md
--rw-r--r--   0 runner    (1001) docker     (123)    35760 2023-05-12 17:56:15.447162 duckduckgo_search-2.9.5/PKG-INFO
--rwxr-xr-x   0 runner    (1001) docker     (123)    34645 2023-05-12 17:55:58.000000 duckduckgo_search-2.9.5/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 17:56:15.443162 duckduckgo_search-2.9.5/duckduckgo_search/
--rwxr-xr-x   0 runner    (1001) docker     (123)      671 2023-05-12 17:55:58.000000 duckduckgo_search-2.9.5/duckduckgo_search/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      145 2023-05-12 17:55:58.000000 duckduckgo_search-2.9.5/duckduckgo_search/__main__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 17:56:15.447162 duckduckgo_search-2.9.5/duckduckgo_search/cli/
--rwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 17:55:58.000000 duckduckgo_search-2.9.5/duckduckgo_search/cli/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    10405 2023-05-12 17:55:58.000000 duckduckgo_search-2.9.5/duckduckgo_search/cli/ddgs.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     6355 2023-05-12 17:55:58.000000 duckduckgo_search-2.9.5/duckduckgo_search/ddg.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     2872 2023-05-12 17:55:58.000000 duckduckgo_search-2.9.5/duckduckgo_search/ddg_answers.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     6565 2023-05-12 17:55:58.000000 duckduckgo_search-2.9.5/duckduckgo_search/ddg_images.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     7206 2023-05-12 17:55:58.000000 duckduckgo_search-2.9.5/duckduckgo_search/ddg_maps.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     3961 2023-05-12 17:55:58.000000 duckduckgo_search-2.9.5/duckduckgo_search/ddg_news.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1070 2023-05-12 17:55:58.000000 duckduckgo_search-2.9.5/duckduckgo_search/ddg_suggestions.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1643 2023-05-12 17:55:58.000000 duckduckgo_search-2.9.5/duckduckgo_search/ddg_translate.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     4084 2023-05-12 17:55:58.000000 duckduckgo_search-2.9.5/duckduckgo_search/ddg_videos.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     3950 2023-05-12 17:55:58.000000 duckduckgo_search-2.9.5/duckduckgo_search/utils.py
--rwxr-xr-x   0 runner    (1001) docker     (123)       22 2023-05-12 17:55:58.000000 duckduckgo_search-2.9.5/duckduckgo_search/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 17:56:15.447162 duckduckgo_search-2.9.5/duckduckgo_search.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    35760 2023-05-12 17:56:15.000000 duckduckgo_search-2.9.5/duckduckgo_search.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      915 2023-05-12 17:56:15.000000 duckduckgo_search-2.9.5/duckduckgo_search.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-12 17:56:15.000000 duckduckgo_search-2.9.5/duckduckgo_search.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       56 2023-05-12 17:56:15.000000 duckduckgo_search-2.9.5/duckduckgo_search.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       47 2023-05-12 17:56:15.000000 duckduckgo_search-2.9.5/duckduckgo_search.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       18 2023-05-12 17:56:15.000000 duckduckgo_search-2.9.5/duckduckgo_search.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1404 2023-05-12 17:55:58.000000 duckduckgo_search-2.9.5/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-12 17:56:15.447162 duckduckgo_search-2.9.5/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 17:56:15.447162 duckduckgo_search-2.9.5/tests/
--rwxr-xr-x   0 runner    (1001) docker     (123)     1619 2023-05-12 17:55:58.000000 duckduckgo_search-2.9.5/tests/test_ddg.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      994 2023-05-12 17:55:58.000000 duckduckgo_search-2.9.5/tests/test_ddg_answers.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     2510 2023-05-12 17:55:58.000000 duckduckgo_search-2.9.5/tests/test_ddg_images.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      418 2023-05-12 17:55:58.000000 duckduckgo_search-2.9.5/tests/test_ddg_maps.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1216 2023-05-12 17:55:58.000000 duckduckgo_search-2.9.5/tests/test_ddg_news.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      974 2023-05-12 17:55:58.000000 duckduckgo_search-2.9.5/tests/test_ddg_suggestions.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1128 2023-05-12 17:55:58.000000 duckduckgo_search-2.9.5/tests/test_ddg_translate.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1325 2023-05-12 17:55:58.000000 duckduckgo_search-2.9.5/tests/test_ddg_videos.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 21:50:09.893731 duckduckgo_search-3.0.2/
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1063 2023-05-17 21:49:51.000000 duckduckgo_search-3.0.2/LICENSE.md
+-rw-r--r--   0 runner    (1001) docker     (123)    14600 2023-05-17 21:50:09.893731 duckduckgo_search-3.0.2/PKG-INFO
+-rwxr-xr-x   0 runner    (1001) docker     (123)    13485 2023-05-17 21:49:51.000000 duckduckgo_search-3.0.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 21:50:09.889731 duckduckgo_search-3.0.2/duckduckgo_search/
+-rwxr-xr-x   0 runner    (1001) docker     (123)      607 2023-05-17 21:49:51.000000 duckduckgo_search-3.0.2/duckduckgo_search/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      138 2023-05-17 21:49:51.000000 duckduckgo_search-3.0.2/duckduckgo_search/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15809 2023-05-17 21:49:51.000000 duckduckgo_search-3.0.2/duckduckgo_search/cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6535 2023-05-17 21:49:51.000000 duckduckgo_search-3.0.2/duckduckgo_search/compat.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23675 2023-05-17 21:49:51.000000 duckduckgo_search-3.0.2/duckduckgo_search/duckduckgo_search.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)       22 2023-05-17 21:49:51.000000 duckduckgo_search-3.0.2/duckduckgo_search/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 21:50:09.893731 duckduckgo_search-3.0.2/duckduckgo_search.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    14600 2023-05-17 21:50:09.000000 duckduckgo_search-3.0.2/duckduckgo_search.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      496 2023-05-17 21:50:09.000000 duckduckgo_search-3.0.2/duckduckgo_search.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-17 21:50:09.000000 duckduckgo_search-3.0.2/duckduckgo_search.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       51 2023-05-17 21:50:09.000000 duckduckgo_search-3.0.2/duckduckgo_search.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       30 2023-05-17 21:50:09.000000 duckduckgo_search-3.0.2/duckduckgo_search.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       18 2023-05-17 21:50:09.000000 duckduckgo_search-3.0.2/duckduckgo_search.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1375 2023-05-17 21:49:51.000000 duckduckgo_search-3.0.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-17 21:50:09.893731 duckduckgo_search-3.0.2/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 21:50:09.893731 duckduckgo_search-3.0.2/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     4578 2023-05-17 21:49:51.000000 duckduckgo_search-3.0.2/tests/test_duckduckgo_search.py
```

### Comparing `duckduckgo_search-2.9.5/LICENSE.md` & `duckduckgo_search-3.0.2/LICENSE.md`

 * *Files identical despite different names*

### Comparing `duckduckgo_search-2.9.5/duckduckgo_search/utils.py` & `duckduckgo_search-3.0.2/tests/test_duckduckgo_search.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,131 +1,183 @@
-import csv
-import json
-import logging
 import os
-import re
-from datetime import datetime
-from html import unescape
-from shutil import copyfileobj
-from time import sleep
-
-import requests
-from diskcache import Cache
-
-logger = logging.getLogger(__name__)
-
-HEADERS = {
-    "User-Agent": "Mozilla/5.0 (Windows NT 10.0; rv:102.0) Gecko/20100101 Firefox/102.0",
-    "Referer": "https://duckduckgo.com/",
-}
-HEADERS_FILE_DOWNLOAD = {
-    "User-Agent": "Mozilla/5.0 (Windows NT 10.0; rv:102.0) Gecko/20100101 Firefox/102.0"
-}
-SESSION = requests.Session()
-SESSION.headers = HEADERS
-RE_STRIP_TAGS = re.compile("<.*?>")
-try:
-    VQD_CACHE = Cache(
-        f"{os.path.dirname(__file__)}/vqd_cache",
-        size_limit=104_857_600,
-        eviction_policy="least-frequently-used",
-    )
-except OSError:
-    VQD_CACHE = Cache(
-        "vqd_cache", size_limit=104_857_600, eviction_policy="least-frequently-used"
-    )
-
-
-def _get_vqd(keywords):
-    global SESSION
-
-    vqd_bytes = VQD_CACHE.get(keywords, None)
-    if vqd_bytes:
-        logger.debug("keywords=%s. Got vqd from cache", keywords)
-        return vqd_bytes.decode()
-
-    payload = {"q": keywords}
-    for _ in range(2):
-        try:
-            resp = SESSION.post("https://duckduckgo.com", data=payload, timeout=10)
-            resp.raise_for_status()
-            vqd_index_start = resp.content.index(b'vqd="') + 5
-            vqd_index_end = resp.content.index(b'"', vqd_index_start)
-            vqd_bytes = resp.content[vqd_index_start:vqd_index_end]
-
-            if vqd_bytes:
-                VQD_CACHE[keywords] = vqd_bytes
-                return vqd_bytes.decode()
-
-        except Exception as ex:
-            logger.info(f"_get_vqd() keywords={keywords} {type(ex).__name__} {ex}")
-
-        # refresh SESSION if not vqd
-        prev_proxies = SESSION.proxies
-        SESSION = requests.Session()
-        SESSION.headers = HEADERS
-        SESSION.proxies = prev_proxies
-        logger.warning("keywords=%s. _get_vqd() is None, refreshing SESSION", keywords)
-        VQD_CACHE.pop(keywords, None)
-        sleep(0.25)
-
-    # sleep to prevent blocking
-    sleep(0.25)
-
-
-def _refresh_vqd(keywords):
-    VQD_CACHE.pop(keywords, None)
-    vqd = _get_vqd(keywords)
-    logger.debug("keywords=%s. _refresh_vqd()", keywords)
-    return vqd
-
-
-def _save_json(jsonfile, data):
-    with open(jsonfile, "w") as file:
-        json.dump(data, file, ensure_ascii=False, indent=4)
-
-
-def _save_csv(csvfile, data):
-    with open(csvfile, "w", newline="", encoding="utf-8") as file:
-        if data:
-            headers = data[0].keys()
-            writer = csv.DictWriter(file, fieldnames=headers, quoting=csv.QUOTE_MINIMAL)
-            writer.writeheader()
-            writer.writerows(data)
-
-
-def _download_file(url, dir_path, filename):
-    try:
-        with requests.get(
-            url, headers=HEADERS_FILE_DOWNLOAD, stream=True, timeout=10
-        ) as resp:
-            resp.raise_for_status()
-            resp.raw.decode_content = True
-            with open(os.path.join(dir_path, filename), "wb") as file:
-                copyfileobj(resp.raw, file)
-            logger.info(f"File downloaded {url}")
-    except Exception as ex:
-        logger.debug(f"_download_file url={url} {type(ex).__name__} {ex}")
-
-
-def _normalize(raw_html):
-    """strip HTML tags"""
-    if raw_html:
-        return unescape(re.sub(RE_STRIP_TAGS, "", raw_html))
-
-
-def _do_output(module_name, keywords, output, results):
-    keywords = keywords.replace('"', "'")
-    if output == "csv":
-        _save_csv(
-            f"{module_name}_{keywords}_{datetime.now():%Y%m%d_%H%M%S}.csv", results
-        )
-    elif output == "json":
-        _save_json(
-            f"{module_name}_{keywords}_{datetime.now():%Y%m%d_%H%M%S}.json", results
-        )
-    """
-    elif output == "print":
-        for i, result in enumerate(results, start=1):
-            print(f"{i}.", json.dumps(result, ensure_ascii=False, indent=4))
-            input()
-    """
+import shutil
+
+from duckduckgo_search import DDGS
+from duckduckgo_search.cli import download_results, save_csv, save_json
+
+
+def test_text():
+    results_gen = DDGS().text("cat")
+    counter = 0
+    for i, x in enumerate(results_gen):
+        counter += 1
+        if i >= 25:
+            break
+    assert counter >= 25
+
+
+def test_images():
+    results_gen = DDGS().images("cat")
+    counter = 0
+    for i, x in enumerate(results_gen):
+        counter += 1
+        if i >= 150:
+            break
+    assert counter >= 150
+
+
+def test_videos():
+    results_gen = DDGS().videos("cat")
+    counter = 0
+    for i, x in enumerate(results_gen):
+        counter += 1
+        if i >= 40:
+            break
+    assert counter >= 40
+
+
+def test_news():
+    results_gen = DDGS().news("cat")
+    counter = 0
+    for i, x in enumerate(results_gen):
+        counter += 1
+        if i >= 40:
+            break
+    assert counter >= 40
+
+
+def test_maps():
+    results_gen = DDGS().maps("school", place="London")
+    counter = 0
+    for i, x in enumerate(results_gen):
+        counter += 1
+        if i >= 40:
+            break
+    assert counter >= 40
+
+
+def test_answers():
+    results_gen = DDGS().answers("cat")
+    counter = 0
+    for i, x in enumerate(results_gen):
+        counter += 1
+        if i >= 1:
+            break
+    assert counter >= 1
+
+
+def test_suggestions():
+    results_gen = DDGS().suggestions("cat")
+    counter = 0
+    for i, x in enumerate(results_gen):
+        counter += 1
+        if i >= 10:
+            break
+    assert counter >= 1
+
+
+def test_translate():
+    results = DDGS().translate("school", to="de")
+    assert results == {
+        "detected_language": "en",
+        "translated": "Schule",
+        "original": "school",
+    }
+
+
+def test_save_csv():
+    keywords = "butterfly"
+    results_gen = DDGS().text(keywords)
+    results = []
+    for r in results_gen:
+        results.append(r)
+        if len(results) >= 20:
+            break
+    assert len(results) >= 20
+
+    save_csv(f"{keywords}.csv", results)
+    save_json(f"{keywords}.json", results)
+
+    # delete files and folders contains keyword in name
+    not_files = True
+    for name in os.listdir():
+        if keywords in name:
+            if os.path.isfile(name):
+                os.remove(name)
+                not_files = False
+    if not_files:
+        raise AssertionError("csv not found")
+
+
+def test_save_json():
+    keywords = "chicago"
+    results_gen = DDGS().text(keywords)
+    results = []
+    for r in results_gen:
+        results.append(r)
+        if len(results) >= 20:
+            break
+    assert len(results) >= 20
+
+    save_json(f"{keywords}.json", results)
+
+    # delete files and folders contains keyword in name
+    not_files = True
+    for name in os.listdir():
+        if keywords in name:
+            if os.path.isfile(name):
+                os.remove(name)
+                not_files = False
+    if not_files:
+        raise AssertionError("json not found")
+
+
+def test_text_download():
+    keywords = "maradona"
+    results = [x for i, x in enumerate(DDGS().text(keywords)) if i <= 10]
+    assert len(results) >= 10
+
+    download_results(keywords, results)
+
+    # delete files contains keyword in name
+    files = False
+    for dir in os.listdir("."):
+        if keywords in dir:
+            for filename in os.listdir(dir):
+                filename = f"{os.getcwd()}/{dir}/{filename}"
+                if os.path.isfile(filename):
+                    os.remove(filename)
+                    files = True
+    if not files:
+        raise AssertionError("images files not found")
+
+    # delete folder contains keyword in name
+    for dir in os.listdir():
+        if f"{keywords}" in dir:
+            if os.path.isdir(dir):
+                shutil.rmtree(dir)
+
+
+def test_images_download():
+    keywords = "real madrid"
+    results = [x for i, x in enumerate(DDGS().images(keywords)) if i <= 10]
+    assert len(results) >= 10
+
+    download_results(keywords, results, images=True)
+
+    # delete files contains keyword in name
+    files = False
+    for dir in os.listdir("."):
+        if keywords in dir:
+            for filename in os.listdir(dir):
+                filename = f"{os.getcwd()}/{dir}/{filename}"
+                if os.path.isfile(filename):
+                    os.remove(filename)
+                    files = True
+    if not files:
+        raise AssertionError("images files not found")
+
+    # delete folder contains keyword in name
+    for dir in os.listdir():
+        if f"{keywords}" in dir:
+            if os.path.isdir(dir):
+                shutil.rmtree(dir)
```

### Comparing `duckduckgo_search-2.9.5/pyproject.toml` & `duckduckgo_search-3.0.2/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -25,20 +25,19 @@
     "Programming Language :: Python :: 3.11",
     "Programming Language :: Python :: Implementation :: CPython",
     "Topic :: Internet :: WWW/HTTP :: Indexing/Search",
     "Topic :: Software Development :: Libraries :: Python Modules",
 ]
 dependencies = [
     "click>=8.1.3",
-    "diskcache>=5.6.1",
-    "requests>=2.29.0",
+    "requests>=2.30.0",
 ]
 dynamic = ["version"]
 
 [project.urls]  # Optional
 "Homepage" = "https://github.com/deedy5/duckduckgo_search"
 
 [project.scripts]
-ddgs = "duckduckgo_search.cli.ddgs:cli"
+ddgs = "duckduckgo_search.cli:cli"
 
 [tool.setuptools.dynamic]
 version = {attr = "duckduckgo_search.version.__version__"}
```

