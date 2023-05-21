# Comparing `tmp/aiotiktok-2.5.4.tar.gz` & `tmp/aiotiktok-2.6.tar.gz`

## Comparing `aiotiktok-2.5.4.tar` & `aiotiktok-2.6.tar`

### file list

```diff
@@ -1,10 +1,11 @@
--rw-r--r--   0        0        0       53 2020-02-02 00:00:00.000000 aiotiktok-2.5.4/aiotiktok/__init__.py
--rw-r--r--   0        0        0     3669 2020-02-02 00:00:00.000000 aiotiktok-2.5.4/aiotiktok/client.py
--rw-r--r--   0        0        0       94 2020-02-02 00:00:00.000000 aiotiktok-2.5.4/aiotiktok/exceptions.py
--rw-r--r--   0        0        0     1817 2020-02-02 00:00:00.000000 aiotiktok-2.5.4/aiotiktok/extractors.py
--rw-r--r--   0        0        0      724 2020-02-02 00:00:00.000000 aiotiktok-2.5.4/aiotiktok/types.py
--rw-r--r--   0        0        0     1942 2020-02-02 00:00:00.000000 aiotiktok-2.5.4/.gitignore
--rw-r--r--   0        0        0     1084 2020-02-02 00:00:00.000000 aiotiktok-2.5.4/LICENSE
--rw-r--r--   0        0        0      688 2020-02-02 00:00:00.000000 aiotiktok-2.5.4/README.md
--rw-r--r--   0        0        0      622 2020-02-02 00:00:00.000000 aiotiktok-2.5.4/pyproject.toml
--rw-r--r--   0        0        0     1062 2020-02-02 00:00:00.000000 aiotiktok-2.5.4/PKG-INFO
+-rw-r--r--   0        0        0       51 2020-02-02 00:00:00.000000 aiotiktok-2.6/aiotiktok/__init__.py
+-rw-r--r--   0        0        0     6472 2020-02-02 00:00:00.000000 aiotiktok-2.6/aiotiktok/client.py
+-rw-r--r--   0        0        0     1480 2020-02-02 00:00:00.000000 aiotiktok-2.6/aiotiktok/constants.py
+-rw-r--r--   0        0        0       94 2020-02-02 00:00:00.000000 aiotiktok-2.6/aiotiktok/exceptions.py
+-rw-r--r--   0        0        0     2149 2020-02-02 00:00:00.000000 aiotiktok-2.6/aiotiktok/extractors.py
+-rw-r--r--   0        0        0     1009 2020-02-02 00:00:00.000000 aiotiktok-2.6/aiotiktok/types.py
+-rw-r--r--   0        0        0     1942 2020-02-02 00:00:00.000000 aiotiktok-2.6/.gitignore
+-rw-r--r--   0        0        0     1084 2020-02-02 00:00:00.000000 aiotiktok-2.6/LICENSE
+-rw-r--r--   0        0        0     1252 2020-02-02 00:00:00.000000 aiotiktok-2.6/README.md
+-rw-r--r--   0        0        0      622 2020-02-02 00:00:00.000000 aiotiktok-2.6/pyproject.toml
+-rw-r--r--   0        0        0     1601 2020-02-02 00:00:00.000000 aiotiktok-2.6/PKG-INFO
```

### Comparing `aiotiktok-2.5.4/aiotiktok/extractors.py` & `aiotiktok-2.6/aiotiktok/extractors.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,51 +1,56 @@
 import json
 import re
 
-from .types import Album, Video, VideoData
-
-video_type_codes = {
-    0: "video",
-    51: "video",
-    55: "video",
-    58: "video",
-    61: "video",
-    150: "album",
-}
+from .types import Album, Author, Video, VideoData, VideoType, video_type_codes
 
 
 def extract_video_data(data: dict) -> VideoData:
-    video_type_code = data["aweme_type"]
-    video_type = video_type_codes.get(video_type_code, "video")
-    if video_type == "album":
+    video_type = video_type_codes.get(data["aweme_type"], VideoType.VIDEO)
+    if video_type == VideoType.ALBUM:
         images_list = []
         for images in data["image_post_info"]["images"]:
             images_list.append(images["display_image"]["url_list"][0])
-        media = Album(images_url=images_list)
+        media = Album(urls=images_list)
     else:
-        media = Video(video_url=data["video"]["play_addr"]["url_list"][0])
+        media = Video(url=data["video"]["play_addr"]["url_list"][0])
+    author_data = data.get("author")
+    author = Author(
+        id=author_data.get("id"),
+        nickname=author_data.get("nickname"),
+        unique_id=author_data.get("unique_id"),
+        avatar=author_data.get("avatar_larger", {}).get("url_list")[0],
+    )
     return VideoData(
-        status="success",
         video_type=video_type,
         media=media,
         cover=data["video"]["cover"]["url_list"][0],
         dynamic_cover=data["video"]["dynamic_cover"]["url_list"][0],
         description=data["desc"],
         play_count=data["statistics"]["comment_count"],
         comment_count=data["statistics"]["comment_count"],
         download_count=data["statistics"]["download_count"],
         share_count=data["statistics"]["share_count"],
         create_time=data["create_time"],
-        author_name=data["author"]["nickname"],
-        author_nick=data["author"]["unique_id"],
-        author_pic=data["author"]["avatar_medium"]["url_list"][0],
+        author=author,
         music_title=data["music"]["title"],
         music_author=data["music"]["author"],
         music_url=data["music"]["play_url"]["uri"],
         music_cover=data["music"]["cover_large"]["url_list"][0],
     )
 
 
-def extract_user_feed(data: str):
+def extract_data_from_html(data: str):
     pattern = r'<script id="SIGI_STATE" type="application\/json">(.*?)<\/script>'
     match = re.search(pattern, data, re.S)
     return json.loads(match.group(1))
+
+
+def extract_user_data(data: dict):
+    user_data = list(data.get("UserModule", {}).get("users", {}).values())[0]
+    return Author(
+        id=user_data.get("id"),
+        unique_id=user_data.get("uniqueId"),
+        nickname=user_data.get("nickname"),
+        sec_uid=user_data.get("secUid"),
+        avatar=user_data.get("avatarLarger"),
+    )
```

#### html2text {}

 * *error from `html2text {}`:*

 * *File "/tmp/diffoscope_bugnq2_w_/tmp_r2yijh0_TarContainer/0/3.py", line 52, column 0: CDATA terminal not found*

 * *File "/tmp/diffoscope_bugnq2_w_/tmp_r2yijh0_TarContainer/0/3.py", line 52, column 0: CDATA terminal not found*

```diff
@@ -1,20 +1,19 @@
-import json import re from .types import Album, Video, VideoData
-video_type_codes = { 0: "video", 51: "video", 55: "video", 58: "video", 61:
-"video", 150: "album", } def extract_video_data(data: dict) -> VideoData:
-video_type_code = data["aweme_type"] video_type = video_type_codes.get
-(video_type_code, "video") if video_type == "album": images_list = [] for
-images in data["image_post_info"]["images"]: images_list.append(images
-["display_image"]["url_list"][0]) media = Album(images_url=images_list) else:
-media = Video(video_url=data["video"]["play_addr"]["url_list"][0]) return
-VideoData( status="success", video_type=video_type, media=media, cover=data
-["video"]["cover"]["url_list"][0], dynamic_cover=data["video"]["dynamic_cover"]
-["url_list"][0], description=data["desc"], play_count=data["statistics"]
-["comment_count"], comment_count=data["statistics"]["comment_count"],
-download_count=data["statistics"]["download_count"], share_count=data
-["statistics"]["share_count"], create_time=data["create_time"],
-author_name=data["author"]["nickname"], author_nick=data["author"]
-["unique_id"], author_pic=data["author"]["avatar_medium"]["url_list"][0],
-music_title=data["music"]["title"], music_author=data["music"]["author"],
-music_url=data["music"]["play_url"]["uri"], music_cover=data["music"]
-["cover_large"]["url_list"][0], ) def extract_user_feed(data: str): pattern =
-r'
+import json import re from .types import Album, Author, Video, VideoData,
+VideoType, video_type_codes def extract_video_data(data: dict) -> VideoData:
+video_type = video_type_codes.get(data["aweme_type"], VideoType.VIDEO) if
+video_type == VideoType.ALBUM: images_list = [] for images in data
+["image_post_info"]["images"]: images_list.append(images["display_image"]
+["url_list"][0]) media = Album(urls=images_list) else: media = Video(url=data
+["video"]["play_addr"]["url_list"][0]) author_data = data.get("author") author
+= Author( id=author_data.get("id"), nickname=author_data.get("nickname"),
+unique_id=author_data.get("unique_id"), avatar=author_data.get("avatar_larger",
+{}).get("url_list")[0], ) return VideoData( video_type=video_type, media=media,
+cover=data["video"]["cover"]["url_list"][0], dynamic_cover=data["video"]
+["dynamic_cover"]["url_list"][0], description=data["desc"], play_count=data
+["statistics"]["comment_count"], comment_count=data["statistics"]
+["comment_count"], download_count=data["statistics"]["download_count"],
+share_count=data["statistics"]["share_count"], create_time=data["create_time"],
+author=author, music_title=data["music"]["title"], music_author=data["music"]
+["author"], music_url=data["music"]["play_url"]["uri"], music_cover=data
+["music"]["cover_large"]["url_list"][0], ) def extract_data_from_html(data:
+str): pattern = r'
```

### Comparing `aiotiktok-2.5.4/.gitignore` & `aiotiktok-2.6/.gitignore`

 * *Files identical despite different names*

### Comparing `aiotiktok-2.5.4/LICENSE` & `aiotiktok-2.6/LICENSE`

 * *Files identical despite different names*

### Comparing `aiotiktok-2.5.4/pyproject.toml` & `aiotiktok-2.6/pyproject.toml`

 * *Files identical despite different names*

