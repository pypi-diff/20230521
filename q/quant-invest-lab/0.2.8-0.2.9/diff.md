# Comparing `tmp/quant_invest_lab-0.2.8.tar.gz` & `tmp/quant_invest_lab-0.2.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "quant_invest_lab-0.2.8.tar", max compression
+gzip compressed data, was "quant_invest_lab-0.2.9.tar", max compression
```

## Comparing `quant_invest_lab-0.2.8.tar` & `quant_invest_lab-0.2.9.tar`

### file list

```diff
@@ -1,15 +1,15 @@
--rw-r--r--   0        0        0     5020 2023-05-21 20:12:27.924557 quant_invest_lab-0.2.8/README.md
--rw-r--r--   0        0        0     1727 2023-05-21 20:12:27.928557 quant_invest_lab-0.2.8/pyproject.toml
--rw-r--r--   0        0        0    29186 2023-05-21 20:12:27.928557 quant_invest_lab-0.2.8/quant_invest_lab/backtest.py
--rw-r--r--   0        0        0     1007 2023-05-21 20:12:27.928557 quant_invest_lab-0.2.8/quant_invest_lab/constants.py
--rw-r--r--   0        0        0    16533 2023-05-21 20:12:27.928557 quant_invest_lab-0.2.8/quant_invest_lab/data_provider.py
--rw-r--r--   0        0        0    26301 2023-05-21 20:12:27.928557 quant_invest_lab-0.2.8/quant_invest_lab/indicators.py
--rw-r--r--   0        0        0    11102 2023-05-21 20:12:27.928557 quant_invest_lab-0.2.8/quant_invest_lab/metrics.py
--rw-r--r--   0        0        0     7659 2023-05-21 20:12:27.928557 quant_invest_lab-0.2.8/quant_invest_lab/optimization.py
--rw-r--r--   0        0        0    18363 2023-05-21 20:12:27.928557 quant_invest_lab-0.2.8/quant_invest_lab/portfolio.py
--rw-r--r--   0        0        0     3577 2023-05-21 20:12:27.928557 quant_invest_lab-0.2.8/quant_invest_lab/screener.py
--rw-r--r--   0        0        0     7329 2023-05-21 20:12:27.928557 quant_invest_lab-0.2.8/quant_invest_lab/signal_processing.py
--rw-r--r--   0        0        0     7848 2023-05-21 20:12:27.928557 quant_invest_lab-0.2.8/quant_invest_lab/simulation.py
--rw-r--r--   0        0        0      178 2023-05-21 20:12:27.928557 quant_invest_lab-0.2.8/quant_invest_lab/types.py
--rw-r--r--   0        0        0     3403 2023-05-21 20:12:27.928557 quant_invest_lab-0.2.8/quant_invest_lab/utils.py
--rw-r--r--   0        0        0     7025 1970-01-01 00:00:00.000000 quant_invest_lab-0.2.8/PKG-INFO
+-rw-r--r--   0        0        0     5020 2023-05-21 20:36:12.658640 quant_invest_lab-0.2.9/README.md
+-rw-r--r--   0        0        0     1727 2023-05-21 20:36:12.662641 quant_invest_lab-0.2.9/pyproject.toml
+-rw-r--r--   0        0        0    29186 2023-05-21 20:36:12.662641 quant_invest_lab-0.2.9/quant_invest_lab/backtest.py
+-rw-r--r--   0        0        0     1007 2023-05-21 20:36:12.662641 quant_invest_lab-0.2.9/quant_invest_lab/constants.py
+-rw-r--r--   0        0        0    16498 2023-05-21 20:36:12.662641 quant_invest_lab-0.2.9/quant_invest_lab/data_provider.py
+-rw-r--r--   0        0        0    26301 2023-05-21 20:36:12.662641 quant_invest_lab-0.2.9/quant_invest_lab/indicators.py
+-rw-r--r--   0        0        0    11102 2023-05-21 20:36:12.662641 quant_invest_lab-0.2.9/quant_invest_lab/metrics.py
+-rw-r--r--   0        0        0     7659 2023-05-21 20:36:12.662641 quant_invest_lab-0.2.9/quant_invest_lab/optimization.py
+-rw-r--r--   0        0        0    18363 2023-05-21 20:36:12.662641 quant_invest_lab-0.2.9/quant_invest_lab/portfolio.py
+-rw-r--r--   0        0        0     3577 2023-05-21 20:36:12.662641 quant_invest_lab-0.2.9/quant_invest_lab/screener.py
+-rw-r--r--   0        0        0     7329 2023-05-21 20:36:12.662641 quant_invest_lab-0.2.9/quant_invest_lab/signal_processing.py
+-rw-r--r--   0        0        0     7848 2023-05-21 20:36:12.662641 quant_invest_lab-0.2.9/quant_invest_lab/simulation.py
+-rw-r--r--   0        0        0      178 2023-05-21 20:36:12.662641 quant_invest_lab-0.2.9/quant_invest_lab/types.py
+-rw-r--r--   0        0        0     3403 2023-05-21 20:36:12.662641 quant_invest_lab-0.2.9/quant_invest_lab/utils.py
+-rw-r--r--   0        0        0     7025 1970-01-01 00:00:00.000000 quant_invest_lab-0.2.9/PKG-INFO
```

### Comparing `quant_invest_lab-0.2.8/README.md` & `quant_invest_lab-0.2.9/README.md`

 * *Files identical despite different names*

### Comparing `quant_invest_lab-0.2.8/pyproject.toml` & `quant_invest_lab-0.2.9/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "quant-invest-lab"
-version = "0.2.8"
+version = "0.2.9"
 description = "Quant Invest Lab is a python package to help you to do some quantitative experiments, while trying to learn or build quantitative investment solutions. This project was initially my own set of functionnalities but I decided to build a package for that and sharing it as open source project."
 authors = ["BaptisteZloch <bzloch@hotmail.fr>"]
 maintainers = ["BaptisteZloch <bzloch@hotmail.fr>"]
 readme = "README.md"
 license = "MIT"
 repository = "https://github.com/BaptisteZloch/Quant-Invest-Lab"
 classifiers = [
```

### Comparing `quant_invest_lab-0.2.8/quant_invest_lab/backtest.py` & `quant_invest_lab-0.2.9/quant_invest_lab/backtest.py`

 * *Files identical despite different names*

### Comparing `quant_invest_lab-0.2.8/quant_invest_lab/constants.py` & `quant_invest_lab-0.2.9/quant_invest_lab/constants.py`

 * *Files identical despite different names*

### Comparing `quant_invest_lab-0.2.8/quant_invest_lab/data_provider.py` & `quant_invest_lab-0.2.9/quant_invest_lab/data_provider.py`

 * *Files 1% similar despite different names*

```diff
@@ -10,15 +10,14 @@
 from concurrent.futures import ThreadPoolExecutor, as_completed
 from tqdm import tqdm
 
 from quant_invest_lab.constants import TIMEFRAME_IN_S, TIMEFRAMES
 from quant_invest_lab.types import Timeframe
 
 
-@lru_cache(maxsize=32, typed=True)
 def build_multi_crypto_dataframe(
     symbols: set,
     drop_na: bool = False,
     column_to_keep: str = "Close",
     timeframe: Timeframe = "1day",
 ) -> pd.DataFrame:
     """Build a multi cryptocurrencies dataframe from a set of symbols. This dataframe will contain the closing price of each symbol or any other column specified in `column_to_keep`. This function is useful to build a dataframe for a multi cryptocurrencies portfolio.
```

### Comparing `quant_invest_lab-0.2.8/quant_invest_lab/indicators.py` & `quant_invest_lab-0.2.9/quant_invest_lab/indicators.py`

 * *Files identical despite different names*

### Comparing `quant_invest_lab-0.2.8/quant_invest_lab/metrics.py` & `quant_invest_lab-0.2.9/quant_invest_lab/metrics.py`

 * *Files identical despite different names*

### Comparing `quant_invest_lab-0.2.8/quant_invest_lab/optimization.py` & `quant_invest_lab-0.2.9/quant_invest_lab/optimization.py`

 * *Files identical despite different names*

### Comparing `quant_invest_lab-0.2.8/quant_invest_lab/portfolio.py` & `quant_invest_lab-0.2.9/quant_invest_lab/portfolio.py`

 * *Files identical despite different names*

### Comparing `quant_invest_lab-0.2.8/quant_invest_lab/screener.py` & `quant_invest_lab-0.2.9/quant_invest_lab/screener.py`

 * *Files identical despite different names*

### Comparing `quant_invest_lab-0.2.8/quant_invest_lab/signal_processing.py` & `quant_invest_lab-0.2.9/quant_invest_lab/signal_processing.py`

 * *Files identical despite different names*

### Comparing `quant_invest_lab-0.2.8/quant_invest_lab/simulation.py` & `quant_invest_lab-0.2.9/quant_invest_lab/simulation.py`

 * *Files identical despite different names*

### Comparing `quant_invest_lab-0.2.8/quant_invest_lab/utils.py` & `quant_invest_lab-0.2.9/quant_invest_lab/utils.py`

 * *Files identical despite different names*

### Comparing `quant_invest_lab-0.2.8/PKG-INFO` & `quant_invest_lab-0.2.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: quant-invest-lab
-Version: 0.2.8
+Version: 0.2.9
 Summary: Quant Invest Lab is a python package to help you to do some quantitative experiments, while trying to learn or build quantitative investment solutions. This project was initially my own set of functionnalities but I decided to build a package for that and sharing it as open source project.
 Home-page: https://github.com/BaptisteZloch/Quant-Invest-Lab
 License: MIT
 Keywords: trading,backtest,investments,portfolio,quantitative
 Author: BaptisteZloch
 Author-email: bzloch@hotmail.fr
 Maintainer: BaptisteZloch
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: quant-invest-lab Version: 0.2.8 Summary: Quant
+Metadata-Version: 2.1 Name: quant-invest-lab Version: 0.2.9 Summary: Quant
 Invest Lab is a python package to help you to do some quantitative experiments,
 while trying to learn or build quantitative investment solutions. This project
 was initially my own set of functionnalities but I decided to build a package
 for that and sharing it as open source project. Home-page: https://github.com/
 BaptisteZloch/Quant-Invest-Lab License: MIT Keywords:
 trading,backtest,investments,portfolio,quantitative Author: BaptisteZloch
 Author-email: bzloch@hotmail.fr Maintainer: BaptisteZloch Maintainer-email:
```

