# Comparing `tmp/arkprts-0.1.1.tar.gz` & `tmp/arkprts-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "arkprts-0.1.1.tar", last modified: Sat May 20 18:07:04 2023, max compression
+gzip compressed data, was "arkprts-0.1.2.tar", last modified: Sun May 21 14:32:30 2023, max compression
```

## Comparing `arkprts-0.1.1.tar` & `arkprts-0.1.2.tar`

### file list

```diff
@@ -1,28 +1,28 @@
-drwxrwxrwx   0        0        0        0 2023-05-20 18:07:04.122009 arkprts-0.1.1/
--rw-rw-rw-   0        0        0    35823 2023-04-30 21:01:40.000000 arkprts-0.1.1/LICENSE
--rw-rw-rw-   0        0        0     1748 2023-05-20 18:07:04.036059 arkprts-0.1.1/PKG-INFO
--rw-rw-rw-   0        0        0     1462 2023-05-19 17:49:21.000000 arkprts-0.1.1/README.md
-drwxrwxrwx   0        0        0        0 2023-05-20 18:07:03.770616 arkprts-0.1.1/arkprts/
--rw-rw-rw-   0        0        0      111 2023-05-19 17:48:39.000000 arkprts-0.1.1/arkprts/__init__.py
--rw-rw-rw-   0        0        0     1922 2023-05-19 18:21:49.000000 arkprts-0.1.1/arkprts/__main__.py
--rw-rw-rw-   0        0        0    12390 2023-05-19 19:14:56.000000 arkprts-0.1.1/arkprts/client.py
--rw-rw-rw-   0        0        0     1356 2023-05-07 16:47:55.000000 arkprts-0.1.1/arkprts/errors.py
--rw-rw-rw-   0        0        0     6033 2023-05-19 18:45:31.000000 arkprts-0.1.1/arkprts/gamedata.py
-drwxrwxrwx   0        0        0        0 2023-05-20 18:07:04.023065 arkprts-0.1.1/arkprts/models/
--rw-rw-rw-   0        0        0       75 2023-05-07 15:46:44.000000 arkprts-0.1.1/arkprts/models/__init__.py
--rw-rw-rw-   0        0        0     2734 2023-05-20 17:40:39.000000 arkprts-0.1.1/arkprts/models/base.py
--rw-rw-rw-   0        0        0     8940 2023-05-20 17:53:56.000000 arkprts-0.1.1/arkprts/models/data.py
--rw-rw-rw-   0        0        0     6953 2023-05-20 17:54:10.000000 arkprts-0.1.1/arkprts/models/social.py
--rw-rw-rw-   0        0        0        0 2023-04-30 21:01:40.000000 arkprts-0.1.1/arkprts/py.typed
-drwxrwxrwx   0        0        0        0 2023-05-20 18:07:04.003078 arkprts-0.1.1/arkprts.egg-info/
--rw-rw-rw-   0        0        0     1748 2023-05-20 18:07:03.000000 arkprts-0.1.1/arkprts.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      450 2023-05-20 18:07:03.000000 arkprts-0.1.1/arkprts.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-20 18:07:03.000000 arkprts-0.1.1/arkprts.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       41 2023-05-20 18:07:03.000000 arkprts-0.1.1/arkprts.egg-info/requires.txt
--rw-rw-rw-   0        0        0        8 2023-05-20 18:07:03.000000 arkprts-0.1.1/arkprts.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     2569 2023-05-19 18:44:52.000000 arkprts-0.1.1/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-05-20 18:07:04.122009 arkprts-0.1.1/setup.cfg
--rw-rw-rw-   0        0        0      623 2023-05-20 18:05:29.000000 arkprts-0.1.1/setup.py
-drwxrwxrwx   0        0        0        0 2023-05-20 18:07:04.032063 arkprts-0.1.1/tests/
--rw-rw-rw-   0        0        0      282 2023-05-01 00:20:38.000000 arkprts-0.1.1/tests/test_config.py
--rw-rw-rw-   0        0        0      357 2023-05-19 18:47:11.000000 arkprts-0.1.1/tests/test_gamedata.py
+drwxrwxrwx   0        0        0        0 2023-05-21 14:32:30.656536 arkprts-0.1.2/
+-rw-rw-rw-   0        0        0    35823 2023-04-30 21:01:40.000000 arkprts-0.1.2/LICENSE
+-rw-rw-rw-   0        0        0     1748 2023-05-21 14:32:30.653533 arkprts-0.1.2/PKG-INFO
+-rw-rw-rw-   0        0        0     1462 2023-05-19 17:49:21.000000 arkprts-0.1.2/README.md
+drwxrwxrwx   0        0        0        0 2023-05-21 14:32:30.575577 arkprts-0.1.2/arkprts/
+-rw-rw-rw-   0        0        0      111 2023-05-19 17:48:39.000000 arkprts-0.1.2/arkprts/__init__.py
+-rw-rw-rw-   0        0        0     1922 2023-05-19 18:21:49.000000 arkprts-0.1.2/arkprts/__main__.py
+-rw-rw-rw-   0        0        0    12390 2023-05-19 19:14:56.000000 arkprts-0.1.2/arkprts/client.py
+-rw-rw-rw-   0        0        0     1356 2023-05-07 16:47:55.000000 arkprts-0.1.2/arkprts/errors.py
+-rw-rw-rw-   0        0        0     6605 2023-05-21 14:06:41.000000 arkprts-0.1.2/arkprts/gamedata.py
+drwxrwxrwx   0        0        0        0 2023-05-21 14:32:30.641540 arkprts-0.1.2/arkprts/models/
+-rw-rw-rw-   0        0        0       75 2023-05-07 15:46:44.000000 arkprts-0.1.2/arkprts/models/__init__.py
+-rw-rw-rw-   0        0        0     3012 2023-05-21 13:53:11.000000 arkprts-0.1.2/arkprts/models/base.py
+-rw-rw-rw-   0        0        0     9871 2023-05-21 13:56:15.000000 arkprts-0.1.2/arkprts/models/data.py
+-rw-rw-rw-   0        0        0     6953 2023-05-21 13:50:03.000000 arkprts-0.1.2/arkprts/models/social.py
+-rw-rw-rw-   0        0        0        0 2023-04-30 21:01:40.000000 arkprts-0.1.2/arkprts/py.typed
+drwxrwxrwx   0        0        0        0 2023-05-21 14:32:30.624552 arkprts-0.1.2/arkprts.egg-info/
+-rw-rw-rw-   0        0        0     1748 2023-05-21 14:32:30.000000 arkprts-0.1.2/arkprts.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      450 2023-05-21 14:32:30.000000 arkprts-0.1.2/arkprts.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-21 14:32:30.000000 arkprts-0.1.2/arkprts.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       41 2023-05-21 14:32:30.000000 arkprts-0.1.2/arkprts.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        8 2023-05-21 14:32:30.000000 arkprts-0.1.2/arkprts.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     2569 2023-05-19 18:44:52.000000 arkprts-0.1.2/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-05-21 14:32:30.657536 arkprts-0.1.2/setup.cfg
+-rw-rw-rw-   0        0        0      623 2023-05-21 14:02:40.000000 arkprts-0.1.2/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-21 14:32:30.649534 arkprts-0.1.2/tests/
+-rw-rw-rw-   0        0        0      282 2023-05-01 00:20:38.000000 arkprts-0.1.2/tests/test_config.py
+-rw-rw-rw-   0        0        0      357 2023-05-19 18:47:11.000000 arkprts-0.1.2/tests/test_gamedata.py
```

### Comparing `arkprts-0.1.1/LICENSE` & `arkprts-0.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `arkprts-0.1.1/PKG-INFO` & `arkprts-0.1.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: arkprts
-Version: 0.1.1
+Version: 0.1.2
 Summary: Arknights python wrapper.
 Home-page: https://github.com/thesadru/arkprts
 License: MIT
 Description-Content-Type: text/markdown
 Provides-Extra: all
 License-File: LICENSE
```

### Comparing `arkprts-0.1.1/README.md` & `arkprts-0.1.2/README.md`

 * *Files identical despite different names*

### Comparing `arkprts-0.1.1/arkprts/__main__.py` & `arkprts-0.1.2/arkprts/__main__.py`

 * *Files identical despite different names*

### Comparing `arkprts-0.1.1/arkprts/client.py` & `arkprts-0.1.2/arkprts/client.py`

 * *Files identical despite different names*

### Comparing `arkprts-0.1.1/arkprts/errors.py` & `arkprts-0.1.2/arkprts/errors.py`

 * *Files identical despite different names*

### Comparing `arkprts-0.1.1/arkprts/gamedata.py` & `arkprts-0.1.2/arkprts/gamedata.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,17 +1,19 @@
 """Gamedata client. Fetches from github and such."""
 from __future__ import annotations
 
 import json
 import logging
+import os
 import os.path
 import pathlib
 import re
 import tarfile
 import tempfile
+import time
 import typing
 
 import aiohttp
 
 from arkprts.models import base as models
 
 __all__ = ("GameData",)
@@ -89,29 +91,41 @@
 
             tar.extractall(self.directory, members=members)
 
         return top_directory.split("-")[-1]
 
     async def download_gamedata(self, allow: str | None = None, *, force: bool = False) -> None:
         """Download game data."""
-        commit = await self._get_commit()
+        if not force and self.commit_file.exists() and time.time() - self.commit_file.stat().st_mtime < 60 * 60 * 6:
+            logger.debug("Game data was updated recently, skipping download")
+            return
+
+        try:
+            commit = await self._get_commit()
+        except aiohttp.ClientResponseError:
+            logger.warning("Failed to get game data commit, skipping download", exc_info=True)
+            return
+
         if not force and self.commit_file.exists() and self.commit_file.read_text() == commit:
             logger.debug("Game data is up to date [%s]", commit)
             return
 
         logger.info("Downloading game data to %s [%s]", self.directory, commit)
         await self._download_tarball()
 
         logger.debug("Decompressing game data")
         tarball_commit = self._decompress_tarball(allow)
         logger.debug("Decompressed data %s", tarball_commit)
         if tarball_commit not in commit:
             raise RuntimeError(f"Tarball commit {tarball_commit} does not match github commit {commit}")
 
+        # sometimes the contents are identical, we still want to update the mtime
         self.commit_file.write_text(commit)
+        os.utime(self.commit_file, (time.time(), time.time()))
+
         logger.info("Downloaded game data")
 
     def _get_data(self, name: str, *, server: str | None = None) -> models.DDict:
         """Get a file."""
         server = server or self.server
 
         if self._cache.get(server, {}).get(name):
@@ -124,40 +138,40 @@
         with path.open(encoding="utf-8") as file:
             data = json.load(file)
 
         self._cache.setdefault(server, {})[name] = data
 
         return models.DDict(data)
 
-    def _get_excel(self, name: str, *, server: str | None = None) -> models.DDict:
-        """Get an excel file."""
+    def get_excel(self, name: str, *, server: str | None = None) -> models.DDict:
+        """Get an excel table file."""
         return self._get_data(f"excel/{name}", server=server)
 
     def get_operator(self, id: str, *, server: str | None = None) -> models.DDict:
         """Get an operator."""
-        data = self._get_excel("character_table", server=server)
+        data = self.get_excel("character_table", server=server)
         return data[id]
 
     def get_item(self, id: str, *, server: str | None = None) -> models.DDict:
         """Get an item."""
-        data = self._get_excel("item_table", server=server)
+        data = self.get_excel("item_table", server=server)
         return data["items"][id]
 
     def get_medal(self, id: str, *, server: str | None = None) -> models.DDict:
         """Get a medal."""
-        data = self._get_excel("medal_table", server=server)
+        data = self.get_excel("medal_table", server=server)
         return data["medalList"][id]
 
     def get_medal_group(self, id: str, *, server: str | None = None) -> models.DDict:
         """Get a medal group. Way too specific probably."""
-        data = self._get_excel("medal_table", server=server)
+        data = self.get_excel("medal_table", server=server)
         return next(i for i in data["medalTypeData"]["activityMedal"]["groupData"] if i["groupId"] == id)
 
     def get_skill(self, id: str, *, server: str | None = None) -> models.DDict:
         """Get a skill."""
-        data = self._get_excel("skill_table", server=server)
+        data = self.get_excel("skill_table", server=server)
         return data[id]
 
     def get_module(self, id: str, *, server: str | None = None) -> models.DDict:
         """Get a module."""
-        data = self._get_excel("uniequip_table", server=server)
+        data = self.get_excel("uniequip_table", server=server)
         return data["equipDict"][id]
```

### Comparing `arkprts-0.1.1/arkprts/models/base.py` & `arkprts-0.1.2/arkprts/models/base.py`

 * *Files 5% similar despite different names*

```diff
@@ -61,14 +61,18 @@
         if isinstance(item, dict):
             item = DDict(item)  # pyright: ignore[reportUnknownArgumentType]
         elif isinstance(item, list):
             item = DList(item)  # pyright: ignore[reportUnknownArgumentType]
 
         return item
 
+    @classmethod
+    def __get_validators__(cls) -> typing.Iterator[typing.Callable[..., typing.Any]]:
+        yield lambda i: cls(i)
+
 
 class DDict(collections.UserDict[str, typing.Any]):
     """Dot-accessed dictionary."""
 
     def __getitem__(self, key: typing.Any) -> typing.Any:
         try:
             item = super().__getitem__(key)
@@ -80,7 +84,11 @@
         elif isinstance(item, list):
             item = DList(item)  # pyright: ignore[reportUnknownArgumentType]
 
         return item
 
     def __getattr__(self, key: str) -> typing.Any:
         return self[key]
+
+    @classmethod
+    def __get_validators__(cls) -> typing.Iterator[typing.Callable[..., typing.Any]]:
+        yield lambda i: cls(i)
```

### Comparing `arkprts-0.1.1/arkprts/models/data.py` & `arkprts-0.1.2/arkprts/models/data.py`

 * *Files 6% similar despite different names*

```diff
@@ -206,18 +206,18 @@
     cur_squad_count: int = pydantic.Field(alias="curSquadCount")
     """Amount of squads. Should be always 4."""
     squads: typing.Mapping[int, Squads]
     """Squad data."""
     chars: typing.Mapping[int, Character]
     """Operator data."""
     char_group: typing.Mapping[str, CharGroup] = pydantic.Field(alias="charGroup")
-    """Operator group data."""
+    """Additional operator data."""
     char_mission: typing.Mapping[str, typing.Mapping[str, bool]] = pydantic.Field(alias="charMission")
     """Special operation missions."""
-    addon: typing.Any
+    addon: base.DDict
     """IDK."""
 
     @pydantic.validator("chars", pre=True)  # pyright: ignore[reportUnknownMemberType]
     def _fix_amiya(cls, value: typing.Any) -> typing.Any:
         """Flatten amiya to only keep her guard form."""
         for v in value.values():
             if v and v.get("tmpl"):
@@ -232,14 +232,38 @@
 
     character_skins: typing.Mapping[str, bool] = pydantic.Field(alias="characterSkins")
     """Owned skins."""
     skin_ts: typing.Mapping[str, datetime.datetime] = pydantic.Field(alias="skinTs")
     """When the skins were obtained."""
 
 
+class AssistChar(base.BaseModel):
+    """Assist operator data."""
+
+    char_inst_id: int = pydantic.Field(alias="charInstId")
+    """Index of the operator."""
+    skill_index: int = pydantic.Field(alias="skillIndex")
+    """Index of the selected skill."""
+    current_equip: typing.Optional[str] = pydantic.Field(alias="currentEquip")
+    """Currently equipped module."""
+
+
+class Social(base.BaseModel):
+    """Social data."""
+
+    assist_char_list: typing.Sequence[AssistChar] = pydantic.Field(alias="assistCharList")
+    """Support operators."""
+    yesterday_reward: base.DDict = pydantic.Field(alias="yesterdayReward")
+    """IDK. Clue exchange data."""
+    y_crisis_ss: typing.Union[str, typing.Any] = pydantic.Field(alias="yCrisisSs")
+    """IDK."""
+    medal_board: base.DDict = pydantic.Field(alias="medalBoard")
+    """Medal board."""
+
+
 class ConsumableExpire(base.BaseModel):
     """Consumable expiration data."""
 
     ts: datetime.datetime
     """When the consumable expires."""
     count: int
     """Amount of consumables."""
@@ -250,14 +274,16 @@
 
     status: Status
     """General user data."""
     troop: Troops
     """Operator data."""
     skin: Skins
     """Operator skin data."""
+    social: Social
+    """Data related to friends."""
     cosumable: typing.Mapping[str, typing.Mapping[int, ConsumableExpire]] = {}
     """Consumable data."""
     inventory: typing.Mapping[str, int]
     """Inventory data. Item ID to amount.
 
     To access the static data for an item, use `client.gamedata.get_item(item_id)`.
     """
```

### Comparing `arkprts-0.1.1/arkprts/models/social.py` & `arkprts-0.1.2/arkprts/models/social.py`

 * *Files 1% similar despite different names*

```diff
@@ -74,15 +74,15 @@
     """Elite phase."""
     favor_point: int = pydantic.Field(alias="favorPoint")
     """Raw trust points (25570 is 200% Trust)"""
     potential_rank: int = pydantic.Field(alias="potentialRank")
     """Operator potential. Starts at 0."""
     level: int
     """Operator level."""
-    crisis_record: typing.Any = pydantic.Field(alias="crisisRecord")
+    crisis_record: base.DDict = pydantic.Field(alias="crisisRecord")
     """IDK. selectedCrisis is used for contingency contracts elsewhere."""
     current_equip: typing.Optional[str] = pydantic.Field(alias="currentEquip")
     """ID of the currently equipped module."""
     equip: typing.Mapping[str, UniEquip]
     """Equipped modules. Module ID to module info."""
 
     @property
```

### Comparing `arkprts-0.1.1/arkprts.egg-info/PKG-INFO` & `arkprts-0.1.2/arkprts.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: arkprts
-Version: 0.1.1
+Version: 0.1.2
 Summary: Arknights python wrapper.
 Home-page: https://github.com/thesadru/arkprts
 License: MIT
 Description-Content-Type: text/markdown
 Provides-Extra: all
 License-File: LICENSE
```

### Comparing `arkprts-0.1.1/pyproject.toml` & `arkprts-0.1.2/pyproject.toml`

 * *Files identical despite different names*

### Comparing `arkprts-0.1.1/setup.py` & `arkprts-0.1.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 """Run setuptools."""
 import pathlib
 
 from setuptools import find_packages, setup
 
 setup(
     name="arkprts",
-    version="0.1.1",
+    version="0.1.2",
     description="Arknights python wrapper.",
     url="https://github.com/thesadru/arkprts",
     packages=find_packages(exclude=["tests", "tests.*"]),
     include_package_data=True,
     package_data={"arkprts": ["py.typed"]},
     install_requires=["aiohttp", "pydantic"],
     extras_require={
```

