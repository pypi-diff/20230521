# Comparing `tmp/CobWeb-lnx-1.0.1.tar.gz` & `tmp/CobWeb-lnx-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "CobWeb-lnx-1.0.1.tar", last modified: Fri Apr 28 13:59:20 2023, max compression
+gzip compressed data, was "CobWeb-lnx-1.1.0.tar", last modified: Sun May 21 12:17:24 2023, max compression
```

## Comparing `CobWeb-lnx-1.0.1.tar` & `CobWeb-lnx-1.1.0.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxrwx   0        0        0        0 2023-04-28 13:59:20.856341 CobWeb-lnx-1.0.1/
--rw-rw-rw-   0        0        0     1094 2022-12-08 18:47:01.000000 CobWeb-lnx-1.0.1/LICENSE.md
--rw-rw-rw-   0        0        0     3856 2023-04-28 13:59:20.856341 CobWeb-lnx-1.0.1/PKG-INFO
--rw-rw-rw-   0        0        0     3098 2023-04-26 17:40:51.000000 CobWeb-lnx-1.0.1/README.md
--rw-rw-rw-   0        0        0      770 2023-04-28 13:56:49.000000 CobWeb-lnx-1.0.1/pyproject.toml
--rw-rw-rw-   0        0        0      480 2023-04-28 13:59:20.859342 CobWeb-lnx-1.0.1/setup.cfg
-drwxrwxrwx   0        0        0        0 2023-04-28 13:59:20.801546 CobWeb-lnx-1.0.1/src/
-drwxrwxrwx   0        0        0        0 2023-04-28 13:59:20.815857 CobWeb-lnx-1.0.1/src/CobWeb/
--rw-rw-rw-   0        0        0       51 2023-04-26 18:02:34.000000 CobWeb-lnx-1.0.1/src/CobWeb/__init__.py
--rw-rw-rw-   0        0        0    11299 2023-04-28 13:50:41.000000 CobWeb-lnx-1.0.1/src/CobWeb/crawler.py
-drwxrwxrwx   0        0        0        0 2023-04-28 13:59:20.854343 CobWeb-lnx-1.0.1/src/CobWeb_lnx.egg-info/
--rw-rw-rw-   0        0        0     3856 2023-04-28 13:59:20.000000 CobWeb-lnx-1.0.1/src/CobWeb_lnx.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      279 2023-04-28 13:59:20.000000 CobWeb-lnx-1.0.1/src/CobWeb_lnx.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-28 13:59:20.000000 CobWeb-lnx-1.0.1/src/CobWeb_lnx.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      362 2023-04-28 13:59:20.000000 CobWeb-lnx-1.0.1/src/CobWeb_lnx.egg-info/requires.txt
--rw-rw-rw-   0        0        0        7 2023-04-28 13:59:20.000000 CobWeb-lnx-1.0.1/src/CobWeb_lnx.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-05-21 12:17:24.573250 CobWeb-lnx-1.1.0/
+-rw-rw-rw-   0        0        0     1094 2022-12-08 18:47:01.000000 CobWeb-lnx-1.1.0/LICENSE.md
+-rw-rw-rw-   0        0        0     3549 2023-05-21 12:17:24.574252 CobWeb-lnx-1.1.0/PKG-INFO
+-rw-rw-rw-   0        0        0     2791 2023-05-21 12:09:05.000000 CobWeb-lnx-1.1.0/README.md
+-rw-rw-rw-   0        0        0      770 2023-05-21 12:09:19.000000 CobWeb-lnx-1.1.0/pyproject.toml
+-rw-rw-rw-   0        0        0      480 2023-05-21 12:17:24.588261 CobWeb-lnx-1.1.0/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-05-21 12:17:24.480178 CobWeb-lnx-1.1.0/src/
+drwxrwxrwx   0        0        0        0 2023-05-21 12:17:24.509184 CobWeb-lnx-1.1.0/src/CobWeb/
+-rw-rw-rw-   0        0        0       51 2023-04-26 18:02:34.000000 CobWeb-lnx-1.1.0/src/CobWeb/__init__.py
+-rw-rw-rw-   0        0        0    11785 2023-05-21 12:08:52.000000 CobWeb-lnx-1.1.0/src/CobWeb/crawler.py
+drwxrwxrwx   0        0        0        0 2023-05-21 12:17:24.569253 CobWeb-lnx-1.1.0/src/CobWeb_lnx.egg-info/
+-rw-rw-rw-   0        0        0     3549 2023-05-21 12:17:24.000000 CobWeb-lnx-1.1.0/src/CobWeb_lnx.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      279 2023-05-21 12:17:24.000000 CobWeb-lnx-1.1.0/src/CobWeb_lnx.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-21 12:17:24.000000 CobWeb-lnx-1.1.0/src/CobWeb_lnx.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      362 2023-05-21 12:17:24.000000 CobWeb-lnx-1.1.0/src/CobWeb_lnx.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        7 2023-05-21 12:17:24.000000 CobWeb-lnx-1.1.0/src/CobWeb_lnx.egg-info/top_level.txt
```

### Comparing `CobWeb-lnx-1.0.1/LICENSE.md` & `CobWeb-lnx-1.1.0/LICENSE.md`

 * *Files identical despite different names*

### Comparing `CobWeb-lnx-1.0.1/PKG-INFO` & `CobWeb-lnx-1.1.0/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: CobWeb-lnx
-Version: 1.0.1
+Version: 1.1.0
 Summary: CobWeb is a Python library for web scraping. The library consists of two classes: Spider and Scraper.
 Author-email: "Gonçalo Marques (_lnx/lnxdread)" <gmgoncalo7@gmail.com>
 Project-URL: Homepage, https://github.com/GoncaloMark/Amara-CobWeb
 Project-URL: Bug Tracker, https://github.com/GoncaloMark/Amara-CobWeb/issues
 Keywords: data,crawler,scraper
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
@@ -18,16 +18,16 @@
 CobWeb is a Python library for web scraping. The library consists of two classes: Spider and Scraper.
 
 ## Spider
 
 The Spider class is used to crawl a website and identify internal and external links. It has the following methods:
 
     __init__(self, url, max_hops = 0): Initializes a Spider object with the given URL and maximum number of links to follow from the initial URL.
-    getLinks(self): Crawls the website and identifies internal and external links.
-    showLinks(self): Returns the set of internal and external URLs found during crawling.
+    _getLinks(self): Crawls the website and identifies internal and external links.
+    _showLinks(self): Returns the set of internal and external URLs found during crawling.
     __str__(self): Returns a string representation of the Spider object.
     __repr__(self): Returns a string representation of the Spider object.
 
 ## Scraper
 
 The Scraper class extends the functionality of the Spider class by scraping HTML content from web pages based on user-defined parameters. It has the following methods:
 
@@ -38,74 +38,74 @@
 
 ## Installation
 
 You can install CobWeb using pip:
 
 ```bash
 
-        pip install CobWeb
+    pip install CobWeb
 
 ```
 
 ## Config
 
 Config is either an object in memory or a YAML file you can build by installing YAMLbuilder or by using the provided template!
 Example of a complete object:
 
- ```python 
-
-        config = {
-                    "url": 
-                    "hops": 
-                    "tags":
-                    "classes":
-                    "attrs":
-                    "attrV":
-                    "IDv":
-                    "selectors":
-                }
+```python
+config = {
+            "url": 
+            "hops": 
+            "tags":
+            "classes":
+            "attrs":
+            "attrV":
+            "IDv":
+            "selectors":
+        }
 ```
 
 Example of YAML file (If you choose this path call the config_parser function and give it a valid path!):
 
 ```yaml
-        IDv:
-        attrV: []
-        attrs: []
-        classes: []
-        hops: 
-        selectors: []
-        tags:
-        - 
-        - 
-        url: 
+IDv:
+attrV: []
+attrs: []
+classes: []
+hops: 
+selectors: []
+tags:
+    - 
+    - 
+url: 
 ```
 
 ## Example Usage
 
 ```python
 
-        from CobWeb import Spider, Scraper
+from CobWeb import Spider, Scraper
 
-        # Create a Spider object with a URL and maximum number of hops
-        spider = Spider("https://example.com", max_hops=10)
+# Create a Spider object with a URL and maximum number of hops
+spider = Spider("https://example.com", max_hops=10)
 
-        # Get the internal and external links
-        internal_links, external_links = spider.showLinks()
-
-        # Create a Scraper object with a configuration dictionary
-        # hops defines how deep it will scrape, it uses the Spider internally to get more links and scrape from those pages! If you just want to scrape from a single page set it to 0 or don't provide hops
-        config = {
-            "url": "https://example.com",
-            "hops": 2,
-            "tags": ["h1", "p"]
-        }
-        scraper = Scraper(config)
+# Get the internal and external links
+links = spider.run()
+print(links)
+
+# Create a Scraper object with a configuration dictionary
+# hops defines how deep it will scrape, it uses the Spider internally to get more links and scrape from those pages! If you just want to scrape from a single page set it to 0 or don't provide hops
+config = {
+    "url": "https://example.com",
+    "hops": 2,
+    "tags": ["h1", "p"]
+    }
+scraper = Scraper(config)
 
-        # Scrape HTML content from web pages based on user-defined parameters
-        results = scraper.run()
+# Scrape HTML content from web pages based on user-defined parameters
+results = scraper.run()
 
-        # Print the results it shall be a dictionary with arrays of scraped content separated by element, attributes, etc provided in the config!
-        print(results)
+# Print the results it shall be a dictionary with arrays of scraped content separated by element, attributes, etc provided in the config!
+print(results)
 
 
 ```
```

### Comparing `CobWeb-lnx-1.0.1/README.md` & `CobWeb-lnx-1.1.0/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -3,16 +3,16 @@
 CobWeb is a Python library for web scraping. The library consists of two classes: Spider and Scraper.
 
 ## Spider
 
 The Spider class is used to crawl a website and identify internal and external links. It has the following methods:
 
     __init__(self, url, max_hops = 0): Initializes a Spider object with the given URL and maximum number of links to follow from the initial URL.
-    getLinks(self): Crawls the website and identifies internal and external links.
-    showLinks(self): Returns the set of internal and external URLs found during crawling.
+    _getLinks(self): Crawls the website and identifies internal and external links.
+    _showLinks(self): Returns the set of internal and external URLs found during crawling.
     __str__(self): Returns a string representation of the Spider object.
     __repr__(self): Returns a string representation of the Spider object.
 
 ## Scraper
 
 The Scraper class extends the functionality of the Spider class by scraping HTML content from web pages based on user-defined parameters. It has the following methods:
 
@@ -23,74 +23,74 @@
 
 ## Installation
 
 You can install CobWeb using pip:
 
 ```bash
 
-        pip install CobWeb
+    pip install CobWeb
 
 ```
 
 ## Config
 
 Config is either an object in memory or a YAML file you can build by installing YAMLbuilder or by using the provided template!
 Example of a complete object:
 
- ```python 
-
-        config = {
-                    "url": 
-                    "hops": 
-                    "tags":
-                    "classes":
-                    "attrs":
-                    "attrV":
-                    "IDv":
-                    "selectors":
-                }
+```python
+config = {
+            "url": 
+            "hops": 
+            "tags":
+            "classes":
+            "attrs":
+            "attrV":
+            "IDv":
+            "selectors":
+        }
 ```
 
 Example of YAML file (If you choose this path call the config_parser function and give it a valid path!):
 
 ```yaml
-        IDv:
-        attrV: []
-        attrs: []
-        classes: []
-        hops: 
-        selectors: []
-        tags:
-        - 
-        - 
-        url: 
+IDv:
+attrV: []
+attrs: []
+classes: []
+hops: 
+selectors: []
+tags:
+    - 
+    - 
+url: 
 ```
 
 ## Example Usage
 
 ```python
 
-        from CobWeb import Spider, Scraper
+from CobWeb import Spider, Scraper
 
-        # Create a Spider object with a URL and maximum number of hops
-        spider = Spider("https://example.com", max_hops=10)
+# Create a Spider object with a URL and maximum number of hops
+spider = Spider("https://example.com", max_hops=10)
 
-        # Get the internal and external links
-        internal_links, external_links = spider.showLinks()
-
-        # Create a Scraper object with a configuration dictionary
-        # hops defines how deep it will scrape, it uses the Spider internally to get more links and scrape from those pages! If you just want to scrape from a single page set it to 0 or don't provide hops
-        config = {
-            "url": "https://example.com",
-            "hops": 2,
-            "tags": ["h1", "p"]
-        }
-        scraper = Scraper(config)
+# Get the internal and external links
+links = spider.run()
+print(links)
+
+# Create a Scraper object with a configuration dictionary
+# hops defines how deep it will scrape, it uses the Spider internally to get more links and scrape from those pages! If you just want to scrape from a single page set it to 0 or don't provide hops
+config = {
+    "url": "https://example.com",
+    "hops": 2,
+    "tags": ["h1", "p"]
+    }
+scraper = Scraper(config)
 
-        # Scrape HTML content from web pages based on user-defined parameters
-        results = scraper.run()
+# Scrape HTML content from web pages based on user-defined parameters
+results = scraper.run()
 
-        # Print the results it shall be a dictionary with arrays of scraped content separated by element, attributes, etc provided in the config!
-        print(results)
+# Print the results it shall be a dictionary with arrays of scraped content separated by element, attributes, etc provided in the config!
+print(results)
 
 
 ```
```

### Comparing `CobWeb-lnx-1.0.1/pyproject.toml` & `CobWeb-lnx-1.1.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "CobWeb-lnx"
-version = "1.0.1"
+version = "1.1.0"
 authors = [
     { name="Gonçalo Marques (_lnx/lnxdread)", email="gmgoncalo7@gmail.com" },
 ]
 description = "CobWeb is a Python library for web scraping. The library consists of two classes: Spider and Scraper."
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
```

### Comparing `CobWeb-lnx-1.0.1/src/CobWeb/crawler.py` & `CobWeb-lnx-1.1.0/src/CobWeb/crawler.py`

 * *Files 2% similar despite different names*

```diff
@@ -48,15 +48,15 @@
         @returns True if the URL is valid, False otherwise.
         """
     def __validateURL(self, url):
         parsed = urlparse(url)
         return bool(parsed.netloc) and bool(parsed.scheme)
 
     ## Crawls the website and identifies internal and external links.
-    async def getLinks(self, session = aiohttp.ClientSession):
+    async def _getLinks(self, session = aiohttp.ClientSession):
         page = await session.request("GET", self._url)
         page.raise_for_status()
         domain_name = urlparse(self._url).netloc
         html = await page.text()
         soup = BeautifulSoup(html, "lxml")
         #TODO: throw netwrok errors like 403 forbidden
 
@@ -89,21 +89,33 @@
             elif href not in self._internal_urls:
                 self._internal_urls.add(href)
                 continue
 
     """Returns the set of internal and external URLs found during crawling.
     @returns A tuple containing the set of internal URLs and the set of external URLs, or just the set of internal URLs or external URLs if one of them is empty.
     """
-    def showLinks(self):
+    def _showLinks(self):
         if self._internal_urls and self._external_urls:
             return (self._internal_urls, self._external_urls)
         elif self._internal_urls:
             return self._internal_urls
         elif self._external_urls:
             return self._external_urls
+        
+    """Crawls the requested website with the specifiend number of hops"""
+    async def __crawl(self):
+        async with aiohttp.ClientSession() as session:
+            if self.hops != 0:
+                await self._getLinks(session)
+    
+    """Runs the event loop and returns the urls found in the page!"""
+    def run(self):
+        asyncio.run(self.__crawl())
+        return self._showLinks()
+
 
     def __str__(self):
         """
         Returns a string representation of the Spider object.
 
         Returns:
             str: A string containing the URL and hops of the Spider object.
@@ -244,16 +256,16 @@
 
         Returns:
             Dict with arrays of scraped content
 
         """
         async with aiohttp.ClientSession() as session:
             if self.__config["hops"] != 0:
-                await self.getLinks(session)
-                links = self.showLinks()
+                await self._getLinks(session)
+                links = self._showLinks()
                 if type(links) == tuple:
                     internal, external = links
                     self.__Ilinks = [self.__config["url"], *internal, *external]
                 else:
                     self.__Ilinks = [self.__config["url"], *links]
             else:
                 self.__Ilinks = [self.__config["url"]]
@@ -305,27 +317,27 @@
     #SCRAPER TEST WITH FILE! 
     """ print("Specify config file (YAML) Path!")
     config_path = input()
     if path.exists(config_path) != True:
         raise ValueError """
     
     #SCRAPER TEST WITH CONFIG OBJECT! 
-    config = {
+    """ config = {
             "url": "http://quotes.toscrape.com/",
             "tags": ["small", "h3"],
             "hops": 1000
-        } 
+        }  """
 
     #config = config_parser(config_file=config_path)
-    scrape = Scraper(config=config)
-    #scrape.getLinks()
-    #print(scrape.showLinks())
+    #scrape = Scraper(config=config)
+    #scrape._getLinks()
+    #print(scrape._showLinks())
     #result = scrape.run()
     #print(result)
-    time = timeit.timeit(scrape.run, number=1)
-    print(time)
+    #time = timeit.timeit(scrape.run, number=1)
+    #print(time)
     
-    """ 
-    SPIDER TEST!
-    crawl = Spider("url", 10)
-    crawl.getLinks()
-    print(crawl.showLinks()) """
+    # SPIDER TEST!
+    spider = Spider("https://example.com", max_hops=10)
+    # Get the internal and external links
+    links = spider.run()
+    print(links)
```

### Comparing `CobWeb-lnx-1.0.1/src/CobWeb_lnx.egg-info/PKG-INFO` & `CobWeb-lnx-1.1.0/src/CobWeb_lnx.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: CobWeb-lnx
-Version: 1.0.1
+Version: 1.1.0
 Summary: CobWeb is a Python library for web scraping. The library consists of two classes: Spider and Scraper.
 Author-email: "Gonçalo Marques (_lnx/lnxdread)" <gmgoncalo7@gmail.com>
 Project-URL: Homepage, https://github.com/GoncaloMark/Amara-CobWeb
 Project-URL: Bug Tracker, https://github.com/GoncaloMark/Amara-CobWeb/issues
 Keywords: data,crawler,scraper
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
@@ -18,16 +18,16 @@
 CobWeb is a Python library for web scraping. The library consists of two classes: Spider and Scraper.
 
 ## Spider
 
 The Spider class is used to crawl a website and identify internal and external links. It has the following methods:
 
     __init__(self, url, max_hops = 0): Initializes a Spider object with the given URL and maximum number of links to follow from the initial URL.
-    getLinks(self): Crawls the website and identifies internal and external links.
-    showLinks(self): Returns the set of internal and external URLs found during crawling.
+    _getLinks(self): Crawls the website and identifies internal and external links.
+    _showLinks(self): Returns the set of internal and external URLs found during crawling.
     __str__(self): Returns a string representation of the Spider object.
     __repr__(self): Returns a string representation of the Spider object.
 
 ## Scraper
 
 The Scraper class extends the functionality of the Spider class by scraping HTML content from web pages based on user-defined parameters. It has the following methods:
 
@@ -38,74 +38,74 @@
 
 ## Installation
 
 You can install CobWeb using pip:
 
 ```bash
 
-        pip install CobWeb
+    pip install CobWeb
 
 ```
 
 ## Config
 
 Config is either an object in memory or a YAML file you can build by installing YAMLbuilder or by using the provided template!
 Example of a complete object:
 
- ```python 
-
-        config = {
-                    "url": 
-                    "hops": 
-                    "tags":
-                    "classes":
-                    "attrs":
-                    "attrV":
-                    "IDv":
-                    "selectors":
-                }
+```python
+config = {
+            "url": 
+            "hops": 
+            "tags":
+            "classes":
+            "attrs":
+            "attrV":
+            "IDv":
+            "selectors":
+        }
 ```
 
 Example of YAML file (If you choose this path call the config_parser function and give it a valid path!):
 
 ```yaml
-        IDv:
-        attrV: []
-        attrs: []
-        classes: []
-        hops: 
-        selectors: []
-        tags:
-        - 
-        - 
-        url: 
+IDv:
+attrV: []
+attrs: []
+classes: []
+hops: 
+selectors: []
+tags:
+    - 
+    - 
+url: 
 ```
 
 ## Example Usage
 
 ```python
 
-        from CobWeb import Spider, Scraper
+from CobWeb import Spider, Scraper
 
-        # Create a Spider object with a URL and maximum number of hops
-        spider = Spider("https://example.com", max_hops=10)
+# Create a Spider object with a URL and maximum number of hops
+spider = Spider("https://example.com", max_hops=10)
 
-        # Get the internal and external links
-        internal_links, external_links = spider.showLinks()
-
-        # Create a Scraper object with a configuration dictionary
-        # hops defines how deep it will scrape, it uses the Spider internally to get more links and scrape from those pages! If you just want to scrape from a single page set it to 0 or don't provide hops
-        config = {
-            "url": "https://example.com",
-            "hops": 2,
-            "tags": ["h1", "p"]
-        }
-        scraper = Scraper(config)
+# Get the internal and external links
+links = spider.run()
+print(links)
+
+# Create a Scraper object with a configuration dictionary
+# hops defines how deep it will scrape, it uses the Spider internally to get more links and scrape from those pages! If you just want to scrape from a single page set it to 0 or don't provide hops
+config = {
+    "url": "https://example.com",
+    "hops": 2,
+    "tags": ["h1", "p"]
+    }
+scraper = Scraper(config)
 
-        # Scrape HTML content from web pages based on user-defined parameters
-        results = scraper.run()
+# Scrape HTML content from web pages based on user-defined parameters
+results = scraper.run()
 
-        # Print the results it shall be a dictionary with arrays of scraped content separated by element, attributes, etc provided in the config!
-        print(results)
+# Print the results it shall be a dictionary with arrays of scraped content separated by element, attributes, etc provided in the config!
+print(results)
 
 
 ```
```

