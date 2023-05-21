# Comparing `tmp/streamlit-reveal-slides-0.1.0.tar.gz` & `tmp/streamlit-reveal-slides-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "streamlit-reveal-slides-0.1.0.tar", last modified: Sat May 20 23:08:35 2023, max compression
+gzip compressed data, was "streamlit-reveal-slides-0.1.1.tar", last modified: Sun May 21 04:22:19 2023, max compression
```

## Comparing `streamlit-reveal-slides-0.1.0.tar` & `streamlit-reveal-slides-0.1.1.tar`

### file list

```diff
@@ -1,115 +1,115 @@
-drwxr-xr-x   0 anasbouzid  (1000) anasbouzid  (1000)        0 2023-05-20 23:08:35.629954 streamlit-reveal-slides-0.1.0/
--rw-r--r--   0 anasbouzid  (1000) anasbouzid  (1000)     1063 2023-02-08 18:48:37.000000 streamlit-reveal-slides-0.1.0/LICENSE
--rw-r--r--   0 anasbouzid  (1000) anasbouzid  (1000)       49 2023-05-20 00:27:59.000000 streamlit-reveal-slides-0.1.0/MANIFEST.in
--rw-r--r--   0 anasbouzid  (1000) anasbouzid  (1000)      393 2023-05-20 23:08:35.629954 streamlit-reveal-slides-0.1.0/PKG-INFO
-drwxr-xr-x   0 anasbouzid  (1000) anasbouzid  (1000)        0 2023-05-20 23:08:35.559954 streamlit-reveal-slides-0.1.0/reveal_slides/
--rw-r--r--   0 anasbouzid  (1000) anasbouzid  (1000)     7021 2023-05-20 23:06:32.000000 streamlit-reveal-slides-0.1.0/reveal_slides/__init__.py
-drwxr-xr-x   0 anasbouzid  (1000) anasbouzid  (1000)        0 2023-05-20 23:08:35.549954 streamlit-reveal-slides-0.1.0/reveal_slides/frontend/
-drwxr-xr-x   0 anasbouzid  (1000) anasbouzid  (1000)        0 2023-05-20 23:08:35.559954 streamlit-reveal-slides-0.1.0/reveal_slides/frontend/build/
--rw-r--r--   0 anasbouzid  (1000) anasbouzid  (1000)     6479 2023-05-20 23:08:16.000000 streamlit-reveal-slides-0.1.0/reveal_slides/frontend/build/asset-manifest.json
--rw-r--r--   0 anasbouzid  (1000) anasbouzid  (1000)   197459 2023-05-20 23:07:43.000000 streamlit-reveal-slides-0.1.0/reveal_slides/frontend/build/bootstrap.min.css
--rw-r--r--   0 anasbouzid  (1000) anasbouzid  (1000)     4356 2023-05-20 23:08:16.000000 streamlit-reveal-slides-0.1.0/reveal_slides/frontend/build/index.html
-drwxr-xr-x   0 anasbouzid  (1000) anasbouzid  (1000)        0 2023-05-20 23:08:35.559954 streamlit-reveal-slides-0.1.0/reveal_slides/frontend/build/static/
-drwxr-xr-x   0 anasbouzid  (1000) anasbouzid  (1000)        0 2023-05-20 23:08:35.569954 streamlit-reveal-slides-0.1.0/reveal_slides/frontend/build/static/css/
--rw-r--r--   0 anasbouzid  (1000) anasbouzid  (1000)     7201 2023-05-20 23:08:16.000000 streamlit-reveal-slides-0.1.0/reveal_slides/frontend/build/static/css/10.1f3244e3.chunk.css
--rw-r--r--   0 anasbouzid  (1000) anasbouzid  (1000)    11924 2023-05-20 23:08:16.000000 streamlit-reveal-slides-0.1.0/reveal_slides/frontend/build/static/css/10.1f3244e3.chunk.css.map
--rw-r--r--   0 anasbouzid  (1000) anasbouzid  (1000)     7253 2023-05-20 23:08:16.000000 streamlit-reveal-slides-0.1.0/reveal_slides/frontend/build/static/css/11.cb699f02.chunk.css
--rw-r--r--   0 anasbouzid  (1000) anasbouzid  (1000)    11744 2023-05-20 23:08:16.000000 streamlit-reveal-slides-0.1.0/reveal_slides/frontend/build/static/css/11.cb699f02.chunk.css.map
--rw-r--r--   0 anasbouzid  (1000) anasbouzid  (1000)     6477 2023-05-20 23:08:16.000000 streamlit-reveal-slides-0.1.0/reveal_slides/frontend/build/static/css/12.158b51eb.chunk.css
--rw-r--r--   0 anasbouzid  (1000) anasbouzid  (1000)    20354 2023-05-20 23:08:16.000000 streamlit-reveal-slides-0.1.0/reveal_slides/frontend/build/static/css/12.158b51eb.chunk.css.map
--rw-r--r--   0 anasbouzid  (1000) anasbouzid  (1000)     7194 2023-05-20 23:08:16.000000 streamlit-reveal-slides-0.1.0/reveal_slides/frontend/build/static/css/13.74908590.chunk.css
--rw-r--r--   0 anasbouzid  (1000) anasbouzid  (1000)    11911 2023-05-20 23:08:16.000000 streamlit-reveal-slides-0.1.0/reveal_slides/frontend/build/static/css/13.74908590.chunk.css.map
--rw-r--r--   0 anasbouzid  (1000) anasbouzid  (1000)     7194 2023-05-20 23:08:16.000000 streamlit-reveal-slides-0.1.0/reveal_slides/frontend/build/static/css/14.e64fc659.chunk.css
--rw-r--r--   0 anasbouzid  (1000) anasbouzid  (1000)    11713 2023-05-20 23:08:16.000000 streamlit-reveal-slides-0.1.0/reveal_slides/frontend/build/static/css/14.e64fc659.chunk.css.map
--rw-r--r--   0 anasbouzid  (1000) anasbouzid  (1000)     7184 2023-05-20 23:08:16.000000 streamlit-reveal-slides-0.1.0/reveal_slides/frontend/build/static/css/15.3adba626.chunk.css
--rw-r--r--   0 anasbouzid  (1000) anasbouzid  (1000)    11931 2023-05-20 23:08:16.000000 streamlit-reveal-slides-0.1.0/reveal_slides/frontend/build/static/css/15.3adba626.chunk.css.map
--rw-r--r--   0 anasbouzid  (1000) anasbouzid  (1000)     6719 2023-05-20 23:08:16.000000 streamlit-reveal-slides-0.1.0/reveal_slides/frontend/build/static/css/16.b573d318.chunk.css
--rw-r--r--   0 anasbouzid  (1000) anasbouzid  (1000)    11404 2023-05-20 23:08:16.000000 streamlit-reveal-slides-0.1.0/reveal_slides/frontend/build/static/css/16.b573d318.chunk.css.map
--rw-r--r--   0 anasbouzid  (1000) anasbouzid  (1000)      405 2023-05-20 23:08:16.000000 streamlit-reveal-slides-0.1.0/reveal_slides/frontend/build/static/css/17.10a8300f.chunk.css
--rw-r--r--   0 anasbouzid  (1000) anasbouzid  (1000)      580 2023-05-20 23:08:16.000000 streamlit-reveal-slides-0.1.0/reveal_slides/frontend/build/static/css/17.10a8300f.chunk.css.map
--rw-r--r--   0 anasbouzid  (1000) anasbouzid  (1000)     1666 2023-05-20 23:08:16.000000 streamlit-reveal-slides-0.1.0/reveal_slides/frontend/build/static/css/18.4eb3e38a.chunk.css
--rw-r--r--   0 anasbouzid  (1000) anasbouzid  (1000)     1954 2023-05-20 23:08:16.000000 streamlit-reveal-slides-0.1.0/reveal_slides/frontend/build/static/css/18.4eb3e38a.chunk.css.map
--rw-r--r--   0 anasbouzid  (1000) anasbouzid  (1000)     5699 2023-05-20 23:08:16.000000 streamlit-reveal-slides-0.1.0/reveal_slides/frontend/build/static/css/19.74b97645.chunk.css
--rw-r--r--   0 anasbouzid  (1000) anasbouzid  (1000)    10009 2023-05-20 23:08:16.000000 streamlit-reveal-slides-0.1.0/reveal_slides/frontend/build/static/css/19.74b97645.chunk.css.map
--rw-r--r--   0 anasbouzid  (1000) anasbouzid  (1000)    47158 2023-05-20 23:08:16.000000 streamlit-reveal-slides-0.1.0/reveal_slides/frontend/build/static/css/2.5029ddca.chunk.css
--rw-r--r--   0 anasbouzid  (1000) anasbouzid  (1000)    60673 2023-05-20 23:08:16.000000 streamlit-reveal-slides-0.1.0/reveal_slides/frontend/build/static/css/2.5029ddca.chunk.css.map
--rw-r--r--   0 anasbouzid  (1000) anasbouzid  (1000)     6543 2023-05-20 23:08:16.000000 streamlit-reveal-slides-0.1.0/reveal_slides/frontend/build/static/css/3.11f8848d.chunk.css
--rw-r--r--   0 anasbouzid  (1000) anasbouzid  (1000)    20560 2023-05-20 23:08:16.000000 streamlit-reveal-slides-0.1.0/reveal_slides/frontend/build/static/css/3.11f8848d.chunk.css.map
--rw-r--r--   0 anasbouzid  (1000) anasbouzid  (1000)     6560 2023-05-20 23:08:16.000000 streamlit-reveal-slides-0.1.0/reveal_slides/frontend/build/static/css/4.2fe0cb1b.chunk.css
--rw-r--r--   0 anasbouzid  (1000) anasbouzid  (1000)    20701 2023-05-20 23:08:16.000000 streamlit-reveal-slides-0.1.0/reveal_slides/frontend/build/static/css/4.2fe0cb1b.chunk.css.map
--rw-r--r--   0 anasbouzid  (1000) anasbouzid  (1000)     6057 2023-05-20 23:08:16.000000 streamlit-reveal-slides-0.1.0/reveal_slides/frontend/build/static/css/5.5a2b8ee3.chunk.css
--rw-r--r--   0 anasbouzid  (1000) anasbouzid  (1000)    19287 2023-05-20 23:08:16.000000 streamlit-reveal-slides-0.1.0/reveal_slides/frontend/build/static/css/5.5a2b8ee3.chunk.css.map
--rw-r--r--   0 anasbouzid  (1000) anasbouzid  (1000)     5695 2023-05-20 23:08:16.000000 streamlit-reveal-slides-0.1.0/reveal_slides/frontend/build/static/css/6.1b9cee33.chunk.css
--rw-r--r--   0 anasbouzid  (1000) anasbouzid  (1000)    18239 2023-05-20 23:08:16.000000 streamlit-reveal-slides-0.1.0/reveal_slides/frontend/build/static/css/6.1b9cee33.chunk.css.map
--rw-r--r--   0 anasbouzid  (1000) anasbouzid  (1000)     5701 2023-05-20 23:08:16.000000 streamlit-reveal-slides-0.1.0/reveal_slides/frontend/build/static/css/7.4e275de2.chunk.css
--rw-r--r--   0 anasbouzid  (1000) anasbouzid  (1000)    18662 2023-05-20 23:08:16.000000 streamlit-reveal-slides-0.1.0/reveal_slides/frontend/build/static/css/7.4e275de2.chunk.css.map
--rw-r--r--   0 anasbouzid  (1000) anasbouzid  (1000)     5826 2023-05-20 23:08:16.000000 streamlit-reveal-slides-0.1.0/reveal_slides/frontend/build/static/css/8.eb5abf62.chunk.css
--rw-r--r--   0 anasbouzid  (1000) anasbouzid  (1000)    19077 2023-05-20 23:08:16.000000 streamlit-reveal-slides-0.1.0/reveal_slides/frontend/build/static/css/8.eb5abf62.chunk.css.map
--rw-r--r--   0 anasbouzid  (1000) anasbouzid  (1000)     5825 2023-05-20 23:08:16.000000 streamlit-reveal-slides-0.1.0/reveal_slides/frontend/build/static/css/9.1253a161.chunk.css
--rw-r--r--   0 anasbouzid  (1000) anasbouzid  (1000)    18776 2023-05-20 23:08:16.000000 streamlit-reveal-slides-0.1.0/reveal_slides/frontend/build/static/css/9.1253a161.chunk.css.map
-drwxr-xr-x   0 anasbouzid  (1000) anasbouzid  (1000)        0 2023-05-20 23:08:35.609954 streamlit-reveal-slides-0.1.0/reveal_slides/frontend/build/static/js/
--rw-r--r--   0 anasbouzid  (1000) anasbouzid  (1000)      180 2023-05-20 23:08:16.000000 streamlit-reveal-slides-0.1.0/reveal_slides/frontend/build/static/js/10.a3f9f257.chunk.js
--rw-r--r--   0 anasbouzid  (1000) anasbouzid  (1000)      107 2023-05-20 23:08:16.000000 streamlit-reveal-slides-0.1.0/reveal_slides/frontend/build/static/js/10.a3f9f257.chunk.js.map
--rw-r--r--   0 anasbouzid  (1000) anasbouzid  (1000)      180 2023-05-20 23:08:16.000000 streamlit-reveal-slides-0.1.0/reveal_slides/frontend/build/static/js/11.90f5ba01.chunk.js
--rw-r--r--   0 anasbouzid  (1000) anasbouzid  (1000)      107 2023-05-20 23:08:16.000000 streamlit-reveal-slides-0.1.0/reveal_slides/frontend/build/static/js/11.90f5ba01.chunk.js.map
--rw-r--r--   0 anasbouzid  (1000) anasbouzid  (1000)      180 2023-05-20 23:08:16.000000 streamlit-reveal-slides-0.1.0/reveal_slides/frontend/build/static/js/12.1edcaba5.chunk.js
--rw-r--r--   0 anasbouzid  (1000) anasbouzid  (1000)      107 2023-05-20 23:08:16.000000 streamlit-reveal-slides-0.1.0/reveal_slides/frontend/build/static/js/12.1edcaba5.chunk.js.map
--rw-r--r--   0 anasbouzid  (1000) anasbouzid  (1000)      180 2023-05-20 23:08:16.000000 streamlit-reveal-slides-0.1.0/reveal_slides/frontend/build/static/js/13.031e1745.chunk.js
--rw-r--r--   0 anasbouzid  (1000) anasbouzid  (1000)      107 2023-05-20 23:08:16.000000 streamlit-reveal-slides-0.1.0/reveal_slides/frontend/build/static/js/13.031e1745.chunk.js.map
--rw-r--r--   0 anasbouzid  (1000) anasbouzid  (1000)      180 2023-05-20 23:08:16.000000 streamlit-reveal-slides-0.1.0/reveal_slides/frontend/build/static/js/14.c2a62bd4.chunk.js
--rw-r--r--   0 anasbouzid  (1000) anasbouzid  (1000)      107 2023-05-20 23:08:16.000000 streamlit-reveal-slides-0.1.0/reveal_slides/frontend/build/static/js/14.c2a62bd4.chunk.js.map
--rw-r--r--   0 anasbouzid  (1000) anasbouzid  (1000)      180 2023-05-20 23:08:16.000000 streamlit-reveal-slides-0.1.0/reveal_slides/frontend/build/static/js/15.257e774f.chunk.js
--rw-r--r--   0 anasbouzid  (1000) anasbouzid  (1000)      107 2023-05-20 23:08:16.000000 streamlit-reveal-slides-0.1.0/reveal_slides/frontend/build/static/js/15.257e774f.chunk.js.map
--rw-r--r--   0 anasbouzid  (1000) anasbouzid  (1000)      180 2023-05-20 23:08:16.000000 streamlit-reveal-slides-0.1.0/reveal_slides/frontend/build/static/js/16.a524310d.chunk.js
--rw-r--r--   0 anasbouzid  (1000) anasbouzid  (1000)      107 2023-05-20 23:08:16.000000 streamlit-reveal-slides-0.1.0/reveal_slides/frontend/build/static/js/16.a524310d.chunk.js.map
--rw-r--r--   0 anasbouzid  (1000) anasbouzid  (1000)      180 2023-05-20 23:08:16.000000 streamlit-reveal-slides-0.1.0/reveal_slides/frontend/build/static/js/17.c959c84a.chunk.js
--rw-r--r--   0 anasbouzid  (1000) anasbouzid  (1000)      107 2023-05-20 23:08:16.000000 streamlit-reveal-slides-0.1.0/reveal_slides/frontend/build/static/js/17.c959c84a.chunk.js.map
--rw-r--r--   0 anasbouzid  (1000) anasbouzid  (1000)      180 2023-05-20 23:08:16.000000 streamlit-reveal-slides-0.1.0/reveal_slides/frontend/build/static/js/18.90e2d74e.chunk.js
--rw-r--r--   0 anasbouzid  (1000) anasbouzid  (1000)      107 2023-05-20 23:08:16.000000 streamlit-reveal-slides-0.1.0/reveal_slides/frontend/build/static/js/18.90e2d74e.chunk.js.map
--rw-r--r--   0 anasbouzid  (1000) anasbouzid  (1000)      180 2023-05-20 23:08:16.000000 streamlit-reveal-slides-0.1.0/reveal_slides/frontend/build/static/js/19.0abf949e.chunk.js
--rw-r--r--   0 anasbouzid  (1000) anasbouzid  (1000)      107 2023-05-20 23:08:16.000000 streamlit-reveal-slides-0.1.0/reveal_slides/frontend/build/static/js/19.0abf949e.chunk.js.map
--rw-r--r--   0 anasbouzid  (1000) anasbouzid  (1000)  1812278 2023-05-20 23:08:16.000000 streamlit-reveal-slides-0.1.0/reveal_slides/frontend/build/static/js/2.fc540633.chunk.js
--rw-r--r--   0 anasbouzid  (1000) anasbouzid  (1000)     2767 2023-05-20 23:08:16.000000 streamlit-reveal-slides-0.1.0/reveal_slides/frontend/build/static/js/2.fc540633.chunk.js.LICENSE.txt
--rw-r--r--   0 anasbouzid  (1000) anasbouzid  (1000)  3752941 2023-05-20 23:08:16.000000 streamlit-reveal-slides-0.1.0/reveal_slides/frontend/build/static/js/2.fc540633.chunk.js.map
--rw-r--r--   0 anasbouzid  (1000) anasbouzid  (1000)      178 2023-05-20 23:08:16.000000 streamlit-reveal-slides-0.1.0/reveal_slides/frontend/build/static/js/3.c4d67f71.chunk.js
--rw-r--r--   0 anasbouzid  (1000) anasbouzid  (1000)      106 2023-05-20 23:08:16.000000 streamlit-reveal-slides-0.1.0/reveal_slides/frontend/build/static/js/3.c4d67f71.chunk.js.map
--rw-r--r--   0 anasbouzid  (1000) anasbouzid  (1000)      178 2023-05-20 23:08:16.000000 streamlit-reveal-slides-0.1.0/reveal_slides/frontend/build/static/js/4.71ecbbd1.chunk.js
--rw-r--r--   0 anasbouzid  (1000) anasbouzid  (1000)      106 2023-05-20 23:08:16.000000 streamlit-reveal-slides-0.1.0/reveal_slides/frontend/build/static/js/4.71ecbbd1.chunk.js.map
--rw-r--r--   0 anasbouzid  (1000) anasbouzid  (1000)      178 2023-05-20 23:08:16.000000 streamlit-reveal-slides-0.1.0/reveal_slides/frontend/build/static/js/5.4c3c6aac.chunk.js
--rw-r--r--   0 anasbouzid  (1000) anasbouzid  (1000)      106 2023-05-20 23:08:16.000000 streamlit-reveal-slides-0.1.0/reveal_slides/frontend/build/static/js/5.4c3c6aac.chunk.js.map
--rw-r--r--   0 anasbouzid  (1000) anasbouzid  (1000)      178 2023-05-20 23:08:16.000000 streamlit-reveal-slides-0.1.0/reveal_slides/frontend/build/static/js/6.2008461d.chunk.js
--rw-r--r--   0 anasbouzid  (1000) anasbouzid  (1000)      106 2023-05-20 23:08:16.000000 streamlit-reveal-slides-0.1.0/reveal_slides/frontend/build/static/js/6.2008461d.chunk.js.map
--rw-r--r--   0 anasbouzid  (1000) anasbouzid  (1000)      178 2023-05-20 23:08:16.000000 streamlit-reveal-slides-0.1.0/reveal_slides/frontend/build/static/js/7.69aea7e9.chunk.js
--rw-r--r--   0 anasbouzid  (1000) anasbouzid  (1000)      106 2023-05-20 23:08:16.000000 streamlit-reveal-slides-0.1.0/reveal_slides/frontend/build/static/js/7.69aea7e9.chunk.js.map
--rw-r--r--   0 anasbouzid  (1000) anasbouzid  (1000)      178 2023-05-20 23:08:16.000000 streamlit-reveal-slides-0.1.0/reveal_slides/frontend/build/static/js/8.86b27921.chunk.js
--rw-r--r--   0 anasbouzid  (1000) anasbouzid  (1000)      106 2023-05-20 23:08:16.000000 streamlit-reveal-slides-0.1.0/reveal_slides/frontend/build/static/js/8.86b27921.chunk.js.map
--rw-r--r--   0 anasbouzid  (1000) anasbouzid  (1000)      178 2023-05-20 23:08:16.000000 streamlit-reveal-slides-0.1.0/reveal_slides/frontend/build/static/js/9.fd893fed.chunk.js
--rw-r--r--   0 anasbouzid  (1000) anasbouzid  (1000)      106 2023-05-20 23:08:16.000000 streamlit-reveal-slides-0.1.0/reveal_slides/frontend/build/static/js/9.fd893fed.chunk.js.map
--rw-r--r--   0 anasbouzid  (1000) anasbouzid  (1000)     4002 2023-05-20 23:08:16.000000 streamlit-reveal-slides-0.1.0/reveal_slides/frontend/build/static/js/main.c54401b6.chunk.js
--rw-r--r--   0 anasbouzid  (1000) anasbouzid  (1000)    16990 2023-05-20 23:08:16.000000 streamlit-reveal-slides-0.1.0/reveal_slides/frontend/build/static/js/main.c54401b6.chunk.js.map
--rw-r--r--   0 anasbouzid  (1000) anasbouzid  (1000)     3774 2023-05-20 23:08:16.000000 streamlit-reveal-slides-0.1.0/reveal_slides/frontend/build/static/js/runtime-main.cda34e22.js
--rw-r--r--   0 anasbouzid  (1000) anasbouzid  (1000)    17321 2023-05-20 23:08:16.000000 streamlit-reveal-slides-0.1.0/reveal_slides/frontend/build/static/js/runtime-main.cda34e22.js.map
-drwxr-xr-x   0 anasbouzid  (1000) anasbouzid  (1000)        0 2023-05-20 23:08:35.629954 streamlit-reveal-slides-0.1.0/reveal_slides/frontend/build/static/media/
--rw-r--r--   0 anasbouzid  (1000) anasbouzid  (1000)    30764 2023-05-20 23:08:16.000000 streamlit-reveal-slides-0.1.0/reveal_slides/frontend/build/static/media/league-gothic.080eee2a.woff
--rw-r--r--   0 anasbouzid  (1000) anasbouzid  (1000)    25696 2023-05-20 23:08:16.000000 streamlit-reveal-slides-0.1.0/reveal_slides/frontend/build/static/media/league-gothic.12baac5d.eot
--rw-r--r--   0 anasbouzid  (1000) anasbouzid  (1000)    64256 2023-05-20 23:08:16.000000 streamlit-reveal-slides-0.1.0/reveal_slides/frontend/build/static/media/league-gothic.6ae91382.ttf
--rw-r--r--   0 anasbouzid  (1000) anasbouzid  (1000)   238084 2023-05-20 23:08:16.000000 streamlit-reveal-slides-0.1.0/reveal_slides/frontend/build/static/media/source-sans-pro-italic.10a5cb40.ttf
--rw-r--r--   0 anasbouzid  (1000) anasbouzid  (1000)    75720 2023-05-20 23:08:16.000000 streamlit-reveal-slides-0.1.0/reveal_slides/frontend/build/static/media/source-sans-pro-italic.97e79d3e.eot
--rw-r--r--   0 anasbouzid  (1000) anasbouzid  (1000)    98556 2023-05-20 23:08:16.000000 streamlit-reveal-slides-0.1.0/reveal_slides/frontend/build/static/media/source-sans-pro-italic.983d97ca.woff
--rw-r--r--   0 anasbouzid  (1000) anasbouzid  (1000)    88070 2023-05-20 23:08:16.000000 streamlit-reveal-slides-0.1.0/reveal_slides/frontend/build/static/media/source-sans-pro-regular.36443d24.eot
--rw-r--r--   0 anasbouzid  (1000) anasbouzid  (1000)   288008 2023-05-20 23:08:16.000000 streamlit-reveal-slides-0.1.0/reveal_slides/frontend/build/static/media/source-sans-pro-regular.45c54810.ttf
--rw-r--r--   0 anasbouzid  (1000) anasbouzid  (1000)   114324 2023-05-20 23:08:16.000000 streamlit-reveal-slides-0.1.0/reveal_slides/frontend/build/static/media/source-sans-pro-regular.d1653550.woff
--rw-r--r--   0 anasbouzid  (1000) anasbouzid  (1000)   284640 2023-05-20 23:08:16.000000 streamlit-reveal-slides-0.1.0/reveal_slides/frontend/build/static/media/source-sans-pro-semibold.6ebea875.ttf
--rw-r--r--   0 anasbouzid  (1000) anasbouzid  (1000)    89897 2023-05-20 23:08:16.000000 streamlit-reveal-slides-0.1.0/reveal_slides/frontend/build/static/media/source-sans-pro-semibold.83db537e.eot
--rw-r--r--   0 anasbouzid  (1000) anasbouzid  (1000)   115648 2023-05-20 23:08:16.000000 streamlit-reveal-slides-0.1.0/reveal_slides/frontend/build/static/media/source-sans-pro-semibold.f11ba60a.woff
--rw-r--r--   0 anasbouzid  (1000) anasbouzid  (1000)   240944 2023-05-20 23:08:16.000000 streamlit-reveal-slides-0.1.0/reveal_slides/frontend/build/static/media/source-sans-pro-semibolditalic.522a9ee9.ttf
--rw-r--r--   0 anasbouzid  (1000) anasbouzid  (1000)    98816 2023-05-20 23:08:16.000000 streamlit-reveal-slides-0.1.0/reveal_slides/frontend/build/static/media/source-sans-pro-semibolditalic.a43f56ac.woff
--rw-r--r--   0 anasbouzid  (1000) anasbouzid  (1000)    75706 2023-05-20 23:08:16.000000 streamlit-reveal-slides-0.1.0/reveal_slides/frontend/build/static/media/source-sans-pro-semibolditalic.fb03c660.eot
--rw-r--r--   0 anasbouzid  (1000) anasbouzid  (1000)       38 2023-05-20 23:08:35.629954 streamlit-reveal-slides-0.1.0/setup.cfg
--rw-r--r--   0 anasbouzid  (1000) anasbouzid  (1000)      764 2023-05-20 22:58:12.000000 streamlit-reveal-slides-0.1.0/setup.py
-drwxr-xr-x   0 anasbouzid  (1000) anasbouzid  (1000)        0 2023-05-20 23:08:35.629954 streamlit-reveal-slides-0.1.0/streamlit_reveal_slides.egg-info/
--rw-r--r--   0 anasbouzid  (1000) anasbouzid  (1000)      393 2023-05-20 23:08:35.000000 streamlit-reveal-slides-0.1.0/streamlit_reveal_slides.egg-info/PKG-INFO
--rw-r--r--   0 anasbouzid  (1000) anasbouzid  (1000)     6440 2023-05-20 23:08:35.000000 streamlit-reveal-slides-0.1.0/streamlit_reveal_slides.egg-info/SOURCES.txt
--rw-r--r--   0 anasbouzid  (1000) anasbouzid  (1000)        1 2023-05-20 23:08:35.000000 streamlit-reveal-slides-0.1.0/streamlit_reveal_slides.egg-info/dependency_links.txt
--rw-r--r--   0 anasbouzid  (1000) anasbouzid  (1000)       16 2023-05-20 23:08:35.000000 streamlit-reveal-slides-0.1.0/streamlit_reveal_slides.egg-info/requires.txt
--rw-r--r--   0 anasbouzid  (1000) anasbouzid  (1000)       14 2023-05-20 23:08:35.000000 streamlit-reveal-slides-0.1.0/streamlit_reveal_slides.egg-info/top_level.txt
+drwxr-xr-x   0 anasbouzid  (1000) anasbouzid  (1000)        0 2023-05-21 04:22:19.441717 streamlit-reveal-slides-0.1.1/
+-rw-r--r--   0 anasbouzid  (1000) anasbouzid  (1000)     1063 2023-02-08 18:48:37.000000 streamlit-reveal-slides-0.1.1/LICENSE
+-rw-r--r--   0 anasbouzid  (1000) anasbouzid  (1000)       49 2023-05-20 00:27:59.000000 streamlit-reveal-slides-0.1.1/MANIFEST.in
+-rw-r--r--   0 anasbouzid  (1000) anasbouzid  (1000)      393 2023-05-21 04:22:19.441717 streamlit-reveal-slides-0.1.1/PKG-INFO
+drwxr-xr-x   0 anasbouzid  (1000) anasbouzid  (1000)        0 2023-05-21 04:22:19.381718 streamlit-reveal-slides-0.1.1/reveal_slides/
+-rw-r--r--   0 anasbouzid  (1000) anasbouzid  (1000)     7021 2023-05-20 23:06:32.000000 streamlit-reveal-slides-0.1.1/reveal_slides/__init__.py
+drwxr-xr-x   0 anasbouzid  (1000) anasbouzid  (1000)        0 2023-05-21 04:22:19.371718 streamlit-reveal-slides-0.1.1/reveal_slides/frontend/
+drwxr-xr-x   0 anasbouzid  (1000) anasbouzid  (1000)        0 2023-05-21 04:22:19.381718 streamlit-reveal-slides-0.1.1/reveal_slides/frontend/build/
+-rw-r--r--   0 anasbouzid  (1000) anasbouzid  (1000)     6479 2023-05-21 04:21:03.000000 streamlit-reveal-slides-0.1.1/reveal_slides/frontend/build/asset-manifest.json
+-rw-r--r--   0 anasbouzid  (1000) anasbouzid  (1000)   197459 2023-05-21 04:20:31.000000 streamlit-reveal-slides-0.1.1/reveal_slides/frontend/build/bootstrap.min.css
+-rw-r--r--   0 anasbouzid  (1000) anasbouzid  (1000)     4356 2023-05-21 04:21:03.000000 streamlit-reveal-slides-0.1.1/reveal_slides/frontend/build/index.html
+drwxr-xr-x   0 anasbouzid  (1000) anasbouzid  (1000)        0 2023-05-21 04:22:19.381718 streamlit-reveal-slides-0.1.1/reveal_slides/frontend/build/static/
+drwxr-xr-x   0 anasbouzid  (1000) anasbouzid  (1000)        0 2023-05-21 04:22:19.401718 streamlit-reveal-slides-0.1.1/reveal_slides/frontend/build/static/css/
+-rw-r--r--   0 anasbouzid  (1000) anasbouzid  (1000)     7201 2023-05-21 04:21:03.000000 streamlit-reveal-slides-0.1.1/reveal_slides/frontend/build/static/css/10.1f3244e3.chunk.css
+-rw-r--r--   0 anasbouzid  (1000) anasbouzid  (1000)    11924 2023-05-21 04:21:03.000000 streamlit-reveal-slides-0.1.1/reveal_slides/frontend/build/static/css/10.1f3244e3.chunk.css.map
+-rw-r--r--   0 anasbouzid  (1000) anasbouzid  (1000)     7253 2023-05-21 04:21:03.000000 streamlit-reveal-slides-0.1.1/reveal_slides/frontend/build/static/css/11.cb699f02.chunk.css
+-rw-r--r--   0 anasbouzid  (1000) anasbouzid  (1000)    11744 2023-05-21 04:21:03.000000 streamlit-reveal-slides-0.1.1/reveal_slides/frontend/build/static/css/11.cb699f02.chunk.css.map
+-rw-r--r--   0 anasbouzid  (1000) anasbouzid  (1000)     6477 2023-05-21 04:21:03.000000 streamlit-reveal-slides-0.1.1/reveal_slides/frontend/build/static/css/12.158b51eb.chunk.css
+-rw-r--r--   0 anasbouzid  (1000) anasbouzid  (1000)    20354 2023-05-21 04:21:03.000000 streamlit-reveal-slides-0.1.1/reveal_slides/frontend/build/static/css/12.158b51eb.chunk.css.map
+-rw-r--r--   0 anasbouzid  (1000) anasbouzid  (1000)     7194 2023-05-21 04:21:03.000000 streamlit-reveal-slides-0.1.1/reveal_slides/frontend/build/static/css/13.74908590.chunk.css
+-rw-r--r--   0 anasbouzid  (1000) anasbouzid  (1000)    11911 2023-05-21 04:21:03.000000 streamlit-reveal-slides-0.1.1/reveal_slides/frontend/build/static/css/13.74908590.chunk.css.map
+-rw-r--r--   0 anasbouzid  (1000) anasbouzid  (1000)     7194 2023-05-21 04:21:03.000000 streamlit-reveal-slides-0.1.1/reveal_slides/frontend/build/static/css/14.e64fc659.chunk.css
+-rw-r--r--   0 anasbouzid  (1000) anasbouzid  (1000)    11713 2023-05-21 04:21:03.000000 streamlit-reveal-slides-0.1.1/reveal_slides/frontend/build/static/css/14.e64fc659.chunk.css.map
+-rw-r--r--   0 anasbouzid  (1000) anasbouzid  (1000)     7184 2023-05-21 04:21:03.000000 streamlit-reveal-slides-0.1.1/reveal_slides/frontend/build/static/css/15.3adba626.chunk.css
+-rw-r--r--   0 anasbouzid  (1000) anasbouzid  (1000)    11931 2023-05-21 04:21:03.000000 streamlit-reveal-slides-0.1.1/reveal_slides/frontend/build/static/css/15.3adba626.chunk.css.map
+-rw-r--r--   0 anasbouzid  (1000) anasbouzid  (1000)     6719 2023-05-21 04:21:03.000000 streamlit-reveal-slides-0.1.1/reveal_slides/frontend/build/static/css/16.b573d318.chunk.css
+-rw-r--r--   0 anasbouzid  (1000) anasbouzid  (1000)    11404 2023-05-21 04:21:03.000000 streamlit-reveal-slides-0.1.1/reveal_slides/frontend/build/static/css/16.b573d318.chunk.css.map
+-rw-r--r--   0 anasbouzid  (1000) anasbouzid  (1000)      405 2023-05-21 04:21:03.000000 streamlit-reveal-slides-0.1.1/reveal_slides/frontend/build/static/css/17.10a8300f.chunk.css
+-rw-r--r--   0 anasbouzid  (1000) anasbouzid  (1000)      580 2023-05-21 04:21:03.000000 streamlit-reveal-slides-0.1.1/reveal_slides/frontend/build/static/css/17.10a8300f.chunk.css.map
+-rw-r--r--   0 anasbouzid  (1000) anasbouzid  (1000)     1666 2023-05-21 04:21:03.000000 streamlit-reveal-slides-0.1.1/reveal_slides/frontend/build/static/css/18.4eb3e38a.chunk.css
+-rw-r--r--   0 anasbouzid  (1000) anasbouzid  (1000)     1954 2023-05-21 04:21:03.000000 streamlit-reveal-slides-0.1.1/reveal_slides/frontend/build/static/css/18.4eb3e38a.chunk.css.map
+-rw-r--r--   0 anasbouzid  (1000) anasbouzid  (1000)     5699 2023-05-21 04:21:03.000000 streamlit-reveal-slides-0.1.1/reveal_slides/frontend/build/static/css/19.74b97645.chunk.css
+-rw-r--r--   0 anasbouzid  (1000) anasbouzid  (1000)    10009 2023-05-21 04:21:03.000000 streamlit-reveal-slides-0.1.1/reveal_slides/frontend/build/static/css/19.74b97645.chunk.css.map
+-rw-r--r--   0 anasbouzid  (1000) anasbouzid  (1000)    47158 2023-05-21 04:21:03.000000 streamlit-reveal-slides-0.1.1/reveal_slides/frontend/build/static/css/2.5029ddca.chunk.css
+-rw-r--r--   0 anasbouzid  (1000) anasbouzid  (1000)    60673 2023-05-21 04:21:03.000000 streamlit-reveal-slides-0.1.1/reveal_slides/frontend/build/static/css/2.5029ddca.chunk.css.map
+-rw-r--r--   0 anasbouzid  (1000) anasbouzid  (1000)     6543 2023-05-21 04:21:03.000000 streamlit-reveal-slides-0.1.1/reveal_slides/frontend/build/static/css/3.11f8848d.chunk.css
+-rw-r--r--   0 anasbouzid  (1000) anasbouzid  (1000)    20560 2023-05-21 04:21:03.000000 streamlit-reveal-slides-0.1.1/reveal_slides/frontend/build/static/css/3.11f8848d.chunk.css.map
+-rw-r--r--   0 anasbouzid  (1000) anasbouzid  (1000)     6560 2023-05-21 04:21:03.000000 streamlit-reveal-slides-0.1.1/reveal_slides/frontend/build/static/css/4.2fe0cb1b.chunk.css
+-rw-r--r--   0 anasbouzid  (1000) anasbouzid  (1000)    20701 2023-05-21 04:21:03.000000 streamlit-reveal-slides-0.1.1/reveal_slides/frontend/build/static/css/4.2fe0cb1b.chunk.css.map
+-rw-r--r--   0 anasbouzid  (1000) anasbouzid  (1000)     6057 2023-05-21 04:21:03.000000 streamlit-reveal-slides-0.1.1/reveal_slides/frontend/build/static/css/5.5a2b8ee3.chunk.css
+-rw-r--r--   0 anasbouzid  (1000) anasbouzid  (1000)    19287 2023-05-21 04:21:03.000000 streamlit-reveal-slides-0.1.1/reveal_slides/frontend/build/static/css/5.5a2b8ee3.chunk.css.map
+-rw-r--r--   0 anasbouzid  (1000) anasbouzid  (1000)     5695 2023-05-21 04:21:03.000000 streamlit-reveal-slides-0.1.1/reveal_slides/frontend/build/static/css/6.1b9cee33.chunk.css
+-rw-r--r--   0 anasbouzid  (1000) anasbouzid  (1000)    18239 2023-05-21 04:21:03.000000 streamlit-reveal-slides-0.1.1/reveal_slides/frontend/build/static/css/6.1b9cee33.chunk.css.map
+-rw-r--r--   0 anasbouzid  (1000) anasbouzid  (1000)     5701 2023-05-21 04:21:03.000000 streamlit-reveal-slides-0.1.1/reveal_slides/frontend/build/static/css/7.4e275de2.chunk.css
+-rw-r--r--   0 anasbouzid  (1000) anasbouzid  (1000)    18662 2023-05-21 04:21:03.000000 streamlit-reveal-slides-0.1.1/reveal_slides/frontend/build/static/css/7.4e275de2.chunk.css.map
+-rw-r--r--   0 anasbouzid  (1000) anasbouzid  (1000)     5826 2023-05-21 04:21:03.000000 streamlit-reveal-slides-0.1.1/reveal_slides/frontend/build/static/css/8.eb5abf62.chunk.css
+-rw-r--r--   0 anasbouzid  (1000) anasbouzid  (1000)    19077 2023-05-21 04:21:03.000000 streamlit-reveal-slides-0.1.1/reveal_slides/frontend/build/static/css/8.eb5abf62.chunk.css.map
+-rw-r--r--   0 anasbouzid  (1000) anasbouzid  (1000)     5825 2023-05-21 04:21:03.000000 streamlit-reveal-slides-0.1.1/reveal_slides/frontend/build/static/css/9.1253a161.chunk.css
+-rw-r--r--   0 anasbouzid  (1000) anasbouzid  (1000)    18776 2023-05-21 04:21:03.000000 streamlit-reveal-slides-0.1.1/reveal_slides/frontend/build/static/css/9.1253a161.chunk.css.map
+drwxr-xr-x   0 anasbouzid  (1000) anasbouzid  (1000)        0 2023-05-21 04:22:19.431717 streamlit-reveal-slides-0.1.1/reveal_slides/frontend/build/static/js/
+-rw-r--r--   0 anasbouzid  (1000) anasbouzid  (1000)      180 2023-05-21 04:21:03.000000 streamlit-reveal-slides-0.1.1/reveal_slides/frontend/build/static/js/10.a3f9f257.chunk.js
+-rw-r--r--   0 anasbouzid  (1000) anasbouzid  (1000)      107 2023-05-21 04:21:03.000000 streamlit-reveal-slides-0.1.1/reveal_slides/frontend/build/static/js/10.a3f9f257.chunk.js.map
+-rw-r--r--   0 anasbouzid  (1000) anasbouzid  (1000)      180 2023-05-21 04:21:03.000000 streamlit-reveal-slides-0.1.1/reveal_slides/frontend/build/static/js/11.90f5ba01.chunk.js
+-rw-r--r--   0 anasbouzid  (1000) anasbouzid  (1000)      107 2023-05-21 04:21:03.000000 streamlit-reveal-slides-0.1.1/reveal_slides/frontend/build/static/js/11.90f5ba01.chunk.js.map
+-rw-r--r--   0 anasbouzid  (1000) anasbouzid  (1000)      180 2023-05-21 04:21:03.000000 streamlit-reveal-slides-0.1.1/reveal_slides/frontend/build/static/js/12.1edcaba5.chunk.js
+-rw-r--r--   0 anasbouzid  (1000) anasbouzid  (1000)      107 2023-05-21 04:21:03.000000 streamlit-reveal-slides-0.1.1/reveal_slides/frontend/build/static/js/12.1edcaba5.chunk.js.map
+-rw-r--r--   0 anasbouzid  (1000) anasbouzid  (1000)      180 2023-05-21 04:21:03.000000 streamlit-reveal-slides-0.1.1/reveal_slides/frontend/build/static/js/13.031e1745.chunk.js
+-rw-r--r--   0 anasbouzid  (1000) anasbouzid  (1000)      107 2023-05-21 04:21:03.000000 streamlit-reveal-slides-0.1.1/reveal_slides/frontend/build/static/js/13.031e1745.chunk.js.map
+-rw-r--r--   0 anasbouzid  (1000) anasbouzid  (1000)      180 2023-05-21 04:21:03.000000 streamlit-reveal-slides-0.1.1/reveal_slides/frontend/build/static/js/14.c2a62bd4.chunk.js
+-rw-r--r--   0 anasbouzid  (1000) anasbouzid  (1000)      107 2023-05-21 04:21:03.000000 streamlit-reveal-slides-0.1.1/reveal_slides/frontend/build/static/js/14.c2a62bd4.chunk.js.map
+-rw-r--r--   0 anasbouzid  (1000) anasbouzid  (1000)      180 2023-05-21 04:21:03.000000 streamlit-reveal-slides-0.1.1/reveal_slides/frontend/build/static/js/15.257e774f.chunk.js
+-rw-r--r--   0 anasbouzid  (1000) anasbouzid  (1000)      107 2023-05-21 04:21:03.000000 streamlit-reveal-slides-0.1.1/reveal_slides/frontend/build/static/js/15.257e774f.chunk.js.map
+-rw-r--r--   0 anasbouzid  (1000) anasbouzid  (1000)      180 2023-05-21 04:21:03.000000 streamlit-reveal-slides-0.1.1/reveal_slides/frontend/build/static/js/16.a524310d.chunk.js
+-rw-r--r--   0 anasbouzid  (1000) anasbouzid  (1000)      107 2023-05-21 04:21:03.000000 streamlit-reveal-slides-0.1.1/reveal_slides/frontend/build/static/js/16.a524310d.chunk.js.map
+-rw-r--r--   0 anasbouzid  (1000) anasbouzid  (1000)      180 2023-05-21 04:21:03.000000 streamlit-reveal-slides-0.1.1/reveal_slides/frontend/build/static/js/17.c959c84a.chunk.js
+-rw-r--r--   0 anasbouzid  (1000) anasbouzid  (1000)      107 2023-05-21 04:21:03.000000 streamlit-reveal-slides-0.1.1/reveal_slides/frontend/build/static/js/17.c959c84a.chunk.js.map
+-rw-r--r--   0 anasbouzid  (1000) anasbouzid  (1000)      180 2023-05-21 04:21:03.000000 streamlit-reveal-slides-0.1.1/reveal_slides/frontend/build/static/js/18.90e2d74e.chunk.js
+-rw-r--r--   0 anasbouzid  (1000) anasbouzid  (1000)      107 2023-05-21 04:21:03.000000 streamlit-reveal-slides-0.1.1/reveal_slides/frontend/build/static/js/18.90e2d74e.chunk.js.map
+-rw-r--r--   0 anasbouzid  (1000) anasbouzid  (1000)      180 2023-05-21 04:21:03.000000 streamlit-reveal-slides-0.1.1/reveal_slides/frontend/build/static/js/19.0abf949e.chunk.js
+-rw-r--r--   0 anasbouzid  (1000) anasbouzid  (1000)      107 2023-05-21 04:21:03.000000 streamlit-reveal-slides-0.1.1/reveal_slides/frontend/build/static/js/19.0abf949e.chunk.js.map
+-rw-r--r--   0 anasbouzid  (1000) anasbouzid  (1000)  1812278 2023-05-21 04:21:03.000000 streamlit-reveal-slides-0.1.1/reveal_slides/frontend/build/static/js/2.fc540633.chunk.js
+-rw-r--r--   0 anasbouzid  (1000) anasbouzid  (1000)     2767 2023-05-21 04:21:03.000000 streamlit-reveal-slides-0.1.1/reveal_slides/frontend/build/static/js/2.fc540633.chunk.js.LICENSE.txt
+-rw-r--r--   0 anasbouzid  (1000) anasbouzid  (1000)  3752941 2023-05-21 04:21:03.000000 streamlit-reveal-slides-0.1.1/reveal_slides/frontend/build/static/js/2.fc540633.chunk.js.map
+-rw-r--r--   0 anasbouzid  (1000) anasbouzid  (1000)      178 2023-05-21 04:21:03.000000 streamlit-reveal-slides-0.1.1/reveal_slides/frontend/build/static/js/3.c4d67f71.chunk.js
+-rw-r--r--   0 anasbouzid  (1000) anasbouzid  (1000)      106 2023-05-21 04:21:03.000000 streamlit-reveal-slides-0.1.1/reveal_slides/frontend/build/static/js/3.c4d67f71.chunk.js.map
+-rw-r--r--   0 anasbouzid  (1000) anasbouzid  (1000)      178 2023-05-21 04:21:03.000000 streamlit-reveal-slides-0.1.1/reveal_slides/frontend/build/static/js/4.71ecbbd1.chunk.js
+-rw-r--r--   0 anasbouzid  (1000) anasbouzid  (1000)      106 2023-05-21 04:21:03.000000 streamlit-reveal-slides-0.1.1/reveal_slides/frontend/build/static/js/4.71ecbbd1.chunk.js.map
+-rw-r--r--   0 anasbouzid  (1000) anasbouzid  (1000)      178 2023-05-21 04:21:03.000000 streamlit-reveal-slides-0.1.1/reveal_slides/frontend/build/static/js/5.4c3c6aac.chunk.js
+-rw-r--r--   0 anasbouzid  (1000) anasbouzid  (1000)      106 2023-05-21 04:21:03.000000 streamlit-reveal-slides-0.1.1/reveal_slides/frontend/build/static/js/5.4c3c6aac.chunk.js.map
+-rw-r--r--   0 anasbouzid  (1000) anasbouzid  (1000)      178 2023-05-21 04:21:03.000000 streamlit-reveal-slides-0.1.1/reveal_slides/frontend/build/static/js/6.2008461d.chunk.js
+-rw-r--r--   0 anasbouzid  (1000) anasbouzid  (1000)      106 2023-05-21 04:21:03.000000 streamlit-reveal-slides-0.1.1/reveal_slides/frontend/build/static/js/6.2008461d.chunk.js.map
+-rw-r--r--   0 anasbouzid  (1000) anasbouzid  (1000)      178 2023-05-21 04:21:03.000000 streamlit-reveal-slides-0.1.1/reveal_slides/frontend/build/static/js/7.69aea7e9.chunk.js
+-rw-r--r--   0 anasbouzid  (1000) anasbouzid  (1000)      106 2023-05-21 04:21:03.000000 streamlit-reveal-slides-0.1.1/reveal_slides/frontend/build/static/js/7.69aea7e9.chunk.js.map
+-rw-r--r--   0 anasbouzid  (1000) anasbouzid  (1000)      178 2023-05-21 04:21:03.000000 streamlit-reveal-slides-0.1.1/reveal_slides/frontend/build/static/js/8.86b27921.chunk.js
+-rw-r--r--   0 anasbouzid  (1000) anasbouzid  (1000)      106 2023-05-21 04:21:03.000000 streamlit-reveal-slides-0.1.1/reveal_slides/frontend/build/static/js/8.86b27921.chunk.js.map
+-rw-r--r--   0 anasbouzid  (1000) anasbouzid  (1000)      178 2023-05-21 04:21:03.000000 streamlit-reveal-slides-0.1.1/reveal_slides/frontend/build/static/js/9.fd893fed.chunk.js
+-rw-r--r--   0 anasbouzid  (1000) anasbouzid  (1000)      106 2023-05-21 04:21:03.000000 streamlit-reveal-slides-0.1.1/reveal_slides/frontend/build/static/js/9.fd893fed.chunk.js.map
+-rw-r--r--   0 anasbouzid  (1000) anasbouzid  (1000)     3909 2023-05-21 04:21:03.000000 streamlit-reveal-slides-0.1.1/reveal_slides/frontend/build/static/js/main.6641c370.chunk.js
+-rw-r--r--   0 anasbouzid  (1000) anasbouzid  (1000)    16690 2023-05-21 04:21:03.000000 streamlit-reveal-slides-0.1.1/reveal_slides/frontend/build/static/js/main.6641c370.chunk.js.map
+-rw-r--r--   0 anasbouzid  (1000) anasbouzid  (1000)     3774 2023-05-21 04:21:03.000000 streamlit-reveal-slides-0.1.1/reveal_slides/frontend/build/static/js/runtime-main.cda34e22.js
+-rw-r--r--   0 anasbouzid  (1000) anasbouzid  (1000)    17321 2023-05-21 04:21:03.000000 streamlit-reveal-slides-0.1.1/reveal_slides/frontend/build/static/js/runtime-main.cda34e22.js.map
+drwxr-xr-x   0 anasbouzid  (1000) anasbouzid  (1000)        0 2023-05-21 04:22:19.441717 streamlit-reveal-slides-0.1.1/reveal_slides/frontend/build/static/media/
+-rw-r--r--   0 anasbouzid  (1000) anasbouzid  (1000)    30764 2023-05-21 04:21:03.000000 streamlit-reveal-slides-0.1.1/reveal_slides/frontend/build/static/media/league-gothic.080eee2a.woff
+-rw-r--r--   0 anasbouzid  (1000) anasbouzid  (1000)    25696 2023-05-21 04:21:03.000000 streamlit-reveal-slides-0.1.1/reveal_slides/frontend/build/static/media/league-gothic.12baac5d.eot
+-rw-r--r--   0 anasbouzid  (1000) anasbouzid  (1000)    64256 2023-05-21 04:21:03.000000 streamlit-reveal-slides-0.1.1/reveal_slides/frontend/build/static/media/league-gothic.6ae91382.ttf
+-rw-r--r--   0 anasbouzid  (1000) anasbouzid  (1000)   238084 2023-05-21 04:21:03.000000 streamlit-reveal-slides-0.1.1/reveal_slides/frontend/build/static/media/source-sans-pro-italic.10a5cb40.ttf
+-rw-r--r--   0 anasbouzid  (1000) anasbouzid  (1000)    75720 2023-05-21 04:21:03.000000 streamlit-reveal-slides-0.1.1/reveal_slides/frontend/build/static/media/source-sans-pro-italic.97e79d3e.eot
+-rw-r--r--   0 anasbouzid  (1000) anasbouzid  (1000)    98556 2023-05-21 04:21:03.000000 streamlit-reveal-slides-0.1.1/reveal_slides/frontend/build/static/media/source-sans-pro-italic.983d97ca.woff
+-rw-r--r--   0 anasbouzid  (1000) anasbouzid  (1000)    88070 2023-05-21 04:21:03.000000 streamlit-reveal-slides-0.1.1/reveal_slides/frontend/build/static/media/source-sans-pro-regular.36443d24.eot
+-rw-r--r--   0 anasbouzid  (1000) anasbouzid  (1000)   288008 2023-05-21 04:21:03.000000 streamlit-reveal-slides-0.1.1/reveal_slides/frontend/build/static/media/source-sans-pro-regular.45c54810.ttf
+-rw-r--r--   0 anasbouzid  (1000) anasbouzid  (1000)   114324 2023-05-21 04:21:03.000000 streamlit-reveal-slides-0.1.1/reveal_slides/frontend/build/static/media/source-sans-pro-regular.d1653550.woff
+-rw-r--r--   0 anasbouzid  (1000) anasbouzid  (1000)   284640 2023-05-21 04:21:03.000000 streamlit-reveal-slides-0.1.1/reveal_slides/frontend/build/static/media/source-sans-pro-semibold.6ebea875.ttf
+-rw-r--r--   0 anasbouzid  (1000) anasbouzid  (1000)    89897 2023-05-21 04:21:03.000000 streamlit-reveal-slides-0.1.1/reveal_slides/frontend/build/static/media/source-sans-pro-semibold.83db537e.eot
+-rw-r--r--   0 anasbouzid  (1000) anasbouzid  (1000)   115648 2023-05-21 04:21:03.000000 streamlit-reveal-slides-0.1.1/reveal_slides/frontend/build/static/media/source-sans-pro-semibold.f11ba60a.woff
+-rw-r--r--   0 anasbouzid  (1000) anasbouzid  (1000)   240944 2023-05-21 04:21:03.000000 streamlit-reveal-slides-0.1.1/reveal_slides/frontend/build/static/media/source-sans-pro-semibolditalic.522a9ee9.ttf
+-rw-r--r--   0 anasbouzid  (1000) anasbouzid  (1000)    98816 2023-05-21 04:21:03.000000 streamlit-reveal-slides-0.1.1/reveal_slides/frontend/build/static/media/source-sans-pro-semibolditalic.a43f56ac.woff
+-rw-r--r--   0 anasbouzid  (1000) anasbouzid  (1000)    75706 2023-05-21 04:21:03.000000 streamlit-reveal-slides-0.1.1/reveal_slides/frontend/build/static/media/source-sans-pro-semibolditalic.fb03c660.eot
+-rw-r--r--   0 anasbouzid  (1000) anasbouzid  (1000)       38 2023-05-21 04:22:19.441717 streamlit-reveal-slides-0.1.1/setup.cfg
+-rw-r--r--   0 anasbouzid  (1000) anasbouzid  (1000)      764 2023-05-21 04:20:23.000000 streamlit-reveal-slides-0.1.1/setup.py
+drwxr-xr-x   0 anasbouzid  (1000) anasbouzid  (1000)        0 2023-05-21 04:22:19.441717 streamlit-reveal-slides-0.1.1/streamlit_reveal_slides.egg-info/
+-rw-r--r--   0 anasbouzid  (1000) anasbouzid  (1000)      393 2023-05-21 04:22:19.000000 streamlit-reveal-slides-0.1.1/streamlit_reveal_slides.egg-info/PKG-INFO
+-rw-r--r--   0 anasbouzid  (1000) anasbouzid  (1000)     6440 2023-05-21 04:22:19.000000 streamlit-reveal-slides-0.1.1/streamlit_reveal_slides.egg-info/SOURCES.txt
+-rw-r--r--   0 anasbouzid  (1000) anasbouzid  (1000)        1 2023-05-21 04:22:19.000000 streamlit-reveal-slides-0.1.1/streamlit_reveal_slides.egg-info/dependency_links.txt
+-rw-r--r--   0 anasbouzid  (1000) anasbouzid  (1000)       16 2023-05-21 04:22:19.000000 streamlit-reveal-slides-0.1.1/streamlit_reveal_slides.egg-info/requires.txt
+-rw-r--r--   0 anasbouzid  (1000) anasbouzid  (1000)       14 2023-05-21 04:22:19.000000 streamlit-reveal-slides-0.1.1/streamlit_reveal_slides.egg-info/top_level.txt
```

### Comparing `streamlit-reveal-slides-0.1.0/LICENSE` & `streamlit-reveal-slides-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `streamlit-reveal-slides-0.1.0/reveal_slides/__init__.py` & `streamlit-reveal-slides-0.1.1/reveal_slides/__init__.py`

 * *Files identical despite different names*

### Comparing `streamlit-reveal-slides-0.1.0/reveal_slides/frontend/build/asset-manifest.json` & `streamlit-reveal-slides-0.1.1/reveal_slides/frontend/build/asset-manifest.json`

 * *Files 1% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.8968750000000001%*

 * *Differences: {"'entrypoints'": "{insert: [(3, 'static/js/main.6641c370.chunk.js')], delete: [3]}",*

 * * "'files'": "{'main.js': './static/js/main.6641c370.chunk.js', 'main.js.map': "*

 * *            "'./static/js/main.6641c370.chunk.js.map'}"}*

```diff
@@ -1,18 +1,18 @@
 {
     "entrypoints": [
         "static/js/runtime-main.cda34e22.js",
         "static/css/2.5029ddca.chunk.css",
         "static/js/2.fc540633.chunk.js",
-        "static/js/main.c54401b6.chunk.js"
+        "static/js/main.6641c370.chunk.js"
     ],
     "files": {
         "index.html": "./index.html",
-        "main.js": "./static/js/main.c54401b6.chunk.js",
-        "main.js.map": "./static/js/main.c54401b6.chunk.js.map",
+        "main.js": "./static/js/main.6641c370.chunk.js",
+        "main.js.map": "./static/js/main.6641c370.chunk.js.map",
         "runtime-main.js": "./static/js/runtime-main.cda34e22.js",
         "runtime-main.js.map": "./static/js/runtime-main.cda34e22.js.map",
         "static/css/10.1f3244e3.chunk.css": "./static/css/10.1f3244e3.chunk.css",
         "static/css/10.1f3244e3.chunk.css.map": "./static/css/10.1f3244e3.chunk.css.map",
         "static/css/11.cb699f02.chunk.css": "./static/css/11.cb699f02.chunk.css",
         "static/css/11.cb699f02.chunk.css.map": "./static/css/11.cb699f02.chunk.css.map",
         "static/css/12.158b51eb.chunk.css": "./static/css/12.158b51eb.chunk.css",
```

### Comparing `streamlit-reveal-slides-0.1.0/reveal_slides/frontend/build/bootstrap.min.css` & `streamlit-reveal-slides-0.1.1/reveal_slides/frontend/build/bootstrap.min.css`

 * *Files identical despite different names*

### Comparing `streamlit-reveal-slides-0.1.0/reveal_slides/frontend/build/index.html` & `streamlit-reveal-slides-0.1.1/reveal_slides/frontend/build/index.html`

 * *Files 2% similar despite different names*

```diff
@@ -1 +1 @@
-<!doctype html><html lang="en"><head><title>Streamlit Component</title><meta charset="UTF-8"/><meta name="viewport" content="width=device-width,initial-scale=1"/><meta name="theme-color" content="#000000"/><meta name="description" content="Streamlit Component"/><link rel="stylesheet" href="bootstrap.min.css"/><link href="./static/css/2.5029ddca.chunk.css" rel="stylesheet"></head><body><noscript>You need to enable JavaScript to run this app.</noscript><div id="root" class="reveal"></div><script>!function(e){function t(t){for(var n,o,u=t[0],i=t[1],f=t[2],l=0,d=[];l<u.length;l++)o=u[l],Object.prototype.hasOwnProperty.call(a,o)&&a[o]&&d.push(a[o][0]),a[o]=0;for(n in i)Object.prototype.hasOwnProperty.call(i,n)&&(e[n]=i[n]);for(s&&s(t);d.length;)d.shift()();return c.push.apply(c,f||[]),r()}function r(){for(var e,t=0;t<c.length;t++){for(var r=c[t],n=!0,o=1;o<r.length;o++){var i=r[o];0!==a[i]&&(n=!1)}n&&(c.splice(t--,1),e=u(u.s=r[0]))}return e}var n={},o={1:0},a={1:0},c=[];function u(t){if(n[t])return n[t].exports;var r=n[t]={i:t,l:!1,exports:{}};return e[t].call(r.exports,r,r.exports,u),r.l=!0,r.exports}u.e=function(e){var t=[];o[e]?t.push(o[e]):0!==o[e]&&{3:1,4:1,5:1,6:1,7:1,8:1,9:1,10:1,11:1,12:1,13:1,14:1,15:1,16:1,17:1,18:1,19:1}[e]&&t.push(o[e]=new Promise((function(t,r){for(var n="static/css/"+({}[e]||e)+"."+{3:"11f8848d",4:"2fe0cb1b",5:"5a2b8ee3",6:"1b9cee33",7:"4e275de2",8:"eb5abf62",9:"1253a161",10:"1f3244e3",11:"cb699f02",12:"158b51eb",13:"74908590",14:"e64fc659",15:"3adba626",16:"b573d318",17:"10a8300f",18:"4eb3e38a",19:"74b97645"}[e]+".chunk.css",a=u.p+n,c=document.getElementsByTagName("link"),i=0;i<c.length;i++){var f=(s=c[i]).getAttribute("data-href")||s.getAttribute("href");if("stylesheet"===s.rel&&(f===n||f===a))return t()}var l=document.getElementsByTagName("style");for(i=0;i<l.length;i++){var s;if((f=(s=l[i]).getAttribute("data-href"))===n||f===a)return t()}var d=document.createElement("link");d.rel="stylesheet",d.type="text/css",d.onload=t,d.onerror=function(t){var n=t&&t.target&&t.target.src||a,c=new Error("Loading CSS chunk "+e+" failed.\n("+n+")");c.code="CSS_CHUNK_LOAD_FAILED",c.request=n,delete o[e],d.parentNode.removeChild(d),r(c)},d.href=a,document.getElementsByTagName("head")[0].appendChild(d)})).then((function(){o[e]=0})));var r=a[e];if(0!==r)if(r)t.push(r[2]);else{var n=new Promise((function(t,n){r=a[e]=[t,n]}));t.push(r[2]=n);var c,i=document.createElement("script");i.charset="utf-8",i.timeout=120,u.nc&&i.setAttribute("nonce",u.nc),i.src=function(e){return u.p+"static/js/"+({}[e]||e)+"."+{3:"c4d67f71",4:"71ecbbd1",5:"4c3c6aac",6:"2008461d",7:"69aea7e9",8:"86b27921",9:"fd893fed",10:"a3f9f257",11:"90f5ba01",12:"1edcaba5",13:"031e1745",14:"c2a62bd4",15:"257e774f",16:"a524310d",17:"c959c84a",18:"90e2d74e",19:"0abf949e"}[e]+".chunk.js"}(e);var f=new Error;c=function(t){i.onerror=i.onload=null,clearTimeout(l);var r=a[e];if(0!==r){if(r){var n=t&&("load"===t.type?"missing":t.type),o=t&&t.target&&t.target.src;f.message="Loading chunk "+e+" failed.\n("+n+": "+o+")",f.name="ChunkLoadError",f.type=n,f.request=o,r[1](f)}a[e]=void 0}};var l=setTimeout((function(){c({type:"timeout",target:i})}),12e4);i.onerror=i.onload=c,document.head.appendChild(i)}return Promise.all(t)},u.m=e,u.c=n,u.d=function(e,t,r){u.o(e,t)||Object.defineProperty(e,t,{enumerable:!0,get:r})},u.r=function(e){"undefined"!=typeof Symbol&&Symbol.toStringTag&&Object.defineProperty(e,Symbol.toStringTag,{value:"Module"}),Object.defineProperty(e,"__esModule",{value:!0})},u.t=function(e,t){if(1&t&&(e=u(e)),8&t)return e;if(4&t&&"object"==typeof e&&e&&e.__esModule)return e;var r=Object.create(null);if(u.r(r),Object.defineProperty(r,"default",{enumerable:!0,value:e}),2&t&&"string"!=typeof e)for(var n in e)u.d(r,n,function(t){return e[t]}.bind(null,n));return r},u.n=function(e){var t=e&&e.__esModule?function(){return e.default}:function(){return e};return u.d(t,"a",t),t},u.o=function(e,t){return Object.prototype.hasOwnProperty.call(e,t)},u.p="./",u.oe=function(e){throw console.error(e),e};var i=this.webpackJsonpstreamlit_component_template=this.webpackJsonpstreamlit_component_template||[],f=i.push.bind(i);i.push=t,i=i.slice();for(var l=0;l<i.length;l++)t(i[l]);var s=f;r()}([])</script><script src="./static/js/2.fc540633.chunk.js"></script><script src="./static/js/main.c54401b6.chunk.js"></script></body></html>
+<!doctype html><html lang="en"><head><title>Streamlit Component</title><meta charset="UTF-8"/><meta name="viewport" content="width=device-width,initial-scale=1"/><meta name="theme-color" content="#000000"/><meta name="description" content="Streamlit Component"/><link rel="stylesheet" href="bootstrap.min.css"/><link href="./static/css/2.5029ddca.chunk.css" rel="stylesheet"></head><body><noscript>You need to enable JavaScript to run this app.</noscript><div id="root" class="reveal"></div><script>!function(e){function t(t){for(var n,o,u=t[0],i=t[1],f=t[2],l=0,d=[];l<u.length;l++)o=u[l],Object.prototype.hasOwnProperty.call(a,o)&&a[o]&&d.push(a[o][0]),a[o]=0;for(n in i)Object.prototype.hasOwnProperty.call(i,n)&&(e[n]=i[n]);for(s&&s(t);d.length;)d.shift()();return c.push.apply(c,f||[]),r()}function r(){for(var e,t=0;t<c.length;t++){for(var r=c[t],n=!0,o=1;o<r.length;o++){var i=r[o];0!==a[i]&&(n=!1)}n&&(c.splice(t--,1),e=u(u.s=r[0]))}return e}var n={},o={1:0},a={1:0},c=[];function u(t){if(n[t])return n[t].exports;var r=n[t]={i:t,l:!1,exports:{}};return e[t].call(r.exports,r,r.exports,u),r.l=!0,r.exports}u.e=function(e){var t=[];o[e]?t.push(o[e]):0!==o[e]&&{3:1,4:1,5:1,6:1,7:1,8:1,9:1,10:1,11:1,12:1,13:1,14:1,15:1,16:1,17:1,18:1,19:1}[e]&&t.push(o[e]=new Promise((function(t,r){for(var n="static/css/"+({}[e]||e)+"."+{3:"11f8848d",4:"2fe0cb1b",5:"5a2b8ee3",6:"1b9cee33",7:"4e275de2",8:"eb5abf62",9:"1253a161",10:"1f3244e3",11:"cb699f02",12:"158b51eb",13:"74908590",14:"e64fc659",15:"3adba626",16:"b573d318",17:"10a8300f",18:"4eb3e38a",19:"74b97645"}[e]+".chunk.css",a=u.p+n,c=document.getElementsByTagName("link"),i=0;i<c.length;i++){var f=(s=c[i]).getAttribute("data-href")||s.getAttribute("href");if("stylesheet"===s.rel&&(f===n||f===a))return t()}var l=document.getElementsByTagName("style");for(i=0;i<l.length;i++){var s;if((f=(s=l[i]).getAttribute("data-href"))===n||f===a)return t()}var d=document.createElement("link");d.rel="stylesheet",d.type="text/css",d.onload=t,d.onerror=function(t){var n=t&&t.target&&t.target.src||a,c=new Error("Loading CSS chunk "+e+" failed.\n("+n+")");c.code="CSS_CHUNK_LOAD_FAILED",c.request=n,delete o[e],d.parentNode.removeChild(d),r(c)},d.href=a,document.getElementsByTagName("head")[0].appendChild(d)})).then((function(){o[e]=0})));var r=a[e];if(0!==r)if(r)t.push(r[2]);else{var n=new Promise((function(t,n){r=a[e]=[t,n]}));t.push(r[2]=n);var c,i=document.createElement("script");i.charset="utf-8",i.timeout=120,u.nc&&i.setAttribute("nonce",u.nc),i.src=function(e){return u.p+"static/js/"+({}[e]||e)+"."+{3:"c4d67f71",4:"71ecbbd1",5:"4c3c6aac",6:"2008461d",7:"69aea7e9",8:"86b27921",9:"fd893fed",10:"a3f9f257",11:"90f5ba01",12:"1edcaba5",13:"031e1745",14:"c2a62bd4",15:"257e774f",16:"a524310d",17:"c959c84a",18:"90e2d74e",19:"0abf949e"}[e]+".chunk.js"}(e);var f=new Error;c=function(t){i.onerror=i.onload=null,clearTimeout(l);var r=a[e];if(0!==r){if(r){var n=t&&("load"===t.type?"missing":t.type),o=t&&t.target&&t.target.src;f.message="Loading chunk "+e+" failed.\n("+n+": "+o+")",f.name="ChunkLoadError",f.type=n,f.request=o,r[1](f)}a[e]=void 0}};var l=setTimeout((function(){c({type:"timeout",target:i})}),12e4);i.onerror=i.onload=c,document.head.appendChild(i)}return Promise.all(t)},u.m=e,u.c=n,u.d=function(e,t,r){u.o(e,t)||Object.defineProperty(e,t,{enumerable:!0,get:r})},u.r=function(e){"undefined"!=typeof Symbol&&Symbol.toStringTag&&Object.defineProperty(e,Symbol.toStringTag,{value:"Module"}),Object.defineProperty(e,"__esModule",{value:!0})},u.t=function(e,t){if(1&t&&(e=u(e)),8&t)return e;if(4&t&&"object"==typeof e&&e&&e.__esModule)return e;var r=Object.create(null);if(u.r(r),Object.defineProperty(r,"default",{enumerable:!0,value:e}),2&t&&"string"!=typeof e)for(var n in e)u.d(r,n,function(t){return e[t]}.bind(null,n));return r},u.n=function(e){var t=e&&e.__esModule?function(){return e.default}:function(){return e};return u.d(t,"a",t),t},u.o=function(e,t){return Object.prototype.hasOwnProperty.call(e,t)},u.p="./",u.oe=function(e){throw console.error(e),e};var i=this.webpackJsonpstreamlit_component_template=this.webpackJsonpstreamlit_component_template||[],f=i.push.bind(i);i.push=t,i=i.slice();for(var l=0;l<i.length;l++)t(i[l]);var s=f;r()}([])</script><script src="./static/js/2.fc540633.chunk.js"></script><script src="./static/js/main.6641c370.chunk.js"></script></body></html>
```

### Comparing `streamlit-reveal-slides-0.1.0/reveal_slides/frontend/build/static/css/10.1f3244e3.chunk.css` & `streamlit-reveal-slides-0.1.1/reveal_slides/frontend/build/static/css/10.1f3244e3.chunk.css`

 * *Files identical despite different names*

### Comparing `streamlit-reveal-slides-0.1.0/reveal_slides/frontend/build/static/css/10.1f3244e3.chunk.css.map` & `streamlit-reveal-slides-0.1.1/reveal_slides/frontend/build/static/css/10.1f3244e3.chunk.css.map`

 * *Files identical despite different names*

### Comparing `streamlit-reveal-slides-0.1.0/reveal_slides/frontend/build/static/css/11.cb699f02.chunk.css` & `streamlit-reveal-slides-0.1.1/reveal_slides/frontend/build/static/css/11.cb699f02.chunk.css`

 * *Files identical despite different names*

### Comparing `streamlit-reveal-slides-0.1.0/reveal_slides/frontend/build/static/css/11.cb699f02.chunk.css.map` & `streamlit-reveal-slides-0.1.1/reveal_slides/frontend/build/static/css/11.cb699f02.chunk.css.map`

 * *Files identical despite different names*

### Comparing `streamlit-reveal-slides-0.1.0/reveal_slides/frontend/build/static/css/12.158b51eb.chunk.css` & `streamlit-reveal-slides-0.1.1/reveal_slides/frontend/build/static/css/12.158b51eb.chunk.css`

 * *Files identical despite different names*

### Comparing `streamlit-reveal-slides-0.1.0/reveal_slides/frontend/build/static/css/12.158b51eb.chunk.css.map` & `streamlit-reveal-slides-0.1.1/reveal_slides/frontend/build/static/css/12.158b51eb.chunk.css.map`

 * *Files identical despite different names*

### Comparing `streamlit-reveal-slides-0.1.0/reveal_slides/frontend/build/static/css/13.74908590.chunk.css` & `streamlit-reveal-slides-0.1.1/reveal_slides/frontend/build/static/css/13.74908590.chunk.css`

 * *Files identical despite different names*

### Comparing `streamlit-reveal-slides-0.1.0/reveal_slides/frontend/build/static/css/13.74908590.chunk.css.map` & `streamlit-reveal-slides-0.1.1/reveal_slides/frontend/build/static/css/13.74908590.chunk.css.map`

 * *Files identical despite different names*

### Comparing `streamlit-reveal-slides-0.1.0/reveal_slides/frontend/build/static/css/14.e64fc659.chunk.css` & `streamlit-reveal-slides-0.1.1/reveal_slides/frontend/build/static/css/14.e64fc659.chunk.css`

 * *Files identical despite different names*

### Comparing `streamlit-reveal-slides-0.1.0/reveal_slides/frontend/build/static/css/14.e64fc659.chunk.css.map` & `streamlit-reveal-slides-0.1.1/reveal_slides/frontend/build/static/css/14.e64fc659.chunk.css.map`

 * *Files identical despite different names*

### Comparing `streamlit-reveal-slides-0.1.0/reveal_slides/frontend/build/static/css/15.3adba626.chunk.css` & `streamlit-reveal-slides-0.1.1/reveal_slides/frontend/build/static/css/15.3adba626.chunk.css`

 * *Files identical despite different names*

### Comparing `streamlit-reveal-slides-0.1.0/reveal_slides/frontend/build/static/css/15.3adba626.chunk.css.map` & `streamlit-reveal-slides-0.1.1/reveal_slides/frontend/build/static/css/15.3adba626.chunk.css.map`

 * *Files identical despite different names*

### Comparing `streamlit-reveal-slides-0.1.0/reveal_slides/frontend/build/static/css/16.b573d318.chunk.css` & `streamlit-reveal-slides-0.1.1/reveal_slides/frontend/build/static/css/16.b573d318.chunk.css`

 * *Files identical despite different names*

### Comparing `streamlit-reveal-slides-0.1.0/reveal_slides/frontend/build/static/css/16.b573d318.chunk.css.map` & `streamlit-reveal-slides-0.1.1/reveal_slides/frontend/build/static/css/16.b573d318.chunk.css.map`

 * *Files identical despite different names*

### Comparing `streamlit-reveal-slides-0.1.0/reveal_slides/frontend/build/static/css/17.10a8300f.chunk.css.map` & `streamlit-reveal-slides-0.1.1/reveal_slides/frontend/build/static/css/17.10a8300f.chunk.css.map`

 * *Files identical despite different names*

### Comparing `streamlit-reveal-slides-0.1.0/reveal_slides/frontend/build/static/css/18.4eb3e38a.chunk.css` & `streamlit-reveal-slides-0.1.1/reveal_slides/frontend/build/static/css/18.4eb3e38a.chunk.css`

 * *Files identical despite different names*

### Comparing `streamlit-reveal-slides-0.1.0/reveal_slides/frontend/build/static/css/18.4eb3e38a.chunk.css.map` & `streamlit-reveal-slides-0.1.1/reveal_slides/frontend/build/static/css/18.4eb3e38a.chunk.css.map`

 * *Files identical despite different names*

### Comparing `streamlit-reveal-slides-0.1.0/reveal_slides/frontend/build/static/css/19.74b97645.chunk.css` & `streamlit-reveal-slides-0.1.1/reveal_slides/frontend/build/static/css/19.74b97645.chunk.css`

 * *Files identical despite different names*

### Comparing `streamlit-reveal-slides-0.1.0/reveal_slides/frontend/build/static/css/19.74b97645.chunk.css.map` & `streamlit-reveal-slides-0.1.1/reveal_slides/frontend/build/static/css/19.74b97645.chunk.css.map`

 * *Files identical despite different names*

### Comparing `streamlit-reveal-slides-0.1.0/reveal_slides/frontend/build/static/css/2.5029ddca.chunk.css` & `streamlit-reveal-slides-0.1.1/reveal_slides/frontend/build/static/css/2.5029ddca.chunk.css`

 * *Files identical despite different names*

### Comparing `streamlit-reveal-slides-0.1.0/reveal_slides/frontend/build/static/css/2.5029ddca.chunk.css.map` & `streamlit-reveal-slides-0.1.1/reveal_slides/frontend/build/static/css/2.5029ddca.chunk.css.map`

 * *Files identical despite different names*

### Comparing `streamlit-reveal-slides-0.1.0/reveal_slides/frontend/build/static/css/3.11f8848d.chunk.css` & `streamlit-reveal-slides-0.1.1/reveal_slides/frontend/build/static/css/3.11f8848d.chunk.css`

 * *Files identical despite different names*

### Comparing `streamlit-reveal-slides-0.1.0/reveal_slides/frontend/build/static/css/3.11f8848d.chunk.css.map` & `streamlit-reveal-slides-0.1.1/reveal_slides/frontend/build/static/css/3.11f8848d.chunk.css.map`

 * *Files identical despite different names*

### Comparing `streamlit-reveal-slides-0.1.0/reveal_slides/frontend/build/static/css/4.2fe0cb1b.chunk.css` & `streamlit-reveal-slides-0.1.1/reveal_slides/frontend/build/static/css/4.2fe0cb1b.chunk.css`

 * *Files identical despite different names*

### Comparing `streamlit-reveal-slides-0.1.0/reveal_slides/frontend/build/static/css/4.2fe0cb1b.chunk.css.map` & `streamlit-reveal-slides-0.1.1/reveal_slides/frontend/build/static/css/4.2fe0cb1b.chunk.css.map`

 * *Files identical despite different names*

### Comparing `streamlit-reveal-slides-0.1.0/reveal_slides/frontend/build/static/css/5.5a2b8ee3.chunk.css` & `streamlit-reveal-slides-0.1.1/reveal_slides/frontend/build/static/css/5.5a2b8ee3.chunk.css`

 * *Files identical despite different names*

### Comparing `streamlit-reveal-slides-0.1.0/reveal_slides/frontend/build/static/css/5.5a2b8ee3.chunk.css.map` & `streamlit-reveal-slides-0.1.1/reveal_slides/frontend/build/static/css/5.5a2b8ee3.chunk.css.map`

 * *Files identical despite different names*

### Comparing `streamlit-reveal-slides-0.1.0/reveal_slides/frontend/build/static/css/6.1b9cee33.chunk.css` & `streamlit-reveal-slides-0.1.1/reveal_slides/frontend/build/static/css/6.1b9cee33.chunk.css`

 * *Files identical despite different names*

### Comparing `streamlit-reveal-slides-0.1.0/reveal_slides/frontend/build/static/css/6.1b9cee33.chunk.css.map` & `streamlit-reveal-slides-0.1.1/reveal_slides/frontend/build/static/css/6.1b9cee33.chunk.css.map`

 * *Files identical despite different names*

### Comparing `streamlit-reveal-slides-0.1.0/reveal_slides/frontend/build/static/css/7.4e275de2.chunk.css` & `streamlit-reveal-slides-0.1.1/reveal_slides/frontend/build/static/css/7.4e275de2.chunk.css`

 * *Files identical despite different names*

### Comparing `streamlit-reveal-slides-0.1.0/reveal_slides/frontend/build/static/css/7.4e275de2.chunk.css.map` & `streamlit-reveal-slides-0.1.1/reveal_slides/frontend/build/static/css/7.4e275de2.chunk.css.map`

 * *Files identical despite different names*

### Comparing `streamlit-reveal-slides-0.1.0/reveal_slides/frontend/build/static/css/8.eb5abf62.chunk.css` & `streamlit-reveal-slides-0.1.1/reveal_slides/frontend/build/static/css/8.eb5abf62.chunk.css`

 * *Files identical despite different names*

### Comparing `streamlit-reveal-slides-0.1.0/reveal_slides/frontend/build/static/css/8.eb5abf62.chunk.css.map` & `streamlit-reveal-slides-0.1.1/reveal_slides/frontend/build/static/css/8.eb5abf62.chunk.css.map`

 * *Files identical despite different names*

### Comparing `streamlit-reveal-slides-0.1.0/reveal_slides/frontend/build/static/css/9.1253a161.chunk.css` & `streamlit-reveal-slides-0.1.1/reveal_slides/frontend/build/static/css/9.1253a161.chunk.css`

 * *Files identical despite different names*

### Comparing `streamlit-reveal-slides-0.1.0/reveal_slides/frontend/build/static/css/9.1253a161.chunk.css.map` & `streamlit-reveal-slides-0.1.1/reveal_slides/frontend/build/static/css/9.1253a161.chunk.css.map`

 * *Files identical despite different names*

### Comparing `streamlit-reveal-slides-0.1.0/reveal_slides/frontend/build/static/js/2.fc540633.chunk.js` & `streamlit-reveal-slides-0.1.1/reveal_slides/frontend/build/static/js/2.fc540633.chunk.js`

 * *Files identical despite different names*

### Comparing `streamlit-reveal-slides-0.1.0/reveal_slides/frontend/build/static/js/2.fc540633.chunk.js.LICENSE.txt` & `streamlit-reveal-slides-0.1.1/reveal_slides/frontend/build/static/js/2.fc540633.chunk.js.LICENSE.txt`

 * *Files identical despite different names*

### Comparing `streamlit-reveal-slides-0.1.0/reveal_slides/frontend/build/static/js/2.fc540633.chunk.js.map` & `streamlit-reveal-slides-0.1.1/reveal_slides/frontend/build/static/js/2.fc540633.chunk.js.map`

 * *Files identical despite different names*

### Comparing `streamlit-reveal-slides-0.1.0/reveal_slides/frontend/build/static/js/main.c54401b6.chunk.js` & `streamlit-reveal-slides-0.1.1/reveal_slides/frontend/build/static/js/main.6641c370.chunk.js`

 * *Files 6% similar despite different names*

#### js-beautify {}

```diff
@@ -48,29 +48,29 @@
                 l = a(6),
                 u = a(14),
                 h = a.n(u),
                 f = a(33),
                 d = a.n(f),
                 v = a(18),
                 g = a.n(v),
-                p = a(34),
-                m = a.n(p),
+                m = a(34),
+                p = a.n(m),
                 b = a(35),
-                y = a.n(b),
-                w = a(36),
-                j = a.n(w),
+                w = a.n(b),
+                y = a(36),
+                j = a.n(y),
                 O = (a(62), a(63), a(11)),
                 x = {
                     RevealMarkdown: h.a,
                     RevealHighlight: d.a,
                     "RevealMath.KaTeX": g.a.KaTeX,
                     "RevealMath.MathJax2": g.a.MathJax2,
                     "RevealMath.MathJax3": g.a.MathJax3,
-                    RevealSearch: m.a,
-                    RevealNotes: y.a,
+                    RevealSearch: p.a,
+                    RevealNotes: w.a,
                     RevealZoom: j.a
                 },
                 _ = Object(r.b)((function(e) {
                     var t = e.args,
                         s = e.disabled,
                         o = JSON.stringify(t.config),
                         i = function(e) {
@@ -139,19 +139,19 @@
                         var e = i();
                         l.a.configure(e)
                     }), [o, t.allow_unsafe_html]), Object(n.useEffect)((function() {
                         if (l.a.isReady())
                             if (s) {
                                 l.a.togglePause(!0);
                                 var e = l.a.getViewportElement();
-                                e && (e.style.pointerEvents = "none", e.style.cursor = "not-allowed", e.style.opacity = "0.5")
+                                e && (e.style.pointerEvents = "none")
                             } else {
                                 l.a.togglePause(!1);
                                 var t = l.a.getViewportElement();
-                                t && (t.style.pointerEvents = "auto", t.style.cursor = "auto", t.style.opacity = "1")
+                                t && (t.style.pointerEvents = "auto")
                             }
                     }), [s]);
                     var u = new ResizeObserver((function(e) {
                             var a;
                             "auto" === t.height || "number" !== typeof t.height ? (r.a.setFrameHeight(null !== (a = e[0].contentBoxSize.blockSize) && void 0 !== a ? a : e[0].contentRect.height), l.a.isReady() && l.a.layout()) : (r.a.setFrameHeight(t.height), l.a.isReady() && l.a.layout())
                         })),
                         f = function(e) {
@@ -181,8 +181,8 @@
             }), document.getElementById("root"))
         }
     },
     [
         [66, 1, 2]
     ]
 ]);
-//# sourceMappingURL=main.c54401b6.chunk.js.map
+//# sourceMappingURL=main.6641c370.chunk.js.map
```

### Comparing `streamlit-reveal-slides-0.1.0/reveal_slides/frontend/build/static/js/main.c54401b6.chunk.js.map` & `streamlit-reveal-slides-0.1.1/reveal_slides/frontend/build/static/js/main.6641c370.chunk.js.map`

 * *Files 4% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.8201058201058201%*

 * *Differences: {"'file'": "'static/js/main.6641c370.chunk.js'",*

 * * "'mappings'": "'gIAAA,IAAIA,EAAM,CACT,cAAe,CACd,GACA,GAED,uBAAwB,CACvB,GACA,IAED,cAAe,CACd,GACA,IAED,cAAe,CACd,GACA,IAED,gBAAiB,CAChB,GACA,IAED,0CAA2C,CAC1C,GACA,IAED,8CAA+C,CAC9C,GACA,IAED,eAAgB,CACf,GACA,GAED,aAAc,CACb,GACA,GAED,cAAe,CACd,GACA,GAED,cAAe,CACd,GACA,IAED,eAAgB,CACf,GACA,GAED,YAAa,CACZ,GACA,GAED,kBAAmB,CAClB,GACA,GAED,uBAAwB,CACvB,GACA,IAED,cAAe,CACd,GACA,IAED,gDAAiD,CAChD,GACA,KAGF,SAASC,EAAoBC,GAC5B,IAAIC,EAAoBC,EAAEJ,EAAKE,GAC9B,OAAOG,QAAQC […]*

```diff
@@ -1,10 +1,10 @@
 {
-    "file": "static/js/main.c54401b6.chunk.js",
-    "mappings": "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",
+    "file": "static/js/main.6641c370.chunk.js",
+    "mappings": "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",
     "names": [
         "map",
         "webpackAsyncContext",
         "req",
         "__webpack_require__",
         "o",
         "Promise",
@@ -77,16 +77,14 @@
         "configure",
         "isReady",
         "togglePause",
         "viewport",
         "getViewportElement",
         "style",
         "pointerEvents",
-        "cursor",
-        "opacity",
         "resizeObserver",
         "ResizeObserver",
         "entries",
         "_entries$0$contentBox",
         "setFrameHeight",
         "contentBoxSize",
         "blockSize",
@@ -115,12 +113,12 @@
     "sources": [
         "../node_modules/reveal.js/dist/theme lazy /^/.//.*/.css$/ groupOptions: {} namespace object",
         "RevealSlides.tsx",
         "index.tsx"
     ],
     "sourcesContent": [
         "var map = {\n\t\"./beige.css\": [\n\t\t67,\n\t\t3\n\t],\n\t\"./black-contrast.css\": [\n\t\t68,\n\t\t10\n\t],\n\t\"./black.css\": [\n\t\t69,\n\t\t11\n\t],\n\t\"./blood.css\": [\n\t\t70,\n\t\t12\n\t],\n\t\"./dracula.css\": [\n\t\t71,\n\t\t16\n\t],\n\t\"./fonts/league-gothic/league-gothic.css\": [\n\t\t72,\n\t\t17\n\t],\n\t\"./fonts/source-sans-pro/source-sans-pro.css\": [\n\t\t73,\n\t\t18\n\t],\n\t\"./league.css\": [\n\t\t74,\n\t\t4\n\t],\n\t\"./moon.css\": [\n\t\t75,\n\t\t5\n\t],\n\t\"./night.css\": [\n\t\t76,\n\t\t6\n\t],\n\t\"./serif.css\": [\n\t\t77,\n\t\t19\n\t],\n\t\"./simple.css\": [\n\t\t78,\n\t\t7\n\t],\n\t\"./sky.css\": [\n\t\t79,\n\t\t8\n\t],\n\t\"./solarized.css\": [\n\t\t80,\n\t\t9\n\t],\n\t\"./white-contrast.css\": [\n\t\t81,\n\t\t13\n\t],\n\t\"./white.css\": [\n\t\t82,\n\t\t14\n\t],\n\t\"./white_contrast_compact_verbatim_headers.css\": [\n\t\t83,\n\t\t15\n\t]\n};\nfunction webpackAsyncContext(req) {\n\tif(!__webpack_require__.o(map, req)) {\n\t\treturn Promise.resolve().then(function() {\n\t\t\tvar e = new Error(\"Cannot find module '\" + req + \"'\");\n\t\t\te.code = 'MODULE_NOT_FOUND';\n\t\t\tthrow e;\n\t\t});\n\t}\n\n\tvar ids = map[req], id = ids[0];\n\treturn __webpack_require__.e(ids[1]).then(function() {\n\t\treturn __webpack_require__.t(id, 7);\n\t});\n}\nwebpackAsyncContext.keys = function webpackAsyncContextKeys() {\n\treturn Object.keys(map);\n};\nwebpackAsyncContext.id = 65;\nmodule.exports = webpackAsyncContext;",
-        "import {\n  Streamlit,\n  ComponentProps,\n  withStreamlitConnection,\n  Theme,\n} from \"streamlit-component-lib\"\nimport { useEffect, useMemo } from \"react\"\n\n\nimport Reveal from 'reveal.js';\nimport RevealMarkdown from 'reveal.js/plugin/markdown/markdown';\nimport RevealHighlight from 'reveal.js/plugin/highlight/highlight';\nimport RevealMath from 'reveal.js/plugin/math/math';\nimport RevealSearch from 'reveal.js/plugin/search/search';\nimport RevealNotes from 'reveal.js/plugin/notes/notes';\nimport RevealZoom from 'reveal.js/plugin/zoom/zoom';\n\n\nimport 'reveal.js/dist/reveal.css';\nimport 'reveal.js/plugin/highlight/monokai.css';\n\ninterface RevealSlidesProps extends ComponentProps {\n  args: any\n  width: number\n  disabled: boolean\n  theme?: Theme\n}\n\nconst includedPlugins = {\"RevealMarkdown\": RevealMarkdown, \"RevealHighlight\": RevealHighlight, \"RevealMath.KaTeX\": RevealMath.KaTeX, \"RevealMath.MathJax2\": RevealMath.MathJax2, \"RevealMath.MathJax3\": RevealMath.MathJax3, \"RevealSearch\": RevealSearch, \"RevealNotes\": RevealNotes, \"RevealZoom\": RevealZoom}\n// const simpleCommands = {\"left\": Reveal.left, \"right\": () => {Reveal.right()}, \"up\": Reveal.up, \"down\": Reveal.down, \"prev\": Reveal.prev, \"next\": Reveal.next, \"prevFragment\": Reveal.prevFragment, \"nextFragment\": Reveal.nextFragment, \"togglePause\": Reveal.togglePause, \"toggleAutoSlide\": Reveal.toggleAutoSlide, \"toggleHelp\": Reveal.toggleHelp, \"toggleOverview\": Reveal.toggleOverview, \"shuffle\": Reveal.shuffle}\n// const commandsWithArgs = {slide: Reveal.slide, togglePause: Reveal.togglePause, toggleAutoSlide: Reveal.toggleAutoSlide, toggleHelp: Reveal.toggleHelp, toggleOverview: Reveal.toggleOverview}\n\n\n/**\n * This is a React-based component template. The `render()` function is called\n * automatically when your component should be re-rendered.\n */\nconst RevealSlides = ({ args, disabled }: RevealSlidesProps) => {   \n\n  let configStr = JSON.stringify(args[\"config\"])\n  // const commandStr = JSON.stringify(args[\"commands\"])\n\n  const setupConfig = (configString: string) : object => {\n    const config = JSON.parse(configStr)\n    // code to run after render goes here\n    if (args[\"allow_unsafe_html\"]) {\n      // do nothing\n    }\n    else {\n      if ('plugins' in config){\n        var arr = config['plugins'];\n        arr.forEach(function(moduleName: string, index: number) {\n          if (moduleName in includedPlugins){\n            arr[index] = (includedPlugins as any)[moduleName];\n          }\n          else {\n            arr[index] = null;\n          }\n        });\n        config['plugins'] = arr.filter((x:any) => !!x) as any[];\n        if(!config['plugins'].includes(RevealMarkdown)){\n          config['plugins'].push(RevealMarkdown);\n        }\n      }\n      else {\n        config['plugins'] = [RevealMarkdown];\n      }\n    }\n    return config;\n  }\n\n  useMemo(()=>{\n    // code to run on component mount goes here\n\n    // To do: remove or disable previously imported css. When the list of\n    // css imports exceed about 25, the page no longer updates.\n    import('../node_modules/reveal.js/dist/theme/' + args.theme + '.css')\n\n    // To do: figure out a way to get a callback after new css is applied\n    // The following code is a hack to get around the fact that the new css\n    // is not applied immediately\n    setTimeout(() => {\n      try{\n        Reveal.layout();\n      }\n      catch (e){\n        console.warn(\"Reveal.layout() call failed.\")\n      }\n    }, 100);\n\n  }, [args.theme]);\n\n  useEffect(() => {\n    const config = setupConfig(configStr)\n    \n    try {\n      Reveal.destroy();\n    }\n    catch (e) {\n    }\n    Reveal.initialize(config).then(() => {\n      // reveal.js is ready \n\n    // For some yet to be determined reason, the highlight plugin is not initialized.\n    // Setting highlight config option highlightOnLoad to true (before passing to initialize function)\n    // does not work\n    // To Do: make sure the highlight plugin only changes the HTML involving the code once instead of many times.\n    // Possible solution is to make a change to the plugin init function.\n    let highlighter = Reveal.getPlugin('highlight') as any;\n    if (highlighter){\n      highlighter.init(Reveal);\n    }\n\n      // Send slide position indecies back to Streamlit on initialization and on slide change\n      const currState = Reveal.getState();\n      Streamlit.setComponentValue(currState);\n      Reveal.on( 'slidechanged', event => {\n\n        const tempState = Reveal.getState();\n        Streamlit.setComponentValue({indexh: (event as any).indexh, indexv: (event as any).indexv, indexf: tempState.indexf, paused: tempState.paused, overview: tempState.overview});\n      });\n      \n      Reveal.on( 'fragmentshown', event => {\n        // event.fragment = the fragment DOM element\n        const tempState = Reveal.getState();\n        Streamlit.setComponentValue(tempState);\n      } );\n      Reveal.on( 'fragmenthidden', event => {\n        // event.fragment = the fragment DOM element\n        const tempState = Reveal.getState();\n        Streamlit.setComponentValue(tempState);\n      } );\n      Reveal.on( 'overviewshown', event => {\n        // event.overview = the overview DOM element\n        const tempState = Reveal.getState();\n        Streamlit.setComponentValue(tempState);\n      } );\n      Reveal.on( 'overviewhidden', event => {\n        // event.overview = the overview DOM element\n        const tempState = Reveal.getState();\n        Streamlit.setComponentValue(tempState);\n      } );\n      Reveal.on( 'paused', event => {\n        // event.fragment = the fragment DOM element\n        const tempState = Reveal.getState();\n        Streamlit.setComponentValue(tempState);\n      } );\n      Reveal.on( 'resumed', event => {\n        // event.fragment = the fragment DOM element\n        const tempState = Reveal.getState();\n        Streamlit.setComponentValue(tempState);\n      } );\n\n    });\n\n    return () => {\n      // code to run on component unmount goes here\n      Reveal.destroy();  \n    }\n  }, []);\n\n  useEffect(() => {\n    const config = setupConfig(configStr)\n    Reveal.configure(config);\n  }, [configStr, args[\"allow_unsafe_html\"]]);\n\n  useEffect(() => {\n    if (Reveal.isReady()){\n      if (disabled){\n        Reveal.togglePause(true);\n        let viewport = Reveal.getViewportElement();\n        if (viewport){\n          viewport.style.pointerEvents = \"none\";\n          viewport.style.cursor = \"not-allowed\";\n          viewport.style.opacity = \"0.5\";\n        }\n      }\n      else {  \n        Reveal.togglePause(false);\n        let viewport = Reveal.getViewportElement();\n        if (viewport){\n          viewport.style.pointerEvents = \"auto\";\n          viewport.style.cursor = \"auto\";\n          viewport.style.opacity = \"1\";\n        }\n      }\n    }\n  }, [disabled]);\n\n  //To do: add support for commands (i.e. control slides from Streamlit)\n  //-----------------\n  // useEffect(() => {\n  //   const commands = JSON.parse(commandStr)\n  //   if (Array.isArray(commands) && commands.length > 0 && Reveal.isReady()){\n  //     commands.forEach((command: any) => {\n  //       if (typeof command === \"string\" && command in simpleCommands){\n  //         (simpleCommands as any)[command]();\n  //       }\n  //       else if (Array.isArray(command) && command.length > 0 && typeof command[0] === \"string\" && command[0] in commandsWithArgs){\n  //         if (command[0] === \"slide\"){\n  //           if (command.length === 3){\n  //             Reveal.slide(command[1], command[2]);\n  //           }\n  //           else if (command.length === 4){\n  //             Reveal.slide(command[1], command[2], command[3]);\n  //           }\n  //           else {\n  //             console.warn(\"Invalid slide command: slide command array must have 3 or 4 elements.\");\n  //           }\n  //         }\n  //         else {\n  //           (commandsWithArgs as any)[command[0]](command[1]);\n  //         }\n  //       }\n  //       else {\n  //         console.warn(\"Invalid command: command must be a string or an array containing a string as its first element.\");\n  //       }\n  //     });\n  //   }\n  //   else if (!Array.isArray(args[\"commands\"])) {\n  //     console.warn(\"Invalid commands property value: commands must be an array containing at least one command.\");\n  //   }\n  // }, [commandStr]);\n\n  /**\n   * resizeObserver observes changes in elements its given to observe and is used here\n   * to communicate to streamlit the height of the component that has changed\n   * so that streamlit can adjust the iframe containing the component accordingly.\n   */\n  const resizeObserver = new ResizeObserver((entries: any) => {\n    // If we know that the body will always fully contain our component (without cutting it off)\n    // then we can use docuemnt.body height instead\n    if (args[\"height\"] === \"auto\" || typeof args[\"height\"] !== \"number\"){\n      Streamlit.setFrameHeight((entries[0].contentBoxSize.blockSize ?? entries[0].contentRect.height)); \n      if (Reveal.isReady()){\n        Reveal.layout();\n      }\n    }\n    else {\n      Streamlit.setFrameHeight(args[\"height\"]);\n      if (Reveal.isReady()){\n        Reveal.layout();\n      }\n    }\n    \n  })\n\n  const observe = (divElem: any) => {\n    divElem ? resizeObserver.observe(divElem as HTMLDivElement) : resizeObserver.disconnect();\n  }\n\n  if (args[\"allow_unsafe_html\"]) {\n    return (\n      <div ref={observe} className=\"slides\" dangerouslySetInnerHTML={{__html: args[\"content\"]}}>\n      </div>\n    )\n  }\n  else {\n    return (\n      <div ref={observe} className=\"slides\">\n        <section data-markdown={\"\"} {...args[\"markdown_props\"]}>\n          <script type={\"text/template\"}>\n          {args[\"content\"]}\n          </script>\n        </section>\n      </div>\n    )\n  }\n}\n\n// \"withStreamlitConnection\" is a wrapper function. It bootstraps the\n// connection between your component and the Streamlit app, and handles\n// passing arguments from Python -> Component.\n//\n// You don't need to edit withStreamlitConnection (but you're welcome to!).\nexport default withStreamlitConnection(RevealSlides)\n",
+        "import {\n  Streamlit,\n  ComponentProps,\n  withStreamlitConnection,\n  Theme,\n} from \"streamlit-component-lib\"\nimport { useEffect, useMemo } from \"react\"\n\n\nimport Reveal from 'reveal.js';\nimport RevealMarkdown from 'reveal.js/plugin/markdown/markdown';\nimport RevealHighlight from 'reveal.js/plugin/highlight/highlight';\nimport RevealMath from 'reveal.js/plugin/math/math';\nimport RevealSearch from 'reveal.js/plugin/search/search';\nimport RevealNotes from 'reveal.js/plugin/notes/notes';\nimport RevealZoom from 'reveal.js/plugin/zoom/zoom';\n\n\nimport 'reveal.js/dist/reveal.css';\nimport 'reveal.js/plugin/highlight/monokai.css';\n\ninterface RevealSlidesProps extends ComponentProps {\n  args: any\n  width: number\n  disabled: boolean\n  theme?: Theme\n}\n\nconst includedPlugins = {\"RevealMarkdown\": RevealMarkdown, \"RevealHighlight\": RevealHighlight, \"RevealMath.KaTeX\": RevealMath.KaTeX, \"RevealMath.MathJax2\": RevealMath.MathJax2, \"RevealMath.MathJax3\": RevealMath.MathJax3, \"RevealSearch\": RevealSearch, \"RevealNotes\": RevealNotes, \"RevealZoom\": RevealZoom}\n// const simpleCommands = {\"left\": Reveal.left, \"right\": () => {Reveal.right()}, \"up\": Reveal.up, \"down\": Reveal.down, \"prev\": Reveal.prev, \"next\": Reveal.next, \"prevFragment\": Reveal.prevFragment, \"nextFragment\": Reveal.nextFragment, \"togglePause\": Reveal.togglePause, \"toggleAutoSlide\": Reveal.toggleAutoSlide, \"toggleHelp\": Reveal.toggleHelp, \"toggleOverview\": Reveal.toggleOverview, \"shuffle\": Reveal.shuffle}\n// const commandsWithArgs = {slide: Reveal.slide, togglePause: Reveal.togglePause, toggleAutoSlide: Reveal.toggleAutoSlide, toggleHelp: Reveal.toggleHelp, toggleOverview: Reveal.toggleOverview}\n\n\n/**\n * This is a React-based component template. The `render()` function is called\n * automatically when your component should be re-rendered.\n */\nconst RevealSlides = ({ args, disabled }: RevealSlidesProps) => {   \n\n  let configStr = JSON.stringify(args[\"config\"])\n  // const commandStr = JSON.stringify(args[\"commands\"])\n\n  const setupConfig = (configString: string) : object => {\n    const config = JSON.parse(configStr)\n    // code to run after render goes here\n    if (args[\"allow_unsafe_html\"]) {\n      // do nothing\n    }\n    else {\n      if ('plugins' in config){\n        var arr = config['plugins'];\n        arr.forEach(function(moduleName: string, index: number) {\n          if (moduleName in includedPlugins){\n            arr[index] = (includedPlugins as any)[moduleName];\n          }\n          else {\n            arr[index] = null;\n          }\n        });\n        config['plugins'] = arr.filter((x:any) => !!x) as any[];\n        if(!config['plugins'].includes(RevealMarkdown)){\n          config['plugins'].push(RevealMarkdown);\n        }\n      }\n      else {\n        config['plugins'] = [RevealMarkdown];\n      }\n    }\n    return config;\n  }\n\n  useMemo(()=>{\n    // code to run on component mount goes here\n\n    // To do: remove or disable previously imported css. When the list of\n    // css imports exceed about 25, the page no longer updates.\n    import('../node_modules/reveal.js/dist/theme/' + args.theme + '.css')\n\n    // To do: figure out a way to get a callback after new css is applied\n    // The following code is a hack to get around the fact that the new css\n    // is not applied immediately\n    setTimeout(() => {\n      try{\n        Reveal.layout();\n      }\n      catch (e){\n        console.warn(\"Reveal.layout() call failed.\")\n      }\n    }, 100);\n\n  }, [args.theme]);\n\n  useEffect(() => {\n    const config = setupConfig(configStr)\n    \n    try {\n      Reveal.destroy();\n    }\n    catch (e) {\n    }\n    Reveal.initialize(config).then(() => {\n      // reveal.js is ready \n\n    // For some yet to be determined reason, the highlight plugin is not initialized.\n    // Setting highlight config option highlightOnLoad to true (before passing to initialize function)\n    // does not work\n    // To Do: make sure the highlight plugin only changes the HTML involving the code once instead of many times.\n    // Possible solution is to make a change to the plugin init function.\n    let highlighter = Reveal.getPlugin('highlight') as any;\n    if (highlighter){\n      highlighter.init(Reveal);\n    }\n\n      // Send slide position indecies back to Streamlit on initialization and on slide change\n      const currState = Reveal.getState();\n      Streamlit.setComponentValue(currState);\n      Reveal.on( 'slidechanged', event => {\n\n        const tempState = Reveal.getState();\n        Streamlit.setComponentValue({indexh: (event as any).indexh, indexv: (event as any).indexv, indexf: tempState.indexf, paused: tempState.paused, overview: tempState.overview});\n      });\n      \n      Reveal.on( 'fragmentshown', event => {\n        // event.fragment = the fragment DOM element\n        const tempState = Reveal.getState();\n        Streamlit.setComponentValue(tempState);\n      } );\n      Reveal.on( 'fragmenthidden', event => {\n        // event.fragment = the fragment DOM element\n        const tempState = Reveal.getState();\n        Streamlit.setComponentValue(tempState);\n      } );\n      Reveal.on( 'overviewshown', event => {\n        // event.overview = the overview DOM element\n        const tempState = Reveal.getState();\n        Streamlit.setComponentValue(tempState);\n      } );\n      Reveal.on( 'overviewhidden', event => {\n        // event.overview = the overview DOM element\n        const tempState = Reveal.getState();\n        Streamlit.setComponentValue(tempState);\n      } );\n      Reveal.on( 'paused', event => {\n        // event.fragment = the fragment DOM element\n        const tempState = Reveal.getState();\n        Streamlit.setComponentValue(tempState);\n      } );\n      Reveal.on( 'resumed', event => {\n        // event.fragment = the fragment DOM element\n        const tempState = Reveal.getState();\n        Streamlit.setComponentValue(tempState);\n      } );\n\n    });\n\n    return () => {\n      // code to run on component unmount goes here\n      Reveal.destroy();  \n    }\n  }, []);\n\n  useEffect(() => {\n    const config = setupConfig(configStr)\n    Reveal.configure(config);\n  }, [configStr, args[\"allow_unsafe_html\"]]);\n\n  useEffect(() => {\n    if (Reveal.isReady()){\n      if (disabled){\n        Reveal.togglePause(true);\n        let viewport = Reveal.getViewportElement();\n        if (viewport){\n          viewport.style.pointerEvents = \"none\";\n        }\n      }\n      else {  \n        Reveal.togglePause(false);\n        let viewport = Reveal.getViewportElement();\n        if (viewport){\n          viewport.style.pointerEvents = \"auto\";\n        }\n      }\n    }\n  }, [disabled]);\n\n  //To do: add support for commands (i.e. control slides from Streamlit)\n  //-----------------\n  // useEffect(() => {\n  //   const commands = JSON.parse(commandStr)\n  //   if (Array.isArray(commands) && commands.length > 0 && Reveal.isReady()){\n  //     commands.forEach((command: any) => {\n  //       if (typeof command === \"string\" && command in simpleCommands){\n  //         (simpleCommands as any)[command]();\n  //       }\n  //       else if (Array.isArray(command) && command.length > 0 && typeof command[0] === \"string\" && command[0] in commandsWithArgs){\n  //         if (command[0] === \"slide\"){\n  //           if (command.length === 3){\n  //             Reveal.slide(command[1], command[2]);\n  //           }\n  //           else if (command.length === 4){\n  //             Reveal.slide(command[1], command[2], command[3]);\n  //           }\n  //           else {\n  //             console.warn(\"Invalid slide command: slide command array must have 3 or 4 elements.\");\n  //           }\n  //         }\n  //         else {\n  //           (commandsWithArgs as any)[command[0]](command[1]);\n  //         }\n  //       }\n  //       else {\n  //         console.warn(\"Invalid command: command must be a string or an array containing a string as its first element.\");\n  //       }\n  //     });\n  //   }\n  //   else if (!Array.isArray(args[\"commands\"])) {\n  //     console.warn(\"Invalid commands property value: commands must be an array containing at least one command.\");\n  //   }\n  // }, [commandStr]);\n\n  /**\n   * resizeObserver observes changes in elements its given to observe and is used here\n   * to communicate to streamlit the height of the component that has changed\n   * so that streamlit can adjust the iframe containing the component accordingly.\n   */\n  const resizeObserver = new ResizeObserver((entries: any) => {\n    // If we know that the body will always fully contain our component (without cutting it off)\n    // then we can use docuemnt.body height instead\n    if (args[\"height\"] === \"auto\" || typeof args[\"height\"] !== \"number\"){\n      Streamlit.setFrameHeight((entries[0].contentBoxSize.blockSize ?? entries[0].contentRect.height)); \n      if (Reveal.isReady()){\n        Reveal.layout();\n      }\n    }\n    else {\n      Streamlit.setFrameHeight(args[\"height\"]);\n      if (Reveal.isReady()){\n        Reveal.layout();\n      }\n    }\n    \n  })\n\n  const observe = (divElem: any) => {\n    divElem ? resizeObserver.observe(divElem as HTMLDivElement) : resizeObserver.disconnect();\n  }\n\n  if (args[\"allow_unsafe_html\"]) {\n    return (\n      <div ref={observe} className=\"slides\" dangerouslySetInnerHTML={{__html: args[\"content\"]}}>\n      </div>\n    )\n  }\n  else {\n    return (\n      <div ref={observe} className=\"slides\">\n        <section data-markdown={\"\"} {...args[\"markdown_props\"]}>\n          <script type={\"text/template\"}>\n          {args[\"content\"]}\n          </script>\n        </section>\n      </div>\n    )\n  }\n}\n\n// \"withStreamlitConnection\" is a wrapper function. It bootstraps the\n// connection between your component and the Streamlit app, and handles\n// passing arguments from Python -> Component.\n//\n// You don't need to edit withStreamlitConnection (but you're welcome to!).\nexport default withStreamlitConnection(RevealSlides)\n",
         "import React from \"react\"\nimport ReactDOM from \"react-dom\"\nimport RevealSlides from \"./RevealSlides\"\n\nReactDOM.render(\n  <React.StrictMode>\n    <RevealSlides />\n  </React.StrictMode>,\n  document.getElementById(\"root\")\n)\n"
     ],
     "version": 3
 }
```

### Comparing `streamlit-reveal-slides-0.1.0/reveal_slides/frontend/build/static/js/runtime-main.cda34e22.js` & `streamlit-reveal-slides-0.1.1/reveal_slides/frontend/build/static/js/runtime-main.cda34e22.js`

 * *Files identical despite different names*

### Comparing `streamlit-reveal-slides-0.1.0/reveal_slides/frontend/build/static/js/runtime-main.cda34e22.js.map` & `streamlit-reveal-slides-0.1.1/reveal_slides/frontend/build/static/js/runtime-main.cda34e22.js.map`

 * *Files identical despite different names*

### Comparing `streamlit-reveal-slides-0.1.0/reveal_slides/frontend/build/static/media/league-gothic.080eee2a.woff` & `streamlit-reveal-slides-0.1.1/reveal_slides/frontend/build/static/media/league-gothic.080eee2a.woff`

 * *Files identical despite different names*

### Comparing `streamlit-reveal-slides-0.1.0/reveal_slides/frontend/build/static/media/league-gothic.12baac5d.eot` & `streamlit-reveal-slides-0.1.1/reveal_slides/frontend/build/static/media/league-gothic.12baac5d.eot`

 * *Files identical despite different names*

### Comparing `streamlit-reveal-slides-0.1.0/reveal_slides/frontend/build/static/media/league-gothic.6ae91382.ttf` & `streamlit-reveal-slides-0.1.1/reveal_slides/frontend/build/static/media/league-gothic.6ae91382.ttf`

 * *Files identical despite different names*

### Comparing `streamlit-reveal-slides-0.1.0/reveal_slides/frontend/build/static/media/source-sans-pro-italic.10a5cb40.ttf` & `streamlit-reveal-slides-0.1.1/reveal_slides/frontend/build/static/media/source-sans-pro-italic.10a5cb40.ttf`

 * *Files identical despite different names*

### Comparing `streamlit-reveal-slides-0.1.0/reveal_slides/frontend/build/static/media/source-sans-pro-italic.97e79d3e.eot` & `streamlit-reveal-slides-0.1.1/reveal_slides/frontend/build/static/media/source-sans-pro-italic.97e79d3e.eot`

 * *Files identical despite different names*

### Comparing `streamlit-reveal-slides-0.1.0/reveal_slides/frontend/build/static/media/source-sans-pro-italic.983d97ca.woff` & `streamlit-reveal-slides-0.1.1/reveal_slides/frontend/build/static/media/source-sans-pro-italic.983d97ca.woff`

 * *Files identical despite different names*

### Comparing `streamlit-reveal-slides-0.1.0/reveal_slides/frontend/build/static/media/source-sans-pro-regular.36443d24.eot` & `streamlit-reveal-slides-0.1.1/reveal_slides/frontend/build/static/media/source-sans-pro-regular.36443d24.eot`

 * *Files identical despite different names*

### Comparing `streamlit-reveal-slides-0.1.0/reveal_slides/frontend/build/static/media/source-sans-pro-regular.45c54810.ttf` & `streamlit-reveal-slides-0.1.1/reveal_slides/frontend/build/static/media/source-sans-pro-regular.45c54810.ttf`

 * *Files identical despite different names*

### Comparing `streamlit-reveal-slides-0.1.0/reveal_slides/frontend/build/static/media/source-sans-pro-regular.d1653550.woff` & `streamlit-reveal-slides-0.1.1/reveal_slides/frontend/build/static/media/source-sans-pro-regular.d1653550.woff`

 * *Files identical despite different names*

### Comparing `streamlit-reveal-slides-0.1.0/reveal_slides/frontend/build/static/media/source-sans-pro-semibold.6ebea875.ttf` & `streamlit-reveal-slides-0.1.1/reveal_slides/frontend/build/static/media/source-sans-pro-semibold.6ebea875.ttf`

 * *Files identical despite different names*

### Comparing `streamlit-reveal-slides-0.1.0/reveal_slides/frontend/build/static/media/source-sans-pro-semibold.83db537e.eot` & `streamlit-reveal-slides-0.1.1/reveal_slides/frontend/build/static/media/source-sans-pro-semibold.83db537e.eot`

 * *Files identical despite different names*

### Comparing `streamlit-reveal-slides-0.1.0/reveal_slides/frontend/build/static/media/source-sans-pro-semibold.f11ba60a.woff` & `streamlit-reveal-slides-0.1.1/reveal_slides/frontend/build/static/media/source-sans-pro-semibold.f11ba60a.woff`

 * *Files identical despite different names*

### Comparing `streamlit-reveal-slides-0.1.0/reveal_slides/frontend/build/static/media/source-sans-pro-semibolditalic.522a9ee9.ttf` & `streamlit-reveal-slides-0.1.1/reveal_slides/frontend/build/static/media/source-sans-pro-semibolditalic.522a9ee9.ttf`

 * *Files identical despite different names*

### Comparing `streamlit-reveal-slides-0.1.0/reveal_slides/frontend/build/static/media/source-sans-pro-semibolditalic.a43f56ac.woff` & `streamlit-reveal-slides-0.1.1/reveal_slides/frontend/build/static/media/source-sans-pro-semibolditalic.a43f56ac.woff`

 * *Files identical despite different names*

### Comparing `streamlit-reveal-slides-0.1.0/reveal_slides/frontend/build/static/media/source-sans-pro-semibolditalic.fb03c660.eot` & `streamlit-reveal-slides-0.1.1/reveal_slides/frontend/build/static/media/source-sans-pro-semibolditalic.fb03c660.eot`

 * *Files identical despite different names*

### Comparing `streamlit-reveal-slides-0.1.0/setup.py` & `streamlit-reveal-slides-0.1.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import setuptools
 
 setuptools.setup(
     name="streamlit-reveal-slides",
-    version="0.1.0",
+    version="0.1.1",
     author="Anas Bouzid",
     author_email="",
     description="reveal.js HTML presentations for streamlit",
     long_description="create and add reveal.js HTML presentations to your streamlit app",
     long_description_content_type="text/plain",
     url="https://github.com/bouzidanas/streamlit.io/tree/master/streamlit-reveal-slides",
     packages=setuptools.find_packages(),
```

### Comparing `streamlit-reveal-slides-0.1.0/streamlit_reveal_slides.egg-info/SOURCES.txt` & `streamlit-reveal-slides-0.1.1/streamlit_reveal_slides.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -74,16 +74,16 @@
 reveal_slides/frontend/build/static/js/6.2008461d.chunk.js.map
 reveal_slides/frontend/build/static/js/7.69aea7e9.chunk.js
 reveal_slides/frontend/build/static/js/7.69aea7e9.chunk.js.map
 reveal_slides/frontend/build/static/js/8.86b27921.chunk.js
 reveal_slides/frontend/build/static/js/8.86b27921.chunk.js.map
 reveal_slides/frontend/build/static/js/9.fd893fed.chunk.js
 reveal_slides/frontend/build/static/js/9.fd893fed.chunk.js.map
-reveal_slides/frontend/build/static/js/main.c54401b6.chunk.js
-reveal_slides/frontend/build/static/js/main.c54401b6.chunk.js.map
+reveal_slides/frontend/build/static/js/main.6641c370.chunk.js
+reveal_slides/frontend/build/static/js/main.6641c370.chunk.js.map
 reveal_slides/frontend/build/static/js/runtime-main.cda34e22.js
 reveal_slides/frontend/build/static/js/runtime-main.cda34e22.js.map
 reveal_slides/frontend/build/static/media/league-gothic.080eee2a.woff
 reveal_slides/frontend/build/static/media/league-gothic.12baac5d.eot
 reveal_slides/frontend/build/static/media/league-gothic.6ae91382.ttf
 reveal_slides/frontend/build/static/media/source-sans-pro-italic.10a5cb40.ttf
 reveal_slides/frontend/build/static/media/source-sans-pro-italic.97e79d3e.eot
```

