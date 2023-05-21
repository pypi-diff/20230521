# Comparing `tmp/APIxoo-0.1.1.tar.gz` & `tmp/APIxoo-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "APIxoo-0.1.1.tar", last modified: Fri May 12 08:16:52 2023, max compression
+gzip compressed data, was "APIxoo-0.2.0.tar", last modified: Sun May 21 13:42:00 2023, max compression
```

## Comparing `APIxoo-0.1.1.tar` & `APIxoo-0.2.0.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 08:16:52.068792 APIxoo-0.1.1/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 08:16:52.068792 APIxoo-0.1.1/APIxoo.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1469 2023-05-12 08:16:52.000000 APIxoo-0.1.1/APIxoo.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      263 2023-05-12 08:16:52.000000 APIxoo-0.1.1/APIxoo.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-12 08:16:52.000000 APIxoo-0.1.1/APIxoo.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-05-12 08:16:52.000000 APIxoo-0.1.1/APIxoo.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-05-12 08:16:52.000000 APIxoo-0.1.1/APIxoo.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1063 2023-05-12 08:16:34.000000 APIxoo-0.1.1/LICENSE.md
--rw-r--r--   0 runner    (1001) docker     (123)     1469 2023-05-12 08:16:52.068792 APIxoo-0.1.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      979 2023-05-12 08:16:34.000000 APIxoo-0.1.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 08:16:52.068792 APIxoo-0.1.1/apixoo/
--rw-r--r--   0 runner    (1001) docker     (123)     4143 2023-05-12 08:16:34.000000 APIxoo-0.1.1/apixoo/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3222 2023-05-12 08:16:34.000000 APIxoo-0.1.1/apixoo/const.py
--rw-r--r--   0 runner    (1001) docker     (123)     2475 2023-05-12 08:16:34.000000 APIxoo-0.1.1/apixoo/pixel_bean.py
--rw-r--r--   0 runner    (1001) docker     (123)     9345 2023-05-12 08:16:34.000000 APIxoo-0.1.1/apixoo/pixel_bean_decoder.py
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-12 08:16:52.068792 APIxoo-0.1.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      882 2023-05-12 08:16:34.000000 APIxoo-0.1.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 13:42:00.296353 APIxoo-0.2.0/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 13:42:00.296353 APIxoo-0.2.0/APIxoo.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1469 2023-05-21 13:42:00.000000 APIxoo-0.2.0/APIxoo.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      263 2023-05-21 13:42:00.000000 APIxoo-0.2.0/APIxoo.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-21 13:42:00.000000 APIxoo-0.2.0/APIxoo.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-05-21 13:42:00.000000 APIxoo-0.2.0/APIxoo.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-05-21 13:42:00.000000 APIxoo-0.2.0/APIxoo.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1063 2023-05-21 13:41:47.000000 APIxoo-0.2.0/LICENSE.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1469 2023-05-21 13:42:00.296353 APIxoo-0.2.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      979 2023-05-21 13:41:47.000000 APIxoo-0.2.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 13:42:00.296353 APIxoo-0.2.0/apixoo/
+-rw-r--r--   0 runner    (1001) docker     (123)     5878 2023-05-21 13:41:47.000000 APIxoo-0.2.0/apixoo/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3542 2023-05-21 13:41:47.000000 APIxoo-0.2.0/apixoo/const.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2519 2023-05-21 13:41:47.000000 APIxoo-0.2.0/apixoo/pixel_bean.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9345 2023-05-21 13:41:47.000000 APIxoo-0.2.0/apixoo/pixel_bean_decoder.py
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-21 13:42:00.296353 APIxoo-0.2.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      882 2023-05-21 13:41:47.000000 APIxoo-0.2.0/setup.py
```

### Comparing `APIxoo-0.1.1/APIxoo.egg-info/PKG-INFO` & `APIxoo-0.2.0/APIxoo.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: APIxoo
-Version: 0.1.1
+Version: 0.2.0
 Summary: Python wrapper for Divoom Pixoo server API
 Home-page: https://github.com/redphx/apixoo
 Download-URL: https://github.com/redphx/apixoo
 Author: redphx
 License: MIT
 Keywords: apixoo,divoom,pixoo,pixoo64
 Platform: any
```

### Comparing `APIxoo-0.1.1/LICENSE.md` & `APIxoo-0.2.0/LICENSE.md`

 * *Files identical despite different names*

### Comparing `APIxoo-0.1.1/PKG-INFO` & `APIxoo-0.2.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: APIxoo
-Version: 0.1.1
+Version: 0.2.0
 Summary: Python wrapper for Divoom Pixoo server API
 Home-page: https://github.com/redphx/apixoo
 Download-URL: https://github.com/redphx/apixoo
 Author: redphx
 License: MIT
 Keywords: apixoo,divoom,pixoo,pixoo64
 Platform: any
```

### Comparing `APIxoo-0.1.1/README.md` & `APIxoo-0.2.0/README.md`

 * *Files identical despite different names*

### Comparing `APIxoo-0.1.1/apixoo/const.py` & `APIxoo-0.2.0/apixoo/const.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,11 +1,9 @@
 from enum import Enum
 
-REQUESTS_TIMEOUT = 10
-
 
 class GalleryCategory(int, Enum):
     NEW = 0
     DEFAULT = 1
     LED_TEXT = 2
     CHARACTER = 3
     EMOJI = 4
@@ -21,15 +19,15 @@
     FESTIVAL = 17
     RECOMMEND = 18
     PLANET = 19
     FOLLOW = 20
     REVIEW_PHOTOS = 21
     REVIEW_STOLEN_PHOTOS = 22
     FILL_GAME = 29
-    PIXEL_MATCH = 30
+    PIXEL_MATCH = 30  # Current event
     PLANT = 31
     ANIMAL = 32
     PERSON = 33
     EMOJI_2 = 34
     FOOD = 35
     OTHERS = 36
     REPORT_PHOTO = 254
@@ -58,38 +56,59 @@
     W16H16 = 1
     W32H32 = 2
     W64H64 = 4
     ALL = 15
 
 
 class Server(str, Enum):
-    API = 'https://app.divoom-gz.com'
-    FILE = 'https://f.divoom-gz.com'
+    API = 'app.divoom-gz.com'
+    FILE = 'f.divoom-gz.com'
 
 
-class UserInfo(dict):
-    KEYS_MAP = {
-        'UserId': 'user_id',
-        'UserName': 'user_name',
-    }
+class ApiEndpoint(str, Enum):
+    GET_ALBUM_LIST = '/Discover/GetAlbumList'
+    GET_ALBUM_FILES = '/Discover/GetAlbumImageList'
+    GET_CATEGORY_FILES = '/GetCategoryFileListV2'
+    GET_GALLERY_INFO = '/Cloud/GalleryInfo'
+    USER_LOGIN = '/UserLogin'
+
+
+class BaseDictInfo(dict):
+    _KEYS_MAP = {}
 
     def __init__(self, info: dict):
         # Rename keys
-        for key in self.KEYS_MAP:
-            self.__dict__[self.KEYS_MAP[key]] = info.get(key)
+        for key in self._KEYS_MAP:
+            self.__dict__[self._KEYS_MAP[key]] = info.get(key)
 
         # Make this object JSON serializable
         dict.__init__(self, **self.__dict__)
 
     def __setattr__(self, name, value):
-        raise Exception('UserInfo object is read only!')
+        raise Exception('%s object is read only!' % (type(self).__name__))
+
+
+class AlbumInfo(BaseDictInfo):
+    _KEYS_MAP = {
+        'AlbumId': 'album_id',
+        'AlbumName': 'album_name',
+        'AlbumImageId': 'album_image_id',
+        'AlbumBigImageId': 'album_big_image_id',
+    }
 
 
-class GalleryInfo(dict):
-    KEYS_MAP = {
+class UserInfo(BaseDictInfo):
+    _KEYS_MAP = {
+        'UserId': 'user_id',
+        'UserName': 'user_name',
+    }
+
+
+class GalleryInfo(BaseDictInfo):
+    _KEYS_MAP = {
         'Classify': 'category',
         'CommentCnt': 'total_comments',
         'Content': 'content',
         'CopyrightFlag': 'copyright_flag',
         'CountryISOCode': 'country_iso_code',
         'Date': 'date',
         'FileId': 'file_id',
@@ -121,21 +140,16 @@
         # 'PixelAmbName': '',
         # 'PrivateFlag': 0,
         # 'RegionId': '55',
         # 'UserHeaderId': 'group1/M00/1B/BF/...',
     }
 
     def __init__(self, info: dict):
-        # Rename keys
-        for key in self.KEYS_MAP:
-            self.__dict__[self.KEYS_MAP[key]] = info.get(key)
+        super().__init__(info)
 
         # Parse user info
         self.__dict__['user'] = None
         if 'UserId' in info:
             self.__dict__['user'] = UserInfo(info)
 
-        # Make this object JSON serializable
+        # Update dict
         dict.__init__(self, **self.__dict__)
-
-    def __setattr__(self, name, value):
-        raise Exception('GalleryInfo object is read only!')
```

### Comparing `APIxoo-0.1.1/apixoo/pixel_bean.py` & `APIxoo-0.2.0/apixoo/pixel_bean.py`

 * *Files 3% similar despite different names*

```diff
@@ -45,14 +45,15 @@
     def save_to_gif(
         self,
         output_path: str,
         scale: int | float = 1,
         width: int = None,
         height: int = None,
     ) -> None:
+        """Convert animation to GIF file"""
         gif_frames = []
 
         org_width = self._column_count * 16
         org_height = self._row_count * 16
 
         for _, frame_data in enumerate(self._frames_data):
             img = Image.new('RGBA', (org_width, org_height))
```

### Comparing `APIxoo-0.1.1/apixoo/pixel_bean_decoder.py` & `APIxoo-0.2.0/apixoo/pixel_bean_decoder.py`

 * *Files identical despite different names*

### Comparing `APIxoo-0.1.1/setup.py` & `APIxoo-0.2.0/setup.py`

 * *Files 13% similar despite different names*

```diff
@@ -4,15 +4,15 @@
     from distutils.core import setup
 
 long_desc = open("README.md").read()
 required = ['requests']
 
 setup(
     name='APIxoo',
-    version="0.1.1",
+    version="0.2.0",
     author="redphx",
     license="MIT",
     url="https://github.com/redphx/apixoo",
     download_url="https://github.com/redphx/apixoo",
     long_description=long_desc,
     long_description_content_type="text/markdown",
     description="Python wrapper for Divoom Pixoo server API",
```

