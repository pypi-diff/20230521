# Comparing `tmp/tessa-0.6.0.tar.gz` & `tmp/tessa-0.7.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tessa-0.6.0.tar", max compression
+gzip compressed data, was "tessa-0.7.0.tar", max compression
```

## Comparing `tessa-0.6.0.tar` & `tessa-0.7.0.tar`

### file list

```diff
@@ -1,29 +1,29 @@
--rw-r--r--   0        0        0     1083 2022-04-10 10:04:52.776933 tessa-0.6.0/LICENSE
--rw-r--r--   0        0        0     1112 2023-04-03 08:38:02.094742 tessa-0.6.0/pyproject.toml
--rw-r--r--   0        0        0     5845 2022-10-02 07:49:11.514152 tessa-0.6.0/README.md
--rw-r--r--   0        0        0      294 2023-04-03 08:40:28.843926 tessa-0.6.0/tessa/__init__.py
--rw-r--r--   0        0        0     1219 2022-09-30 09:10:45.569141 tessa-0.6.0/tessa/price/__init__.py
--rw-r--r--   0        0        0     1359 2022-09-30 09:10:45.569141 tessa-0.6.0/tessa/price/coingecko.py
--rw-r--r--   0        0        0     3295 2023-04-03 08:28:24.833664 tessa-0.6.0/tessa/price/price.py
--rw-r--r--   0        0        0      814 2022-09-30 09:10:45.570136 tessa-0.6.0/tessa/price/types.py
--rw-r--r--   0        0        0     1533 2023-01-02 19:45:05.131447 tessa-0.6.0/tessa/price/yahoo.py
--rw-r--r--   0        0        0      817 2022-09-30 09:10:45.571135 tessa-0.6.0/tessa/search/__init__.py
--rw-r--r--   0        0        0     1264 2022-09-30 09:10:45.571135 tessa-0.6.0/tessa/search/coingecko.py
--rw-r--r--   0        0        0      624 2022-09-30 09:10:45.571135 tessa-0.6.0/tessa/search/search.py
--rw-r--r--   0        0        0     8415 2022-09-30 09:10:45.572138 tessa-0.6.0/tessa/search/search_result.py
--rw-r--r--   0        0        0     3230 2022-09-30 09:10:45.572138 tessa-0.6.0/tessa/search/yahoo.py
--rw-r--r--   0        0        0      456 2022-09-30 09:10:45.572138 tessa-0.6.0/tessa/sources/__init__.py
--rw-r--r--   0        0        0     2943 2022-09-30 09:10:45.573137 tessa-0.6.0/tessa/sources/low_level_rate_limiter.py
--rw-r--r--   0        0        0     1484 2022-09-30 09:10:45.573137 tessa-0.6.0/tessa/sources/rate_limiter.py
--rw-r--r--   0        0        0     2797 2023-04-03 08:28:24.834171 tessa-0.6.0/tessa/sources/sources.py
--rw-r--r--   0        0        0      972 2022-09-30 09:10:45.574136 tessa-0.6.0/tessa/sources/sources_directory.py
--rw-r--r--   0        0        0      218 2022-09-30 09:10:45.574136 tessa-0.6.0/tessa/sources/sourcetype.py
--rw-r--r--   0        0        0      973 2022-09-30 09:10:45.575684 tessa-0.6.0/tessa/symbol/__init__.py
--rw-r--r--   0        0        0     3486 2022-09-30 09:10:45.575684 tessa-0.6.0/tessa/symbol/extended_symbol.py
--rw-r--r--   0        0        0      130 2022-09-30 09:10:45.576686 tessa-0.6.0/tessa/symbol/geo/__init__.py
--rw-r--r--   0        0        0     4788 2022-09-30 09:10:45.576686 tessa-0.6.0/tessa/symbol/geo/countrynames.py
--rw-r--r--   0        0        0     4811 2022-09-30 09:10:45.577686 tessa-0.6.0/tessa/symbol/geo/jurisdiction2region.py
--rw-r--r--   0        0        0     4725 2022-09-30 09:10:45.577686 tessa-0.6.0/tessa/symbol/symbol.py
--rw-r--r--   0        0        0     3206 2022-09-30 08:03:43.472741 tessa-0.6.0/tessa/symbol/symbolcollection.py
--rw-r--r--   0        0        0     6780 1970-01-01 00:00:00.000000 tessa-0.6.0/setup.py
--rw-r--r--   0        0        0     6735 1970-01-01 00:00:00.000000 tessa-0.6.0/PKG-INFO
+-rw-r--r--   0        0        0     1083 2022-04-10 10:04:52.776933 tessa-0.7.0/LICENSE
+-rw-r--r--   0        0        0     1090 2023-05-21 16:07:28.860065 tessa-0.7.0/pyproject.toml
+-rw-r--r--   0        0        0     5845 2022-10-02 07:49:11.514152 tessa-0.7.0/README.md
+-rw-r--r--   0        0        0      294 2023-05-21 16:07:44.375488 tessa-0.7.0/tessa/__init__.py
+-rw-r--r--   0        0        0     1219 2022-09-30 09:10:45.569141 tessa-0.7.0/tessa/price/__init__.py
+-rw-r--r--   0        0        0     1562 2023-05-21 15:42:00.992234 tessa-0.7.0/tessa/price/coingecko.py
+-rw-r--r--   0        0        0     3371 2023-05-21 15:53:44.716520 tessa-0.7.0/tessa/price/price.py
+-rw-r--r--   0        0        0     1114 2023-05-21 15:46:32.721421 tessa-0.7.0/tessa/price/types.py
+-rw-r--r--   0        0        0     1533 2023-05-21 15:42:00.993708 tessa-0.7.0/tessa/price/yahoo.py
+-rw-r--r--   0        0        0      817 2022-09-30 09:10:45.571135 tessa-0.7.0/tessa/search/__init__.py
+-rw-r--r--   0        0        0     1264 2022-09-30 09:10:45.571135 tessa-0.7.0/tessa/search/coingecko.py
+-rw-r--r--   0        0        0      624 2022-09-30 09:10:45.571135 tessa-0.7.0/tessa/search/search.py
+-rw-r--r--   0        0        0     8415 2022-09-30 09:10:45.572138 tessa-0.7.0/tessa/search/search_result.py
+-rw-r--r--   0        0        0     3230 2022-09-30 09:10:45.572138 tessa-0.7.0/tessa/search/yahoo.py
+-rw-r--r--   0        0        0      456 2022-09-30 09:10:45.572138 tessa-0.7.0/tessa/sources/__init__.py
+-rw-r--r--   0        0        0     2943 2022-09-30 09:10:45.573137 tessa-0.7.0/tessa/sources/low_level_rate_limiter.py
+-rw-r--r--   0        0        0     1931 2023-05-21 15:11:06.127141 tessa-0.7.0/tessa/sources/rate_limiter.py
+-rw-r--r--   0        0        0     3182 2023-05-21 15:44:25.238375 tessa-0.7.0/tessa/sources/sources.py
+-rw-r--r--   0        0        0      972 2022-09-30 09:10:45.574136 tessa-0.7.0/tessa/sources/sources_directory.py
+-rw-r--r--   0        0        0      218 2022-09-30 09:10:45.574136 tessa-0.7.0/tessa/sources/sourcetype.py
+-rw-r--r--   0        0        0      973 2022-09-30 09:10:45.575684 tessa-0.7.0/tessa/symbol/__init__.py
+-rw-r--r--   0        0        0     3486 2022-09-30 09:10:45.575684 tessa-0.7.0/tessa/symbol/extended_symbol.py
+-rw-r--r--   0        0        0      130 2022-09-30 09:10:45.576686 tessa-0.7.0/tessa/symbol/geo/__init__.py
+-rw-r--r--   0        0        0     4788 2022-09-30 09:10:45.576686 tessa-0.7.0/tessa/symbol/geo/countrynames.py
+-rw-r--r--   0        0        0     4811 2022-09-30 09:10:45.577686 tessa-0.7.0/tessa/symbol/geo/jurisdiction2region.py
+-rw-r--r--   0        0        0     4725 2022-09-30 09:10:45.577686 tessa-0.7.0/tessa/symbol/symbol.py
+-rw-r--r--   0        0        0     3206 2022-09-30 08:03:43.472741 tessa-0.7.0/tessa/symbol/symbolcollection.py
+-rw-r--r--   0        0        0     6760 1970-01-01 00:00:00.000000 tessa-0.7.0/setup.py
+-rw-r--r--   0        0        0     6701 1970-01-01 00:00:00.000000 tessa-0.7.0/PKG-INFO
```

### Comparing `tessa-0.6.0/LICENSE` & `tessa-0.7.0/LICENSE`

 * *Files identical despite different names*

### Comparing `tessa-0.6.0/pyproject.toml` & `tessa-0.7.0/pyproject.toml`

 * *Files 11% similar despite different names*

```diff
@@ -1,25 +1,24 @@
 [tool.poetry]
 name = "tessa"
-version = "0.6.0"
+version = "0.7.0"
 description = "Find financial assets and get their price history without worrying about different APIs or rate limiting."
 authors = ["ymyke"]
 license = "MIT"
 repository = "https://github.com/ymyke/tessa"
 homepage = "https://github.com/ymyke/tessa"
 documentation = "https://ymyke.github.io/tessa/tessa.html"
 readme = "README.md"
 keywords = ["python", "finance", "investing", "financial-analysis", "investment-analysis", "financial-data", "coingecko", "pycoingecko", "yahoo", "yahoo-finance", "yfinance"]
 
 [tool.poetry.dependencies]
 # General:
 python = ">=3.7.13,<3.10"
 pendulum = ">=2.1"
 # price- and search-specific:
-frozendict = ">=2.3"
 pycoingecko = ">=2.2"
 yfinance = "^0.2.3"
 beautifulsoup4 = "^4.11.1"
 # symbol-specific:
 seaborn = ">=0.11"
 matplotlib = ">=3.5"
 PyYAML = ">=6"
```

### Comparing `tessa-0.6.0/README.md` & `tessa-0.7.0/README.md`

 * *Files identical despite different names*

### Comparing `tessa-0.6.0/tessa/price/__init__.py` & `tessa-0.7.0/tessa/price/__init__.py`

 * *Files identical despite different names*

### Comparing `tessa-0.6.0/tessa/price/coingecko.py` & `tessa-0.7.0/tessa/price/coingecko.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,12 +1,17 @@
 """Everything coingecko-related (other than search)."""
 
 import pandas as pd
 from pycoingecko import CoinGeckoAPI
-from .types import PriceHistory, SymbolNotFoundError, CurrencyPreferenceNotFoundError
+from .types import (
+    PriceHistory,
+    SymbolNotFoundError,
+    CurrencyPreferenceNotFoundError,
+    RateLimitHitError,
+)
 
 
 def dataframify_price_list(prices: list) -> pd.DataFrame:
     """Turn price list returned by Coingecko API into a pricing dataframe in the form
     that we use.
     """
     df = pd.DataFrame(prices)
@@ -26,10 +31,13 @@
             interval="daily",
         )["prices"]
     except ValueError as exc:
         if "invalid vs_currency" in str(exc):
             raise CurrencyPreferenceNotFoundError(
                 source="coingecko", cur_pref=currency_preference
             ) from exc
+        if "429" in str(exc):
+            # (pycoingecko masks the underlying HTTPError.)
+            raise RateLimitHitError(source="coingecko") from exc
         raise SymbolNotFoundError(source="coingecko", query=query) from exc
 
     return PriceHistory(dataframify_price_list(res), currency_preference)
```

### Comparing `tessa-0.6.0/tessa/price/price.py` & `tessa-0.7.0/tessa/price/price.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,16 +1,19 @@
 """Retrieve price information."""
 
+from __future__ import annotations
 from functools import lru_cache, wraps
-from typing import Union
+from typing import Union, TYPE_CHECKING
 import pandas as pd
 from . import PriceHistory, PricePoint
-from .. import SourceType
 from .. import sources
 
+if TYPE_CHECKING:
+    from .. import SourceType
+
 
 def custom_cache_wrapper(func):
     """To preserve the function's signature _and_ give access to `cache_clear` etc."""
     cached_func = lru_cache(maxsize=None)(func)
     wrapped_func = wraps(func)(cached_func)
     return wrapped_func
```

### Comparing `tessa-0.6.0/tessa/price/yahoo.py` & `tessa-0.7.0/tessa/price/yahoo.py`

 * *Files identical despite different names*

### Comparing `tessa-0.6.0/tessa/search/__init__.py` & `tessa-0.7.0/tessa/search/__init__.py`

 * *Files identical despite different names*

### Comparing `tessa-0.6.0/tessa/search/coingecko.py` & `tessa-0.7.0/tessa/search/coingecko.py`

 * *Files identical despite different names*

### Comparing `tessa-0.6.0/tessa/search/search.py` & `tessa-0.7.0/tessa/search/search.py`

 * *Files identical despite different names*

### Comparing `tessa-0.6.0/tessa/search/search_result.py` & `tessa-0.7.0/tessa/search/search_result.py`

 * *Files identical despite different names*

### Comparing `tessa-0.6.0/tessa/search/yahoo.py` & `tessa-0.7.0/tessa/search/yahoo.py`

 * *Files identical despite different names*

### Comparing `tessa-0.6.0/tessa/sources/low_level_rate_limiter.py` & `tessa-0.7.0/tessa/sources/low_level_rate_limiter.py`

 * *Files identical despite different names*

### Comparing `tessa-0.6.0/tessa/sources/rate_limiter.py` & `tessa-0.7.0/tessa/sources/rate_limiter.py`

 * *Files 13% similar despite different names*

```diff
@@ -9,14 +9,15 @@
 from dataclasses import dataclass
 import datetime
 import time
 import pendulum
 
 
 VERY_LONG_AGO = pendulum.parse("1900")
+INITIAL_BACK_OFF_TIME = 10
 
 
 @dataclass
 class RateLimiter:
     """Encapsulates state and stats of a rate limiter object."""
 
     wait_seconds: float
@@ -27,20 +28,33 @@
 
     count_all_calls: int = 0
     """Number of total calls."""
 
     count_limited_calls: int = 0
     """Number of calls that triggered some waiting."""
 
+    back_off_time: int = INITIAL_BACK_OFF_TIME
+    """Number of seconds to wait after a rate limit hit."""
+
+    def reset_back_off(self):
+        """Reset back-off time to initial value."""
+        self.back_off_time = INITIAL_BACK_OFF_TIME
+
     def reset(self):
         """Reset state and stats."""
         self.last_call = VERY_LONG_AGO
         self.count_all_calls = self.count_limited_calls = 0
+        self.reset_back_off()
 
     def rate_limit(self):
         """Enforce the minimum wait time as specified in `wait_seconds`."""
         diff = (pendulum.now() - self.last_call).total_seconds()
         if diff < self.wait_seconds:
             time.sleep(self.wait_seconds - diff)
             self.count_limited_calls += 1
         self.last_call = pendulum.now()
         self.count_all_calls += 1
+
+    def back_off(self):
+        """Back off exponentially."""
+        time.sleep(self.back_off_time)
+        self.back_off_time *= 2
```

### Comparing `tessa-0.6.0/tessa/sources/sources.py` & `tessa-0.7.0/tessa/sources/sources.py`

 * *Files 4% similar despite different names*

```diff
@@ -3,14 +3,15 @@
 from __future__ import annotations
 from dataclasses import dataclass
 from typing import Callable, Generator, TYPE_CHECKING
 import warnings
 import requests
 from .sourcetype import SourceType
 from .rate_limiter import RateLimiter
+from ..price.types import RateLimitHitError
 
 if TYPE_CHECKING:
     from ..price import PriceHistory
 
 
 @dataclass
 class Source:
@@ -35,29 +36,37 @@
         retries.
         """
         max_tries = 100
         tries = 0
         while True:
             tries += 1
             try:
-                return self.get_price_history(query, currency_preference)
+                res = self.get_price_history(query, currency_preference)
+                self.rate_limiter.reset_back_off()
+                return res
             except requests.HTTPError as exc:
                 if exc.response.status_code not in [504, 503, 502]:
                     raise exc
                 if tries > max_tries:
                     raise ConnectionError(
                         f"Cannot access source, even after {max_tries} tries. "
                         "(Reraising from latest exception, there might have been "
                         "several.)"
                     ) from exc
                 warnings.warn(
                     f"Latest request raised for status code {exc.response.status_code}."
                     f" Retrying ({tries}/{max_tries}).",
                     RuntimeWarning,
                 )
+            except RateLimitHitError:
+                warnings.warn(
+                    "Rate limit hit (429). "
+                    f"Backing off {self.rate_limiter.back_off_time} seconds."
+                )
+                self.rate_limiter.back_off()
 
 
 def get_source(name: SourceType) -> Source:
     """Get a specific source."""
     # Prevent circular dependencies -- pylint: disable=import-outside-toplevel
     from .sources_directory import SOURCES_DIRECTORY
```

### Comparing `tessa-0.6.0/tessa/sources/sources_directory.py` & `tessa-0.7.0/tessa/sources/sources_directory.py`

 * *Files identical despite different names*

### Comparing `tessa-0.6.0/tessa/symbol/__init__.py` & `tessa-0.7.0/tessa/symbol/__init__.py`

 * *Files identical despite different names*

### Comparing `tessa-0.6.0/tessa/symbol/extended_symbol.py` & `tessa-0.7.0/tessa/symbol/extended_symbol.py`

 * *Files identical despite different names*

### Comparing `tessa-0.6.0/tessa/symbol/geo/countrynames.py` & `tessa-0.7.0/tessa/symbol/geo/countrynames.py`

 * *Files identical despite different names*

### Comparing `tessa-0.6.0/tessa/symbol/geo/jurisdiction2region.py` & `tessa-0.7.0/tessa/symbol/geo/jurisdiction2region.py`

 * *Files identical despite different names*

### Comparing `tessa-0.6.0/tessa/symbol/symbol.py` & `tessa-0.7.0/tessa/symbol/symbol.py`

 * *Files identical despite different names*

### Comparing `tessa-0.6.0/tessa/symbol/symbolcollection.py` & `tessa-0.7.0/tessa/symbol/symbolcollection.py`

 * *Files identical despite different names*

### Comparing `tessa-0.6.0/setup.py` & `tessa-0.7.0/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -11,24 +11,23 @@
 
 package_data = \
 {'': ['*']}
 
 install_requires = \
 ['PyYAML>=6',
  'beautifulsoup4>=4.11.1,<5.0.0',
- 'frozendict>=2.3',
  'matplotlib>=3.5',
  'pendulum>=2.1',
  'pycoingecko>=2.2',
  'seaborn>=0.11',
  'yfinance>=0.2.3,<0.3.0']
 
 setup_kwargs = {
     'name': 'tessa',
-    'version': '0.6.0',
+    'version': '0.7.0',
     'description': 'Find financial assets and get their price history without worrying about different APIs or rate limiting.',
     'long_description': '\n# tessa – simple, hassle-free access to price information of financial assets 📉🤓📈\n\ntessa is a Python library to help you **easily search asset identifiers** (e.g.,\ntickers) and **retrieve price information** for assets from different sources such as\nYahoo or Coingecko. It takes care of the different APIs, caching, rate limiting, and\nother hassles.\n\ntessa provides a **Symbol class that encapsulates nicely the methods relevant for a\nsymbol**. tessa also provides functionality to **manage collections of symbols**, store\nand load them, and extend their functionality.\n\nFinally, tessa makes sure to be nice to the sites being accessed and tries to **prevent\nusers from being blocked by 429 rate limiting errors** by 1) caching results upon\nretrieval and 2) keeping track of request timestamps and waiting appropriate amounts of\ntime if necessary.\n\n[→ Check out the full documentation. 📖](https://ymyke.github.io/tessa/tessa.html)\n\n\n## How to use\n\nHere\'s a longer example that quickly shows all aspects of the library. Refer to\nsubmodules [symbol](tessa/symbol.html), [search](tessa/search.html), and\n[price](tessa/price.html) for more information.\n\n- Imports:\n\n```python\nfrom tessa import Symbol, SymbolCollection, search\n```\n\n- Create a symbol for MSFT and access some functions:\n\n```python\ns1 = Symbol("MSFT")         # will use "yahoo" as the default source\ns1.price_latest()           # get latest price\n```\n\n- Create another symbol from a bloomberg ticker as it is used by Yahoo Finance:\n\n```python\ns2 = Symbol("SREN.SW")\ns2.price_point("2022-06-30")    # get price at specific point in time\n```\n\n- Create a symbol from the coingecko source with an id as it is used by coingecko:\n\n```python\ns3 = Symbol("bitcoin", source="coingecko")\ns3.price_graph()            # show price graph\n```\n\n- Search for a more crypto ticker on coingecko:\n\n```python\nres = search("GAME")        # search and print search result summary\nfiltered = res.filter(source="coingecko")  # filter results\nfiltered.p()                # print summary of filtered results\nfiltered.buckets[0].symbols # review the best bucket in the filtered results\ns4 = filtered.buckets[0].symbols[2]   # our symbol is the 3rd in that list\ns4.price_history()          # get entire history\n```\n\n- Build a collection of several symbols and use the collection to retrieve symbols:\n\n```python\nsc = SymbolCollection([s1, s2, s3, s4])\nsc.add(Symbol("AAPL"))      # add another one\nsc.find_one("SREN").price_graph()\n```\n\n- Store and load a symbol collection:\n\n```python\nsc.save_yaml("my_symbols.yaml")\nsc_new = SymbolCollection()\nsc_new.load_yaml("my_symbols.yaml")\n```\n\n- Use a different currency preference:\n\n```python\nsc.find_one("game").price_latest()  # will return price in USD\nSymbol.currency_preference = "CHF"\nsc.find_one("game").price_latest()  # will return price in CHF\n```\n\nNote that `currency_preference` will only have an effect with sources that support it.\nIt is supported for Coingecko but not for Yahoo. So you should always verify the\neffective currency you receive in the result.\n\n\n## Data sources\n\ntessa builds on [yfinance](https://pypi.org/project/yfinance/) and\n[pycoingecko](https://github.com/man-c/pycoingecko) and offers **a simplified and\nunified interface**. \n\nWhy these two sources? Yahoo Finance (via yfinance) is fast and offers an extensive\ndatabase that also contains many non-US markets. Coingecko (via pycoingecko) offers\ngreat access to crypto prices. While Yahoo Finance also offers crypto information,\npycoingecko has the advantage that you can have the prices quoted in many more currency\npreferences (a function that is also exposed via tessa).\n\nMore sources can be added in the future. Let me know in the\n[issues](https://github.com/ymyke/tessa/issues) of you have a particular request.\n\n\n## Main submodules\n\n- [symbol](tessa/symbol.html): working with symbols and symbol collections.\n- [search](tessa/search.html): searching the different sources.\n- [price](tessa/price.html): accessing price functions directly instead of via the\n  `Symbol` class.\n- [sources](tessa/sources.html): if you\'d like to add additional sources to the library.\n\n\n## How to install\n\n`pip install tessa`\n\n\n## Prerequisites\n\nSee `pyproject.toml`. Major prerequisites are the `yfinance` and `pycoingecko` packages\nto access finance information as well as the `beautifulsoup4` package to do some\nscraping for searching on Yahoo Finance.\n\n\n## Repository\n\nhttps://github.com/ymyke/tessa\n\n\n## Future Work\n\nThis is an initial version. There are a number of ideas on how to extend. Please leave\nyour suggestions and comments in the [Issues\nsection](https://github.com/ymyke/tessa/issues).\n\n\n## On terminology\n\nI\'m using symbol instead of ticker because a ticker is mainly used for stock on stock\nmarkets, whereas tessa is inteded to be used for any kind of financial assets, e.g. also\ncrypto.\n\n\n## Other noteworthy libraries\n\n- [strela](https://github.com/ymyke/strela): A python package for financial alerts.\n- [pypme](https://github.com/ymyke/pypme): A Python package for PME (Public Market\n  Equivalent) calculation.\n\n\n## On investpy as a data source\n\nTessa used to use the [investpy package](https://github.com/alvarobartt/investpy) as the\nmain source of information until mid 2022 until investing.com introduced Cloudflare,\nwhich broke access by investpy. 😖 It is currently unclear if investpy will be available\nagain in the future. [You can follow the developments in issue\n600.](https://github.com/alvarobartt/investpy/issues/600) The old tessa/investpy code is\nstill available in the [add-symbols-based-on-investpy\nbranch](https://github.com/ymyke/tessa/tree/add-symbols-based-on-investpy).\n',
     'author': 'ymyke',
     'author_email': 'None',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'https://github.com/ymyke/tessa',
```

### Comparing `tessa-0.6.0/PKG-INFO` & `tessa-0.7.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,23 +1,22 @@
 Metadata-Version: 2.1
 Name: tessa
-Version: 0.6.0
+Version: 0.7.0
 Summary: Find financial assets and get their price history without worrying about different APIs or rate limiting.
 Home-page: https://github.com/ymyke/tessa
 License: MIT
 Keywords: python,finance,investing,financial-analysis,investment-analysis,financial-data,coingecko,pycoingecko,yahoo,yahoo-finance,yfinance
 Author: ymyke
 Requires-Python: >=3.7.13,<3.10
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Requires-Dist: PyYAML (>=6)
 Requires-Dist: beautifulsoup4 (>=4.11.1,<5.0.0)
-Requires-Dist: frozendict (>=2.3)
 Requires-Dist: matplotlib (>=3.5)
 Requires-Dist: pendulum (>=2.1)
 Requires-Dist: pycoingecko (>=2.2)
 Requires-Dist: seaborn (>=0.11)
 Requires-Dist: yfinance (>=0.2.3,<0.3.0)
 Project-URL: Documentation, https://ymyke.github.io/tessa/tessa.html
 Project-URL: Repository, https://github.com/ymyke/tessa
```

