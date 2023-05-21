# Comparing `tmp/pydude-0.9.1.tar.gz` & `tmp/pydude-0.9.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pydude-0.9.1.tar", max compression
+gzip compressed data, was "pydude-0.9.2.tar", max compression
```

## Comparing `pydude-0.9.1.tar` & `pydude-0.9.2.tar`

### file list

```diff
@@ -1,19 +1,19 @@
--rw-r--r--   0        0        0    34523 2022-03-11 21:29:40.017499 pydude-0.9.1/LICENSE
--rw-r--r--   0        0        0     7674 2022-03-11 21:29:40.017499 pydude-0.9.1/README.md
--rw-r--r--   0        0        0     5946 2022-03-11 21:29:40.021499 pydude-0.9.1/dude/__init__.py
--rw-r--r--   0        0        0    12234 2022-03-11 21:29:40.021499 pydude-0.9.1/dude/base.py
--rw-r--r--   0        0        0      386 2022-03-11 21:29:40.021499 pydude-0.9.1/dude/context.py
--rw-r--r--   0        0        0        0 2022-03-11 21:29:40.021499 pydude-0.9.1/dude/optional/__init__.py
--rw-r--r--   0        0        0     6144 2022-03-11 21:29:40.021499 pydude-0.9.1/dude/optional/beautifulsoup_scraper.py
--rw-r--r--   0        0        0     6357 2022-03-11 21:29:40.021499 pydude-0.9.1/dude/optional/lxml_scraper.py
--rw-r--r--   0        0        0     6263 2022-03-11 21:29:40.021499 pydude-0.9.1/dude/optional/parsel_scraper.py
--rw-r--r--   0        0        0     7069 2022-03-11 21:29:40.021499 pydude-0.9.1/dude/optional/pyppeteer_scraper.py
--rw-r--r--   0        0        0     9834 2022-03-11 21:29:40.021499 pydude-0.9.1/dude/optional/selenium_scraper.py
--rw-r--r--   0        0        0     9168 2022-03-11 21:29:40.021499 pydude-0.9.1/dude/playwright_scraper.py
--rw-r--r--   0        0        0     2390 2022-03-11 21:29:40.021499 pydude-0.9.1/dude/rule.py
--rw-r--r--   0        0        0      553 2022-03-11 21:29:40.021499 pydude-0.9.1/dude/scraped_data.py
--rw-r--r--   0        0        0     3729 2022-03-11 21:29:40.021499 pydude-0.9.1/dude/scraper.py
--rw-r--r--   0        0        0     2305 2022-03-11 21:29:40.021499 pydude-0.9.1/dude/storage.py
--rw-r--r--   0        0        0     3022 2022-03-11 21:29:40.025499 pydude-0.9.1/pyproject.toml
--rw-r--r--   0        0        0     9113 2022-03-11 21:29:52.641403 pydude-0.9.1/setup.py
--rw-r--r--   0        0        0     9442 2022-03-11 21:29:52.642272 pydude-0.9.1/PKG-INFO
+-rw-r--r--   0        0        0    34523 2022-03-12 14:20:57.473200 pydude-0.9.2/LICENSE
+-rw-r--r--   0        0        0     7674 2022-03-12 14:20:57.473200 pydude-0.9.2/README.md
+-rw-r--r--   0        0        0     5946 2022-03-12 14:20:57.477200 pydude-0.9.2/dude/__init__.py
+-rw-r--r--   0        0        0    12234 2022-03-12 14:20:57.477200 pydude-0.9.2/dude/base.py
+-rw-r--r--   0        0        0      386 2022-03-12 14:20:57.477200 pydude-0.9.2/dude/context.py
+-rw-r--r--   0        0        0        0 2022-03-12 14:20:57.477200 pydude-0.9.2/dude/optional/__init__.py
+-rw-r--r--   0        0        0     6144 2022-03-12 14:20:57.477200 pydude-0.9.2/dude/optional/beautifulsoup_scraper.py
+-rw-r--r--   0        0        0     6357 2022-03-12 14:20:57.477200 pydude-0.9.2/dude/optional/lxml_scraper.py
+-rw-r--r--   0        0        0     6263 2022-03-12 14:20:57.477200 pydude-0.9.2/dude/optional/parsel_scraper.py
+-rw-r--r--   0        0        0     7096 2022-03-12 14:20:57.477200 pydude-0.9.2/dude/optional/pyppeteer_scraper.py
+-rw-r--r--   0        0        0     9977 2022-03-12 14:20:57.477200 pydude-0.9.2/dude/optional/selenium_scraper.py
+-rw-r--r--   0        0        0     9610 2022-03-12 14:20:57.477200 pydude-0.9.2/dude/playwright_scraper.py
+-rw-r--r--   0        0        0     2390 2022-03-12 14:20:57.477200 pydude-0.9.2/dude/rule.py
+-rw-r--r--   0        0        0      553 2022-03-12 14:20:57.477200 pydude-0.9.2/dude/scraped_data.py
+-rw-r--r--   0        0        0     3729 2022-03-12 14:20:57.477200 pydude-0.9.2/dude/scraper.py
+-rw-r--r--   0        0        0     2305 2022-03-12 14:20:57.477200 pydude-0.9.2/dude/storage.py
+-rw-r--r--   0        0        0     3022 2022-03-12 14:20:57.481200 pydude-0.9.2/pyproject.toml
+-rw-r--r--   0        0        0     9113 2022-03-12 14:21:11.510365 pydude-0.9.2/setup.py
+-rw-r--r--   0        0        0     9442 2022-03-12 14:21:11.511482 pydude-0.9.2/PKG-INFO
```

### Comparing `pydude-0.9.1/LICENSE` & `pydude-0.9.2/LICENSE`

 * *Files identical despite different names*

### Comparing `pydude-0.9.1/README.md` & `pydude-0.9.2/README.md`

 * *Files identical despite different names*

### Comparing `pydude-0.9.1/dude/__init__.py` & `pydude-0.9.2/dude/__init__.py`

 * *Files identical despite different names*

### Comparing `pydude-0.9.1/dude/base.py` & `pydude-0.9.2/dude/base.py`

 * *Files identical despite different names*

### Comparing `pydude-0.9.1/dude/optional/beautifulsoup_scraper.py` & `pydude-0.9.2/dude/optional/beautifulsoup_scraper.py`

 * *Files identical despite different names*

### Comparing `pydude-0.9.1/dude/optional/lxml_scraper.py` & `pydude-0.9.2/dude/optional/lxml_scraper.py`

 * *Files identical despite different names*

### Comparing `pydude-0.9.1/dude/optional/parsel_scraper.py` & `pydude-0.9.2/dude/optional/parsel_scraper.py`

 * *Files identical despite different names*

### Comparing `pydude-0.9.1/dude/optional/pyppeteer_scraper.py` & `pydude-0.9.2/dude/optional/pyppeteer_scraper.py`

 * *Files 2% similar despite different names*

```diff
@@ -102,15 +102,15 @@
         urls: Sequence[str],
         headless: bool,
         pages: int,
         proxy: Optional[Dict],
         output: Optional[str],
         format: str,
     ) -> None:
-        launch_args: Dict[str, Any] = {"headless": headless, "args": ["--no-sandbox"]}
+        launch_args: Dict[str, Any] = {"headless": headless, "args": ["--no-sandbox", "--disable-notifications"]}
         if proxy:
             launch_args["args"] = [f"--proxy-server={proxy['server']}"]
 
         browser = await launch(options=launch_args)
         page = await browser.newPage()
 
         if proxy and proxy["username"] and proxy["password"]:
```

### Comparing `pydude-0.9.1/dude/optional/selenium_scraper.py` & `pydude-0.9.2/dude/optional/selenium_scraper.py`

 * *Files 2% similar despite different names*

```diff
@@ -206,18 +206,20 @@
     @staticmethod
     def _get_driver(browser_type: str, headless: bool) -> WebDriver:
         # TODO: Add more drivers: https://github.com/SergeyPirogov/webdriver_manager#webdriver-manager-for-python
         if browser_type == "firefox":
             executable_path = GeckoDriverManager().install()
             firefox_options = FirefoxOptions()
             firefox_options.headless = headless
+            firefox_options.set_preference("dom.webnotifications.enabled", False)
             return webdriver.Firefox(service=FirefoxService(executable_path=executable_path), options=firefox_options)
 
         chrome_options = ChromeOptions()
         chrome_options.headless = headless
+        chrome_options.add_argument("disable-notifications")
         executable_path = ChromeDriverManager(
             chrome_type=ChromeType.CHROMIUM, version=os.getenv("CHROMEDRIVER_VERSION", "latest")
         ).install()
         return webdriver.Chrome(service=ChromeService(executable_path=executable_path), options=chrome_options)
 
     def collect_elements(self, driver: WebDriver = None) -> Iterable[Tuple[str, int, int, int, Any, Callable]]:
         """
```

### Comparing `pydude-0.9.1/dude/playwright_scraper.py` & `pydude-0.9.2/dude/playwright_scraper.py`

 * *Files 12% similar despite different names*

```diff
@@ -149,15 +149,20 @@
         pages: int,
         proxy: Optional[sync_api.ProxySettings],
         output: Optional[str],
         format: str,
     ) -> None:
         # FIXME: Coverage fails to cover anything within this context manager block
         with sync_playwright() as p:
-            browser = p[browser_type].launch(headless=headless, proxy=proxy)
+            args = []
+            if browser_type == "chromium":
+                args.append("--disable-notifications")
+            browser = p[browser_type].launch(
+                headless=headless, proxy=proxy, args=args, firefox_user_prefs={"dom.webnotifications.enabled": False}
+            )
             page = browser.new_page()
             self._scrape_sync(page, urls, pages)
             browser.close()
         self._save(format, output)
 
     def _scrape_sync(self, page: sync_api.Page, urls: Sequence[str], pages: int) -> None:
         for _ in (page.goto(url) for url in urls):
@@ -178,15 +183,20 @@
         browser_type: str,
         pages: int,
         proxy: Optional[sync_api.ProxySettings],
         output: Optional[str],
         format: str,
     ) -> None:
         async with async_playwright() as p:
-            browser = await p[browser_type].launch(headless=headless, proxy=proxy)
+            args = []
+            if browser_type == "chromium":
+                args.append("--disable-notifications")
+            browser = await p[browser_type].launch(
+                headless=headless, proxy=proxy, args=args, firefox_user_prefs={"dom.webnotifications.enabled": False}
+            )
             page = await browser.new_page()
             for url in urls:
                 await page.goto(url)
                 logger.info("Loaded page %s", page.url)
                 await self.setup_async(page=page)
 
                 for i in range(1, pages + 1):
```

### Comparing `pydude-0.9.1/dude/rule.py` & `pydude-0.9.2/dude/rule.py`

 * *Files identical despite different names*

### Comparing `pydude-0.9.1/dude/scraped_data.py` & `pydude-0.9.2/dude/scraped_data.py`

 * *Files identical despite different names*

### Comparing `pydude-0.9.1/dude/scraper.py` & `pydude-0.9.2/dude/scraper.py`

 * *Files identical despite different names*

### Comparing `pydude-0.9.1/dude/storage.py` & `pydude-0.9.2/dude/storage.py`

 * *Files identical despite different names*

### Comparing `pydude-0.9.1/pyproject.toml` & `pydude-0.9.2/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "pydude"
-version = "0.9.1"
+version = "0.9.2"
 repository = "https://github.com/roniemartinez/dude"
 description = "dude uncomplicated data extraction"
 authors = ["Ronie Martinez <ronmarti18@gmail.com>"]
 license = "AGPL-3.0-or-later"
 readme = "README.md"
 documentation = "https://roniemartinez.github.io/dude/"
 keywords = [
```

### Comparing `pydude-0.9.1/setup.py` & `pydude-0.9.2/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -20,15 +20,15 @@
  'selenium': ['selenium>=4.1.3,<5.0.0', 'webdriver-manager>=3.5.3,<4.0.0']}
 
 entry_points = \
 {'console_scripts': ['dude = dude:cli']}
 
 setup_kwargs = {
     'name': 'pydude',
-    'version': '0.9.1',
+    'version': '0.9.2',
     'description': 'dude uncomplicated data extraction',
     'long_description': '<table>\n    <tr>\n        <td>License</td>\n        <td><img src=\'https://img.shields.io/pypi/l/pydude.svg?style=for-the-badge\' alt="License"></td>\n        <td>Version</td>\n        <td><img src=\'https://img.shields.io/pypi/v/pydude.svg?logo=pypi&style=for-the-badge\' alt="Version"></td>\n    </tr>\n    <tr>\n        <td>Github Actions</td>\n        <td><img src=\'https://img.shields.io/github/workflow/status/roniemartinez/dude/Python?label=actions&logo=github%20actions&style=for-the-badge\' alt="Github Actions"></td>\n        <td>Coverage</td>\n        <td><img src=\'https://img.shields.io/codecov/c/github/roniemartinez/dude/branch?label=codecov&logo=codecov&style=for-the-badge\' alt="CodeCov"></td>\n    </tr>\n    <tr>\n        <td>Supported versions</td>\n        <td><img src=\'https://img.shields.io/pypi/pyversions/pydude.svg?logo=python&style=for-the-badge\' alt="Python Versions"></td>\n        <td>Wheel</td>\n        <td><img src=\'https://img.shields.io/pypi/wheel/pydude.svg?style=for-the-badge\' alt="Wheel"></td>\n    </tr>\n    <tr>\n        <td>Status</td>\n        <td><img src=\'https://img.shields.io/pypi/status/pydude.svg?style=for-the-badge\' alt="Status"></td>\n        <td>Downloads</td>\n        <td><img src=\'https://img.shields.io/pypi/dm/pydude.svg?style=for-the-badge\' alt="Downloads"></td>\n    </tr>\n</table>\n\n# dude uncomplicated data extraction\n\nDude is a very simple framework for writing a web scraper using Python decorators.\nThe design, inspired by [Flask](https://github.com/pallets/flask), was to easily build a web scraper in just a few lines of code.\nDude has an easy-to-learn syntax.\n\n> 🚨 Dude is currently in Pre-Alpha. Please expect breaking changes.\n\n## Installation\n\nTo install, simply run the following from terminal.\n\n```bash\npip install pydude\nplaywright install  # Install playwright binaries for Chrome, Firefox and Webkit.\n```\n\n## Minimal web scraper\n\nThe simplest web scraper will look like this:\n\n```python\nfrom dude import select\n\n\n@select(css="a")\ndef get_link(element):\n    return {"url": element.get_attribute("href")}\n```\n\nThe example above will get all the [hyperlink](https://en.wikipedia.org/wiki/Hyperlink#HTML) elements in a page and calls the handler function `get_link()` for each element.\n\n## How to run the scraper\n\nYou can run your scraper from terminal/shell/command-line by supplying URLs, the output filename of your choice and the paths to your python scripts to `dude scrape` command.\n\n```bash\ndude scrape --url "<url>" --output data.json path/to/script.py\n```\n\n## Features\n\n- Simple [Flask](https://github.com/pallets/flask)-inspired design - build a scraper with decorators.\n- Uses [Playwright](https://playwright.dev/python/) API - run your scraper in Chrome, Firefox and Webkit and leverage Playwright\'s powerful selector engine supporting CSS, XPath, text, regex, etc.\n- Data grouping - group related scraping data.\n- URL pattern matching - run functions on specific URLs.\n- Priority - reorder functions based on priority.\n- Setup function - enable setup steps (clicking dialogs or login).\n- Navigate function - enable navigation steps to move to other pages.\n- Custom storage - option to save data to other formats or database.\n- Async support - write async handlers.\n- Option to use other parsers aside from Playwright.\n  - [BeautifulSoup4](https://roniemartinez.github.io/dude/advanced/09_beautifulsoup4.html) - `pip install pydude[bs4]`\n  - [Parsel](https://roniemartinez.github.io/dude/advanced/10_parsel.html) - `pip install pydude[parsel]`\n  - [lxml](https://roniemartinez.github.io/dude/advanced/11_lxml.html) - `pip install pydude[lxml]`\n  - [Pyppeteer](https://roniemartinez.github.io/dude/advanced/12_pyppeteer.html) - `pip install pydude[pyppeteer]`\n  - [Selenium](https://roniemartinez.github.io/dude/advanced/13_selenium.html) - `pip install pydude[selenium]`\n\n## Supported Parsers\n\nBy default, Dude uses Playwright but gives you an option to use parsers that you are familiar with.\nIt is possible to use parser backends like \n[BeautifulSoup4](https://www.crummy.com/software/BeautifulSoup/bs4/doc/), \n[Parsel](https://github.com/scrapy/parsel),\n[lxml](https://lxml.de/),\n[Pyppeteer](https://github.com/pyppeteer/pyppeteer), \nand [Selenium](https://github.com/SeleniumHQ/Selenium).\n\nHere is the summary of features supported by each parser.\n\n<table>\n<thead>\n  <tr>\n    <td rowspan="2" style=\'text-align:center;\'>Parser Backend</td>\n    <td rowspan="2" style=\'text-align:center;\'>Supports<br>Sync?</td>\n    <td rowspan="2" style=\'text-align:center;\'>Supports<br>Async?</td>\n    <td colspan="4" style=\'text-align:center;\'>Selectors</td>\n    <td rowspan="2" style=\'text-align:center;\'><a href="https://roniemartinez.github.io/dude/advanced/01_setup.html">Setup<br>Handler</a></td>\n    <td rowspan="2" style=\'text-align:center;\'><a href="https://roniemartinez.github.io/dude/advanced/02_navigate.html">Navigate<br>Handler</a></td>\n  </tr>\n  <tr>\n    <td>CSS</td>\n    <td>XPath</td>\n    <td>Text</td>\n    <td>Regex</td>\n  </tr>\n</thead>\n<tbody>\n  <tr>\n    <td>Playwright</td>\n    <td>✅</td>\n    <td>✅</td>\n    <td>✅</td>\n    <td>✅</td>\n    <td>✅</td>\n    <td>✅</td>\n    <td>✅</td>\n    <td>✅</td>\n  </tr>\n  <tr>\n    <td>BeautifulSoup4</td>\n    <td>✅</td>\n    <td>✅</td>\n    <td>✅</td>\n    <td>🚫</td>\n    <td>🚫</td>\n    <td>🚫</td>\n    <td>🚫</td>\n    <td>🚫</td>\n  </tr>\n  <tr>\n    <td>Parsel</td>\n    <td>✅</td>\n    <td>✅</td>\n    <td>✅</td>\n    <td>✅</td>\n    <td>✅</td>\n    <td>✅</td>\n    <td>🚫</td>\n    <td>🚫</td>\n  </tr>\n  <tr>\n    <td>lxml</td>\n    <td>✅</td>\n    <td>✅</td>\n    <td>✅</td>\n    <td>✅</td>\n    <td>✅</td>\n    <td>✅</td>\n    <td>🚫</td>\n    <td>🚫</td>\n  </tr>\n  <tr>\n    <td>Pyppeteer</td>\n    <td>🚫</td>\n    <td>✅</td>\n    <td>✅</td>\n    <td>✅</td>\n    <td>✅</td>\n    <td>🚫</td>\n    <td>✅</td>\n    <td>✅</td>\n  </tr>\n  <tr>\n    <td>Selenium</td>\n    <td>✅</td>\n    <td>✅</td>\n    <td>✅</td>\n    <td>✅</td>\n    <td>✅</td>\n    <td>🚫</td>\n    <td>✅</td>\n    <td>✅</td>\n  </tr>\n</tbody>\n</table>\n\n## Documentation\n\nRead the complete documentation at [https://roniemartinez.github.io/dude/](https://roniemartinez.github.io/dude/).\nAll the advanced and useful features are documented there.\n\n## Support\n\nThis project is at a very early stage. This dude needs some love! ❤️\n\nContribute to this project by feature requests, idea discussions, reporting bugs, opening pull requests, or through Github Sponsors. Your help is highly appreciated.\n\n[![Github Sponsors](https://img.shields.io/github/sponsors/roniemartinez?label=github%20sponsors&logo=github%20sponsors&style=for-the-badge)](https://github.com/sponsors/roniemartinez)\n\n## Requirements\n\n- ✅ Any dude should know how to work with selectors (CSS or XPath).\n- ✅ This library was built on top of [Playwright](https://github.com/microsoft/playwright-python). Any dude should be at least familiar with the basics of Playwright - they also extended the selectors to support text, regular expressions, etc. See [Selectors | Playwright Python](https://playwright.dev/python/docs/selectors).\n- ✅ Python decorators... you\'ll live, dude!\n\n## Why name this project "dude"?\n\n- ✅ A [Recursive acronym](https://en.wikipedia.org/wiki/Recursive_acronym) looks nice.\n- ✅ Adding "uncomplicated" (like [`ufw`](https://wiki.ubuntu.com/UncomplicatedFirewall)) into the name says it is a very simple framework. \n- ✅ Puns! I also think that if you want to do web scraping, there\'s probably some random dude around the corner who can make it very easy for you to start with it. 😊\n\n## Author\n\n[Ronie Martinez](mailto:ronmarti18@gmail.com)\n',
     'author': 'Ronie Martinez',
     'author_email': 'ronmarti18@gmail.com',
     'maintainer': None,
     'maintainer_email': None,
     'url': 'https://github.com/roniemartinez/dude',
```

### Comparing `pydude-0.9.1/PKG-INFO` & `pydude-0.9.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pydude
-Version: 0.9.1
+Version: 0.9.2
 Summary: dude uncomplicated data extraction
 Home-page: https://github.com/roniemartinez/dude
 License: AGPL-3.0-or-later
 Keywords: scraping
 Author: Ronie Martinez
 Author-email: ronmarti18@gmail.com
 Requires-Python: >=3.7,<4.0
```

