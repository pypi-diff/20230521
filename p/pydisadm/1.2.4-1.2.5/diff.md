# Comparing `tmp/pydisadm-1.2.4.tar.gz` & `tmp/pydisadm-1.2.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pydisadm-1.2.4.tar", max compression
+gzip compressed data, was "pydisadm-1.2.5.tar", max compression
```

## Comparing `pydisadm-1.2.4.tar` & `pydisadm-1.2.5.tar`

### file list

```diff
@@ -1,24 +1,24 @@
--rw-r--r--   0        0        0     2936 2023-05-20 03:37:51.006777 pydisadm-1.2.4/README.md
--rw-r--r--   0        0        0      111 2023-05-20 03:37:51.006777 pydisadm-1.2.4/pydisadm/__init__.py
--rw-r--r--   0        0        0     1130 2023-05-20 03:37:51.006777 pydisadm-1.2.4/pydisadm/__main__.py
--rw-r--r--   0        0        0     1541 2023-05-20 03:37:51.006777 pydisadm-1.2.4/pydisadm/bot/adm_bot.py
--rw-r--r--   0        0        0     7238 2023-05-20 03:37:51.006777 pydisadm-1.2.4/pydisadm/bot/adm_cog.py
--rw-r--r--   0        0        0     2649 2023-05-20 03:37:51.006777 pydisadm-1.2.4/pydisadm/bot/update_adm_modal.py
--rw-r--r--   0        0        0      702 2023-05-20 03:37:51.006777 pydisadm-1.2.4/pydisadm/bot/utils.py
--rw-r--r--   0        0        0     1413 2023-05-20 03:37:51.006777 pydisadm-1.2.4/pydisadm/configuration.py
--rw-r--r--   0        0        0     8044 2023-05-20 03:37:51.006777 pydisadm-1.2.4/pydisadm/controller/adm_controller.py
--rw-r--r--   0        0        0        0 2023-05-20 03:37:51.006777 pydisadm-1.2.4/pydisadm/data/__init__.py
--rw-r--r--   0        0        0   368313 2023-05-20 03:37:51.010777 pydisadm-1.2.4/pydisadm/data/mapConstellations.csv
--rw-r--r--   0        0        0    34613 2023-05-20 03:37:51.010777 pydisadm-1.2.4/pydisadm/data/mapRegions.csv
--rw-r--r--   0        0        0  3277768 2023-05-20 03:37:51.026777 pydisadm-1.2.4/pydisadm/data/mapSolarSystems.csv
--rw-r--r--   0        0        0      607 2023-05-20 03:37:51.026777 pydisadm-1.2.4/pydisadm/loader/datasets.py
--rw-r--r--   0        0        0     1085 2023-05-20 03:37:51.026777 pydisadm-1.2.4/pydisadm/loader/static_data.py
--rw-r--r--   0        0        0     1294 2023-05-20 03:37:51.026777 pydisadm-1.2.4/pydisadm/runnable/runnable_refresh.py
--rw-r--r--   0        0        0     3814 2023-05-20 03:37:51.026777 pydisadm-1.2.4/pydisadm/services/database.py
--rw-r--r--   0        0        0     1543 2023-05-20 03:37:51.026777 pydisadm-1.2.4/pydisadm/services/esi.py
--rw-r--r--   0        0        0      484 2023-05-20 03:37:51.026777 pydisadm-1.2.4/pydisadm/utils/adm_utils.py
--rw-r--r--   0        0        0      472 2023-05-20 03:37:51.026777 pydisadm-1.2.4/pydisadm/utils/datetime_utils.py
--rw-r--r--   0        0        0      623 2023-05-20 03:37:51.026777 pydisadm-1.2.4/pydisadm/utils/plot_utils.py
--rw-r--r--   0        0        0      193 2023-05-20 03:37:51.026777 pydisadm-1.2.4/pydisadm/utils/thread_utils.py
--rw-r--r--   0        0        0      953 2023-05-20 03:38:23.246999 pydisadm-1.2.4/pyproject.toml
--rw-r--r--   0        0        0     3842 1970-01-01 00:00:00.000000 pydisadm-1.2.4/PKG-INFO
+-rw-r--r--   0        0        0     2936 2023-05-21 03:30:25.999579 pydisadm-1.2.5/README.md
+-rw-r--r--   0        0        0      111 2023-05-21 03:30:26.003579 pydisadm-1.2.5/pydisadm/__init__.py
+-rw-r--r--   0        0        0     1130 2023-05-21 03:30:26.003579 pydisadm-1.2.5/pydisadm/__main__.py
+-rw-r--r--   0        0        0     1540 2023-05-21 03:30:26.003579 pydisadm-1.2.5/pydisadm/bot/adm_bot.py
+-rw-r--r--   0        0        0     7238 2023-05-21 03:30:26.003579 pydisadm-1.2.5/pydisadm/bot/adm_cog.py
+-rw-r--r--   0        0        0     2649 2023-05-21 03:30:26.003579 pydisadm-1.2.5/pydisadm/bot/update_adm_modal.py
+-rw-r--r--   0        0        0      702 2023-05-21 03:30:26.003579 pydisadm-1.2.5/pydisadm/bot/utils.py
+-rw-r--r--   0        0        0     1413 2023-05-21 03:30:26.003579 pydisadm-1.2.5/pydisadm/configuration.py
+-rw-r--r--   0        0        0     8044 2023-05-21 03:30:26.003579 pydisadm-1.2.5/pydisadm/controller/adm_controller.py
+-rw-r--r--   0        0        0        0 2023-05-21 03:30:26.003579 pydisadm-1.2.5/pydisadm/data/__init__.py
+-rw-r--r--   0        0        0   368313 2023-05-21 03:30:26.003579 pydisadm-1.2.5/pydisadm/data/mapConstellations.csv
+-rw-r--r--   0        0        0    34613 2023-05-21 03:30:26.003579 pydisadm-1.2.5/pydisadm/data/mapRegions.csv
+-rw-r--r--   0        0        0  3277768 2023-05-21 03:30:26.019579 pydisadm-1.2.5/pydisadm/data/mapSolarSystems.csv
+-rw-r--r--   0        0        0      607 2023-05-21 03:30:26.019579 pydisadm-1.2.5/pydisadm/loader/datasets.py
+-rw-r--r--   0        0        0     1085 2023-05-21 03:30:26.019579 pydisadm-1.2.5/pydisadm/loader/static_data.py
+-rw-r--r--   0        0        0     1294 2023-05-21 03:30:26.023579 pydisadm-1.2.5/pydisadm/runnable/runnable_refresh.py
+-rw-r--r--   0        0        0     3814 2023-05-21 03:30:26.023579 pydisadm-1.2.5/pydisadm/services/database.py
+-rw-r--r--   0        0        0     1543 2023-05-21 03:30:26.023579 pydisadm-1.2.5/pydisadm/services/esi.py
+-rw-r--r--   0        0        0      484 2023-05-21 03:30:26.023579 pydisadm-1.2.5/pydisadm/utils/adm_utils.py
+-rw-r--r--   0        0        0      472 2023-05-21 03:30:26.023579 pydisadm-1.2.5/pydisadm/utils/datetime_utils.py
+-rw-r--r--   0        0        0      623 2023-05-21 03:30:26.023579 pydisadm-1.2.5/pydisadm/utils/plot_utils.py
+-rw-r--r--   0        0        0      193 2023-05-21 03:30:26.023579 pydisadm-1.2.5/pydisadm/utils/thread_utils.py
+-rw-r--r--   0        0        0      953 2023-05-21 03:30:53.587786 pydisadm-1.2.5/pyproject.toml
+-rw-r--r--   0        0        0     3842 1970-01-01 00:00:00.000000 pydisadm-1.2.5/PKG-INFO
```

### Comparing `pydisadm-1.2.4/README.md` & `pydisadm-1.2.5/README.md`

 * *Files identical despite different names*

### Comparing `pydisadm-1.2.4/pydisadm/__main__.py` & `pydisadm-1.2.5/pydisadm/__main__.py`

 * *Files identical despite different names*

### Comparing `pydisadm-1.2.4/pydisadm/bot/adm_bot.py` & `pydisadm-1.2.5/pydisadm/bot/adm_bot.py`

 * *Files 2% similar despite different names*

```diff
@@ -20,15 +20,15 @@
     def __init__(self, configuration: Configuration, controller: AdmController):
         self.configuration = configuration
         self.controller = controller
 
         intents = create_intents()
         self.bot = commands.Bot(
             application_id=configuration.discord_app_id,
-            command_prefix=None,
+            command_prefix='!',
             intents=intents,
             help_command=None
         )
 
     async def setup_cogs_async(self):
         """Asynchronously setup cogs"""
         await self.bot.add_cog(Adm(self.bot, self.configuration, self.controller))
```

### Comparing `pydisadm-1.2.4/pydisadm/bot/adm_cog.py` & `pydisadm-1.2.5/pydisadm/bot/adm_cog.py`

 * *Files identical despite different names*

### Comparing `pydisadm-1.2.4/pydisadm/bot/update_adm_modal.py` & `pydisadm-1.2.5/pydisadm/bot/update_adm_modal.py`

 * *Files identical despite different names*

### Comparing `pydisadm-1.2.4/pydisadm/bot/utils.py` & `pydisadm-1.2.5/pydisadm/bot/utils.py`

 * *Files identical despite different names*

### Comparing `pydisadm-1.2.4/pydisadm/configuration.py` & `pydisadm-1.2.5/pydisadm/configuration.py`

 * *Files identical despite different names*

### Comparing `pydisadm-1.2.4/pydisadm/controller/adm_controller.py` & `pydisadm-1.2.5/pydisadm/controller/adm_controller.py`

 * *Files identical despite different names*

### Comparing `pydisadm-1.2.4/pydisadm/data/mapConstellations.csv` & `pydisadm-1.2.5/pydisadm/data/mapConstellations.csv`

 * *Files identical despite different names*

### Comparing `pydisadm-1.2.4/pydisadm/data/mapRegions.csv` & `pydisadm-1.2.5/pydisadm/data/mapRegions.csv`

 * *Files identical despite different names*

### Comparing `pydisadm-1.2.4/pydisadm/data/mapSolarSystems.csv` & `pydisadm-1.2.5/pydisadm/data/mapSolarSystems.csv`

 * *Files identical despite different names*

### Comparing `pydisadm-1.2.4/pydisadm/loader/datasets.py` & `pydisadm-1.2.5/pydisadm/loader/datasets.py`

 * *Files identical despite different names*

### Comparing `pydisadm-1.2.4/pydisadm/loader/static_data.py` & `pydisadm-1.2.5/pydisadm/loader/static_data.py`

 * *Files identical despite different names*

### Comparing `pydisadm-1.2.4/pydisadm/runnable/runnable_refresh.py` & `pydisadm-1.2.5/pydisadm/runnable/runnable_refresh.py`

 * *Files identical despite different names*

### Comparing `pydisadm-1.2.4/pydisadm/services/database.py` & `pydisadm-1.2.5/pydisadm/services/database.py`

 * *Files identical despite different names*

### Comparing `pydisadm-1.2.4/pydisadm/services/esi.py` & `pydisadm-1.2.5/pydisadm/services/esi.py`

 * *Files identical despite different names*

### Comparing `pydisadm-1.2.4/pydisadm/utils/plot_utils.py` & `pydisadm-1.2.5/pydisadm/utils/plot_utils.py`

 * *Files identical despite different names*

### Comparing `pydisadm-1.2.4/pyproject.toml` & `pydisadm-1.2.5/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "pydisadm"
-version = "1.2.4"
+version = "1.2.5"
 description = "A Discord bot providing ADM summaries."
 repository = "https://github.com/agelito/adm-bot"
 authors = ["Axel Wettervik"]
 license = "MIT"
 readme = "README.md"
 include = ["data/*.csv"]
```

### Comparing `pydisadm-1.2.4/PKG-INFO` & `pydisadm-1.2.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pydisadm
-Version: 1.2.4
+Version: 1.2.5
 Summary: A Discord bot providing ADM summaries.
 Home-page: https://github.com/agelito/adm-bot
 License: MIT
 Author: Axel Wettervik
 Requires-Python: >=3.8,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

