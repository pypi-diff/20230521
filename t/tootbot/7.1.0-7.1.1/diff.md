# Comparing `tmp/tootbot-7.1.0.tar.gz` & `tmp/tootbot-7.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tootbot-7.1.0.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
+gzip compressed data, was "tootbot-7.1.1.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `tootbot-7.1.0.tar` & `tootbot-7.1.1.tar`

### file list

```diff
@@ -1,11 +1,11 @@
--rw-r--r--   0        0        0     4489 2023-05-20 04:42:27.706811 tootbot-7.1.0/README.rst
--rw-r--r--   0        0        0     3833 2023-05-20 04:42:27.714810 tootbot-7.1.0/pyproject.toml
--rw-r--r--   0        0        0      752 2023-05-20 04:42:27.714810 tootbot-7.1.0/src/tootbot/__init__.py
--rw-r--r--   0        0        0     7645 2023-05-20 04:42:27.714810 tootbot-7.1.0/src/tootbot/app.py
--rw-r--r--   0        0        0    31577 2023-05-20 04:42:27.714810 tootbot-7.1.0/src/tootbot/collect.py
--rw-r--r--   0        0        0    18239 2023-05-20 04:42:27.714810 tootbot-7.1.0/src/tootbot/control.py
--rw-r--r--   0        0        0     4774 2023-05-20 04:42:27.714810 tootbot-7.1.0/src/tootbot/create_config.py
--rw-r--r--   0        0        0     4466 2023-05-20 04:42:27.714810 tootbot-7.1.0/src/tootbot/debug.py
--rw-r--r--   0        0        0     2472 2023-05-20 04:42:27.714810 tootbot-7.1.0/src/tootbot/monitoring.py
--rw-r--r--   0        0        0    16491 2023-05-20 04:42:27.714810 tootbot-7.1.0/src/tootbot/publish.py
--rw-r--r--   0        0        0     6316 1970-01-01 00:00:00.000000 tootbot-7.1.0/PKG-INFO
+-rw-r--r--   0        0        0     4489 2023-05-21 07:37:02.157318 tootbot-7.1.1/README.rst
+-rw-r--r--   0        0        0     3833 2023-05-21 07:37:02.161318 tootbot-7.1.1/pyproject.toml
+-rw-r--r--   0        0        0      752 2023-05-21 07:37:02.161318 tootbot-7.1.1/src/tootbot/__init__.py
+-rw-r--r--   0        0        0     7645 2023-05-21 07:37:02.161318 tootbot-7.1.1/src/tootbot/app.py
+-rw-r--r--   0        0        0    31019 2023-05-21 07:37:02.161318 tootbot-7.1.1/src/tootbot/collect.py
+-rw-r--r--   0        0        0    18239 2023-05-21 07:37:02.161318 tootbot-7.1.1/src/tootbot/control.py
+-rw-r--r--   0        0        0     4766 2023-05-21 07:37:02.161318 tootbot-7.1.1/src/tootbot/create_config.py
+-rw-r--r--   0        0        0     4466 2023-05-21 07:37:02.161318 tootbot-7.1.1/src/tootbot/debug.py
+-rw-r--r--   0        0        0     2472 2023-05-21 07:37:02.161318 tootbot-7.1.1/src/tootbot/monitoring.py
+-rw-r--r--   0        0        0    16491 2023-05-21 07:37:02.161318 tootbot-7.1.1/src/tootbot/publish.py
+-rw-r--r--   0        0        0     6316 1970-01-01 00:00:00.000000 tootbot-7.1.1/PKG-INFO
```

### Comparing `tootbot-7.1.0/README.rst` & `tootbot-7.1.1/README.rst`

 * *Files identical despite different names*

### Comparing `tootbot-7.1.0/pyproject.toml` & `tootbot-7.1.1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `tootbot-7.1.0/src/tootbot/__init__.py` & `tootbot-7.1.1/src/tootbot/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 """Package 'tootbot' level definitions."""
 import sys
 from typing import Final
 
-__version__: Final[str] = "7.1.0"
+__version__: Final[str] = "7.1.1"
 __display_name__: Final[str] = "Tootbot"
 __package_name__: Final[str] = __display_name__.lower()
 
 # Package level Static Variables
 POST_RECORDER_SQLITE_DB: Final[str] = "history.db"
 POST_RECORDER_HISTORY_RETENTION_DAYS: Final[int] = 31
 USER_AGENT: Final[str] = __display_name__
```

### Comparing `tootbot-7.1.0/src/tootbot/app.py` & `tootbot-7.1.1/src/tootbot/app.py`

 * *Files identical despite different names*

### Comparing `tootbot-7.1.0/src/tootbot/collect.py` & `tootbot-7.1.1/src/tootbot/collect.py`

 * *Files 2% similar despite different names*

```diff
@@ -206,15 +206,15 @@
 
         await reddit_con.close()
 
     async def get_reddit_posts(
         self: RH,
         subreddit: SubredditConfig,
         reddit_con: asyncpraw.Reddit,
-    ) -> Dict[str, asyncpraw.models.Submission]:
+    ) -> Dict[str, Dict[str, asyncpraw.models.Submission]]:
         """Collect posts considered hot from configured sub/multi-reddits.
 
         :param subreddit: subreddits to check for posts to x-post
         :param reddit_con: API reference
 
         :returns:
         Dictionary with str of tags to use and subreddit posts
@@ -377,23 +377,26 @@
                 client_id=imgur_secrets.client_id,
                 client_secret=imgur_secrets.client_secret,
             )
 
             logger.debug(
                 "Imgur rate limiting information: %s", self.imgur_client.credits
             )
-            reset_epoch = self.imgur_client.credits.get("UserReset")
+            try:
+                reset_epoch = int(self.imgur_client.credits.get("UserReset"))
+            except (ValueError, TypeError):
+                reset_epoch = None
             if reset_epoch:
                 reset_at = arrow.get(reset_epoch).format("YYYY-MM-DD HH:mm:ss")
                 reset_in = arrow.get(reset_epoch).humanize()
                 logger.debug("Imgur rate limit resetting %s at %s", reset_in, reset_at)
         except ImgurClientRateLimitError as rate_limited:
             logger.error("Hit ratelimit at imgur: %s", rate_limited)
 
-    async def get_attachments(  # noqa: C901
+    async def get_attachments(
         self: LMH,
         reddit_post: Submission,
     ) -> List[Attachment]:
         """Determine which method to call depending on which site the media_url is pointing to.
 
         :returns:
         list of Attachment objects
@@ -415,20 +418,14 @@
             )
         elif "v.redd.it" in reddit_post.url:
             single_attachment = await self.get_reddit_video(reddit_post)
 
         elif "imgur.com" in reddit_post.url:
             multiple_attachments = await self.get_imgur_image(reddit_post.url)
 
-        # Todo: Gfycat might be defunct and might soon need to be removed
-        elif "gfycat.com" in reddit_post.url:
-            single_attachment = await LinkedMediaHelper.get_gfycat_image(
-                reddit_post.url
-            )
-
         elif "giphy.com" in reddit_post.url:
             single_attachment = await LinkedMediaHelper.get_giphy_image(reddit_post.url)
 
         elif "reddit.com/gallery/" in reddit_post.url:  # Need to check for gallery post
             if hasattr(reddit_post, "is_gallery"):
                 logger.debug("%s is a gallery post", reddit_post.id)
                 multiple_attachments = await LinkedMediaHelper.get_reddit_gallery(
@@ -571,42 +568,30 @@
             else:  # Single image
                 imgur_img = self.imgur_client.get_image(imgur_id)
                 image_urls = [imgur_img.link]  # pylint: disable=no-member
 
             logger.debug(
                 "Imgur rate limiting information: %s", self.imgur_client.credits
             )
-            reset_epoch = self.imgur_client.credits.get("UserReset")
+            try:
+                reset_epoch = int(self.imgur_client.credits.get("UserReset"))
+            except (ValueError, TypeError):
+                reset_epoch = None
             if reset_epoch:
                 reset_at = arrow.get(reset_epoch).format("YYYY-MM-DD HH:mm:ss")
                 reset_in = arrow.get(reset_epoch).humanize()
                 logger.debug("Imgur rate limit resetting %s at %s", reset_in, reset_at)
 
         except ImgurClientError as imgur_error:
             logger.error("Could not get information from imgur: %s", imgur_error)
         except ImgurClientRateLimitError as rate_limited:
             logger.error("Hit ratelimit at imgur: %s", rate_limited)
             logger.debug("Imgur Rate Limits: %s", self.imgur_client.credits)
         return image_urls
 
-    # Todo: Gfycat might be defunct and might soon need to be removed
-    @staticmethod
-    async def get_gfycat_image(img_url: str) -> Optional[Attachment]:
-        """Download full resolution images from gfycat.
-
-        :param img_url: url of gfycat image to download
-
-        :returns:
-        Attachment or None
-        """
-        logger.debug("LinkedMediaHelper.get_gfycat_image(img_url=%s)", img_url)
-
-        attachment = await LinkedMediaHelper._get_video_with_yt_dlp(video_url=img_url)
-        return attachment
-
     @staticmethod
     async def get_reddit_image(img_url: str) -> Optional[Attachment]:
         """Download full resolution images from i.reddit or reddituploads.com.
 
         :param img_url: url of imgur image to download
 
         :returns:
```

### Comparing `tootbot-7.1.0/src/tootbot/control.py` & `tootbot-7.1.1/src/tootbot/control.py`

 * *Files identical despite different names*

### Comparing `tootbot-7.1.0/src/tootbot/create_config.py` & `tootbot-7.1.1/src/tootbot/create_config.py`

 * *Files 1% similar despite different names*

```diff
@@ -75,15 +75,15 @@
 UUID :
 
 # Settings related to media attachments
 [MediaSettings]
 # Folder name for media downloads (default is 'media')
 MediaFolder: media
 # Set the bot to only post Reddit posts that directly link to media
-# Links from Gfycat, Giphy, Imgur, i.redd.it, and i.reddituploads.com are
+# Links from Giphy, Imgur, i.redd.it, and i.reddituploads.com are
 # currently supported
 MediaPostsOnly: false
 
 # Mastodon settings
 [Mastodon]
 # Name of instance to log into (example: mastodon.social). This is mandatory
 InstanceDomain :
```

### Comparing `tootbot-7.1.0/src/tootbot/debug.py` & `tootbot-7.1.1/src/tootbot/debug.py`

 * *Files identical despite different names*

### Comparing `tootbot-7.1.0/src/tootbot/monitoring.py` & `tootbot-7.1.1/src/tootbot/monitoring.py`

 * *Files identical despite different names*

### Comparing `tootbot-7.1.0/src/tootbot/publish.py` & `tootbot-7.1.1/src/tootbot/publish.py`

 * *Files identical despite different names*

### Comparing `tootbot-7.1.0/PKG-INFO` & `tootbot-7.1.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tootbot
-Version: 7.1.0
+Version: 7.1.1
 Summary: A Python bot that looks up posts from specified subreddits and automatically posts them on Mastodon
 Author-email: marvin8 <marvin8@tuta.io>
 Requires-Python: >=3.8
 Description-Content-Type: text/x-rst
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
 Classifier: Environment :: Console
```

