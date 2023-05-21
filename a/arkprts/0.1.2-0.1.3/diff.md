# Comparing `tmp/arkprts-0.1.2.tar.gz` & `tmp/arkprts-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "arkprts-0.1.2.tar", last modified: Sun May 21 14:32:30 2023, max compression
+gzip compressed data, was "arkprts-0.1.3.tar", last modified: Sun May 21 17:13:42 2023, max compression
```

## Comparing `arkprts-0.1.2.tar` & `arkprts-0.1.3.tar`

### file list

```diff
@@ -1,28 +1,28 @@
-drwxrwxrwx   0        0        0        0 2023-05-21 14:32:30.656536 arkprts-0.1.2/
--rw-rw-rw-   0        0        0    35823 2023-04-30 21:01:40.000000 arkprts-0.1.2/LICENSE
--rw-rw-rw-   0        0        0     1748 2023-05-21 14:32:30.653533 arkprts-0.1.2/PKG-INFO
--rw-rw-rw-   0        0        0     1462 2023-05-19 17:49:21.000000 arkprts-0.1.2/README.md
-drwxrwxrwx   0        0        0        0 2023-05-21 14:32:30.575577 arkprts-0.1.2/arkprts/
--rw-rw-rw-   0        0        0      111 2023-05-19 17:48:39.000000 arkprts-0.1.2/arkprts/__init__.py
--rw-rw-rw-   0        0        0     1922 2023-05-19 18:21:49.000000 arkprts-0.1.2/arkprts/__main__.py
--rw-rw-rw-   0        0        0    12390 2023-05-19 19:14:56.000000 arkprts-0.1.2/arkprts/client.py
--rw-rw-rw-   0        0        0     1356 2023-05-07 16:47:55.000000 arkprts-0.1.2/arkprts/errors.py
--rw-rw-rw-   0        0        0     6605 2023-05-21 14:06:41.000000 arkprts-0.1.2/arkprts/gamedata.py
-drwxrwxrwx   0        0        0        0 2023-05-21 14:32:30.641540 arkprts-0.1.2/arkprts/models/
--rw-rw-rw-   0        0        0       75 2023-05-07 15:46:44.000000 arkprts-0.1.2/arkprts/models/__init__.py
--rw-rw-rw-   0        0        0     3012 2023-05-21 13:53:11.000000 arkprts-0.1.2/arkprts/models/base.py
--rw-rw-rw-   0        0        0     9871 2023-05-21 13:56:15.000000 arkprts-0.1.2/arkprts/models/data.py
--rw-rw-rw-   0        0        0     6953 2023-05-21 13:50:03.000000 arkprts-0.1.2/arkprts/models/social.py
--rw-rw-rw-   0        0        0        0 2023-04-30 21:01:40.000000 arkprts-0.1.2/arkprts/py.typed
-drwxrwxrwx   0        0        0        0 2023-05-21 14:32:30.624552 arkprts-0.1.2/arkprts.egg-info/
--rw-rw-rw-   0        0        0     1748 2023-05-21 14:32:30.000000 arkprts-0.1.2/arkprts.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      450 2023-05-21 14:32:30.000000 arkprts-0.1.2/arkprts.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-21 14:32:30.000000 arkprts-0.1.2/arkprts.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       41 2023-05-21 14:32:30.000000 arkprts-0.1.2/arkprts.egg-info/requires.txt
--rw-rw-rw-   0        0        0        8 2023-05-21 14:32:30.000000 arkprts-0.1.2/arkprts.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     2569 2023-05-19 18:44:52.000000 arkprts-0.1.2/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-05-21 14:32:30.657536 arkprts-0.1.2/setup.cfg
--rw-rw-rw-   0        0        0      623 2023-05-21 14:02:40.000000 arkprts-0.1.2/setup.py
-drwxrwxrwx   0        0        0        0 2023-05-21 14:32:30.649534 arkprts-0.1.2/tests/
--rw-rw-rw-   0        0        0      282 2023-05-01 00:20:38.000000 arkprts-0.1.2/tests/test_config.py
--rw-rw-rw-   0        0        0      357 2023-05-19 18:47:11.000000 arkprts-0.1.2/tests/test_gamedata.py
+drwxrwxrwx   0        0        0        0 2023-05-21 17:13:42.396297 arkprts-0.1.3/
+-rw-rw-rw-   0        0        0    35823 2023-04-30 21:01:40.000000 arkprts-0.1.3/LICENSE
+-rw-rw-rw-   0        0        0     1748 2023-05-21 17:13:42.393309 arkprts-0.1.3/PKG-INFO
+-rw-rw-rw-   0        0        0     1462 2023-05-19 17:49:21.000000 arkprts-0.1.3/README.md
+drwxrwxrwx   0        0        0        0 2023-05-21 17:13:42.235389 arkprts-0.1.3/arkprts/
+-rw-rw-rw-   0        0        0      111 2023-05-19 17:48:39.000000 arkprts-0.1.3/arkprts/__init__.py
+-rw-rw-rw-   0        0        0     1922 2023-05-19 18:21:49.000000 arkprts-0.1.3/arkprts/__main__.py
+-rw-rw-rw-   0        0        0    12390 2023-05-19 19:14:56.000000 arkprts-0.1.3/arkprts/client.py
+-rw-rw-rw-   0        0        0     1356 2023-05-07 16:47:55.000000 arkprts-0.1.3/arkprts/errors.py
+-rw-rw-rw-   0        0        0     6605 2023-05-21 14:06:41.000000 arkprts-0.1.3/arkprts/gamedata.py
+drwxrwxrwx   0        0        0        0 2023-05-21 17:13:42.358318 arkprts-0.1.3/arkprts/models/
+-rw-rw-rw-   0        0        0       75 2023-05-07 15:46:44.000000 arkprts-0.1.3/arkprts/models/__init__.py
+-rw-rw-rw-   0        0        0     3012 2023-05-21 13:53:11.000000 arkprts-0.1.3/arkprts/models/base.py
+-rw-rw-rw-   0        0        0    10890 2023-05-21 17:06:34.000000 arkprts-0.1.3/arkprts/models/data.py
+-rw-rw-rw-   0        0        0     6953 2023-05-21 13:50:03.000000 arkprts-0.1.3/arkprts/models/social.py
+-rw-rw-rw-   0        0        0        0 2023-04-30 21:01:40.000000 arkprts-0.1.3/arkprts/py.typed
+drwxrwxrwx   0        0        0        0 2023-05-21 17:13:42.307348 arkprts-0.1.3/arkprts.egg-info/
+-rw-rw-rw-   0        0        0     1748 2023-05-21 17:13:42.000000 arkprts-0.1.3/arkprts.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      450 2023-05-21 17:13:42.000000 arkprts-0.1.3/arkprts.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-21 17:13:42.000000 arkprts-0.1.3/arkprts.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       41 2023-05-21 17:13:42.000000 arkprts-0.1.3/arkprts.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        8 2023-05-21 17:13:42.000000 arkprts-0.1.3/arkprts.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     2569 2023-05-19 18:44:52.000000 arkprts-0.1.3/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-05-21 17:13:42.397296 arkprts-0.1.3/setup.cfg
+-rw-rw-rw-   0        0        0      623 2023-05-21 17:12:18.000000 arkprts-0.1.3/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-21 17:13:42.383303 arkprts-0.1.3/tests/
+-rw-rw-rw-   0        0        0      282 2023-05-01 00:20:38.000000 arkprts-0.1.3/tests/test_config.py
+-rw-rw-rw-   0        0        0      357 2023-05-19 18:47:11.000000 arkprts-0.1.3/tests/test_gamedata.py
```

### Comparing `arkprts-0.1.2/LICENSE` & `arkprts-0.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `arkprts-0.1.2/PKG-INFO` & `arkprts-0.1.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: arkprts
-Version: 0.1.2
+Version: 0.1.3
 Summary: Arknights python wrapper.
 Home-page: https://github.com/thesadru/arkprts
 License: MIT
 Description-Content-Type: text/markdown
 Provides-Extra: all
 License-File: LICENSE
```

### Comparing `arkprts-0.1.2/README.md` & `arkprts-0.1.3/README.md`

 * *Files identical despite different names*

### Comparing `arkprts-0.1.2/arkprts/__main__.py` & `arkprts-0.1.3/arkprts/__main__.py`

 * *Files identical despite different names*

### Comparing `arkprts-0.1.2/arkprts/client.py` & `arkprts-0.1.3/arkprts/client.py`

 * *Files identical despite different names*

### Comparing `arkprts-0.1.2/arkprts/errors.py` & `arkprts-0.1.3/arkprts/errors.py`

 * *Files identical despite different names*

### Comparing `arkprts-0.1.2/arkprts/gamedata.py` & `arkprts-0.1.3/arkprts/gamedata.py`

 * *Files identical despite different names*

### Comparing `arkprts-0.1.2/arkprts/models/base.py` & `arkprts-0.1.3/arkprts/models/base.py`

 * *Files identical despite different names*

### Comparing `arkprts-0.1.2/arkprts/models/data.py` & `arkprts-0.1.3/arkprts/models/data.py`

 * *Files 7% similar despite different names*

```diff
@@ -27,15 +27,15 @@
     nick_number: str = pydantic.Field(alias="nickNumber")
     """Player nickname number after #."""
     level: int
     """Player level."""
     exp: int
     """Player experience."""
     social_point: int = pydantic.Field(alias="socialPoint")
-    """IDK."""
+    """Credit shop credits."""
     gacha_ticket: int = pydantic.Field(alias="gachaTicket")
     """Amount of single headhunting permits."""
     ten_gacha_ticket: int = pydantic.Field(alias="tenGachaTicket")
     """Amount of 10-headhunting permits."""
     instant_finish_ticket: int = pydantic.Field(alias="instantFinishTicket")
     """Amount of expedited completion permits."""
     hgg_shard: int = pydantic.Field(alias="hggShard")
@@ -45,35 +45,35 @@
     recruit_license: int = pydantic.Field(alias="recruitLicense")
     """Amount of recruitment permit."""
     progress: int
     """IDK."""
     buy_ap_remain_times: int = pydantic.Field(alias="buyApRemainTimes")
     """Remaining pulls until guaranteed 5 star operator."""
     ap_limit_up_flag: bool = pydantic.Field(alias="apLimitUpFlag")
-    """Whether the guaranteed 5 star has been pulled."""
+    """IDK. Ap refers to sanity."""
     uid: str
     """User ID."""
     flags: typing.Mapping[str, bool]
     """Completed stories."""
     ap: int
-    """Pulls made on the current banner."""
+    """Current sanity."""
     max_ap: int = pydantic.Field(alias="maxAp")
-    """IDK."""
+    """Max sanity."""
     pay_diamond: int = pydantic.Field(alias="payDiamond")
     """Bough originium prime."""
     free_diamond: int = pydantic.Field(alias="freeDiamond")
     """Earned originium prime."""
     diamond_shard: int = pydantic.Field(alias="diamondShard")
     """Amount of orundum."""
     gold: int
     """Amount of LMD."""
     practice_ticket: int = pydantic.Field(alias="practiceTicket")
     """Amount of training permits."""
     last_refresh_ts: datetime.datetime = pydantic.Field(alias="lastRefreshTs")
-    """IDK."""
+    """IDK. When sanity was last incremented."""
     last_ap_add_time: datetime.datetime = pydantic.Field(alias="lastApAddTime")
     """IDK."""
     main_stage_progress: str = pydantic.Field(alias="mainStageProgress")
     """Current main story stage ID. None if completed."""
     register_ts: datetime.datetime = pydantic.Field(alias="registerTs")
     """Account creation time."""
     server_name: str = pydantic.Field(alias="serverName")
@@ -89,14 +89,33 @@
     secretary_skin_id: str = pydantic.Field(alias="secretarySkinId")
     """ID of the secretary operator's skin."""
     global_voice_lan: typing.Optional[str] = pydantic.Field(None, alias="globalVoiceLan")
     """Default voice-over language."""
     avatar: Avatar
     """Selected avatar."""
 
+    @property
+    def basic_item_inventory(self) -> typing.Mapping[str, int]:
+        """Basic item inventory. These are not shown in the inventory object."""
+        return {
+            "SOCIAL_PT": self.social_point,
+            "AP_GAMEPLAY": self.ap,
+            "4001": self.gold,
+            "4002": self.pay_diamond + self.free_diamond,
+            "4003": self.diamond_shard,
+            "4004": self.hgg_shard,
+            "4005": self.lgg_shard,
+            "5001": self.exp,
+            "6001": self.practice_ticket,
+            "7001": self.recruit_license,
+            "7002": self.instant_finish_ticket,
+            "7003": self.gacha_ticket,
+            "7004": self.ten_gacha_ticket,
+        }
+
 
 class SquadSlot(base.BaseModel):
     """Squad slot."""
 
     char_inst_id: int = pydantic.Field(alias="charInstId")
     """Operator index."""
     skill_index: int = pydantic.Field(alias="skillIndex")
@@ -177,17 +196,20 @@
     """Elite phase."""
     default_skill_index: int = pydantic.Field(alias="defaultSkillIndex")
     """Index of the default skill."""
     skills: typing.Sequence[Skill]
     """Operator skills."""
     voice_lan: str = pydantic.Field(alias="voiceLan")
     """Operator voice-over language."""
-    current_equip: typing.Optional[str] = None
+    current_equip: typing.Optional[str] = pydantic.Field(alias="currentEquip")
     """Currently equipped module."""
     equip: typing.Mapping[str, Equip]
+    """Operator modules."""
+    star_mark: bool = pydantic.Field(False, alias="starMark")
+    """Whether the operator is marked as favorite."""
 
     @property
     def static(self) -> base.DDict:
         """Static data for this operator."""
         return self.client.gamedata.get_operator(self.char_id)
 
 
@@ -209,15 +231,15 @@
     """Squad data."""
     chars: typing.Mapping[int, Character]
     """Operator data."""
     char_group: typing.Mapping[str, CharGroup] = pydantic.Field(alias="charGroup")
     """Additional operator data."""
     char_mission: typing.Mapping[str, typing.Mapping[str, bool]] = pydantic.Field(alias="charMission")
     """Special operation missions."""
-    addon: base.DDict
+    addon: base.DDict = pydantic.Field(default_factory=base.DDict)
     """IDK."""
 
     @pydantic.validator("chars", pre=True)  # pyright: ignore[reportUnknownMemberType]
     def _fix_amiya(cls, value: typing.Any) -> typing.Any:
         """Flatten amiya to only keep her guard form."""
         for v in value.values():
             if v and v.get("tmpl"):
@@ -246,21 +268,21 @@
     current_equip: typing.Optional[str] = pydantic.Field(alias="currentEquip")
     """Currently equipped module."""
 
 
 class Social(base.BaseModel):
     """Social data."""
 
-    assist_char_list: typing.Sequence[AssistChar] = pydantic.Field(alias="assistCharList")
+    assist_char_list: typing.Sequence[typing.Optional[AssistChar]] = pydantic.Field(alias="assistCharList")
     """Support operators."""
     yesterday_reward: base.DDict = pydantic.Field(alias="yesterdayReward")
     """IDK. Clue exchange data."""
     y_crisis_ss: typing.Union[str, typing.Any] = pydantic.Field(alias="yCrisisSs")
     """IDK."""
-    medal_board: base.DDict = pydantic.Field(alias="medalBoard")
+    medal_board: base.DDict = pydantic.Field(default_factory=base.DDict, alias="medalBoard")
     """Medal board."""
 
 
 class ConsumableExpire(base.BaseModel):
     """Consumable expiration data."""
 
     ts: datetime.datetime
@@ -276,14 +298,14 @@
     """General user data."""
     troop: Troops
     """Operator data."""
     skin: Skins
     """Operator skin data."""
     social: Social
     """Data related to friends."""
-    cosumable: typing.Mapping[str, typing.Mapping[int, ConsumableExpire]] = {}
+    consumable: typing.Mapping[str, typing.Mapping[int, ConsumableExpire]] = {}
     """Consumable data."""
     inventory: typing.Mapping[str, int]
     """Inventory data. Item ID to amount.
 
     To access the static data for an item, use `client.gamedata.get_item(item_id)`.
     """
```

### Comparing `arkprts-0.1.2/arkprts/models/social.py` & `arkprts-0.1.3/arkprts/models/social.py`

 * *Files identical despite different names*

### Comparing `arkprts-0.1.2/arkprts.egg-info/PKG-INFO` & `arkprts-0.1.3/arkprts.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: arkprts
-Version: 0.1.2
+Version: 0.1.3
 Summary: Arknights python wrapper.
 Home-page: https://github.com/thesadru/arkprts
 License: MIT
 Description-Content-Type: text/markdown
 Provides-Extra: all
 License-File: LICENSE
```

### Comparing `arkprts-0.1.2/pyproject.toml` & `arkprts-0.1.3/pyproject.toml`

 * *Files identical despite different names*

### Comparing `arkprts-0.1.2/setup.py` & `arkprts-0.1.3/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 """Run setuptools."""
 import pathlib
 
 from setuptools import find_packages, setup
 
 setup(
     name="arkprts",
-    version="0.1.2",
+    version="0.1.3",
     description="Arknights python wrapper.",
     url="https://github.com/thesadru/arkprts",
     packages=find_packages(exclude=["tests", "tests.*"]),
     include_package_data=True,
     package_data={"arkprts": ["py.typed"]},
     install_requires=["aiohttp", "pydantic"],
     extras_require={
```

