# Comparing `tmp/weewx-5.0.0a30.tar.gz` & `tmp/weewx-5.0.0b1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "weewx-5.0.0a30.tar", max compression
+gzip compressed data, was "weewx-5.0.0b1.tar", max compression
```

## Comparing `weewx-5.0.0a30.tar` & `weewx-5.0.0b1.tar`

### file list

```diff
@@ -1,460 +1,456 @@
--rw-r--r--   0        0        0    32472 2020-04-14 15:37:59.000000 weewx-5.0.0a30/LICENSE.txt
--rw-r--r--   0        0        0     3301 2023-04-30 14:54:09.894705 weewx-5.0.0a30/README.md
--rw-r--r--   0        0        0      230 2022-10-29 23:29:54.801313 weewx-5.0.0a30/bin/schemas/__init__.py
--rw-r--r--   0        0        0     3448 2023-03-10 17:12:41.226442 weewx-5.0.0a30/bin/schemas/wview.py
--rw-r--r--   0        0        0     5953 2023-03-10 17:12:41.226442 weewx-5.0.0a30/bin/schemas/wview_extended.py
--rw-r--r--   0        0        0     2105 2023-03-10 17:12:41.226442 weewx-5.0.0a30/bin/schemas/wview_small.py
--rwxr-xr-x   0        0        0    52419 2023-04-30 14:54:09.894705 weewx-5.0.0a30/bin/wee_database.py
--rwxr-xr-x   0        0        0    16203 2023-04-30 14:54:09.894705 weewx-5.0.0a30/bin/wee_debug.py
--rwxr-xr-x   0        0        0     2209 2023-04-30 14:54:09.894705 weewx-5.0.0a30/bin/wee_device.py
--rwxr-xr-x   0        0        0    38964 2023-04-30 14:54:09.894705 weewx-5.0.0a30/bin/wee_import.py
--rwxr-xr-x   0        0        0     5652 2023-04-30 14:54:09.894705 weewx-5.0.0a30/bin/wee_reports.py
--rw-r--r--   0        0        0        0 2023-05-05 18:26:40.177938 weewx-5.0.0a30/bin/wee_resources/__init__.py
--rw-r--r--   0        0        0      306 2023-03-13 13:33:49.291977 weewx-5.0.0a30/bin/wee_resources/bin/user/__init__.py
--rw-r--r--   0        0        0      324 2023-05-05 15:30:16.802962 weewx-5.0.0a30/bin/wee_resources/bin/user/__pycache__/__init__.cpython-37.pyc
--rw-r--r--   0        0        0      398 2023-05-05 15:30:16.802962 weewx-5.0.0a30/bin/wee_resources/bin/user/__pycache__/extensions.cpython-37.pyc
--rw-r--r--   0        0        0      541 2023-03-13 13:33:49.291977 weewx-5.0.0a30/bin/wee_resources/bin/user/extensions.py
--rw-r--r--   0        0        0    30946 2023-05-05 18:26:39.721941 weewx-5.0.0a30/bin/wee_resources/docs/404.html
--rw-r--r--   0        0        0     1870 2023-05-05 18:26:39.621942 weewx-5.0.0a30/bin/wee_resources/docs/assets/images/favicon.png
--rw-r--r--   0        0        0   113550 2023-05-05 18:26:39.621942 weewx-5.0.0a30/bin/wee_resources/docs/assets/javascripts/bundle.4b2c34cd.min.js
--rw-r--r--   0        0        0   954048 2023-05-05 18:26:39.625942 weewx-5.0.0a30/bin/wee_resources/docs/assets/javascripts/bundle.4b2c34cd.min.js.map
--rw-r--r--   0        0        0    17074 2023-05-05 18:26:39.625942 weewx-5.0.0a30/bin/wee_resources/docs/assets/javascripts/lunr/min/lunr.ar.min.js
--rw-r--r--   0        0        0     4654 2023-05-05 18:26:39.625942 weewx-5.0.0a30/bin/wee_resources/docs/assets/javascripts/lunr/min/lunr.da.min.js
--rw-r--r--   0        0        0     6119 2023-05-05 18:26:39.625942 weewx-5.0.0a30/bin/wee_resources/docs/assets/javascripts/lunr/min/lunr.de.min.js
--rw-r--r--   0        0        0     6208 2023-05-05 18:26:39.625942 weewx-5.0.0a30/bin/wee_resources/docs/assets/javascripts/lunr/min/lunr.du.min.js
--rw-r--r--   0        0        0    11499 2023-05-05 18:26:39.625942 weewx-5.0.0a30/bin/wee_resources/docs/assets/javascripts/lunr/min/lunr.es.min.js
--rw-r--r--   0        0        0     9342 2023-05-05 18:26:39.625942 weewx-5.0.0a30/bin/wee_resources/docs/assets/javascripts/lunr/min/lunr.fi.min.js
--rw-r--r--   0        0        0    10669 2023-05-05 18:26:39.625942 weewx-5.0.0a30/bin/wee_resources/docs/assets/javascripts/lunr/min/lunr.fr.min.js
--rw-r--r--   0        0        0     3383 2023-05-05 18:26:39.625942 weewx-5.0.0a30/bin/wee_resources/docs/assets/javascripts/lunr/min/lunr.hi.min.js
--rw-r--r--   0        0        0     9437 2023-05-05 18:26:39.625942 weewx-5.0.0a30/bin/wee_resources/docs/assets/javascripts/lunr/min/lunr.hu.min.js
--rw-r--r--   0        0        0    11232 2023-05-05 18:26:39.625942 weewx-5.0.0a30/bin/wee_resources/docs/assets/javascripts/lunr/min/lunr.it.min.js
--rw-r--r--   0        0        0     2313 2023-05-05 18:26:39.625942 weewx-5.0.0a30/bin/wee_resources/docs/assets/javascripts/lunr/min/lunr.ja.min.js
--rw-r--r--   0        0        0       36 2023-05-05 18:26:39.625942 weewx-5.0.0a30/bin/wee_resources/docs/assets/javascripts/lunr/min/lunr.jp.min.js
--rw-r--r--   0        0        0     7973 2023-05-05 18:26:39.625942 weewx-5.0.0a30/bin/wee_resources/docs/assets/javascripts/lunr/min/lunr.ko.min.js
--rw-r--r--   0        0        0      817 2023-05-05 18:26:39.625942 weewx-5.0.0a30/bin/wee_resources/docs/assets/javascripts/lunr/min/lunr.multi.min.js
--rw-r--r--   0        0        0     6026 2023-05-05 18:26:39.625942 weewx-5.0.0a30/bin/wee_resources/docs/assets/javascripts/lunr/min/lunr.nl.min.js
--rw-r--r--   0        0        0     4754 2023-05-05 18:26:39.625942 weewx-5.0.0a30/bin/wee_resources/docs/assets/javascripts/lunr/min/lunr.no.min.js
--rw-r--r--   0        0        0    10171 2023-05-05 18:26:39.625942 weewx-5.0.0a30/bin/wee_resources/docs/assets/javascripts/lunr/min/lunr.pt.min.js
--rw-r--r--   0        0        0    10958 2023-05-05 18:26:39.625942 weewx-5.0.0a30/bin/wee_resources/docs/assets/javascripts/lunr/min/lunr.ro.min.js
--rw-r--r--   0        0        0    10331 2023-05-05 18:26:39.625942 weewx-5.0.0a30/bin/wee_resources/docs/assets/javascripts/lunr/min/lunr.ru.min.js
--rw-r--r--   0        0        0     3647 2023-05-05 18:26:39.625942 weewx-5.0.0a30/bin/wee_resources/docs/assets/javascripts/lunr/min/lunr.stemmer.support.min.js
--rw-r--r--   0        0        0     4523 2023-05-05 18:26:39.625942 weewx-5.0.0a30/bin/wee_resources/docs/assets/javascripts/lunr/min/lunr.sv.min.js
--rw-r--r--   0        0        0     2406 2023-05-05 18:26:39.625942 weewx-5.0.0a30/bin/wee_resources/docs/assets/javascripts/lunr/min/lunr.ta.min.js
--rw-r--r--   0        0        0     1031 2023-05-05 18:26:39.625942 weewx-5.0.0a30/bin/wee_resources/docs/assets/javascripts/lunr/min/lunr.th.min.js
--rw-r--r--   0        0        0    15009 2023-05-05 18:26:39.625942 weewx-5.0.0a30/bin/wee_resources/docs/assets/javascripts/lunr/min/lunr.tr.min.js
--rw-r--r--   0        0        0      784 2023-05-05 18:26:39.625942 weewx-5.0.0a30/bin/wee_resources/docs/assets/javascripts/lunr/min/lunr.vi.min.js
--rw-r--r--   0        0        0     2062 2023-05-05 18:26:39.625942 weewx-5.0.0a30/bin/wee_resources/docs/assets/javascripts/lunr/min/lunr.zh.min.js
--rw-r--r--   0        0        0    22878 2023-05-05 18:26:39.625942 weewx-5.0.0a30/bin/wee_resources/docs/assets/javascripts/lunr/tinyseg.js
--rw-r--r--   0        0        0   677455 2023-05-05 18:26:39.625942 weewx-5.0.0a30/bin/wee_resources/docs/assets/javascripts/lunr/wordcut.js
--rw-r--r--   0        0        0    38916 2023-05-05 18:26:39.625942 weewx-5.0.0a30/bin/wee_resources/docs/assets/javascripts/workers/search.db81ec45.min.js
--rw-r--r--   0        0        0   210371 2023-05-05 18:26:39.625942 weewx-5.0.0a30/bin/wee_resources/docs/assets/javascripts/workers/search.db81ec45.min.js.map
--rw-r--r--   0        0        0   113427 2023-05-05 18:26:39.625942 weewx-5.0.0a30/bin/wee_resources/docs/assets/stylesheets/main.0d440cfe.min.css
--rw-r--r--   0        0        0    38997 2023-05-05 18:26:39.625942 weewx-5.0.0a30/bin/wee_resources/docs/assets/stylesheets/main.0d440cfe.min.css.map
--rw-r--r--   0        0        0    12289 2023-05-05 18:26:39.625942 weewx-5.0.0a30/bin/wee_resources/docs/assets/stylesheets/palette.2505c338.min.css
--rw-r--r--   0        0        0     3635 2023-05-05 18:26:39.625942 weewx-5.0.0a30/bin/wee_resources/docs/assets/stylesheets/palette.2505c338.min.css.map
--rw-r--r--   0        0        0   192015 2023-05-05 18:26:39.765941 weewx-5.0.0a30/bin/wee_resources/docs/changes/index.html
--rw-r--r--   0        0        0    33623 2023-05-05 18:26:39.765941 weewx-5.0.0a30/bin/wee_resources/docs/copyright/index.html
--rw-r--r--   0        0        0      565 2023-05-05 18:26:39.621942 weewx-5.0.0a30/bin/wee_resources/docs/css/tocbot-4.12.0.css
--rw-r--r--   0        0        0      565 2023-05-05 18:26:39.621942 weewx-5.0.0a30/bin/wee_resources/docs/css/tocbot-4.3.1.css
--rw-r--r--   0        0        0    11924 2023-05-05 18:26:39.621942 weewx-5.0.0a30/bin/wee_resources/docs/css/weewx_ui.css
--rw-r--r--   0        0        0    60444 2023-05-05 18:26:39.829941 weewx-5.0.0a30/bin/wee_resources/docs/custom/appendix/index.html
--rw-r--r--   0        0        0   138708 2023-05-05 18:26:39.869940 weewx-5.0.0a30/bin/wee_resources/docs/custom/cheetah/index.html
--rw-r--r--   0        0        0    71015 2023-05-05 18:26:39.881940 weewx-5.0.0a30/bin/wee_resources/docs/custom/custom_reports/index.html
--rw-r--r--   0        0        0    58081 2023-05-05 18:26:39.889940 weewx-5.0.0a30/bin/wee_resources/docs/custom/database/index.html
--rw-r--r--   0        0        0    32622 2023-05-05 18:26:39.893940 weewx-5.0.0a30/bin/wee_resources/docs/custom/derived/index.html
--rw-r--r--   0        0        0    47003 2023-05-05 18:26:39.897940 weewx-5.0.0a30/bin/wee_resources/docs/custom/drivers/index.html
--rw-r--r--   0        0        0    38281 2023-05-05 18:26:39.901940 weewx-5.0.0a30/bin/wee_resources/docs/custom/extensions/index.html
--rw-r--r--   0        0        0    59542 2023-05-05 18:26:39.909940 weewx-5.0.0a30/bin/wee_resources/docs/custom/image_generator/index.html
--rw-r--r--   0        0        0    68886 2023-05-05 18:26:39.817941 weewx-5.0.0a30/bin/wee_resources/docs/custom/index.html
--rw-r--r--   0        0        0    62835 2023-05-05 18:26:39.925940 weewx-5.0.0a30/bin/wee_resources/docs/custom/localization/index.html
--rw-r--r--   0        0        0    45787 2023-05-05 18:26:39.929940 weewx-5.0.0a30/bin/wee_resources/docs/custom/multiple_bindings/index.html
--rw-r--r--   0        0        0   117586 2023-05-05 18:26:39.953940 weewx-5.0.0a30/bin/wee_resources/docs/custom/options_ref/index.html
--rw-r--r--   0        0        0    81357 2023-05-05 18:26:39.977939 weewx-5.0.0a30/bin/wee_resources/docs/custom/service_engine/index.html
--rw-r--r--   0        0        0    43656 2023-05-05 18:26:39.981939 weewx-5.0.0a30/bin/wee_resources/docs/custom/units/index.html
--rw-r--r--   0        0        0    73263 2023-05-05 18:26:39.777941 weewx-5.0.0a30/bin/wee_resources/docs/devnotes/index.html
--rw-r--r--   0        0        0     2747 2023-05-05 18:26:39.621942 weewx-5.0.0a30/bin/wee_resources/docs/examples/tag.htm
--rw-r--r--   0        0        0   182366 2023-05-05 18:26:39.621942 weewx-5.0.0a30/bin/wee_resources/docs/hardware.htm
--rw-r--r--   0        0        0    54196 2023-05-05 18:26:39.621942 weewx-5.0.0a30/bin/wee_resources/docs/images/antialias.gif
--rw-r--r--   0        0        0     3145 2023-05-05 18:26:39.621942 weewx-5.0.0a30/bin/wee_resources/docs/images/day-gap-not-shown.png
--rw-r--r--   0        0        0     3269 2023-05-05 18:26:39.621942 weewx-5.0.0a30/bin/wee_resources/docs/images/day-gap-showing.png
--rw-r--r--   0        0        0     7579 2023-05-05 18:26:39.621942 weewx-5.0.0a30/bin/wee_resources/docs/images/daycompare.png
--rw-r--r--   0        0        0     8705 2023-05-05 18:26:39.621942 weewx-5.0.0a30/bin/wee_resources/docs/images/daytemp_with_avg.png
--rw-r--r--   0        0        0     7803 2023-05-05 18:26:39.621942 weewx-5.0.0a30/bin/wee_resources/docs/images/dayvaporp.png
--rw-r--r--   0        0        0     7663 2023-05-05 18:26:39.621942 weewx-5.0.0a30/bin/wee_resources/docs/images/daywindvec.png
--rw-r--r--   0        0        0     1026 2023-05-05 18:26:39.621942 weewx-5.0.0a30/bin/wee_resources/docs/images/favicon.png
--rw-r--r--   0        0        0    38406 2023-05-05 18:26:39.621942 weewx-5.0.0a30/bin/wee_resources/docs/images/ferrites.jpg
--rw-r--r--   0        0        0     3638 2023-05-05 18:26:39.621942 weewx-5.0.0a30/bin/wee_resources/docs/images/funky_degree.png
--rw-r--r--   0        0        0    19123 2023-05-05 18:26:39.621942 weewx-5.0.0a30/bin/wee_resources/docs/images/image_parts.png
--rw-r--r--   0        0        0    86388 2023-05-05 18:26:39.621942 weewx-5.0.0a30/bin/wee_resources/docs/images/image_parts.xcf
--rw-r--r--   0        0        0     2136 2023-05-05 18:26:39.621942 weewx-5.0.0a30/bin/wee_resources/docs/images/logo-apple.png
--rw-r--r--   0        0        0     4734 2023-05-05 18:26:39.621942 weewx-5.0.0a30/bin/wee_resources/docs/images/logo-centos.png
--rw-r--r--   0        0        0    14541 2023-05-05 18:26:39.621942 weewx-5.0.0a30/bin/wee_resources/docs/images/logo-debian.png
--rw-r--r--   0        0        0    24662 2023-05-05 18:26:39.621942 weewx-5.0.0a30/bin/wee_resources/docs/images/logo-fedora.png
--rw-r--r--   0        0        0    12046 2023-05-05 18:26:39.621942 weewx-5.0.0a30/bin/wee_resources/docs/images/logo-linux.png
--rw-r--r--   0        0        0    27245 2023-05-05 18:26:39.621942 weewx-5.0.0a30/bin/wee_resources/docs/images/logo-mint.png
--rw-r--r--   0        0        0    15980 2023-05-05 18:26:39.621942 weewx-5.0.0a30/bin/wee_resources/docs/images/logo-opensuse.png
--rw-r--r--   0        0        0    14374 2023-05-05 18:26:39.621942 weewx-5.0.0a30/bin/wee_resources/docs/images/logo-pypi.svg
--rw-r--r--   0        0        0     1192 2023-05-05 18:26:39.621942 weewx-5.0.0a30/bin/wee_resources/docs/images/logo-redhat.png
--rw-r--r--   0        0        0     3926 2023-05-05 18:26:39.621942 weewx-5.0.0a30/bin/wee_resources/docs/images/logo-rpi.png
--rw-r--r--   0        0        0     7877 2023-05-05 18:26:39.621942 weewx-5.0.0a30/bin/wee_resources/docs/images/logo-suse.png
--rw-r--r--   0        0        0    13954 2023-05-05 18:26:39.621942 weewx-5.0.0a30/bin/wee_resources/docs/images/logo-ubuntu.png
--rw-r--r--   0        0        0    12208 2023-05-05 18:26:39.621942 weewx-5.0.0a30/bin/wee_resources/docs/images/logo-weewx.png
--rw-r--r--   0        0        0    35496 2023-05-05 18:26:39.621942 weewx-5.0.0a30/bin/wee_resources/docs/images/pipeline.png
--rw-r--r--   0        0        0     6709 2023-05-05 18:26:39.621942 weewx-5.0.0a30/bin/wee_resources/docs/images/sample_monthrain.png
--rw-r--r--   0        0        0    10107 2023-05-05 18:26:39.621942 weewx-5.0.0a30/bin/wee_resources/docs/images/sample_monthtempdew.png
--rw-r--r--   0        0        0    10649 2023-05-05 18:26:39.621942 weewx-5.0.0a30/bin/wee_resources/docs/images/weekgustoverlay.png
--rw-r--r--   0        0        0     8468 2023-05-05 18:26:39.621942 weewx-5.0.0a30/bin/wee_resources/docs/images/weektempdew.png
--rw-r--r--   0        0        0     6602 2023-05-05 18:26:39.621942 weewx-5.0.0a30/bin/wee_resources/docs/images/yeardiff.png
--rw-r--r--   0        0        0     7286 2023-05-05 18:26:39.621942 weewx-5.0.0a30/bin/wee_resources/docs/images/yearhilow.png
--rw-r--r--   0        0        0    35469 2023-05-05 18:26:39.737941 weewx-5.0.0a30/bin/wee_resources/docs/index.html
--rw-r--r--   0        0        0    32611 2023-05-05 18:26:39.621942 weewx-5.0.0a30/bin/wee_resources/docs/js/cash.js
--rw-r--r--   0        0        0    14828 2023-05-05 18:26:39.621942 weewx-5.0.0a30/bin/wee_resources/docs/js/cash.min.js
--rw-r--r--   0        0        0    11422 2023-05-05 18:26:39.621942 weewx-5.0.0a30/bin/wee_resources/docs/js/tocbot-4.12.0.js
--rw-r--r--   0        0        0    11422 2023-05-05 18:26:39.621942 weewx-5.0.0a30/bin/wee_resources/docs/js/tocbot-4.12.0.min.js
--rw-r--r--   0        0        0     8892 2023-05-05 18:26:39.621942 weewx-5.0.0a30/bin/wee_resources/docs/js/tocbot-4.3.1.min.js
--rw-r--r--   0        0        0     4640 2023-05-05 18:26:39.621942 weewx-5.0.0a30/bin/wee_resources/docs/js/weewx.js
--rw-r--r--   0        0        0    40090 2023-05-05 18:26:39.989939 weewx-5.0.0a30/bin/wee_resources/docs/quickstarts/debian/index.html
--rw-r--r--   0        0        0    32984 2023-05-05 18:26:39.985939 weewx-5.0.0a30/bin/wee_resources/docs/quickstarts/index.html
--rw-r--r--   0        0        0    54980 2023-05-05 18:26:39.997939 weewx-5.0.0a30/bin/wee_resources/docs/quickstarts/pip/index.html
--rw-r--r--   0        0        0    39647 2023-05-05 18:26:40.001939 weewx-5.0.0a30/bin/wee_resources/docs/quickstarts/redhat/index.html
--rw-r--r--   0        0        0    38980 2023-05-05 18:26:40.009939 weewx-5.0.0a30/bin/wee_resources/docs/quickstarts/suse/index.html
--rw-r--r--   0        0        0    44882 2023-05-05 18:26:40.013939 weewx-5.0.0a30/bin/wee_resources/docs/quickstarts/v5-upgrade/index.html
--rw-r--r--   0        0        0    45914 2023-05-05 18:26:39.781941 weewx-5.0.0a30/bin/wee_resources/docs/report_scheduling/index.html
--rw-r--r--   0        0        0   645772 2023-05-05 18:26:40.149938 weewx-5.0.0a30/bin/wee_resources/docs/search/search_index.json
--rw-r--r--   0        0        0     9306 2023-05-05 18:26:39.629942 weewx-5.0.0a30/bin/wee_resources/docs/sitemap.xml
--rw-r--r--   0        0        0      635 2023-05-05 18:26:39.629942 weewx-5.0.0a30/bin/wee_resources/docs/sitemap.xml.gz
--rw-r--r--   0        0        0    93063 2023-05-05 18:26:39.805941 weewx-5.0.0a30/bin/wee_resources/docs/sle/index.html
--rw-r--r--   0        0        0    35894 2023-05-05 18:26:39.809941 weewx-5.0.0a30/bin/wee_resources/docs/support/index.html
--rw-r--r--   0        0        0   101774 2023-05-05 18:26:39.621942 weewx-5.0.0a30/bin/wee_resources/docs/upgrading.htm
--rw-r--r--   0        0        0    34894 2023-05-05 18:26:40.021939 weewx-5.0.0a30/bin/wee_resources/docs/usersguide/backing-up-weewx/index.html
--rw-r--r--   0        0        0    32661 2023-05-05 18:26:40.017939 weewx-5.0.0a30/bin/wee_resources/docs/usersguide/index.html
--rw-r--r--   0        0        0    38318 2023-05-05 18:26:40.025939 weewx-5.0.0a30/bin/wee_resources/docs/usersguide/installing-weewx/index.html
--rw-r--r--   0        0        0    37113 2023-05-05 18:26:40.029939 weewx-5.0.0a30/bin/wee_resources/docs/usersguide/mysql-mariadb-config/index.html
--rw-r--r--   0        0        0    36130 2023-05-05 18:26:40.029939 weewx-5.0.0a30/bin/wee_resources/docs/usersguide/running-weewx/index.html
--rw-r--r--   0        0        0    36138 2023-05-05 18:26:40.033939 weewx-5.0.0a30/bin/wee_resources/docs/usersguide/system-requirements/index.html
--rw-r--r--   0        0        0    76783 2023-05-05 18:26:40.045939 weewx-5.0.0a30/bin/wee_resources/docs/usersguide/troubleshooting-guide/index.html
--rw-r--r--   0        0        0    39572 2023-05-05 18:26:40.049939 weewx-5.0.0a30/bin/wee_resources/docs/usersguide/webserver-integration/index.html
--rw-r--r--   0        0        0    36611 2023-05-05 18:26:40.061939 weewx-5.0.0a30/bin/wee_resources/docs/usersguide/weewx-config-file/data-bindings/index.html
--rw-r--r--   0        0        0    36118 2023-05-05 18:26:40.065939 weewx-5.0.0a30/bin/wee_resources/docs/usersguide/weewx-config-file/databases/index.html
--rw-r--r--   0        0        0    39542 2023-05-05 18:26:40.069939 weewx-5.0.0a30/bin/wee_resources/docs/usersguide/weewx-config-file/databasetypes/index.html
--rw-r--r--   0        0        0    40171 2023-05-05 18:26:40.073938 weewx-5.0.0a30/bin/wee_resources/docs/usersguide/weewx-config-file/engine/index.html
--rw-r--r--   0        0        0    37139 2023-05-05 18:26:40.077938 weewx-5.0.0a30/bin/wee_resources/docs/usersguide/weewx-config-file/general/index.html
--rw-r--r--   0        0        0    35456 2023-05-05 18:26:40.057939 weewx-5.0.0a30/bin/wee_resources/docs/usersguide/weewx-config-file/index.html
--rw-r--r--   0        0        0    81553 2023-05-05 18:26:40.089938 weewx-5.0.0a30/bin/wee_resources/docs/usersguide/weewx-config-file/stations-config/index.html
--rw-r--r--   0        0        0    37944 2023-05-05 18:26:40.093938 weewx-5.0.0a30/bin/wee_resources/docs/usersguide/weewx-config-file/stdarchive/index.html
--rw-r--r--   0        0        0    34481 2023-05-05 18:26:40.093938 weewx-5.0.0a30/bin/wee_resources/docs/usersguide/weewx-config-file/stdcalibrate-config/index.html
--rw-r--r--   0        0        0    35066 2023-05-05 18:26:40.097938 weewx-5.0.0a30/bin/wee_resources/docs/usersguide/weewx-config-file/stdconvert-config/index.html
--rw-r--r--   0        0        0    35274 2023-05-05 18:26:40.101938 weewx-5.0.0a30/bin/wee_resources/docs/usersguide/weewx-config-file/stdqc-config/index.html
--rw-r--r--   0        0        0    57882 2023-05-05 18:26:40.105938 weewx-5.0.0a30/bin/wee_resources/docs/usersguide/weewx-config-file/stdreport-config/index.html
--rw-r--r--   0        0        0    68501 2023-05-05 18:26:40.117938 weewx-5.0.0a30/bin/wee_resources/docs/usersguide/weewx-config-file/stdrestful-config/index.html
--rw-r--r--   0        0        0    33455 2023-05-05 18:26:40.117938 weewx-5.0.0a30/bin/wee_resources/docs/usersguide/weewx-config-file/stdtimesynch/index.html
--rw-r--r--   0        0        0    54544 2023-05-05 18:26:40.125938 weewx-5.0.0a30/bin/wee_resources/docs/usersguide/weewx-config-file/stdwxcalculate-config/index.html
--rw-r--r--   0        0        0    40424 2023-05-05 18:26:40.057939 weewx-5.0.0a30/bin/wee_resources/docs/usersguide/where/index.html
--rw-r--r--   0        0        0    34364 2023-05-05 18:26:40.129938 weewx-5.0.0a30/bin/wee_resources/docs/utilities/index.html
--rw-r--r--   0        0        0   265633 2023-05-05 18:26:39.621942 weewx-5.0.0a30/bin/wee_resources/docs/utilities/utilities.htm
--rw-r--r--   0        0        0    55581 2023-05-05 18:26:40.141938 weewx-5.0.0a30/bin/wee_resources/docs/weectl/extension/index.html
--rw-r--r--   0        0        0    34019 2023-05-05 18:26:40.133938 weewx-5.0.0a30/bin/wee_resources/docs/weectl/index.html
--rw-r--r--   0        0        0    59933 2023-05-05 18:26:40.149938 weewx-5.0.0a30/bin/wee_resources/docs/weectl/station/index.html
--rw-r--r--   0        0        0     2503 2023-04-13 14:30:10.606500 weewx-5.0.0a30/bin/wee_resources/examples/__pycache__/seven_day.cpython-37.pyc
--rw-r--r--   0        0        0     3135 2023-03-14 22:33:02.247096 weewx-5.0.0a30/bin/wee_resources/examples/__pycache__/vaporpressure.cpython-310.pyc
--rw-r--r--   0        0        0     3097 2023-03-13 19:28:02.920821 weewx-5.0.0a30/bin/wee_resources/examples/__pycache__/vaporpressure.cpython-37.pyc
--rw-r--r--   0        0        0    10729 2023-04-30 14:54:09.930705 weewx-5.0.0a30/bin/wee_resources/examples/alarm.py
--rw-r--r--   0        0        0      179 2023-04-30 14:54:09.930705 weewx-5.0.0a30/bin/wee_resources/examples/basic/changelog
--rw-r--r--   0        0        0     1563 2023-04-30 14:54:09.930705 weewx-5.0.0a30/bin/wee_resources/examples/basic/install.py
--rw-r--r--   0        0        0     1243 2023-04-30 14:54:09.930705 weewx-5.0.0a30/bin/wee_resources/examples/basic/readme.md
--rw-r--r--   0        0        0     1510 2023-03-13 13:33:49.291977 weewx-5.0.0a30/bin/wee_resources/examples/basic/skins/basic/basic.css
--rw-r--r--   0        0        0     6451 2023-03-13 13:33:49.291977 weewx-5.0.0a30/bin/wee_resources/examples/basic/skins/basic/current.inc
--rw-r--r--   0        0        0     1150 2023-03-13 13:33:49.291977 weewx-5.0.0a30/bin/wee_resources/examples/basic/skins/basic/favicon.ico
--rw-r--r--   0        0        0    11292 2023-03-13 13:33:49.291977 weewx-5.0.0a30/bin/wee_resources/examples/basic/skins/basic/hilo.inc
--rw-r--r--   0        0        0     1665 2023-04-30 14:54:09.930705 weewx-5.0.0a30/bin/wee_resources/examples/basic/skins/basic/index.html.tmpl
--rw-r--r--   0        0        0     2216 2023-03-13 13:33:49.291977 weewx-5.0.0a30/bin/wee_resources/examples/basic/skins/basic/lang/en.conf
--rw-r--r--   0        0        0     2408 2023-03-13 13:33:49.291977 weewx-5.0.0a30/bin/wee_resources/examples/basic/skins/basic/lang/fr.conf
--rw-r--r--   0        0        0     3173 2023-03-13 13:33:49.291977 weewx-5.0.0a30/bin/wee_resources/examples/basic/skins/basic/skin.conf
--rw-r--r--   0        0        0     1965 2023-04-13 14:30:10.534500 weewx-5.0.0a30/bin/wee_resources/examples/colorize/__pycache__/colorize_1.cpython-37.pyc
--rw-r--r--   0        0        0     2140 2023-04-13 14:30:10.562500 weewx-5.0.0a30/bin/wee_resources/examples/colorize/__pycache__/colorize_2.cpython-37.pyc
--rw-r--r--   0        0        0     3175 2023-04-13 14:30:10.562500 weewx-5.0.0a30/bin/wee_resources/examples/colorize/__pycache__/colorize_3.cpython-37.pyc
--rw-r--r--   0        0        0     2128 2023-04-30 14:54:09.930705 weewx-5.0.0a30/bin/wee_resources/examples/colorize/colorize_1.py
--rw-r--r--   0        0        0     2617 2023-04-30 14:54:09.930705 weewx-5.0.0a30/bin/wee_resources/examples/colorize/colorize_2.py
--rw-r--r--   0        0        0     4001 2023-04-30 14:54:09.930705 weewx-5.0.0a30/bin/wee_resources/examples/colorize/colorize_3.py
--rw-r--r--   0        0        0     4180 2023-04-30 14:54:09.930705 weewx-5.0.0a30/bin/wee_resources/examples/fileparse/bin/user/fileparse.py
--rw-r--r--   0        0        0      269 2023-04-30 14:54:09.930705 weewx-5.0.0a30/bin/wee_resources/examples/fileparse/changelog
--rw-r--r--   0        0        0      835 2023-04-30 14:54:09.930705 weewx-5.0.0a30/bin/wee_resources/examples/fileparse/install.py
--rw-r--r--   0        0        0     2086 2023-04-30 14:54:09.930705 weewx-5.0.0a30/bin/wee_resources/examples/fileparse/readme.md
--rw-r--r--   0        0        0    10792 2023-04-30 14:54:09.930705 weewx-5.0.0a30/bin/wee_resources/examples/lowBattery.py
--rw-r--r--   0        0        0     1108 2023-03-13 13:33:49.295977 weewx-5.0.0a30/bin/wee_resources/examples/mem.py
--rw-r--r--   0        0        0     5986 2023-04-30 14:54:09.930705 weewx-5.0.0a30/bin/wee_resources/examples/pmon/bin/user/pmon.py
--rw-r--r--   0        0        0      341 2023-04-30 14:54:09.930705 weewx-5.0.0a30/bin/wee_resources/examples/pmon/changelog
--rw-r--r--   0        0        0     1511 2023-04-30 14:54:09.930705 weewx-5.0.0a30/bin/wee_resources/examples/pmon/install.py
--rw-r--r--   0        0        0     2628 2023-04-30 14:54:09.930705 weewx-5.0.0a30/bin/wee_resources/examples/pmon/readme.md
--rw-r--r--   0        0        0      507 2023-04-30 14:54:09.930705 weewx-5.0.0a30/bin/wee_resources/examples/pmon/skins/pmon/index.html.tmpl
--rw-r--r--   0        0        0     1234 2023-03-13 13:33:49.295977 weewx-5.0.0a30/bin/wee_resources/examples/pmon/skins/pmon/skin.conf
--rw-r--r--   0        0        0     4334 2023-04-30 14:54:09.930705 weewx-5.0.0a30/bin/wee_resources/examples/tests/test_vaporpressure.py
--rw-r--r--   0        0        0     4285 2023-03-13 13:33:49.295977 weewx-5.0.0a30/bin/wee_resources/examples/vaporpressure.py
--rw-r--r--   0        0        0     3034 2023-05-05 15:30:08.910203 weewx-5.0.0a30/bin/wee_resources/examples/xstats/bin/user/__pycache__/xstats.cpython-37.pyc
--rw-r--r--   0        0        0     5662 2023-04-30 14:54:09.930705 weewx-5.0.0a30/bin/wee_resources/examples/xstats/bin/user/xstats.py
--rw-r--r--   0        0        0      146 2023-04-30 14:54:09.930705 weewx-5.0.0a30/bin/wee_resources/examples/xstats/changelog
--rw-r--r--   0        0        0      850 2023-04-30 14:54:09.930705 weewx-5.0.0a30/bin/wee_resources/examples/xstats/install.py
--rw-r--r--   0        0        0     2923 2023-04-30 14:54:09.930705 weewx-5.0.0a30/bin/wee_resources/examples/xstats/readme.txt
--rw-r--r--   0        0        0     2138 2023-04-30 14:54:09.930705 weewx-5.0.0a30/bin/wee_resources/examples/xstats/skins/xstats/index.html.tmpl
--rw-r--r--   0        0        0      591 2023-04-30 14:54:09.930705 weewx-5.0.0a30/bin/wee_resources/examples/xstats/skins/xstats/skin.conf
--rw-r--r--   0        0        0      677 2023-05-05 18:26:03.170228 weewx-5.0.0a30/bin/wee_resources/skins/Ftp/skin.conf
--rw-r--r--   0        0        0     1150 2023-03-13 13:33:49.295977 weewx-5.0.0a30/bin/wee_resources/skins/Mobile/favicon.ico
--rw-r--r--   0        0        0     2573 2023-03-13 13:33:49.295977 weewx-5.0.0a30/bin/wee_resources/skins/Mobile/index.html.tmpl
--rw-r--r--   0        0        0     1021 2023-03-13 13:33:49.295977 weewx-5.0.0a30/bin/wee_resources/skins/Mobile/lang/de.conf
--rw-r--r--   0        0        0     1000 2023-03-13 13:33:49.295977 weewx-5.0.0a30/bin/wee_resources/skins/Mobile/lang/en.conf
--rw-r--r--   0        0        0     1101 2023-03-13 13:33:49.295977 weewx-5.0.0a30/bin/wee_resources/skins/Mobile/lang/nl.conf
--rw-r--r--   0        0        0     2940 2023-03-13 13:33:49.295977 weewx-5.0.0a30/bin/wee_resources/skins/Mobile/lang/no.conf
--rw-r--r--   0        0        0      671 2023-03-13 13:33:49.295977 weewx-5.0.0a30/bin/wee_resources/skins/Mobile/mobile.css
--rw-r--r--   0        0        0     5172 2023-05-05 18:26:03.170228 weewx-5.0.0a30/bin/wee_resources/skins/Mobile/skin.conf
--rw-r--r--   0        0        0      761 2023-05-05 18:26:03.174228 weewx-5.0.0a30/bin/wee_resources/skins/Rsync/skin.conf
--rw-r--r--   0        0        0     2667 2023-03-13 13:33:49.295977 weewx-5.0.0a30/bin/wee_resources/skins/Seasons/NOAA/NOAA-%Y-%m.txt.tmpl
--rw-r--r--   0        0        0     5460 2023-03-13 13:33:49.295977 weewx-5.0.0a30/bin/wee_resources/skins/Seasons/NOAA/NOAA-%Y.txt.tmpl
--rw-r--r--   0        0        0     1482 2023-03-13 13:33:49.295977 weewx-5.0.0a30/bin/wee_resources/skins/Seasons/about.inc
--rw-r--r--   0        0        0      674 2023-03-13 13:33:49.295977 weewx-5.0.0a30/bin/wee_resources/skins/Seasons/analytics.inc
--rw-r--r--   0        0        0     1137 2023-03-13 13:33:49.295977 weewx-5.0.0a30/bin/wee_resources/skins/Seasons/celestial.html.tmpl
--rw-r--r--   0        0        0     6138 2023-03-13 13:33:49.295977 weewx-5.0.0a30/bin/wee_resources/skins/Seasons/celestial.inc
--rw-r--r--   0        0        0     1291 2023-03-13 13:33:49.295977 weewx-5.0.0a30/bin/wee_resources/skins/Seasons/current.inc
--rw-r--r--   0        0        0     1150 2023-03-13 13:33:49.295977 weewx-5.0.0a30/bin/wee_resources/skins/Seasons/favicon.ico
--rw-r--r--   0        0        0   172876 2023-03-13 13:33:49.295977 weewx-5.0.0a30/bin/wee_resources/skins/Seasons/font/Kanit-Bold.ttf
--rw-r--r--   0        0        0   169744 2023-03-13 13:33:49.295977 weewx-5.0.0a30/bin/wee_resources/skins/Seasons/font/Kanit-Regular.ttf
--rw-r--r--   0        0        0     4383 2023-04-30 14:54:09.934705 weewx-5.0.0a30/bin/wee_resources/skins/Seasons/font/OFL.txt
--rw-r--r--   0        0        0   224592 2023-03-13 13:33:49.299977 weewx-5.0.0a30/bin/wee_resources/skins/Seasons/font/OpenSans-Bold.ttf
--rw-r--r--   0        0        0   217360 2023-03-13 13:33:49.299977 weewx-5.0.0a30/bin/wee_resources/skins/Seasons/font/OpenSans-Regular.ttf
--rw-r--r--   0        0        0    20248 2023-03-13 13:33:49.299977 weewx-5.0.0a30/bin/wee_resources/skins/Seasons/font/OpenSans.woff
--rw-r--r--   0        0        0    10352 2023-03-13 13:33:49.299977 weewx-5.0.0a30/bin/wee_resources/skins/Seasons/font/OpenSans.woff2
--rw-r--r--   0        0        0     4348 2023-03-13 13:33:49.299977 weewx-5.0.0a30/bin/wee_resources/skins/Seasons/font/license.txt
--rw-r--r--   0        0        0     4360 2023-03-13 13:33:49.299977 weewx-5.0.0a30/bin/wee_resources/skins/Seasons/hilo.inc
--rw-r--r--   0        0        0      858 2023-03-13 13:33:49.299977 weewx-5.0.0a30/bin/wee_resources/skins/Seasons/identifier.inc
--rw-r--r--   0        0        0     2787 2023-03-13 13:33:49.299977 weewx-5.0.0a30/bin/wee_resources/skins/Seasons/index.html.tmpl
--rw-r--r--   0        0        0     9216 2023-03-13 13:33:49.299977 weewx-5.0.0a30/bin/wee_resources/skins/Seasons/lang/cn.conf
--rw-r--r--   0        0        0     9844 2023-03-13 13:33:49.299977 weewx-5.0.0a30/bin/wee_resources/skins/Seasons/lang/cz.conf
--rw-r--r--   0        0        0     9745 2023-03-13 13:33:49.299977 weewx-5.0.0a30/bin/wee_resources/skins/Seasons/lang/de.conf
--rw-r--r--   0        0        0     9459 2023-03-13 13:33:49.299977 weewx-5.0.0a30/bin/wee_resources/skins/Seasons/lang/en.conf
--rw-r--r--   0        0        0    10702 2023-03-13 13:33:49.299977 weewx-5.0.0a30/bin/wee_resources/skins/Seasons/lang/es.conf
--rw-r--r--   0        0        0    10673 2023-03-13 13:33:49.299977 weewx-5.0.0a30/bin/wee_resources/skins/Seasons/lang/fr.conf
--rw-r--r--   0        0        0    11838 2023-03-13 13:33:49.299977 weewx-5.0.0a30/bin/wee_resources/skins/Seasons/lang/gr.conf
--rw-r--r--   0        0        0     9947 2023-03-13 13:33:49.299977 weewx-5.0.0a30/bin/wee_resources/skins/Seasons/lang/it.conf
--rw-r--r--   0        0        0     9548 2023-03-13 13:33:49.299977 weewx-5.0.0a30/bin/wee_resources/skins/Seasons/lang/nl.conf
--rw-r--r--   0        0        0    10705 2023-03-13 13:33:49.299977 weewx-5.0.0a30/bin/wee_resources/skins/Seasons/lang/no.conf
--rw-r--r--   0        0        0    15356 2023-03-13 13:33:49.299977 weewx-5.0.0a30/bin/wee_resources/skins/Seasons/lang/th.conf
--rw-r--r--   0        0        0      920 2023-03-13 13:33:49.299977 weewx-5.0.0a30/bin/wee_resources/skins/Seasons/map.inc
--rw-r--r--   0        0        0      572 2023-03-13 13:33:49.299977 weewx-5.0.0a30/bin/wee_resources/skins/Seasons/radar.inc
--rw-r--r--   0        0        0     4373 2023-03-13 13:33:49.299977 weewx-5.0.0a30/bin/wee_resources/skins/Seasons/rss.xml.tmpl
--rw-r--r--   0        0        0      642 2023-03-13 13:33:49.299977 weewx-5.0.0a30/bin/wee_resources/skins/Seasons/satellite.inc
--rw-r--r--   0        0        0     5406 2023-03-13 13:33:49.299977 weewx-5.0.0a30/bin/wee_resources/skins/Seasons/seasons.css
--rw-r--r--   0        0        0     6404 2023-03-13 13:33:49.299977 weewx-5.0.0a30/bin/wee_resources/skins/Seasons/seasons.js
--rw-r--r--   0        0        0     3947 2023-03-13 13:33:49.299977 weewx-5.0.0a30/bin/wee_resources/skins/Seasons/sensors.inc
--rw-r--r--   0        0        0    27403 2023-05-05 18:26:03.174228 weewx-5.0.0a30/bin/wee_resources/skins/Seasons/skin.conf
--rw-r--r--   0        0        0     1294 2023-03-13 13:33:49.299977 weewx-5.0.0a30/bin/wee_resources/skins/Seasons/statistics.html.tmpl
--rw-r--r--   0        0        0     3971 2023-03-13 13:33:49.299977 weewx-5.0.0a30/bin/wee_resources/skins/Seasons/statistics.inc
--rw-r--r--   0        0        0     2771 2023-03-13 13:33:49.299977 weewx-5.0.0a30/bin/wee_resources/skins/Seasons/sunmoon.inc
--rw-r--r--   0        0        0      987 2023-03-13 13:33:49.299977 weewx-5.0.0a30/bin/wee_resources/skins/Seasons/tabular.html.tmpl
--rw-r--r--   0        0        0     2450 2023-03-13 13:33:49.299977 weewx-5.0.0a30/bin/wee_resources/skins/Seasons/telemetry.html.tmpl
--rw-r--r--   0        0        0     1115 2023-03-13 13:33:49.299977 weewx-5.0.0a30/bin/wee_resources/skins/Seasons/titlebar.inc
--rw-r--r--   0        0        0     1804 2023-03-13 13:33:49.299977 weewx-5.0.0a30/bin/wee_resources/skins/Smartphone/barometer.html.tmpl
--rw-r--r--   0        0        0      143 2023-03-13 13:33:49.299977 weewx-5.0.0a30/bin/wee_resources/skins/Smartphone/custom.js
--rw-r--r--   0        0        0     1150 2023-03-13 13:33:49.299977 weewx-5.0.0a30/bin/wee_resources/skins/Smartphone/favicon.ico
--rw-r--r--   0        0        0     1043 2023-03-13 13:33:49.299977 weewx-5.0.0a30/bin/wee_resources/skins/Smartphone/humidity.html.tmpl
--rw-r--r--   0        0        0     4846 2023-03-13 13:33:49.299977 weewx-5.0.0a30/bin/wee_resources/skins/Smartphone/icons/icon_ipad_x1.png
--rw-r--r--   0        0        0     7142 2023-03-13 13:33:49.299977 weewx-5.0.0a30/bin/wee_resources/skins/Smartphone/icons/icon_ipad_x2.png
--rw-r--r--   0        0        0     4421 2023-03-13 13:33:49.299977 weewx-5.0.0a30/bin/wee_resources/skins/Smartphone/icons/icon_iphone_x1.png
--rw-r--r--   0        0        0     6095 2023-03-13 13:33:49.299977 weewx-5.0.0a30/bin/wee_resources/skins/Smartphone/icons/icon_iphone_x2.png
--rw-r--r--   0        0        0     2457 2023-03-13 13:33:49.299977 weewx-5.0.0a30/bin/wee_resources/skins/Smartphone/index.html.tmpl
--rw-r--r--   0        0        0     1639 2023-03-13 13:33:49.299977 weewx-5.0.0a30/bin/wee_resources/skins/Smartphone/lang/de.conf
--rw-r--r--   0        0        0     1554 2023-03-13 13:33:49.299977 weewx-5.0.0a30/bin/wee_resources/skins/Smartphone/lang/en.conf
--rw-r--r--   0        0        0     1594 2023-03-13 13:33:49.299977 weewx-5.0.0a30/bin/wee_resources/skins/Smartphone/lang/nl.conf
--rw-r--r--   0        0        0     3530 2023-03-13 13:33:49.299977 weewx-5.0.0a30/bin/wee_resources/skins/Smartphone/lang/no.conf
--rw-r--r--   0        0        0     1502 2023-03-13 13:33:49.299977 weewx-5.0.0a30/bin/wee_resources/skins/Smartphone/rain.html.tmpl
--rw-r--r--   0        0        0     7807 2023-05-05 18:26:03.178228 weewx-5.0.0a30/bin/wee_resources/skins/Smartphone/skin.conf
--rw-r--r--   0        0        0     1588 2023-03-13 13:33:49.299977 weewx-5.0.0a30/bin/wee_resources/skins/Smartphone/temp.html.tmpl
--rw-r--r--   0        0        0     1681 2023-03-13 13:33:49.299977 weewx-5.0.0a30/bin/wee_resources/skins/Smartphone/wind.html.tmpl
--rw-r--r--   0        0        0     2591 2023-03-13 13:33:49.299977 weewx-5.0.0a30/bin/wee_resources/skins/Standard/NOAA/NOAA-%Y-%m.txt.tmpl
--rw-r--r--   0        0        0     5364 2023-03-13 13:33:49.299977 weewx-5.0.0a30/bin/wee_resources/skins/Standard/NOAA/NOAA-%Y.txt.tmpl
--rw-r--r--   0        0        0     8546 2023-03-13 13:33:49.299977 weewx-5.0.0a30/bin/wee_resources/skins/Standard/RSS/weewx_rss.xml.tmpl
--rw-r--r--   0        0        0       76 2023-03-13 13:33:49.299977 weewx-5.0.0a30/bin/wee_resources/skins/Standard/backgrounds/band.gif
--rw-r--r--   0        0        0     2593 2023-03-13 13:33:49.299977 weewx-5.0.0a30/bin/wee_resources/skins/Standard/backgrounds/butterfly.jpg
--rw-r--r--   0        0        0     1508 2023-03-13 13:33:49.299977 weewx-5.0.0a30/bin/wee_resources/skins/Standard/backgrounds/drops.gif
--rw-r--r--   0        0        0     1386 2023-03-13 13:33:49.299977 weewx-5.0.0a30/bin/wee_resources/skins/Standard/backgrounds/flower.jpg
--rw-r--r--   0        0        0     2277 2023-03-13 13:33:49.299977 weewx-5.0.0a30/bin/wee_resources/skins/Standard/backgrounds/leaf.jpg
--rw-r--r--   0        0        0     8609 2023-03-13 13:33:49.299977 weewx-5.0.0a30/bin/wee_resources/skins/Standard/backgrounds/night.gif
--rw-r--r--   0        0        0     1150 2023-03-13 13:33:49.299977 weewx-5.0.0a30/bin/wee_resources/skins/Standard/favicon.ico
--rw-r--r--   0        0        0   313856 2023-04-30 14:54:09.934705 weewx-5.0.0a30/bin/wee_resources/skins/Standard/font/DejaVuSansMono-Bold.ttf
--rw-r--r--   0        0        0    20739 2023-03-13 13:33:49.303977 weewx-5.0.0a30/bin/wee_resources/skins/Standard/index.html.tmpl
--rw-r--r--   0        0        0     9390 2023-03-13 13:33:49.303977 weewx-5.0.0a30/bin/wee_resources/skins/Standard/lang/de.conf
--rw-r--r--   0        0        0     9264 2023-03-13 13:33:49.303977 weewx-5.0.0a30/bin/wee_resources/skins/Standard/lang/en.conf
--rw-r--r--   0        0        0     9765 2023-03-13 13:33:49.303977 weewx-5.0.0a30/bin/wee_resources/skins/Standard/lang/fr.conf
--rw-r--r--   0        0        0     9356 2023-03-13 13:33:49.303977 weewx-5.0.0a30/bin/wee_resources/skins/Standard/lang/nl.conf
--rw-r--r--   0        0        0    10875 2023-03-13 13:33:49.303977 weewx-5.0.0a30/bin/wee_resources/skins/Standard/lang/no.conf
--rw-r--r--   0        0        0    15140 2023-03-13 13:33:49.303977 weewx-5.0.0a30/bin/wee_resources/skins/Standard/month.html.tmpl
--rw-r--r--   0        0        0    16430 2023-05-05 18:26:03.182227 weewx-5.0.0a30/bin/wee_resources/skins/Standard/skin.conf
--rw-r--r--   0        0        0     1456 2023-03-13 13:33:49.303977 weewx-5.0.0a30/bin/wee_resources/skins/Standard/smartphone/barometer.html.tmpl
--rw-r--r--   0        0        0      143 2023-03-13 13:33:49.303977 weewx-5.0.0a30/bin/wee_resources/skins/Standard/smartphone/custom.js
--rw-r--r--   0        0        0     1012 2023-03-13 13:33:49.303977 weewx-5.0.0a30/bin/wee_resources/skins/Standard/smartphone/humidity.html.tmpl
--rw-r--r--   0        0        0     4846 2023-03-13 13:33:49.303977 weewx-5.0.0a30/bin/wee_resources/skins/Standard/smartphone/icons/icon_ipad_x1.png
--rw-r--r--   0        0        0     7142 2023-03-13 13:33:49.303977 weewx-5.0.0a30/bin/wee_resources/skins/Standard/smartphone/icons/icon_ipad_x2.png
--rw-r--r--   0        0        0     4421 2023-03-13 13:33:49.303977 weewx-5.0.0a30/bin/wee_resources/skins/Standard/smartphone/icons/icon_iphone_x1.png
--rw-r--r--   0        0        0     6095 2023-03-13 13:33:49.303977 weewx-5.0.0a30/bin/wee_resources/skins/Standard/smartphone/icons/icon_iphone_x2.png
--rw-r--r--   0        0        0     1918 2023-03-13 13:33:49.303977 weewx-5.0.0a30/bin/wee_resources/skins/Standard/smartphone/index.html.tmpl
--rw-r--r--   0        0        0     1000 2023-03-13 13:33:49.303977 weewx-5.0.0a30/bin/wee_resources/skins/Standard/smartphone/radar.html.tmpl
--rw-r--r--   0        0        0     1394 2023-03-13 13:33:49.303977 weewx-5.0.0a30/bin/wee_resources/skins/Standard/smartphone/rain.html.tmpl
--rw-r--r--   0        0        0     1441 2023-03-13 13:33:49.303977 weewx-5.0.0a30/bin/wee_resources/skins/Standard/smartphone/temp_outside.html.tmpl
--rw-r--r--   0        0        0     1508 2023-03-13 13:33:49.303977 weewx-5.0.0a30/bin/wee_resources/skins/Standard/smartphone/wind.html.tmpl
--rw-r--r--   0        0        0    15057 2023-03-13 13:33:49.303977 weewx-5.0.0a30/bin/wee_resources/skins/Standard/week.html.tmpl
--rw-r--r--   0        0        0     3533 2023-03-13 13:33:49.303977 weewx-5.0.0a30/bin/wee_resources/skins/Standard/weewx.css
--rw-r--r--   0        0        0     9990 2023-03-13 13:33:49.303977 weewx-5.0.0a30/bin/wee_resources/skins/Standard/year.html.tmpl
--rwxr-xr-x   0        0        0     6057 2023-03-13 13:33:49.303977 weewx-5.0.0a30/bin/wee_resources/util/init.d/weewx-multi
--rwxr-xr-x   0        0        0      862 2023-03-13 13:33:49.303977 weewx-5.0.0a30/bin/wee_resources/util/init.d/weewx.bsd
--rwxr-xr-x   0        0        0     5111 2023-03-13 13:33:49.303977 weewx-5.0.0a30/bin/wee_resources/util/init.d/weewx.debian
--rw-r--r--   0        0        0      647 2023-03-13 13:33:49.303977 weewx-5.0.0a30/bin/wee_resources/util/init.d/weewx.freebsd
--rwxr-xr-x   0        0        0     8372 2023-03-13 13:33:49.303977 weewx-5.0.0a30/bin/wee_resources/util/init.d/weewx.lsb
--rwxr-xr-x   0        0        0     1659 2023-03-13 13:33:49.303977 weewx-5.0.0a30/bin/wee_resources/util/init.d/weewx.redhat
--rwxr-xr-x   0        0        0     4856 2023-03-13 13:33:49.303977 weewx-5.0.0a30/bin/wee_resources/util/init.d/weewx.suse
--rw-r--r--   0        0        0      914 2023-04-30 14:54:09.934705 weewx-5.0.0a30/bin/wee_resources/util/launchd/com.weewx.weewxd.plist
--rw-r--r--   0        0        0      536 2023-03-28 23:07:34.757396 weewx-5.0.0a30/bin/wee_resources/util/systemd/weewx.service
--rw-r--r--   0        0        0    18474 2023-05-05 18:26:03.166228 weewx-5.0.0a30/bin/wee_resources/weewx.conf
--rw-r--r--   0        0        0    25898 2023-04-30 14:54:09.894705 weewx-5.0.0a30/bin/weecfg/__init__.py
--rw-r--r--   0        0        0    26461 2023-04-30 14:54:09.894705 weewx-5.0.0a30/bin/weecfg/database.py
--rw-r--r--   0        0        0    24020 2023-04-30 14:54:09.894705 weewx-5.0.0a30/bin/weecfg/extension.py
--rw-r--r--   0        0        0    33749 2023-05-05 18:22:35.439337 weewx-5.0.0a30/bin/weecfg/station_config.py
--rw-r--r--   0        0        0    45364 2023-04-30 14:54:09.894705 weewx-5.0.0a30/bin/weecfg/update_config.py
--rwxr-xr-x   0        0        0     1455 2023-04-30 14:54:09.894705 weewx-5.0.0a30/bin/weectl.py
--rw-r--r--   0        0        0      139 2023-04-30 14:54:09.894705 weewx-5.0.0a30/bin/weectllib/__init__.py
--rw-r--r--   0        0        0     6429 2023-04-30 14:54:09.894705 weewx-5.0.0a30/bin/weectllib/parse_extension.py
--rw-r--r--   0        0        0    17231 2023-04-30 14:54:09.894705 weewx-5.0.0a30/bin/weectllib/parse_station.py
--rw-r--r--   0        0        0     4538 2023-03-10 17:12:41.230442 weewx-5.0.0a30/bin/weedb/NOTES.md
--rw-r--r--   0        0        0     6717 2023-04-30 14:54:09.894705 weewx-5.0.0a30/bin/weedb/__init__.py
--rw-r--r--   0        0        0    11213 2023-04-30 14:54:09.894705 weewx-5.0.0a30/bin/weedb/mysql.py
--rw-r--r--   0        0        0    11161 2023-04-30 14:54:09.894705 weewx-5.0.0a30/bin/weedb/sqlite.py
--rw-r--r--   0        0        0      255 2023-03-10 17:12:41.230442 weewx-5.0.0a30/bin/weeimport/__init__.py
--rw-r--r--   0        0        0    11110 2023-03-10 17:12:41.230442 weewx-5.0.0a30/bin/weeimport/csvimport.py
--rw-r--r--   0        0        0    20265 2023-03-10 17:12:41.230442 weewx-5.0.0a30/bin/weeimport/cumulusimport.py
--rw-r--r--   0        0        0    35701 2023-03-10 17:12:41.230442 weewx-5.0.0a30/bin/weeimport/wdimport.py
--rw-r--r--   0        0        0    18225 2023-04-30 14:54:09.898705 weewx-5.0.0a30/bin/weeimport/weathercatimport.py
--rw-r--r--   0        0        0    69526 2023-04-30 14:54:09.898705 weewx-5.0.0a30/bin/weeimport/weeimport.py
--rw-r--r--   0        0        0    17222 2023-04-30 14:54:09.898705 weewx-5.0.0a30/bin/weeimport/wuimport.py
--rw-r--r--   0        0        0      367 2023-03-10 17:12:41.230442 weewx-5.0.0a30/bin/weeplot/__init__.py
--rw-r--r--   0        0        0    33267 2023-04-30 14:54:09.898705 weewx-5.0.0a30/bin/weeplot/genplot.py
--rw-r--r--   0        0        0    24811 2023-04-30 14:54:09.898705 weewx-5.0.0a30/bin/weeplot/utilities.py
--rw-r--r--   0        0        0     1633 2023-03-10 17:12:41.230442 weewx-5.0.0a30/bin/weeutil/Moon.py
--rw-r--r--   0        0        0    18296 2023-03-10 17:12:41.230442 weewx-5.0.0a30/bin/weeutil/Sun.py
--rw-r--r--   0        0        0      142 2022-10-29 23:29:54.809313 weewx-5.0.0a30/bin/weeutil/__init__.py
--rw-r--r--   0        0        0     9408 2023-04-30 14:54:09.898705 weewx-5.0.0a30/bin/weeutil/config.py
--rw-r--r--   0        0        0    12986 2023-04-30 14:54:09.898705 weewx-5.0.0a30/bin/weeutil/ftpupload.py
--rw-r--r--   0        0        0     3150 2023-04-30 14:54:09.898705 weewx-5.0.0a30/bin/weeutil/log.py
--rw-r--r--   0        0        0     5896 2023-04-30 14:54:09.898705 weewx-5.0.0a30/bin/weeutil/logger.py
--rw-r--r--   0        0        0     6593 2023-03-10 17:12:41.230442 weewx-5.0.0a30/bin/weeutil/rsyncupload.py
--rw-r--r--   0        0        0     2224 2023-03-10 17:12:41.230442 weewx-5.0.0a30/bin/weeutil/timediff.py
--rw-r--r--   0        0        0    65548 2023-04-30 17:16:26.743600 weewx-5.0.0a30/bin/weeutil/weeutil.py
--rw-r--r--   0        0        0     5930 2023-05-05 18:26:03.186227 weewx-5.0.0a30/bin/weewx/__init__.py
--rw-r--r--   0        0        0    26063 2023-05-03 22:28:25.815553 weewx-5.0.0a30/bin/weewx/accum.py
--rw-r--r--   0        0        0    22812 2023-03-10 17:12:41.238442 weewx-5.0.0a30/bin/weewx/almanac.py
--rw-r--r--   0        0        0    33390 2023-04-30 14:54:09.902705 weewx-5.0.0a30/bin/weewx/cheetahgenerator.py
--rw-r--r--   0        0        0     3393 2023-03-10 17:12:41.238442 weewx-5.0.0a30/bin/weewx/crc16.py
--rw-r--r--   0        0        0     2888 2023-04-30 14:54:09.902705 weewx-5.0.0a30/bin/weewx/daemon.py
--rw-r--r--   0        0        0    11815 2023-03-10 17:12:41.238442 weewx-5.0.0a30/bin/weewx/defaults.py
--rw-r--r--   0        0        0     5147 2023-04-30 14:54:09.902705 weewx-5.0.0a30/bin/weewx/drivers/__init__.py
--rw-r--r--   0        0        0    38987 2023-03-10 17:12:41.238442 weewx-5.0.0a30/bin/weewx/drivers/acurite.py
--rw-r--r--   0        0        0    64005 2023-04-30 14:54:09.902705 weewx-5.0.0a30/bin/weewx/drivers/cc3000.py
--rw-r--r--   0        0        0    78592 2023-04-30 14:54:09.902705 weewx-5.0.0a30/bin/weewx/drivers/fousb.py
--rw-r--r--   0        0        0    14931 2023-03-10 17:12:41.238442 weewx-5.0.0a30/bin/weewx/drivers/simulator.py
--rw-r--r--   0        0        0    99881 2023-03-10 17:12:41.238442 weewx-5.0.0a30/bin/weewx/drivers/te923.py
--rw-r--r--   0        0        0    15797 2023-03-10 17:12:41.238442 weewx-5.0.0a30/bin/weewx/drivers/ultimeter.py
--rw-r--r--   0        0        0   139705 2023-05-01 23:43:59.213830 weewx-5.0.0a30/bin/weewx/drivers/vantage.py
--rw-r--r--   0        0        0    17795 2023-03-10 17:12:41.238442 weewx-5.0.0a30/bin/weewx/drivers/wmr100.py
--rw-r--r--   0        0        0    72747 2023-03-10 17:12:41.238442 weewx-5.0.0a30/bin/weewx/drivers/wmr300.py
--rw-r--r--   0        0        0    29536 2023-04-30 14:54:09.906705 weewx-5.0.0a30/bin/weewx/drivers/wmr9x8.py
--rw-r--r--   0        0        0    18843 2023-04-30 14:54:09.906705 weewx-5.0.0a30/bin/weewx/drivers/ws1.py
--rw-r--r--   0        0        0    79489 2023-04-30 14:54:09.910705 weewx-5.0.0a30/bin/weewx/drivers/ws23xx.py
--rw-r--r--   0        0        0   173578 2023-03-10 17:12:41.242442 weewx-5.0.0a30/bin/weewx/drivers/ws28xx.py
--rw-r--r--   0        0        0    37475 2023-04-30 14:54:09.910705 weewx-5.0.0a30/bin/weewx/engine.py
--rw-r--r--   0        0        0      276 2023-03-10 17:12:41.242442 weewx-5.0.0a30/bin/weewx/filegenerator.py
--rw-r--r--   0        0        0    18278 2023-04-30 14:54:09.914705 weewx-5.0.0a30/bin/weewx/imagegenerator.py
--rw-r--r--   0        0        0    73115 2023-04-30 14:54:09.914705 weewx-5.0.0a30/bin/weewx/manager.py
--rw-r--r--   0        0        0     3187 2023-03-10 17:12:41.242442 weewx-5.0.0a30/bin/weewx/qc.py
--rw-r--r--   0        0        0    37780 2023-04-30 14:54:09.914705 weewx-5.0.0a30/bin/weewx/reportengine.py
--rw-r--r--   0        0        0    79107 2023-04-30 14:54:09.914705 weewx-5.0.0a30/bin/weewx/restx.py
--rw-r--r--   0        0        0     7207 2023-03-10 17:12:41.242442 weewx-5.0.0a30/bin/weewx/station.py
--rw-r--r--   0        0        0    31690 2023-04-30 14:54:09.914705 weewx-5.0.0a30/bin/weewx/tags.py
--rw-r--r--   0        0        0    71374 2023-04-30 14:54:09.918705 weewx-5.0.0a30/bin/weewx/units.py
--rw-r--r--   0        0        0    25248 2023-03-10 17:12:41.246442 weewx-5.0.0a30/bin/weewx/uwxutils.py
--rw-r--r--   0        0        0      246 2023-03-10 17:12:41.246442 weewx-5.0.0a30/bin/weewx/wxengine.py
--rw-r--r--   0        0        0    30034 2023-03-10 17:12:41.246442 weewx-5.0.0a30/bin/weewx/wxformulas.py
--rw-r--r--   0        0        0      367 2023-03-10 17:12:41.246442 weewx-5.0.0a30/bin/weewx/wxmanager.py
--rw-r--r--   0        0        0     7270 2023-03-10 17:12:41.246442 weewx-5.0.0a30/bin/weewx/wxservices.py
--rw-r--r--   0        0        0    34292 2023-03-10 17:12:41.246442 weewx-5.0.0a30/bin/weewx/wxxtypes.py
--rw-r--r--   0        0        0    55988 2023-05-03 13:50:47.178185 weewx-5.0.0a30/bin/weewx/xtypes.py
--rwxr-xr-x   0        0        0     9681 2023-04-30 14:54:09.918705 weewx-5.0.0a30/bin/weewxd.py
--rwxr-xr-x   0        0        0    23621 2023-04-30 14:54:09.918705 weewx-5.0.0a30/bin/wunderfixer.py
--rw-r--r--   0        0        0    11861 2023-03-10 17:12:41.258442 weewx-5.0.0a30/pkg/changelog.el
--rw-r--r--   0        0        0    11756 2023-03-10 17:12:41.258442 weewx-5.0.0a30/pkg/changelog.suse
--rw-r--r--   0        0        0     2731 2023-03-10 17:12:41.258442 weewx-5.0.0a30/pkg/debian/README
--rw-r--r--   0        0        0    20599 2023-04-30 14:54:09.930705 weewx-5.0.0a30/pkg/debian/changelog
--rw-r--r--   0        0        0        3 2023-04-30 14:54:09.930705 weewx-5.0.0a30/pkg/debian/compat
--rw-r--r--   0        0        0       36 2023-03-10 17:12:41.258442 weewx-5.0.0a30/pkg/debian/conffiles
--rwxr-xr-x   0        0        0     3398 2023-04-30 14:54:09.930705 weewx-5.0.0a30/pkg/debian/config
--rw-r--r--   0        0        0      724 2023-04-30 14:54:09.930705 weewx-5.0.0a30/pkg/debian/control
--rw-r--r--   0        0        0      926 2023-05-05 18:25:31.378457 weewx-5.0.0a30/pkg/debian/copyright
--rwxr-xr-x   0        0        0     8937 2023-04-30 14:54:09.930705 weewx-5.0.0a30/pkg/debian/postinst
--rwxr-xr-x   0        0        0      906 2023-03-10 17:12:41.258442 weewx-5.0.0a30/pkg/debian/postrm
--rwxr-xr-x   0        0        0      410 2023-03-10 17:12:41.258442 weewx-5.0.0a30/pkg/debian/preinst
--rwxr-xr-x   0        0        0      693 2023-04-30 14:54:09.930705 weewx-5.0.0a30/pkg/debian/prerm
--rwxr-xr-x   0        0        0     3000 2023-04-30 14:54:09.934705 weewx-5.0.0a30/pkg/debian/rules
--rw-r--r--   0        0        0       12 2020-03-05 01:18:46.000000 weewx-5.0.0a30/pkg/debian/source/format
--rw-r--r--   0        0        0     5501 2023-04-30 14:54:09.934705 weewx-5.0.0a30/pkg/debian/templates
--rw-r--r--   0        0        0     1708 2023-04-30 14:54:09.934705 weewx-5.0.0a30/pkg/index-apt.html
--rw-r--r--   0        0        0     1728 2023-03-10 17:12:41.258442 weewx-5.0.0a30/pkg/index-suse.html
--rw-r--r--   0        0        0     1714 2023-03-10 17:12:41.258442 weewx-5.0.0a30/pkg/index-yum.html
--rwxr-xr-x   0        0        0     9874 2023-03-10 17:12:41.258442 weewx-5.0.0a30/pkg/mkchangelog.pl
--rw-r--r--   0        0        0       79 2023-03-10 17:12:41.258442 weewx-5.0.0a30/pkg/weewx-el7.repo
--rw-r--r--   0        0        0       79 2023-03-10 17:12:41.258442 weewx-5.0.0a30/pkg/weewx-el8.repo
--rw-r--r--   0        0        0       57 2023-03-10 17:12:41.258442 weewx-5.0.0a30/pkg/weewx-python2.list
--rw-r--r--   0        0        0       56 2023-03-10 17:12:41.258442 weewx-5.0.0a30/pkg/weewx-python3.list
--rw-r--r--   0        0        0       83 2023-03-10 17:12:41.258442 weewx-5.0.0a30/pkg/weewx-suse12.repo
--rw-r--r--   0        0        0       83 2023-03-10 17:12:41.258442 weewx-5.0.0a30/pkg/weewx-suse15.repo
--rw-r--r--   0        0        0     2201 2023-03-10 17:12:41.258442 weewx-5.0.0a30/pkg/weewx.smf
--rw-r--r--   0        0        0     7756 2023-03-10 17:12:41.258442 weewx-5.0.0a30/pkg/weewx.spec.in
--rw-r--r--   0        0        0     2930 2023-05-05 18:24:29.754845 weewx-5.0.0a30/pyproject.toml
--rw-r--r--   0        0        0      154 2023-03-10 17:12:41.266442 weewx-5.0.0a30/util/apache/conf-available/weewx.conf
--rw-r--r--   0        0        0      167 2023-03-10 17:12:41.266442 weewx-5.0.0a30/util/apache/conf.d/weewx.conf
--rw-r--r--   0        0        0      136 2023-04-30 14:54:09.934705 weewx-5.0.0a30/util/default/weewx
--rwxr-xr-x   0        0        0     8897 2023-03-10 17:12:41.266442 weewx-5.0.0a30/util/i18n/i18n-report
--rw-r--r--   0        0        0     9052 2023-03-10 17:12:41.266442 weewx-5.0.0a30/util/import/csv-example.conf
--rw-r--r--   0        0        0     8250 2023-03-10 17:12:41.266442 weewx-5.0.0a30/util/import/cumulus-example.conf
--rw-r--r--   0        0        0    14923 2023-03-10 17:12:41.266442 weewx-5.0.0a30/util/import/wd-example.conf
--rw-r--r--   0        0        0     7100 2023-03-10 17:12:41.266442 weewx-5.0.0a30/util/import/weathercat-example.conf
--rw-r--r--   0        0        0     6202 2023-03-10 17:12:41.266442 weewx-5.0.0a30/util/import/wu-example.conf
--rwxr-xr-x   0        0        0     6057 2023-03-13 13:33:49.303977 weewx-5.0.0a30/util/init.d/weewx-multi
--rwxr-xr-x   0        0        0      862 2023-03-13 13:33:49.303977 weewx-5.0.0a30/util/init.d/weewx.bsd
--rwxr-xr-x   0        0        0     5111 2023-03-13 13:33:49.303977 weewx-5.0.0a30/util/init.d/weewx.debian
--rw-r--r--   0        0        0      647 2023-03-13 13:33:49.303977 weewx-5.0.0a30/util/init.d/weewx.freebsd
--rwxr-xr-x   0        0        0     8372 2023-03-13 13:33:49.303977 weewx-5.0.0a30/util/init.d/weewx.lsb
--rwxr-xr-x   0        0        0     1659 2023-03-13 13:33:49.303977 weewx-5.0.0a30/util/init.d/weewx.redhat
--rwxr-xr-x   0        0        0     4856 2023-03-13 13:33:49.303977 weewx-5.0.0a30/util/init.d/weewx.suse
--rw-r--r--   0        0        0      914 2023-04-30 14:54:09.934705 weewx-5.0.0a30/util/launchd/com.weewx.weewxd.plist
--rw-r--r--   0        0        0     1800 2023-03-10 17:12:41.266442 weewx-5.0.0a30/util/logrotate.d/weewx
--rw-r--r--   0        0        0       83 2020-04-14 15:38:00.000000 weewx-5.0.0a30/util/logwatch/conf/logfiles/weewx.conf
--rw-r--r--   0        0        0       32 2020-04-14 15:38:00.000000 weewx-5.0.0a30/util/logwatch/conf/services/weewx.conf
--rwxr-xr-x   0        0        0    54942 2023-03-10 17:12:41.266442 weewx-5.0.0a30/util/logwatch/scripts/services/weewx
--rw-r--r--   0        0        0       82 2023-03-10 17:12:41.266442 weewx-5.0.0a30/util/newsyslog.d/weewx.conf
--rw-r--r--   0        0        0     2219 2023-03-10 17:12:41.266442 weewx-5.0.0a30/util/rsyslog.d/weewx.conf
--rwxr-xr-x   0        0        0      319 2023-04-30 14:54:09.938705 weewx-5.0.0a30/util/scripts/wee_database
--rwxr-xr-x   0        0        0      316 2023-04-30 14:54:09.938705 weewx-5.0.0a30/util/scripts/wee_debug
--rwxr-xr-x   0        0        0      317 2023-04-30 14:54:09.938705 weewx-5.0.0a30/util/scripts/wee_device
--rwxr-xr-x   0        0        0      317 2023-04-30 14:54:09.938705 weewx-5.0.0a30/util/scripts/wee_import
--rwxr-xr-x   0        0        0      318 2023-04-30 14:54:09.938705 weewx-5.0.0a30/util/scripts/wee_reports
--rwxr-xr-x   0        0        0      313 2023-04-30 14:54:09.938705 weewx-5.0.0a30/util/scripts/weectl
--rwxr-xr-x   0        0        0      313 2023-04-30 14:54:09.938705 weewx-5.0.0a30/util/scripts/weewxd
--rwxr-xr-x   0        0        0      318 2023-04-30 14:54:09.938705 weewx-5.0.0a30/util/scripts/wunderfixer
--rw-r--r--   0        0        0     2564 2023-03-10 17:12:41.266442 weewx-5.0.0a30/util/solaris/weewx-smf.xml
--rw-r--r--   0        0        0      536 2023-03-28 23:07:34.757396 weewx-5.0.0a30/util/systemd/weewx.service
--rw-r--r--   0        0        0       34 2023-03-10 17:12:41.266442 weewx-5.0.0a30/util/tmpfiles.d/weewx.conf
--rw-r--r--   0        0        0      149 2020-04-14 15:38:00.000000 weewx-5.0.0a30/util/udev/rules.d/acurite.rules
--rw-r--r--   0        0        0      135 2023-03-10 17:12:41.266442 weewx-5.0.0a30/util/udev/rules.d/cc3000.rules
--rw-r--r--   0        0        0      153 2020-04-14 15:38:00.000000 weewx-5.0.0a30/util/udev/rules.d/fousb.rules
--rw-r--r--   0        0        0      147 2020-04-14 15:38:00.000000 weewx-5.0.0a30/util/udev/rules.d/te923.rules
--rw-r--r--   0        0        0      624 2023-03-10 17:12:41.266442 weewx-5.0.0a30/util/udev/rules.d/vantage.rules
--rw-r--r--   0        0        0     1560 2023-03-10 17:12:41.266442 weewx-5.0.0a30/util/udev/rules.d/weewx.rules
--rw-r--r--   0        0        0      158 2020-04-14 15:38:00.000000 weewx-5.0.0a30/util/udev/rules.d/wmr100.rules
--rw-r--r--   0        0        0      158 2020-04-14 15:38:00.000000 weewx-5.0.0a30/util/udev/rules.d/wmr300.rules
--rw-r--r--   0        0        0      152 2020-04-14 15:38:00.000000 weewx-5.0.0a30/util/udev/rules.d/ws28xx.rules
--rw-r--r--   0        0        0     5072 1970-01-01 00:00:00.000000 weewx-5.0.0a30/PKG-INFO
+-rw-r--r--   0        0        0    32472 2020-04-14 15:37:59.000000 weewx-5.0.0b1/LICENSE.txt
+-rw-r--r--   0        0        0     3301 2023-04-30 14:54:09.894705 weewx-5.0.0b1/README.md
+-rw-r--r--   0        0        0      230 2022-10-29 23:29:54.801313 weewx-5.0.0b1/bin/schemas/__init__.py
+-rw-r--r--   0        0        0     3448 2023-03-10 17:12:41.226442 weewx-5.0.0b1/bin/schemas/wview.py
+-rw-r--r--   0        0        0     5953 2023-03-10 17:12:41.226442 weewx-5.0.0b1/bin/schemas/wview_extended.py
+-rw-r--r--   0        0        0     2105 2023-03-10 17:12:41.226442 weewx-5.0.0b1/bin/schemas/wview_small.py
+-rwxr-xr-x   0        0        0    52419 2023-04-30 14:54:09.894705 weewx-5.0.0b1/bin/wee_database.py
+-rwxr-xr-x   0        0        0    16203 2023-04-30 14:54:09.894705 weewx-5.0.0b1/bin/wee_debug.py
+-rwxr-xr-x   0        0        0     2209 2023-04-30 14:54:09.894705 weewx-5.0.0b1/bin/wee_device.py
+-rwxr-xr-x   0        0        0    38964 2023-04-30 14:54:09.894705 weewx-5.0.0b1/bin/wee_import.py
+-rwxr-xr-x   0        0        0     5652 2023-04-30 14:54:09.894705 weewx-5.0.0b1/bin/wee_reports.py
+-rw-r--r--   0        0        0        0 2023-05-21 11:48:35.634439 weewx-5.0.0b1/bin/wee_resources/__init__.py
+-rw-r--r--   0        0        0      306 2023-03-13 13:33:49.291977 weewx-5.0.0b1/bin/wee_resources/bin/user/__init__.py
+-rw-r--r--   0        0        0      541 2023-03-13 13:33:49.291977 weewx-5.0.0b1/bin/wee_resources/bin/user/extensions.py
+-rw-r--r--   0        0        0    30946 2023-05-21 11:48:35.166446 weewx-5.0.0b1/bin/wee_resources/docs/404.html
+-rw-r--r--   0        0        0     1870 2023-05-21 11:48:35.066447 weewx-5.0.0b1/bin/wee_resources/docs/assets/images/favicon.png
+-rw-r--r--   0        0        0   113550 2023-05-21 11:48:35.066447 weewx-5.0.0b1/bin/wee_resources/docs/assets/javascripts/bundle.4b2c34cd.min.js
+-rw-r--r--   0        0        0   954048 2023-05-21 11:48:35.070447 weewx-5.0.0b1/bin/wee_resources/docs/assets/javascripts/bundle.4b2c34cd.min.js.map
+-rw-r--r--   0        0        0    17074 2023-05-21 11:48:35.070447 weewx-5.0.0b1/bin/wee_resources/docs/assets/javascripts/lunr/min/lunr.ar.min.js
+-rw-r--r--   0        0        0     4654 2023-05-21 11:48:35.070447 weewx-5.0.0b1/bin/wee_resources/docs/assets/javascripts/lunr/min/lunr.da.min.js
+-rw-r--r--   0        0        0     6119 2023-05-21 11:48:35.070447 weewx-5.0.0b1/bin/wee_resources/docs/assets/javascripts/lunr/min/lunr.de.min.js
+-rw-r--r--   0        0        0     6208 2023-05-21 11:48:35.070447 weewx-5.0.0b1/bin/wee_resources/docs/assets/javascripts/lunr/min/lunr.du.min.js
+-rw-r--r--   0        0        0    11499 2023-05-21 11:48:35.070447 weewx-5.0.0b1/bin/wee_resources/docs/assets/javascripts/lunr/min/lunr.es.min.js
+-rw-r--r--   0        0        0     9342 2023-05-21 11:48:35.070447 weewx-5.0.0b1/bin/wee_resources/docs/assets/javascripts/lunr/min/lunr.fi.min.js
+-rw-r--r--   0        0        0    10669 2023-05-21 11:48:35.070447 weewx-5.0.0b1/bin/wee_resources/docs/assets/javascripts/lunr/min/lunr.fr.min.js
+-rw-r--r--   0        0        0     3383 2023-05-21 11:48:35.070447 weewx-5.0.0b1/bin/wee_resources/docs/assets/javascripts/lunr/min/lunr.hi.min.js
+-rw-r--r--   0        0        0     9437 2023-05-21 11:48:35.070447 weewx-5.0.0b1/bin/wee_resources/docs/assets/javascripts/lunr/min/lunr.hu.min.js
+-rw-r--r--   0        0        0    11232 2023-05-21 11:48:35.070447 weewx-5.0.0b1/bin/wee_resources/docs/assets/javascripts/lunr/min/lunr.it.min.js
+-rw-r--r--   0        0        0     2313 2023-05-21 11:48:35.070447 weewx-5.0.0b1/bin/wee_resources/docs/assets/javascripts/lunr/min/lunr.ja.min.js
+-rw-r--r--   0        0        0       36 2023-05-21 11:48:35.070447 weewx-5.0.0b1/bin/wee_resources/docs/assets/javascripts/lunr/min/lunr.jp.min.js
+-rw-r--r--   0        0        0     7973 2023-05-21 11:48:35.070447 weewx-5.0.0b1/bin/wee_resources/docs/assets/javascripts/lunr/min/lunr.ko.min.js
+-rw-r--r--   0        0        0      817 2023-05-21 11:48:35.070447 weewx-5.0.0b1/bin/wee_resources/docs/assets/javascripts/lunr/min/lunr.multi.min.js
+-rw-r--r--   0        0        0     6026 2023-05-21 11:48:35.070447 weewx-5.0.0b1/bin/wee_resources/docs/assets/javascripts/lunr/min/lunr.nl.min.js
+-rw-r--r--   0        0        0     4754 2023-05-21 11:48:35.070447 weewx-5.0.0b1/bin/wee_resources/docs/assets/javascripts/lunr/min/lunr.no.min.js
+-rw-r--r--   0        0        0    10171 2023-05-21 11:48:35.070447 weewx-5.0.0b1/bin/wee_resources/docs/assets/javascripts/lunr/min/lunr.pt.min.js
+-rw-r--r--   0        0        0    10958 2023-05-21 11:48:35.070447 weewx-5.0.0b1/bin/wee_resources/docs/assets/javascripts/lunr/min/lunr.ro.min.js
+-rw-r--r--   0        0        0    10331 2023-05-21 11:48:35.070447 weewx-5.0.0b1/bin/wee_resources/docs/assets/javascripts/lunr/min/lunr.ru.min.js
+-rw-r--r--   0        0        0     3647 2023-05-21 11:48:35.070447 weewx-5.0.0b1/bin/wee_resources/docs/assets/javascripts/lunr/min/lunr.stemmer.support.min.js
+-rw-r--r--   0        0        0     4523 2023-05-21 11:48:35.070447 weewx-5.0.0b1/bin/wee_resources/docs/assets/javascripts/lunr/min/lunr.sv.min.js
+-rw-r--r--   0        0        0     2406 2023-05-21 11:48:35.070447 weewx-5.0.0b1/bin/wee_resources/docs/assets/javascripts/lunr/min/lunr.ta.min.js
+-rw-r--r--   0        0        0     1031 2023-05-21 11:48:35.070447 weewx-5.0.0b1/bin/wee_resources/docs/assets/javascripts/lunr/min/lunr.th.min.js
+-rw-r--r--   0        0        0    15009 2023-05-21 11:48:35.070447 weewx-5.0.0b1/bin/wee_resources/docs/assets/javascripts/lunr/min/lunr.tr.min.js
+-rw-r--r--   0        0        0      784 2023-05-21 11:48:35.070447 weewx-5.0.0b1/bin/wee_resources/docs/assets/javascripts/lunr/min/lunr.vi.min.js
+-rw-r--r--   0        0        0     2062 2023-05-21 11:48:35.070447 weewx-5.0.0b1/bin/wee_resources/docs/assets/javascripts/lunr/min/lunr.zh.min.js
+-rw-r--r--   0        0        0    22878 2023-05-21 11:48:35.070447 weewx-5.0.0b1/bin/wee_resources/docs/assets/javascripts/lunr/tinyseg.js
+-rw-r--r--   0        0        0   677455 2023-05-21 11:48:35.070447 weewx-5.0.0b1/bin/wee_resources/docs/assets/javascripts/lunr/wordcut.js
+-rw-r--r--   0        0        0    38916 2023-05-21 11:48:35.070447 weewx-5.0.0b1/bin/wee_resources/docs/assets/javascripts/workers/search.db81ec45.min.js
+-rw-r--r--   0        0        0   210371 2023-05-21 11:48:35.070447 weewx-5.0.0b1/bin/wee_resources/docs/assets/javascripts/workers/search.db81ec45.min.js.map
+-rw-r--r--   0        0        0   113427 2023-05-21 11:48:35.070447 weewx-5.0.0b1/bin/wee_resources/docs/assets/stylesheets/main.0d440cfe.min.css
+-rw-r--r--   0        0        0    38997 2023-05-21 11:48:35.070447 weewx-5.0.0b1/bin/wee_resources/docs/assets/stylesheets/main.0d440cfe.min.css.map
+-rw-r--r--   0        0        0    12289 2023-05-21 11:48:35.070447 weewx-5.0.0b1/bin/wee_resources/docs/assets/stylesheets/palette.2505c338.min.css
+-rw-r--r--   0        0        0     3635 2023-05-21 11:48:35.070447 weewx-5.0.0b1/bin/wee_resources/docs/assets/stylesheets/palette.2505c338.min.css.map
+-rw-r--r--   0        0        0   192015 2023-05-21 11:48:35.210445 weewx-5.0.0b1/bin/wee_resources/docs/changes/index.html
+-rw-r--r--   0        0        0    33623 2023-05-21 11:48:35.214445 weewx-5.0.0b1/bin/wee_resources/docs/copyright/index.html
+-rw-r--r--   0        0        0      565 2023-05-21 11:48:35.066447 weewx-5.0.0b1/bin/wee_resources/docs/css/tocbot-4.12.0.css
+-rw-r--r--   0        0        0      565 2023-05-21 11:48:35.066447 weewx-5.0.0b1/bin/wee_resources/docs/css/tocbot-4.3.1.css
+-rw-r--r--   0        0        0    11924 2023-05-21 11:48:35.066447 weewx-5.0.0b1/bin/wee_resources/docs/css/weewx_ui.css
+-rw-r--r--   0        0        0    60444 2023-05-21 11:48:35.278444 weewx-5.0.0b1/bin/wee_resources/docs/custom/appendix/index.html
+-rw-r--r--   0        0        0   138708 2023-05-21 11:48:35.314444 weewx-5.0.0b1/bin/wee_resources/docs/custom/cheetah/index.html
+-rw-r--r--   0        0        0    71015 2023-05-21 11:48:35.330443 weewx-5.0.0b1/bin/wee_resources/docs/custom/custom_reports/index.html
+-rw-r--r--   0        0        0    58081 2023-05-21 11:48:35.338443 weewx-5.0.0b1/bin/wee_resources/docs/custom/database/index.html
+-rw-r--r--   0        0        0    32622 2023-05-21 11:48:35.338443 weewx-5.0.0b1/bin/wee_resources/docs/custom/derived/index.html
+-rw-r--r--   0        0        0    47003 2023-05-21 11:48:35.342443 weewx-5.0.0b1/bin/wee_resources/docs/custom/drivers/index.html
+-rw-r--r--   0        0        0    38281 2023-05-21 11:48:35.346443 weewx-5.0.0b1/bin/wee_resources/docs/custom/extensions/index.html
+-rw-r--r--   0        0        0    59542 2023-05-21 11:48:35.358443 weewx-5.0.0b1/bin/wee_resources/docs/custom/image_generator/index.html
+-rw-r--r--   0        0        0    68886 2023-05-21 11:48:35.262445 weewx-5.0.0b1/bin/wee_resources/docs/custom/index.html
+-rw-r--r--   0        0        0    62835 2023-05-21 11:48:35.370443 weewx-5.0.0b1/bin/wee_resources/docs/custom/localization/index.html
+-rw-r--r--   0        0        0    45787 2023-05-21 11:48:35.378443 weewx-5.0.0b1/bin/wee_resources/docs/custom/multiple_bindings/index.html
+-rw-r--r--   0        0        0   117586 2023-05-21 11:48:35.398443 weewx-5.0.0b1/bin/wee_resources/docs/custom/options_ref/index.html
+-rw-r--r--   0        0        0    81357 2023-05-21 11:48:35.422442 weewx-5.0.0b1/bin/wee_resources/docs/custom/service_engine/index.html
+-rw-r--r--   0        0        0    43656 2023-05-21 11:48:35.430442 weewx-5.0.0b1/bin/wee_resources/docs/custom/units/index.html
+-rw-r--r--   0        0        0    73263 2023-05-21 11:48:35.222445 weewx-5.0.0b1/bin/wee_resources/docs/devnotes/index.html
+-rw-r--r--   0        0        0     2747 2023-05-21 11:48:35.066447 weewx-5.0.0b1/bin/wee_resources/docs/examples/tag.htm
+-rw-r--r--   0        0        0   182366 2023-05-21 11:48:35.066447 weewx-5.0.0b1/bin/wee_resources/docs/hardware.htm
+-rw-r--r--   0        0        0    54196 2023-05-21 11:48:35.066447 weewx-5.0.0b1/bin/wee_resources/docs/images/antialias.gif
+-rw-r--r--   0        0        0     3145 2023-05-21 11:48:35.066447 weewx-5.0.0b1/bin/wee_resources/docs/images/day-gap-not-shown.png
+-rw-r--r--   0        0        0     3269 2023-05-21 11:48:35.066447 weewx-5.0.0b1/bin/wee_resources/docs/images/day-gap-showing.png
+-rw-r--r--   0        0        0     7579 2023-05-21 11:48:35.066447 weewx-5.0.0b1/bin/wee_resources/docs/images/daycompare.png
+-rw-r--r--   0        0        0     8705 2023-05-21 11:48:35.066447 weewx-5.0.0b1/bin/wee_resources/docs/images/daytemp_with_avg.png
+-rw-r--r--   0        0        0     7803 2023-05-21 11:48:35.066447 weewx-5.0.0b1/bin/wee_resources/docs/images/dayvaporp.png
+-rw-r--r--   0        0        0     7663 2023-05-21 11:48:35.066447 weewx-5.0.0b1/bin/wee_resources/docs/images/daywindvec.png
+-rw-r--r--   0        0        0     1026 2023-05-21 11:48:35.066447 weewx-5.0.0b1/bin/wee_resources/docs/images/favicon.png
+-rw-r--r--   0        0        0    38406 2023-05-21 11:48:35.066447 weewx-5.0.0b1/bin/wee_resources/docs/images/ferrites.jpg
+-rw-r--r--   0        0        0     3638 2023-05-21 11:48:35.066447 weewx-5.0.0b1/bin/wee_resources/docs/images/funky_degree.png
+-rw-r--r--   0        0        0    19123 2023-05-21 11:48:35.066447 weewx-5.0.0b1/bin/wee_resources/docs/images/image_parts.png
+-rw-r--r--   0        0        0    86388 2023-05-21 11:48:35.066447 weewx-5.0.0b1/bin/wee_resources/docs/images/image_parts.xcf
+-rw-r--r--   0        0        0     2136 2023-05-21 11:48:35.066447 weewx-5.0.0b1/bin/wee_resources/docs/images/logo-apple.png
+-rw-r--r--   0        0        0     4734 2023-05-21 11:48:35.066447 weewx-5.0.0b1/bin/wee_resources/docs/images/logo-centos.png
+-rw-r--r--   0        0        0    14541 2023-05-21 11:48:35.066447 weewx-5.0.0b1/bin/wee_resources/docs/images/logo-debian.png
+-rw-r--r--   0        0        0    24662 2023-05-21 11:48:35.066447 weewx-5.0.0b1/bin/wee_resources/docs/images/logo-fedora.png
+-rw-r--r--   0        0        0    12046 2023-05-21 11:48:35.066447 weewx-5.0.0b1/bin/wee_resources/docs/images/logo-linux.png
+-rw-r--r--   0        0        0    27245 2023-05-21 11:48:35.066447 weewx-5.0.0b1/bin/wee_resources/docs/images/logo-mint.png
+-rw-r--r--   0        0        0    15980 2023-05-21 11:48:35.066447 weewx-5.0.0b1/bin/wee_resources/docs/images/logo-opensuse.png
+-rw-r--r--   0        0        0    14374 2023-05-21 11:48:35.066447 weewx-5.0.0b1/bin/wee_resources/docs/images/logo-pypi.svg
+-rw-r--r--   0        0        0     1192 2023-05-21 11:48:35.066447 weewx-5.0.0b1/bin/wee_resources/docs/images/logo-redhat.png
+-rw-r--r--   0        0        0     3926 2023-05-21 11:48:35.066447 weewx-5.0.0b1/bin/wee_resources/docs/images/logo-rpi.png
+-rw-r--r--   0        0        0     7877 2023-05-21 11:48:35.066447 weewx-5.0.0b1/bin/wee_resources/docs/images/logo-suse.png
+-rw-r--r--   0        0        0    13954 2023-05-21 11:48:35.066447 weewx-5.0.0b1/bin/wee_resources/docs/images/logo-ubuntu.png
+-rw-r--r--   0        0        0    12208 2023-05-21 11:48:35.066447 weewx-5.0.0b1/bin/wee_resources/docs/images/logo-weewx.png
+-rw-r--r--   0        0        0    35496 2023-05-21 11:48:35.066447 weewx-5.0.0b1/bin/wee_resources/docs/images/pipeline.png
+-rw-r--r--   0        0        0     6709 2023-05-21 11:48:35.066447 weewx-5.0.0b1/bin/wee_resources/docs/images/sample_monthrain.png
+-rw-r--r--   0        0        0    10107 2023-05-21 11:48:35.066447 weewx-5.0.0b1/bin/wee_resources/docs/images/sample_monthtempdew.png
+-rw-r--r--   0        0        0    10649 2023-05-21 11:48:35.066447 weewx-5.0.0b1/bin/wee_resources/docs/images/weekgustoverlay.png
+-rw-r--r--   0        0        0     8468 2023-05-21 11:48:35.066447 weewx-5.0.0b1/bin/wee_resources/docs/images/weektempdew.png
+-rw-r--r--   0        0        0     6602 2023-05-21 11:48:35.066447 weewx-5.0.0b1/bin/wee_resources/docs/images/yeardiff.png
+-rw-r--r--   0        0        0     7286 2023-05-21 11:48:35.066447 weewx-5.0.0b1/bin/wee_resources/docs/images/yearhilow.png
+-rw-r--r--   0        0        0    35469 2023-05-21 11:48:35.182446 weewx-5.0.0b1/bin/wee_resources/docs/index.html
+-rw-r--r--   0        0        0    32611 2023-05-21 11:48:35.066447 weewx-5.0.0b1/bin/wee_resources/docs/js/cash.js
+-rw-r--r--   0        0        0    14828 2023-05-21 11:48:35.066447 weewx-5.0.0b1/bin/wee_resources/docs/js/cash.min.js
+-rw-r--r--   0        0        0    11422 2023-05-21 11:48:35.066447 weewx-5.0.0b1/bin/wee_resources/docs/js/tocbot-4.12.0.js
+-rw-r--r--   0        0        0    11422 2023-05-21 11:48:35.066447 weewx-5.0.0b1/bin/wee_resources/docs/js/tocbot-4.12.0.min.js
+-rw-r--r--   0        0        0     8892 2023-05-21 11:48:35.066447 weewx-5.0.0b1/bin/wee_resources/docs/js/tocbot-4.3.1.min.js
+-rw-r--r--   0        0        0     4640 2023-05-21 11:48:35.066447 weewx-5.0.0b1/bin/wee_resources/docs/js/weewx.js
+-rw-r--r--   0        0        0    40090 2023-05-21 11:48:35.434442 weewx-5.0.0b1/bin/wee_resources/docs/quickstarts/debian/index.html
+-rw-r--r--   0        0        0    32984 2023-05-21 11:48:35.430442 weewx-5.0.0b1/bin/wee_resources/docs/quickstarts/index.html
+-rw-r--r--   0        0        0    53218 2023-05-21 11:48:35.446442 weewx-5.0.0b1/bin/wee_resources/docs/quickstarts/pip/index.html
+-rw-r--r--   0        0        0    39647 2023-05-21 11:48:35.450442 weewx-5.0.0b1/bin/wee_resources/docs/quickstarts/redhat/index.html
+-rw-r--r--   0        0        0    38980 2023-05-21 11:48:35.454442 weewx-5.0.0b1/bin/wee_resources/docs/quickstarts/suse/index.html
+-rw-r--r--   0        0        0    44882 2023-05-21 11:48:35.458442 weewx-5.0.0b1/bin/wee_resources/docs/quickstarts/v5-upgrade/index.html
+-rw-r--r--   0        0        0    45914 2023-05-21 11:48:35.226445 weewx-5.0.0b1/bin/wee_resources/docs/report_scheduling/index.html
+-rw-r--r--   0        0        0   645319 2023-05-21 11:48:35.606440 weewx-5.0.0b1/bin/wee_resources/docs/search/search_index.json
+-rw-r--r--   0        0        0     9306 2023-05-21 11:48:35.074447 weewx-5.0.0b1/bin/wee_resources/docs/sitemap.xml
+-rw-r--r--   0        0        0      636 2023-05-21 11:48:35.074447 weewx-5.0.0b1/bin/wee_resources/docs/sitemap.xml.gz
+-rw-r--r--   0        0        0    93063 2023-05-21 11:48:35.250445 weewx-5.0.0b1/bin/wee_resources/docs/sle/index.html
+-rw-r--r--   0        0        0    35894 2023-05-21 11:48:35.254445 weewx-5.0.0b1/bin/wee_resources/docs/support/index.html
+-rw-r--r--   0        0        0   101774 2023-05-21 11:48:35.066447 weewx-5.0.0b1/bin/wee_resources/docs/upgrading.htm
+-rw-r--r--   0        0        0    34894 2023-05-21 11:48:35.466442 weewx-5.0.0b1/bin/wee_resources/docs/usersguide/backing-up-weewx/index.html
+-rw-r--r--   0        0        0    32661 2023-05-21 11:48:35.462442 weewx-5.0.0b1/bin/wee_resources/docs/usersguide/index.html
+-rw-r--r--   0        0        0    38318 2023-05-21 11:48:35.466442 weewx-5.0.0b1/bin/wee_resources/docs/usersguide/installing-weewx/index.html
+-rw-r--r--   0        0        0    37113 2023-05-21 11:48:35.474442 weewx-5.0.0b1/bin/wee_resources/docs/usersguide/mysql-mariadb-config/index.html
+-rw-r--r--   0        0        0    36130 2023-05-21 11:48:35.474442 weewx-5.0.0b1/bin/wee_resources/docs/usersguide/running-weewx/index.html
+-rw-r--r--   0        0        0    36138 2023-05-21 11:48:35.478442 weewx-5.0.0b1/bin/wee_resources/docs/usersguide/system-requirements/index.html
+-rw-r--r--   0        0        0    76783 2023-05-21 11:48:35.490441 weewx-5.0.0b1/bin/wee_resources/docs/usersguide/troubleshooting-guide/index.html
+-rw-r--r--   0        0        0    39572 2023-05-21 11:48:35.494441 weewx-5.0.0b1/bin/wee_resources/docs/usersguide/webserver-integration/index.html
+-rw-r--r--   0        0        0    36611 2023-05-21 11:48:35.506441 weewx-5.0.0b1/bin/wee_resources/docs/usersguide/weewx-config-file/data-bindings/index.html
+-rw-r--r--   0        0        0    36118 2023-05-21 11:48:35.510441 weewx-5.0.0b1/bin/wee_resources/docs/usersguide/weewx-config-file/databases/index.html
+-rw-r--r--   0        0        0    39542 2023-05-21 11:48:35.514441 weewx-5.0.0b1/bin/wee_resources/docs/usersguide/weewx-config-file/databasetypes/index.html
+-rw-r--r--   0        0        0    40171 2023-05-21 11:48:35.518441 weewx-5.0.0b1/bin/wee_resources/docs/usersguide/weewx-config-file/engine/index.html
+-rw-r--r--   0        0        0    37139 2023-05-21 11:48:35.522441 weewx-5.0.0b1/bin/wee_resources/docs/usersguide/weewx-config-file/general/index.html
+-rw-r--r--   0        0        0    35456 2023-05-21 11:48:35.502441 weewx-5.0.0b1/bin/wee_resources/docs/usersguide/weewx-config-file/index.html
+-rw-r--r--   0        0        0    81553 2023-05-21 11:48:35.542441 weewx-5.0.0b1/bin/wee_resources/docs/usersguide/weewx-config-file/stations-config/index.html
+-rw-r--r--   0        0        0    37944 2023-05-21 11:48:35.546441 weewx-5.0.0b1/bin/wee_resources/docs/usersguide/weewx-config-file/stdarchive/index.html
+-rw-r--r--   0        0        0    34481 2023-05-21 11:48:35.550441 weewx-5.0.0b1/bin/wee_resources/docs/usersguide/weewx-config-file/stdcalibrate-config/index.html
+-rw-r--r--   0        0        0    35066 2023-05-21 11:48:35.550441 weewx-5.0.0b1/bin/wee_resources/docs/usersguide/weewx-config-file/stdconvert-config/index.html
+-rw-r--r--   0        0        0    35274 2023-05-21 11:48:35.554441 weewx-5.0.0b1/bin/wee_resources/docs/usersguide/weewx-config-file/stdqc-config/index.html
+-rw-r--r--   0        0        0    57882 2023-05-21 11:48:35.562440 weewx-5.0.0b1/bin/wee_resources/docs/usersguide/weewx-config-file/stdreport-config/index.html
+-rw-r--r--   0        0        0    68501 2023-05-21 11:48:35.570440 weewx-5.0.0b1/bin/wee_resources/docs/usersguide/weewx-config-file/stdrestful-config/index.html
+-rw-r--r--   0        0        0    33455 2023-05-21 11:48:35.574440 weewx-5.0.0b1/bin/wee_resources/docs/usersguide/weewx-config-file/stdtimesynch/index.html
+-rw-r--r--   0        0        0    54544 2023-05-21 11:48:35.582440 weewx-5.0.0b1/bin/wee_resources/docs/usersguide/weewx-config-file/stdwxcalculate-config/index.html
+-rw-r--r--   0        0        0    40424 2023-05-21 11:48:35.502441 weewx-5.0.0b1/bin/wee_resources/docs/usersguide/where/index.html
+-rw-r--r--   0        0        0    34364 2023-05-21 11:48:35.582440 weewx-5.0.0b1/bin/wee_resources/docs/utilities/index.html
+-rw-r--r--   0        0        0   265633 2023-05-21 11:48:35.066447 weewx-5.0.0b1/bin/wee_resources/docs/utilities/utilities.htm
+-rw-r--r--   0        0        0    55581 2023-05-21 11:48:35.598440 weewx-5.0.0b1/bin/wee_resources/docs/weectl/extension/index.html
+-rw-r--r--   0        0        0    34019 2023-05-21 11:48:35.586440 weewx-5.0.0b1/bin/wee_resources/docs/weectl/index.html
+-rw-r--r--   0        0        0    59933 2023-05-21 11:48:35.602440 weewx-5.0.0b1/bin/wee_resources/docs/weectl/station/index.html
+-rw-r--r--   0        0        0     2503 2023-04-13 14:30:10.606500 weewx-5.0.0b1/bin/wee_resources/examples/__pycache__/seven_day.cpython-37.pyc
+-rw-r--r--   0        0        0     3135 2023-03-14 22:33:02.247096 weewx-5.0.0b1/bin/wee_resources/examples/__pycache__/vaporpressure.cpython-310.pyc
+-rw-r--r--   0        0        0     3097 2023-03-13 19:28:02.920821 weewx-5.0.0b1/bin/wee_resources/examples/__pycache__/vaporpressure.cpython-37.pyc
+-rw-r--r--   0        0        0    10729 2023-04-30 14:54:09.930705 weewx-5.0.0b1/bin/wee_resources/examples/alarm.py
+-rw-r--r--   0        0        0      179 2023-04-30 14:54:09.930705 weewx-5.0.0b1/bin/wee_resources/examples/basic/changelog
+-rw-r--r--   0        0        0     1563 2023-04-30 14:54:09.930705 weewx-5.0.0b1/bin/wee_resources/examples/basic/install.py
+-rw-r--r--   0        0        0     1243 2023-04-30 14:54:09.930705 weewx-5.0.0b1/bin/wee_resources/examples/basic/readme.md
+-rw-r--r--   0        0        0     1510 2023-03-13 13:33:49.291977 weewx-5.0.0b1/bin/wee_resources/examples/basic/skins/basic/basic.css
+-rw-r--r--   0        0        0     6451 2023-03-13 13:33:49.291977 weewx-5.0.0b1/bin/wee_resources/examples/basic/skins/basic/current.inc
+-rw-r--r--   0        0        0     1150 2023-03-13 13:33:49.291977 weewx-5.0.0b1/bin/wee_resources/examples/basic/skins/basic/favicon.ico
+-rw-r--r--   0        0        0    11292 2023-03-13 13:33:49.291977 weewx-5.0.0b1/bin/wee_resources/examples/basic/skins/basic/hilo.inc
+-rw-r--r--   0        0        0     1665 2023-04-30 14:54:09.930705 weewx-5.0.0b1/bin/wee_resources/examples/basic/skins/basic/index.html.tmpl
+-rw-r--r--   0        0        0     2216 2023-03-13 13:33:49.291977 weewx-5.0.0b1/bin/wee_resources/examples/basic/skins/basic/lang/en.conf
+-rw-r--r--   0        0        0     2408 2023-03-13 13:33:49.291977 weewx-5.0.0b1/bin/wee_resources/examples/basic/skins/basic/lang/fr.conf
+-rw-r--r--   0        0        0     3173 2023-03-13 13:33:49.291977 weewx-5.0.0b1/bin/wee_resources/examples/basic/skins/basic/skin.conf
+-rw-r--r--   0        0        0     1965 2023-04-13 14:30:10.534500 weewx-5.0.0b1/bin/wee_resources/examples/colorize/__pycache__/colorize_1.cpython-37.pyc
+-rw-r--r--   0        0        0     2140 2023-04-13 14:30:10.562500 weewx-5.0.0b1/bin/wee_resources/examples/colorize/__pycache__/colorize_2.cpython-37.pyc
+-rw-r--r--   0        0        0     3175 2023-04-13 14:30:10.562500 weewx-5.0.0b1/bin/wee_resources/examples/colorize/__pycache__/colorize_3.cpython-37.pyc
+-rw-r--r--   0        0        0     2128 2023-04-30 14:54:09.930705 weewx-5.0.0b1/bin/wee_resources/examples/colorize/colorize_1.py
+-rw-r--r--   0        0        0     2617 2023-04-30 14:54:09.930705 weewx-5.0.0b1/bin/wee_resources/examples/colorize/colorize_2.py
+-rw-r--r--   0        0        0     4001 2023-04-30 14:54:09.930705 weewx-5.0.0b1/bin/wee_resources/examples/colorize/colorize_3.py
+-rw-r--r--   0        0        0     4180 2023-04-30 14:54:09.930705 weewx-5.0.0b1/bin/wee_resources/examples/fileparse/bin/user/fileparse.py
+-rw-r--r--   0        0        0      269 2023-04-30 14:54:09.930705 weewx-5.0.0b1/bin/wee_resources/examples/fileparse/changelog
+-rw-r--r--   0        0        0      835 2023-04-30 14:54:09.930705 weewx-5.0.0b1/bin/wee_resources/examples/fileparse/install.py
+-rw-r--r--   0        0        0     2086 2023-04-30 14:54:09.930705 weewx-5.0.0b1/bin/wee_resources/examples/fileparse/readme.md
+-rw-r--r--   0        0        0    10792 2023-04-30 14:54:09.930705 weewx-5.0.0b1/bin/wee_resources/examples/lowBattery.py
+-rw-r--r--   0        0        0     1108 2023-03-13 13:33:49.295977 weewx-5.0.0b1/bin/wee_resources/examples/mem.py
+-rw-r--r--   0        0        0     5986 2023-04-30 14:54:09.930705 weewx-5.0.0b1/bin/wee_resources/examples/pmon/bin/user/pmon.py
+-rw-r--r--   0        0        0      341 2023-04-30 14:54:09.930705 weewx-5.0.0b1/bin/wee_resources/examples/pmon/changelog
+-rw-r--r--   0        0        0     1511 2023-04-30 14:54:09.930705 weewx-5.0.0b1/bin/wee_resources/examples/pmon/install.py
+-rw-r--r--   0        0        0     2628 2023-04-30 14:54:09.930705 weewx-5.0.0b1/bin/wee_resources/examples/pmon/readme.md
+-rw-r--r--   0        0        0      507 2023-04-30 14:54:09.930705 weewx-5.0.0b1/bin/wee_resources/examples/pmon/skins/pmon/index.html.tmpl
+-rw-r--r--   0        0        0     1234 2023-03-13 13:33:49.295977 weewx-5.0.0b1/bin/wee_resources/examples/pmon/skins/pmon/skin.conf
+-rw-r--r--   0        0        0     4334 2023-04-30 14:54:09.930705 weewx-5.0.0b1/bin/wee_resources/examples/tests/test_vaporpressure.py
+-rw-r--r--   0        0        0     4285 2023-03-13 13:33:49.295977 weewx-5.0.0b1/bin/wee_resources/examples/vaporpressure.py
+-rw-r--r--   0        0        0     5662 2023-04-30 14:54:09.930705 weewx-5.0.0b1/bin/wee_resources/examples/xstats/bin/user/xstats.py
+-rw-r--r--   0        0        0      146 2023-04-30 14:54:09.930705 weewx-5.0.0b1/bin/wee_resources/examples/xstats/changelog
+-rw-r--r--   0        0        0      850 2023-04-30 14:54:09.930705 weewx-5.0.0b1/bin/wee_resources/examples/xstats/install.py
+-rw-r--r--   0        0        0     2923 2023-04-30 14:54:09.930705 weewx-5.0.0b1/bin/wee_resources/examples/xstats/readme.txt
+-rw-r--r--   0        0        0     2138 2023-04-30 14:54:09.930705 weewx-5.0.0b1/bin/wee_resources/examples/xstats/skins/xstats/index.html.tmpl
+-rw-r--r--   0        0        0      591 2023-04-30 14:54:09.930705 weewx-5.0.0b1/bin/wee_resources/examples/xstats/skins/xstats/skin.conf
+-rw-r--r--   0        0        0      676 2023-05-06 12:11:54.181870 weewx-5.0.0b1/bin/wee_resources/skins/Ftp/skin.conf
+-rw-r--r--   0        0        0     1150 2023-03-13 13:33:49.295977 weewx-5.0.0b1/bin/wee_resources/skins/Mobile/favicon.ico
+-rw-r--r--   0        0        0     2573 2023-03-13 13:33:49.295977 weewx-5.0.0b1/bin/wee_resources/skins/Mobile/index.html.tmpl
+-rw-r--r--   0        0        0     1021 2023-03-13 13:33:49.295977 weewx-5.0.0b1/bin/wee_resources/skins/Mobile/lang/de.conf
+-rw-r--r--   0        0        0     1000 2023-03-13 13:33:49.295977 weewx-5.0.0b1/bin/wee_resources/skins/Mobile/lang/en.conf
+-rw-r--r--   0        0        0     1101 2023-03-13 13:33:49.295977 weewx-5.0.0b1/bin/wee_resources/skins/Mobile/lang/nl.conf
+-rw-r--r--   0        0        0     2940 2023-03-13 13:33:49.295977 weewx-5.0.0b1/bin/wee_resources/skins/Mobile/lang/no.conf
+-rw-r--r--   0        0        0      671 2023-03-13 13:33:49.295977 weewx-5.0.0b1/bin/wee_resources/skins/Mobile/mobile.css
+-rw-r--r--   0        0        0     5171 2023-05-06 12:11:54.181870 weewx-5.0.0b1/bin/wee_resources/skins/Mobile/skin.conf
+-rw-r--r--   0        0        0      760 2023-05-06 12:11:54.181870 weewx-5.0.0b1/bin/wee_resources/skins/Rsync/skin.conf
+-rw-r--r--   0        0        0     2667 2023-03-13 13:33:49.295977 weewx-5.0.0b1/bin/wee_resources/skins/Seasons/NOAA/NOAA-%Y-%m.txt.tmpl
+-rw-r--r--   0        0        0     5460 2023-03-13 13:33:49.295977 weewx-5.0.0b1/bin/wee_resources/skins/Seasons/NOAA/NOAA-%Y.txt.tmpl
+-rw-r--r--   0        0        0     1482 2023-03-13 13:33:49.295977 weewx-5.0.0b1/bin/wee_resources/skins/Seasons/about.inc
+-rw-r--r--   0        0        0      674 2023-03-13 13:33:49.295977 weewx-5.0.0b1/bin/wee_resources/skins/Seasons/analytics.inc
+-rw-r--r--   0        0        0     1137 2023-03-13 13:33:49.295977 weewx-5.0.0b1/bin/wee_resources/skins/Seasons/celestial.html.tmpl
+-rw-r--r--   0        0        0     6138 2023-03-13 13:33:49.295977 weewx-5.0.0b1/bin/wee_resources/skins/Seasons/celestial.inc
+-rw-r--r--   0        0        0     1291 2023-03-13 13:33:49.295977 weewx-5.0.0b1/bin/wee_resources/skins/Seasons/current.inc
+-rw-r--r--   0        0        0     1150 2023-03-13 13:33:49.295977 weewx-5.0.0b1/bin/wee_resources/skins/Seasons/favicon.ico
+-rw-r--r--   0        0        0   172876 2023-03-13 13:33:49.295977 weewx-5.0.0b1/bin/wee_resources/skins/Seasons/font/Kanit-Bold.ttf
+-rw-r--r--   0        0        0   169744 2023-03-13 13:33:49.295977 weewx-5.0.0b1/bin/wee_resources/skins/Seasons/font/Kanit-Regular.ttf
+-rw-r--r--   0        0        0     4383 2023-04-30 14:54:09.934705 weewx-5.0.0b1/bin/wee_resources/skins/Seasons/font/OFL.txt
+-rw-r--r--   0        0        0   224592 2023-03-13 13:33:49.299977 weewx-5.0.0b1/bin/wee_resources/skins/Seasons/font/OpenSans-Bold.ttf
+-rw-r--r--   0        0        0   217360 2023-03-13 13:33:49.299977 weewx-5.0.0b1/bin/wee_resources/skins/Seasons/font/OpenSans-Regular.ttf
+-rw-r--r--   0        0        0    20248 2023-03-13 13:33:49.299977 weewx-5.0.0b1/bin/wee_resources/skins/Seasons/font/OpenSans.woff
+-rw-r--r--   0        0        0    10352 2023-03-13 13:33:49.299977 weewx-5.0.0b1/bin/wee_resources/skins/Seasons/font/OpenSans.woff2
+-rw-r--r--   0        0        0     4348 2023-03-13 13:33:49.299977 weewx-5.0.0b1/bin/wee_resources/skins/Seasons/font/license.txt
+-rw-r--r--   0        0        0     4360 2023-03-13 13:33:49.299977 weewx-5.0.0b1/bin/wee_resources/skins/Seasons/hilo.inc
+-rw-r--r--   0        0        0      858 2023-03-13 13:33:49.299977 weewx-5.0.0b1/bin/wee_resources/skins/Seasons/identifier.inc
+-rw-r--r--   0        0        0     2787 2023-03-13 13:33:49.299977 weewx-5.0.0b1/bin/wee_resources/skins/Seasons/index.html.tmpl
+-rw-r--r--   0        0        0     9216 2023-03-13 13:33:49.299977 weewx-5.0.0b1/bin/wee_resources/skins/Seasons/lang/cn.conf
+-rw-r--r--   0        0        0     9844 2023-03-13 13:33:49.299977 weewx-5.0.0b1/bin/wee_resources/skins/Seasons/lang/cz.conf
+-rw-r--r--   0        0        0     9745 2023-03-13 13:33:49.299977 weewx-5.0.0b1/bin/wee_resources/skins/Seasons/lang/de.conf
+-rw-r--r--   0        0        0     9459 2023-03-13 13:33:49.299977 weewx-5.0.0b1/bin/wee_resources/skins/Seasons/lang/en.conf
+-rw-r--r--   0        0        0    10702 2023-03-13 13:33:49.299977 weewx-5.0.0b1/bin/wee_resources/skins/Seasons/lang/es.conf
+-rw-r--r--   0        0        0    10673 2023-03-13 13:33:49.299977 weewx-5.0.0b1/bin/wee_resources/skins/Seasons/lang/fr.conf
+-rw-r--r--   0        0        0    11838 2023-03-13 13:33:49.299977 weewx-5.0.0b1/bin/wee_resources/skins/Seasons/lang/gr.conf
+-rw-r--r--   0        0        0     9947 2023-03-13 13:33:49.299977 weewx-5.0.0b1/bin/wee_resources/skins/Seasons/lang/it.conf
+-rw-r--r--   0        0        0     9548 2023-03-13 13:33:49.299977 weewx-5.0.0b1/bin/wee_resources/skins/Seasons/lang/nl.conf
+-rw-r--r--   0        0        0    10705 2023-03-13 13:33:49.299977 weewx-5.0.0b1/bin/wee_resources/skins/Seasons/lang/no.conf
+-rw-r--r--   0        0        0    15356 2023-03-13 13:33:49.299977 weewx-5.0.0b1/bin/wee_resources/skins/Seasons/lang/th.conf
+-rw-r--r--   0        0        0      920 2023-03-13 13:33:49.299977 weewx-5.0.0b1/bin/wee_resources/skins/Seasons/map.inc
+-rw-r--r--   0        0        0      572 2023-03-13 13:33:49.299977 weewx-5.0.0b1/bin/wee_resources/skins/Seasons/radar.inc
+-rw-r--r--   0        0        0     4373 2023-03-13 13:33:49.299977 weewx-5.0.0b1/bin/wee_resources/skins/Seasons/rss.xml.tmpl
+-rw-r--r--   0        0        0      642 2023-03-13 13:33:49.299977 weewx-5.0.0b1/bin/wee_resources/skins/Seasons/satellite.inc
+-rw-r--r--   0        0        0     5406 2023-03-13 13:33:49.299977 weewx-5.0.0b1/bin/wee_resources/skins/Seasons/seasons.css
+-rw-r--r--   0        0        0     6404 2023-03-13 13:33:49.299977 weewx-5.0.0b1/bin/wee_resources/skins/Seasons/seasons.js
+-rw-r--r--   0        0        0     3947 2023-03-13 13:33:49.299977 weewx-5.0.0b1/bin/wee_resources/skins/Seasons/sensors.inc
+-rw-r--r--   0        0        0    27402 2023-05-06 12:11:54.181870 weewx-5.0.0b1/bin/wee_resources/skins/Seasons/skin.conf
+-rw-r--r--   0        0        0     1294 2023-03-13 13:33:49.299977 weewx-5.0.0b1/bin/wee_resources/skins/Seasons/statistics.html.tmpl
+-rw-r--r--   0        0        0     3971 2023-03-13 13:33:49.299977 weewx-5.0.0b1/bin/wee_resources/skins/Seasons/statistics.inc
+-rw-r--r--   0        0        0     2771 2023-03-13 13:33:49.299977 weewx-5.0.0b1/bin/wee_resources/skins/Seasons/sunmoon.inc
+-rw-r--r--   0        0        0      987 2023-03-13 13:33:49.299977 weewx-5.0.0b1/bin/wee_resources/skins/Seasons/tabular.html.tmpl
+-rw-r--r--   0        0        0     2450 2023-03-13 13:33:49.299977 weewx-5.0.0b1/bin/wee_resources/skins/Seasons/telemetry.html.tmpl
+-rw-r--r--   0        0        0     1115 2023-03-13 13:33:49.299977 weewx-5.0.0b1/bin/wee_resources/skins/Seasons/titlebar.inc
+-rw-r--r--   0        0        0     1804 2023-03-13 13:33:49.299977 weewx-5.0.0b1/bin/wee_resources/skins/Smartphone/barometer.html.tmpl
+-rw-r--r--   0        0        0      143 2023-03-13 13:33:49.299977 weewx-5.0.0b1/bin/wee_resources/skins/Smartphone/custom.js
+-rw-r--r--   0        0        0     1150 2023-03-13 13:33:49.299977 weewx-5.0.0b1/bin/wee_resources/skins/Smartphone/favicon.ico
+-rw-r--r--   0        0        0     1043 2023-03-13 13:33:49.299977 weewx-5.0.0b1/bin/wee_resources/skins/Smartphone/humidity.html.tmpl
+-rw-r--r--   0        0        0     4846 2023-03-13 13:33:49.299977 weewx-5.0.0b1/bin/wee_resources/skins/Smartphone/icons/icon_ipad_x1.png
+-rw-r--r--   0        0        0     7142 2023-03-13 13:33:49.299977 weewx-5.0.0b1/bin/wee_resources/skins/Smartphone/icons/icon_ipad_x2.png
+-rw-r--r--   0        0        0     4421 2023-03-13 13:33:49.299977 weewx-5.0.0b1/bin/wee_resources/skins/Smartphone/icons/icon_iphone_x1.png
+-rw-r--r--   0        0        0     6095 2023-03-13 13:33:49.299977 weewx-5.0.0b1/bin/wee_resources/skins/Smartphone/icons/icon_iphone_x2.png
+-rw-r--r--   0        0        0     2457 2023-03-13 13:33:49.299977 weewx-5.0.0b1/bin/wee_resources/skins/Smartphone/index.html.tmpl
+-rw-r--r--   0        0        0     1639 2023-03-13 13:33:49.299977 weewx-5.0.0b1/bin/wee_resources/skins/Smartphone/lang/de.conf
+-rw-r--r--   0        0        0     1554 2023-03-13 13:33:49.299977 weewx-5.0.0b1/bin/wee_resources/skins/Smartphone/lang/en.conf
+-rw-r--r--   0        0        0     1594 2023-03-13 13:33:49.299977 weewx-5.0.0b1/bin/wee_resources/skins/Smartphone/lang/nl.conf
+-rw-r--r--   0        0        0     3530 2023-03-13 13:33:49.299977 weewx-5.0.0b1/bin/wee_resources/skins/Smartphone/lang/no.conf
+-rw-r--r--   0        0        0     1502 2023-03-13 13:33:49.299977 weewx-5.0.0b1/bin/wee_resources/skins/Smartphone/rain.html.tmpl
+-rw-r--r--   0        0        0     7806 2023-05-06 12:11:54.181870 weewx-5.0.0b1/bin/wee_resources/skins/Smartphone/skin.conf
+-rw-r--r--   0        0        0     1588 2023-03-13 13:33:49.299977 weewx-5.0.0b1/bin/wee_resources/skins/Smartphone/temp.html.tmpl
+-rw-r--r--   0        0        0     1681 2023-03-13 13:33:49.299977 weewx-5.0.0b1/bin/wee_resources/skins/Smartphone/wind.html.tmpl
+-rw-r--r--   0        0        0     2591 2023-03-13 13:33:49.299977 weewx-5.0.0b1/bin/wee_resources/skins/Standard/NOAA/NOAA-%Y-%m.txt.tmpl
+-rw-r--r--   0        0        0     5364 2023-03-13 13:33:49.299977 weewx-5.0.0b1/bin/wee_resources/skins/Standard/NOAA/NOAA-%Y.txt.tmpl
+-rw-r--r--   0        0        0     8546 2023-03-13 13:33:49.299977 weewx-5.0.0b1/bin/wee_resources/skins/Standard/RSS/weewx_rss.xml.tmpl
+-rw-r--r--   0        0        0       76 2023-03-13 13:33:49.299977 weewx-5.0.0b1/bin/wee_resources/skins/Standard/backgrounds/band.gif
+-rw-r--r--   0        0        0     2593 2023-03-13 13:33:49.299977 weewx-5.0.0b1/bin/wee_resources/skins/Standard/backgrounds/butterfly.jpg
+-rw-r--r--   0        0        0     1508 2023-03-13 13:33:49.299977 weewx-5.0.0b1/bin/wee_resources/skins/Standard/backgrounds/drops.gif
+-rw-r--r--   0        0        0     1386 2023-03-13 13:33:49.299977 weewx-5.0.0b1/bin/wee_resources/skins/Standard/backgrounds/flower.jpg
+-rw-r--r--   0        0        0     2277 2023-03-13 13:33:49.299977 weewx-5.0.0b1/bin/wee_resources/skins/Standard/backgrounds/leaf.jpg
+-rw-r--r--   0        0        0     8609 2023-03-13 13:33:49.299977 weewx-5.0.0b1/bin/wee_resources/skins/Standard/backgrounds/night.gif
+-rw-r--r--   0        0        0     1150 2023-03-13 13:33:49.299977 weewx-5.0.0b1/bin/wee_resources/skins/Standard/favicon.ico
+-rw-r--r--   0        0        0   313856 2023-04-30 14:54:09.934705 weewx-5.0.0b1/bin/wee_resources/skins/Standard/font/DejaVuSansMono-Bold.ttf
+-rw-r--r--   0        0        0    20739 2023-03-13 13:33:49.303977 weewx-5.0.0b1/bin/wee_resources/skins/Standard/index.html.tmpl
+-rw-r--r--   0        0        0     9390 2023-03-13 13:33:49.303977 weewx-5.0.0b1/bin/wee_resources/skins/Standard/lang/de.conf
+-rw-r--r--   0        0        0     9264 2023-03-13 13:33:49.303977 weewx-5.0.0b1/bin/wee_resources/skins/Standard/lang/en.conf
+-rw-r--r--   0        0        0     9765 2023-03-13 13:33:49.303977 weewx-5.0.0b1/bin/wee_resources/skins/Standard/lang/fr.conf
+-rw-r--r--   0        0        0     9356 2023-03-13 13:33:49.303977 weewx-5.0.0b1/bin/wee_resources/skins/Standard/lang/nl.conf
+-rw-r--r--   0        0        0    10875 2023-03-13 13:33:49.303977 weewx-5.0.0b1/bin/wee_resources/skins/Standard/lang/no.conf
+-rw-r--r--   0        0        0    15140 2023-03-13 13:33:49.303977 weewx-5.0.0b1/bin/wee_resources/skins/Standard/month.html.tmpl
+-rw-r--r--   0        0        0    16429 2023-05-06 12:11:54.181870 weewx-5.0.0b1/bin/wee_resources/skins/Standard/skin.conf
+-rw-r--r--   0        0        0     1456 2023-03-13 13:33:49.303977 weewx-5.0.0b1/bin/wee_resources/skins/Standard/smartphone/barometer.html.tmpl
+-rw-r--r--   0        0        0      143 2023-03-13 13:33:49.303977 weewx-5.0.0b1/bin/wee_resources/skins/Standard/smartphone/custom.js
+-rw-r--r--   0        0        0     1012 2023-03-13 13:33:49.303977 weewx-5.0.0b1/bin/wee_resources/skins/Standard/smartphone/humidity.html.tmpl
+-rw-r--r--   0        0        0     4846 2023-03-13 13:33:49.303977 weewx-5.0.0b1/bin/wee_resources/skins/Standard/smartphone/icons/icon_ipad_x1.png
+-rw-r--r--   0        0        0     7142 2023-03-13 13:33:49.303977 weewx-5.0.0b1/bin/wee_resources/skins/Standard/smartphone/icons/icon_ipad_x2.png
+-rw-r--r--   0        0        0     4421 2023-03-13 13:33:49.303977 weewx-5.0.0b1/bin/wee_resources/skins/Standard/smartphone/icons/icon_iphone_x1.png
+-rw-r--r--   0        0        0     6095 2023-03-13 13:33:49.303977 weewx-5.0.0b1/bin/wee_resources/skins/Standard/smartphone/icons/icon_iphone_x2.png
+-rw-r--r--   0        0        0     1918 2023-03-13 13:33:49.303977 weewx-5.0.0b1/bin/wee_resources/skins/Standard/smartphone/index.html.tmpl
+-rw-r--r--   0        0        0     1000 2023-03-13 13:33:49.303977 weewx-5.0.0b1/bin/wee_resources/skins/Standard/smartphone/radar.html.tmpl
+-rw-r--r--   0        0        0     1394 2023-03-13 13:33:49.303977 weewx-5.0.0b1/bin/wee_resources/skins/Standard/smartphone/rain.html.tmpl
+-rw-r--r--   0        0        0     1441 2023-03-13 13:33:49.303977 weewx-5.0.0b1/bin/wee_resources/skins/Standard/smartphone/temp_outside.html.tmpl
+-rw-r--r--   0        0        0     1508 2023-03-13 13:33:49.303977 weewx-5.0.0b1/bin/wee_resources/skins/Standard/smartphone/wind.html.tmpl
+-rw-r--r--   0        0        0    15057 2023-03-13 13:33:49.303977 weewx-5.0.0b1/bin/wee_resources/skins/Standard/week.html.tmpl
+-rw-r--r--   0        0        0     3533 2023-03-13 13:33:49.303977 weewx-5.0.0b1/bin/wee_resources/skins/Standard/weewx.css
+-rw-r--r--   0        0        0     9990 2023-03-13 13:33:49.303977 weewx-5.0.0b1/bin/wee_resources/skins/Standard/year.html.tmpl
+-rwxr-xr-x   0        0        0     6057 2023-03-13 13:33:49.303977 weewx-5.0.0b1/bin/wee_resources/util/init.d/weewx-multi
+-rwxr-xr-x   0        0        0      862 2023-03-13 13:33:49.303977 weewx-5.0.0b1/bin/wee_resources/util/init.d/weewx.bsd
+-rwxr-xr-x   0        0        0     5111 2023-03-13 13:33:49.303977 weewx-5.0.0b1/bin/wee_resources/util/init.d/weewx.debian
+-rw-r--r--   0        0        0      647 2023-03-13 13:33:49.303977 weewx-5.0.0b1/bin/wee_resources/util/init.d/weewx.freebsd
+-rwxr-xr-x   0        0        0     8372 2023-03-13 13:33:49.303977 weewx-5.0.0b1/bin/wee_resources/util/init.d/weewx.lsb
+-rwxr-xr-x   0        0        0     1659 2023-03-13 13:33:49.303977 weewx-5.0.0b1/bin/wee_resources/util/init.d/weewx.redhat
+-rwxr-xr-x   0        0        0     4856 2023-03-13 13:33:49.303977 weewx-5.0.0b1/bin/wee_resources/util/init.d/weewx.suse
+-rw-r--r--   0        0        0      914 2023-04-30 14:54:09.934705 weewx-5.0.0b1/bin/wee_resources/util/launchd/com.weewx.weewxd.plist
+-rw-r--r--   0        0        0      536 2023-03-28 23:07:34.757396 weewx-5.0.0b1/bin/wee_resources/util/systemd/weewx.service
+-rw-r--r--   0        0        0    18473 2023-05-06 12:11:54.181870 weewx-5.0.0b1/bin/wee_resources/weewx.conf
+-rw-r--r--   0        0        0    25898 2023-04-30 14:54:09.894705 weewx-5.0.0b1/bin/weecfg/__init__.py
+-rw-r--r--   0        0        0    26461 2023-04-30 14:54:09.894705 weewx-5.0.0b1/bin/weecfg/database.py
+-rw-r--r--   0        0        0    24020 2023-04-30 14:54:09.894705 weewx-5.0.0b1/bin/weecfg/extension.py
+-rw-r--r--   0        0        0    33749 2023-05-05 18:22:35.439337 weewx-5.0.0b1/bin/weecfg/station_config.py
+-rw-r--r--   0        0        0    45364 2023-04-30 14:54:09.894705 weewx-5.0.0b1/bin/weecfg/update_config.py
+-rwxr-xr-x   0        0        0     1455 2023-04-30 14:54:09.894705 weewx-5.0.0b1/bin/weectl.py
+-rw-r--r--   0        0        0      139 2023-04-30 14:54:09.894705 weewx-5.0.0b1/bin/weectllib/__init__.py
+-rw-r--r--   0        0        0     6429 2023-04-30 14:54:09.894705 weewx-5.0.0b1/bin/weectllib/parse_extension.py
+-rw-r--r--   0        0        0    17231 2023-04-30 14:54:09.894705 weewx-5.0.0b1/bin/weectllib/parse_station.py
+-rw-r--r--   0        0        0     4538 2023-03-10 17:12:41.230442 weewx-5.0.0b1/bin/weedb/NOTES.md
+-rw-r--r--   0        0        0     6717 2023-04-30 14:54:09.894705 weewx-5.0.0b1/bin/weedb/__init__.py
+-rw-r--r--   0        0        0    11213 2023-04-30 14:54:09.894705 weewx-5.0.0b1/bin/weedb/mysql.py
+-rw-r--r--   0        0        0    11161 2023-04-30 14:54:09.894705 weewx-5.0.0b1/bin/weedb/sqlite.py
+-rw-r--r--   0        0        0      255 2023-03-10 17:12:41.230442 weewx-5.0.0b1/bin/weeimport/__init__.py
+-rw-r--r--   0        0        0    11110 2023-03-10 17:12:41.230442 weewx-5.0.0b1/bin/weeimport/csvimport.py
+-rw-r--r--   0        0        0    20265 2023-03-10 17:12:41.230442 weewx-5.0.0b1/bin/weeimport/cumulusimport.py
+-rw-r--r--   0        0        0    35701 2023-03-10 17:12:41.230442 weewx-5.0.0b1/bin/weeimport/wdimport.py
+-rw-r--r--   0        0        0    18225 2023-04-30 14:54:09.898705 weewx-5.0.0b1/bin/weeimport/weathercatimport.py
+-rw-r--r--   0        0        0    69526 2023-04-30 14:54:09.898705 weewx-5.0.0b1/bin/weeimport/weeimport.py
+-rw-r--r--   0        0        0    17222 2023-04-30 14:54:09.898705 weewx-5.0.0b1/bin/weeimport/wuimport.py
+-rw-r--r--   0        0        0      367 2023-03-10 17:12:41.230442 weewx-5.0.0b1/bin/weeplot/__init__.py
+-rw-r--r--   0        0        0    33267 2023-04-30 14:54:09.898705 weewx-5.0.0b1/bin/weeplot/genplot.py
+-rw-r--r--   0        0        0    24811 2023-04-30 14:54:09.898705 weewx-5.0.0b1/bin/weeplot/utilities.py
+-rw-r--r--   0        0        0     1633 2023-03-10 17:12:41.230442 weewx-5.0.0b1/bin/weeutil/Moon.py
+-rw-r--r--   0        0        0    18296 2023-03-10 17:12:41.230442 weewx-5.0.0b1/bin/weeutil/Sun.py
+-rw-r--r--   0        0        0      142 2022-10-29 23:29:54.809313 weewx-5.0.0b1/bin/weeutil/__init__.py
+-rw-r--r--   0        0        0     9408 2023-04-30 14:54:09.898705 weewx-5.0.0b1/bin/weeutil/config.py
+-rw-r--r--   0        0        0    12986 2023-04-30 14:54:09.898705 weewx-5.0.0b1/bin/weeutil/ftpupload.py
+-rw-r--r--   0        0        0     3150 2023-04-30 14:54:09.898705 weewx-5.0.0b1/bin/weeutil/log.py
+-rw-r--r--   0        0        0     5896 2023-04-30 14:54:09.898705 weewx-5.0.0b1/bin/weeutil/logger.py
+-rw-r--r--   0        0        0     6593 2023-03-10 17:12:41.230442 weewx-5.0.0b1/bin/weeutil/rsyncupload.py
+-rw-r--r--   0        0        0     2224 2023-03-10 17:12:41.230442 weewx-5.0.0b1/bin/weeutil/timediff.py
+-rw-r--r--   0        0        0    65548 2023-04-30 17:16:26.743600 weewx-5.0.0b1/bin/weeutil/weeutil.py
+-rw-r--r--   0        0        0     5929 2023-05-06 12:11:54.181870 weewx-5.0.0b1/bin/weewx/__init__.py
+-rw-r--r--   0        0        0    26063 2023-05-03 22:28:25.815553 weewx-5.0.0b1/bin/weewx/accum.py
+-rw-r--r--   0        0        0    22812 2023-03-10 17:12:41.238442 weewx-5.0.0b1/bin/weewx/almanac.py
+-rw-r--r--   0        0        0    33390 2023-04-30 14:54:09.902705 weewx-5.0.0b1/bin/weewx/cheetahgenerator.py
+-rw-r--r--   0        0        0     3393 2023-03-10 17:12:41.238442 weewx-5.0.0b1/bin/weewx/crc16.py
+-rw-r--r--   0        0        0     2888 2023-04-30 14:54:09.902705 weewx-5.0.0b1/bin/weewx/daemon.py
+-rw-r--r--   0        0        0    11815 2023-03-10 17:12:41.238442 weewx-5.0.0b1/bin/weewx/defaults.py
+-rw-r--r--   0        0        0     5147 2023-04-30 14:54:09.902705 weewx-5.0.0b1/bin/weewx/drivers/__init__.py
+-rw-r--r--   0        0        0    38987 2023-03-10 17:12:41.238442 weewx-5.0.0b1/bin/weewx/drivers/acurite.py
+-rw-r--r--   0        0        0    64005 2023-04-30 14:54:09.902705 weewx-5.0.0b1/bin/weewx/drivers/cc3000.py
+-rw-r--r--   0        0        0    78592 2023-04-30 14:54:09.902705 weewx-5.0.0b1/bin/weewx/drivers/fousb.py
+-rw-r--r--   0        0        0    14931 2023-03-10 17:12:41.238442 weewx-5.0.0b1/bin/weewx/drivers/simulator.py
+-rw-r--r--   0        0        0    99881 2023-03-10 17:12:41.238442 weewx-5.0.0b1/bin/weewx/drivers/te923.py
+-rw-r--r--   0        0        0    15797 2023-03-10 17:12:41.238442 weewx-5.0.0b1/bin/weewx/drivers/ultimeter.py
+-rw-r--r--   0        0        0   139705 2023-05-01 23:43:59.213830 weewx-5.0.0b1/bin/weewx/drivers/vantage.py
+-rw-r--r--   0        0        0    17795 2023-03-10 17:12:41.238442 weewx-5.0.0b1/bin/weewx/drivers/wmr100.py
+-rw-r--r--   0        0        0    72747 2023-03-10 17:12:41.238442 weewx-5.0.0b1/bin/weewx/drivers/wmr300.py
+-rw-r--r--   0        0        0    29536 2023-04-30 14:54:09.906705 weewx-5.0.0b1/bin/weewx/drivers/wmr9x8.py
+-rw-r--r--   0        0        0    18843 2023-04-30 14:54:09.906705 weewx-5.0.0b1/bin/weewx/drivers/ws1.py
+-rw-r--r--   0        0        0    79489 2023-04-30 14:54:09.910705 weewx-5.0.0b1/bin/weewx/drivers/ws23xx.py
+-rw-r--r--   0        0        0   173578 2023-03-10 17:12:41.242442 weewx-5.0.0b1/bin/weewx/drivers/ws28xx.py
+-rw-r--r--   0        0        0    37475 2023-04-30 14:54:09.910705 weewx-5.0.0b1/bin/weewx/engine.py
+-rw-r--r--   0        0        0      276 2023-03-10 17:12:41.242442 weewx-5.0.0b1/bin/weewx/filegenerator.py
+-rw-r--r--   0        0        0    18278 2023-04-30 14:54:09.914705 weewx-5.0.0b1/bin/weewx/imagegenerator.py
+-rw-r--r--   0        0        0    73115 2023-04-30 14:54:09.914705 weewx-5.0.0b1/bin/weewx/manager.py
+-rw-r--r--   0        0        0     3187 2023-03-10 17:12:41.242442 weewx-5.0.0b1/bin/weewx/qc.py
+-rw-r--r--   0        0        0    37780 2023-04-30 14:54:09.914705 weewx-5.0.0b1/bin/weewx/reportengine.py
+-rw-r--r--   0        0        0    79107 2023-04-30 14:54:09.914705 weewx-5.0.0b1/bin/weewx/restx.py
+-rw-r--r--   0        0        0     7207 2023-03-10 17:12:41.242442 weewx-5.0.0b1/bin/weewx/station.py
+-rw-r--r--   0        0        0    31690 2023-04-30 14:54:09.914705 weewx-5.0.0b1/bin/weewx/tags.py
+-rw-r--r--   0        0        0    71374 2023-04-30 14:54:09.918705 weewx-5.0.0b1/bin/weewx/units.py
+-rw-r--r--   0        0        0    25248 2023-03-10 17:12:41.246442 weewx-5.0.0b1/bin/weewx/uwxutils.py
+-rw-r--r--   0        0        0      246 2023-03-10 17:12:41.246442 weewx-5.0.0b1/bin/weewx/wxengine.py
+-rw-r--r--   0        0        0    30034 2023-03-10 17:12:41.246442 weewx-5.0.0b1/bin/weewx/wxformulas.py
+-rw-r--r--   0        0        0      367 2023-03-10 17:12:41.246442 weewx-5.0.0b1/bin/weewx/wxmanager.py
+-rw-r--r--   0        0        0     7270 2023-03-10 17:12:41.246442 weewx-5.0.0b1/bin/weewx/wxservices.py
+-rw-r--r--   0        0        0    34292 2023-03-10 17:12:41.246442 weewx-5.0.0b1/bin/weewx/wxxtypes.py
+-rw-r--r--   0        0        0    55988 2023-05-03 13:50:47.178185 weewx-5.0.0b1/bin/weewx/xtypes.py
+-rwxr-xr-x   0        0        0     9681 2023-04-30 14:54:09.918705 weewx-5.0.0b1/bin/weewxd.py
+-rwxr-xr-x   0        0        0    23621 2023-04-30 14:54:09.918705 weewx-5.0.0b1/bin/wunderfixer.py
+-rw-r--r--   0        0        0    12175 2023-05-06 12:11:54.181870 weewx-5.0.0b1/pkg/changelog.el
+-rw-r--r--   0        0        0    12070 2023-05-06 12:11:54.181870 weewx-5.0.0b1/pkg/changelog.suse
+-rw-r--r--   0        0        0     2731 2023-03-10 17:12:41.258442 weewx-5.0.0b1/pkg/debian/README
+-rw-r--r--   0        0        0    21100 2023-05-06 12:11:54.181870 weewx-5.0.0b1/pkg/debian/changelog
+-rw-r--r--   0        0        0        3 2023-04-30 14:54:09.930705 weewx-5.0.0b1/pkg/debian/compat
+-rw-r--r--   0        0        0       36 2023-03-10 17:12:41.258442 weewx-5.0.0b1/pkg/debian/conffiles
+-rwxr-xr-x   0        0        0     3398 2023-04-30 14:54:09.930705 weewx-5.0.0b1/pkg/debian/config
+-rw-r--r--   0        0        0      724 2023-04-30 14:54:09.930705 weewx-5.0.0b1/pkg/debian/control
+-rw-r--r--   0        0        0      926 2023-05-05 18:25:31.378457 weewx-5.0.0b1/pkg/debian/copyright
+-rwxr-xr-x   0        0        0     8937 2023-04-30 14:54:09.930705 weewx-5.0.0b1/pkg/debian/postinst
+-rwxr-xr-x   0        0        0      906 2023-03-10 17:12:41.258442 weewx-5.0.0b1/pkg/debian/postrm
+-rwxr-xr-x   0        0        0      410 2023-03-10 17:12:41.258442 weewx-5.0.0b1/pkg/debian/preinst
+-rwxr-xr-x   0        0        0      693 2023-04-30 14:54:09.930705 weewx-5.0.0b1/pkg/debian/prerm
+-rwxr-xr-x   0        0        0     2997 2023-05-06 12:11:54.181870 weewx-5.0.0b1/pkg/debian/rules
+-rw-r--r--   0        0        0       12 2020-03-05 01:18:46.000000 weewx-5.0.0b1/pkg/debian/source/format
+-rw-r--r--   0        0        0     5501 2023-04-30 14:54:09.934705 weewx-5.0.0b1/pkg/debian/templates
+-rw-r--r--   0        0        0     1708 2023-04-30 14:54:09.934705 weewx-5.0.0b1/pkg/index-apt.html
+-rw-r--r--   0        0        0     1728 2023-03-10 17:12:41.258442 weewx-5.0.0b1/pkg/index-suse.html
+-rw-r--r--   0        0        0     1714 2023-03-10 17:12:41.258442 weewx-5.0.0b1/pkg/index-yum.html
+-rwxr-xr-x   0        0        0     9874 2023-03-10 17:12:41.258442 weewx-5.0.0b1/pkg/mkchangelog.pl
+-rw-r--r--   0        0        0       79 2023-03-10 17:12:41.258442 weewx-5.0.0b1/pkg/weewx-el8.repo
+-rw-r--r--   0        0        0       57 2023-03-10 17:12:41.258442 weewx-5.0.0b1/pkg/weewx-python2.list
+-rw-r--r--   0        0        0       56 2023-03-10 17:12:41.258442 weewx-5.0.0b1/pkg/weewx-python3.list
+-rw-r--r--   0        0        0       83 2023-03-10 17:12:41.258442 weewx-5.0.0b1/pkg/weewx-suse12.repo
+-rw-r--r--   0        0        0       83 2023-03-10 17:12:41.258442 weewx-5.0.0b1/pkg/weewx-suse15.repo
+-rw-r--r--   0        0        0     2201 2023-03-10 17:12:41.258442 weewx-5.0.0b1/pkg/weewx.smf
+-rw-r--r--   0        0        0     7179 2023-05-06 12:11:54.181870 weewx-5.0.0b1/pkg/weewx.spec.in
+-rw-r--r--   0        0        0     2929 2023-05-06 12:11:54.181870 weewx-5.0.0b1/pyproject.toml
+-rw-r--r--   0        0        0      154 2023-03-10 17:12:41.266442 weewx-5.0.0b1/util/apache/conf-available/weewx.conf
+-rw-r--r--   0        0        0      167 2023-03-10 17:12:41.266442 weewx-5.0.0b1/util/apache/conf.d/weewx.conf
+-rw-r--r--   0        0        0      136 2023-04-30 14:54:09.934705 weewx-5.0.0b1/util/default/weewx
+-rwxr-xr-x   0        0        0     8897 2023-03-10 17:12:41.266442 weewx-5.0.0b1/util/i18n/i18n-report
+-rw-r--r--   0        0        0     9052 2023-03-10 17:12:41.266442 weewx-5.0.0b1/util/import/csv-example.conf
+-rw-r--r--   0        0        0     8250 2023-03-10 17:12:41.266442 weewx-5.0.0b1/util/import/cumulus-example.conf
+-rw-r--r--   0        0        0    14923 2023-03-10 17:12:41.266442 weewx-5.0.0b1/util/import/wd-example.conf
+-rw-r--r--   0        0        0     7100 2023-03-10 17:12:41.266442 weewx-5.0.0b1/util/import/weathercat-example.conf
+-rw-r--r--   0        0        0     6202 2023-03-10 17:12:41.266442 weewx-5.0.0b1/util/import/wu-example.conf
+-rwxr-xr-x   0        0        0     6057 2023-03-13 13:33:49.303977 weewx-5.0.0b1/util/init.d/weewx-multi
+-rwxr-xr-x   0        0        0      862 2023-03-13 13:33:49.303977 weewx-5.0.0b1/util/init.d/weewx.bsd
+-rwxr-xr-x   0        0        0     5111 2023-03-13 13:33:49.303977 weewx-5.0.0b1/util/init.d/weewx.debian
+-rw-r--r--   0        0        0      647 2023-03-13 13:33:49.303977 weewx-5.0.0b1/util/init.d/weewx.freebsd
+-rwxr-xr-x   0        0        0     8372 2023-03-13 13:33:49.303977 weewx-5.0.0b1/util/init.d/weewx.lsb
+-rwxr-xr-x   0        0        0     1659 2023-03-13 13:33:49.303977 weewx-5.0.0b1/util/init.d/weewx.redhat
+-rwxr-xr-x   0        0        0     4856 2023-03-13 13:33:49.303977 weewx-5.0.0b1/util/init.d/weewx.suse
+-rw-r--r--   0        0        0      914 2023-04-30 14:54:09.934705 weewx-5.0.0b1/util/launchd/com.weewx.weewxd.plist
+-rw-r--r--   0        0        0     1800 2023-03-10 17:12:41.266442 weewx-5.0.0b1/util/logrotate.d/weewx
+-rw-r--r--   0        0        0       83 2020-04-14 15:38:00.000000 weewx-5.0.0b1/util/logwatch/conf/logfiles/weewx.conf
+-rw-r--r--   0        0        0       32 2020-04-14 15:38:00.000000 weewx-5.0.0b1/util/logwatch/conf/services/weewx.conf
+-rwxr-xr-x   0        0        0    54942 2023-03-10 17:12:41.266442 weewx-5.0.0b1/util/logwatch/scripts/services/weewx
+-rw-r--r--   0        0        0       82 2023-03-10 17:12:41.266442 weewx-5.0.0b1/util/newsyslog.d/weewx.conf
+-rw-r--r--   0        0        0     2219 2023-03-10 17:12:41.266442 weewx-5.0.0b1/util/rsyslog.d/weewx.conf
+-rwxr-xr-x   0        0        0      319 2023-04-30 14:54:09.938705 weewx-5.0.0b1/util/scripts/wee_database
+-rwxr-xr-x   0        0        0      316 2023-04-30 14:54:09.938705 weewx-5.0.0b1/util/scripts/wee_debug
+-rwxr-xr-x   0        0        0      317 2023-04-30 14:54:09.938705 weewx-5.0.0b1/util/scripts/wee_device
+-rwxr-xr-x   0        0        0      317 2023-04-30 14:54:09.938705 weewx-5.0.0b1/util/scripts/wee_import
+-rwxr-xr-x   0        0        0      318 2023-04-30 14:54:09.938705 weewx-5.0.0b1/util/scripts/wee_reports
+-rwxr-xr-x   0        0        0      313 2023-04-30 14:54:09.938705 weewx-5.0.0b1/util/scripts/weectl
+-rwxr-xr-x   0        0        0      313 2023-04-30 14:54:09.938705 weewx-5.0.0b1/util/scripts/weewxd
+-rwxr-xr-x   0        0        0      318 2023-04-30 14:54:09.938705 weewx-5.0.0b1/util/scripts/wunderfixer
+-rw-r--r--   0        0        0     2564 2023-03-10 17:12:41.266442 weewx-5.0.0b1/util/solaris/weewx-smf.xml
+-rw-r--r--   0        0        0      536 2023-03-28 23:07:34.757396 weewx-5.0.0b1/util/systemd/weewx.service
+-rw-r--r--   0        0        0       34 2023-03-10 17:12:41.266442 weewx-5.0.0b1/util/tmpfiles.d/weewx.conf
+-rw-r--r--   0        0        0      149 2020-04-14 15:38:00.000000 weewx-5.0.0b1/util/udev/rules.d/acurite.rules
+-rw-r--r--   0        0        0      135 2023-03-10 17:12:41.266442 weewx-5.0.0b1/util/udev/rules.d/cc3000.rules
+-rw-r--r--   0        0        0      153 2020-04-14 15:38:00.000000 weewx-5.0.0b1/util/udev/rules.d/fousb.rules
+-rw-r--r--   0        0        0      147 2020-04-14 15:38:00.000000 weewx-5.0.0b1/util/udev/rules.d/te923.rules
+-rw-r--r--   0        0        0      624 2023-03-10 17:12:41.266442 weewx-5.0.0b1/util/udev/rules.d/vantage.rules
+-rw-r--r--   0        0        0     1560 2023-03-10 17:12:41.266442 weewx-5.0.0b1/util/udev/rules.d/weewx.rules
+-rw-r--r--   0        0        0      158 2020-04-14 15:38:00.000000 weewx-5.0.0b1/util/udev/rules.d/wmr100.rules
+-rw-r--r--   0        0        0      158 2020-04-14 15:38:00.000000 weewx-5.0.0b1/util/udev/rules.d/wmr300.rules
+-rw-r--r--   0        0        0      152 2020-04-14 15:38:00.000000 weewx-5.0.0b1/util/udev/rules.d/ws28xx.rules
+-rw-r--r--   0        0        0     5071 1970-01-01 00:00:00.000000 weewx-5.0.0b1/PKG-INFO
```

### Comparing `weewx-5.0.0a30/LICENSE.txt` & `weewx-5.0.0b1/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `weewx-5.0.0a30/README.md` & `weewx-5.0.0b1/README.md`

 * *Files identical despite different names*

### Comparing `weewx-5.0.0a30/bin/schemas/wview.py` & `weewx-5.0.0b1/bin/schemas/wview.py`

 * *Files identical despite different names*

### Comparing `weewx-5.0.0a30/bin/schemas/wview_extended.py` & `weewx-5.0.0b1/bin/schemas/wview_extended.py`

 * *Files identical despite different names*

### Comparing `weewx-5.0.0a30/bin/schemas/wview_small.py` & `weewx-5.0.0b1/bin/schemas/wview_small.py`

 * *Files identical despite different names*

### Comparing `weewx-5.0.0a30/bin/wee_database.py` & `weewx-5.0.0b1/bin/wee_database.py`

 * *Files identical despite different names*

### Comparing `weewx-5.0.0a30/bin/wee_debug.py` & `weewx-5.0.0b1/bin/wee_debug.py`

 * *Files identical despite different names*

### Comparing `weewx-5.0.0a30/bin/wee_device.py` & `weewx-5.0.0b1/bin/wee_device.py`

 * *Files identical despite different names*

### Comparing `weewx-5.0.0a30/bin/wee_import.py` & `weewx-5.0.0b1/bin/wee_import.py`

 * *Files identical despite different names*

### Comparing `weewx-5.0.0a30/bin/wee_reports.py` & `weewx-5.0.0b1/bin/wee_reports.py`

 * *Files identical despite different names*

### Comparing `weewx-5.0.0a30/bin/wee_resources/bin/user/extensions.py` & `weewx-5.0.0b1/bin/wee_resources/bin/user/extensions.py`

 * *Files identical despite different names*

### Comparing `weewx-5.0.0a30/bin/wee_resources/docs/404.html` & `weewx-5.0.0b1/bin/wee_resources/docs/404.html`

 * *Files identical despite different names*

### Comparing `weewx-5.0.0a30/bin/wee_resources/docs/assets/images/favicon.png` & `weewx-5.0.0b1/bin/wee_resources/docs/assets/images/favicon.png`

 * *Files identical despite different names*

### Comparing `weewx-5.0.0a30/bin/wee_resources/docs/assets/javascripts/bundle.4b2c34cd.min.js` & `weewx-5.0.0b1/bin/wee_resources/docs/assets/javascripts/bundle.4b2c34cd.min.js`

 * *Files identical despite different names*

### Comparing `weewx-5.0.0a30/bin/wee_resources/docs/assets/javascripts/bundle.4b2c34cd.min.js.map` & `weewx-5.0.0b1/bin/wee_resources/docs/assets/javascripts/bundle.4b2c34cd.min.js.map`

 * *Files identical despite different names*

### Comparing `weewx-5.0.0a30/bin/wee_resources/docs/assets/javascripts/lunr/min/lunr.ar.min.js` & `weewx-5.0.0b1/bin/wee_resources/docs/assets/javascripts/lunr/min/lunr.ar.min.js`

 * *Files identical despite different names*

### Comparing `weewx-5.0.0a30/bin/wee_resources/docs/assets/javascripts/lunr/min/lunr.da.min.js` & `weewx-5.0.0b1/bin/wee_resources/docs/assets/javascripts/lunr/min/lunr.da.min.js`

 * *Files identical despite different names*

### Comparing `weewx-5.0.0a30/bin/wee_resources/docs/assets/javascripts/lunr/min/lunr.de.min.js` & `weewx-5.0.0b1/bin/wee_resources/docs/assets/javascripts/lunr/min/lunr.de.min.js`

 * *Files identical despite different names*

### Comparing `weewx-5.0.0a30/bin/wee_resources/docs/assets/javascripts/lunr/min/lunr.du.min.js` & `weewx-5.0.0b1/bin/wee_resources/docs/assets/javascripts/lunr/min/lunr.du.min.js`

 * *Files identical despite different names*

### Comparing `weewx-5.0.0a30/bin/wee_resources/docs/assets/javascripts/lunr/min/lunr.es.min.js` & `weewx-5.0.0b1/bin/wee_resources/docs/assets/javascripts/lunr/min/lunr.es.min.js`

 * *Files identical despite different names*

### Comparing `weewx-5.0.0a30/bin/wee_resources/docs/assets/javascripts/lunr/min/lunr.fi.min.js` & `weewx-5.0.0b1/bin/wee_resources/docs/assets/javascripts/lunr/min/lunr.fi.min.js`

 * *Files identical despite different names*

### Comparing `weewx-5.0.0a30/bin/wee_resources/docs/assets/javascripts/lunr/min/lunr.fr.min.js` & `weewx-5.0.0b1/bin/wee_resources/docs/assets/javascripts/lunr/min/lunr.fr.min.js`

 * *Files identical despite different names*

### Comparing `weewx-5.0.0a30/bin/wee_resources/docs/assets/javascripts/lunr/min/lunr.hi.min.js` & `weewx-5.0.0b1/bin/wee_resources/docs/assets/javascripts/lunr/min/lunr.hi.min.js`

 * *Files identical despite different names*

### Comparing `weewx-5.0.0a30/bin/wee_resources/docs/assets/javascripts/lunr/min/lunr.hu.min.js` & `weewx-5.0.0b1/bin/wee_resources/docs/assets/javascripts/lunr/min/lunr.hu.min.js`

 * *Files identical despite different names*

### Comparing `weewx-5.0.0a30/bin/wee_resources/docs/assets/javascripts/lunr/min/lunr.it.min.js` & `weewx-5.0.0b1/bin/wee_resources/docs/assets/javascripts/lunr/min/lunr.it.min.js`

 * *Files identical despite different names*

### Comparing `weewx-5.0.0a30/bin/wee_resources/docs/assets/javascripts/lunr/min/lunr.ja.min.js` & `weewx-5.0.0b1/bin/wee_resources/docs/assets/javascripts/lunr/min/lunr.ja.min.js`

 * *Files identical despite different names*

### Comparing `weewx-5.0.0a30/bin/wee_resources/docs/assets/javascripts/lunr/min/lunr.ko.min.js` & `weewx-5.0.0b1/bin/wee_resources/docs/assets/javascripts/lunr/min/lunr.ko.min.js`

 * *Files identical despite different names*

### Comparing `weewx-5.0.0a30/bin/wee_resources/docs/assets/javascripts/lunr/min/lunr.multi.min.js` & `weewx-5.0.0b1/bin/wee_resources/docs/assets/javascripts/lunr/min/lunr.multi.min.js`

 * *Files identical despite different names*

### Comparing `weewx-5.0.0a30/bin/wee_resources/docs/assets/javascripts/lunr/min/lunr.nl.min.js` & `weewx-5.0.0b1/bin/wee_resources/docs/assets/javascripts/lunr/min/lunr.nl.min.js`

 * *Files identical despite different names*

### Comparing `weewx-5.0.0a30/bin/wee_resources/docs/assets/javascripts/lunr/min/lunr.no.min.js` & `weewx-5.0.0b1/bin/wee_resources/docs/assets/javascripts/lunr/min/lunr.no.min.js`

 * *Files identical despite different names*

### Comparing `weewx-5.0.0a30/bin/wee_resources/docs/assets/javascripts/lunr/min/lunr.pt.min.js` & `weewx-5.0.0b1/bin/wee_resources/docs/assets/javascripts/lunr/min/lunr.pt.min.js`

 * *Files identical despite different names*

### Comparing `weewx-5.0.0a30/bin/wee_resources/docs/assets/javascripts/lunr/min/lunr.ro.min.js` & `weewx-5.0.0b1/bin/wee_resources/docs/assets/javascripts/lunr/min/lunr.ro.min.js`

 * *Files identical despite different names*

### Comparing `weewx-5.0.0a30/bin/wee_resources/docs/assets/javascripts/lunr/min/lunr.ru.min.js` & `weewx-5.0.0b1/bin/wee_resources/docs/assets/javascripts/lunr/min/lunr.ru.min.js`

 * *Files identical despite different names*

### Comparing `weewx-5.0.0a30/bin/wee_resources/docs/assets/javascripts/lunr/min/lunr.stemmer.support.min.js` & `weewx-5.0.0b1/bin/wee_resources/docs/assets/javascripts/lunr/min/lunr.stemmer.support.min.js`

 * *Files identical despite different names*

### Comparing `weewx-5.0.0a30/bin/wee_resources/docs/assets/javascripts/lunr/min/lunr.sv.min.js` & `weewx-5.0.0b1/bin/wee_resources/docs/assets/javascripts/lunr/min/lunr.sv.min.js`

 * *Files identical despite different names*

### Comparing `weewx-5.0.0a30/bin/wee_resources/docs/assets/javascripts/lunr/min/lunr.ta.min.js` & `weewx-5.0.0b1/bin/wee_resources/docs/assets/javascripts/lunr/min/lunr.ta.min.js`

 * *Files identical despite different names*

### Comparing `weewx-5.0.0a30/bin/wee_resources/docs/assets/javascripts/lunr/min/lunr.th.min.js` & `weewx-5.0.0b1/bin/wee_resources/docs/assets/javascripts/lunr/min/lunr.th.min.js`

 * *Files identical despite different names*

### Comparing `weewx-5.0.0a30/bin/wee_resources/docs/assets/javascripts/lunr/min/lunr.tr.min.js` & `weewx-5.0.0b1/bin/wee_resources/docs/assets/javascripts/lunr/min/lunr.tr.min.js`

 * *Files identical despite different names*

### Comparing `weewx-5.0.0a30/bin/wee_resources/docs/assets/javascripts/lunr/min/lunr.vi.min.js` & `weewx-5.0.0b1/bin/wee_resources/docs/assets/javascripts/lunr/min/lunr.vi.min.js`

 * *Files identical despite different names*

### Comparing `weewx-5.0.0a30/bin/wee_resources/docs/assets/javascripts/lunr/min/lunr.zh.min.js` & `weewx-5.0.0b1/bin/wee_resources/docs/assets/javascripts/lunr/min/lunr.zh.min.js`

 * *Files identical despite different names*

### Comparing `weewx-5.0.0a30/bin/wee_resources/docs/assets/javascripts/lunr/tinyseg.js` & `weewx-5.0.0b1/bin/wee_resources/docs/assets/javascripts/lunr/tinyseg.js`

 * *Files identical despite different names*

### Comparing `weewx-5.0.0a30/bin/wee_resources/docs/assets/javascripts/lunr/wordcut.js` & `weewx-5.0.0b1/bin/wee_resources/docs/assets/javascripts/lunr/wordcut.js`

 * *Files identical despite different names*

### Comparing `weewx-5.0.0a30/bin/wee_resources/docs/assets/javascripts/workers/search.db81ec45.min.js` & `weewx-5.0.0b1/bin/wee_resources/docs/assets/javascripts/workers/search.db81ec45.min.js`

 * *Files identical despite different names*

### Comparing `weewx-5.0.0a30/bin/wee_resources/docs/assets/javascripts/workers/search.db81ec45.min.js.map` & `weewx-5.0.0b1/bin/wee_resources/docs/assets/javascripts/workers/search.db81ec45.min.js.map`

 * *Files identical despite different names*

### Comparing `weewx-5.0.0a30/bin/wee_resources/docs/assets/stylesheets/main.0d440cfe.min.css` & `weewx-5.0.0b1/bin/wee_resources/docs/assets/stylesheets/main.0d440cfe.min.css`

 * *Files identical despite different names*

### Comparing `weewx-5.0.0a30/bin/wee_resources/docs/assets/stylesheets/main.0d440cfe.min.css.map` & `weewx-5.0.0b1/bin/wee_resources/docs/assets/stylesheets/main.0d440cfe.min.css.map`

 * *Files identical despite different names*

### Comparing `weewx-5.0.0a30/bin/wee_resources/docs/assets/stylesheets/palette.2505c338.min.css` & `weewx-5.0.0b1/bin/wee_resources/docs/assets/stylesheets/palette.2505c338.min.css`

 * *Files identical despite different names*

### Comparing `weewx-5.0.0a30/bin/wee_resources/docs/assets/stylesheets/palette.2505c338.min.css.map` & `weewx-5.0.0b1/bin/wee_resources/docs/assets/stylesheets/palette.2505c338.min.css.map`

 * *Files identical despite different names*

### Comparing `weewx-5.0.0a30/bin/wee_resources/docs/changes/index.html` & `weewx-5.0.0b1/bin/wee_resources/docs/changes/index.html`

 * *Files identical despite different names*

### Comparing `weewx-5.0.0a30/bin/wee_resources/docs/copyright/index.html` & `weewx-5.0.0b1/bin/wee_resources/docs/copyright/index.html`

 * *Files identical despite different names*

### Comparing `weewx-5.0.0a30/bin/wee_resources/docs/css/tocbot-4.12.0.css` & `weewx-5.0.0b1/bin/wee_resources/docs/css/tocbot-4.12.0.css`

 * *Files identical despite different names*

### Comparing `weewx-5.0.0a30/bin/wee_resources/docs/css/tocbot-4.3.1.css` & `weewx-5.0.0b1/bin/wee_resources/docs/css/tocbot-4.3.1.css`

 * *Files identical despite different names*

### Comparing `weewx-5.0.0a30/bin/wee_resources/docs/css/weewx_ui.css` & `weewx-5.0.0b1/bin/wee_resources/docs/css/weewx_ui.css`

 * *Files identical despite different names*

### Comparing `weewx-5.0.0a30/bin/wee_resources/docs/custom/appendix/index.html` & `weewx-5.0.0b1/bin/wee_resources/docs/custom/appendix/index.html`

 * *Files identical despite different names*

### Comparing `weewx-5.0.0a30/bin/wee_resources/docs/custom/cheetah/index.html` & `weewx-5.0.0b1/bin/wee_resources/docs/custom/cheetah/index.html`

 * *Files identical despite different names*

### Comparing `weewx-5.0.0a30/bin/wee_resources/docs/custom/custom_reports/index.html` & `weewx-5.0.0b1/bin/wee_resources/docs/custom/custom_reports/index.html`

 * *Files identical despite different names*

### Comparing `weewx-5.0.0a30/bin/wee_resources/docs/custom/database/index.html` & `weewx-5.0.0b1/bin/wee_resources/docs/custom/database/index.html`

 * *Files identical despite different names*

### Comparing `weewx-5.0.0a30/bin/wee_resources/docs/custom/derived/index.html` & `weewx-5.0.0b1/bin/wee_resources/docs/custom/derived/index.html`

 * *Files identical despite different names*

### Comparing `weewx-5.0.0a30/bin/wee_resources/docs/custom/drivers/index.html` & `weewx-5.0.0b1/bin/wee_resources/docs/custom/drivers/index.html`

 * *Files identical despite different names*

### Comparing `weewx-5.0.0a30/bin/wee_resources/docs/custom/extensions/index.html` & `weewx-5.0.0b1/bin/wee_resources/docs/custom/extensions/index.html`

 * *Files identical despite different names*

### Comparing `weewx-5.0.0a30/bin/wee_resources/docs/custom/image_generator/index.html` & `weewx-5.0.0b1/bin/wee_resources/docs/custom/image_generator/index.html`

 * *Files identical despite different names*

### Comparing `weewx-5.0.0a30/bin/wee_resources/docs/custom/index.html` & `weewx-5.0.0b1/bin/wee_resources/docs/custom/index.html`

 * *Files identical despite different names*

### Comparing `weewx-5.0.0a30/bin/wee_resources/docs/custom/localization/index.html` & `weewx-5.0.0b1/bin/wee_resources/docs/custom/localization/index.html`

 * *Files identical despite different names*

### Comparing `weewx-5.0.0a30/bin/wee_resources/docs/custom/multiple_bindings/index.html` & `weewx-5.0.0b1/bin/wee_resources/docs/custom/multiple_bindings/index.html`

 * *Files identical despite different names*

### Comparing `weewx-5.0.0a30/bin/wee_resources/docs/custom/options_ref/index.html` & `weewx-5.0.0b1/bin/wee_resources/docs/custom/options_ref/index.html`

 * *Files identical despite different names*

### Comparing `weewx-5.0.0a30/bin/wee_resources/docs/custom/service_engine/index.html` & `weewx-5.0.0b1/bin/wee_resources/docs/custom/service_engine/index.html`

 * *Files identical despite different names*

### Comparing `weewx-5.0.0a30/bin/wee_resources/docs/custom/units/index.html` & `weewx-5.0.0b1/bin/wee_resources/docs/custom/units/index.html`

 * *Files identical despite different names*

### Comparing `weewx-5.0.0a30/bin/wee_resources/docs/devnotes/index.html` & `weewx-5.0.0b1/bin/wee_resources/docs/devnotes/index.html`

 * *Files identical despite different names*

### Comparing `weewx-5.0.0a30/bin/wee_resources/docs/examples/tag.htm` & `weewx-5.0.0b1/bin/wee_resources/docs/examples/tag.htm`

 * *Files identical despite different names*

### Comparing `weewx-5.0.0a30/bin/wee_resources/docs/hardware.htm` & `weewx-5.0.0b1/bin/wee_resources/docs/hardware.htm`

 * *Files identical despite different names*

### Comparing `weewx-5.0.0a30/bin/wee_resources/docs/images/antialias.gif` & `weewx-5.0.0b1/bin/wee_resources/docs/images/antialias.gif`

 * *Files identical despite different names*

### Comparing `weewx-5.0.0a30/bin/wee_resources/docs/images/day-gap-not-shown.png` & `weewx-5.0.0b1/bin/wee_resources/docs/images/day-gap-not-shown.png`

 * *Files identical despite different names*

### Comparing `weewx-5.0.0a30/bin/wee_resources/docs/images/day-gap-showing.png` & `weewx-5.0.0b1/bin/wee_resources/docs/images/day-gap-showing.png`

 * *Files identical despite different names*

### Comparing `weewx-5.0.0a30/bin/wee_resources/docs/images/daycompare.png` & `weewx-5.0.0b1/bin/wee_resources/docs/images/daycompare.png`

 * *Files identical despite different names*

### Comparing `weewx-5.0.0a30/bin/wee_resources/docs/images/daytemp_with_avg.png` & `weewx-5.0.0b1/bin/wee_resources/docs/images/daytemp_with_avg.png`

 * *Files identical despite different names*

### Comparing `weewx-5.0.0a30/bin/wee_resources/docs/images/dayvaporp.png` & `weewx-5.0.0b1/bin/wee_resources/docs/images/dayvaporp.png`

 * *Files identical despite different names*

### Comparing `weewx-5.0.0a30/bin/wee_resources/docs/images/daywindvec.png` & `weewx-5.0.0b1/bin/wee_resources/docs/images/daywindvec.png`

 * *Files identical despite different names*

### Comparing `weewx-5.0.0a30/bin/wee_resources/docs/images/favicon.png` & `weewx-5.0.0b1/bin/wee_resources/docs/images/favicon.png`

 * *Files identical despite different names*

### Comparing `weewx-5.0.0a30/bin/wee_resources/docs/images/ferrites.jpg` & `weewx-5.0.0b1/bin/wee_resources/docs/images/ferrites.jpg`

 * *Files identical despite different names*

### Comparing `weewx-5.0.0a30/bin/wee_resources/docs/images/funky_degree.png` & `weewx-5.0.0b1/bin/wee_resources/docs/images/funky_degree.png`

 * *Files identical despite different names*

### Comparing `weewx-5.0.0a30/bin/wee_resources/docs/images/image_parts.png` & `weewx-5.0.0b1/bin/wee_resources/docs/images/image_parts.png`

 * *Files identical despite different names*

### Comparing `weewx-5.0.0a30/bin/wee_resources/docs/images/image_parts.xcf` & `weewx-5.0.0b1/bin/wee_resources/docs/images/image_parts.xcf`

 * *Files identical despite different names*

### Comparing `weewx-5.0.0a30/bin/wee_resources/docs/images/logo-apple.png` & `weewx-5.0.0b1/bin/wee_resources/docs/images/logo-apple.png`

 * *Files identical despite different names*

### Comparing `weewx-5.0.0a30/bin/wee_resources/docs/images/logo-centos.png` & `weewx-5.0.0b1/bin/wee_resources/docs/images/logo-centos.png`

 * *Files identical despite different names*

### Comparing `weewx-5.0.0a30/bin/wee_resources/docs/images/logo-debian.png` & `weewx-5.0.0b1/bin/wee_resources/docs/images/logo-debian.png`

 * *Files identical despite different names*

### Comparing `weewx-5.0.0a30/bin/wee_resources/docs/images/logo-fedora.png` & `weewx-5.0.0b1/bin/wee_resources/docs/images/logo-fedora.png`

 * *Files identical despite different names*

### Comparing `weewx-5.0.0a30/bin/wee_resources/docs/images/logo-linux.png` & `weewx-5.0.0b1/bin/wee_resources/docs/images/logo-linux.png`

 * *Files identical despite different names*

### Comparing `weewx-5.0.0a30/bin/wee_resources/docs/images/logo-mint.png` & `weewx-5.0.0b1/bin/wee_resources/docs/images/logo-mint.png`

 * *Files identical despite different names*

### Comparing `weewx-5.0.0a30/bin/wee_resources/docs/images/logo-opensuse.png` & `weewx-5.0.0b1/bin/wee_resources/docs/images/logo-opensuse.png`

 * *Files identical despite different names*

### Comparing `weewx-5.0.0a30/bin/wee_resources/docs/images/logo-pypi.svg` & `weewx-5.0.0b1/bin/wee_resources/docs/images/logo-pypi.svg`

 * *Files identical despite different names*

### Comparing `weewx-5.0.0a30/bin/wee_resources/docs/images/logo-redhat.png` & `weewx-5.0.0b1/bin/wee_resources/docs/images/logo-redhat.png`

 * *Files identical despite different names*

### Comparing `weewx-5.0.0a30/bin/wee_resources/docs/images/logo-rpi.png` & `weewx-5.0.0b1/bin/wee_resources/docs/images/logo-rpi.png`

 * *Files identical despite different names*

### Comparing `weewx-5.0.0a30/bin/wee_resources/docs/images/logo-suse.png` & `weewx-5.0.0b1/bin/wee_resources/docs/images/logo-suse.png`

 * *Files identical despite different names*

### Comparing `weewx-5.0.0a30/bin/wee_resources/docs/images/logo-ubuntu.png` & `weewx-5.0.0b1/bin/wee_resources/docs/images/logo-ubuntu.png`

 * *Files identical despite different names*

### Comparing `weewx-5.0.0a30/bin/wee_resources/docs/images/logo-weewx.png` & `weewx-5.0.0b1/bin/wee_resources/docs/images/logo-weewx.png`

 * *Files identical despite different names*

### Comparing `weewx-5.0.0a30/bin/wee_resources/docs/images/pipeline.png` & `weewx-5.0.0b1/bin/wee_resources/docs/images/pipeline.png`

 * *Files identical despite different names*

### Comparing `weewx-5.0.0a30/bin/wee_resources/docs/images/sample_monthrain.png` & `weewx-5.0.0b1/bin/wee_resources/docs/images/sample_monthrain.png`

 * *Files identical despite different names*

### Comparing `weewx-5.0.0a30/bin/wee_resources/docs/images/sample_monthtempdew.png` & `weewx-5.0.0b1/bin/wee_resources/docs/images/sample_monthtempdew.png`

 * *Files identical despite different names*

### Comparing `weewx-5.0.0a30/bin/wee_resources/docs/images/weekgustoverlay.png` & `weewx-5.0.0b1/bin/wee_resources/docs/images/weekgustoverlay.png`

 * *Files identical despite different names*

### Comparing `weewx-5.0.0a30/bin/wee_resources/docs/images/weektempdew.png` & `weewx-5.0.0b1/bin/wee_resources/docs/images/weektempdew.png`

 * *Files identical despite different names*

### Comparing `weewx-5.0.0a30/bin/wee_resources/docs/images/yeardiff.png` & `weewx-5.0.0b1/bin/wee_resources/docs/images/yeardiff.png`

 * *Files identical despite different names*

### Comparing `weewx-5.0.0a30/bin/wee_resources/docs/images/yearhilow.png` & `weewx-5.0.0b1/bin/wee_resources/docs/images/yearhilow.png`

 * *Files identical despite different names*

### Comparing `weewx-5.0.0a30/bin/wee_resources/docs/index.html` & `weewx-5.0.0b1/bin/wee_resources/docs/index.html`

 * *Files identical despite different names*

### Comparing `weewx-5.0.0a30/bin/wee_resources/docs/js/cash.js` & `weewx-5.0.0b1/bin/wee_resources/docs/js/cash.js`

 * *Files identical despite different names*

### Comparing `weewx-5.0.0a30/bin/wee_resources/docs/js/cash.min.js` & `weewx-5.0.0b1/bin/wee_resources/docs/js/cash.min.js`

 * *Files identical despite different names*

### Comparing `weewx-5.0.0a30/bin/wee_resources/docs/js/tocbot-4.12.0.js` & `weewx-5.0.0b1/bin/wee_resources/docs/js/tocbot-4.12.0.js`

 * *Files identical despite different names*

### Comparing `weewx-5.0.0a30/bin/wee_resources/docs/js/tocbot-4.12.0.min.js` & `weewx-5.0.0b1/bin/wee_resources/docs/js/tocbot-4.12.0.min.js`

 * *Files identical despite different names*

### Comparing `weewx-5.0.0a30/bin/wee_resources/docs/js/tocbot-4.3.1.min.js` & `weewx-5.0.0b1/bin/wee_resources/docs/js/tocbot-4.3.1.min.js`

 * *Files identical despite different names*

### Comparing `weewx-5.0.0a30/bin/wee_resources/docs/js/weewx.js` & `weewx-5.0.0b1/bin/wee_resources/docs/js/weewx.js`

 * *Files identical despite different names*

### Comparing `weewx-5.0.0a30/bin/wee_resources/docs/quickstarts/debian/index.html` & `weewx-5.0.0b1/bin/wee_resources/docs/quickstarts/debian/index.html`

 * *Files identical despite different names*

### Comparing `weewx-5.0.0a30/bin/wee_resources/docs/quickstarts/index.html` & `weewx-5.0.0b1/bin/wee_resources/docs/quickstarts/index.html`

 * *Files identical despite different names*

### Comparing `weewx-5.0.0a30/bin/wee_resources/docs/quickstarts/pip/index.html` & `weewx-5.0.0b1/bin/wee_resources/docs/quickstarts/pip/index.html`

 * *Files 10% similar despite different names*

```diff
@@ -369,26 +369,26 @@
     <label class="md-nav__title" for="__toc">
       <span class="md-nav__icon md-icon"></span>
       Table of contents
     </label>
     <ul class="md-nav__list" data-md-component="toc" data-md-scrollfix>
       
         <li class="md-nav__item">
-  <a href="#preparation" class="md-nav__link">
-    Preparation
+  <a href="#prepare-for-install" class="md-nav__link">
+    Prepare for install
   </a>
   
 </li>
       
         <li class="md-nav__item">
-  <a href="#installation-steps" class="md-nav__link">
-    Installation steps
+  <a href="#install" class="md-nav__link">
+    Install
   </a>
   
-    <nav class="md-nav" aria-label="Installation steps">
+    <nav class="md-nav" aria-label="Install">
       <ul class="md-nav__list">
         
           <li class="md-nav__item">
   <a href="#step-1-install-the-application-using-pip" class="md-nav__link">
     Step 1: Install the application using pip
   </a>
   
@@ -403,19 +403,19 @@
         
       </ul>
     </nav>
   
 </li>
       
         <li class="md-nav__item">
-  <a href="#running-weewxd" class="md-nav__link">
-    Running weewxd
+  <a href="#run-weewxd" class="md-nav__link">
+    Run weewxd
   </a>
   
-    <nav class="md-nav" aria-label="Running weewxd">
+    <nav class="md-nav" aria-label="Run weewxd">
       <ul class="md-nav__list">
         
           <li class="md-nav__item">
   <a href="#run-directly" class="md-nav__link">
     Run directly
   </a>
   
@@ -424,25 +424,25 @@
           <li class="md-nav__item">
   <a href="#run-as-a-daemon" class="md-nav__link">
     Run as a daemon
   </a>
   
 </li>
         
-          <li class="md-nav__item">
+      </ul>
+    </nav>
+  
+</li>
+      
+        <li class="md-nav__item">
   <a href="#verify" class="md-nav__link">
     Verify
   </a>
   
 </li>
-        
-      </ul>
-    </nav>
-  
-</li>
       
         <li class="md-nav__item">
   <a href="#configure" class="md-nav__link">
     Configure
   </a>
   
 </li>
@@ -1538,26 +1538,26 @@
     <label class="md-nav__title" for="__toc">
       <span class="md-nav__icon md-icon"></span>
       Table of contents
     </label>
     <ul class="md-nav__list" data-md-component="toc" data-md-scrollfix>
       
         <li class="md-nav__item">
-  <a href="#preparation" class="md-nav__link">
-    Preparation
+  <a href="#prepare-for-install" class="md-nav__link">
+    Prepare for install
   </a>
   
 </li>
       
         <li class="md-nav__item">
-  <a href="#installation-steps" class="md-nav__link">
-    Installation steps
+  <a href="#install" class="md-nav__link">
+    Install
   </a>
   
-    <nav class="md-nav" aria-label="Installation steps">
+    <nav class="md-nav" aria-label="Install">
       <ul class="md-nav__list">
         
           <li class="md-nav__item">
   <a href="#step-1-install-the-application-using-pip" class="md-nav__link">
     Step 1: Install the application using pip
   </a>
   
@@ -1572,19 +1572,19 @@
         
       </ul>
     </nav>
   
 </li>
       
         <li class="md-nav__item">
-  <a href="#running-weewxd" class="md-nav__link">
-    Running weewxd
+  <a href="#run-weewxd" class="md-nav__link">
+    Run weewxd
   </a>
   
-    <nav class="md-nav" aria-label="Running weewxd">
+    <nav class="md-nav" aria-label="Run weewxd">
       <ul class="md-nav__list">
         
           <li class="md-nav__item">
   <a href="#run-directly" class="md-nav__link">
     Run directly
   </a>
   
@@ -1593,25 +1593,25 @@
           <li class="md-nav__item">
   <a href="#run-as-a-daemon" class="md-nav__link">
     Run as a daemon
   </a>
   
 </li>
         
-          <li class="md-nav__item">
+      </ul>
+    </nav>
+  
+</li>
+      
+        <li class="md-nav__item">
   <a href="#verify" class="md-nav__link">
     Verify
   </a>
   
 </li>
-        
-      </ul>
-    </nav>
-  
-</li>
       
         <li class="md-nav__item">
   <a href="#configure" class="md-nav__link">
     Configure
   </a>
   
 </li>
@@ -1643,34 +1643,36 @@
               <article class="md-content__inner md-typeset">
                 
                   
 
 
 
 <h1 id="installation-using-pip">Installation using pip<a class="headerlink" href="#installation-using-pip" title="Permanent link">&para;</a></h1>
-<p>This is a guide to installing WeeWX using <a href="https://pip.pypa.io">pip</a>. It can be used to
-install WeeWX on almost any operating system, including macOS.</p>
-<h2 id="preparation">Preparation<a class="headerlink" href="#preparation" title="Permanent link">&para;</a></h2>
+<p>This is a guide to installing WeeWX using <a href="https://pip.pypa.io">pip</a>. It can
+be used to install WeeWX on almost any operating system, including macOS.</p>
+<h2 id="prepare-for-install">Prepare for install<a class="headerlink" href="#prepare-for-install" title="Permanent link">&para;</a></h2>
 <ul>
 <li>
-<p>WeeWX V5.x requires Python 3.7 or greater. It cannot be run with Python 2.x.  If you are constrained by this, install WeeWX V4.10, the
-  last version to support Python 2.7, Python 3.5, and Python 3.6.</p>
+<p>WeeWX V5.x requires Python 3.7 or greater. It cannot be run with Python 2.x.
+  If you are constrained by this, install WeeWX V4.10, the last version to
+  support Python 2.7, Python 3.5, and Python 3.6.</p>
 </li>
 <li>
-<p>You must also have a copy of pip. In most cases, your operating system will offer an
-  <a href="https://packaging.python.org/en/latest/guides/installing-using-linux-tools/">installation package</a>.
+<p>You must also have a copy of pip. In most cases, your operating system will
+  offer an <a href="https://packaging.python.org/en/latest/guides/installing-using-linux-tools/">installation package</a>.
   Otherwise, <a href="https://pip.pypa.io/en/stable/installation/">see the directions on the pip website</a>.</p>
 </li>
 <li>
-<p>While you will not need root privileges to install and configure WeeWX,
-  you will need them to set up a daemon and, perhaps, to change device permissions.</p>
+<p>While you will not need root privileges to install and configure WeeWX, you
+  will need them to set up a daemon and, perhaps, to change device permissions.</p>
 </li>
 </ul>
-<p>Depending on your operating system and how complete it is, you may have to install some tools
-before beginning. Follow the directions below for your system:</p>
+<p>Depending on your operating system and what has already been installed, you may
+have to install some tools before beginning. Follow the directions below for
+your system:</p>
 <div class="tabbed-set tabbed-alternate" data-tabs="1:3"><input checked="checked" id="__tabbed_1_1" name="__tabbed_1" type="radio" /><input id="__tabbed_1_2" name="__tabbed_1" type="radio" /><input id="__tabbed_1_3" name="__tabbed_1" type="radio" /><div class="tabbed-labels"><label for="__tabbed_1_1">Debian</label><label for="__tabbed_1_2">Redhat</label><label for="__tabbed_1_3">openSUSE Leap</label></div>
 <div class="tabbed-content">
 <div class="tabbed-block">
 <div class="highlight"><pre><span></span><code>sudo<span class="w"> </span>apt<span class="w"> </span>update<span class="w"> </span><span class="o">&amp;&amp;</span><span class="w"> </span>sudo<span class="w"> </span>apt<span class="w"> </span>upgrade
 sudo<span class="w"> </span>apt<span class="w"> </span>-y<span class="w"> </span>install<span class="w"> </span>gcc
 sudo<span class="w"> </span>apt<span class="w"> </span>-y<span class="w"> </span>install<span class="w"> </span>python3-dev
 <span class="c1"># This makes the install of pyephem go more smoothly:</span>
@@ -1684,176 +1686,153 @@
 <span class="c1"># This makes the install of pyephem go more smoothly:</span>
 python3<span class="w"> </span>-m<span class="w"> </span>pip<span class="w"> </span>install<span class="w"> </span>wheel
 </code></pre></div>
 </div>
 <div class="tabbed-block">
 <div class="highlight"><pre><span></span><code><span class="c1"># Check to see what version of Python you have:</span>
 python3<span class="w"> </span>-V
-<span class="c1"># If it is less than Python 3.7, you will have to upgrade to a </span>
-<span class="c1"># later version. The following installs 3.9. Afterwards, you must</span>
-<span class="c1"># invoke Python by using &quot;python3.9&quot;, NOT &quot;python3&quot;</span>
+
+<span class="c1"># If it is less than Python 3.7, you will have to upgrade to a later</span>
+<span class="c1"># version. The following installs 3.9. Afterwards, you must invoke Python</span>
+<span class="c1"># by using &quot;python3.9&quot;, NOT &quot;python3&quot;</span>
 sudo<span class="w"> </span>zypper<span class="w"> </span>install<span class="w"> </span>-y<span class="w"> </span>python39<span class="w"> </span>python39-devel
 python3.9<span class="w"> </span>-m<span class="w"> </span>pip<span class="w"> </span>install<span class="w"> </span>wheel
 
 <span class="c1"># Finally, you may have to add ~/.local/bin to your path:</span>
 <span class="nb">echo</span><span class="w"> </span><span class="s1">&#39;export PATH=&quot;$PATH:$HOME/.local/bin&quot;&#39;</span><span class="w"> </span>&gt;&gt;<span class="w"> </span>~/.profile
 <span class="nb">source</span><span class="w"> </span>~/.profile
 </code></pre></div>
 </div>
 </div>
 </div>
-<h2 id="installation-steps">Installation steps<a class="headerlink" href="#installation-steps" title="Permanent link">&para;</a></h2>
+<h2 id="install">Install<a class="headerlink" href="#install" title="Permanent link">&para;</a></h2>
 <p>Installation is a two-step process:</p>
 <ol>
 <li>Install the WeeWX application using pip.</li>
 <li>Provision a new station using the tool <code>weectl</code>.</li>
 </ol>
 <h3 id="step-1-install-the-application-using-pip">Step 1: Install the application using pip<a class="headerlink" href="#step-1-install-the-application-using-pip" title="Permanent link">&para;</a></h3>
-<p>Once the preparatory steps are out of the way, you're ready to install WeeWX using pip.</p>
+<p>Once the preparatory steps are out of the way, you're ready to install WeeWX
+using pip.</p>
 <p>There are many ways to do this (see the wiki document <a href="https://github.com/weewx/weewx/wiki/pip-install-strategies">pip
 install strategies</a>
 for a partial list), but the method below is one of the simplest and safest.</p>
 <div class="admonition note">
 <p class="admonition-title">Note</p>
-<p>While not strictly necessary, it's a good idea to invoke pip using <code>python3 -m pip</code>, rather 
-than simply <code>pip</code>. This way you can be sure which version of Python is being used.</p>
+<p>While not strictly necessary, it's a good idea to invoke pip using
+<code>python3 -m pip</code>, rather than simply <code>pip</code>. This way you can be sure which
+version of Python is being used.</p>
 </div>
 <div class="highlight"><pre><span></span><code>python3<span class="w"> </span>-m<span class="w"> </span>pip<span class="w"> </span>install<span class="w"> </span>weewx<span class="w"> </span>--user
 </code></pre></div>
-<p>When finished, the WeeWX executables will have been installed in <code>~/.local/bin</code>,
-and the libraries in your Python "user" area, generally <code>~/.local/lib/python3.x/site-packages/</code>,
-where <code>3.x</code> is your version of Python.</p>
+<p>When finished, the WeeWX executables will have been installed in
+<code>~/.local/bin</code>, and the libraries in your Python "user" area, generally
+<code>~/.local/lib/python3.x/site-packages/</code>, where <code>3.x</code> is your version of Python.</p>
 <div class="admonition note">
 <p class="admonition-title">Note</p>
 <p>You may get a warning to the effect:
-      <div class="highlight"><pre><span></span><code>WARNING: The script wheel is installed in &#39;/home/ubuntu/.local/bin&#39; which is not on PATH.
+<div class="highlight"><pre><span></span><code>WARNING: The script wheel is installed in &#39;/home/ubuntu/.local/bin&#39; which is not on PATH.
 Consider adding this directory to PATH or, if you prefer to suppress this warning, use --no-warn-script-location.
 </code></pre></div>
 If you do, log out, then log back in.</p>
 </div>
 <h3 id="step-2-provision-a-new-station">Step 2: Provision a new station<a class="headerlink" href="#step-2-provision-a-new-station" title="Permanent link">&para;</a></h3>
-<p>While the first step downloads everything into your local Python source tree, it
-does not set up the configuration specific to your station, nor does it set up the
-reporting skins. That is the job of the next step, which uses the tool <code>weectl</code>. </p>
+<p>While the first step downloads everything into your local Python source tree,
+it does not set up the configuration specific to your station, nor does it set
+up the reporting skins. That is the job of the next step, which uses the tool
+<code>weectl</code>. </p>
 <p>This step also does not require root privileges.</p>
 <div class="highlight"><pre><span></span><code>weectl<span class="w"> </span>station<span class="w"> </span>create
 </code></pre></div>
-<p>The tool will ask you a series of questions, then create a directory <code>~/weewx-data</code> in your home
-directory with a new configuration file. It will also install skins, documentation, utilitiy files,
-and examples in the same directory. After running <code>weewxd</code>, the same directory will be used to hold
-the database file and any generated HTML pages. It plays a role similar to <code>/home/weewx</code> in older
-versions of WeeWX but, unlike <code>/home/weewx</code>, it does not hold any code.</p>
+<p>The tool will ask you a series of questions, then create a directory
+<code>~/weewx-data</code> in your home directory with a new configuration file. It will
+also install skins, documentation, utilitiy files, and examples in the same
+directory. After running <code>weewxd</code>, the same directory will be used to hold
+the database file and any generated HTML pages. It plays a role similar to
+<code>/home/weewx</code> in older versions of WeeWX but, unlike <code>/home/weewx</code>, it does
+not hold any code.</p>
 <p>If you already have a <code>/home/weewx</code> and wish to reuse it, see the <a href="../../upgrading.htm">Upgrading
 guide</a> and the <a href="../v5-upgrade/"><em>Migrating setup.py installs to Version 5</em></a>.</p>
-<h2 id="running-weewxd">Running <code>weewxd</code><a class="headerlink" href="#running-weewxd" title="Permanent link">&para;</a></h2>
+<h2 id="run-weewxd">Run <code>weewxd</code><a class="headerlink" href="#run-weewxd" title="Permanent link">&para;</a></h2>
 <h3 id="run-directly">Run directly<a class="headerlink" href="#run-directly" title="Permanent link">&para;</a></h3>
-<p>After the last step, the main program <code>weewxd</code> can be run directly like any
-other program:</p>
+<p>The main program <code>weewxd</code> can be run directly like any other program.  When
+you run weewx this way, it will print data to the screen, and weewx will stop
+when you log out.</p>
 <div class="highlight"><pre><span></span><code>weewxd
 </code></pre></div>
 <h3 id="run-as-a-daemon">Run as a daemon<a class="headerlink" href="#run-as-a-daemon" title="Permanent link">&para;</a></h3>
-<p>If you wish to run <code>weewxd</code> as a daemon, follow the following steps, depending
-on your operating system. These steps will require root privileges in order to
-install the required daemon file.</p>
-<div class="tabbed-set tabbed-alternate" data-tabs="2:5"><input checked="checked" id="__tabbed_2_1" name="__tabbed_2" type="radio" /><input id="__tabbed_2_2" name="__tabbed_2" type="radio" /><input id="__tabbed_2_3" name="__tabbed_2" type="radio" /><input id="__tabbed_2_4" name="__tabbed_2" type="radio" /><input id="__tabbed_2_5" name="__tabbed_2" type="radio" /><div class="tabbed-labels"><label for="__tabbed_2_1">Debian</label><label for="__tabbed_2_2">Very old Debian</label><label for="__tabbed_2_3">Redhat</label><label for="__tabbed_2_4">openSUSE Leap</label><label for="__tabbed_2_5">macOS</label></div>
+<p>To make <code>weewxd</code> start when the system is booted, run <code>weewxd</code> as a daemon.
+The steps to configure <code>weewxd</code> to run as a damone depend on your operating
+system, and require root privileges.</p>
+<div class="tabbed-set tabbed-alternate" data-tabs="2:3"><input checked="checked" id="__tabbed_2_1" name="__tabbed_2" type="radio" /><input id="__tabbed_2_2" name="__tabbed_2" type="radio" /><input id="__tabbed_2_3" name="__tabbed_2" type="radio" /><div class="tabbed-labels"><label for="__tabbed_2_1">Systems that use systemd (e.g., Debian, Redhat, SUSE)</label><label for="__tabbed_2_2">Systems that use SysV init (e.g., Slackware, Devuan, Puppy, DD-WRT)</label><label for="__tabbed_2_3">macOS</label></div>
 <div class="tabbed-content">
 <div class="tabbed-block">
 <div class="admonition note">
 <p class="admonition-title">Note</p>
-<p>The resulting daemon will be run using your username. If you prefer to use run as <code>root</code>,
-you will have to modify the file <code>/etc/systemd/system/weewx.service</code>.</p>
+<p>The resulting daemon will be run using your username. If you prefer to
+use run as <code>root</code>, you will have to modify the file
+<code>/etc/systemd/system/weewx.service</code>.</p>
 </div>
-<div class="highlight"><pre><span></span><code><span class="nb">cd</span><span class="w"> </span>~/weewx-data
-sudo<span class="w"> </span>cp<span class="w"> </span>util/systemd/weewx.service<span class="w"> </span>/etc/systemd/system
+<div class="highlight"><pre><span></span><code>sudo<span class="w"> </span>cp<span class="w"> </span>~/weewx-data/util/systemd/weewx.service<span class="w"> </span>/etc/systemd/system
 sudo<span class="w"> </span>systemctl<span class="w"> </span>daemon-reload
 sudo<span class="w"> </span>systemctl<span class="w"> </span><span class="nb">enable</span><span class="w"> </span>weewx
 sudo<span class="w"> </span>systemctl<span class="w"> </span>start<span class="w"> </span>weewx
 </code></pre></div>
 </div>
 <div class="tabbed-block">
 <div class="admonition note">
 <p class="admonition-title">Note</p>
-<p>The resulting daemon will be run using your username. If you prefer to use run as <code>root</code>,
-you will have to modify the file <code>/etc/init.d/weewx</code>.</p>
+<p>The resulting daemon will be run using your username. If you prefer to
+use run as <code>root</code>, you will have to modify the file
+<code>/etc/init.d/weewx</code>.</p>
 </div>
-<div class="highlight"><pre><span></span><code><span class="c1"># Use the old init.d method if your os is ancient</span>
-<span class="nb">cd</span><span class="w"> </span>~/weewx-data
-sudo<span class="w"> </span>cp<span class="w"> </span>util/init.d/weewx.debian<span class="w"> </span>/etc/init.d/weewx
+<div class="highlight"><pre><span></span><code>sudo<span class="w"> </span>cp<span class="w"> </span>~/weewx-data/util/init.d/weewx.debian<span class="w"> </span>/etc/init.d/weewx
 sudo<span class="w"> </span>chmod<span class="w"> </span>+x<span class="w"> </span>/etc/init.d/weewx
 sudo<span class="w"> </span>update-rc.d<span class="w"> </span>weewx<span class="w"> </span>defaults<span class="w"> </span><span class="m">98</span>
 sudo<span class="w"> </span>/etc/init.d/weewx<span class="w"> </span>start<span class="w">     </span>
 </code></pre></div>
 </div>
 <div class="tabbed-block">
-<div class="admonition note">
-<p class="admonition-title">Note</p>
-<p>The resulting daemon will be run using your username. If you prefer to use run as <code>root</code>,
-you will have to modify the file <code>/etc/systemd/system/weewx.service</code>.</p>
-</div>
-<div class="highlight"><pre><span></span><code><span class="c1"># If SELinux is enabled, you will need the following command first:</span>
-chcon<span class="w"> </span>-R<span class="w"> </span>--reference<span class="w"> </span>/bin/ls<span class="w"> </span>~/.local/bin
-
-<span class="c1"># Then proceed as normal:</span>
-<span class="nb">cd</span><span class="w"> </span>~/weewx-data
-sudo<span class="w"> </span>cp<span class="w"> </span>util/systemd/weewx.service<span class="w"> </span>/etc/systemd/system
-sudo<span class="w"> </span>systemctl<span class="w"> </span>daemon-reload
-sudo<span class="w"> </span>systemctl<span class="w"> </span><span class="nb">enable</span><span class="w"> </span>weewx
-sudo<span class="w"> </span>systemctl<span class="w"> </span>start<span class="w"> </span>weewx
-</code></pre></div>
-</div>
-<div class="tabbed-block">
-<div class="admonition note">
-<p class="admonition-title">Note</p>
-<p>The resulting daemon will be run using your username. If you prefer to use run as <code>root</code>,
-you will have to modify the file <code>/etc/systemd/system/weewx.service</code>.</p>
-</div>
-<div class="highlight"><pre><span></span><code><span class="nb">cd</span><span class="w"> </span>~/weewx-data
-sudo<span class="w"> </span>cp<span class="w"> </span>util/systemd/weewx.service<span class="w"> </span>/etc/systemd/system
-sudo<span class="w"> </span>systemctl<span class="w"> </span>daemon-reload
-sudo<span class="w"> </span>systemctl<span class="w"> </span><span class="nb">enable</span><span class="w"> </span>weewx
-sudo<span class="w"> </span>systemctl<span class="w"> </span>start<span class="w"> </span>weewx
-</code></pre></div>
-</div>
-<div class="tabbed-block">
-<div class="highlight"><pre><span></span><code><span class="nb">cd</span><span class="w"> </span>~/weewx-data
-sudo<span class="w"> </span>cp<span class="w"> </span>util/launchd/com.weewx.weewxd.plist<span class="w"> </span>/Library/LaunchDaemons
+<div class="highlight"><pre><span></span><code>sudo<span class="w"> </span>cp<span class="w"> </span>~/weewx-data/util/launchd/com.weewx.weewxd.plist<span class="w"> </span>/Library/LaunchDaemons
 sudo<span class="w"> </span>launchctl<span class="w"> </span>load<span class="w"> </span>/Library/LaunchDaemons/com.weewx.weewxd.plist
 </code></pre></div>
 </div>
 </div>
 </div>
-<h3 id="verify">Verify<a class="headerlink" href="#verify" title="Permanent link">&para;</a></h3>
-<p>After about 5 minutes (the exact length of time depends on your archive interval), cut and
-paste the following into your web browser:</p>
+<h2 id="verify">Verify<a class="headerlink" href="#verify" title="Permanent link">&para;</a></h2>
+<p>After about 5 minutes (the exact length of time depends on your archive
+interval), copy the following and paste into a web browser:</p>
 <div class="highlight"><pre><span></span><code>~/weewx-data/public_html/index.html
 </code></pre></div>
 <p>You should see your station information and data.</p>
 <p>You may also want to check your system log for any problems.</p>
 <h2 id="configure">Configure<a class="headerlink" href="#configure" title="Permanent link">&para;</a></h2>
 <p>If you chose the simulator as your station type, then at some point you will
 probably want to switch to using real hardware. Here's how to reconfigure.</p>
-<div class="tabbed-set tabbed-alternate" data-tabs="3:3"><input checked="checked" id="__tabbed_3_1" name="__tabbed_3" type="radio" /><input id="__tabbed_3_2" name="__tabbed_3" type="radio" /><input id="__tabbed_3_3" name="__tabbed_3" type="radio" /><div class="tabbed-labels"><label for="__tabbed_3_1">Debian/Redhat/openSUSE</label><label for="__tabbed_3_2">Very old Debian</label><label for="__tabbed_3_3">macOS</label></div>
+<div class="tabbed-set tabbed-alternate" data-tabs="3:3"><input checked="checked" id="__tabbed_3_1" name="__tabbed_3" type="radio" /><input id="__tabbed_3_2" name="__tabbed_3" type="radio" /><input id="__tabbed_3_3" name="__tabbed_3" type="radio" /><div class="tabbed-labels"><label for="__tabbed_3_1">Systems that use systemd (e.g., Debian, Redhat, SUSE)</label><label for="__tabbed_3_2">Systems that use SysV init (e.g., Slackware, Devuan, Puppy, DD-WRT)</label><label for="__tabbed_3_3">macOS</label></div>
 <div class="tabbed-content">
 <div class="tabbed-block">
-<div class="highlight"><pre><span></span><code>sudo<span class="w"> </span>systemctl<span class="w"> </span>stop
+<div class="highlight"><pre><span></span><code><span class="c1"># Stop the weewx daemon:</span>
+sudo<span class="w"> </span>systemctl<span class="w"> </span>stop<span class="w"> </span>weewx
 <span class="c1"># Reconfigure to use your hardware:</span>
 weectl<span class="w"> </span>station<span class="w"> </span>reconfigure
 <span class="c1"># Remove the old database:</span>
 rm<span class="w"> </span>~/weewx-data/archive/weewx.sdb
-<span class="c1"># Restart:</span>
-sudo<span class="w"> </span>systemctl<span class="w"> </span>start
+<span class="c1"># Start the weewx daemon:</span>
+sudo<span class="w"> </span>systemctl<span class="w"> </span>start<span class="w"> </span>weewx
 </code></pre></div>
 </div>
 <div class="tabbed-block">
-<div class="highlight"><pre><span></span><code>sudo<span class="w"> </span>/etc/init.d/weewx<span class="w"> </span>stop
+<div class="highlight"><pre><span></span><code><span class="c1"># Stop the weewx daemon:</span>
+sudo<span class="w"> </span>/etc/init.d/weewx<span class="w"> </span>stop
 <span class="c1"># Reconfigure to use your hardware:</span>
 weectl<span class="w"> </span>station<span class="w"> </span>reconfigure
 <span class="c1"># Remove the old database:</span>
 rm<span class="w"> </span>~/weewx-data/archive/weewx.sdb
-<span class="c1"># Restart:</span>
+<span class="c1"># Start the weewx daemon:</span>
 sudo<span class="w"> </span>/etc/init.d/weewx<span class="w"> </span>start
 </code></pre></div>
 </div>
 <div class="tabbed-block">
 <div class="highlight"><pre><span></span><code>sudo<span class="w"> </span>launchctl<span class="w"> </span>unload<span class="w"> </span>/Library/LaunchDaemons/com.weewx.weewxd.plist
 <span class="c1"># Reconfigure to use your hardware:</span>
 weectl<span class="w"> </span>station<span class="w"> </span>reconfigure
@@ -1866,40 +1845,42 @@
 </div>
 </div>
 <h2 id="customize">Customize<a class="headerlink" href="#customize" title="Permanent link">&para;</a></h2>
 <p>To enable uploads, such as Weather Underground, or to customize reports, modify
 the configuration file <code>~/weewx-data/weewx.conf</code>. See the <a href="../usersguide"><em>User
 Guide</em></a> and <a href="../custom"><em>Customization Guide</em></a> for details.</p>
 <h2 id="uninstall">Uninstall<a class="headerlink" href="#uninstall" title="Permanent link">&para;</a></h2>
-<p>Stop, disable, and remove any daemon files:</p>
-<div class="tabbed-set tabbed-alternate" data-tabs="4:3"><input checked="checked" id="__tabbed_4_1" name="__tabbed_4" type="radio" /><input id="__tabbed_4_2" name="__tabbed_4" type="radio" /><input id="__tabbed_4_3" name="__tabbed_4" type="radio" /><div class="tabbed-labels"><label for="__tabbed_4_1">Debian/Redhat/openSUSE</label><label for="__tabbed_4_2">Very old Debian</label><label for="__tabbed_4_3">macOS</label></div>
+<p>Before you uninstall, be sure that <code>weewxd</code> is not running.  Then remove the
+daemon configuration.</p>
+<div class="tabbed-set tabbed-alternate" data-tabs="4:3"><input checked="checked" id="__tabbed_4_1" name="__tabbed_4" type="radio" /><input id="__tabbed_4_2" name="__tabbed_4" type="radio" /><input id="__tabbed_4_3" name="__tabbed_4" type="radio" /><div class="tabbed-labels"><label for="__tabbed_4_1">Systems that use systemd (e.g., Debian, Redhat, SUSE)</label><label for="__tabbed_4_2">Systems that use SysV init (e.g., Slackware, Devuan, Puppy, DD-WRT)</label><label for="__tabbed_4_3">macOS</label></div>
 <div class="tabbed-content">
 <div class="tabbed-block">
 <div class="highlight"><pre><span></span><code>sudo<span class="w"> </span>systemctl<span class="w"> </span>stop<span class="w"> </span>weewx
 sudo<span class="w"> </span>systemctl<span class="w"> </span>disable<span class="w"> </span>weewx
 sudo<span class="w"> </span>rm<span class="w"> </span>/etc/systemd/system/weewx.service
 </code></pre></div>
 </div>
 <div class="tabbed-block">
 <div class="highlight"><pre><span></span><code>sudo<span class="w"> </span>/etc/rc.d/init.d/weewx<span class="w"> </span>stop
+sudo<span class="w"> </span>update-rc.d<span class="w"> </span>weewx<span class="w"> </span>remove
 sudo<span class="w"> </span>rm<span class="w"> </span>/etc/init.d/weewx
 </code></pre></div>
 </div>
 <div class="tabbed-block">
 <div class="highlight"><pre><span></span><code>sudo<span class="w"> </span>launchctl<span class="w"> </span>unload<span class="w"> </span>/Library/LaunchDaemons/com.weewx.weewxd.plist
 sudo<span class="w"> </span>rm<span class="w"> </span>/Library/LaunchDaemons/com.weewx.weewxd.plist
 </code></pre></div>
 </div>
 </div>
 </div>
-<p>Use pip to uninstall the program.</p>
+<p>Use pip to uninstall weewx.</p>
 <div class="highlight"><pre><span></span><code>python3<span class="w"> </span>-m<span class="w"> </span>pip<span class="w"> </span>uninstall<span class="w"> </span>weewx<span class="w"> </span>-y
 </code></pre></div>
-<p>You can also use pip to uninstall the dependencies, but first check that they are
-not being used by other programs!</p>
+<p>You can also use pip to uninstall the dependencies, but first check that they
+are not being used by other programs!</p>
 <div class="highlight"><pre><span></span><code>python3<span class="w"> </span>-m<span class="w"> </span>pip<span class="w"> </span>uninstall<span class="w"> </span>pyserial<span class="w"> </span>pyusb<span class="w"> </span>CT3<span class="w"> </span>Pillow<span class="w"> </span>configobj<span class="w"> </span>PyMySQL<span class="w"> </span>pyephem<span class="w"> </span>ephem<span class="w"> </span>-y
 </code></pre></div>
 <p>Finally, if desired, delete the data directory:</p>
 <div class="highlight"><pre><span></span><code>rm<span class="w"> </span>-r<span class="w"> </span>~/weewx-data
 </code></pre></div>
```

#### html2text {}

```diff
@@ -26,22 +26,22 @@
     * *
       Quick_starts
          Quick starts
           o Debian
           o RedHat
           o SuSE
           o ⁰  pip   pip    Table of contents
-                # Preparation
-                # Installation_steps
+                # Prepare_for_install
+                # Install
                       # Step_1:_Install_the_application_using_pip
                       # Step_2:_Provision_a_new_station
-                # Running_weewxd
+                # Run_weewxd
                       # Run_directly
                       # Run_as_a_daemon
-                      # Verify
+                # Verify
                 # Configure
                 # Customize
                 # Uninstall
           o Migrating_to_V5
     * ⁰
       User's_guide
          User's guide
@@ -103,65 +103,66 @@
     * Upgrade_guide
     * Hardware_guide
     * Notes_for_developers
     * Hardware_comparison
     * Change_log
     * Support
    Table of contents
-    * Preparation
-    * Installation_steps
+    * Prepare_for_install
+    * Install
           o Step_1:_Install_the_application_using_pip
           o Step_2:_Provision_a_new_station
-    * Running_weewxd
+    * Run_weewxd
           o Run_directly
           o Run_as_a_daemon
-          o Verify
+    * Verify
     * Configure
     * Customize
     * Uninstall
 ****** Installation using pip¶ ******
 This is a guide to installing WeeWX using pip. It can be used to install WeeWX
 on almost any operating system, including macOS.
-***** Preparation¶ *****
+***** Prepare for install¶ *****
     * WeeWX V5.x requires Python 3.7 or greater. It cannot be run with Python
       2.x. If you are constrained by this, install WeeWX V4.10, the last
       version to support Python 2.7, Python 3.5, and Python 3.6.
     * You must also have a copy of pip. In most cases, your operating system
       will offer an installation_package. Otherwise, see_the_directions_on_the
       pip_website.
     * While you will not need root privileges to install and configure WeeWX,
       you will need them to set up a daemon and, perhaps, to change device
       permissions.
-Depending on your operating system and how complete it is, you may have to
-install some tools before beginning. Follow the directions below for your
-system:
+Depending on your operating system and what has already been installed, you may
+have to install some tools before beginning. Follow the directions below for
+your system:
 #oo
 DebianRedhatopenSUSE Leap
 sudo apt update && sudo apt upgrade
 sudo apt -y install gcc
 sudo apt -y install python3-dev
 # This makes the install of pyephem go more smoothly:
 python3 -m pip install wheel
 sudo yum update
 sudo yum install -y gcc
 sudo yum install -y python3-devel
 # This makes the install of pyephem go more smoothly:
 python3 -m pip install wheel
 # Check to see what version of Python you have:
 python3 -V
-# If it is less than Python 3.7, you will have to upgrade to a
-# later version. The following installs 3.9. Afterwards, you must
-# invoke Python by using "python3.9", NOT "python3"
+
+# If it is less than Python 3.7, you will have to upgrade to a later
+# version. The following installs 3.9. Afterwards, you must invoke Python
+# by using "python3.9", NOT "python3"
 sudo zypper install -y python39 python39-devel
 python3.9 -m pip install wheel
 
 # Finally, you may have to add ~/.local/bin to your path:
 echo 'export PATH="$PATH:$HOME/.local/bin"' >> ~/.profile
 source ~/.profile
-***** Installation steps¶ *****
+***** Install¶ *****
 Installation is a two-step process:
    1. Install the WeeWX application using pip.
    2. Provision a new station using the tool weectl.
 **** Step 1: Install the application using pip¶ ****
 Once the preparatory steps are out of the way, you're ready to install WeeWX
 using pip.
 There are many ways to do this (see the wiki document pip_install_strategies
@@ -192,113 +193,97 @@
 data in your home directory with a new configuration file. It will also install
 skins, documentation, utilitiy files, and examples in the same directory. After
 running weewxd, the same directory will be used to hold the database file and
 any generated HTML pages. It plays a role similar to /home/weewx in older
 versions of WeeWX but, unlike /home/weewx, it does not hold any code.
 If you already have a /home/weewx and wish to reuse it, see the Upgrading_guide
 and the Migrating_setup.py_installs_to_Version_5.
-***** Running weewxd¶ *****
+***** Run weewxd¶ *****
 **** Run directly¶ ****
-After the last step, the main program weewxd can be run directly like any other
-program:
+The main program weewxd can be run directly like any other program. When you
+run weewx this way, it will print data to the screen, and weewx will stop when
+you log out.
 weewxd
 **** Run as a daemon¶ ****
-If you wish to run weewxd as a daemon, follow the following steps, depending on
-your operating system. These steps will require root privileges in order to
-install the required daemon file.
-#oooo
-DebianVery old DebianRedhatopenSUSE LeapmacOS
+To make weewxd start when the system is booted, run weewxd as a daemon. The
+steps to configure weewxd to run as a damone depend on your operating system,
+and require root privileges.
+#oo
+Systems that use systemd (e.g., Debian, Redhat, SUSE)Systems that use SysV init
+(e.g., Slackware, Devuan, Puppy, DD-WRT)macOS
 Note
 The resulting daemon will be run using your username. If you prefer to use run
 as root, you will have to modify the file /etc/systemd/system/weewx.service.
-cd ~/weewx-data
-sudo cp util/systemd/weewx.service /etc/systemd/system
+sudo cp ~/weewx-data/util/systemd/weewx.service /etc/systemd/system
 sudo systemctl daemon-reload
 sudo systemctl enable weewx
 sudo systemctl start weewx
 Note
 The resulting daemon will be run using your username. If you prefer to use run
 as root, you will have to modify the file /etc/init.d/weewx.
-# Use the old init.d method if your os is ancient
-cd ~/weewx-data
-sudo cp util/init.d/weewx.debian /etc/init.d/weewx
+sudo cp ~/weewx-data/util/init.d/weewx.debian /etc/init.d/weewx
 sudo chmod +x /etc/init.d/weewx
 sudo update-rc.d weewx defaults 98
 sudo /etc/init.d/weewx start
-Note
-The resulting daemon will be run using your username. If you prefer to use run
-as root, you will have to modify the file /etc/systemd/system/weewx.service.
-# If SELinux is enabled, you will need the following command first:
-chcon -R --reference /bin/ls ~/.local/bin
-
-# Then proceed as normal:
-cd ~/weewx-data
-sudo cp util/systemd/weewx.service /etc/systemd/system
-sudo systemctl daemon-reload
-sudo systemctl enable weewx
-sudo systemctl start weewx
-Note
-The resulting daemon will be run using your username. If you prefer to use run
-as root, you will have to modify the file /etc/systemd/system/weewx.service.
-cd ~/weewx-data
-sudo cp util/systemd/weewx.service /etc/systemd/system
-sudo systemctl daemon-reload
-sudo systemctl enable weewx
-sudo systemctl start weewx
-cd ~/weewx-data
-sudo cp util/launchd/com.weewx.weewxd.plist /Library/LaunchDaemons
+sudo cp ~/weewx-data/util/launchd/com.weewx.weewxd.plist /Library/LaunchDaemons
 sudo launchctl load /Library/LaunchDaemons/com.weewx.weewxd.plist
-**** Verify¶ ****
+***** Verify¶ *****
 After about 5 minutes (the exact length of time depends on your archive
-interval), cut and paste the following into your web browser:
+interval), copy the following and paste into a web browser:
 ~/weewx-data/public_html/index.html
 You should see your station information and data.
 You may also want to check your system log for any problems.
 ***** Configure¶ *****
 If you chose the simulator as your station type, then at some point you will
 probably want to switch to using real hardware. Here's how to reconfigure.
 #oo
-Debian/Redhat/openSUSEVery old DebianmacOS
-sudo systemctl stop
+Systems that use systemd (e.g., Debian, Redhat, SUSE)Systems that use SysV init
+(e.g., Slackware, Devuan, Puppy, DD-WRT)macOS
+# Stop the weewx daemon:
+sudo systemctl stop weewx
 # Reconfigure to use your hardware:
 weectl station reconfigure
 # Remove the old database:
 rm ~/weewx-data/archive/weewx.sdb
-# Restart:
-sudo systemctl start
+# Start the weewx daemon:
+sudo systemctl start weewx
+# Stop the weewx daemon:
 sudo /etc/init.d/weewx stop
 # Reconfigure to use your hardware:
 weectl station reconfigure
 # Remove the old database:
 rm ~/weewx-data/archive/weewx.sdb
-# Restart:
+# Start the weewx daemon:
 sudo /etc/init.d/weewx start
 sudo launchctl unload /Library/LaunchDaemons/com.weewx.weewxd.plist
 # Reconfigure to use your hardware:
 weectl station reconfigure
 # Remove the old database:
 rm ~/weewx-data/archive/weewx.sdb
 # Restart:
 sudo launchctl load /Library/LaunchDaemons/com.weewx.weewxd.plist
 ***** Customize¶ *****
 To enable uploads, such as Weather Underground, or to customize reports, modify
 the configuration file ~/weewx-data/weewx.conf. See the User_Guide and
 Customization_Guide for details.
 ***** Uninstall¶ *****
-Stop, disable, and remove any daemon files:
+Before you uninstall, be sure that weewxd is not running. Then remove the
+daemon configuration.
 #oo
-Debian/Redhat/openSUSEVery old DebianmacOS
+Systems that use systemd (e.g., Debian, Redhat, SUSE)Systems that use SysV init
+(e.g., Slackware, Devuan, Puppy, DD-WRT)macOS
 sudo systemctl stop weewx
 sudo systemctl disable weewx
 sudo rm /etc/systemd/system/weewx.service
 sudo /etc/rc.d/init.d/weewx stop
+sudo update-rc.d weewx remove
 sudo rm /etc/init.d/weewx
 sudo launchctl unload /Library/LaunchDaemons/com.weewx.weewxd.plist
 sudo rm /Library/LaunchDaemons/com.weewx.weewxd.plist
-Use pip to uninstall the program.
+Use pip to uninstall weewx.
 python3 -m pip uninstall weewx -y
 You can also use pip to uninstall the dependencies, but first check that they
 are not being used by other programs!
 python3 -m pip uninstall pyserial pyusb CT3 Pillow configobj PyMySQL pyephem
 ephem -y
 Finally, if desired, delete the data directory:
 rm -r ~/weewx-data
```

### Comparing `weewx-5.0.0a30/bin/wee_resources/docs/quickstarts/redhat/index.html` & `weewx-5.0.0b1/bin/wee_resources/docs/quickstarts/redhat/index.html`

 * *Files identical despite different names*

### Comparing `weewx-5.0.0a30/bin/wee_resources/docs/quickstarts/suse/index.html` & `weewx-5.0.0b1/bin/wee_resources/docs/quickstarts/suse/index.html`

 * *Files identical despite different names*

### Comparing `weewx-5.0.0a30/bin/wee_resources/docs/quickstarts/v5-upgrade/index.html` & `weewx-5.0.0b1/bin/wee_resources/docs/quickstarts/v5-upgrade/index.html`

 * *Files identical despite different names*

### Comparing `weewx-5.0.0a30/bin/wee_resources/docs/report_scheduling/index.html` & `weewx-5.0.0b1/bin/wee_resources/docs/report_scheduling/index.html`

 * *Files identical despite different names*

### Comparing `weewx-5.0.0a30/bin/wee_resources/docs/search/search_index.json` & `weewx-5.0.0b1/bin/wee_resources/docs/search/search_index.json`

 * *Files 0% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9993402354851806%*

 * *Differences: {"'docs'": "{428: {'location': 'quickstarts/pip/#prepare-for-install', 'title': 'Prepare for "*

 * *           "install', 'text': '<ul> <li> <p>WeeWX V5.x requires Python 3.7 or greater. It cannot "*

 * *           'be run with Python 2.x.   If you are constrained by this, install WeeWX V4.10, the '*

 * *           'last version to   support Python 2.7, Python 3.5, and Python 3.6.</p> </li> <li> '*

 * *           '<p>You must also have a copy of pip. In most cases, your operating system will   offer '*

 * *           'an installati […]*

```diff
@@ -2146,66 +2146,66 @@
         },
         {
             "location": "quickstarts/pip/",
             "text": "<p>This is a guide to installing WeeWX using pip. It can be used to install WeeWX on almost any operating system, including macOS.</p>",
             "title": "Installation using pip"
         },
         {
-            "location": "quickstarts/pip/#preparation",
-            "text": "<ul> <li> <p>WeeWX V5.x requires Python 3.7 or greater. It cannot be run with Python 2.x.  If you are constrained by this, install WeeWX V4.10, the   last version to support Python 2.7, Python 3.5, and Python 3.6.</p> </li> <li> <p>You must also have a copy of pip. In most cases, your operating system will offer an   installation package.   Otherwise, see the directions on the pip website.</p> </li> <li> <p>While you will not need root privileges to install and configure WeeWX,   you will need them to set up a daemon and, perhaps, to change device permissions.</p> </li> </ul> <p>Depending on your operating system and how complete it is, you may have to install some tools before beginning. Follow the directions below for your system:</p> DebianRedhatopenSUSE Leap <pre><code>sudo apt update &amp;&amp; sudo apt upgrade\nsudo apt -y install gcc\nsudo apt -y install python3-dev\n# This makes the install of pyephem go more smoothly:\npython3 -m pip install wheel\n</code></pre> <pre><code>sudo yum update\nsudo yum install -y gcc\nsudo yum install -y python3-devel\n# This makes the install of pyephem go more smoothly:\npython3 -m pip install wheel\n</code></pre> <pre><code># Check to see what version of Python you have:\npython3 -V\n# If it is less than Python 3.7, you will have to upgrade to a \n# later version. The following installs 3.9. Afterwards, you must\n# invoke Python by using \"python3.9\", NOT \"python3\"\nsudo zypper install -y python39 python39-devel\npython3.9 -m pip install wheel\n\n# Finally, you may have to add ~/.local/bin to your path:\necho 'export PATH=\"$PATH:$HOME/.local/bin\"' &gt;&gt; ~/.profile\nsource ~/.profile\n</code></pre>",
-            "title": "Preparation"
+            "location": "quickstarts/pip/#prepare-for-install",
+            "text": "<ul> <li> <p>WeeWX V5.x requires Python 3.7 or greater. It cannot be run with Python 2.x.   If you are constrained by this, install WeeWX V4.10, the last version to   support Python 2.7, Python 3.5, and Python 3.6.</p> </li> <li> <p>You must also have a copy of pip. In most cases, your operating system will   offer an installation package.   Otherwise, see the directions on the pip website.</p> </li> <li> <p>While you will not need root privileges to install and configure WeeWX, you   will need them to set up a daemon and, perhaps, to change device permissions.</p> </li> </ul> <p>Depending on your operating system and what has already been installed, you may have to install some tools before beginning. Follow the directions below for your system:</p> DebianRedhatopenSUSE Leap <pre><code>sudo apt update &amp;&amp; sudo apt upgrade\nsudo apt -y install gcc\nsudo apt -y install python3-dev\n# This makes the install of pyephem go more smoothly:\npython3 -m pip install wheel\n</code></pre> <pre><code>sudo yum update\nsudo yum install -y gcc\nsudo yum install -y python3-devel\n# This makes the install of pyephem go more smoothly:\npython3 -m pip install wheel\n</code></pre> <pre><code># Check to see what version of Python you have:\npython3 -V\n\n# If it is less than Python 3.7, you will have to upgrade to a later\n# version. The following installs 3.9. Afterwards, you must invoke Python\n# by using \"python3.9\", NOT \"python3\"\nsudo zypper install -y python39 python39-devel\npython3.9 -m pip install wheel\n\n# Finally, you may have to add ~/.local/bin to your path:\necho 'export PATH=\"$PATH:$HOME/.local/bin\"' &gt;&gt; ~/.profile\nsource ~/.profile\n</code></pre>",
+            "title": "Prepare for install"
         },
         {
-            "location": "quickstarts/pip/#installation-steps",
+            "location": "quickstarts/pip/#install",
             "text": "<p>Installation is a two-step process:</p> <ol> <li>Install the WeeWX application using pip.</li> <li>Provision a new station using the tool <code>weectl</code>.</li> </ol>",
-            "title": "Installation steps"
+            "title": "Install"
         },
         {
             "location": "quickstarts/pip/#step-1-install-the-application-using-pip",
-            "text": "<p>Once the preparatory steps are out of the way, you're ready to install WeeWX using pip.</p> <p>There are many ways to do this (see the wiki document pip install strategies for a partial list), but the method below is one of the simplest and safest.</p> <p>Note</p> <p>While not strictly necessary, it's a good idea to invoke pip using <code>python3 -m pip</code>, rather  than simply <code>pip</code>. This way you can be sure which version of Python is being used.</p> <pre><code>python3 -m pip install weewx --user\n</code></pre> <p>When finished, the WeeWX executables will have been installed in <code>~/.local/bin</code>, and the libraries in your Python \"user\" area, generally <code>~/.local/lib/python3.x/site-packages/</code>, where <code>3.x</code> is your version of Python.</p> <p>Note</p> <p>You may get a warning to the effect:       <pre><code>WARNING: The script wheel is installed in '/home/ubuntu/.local/bin' which is not on PATH.\nConsider adding this directory to PATH or, if you prefer to suppress this warning, use --no-warn-script-location.\n</code></pre> If you do, log out, then log back in.</p>",
+            "text": "<p>Once the preparatory steps are out of the way, you're ready to install WeeWX using pip.</p> <p>There are many ways to do this (see the wiki document pip install strategies for a partial list), but the method below is one of the simplest and safest.</p> <p>Note</p> <p>While not strictly necessary, it's a good idea to invoke pip using <code>python3 -m pip</code>, rather than simply <code>pip</code>. This way you can be sure which version of Python is being used.</p> <pre><code>python3 -m pip install weewx --user\n</code></pre> <p>When finished, the WeeWX executables will have been installed in <code>~/.local/bin</code>, and the libraries in your Python \"user\" area, generally <code>~/.local/lib/python3.x/site-packages/</code>, where <code>3.x</code> is your version of Python.</p> <p>Note</p> <p>You may get a warning to the effect: <pre><code>WARNING: The script wheel is installed in '/home/ubuntu/.local/bin' which is not on PATH.\nConsider adding this directory to PATH or, if you prefer to suppress this warning, use --no-warn-script-location.\n</code></pre> If you do, log out, then log back in.</p>",
             "title": "Step 1: Install the application using pip"
         },
         {
             "location": "quickstarts/pip/#step-2-provision-a-new-station",
             "text": "<p>While the first step downloads everything into your local Python source tree, it does not set up the configuration specific to your station, nor does it set up the reporting skins. That is the job of the next step, which uses the tool <code>weectl</code>. </p> <p>This step also does not require root privileges.</p> <pre><code>weectl station create\n</code></pre> <p>The tool will ask you a series of questions, then create a directory <code>~/weewx-data</code> in your home directory with a new configuration file. It will also install skins, documentation, utilitiy files, and examples in the same directory. After running <code>weewxd</code>, the same directory will be used to hold the database file and any generated HTML pages. It plays a role similar to <code>/home/weewx</code> in older versions of WeeWX but, unlike <code>/home/weewx</code>, it does not hold any code.</p> <p>If you already have a <code>/home/weewx</code> and wish to reuse it, see the Upgrading guide and the Migrating setup.py installs to Version 5.</p>",
             "title": "Step 2: Provision a new station"
         },
         {
-            "location": "quickstarts/pip/#running-weewxd",
+            "location": "quickstarts/pip/#run-weewxd",
             "text": "",
-            "title": "Running <code>weewxd</code>"
+            "title": "Run <code>weewxd</code>"
         },
         {
             "location": "quickstarts/pip/#run-directly",
-            "text": "<p>After the last step, the main program <code>weewxd</code> can be run directly like any other program:</p> <pre><code>weewxd\n</code></pre>",
+            "text": "<p>The main program <code>weewxd</code> can be run directly like any other program.  When you run weewx this way, it will print data to the screen, and weewx will stop when you log out.</p> <pre><code>weewxd\n</code></pre>",
             "title": "Run directly"
         },
         {
             "location": "quickstarts/pip/#run-as-a-daemon",
-            "text": "<p>If you wish to run <code>weewxd</code> as a daemon, follow the following steps, depending on your operating system. These steps will require root privileges in order to install the required daemon file.</p> DebianVery old DebianRedhatopenSUSE LeapmacOS <p>Note</p> <p>The resulting daemon will be run using your username. If you prefer to use run as <code>root</code>, you will have to modify the file <code>/etc/systemd/system/weewx.service</code>.</p> <pre><code>cd ~/weewx-data\nsudo cp util/systemd/weewx.service /etc/systemd/system\nsudo systemctl daemon-reload\nsudo systemctl enable weewx\nsudo systemctl start weewx\n</code></pre> <p>Note</p> <p>The resulting daemon will be run using your username. If you prefer to use run as <code>root</code>, you will have to modify the file <code>/etc/init.d/weewx</code>.</p> <pre><code># Use the old init.d method if your os is ancient\ncd ~/weewx-data\nsudo cp util/init.d/weewx.debian /etc/init.d/weewx\nsudo chmod +x /etc/init.d/weewx\nsudo update-rc.d weewx defaults 98\nsudo /etc/init.d/weewx start     </code></pre> <p>Note</p> <p>The resulting daemon will be run using your username. If you prefer to use run as <code>root</code>, you will have to modify the file <code>/etc/systemd/system/weewx.service</code>.</p> <pre><code># If SELinux is enabled, you will need the following command first:\nchcon -R --reference /bin/ls ~/.local/bin\n\n# Then proceed as normal:\ncd ~/weewx-data\nsudo cp util/systemd/weewx.service /etc/systemd/system\nsudo systemctl daemon-reload\nsudo systemctl enable weewx\nsudo systemctl start weewx\n</code></pre> <p>Note</p> <p>The resulting daemon will be run using your username. If you prefer to use run as <code>root</code>, you will have to modify the file <code>/etc/systemd/system/weewx.service</code>.</p> <pre><code>cd ~/weewx-data\nsudo cp util/systemd/weewx.service /etc/systemd/system\nsudo systemctl daemon-reload\nsudo systemctl enable weewx\nsudo systemctl start weewx\n</code></pre> <pre><code>cd ~/weewx-data\nsudo cp util/launchd/com.weewx.weewxd.plist /Library/LaunchDaemons\nsudo launchctl load /Library/LaunchDaemons/com.weewx.weewxd.plist\n</code></pre>",
+            "text": "<p>To make <code>weewxd</code> start when the system is booted, run <code>weewxd</code> as a daemon. The steps to configure <code>weewxd</code> to run as a damone depend on your operating system, and require root privileges.</p> Systems that use systemd (e.g., Debian, Redhat, SUSE)Systems that use SysV init (e.g., Slackware, Devuan, Puppy, DD-WRT)macOS <p>Note</p> <p>The resulting daemon will be run using your username. If you prefer to use run as <code>root</code>, you will have to modify the file <code>/etc/systemd/system/weewx.service</code>.</p> <pre><code>sudo cp ~/weewx-data/util/systemd/weewx.service /etc/systemd/system\nsudo systemctl daemon-reload\nsudo systemctl enable weewx\nsudo systemctl start weewx\n</code></pre> <p>Note</p> <p>The resulting daemon will be run using your username. If you prefer to use run as <code>root</code>, you will have to modify the file <code>/etc/init.d/weewx</code>.</p> <pre><code>sudo cp ~/weewx-data/util/init.d/weewx.debian /etc/init.d/weewx\nsudo chmod +x /etc/init.d/weewx\nsudo update-rc.d weewx defaults 98\nsudo /etc/init.d/weewx start     </code></pre> <pre><code>sudo cp ~/weewx-data/util/launchd/com.weewx.weewxd.plist /Library/LaunchDaemons\nsudo launchctl load /Library/LaunchDaemons/com.weewx.weewxd.plist\n</code></pre>",
             "title": "Run as a daemon"
         },
         {
             "location": "quickstarts/pip/#verify",
-            "text": "<p>After about 5 minutes (the exact length of time depends on your archive interval), cut and paste the following into your web browser:</p> <pre><code>~/weewx-data/public_html/index.html\n</code></pre> <p>You should see your station information and data.</p> <p>You may also want to check your system log for any problems.</p>",
+            "text": "<p>After about 5 minutes (the exact length of time depends on your archive interval), copy the following and paste into a web browser:</p> <pre><code>~/weewx-data/public_html/index.html\n</code></pre> <p>You should see your station information and data.</p> <p>You may also want to check your system log for any problems.</p>",
             "title": "Verify"
         },
         {
             "location": "quickstarts/pip/#configure",
-            "text": "<p>If you chose the simulator as your station type, then at some point you will probably want to switch to using real hardware. Here's how to reconfigure.</p> Debian/Redhat/openSUSEVery old DebianmacOS <pre><code>sudo systemctl stop\n# Reconfigure to use your hardware:\nweectl station reconfigure\n# Remove the old database:\nrm ~/weewx-data/archive/weewx.sdb\n# Restart:\nsudo systemctl start\n</code></pre> <pre><code>sudo /etc/init.d/weewx stop\n# Reconfigure to use your hardware:\nweectl station reconfigure\n# Remove the old database:\nrm ~/weewx-data/archive/weewx.sdb\n# Restart:\nsudo /etc/init.d/weewx start\n</code></pre> <pre><code>sudo launchctl unload /Library/LaunchDaemons/com.weewx.weewxd.plist\n# Reconfigure to use your hardware:\nweectl station reconfigure\n# Remove the old database:\nrm ~/weewx-data/archive/weewx.sdb\n# Restart:\nsudo launchctl load /Library/LaunchDaemons/com.weewx.weewxd.plist\n</code></pre>",
+            "text": "<p>If you chose the simulator as your station type, then at some point you will probably want to switch to using real hardware. Here's how to reconfigure.</p> Systems that use systemd (e.g., Debian, Redhat, SUSE)Systems that use SysV init (e.g., Slackware, Devuan, Puppy, DD-WRT)macOS <pre><code># Stop the weewx daemon:\nsudo systemctl stop weewx\n# Reconfigure to use your hardware:\nweectl station reconfigure\n# Remove the old database:\nrm ~/weewx-data/archive/weewx.sdb\n# Start the weewx daemon:\nsudo systemctl start weewx\n</code></pre> <pre><code># Stop the weewx daemon:\nsudo /etc/init.d/weewx stop\n# Reconfigure to use your hardware:\nweectl station reconfigure\n# Remove the old database:\nrm ~/weewx-data/archive/weewx.sdb\n# Start the weewx daemon:\nsudo /etc/init.d/weewx start\n</code></pre> <pre><code>sudo launchctl unload /Library/LaunchDaemons/com.weewx.weewxd.plist\n# Reconfigure to use your hardware:\nweectl station reconfigure\n# Remove the old database:\nrm ~/weewx-data/archive/weewx.sdb\n# Restart:\nsudo launchctl load /Library/LaunchDaemons/com.weewx.weewxd.plist\n</code></pre>",
             "title": "Configure"
         },
         {
             "location": "quickstarts/pip/#customize",
             "text": "<p>To enable uploads, such as Weather Underground, or to customize reports, modify the configuration file <code>~/weewx-data/weewx.conf</code>. See the User Guide and Customization Guide for details.</p>",
             "title": "Customize"
         },
         {
             "location": "quickstarts/pip/#uninstall",
-            "text": "<p>Stop, disable, and remove any daemon files:</p> Debian/Redhat/openSUSEVery old DebianmacOS <pre><code>sudo systemctl stop weewx\nsudo systemctl disable weewx\nsudo rm /etc/systemd/system/weewx.service\n</code></pre> <pre><code>sudo /etc/rc.d/init.d/weewx stop\nsudo rm /etc/init.d/weewx\n</code></pre> <pre><code>sudo launchctl unload /Library/LaunchDaemons/com.weewx.weewxd.plist\nsudo rm /Library/LaunchDaemons/com.weewx.weewxd.plist\n</code></pre> <p>Use pip to uninstall the program.</p> <pre><code>python3 -m pip uninstall weewx -y\n</code></pre> <p>You can also use pip to uninstall the dependencies, but first check that they are not being used by other programs!</p> <pre><code>python3 -m pip uninstall pyserial pyusb CT3 Pillow configobj PyMySQL pyephem ephem -y\n</code></pre> <p>Finally, if desired, delete the data directory:</p> <pre><code>rm -r ~/weewx-data\n</code></pre>",
+            "text": "<p>Before you uninstall, be sure that <code>weewxd</code> is not running.  Then remove the daemon configuration.</p> Systems that use systemd (e.g., Debian, Redhat, SUSE)Systems that use SysV init (e.g., Slackware, Devuan, Puppy, DD-WRT)macOS <pre><code>sudo systemctl stop weewx\nsudo systemctl disable weewx\nsudo rm /etc/systemd/system/weewx.service\n</code></pre> <pre><code>sudo /etc/rc.d/init.d/weewx stop\nsudo update-rc.d weewx remove\nsudo rm /etc/init.d/weewx\n</code></pre> <pre><code>sudo launchctl unload /Library/LaunchDaemons/com.weewx.weewxd.plist\nsudo rm /Library/LaunchDaemons/com.weewx.weewxd.plist\n</code></pre> <p>Use pip to uninstall weewx.</p> <pre><code>python3 -m pip uninstall weewx -y\n</code></pre> <p>You can also use pip to uninstall the dependencies, but first check that they are not being used by other programs!</p> <pre><code>python3 -m pip uninstall pyserial pyusb CT3 Pillow configobj PyMySQL pyephem ephem -y\n</code></pre> <p>Finally, if desired, delete the data directory:</p> <pre><code>rm -r ~/weewx-data\n</code></pre>",
             "title": "Uninstall"
         },
         {
             "location": "quickstarts/redhat/",
             "text": "<p>This is a guide to installing WeeWX from an RPM package on systems such as Redhat, CentOS or Fedora.</p>",
             "title": "Installation on Redhat-based systems"
         },
```

### Comparing `weewx-5.0.0a30/bin/wee_resources/docs/sitemap.xml` & `weewx-5.0.0b1/bin/wee_resources/docs/sitemap.xml`

 * *Files 26% similar despite different names*

#### Comparing `weewx-5.0.0a30/bin/wee_resources/docs/sitemap.xml` & `weewx-5.0.0b1/bin/wee_resources/docs/sitemap.xml`

```diff
@@ -1,278 +1,278 @@
 <?xml version="1.0" encoding="utf-8"?>
 <urlset xmlns="http://www.sitemaps.org/schemas/sitemap/0.9">
   <url>
     <loc>https://www.weewx.com/</loc>
-    <lastmod>2023-05-05</lastmod>
+    <lastmod>2023-05-21</lastmod>
     <changefreq>daily</changefreq>
   </url>
   <url>
     <loc>https://www.weewx.com/changes/</loc>
-    <lastmod>2023-05-05</lastmod>
+    <lastmod>2023-05-21</lastmod>
     <changefreq>daily</changefreq>
   </url>
   <url>
     <loc>https://www.weewx.com/copyright/</loc>
-    <lastmod>2023-05-05</lastmod>
+    <lastmod>2023-05-21</lastmod>
     <changefreq>daily</changefreq>
   </url>
   <url>
     <loc>https://www.weewx.com/devnotes/</loc>
-    <lastmod>2023-05-05</lastmod>
+    <lastmod>2023-05-21</lastmod>
     <changefreq>daily</changefreq>
   </url>
   <url>
     <loc>https://www.weewx.com/report_scheduling/</loc>
-    <lastmod>2023-05-05</lastmod>
+    <lastmod>2023-05-21</lastmod>
     <changefreq>daily</changefreq>
   </url>
   <url>
     <loc>https://www.weewx.com/sle/</loc>
-    <lastmod>2023-05-05</lastmod>
+    <lastmod>2023-05-21</lastmod>
     <changefreq>daily</changefreq>
   </url>
   <url>
     <loc>https://www.weewx.com/support/</loc>
-    <lastmod>2023-05-05</lastmod>
+    <lastmod>2023-05-21</lastmod>
     <changefreq>daily</changefreq>
   </url>
   <url>
     <loc>https://www.weewx.com/custom/</loc>
-    <lastmod>2023-05-05</lastmod>
+    <lastmod>2023-05-21</lastmod>
     <changefreq>daily</changefreq>
   </url>
   <url>
     <loc>https://www.weewx.com/custom/appendix/</loc>
-    <lastmod>2023-05-05</lastmod>
+    <lastmod>2023-05-21</lastmod>
     <changefreq>daily</changefreq>
   </url>
   <url>
     <loc>https://www.weewx.com/custom/cheetah/</loc>
-    <lastmod>2023-05-05</lastmod>
+    <lastmod>2023-05-21</lastmod>
     <changefreq>daily</changefreq>
   </url>
   <url>
     <loc>https://www.weewx.com/custom/custom_reports/</loc>
-    <lastmod>2023-05-05</lastmod>
+    <lastmod>2023-05-21</lastmod>
     <changefreq>daily</changefreq>
   </url>
   <url>
     <loc>https://www.weewx.com/custom/database/</loc>
-    <lastmod>2023-05-05</lastmod>
+    <lastmod>2023-05-21</lastmod>
     <changefreq>daily</changefreq>
   </url>
   <url>
     <loc>https://www.weewx.com/custom/derived/</loc>
-    <lastmod>2023-05-05</lastmod>
+    <lastmod>2023-05-21</lastmod>
     <changefreq>daily</changefreq>
   </url>
   <url>
     <loc>https://www.weewx.com/custom/drivers/</loc>
-    <lastmod>2023-05-05</lastmod>
+    <lastmod>2023-05-21</lastmod>
     <changefreq>daily</changefreq>
   </url>
   <url>
     <loc>https://www.weewx.com/custom/extensions/</loc>
-    <lastmod>2023-05-05</lastmod>
+    <lastmod>2023-05-21</lastmod>
     <changefreq>daily</changefreq>
   </url>
   <url>
     <loc>https://www.weewx.com/custom/image_generator/</loc>
-    <lastmod>2023-05-05</lastmod>
+    <lastmod>2023-05-21</lastmod>
     <changefreq>daily</changefreq>
   </url>
   <url>
     <loc>https://www.weewx.com/custom/localization/</loc>
-    <lastmod>2023-05-05</lastmod>
+    <lastmod>2023-05-21</lastmod>
     <changefreq>daily</changefreq>
   </url>
   <url>
     <loc>https://www.weewx.com/custom/multiple_bindings/</loc>
-    <lastmod>2023-05-05</lastmod>
+    <lastmod>2023-05-21</lastmod>
     <changefreq>daily</changefreq>
   </url>
   <url>
     <loc>https://www.weewx.com/custom/options_ref/</loc>
-    <lastmod>2023-05-05</lastmod>
+    <lastmod>2023-05-21</lastmod>
     <changefreq>daily</changefreq>
   </url>
   <url>
     <loc>https://www.weewx.com/custom/service_engine/</loc>
-    <lastmod>2023-05-05</lastmod>
+    <lastmod>2023-05-21</lastmod>
     <changefreq>daily</changefreq>
   </url>
   <url>
     <loc>https://www.weewx.com/custom/units/</loc>
-    <lastmod>2023-05-05</lastmod>
+    <lastmod>2023-05-21</lastmod>
     <changefreq>daily</changefreq>
   </url>
   <url>
     <loc>https://www.weewx.com/quickstarts/</loc>
-    <lastmod>2023-05-05</lastmod>
+    <lastmod>2023-05-21</lastmod>
     <changefreq>daily</changefreq>
   </url>
   <url>
     <loc>https://www.weewx.com/quickstarts/debian/</loc>
-    <lastmod>2023-05-05</lastmod>
+    <lastmod>2023-05-21</lastmod>
     <changefreq>daily</changefreq>
   </url>
   <url>
     <loc>https://www.weewx.com/quickstarts/pip/</loc>
-    <lastmod>2023-05-05</lastmod>
+    <lastmod>2023-05-21</lastmod>
     <changefreq>daily</changefreq>
   </url>
   <url>
     <loc>https://www.weewx.com/quickstarts/redhat/</loc>
-    <lastmod>2023-05-05</lastmod>
+    <lastmod>2023-05-21</lastmod>
     <changefreq>daily</changefreq>
   </url>
   <url>
     <loc>https://www.weewx.com/quickstarts/suse/</loc>
-    <lastmod>2023-05-05</lastmod>
+    <lastmod>2023-05-21</lastmod>
     <changefreq>daily</changefreq>
   </url>
   <url>
     <loc>https://www.weewx.com/quickstarts/v5-upgrade/</loc>
-    <lastmod>2023-05-05</lastmod>
+    <lastmod>2023-05-21</lastmod>
     <changefreq>daily</changefreq>
   </url>
   <url>
     <loc>https://www.weewx.com/usersguide/</loc>
-    <lastmod>2023-05-05</lastmod>
+    <lastmod>2023-05-21</lastmod>
     <changefreq>daily</changefreq>
   </url>
   <url>
     <loc>https://www.weewx.com/usersguide/backing-up-weewx/</loc>
-    <lastmod>2023-05-05</lastmod>
+    <lastmod>2023-05-21</lastmod>
     <changefreq>daily</changefreq>
   </url>
   <url>
     <loc>https://www.weewx.com/usersguide/installing-weewx/</loc>
-    <lastmod>2023-05-05</lastmod>
+    <lastmod>2023-05-21</lastmod>
     <changefreq>daily</changefreq>
   </url>
   <url>
     <loc>https://www.weewx.com/usersguide/mysql-mariadb-config/</loc>
-    <lastmod>2023-05-05</lastmod>
+    <lastmod>2023-05-21</lastmod>
     <changefreq>daily</changefreq>
   </url>
   <url>
     <loc>https://www.weewx.com/usersguide/running-weewx/</loc>
-    <lastmod>2023-05-05</lastmod>
+    <lastmod>2023-05-21</lastmod>
     <changefreq>daily</changefreq>
   </url>
   <url>
     <loc>https://www.weewx.com/usersguide/system-requirements/</loc>
-    <lastmod>2023-05-05</lastmod>
+    <lastmod>2023-05-21</lastmod>
     <changefreq>daily</changefreq>
   </url>
   <url>
     <loc>https://www.weewx.com/usersguide/troubleshooting-guide/</loc>
-    <lastmod>2023-05-05</lastmod>
+    <lastmod>2023-05-21</lastmod>
     <changefreq>daily</changefreq>
   </url>
   <url>
     <loc>https://www.weewx.com/usersguide/webserver-integration/</loc>
-    <lastmod>2023-05-05</lastmod>
+    <lastmod>2023-05-21</lastmod>
     <changefreq>daily</changefreq>
   </url>
   <url>
     <loc>https://www.weewx.com/usersguide/where/</loc>
-    <lastmod>2023-05-05</lastmod>
+    <lastmod>2023-05-21</lastmod>
     <changefreq>daily</changefreq>
   </url>
   <url>
     <loc>https://www.weewx.com/usersguide/weewx-config-file/</loc>
-    <lastmod>2023-05-05</lastmod>
+    <lastmod>2023-05-21</lastmod>
     <changefreq>daily</changefreq>
   </url>
   <url>
     <loc>https://www.weewx.com/usersguide/weewx-config-file/data-bindings/</loc>
-    <lastmod>2023-05-05</lastmod>
+    <lastmod>2023-05-21</lastmod>
     <changefreq>daily</changefreq>
   </url>
   <url>
     <loc>https://www.weewx.com/usersguide/weewx-config-file/databases/</loc>
-    <lastmod>2023-05-05</lastmod>
+    <lastmod>2023-05-21</lastmod>
     <changefreq>daily</changefreq>
   </url>
   <url>
     <loc>https://www.weewx.com/usersguide/weewx-config-file/databasetypes/</loc>
-    <lastmod>2023-05-05</lastmod>
+    <lastmod>2023-05-21</lastmod>
     <changefreq>daily</changefreq>
   </url>
   <url>
     <loc>https://www.weewx.com/usersguide/weewx-config-file/engine/</loc>
-    <lastmod>2023-05-05</lastmod>
+    <lastmod>2023-05-21</lastmod>
     <changefreq>daily</changefreq>
   </url>
   <url>
     <loc>https://www.weewx.com/usersguide/weewx-config-file/general/</loc>
-    <lastmod>2023-05-05</lastmod>
+    <lastmod>2023-05-21</lastmod>
     <changefreq>daily</changefreq>
   </url>
   <url>
     <loc>https://www.weewx.com/usersguide/weewx-config-file/stations-config/</loc>
-    <lastmod>2023-05-05</lastmod>
+    <lastmod>2023-05-21</lastmod>
     <changefreq>daily</changefreq>
   </url>
   <url>
     <loc>https://www.weewx.com/usersguide/weewx-config-file/stdarchive/</loc>
-    <lastmod>2023-05-05</lastmod>
+    <lastmod>2023-05-21</lastmod>
     <changefreq>daily</changefreq>
   </url>
   <url>
     <loc>https://www.weewx.com/usersguide/weewx-config-file/stdcalibrate-config/</loc>
-    <lastmod>2023-05-05</lastmod>
+    <lastmod>2023-05-21</lastmod>
     <changefreq>daily</changefreq>
   </url>
   <url>
     <loc>https://www.weewx.com/usersguide/weewx-config-file/stdconvert-config/</loc>
-    <lastmod>2023-05-05</lastmod>
+    <lastmod>2023-05-21</lastmod>
     <changefreq>daily</changefreq>
   </url>
   <url>
     <loc>https://www.weewx.com/usersguide/weewx-config-file/stdqc-config/</loc>
-    <lastmod>2023-05-05</lastmod>
+    <lastmod>2023-05-21</lastmod>
     <changefreq>daily</changefreq>
   </url>
   <url>
     <loc>https://www.weewx.com/usersguide/weewx-config-file/stdreport-config/</loc>
-    <lastmod>2023-05-05</lastmod>
+    <lastmod>2023-05-21</lastmod>
     <changefreq>daily</changefreq>
   </url>
   <url>
     <loc>https://www.weewx.com/usersguide/weewx-config-file/stdrestful-config/</loc>
-    <lastmod>2023-05-05</lastmod>
+    <lastmod>2023-05-21</lastmod>
     <changefreq>daily</changefreq>
   </url>
   <url>
     <loc>https://www.weewx.com/usersguide/weewx-config-file/stdtimesynch/</loc>
-    <lastmod>2023-05-05</lastmod>
+    <lastmod>2023-05-21</lastmod>
     <changefreq>daily</changefreq>
   </url>
   <url>
     <loc>https://www.weewx.com/usersguide/weewx-config-file/stdwxcalculate-config/</loc>
-    <lastmod>2023-05-05</lastmod>
+    <lastmod>2023-05-21</lastmod>
     <changefreq>daily</changefreq>
   </url>
   <url>
     <loc>https://www.weewx.com/utilities/</loc>
-    <lastmod>2023-05-05</lastmod>
+    <lastmod>2023-05-21</lastmod>
     <changefreq>daily</changefreq>
   </url>
   <url>
     <loc>https://www.weewx.com/weectl/</loc>
-    <lastmod>2023-05-05</lastmod>
+    <lastmod>2023-05-21</lastmod>
     <changefreq>daily</changefreq>
   </url>
   <url>
     <loc>https://www.weewx.com/weectl/extension/</loc>
-    <lastmod>2023-05-05</lastmod>
+    <lastmod>2023-05-21</lastmod>
     <changefreq>daily</changefreq>
   </url>
   <url>
     <loc>https://www.weewx.com/weectl/station/</loc>
-    <lastmod>2023-05-05</lastmod>
+    <lastmod>2023-05-21</lastmod>
     <changefreq>daily</changefreq>
   </url>
 </urlset>
```

### Comparing `weewx-5.0.0a30/bin/wee_resources/docs/sle/index.html` & `weewx-5.0.0b1/bin/wee_resources/docs/sle/index.html`

 * *Files identical despite different names*

### Comparing `weewx-5.0.0a30/bin/wee_resources/docs/support/index.html` & `weewx-5.0.0b1/bin/wee_resources/docs/support/index.html`

 * *Files identical despite different names*

### Comparing `weewx-5.0.0a30/bin/wee_resources/docs/upgrading.htm` & `weewx-5.0.0b1/bin/wee_resources/docs/upgrading.htm`

 * *Files identical despite different names*

### Comparing `weewx-5.0.0a30/bin/wee_resources/docs/usersguide/backing-up-weewx/index.html` & `weewx-5.0.0b1/bin/wee_resources/docs/usersguide/backing-up-weewx/index.html`

 * *Files identical despite different names*

### Comparing `weewx-5.0.0a30/bin/wee_resources/docs/usersguide/index.html` & `weewx-5.0.0b1/bin/wee_resources/docs/usersguide/index.html`

 * *Files identical despite different names*

### Comparing `weewx-5.0.0a30/bin/wee_resources/docs/usersguide/installing-weewx/index.html` & `weewx-5.0.0b1/bin/wee_resources/docs/usersguide/installing-weewx/index.html`

 * *Files identical despite different names*

### Comparing `weewx-5.0.0a30/bin/wee_resources/docs/usersguide/mysql-mariadb-config/index.html` & `weewx-5.0.0b1/bin/wee_resources/docs/usersguide/mysql-mariadb-config/index.html`

 * *Files identical despite different names*

### Comparing `weewx-5.0.0a30/bin/wee_resources/docs/usersguide/running-weewx/index.html` & `weewx-5.0.0b1/bin/wee_resources/docs/usersguide/running-weewx/index.html`

 * *Files identical despite different names*

### Comparing `weewx-5.0.0a30/bin/wee_resources/docs/usersguide/system-requirements/index.html` & `weewx-5.0.0b1/bin/wee_resources/docs/usersguide/system-requirements/index.html`

 * *Files identical despite different names*

### Comparing `weewx-5.0.0a30/bin/wee_resources/docs/usersguide/troubleshooting-guide/index.html` & `weewx-5.0.0b1/bin/wee_resources/docs/usersguide/troubleshooting-guide/index.html`

 * *Files identical despite different names*

### Comparing `weewx-5.0.0a30/bin/wee_resources/docs/usersguide/webserver-integration/index.html` & `weewx-5.0.0b1/bin/wee_resources/docs/usersguide/webserver-integration/index.html`

 * *Files identical despite different names*

### Comparing `weewx-5.0.0a30/bin/wee_resources/docs/usersguide/weewx-config-file/data-bindings/index.html` & `weewx-5.0.0b1/bin/wee_resources/docs/usersguide/weewx-config-file/data-bindings/index.html`

 * *Files identical despite different names*

### Comparing `weewx-5.0.0a30/bin/wee_resources/docs/usersguide/weewx-config-file/databases/index.html` & `weewx-5.0.0b1/bin/wee_resources/docs/usersguide/weewx-config-file/databases/index.html`

 * *Files identical despite different names*

### Comparing `weewx-5.0.0a30/bin/wee_resources/docs/usersguide/weewx-config-file/databasetypes/index.html` & `weewx-5.0.0b1/bin/wee_resources/docs/usersguide/weewx-config-file/databasetypes/index.html`

 * *Files identical despite different names*

### Comparing `weewx-5.0.0a30/bin/wee_resources/docs/usersguide/weewx-config-file/engine/index.html` & `weewx-5.0.0b1/bin/wee_resources/docs/usersguide/weewx-config-file/engine/index.html`

 * *Files identical despite different names*

### Comparing `weewx-5.0.0a30/bin/wee_resources/docs/usersguide/weewx-config-file/general/index.html` & `weewx-5.0.0b1/bin/wee_resources/docs/usersguide/weewx-config-file/general/index.html`

 * *Files identical despite different names*

### Comparing `weewx-5.0.0a30/bin/wee_resources/docs/usersguide/weewx-config-file/index.html` & `weewx-5.0.0b1/bin/wee_resources/docs/usersguide/weewx-config-file/index.html`

 * *Files identical despite different names*

### Comparing `weewx-5.0.0a30/bin/wee_resources/docs/usersguide/weewx-config-file/stations-config/index.html` & `weewx-5.0.0b1/bin/wee_resources/docs/usersguide/weewx-config-file/stations-config/index.html`

 * *Files identical despite different names*

### Comparing `weewx-5.0.0a30/bin/wee_resources/docs/usersguide/weewx-config-file/stdarchive/index.html` & `weewx-5.0.0b1/bin/wee_resources/docs/usersguide/weewx-config-file/stdarchive/index.html`

 * *Files identical despite different names*

### Comparing `weewx-5.0.0a30/bin/wee_resources/docs/usersguide/weewx-config-file/stdcalibrate-config/index.html` & `weewx-5.0.0b1/bin/wee_resources/docs/usersguide/weewx-config-file/stdcalibrate-config/index.html`

 * *Files identical despite different names*

### Comparing `weewx-5.0.0a30/bin/wee_resources/docs/usersguide/weewx-config-file/stdconvert-config/index.html` & `weewx-5.0.0b1/bin/wee_resources/docs/usersguide/weewx-config-file/stdconvert-config/index.html`

 * *Files identical despite different names*

### Comparing `weewx-5.0.0a30/bin/wee_resources/docs/usersguide/weewx-config-file/stdqc-config/index.html` & `weewx-5.0.0b1/bin/wee_resources/docs/usersguide/weewx-config-file/stdqc-config/index.html`

 * *Files identical despite different names*

### Comparing `weewx-5.0.0a30/bin/wee_resources/docs/usersguide/weewx-config-file/stdreport-config/index.html` & `weewx-5.0.0b1/bin/wee_resources/docs/usersguide/weewx-config-file/stdreport-config/index.html`

 * *Files identical despite different names*

### Comparing `weewx-5.0.0a30/bin/wee_resources/docs/usersguide/weewx-config-file/stdrestful-config/index.html` & `weewx-5.0.0b1/bin/wee_resources/docs/usersguide/weewx-config-file/stdrestful-config/index.html`

 * *Files identical despite different names*

### Comparing `weewx-5.0.0a30/bin/wee_resources/docs/usersguide/weewx-config-file/stdtimesynch/index.html` & `weewx-5.0.0b1/bin/wee_resources/docs/usersguide/weewx-config-file/stdtimesynch/index.html`

 * *Files identical despite different names*

### Comparing `weewx-5.0.0a30/bin/wee_resources/docs/usersguide/weewx-config-file/stdwxcalculate-config/index.html` & `weewx-5.0.0b1/bin/wee_resources/docs/usersguide/weewx-config-file/stdwxcalculate-config/index.html`

 * *Files identical despite different names*

### Comparing `weewx-5.0.0a30/bin/wee_resources/docs/usersguide/where/index.html` & `weewx-5.0.0b1/bin/wee_resources/docs/usersguide/where/index.html`

 * *Files identical despite different names*

### Comparing `weewx-5.0.0a30/bin/wee_resources/docs/utilities/index.html` & `weewx-5.0.0b1/bin/wee_resources/docs/utilities/index.html`

 * *Files identical despite different names*

### Comparing `weewx-5.0.0a30/bin/wee_resources/docs/utilities/utilities.htm` & `weewx-5.0.0b1/bin/wee_resources/docs/utilities/utilities.htm`

 * *Files identical despite different names*

### Comparing `weewx-5.0.0a30/bin/wee_resources/docs/weectl/extension/index.html` & `weewx-5.0.0b1/bin/wee_resources/docs/weectl/extension/index.html`

 * *Files identical despite different names*

### Comparing `weewx-5.0.0a30/bin/wee_resources/docs/weectl/index.html` & `weewx-5.0.0b1/bin/wee_resources/docs/weectl/index.html`

 * *Files identical despite different names*

### Comparing `weewx-5.0.0a30/bin/wee_resources/docs/weectl/station/index.html` & `weewx-5.0.0b1/bin/wee_resources/docs/weectl/station/index.html`

 * *Files identical despite different names*

### Comparing `weewx-5.0.0a30/bin/wee_resources/examples/__pycache__/seven_day.cpython-37.pyc` & `weewx-5.0.0b1/bin/wee_resources/examples/__pycache__/seven_day.cpython-37.pyc`

 * *Files identical despite different names*

### Comparing `weewx-5.0.0a30/bin/wee_resources/examples/__pycache__/vaporpressure.cpython-310.pyc` & `weewx-5.0.0b1/bin/wee_resources/examples/__pycache__/vaporpressure.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `weewx-5.0.0a30/bin/wee_resources/examples/__pycache__/vaporpressure.cpython-37.pyc` & `weewx-5.0.0b1/bin/wee_resources/examples/__pycache__/vaporpressure.cpython-37.pyc`

 * *Files identical despite different names*

### Comparing `weewx-5.0.0a30/bin/wee_resources/examples/alarm.py` & `weewx-5.0.0b1/bin/wee_resources/examples/alarm.py`

 * *Files identical despite different names*

### Comparing `weewx-5.0.0a30/bin/wee_resources/examples/basic/install.py` & `weewx-5.0.0b1/bin/wee_resources/examples/basic/install.py`

 * *Files identical despite different names*

### Comparing `weewx-5.0.0a30/bin/wee_resources/examples/basic/readme.md` & `weewx-5.0.0b1/bin/wee_resources/examples/basic/readme.md`

 * *Files identical despite different names*

### Comparing `weewx-5.0.0a30/bin/wee_resources/examples/basic/skins/basic/basic.css` & `weewx-5.0.0b1/bin/wee_resources/examples/basic/skins/basic/basic.css`

 * *Files identical despite different names*

### Comparing `weewx-5.0.0a30/bin/wee_resources/examples/basic/skins/basic/current.inc` & `weewx-5.0.0b1/bin/wee_resources/examples/basic/skins/basic/current.inc`

 * *Files identical despite different names*

### Comparing `weewx-5.0.0a30/bin/wee_resources/examples/basic/skins/basic/favicon.ico` & `weewx-5.0.0b1/bin/wee_resources/examples/basic/skins/basic/favicon.ico`

 * *Files identical despite different names*

### Comparing `weewx-5.0.0a30/bin/wee_resources/examples/basic/skins/basic/hilo.inc` & `weewx-5.0.0b1/bin/wee_resources/examples/basic/skins/basic/hilo.inc`

 * *Files identical despite different names*

### Comparing `weewx-5.0.0a30/bin/wee_resources/examples/basic/skins/basic/index.html.tmpl` & `weewx-5.0.0b1/bin/wee_resources/examples/basic/skins/basic/index.html.tmpl`

 * *Files identical despite different names*

### Comparing `weewx-5.0.0a30/bin/wee_resources/examples/basic/skins/basic/lang/en.conf` & `weewx-5.0.0b1/bin/wee_resources/examples/basic/skins/basic/lang/en.conf`

 * *Files identical despite different names*

### Comparing `weewx-5.0.0a30/bin/wee_resources/examples/basic/skins/basic/lang/fr.conf` & `weewx-5.0.0b1/bin/wee_resources/examples/basic/skins/basic/lang/fr.conf`

 * *Files identical despite different names*

### Comparing `weewx-5.0.0a30/bin/wee_resources/examples/basic/skins/basic/skin.conf` & `weewx-5.0.0b1/bin/wee_resources/examples/basic/skins/basic/skin.conf`

 * *Files identical despite different names*

### Comparing `weewx-5.0.0a30/bin/wee_resources/examples/colorize/__pycache__/colorize_1.cpython-37.pyc` & `weewx-5.0.0b1/bin/wee_resources/examples/colorize/__pycache__/colorize_1.cpython-37.pyc`

 * *Files identical despite different names*

### Comparing `weewx-5.0.0a30/bin/wee_resources/examples/colorize/__pycache__/colorize_2.cpython-37.pyc` & `weewx-5.0.0b1/bin/wee_resources/examples/colorize/__pycache__/colorize_2.cpython-37.pyc`

 * *Files identical despite different names*

### Comparing `weewx-5.0.0a30/bin/wee_resources/examples/colorize/__pycache__/colorize_3.cpython-37.pyc` & `weewx-5.0.0b1/bin/wee_resources/examples/colorize/__pycache__/colorize_3.cpython-37.pyc`

 * *Files identical despite different names*

### Comparing `weewx-5.0.0a30/bin/wee_resources/examples/colorize/colorize_1.py` & `weewx-5.0.0b1/bin/wee_resources/examples/colorize/colorize_1.py`

 * *Files identical despite different names*

### Comparing `weewx-5.0.0a30/bin/wee_resources/examples/colorize/colorize_2.py` & `weewx-5.0.0b1/bin/wee_resources/examples/colorize/colorize_2.py`

 * *Files identical despite different names*

### Comparing `weewx-5.0.0a30/bin/wee_resources/examples/colorize/colorize_3.py` & `weewx-5.0.0b1/bin/wee_resources/examples/colorize/colorize_3.py`

 * *Files identical despite different names*

### Comparing `weewx-5.0.0a30/bin/wee_resources/examples/fileparse/bin/user/fileparse.py` & `weewx-5.0.0b1/bin/wee_resources/examples/fileparse/bin/user/fileparse.py`

 * *Files identical despite different names*

### Comparing `weewx-5.0.0a30/bin/wee_resources/examples/fileparse/install.py` & `weewx-5.0.0b1/bin/wee_resources/examples/fileparse/install.py`

 * *Files identical despite different names*

### Comparing `weewx-5.0.0a30/bin/wee_resources/examples/fileparse/readme.md` & `weewx-5.0.0b1/bin/wee_resources/examples/fileparse/readme.md`

 * *Files identical despite different names*

### Comparing `weewx-5.0.0a30/bin/wee_resources/examples/lowBattery.py` & `weewx-5.0.0b1/bin/wee_resources/examples/lowBattery.py`

 * *Files identical despite different names*

### Comparing `weewx-5.0.0a30/bin/wee_resources/examples/mem.py` & `weewx-5.0.0b1/bin/wee_resources/examples/mem.py`

 * *Files identical despite different names*

### Comparing `weewx-5.0.0a30/bin/wee_resources/examples/pmon/bin/user/pmon.py` & `weewx-5.0.0b1/bin/wee_resources/examples/pmon/bin/user/pmon.py`

 * *Files identical despite different names*

### Comparing `weewx-5.0.0a30/bin/wee_resources/examples/pmon/install.py` & `weewx-5.0.0b1/bin/wee_resources/examples/pmon/install.py`

 * *Files identical despite different names*

### Comparing `weewx-5.0.0a30/bin/wee_resources/examples/pmon/readme.md` & `weewx-5.0.0b1/bin/wee_resources/examples/pmon/readme.md`

 * *Files identical despite different names*

### Comparing `weewx-5.0.0a30/bin/wee_resources/examples/pmon/skins/pmon/skin.conf` & `weewx-5.0.0b1/bin/wee_resources/examples/pmon/skins/pmon/skin.conf`

 * *Files identical despite different names*

### Comparing `weewx-5.0.0a30/bin/wee_resources/examples/tests/test_vaporpressure.py` & `weewx-5.0.0b1/bin/wee_resources/examples/tests/test_vaporpressure.py`

 * *Files identical despite different names*

### Comparing `weewx-5.0.0a30/bin/wee_resources/examples/vaporpressure.py` & `weewx-5.0.0b1/bin/wee_resources/examples/vaporpressure.py`

 * *Files identical despite different names*

### Comparing `weewx-5.0.0a30/bin/wee_resources/examples/xstats/bin/user/xstats.py` & `weewx-5.0.0b1/bin/wee_resources/examples/xstats/bin/user/xstats.py`

 * *Files identical despite different names*

### Comparing `weewx-5.0.0a30/bin/wee_resources/examples/xstats/install.py` & `weewx-5.0.0b1/bin/wee_resources/examples/xstats/install.py`

 * *Files identical despite different names*

### Comparing `weewx-5.0.0a30/bin/wee_resources/examples/xstats/readme.txt` & `weewx-5.0.0b1/bin/wee_resources/examples/xstats/readme.txt`

 * *Files identical despite different names*

### Comparing `weewx-5.0.0a30/bin/wee_resources/examples/xstats/skins/xstats/index.html.tmpl` & `weewx-5.0.0b1/bin/wee_resources/examples/xstats/skins/xstats/index.html.tmpl`

 * *Files identical despite different names*

### Comparing `weewx-5.0.0a30/bin/wee_resources/examples/xstats/skins/xstats/skin.conf` & `weewx-5.0.0b1/bin/wee_resources/examples/xstats/skins/xstats/skin.conf`

 * *Files identical despite different names*

### Comparing `weewx-5.0.0a30/bin/wee_resources/skins/Ftp/skin.conf` & `weewx-5.0.0b1/bin/wee_resources/skins/Ftp/skin.conf`

 * *Files 2% similar despite different names*

```diff
@@ -3,12 +3,12 @@
 #                                                                             #
 # FTP CONFIGURATION FILE                                                      #
 #   This 'report' does not generate any files. Instead, we use the report     #
 #   engine to invoke FTP, which copies files to another location.             #
 ###############################################################################
 
 SKIN_NAME = Ftp
-SKIN_VERSION = 5.0.0a30
+SKIN_VERSION = 5.0.0b1
 
 [Generators]
     generator_list = weewx.reportengine.FtpGenerator
```

### Comparing `weewx-5.0.0a30/bin/wee_resources/skins/Mobile/favicon.ico` & `weewx-5.0.0b1/bin/wee_resources/skins/Mobile/favicon.ico`

 * *Files identical despite different names*

### Comparing `weewx-5.0.0a30/bin/wee_resources/skins/Mobile/index.html.tmpl` & `weewx-5.0.0b1/bin/wee_resources/skins/Mobile/index.html.tmpl`

 * *Files identical despite different names*

### Comparing `weewx-5.0.0a30/bin/wee_resources/skins/Mobile/lang/de.conf` & `weewx-5.0.0b1/bin/wee_resources/skins/Mobile/lang/de.conf`

 * *Files identical despite different names*

### Comparing `weewx-5.0.0a30/bin/wee_resources/skins/Mobile/lang/en.conf` & `weewx-5.0.0b1/bin/wee_resources/skins/Mobile/lang/en.conf`

 * *Files identical despite different names*

### Comparing `weewx-5.0.0a30/bin/wee_resources/skins/Mobile/lang/nl.conf` & `weewx-5.0.0b1/bin/wee_resources/skins/Mobile/lang/nl.conf`

 * *Files identical despite different names*

### Comparing `weewx-5.0.0a30/bin/wee_resources/skins/Mobile/lang/no.conf` & `weewx-5.0.0b1/bin/wee_resources/skins/Mobile/lang/no.conf`

 * *Files identical despite different names*

### Comparing `weewx-5.0.0a30/bin/wee_resources/skins/Mobile/mobile.css` & `weewx-5.0.0b1/bin/wee_resources/skins/Mobile/mobile.css`

 * *Files identical despite different names*

### Comparing `weewx-5.0.0a30/bin/wee_resources/skins/Mobile/skin.conf` & `weewx-5.0.0b1/bin/wee_resources/skins/Mobile/skin.conf`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 # configuration file for Mobile skin
 
 SKIN_NAME = Mobile
-SKIN_VERSION = 5.0.0a30
+SKIN_VERSION = 5.0.0b1
 
 [Extras]
     # Set this URL to display a radar image
     #radar_img = http://radar.weather.gov/ridge/lite/N0R/RTX_loop.gif
     # Set this URL for the radar image link
     #radar_url = http://radar.weather.gov/ridge/radar.php?product=NCR&rid=RTX&loop=yes
```

### Comparing `weewx-5.0.0a30/bin/wee_resources/skins/Rsync/skin.conf` & `weewx-5.0.0b1/bin/wee_resources/skins/Rsync/skin.conf`

 * *Files 1% similar despite different names*

```diff
@@ -4,12 +4,12 @@
 #                                                                             #
 # RSYNC CONFIGURATION FILE                                                    #
 #   This 'report' does not generate any files. Instead, we use the report     #
 #   engine to invoke rsync, which synchronizes files between two locations.   #
 ###############################################################################
 
 SKIN_NAME = Rsync
-SKIN_VERSION = 5.0.0a30
+SKIN_VERSION = 5.0.0b1
 
 [Generators]
     generator_list = weewx.reportengine.RsyncGenerator
```

### Comparing `weewx-5.0.0a30/bin/wee_resources/skins/Seasons/NOAA/NOAA-%Y-%m.txt.tmpl` & `weewx-5.0.0b1/bin/wee_resources/skins/Seasons/NOAA/NOAA-%Y-%m.txt.tmpl`

 * *Files identical despite different names*

### Comparing `weewx-5.0.0a30/bin/wee_resources/skins/Seasons/NOAA/NOAA-%Y.txt.tmpl` & `weewx-5.0.0b1/bin/wee_resources/skins/Seasons/NOAA/NOAA-%Y.txt.tmpl`

 * *Files identical despite different names*

### Comparing `weewx-5.0.0a30/bin/wee_resources/skins/Seasons/about.inc` & `weewx-5.0.0b1/bin/wee_resources/skins/Seasons/about.inc`

 * *Files identical despite different names*

### Comparing `weewx-5.0.0a30/bin/wee_resources/skins/Seasons/analytics.inc` & `weewx-5.0.0b1/bin/wee_resources/skins/Seasons/analytics.inc`

 * *Files identical despite different names*

### Comparing `weewx-5.0.0a30/bin/wee_resources/skins/Seasons/celestial.html.tmpl` & `weewx-5.0.0b1/bin/wee_resources/skins/Seasons/celestial.html.tmpl`

 * *Files identical despite different names*

### Comparing `weewx-5.0.0a30/bin/wee_resources/skins/Seasons/celestial.inc` & `weewx-5.0.0b1/bin/wee_resources/skins/Seasons/celestial.inc`

 * *Files identical despite different names*

### Comparing `weewx-5.0.0a30/bin/wee_resources/skins/Seasons/current.inc` & `weewx-5.0.0b1/bin/wee_resources/skins/Seasons/current.inc`

 * *Files identical despite different names*

### Comparing `weewx-5.0.0a30/bin/wee_resources/skins/Seasons/favicon.ico` & `weewx-5.0.0b1/bin/wee_resources/skins/Seasons/favicon.ico`

 * *Files identical despite different names*

### Comparing `weewx-5.0.0a30/bin/wee_resources/skins/Seasons/font/Kanit-Bold.ttf` & `weewx-5.0.0b1/bin/wee_resources/skins/Seasons/font/Kanit-Bold.ttf`

 * *Files identical despite different names*

### Comparing `weewx-5.0.0a30/bin/wee_resources/skins/Seasons/font/Kanit-Regular.ttf` & `weewx-5.0.0b1/bin/wee_resources/skins/Seasons/font/Kanit-Regular.ttf`

 * *Files identical despite different names*

### Comparing `weewx-5.0.0a30/bin/wee_resources/skins/Seasons/font/OFL.txt` & `weewx-5.0.0b1/bin/wee_resources/skins/Seasons/font/OFL.txt`

 * *Files identical despite different names*

### Comparing `weewx-5.0.0a30/bin/wee_resources/skins/Seasons/font/OpenSans-Bold.ttf` & `weewx-5.0.0b1/bin/wee_resources/skins/Seasons/font/OpenSans-Bold.ttf`

 * *Files identical despite different names*

### Comparing `weewx-5.0.0a30/bin/wee_resources/skins/Seasons/font/OpenSans-Regular.ttf` & `weewx-5.0.0b1/bin/wee_resources/skins/Seasons/font/OpenSans-Regular.ttf`

 * *Files identical despite different names*

### Comparing `weewx-5.0.0a30/bin/wee_resources/skins/Seasons/font/OpenSans.woff` & `weewx-5.0.0b1/bin/wee_resources/skins/Seasons/font/OpenSans.woff`

 * *Files identical despite different names*

### Comparing `weewx-5.0.0a30/bin/wee_resources/skins/Seasons/font/OpenSans.woff2` & `weewx-5.0.0b1/bin/wee_resources/skins/Seasons/font/OpenSans.woff2`

 * *Files identical despite different names*

### Comparing `weewx-5.0.0a30/bin/wee_resources/skins/Seasons/font/license.txt` & `weewx-5.0.0b1/bin/wee_resources/skins/Seasons/font/license.txt`

 * *Files identical despite different names*

### Comparing `weewx-5.0.0a30/bin/wee_resources/skins/Seasons/hilo.inc` & `weewx-5.0.0b1/bin/wee_resources/skins/Seasons/hilo.inc`

 * *Files identical despite different names*

### Comparing `weewx-5.0.0a30/bin/wee_resources/skins/Seasons/identifier.inc` & `weewx-5.0.0b1/bin/wee_resources/skins/Seasons/identifier.inc`

 * *Files identical despite different names*

### Comparing `weewx-5.0.0a30/bin/wee_resources/skins/Seasons/index.html.tmpl` & `weewx-5.0.0b1/bin/wee_resources/skins/Seasons/index.html.tmpl`

 * *Files identical despite different names*

### Comparing `weewx-5.0.0a30/bin/wee_resources/skins/Seasons/lang/cn.conf` & `weewx-5.0.0b1/bin/wee_resources/skins/Seasons/lang/cn.conf`

 * *Files identical despite different names*

### Comparing `weewx-5.0.0a30/bin/wee_resources/skins/Seasons/lang/cz.conf` & `weewx-5.0.0b1/bin/wee_resources/skins/Seasons/lang/cz.conf`

 * *Files identical despite different names*

### Comparing `weewx-5.0.0a30/bin/wee_resources/skins/Seasons/lang/de.conf` & `weewx-5.0.0b1/bin/wee_resources/skins/Seasons/lang/de.conf`

 * *Files identical despite different names*

### Comparing `weewx-5.0.0a30/bin/wee_resources/skins/Seasons/lang/en.conf` & `weewx-5.0.0b1/bin/wee_resources/skins/Seasons/lang/en.conf`

 * *Files identical despite different names*

### Comparing `weewx-5.0.0a30/bin/wee_resources/skins/Seasons/lang/es.conf` & `weewx-5.0.0b1/bin/wee_resources/skins/Seasons/lang/es.conf`

 * *Files identical despite different names*

### Comparing `weewx-5.0.0a30/bin/wee_resources/skins/Seasons/lang/fr.conf` & `weewx-5.0.0b1/bin/wee_resources/skins/Seasons/lang/fr.conf`

 * *Files identical despite different names*

### Comparing `weewx-5.0.0a30/bin/wee_resources/skins/Seasons/lang/gr.conf` & `weewx-5.0.0b1/bin/wee_resources/skins/Seasons/lang/gr.conf`

 * *Files identical despite different names*

### Comparing `weewx-5.0.0a30/bin/wee_resources/skins/Seasons/lang/it.conf` & `weewx-5.0.0b1/bin/wee_resources/skins/Seasons/lang/it.conf`

 * *Files identical despite different names*

### Comparing `weewx-5.0.0a30/bin/wee_resources/skins/Seasons/lang/nl.conf` & `weewx-5.0.0b1/bin/wee_resources/skins/Seasons/lang/nl.conf`

 * *Files identical despite different names*

### Comparing `weewx-5.0.0a30/bin/wee_resources/skins/Seasons/lang/no.conf` & `weewx-5.0.0b1/bin/wee_resources/skins/Seasons/lang/no.conf`

 * *Files identical despite different names*

### Comparing `weewx-5.0.0a30/bin/wee_resources/skins/Seasons/lang/th.conf` & `weewx-5.0.0b1/bin/wee_resources/skins/Seasons/lang/th.conf`

 * *Files identical despite different names*

### Comparing `weewx-5.0.0a30/bin/wee_resources/skins/Seasons/map.inc` & `weewx-5.0.0b1/bin/wee_resources/skins/Seasons/map.inc`

 * *Files identical despite different names*

### Comparing `weewx-5.0.0a30/bin/wee_resources/skins/Seasons/radar.inc` & `weewx-5.0.0b1/bin/wee_resources/skins/Seasons/radar.inc`

 * *Files identical despite different names*

### Comparing `weewx-5.0.0a30/bin/wee_resources/skins/Seasons/rss.xml.tmpl` & `weewx-5.0.0b1/bin/wee_resources/skins/Seasons/rss.xml.tmpl`

 * *Files identical despite different names*

### Comparing `weewx-5.0.0a30/bin/wee_resources/skins/Seasons/satellite.inc` & `weewx-5.0.0b1/bin/wee_resources/skins/Seasons/satellite.inc`

 * *Files identical despite different names*

### Comparing `weewx-5.0.0a30/bin/wee_resources/skins/Seasons/seasons.css` & `weewx-5.0.0b1/bin/wee_resources/skins/Seasons/seasons.css`

 * *Files identical despite different names*

### Comparing `weewx-5.0.0a30/bin/wee_resources/skins/Seasons/seasons.js` & `weewx-5.0.0b1/bin/wee_resources/skins/Seasons/seasons.js`

 * *Files identical despite different names*

### Comparing `weewx-5.0.0a30/bin/wee_resources/skins/Seasons/sensors.inc` & `weewx-5.0.0b1/bin/wee_resources/skins/Seasons/sensors.inc`

 * *Files identical despite different names*

### Comparing `weewx-5.0.0a30/bin/wee_resources/skins/Seasons/skin.conf` & `weewx-5.0.0b1/bin/wee_resources/skins/Seasons/skin.conf`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 ###############################################################################
 # SEASONS SKIN CONFIGURATION FILE                                             #
 # Copyright (c) 2018-2021 Tom Keffer <tkeffer@gmail.com> and Matthew Wall     #
 # See the file LICENSE.txt for your rights.                                   #
 ###############################################################################
 
 SKIN_NAME = Seasons
-SKIN_VERSION = 5.0.0a30
+SKIN_VERSION = 5.0.0b1
 
 ###############################################################################
 
 # The following section is for any extra tags that you want to be available in
 # the templates
 
 [Extras]
```

### Comparing `weewx-5.0.0a30/bin/wee_resources/skins/Seasons/statistics.html.tmpl` & `weewx-5.0.0b1/bin/wee_resources/skins/Seasons/statistics.html.tmpl`

 * *Files identical despite different names*

### Comparing `weewx-5.0.0a30/bin/wee_resources/skins/Seasons/statistics.inc` & `weewx-5.0.0b1/bin/wee_resources/skins/Seasons/statistics.inc`

 * *Files identical despite different names*

### Comparing `weewx-5.0.0a30/bin/wee_resources/skins/Seasons/sunmoon.inc` & `weewx-5.0.0b1/bin/wee_resources/skins/Seasons/sunmoon.inc`

 * *Files identical despite different names*

### Comparing `weewx-5.0.0a30/bin/wee_resources/skins/Seasons/tabular.html.tmpl` & `weewx-5.0.0b1/bin/wee_resources/skins/Seasons/tabular.html.tmpl`

 * *Files identical despite different names*

### Comparing `weewx-5.0.0a30/bin/wee_resources/skins/Seasons/telemetry.html.tmpl` & `weewx-5.0.0b1/bin/wee_resources/skins/Seasons/telemetry.html.tmpl`

 * *Files identical despite different names*

### Comparing `weewx-5.0.0a30/bin/wee_resources/skins/Seasons/titlebar.inc` & `weewx-5.0.0b1/bin/wee_resources/skins/Seasons/titlebar.inc`

 * *Files identical despite different names*

### Comparing `weewx-5.0.0a30/bin/wee_resources/skins/Smartphone/barometer.html.tmpl` & `weewx-5.0.0b1/bin/wee_resources/skins/Smartphone/barometer.html.tmpl`

 * *Files identical despite different names*

### Comparing `weewx-5.0.0a30/bin/wee_resources/skins/Smartphone/favicon.ico` & `weewx-5.0.0b1/bin/wee_resources/skins/Smartphone/favicon.ico`

 * *Files identical despite different names*

### Comparing `weewx-5.0.0a30/bin/wee_resources/skins/Smartphone/humidity.html.tmpl` & `weewx-5.0.0b1/bin/wee_resources/skins/Smartphone/humidity.html.tmpl`

 * *Files identical despite different names*

### Comparing `weewx-5.0.0a30/bin/wee_resources/skins/Smartphone/icons/icon_ipad_x1.png` & `weewx-5.0.0b1/bin/wee_resources/skins/Smartphone/icons/icon_ipad_x1.png`

 * *Files identical despite different names*

### Comparing `weewx-5.0.0a30/bin/wee_resources/skins/Smartphone/icons/icon_ipad_x2.png` & `weewx-5.0.0b1/bin/wee_resources/skins/Smartphone/icons/icon_ipad_x2.png`

 * *Files identical despite different names*

### Comparing `weewx-5.0.0a30/bin/wee_resources/skins/Smartphone/icons/icon_iphone_x1.png` & `weewx-5.0.0b1/bin/wee_resources/skins/Smartphone/icons/icon_iphone_x1.png`

 * *Files identical despite different names*

### Comparing `weewx-5.0.0a30/bin/wee_resources/skins/Smartphone/icons/icon_iphone_x2.png` & `weewx-5.0.0b1/bin/wee_resources/skins/Smartphone/icons/icon_iphone_x2.png`

 * *Files identical despite different names*

### Comparing `weewx-5.0.0a30/bin/wee_resources/skins/Smartphone/index.html.tmpl` & `weewx-5.0.0b1/bin/wee_resources/skins/Smartphone/index.html.tmpl`

 * *Files identical despite different names*

### Comparing `weewx-5.0.0a30/bin/wee_resources/skins/Smartphone/lang/de.conf` & `weewx-5.0.0b1/bin/wee_resources/skins/Smartphone/lang/de.conf`

 * *Files identical despite different names*

### Comparing `weewx-5.0.0a30/bin/wee_resources/skins/Smartphone/lang/en.conf` & `weewx-5.0.0b1/bin/wee_resources/skins/Smartphone/lang/en.conf`

 * *Files identical despite different names*

### Comparing `weewx-5.0.0a30/bin/wee_resources/skins/Smartphone/lang/nl.conf` & `weewx-5.0.0b1/bin/wee_resources/skins/Smartphone/lang/nl.conf`

 * *Files identical despite different names*

### Comparing `weewx-5.0.0a30/bin/wee_resources/skins/Smartphone/lang/no.conf` & `weewx-5.0.0b1/bin/wee_resources/skins/Smartphone/lang/no.conf`

 * *Files identical despite different names*

### Comparing `weewx-5.0.0a30/bin/wee_resources/skins/Smartphone/rain.html.tmpl` & `weewx-5.0.0b1/bin/wee_resources/skins/Smartphone/rain.html.tmpl`

 * *Files identical despite different names*

### Comparing `weewx-5.0.0a30/bin/wee_resources/skins/Smartphone/skin.conf` & `weewx-5.0.0b1/bin/wee_resources/skins/Smartphone/skin.conf`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 # configuration file for Smartphone skin
 
 SKIN_NAME = Smartphone
-SKIN_VERSION = 5.0.0a30
+SKIN_VERSION = 5.0.0b1
 
 [Extras]
     # Set this URL to display a radar image
     #radar_img = http://radar.weather.gov/ridge/lite/N0R/RTX_loop.gif
     # Set this URL for the radar image link
     #radar_url = http://radar.weather.gov/ridge/radar.php?product=NCR&rid=RTX&loop=yes
```

### Comparing `weewx-5.0.0a30/bin/wee_resources/skins/Smartphone/temp.html.tmpl` & `weewx-5.0.0b1/bin/wee_resources/skins/Smartphone/temp.html.tmpl`

 * *Files identical despite different names*

### Comparing `weewx-5.0.0a30/bin/wee_resources/skins/Smartphone/wind.html.tmpl` & `weewx-5.0.0b1/bin/wee_resources/skins/Smartphone/wind.html.tmpl`

 * *Files identical despite different names*

### Comparing `weewx-5.0.0a30/bin/wee_resources/skins/Standard/NOAA/NOAA-%Y-%m.txt.tmpl` & `weewx-5.0.0b1/bin/wee_resources/skins/Standard/NOAA/NOAA-%Y-%m.txt.tmpl`

 * *Files identical despite different names*

### Comparing `weewx-5.0.0a30/bin/wee_resources/skins/Standard/NOAA/NOAA-%Y.txt.tmpl` & `weewx-5.0.0b1/bin/wee_resources/skins/Standard/NOAA/NOAA-%Y.txt.tmpl`

 * *Files identical despite different names*

### Comparing `weewx-5.0.0a30/bin/wee_resources/skins/Standard/RSS/weewx_rss.xml.tmpl` & `weewx-5.0.0b1/bin/wee_resources/skins/Standard/RSS/weewx_rss.xml.tmpl`

 * *Files identical despite different names*

### Comparing `weewx-5.0.0a30/bin/wee_resources/skins/Standard/backgrounds/butterfly.jpg` & `weewx-5.0.0b1/bin/wee_resources/skins/Standard/backgrounds/butterfly.jpg`

 * *Files identical despite different names*

### Comparing `weewx-5.0.0a30/bin/wee_resources/skins/Standard/backgrounds/drops.gif` & `weewx-5.0.0b1/bin/wee_resources/skins/Standard/backgrounds/drops.gif`

 * *Files identical despite different names*

### Comparing `weewx-5.0.0a30/bin/wee_resources/skins/Standard/backgrounds/flower.jpg` & `weewx-5.0.0b1/bin/wee_resources/skins/Standard/backgrounds/flower.jpg`

 * *Files identical despite different names*

### Comparing `weewx-5.0.0a30/bin/wee_resources/skins/Standard/backgrounds/leaf.jpg` & `weewx-5.0.0b1/bin/wee_resources/skins/Standard/backgrounds/leaf.jpg`

 * *Files identical despite different names*

### Comparing `weewx-5.0.0a30/bin/wee_resources/skins/Standard/backgrounds/night.gif` & `weewx-5.0.0b1/bin/wee_resources/skins/Standard/backgrounds/night.gif`

 * *Files identical despite different names*

### Comparing `weewx-5.0.0a30/bin/wee_resources/skins/Standard/favicon.ico` & `weewx-5.0.0b1/bin/wee_resources/skins/Standard/favicon.ico`

 * *Files identical despite different names*

### Comparing `weewx-5.0.0a30/bin/wee_resources/skins/Standard/font/DejaVuSansMono-Bold.ttf` & `weewx-5.0.0b1/bin/wee_resources/skins/Standard/font/DejaVuSansMono-Bold.ttf`

 * *Files identical despite different names*

### Comparing `weewx-5.0.0a30/bin/wee_resources/skins/Standard/index.html.tmpl` & `weewx-5.0.0b1/bin/wee_resources/skins/Standard/index.html.tmpl`

 * *Files identical despite different names*

### Comparing `weewx-5.0.0a30/bin/wee_resources/skins/Standard/lang/de.conf` & `weewx-5.0.0b1/bin/wee_resources/skins/Standard/lang/de.conf`

 * *Files identical despite different names*

### Comparing `weewx-5.0.0a30/bin/wee_resources/skins/Standard/lang/en.conf` & `weewx-5.0.0b1/bin/wee_resources/skins/Standard/lang/en.conf`

 * *Files identical despite different names*

### Comparing `weewx-5.0.0a30/bin/wee_resources/skins/Standard/lang/fr.conf` & `weewx-5.0.0b1/bin/wee_resources/skins/Standard/lang/fr.conf`

 * *Files identical despite different names*

### Comparing `weewx-5.0.0a30/bin/wee_resources/skins/Standard/lang/nl.conf` & `weewx-5.0.0b1/bin/wee_resources/skins/Standard/lang/nl.conf`

 * *Files identical despite different names*

### Comparing `weewx-5.0.0a30/bin/wee_resources/skins/Standard/lang/no.conf` & `weewx-5.0.0b1/bin/wee_resources/skins/Standard/lang/no.conf`

 * *Files identical despite different names*

### Comparing `weewx-5.0.0a30/bin/wee_resources/skins/Standard/month.html.tmpl` & `weewx-5.0.0b1/bin/wee_resources/skins/Standard/month.html.tmpl`

 * *Files identical despite different names*

### Comparing `weewx-5.0.0a30/bin/wee_resources/skins/Standard/skin.conf` & `weewx-5.0.0b1/bin/wee_resources/skins/Standard/skin.conf`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 ###############################################################################
 # STANDARD SKIN CONFIGURATION FILE                                            #
 # Copyright (c) 2010-2021 Tom Keffer <tkeffer@gmail.com>                      #
 # See the file LICENSE.txt for your rights.                                   #
 ###############################################################################
 
 SKIN_NAME = Standard
-SKIN_VERSION = 5.0.0a30
+SKIN_VERSION = 5.0.0b1
 
 ###############################################################################
 
 # The following section is for any extra tags that you want to be available in the templates
 [Extras]
     
     # This radar image would be available as $Extras.radar_img
```

### Comparing `weewx-5.0.0a30/bin/wee_resources/skins/Standard/smartphone/barometer.html.tmpl` & `weewx-5.0.0b1/bin/wee_resources/skins/Standard/smartphone/barometer.html.tmpl`

 * *Files identical despite different names*

### Comparing `weewx-5.0.0a30/bin/wee_resources/skins/Standard/smartphone/humidity.html.tmpl` & `weewx-5.0.0b1/bin/wee_resources/skins/Standard/smartphone/humidity.html.tmpl`

 * *Files identical despite different names*

### Comparing `weewx-5.0.0a30/bin/wee_resources/skins/Standard/smartphone/icons/icon_ipad_x1.png` & `weewx-5.0.0b1/bin/wee_resources/skins/Standard/smartphone/icons/icon_ipad_x1.png`

 * *Files identical despite different names*

### Comparing `weewx-5.0.0a30/bin/wee_resources/skins/Standard/smartphone/icons/icon_ipad_x2.png` & `weewx-5.0.0b1/bin/wee_resources/skins/Standard/smartphone/icons/icon_ipad_x2.png`

 * *Files identical despite different names*

### Comparing `weewx-5.0.0a30/bin/wee_resources/skins/Standard/smartphone/icons/icon_iphone_x1.png` & `weewx-5.0.0b1/bin/wee_resources/skins/Standard/smartphone/icons/icon_iphone_x1.png`

 * *Files identical despite different names*

### Comparing `weewx-5.0.0a30/bin/wee_resources/skins/Standard/smartphone/icons/icon_iphone_x2.png` & `weewx-5.0.0b1/bin/wee_resources/skins/Standard/smartphone/icons/icon_iphone_x2.png`

 * *Files identical despite different names*

### Comparing `weewx-5.0.0a30/bin/wee_resources/skins/Standard/smartphone/index.html.tmpl` & `weewx-5.0.0b1/bin/wee_resources/skins/Standard/smartphone/index.html.tmpl`

 * *Files identical despite different names*

### Comparing `weewx-5.0.0a30/bin/wee_resources/skins/Standard/smartphone/radar.html.tmpl` & `weewx-5.0.0b1/bin/wee_resources/skins/Standard/smartphone/radar.html.tmpl`

 * *Files identical despite different names*

### Comparing `weewx-5.0.0a30/bin/wee_resources/skins/Standard/smartphone/rain.html.tmpl` & `weewx-5.0.0b1/bin/wee_resources/skins/Standard/smartphone/rain.html.tmpl`

 * *Files identical despite different names*

### Comparing `weewx-5.0.0a30/bin/wee_resources/skins/Standard/smartphone/temp_outside.html.tmpl` & `weewx-5.0.0b1/bin/wee_resources/skins/Standard/smartphone/temp_outside.html.tmpl`

 * *Files identical despite different names*

### Comparing `weewx-5.0.0a30/bin/wee_resources/skins/Standard/smartphone/wind.html.tmpl` & `weewx-5.0.0b1/bin/wee_resources/skins/Standard/smartphone/wind.html.tmpl`

 * *Files identical despite different names*

### Comparing `weewx-5.0.0a30/bin/wee_resources/skins/Standard/week.html.tmpl` & `weewx-5.0.0b1/bin/wee_resources/skins/Standard/week.html.tmpl`

 * *Files identical despite different names*

### Comparing `weewx-5.0.0a30/bin/wee_resources/skins/Standard/weewx.css` & `weewx-5.0.0b1/bin/wee_resources/skins/Standard/weewx.css`

 * *Files identical despite different names*

### Comparing `weewx-5.0.0a30/bin/wee_resources/skins/Standard/year.html.tmpl` & `weewx-5.0.0b1/bin/wee_resources/skins/Standard/year.html.tmpl`

 * *Files identical despite different names*

### Comparing `weewx-5.0.0a30/bin/wee_resources/util/init.d/weewx-multi` & `weewx-5.0.0b1/bin/wee_resources/util/init.d/weewx-multi`

 * *Files identical despite different names*

### Comparing `weewx-5.0.0a30/bin/wee_resources/util/init.d/weewx.bsd` & `weewx-5.0.0b1/bin/wee_resources/util/init.d/weewx.bsd`

 * *Files identical despite different names*

### Comparing `weewx-5.0.0a30/bin/wee_resources/util/init.d/weewx.debian` & `weewx-5.0.0b1/bin/wee_resources/util/init.d/weewx.debian`

 * *Files identical despite different names*

### Comparing `weewx-5.0.0a30/bin/wee_resources/util/init.d/weewx.freebsd` & `weewx-5.0.0b1/bin/wee_resources/util/init.d/weewx.freebsd`

 * *Files identical despite different names*

### Comparing `weewx-5.0.0a30/bin/wee_resources/util/init.d/weewx.lsb` & `weewx-5.0.0b1/bin/wee_resources/util/init.d/weewx.lsb`

 * *Files identical despite different names*

### Comparing `weewx-5.0.0a30/bin/wee_resources/util/init.d/weewx.redhat` & `weewx-5.0.0b1/bin/wee_resources/util/init.d/weewx.redhat`

 * *Files identical despite different names*

### Comparing `weewx-5.0.0a30/bin/wee_resources/util/init.d/weewx.suse` & `weewx-5.0.0b1/bin/wee_resources/util/init.d/weewx.suse`

 * *Files identical despite different names*

### Comparing `weewx-5.0.0a30/bin/wee_resources/util/launchd/com.weewx.weewxd.plist` & `weewx-5.0.0b1/bin/wee_resources/util/launchd/com.weewx.weewxd.plist`

 * *Files identical despite different names*

### Comparing `weewx-5.0.0a30/bin/wee_resources/util/systemd/weewx.service` & `weewx-5.0.0b1/bin/wee_resources/util/systemd/weewx.service`

 * *Files identical despite different names*

### Comparing `weewx-5.0.0a30/bin/wee_resources/weewx.conf` & `weewx-5.0.0b1/bin/wee_resources/weewx.conf`

 * *Files 1% similar despite different names*

```diff
@@ -16,15 +16,15 @@
 # Whether to log successful operations. May get overridden below.
 log_success = True
 
 # Whether to log unsuccessful operations. May get overridden below.
 log_failure = True
 
 # Do not modify this. It is used when installing and updating weewx.
-version = 5.0.0a30
+version = 5.0.0b1
 
 ##############################################################################
 
 #   This section is for information about the station.
 
 [Station]
```

### Comparing `weewx-5.0.0a30/bin/weecfg/__init__.py` & `weewx-5.0.0b1/bin/weecfg/__init__.py`

 * *Files identical despite different names*

### Comparing `weewx-5.0.0a30/bin/weecfg/database.py` & `weewx-5.0.0b1/bin/weecfg/database.py`

 * *Files identical despite different names*

### Comparing `weewx-5.0.0a30/bin/weecfg/extension.py` & `weewx-5.0.0b1/bin/weecfg/extension.py`

 * *Files identical despite different names*

### Comparing `weewx-5.0.0a30/bin/weecfg/station_config.py` & `weewx-5.0.0b1/bin/weecfg/station_config.py`

 * *Files identical despite different names*

### Comparing `weewx-5.0.0a30/bin/weecfg/update_config.py` & `weewx-5.0.0b1/bin/weecfg/update_config.py`

 * *Files identical despite different names*

### Comparing `weewx-5.0.0a30/bin/weectl.py` & `weewx-5.0.0b1/bin/weectl.py`

 * *Files identical despite different names*

### Comparing `weewx-5.0.0a30/bin/weectllib/parse_extension.py` & `weewx-5.0.0b1/bin/weectllib/parse_extension.py`

 * *Files identical despite different names*

### Comparing `weewx-5.0.0a30/bin/weectllib/parse_station.py` & `weewx-5.0.0b1/bin/weectllib/parse_station.py`

 * *Files identical despite different names*

### Comparing `weewx-5.0.0a30/bin/weedb/NOTES.md` & `weewx-5.0.0b1/bin/weedb/NOTES.md`

 * *Files identical despite different names*

### Comparing `weewx-5.0.0a30/bin/weedb/__init__.py` & `weewx-5.0.0b1/bin/weedb/__init__.py`

 * *Files identical despite different names*

### Comparing `weewx-5.0.0a30/bin/weedb/mysql.py` & `weewx-5.0.0b1/bin/weedb/mysql.py`

 * *Files identical despite different names*

### Comparing `weewx-5.0.0a30/bin/weedb/sqlite.py` & `weewx-5.0.0b1/bin/weedb/sqlite.py`

 * *Files identical despite different names*

### Comparing `weewx-5.0.0a30/bin/weeimport/csvimport.py` & `weewx-5.0.0b1/bin/weeimport/csvimport.py`

 * *Files identical despite different names*

### Comparing `weewx-5.0.0a30/bin/weeimport/cumulusimport.py` & `weewx-5.0.0b1/bin/weeimport/cumulusimport.py`

 * *Files identical despite different names*

### Comparing `weewx-5.0.0a30/bin/weeimport/wdimport.py` & `weewx-5.0.0b1/bin/weeimport/wdimport.py`

 * *Files identical despite different names*

### Comparing `weewx-5.0.0a30/bin/weeimport/weathercatimport.py` & `weewx-5.0.0b1/bin/weeimport/weathercatimport.py`

 * *Files identical despite different names*

### Comparing `weewx-5.0.0a30/bin/weeimport/weeimport.py` & `weewx-5.0.0b1/bin/weeimport/weeimport.py`

 * *Files identical despite different names*

### Comparing `weewx-5.0.0a30/bin/weeimport/wuimport.py` & `weewx-5.0.0b1/bin/weeimport/wuimport.py`

 * *Files identical despite different names*

### Comparing `weewx-5.0.0a30/bin/weeplot/genplot.py` & `weewx-5.0.0b1/bin/weeplot/genplot.py`

 * *Files identical despite different names*

### Comparing `weewx-5.0.0a30/bin/weeplot/utilities.py` & `weewx-5.0.0b1/bin/weeplot/utilities.py`

 * *Files identical despite different names*

### Comparing `weewx-5.0.0a30/bin/weeutil/Moon.py` & `weewx-5.0.0b1/bin/weeutil/Moon.py`

 * *Files identical despite different names*

### Comparing `weewx-5.0.0a30/bin/weeutil/Sun.py` & `weewx-5.0.0b1/bin/weeutil/Sun.py`

 * *Files identical despite different names*

### Comparing `weewx-5.0.0a30/bin/weeutil/config.py` & `weewx-5.0.0b1/bin/weeutil/config.py`

 * *Files identical despite different names*

### Comparing `weewx-5.0.0a30/bin/weeutil/ftpupload.py` & `weewx-5.0.0b1/bin/weeutil/ftpupload.py`

 * *Files identical despite different names*

### Comparing `weewx-5.0.0a30/bin/weeutil/log.py` & `weewx-5.0.0b1/bin/weeutil/log.py`

 * *Files identical despite different names*

### Comparing `weewx-5.0.0a30/bin/weeutil/logger.py` & `weewx-5.0.0b1/bin/weeutil/logger.py`

 * *Files identical despite different names*

### Comparing `weewx-5.0.0a30/bin/weeutil/rsyncupload.py` & `weewx-5.0.0b1/bin/weeutil/rsyncupload.py`

 * *Files identical despite different names*

### Comparing `weewx-5.0.0a30/bin/weeutil/timediff.py` & `weewx-5.0.0b1/bin/weeutil/timediff.py`

 * *Files identical despite different names*

### Comparing `weewx-5.0.0a30/bin/weeutil/weeutil.py` & `weewx-5.0.0b1/bin/weeutil/weeutil.py`

 * *Files identical despite different names*

### Comparing `weewx-5.0.0a30/bin/weewx/__init__.py` & `weewx-5.0.0b1/bin/weewx/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 #    See the file LICENSE.txt for your full rights.
 #
 """Package weewx, containing modules specific to the weewx runtime engine."""
 import os.path
 import sys
 import time
 
-__version__ = "5.0.0a30"
+__version__ = "5.0.0b1"
 
 # Holds the program launch time in unix epoch seconds:
 # Useful for calculating 'uptime.'
 launchtime_ts = time.time()
 
 # Set to true for extra debug information:
 debug = False
```

### Comparing `weewx-5.0.0a30/bin/weewx/accum.py` & `weewx-5.0.0b1/bin/weewx/accum.py`

 * *Files identical despite different names*

### Comparing `weewx-5.0.0a30/bin/weewx/almanac.py` & `weewx-5.0.0b1/bin/weewx/almanac.py`

 * *Files identical despite different names*

### Comparing `weewx-5.0.0a30/bin/weewx/cheetahgenerator.py` & `weewx-5.0.0b1/bin/weewx/cheetahgenerator.py`

 * *Files identical despite different names*

### Comparing `weewx-5.0.0a30/bin/weewx/crc16.py` & `weewx-5.0.0b1/bin/weewx/crc16.py`

 * *Files identical despite different names*

### Comparing `weewx-5.0.0a30/bin/weewx/daemon.py` & `weewx-5.0.0b1/bin/weewx/daemon.py`

 * *Files identical despite different names*

### Comparing `weewx-5.0.0a30/bin/weewx/defaults.py` & `weewx-5.0.0b1/bin/weewx/defaults.py`

 * *Files identical despite different names*

### Comparing `weewx-5.0.0a30/bin/weewx/drivers/__init__.py` & `weewx-5.0.0b1/bin/weewx/drivers/__init__.py`

 * *Files identical despite different names*

### Comparing `weewx-5.0.0a30/bin/weewx/drivers/acurite.py` & `weewx-5.0.0b1/bin/weewx/drivers/acurite.py`

 * *Files identical despite different names*

### Comparing `weewx-5.0.0a30/bin/weewx/drivers/cc3000.py` & `weewx-5.0.0b1/bin/weewx/drivers/cc3000.py`

 * *Files identical despite different names*

### Comparing `weewx-5.0.0a30/bin/weewx/drivers/fousb.py` & `weewx-5.0.0b1/bin/weewx/drivers/fousb.py`

 * *Files identical despite different names*

### Comparing `weewx-5.0.0a30/bin/weewx/drivers/simulator.py` & `weewx-5.0.0b1/bin/weewx/drivers/simulator.py`

 * *Files identical despite different names*

### Comparing `weewx-5.0.0a30/bin/weewx/drivers/te923.py` & `weewx-5.0.0b1/bin/weewx/drivers/te923.py`

 * *Files identical despite different names*

### Comparing `weewx-5.0.0a30/bin/weewx/drivers/ultimeter.py` & `weewx-5.0.0b1/bin/weewx/drivers/ultimeter.py`

 * *Files identical despite different names*

### Comparing `weewx-5.0.0a30/bin/weewx/drivers/vantage.py` & `weewx-5.0.0b1/bin/weewx/drivers/vantage.py`

 * *Files identical despite different names*

### Comparing `weewx-5.0.0a30/bin/weewx/drivers/wmr100.py` & `weewx-5.0.0b1/bin/weewx/drivers/wmr100.py`

 * *Files identical despite different names*

### Comparing `weewx-5.0.0a30/bin/weewx/drivers/wmr300.py` & `weewx-5.0.0b1/bin/weewx/drivers/wmr300.py`

 * *Files identical despite different names*

### Comparing `weewx-5.0.0a30/bin/weewx/drivers/wmr9x8.py` & `weewx-5.0.0b1/bin/weewx/drivers/wmr9x8.py`

 * *Files identical despite different names*

### Comparing `weewx-5.0.0a30/bin/weewx/drivers/ws1.py` & `weewx-5.0.0b1/bin/weewx/drivers/ws1.py`

 * *Files identical despite different names*

### Comparing `weewx-5.0.0a30/bin/weewx/drivers/ws23xx.py` & `weewx-5.0.0b1/bin/weewx/drivers/ws23xx.py`

 * *Files identical despite different names*

### Comparing `weewx-5.0.0a30/bin/weewx/drivers/ws28xx.py` & `weewx-5.0.0b1/bin/weewx/drivers/ws28xx.py`

 * *Files identical despite different names*

### Comparing `weewx-5.0.0a30/bin/weewx/engine.py` & `weewx-5.0.0b1/bin/weewx/engine.py`

 * *Files identical despite different names*

### Comparing `weewx-5.0.0a30/bin/weewx/imagegenerator.py` & `weewx-5.0.0b1/bin/weewx/imagegenerator.py`

 * *Files identical despite different names*

### Comparing `weewx-5.0.0a30/bin/weewx/manager.py` & `weewx-5.0.0b1/bin/weewx/manager.py`

 * *Files identical despite different names*

### Comparing `weewx-5.0.0a30/bin/weewx/qc.py` & `weewx-5.0.0b1/bin/weewx/qc.py`

 * *Files identical despite different names*

### Comparing `weewx-5.0.0a30/bin/weewx/reportengine.py` & `weewx-5.0.0b1/bin/weewx/reportengine.py`

 * *Files identical despite different names*

### Comparing `weewx-5.0.0a30/bin/weewx/restx.py` & `weewx-5.0.0b1/bin/weewx/restx.py`

 * *Files identical despite different names*

### Comparing `weewx-5.0.0a30/bin/weewx/station.py` & `weewx-5.0.0b1/bin/weewx/station.py`

 * *Files identical despite different names*

### Comparing `weewx-5.0.0a30/bin/weewx/tags.py` & `weewx-5.0.0b1/bin/weewx/tags.py`

 * *Files identical despite different names*

### Comparing `weewx-5.0.0a30/bin/weewx/units.py` & `weewx-5.0.0b1/bin/weewx/units.py`

 * *Files identical despite different names*

### Comparing `weewx-5.0.0a30/bin/weewx/uwxutils.py` & `weewx-5.0.0b1/bin/weewx/uwxutils.py`

 * *Files identical despite different names*

### Comparing `weewx-5.0.0a30/bin/weewx/wxformulas.py` & `weewx-5.0.0b1/bin/weewx/wxformulas.py`

 * *Files identical despite different names*

### Comparing `weewx-5.0.0a30/bin/weewx/wxservices.py` & `weewx-5.0.0b1/bin/weewx/wxservices.py`

 * *Files identical despite different names*

### Comparing `weewx-5.0.0a30/bin/weewx/wxxtypes.py` & `weewx-5.0.0b1/bin/weewx/wxxtypes.py`

 * *Files identical despite different names*

### Comparing `weewx-5.0.0a30/bin/weewx/xtypes.py` & `weewx-5.0.0b1/bin/weewx/xtypes.py`

 * *Files identical despite different names*

### Comparing `weewx-5.0.0a30/bin/weewxd.py` & `weewx-5.0.0b1/bin/weewxd.py`

 * *Files identical despite different names*

### Comparing `weewx-5.0.0a30/bin/wunderfixer.py` & `weewx-5.0.0b1/bin/wunderfixer.py`

 * *Files identical despite different names*

### Comparing `weewx-5.0.0a30/pkg/changelog.el` & `weewx-5.0.0b1/pkg/changelog.el`

 * *Files 5% similar despite different names*

```diff
@@ -1,7 +1,13 @@
+* Sat May 06 2023 Matthew Wall (weewx) <mwall@users.sourceforge.net> - 5.0.0b1-1
+- new upstream release
+* Sat May 06 2023 Matthew Wall (weewx) <mwall@users.sourceforge.net> - 5.0.0a30-1
+- new upstream release
+* Fri May 05 2023 Matthew Wall (weewx) <mwall@users.sourceforge.net> - 5.0.0a29-1
+- new upstream release
 * Wed Feb 22 2023 Thomas Keffer (Author of weewx) <tkeffer@gmail.com> - 4.10.2-1
 - new upstream release
 * Mon Jan 30 2023 Matthew Wall (weewx) <mwall@users.sourceforge.net> - 4.10.1-1
 - new upstream release
 * Sun Jan 29 2023 Matthew Wall (weewx) <mwall@users.sourceforge.net> - 4.10.0-1
 - new upstream release
 * Tue Oct 25 2022 Thomas Keffer (Author of weewx) <tkeffer@gmail.com> - 4.9.1-1
```

### Comparing `weewx-5.0.0a30/pkg/changelog.suse` & `weewx-5.0.0b1/pkg/changelog.suse`

 * *Files 8% similar despite different names*

```diff
@@ -1,7 +1,13 @@
+* Sat May 06 2023 Matthew Wall (weewx) <mwall@users.sourceforge.net> - 5.0.0b1-1
+- new upstream release
+* Sat May 06 2023 Matthew Wall (weewx) <mwall@users.sourceforge.net> - 5.0.0a30-1
+- new upstream release
+* Fri May 05 2023 Matthew Wall (weewx) <mwall@users.sourceforge.net> - 5.0.0a29-1
+- new upstream release
 * Wed Feb 22 2023 Thomas Keffer (Author of weewx) <tkeffer@gmail.com> - 4.10.2-1
 - new upstream release
 * Mon Jan 30 2023 Matthew Wall (weewx) <mwall@users.sourceforge.net> - 4.10.1-1
 - new upstream release
 * Sun Jan 29 2023 Matthew Wall (weewx) <mwall@users.sourceforge.net> - 4.10.0-1
 - new upstream release
 * Tue Oct 25 2022 Thomas Keffer (Author of weewx) <tkeffer@gmail.com> - 4.9.1-1
```

### Comparing `weewx-5.0.0a30/pkg/debian/README` & `weewx-5.0.0b1/pkg/debian/README`

 * *Files identical despite different names*

### Comparing `weewx-5.0.0a30/pkg/debian/changelog` & `weewx-5.0.0b1/pkg/debian/changelog`

 * *Files 0% similar despite different names*

```diff
@@ -1,7 +1,16 @@
+weewx (5.0.0b1-1) unstable; urgency=low
+  * new upstream release
+ -- Matthew Wall (weewx) <mwall@users.sourceforge.net>  Sat, 06 May 2023 07:35:56 -0400
+weewx (5.0.0a30-1) unstable; urgency=low
+  * Back up skins individually, instead of the whole directory.
+ -- Thomas Keffer (Author of weewx) <tkeffer@gmail.com>  Fri, 05 May 2023 11:28:04 -0700
+weewx (5.0.0a29-1) unstable; urgency=low
+  * new upstream release
+ -- Matthew Wall (weewx) <mwall@users.sourceforge.net>  Fri, 05 May 2023 13:35:31 -0400
 weewx (5.0.0a28-1) unstable; urgency=low
   * Use flag --config-only to upgrade config file
  -- Thomas Keffer (Author of weewx) <tkeffer@gmail.com>  Fri, 07 Apr 2023 05:36:56 -0700
 weewx (5.0.0a27-1) unstable; urgency=low
   * Fix bug in postinst
  -- Thomas Keffer (Author of weewx) <tkeffer@gmail.com>  Wed, 29 Mar 2023 14:47:50 -0700
 weewx (5.0.0a26-1) unstable; urgency=low
```

### Comparing `weewx-5.0.0a30/pkg/debian/config` & `weewx-5.0.0b1/pkg/debian/config`

 * *Files identical despite different names*

### Comparing `weewx-5.0.0a30/pkg/debian/control` & `weewx-5.0.0b1/pkg/debian/control`

 * *Files identical despite different names*

### Comparing `weewx-5.0.0a30/pkg/debian/copyright` & `weewx-5.0.0b1/pkg/debian/copyright`

 * *Files identical despite different names*

### Comparing `weewx-5.0.0a30/pkg/debian/postinst` & `weewx-5.0.0b1/pkg/debian/postinst`

 * *Files identical despite different names*

### Comparing `weewx-5.0.0a30/pkg/debian/postrm` & `weewx-5.0.0b1/pkg/debian/postrm`

 * *Files identical despite different names*

### Comparing `weewx-5.0.0a30/pkg/debian/prerm` & `weewx-5.0.0b1/pkg/debian/prerm`

 * *Files identical despite different names*

### Comparing `weewx-5.0.0a30/pkg/debian/rules` & `weewx-5.0.0b1/pkg/debian/rules`

 * *Files 5% similar despite different names*

```diff
@@ -40,35 +40,35 @@
 	mkdir -p $(DST_BINDIR)
 	mkdir -p $(DST_DOCDIR)
 	mkdir -p $(DST_CFGDIR)
 	mkdir -p $(DST)/etc/default
 
 # copy files from the source tree
 	cp -r $(SRC)/bin/* $(DST_BINDIR)
-	cp -r $(SRC)/docs/* $(DST_DOCDIR)
+	cp -r $(SRC)/../docs/* $(DST_DOCDIR)
 	cp -r $(SRC)/examples $(DST_DOCDIR)
 	cp -r $(SRC)/skins $(DST_CFGDIR)
 	cp -r $(SRC)/util/apache $(DST_CFGDIR)
 	cp -r $(SRC)/util/import $(DST_CFGDIR)
 	cp -r $(SRC)/util/logrotate.d $(DST_CFGDIR)
 	cp -r $(SRC)/util/logwatch $(DST_CFGDIR)
 	cp -r $(SRC)/util/rsyslog.d $(DST_CFGDIR)
 	cp -r $(SRC)/util/scripts $(DST_CFGDIR)
 	cp -r $(SRC)/util/udev $(DST_CFGDIR)
 
-    # Patch weewx.conf with the various ROOT symbols
+# Patch weewx.conf with the various ROOT symbols
 	cat $(SRC)/weewx.conf | sed \
  -e 's%^WEEWX_ROOT =.*%WEEWX_ROOT = /etc/weewx%' \
  -e 's%SKIN_ROOT =.*%SKIN_ROOT = skins%' \
  -e 's%HTML_ROOT = public_html%HTML_ROOT = /var/www/html/weewx%' \
  -e 's%SQLITE_ROOT = .*%SQLITE_ROOT = /var/lib/weewx%' \
  > $(DST_CFGDIR)/weewx.conf
 
-	# Patch the weewx.service file to read /etd/default/weewx, then
-	# use its symbols to invoke weewxd
+# Patch the weewx.service file to read /etd/default/weewx, then
+# use its symbols to invoke weewxd
 	cat $(SRC)/util/systemd/weewx.service | sed \
  -e '/^\[Service\]/a EnvironmentFile=/etc/default/weewx' \
  -e 's%^ExecStart=.*%ExecStart=/usr/bin/env $${WEEWX_BIN} $${WEEWX_CFG}%' \
  > $(DST_SYSTEMDDIR)/weewx.service
 
 # make a virgin copy of the configuration file
 	cp $(DST_CFGDIR)/weewx.conf $(DST_CFGDIR)/weewx.conf.dist
```

### Comparing `weewx-5.0.0a30/pkg/debian/templates` & `weewx-5.0.0b1/pkg/debian/templates`

 * *Files identical despite different names*

### Comparing `weewx-5.0.0a30/pkg/index-apt.html` & `weewx-5.0.0b1/pkg/index-apt.html`

 * *Files identical despite different names*

### Comparing `weewx-5.0.0a30/pkg/index-suse.html` & `weewx-5.0.0b1/pkg/index-suse.html`

 * *Files identical despite different names*

### Comparing `weewx-5.0.0a30/pkg/index-yum.html` & `weewx-5.0.0b1/pkg/index-yum.html`

 * *Files identical despite different names*

### Comparing `weewx-5.0.0a30/pkg/mkchangelog.pl` & `weewx-5.0.0b1/pkg/mkchangelog.pl`

 * *Files identical despite different names*

### Comparing `weewx-5.0.0a30/pkg/weewx.smf` & `weewx-5.0.0b1/pkg/weewx.smf`

 * *Files identical despite different names*

### Comparing `weewx-5.0.0a30/pkg/weewx.spec.in` & `weewx-5.0.0b1/pkg/weewx.spec.in`

 * *Files 4% similar despite different names*

```diff
@@ -33,29 +33,14 @@
 %define initdir /etc/systemd/system
 #define initdir /etc/init.d
 %define deps python , python-configobj , python-cheetah , python-imaging , python-pyserial, python-usb
 %define html_root /srv/www/htdocs/weewx
 %define python python
 %endif
 
-# rh7: python2 on redhat, fedora, centos
-%if "%{_vendor}" == "redhat" && "%{os_target}" == "7"
-%define relos .el7
-%define platform redhat
-%define initdir %{_initrddir}
-# must install pyserial and pyusb using easy_install or pip
-%define deps python, python-setuptools, python-configobj, python-cheetah, python-imaging
-%define python python2
-%define html_root /var/www/html/weewx
-# Disable Fedora's shebang mangling script,
-# which errors out on any file with versionless `python` in its shebang
-# See: https://github.com/atom/atom/issues/21937
-%undefine __brp_mangle_shebangs
-%endif
-
 # rh8: python3 on redhat, fedora, centos
 %if "%{_vendor}" == "redhat" && "%{os_target}" == "8"
 %define relos .el8
 %define platform redhat
 %define initdir %{_initrddir}
 # must install cheetah from epel-release or using pip3
 %define deps python3, python3-setuptools, python3-configobj, python3-pillow, python3-pyserial, python3-pyusb
@@ -109,15 +94,15 @@
 mkdir -p %{buildroot}%{dst_doc_dir}
 mkdir -p %{buildroot}%{dst_cfg_dir}
 mkdir -p %{buildroot}%{initdir}
 mkdir -p %{buildroot}/etc/default
 
 # copy files from the source tree
 cp -r bin/* %{buildroot}%{dst_bin_dir}
-cp -r docs/* %{buildroot}%{dst_doc_dir}
+cp -r ../../docs/* %{buildroot}%{dst_doc_dir}
 cp -r examples %{buildroot}%{dst_doc_dir}
 cp -r skins %{buildroot}%{dst_cfg_dir}
 cp -r util/apache %{buildroot}%{dst_cfg_dir}
 cp -r util/import %{buildroot}%{dst_cfg_dir}
 cp -r util/logrotate.d %{buildroot}%{dst_cfg_dir}
 cp -r util/logwatch %{buildroot}%{dst_cfg_dir}
 cp -r util/rsyslog.d %{buildroot}%{dst_cfg_dir}
```

### Comparing `weewx-5.0.0a30/pyproject.toml` & `weewx-5.0.0b1/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "weewx"
-version = "5.0.0a30"
+version = "5.0.0b1"
 description = "The WeeWX weather software system. This is an ALPHA release, and is likely to be unstable!"
 authors = ["Tom Keffer <tkeffer@gmail.com>"]
 license = "GPL3"
 readme = 'README.md'
 repository = "https://github.com/weewx/weewx"
 homepage = "https://weewx.com"
 documentation = "https://weewx.com/docs"
```

### Comparing `weewx-5.0.0a30/util/i18n/i18n-report` & `weewx-5.0.0b1/util/i18n/i18n-report`

 * *Files identical despite different names*

### Comparing `weewx-5.0.0a30/util/import/csv-example.conf` & `weewx-5.0.0b1/util/import/csv-example.conf`

 * *Files identical despite different names*

### Comparing `weewx-5.0.0a30/util/import/cumulus-example.conf` & `weewx-5.0.0b1/util/import/cumulus-example.conf`

 * *Files identical despite different names*

### Comparing `weewx-5.0.0a30/util/import/wd-example.conf` & `weewx-5.0.0b1/util/import/wd-example.conf`

 * *Files identical despite different names*

### Comparing `weewx-5.0.0a30/util/import/weathercat-example.conf` & `weewx-5.0.0b1/util/import/weathercat-example.conf`

 * *Files identical despite different names*

### Comparing `weewx-5.0.0a30/util/import/wu-example.conf` & `weewx-5.0.0b1/util/import/wu-example.conf`

 * *Files identical despite different names*

### Comparing `weewx-5.0.0a30/util/init.d/weewx-multi` & `weewx-5.0.0b1/util/init.d/weewx-multi`

 * *Files identical despite different names*

### Comparing `weewx-5.0.0a30/util/init.d/weewx.bsd` & `weewx-5.0.0b1/util/init.d/weewx.bsd`

 * *Files identical despite different names*

### Comparing `weewx-5.0.0a30/util/init.d/weewx.debian` & `weewx-5.0.0b1/util/init.d/weewx.debian`

 * *Files identical despite different names*

### Comparing `weewx-5.0.0a30/util/init.d/weewx.freebsd` & `weewx-5.0.0b1/util/init.d/weewx.freebsd`

 * *Files identical despite different names*

### Comparing `weewx-5.0.0a30/util/init.d/weewx.lsb` & `weewx-5.0.0b1/util/init.d/weewx.lsb`

 * *Files identical despite different names*

### Comparing `weewx-5.0.0a30/util/init.d/weewx.redhat` & `weewx-5.0.0b1/util/init.d/weewx.redhat`

 * *Files identical despite different names*

### Comparing `weewx-5.0.0a30/util/init.d/weewx.suse` & `weewx-5.0.0b1/util/init.d/weewx.suse`

 * *Files identical despite different names*

### Comparing `weewx-5.0.0a30/util/launchd/com.weewx.weewxd.plist` & `weewx-5.0.0b1/util/launchd/com.weewx.weewxd.plist`

 * *Files identical despite different names*

### Comparing `weewx-5.0.0a30/util/logrotate.d/weewx` & `weewx-5.0.0b1/util/logrotate.d/weewx`

 * *Files identical despite different names*

### Comparing `weewx-5.0.0a30/util/logwatch/scripts/services/weewx` & `weewx-5.0.0b1/util/logwatch/scripts/services/weewx`

 * *Files identical despite different names*

### Comparing `weewx-5.0.0a30/util/rsyslog.d/weewx.conf` & `weewx-5.0.0b1/util/rsyslog.d/weewx.conf`

 * *Files identical despite different names*

### Comparing `weewx-5.0.0a30/util/solaris/weewx-smf.xml` & `weewx-5.0.0b1/util/solaris/weewx-smf.xml`

 * *Files identical despite different names*

### Comparing `weewx-5.0.0a30/util/systemd/weewx.service` & `weewx-5.0.0b1/util/systemd/weewx.service`

 * *Files identical despite different names*

### Comparing `weewx-5.0.0a30/util/udev/rules.d/vantage.rules` & `weewx-5.0.0b1/util/udev/rules.d/vantage.rules`

 * *Files identical despite different names*

### Comparing `weewx-5.0.0a30/util/udev/rules.d/weewx.rules` & `weewx-5.0.0b1/util/udev/rules.d/weewx.rules`

 * *Files identical despite different names*

### Comparing `weewx-5.0.0a30/PKG-INFO` & `weewx-5.0.0b1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: weewx
-Version: 5.0.0a30
+Version: 5.0.0b1
 Summary: The WeeWX weather software system. This is an ALPHA release, and is likely to be unstable!
 Home-page: https://weewx.com
 License: GPL3
 Author: Tom Keffer
 Author-email: tkeffer@gmail.com
 Requires-Python: >=3.7,<4.0
 Classifier: Development Status :: 5 - Production/Stable
```

