# Comparing `tmp/pydisadm-1.2.5.tar.gz` & `tmp/pydisadm-1.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pydisadm-1.2.5.tar", max compression
+gzip compressed data, was "pydisadm-1.3.0.tar", max compression
```

## Comparing `pydisadm-1.2.5.tar` & `pydisadm-1.3.0.tar`

### file list

```diff
@@ -1,24 +1,24 @@
--rw-r--r--   0        0        0     2936 2023-05-21 03:30:25.999579 pydisadm-1.2.5/README.md
--rw-r--r--   0        0        0      111 2023-05-21 03:30:26.003579 pydisadm-1.2.5/pydisadm/__init__.py
--rw-r--r--   0        0        0     1130 2023-05-21 03:30:26.003579 pydisadm-1.2.5/pydisadm/__main__.py
--rw-r--r--   0        0        0     1540 2023-05-21 03:30:26.003579 pydisadm-1.2.5/pydisadm/bot/adm_bot.py
--rw-r--r--   0        0        0     7238 2023-05-21 03:30:26.003579 pydisadm-1.2.5/pydisadm/bot/adm_cog.py
--rw-r--r--   0        0        0     2649 2023-05-21 03:30:26.003579 pydisadm-1.2.5/pydisadm/bot/update_adm_modal.py
--rw-r--r--   0        0        0      702 2023-05-21 03:30:26.003579 pydisadm-1.2.5/pydisadm/bot/utils.py
--rw-r--r--   0        0        0     1413 2023-05-21 03:30:26.003579 pydisadm-1.2.5/pydisadm/configuration.py
--rw-r--r--   0        0        0     8044 2023-05-21 03:30:26.003579 pydisadm-1.2.5/pydisadm/controller/adm_controller.py
--rw-r--r--   0        0        0        0 2023-05-21 03:30:26.003579 pydisadm-1.2.5/pydisadm/data/__init__.py
--rw-r--r--   0        0        0   368313 2023-05-21 03:30:26.003579 pydisadm-1.2.5/pydisadm/data/mapConstellations.csv
--rw-r--r--   0        0        0    34613 2023-05-21 03:30:26.003579 pydisadm-1.2.5/pydisadm/data/mapRegions.csv
--rw-r--r--   0        0        0  3277768 2023-05-21 03:30:26.019579 pydisadm-1.2.5/pydisadm/data/mapSolarSystems.csv
--rw-r--r--   0        0        0      607 2023-05-21 03:30:26.019579 pydisadm-1.2.5/pydisadm/loader/datasets.py
--rw-r--r--   0        0        0     1085 2023-05-21 03:30:26.019579 pydisadm-1.2.5/pydisadm/loader/static_data.py
--rw-r--r--   0        0        0     1294 2023-05-21 03:30:26.023579 pydisadm-1.2.5/pydisadm/runnable/runnable_refresh.py
--rw-r--r--   0        0        0     3814 2023-05-21 03:30:26.023579 pydisadm-1.2.5/pydisadm/services/database.py
--rw-r--r--   0        0        0     1543 2023-05-21 03:30:26.023579 pydisadm-1.2.5/pydisadm/services/esi.py
--rw-r--r--   0        0        0      484 2023-05-21 03:30:26.023579 pydisadm-1.2.5/pydisadm/utils/adm_utils.py
--rw-r--r--   0        0        0      472 2023-05-21 03:30:26.023579 pydisadm-1.2.5/pydisadm/utils/datetime_utils.py
--rw-r--r--   0        0        0      623 2023-05-21 03:30:26.023579 pydisadm-1.2.5/pydisadm/utils/plot_utils.py
--rw-r--r--   0        0        0      193 2023-05-21 03:30:26.023579 pydisadm-1.2.5/pydisadm/utils/thread_utils.py
--rw-r--r--   0        0        0      953 2023-05-21 03:30:53.587786 pydisadm-1.2.5/pyproject.toml
--rw-r--r--   0        0        0     3842 1970-01-01 00:00:00.000000 pydisadm-1.2.5/PKG-INFO
+-rw-r--r--   0        0        0     2936 2023-05-21 16:07:32.973435 pydisadm-1.3.0/README.md
+-rw-r--r--   0        0        0      111 2023-05-21 16:07:32.977435 pydisadm-1.3.0/pydisadm/__init__.py
+-rw-r--r--   0        0        0     1130 2023-05-21 16:07:32.977435 pydisadm-1.3.0/pydisadm/__main__.py
+-rw-r--r--   0        0        0     1540 2023-05-21 16:07:32.977435 pydisadm-1.3.0/pydisadm/bot/adm_bot.py
+-rw-r--r--   0        0        0     7714 2023-05-21 16:07:32.977435 pydisadm-1.3.0/pydisadm/bot/adm_cog.py
+-rw-r--r--   0        0        0     2649 2023-05-21 16:07:32.977435 pydisadm-1.3.0/pydisadm/bot/update_adm_modal.py
+-rw-r--r--   0        0        0      702 2023-05-21 16:07:32.977435 pydisadm-1.3.0/pydisadm/bot/utils.py
+-rw-r--r--   0        0        0     1535 2023-05-21 16:07:32.977435 pydisadm-1.3.0/pydisadm/configuration.py
+-rw-r--r--   0        0        0     8044 2023-05-21 16:07:32.977435 pydisadm-1.3.0/pydisadm/controller/adm_controller.py
+-rw-r--r--   0        0        0        0 2023-05-21 16:07:32.977435 pydisadm-1.3.0/pydisadm/data/__init__.py
+-rw-r--r--   0        0        0   368313 2023-05-21 16:07:32.977435 pydisadm-1.3.0/pydisadm/data/mapConstellations.csv
+-rw-r--r--   0        0        0    34613 2023-05-21 16:07:32.977435 pydisadm-1.3.0/pydisadm/data/mapRegions.csv
+-rw-r--r--   0        0        0  3277768 2023-05-21 16:07:32.993436 pydisadm-1.3.0/pydisadm/data/mapSolarSystems.csv
+-rw-r--r--   0        0        0      607 2023-05-21 16:07:32.993436 pydisadm-1.3.0/pydisadm/loader/datasets.py
+-rw-r--r--   0        0        0     1085 2023-05-21 16:07:32.993436 pydisadm-1.3.0/pydisadm/loader/static_data.py
+-rw-r--r--   0        0        0     1294 2023-05-21 16:07:32.993436 pydisadm-1.3.0/pydisadm/runnable/runnable_refresh.py
+-rw-r--r--   0        0        0     3814 2023-05-21 16:07:32.993436 pydisadm-1.3.0/pydisadm/services/database.py
+-rw-r--r--   0        0        0     1543 2023-05-21 16:07:32.993436 pydisadm-1.3.0/pydisadm/services/esi.py
+-rw-r--r--   0        0        0      484 2023-05-21 16:07:32.993436 pydisadm-1.3.0/pydisadm/utils/adm_utils.py
+-rw-r--r--   0        0        0      472 2023-05-21 16:07:32.993436 pydisadm-1.3.0/pydisadm/utils/datetime_utils.py
+-rw-r--r--   0        0        0      623 2023-05-21 16:07:32.993436 pydisadm-1.3.0/pydisadm/utils/plot_utils.py
+-rw-r--r--   0        0        0      193 2023-05-21 16:07:32.993436 pydisadm-1.3.0/pydisadm/utils/thread_utils.py
+-rw-r--r--   0        0        0      953 2023-05-21 16:08:05.201922 pydisadm-1.3.0/pyproject.toml
+-rw-r--r--   0        0        0     3842 1970-01-01 00:00:00.000000 pydisadm-1.3.0/PKG-INFO
```

### Comparing `pydisadm-1.2.5/README.md` & `pydisadm-1.3.0/README.md`

 * *Files identical despite different names*

### Comparing `pydisadm-1.2.5/pydisadm/__main__.py` & `pydisadm-1.3.0/pydisadm/__main__.py`

 * *Files identical despite different names*

### Comparing `pydisadm-1.2.5/pydisadm/bot/adm_bot.py` & `pydisadm-1.3.0/pydisadm/bot/adm_bot.py`

 * *Files identical despite different names*

### Comparing `pydisadm-1.2.5/pydisadm/bot/adm_cog.py` & `pydisadm-1.3.0/pydisadm/bot/adm_cog.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 """Cog providing ADM related commands"""
 
 import discord
 from discord.ext import commands
 from discord import app_commands
+from discord.ext.commands import Context
 import pydisadm
 from pydisadm.bot.update_adm_modal import UpdateAdmModal
 
 from pydisadm.bot.utils import check_allowed_channel, text_channels_with_send_permission
 from pydisadm.configuration import Configuration
 from pydisadm.controller.adm_controller import AdmController
 from pydisadm.utils.datetime_utils import convert_to_local_timestamp
@@ -135,23 +136,34 @@
         await interaction.response.send_modal(UpdateAdmModal(system_name, self.controller))
 
     @commands.Cog.listener()
     async def on_ready(self):
         """cog on_ready event callback"""
         channels = text_channels_with_send_permission(self.bot)
 
-        await self.bot.tree.sync()
-
         valid_channels = [
             channel for channel in channels if channel.name == self.configuration.discord_channel]
 
         embed = discord.Embed(title=f'🦀 ADM Bot v{pydisadm.__version__}')
         embed.add_field(name='Summary', value='/adm summary')
         embed.add_field(name='CSV', value='/adm csv')
         embed.add_field(name='History', value='/adm history <name>')
         embed.add_field(name='Update', value='/adm update <system>')
         embed.add_field(name='Recommend', value='/adm recommend')
         embed.add_field(name='Refresh', value='/adm refresh')
         embed.add_field(name='Source', value='[github](https://github.com/agelito/adm-bot)')
 
         for channel in valid_channels:
             await channel.send(embed=embed)
+
+    @commands.command(pass_context=True)
+    async def adm_sync_commands(self, ctx: Context):
+        """synchronize slash commands"""
+
+        if self.configuration.discord_guild_id:
+            guild = discord.Object(id=self.configuration.discord_guild_id)
+            self.bot.tree.copy_global_to(guild=guild)
+            await self.bot.tree.sync(guild=guild)
+        else:
+            await self.bot.tree.sync()
+
+        await ctx.send('Synchronized bot commands.')
```

### Comparing `pydisadm-1.2.5/pydisadm/bot/update_adm_modal.py` & `pydisadm-1.3.0/pydisadm/bot/update_adm_modal.py`

 * *Files identical despite different names*

### Comparing `pydisadm-1.2.5/pydisadm/bot/utils.py` & `pydisadm-1.3.0/pydisadm/bot/utils.py`

 * *Files identical despite different names*

### Comparing `pydisadm-1.2.5/pydisadm/configuration.py` & `pydisadm-1.3.0/pydisadm/configuration.py`

 * *Files 10% similar despite different names*

```diff
@@ -3,14 +3,15 @@
 class Configuration:
     """App configuration variables"""
 
     def __init__(self):
         self.discord_token = os.getenv('DISCORD_TOKEN')
         self.discord_channel = os.getenv('DISCORD_CHANNEL')
         self.discord_app_id = os.getenv('DISCORD_APP_ID')
+        self.discord_guild_id = os.getenv('DISCORD_GUILD_ID')
 
         alliance_id = os.getenv('ALLIANCE_ID')
 
         db_keep_adm_days = os.getenv('DB_KEEP_ADM_DAYS', '7')
         if db_keep_adm_days is not None:
             try:
                 db_keep_adm_days = int(db_keep_adm_days)
@@ -32,9 +33,10 @@
         self.alliance_id = alliance_id
 
     def __str__(self):
         return (f'{self.__class__.__name__}' +
             f'(discord_token={self.discord_token}, ' +
             f'discord_channel={self.discord_channel}, ' +
             f'discord_app_id={self.discord_app_id}, ' +
+            f'discord_guild_id={self.discord_guild_id}, ' +
             f'alliance_id={self.alliance_id} ' +
             f'db_keep_adm_days={self.db_keep_adm_days})')
```

### Comparing `pydisadm-1.2.5/pydisadm/controller/adm_controller.py` & `pydisadm-1.3.0/pydisadm/controller/adm_controller.py`

 * *Files identical despite different names*

### Comparing `pydisadm-1.2.5/pydisadm/data/mapConstellations.csv` & `pydisadm-1.3.0/pydisadm/data/mapConstellations.csv`

 * *Files identical despite different names*

### Comparing `pydisadm-1.2.5/pydisadm/data/mapRegions.csv` & `pydisadm-1.3.0/pydisadm/data/mapRegions.csv`

 * *Files identical despite different names*

### Comparing `pydisadm-1.2.5/pydisadm/data/mapSolarSystems.csv` & `pydisadm-1.3.0/pydisadm/data/mapSolarSystems.csv`

 * *Files identical despite different names*

### Comparing `pydisadm-1.2.5/pydisadm/loader/datasets.py` & `pydisadm-1.3.0/pydisadm/loader/datasets.py`

 * *Files identical despite different names*

### Comparing `pydisadm-1.2.5/pydisadm/loader/static_data.py` & `pydisadm-1.3.0/pydisadm/loader/static_data.py`

 * *Files identical despite different names*

### Comparing `pydisadm-1.2.5/pydisadm/runnable/runnable_refresh.py` & `pydisadm-1.3.0/pydisadm/runnable/runnable_refresh.py`

 * *Files identical despite different names*

### Comparing `pydisadm-1.2.5/pydisadm/services/database.py` & `pydisadm-1.3.0/pydisadm/services/database.py`

 * *Files identical despite different names*

### Comparing `pydisadm-1.2.5/pydisadm/services/esi.py` & `pydisadm-1.3.0/pydisadm/services/esi.py`

 * *Files identical despite different names*

### Comparing `pydisadm-1.2.5/pydisadm/utils/plot_utils.py` & `pydisadm-1.3.0/pydisadm/utils/plot_utils.py`

 * *Files identical despite different names*

### Comparing `pydisadm-1.2.5/pyproject.toml` & `pydisadm-1.3.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "pydisadm"
-version = "1.2.5"
+version = "1.3.0"
 description = "A Discord bot providing ADM summaries."
 repository = "https://github.com/agelito/adm-bot"
 authors = ["Axel Wettervik"]
 license = "MIT"
 readme = "README.md"
 include = ["data/*.csv"]
```

### Comparing `pydisadm-1.2.5/PKG-INFO` & `pydisadm-1.3.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pydisadm
-Version: 1.2.5
+Version: 1.3.0
 Summary: A Discord bot providing ADM summaries.
 Home-page: https://github.com/agelito/adm-bot
 License: MIT
 Author: Axel Wettervik
 Requires-Python: >=3.8,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

