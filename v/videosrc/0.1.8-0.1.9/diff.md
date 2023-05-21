# Comparing `tmp/videosrc-0.1.8-py3-none-any.whl.zip` & `tmp/videosrc-0.1.9-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,8 +1,8 @@
-Zip file size: 92132 bytes, number of entries: 28
+Zip file size: 92241 bytes, number of entries: 28
 -rw-rw-r--  2.0 unx      311 b- defN 23-May-12 19:55 tests/__init__.py
 -rw-rw-r--  2.0 unx     2862 b- defN 23-May-17 02:05 tests/test_html.py
 -rw-rw-r--  2.0 unx     6475 b- defN 23-May-17 02:05 tests/test_mrss.py
 -rw-rw-r--  2.0 unx    34252 b- defN 23-May-17 02:12 tests/test_odysee.py
 -rw-rw-r--  2.0 unx    29900 b- defN 23-May-14 05:44 tests/test_peertube.py
 -rw-rw-r--  2.0 unx    76475 b- defN 23-May-14 05:44 tests/test_rumble.py
 -rw-rw-r--  2.0 unx   191646 b- defN 23-May-14 05:44 tests/test_timcast.py
@@ -14,17 +14,17 @@
 -rw-rw-r--  2.0 unx      500 b- defN 23-May-11 21:33 videosrc/crawlers/__init__.py
 -rw-rw-r--  2.0 unx     2256 b- defN 23-May-17 02:04 videosrc/crawlers/base.py
 -rw-rw-r--  2.0 unx     3565 b- defN 23-May-17 02:02 videosrc/crawlers/html.py
 -rw-rw-r--  2.0 unx     6869 b- defN 23-May-17 01:59 videosrc/crawlers/mrss.py
 -rw-rw-r--  2.0 unx    12992 b- defN 23-May-21 16:04 videosrc/crawlers/odysee.py
 -rw-rw-r--  2.0 unx     5709 b- defN 23-May-17 02:02 videosrc/crawlers/peertube.py
 -rw-rw-r--  2.0 unx     3928 b- defN 23-May-21 16:04 videosrc/crawlers/rumble.py
--rw-rw-r--  2.0 unx     6903 b- defN 23-May-21 16:04 videosrc/crawlers/timcast.py
+-rw-rw-r--  2.0 unx     7064 b- defN 23-May-21 16:50 videosrc/crawlers/timcast.py
 -rw-rw-r--  2.0 unx     3379 b- defN 23-May-21 16:07 videosrc/crawlers/twitter.py
--rw-rw-r--  2.0 unx        0 b- defN 23-May-21 16:09 videosrc/crawlers/youtube.py
+-rw-rw-r--  2.0 unx       85 b- defN 23-May-21 16:18 videosrc/crawlers/youtube.py
 -rw-rw-r--  2.0 unx      626 b- defN 23-May-14 05:19 videosrc/models/__init__.py
--rw-rw-r--  2.0 unx     1066 b- defN 23-May-21 16:10 videosrc-0.1.8.dist-info/LICENSE
--rw-rw-r--  2.0 unx     2044 b- defN 23-May-21 16:10 videosrc-0.1.8.dist-info/METADATA
--rw-rw-r--  2.0 unx       92 b- defN 23-May-21 16:10 videosrc-0.1.8.dist-info/WHEEL
--rw-rw-r--  2.0 unx       15 b- defN 23-May-21 16:10 videosrc-0.1.8.dist-info/top_level.txt
--rw-rw-r--  2.0 unx     2231 b- defN 23-May-21 16:10 videosrc-0.1.8.dist-info/RECORD
-28 files, 404276 bytes uncompressed, 88594 bytes compressed:  78.1%
+-rw-rw-r--  2.0 unx     1066 b- defN 23-May-21 16:54 videosrc-0.1.9.dist-info/LICENSE
+-rw-rw-r--  2.0 unx     2039 b- defN 23-May-21 16:54 videosrc-0.1.9.dist-info/METADATA
+-rw-rw-r--  2.0 unx       92 b- defN 23-May-21 16:54 videosrc-0.1.9.dist-info/WHEEL
+-rw-rw-r--  2.0 unx       15 b- defN 23-May-21 16:54 videosrc-0.1.9.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx     2232 b- defN 23-May-21 16:54 videosrc-0.1.9.dist-info/RECORD
+28 files, 404518 bytes uncompressed, 88703 bytes compressed:  78.1%
```

## zipnote {}

```diff
@@ -63,23 +63,23 @@
 
 Filename: videosrc/crawlers/youtube.py
 Comment: 
 
 Filename: videosrc/models/__init__.py
 Comment: 
 
-Filename: videosrc-0.1.8.dist-info/LICENSE
+Filename: videosrc-0.1.9.dist-info/LICENSE
 Comment: 
 
-Filename: videosrc-0.1.8.dist-info/METADATA
+Filename: videosrc-0.1.9.dist-info/METADATA
 Comment: 
 
-Filename: videosrc-0.1.8.dist-info/WHEEL
+Filename: videosrc-0.1.9.dist-info/WHEEL
 Comment: 
 
-Filename: videosrc-0.1.8.dist-info/top_level.txt
+Filename: videosrc-0.1.9.dist-info/top_level.txt
 Comment: 
 
-Filename: videosrc-0.1.8.dist-info/RECORD
+Filename: videosrc-0.1.9.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## videosrc/crawlers/timcast.py

```diff
@@ -136,16 +136,22 @@
             video_page_url = video_link['href']
             video_page_url = urljoin(url, urlparse(video_page_url).path)
             async with ScraperSession() as s:
                 video_page = BeautifulSoup(
                     await s.get_html(video_page_url, proxy=self._proxy,
                                      **self.auth),
                     'html.parser')
-            iframe_tag = video_page.find('iframe')
-            embed_url = iframe_tag['src']
+            try:
+                iframe_tag = video_page.find('iframe')
+                embed_url = iframe_tag['src']
+
+            except TypeError:
+                LOGGER.warning('Skipped video, missing iframe', exc_info=True)
+                continue
+
             video_details = await get_embed_details(
                 embed_url, proxy=self._proxy)
             pubDate = parse_date(video_details['pubDate'])
 
             if state and pubDate < state:
                 LOGGER.info('Video published before last state %s', pubDate)
                 return
```

## videosrc/crawlers/youtube.py

```diff
@@ -0,0 +1,6 @@
+00000000: 6672 6f6d 2076 6964 656f 7372 632e 6372  from videosrc.cr
+00000010: 6177 6c65 7273 2e62 6173 6520 696d 706f  awlers.base impo
+00000020: 7274 2043 7261 776c 6572 0a0a 0a63 6c61  rt Crawler...cla
+00000030: 7373 2059 6f75 7475 6265 4372 6177 6c65  ss YoutubeCrawle
+00000040: 7228 4372 6177 6c65 7229 3a0a 2020 2020  r(Crawler):.    
+00000050: 7061 7373 0a                             pass.
```

## Comparing `videosrc-0.1.8.dist-info/LICENSE` & `videosrc-0.1.9.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `videosrc-0.1.8.dist-info/METADATA` & `videosrc-0.1.9.dist-info/METADATA`

 * *Files 4% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 Metadata-Version: 2.1
 Name: videosrc
-Version: 0.1.8
+Version: 0.1.9
 Summary: Video src crawler
-Home-page: https://github.com/btimby/cesium.tv/vidsrc/
+Home-page: https://github.com/cesium-tv/videosrc/
 Author: Ben Timby
 Author-email: btimby@gmail.com
 License-File: LICENSE
 Requires-Dist: aiohttp-scraper (==0.1.4)
 Requires-Dist: pyppeteer (==1.0.2)
 Requires-Dist: beautifulsoup4 (==4.10.0)
 Requires-Dist: requests (==2.25.1)
```

## Comparing `videosrc-0.1.8.dist-info/RECORD` & `videosrc-0.1.9.dist-info/RECORD`

 * *Files 9% similar despite different names*

```diff
@@ -13,16 +13,16 @@
 videosrc/crawlers/__init__.py,sha256=tEwn_Q7xIYuXhUP9t-CFqM8WPwEP_2n6v8s9FuaHwE4,500
 videosrc/crawlers/base.py,sha256=OIoZfmIkF8qVOYkdBBh1gRRCsMHLpVP_6EiDb-dG638,2256
 videosrc/crawlers/html.py,sha256=-AOjNEfGI4THK4OMfVwlG3K17HVa1ctMZoM3sBHOFwI,3565
 videosrc/crawlers/mrss.py,sha256=cwmzIoJApoAhkSMNgYO4OFYS-b5-wwRfFtFzLGWB6dY,6869
 videosrc/crawlers/odysee.py,sha256=7K3eHnlwCsJw3QG4oEhfM24nG8o81kBTa4b4Wy-r5LU,12992
 videosrc/crawlers/peertube.py,sha256=ndNjyZBGkgN6_w1PYdcAWqb54Yu5umllLQS4coCp3S8,5709
 videosrc/crawlers/rumble.py,sha256=4vkcqg-BJDbvrPLGKwObp1vDWYT10J7DSnhMj-9afzc,3928
-videosrc/crawlers/timcast.py,sha256=zTA_PxKBNYp_CrWO7vIqZ54OU4G3fNL3D3dYuoPhd2o,6903
+videosrc/crawlers/timcast.py,sha256=Mxj2A40RLl1zeLx0EVneYMSgVgERBhWrRtbxbmDl8So,7064
 videosrc/crawlers/twitter.py,sha256=2a5NGn7wZ0142brzk-ANBQ7St_M8_pWIRgxdBCbcsNE,3379
-videosrc/crawlers/youtube.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
+videosrc/crawlers/youtube.py,sha256=iorOHW_syI_MKnhKsDhYTA7871fTGPRnVfLl3dTY4hE,85
 videosrc/models/__init__.py,sha256=33PwZuf3LbSS1FZSVq-RVn2PbejFASLIItv005ixce4,626
-videosrc-0.1.8.dist-info/LICENSE,sha256=ZrmE4LhjnartZCuclnrGM1kWT3L1WxtXC84vnHMOxTc,1066
-videosrc-0.1.8.dist-info/METADATA,sha256=zujIQfgEW_R_CBDT0RWzXKTkGRUVb91uAemXAFFplNw,2044
-videosrc-0.1.8.dist-info/WHEEL,sha256=pkctZYzUS4AYVn6dJ-7367OJZivF2e8RA9b_ZBjif18,92
-videosrc-0.1.8.dist-info/top_level.txt,sha256=GVj7Kn2EZJ5LjJjdb6uJtVlPu5yaZ8MjWnmK76wRyAk,15
-videosrc-0.1.8.dist-info/RECORD,,
+videosrc-0.1.9.dist-info/LICENSE,sha256=ZrmE4LhjnartZCuclnrGM1kWT3L1WxtXC84vnHMOxTc,1066
+videosrc-0.1.9.dist-info/METADATA,sha256=Pe_vqZK6WKsd5WDKGgFUZiefPtGLu2jLGVFxSlLfLYk,2039
+videosrc-0.1.9.dist-info/WHEEL,sha256=pkctZYzUS4AYVn6dJ-7367OJZivF2e8RA9b_ZBjif18,92
+videosrc-0.1.9.dist-info/top_level.txt,sha256=GVj7Kn2EZJ5LjJjdb6uJtVlPu5yaZ8MjWnmK76wRyAk,15
+videosrc-0.1.9.dist-info/RECORD,,
```

