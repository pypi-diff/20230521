# Comparing `tmp/videosrc-0.1.7-py3-none-any.whl.zip` & `tmp/videosrc-0.1.8-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,29 +1,30 @@
-Zip file size: 91788 bytes, number of entries: 27
+Zip file size: 92132 bytes, number of entries: 28
 -rw-rw-r--  2.0 unx      311 b- defN 23-May-12 19:55 tests/__init__.py
 -rw-rw-r--  2.0 unx     2862 b- defN 23-May-17 02:05 tests/test_html.py
 -rw-rw-r--  2.0 unx     6475 b- defN 23-May-17 02:05 tests/test_mrss.py
 -rw-rw-r--  2.0 unx    34252 b- defN 23-May-17 02:12 tests/test_odysee.py
 -rw-rw-r--  2.0 unx    29900 b- defN 23-May-14 05:44 tests/test_peertube.py
 -rw-rw-r--  2.0 unx    76475 b- defN 23-May-14 05:44 tests/test_rumble.py
 -rw-rw-r--  2.0 unx   191646 b- defN 23-May-14 05:44 tests/test_timcast.py
 -rw-rw-r--  2.0 unx     1112 b- defN 23-May-14 20:05 tests/test_twitter.py
--rw-rw-r--  2.0 unx     1685 b- defN 23-May-20 19:55 videosrc/__init__.py
+-rw-rw-r--  2.0 unx     1771 b- defN 23-May-21 16:10 videosrc/__init__.py
 -rw-rw-r--  2.0 unx     1812 b- defN 23-May-15 15:31 videosrc/__main__.py
 -rw-rw-r--  2.0 unx      189 b- defN 23-May-14 21:39 videosrc/errors.py
 -rw-rw-r--  2.0 unx     5296 b- defN 23-May-15 15:50 videosrc/utils.py
 -rw-rw-r--  2.0 unx      500 b- defN 23-May-11 21:33 videosrc/crawlers/__init__.py
 -rw-rw-r--  2.0 unx     2256 b- defN 23-May-17 02:04 videosrc/crawlers/base.py
 -rw-rw-r--  2.0 unx     3565 b- defN 23-May-17 02:02 videosrc/crawlers/html.py
 -rw-rw-r--  2.0 unx     6869 b- defN 23-May-17 01:59 videosrc/crawlers/mrss.py
--rw-rw-r--  2.0 unx    12880 b- defN 23-May-17 02:12 videosrc/crawlers/odysee.py
+-rw-rw-r--  2.0 unx    12992 b- defN 23-May-21 16:04 videosrc/crawlers/odysee.py
 -rw-rw-r--  2.0 unx     5709 b- defN 23-May-17 02:02 videosrc/crawlers/peertube.py
--rw-rw-r--  2.0 unx     3804 b- defN 23-May-15 14:56 videosrc/crawlers/rumble.py
--rw-rw-r--  2.0 unx     6783 b- defN 23-May-17 02:02 videosrc/crawlers/timcast.py
--rw-rw-r--  2.0 unx     3121 b- defN 23-May-15 14:41 videosrc/crawlers/twitter.py
+-rw-rw-r--  2.0 unx     3928 b- defN 23-May-21 16:04 videosrc/crawlers/rumble.py
+-rw-rw-r--  2.0 unx     6903 b- defN 23-May-21 16:04 videosrc/crawlers/timcast.py
+-rw-rw-r--  2.0 unx     3379 b- defN 23-May-21 16:07 videosrc/crawlers/twitter.py
+-rw-rw-r--  2.0 unx        0 b- defN 23-May-21 16:09 videosrc/crawlers/youtube.py
 -rw-rw-r--  2.0 unx      626 b- defN 23-May-14 05:19 videosrc/models/__init__.py
--rw-rw-r--  2.0 unx     1066 b- defN 23-May-20 20:05 videosrc-0.1.7.dist-info/LICENSE
--rw-rw-r--  2.0 unx     2011 b- defN 23-May-20 20:05 videosrc-0.1.7.dist-info/METADATA
--rw-rw-r--  2.0 unx       92 b- defN 23-May-20 20:05 videosrc-0.1.7.dist-info/WHEEL
--rw-rw-r--  2.0 unx       15 b- defN 23-May-20 20:05 videosrc-0.1.7.dist-info/top_level.txt
--rw-rw-r--  2.0 unx     2149 b- defN 23-May-20 20:05 videosrc-0.1.7.dist-info/RECORD
-27 files, 403461 bytes uncompressed, 88382 bytes compressed:  78.1%
+-rw-rw-r--  2.0 unx     1066 b- defN 23-May-21 16:10 videosrc-0.1.8.dist-info/LICENSE
+-rw-rw-r--  2.0 unx     2044 b- defN 23-May-21 16:10 videosrc-0.1.8.dist-info/METADATA
+-rw-rw-r--  2.0 unx       92 b- defN 23-May-21 16:10 videosrc-0.1.8.dist-info/WHEEL
+-rw-rw-r--  2.0 unx       15 b- defN 23-May-21 16:10 videosrc-0.1.8.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx     2231 b- defN 23-May-21 16:10 videosrc-0.1.8.dist-info/RECORD
+28 files, 404276 bytes uncompressed, 88594 bytes compressed:  78.1%
```

## zipnote {}

```diff
@@ -57,26 +57,29 @@
 
 Filename: videosrc/crawlers/timcast.py
 Comment: 
 
 Filename: videosrc/crawlers/twitter.py
 Comment: 
 
+Filename: videosrc/crawlers/youtube.py
+Comment: 
+
 Filename: videosrc/models/__init__.py
 Comment: 
 
-Filename: videosrc-0.1.7.dist-info/LICENSE
+Filename: videosrc-0.1.8.dist-info/LICENSE
 Comment: 
 
-Filename: videosrc-0.1.7.dist-info/METADATA
+Filename: videosrc-0.1.8.dist-info/METADATA
 Comment: 
 
-Filename: videosrc-0.1.7.dist-info/WHEEL
+Filename: videosrc-0.1.8.dist-info/WHEEL
 Comment: 
 
-Filename: videosrc-0.1.7.dist-info/top_level.txt
+Filename: videosrc-0.1.8.dist-info/top_level.txt
 Comment: 
 
-Filename: videosrc-0.1.7.dist-info/RECORD
+Filename: videosrc-0.1.8.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## videosrc/__init__.py

```diff
@@ -24,16 +24,20 @@
     return crawlers
 
 
 async def login(url, **kwargs):
     init_kwargs = {
         'state': kwargs.pop('state', None),
         'save_state': kwargs.pop('save_state', None),
-        'proxy': kwargs.pop('proxy', None),
-    }    
+    }
+    try:
+        init_kwargs['proxy'] = kwargs['proxy']
+
+    except KeyError:
+        pass
 
     crawler_klass = detect_crawler(url)[0]
     crawler = crawler_klass(**init_kwargs)
 
     try:
         return await crawler.login(url, **kwargs)
 
@@ -41,16 +45,20 @@
         raise AuthenticationError('Failure logging in')
 
 
 async def crawl(url, **kwargs):
     init_kwargs = {
         'state': kwargs.pop('state', None),
         'save_state': kwargs.pop('save_state', None),
-        'proxy': kwargs.pop('proxy', None),
-    }    
+    }
+    try:
+        init_kwargs['proxy'] = kwargs['proxy']
+
+    except KeyError:
+        pass
 
     crawler_klass = detect_crawler(url)[0]
     crawler = crawler_klass(**init_kwargs)
 
     return await crawler.crawl(url, **kwargs)
```

## videosrc/crawlers/odysee.py

```diff
@@ -279,15 +279,16 @@
                 try:
                     yield video
 
                 except Exception as e:
                     LOGGER.exception(e)
 
                 else:
-                    self._state = published
+                    self._state = max(self._state, published) if self._state \
+                                                              else published
 
             if len(items) + 1 < PAGE_SIZE:
                 break
 
             page_number += 1
 
     async def crawl(self, url, **kwargs):
```

## videosrc/crawlers/rumble.py

```diff
@@ -52,19 +52,20 @@
 class RumbleCrawler(Crawler):
     @staticmethod
     def check_url(url):
         urlp = urlparse(url)
         return urlp.netloc.endswith('rumble.com')
 
     async def _iter_videos(self, url, page):
+        state = self._state
         for li in page.find_all('li', class_='video-listing-entry'):
             url = urljoin(url, li.article.a['href'])
             video_details = await get_video_details(url, proxy=self._proxy)
             published = parse_date(video_details['pubDate'])
-            if self._state and self._state > published:
+            if state and state > published:
                 LOGGER.info('Video published before given state')
                 break
             sources = [
                 self.VideoSourceModel(
                     extern_id=md5sum(src['url']),
                     width=src['meta']['w'],
                     height=src['meta']['h'],
@@ -87,15 +88,16 @@
             try:
                 yield video
 
             except Exception as e:
                 LOGGER.exception(e)
 
             else:
-                self._state = published
+                self._state = max(self._state, published) if self._state \
+                                                          else published
 
     async def crawl(self, url, **kwargs):
         # https://rumble.com/user/vivafrei
         urlp = urlparse(url)
         pparts = pathsplit(urlp.path.strip('/'))
 
         async with ScraperSession() as s:
```

## videosrc/crawlers/timcast.py

```diff
@@ -124,14 +124,15 @@
 
                 LOGGER.exception('Login failed, retrying')
                 time.sleep(3 ** i)
 
     async def _iter_videos(self, url, page):
         grid = page.find(
             'div', class_='t-grid:s:fit:2 t-grid:m:fit:4 t-pad:25pc:top')
+        state = self._state
         for article in grid.find_all('div', class_='article'):
             video_link = article.find('a', class_='image')
             thumbnail = video_link.img['src']
             description = video_link.img['alt']
             video_page_url = video_link['href']
             video_page_url = urljoin(url, urlparse(video_page_url).path)
             async with ScraperSession() as s:
@@ -141,15 +142,15 @@
                     'html.parser')
             iframe_tag = video_page.find('iframe')
             embed_url = iframe_tag['src']
             video_details = await get_embed_details(
                 embed_url, proxy=self._proxy)
             pubDate = parse_date(video_details['pubDate'])
 
-            if self._state and pubDate < self._state:
+            if state and pubDate < state:
                 LOGGER.info('Video published before last state %s', pubDate)
                 return
 
             sources = [
                 self.VideoSourceModel(
                     extern_id=md5sum(src['url']),
                     width=src['meta']['w'],
@@ -173,15 +174,16 @@
             try:
                 yield video
 
             except Exception as e:
                 LOGGER.exception(e)
 
             else:
-                self._state = pubDate
+                self._state = max(self._state, pubDate) if self._state \
+                                                        else pubDate
 
     async def _iter_pages(self, url, page):
         page_num = 1
         async with ScraperSession() as s:
             while True:
                 LOGGER.debug('Scraping page %i', page_num)
                 async for video in self._iter_videos(url, page):
```

## videosrc/crawlers/twitter.py

```diff
@@ -21,22 +21,28 @@
 
     @staticmethod
     def check_url(url):
         urlp = urlparse(url)
         return urlp.netloc.endswith('twitter.com')
 
     async def _iter_videos(self, url, items, max_count=100, max_days=None):
+        state = self._state
         for item in items:
             try:
                 media = item.media[0]
             except (TypeError, IndexError):
                 continue
+
             if not isinstance(media, sntwitter.Video):
                 continue
 
+            if state and item.id < state:
+                LOGGER.info('Video published before last state %i', state)
+                continue
+
             sources = []
             for variant in media.variants:
                 with MediaInfo(variant.url) as info:
                     sources.append(self.VideoSourceModel(
                         extern_id=md5sum(variant.url),
                         width=info.width,
                         height=info.height,
@@ -68,15 +74,16 @@
             try:
                 yield video
 
             except Exception as e:
                 LOGGER.exception(e)
 
             else:
-                self._state = max(item.id, self._state)
+                self._state = max(self._state, item.id) if self._state \
+                                                        else item.id
 
     # https://twitter.com/MattWalshShow
     async def crawl(self, url, **kwargs):
         # Parse name from URL
         name = urlparse(url).path.strip('/')
         proxies = {}
         if self._proxy:
```

## Comparing `videosrc-0.1.7.dist-info/LICENSE` & `videosrc-0.1.8.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `videosrc-0.1.7.dist-info/METADATA` & `videosrc-0.1.8.dist-info/METADATA`

 * *Files 8% similar despite different names*

```diff
@@ -1,22 +1,23 @@
 Metadata-Version: 2.1
 Name: videosrc
-Version: 0.1.7
+Version: 0.1.8
 Summary: Video src crawler
 Home-page: https://github.com/btimby/cesium.tv/vidsrc/
 Author: Ben Timby
 Author-email: btimby@gmail.com
 License-File: LICENSE
 Requires-Dist: aiohttp-scraper (==0.1.4)
 Requires-Dist: pyppeteer (==1.0.2)
 Requires-Dist: beautifulsoup4 (==4.10.0)
 Requires-Dist: requests (==2.25.1)
 Requires-Dist: av (==9.2.0)
 Requires-Dist: snscrape (==0.6.2.20230320)
 Requires-Dist: Pillow (==9.5.0)
+Requires-Dist: pytube (==15.0.0)
 Provides-Extra: dev
 Requires-Dist: flake8 ; extra == 'dev'
 Requires-Dist: responses-server ; extra == 'dev'
 
 ********
 videosrc
 ********
```

## Comparing `videosrc-0.1.7.dist-info/RECORD` & `videosrc-0.1.8.dist-info/RECORD`

 * *Files 26% similar despite different names*

```diff
@@ -2,26 +2,27 @@
 tests/test_html.py,sha256=Lr_IPVetCznEEU_pIF6KkOy5rS6bFV3aBk8CNcB29BU,2862
 tests/test_mrss.py,sha256=IL1VFvg9dUBiaXW7fPHrWgrUxMBkD5HtH9yNgY-6yl4,6475
 tests/test_odysee.py,sha256=yI7yiUwM5YQH_LuvtG27vhl3HSDQDfUSPdOhdIn7WX8,34252
 tests/test_peertube.py,sha256=AwZnrBoY7ZYlWw92h_4A6vrUmE9i66d998mSnhZ9MT8,29900
 tests/test_rumble.py,sha256=dsY5hrNijIZ5JAP6VBaEdhslahqyDvvz5UAHrP2S2AA,76475
 tests/test_timcast.py,sha256=a_yzZcI_P-PlhQNzvc2EUX2mmsMvJrW7C0T267mOVQI,191646
 tests/test_twitter.py,sha256=NyxGIzYw6ge6AdNuQZbCibZec1F10xqKlDeXyhXTW7w,1112
-videosrc/__init__.py,sha256=kw3tNEbF5DeKIxwdHlNjo5RyyL-6SliFEiIWZiqBKr4,1685
+videosrc/__init__.py,sha256=p1SmdzmXof5Xq3XJZmFBz5CMBOTm0ltlzhhfV7eHg0o,1771
 videosrc/__main__.py,sha256=6SpxV8YXkwM5Tmq4YCJxqQF5aXTHCR0oTY9ISFiKCVg,1812
 videosrc/errors.py,sha256=4TuFGWdjaBKSzzUglz05x4VLHos9AjTm6_IodWrm_2M,189
 videosrc/utils.py,sha256=mQos14ZTZuXioRc1GtLcnMFAWX1u82qxgkGr9M7Q5zk,5296
 videosrc/crawlers/__init__.py,sha256=tEwn_Q7xIYuXhUP9t-CFqM8WPwEP_2n6v8s9FuaHwE4,500
 videosrc/crawlers/base.py,sha256=OIoZfmIkF8qVOYkdBBh1gRRCsMHLpVP_6EiDb-dG638,2256
 videosrc/crawlers/html.py,sha256=-AOjNEfGI4THK4OMfVwlG3K17HVa1ctMZoM3sBHOFwI,3565
 videosrc/crawlers/mrss.py,sha256=cwmzIoJApoAhkSMNgYO4OFYS-b5-wwRfFtFzLGWB6dY,6869
-videosrc/crawlers/odysee.py,sha256=fR5UebO9H8hodm0hUmSunLraxbVSxJ_SSjSGUQ-oUTs,12880
+videosrc/crawlers/odysee.py,sha256=7K3eHnlwCsJw3QG4oEhfM24nG8o81kBTa4b4Wy-r5LU,12992
 videosrc/crawlers/peertube.py,sha256=ndNjyZBGkgN6_w1PYdcAWqb54Yu5umllLQS4coCp3S8,5709
-videosrc/crawlers/rumble.py,sha256=_sYRANtT-vd3aoKx4krmLxlYE08WLqVb3KbtWTUcxPQ,3804
-videosrc/crawlers/timcast.py,sha256=JF4EKj3F4gfkAy-WpyopUQgpeSNXtzFlRFM3rky9ADQ,6783
-videosrc/crawlers/twitter.py,sha256=MGcv_D6EOJKqBz2VU-CQOn0ZnPZPhD1swVYZ-hIEkG4,3121
+videosrc/crawlers/rumble.py,sha256=4vkcqg-BJDbvrPLGKwObp1vDWYT10J7DSnhMj-9afzc,3928
+videosrc/crawlers/timcast.py,sha256=zTA_PxKBNYp_CrWO7vIqZ54OU4G3fNL3D3dYuoPhd2o,6903
+videosrc/crawlers/twitter.py,sha256=2a5NGn7wZ0142brzk-ANBQ7St_M8_pWIRgxdBCbcsNE,3379
+videosrc/crawlers/youtube.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 videosrc/models/__init__.py,sha256=33PwZuf3LbSS1FZSVq-RVn2PbejFASLIItv005ixce4,626
-videosrc-0.1.7.dist-info/LICENSE,sha256=ZrmE4LhjnartZCuclnrGM1kWT3L1WxtXC84vnHMOxTc,1066
-videosrc-0.1.7.dist-info/METADATA,sha256=vxpCvj6mI7kUfjSZEVkXEyML13iMKEmSTiA5E0vhQMs,2011
-videosrc-0.1.7.dist-info/WHEEL,sha256=pkctZYzUS4AYVn6dJ-7367OJZivF2e8RA9b_ZBjif18,92
-videosrc-0.1.7.dist-info/top_level.txt,sha256=GVj7Kn2EZJ5LjJjdb6uJtVlPu5yaZ8MjWnmK76wRyAk,15
-videosrc-0.1.7.dist-info/RECORD,,
+videosrc-0.1.8.dist-info/LICENSE,sha256=ZrmE4LhjnartZCuclnrGM1kWT3L1WxtXC84vnHMOxTc,1066
+videosrc-0.1.8.dist-info/METADATA,sha256=zujIQfgEW_R_CBDT0RWzXKTkGRUVb91uAemXAFFplNw,2044
+videosrc-0.1.8.dist-info/WHEEL,sha256=pkctZYzUS4AYVn6dJ-7367OJZivF2e8RA9b_ZBjif18,92
+videosrc-0.1.8.dist-info/top_level.txt,sha256=GVj7Kn2EZJ5LjJjdb6uJtVlPu5yaZ8MjWnmK76wRyAk,15
+videosrc-0.1.8.dist-info/RECORD,,
```

