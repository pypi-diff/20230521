# Comparing `tmp/not1mm-23.5.9.1.tar.gz` & `tmp/not1mm-23.5.9.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "not1mm-23.5.9.1.tar", last modified: Tue May  9 20:15:55 2023, max compression
+gzip compressed data, was "not1mm-23.5.9.2.tar", last modified: Wed May 10 04:06:27 2023, max compression
```

## Comparing `not1mm-23.5.9.1.tar` & `not1mm-23.5.9.2.tar`

### file list

```diff
@@ -1,137 +1,137 @@
-drwxr-xr-x   0 mbridak   (1000) mbridak   (1000)        0 2023-05-09 20:15:55.971519 not1mm-23.5.9.1/
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)    35149 2022-05-05 15:15:13.000000 not1mm-23.5.9.1/LICENSE
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)    25054 2023-05-09 20:15:55.971519 not1mm-23.5.9.1/PKG-INFO
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)    24307 2023-05-09 20:15:01.000000 not1mm-23.5.9.1/README.md
-drwxr-xr-x   0 mbridak   (1000) mbridak   (1000)        0 2023-05-09 20:15:55.944520 not1mm-23.5.9.1/not1mm/
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)        0 2022-11-03 15:04:39.000000 not1mm-23.5.9.1/not1mm/__init__.py
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)    80054 2023-05-09 20:13:32.000000 not1mm-23.5.9.1/not1mm/__main__.py
--rwxr-xr-x   0 mbridak   (1000) mbridak   (1000)    23860 2023-05-09 20:08:28.000000 not1mm-23.5.9.1/not1mm/bandmap.py
-drwxr-xr-x   0 mbridak   (1000) mbridak   (1000)        0 2023-05-09 20:15:55.953520 not1mm-23.5.9.1/not1mm/data/
--rw-rw-rw-   0 mbridak   (1000) mbridak   (1000)    16590 2023-02-15 20:52:35.000000 not1mm-23.5.9.1/not1mm/data/Combinear.qss
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)   203952 2023-01-27 16:44:51.000000 not1mm-23.5.9.1/not1mm/data/JetBrainsMono-Regular.ttf
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)   542666 2023-02-14 19:22:02.000000 not1mm-23.5.9.1/not1mm/data/MASTER.SCP
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)     2352 2023-04-10 21:02:17.000000 not1mm-23.5.9.1/not1mm/data/about.ui
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)      224 2023-04-18 03:49:58.000000 not1mm-23.5.9.1/not1mm/data/alpha bravo charlie delta.txt
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)     5246 2023-05-01 15:41:16.000000 not1mm-23.5.9.1/not1mm/data/bandmap.ui
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)      387 2023-03-15 16:56:38.000000 not1mm-23.5.9.1/not1mm/data/check.png
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)    40156 2023-05-06 20:10:52.000000 not1mm-23.5.9.1/not1mm/data/configuration.ui
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)    89307 2023-03-07 17:30:38.000000 not1mm-23.5.9.1/not1mm/data/contests.sql
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)  4534539 2023-02-21 19:49:24.000000 not1mm-23.5.9.1/not1mm/data/cty.json
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)      451 2023-04-11 19:54:10.000000 not1mm-23.5.9.1/not1mm/data/cwmacros.txt
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)    19280 2023-03-20 20:22:09.000000 not1mm-23.5.9.1/not1mm/data/editcontact.ui
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)     2273 2023-02-21 14:39:24.000000 not1mm-23.5.9.1/not1mm/data/editmacro.ui
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)      474 2023-02-10 02:42:18.000000 not1mm-23.5.9.1/not1mm/data/greendot.png
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)      205 2023-02-09 20:47:40.000000 not1mm-23.5.9.1/not1mm/data/k6gte-not1mm.desktop
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)     4010 2023-02-09 20:45:38.000000 not1mm-23.5.9.1/not1mm/data/k6gte.not1mm-128.png
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)     1108 2023-02-09 20:45:03.000000 not1mm-23.5.9.1/not1mm/data/k6gte.not1mm-32.png
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)     2152 2023-02-09 20:45:22.000000 not1mm-23.5.9.1/not1mm/data/k6gte.not1mm-64.png
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)      970 2023-03-23 20:14:51.000000 not1mm-23.5.9.1/not1mm/data/logwindow.ui
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)    43909 2023-05-08 20:14:41.000000 not1mm-23.5.9.1/not1mm/data/main.ui
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)    17963 2023-05-05 12:59:56.000000 not1mm-23.5.9.1/not1mm/data/new_contest.ui
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)     2018 2023-02-12 17:56:36.000000 not1mm-23.5.9.1/not1mm/data/opon.ui
-drwxr-xr-x   0 mbridak   (1000) mbridak   (1000)        0 2023-05-09 20:15:55.963520 not1mm-23.5.9.1/not1mm/data/phonetics/
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)    42590 2023-04-21 20:24:24.000000 not1mm-23.5.9.1/not1mm/data/phonetics/0.wav
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)    30248 2023-04-21 20:25:33.000000 not1mm-23.5.9.1/not1mm/data/phonetics/1.wav
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)    29584 2023-04-21 20:27:16.000000 not1mm-23.5.9.1/not1mm/data/phonetics/2.wav
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)    32072 2023-04-21 20:29:07.000000 not1mm-23.5.9.1/not1mm/data/phonetics/3.wav
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)    43052 2023-04-21 20:29:49.000000 not1mm-23.5.9.1/not1mm/data/phonetics/4.wav
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)    51976 2023-04-21 21:46:26.000000 not1mm-23.5.9.1/not1mm/data/phonetics/5.wav
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)    58634 2023-04-21 21:08:45.000000 not1mm-23.5.9.1/not1mm/data/phonetics/6.wav
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)    49154 2023-04-21 21:10:50.000000 not1mm-23.5.9.1/not1mm/data/phonetics/7.wav
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)    32842 2023-04-21 21:13:51.000000 not1mm-23.5.9.1/not1mm/data/phonetics/73.wav
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)    35636 2023-04-21 21:11:40.000000 not1mm-23.5.9.1/not1mm/data/phonetics/8.wav
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)    39592 2023-04-21 21:12:32.000000 not1mm-23.5.9.1/not1mm/data/phonetics/9.wav
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)    46800 2023-04-21 21:14:36.000000 not1mm-23.5.9.1/not1mm/data/phonetics/a.wav
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)    44594 2023-04-21 21:15:20.000000 not1mm-23.5.9.1/not1mm/data/phonetics/again.wav
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)    40976 2023-04-21 21:16:10.000000 not1mm-23.5.9.1/not1mm/data/phonetics/b.wav
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)    46746 2023-04-21 21:17:07.000000 not1mm-23.5.9.1/not1mm/data/phonetics/c.wav
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)    62558 2023-04-21 13:38:05.000000 not1mm-23.5.9.1/not1mm/data/phonetics/contest.wav
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)    92498 2023-04-21 21:17:54.000000 not1mm-23.5.9.1/not1mm/data/phonetics/cq.wav
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)    52524 2023-04-21 21:18:24.000000 not1mm-23.5.9.1/not1mm/data/phonetics/d.wav
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)    45700 2023-04-21 21:19:02.000000 not1mm-23.5.9.1/not1mm/data/phonetics/e.wav
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)    53438 2023-04-21 21:19:38.000000 not1mm-23.5.9.1/not1mm/data/phonetics/f.wav
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)    42766 2023-04-21 21:20:18.000000 not1mm-23.5.9.1/not1mm/data/phonetics/g.wav
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)    50040 2023-04-21 21:21:03.000000 not1mm-23.5.9.1/not1mm/data/phonetics/h.wav
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)    46372 2023-04-21 21:23:33.000000 not1mm-23.5.9.1/not1mm/data/phonetics/i.wav
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)    43434 2023-04-21 21:24:12.000000 not1mm-23.5.9.1/not1mm/data/phonetics/j.wav
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)    49066 2023-04-21 21:24:57.000000 not1mm-23.5.9.1/not1mm/data/phonetics/k.wav
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)   185562 2023-04-21 21:25:43.000000 not1mm-23.5.9.1/not1mm/data/phonetics/k6gte.wav
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)    43154 2023-04-21 21:26:21.000000 not1mm-23.5.9.1/not1mm/data/phonetics/l.wav
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)    54352 2023-04-21 21:27:07.000000 not1mm-23.5.9.1/not1mm/data/phonetics/m.wav
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)    56798 2023-04-21 21:27:57.000000 not1mm-23.5.9.1/not1mm/data/phonetics/mynumber.wav
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)    52204 2023-04-21 21:28:42.000000 not1mm-23.5.9.1/not1mm/data/phonetics/n.wav
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)   154544 2023-04-21 21:29:54.000000 not1mm-23.5.9.1/not1mm/data/phonetics/nil.wav
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)    47440 2023-04-21 21:30:37.000000 not1mm-23.5.9.1/not1mm/data/phonetics/o.wav
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)    38300 2023-04-21 21:31:22.000000 not1mm-23.5.9.1/not1mm/data/phonetics/p.wav
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)    55288 2023-04-21 21:31:58.000000 not1mm-23.5.9.1/not1mm/data/phonetics/q.wav
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)    47432 2023-04-21 21:32:39.000000 not1mm-23.5.9.1/not1mm/data/phonetics/r.wav
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)    46122 2023-04-21 21:33:20.000000 not1mm-23.5.9.1/not1mm/data/phonetics/roger.wav
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)    60698 2023-04-21 21:33:59.000000 not1mm-23.5.9.1/not1mm/data/phonetics/s.wav
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)    70424 2023-04-17 20:43:04.000000 not1mm-23.5.9.1/not1mm/data/phonetics/space.wav
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)    58196 2023-04-21 21:35:28.000000 not1mm-23.5.9.1/not1mm/data/phonetics/t.wav
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)    56320 2023-04-21 21:36:54.000000 not1mm-23.5.9.1/not1mm/data/phonetics/thankyou.wav
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)    94980 2023-04-21 21:37:27.000000 not1mm-23.5.9.1/not1mm/data/phonetics/thankyouqrz.wav
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)    65922 2023-04-21 21:38:05.000000 not1mm-23.5.9.1/not1mm/data/phonetics/u.wav
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)    50142 2023-04-21 21:38:37.000000 not1mm-23.5.9.1/not1mm/data/phonetics/v.wav
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)    37638 2023-04-21 21:39:21.000000 not1mm-23.5.9.1/not1mm/data/phonetics/w.wav
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)    61870 2023-04-21 21:40:02.000000 not1mm-23.5.9.1/not1mm/data/phonetics/x.wav
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)    56524 2023-04-21 21:40:40.000000 not1mm-23.5.9.1/not1mm/data/phonetics/y.wav
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)    46510 2023-04-21 21:41:22.000000 not1mm-23.5.9.1/not1mm/data/phonetics/yourcall.wav
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)    51768 2023-04-21 21:41:59.000000 not1mm-23.5.9.1/not1mm/data/phonetics/z.wav
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)     1600 2023-04-03 14:20:44.000000 not1mm-23.5.9.1/not1mm/data/pickcontest.ui
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)      565 2023-02-10 02:42:40.000000 not1mm-23.5.9.1/not1mm/data/reddot.png
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)    35566 2023-04-15 16:43:11.000000 not1mm-23.5.9.1/not1mm/data/settings.ui
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)      470 2023-04-18 18:00:45.000000 not1mm-23.5.9.1/not1mm/data/ssbmacros.txt
-drwxr-xr-x   0 mbridak   (1000) mbridak   (1000)        0 2023-05-09 20:15:55.966519 not1mm-23.5.9.1/not1mm/lib/
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)        0 2022-11-03 15:04:39.000000 not1mm-23.5.9.1/not1mm/lib/__init__.py
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)      379 2023-04-10 20:24:21.000000 not1mm-23.5.9.1/not1mm/lib/about.py
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)    13705 2023-05-07 16:50:54.000000 not1mm-23.5.9.1/not1mm/lib/cat_interface.py
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)     1772 2023-03-17 21:26:43.000000 not1mm-23.5.9.1/not1mm/lib/cwinterface.py
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)    34193 2023-05-05 18:13:45.000000 not1mm-23.5.9.1/not1mm/lib/database.py
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)      357 2023-03-20 13:17:21.000000 not1mm-23.5.9.1/not1mm/lib/edit_contact.py
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)      559 2023-03-06 17:59:31.000000 not1mm-23.5.9.1/not1mm/lib/edit_macro.py
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)      363 2023-03-06 18:02:53.000000 not1mm-23.5.9.1/not1mm/lib/edit_opon.py
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)     1973 2023-04-11 17:58:02.000000 not1mm-23.5.9.1/not1mm/lib/edit_station.py
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)     8760 2023-04-05 20:29:02.000000 not1mm-23.5.9.1/not1mm/lib/ham_utility.py
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)    13916 2023-03-07 18:49:31.000000 not1mm-23.5.9.1/not1mm/lib/lookup.py
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)     1999 2023-04-12 19:58:03.000000 not1mm-23.5.9.1/not1mm/lib/multicast.py
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)     4434 2023-03-17 16:20:37.000000 not1mm-23.5.9.1/not1mm/lib/n1mm.py
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)      354 2023-03-28 20:21:24.000000 not1mm-23.5.9.1/not1mm/lib/new_contest.py
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)      363 2023-03-31 21:22:27.000000 not1mm-23.5.9.1/not1mm/lib/select_contest.py
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)     6188 2023-05-06 20:36:00.000000 not1mm-23.5.9.1/not1mm/lib/settings.py
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)       48 2023-05-09 20:07:08.000000 not1mm-23.5.9.1/not1mm/lib/version.py
--rwxr-xr-x   0 mbridak   (1000) mbridak   (1000)    30275 2023-05-09 15:02:00.000000 not1mm-23.5.9.1/not1mm/logwindow.py
-drwxr-xr-x   0 mbridak   (1000) mbridak   (1000)        0 2023-05-09 20:15:55.970519 not1mm-23.5.9.1/not1mm/plugins/
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)    13746 2023-05-05 16:08:13.000000 not1mm-23.5.9.1/not1mm/plugins/10_10_fall_cw.py
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)    13752 2023-05-05 16:08:31.000000 not1mm-23.5.9.1/not1mm/plugins/10_10_spring_cw.py
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)    13759 2023-05-05 16:08:41.000000 not1mm-23.5.9.1/not1mm/plugins/10_10_summer_phone.py
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)    13762 2023-05-05 16:08:51.000000 not1mm-23.5.9.1/not1mm/plugins/10_10_winter_phone.py
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)        0 2023-02-20 21:20:03.000000 not1mm-23.5.9.1/not1mm/plugins/__init__.py
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)    14549 2023-05-05 16:08:59.000000 not1mm-23.5.9.1/not1mm/plugins/arrl_dx_cw.py
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)    14552 2023-05-05 16:09:07.000000 not1mm-23.5.9.1/not1mm/plugins/arrl_dx_ssb.py
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)    12990 2023-05-05 16:10:17.000000 not1mm-23.5.9.1/not1mm/plugins/arrl_field_day.py
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)     2860 2023-05-05 16:10:11.000000 not1mm-23.5.9.1/not1mm/plugins/arrl_rtty_ru.py
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)    15941 2023-05-05 19:46:43.000000 not1mm-23.5.9.1/not1mm/plugins/arrl_ss_cw.py
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)    15946 2023-05-05 19:54:23.000000 not1mm-23.5.9.1/not1mm/plugins/arrl_ss_phone.py
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)    14939 2023-05-08 19:30:37.000000 not1mm-23.5.9.1/not1mm/plugins/cq_wpx_cw.py
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)    15026 2023-05-05 16:10:01.000000 not1mm-23.5.9.1/not1mm/plugins/cq_wpx_ssb.py
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)    13895 2023-05-05 16:09:55.000000 not1mm-23.5.9.1/not1mm/plugins/cq_ww_cw.py
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)    13899 2023-05-05 16:11:06.000000 not1mm-23.5.9.1/not1mm/plugins/cq_ww_ssb.py
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)    14753 2023-05-05 16:11:03.000000 not1mm-23.5.9.1/not1mm/plugins/cwt.py
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)     7453 2023-05-05 16:10:58.000000 not1mm-23.5.9.1/not1mm/plugins/general_logging.py
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)    13854 2023-05-05 16:10:55.000000 not1mm-23.5.9.1/not1mm/plugins/jidx_cw.py
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)    13855 2023-05-05 16:10:48.000000 not1mm-23.5.9.1/not1mm/plugins/jidx_ph.py
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)     3121 2023-05-05 16:11:15.000000 not1mm-23.5.9.1/not1mm/plugins/winter_field_day.py
-drwxr-xr-x   0 mbridak   (1000) mbridak   (1000)        0 2023-05-09 20:15:55.970519 not1mm-23.5.9.1/not1mm/testing/
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)      565 2023-05-05 15:04:14.000000 not1mm-23.5.9.1/not1mm/testing/test.py
-drwxr-xr-x   0 mbridak   (1000) mbridak   (1000)        0 2023-05-09 20:15:55.944520 not1mm-23.5.9.1/not1mm.egg-info/
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)    25054 2023-05-09 20:15:55.000000 not1mm-23.5.9.1/not1mm.egg-info/PKG-INFO
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)     3443 2023-05-09 20:15:55.000000 not1mm-23.5.9.1/not1mm.egg-info/SOURCES.txt
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)        1 2023-05-09 20:15:55.000000 not1mm-23.5.9.1/not1mm.egg-info/dependency_links.txt
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)       47 2023-05-09 20:15:55.000000 not1mm-23.5.9.1/not1mm.egg-info/entry_points.txt
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)       64 2023-05-09 20:15:55.000000 not1mm-23.5.9.1/not1mm.egg-info/requires.txt
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)       33 2023-05-09 20:15:55.000000 not1mm-23.5.9.1/not1mm.egg-info/top_level.txt
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)     1219 2023-05-09 20:07:09.000000 not1mm-23.5.9.1/pyproject.toml
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)       38 2023-05-09 20:15:55.971519 not1mm-23.5.9.1/setup.cfg
-drwxr-xr-x   0 mbridak   (1000) mbridak   (1000)        0 2023-05-09 20:15:55.970519 not1mm-23.5.9.1/testing/
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)     2248 2023-03-07 22:04:42.000000 not1mm-23.5.9.1/testing/test.py
+drwxr-xr-x   0 mbridak   (1000) mbridak   (1000)        0 2023-05-10 04:06:27.239200 not1mm-23.5.9.2/
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)    35149 2022-05-05 15:15:13.000000 not1mm-23.5.9.2/LICENSE
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)    25132 2023-05-10 04:06:27.238201 not1mm-23.5.9.2/PKG-INFO
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)    24385 2023-05-10 04:05:08.000000 not1mm-23.5.9.2/README.md
+drwxr-xr-x   0 mbridak   (1000) mbridak   (1000)        0 2023-05-10 04:06:26.977197 not1mm-23.5.9.2/not1mm/
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)        0 2022-11-03 15:04:39.000000 not1mm-23.5.9.2/not1mm/__init__.py
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)    80096 2023-05-10 03:49:09.000000 not1mm-23.5.9.2/not1mm/__main__.py
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)    23860 2023-05-09 20:08:28.000000 not1mm-23.5.9.2/not1mm/bandmap.py
+drwxr-xr-x   0 mbridak   (1000) mbridak   (1000)        0 2023-05-10 04:06:27.032198 not1mm-23.5.9.2/not1mm/data/
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)    16590 2023-02-15 20:52:35.000000 not1mm-23.5.9.2/not1mm/data/Combinear.qss
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)   203952 2023-01-27 16:44:51.000000 not1mm-23.5.9.2/not1mm/data/JetBrainsMono-Regular.ttf
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)   542666 2023-02-14 19:22:02.000000 not1mm-23.5.9.2/not1mm/data/MASTER.SCP
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)     2352 2023-04-10 21:02:17.000000 not1mm-23.5.9.2/not1mm/data/about.ui
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)      224 2023-04-18 03:49:58.000000 not1mm-23.5.9.2/not1mm/data/alpha bravo charlie delta.txt
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)     5246 2023-05-01 15:41:16.000000 not1mm-23.5.9.2/not1mm/data/bandmap.ui
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)      387 2023-03-15 16:56:38.000000 not1mm-23.5.9.2/not1mm/data/check.png
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)    40156 2023-05-06 20:10:52.000000 not1mm-23.5.9.2/not1mm/data/configuration.ui
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)    89307 2023-03-07 17:30:38.000000 not1mm-23.5.9.2/not1mm/data/contests.sql
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)  4534539 2023-02-21 19:49:24.000000 not1mm-23.5.9.2/not1mm/data/cty.json
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)      451 2023-04-11 19:54:10.000000 not1mm-23.5.9.2/not1mm/data/cwmacros.txt
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)    19280 2023-03-20 20:22:09.000000 not1mm-23.5.9.2/not1mm/data/editcontact.ui
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)     2273 2023-02-21 14:39:24.000000 not1mm-23.5.9.2/not1mm/data/editmacro.ui
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)      474 2023-02-10 02:42:18.000000 not1mm-23.5.9.2/not1mm/data/greendot.png
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)      205 2023-02-09 20:47:40.000000 not1mm-23.5.9.2/not1mm/data/k6gte-not1mm.desktop
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)     4010 2023-02-09 20:45:38.000000 not1mm-23.5.9.2/not1mm/data/k6gte.not1mm-128.png
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)     1108 2023-02-09 20:45:03.000000 not1mm-23.5.9.2/not1mm/data/k6gte.not1mm-32.png
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)     2152 2023-02-09 20:45:22.000000 not1mm-23.5.9.2/not1mm/data/k6gte.not1mm-64.png
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)      970 2023-03-23 20:14:51.000000 not1mm-23.5.9.2/not1mm/data/logwindow.ui
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)    43909 2023-05-08 20:14:41.000000 not1mm-23.5.9.2/not1mm/data/main.ui
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)    17963 2023-05-05 12:59:56.000000 not1mm-23.5.9.2/not1mm/data/new_contest.ui
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)     2018 2023-02-12 17:56:36.000000 not1mm-23.5.9.2/not1mm/data/opon.ui
+drwxr-xr-x   0 mbridak   (1000) mbridak   (1000)        0 2023-05-10 04:06:27.134199 not1mm-23.5.9.2/not1mm/data/phonetics/
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)    42590 2023-04-21 20:24:24.000000 not1mm-23.5.9.2/not1mm/data/phonetics/0.wav
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)    30248 2023-04-21 20:25:33.000000 not1mm-23.5.9.2/not1mm/data/phonetics/1.wav
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)    29584 2023-04-21 20:27:16.000000 not1mm-23.5.9.2/not1mm/data/phonetics/2.wav
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)    32072 2023-04-21 20:29:07.000000 not1mm-23.5.9.2/not1mm/data/phonetics/3.wav
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)    43052 2023-04-21 20:29:49.000000 not1mm-23.5.9.2/not1mm/data/phonetics/4.wav
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)    51976 2023-04-21 21:46:26.000000 not1mm-23.5.9.2/not1mm/data/phonetics/5.wav
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)    58634 2023-04-21 21:08:45.000000 not1mm-23.5.9.2/not1mm/data/phonetics/6.wav
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)    49154 2023-04-21 21:10:50.000000 not1mm-23.5.9.2/not1mm/data/phonetics/7.wav
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)    32842 2023-04-21 21:13:51.000000 not1mm-23.5.9.2/not1mm/data/phonetics/73.wav
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)    35636 2023-04-21 21:11:40.000000 not1mm-23.5.9.2/not1mm/data/phonetics/8.wav
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)    39592 2023-04-21 21:12:32.000000 not1mm-23.5.9.2/not1mm/data/phonetics/9.wav
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)    46800 2023-04-21 21:14:36.000000 not1mm-23.5.9.2/not1mm/data/phonetics/a.wav
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)    44594 2023-04-21 21:15:20.000000 not1mm-23.5.9.2/not1mm/data/phonetics/again.wav
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)    40976 2023-04-21 21:16:10.000000 not1mm-23.5.9.2/not1mm/data/phonetics/b.wav
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)    46746 2023-04-21 21:17:07.000000 not1mm-23.5.9.2/not1mm/data/phonetics/c.wav
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)    62558 2023-04-21 13:38:05.000000 not1mm-23.5.9.2/not1mm/data/phonetics/contest.wav
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)    92498 2023-04-21 21:17:54.000000 not1mm-23.5.9.2/not1mm/data/phonetics/cq.wav
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)    52524 2023-04-21 21:18:24.000000 not1mm-23.5.9.2/not1mm/data/phonetics/d.wav
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)    45700 2023-04-21 21:19:02.000000 not1mm-23.5.9.2/not1mm/data/phonetics/e.wav
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)    53438 2023-04-21 21:19:38.000000 not1mm-23.5.9.2/not1mm/data/phonetics/f.wav
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)    42766 2023-04-21 21:20:18.000000 not1mm-23.5.9.2/not1mm/data/phonetics/g.wav
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)    50040 2023-04-21 21:21:03.000000 not1mm-23.5.9.2/not1mm/data/phonetics/h.wav
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)    46372 2023-04-21 21:23:33.000000 not1mm-23.5.9.2/not1mm/data/phonetics/i.wav
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)    43434 2023-04-21 21:24:12.000000 not1mm-23.5.9.2/not1mm/data/phonetics/j.wav
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)    49066 2023-04-21 21:24:57.000000 not1mm-23.5.9.2/not1mm/data/phonetics/k.wav
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)   185562 2023-04-21 21:25:43.000000 not1mm-23.5.9.2/not1mm/data/phonetics/k6gte.wav
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)    43154 2023-04-21 21:26:21.000000 not1mm-23.5.9.2/not1mm/data/phonetics/l.wav
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)    54352 2023-04-21 21:27:07.000000 not1mm-23.5.9.2/not1mm/data/phonetics/m.wav
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)    56798 2023-04-21 21:27:57.000000 not1mm-23.5.9.2/not1mm/data/phonetics/mynumber.wav
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)    52204 2023-04-21 21:28:42.000000 not1mm-23.5.9.2/not1mm/data/phonetics/n.wav
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)   154544 2023-04-21 21:29:54.000000 not1mm-23.5.9.2/not1mm/data/phonetics/nil.wav
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)    47440 2023-04-21 21:30:37.000000 not1mm-23.5.9.2/not1mm/data/phonetics/o.wav
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)    38300 2023-04-21 21:31:22.000000 not1mm-23.5.9.2/not1mm/data/phonetics/p.wav
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)    55288 2023-04-21 21:31:58.000000 not1mm-23.5.9.2/not1mm/data/phonetics/q.wav
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)    47432 2023-04-21 21:32:39.000000 not1mm-23.5.9.2/not1mm/data/phonetics/r.wav
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)    46122 2023-04-21 21:33:20.000000 not1mm-23.5.9.2/not1mm/data/phonetics/roger.wav
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)    60698 2023-04-21 21:33:59.000000 not1mm-23.5.9.2/not1mm/data/phonetics/s.wav
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)    70424 2023-04-17 20:43:04.000000 not1mm-23.5.9.2/not1mm/data/phonetics/space.wav
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)    58196 2023-04-21 21:35:28.000000 not1mm-23.5.9.2/not1mm/data/phonetics/t.wav
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)    56320 2023-04-21 21:36:54.000000 not1mm-23.5.9.2/not1mm/data/phonetics/thankyou.wav
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)    94980 2023-04-21 21:37:27.000000 not1mm-23.5.9.2/not1mm/data/phonetics/thankyouqrz.wav
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)    65922 2023-04-21 21:38:05.000000 not1mm-23.5.9.2/not1mm/data/phonetics/u.wav
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)    50142 2023-04-21 21:38:37.000000 not1mm-23.5.9.2/not1mm/data/phonetics/v.wav
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)    37638 2023-04-21 21:39:21.000000 not1mm-23.5.9.2/not1mm/data/phonetics/w.wav
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)    61870 2023-04-21 21:40:02.000000 not1mm-23.5.9.2/not1mm/data/phonetics/x.wav
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)    56524 2023-04-21 21:40:40.000000 not1mm-23.5.9.2/not1mm/data/phonetics/y.wav
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)    46510 2023-04-21 21:41:22.000000 not1mm-23.5.9.2/not1mm/data/phonetics/yourcall.wav
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)    51768 2023-04-21 21:41:59.000000 not1mm-23.5.9.2/not1mm/data/phonetics/z.wav
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)     1600 2023-04-03 14:20:44.000000 not1mm-23.5.9.2/not1mm/data/pickcontest.ui
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)      565 2023-02-10 02:42:40.000000 not1mm-23.5.9.2/not1mm/data/reddot.png
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)    35566 2023-04-15 16:43:11.000000 not1mm-23.5.9.2/not1mm/data/settings.ui
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)      470 2023-04-18 18:00:45.000000 not1mm-23.5.9.2/not1mm/data/ssbmacros.txt
+drwxr-xr-x   0 mbridak   (1000) mbridak   (1000)        0 2023-05-10 04:06:27.178200 not1mm-23.5.9.2/not1mm/lib/
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)        0 2022-11-03 15:04:39.000000 not1mm-23.5.9.2/not1mm/lib/__init__.py
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)      379 2023-04-10 20:24:21.000000 not1mm-23.5.9.2/not1mm/lib/about.py
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)    13705 2023-05-07 16:50:54.000000 not1mm-23.5.9.2/not1mm/lib/cat_interface.py
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)     1772 2023-03-17 21:26:43.000000 not1mm-23.5.9.2/not1mm/lib/cwinterface.py
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)    34193 2023-05-05 18:13:45.000000 not1mm-23.5.9.2/not1mm/lib/database.py
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)      357 2023-03-20 13:17:21.000000 not1mm-23.5.9.2/not1mm/lib/edit_contact.py
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)      559 2023-03-06 17:59:31.000000 not1mm-23.5.9.2/not1mm/lib/edit_macro.py
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)      363 2023-03-06 18:02:53.000000 not1mm-23.5.9.2/not1mm/lib/edit_opon.py
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)     1973 2023-04-11 17:58:02.000000 not1mm-23.5.9.2/not1mm/lib/edit_station.py
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)     8760 2023-04-05 20:29:02.000000 not1mm-23.5.9.2/not1mm/lib/ham_utility.py
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)    13916 2023-03-07 18:49:31.000000 not1mm-23.5.9.2/not1mm/lib/lookup.py
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)     1999 2023-04-12 19:58:03.000000 not1mm-23.5.9.2/not1mm/lib/multicast.py
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)     4434 2023-03-17 16:20:37.000000 not1mm-23.5.9.2/not1mm/lib/n1mm.py
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)      354 2023-03-28 20:21:24.000000 not1mm-23.5.9.2/not1mm/lib/new_contest.py
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)      363 2023-03-31 21:22:27.000000 not1mm-23.5.9.2/not1mm/lib/select_contest.py
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)     6188 2023-05-06 20:36:00.000000 not1mm-23.5.9.2/not1mm/lib/settings.py
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)       48 2023-05-10 04:00:32.000000 not1mm-23.5.9.2/not1mm/lib/version.py
+-rwxr-xr-x   0 mbridak   (1000) mbridak   (1000)    30275 2023-05-09 15:02:00.000000 not1mm-23.5.9.2/not1mm/logwindow.py
+drwxr-xr-x   0 mbridak   (1000) mbridak   (1000)        0 2023-05-10 04:06:27.230200 not1mm-23.5.9.2/not1mm/plugins/
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)    13746 2023-05-05 16:08:13.000000 not1mm-23.5.9.2/not1mm/plugins/10_10_fall_cw.py
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)    13752 2023-05-05 16:08:31.000000 not1mm-23.5.9.2/not1mm/plugins/10_10_spring_cw.py
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)    13759 2023-05-05 16:08:41.000000 not1mm-23.5.9.2/not1mm/plugins/10_10_summer_phone.py
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)    13762 2023-05-05 16:08:51.000000 not1mm-23.5.9.2/not1mm/plugins/10_10_winter_phone.py
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)        0 2023-02-20 21:20:03.000000 not1mm-23.5.9.2/not1mm/plugins/__init__.py
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)    14549 2023-05-05 16:08:59.000000 not1mm-23.5.9.2/not1mm/plugins/arrl_dx_cw.py
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)    14552 2023-05-05 16:09:07.000000 not1mm-23.5.9.2/not1mm/plugins/arrl_dx_ssb.py
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)    12990 2023-05-05 16:10:17.000000 not1mm-23.5.9.2/not1mm/plugins/arrl_field_day.py
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)     2860 2023-05-05 16:10:11.000000 not1mm-23.5.9.2/not1mm/plugins/arrl_rtty_ru.py
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)    15941 2023-05-05 19:46:43.000000 not1mm-23.5.9.2/not1mm/plugins/arrl_ss_cw.py
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)    15946 2023-05-05 19:54:23.000000 not1mm-23.5.9.2/not1mm/plugins/arrl_ss_phone.py
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)    14939 2023-05-08 19:30:37.000000 not1mm-23.5.9.2/not1mm/plugins/cq_wpx_cw.py
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)    15026 2023-05-05 16:10:01.000000 not1mm-23.5.9.2/not1mm/plugins/cq_wpx_ssb.py
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)    13895 2023-05-05 16:09:55.000000 not1mm-23.5.9.2/not1mm/plugins/cq_ww_cw.py
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)    13899 2023-05-05 16:11:06.000000 not1mm-23.5.9.2/not1mm/plugins/cq_ww_ssb.py
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)    14753 2023-05-05 16:11:03.000000 not1mm-23.5.9.2/not1mm/plugins/cwt.py
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)     7453 2023-05-05 16:10:58.000000 not1mm-23.5.9.2/not1mm/plugins/general_logging.py
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)    13854 2023-05-05 16:10:55.000000 not1mm-23.5.9.2/not1mm/plugins/jidx_cw.py
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)    13855 2023-05-05 16:10:48.000000 not1mm-23.5.9.2/not1mm/plugins/jidx_ph.py
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)     3121 2023-05-05 16:11:15.000000 not1mm-23.5.9.2/not1mm/plugins/winter_field_day.py
+drwxr-xr-x   0 mbridak   (1000) mbridak   (1000)        0 2023-05-10 04:06:27.232200 not1mm-23.5.9.2/not1mm/testing/
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)      565 2023-05-05 15:04:14.000000 not1mm-23.5.9.2/not1mm/testing/test.py
+drwxr-xr-x   0 mbridak   (1000) mbridak   (1000)        0 2023-05-10 04:06:26.980197 not1mm-23.5.9.2/not1mm.egg-info/
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)    25132 2023-05-10 04:06:26.000000 not1mm-23.5.9.2/not1mm.egg-info/PKG-INFO
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)     3443 2023-05-10 04:06:26.000000 not1mm-23.5.9.2/not1mm.egg-info/SOURCES.txt
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)        1 2023-05-10 04:06:26.000000 not1mm-23.5.9.2/not1mm.egg-info/dependency_links.txt
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)       47 2023-05-10 04:06:26.000000 not1mm-23.5.9.2/not1mm.egg-info/entry_points.txt
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)       64 2023-05-10 04:06:26.000000 not1mm-23.5.9.2/not1mm.egg-info/requires.txt
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)       33 2023-05-10 04:06:26.000000 not1mm-23.5.9.2/not1mm.egg-info/top_level.txt
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)     1219 2023-05-10 04:01:51.000000 not1mm-23.5.9.2/pyproject.toml
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)       38 2023-05-10 04:06:27.241201 not1mm-23.5.9.2/setup.cfg
+drwxr-xr-x   0 mbridak   (1000) mbridak   (1000)        0 2023-05-10 04:06:27.234200 not1mm-23.5.9.2/testing/
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)     2248 2023-03-07 22:04:42.000000 not1mm-23.5.9.2/testing/test.py
```

### Comparing `not1mm-23.5.9.1/LICENSE` & `not1mm-23.5.9.2/LICENSE`

 * *Files identical despite different names*

### Comparing `not1mm-23.5.9.1/PKG-INFO` & `not1mm-23.5.9.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: not1mm
-Version: 23.5.9.1
+Version: 23.5.9.2
 Summary: NOT1MM Logger
 Author-email: Michael Bridak <michael.bridak@gmail.com>
 Project-URL: Homepage, https://github.com/mbridak/not1mm
 Project-URL: Bug Tracker, https://github.com/mbridak/not1mm/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: Development Status :: 4 - Beta
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
@@ -63,16 +63,16 @@
     - [Macro use with voice](#macro-use-with-voice)
   - [cty.dat and QRZ lookups for distance and bearing](#ctydat-and-qrz-lookups-for-distance-and-bearing)
   - [Other uses for the call field](#other-uses-for-the-call-field)
   - [Windows](#windows)
     - [The Main Window](#the-main-window)
       - [Keyboard commands](#keyboard-commands)
     - [Log Display](#log-display)
+      - [Editing a contact](#editing-a-contact)
     - [Bandmap](#bandmap)
-  - [Editing a contact](#editing-a-contact)
   - [Recalulate Mults](#recalulate-mults)
   - [Cabrillo](#cabrillo)
   - [ADIF](#adif)
   - [Dupe checking](#dupe-checking)
   - [Contest specific notes](#contest-specific-notes)
     - [ARRL Sweekstakes](#arrl-sweekstakes)
       - [The exchange parser](#the-exchange-parser)
@@ -114,15 +114,15 @@
 - CQ World Wide SSB
 - CWOps CWT
 - Japan International DX CW
 - Japan International DX SSB
 
 ## Changes of note
 
-- [23-5-9] Removed 1 second timers in the bandmap and log window, made them UDP readyRead(). Much smoother. Add CTRL-PgUp and CTRL-PgDown keys to jump to the next/prev spots in the bandmap. Fix: Voice not keying on LSB.
+- [23-5-9] Removed 1 second timers in the bandmap and log window, made them UDP readyRead(). Much smoother. Add CTRL-PgUp and CTRL-PgDown keys to jump to the next/prev spots in the bandmap. Fix: Voice not keying on LSB. Fix: calling pttoff when no CAT interface. Fix: Voice not keying on LSB
 - [23-5-8] Bandmap zoom in/out now centers scale to RX Freq.
 - [23-5-7] Added bandwidth marker to the bandmap.
 - [23-5-6] Added AR Cluster filter options for the bandmap. Added a station ID to the multicast packets. This will prevent erratic bevahiour if 2 stations are on the same network.
 - [23-5-5] Re-wrote most of the log window code. Added ARRL Sweepstakes.
 - [23-5-4] Fixed 'Operators' line in WPX cabrillo file. Fix window title not updating if no CAT control.
 - [23-5-3] Added '#' macro.
 - [23-5-1] Added 10 10 CW and Phone contests. Added a `Cluster` TAB for the AR Cluster server/port in the configuration settings.
@@ -412,36 +412,36 @@
 
 The Log display gets updated automatically when a contact is entered. The top half is a list of all contacts.
 
 ![Log Display Window](https://github.com/mbridak/not1mm/raw/master/pic/logdisplay.png)
 
 The bottom half of the log displays contacts sorted by what's currently in the call entry field. The columns displayed in the log window are dependant on what contests is currently active.
 
-### Bandmap
-
-`Window`>`Bandmap`
-
-Put your callsign in the top and press the connect button.
-
-The bandmap window is, as with everything, a work in progress. The bandmap now follows the VFO. VFO indicator now displays as small triangle in the frequency tickmarks. A small blue rectangle shows the receivers bandwidth. Clicked on spots now tune the radio and set the callsign field.
-
-![Bandmap Window](https://github.com/mbridak/not1mm/raw/master/pic/bandmap.png)
-
-## Editing a contact
+#### Editing a contact
 
 ![Editing a cell](https://github.com/mbridak/not1mm/raw/master/pic/edit_cell.png)
 
 You can double click a cell in the log window and edit its contents.
 
 You can also Right-Click on a cell to bring up the edit dialog.
 
 ![right click edit dialog](https://github.com/mbridak/not1mm/raw/master/pic/edit_dialog.png)
 
 You can not directly edit the multiplier status of a contact. Instead see the next section on recalculating mults. If you change the callsign make sure the `WPX` field is still valid.
 
+### Bandmap
+
+`Window`>`Bandmap`
+
+Put your callsign in the top and press the connect button.
+
+The bandmap window is, as with everything, a work in progress. The bandmap now follows the VFO. VFO indicator now displays as small triangle in the frequency tickmarks. A small blue rectangle shows the receivers bandwidth. Clicked on spots now tune the radio and set the callsign field.
+
+![Bandmap Window](https://github.com/mbridak/not1mm/raw/master/pic/bandmap.png)
+
 ## Recalulate Mults
 
 After editing a contact and before generating a Cabrillo file. There is a Misc menu option that will recalculate the multipliers incase an edit had caused a change.
 
 ## Cabrillo
 
 Click on `File` > `Generate Cabrillo`
```

### Comparing `not1mm-23.5.9.1/README.md` & `not1mm-23.5.9.2/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -44,16 +44,16 @@
     - [Macro use with voice](#macro-use-with-voice)
   - [cty.dat and QRZ lookups for distance and bearing](#ctydat-and-qrz-lookups-for-distance-and-bearing)
   - [Other uses for the call field](#other-uses-for-the-call-field)
   - [Windows](#windows)
     - [The Main Window](#the-main-window)
       - [Keyboard commands](#keyboard-commands)
     - [Log Display](#log-display)
+      - [Editing a contact](#editing-a-contact)
     - [Bandmap](#bandmap)
-  - [Editing a contact](#editing-a-contact)
   - [Recalulate Mults](#recalulate-mults)
   - [Cabrillo](#cabrillo)
   - [ADIF](#adif)
   - [Dupe checking](#dupe-checking)
   - [Contest specific notes](#contest-specific-notes)
     - [ARRL Sweekstakes](#arrl-sweekstakes)
       - [The exchange parser](#the-exchange-parser)
@@ -95,15 +95,15 @@
 - CQ World Wide SSB
 - CWOps CWT
 - Japan International DX CW
 - Japan International DX SSB
 
 ## Changes of note
 
-- [23-5-9] Removed 1 second timers in the bandmap and log window, made them UDP readyRead(). Much smoother. Add CTRL-PgUp and CTRL-PgDown keys to jump to the next/prev spots in the bandmap. Fix: Voice not keying on LSB.
+- [23-5-9] Removed 1 second timers in the bandmap and log window, made them UDP readyRead(). Much smoother. Add CTRL-PgUp and CTRL-PgDown keys to jump to the next/prev spots in the bandmap. Fix: Voice not keying on LSB. Fix: calling pttoff when no CAT interface. Fix: Voice not keying on LSB
 - [23-5-8] Bandmap zoom in/out now centers scale to RX Freq.
 - [23-5-7] Added bandwidth marker to the bandmap.
 - [23-5-6] Added AR Cluster filter options for the bandmap. Added a station ID to the multicast packets. This will prevent erratic bevahiour if 2 stations are on the same network.
 - [23-5-5] Re-wrote most of the log window code. Added ARRL Sweepstakes.
 - [23-5-4] Fixed 'Operators' line in WPX cabrillo file. Fix window title not updating if no CAT control.
 - [23-5-3] Added '#' macro.
 - [23-5-1] Added 10 10 CW and Phone contests. Added a `Cluster` TAB for the AR Cluster server/port in the configuration settings.
@@ -393,36 +393,36 @@
 
 The Log display gets updated automatically when a contact is entered. The top half is a list of all contacts.
 
 ![Log Display Window](https://github.com/mbridak/not1mm/raw/master/pic/logdisplay.png)
 
 The bottom half of the log displays contacts sorted by what's currently in the call entry field. The columns displayed in the log window are dependant on what contests is currently active.
 
-### Bandmap
-
-`Window`>`Bandmap`
-
-Put your callsign in the top and press the connect button.
-
-The bandmap window is, as with everything, a work in progress. The bandmap now follows the VFO. VFO indicator now displays as small triangle in the frequency tickmarks. A small blue rectangle shows the receivers bandwidth. Clicked on spots now tune the radio and set the callsign field.
-
-![Bandmap Window](https://github.com/mbridak/not1mm/raw/master/pic/bandmap.png)
-
-## Editing a contact
+#### Editing a contact
 
 ![Editing a cell](https://github.com/mbridak/not1mm/raw/master/pic/edit_cell.png)
 
 You can double click a cell in the log window and edit its contents.
 
 You can also Right-Click on a cell to bring up the edit dialog.
 
 ![right click edit dialog](https://github.com/mbridak/not1mm/raw/master/pic/edit_dialog.png)
 
 You can not directly edit the multiplier status of a contact. Instead see the next section on recalculating mults. If you change the callsign make sure the `WPX` field is still valid.
 
+### Bandmap
+
+`Window`>`Bandmap`
+
+Put your callsign in the top and press the connect button.
+
+The bandmap window is, as with everything, a work in progress. The bandmap now follows the VFO. VFO indicator now displays as small triangle in the frequency tickmarks. A small blue rectangle shows the receivers bandwidth. Clicked on spots now tune the radio and set the callsign field.
+
+![Bandmap Window](https://github.com/mbridak/not1mm/raw/master/pic/bandmap.png)
+
 ## Recalulate Mults
 
 After editing a contact and before generating a Cabrillo file. There is a Misc menu option that will recalculate the multipliers incase an edit had caused a change.
 
 ## Cabrillo
 
 Click on `File` > `Generate Cabrillo`
```

### Comparing `not1mm-23.5.9.1/not1mm/__main__.py` & `not1mm-23.5.9.2/not1mm/__main__.py`

 * *Files 0% similar despite different names*

```diff
@@ -272,4733 +272,4735 @@
 000010f0: 636c 6f75 646c 6f67 223a 2046 616c 7365  cloudlog": False
 00001100: 2c0a 2020 2020 2020 2020 2263 6c6f 7564  ,.        "cloud
 00001110: 6c6f 6761 7069 223a 2022 222c 0a20 2020  logapi": "",.   
 00001120: 2020 2020 2022 636c 6f75 646c 6f67 7572       "cloudlogur
 00001130: 6c22 3a20 2222 2c0a 2020 2020 2020 2020  l": "",.        
 00001140: 2243 4154 5f69 7022 3a20 2231 3237 2e30  "CAT_ip": "127.0
 00001150: 2e30 2e31 222c 0a20 2020 2020 2020 2022  .0.1",.        "
-00001160: 7573 6572 6967 6374 6c64 223a 2054 7275  userigctld": Tru
-00001170: 652c 0a20 2020 2020 2020 2022 7573 6566  e,.        "usef
-00001180: 6c72 6967 223a 2046 616c 7365 2c0a 2020  lrig": False,.  
-00001190: 2020 2020 2020 2263 7769 7022 3a20 2231        "cwip": "1
-000011a0: 3237 2e30 2e30 2e31 222c 0a20 2020 2020  27.0.0.1",.     
-000011b0: 2020 2022 6377 706f 7274 223a 2036 3738     "cwport": 678
-000011c0: 392c 0a20 2020 2020 2020 2022 6377 7479  9,.        "cwty
-000011d0: 7065 223a 2031 2c0a 2020 2020 2020 2020  pe": 1,.        
-000011e0: 2275 7365 7365 7276 6572 223a 2046 616c  "useserver": Fal
-000011f0: 7365 2c0a 2020 2020 2020 2020 2243 4154  se,.        "CAT
-00001200: 5f70 6f72 7422 3a20 3435 3332 2c0a 2020  _port": 4532,.  
-00001210: 2020 2020 2020 2263 6c75 7374 6572 5f73        "cluster_s
-00001220: 6572 7665 7222 3a20 2264 7863 2e6e 6337  erver": "dxc.nc7
-00001230: 6a2e 636f 6d22 2c0a 2020 2020 2020 2020  j.com",.        
-00001240: 2263 6c75 7374 6572 5f70 6f72 7422 3a20  "cluster_port": 
-00001250: 3733 3733 2c0a 2020 2020 2020 2020 2263  7373,.        "c
-00001260: 6c75 7374 6572 5f66 696c 7465 7222 3a20  luster_filter": 
-00001270: 2253 6574 2044 5820 4669 6c74 6572 2053  "Set DX Filter S
-00001280: 706f 7474 6572 436f 6e74 3d4e 4122 2c0a  potterCont=NA",.
-00001290: 2020 2020 2020 2020 2263 6c75 7374 6572          "cluster
-000012a0: 5f6d 6f64 6522 3a20 224f 5045 4e22 2c0a  _mode": "OPEN",.
-000012b0: 2020 2020 7d0a 2020 2020 6170 7073 7461      }.    appsta
-000012c0: 7274 6564 203d 2046 616c 7365 0a20 2020  rted = False.   
-000012d0: 2063 6f6e 7461 6374 203d 207b 7d0a 2020   contact = {}.  
-000012e0: 2020 636f 6e74 6573 7420 3d20 4e6f 6e65    contest = None
-000012f0: 0a20 2020 2063 6f6e 7465 7374 5f73 6574  .    contest_set
-00001300: 7469 6e67 7320 3d20 7b7d 0a20 2020 2070  tings = {}.    p
-00001310: 7265 6620 3d20 4e6f 6e65 0a20 2020 2073  ref = None.    s
-00001320: 7461 7469 6f6e 203d 207b 7d0a 2020 2020  tation = {}.    
-00001330: 6375 7272 656e 745f 6f70 203d 2022 220a  current_op = "".
-00001340: 2020 2020 6375 7272 656e 745f 6d6f 6465      current_mode
-00001350: 203d 2022 220a 2020 2020 6375 7272 656e   = "".    curren
-00001360: 745f 6261 6e64 203d 2022 220a 2020 2020  t_band = "".    
-00001370: 6377 203d 204e 6f6e 650a 2020 2020 6c6f  cw = None.    lo
-00001380: 6f6b 5f75 7020 3d20 4e6f 6e65 0a20 2020  ok_up = None.   
-00001390: 2072 756e 5f73 7461 7465 203d 2046 616c   run_state = Fal
-000013a0: 7365 0a20 2020 2066 6b65 7973 203d 207b  se.    fkeys = {
-000013b0: 7d0a 2020 2020 6162 6f75 745f 6469 616c  }.    about_dial
-000013c0: 6f67 203d 204e 6f6e 650a 2020 2020 7172  og = None.    qr
-000013d0: 7a5f 6469 616c 6f67 203d 204e 6f6e 650a  z_dialog = None.
-000013e0: 2020 2020 7365 7474 696e 6773 5f64 6961      settings_dia
-000013f0: 6c6f 6720 3d20 4e6f 6e65 0a20 2020 2065  log = None.    e
-00001400: 6469 745f 6d61 6372 6f5f 6469 616c 6f67  dit_macro_dialog
-00001410: 203d 204e 6f6e 650a 2020 2020 636f 6e74   = None.    cont
-00001420: 6573 745f 6469 616c 6f67 203d 204e 6f6e  est_dialog = Non
-00001430: 650a 2020 2020 636f 6e66 6967 7572 6174  e.    configurat
-00001440: 696f 6e5f 6469 616c 6f67 203d 204e 6f6e  ion_dialog = Non
-00001450: 650a 2020 2020 6f70 6f6e 5f64 6961 6c6f  e.    opon_dialo
-00001460: 6720 3d20 4e6f 6e65 0a20 2020 2064 626e  g = None.    dbn
-00001470: 616d 6520 3d20 4441 5441 5f50 4154 4820  ame = DATA_PATH 
-00001480: 2b20 222f 6861 6d2e 6462 220a 2020 2020  + "/ham.db".    
-00001490: 7261 6469 6f5f 7374 6174 6520 3d20 7b7d  radio_state = {}
-000014a0: 0a20 2020 2072 6967 5f63 6f6e 7472 6f6c  .    rig_control
-000014b0: 203d 204e 6f6e 650a 2020 2020 7365 7276   = None.    serv
-000014c0: 6572 5f75 6470 203d 204e 6f6e 650a 2020  er_udp = None.  
-000014d0: 2020 6d75 6c74 6963 6173 745f 6772 6f75    multicast_grou
-000014e0: 7020 3d20 4e6f 6e65 0a20 2020 206d 756c  p = None.    mul
-000014f0: 7469 6361 7374 5f70 6f72 7420 3d20 4e6f  ticast_port = No
-00001500: 6e65 0a20 2020 2069 6e74 6572 6661 6365  ne.    interface
-00001510: 5f69 7020 3d20 4e6f 6e65 0a20 2020 2072  _ip = None.    r
-00001520: 6967 5f63 6f6e 7472 6f6c 203d 204e 6f6e  ig_control = Non
-00001530: 650a 0a20 2020 2064 6566 205f 5f69 6e69  e..    def __ini
-00001540: 745f 5f28 7365 6c66 2c20 2a61 7267 732c  t__(self, *args,
-00001550: 202a 2a6b 7761 7267 7329 3a0a 2020 2020   **kwargs):.    
-00001560: 2020 2020 7375 7065 7228 292e 5f5f 696e      super().__in
-00001570: 6974 5f5f 282a 6172 6773 2c20 2a2a 6b77  it__(*args, **kw
-00001580: 6172 6773 290a 2020 2020 2020 2020 6c6f  args).        lo
-00001590: 6767 6572 2e69 6e66 6f28 224d 6169 6e57  gger.info("MainW
-000015a0: 696e 646f 773a 205f 5f69 6e69 745f 5f22  indow: __init__"
-000015b0: 290a 2020 2020 2020 2020 7365 6c66 2e5f  ).        self._
-000015c0: 7564 7077 6174 6368 203d 204e 6f6e 650a  udpwatch = None.
-000015d0: 2020 2020 2020 2020 7365 6c66 2e75 6470          self.udp
-000015e0: 5f66 6966 6f20 3d20 7175 6575 652e 5175  _fifo = queue.Qu
-000015f0: 6575 6528 290a 2020 2020 2020 2020 6461  eue().        da
-00001600: 7461 5f70 6174 6820 3d20 574f 524b 494e  ta_path = WORKIN
-00001610: 475f 5041 5448 202b 2022 2f64 6174 612f  G_PATH + "/data/
-00001620: 6d61 696e 2e75 6922 0a20 2020 2020 2020  main.ui".       
-00001630: 2075 6963 2e6c 6f61 6455 6928 6461 7461   uic.loadUi(data
-00001640: 5f70 6174 682c 2073 656c 6629 0a20 2020  _path, self).   
-00001650: 2020 2020 2073 656c 662e 6c65 6674 646f       self.leftdo
-00001660: 742e 6869 6465 2829 0a20 2020 2020 2020  t.hide().       
-00001670: 2073 656c 662e 7269 6768 7464 6f74 2e68   self.rightdot.h
-00001680: 6964 6528 290a 2020 2020 2020 2020 7365  ide().        se
-00001690: 6c66 2e6e 316d 6d20 3d20 4e31 4d4d 2829  lf.n1mm = N1MM()
-000016a0: 0a20 2020 2020 2020 2073 656c 662e 6e65  .        self.ne
-000016b0: 7874 5f66 6965 6c64 203d 2073 656c 662e  xt_field = self.
-000016c0: 6f74 6865 725f 320a 2020 2020 2020 2020  other_2.        
-000016d0: 7365 6c66 2e64 7570 655f 696e 6469 6361  self.dupe_indica
-000016e0: 746f 722e 6869 6465 2829 0a20 2020 2020  tor.hide().     
-000016f0: 2020 2073 656c 662e 6377 5f73 7065 6564     self.cw_speed
-00001700: 2e76 616c 7565 4368 616e 6765 642e 636f  .valueChanged.co
-00001710: 6e6e 6563 7428 7365 6c66 2e63 7773 7065  nnect(self.cwspe
-00001720: 6564 5f73 7069 6e62 6f78 5f63 6861 6e67  ed_spinbox_chang
-00001730: 6564 290a 0a20 2020 2020 2020 2073 656c  ed)..        sel
-00001740: 662e 6163 7469 6f6e 4357 5f4d 6163 726f  f.actionCW_Macro
-00001750: 732e 7472 6967 6765 7265 642e 636f 6e6e  s.triggered.conn
-00001760: 6563 7428 7365 6c66 2e63 775f 6d61 6372  ect(self.cw_macr
-00001770: 6f73 5f73 7461 7465 5f63 6861 6e67 6564  os_state_changed
-00001780: 290a 2020 2020 2020 2020 7365 6c66 2e61  ).        self.a
-00001790: 6374 696f 6e43 6f6d 6d61 6e64 5f42 7574  ctionCommand_But
-000017a0: 746f 6e73 2e74 7269 6767 6572 6564 2e63  tons.triggered.c
-000017b0: 6f6e 6e65 6374 2873 656c 662e 636f 6d6d  onnect(self.comm
-000017c0: 616e 645f 6275 7474 6f6e 735f 7374 6174  and_buttons_stat
-000017d0: 655f 6368 616e 6765 290a 2020 2020 2020  e_change).      
-000017e0: 2020 7365 6c66 2e61 6374 696f 6e44 6172    self.actionDar
-000017f0: 6b5f 4d6f 6465 2e74 7269 6767 6572 6564  k_Mode.triggered
-00001800: 2e63 6f6e 6e65 6374 2873 656c 662e 6461  .connect(self.da
-00001810: 726b 5f6d 6f64 655f 7374 6174 655f 6368  rk_mode_state_ch
-00001820: 616e 6765 290a 2020 2020 2020 2020 7365  ange).        se
-00001830: 6c66 2e61 6374 696f 6e4c 6f67 5f57 696e  lf.actionLog_Win
-00001840: 646f 772e 7472 6967 6765 7265 642e 636f  dow.triggered.co
-00001850: 6e6e 6563 7428 7365 6c66 2e6c 6175 6e63  nnect(self.launc
-00001860: 685f 6c6f 675f 7769 6e64 6f77 290a 2020  h_log_window).  
-00001870: 2020 2020 2020 7365 6c66 2e61 6374 696f        self.actio
-00001880: 6e42 616e 646d 6170 2e74 7269 6767 6572  nBandmap.trigger
-00001890: 6564 2e63 6f6e 6e65 6374 2873 656c 662e  ed.connect(self.
-000018a0: 6c61 756e 6368 5f62 616e 646d 6170 5f77  launch_bandmap_w
-000018b0: 696e 646f 7729 0a20 2020 2020 2020 2073  indow).        s
-000018c0: 656c 662e 6163 7469 6f6e 5265 6361 6c63  elf.actionRecalc
-000018d0: 756c 6174 655f 4d75 6c74 732e 7472 6967  ulate_Mults.trig
-000018e0: 6765 7265 642e 636f 6e6e 6563 7428 7365  gered.connect(se
-000018f0: 6c66 2e72 6563 616c 6375 6c61 7465 5f6d  lf.recalculate_m
-00001900: 756c 7473 290a 0a20 2020 2020 2020 2073  ults)..        s
-00001910: 656c 662e 6163 7469 6f6e 4765 6e65 7261  elf.actionGenera
-00001920: 7465 5f43 6162 7269 6c6c 6f2e 7472 6967  te_Cabrillo.trig
-00001930: 6765 7265 642e 636f 6e6e 6563 7428 7365  gered.connect(se
-00001940: 6c66 2e67 656e 6572 6174 655f 6361 6272  lf.generate_cabr
-00001950: 696c 6c6f 290a 2020 2020 2020 2020 7365  illo).        se
-00001960: 6c66 2e61 6374 696f 6e47 656e 6572 6174  lf.actionGenerat
-00001970: 655f 4144 4946 2e74 7269 6767 6572 6564  e_ADIF.triggered
-00001980: 2e63 6f6e 6e65 6374 2873 656c 662e 6765  .connect(self.ge
-00001990: 6e65 7261 7465 5f61 6469 6629 0a0a 2020  nerate_adif)..  
-000019a0: 2020 2020 2020 7365 6c66 2e61 6374 696f        self.actio
-000019b0: 6e43 6f6e 6669 6775 7261 7469 6f6e 5f53  nConfiguration_S
-000019c0: 6574 7469 6e67 732e 7472 6967 6765 7265  ettings.triggere
-000019d0: 642e 636f 6e6e 6563 7428 0a20 2020 2020  d.connect(.     
-000019e0: 2020 2020 2020 2073 656c 662e 6564 6974         self.edit
-000019f0: 5f63 6f6e 6669 6775 7261 7469 6f6e 5f73  _configuration_s
-00001a00: 6574 7469 6e67 730a 2020 2020 2020 2020  ettings.        
-00001a10: 290a 2020 2020 2020 2020 7365 6c66 2e61  ).        self.a
-00001a20: 6374 696f 6e53 7461 7469 6f6e 5365 7474  ctionStationSett
-00001a30: 696e 6773 2e74 7269 6767 6572 6564 2e63  ings.triggered.c
-00001a40: 6f6e 6e65 6374 2873 656c 662e 6564 6974  onnect(self.edit
-00001a50: 5f73 7461 7469 6f6e 5f73 6574 7469 6e67  _station_setting
-00001a60: 7329 0a0a 2020 2020 2020 2020 7365 6c66  s)..        self
-00001a70: 2e61 6374 696f 6e4e 6577 5f43 6f6e 7465  .actionNew_Conte
-00001a80: 7374 2e74 7269 6767 6572 6564 2e63 6f6e  st.triggered.con
-00001a90: 6e65 6374 2873 656c 662e 6e65 775f 636f  nect(self.new_co
-00001aa0: 6e74 6573 745f 6469 616c 6f67 290a 2020  ntest_dialog).  
-00001ab0: 2020 2020 2020 7365 6c66 2e61 6374 696f        self.actio
-00001ac0: 6e4f 7065 6e5f 436f 6e74 6573 742e 7472  nOpen_Contest.tr
-00001ad0: 6967 6765 7265 642e 636f 6e6e 6563 7428  iggered.connect(
-00001ae0: 7365 6c66 2e6f 7065 6e5f 636f 6e74 6573  self.open_contes
-00001af0: 7429 0a20 2020 2020 2020 2073 656c 662e  t).        self.
-00001b00: 6163 7469 6f6e 4564 6974 5f43 7572 7265  actionEdit_Curre
-00001b10: 6e74 5f43 6f6e 7465 7374 2e74 7269 6767  nt_Contest.trigg
-00001b20: 6572 6564 2e63 6f6e 6e65 6374 2873 656c  ered.connect(sel
-00001b30: 662e 6564 6974 5f63 6f6e 7465 7374 290a  f.edit_contest).
-00001b40: 0a20 2020 2020 2020 2073 656c 662e 6163  .        self.ac
-00001b50: 7469 6f6e 4e65 775f 4461 7461 6261 7365  tionNew_Database
-00001b60: 2e74 7269 6767 6572 6564 2e63 6f6e 6e65  .triggered.conne
-00001b70: 6374 2873 656c 662e 6e65 775f 6461 7461  ct(self.new_data
-00001b80: 6261 7365 290a 2020 2020 2020 2020 7365  base).        se
-00001b90: 6c66 2e61 6374 696f 6e4f 7065 6e5f 4461  lf.actionOpen_Da
-00001ba0: 7461 6261 7365 2e74 7269 6767 6572 6564  tabase.triggered
-00001bb0: 2e63 6f6e 6e65 6374 2873 656c 662e 6f70  .connect(self.op
-00001bc0: 656e 5f64 6174 6162 6173 6529 0a0a 2020  en_database)..  
-00001bd0: 2020 2020 2020 7365 6c66 2e61 6374 696f        self.actio
-00001be0: 6e45 6469 745f 4d61 6372 6f73 2e74 7269  nEdit_Macros.tri
-00001bf0: 6767 6572 6564 2e63 6f6e 6e65 6374 2873  ggered.connect(s
-00001c00: 656c 662e 6564 6974 5f63 775f 6d61 6372  elf.edit_cw_macr
-00001c10: 6f73 290a 0a20 2020 2020 2020 2073 656c  os)..        sel
-00001c20: 662e 6163 7469 6f6e 4162 6f75 742e 7472  f.actionAbout.tr
-00001c30: 6967 6765 7265 642e 636f 6e6e 6563 7428  iggered.connect(
-00001c40: 7365 6c66 2e73 686f 775f 6162 6f75 745f  self.show_about_
-00001c50: 6469 616c 6f67 290a 0a20 2020 2020 2020  dialog)..       
-00001c60: 2073 656c 662e 7261 6469 6f42 7574 746f   self.radioButto
-00001c70: 6e5f 7275 6e2e 636c 6963 6b65 642e 636f  n_run.clicked.co
-00001c80: 6e6e 6563 7428 7365 6c66 2e72 756e 5f73  nnect(self.run_s
-00001c90: 705f 6275 7474 6f6e 735f 636c 6963 6b65  p_buttons_clicke
-00001ca0: 6429 0a20 2020 2020 2020 2073 656c 662e  d).        self.
-00001cb0: 7261 6469 6f42 7574 746f 6e5f 7370 2e63  radioButton_sp.c
-00001cc0: 6c69 636b 6564 2e63 6f6e 6e65 6374 2873  licked.connect(s
-00001cd0: 656c 662e 7275 6e5f 7370 5f62 7574 746f  elf.run_sp_butto
-00001ce0: 6e73 5f63 6c69 636b 6564 290a 2020 2020  ns_clicked).    
-00001cf0: 2020 2020 7365 6c66 2e73 636f 7265 2e73      self.score.s
-00001d00: 6574 5465 7874 2822 3022 290a 2020 2020  etText("0").    
-00001d10: 2020 2020 7365 6c66 2e63 616c 6c73 6967      self.callsig
-00001d20: 6e2e 7465 7874 4564 6974 6564 2e63 6f6e  n.textEdited.con
-00001d30: 6e65 6374 2873 656c 662e 6361 6c6c 7369  nect(self.callsi
-00001d40: 676e 5f63 6861 6e67 6564 290a 2020 2020  gn_changed).    
-00001d50: 2020 2020 7365 6c66 2e63 616c 6c73 6967      self.callsig
-00001d60: 6e2e 7265 7475 726e 5072 6573 7365 642e  n.returnPressed.
-00001d70: 636f 6e6e 6563 7428 7365 6c66 2e73 6176  connect(self.sav
-00001d80: 655f 636f 6e74 6163 7429 0a20 2020 2020  e_contact).     
-00001d90: 2020 2073 656c 662e 7365 6e74 2e72 6574     self.sent.ret
-00001da0: 7572 6e50 7265 7373 6564 2e63 6f6e 6e65  urnPressed.conne
-00001db0: 6374 2873 656c 662e 7361 7665 5f63 6f6e  ct(self.save_con
-00001dc0: 7461 6374 290a 2020 2020 2020 2020 7365  tact).        se
-00001dd0: 6c66 2e72 6563 6569 7665 2e72 6574 7572  lf.receive.retur
-00001de0: 6e50 7265 7373 6564 2e63 6f6e 6e65 6374  nPressed.connect
-00001df0: 2873 656c 662e 7361 7665 5f63 6f6e 7461  (self.save_conta
-00001e00: 6374 290a 2020 2020 2020 2020 7365 6c66  ct).        self
-00001e10: 2e6f 7468 6572 5f31 2e72 6574 7572 6e50  .other_1.returnP
-00001e20: 7265 7373 6564 2e63 6f6e 6e65 6374 2873  ressed.connect(s
-00001e30: 656c 662e 7361 7665 5f63 6f6e 7461 6374  elf.save_contact
-00001e40: 290a 2020 2020 2020 2020 7365 6c66 2e6f  ).        self.o
-00001e50: 7468 6572 5f32 2e72 6574 7572 6e50 7265  ther_2.returnPre
-00001e60: 7373 6564 2e63 6f6e 6e65 6374 2873 656c  ssed.connect(sel
-00001e70: 662e 7361 7665 5f63 6f6e 7461 6374 290a  f.save_contact).
-00001e80: 2020 2020 2020 2020 7365 6c66 2e6f 7468          self.oth
-00001e90: 6572 5f32 2e74 6578 7445 6469 7465 642e  er_2.textEdited.
-00001ea0: 636f 6e6e 6563 7428 7365 6c66 2e6f 7468  connect(self.oth
-00001eb0: 6572 5f32 5f63 6861 6e67 6564 290a 2020  er_2_changed).  
-00001ec0: 2020 2020 2020 7365 6c66 2e73 656e 742e        self.sent.
-00001ed0: 7365 7454 6578 7428 2235 3922 290a 2020  setText("59").  
-00001ee0: 2020 2020 2020 7365 6c66 2e72 6563 6569        self.recei
-00001ef0: 7665 2e73 6574 5465 7874 2822 3539 2229  ve.setText("59")
-00001f00: 0a20 2020 2020 2020 2069 636f 6e5f 7061  .        icon_pa
-00001f10: 7468 203d 2057 4f52 4b49 4e47 5f50 4154  th = WORKING_PAT
-00001f20: 4820 2b20 222f 6461 7461 2f22 0a20 2020  H + "/data/".   
-00001f30: 2020 2020 2073 656c 662e 6772 6565 6e64       self.greend
-00001f40: 6f74 203d 2051 7447 7569 2e51 5069 786d  ot = QtGui.QPixm
-00001f50: 6170 2869 636f 6e5f 7061 7468 202b 2022  ap(icon_path + "
-00001f60: 6772 6565 6e64 6f74 2e70 6e67 2229 0a20  greendot.png"). 
-00001f70: 2020 2020 2020 2073 656c 662e 7265 6464         self.redd
-00001f80: 6f74 203d 2051 7447 7569 2e51 5069 786d  ot = QtGui.QPixm
-00001f90: 6170 2869 636f 6e5f 7061 7468 202b 2022  ap(icon_path + "
-00001fa0: 7265 6464 6f74 2e70 6e67 2229 0a20 2020  reddot.png").   
-00001fb0: 2020 2020 2073 656c 662e 6c65 6674 646f       self.leftdo
-00001fc0: 742e 7365 7450 6978 6d61 7028 7365 6c66  t.setPixmap(self
-00001fd0: 2e67 7265 656e 646f 7429 0a20 2020 2020  .greendot).     
-00001fe0: 2020 2073 656c 662e 7269 6768 7464 6f74     self.rightdot
-00001ff0: 2e73 6574 5069 786d 6170 2873 656c 662e  .setPixmap(self.
-00002000: 7265 6464 6f74 290a 0a20 2020 2020 2020  reddot)..       
-00002010: 2073 656c 662e 4631 2e73 6574 436f 6e74   self.F1.setCont
-00002020: 6578 744d 656e 7550 6f6c 6963 7928 5174  extMenuPolicy(Qt
-00002030: 436f 7265 2e51 742e 4375 7374 6f6d 436f  Core.Qt.CustomCo
-00002040: 6e74 6578 744d 656e 7529 0a20 2020 2020  ntextMenu).     
-00002050: 2020 2073 656c 662e 4631 2e63 7573 746f     self.F1.custo
-00002060: 6d43 6f6e 7465 7874 4d65 6e75 5265 7175  mContextMenuRequ
-00002070: 6573 7465 642e 636f 6e6e 6563 7428 7365  ested.connect(se
-00002080: 6c66 2e65 6469 745f 4631 290a 2020 2020  lf.edit_F1).    
-00002090: 2020 2020 7365 6c66 2e46 312e 636c 6963      self.F1.clic
-000020a0: 6b65 642e 636f 6e6e 6563 7428 7365 6c66  ked.connect(self
-000020b0: 2e73 656e 6466 3129 0a20 2020 2020 2020  .sendf1).       
-000020c0: 2073 656c 662e 4632 2e73 6574 436f 6e74   self.F2.setCont
-000020d0: 6578 744d 656e 7550 6f6c 6963 7928 5174  extMenuPolicy(Qt
-000020e0: 436f 7265 2e51 742e 4375 7374 6f6d 436f  Core.Qt.CustomCo
-000020f0: 6e74 6578 744d 656e 7529 0a20 2020 2020  ntextMenu).     
-00002100: 2020 2073 656c 662e 4632 2e63 7573 746f     self.F2.custo
-00002110: 6d43 6f6e 7465 7874 4d65 6e75 5265 7175  mContextMenuRequ
-00002120: 6573 7465 642e 636f 6e6e 6563 7428 7365  ested.connect(se
-00002130: 6c66 2e65 6469 745f 4632 290a 2020 2020  lf.edit_F2).    
-00002140: 2020 2020 7365 6c66 2e46 322e 636c 6963      self.F2.clic
-00002150: 6b65 642e 636f 6e6e 6563 7428 7365 6c66  ked.connect(self
-00002160: 2e73 656e 6466 3229 0a20 2020 2020 2020  .sendf2).       
-00002170: 2073 656c 662e 4633 2e73 6574 436f 6e74   self.F3.setCont
-00002180: 6578 744d 656e 7550 6f6c 6963 7928 5174  extMenuPolicy(Qt
-00002190: 436f 7265 2e51 742e 4375 7374 6f6d 436f  Core.Qt.CustomCo
-000021a0: 6e74 6578 744d 656e 7529 0a20 2020 2020  ntextMenu).     
-000021b0: 2020 2073 656c 662e 4633 2e63 7573 746f     self.F3.custo
-000021c0: 6d43 6f6e 7465 7874 4d65 6e75 5265 7175  mContextMenuRequ
-000021d0: 6573 7465 642e 636f 6e6e 6563 7428 7365  ested.connect(se
-000021e0: 6c66 2e65 6469 745f 4633 290a 2020 2020  lf.edit_F3).    
-000021f0: 2020 2020 7365 6c66 2e46 332e 636c 6963      self.F3.clic
-00002200: 6b65 642e 636f 6e6e 6563 7428 7365 6c66  ked.connect(self
-00002210: 2e73 656e 6466 3329 0a20 2020 2020 2020  .sendf3).       
-00002220: 2073 656c 662e 4634 2e73 6574 436f 6e74   self.F4.setCont
-00002230: 6578 744d 656e 7550 6f6c 6963 7928 5174  extMenuPolicy(Qt
-00002240: 436f 7265 2e51 742e 4375 7374 6f6d 436f  Core.Qt.CustomCo
-00002250: 6e74 6578 744d 656e 7529 0a20 2020 2020  ntextMenu).     
-00002260: 2020 2073 656c 662e 4634 2e63 7573 746f     self.F4.custo
-00002270: 6d43 6f6e 7465 7874 4d65 6e75 5265 7175  mContextMenuRequ
-00002280: 6573 7465 642e 636f 6e6e 6563 7428 7365  ested.connect(se
-00002290: 6c66 2e65 6469 745f 4634 290a 2020 2020  lf.edit_F4).    
-000022a0: 2020 2020 7365 6c66 2e46 342e 636c 6963      self.F4.clic
-000022b0: 6b65 642e 636f 6e6e 6563 7428 7365 6c66  ked.connect(self
-000022c0: 2e73 656e 6466 3429 0a20 2020 2020 2020  .sendf4).       
-000022d0: 2073 656c 662e 4635 2e73 6574 436f 6e74   self.F5.setCont
-000022e0: 6578 744d 656e 7550 6f6c 6963 7928 5174  extMenuPolicy(Qt
-000022f0: 436f 7265 2e51 742e 4375 7374 6f6d 436f  Core.Qt.CustomCo
-00002300: 6e74 6578 744d 656e 7529 0a20 2020 2020  ntextMenu).     
-00002310: 2020 2073 656c 662e 4635 2e63 7573 746f     self.F5.custo
-00002320: 6d43 6f6e 7465 7874 4d65 6e75 5265 7175  mContextMenuRequ
-00002330: 6573 7465 642e 636f 6e6e 6563 7428 7365  ested.connect(se
-00002340: 6c66 2e65 6469 745f 4635 290a 2020 2020  lf.edit_F5).    
-00002350: 2020 2020 7365 6c66 2e46 352e 636c 6963      self.F5.clic
-00002360: 6b65 642e 636f 6e6e 6563 7428 7365 6c66  ked.connect(self
-00002370: 2e73 656e 6466 3529 0a20 2020 2020 2020  .sendf5).       
-00002380: 2073 656c 662e 4636 2e73 6574 436f 6e74   self.F6.setCont
-00002390: 6578 744d 656e 7550 6f6c 6963 7928 5174  extMenuPolicy(Qt
-000023a0: 436f 7265 2e51 742e 4375 7374 6f6d 436f  Core.Qt.CustomCo
-000023b0: 6e74 6578 744d 656e 7529 0a20 2020 2020  ntextMenu).     
-000023c0: 2020 2073 656c 662e 4636 2e63 7573 746f     self.F6.custo
-000023d0: 6d43 6f6e 7465 7874 4d65 6e75 5265 7175  mContextMenuRequ
-000023e0: 6573 7465 642e 636f 6e6e 6563 7428 7365  ested.connect(se
-000023f0: 6c66 2e65 6469 745f 4636 290a 2020 2020  lf.edit_F6).    
-00002400: 2020 2020 7365 6c66 2e46 362e 636c 6963      self.F6.clic
-00002410: 6b65 642e 636f 6e6e 6563 7428 7365 6c66  ked.connect(self
-00002420: 2e73 656e 6466 3629 0a20 2020 2020 2020  .sendf6).       
-00002430: 2073 656c 662e 4637 2e73 6574 436f 6e74   self.F7.setCont
-00002440: 6578 744d 656e 7550 6f6c 6963 7928 5174  extMenuPolicy(Qt
-00002450: 436f 7265 2e51 742e 4375 7374 6f6d 436f  Core.Qt.CustomCo
-00002460: 6e74 6578 744d 656e 7529 0a20 2020 2020  ntextMenu).     
-00002470: 2020 2073 656c 662e 4637 2e63 7573 746f     self.F7.custo
-00002480: 6d43 6f6e 7465 7874 4d65 6e75 5265 7175  mContextMenuRequ
-00002490: 6573 7465 642e 636f 6e6e 6563 7428 7365  ested.connect(se
-000024a0: 6c66 2e65 6469 745f 4637 290a 2020 2020  lf.edit_F7).    
-000024b0: 2020 2020 7365 6c66 2e46 372e 636c 6963      self.F7.clic
-000024c0: 6b65 642e 636f 6e6e 6563 7428 7365 6c66  ked.connect(self
-000024d0: 2e73 656e 6466 3729 0a20 2020 2020 2020  .sendf7).       
-000024e0: 2073 656c 662e 4638 2e73 6574 436f 6e74   self.F8.setCont
-000024f0: 6578 744d 656e 7550 6f6c 6963 7928 5174  extMenuPolicy(Qt
-00002500: 436f 7265 2e51 742e 4375 7374 6f6d 436f  Core.Qt.CustomCo
-00002510: 6e74 6578 744d 656e 7529 0a20 2020 2020  ntextMenu).     
-00002520: 2020 2073 656c 662e 4638 2e63 7573 746f     self.F8.custo
-00002530: 6d43 6f6e 7465 7874 4d65 6e75 5265 7175  mContextMenuRequ
-00002540: 6573 7465 642e 636f 6e6e 6563 7428 7365  ested.connect(se
-00002550: 6c66 2e65 6469 745f 4638 290a 2020 2020  lf.edit_F8).    
-00002560: 2020 2020 7365 6c66 2e46 382e 636c 6963      self.F8.clic
-00002570: 6b65 642e 636f 6e6e 6563 7428 7365 6c66  ked.connect(self
-00002580: 2e73 656e 6466 3829 0a20 2020 2020 2020  .sendf8).       
-00002590: 2073 656c 662e 4639 2e73 6574 436f 6e74   self.F9.setCont
-000025a0: 6578 744d 656e 7550 6f6c 6963 7928 5174  extMenuPolicy(Qt
-000025b0: 436f 7265 2e51 742e 4375 7374 6f6d 436f  Core.Qt.CustomCo
-000025c0: 6e74 6578 744d 656e 7529 0a20 2020 2020  ntextMenu).     
-000025d0: 2020 2073 656c 662e 4639 2e63 7573 746f     self.F9.custo
-000025e0: 6d43 6f6e 7465 7874 4d65 6e75 5265 7175  mContextMenuRequ
-000025f0: 6573 7465 642e 636f 6e6e 6563 7428 7365  ested.connect(se
-00002600: 6c66 2e65 6469 745f 4639 290a 2020 2020  lf.edit_F9).    
-00002610: 2020 2020 7365 6c66 2e46 392e 636c 6963      self.F9.clic
-00002620: 6b65 642e 636f 6e6e 6563 7428 7365 6c66  ked.connect(self
-00002630: 2e73 656e 6466 3929 0a20 2020 2020 2020  .sendf9).       
-00002640: 2073 656c 662e 4631 302e 7365 7443 6f6e   self.F10.setCon
-00002650: 7465 7874 4d65 6e75 506f 6c69 6379 2851  textMenuPolicy(Q
-00002660: 7443 6f72 652e 5174 2e43 7573 746f 6d43  tCore.Qt.CustomC
-00002670: 6f6e 7465 7874 4d65 6e75 290a 2020 2020  ontextMenu).    
-00002680: 2020 2020 7365 6c66 2e46 3130 2e63 7573      self.F10.cus
-00002690: 746f 6d43 6f6e 7465 7874 4d65 6e75 5265  tomContextMenuRe
-000026a0: 7175 6573 7465 642e 636f 6e6e 6563 7428  quested.connect(
-000026b0: 7365 6c66 2e65 6469 745f 4631 3029 0a20  self.edit_F10). 
-000026c0: 2020 2020 2020 2073 656c 662e 4631 302e         self.F10.
-000026d0: 636c 6963 6b65 642e 636f 6e6e 6563 7428  clicked.connect(
-000026e0: 7365 6c66 2e73 656e 6466 3130 290a 2020  self.sendf10).  
-000026f0: 2020 2020 2020 7365 6c66 2e46 3131 2e73        self.F11.s
-00002700: 6574 436f 6e74 6578 744d 656e 7550 6f6c  etContextMenuPol
-00002710: 6963 7928 5174 436f 7265 2e51 742e 4375  icy(QtCore.Qt.Cu
-00002720: 7374 6f6d 436f 6e74 6578 744d 656e 7529  stomContextMenu)
-00002730: 0a20 2020 2020 2020 2073 656c 662e 4631  .        self.F1
-00002740: 312e 6375 7374 6f6d 436f 6e74 6578 744d  1.customContextM
-00002750: 656e 7552 6571 7565 7374 6564 2e63 6f6e  enuRequested.con
-00002760: 6e65 6374 2873 656c 662e 6564 6974 5f46  nect(self.edit_F
-00002770: 3131 290a 2020 2020 2020 2020 7365 6c66  11).        self
-00002780: 2e46 3131 2e63 6c69 636b 6564 2e63 6f6e  .F11.clicked.con
-00002790: 6e65 6374 2873 656c 662e 7365 6e64 6631  nect(self.sendf1
-000027a0: 3129 0a20 2020 2020 2020 2073 656c 662e  1).        self.
-000027b0: 4631 322e 7365 7443 6f6e 7465 7874 4d65  F12.setContextMe
-000027c0: 6e75 506f 6c69 6379 2851 7443 6f72 652e  nuPolicy(QtCore.
-000027d0: 5174 2e43 7573 746f 6d43 6f6e 7465 7874  Qt.CustomContext
-000027e0: 4d65 6e75 290a 2020 2020 2020 2020 7365  Menu).        se
-000027f0: 6c66 2e46 3132 2e63 7573 746f 6d43 6f6e  lf.F12.customCon
-00002800: 7465 7874 4d65 6e75 5265 7175 6573 7465  textMenuRequeste
-00002810: 642e 636f 6e6e 6563 7428 7365 6c66 2e65  d.connect(self.e
-00002820: 6469 745f 4631 3229 0a20 2020 2020 2020  dit_F12).       
-00002830: 2073 656c 662e 4631 322e 636c 6963 6b65   self.F12.clicke
-00002840: 642e 636f 6e6e 6563 7428 7365 6c66 2e73  d.connect(self.s
-00002850: 656e 6466 3132 290a 0a20 2020 2020 2020  endf12)..       
-00002860: 2073 656c 662e 7265 6164 7072 6566 6572   self.readprefer
-00002870: 656e 6365 7328 290a 2020 2020 2020 2020  ences().        
-00002880: 7365 6c66 2e64 626e 616d 6520 3d20 4441  self.dbname = DA
-00002890: 5441 5f50 4154 4820 2b20 222f 2220 2b20  TA_PATH + "/" + 
-000028a0: 7365 6c66 2e70 7265 662e 6765 7428 2263  self.pref.get("c
-000028b0: 7572 7265 6e74 5f64 6174 6162 6173 6522  urrent_database"
-000028c0: 2c20 2268 616d 2e64 6222 290a 2020 2020  , "ham.db").    
-000028d0: 2020 2020 7365 6c66 2e64 6174 6162 6173      self.databas
-000028e0: 6520 3d20 4461 7461 4261 7365 2873 656c  e = DataBase(sel
-000028f0: 662e 6462 6e61 6d65 2c20 574f 524b 494e  f.dbname, WORKIN
-00002900: 475f 5041 5448 290a 2020 2020 2020 2020  G_PATH).        
-00002910: 7365 6c66 2e73 7461 7469 6f6e 203d 2073  self.station = s
-00002920: 656c 662e 6461 7461 6261 7365 2e66 6574  elf.database.fet
-00002930: 6368 5f73 7461 7469 6f6e 2829 0a20 2020  ch_station().   
-00002940: 2020 2020 2069 6620 7365 6c66 2e73 7461       if self.sta
-00002950: 7469 6f6e 2069 7320 4e6f 6e65 3a0a 2020  tion is None:.  
-00002960: 2020 2020 2020 2020 2020 7365 6c66 2e73            self.s
-00002970: 7461 7469 6f6e 203d 207b 7d0a 2020 2020  tation = {}.    
-00002980: 2020 2020 2020 2020 7365 6c66 2e65 6469          self.edi
-00002990: 745f 7374 6174 696f 6e5f 7365 7474 696e  t_station_settin
-000029a0: 6773 2829 0a20 2020 2020 2020 2020 2020  gs().           
-000029b0: 2073 656c 662e 7374 6174 696f 6e20 3d20   self.station = 
-000029c0: 7365 6c66 2e64 6174 6162 6173 652e 6665  self.database.fe
-000029d0: 7463 685f 7374 6174 696f 6e28 290a 2020  tch_station().  
-000029e0: 2020 2020 2020 2020 2020 6966 2073 656c            if sel
-000029f0: 662e 7374 6174 696f 6e20 6973 204e 6f6e  f.station is Non
-00002a00: 653a 0a20 2020 2020 2020 2020 2020 2020  e:.             
-00002a10: 2020 2073 656c 662e 7374 6174 696f 6e20     self.station 
-00002a20: 3d20 7b7d 0a20 2020 2020 2020 2073 656c  = {}.        sel
-00002a30: 662e 636f 6e74 6163 7420 3d20 7365 6c66  f.contact = self
-00002a40: 2e64 6174 6162 6173 652e 656d 7074 795f  .database.empty_
-00002a50: 636f 6e74 6163 740a 2020 2020 2020 2020  contact.        
-00002a60: 7365 6c66 2e63 7572 7265 6e74 5f6f 7020  self.current_op 
-00002a70: 3d20 7365 6c66 2e73 7461 7469 6f6e 2e67  = self.station.g
-00002a80: 6574 2822 4361 6c6c 222c 2022 2229 0a20  et("Call", ""). 
-00002a90: 2020 2020 2020 2073 656c 662e 6d61 6b65         self.make
-00002aa0: 5f6f 705f 6469 7228 290a 2020 2020 2020  _op_dir().      
-00002ab0: 2020 6966 2073 656c 662e 7072 6566 2e67    if self.pref.g
-00002ac0: 6574 2822 636f 6e74 6573 7422 293a 0a20  et("contest"):. 
-00002ad0: 2020 2020 2020 2020 2020 2073 656c 662e             self.
-00002ae0: 6c6f 6164 5f63 6f6e 7465 7374 2829 0a0a  load_contest()..
-00002af0: 2020 2020 2020 2020 7365 6c66 2e72 6561          self.rea
-00002b00: 645f 6377 5f6d 6163 726f 7328 290a 2020  d_cw_macros().  
-00002b10: 2020 2020 2020 7365 6c66 2e63 6c65 6172        self.clear
-00002b20: 696e 7075 7473 2829 0a20 2020 2020 2020  inputs().       
-00002b30: 2023 2073 656c 662e 6c61 756e 6368 5f6c   # self.launch_l
-00002b40: 6f67 5f77 696e 646f 7728 290a 0a20 2020  og_window()..   
-00002b50: 2020 2020 2073 656c 662e 6261 6e64 5f69       self.band_i
-00002b60: 6e64 6963 6174 6f72 735f 6377 203d 207b  ndicators_cw = {
-00002b70: 0a20 2020 2020 2020 2020 2020 2022 3136  .            "16
-00002b80: 3022 3a20 7365 6c66 2e63 775f 6261 6e64  0": self.cw_band
-00002b90: 5f31 3630 2c0a 2020 2020 2020 2020 2020  _160,.          
-00002ba0: 2020 2238 3022 3a20 7365 6c66 2e63 775f    "80": self.cw_
-00002bb0: 6261 6e64 5f38 302c 0a20 2020 2020 2020  band_80,.       
-00002bc0: 2020 2020 2022 3430 223a 2073 656c 662e       "40": self.
-00002bd0: 6377 5f62 616e 645f 3430 2c0a 2020 2020  cw_band_40,.    
-00002be0: 2020 2020 2020 2020 2232 3022 3a20 7365          "20": se
-00002bf0: 6c66 2e63 775f 6261 6e64 5f32 302c 0a20  lf.cw_band_20,. 
-00002c00: 2020 2020 2020 2020 2020 2022 3135 223a             "15":
-00002c10: 2073 656c 662e 6377 5f62 616e 645f 3135   self.cw_band_15
-00002c20: 2c0a 2020 2020 2020 2020 2020 2020 2231  ,.            "1
-00002c30: 3022 3a20 7365 6c66 2e63 775f 6261 6e64  0": self.cw_band
-00002c40: 5f31 302c 0a20 2020 2020 2020 207d 0a0a  _10,.        }..
-00002c50: 2020 2020 2020 2020 7365 6c66 2e62 616e          self.ban
-00002c60: 645f 696e 6469 6361 746f 7273 5f73 7362  d_indicators_ssb
-00002c70: 203d 207b 0a20 2020 2020 2020 2020 2020   = {.           
-00002c80: 2022 3136 3022 3a20 7365 6c66 2e73 7362   "160": self.ssb
-00002c90: 5f62 616e 645f 3136 302c 0a20 2020 2020  _band_160,.     
-00002ca0: 2020 2020 2020 2022 3830 223a 2073 656c         "80": sel
-00002cb0: 662e 7373 625f 6261 6e64 5f38 302c 0a20  f.ssb_band_80,. 
-00002cc0: 2020 2020 2020 2020 2020 2022 3430 223a             "40":
-00002cd0: 2073 656c 662e 7373 625f 6261 6e64 5f34   self.ssb_band_4
-00002ce0: 302c 0a20 2020 2020 2020 2020 2020 2022  0,.            "
-00002cf0: 3230 223a 2073 656c 662e 7373 625f 6261  20": self.ssb_ba
-00002d00: 6e64 5f32 302c 0a20 2020 2020 2020 2020  nd_20,.         
-00002d10: 2020 2022 3135 223a 2073 656c 662e 7373     "15": self.ss
-00002d20: 625f 6261 6e64 5f31 352c 0a20 2020 2020  b_band_15,.     
-00002d30: 2020 2020 2020 2022 3130 223a 2073 656c         "10": sel
-00002d40: 662e 7373 625f 6261 6e64 5f31 302c 0a20  f.ssb_band_10,. 
-00002d50: 2020 2020 2020 207d 0a0a 2020 2020 2020         }..      
-00002d60: 2020 7365 6c66 2e62 616e 645f 696e 6469    self.band_indi
-00002d70: 6361 746f 7273 5f72 7474 7920 3d20 7b0a  cators_rtty = {.
-00002d80: 2020 2020 2020 2020 2020 2020 2231 3630              "160
-00002d90: 223a 2073 656c 662e 7274 7479 5f62 616e  ": self.rtty_ban
-00002da0: 645f 3136 302c 0a20 2020 2020 2020 2020  d_160,.         
-00002db0: 2020 2022 3830 223a 2073 656c 662e 7274     "80": self.rt
-00002dc0: 7479 5f62 616e 645f 3830 2c0a 2020 2020  ty_band_80,.    
-00002dd0: 2020 2020 2020 2020 2234 3022 3a20 7365          "40": se
-00002de0: 6c66 2e72 7474 795f 6261 6e64 5f34 302c  lf.rtty_band_40,
-00002df0: 0a20 2020 2020 2020 2020 2020 2022 3230  .            "20
-00002e00: 223a 2073 656c 662e 7274 7479 5f62 616e  ": self.rtty_ban
-00002e10: 645f 3230 2c0a 2020 2020 2020 2020 2020  d_20,.          
-00002e20: 2020 2231 3522 3a20 7365 6c66 2e72 7474    "15": self.rtt
-00002e30: 795f 6261 6e64 5f31 352c 0a20 2020 2020  y_band_15,.     
-00002e40: 2020 2020 2020 2022 3130 223a 2073 656c         "10": sel
-00002e50: 662e 7274 7479 5f62 616e 645f 3130 2c0a  f.rtty_band_10,.
-00002e60: 2020 2020 2020 2020 7d0a 0a20 2020 2020          }..     
-00002e70: 2020 2073 656c 662e 616c 6c5f 6d6f 6465     self.all_mode
-00002e80: 5f69 6e64 6963 6174 6f72 7320 3d20 7b0a  _indicators = {.
-00002e90: 2020 2020 2020 2020 2020 2020 2243 5722              "CW"
-00002ea0: 3a20 7365 6c66 2e62 616e 645f 696e 6469  : self.band_indi
-00002eb0: 6361 746f 7273 5f63 772c 0a20 2020 2020  cators_cw,.     
-00002ec0: 2020 2020 2020 2022 5353 4222 3a20 7365         "SSB": se
-00002ed0: 6c66 2e62 616e 645f 696e 6469 6361 746f  lf.band_indicato
-00002ee0: 7273 5f73 7362 2c0a 2020 2020 2020 2020  rs_ssb,.        
-00002ef0: 2020 2020 2252 5454 5922 3a20 7365 6c66      "RTTY": self
-00002f00: 2e62 616e 645f 696e 6469 6361 746f 7273  .band_indicators
-00002f10: 5f72 7474 792c 0a20 2020 2020 2020 207d  _rtty,.        }
-00002f20: 0a20 2020 2020 2020 2069 6620 7365 6c66  .        if self
-00002f30: 2e5f 7564 7077 6174 6368 2069 7320 4e6f  ._udpwatch is No
-00002f40: 6e65 3a0a 2020 2020 2020 2020 2020 2020  ne:.            
-00002f50: 7365 6c66 2e5f 7564 7077 6174 6368 203d  self._udpwatch =
-00002f60: 2074 6872 6561 6469 6e67 2e54 6872 6561   threading.Threa
-00002f70: 6428 0a20 2020 2020 2020 2020 2020 2020  d(.             
-00002f80: 2020 2074 6172 6765 743d 7365 6c66 2e77     target=self.w
-00002f90: 6174 6368 5f75 6470 2c0a 2020 2020 2020  atch_udp,.      
-00002fa0: 2020 2020 2020 2020 2020 6461 656d 6f6e            daemon
-00002fb0: 3d54 7275 652c 0a20 2020 2020 2020 2020  =True,.         
-00002fc0: 2020 2029 0a20 2020 2020 2020 2020 2020     ).           
-00002fd0: 2073 656c 662e 5f75 6470 7761 7463 682e   self._udpwatch.
-00002fe0: 7374 6172 7428 290a 0a20 2020 2040 7374  start()..    @st
-00002ff0: 6174 6963 6d65 7468 6f64 0a20 2020 2064  aticmethod.    d
-00003000: 6566 2063 6865 636b 5f70 726f 6365 7373  ef check_process
-00003010: 286e 616d 653a 2073 7472 2920 2d3e 2062  (name: str) -> b
-00003020: 6f6f 6c3a 0a20 2020 2020 2020 2022 2222  ool:.        """
-00003030: 6368 6563 6b73 2074 6f20 7365 6520 6966  checks to see if
-00003040: 2070 726f 6772 616d 206f 6620 6e61 6d65   program of name
-00003050: 2069 7320 696e 2074 6865 2061 6374 6976   is in the activ
-00003060: 6520 7072 6f63 6573 7320 6c69 7374 2222  e process list""
-00003070: 220a 2020 2020 2020 2020 666f 7220 7072  ".        for pr
-00003080: 6f63 2069 6e20 7073 7574 696c 2e70 726f  oc in psutil.pro
-00003090: 6365 7373 5f69 7465 7228 293a 0a20 2020  cess_iter():.   
-000030a0: 2020 2020 2020 2020 2069 6620 626f 6f6c           if bool
-000030b0: 2872 652e 6d61 7463 6828 6e61 6d65 2c20  (re.match(name, 
-000030c0: 7072 6f63 2e6e 616d 6528 292e 6c6f 7765  proc.name().lowe
-000030d0: 7228 2929 293a 0a20 2020 2020 2020 2020  r())):.         
-000030e0: 2020 2020 2020 2072 6574 7572 6e20 5472         return Tr
-000030f0: 7565 0a20 2020 2020 2020 2072 6574 7572  ue.        retur
-00003100: 6e20 4661 6c73 650a 0a20 2020 2064 6566  n False..    def
-00003110: 2073 686f 775f 6d65 7373 6167 655f 626f   show_message_bo
-00003120: 7828 7365 6c66 2c20 6d65 7373 6167 653a  x(self, message:
-00003130: 2073 7472 2920 2d3e 204e 6f6e 653a 0a20   str) -> None:. 
-00003140: 2020 2020 2020 2022 2222 646f 6322 2222         """doc"""
-00003150: 0a20 2020 2020 2020 206d 6573 7361 6765  .        message
-00003160: 5f62 6f78 203d 2051 7457 6964 6765 7473  _box = QtWidgets
-00003170: 2e51 4d65 7373 6167 6542 6f78 2829 0a20  .QMessageBox(). 
-00003180: 2020 2020 2020 206d 6573 7361 6765 5f62         message_b
-00003190: 6f78 2e73 6574 4963 6f6e 2851 7457 6964  ox.setIcon(QtWid
-000031a0: 6765 7473 2e51 4d65 7373 6167 6542 6f78  gets.QMessageBox
-000031b0: 2e49 6e66 6f72 6d61 7469 6f6e 290a 2020  .Information).  
-000031c0: 2020 2020 2020 6d65 7373 6167 655f 626f        message_bo
-000031d0: 782e 7365 7454 6578 7428 6d65 7373 6167  x.setText(messag
-000031e0: 6529 0a20 2020 2020 2020 206d 6573 7361  e).        messa
-000031f0: 6765 5f62 6f78 2e73 6574 5769 6e64 6f77  ge_box.setWindow
-00003200: 5469 746c 6528 2249 6e66 6f72 6d61 7469  Title("Informati
-00003210: 6f6e 2229 0a20 2020 2020 2020 206d 6573  on").        mes
-00003220: 7361 6765 5f62 6f78 2e73 6574 5374 616e  sage_box.setStan
-00003230: 6461 7264 4275 7474 6f6e 7328 5174 5769  dardButtons(QtWi
-00003240: 6467 6574 732e 514d 6573 7361 6765 426f  dgets.QMessageBo
-00003250: 782e 4f6b 290a 2020 2020 2020 2020 5f20  x.Ok).        _ 
-00003260: 3d20 6d65 7373 6167 655f 626f 782e 6578  = message_box.ex
-00003270: 6563 5f28 290a 0a20 2020 2064 6566 2073  ec_()..    def s
-00003280: 686f 775f 6162 6f75 745f 6469 616c 6f67  how_about_dialog
-00003290: 2873 656c 6629 3a0a 2020 2020 2020 2020  (self):.        
-000032a0: 2222 2253 686f 7720 6162 6f75 7420 6469  """Show about di
-000032b0: 616c 6f67 2222 220a 2020 2020 2020 2020  alog""".        
-000032c0: 7365 6c66 2e61 626f 7574 5f64 6961 6c6f  self.about_dialo
-000032d0: 6720 3d20 4162 6f75 7428 574f 524b 494e  g = About(WORKIN
-000032e0: 475f 5041 5448 290a 2020 2020 2020 2020  G_PATH).        
-000032f0: 6966 2073 656c 662e 7072 6566 2e67 6574  if self.pref.get
-00003300: 2822 6461 726b 5f6d 6f64 6522 293a 0a20  ("dark_mode"):. 
-00003310: 2020 2020 2020 2020 2020 2073 656c 662e             self.
-00003320: 6162 6f75 745f 6469 616c 6f67 2e73 6574  about_dialog.set
-00003330: 5374 796c 6553 6865 6574 2844 4152 4b5f  StyleSheet(DARK_
-00003340: 5354 594c 4553 4845 4554 290a 2020 2020  STYLESHEET).    
-00003350: 2020 2020 7365 6c66 2e61 626f 7574 5f64      self.about_d
-00003360: 6961 6c6f 672e 6f70 656e 2829 0a0a 2020  ialog.open()..  
-00003370: 2020 6465 6620 6564 6974 5f63 6f6e 6669    def edit_confi
-00003380: 6775 7261 7469 6f6e 5f73 6574 7469 6e67  guration_setting
-00003390: 7328 7365 6c66 293a 0a20 2020 2020 2020  s(self):.       
-000033a0: 2022 2222 436f 6e66 6967 7572 6174 696f   """Configuratio
-000033b0: 6e20 5365 7474 696e 6773 2077 6173 2063  n Settings was c
-000033c0: 6c69 636b 6564 2222 220a 2020 2020 2020  licked""".      
-000033d0: 2020 7365 6c66 2e63 6f6e 6669 6775 7261    self.configura
-000033e0: 7469 6f6e 5f64 6961 6c6f 6720 3d20 5365  tion_dialog = Se
-000033f0: 7474 696e 6773 2857 4f52 4b49 4e47 5f50  ttings(WORKING_P
-00003400: 4154 482c 2043 4f4e 4649 475f 5041 5448  ATH, CONFIG_PATH
-00003410: 2c20 7365 6c66 2e70 7265 6629 0a20 2020  , self.pref).   
-00003420: 2020 2020 2069 6620 7365 6c66 2e70 7265       if self.pre
-00003430: 662e 6765 7428 2264 6172 6b5f 6d6f 6465  f.get("dark_mode
-00003440: 2229 3a0a 2020 2020 2020 2020 2020 2020  "):.            
-00003450: 7365 6c66 2e63 6f6e 6669 6775 7261 7469  self.configurati
-00003460: 6f6e 5f64 6961 6c6f 672e 7365 7453 7479  on_dialog.setSty
-00003470: 6c65 5368 6565 7428 4441 524b 5f53 5459  leSheet(DARK_STY
-00003480: 4c45 5348 4545 5429 0a20 2020 2020 2020  LESHEET).       
-00003490: 2073 656c 662e 636f 6e66 6967 7572 6174   self.configurat
-000034a0: 696f 6e5f 6469 616c 6f67 2e75 7365 6861  ion_dialog.useha
-000034b0: 6d64 625f 7261 6469 6f42 7574 746f 6e2e  mdb_radioButton.
-000034c0: 6869 6465 2829 0a20 2020 2020 2020 2023  hide().        #
-000034d0: 2073 656c 662e 636f 6e66 6967 7572 6174   self.configurat
-000034e0: 696f 6e5f 6469 616c 6f67 2e6e 316d 6d5f  ion_dialog.n1mm_
-000034f0: 7461 622e 6869 6465 2829 0a20 2020 2020  tab.hide().     
-00003500: 2020 2073 656c 662e 636f 6e66 6967 7572     self.configur
-00003510: 6174 696f 6e5f 6469 616c 6f67 2e73 686f  ation_dialog.sho
-00003520: 7728 290a 2020 2020 2020 2020 7365 6c66  w().        self
-00003530: 2e63 6f6e 6669 6775 7261 7469 6f6e 5f64  .configuration_d
-00003540: 6961 6c6f 672e 6163 6365 7074 6564 2e63  ialog.accepted.c
-00003550: 6f6e 6e65 6374 2873 656c 662e 6564 6974  onnect(self.edit
-00003560: 5f63 6f6e 6669 6775 7261 7469 6f6e 5f72  _configuration_r
-00003570: 6574 7572 6e29 0a0a 2020 2020 6465 6620  eturn)..    def 
-00003580: 6564 6974 5f63 6f6e 6669 6775 7261 7469  edit_configurati
-00003590: 6f6e 5f72 6574 7572 6e28 7365 6c66 293a  on_return(self):
-000035a0: 0a20 2020 2020 2020 2022 2222 5265 7475  .        """Retu
-000035b0: 726e 7320 6865 7265 2077 6865 6e20 636f  rns here when co
-000035c0: 6e66 6967 7572 6174 696f 6e20 6469 616c  nfiguration dial
-000035d0: 6f67 2063 6c6f 7365 6420 7769 7468 206f  og closed with o
-000035e0: 6b61 792e 2222 220a 2020 2020 2020 2020  kay.""".        
-000035f0: 7365 6c66 2e63 6f6e 6669 6775 7261 7469  self.configurati
-00003600: 6f6e 5f64 6961 6c6f 672e 7361 7665 5f63  on_dialog.save_c
-00003610: 6861 6e67 6573 2829 0a20 2020 2020 2020  hanges().       
-00003620: 2073 656c 662e 7772 6974 655f 7072 6566   self.write_pref
-00003630: 6572 656e 6365 2829 0a20 2020 2020 2020  erence().       
-00003640: 206c 6f67 6765 722e 6465 6275 6728 2225   logger.debug("%
-00003650: 7322 2c20 6622 7b73 656c 662e 7072 6566  s", f"{self.pref
-00003660: 7d22 290a 2020 2020 2020 2020 7365 6c66  }").        self
-00003670: 2e72 6561 6470 7265 6665 7265 6e63 6573  .readpreferences
-00003680: 2829 0a0a 2020 2020 6465 6620 6e65 775f  ()..    def new_
-00003690: 6461 7461 6261 7365 2873 656c 6629 3a0a  database(self):.
-000036a0: 2020 2020 2020 2020 2222 2243 7265 6174          """Creat
-000036b0: 6520 6e65 7720 6461 7461 6261 7365 2e22  e new database."
-000036c0: 2222 0a20 2020 2020 2020 2066 696c 656e  "".        filen
-000036d0: 616d 6520 3d20 7365 6c66 2e66 696c 6570  ame = self.filep
-000036e0: 6963 6b65 7228 226e 6577 2229 0a20 2020  icker("new").   
-000036f0: 2020 2020 2069 6620 6669 6c65 6e61 6d65       if filename
-00003700: 3a0a 2020 2020 2020 2020 2020 2020 6966  :.            if
-00003710: 2066 696c 656e 616d 655b 2d33 3a5d 2021   filename[-3:] !
-00003720: 3d20 222e 6462 223a 0a20 2020 2020 2020  = ".db":.       
-00003730: 2020 2020 2020 2020 2066 696c 656e 616d           filenam
-00003740: 6520 2b3d 2022 2e64 6222 0a20 2020 2020  e += ".db".     
-00003750: 2020 2020 2020 2073 656c 662e 7072 6566         self.pref
-00003760: 5b22 6375 7272 656e 745f 6461 7461 6261  ["current_databa
-00003770: 7365 225d 203d 2066 696c 656e 616d 652e  se"] = filename.
-00003780: 7370 6c69 7428 222f 2229 5b2d 313a 5d5b  split("/")[-1:][
-00003790: 305d 0a20 2020 2020 2020 2020 2020 2073  0].            s
-000037a0: 656c 662e 7772 6974 655f 7072 6566 6572  elf.write_prefer
-000037b0: 656e 6365 2829 0a20 2020 2020 2020 2020  ence().         
-000037c0: 2020 2073 656c 662e 6462 6e61 6d65 203d     self.dbname =
-000037d0: 2044 4154 415f 5041 5448 202b 2022 2f22   DATA_PATH + "/"
-000037e0: 202b 2073 656c 662e 7072 6566 2e67 6574   + self.pref.get
-000037f0: 2822 6375 7272 656e 745f 6461 7461 6261  ("current_databa
-00003800: 7365 222c 2022 6861 6d2e 6462 2229 0a20  se", "ham.db"). 
-00003810: 2020 2020 2020 2020 2020 2073 656c 662e             self.
-00003820: 6461 7461 6261 7365 203d 2044 6174 6142  database = DataB
-00003830: 6173 6528 7365 6c66 2e64 626e 616d 652c  ase(self.dbname,
-00003840: 2057 4f52 4b49 4e47 5f50 4154 4829 0a20   WORKING_PATH). 
-00003850: 2020 2020 2020 2020 2020 2073 656c 662e             self.
-00003860: 636f 6e74 6163 7420 3d20 7365 6c66 2e64  contact = self.d
-00003870: 6174 6162 6173 652e 656d 7074 795f 636f  atabase.empty_co
-00003880: 6e74 6163 740a 2020 2020 2020 2020 2020  ntact.          
-00003890: 2020 7365 6c66 2e73 7461 7469 6f6e 203d    self.station =
-000038a0: 2073 656c 662e 6461 7461 6261 7365 2e66   self.database.f
-000038b0: 6574 6368 5f73 7461 7469 6f6e 2829 0a20  etch_station(). 
-000038c0: 2020 2020 2020 2020 2020 2069 6620 7365             if se
-000038d0: 6c66 2e73 7461 7469 6f6e 2069 7320 4e6f  lf.station is No
-000038e0: 6e65 3a0a 2020 2020 2020 2020 2020 2020  ne:.            
-000038f0: 2020 2020 7365 6c66 2e73 7461 7469 6f6e      self.station
-00003900: 203d 207b 7d0a 2020 2020 2020 2020 2020   = {}.          
-00003910: 2020 7365 6c66 2e63 7572 7265 6e74 5f6f    self.current_o
-00003920: 7020 3d20 7365 6c66 2e73 7461 7469 6f6e  p = self.station
-00003930: 2e67 6574 2822 4361 6c6c 222c 2022 2229  .get("Call", "")
-00003940: 0a20 2020 2020 2020 2020 2020 2073 656c  .            sel
-00003950: 662e 6d61 6b65 5f6f 705f 6469 7228 290a  f.make_op_dir().
-00003960: 2020 2020 2020 2020 2020 2020 636d 6420              cmd 
-00003970: 3d20 7b7d 0a20 2020 2020 2020 2020 2020  = {}.           
-00003980: 2063 6d64 5b22 636d 6422 5d20 3d20 224e   cmd["cmd"] = "N
-00003990: 4557 4442 220a 2020 2020 2020 2020 2020  EWDB".          
-000039a0: 2020 636d 645b 2273 7461 7469 6f6e 225d    cmd["station"]
-000039b0: 203d 2070 6c61 7466 6f72 6d2e 6e6f 6465   = platform.node
-000039c0: 2829 0a20 2020 2020 2020 2020 2020 2073  ().            s
-000039d0: 656c 662e 6d75 6c74 6963 6173 745f 696e  elf.multicast_in
-000039e0: 7465 7266 6163 652e 7365 6e64 5f61 735f  terface.send_as_
-000039f0: 6a73 6f6e 2863 6d64 290a 2020 2020 2020  json(cmd).      
-00003a00: 2020 2020 2020 7365 6c66 2e63 6c65 6172        self.clear
-00003a10: 696e 7075 7473 2829 0a20 2020 2020 2020  inputs().       
-00003a20: 2020 2020 2073 656c 662e 6564 6974 5f73       self.edit_s
-00003a30: 7461 7469 6f6e 5f73 6574 7469 6e67 7328  tation_settings(
-00003a40: 290a 0a20 2020 2064 6566 206f 7065 6e5f  )..    def open_
-00003a50: 6461 7461 6261 7365 2873 656c 6629 3a0a  database(self):.
-00003a60: 2020 2020 2020 2020 2222 224f 7065 6e20          """Open 
-00003a70: 6578 6973 7469 6e67 2064 6174 6162 6173  existing databas
-00003a80: 652e 2222 220a 2020 2020 2020 2020 6669  e.""".        fi
-00003a90: 6c65 6e61 6d65 203d 2073 656c 662e 6669  lename = self.fi
-00003aa0: 6c65 7069 636b 6572 2822 6f70 656e 2229  lepicker("open")
-00003ab0: 0a20 2020 2020 2020 2069 6620 6669 6c65  .        if file
-00003ac0: 6e61 6d65 3a0a 2020 2020 2020 2020 2020  name:.          
-00003ad0: 2020 7365 6c66 2e70 7265 665b 2263 7572    self.pref["cur
-00003ae0: 7265 6e74 5f64 6174 6162 6173 6522 5d20  rent_database"] 
-00003af0: 3d20 6669 6c65 6e61 6d65 2e73 706c 6974  = filename.split
-00003b00: 2822 2f22 295b 2d31 3a5d 5b30 5d0a 2020  ("/")[-1:][0].  
-00003b10: 2020 2020 2020 2020 2020 7365 6c66 2e77            self.w
-00003b20: 7269 7465 5f70 7265 6665 7265 6e63 6528  rite_preference(
-00003b30: 290a 2020 2020 2020 2020 2020 2020 7365  ).            se
-00003b40: 6c66 2e64 626e 616d 6520 3d20 4441 5441  lf.dbname = DATA
-00003b50: 5f50 4154 4820 2b20 222f 2220 2b20 7365  _PATH + "/" + se
-00003b60: 6c66 2e70 7265 662e 6765 7428 2263 7572  lf.pref.get("cur
-00003b70: 7265 6e74 5f64 6174 6162 6173 6522 2c20  rent_database", 
-00003b80: 2268 616d 2e64 6222 290a 2020 2020 2020  "ham.db").      
-00003b90: 2020 2020 2020 7365 6c66 2e64 6174 6162        self.datab
-00003ba0: 6173 6520 3d20 4461 7461 4261 7365 2873  ase = DataBase(s
-00003bb0: 656c 662e 6462 6e61 6d65 2c20 574f 524b  elf.dbname, WORK
-00003bc0: 494e 475f 5041 5448 290a 2020 2020 2020  ING_PATH).      
-00003bd0: 2020 2020 2020 7365 6c66 2e63 6f6e 7461        self.conta
-00003be0: 6374 203d 2073 656c 662e 6461 7461 6261  ct = self.databa
-00003bf0: 7365 2e65 6d70 7479 5f63 6f6e 7461 6374  se.empty_contact
-00003c00: 0a20 2020 2020 2020 2020 2020 2073 656c  .            sel
-00003c10: 662e 7374 6174 696f 6e20 3d20 7365 6c66  f.station = self
-00003c20: 2e64 6174 6162 6173 652e 6665 7463 685f  .database.fetch_
-00003c30: 7374 6174 696f 6e28 290a 2020 2020 2020  station().      
-00003c40: 2020 2020 2020 6966 2073 656c 662e 7374        if self.st
-00003c50: 6174 696f 6e20 6973 204e 6f6e 653a 0a20  ation is None:. 
-00003c60: 2020 2020 2020 2020 2020 2020 2020 2073                 s
-00003c70: 656c 662e 7374 6174 696f 6e20 3d20 7b7d  elf.station = {}
-00003c80: 0a20 2020 2020 2020 2020 2020 2069 6620  .            if 
-00003c90: 7365 6c66 2e73 7461 7469 6f6e 2e67 6574  self.station.get
-00003ca0: 2822 4361 6c6c 222c 2022 2229 203d 3d20  ("Call", "") == 
-00003cb0: 2222 3a0a 2020 2020 2020 2020 2020 2020  "":.            
-00003cc0: 2020 2020 7365 6c66 2e65 6469 745f 7374      self.edit_st
-00003cd0: 6174 696f 6e5f 7365 7474 696e 6773 2829  ation_settings()
-00003ce0: 0a20 2020 2020 2020 2020 2020 2073 656c  .            sel
-00003cf0: 662e 6375 7272 656e 745f 6f70 203d 2073  f.current_op = s
-00003d00: 656c 662e 7374 6174 696f 6e2e 6765 7428  elf.station.get(
-00003d10: 2243 616c 6c22 2c20 2222 290a 2020 2020  "Call", "").    
-00003d20: 2020 2020 2020 2020 7365 6c66 2e6d 616b          self.mak
-00003d30: 655f 6f70 5f64 6972 2829 0a20 2020 2020  e_op_dir().     
-00003d40: 2020 2020 2020 2063 6d64 203d 207b 7d0a         cmd = {}.
-00003d50: 2020 2020 2020 2020 2020 2020 636d 645b              cmd[
-00003d60: 2263 6d64 225d 203d 2022 4e45 5744 4222  "cmd"] = "NEWDB"
-00003d70: 0a20 2020 2020 2020 2020 2020 2063 6d64  .            cmd
-00003d80: 5b22 7374 6174 696f 6e22 5d20 3d20 706c  ["station"] = pl
-00003d90: 6174 666f 726d 2e6e 6f64 6528 290a 2020  atform.node().  
-00003da0: 2020 2020 2020 2020 2020 7365 6c66 2e6d            self.m
-00003db0: 756c 7469 6361 7374 5f69 6e74 6572 6661  ulticast_interfa
-00003dc0: 6365 2e73 656e 645f 6173 5f6a 736f 6e28  ce.send_as_json(
-00003dd0: 636d 6429 0a20 2020 2020 2020 2020 2020  cmd).           
-00003de0: 2073 656c 662e 636c 6561 7269 6e70 7574   self.clearinput
-00003df0: 7328 290a 0a20 2020 2064 6566 206e 6577  s()..    def new
-00003e00: 5f63 6f6e 7465 7374 2873 656c 6629 3a0a  _contest(self):.
-00003e10: 2020 2020 2020 2020 2222 2243 7265 6174          """Creat
-00003e20: 6520 6e65 7720 636f 6e74 6573 7420 696e  e new contest in
-00003e30: 2065 7869 7374 696e 6720 6461 7461 6261   existing databa
-00003e40: 7365 2e22 2222 0a0a 2020 2020 6465 6620  se."""..    def 
-00003e50: 6f70 656e 5f63 6f6e 7465 7374 2873 656c  open_contest(sel
-00003e60: 6629 3a0a 2020 2020 2020 2020 2222 2253  f):.        """S
-00003e70: 7769 7463 6820 746f 2061 2064 6966 6665  witch to a diffe
-00003e80: 7265 6e74 2065 7869 7374 696e 6720 636f  rent existing co
-00003e90: 6e74 6573 7420 696e 2065 7869 7374 696e  ntest in existin
-00003ea0: 6720 6461 7461 6261 7365 2e22 2222 0a20  g database.""". 
-00003eb0: 2020 2020 2020 206c 6f67 6765 722e 6465         logger.de
-00003ec0: 6275 6728 224f 7065 6e20 436f 6e74 6573  bug("Open Contes
-00003ed0: 7420 7365 6c65 6374 6564 2229 0a20 2020  t selected").   
-00003ee0: 2020 2020 2063 6f6e 7465 7374 7320 3d20       contests = 
-00003ef0: 7365 6c66 2e64 6174 6162 6173 652e 6665  self.database.fe
-00003f00: 7463 685f 616c 6c5f 636f 6e74 6573 7473  tch_all_contests
-00003f10: 2829 0a20 2020 2020 2020 206c 6f67 6765  ().        logge
-00003f20: 722e 6465 6275 6728 2225 7322 2c20 6622  r.debug("%s", f"
-00003f30: 7b63 6f6e 7465 7374 737d 2229 0a0a 2020  {contests}")..  
-00003f40: 2020 2020 2020 6966 2063 6f6e 7465 7374        if contest
-00003f50: 733a 0a20 2020 2020 2020 2020 2020 2073  s:.            s
-00003f60: 656c 662e 636f 6e74 6573 745f 6469 616c  elf.contest_dial
-00003f70: 6f67 203d 2053 656c 6563 7443 6f6e 7465  og = SelectConte
-00003f80: 7374 2857 4f52 4b49 4e47 5f50 4154 4829  st(WORKING_PATH)
-00003f90: 0a20 2020 2020 2020 2020 2020 2069 6620  .            if 
-00003fa0: 7365 6c66 2e70 7265 662e 6765 7428 2264  self.pref.get("d
-00003fb0: 6172 6b5f 6d6f 6465 2229 3a0a 2020 2020  ark_mode"):.    
-00003fc0: 2020 2020 2020 2020 2020 2020 7365 6c66              self
-00003fd0: 2e63 6f6e 7465 7374 5f64 6961 6c6f 672e  .contest_dialog.
-00003fe0: 7365 7453 7479 6c65 5368 6565 7428 4441  setStyleSheet(DA
-00003ff0: 524b 5f53 5459 4c45 5348 4545 5429 0a20  RK_STYLESHEET). 
-00004000: 2020 2020 2020 2020 2020 2073 656c 662e             self.
-00004010: 636f 6e74 6573 745f 6469 616c 6f67 2e63  contest_dialog.c
-00004020: 6f6e 7465 7374 5f6c 6973 742e 7365 7452  ontest_list.setR
-00004030: 6f77 436f 756e 7428 3029 0a20 2020 2020  owCount(0).     
-00004040: 2020 2020 2020 2073 656c 662e 636f 6e74         self.cont
-00004050: 6573 745f 6469 616c 6f67 2e63 6f6e 7465  est_dialog.conte
-00004060: 7374 5f6c 6973 742e 7365 7443 6f6c 756d  st_list.setColum
-00004070: 6e43 6f75 6e74 2834 290a 2020 2020 2020  nCount(4).      
-00004080: 2020 2020 2020 7365 6c66 2e63 6f6e 7465        self.conte
-00004090: 7374 5f64 6961 6c6f 672e 636f 6e74 6573  st_dialog.contes
-000040a0: 745f 6c69 7374 2e76 6572 7469 6361 6c48  t_list.verticalH
-000040b0: 6561 6465 7228 292e 7365 7456 6973 6962  eader().setVisib
-000040c0: 6c65 2846 616c 7365 290a 2020 2020 2020  le(False).      
-000040d0: 2020 2020 2020 7365 6c66 2e63 6f6e 7465        self.conte
-000040e0: 7374 5f64 6961 6c6f 672e 636f 6e74 6573  st_dialog.contes
-000040f0: 745f 6c69 7374 2e73 6574 436f 6c75 6d6e  t_list.setColumn
-00004100: 5769 6474 6828 312c 2032 3030 290a 2020  Width(1, 200).  
-00004110: 2020 2020 2020 2020 2020 7365 6c66 2e63            self.c
-00004120: 6f6e 7465 7374 5f64 6961 6c6f 672e 636f  ontest_dialog.co
-00004130: 6e74 6573 745f 6c69 7374 2e73 6574 436f  ntest_list.setCo
-00004140: 6c75 6d6e 5769 6474 6828 322c 2032 3030  lumnWidth(2, 200
-00004150: 290a 2020 2020 2020 2020 2020 2020 7365  ).            se
-00004160: 6c66 2e63 6f6e 7465 7374 5f64 6961 6c6f  lf.contest_dialo
-00004170: 672e 636f 6e74 6573 745f 6c69 7374 2e73  g.contest_list.s
-00004180: 6574 486f 7269 7a6f 6e74 616c 4865 6164  etHorizontalHead
-00004190: 6572 4974 656d 280a 2020 2020 2020 2020  erItem(.        
-000041a0: 2020 2020 2020 2020 302c 2051 7457 6964          0, QtWid
-000041b0: 6765 7473 2e51 5461 626c 6557 6964 6765  gets.QTableWidge
-000041c0: 7449 7465 6d28 2243 6f6e 7465 7374 204e  tItem("Contest N
-000041d0: 7222 290a 2020 2020 2020 2020 2020 2020  r").            
-000041e0: 290a 2020 2020 2020 2020 2020 2020 7365  ).            se
-000041f0: 6c66 2e63 6f6e 7465 7374 5f64 6961 6c6f  lf.contest_dialo
-00004200: 672e 636f 6e74 6573 745f 6c69 7374 2e73  g.contest_list.s
-00004210: 6574 486f 7269 7a6f 6e74 616c 4865 6164  etHorizontalHead
-00004220: 6572 4974 656d 280a 2020 2020 2020 2020  erItem(.        
-00004230: 2020 2020 2020 2020 312c 2051 7457 6964          1, QtWid
-00004240: 6765 7473 2e51 5461 626c 6557 6964 6765  gets.QTableWidge
-00004250: 7449 7465 6d28 2243 6f6e 7465 7374 204e  tItem("Contest N
-00004260: 616d 6522 290a 2020 2020 2020 2020 2020  ame").          
-00004270: 2020 290a 2020 2020 2020 2020 2020 2020    ).            
-00004280: 7365 6c66 2e63 6f6e 7465 7374 5f64 6961  self.contest_dia
-00004290: 6c6f 672e 636f 6e74 6573 745f 6c69 7374  log.contest_list
-000042a0: 2e73 6574 486f 7269 7a6f 6e74 616c 4865  .setHorizontalHe
-000042b0: 6164 6572 4974 656d 280a 2020 2020 2020  aderItem(.      
-000042c0: 2020 2020 2020 2020 2020 322c 2051 7457            2, QtW
-000042d0: 6964 6765 7473 2e51 5461 626c 6557 6964  idgets.QTableWid
-000042e0: 6765 7449 7465 6d28 2243 6f6e 7465 7374  getItem("Contest
-000042f0: 2053 7461 7274 2229 0a20 2020 2020 2020   Start").       
-00004300: 2020 2020 2029 0a20 2020 2020 2020 2020       ).         
-00004310: 2020 2073 656c 662e 636f 6e74 6573 745f     self.contest_
-00004320: 6469 616c 6f67 2e63 6f6e 7465 7374 5f6c  dialog.contest_l
-00004330: 6973 742e 7365 7448 6f72 697a 6f6e 7461  ist.setHorizonta
-00004340: 6c48 6561 6465 7249 7465 6d28 0a20 2020  lHeaderItem(.   
-00004350: 2020 2020 2020 2020 2020 2020 2033 2c20               3, 
-00004360: 5174 5769 6467 6574 732e 5154 6162 6c65  QtWidgets.QTable
-00004370: 5769 6467 6574 4974 656d 2822 4e6f 7420  WidgetItem("Not 
-00004380: 5549 7365 6422 290a 2020 2020 2020 2020  UIsed").        
-00004390: 2020 2020 290a 2020 2020 2020 2020 2020      ).          
-000043a0: 2020 7365 6c66 2e63 6f6e 7465 7374 5f64    self.contest_d
-000043b0: 6961 6c6f 672e 636f 6e74 6573 745f 6c69  ialog.contest_li
-000043c0: 7374 2e73 6574 436f 6c75 6d6e 4869 6464  st.setColumnHidd
-000043d0: 656e 2830 2c20 5472 7565 290a 2020 2020  en(0, True).    
-000043e0: 2020 2020 2020 2020 7365 6c66 2e63 6f6e          self.con
-000043f0: 7465 7374 5f64 6961 6c6f 672e 636f 6e74  test_dialog.cont
-00004400: 6573 745f 6c69 7374 2e73 6574 436f 6c75  est_list.setColu
-00004410: 6d6e 4869 6464 656e 2833 2c20 5472 7565  mnHidden(3, True
-00004420: 290a 2020 2020 2020 2020 2020 2020 7365  ).            se
-00004430: 6c66 2e63 6f6e 7465 7374 5f64 6961 6c6f  lf.contest_dialo
-00004440: 672e 6163 6365 7074 6564 2e63 6f6e 6e65  g.accepted.conne
-00004450: 6374 2873 656c 662e 6f70 656e 5f63 6f6e  ct(self.open_con
-00004460: 7465 7374 5f72 6574 7572 6e29 0a20 2020  test_return).   
-00004470: 2020 2020 2020 2020 2066 6f72 2063 6f6e           for con
-00004480: 7465 7374 2069 6e20 636f 6e74 6573 7473  test in contests
-00004490: 3a0a 2020 2020 2020 2020 2020 2020 2020  :.              
-000044a0: 2020 6e75 6d62 6572 5f6f 665f 726f 7773    number_of_rows
-000044b0: 203d 2073 656c 662e 636f 6e74 6573 745f   = self.contest_
-000044c0: 6469 616c 6f67 2e63 6f6e 7465 7374 5f6c  dialog.contest_l
-000044d0: 6973 742e 726f 7743 6f75 6e74 2829 0a20  ist.rowCount(). 
-000044e0: 2020 2020 2020 2020 2020 2020 2020 2073                 s
-000044f0: 656c 662e 636f 6e74 6573 745f 6469 616c  elf.contest_dial
-00004500: 6f67 2e63 6f6e 7465 7374 5f6c 6973 742e  og.contest_list.
-00004510: 696e 7365 7274 526f 7728 6e75 6d62 6572  insertRow(number
-00004520: 5f6f 665f 726f 7773 290a 2020 2020 2020  _of_rows).      
-00004530: 2020 2020 2020 2020 2020 636f 6e74 6573            contes
-00004540: 745f 6964 203d 2073 7472 2863 6f6e 7465  t_id = str(conte
-00004550: 7374 2e67 6574 2822 436f 6e74 6573 7449  st.get("ContestI
-00004560: 4422 2c20 3129 290a 2020 2020 2020 2020  D", 1)).        
-00004570: 2020 2020 2020 2020 636f 6e74 6573 745f          contest_
-00004580: 6e61 6d65 203d 2063 6f6e 7465 7374 2e67  name = contest.g
-00004590: 6574 2822 436f 6e74 6573 744e 616d 6522  et("ContestName"
-000045a0: 2c20 3129 0a20 2020 2020 2020 2020 2020  , 1).           
-000045b0: 2020 2020 2073 7461 7274 5f64 6174 6520       start_date 
-000045c0: 3d20 636f 6e74 6573 742e 6765 7428 2253  = contest.get("S
-000045d0: 7461 7274 4461 7465 222c 2031 290a 2020  tartDate", 1).  
-000045e0: 2020 2020 2020 2020 2020 2020 2020 7365                se
-000045f0: 6c66 2e63 6f6e 7465 7374 5f64 6961 6c6f  lf.contest_dialo
-00004600: 672e 636f 6e74 6573 745f 6c69 7374 2e73  g.contest_list.s
-00004610: 6574 4974 656d 280a 2020 2020 2020 2020  etItem(.        
-00004620: 2020 2020 2020 2020 2020 2020 6e75 6d62              numb
-00004630: 6572 5f6f 665f 726f 7773 2c20 302c 2051  er_of_rows, 0, Q
-00004640: 7457 6964 6765 7473 2e51 5461 626c 6557  tWidgets.QTableW
-00004650: 6964 6765 7449 7465 6d28 636f 6e74 6573  idgetItem(contes
-00004660: 745f 6964 290a 2020 2020 2020 2020 2020  t_id).          
-00004670: 2020 2020 2020 290a 2020 2020 2020 2020        ).        
-00004680: 2020 2020 2020 2020 7365 6c66 2e63 6f6e          self.con
-00004690: 7465 7374 5f64 6961 6c6f 672e 636f 6e74  test_dialog.cont
-000046a0: 6573 745f 6c69 7374 2e73 6574 4974 656d  est_list.setItem
-000046b0: 280a 2020 2020 2020 2020 2020 2020 2020  (.              
-000046c0: 2020 2020 2020 6e75 6d62 6572 5f6f 665f        number_of_
-000046d0: 726f 7773 2c20 312c 2051 7457 6964 6765  rows, 1, QtWidge
-000046e0: 7473 2e51 5461 626c 6557 6964 6765 7449  ts.QTableWidgetI
-000046f0: 7465 6d28 636f 6e74 6573 745f 6e61 6d65  tem(contest_name
-00004700: 290a 2020 2020 2020 2020 2020 2020 2020  ).              
-00004710: 2020 290a 2020 2020 2020 2020 2020 2020    ).            
-00004720: 2020 2020 7365 6c66 2e63 6f6e 7465 7374      self.contest
-00004730: 5f64 6961 6c6f 672e 636f 6e74 6573 745f  _dialog.contest_
-00004740: 6c69 7374 2e73 6574 4974 656d 280a 2020  list.setItem(.  
+00001160: 7573 6572 6967 6374 6c64 223a 2046 616c  userigctld": Fal
+00001170: 7365 2c0a 2020 2020 2020 2020 2275 7365  se,.        "use
+00001180: 666c 7269 6722 3a20 4661 6c73 652c 0a20  flrig": False,. 
+00001190: 2020 2020 2020 2022 6377 6970 223a 2022         "cwip": "
+000011a0: 3132 372e 302e 302e 3122 2c0a 2020 2020  127.0.0.1",.    
+000011b0: 2020 2020 2263 7770 6f72 7422 3a20 3637      "cwport": 67
+000011c0: 3839 2c0a 2020 2020 2020 2020 2263 7774  89,.        "cwt
+000011d0: 7970 6522 3a20 302c 0a20 2020 2020 2020  ype": 0,.       
+000011e0: 2022 7573 6573 6572 7665 7222 3a20 4661   "useserver": Fa
+000011f0: 6c73 652c 0a20 2020 2020 2020 2022 4341  lse,.        "CA
+00001200: 545f 706f 7274 223a 2034 3533 322c 0a20  T_port": 4532,. 
+00001210: 2020 2020 2020 2022 636c 7573 7465 725f         "cluster_
+00001220: 7365 7276 6572 223a 2022 6478 632e 6e63  server": "dxc.nc
+00001230: 376a 2e63 6f6d 222c 0a20 2020 2020 2020  7j.com",.       
+00001240: 2022 636c 7573 7465 725f 706f 7274 223a   "cluster_port":
+00001250: 2037 3337 332c 0a20 2020 2020 2020 2022   7373,.        "
+00001260: 636c 7573 7465 725f 6669 6c74 6572 223a  cluster_filter":
+00001270: 2022 5365 7420 4458 2046 696c 7465 7220   "Set DX Filter 
+00001280: 5370 6f74 7465 7243 6f6e 743d 4e41 222c  SpotterCont=NA",
+00001290: 0a20 2020 2020 2020 2022 636c 7573 7465  .        "cluste
+000012a0: 725f 6d6f 6465 223a 2022 4f50 454e 222c  r_mode": "OPEN",
+000012b0: 0a20 2020 207d 0a20 2020 2061 7070 7374  .    }.    appst
+000012c0: 6172 7465 6420 3d20 4661 6c73 650a 2020  arted = False.  
+000012d0: 2020 636f 6e74 6163 7420 3d20 7b7d 0a20    contact = {}. 
+000012e0: 2020 2063 6f6e 7465 7374 203d 204e 6f6e     contest = Non
+000012f0: 650a 2020 2020 636f 6e74 6573 745f 7365  e.    contest_se
+00001300: 7474 696e 6773 203d 207b 7d0a 2020 2020  ttings = {}.    
+00001310: 7072 6566 203d 204e 6f6e 650a 2020 2020  pref = None.    
+00001320: 7374 6174 696f 6e20 3d20 7b7d 0a20 2020  station = {}.   
+00001330: 2063 7572 7265 6e74 5f6f 7020 3d20 2222   current_op = ""
+00001340: 0a20 2020 2063 7572 7265 6e74 5f6d 6f64  .    current_mod
+00001350: 6520 3d20 2222 0a20 2020 2063 7572 7265  e = "".    curre
+00001360: 6e74 5f62 616e 6420 3d20 2222 0a20 2020  nt_band = "".   
+00001370: 2063 7720 3d20 4e6f 6e65 0a20 2020 206c   cw = None.    l
+00001380: 6f6f 6b5f 7570 203d 204e 6f6e 650a 2020  ook_up = None.  
+00001390: 2020 7275 6e5f 7374 6174 6520 3d20 4661    run_state = Fa
+000013a0: 6c73 650a 2020 2020 666b 6579 7320 3d20  lse.    fkeys = 
+000013b0: 7b7d 0a20 2020 2061 626f 7574 5f64 6961  {}.    about_dia
+000013c0: 6c6f 6720 3d20 4e6f 6e65 0a20 2020 2071  log = None.    q
+000013d0: 727a 5f64 6961 6c6f 6720 3d20 4e6f 6e65  rz_dialog = None
+000013e0: 0a20 2020 2073 6574 7469 6e67 735f 6469  .    settings_di
+000013f0: 616c 6f67 203d 204e 6f6e 650a 2020 2020  alog = None.    
+00001400: 6564 6974 5f6d 6163 726f 5f64 6961 6c6f  edit_macro_dialo
+00001410: 6720 3d20 4e6f 6e65 0a20 2020 2063 6f6e  g = None.    con
+00001420: 7465 7374 5f64 6961 6c6f 6720 3d20 4e6f  test_dialog = No
+00001430: 6e65 0a20 2020 2063 6f6e 6669 6775 7261  ne.    configura
+00001440: 7469 6f6e 5f64 6961 6c6f 6720 3d20 4e6f  tion_dialog = No
+00001450: 6e65 0a20 2020 206f 706f 6e5f 6469 616c  ne.    opon_dial
+00001460: 6f67 203d 204e 6f6e 650a 2020 2020 6462  og = None.    db
+00001470: 6e61 6d65 203d 2044 4154 415f 5041 5448  name = DATA_PATH
+00001480: 202b 2022 2f68 616d 2e64 6222 0a20 2020   + "/ham.db".   
+00001490: 2072 6164 696f 5f73 7461 7465 203d 207b   radio_state = {
+000014a0: 7d0a 2020 2020 7269 675f 636f 6e74 726f  }.    rig_contro
+000014b0: 6c20 3d20 4e6f 6e65 0a20 2020 2073 6572  l = None.    ser
+000014c0: 7665 725f 7564 7020 3d20 4e6f 6e65 0a20  ver_udp = None. 
+000014d0: 2020 206d 756c 7469 6361 7374 5f67 726f     multicast_gro
+000014e0: 7570 203d 204e 6f6e 650a 2020 2020 6d75  up = None.    mu
+000014f0: 6c74 6963 6173 745f 706f 7274 203d 204e  lticast_port = N
+00001500: 6f6e 650a 2020 2020 696e 7465 7266 6163  one.    interfac
+00001510: 655f 6970 203d 204e 6f6e 650a 2020 2020  e_ip = None.    
+00001520: 7269 675f 636f 6e74 726f 6c20 3d20 4e6f  rig_control = No
+00001530: 6e65 0a0a 2020 2020 6465 6620 5f5f 696e  ne..    def __in
+00001540: 6974 5f5f 2873 656c 662c 202a 6172 6773  it__(self, *args
+00001550: 2c20 2a2a 6b77 6172 6773 293a 0a20 2020  , **kwargs):.   
+00001560: 2020 2020 2073 7570 6572 2829 2e5f 5f69       super().__i
+00001570: 6e69 745f 5f28 2a61 7267 732c 202a 2a6b  nit__(*args, **k
+00001580: 7761 7267 7329 0a20 2020 2020 2020 206c  wargs).        l
+00001590: 6f67 6765 722e 696e 666f 2822 4d61 696e  ogger.info("Main
+000015a0: 5769 6e64 6f77 3a20 5f5f 696e 6974 5f5f  Window: __init__
+000015b0: 2229 0a20 2020 2020 2020 2073 656c 662e  ").        self.
+000015c0: 5f75 6470 7761 7463 6820 3d20 4e6f 6e65  _udpwatch = None
+000015d0: 0a20 2020 2020 2020 2073 656c 662e 7564  .        self.ud
+000015e0: 705f 6669 666f 203d 2071 7565 7565 2e51  p_fifo = queue.Q
+000015f0: 7565 7565 2829 0a20 2020 2020 2020 2064  ueue().        d
+00001600: 6174 615f 7061 7468 203d 2057 4f52 4b49  ata_path = WORKI
+00001610: 4e47 5f50 4154 4820 2b20 222f 6461 7461  NG_PATH + "/data
+00001620: 2f6d 6169 6e2e 7569 220a 2020 2020 2020  /main.ui".      
+00001630: 2020 7569 632e 6c6f 6164 5569 2864 6174    uic.loadUi(dat
+00001640: 615f 7061 7468 2c20 7365 6c66 290a 2020  a_path, self).  
+00001650: 2020 2020 2020 7365 6c66 2e6c 6566 7464        self.leftd
+00001660: 6f74 2e68 6964 6528 290a 2020 2020 2020  ot.hide().      
+00001670: 2020 7365 6c66 2e72 6967 6874 646f 742e    self.rightdot.
+00001680: 6869 6465 2829 0a20 2020 2020 2020 2073  hide().        s
+00001690: 656c 662e 6e31 6d6d 203d 204e 314d 4d28  elf.n1mm = N1MM(
+000016a0: 290a 2020 2020 2020 2020 7365 6c66 2e6e  ).        self.n
+000016b0: 6578 745f 6669 656c 6420 3d20 7365 6c66  ext_field = self
+000016c0: 2e6f 7468 6572 5f32 0a20 2020 2020 2020  .other_2.       
+000016d0: 2073 656c 662e 6475 7065 5f69 6e64 6963   self.dupe_indic
+000016e0: 6174 6f72 2e68 6964 6528 290a 2020 2020  ator.hide().    
+000016f0: 2020 2020 7365 6c66 2e63 775f 7370 6565      self.cw_spee
+00001700: 642e 7661 6c75 6543 6861 6e67 6564 2e63  d.valueChanged.c
+00001710: 6f6e 6e65 6374 2873 656c 662e 6377 7370  onnect(self.cwsp
+00001720: 6565 645f 7370 696e 626f 785f 6368 616e  eed_spinbox_chan
+00001730: 6765 6429 0a0a 2020 2020 2020 2020 7365  ged)..        se
+00001740: 6c66 2e61 6374 696f 6e43 575f 4d61 6372  lf.actionCW_Macr
+00001750: 6f73 2e74 7269 6767 6572 6564 2e63 6f6e  os.triggered.con
+00001760: 6e65 6374 2873 656c 662e 6377 5f6d 6163  nect(self.cw_mac
+00001770: 726f 735f 7374 6174 655f 6368 616e 6765  ros_state_change
+00001780: 6429 0a20 2020 2020 2020 2073 656c 662e  d).        self.
+00001790: 6163 7469 6f6e 436f 6d6d 616e 645f 4275  actionCommand_Bu
+000017a0: 7474 6f6e 732e 7472 6967 6765 7265 642e  ttons.triggered.
+000017b0: 636f 6e6e 6563 7428 7365 6c66 2e63 6f6d  connect(self.com
+000017c0: 6d61 6e64 5f62 7574 746f 6e73 5f73 7461  mand_buttons_sta
+000017d0: 7465 5f63 6861 6e67 6529 0a20 2020 2020  te_change).     
+000017e0: 2020 2073 656c 662e 6163 7469 6f6e 4461     self.actionDa
+000017f0: 726b 5f4d 6f64 652e 7472 6967 6765 7265  rk_Mode.triggere
+00001800: 642e 636f 6e6e 6563 7428 7365 6c66 2e64  d.connect(self.d
+00001810: 6172 6b5f 6d6f 6465 5f73 7461 7465 5f63  ark_mode_state_c
+00001820: 6861 6e67 6529 0a20 2020 2020 2020 2073  hange).        s
+00001830: 656c 662e 6163 7469 6f6e 4c6f 675f 5769  elf.actionLog_Wi
+00001840: 6e64 6f77 2e74 7269 6767 6572 6564 2e63  ndow.triggered.c
+00001850: 6f6e 6e65 6374 2873 656c 662e 6c61 756e  onnect(self.laun
+00001860: 6368 5f6c 6f67 5f77 696e 646f 7729 0a20  ch_log_window). 
+00001870: 2020 2020 2020 2073 656c 662e 6163 7469         self.acti
+00001880: 6f6e 4261 6e64 6d61 702e 7472 6967 6765  onBandmap.trigge
+00001890: 7265 642e 636f 6e6e 6563 7428 7365 6c66  red.connect(self
+000018a0: 2e6c 6175 6e63 685f 6261 6e64 6d61 705f  .launch_bandmap_
+000018b0: 7769 6e64 6f77 290a 2020 2020 2020 2020  window).        
+000018c0: 7365 6c66 2e61 6374 696f 6e52 6563 616c  self.actionRecal
+000018d0: 6375 6c61 7465 5f4d 756c 7473 2e74 7269  culate_Mults.tri
+000018e0: 6767 6572 6564 2e63 6f6e 6e65 6374 2873  ggered.connect(s
+000018f0: 656c 662e 7265 6361 6c63 756c 6174 655f  elf.recalculate_
+00001900: 6d75 6c74 7329 0a0a 2020 2020 2020 2020  mults)..        
+00001910: 7365 6c66 2e61 6374 696f 6e47 656e 6572  self.actionGener
+00001920: 6174 655f 4361 6272 696c 6c6f 2e74 7269  ate_Cabrillo.tri
+00001930: 6767 6572 6564 2e63 6f6e 6e65 6374 2873  ggered.connect(s
+00001940: 656c 662e 6765 6e65 7261 7465 5f63 6162  elf.generate_cab
+00001950: 7269 6c6c 6f29 0a20 2020 2020 2020 2073  rillo).        s
+00001960: 656c 662e 6163 7469 6f6e 4765 6e65 7261  elf.actionGenera
+00001970: 7465 5f41 4449 462e 7472 6967 6765 7265  te_ADIF.triggere
+00001980: 642e 636f 6e6e 6563 7428 7365 6c66 2e67  d.connect(self.g
+00001990: 656e 6572 6174 655f 6164 6966 290a 0a20  enerate_adif).. 
+000019a0: 2020 2020 2020 2073 656c 662e 6163 7469         self.acti
+000019b0: 6f6e 436f 6e66 6967 7572 6174 696f 6e5f  onConfiguration_
+000019c0: 5365 7474 696e 6773 2e74 7269 6767 6572  Settings.trigger
+000019d0: 6564 2e63 6f6e 6e65 6374 280a 2020 2020  ed.connect(.    
+000019e0: 2020 2020 2020 2020 7365 6c66 2e65 6469          self.edi
+000019f0: 745f 636f 6e66 6967 7572 6174 696f 6e5f  t_configuration_
+00001a00: 7365 7474 696e 6773 0a20 2020 2020 2020  settings.       
+00001a10: 2029 0a20 2020 2020 2020 2073 656c 662e   ).        self.
+00001a20: 6163 7469 6f6e 5374 6174 696f 6e53 6574  actionStationSet
+00001a30: 7469 6e67 732e 7472 6967 6765 7265 642e  tings.triggered.
+00001a40: 636f 6e6e 6563 7428 7365 6c66 2e65 6469  connect(self.edi
+00001a50: 745f 7374 6174 696f 6e5f 7365 7474 696e  t_station_settin
+00001a60: 6773 290a 0a20 2020 2020 2020 2073 656c  gs)..        sel
+00001a70: 662e 6163 7469 6f6e 4e65 775f 436f 6e74  f.actionNew_Cont
+00001a80: 6573 742e 7472 6967 6765 7265 642e 636f  est.triggered.co
+00001a90: 6e6e 6563 7428 7365 6c66 2e6e 6577 5f63  nnect(self.new_c
+00001aa0: 6f6e 7465 7374 5f64 6961 6c6f 6729 0a20  ontest_dialog). 
+00001ab0: 2020 2020 2020 2073 656c 662e 6163 7469         self.acti
+00001ac0: 6f6e 4f70 656e 5f43 6f6e 7465 7374 2e74  onOpen_Contest.t
+00001ad0: 7269 6767 6572 6564 2e63 6f6e 6e65 6374  riggered.connect
+00001ae0: 2873 656c 662e 6f70 656e 5f63 6f6e 7465  (self.open_conte
+00001af0: 7374 290a 2020 2020 2020 2020 7365 6c66  st).        self
+00001b00: 2e61 6374 696f 6e45 6469 745f 4375 7272  .actionEdit_Curr
+00001b10: 656e 745f 436f 6e74 6573 742e 7472 6967  ent_Contest.trig
+00001b20: 6765 7265 642e 636f 6e6e 6563 7428 7365  gered.connect(se
+00001b30: 6c66 2e65 6469 745f 636f 6e74 6573 7429  lf.edit_contest)
+00001b40: 0a0a 2020 2020 2020 2020 7365 6c66 2e61  ..        self.a
+00001b50: 6374 696f 6e4e 6577 5f44 6174 6162 6173  ctionNew_Databas
+00001b60: 652e 7472 6967 6765 7265 642e 636f 6e6e  e.triggered.conn
+00001b70: 6563 7428 7365 6c66 2e6e 6577 5f64 6174  ect(self.new_dat
+00001b80: 6162 6173 6529 0a20 2020 2020 2020 2073  abase).        s
+00001b90: 656c 662e 6163 7469 6f6e 4f70 656e 5f44  elf.actionOpen_D
+00001ba0: 6174 6162 6173 652e 7472 6967 6765 7265  atabase.triggere
+00001bb0: 642e 636f 6e6e 6563 7428 7365 6c66 2e6f  d.connect(self.o
+00001bc0: 7065 6e5f 6461 7461 6261 7365 290a 0a20  pen_database).. 
+00001bd0: 2020 2020 2020 2073 656c 662e 6163 7469         self.acti
+00001be0: 6f6e 4564 6974 5f4d 6163 726f 732e 7472  onEdit_Macros.tr
+00001bf0: 6967 6765 7265 642e 636f 6e6e 6563 7428  iggered.connect(
+00001c00: 7365 6c66 2e65 6469 745f 6377 5f6d 6163  self.edit_cw_mac
+00001c10: 726f 7329 0a0a 2020 2020 2020 2020 7365  ros)..        se
+00001c20: 6c66 2e61 6374 696f 6e41 626f 7574 2e74  lf.actionAbout.t
+00001c30: 7269 6767 6572 6564 2e63 6f6e 6e65 6374  riggered.connect
+00001c40: 2873 656c 662e 7368 6f77 5f61 626f 7574  (self.show_about
+00001c50: 5f64 6961 6c6f 6729 0a0a 2020 2020 2020  _dialog)..      
+00001c60: 2020 7365 6c66 2e72 6164 696f 4275 7474    self.radioButt
+00001c70: 6f6e 5f72 756e 2e63 6c69 636b 6564 2e63  on_run.clicked.c
+00001c80: 6f6e 6e65 6374 2873 656c 662e 7275 6e5f  onnect(self.run_
+00001c90: 7370 5f62 7574 746f 6e73 5f63 6c69 636b  sp_buttons_click
+00001ca0: 6564 290a 2020 2020 2020 2020 7365 6c66  ed).        self
+00001cb0: 2e72 6164 696f 4275 7474 6f6e 5f73 702e  .radioButton_sp.
+00001cc0: 636c 6963 6b65 642e 636f 6e6e 6563 7428  clicked.connect(
+00001cd0: 7365 6c66 2e72 756e 5f73 705f 6275 7474  self.run_sp_butt
+00001ce0: 6f6e 735f 636c 6963 6b65 6429 0a20 2020  ons_clicked).   
+00001cf0: 2020 2020 2073 656c 662e 7363 6f72 652e       self.score.
+00001d00: 7365 7454 6578 7428 2230 2229 0a20 2020  setText("0").   
+00001d10: 2020 2020 2073 656c 662e 6361 6c6c 7369       self.callsi
+00001d20: 676e 2e74 6578 7445 6469 7465 642e 636f  gn.textEdited.co
+00001d30: 6e6e 6563 7428 7365 6c66 2e63 616c 6c73  nnect(self.calls
+00001d40: 6967 6e5f 6368 616e 6765 6429 0a20 2020  ign_changed).   
+00001d50: 2020 2020 2073 656c 662e 6361 6c6c 7369       self.callsi
+00001d60: 676e 2e72 6574 7572 6e50 7265 7373 6564  gn.returnPressed
+00001d70: 2e63 6f6e 6e65 6374 2873 656c 662e 7361  .connect(self.sa
+00001d80: 7665 5f63 6f6e 7461 6374 290a 2020 2020  ve_contact).    
+00001d90: 2020 2020 7365 6c66 2e73 656e 742e 7265      self.sent.re
+00001da0: 7475 726e 5072 6573 7365 642e 636f 6e6e  turnPressed.conn
+00001db0: 6563 7428 7365 6c66 2e73 6176 655f 636f  ect(self.save_co
+00001dc0: 6e74 6163 7429 0a20 2020 2020 2020 2073  ntact).        s
+00001dd0: 656c 662e 7265 6365 6976 652e 7265 7475  elf.receive.retu
+00001de0: 726e 5072 6573 7365 642e 636f 6e6e 6563  rnPressed.connec
+00001df0: 7428 7365 6c66 2e73 6176 655f 636f 6e74  t(self.save_cont
+00001e00: 6163 7429 0a20 2020 2020 2020 2073 656c  act).        sel
+00001e10: 662e 6f74 6865 725f 312e 7265 7475 726e  f.other_1.return
+00001e20: 5072 6573 7365 642e 636f 6e6e 6563 7428  Pressed.connect(
+00001e30: 7365 6c66 2e73 6176 655f 636f 6e74 6163  self.save_contac
+00001e40: 7429 0a20 2020 2020 2020 2073 656c 662e  t).        self.
+00001e50: 6f74 6865 725f 322e 7265 7475 726e 5072  other_2.returnPr
+00001e60: 6573 7365 642e 636f 6e6e 6563 7428 7365  essed.connect(se
+00001e70: 6c66 2e73 6176 655f 636f 6e74 6163 7429  lf.save_contact)
+00001e80: 0a20 2020 2020 2020 2073 656c 662e 6f74  .        self.ot
+00001e90: 6865 725f 322e 7465 7874 4564 6974 6564  her_2.textEdited
+00001ea0: 2e63 6f6e 6e65 6374 2873 656c 662e 6f74  .connect(self.ot
+00001eb0: 6865 725f 325f 6368 616e 6765 6429 0a20  her_2_changed). 
+00001ec0: 2020 2020 2020 2073 656c 662e 7365 6e74         self.sent
+00001ed0: 2e73 6574 5465 7874 2822 3539 2229 0a20  .setText("59"). 
+00001ee0: 2020 2020 2020 2073 656c 662e 7265 6365         self.rece
+00001ef0: 6976 652e 7365 7454 6578 7428 2235 3922  ive.setText("59"
+00001f00: 290a 2020 2020 2020 2020 6963 6f6e 5f70  ).        icon_p
+00001f10: 6174 6820 3d20 574f 524b 494e 475f 5041  ath = WORKING_PA
+00001f20: 5448 202b 2022 2f64 6174 612f 220a 2020  TH + "/data/".  
+00001f30: 2020 2020 2020 7365 6c66 2e67 7265 656e        self.green
+00001f40: 646f 7420 3d20 5174 4775 692e 5150 6978  dot = QtGui.QPix
+00001f50: 6d61 7028 6963 6f6e 5f70 6174 6820 2b20  map(icon_path + 
+00001f60: 2267 7265 656e 646f 742e 706e 6722 290a  "greendot.png").
+00001f70: 2020 2020 2020 2020 7365 6c66 2e72 6564          self.red
+00001f80: 646f 7420 3d20 5174 4775 692e 5150 6978  dot = QtGui.QPix
+00001f90: 6d61 7028 6963 6f6e 5f70 6174 6820 2b20  map(icon_path + 
+00001fa0: 2272 6564 646f 742e 706e 6722 290a 2020  "reddot.png").  
+00001fb0: 2020 2020 2020 7365 6c66 2e6c 6566 7464        self.leftd
+00001fc0: 6f74 2e73 6574 5069 786d 6170 2873 656c  ot.setPixmap(sel
+00001fd0: 662e 6772 6565 6e64 6f74 290a 2020 2020  f.greendot).    
+00001fe0: 2020 2020 7365 6c66 2e72 6967 6874 646f      self.rightdo
+00001ff0: 742e 7365 7450 6978 6d61 7028 7365 6c66  t.setPixmap(self
+00002000: 2e72 6564 646f 7429 0a0a 2020 2020 2020  .reddot)..      
+00002010: 2020 7365 6c66 2e46 312e 7365 7443 6f6e    self.F1.setCon
+00002020: 7465 7874 4d65 6e75 506f 6c69 6379 2851  textMenuPolicy(Q
+00002030: 7443 6f72 652e 5174 2e43 7573 746f 6d43  tCore.Qt.CustomC
+00002040: 6f6e 7465 7874 4d65 6e75 290a 2020 2020  ontextMenu).    
+00002050: 2020 2020 7365 6c66 2e46 312e 6375 7374      self.F1.cust
+00002060: 6f6d 436f 6e74 6578 744d 656e 7552 6571  omContextMenuReq
+00002070: 7565 7374 6564 2e63 6f6e 6e65 6374 2873  uested.connect(s
+00002080: 656c 662e 6564 6974 5f46 3129 0a20 2020  elf.edit_F1).   
+00002090: 2020 2020 2073 656c 662e 4631 2e63 6c69       self.F1.cli
+000020a0: 636b 6564 2e63 6f6e 6e65 6374 2873 656c  cked.connect(sel
+000020b0: 662e 7365 6e64 6631 290a 2020 2020 2020  f.sendf1).      
+000020c0: 2020 7365 6c66 2e46 322e 7365 7443 6f6e    self.F2.setCon
+000020d0: 7465 7874 4d65 6e75 506f 6c69 6379 2851  textMenuPolicy(Q
+000020e0: 7443 6f72 652e 5174 2e43 7573 746f 6d43  tCore.Qt.CustomC
+000020f0: 6f6e 7465 7874 4d65 6e75 290a 2020 2020  ontextMenu).    
+00002100: 2020 2020 7365 6c66 2e46 322e 6375 7374      self.F2.cust
+00002110: 6f6d 436f 6e74 6578 744d 656e 7552 6571  omContextMenuReq
+00002120: 7565 7374 6564 2e63 6f6e 6e65 6374 2873  uested.connect(s
+00002130: 656c 662e 6564 6974 5f46 3229 0a20 2020  elf.edit_F2).   
+00002140: 2020 2020 2073 656c 662e 4632 2e63 6c69       self.F2.cli
+00002150: 636b 6564 2e63 6f6e 6e65 6374 2873 656c  cked.connect(sel
+00002160: 662e 7365 6e64 6632 290a 2020 2020 2020  f.sendf2).      
+00002170: 2020 7365 6c66 2e46 332e 7365 7443 6f6e    self.F3.setCon
+00002180: 7465 7874 4d65 6e75 506f 6c69 6379 2851  textMenuPolicy(Q
+00002190: 7443 6f72 652e 5174 2e43 7573 746f 6d43  tCore.Qt.CustomC
+000021a0: 6f6e 7465 7874 4d65 6e75 290a 2020 2020  ontextMenu).    
+000021b0: 2020 2020 7365 6c66 2e46 332e 6375 7374      self.F3.cust
+000021c0: 6f6d 436f 6e74 6578 744d 656e 7552 6571  omContextMenuReq
+000021d0: 7565 7374 6564 2e63 6f6e 6e65 6374 2873  uested.connect(s
+000021e0: 656c 662e 6564 6974 5f46 3329 0a20 2020  elf.edit_F3).   
+000021f0: 2020 2020 2073 656c 662e 4633 2e63 6c69       self.F3.cli
+00002200: 636b 6564 2e63 6f6e 6e65 6374 2873 656c  cked.connect(sel
+00002210: 662e 7365 6e64 6633 290a 2020 2020 2020  f.sendf3).      
+00002220: 2020 7365 6c66 2e46 342e 7365 7443 6f6e    self.F4.setCon
+00002230: 7465 7874 4d65 6e75 506f 6c69 6379 2851  textMenuPolicy(Q
+00002240: 7443 6f72 652e 5174 2e43 7573 746f 6d43  tCore.Qt.CustomC
+00002250: 6f6e 7465 7874 4d65 6e75 290a 2020 2020  ontextMenu).    
+00002260: 2020 2020 7365 6c66 2e46 342e 6375 7374      self.F4.cust
+00002270: 6f6d 436f 6e74 6578 744d 656e 7552 6571  omContextMenuReq
+00002280: 7565 7374 6564 2e63 6f6e 6e65 6374 2873  uested.connect(s
+00002290: 656c 662e 6564 6974 5f46 3429 0a20 2020  elf.edit_F4).   
+000022a0: 2020 2020 2073 656c 662e 4634 2e63 6c69       self.F4.cli
+000022b0: 636b 6564 2e63 6f6e 6e65 6374 2873 656c  cked.connect(sel
+000022c0: 662e 7365 6e64 6634 290a 2020 2020 2020  f.sendf4).      
+000022d0: 2020 7365 6c66 2e46 352e 7365 7443 6f6e    self.F5.setCon
+000022e0: 7465 7874 4d65 6e75 506f 6c69 6379 2851  textMenuPolicy(Q
+000022f0: 7443 6f72 652e 5174 2e43 7573 746f 6d43  tCore.Qt.CustomC
+00002300: 6f6e 7465 7874 4d65 6e75 290a 2020 2020  ontextMenu).    
+00002310: 2020 2020 7365 6c66 2e46 352e 6375 7374      self.F5.cust
+00002320: 6f6d 436f 6e74 6578 744d 656e 7552 6571  omContextMenuReq
+00002330: 7565 7374 6564 2e63 6f6e 6e65 6374 2873  uested.connect(s
+00002340: 656c 662e 6564 6974 5f46 3529 0a20 2020  elf.edit_F5).   
+00002350: 2020 2020 2073 656c 662e 4635 2e63 6c69       self.F5.cli
+00002360: 636b 6564 2e63 6f6e 6e65 6374 2873 656c  cked.connect(sel
+00002370: 662e 7365 6e64 6635 290a 2020 2020 2020  f.sendf5).      
+00002380: 2020 7365 6c66 2e46 362e 7365 7443 6f6e    self.F6.setCon
+00002390: 7465 7874 4d65 6e75 506f 6c69 6379 2851  textMenuPolicy(Q
+000023a0: 7443 6f72 652e 5174 2e43 7573 746f 6d43  tCore.Qt.CustomC
+000023b0: 6f6e 7465 7874 4d65 6e75 290a 2020 2020  ontextMenu).    
+000023c0: 2020 2020 7365 6c66 2e46 362e 6375 7374      self.F6.cust
+000023d0: 6f6d 436f 6e74 6578 744d 656e 7552 6571  omContextMenuReq
+000023e0: 7565 7374 6564 2e63 6f6e 6e65 6374 2873  uested.connect(s
+000023f0: 656c 662e 6564 6974 5f46 3629 0a20 2020  elf.edit_F6).   
+00002400: 2020 2020 2073 656c 662e 4636 2e63 6c69       self.F6.cli
+00002410: 636b 6564 2e63 6f6e 6e65 6374 2873 656c  cked.connect(sel
+00002420: 662e 7365 6e64 6636 290a 2020 2020 2020  f.sendf6).      
+00002430: 2020 7365 6c66 2e46 372e 7365 7443 6f6e    self.F7.setCon
+00002440: 7465 7874 4d65 6e75 506f 6c69 6379 2851  textMenuPolicy(Q
+00002450: 7443 6f72 652e 5174 2e43 7573 746f 6d43  tCore.Qt.CustomC
+00002460: 6f6e 7465 7874 4d65 6e75 290a 2020 2020  ontextMenu).    
+00002470: 2020 2020 7365 6c66 2e46 372e 6375 7374      self.F7.cust
+00002480: 6f6d 436f 6e74 6578 744d 656e 7552 6571  omContextMenuReq
+00002490: 7565 7374 6564 2e63 6f6e 6e65 6374 2873  uested.connect(s
+000024a0: 656c 662e 6564 6974 5f46 3729 0a20 2020  elf.edit_F7).   
+000024b0: 2020 2020 2073 656c 662e 4637 2e63 6c69       self.F7.cli
+000024c0: 636b 6564 2e63 6f6e 6e65 6374 2873 656c  cked.connect(sel
+000024d0: 662e 7365 6e64 6637 290a 2020 2020 2020  f.sendf7).      
+000024e0: 2020 7365 6c66 2e46 382e 7365 7443 6f6e    self.F8.setCon
+000024f0: 7465 7874 4d65 6e75 506f 6c69 6379 2851  textMenuPolicy(Q
+00002500: 7443 6f72 652e 5174 2e43 7573 746f 6d43  tCore.Qt.CustomC
+00002510: 6f6e 7465 7874 4d65 6e75 290a 2020 2020  ontextMenu).    
+00002520: 2020 2020 7365 6c66 2e46 382e 6375 7374      self.F8.cust
+00002530: 6f6d 436f 6e74 6578 744d 656e 7552 6571  omContextMenuReq
+00002540: 7565 7374 6564 2e63 6f6e 6e65 6374 2873  uested.connect(s
+00002550: 656c 662e 6564 6974 5f46 3829 0a20 2020  elf.edit_F8).   
+00002560: 2020 2020 2073 656c 662e 4638 2e63 6c69       self.F8.cli
+00002570: 636b 6564 2e63 6f6e 6e65 6374 2873 656c  cked.connect(sel
+00002580: 662e 7365 6e64 6638 290a 2020 2020 2020  f.sendf8).      
+00002590: 2020 7365 6c66 2e46 392e 7365 7443 6f6e    self.F9.setCon
+000025a0: 7465 7874 4d65 6e75 506f 6c69 6379 2851  textMenuPolicy(Q
+000025b0: 7443 6f72 652e 5174 2e43 7573 746f 6d43  tCore.Qt.CustomC
+000025c0: 6f6e 7465 7874 4d65 6e75 290a 2020 2020  ontextMenu).    
+000025d0: 2020 2020 7365 6c66 2e46 392e 6375 7374      self.F9.cust
+000025e0: 6f6d 436f 6e74 6578 744d 656e 7552 6571  omContextMenuReq
+000025f0: 7565 7374 6564 2e63 6f6e 6e65 6374 2873  uested.connect(s
+00002600: 656c 662e 6564 6974 5f46 3929 0a20 2020  elf.edit_F9).   
+00002610: 2020 2020 2073 656c 662e 4639 2e63 6c69       self.F9.cli
+00002620: 636b 6564 2e63 6f6e 6e65 6374 2873 656c  cked.connect(sel
+00002630: 662e 7365 6e64 6639 290a 2020 2020 2020  f.sendf9).      
+00002640: 2020 7365 6c66 2e46 3130 2e73 6574 436f    self.F10.setCo
+00002650: 6e74 6578 744d 656e 7550 6f6c 6963 7928  ntextMenuPolicy(
+00002660: 5174 436f 7265 2e51 742e 4375 7374 6f6d  QtCore.Qt.Custom
+00002670: 436f 6e74 6578 744d 656e 7529 0a20 2020  ContextMenu).   
+00002680: 2020 2020 2073 656c 662e 4631 302e 6375       self.F10.cu
+00002690: 7374 6f6d 436f 6e74 6578 744d 656e 7552  stomContextMenuR
+000026a0: 6571 7565 7374 6564 2e63 6f6e 6e65 6374  equested.connect
+000026b0: 2873 656c 662e 6564 6974 5f46 3130 290a  (self.edit_F10).
+000026c0: 2020 2020 2020 2020 7365 6c66 2e46 3130          self.F10
+000026d0: 2e63 6c69 636b 6564 2e63 6f6e 6e65 6374  .clicked.connect
+000026e0: 2873 656c 662e 7365 6e64 6631 3029 0a20  (self.sendf10). 
+000026f0: 2020 2020 2020 2073 656c 662e 4631 312e         self.F11.
+00002700: 7365 7443 6f6e 7465 7874 4d65 6e75 506f  setContextMenuPo
+00002710: 6c69 6379 2851 7443 6f72 652e 5174 2e43  licy(QtCore.Qt.C
+00002720: 7573 746f 6d43 6f6e 7465 7874 4d65 6e75  ustomContextMenu
+00002730: 290a 2020 2020 2020 2020 7365 6c66 2e46  ).        self.F
+00002740: 3131 2e63 7573 746f 6d43 6f6e 7465 7874  11.customContext
+00002750: 4d65 6e75 5265 7175 6573 7465 642e 636f  MenuRequested.co
+00002760: 6e6e 6563 7428 7365 6c66 2e65 6469 745f  nnect(self.edit_
+00002770: 4631 3129 0a20 2020 2020 2020 2073 656c  F11).        sel
+00002780: 662e 4631 312e 636c 6963 6b65 642e 636f  f.F11.clicked.co
+00002790: 6e6e 6563 7428 7365 6c66 2e73 656e 6466  nnect(self.sendf
+000027a0: 3131 290a 2020 2020 2020 2020 7365 6c66  11).        self
+000027b0: 2e46 3132 2e73 6574 436f 6e74 6578 744d  .F12.setContextM
+000027c0: 656e 7550 6f6c 6963 7928 5174 436f 7265  enuPolicy(QtCore
+000027d0: 2e51 742e 4375 7374 6f6d 436f 6e74 6578  .Qt.CustomContex
+000027e0: 744d 656e 7529 0a20 2020 2020 2020 2073  tMenu).        s
+000027f0: 656c 662e 4631 322e 6375 7374 6f6d 436f  elf.F12.customCo
+00002800: 6e74 6578 744d 656e 7552 6571 7565 7374  ntextMenuRequest
+00002810: 6564 2e63 6f6e 6e65 6374 2873 656c 662e  ed.connect(self.
+00002820: 6564 6974 5f46 3132 290a 2020 2020 2020  edit_F12).      
+00002830: 2020 7365 6c66 2e46 3132 2e63 6c69 636b    self.F12.click
+00002840: 6564 2e63 6f6e 6e65 6374 2873 656c 662e  ed.connect(self.
+00002850: 7365 6e64 6631 3229 0a0a 2020 2020 2020  sendf12)..      
+00002860: 2020 7365 6c66 2e72 6561 6470 7265 6665    self.readprefe
+00002870: 7265 6e63 6573 2829 0a20 2020 2020 2020  rences().       
+00002880: 2073 656c 662e 6462 6e61 6d65 203d 2044   self.dbname = D
+00002890: 4154 415f 5041 5448 202b 2022 2f22 202b  ATA_PATH + "/" +
+000028a0: 2073 656c 662e 7072 6566 2e67 6574 2822   self.pref.get("
+000028b0: 6375 7272 656e 745f 6461 7461 6261 7365  current_database
+000028c0: 222c 2022 6861 6d2e 6462 2229 0a20 2020  ", "ham.db").   
+000028d0: 2020 2020 2073 656c 662e 6461 7461 6261       self.databa
+000028e0: 7365 203d 2044 6174 6142 6173 6528 7365  se = DataBase(se
+000028f0: 6c66 2e64 626e 616d 652c 2057 4f52 4b49  lf.dbname, WORKI
+00002900: 4e47 5f50 4154 4829 0a20 2020 2020 2020  NG_PATH).       
+00002910: 2073 656c 662e 7374 6174 696f 6e20 3d20   self.station = 
+00002920: 7365 6c66 2e64 6174 6162 6173 652e 6665  self.database.fe
+00002930: 7463 685f 7374 6174 696f 6e28 290a 2020  tch_station().  
+00002940: 2020 2020 2020 6966 2073 656c 662e 7374        if self.st
+00002950: 6174 696f 6e20 6973 204e 6f6e 653a 0a20  ation is None:. 
+00002960: 2020 2020 2020 2020 2020 2073 656c 662e             self.
+00002970: 7374 6174 696f 6e20 3d20 7b7d 0a20 2020  station = {}.   
+00002980: 2020 2020 2020 2020 2073 656c 662e 6564           self.ed
+00002990: 6974 5f73 7461 7469 6f6e 5f73 6574 7469  it_station_setti
+000029a0: 6e67 7328 290a 2020 2020 2020 2020 2020  ngs().          
+000029b0: 2020 7365 6c66 2e73 7461 7469 6f6e 203d    self.station =
+000029c0: 2073 656c 662e 6461 7461 6261 7365 2e66   self.database.f
+000029d0: 6574 6368 5f73 7461 7469 6f6e 2829 0a20  etch_station(). 
+000029e0: 2020 2020 2020 2020 2020 2069 6620 7365             if se
+000029f0: 6c66 2e73 7461 7469 6f6e 2069 7320 4e6f  lf.station is No
+00002a00: 6e65 3a0a 2020 2020 2020 2020 2020 2020  ne:.            
+00002a10: 2020 2020 7365 6c66 2e73 7461 7469 6f6e      self.station
+00002a20: 203d 207b 7d0a 2020 2020 2020 2020 7365   = {}.        se
+00002a30: 6c66 2e63 6f6e 7461 6374 203d 2073 656c  lf.contact = sel
+00002a40: 662e 6461 7461 6261 7365 2e65 6d70 7479  f.database.empty
+00002a50: 5f63 6f6e 7461 6374 0a20 2020 2020 2020  _contact.       
+00002a60: 2073 656c 662e 6375 7272 656e 745f 6f70   self.current_op
+00002a70: 203d 2073 656c 662e 7374 6174 696f 6e2e   = self.station.
+00002a80: 6765 7428 2243 616c 6c22 2c20 2222 290a  get("Call", "").
+00002a90: 2020 2020 2020 2020 7365 6c66 2e6d 616b          self.mak
+00002aa0: 655f 6f70 5f64 6972 2829 0a20 2020 2020  e_op_dir().     
+00002ab0: 2020 2069 6620 7365 6c66 2e70 7265 662e     if self.pref.
+00002ac0: 6765 7428 2263 6f6e 7465 7374 2229 3a0a  get("contest"):.
+00002ad0: 2020 2020 2020 2020 2020 2020 7365 6c66              self
+00002ae0: 2e6c 6f61 645f 636f 6e74 6573 7428 290a  .load_contest().
+00002af0: 0a20 2020 2020 2020 2073 656c 662e 7265  .        self.re
+00002b00: 6164 5f63 775f 6d61 6372 6f73 2829 0a20  ad_cw_macros(). 
+00002b10: 2020 2020 2020 2073 656c 662e 636c 6561         self.clea
+00002b20: 7269 6e70 7574 7328 290a 2020 2020 2020  rinputs().      
+00002b30: 2020 2320 7365 6c66 2e6c 6175 6e63 685f    # self.launch_
+00002b40: 6c6f 675f 7769 6e64 6f77 2829 0a0a 2020  log_window()..  
+00002b50: 2020 2020 2020 7365 6c66 2e62 616e 645f        self.band_
+00002b60: 696e 6469 6361 746f 7273 5f63 7720 3d20  indicators_cw = 
+00002b70: 7b0a 2020 2020 2020 2020 2020 2020 2231  {.            "1
+00002b80: 3630 223a 2073 656c 662e 6377 5f62 616e  60": self.cw_ban
+00002b90: 645f 3136 302c 0a20 2020 2020 2020 2020  d_160,.         
+00002ba0: 2020 2022 3830 223a 2073 656c 662e 6377     "80": self.cw
+00002bb0: 5f62 616e 645f 3830 2c0a 2020 2020 2020  _band_80,.      
+00002bc0: 2020 2020 2020 2234 3022 3a20 7365 6c66        "40": self
+00002bd0: 2e63 775f 6261 6e64 5f34 302c 0a20 2020  .cw_band_40,.   
+00002be0: 2020 2020 2020 2020 2022 3230 223a 2073           "20": s
+00002bf0: 656c 662e 6377 5f62 616e 645f 3230 2c0a  elf.cw_band_20,.
+00002c00: 2020 2020 2020 2020 2020 2020 2231 3522              "15"
+00002c10: 3a20 7365 6c66 2e63 775f 6261 6e64 5f31  : self.cw_band_1
+00002c20: 352c 0a20 2020 2020 2020 2020 2020 2022  5,.            "
+00002c30: 3130 223a 2073 656c 662e 6377 5f62 616e  10": self.cw_ban
+00002c40: 645f 3130 2c0a 2020 2020 2020 2020 7d0a  d_10,.        }.
+00002c50: 0a20 2020 2020 2020 2073 656c 662e 6261  .        self.ba
+00002c60: 6e64 5f69 6e64 6963 6174 6f72 735f 7373  nd_indicators_ss
+00002c70: 6220 3d20 7b0a 2020 2020 2020 2020 2020  b = {.          
+00002c80: 2020 2231 3630 223a 2073 656c 662e 7373    "160": self.ss
+00002c90: 625f 6261 6e64 5f31 3630 2c0a 2020 2020  b_band_160,.    
+00002ca0: 2020 2020 2020 2020 2238 3022 3a20 7365          "80": se
+00002cb0: 6c66 2e73 7362 5f62 616e 645f 3830 2c0a  lf.ssb_band_80,.
+00002cc0: 2020 2020 2020 2020 2020 2020 2234 3022              "40"
+00002cd0: 3a20 7365 6c66 2e73 7362 5f62 616e 645f  : self.ssb_band_
+00002ce0: 3430 2c0a 2020 2020 2020 2020 2020 2020  40,.            
+00002cf0: 2232 3022 3a20 7365 6c66 2e73 7362 5f62  "20": self.ssb_b
+00002d00: 616e 645f 3230 2c0a 2020 2020 2020 2020  and_20,.        
+00002d10: 2020 2020 2231 3522 3a20 7365 6c66 2e73      "15": self.s
+00002d20: 7362 5f62 616e 645f 3135 2c0a 2020 2020  sb_band_15,.    
+00002d30: 2020 2020 2020 2020 2231 3022 3a20 7365          "10": se
+00002d40: 6c66 2e73 7362 5f62 616e 645f 3130 2c0a  lf.ssb_band_10,.
+00002d50: 2020 2020 2020 2020 7d0a 0a20 2020 2020          }..     
+00002d60: 2020 2073 656c 662e 6261 6e64 5f69 6e64     self.band_ind
+00002d70: 6963 6174 6f72 735f 7274 7479 203d 207b  icators_rtty = {
+00002d80: 0a20 2020 2020 2020 2020 2020 2022 3136  .            "16
+00002d90: 3022 3a20 7365 6c66 2e72 7474 795f 6261  0": self.rtty_ba
+00002da0: 6e64 5f31 3630 2c0a 2020 2020 2020 2020  nd_160,.        
+00002db0: 2020 2020 2238 3022 3a20 7365 6c66 2e72      "80": self.r
+00002dc0: 7474 795f 6261 6e64 5f38 302c 0a20 2020  tty_band_80,.   
+00002dd0: 2020 2020 2020 2020 2022 3430 223a 2073           "40": s
+00002de0: 656c 662e 7274 7479 5f62 616e 645f 3430  elf.rtty_band_40
+00002df0: 2c0a 2020 2020 2020 2020 2020 2020 2232  ,.            "2
+00002e00: 3022 3a20 7365 6c66 2e72 7474 795f 6261  0": self.rtty_ba
+00002e10: 6e64 5f32 302c 0a20 2020 2020 2020 2020  nd_20,.         
+00002e20: 2020 2022 3135 223a 2073 656c 662e 7274     "15": self.rt
+00002e30: 7479 5f62 616e 645f 3135 2c0a 2020 2020  ty_band_15,.    
+00002e40: 2020 2020 2020 2020 2231 3022 3a20 7365          "10": se
+00002e50: 6c66 2e72 7474 795f 6261 6e64 5f31 302c  lf.rtty_band_10,
+00002e60: 0a20 2020 2020 2020 207d 0a0a 2020 2020  .        }..    
+00002e70: 2020 2020 7365 6c66 2e61 6c6c 5f6d 6f64      self.all_mod
+00002e80: 655f 696e 6469 6361 746f 7273 203d 207b  e_indicators = {
+00002e90: 0a20 2020 2020 2020 2020 2020 2022 4357  .            "CW
+00002ea0: 223a 2073 656c 662e 6261 6e64 5f69 6e64  ": self.band_ind
+00002eb0: 6963 6174 6f72 735f 6377 2c0a 2020 2020  icators_cw,.    
+00002ec0: 2020 2020 2020 2020 2253 5342 223a 2073          "SSB": s
+00002ed0: 656c 662e 6261 6e64 5f69 6e64 6963 6174  elf.band_indicat
+00002ee0: 6f72 735f 7373 622c 0a20 2020 2020 2020  ors_ssb,.       
+00002ef0: 2020 2020 2022 5254 5459 223a 2073 656c       "RTTY": sel
+00002f00: 662e 6261 6e64 5f69 6e64 6963 6174 6f72  f.band_indicator
+00002f10: 735f 7274 7479 2c0a 2020 2020 2020 2020  s_rtty,.        
+00002f20: 7d0a 2020 2020 2020 2020 6966 2073 656c  }.        if sel
+00002f30: 662e 5f75 6470 7761 7463 6820 6973 204e  f._udpwatch is N
+00002f40: 6f6e 653a 0a20 2020 2020 2020 2020 2020  one:.           
+00002f50: 2073 656c 662e 5f75 6470 7761 7463 6820   self._udpwatch 
+00002f60: 3d20 7468 7265 6164 696e 672e 5468 7265  = threading.Thre
+00002f70: 6164 280a 2020 2020 2020 2020 2020 2020  ad(.            
+00002f80: 2020 2020 7461 7267 6574 3d73 656c 662e      target=self.
+00002f90: 7761 7463 685f 7564 702c 0a20 2020 2020  watch_udp,.     
+00002fa0: 2020 2020 2020 2020 2020 2064 6165 6d6f             daemo
+00002fb0: 6e3d 5472 7565 2c0a 2020 2020 2020 2020  n=True,.        
+00002fc0: 2020 2020 290a 2020 2020 2020 2020 2020      ).          
+00002fd0: 2020 7365 6c66 2e5f 7564 7077 6174 6368    self._udpwatch
+00002fe0: 2e73 7461 7274 2829 0a0a 2020 2020 4073  .start()..    @s
+00002ff0: 7461 7469 636d 6574 686f 640a 2020 2020  taticmethod.    
+00003000: 6465 6620 6368 6563 6b5f 7072 6f63 6573  def check_proces
+00003010: 7328 6e61 6d65 3a20 7374 7229 202d 3e20  s(name: str) -> 
+00003020: 626f 6f6c 3a0a 2020 2020 2020 2020 2222  bool:.        ""
+00003030: 2263 6865 636b 7320 746f 2073 6565 2069  "checks to see i
+00003040: 6620 7072 6f67 7261 6d20 6f66 206e 616d  f program of nam
+00003050: 6520 6973 2069 6e20 7468 6520 6163 7469  e is in the acti
+00003060: 7665 2070 726f 6365 7373 206c 6973 7422  ve process list"
+00003070: 2222 0a20 2020 2020 2020 2066 6f72 2070  "".        for p
+00003080: 726f 6320 696e 2070 7375 7469 6c2e 7072  roc in psutil.pr
+00003090: 6f63 6573 735f 6974 6572 2829 3a0a 2020  ocess_iter():.  
+000030a0: 2020 2020 2020 2020 2020 6966 2062 6f6f            if boo
+000030b0: 6c28 7265 2e6d 6174 6368 286e 616d 652c  l(re.match(name,
+000030c0: 2070 726f 632e 6e61 6d65 2829 2e6c 6f77   proc.name().low
+000030d0: 6572 2829 2929 3a0a 2020 2020 2020 2020  er())):.        
+000030e0: 2020 2020 2020 2020 7265 7475 726e 2054          return T
+000030f0: 7275 650a 2020 2020 2020 2020 7265 7475  rue.        retu
+00003100: 726e 2046 616c 7365 0a0a 2020 2020 6465  rn False..    de
+00003110: 6620 7368 6f77 5f6d 6573 7361 6765 5f62  f show_message_b
+00003120: 6f78 2873 656c 662c 206d 6573 7361 6765  ox(self, message
+00003130: 3a20 7374 7229 202d 3e20 4e6f 6e65 3a0a  : str) -> None:.
+00003140: 2020 2020 2020 2020 2222 2264 6f63 2222          """doc""
+00003150: 220a 2020 2020 2020 2020 6d65 7373 6167  ".        messag
+00003160: 655f 626f 7820 3d20 5174 5769 6467 6574  e_box = QtWidget
+00003170: 732e 514d 6573 7361 6765 426f 7828 290a  s.QMessageBox().
+00003180: 2020 2020 2020 2020 6d65 7373 6167 655f          message_
+00003190: 626f 782e 7365 7449 636f 6e28 5174 5769  box.setIcon(QtWi
+000031a0: 6467 6574 732e 514d 6573 7361 6765 426f  dgets.QMessageBo
+000031b0: 782e 496e 666f 726d 6174 696f 6e29 0a20  x.Information). 
+000031c0: 2020 2020 2020 206d 6573 7361 6765 5f62         message_b
+000031d0: 6f78 2e73 6574 5465 7874 286d 6573 7361  ox.setText(messa
+000031e0: 6765 290a 2020 2020 2020 2020 6d65 7373  ge).        mess
+000031f0: 6167 655f 626f 782e 7365 7457 696e 646f  age_box.setWindo
+00003200: 7754 6974 6c65 2822 496e 666f 726d 6174  wTitle("Informat
+00003210: 696f 6e22 290a 2020 2020 2020 2020 6d65  ion").        me
+00003220: 7373 6167 655f 626f 782e 7365 7453 7461  ssage_box.setSta
+00003230: 6e64 6172 6442 7574 746f 6e73 2851 7457  ndardButtons(QtW
+00003240: 6964 6765 7473 2e51 4d65 7373 6167 6542  idgets.QMessageB
+00003250: 6f78 2e4f 6b29 0a20 2020 2020 2020 205f  ox.Ok).        _
+00003260: 203d 206d 6573 7361 6765 5f62 6f78 2e65   = message_box.e
+00003270: 7865 635f 2829 0a0a 2020 2020 6465 6620  xec_()..    def 
+00003280: 7368 6f77 5f61 626f 7574 5f64 6961 6c6f  show_about_dialo
+00003290: 6728 7365 6c66 293a 0a20 2020 2020 2020  g(self):.       
+000032a0: 2022 2222 5368 6f77 2061 626f 7574 2064   """Show about d
+000032b0: 6961 6c6f 6722 2222 0a20 2020 2020 2020  ialog""".       
+000032c0: 2073 656c 662e 6162 6f75 745f 6469 616c   self.about_dial
+000032d0: 6f67 203d 2041 626f 7574 2857 4f52 4b49  og = About(WORKI
+000032e0: 4e47 5f50 4154 4829 0a20 2020 2020 2020  NG_PATH).       
+000032f0: 2069 6620 7365 6c66 2e70 7265 662e 6765   if self.pref.ge
+00003300: 7428 2264 6172 6b5f 6d6f 6465 2229 3a0a  t("dark_mode"):.
+00003310: 2020 2020 2020 2020 2020 2020 7365 6c66              self
+00003320: 2e61 626f 7574 5f64 6961 6c6f 672e 7365  .about_dialog.se
+00003330: 7453 7479 6c65 5368 6565 7428 4441 524b  tStyleSheet(DARK
+00003340: 5f53 5459 4c45 5348 4545 5429 0a20 2020  _STYLESHEET).   
+00003350: 2020 2020 2073 656c 662e 6162 6f75 745f       self.about_
+00003360: 6469 616c 6f67 2e6f 7065 6e28 290a 0a20  dialog.open().. 
+00003370: 2020 2064 6566 2065 6469 745f 636f 6e66     def edit_conf
+00003380: 6967 7572 6174 696f 6e5f 7365 7474 696e  iguration_settin
+00003390: 6773 2873 656c 6629 3a0a 2020 2020 2020  gs(self):.      
+000033a0: 2020 2222 2243 6f6e 6669 6775 7261 7469    """Configurati
+000033b0: 6f6e 2053 6574 7469 6e67 7320 7761 7320  on Settings was 
+000033c0: 636c 6963 6b65 6422 2222 0a20 2020 2020  clicked""".     
+000033d0: 2020 2073 656c 662e 636f 6e66 6967 7572     self.configur
+000033e0: 6174 696f 6e5f 6469 616c 6f67 203d 2053  ation_dialog = S
+000033f0: 6574 7469 6e67 7328 574f 524b 494e 475f  ettings(WORKING_
+00003400: 5041 5448 2c20 434f 4e46 4947 5f50 4154  PATH, CONFIG_PAT
+00003410: 482c 2073 656c 662e 7072 6566 290a 2020  H, self.pref).  
+00003420: 2020 2020 2020 6966 2073 656c 662e 7072        if self.pr
+00003430: 6566 2e67 6574 2822 6461 726b 5f6d 6f64  ef.get("dark_mod
+00003440: 6522 293a 0a20 2020 2020 2020 2020 2020  e"):.           
+00003450: 2073 656c 662e 636f 6e66 6967 7572 6174   self.configurat
+00003460: 696f 6e5f 6469 616c 6f67 2e73 6574 5374  ion_dialog.setSt
+00003470: 796c 6553 6865 6574 2844 4152 4b5f 5354  yleSheet(DARK_ST
+00003480: 594c 4553 4845 4554 290a 2020 2020 2020  YLESHEET).      
+00003490: 2020 7365 6c66 2e63 6f6e 6669 6775 7261    self.configura
+000034a0: 7469 6f6e 5f64 6961 6c6f 672e 7573 6568  tion_dialog.useh
+000034b0: 616d 6462 5f72 6164 696f 4275 7474 6f6e  amdb_radioButton
+000034c0: 2e68 6964 6528 290a 2020 2020 2020 2020  .hide().        
+000034d0: 2320 7365 6c66 2e63 6f6e 6669 6775 7261  # self.configura
+000034e0: 7469 6f6e 5f64 6961 6c6f 672e 6e31 6d6d  tion_dialog.n1mm
+000034f0: 5f74 6162 2e68 6964 6528 290a 2020 2020  _tab.hide().    
+00003500: 2020 2020 7365 6c66 2e63 6f6e 6669 6775      self.configu
+00003510: 7261 7469 6f6e 5f64 6961 6c6f 672e 7368  ration_dialog.sh
+00003520: 6f77 2829 0a20 2020 2020 2020 2073 656c  ow().        sel
+00003530: 662e 636f 6e66 6967 7572 6174 696f 6e5f  f.configuration_
+00003540: 6469 616c 6f67 2e61 6363 6570 7465 642e  dialog.accepted.
+00003550: 636f 6e6e 6563 7428 7365 6c66 2e65 6469  connect(self.edi
+00003560: 745f 636f 6e66 6967 7572 6174 696f 6e5f  t_configuration_
+00003570: 7265 7475 726e 290a 0a20 2020 2064 6566  return)..    def
+00003580: 2065 6469 745f 636f 6e66 6967 7572 6174   edit_configurat
+00003590: 696f 6e5f 7265 7475 726e 2873 656c 6629  ion_return(self)
+000035a0: 3a0a 2020 2020 2020 2020 2222 2252 6574  :.        """Ret
+000035b0: 7572 6e73 2068 6572 6520 7768 656e 2063  urns here when c
+000035c0: 6f6e 6669 6775 7261 7469 6f6e 2064 6961  onfiguration dia
+000035d0: 6c6f 6720 636c 6f73 6564 2077 6974 6820  log closed with 
+000035e0: 6f6b 6179 2e22 2222 0a20 2020 2020 2020  okay.""".       
+000035f0: 2073 656c 662e 636f 6e66 6967 7572 6174   self.configurat
+00003600: 696f 6e5f 6469 616c 6f67 2e73 6176 655f  ion_dialog.save_
+00003610: 6368 616e 6765 7328 290a 2020 2020 2020  changes().      
+00003620: 2020 7365 6c66 2e77 7269 7465 5f70 7265    self.write_pre
+00003630: 6665 7265 6e63 6528 290a 2020 2020 2020  ference().      
+00003640: 2020 6c6f 6767 6572 2e64 6562 7567 2822    logger.debug("
+00003650: 2573 222c 2066 227b 7365 6c66 2e70 7265  %s", f"{self.pre
+00003660: 667d 2229 0a20 2020 2020 2020 2073 656c  f}").        sel
+00003670: 662e 7265 6164 7072 6566 6572 656e 6365  f.readpreference
+00003680: 7328 290a 0a20 2020 2064 6566 206e 6577  s()..    def new
+00003690: 5f64 6174 6162 6173 6528 7365 6c66 293a  _database(self):
+000036a0: 0a20 2020 2020 2020 2022 2222 4372 6561  .        """Crea
+000036b0: 7465 206e 6577 2064 6174 6162 6173 652e  te new database.
+000036c0: 2222 220a 2020 2020 2020 2020 6669 6c65  """.        file
+000036d0: 6e61 6d65 203d 2073 656c 662e 6669 6c65  name = self.file
+000036e0: 7069 636b 6572 2822 6e65 7722 290a 2020  picker("new").  
+000036f0: 2020 2020 2020 6966 2066 696c 656e 616d        if filenam
+00003700: 653a 0a20 2020 2020 2020 2020 2020 2069  e:.            i
+00003710: 6620 6669 6c65 6e61 6d65 5b2d 333a 5d20  f filename[-3:] 
+00003720: 213d 2022 2e64 6222 3a0a 2020 2020 2020  != ".db":.      
+00003730: 2020 2020 2020 2020 2020 6669 6c65 6e61            filena
+00003740: 6d65 202b 3d20 222e 6462 220a 2020 2020  me += ".db".    
+00003750: 2020 2020 2020 2020 7365 6c66 2e70 7265          self.pre
+00003760: 665b 2263 7572 7265 6e74 5f64 6174 6162  f["current_datab
+00003770: 6173 6522 5d20 3d20 6669 6c65 6e61 6d65  ase"] = filename
+00003780: 2e73 706c 6974 2822 2f22 295b 2d31 3a5d  .split("/")[-1:]
+00003790: 5b30 5d0a 2020 2020 2020 2020 2020 2020  [0].            
+000037a0: 7365 6c66 2e77 7269 7465 5f70 7265 6665  self.write_prefe
+000037b0: 7265 6e63 6528 290a 2020 2020 2020 2020  rence().        
+000037c0: 2020 2020 7365 6c66 2e64 626e 616d 6520      self.dbname 
+000037d0: 3d20 4441 5441 5f50 4154 4820 2b20 222f  = DATA_PATH + "/
+000037e0: 2220 2b20 7365 6c66 2e70 7265 662e 6765  " + self.pref.ge
+000037f0: 7428 2263 7572 7265 6e74 5f64 6174 6162  t("current_datab
+00003800: 6173 6522 2c20 2268 616d 2e64 6222 290a  ase", "ham.db").
+00003810: 2020 2020 2020 2020 2020 2020 7365 6c66              self
+00003820: 2e64 6174 6162 6173 6520 3d20 4461 7461  .database = Data
+00003830: 4261 7365 2873 656c 662e 6462 6e61 6d65  Base(self.dbname
+00003840: 2c20 574f 524b 494e 475f 5041 5448 290a  , WORKING_PATH).
+00003850: 2020 2020 2020 2020 2020 2020 7365 6c66              self
+00003860: 2e63 6f6e 7461 6374 203d 2073 656c 662e  .contact = self.
+00003870: 6461 7461 6261 7365 2e65 6d70 7479 5f63  database.empty_c
+00003880: 6f6e 7461 6374 0a20 2020 2020 2020 2020  ontact.         
+00003890: 2020 2073 656c 662e 7374 6174 696f 6e20     self.station 
+000038a0: 3d20 7365 6c66 2e64 6174 6162 6173 652e  = self.database.
+000038b0: 6665 7463 685f 7374 6174 696f 6e28 290a  fetch_station().
+000038c0: 2020 2020 2020 2020 2020 2020 6966 2073              if s
+000038d0: 656c 662e 7374 6174 696f 6e20 6973 204e  elf.station is N
+000038e0: 6f6e 653a 0a20 2020 2020 2020 2020 2020  one:.           
+000038f0: 2020 2020 2073 656c 662e 7374 6174 696f       self.statio
+00003900: 6e20 3d20 7b7d 0a20 2020 2020 2020 2020  n = {}.         
+00003910: 2020 2073 656c 662e 6375 7272 656e 745f     self.current_
+00003920: 6f70 203d 2073 656c 662e 7374 6174 696f  op = self.statio
+00003930: 6e2e 6765 7428 2243 616c 6c22 2c20 2222  n.get("Call", ""
+00003940: 290a 2020 2020 2020 2020 2020 2020 7365  ).            se
+00003950: 6c66 2e6d 616b 655f 6f70 5f64 6972 2829  lf.make_op_dir()
+00003960: 0a20 2020 2020 2020 2020 2020 2063 6d64  .            cmd
+00003970: 203d 207b 7d0a 2020 2020 2020 2020 2020   = {}.          
+00003980: 2020 636d 645b 2263 6d64 225d 203d 2022    cmd["cmd"] = "
+00003990: 4e45 5744 4222 0a20 2020 2020 2020 2020  NEWDB".         
+000039a0: 2020 2063 6d64 5b22 7374 6174 696f 6e22     cmd["station"
+000039b0: 5d20 3d20 706c 6174 666f 726d 2e6e 6f64  ] = platform.nod
+000039c0: 6528 290a 2020 2020 2020 2020 2020 2020  e().            
+000039d0: 7365 6c66 2e6d 756c 7469 6361 7374 5f69  self.multicast_i
+000039e0: 6e74 6572 6661 6365 2e73 656e 645f 6173  nterface.send_as
+000039f0: 5f6a 736f 6e28 636d 6429 0a20 2020 2020  _json(cmd).     
+00003a00: 2020 2020 2020 2073 656c 662e 636c 6561         self.clea
+00003a10: 7269 6e70 7574 7328 290a 2020 2020 2020  rinputs().      
+00003a20: 2020 2020 2020 7365 6c66 2e65 6469 745f        self.edit_
+00003a30: 7374 6174 696f 6e5f 7365 7474 696e 6773  station_settings
+00003a40: 2829 0a0a 2020 2020 6465 6620 6f70 656e  ()..    def open
+00003a50: 5f64 6174 6162 6173 6528 7365 6c66 293a  _database(self):
+00003a60: 0a20 2020 2020 2020 2022 2222 4f70 656e  .        """Open
+00003a70: 2065 7869 7374 696e 6720 6461 7461 6261   existing databa
+00003a80: 7365 2e22 2222 0a20 2020 2020 2020 2066  se.""".        f
+00003a90: 696c 656e 616d 6520 3d20 7365 6c66 2e66  ilename = self.f
+00003aa0: 696c 6570 6963 6b65 7228 226f 7065 6e22  ilepicker("open"
+00003ab0: 290a 2020 2020 2020 2020 6966 2066 696c  ).        if fil
+00003ac0: 656e 616d 653a 0a20 2020 2020 2020 2020  ename:.         
+00003ad0: 2020 2073 656c 662e 7072 6566 5b22 6375     self.pref["cu
+00003ae0: 7272 656e 745f 6461 7461 6261 7365 225d  rrent_database"]
+00003af0: 203d 2066 696c 656e 616d 652e 7370 6c69   = filename.spli
+00003b00: 7428 222f 2229 5b2d 313a 5d5b 305d 0a20  t("/")[-1:][0]. 
+00003b10: 2020 2020 2020 2020 2020 2073 656c 662e             self.
+00003b20: 7772 6974 655f 7072 6566 6572 656e 6365  write_preference
+00003b30: 2829 0a20 2020 2020 2020 2020 2020 2073  ().            s
+00003b40: 656c 662e 6462 6e61 6d65 203d 2044 4154  elf.dbname = DAT
+00003b50: 415f 5041 5448 202b 2022 2f22 202b 2073  A_PATH + "/" + s
+00003b60: 656c 662e 7072 6566 2e67 6574 2822 6375  elf.pref.get("cu
+00003b70: 7272 656e 745f 6461 7461 6261 7365 222c  rrent_database",
+00003b80: 2022 6861 6d2e 6462 2229 0a20 2020 2020   "ham.db").     
+00003b90: 2020 2020 2020 2073 656c 662e 6461 7461         self.data
+00003ba0: 6261 7365 203d 2044 6174 6142 6173 6528  base = DataBase(
+00003bb0: 7365 6c66 2e64 626e 616d 652c 2057 4f52  self.dbname, WOR
+00003bc0: 4b49 4e47 5f50 4154 4829 0a20 2020 2020  KING_PATH).     
+00003bd0: 2020 2020 2020 2073 656c 662e 636f 6e74         self.cont
+00003be0: 6163 7420 3d20 7365 6c66 2e64 6174 6162  act = self.datab
+00003bf0: 6173 652e 656d 7074 795f 636f 6e74 6163  ase.empty_contac
+00003c00: 740a 2020 2020 2020 2020 2020 2020 7365  t.            se
+00003c10: 6c66 2e73 7461 7469 6f6e 203d 2073 656c  lf.station = sel
+00003c20: 662e 6461 7461 6261 7365 2e66 6574 6368  f.database.fetch
+00003c30: 5f73 7461 7469 6f6e 2829 0a20 2020 2020  _station().     
+00003c40: 2020 2020 2020 2069 6620 7365 6c66 2e73         if self.s
+00003c50: 7461 7469 6f6e 2069 7320 4e6f 6e65 3a0a  tation is None:.
+00003c60: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00003c70: 7365 6c66 2e73 7461 7469 6f6e 203d 207b  self.station = {
+00003c80: 7d0a 2020 2020 2020 2020 2020 2020 6966  }.            if
+00003c90: 2073 656c 662e 7374 6174 696f 6e2e 6765   self.station.ge
+00003ca0: 7428 2243 616c 6c22 2c20 2222 2920 3d3d  t("Call", "") ==
+00003cb0: 2022 223a 0a20 2020 2020 2020 2020 2020   "":.           
+00003cc0: 2020 2020 2073 656c 662e 6564 6974 5f73       self.edit_s
+00003cd0: 7461 7469 6f6e 5f73 6574 7469 6e67 7328  tation_settings(
+00003ce0: 290a 2020 2020 2020 2020 2020 2020 7365  ).            se
+00003cf0: 6c66 2e63 7572 7265 6e74 5f6f 7020 3d20  lf.current_op = 
+00003d00: 7365 6c66 2e73 7461 7469 6f6e 2e67 6574  self.station.get
+00003d10: 2822 4361 6c6c 222c 2022 2229 0a20 2020  ("Call", "").   
+00003d20: 2020 2020 2020 2020 2073 656c 662e 6d61           self.ma
+00003d30: 6b65 5f6f 705f 6469 7228 290a 2020 2020  ke_op_dir().    
+00003d40: 2020 2020 2020 2020 636d 6420 3d20 7b7d          cmd = {}
+00003d50: 0a20 2020 2020 2020 2020 2020 2063 6d64  .            cmd
+00003d60: 5b22 636d 6422 5d20 3d20 224e 4557 4442  ["cmd"] = "NEWDB
+00003d70: 220a 2020 2020 2020 2020 2020 2020 636d  ".            cm
+00003d80: 645b 2273 7461 7469 6f6e 225d 203d 2070  d["station"] = p
+00003d90: 6c61 7466 6f72 6d2e 6e6f 6465 2829 0a20  latform.node(). 
+00003da0: 2020 2020 2020 2020 2020 2073 656c 662e             self.
+00003db0: 6d75 6c74 6963 6173 745f 696e 7465 7266  multicast_interf
+00003dc0: 6163 652e 7365 6e64 5f61 735f 6a73 6f6e  ace.send_as_json
+00003dd0: 2863 6d64 290a 2020 2020 2020 2020 2020  (cmd).          
+00003de0: 2020 7365 6c66 2e63 6c65 6172 696e 7075    self.clearinpu
+00003df0: 7473 2829 0a0a 2020 2020 6465 6620 6e65  ts()..    def ne
+00003e00: 775f 636f 6e74 6573 7428 7365 6c66 293a  w_contest(self):
+00003e10: 0a20 2020 2020 2020 2022 2222 4372 6561  .        """Crea
+00003e20: 7465 206e 6577 2063 6f6e 7465 7374 2069  te new contest i
+00003e30: 6e20 6578 6973 7469 6e67 2064 6174 6162  n existing datab
+00003e40: 6173 652e 2222 220a 0a20 2020 2064 6566  ase."""..    def
+00003e50: 206f 7065 6e5f 636f 6e74 6573 7428 7365   open_contest(se
+00003e60: 6c66 293a 0a20 2020 2020 2020 2022 2222  lf):.        """
+00003e70: 5377 6974 6368 2074 6f20 6120 6469 6666  Switch to a diff
+00003e80: 6572 656e 7420 6578 6973 7469 6e67 2063  erent existing c
+00003e90: 6f6e 7465 7374 2069 6e20 6578 6973 7469  ontest in existi
+00003ea0: 6e67 2064 6174 6162 6173 652e 2222 220a  ng database.""".
+00003eb0: 2020 2020 2020 2020 6c6f 6767 6572 2e64          logger.d
+00003ec0: 6562 7567 2822 4f70 656e 2043 6f6e 7465  ebug("Open Conte
+00003ed0: 7374 2073 656c 6563 7465 6422 290a 2020  st selected").  
+00003ee0: 2020 2020 2020 636f 6e74 6573 7473 203d        contests =
+00003ef0: 2073 656c 662e 6461 7461 6261 7365 2e66   self.database.f
+00003f00: 6574 6368 5f61 6c6c 5f63 6f6e 7465 7374  etch_all_contest
+00003f10: 7328 290a 2020 2020 2020 2020 6c6f 6767  s().        logg
+00003f20: 6572 2e64 6562 7567 2822 2573 222c 2066  er.debug("%s", f
+00003f30: 227b 636f 6e74 6573 7473 7d22 290a 0a20  "{contests}").. 
+00003f40: 2020 2020 2020 2069 6620 636f 6e74 6573         if contes
+00003f50: 7473 3a0a 2020 2020 2020 2020 2020 2020  ts:.            
+00003f60: 7365 6c66 2e63 6f6e 7465 7374 5f64 6961  self.contest_dia
+00003f70: 6c6f 6720 3d20 5365 6c65 6374 436f 6e74  log = SelectCont
+00003f80: 6573 7428 574f 524b 494e 475f 5041 5448  est(WORKING_PATH
+00003f90: 290a 2020 2020 2020 2020 2020 2020 6966  ).            if
+00003fa0: 2073 656c 662e 7072 6566 2e67 6574 2822   self.pref.get("
+00003fb0: 6461 726b 5f6d 6f64 6522 293a 0a20 2020  dark_mode"):.   
+00003fc0: 2020 2020 2020 2020 2020 2020 2073 656c               sel
+00003fd0: 662e 636f 6e74 6573 745f 6469 616c 6f67  f.contest_dialog
+00003fe0: 2e73 6574 5374 796c 6553 6865 6574 2844  .setStyleSheet(D
+00003ff0: 4152 4b5f 5354 594c 4553 4845 4554 290a  ARK_STYLESHEET).
+00004000: 2020 2020 2020 2020 2020 2020 7365 6c66              self
+00004010: 2e63 6f6e 7465 7374 5f64 6961 6c6f 672e  .contest_dialog.
+00004020: 636f 6e74 6573 745f 6c69 7374 2e73 6574  contest_list.set
+00004030: 526f 7743 6f75 6e74 2830 290a 2020 2020  RowCount(0).    
+00004040: 2020 2020 2020 2020 7365 6c66 2e63 6f6e          self.con
+00004050: 7465 7374 5f64 6961 6c6f 672e 636f 6e74  test_dialog.cont
+00004060: 6573 745f 6c69 7374 2e73 6574 436f 6c75  est_list.setColu
+00004070: 6d6e 436f 756e 7428 3429 0a20 2020 2020  mnCount(4).     
+00004080: 2020 2020 2020 2073 656c 662e 636f 6e74         self.cont
+00004090: 6573 745f 6469 616c 6f67 2e63 6f6e 7465  est_dialog.conte
+000040a0: 7374 5f6c 6973 742e 7665 7274 6963 616c  st_list.vertical
+000040b0: 4865 6164 6572 2829 2e73 6574 5669 7369  Header().setVisi
+000040c0: 626c 6528 4661 6c73 6529 0a20 2020 2020  ble(False).     
+000040d0: 2020 2020 2020 2073 656c 662e 636f 6e74         self.cont
+000040e0: 6573 745f 6469 616c 6f67 2e63 6f6e 7465  est_dialog.conte
+000040f0: 7374 5f6c 6973 742e 7365 7443 6f6c 756d  st_list.setColum
+00004100: 6e57 6964 7468 2831 2c20 3230 3029 0a20  nWidth(1, 200). 
+00004110: 2020 2020 2020 2020 2020 2073 656c 662e             self.
+00004120: 636f 6e74 6573 745f 6469 616c 6f67 2e63  contest_dialog.c
+00004130: 6f6e 7465 7374 5f6c 6973 742e 7365 7443  ontest_list.setC
+00004140: 6f6c 756d 6e57 6964 7468 2832 2c20 3230  olumnWidth(2, 20
+00004150: 3029 0a20 2020 2020 2020 2020 2020 2073  0).            s
+00004160: 656c 662e 636f 6e74 6573 745f 6469 616c  elf.contest_dial
+00004170: 6f67 2e63 6f6e 7465 7374 5f6c 6973 742e  og.contest_list.
+00004180: 7365 7448 6f72 697a 6f6e 7461 6c48 6561  setHorizontalHea
+00004190: 6465 7249 7465 6d28 0a20 2020 2020 2020  derItem(.       
+000041a0: 2020 2020 2020 2020 2030 2c20 5174 5769           0, QtWi
+000041b0: 6467 6574 732e 5154 6162 6c65 5769 6467  dgets.QTableWidg
+000041c0: 6574 4974 656d 2822 436f 6e74 6573 7420  etItem("Contest 
+000041d0: 4e72 2229 0a20 2020 2020 2020 2020 2020  Nr").           
+000041e0: 2029 0a20 2020 2020 2020 2020 2020 2073   ).            s
+000041f0: 656c 662e 636f 6e74 6573 745f 6469 616c  elf.contest_dial
+00004200: 6f67 2e63 6f6e 7465 7374 5f6c 6973 742e  og.contest_list.
+00004210: 7365 7448 6f72 697a 6f6e 7461 6c48 6561  setHorizontalHea
+00004220: 6465 7249 7465 6d28 0a20 2020 2020 2020  derItem(.       
+00004230: 2020 2020 2020 2020 2031 2c20 5174 5769           1, QtWi
+00004240: 6467 6574 732e 5154 6162 6c65 5769 6467  dgets.QTableWidg
+00004250: 6574 4974 656d 2822 436f 6e74 6573 7420  etItem("Contest 
+00004260: 4e61 6d65 2229 0a20 2020 2020 2020 2020  Name").         
+00004270: 2020 2029 0a20 2020 2020 2020 2020 2020     ).           
+00004280: 2073 656c 662e 636f 6e74 6573 745f 6469   self.contest_di
+00004290: 616c 6f67 2e63 6f6e 7465 7374 5f6c 6973  alog.contest_lis
+000042a0: 742e 7365 7448 6f72 697a 6f6e 7461 6c48  t.setHorizontalH
+000042b0: 6561 6465 7249 7465 6d28 0a20 2020 2020  eaderItem(.     
+000042c0: 2020 2020 2020 2020 2020 2032 2c20 5174             2, Qt
+000042d0: 5769 6467 6574 732e 5154 6162 6c65 5769  Widgets.QTableWi
+000042e0: 6467 6574 4974 656d 2822 436f 6e74 6573  dgetItem("Contes
+000042f0: 7420 5374 6172 7422 290a 2020 2020 2020  t Start").      
+00004300: 2020 2020 2020 290a 2020 2020 2020 2020        ).        
+00004310: 2020 2020 7365 6c66 2e63 6f6e 7465 7374      self.contest
+00004320: 5f64 6961 6c6f 672e 636f 6e74 6573 745f  _dialog.contest_
+00004330: 6c69 7374 2e73 6574 486f 7269 7a6f 6e74  list.setHorizont
+00004340: 616c 4865 6164 6572 4974 656d 280a 2020  alHeaderItem(.  
+00004350: 2020 2020 2020 2020 2020 2020 2020 332c                3,
+00004360: 2051 7457 6964 6765 7473 2e51 5461 626c   QtWidgets.QTabl
+00004370: 6557 6964 6765 7449 7465 6d28 224e 6f74  eWidgetItem("Not
+00004380: 2055 4973 6564 2229 0a20 2020 2020 2020   UIsed").       
+00004390: 2020 2020 2029 0a20 2020 2020 2020 2020       ).         
+000043a0: 2020 2073 656c 662e 636f 6e74 6573 745f     self.contest_
+000043b0: 6469 616c 6f67 2e63 6f6e 7465 7374 5f6c  dialog.contest_l
+000043c0: 6973 742e 7365 7443 6f6c 756d 6e48 6964  ist.setColumnHid
+000043d0: 6465 6e28 302c 2054 7275 6529 0a20 2020  den(0, True).   
+000043e0: 2020 2020 2020 2020 2073 656c 662e 636f           self.co
+000043f0: 6e74 6573 745f 6469 616c 6f67 2e63 6f6e  ntest_dialog.con
+00004400: 7465 7374 5f6c 6973 742e 7365 7443 6f6c  test_list.setCol
+00004410: 756d 6e48 6964 6465 6e28 332c 2054 7275  umnHidden(3, Tru
+00004420: 6529 0a20 2020 2020 2020 2020 2020 2073  e).            s
+00004430: 656c 662e 636f 6e74 6573 745f 6469 616c  elf.contest_dial
+00004440: 6f67 2e61 6363 6570 7465 642e 636f 6e6e  og.accepted.conn
+00004450: 6563 7428 7365 6c66 2e6f 7065 6e5f 636f  ect(self.open_co
+00004460: 6e74 6573 745f 7265 7475 726e 290a 2020  ntest_return).  
+00004470: 2020 2020 2020 2020 2020 666f 7220 636f            for co
+00004480: 6e74 6573 7420 696e 2063 6f6e 7465 7374  ntest in contest
+00004490: 733a 0a20 2020 2020 2020 2020 2020 2020  s:.             
+000044a0: 2020 206e 756d 6265 725f 6f66 5f72 6f77     number_of_row
+000044b0: 7320 3d20 7365 6c66 2e63 6f6e 7465 7374  s = self.contest
+000044c0: 5f64 6961 6c6f 672e 636f 6e74 6573 745f  _dialog.contest_
+000044d0: 6c69 7374 2e72 6f77 436f 756e 7428 290a  list.rowCount().
+000044e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000044f0: 7365 6c66 2e63 6f6e 7465 7374 5f64 6961  self.contest_dia
+00004500: 6c6f 672e 636f 6e74 6573 745f 6c69 7374  log.contest_list
+00004510: 2e69 6e73 6572 7452 6f77 286e 756d 6265  .insertRow(numbe
+00004520: 725f 6f66 5f72 6f77 7329 0a20 2020 2020  r_of_rows).     
+00004530: 2020 2020 2020 2020 2020 2063 6f6e 7465             conte
+00004540: 7374 5f69 6420 3d20 7374 7228 636f 6e74  st_id = str(cont
+00004550: 6573 742e 6765 7428 2243 6f6e 7465 7374  est.get("Contest
+00004560: 4944 222c 2031 2929 0a20 2020 2020 2020  ID", 1)).       
+00004570: 2020 2020 2020 2020 2063 6f6e 7465 7374           contest
+00004580: 5f6e 616d 6520 3d20 636f 6e74 6573 742e  _name = contest.
+00004590: 6765 7428 2243 6f6e 7465 7374 4e61 6d65  get("ContestName
+000045a0: 222c 2031 290a 2020 2020 2020 2020 2020  ", 1).          
+000045b0: 2020 2020 2020 7374 6172 745f 6461 7465        start_date
+000045c0: 203d 2063 6f6e 7465 7374 2e67 6574 2822   = contest.get("
+000045d0: 5374 6172 7444 6174 6522 2c20 3129 0a20  StartDate", 1). 
+000045e0: 2020 2020 2020 2020 2020 2020 2020 2073                 s
+000045f0: 656c 662e 636f 6e74 6573 745f 6469 616c  elf.contest_dial
+00004600: 6f67 2e63 6f6e 7465 7374 5f6c 6973 742e  og.contest_list.
+00004610: 7365 7449 7465 6d28 0a20 2020 2020 2020  setItem(.       
+00004620: 2020 2020 2020 2020 2020 2020 206e 756d               num
+00004630: 6265 725f 6f66 5f72 6f77 732c 2030 2c20  ber_of_rows, 0, 
+00004640: 5174 5769 6467 6574 732e 5154 6162 6c65  QtWidgets.QTable
+00004650: 5769 6467 6574 4974 656d 2863 6f6e 7465  WidgetItem(conte
+00004660: 7374 5f69 6429 0a20 2020 2020 2020 2020  st_id).         
+00004670: 2020 2020 2020 2029 0a20 2020 2020 2020         ).       
+00004680: 2020 2020 2020 2020 2073 656c 662e 636f           self.co
+00004690: 6e74 6573 745f 6469 616c 6f67 2e63 6f6e  ntest_dialog.con
+000046a0: 7465 7374 5f6c 6973 742e 7365 7449 7465  test_list.setIte
+000046b0: 6d28 0a20 2020 2020 2020 2020 2020 2020  m(.             
+000046c0: 2020 2020 2020 206e 756d 6265 725f 6f66         number_of
+000046d0: 5f72 6f77 732c 2031 2c20 5174 5769 6467  _rows, 1, QtWidg
+000046e0: 6574 732e 5154 6162 6c65 5769 6467 6574  ets.QTableWidget
+000046f0: 4974 656d 2863 6f6e 7465 7374 5f6e 616d  Item(contest_nam
+00004700: 6529 0a20 2020 2020 2020 2020 2020 2020  e).             
+00004710: 2020 2029 0a20 2020 2020 2020 2020 2020     ).           
+00004720: 2020 2020 2073 656c 662e 636f 6e74 6573       self.contes
+00004730: 745f 6469 616c 6f67 2e63 6f6e 7465 7374  t_dialog.contest
+00004740: 5f6c 6973 742e 7365 7449 7465 6d28 0a20  _list.setItem(. 
 00004750: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00004760: 2020 6e75 6d62 6572 5f6f 665f 726f 7773    number_of_rows
-00004770: 2c20 322c 2051 7457 6964 6765 7473 2e51  , 2, QtWidgets.Q
-00004780: 5461 626c 6557 6964 6765 7449 7465 6d28  TableWidgetItem(
-00004790: 7374 6172 745f 6461 7465 290a 2020 2020  start_date).    
-000047a0: 2020 2020 2020 2020 2020 2020 290a 2020              ).  
-000047b0: 2020 2020 2020 7365 6c66 2e63 6f6e 7465        self.conte
-000047c0: 7374 5f64 6961 6c6f 672e 7368 6f77 2829  st_dialog.show()
-000047d0: 0a0a 2020 2020 6465 6620 6f70 656e 5f63  ..    def open_c
-000047e0: 6f6e 7465 7374 5f72 6574 7572 6e28 7365  ontest_return(se
-000047f0: 6c66 293a 0a20 2020 2020 2020 2022 2222  lf):.        """
-00004800: 4361 6c6c 6564 2062 7920 6f70 656e 5f63  Called by open_c
-00004810: 6f6e 7465 7374 2222 220a 2020 2020 2020  ontest""".      
-00004820: 2020 7365 6c65 6374 6564 5f72 6f77 203d    selected_row =
-00004830: 2073 656c 662e 636f 6e74 6573 745f 6469   self.contest_di
-00004840: 616c 6f67 2e63 6f6e 7465 7374 5f6c 6973  alog.contest_lis
-00004850: 742e 6375 7272 656e 7452 6f77 2829 0a20  t.currentRow(). 
-00004860: 2020 2020 2020 2063 6f6e 7465 7374 203d         contest =
-00004870: 2073 656c 662e 636f 6e74 6573 745f 6469   self.contest_di
-00004880: 616c 6f67 2e63 6f6e 7465 7374 5f6c 6973  alog.contest_lis
-00004890: 742e 6974 656d 2873 656c 6563 7465 645f  t.item(selected_
-000048a0: 726f 772c 2030 292e 7465 7874 2829 0a20  row, 0).text(). 
-000048b0: 2020 2020 2020 2073 656c 662e 7072 6566         self.pref
-000048c0: 5b22 636f 6e74 6573 7422 5d20 3d20 636f  ["contest"] = co
-000048d0: 6e74 6573 740a 2020 2020 2020 2020 7365  ntest.        se
-000048e0: 6c66 2e77 7269 7465 5f70 7265 6665 7265  lf.write_prefere
-000048f0: 6e63 6528 290a 2020 2020 2020 2020 6c6f  nce().        lo
-00004900: 6767 6572 2e64 6562 7567 2822 5365 6c65  gger.debug("Sele
-00004910: 6374 6564 2063 6f6e 7465 7374 3a20 2573  cted contest: %s
-00004920: 222c 2066 227b 636f 6e74 6573 747d 2229  ", f"{contest}")
-00004930: 0a20 2020 2020 2020 2073 656c 662e 6c6f  .        self.lo
-00004940: 6164 5f63 6f6e 7465 7374 2829 0a0a 2020  ad_contest()..  
-00004950: 2020 6465 6620 7265 6669 6c6c 5f64 726f    def refill_dro
-00004960: 7064 6f77 6e28 7365 6c66 2c20 7461 7267  pdown(self, targ
-00004970: 6574 2c20 736f 7572 6365 293a 0a20 2020  et, source):.   
-00004980: 2020 2020 2022 2222 5265 6669 6c6c 2051       """Refill Q
-00004990: 436f 6d62 6f62 6f78 2077 6964 6765 7420  Combobox widget 
-000049a0: 7769 7468 2076 616c 7565 2e22 2222 0a20  with value.""". 
-000049b0: 2020 2020 2020 2069 6e64 6578 203d 2074         index = t
-000049c0: 6172 6765 742e 6669 6e64 5465 7874 2873  arget.findText(s
-000049d0: 6f75 7263 6529 0a20 2020 2020 2020 2074  ource).        t
-000049e0: 6172 6765 742e 7365 7443 7572 7265 6e74  arget.setCurrent
-000049f0: 496e 6465 7828 696e 6465 7829 0a0a 2020  Index(index)..  
-00004a00: 2020 6465 6620 6564 6974 5f63 6f6e 7465    def edit_conte
-00004a10: 7374 2873 656c 6629 3a0a 2020 2020 2020  st(self):.      
-00004a20: 2020 2222 2245 6469 7420 7468 6520 6375    """Edit the cu
-00004a30: 7272 656e 7420 636f 6e74 6573 7422 2222  rrent contest"""
-00004a40: 0a20 2020 2020 2020 206c 6f67 6765 722e  .        logger.
-00004a50: 6465 6275 6728 2245 6469 7420 636f 6e74  debug("Edit cont
-00004a60: 6573 7420 4469 616c 6f67 2229 0a20 2020  est Dialog").   
-00004a70: 2020 2020 2069 6620 7365 6c66 2e63 6f6e       if self.con
-00004a80: 7465 7374 5f73 6574 7469 6e67 7320 6973  test_settings is
-00004a90: 204e 6f6e 653a 0a20 2020 2020 2020 2020   None:.         
-00004aa0: 2020 2072 6574 7572 6e0a 2020 2020 2020     return.      
-00004ab0: 2020 7365 6c66 2e63 6f6e 7465 7374 5f64    self.contest_d
-00004ac0: 6961 6c6f 6720 3d20 4e65 7743 6f6e 7465  ialog = NewConte
-00004ad0: 7374 2857 4f52 4b49 4e47 5f50 4154 4829  st(WORKING_PATH)
-00004ae0: 0a20 2020 2020 2020 2069 6620 7365 6c66  .        if self
-00004af0: 2e70 7265 662e 6765 7428 2264 6172 6b5f  .pref.get("dark_
-00004b00: 6d6f 6465 2229 3a0a 2020 2020 2020 2020  mode"):.        
-00004b10: 2020 2020 7365 6c66 2e63 6f6e 7465 7374      self.contest
-00004b20: 5f64 6961 6c6f 672e 7365 7453 7479 6c65  _dialog.setStyle
-00004b30: 5368 6565 7428 4441 524b 5f53 5459 4c45  Sheet(DARK_STYLE
-00004b40: 5348 4545 5429 0a20 2020 2020 2020 2073  SHEET).        s
-00004b50: 656c 662e 636f 6e74 6573 745f 6469 616c  elf.contest_dial
-00004b60: 6f67 2e73 6574 5769 6e64 6f77 5469 746c  og.setWindowTitl
-00004b70: 6528 2245 6469 7420 436f 6e74 6573 7422  e("Edit Contest"
-00004b80: 290a 2020 2020 2020 2020 7365 6c66 2e63  ).        self.c
-00004b90: 6f6e 7465 7374 5f64 6961 6c6f 672e 7469  ontest_dialog.ti
-00004ba0: 746c 652e 7365 7454 6578 7428 2222 290a  tle.setText("").
-00004bb0: 2020 2020 2020 2020 7365 6c66 2e63 6f6e          self.con
-00004bc0: 7465 7374 5f64 6961 6c6f 672e 6163 6365  test_dialog.acce
-00004bd0: 7074 6564 2e63 6f6e 6e65 6374 2873 656c  pted.connect(sel
-00004be0: 662e 7361 7665 5f65 6469 7465 645f 636f  f.save_edited_co
-00004bf0: 6e74 6573 7429 0a20 2020 2020 2020 2069  ntest).        i
-00004c00: 6620 7365 6c66 2e70 7265 662e 6765 7428  f self.pref.get(
-00004c10: 2264 6172 6b5f 6d6f 6465 2229 3a0a 2020  "dark_mode"):.  
-00004c20: 2020 2020 2020 2020 2020 7365 6c66 2e63            self.c
-00004c30: 6f6e 7465 7374 5f64 6961 6c6f 672e 7365  ontest_dialog.se
-00004c40: 7453 7479 6c65 5368 6565 7428 4441 524b  tStyleSheet(DARK
-00004c50: 5f53 5459 4c45 5348 4545 5429 0a0a 2020  _STYLESHEET)..  
-00004c60: 2020 2020 2020 7661 6c75 6520 3d20 7365        value = se
-00004c70: 6c66 2e63 6f6e 7465 7374 5f73 6574 7469  lf.contest_setti
-00004c80: 6e67 732e 6765 7428 2243 6f6e 7465 7374  ngs.get("Contest
-00004c90: 4e61 6d65 2229 2e75 7070 6572 2829 2e72  Name").upper().r
-00004ca0: 6570 6c61 6365 2822 5f22 2c20 2220 2229  eplace("_", " ")
-00004cb0: 0a20 2020 2020 2020 2069 6620 7661 6c75  .        if valu
-00004cc0: 6520 3d3d 2022 4745 4e45 5241 4c20 4c4f  e == "GENERAL LO
-00004cd0: 4747 494e 4722 3a0a 2020 2020 2020 2020  GGING":.        
-00004ce0: 2020 2020 7661 6c75 6520 3d20 2247 656e      value = "Gen
-00004cf0: 6572 616c 204c 6f67 6769 6e67 220a 2020  eral Logging".  
-00004d00: 2020 2020 2020 7365 6c66 2e72 6566 696c        self.refil
-00004d10: 6c5f 6472 6f70 646f 776e 2873 656c 662e  l_dropdown(self.
-00004d20: 636f 6e74 6573 745f 6469 616c 6f67 2e63  contest_dialog.c
-00004d30: 6f6e 7465 7374 2c20 7661 6c75 6529 0a20  ontest, value). 
-00004d40: 2020 2020 2020 2076 616c 7565 203d 2073         value = s
-00004d50: 656c 662e 636f 6e74 6573 745f 7365 7474  elf.contest_sett
-00004d60: 696e 6773 2e67 6574 2822 4f70 6572 6174  ings.get("Operat
-00004d70: 6f72 4361 7465 676f 7279 2229 0a20 2020  orCategory").   
-00004d80: 2020 2020 2073 656c 662e 7265 6669 6c6c       self.refill
-00004d90: 5f64 726f 7064 6f77 6e28 7365 6c66 2e63  _dropdown(self.c
-00004da0: 6f6e 7465 7374 5f64 6961 6c6f 672e 6f70  ontest_dialog.op
-00004db0: 6572 6174 6f72 5f63 6c61 7373 2c20 7661  erator_class, va
-00004dc0: 6c75 6529 0a20 2020 2020 2020 2076 616c  lue).        val
-00004dd0: 7565 203d 2073 656c 662e 636f 6e74 6573  ue = self.contes
-00004de0: 745f 7365 7474 696e 6773 2e67 6574 2822  t_settings.get("
-00004df0: 4261 6e64 4361 7465 676f 7279 2229 0a20  BandCategory"). 
-00004e00: 2020 2020 2020 2073 656c 662e 7265 6669         self.refi
-00004e10: 6c6c 5f64 726f 7064 6f77 6e28 7365 6c66  ll_dropdown(self
-00004e20: 2e63 6f6e 7465 7374 5f64 6961 6c6f 672e  .contest_dialog.
-00004e30: 6261 6e64 2c20 7661 6c75 6529 0a20 2020  band, value).   
-00004e40: 2020 2020 2076 616c 7565 203d 2073 656c       value = sel
-00004e50: 662e 636f 6e74 6573 745f 7365 7474 696e  f.contest_settin
-00004e60: 6773 2e67 6574 2822 506f 7765 7243 6174  gs.get("PowerCat
-00004e70: 6567 6f72 7922 290a 2020 2020 2020 2020  egory").        
-00004e80: 7365 6c66 2e72 6566 696c 6c5f 6472 6f70  self.refill_drop
-00004e90: 646f 776e 2873 656c 662e 636f 6e74 6573  down(self.contes
-00004ea0: 745f 6469 616c 6f67 2e70 6f77 6572 2c20  t_dialog.power, 
-00004eb0: 7661 6c75 6529 0a20 2020 2020 2020 2076  value).        v
-00004ec0: 616c 7565 203d 2073 656c 662e 636f 6e74  alue = self.cont
-00004ed0: 6573 745f 7365 7474 696e 6773 2e67 6574  est_settings.get
-00004ee0: 2822 4d6f 6465 4361 7465 676f 7279 2229  ("ModeCategory")
-00004ef0: 0a20 2020 2020 2020 2073 656c 662e 7265  .        self.re
-00004f00: 6669 6c6c 5f64 726f 7064 6f77 6e28 7365  fill_dropdown(se
-00004f10: 6c66 2e63 6f6e 7465 7374 5f64 6961 6c6f  lf.contest_dialo
-00004f20: 672e 6d6f 6465 2c20 7661 6c75 6529 0a20  g.mode, value). 
-00004f30: 2020 2020 2020 2076 616c 7565 203d 2073         value = s
-00004f40: 656c 662e 636f 6e74 6573 745f 7365 7474  elf.contest_sett
-00004f50: 696e 6773 2e67 6574 2822 4f76 6572 6c61  ings.get("Overla
-00004f60: 7943 6174 6567 6f72 7922 290a 2020 2020  yCategory").    
-00004f70: 2020 2020 7365 6c66 2e72 6566 696c 6c5f      self.refill_
-00004f80: 6472 6f70 646f 776e 2873 656c 662e 636f  dropdown(self.co
-00004f90: 6e74 6573 745f 6469 616c 6f67 2e6f 7665  ntest_dialog.ove
-00004fa0: 726c 6179 2c20 7661 6c75 6529 0a20 2020  rlay, value).   
-00004fb0: 2020 2020 2073 656c 662e 636f 6e74 6573       self.contes
-00004fc0: 745f 6469 616c 6f67 2e6f 7065 7261 746f  t_dialog.operato
-00004fd0: 7273 2e73 6574 5465 7874 2873 656c 662e  rs.setText(self.
-00004fe0: 636f 6e74 6573 745f 7365 7474 696e 6773  contest_settings
-00004ff0: 2e67 6574 2822 4f70 6572 6174 6f72 7322  .get("Operators"
-00005000: 2929 0a20 2020 2020 2020 2073 656c 662e  )).        self.
-00005010: 636f 6e74 6573 745f 6469 616c 6f67 2e73  contest_dialog.s
-00005020: 6f61 7062 6f78 2e73 6574 506c 6169 6e54  oapbox.setPlainT
-00005030: 6578 7428 7365 6c66 2e63 6f6e 7465 7374  ext(self.contest
-00005040: 5f73 6574 7469 6e67 732e 6765 7428 2253  _settings.get("S
-00005050: 6f61 7062 6f78 2229 290a 2020 2020 2020  oapbox")).      
-00005060: 2020 7365 6c66 2e63 6f6e 7465 7374 5f64    self.contest_d
-00005070: 6961 6c6f 672e 6578 6368 616e 6765 2e73  ialog.exchange.s
-00005080: 6574 5465 7874 2873 656c 662e 636f 6e74  etText(self.cont
-00005090: 6573 745f 7365 7474 696e 6773 2e67 6574  est_settings.get
-000050a0: 2822 5365 6e74 4578 6368 616e 6765 2229  ("SentExchange")
-000050b0: 290a 2020 2020 2020 2020 7661 6c75 6520  ).        value 
-000050c0: 3d20 7365 6c66 2e63 6f6e 7465 7374 5f73  = self.contest_s
-000050d0: 6574 7469 6e67 732e 6765 7428 2253 7461  ettings.get("Sta
-000050e0: 7469 6f6e 4361 7465 676f 7279 2229 0a20  tionCategory"). 
-000050f0: 2020 2020 2020 2073 656c 662e 7265 6669         self.refi
-00005100: 6c6c 5f64 726f 7064 6f77 6e28 7365 6c66  ll_dropdown(self
-00005110: 2e63 6f6e 7465 7374 5f64 6961 6c6f 672e  .contest_dialog.
-00005120: 7374 6174 696f 6e2c 2076 616c 7565 290a  station, value).
-00005130: 2020 2020 2020 2020 7661 6c75 6520 3d20          value = 
-00005140: 7365 6c66 2e63 6f6e 7465 7374 5f73 6574  self.contest_set
-00005150: 7469 6e67 732e 6765 7428 2241 7373 6973  tings.get("Assis
-00005160: 7465 6443 6174 6567 6f72 7922 290a 2020  tedCategory").  
-00005170: 2020 2020 2020 7365 6c66 2e72 6566 696c        self.refil
-00005180: 6c5f 6472 6f70 646f 776e 2873 656c 662e  l_dropdown(self.
-00005190: 636f 6e74 6573 745f 6469 616c 6f67 2e61  contest_dialog.a
-000051a0: 7373 6973 7465 642c 2076 616c 7565 290a  ssisted, value).
-000051b0: 2020 2020 2020 2020 7661 6c75 6520 3d20          value = 
-000051c0: 7365 6c66 2e63 6f6e 7465 7374 5f73 6574  self.contest_set
-000051d0: 7469 6e67 732e 6765 7428 2254 7261 6e73  tings.get("Trans
-000051e0: 6d69 7474 6572 4361 7465 676f 7279 2229  mitterCategory")
-000051f0: 0a20 2020 2020 2020 2073 656c 662e 7265  .        self.re
-00005200: 6669 6c6c 5f64 726f 7064 6f77 6e28 7365  fill_dropdown(se
-00005210: 6c66 2e63 6f6e 7465 7374 5f64 6961 6c6f  lf.contest_dialo
-00005220: 672e 7472 616e 736d 6974 7465 722c 2076  g.transmitter, v
-00005230: 616c 7565 290a 2020 2020 2020 2020 7661  alue).        va
-00005240: 6c75 6520 3d20 7365 6c66 2e63 6f6e 7465  lue = self.conte
-00005250: 7374 5f73 6574 7469 6e67 732e 6765 7428  st_settings.get(
-00005260: 2253 7461 7274 4461 7465 2229 0a20 2020  "StartDate").   
-00005270: 2020 2020 2074 6865 5f64 6174 652c 2074       the_date, t
-00005280: 6865 5f74 696d 6520 3d20 7661 6c75 652e  he_time = value.
-00005290: 7370 6c69 7428 290a 2020 2020 2020 2020  split().        
-000052a0: 7365 6c66 2e63 6f6e 7465 7374 5f64 6961  self.contest_dia
-000052b0: 6c6f 672e 6461 7465 5469 6d65 4564 6974  log.dateTimeEdit
-000052c0: 2e73 6574 4461 7465 280a 2020 2020 2020  .setDate(.      
-000052d0: 2020 2020 2020 5174 436f 7265 2e51 4461        QtCore.QDa
-000052e0: 7465 2e66 726f 6d53 7472 696e 6728 7468  te.fromString(th
-000052f0: 655f 6461 7465 2c20 2279 7979 792d 4d4d  e_date, "yyyy-MM
-00005300: 2d64 6422 290a 2020 2020 2020 2020 290a  -dd").        ).
-00005310: 2020 2020 2020 2020 7365 6c66 2e63 6f6e          self.con
-00005320: 7465 7374 5f64 6961 6c6f 672e 6461 7465  test_dialog.date
-00005330: 5469 6d65 4564 6974 2e73 6574 4361 6c65  TimeEdit.setCale
-00005340: 6e64 6172 506f 7075 7028 5472 7565 290a  ndarPopup(True).
-00005350: 2020 2020 2020 2020 7365 6c66 2e63 6f6e          self.con
-00005360: 7465 7374 5f64 6961 6c6f 672e 6461 7465  test_dialog.date
-00005370: 5469 6d65 4564 6974 2e73 6574 5469 6d65  TimeEdit.setTime
-00005380: 280a 2020 2020 2020 2020 2020 2020 5174  (.            Qt
-00005390: 436f 7265 2e51 5469 6d65 2e66 726f 6d53  Core.QTime.fromS
-000053a0: 7472 696e 6728 7468 655f 7469 6d65 2c20  tring(the_time, 
-000053b0: 2268 683a 6d6d 3a73 7322 290a 2020 2020  "hh:mm:ss").    
-000053c0: 2020 2020 290a 2020 2020 2020 2020 7365      ).        se
-000053d0: 6c66 2e63 6f6e 7465 7374 5f64 6961 6c6f  lf.contest_dialo
-000053e0: 672e 6f70 656e 2829 0a0a 2020 2020 6465  g.open()..    de
-000053f0: 6620 7361 7665 5f65 6469 7465 645f 636f  f save_edited_co
-00005400: 6e74 6573 7428 7365 6c66 293a 0a20 2020  ntest(self):.   
-00005410: 2020 2020 2022 2222 5361 7665 2074 6865       """Save the
-00005420: 2065 6469 7465 6420 636f 6e74 6573 7422   edited contest"
-00005430: 2222 0a20 2020 2020 2020 2063 6f6e 7465  "".        conte
-00005440: 7374 203d 207b 7d0a 2020 2020 2020 2020  st = {}.        
-00005450: 636f 6e74 6573 745b 2243 6f6e 7465 7374  contest["Contest
-00005460: 4e61 6d65 225d 203d 2028 0a20 2020 2020  Name"] = (.     
-00005470: 2020 2020 2020 2073 656c 662e 636f 6e74         self.cont
-00005480: 6573 745f 6469 616c 6f67 2e63 6f6e 7465  est_dialog.conte
-00005490: 7374 2e63 7572 7265 6e74 5465 7874 2829  st.currentText()
-000054a0: 2e6c 6f77 6572 2829 2e72 6570 6c61 6365  .lower().replace
-000054b0: 2822 2022 2c20 225f 2229 0a20 2020 2020  (" ", "_").     
-000054c0: 2020 2029 0a20 2020 2020 2020 2063 6f6e     ).        con
-000054d0: 7465 7374 5b22 5374 6172 7444 6174 6522  test["StartDate"
-000054e0: 5d20 3d20 7365 6c66 2e63 6f6e 7465 7374  ] = self.contest
-000054f0: 5f64 6961 6c6f 672e 6461 7465 5469 6d65  _dialog.dateTime
-00005500: 4564 6974 2e64 6174 6554 696d 6528 292e  Edit.dateTime().
-00005510: 746f 5374 7269 6e67 280a 2020 2020 2020  toString(.      
-00005520: 2020 2020 2020 2279 7979 792d 4d4d 2d64        "yyyy-MM-d
-00005530: 6420 6868 3a6d 6d3a 7373 220a 2020 2020  d hh:mm:ss".    
-00005540: 2020 2020 290a 2020 2020 2020 2020 636f      ).        co
-00005550: 6e74 6573 745b 224f 7065 7261 746f 7243  ntest["OperatorC
-00005560: 6174 6567 6f72 7922 5d20 3d20 7365 6c66  ategory"] = self
-00005570: 2e63 6f6e 7465 7374 5f64 6961 6c6f 672e  .contest_dialog.
-00005580: 6f70 6572 6174 6f72 5f63 6c61 7373 2e63  operator_class.c
-00005590: 7572 7265 6e74 5465 7874 2829 0a20 2020  urrentText().   
-000055a0: 2020 2020 2063 6f6e 7465 7374 5b22 4261       contest["Ba
-000055b0: 6e64 4361 7465 676f 7279 225d 203d 2073  ndCategory"] = s
-000055c0: 656c 662e 636f 6e74 6573 745f 6469 616c  elf.contest_dial
-000055d0: 6f67 2e62 616e 642e 6375 7272 656e 7454  og.band.currentT
-000055e0: 6578 7428 290a 2020 2020 2020 2020 636f  ext().        co
-000055f0: 6e74 6573 745b 2250 6f77 6572 4361 7465  ntest["PowerCate
-00005600: 676f 7279 225d 203d 2073 656c 662e 636f  gory"] = self.co
-00005610: 6e74 6573 745f 6469 616c 6f67 2e70 6f77  ntest_dialog.pow
-00005620: 6572 2e63 7572 7265 6e74 5465 7874 2829  er.currentText()
-00005630: 0a20 2020 2020 2020 2063 6f6e 7465 7374  .        contest
-00005640: 5b22 4d6f 6465 4361 7465 676f 7279 225d  ["ModeCategory"]
-00005650: 203d 2073 656c 662e 636f 6e74 6573 745f   = self.contest_
-00005660: 6469 616c 6f67 2e6d 6f64 652e 6375 7272  dialog.mode.curr
-00005670: 656e 7454 6578 7428 290a 2020 2020 2020  entText().      
-00005680: 2020 636f 6e74 6573 745b 224f 7665 726c    contest["Overl
-00005690: 6179 4361 7465 676f 7279 225d 203d 2073  ayCategory"] = s
-000056a0: 656c 662e 636f 6e74 6573 745f 6469 616c  elf.contest_dial
-000056b0: 6f67 2e6f 7665 726c 6179 2e63 7572 7265  og.overlay.curre
-000056c0: 6e74 5465 7874 2829 0a20 2020 2020 2020  ntText().       
-000056d0: 2063 6f6e 7465 7374 5b22 4f70 6572 6174   contest["Operat
-000056e0: 6f72 7322 5d20 3d20 7365 6c66 2e63 6f6e  ors"] = self.con
-000056f0: 7465 7374 5f64 6961 6c6f 672e 6f70 6572  test_dialog.oper
-00005700: 6174 6f72 732e 7465 7874 2829 0a20 2020  ators.text().   
-00005710: 2020 2020 2063 6f6e 7465 7374 5b22 536f       contest["So
-00005720: 6170 626f 7822 5d20 3d20 7365 6c66 2e63  apbox"] = self.c
-00005730: 6f6e 7465 7374 5f64 6961 6c6f 672e 736f  ontest_dialog.so
-00005740: 6170 626f 782e 746f 506c 6169 6e54 6578  apbox.toPlainTex
-00005750: 7428 290a 2020 2020 2020 2020 636f 6e74  t().        cont
-00005760: 6573 745b 2253 656e 7445 7863 6861 6e67  est["SentExchang
-00005770: 6522 5d20 3d20 7365 6c66 2e63 6f6e 7465  e"] = self.conte
-00005780: 7374 5f64 6961 6c6f 672e 6578 6368 616e  st_dialog.exchan
-00005790: 6765 2e74 6578 7428 290a 2020 2020 2020  ge.text().      
-000057a0: 2020 636f 6e74 6573 745b 2243 6f6e 7465    contest["Conte
-000057b0: 7374 4e52 225d 203d 2073 656c 662e 7072  stNR"] = self.pr
-000057c0: 6566 2e67 6574 2822 636f 6e74 6573 7422  ef.get("contest"
-000057d0: 2c20 3129 0a20 2020 2020 2020 2063 6f6e  , 1).        con
-000057e0: 7465 7374 5b22 5374 6174 696f 6e43 6174  test["StationCat
-000057f0: 6567 6f72 7922 5d20 3d20 7365 6c66 2e63  egory"] = self.c
-00005800: 6f6e 7465 7374 5f64 6961 6c6f 672e 7374  ontest_dialog.st
-00005810: 6174 696f 6e2e 6375 7272 656e 7454 6578  ation.currentTex
-00005820: 7428 290a 2020 2020 2020 2020 636f 6e74  t().        cont
-00005830: 6573 745b 2241 7373 6973 7465 6443 6174  est["AssistedCat
-00005840: 6567 6f72 7922 5d20 3d20 7365 6c66 2e63  egory"] = self.c
-00005850: 6f6e 7465 7374 5f64 6961 6c6f 672e 6173  ontest_dialog.as
-00005860: 7369 7374 6564 2e63 7572 7265 6e74 5465  sisted.currentTe
-00005870: 7874 2829 0a20 2020 2020 2020 2063 6f6e  xt().        con
-00005880: 7465 7374 5b22 5472 616e 736d 6974 7465  test["Transmitte
-00005890: 7243 6174 6567 6f72 7922 5d20 3d20 7365  rCategory"] = se
-000058a0: 6c66 2e63 6f6e 7465 7374 5f64 6961 6c6f  lf.contest_dialo
-000058b0: 672e 7472 616e 736d 6974 7465 722e 6375  g.transmitter.cu
-000058c0: 7272 656e 7454 6578 7428 290a 0a20 2020  rrentText()..   
-000058d0: 2020 2020 206c 6f67 6765 722e 6465 6275       logger.debu
-000058e0: 6728 2225 7322 2c20 6622 7b63 6f6e 7465  g("%s", f"{conte
-000058f0: 7374 7d22 290a 2020 2020 2020 2020 7365  st}").        se
-00005900: 6c66 2e64 6174 6162 6173 652e 7570 6461  lf.database.upda
-00005910: 7465 5f63 6f6e 7465 7374 2863 6f6e 7465  te_contest(conte
-00005920: 7374 290a 2020 2020 2020 2020 7365 6c66  st).        self
-00005930: 2e77 7269 7465 5f70 7265 6665 7265 6e63  .write_preferenc
-00005940: 6528 290a 2020 2020 2020 2020 7365 6c66  e().        self
-00005950: 2e6c 6f61 645f 636f 6e74 6573 7428 290a  .load_contest().
-00005960: 0a20 2020 2064 6566 206c 6f61 645f 636f  .    def load_co
-00005970: 6e74 6573 7428 7365 6c66 293a 0a20 2020  ntest(self):.   
-00005980: 2020 2020 2022 2222 6c6f 6164 2061 2063       """load a c
-00005990: 6f6e 7465 7374 2222 220a 2020 2020 2020  ontest""".      
-000059a0: 2020 6966 2073 656c 662e 7072 6566 2e67    if self.pref.g
-000059b0: 6574 2822 636f 6e74 6573 7422 293a 0a20  et("contest"):. 
-000059c0: 2020 2020 2020 2020 2020 2073 656c 662e             self.
-000059d0: 636f 6e74 6573 745f 7365 7474 696e 6773  contest_settings
-000059e0: 203d 2073 656c 662e 6461 7461 6261 7365   = self.database
-000059f0: 2e66 6574 6368 5f63 6f6e 7465 7374 5f62  .fetch_contest_b
-00005a00: 795f 6964 280a 2020 2020 2020 2020 2020  y_id(.          
-00005a10: 2020 2020 2020 7365 6c66 2e70 7265 662e        self.pref.
-00005a20: 6765 7428 2263 6f6e 7465 7374 2229 0a20  get("contest"). 
-00005a30: 2020 2020 2020 2020 2020 2029 0a20 2020             ).   
-00005a40: 2020 2020 2020 2020 2069 6620 7365 6c66           if self
-00005a50: 2e63 6f6e 7465 7374 5f73 6574 7469 6e67  .contest_setting
-00005a60: 733a 0a20 2020 2020 2020 2020 2020 2020  s:.             
-00005a70: 2020 2073 656c 662e 6461 7461 6261 7365     self.database
-00005a80: 2e63 7572 7265 6e74 5f63 6f6e 7465 7374  .current_contest
-00005a90: 203d 2073 656c 662e 7072 6566 2e67 6574   = self.pref.get
-00005aa0: 2822 636f 6e74 6573 7422 290a 2020 2020  ("contest").    
-00005ab0: 2020 2020 2020 2020 2020 2020 6966 2073              if s
-00005ac0: 656c 662e 636f 6e74 6573 745f 7365 7474  elf.contest_sett
-00005ad0: 696e 6773 2e67 6574 2822 436f 6e74 6573  ings.get("Contes
-00005ae0: 744e 616d 6522 293a 0a20 2020 2020 2020  tName"):.       
-00005af0: 2020 2020 2020 2020 2020 2020 2073 656c               sel
-00005b00: 662e 636f 6e74 6573 7420 3d20 646f 696d  f.contest = doim
-00005b10: 7028 7365 6c66 2e63 6f6e 7465 7374 5f73  p(self.contest_s
-00005b20: 6574 7469 6e67 732e 6765 7428 2243 6f6e  ettings.get("Con
-00005b30: 7465 7374 4e61 6d65 2229 290a 2020 2020  testName")).    
+00004760: 2020 206e 756d 6265 725f 6f66 5f72 6f77     number_of_row
+00004770: 732c 2032 2c20 5174 5769 6467 6574 732e  s, 2, QtWidgets.
+00004780: 5154 6162 6c65 5769 6467 6574 4974 656d  QTableWidgetItem
+00004790: 2873 7461 7274 5f64 6174 6529 0a20 2020  (start_date).   
+000047a0: 2020 2020 2020 2020 2020 2020 2029 0a20               ). 
+000047b0: 2020 2020 2020 2073 656c 662e 636f 6e74         self.cont
+000047c0: 6573 745f 6469 616c 6f67 2e73 686f 7728  est_dialog.show(
+000047d0: 290a 0a20 2020 2064 6566 206f 7065 6e5f  )..    def open_
+000047e0: 636f 6e74 6573 745f 7265 7475 726e 2873  contest_return(s
+000047f0: 656c 6629 3a0a 2020 2020 2020 2020 2222  elf):.        ""
+00004800: 2243 616c 6c65 6420 6279 206f 7065 6e5f  "Called by open_
+00004810: 636f 6e74 6573 7422 2222 0a20 2020 2020  contest""".     
+00004820: 2020 2073 656c 6563 7465 645f 726f 7720     selected_row 
+00004830: 3d20 7365 6c66 2e63 6f6e 7465 7374 5f64  = self.contest_d
+00004840: 6961 6c6f 672e 636f 6e74 6573 745f 6c69  ialog.contest_li
+00004850: 7374 2e63 7572 7265 6e74 526f 7728 290a  st.currentRow().
+00004860: 2020 2020 2020 2020 636f 6e74 6573 7420          contest 
+00004870: 3d20 7365 6c66 2e63 6f6e 7465 7374 5f64  = self.contest_d
+00004880: 6961 6c6f 672e 636f 6e74 6573 745f 6c69  ialog.contest_li
+00004890: 7374 2e69 7465 6d28 7365 6c65 6374 6564  st.item(selected
+000048a0: 5f72 6f77 2c20 3029 2e74 6578 7428 290a  _row, 0).text().
+000048b0: 2020 2020 2020 2020 7365 6c66 2e70 7265          self.pre
+000048c0: 665b 2263 6f6e 7465 7374 225d 203d 2063  f["contest"] = c
+000048d0: 6f6e 7465 7374 0a20 2020 2020 2020 2073  ontest.        s
+000048e0: 656c 662e 7772 6974 655f 7072 6566 6572  elf.write_prefer
+000048f0: 656e 6365 2829 0a20 2020 2020 2020 206c  ence().        l
+00004900: 6f67 6765 722e 6465 6275 6728 2253 656c  ogger.debug("Sel
+00004910: 6563 7465 6420 636f 6e74 6573 743a 2025  ected contest: %
+00004920: 7322 2c20 6622 7b63 6f6e 7465 7374 7d22  s", f"{contest}"
+00004930: 290a 2020 2020 2020 2020 7365 6c66 2e6c  ).        self.l
+00004940: 6f61 645f 636f 6e74 6573 7428 290a 0a20  oad_contest().. 
+00004950: 2020 2064 6566 2072 6566 696c 6c5f 6472     def refill_dr
+00004960: 6f70 646f 776e 2873 656c 662c 2074 6172  opdown(self, tar
+00004970: 6765 742c 2073 6f75 7263 6529 3a0a 2020  get, source):.  
+00004980: 2020 2020 2020 2222 2252 6566 696c 6c20        """Refill 
+00004990: 5143 6f6d 626f 626f 7820 7769 6467 6574  QCombobox widget
+000049a0: 2077 6974 6820 7661 6c75 652e 2222 220a   with value.""".
+000049b0: 2020 2020 2020 2020 696e 6465 7820 3d20          index = 
+000049c0: 7461 7267 6574 2e66 696e 6454 6578 7428  target.findText(
+000049d0: 736f 7572 6365 290a 2020 2020 2020 2020  source).        
+000049e0: 7461 7267 6574 2e73 6574 4375 7272 656e  target.setCurren
+000049f0: 7449 6e64 6578 2869 6e64 6578 290a 0a20  tIndex(index).. 
+00004a00: 2020 2064 6566 2065 6469 745f 636f 6e74     def edit_cont
+00004a10: 6573 7428 7365 6c66 293a 0a20 2020 2020  est(self):.     
+00004a20: 2020 2022 2222 4564 6974 2074 6865 2063     """Edit the c
+00004a30: 7572 7265 6e74 2063 6f6e 7465 7374 2222  urrent contest""
+00004a40: 220a 2020 2020 2020 2020 6c6f 6767 6572  ".        logger
+00004a50: 2e64 6562 7567 2822 4564 6974 2063 6f6e  .debug("Edit con
+00004a60: 7465 7374 2044 6961 6c6f 6722 290a 2020  test Dialog").  
+00004a70: 2020 2020 2020 6966 2073 656c 662e 636f        if self.co
+00004a80: 6e74 6573 745f 7365 7474 696e 6773 2069  ntest_settings i
+00004a90: 7320 4e6f 6e65 3a0a 2020 2020 2020 2020  s None:.        
+00004aa0: 2020 2020 7265 7475 726e 0a20 2020 2020      return.     
+00004ab0: 2020 2073 656c 662e 636f 6e74 6573 745f     self.contest_
+00004ac0: 6469 616c 6f67 203d 204e 6577 436f 6e74  dialog = NewCont
+00004ad0: 6573 7428 574f 524b 494e 475f 5041 5448  est(WORKING_PATH
+00004ae0: 290a 2020 2020 2020 2020 6966 2073 656c  ).        if sel
+00004af0: 662e 7072 6566 2e67 6574 2822 6461 726b  f.pref.get("dark
+00004b00: 5f6d 6f64 6522 293a 0a20 2020 2020 2020  _mode"):.       
+00004b10: 2020 2020 2073 656c 662e 636f 6e74 6573       self.contes
+00004b20: 745f 6469 616c 6f67 2e73 6574 5374 796c  t_dialog.setStyl
+00004b30: 6553 6865 6574 2844 4152 4b5f 5354 594c  eSheet(DARK_STYL
+00004b40: 4553 4845 4554 290a 2020 2020 2020 2020  ESHEET).        
+00004b50: 7365 6c66 2e63 6f6e 7465 7374 5f64 6961  self.contest_dia
+00004b60: 6c6f 672e 7365 7457 696e 646f 7754 6974  log.setWindowTit
+00004b70: 6c65 2822 4564 6974 2043 6f6e 7465 7374  le("Edit Contest
+00004b80: 2229 0a20 2020 2020 2020 2073 656c 662e  ").        self.
+00004b90: 636f 6e74 6573 745f 6469 616c 6f67 2e74  contest_dialog.t
+00004ba0: 6974 6c65 2e73 6574 5465 7874 2822 2229  itle.setText("")
+00004bb0: 0a20 2020 2020 2020 2073 656c 662e 636f  .        self.co
+00004bc0: 6e74 6573 745f 6469 616c 6f67 2e61 6363  ntest_dialog.acc
+00004bd0: 6570 7465 642e 636f 6e6e 6563 7428 7365  epted.connect(se
+00004be0: 6c66 2e73 6176 655f 6564 6974 6564 5f63  lf.save_edited_c
+00004bf0: 6f6e 7465 7374 290a 2020 2020 2020 2020  ontest).        
+00004c00: 6966 2073 656c 662e 7072 6566 2e67 6574  if self.pref.get
+00004c10: 2822 6461 726b 5f6d 6f64 6522 293a 0a20  ("dark_mode"):. 
+00004c20: 2020 2020 2020 2020 2020 2073 656c 662e             self.
+00004c30: 636f 6e74 6573 745f 6469 616c 6f67 2e73  contest_dialog.s
+00004c40: 6574 5374 796c 6553 6865 6574 2844 4152  etStyleSheet(DAR
+00004c50: 4b5f 5354 594c 4553 4845 4554 290a 0a20  K_STYLESHEET).. 
+00004c60: 2020 2020 2020 2076 616c 7565 203d 2073         value = s
+00004c70: 656c 662e 636f 6e74 6573 745f 7365 7474  elf.contest_sett
+00004c80: 696e 6773 2e67 6574 2822 436f 6e74 6573  ings.get("Contes
+00004c90: 744e 616d 6522 292e 7570 7065 7228 292e  tName").upper().
+00004ca0: 7265 706c 6163 6528 225f 222c 2022 2022  replace("_", " "
+00004cb0: 290a 2020 2020 2020 2020 6966 2076 616c  ).        if val
+00004cc0: 7565 203d 3d20 2247 454e 4552 414c 204c  ue == "GENERAL L
+00004cd0: 4f47 4749 4e47 223a 0a20 2020 2020 2020  OGGING":.       
+00004ce0: 2020 2020 2076 616c 7565 203d 2022 4765       value = "Ge
+00004cf0: 6e65 7261 6c20 4c6f 6767 696e 6722 0a20  neral Logging". 
+00004d00: 2020 2020 2020 2073 656c 662e 7265 6669         self.refi
+00004d10: 6c6c 5f64 726f 7064 6f77 6e28 7365 6c66  ll_dropdown(self
+00004d20: 2e63 6f6e 7465 7374 5f64 6961 6c6f 672e  .contest_dialog.
+00004d30: 636f 6e74 6573 742c 2076 616c 7565 290a  contest, value).
+00004d40: 2020 2020 2020 2020 7661 6c75 6520 3d20          value = 
+00004d50: 7365 6c66 2e63 6f6e 7465 7374 5f73 6574  self.contest_set
+00004d60: 7469 6e67 732e 6765 7428 224f 7065 7261  tings.get("Opera
+00004d70: 746f 7243 6174 6567 6f72 7922 290a 2020  torCategory").  
+00004d80: 2020 2020 2020 7365 6c66 2e72 6566 696c        self.refil
+00004d90: 6c5f 6472 6f70 646f 776e 2873 656c 662e  l_dropdown(self.
+00004da0: 636f 6e74 6573 745f 6469 616c 6f67 2e6f  contest_dialog.o
+00004db0: 7065 7261 746f 725f 636c 6173 732c 2076  perator_class, v
+00004dc0: 616c 7565 290a 2020 2020 2020 2020 7661  alue).        va
+00004dd0: 6c75 6520 3d20 7365 6c66 2e63 6f6e 7465  lue = self.conte
+00004de0: 7374 5f73 6574 7469 6e67 732e 6765 7428  st_settings.get(
+00004df0: 2242 616e 6443 6174 6567 6f72 7922 290a  "BandCategory").
+00004e00: 2020 2020 2020 2020 7365 6c66 2e72 6566          self.ref
+00004e10: 696c 6c5f 6472 6f70 646f 776e 2873 656c  ill_dropdown(sel
+00004e20: 662e 636f 6e74 6573 745f 6469 616c 6f67  f.contest_dialog
+00004e30: 2e62 616e 642c 2076 616c 7565 290a 2020  .band, value).  
+00004e40: 2020 2020 2020 7661 6c75 6520 3d20 7365        value = se
+00004e50: 6c66 2e63 6f6e 7465 7374 5f73 6574 7469  lf.contest_setti
+00004e60: 6e67 732e 6765 7428 2250 6f77 6572 4361  ngs.get("PowerCa
+00004e70: 7465 676f 7279 2229 0a20 2020 2020 2020  tegory").       
+00004e80: 2073 656c 662e 7265 6669 6c6c 5f64 726f   self.refill_dro
+00004e90: 7064 6f77 6e28 7365 6c66 2e63 6f6e 7465  pdown(self.conte
+00004ea0: 7374 5f64 6961 6c6f 672e 706f 7765 722c  st_dialog.power,
+00004eb0: 2076 616c 7565 290a 2020 2020 2020 2020   value).        
+00004ec0: 7661 6c75 6520 3d20 7365 6c66 2e63 6f6e  value = self.con
+00004ed0: 7465 7374 5f73 6574 7469 6e67 732e 6765  test_settings.ge
+00004ee0: 7428 224d 6f64 6543 6174 6567 6f72 7922  t("ModeCategory"
+00004ef0: 290a 2020 2020 2020 2020 7365 6c66 2e72  ).        self.r
+00004f00: 6566 696c 6c5f 6472 6f70 646f 776e 2873  efill_dropdown(s
+00004f10: 656c 662e 636f 6e74 6573 745f 6469 616c  elf.contest_dial
+00004f20: 6f67 2e6d 6f64 652c 2076 616c 7565 290a  og.mode, value).
+00004f30: 2020 2020 2020 2020 7661 6c75 6520 3d20          value = 
+00004f40: 7365 6c66 2e63 6f6e 7465 7374 5f73 6574  self.contest_set
+00004f50: 7469 6e67 732e 6765 7428 224f 7665 726c  tings.get("Overl
+00004f60: 6179 4361 7465 676f 7279 2229 0a20 2020  ayCategory").   
+00004f70: 2020 2020 2073 656c 662e 7265 6669 6c6c       self.refill
+00004f80: 5f64 726f 7064 6f77 6e28 7365 6c66 2e63  _dropdown(self.c
+00004f90: 6f6e 7465 7374 5f64 6961 6c6f 672e 6f76  ontest_dialog.ov
+00004fa0: 6572 6c61 792c 2076 616c 7565 290a 2020  erlay, value).  
+00004fb0: 2020 2020 2020 7365 6c66 2e63 6f6e 7465        self.conte
+00004fc0: 7374 5f64 6961 6c6f 672e 6f70 6572 6174  st_dialog.operat
+00004fd0: 6f72 732e 7365 7454 6578 7428 7365 6c66  ors.setText(self
+00004fe0: 2e63 6f6e 7465 7374 5f73 6574 7469 6e67  .contest_setting
+00004ff0: 732e 6765 7428 224f 7065 7261 746f 7273  s.get("Operators
+00005000: 2229 290a 2020 2020 2020 2020 7365 6c66  ")).        self
+00005010: 2e63 6f6e 7465 7374 5f64 6961 6c6f 672e  .contest_dialog.
+00005020: 736f 6170 626f 782e 7365 7450 6c61 696e  soapbox.setPlain
+00005030: 5465 7874 2873 656c 662e 636f 6e74 6573  Text(self.contes
+00005040: 745f 7365 7474 696e 6773 2e67 6574 2822  t_settings.get("
+00005050: 536f 6170 626f 7822 2929 0a20 2020 2020  Soapbox")).     
+00005060: 2020 2073 656c 662e 636f 6e74 6573 745f     self.contest_
+00005070: 6469 616c 6f67 2e65 7863 6861 6e67 652e  dialog.exchange.
+00005080: 7365 7454 6578 7428 7365 6c66 2e63 6f6e  setText(self.con
+00005090: 7465 7374 5f73 6574 7469 6e67 732e 6765  test_settings.ge
+000050a0: 7428 2253 656e 7445 7863 6861 6e67 6522  t("SentExchange"
+000050b0: 2929 0a20 2020 2020 2020 2076 616c 7565  )).        value
+000050c0: 203d 2073 656c 662e 636f 6e74 6573 745f   = self.contest_
+000050d0: 7365 7474 696e 6773 2e67 6574 2822 5374  settings.get("St
+000050e0: 6174 696f 6e43 6174 6567 6f72 7922 290a  ationCategory").
+000050f0: 2020 2020 2020 2020 7365 6c66 2e72 6566          self.ref
+00005100: 696c 6c5f 6472 6f70 646f 776e 2873 656c  ill_dropdown(sel
+00005110: 662e 636f 6e74 6573 745f 6469 616c 6f67  f.contest_dialog
+00005120: 2e73 7461 7469 6f6e 2c20 7661 6c75 6529  .station, value)
+00005130: 0a20 2020 2020 2020 2076 616c 7565 203d  .        value =
+00005140: 2073 656c 662e 636f 6e74 6573 745f 7365   self.contest_se
+00005150: 7474 696e 6773 2e67 6574 2822 4173 7369  ttings.get("Assi
+00005160: 7374 6564 4361 7465 676f 7279 2229 0a20  stedCategory"). 
+00005170: 2020 2020 2020 2073 656c 662e 7265 6669         self.refi
+00005180: 6c6c 5f64 726f 7064 6f77 6e28 7365 6c66  ll_dropdown(self
+00005190: 2e63 6f6e 7465 7374 5f64 6961 6c6f 672e  .contest_dialog.
+000051a0: 6173 7369 7374 6564 2c20 7661 6c75 6529  assisted, value)
+000051b0: 0a20 2020 2020 2020 2076 616c 7565 203d  .        value =
+000051c0: 2073 656c 662e 636f 6e74 6573 745f 7365   self.contest_se
+000051d0: 7474 696e 6773 2e67 6574 2822 5472 616e  ttings.get("Tran
+000051e0: 736d 6974 7465 7243 6174 6567 6f72 7922  smitterCategory"
+000051f0: 290a 2020 2020 2020 2020 7365 6c66 2e72  ).        self.r
+00005200: 6566 696c 6c5f 6472 6f70 646f 776e 2873  efill_dropdown(s
+00005210: 656c 662e 636f 6e74 6573 745f 6469 616c  elf.contest_dial
+00005220: 6f67 2e74 7261 6e73 6d69 7474 6572 2c20  og.transmitter, 
+00005230: 7661 6c75 6529 0a20 2020 2020 2020 2076  value).        v
+00005240: 616c 7565 203d 2073 656c 662e 636f 6e74  alue = self.cont
+00005250: 6573 745f 7365 7474 696e 6773 2e67 6574  est_settings.get
+00005260: 2822 5374 6172 7444 6174 6522 290a 2020  ("StartDate").  
+00005270: 2020 2020 2020 7468 655f 6461 7465 2c20        the_date, 
+00005280: 7468 655f 7469 6d65 203d 2076 616c 7565  the_time = value
+00005290: 2e73 706c 6974 2829 0a20 2020 2020 2020  .split().       
+000052a0: 2073 656c 662e 636f 6e74 6573 745f 6469   self.contest_di
+000052b0: 616c 6f67 2e64 6174 6554 696d 6545 6469  alog.dateTimeEdi
+000052c0: 742e 7365 7444 6174 6528 0a20 2020 2020  t.setDate(.     
+000052d0: 2020 2020 2020 2051 7443 6f72 652e 5144         QtCore.QD
+000052e0: 6174 652e 6672 6f6d 5374 7269 6e67 2874  ate.fromString(t
+000052f0: 6865 5f64 6174 652c 2022 7979 7979 2d4d  he_date, "yyyy-M
+00005300: 4d2d 6464 2229 0a20 2020 2020 2020 2029  M-dd").        )
+00005310: 0a20 2020 2020 2020 2073 656c 662e 636f  .        self.co
+00005320: 6e74 6573 745f 6469 616c 6f67 2e64 6174  ntest_dialog.dat
+00005330: 6554 696d 6545 6469 742e 7365 7443 616c  eTimeEdit.setCal
+00005340: 656e 6461 7250 6f70 7570 2854 7275 6529  endarPopup(True)
+00005350: 0a20 2020 2020 2020 2073 656c 662e 636f  .        self.co
+00005360: 6e74 6573 745f 6469 616c 6f67 2e64 6174  ntest_dialog.dat
+00005370: 6554 696d 6545 6469 742e 7365 7454 696d  eTimeEdit.setTim
+00005380: 6528 0a20 2020 2020 2020 2020 2020 2051  e(.            Q
+00005390: 7443 6f72 652e 5154 696d 652e 6672 6f6d  tCore.QTime.from
+000053a0: 5374 7269 6e67 2874 6865 5f74 696d 652c  String(the_time,
+000053b0: 2022 6868 3a6d 6d3a 7373 2229 0a20 2020   "hh:mm:ss").   
+000053c0: 2020 2020 2029 0a20 2020 2020 2020 2073       ).        s
+000053d0: 656c 662e 636f 6e74 6573 745f 6469 616c  elf.contest_dial
+000053e0: 6f67 2e6f 7065 6e28 290a 0a20 2020 2064  og.open()..    d
+000053f0: 6566 2073 6176 655f 6564 6974 6564 5f63  ef save_edited_c
+00005400: 6f6e 7465 7374 2873 656c 6629 3a0a 2020  ontest(self):.  
+00005410: 2020 2020 2020 2222 2253 6176 6520 7468        """Save th
+00005420: 6520 6564 6974 6564 2063 6f6e 7465 7374  e edited contest
+00005430: 2222 220a 2020 2020 2020 2020 636f 6e74  """.        cont
+00005440: 6573 7420 3d20 7b7d 0a20 2020 2020 2020  est = {}.       
+00005450: 2063 6f6e 7465 7374 5b22 436f 6e74 6573   contest["Contes
+00005460: 744e 616d 6522 5d20 3d20 280a 2020 2020  tName"] = (.    
+00005470: 2020 2020 2020 2020 7365 6c66 2e63 6f6e          self.con
+00005480: 7465 7374 5f64 6961 6c6f 672e 636f 6e74  test_dialog.cont
+00005490: 6573 742e 6375 7272 656e 7454 6578 7428  est.currentText(
+000054a0: 292e 6c6f 7765 7228 292e 7265 706c 6163  ).lower().replac
+000054b0: 6528 2220 222c 2022 5f22 290a 2020 2020  e(" ", "_").    
+000054c0: 2020 2020 290a 2020 2020 2020 2020 636f      ).        co
+000054d0: 6e74 6573 745b 2253 7461 7274 4461 7465  ntest["StartDate
+000054e0: 225d 203d 2073 656c 662e 636f 6e74 6573  "] = self.contes
+000054f0: 745f 6469 616c 6f67 2e64 6174 6554 696d  t_dialog.dateTim
+00005500: 6545 6469 742e 6461 7465 5469 6d65 2829  eEdit.dateTime()
+00005510: 2e74 6f53 7472 696e 6728 0a20 2020 2020  .toString(.     
+00005520: 2020 2020 2020 2022 7979 7979 2d4d 4d2d         "yyyy-MM-
+00005530: 6464 2068 683a 6d6d 3a73 7322 0a20 2020  dd hh:mm:ss".   
+00005540: 2020 2020 2029 0a20 2020 2020 2020 2063       ).        c
+00005550: 6f6e 7465 7374 5b22 4f70 6572 6174 6f72  ontest["Operator
+00005560: 4361 7465 676f 7279 225d 203d 2073 656c  Category"] = sel
+00005570: 662e 636f 6e74 6573 745f 6469 616c 6f67  f.contest_dialog
+00005580: 2e6f 7065 7261 746f 725f 636c 6173 732e  .operator_class.
+00005590: 6375 7272 656e 7454 6578 7428 290a 2020  currentText().  
+000055a0: 2020 2020 2020 636f 6e74 6573 745b 2242        contest["B
+000055b0: 616e 6443 6174 6567 6f72 7922 5d20 3d20  andCategory"] = 
+000055c0: 7365 6c66 2e63 6f6e 7465 7374 5f64 6961  self.contest_dia
+000055d0: 6c6f 672e 6261 6e64 2e63 7572 7265 6e74  log.band.current
+000055e0: 5465 7874 2829 0a20 2020 2020 2020 2063  Text().        c
+000055f0: 6f6e 7465 7374 5b22 506f 7765 7243 6174  ontest["PowerCat
+00005600: 6567 6f72 7922 5d20 3d20 7365 6c66 2e63  egory"] = self.c
+00005610: 6f6e 7465 7374 5f64 6961 6c6f 672e 706f  ontest_dialog.po
+00005620: 7765 722e 6375 7272 656e 7454 6578 7428  wer.currentText(
+00005630: 290a 2020 2020 2020 2020 636f 6e74 6573  ).        contes
+00005640: 745b 224d 6f64 6543 6174 6567 6f72 7922  t["ModeCategory"
+00005650: 5d20 3d20 7365 6c66 2e63 6f6e 7465 7374  ] = self.contest
+00005660: 5f64 6961 6c6f 672e 6d6f 6465 2e63 7572  _dialog.mode.cur
+00005670: 7265 6e74 5465 7874 2829 0a20 2020 2020  rentText().     
+00005680: 2020 2063 6f6e 7465 7374 5b22 4f76 6572     contest["Over
+00005690: 6c61 7943 6174 6567 6f72 7922 5d20 3d20  layCategory"] = 
+000056a0: 7365 6c66 2e63 6f6e 7465 7374 5f64 6961  self.contest_dia
+000056b0: 6c6f 672e 6f76 6572 6c61 792e 6375 7272  log.overlay.curr
+000056c0: 656e 7454 6578 7428 290a 2020 2020 2020  entText().      
+000056d0: 2020 636f 6e74 6573 745b 224f 7065 7261    contest["Opera
+000056e0: 746f 7273 225d 203d 2073 656c 662e 636f  tors"] = self.co
+000056f0: 6e74 6573 745f 6469 616c 6f67 2e6f 7065  ntest_dialog.ope
+00005700: 7261 746f 7273 2e74 6578 7428 290a 2020  rators.text().  
+00005710: 2020 2020 2020 636f 6e74 6573 745b 2253        contest["S
+00005720: 6f61 7062 6f78 225d 203d 2073 656c 662e  oapbox"] = self.
+00005730: 636f 6e74 6573 745f 6469 616c 6f67 2e73  contest_dialog.s
+00005740: 6f61 7062 6f78 2e74 6f50 6c61 696e 5465  oapbox.toPlainTe
+00005750: 7874 2829 0a20 2020 2020 2020 2063 6f6e  xt().        con
+00005760: 7465 7374 5b22 5365 6e74 4578 6368 616e  test["SentExchan
+00005770: 6765 225d 203d 2073 656c 662e 636f 6e74  ge"] = self.cont
+00005780: 6573 745f 6469 616c 6f67 2e65 7863 6861  est_dialog.excha
+00005790: 6e67 652e 7465 7874 2829 0a20 2020 2020  nge.text().     
+000057a0: 2020 2063 6f6e 7465 7374 5b22 436f 6e74     contest["Cont
+000057b0: 6573 744e 5222 5d20 3d20 7365 6c66 2e70  estNR"] = self.p
+000057c0: 7265 662e 6765 7428 2263 6f6e 7465 7374  ref.get("contest
+000057d0: 222c 2031 290a 2020 2020 2020 2020 636f  ", 1).        co
+000057e0: 6e74 6573 745b 2253 7461 7469 6f6e 4361  ntest["StationCa
+000057f0: 7465 676f 7279 225d 203d 2073 656c 662e  tegory"] = self.
+00005800: 636f 6e74 6573 745f 6469 616c 6f67 2e73  contest_dialog.s
+00005810: 7461 7469 6f6e 2e63 7572 7265 6e74 5465  tation.currentTe
+00005820: 7874 2829 0a20 2020 2020 2020 2063 6f6e  xt().        con
+00005830: 7465 7374 5b22 4173 7369 7374 6564 4361  test["AssistedCa
+00005840: 7465 676f 7279 225d 203d 2073 656c 662e  tegory"] = self.
+00005850: 636f 6e74 6573 745f 6469 616c 6f67 2e61  contest_dialog.a
+00005860: 7373 6973 7465 642e 6375 7272 656e 7454  ssisted.currentT
+00005870: 6578 7428 290a 2020 2020 2020 2020 636f  ext().        co
+00005880: 6e74 6573 745b 2254 7261 6e73 6d69 7474  ntest["Transmitt
+00005890: 6572 4361 7465 676f 7279 225d 203d 2073  erCategory"] = s
+000058a0: 656c 662e 636f 6e74 6573 745f 6469 616c  elf.contest_dial
+000058b0: 6f67 2e74 7261 6e73 6d69 7474 6572 2e63  og.transmitter.c
+000058c0: 7572 7265 6e74 5465 7874 2829 0a0a 2020  urrentText()..  
+000058d0: 2020 2020 2020 6c6f 6767 6572 2e64 6562        logger.deb
+000058e0: 7567 2822 2573 222c 2066 227b 636f 6e74  ug("%s", f"{cont
+000058f0: 6573 747d 2229 0a20 2020 2020 2020 2073  est}").        s
+00005900: 656c 662e 6461 7461 6261 7365 2e75 7064  elf.database.upd
+00005910: 6174 655f 636f 6e74 6573 7428 636f 6e74  ate_contest(cont
+00005920: 6573 7429 0a20 2020 2020 2020 2073 656c  est).        sel
+00005930: 662e 7772 6974 655f 7072 6566 6572 656e  f.write_preferen
+00005940: 6365 2829 0a20 2020 2020 2020 2073 656c  ce().        sel
+00005950: 662e 6c6f 6164 5f63 6f6e 7465 7374 2829  f.load_contest()
+00005960: 0a0a 2020 2020 6465 6620 6c6f 6164 5f63  ..    def load_c
+00005970: 6f6e 7465 7374 2873 656c 6629 3a0a 2020  ontest(self):.  
+00005980: 2020 2020 2020 2222 226c 6f61 6420 6120        """load a 
+00005990: 636f 6e74 6573 7422 2222 0a20 2020 2020  contest""".     
+000059a0: 2020 2069 6620 7365 6c66 2e70 7265 662e     if self.pref.
+000059b0: 6765 7428 2263 6f6e 7465 7374 2229 3a0a  get("contest"):.
+000059c0: 2020 2020 2020 2020 2020 2020 7365 6c66              self
+000059d0: 2e63 6f6e 7465 7374 5f73 6574 7469 6e67  .contest_setting
+000059e0: 7320 3d20 7365 6c66 2e64 6174 6162 6173  s = self.databas
+000059f0: 652e 6665 7463 685f 636f 6e74 6573 745f  e.fetch_contest_
+00005a00: 6279 5f69 6428 0a20 2020 2020 2020 2020  by_id(.         
+00005a10: 2020 2020 2020 2073 656c 662e 7072 6566         self.pref
+00005a20: 2e67 6574 2822 636f 6e74 6573 7422 290a  .get("contest").
+00005a30: 2020 2020 2020 2020 2020 2020 290a 2020              ).  
+00005a40: 2020 2020 2020 2020 2020 6966 2073 656c            if sel
+00005a50: 662e 636f 6e74 6573 745f 7365 7474 696e  f.contest_settin
+00005a60: 6773 3a0a 2020 2020 2020 2020 2020 2020  gs:.            
+00005a70: 2020 2020 7365 6c66 2e64 6174 6162 6173      self.databas
+00005a80: 652e 6375 7272 656e 745f 636f 6e74 6573  e.current_contes
+00005a90: 7420 3d20 7365 6c66 2e70 7265 662e 6765  t = self.pref.ge
+00005aa0: 7428 2263 6f6e 7465 7374 2229 0a20 2020  t("contest").   
+00005ab0: 2020 2020 2020 2020 2020 2020 2069 6620               if 
+00005ac0: 7365 6c66 2e63 6f6e 7465 7374 5f73 6574  self.contest_set
+00005ad0: 7469 6e67 732e 6765 7428 2243 6f6e 7465  tings.get("Conte
+00005ae0: 7374 4e61 6d65 2229 3a0a 2020 2020 2020  stName"):.      
+00005af0: 2020 2020 2020 2020 2020 2020 2020 7365                se
+00005b00: 6c66 2e63 6f6e 7465 7374 203d 2064 6f69  lf.contest = doi
+00005b10: 6d70 2873 656c 662e 636f 6e74 6573 745f  mp(self.contest_
+00005b20: 7365 7474 696e 6773 2e67 6574 2822 436f  settings.get("Co
+00005b30: 6e74 6573 744e 616d 6522 2929 0a20 2020  ntestName")).   
 00005b40: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00005b50: 6c6f 6767 6572 2e64 6562 7567 2822 4c6f  logger.debug("Lo
-00005b60: 6164 6564 2043 6f6e 7465 7374 204e 616d  aded Contest Nam
-00005b70: 6520 3d20 2573 222c 2073 656c 662e 636f  e = %s", self.co
-00005b80: 6e74 6573 742e 6e61 6d65 290a 2020 2020  ntest.name).    
+00005b50: 206c 6f67 6765 722e 6465 6275 6728 224c   logger.debug("L
+00005b60: 6f61 6465 6420 436f 6e74 6573 7420 4e61  oaded Contest Na
+00005b70: 6d65 203d 2025 7322 2c20 7365 6c66 2e63  me = %s", self.c
+00005b80: 6f6e 7465 7374 2e6e 616d 6529 0a20 2020  ontest.name).   
 00005b90: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00005ba0: 7365 6c66 2e73 6574 5f77 696e 646f 775f  self.set_window_
-00005bb0: 7469 746c 6528 290a 2020 2020 2020 2020  title().        
-00005bc0: 2020 2020 2020 2020 2020 2020 7365 6c66              self
-00005bd0: 2e63 6f6e 7465 7374 2e69 6e69 745f 636f  .contest.init_co
-00005be0: 6e74 6573 7428 7365 6c66 290a 2020 2020  ntest(self).    
+00005ba0: 2073 656c 662e 7365 745f 7769 6e64 6f77   self.set_window
+00005bb0: 5f74 6974 6c65 2829 0a20 2020 2020 2020  _title().       
+00005bc0: 2020 2020 2020 2020 2020 2020 2073 656c               sel
+00005bd0: 662e 636f 6e74 6573 742e 696e 6974 5f63  f.contest.init_c
+00005be0: 6f6e 7465 7374 2873 656c 6629 0a20 2020  ontest(self).   
 00005bf0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00005c00: 7365 6c66 2e68 6964 655f 6261 6e64 5f6d  self.hide_band_m
-00005c10: 6f64 6528 7365 6c66 2e63 6f6e 7465 7374  ode(self.contest
-00005c20: 5f73 6574 7469 6e67 732e 6765 7428 224d  _settings.get("M
-00005c30: 6f64 6543 6174 6567 6f72 7922 2c20 2222  odeCategory", ""
-00005c40: 2929 0a0a 2020 2020 2020 2020 2020 2020  ))..            
-00005c50: 2020 2020 6966 2068 6173 6174 7472 2873      if hasattr(s
-00005c60: 656c 662e 636f 6e74 6573 742c 2022 6d6f  elf.contest, "mo
-00005c70: 6465 2229 3a0a 2020 2020 2020 2020 2020  de"):.          
-00005c80: 2020 2020 2020 2020 2020 6966 2073 656c            if sel
-00005c90: 662e 636f 6e74 6573 742e 6d6f 6465 2069  f.contest.mode i
-00005ca0: 6e20 5b22 4357 222c 2022 424f 5448 225d  n ["CW", "BOTH"]
-00005cb0: 3a0a 2020 2020 2020 2020 2020 2020 2020  :.              
-00005cc0: 2020 2020 2020 2020 2020 7365 6c66 2e63            self.c
-00005cd0: 775f 7370 6565 642e 7368 6f77 2829 0a20  w_speed.show(). 
+00005c00: 2073 656c 662e 6869 6465 5f62 616e 645f   self.hide_band_
+00005c10: 6d6f 6465 2873 656c 662e 636f 6e74 6573  mode(self.contes
+00005c20: 745f 7365 7474 696e 6773 2e67 6574 2822  t_settings.get("
+00005c30: 4d6f 6465 4361 7465 676f 7279 222c 2022  ModeCategory", "
+00005c40: 2229 290a 0a20 2020 2020 2020 2020 2020  "))..           
+00005c50: 2020 2020 2069 6620 6861 7361 7474 7228       if hasattr(
+00005c60: 7365 6c66 2e63 6f6e 7465 7374 2c20 226d  self.contest, "m
+00005c70: 6f64 6522 293a 0a20 2020 2020 2020 2020  ode"):.         
+00005c80: 2020 2020 2020 2020 2020 2069 6620 7365             if se
+00005c90: 6c66 2e63 6f6e 7465 7374 2e6d 6f64 6520  lf.contest.mode 
+00005ca0: 696e 205b 2243 5722 2c20 2242 4f54 4822  in ["CW", "BOTH"
+00005cb0: 5d3a 0a20 2020 2020 2020 2020 2020 2020  ]:.             
+00005cc0: 2020 2020 2020 2020 2020 2073 656c 662e             self.
+00005cd0: 6377 5f73 7065 6564 2e73 686f 7728 290a  cw_speed.show().
 00005ce0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00005cf0: 2020 2065 6c73 653a 0a20 2020 2020 2020     else:.       
+00005cf0: 2020 2020 656c 7365 3a0a 2020 2020 2020      else:.      
 00005d00: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00005d10: 2073 656c 662e 6377 5f73 7065 6564 2e68   self.cw_speed.h
-00005d20: 6964 6528 290a 0a20 2020 2020 2020 2020  ide()..         
-00005d30: 2020 2020 2020 2063 6d64 203d 207b 7d0a         cmd = {}.
-00005d40: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00005d50: 636d 645b 2263 6d64 225d 203d 2022 4e45  cmd["cmd"] = "NE
-00005d60: 5744 4222 0a20 2020 2020 2020 2020 2020  WDB".           
-00005d70: 2020 2020 2063 6d64 5b22 7374 6174 696f       cmd["statio
-00005d80: 6e22 5d20 3d20 706c 6174 666f 726d 2e6e  n"] = platform.n
-00005d90: 6f64 6528 290a 2020 2020 2020 2020 2020  ode().          
-00005da0: 2020 2020 2020 7365 6c66 2e6d 756c 7469        self.multi
-00005db0: 6361 7374 5f69 6e74 6572 6661 6365 2e73  cast_interface.s
-00005dc0: 656e 645f 6173 5f6a 736f 6e28 636d 6429  end_as_json(cmd)
-00005dd0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00005de0: 2069 6620 6861 7361 7474 7228 7365 6c66   if hasattr(self
-00005df0: 2e63 6f6e 7465 7374 2c20 2263 6f6c 756d  .contest, "colum
-00005e00: 6e73 2229 3a0a 2020 2020 2020 2020 2020  ns"):.          
-00005e10: 2020 2020 2020 2020 2020 636d 6420 3d20            cmd = 
-00005e20: 7b7d 0a20 2020 2020 2020 2020 2020 2020  {}.             
-00005e30: 2020 2020 2020 2063 6d64 5b22 636d 6422         cmd["cmd"
-00005e40: 5d20 3d20 2253 484f 5743 4f4c 554d 4e53  ] = "SHOWCOLUMNS
-00005e50: 220a 2020 2020 2020 2020 2020 2020 2020  ".              
-00005e60: 2020 2020 2020 636d 645b 2273 7461 7469        cmd["stati
-00005e70: 6f6e 225d 203d 2070 6c61 7466 6f72 6d2e  on"] = platform.
-00005e80: 6e6f 6465 2829 0a20 2020 2020 2020 2020  node().         
-00005e90: 2020 2020 2020 2020 2020 2063 6d64 5b22             cmd["
-00005ea0: 434f 4c55 4d4e 5322 5d20 3d20 7365 6c66  COLUMNS"] = self
-00005eb0: 2e63 6f6e 7465 7374 2e63 6f6c 756d 6e73  .contest.columns
-00005ec0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00005ed0: 2020 2020 2073 656c 662e 6d75 6c74 6963       self.multic
-00005ee0: 6173 745f 696e 7465 7266 6163 652e 7365  ast_interface.se
-00005ef0: 6e64 5f61 735f 6a73 6f6e 2863 6d64 290a  nd_as_json(cmd).
-00005f00: 0a20 2020 2064 6566 2068 6964 655f 6261  .    def hide_ba
-00005f10: 6e64 5f6d 6f64 6528 7365 6c66 2c20 7468  nd_mode(self, th
-00005f20: 655f 6d6f 6465 3a20 7374 7229 202d 3e20  e_mode: str) -> 
-00005f30: 4e6f 6e65 3a0a 2020 2020 2020 2020 2222  None:.        ""
-00005f40: 2268 6964 6522 2222 0a20 2020 2020 2020  "hide""".       
-00005f50: 206c 6f67 6765 722e 6465 6275 6728 2225   logger.debug("%
-00005f60: 7322 2c20 6622 7b74 6865 5f6d 6f64 657d  s", f"{the_mode}
-00005f70: 2229 0a20 2020 2020 2020 2073 656c 662e  ").        self.
-00005f80: 4261 6e64 5f4d 6f64 655f 4672 616d 655f  Band_Mode_Frame_
-00005f90: 4357 2e68 6964 6528 290a 2020 2020 2020  CW.hide().      
-00005fa0: 2020 7365 6c66 2e42 616e 645f 4d6f 6465    self.Band_Mode
-00005fb0: 5f46 7261 6d65 5f53 5342 2e68 6964 6528  _Frame_SSB.hide(
-00005fc0: 290a 2020 2020 2020 2020 7365 6c66 2e42  ).        self.B
-00005fd0: 616e 645f 4d6f 6465 5f46 7261 6d65 5f52  and_Mode_Frame_R
-00005fe0: 5454 592e 6869 6465 2829 0a20 2020 2020  TTY.hide().     
-00005ff0: 2020 206d 6f64 6573 203d 207b 0a20 2020     modes = {.   
-00006000: 2020 2020 2020 2020 2022 4357 223a 2028           "CW": (
-00006010: 7365 6c66 2e42 616e 645f 4d6f 6465 5f46  self.Band_Mode_F
-00006020: 7261 6d65 5f43 572c 292c 0a20 2020 2020  rame_CW,),.     
-00006030: 2020 2020 2020 2022 5353 4222 3a20 2873         "SSB": (s
-00006040: 656c 662e 4261 6e64 5f4d 6f64 655f 4672  elf.Band_Mode_Fr
-00006050: 616d 655f 5353 422c 292c 0a20 2020 2020  ame_SSB,),.     
-00006060: 2020 2020 2020 2022 5254 5459 223a 2028         "RTTY": (
-00006070: 7365 6c66 2e42 616e 645f 4d6f 6465 5f46  self.Band_Mode_F
-00006080: 7261 6d65 5f52 5454 592c 292c 0a20 2020  rame_RTTY,),.   
-00006090: 2020 2020 2020 2020 2022 5053 4b22 3a20           "PSK": 
-000060a0: 2873 656c 662e 4261 6e64 5f4d 6f64 655f  (self.Band_Mode_
-000060b0: 4672 616d 655f 5254 5459 2c29 2c0a 2020  Frame_RTTY,),.  
-000060c0: 2020 2020 2020 2020 2020 2253 5342 2b43            "SSB+C
-000060d0: 5722 3a20 2873 656c 662e 4261 6e64 5f4d  W": (self.Band_M
-000060e0: 6f64 655f 4672 616d 655f 4357 2c20 7365  ode_Frame_CW, se
-000060f0: 6c66 2e42 616e 645f 4d6f 6465 5f46 7261  lf.Band_Mode_Fra
-00006100: 6d65 5f53 5342 292c 0a20 2020 2020 2020  me_SSB),.       
-00006110: 2020 2020 2022 424f 5448 223a 2028 7365       "BOTH": (se
-00006120: 6c66 2e42 616e 645f 4d6f 6465 5f46 7261  lf.Band_Mode_Fra
-00006130: 6d65 5f43 572c 2073 656c 662e 4261 6e64  me_CW, self.Band
-00006140: 5f4d 6f64 655f 4672 616d 655f 5353 4229  _Mode_Frame_SSB)
-00006150: 2c0a 2020 2020 2020 2020 2020 2020 2244  ,.            "D
-00006160: 4947 4954 414c 223a 2028 7365 6c66 2e42  IGITAL": (self.B
-00006170: 616e 645f 4d6f 6465 5f46 7261 6d65 5f52  and_Mode_Frame_R
-00006180: 5454 592c 292c 0a20 2020 2020 2020 2020  TTY,),.         
-00006190: 2020 2022 5353 422b 4357 2b44 4947 4954     "SSB+CW+DIGIT
-000061a0: 414c 223a 2028 0a20 2020 2020 2020 2020  AL": (.         
-000061b0: 2020 2020 2020 2073 656c 662e 4261 6e64         self.Band
-000061c0: 5f4d 6f64 655f 4672 616d 655f 5254 5459  _Mode_Frame_RTTY
-000061d0: 2c0a 2020 2020 2020 2020 2020 2020 2020  ,.              
-000061e0: 2020 7365 6c66 2e42 616e 645f 4d6f 6465    self.Band_Mode
-000061f0: 5f46 7261 6d65 5f43 572c 0a20 2020 2020  _Frame_CW,.     
-00006200: 2020 2020 2020 2020 2020 2073 656c 662e             self.
-00006210: 4261 6e64 5f4d 6f64 655f 4672 616d 655f  Band_Mode_Frame_
-00006220: 5353 422c 0a20 2020 2020 2020 2020 2020  SSB,.           
-00006230: 2029 2c0a 2020 2020 2020 2020 2020 2020   ),.            
-00006240: 2246 4d22 3a20 2873 656c 662e 4261 6e64  "FM": (self.Band
-00006250: 5f4d 6f64 655f 4672 616d 655f 5353 422c  _Mode_Frame_SSB,
-00006260: 292c 0a20 2020 2020 2020 207d 0a20 2020  ),.        }.   
-00006270: 2020 2020 2066 7261 6d65 7320 3d20 6d6f       frames = mo
-00006280: 6465 732e 6765 7428 7468 655f 6d6f 6465  des.get(the_mode
-00006290: 290a 2020 2020 2020 2020 6966 2066 7261  ).        if fra
-000062a0: 6d65 733a 0a20 2020 2020 2020 2020 2020  mes:.           
-000062b0: 2066 6f72 2066 7261 6d65 2069 6e20 6672   for frame in fr
-000062c0: 616d 6573 3a0a 2020 2020 2020 2020 2020  ames:.          
-000062d0: 2020 2020 2020 6672 616d 652e 7368 6f77        frame.show
-000062e0: 2829 0a0a 2020 2020 6465 6620 6669 6c65  ()..    def file
-000062f0: 7069 636b 6572 2873 656c 662c 2061 6374  picker(self, act
-00006300: 696f 6e3a 2073 7472 2920 2d3e 2073 7472  ion: str) -> str
-00006310: 3a0a 2020 2020 2020 2020 2222 220a 2020  :.        """.  
-00006320: 2020 2020 2020 4765 7420 6120 6669 6c65        Get a file
-00006330: 6e61 6d65 0a20 2020 2020 2020 2061 6374  name.        act
-00006340: 696f 6e3a 2022 6e65 7722 206f 7220 226f  ion: "new" or "o
-00006350: 7065 6e22 0a20 2020 2020 2020 2022 2222  pen".        """
-00006360: 0a20 2020 2020 2020 206f 7074 696f 6e73  .        options
-00006370: 203d 2051 4669 6c65 4469 616c 6f67 2e4f   = QFileDialog.O
-00006380: 7074 696f 6e73 2829 0a20 2020 2020 2020  ptions().       
-00006390: 206f 7074 696f 6e73 207c 3d20 5146 696c   options |= QFil
-000063a0: 6544 6961 6c6f 672e 446f 6e74 5573 654e  eDialog.DontUseN
-000063b0: 6174 6976 6544 6961 6c6f 670a 2020 2020  ativeDialog.    
-000063c0: 2020 2020 6f70 7469 6f6e 7320 7c3d 2051      options |= Q
-000063d0: 4669 6c65 4469 616c 6f67 2e44 6f6e 7443  FileDialog.DontC
-000063e0: 6f6e 6669 726d 4f76 6572 7772 6974 650a  onfirmOverwrite.
-000063f0: 2020 2020 2020 2020 2320 7069 636b 6572          # picker
-00006400: 203d 2051 4669 6c65 4469 616c 6f67 2873   = QFileDialog(s
-00006410: 656c 6629 0a20 2020 2020 2020 2069 6620  elf).        if 
-00006420: 6163 7469 6f6e 203d 3d20 226e 6577 223a  action == "new":
-00006430: 0a20 2020 2020 2020 2020 2020 2066 696c  .            fil
-00006440: 652c 205f 203d 2051 4669 6c65 4469 616c  e, _ = QFileDial
-00006450: 6f67 2e67 6574 5361 7665 4669 6c65 4e61  og.getSaveFileNa
-00006460: 6d65 280a 2020 2020 2020 2020 2020 2020  me(.            
-00006470: 2020 2020 7365 6c66 2c0a 2020 2020 2020      self,.      
-00006480: 2020 2020 2020 2020 2020 2243 686f 6f73            "Choos
-00006490: 6520 6120 4461 7461 6261 7365 222c 0a20  e a Database",. 
-000064a0: 2020 2020 2020 2020 2020 2020 2020 2044                 D
-000064b0: 4154 415f 5041 5448 2c0a 2020 2020 2020  ATA_PATH,.      
-000064c0: 2020 2020 2020 2020 2020 2244 6174 6162            "Datab
-000064d0: 6173 6520 282a 2e64 6229 222c 0a20 2020  ase (*.db)",.   
-000064e0: 2020 2020 2020 2020 2020 2020 206f 7074               opt
-000064f0: 696f 6e73 3d6f 7074 696f 6e73 2c0a 2020  ions=options,.  
-00006500: 2020 2020 2020 2020 2020 290a 2020 2020            ).    
-00006510: 2020 2020 6966 2061 6374 696f 6e20 3d3d      if action ==
-00006520: 2022 6f70 656e 223a 0a20 2020 2020 2020   "open":.       
-00006530: 2020 2020 2066 696c 652c 205f 203d 2051       file, _ = Q
-00006540: 4669 6c65 4469 616c 6f67 2e67 6574 4f70  FileDialog.getOp
-00006550: 656e 4669 6c65 4e61 6d65 280a 2020 2020  enFileName(.    
-00006560: 2020 2020 2020 2020 2020 2020 7365 6c66              self
-00006570: 2c0a 2020 2020 2020 2020 2020 2020 2020  ,.              
-00006580: 2020 2243 686f 6f73 6520 6120 4461 7461    "Choose a Data
-00006590: 6261 7365 222c 0a20 2020 2020 2020 2020  base",.         
-000065a0: 2020 2020 2020 2044 4154 415f 5041 5448         DATA_PATH
-000065b0: 2c0a 2020 2020 2020 2020 2020 2020 2020  ,.              
-000065c0: 2020 2244 6174 6162 6173 6520 282a 2e64    "Database (*.d
-000065d0: 6229 222c 0a20 2020 2020 2020 2020 2020  b)",.           
-000065e0: 2020 2020 206f 7074 696f 6e73 3d6f 7074       options=opt
-000065f0: 696f 6e73 2c0a 2020 2020 2020 2020 2020  ions,.          
-00006600: 2020 290a 2020 2020 2020 2020 7265 7475    ).        retu
-00006610: 726e 2066 696c 650a 0a20 2020 2064 6566  rn file..    def
-00006620: 2072 6563 616c 6375 6c61 7465 5f6d 756c   recalculate_mul
-00006630: 7473 2873 656c 6629 3a0a 2020 2020 2020  ts(self):.      
-00006640: 2020 2222 2252 6563 616c 6375 6c61 7465    """Recalculate
-00006650: 204d 756c 7469 706c 6965 7273 2222 220a   Multipliers""".
-00006660: 2020 2020 2020 2020 7365 6c66 2e63 6f6e          self.con
-00006670: 7465 7374 2e72 6563 616c 6375 6c61 7465  test.recalculate
-00006680: 5f6d 756c 7473 2873 656c 6629 0a0a 2020  _mults(self)..  
-00006690: 2020 6465 6620 6c61 756e 6368 5f6c 6f67    def launch_log
-000066a0: 5f77 696e 646f 7728 7365 6c66 293a 0a20  _window(self):. 
-000066b0: 2020 2020 2020 2022 2222 6c61 756e 6368         """launch
-000066c0: 2074 6865 204c 6f67 2057 696e 646f 7722   the Log Window"
-000066d0: 2222 0a20 2020 2020 2020 2069 6620 6e6f  "".        if no
-000066e0: 7420 6368 6563 6b5f 7072 6f63 6573 7328  t check_process(
-000066f0: 226c 6f67 7769 6e64 6f77 2e70 7922 293a  "logwindow.py"):
-00006700: 0a20 2020 2020 2020 2020 2020 205f 203d  .            _ =
-00006710: 2073 7562 7072 6f63 6573 732e 506f 7065   subprocess.Pope
-00006720: 6e28 5b73 7973 2e65 7865 6375 7461 626c  n([sys.executabl
-00006730: 652c 2057 4f52 4b49 4e47 5f50 4154 4820  e, WORKING_PATH 
-00006740: 2b20 222f 6c6f 6777 696e 646f 772e 7079  + "/logwindow.py
-00006750: 225d 290a 0a20 2020 2064 6566 206c 6175  "])..    def lau
-00006760: 6e63 685f 6261 6e64 6d61 705f 7769 6e64  nch_bandmap_wind
-00006770: 6f77 2873 656c 6629 3a0a 2020 2020 2020  ow(self):.      
-00006780: 2020 2222 226c 6175 6e63 6820 7468 6520    """launch the 
-00006790: 4c6f 6720 5769 6e64 6f77 2222 220a 2020  Log Window""".  
-000067a0: 2020 2020 2020 6966 206e 6f74 2063 6865        if not che
-000067b0: 636b 5f70 726f 6365 7373 2822 6261 6e64  ck_process("band
-000067c0: 6d61 702e 7079 2229 3a0a 2020 2020 2020  map.py"):.      
-000067d0: 2020 2020 2020 5f20 3d20 7375 6270 726f        _ = subpro
-000067e0: 6365 7373 2e50 6f70 656e 285b 7379 732e  cess.Popen([sys.
-000067f0: 6578 6563 7574 6162 6c65 2c20 574f 524b  executable, WORK
-00006800: 494e 475f 5041 5448 202b 2022 2f62 616e  ING_PATH + "/ban
-00006810: 646d 6170 2e70 7922 5d29 0a0a 2020 2020  dmap.py"])..    
-00006820: 6465 6620 636c 6561 725f 6261 6e64 5f69  def clear_band_i
-00006830: 6e64 6963 6174 6f72 7328 7365 6c66 293a  ndicators(self):
-00006840: 0a20 2020 2020 2020 2022 2222 436c 6561  .        """Clea
-00006850: 7220 7468 6520 696e 6469 6361 746f 7273  r the indicators
-00006860: 2222 220a 2020 2020 2020 2020 666f 7220  """.        for 
-00006870: 5f2c 2069 6e64 6963 6174 6f72 7320 696e  _, indicators in
-00006880: 2073 656c 662e 616c 6c5f 6d6f 6465 5f69   self.all_mode_i
-00006890: 6e64 6963 6174 6f72 732e 6974 656d 7328  ndicators.items(
-000068a0: 293a 0a20 2020 2020 2020 2020 2020 2066  ):.            f
-000068b0: 6f72 205f 2c20 696e 6469 6361 746f 7220  or _, indicator 
-000068c0: 696e 2069 6e64 6963 6174 6f72 732e 6974  in indicators.it
-000068d0: 656d 7328 293a 0a20 2020 2020 2020 2020  ems():.         
-000068e0: 2020 2020 2020 2069 6e64 6963 6174 6f72         indicator
-000068f0: 2e73 6574 4672 616d 6553 6861 7065 2851  .setFrameShape(Q
-00006900: 7457 6964 6765 7473 2e51 4672 616d 652e  tWidgets.QFrame.
-00006910: 4e6f 4672 616d 6529 0a0a 2020 2020 6465  NoFrame)..    de
-00006920: 6620 7365 745f 6261 6e64 5f69 6e64 6963  f set_band_indic
-00006930: 6174 6f72 2873 656c 662c 2062 616e 643a  ator(self, band:
-00006940: 2073 7472 2920 2d3e 204e 6f6e 653a 0a20   str) -> None:. 
-00006950: 2020 2020 2020 2022 2222 5365 7420 7468         """Set th
-00006960: 6520 6261 6e64 2069 6e64 6963 6174 6f72  e band indicator
-00006970: 2222 220a 2020 2020 2020 2020 6c6f 6767  """.        logg
-00006980: 6572 2e64 6562 7567 2822 2573 222c 2066  er.debug("%s", f
-00006990: 2262 616e 643a 7b62 616e 647d 206d 6f64  "band:{band} mod
-000069a0: 653a 207b 7365 6c66 2e63 7572 7265 6e74  e: {self.current
-000069b0: 5f6d 6f64 657d 2229 0a20 2020 2020 2020  _mode}").       
-000069c0: 2069 6620 6261 6e64 2061 6e64 2073 656c   if band and sel
-000069d0: 662e 6375 7272 656e 745f 6d6f 6465 3a0a  f.current_mode:.
-000069e0: 2020 2020 2020 2020 2020 2020 7365 6c66              self
-000069f0: 2e63 6c65 6172 5f62 616e 645f 696e 6469  .clear_band_indi
-00006a00: 6361 746f 7273 2829 0a20 2020 2020 2020  cators().       
-00006a10: 2020 2020 2069 6e64 6963 6174 6f72 203d       indicator =
-00006a20: 2073 656c 662e 616c 6c5f 6d6f 6465 5f69   self.all_mode_i
-00006a30: 6e64 6963 6174 6f72 735b 7365 6c66 2e63  ndicators[self.c
-00006a40: 7572 7265 6e74 5f6d 6f64 655d 2e67 6574  urrent_mode].get
-00006a50: 2862 616e 642c 204e 6f6e 6529 0a20 2020  (band, None).   
-00006a60: 2020 2020 2020 2020 2069 6620 696e 6469           if indi
-00006a70: 6361 746f 723a 0a20 2020 2020 2020 2020  cator:.         
-00006a80: 2020 2020 2020 2069 6e64 6963 6174 6f72         indicator
-00006a90: 2e73 6574 4672 616d 6553 6861 7065 2851  .setFrameShape(Q
-00006aa0: 7457 6964 6765 7473 2e51 4672 616d 652e  tWidgets.QFrame.
-00006ab0: 426f 7829 0a0a 2020 2020 6465 6620 636c  Box)..    def cl
-00006ac0: 6f73 6545 7665 6e74 2873 656c 662c 205f  oseEvent(self, _
-00006ad0: 6576 656e 7429 3a0a 2020 2020 2020 2020  event):.        
-00006ae0: 2222 220a 2020 2020 2020 2020 5772 6974  """.        Writ
-00006af0: 6520 7769 6e64 6f77 2073 697a 6520 616e  e window size an
-00006b00: 6420 706f 7369 7469 6f6e 2074 6f20 636f  d position to co
-00006b10: 6e66 6967 2066 696c 650a 2020 2020 2020  nfig file.      
-00006b20: 2020 2222 220a 2020 2020 2020 2020 7365    """.        se
-00006b30: 6c66 2e70 7265 665b 2277 696e 646f 775f  lf.pref["window_
-00006b40: 7769 6474 6822 5d20 3d20 7365 6c66 2e73  width"] = self.s
-00006b50: 697a 6528 292e 7769 6474 6828 290a 2020  ize().width().  
-00006b60: 2020 2020 2020 7365 6c66 2e70 7265 665b        self.pref[
-00006b70: 2277 696e 646f 775f 6865 6967 6874 225d  "window_height"]
-00006b80: 203d 2073 656c 662e 7369 7a65 2829 2e68   = self.size().h
-00006b90: 6569 6768 7428 290a 2020 2020 2020 2020  eight().        
-00006ba0: 7365 6c66 2e70 7265 665b 2277 696e 646f  self.pref["windo
-00006bb0: 775f 7822 5d20 3d20 7365 6c66 2e70 6f73  w_x"] = self.pos
-00006bc0: 2829 2e78 2829 0a20 2020 2020 2020 2073  ().x().        s
-00006bd0: 656c 662e 7072 6566 5b22 7769 6e64 6f77  elf.pref["window
-00006be0: 5f79 225d 203d 2073 656c 662e 706f 7328  _y"] = self.pos(
-00006bf0: 292e 7928 290a 2020 2020 2020 2020 7365  ).y().        se
-00006c00: 6c66 2e77 7269 7465 5f70 7265 6665 7265  lf.write_prefere
-00006c10: 6e63 6528 290a 0a20 2020 2064 6566 2063  nce()..    def c
-00006c20: 7479 5f6c 6f6f 6b75 7028 7365 6c66 2c20  ty_lookup(self, 
-00006c30: 6361 6c6c 7369 676e 3a20 7374 7229 3a0a  callsign: str):.
-00006c40: 2020 2020 2020 2020 2222 224c 6f6f 6b75          """Looku
-00006c50: 7020 6361 6c6c 7369 676e 2069 6e20 6374  p callsign in ct
-00006c60: 792e 6461 7420 6669 6c65 2222 220a 2020  y.dat file""".  
-00006c70: 2020 2020 2020 6361 6c6c 7369 676e 203d        callsign =
-00006c80: 2063 616c 6c73 6967 6e2e 7570 7065 7228   callsign.upper(
-00006c90: 290a 2020 2020 2020 2020 666f 7220 636f  ).        for co
-00006ca0: 756e 7420 696e 2072 6576 6572 7365 6428  unt in reversed(
-00006cb0: 7261 6e67 6528 6c65 6e28 6361 6c6c 7369  range(len(callsi
-00006cc0: 676e 2929 293a 0a20 2020 2020 2020 2020  gn))):.         
-00006cd0: 2020 2073 6561 7263 6869 7465 6d20 3d20     searchitem = 
-00006ce0: 6361 6c6c 7369 676e 5b3a 2063 6f75 6e74  callsign[: count
-00006cf0: 202b 2031 5d0a 2020 2020 2020 2020 2020   + 1].          
-00006d00: 2020 7265 7375 6c74 203d 207b 6b65 793a    result = {key:
-00006d10: 2076 616c 2066 6f72 206b 6579 2c20 7661   val for key, va
-00006d20: 6c20 696e 2043 5459 4649 4c45 2e69 7465  l in CTYFILE.ite
-00006d30: 6d73 2829 2069 6620 6b65 7920 3d3d 2073  ms() if key == s
-00006d40: 6561 7263 6869 7465 6d7d 0a20 2020 2020  earchitem}.     
-00006d50: 2020 2020 2020 2069 6620 6e6f 7420 7265         if not re
-00006d60: 7375 6c74 3a0a 2020 2020 2020 2020 2020  sult:.          
-00006d70: 2020 2020 2020 636f 6e74 696e 7565 0a20        continue. 
-00006d80: 2020 2020 2020 2020 2020 2069 6620 7265             if re
-00006d90: 7375 6c74 2e67 6574 2873 6561 7263 6869  sult.get(searchi
-00006da0: 7465 6d29 2e67 6574 2822 6578 6163 745f  tem).get("exact_
-00006db0: 6d61 7463 6822 293a 0a20 2020 2020 2020  match"):.       
-00006dc0: 2020 2020 2020 2020 2069 6620 7365 6172           if sear
-00006dd0: 6368 6974 656d 203d 3d20 6361 6c6c 7369  chitem == callsi
-00006de0: 676e 3a0a 2020 2020 2020 2020 2020 2020  gn:.            
-00006df0: 2020 2020 2020 2020 7265 7475 726e 2072          return r
-00006e00: 6573 756c 740a 2020 2020 2020 2020 2020  esult.          
-00006e10: 2020 2020 2020 636f 6e74 696e 7565 0a20        continue. 
-00006e20: 2020 2020 2020 2020 2020 2072 6574 7572             retur
-00006e30: 6e20 7265 7375 6c74 0a0a 2020 2020 6465  n result..    de
-00006e40: 6620 6377 7370 6565 645f 7370 696e 626f  f cwspeed_spinbo
-00006e50: 785f 6368 616e 6765 6428 7365 6c66 293a  x_changed(self):
-00006e60: 0a20 2020 2020 2020 2022 2222 7472 6967  .        """trig
-00006e70: 6765 7265 6420 7768 656e 2076 616c 7565  gered when value
-00006e80: 206f 6620 4357 2073 7065 6564 2069 6e20   of CW speed in 
-00006e90: 7468 6520 7370 696e 626f 7820 6368 616e  the spinbox chan
-00006ea0: 6765 732e 2222 220a 2020 2020 2020 2020  ges.""".        
-00006eb0: 6966 2073 656c 662e 6377 2e73 6572 7665  if self.cw.serve
-00006ec0: 7274 7970 6520 3d3d 2031 3a0a 2020 2020  rtype == 1:.    
-00006ed0: 2020 2020 2020 2020 7365 6c66 2e63 772e          self.cw.
-00006ee0: 7370 6565 6420 3d20 7365 6c66 2e63 775f  speed = self.cw_
-00006ef0: 7370 6565 642e 7661 6c75 6528 290a 2020  speed.value().  
-00006f00: 2020 2020 2020 2020 2020 7365 6c66 2e63            self.c
-00006f10: 772e 7365 6e64 6377 2866 225c 7831 6232  w.sendcw(f"\x1b2
-00006f20: 7b73 656c 662e 6377 2e73 7065 6564 7d22  {self.cw.speed}"
-00006f30: 290a 0a20 2020 2064 6566 206b 6579 5072  )..    def keyPr
-00006f40: 6573 7345 7665 6e74 2873 656c 662c 2065  essEvent(self, e
-00006f50: 7665 6e74 293a 2020 2320 7079 6c69 6e74  vent):  # pylint
-00006f60: 3a20 6469 7361 626c 653d 696e 7661 6c69  : disable=invali
-00006f70: 642d 6e61 6d65 0a20 2020 2020 2020 2022  d-name.        "
-00006f80: 2222 5468 6973 206f 7665 7272 6964 6573  ""This overrides
-00006f90: 2051 7420 6b65 7920 6576 656e 742e 2222   Qt key event.""
-00006fa0: 220a 2020 2020 2020 2020 6d6f 6469 6669  ".        modifi
-00006fb0: 6572 203d 2065 7665 6e74 2e6d 6f64 6966  er = event.modif
-00006fc0: 6965 7273 2829 0a20 2020 2020 2020 2069  iers().        i
-00006fd0: 6620 280a 2020 2020 2020 2020 2020 2020  f (.            
-00006fe0: 6576 656e 742e 6b65 7928 2920 3d3d 2051  event.key() == Q
-00006ff0: 742e 4b65 792e 4b65 795f 4573 6361 7065  t.Key.Key_Escape
-00007000: 2061 6e64 206d 6f64 6966 6965 7220 213d   and modifier !=
-00007010: 2051 742e 436f 6e74 726f 6c4d 6f64 6966   Qt.ControlModif
-00007020: 6965 720a 2020 2020 2020 2020 293a 2020  ier.        ):  
-00007030: 2320 7079 6c69 6e74 3a20 6469 7361 626c  # pylint: disabl
-00007040: 653d 6e6f 2d6d 656d 6265 720a 2020 2020  e=no-member.    
-00007050: 2020 2020 2020 2020 7365 6c66 2e63 6c65          self.cle
-00007060: 6172 696e 7075 7473 2829 0a20 2020 2020  arinputs().     
-00007070: 2020 2020 2020 2072 6574 7572 6e0a 2020         return.  
-00007080: 2020 2020 2020 6966 2065 7665 6e74 2e6b        if event.k
-00007090: 6579 2829 203d 3d20 5174 2e4b 6579 2e4b  ey() == Qt.Key.K
-000070a0: 6579 5f45 7363 6170 6520 616e 6420 6d6f  ey_Escape and mo
-000070b0: 6469 6669 6572 203d 3d20 5174 2e43 6f6e  difier == Qt.Con
-000070c0: 7472 6f6c 4d6f 6469 6669 6572 3a0a 2020  trolModifier:.  
-000070d0: 2020 2020 2020 2020 2020 6966 2073 656c            if sel
-000070e0: 662e 6377 2069 7320 6e6f 7420 4e6f 6e65  f.cw is not None
-000070f0: 3a0a 2020 2020 2020 2020 2020 2020 2020  :.              
-00007100: 2020 6966 2073 656c 662e 6377 2e73 6572    if self.cw.ser
-00007110: 7665 7274 7970 6520 3d3d 2031 3a0a 2020  vertype == 1:.  
+00005d10: 2020 7365 6c66 2e63 775f 7370 6565 642e    self.cw_speed.
+00005d20: 6869 6465 2829 0a0a 2020 2020 2020 2020  hide()..        
+00005d30: 2020 2020 2020 2020 636d 6420 3d20 7b7d          cmd = {}
+00005d40: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00005d50: 2063 6d64 5b22 636d 6422 5d20 3d20 224e   cmd["cmd"] = "N
+00005d60: 4557 4442 220a 2020 2020 2020 2020 2020  EWDB".          
+00005d70: 2020 2020 2020 636d 645b 2273 7461 7469        cmd["stati
+00005d80: 6f6e 225d 203d 2070 6c61 7466 6f72 6d2e  on"] = platform.
+00005d90: 6e6f 6465 2829 0a20 2020 2020 2020 2020  node().         
+00005da0: 2020 2020 2020 2073 656c 662e 6d75 6c74         self.mult
+00005db0: 6963 6173 745f 696e 7465 7266 6163 652e  icast_interface.
+00005dc0: 7365 6e64 5f61 735f 6a73 6f6e 2863 6d64  send_as_json(cmd
+00005dd0: 290a 2020 2020 2020 2020 2020 2020 2020  ).              
+00005de0: 2020 6966 2068 6173 6174 7472 2873 656c    if hasattr(sel
+00005df0: 662e 636f 6e74 6573 742c 2022 636f 6c75  f.contest, "colu
+00005e00: 6d6e 7322 293a 0a20 2020 2020 2020 2020  mns"):.         
+00005e10: 2020 2020 2020 2020 2020 2063 6d64 203d             cmd =
+00005e20: 207b 7d0a 2020 2020 2020 2020 2020 2020   {}.            
+00005e30: 2020 2020 2020 2020 636d 645b 2263 6d64          cmd["cmd
+00005e40: 225d 203d 2022 5348 4f57 434f 4c55 4d4e  "] = "SHOWCOLUMN
+00005e50: 5322 0a20 2020 2020 2020 2020 2020 2020  S".             
+00005e60: 2020 2020 2020 2063 6d64 5b22 7374 6174         cmd["stat
+00005e70: 696f 6e22 5d20 3d20 706c 6174 666f 726d  ion"] = platform
+00005e80: 2e6e 6f64 6528 290a 2020 2020 2020 2020  .node().        
+00005e90: 2020 2020 2020 2020 2020 2020 636d 645b              cmd[
+00005ea0: 2243 4f4c 554d 4e53 225d 203d 2073 656c  "COLUMNS"] = sel
+00005eb0: 662e 636f 6e74 6573 742e 636f 6c75 6d6e  f.contest.column
+00005ec0: 730a 2020 2020 2020 2020 2020 2020 2020  s.              
+00005ed0: 2020 2020 2020 7365 6c66 2e6d 756c 7469        self.multi
+00005ee0: 6361 7374 5f69 6e74 6572 6661 6365 2e73  cast_interface.s
+00005ef0: 656e 645f 6173 5f6a 736f 6e28 636d 6429  end_as_json(cmd)
+00005f00: 0a0a 2020 2020 6465 6620 6869 6465 5f62  ..    def hide_b
+00005f10: 616e 645f 6d6f 6465 2873 656c 662c 2074  and_mode(self, t
+00005f20: 6865 5f6d 6f64 653a 2073 7472 2920 2d3e  he_mode: str) ->
+00005f30: 204e 6f6e 653a 0a20 2020 2020 2020 2022   None:.        "
+00005f40: 2222 6869 6465 2222 220a 2020 2020 2020  ""hide""".      
+00005f50: 2020 6c6f 6767 6572 2e64 6562 7567 2822    logger.debug("
+00005f60: 2573 222c 2066 227b 7468 655f 6d6f 6465  %s", f"{the_mode
+00005f70: 7d22 290a 2020 2020 2020 2020 7365 6c66  }").        self
+00005f80: 2e42 616e 645f 4d6f 6465 5f46 7261 6d65  .Band_Mode_Frame
+00005f90: 5f43 572e 6869 6465 2829 0a20 2020 2020  _CW.hide().     
+00005fa0: 2020 2073 656c 662e 4261 6e64 5f4d 6f64     self.Band_Mod
+00005fb0: 655f 4672 616d 655f 5353 422e 6869 6465  e_Frame_SSB.hide
+00005fc0: 2829 0a20 2020 2020 2020 2073 656c 662e  ().        self.
+00005fd0: 4261 6e64 5f4d 6f64 655f 4672 616d 655f  Band_Mode_Frame_
+00005fe0: 5254 5459 2e68 6964 6528 290a 2020 2020  RTTY.hide().    
+00005ff0: 2020 2020 6d6f 6465 7320 3d20 7b0a 2020      modes = {.  
+00006000: 2020 2020 2020 2020 2020 2243 5722 3a20            "CW": 
+00006010: 2873 656c 662e 4261 6e64 5f4d 6f64 655f  (self.Band_Mode_
+00006020: 4672 616d 655f 4357 2c29 2c0a 2020 2020  Frame_CW,),.    
+00006030: 2020 2020 2020 2020 2253 5342 223a 2028          "SSB": (
+00006040: 7365 6c66 2e42 616e 645f 4d6f 6465 5f46  self.Band_Mode_F
+00006050: 7261 6d65 5f53 5342 2c29 2c0a 2020 2020  rame_SSB,),.    
+00006060: 2020 2020 2020 2020 2252 5454 5922 3a20          "RTTY": 
+00006070: 2873 656c 662e 4261 6e64 5f4d 6f64 655f  (self.Band_Mode_
+00006080: 4672 616d 655f 5254 5459 2c29 2c0a 2020  Frame_RTTY,),.  
+00006090: 2020 2020 2020 2020 2020 2250 534b 223a            "PSK":
+000060a0: 2028 7365 6c66 2e42 616e 645f 4d6f 6465   (self.Band_Mode
+000060b0: 5f46 7261 6d65 5f52 5454 592c 292c 0a20  _Frame_RTTY,),. 
+000060c0: 2020 2020 2020 2020 2020 2022 5353 422b             "SSB+
+000060d0: 4357 223a 2028 7365 6c66 2e42 616e 645f  CW": (self.Band_
+000060e0: 4d6f 6465 5f46 7261 6d65 5f43 572c 2073  Mode_Frame_CW, s
+000060f0: 656c 662e 4261 6e64 5f4d 6f64 655f 4672  elf.Band_Mode_Fr
+00006100: 616d 655f 5353 4229 2c0a 2020 2020 2020  ame_SSB),.      
+00006110: 2020 2020 2020 2242 4f54 4822 3a20 2873        "BOTH": (s
+00006120: 656c 662e 4261 6e64 5f4d 6f64 655f 4672  elf.Band_Mode_Fr
+00006130: 616d 655f 4357 2c20 7365 6c66 2e42 616e  ame_CW, self.Ban
+00006140: 645f 4d6f 6465 5f46 7261 6d65 5f53 5342  d_Mode_Frame_SSB
+00006150: 292c 0a20 2020 2020 2020 2020 2020 2022  ),.            "
+00006160: 4449 4749 5441 4c22 3a20 2873 656c 662e  DIGITAL": (self.
+00006170: 4261 6e64 5f4d 6f64 655f 4672 616d 655f  Band_Mode_Frame_
+00006180: 5254 5459 2c29 2c0a 2020 2020 2020 2020  RTTY,),.        
+00006190: 2020 2020 2253 5342 2b43 572b 4449 4749      "SSB+CW+DIGI
+000061a0: 5441 4c22 3a20 280a 2020 2020 2020 2020  TAL": (.        
+000061b0: 2020 2020 2020 2020 7365 6c66 2e42 616e          self.Ban
+000061c0: 645f 4d6f 6465 5f46 7261 6d65 5f52 5454  d_Mode_Frame_RTT
+000061d0: 592c 0a20 2020 2020 2020 2020 2020 2020  Y,.             
+000061e0: 2020 2073 656c 662e 4261 6e64 5f4d 6f64     self.Band_Mod
+000061f0: 655f 4672 616d 655f 4357 2c0a 2020 2020  e_Frame_CW,.    
+00006200: 2020 2020 2020 2020 2020 2020 7365 6c66              self
+00006210: 2e42 616e 645f 4d6f 6465 5f46 7261 6d65  .Band_Mode_Frame
+00006220: 5f53 5342 2c0a 2020 2020 2020 2020 2020  _SSB,.          
+00006230: 2020 292c 0a20 2020 2020 2020 2020 2020    ),.           
+00006240: 2022 464d 223a 2028 7365 6c66 2e42 616e   "FM": (self.Ban
+00006250: 645f 4d6f 6465 5f46 7261 6d65 5f53 5342  d_Mode_Frame_SSB
+00006260: 2c29 2c0a 2020 2020 2020 2020 7d0a 2020  ,),.        }.  
+00006270: 2020 2020 2020 6672 616d 6573 203d 206d        frames = m
+00006280: 6f64 6573 2e67 6574 2874 6865 5f6d 6f64  odes.get(the_mod
+00006290: 6529 0a20 2020 2020 2020 2069 6620 6672  e).        if fr
+000062a0: 616d 6573 3a0a 2020 2020 2020 2020 2020  ames:.          
+000062b0: 2020 666f 7220 6672 616d 6520 696e 2066    for frame in f
+000062c0: 7261 6d65 733a 0a20 2020 2020 2020 2020  rames:.         
+000062d0: 2020 2020 2020 2066 7261 6d65 2e73 686f         frame.sho
+000062e0: 7728 290a 0a20 2020 2064 6566 2066 696c  w()..    def fil
+000062f0: 6570 6963 6b65 7228 7365 6c66 2c20 6163  epicker(self, ac
+00006300: 7469 6f6e 3a20 7374 7229 202d 3e20 7374  tion: str) -> st
+00006310: 723a 0a20 2020 2020 2020 2022 2222 0a20  r:.        """. 
+00006320: 2020 2020 2020 2047 6574 2061 2066 696c         Get a fil
+00006330: 656e 616d 650a 2020 2020 2020 2020 6163  ename.        ac
+00006340: 7469 6f6e 3a20 226e 6577 2220 6f72 2022  tion: "new" or "
+00006350: 6f70 656e 220a 2020 2020 2020 2020 2222  open".        ""
+00006360: 220a 2020 2020 2020 2020 6f70 7469 6f6e  ".        option
+00006370: 7320 3d20 5146 696c 6544 6961 6c6f 672e  s = QFileDialog.
+00006380: 4f70 7469 6f6e 7328 290a 2020 2020 2020  Options().      
+00006390: 2020 6f70 7469 6f6e 7320 7c3d 2051 4669    options |= QFi
+000063a0: 6c65 4469 616c 6f67 2e44 6f6e 7455 7365  leDialog.DontUse
+000063b0: 4e61 7469 7665 4469 616c 6f67 0a20 2020  NativeDialog.   
+000063c0: 2020 2020 206f 7074 696f 6e73 207c 3d20       options |= 
+000063d0: 5146 696c 6544 6961 6c6f 672e 446f 6e74  QFileDialog.Dont
+000063e0: 436f 6e66 6972 6d4f 7665 7277 7269 7465  ConfirmOverwrite
+000063f0: 0a20 2020 2020 2020 2023 2070 6963 6b65  .        # picke
+00006400: 7220 3d20 5146 696c 6544 6961 6c6f 6728  r = QFileDialog(
+00006410: 7365 6c66 290a 2020 2020 2020 2020 6966  self).        if
+00006420: 2061 6374 696f 6e20 3d3d 2022 6e65 7722   action == "new"
+00006430: 3a0a 2020 2020 2020 2020 2020 2020 6669  :.            fi
+00006440: 6c65 2c20 5f20 3d20 5146 696c 6544 6961  le, _ = QFileDia
+00006450: 6c6f 672e 6765 7453 6176 6546 696c 654e  log.getSaveFileN
+00006460: 616d 6528 0a20 2020 2020 2020 2020 2020  ame(.           
+00006470: 2020 2020 2073 656c 662c 0a20 2020 2020       self,.     
+00006480: 2020 2020 2020 2020 2020 2022 4368 6f6f             "Choo
+00006490: 7365 2061 2044 6174 6162 6173 6522 2c0a  se a Database",.
+000064a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000064b0: 4441 5441 5f50 4154 482c 0a20 2020 2020  DATA_PATH,.     
+000064c0: 2020 2020 2020 2020 2020 2022 4461 7461             "Data
+000064d0: 6261 7365 2028 2a2e 6462 2922 2c0a 2020  base (*.db)",.  
+000064e0: 2020 2020 2020 2020 2020 2020 2020 6f70                op
+000064f0: 7469 6f6e 733d 6f70 7469 6f6e 732c 0a20  tions=options,. 
+00006500: 2020 2020 2020 2020 2020 2029 0a20 2020             ).   
+00006510: 2020 2020 2069 6620 6163 7469 6f6e 203d       if action =
+00006520: 3d20 226f 7065 6e22 3a0a 2020 2020 2020  = "open":.      
+00006530: 2020 2020 2020 6669 6c65 2c20 5f20 3d20        file, _ = 
+00006540: 5146 696c 6544 6961 6c6f 672e 6765 744f  QFileDialog.getO
+00006550: 7065 6e46 696c 654e 616d 6528 0a20 2020  penFileName(.   
+00006560: 2020 2020 2020 2020 2020 2020 2073 656c               sel
+00006570: 662c 0a20 2020 2020 2020 2020 2020 2020  f,.             
+00006580: 2020 2022 4368 6f6f 7365 2061 2044 6174     "Choose a Dat
+00006590: 6162 6173 6522 2c0a 2020 2020 2020 2020  abase",.        
+000065a0: 2020 2020 2020 2020 4441 5441 5f50 4154          DATA_PAT
+000065b0: 482c 0a20 2020 2020 2020 2020 2020 2020  H,.             
+000065c0: 2020 2022 4461 7461 6261 7365 2028 2a2e     "Database (*.
+000065d0: 6462 2922 2c0a 2020 2020 2020 2020 2020  db)",.          
+000065e0: 2020 2020 2020 6f70 7469 6f6e 733d 6f70        options=op
+000065f0: 7469 6f6e 732c 0a20 2020 2020 2020 2020  tions,.         
+00006600: 2020 2029 0a20 2020 2020 2020 2072 6574     ).        ret
+00006610: 7572 6e20 6669 6c65 0a0a 2020 2020 6465  urn file..    de
+00006620: 6620 7265 6361 6c63 756c 6174 655f 6d75  f recalculate_mu
+00006630: 6c74 7328 7365 6c66 293a 0a20 2020 2020  lts(self):.     
+00006640: 2020 2022 2222 5265 6361 6c63 756c 6174     """Recalculat
+00006650: 6520 4d75 6c74 6970 6c69 6572 7322 2222  e Multipliers"""
+00006660: 0a20 2020 2020 2020 2073 656c 662e 636f  .        self.co
+00006670: 6e74 6573 742e 7265 6361 6c63 756c 6174  ntest.recalculat
+00006680: 655f 6d75 6c74 7328 7365 6c66 290a 0a20  e_mults(self).. 
+00006690: 2020 2064 6566 206c 6175 6e63 685f 6c6f     def launch_lo
+000066a0: 675f 7769 6e64 6f77 2873 656c 6629 3a0a  g_window(self):.
+000066b0: 2020 2020 2020 2020 2222 226c 6175 6e63          """launc
+000066c0: 6820 7468 6520 4c6f 6720 5769 6e64 6f77  h the Log Window
+000066d0: 2222 220a 2020 2020 2020 2020 6966 206e  """.        if n
+000066e0: 6f74 2063 6865 636b 5f70 726f 6365 7373  ot check_process
+000066f0: 2822 6c6f 6777 696e 646f 772e 7079 2229  ("logwindow.py")
+00006700: 3a0a 2020 2020 2020 2020 2020 2020 5f20  :.            _ 
+00006710: 3d20 7375 6270 726f 6365 7373 2e50 6f70  = subprocess.Pop
+00006720: 656e 285b 7379 732e 6578 6563 7574 6162  en([sys.executab
+00006730: 6c65 2c20 574f 524b 494e 475f 5041 5448  le, WORKING_PATH
+00006740: 202b 2022 2f6c 6f67 7769 6e64 6f77 2e70   + "/logwindow.p
+00006750: 7922 5d29 0a0a 2020 2020 6465 6620 6c61  y"])..    def la
+00006760: 756e 6368 5f62 616e 646d 6170 5f77 696e  unch_bandmap_win
+00006770: 646f 7728 7365 6c66 293a 0a20 2020 2020  dow(self):.     
+00006780: 2020 2022 2222 6c61 756e 6368 2074 6865     """launch the
+00006790: 204c 6f67 2057 696e 646f 7722 2222 0a20   Log Window""". 
+000067a0: 2020 2020 2020 2069 6620 6e6f 7420 6368         if not ch
+000067b0: 6563 6b5f 7072 6f63 6573 7328 2262 616e  eck_process("ban
+000067c0: 646d 6170 2e70 7922 293a 0a20 2020 2020  dmap.py"):.     
+000067d0: 2020 2020 2020 205f 203d 2073 7562 7072         _ = subpr
+000067e0: 6f63 6573 732e 506f 7065 6e28 5b73 7973  ocess.Popen([sys
+000067f0: 2e65 7865 6375 7461 626c 652c 2057 4f52  .executable, WOR
+00006800: 4b49 4e47 5f50 4154 4820 2b20 222f 6261  KING_PATH + "/ba
+00006810: 6e64 6d61 702e 7079 225d 290a 0a20 2020  ndmap.py"])..   
+00006820: 2064 6566 2063 6c65 6172 5f62 616e 645f   def clear_band_
+00006830: 696e 6469 6361 746f 7273 2873 656c 6629  indicators(self)
+00006840: 3a0a 2020 2020 2020 2020 2222 2243 6c65  :.        """Cle
+00006850: 6172 2074 6865 2069 6e64 6963 6174 6f72  ar the indicator
+00006860: 7322 2222 0a20 2020 2020 2020 2066 6f72  s""".        for
+00006870: 205f 2c20 696e 6469 6361 746f 7273 2069   _, indicators i
+00006880: 6e20 7365 6c66 2e61 6c6c 5f6d 6f64 655f  n self.all_mode_
+00006890: 696e 6469 6361 746f 7273 2e69 7465 6d73  indicators.items
+000068a0: 2829 3a0a 2020 2020 2020 2020 2020 2020  ():.            
+000068b0: 666f 7220 5f2c 2069 6e64 6963 6174 6f72  for _, indicator
+000068c0: 2069 6e20 696e 6469 6361 746f 7273 2e69   in indicators.i
+000068d0: 7465 6d73 2829 3a0a 2020 2020 2020 2020  tems():.        
+000068e0: 2020 2020 2020 2020 696e 6469 6361 746f          indicato
+000068f0: 722e 7365 7446 7261 6d65 5368 6170 6528  r.setFrameShape(
+00006900: 5174 5769 6467 6574 732e 5146 7261 6d65  QtWidgets.QFrame
+00006910: 2e4e 6f46 7261 6d65 290a 0a20 2020 2064  .NoFrame)..    d
+00006920: 6566 2073 6574 5f62 616e 645f 696e 6469  ef set_band_indi
+00006930: 6361 746f 7228 7365 6c66 2c20 6261 6e64  cator(self, band
+00006940: 3a20 7374 7229 202d 3e20 4e6f 6e65 3a0a  : str) -> None:.
+00006950: 2020 2020 2020 2020 2222 2253 6574 2074          """Set t
+00006960: 6865 2062 616e 6420 696e 6469 6361 746f  he band indicato
+00006970: 7222 2222 0a20 2020 2020 2020 206c 6f67  r""".        log
+00006980: 6765 722e 6465 6275 6728 2225 7322 2c20  ger.debug("%s", 
+00006990: 6622 6261 6e64 3a7b 6261 6e64 7d20 6d6f  f"band:{band} mo
+000069a0: 6465 3a20 7b73 656c 662e 6375 7272 656e  de: {self.curren
+000069b0: 745f 6d6f 6465 7d22 290a 2020 2020 2020  t_mode}").      
+000069c0: 2020 6966 2062 616e 6420 616e 6420 7365    if band and se
+000069d0: 6c66 2e63 7572 7265 6e74 5f6d 6f64 653a  lf.current_mode:
+000069e0: 0a20 2020 2020 2020 2020 2020 2073 656c  .            sel
+000069f0: 662e 636c 6561 725f 6261 6e64 5f69 6e64  f.clear_band_ind
+00006a00: 6963 6174 6f72 7328 290a 2020 2020 2020  icators().      
+00006a10: 2020 2020 2020 696e 6469 6361 746f 7220        indicator 
+00006a20: 3d20 7365 6c66 2e61 6c6c 5f6d 6f64 655f  = self.all_mode_
+00006a30: 696e 6469 6361 746f 7273 5b73 656c 662e  indicators[self.
+00006a40: 6375 7272 656e 745f 6d6f 6465 5d2e 6765  current_mode].ge
+00006a50: 7428 6261 6e64 2c20 4e6f 6e65 290a 2020  t(band, None).  
+00006a60: 2020 2020 2020 2020 2020 6966 2069 6e64            if ind
+00006a70: 6963 6174 6f72 3a0a 2020 2020 2020 2020  icator:.        
+00006a80: 2020 2020 2020 2020 696e 6469 6361 746f          indicato
+00006a90: 722e 7365 7446 7261 6d65 5368 6170 6528  r.setFrameShape(
+00006aa0: 5174 5769 6467 6574 732e 5146 7261 6d65  QtWidgets.QFrame
+00006ab0: 2e42 6f78 290a 0a20 2020 2064 6566 2063  .Box)..    def c
+00006ac0: 6c6f 7365 4576 656e 7428 7365 6c66 2c20  loseEvent(self, 
+00006ad0: 5f65 7665 6e74 293a 0a20 2020 2020 2020  _event):.       
+00006ae0: 2022 2222 0a20 2020 2020 2020 2057 7269   """.        Wri
+00006af0: 7465 2077 696e 646f 7720 7369 7a65 2061  te window size a
+00006b00: 6e64 2070 6f73 6974 696f 6e20 746f 2063  nd position to c
+00006b10: 6f6e 6669 6720 6669 6c65 0a20 2020 2020  onfig file.     
+00006b20: 2020 2022 2222 0a20 2020 2020 2020 2073     """.        s
+00006b30: 656c 662e 7072 6566 5b22 7769 6e64 6f77  elf.pref["window
+00006b40: 5f77 6964 7468 225d 203d 2073 656c 662e  _width"] = self.
+00006b50: 7369 7a65 2829 2e77 6964 7468 2829 0a20  size().width(). 
+00006b60: 2020 2020 2020 2073 656c 662e 7072 6566         self.pref
+00006b70: 5b22 7769 6e64 6f77 5f68 6569 6768 7422  ["window_height"
+00006b80: 5d20 3d20 7365 6c66 2e73 697a 6528 292e  ] = self.size().
+00006b90: 6865 6967 6874 2829 0a20 2020 2020 2020  height().       
+00006ba0: 2073 656c 662e 7072 6566 5b22 7769 6e64   self.pref["wind
+00006bb0: 6f77 5f78 225d 203d 2073 656c 662e 706f  ow_x"] = self.po
+00006bc0: 7328 292e 7828 290a 2020 2020 2020 2020  s().x().        
+00006bd0: 7365 6c66 2e70 7265 665b 2277 696e 646f  self.pref["windo
+00006be0: 775f 7922 5d20 3d20 7365 6c66 2e70 6f73  w_y"] = self.pos
+00006bf0: 2829 2e79 2829 0a20 2020 2020 2020 2073  ().y().        s
+00006c00: 656c 662e 7772 6974 655f 7072 6566 6572  elf.write_prefer
+00006c10: 656e 6365 2829 0a0a 2020 2020 6465 6620  ence()..    def 
+00006c20: 6374 795f 6c6f 6f6b 7570 2873 656c 662c  cty_lookup(self,
+00006c30: 2063 616c 6c73 6967 6e3a 2073 7472 293a   callsign: str):
+00006c40: 0a20 2020 2020 2020 2022 2222 4c6f 6f6b  .        """Look
+00006c50: 7570 2063 616c 6c73 6967 6e20 696e 2063  up callsign in c
+00006c60: 7479 2e64 6174 2066 696c 6522 2222 0a20  ty.dat file""". 
+00006c70: 2020 2020 2020 2063 616c 6c73 6967 6e20         callsign 
+00006c80: 3d20 6361 6c6c 7369 676e 2e75 7070 6572  = callsign.upper
+00006c90: 2829 0a20 2020 2020 2020 2066 6f72 2063  ().        for c
+00006ca0: 6f75 6e74 2069 6e20 7265 7665 7273 6564  ount in reversed
+00006cb0: 2872 616e 6765 286c 656e 2863 616c 6c73  (range(len(calls
+00006cc0: 6967 6e29 2929 3a0a 2020 2020 2020 2020  ign))):.        
+00006cd0: 2020 2020 7365 6172 6368 6974 656d 203d      searchitem =
+00006ce0: 2063 616c 6c73 6967 6e5b 3a20 636f 756e   callsign[: coun
+00006cf0: 7420 2b20 315d 0a20 2020 2020 2020 2020  t + 1].         
+00006d00: 2020 2072 6573 756c 7420 3d20 7b6b 6579     result = {key
+00006d10: 3a20 7661 6c20 666f 7220 6b65 792c 2076  : val for key, v
+00006d20: 616c 2069 6e20 4354 5946 494c 452e 6974  al in CTYFILE.it
+00006d30: 656d 7328 2920 6966 206b 6579 203d 3d20  ems() if key == 
+00006d40: 7365 6172 6368 6974 656d 7d0a 2020 2020  searchitem}.    
+00006d50: 2020 2020 2020 2020 6966 206e 6f74 2072          if not r
+00006d60: 6573 756c 743a 0a20 2020 2020 2020 2020  esult:.         
+00006d70: 2020 2020 2020 2063 6f6e 7469 6e75 650a         continue.
+00006d80: 2020 2020 2020 2020 2020 2020 6966 2072              if r
+00006d90: 6573 756c 742e 6765 7428 7365 6172 6368  esult.get(search
+00006da0: 6974 656d 292e 6765 7428 2265 7861 6374  item).get("exact
+00006db0: 5f6d 6174 6368 2229 3a0a 2020 2020 2020  _match"):.      
+00006dc0: 2020 2020 2020 2020 2020 6966 2073 6561            if sea
+00006dd0: 7263 6869 7465 6d20 3d3d 2063 616c 6c73  rchitem == calls
+00006de0: 6967 6e3a 0a20 2020 2020 2020 2020 2020  ign:.           
+00006df0: 2020 2020 2020 2020 2072 6574 7572 6e20           return 
+00006e00: 7265 7375 6c74 0a20 2020 2020 2020 2020  result.         
+00006e10: 2020 2020 2020 2063 6f6e 7469 6e75 650a         continue.
+00006e20: 2020 2020 2020 2020 2020 2020 7265 7475              retu
+00006e30: 726e 2072 6573 756c 740a 0a20 2020 2064  rn result..    d
+00006e40: 6566 2063 7773 7065 6564 5f73 7069 6e62  ef cwspeed_spinb
+00006e50: 6f78 5f63 6861 6e67 6564 2873 656c 6629  ox_changed(self)
+00006e60: 3a0a 2020 2020 2020 2020 2222 2274 7269  :.        """tri
+00006e70: 6767 6572 6564 2077 6865 6e20 7661 6c75  ggered when valu
+00006e80: 6520 6f66 2043 5720 7370 6565 6420 696e  e of CW speed in
+00006e90: 2074 6865 2073 7069 6e62 6f78 2063 6861   the spinbox cha
+00006ea0: 6e67 6573 2e22 2222 0a20 2020 2020 2020  nges.""".       
+00006eb0: 2069 6620 7365 6c66 2e63 772e 7365 7276   if self.cw.serv
+00006ec0: 6572 7479 7065 203d 3d20 313a 0a20 2020  ertype == 1:.   
+00006ed0: 2020 2020 2020 2020 2073 656c 662e 6377           self.cw
+00006ee0: 2e73 7065 6564 203d 2073 656c 662e 6377  .speed = self.cw
+00006ef0: 5f73 7065 6564 2e76 616c 7565 2829 0a20  _speed.value(). 
+00006f00: 2020 2020 2020 2020 2020 2073 656c 662e             self.
+00006f10: 6377 2e73 656e 6463 7728 6622 5c78 3162  cw.sendcw(f"\x1b
+00006f20: 327b 7365 6c66 2e63 772e 7370 6565 647d  2{self.cw.speed}
+00006f30: 2229 0a0a 2020 2020 6465 6620 6b65 7950  ")..    def keyP
+00006f40: 7265 7373 4576 656e 7428 7365 6c66 2c20  ressEvent(self, 
+00006f50: 6576 656e 7429 3a20 2023 2070 796c 696e  event):  # pylin
+00006f60: 743a 2064 6973 6162 6c65 3d69 6e76 616c  t: disable=inval
+00006f70: 6964 2d6e 616d 650a 2020 2020 2020 2020  id-name.        
+00006f80: 2222 2254 6869 7320 6f76 6572 7269 6465  """This override
+00006f90: 7320 5174 206b 6579 2065 7665 6e74 2e22  s Qt key event."
+00006fa0: 2222 0a20 2020 2020 2020 206d 6f64 6966  "".        modif
+00006fb0: 6965 7220 3d20 6576 656e 742e 6d6f 6469  ier = event.modi
+00006fc0: 6669 6572 7328 290a 2020 2020 2020 2020  fiers().        
+00006fd0: 6966 2028 0a20 2020 2020 2020 2020 2020  if (.           
+00006fe0: 2065 7665 6e74 2e6b 6579 2829 203d 3d20   event.key() == 
+00006ff0: 5174 2e4b 6579 2e4b 6579 5f45 7363 6170  Qt.Key.Key_Escap
+00007000: 6520 616e 6420 6d6f 6469 6669 6572 2021  e and modifier !
+00007010: 3d20 5174 2e43 6f6e 7472 6f6c 4d6f 6469  = Qt.ControlModi
+00007020: 6669 6572 0a20 2020 2020 2020 2029 3a20  fier.        ): 
+00007030: 2023 2070 796c 696e 743a 2064 6973 6162   # pylint: disab
+00007040: 6c65 3d6e 6f2d 6d65 6d62 6572 0a20 2020  le=no-member.   
+00007050: 2020 2020 2020 2020 2073 656c 662e 636c           self.cl
+00007060: 6561 7269 6e70 7574 7328 290a 2020 2020  earinputs().    
+00007070: 2020 2020 2020 2020 7265 7475 726e 0a20          return. 
+00007080: 2020 2020 2020 2069 6620 6576 656e 742e         if event.
+00007090: 6b65 7928 2920 3d3d 2051 742e 4b65 792e  key() == Qt.Key.
+000070a0: 4b65 795f 4573 6361 7065 2061 6e64 206d  Key_Escape and m
+000070b0: 6f64 6966 6965 7220 3d3d 2051 742e 436f  odifier == Qt.Co
+000070c0: 6e74 726f 6c4d 6f64 6966 6965 723a 0a20  ntrolModifier:. 
+000070d0: 2020 2020 2020 2020 2020 2069 6620 7365             if se
+000070e0: 6c66 2e63 7720 6973 206e 6f74 204e 6f6e  lf.cw is not Non
+000070f0: 653a 0a20 2020 2020 2020 2020 2020 2020  e:.             
+00007100: 2020 2069 6620 7365 6c66 2e63 772e 7365     if self.cw.se
+00007110: 7276 6572 7479 7065 203d 3d20 313a 0a20  rvertype == 1:. 
 00007120: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00007130: 2020 7365 6c66 2e63 772e 7365 6e64 6377    self.cw.sendcw
-00007140: 2822 5c78 3162 3422 290a 2020 2020 2020  ("\x1b4").      
-00007150: 2020 2020 2020 2020 2020 2020 2020 7265                re
-00007160: 7475 726e 0a20 2020 2020 2020 2069 6620  turn.        if 
-00007170: 6576 656e 742e 6b65 7928 2920 3d3d 2051  event.key() == Q
-00007180: 742e 4b65 792e 4b65 795f 5061 6765 5570  t.Key.Key_PageUp
-00007190: 2061 6e64 206d 6f64 6966 6965 7220 3d3d   and modifier ==
-000071a0: 2051 742e 436f 6e74 726f 6c4d 6f64 6966   Qt.ControlModif
-000071b0: 6965 723a 0a20 2020 2020 2020 2020 2020  ier:.           
-000071c0: 2063 6d64 203d 207b 7d0a 2020 2020 2020   cmd = {}.      
-000071d0: 2020 2020 2020 636d 645b 2263 6d64 225d        cmd["cmd"]
-000071e0: 203d 2022 4e45 5854 5350 4f54 220a 2020   = "NEXTSPOT".  
-000071f0: 2020 2020 2020 2020 2020 636d 645b 2273            cmd["s
-00007200: 7461 7469 6f6e 225d 203d 2070 6c61 7466  tation"] = platf
-00007210: 6f72 6d2e 6e6f 6465 2829 0a20 2020 2020  orm.node().     
-00007220: 2020 2020 2020 2073 656c 662e 6d75 6c74         self.mult
-00007230: 6963 6173 745f 696e 7465 7266 6163 652e  icast_interface.
-00007240: 7365 6e64 5f61 735f 6a73 6f6e 2863 6d64  send_as_json(cmd
-00007250: 290a 2020 2020 2020 2020 2020 2020 7265  ).            re
-00007260: 7475 726e 0a20 2020 2020 2020 2069 6620  turn.        if 
-00007270: 6576 656e 742e 6b65 7928 2920 3d3d 2051  event.key() == Q
-00007280: 742e 4b65 792e 4b65 795f 5061 6765 446f  t.Key.Key_PageDo
-00007290: 776e 2061 6e64 206d 6f64 6966 6965 7220  wn and modifier 
-000072a0: 3d3d 2051 742e 436f 6e74 726f 6c4d 6f64  == Qt.ControlMod
-000072b0: 6966 6965 723a 0a20 2020 2020 2020 2020  ifier:.         
-000072c0: 2020 2063 6d64 203d 207b 7d0a 2020 2020     cmd = {}.    
-000072d0: 2020 2020 2020 2020 636d 645b 2263 6d64          cmd["cmd
-000072e0: 225d 203d 2022 5052 4556 5350 4f54 220a  "] = "PREVSPOT".
-000072f0: 2020 2020 2020 2020 2020 2020 636d 645b              cmd[
-00007300: 2273 7461 7469 6f6e 225d 203d 2070 6c61  "station"] = pla
-00007310: 7466 6f72 6d2e 6e6f 6465 2829 0a20 2020  tform.node().   
-00007320: 2020 2020 2020 2020 2073 656c 662e 6d75           self.mu
-00007330: 6c74 6963 6173 745f 696e 7465 7266 6163  lticast_interfac
-00007340: 652e 7365 6e64 5f61 735f 6a73 6f6e 2863  e.send_as_json(c
-00007350: 6d64 290a 2020 2020 2020 2020 2020 2020  md).            
-00007360: 7265 7475 726e 0a20 2020 2020 2020 2069  return.        i
-00007370: 6620 6576 656e 742e 6b65 7928 2920 3d3d  f event.key() ==
-00007380: 2051 742e 4b65 792e 4b65 795f 5061 6765   Qt.Key.Key_Page
-00007390: 5570 2061 6e64 206d 6f64 6966 6965 7220  Up and modifier 
-000073a0: 213d 2051 742e 436f 6e74 726f 6c4d 6f64  != Qt.ControlMod
-000073b0: 6966 6965 723a 0a20 2020 2020 2020 2020  ifier:.         
-000073c0: 2020 2069 6620 7365 6c66 2e63 7720 6973     if self.cw is
-000073d0: 206e 6f74 204e 6f6e 653a 0a20 2020 2020   not None:.     
-000073e0: 2020 2020 2020 2020 2020 2069 6620 7365             if se
-000073f0: 6c66 2e63 772e 7365 7276 6572 7479 7065  lf.cw.servertype
-00007400: 203d 3d20 313a 0a20 2020 2020 2020 2020   == 1:.         
-00007410: 2020 2020 2020 2020 2020 2073 656c 662e             self.
-00007420: 6377 2e73 7065 6564 202b 3d20 310a 2020  cw.speed += 1.  
+00007130: 2020 2073 656c 662e 6377 2e73 656e 6463     self.cw.sendc
+00007140: 7728 225c 7831 6234 2229 0a20 2020 2020  w("\x1b4").     
+00007150: 2020 2020 2020 2020 2020 2020 2020 2072                 r
+00007160: 6574 7572 6e0a 2020 2020 2020 2020 6966  eturn.        if
+00007170: 2065 7665 6e74 2e6b 6579 2829 203d 3d20   event.key() == 
+00007180: 5174 2e4b 6579 2e4b 6579 5f50 6167 6555  Qt.Key.Key_PageU
+00007190: 7020 616e 6420 6d6f 6469 6669 6572 203d  p and modifier =
+000071a0: 3d20 5174 2e43 6f6e 7472 6f6c 4d6f 6469  = Qt.ControlModi
+000071b0: 6669 6572 3a0a 2020 2020 2020 2020 2020  fier:.          
+000071c0: 2020 636d 6420 3d20 7b7d 0a20 2020 2020    cmd = {}.     
+000071d0: 2020 2020 2020 2063 6d64 5b22 636d 6422         cmd["cmd"
+000071e0: 5d20 3d20 2250 5245 5653 504f 5422 0a20  ] = "PREVSPOT". 
+000071f0: 2020 2020 2020 2020 2020 2063 6d64 5b22             cmd["
+00007200: 7374 6174 696f 6e22 5d20 3d20 706c 6174  station"] = plat
+00007210: 666f 726d 2e6e 6f64 6528 290a 2020 2020  form.node().    
+00007220: 2020 2020 2020 2020 7365 6c66 2e6d 756c          self.mul
+00007230: 7469 6361 7374 5f69 6e74 6572 6661 6365  ticast_interface
+00007240: 2e73 656e 645f 6173 5f6a 736f 6e28 636d  .send_as_json(cm
+00007250: 6429 0a20 2020 2020 2020 2020 2020 2072  d).            r
+00007260: 6574 7572 6e0a 2020 2020 2020 2020 6966  eturn.        if
+00007270: 2065 7665 6e74 2e6b 6579 2829 203d 3d20   event.key() == 
+00007280: 5174 2e4b 6579 2e4b 6579 5f50 6167 6544  Qt.Key.Key_PageD
+00007290: 6f77 6e20 616e 6420 6d6f 6469 6669 6572  own and modifier
+000072a0: 203d 3d20 5174 2e43 6f6e 7472 6f6c 4d6f   == Qt.ControlMo
+000072b0: 6469 6669 6572 3a0a 2020 2020 2020 2020  difier:.        
+000072c0: 2020 2020 636d 6420 3d20 7b7d 0a20 2020      cmd = {}.   
+000072d0: 2020 2020 2020 2020 2063 6d64 5b22 636d           cmd["cm
+000072e0: 6422 5d20 3d20 224e 4558 5453 504f 5422  d"] = "NEXTSPOT"
+000072f0: 0a20 2020 2020 2020 2020 2020 2063 6d64  .            cmd
+00007300: 5b22 7374 6174 696f 6e22 5d20 3d20 706c  ["station"] = pl
+00007310: 6174 666f 726d 2e6e 6f64 6528 290a 2020  atform.node().  
+00007320: 2020 2020 2020 2020 2020 7365 6c66 2e6d            self.m
+00007330: 756c 7469 6361 7374 5f69 6e74 6572 6661  ulticast_interfa
+00007340: 6365 2e73 656e 645f 6173 5f6a 736f 6e28  ce.send_as_json(
+00007350: 636d 6429 0a20 2020 2020 2020 2020 2020  cmd).           
+00007360: 2072 6574 7572 6e0a 2020 2020 2020 2020   return.        
+00007370: 6966 2065 7665 6e74 2e6b 6579 2829 203d  if event.key() =
+00007380: 3d20 5174 2e4b 6579 2e4b 6579 5f50 6167  = Qt.Key.Key_Pag
+00007390: 6555 7020 616e 6420 6d6f 6469 6669 6572  eUp and modifier
+000073a0: 2021 3d20 5174 2e43 6f6e 7472 6f6c 4d6f   != Qt.ControlMo
+000073b0: 6469 6669 6572 3a0a 2020 2020 2020 2020  difier:.        
+000073c0: 2020 2020 6966 2073 656c 662e 6377 2069      if self.cw i
+000073d0: 7320 6e6f 7420 4e6f 6e65 3a0a 2020 2020  s not None:.    
+000073e0: 2020 2020 2020 2020 2020 2020 6966 2073              if s
+000073f0: 656c 662e 6377 2e73 6572 7665 7274 7970  elf.cw.servertyp
+00007400: 6520 3d3d 2031 3a0a 2020 2020 2020 2020  e == 1:.        
+00007410: 2020 2020 2020 2020 2020 2020 7365 6c66              self
+00007420: 2e63 772e 7370 6565 6420 2b3d 2031 0a20  .cw.speed += 1. 
 00007430: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00007440: 2020 7365 6c66 2e63 775f 7370 6565 642e    self.cw_speed.
-00007450: 7365 7456 616c 7565 2873 656c 662e 6377  setValue(self.cw
-00007460: 2e73 7065 6564 290a 2020 2020 2020 2020  .speed).        
-00007470: 2020 2020 2020 2020 2020 2020 7365 6c66              self
-00007480: 2e63 772e 7365 6e64 6377 2866 225c 7831  .cw.sendcw(f"\x1
-00007490: 6232 7b73 656c 662e 6377 2e73 7065 6564  b2{self.cw.speed
-000074a0: 7d22 290a 2020 2020 2020 2020 2020 2020  }").            
-000074b0: 2020 2020 2020 2020 7265 7475 726e 0a20          return. 
-000074c0: 2020 2020 2020 2069 6620 6576 656e 742e         if event.
-000074d0: 6b65 7928 2920 3d3d 2051 742e 4b65 792e  key() == Qt.Key.
-000074e0: 4b65 795f 5061 6765 446f 776e 2061 6e64  Key_PageDown and
-000074f0: 206d 6f64 6966 6965 7220 213d 2051 742e   modifier != Qt.
-00007500: 436f 6e74 726f 6c4d 6f64 6966 6965 723a  ControlModifier:
-00007510: 0a20 2020 2020 2020 2020 2020 2069 6620  .            if 
-00007520: 7365 6c66 2e63 7720 6973 206e 6f74 204e  self.cw is not N
-00007530: 6f6e 653a 0a20 2020 2020 2020 2020 2020  one:.           
-00007540: 2020 2020 2069 6620 7365 6c66 2e63 772e       if self.cw.
-00007550: 7365 7276 6572 7479 7065 203d 3d20 313a  servertype == 1:
-00007560: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00007570: 2020 2020 2073 656c 662e 6377 2e73 7065       self.cw.spe
-00007580: 6564 202d 3d20 310a 2020 2020 2020 2020  ed -= 1.        
-00007590: 2020 2020 2020 2020 2020 2020 7365 6c66              self
-000075a0: 2e63 775f 7370 6565 642e 7365 7456 616c  .cw_speed.setVal
-000075b0: 7565 2873 656c 662e 6377 2e73 7065 6564  ue(self.cw.speed
-000075c0: 290a 2020 2020 2020 2020 2020 2020 2020  ).              
-000075d0: 2020 2020 2020 7365 6c66 2e63 772e 7365        self.cw.se
-000075e0: 6e64 6377 2866 225c 7831 6232 7b73 656c  ndcw(f"\x1b2{sel
-000075f0: 662e 6377 2e73 7065 6564 7d22 290a 2020  f.cw.speed}").  
+00007440: 2020 2073 656c 662e 6377 5f73 7065 6564     self.cw_speed
+00007450: 2e73 6574 5661 6c75 6528 7365 6c66 2e63  .setValue(self.c
+00007460: 772e 7370 6565 6429 0a20 2020 2020 2020  w.speed).       
+00007470: 2020 2020 2020 2020 2020 2020 2073 656c               sel
+00007480: 662e 6377 2e73 656e 6463 7728 6622 5c78  f.cw.sendcw(f"\x
+00007490: 3162 327b 7365 6c66 2e63 772e 7370 6565  1b2{self.cw.spee
+000074a0: 647d 2229 0a20 2020 2020 2020 2020 2020  d}").           
+000074b0: 2020 2020 2020 2020 2072 6574 7572 6e0a           return.
+000074c0: 2020 2020 2020 2020 6966 2065 7665 6e74          if event
+000074d0: 2e6b 6579 2829 203d 3d20 5174 2e4b 6579  .key() == Qt.Key
+000074e0: 2e4b 6579 5f50 6167 6544 6f77 6e20 616e  .Key_PageDown an
+000074f0: 6420 6d6f 6469 6669 6572 2021 3d20 5174  d modifier != Qt
+00007500: 2e43 6f6e 7472 6f6c 4d6f 6469 6669 6572  .ControlModifier
+00007510: 3a0a 2020 2020 2020 2020 2020 2020 6966  :.            if
+00007520: 2073 656c 662e 6377 2069 7320 6e6f 7420   self.cw is not 
+00007530: 4e6f 6e65 3a0a 2020 2020 2020 2020 2020  None:.          
+00007540: 2020 2020 2020 6966 2073 656c 662e 6377        if self.cw
+00007550: 2e73 6572 7665 7274 7970 6520 3d3d 2031  .servertype == 1
+00007560: 3a0a 2020 2020 2020 2020 2020 2020 2020  :.              
+00007570: 2020 2020 2020 7365 6c66 2e63 772e 7370        self.cw.sp
+00007580: 6565 6420 2d3d 2031 0a20 2020 2020 2020  eed -= 1.       
+00007590: 2020 2020 2020 2020 2020 2020 2073 656c               sel
+000075a0: 662e 6377 5f73 7065 6564 2e73 6574 5661  f.cw_speed.setVa
+000075b0: 6c75 6528 7365 6c66 2e63 772e 7370 6565  lue(self.cw.spee
+000075c0: 6429 0a20 2020 2020 2020 2020 2020 2020  d).             
+000075d0: 2020 2020 2020 2073 656c 662e 6377 2e73         self.cw.s
+000075e0: 656e 6463 7728 6622 5c78 3162 327b 7365  endcw(f"\x1b2{se
+000075f0: 6c66 2e63 772e 7370 6565 647d 2229 0a20  lf.cw.speed}"). 
 00007600: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00007610: 2020 7265 7475 726e 0a20 2020 2020 2020    return.       
-00007620: 2023 2069 6620 6576 656e 742e 6b65 7928   # if event.key(
-00007630: 2920 3d3d 2051 742e 4b65 792e 4b65 795f  ) == Qt.Key.Key_
-00007640: 456e 7465 723a 0a20 2020 2020 2020 2023  Enter:.        #
-00007650: 2020 2020 2073 656c 662e 7361 7665 5f63       self.save_c
-00007660: 6f6e 7461 6374 2829 0a20 2020 2020 2020  ontact().       
-00007670: 2069 6620 6576 656e 742e 6b65 7928 2920   if event.key() 
-00007680: 3d3d 2051 742e 4b65 792e 4b65 795f 5461  == Qt.Key.Key_Ta
-00007690: 6220 6f72 2065 7665 6e74 2e6b 6579 2829  b or event.key()
-000076a0: 203d 3d20 5174 2e4b 6579 2e4b 6579 5f42   == Qt.Key.Key_B
-000076b0: 6163 6b74 6162 3a0a 2020 2020 2020 2020  acktab:.        
-000076c0: 2020 2020 6966 2073 656c 662e 7365 6e74      if self.sent
-000076d0: 2e68 6173 466f 6375 7328 293a 0a20 2020  .hasFocus():.   
-000076e0: 2020 2020 2020 2020 2020 2020 206c 6f67               log
-000076f0: 6765 722e 6465 6275 6728 2246 726f 6d20  ger.debug("From 
-00007700: 7365 6e74 2229 0a20 2020 2020 2020 2020  sent").         
-00007710: 2020 2020 2020 2069 6620 6d6f 6469 6669         if modifi
-00007720: 6572 203d 3d20 5174 2e53 6869 6674 4d6f  er == Qt.ShiftMo
-00007730: 6469 6669 6572 3a0a 2020 2020 2020 2020  difier:.        
-00007740: 2020 2020 2020 2020 2020 2020 7072 6576              prev
-00007750: 5f74 6162 203d 2073 656c 662e 7461 625f  _tab = self.tab_
-00007760: 7072 6576 2e67 6574 2873 656c 662e 7365  prev.get(self.se
-00007770: 6e74 290a 2020 2020 2020 2020 2020 2020  nt).            
-00007780: 2020 2020 2020 2020 7072 6576 5f74 6162          prev_tab
-00007790: 2e73 6574 466f 6375 7328 290a 2020 2020  .setFocus().    
+00007610: 2020 2072 6574 7572 6e0a 2020 2020 2020     return.      
+00007620: 2020 2320 6966 2065 7665 6e74 2e6b 6579    # if event.key
+00007630: 2829 203d 3d20 5174 2e4b 6579 2e4b 6579  () == Qt.Key.Key
+00007640: 5f45 6e74 6572 3a0a 2020 2020 2020 2020  _Enter:.        
+00007650: 2320 2020 2020 7365 6c66 2e73 6176 655f  #     self.save_
+00007660: 636f 6e74 6163 7428 290a 2020 2020 2020  contact().      
+00007670: 2020 6966 2065 7665 6e74 2e6b 6579 2829    if event.key()
+00007680: 203d 3d20 5174 2e4b 6579 2e4b 6579 5f54   == Qt.Key.Key_T
+00007690: 6162 206f 7220 6576 656e 742e 6b65 7928  ab or event.key(
+000076a0: 2920 3d3d 2051 742e 4b65 792e 4b65 795f  ) == Qt.Key.Key_
+000076b0: 4261 636b 7461 623a 0a20 2020 2020 2020  Backtab:.       
+000076c0: 2020 2020 2069 6620 7365 6c66 2e73 656e       if self.sen
+000076d0: 742e 6861 7346 6f63 7573 2829 3a0a 2020  t.hasFocus():.  
+000076e0: 2020 2020 2020 2020 2020 2020 2020 6c6f                lo
+000076f0: 6767 6572 2e64 6562 7567 2822 4672 6f6d  gger.debug("From
+00007700: 2073 656e 7422 290a 2020 2020 2020 2020   sent").        
+00007710: 2020 2020 2020 2020 6966 206d 6f64 6966          if modif
+00007720: 6965 7220 3d3d 2051 742e 5368 6966 744d  ier == Qt.ShiftM
+00007730: 6f64 6966 6965 723a 0a20 2020 2020 2020  odifier:.       
+00007740: 2020 2020 2020 2020 2020 2020 2070 7265               pre
+00007750: 765f 7461 6220 3d20 7365 6c66 2e74 6162  v_tab = self.tab
+00007760: 5f70 7265 762e 6765 7428 7365 6c66 2e73  _prev.get(self.s
+00007770: 656e 7429 0a20 2020 2020 2020 2020 2020  ent).           
+00007780: 2020 2020 2020 2020 2070 7265 765f 7461           prev_ta
+00007790: 622e 7365 7446 6f63 7573 2829 0a20 2020  b.setFocus().   
 000077a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000077b0: 7072 6576 5f74 6162 2e64 6573 656c 6563  prev_tab.deselec
-000077c0: 7428 290a 2020 2020 2020 2020 2020 2020  t().            
-000077d0: 2020 2020 2020 2020 7072 6576 5f74 6162          prev_tab
-000077e0: 2e65 6e64 2846 616c 7365 290a 2020 2020  .end(False).    
-000077f0: 2020 2020 2020 2020 2020 2020 656c 7365              else
-00007800: 3a0a 2020 2020 2020 2020 2020 2020 2020  :.              
-00007810: 2020 2020 2020 6e65 7874 5f74 6162 203d        next_tab =
-00007820: 2073 656c 662e 7461 625f 6e65 7874 2e67   self.tab_next.g
-00007830: 6574 2873 656c 662e 7365 6e74 290a 2020  et(self.sent).  
+000077b0: 2070 7265 765f 7461 622e 6465 7365 6c65   prev_tab.desele
+000077c0: 6374 2829 0a20 2020 2020 2020 2020 2020  ct().           
+000077d0: 2020 2020 2020 2020 2070 7265 765f 7461           prev_ta
+000077e0: 622e 656e 6428 4661 6c73 6529 0a20 2020  b.end(False).   
+000077f0: 2020 2020 2020 2020 2020 2020 2065 6c73               els
+00007800: 653a 0a20 2020 2020 2020 2020 2020 2020  e:.             
+00007810: 2020 2020 2020 206e 6578 745f 7461 6220         next_tab 
+00007820: 3d20 7365 6c66 2e74 6162 5f6e 6578 742e  = self.tab_next.
+00007830: 6765 7428 7365 6c66 2e73 656e 7429 0a20  get(self.sent). 
 00007840: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00007850: 2020 6e65 7874 5f74 6162 2e73 6574 466f    next_tab.setFo
-00007860: 6375 7328 290a 2020 2020 2020 2020 2020  cus().          
-00007870: 2020 2020 2020 2020 2020 6e65 7874 5f74            next_t
-00007880: 6162 2e64 6573 656c 6563 7428 290a 2020  ab.deselect().  
+00007850: 2020 206e 6578 745f 7461 622e 7365 7446     next_tab.setF
+00007860: 6f63 7573 2829 0a20 2020 2020 2020 2020  ocus().         
+00007870: 2020 2020 2020 2020 2020 206e 6578 745f             next_
+00007880: 7461 622e 6465 7365 6c65 6374 2829 0a20  tab.deselect(). 
 00007890: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000078a0: 2020 6e65 7874 5f74 6162 2e65 6e64 2846    next_tab.end(F
-000078b0: 616c 7365 290a 2020 2020 2020 2020 2020  alse).          
-000078c0: 2020 2020 2020 7265 7475 726e 0a20 2020        return.   
-000078d0: 2020 2020 2020 2020 2069 6620 7365 6c66           if self
-000078e0: 2e72 6563 6569 7665 2e68 6173 466f 6375  .receive.hasFocu
-000078f0: 7328 293a 0a20 2020 2020 2020 2020 2020  s():.           
-00007900: 2020 2020 206c 6f67 6765 722e 6465 6275       logger.debu
-00007910: 6728 2246 726f 6d20 7265 6365 6976 6522  g("From receive"
-00007920: 290a 2020 2020 2020 2020 2020 2020 2020  ).              
-00007930: 2020 6966 206d 6f64 6966 6965 7220 3d3d    if modifier ==
-00007940: 2051 742e 5368 6966 744d 6f64 6966 6965   Qt.ShiftModifie
-00007950: 723a 0a20 2020 2020 2020 2020 2020 2020  r:.             
-00007960: 2020 2020 2020 2070 7265 765f 7461 6220         prev_tab 
-00007970: 3d20 7365 6c66 2e74 6162 5f70 7265 762e  = self.tab_prev.
-00007980: 6765 7428 7365 6c66 2e72 6563 6569 7665  get(self.receive
-00007990: 290a 2020 2020 2020 2020 2020 2020 2020  ).              
-000079a0: 2020 2020 2020 7072 6576 5f74 6162 2e73        prev_tab.s
-000079b0: 6574 466f 6375 7328 290a 2020 2020 2020  etFocus().      
-000079c0: 2020 2020 2020 2020 2020 2020 2020 7072                pr
-000079d0: 6576 5f74 6162 2e64 6573 656c 6563 7428  ev_tab.deselect(
-000079e0: 290a 2020 2020 2020 2020 2020 2020 2020  ).              
-000079f0: 2020 2020 2020 7072 6576 5f74 6162 2e65        prev_tab.e
-00007a00: 6e64 2846 616c 7365 290a 2020 2020 2020  nd(False).      
-00007a10: 2020 2020 2020 2020 2020 656c 7365 3a0a            else:.
-00007a20: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00007a30: 2020 2020 6e65 7874 5f74 6162 203d 2073      next_tab = s
-00007a40: 656c 662e 7461 625f 6e65 7874 2e67 6574  elf.tab_next.get
-00007a50: 2873 656c 662e 7265 6365 6976 6529 0a20  (self.receive). 
+000078a0: 2020 206e 6578 745f 7461 622e 656e 6428     next_tab.end(
+000078b0: 4661 6c73 6529 0a20 2020 2020 2020 2020  False).         
+000078c0: 2020 2020 2020 2072 6574 7572 6e0a 2020         return.  
+000078d0: 2020 2020 2020 2020 2020 6966 2073 656c            if sel
+000078e0: 662e 7265 6365 6976 652e 6861 7346 6f63  f.receive.hasFoc
+000078f0: 7573 2829 3a0a 2020 2020 2020 2020 2020  us():.          
+00007900: 2020 2020 2020 6c6f 6767 6572 2e64 6562        logger.deb
+00007910: 7567 2822 4672 6f6d 2072 6563 6569 7665  ug("From receive
+00007920: 2229 0a20 2020 2020 2020 2020 2020 2020  ").             
+00007930: 2020 2069 6620 6d6f 6469 6669 6572 203d     if modifier =
+00007940: 3d20 5174 2e53 6869 6674 4d6f 6469 6669  = Qt.ShiftModifi
+00007950: 6572 3a0a 2020 2020 2020 2020 2020 2020  er:.            
+00007960: 2020 2020 2020 2020 7072 6576 5f74 6162          prev_tab
+00007970: 203d 2073 656c 662e 7461 625f 7072 6576   = self.tab_prev
+00007980: 2e67 6574 2873 656c 662e 7265 6365 6976  .get(self.receiv
+00007990: 6529 0a20 2020 2020 2020 2020 2020 2020  e).             
+000079a0: 2020 2020 2020 2070 7265 765f 7461 622e         prev_tab.
+000079b0: 7365 7446 6f63 7573 2829 0a20 2020 2020  setFocus().     
+000079c0: 2020 2020 2020 2020 2020 2020 2020 2070                 p
+000079d0: 7265 765f 7461 622e 6465 7365 6c65 6374  rev_tab.deselect
+000079e0: 2829 0a20 2020 2020 2020 2020 2020 2020  ().             
+000079f0: 2020 2020 2020 2070 7265 765f 7461 622e         prev_tab.
+00007a00: 656e 6428 4661 6c73 6529 0a20 2020 2020  end(False).     
+00007a10: 2020 2020 2020 2020 2020 2065 6c73 653a             else:
+00007a20: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00007a30: 2020 2020 206e 6578 745f 7461 6220 3d20       next_tab = 
+00007a40: 7365 6c66 2e74 6162 5f6e 6578 742e 6765  self.tab_next.ge
+00007a50: 7428 7365 6c66 2e72 6563 6569 7665 290a  t(self.receive).
 00007a60: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00007a70: 2020 206e 6578 745f 7461 622e 7365 7446     next_tab.setF
-00007a80: 6f63 7573 2829 0a20 2020 2020 2020 2020  ocus().         
-00007a90: 2020 2020 2020 2020 2020 206e 6578 745f             next_
-00007aa0: 7461 622e 6465 7365 6c65 6374 2829 0a20  tab.deselect(). 
+00007a70: 2020 2020 6e65 7874 5f74 6162 2e73 6574      next_tab.set
+00007a80: 466f 6375 7328 290a 2020 2020 2020 2020  Focus().        
+00007a90: 2020 2020 2020 2020 2020 2020 6e65 7874              next
+00007aa0: 5f74 6162 2e64 6573 656c 6563 7428 290a  _tab.deselect().
 00007ab0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00007ac0: 2020 206e 6578 745f 7461 622e 656e 6428     next_tab.end(
-00007ad0: 4661 6c73 6529 0a20 2020 2020 2020 2020  False).         
-00007ae0: 2020 2020 2020 2072 6574 7572 6e0a 2020         return.  
-00007af0: 2020 2020 2020 2020 2020 6966 2073 656c            if sel
-00007b00: 662e 6f74 6865 725f 312e 6861 7346 6f63  f.other_1.hasFoc
-00007b10: 7573 2829 3a0a 2020 2020 2020 2020 2020  us():.          
-00007b20: 2020 2020 2020 6c6f 6767 6572 2e64 6562        logger.deb
-00007b30: 7567 2822 4672 6f6d 206f 7468 6572 5f31  ug("From other_1
-00007b40: 2229 0a20 2020 2020 2020 2020 2020 2020  ").             
-00007b50: 2020 2069 6620 6d6f 6469 6669 6572 203d     if modifier =
-00007b60: 3d20 5174 2e53 6869 6674 4d6f 6469 6669  = Qt.ShiftModifi
-00007b70: 6572 3a0a 2020 2020 2020 2020 2020 2020  er:.            
-00007b80: 2020 2020 2020 2020 7072 6576 5f74 6162          prev_tab
-00007b90: 203d 2073 656c 662e 7461 625f 7072 6576   = self.tab_prev
-00007ba0: 2e67 6574 2873 656c 662e 6f74 6865 725f  .get(self.other_
-00007bb0: 3129 0a20 2020 2020 2020 2020 2020 2020  1).             
-00007bc0: 2020 2020 2020 2070 7265 765f 7461 622e         prev_tab.
-00007bd0: 7365 7446 6f63 7573 2829 0a20 2020 2020  setFocus().     
-00007be0: 2020 2020 2020 2020 2020 2020 2020 2070                 p
-00007bf0: 7265 765f 7461 622e 6465 7365 6c65 6374  rev_tab.deselect
-00007c00: 2829 0a20 2020 2020 2020 2020 2020 2020  ().             
-00007c10: 2020 2020 2020 2070 7265 765f 7461 622e         prev_tab.
-00007c20: 656e 6428 4661 6c73 6529 0a20 2020 2020  end(False).     
-00007c30: 2020 2020 2020 2020 2020 2065 6c73 653a             else:
-00007c40: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00007c50: 2020 2020 206e 6578 745f 7461 6220 3d20       next_tab = 
-00007c60: 7365 6c66 2e74 6162 5f6e 6578 742e 6765  self.tab_next.ge
-00007c70: 7428 7365 6c66 2e6f 7468 6572 5f31 290a  t(self.other_1).
-00007c80: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00007c90: 2020 2020 6e65 7874 5f74 6162 2e73 6574      next_tab.set
-00007ca0: 466f 6375 7328 290a 2020 2020 2020 2020  Focus().        
-00007cb0: 2020 2020 2020 2020 2020 2020 6e65 7874              next
-00007cc0: 5f74 6162 2e64 6573 656c 6563 7428 290a  _tab.deselect().
-00007cd0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00007ce0: 2020 2020 6e65 7874 5f74 6162 2e65 6e64      next_tab.end
-00007cf0: 2846 616c 7365 290a 2020 2020 2020 2020  (False).        
-00007d00: 2020 2020 2020 2020 7265 7475 726e 0a20          return. 
-00007d10: 2020 2020 2020 2020 2020 2069 6620 7365             if se
-00007d20: 6c66 2e6f 7468 6572 5f32 2e68 6173 466f  lf.other_2.hasFo
-00007d30: 6375 7328 293a 0a20 2020 2020 2020 2020  cus():.         
-00007d40: 2020 2020 2020 206c 6f67 6765 722e 6465         logger.de
-00007d50: 6275 6728 2246 726f 6d20 6f74 6865 725f  bug("From other_
-00007d60: 3222 290a 2020 2020 2020 2020 2020 2020  2").            
-00007d70: 2020 2020 6966 206d 6f64 6966 6965 7220      if modifier 
-00007d80: 3d3d 2051 742e 5368 6966 744d 6f64 6966  == Qt.ShiftModif
-00007d90: 6965 723a 0a20 2020 2020 2020 2020 2020  ier:.           
-00007da0: 2020 2020 2020 2020 2070 7265 765f 7461           prev_ta
-00007db0: 6220 3d20 7365 6c66 2e74 6162 5f70 7265  b = self.tab_pre
-00007dc0: 762e 6765 7428 7365 6c66 2e6f 7468 6572  v.get(self.other
-00007dd0: 5f32 290a 2020 2020 2020 2020 2020 2020  _2).            
-00007de0: 2020 2020 2020 2020 7072 6576 5f74 6162          prev_tab
-00007df0: 2e73 6574 466f 6375 7328 290a 2020 2020  .setFocus().    
+00007ac0: 2020 2020 6e65 7874 5f74 6162 2e65 6e64      next_tab.end
+00007ad0: 2846 616c 7365 290a 2020 2020 2020 2020  (False).        
+00007ae0: 2020 2020 2020 2020 7265 7475 726e 0a20          return. 
+00007af0: 2020 2020 2020 2020 2020 2069 6620 7365             if se
+00007b00: 6c66 2e6f 7468 6572 5f31 2e68 6173 466f  lf.other_1.hasFo
+00007b10: 6375 7328 293a 0a20 2020 2020 2020 2020  cus():.         
+00007b20: 2020 2020 2020 206c 6f67 6765 722e 6465         logger.de
+00007b30: 6275 6728 2246 726f 6d20 6f74 6865 725f  bug("From other_
+00007b40: 3122 290a 2020 2020 2020 2020 2020 2020  1").            
+00007b50: 2020 2020 6966 206d 6f64 6966 6965 7220      if modifier 
+00007b60: 3d3d 2051 742e 5368 6966 744d 6f64 6966  == Qt.ShiftModif
+00007b70: 6965 723a 0a20 2020 2020 2020 2020 2020  ier:.           
+00007b80: 2020 2020 2020 2020 2070 7265 765f 7461           prev_ta
+00007b90: 6220 3d20 7365 6c66 2e74 6162 5f70 7265  b = self.tab_pre
+00007ba0: 762e 6765 7428 7365 6c66 2e6f 7468 6572  v.get(self.other
+00007bb0: 5f31 290a 2020 2020 2020 2020 2020 2020  _1).            
+00007bc0: 2020 2020 2020 2020 7072 6576 5f74 6162          prev_tab
+00007bd0: 2e73 6574 466f 6375 7328 290a 2020 2020  .setFocus().    
+00007be0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00007bf0: 7072 6576 5f74 6162 2e64 6573 656c 6563  prev_tab.deselec
+00007c00: 7428 290a 2020 2020 2020 2020 2020 2020  t().            
+00007c10: 2020 2020 2020 2020 7072 6576 5f74 6162          prev_tab
+00007c20: 2e65 6e64 2846 616c 7365 290a 2020 2020  .end(False).    
+00007c30: 2020 2020 2020 2020 2020 2020 656c 7365              else
+00007c40: 3a0a 2020 2020 2020 2020 2020 2020 2020  :.              
+00007c50: 2020 2020 2020 6e65 7874 5f74 6162 203d        next_tab =
+00007c60: 2073 656c 662e 7461 625f 6e65 7874 2e67   self.tab_next.g
+00007c70: 6574 2873 656c 662e 6f74 6865 725f 3129  et(self.other_1)
+00007c80: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00007c90: 2020 2020 206e 6578 745f 7461 622e 7365       next_tab.se
+00007ca0: 7446 6f63 7573 2829 0a20 2020 2020 2020  tFocus().       
+00007cb0: 2020 2020 2020 2020 2020 2020 206e 6578               nex
+00007cc0: 745f 7461 622e 6465 7365 6c65 6374 2829  t_tab.deselect()
+00007cd0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00007ce0: 2020 2020 206e 6578 745f 7461 622e 656e       next_tab.en
+00007cf0: 6428 4661 6c73 6529 0a20 2020 2020 2020  d(False).       
+00007d00: 2020 2020 2020 2020 2072 6574 7572 6e0a           return.
+00007d10: 2020 2020 2020 2020 2020 2020 6966 2073              if s
+00007d20: 656c 662e 6f74 6865 725f 322e 6861 7346  elf.other_2.hasF
+00007d30: 6f63 7573 2829 3a0a 2020 2020 2020 2020  ocus():.        
+00007d40: 2020 2020 2020 2020 6c6f 6767 6572 2e64          logger.d
+00007d50: 6562 7567 2822 4672 6f6d 206f 7468 6572  ebug("From other
+00007d60: 5f32 2229 0a20 2020 2020 2020 2020 2020  _2").           
+00007d70: 2020 2020 2069 6620 6d6f 6469 6669 6572       if modifier
+00007d80: 203d 3d20 5174 2e53 6869 6674 4d6f 6469   == Qt.ShiftModi
+00007d90: 6669 6572 3a0a 2020 2020 2020 2020 2020  fier:.          
+00007da0: 2020 2020 2020 2020 2020 7072 6576 5f74            prev_t
+00007db0: 6162 203d 2073 656c 662e 7461 625f 7072  ab = self.tab_pr
+00007dc0: 6576 2e67 6574 2873 656c 662e 6f74 6865  ev.get(self.othe
+00007dd0: 725f 3229 0a20 2020 2020 2020 2020 2020  r_2).           
+00007de0: 2020 2020 2020 2020 2070 7265 765f 7461           prev_ta
+00007df0: 622e 7365 7446 6f63 7573 2829 0a20 2020  b.setFocus().   
 00007e00: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00007e10: 7072 6576 5f74 6162 2e64 6573 656c 6563  prev_tab.deselec
-00007e20: 7428 290a 2020 2020 2020 2020 2020 2020  t().            
-00007e30: 2020 2020 2020 2020 7072 6576 5f74 6162          prev_tab
-00007e40: 2e65 6e64 2846 616c 7365 290a 2020 2020  .end(False).    
-00007e50: 2020 2020 2020 2020 2020 2020 656c 7365              else
-00007e60: 3a0a 2020 2020 2020 2020 2020 2020 2020  :.              
-00007e70: 2020 2020 2020 6e65 7874 5f74 6162 203d        next_tab =
-00007e80: 2073 656c 662e 7461 625f 6e65 7874 2e67   self.tab_next.g
-00007e90: 6574 2873 656c 662e 6f74 6865 725f 3229  et(self.other_2)
-00007ea0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00007eb0: 2020 2020 206e 6578 745f 7461 622e 7365       next_tab.se
-00007ec0: 7446 6f63 7573 2829 0a20 2020 2020 2020  tFocus().       
-00007ed0: 2020 2020 2020 2020 2020 2020 206e 6578               nex
-00007ee0: 745f 7461 622e 6465 7365 6c65 6374 2829  t_tab.deselect()
-00007ef0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00007f00: 2020 2020 206e 6578 745f 7461 622e 656e       next_tab.en
-00007f10: 6428 4661 6c73 6529 0a20 2020 2020 2020  d(False).       
-00007f20: 2020 2020 2020 2020 2072 6574 7572 6e0a           return.
-00007f30: 2020 2020 2020 2020 2020 2020 6966 2073              if s
-00007f40: 656c 662e 6361 6c6c 7369 676e 2e68 6173  elf.callsign.has
-00007f50: 466f 6375 7328 293a 0a20 2020 2020 2020  Focus():.       
-00007f60: 2020 2020 2020 2020 206c 6f67 6765 722e           logger.
-00007f70: 6465 6275 6728 2246 726f 6d20 6361 6c6c  debug("From call
-00007f80: 7369 676e 2229 0a20 2020 2020 2020 2020  sign").         
-00007f90: 2020 2020 2020 2069 6620 6d6f 6469 6669         if modifi
-00007fa0: 6572 203d 3d20 5174 2e53 6869 6674 4d6f  er == Qt.ShiftMo
-00007fb0: 6469 6669 6572 3a0a 2020 2020 2020 2020  difier:.        
-00007fc0: 2020 2020 2020 2020 2020 2020 7072 6576              prev
-00007fd0: 5f74 6162 203d 2073 656c 662e 7461 625f  _tab = self.tab_
-00007fe0: 7072 6576 2e67 6574 2873 656c 662e 6361  prev.get(self.ca
-00007ff0: 6c6c 7369 676e 290a 2020 2020 2020 2020  llsign).        
-00008000: 2020 2020 2020 2020 2020 2020 7072 6576              prev
-00008010: 5f74 6162 2e73 6574 466f 6375 7328 290a  _tab.setFocus().
-00008020: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00008030: 2020 2020 7072 6576 5f74 6162 2e64 6573      prev_tab.des
-00008040: 656c 6563 7428 290a 2020 2020 2020 2020  elect().        
-00008050: 2020 2020 2020 2020 2020 2020 7072 6576              prev
-00008060: 5f74 6162 2e65 6e64 2846 616c 7365 290a  _tab.end(False).
-00008070: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00008080: 656c 7365 3a0a 2020 2020 2020 2020 2020  else:.          
-00008090: 2020 2020 2020 2020 2020 7465 7874 203d            text =
-000080a0: 2073 656c 662e 6361 6c6c 7369 676e 2e74   self.callsign.t
-000080b0: 6578 7428 290a 2020 2020 2020 2020 2020  ext().          
-000080c0: 2020 2020 2020 2020 2020 7465 7874 203d            text =
-000080d0: 2074 6578 742e 7570 7065 7228 290a 2020   text.upper().  
+00007e10: 2070 7265 765f 7461 622e 6465 7365 6c65   prev_tab.desele
+00007e20: 6374 2829 0a20 2020 2020 2020 2020 2020  ct().           
+00007e30: 2020 2020 2020 2020 2070 7265 765f 7461           prev_ta
+00007e40: 622e 656e 6428 4661 6c73 6529 0a20 2020  b.end(False).   
+00007e50: 2020 2020 2020 2020 2020 2020 2065 6c73               els
+00007e60: 653a 0a20 2020 2020 2020 2020 2020 2020  e:.             
+00007e70: 2020 2020 2020 206e 6578 745f 7461 6220         next_tab 
+00007e80: 3d20 7365 6c66 2e74 6162 5f6e 6578 742e  = self.tab_next.
+00007e90: 6765 7428 7365 6c66 2e6f 7468 6572 5f32  get(self.other_2
+00007ea0: 290a 2020 2020 2020 2020 2020 2020 2020  ).              
+00007eb0: 2020 2020 2020 6e65 7874 5f74 6162 2e73        next_tab.s
+00007ec0: 6574 466f 6375 7328 290a 2020 2020 2020  etFocus().      
+00007ed0: 2020 2020 2020 2020 2020 2020 2020 6e65                ne
+00007ee0: 7874 5f74 6162 2e64 6573 656c 6563 7428  xt_tab.deselect(
+00007ef0: 290a 2020 2020 2020 2020 2020 2020 2020  ).              
+00007f00: 2020 2020 2020 6e65 7874 5f74 6162 2e65        next_tab.e
+00007f10: 6e64 2846 616c 7365 290a 2020 2020 2020  nd(False).      
+00007f20: 2020 2020 2020 2020 2020 7265 7475 726e            return
+00007f30: 0a20 2020 2020 2020 2020 2020 2069 6620  .            if 
+00007f40: 7365 6c66 2e63 616c 6c73 6967 6e2e 6861  self.callsign.ha
+00007f50: 7346 6f63 7573 2829 3a0a 2020 2020 2020  sFocus():.      
+00007f60: 2020 2020 2020 2020 2020 6c6f 6767 6572            logger
+00007f70: 2e64 6562 7567 2822 4672 6f6d 2063 616c  .debug("From cal
+00007f80: 6c73 6967 6e22 290a 2020 2020 2020 2020  lsign").        
+00007f90: 2020 2020 2020 2020 6966 206d 6f64 6966          if modif
+00007fa0: 6965 7220 3d3d 2051 742e 5368 6966 744d  ier == Qt.ShiftM
+00007fb0: 6f64 6966 6965 723a 0a20 2020 2020 2020  odifier:.       
+00007fc0: 2020 2020 2020 2020 2020 2020 2070 7265               pre
+00007fd0: 765f 7461 6220 3d20 7365 6c66 2e74 6162  v_tab = self.tab
+00007fe0: 5f70 7265 762e 6765 7428 7365 6c66 2e63  _prev.get(self.c
+00007ff0: 616c 6c73 6967 6e29 0a20 2020 2020 2020  allsign).       
+00008000: 2020 2020 2020 2020 2020 2020 2070 7265               pre
+00008010: 765f 7461 622e 7365 7446 6f63 7573 2829  v_tab.setFocus()
+00008020: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00008030: 2020 2020 2070 7265 765f 7461 622e 6465       prev_tab.de
+00008040: 7365 6c65 6374 2829 0a20 2020 2020 2020  select().       
+00008050: 2020 2020 2020 2020 2020 2020 2070 7265               pre
+00008060: 765f 7461 622e 656e 6428 4661 6c73 6529  v_tab.end(False)
+00008070: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00008080: 2065 6c73 653a 0a20 2020 2020 2020 2020   else:.         
+00008090: 2020 2020 2020 2020 2020 2074 6578 7420             text 
+000080a0: 3d20 7365 6c66 2e63 616c 6c73 6967 6e2e  = self.callsign.
+000080b0: 7465 7874 2829 0a20 2020 2020 2020 2020  text().         
+000080c0: 2020 2020 2020 2020 2020 2074 6578 7420             text 
+000080d0: 3d20 7465 7874 2e75 7070 6572 2829 0a20  = text.upper(). 
 000080e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000080f0: 2020 5f74 6865 7468 7265 6164 203d 2074    _thethread = t
-00008100: 6872 6561 6469 6e67 2e54 6872 6561 6428  hreading.Thread(
-00008110: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00008120: 2020 2020 2020 2020 2074 6172 6765 743d           target=
-00008130: 7365 6c66 2e63 6865 636b 5f63 616c 6c73  self.check_calls
-00008140: 6967 6e32 2c0a 2020 2020 2020 2020 2020  ign2,.          
-00008150: 2020 2020 2020 2020 2020 2020 2020 6172                ar
-00008160: 6773 3d28 7465 7874 2c29 2c0a 2020 2020  gs=(text,),.    
+000080f0: 2020 205f 7468 6574 6872 6561 6420 3d20     _thethread = 
+00008100: 7468 7265 6164 696e 672e 5468 7265 6164  threading.Thread
+00008110: 280a 2020 2020 2020 2020 2020 2020 2020  (.              
+00008120: 2020 2020 2020 2020 2020 7461 7267 6574            target
+00008130: 3d73 656c 662e 6368 6563 6b5f 6361 6c6c  =self.check_call
+00008140: 7369 676e 322c 0a20 2020 2020 2020 2020  sign2,.         
+00008150: 2020 2020 2020 2020 2020 2020 2020 2061                 a
+00008160: 7267 733d 2874 6578 742c 292c 0a20 2020  rgs=(text,),.   
 00008170: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00008180: 2020 2020 6461 656d 6f6e 3d54 7275 652c      daemon=True,
-00008190: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-000081a0: 2020 2020 2029 0a20 2020 2020 2020 2020       ).         
-000081b0: 2020 2020 2020 2020 2020 205f 7468 6574             _thet
-000081c0: 6872 6561 642e 7374 6172 7428 290a 2020  hread.start().  
+00008180: 2020 2020 2064 6165 6d6f 6e3d 5472 7565       daemon=True
+00008190: 2c0a 2020 2020 2020 2020 2020 2020 2020  ,.              
+000081a0: 2020 2020 2020 290a 2020 2020 2020 2020        ).        
+000081b0: 2020 2020 2020 2020 2020 2020 5f74 6865              _the
+000081c0: 7468 7265 6164 2e73 7461 7274 2829 0a20  thread.start(). 
 000081d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000081e0: 2020 6e65 7874 5f74 6162 203d 2073 656c    next_tab = sel
-000081f0: 662e 7461 625f 6e65 7874 2e67 6574 2873  f.tab_next.get(s
-00008200: 656c 662e 6361 6c6c 7369 676e 290a 2020  elf.callsign).  
+000081e0: 2020 206e 6578 745f 7461 6220 3d20 7365     next_tab = se
+000081f0: 6c66 2e74 6162 5f6e 6578 742e 6765 7428  lf.tab_next.get(
+00008200: 7365 6c66 2e63 616c 6c73 6967 6e29 0a20  self.callsign). 
 00008210: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00008220: 2020 6e65 7874 5f74 6162 2e73 6574 466f    next_tab.setFo
-00008230: 6375 7328 290a 2020 2020 2020 2020 2020  cus().          
-00008240: 2020 2020 2020 2020 2020 6e65 7874 5f74            next_t
-00008250: 6162 2e64 6573 656c 6563 7428 290a 2020  ab.deselect().  
+00008220: 2020 206e 6578 745f 7461 622e 7365 7446     next_tab.setF
+00008230: 6f63 7573 2829 0a20 2020 2020 2020 2020  ocus().         
+00008240: 2020 2020 2020 2020 2020 206e 6578 745f             next_
+00008250: 7461 622e 6465 7365 6c65 6374 2829 0a20  tab.deselect(). 
 00008260: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00008270: 2020 6e65 7874 5f74 6162 2e65 6e64 2846    next_tab.end(F
-00008280: 616c 7365 290a 2020 2020 2020 2020 2020  alse).          
-00008290: 2020 2020 2020 7265 7475 726e 0a20 2020        return.   
-000082a0: 2020 2020 2069 6620 6576 656e 742e 6b65       if event.ke
-000082b0: 7928 2920 3d3d 2051 742e 4b65 795f 4631  y() == Qt.Key_F1
-000082c0: 3a0a 2020 2020 2020 2020 2020 2020 7365  :.            se
-000082d0: 6c66 2e73 656e 6466 3128 290a 2020 2020  lf.sendf1().    
-000082e0: 2020 2020 6966 2065 7665 6e74 2e6b 6579      if event.key
-000082f0: 2829 203d 3d20 5174 2e4b 6579 5f46 323a  () == Qt.Key_F2:
-00008300: 0a20 2020 2020 2020 2020 2020 2073 656c  .            sel
-00008310: 662e 7365 6e64 6632 2829 0a20 2020 2020  f.sendf2().     
-00008320: 2020 2069 6620 6576 656e 742e 6b65 7928     if event.key(
-00008330: 2920 3d3d 2051 742e 4b65 795f 4633 3a0a  ) == Qt.Key_F3:.
-00008340: 2020 2020 2020 2020 2020 2020 7365 6c66              self
-00008350: 2e73 656e 6466 3328 290a 2020 2020 2020  .sendf3().      
-00008360: 2020 6966 2065 7665 6e74 2e6b 6579 2829    if event.key()
-00008370: 203d 3d20 5174 2e4b 6579 5f46 343a 0a20   == Qt.Key_F4:. 
-00008380: 2020 2020 2020 2020 2020 2073 656c 662e             self.
-00008390: 7365 6e64 6634 2829 0a20 2020 2020 2020  sendf4().       
-000083a0: 2069 6620 6576 656e 742e 6b65 7928 2920   if event.key() 
-000083b0: 3d3d 2051 742e 4b65 795f 4635 3a0a 2020  == Qt.Key_F5:.  
-000083c0: 2020 2020 2020 2020 2020 7365 6c66 2e73            self.s
-000083d0: 656e 6466 3528 290a 2020 2020 2020 2020  endf5().        
-000083e0: 6966 2065 7665 6e74 2e6b 6579 2829 203d  if event.key() =
-000083f0: 3d20 5174 2e4b 6579 5f46 363a 0a20 2020  = Qt.Key_F6:.   
-00008400: 2020 2020 2020 2020 2073 656c 662e 7365           self.se
-00008410: 6e64 6636 2829 0a20 2020 2020 2020 2069  ndf6().        i
-00008420: 6620 6576 656e 742e 6b65 7928 2920 3d3d  f event.key() ==
-00008430: 2051 742e 4b65 795f 4637 3a0a 2020 2020   Qt.Key_F7:.    
-00008440: 2020 2020 2020 2020 7365 6c66 2e73 656e          self.sen
-00008450: 6466 3728 290a 2020 2020 2020 2020 6966  df7().        if
-00008460: 2065 7665 6e74 2e6b 6579 2829 203d 3d20   event.key() == 
-00008470: 5174 2e4b 6579 5f46 383a 0a20 2020 2020  Qt.Key_F8:.     
-00008480: 2020 2020 2020 2073 656c 662e 7365 6e64         self.send
-00008490: 6638 2829 0a20 2020 2020 2020 2069 6620  f8().        if 
-000084a0: 6576 656e 742e 6b65 7928 2920 3d3d 2051  event.key() == Q
-000084b0: 742e 4b65 795f 4639 3a0a 2020 2020 2020  t.Key_F9:.      
-000084c0: 2020 2020 2020 7365 6c66 2e73 656e 6466        self.sendf
-000084d0: 3928 290a 2020 2020 2020 2020 6966 2065  9().        if e
-000084e0: 7665 6e74 2e6b 6579 2829 203d 3d20 5174  vent.key() == Qt
-000084f0: 2e4b 6579 5f46 3130 3a0a 2020 2020 2020  .Key_F10:.      
-00008500: 2020 2020 2020 7365 6c66 2e73 656e 6466        self.sendf
-00008510: 3130 2829 0a20 2020 2020 2020 2069 6620  10().        if 
-00008520: 6576 656e 742e 6b65 7928 2920 3d3d 2051  event.key() == Q
-00008530: 742e 4b65 795f 4631 313a 0a20 2020 2020  t.Key_F11:.     
-00008540: 2020 2020 2020 2073 656c 662e 7365 6e64         self.send
-00008550: 6631 3128 290a 2020 2020 2020 2020 6966  f11().        if
-00008560: 2065 7665 6e74 2e6b 6579 2829 203d 3d20   event.key() == 
-00008570: 5174 2e4b 6579 5f46 3132 3a0a 2020 2020  Qt.Key_F12:.    
-00008580: 2020 2020 2020 2020 7365 6c66 2e73 656e          self.sen
-00008590: 6466 3132 2829 0a0a 2020 2020 6465 6620  df12()..    def 
-000085a0: 7365 745f 7769 6e64 6f77 5f74 6974 6c65  set_window_title
-000085b0: 2873 656c 6629 3a0a 2020 2020 2020 2020  (self):.        
-000085c0: 2222 2253 6574 2077 696e 646f 7720 7469  """Set window ti
-000085d0: 746c 6522 2222 0a20 2020 2020 2020 2076  tle""".        v
-000085e0: 666f 6120 3d20 7365 6c66 2e72 6164 696f  foa = self.radio
-000085f0: 5f73 7461 7465 2e67 6574 2822 7666 6f61  _state.get("vfoa
-00008600: 222c 2022 2229 0a20 2020 2020 2020 2069  ", "").        i
-00008610: 6620 7666 6f61 3a0a 2020 2020 2020 2020  f vfoa:.        
-00008620: 2020 2020 7666 6f61 203d 2069 6e74 2876      vfoa = int(v
-00008630: 666f 6129 202f 2031 3030 300a 2020 2020  foa) / 1000.    
-00008640: 2020 2020 656c 7365 3a0a 2020 2020 2020      else:.      
-00008650: 2020 2020 2020 7666 6f61 203d 2030 2e30        vfoa = 0.0
-00008660: 0a20 2020 2020 2020 2063 6f6e 7465 7374  .        contest
-00008670: 5f6e 616d 6520 3d20 2222 0a20 2020 2020  _name = "".     
-00008680: 2020 2069 6620 7365 6c66 2e63 6f6e 7465     if self.conte
-00008690: 7374 3a0a 2020 2020 2020 2020 2020 2020  st:.            
-000086a0: 636f 6e74 6573 745f 6e61 6d65 203d 2073  contest_name = s
-000086b0: 656c 662e 636f 6e74 6573 742e 6e61 6d65  elf.contest.name
-000086c0: 0a20 2020 2020 2020 206c 696e 6520 3d20  .        line = 
-000086d0: 280a 2020 2020 2020 2020 2020 2020 6622  (.            f"
-000086e0: 7666 6f61 3a7b 726f 756e 6428 7666 6f61  vfoa:{round(vfoa
-000086f0: 2c32 297d 2022 0a20 2020 2020 2020 2020  ,2)} ".         
-00008700: 2020 2066 226d 6f64 653a 7b73 656c 662e     f"mode:{self.
-00008710: 7261 6469 6f5f 7374 6174 652e 6765 7428  radio_state.get(
-00008720: 276d 6f64 6527 2c20 2727 297d 2022 0a20  'mode', '')} ". 
-00008730: 2020 2020 2020 2020 2020 2066 224f 503a             f"OP:
-00008740: 7b73 656c 662e 6375 7272 656e 745f 6f70  {self.current_op
-00008750: 7d20 7b63 6f6e 7465 7374 5f6e 616d 657d  } {contest_name}
-00008760: 2022 0a20 2020 2020 2020 2020 2020 2066   ".            f
-00008770: 222d 204e 6f74 314d 4d20 767b 5f5f 7665  "- Not1MM v{__ve
-00008780: 7273 696f 6e5f 5f7d 220a 2020 2020 2020  rsion__}".      
-00008790: 2020 290a 2020 2020 2020 2020 6c6f 6767    ).        logg
-000087a0: 6572 2e64 6562 7567 2822 2573 222c 206c  er.debug("%s", l
-000087b0: 696e 6529 0a20 2020 2020 2020 2073 656c  ine).        sel
-000087c0: 662e 7365 7457 696e 646f 7754 6974 6c65  f.setWindowTitle
-000087d0: 286c 696e 6529 0a0a 2020 2020 6465 6620  (line)..    def 
-000087e0: 636c 6561 7269 6e70 7574 7328 7365 6c66  clearinputs(self
-000087f0: 293a 0a20 2020 2020 2020 2022 2222 436c  ):.        """Cl
-00008800: 6561 7273 2074 6865 2074 6578 7420 696e  ears the text in
-00008810: 7075 7420 6669 656c 6473 2061 6e64 2073  put fields and s
-00008820: 6574 7320 666f 6375 7320 746f 2063 616c  ets focus to cal
-00008830: 6c73 6967 6e20 6669 656c 642e 2222 220a  lsign field.""".
-00008840: 2020 2020 2020 2020 7365 6c66 2e64 7570          self.dup
-00008850: 655f 696e 6469 6361 746f 722e 6869 6465  e_indicator.hide
-00008860: 2829 0a20 2020 2020 2020 2073 656c 662e  ().        self.
-00008870: 636f 6e74 6163 7420 3d20 7365 6c66 2e64  contact = self.d
-00008880: 6174 6162 6173 652e 656d 7074 795f 636f  atabase.empty_co
-00008890: 6e74 6163 740a 2020 2020 2020 2020 7365  ntact.        se
-000088a0: 6c66 2e68 6561 6469 6e67 5f64 6973 7461  lf.heading_dista
-000088b0: 6e63 652e 7365 7454 6578 7428 2222 290a  nce.setText("").
-000088c0: 2020 2020 2020 2020 7365 6c66 2e64 785f          self.dx_
-000088d0: 656e 7469 7479 2e73 6574 5465 7874 2822  entity.setText("
-000088e0: 2229 0a20 2020 2020 2020 2069 6620 7365  ").        if se
-000088f0: 6c66 2e63 6f6e 7465 7374 3a0a 2020 2020  lf.contest:.    
-00008900: 2020 2020 2020 2020 6d75 6c74 7320 3d20          mults = 
-00008910: 7365 6c66 2e63 6f6e 7465 7374 2e73 686f  self.contest.sho
-00008920: 775f 6d75 6c74 7328 7365 6c66 290a 2020  w_mults(self).  
-00008930: 2020 2020 2020 2020 2020 7173 6f73 203d            qsos =
-00008940: 2073 656c 662e 636f 6e74 6573 742e 7368   self.contest.sh
-00008950: 6f77 5f71 736f 2873 656c 6629 0a20 2020  ow_qso(self).   
-00008960: 2020 2020 2020 2020 206d 756c 7473 7472           multstr
-00008970: 696e 6720 3d20 6622 7b71 736f 737d 2f7b  ing = f"{qsos}/{
-00008980: 6d75 6c74 737d 220a 2020 2020 2020 2020  mults}".        
-00008990: 2020 2020 7365 6c66 2e6d 756c 7473 2e73      self.mults.s
-000089a0: 6574 5465 7874 286d 756c 7473 7472 696e  etText(multstrin
-000089b0: 6729 0a20 2020 2020 2020 2020 2020 2073  g).            s
-000089c0: 636f 7265 203d 2073 656c 662e 636f 6e74  core = self.cont
-000089d0: 6573 742e 6361 6c63 5f73 636f 7265 2873  est.calc_score(s
-000089e0: 656c 6629 0a20 2020 2020 2020 2020 2020  elf).           
-000089f0: 2073 656c 662e 7363 6f72 652e 7365 7454   self.score.setT
-00008a00: 6578 7428 7374 7228 7363 6f72 6529 290a  ext(str(score)).
-00008a10: 2020 2020 2020 2020 2020 2020 7365 6c66              self
-00008a20: 2e63 6f6e 7465 7374 2e72 6573 6574 5f6c  .contest.reset_l
-00008a30: 6162 656c 2873 656c 6629 0a20 2020 2020  abel(self).     
-00008a40: 2020 2073 656c 662e 6361 6c6c 7369 676e     self.callsign
-00008a50: 2e63 6c65 6172 2829 0a20 2020 2020 2020  .clear().       
-00008a60: 2069 6620 7365 6c66 2e63 7572 7265 6e74   if self.current
-00008a70: 5f6d 6f64 6520 3d3d 2022 4357 223a 0a20  _mode == "CW":. 
-00008a80: 2020 2020 2020 2020 2020 2073 656c 662e             self.
-00008a90: 7365 6e74 2e73 6574 5465 7874 2822 3539  sent.setText("59
-00008aa0: 3922 290a 2020 2020 2020 2020 2020 2020  9").            
-00008ab0: 7365 6c66 2e72 6563 6569 7665 2e73 6574  self.receive.set
-00008ac0: 5465 7874 2822 3539 3922 290a 2020 2020  Text("599").    
-00008ad0: 2020 2020 656c 7365 3a0a 2020 2020 2020      else:.      
-00008ae0: 2020 2020 2020 7365 6c66 2e73 656e 742e        self.sent.
-00008af0: 7365 7454 6578 7428 2235 3922 290a 2020  setText("59").  
-00008b00: 2020 2020 2020 2020 2020 7365 6c66 2e72            self.r
-00008b10: 6563 6569 7665 2e73 6574 5465 7874 2822  eceive.setText("
-00008b20: 3539 2229 0a20 2020 2020 2020 2073 656c  59").        sel
-00008b30: 662e 6f74 6865 725f 312e 636c 6561 7228  f.other_1.clear(
-00008b40: 290a 2020 2020 2020 2020 7365 6c66 2e6f  ).        self.o
-00008b50: 7468 6572 5f32 2e63 6c65 6172 2829 0a20  ther_2.clear(). 
-00008b60: 2020 2020 2020 2073 656c 662e 6361 6c6c         self.call
-00008b70: 7369 676e 2e73 6574 466f 6375 7328 290a  sign.setFocus().
-00008b80: 2020 2020 2020 2020 636d 6420 3d20 7b7d          cmd = {}
-00008b90: 0a20 2020 2020 2020 2063 6d64 5b22 636d  .        cmd["cm
-00008ba0: 6422 5d20 3d20 2243 414c 4c43 4841 4e47  d"] = "CALLCHANG
-00008bb0: 4544 220a 2020 2020 2020 2020 636d 645b  ED".        cmd[
-00008bc0: 2273 7461 7469 6f6e 225d 203d 2070 6c61  "station"] = pla
-00008bd0: 7466 6f72 6d2e 6e6f 6465 2829 0a20 2020  tform.node().   
-00008be0: 2020 2020 2063 6d64 5b22 6361 6c6c 225d       cmd["call"]
-00008bf0: 203d 2022 220a 2020 2020 2020 2020 7365   = "".        se
-00008c00: 6c66 2e6d 756c 7469 6361 7374 5f69 6e74  lf.multicast_int
-00008c10: 6572 6661 6365 2e73 656e 645f 6173 5f6a  erface.send_as_j
-00008c20: 736f 6e28 636d 6429 0a0a 2020 2020 6465  son(cmd)..    de
-00008c30: 6620 7361 7665 5f63 6f6e 7461 6374 2873  f save_contact(s
-00008c40: 656c 6629 3a0a 2020 2020 2020 2020 2222  elf):.        ""
-00008c50: 2253 6176 6520 746f 2064 6222 2222 0a20  "Save to db""". 
-00008c60: 2020 2020 2020 206c 6f67 6765 722e 6465         logger.de
-00008c70: 6275 6728 2273 6176 696e 6720 636f 6e74  bug("saving cont
-00008c80: 6163 7422 290a 2020 2020 2020 2020 6966  act").        if
-00008c90: 206c 656e 2873 656c 662e 6361 6c6c 7369   len(self.callsi
-00008ca0: 676e 2e74 6578 7428 2929 203c 2033 3a0a  gn.text()) < 3:.
-00008cb0: 2020 2020 2020 2020 2020 2020 7265 7475              retu
-00008cc0: 726e 0a20 2020 2020 2020 2069 6620 6e6f  rn.        if no
-00008cd0: 7420 616e 7928 6368 6172 2e69 7364 6967  t any(char.isdig
-00008ce0: 6974 2829 2066 6f72 2063 6861 7220 696e  it() for char in
-00008cf0: 2073 656c 662e 6361 6c6c 7369 676e 2e74   self.callsign.t
-00008d00: 6578 7428 2929 3a0a 2020 2020 2020 2020  ext()):.        
-00008d10: 2020 2020 7265 7475 726e 0a20 2020 2020      return.     
-00008d20: 2020 2069 6620 6e6f 7420 616e 7928 6368     if not any(ch
-00008d30: 6172 2e69 7361 6c70 6861 2829 2066 6f72  ar.isalpha() for
-00008d40: 2063 6861 7220 696e 2073 656c 662e 6361   char in self.ca
-00008d50: 6c6c 7369 676e 2e74 6578 7428 2929 3a0a  llsign.text()):.
-00008d60: 2020 2020 2020 2020 2020 2020 7265 7475              retu
-00008d70: 726e 0a0a 2020 2020 2020 2020 7365 6c66  rn..        self
-00008d80: 2e63 6f6e 7461 6374 5b22 5453 225d 203d  .contact["TS"] =
-00008d90: 2064 6174 6574 696d 652e 7574 636e 6f77   datetime.utcnow
-00008da0: 2829 2e69 736f 666f 726d 6174 2822 2022  ().isoformat(" "
-00008db0: 295b 3a31 395d 0a20 2020 2020 2020 2073  )[:19].        s
-00008dc0: 656c 662e 636f 6e74 6163 745b 2243 616c  elf.contact["Cal
-00008dd0: 6c22 5d20 3d20 7365 6c66 2e63 616c 6c73  l"] = self.calls
-00008de0: 6967 6e2e 7465 7874 2829 0a20 2020 2020  ign.text().     
-00008df0: 2020 2073 656c 662e 636f 6e74 6163 745b     self.contact[
-00008e00: 2246 7265 7122 5d20 3d20 726f 756e 6428  "Freq"] = round(
-00008e10: 666c 6f61 7428 7365 6c66 2e72 6164 696f  float(self.radio
-00008e20: 5f73 7461 7465 2e67 6574 2822 7666 6f61  _state.get("vfoa
-00008e30: 222c 2030 2e30 2929 202f 2031 3030 302c  ", 0.0)) / 1000,
-00008e40: 2032 290a 2020 2020 2020 2020 7365 6c66   2).        self
-00008e50: 2e63 6f6e 7461 6374 5b22 5153 5846 7265  .contact["QSXFre
-00008e60: 7122 5d20 3d20 726f 756e 6428 0a20 2020  q"] = round(.   
-00008e70: 2020 2020 2020 2020 2066 6c6f 6174 2873           float(s
-00008e80: 656c 662e 7261 6469 6f5f 7374 6174 652e  elf.radio_state.
-00008e90: 6765 7428 2276 666f 6122 2c20 302e 3029  get("vfoa", 0.0)
-00008ea0: 2920 2f20 3130 3030 2c20 320a 2020 2020  ) / 1000, 2.    
-00008eb0: 2020 2020 290a 2020 2020 2020 2020 7365      ).        se
-00008ec0: 6c66 2e63 6f6e 7461 6374 5b22 4d6f 6465  lf.contact["Mode
-00008ed0: 225d 203d 2073 656c 662e 7261 6469 6f5f  "] = self.radio_
-00008ee0: 7374 6174 652e 6765 7428 226d 6f64 6522  state.get("mode"
-00008ef0: 2c20 2222 290a 2020 2020 2020 2020 7365  , "").        se
-00008f00: 6c66 2e63 6f6e 7461 6374 5b22 436f 6e74  lf.contact["Cont
-00008f10: 6573 744e 616d 6522 5d20 3d20 7365 6c66  estName"] = self
-00008f20: 2e63 6f6e 7465 7374 2e63 6162 7269 6c6c  .contest.cabrill
-00008f30: 6f5f 6e61 6d65 0a20 2020 2020 2020 2073  o_name.        s
-00008f40: 656c 662e 636f 6e74 6163 745b 2243 6f6e  elf.contact["Con
-00008f50: 7465 7374 4e52 225d 203d 2073 656c 662e  testNR"] = self.
-00008f60: 7072 6566 2e67 6574 2822 636f 6e74 6573  pref.get("contes
-00008f70: 7422 2c20 2230 2229 0a20 2020 2020 2020  t", "0").       
-00008f80: 2073 656c 662e 636f 6e74 6163 745b 2253   self.contact["S
-00008f90: 7461 7469 6f6e 5072 6566 6978 225d 203d  tationPrefix"] =
-00008fa0: 2073 656c 662e 7374 6174 696f 6e2e 6765   self.station.ge
-00008fb0: 7428 2243 616c 6c22 2c20 2222 290a 2020  t("Call", "").  
-00008fc0: 2020 2020 2020 7365 6c66 2e63 6f6e 7461        self.conta
-00008fd0: 6374 5b22 5750 5850 7265 6669 7822 5d20  ct["WPXPrefix"] 
-00008fe0: 3d20 6361 6c63 756c 6174 655f 7770 785f  = calculate_wpx_
-00008ff0: 7072 6566 6978 2873 656c 662e 6361 6c6c  prefix(self.call
-00009000: 7369 676e 2e74 6578 7428 2929 0a20 2020  sign.text()).   
-00009010: 2020 2020 2073 656c 662e 636f 6e74 6163       self.contac
-00009020: 745b 2249 7352 756e 5153 4f22 5d20 3d20  t["IsRunQSO"] = 
-00009030: 7365 6c66 2e72 6164 696f 4275 7474 6f6e  self.radioButton
-00009040: 5f72 756e 2e69 7343 6865 636b 6564 2829  _run.isChecked()
-00009050: 0a20 2020 2020 2020 2073 656c 662e 636f  .        self.co
-00009060: 6e74 6163 745b 224f 7065 7261 746f 7222  ntact["Operator"
-00009070: 5d20 3d20 7365 6c66 2e63 7572 7265 6e74  ] = self.current
-00009080: 5f6f 700a 2020 2020 2020 2020 7365 6c66  _op.        self
-00009090: 2e63 6f6e 7461 6374 5b22 4e65 7442 696f  .contact["NetBio
-000090a0: 734e 616d 6522 5d20 3d20 736f 636b 6574  sName"] = socket
-000090b0: 2e67 6574 686f 7374 6e61 6d65 2829 0a20  .gethostname(). 
-000090c0: 2020 2020 2020 2073 656c 662e 636f 6e74         self.cont
-000090d0: 6163 745b 2249 734f 7269 6769 6e61 6c22  act["IsOriginal"
-000090e0: 5d20 3d20 310a 2020 2020 2020 2020 7365  ] = 1.        se
-000090f0: 6c66 2e63 6f6e 7461 6374 5b22 4944 225d  lf.contact["ID"]
-00009100: 203d 2075 7569 642e 7575 6964 3428 292e   = uuid.uuid4().
-00009110: 6865 780a 2020 2020 2020 2020 7365 6c66  hex.        self
-00009120: 2e63 6f6e 7465 7374 2e73 6574 5f63 6f6e  .contest.set_con
-00009130: 7461 6374 5f76 6172 7328 7365 6c66 290a  tact_vars(self).
-00009140: 2020 2020 2020 2020 7365 6c66 2e63 6f6e          self.con
-00009150: 7461 6374 5b22 506f 696e 7473 225d 203d  tact["Points"] =
-00009160: 2073 656c 662e 636f 6e74 6573 742e 706f   self.contest.po
-00009170: 696e 7473 2873 656c 6629 0a20 2020 2020  ints(self).     
-00009180: 2020 2064 6562 7567 5f6f 7574 7075 7420     debug_output 
-00009190: 3d20 6622 7b73 656c 662e 636f 6e74 6163  = f"{self.contac
-000091a0: 747d 220a 2020 2020 2020 2020 6c6f 6767  t}".        logg
-000091b0: 6572 2e64 6562 7567 2864 6562 7567 5f6f  er.debug(debug_o
-000091c0: 7574 7075 7429 0a20 2020 2020 2020 2073  utput).        s
-000091d0: 656c 662e 6461 7461 6261 7365 2e6c 6f67  elf.database.log
-000091e0: 5f63 6f6e 7461 6374 2873 656c 662e 636f  _contact(self.co
-000091f0: 6e74 6163 7429 0a20 2020 2020 2020 2073  ntact).        s
-00009200: 656c 662e 6e31 6d6d 2e73 656e 645f 636f  elf.n1mm.send_co
-00009210: 6e74 6163 745f 696e 666f 2829 0a20 2020  ntact_info().   
-00009220: 2020 2020 2073 656c 662e 636c 6561 7269       self.cleari
-00009230: 6e70 7574 7328 290a 2020 2020 2020 2020  nputs().        
-00009240: 636d 6420 3d20 7b7d 0a20 2020 2020 2020  cmd = {}.       
-00009250: 2063 6d64 5b22 636d 6422 5d20 3d20 2255   cmd["cmd"] = "U
-00009260: 5044 4154 454c 4f47 220a 2020 2020 2020  PDATELOG".      
-00009270: 2020 636d 645b 2273 7461 7469 6f6e 225d    cmd["station"]
-00009280: 203d 2070 6c61 7466 6f72 6d2e 6e6f 6465   = platform.node
-00009290: 2829 0a20 2020 2020 2020 2073 656c 662e  ().        self.
-000092a0: 6d75 6c74 6963 6173 745f 696e 7465 7266  multicast_interf
-000092b0: 6163 652e 7365 6e64 5f61 735f 6a73 6f6e  ace.send_as_json
-000092c0: 2863 6d64 290a 2020 2020 2020 2020 2320  (cmd).        # 
-000092d0: 7365 6c66 2e63 6f6e 7461 6374 5b22 436f  self.contact["Co
-000092e0: 6e74 6573 744e 616d 6522 5d20 3d20 7365  ntestName"] = se
-000092f0: 6c66 2e63 6f6e 7465 7374 2e6e 616d 650a  lf.contest.name.
-00009300: 2020 2020 2020 2020 2320 7365 6c66 2e63          # self.c
-00009310: 6f6e 7461 6374 5b22 534e 5422 5d20 3d20  ontact["SNT"] = 
-00009320: 7365 6c66 2e73 656e 742e 7465 7874 2829  self.sent.text()
-00009330: 0a20 2020 2020 2020 2023 2073 656c 662e  .        # self.
-00009340: 636f 6e74 6163 745b 2252 4356 225d 203d  contact["RCV"] =
-00009350: 2073 656c 662e 7265 6365 6976 652e 7465   self.receive.te
-00009360: 7874 2829 0a20 2020 2020 2020 2023 2073  xt().        # s
-00009370: 656c 662e 636f 6e74 6163 745b 2243 6f75  elf.contact["Cou
-00009380: 6e74 7279 5072 6566 6978 225d 0a20 2020  ntryPrefix"].   
-00009390: 2020 2020 2023 2073 656c 662e 636f 6e74       # self.cont
-000093a0: 6163 745b 2253 7461 7469 6f6e 5072 6566  act["StationPref
-000093b0: 6978 225d 203d 2073 656c 662e 7072 6566  ix"] = self.pref
-000093c0: 2e67 6574 2822 6361 6c6c 7369 676e 222c  .get("callsign",
-000093d0: 2022 2229 0a20 2020 2020 2020 2023 2073   "").        # s
-000093e0: 656c 662e 636f 6e74 6163 745b 2251 5448  elf.contact["QTH
-000093f0: 225d 0a20 2020 2020 2020 2023 2073 656c  "].        # sel
-00009400: 662e 636f 6e74 6163 745b 224e 616d 6522  f.contact["Name"
-00009410: 5d20 3d20 7365 6c66 2e6f 7468 6572 5f31  ] = self.other_1
-00009420: 2e74 6578 7428 290a 2020 2020 2020 2020  .text().        
-00009430: 2320 7365 6c66 2e63 6f6e 7461 6374 5b22  # self.contact["
-00009440: 436f 6d6d 656e 7422 5d20 3d20 7365 6c66  Comment"] = self
-00009450: 2e6f 7468 6572 5f32 2e74 6578 7428 290a  .other_2.text().
-00009460: 2020 2020 2020 2020 2320 7365 6c66 2e63          # self.c
-00009470: 6f6e 7461 6374 5b22 4e52 225d 0a20 2020  ontact["NR"].   
-00009480: 2020 2020 2023 2073 656c 662e 636f 6e74       # self.cont
-00009490: 6163 745b 2253 6563 7422 5d0a 2020 2020  act["Sect"].    
-000094a0: 2020 2020 2320 7365 6c66 2e63 6f6e 7461      # self.conta
-000094b0: 6374 5b22 5072 6563 225d 0a20 2020 2020  ct["Prec"].     
-000094c0: 2020 2023 2073 656c 662e 636f 6e74 6163     # self.contac
-000094d0: 745b 2243 4b22 5d0a 2020 2020 2020 2020  t["CK"].        
-000094e0: 2320 7365 6c66 2e63 6f6e 7461 6374 5b22  # self.contact["
-000094f0: 5a4e 225d 0a20 2020 2020 2020 2023 2073  ZN"].        # s
-00009500: 656c 662e 636f 6e74 6163 745b 2253 656e  elf.contact["Sen
-00009510: 744e 7222 5d0a 2020 2020 2020 2020 2320  tNr"].        # 
-00009520: 7365 6c66 2e63 6f6e 7461 6374 5b22 506f  self.contact["Po
-00009530: 696e 7473 225d 0a20 2020 2020 2020 2023  ints"].        #
-00009540: 2073 656c 662e 636f 6e74 6163 745b 2249   self.contact["I
-00009550: 734d 756c 7469 706c 6965 7231 225d 0a20  sMultiplier1"]. 
-00009560: 2020 2020 2020 2023 2073 656c 662e 636f         # self.co
-00009570: 6e74 6163 745b 2249 734d 756c 7469 706c  ntact["IsMultipl
-00009580: 6965 7232 225d 0a20 2020 2020 2020 2023  ier2"].        #
-00009590: 2073 656c 662e 636f 6e74 6163 745b 2250   self.contact["P
-000095a0: 6f77 6572 225d 0a20 2020 2020 2020 2023  ower"].        #
-000095b0: 2073 656c 662e 636f 6e74 6163 745b 2242   self.contact["B
-000095c0: 616e 6422 5d0a 2020 2020 2020 2020 2320  and"].        # 
-000095d0: 7365 6c66 2e63 6f6e 7461 6374 5b22 5750  self.contact["WP
-000095e0: 5850 7265 6669 7822 5d20 3d20 6361 6c63  XPrefix"] = calc
-000095f0: 756c 6174 655f 7770 785f 7072 6566 6978  ulate_wpx_prefix
-00009600: 2873 656c 662e 6361 6c6c 7369 676e 2e74  (self.callsign.t
-00009610: 6578 7428 2929 0a20 2020 2020 2020 2023  ext()).        #
-00009620: 2073 656c 662e 636f 6e74 6163 745b 2245   self.contact["E
-00009630: 7863 6861 6e67 6531 225d 0a20 2020 2020  xchange1"].     
-00009640: 2020 2023 2073 656c 662e 636f 6e74 6163     # self.contac
-00009650: 745b 2252 6164 696f 4e52 225d 0a20 2020  t["RadioNR"].   
-00009660: 2020 2020 2023 2073 656c 662e 636f 6e74       # self.cont
-00009670: 6163 745b 2269 734d 756c 7469 706c 6965  act["isMultiplie
-00009680: 7233 225d 0a20 2020 2020 2020 2023 2073  r3"].        # s
-00009690: 656c 662e 636f 6e74 6163 745b 224d 6973  elf.contact["Mis
-000096a0: 6354 6578 7422 5d0a 2020 2020 2020 2020  cText"].        
-000096b0: 2320 7365 6c66 2e63 6f6e 7461 6374 5b22  # self.contact["
-000096c0: 436f 6e74 6163 7454 7970 6522 5d0a 2020  ContactType"].  
-000096d0: 2020 2020 2020 2320 7365 6c66 2e63 6f6e        # self.con
-000096e0: 7461 6374 5b22 5275 6e31 5275 6e32 225d  tact["Run1Run2"]
-000096f0: 0a20 2020 2020 2020 2023 2073 656c 662e  .        # self.
-00009700: 636f 6e74 6163 745b 2247 7269 6453 7175  contact["GridSqu
-00009710: 6172 6522 5d0a 2020 2020 2020 2020 2320  are"].        # 
-00009720: 7365 6c66 2e63 6f6e 7461 6374 5b22 436f  self.contact["Co
-00009730: 6e74 696e 656e 7422 5d0a 2020 2020 2020  ntinent"].      
-00009740: 2020 2320 7365 6c66 2e63 6f6e 7461 6374    # self.contact
-00009750: 5b22 526f 7665 724c 6f63 6174 696f 6e22  ["RoverLocation"
-00009760: 5d0a 2020 2020 2020 2020 2320 7365 6c66  ].        # self
-00009770: 2e63 6f6e 7461 6374 5b22 5261 6469 6f49  .contact["RadioI
-00009780: 6e74 6572 6661 6365 6422 5d0a 2020 2020  nterfaced"].    
-00009790: 2020 2020 2320 7365 6c66 2e63 6f6e 7461      # self.conta
-000097a0: 6374 5b22 4e65 7477 6f72 6b65 6443 6f6d  ct["NetworkedCom
-000097b0: 704e 7222 5d0a 2020 2020 2020 2020 2320  pNr"].        # 
-000097c0: 7365 6c66 2e63 6f6e 7461 6374 5b22 434c  self.contact["CL
-000097d0: 4149 4d45 4451 534f 225d 0a0a 2020 2020  AIMEDQSO"]..    
-000097e0: 6465 6620 6e65 775f 636f 6e74 6573 745f  def new_contest_
-000097f0: 6469 616c 6f67 2873 656c 6629 3a0a 2020  dialog(self):.  
-00009800: 2020 2020 2020 2222 2253 686f 7720 6e65        """Show ne
-00009810: 7720 636f 6e74 6573 7420 6469 616c 6f67  w contest dialog
-00009820: 2222 220a 2020 2020 2020 2020 6c6f 6767  """.        logg
-00009830: 6572 2e64 6562 7567 2822 4e65 7720 636f  er.debug("New co
-00009840: 6e74 6573 7420 4469 616c 6f67 2229 0a20  ntest Dialog"). 
-00009850: 2020 2020 2020 2073 656c 662e 636f 6e74         self.cont
-00009860: 6573 745f 6469 616c 6f67 203d 204e 6577  est_dialog = New
-00009870: 436f 6e74 6573 7428 574f 524b 494e 475f  Contest(WORKING_
-00009880: 5041 5448 290a 2020 2020 2020 2020 7365  PATH).        se
-00009890: 6c66 2e63 6f6e 7465 7374 5f64 6961 6c6f  lf.contest_dialo
-000098a0: 672e 6163 6365 7074 6564 2e63 6f6e 6e65  g.accepted.conne
-000098b0: 6374 2873 656c 662e 7361 7665 5f63 6f6e  ct(self.save_con
-000098c0: 7465 7374 290a 2020 2020 2020 2020 6966  test).        if
-000098d0: 2073 656c 662e 7072 6566 2e67 6574 2822   self.pref.get("
-000098e0: 6461 726b 5f6d 6f64 6522 293a 0a20 2020  dark_mode"):.   
-000098f0: 2020 2020 2020 2020 2073 656c 662e 636f           self.co
-00009900: 6e74 6573 745f 6469 616c 6f67 2e73 6574  ntest_dialog.set
-00009910: 5374 796c 6553 6865 6574 2844 4152 4b5f  StyleSheet(DARK_
-00009920: 5354 594c 4553 4845 4554 290a 2020 2020  STYLESHEET).    
-00009930: 2020 2020 7365 6c66 2e63 6f6e 7465 7374      self.contest
-00009940: 5f64 6961 6c6f 672e 6461 7465 5469 6d65  _dialog.dateTime
-00009950: 4564 6974 2e73 6574 4461 7465 2851 7443  Edit.setDate(QtC
-00009960: 6f72 652e 5144 6174 652e 6375 7272 656e  ore.QDate.curren
-00009970: 7444 6174 6528 2929 0a20 2020 2020 2020  tDate()).       
-00009980: 2073 656c 662e 636f 6e74 6573 745f 6469   self.contest_di
-00009990: 616c 6f67 2e64 6174 6554 696d 6545 6469  alog.dateTimeEdi
-000099a0: 742e 7365 7443 616c 656e 6461 7250 6f70  t.setCalendarPop
-000099b0: 7570 2854 7275 6529 0a20 2020 2020 2020  up(True).       
-000099c0: 2073 656c 662e 636f 6e74 6573 745f 6469   self.contest_di
-000099d0: 616c 6f67 2e64 6174 6554 696d 6545 6469  alog.dateTimeEdi
-000099e0: 742e 7365 7454 696d 6528 5174 436f 7265  t.setTime(QtCore
-000099f0: 2e51 5469 6d65 2830 2c20 3029 290a 2020  .QTime(0, 0)).  
-00009a00: 2020 2020 2020 7365 6c66 2e63 6f6e 7465        self.conte
-00009a10: 7374 5f64 6961 6c6f 672e 706f 7765 722e  st_dialog.power.
-00009a20: 7365 7443 7572 7265 6e74 5465 7874 2822  setCurrentText("
-00009a30: 4c4f 5722 290a 2020 2020 2020 2020 7365  LOW").        se
-00009a40: 6c66 2e63 6f6e 7465 7374 5f64 6961 6c6f  lf.contest_dialo
-00009a50: 672e 7374 6174 696f 6e2e 7365 7443 7572  g.station.setCur
-00009a60: 7265 6e74 5465 7874 2822 4649 5845 4422  rentText("FIXED"
-00009a70: 290a 2020 2020 2020 2020 7365 6c66 2e63  ).        self.c
-00009a80: 6f6e 7465 7374 5f64 6961 6c6f 672e 6f70  ontest_dialog.op
-00009a90: 656e 2829 0a0a 2020 2020 6465 6620 7361  en()..    def sa
-00009aa0: 7665 5f63 6f6e 7465 7374 2873 656c 6629  ve_contest(self)
-00009ab0: 3a0a 2020 2020 2020 2020 2222 2253 6176  :.        """Sav
-00009ac0: 6520 436f 6e74 6573 7422 2222 0a20 2020  e Contest""".   
-00009ad0: 2020 2020 206e 6578 745f 6e75 6d62 6572       next_number
-00009ae0: 203d 2073 656c 662e 6461 7461 6261 7365   = self.database
-00009af0: 2e67 6574 5f6e 6578 745f 636f 6e74 6573  .get_next_contes
-00009b00: 745f 6e72 2829 0a20 2020 2020 2020 2063  t_nr().        c
-00009b10: 6f6e 7465 7374 203d 207b 7d0a 2020 2020  ontest = {}.    
-00009b20: 2020 2020 636f 6e74 6573 745b 2243 6f6e      contest["Con
-00009b30: 7465 7374 4e61 6d65 225d 203d 2028 0a20  testName"] = (. 
-00009b40: 2020 2020 2020 2020 2020 2073 656c 662e             self.
-00009b50: 636f 6e74 6573 745f 6469 616c 6f67 2e63  contest_dialog.c
-00009b60: 6f6e 7465 7374 2e63 7572 7265 6e74 5465  ontest.currentTe
-00009b70: 7874 2829 2e6c 6f77 6572 2829 2e72 6570  xt().lower().rep
-00009b80: 6c61 6365 2822 2022 2c20 225f 2229 0a20  lace(" ", "_"). 
-00009b90: 2020 2020 2020 2029 0a20 2020 2020 2020         ).       
-00009ba0: 2063 6f6e 7465 7374 5b22 5374 6172 7444   contest["StartD
-00009bb0: 6174 6522 5d20 3d20 7365 6c66 2e63 6f6e  ate"] = self.con
-00009bc0: 7465 7374 5f64 6961 6c6f 672e 6461 7465  test_dialog.date
-00009bd0: 5469 6d65 4564 6974 2e64 6174 6554 696d  TimeEdit.dateTim
-00009be0: 6528 292e 746f 5374 7269 6e67 280a 2020  e().toString(.  
-00009bf0: 2020 2020 2020 2020 2020 2279 7979 792d            "yyyy-
-00009c00: 4d4d 2d64 6420 6868 3a6d 6d3a 7373 220a  MM-dd hh:mm:ss".
-00009c10: 2020 2020 2020 2020 290a 2020 2020 2020          ).      
-00009c20: 2020 636f 6e74 6573 745b 224f 7065 7261    contest["Opera
-00009c30: 746f 7243 6174 6567 6f72 7922 5d20 3d20  torCategory"] = 
-00009c40: 7365 6c66 2e63 6f6e 7465 7374 5f64 6961  self.contest_dia
-00009c50: 6c6f 672e 6f70 6572 6174 6f72 5f63 6c61  log.operator_cla
-00009c60: 7373 2e63 7572 7265 6e74 5465 7874 2829  ss.currentText()
-00009c70: 0a20 2020 2020 2020 2063 6f6e 7465 7374  .        contest
-00009c80: 5b22 4261 6e64 4361 7465 676f 7279 225d  ["BandCategory"]
-00009c90: 203d 2073 656c 662e 636f 6e74 6573 745f   = self.contest_
-00009ca0: 6469 616c 6f67 2e62 616e 642e 6375 7272  dialog.band.curr
-00009cb0: 656e 7454 6578 7428 290a 2020 2020 2020  entText().      
-00009cc0: 2020 636f 6e74 6573 745b 2250 6f77 6572    contest["Power
-00009cd0: 4361 7465 676f 7279 225d 203d 2073 656c  Category"] = sel
-00009ce0: 662e 636f 6e74 6573 745f 6469 616c 6f67  f.contest_dialog
-00009cf0: 2e70 6f77 6572 2e63 7572 7265 6e74 5465  .power.currentTe
-00009d00: 7874 2829 0a20 2020 2020 2020 2063 6f6e  xt().        con
-00009d10: 7465 7374 5b22 4d6f 6465 4361 7465 676f  test["ModeCatego
-00009d20: 7279 225d 203d 2073 656c 662e 636f 6e74  ry"] = self.cont
-00009d30: 6573 745f 6469 616c 6f67 2e6d 6f64 652e  est_dialog.mode.
-00009d40: 6375 7272 656e 7454 6578 7428 290a 2020  currentText().  
-00009d50: 2020 2020 2020 636f 6e74 6573 745b 224f        contest["O
-00009d60: 7665 726c 6179 4361 7465 676f 7279 225d  verlayCategory"]
-00009d70: 203d 2073 656c 662e 636f 6e74 6573 745f   = self.contest_
-00009d80: 6469 616c 6f67 2e6f 7665 726c 6179 2e63  dialog.overlay.c
-00009d90: 7572 7265 6e74 5465 7874 2829 0a20 2020  urrentText().   
-00009da0: 2020 2020 2023 2063 6f6e 7465 7374 5b27       # contest['
-00009db0: 436c 6169 6d65 6453 636f 7265 275d 203d  ClaimedScore'] =
-00009dc0: 2073 656c 662e 636f 6e74 6573 745f 6469   self.contest_di
-00009dd0: 616c 6f67 2e0a 2020 2020 2020 2020 636f  alog..        co
-00009de0: 6e74 6573 745b 224f 7065 7261 746f 7273  ntest["Operators
-00009df0: 225d 203d 2073 656c 662e 636f 6e74 6573  "] = self.contes
-00009e00: 745f 6469 616c 6f67 2e6f 7065 7261 746f  t_dialog.operato
-00009e10: 7273 2e74 6578 7428 290a 2020 2020 2020  rs.text().      
-00009e20: 2020 636f 6e74 6573 745b 2253 6f61 7062    contest["Soapb
-00009e30: 6f78 225d 203d 2073 656c 662e 636f 6e74  ox"] = self.cont
-00009e40: 6573 745f 6469 616c 6f67 2e73 6f61 7062  est_dialog.soapb
-00009e50: 6f78 2e74 6f50 6c61 696e 5465 7874 2829  ox.toPlainText()
-00009e60: 0a20 2020 2020 2020 2063 6f6e 7465 7374  .        contest
-00009e70: 5b22 5365 6e74 4578 6368 616e 6765 225d  ["SentExchange"]
-00009e80: 203d 2073 656c 662e 636f 6e74 6573 745f   = self.contest_
-00009e90: 6469 616c 6f67 2e65 7863 6861 6e67 652e  dialog.exchange.
-00009ea0: 7465 7874 2829 0a20 2020 2020 2020 2063  text().        c
-00009eb0: 6f6e 7465 7374 5b22 436f 6e74 6573 744e  ontest["ContestN
-00009ec0: 5222 5d20 3d20 6e65 7874 5f6e 756d 6265  R"] = next_numbe
-00009ed0: 722e 6765 7428 2263 6f75 6e74 222c 2031  r.get("count", 1
-00009ee0: 290a 2020 2020 2020 2020 7365 6c66 2e70  ).        self.p
-00009ef0: 7265 665b 2263 6f6e 7465 7374 225d 203d  ref["contest"] =
-00009f00: 206e 6578 745f 6e75 6d62 6572 2e67 6574   next_number.get
-00009f10: 2822 636f 756e 7422 2c20 3129 0a20 2020  ("count", 1).   
-00009f20: 2020 2020 2023 2063 6f6e 7465 7374 5b27       # contest['
-00009f30: 5375 6254 7970 6527 5d20 3d20 7365 6c66  SubType'] = self
-00009f40: 2e63 6f6e 7465 7374 5f64 6961 6c6f 672e  .contest_dialog.
-00009f50: 0a20 2020 2020 2020 2063 6f6e 7465 7374  .        contest
-00009f60: 5b22 5374 6174 696f 6e43 6174 6567 6f72  ["StationCategor
-00009f70: 7922 5d20 3d20 7365 6c66 2e63 6f6e 7465  y"] = self.conte
-00009f80: 7374 5f64 6961 6c6f 672e 7374 6174 696f  st_dialog.statio
-00009f90: 6e2e 6375 7272 656e 7454 6578 7428 290a  n.currentText().
-00009fa0: 2020 2020 2020 2020 636f 6e74 6573 745b          contest[
-00009fb0: 2241 7373 6973 7465 6443 6174 6567 6f72  "AssistedCategor
-00009fc0: 7922 5d20 3d20 7365 6c66 2e63 6f6e 7465  y"] = self.conte
-00009fd0: 7374 5f64 6961 6c6f 672e 6173 7369 7374  st_dialog.assist
-00009fe0: 6564 2e63 7572 7265 6e74 5465 7874 2829  ed.currentText()
-00009ff0: 0a20 2020 2020 2020 2063 6f6e 7465 7374  .        contest
-0000a000: 5b22 5472 616e 736d 6974 7465 7243 6174  ["TransmitterCat
-0000a010: 6567 6f72 7922 5d20 3d20 7365 6c66 2e63  egory"] = self.c
-0000a020: 6f6e 7465 7374 5f64 6961 6c6f 672e 7472  ontest_dialog.tr
-0000a030: 616e 736d 6974 7465 722e 6375 7272 656e  ansmitter.curren
-0000a040: 7454 6578 7428 290a 2020 2020 2020 2020  tText().        
-0000a050: 2320 636f 6e74 6573 745b 2754 696d 6543  # contest['TimeC
-0000a060: 6174 6567 6f72 7927 5d20 3d20 7365 6c66  ategory'] = self
-0000a070: 2e63 6f6e 7465 7374 5f64 6961 6c6f 672e  .contest_dialog.
-0000a080: 0a20 2020 2020 2020 206c 6f67 6765 722e  .        logger.
-0000a090: 6465 6275 6728 2225 7322 2c20 6622 7b63  debug("%s", f"{c
-0000a0a0: 6f6e 7465 7374 7d22 290a 2020 2020 2020  ontest}").      
-0000a0b0: 2020 7365 6c66 2e64 6174 6162 6173 652e    self.database.
-0000a0c0: 6164 645f 636f 6e74 6573 7428 636f 6e74  add_contest(cont
-0000a0d0: 6573 7429 0a20 2020 2020 2020 2073 656c  est).        sel
-0000a0e0: 662e 7772 6974 655f 7072 6566 6572 656e  f.write_preferen
-0000a0f0: 6365 2829 0a20 2020 2020 2020 2073 656c  ce().        sel
-0000a100: 662e 6c6f 6164 5f63 6f6e 7465 7374 2829  f.load_contest()
-0000a110: 0a0a 2020 2020 6465 6620 6564 6974 5f73  ..    def edit_s
-0000a120: 7461 7469 6f6e 5f73 6574 7469 6e67 7328  tation_settings(
-0000a130: 7365 6c66 293a 0a20 2020 2020 2020 2022  self):.        "
-0000a140: 2222 5368 6f77 2073 6574 7469 6e67 7320  ""Show settings 
-0000a150: 6469 616c 6f67 2222 220a 2020 2020 2020  dialog""".      
-0000a160: 2020 6c6f 6767 6572 2e64 6562 7567 2822    logger.debug("
-0000a170: 5374 6174 696f 6e20 5365 7474 696e 6773  Station Settings
-0000a180: 2073 656c 6563 7465 6422 290a 2020 2020   selected").    
-0000a190: 2020 2020 7365 6c66 2e73 6574 7469 6e67      self.setting
-0000a1a0: 735f 6469 616c 6f67 203d 2045 6469 7453  s_dialog = EditS
-0000a1b0: 7461 7469 6f6e 2857 4f52 4b49 4e47 5f50  tation(WORKING_P
-0000a1c0: 4154 4829 0a20 2020 2020 2020 2069 6620  ATH).        if 
-0000a1d0: 7365 6c66 2e70 7265 662e 6765 7428 2264  self.pref.get("d
-0000a1e0: 6172 6b5f 6d6f 6465 2229 3a0a 2020 2020  ark_mode"):.    
-0000a1f0: 2020 2020 2020 2020 7365 6c66 2e73 6574          self.set
-0000a200: 7469 6e67 735f 6469 616c 6f67 2e73 6574  tings_dialog.set
-0000a210: 5374 796c 6553 6865 6574 2844 4152 4b5f  StyleSheet(DARK_
-0000a220: 5354 594c 4553 4845 4554 290a 2020 2020  STYLESHEET).    
-0000a230: 2020 2020 7365 6c66 2e73 6574 7469 6e67      self.setting
-0000a240: 735f 6469 616c 6f67 2e61 6363 6570 7465  s_dialog.accepte
-0000a250: 642e 636f 6e6e 6563 7428 7365 6c66 2e73  d.connect(self.s
-0000a260: 6176 655f 7365 7474 696e 6773 290a 2020  ave_settings).  
-0000a270: 2020 2020 2020 2320 6966 2073 656c 662e        # if self.
-0000a280: 7072 6566 2e67 6574 2822 6461 726b 5f6d  pref.get("dark_m
-0000a290: 6f64 6522 293a 0a20 2020 2020 2020 2023  ode"):.        #
-0000a2a0: 2020 2020 2073 656c 662e 7365 7474 696e       self.settin
-0000a2b0: 6773 5f64 6961 6c6f 672e 7365 7453 7479  gs_dialog.setSty
-0000a2c0: 6c65 5368 6565 7428 4441 524b 5f53 5459  leSheet(DARK_STY
-0000a2d0: 4c45 5348 4545 5429 0a0a 2020 2020 2020  LESHEET)..      
-0000a2e0: 2020 7365 6c66 2e73 6574 7469 6e67 735f    self.settings_
-0000a2f0: 6469 616c 6f67 2e43 616c 6c2e 7365 7454  dialog.Call.setT
-0000a300: 6578 7428 7365 6c66 2e73 7461 7469 6f6e  ext(self.station
-0000a310: 2e67 6574 2822 4361 6c6c 222c 2022 2229  .get("Call", "")
-0000a320: 290a 2020 2020 2020 2020 7365 6c66 2e73  ).        self.s
-0000a330: 6574 7469 6e67 735f 6469 616c 6f67 2e4e  ettings_dialog.N
-0000a340: 616d 652e 7365 7454 6578 7428 7365 6c66  ame.setText(self
-0000a350: 2e73 7461 7469 6f6e 2e67 6574 2822 4e61  .station.get("Na
-0000a360: 6d65 222c 2022 2229 290a 2020 2020 2020  me", "")).      
-0000a370: 2020 7365 6c66 2e73 6574 7469 6e67 735f    self.settings_
-0000a380: 6469 616c 6f67 2e41 6464 7265 7373 312e  dialog.Address1.
-0000a390: 7365 7454 6578 7428 7365 6c66 2e73 7461  setText(self.sta
-0000a3a0: 7469 6f6e 2e67 6574 2822 5374 7265 6574  tion.get("Street
-0000a3b0: 3122 2c20 2222 2929 0a20 2020 2020 2020  1", "")).       
-0000a3c0: 2073 656c 662e 7365 7474 696e 6773 5f64   self.settings_d
-0000a3d0: 6961 6c6f 672e 4164 6472 6573 7332 2e73  ialog.Address2.s
-0000a3e0: 6574 5465 7874 2873 656c 662e 7374 6174  etText(self.stat
-0000a3f0: 696f 6e2e 6765 7428 2253 7472 6565 7432  ion.get("Street2
-0000a400: 222c 2022 2229 290a 2020 2020 2020 2020  ", "")).        
-0000a410: 7365 6c66 2e73 6574 7469 6e67 735f 6469  self.settings_di
-0000a420: 616c 6f67 2e43 6974 792e 7365 7454 6578  alog.City.setTex
-0000a430: 7428 7365 6c66 2e73 7461 7469 6f6e 2e67  t(self.station.g
-0000a440: 6574 2822 4369 7479 222c 2022 2229 290a  et("City", "")).
-0000a450: 2020 2020 2020 2020 7365 6c66 2e73 6574          self.set
-0000a460: 7469 6e67 735f 6469 616c 6f67 2e53 7461  tings_dialog.Sta
-0000a470: 7465 2e73 6574 5465 7874 2873 656c 662e  te.setText(self.
-0000a480: 7374 6174 696f 6e2e 6765 7428 2253 7461  station.get("Sta
-0000a490: 7465 222c 2022 2229 290a 2020 2020 2020  te", "")).      
-0000a4a0: 2020 7365 6c66 2e73 6574 7469 6e67 735f    self.settings_
-0000a4b0: 6469 616c 6f67 2e5a 6970 2e73 6574 5465  dialog.Zip.setTe
-0000a4c0: 7874 2873 656c 662e 7374 6174 696f 6e2e  xt(self.station.
-0000a4d0: 6765 7428 225a 6970 222c 2022 2229 290a  get("Zip", "")).
-0000a4e0: 2020 2020 2020 2020 7365 6c66 2e73 6574          self.set
-0000a4f0: 7469 6e67 735f 6469 616c 6f67 2e43 6f75  tings_dialog.Cou
-0000a500: 6e74 7279 2e73 6574 5465 7874 2873 656c  ntry.setText(sel
-0000a510: 662e 7374 6174 696f 6e2e 6765 7428 2243  f.station.get("C
-0000a520: 6f75 6e74 7279 222c 2022 2229 290a 2020  ountry", "")).  
-0000a530: 2020 2020 2020 7365 6c66 2e73 6574 7469        self.setti
-0000a540: 6e67 735f 6469 616c 6f67 2e47 7269 6453  ngs_dialog.GridS
-0000a550: 7175 6172 652e 7365 7454 6578 7428 7365  quare.setText(se
-0000a560: 6c66 2e73 7461 7469 6f6e 2e67 6574 2822  lf.station.get("
-0000a570: 4772 6964 5371 7561 7265 222c 2022 2229  GridSquare", "")
-0000a580: 290a 2020 2020 2020 2020 7365 6c66 2e73  ).        self.s
-0000a590: 6574 7469 6e67 735f 6469 616c 6f67 2e43  ettings_dialog.C
-0000a5a0: 515a 6f6e 652e 7365 7454 6578 7428 7374  QZone.setText(st
-0000a5b0: 7228 7365 6c66 2e73 7461 7469 6f6e 2e67  r(self.station.g
-0000a5c0: 6574 2822 4351 5a6f 6e65 222c 2022 2229  et("CQZone", "")
-0000a5d0: 2929 0a20 2020 2020 2020 2073 656c 662e  )).        self.
-0000a5e0: 7365 7474 696e 6773 5f64 6961 6c6f 672e  settings_dialog.
-0000a5f0: 4954 555a 6f6e 652e 7365 7454 6578 7428  ITUZone.setText(
-0000a600: 7374 7228 7365 6c66 2e73 7461 7469 6f6e  str(self.station
-0000a610: 2e67 6574 2822 4941 5255 5a6f 6e65 222c  .get("IARUZone",
-0000a620: 2022 2229 2929 0a20 2020 2020 2020 2073   ""))).        s
-0000a630: 656c 662e 7365 7474 696e 6773 5f64 6961  elf.settings_dia
-0000a640: 6c6f 672e 4c69 6365 6e73 652e 7365 7454  log.License.setT
-0000a650: 6578 7428 7365 6c66 2e73 7461 7469 6f6e  ext(self.station
-0000a660: 2e67 6574 2822 4c69 6365 6e73 6543 6c61  .get("LicenseCla
-0000a670: 7373 222c 2022 2229 290a 2020 2020 2020  ss", "")).      
-0000a680: 2020 7365 6c66 2e73 6574 7469 6e67 735f    self.settings_
-0000a690: 6469 616c 6f67 2e4c 6174 6974 7564 652e  dialog.Latitude.
-0000a6a0: 7365 7454 6578 7428 7374 7228 7365 6c66  setText(str(self
-0000a6b0: 2e73 7461 7469 6f6e 2e67 6574 2822 4c61  .station.get("La
-0000a6c0: 7469 7475 6465 222c 2022 2229 2929 0a20  titude", ""))). 
-0000a6d0: 2020 2020 2020 2073 656c 662e 7365 7474         self.sett
-0000a6e0: 696e 6773 5f64 6961 6c6f 672e 4c6f 6e67  ings_dialog.Long
-0000a6f0: 6974 7564 652e 7365 7454 6578 7428 7374  itude.setText(st
-0000a700: 7228 7365 6c66 2e73 7461 7469 6f6e 2e67  r(self.station.g
-0000a710: 6574 2822 4c6f 6e67 6974 7564 6522 2c20  et("Longitude", 
-0000a720: 2222 2929 290a 2020 2020 2020 2020 7365  ""))).        se
-0000a730: 6c66 2e73 6574 7469 6e67 735f 6469 616c  lf.settings_dial
-0000a740: 6f67 2e53 7461 7469 6f6e 5458 5258 2e73  og.StationTXRX.s
-0000a750: 6574 5465 7874 2873 656c 662e 7374 6174  etText(self.stat
-0000a760: 696f 6e2e 6765 7428 2273 7461 7469 6f6e  ion.get("station
-0000a770: 7478 7278 222c 2022 2229 290a 2020 2020  txrx", "")).    
-0000a780: 2020 2020 7365 6c66 2e73 6574 7469 6e67      self.setting
-0000a790: 735f 6469 616c 6f67 2e50 6f77 6572 2e73  s_dialog.Power.s
-0000a7a0: 6574 5465 7874 2873 656c 662e 7374 6174  etText(self.stat
-0000a7b0: 696f 6e2e 6765 7428 2253 506f 7765 222c  ion.get("SPowe",
-0000a7c0: 2022 2229 290a 2020 2020 2020 2020 7365   "")).        se
-0000a7d0: 6c66 2e73 6574 7469 6e67 735f 6469 616c  lf.settings_dial
-0000a7e0: 6f67 2e41 6e74 656e 6e61 2e73 6574 5465  og.Antenna.setTe
-0000a7f0: 7874 2873 656c 662e 7374 6174 696f 6e2e  xt(self.station.
-0000a800: 6765 7428 2253 416e 7465 222c 2022 2229  get("SAnte", "")
-0000a810: 290a 2020 2020 2020 2020 7365 6c66 2e73  ).        self.s
-0000a820: 6574 7469 6e67 735f 6469 616c 6f67 2e41  ettings_dialog.A
-0000a830: 6e74 4865 6967 6874 2e73 6574 5465 7874  ntHeight.setText
-0000a840: 2873 656c 662e 7374 6174 696f 6e2e 6765  (self.station.ge
-0000a850: 7428 2253 416e 7448 3122 2c20 2222 2929  t("SAntH1", ""))
-0000a860: 0a20 2020 2020 2020 2073 656c 662e 7365  .        self.se
-0000a870: 7474 696e 6773 5f64 6961 6c6f 672e 4153  ttings_dialog.AS
-0000a880: 4c2e 7365 7454 6578 7428 7365 6c66 2e73  L.setText(self.s
-0000a890: 7461 7469 6f6e 2e67 6574 2822 5341 6e74  tation.get("SAnt
-0000a8a0: 4832 222c 2022 2229 290a 2020 2020 2020  H2", "")).      
-0000a8b0: 2020 7365 6c66 2e73 6574 7469 6e67 735f    self.settings_
-0000a8c0: 6469 616c 6f67 2e41 5252 4c53 6563 7469  dialog.ARRLSecti
-0000a8d0: 6f6e 2e73 6574 5465 7874 2873 656c 662e  on.setText(self.
-0000a8e0: 7374 6174 696f 6e2e 6765 7428 2241 5252  station.get("ARR
-0000a8f0: 4c53 6563 7469 6f6e 222c 2022 2229 290a  LSection", "")).
-0000a900: 2020 2020 2020 2020 7365 6c66 2e73 6574          self.set
-0000a910: 7469 6e67 735f 6469 616c 6f67 2e52 6f76  tings_dialog.Rov
-0000a920: 6572 5154 482e 7365 7454 6578 7428 7365  erQTH.setText(se
-0000a930: 6c66 2e73 7461 7469 6f6e 2e67 6574 2822  lf.station.get("
-0000a940: 526f 7665 7251 5448 222c 2022 2229 290a  RoverQTH", "")).
-0000a950: 2020 2020 2020 2020 7365 6c66 2e73 6574          self.set
-0000a960: 7469 6e67 735f 6469 616c 6f67 2e43 6c75  tings_dialog.Clu
-0000a970: 622e 7365 7454 6578 7428 7365 6c66 2e73  b.setText(self.s
-0000a980: 7461 7469 6f6e 2e67 6574 2822 436c 7562  tation.get("Club
-0000a990: 222c 2022 2229 290a 2020 2020 2020 2020  ", "")).        
-0000a9a0: 7365 6c66 2e73 6574 7469 6e67 735f 6469  self.settings_di
-0000a9b0: 616c 6f67 2e45 6d61 696c 2e73 6574 5465  alog.Email.setTe
-0000a9c0: 7874 2873 656c 662e 7374 6174 696f 6e2e  xt(self.station.
-0000a9d0: 6765 7428 2245 6d61 696c 222c 2022 2229  get("Email", "")
-0000a9e0: 290a 2020 2020 2020 2020 7365 6c66 2e73  ).        self.s
-0000a9f0: 6574 7469 6e67 735f 6469 616c 6f67 2e6f  ettings_dialog.o
-0000aa00: 7065 6e28 290a 0a20 2020 2064 6566 2073  pen()..    def s
-0000aa10: 6176 655f 7365 7474 696e 6773 2873 656c  ave_settings(sel
-0000aa20: 6629 3a0a 2020 2020 2020 2020 2222 2253  f):.        """S
-0000aa30: 6176 6520 7365 7474 696e 6773 2222 220a  ave settings""".
-0000aa40: 2020 2020 2020 2020 6373 203d 2073 656c          cs = sel
-0000aa50: 662e 7365 7474 696e 6773 5f64 6961 6c6f  f.settings_dialo
-0000aa60: 672e 4361 6c6c 2e74 6578 7428 290a 2020  g.Call.text().  
-0000aa70: 2020 2020 2020 7365 6c66 2e73 7461 7469        self.stati
-0000aa80: 6f6e 203d 207b 7d0a 2020 2020 2020 2020  on = {}.        
-0000aa90: 7365 6c66 2e73 7461 7469 6f6e 5b22 4361  self.station["Ca
-0000aaa0: 6c6c 225d 203d 2063 732e 7570 7065 7228  ll"] = cs.upper(
-0000aab0: 290a 2020 2020 2020 2020 7365 6c66 2e73  ).        self.s
-0000aac0: 7461 7469 6f6e 5b22 4e61 6d65 225d 203d  tation["Name"] =
-0000aad0: 2073 656c 662e 7365 7474 696e 6773 5f64   self.settings_d
-0000aae0: 6961 6c6f 672e 4e61 6d65 2e74 6578 7428  ialog.Name.text(
-0000aaf0: 292e 7469 746c 6528 290a 2020 2020 2020  ).title().      
-0000ab00: 2020 7365 6c66 2e73 7461 7469 6f6e 5b22    self.station["
-0000ab10: 5374 7265 6574 3122 5d20 3d20 7365 6c66  Street1"] = self
-0000ab20: 2e73 6574 7469 6e67 735f 6469 616c 6f67  .settings_dialog
-0000ab30: 2e41 6464 7265 7373 312e 7465 7874 2829  .Address1.text()
-0000ab40: 2e74 6974 6c65 2829 0a20 2020 2020 2020  .title().       
-0000ab50: 2073 656c 662e 7374 6174 696f 6e5b 2253   self.station["S
-0000ab60: 7472 6565 7432 225d 203d 2073 656c 662e  treet2"] = self.
-0000ab70: 7365 7474 696e 6773 5f64 6961 6c6f 672e  settings_dialog.
-0000ab80: 4164 6472 6573 7332 2e74 6578 7428 292e  Address2.text().
-0000ab90: 7469 746c 6528 290a 2020 2020 2020 2020  title().        
-0000aba0: 7365 6c66 2e73 7461 7469 6f6e 5b22 4369  self.station["Ci
-0000abb0: 7479 225d 203d 2073 656c 662e 7365 7474  ty"] = self.sett
-0000abc0: 696e 6773 5f64 6961 6c6f 672e 4369 7479  ings_dialog.City
-0000abd0: 2e74 6578 7428 292e 7469 746c 6528 290a  .text().title().
-0000abe0: 2020 2020 2020 2020 7365 6c66 2e73 7461          self.sta
-0000abf0: 7469 6f6e 5b22 5374 6174 6522 5d20 3d20  tion["State"] = 
-0000ac00: 7365 6c66 2e73 6574 7469 6e67 735f 6469  self.settings_di
-0000ac10: 616c 6f67 2e53 7461 7465 2e74 6578 7428  alog.State.text(
-0000ac20: 292e 7570 7065 7228 290a 2020 2020 2020  ).upper().      
-0000ac30: 2020 7365 6c66 2e73 7461 7469 6f6e 5b22    self.station["
-0000ac40: 5a69 7022 5d20 3d20 7365 6c66 2e73 6574  Zip"] = self.set
-0000ac50: 7469 6e67 735f 6469 616c 6f67 2e5a 6970  tings_dialog.Zip
-0000ac60: 2e74 6578 7428 290a 2020 2020 2020 2020  .text().        
-0000ac70: 7365 6c66 2e73 7461 7469 6f6e 5b22 436f  self.station["Co
-0000ac80: 756e 7472 7922 5d20 3d20 7365 6c66 2e73  untry"] = self.s
-0000ac90: 6574 7469 6e67 735f 6469 616c 6f67 2e43  ettings_dialog.C
-0000aca0: 6f75 6e74 7279 2e74 6578 7428 292e 7469  ountry.text().ti
-0000acb0: 746c 6528 290a 2020 2020 2020 2020 7365  tle().        se
-0000acc0: 6c66 2e73 7461 7469 6f6e 5b22 4772 6964  lf.station["Grid
-0000acd0: 5371 7561 7265 225d 203d 2073 656c 662e  Square"] = self.
-0000ace0: 7365 7474 696e 6773 5f64 6961 6c6f 672e  settings_dialog.
-0000acf0: 4772 6964 5371 7561 7265 2e74 6578 7428  GridSquare.text(
-0000ad00: 290a 2020 2020 2020 2020 7365 6c66 2e73  ).        self.s
-0000ad10: 7461 7469 6f6e 5b22 4351 5a6f 6e65 225d  tation["CQZone"]
-0000ad20: 203d 2073 656c 662e 7365 7474 696e 6773   = self.settings
-0000ad30: 5f64 6961 6c6f 672e 4351 5a6f 6e65 2e74  _dialog.CQZone.t
-0000ad40: 6578 7428 290a 2020 2020 2020 2020 7365  ext().        se
-0000ad50: 6c66 2e73 7461 7469 6f6e 5b22 4941 5255  lf.station["IARU
-0000ad60: 5a6f 6e65 225d 203d 2073 656c 662e 7365  Zone"] = self.se
-0000ad70: 7474 696e 6773 5f64 6961 6c6f 672e 4954  ttings_dialog.IT
-0000ad80: 555a 6f6e 652e 7465 7874 2829 0a20 2020  UZone.text().   
-0000ad90: 2020 2020 2073 656c 662e 7374 6174 696f       self.statio
-0000ada0: 6e5b 224c 6963 656e 7365 436c 6173 7322  n["LicenseClass"
-0000adb0: 5d20 3d20 7365 6c66 2e73 6574 7469 6e67  ] = self.setting
-0000adc0: 735f 6469 616c 6f67 2e4c 6963 656e 7365  s_dialog.License
-0000add0: 2e74 6578 7428 292e 7469 746c 6528 290a  .text().title().
-0000ade0: 2020 2020 2020 2020 7365 6c66 2e73 7461          self.sta
-0000adf0: 7469 6f6e 5b22 4c61 7469 7475 6465 225d  tion["Latitude"]
-0000ae00: 203d 2073 656c 662e 7365 7474 696e 6773   = self.settings
-0000ae10: 5f64 6961 6c6f 672e 4c61 7469 7475 6465  _dialog.Latitude
-0000ae20: 2e74 6578 7428 290a 2020 2020 2020 2020  .text().        
-0000ae30: 7365 6c66 2e73 7461 7469 6f6e 5b22 4c6f  self.station["Lo
-0000ae40: 6e67 6974 7564 6522 5d20 3d20 7365 6c66  ngitude"] = self
-0000ae50: 2e73 6574 7469 6e67 735f 6469 616c 6f67  .settings_dialog
-0000ae60: 2e4c 6f6e 6769 7475 6465 2e74 6578 7428  .Longitude.text(
-0000ae70: 290a 2020 2020 2020 2020 7365 6c66 2e73  ).        self.s
-0000ae80: 7461 7469 6f6e 5b22 5354 5865 7122 5d20  tation["STXeq"] 
-0000ae90: 3d20 7365 6c66 2e73 6574 7469 6e67 735f  = self.settings_
-0000aea0: 6469 616c 6f67 2e53 7461 7469 6f6e 5458  dialog.StationTX
-0000aeb0: 5258 2e74 6578 7428 290a 2020 2020 2020  RX.text().      
-0000aec0: 2020 7365 6c66 2e73 7461 7469 6f6e 5b22    self.station["
-0000aed0: 5350 6f77 6522 5d20 3d20 7365 6c66 2e73  SPowe"] = self.s
-0000aee0: 6574 7469 6e67 735f 6469 616c 6f67 2e50  ettings_dialog.P
-0000aef0: 6f77 6572 2e74 6578 7428 290a 2020 2020  ower.text().    
-0000af00: 2020 2020 7365 6c66 2e73 7461 7469 6f6e      self.station
-0000af10: 5b22 5341 6e74 6522 5d20 3d20 7365 6c66  ["SAnte"] = self
-0000af20: 2e73 6574 7469 6e67 735f 6469 616c 6f67  .settings_dialog
-0000af30: 2e41 6e74 656e 6e61 2e74 6578 7428 290a  .Antenna.text().
-0000af40: 2020 2020 2020 2020 7365 6c66 2e73 7461          self.sta
-0000af50: 7469 6f6e 5b22 5341 6e74 4831 225d 203d  tion["SAntH1"] =
-0000af60: 2073 656c 662e 7365 7474 696e 6773 5f64   self.settings_d
-0000af70: 6961 6c6f 672e 416e 7448 6569 6768 742e  ialog.AntHeight.
-0000af80: 7465 7874 2829 0a20 2020 2020 2020 2073  text().        s
-0000af90: 656c 662e 7374 6174 696f 6e5b 2253 416e  elf.station["SAn
-0000afa0: 7448 3222 5d20 3d20 7365 6c66 2e73 6574  tH2"] = self.set
-0000afb0: 7469 6e67 735f 6469 616c 6f67 2e41 534c  tings_dialog.ASL
-0000afc0: 2e74 6578 7428 290a 2020 2020 2020 2020  .text().        
-0000afd0: 7365 6c66 2e73 7461 7469 6f6e 5b22 4152  self.station["AR
-0000afe0: 524c 5365 6374 696f 6e22 5d20 3d20 7365  RLSection"] = se
-0000aff0: 6c66 2e73 6574 7469 6e67 735f 6469 616c  lf.settings_dial
-0000b000: 6f67 2e41 5252 4c53 6563 7469 6f6e 2e74  og.ARRLSection.t
-0000b010: 6578 7428 292e 7570 7065 7228 290a 2020  ext().upper().  
-0000b020: 2020 2020 2020 7365 6c66 2e73 7461 7469        self.stati
-0000b030: 6f6e 5b22 526f 7665 7251 5448 225d 203d  on["RoverQTH"] =
-0000b040: 2073 656c 662e 7365 7474 696e 6773 5f64   self.settings_d
-0000b050: 6961 6c6f 672e 526f 7665 7251 5448 2e74  ialog.RoverQTH.t
-0000b060: 6578 7428 290a 2020 2020 2020 2020 7365  ext().        se
-0000b070: 6c66 2e73 7461 7469 6f6e 5b22 436c 7562  lf.station["Club
-0000b080: 225d 203d 2073 656c 662e 7365 7474 696e  "] = self.settin
-0000b090: 6773 5f64 6961 6c6f 672e 436c 7562 2e74  gs_dialog.Club.t
-0000b0a0: 6578 7428 292e 7469 746c 6528 290a 2020  ext().title().  
-0000b0b0: 2020 2020 2020 7365 6c66 2e73 7461 7469        self.stati
-0000b0c0: 6f6e 5b22 456d 6169 6c22 5d20 3d20 7365  on["Email"] = se
-0000b0d0: 6c66 2e73 6574 7469 6e67 735f 6469 616c  lf.settings_dial
-0000b0e0: 6f67 2e45 6d61 696c 2e74 6578 7428 290a  og.Email.text().
-0000b0f0: 2020 2020 2020 2020 7365 6c66 2e64 6174          self.dat
-0000b100: 6162 6173 652e 6164 645f 7374 6174 696f  abase.add_statio
-0000b110: 6e28 7365 6c66 2e73 7461 7469 6f6e 290a  n(self.station).
-0000b120: 2020 2020 2020 2020 7365 6c66 2e73 6574          self.set
-0000b130: 7469 6e67 735f 6469 616c 6f67 2e63 6c6f  tings_dialog.clo
-0000b140: 7365 2829 0a20 2020 2020 2020 2069 6620  se().        if 
-0000b150: 7365 6c66 2e63 7572 7265 6e74 5f6f 7020  self.current_op 
-0000b160: 3d3d 2022 223a 0a20 2020 2020 2020 2020  == "":.         
-0000b170: 2020 2073 656c 662e 6375 7272 656e 745f     self.current_
-0000b180: 6f70 203d 2073 656c 662e 7374 6174 696f  op = self.statio
-0000b190: 6e2e 6765 7428 2243 616c 6c22 2c20 2222  n.get("Call", ""
-0000b1a0: 290a 2020 2020 2020 2020 2020 2020 7365  ).            se
-0000b1b0: 6c66 2e6d 616b 655f 6f70 5f64 6972 2829  lf.make_op_dir()
-0000b1c0: 0a20 2020 2020 2020 2063 6f6e 7465 7374  .        contest
-0000b1d0: 5f63 6f75 6e74 203d 2073 656c 662e 6461  _count = self.da
-0000b1e0: 7461 6261 7365 2e66 6574 6368 5f61 6c6c  tabase.fetch_all
-0000b1f0: 5f63 6f6e 7465 7374 7328 290a 2020 2020  _contests().    
-0000b200: 2020 2020 6966 206c 656e 2863 6f6e 7465      if len(conte
-0000b210: 7374 5f63 6f75 6e74 2920 3d3d 2030 3a0a  st_count) == 0:.
-0000b220: 2020 2020 2020 2020 2020 2020 7365 6c66              self
-0000b230: 2e6e 6577 5f63 6f6e 7465 7374 5f64 6961  .new_contest_dia
-0000b240: 6c6f 6728 290a 0a20 2020 2064 6566 2065  log()..    def e
-0000b250: 6469 745f 6d61 6372 6f28 7365 6c66 2c20  dit_macro(self, 
-0000b260: 6675 6e63 7469 6f6e 5f6b 6579 293a 0a20  function_key):. 
-0000b270: 2020 2020 2020 2022 2222 5368 6f77 2065         """Show e
-0000b280: 6469 7420 6d61 6372 6f20 6469 616c 6f67  dit macro dialog
-0000b290: 2222 220a 2020 2020 2020 2020 7365 6c66  """.        self
-0000b2a0: 2e65 6469 745f 6d61 6372 6f5f 6469 616c  .edit_macro_dial
-0000b2b0: 6f67 203d 2045 6469 744d 6163 726f 2866  og = EditMacro(f
-0000b2c0: 756e 6374 696f 6e5f 6b65 792c 2057 4f52  unction_key, WOR
-0000b2d0: 4b49 4e47 5f50 4154 4829 0a20 2020 2020  KING_PATH).     
-0000b2e0: 2020 2073 656c 662e 6564 6974 5f6d 6163     self.edit_mac
-0000b2f0: 726f 5f64 6961 6c6f 672e 6163 6365 7074  ro_dialog.accept
-0000b300: 6564 2e63 6f6e 6e65 6374 2873 656c 662e  ed.connect(self.
-0000b310: 6564 6974 6564 5f6d 6163 726f 290a 2020  edited_macro).  
-0000b320: 2020 2020 2020 6966 2073 656c 662e 7072        if self.pr
-0000b330: 6566 2e67 6574 2822 6461 726b 5f6d 6f64  ef.get("dark_mod
-0000b340: 6522 293a 0a20 2020 2020 2020 2020 2020  e"):.           
-0000b350: 2073 656c 662e 6564 6974 5f6d 6163 726f   self.edit_macro
-0000b360: 5f64 6961 6c6f 672e 7365 7453 7479 6c65  _dialog.setStyle
-0000b370: 5368 6565 7428 4441 524b 5f53 5459 4c45  Sheet(DARK_STYLE
-0000b380: 5348 4545 5429 0a20 2020 2020 2020 2073  SHEET).        s
-0000b390: 656c 662e 6564 6974 5f6d 6163 726f 5f64  elf.edit_macro_d
-0000b3a0: 6961 6c6f 672e 6f70 656e 2829 0a0a 2020  ialog.open()..  
-0000b3b0: 2020 6465 6620 6564 6974 6564 5f6d 6163    def edited_mac
-0000b3c0: 726f 2873 656c 6629 3a0a 2020 2020 2020  ro(self):.      
-0000b3d0: 2020 2222 2253 6176 6520 6564 6974 6564    """Save edited
-0000b3e0: 206d 6163 726f 2222 220a 2020 2020 2020   macro""".      
-0000b3f0: 2020 7365 6c66 2e65 6469 745f 6d61 6372    self.edit_macr
-0000b400: 6f5f 6469 616c 6f67 2e66 756e 6374 696f  o_dialog.functio
-0000b410: 6e5f 6b65 792e 7365 7454 6578 7428 0a20  n_key.setText(. 
-0000b420: 2020 2020 2020 2020 2020 2073 656c 662e             self.
-0000b430: 6564 6974 5f6d 6163 726f 5f64 6961 6c6f  edit_macro_dialo
-0000b440: 672e 6d61 6372 6f5f 6c61 6265 6c2e 7465  g.macro_label.te
-0000b450: 7874 2829 0a20 2020 2020 2020 2029 0a20  xt().        ). 
-0000b460: 2020 2020 2020 2073 656c 662e 6564 6974         self.edit
-0000b470: 5f6d 6163 726f 5f64 6961 6c6f 672e 6675  _macro_dialog.fu
-0000b480: 6e63 7469 6f6e 5f6b 6579 2e73 6574 546f  nction_key.setTo
-0000b490: 6f6c 5469 7028 0a20 2020 2020 2020 2020  olTip(.         
-0000b4a0: 2020 2073 656c 662e 6564 6974 5f6d 6163     self.edit_mac
-0000b4b0: 726f 5f64 6961 6c6f 672e 7468 655f 6d61  ro_dialog.the_ma
-0000b4c0: 6372 6f2e 7465 7874 2829 0a20 2020 2020  cro.text().     
-0000b4d0: 2020 2029 0a20 2020 2020 2020 2073 656c     ).        sel
-0000b4e0: 662e 6564 6974 5f6d 6163 726f 5f64 6961  f.edit_macro_dia
-0000b4f0: 6c6f 672e 636c 6f73 6528 290a 0a20 2020  log.close()..   
-0000b500: 2064 6566 2065 6469 745f 4631 2873 656c   def edit_F1(sel
-0000b510: 6629 3a0a 2020 2020 2020 2020 2222 2273  f):.        """s
-0000b520: 7475 6222 2222 0a20 2020 2020 2020 206c  tub""".        l
-0000b530: 6f67 6765 722e 6465 6275 6728 2246 3120  ogger.debug("F1 
-0000b540: 5269 6768 7420 436c 6963 6b65 642e 2229  Right Clicked.")
-0000b550: 0a20 2020 2020 2020 2073 656c 662e 6564  .        self.ed
-0000b560: 6974 5f6d 6163 726f 2873 656c 662e 4631  it_macro(self.F1
-0000b570: 290a 0a20 2020 2064 6566 2065 6469 745f  )..    def edit_
-0000b580: 4632 2873 656c 6629 3a0a 2020 2020 2020  F2(self):.      
-0000b590: 2020 2222 2273 7475 6222 2222 0a20 2020    """stub""".   
-0000b5a0: 2020 2020 206c 6f67 6765 722e 6465 6275       logger.debu
-0000b5b0: 6728 2246 3220 5269 6768 7420 436c 6963  g("F2 Right Clic
-0000b5c0: 6b65 642e 2229 0a20 2020 2020 2020 2073  ked.").        s
-0000b5d0: 656c 662e 6564 6974 5f6d 6163 726f 2873  elf.edit_macro(s
-0000b5e0: 656c 662e 4632 290a 0a20 2020 2064 6566  elf.F2)..    def
-0000b5f0: 2065 6469 745f 4633 2873 656c 6629 3a0a   edit_F3(self):.
-0000b600: 2020 2020 2020 2020 2222 2273 7475 6222          """stub"
-0000b610: 2222 0a20 2020 2020 2020 206c 6f67 6765  "".        logge
-0000b620: 722e 6465 6275 6728 2246 3320 5269 6768  r.debug("F3 Righ
-0000b630: 7420 436c 6963 6b65 642e 2229 0a20 2020  t Clicked.").   
-0000b640: 2020 2020 2073 656c 662e 6564 6974 5f6d       self.edit_m
-0000b650: 6163 726f 2873 656c 662e 4633 290a 0a20  acro(self.F3).. 
-0000b660: 2020 2064 6566 2065 6469 745f 4634 2873     def edit_F4(s
-0000b670: 656c 6629 3a0a 2020 2020 2020 2020 2222  elf):.        ""
-0000b680: 2273 7475 6222 2222 0a20 2020 2020 2020  "stub""".       
-0000b690: 206c 6f67 6765 722e 6465 6275 6728 2246   logger.debug("F
-0000b6a0: 3420 5269 6768 7420 436c 6963 6b65 642e  4 Right Clicked.
-0000b6b0: 2229 0a20 2020 2020 2020 2073 656c 662e  ").        self.
-0000b6c0: 6564 6974 5f6d 6163 726f 2873 656c 662e  edit_macro(self.
-0000b6d0: 4634 290a 0a20 2020 2064 6566 2065 6469  F4)..    def edi
-0000b6e0: 745f 4635 2873 656c 6629 3a0a 2020 2020  t_F5(self):.    
-0000b6f0: 2020 2020 2222 2273 7475 6222 2222 0a20      """stub""". 
-0000b700: 2020 2020 2020 206c 6f67 6765 722e 6465         logger.de
-0000b710: 6275 6728 2246 3520 5269 6768 7420 436c  bug("F5 Right Cl
-0000b720: 6963 6b65 642e 2229 0a20 2020 2020 2020  icked.").       
-0000b730: 2073 656c 662e 6564 6974 5f6d 6163 726f   self.edit_macro
-0000b740: 2873 656c 662e 4635 290a 0a20 2020 2064  (self.F5)..    d
-0000b750: 6566 2065 6469 745f 4636 2873 656c 6629  ef edit_F6(self)
-0000b760: 3a0a 2020 2020 2020 2020 2222 2273 7475  :.        """stu
-0000b770: 6222 2222 0a20 2020 2020 2020 206c 6f67  b""".        log
-0000b780: 6765 722e 6465 6275 6728 2246 3620 5269  ger.debug("F6 Ri
-0000b790: 6768 7420 436c 6963 6b65 642e 2229 0a20  ght Clicked."). 
-0000b7a0: 2020 2020 2020 2073 656c 662e 6564 6974         self.edit
-0000b7b0: 5f6d 6163 726f 2873 656c 662e 4636 290a  _macro(self.F6).
-0000b7c0: 0a20 2020 2064 6566 2065 6469 745f 4637  .    def edit_F7
-0000b7d0: 2873 656c 6629 3a0a 2020 2020 2020 2020  (self):.        
-0000b7e0: 2222 2273 7475 6222 2222 0a20 2020 2020  """stub""".     
-0000b7f0: 2020 206c 6f67 6765 722e 6465 6275 6728     logger.debug(
-0000b800: 2246 3720 5269 6768 7420 436c 6963 6b65  "F7 Right Clicke
-0000b810: 642e 2229 0a20 2020 2020 2020 2073 656c  d.").        sel
-0000b820: 662e 6564 6974 5f6d 6163 726f 2873 656c  f.edit_macro(sel
-0000b830: 662e 4637 290a 0a20 2020 2064 6566 2065  f.F7)..    def e
-0000b840: 6469 745f 4638 2873 656c 6629 3a0a 2020  dit_F8(self):.  
-0000b850: 2020 2020 2020 2222 2273 7475 6222 2222        """stub"""
-0000b860: 0a20 2020 2020 2020 206c 6f67 6765 722e  .        logger.
-0000b870: 6465 6275 6728 2246 3820 5269 6768 7420  debug("F8 Right 
-0000b880: 436c 6963 6b65 642e 2229 0a20 2020 2020  Clicked.").     
-0000b890: 2020 2073 656c 662e 6564 6974 5f6d 6163     self.edit_mac
-0000b8a0: 726f 2873 656c 662e 4638 290a 0a20 2020  ro(self.F8)..   
-0000b8b0: 2064 6566 2065 6469 745f 4639 2873 656c   def edit_F9(sel
-0000b8c0: 6629 3a0a 2020 2020 2020 2020 2222 2273  f):.        """s
-0000b8d0: 7475 6222 2222 0a20 2020 2020 2020 206c  tub""".        l
-0000b8e0: 6f67 6765 722e 6465 6275 6728 2246 3920  ogger.debug("F9 
-0000b8f0: 5269 6768 7420 436c 6963 6b65 642e 2229  Right Clicked.")
-0000b900: 0a20 2020 2020 2020 2073 656c 662e 6564  .        self.ed
-0000b910: 6974 5f6d 6163 726f 2873 656c 662e 4639  it_macro(self.F9
-0000b920: 290a 0a20 2020 2064 6566 2065 6469 745f  )..    def edit_
-0000b930: 4631 3028 7365 6c66 293a 0a20 2020 2020  F10(self):.     
-0000b940: 2020 2022 2222 7374 7562 2222 220a 2020     """stub""".  
-0000b950: 2020 2020 2020 6c6f 6767 6572 2e64 6562        logger.deb
-0000b960: 7567 2822 4631 3020 5269 6768 7420 436c  ug("F10 Right Cl
-0000b970: 6963 6b65 642e 2229 0a20 2020 2020 2020  icked.").       
-0000b980: 2073 656c 662e 6564 6974 5f6d 6163 726f   self.edit_macro
-0000b990: 2873 656c 662e 4631 3029 0a0a 2020 2020  (self.F10)..    
-0000b9a0: 6465 6620 6564 6974 5f46 3131 2873 656c  def edit_F11(sel
-0000b9b0: 6629 3a0a 2020 2020 2020 2020 2222 2273  f):.        """s
-0000b9c0: 7475 6222 2222 0a20 2020 2020 2020 206c  tub""".        l
-0000b9d0: 6f67 6765 722e 6465 6275 6728 2246 3131  ogger.debug("F11
-0000b9e0: 2052 6967 6874 2043 6c69 636b 6564 2e22   Right Clicked."
-0000b9f0: 290a 2020 2020 2020 2020 7365 6c66 2e65  ).        self.e
-0000ba00: 6469 745f 6d61 6372 6f28 7365 6c66 2e46  dit_macro(self.F
-0000ba10: 3131 290a 0a20 2020 2064 6566 2065 6469  11)..    def edi
-0000ba20: 745f 4631 3228 7365 6c66 293a 0a20 2020  t_F12(self):.   
-0000ba30: 2020 2020 2022 2222 7374 7562 2222 220a       """stub""".
-0000ba40: 2020 2020 2020 2020 6c6f 6767 6572 2e64          logger.d
-0000ba50: 6562 7567 2822 4631 3220 5269 6768 7420  ebug("F12 Right 
-0000ba60: 436c 6963 6b65 642e 2229 0a20 2020 2020  Clicked.").     
-0000ba70: 2020 2073 656c 662e 6564 6974 5f6d 6163     self.edit_mac
-0000ba80: 726f 2873 656c 662e 4631 3229 0a0a 2020  ro(self.F12)..  
-0000ba90: 2020 6465 6620 7072 6f63 6573 735f 6d61    def process_ma
-0000baa0: 6372 6f28 7365 6c66 2c20 6d61 6372 6f3a  cro(self, macro:
-0000bab0: 2073 7472 2920 2d3e 2073 7472 3a0a 2020   str) -> str:.  
-0000bac0: 2020 2020 2020 2222 2250 726f 6365 7373        """Process
-0000bad0: 2043 5720 6d61 6372 6f20 7375 6273 7469   CW macro substi
-0000bae0: 7475 7469 6f6e 7322 2222 0a20 2020 2020  tutions""".     
-0000baf0: 2020 2072 6573 756c 7420 3d20 7365 6c66     result = self
-0000bb00: 2e64 6174 6162 6173 652e 6765 745f 7365  .database.get_se
-0000bb10: 7269 616c 2829 0a20 2020 2020 2020 206e  rial().        n
-0000bb20: 6578 745f 7365 7269 616c 203d 2073 7472  ext_serial = str
-0000bb30: 2872 6573 756c 742e 6765 7428 2273 6572  (result.get("ser
-0000bb40: 6961 6c5f 6e72 222c 2022 3122 2929 0a20  ial_nr", "1")). 
-0000bb50: 2020 2020 2020 2069 6620 6e65 7874 5f73         if next_s
-0000bb60: 6572 6961 6c20 3d3d 2022 4e6f 6e65 223a  erial == "None":
-0000bb70: 0a20 2020 2020 2020 2020 2020 206e 6578  .            nex
-0000bb80: 745f 7365 7269 616c 203d 2022 3122 0a20  t_serial = "1". 
-0000bb90: 2020 2020 2020 206d 6163 726f 203d 206d         macro = m
-0000bba0: 6163 726f 2e75 7070 6572 2829 0a20 2020  acro.upper().   
-0000bbb0: 2020 2020 206d 6163 726f 203d 206d 6163       macro = mac
-0000bbc0: 726f 2e72 6570 6c61 6365 2822 2322 2c20  ro.replace("#", 
-0000bbd0: 6e65 7874 5f73 6572 6961 6c29 0a20 2020  next_serial).   
-0000bbe0: 2020 2020 206d 6163 726f 203d 206d 6163       macro = mac
-0000bbf0: 726f 2e72 6570 6c61 6365 2822 7b4d 5943  ro.replace("{MYC
-0000bc00: 414c 4c7d 222c 2073 656c 662e 7374 6174  ALL}", self.stat
-0000bc10: 696f 6e2e 6765 7428 2243 616c 6c22 2c20  ion.get("Call", 
-0000bc20: 2222 2929 0a20 2020 2020 2020 206d 6163  "")).        mac
-0000bc30: 726f 203d 206d 6163 726f 2e72 6570 6c61  ro = macro.repla
-0000bc40: 6365 2822 7b48 4953 4341 4c4c 7d22 2c20  ce("{HISCALL}", 
-0000bc50: 7365 6c66 2e63 616c 6c73 6967 6e2e 7465  self.callsign.te
-0000bc60: 7874 2829 290a 2020 2020 2020 2020 6966  xt()).        if
-0000bc70: 2073 656c 662e 7261 6469 6f5f 7374 6174   self.radio_stat
-0000bc80: 652e 6765 7428 226d 6f64 6522 2920 3d3d  e.get("mode") ==
-0000bc90: 2022 4357 223a 0a20 2020 2020 2020 2020   "CW":.         
-0000bca0: 2020 206d 6163 726f 203d 206d 6163 726f     macro = macro
-0000bcb0: 2e72 6570 6c61 6365 2822 7b53 4e54 7d22  .replace("{SNT}"
-0000bcc0: 2c20 7365 6c66 2e73 656e 742e 7465 7874  , self.sent.text
-0000bcd0: 2829 2e72 6570 6c61 6365 2822 3922 2c20  ().replace("9", 
-0000bce0: 226e 2229 290a 2020 2020 2020 2020 656c  "n")).        el
-0000bcf0: 7365 3a0a 2020 2020 2020 2020 2020 2020  se:.            
-0000bd00: 6d61 6372 6f20 3d20 6d61 6372 6f2e 7265  macro = macro.re
-0000bd10: 706c 6163 6528 227b 534e 547d 222c 2073  place("{SNT}", s
-0000bd20: 656c 662e 7365 6e74 2e74 6578 7428 2929  elf.sent.text())
-0000bd30: 0a20 2020 2020 2020 206d 6163 726f 203d  .        macro =
-0000bd40: 206d 6163 726f 2e72 6570 6c61 6365 2822   macro.replace("
-0000bd50: 7b53 454e 544e 527d 222c 2073 656c 662e  {SENTNR}", self.
-0000bd60: 6f74 6865 725f 312e 7465 7874 2829 290a  other_1.text()).
-0000bd70: 2020 2020 2020 2020 6d61 6372 6f20 3d20          macro = 
-0000bd80: 6d61 6372 6f2e 7265 706c 6163 6528 0a20  macro.replace(. 
-0000bd90: 2020 2020 2020 2020 2020 2022 7b45 5843             "{EXC
-0000bda0: 487d 222c 2073 656c 662e 636f 6e74 6573  H}", self.contes
-0000bdb0: 745f 7365 7474 696e 6773 2e67 6574 2822  t_settings.get("
-0000bdc0: 5365 6e74 4578 6368 616e 6765 222c 2022  SentExchange", "
-0000bdd0: 7878 7822 290a 2020 2020 2020 2020 290a  xxx").        ).
-0000bde0: 2020 2020 2020 2020 7265 7475 726e 206d          return m
-0000bdf0: 6163 726f 0a0a 2020 2020 6465 6620 766f  acro..    def vo
-0000be00: 6963 655f 7374 7269 6e67 2873 656c 662c  ice_string(self,
-0000be10: 2074 6865 5f73 7472 696e 673a 2073 7472   the_string: str
-0000be20: 2920 2d3e 204e 6f6e 653a 0a20 2020 2020  ) -> None:.     
-0000be30: 2020 2022 2222 766f 6963 6573 2073 7472     """voices str
-0000be40: 696e 6720 7573 696e 6720 6e61 746f 2070  ing using nato p
-0000be50: 686f 6e65 7469 6373 2222 220a 2020 2020  honetics""".    
-0000be60: 2020 2020 6c6f 6767 6572 2e64 6562 7567      logger.debug
-0000be70: 2822 566f 6963 696e 673a 2025 7322 2c20  ("Voicing: %s", 
-0000be80: 7468 655f 7374 7269 6e67 290a 2020 2020  the_string).    
-0000be90: 2020 2020 6f70 5f70 6174 6820 3d20 5061      op_path = Pa
-0000bea0: 7468 2844 4154 415f 5041 5448 2920 2f20  th(DATA_PATH) / 
-0000beb0: 7365 6c66 2e63 7572 7265 6e74 5f6f 700a  self.current_op.
-0000bec0: 2020 2020 2020 2020 6966 2022 5b22 2069          if "[" i
-0000bed0: 6e20 7468 655f 7374 7269 6e67 3a0a 2020  n the_string:.  
-0000bee0: 2020 2020 2020 2020 2020 7375 625f 7374            sub_st
-0000bef0: 7269 6e67 203d 2074 6865 5f73 7472 696e  ring = the_strin
-0000bf00: 672e 7374 7269 7028 225b 5d22 292e 6c6f  g.strip("[]").lo
-0000bf10: 7765 7228 290a 2020 2020 2020 2020 2020  wer().          
-0000bf20: 2020 6669 6c65 6e61 6d65 203d 2066 227b    filename = f"{
-0000bf30: 7374 7228 6f70 5f70 6174 6829 7d2f 7b73  str(op_path)}/{s
-0000bf40: 7562 5f73 7472 696e 677d 2e77 6176 220a  ub_string}.wav".
-0000bf50: 2020 2020 2020 2020 2020 2020 6966 2050              if P
-0000bf60: 6174 6828 6669 6c65 6e61 6d65 292e 6973  ath(filename).is
-0000bf70: 5f66 696c 6528 293a 0a20 2020 2020 2020  _file():.       
-0000bf80: 2020 2020 2020 2020 206c 6f67 6765 722e           logger.
-0000bf90: 6465 6275 6728 2256 6f69 6369 6e67 3a20  debug("Voicing: 
-0000bfa0: 2573 222c 2066 696c 656e 616d 6529 0a20  %s", filename). 
-0000bfb0: 2020 2020 2020 2020 2020 2020 2020 2064                 d
-0000bfc0: 6174 612c 205f 6673 203d 2073 662e 7265  ata, _fs = sf.re
-0000bfd0: 6164 2866 696c 656e 616d 652c 2064 7479  ad(filename, dty
-0000bfe0: 7065 3d22 666c 6f61 7433 3222 290a 2020  pe="float32").  
-0000bff0: 2020 2020 2020 2020 2020 2020 2020 7365                se
-0000c000: 6c66 2e70 7474 5f6f 6e28 290a 2020 2020  lf.ptt_on().    
-0000c010: 2020 2020 2020 2020 2020 2020 7472 793a              try:
-0000c020: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-0000c030: 2020 2020 2073 642e 6465 6661 756c 742e       sd.default.
-0000c040: 6465 7669 6365 203d 2073 656c 662e 7072  device = self.pr
-0000c050: 6566 2e67 6574 2822 736f 756e 6464 6576  ef.get("sounddev
-0000c060: 6963 6522 2c20 2264 6566 6175 6c74 2229  ice", "default")
-0000c070: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-0000c080: 2020 2020 2073 642e 6465 6661 756c 742e       sd.default.
-0000c090: 7361 6d70 6c65 7261 7465 203d 2034 3431  samplerate = 441
-0000c0a0: 3030 2e30 0a20 2020 2020 2020 2020 2020  00.0.           
-0000c0b0: 2020 2020 2020 2020 2073 642e 706c 6179           sd.play
-0000c0c0: 2864 6174 6129 0a20 2020 2020 2020 2020  (data).         
-0000c0d0: 2020 2020 2020 2020 2020 205f 7374 6174             _stat
-0000c0e0: 7573 203d 2073 642e 7761 6974 2829 0a20  us = sd.wait(). 
+00008270: 2020 206e 6578 745f 7461 622e 656e 6428     next_tab.end(
+00008280: 4661 6c73 6529 0a20 2020 2020 2020 2020  False).         
+00008290: 2020 2020 2020 2072 6574 7572 6e0a 2020         return.  
+000082a0: 2020 2020 2020 6966 2065 7665 6e74 2e6b        if event.k
+000082b0: 6579 2829 203d 3d20 5174 2e4b 6579 5f46  ey() == Qt.Key_F
+000082c0: 313a 0a20 2020 2020 2020 2020 2020 2073  1:.            s
+000082d0: 656c 662e 7365 6e64 6631 2829 0a20 2020  elf.sendf1().   
+000082e0: 2020 2020 2069 6620 6576 656e 742e 6b65       if event.ke
+000082f0: 7928 2920 3d3d 2051 742e 4b65 795f 4632  y() == Qt.Key_F2
+00008300: 3a0a 2020 2020 2020 2020 2020 2020 7365  :.            se
+00008310: 6c66 2e73 656e 6466 3228 290a 2020 2020  lf.sendf2().    
+00008320: 2020 2020 6966 2065 7665 6e74 2e6b 6579      if event.key
+00008330: 2829 203d 3d20 5174 2e4b 6579 5f46 333a  () == Qt.Key_F3:
+00008340: 0a20 2020 2020 2020 2020 2020 2073 656c  .            sel
+00008350: 662e 7365 6e64 6633 2829 0a20 2020 2020  f.sendf3().     
+00008360: 2020 2069 6620 6576 656e 742e 6b65 7928     if event.key(
+00008370: 2920 3d3d 2051 742e 4b65 795f 4634 3a0a  ) == Qt.Key_F4:.
+00008380: 2020 2020 2020 2020 2020 2020 7365 6c66              self
+00008390: 2e73 656e 6466 3428 290a 2020 2020 2020  .sendf4().      
+000083a0: 2020 6966 2065 7665 6e74 2e6b 6579 2829    if event.key()
+000083b0: 203d 3d20 5174 2e4b 6579 5f46 353a 0a20   == Qt.Key_F5:. 
+000083c0: 2020 2020 2020 2020 2020 2073 656c 662e             self.
+000083d0: 7365 6e64 6635 2829 0a20 2020 2020 2020  sendf5().       
+000083e0: 2069 6620 6576 656e 742e 6b65 7928 2920   if event.key() 
+000083f0: 3d3d 2051 742e 4b65 795f 4636 3a0a 2020  == Qt.Key_F6:.  
+00008400: 2020 2020 2020 2020 2020 7365 6c66 2e73            self.s
+00008410: 656e 6466 3628 290a 2020 2020 2020 2020  endf6().        
+00008420: 6966 2065 7665 6e74 2e6b 6579 2829 203d  if event.key() =
+00008430: 3d20 5174 2e4b 6579 5f46 373a 0a20 2020  = Qt.Key_F7:.   
+00008440: 2020 2020 2020 2020 2073 656c 662e 7365           self.se
+00008450: 6e64 6637 2829 0a20 2020 2020 2020 2069  ndf7().        i
+00008460: 6620 6576 656e 742e 6b65 7928 2920 3d3d  f event.key() ==
+00008470: 2051 742e 4b65 795f 4638 3a0a 2020 2020   Qt.Key_F8:.    
+00008480: 2020 2020 2020 2020 7365 6c66 2e73 656e          self.sen
+00008490: 6466 3828 290a 2020 2020 2020 2020 6966  df8().        if
+000084a0: 2065 7665 6e74 2e6b 6579 2829 203d 3d20   event.key() == 
+000084b0: 5174 2e4b 6579 5f46 393a 0a20 2020 2020  Qt.Key_F9:.     
+000084c0: 2020 2020 2020 2073 656c 662e 7365 6e64         self.send
+000084d0: 6639 2829 0a20 2020 2020 2020 2069 6620  f9().        if 
+000084e0: 6576 656e 742e 6b65 7928 2920 3d3d 2051  event.key() == Q
+000084f0: 742e 4b65 795f 4631 303a 0a20 2020 2020  t.Key_F10:.     
+00008500: 2020 2020 2020 2073 656c 662e 7365 6e64         self.send
+00008510: 6631 3028 290a 2020 2020 2020 2020 6966  f10().        if
+00008520: 2065 7665 6e74 2e6b 6579 2829 203d 3d20   event.key() == 
+00008530: 5174 2e4b 6579 5f46 3131 3a0a 2020 2020  Qt.Key_F11:.    
+00008540: 2020 2020 2020 2020 7365 6c66 2e73 656e          self.sen
+00008550: 6466 3131 2829 0a20 2020 2020 2020 2069  df11().        i
+00008560: 6620 6576 656e 742e 6b65 7928 2920 3d3d  f event.key() ==
+00008570: 2051 742e 4b65 795f 4631 323a 0a20 2020   Qt.Key_F12:.   
+00008580: 2020 2020 2020 2020 2073 656c 662e 7365           self.se
+00008590: 6e64 6631 3228 290a 0a20 2020 2064 6566  ndf12()..    def
+000085a0: 2073 6574 5f77 696e 646f 775f 7469 746c   set_window_titl
+000085b0: 6528 7365 6c66 293a 0a20 2020 2020 2020  e(self):.       
+000085c0: 2022 2222 5365 7420 7769 6e64 6f77 2074   """Set window t
+000085d0: 6974 6c65 2222 220a 2020 2020 2020 2020  itle""".        
+000085e0: 7666 6f61 203d 2073 656c 662e 7261 6469  vfoa = self.radi
+000085f0: 6f5f 7374 6174 652e 6765 7428 2276 666f  o_state.get("vfo
+00008600: 6122 2c20 2222 290a 2020 2020 2020 2020  a", "").        
+00008610: 6966 2076 666f 613a 0a20 2020 2020 2020  if vfoa:.       
+00008620: 2020 2020 2076 666f 6120 3d20 696e 7428       vfoa = int(
+00008630: 7666 6f61 2920 2f20 3130 3030 0a20 2020  vfoa) / 1000.   
+00008640: 2020 2020 2065 6c73 653a 0a20 2020 2020       else:.     
+00008650: 2020 2020 2020 2076 666f 6120 3d20 302e         vfoa = 0.
+00008660: 300a 2020 2020 2020 2020 636f 6e74 6573  0.        contes
+00008670: 745f 6e61 6d65 203d 2022 220a 2020 2020  t_name = "".    
+00008680: 2020 2020 6966 2073 656c 662e 636f 6e74      if self.cont
+00008690: 6573 743a 0a20 2020 2020 2020 2020 2020  est:.           
+000086a0: 2063 6f6e 7465 7374 5f6e 616d 6520 3d20   contest_name = 
+000086b0: 7365 6c66 2e63 6f6e 7465 7374 2e6e 616d  self.contest.nam
+000086c0: 650a 2020 2020 2020 2020 6c69 6e65 203d  e.        line =
+000086d0: 2028 0a20 2020 2020 2020 2020 2020 2066   (.            f
+000086e0: 2276 666f 613a 7b72 6f75 6e64 2876 666f  "vfoa:{round(vfo
+000086f0: 612c 3229 7d20 220a 2020 2020 2020 2020  a,2)} ".        
+00008700: 2020 2020 6622 6d6f 6465 3a7b 7365 6c66      f"mode:{self
+00008710: 2e72 6164 696f 5f73 7461 7465 2e67 6574  .radio_state.get
+00008720: 2827 6d6f 6465 272c 2027 2729 7d20 220a  ('mode', '')} ".
+00008730: 2020 2020 2020 2020 2020 2020 6622 4f50              f"OP
+00008740: 3a7b 7365 6c66 2e63 7572 7265 6e74 5f6f  :{self.current_o
+00008750: 707d 207b 636f 6e74 6573 745f 6e61 6d65  p} {contest_name
+00008760: 7d20 220a 2020 2020 2020 2020 2020 2020  } ".            
+00008770: 6622 2d20 4e6f 7431 4d4d 2076 7b5f 5f76  f"- Not1MM v{__v
+00008780: 6572 7369 6f6e 5f5f 7d22 0a20 2020 2020  ersion__}".     
+00008790: 2020 2029 0a20 2020 2020 2020 206c 6f67     ).        log
+000087a0: 6765 722e 6465 6275 6728 2225 7322 2c20  ger.debug("%s", 
+000087b0: 6c69 6e65 290a 2020 2020 2020 2020 7365  line).        se
+000087c0: 6c66 2e73 6574 5769 6e64 6f77 5469 746c  lf.setWindowTitl
+000087d0: 6528 6c69 6e65 290a 0a20 2020 2064 6566  e(line)..    def
+000087e0: 2063 6c65 6172 696e 7075 7473 2873 656c   clearinputs(sel
+000087f0: 6629 3a0a 2020 2020 2020 2020 2222 2243  f):.        """C
+00008800: 6c65 6172 7320 7468 6520 7465 7874 2069  lears the text i
+00008810: 6e70 7574 2066 6965 6c64 7320 616e 6420  nput fields and 
+00008820: 7365 7473 2066 6f63 7573 2074 6f20 6361  sets focus to ca
+00008830: 6c6c 7369 676e 2066 6965 6c64 2e22 2222  llsign field."""
+00008840: 0a20 2020 2020 2020 2073 656c 662e 6475  .        self.du
+00008850: 7065 5f69 6e64 6963 6174 6f72 2e68 6964  pe_indicator.hid
+00008860: 6528 290a 2020 2020 2020 2020 7365 6c66  e().        self
+00008870: 2e63 6f6e 7461 6374 203d 2073 656c 662e  .contact = self.
+00008880: 6461 7461 6261 7365 2e65 6d70 7479 5f63  database.empty_c
+00008890: 6f6e 7461 6374 0a20 2020 2020 2020 2073  ontact.        s
+000088a0: 656c 662e 6865 6164 696e 675f 6469 7374  elf.heading_dist
+000088b0: 616e 6365 2e73 6574 5465 7874 2822 2229  ance.setText("")
+000088c0: 0a20 2020 2020 2020 2073 656c 662e 6478  .        self.dx
+000088d0: 5f65 6e74 6974 792e 7365 7454 6578 7428  _entity.setText(
+000088e0: 2222 290a 2020 2020 2020 2020 6966 2073  "").        if s
+000088f0: 656c 662e 636f 6e74 6573 743a 0a20 2020  elf.contest:.   
+00008900: 2020 2020 2020 2020 206d 756c 7473 203d           mults =
+00008910: 2073 656c 662e 636f 6e74 6573 742e 7368   self.contest.sh
+00008920: 6f77 5f6d 756c 7473 2873 656c 6629 0a20  ow_mults(self). 
+00008930: 2020 2020 2020 2020 2020 2071 736f 7320             qsos 
+00008940: 3d20 7365 6c66 2e63 6f6e 7465 7374 2e73  = self.contest.s
+00008950: 686f 775f 7173 6f28 7365 6c66 290a 2020  how_qso(self).  
+00008960: 2020 2020 2020 2020 2020 6d75 6c74 7374            multst
+00008970: 7269 6e67 203d 2066 227b 7173 6f73 7d2f  ring = f"{qsos}/
+00008980: 7b6d 756c 7473 7d22 0a20 2020 2020 2020  {mults}".       
+00008990: 2020 2020 2073 656c 662e 6d75 6c74 732e       self.mults.
+000089a0: 7365 7454 6578 7428 6d75 6c74 7374 7269  setText(multstri
+000089b0: 6e67 290a 2020 2020 2020 2020 2020 2020  ng).            
+000089c0: 7363 6f72 6520 3d20 7365 6c66 2e63 6f6e  score = self.con
+000089d0: 7465 7374 2e63 616c 635f 7363 6f72 6528  test.calc_score(
+000089e0: 7365 6c66 290a 2020 2020 2020 2020 2020  self).          
+000089f0: 2020 7365 6c66 2e73 636f 7265 2e73 6574    self.score.set
+00008a00: 5465 7874 2873 7472 2873 636f 7265 2929  Text(str(score))
+00008a10: 0a20 2020 2020 2020 2020 2020 2073 656c  .            sel
+00008a20: 662e 636f 6e74 6573 742e 7265 7365 745f  f.contest.reset_
+00008a30: 6c61 6265 6c28 7365 6c66 290a 2020 2020  label(self).    
+00008a40: 2020 2020 7365 6c66 2e63 616c 6c73 6967      self.callsig
+00008a50: 6e2e 636c 6561 7228 290a 2020 2020 2020  n.clear().      
+00008a60: 2020 6966 2073 656c 662e 6375 7272 656e    if self.curren
+00008a70: 745f 6d6f 6465 203d 3d20 2243 5722 3a0a  t_mode == "CW":.
+00008a80: 2020 2020 2020 2020 2020 2020 7365 6c66              self
+00008a90: 2e73 656e 742e 7365 7454 6578 7428 2235  .sent.setText("5
+00008aa0: 3939 2229 0a20 2020 2020 2020 2020 2020  99").           
+00008ab0: 2073 656c 662e 7265 6365 6976 652e 7365   self.receive.se
+00008ac0: 7454 6578 7428 2235 3939 2229 0a20 2020  tText("599").   
+00008ad0: 2020 2020 2065 6c73 653a 0a20 2020 2020       else:.     
+00008ae0: 2020 2020 2020 2073 656c 662e 7365 6e74         self.sent
+00008af0: 2e73 6574 5465 7874 2822 3539 2229 0a20  .setText("59"). 
+00008b00: 2020 2020 2020 2020 2020 2073 656c 662e             self.
+00008b10: 7265 6365 6976 652e 7365 7454 6578 7428  receive.setText(
+00008b20: 2235 3922 290a 2020 2020 2020 2020 7365  "59").        se
+00008b30: 6c66 2e6f 7468 6572 5f31 2e63 6c65 6172  lf.other_1.clear
+00008b40: 2829 0a20 2020 2020 2020 2073 656c 662e  ().        self.
+00008b50: 6f74 6865 725f 322e 636c 6561 7228 290a  other_2.clear().
+00008b60: 2020 2020 2020 2020 7365 6c66 2e63 616c          self.cal
+00008b70: 6c73 6967 6e2e 7365 7446 6f63 7573 2829  lsign.setFocus()
+00008b80: 0a20 2020 2020 2020 2063 6d64 203d 207b  .        cmd = {
+00008b90: 7d0a 2020 2020 2020 2020 636d 645b 2263  }.        cmd["c
+00008ba0: 6d64 225d 203d 2022 4341 4c4c 4348 414e  md"] = "CALLCHAN
+00008bb0: 4745 4422 0a20 2020 2020 2020 2063 6d64  GED".        cmd
+00008bc0: 5b22 7374 6174 696f 6e22 5d20 3d20 706c  ["station"] = pl
+00008bd0: 6174 666f 726d 2e6e 6f64 6528 290a 2020  atform.node().  
+00008be0: 2020 2020 2020 636d 645b 2263 616c 6c22        cmd["call"
+00008bf0: 5d20 3d20 2222 0a20 2020 2020 2020 2073  ] = "".        s
+00008c00: 656c 662e 6d75 6c74 6963 6173 745f 696e  elf.multicast_in
+00008c10: 7465 7266 6163 652e 7365 6e64 5f61 735f  terface.send_as_
+00008c20: 6a73 6f6e 2863 6d64 290a 0a20 2020 2064  json(cmd)..    d
+00008c30: 6566 2073 6176 655f 636f 6e74 6163 7428  ef save_contact(
+00008c40: 7365 6c66 293a 0a20 2020 2020 2020 2022  self):.        "
+00008c50: 2222 5361 7665 2074 6f20 6462 2222 220a  ""Save to db""".
+00008c60: 2020 2020 2020 2020 6c6f 6767 6572 2e64          logger.d
+00008c70: 6562 7567 2822 7361 7669 6e67 2063 6f6e  ebug("saving con
+00008c80: 7461 6374 2229 0a20 2020 2020 2020 2069  tact").        i
+00008c90: 6620 6c65 6e28 7365 6c66 2e63 616c 6c73  f len(self.calls
+00008ca0: 6967 6e2e 7465 7874 2829 2920 3c20 333a  ign.text()) < 3:
+00008cb0: 0a20 2020 2020 2020 2020 2020 2072 6574  .            ret
+00008cc0: 7572 6e0a 2020 2020 2020 2020 6966 206e  urn.        if n
+00008cd0: 6f74 2061 6e79 2863 6861 722e 6973 6469  ot any(char.isdi
+00008ce0: 6769 7428 2920 666f 7220 6368 6172 2069  git() for char i
+00008cf0: 6e20 7365 6c66 2e63 616c 6c73 6967 6e2e  n self.callsign.
+00008d00: 7465 7874 2829 293a 0a20 2020 2020 2020  text()):.       
+00008d10: 2020 2020 2072 6574 7572 6e0a 2020 2020       return.    
+00008d20: 2020 2020 6966 206e 6f74 2061 6e79 2863      if not any(c
+00008d30: 6861 722e 6973 616c 7068 6128 2920 666f  har.isalpha() fo
+00008d40: 7220 6368 6172 2069 6e20 7365 6c66 2e63  r char in self.c
+00008d50: 616c 6c73 6967 6e2e 7465 7874 2829 293a  allsign.text()):
+00008d60: 0a20 2020 2020 2020 2020 2020 2072 6574  .            ret
+00008d70: 7572 6e0a 0a20 2020 2020 2020 2073 656c  urn..        sel
+00008d80: 662e 636f 6e74 6163 745b 2254 5322 5d20  f.contact["TS"] 
+00008d90: 3d20 6461 7465 7469 6d65 2e75 7463 6e6f  = datetime.utcno
+00008da0: 7728 292e 6973 6f66 6f72 6d61 7428 2220  w().isoformat(" 
+00008db0: 2229 5b3a 3139 5d0a 2020 2020 2020 2020  ")[:19].        
+00008dc0: 7365 6c66 2e63 6f6e 7461 6374 5b22 4361  self.contact["Ca
+00008dd0: 6c6c 225d 203d 2073 656c 662e 6361 6c6c  ll"] = self.call
+00008de0: 7369 676e 2e74 6578 7428 290a 2020 2020  sign.text().    
+00008df0: 2020 2020 7365 6c66 2e63 6f6e 7461 6374      self.contact
+00008e00: 5b22 4672 6571 225d 203d 2072 6f75 6e64  ["Freq"] = round
+00008e10: 2866 6c6f 6174 2873 656c 662e 7261 6469  (float(self.radi
+00008e20: 6f5f 7374 6174 652e 6765 7428 2276 666f  o_state.get("vfo
+00008e30: 6122 2c20 302e 3029 2920 2f20 3130 3030  a", 0.0)) / 1000
+00008e40: 2c20 3229 0a20 2020 2020 2020 2073 656c  , 2).        sel
+00008e50: 662e 636f 6e74 6163 745b 2251 5358 4672  f.contact["QSXFr
+00008e60: 6571 225d 203d 2072 6f75 6e64 280a 2020  eq"] = round(.  
+00008e70: 2020 2020 2020 2020 2020 666c 6f61 7428            float(
+00008e80: 7365 6c66 2e72 6164 696f 5f73 7461 7465  self.radio_state
+00008e90: 2e67 6574 2822 7666 6f61 222c 2030 2e30  .get("vfoa", 0.0
+00008ea0: 2929 202f 2031 3030 302c 2032 0a20 2020  )) / 1000, 2.   
+00008eb0: 2020 2020 2029 0a20 2020 2020 2020 2073       ).        s
+00008ec0: 656c 662e 636f 6e74 6163 745b 224d 6f64  elf.contact["Mod
+00008ed0: 6522 5d20 3d20 7365 6c66 2e72 6164 696f  e"] = self.radio
+00008ee0: 5f73 7461 7465 2e67 6574 2822 6d6f 6465  _state.get("mode
+00008ef0: 222c 2022 2229 0a20 2020 2020 2020 2073  ", "").        s
+00008f00: 656c 662e 636f 6e74 6163 745b 2243 6f6e  elf.contact["Con
+00008f10: 7465 7374 4e61 6d65 225d 203d 2073 656c  testName"] = sel
+00008f20: 662e 636f 6e74 6573 742e 6361 6272 696c  f.contest.cabril
+00008f30: 6c6f 5f6e 616d 650a 2020 2020 2020 2020  lo_name.        
+00008f40: 7365 6c66 2e63 6f6e 7461 6374 5b22 436f  self.contact["Co
+00008f50: 6e74 6573 744e 5222 5d20 3d20 7365 6c66  ntestNR"] = self
+00008f60: 2e70 7265 662e 6765 7428 2263 6f6e 7465  .pref.get("conte
+00008f70: 7374 222c 2022 3022 290a 2020 2020 2020  st", "0").      
+00008f80: 2020 7365 6c66 2e63 6f6e 7461 6374 5b22    self.contact["
+00008f90: 5374 6174 696f 6e50 7265 6669 7822 5d20  StationPrefix"] 
+00008fa0: 3d20 7365 6c66 2e73 7461 7469 6f6e 2e67  = self.station.g
+00008fb0: 6574 2822 4361 6c6c 222c 2022 2229 0a20  et("Call", ""). 
+00008fc0: 2020 2020 2020 2073 656c 662e 636f 6e74         self.cont
+00008fd0: 6163 745b 2257 5058 5072 6566 6978 225d  act["WPXPrefix"]
+00008fe0: 203d 2063 616c 6375 6c61 7465 5f77 7078   = calculate_wpx
+00008ff0: 5f70 7265 6669 7828 7365 6c66 2e63 616c  _prefix(self.cal
+00009000: 6c73 6967 6e2e 7465 7874 2829 290a 2020  lsign.text()).  
+00009010: 2020 2020 2020 7365 6c66 2e63 6f6e 7461        self.conta
+00009020: 6374 5b22 4973 5275 6e51 534f 225d 203d  ct["IsRunQSO"] =
+00009030: 2073 656c 662e 7261 6469 6f42 7574 746f   self.radioButto
+00009040: 6e5f 7275 6e2e 6973 4368 6563 6b65 6428  n_run.isChecked(
+00009050: 290a 2020 2020 2020 2020 7365 6c66 2e63  ).        self.c
+00009060: 6f6e 7461 6374 5b22 4f70 6572 6174 6f72  ontact["Operator
+00009070: 225d 203d 2073 656c 662e 6375 7272 656e  "] = self.curren
+00009080: 745f 6f70 0a20 2020 2020 2020 2073 656c  t_op.        sel
+00009090: 662e 636f 6e74 6163 745b 224e 6574 4269  f.contact["NetBi
+000090a0: 6f73 4e61 6d65 225d 203d 2073 6f63 6b65  osName"] = socke
+000090b0: 742e 6765 7468 6f73 746e 616d 6528 290a  t.gethostname().
+000090c0: 2020 2020 2020 2020 7365 6c66 2e63 6f6e          self.con
+000090d0: 7461 6374 5b22 4973 4f72 6967 696e 616c  tact["IsOriginal
+000090e0: 225d 203d 2031 0a20 2020 2020 2020 2073  "] = 1.        s
+000090f0: 656c 662e 636f 6e74 6163 745b 2249 4422  elf.contact["ID"
+00009100: 5d20 3d20 7575 6964 2e75 7569 6434 2829  ] = uuid.uuid4()
+00009110: 2e68 6578 0a20 2020 2020 2020 2073 656c  .hex.        sel
+00009120: 662e 636f 6e74 6573 742e 7365 745f 636f  f.contest.set_co
+00009130: 6e74 6163 745f 7661 7273 2873 656c 6629  ntact_vars(self)
+00009140: 0a20 2020 2020 2020 2073 656c 662e 636f  .        self.co
+00009150: 6e74 6163 745b 2250 6f69 6e74 7322 5d20  ntact["Points"] 
+00009160: 3d20 7365 6c66 2e63 6f6e 7465 7374 2e70  = self.contest.p
+00009170: 6f69 6e74 7328 7365 6c66 290a 2020 2020  oints(self).    
+00009180: 2020 2020 6465 6275 675f 6f75 7470 7574      debug_output
+00009190: 203d 2066 227b 7365 6c66 2e63 6f6e 7461   = f"{self.conta
+000091a0: 6374 7d22 0a20 2020 2020 2020 206c 6f67  ct}".        log
+000091b0: 6765 722e 6465 6275 6728 6465 6275 675f  ger.debug(debug_
+000091c0: 6f75 7470 7574 290a 2020 2020 2020 2020  output).        
+000091d0: 7365 6c66 2e64 6174 6162 6173 652e 6c6f  self.database.lo
+000091e0: 675f 636f 6e74 6163 7428 7365 6c66 2e63  g_contact(self.c
+000091f0: 6f6e 7461 6374 290a 2020 2020 2020 2020  ontact).        
+00009200: 7365 6c66 2e6e 316d 6d2e 7365 6e64 5f63  self.n1mm.send_c
+00009210: 6f6e 7461 6374 5f69 6e66 6f28 290a 2020  ontact_info().  
+00009220: 2020 2020 2020 7365 6c66 2e63 6c65 6172        self.clear
+00009230: 696e 7075 7473 2829 0a20 2020 2020 2020  inputs().       
+00009240: 2063 6d64 203d 207b 7d0a 2020 2020 2020   cmd = {}.      
+00009250: 2020 636d 645b 2263 6d64 225d 203d 2022    cmd["cmd"] = "
+00009260: 5550 4441 5445 4c4f 4722 0a20 2020 2020  UPDATELOG".     
+00009270: 2020 2063 6d64 5b22 7374 6174 696f 6e22     cmd["station"
+00009280: 5d20 3d20 706c 6174 666f 726d 2e6e 6f64  ] = platform.nod
+00009290: 6528 290a 2020 2020 2020 2020 7365 6c66  e().        self
+000092a0: 2e6d 756c 7469 6361 7374 5f69 6e74 6572  .multicast_inter
+000092b0: 6661 6365 2e73 656e 645f 6173 5f6a 736f  face.send_as_jso
+000092c0: 6e28 636d 6429 0a20 2020 2020 2020 2023  n(cmd).        #
+000092d0: 2073 656c 662e 636f 6e74 6163 745b 2243   self.contact["C
+000092e0: 6f6e 7465 7374 4e61 6d65 225d 203d 2073  ontestName"] = s
+000092f0: 656c 662e 636f 6e74 6573 742e 6e61 6d65  elf.contest.name
+00009300: 0a20 2020 2020 2020 2023 2073 656c 662e  .        # self.
+00009310: 636f 6e74 6163 745b 2253 4e54 225d 203d  contact["SNT"] =
+00009320: 2073 656c 662e 7365 6e74 2e74 6578 7428   self.sent.text(
+00009330: 290a 2020 2020 2020 2020 2320 7365 6c66  ).        # self
+00009340: 2e63 6f6e 7461 6374 5b22 5243 5622 5d20  .contact["RCV"] 
+00009350: 3d20 7365 6c66 2e72 6563 6569 7665 2e74  = self.receive.t
+00009360: 6578 7428 290a 2020 2020 2020 2020 2320  ext().        # 
+00009370: 7365 6c66 2e63 6f6e 7461 6374 5b22 436f  self.contact["Co
+00009380: 756e 7472 7950 7265 6669 7822 5d0a 2020  untryPrefix"].  
+00009390: 2020 2020 2020 2320 7365 6c66 2e63 6f6e        # self.con
+000093a0: 7461 6374 5b22 5374 6174 696f 6e50 7265  tact["StationPre
+000093b0: 6669 7822 5d20 3d20 7365 6c66 2e70 7265  fix"] = self.pre
+000093c0: 662e 6765 7428 2263 616c 6c73 6967 6e22  f.get("callsign"
+000093d0: 2c20 2222 290a 2020 2020 2020 2020 2320  , "").        # 
+000093e0: 7365 6c66 2e63 6f6e 7461 6374 5b22 5154  self.contact["QT
+000093f0: 4822 5d0a 2020 2020 2020 2020 2320 7365  H"].        # se
+00009400: 6c66 2e63 6f6e 7461 6374 5b22 4e61 6d65  lf.contact["Name
+00009410: 225d 203d 2073 656c 662e 6f74 6865 725f  "] = self.other_
+00009420: 312e 7465 7874 2829 0a20 2020 2020 2020  1.text().       
+00009430: 2023 2073 656c 662e 636f 6e74 6163 745b   # self.contact[
+00009440: 2243 6f6d 6d65 6e74 225d 203d 2073 656c  "Comment"] = sel
+00009450: 662e 6f74 6865 725f 322e 7465 7874 2829  f.other_2.text()
+00009460: 0a20 2020 2020 2020 2023 2073 656c 662e  .        # self.
+00009470: 636f 6e74 6163 745b 224e 5222 5d0a 2020  contact["NR"].  
+00009480: 2020 2020 2020 2320 7365 6c66 2e63 6f6e        # self.con
+00009490: 7461 6374 5b22 5365 6374 225d 0a20 2020  tact["Sect"].   
+000094a0: 2020 2020 2023 2073 656c 662e 636f 6e74       # self.cont
+000094b0: 6163 745b 2250 7265 6322 5d0a 2020 2020  act["Prec"].    
+000094c0: 2020 2020 2320 7365 6c66 2e63 6f6e 7461      # self.conta
+000094d0: 6374 5b22 434b 225d 0a20 2020 2020 2020  ct["CK"].       
+000094e0: 2023 2073 656c 662e 636f 6e74 6163 745b   # self.contact[
+000094f0: 225a 4e22 5d0a 2020 2020 2020 2020 2320  "ZN"].        # 
+00009500: 7365 6c66 2e63 6f6e 7461 6374 5b22 5365  self.contact["Se
+00009510: 6e74 4e72 225d 0a20 2020 2020 2020 2023  ntNr"].        #
+00009520: 2073 656c 662e 636f 6e74 6163 745b 2250   self.contact["P
+00009530: 6f69 6e74 7322 5d0a 2020 2020 2020 2020  oints"].        
+00009540: 2320 7365 6c66 2e63 6f6e 7461 6374 5b22  # self.contact["
+00009550: 4973 4d75 6c74 6970 6c69 6572 3122 5d0a  IsMultiplier1"].
+00009560: 2020 2020 2020 2020 2320 7365 6c66 2e63          # self.c
+00009570: 6f6e 7461 6374 5b22 4973 4d75 6c74 6970  ontact["IsMultip
+00009580: 6c69 6572 3222 5d0a 2020 2020 2020 2020  lier2"].        
+00009590: 2320 7365 6c66 2e63 6f6e 7461 6374 5b22  # self.contact["
+000095a0: 506f 7765 7222 5d0a 2020 2020 2020 2020  Power"].        
+000095b0: 2320 7365 6c66 2e63 6f6e 7461 6374 5b22  # self.contact["
+000095c0: 4261 6e64 225d 0a20 2020 2020 2020 2023  Band"].        #
+000095d0: 2073 656c 662e 636f 6e74 6163 745b 2257   self.contact["W
+000095e0: 5058 5072 6566 6978 225d 203d 2063 616c  PXPrefix"] = cal
+000095f0: 6375 6c61 7465 5f77 7078 5f70 7265 6669  culate_wpx_prefi
+00009600: 7828 7365 6c66 2e63 616c 6c73 6967 6e2e  x(self.callsign.
+00009610: 7465 7874 2829 290a 2020 2020 2020 2020  text()).        
+00009620: 2320 7365 6c66 2e63 6f6e 7461 6374 5b22  # self.contact["
+00009630: 4578 6368 616e 6765 3122 5d0a 2020 2020  Exchange1"].    
+00009640: 2020 2020 2320 7365 6c66 2e63 6f6e 7461      # self.conta
+00009650: 6374 5b22 5261 6469 6f4e 5222 5d0a 2020  ct["RadioNR"].  
+00009660: 2020 2020 2020 2320 7365 6c66 2e63 6f6e        # self.con
+00009670: 7461 6374 5b22 6973 4d75 6c74 6970 6c69  tact["isMultipli
+00009680: 6572 3322 5d0a 2020 2020 2020 2020 2320  er3"].        # 
+00009690: 7365 6c66 2e63 6f6e 7461 6374 5b22 4d69  self.contact["Mi
+000096a0: 7363 5465 7874 225d 0a20 2020 2020 2020  scText"].       
+000096b0: 2023 2073 656c 662e 636f 6e74 6163 745b   # self.contact[
+000096c0: 2243 6f6e 7461 6374 5479 7065 225d 0a20  "ContactType"]. 
+000096d0: 2020 2020 2020 2023 2073 656c 662e 636f         # self.co
+000096e0: 6e74 6163 745b 2252 756e 3152 756e 3222  ntact["Run1Run2"
+000096f0: 5d0a 2020 2020 2020 2020 2320 7365 6c66  ].        # self
+00009700: 2e63 6f6e 7461 6374 5b22 4772 6964 5371  .contact["GridSq
+00009710: 7561 7265 225d 0a20 2020 2020 2020 2023  uare"].        #
+00009720: 2073 656c 662e 636f 6e74 6163 745b 2243   self.contact["C
+00009730: 6f6e 7469 6e65 6e74 225d 0a20 2020 2020  ontinent"].     
+00009740: 2020 2023 2073 656c 662e 636f 6e74 6163     # self.contac
+00009750: 745b 2252 6f76 6572 4c6f 6361 7469 6f6e  t["RoverLocation
+00009760: 225d 0a20 2020 2020 2020 2023 2073 656c  "].        # sel
+00009770: 662e 636f 6e74 6163 745b 2252 6164 696f  f.contact["Radio
+00009780: 496e 7465 7266 6163 6564 225d 0a20 2020  Interfaced"].   
+00009790: 2020 2020 2023 2073 656c 662e 636f 6e74       # self.cont
+000097a0: 6163 745b 224e 6574 776f 726b 6564 436f  act["NetworkedCo
+000097b0: 6d70 4e72 225d 0a20 2020 2020 2020 2023  mpNr"].        #
+000097c0: 2073 656c 662e 636f 6e74 6163 745b 2243   self.contact["C
+000097d0: 4c41 494d 4544 5153 4f22 5d0a 0a20 2020  LAIMEDQSO"]..   
+000097e0: 2064 6566 206e 6577 5f63 6f6e 7465 7374   def new_contest
+000097f0: 5f64 6961 6c6f 6728 7365 6c66 293a 0a20  _dialog(self):. 
+00009800: 2020 2020 2020 2022 2222 5368 6f77 206e         """Show n
+00009810: 6577 2063 6f6e 7465 7374 2064 6961 6c6f  ew contest dialo
+00009820: 6722 2222 0a20 2020 2020 2020 206c 6f67  g""".        log
+00009830: 6765 722e 6465 6275 6728 224e 6577 2063  ger.debug("New c
+00009840: 6f6e 7465 7374 2044 6961 6c6f 6722 290a  ontest Dialog").
+00009850: 2020 2020 2020 2020 7365 6c66 2e63 6f6e          self.con
+00009860: 7465 7374 5f64 6961 6c6f 6720 3d20 4e65  test_dialog = Ne
+00009870: 7743 6f6e 7465 7374 2857 4f52 4b49 4e47  wContest(WORKING
+00009880: 5f50 4154 4829 0a20 2020 2020 2020 2073  _PATH).        s
+00009890: 656c 662e 636f 6e74 6573 745f 6469 616c  elf.contest_dial
+000098a0: 6f67 2e61 6363 6570 7465 642e 636f 6e6e  og.accepted.conn
+000098b0: 6563 7428 7365 6c66 2e73 6176 655f 636f  ect(self.save_co
+000098c0: 6e74 6573 7429 0a20 2020 2020 2020 2069  ntest).        i
+000098d0: 6620 7365 6c66 2e70 7265 662e 6765 7428  f self.pref.get(
+000098e0: 2264 6172 6b5f 6d6f 6465 2229 3a0a 2020  "dark_mode"):.  
+000098f0: 2020 2020 2020 2020 2020 7365 6c66 2e63            self.c
+00009900: 6f6e 7465 7374 5f64 6961 6c6f 672e 7365  ontest_dialog.se
+00009910: 7453 7479 6c65 5368 6565 7428 4441 524b  tStyleSheet(DARK
+00009920: 5f53 5459 4c45 5348 4545 5429 0a20 2020  _STYLESHEET).   
+00009930: 2020 2020 2073 656c 662e 636f 6e74 6573       self.contes
+00009940: 745f 6469 616c 6f67 2e64 6174 6554 696d  t_dialog.dateTim
+00009950: 6545 6469 742e 7365 7444 6174 6528 5174  eEdit.setDate(Qt
+00009960: 436f 7265 2e51 4461 7465 2e63 7572 7265  Core.QDate.curre
+00009970: 6e74 4461 7465 2829 290a 2020 2020 2020  ntDate()).      
+00009980: 2020 7365 6c66 2e63 6f6e 7465 7374 5f64    self.contest_d
+00009990: 6961 6c6f 672e 6461 7465 5469 6d65 4564  ialog.dateTimeEd
+000099a0: 6974 2e73 6574 4361 6c65 6e64 6172 506f  it.setCalendarPo
+000099b0: 7075 7028 5472 7565 290a 2020 2020 2020  pup(True).      
+000099c0: 2020 7365 6c66 2e63 6f6e 7465 7374 5f64    self.contest_d
+000099d0: 6961 6c6f 672e 6461 7465 5469 6d65 4564  ialog.dateTimeEd
+000099e0: 6974 2e73 6574 5469 6d65 2851 7443 6f72  it.setTime(QtCor
+000099f0: 652e 5154 696d 6528 302c 2030 2929 0a20  e.QTime(0, 0)). 
+00009a00: 2020 2020 2020 2073 656c 662e 636f 6e74         self.cont
+00009a10: 6573 745f 6469 616c 6f67 2e70 6f77 6572  est_dialog.power
+00009a20: 2e73 6574 4375 7272 656e 7454 6578 7428  .setCurrentText(
+00009a30: 224c 4f57 2229 0a20 2020 2020 2020 2073  "LOW").        s
+00009a40: 656c 662e 636f 6e74 6573 745f 6469 616c  elf.contest_dial
+00009a50: 6f67 2e73 7461 7469 6f6e 2e73 6574 4375  og.station.setCu
+00009a60: 7272 656e 7454 6578 7428 2246 4958 4544  rrentText("FIXED
+00009a70: 2229 0a20 2020 2020 2020 2073 656c 662e  ").        self.
+00009a80: 636f 6e74 6573 745f 6469 616c 6f67 2e6f  contest_dialog.o
+00009a90: 7065 6e28 290a 0a20 2020 2064 6566 2073  pen()..    def s
+00009aa0: 6176 655f 636f 6e74 6573 7428 7365 6c66  ave_contest(self
+00009ab0: 293a 0a20 2020 2020 2020 2022 2222 5361  ):.        """Sa
+00009ac0: 7665 2043 6f6e 7465 7374 2222 220a 2020  ve Contest""".  
+00009ad0: 2020 2020 2020 6e65 7874 5f6e 756d 6265        next_numbe
+00009ae0: 7220 3d20 7365 6c66 2e64 6174 6162 6173  r = self.databas
+00009af0: 652e 6765 745f 6e65 7874 5f63 6f6e 7465  e.get_next_conte
+00009b00: 7374 5f6e 7228 290a 2020 2020 2020 2020  st_nr().        
+00009b10: 636f 6e74 6573 7420 3d20 7b7d 0a20 2020  contest = {}.   
+00009b20: 2020 2020 2063 6f6e 7465 7374 5b22 436f       contest["Co
+00009b30: 6e74 6573 744e 616d 6522 5d20 3d20 280a  ntestName"] = (.
+00009b40: 2020 2020 2020 2020 2020 2020 7365 6c66              self
+00009b50: 2e63 6f6e 7465 7374 5f64 6961 6c6f 672e  .contest_dialog.
+00009b60: 636f 6e74 6573 742e 6375 7272 656e 7454  contest.currentT
+00009b70: 6578 7428 292e 6c6f 7765 7228 292e 7265  ext().lower().re
+00009b80: 706c 6163 6528 2220 222c 2022 5f22 290a  place(" ", "_").
+00009b90: 2020 2020 2020 2020 290a 2020 2020 2020          ).      
+00009ba0: 2020 636f 6e74 6573 745b 2253 7461 7274    contest["Start
+00009bb0: 4461 7465 225d 203d 2073 656c 662e 636f  Date"] = self.co
+00009bc0: 6e74 6573 745f 6469 616c 6f67 2e64 6174  ntest_dialog.dat
+00009bd0: 6554 696d 6545 6469 742e 6461 7465 5469  eTimeEdit.dateTi
+00009be0: 6d65 2829 2e74 6f53 7472 696e 6728 0a20  me().toString(. 
+00009bf0: 2020 2020 2020 2020 2020 2022 7979 7979             "yyyy
+00009c00: 2d4d 4d2d 6464 2068 683a 6d6d 3a73 7322  -MM-dd hh:mm:ss"
+00009c10: 0a20 2020 2020 2020 2029 0a20 2020 2020  .        ).     
+00009c20: 2020 2063 6f6e 7465 7374 5b22 4f70 6572     contest["Oper
+00009c30: 6174 6f72 4361 7465 676f 7279 225d 203d  atorCategory"] =
+00009c40: 2073 656c 662e 636f 6e74 6573 745f 6469   self.contest_di
+00009c50: 616c 6f67 2e6f 7065 7261 746f 725f 636c  alog.operator_cl
+00009c60: 6173 732e 6375 7272 656e 7454 6578 7428  ass.currentText(
+00009c70: 290a 2020 2020 2020 2020 636f 6e74 6573  ).        contes
+00009c80: 745b 2242 616e 6443 6174 6567 6f72 7922  t["BandCategory"
+00009c90: 5d20 3d20 7365 6c66 2e63 6f6e 7465 7374  ] = self.contest
+00009ca0: 5f64 6961 6c6f 672e 6261 6e64 2e63 7572  _dialog.band.cur
+00009cb0: 7265 6e74 5465 7874 2829 0a20 2020 2020  rentText().     
+00009cc0: 2020 2063 6f6e 7465 7374 5b22 506f 7765     contest["Powe
+00009cd0: 7243 6174 6567 6f72 7922 5d20 3d20 7365  rCategory"] = se
+00009ce0: 6c66 2e63 6f6e 7465 7374 5f64 6961 6c6f  lf.contest_dialo
+00009cf0: 672e 706f 7765 722e 6375 7272 656e 7454  g.power.currentT
+00009d00: 6578 7428 290a 2020 2020 2020 2020 636f  ext().        co
+00009d10: 6e74 6573 745b 224d 6f64 6543 6174 6567  ntest["ModeCateg
+00009d20: 6f72 7922 5d20 3d20 7365 6c66 2e63 6f6e  ory"] = self.con
+00009d30: 7465 7374 5f64 6961 6c6f 672e 6d6f 6465  test_dialog.mode
+00009d40: 2e63 7572 7265 6e74 5465 7874 2829 0a20  .currentText(). 
+00009d50: 2020 2020 2020 2063 6f6e 7465 7374 5b22         contest["
+00009d60: 4f76 6572 6c61 7943 6174 6567 6f72 7922  OverlayCategory"
+00009d70: 5d20 3d20 7365 6c66 2e63 6f6e 7465 7374  ] = self.contest
+00009d80: 5f64 6961 6c6f 672e 6f76 6572 6c61 792e  _dialog.overlay.
+00009d90: 6375 7272 656e 7454 6578 7428 290a 2020  currentText().  
+00009da0: 2020 2020 2020 2320 636f 6e74 6573 745b        # contest[
+00009db0: 2743 6c61 696d 6564 5363 6f72 6527 5d20  'ClaimedScore'] 
+00009dc0: 3d20 7365 6c66 2e63 6f6e 7465 7374 5f64  = self.contest_d
+00009dd0: 6961 6c6f 672e 0a20 2020 2020 2020 2063  ialog..        c
+00009de0: 6f6e 7465 7374 5b22 4f70 6572 6174 6f72  ontest["Operator
+00009df0: 7322 5d20 3d20 7365 6c66 2e63 6f6e 7465  s"] = self.conte
+00009e00: 7374 5f64 6961 6c6f 672e 6f70 6572 6174  st_dialog.operat
+00009e10: 6f72 732e 7465 7874 2829 0a20 2020 2020  ors.text().     
+00009e20: 2020 2063 6f6e 7465 7374 5b22 536f 6170     contest["Soap
+00009e30: 626f 7822 5d20 3d20 7365 6c66 2e63 6f6e  box"] = self.con
+00009e40: 7465 7374 5f64 6961 6c6f 672e 736f 6170  test_dialog.soap
+00009e50: 626f 782e 746f 506c 6169 6e54 6578 7428  box.toPlainText(
+00009e60: 290a 2020 2020 2020 2020 636f 6e74 6573  ).        contes
+00009e70: 745b 2253 656e 7445 7863 6861 6e67 6522  t["SentExchange"
+00009e80: 5d20 3d20 7365 6c66 2e63 6f6e 7465 7374  ] = self.contest
+00009e90: 5f64 6961 6c6f 672e 6578 6368 616e 6765  _dialog.exchange
+00009ea0: 2e74 6578 7428 290a 2020 2020 2020 2020  .text().        
+00009eb0: 636f 6e74 6573 745b 2243 6f6e 7465 7374  contest["Contest
+00009ec0: 4e52 225d 203d 206e 6578 745f 6e75 6d62  NR"] = next_numb
+00009ed0: 6572 2e67 6574 2822 636f 756e 7422 2c20  er.get("count", 
+00009ee0: 3129 0a20 2020 2020 2020 2073 656c 662e  1).        self.
+00009ef0: 7072 6566 5b22 636f 6e74 6573 7422 5d20  pref["contest"] 
+00009f00: 3d20 6e65 7874 5f6e 756d 6265 722e 6765  = next_number.ge
+00009f10: 7428 2263 6f75 6e74 222c 2031 290a 2020  t("count", 1).  
+00009f20: 2020 2020 2020 2320 636f 6e74 6573 745b        # contest[
+00009f30: 2753 7562 5479 7065 275d 203d 2073 656c  'SubType'] = sel
+00009f40: 662e 636f 6e74 6573 745f 6469 616c 6f67  f.contest_dialog
+00009f50: 2e0a 2020 2020 2020 2020 636f 6e74 6573  ..        contes
+00009f60: 745b 2253 7461 7469 6f6e 4361 7465 676f  t["StationCatego
+00009f70: 7279 225d 203d 2073 656c 662e 636f 6e74  ry"] = self.cont
+00009f80: 6573 745f 6469 616c 6f67 2e73 7461 7469  est_dialog.stati
+00009f90: 6f6e 2e63 7572 7265 6e74 5465 7874 2829  on.currentText()
+00009fa0: 0a20 2020 2020 2020 2063 6f6e 7465 7374  .        contest
+00009fb0: 5b22 4173 7369 7374 6564 4361 7465 676f  ["AssistedCatego
+00009fc0: 7279 225d 203d 2073 656c 662e 636f 6e74  ry"] = self.cont
+00009fd0: 6573 745f 6469 616c 6f67 2e61 7373 6973  est_dialog.assis
+00009fe0: 7465 642e 6375 7272 656e 7454 6578 7428  ted.currentText(
+00009ff0: 290a 2020 2020 2020 2020 636f 6e74 6573  ).        contes
+0000a000: 745b 2254 7261 6e73 6d69 7474 6572 4361  t["TransmitterCa
+0000a010: 7465 676f 7279 225d 203d 2073 656c 662e  tegory"] = self.
+0000a020: 636f 6e74 6573 745f 6469 616c 6f67 2e74  contest_dialog.t
+0000a030: 7261 6e73 6d69 7474 6572 2e63 7572 7265  ransmitter.curre
+0000a040: 6e74 5465 7874 2829 0a20 2020 2020 2020  ntText().       
+0000a050: 2023 2063 6f6e 7465 7374 5b27 5469 6d65   # contest['Time
+0000a060: 4361 7465 676f 7279 275d 203d 2073 656c  Category'] = sel
+0000a070: 662e 636f 6e74 6573 745f 6469 616c 6f67  f.contest_dialog
+0000a080: 2e0a 2020 2020 2020 2020 6c6f 6767 6572  ..        logger
+0000a090: 2e64 6562 7567 2822 2573 222c 2066 227b  .debug("%s", f"{
+0000a0a0: 636f 6e74 6573 747d 2229 0a20 2020 2020  contest}").     
+0000a0b0: 2020 2073 656c 662e 6461 7461 6261 7365     self.database
+0000a0c0: 2e61 6464 5f63 6f6e 7465 7374 2863 6f6e  .add_contest(con
+0000a0d0: 7465 7374 290a 2020 2020 2020 2020 7365  test).        se
+0000a0e0: 6c66 2e77 7269 7465 5f70 7265 6665 7265  lf.write_prefere
+0000a0f0: 6e63 6528 290a 2020 2020 2020 2020 7365  nce().        se
+0000a100: 6c66 2e6c 6f61 645f 636f 6e74 6573 7428  lf.load_contest(
+0000a110: 290a 0a20 2020 2064 6566 2065 6469 745f  )..    def edit_
+0000a120: 7374 6174 696f 6e5f 7365 7474 696e 6773  station_settings
+0000a130: 2873 656c 6629 3a0a 2020 2020 2020 2020  (self):.        
+0000a140: 2222 2253 686f 7720 7365 7474 696e 6773  """Show settings
+0000a150: 2064 6961 6c6f 6722 2222 0a20 2020 2020   dialog""".     
+0000a160: 2020 206c 6f67 6765 722e 6465 6275 6728     logger.debug(
+0000a170: 2253 7461 7469 6f6e 2053 6574 7469 6e67  "Station Setting
+0000a180: 7320 7365 6c65 6374 6564 2229 0a20 2020  s selected").   
+0000a190: 2020 2020 2073 656c 662e 7365 7474 696e       self.settin
+0000a1a0: 6773 5f64 6961 6c6f 6720 3d20 4564 6974  gs_dialog = Edit
+0000a1b0: 5374 6174 696f 6e28 574f 524b 494e 475f  Station(WORKING_
+0000a1c0: 5041 5448 290a 2020 2020 2020 2020 6966  PATH).        if
+0000a1d0: 2073 656c 662e 7072 6566 2e67 6574 2822   self.pref.get("
+0000a1e0: 6461 726b 5f6d 6f64 6522 293a 0a20 2020  dark_mode"):.   
+0000a1f0: 2020 2020 2020 2020 2073 656c 662e 7365           self.se
+0000a200: 7474 696e 6773 5f64 6961 6c6f 672e 7365  ttings_dialog.se
+0000a210: 7453 7479 6c65 5368 6565 7428 4441 524b  tStyleSheet(DARK
+0000a220: 5f53 5459 4c45 5348 4545 5429 0a20 2020  _STYLESHEET).   
+0000a230: 2020 2020 2073 656c 662e 7365 7474 696e       self.settin
+0000a240: 6773 5f64 6961 6c6f 672e 6163 6365 7074  gs_dialog.accept
+0000a250: 6564 2e63 6f6e 6e65 6374 2873 656c 662e  ed.connect(self.
+0000a260: 7361 7665 5f73 6574 7469 6e67 7329 0a20  save_settings). 
+0000a270: 2020 2020 2020 2023 2069 6620 7365 6c66         # if self
+0000a280: 2e70 7265 662e 6765 7428 2264 6172 6b5f  .pref.get("dark_
+0000a290: 6d6f 6465 2229 3a0a 2020 2020 2020 2020  mode"):.        
+0000a2a0: 2320 2020 2020 7365 6c66 2e73 6574 7469  #     self.setti
+0000a2b0: 6e67 735f 6469 616c 6f67 2e73 6574 5374  ngs_dialog.setSt
+0000a2c0: 796c 6553 6865 6574 2844 4152 4b5f 5354  yleSheet(DARK_ST
+0000a2d0: 594c 4553 4845 4554 290a 0a20 2020 2020  YLESHEET)..     
+0000a2e0: 2020 2073 656c 662e 7365 7474 696e 6773     self.settings
+0000a2f0: 5f64 6961 6c6f 672e 4361 6c6c 2e73 6574  _dialog.Call.set
+0000a300: 5465 7874 2873 656c 662e 7374 6174 696f  Text(self.statio
+0000a310: 6e2e 6765 7428 2243 616c 6c22 2c20 2222  n.get("Call", ""
+0000a320: 2929 0a20 2020 2020 2020 2073 656c 662e  )).        self.
+0000a330: 7365 7474 696e 6773 5f64 6961 6c6f 672e  settings_dialog.
+0000a340: 4e61 6d65 2e73 6574 5465 7874 2873 656c  Name.setText(sel
+0000a350: 662e 7374 6174 696f 6e2e 6765 7428 224e  f.station.get("N
+0000a360: 616d 6522 2c20 2222 2929 0a20 2020 2020  ame", "")).     
+0000a370: 2020 2073 656c 662e 7365 7474 696e 6773     self.settings
+0000a380: 5f64 6961 6c6f 672e 4164 6472 6573 7331  _dialog.Address1
+0000a390: 2e73 6574 5465 7874 2873 656c 662e 7374  .setText(self.st
+0000a3a0: 6174 696f 6e2e 6765 7428 2253 7472 6565  ation.get("Stree
+0000a3b0: 7431 222c 2022 2229 290a 2020 2020 2020  t1", "")).      
+0000a3c0: 2020 7365 6c66 2e73 6574 7469 6e67 735f    self.settings_
+0000a3d0: 6469 616c 6f67 2e41 6464 7265 7373 322e  dialog.Address2.
+0000a3e0: 7365 7454 6578 7428 7365 6c66 2e73 7461  setText(self.sta
+0000a3f0: 7469 6f6e 2e67 6574 2822 5374 7265 6574  tion.get("Street
+0000a400: 3222 2c20 2222 2929 0a20 2020 2020 2020  2", "")).       
+0000a410: 2073 656c 662e 7365 7474 696e 6773 5f64   self.settings_d
+0000a420: 6961 6c6f 672e 4369 7479 2e73 6574 5465  ialog.City.setTe
+0000a430: 7874 2873 656c 662e 7374 6174 696f 6e2e  xt(self.station.
+0000a440: 6765 7428 2243 6974 7922 2c20 2222 2929  get("City", ""))
+0000a450: 0a20 2020 2020 2020 2073 656c 662e 7365  .        self.se
+0000a460: 7474 696e 6773 5f64 6961 6c6f 672e 5374  ttings_dialog.St
+0000a470: 6174 652e 7365 7454 6578 7428 7365 6c66  ate.setText(self
+0000a480: 2e73 7461 7469 6f6e 2e67 6574 2822 5374  .station.get("St
+0000a490: 6174 6522 2c20 2222 2929 0a20 2020 2020  ate", "")).     
+0000a4a0: 2020 2073 656c 662e 7365 7474 696e 6773     self.settings
+0000a4b0: 5f64 6961 6c6f 672e 5a69 702e 7365 7454  _dialog.Zip.setT
+0000a4c0: 6578 7428 7365 6c66 2e73 7461 7469 6f6e  ext(self.station
+0000a4d0: 2e67 6574 2822 5a69 7022 2c20 2222 2929  .get("Zip", ""))
+0000a4e0: 0a20 2020 2020 2020 2073 656c 662e 7365  .        self.se
+0000a4f0: 7474 696e 6773 5f64 6961 6c6f 672e 436f  ttings_dialog.Co
+0000a500: 756e 7472 792e 7365 7454 6578 7428 7365  untry.setText(se
+0000a510: 6c66 2e73 7461 7469 6f6e 2e67 6574 2822  lf.station.get("
+0000a520: 436f 756e 7472 7922 2c20 2222 2929 0a20  Country", "")). 
+0000a530: 2020 2020 2020 2073 656c 662e 7365 7474         self.sett
+0000a540: 696e 6773 5f64 6961 6c6f 672e 4772 6964  ings_dialog.Grid
+0000a550: 5371 7561 7265 2e73 6574 5465 7874 2873  Square.setText(s
+0000a560: 656c 662e 7374 6174 696f 6e2e 6765 7428  elf.station.get(
+0000a570: 2247 7269 6453 7175 6172 6522 2c20 2222  "GridSquare", ""
+0000a580: 2929 0a20 2020 2020 2020 2073 656c 662e  )).        self.
+0000a590: 7365 7474 696e 6773 5f64 6961 6c6f 672e  settings_dialog.
+0000a5a0: 4351 5a6f 6e65 2e73 6574 5465 7874 2873  CQZone.setText(s
+0000a5b0: 7472 2873 656c 662e 7374 6174 696f 6e2e  tr(self.station.
+0000a5c0: 6765 7428 2243 515a 6f6e 6522 2c20 2222  get("CQZone", ""
+0000a5d0: 2929 290a 2020 2020 2020 2020 7365 6c66  ))).        self
+0000a5e0: 2e73 6574 7469 6e67 735f 6469 616c 6f67  .settings_dialog
+0000a5f0: 2e49 5455 5a6f 6e65 2e73 6574 5465 7874  .ITUZone.setText
+0000a600: 2873 7472 2873 656c 662e 7374 6174 696f  (str(self.statio
+0000a610: 6e2e 6765 7428 2249 4152 555a 6f6e 6522  n.get("IARUZone"
+0000a620: 2c20 2222 2929 290a 2020 2020 2020 2020  , ""))).        
+0000a630: 7365 6c66 2e73 6574 7469 6e67 735f 6469  self.settings_di
+0000a640: 616c 6f67 2e4c 6963 656e 7365 2e73 6574  alog.License.set
+0000a650: 5465 7874 2873 656c 662e 7374 6174 696f  Text(self.statio
+0000a660: 6e2e 6765 7428 224c 6963 656e 7365 436c  n.get("LicenseCl
+0000a670: 6173 7322 2c20 2222 2929 0a20 2020 2020  ass", "")).     
+0000a680: 2020 2073 656c 662e 7365 7474 696e 6773     self.settings
+0000a690: 5f64 6961 6c6f 672e 4c61 7469 7475 6465  _dialog.Latitude
+0000a6a0: 2e73 6574 5465 7874 2873 7472 2873 656c  .setText(str(sel
+0000a6b0: 662e 7374 6174 696f 6e2e 6765 7428 224c  f.station.get("L
+0000a6c0: 6174 6974 7564 6522 2c20 2222 2929 290a  atitude", ""))).
+0000a6d0: 2020 2020 2020 2020 7365 6c66 2e73 6574          self.set
+0000a6e0: 7469 6e67 735f 6469 616c 6f67 2e4c 6f6e  tings_dialog.Lon
+0000a6f0: 6769 7475 6465 2e73 6574 5465 7874 2873  gitude.setText(s
+0000a700: 7472 2873 656c 662e 7374 6174 696f 6e2e  tr(self.station.
+0000a710: 6765 7428 224c 6f6e 6769 7475 6465 222c  get("Longitude",
+0000a720: 2022 2229 2929 0a20 2020 2020 2020 2073   ""))).        s
+0000a730: 656c 662e 7365 7474 696e 6773 5f64 6961  elf.settings_dia
+0000a740: 6c6f 672e 5374 6174 696f 6e54 5852 582e  log.StationTXRX.
+0000a750: 7365 7454 6578 7428 7365 6c66 2e73 7461  setText(self.sta
+0000a760: 7469 6f6e 2e67 6574 2822 7374 6174 696f  tion.get("statio
+0000a770: 6e74 7872 7822 2c20 2222 2929 0a20 2020  ntxrx", "")).   
+0000a780: 2020 2020 2073 656c 662e 7365 7474 696e       self.settin
+0000a790: 6773 5f64 6961 6c6f 672e 506f 7765 722e  gs_dialog.Power.
+0000a7a0: 7365 7454 6578 7428 7365 6c66 2e73 7461  setText(self.sta
+0000a7b0: 7469 6f6e 2e67 6574 2822 5350 6f77 6522  tion.get("SPowe"
+0000a7c0: 2c20 2222 2929 0a20 2020 2020 2020 2073  , "")).        s
+0000a7d0: 656c 662e 7365 7474 696e 6773 5f64 6961  elf.settings_dia
+0000a7e0: 6c6f 672e 416e 7465 6e6e 612e 7365 7454  log.Antenna.setT
+0000a7f0: 6578 7428 7365 6c66 2e73 7461 7469 6f6e  ext(self.station
+0000a800: 2e67 6574 2822 5341 6e74 6522 2c20 2222  .get("SAnte", ""
+0000a810: 2929 0a20 2020 2020 2020 2073 656c 662e  )).        self.
+0000a820: 7365 7474 696e 6773 5f64 6961 6c6f 672e  settings_dialog.
+0000a830: 416e 7448 6569 6768 742e 7365 7454 6578  AntHeight.setTex
+0000a840: 7428 7365 6c66 2e73 7461 7469 6f6e 2e67  t(self.station.g
+0000a850: 6574 2822 5341 6e74 4831 222c 2022 2229  et("SAntH1", "")
+0000a860: 290a 2020 2020 2020 2020 7365 6c66 2e73  ).        self.s
+0000a870: 6574 7469 6e67 735f 6469 616c 6f67 2e41  ettings_dialog.A
+0000a880: 534c 2e73 6574 5465 7874 2873 656c 662e  SL.setText(self.
+0000a890: 7374 6174 696f 6e2e 6765 7428 2253 416e  station.get("SAn
+0000a8a0: 7448 3222 2c20 2222 2929 0a20 2020 2020  tH2", "")).     
+0000a8b0: 2020 2073 656c 662e 7365 7474 696e 6773     self.settings
+0000a8c0: 5f64 6961 6c6f 672e 4152 524c 5365 6374  _dialog.ARRLSect
+0000a8d0: 696f 6e2e 7365 7454 6578 7428 7365 6c66  ion.setText(self
+0000a8e0: 2e73 7461 7469 6f6e 2e67 6574 2822 4152  .station.get("AR
+0000a8f0: 524c 5365 6374 696f 6e22 2c20 2222 2929  RLSection", ""))
+0000a900: 0a20 2020 2020 2020 2073 656c 662e 7365  .        self.se
+0000a910: 7474 696e 6773 5f64 6961 6c6f 672e 526f  ttings_dialog.Ro
+0000a920: 7665 7251 5448 2e73 6574 5465 7874 2873  verQTH.setText(s
+0000a930: 656c 662e 7374 6174 696f 6e2e 6765 7428  elf.station.get(
+0000a940: 2252 6f76 6572 5154 4822 2c20 2222 2929  "RoverQTH", ""))
+0000a950: 0a20 2020 2020 2020 2073 656c 662e 7365  .        self.se
+0000a960: 7474 696e 6773 5f64 6961 6c6f 672e 436c  ttings_dialog.Cl
+0000a970: 7562 2e73 6574 5465 7874 2873 656c 662e  ub.setText(self.
+0000a980: 7374 6174 696f 6e2e 6765 7428 2243 6c75  station.get("Clu
+0000a990: 6222 2c20 2222 2929 0a20 2020 2020 2020  b", "")).       
+0000a9a0: 2073 656c 662e 7365 7474 696e 6773 5f64   self.settings_d
+0000a9b0: 6961 6c6f 672e 456d 6169 6c2e 7365 7454  ialog.Email.setT
+0000a9c0: 6578 7428 7365 6c66 2e73 7461 7469 6f6e  ext(self.station
+0000a9d0: 2e67 6574 2822 456d 6169 6c22 2c20 2222  .get("Email", ""
+0000a9e0: 2929 0a20 2020 2020 2020 2073 656c 662e  )).        self.
+0000a9f0: 7365 7474 696e 6773 5f64 6961 6c6f 672e  settings_dialog.
+0000aa00: 6f70 656e 2829 0a0a 2020 2020 6465 6620  open()..    def 
+0000aa10: 7361 7665 5f73 6574 7469 6e67 7328 7365  save_settings(se
+0000aa20: 6c66 293a 0a20 2020 2020 2020 2022 2222  lf):.        """
+0000aa30: 5361 7665 2073 6574 7469 6e67 7322 2222  Save settings"""
+0000aa40: 0a20 2020 2020 2020 2063 7320 3d20 7365  .        cs = se
+0000aa50: 6c66 2e73 6574 7469 6e67 735f 6469 616c  lf.settings_dial
+0000aa60: 6f67 2e43 616c 6c2e 7465 7874 2829 0a20  og.Call.text(). 
+0000aa70: 2020 2020 2020 2073 656c 662e 7374 6174         self.stat
+0000aa80: 696f 6e20 3d20 7b7d 0a20 2020 2020 2020  ion = {}.       
+0000aa90: 2073 656c 662e 7374 6174 696f 6e5b 2243   self.station["C
+0000aaa0: 616c 6c22 5d20 3d20 6373 2e75 7070 6572  all"] = cs.upper
+0000aab0: 2829 0a20 2020 2020 2020 2073 656c 662e  ().        self.
+0000aac0: 7374 6174 696f 6e5b 224e 616d 6522 5d20  station["Name"] 
+0000aad0: 3d20 7365 6c66 2e73 6574 7469 6e67 735f  = self.settings_
+0000aae0: 6469 616c 6f67 2e4e 616d 652e 7465 7874  dialog.Name.text
+0000aaf0: 2829 2e74 6974 6c65 2829 0a20 2020 2020  ().title().     
+0000ab00: 2020 2073 656c 662e 7374 6174 696f 6e5b     self.station[
+0000ab10: 2253 7472 6565 7431 225d 203d 2073 656c  "Street1"] = sel
+0000ab20: 662e 7365 7474 696e 6773 5f64 6961 6c6f  f.settings_dialo
+0000ab30: 672e 4164 6472 6573 7331 2e74 6578 7428  g.Address1.text(
+0000ab40: 292e 7469 746c 6528 290a 2020 2020 2020  ).title().      
+0000ab50: 2020 7365 6c66 2e73 7461 7469 6f6e 5b22    self.station["
+0000ab60: 5374 7265 6574 3222 5d20 3d20 7365 6c66  Street2"] = self
+0000ab70: 2e73 6574 7469 6e67 735f 6469 616c 6f67  .settings_dialog
+0000ab80: 2e41 6464 7265 7373 322e 7465 7874 2829  .Address2.text()
+0000ab90: 2e74 6974 6c65 2829 0a20 2020 2020 2020  .title().       
+0000aba0: 2073 656c 662e 7374 6174 696f 6e5b 2243   self.station["C
+0000abb0: 6974 7922 5d20 3d20 7365 6c66 2e73 6574  ity"] = self.set
+0000abc0: 7469 6e67 735f 6469 616c 6f67 2e43 6974  tings_dialog.Cit
+0000abd0: 792e 7465 7874 2829 2e74 6974 6c65 2829  y.text().title()
+0000abe0: 0a20 2020 2020 2020 2073 656c 662e 7374  .        self.st
+0000abf0: 6174 696f 6e5b 2253 7461 7465 225d 203d  ation["State"] =
+0000ac00: 2073 656c 662e 7365 7474 696e 6773 5f64   self.settings_d
+0000ac10: 6961 6c6f 672e 5374 6174 652e 7465 7874  ialog.State.text
+0000ac20: 2829 2e75 7070 6572 2829 0a20 2020 2020  ().upper().     
+0000ac30: 2020 2073 656c 662e 7374 6174 696f 6e5b     self.station[
+0000ac40: 225a 6970 225d 203d 2073 656c 662e 7365  "Zip"] = self.se
+0000ac50: 7474 696e 6773 5f64 6961 6c6f 672e 5a69  ttings_dialog.Zi
+0000ac60: 702e 7465 7874 2829 0a20 2020 2020 2020  p.text().       
+0000ac70: 2073 656c 662e 7374 6174 696f 6e5b 2243   self.station["C
+0000ac80: 6f75 6e74 7279 225d 203d 2073 656c 662e  ountry"] = self.
+0000ac90: 7365 7474 696e 6773 5f64 6961 6c6f 672e  settings_dialog.
+0000aca0: 436f 756e 7472 792e 7465 7874 2829 2e74  Country.text().t
+0000acb0: 6974 6c65 2829 0a20 2020 2020 2020 2073  itle().        s
+0000acc0: 656c 662e 7374 6174 696f 6e5b 2247 7269  elf.station["Gri
+0000acd0: 6453 7175 6172 6522 5d20 3d20 7365 6c66  dSquare"] = self
+0000ace0: 2e73 6574 7469 6e67 735f 6469 616c 6f67  .settings_dialog
+0000acf0: 2e47 7269 6453 7175 6172 652e 7465 7874  .GridSquare.text
+0000ad00: 2829 0a20 2020 2020 2020 2073 656c 662e  ().        self.
+0000ad10: 7374 6174 696f 6e5b 2243 515a 6f6e 6522  station["CQZone"
+0000ad20: 5d20 3d20 7365 6c66 2e73 6574 7469 6e67  ] = self.setting
+0000ad30: 735f 6469 616c 6f67 2e43 515a 6f6e 652e  s_dialog.CQZone.
+0000ad40: 7465 7874 2829 0a20 2020 2020 2020 2073  text().        s
+0000ad50: 656c 662e 7374 6174 696f 6e5b 2249 4152  elf.station["IAR
+0000ad60: 555a 6f6e 6522 5d20 3d20 7365 6c66 2e73  UZone"] = self.s
+0000ad70: 6574 7469 6e67 735f 6469 616c 6f67 2e49  ettings_dialog.I
+0000ad80: 5455 5a6f 6e65 2e74 6578 7428 290a 2020  TUZone.text().  
+0000ad90: 2020 2020 2020 7365 6c66 2e73 7461 7469        self.stati
+0000ada0: 6f6e 5b22 4c69 6365 6e73 6543 6c61 7373  on["LicenseClass
+0000adb0: 225d 203d 2073 656c 662e 7365 7474 696e  "] = self.settin
+0000adc0: 6773 5f64 6961 6c6f 672e 4c69 6365 6e73  gs_dialog.Licens
+0000add0: 652e 7465 7874 2829 2e74 6974 6c65 2829  e.text().title()
+0000ade0: 0a20 2020 2020 2020 2073 656c 662e 7374  .        self.st
+0000adf0: 6174 696f 6e5b 224c 6174 6974 7564 6522  ation["Latitude"
+0000ae00: 5d20 3d20 7365 6c66 2e73 6574 7469 6e67  ] = self.setting
+0000ae10: 735f 6469 616c 6f67 2e4c 6174 6974 7564  s_dialog.Latitud
+0000ae20: 652e 7465 7874 2829 0a20 2020 2020 2020  e.text().       
+0000ae30: 2073 656c 662e 7374 6174 696f 6e5b 224c   self.station["L
+0000ae40: 6f6e 6769 7475 6465 225d 203d 2073 656c  ongitude"] = sel
+0000ae50: 662e 7365 7474 696e 6773 5f64 6961 6c6f  f.settings_dialo
+0000ae60: 672e 4c6f 6e67 6974 7564 652e 7465 7874  g.Longitude.text
+0000ae70: 2829 0a20 2020 2020 2020 2073 656c 662e  ().        self.
+0000ae80: 7374 6174 696f 6e5b 2253 5458 6571 225d  station["STXeq"]
+0000ae90: 203d 2073 656c 662e 7365 7474 696e 6773   = self.settings
+0000aea0: 5f64 6961 6c6f 672e 5374 6174 696f 6e54  _dialog.StationT
+0000aeb0: 5852 582e 7465 7874 2829 0a20 2020 2020  XRX.text().     
+0000aec0: 2020 2073 656c 662e 7374 6174 696f 6e5b     self.station[
+0000aed0: 2253 506f 7765 225d 203d 2073 656c 662e  "SPowe"] = self.
+0000aee0: 7365 7474 696e 6773 5f64 6961 6c6f 672e  settings_dialog.
+0000aef0: 506f 7765 722e 7465 7874 2829 0a20 2020  Power.text().   
+0000af00: 2020 2020 2073 656c 662e 7374 6174 696f       self.statio
+0000af10: 6e5b 2253 416e 7465 225d 203d 2073 656c  n["SAnte"] = sel
+0000af20: 662e 7365 7474 696e 6773 5f64 6961 6c6f  f.settings_dialo
+0000af30: 672e 416e 7465 6e6e 612e 7465 7874 2829  g.Antenna.text()
+0000af40: 0a20 2020 2020 2020 2073 656c 662e 7374  .        self.st
+0000af50: 6174 696f 6e5b 2253 416e 7448 3122 5d20  ation["SAntH1"] 
+0000af60: 3d20 7365 6c66 2e73 6574 7469 6e67 735f  = self.settings_
+0000af70: 6469 616c 6f67 2e41 6e74 4865 6967 6874  dialog.AntHeight
+0000af80: 2e74 6578 7428 290a 2020 2020 2020 2020  .text().        
+0000af90: 7365 6c66 2e73 7461 7469 6f6e 5b22 5341  self.station["SA
+0000afa0: 6e74 4832 225d 203d 2073 656c 662e 7365  ntH2"] = self.se
+0000afb0: 7474 696e 6773 5f64 6961 6c6f 672e 4153  ttings_dialog.AS
+0000afc0: 4c2e 7465 7874 2829 0a20 2020 2020 2020  L.text().       
+0000afd0: 2073 656c 662e 7374 6174 696f 6e5b 2241   self.station["A
+0000afe0: 5252 4c53 6563 7469 6f6e 225d 203d 2073  RRLSection"] = s
+0000aff0: 656c 662e 7365 7474 696e 6773 5f64 6961  elf.settings_dia
+0000b000: 6c6f 672e 4152 524c 5365 6374 696f 6e2e  log.ARRLSection.
+0000b010: 7465 7874 2829 2e75 7070 6572 2829 0a20  text().upper(). 
+0000b020: 2020 2020 2020 2073 656c 662e 7374 6174         self.stat
+0000b030: 696f 6e5b 2252 6f76 6572 5154 4822 5d20  ion["RoverQTH"] 
+0000b040: 3d20 7365 6c66 2e73 6574 7469 6e67 735f  = self.settings_
+0000b050: 6469 616c 6f67 2e52 6f76 6572 5154 482e  dialog.RoverQTH.
+0000b060: 7465 7874 2829 0a20 2020 2020 2020 2073  text().        s
+0000b070: 656c 662e 7374 6174 696f 6e5b 2243 6c75  elf.station["Clu
+0000b080: 6222 5d20 3d20 7365 6c66 2e73 6574 7469  b"] = self.setti
+0000b090: 6e67 735f 6469 616c 6f67 2e43 6c75 622e  ngs_dialog.Club.
+0000b0a0: 7465 7874 2829 2e74 6974 6c65 2829 0a20  text().title(). 
+0000b0b0: 2020 2020 2020 2073 656c 662e 7374 6174         self.stat
+0000b0c0: 696f 6e5b 2245 6d61 696c 225d 203d 2073  ion["Email"] = s
+0000b0d0: 656c 662e 7365 7474 696e 6773 5f64 6961  elf.settings_dia
+0000b0e0: 6c6f 672e 456d 6169 6c2e 7465 7874 2829  log.Email.text()
+0000b0f0: 0a20 2020 2020 2020 2073 656c 662e 6461  .        self.da
+0000b100: 7461 6261 7365 2e61 6464 5f73 7461 7469  tabase.add_stati
+0000b110: 6f6e 2873 656c 662e 7374 6174 696f 6e29  on(self.station)
+0000b120: 0a20 2020 2020 2020 2073 656c 662e 7365  .        self.se
+0000b130: 7474 696e 6773 5f64 6961 6c6f 672e 636c  ttings_dialog.cl
+0000b140: 6f73 6528 290a 2020 2020 2020 2020 6966  ose().        if
+0000b150: 2073 656c 662e 6375 7272 656e 745f 6f70   self.current_op
+0000b160: 203d 3d20 2222 3a0a 2020 2020 2020 2020   == "":.        
+0000b170: 2020 2020 7365 6c66 2e63 7572 7265 6e74      self.current
+0000b180: 5f6f 7020 3d20 7365 6c66 2e73 7461 7469  _op = self.stati
+0000b190: 6f6e 2e67 6574 2822 4361 6c6c 222c 2022  on.get("Call", "
+0000b1a0: 2229 0a20 2020 2020 2020 2020 2020 2073  ").            s
+0000b1b0: 656c 662e 6d61 6b65 5f6f 705f 6469 7228  elf.make_op_dir(
+0000b1c0: 290a 2020 2020 2020 2020 636f 6e74 6573  ).        contes
+0000b1d0: 745f 636f 756e 7420 3d20 7365 6c66 2e64  t_count = self.d
+0000b1e0: 6174 6162 6173 652e 6665 7463 685f 616c  atabase.fetch_al
+0000b1f0: 6c5f 636f 6e74 6573 7473 2829 0a20 2020  l_contests().   
+0000b200: 2020 2020 2069 6620 6c65 6e28 636f 6e74       if len(cont
+0000b210: 6573 745f 636f 756e 7429 203d 3d20 303a  est_count) == 0:
+0000b220: 0a20 2020 2020 2020 2020 2020 2073 656c  .            sel
+0000b230: 662e 6e65 775f 636f 6e74 6573 745f 6469  f.new_contest_di
+0000b240: 616c 6f67 2829 0a0a 2020 2020 6465 6620  alog()..    def 
+0000b250: 6564 6974 5f6d 6163 726f 2873 656c 662c  edit_macro(self,
+0000b260: 2066 756e 6374 696f 6e5f 6b65 7929 3a0a   function_key):.
+0000b270: 2020 2020 2020 2020 2222 2253 686f 7720          """Show 
+0000b280: 6564 6974 206d 6163 726f 2064 6961 6c6f  edit macro dialo
+0000b290: 6722 2222 0a20 2020 2020 2020 2073 656c  g""".        sel
+0000b2a0: 662e 6564 6974 5f6d 6163 726f 5f64 6961  f.edit_macro_dia
+0000b2b0: 6c6f 6720 3d20 4564 6974 4d61 6372 6f28  log = EditMacro(
+0000b2c0: 6675 6e63 7469 6f6e 5f6b 6579 2c20 574f  function_key, WO
+0000b2d0: 524b 494e 475f 5041 5448 290a 2020 2020  RKING_PATH).    
+0000b2e0: 2020 2020 7365 6c66 2e65 6469 745f 6d61      self.edit_ma
+0000b2f0: 6372 6f5f 6469 616c 6f67 2e61 6363 6570  cro_dialog.accep
+0000b300: 7465 642e 636f 6e6e 6563 7428 7365 6c66  ted.connect(self
+0000b310: 2e65 6469 7465 645f 6d61 6372 6f29 0a20  .edited_macro). 
+0000b320: 2020 2020 2020 2069 6620 7365 6c66 2e70         if self.p
+0000b330: 7265 662e 6765 7428 2264 6172 6b5f 6d6f  ref.get("dark_mo
+0000b340: 6465 2229 3a0a 2020 2020 2020 2020 2020  de"):.          
+0000b350: 2020 7365 6c66 2e65 6469 745f 6d61 6372    self.edit_macr
+0000b360: 6f5f 6469 616c 6f67 2e73 6574 5374 796c  o_dialog.setStyl
+0000b370: 6553 6865 6574 2844 4152 4b5f 5354 594c  eSheet(DARK_STYL
+0000b380: 4553 4845 4554 290a 2020 2020 2020 2020  ESHEET).        
+0000b390: 7365 6c66 2e65 6469 745f 6d61 6372 6f5f  self.edit_macro_
+0000b3a0: 6469 616c 6f67 2e6f 7065 6e28 290a 0a20  dialog.open().. 
+0000b3b0: 2020 2064 6566 2065 6469 7465 645f 6d61     def edited_ma
+0000b3c0: 6372 6f28 7365 6c66 293a 0a20 2020 2020  cro(self):.     
+0000b3d0: 2020 2022 2222 5361 7665 2065 6469 7465     """Save edite
+0000b3e0: 6420 6d61 6372 6f22 2222 0a20 2020 2020  d macro""".     
+0000b3f0: 2020 2073 656c 662e 6564 6974 5f6d 6163     self.edit_mac
+0000b400: 726f 5f64 6961 6c6f 672e 6675 6e63 7469  ro_dialog.functi
+0000b410: 6f6e 5f6b 6579 2e73 6574 5465 7874 280a  on_key.setText(.
+0000b420: 2020 2020 2020 2020 2020 2020 7365 6c66              self
+0000b430: 2e65 6469 745f 6d61 6372 6f5f 6469 616c  .edit_macro_dial
+0000b440: 6f67 2e6d 6163 726f 5f6c 6162 656c 2e74  og.macro_label.t
+0000b450: 6578 7428 290a 2020 2020 2020 2020 290a  ext().        ).
+0000b460: 2020 2020 2020 2020 7365 6c66 2e65 6469          self.edi
+0000b470: 745f 6d61 6372 6f5f 6469 616c 6f67 2e66  t_macro_dialog.f
+0000b480: 756e 6374 696f 6e5f 6b65 792e 7365 7454  unction_key.setT
+0000b490: 6f6f 6c54 6970 280a 2020 2020 2020 2020  oolTip(.        
+0000b4a0: 2020 2020 7365 6c66 2e65 6469 745f 6d61      self.edit_ma
+0000b4b0: 6372 6f5f 6469 616c 6f67 2e74 6865 5f6d  cro_dialog.the_m
+0000b4c0: 6163 726f 2e74 6578 7428 290a 2020 2020  acro.text().    
+0000b4d0: 2020 2020 290a 2020 2020 2020 2020 7365      ).        se
+0000b4e0: 6c66 2e65 6469 745f 6d61 6372 6f5f 6469  lf.edit_macro_di
+0000b4f0: 616c 6f67 2e63 6c6f 7365 2829 0a0a 2020  alog.close()..  
+0000b500: 2020 6465 6620 6564 6974 5f46 3128 7365    def edit_F1(se
+0000b510: 6c66 293a 0a20 2020 2020 2020 2022 2222  lf):.        """
+0000b520: 7374 7562 2222 220a 2020 2020 2020 2020  stub""".        
+0000b530: 6c6f 6767 6572 2e64 6562 7567 2822 4631  logger.debug("F1
+0000b540: 2052 6967 6874 2043 6c69 636b 6564 2e22   Right Clicked."
+0000b550: 290a 2020 2020 2020 2020 7365 6c66 2e65  ).        self.e
+0000b560: 6469 745f 6d61 6372 6f28 7365 6c66 2e46  dit_macro(self.F
+0000b570: 3129 0a0a 2020 2020 6465 6620 6564 6974  1)..    def edit
+0000b580: 5f46 3228 7365 6c66 293a 0a20 2020 2020  _F2(self):.     
+0000b590: 2020 2022 2222 7374 7562 2222 220a 2020     """stub""".  
+0000b5a0: 2020 2020 2020 6c6f 6767 6572 2e64 6562        logger.deb
+0000b5b0: 7567 2822 4632 2052 6967 6874 2043 6c69  ug("F2 Right Cli
+0000b5c0: 636b 6564 2e22 290a 2020 2020 2020 2020  cked.").        
+0000b5d0: 7365 6c66 2e65 6469 745f 6d61 6372 6f28  self.edit_macro(
+0000b5e0: 7365 6c66 2e46 3229 0a0a 2020 2020 6465  self.F2)..    de
+0000b5f0: 6620 6564 6974 5f46 3328 7365 6c66 293a  f edit_F3(self):
+0000b600: 0a20 2020 2020 2020 2022 2222 7374 7562  .        """stub
+0000b610: 2222 220a 2020 2020 2020 2020 6c6f 6767  """.        logg
+0000b620: 6572 2e64 6562 7567 2822 4633 2052 6967  er.debug("F3 Rig
+0000b630: 6874 2043 6c69 636b 6564 2e22 290a 2020  ht Clicked.").  
+0000b640: 2020 2020 2020 7365 6c66 2e65 6469 745f        self.edit_
+0000b650: 6d61 6372 6f28 7365 6c66 2e46 3329 0a0a  macro(self.F3)..
+0000b660: 2020 2020 6465 6620 6564 6974 5f46 3428      def edit_F4(
+0000b670: 7365 6c66 293a 0a20 2020 2020 2020 2022  self):.        "
+0000b680: 2222 7374 7562 2222 220a 2020 2020 2020  ""stub""".      
+0000b690: 2020 6c6f 6767 6572 2e64 6562 7567 2822    logger.debug("
+0000b6a0: 4634 2052 6967 6874 2043 6c69 636b 6564  F4 Right Clicked
+0000b6b0: 2e22 290a 2020 2020 2020 2020 7365 6c66  .").        self
+0000b6c0: 2e65 6469 745f 6d61 6372 6f28 7365 6c66  .edit_macro(self
+0000b6d0: 2e46 3429 0a0a 2020 2020 6465 6620 6564  .F4)..    def ed
+0000b6e0: 6974 5f46 3528 7365 6c66 293a 0a20 2020  it_F5(self):.   
+0000b6f0: 2020 2020 2022 2222 7374 7562 2222 220a       """stub""".
+0000b700: 2020 2020 2020 2020 6c6f 6767 6572 2e64          logger.d
+0000b710: 6562 7567 2822 4635 2052 6967 6874 2043  ebug("F5 Right C
+0000b720: 6c69 636b 6564 2e22 290a 2020 2020 2020  licked.").      
+0000b730: 2020 7365 6c66 2e65 6469 745f 6d61 6372    self.edit_macr
+0000b740: 6f28 7365 6c66 2e46 3529 0a0a 2020 2020  o(self.F5)..    
+0000b750: 6465 6620 6564 6974 5f46 3628 7365 6c66  def edit_F6(self
+0000b760: 293a 0a20 2020 2020 2020 2022 2222 7374  ):.        """st
+0000b770: 7562 2222 220a 2020 2020 2020 2020 6c6f  ub""".        lo
+0000b780: 6767 6572 2e64 6562 7567 2822 4636 2052  gger.debug("F6 R
+0000b790: 6967 6874 2043 6c69 636b 6564 2e22 290a  ight Clicked.").
+0000b7a0: 2020 2020 2020 2020 7365 6c66 2e65 6469          self.edi
+0000b7b0: 745f 6d61 6372 6f28 7365 6c66 2e46 3629  t_macro(self.F6)
+0000b7c0: 0a0a 2020 2020 6465 6620 6564 6974 5f46  ..    def edit_F
+0000b7d0: 3728 7365 6c66 293a 0a20 2020 2020 2020  7(self):.       
+0000b7e0: 2022 2222 7374 7562 2222 220a 2020 2020   """stub""".    
+0000b7f0: 2020 2020 6c6f 6767 6572 2e64 6562 7567      logger.debug
+0000b800: 2822 4637 2052 6967 6874 2043 6c69 636b  ("F7 Right Click
+0000b810: 6564 2e22 290a 2020 2020 2020 2020 7365  ed.").        se
+0000b820: 6c66 2e65 6469 745f 6d61 6372 6f28 7365  lf.edit_macro(se
+0000b830: 6c66 2e46 3729 0a0a 2020 2020 6465 6620  lf.F7)..    def 
+0000b840: 6564 6974 5f46 3828 7365 6c66 293a 0a20  edit_F8(self):. 
+0000b850: 2020 2020 2020 2022 2222 7374 7562 2222         """stub""
+0000b860: 220a 2020 2020 2020 2020 6c6f 6767 6572  ".        logger
+0000b870: 2e64 6562 7567 2822 4638 2052 6967 6874  .debug("F8 Right
+0000b880: 2043 6c69 636b 6564 2e22 290a 2020 2020   Clicked.").    
+0000b890: 2020 2020 7365 6c66 2e65 6469 745f 6d61      self.edit_ma
+0000b8a0: 6372 6f28 7365 6c66 2e46 3829 0a0a 2020  cro(self.F8)..  
+0000b8b0: 2020 6465 6620 6564 6974 5f46 3928 7365    def edit_F9(se
+0000b8c0: 6c66 293a 0a20 2020 2020 2020 2022 2222  lf):.        """
+0000b8d0: 7374 7562 2222 220a 2020 2020 2020 2020  stub""".        
+0000b8e0: 6c6f 6767 6572 2e64 6562 7567 2822 4639  logger.debug("F9
+0000b8f0: 2052 6967 6874 2043 6c69 636b 6564 2e22   Right Clicked."
+0000b900: 290a 2020 2020 2020 2020 7365 6c66 2e65  ).        self.e
+0000b910: 6469 745f 6d61 6372 6f28 7365 6c66 2e46  dit_macro(self.F
+0000b920: 3929 0a0a 2020 2020 6465 6620 6564 6974  9)..    def edit
+0000b930: 5f46 3130 2873 656c 6629 3a0a 2020 2020  _F10(self):.    
+0000b940: 2020 2020 2222 2273 7475 6222 2222 0a20      """stub""". 
+0000b950: 2020 2020 2020 206c 6f67 6765 722e 6465         logger.de
+0000b960: 6275 6728 2246 3130 2052 6967 6874 2043  bug("F10 Right C
+0000b970: 6c69 636b 6564 2e22 290a 2020 2020 2020  licked.").      
+0000b980: 2020 7365 6c66 2e65 6469 745f 6d61 6372    self.edit_macr
+0000b990: 6f28 7365 6c66 2e46 3130 290a 0a20 2020  o(self.F10)..   
+0000b9a0: 2064 6566 2065 6469 745f 4631 3128 7365   def edit_F11(se
+0000b9b0: 6c66 293a 0a20 2020 2020 2020 2022 2222  lf):.        """
+0000b9c0: 7374 7562 2222 220a 2020 2020 2020 2020  stub""".        
+0000b9d0: 6c6f 6767 6572 2e64 6562 7567 2822 4631  logger.debug("F1
+0000b9e0: 3120 5269 6768 7420 436c 6963 6b65 642e  1 Right Clicked.
+0000b9f0: 2229 0a20 2020 2020 2020 2073 656c 662e  ").        self.
+0000ba00: 6564 6974 5f6d 6163 726f 2873 656c 662e  edit_macro(self.
+0000ba10: 4631 3129 0a0a 2020 2020 6465 6620 6564  F11)..    def ed
+0000ba20: 6974 5f46 3132 2873 656c 6629 3a0a 2020  it_F12(self):.  
+0000ba30: 2020 2020 2020 2222 2273 7475 6222 2222        """stub"""
+0000ba40: 0a20 2020 2020 2020 206c 6f67 6765 722e  .        logger.
+0000ba50: 6465 6275 6728 2246 3132 2052 6967 6874  debug("F12 Right
+0000ba60: 2043 6c69 636b 6564 2e22 290a 2020 2020   Clicked.").    
+0000ba70: 2020 2020 7365 6c66 2e65 6469 745f 6d61      self.edit_ma
+0000ba80: 6372 6f28 7365 6c66 2e46 3132 290a 0a20  cro(self.F12).. 
+0000ba90: 2020 2064 6566 2070 726f 6365 7373 5f6d     def process_m
+0000baa0: 6163 726f 2873 656c 662c 206d 6163 726f  acro(self, macro
+0000bab0: 3a20 7374 7229 202d 3e20 7374 723a 0a20  : str) -> str:. 
+0000bac0: 2020 2020 2020 2022 2222 5072 6f63 6573         """Proces
+0000bad0: 7320 4357 206d 6163 726f 2073 7562 7374  s CW macro subst
+0000bae0: 6974 7574 696f 6e73 2222 220a 2020 2020  itutions""".    
+0000baf0: 2020 2020 7265 7375 6c74 203d 2073 656c      result = sel
+0000bb00: 662e 6461 7461 6261 7365 2e67 6574 5f73  f.database.get_s
+0000bb10: 6572 6961 6c28 290a 2020 2020 2020 2020  erial().        
+0000bb20: 6e65 7874 5f73 6572 6961 6c20 3d20 7374  next_serial = st
+0000bb30: 7228 7265 7375 6c74 2e67 6574 2822 7365  r(result.get("se
+0000bb40: 7269 616c 5f6e 7222 2c20 2231 2229 290a  rial_nr", "1")).
+0000bb50: 2020 2020 2020 2020 6966 206e 6578 745f          if next_
+0000bb60: 7365 7269 616c 203d 3d20 224e 6f6e 6522  serial == "None"
+0000bb70: 3a0a 2020 2020 2020 2020 2020 2020 6e65  :.            ne
+0000bb80: 7874 5f73 6572 6961 6c20 3d20 2231 220a  xt_serial = "1".
+0000bb90: 2020 2020 2020 2020 6d61 6372 6f20 3d20          macro = 
+0000bba0: 6d61 6372 6f2e 7570 7065 7228 290a 2020  macro.upper().  
+0000bbb0: 2020 2020 2020 6d61 6372 6f20 3d20 6d61        macro = ma
+0000bbc0: 6372 6f2e 7265 706c 6163 6528 2223 222c  cro.replace("#",
+0000bbd0: 206e 6578 745f 7365 7269 616c 290a 2020   next_serial).  
+0000bbe0: 2020 2020 2020 6d61 6372 6f20 3d20 6d61        macro = ma
+0000bbf0: 6372 6f2e 7265 706c 6163 6528 227b 4d59  cro.replace("{MY
+0000bc00: 4341 4c4c 7d22 2c20 7365 6c66 2e73 7461  CALL}", self.sta
+0000bc10: 7469 6f6e 2e67 6574 2822 4361 6c6c 222c  tion.get("Call",
+0000bc20: 2022 2229 290a 2020 2020 2020 2020 6d61   "")).        ma
+0000bc30: 6372 6f20 3d20 6d61 6372 6f2e 7265 706c  cro = macro.repl
+0000bc40: 6163 6528 227b 4849 5343 414c 4c7d 222c  ace("{HISCALL}",
+0000bc50: 2073 656c 662e 6361 6c6c 7369 676e 2e74   self.callsign.t
+0000bc60: 6578 7428 2929 0a20 2020 2020 2020 2069  ext()).        i
+0000bc70: 6620 7365 6c66 2e72 6164 696f 5f73 7461  f self.radio_sta
+0000bc80: 7465 2e67 6574 2822 6d6f 6465 2229 203d  te.get("mode") =
+0000bc90: 3d20 2243 5722 3a0a 2020 2020 2020 2020  = "CW":.        
+0000bca0: 2020 2020 6d61 6372 6f20 3d20 6d61 6372      macro = macr
+0000bcb0: 6f2e 7265 706c 6163 6528 227b 534e 547d  o.replace("{SNT}
+0000bcc0: 222c 2073 656c 662e 7365 6e74 2e74 6578  ", self.sent.tex
+0000bcd0: 7428 292e 7265 706c 6163 6528 2239 222c  t().replace("9",
+0000bce0: 2022 6e22 2929 0a20 2020 2020 2020 2065   "n")).        e
+0000bcf0: 6c73 653a 0a20 2020 2020 2020 2020 2020  lse:.           
+0000bd00: 206d 6163 726f 203d 206d 6163 726f 2e72   macro = macro.r
+0000bd10: 6570 6c61 6365 2822 7b53 4e54 7d22 2c20  eplace("{SNT}", 
+0000bd20: 7365 6c66 2e73 656e 742e 7465 7874 2829  self.sent.text()
+0000bd30: 290a 2020 2020 2020 2020 6d61 6372 6f20  ).        macro 
+0000bd40: 3d20 6d61 6372 6f2e 7265 706c 6163 6528  = macro.replace(
+0000bd50: 227b 5345 4e54 4e52 7d22 2c20 7365 6c66  "{SENTNR}", self
+0000bd60: 2e6f 7468 6572 5f31 2e74 6578 7428 2929  .other_1.text())
+0000bd70: 0a20 2020 2020 2020 206d 6163 726f 203d  .        macro =
+0000bd80: 206d 6163 726f 2e72 6570 6c61 6365 280a   macro.replace(.
+0000bd90: 2020 2020 2020 2020 2020 2020 227b 4558              "{EX
+0000bda0: 4348 7d22 2c20 7365 6c66 2e63 6f6e 7465  CH}", self.conte
+0000bdb0: 7374 5f73 6574 7469 6e67 732e 6765 7428  st_settings.get(
+0000bdc0: 2253 656e 7445 7863 6861 6e67 6522 2c20  "SentExchange", 
+0000bdd0: 2278 7878 2229 0a20 2020 2020 2020 2029  "xxx").        )
+0000bde0: 0a20 2020 2020 2020 2072 6574 7572 6e20  .        return 
+0000bdf0: 6d61 6372 6f0a 0a20 2020 2064 6566 2076  macro..    def v
+0000be00: 6f69 6365 5f73 7472 696e 6728 7365 6c66  oice_string(self
+0000be10: 2c20 7468 655f 7374 7269 6e67 3a20 7374  , the_string: st
+0000be20: 7229 202d 3e20 4e6f 6e65 3a0a 2020 2020  r) -> None:.    
+0000be30: 2020 2020 2222 2276 6f69 6365 7320 7374      """voices st
+0000be40: 7269 6e67 2075 7369 6e67 206e 6174 6f20  ring using nato 
+0000be50: 7068 6f6e 6574 6963 7322 2222 0a20 2020  phonetics""".   
+0000be60: 2020 2020 206c 6f67 6765 722e 6465 6275       logger.debu
+0000be70: 6728 2256 6f69 6369 6e67 3a20 2573 222c  g("Voicing: %s",
+0000be80: 2074 6865 5f73 7472 696e 6729 0a20 2020   the_string).   
+0000be90: 2020 2020 206f 705f 7061 7468 203d 2050       op_path = P
+0000bea0: 6174 6828 4441 5441 5f50 4154 4829 202f  ath(DATA_PATH) /
+0000beb0: 2073 656c 662e 6375 7272 656e 745f 6f70   self.current_op
+0000bec0: 0a20 2020 2020 2020 2069 6620 225b 2220  .        if "[" 
+0000bed0: 696e 2074 6865 5f73 7472 696e 673a 0a20  in the_string:. 
+0000bee0: 2020 2020 2020 2020 2020 2073 7562 5f73             sub_s
+0000bef0: 7472 696e 6720 3d20 7468 655f 7374 7269  tring = the_stri
+0000bf00: 6e67 2e73 7472 6970 2822 5b5d 2229 2e6c  ng.strip("[]").l
+0000bf10: 6f77 6572 2829 0a20 2020 2020 2020 2020  ower().         
+0000bf20: 2020 2066 696c 656e 616d 6520 3d20 6622     filename = f"
+0000bf30: 7b73 7472 286f 705f 7061 7468 297d 2f7b  {str(op_path)}/{
+0000bf40: 7375 625f 7374 7269 6e67 7d2e 7761 7622  sub_string}.wav"
+0000bf50: 0a20 2020 2020 2020 2020 2020 2069 6620  .            if 
+0000bf60: 5061 7468 2866 696c 656e 616d 6529 2e69  Path(filename).i
+0000bf70: 735f 6669 6c65 2829 3a0a 2020 2020 2020  s_file():.      
+0000bf80: 2020 2020 2020 2020 2020 6c6f 6767 6572            logger
+0000bf90: 2e64 6562 7567 2822 566f 6963 696e 673a  .debug("Voicing:
+0000bfa0: 2025 7322 2c20 6669 6c65 6e61 6d65 290a   %s", filename).
+0000bfb0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000bfc0: 6461 7461 2c20 5f66 7320 3d20 7366 2e72  data, _fs = sf.r
+0000bfd0: 6561 6428 6669 6c65 6e61 6d65 2c20 6474  ead(filename, dt
+0000bfe0: 7970 653d 2266 6c6f 6174 3332 2229 0a20  ype="float32"). 
+0000bff0: 2020 2020 2020 2020 2020 2020 2020 2073                 s
+0000c000: 656c 662e 7074 745f 6f6e 2829 0a20 2020  elf.ptt_on().   
+0000c010: 2020 2020 2020 2020 2020 2020 2074 7279               try
+0000c020: 3a0a 2020 2020 2020 2020 2020 2020 2020  :.              
+0000c030: 2020 2020 2020 7364 2e64 6566 6175 6c74        sd.default
+0000c040: 2e64 6576 6963 6520 3d20 7365 6c66 2e70  .device = self.p
+0000c050: 7265 662e 6765 7428 2273 6f75 6e64 6465  ref.get("soundde
+0000c060: 7669 6365 222c 2022 6465 6661 756c 7422  vice", "default"
+0000c070: 290a 2020 2020 2020 2020 2020 2020 2020  ).              
+0000c080: 2020 2020 2020 7364 2e64 6566 6175 6c74        sd.default
+0000c090: 2e73 616d 706c 6572 6174 6520 3d20 3434  .samplerate = 44
+0000c0a0: 3130 302e 300a 2020 2020 2020 2020 2020  100.0.          
+0000c0b0: 2020 2020 2020 2020 2020 7364 2e70 6c61            sd.pla
+0000c0c0: 7928 6461 7461 290a 2020 2020 2020 2020  y(data).        
+0000c0d0: 2020 2020 2020 2020 2020 2020 5f73 7461              _sta
+0000c0e0: 7475 7320 3d20 7364 2e77 6169 7428 290a  tus = sd.wait().
 0000c0f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000c100: 2020 2023 2068 7474 7073 3a2f 2f73 6e79     # https://sny
-0000c110: 6b2e 696f 2f61 6476 6973 6f72 2f70 7974  k.io/advisor/pyt
-0000c120: 686f 6e2f 736f 756e 6464 6576 6963 652f  hon/sounddevice/
-0000c130: 6675 6e63 7469 6f6e 732f 736f 756e 6464  functions/soundd
-0000c140: 6576 6963 652e 506f 7274 4175 6469 6f45  evice.PortAudioE
-0000c150: 7272 6f72 0a20 2020 2020 2020 2020 2020  rror.           
-0000c160: 2020 2020 2065 7863 6570 7420 7364 2e50       except sd.P
-0000c170: 6f72 7441 7564 696f 4572 726f 7220 6173  ortAudioError as
-0000c180: 2065 7272 3a0a 2020 2020 2020 2020 2020   err:.          
-0000c190: 2020 2020 2020 2020 2020 6c6f 6767 6572            logger
-0000c1a0: 2e64 6562 7567 2822 2573 222c 2066 227b  .debug("%s", f"{
-0000c1b0: 6572 727d 2229 0a0a 2020 2020 2020 2020  err}")..        
-0000c1c0: 2020 2020 2020 2020 7365 6c66 2e70 7474          self.ptt
-0000c1d0: 5f6f 6666 2829 0a20 2020 2020 2020 2020  _off().         
-0000c1e0: 2020 2072 6574 7572 6e0a 2020 2020 2020     return.      
-0000c1f0: 2020 7365 6c66 2e70 7474 5f6f 6e28 290a    self.ptt_on().
-0000c200: 2020 2020 2020 2020 666f 7220 6c65 7474          for lett
-0000c210: 6572 2069 6e20 7468 655f 7374 7269 6e67  er in the_string
-0000c220: 2e6c 6f77 6572 2829 3a0a 2020 2020 2020  .lower():.      
-0000c230: 2020 2020 2020 6966 206c 6574 7465 7220        if letter 
-0000c240: 696e 2022 6162 6364 6566 6768 696a 6b6c  in "abcdefghijkl
-0000c250: 6d6e 6f70 7172 7374 7576 7778 797a 2031  mnopqrstuvwxyz 1
-0000c260: 3233 3435 3637 3839 3022 3a0a 2020 2020  234567890":.    
-0000c270: 2020 2020 2020 2020 2020 2020 6966 206c              if l
-0000c280: 6574 7465 7220 3d3d 2022 2022 3a0a 2020  etter == " ":.  
+0000c100: 2020 2020 2320 6874 7470 733a 2f2f 736e      # https://sn
+0000c110: 796b 2e69 6f2f 6164 7669 736f 722f 7079  yk.io/advisor/py
+0000c120: 7468 6f6e 2f73 6f75 6e64 6465 7669 6365  thon/sounddevice
+0000c130: 2f66 756e 6374 696f 6e73 2f73 6f75 6e64  /functions/sound
+0000c140: 6465 7669 6365 2e50 6f72 7441 7564 696f  device.PortAudio
+0000c150: 4572 726f 720a 2020 2020 2020 2020 2020  Error.          
+0000c160: 2020 2020 2020 6578 6365 7074 2073 642e        except sd.
+0000c170: 506f 7274 4175 6469 6f45 7272 6f72 2061  PortAudioError a
+0000c180: 7320 6572 723a 0a20 2020 2020 2020 2020  s err:.         
+0000c190: 2020 2020 2020 2020 2020 206c 6f67 6765             logge
+0000c1a0: 722e 6465 6275 6728 2225 7322 2c20 6622  r.debug("%s", f"
+0000c1b0: 7b65 7272 7d22 290a 0a20 2020 2020 2020  {err}")..       
+0000c1c0: 2020 2020 2020 2020 2073 656c 662e 7074           self.pt
+0000c1d0: 745f 6f66 6628 290a 2020 2020 2020 2020  t_off().        
+0000c1e0: 2020 2020 7265 7475 726e 0a20 2020 2020      return.     
+0000c1f0: 2020 2073 656c 662e 7074 745f 6f6e 2829     self.ptt_on()
+0000c200: 0a20 2020 2020 2020 2066 6f72 206c 6574  .        for let
+0000c210: 7465 7220 696e 2074 6865 5f73 7472 696e  ter in the_strin
+0000c220: 672e 6c6f 7765 7228 293a 0a20 2020 2020  g.lower():.     
+0000c230: 2020 2020 2020 2069 6620 6c65 7474 6572         if letter
+0000c240: 2069 6e20 2261 6263 6465 6667 6869 6a6b   in "abcdefghijk
+0000c250: 6c6d 6e6f 7071 7273 7475 7677 7879 7a20  lmnopqrstuvwxyz 
+0000c260: 3132 3334 3536 3738 3930 223a 0a20 2020  1234567890":.   
+0000c270: 2020 2020 2020 2020 2020 2020 2069 6620               if 
+0000c280: 6c65 7474 6572 203d 3d20 2220 223a 0a20  letter == " ":. 
 0000c290: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000c2a0: 2020 6c65 7474 6572 203d 2022 7370 6163    letter = "spac
-0000c2b0: 6522 0a20 2020 2020 2020 2020 2020 2020  e".             
-0000c2c0: 2020 2066 696c 656e 616d 6520 3d20 6622     filename = f"
-0000c2d0: 7b73 7472 286f 705f 7061 7468 297d 2f7b  {str(op_path)}/{
-0000c2e0: 6c65 7474 6572 7d2e 7761 7622 0a20 2020  letter}.wav".   
-0000c2f0: 2020 2020 2020 2020 2020 2020 2069 6620               if 
-0000c300: 5061 7468 2866 696c 656e 616d 6529 2e69  Path(filename).i
-0000c310: 735f 6669 6c65 2829 3a0a 2020 2020 2020  s_file():.      
-0000c320: 2020 2020 2020 2020 2020 2020 2020 6c6f                lo
-0000c330: 6767 6572 2e64 6562 7567 2822 566f 6963  gger.debug("Voic
-0000c340: 696e 673a 2025 7322 2c20 6669 6c65 6e61  ing: %s", filena
-0000c350: 6d65 290a 2020 2020 2020 2020 2020 2020  me).            
-0000c360: 2020 2020 2020 2020 6461 7461 2c20 5f66          data, _f
-0000c370: 7320 3d20 7366 2e72 6561 6428 6669 6c65  s = sf.read(file
-0000c380: 6e61 6d65 2c20 6474 7970 653d 2266 6c6f  name, dtype="flo
-0000c390: 6174 3332 2229 0a20 2020 2020 2020 2020  at32").         
-0000c3a0: 2020 2020 2020 2020 2020 2074 7279 3a0a             try:.
-0000c3b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000c3c0: 2020 2020 2020 2020 7364 2e64 6566 6175          sd.defau
-0000c3d0: 6c74 2e64 6576 6963 6520 3d20 7365 6c66  lt.device = self
-0000c3e0: 2e70 7265 662e 6765 7428 2273 6f75 6e64  .pref.get("sound
-0000c3f0: 6465 7669 6365 222c 2022 6465 6661 756c  device", "defaul
-0000c400: 7422 290a 2020 2020 2020 2020 2020 2020  t").            
-0000c410: 2020 2020 2020 2020 2020 2020 7364 2e64              sd.d
-0000c420: 6566 6175 6c74 2e73 616d 706c 6572 6174  efault.samplerat
-0000c430: 6520 3d20 3434 3130 302e 300a 2020 2020  e = 44100.0.    
+0000c2a0: 2020 206c 6574 7465 7220 3d20 2273 7061     letter = "spa
+0000c2b0: 6365 220a 2020 2020 2020 2020 2020 2020  ce".            
+0000c2c0: 2020 2020 6669 6c65 6e61 6d65 203d 2066      filename = f
+0000c2d0: 227b 7374 7228 6f70 5f70 6174 6829 7d2f  "{str(op_path)}/
+0000c2e0: 7b6c 6574 7465 727d 2e77 6176 220a 2020  {letter}.wav".  
+0000c2f0: 2020 2020 2020 2020 2020 2020 2020 6966                if
+0000c300: 2050 6174 6828 6669 6c65 6e61 6d65 292e   Path(filename).
+0000c310: 6973 5f66 696c 6528 293a 0a20 2020 2020  is_file():.     
+0000c320: 2020 2020 2020 2020 2020 2020 2020 206c                 l
+0000c330: 6f67 6765 722e 6465 6275 6728 2256 6f69  ogger.debug("Voi
+0000c340: 6369 6e67 3a20 2573 222c 2066 696c 656e  cing: %s", filen
+0000c350: 616d 6529 0a20 2020 2020 2020 2020 2020  ame).           
+0000c360: 2020 2020 2020 2020 2064 6174 612c 205f           data, _
+0000c370: 6673 203d 2073 662e 7265 6164 2866 696c  fs = sf.read(fil
+0000c380: 656e 616d 652c 2064 7479 7065 3d22 666c  ename, dtype="fl
+0000c390: 6f61 7433 3222 290a 2020 2020 2020 2020  oat32").        
+0000c3a0: 2020 2020 2020 2020 2020 2020 7472 793a              try:
+0000c3b0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+0000c3c0: 2020 2020 2020 2020 2073 642e 6465 6661           sd.defa
+0000c3d0: 756c 742e 6465 7669 6365 203d 2073 656c  ult.device = sel
+0000c3e0: 662e 7072 6566 2e67 6574 2822 736f 756e  f.pref.get("soun
+0000c3f0: 6464 6576 6963 6522 2c20 2264 6566 6175  ddevice", "defau
+0000c400: 6c74 2229 0a20 2020 2020 2020 2020 2020  lt").           
+0000c410: 2020 2020 2020 2020 2020 2020 2073 642e               sd.
+0000c420: 6465 6661 756c 742e 7361 6d70 6c65 7261  default.samplera
+0000c430: 7465 203d 2034 3431 3030 2e30 0a20 2020  te = 44100.0.   
 0000c440: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000c450: 2020 2020 7364 2e70 6c61 7928 6461 7461      sd.play(data
-0000c460: 290a 2020 2020 2020 2020 2020 2020 2020  ).              
-0000c470: 2020 2020 2020 2020 2020 6c6f 6767 6572            logger
-0000c480: 2e64 6562 7567 2822 2573 222c 2066 227b  .debug("%s", f"{
-0000c490: 7364 2e77 6169 7428 297d 2229 0a20 2020  sd.wait()}").   
+0000c450: 2020 2020 2073 642e 706c 6179 2864 6174       sd.play(dat
+0000c460: 6129 0a20 2020 2020 2020 2020 2020 2020  a).             
+0000c470: 2020 2020 2020 2020 2020 206c 6f67 6765             logge
+0000c480: 722e 6465 6275 6728 2225 7322 2c20 6622  r.debug("%s", f"
+0000c490: 7b73 642e 7761 6974 2829 7d22 290a 2020  {sd.wait()}").  
 0000c4a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000c4b0: 2065 7863 6570 7420 7364 2e50 6f72 7441   except sd.PortA
-0000c4c0: 7564 696f 4572 726f 7220 6173 2065 7272  udioError as err
-0000c4d0: 3a0a 2020 2020 2020 2020 2020 2020 2020  :.              
-0000c4e0: 2020 2020 2020 2020 2020 6c6f 6767 6572            logger
-0000c4f0: 2e64 6562 7567 2822 2573 222c 2066 227b  .debug("%s", f"{
-0000c500: 6572 727d 2229 0a20 2020 2020 2020 2073  err}").        s
-0000c510: 656c 662e 7074 745f 6f66 6628 290a 0a20  elf.ptt_off().. 
-0000c520: 2020 2064 6566 2070 7474 5f6f 6e28 7365     def ptt_on(se
-0000c530: 6c66 293a 0a20 2020 2020 2020 2022 2222  lf):.        """
-0000c540: 7475 726e 206f 6e20 7074 7422 2222 0a20  turn on ptt""". 
-0000c550: 2020 2020 2020 2069 6620 7365 6c66 2e72         if self.r
-0000c560: 6967 5f63 6f6e 7472 6f6c 3a0a 2020 2020  ig_control:.    
-0000c570: 2020 2020 2020 2020 7365 6c66 2e6c 6566          self.lef
-0000c580: 7464 6f74 2e73 6574 5069 786d 6170 2873  tdot.setPixmap(s
-0000c590: 656c 662e 6772 6565 6e64 6f74 290a 2020  elf.greendot).  
-0000c5a0: 2020 2020 2020 2020 2020 6170 702e 7072            app.pr
-0000c5b0: 6f63 6573 7345 7665 6e74 7328 290a 2020  ocessEvents().  
-0000c5c0: 2020 2020 2020 2020 2020 7365 6c66 2e72            self.r
-0000c5d0: 6967 5f63 6f6e 7472 6f6c 2e70 7474 5f6f  ig_control.ptt_o
-0000c5e0: 6e28 290a 0a20 2020 2064 6566 2070 7474  n()..    def ptt
-0000c5f0: 5f6f 6666 2873 656c 6629 3a0a 2020 2020  _off(self):.    
-0000c600: 2020 2020 2222 2274 7572 6e20 6f66 6620      """turn off 
-0000c610: 7074 7422 2222 0a20 2020 2020 2020 2073  ptt""".        s
-0000c620: 656c 662e 6c65 6674 646f 742e 7365 7450  elf.leftdot.setP
-0000c630: 6978 6d61 7028 7365 6c66 2e72 6564 646f  ixmap(self.reddo
-0000c640: 7429 0a20 2020 2020 2020 2061 7070 2e70  t).        app.p
-0000c650: 726f 6365 7373 4576 656e 7473 2829 0a20  rocessEvents(). 
-0000c660: 2020 2020 2020 2073 656c 662e 7269 675f         self.rig_
-0000c670: 636f 6e74 726f 6c2e 7074 745f 6f66 6628  control.ptt_off(
-0000c680: 290a 0a20 2020 2064 6566 2073 656e 6466  )..    def sendf
-0000c690: 3128 7365 6c66 293a 0a20 2020 2020 2020  1(self):.       
-0000c6a0: 2022 2222 7374 7562 2222 220a 2020 2020   """stub""".    
-0000c6b0: 2020 2020 6c6f 6767 6572 2e64 6562 7567      logger.debug
-0000c6c0: 2822 4631 2043 6c69 636b 6564 2229 0a20  ("F1 Clicked"). 
-0000c6d0: 2020 2020 2020 2069 6620 7365 6c66 2e72         if self.r
-0000c6e0: 6164 696f 5f73 7461 7465 2e67 6574 2822  adio_state.get("
-0000c6f0: 6d6f 6465 2229 2069 6e20 5b22 4c53 4222  mode") in ["LSB"
-0000c700: 2c20 2255 5342 222c 2022 5353 4222 5d3a  , "USB", "SSB"]:
-0000c710: 0a20 2020 2020 2020 2020 2020 2073 656c  .            sel
-0000c720: 662e 766f 6963 655f 7374 7269 6e67 2873  f.voice_string(s
-0000c730: 656c 662e 7072 6f63 6573 735f 6d61 6372  elf.process_macr
-0000c740: 6f28 7365 6c66 2e46 312e 746f 6f6c 5469  o(self.F1.toolTi
-0000c750: 7028 2929 290a 2020 2020 2020 2020 2020  p())).          
-0000c760: 2020 7265 7475 726e 0a20 2020 2020 2020    return.       
-0000c770: 2069 6620 7365 6c66 2e63 773a 0a20 2020   if self.cw:.   
-0000c780: 2020 2020 2020 2020 2023 2069 6620 7365           # if se
-0000c790: 6c66 2e70 7265 6665 7265 6e63 652e 6765  lf.preference.ge
-0000c7a0: 7428 2273 656e 645f 6e31 6d6d 5f70 6163  t("send_n1mm_pac
-0000c7b0: 6b65 7473 2229 3a0a 2020 2020 2020 2020  kets"):.        
-0000c7c0: 2020 2020 2320 2020 2020 7365 6c66 2e6e      #     self.n
-0000c7d0: 316d 6d2e 7261 6469 6f5f 696e 666f 5b22  1mm.radio_info["
-0000c7e0: 4675 6e63 7469 6f6e 4b65 7943 6170 7469  FunctionKeyCapti
-0000c7f0: 6f6e 225d 203d 2073 656c 662e 4631 2e74  on"] = self.F1.t
-0000c800: 6578 7428 290a 2020 2020 2020 2020 2020  ext().          
-0000c810: 2020 7365 6c66 2e63 772e 7365 6e64 6377    self.cw.sendcw
-0000c820: 2873 656c 662e 7072 6f63 6573 735f 6d61  (self.process_ma
-0000c830: 6372 6f28 7365 6c66 2e46 312e 746f 6f6c  cro(self.F1.tool
-0000c840: 5469 7028 2929 290a 0a20 2020 2064 6566  Tip()))..    def
-0000c850: 2073 656e 6466 3228 7365 6c66 293a 0a20   sendf2(self):. 
-0000c860: 2020 2020 2020 2022 2222 7374 7562 2222         """stub""
-0000c870: 220a 2020 2020 2020 2020 6c6f 6767 6572  ".        logger
-0000c880: 2e64 6562 7567 2822 4632 2043 6c69 636b  .debug("F2 Click
-0000c890: 6564 2229 0a20 2020 2020 2020 2069 6620  ed").        if 
-0000c8a0: 7365 6c66 2e72 6164 696f 5f73 7461 7465  self.radio_state
-0000c8b0: 2e67 6574 2822 6d6f 6465 2229 2069 6e20  .get("mode") in 
-0000c8c0: 5b22 4c53 4222 2c20 2255 5342 222c 2022  ["LSB", "USB", "
-0000c8d0: 5353 4222 5d3a 0a20 2020 2020 2020 2020  SSB"]:.         
-0000c8e0: 2020 2073 656c 662e 766f 6963 655f 7374     self.voice_st
-0000c8f0: 7269 6e67 2873 656c 662e 7072 6f63 6573  ring(self.proces
-0000c900: 735f 6d61 6372 6f28 7365 6c66 2e46 322e  s_macro(self.F2.
-0000c910: 746f 6f6c 5469 7028 2929 290a 2020 2020  toolTip())).    
-0000c920: 2020 2020 2020 2020 7265 7475 726e 0a20          return. 
-0000c930: 2020 2020 2020 2069 6620 7365 6c66 2e63         if self.c
-0000c940: 773a 0a20 2020 2020 2020 2020 2020 2073  w:.            s
-0000c950: 656c 662e 6377 2e73 656e 6463 7728 7365  elf.cw.sendcw(se
-0000c960: 6c66 2e70 726f 6365 7373 5f6d 6163 726f  lf.process_macro
-0000c970: 2873 656c 662e 4632 2e74 6f6f 6c54 6970  (self.F2.toolTip
-0000c980: 2829 2929 0a0a 2020 2020 6465 6620 7365  ()))..    def se
-0000c990: 6e64 6633 2873 656c 6629 3a0a 2020 2020  ndf3(self):.    
-0000c9a0: 2020 2020 2222 2273 7475 6222 2222 0a20      """stub""". 
-0000c9b0: 2020 2020 2020 206c 6f67 6765 722e 6465         logger.de
-0000c9c0: 6275 6728 2246 3320 436c 6963 6b65 6422  bug("F3 Clicked"
-0000c9d0: 290a 2020 2020 2020 2020 6966 2073 656c  ).        if sel
-0000c9e0: 662e 7261 6469 6f5f 7374 6174 652e 6765  f.radio_state.ge
-0000c9f0: 7428 226d 6f64 6522 2920 696e 205b 224c  t("mode") in ["L
-0000ca00: 5342 222c 2022 5553 4222 2c20 2253 5342  SB", "USB", "SSB
-0000ca10: 225d 3a0a 2020 2020 2020 2020 2020 2020  "]:.            
-0000ca20: 7365 6c66 2e76 6f69 6365 5f73 7472 696e  self.voice_strin
-0000ca30: 6728 7365 6c66 2e70 726f 6365 7373 5f6d  g(self.process_m
-0000ca40: 6163 726f 2873 656c 662e 4633 2e74 6f6f  acro(self.F3.too
-0000ca50: 6c54 6970 2829 2929 0a20 2020 2020 2020  lTip())).       
-0000ca60: 2020 2020 2072 6574 7572 6e0a 2020 2020       return.    
-0000ca70: 2020 2020 6966 2073 656c 662e 6377 3a0a      if self.cw:.
-0000ca80: 2020 2020 2020 2020 2020 2020 7365 6c66              self
-0000ca90: 2e63 772e 7365 6e64 6377 2873 656c 662e  .cw.sendcw(self.
-0000caa0: 7072 6f63 6573 735f 6d61 6372 6f28 7365  process_macro(se
-0000cab0: 6c66 2e46 332e 746f 6f6c 5469 7028 2929  lf.F3.toolTip())
-0000cac0: 290a 0a20 2020 2064 6566 2073 656e 6466  )..    def sendf
-0000cad0: 3428 7365 6c66 293a 0a20 2020 2020 2020  4(self):.       
-0000cae0: 2022 2222 7374 7562 2222 220a 2020 2020   """stub""".    
-0000caf0: 2020 2020 6c6f 6767 6572 2e64 6562 7567      logger.debug
-0000cb00: 2822 4634 2043 6c69 636b 6564 2229 0a20  ("F4 Clicked"). 
-0000cb10: 2020 2020 2020 2069 6620 7365 6c66 2e72         if self.r
-0000cb20: 6164 696f 5f73 7461 7465 2e67 6574 2822  adio_state.get("
-0000cb30: 6d6f 6465 2229 2069 6e20 5b22 4c53 4222  mode") in ["LSB"
-0000cb40: 2c20 2255 5342 222c 2022 5353 4222 5d3a  , "USB", "SSB"]:
-0000cb50: 0a20 2020 2020 2020 2020 2020 2073 656c  .            sel
-0000cb60: 662e 766f 6963 655f 7374 7269 6e67 2873  f.voice_string(s
-0000cb70: 656c 662e 7072 6f63 6573 735f 6d61 6372  elf.process_macr
-0000cb80: 6f28 7365 6c66 2e46 342e 746f 6f6c 5469  o(self.F4.toolTi
-0000cb90: 7028 2929 290a 2020 2020 2020 2020 2020  p())).          
-0000cba0: 2020 7265 7475 726e 0a20 2020 2020 2020    return.       
-0000cbb0: 2069 6620 7365 6c66 2e63 773a 0a20 2020   if self.cw:.   
-0000cbc0: 2020 2020 2020 2020 2073 656c 662e 6377           self.cw
-0000cbd0: 2e73 656e 6463 7728 7365 6c66 2e70 726f  .sendcw(self.pro
-0000cbe0: 6365 7373 5f6d 6163 726f 2873 656c 662e  cess_macro(self.
-0000cbf0: 4634 2e74 6f6f 6c54 6970 2829 2929 0a0a  F4.toolTip()))..
-0000cc00: 2020 2020 6465 6620 7365 6e64 6635 2873      def sendf5(s
-0000cc10: 656c 6629 3a0a 2020 2020 2020 2020 2222  elf):.        ""
-0000cc20: 2273 7475 6222 2222 0a20 2020 2020 2020  "stub""".       
-0000cc30: 206c 6f67 6765 722e 6465 6275 6728 2246   logger.debug("F
-0000cc40: 3520 436c 6963 6b65 6422 290a 2020 2020  5 Clicked").    
-0000cc50: 2020 2020 6966 2073 656c 662e 7261 6469      if self.radi
-0000cc60: 6f5f 7374 6174 652e 6765 7428 226d 6f64  o_state.get("mod
-0000cc70: 6522 2920 696e 205b 224c 5342 222c 2022  e") in ["LSB", "
-0000cc80: 5553 4222 2c20 2253 5342 225d 3a0a 2020  USB", "SSB"]:.  
-0000cc90: 2020 2020 2020 2020 2020 7365 6c66 2e76            self.v
-0000cca0: 6f69 6365 5f73 7472 696e 6728 7365 6c66  oice_string(self
-0000ccb0: 2e70 726f 6365 7373 5f6d 6163 726f 2873  .process_macro(s
-0000ccc0: 656c 662e 4635 2e74 6f6f 6c54 6970 2829  elf.F5.toolTip()
-0000ccd0: 2929 0a20 2020 2020 2020 2020 2020 2072  )).            r
-0000cce0: 6574 7572 6e0a 2020 2020 2020 2020 6966  eturn.        if
-0000ccf0: 2073 656c 662e 6377 3a0a 2020 2020 2020   self.cw:.      
-0000cd00: 2020 2020 2020 7365 6c66 2e63 772e 7365        self.cw.se
-0000cd10: 6e64 6377 2873 656c 662e 7072 6f63 6573  ndcw(self.proces
-0000cd20: 735f 6d61 6372 6f28 7365 6c66 2e46 352e  s_macro(self.F5.
-0000cd30: 746f 6f6c 5469 7028 2929 290a 0a20 2020  toolTip()))..   
-0000cd40: 2064 6566 2073 656e 6466 3628 7365 6c66   def sendf6(self
-0000cd50: 293a 0a20 2020 2020 2020 2022 2222 7374  ):.        """st
-0000cd60: 7562 2222 220a 2020 2020 2020 2020 6c6f  ub""".        lo
-0000cd70: 6767 6572 2e64 6562 7567 2822 4636 2043  gger.debug("F6 C
-0000cd80: 6c69 636b 6564 2229 0a20 2020 2020 2020  licked").       
-0000cd90: 2069 6620 7365 6c66 2e72 6164 696f 5f73   if self.radio_s
-0000cda0: 7461 7465 2e67 6574 2822 6d6f 6465 2229  tate.get("mode")
-0000cdb0: 2069 6e20 5b22 4c53 4222 2c20 2255 5342   in ["LSB", "USB
-0000cdc0: 222c 2022 5353 4222 5d3a 0a20 2020 2020  ", "SSB"]:.     
-0000cdd0: 2020 2020 2020 2073 656c 662e 766f 6963         self.voic
-0000cde0: 655f 7374 7269 6e67 2873 656c 662e 7072  e_string(self.pr
-0000cdf0: 6f63 6573 735f 6d61 6372 6f28 7365 6c66  ocess_macro(self
-0000ce00: 2e46 362e 746f 6f6c 5469 7028 2929 290a  .F6.toolTip())).
-0000ce10: 2020 2020 2020 2020 2020 2020 7265 7475              retu
-0000ce20: 726e 0a20 2020 2020 2020 2069 6620 7365  rn.        if se
-0000ce30: 6c66 2e63 773a 0a20 2020 2020 2020 2020  lf.cw:.         
-0000ce40: 2020 2073 656c 662e 6377 2e73 656e 6463     self.cw.sendc
-0000ce50: 7728 7365 6c66 2e70 726f 6365 7373 5f6d  w(self.process_m
-0000ce60: 6163 726f 2873 656c 662e 4636 2e74 6f6f  acro(self.F6.too
-0000ce70: 6c54 6970 2829 2929 0a0a 2020 2020 6465  lTip()))..    de
-0000ce80: 6620 7365 6e64 6637 2873 656c 6629 3a0a  f sendf7(self):.
-0000ce90: 2020 2020 2020 2020 2222 2273 7475 6222          """stub"
-0000cea0: 2222 0a20 2020 2020 2020 206c 6f67 6765  "".        logge
-0000ceb0: 722e 6465 6275 6728 2246 3720 436c 6963  r.debug("F7 Clic
-0000cec0: 6b65 6422 290a 2020 2020 2020 2020 6966  ked").        if
-0000ced0: 2073 656c 662e 7261 6469 6f5f 7374 6174   self.radio_stat
-0000cee0: 652e 6765 7428 226d 6f64 6522 2920 696e  e.get("mode") in
-0000cef0: 205b 224c 5342 222c 2022 5553 4222 2c20   ["LSB", "USB", 
-0000cf00: 2253 5342 225d 3a0a 2020 2020 2020 2020  "SSB"]:.        
-0000cf10: 2020 2020 7365 6c66 2e76 6f69 6365 5f73      self.voice_s
-0000cf20: 7472 696e 6728 7365 6c66 2e70 726f 6365  tring(self.proce
-0000cf30: 7373 5f6d 6163 726f 2873 656c 662e 4637  ss_macro(self.F7
-0000cf40: 2e74 6f6f 6c54 6970 2829 2929 0a20 2020  .toolTip())).   
-0000cf50: 2020 2020 2020 2020 2072 6574 7572 6e0a           return.
-0000cf60: 2020 2020 2020 2020 6966 2073 656c 662e          if self.
-0000cf70: 6377 3a0a 2020 2020 2020 2020 2020 2020  cw:.            
-0000cf80: 7365 6c66 2e63 772e 7365 6e64 6377 2873  self.cw.sendcw(s
-0000cf90: 656c 662e 7072 6f63 6573 735f 6d61 6372  elf.process_macr
-0000cfa0: 6f28 7365 6c66 2e46 372e 746f 6f6c 5469  o(self.F7.toolTi
-0000cfb0: 7028 2929 290a 0a20 2020 2064 6566 2073  p()))..    def s
-0000cfc0: 656e 6466 3828 7365 6c66 293a 0a20 2020  endf8(self):.   
-0000cfd0: 2020 2020 2022 2222 7374 7562 2222 220a       """stub""".
-0000cfe0: 2020 2020 2020 2020 6c6f 6767 6572 2e64          logger.d
-0000cff0: 6562 7567 2822 4638 2043 6c69 636b 6564  ebug("F8 Clicked
-0000d000: 2229 0a20 2020 2020 2020 2069 6620 7365  ").        if se
-0000d010: 6c66 2e72 6164 696f 5f73 7461 7465 2e67  lf.radio_state.g
-0000d020: 6574 2822 6d6f 6465 2229 2069 6e20 5b22  et("mode") in ["
-0000d030: 4c53 4222 2c20 2255 5342 222c 2022 5353  LSB", "USB", "SS
-0000d040: 4222 5d3a 0a20 2020 2020 2020 2020 2020  B"]:.           
-0000d050: 2073 656c 662e 766f 6963 655f 7374 7269   self.voice_stri
-0000d060: 6e67 2873 656c 662e 7072 6f63 6573 735f  ng(self.process_
-0000d070: 6d61 6372 6f28 7365 6c66 2e46 382e 746f  macro(self.F8.to
-0000d080: 6f6c 5469 7028 2929 290a 2020 2020 2020  olTip())).      
-0000d090: 2020 2020 2020 7265 7475 726e 0a20 2020        return.   
-0000d0a0: 2020 2020 2069 6620 7365 6c66 2e63 773a       if self.cw:
-0000d0b0: 0a20 2020 2020 2020 2020 2020 2073 656c  .            sel
-0000d0c0: 662e 6377 2e73 656e 6463 7728 7365 6c66  f.cw.sendcw(self
-0000d0d0: 2e70 726f 6365 7373 5f6d 6163 726f 2873  .process_macro(s
-0000d0e0: 656c 662e 4638 2e74 6f6f 6c54 6970 2829  elf.F8.toolTip()
-0000d0f0: 2929 0a0a 2020 2020 6465 6620 7365 6e64  ))..    def send
-0000d100: 6639 2873 656c 6629 3a0a 2020 2020 2020  f9(self):.      
-0000d110: 2020 2222 2273 7475 6222 2222 0a20 2020    """stub""".   
-0000d120: 2020 2020 206c 6f67 6765 722e 6465 6275       logger.debu
-0000d130: 6728 2246 3920 436c 6963 6b65 6422 290a  g("F9 Clicked").
-0000d140: 2020 2020 2020 2020 6966 2073 656c 662e          if self.
-0000d150: 7261 6469 6f5f 7374 6174 652e 6765 7428  radio_state.get(
-0000d160: 226d 6f64 6522 2920 696e 205b 224c 5342  "mode") in ["LSB
-0000d170: 222c 2022 5553 4222 2c20 2253 5342 225d  ", "USB", "SSB"]
-0000d180: 3a0a 2020 2020 2020 2020 2020 2020 7365  :.            se
-0000d190: 6c66 2e76 6f69 6365 5f73 7472 696e 6728  lf.voice_string(
-0000d1a0: 7365 6c66 2e70 726f 6365 7373 5f6d 6163  self.process_mac
-0000d1b0: 726f 2873 656c 662e 4639 2e74 6f6f 6c54  ro(self.F9.toolT
-0000d1c0: 6970 2829 2929 0a20 2020 2020 2020 2020  ip())).         
-0000d1d0: 2020 2072 6574 7572 6e0a 2020 2020 2020     return.      
-0000d1e0: 2020 6966 2073 656c 662e 6377 3a0a 2020    if self.cw:.  
-0000d1f0: 2020 2020 2020 2020 2020 7365 6c66 2e63            self.c
-0000d200: 772e 7365 6e64 6377 2873 656c 662e 7072  w.sendcw(self.pr
-0000d210: 6f63 6573 735f 6d61 6372 6f28 7365 6c66  ocess_macro(self
-0000d220: 2e46 392e 746f 6f6c 5469 7028 2929 290a  .F9.toolTip())).
-0000d230: 0a20 2020 2064 6566 2073 656e 6466 3130  .    def sendf10
-0000d240: 2873 656c 6629 3a0a 2020 2020 2020 2020  (self):.        
-0000d250: 2222 2273 7475 6222 2222 0a20 2020 2020  """stub""".     
-0000d260: 2020 206c 6f67 6765 722e 6465 6275 6728     logger.debug(
-0000d270: 2246 3130 2043 6c69 636b 6564 2229 0a20  "F10 Clicked"). 
-0000d280: 2020 2020 2020 2069 6620 7365 6c66 2e72         if self.r
-0000d290: 6164 696f 5f73 7461 7465 2e67 6574 2822  adio_state.get("
-0000d2a0: 6d6f 6465 2229 2069 6e20 5b22 4c53 4222  mode") in ["LSB"
-0000d2b0: 2c20 2255 5342 222c 2022 5353 4222 5d3a  , "USB", "SSB"]:
-0000d2c0: 0a20 2020 2020 2020 2020 2020 2073 656c  .            sel
-0000d2d0: 662e 766f 6963 655f 7374 7269 6e67 2873  f.voice_string(s
-0000d2e0: 656c 662e 7072 6f63 6573 735f 6d61 6372  elf.process_macr
-0000d2f0: 6f28 7365 6c66 2e46 3130 2e74 6f6f 6c54  o(self.F10.toolT
-0000d300: 6970 2829 2929 0a20 2020 2020 2020 2020  ip())).         
-0000d310: 2020 2072 6574 7572 6e0a 2020 2020 2020     return.      
-0000d320: 2020 6966 2073 656c 662e 6377 3a0a 2020    if self.cw:.  
-0000d330: 2020 2020 2020 2020 2020 7365 6c66 2e63            self.c
-0000d340: 772e 7365 6e64 6377 2873 656c 662e 7072  w.sendcw(self.pr
-0000d350: 6f63 6573 735f 6d61 6372 6f28 7365 6c66  ocess_macro(self
-0000d360: 2e46 3130 2e74 6f6f 6c54 6970 2829 2929  .F10.toolTip()))
-0000d370: 0a0a 2020 2020 6465 6620 7365 6e64 6631  ..    def sendf1
-0000d380: 3128 7365 6c66 293a 0a20 2020 2020 2020  1(self):.       
-0000d390: 2022 2222 7374 7562 2222 220a 2020 2020   """stub""".    
-0000d3a0: 2020 2020 6c6f 6767 6572 2e64 6562 7567      logger.debug
-0000d3b0: 2822 4631 3120 436c 6963 6b65 6422 290a  ("F11 Clicked").
-0000d3c0: 2020 2020 2020 2020 6966 2073 656c 662e          if self.
-0000d3d0: 7261 6469 6f5f 7374 6174 652e 6765 7428  radio_state.get(
-0000d3e0: 226d 6f64 6522 2920 696e 205b 224c 5342  "mode") in ["LSB
-0000d3f0: 222c 2022 5553 4222 2c20 2253 5342 225d  ", "USB", "SSB"]
-0000d400: 3a0a 2020 2020 2020 2020 2020 2020 7365  :.            se
-0000d410: 6c66 2e76 6f69 6365 5f73 7472 696e 6728  lf.voice_string(
-0000d420: 7365 6c66 2e70 726f 6365 7373 5f6d 6163  self.process_mac
-0000d430: 726f 2873 656c 662e 4631 312e 746f 6f6c  ro(self.F11.tool
-0000d440: 5469 7028 2929 290a 2020 2020 2020 2020  Tip())).        
-0000d450: 2020 2020 7265 7475 726e 0a20 2020 2020      return.     
-0000d460: 2020 2069 6620 7365 6c66 2e63 773a 0a20     if self.cw:. 
-0000d470: 2020 2020 2020 2020 2020 2073 656c 662e             self.
-0000d480: 6377 2e73 656e 6463 7728 7365 6c66 2e70  cw.sendcw(self.p
-0000d490: 726f 6365 7373 5f6d 6163 726f 2873 656c  rocess_macro(sel
-0000d4a0: 662e 4631 312e 746f 6f6c 5469 7028 2929  f.F11.toolTip())
-0000d4b0: 290a 0a20 2020 2064 6566 2073 656e 6466  )..    def sendf
-0000d4c0: 3132 2873 656c 6629 3a0a 2020 2020 2020  12(self):.      
-0000d4d0: 2020 2222 2273 7475 6222 2222 0a20 2020    """stub""".   
-0000d4e0: 2020 2020 206c 6f67 6765 722e 6465 6275       logger.debu
-0000d4f0: 6728 2246 3132 2043 6c69 636b 6564 2229  g("F12 Clicked")
-0000d500: 0a20 2020 2020 2020 2069 6620 7365 6c66  .        if self
-0000d510: 2e72 6164 696f 5f73 7461 7465 2e67 6574  .radio_state.get
-0000d520: 2822 6d6f 6465 2229 2069 6e20 5b22 4c53  ("mode") in ["LS
-0000d530: 4222 2c20 2255 5342 222c 2022 5353 4222  B", "USB", "SSB"
-0000d540: 5d3a 0a20 2020 2020 2020 2020 2020 2073  ]:.            s
-0000d550: 656c 662e 766f 6963 655f 7374 7269 6e67  elf.voice_string
-0000d560: 2873 656c 662e 7072 6f63 6573 735f 6d61  (self.process_ma
-0000d570: 6372 6f28 7365 6c66 2e46 3132 2e74 6f6f  cro(self.F12.too
-0000d580: 6c54 6970 2829 2929 0a20 2020 2020 2020  lTip())).       
-0000d590: 2020 2020 2072 6574 7572 6e0a 2020 2020       return.    
-0000d5a0: 2020 2020 6966 2073 656c 662e 6377 3a0a      if self.cw:.
-0000d5b0: 2020 2020 2020 2020 2020 2020 7365 6c66              self
-0000d5c0: 2e63 772e 7365 6e64 6377 2873 656c 662e  .cw.sendcw(self.
-0000d5d0: 7072 6f63 6573 735f 6d61 6372 6f28 7365  process_macro(se
-0000d5e0: 6c66 2e46 3132 2e74 6f6f 6c54 6970 2829  lf.F12.toolTip()
-0000d5f0: 2929 0a0a 2020 2020 6465 6620 7275 6e5f  ))..    def run_
-0000d600: 7370 5f62 7574 746f 6e73 5f63 6c69 636b  sp_buttons_click
-0000d610: 6564 2873 656c 6629 3a0a 2020 2020 2020  ed(self):.      
-0000d620: 2020 2222 2248 616e 646c 6520 7275 6e2f    """Handle run/
-0000d630: 7326 7020 6d6f 6465 2222 220a 2020 2020  s&p mode""".    
-0000d640: 2020 2020 7365 6c66 2e70 7265 665b 2272      self.pref["r
-0000d650: 756e 5f73 7461 7465 225d 203d 2073 656c  un_state"] = sel
-0000d660: 662e 7261 6469 6f42 7574 746f 6e5f 7275  f.radioButton_ru
-0000d670: 6e2e 6973 4368 6563 6b65 6428 290a 2020  n.isChecked().  
-0000d680: 2020 2020 2020 7365 6c66 2e77 7269 7465        self.write
-0000d690: 5f70 7265 6665 7265 6e63 6528 290a 2020  _preference().  
-0000d6a0: 2020 2020 2020 7365 6c66 2e72 6561 645f        self.read_
-0000d6b0: 6377 5f6d 6163 726f 7328 290a 0a20 2020  cw_macros()..   
-0000d6c0: 2064 6566 2077 7269 7465 5f70 7265 6665   def write_prefe
-0000d6d0: 7265 6e63 6528 7365 6c66 293a 0a20 2020  rence(self):.   
-0000d6e0: 2020 2020 2022 2222 0a20 2020 2020 2020       """.       
-0000d6f0: 2057 7269 7465 2070 7265 6665 7265 6e63   Write preferenc
-0000d700: 6573 2074 6f20 6a73 6f6e 2066 696c 652e  es to json file.
-0000d710: 0a20 2020 2020 2020 2022 2222 0a20 2020  .        """.   
-0000d720: 2020 2020 2074 7279 3a0a 2020 2020 2020       try:.      
-0000d730: 2020 2020 2020 7769 7468 206f 7065 6e28        with open(
-0000d740: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-0000d750: 2043 4f4e 4649 475f 5041 5448 202b 2022   CONFIG_PATH + "
-0000d760: 2f6e 6f74 316d 6d2e 6a73 6f6e 222c 2022  /not1mm.json", "
-0000d770: 7774 222c 2065 6e63 6f64 696e 673d 2275  wt", encoding="u
-0000d780: 7466 2d38 220a 2020 2020 2020 2020 2020  tf-8".          
-0000d790: 2020 2920 6173 2066 696c 655f 6465 7363    ) as file_desc
-0000d7a0: 7269 7074 6f72 3a0a 2020 2020 2020 2020  riptor:.        
-0000d7b0: 2020 2020 2020 2020 6669 6c65 5f64 6573          file_des
-0000d7c0: 6372 6970 746f 722e 7772 6974 6528 6475  criptor.write(du
-0000d7d0: 6d70 7328 7365 6c66 2e70 7265 662c 2069  mps(self.pref, i
-0000d7e0: 6e64 656e 743d 3429 290a 2020 2020 2020  ndent=4)).      
-0000d7f0: 2020 2020 2020 2020 2020 6c6f 6767 6572            logger
-0000d800: 2e69 6e66 6f28 2277 7269 7469 6e67 3a20  .info("writing: 
-0000d810: 2573 222c 2073 656c 662e 7072 6566 290a  %s", self.pref).
-0000d820: 2020 2020 2020 2020 6578 6365 7074 2049          except I
-0000d830: 4f45 7272 6f72 2061 7320 6578 6365 7074  OError as except
-0000d840: 696f 6e3a 0a20 2020 2020 2020 2020 2020  ion:.           
-0000d850: 206c 6f67 6765 722e 6372 6974 6963 616c   logger.critical
-0000d860: 2822 7772 6974 6570 7265 6665 7265 6e63  ("writepreferenc
-0000d870: 6573 3a20 2573 222c 2065 7863 6570 7469  es: %s", excepti
-0000d880: 6f6e 290a 0a20 2020 2064 6566 2072 6561  on)..    def rea
-0000d890: 6470 7265 6665 7265 6e63 6573 2873 656c  dpreferences(sel
-0000d8a0: 6629 3a0a 2020 2020 2020 2020 2222 220a  f):.        """.
-0000d8b0: 2020 2020 2020 2020 5265 7374 6f72 6520          Restore 
-0000d8c0: 7072 6566 6572 656e 6365 7320 6966 2074  preferences if t
-0000d8d0: 6865 7920 6578 6973 742c 206f 7468 6572  hey exist, other
-0000d8e0: 7769 7365 2063 7265 6174 6520 736f 6d65  wise create some
-0000d8f0: 2073 616e 6520 6465 6661 756c 7473 2e0a   sane defaults..
-0000d900: 2020 2020 2020 2020 2222 220a 2020 2020          """.    
-0000d910: 2020 2020 7472 793a 0a20 2020 2020 2020      try:.       
-0000d920: 2020 2020 2069 6620 6f73 2e70 6174 682e       if os.path.
-0000d930: 6578 6973 7473 2843 4f4e 4649 475f 5041  exists(CONFIG_PA
-0000d940: 5448 202b 2022 2f6e 6f74 316d 6d2e 6a73  TH + "/not1mm.js
-0000d950: 6f6e 2229 3a0a 2020 2020 2020 2020 2020  on"):.          
-0000d960: 2020 2020 2020 7769 7468 206f 7065 6e28        with open(
-0000d970: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-0000d980: 2020 2020 2043 4f4e 4649 475f 5041 5448       CONFIG_PATH
-0000d990: 202b 2022 2f6e 6f74 316d 6d2e 6a73 6f6e   + "/not1mm.json
-0000d9a0: 222c 2022 7274 222c 2065 6e63 6f64 696e  ", "rt", encodin
-0000d9b0: 673d 2275 7466 2d38 220a 2020 2020 2020  g="utf-8".      
-0000d9c0: 2020 2020 2020 2020 2020 2920 6173 2066            ) as f
-0000d9d0: 696c 655f 6465 7363 7269 7074 6f72 3a0a  ile_descriptor:.
-0000d9e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000d9f0: 2020 2020 7365 6c66 2e70 7265 6620 3d20      self.pref = 
-0000da00: 6c6f 6164 7328 6669 6c65 5f64 6573 6372  loads(file_descr
-0000da10: 6970 746f 722e 7265 6164 2829 290a 2020  iptor.read()).  
-0000da20: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000da30: 2020 6c6f 6767 6572 2e69 6e66 6f28 2225    logger.info("%
-0000da40: 7322 2c20 7365 6c66 2e70 7265 6629 0a20  s", self.pref). 
-0000da50: 2020 2020 2020 2020 2020 2065 6c73 653a             else:
-0000da60: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-0000da70: 206c 6f67 6765 722e 696e 666f 2822 4e6f   logger.info("No
-0000da80: 2070 7265 6665 7265 6e63 6520 6669 6c65   preference file
-0000da90: 2e20 5772 6974 696e 6720 7072 6566 6572  . Writing prefer
-0000daa0: 656e 6365 2e22 290a 2020 2020 2020 2020  ence.").        
-0000dab0: 2020 2020 2020 2020 7769 7468 206f 7065          with ope
-0000dac0: 6e28 0a20 2020 2020 2020 2020 2020 2020  n(.             
-0000dad0: 2020 2020 2020 2043 4f4e 4649 475f 5041         CONFIG_PA
-0000dae0: 5448 202b 2022 2f6e 6f74 316d 6d2e 6a73  TH + "/not1mm.js
-0000daf0: 6f6e 222c 2022 7774 222c 2065 6e63 6f64  on", "wt", encod
-0000db00: 696e 673d 2275 7466 2d38 220a 2020 2020  ing="utf-8".    
-0000db10: 2020 2020 2020 2020 2020 2020 2920 6173              ) as
-0000db20: 2066 696c 655f 6465 7363 7269 7074 6f72   file_descriptor
-0000db30: 3a0a 2020 2020 2020 2020 2020 2020 2020  :.              
-0000db40: 2020 2020 2020 7365 6c66 2e70 7265 6620        self.pref 
-0000db50: 3d20 7365 6c66 2e70 7265 665f 7265 662e  = self.pref_ref.
-0000db60: 636f 7079 2829 0a20 2020 2020 2020 2020  copy().         
-0000db70: 2020 2020 2020 2020 2020 2066 696c 655f             file_
-0000db80: 6465 7363 7269 7074 6f72 2e77 7269 7465  descriptor.write
-0000db90: 2864 756d 7073 2873 656c 662e 7072 6566  (dumps(self.pref
-0000dba0: 2c20 696e 6465 6e74 3d34 2929 0a20 2020  , indent=4)).   
-0000dbb0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000dbc0: 206c 6f67 6765 722e 696e 666f 2822 2573   logger.info("%s
-0000dbd0: 222c 2073 656c 662e 7072 6566 290a 2020  ", self.pref).  
-0000dbe0: 2020 2020 2020 6578 6365 7074 2049 4f45        except IOE
-0000dbf0: 7272 6f72 2061 7320 6578 6365 7074 696f  rror as exceptio
-0000dc00: 6e3a 0a20 2020 2020 2020 2020 2020 206c  n:.            l
-0000dc10: 6f67 6765 722e 6372 6974 6963 616c 2822  ogger.critical("
-0000dc20: 4572 726f 723a 2025 7322 2c20 6578 6365  Error: %s", exce
-0000dc30: 7074 696f 6e29 0a0a 2020 2020 2020 2020  ption)..        
-0000dc40: 7365 6c66 2e6c 6f6f 6b5f 7570 203d 204e  self.look_up = N
-0000dc50: 6f6e 650a 2020 2020 2020 2020 6966 2073  one.        if s
-0000dc60: 656c 662e 7072 6566 2e67 6574 2822 7573  elf.pref.get("us
-0000dc70: 6571 727a 2229 3a0a 2020 2020 2020 2020  eqrz"):.        
-0000dc80: 2020 2020 7365 6c66 2e6c 6f6f 6b5f 7570      self.look_up
-0000dc90: 203d 2051 525a 6c6f 6f6b 7570 280a 2020   = QRZlookup(.  
-0000dca0: 2020 2020 2020 2020 2020 2020 2020 7365                se
-0000dcb0: 6c66 2e70 7265 662e 6765 7428 226c 6f6f  lf.pref.get("loo
-0000dcc0: 6b75 7075 7365 726e 616d 6522 292c 0a20  kupusername"),. 
-0000dcd0: 2020 2020 2020 2020 2020 2020 2020 2073                 s
-0000dce0: 656c 662e 7072 6566 2e67 6574 2822 6c6f  elf.pref.get("lo
-0000dcf0: 6f6b 7570 7061 7373 776f 7264 2229 2c0a  okuppassword"),.
-0000dd00: 2020 2020 2020 2020 2020 2020 290a 2020              ).  
-0000dd10: 2020 2020 2020 2320 6966 2073 656c 662e        # if self.
-0000dd20: 7072 6566 2e67 6574 2822 7573 6568 616d  pref.get("useham
-0000dd30: 6462 2229 3a0a 2020 2020 2020 2020 2320  db"):.        # 
-0000dd40: 2020 2020 7365 6c66 2e6c 6f6f 6b5f 7570      self.look_up
-0000dd50: 203d 2048 616d 4442 6c6f 6f6b 7570 2829   = HamDBlookup()
-0000dd60: 0a20 2020 2020 2020 2069 6620 7365 6c66  .        if self
-0000dd70: 2e70 7265 662e 6765 7428 2275 7365 6861  .pref.get("useha
-0000dd80: 6d71 7468 2229 3a0a 2020 2020 2020 2020  mqth"):.        
-0000dd90: 2020 2020 7365 6c66 2e6c 6f6f 6b5f 7570      self.look_up
-0000dda0: 203d 2048 616d 5154 4828 0a20 2020 2020   = HamQTH(.     
-0000ddb0: 2020 2020 2020 2020 2020 2073 656c 662e             self.
-0000ddc0: 7072 6566 2e67 6574 2822 6c6f 6f6b 7570  pref.get("lookup
-0000ddd0: 7573 6572 6e61 6d65 2229 2c0a 2020 2020  username"),.    
-0000dde0: 2020 2020 2020 2020 2020 2020 7365 6c66              self
-0000ddf0: 2e70 7265 662e 6765 7428 226c 6f6f 6b75  .pref.get("looku
-0000de00: 7070 6173 7377 6f72 6422 292c 0a20 2020  ppassword"),.   
-0000de10: 2020 2020 2020 2020 2029 0a0a 2020 2020           )..    
-0000de20: 2020 2020 6966 2073 656c 662e 7072 6566      if self.pref
-0000de30: 2e67 6574 2822 7275 6e5f 7374 6174 6522  .get("run_state"
-0000de40: 293a 0a20 2020 2020 2020 2020 2020 2073  ):.            s
-0000de50: 656c 662e 7261 6469 6f42 7574 746f 6e5f  elf.radioButton_
-0000de60: 7275 6e2e 7365 7443 6865 636b 6564 2854  run.setChecked(T
-0000de70: 7275 6529 0a20 2020 2020 2020 2065 6c73  rue).        els
-0000de80: 653a 0a20 2020 2020 2020 2020 2020 2073  e:.            s
-0000de90: 656c 662e 7261 6469 6f42 7574 746f 6e5f  elf.radioButton_
-0000dea0: 7370 2e73 6574 4368 6563 6b65 6428 5472  sp.setChecked(Tr
-0000deb0: 7565 290a 0a20 2020 2020 2020 2069 6620  ue)..        if 
-0000dec0: 7365 6c66 2e70 7265 662e 6765 7428 2264  self.pref.get("d
-0000ded0: 6172 6b5f 6d6f 6465 2229 3a0a 2020 2020  ark_mode"):.    
-0000dee0: 2020 2020 2020 2020 7365 6c66 2e61 6374          self.act
-0000def0: 696f 6e44 6172 6b5f 4d6f 6465 2e73 6574  ionDark_Mode.set
-0000df00: 4368 6563 6b65 6428 5472 7565 290a 2020  Checked(True).  
-0000df10: 2020 2020 2020 656c 7365 3a0a 2020 2020        else:.    
-0000df20: 2020 2020 2020 2020 7365 6c66 2e61 6374          self.act
-0000df30: 696f 6e44 6172 6b5f 4d6f 6465 2e73 6574  ionDark_Mode.set
-0000df40: 4368 6563 6b65 6428 4661 6c73 6529 0a0a  Checked(False)..
-0000df50: 2020 2020 2020 2020 6966 2073 656c 662e          if self.
-0000df60: 7072 6566 2e67 6574 2822 636f 6d6d 616e  pref.get("comman
-0000df70: 645f 6275 7474 6f6e 7322 293a 0a20 2020  d_buttons"):.   
-0000df80: 2020 2020 2020 2020 2073 656c 662e 6163           self.ac
-0000df90: 7469 6f6e 436f 6d6d 616e 645f 4275 7474  tionCommand_Butt
-0000dfa0: 6f6e 732e 7365 7443 6865 636b 6564 2854  ons.setChecked(T
-0000dfb0: 7275 6529 0a20 2020 2020 2020 2065 6c73  rue).        els
-0000dfc0: 653a 0a20 2020 2020 2020 2020 2020 2073  e:.            s
-0000dfd0: 656c 662e 6163 7469 6f6e 436f 6d6d 616e  elf.actionComman
-0000dfe0: 645f 4275 7474 6f6e 732e 7365 7443 6865  d_Buttons.setChe
-0000dff0: 636b 6564 2846 616c 7365 290a 0a20 2020  cked(False)..   
-0000e000: 2020 2020 2069 6620 7365 6c66 2e70 7265       if self.pre
-0000e010: 662e 6765 7428 2263 775f 6d61 6372 6f73  f.get("cw_macros
-0000e020: 2229 3a0a 2020 2020 2020 2020 2020 2020  "):.            
-0000e030: 7365 6c66 2e61 6374 696f 6e43 575f 4d61  self.actionCW_Ma
-0000e040: 6372 6f73 2e73 6574 4368 6563 6b65 6428  cros.setChecked(
-0000e050: 5472 7565 290a 2020 2020 2020 2020 656c  True).        el
-0000e060: 7365 3a0a 2020 2020 2020 2020 2020 2020  se:.            
-0000e070: 7365 6c66 2e61 6374 696f 6e43 575f 4d61  self.actionCW_Ma
-0000e080: 6372 6f73 2e73 6574 4368 6563 6b65 6428  cros.setChecked(
-0000e090: 4661 6c73 6529 0a0a 2020 2020 2020 2020  False)..        
-0000e0a0: 6966 2073 656c 662e 7072 6566 2e67 6574  if self.pref.get
-0000e0b0: 2822 6261 6e64 735f 6d6f 6465 7322 293a  ("bands_modes"):
-0000e0c0: 0a20 2020 2020 2020 2020 2020 2073 656c  .            sel
-0000e0d0: 662e 6163 7469 6f6e 4d6f 6465 5f61 6e64  f.actionMode_and
-0000e0e0: 5f42 616e 6473 2e73 6574 4368 6563 6b65  _Bands.setChecke
-0000e0f0: 6428 5472 7565 290a 2020 2020 2020 2020  d(True).        
-0000e100: 656c 7365 3a0a 2020 2020 2020 2020 2020  else:.          
-0000e110: 2020 7365 6c66 2e61 6374 696f 6e4d 6f64    self.actionMod
-0000e120: 655f 616e 645f 4261 6e64 732e 7365 7443  e_and_Bands.setC
-0000e130: 6865 636b 6564 2846 616c 7365 290a 0a20  hecked(False).. 
-0000e140: 2020 2020 2020 206d 756c 7469 6361 7374         multicast
-0000e150: 5f67 726f 7570 203d 2073 656c 662e 7072  _group = self.pr
-0000e160: 6566 2e67 6574 2822 6d75 6c74 6963 6173  ef.get("multicas
-0000e170: 745f 6772 6f75 7022 2c20 2232 3234 2e31  t_group", "224.1
-0000e180: 2e31 2e31 2229 0a20 2020 2020 2020 206d  .1.1").        m
-0000e190: 756c 7469 6361 7374 5f70 6f72 7420 3d20  ulticast_port = 
-0000e1a0: 7365 6c66 2e70 7265 662e 6765 7428 226d  self.pref.get("m
-0000e1b0: 756c 7469 6361 7374 5f70 6f72 7422 2c20  ulticast_port", 
-0000e1c0: 3232 3339 290a 2020 2020 2020 2020 696e  2239).        in
-0000e1d0: 7465 7266 6163 655f 6970 203d 2073 656c  terface_ip = sel
-0000e1e0: 662e 7072 6566 2e67 6574 2822 696e 7465  f.pref.get("inte
-0000e1f0: 7266 6163 655f 6970 222c 2022 302e 302e  rface_ip", "0.0.
-0000e200: 302e 3022 290a 2020 2020 2020 2020 7365  0.0").        se
-0000e210: 6c66 2e6d 756c 7469 6361 7374 5f69 6e74  lf.multicast_int
-0000e220: 6572 6661 6365 203d 204d 756c 7469 6361  erface = Multica
-0000e230: 7374 280a 2020 2020 2020 2020 2020 2020  st(.            
-0000e240: 6d75 6c74 6963 6173 745f 6772 6f75 702c  multicast_group,
-0000e250: 206d 756c 7469 6361 7374 5f70 6f72 742c   multicast_port,
-0000e260: 2069 6e74 6572 6661 6365 5f69 700a 2020   interface_ip.  
-0000e270: 2020 2020 2020 290a 0a20 2020 2020 2020        )..       
-0000e280: 2073 656c 662e 7269 675f 636f 6e74 726f   self.rig_contro
-0000e290: 6c20 3d20 4e6f 6e65 0a0a 2020 2020 2020  l = None..      
-0000e2a0: 2020 6966 2073 656c 662e 7072 6566 2e67    if self.pref.g
-0000e2b0: 6574 2822 7573 6566 6c72 6967 222c 2046  et("useflrig", F
-0000e2c0: 616c 7365 293a 0a20 2020 2020 2020 2020  alse):.         
-0000e2d0: 2020 206c 6f67 6765 722e 6465 6275 6728     logger.debug(
-0000e2e0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-0000e2f0: 2022 5573 696e 6720 666c 7269 673a 2025   "Using flrig: %
-0000e300: 7322 2c0a 2020 2020 2020 2020 2020 2020  s",.            
-0000e310: 2020 2020 6622 7b73 656c 662e 7072 6566      f"{self.pref
-0000e320: 2e67 6574 2827 4341 545f 6970 2729 7d20  .get('CAT_ip')} 
-0000e330: 7b73 656c 662e 7072 6566 2e67 6574 2827  {self.pref.get('
-0000e340: 4341 545f 706f 7274 2729 7d22 2c0a 2020  CAT_port')}",.  
-0000e350: 2020 2020 2020 2020 2020 290a 2020 2020            ).    
-0000e360: 2020 2020 2020 2020 7365 6c66 2e72 6967          self.rig
-0000e370: 5f63 6f6e 7472 6f6c 203d 2043 4154 280a  _control = CAT(.
-0000e380: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000e390: 2266 6c72 6967 222c 0a20 2020 2020 2020  "flrig",.       
-0000e3a0: 2020 2020 2020 2020 2073 656c 662e 7072           self.pr
-0000e3b0: 6566 2e67 6574 2822 4341 545f 6970 222c  ef.get("CAT_ip",
-0000e3c0: 2022 3132 372e 302e 302e 3122 292c 0a20   "127.0.0.1"),. 
-0000e3d0: 2020 2020 2020 2020 2020 2020 2020 2069                 i
-0000e3e0: 6e74 2873 656c 662e 7072 6566 2e67 6574  nt(self.pref.get
-0000e3f0: 2822 4341 545f 706f 7274 222c 2031 3233  ("CAT_port", 123
-0000e400: 3435 2929 2c0a 2020 2020 2020 2020 2020  45)),.          
-0000e410: 2020 290a 2020 2020 2020 2020 6966 2073    ).        if s
-0000e420: 656c 662e 7072 6566 2e67 6574 2822 7573  elf.pref.get("us
-0000e430: 6572 6967 6374 6c64 222c 2046 616c 7365  erigctld", False
-0000e440: 293a 0a20 2020 2020 2020 2020 2020 206c  ):.            l
-0000e450: 6f67 6765 722e 6465 6275 6728 0a20 2020  ogger.debug(.   
-0000e460: 2020 2020 2020 2020 2020 2020 2022 5573               "Us
-0000e470: 696e 6720 7269 6763 746c 643a 2025 7322  ing rigctld: %s"
-0000e480: 2c0a 2020 2020 2020 2020 2020 2020 2020  ,.              
-0000e490: 2020 6622 7b73 656c 662e 7072 6566 2e67    f"{self.pref.g
-0000e4a0: 6574 2827 4341 545f 6970 2729 7d20 7b73  et('CAT_ip')} {s
-0000e4b0: 656c 662e 7072 6566 2e67 6574 2827 4341  elf.pref.get('CA
-0000e4c0: 545f 706f 7274 2729 7d22 2c0a 2020 2020  T_port')}",.    
-0000e4d0: 2020 2020 2020 2020 290a 2020 2020 2020          ).      
-0000e4e0: 2020 2020 2020 7365 6c66 2e72 6967 5f63        self.rig_c
-0000e4f0: 6f6e 7472 6f6c 203d 2043 4154 280a 2020  ontrol = CAT(.  
-0000e500: 2020 2020 2020 2020 2020 2020 2020 2272                "r
-0000e510: 6967 6374 6c64 222c 0a20 2020 2020 2020  igctld",.       
-0000e520: 2020 2020 2020 2020 2073 656c 662e 7072           self.pr
-0000e530: 6566 2e67 6574 2822 4341 545f 6970 222c  ef.get("CAT_ip",
-0000e540: 2022 3132 372e 302e 302e 3122 292c 0a20   "127.0.0.1"),. 
-0000e550: 2020 2020 2020 2020 2020 2020 2020 2069                 i
-0000e560: 6e74 2873 656c 662e 7072 6566 2e67 6574  nt(self.pref.get
-0000e570: 2822 4341 545f 706f 7274 222c 2034 3533  ("CAT_port", 453
-0000e580: 3229 292c 0a20 2020 2020 2020 2020 2020  2)),.           
-0000e590: 2029 0a0a 2020 2020 2020 2020 6966 2073   )..        if s
-0000e5a0: 656c 662e 7072 6566 2e67 6574 2822 6377  elf.pref.get("cw
-0000e5b0: 7479 7065 222c 2030 2920 3d3d 2030 3a0a  type", 0) == 0:.
-0000e5c0: 2020 2020 2020 2020 2020 2020 7365 6c66              self
-0000e5d0: 2e63 7720 3d20 4e6f 6e65 0a20 2020 2020  .cw = None.     
-0000e5e0: 2020 2065 6c73 653a 0a20 2020 2020 2020     else:.       
-0000e5f0: 2020 2020 2073 656c 662e 6377 203d 2043       self.cw = C
-0000e600: 5728 0a20 2020 2020 2020 2020 2020 2020  W(.             
-0000e610: 2020 2069 6e74 2873 656c 662e 7072 6566     int(self.pref
-0000e620: 2e67 6574 2822 6377 7479 7065 2229 292c  .get("cwtype")),
-0000e630: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-0000e640: 2073 656c 662e 7072 6566 2e67 6574 2822   self.pref.get("
-0000e650: 6377 6970 2229 2c0a 2020 2020 2020 2020  cwip"),.        
-0000e660: 2020 2020 2020 2020 696e 7428 7365 6c66          int(self
-0000e670: 2e70 7265 662e 6765 7428 2263 7770 6f72  .pref.get("cwpor
-0000e680: 7422 2c20 3637 3839 2929 2c0a 2020 2020  t", 6789)),.    
-0000e690: 2020 2020 2020 2020 290a 2020 2020 2020          ).      
-0000e6a0: 2020 2020 2020 7365 6c66 2e63 772e 7370        self.cw.sp
-0000e6b0: 6565 6420 3d20 3230 0a0a 2020 2020 2020  eed = 20..      
-0000e6c0: 2020 7365 6c66 2e64 6172 6b5f 6d6f 6465    self.dark_mode
-0000e6d0: 2829 0a20 2020 2020 2020 2073 656c 662e  ().        self.
-0000e6e0: 7368 6f77 5f63 6f6d 6d61 6e64 5f62 7574  show_command_but
-0000e6f0: 746f 6e73 2829 0a20 2020 2020 2020 2073  tons().        s
-0000e700: 656c 662e 7368 6f77 5f43 575f 6d61 6372  elf.show_CW_macr
-0000e710: 6f73 2829 0a20 2020 2020 2020 2023 2073  os().        # s
-0000e720: 656c 662e 7368 6f77 5f62 616e 645f 6d6f  elf.show_band_mo
-0000e730: 6465 2829 0a0a 2020 2020 6465 6620 7761  de()..    def wa
-0000e740: 7463 685f 7564 7028 7365 6c66 293a 0a20  tch_udp(self):. 
-0000e750: 2020 2020 2020 2022 2222 5075 7473 2055         """Puts U
-0000e760: 4450 2064 6174 6167 7261 6d73 2069 6e20  DP datagrams in 
-0000e770: 6120 4649 464f 2071 7565 7565 2222 220a  a FIFO queue""".
-0000e780: 2020 2020 2020 2020 7768 696c 6520 5472          while Tr
-0000e790: 7565 3a0a 2020 2020 2020 2020 2020 2020  ue:.            
-0000e7a0: 7472 793a 0a20 2020 2020 2020 2020 2020  try:.           
-0000e7b0: 2020 2020 2064 6174 6167 7261 6d20 3d20       datagram = 
-0000e7c0: 7365 6c66 2e6d 756c 7469 6361 7374 5f69  self.multicast_i
-0000e7d0: 6e74 6572 6661 6365 2e73 6572 7665 725f  nterface.server_
-0000e7e0: 7564 702e 7265 6376 2831 3530 3029 0a20  udp.recv(1500). 
-0000e7f0: 2020 2020 2020 2020 2020 2020 2020 206c                 l
-0000e800: 6f67 6765 722e 6465 6275 6728 6461 7461  ogger.debug(data
-0000e810: 6772 616d 2e64 6563 6f64 6528 2929 0a20  gram.decode()). 
-0000e820: 2020 2020 2020 2020 2020 2065 7863 6570             excep
-0000e830: 7420 736f 636b 6574 2e74 696d 656f 7574  t socket.timeout
-0000e840: 3a0a 2020 2020 2020 2020 2020 2020 2020  :.              
-0000e850: 2020 7469 6d65 2e73 6c65 6570 2830 2e31    time.sleep(0.1
-0000e860: 290a 2020 2020 2020 2020 2020 2020 2020  ).              
-0000e870: 2020 636f 6e74 696e 7565 0a20 2020 2020    continue.     
-0000e880: 2020 2020 2020 2069 6620 6461 7461 6772         if datagr
-0000e890: 616d 3a0a 2020 2020 2020 2020 2020 2020  am:.            
-0000e8a0: 2020 2020 7365 6c66 2e75 6470 5f66 6966      self.udp_fif
-0000e8b0: 6f2e 7075 7428 6461 7461 6772 616d 290a  o.put(datagram).
-0000e8c0: 0a20 2020 2064 6566 2063 6865 636b 5f75  .    def check_u
-0000e8d0: 6470 5f74 7261 6666 6963 2873 656c 6629  dp_traffic(self)
-0000e8e0: 3a0a 2020 2020 2020 2020 2222 2243 6865  :.        """Che
-0000e8f0: 636b 7320 5544 5020 5472 6166 6669 6322  cks UDP Traffic"
-0000e900: 2222 0a20 2020 2020 2020 2077 6869 6c65  "".        while
-0000e910: 206e 6f74 2073 656c 662e 7564 705f 6669   not self.udp_fi
-0000e920: 666f 2e65 6d70 7479 2829 3a0a 2020 2020  fo.empty():.    
-0000e930: 2020 2020 2020 2020 6461 7461 6772 616d          datagram
-0000e940: 203d 2073 656c 662e 7564 705f 6669 666f   = self.udp_fifo
-0000e950: 2e67 6574 2829 0a20 2020 2020 2020 2020  .get().         
-0000e960: 2020 2074 7279 3a0a 2020 2020 2020 2020     try:.        
-0000e970: 2020 2020 2020 2020 6465 6275 675f 696e          debug_in
-0000e980: 666f 203d 2066 227b 6461 7461 6772 616d  fo = f"{datagram
-0000e990: 2e64 6563 6f64 6528 297d 220a 2020 2020  .decode()}".    
-0000e9a0: 2020 2020 2020 2020 2020 2020 6c6f 6767              logg
-0000e9b0: 6572 2e64 6562 7567 2864 6562 7567 5f69  er.debug(debug_i
-0000e9c0: 6e66 6f29 0a20 2020 2020 2020 2020 2020  nfo).           
-0000e9d0: 2020 2020 206a 736f 6e5f 6461 7461 203d       json_data =
-0000e9e0: 206c 6f61 6473 2864 6174 6167 7261 6d2e   loads(datagram.
-0000e9f0: 6465 636f 6465 2829 290a 2020 2020 2020  decode()).      
-0000ea00: 2020 2020 2020 6578 6365 7074 2055 6e69        except Uni
-0000ea10: 636f 6465 4465 636f 6465 4572 726f 7220  codeDecodeError 
-0000ea20: 6173 2065 7272 3a0a 2020 2020 2020 2020  as err:.        
-0000ea30: 2020 2020 2020 2020 7468 655f 6572 726f          the_erro
-0000ea40: 7220 3d20 6622 4e6f 7420 556e 6963 6f64  r = f"Not Unicod
-0000ea50: 653a 207b 6572 727d 5c6e 7b64 6174 6167  e: {err}\n{datag
-0000ea60: 7261 6d7d 220a 2020 2020 2020 2020 2020  ram}".          
-0000ea70: 2020 2020 2020 6c6f 6767 6572 2e64 6562        logger.deb
-0000ea80: 7567 2874 6865 5f65 7272 6f72 290a 2020  ug(the_error).  
-0000ea90: 2020 2020 2020 2020 2020 2020 2020 636f                co
-0000eaa0: 6e74 696e 7565 0a20 2020 2020 2020 2020  ntinue.         
-0000eab0: 2020 2065 7863 6570 7420 4a53 4f4e 4465     except JSONDe
-0000eac0: 636f 6465 4572 726f 7220 6173 2065 7272  codeError as err
-0000ead0: 3a0a 2020 2020 2020 2020 2020 2020 2020  :.              
-0000eae0: 2020 7468 655f 6572 726f 7220 3d20 6622    the_error = f"
-0000eaf0: 4e6f 7420 4a53 4f4e 3a20 7b65 7272 7d5c  Not JSON: {err}\
-0000eb00: 6e7b 6461 7461 6772 616d 7d22 0a20 2020  n{datagram}".   
-0000eb10: 2020 2020 2020 2020 2020 2020 206c 6f67               log
-0000eb20: 6765 722e 6465 6275 6728 7468 655f 6572  ger.debug(the_er
-0000eb30: 726f 7229 0a20 2020 2020 2020 2020 2020  ror).           
-0000eb40: 2020 2020 2063 6f6e 7469 6e75 650a 2020       continue.  
-0000eb50: 2020 2020 2020 2020 2020 6966 2028 0a20            if (. 
-0000eb60: 2020 2020 2020 2020 2020 2020 2020 206a                 j
-0000eb70: 736f 6e5f 6461 7461 2e67 6574 2822 636d  son_data.get("cm
-0000eb80: 6422 2c20 2222 2920 3d3d 2022 4745 5443  d", "") == "GETC
-0000eb90: 4f4c 554d 4e53 220a 2020 2020 2020 2020  OLUMNS".        
-0000eba0: 2020 2020 2020 2020 616e 6420 6a73 6f6e          and json
-0000ebb0: 5f64 6174 612e 6765 7428 2273 7461 7469  _data.get("stati
-0000ebc0: 6f6e 222c 2022 2229 203d 3d20 706c 6174  on", "") == plat
-0000ebd0: 666f 726d 2e6e 6f64 6528 290a 2020 2020  form.node().    
-0000ebe0: 2020 2020 2020 2020 293a 0a20 2020 2020          ):.     
-0000ebf0: 2020 2020 2020 2020 2020 2069 6620 6861             if ha
-0000ec00: 7361 7474 7228 7365 6c66 2e63 6f6e 7465  sattr(self.conte
-0000ec10: 7374 2c20 2263 6f6c 756d 6e73 2229 3a0a  st, "columns"):.
-0000ec20: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000ec30: 2020 2020 636d 6420 3d20 7b7d 0a20 2020      cmd = {}.   
-0000ec40: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000ec50: 2063 6d64 5b22 636d 6422 5d20 3d20 2253   cmd["cmd"] = "S
-0000ec60: 484f 5743 4f4c 554d 4e53 220a 2020 2020  HOWCOLUMNS".    
-0000ec70: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000ec80: 636d 645b 2273 7461 7469 6f6e 225d 203d  cmd["station"] =
-0000ec90: 2070 6c61 7466 6f72 6d2e 6e6f 6465 2829   platform.node()
-0000eca0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-0000ecb0: 2020 2020 2063 6d64 5b22 434f 4c55 4d4e       cmd["COLUMN
-0000ecc0: 5322 5d20 3d20 7365 6c66 2e63 6f6e 7465  S"] = self.conte
-0000ecd0: 7374 2e63 6f6c 756d 6e73 0a20 2020 2020  st.columns.     
-0000ece0: 2020 2020 2020 2020 2020 2020 2020 2073                 s
-0000ecf0: 656c 662e 6d75 6c74 6963 6173 745f 696e  elf.multicast_in
-0000ed00: 7465 7266 6163 652e 7365 6e64 5f61 735f  terface.send_as_
-0000ed10: 6a73 6f6e 2863 6d64 290a 2020 2020 2020  json(cmd).      
-0000ed20: 2020 2020 2020 6966 2028 0a20 2020 2020        if (.     
-0000ed30: 2020 2020 2020 2020 2020 206a 736f 6e5f             json_
-0000ed40: 6461 7461 2e67 6574 2822 636d 6422 2c20  data.get("cmd", 
-0000ed50: 2222 2920 3d3d 2022 5455 4e45 220a 2020  "") == "TUNE".  
-0000ed60: 2020 2020 2020 2020 2020 2020 2020 616e                an
-0000ed70: 6420 6a73 6f6e 5f64 6174 612e 6765 7428  d json_data.get(
-0000ed80: 2273 7461 7469 6f6e 222c 2022 2229 203d  "station", "") =
-0000ed90: 3d20 706c 6174 666f 726d 2e6e 6f64 6528  = platform.node(
-0000eda0: 290a 2020 2020 2020 2020 2020 2020 293a  ).            ):
-0000edb0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-0000edc0: 2023 2062 277b 2263 6d64 223a 2022 5455   # b'{"cmd": "TU
-0000edd0: 4e45 222c 2022 6672 6571 223a 2037 2e30  NE", "freq": 7.0
-0000ede0: 3233 352c 2022 7370 6f74 223a 2022 4d4d  235, "spot": "MM
-0000edf0: 3044 4749 227d 270a 2020 2020 2020 2020  0DGI"}'.        
-0000ee00: 2020 2020 2020 2020 7666 6f20 3d20 6a73          vfo = js
-0000ee10: 6f6e 5f64 6174 612e 6765 7428 2266 7265  on_data.get("fre
-0000ee20: 7122 290a 2020 2020 2020 2020 2020 2020  q").            
-0000ee30: 2020 2020 7666 6f20 3d20 666c 6f61 7428      vfo = float(
-0000ee40: 7666 6f29 202a 2031 3030 3030 3030 0a20  vfo) * 1000000. 
-0000ee50: 2020 2020 2020 2020 2020 2020 2020 2073                 s
-0000ee60: 656c 662e 7261 6469 6f5f 7374 6174 655b  elf.radio_state[
-0000ee70: 2276 666f 6122 5d20 3d20 696e 7428 7666  "vfoa"] = int(vf
-0000ee80: 6f29 0a20 2020 2020 2020 2020 2020 2020  o).             
-0000ee90: 2020 2069 6620 7365 6c66 2e72 6967 5f63     if self.rig_c
-0000eea0: 6f6e 7472 6f6c 3a0a 2020 2020 2020 2020  ontrol:.        
-0000eeb0: 2020 2020 2020 2020 2020 2020 7365 6c66              self
-0000eec0: 2e72 6967 5f63 6f6e 7472 6f6c 2e73 6574  .rig_control.set
-0000eed0: 5f76 666f 2869 6e74 2876 666f 2929 0a20  _vfo(int(vfo)). 
-0000eee0: 2020 2020 2020 2020 2020 2020 2020 2073                 s
-0000eef0: 706f 7420 3d20 6a73 6f6e 5f64 6174 612e  pot = json_data.
-0000ef00: 6765 7428 2273 706f 7422 2c20 2222 290a  get("spot", "").
-0000ef10: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000ef20: 7365 6c66 2e63 616c 6c73 6967 6e2e 7365  self.callsign.se
-0000ef30: 7454 6578 7428 7370 6f74 290a 2020 2020  tText(spot).    
-0000ef40: 2020 2020 2020 2020 2020 2020 7365 6c66              self
-0000ef50: 2e63 616c 6c73 6967 6e5f 6368 616e 6765  .callsign_change
-0000ef60: 6428 290a 2020 2020 2020 2020 2020 2020  d().            
-0000ef70: 2020 2020 7365 6c66 2e63 616c 6c73 6967      self.callsig
-0000ef80: 6e2e 7365 7446 6f63 7573 2829 0a20 2020  n.setFocus().   
-0000ef90: 2020 2020 2020 2020 2020 2020 2073 656c               sel
-0000efa0: 662e 6361 6c6c 7369 676e 2e61 6374 6976  f.callsign.activ
-0000efb0: 6174 6557 696e 646f 7728 290a 2020 2020  ateWindow().    
-0000efc0: 2020 2020 2020 2020 2020 2020 7769 6e64              wind
-0000efd0: 6f77 2e72 6169 7365 5f28 290a 0a20 2020  ow.raise_()..   
-0000efe0: 2064 6566 2064 6172 6b5f 6d6f 6465 5f73   def dark_mode_s
-0000eff0: 7461 7465 5f63 6861 6e67 6528 7365 6c66  tate_change(self
-0000f000: 293a 0a20 2020 2020 2020 2022 2222 6461  ):.        """da
-0000f010: 726b 6d6f 6465 2064 726f 7064 6f77 6e20  rkmode dropdown 
-0000f020: 6368 6563 6b6d 6172 6b20 6368 616e 6765  checkmark change
-0000f030: 6422 2222 0a20 2020 2020 2020 2073 656c  d""".        sel
-0000f040: 662e 7072 6566 5b22 6461 726b 5f6d 6f64  f.pref["dark_mod
-0000f050: 6522 5d20 3d20 7365 6c66 2e61 6374 696f  e"] = self.actio
-0000f060: 6e44 6172 6b5f 4d6f 6465 2e69 7343 6865  nDark_Mode.isChe
-0000f070: 636b 6564 2829 0a20 2020 2020 2020 2073  cked().        s
-0000f080: 656c 662e 7772 6974 655f 7072 6566 6572  elf.write_prefer
-0000f090: 656e 6365 2829 0a20 2020 2020 2020 2073  ence().        s
-0000f0a0: 656c 662e 6461 726b 5f6d 6f64 6528 290a  elf.dark_mode().
-0000f0b0: 0a20 2020 2064 6566 2064 6172 6b5f 6d6f  .    def dark_mo
-0000f0c0: 6465 2873 656c 6629 3a0a 2020 2020 2020  de(self):.      
-0000f0d0: 2020 2222 2263 6861 6e67 6520 6469 7370    """change disp
-0000f0e0: 6c61 7920 6d6f 6465 2222 220a 2020 2020  lay mode""".    
-0000f0f0: 2020 2020 6966 2073 656c 662e 7072 6566      if self.pref
-0000f100: 2e67 6574 2822 6461 726b 5f6d 6f64 6522  .get("dark_mode"
-0000f110: 293a 0a20 2020 2020 2020 2020 2020 2073  ):.            s
-0000f120: 656c 662e 7365 7453 7479 6c65 5368 6565  elf.setStyleShee
-0000f130: 7428 4441 524b 5f53 5459 4c45 5348 4545  t(DARK_STYLESHEE
-0000f140: 5429 0a20 2020 2020 2020 2065 6c73 653a  T).        else:
-0000f150: 0a20 2020 2020 2020 2020 2020 2073 656c  .            sel
-0000f160: 662e 7365 7453 7479 6c65 5368 6565 7428  f.setStyleSheet(
-0000f170: 2222 290a 0a20 2020 2064 6566 2063 775f  "")..    def cw_
-0000f180: 6d61 6372 6f73 5f73 7461 7465 5f63 6861  macros_state_cha
-0000f190: 6e67 6564 2873 656c 6629 3a0a 2020 2020  nged(self):.    
-0000f1a0: 2020 2020 2222 224d 656e 7520 6974 656d      """Menu item
-0000f1b0: 2074 6f20 7368 6f77 2f68 6964 6520 6d61   to show/hide ma
-0000f1c0: 6372 6f20 6275 7474 6f6e 7322 2222 0a20  cro buttons""". 
-0000f1d0: 2020 2020 2020 2073 656c 662e 7072 6566         self.pref
-0000f1e0: 5b22 6377 5f6d 6163 726f 7322 5d20 3d20  ["cw_macros"] = 
-0000f1f0: 7365 6c66 2e61 6374 696f 6e43 575f 4d61  self.actionCW_Ma
-0000f200: 6372 6f73 2e69 7343 6865 636b 6564 2829  cros.isChecked()
-0000f210: 0a20 2020 2020 2020 2073 656c 662e 7772  .        self.wr
-0000f220: 6974 655f 7072 6566 6572 656e 6365 2829  ite_preference()
-0000f230: 0a20 2020 2020 2020 2073 656c 662e 7368  .        self.sh
-0000f240: 6f77 5f43 575f 6d61 6372 6f73 2829 0a0a  ow_CW_macros()..
-0000f250: 2020 2020 6465 6620 7368 6f77 5f43 575f      def show_CW_
-0000f260: 6d61 6372 6f73 2873 656c 6629 3a0a 2020  macros(self):.  
-0000f270: 2020 2020 2020 2222 226d 6163 726f 2062        """macro b
-0000f280: 7574 746f 6e20 7374 6174 6520 6368 616e  utton state chan
-0000f290: 6765 2222 220a 2020 2020 2020 2020 6966  ge""".        if
-0000f2a0: 2073 656c 662e 7072 6566 2e67 6574 2822   self.pref.get("
-0000f2b0: 6377 5f6d 6163 726f 7322 293a 0a20 2020  cw_macros"):.   
-0000f2c0: 2020 2020 2020 2020 2073 656c 662e 4275           self.Bu
-0000f2d0: 7474 6f6e 5f52 6f77 312e 7368 6f77 2829  tton_Row1.show()
-0000f2e0: 0a20 2020 2020 2020 2020 2020 2073 656c  .            sel
-0000f2f0: 662e 4275 7474 6f6e 5f52 6f77 322e 7368  f.Button_Row2.sh
-0000f300: 6f77 2829 0a20 2020 2020 2020 2065 6c73  ow().        els
-0000f310: 653a 0a20 2020 2020 2020 2020 2020 2073  e:.            s
-0000f320: 656c 662e 4275 7474 6f6e 5f52 6f77 312e  elf.Button_Row1.
-0000f330: 6869 6465 2829 0a20 2020 2020 2020 2020  hide().         
-0000f340: 2020 2073 656c 662e 4275 7474 6f6e 5f52     self.Button_R
-0000f350: 6f77 322e 6869 6465 2829 0a0a 2020 2020  ow2.hide()..    
-0000f360: 6465 6620 636f 6d6d 616e 645f 6275 7474  def command_butt
-0000f370: 6f6e 735f 7374 6174 655f 6368 616e 6765  ons_state_change
-0000f380: 2873 656c 6629 3a0a 2020 2020 2020 2020  (self):.        
-0000f390: 2222 224d 656e 7520 6974 656d 2074 6f20  """Menu item to 
-0000f3a0: 7368 6f77 2f68 6964 6520 636f 6d6d 616e  show/hide comman
-0000f3b0: 6420 6275 7474 6f6e 7322 2222 0a20 2020  d buttons""".   
-0000f3c0: 2020 2020 2073 656c 662e 7072 6566 5b22       self.pref["
-0000f3d0: 636f 6d6d 616e 645f 6275 7474 6f6e 7322  command_buttons"
-0000f3e0: 5d20 3d20 7365 6c66 2e61 6374 696f 6e43  ] = self.actionC
-0000f3f0: 6f6d 6d61 6e64 5f42 7574 746f 6e73 2e69  ommand_Buttons.i
-0000f400: 7343 6865 636b 6564 2829 0a20 2020 2020  sChecked().     
-0000f410: 2020 2073 656c 662e 7772 6974 655f 7072     self.write_pr
-0000f420: 6566 6572 656e 6365 2829 0a20 2020 2020  eference().     
-0000f430: 2020 2073 656c 662e 7368 6f77 5f63 6f6d     self.show_com
-0000f440: 6d61 6e64 5f62 7574 746f 6e73 2829 0a0a  mand_buttons()..
-0000f450: 2020 2020 6465 6620 7368 6f77 5f63 6f6d      def show_com
-0000f460: 6d61 6e64 5f62 7574 746f 6e73 2873 656c  mand_buttons(sel
-0000f470: 6629 3a0a 2020 2020 2020 2020 2222 2263  f):.        """c
-0000f480: 6f6d 6d61 6e64 2062 7574 746f 6e20 7374  ommand button st
-0000f490: 6174 6520 6368 616e 6765 2222 220a 2020  ate change""".  
-0000f4a0: 2020 2020 2020 6966 2073 656c 662e 7072        if self.pr
-0000f4b0: 6566 2e67 6574 2822 636f 6d6d 616e 645f  ef.get("command_
-0000f4c0: 6275 7474 6f6e 7322 293a 0a20 2020 2020  buttons"):.     
-0000f4d0: 2020 2020 2020 2073 656c 662e 436f 6d6d         self.Comm
-0000f4e0: 616e 645f 4275 7474 6f6e 732e 7368 6f77  and_Buttons.show
-0000f4f0: 2829 0a20 2020 2020 2020 2065 6c73 653a  ().        else:
-0000f500: 0a20 2020 2020 2020 2020 2020 2073 656c  .            sel
-0000f510: 662e 436f 6d6d 616e 645f 4275 7474 6f6e  f.Command_Button
-0000f520: 732e 6869 6465 2829 0a0a 2020 2020 6465  s.hide()..    de
-0000f530: 6620 6973 5f66 6c6f 6174 6162 6c65 2873  f is_floatable(s
-0000f540: 656c 662c 2069 7465 6d3a 2073 7472 2920  elf, item: str) 
-0000f550: 2d3e 2062 6f6f 6c3a 0a20 2020 2020 2020  -> bool:.       
-0000f560: 2022 2222 6368 6563 6b20 746f 2073 6565   """check to see
-0000f570: 2069 6620 7374 7269 6e67 2063 616e 2062   if string can b
-0000f580: 6520 6120 666c 6f61 7422 2222 0a20 2020  e a float""".   
-0000f590: 2020 2020 2069 6620 6974 656d 2e69 736e       if item.isn
-0000f5a0: 756d 6572 6963 2829 3a0a 2020 2020 2020  umeric():.      
-0000f5b0: 2020 2020 2020 7265 7475 726e 2054 7275        return Tru
-0000f5c0: 650a 2020 2020 2020 2020 7472 793a 0a20  e.        try:. 
-0000f5d0: 2020 2020 2020 2020 2020 205f 7465 7374             _test
-0000f5e0: 203d 2066 6c6f 6174 2869 7465 6d29 0a20   = float(item). 
-0000f5f0: 2020 2020 2020 2065 7863 6570 7420 5661         except Va
-0000f600: 6c75 6545 7272 6f72 3a0a 2020 2020 2020  lueError:.      
-0000f610: 2020 2020 2020 7265 7475 726e 2046 616c        return Fal
-0000f620: 7365 0a20 2020 2020 2020 2072 6574 7572  se.        retur
-0000f630: 6e20 5472 7565 0a0a 2020 2020 6465 6620  n True..    def 
-0000f640: 6f74 6865 725f 325f 6368 616e 6765 6428  other_2_changed(
-0000f650: 7365 6c66 293a 0a20 2020 2020 2020 2022  self):.        "
-0000f660: 2222 4361 6c6c 6564 2077 6865 6e20 7765  ""Called when we
-0000f670: 206e 6565 6420 746f 2070 6172 7365 2053   need to parse S
-0000f680: 5320 6578 6368 616e 6765 2e22 2222 0a20  S exchange.""". 
-0000f690: 2020 2020 2020 2069 6620 7365 6c66 2e63         if self.c
-0000f6a0: 6f6e 7465 7374 3a0a 2020 2020 2020 2020  ontest:.        
-0000f6b0: 2020 2020 6966 2022 4152 524c 2053 7765      if "ARRL Swe
-0000f6c0: 6570 7374 616b 6573 2220 696e 2073 656c  epstakes" in sel
-0000f6d0: 662e 636f 6e74 6573 742e 6e61 6d65 3a0a  f.contest.name:.
-0000f6e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000f6f0: 7365 6c66 2e63 6f6e 7465 7374 2e70 6172  self.contest.par
-0000f700: 7365 5f65 7863 6861 6e67 6528 7365 6c66  se_exchange(self
-0000f710: 290a 0a20 2020 2064 6566 2063 616c 6c73  )..    def calls
-0000f720: 6967 6e5f 6368 616e 6765 6428 7365 6c66  ign_changed(self
-0000f730: 293a 0a20 2020 2020 2020 2022 2222 4361  ):.        """Ca
-0000f740: 6c6c 6564 2077 6865 6e20 7465 7874 2069  lled when text i
-0000f750: 6e20 7468 6520 6361 6c6c 7369 676e 2066  n the callsign f
-0000f760: 6965 6c64 2068 6173 2063 6861 6e67 6564  ield has changed
-0000f770: 2222 220a 2020 2020 2020 2020 7465 7874  """.        text
-0000f780: 203d 2073 656c 662e 6361 6c6c 7369 676e   = self.callsign
-0000f790: 2e74 6578 7428 290a 2020 2020 2020 2020  .text().        
-0000f7a0: 7465 7874 203d 2074 6578 742e 7570 7065  text = text.uppe
-0000f7b0: 7228 290a 2020 2020 2020 2020 706f 7369  r().        posi
-0000f7c0: 7469 6f6e 203d 2073 656c 662e 6361 6c6c  tion = self.call
-0000f7d0: 7369 676e 2e63 7572 736f 7250 6f73 6974  sign.cursorPosit
-0000f7e0: 696f 6e28 290a 2020 2020 2020 2020 7374  ion().        st
-0000f7f0: 7269 7070 6564 5f74 6578 7420 3d20 7465  ripped_text = te
-0000f800: 7874 2e73 7472 6970 2829 2e72 6570 6c61  xt.strip().repla
-0000f810: 6365 2822 2022 2c20 2222 290a 2020 2020  ce(" ", "").    
-0000f820: 2020 2020 7365 6c66 2e63 616c 6c73 6967      self.callsig
-0000f830: 6e2e 7365 7454 6578 7428 7374 7269 7070  n.setText(stripp
-0000f840: 6564 5f74 6578 7429 0a20 2020 2020 2020  ed_text).       
-0000f850: 2073 656c 662e 6361 6c6c 7369 676e 2e73   self.callsign.s
-0000f860: 6574 4375 7273 6f72 506f 7369 7469 6f6e  etCursorPosition
-0000f870: 2870 6f73 6974 696f 6e29 0a0a 2020 2020  (position)..    
-0000f880: 2020 2020 6966 2022 2022 2069 6e20 7465      if " " in te
-0000f890: 7874 3a0a 2020 2020 2020 2020 2020 2020  xt:.            
-0000f8a0: 6966 2073 7472 6970 7065 645f 7465 7874  if stripped_text
-0000f8b0: 203d 3d20 2243 5722 3a0a 2020 2020 2020   == "CW":.      
-0000f8c0: 2020 2020 2020 2020 2020 7365 6c66 2e73            self.s
-0000f8d0: 6574 6d6f 6465 2822 4357 2229 0a20 2020  etmode("CW").   
-0000f8e0: 2020 2020 2020 2020 2020 2020 2073 656c               sel
-0000f8f0: 662e 7261 6469 6f5f 7374 6174 655b 226d  f.radio_state["m
-0000f900: 6f64 6522 5d20 3d20 2243 5722 0a20 2020  ode"] = "CW".   
-0000f910: 2020 2020 2020 2020 2020 2020 2069 6620               if 
-0000f920: 7365 6c66 2e72 6967 5f63 6f6e 7472 6f6c  self.rig_control
-0000f930: 3a0a 2020 2020 2020 2020 2020 2020 2020  :.              
-0000f940: 2020 2020 2020 6966 2073 656c 662e 7269        if self.ri
-0000f950: 675f 636f 6e74 726f 6c2e 6f6e 6c69 6e65  g_control.online
-0000f960: 3a0a 2020 2020 2020 2020 2020 2020 2020  :.              
-0000f970: 2020 2020 2020 2020 2020 7365 6c66 2e72            self.r
-0000f980: 6967 5f63 6f6e 7472 6f6c 2e73 6574 5f6d  ig_control.set_m
-0000f990: 6f64 6528 2243 5722 290a 2020 2020 2020  ode("CW").      
-0000f9a0: 2020 2020 2020 2020 2020 7365 6c66 2e73            self.s
-0000f9b0: 6574 5f77 696e 646f 775f 7469 746c 6528  et_window_title(
-0000f9c0: 290a 2020 2020 2020 2020 2020 2020 2020  ).              
-0000f9d0: 2020 7365 6c66 2e63 6c65 6172 696e 7075    self.clearinpu
-0000f9e0: 7473 2829 0a20 2020 2020 2020 2020 2020  ts().           
-0000f9f0: 2020 2020 2073 656c 662e 7265 6164 5f63       self.read_c
-0000fa00: 775f 6d61 6372 6f73 2829 0a20 2020 2020  w_macros().     
-0000fa10: 2020 2020 2020 2020 2020 2072 6574 7572             retur
-0000fa20: 6e0a 2020 2020 2020 2020 2020 2020 6966  n.            if
-0000fa30: 2073 7472 6970 7065 645f 7465 7874 203d   stripped_text =
-0000fa40: 3d20 2252 5454 5922 3a0a 2020 2020 2020  = "RTTY":.      
-0000fa50: 2020 2020 2020 2020 2020 7365 6c66 2e73            self.s
-0000fa60: 6574 6d6f 6465 2822 5254 5459 2229 0a20  etmode("RTTY"). 
-0000fa70: 2020 2020 2020 2020 2020 2020 2020 2069                 i
-0000fa80: 6620 7365 6c66 2e72 6967 5f63 6f6e 7472  f self.rig_contr
-0000fa90: 6f6c 3a0a 2020 2020 2020 2020 2020 2020  ol:.            
-0000faa0: 2020 2020 2020 2020 6966 2073 656c 662e          if self.
-0000fab0: 7269 675f 636f 6e74 726f 6c2e 6f6e 6c69  rig_control.onli
-0000fac0: 6e65 3a0a 2020 2020 2020 2020 2020 2020  ne:.            
-0000fad0: 2020 2020 2020 2020 2020 2020 7365 6c66              self
-0000fae0: 2e72 6967 5f63 6f6e 7472 6f6c 2e73 6574  .rig_control.set
-0000faf0: 5f6d 6f64 6528 2252 5454 5922 290a 2020  _mode("RTTY").  
-0000fb00: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000fb10: 2020 656c 7365 3a0a 2020 2020 2020 2020    else:.        
-0000fb20: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000fb30: 7365 6c66 2e72 6164 696f 5f73 7461 7465  self.radio_state
-0000fb40: 5b22 6d6f 6465 225d 203d 2022 5254 5459  ["mode"] = "RTTY
-0000fb50: 220a 2020 2020 2020 2020 2020 2020 2020  ".              
-0000fb60: 2020 7365 6c66 2e73 6574 5f77 696e 646f    self.set_windo
-0000fb70: 775f 7469 746c 6528 290a 2020 2020 2020  w_title().      
-0000fb80: 2020 2020 2020 2020 2020 7365 6c66 2e63            self.c
-0000fb90: 6c65 6172 696e 7075 7473 2829 0a20 2020  learinputs().   
-0000fba0: 2020 2020 2020 2020 2020 2020 2072 6574               ret
-0000fbb0: 7572 6e0a 2020 2020 2020 2020 2020 2020  urn.            
-0000fbc0: 6966 2073 7472 6970 7065 645f 7465 7874  if stripped_text
-0000fbd0: 203d 3d20 2253 5342 223a 0a20 2020 2020   == "SSB":.     
-0000fbe0: 2020 2020 2020 2020 2020 2073 656c 662e             self.
-0000fbf0: 7365 746d 6f64 6528 2253 5342 2229 0a20  setmode("SSB"). 
-0000fc00: 2020 2020 2020 2020 2020 2020 2020 2069                 i
-0000fc10: 6620 696e 7428 7365 6c66 2e72 6164 696f  f int(self.radio
-0000fc20: 5f73 7461 7465 2e67 6574 2822 7666 6f61  _state.get("vfoa
-0000fc30: 222c 2030 2929 203e 2031 3030 3030 3030  ", 0)) > 1000000
-0000fc40: 303a 0a20 2020 2020 2020 2020 2020 2020  0:.             
-0000fc50: 2020 2020 2020 2073 656c 662e 7261 6469         self.radi
-0000fc60: 6f5f 7374 6174 655b 226d 6f64 6522 5d20  o_state["mode"] 
-0000fc70: 3d20 2255 5342 220a 2020 2020 2020 2020  = "USB".        
-0000fc80: 2020 2020 2020 2020 656c 7365 3a0a 2020          else:.  
-0000fc90: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000fca0: 2020 7365 6c66 2e72 6164 696f 5f73 7461    self.radio_sta
-0000fcb0: 7465 5b22 6d6f 6465 225d 203d 2022 4c53  te["mode"] = "LS
-0000fcc0: 4222 0a20 2020 2020 2020 2020 2020 2020  B".             
-0000fcd0: 2020 2073 656c 662e 7365 745f 7769 6e64     self.set_wind
-0000fce0: 6f77 5f74 6974 6c65 2829 0a20 2020 2020  ow_title().     
-0000fcf0: 2020 2020 2020 2020 2020 2069 6620 7365             if se
-0000fd00: 6c66 2e72 6967 5f63 6f6e 7472 6f6c 3a0a  lf.rig_control:.
-0000fd10: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000fd20: 2020 2020 7365 6c66 2e72 6967 5f63 6f6e      self.rig_con
-0000fd30: 7472 6f6c 2e73 6574 5f6d 6f64 6528 7365  trol.set_mode(se
-0000fd40: 6c66 2e72 6164 696f 5f73 7461 7465 2e67  lf.radio_state.g
-0000fd50: 6574 2822 6d6f 6465 2229 290a 2020 2020  et("mode")).    
-0000fd60: 2020 2020 2020 2020 2020 2020 7365 6c66              self
-0000fd70: 2e63 6c65 6172 696e 7075 7473 2829 0a20  .clearinputs(). 
-0000fd80: 2020 2020 2020 2020 2020 2020 2020 2073                 s
-0000fd90: 656c 662e 7265 6164 5f63 775f 6d61 6372  elf.read_cw_macr
-0000fda0: 6f73 2829 0a20 2020 2020 2020 2020 2020  os().           
-0000fdb0: 2020 2020 2072 6574 7572 6e0a 2020 2020       return.    
-0000fdc0: 2020 2020 2020 2020 6966 2073 7472 6970          if strip
-0000fdd0: 7065 645f 7465 7874 203d 3d20 224f 504f  ped_text == "OPO
-0000fde0: 4e22 3a0a 2020 2020 2020 2020 2020 2020  N":.            
-0000fdf0: 2020 2020 7365 6c66 2e67 6574 5f6f 706f      self.get_opo
-0000fe00: 6e28 290a 2020 2020 2020 2020 2020 2020  n().            
-0000fe10: 2020 2020 7365 6c66 2e63 6c65 6172 696e      self.clearin
-0000fe20: 7075 7473 2829 0a20 2020 2020 2020 2020  puts().         
-0000fe30: 2020 2020 2020 2072 6574 7572 6e0a 2020         return.  
-0000fe40: 2020 2020 2020 2020 2020 6966 2073 7472            if str
-0000fe50: 6970 7065 645f 7465 7874 203d 3d20 2254  ipped_text == "T
-0000fe60: 4553 5422 3a0a 2020 2020 2020 2020 2020  EST":.          
-0000fe70: 2020 2020 2020 7365 6c66 2e73 686f 775f        self.show_
-0000fe80: 6d65 7373 6167 655f 626f 7828 2254 6869  message_box("Thi
-0000fe90: 7320 6973 2061 2074 6573 7422 290a 2020  s is a test").  
-0000fea0: 2020 2020 2020 2020 2020 2020 2020 7365                se
-0000feb0: 6c66 2e63 6c65 6172 696e 7075 7473 2829  lf.clearinputs()
-0000fec0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-0000fed0: 2072 6574 7572 6e0a 2020 2020 2020 2020   return.        
-0000fee0: 2020 2020 6966 2073 656c 662e 6973 5f66      if self.is_f
-0000fef0: 6c6f 6174 6162 6c65 2873 7472 6970 7065  loatable(strippe
-0000ff00: 645f 7465 7874 293a 0a20 2020 2020 2020  d_text):.       
-0000ff10: 2020 2020 2020 2020 2076 666f 203d 2066           vfo = f
-0000ff20: 6c6f 6174 2873 7472 6970 7065 645f 7465  loat(stripped_te
-0000ff30: 7874 290a 2020 2020 2020 2020 2020 2020  xt).            
-0000ff40: 2020 2020 7666 6f20 3d20 696e 7428 7666      vfo = int(vf
-0000ff50: 6f20 2a20 3130 3030 290a 2020 2020 2020  o * 1000).      
-0000ff60: 2020 2020 2020 2020 2020 6261 6e64 203d            band =
-0000ff70: 2067 6574 6261 6e64 2873 7472 2876 666f   getband(str(vfo
-0000ff80: 2929 0a20 2020 2020 2020 2020 2020 2020  )).             
-0000ff90: 2020 2073 656c 662e 7365 745f 6261 6e64     self.set_band
-0000ffa0: 5f69 6e64 6963 6174 6f72 2862 616e 6429  _indicator(band)
-0000ffb0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-0000ffc0: 2023 2073 656c 662e 636f 6e74 6163 745b   # self.contact[
-0000ffd0: 2242 616e 6422 5d20 3d20 6765 745f 6c6f  "Band"] = get_lo
-0000ffe0: 6767 6564 5f62 616e 6428 7374 7228 7365  gged_band(str(se
-0000fff0: 6c66 2e72 6164 696f 5f73 7461 7465 2e67  lf.radio_state.g
-00010000: 6574 2822 7666 6f61 222c 2030 2e30 2929  et("vfoa", 0.0))
-00010010: 290a 2020 2020 2020 2020 2020 2020 2020  ).              
-00010020: 2020 7365 6c66 2e72 6164 696f 5f73 7461    self.radio_sta
-00010030: 7465 5b22 7666 6f61 225d 203d 2076 666f  te["vfoa"] = vfo
-00010040: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00010050: 2073 656c 662e 7365 745f 7769 6e64 6f77   self.set_window
-00010060: 5f74 6974 6c65 2829 0a20 2020 2020 2020  _title().       
-00010070: 2020 2020 2020 2020 2073 656c 662e 636c           self.cl
-00010080: 6561 7269 6e70 7574 7328 290a 2020 2020  earinputs().    
-00010090: 2020 2020 2020 2020 2020 2020 6966 2073              if s
-000100a0: 656c 662e 7269 675f 636f 6e74 726f 6c3a  elf.rig_control:
-000100b0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-000100c0: 2020 2020 2073 656c 662e 7269 675f 636f       self.rig_co
-000100d0: 6e74 726f 6c2e 7365 745f 7666 6f28 7666  ntrol.set_vfo(vf
-000100e0: 6f29 0a20 2020 2020 2020 2020 2020 2020  o).             
-000100f0: 2020 2072 6574 7572 6e0a 0a20 2020 2020     return..     
-00010100: 2020 2020 2020 2073 656c 662e 6368 6563         self.chec
-00010110: 6b5f 6361 6c6c 7369 676e 2873 7472 6970  k_callsign(strip
-00010120: 7065 645f 7465 7874 290a 2020 2020 2020  ped_text).      
-00010130: 2020 2020 2020 6966 2073 656c 662e 6368        if self.ch
-00010140: 6563 6b5f 6475 7065 2873 7472 6970 7065  eck_dupe(strippe
-00010150: 645f 7465 7874 293a 0a20 2020 2020 2020  d_text):.       
-00010160: 2020 2020 2020 2020 2073 656c 662e 6475           self.du
-00010170: 7065 5f69 6e64 6963 6174 6f72 2e73 686f  pe_indicator.sho
-00010180: 7728 290a 2020 2020 2020 2020 2020 2020  w().            
-00010190: 656c 7365 3a0a 2020 2020 2020 2020 2020  else:.          
-000101a0: 2020 2020 2020 7365 6c66 2e64 7570 655f        self.dupe_
-000101b0: 696e 6469 6361 746f 722e 6869 6465 2829  indicator.hide()
-000101c0: 0a20 2020 2020 2020 2020 2020 205f 7468  .            _th
-000101d0: 6574 6872 6561 6420 3d20 7468 7265 6164  ethread = thread
-000101e0: 696e 672e 5468 7265 6164 280a 2020 2020  ing.Thread(.    
-000101f0: 2020 2020 2020 2020 2020 2020 7461 7267              targ
-00010200: 6574 3d73 656c 662e 6368 6563 6b5f 6361  et=self.check_ca
-00010210: 6c6c 7369 676e 322c 0a20 2020 2020 2020  llsign2,.       
-00010220: 2020 2020 2020 2020 2061 7267 733d 2874           args=(t
-00010230: 6578 742c 292c 0a20 2020 2020 2020 2020  ext,),.         
-00010240: 2020 2020 2020 2064 6165 6d6f 6e3d 5472         daemon=Tr
-00010250: 7565 2c0a 2020 2020 2020 2020 2020 2020  ue,.            
-00010260: 290a 2020 2020 2020 2020 2020 2020 5f74  ).            _t
-00010270: 6865 7468 7265 6164 2e73 7461 7274 2829  hethread.start()
-00010280: 0a20 2020 2020 2020 2020 2020 2073 656c  .            sel
-00010290: 662e 6e65 7874 5f66 6965 6c64 2e73 6574  f.next_field.set
-000102a0: 466f 6375 7328 290a 2020 2020 2020 2020  Focus().        
-000102b0: 2020 2020 7265 7475 726e 0a20 2020 2020      return.     
-000102c0: 2020 2063 6d64 203d 207b 7d0a 2020 2020     cmd = {}.    
-000102d0: 2020 2020 636d 645b 2263 6d64 225d 203d      cmd["cmd"] =
-000102e0: 2022 4341 4c4c 4348 414e 4745 4422 0a20   "CALLCHANGED". 
-000102f0: 2020 2020 2020 2063 6d64 5b22 7374 6174         cmd["stat
-00010300: 696f 6e22 5d20 3d20 706c 6174 666f 726d  ion"] = platform
-00010310: 2e6e 6f64 6528 290a 2020 2020 2020 2020  .node().        
-00010320: 636d 645b 2263 616c 6c22 5d20 3d20 7374  cmd["call"] = st
-00010330: 7269 7070 6564 5f74 6578 740a 2020 2020  ripped_text.    
-00010340: 2020 2020 7365 6c66 2e6d 756c 7469 6361      self.multica
-00010350: 7374 5f69 6e74 6572 6661 6365 2e73 656e  st_interface.sen
-00010360: 645f 6173 5f6a 736f 6e28 636d 6429 0a20  d_as_json(cmd). 
-00010370: 2020 2020 2020 2073 656c 662e 6368 6563         self.chec
-00010380: 6b5f 6361 6c6c 7369 676e 2873 7472 6970  k_callsign(strip
-00010390: 7065 645f 7465 7874 290a 0a20 2020 2064  ped_text)..    d
-000103a0: 6566 2063 6865 636b 5f63 616c 6c73 6967  ef check_callsig
-000103b0: 6e28 7365 6c66 2c20 6361 6c6c 7369 676e  n(self, callsign
-000103c0: 293a 0a20 2020 2020 2020 2022 2222 4368  ):.        """Ch
-000103d0: 6563 6b20 6361 6c6c 2061 7320 656e 7465  eck call as ente
-000103e0: 7265 6422 2222 0a20 2020 2020 2020 2072  red""".        r
-000103f0: 6573 756c 7420 3d20 6374 795f 6c6f 6f6b  esult = cty_look
-00010400: 7570 2863 616c 6c73 6967 6e29 0a20 2020  up(callsign).   
-00010410: 2020 2020 2064 6562 7567 5f72 6573 756c       debug_resul
-00010420: 7420 3d20 6622 7b72 6573 756c 747d 220a  t = f"{result}".
-00010430: 2020 2020 2020 2020 6c6f 6767 6572 2e64          logger.d
-00010440: 6562 7567 2822 2573 222c 2064 6562 7567  ebug("%s", debug
-00010450: 5f72 6573 756c 7429 0a20 2020 2020 2020  _result).       
-00010460: 2069 6620 7265 7375 6c74 3a0a 2020 2020   if result:.    
-00010470: 2020 2020 2020 2020 666f 7220 6120 696e          for a in
-00010480: 2072 6573 756c 742e 6974 656d 7328 293a   result.items():
-00010490: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-000104a0: 2065 6e74 6974 7920 3d20 615b 315d 2e67   entity = a[1].g
-000104b0: 6574 2822 656e 7469 7479 222c 2022 2229  et("entity", "")
-000104c0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-000104d0: 2063 7120 3d20 615b 315d 2e67 6574 2822   cq = a[1].get("
-000104e0: 6371 222c 2022 2229 0a20 2020 2020 2020  cq", "").       
-000104f0: 2020 2020 2020 2020 2069 7475 203d 2061           itu = a
-00010500: 5b31 5d2e 6765 7428 2269 7475 222c 2022  [1].get("itu", "
+0000c4b0: 2020 6578 6365 7074 2073 642e 506f 7274    except sd.Port
+0000c4c0: 4175 6469 6f45 7272 6f72 2061 7320 6572  AudioError as er
+0000c4d0: 723a 0a20 2020 2020 2020 2020 2020 2020  r:.             
+0000c4e0: 2020 2020 2020 2020 2020 206c 6f67 6765             logge
+0000c4f0: 722e 6465 6275 6728 2225 7322 2c20 6622  r.debug("%s", f"
+0000c500: 7b65 7272 7d22 290a 2020 2020 2020 2020  {err}").        
+0000c510: 7365 6c66 2e70 7474 5f6f 6666 2829 0a0a  self.ptt_off()..
+0000c520: 2020 2020 6465 6620 7074 745f 6f6e 2873      def ptt_on(s
+0000c530: 656c 6629 3a0a 2020 2020 2020 2020 2222  elf):.        ""
+0000c540: 2274 7572 6e20 6f6e 2070 7474 2222 220a  "turn on ptt""".
+0000c550: 2020 2020 2020 2020 6966 2073 656c 662e          if self.
+0000c560: 7269 675f 636f 6e74 726f 6c3a 0a20 2020  rig_control:.   
+0000c570: 2020 2020 2020 2020 2073 656c 662e 6c65           self.le
+0000c580: 6674 646f 742e 7365 7450 6978 6d61 7028  ftdot.setPixmap(
+0000c590: 7365 6c66 2e67 7265 656e 646f 7429 0a20  self.greendot). 
+0000c5a0: 2020 2020 2020 2020 2020 2061 7070 2e70             app.p
+0000c5b0: 726f 6365 7373 4576 656e 7473 2829 0a20  rocessEvents(). 
+0000c5c0: 2020 2020 2020 2020 2020 2073 656c 662e             self.
+0000c5d0: 7269 675f 636f 6e74 726f 6c2e 7074 745f  rig_control.ptt_
+0000c5e0: 6f6e 2829 0a0a 2020 2020 6465 6620 7074  on()..    def pt
+0000c5f0: 745f 6f66 6628 7365 6c66 293a 0a20 2020  t_off(self):.   
+0000c600: 2020 2020 2022 2222 7475 726e 206f 6666       """turn off
+0000c610: 2070 7474 2222 220a 2020 2020 2020 2020   ptt""".        
+0000c620: 6966 2073 656c 662e 7269 675f 636f 6e74  if self.rig_cont
+0000c630: 726f 6c3a 0a20 2020 2020 2020 2020 2020  rol:.           
+0000c640: 2073 656c 662e 6c65 6674 646f 742e 7365   self.leftdot.se
+0000c650: 7450 6978 6d61 7028 7365 6c66 2e72 6564  tPixmap(self.red
+0000c660: 646f 7429 0a20 2020 2020 2020 2020 2020  dot).           
+0000c670: 2061 7070 2e70 726f 6365 7373 4576 656e   app.processEven
+0000c680: 7473 2829 0a20 2020 2020 2020 2020 2020  ts().           
+0000c690: 2073 656c 662e 7269 675f 636f 6e74 726f   self.rig_contro
+0000c6a0: 6c2e 7074 745f 6f66 6628 290a 0a20 2020  l.ptt_off()..   
+0000c6b0: 2064 6566 2073 656e 6466 3128 7365 6c66   def sendf1(self
+0000c6c0: 293a 0a20 2020 2020 2020 2022 2222 7374  ):.        """st
+0000c6d0: 7562 2222 220a 2020 2020 2020 2020 6c6f  ub""".        lo
+0000c6e0: 6767 6572 2e64 6562 7567 2822 4631 2043  gger.debug("F1 C
+0000c6f0: 6c69 636b 6564 2229 0a20 2020 2020 2020  licked").       
+0000c700: 2069 6620 7365 6c66 2e72 6164 696f 5f73   if self.radio_s
+0000c710: 7461 7465 2e67 6574 2822 6d6f 6465 2229  tate.get("mode")
+0000c720: 2069 6e20 5b22 4c53 4222 2c20 2255 5342   in ["LSB", "USB
+0000c730: 222c 2022 5353 4222 5d3a 0a20 2020 2020  ", "SSB"]:.     
+0000c740: 2020 2020 2020 2073 656c 662e 766f 6963         self.voic
+0000c750: 655f 7374 7269 6e67 2873 656c 662e 7072  e_string(self.pr
+0000c760: 6f63 6573 735f 6d61 6372 6f28 7365 6c66  ocess_macro(self
+0000c770: 2e46 312e 746f 6f6c 5469 7028 2929 290a  .F1.toolTip())).
+0000c780: 2020 2020 2020 2020 2020 2020 7265 7475              retu
+0000c790: 726e 0a20 2020 2020 2020 2069 6620 7365  rn.        if se
+0000c7a0: 6c66 2e63 773a 0a20 2020 2020 2020 2020  lf.cw:.         
+0000c7b0: 2020 2023 2069 6620 7365 6c66 2e70 7265     # if self.pre
+0000c7c0: 6665 7265 6e63 652e 6765 7428 2273 656e  ference.get("sen
+0000c7d0: 645f 6e31 6d6d 5f70 6163 6b65 7473 2229  d_n1mm_packets")
+0000c7e0: 3a0a 2020 2020 2020 2020 2020 2020 2320  :.            # 
+0000c7f0: 2020 2020 7365 6c66 2e6e 316d 6d2e 7261      self.n1mm.ra
+0000c800: 6469 6f5f 696e 666f 5b22 4675 6e63 7469  dio_info["Functi
+0000c810: 6f6e 4b65 7943 6170 7469 6f6e 225d 203d  onKeyCaption"] =
+0000c820: 2073 656c 662e 4631 2e74 6578 7428 290a   self.F1.text().
+0000c830: 2020 2020 2020 2020 2020 2020 7365 6c66              self
+0000c840: 2e63 772e 7365 6e64 6377 2873 656c 662e  .cw.sendcw(self.
+0000c850: 7072 6f63 6573 735f 6d61 6372 6f28 7365  process_macro(se
+0000c860: 6c66 2e46 312e 746f 6f6c 5469 7028 2929  lf.F1.toolTip())
+0000c870: 290a 0a20 2020 2064 6566 2073 656e 6466  )..    def sendf
+0000c880: 3228 7365 6c66 293a 0a20 2020 2020 2020  2(self):.       
+0000c890: 2022 2222 7374 7562 2222 220a 2020 2020   """stub""".    
+0000c8a0: 2020 2020 6c6f 6767 6572 2e64 6562 7567      logger.debug
+0000c8b0: 2822 4632 2043 6c69 636b 6564 2229 0a20  ("F2 Clicked"). 
+0000c8c0: 2020 2020 2020 2069 6620 7365 6c66 2e72         if self.r
+0000c8d0: 6164 696f 5f73 7461 7465 2e67 6574 2822  adio_state.get("
+0000c8e0: 6d6f 6465 2229 2069 6e20 5b22 4c53 4222  mode") in ["LSB"
+0000c8f0: 2c20 2255 5342 222c 2022 5353 4222 5d3a  , "USB", "SSB"]:
+0000c900: 0a20 2020 2020 2020 2020 2020 2073 656c  .            sel
+0000c910: 662e 766f 6963 655f 7374 7269 6e67 2873  f.voice_string(s
+0000c920: 656c 662e 7072 6f63 6573 735f 6d61 6372  elf.process_macr
+0000c930: 6f28 7365 6c66 2e46 322e 746f 6f6c 5469  o(self.F2.toolTi
+0000c940: 7028 2929 290a 2020 2020 2020 2020 2020  p())).          
+0000c950: 2020 7265 7475 726e 0a20 2020 2020 2020    return.       
+0000c960: 2069 6620 7365 6c66 2e63 773a 0a20 2020   if self.cw:.   
+0000c970: 2020 2020 2020 2020 2073 656c 662e 6377           self.cw
+0000c980: 2e73 656e 6463 7728 7365 6c66 2e70 726f  .sendcw(self.pro
+0000c990: 6365 7373 5f6d 6163 726f 2873 656c 662e  cess_macro(self.
+0000c9a0: 4632 2e74 6f6f 6c54 6970 2829 2929 0a0a  F2.toolTip()))..
+0000c9b0: 2020 2020 6465 6620 7365 6e64 6633 2873      def sendf3(s
+0000c9c0: 656c 6629 3a0a 2020 2020 2020 2020 2222  elf):.        ""
+0000c9d0: 2273 7475 6222 2222 0a20 2020 2020 2020  "stub""".       
+0000c9e0: 206c 6f67 6765 722e 6465 6275 6728 2246   logger.debug("F
+0000c9f0: 3320 436c 6963 6b65 6422 290a 2020 2020  3 Clicked").    
+0000ca00: 2020 2020 6966 2073 656c 662e 7261 6469      if self.radi
+0000ca10: 6f5f 7374 6174 652e 6765 7428 226d 6f64  o_state.get("mod
+0000ca20: 6522 2920 696e 205b 224c 5342 222c 2022  e") in ["LSB", "
+0000ca30: 5553 4222 2c20 2253 5342 225d 3a0a 2020  USB", "SSB"]:.  
+0000ca40: 2020 2020 2020 2020 2020 7365 6c66 2e76            self.v
+0000ca50: 6f69 6365 5f73 7472 696e 6728 7365 6c66  oice_string(self
+0000ca60: 2e70 726f 6365 7373 5f6d 6163 726f 2873  .process_macro(s
+0000ca70: 656c 662e 4633 2e74 6f6f 6c54 6970 2829  elf.F3.toolTip()
+0000ca80: 2929 0a20 2020 2020 2020 2020 2020 2072  )).            r
+0000ca90: 6574 7572 6e0a 2020 2020 2020 2020 6966  eturn.        if
+0000caa0: 2073 656c 662e 6377 3a0a 2020 2020 2020   self.cw:.      
+0000cab0: 2020 2020 2020 7365 6c66 2e63 772e 7365        self.cw.se
+0000cac0: 6e64 6377 2873 656c 662e 7072 6f63 6573  ndcw(self.proces
+0000cad0: 735f 6d61 6372 6f28 7365 6c66 2e46 332e  s_macro(self.F3.
+0000cae0: 746f 6f6c 5469 7028 2929 290a 0a20 2020  toolTip()))..   
+0000caf0: 2064 6566 2073 656e 6466 3428 7365 6c66   def sendf4(self
+0000cb00: 293a 0a20 2020 2020 2020 2022 2222 7374  ):.        """st
+0000cb10: 7562 2222 220a 2020 2020 2020 2020 6c6f  ub""".        lo
+0000cb20: 6767 6572 2e64 6562 7567 2822 4634 2043  gger.debug("F4 C
+0000cb30: 6c69 636b 6564 2229 0a20 2020 2020 2020  licked").       
+0000cb40: 2069 6620 7365 6c66 2e72 6164 696f 5f73   if self.radio_s
+0000cb50: 7461 7465 2e67 6574 2822 6d6f 6465 2229  tate.get("mode")
+0000cb60: 2069 6e20 5b22 4c53 4222 2c20 2255 5342   in ["LSB", "USB
+0000cb70: 222c 2022 5353 4222 5d3a 0a20 2020 2020  ", "SSB"]:.     
+0000cb80: 2020 2020 2020 2073 656c 662e 766f 6963         self.voic
+0000cb90: 655f 7374 7269 6e67 2873 656c 662e 7072  e_string(self.pr
+0000cba0: 6f63 6573 735f 6d61 6372 6f28 7365 6c66  ocess_macro(self
+0000cbb0: 2e46 342e 746f 6f6c 5469 7028 2929 290a  .F4.toolTip())).
+0000cbc0: 2020 2020 2020 2020 2020 2020 7265 7475              retu
+0000cbd0: 726e 0a20 2020 2020 2020 2069 6620 7365  rn.        if se
+0000cbe0: 6c66 2e63 773a 0a20 2020 2020 2020 2020  lf.cw:.         
+0000cbf0: 2020 2073 656c 662e 6377 2e73 656e 6463     self.cw.sendc
+0000cc00: 7728 7365 6c66 2e70 726f 6365 7373 5f6d  w(self.process_m
+0000cc10: 6163 726f 2873 656c 662e 4634 2e74 6f6f  acro(self.F4.too
+0000cc20: 6c54 6970 2829 2929 0a0a 2020 2020 6465  lTip()))..    de
+0000cc30: 6620 7365 6e64 6635 2873 656c 6629 3a0a  f sendf5(self):.
+0000cc40: 2020 2020 2020 2020 2222 2273 7475 6222          """stub"
+0000cc50: 2222 0a20 2020 2020 2020 206c 6f67 6765  "".        logge
+0000cc60: 722e 6465 6275 6728 2246 3520 436c 6963  r.debug("F5 Clic
+0000cc70: 6b65 6422 290a 2020 2020 2020 2020 6966  ked").        if
+0000cc80: 2073 656c 662e 7261 6469 6f5f 7374 6174   self.radio_stat
+0000cc90: 652e 6765 7428 226d 6f64 6522 2920 696e  e.get("mode") in
+0000cca0: 205b 224c 5342 222c 2022 5553 4222 2c20   ["LSB", "USB", 
+0000ccb0: 2253 5342 225d 3a0a 2020 2020 2020 2020  "SSB"]:.        
+0000ccc0: 2020 2020 7365 6c66 2e76 6f69 6365 5f73      self.voice_s
+0000ccd0: 7472 696e 6728 7365 6c66 2e70 726f 6365  tring(self.proce
+0000cce0: 7373 5f6d 6163 726f 2873 656c 662e 4635  ss_macro(self.F5
+0000ccf0: 2e74 6f6f 6c54 6970 2829 2929 0a20 2020  .toolTip())).   
+0000cd00: 2020 2020 2020 2020 2072 6574 7572 6e0a           return.
+0000cd10: 2020 2020 2020 2020 6966 2073 656c 662e          if self.
+0000cd20: 6377 3a0a 2020 2020 2020 2020 2020 2020  cw:.            
+0000cd30: 7365 6c66 2e63 772e 7365 6e64 6377 2873  self.cw.sendcw(s
+0000cd40: 656c 662e 7072 6f63 6573 735f 6d61 6372  elf.process_macr
+0000cd50: 6f28 7365 6c66 2e46 352e 746f 6f6c 5469  o(self.F5.toolTi
+0000cd60: 7028 2929 290a 0a20 2020 2064 6566 2073  p()))..    def s
+0000cd70: 656e 6466 3628 7365 6c66 293a 0a20 2020  endf6(self):.   
+0000cd80: 2020 2020 2022 2222 7374 7562 2222 220a       """stub""".
+0000cd90: 2020 2020 2020 2020 6c6f 6767 6572 2e64          logger.d
+0000cda0: 6562 7567 2822 4636 2043 6c69 636b 6564  ebug("F6 Clicked
+0000cdb0: 2229 0a20 2020 2020 2020 2069 6620 7365  ").        if se
+0000cdc0: 6c66 2e72 6164 696f 5f73 7461 7465 2e67  lf.radio_state.g
+0000cdd0: 6574 2822 6d6f 6465 2229 2069 6e20 5b22  et("mode") in ["
+0000cde0: 4c53 4222 2c20 2255 5342 222c 2022 5353  LSB", "USB", "SS
+0000cdf0: 4222 5d3a 0a20 2020 2020 2020 2020 2020  B"]:.           
+0000ce00: 2073 656c 662e 766f 6963 655f 7374 7269   self.voice_stri
+0000ce10: 6e67 2873 656c 662e 7072 6f63 6573 735f  ng(self.process_
+0000ce20: 6d61 6372 6f28 7365 6c66 2e46 362e 746f  macro(self.F6.to
+0000ce30: 6f6c 5469 7028 2929 290a 2020 2020 2020  olTip())).      
+0000ce40: 2020 2020 2020 7265 7475 726e 0a20 2020        return.   
+0000ce50: 2020 2020 2069 6620 7365 6c66 2e63 773a       if self.cw:
+0000ce60: 0a20 2020 2020 2020 2020 2020 2073 656c  .            sel
+0000ce70: 662e 6377 2e73 656e 6463 7728 7365 6c66  f.cw.sendcw(self
+0000ce80: 2e70 726f 6365 7373 5f6d 6163 726f 2873  .process_macro(s
+0000ce90: 656c 662e 4636 2e74 6f6f 6c54 6970 2829  elf.F6.toolTip()
+0000cea0: 2929 0a0a 2020 2020 6465 6620 7365 6e64  ))..    def send
+0000ceb0: 6637 2873 656c 6629 3a0a 2020 2020 2020  f7(self):.      
+0000cec0: 2020 2222 2273 7475 6222 2222 0a20 2020    """stub""".   
+0000ced0: 2020 2020 206c 6f67 6765 722e 6465 6275       logger.debu
+0000cee0: 6728 2246 3720 436c 6963 6b65 6422 290a  g("F7 Clicked").
+0000cef0: 2020 2020 2020 2020 6966 2073 656c 662e          if self.
+0000cf00: 7261 6469 6f5f 7374 6174 652e 6765 7428  radio_state.get(
+0000cf10: 226d 6f64 6522 2920 696e 205b 224c 5342  "mode") in ["LSB
+0000cf20: 222c 2022 5553 4222 2c20 2253 5342 225d  ", "USB", "SSB"]
+0000cf30: 3a0a 2020 2020 2020 2020 2020 2020 7365  :.            se
+0000cf40: 6c66 2e76 6f69 6365 5f73 7472 696e 6728  lf.voice_string(
+0000cf50: 7365 6c66 2e70 726f 6365 7373 5f6d 6163  self.process_mac
+0000cf60: 726f 2873 656c 662e 4637 2e74 6f6f 6c54  ro(self.F7.toolT
+0000cf70: 6970 2829 2929 0a20 2020 2020 2020 2020  ip())).         
+0000cf80: 2020 2072 6574 7572 6e0a 2020 2020 2020     return.      
+0000cf90: 2020 6966 2073 656c 662e 6377 3a0a 2020    if self.cw:.  
+0000cfa0: 2020 2020 2020 2020 2020 7365 6c66 2e63            self.c
+0000cfb0: 772e 7365 6e64 6377 2873 656c 662e 7072  w.sendcw(self.pr
+0000cfc0: 6f63 6573 735f 6d61 6372 6f28 7365 6c66  ocess_macro(self
+0000cfd0: 2e46 372e 746f 6f6c 5469 7028 2929 290a  .F7.toolTip())).
+0000cfe0: 0a20 2020 2064 6566 2073 656e 6466 3828  .    def sendf8(
+0000cff0: 7365 6c66 293a 0a20 2020 2020 2020 2022  self):.        "
+0000d000: 2222 7374 7562 2222 220a 2020 2020 2020  ""stub""".      
+0000d010: 2020 6c6f 6767 6572 2e64 6562 7567 2822    logger.debug("
+0000d020: 4638 2043 6c69 636b 6564 2229 0a20 2020  F8 Clicked").   
+0000d030: 2020 2020 2069 6620 7365 6c66 2e72 6164       if self.rad
+0000d040: 696f 5f73 7461 7465 2e67 6574 2822 6d6f  io_state.get("mo
+0000d050: 6465 2229 2069 6e20 5b22 4c53 4222 2c20  de") in ["LSB", 
+0000d060: 2255 5342 222c 2022 5353 4222 5d3a 0a20  "USB", "SSB"]:. 
+0000d070: 2020 2020 2020 2020 2020 2073 656c 662e             self.
+0000d080: 766f 6963 655f 7374 7269 6e67 2873 656c  voice_string(sel
+0000d090: 662e 7072 6f63 6573 735f 6d61 6372 6f28  f.process_macro(
+0000d0a0: 7365 6c66 2e46 382e 746f 6f6c 5469 7028  self.F8.toolTip(
+0000d0b0: 2929 290a 2020 2020 2020 2020 2020 2020  ))).            
+0000d0c0: 7265 7475 726e 0a20 2020 2020 2020 2069  return.        i
+0000d0d0: 6620 7365 6c66 2e63 773a 0a20 2020 2020  f self.cw:.     
+0000d0e0: 2020 2020 2020 2073 656c 662e 6377 2e73         self.cw.s
+0000d0f0: 656e 6463 7728 7365 6c66 2e70 726f 6365  endcw(self.proce
+0000d100: 7373 5f6d 6163 726f 2873 656c 662e 4638  ss_macro(self.F8
+0000d110: 2e74 6f6f 6c54 6970 2829 2929 0a0a 2020  .toolTip()))..  
+0000d120: 2020 6465 6620 7365 6e64 6639 2873 656c    def sendf9(sel
+0000d130: 6629 3a0a 2020 2020 2020 2020 2222 2273  f):.        """s
+0000d140: 7475 6222 2222 0a20 2020 2020 2020 206c  tub""".        l
+0000d150: 6f67 6765 722e 6465 6275 6728 2246 3920  ogger.debug("F9 
+0000d160: 436c 6963 6b65 6422 290a 2020 2020 2020  Clicked").      
+0000d170: 2020 6966 2073 656c 662e 7261 6469 6f5f    if self.radio_
+0000d180: 7374 6174 652e 6765 7428 226d 6f64 6522  state.get("mode"
+0000d190: 2920 696e 205b 224c 5342 222c 2022 5553  ) in ["LSB", "US
+0000d1a0: 4222 2c20 2253 5342 225d 3a0a 2020 2020  B", "SSB"]:.    
+0000d1b0: 2020 2020 2020 2020 7365 6c66 2e76 6f69          self.voi
+0000d1c0: 6365 5f73 7472 696e 6728 7365 6c66 2e70  ce_string(self.p
+0000d1d0: 726f 6365 7373 5f6d 6163 726f 2873 656c  rocess_macro(sel
+0000d1e0: 662e 4639 2e74 6f6f 6c54 6970 2829 2929  f.F9.toolTip()))
+0000d1f0: 0a20 2020 2020 2020 2020 2020 2072 6574  .            ret
+0000d200: 7572 6e0a 2020 2020 2020 2020 6966 2073  urn.        if s
+0000d210: 656c 662e 6377 3a0a 2020 2020 2020 2020  elf.cw:.        
+0000d220: 2020 2020 7365 6c66 2e63 772e 7365 6e64      self.cw.send
+0000d230: 6377 2873 656c 662e 7072 6f63 6573 735f  cw(self.process_
+0000d240: 6d61 6372 6f28 7365 6c66 2e46 392e 746f  macro(self.F9.to
+0000d250: 6f6c 5469 7028 2929 290a 0a20 2020 2064  olTip()))..    d
+0000d260: 6566 2073 656e 6466 3130 2873 656c 6629  ef sendf10(self)
+0000d270: 3a0a 2020 2020 2020 2020 2222 2273 7475  :.        """stu
+0000d280: 6222 2222 0a20 2020 2020 2020 206c 6f67  b""".        log
+0000d290: 6765 722e 6465 6275 6728 2246 3130 2043  ger.debug("F10 C
+0000d2a0: 6c69 636b 6564 2229 0a20 2020 2020 2020  licked").       
+0000d2b0: 2069 6620 7365 6c66 2e72 6164 696f 5f73   if self.radio_s
+0000d2c0: 7461 7465 2e67 6574 2822 6d6f 6465 2229  tate.get("mode")
+0000d2d0: 2069 6e20 5b22 4c53 4222 2c20 2255 5342   in ["LSB", "USB
+0000d2e0: 222c 2022 5353 4222 5d3a 0a20 2020 2020  ", "SSB"]:.     
+0000d2f0: 2020 2020 2020 2073 656c 662e 766f 6963         self.voic
+0000d300: 655f 7374 7269 6e67 2873 656c 662e 7072  e_string(self.pr
+0000d310: 6f63 6573 735f 6d61 6372 6f28 7365 6c66  ocess_macro(self
+0000d320: 2e46 3130 2e74 6f6f 6c54 6970 2829 2929  .F10.toolTip()))
+0000d330: 0a20 2020 2020 2020 2020 2020 2072 6574  .            ret
+0000d340: 7572 6e0a 2020 2020 2020 2020 6966 2073  urn.        if s
+0000d350: 656c 662e 6377 3a0a 2020 2020 2020 2020  elf.cw:.        
+0000d360: 2020 2020 7365 6c66 2e63 772e 7365 6e64      self.cw.send
+0000d370: 6377 2873 656c 662e 7072 6f63 6573 735f  cw(self.process_
+0000d380: 6d61 6372 6f28 7365 6c66 2e46 3130 2e74  macro(self.F10.t
+0000d390: 6f6f 6c54 6970 2829 2929 0a0a 2020 2020  oolTip()))..    
+0000d3a0: 6465 6620 7365 6e64 6631 3128 7365 6c66  def sendf11(self
+0000d3b0: 293a 0a20 2020 2020 2020 2022 2222 7374  ):.        """st
+0000d3c0: 7562 2222 220a 2020 2020 2020 2020 6c6f  ub""".        lo
+0000d3d0: 6767 6572 2e64 6562 7567 2822 4631 3120  gger.debug("F11 
+0000d3e0: 436c 6963 6b65 6422 290a 2020 2020 2020  Clicked").      
+0000d3f0: 2020 6966 2073 656c 662e 7261 6469 6f5f    if self.radio_
+0000d400: 7374 6174 652e 6765 7428 226d 6f64 6522  state.get("mode"
+0000d410: 2920 696e 205b 224c 5342 222c 2022 5553  ) in ["LSB", "US
+0000d420: 4222 2c20 2253 5342 225d 3a0a 2020 2020  B", "SSB"]:.    
+0000d430: 2020 2020 2020 2020 7365 6c66 2e76 6f69          self.voi
+0000d440: 6365 5f73 7472 696e 6728 7365 6c66 2e70  ce_string(self.p
+0000d450: 726f 6365 7373 5f6d 6163 726f 2873 656c  rocess_macro(sel
+0000d460: 662e 4631 312e 746f 6f6c 5469 7028 2929  f.F11.toolTip())
+0000d470: 290a 2020 2020 2020 2020 2020 2020 7265  ).            re
+0000d480: 7475 726e 0a20 2020 2020 2020 2069 6620  turn.        if 
+0000d490: 7365 6c66 2e63 773a 0a20 2020 2020 2020  self.cw:.       
+0000d4a0: 2020 2020 2073 656c 662e 6377 2e73 656e       self.cw.sen
+0000d4b0: 6463 7728 7365 6c66 2e70 726f 6365 7373  dcw(self.process
+0000d4c0: 5f6d 6163 726f 2873 656c 662e 4631 312e  _macro(self.F11.
+0000d4d0: 746f 6f6c 5469 7028 2929 290a 0a20 2020  toolTip()))..   
+0000d4e0: 2064 6566 2073 656e 6466 3132 2873 656c   def sendf12(sel
+0000d4f0: 6629 3a0a 2020 2020 2020 2020 2222 2273  f):.        """s
+0000d500: 7475 6222 2222 0a20 2020 2020 2020 206c  tub""".        l
+0000d510: 6f67 6765 722e 6465 6275 6728 2246 3132  ogger.debug("F12
+0000d520: 2043 6c69 636b 6564 2229 0a20 2020 2020   Clicked").     
+0000d530: 2020 2069 6620 7365 6c66 2e72 6164 696f     if self.radio
+0000d540: 5f73 7461 7465 2e67 6574 2822 6d6f 6465  _state.get("mode
+0000d550: 2229 2069 6e20 5b22 4c53 4222 2c20 2255  ") in ["LSB", "U
+0000d560: 5342 222c 2022 5353 4222 5d3a 0a20 2020  SB", "SSB"]:.   
+0000d570: 2020 2020 2020 2020 2073 656c 662e 766f           self.vo
+0000d580: 6963 655f 7374 7269 6e67 2873 656c 662e  ice_string(self.
+0000d590: 7072 6f63 6573 735f 6d61 6372 6f28 7365  process_macro(se
+0000d5a0: 6c66 2e46 3132 2e74 6f6f 6c54 6970 2829  lf.F12.toolTip()
+0000d5b0: 2929 0a20 2020 2020 2020 2020 2020 2072  )).            r
+0000d5c0: 6574 7572 6e0a 2020 2020 2020 2020 6966  eturn.        if
+0000d5d0: 2073 656c 662e 6377 3a0a 2020 2020 2020   self.cw:.      
+0000d5e0: 2020 2020 2020 7365 6c66 2e63 772e 7365        self.cw.se
+0000d5f0: 6e64 6377 2873 656c 662e 7072 6f63 6573  ndcw(self.proces
+0000d600: 735f 6d61 6372 6f28 7365 6c66 2e46 3132  s_macro(self.F12
+0000d610: 2e74 6f6f 6c54 6970 2829 2929 0a0a 2020  .toolTip()))..  
+0000d620: 2020 6465 6620 7275 6e5f 7370 5f62 7574    def run_sp_but
+0000d630: 746f 6e73 5f63 6c69 636b 6564 2873 656c  tons_clicked(sel
+0000d640: 6629 3a0a 2020 2020 2020 2020 2222 2248  f):.        """H
+0000d650: 616e 646c 6520 7275 6e2f 7326 7020 6d6f  andle run/s&p mo
+0000d660: 6465 2222 220a 2020 2020 2020 2020 7365  de""".        se
+0000d670: 6c66 2e70 7265 665b 2272 756e 5f73 7461  lf.pref["run_sta
+0000d680: 7465 225d 203d 2073 656c 662e 7261 6469  te"] = self.radi
+0000d690: 6f42 7574 746f 6e5f 7275 6e2e 6973 4368  oButton_run.isCh
+0000d6a0: 6563 6b65 6428 290a 2020 2020 2020 2020  ecked().        
+0000d6b0: 7365 6c66 2e77 7269 7465 5f70 7265 6665  self.write_prefe
+0000d6c0: 7265 6e63 6528 290a 2020 2020 2020 2020  rence().        
+0000d6d0: 7365 6c66 2e72 6561 645f 6377 5f6d 6163  self.read_cw_mac
+0000d6e0: 726f 7328 290a 0a20 2020 2064 6566 2077  ros()..    def w
+0000d6f0: 7269 7465 5f70 7265 6665 7265 6e63 6528  rite_preference(
+0000d700: 7365 6c66 293a 0a20 2020 2020 2020 2022  self):.        "
+0000d710: 2222 0a20 2020 2020 2020 2057 7269 7465  "".        Write
+0000d720: 2070 7265 6665 7265 6e63 6573 2074 6f20   preferences to 
+0000d730: 6a73 6f6e 2066 696c 652e 0a20 2020 2020  json file..     
+0000d740: 2020 2022 2222 0a20 2020 2020 2020 2074     """.        t
+0000d750: 7279 3a0a 2020 2020 2020 2020 2020 2020  ry:.            
+0000d760: 7769 7468 206f 7065 6e28 0a20 2020 2020  with open(.     
+0000d770: 2020 2020 2020 2020 2020 2043 4f4e 4649             CONFI
+0000d780: 475f 5041 5448 202b 2022 2f6e 6f74 316d  G_PATH + "/not1m
+0000d790: 6d2e 6a73 6f6e 222c 2022 7774 222c 2065  m.json", "wt", e
+0000d7a0: 6e63 6f64 696e 673d 2275 7466 2d38 220a  ncoding="utf-8".
+0000d7b0: 2020 2020 2020 2020 2020 2020 2920 6173              ) as
+0000d7c0: 2066 696c 655f 6465 7363 7269 7074 6f72   file_descriptor
+0000d7d0: 3a0a 2020 2020 2020 2020 2020 2020 2020  :.              
+0000d7e0: 2020 6669 6c65 5f64 6573 6372 6970 746f    file_descripto
+0000d7f0: 722e 7772 6974 6528 6475 6d70 7328 7365  r.write(dumps(se
+0000d800: 6c66 2e70 7265 662c 2069 6e64 656e 743d  lf.pref, indent=
+0000d810: 3429 290a 2020 2020 2020 2020 2020 2020  4)).            
+0000d820: 2020 2020 6c6f 6767 6572 2e69 6e66 6f28      logger.info(
+0000d830: 2277 7269 7469 6e67 3a20 2573 222c 2073  "writing: %s", s
+0000d840: 656c 662e 7072 6566 290a 2020 2020 2020  elf.pref).      
+0000d850: 2020 6578 6365 7074 2049 4f45 7272 6f72    except IOError
+0000d860: 2061 7320 6578 6365 7074 696f 6e3a 0a20   as exception:. 
+0000d870: 2020 2020 2020 2020 2020 206c 6f67 6765             logge
+0000d880: 722e 6372 6974 6963 616c 2822 7772 6974  r.critical("writ
+0000d890: 6570 7265 6665 7265 6e63 6573 3a20 2573  epreferences: %s
+0000d8a0: 222c 2065 7863 6570 7469 6f6e 290a 0a20  ", exception).. 
+0000d8b0: 2020 2064 6566 2072 6561 6470 7265 6665     def readprefe
+0000d8c0: 7265 6e63 6573 2873 656c 6629 3a0a 2020  rences(self):.  
+0000d8d0: 2020 2020 2020 2222 220a 2020 2020 2020        """.      
+0000d8e0: 2020 5265 7374 6f72 6520 7072 6566 6572    Restore prefer
+0000d8f0: 656e 6365 7320 6966 2074 6865 7920 6578  ences if they ex
+0000d900: 6973 742c 206f 7468 6572 7769 7365 2063  ist, otherwise c
+0000d910: 7265 6174 6520 736f 6d65 2073 616e 6520  reate some sane 
+0000d920: 6465 6661 756c 7473 2e0a 2020 2020 2020  defaults..      
+0000d930: 2020 2222 220a 2020 2020 2020 2020 7472    """.        tr
+0000d940: 793a 0a20 2020 2020 2020 2020 2020 2069  y:.            i
+0000d950: 6620 6f73 2e70 6174 682e 6578 6973 7473  f os.path.exists
+0000d960: 2843 4f4e 4649 475f 5041 5448 202b 2022  (CONFIG_PATH + "
+0000d970: 2f6e 6f74 316d 6d2e 6a73 6f6e 2229 3a0a  /not1mm.json"):.
+0000d980: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000d990: 7769 7468 206f 7065 6e28 0a20 2020 2020  with open(.     
+0000d9a0: 2020 2020 2020 2020 2020 2020 2020 2043                 C
+0000d9b0: 4f4e 4649 475f 5041 5448 202b 2022 2f6e  ONFIG_PATH + "/n
+0000d9c0: 6f74 316d 6d2e 6a73 6f6e 222c 2022 7274  ot1mm.json", "rt
+0000d9d0: 222c 2065 6e63 6f64 696e 673d 2275 7466  ", encoding="utf
+0000d9e0: 2d38 220a 2020 2020 2020 2020 2020 2020  -8".            
+0000d9f0: 2020 2020 2920 6173 2066 696c 655f 6465      ) as file_de
+0000da00: 7363 7269 7074 6f72 3a0a 2020 2020 2020  scriptor:.      
+0000da10: 2020 2020 2020 2020 2020 2020 2020 7365                se
+0000da20: 6c66 2e70 7265 6620 3d20 6c6f 6164 7328  lf.pref = loads(
+0000da30: 6669 6c65 5f64 6573 6372 6970 746f 722e  file_descriptor.
+0000da40: 7265 6164 2829 290a 2020 2020 2020 2020  read()).        
+0000da50: 2020 2020 2020 2020 2020 2020 6c6f 6767              logg
+0000da60: 6572 2e69 6e66 6f28 2225 7322 2c20 7365  er.info("%s", se
+0000da70: 6c66 2e70 7265 6629 0a20 2020 2020 2020  lf.pref).       
+0000da80: 2020 2020 2065 6c73 653a 0a20 2020 2020       else:.     
+0000da90: 2020 2020 2020 2020 2020 206c 6f67 6765             logge
+0000daa0: 722e 696e 666f 2822 4e6f 2070 7265 6665  r.info("No prefe
+0000dab0: 7265 6e63 6520 6669 6c65 2e20 5772 6974  rence file. Writ
+0000dac0: 696e 6720 7072 6566 6572 656e 6365 2e22  ing preference."
+0000dad0: 290a 2020 2020 2020 2020 2020 2020 2020  ).              
+0000dae0: 2020 7769 7468 206f 7065 6e28 0a20 2020    with open(.   
+0000daf0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000db00: 2043 4f4e 4649 475f 5041 5448 202b 2022   CONFIG_PATH + "
+0000db10: 2f6e 6f74 316d 6d2e 6a73 6f6e 222c 2022  /not1mm.json", "
+0000db20: 7774 222c 2065 6e63 6f64 696e 673d 2275  wt", encoding="u
+0000db30: 7466 2d38 220a 2020 2020 2020 2020 2020  tf-8".          
+0000db40: 2020 2020 2020 2920 6173 2066 696c 655f        ) as file_
+0000db50: 6465 7363 7269 7074 6f72 3a0a 2020 2020  descriptor:.    
+0000db60: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000db70: 7365 6c66 2e70 7265 6620 3d20 7365 6c66  self.pref = self
+0000db80: 2e70 7265 665f 7265 662e 636f 7079 2829  .pref_ref.copy()
+0000db90: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+0000dba0: 2020 2020 2066 696c 655f 6465 7363 7269       file_descri
+0000dbb0: 7074 6f72 2e77 7269 7465 2864 756d 7073  ptor.write(dumps
+0000dbc0: 2873 656c 662e 7072 6566 2c20 696e 6465  (self.pref, inde
+0000dbd0: 6e74 3d34 2929 0a20 2020 2020 2020 2020  nt=4)).         
+0000dbe0: 2020 2020 2020 2020 2020 206c 6f67 6765             logge
+0000dbf0: 722e 696e 666f 2822 2573 222c 2073 656c  r.info("%s", sel
+0000dc00: 662e 7072 6566 290a 2020 2020 2020 2020  f.pref).        
+0000dc10: 6578 6365 7074 2049 4f45 7272 6f72 2061  except IOError a
+0000dc20: 7320 6578 6365 7074 696f 6e3a 0a20 2020  s exception:.   
+0000dc30: 2020 2020 2020 2020 206c 6f67 6765 722e           logger.
+0000dc40: 6372 6974 6963 616c 2822 4572 726f 723a  critical("Error:
+0000dc50: 2025 7322 2c20 6578 6365 7074 696f 6e29   %s", exception)
+0000dc60: 0a0a 2020 2020 2020 2020 7365 6c66 2e6c  ..        self.l
+0000dc70: 6f6f 6b5f 7570 203d 204e 6f6e 650a 2020  ook_up = None.  
+0000dc80: 2020 2020 2020 6966 2073 656c 662e 7072        if self.pr
+0000dc90: 6566 2e67 6574 2822 7573 6571 727a 2229  ef.get("useqrz")
+0000dca0: 3a0a 2020 2020 2020 2020 2020 2020 7365  :.            se
+0000dcb0: 6c66 2e6c 6f6f 6b5f 7570 203d 2051 525a  lf.look_up = QRZ
+0000dcc0: 6c6f 6f6b 7570 280a 2020 2020 2020 2020  lookup(.        
+0000dcd0: 2020 2020 2020 2020 7365 6c66 2e70 7265          self.pre
+0000dce0: 662e 6765 7428 226c 6f6f 6b75 7075 7365  f.get("lookupuse
+0000dcf0: 726e 616d 6522 292c 0a20 2020 2020 2020  rname"),.       
+0000dd00: 2020 2020 2020 2020 2073 656c 662e 7072           self.pr
+0000dd10: 6566 2e67 6574 2822 6c6f 6f6b 7570 7061  ef.get("lookuppa
+0000dd20: 7373 776f 7264 2229 2c0a 2020 2020 2020  ssword"),.      
+0000dd30: 2020 2020 2020 290a 2020 2020 2020 2020        ).        
+0000dd40: 2320 6966 2073 656c 662e 7072 6566 2e67  # if self.pref.g
+0000dd50: 6574 2822 7573 6568 616d 6462 2229 3a0a  et("usehamdb"):.
+0000dd60: 2020 2020 2020 2020 2320 2020 2020 7365          #     se
+0000dd70: 6c66 2e6c 6f6f 6b5f 7570 203d 2048 616d  lf.look_up = Ham
+0000dd80: 4442 6c6f 6f6b 7570 2829 0a20 2020 2020  DBlookup().     
+0000dd90: 2020 2069 6620 7365 6c66 2e70 7265 662e     if self.pref.
+0000dda0: 6765 7428 2275 7365 6861 6d71 7468 2229  get("usehamqth")
+0000ddb0: 3a0a 2020 2020 2020 2020 2020 2020 7365  :.            se
+0000ddc0: 6c66 2e6c 6f6f 6b5f 7570 203d 2048 616d  lf.look_up = Ham
+0000ddd0: 5154 4828 0a20 2020 2020 2020 2020 2020  QTH(.           
+0000dde0: 2020 2020 2073 656c 662e 7072 6566 2e67       self.pref.g
+0000ddf0: 6574 2822 6c6f 6f6b 7570 7573 6572 6e61  et("lookupuserna
+0000de00: 6d65 2229 2c0a 2020 2020 2020 2020 2020  me"),.          
+0000de10: 2020 2020 2020 7365 6c66 2e70 7265 662e        self.pref.
+0000de20: 6765 7428 226c 6f6f 6b75 7070 6173 7377  get("lookuppassw
+0000de30: 6f72 6422 292c 0a20 2020 2020 2020 2020  ord"),.         
+0000de40: 2020 2029 0a0a 2020 2020 2020 2020 6966     )..        if
+0000de50: 2073 656c 662e 7072 6566 2e67 6574 2822   self.pref.get("
+0000de60: 7275 6e5f 7374 6174 6522 293a 0a20 2020  run_state"):.   
+0000de70: 2020 2020 2020 2020 2073 656c 662e 7261           self.ra
+0000de80: 6469 6f42 7574 746f 6e5f 7275 6e2e 7365  dioButton_run.se
+0000de90: 7443 6865 636b 6564 2854 7275 6529 0a20  tChecked(True). 
+0000dea0: 2020 2020 2020 2065 6c73 653a 0a20 2020         else:.   
+0000deb0: 2020 2020 2020 2020 2073 656c 662e 7261           self.ra
+0000dec0: 6469 6f42 7574 746f 6e5f 7370 2e73 6574  dioButton_sp.set
+0000ded0: 4368 6563 6b65 6428 5472 7565 290a 0a20  Checked(True).. 
+0000dee0: 2020 2020 2020 2069 6620 7365 6c66 2e70         if self.p
+0000def0: 7265 662e 6765 7428 2264 6172 6b5f 6d6f  ref.get("dark_mo
+0000df00: 6465 2229 3a0a 2020 2020 2020 2020 2020  de"):.          
+0000df10: 2020 7365 6c66 2e61 6374 696f 6e44 6172    self.actionDar
+0000df20: 6b5f 4d6f 6465 2e73 6574 4368 6563 6b65  k_Mode.setChecke
+0000df30: 6428 5472 7565 290a 2020 2020 2020 2020  d(True).        
+0000df40: 656c 7365 3a0a 2020 2020 2020 2020 2020  else:.          
+0000df50: 2020 7365 6c66 2e61 6374 696f 6e44 6172    self.actionDar
+0000df60: 6b5f 4d6f 6465 2e73 6574 4368 6563 6b65  k_Mode.setChecke
+0000df70: 6428 4661 6c73 6529 0a0a 2020 2020 2020  d(False)..      
+0000df80: 2020 6966 2073 656c 662e 7072 6566 2e67    if self.pref.g
+0000df90: 6574 2822 636f 6d6d 616e 645f 6275 7474  et("command_butt
+0000dfa0: 6f6e 7322 293a 0a20 2020 2020 2020 2020  ons"):.         
+0000dfb0: 2020 2073 656c 662e 6163 7469 6f6e 436f     self.actionCo
+0000dfc0: 6d6d 616e 645f 4275 7474 6f6e 732e 7365  mmand_Buttons.se
+0000dfd0: 7443 6865 636b 6564 2854 7275 6529 0a20  tChecked(True). 
+0000dfe0: 2020 2020 2020 2065 6c73 653a 0a20 2020         else:.   
+0000dff0: 2020 2020 2020 2020 2073 656c 662e 6163           self.ac
+0000e000: 7469 6f6e 436f 6d6d 616e 645f 4275 7474  tionCommand_Butt
+0000e010: 6f6e 732e 7365 7443 6865 636b 6564 2846  ons.setChecked(F
+0000e020: 616c 7365 290a 0a20 2020 2020 2020 2069  alse)..        i
+0000e030: 6620 7365 6c66 2e70 7265 662e 6765 7428  f self.pref.get(
+0000e040: 2263 775f 6d61 6372 6f73 2229 3a0a 2020  "cw_macros"):.  
+0000e050: 2020 2020 2020 2020 2020 7365 6c66 2e61            self.a
+0000e060: 6374 696f 6e43 575f 4d61 6372 6f73 2e73  ctionCW_Macros.s
+0000e070: 6574 4368 6563 6b65 6428 5472 7565 290a  etChecked(True).
+0000e080: 2020 2020 2020 2020 656c 7365 3a0a 2020          else:.  
+0000e090: 2020 2020 2020 2020 2020 7365 6c66 2e61            self.a
+0000e0a0: 6374 696f 6e43 575f 4d61 6372 6f73 2e73  ctionCW_Macros.s
+0000e0b0: 6574 4368 6563 6b65 6428 4661 6c73 6529  etChecked(False)
+0000e0c0: 0a0a 2020 2020 2020 2020 6966 2073 656c  ..        if sel
+0000e0d0: 662e 7072 6566 2e67 6574 2822 6261 6e64  f.pref.get("band
+0000e0e0: 735f 6d6f 6465 7322 293a 0a20 2020 2020  s_modes"):.     
+0000e0f0: 2020 2020 2020 2073 656c 662e 6163 7469         self.acti
+0000e100: 6f6e 4d6f 6465 5f61 6e64 5f42 616e 6473  onMode_and_Bands
+0000e110: 2e73 6574 4368 6563 6b65 6428 5472 7565  .setChecked(True
+0000e120: 290a 2020 2020 2020 2020 656c 7365 3a0a  ).        else:.
+0000e130: 2020 2020 2020 2020 2020 2020 7365 6c66              self
+0000e140: 2e61 6374 696f 6e4d 6f64 655f 616e 645f  .actionMode_and_
+0000e150: 4261 6e64 732e 7365 7443 6865 636b 6564  Bands.setChecked
+0000e160: 2846 616c 7365 290a 0a20 2020 2020 2020  (False)..       
+0000e170: 206d 756c 7469 6361 7374 5f67 726f 7570   multicast_group
+0000e180: 203d 2073 656c 662e 7072 6566 2e67 6574   = self.pref.get
+0000e190: 2822 6d75 6c74 6963 6173 745f 6772 6f75  ("multicast_grou
+0000e1a0: 7022 2c20 2232 3234 2e31 2e31 2e31 2229  p", "224.1.1.1")
+0000e1b0: 0a20 2020 2020 2020 206d 756c 7469 6361  .        multica
+0000e1c0: 7374 5f70 6f72 7420 3d20 7365 6c66 2e70  st_port = self.p
+0000e1d0: 7265 662e 6765 7428 226d 756c 7469 6361  ref.get("multica
+0000e1e0: 7374 5f70 6f72 7422 2c20 3232 3339 290a  st_port", 2239).
+0000e1f0: 2020 2020 2020 2020 696e 7465 7266 6163          interfac
+0000e200: 655f 6970 203d 2073 656c 662e 7072 6566  e_ip = self.pref
+0000e210: 2e67 6574 2822 696e 7465 7266 6163 655f  .get("interface_
+0000e220: 6970 222c 2022 302e 302e 302e 3022 290a  ip", "0.0.0.0").
+0000e230: 2020 2020 2020 2020 7365 6c66 2e6d 756c          self.mul
+0000e240: 7469 6361 7374 5f69 6e74 6572 6661 6365  ticast_interface
+0000e250: 203d 204d 756c 7469 6361 7374 280a 2020   = Multicast(.  
+0000e260: 2020 2020 2020 2020 2020 6d75 6c74 6963            multic
+0000e270: 6173 745f 6772 6f75 702c 206d 756c 7469  ast_group, multi
+0000e280: 6361 7374 5f70 6f72 742c 2069 6e74 6572  cast_port, inter
+0000e290: 6661 6365 5f69 700a 2020 2020 2020 2020  face_ip.        
+0000e2a0: 290a 0a20 2020 2020 2020 2073 656c 662e  )..        self.
+0000e2b0: 7269 675f 636f 6e74 726f 6c20 3d20 4e6f  rig_control = No
+0000e2c0: 6e65 0a0a 2020 2020 2020 2020 6966 2073  ne..        if s
+0000e2d0: 656c 662e 7072 6566 2e67 6574 2822 7573  elf.pref.get("us
+0000e2e0: 6566 6c72 6967 222c 2046 616c 7365 293a  eflrig", False):
+0000e2f0: 0a20 2020 2020 2020 2020 2020 206c 6f67  .            log
+0000e300: 6765 722e 6465 6275 6728 0a20 2020 2020  ger.debug(.     
+0000e310: 2020 2020 2020 2020 2020 2022 5573 696e             "Usin
+0000e320: 6720 666c 7269 673a 2025 7322 2c0a 2020  g flrig: %s",.  
+0000e330: 2020 2020 2020 2020 2020 2020 2020 6622                f"
+0000e340: 7b73 656c 662e 7072 6566 2e67 6574 2827  {self.pref.get('
+0000e350: 4341 545f 6970 2729 7d20 7b73 656c 662e  CAT_ip')} {self.
+0000e360: 7072 6566 2e67 6574 2827 4341 545f 706f  pref.get('CAT_po
+0000e370: 7274 2729 7d22 2c0a 2020 2020 2020 2020  rt')}",.        
+0000e380: 2020 2020 290a 2020 2020 2020 2020 2020      ).          
+0000e390: 2020 7365 6c66 2e72 6967 5f63 6f6e 7472    self.rig_contr
+0000e3a0: 6f6c 203d 2043 4154 280a 2020 2020 2020  ol = CAT(.      
+0000e3b0: 2020 2020 2020 2020 2020 2266 6c72 6967            "flrig
+0000e3c0: 222c 0a20 2020 2020 2020 2020 2020 2020  ",.             
+0000e3d0: 2020 2073 656c 662e 7072 6566 2e67 6574     self.pref.get
+0000e3e0: 2822 4341 545f 6970 222c 2022 3132 372e  ("CAT_ip", "127.
+0000e3f0: 302e 302e 3122 292c 0a20 2020 2020 2020  0.0.1"),.       
+0000e400: 2020 2020 2020 2020 2069 6e74 2873 656c           int(sel
+0000e410: 662e 7072 6566 2e67 6574 2822 4341 545f  f.pref.get("CAT_
+0000e420: 706f 7274 222c 2031 3233 3435 2929 2c0a  port", 12345)),.
+0000e430: 2020 2020 2020 2020 2020 2020 290a 2020              ).  
+0000e440: 2020 2020 2020 6966 2073 656c 662e 7072        if self.pr
+0000e450: 6566 2e67 6574 2822 7573 6572 6967 6374  ef.get("userigct
+0000e460: 6c64 222c 2046 616c 7365 293a 0a20 2020  ld", False):.   
+0000e470: 2020 2020 2020 2020 206c 6f67 6765 722e           logger.
+0000e480: 6465 6275 6728 0a20 2020 2020 2020 2020  debug(.         
+0000e490: 2020 2020 2020 2022 5573 696e 6720 7269         "Using ri
+0000e4a0: 6763 746c 643a 2025 7322 2c0a 2020 2020  gctld: %s",.    
+0000e4b0: 2020 2020 2020 2020 2020 2020 6622 7b73              f"{s
+0000e4c0: 656c 662e 7072 6566 2e67 6574 2827 4341  elf.pref.get('CA
+0000e4d0: 545f 6970 2729 7d20 7b73 656c 662e 7072  T_ip')} {self.pr
+0000e4e0: 6566 2e67 6574 2827 4341 545f 706f 7274  ef.get('CAT_port
+0000e4f0: 2729 7d22 2c0a 2020 2020 2020 2020 2020  ')}",.          
+0000e500: 2020 290a 2020 2020 2020 2020 2020 2020    ).            
+0000e510: 7365 6c66 2e72 6967 5f63 6f6e 7472 6f6c  self.rig_control
+0000e520: 203d 2043 4154 280a 2020 2020 2020 2020   = CAT(.        
+0000e530: 2020 2020 2020 2020 2272 6967 6374 6c64          "rigctld
+0000e540: 222c 0a20 2020 2020 2020 2020 2020 2020  ",.             
+0000e550: 2020 2073 656c 662e 7072 6566 2e67 6574     self.pref.get
+0000e560: 2822 4341 545f 6970 222c 2022 3132 372e  ("CAT_ip", "127.
+0000e570: 302e 302e 3122 292c 0a20 2020 2020 2020  0.0.1"),.       
+0000e580: 2020 2020 2020 2020 2069 6e74 2873 656c           int(sel
+0000e590: 662e 7072 6566 2e67 6574 2822 4341 545f  f.pref.get("CAT_
+0000e5a0: 706f 7274 222c 2034 3533 3229 292c 0a20  port", 4532)),. 
+0000e5b0: 2020 2020 2020 2020 2020 2029 0a0a 2020             )..  
+0000e5c0: 2020 2020 2020 6966 2073 656c 662e 7072        if self.pr
+0000e5d0: 6566 2e67 6574 2822 6377 7479 7065 222c  ef.get("cwtype",
+0000e5e0: 2030 2920 3d3d 2030 3a0a 2020 2020 2020   0) == 0:.      
+0000e5f0: 2020 2020 2020 7365 6c66 2e63 7720 3d20        self.cw = 
+0000e600: 4e6f 6e65 0a20 2020 2020 2020 2065 6c73  None.        els
+0000e610: 653a 0a20 2020 2020 2020 2020 2020 2073  e:.            s
+0000e620: 656c 662e 6377 203d 2043 5728 0a20 2020  elf.cw = CW(.   
+0000e630: 2020 2020 2020 2020 2020 2020 2069 6e74               int
+0000e640: 2873 656c 662e 7072 6566 2e67 6574 2822  (self.pref.get("
+0000e650: 6377 7479 7065 2229 292c 0a20 2020 2020  cwtype")),.     
+0000e660: 2020 2020 2020 2020 2020 2073 656c 662e             self.
+0000e670: 7072 6566 2e67 6574 2822 6377 6970 2229  pref.get("cwip")
+0000e680: 2c0a 2020 2020 2020 2020 2020 2020 2020  ,.              
+0000e690: 2020 696e 7428 7365 6c66 2e70 7265 662e    int(self.pref.
+0000e6a0: 6765 7428 2263 7770 6f72 7422 2c20 3637  get("cwport", 67
+0000e6b0: 3839 2929 2c0a 2020 2020 2020 2020 2020  89)),.          
+0000e6c0: 2020 290a 2020 2020 2020 2020 2020 2020    ).            
+0000e6d0: 7365 6c66 2e63 772e 7370 6565 6420 3d20  self.cw.speed = 
+0000e6e0: 3230 0a0a 2020 2020 2020 2020 7365 6c66  20..        self
+0000e6f0: 2e64 6172 6b5f 6d6f 6465 2829 0a20 2020  .dark_mode().   
+0000e700: 2020 2020 2073 656c 662e 7368 6f77 5f63       self.show_c
+0000e710: 6f6d 6d61 6e64 5f62 7574 746f 6e73 2829  ommand_buttons()
+0000e720: 0a20 2020 2020 2020 2073 656c 662e 7368  .        self.sh
+0000e730: 6f77 5f43 575f 6d61 6372 6f73 2829 0a20  ow_CW_macros(). 
+0000e740: 2020 2020 2020 2023 2073 656c 662e 7368         # self.sh
+0000e750: 6f77 5f62 616e 645f 6d6f 6465 2829 0a0a  ow_band_mode()..
+0000e760: 2020 2020 6465 6620 7761 7463 685f 7564      def watch_ud
+0000e770: 7028 7365 6c66 293a 0a20 2020 2020 2020  p(self):.       
+0000e780: 2022 2222 5075 7473 2055 4450 2064 6174   """Puts UDP dat
+0000e790: 6167 7261 6d73 2069 6e20 6120 4649 464f  agrams in a FIFO
+0000e7a0: 2071 7565 7565 2222 220a 2020 2020 2020   queue""".      
+0000e7b0: 2020 7768 696c 6520 5472 7565 3a0a 2020    while True:.  
+0000e7c0: 2020 2020 2020 2020 2020 7472 793a 0a20            try:. 
+0000e7d0: 2020 2020 2020 2020 2020 2020 2020 2064                 d
+0000e7e0: 6174 6167 7261 6d20 3d20 7365 6c66 2e6d  atagram = self.m
+0000e7f0: 756c 7469 6361 7374 5f69 6e74 6572 6661  ulticast_interfa
+0000e800: 6365 2e73 6572 7665 725f 7564 702e 7265  ce.server_udp.re
+0000e810: 6376 2831 3530 3029 0a20 2020 2020 2020  cv(1500).       
+0000e820: 2020 2020 2020 2020 206c 6f67 6765 722e           logger.
+0000e830: 6465 6275 6728 6461 7461 6772 616d 2e64  debug(datagram.d
+0000e840: 6563 6f64 6528 2929 0a20 2020 2020 2020  ecode()).       
+0000e850: 2020 2020 2065 7863 6570 7420 736f 636b       except sock
+0000e860: 6574 2e74 696d 656f 7574 3a0a 2020 2020  et.timeout:.    
+0000e870: 2020 2020 2020 2020 2020 2020 7469 6d65              time
+0000e880: 2e73 6c65 6570 2830 2e31 290a 2020 2020  .sleep(0.1).    
+0000e890: 2020 2020 2020 2020 2020 2020 636f 6e74              cont
+0000e8a0: 696e 7565 0a20 2020 2020 2020 2020 2020  inue.           
+0000e8b0: 2069 6620 6461 7461 6772 616d 3a0a 2020   if datagram:.  
+0000e8c0: 2020 2020 2020 2020 2020 2020 2020 7365                se
+0000e8d0: 6c66 2e75 6470 5f66 6966 6f2e 7075 7428  lf.udp_fifo.put(
+0000e8e0: 6461 7461 6772 616d 290a 0a20 2020 2064  datagram)..    d
+0000e8f0: 6566 2063 6865 636b 5f75 6470 5f74 7261  ef check_udp_tra
+0000e900: 6666 6963 2873 656c 6629 3a0a 2020 2020  ffic(self):.    
+0000e910: 2020 2020 2222 2243 6865 636b 7320 5544      """Checks UD
+0000e920: 5020 5472 6166 6669 6322 2222 0a20 2020  P Traffic""".   
+0000e930: 2020 2020 2077 6869 6c65 206e 6f74 2073       while not s
+0000e940: 656c 662e 7564 705f 6669 666f 2e65 6d70  elf.udp_fifo.emp
+0000e950: 7479 2829 3a0a 2020 2020 2020 2020 2020  ty():.          
+0000e960: 2020 6461 7461 6772 616d 203d 2073 656c    datagram = sel
+0000e970: 662e 7564 705f 6669 666f 2e67 6574 2829  f.udp_fifo.get()
+0000e980: 0a20 2020 2020 2020 2020 2020 2074 7279  .            try
+0000e990: 3a0a 2020 2020 2020 2020 2020 2020 2020  :.              
+0000e9a0: 2020 6465 6275 675f 696e 666f 203d 2066    debug_info = f
+0000e9b0: 227b 6461 7461 6772 616d 2e64 6563 6f64  "{datagram.decod
+0000e9c0: 6528 297d 220a 2020 2020 2020 2020 2020  e()}".          
+0000e9d0: 2020 2020 2020 6c6f 6767 6572 2e64 6562        logger.deb
+0000e9e0: 7567 2864 6562 7567 5f69 6e66 6f29 0a20  ug(debug_info). 
+0000e9f0: 2020 2020 2020 2020 2020 2020 2020 206a                 j
+0000ea00: 736f 6e5f 6461 7461 203d 206c 6f61 6473  son_data = loads
+0000ea10: 2864 6174 6167 7261 6d2e 6465 636f 6465  (datagram.decode
+0000ea20: 2829 290a 2020 2020 2020 2020 2020 2020  ()).            
+0000ea30: 6578 6365 7074 2055 6e69 636f 6465 4465  except UnicodeDe
+0000ea40: 636f 6465 4572 726f 7220 6173 2065 7272  codeError as err
+0000ea50: 3a0a 2020 2020 2020 2020 2020 2020 2020  :.              
+0000ea60: 2020 7468 655f 6572 726f 7220 3d20 6622    the_error = f"
+0000ea70: 4e6f 7420 556e 6963 6f64 653a 207b 6572  Not Unicode: {er
+0000ea80: 727d 5c6e 7b64 6174 6167 7261 6d7d 220a  r}\n{datagram}".
+0000ea90: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000eaa0: 6c6f 6767 6572 2e64 6562 7567 2874 6865  logger.debug(the
+0000eab0: 5f65 7272 6f72 290a 2020 2020 2020 2020  _error).        
+0000eac0: 2020 2020 2020 2020 636f 6e74 696e 7565          continue
+0000ead0: 0a20 2020 2020 2020 2020 2020 2065 7863  .            exc
+0000eae0: 6570 7420 4a53 4f4e 4465 636f 6465 4572  ept JSONDecodeEr
+0000eaf0: 726f 7220 6173 2065 7272 3a0a 2020 2020  ror as err:.    
+0000eb00: 2020 2020 2020 2020 2020 2020 7468 655f              the_
+0000eb10: 6572 726f 7220 3d20 6622 4e6f 7420 4a53  error = f"Not JS
+0000eb20: 4f4e 3a20 7b65 7272 7d5c 6e7b 6461 7461  ON: {err}\n{data
+0000eb30: 6772 616d 7d22 0a20 2020 2020 2020 2020  gram}".         
+0000eb40: 2020 2020 2020 206c 6f67 6765 722e 6465         logger.de
+0000eb50: 6275 6728 7468 655f 6572 726f 7229 0a20  bug(the_error). 
+0000eb60: 2020 2020 2020 2020 2020 2020 2020 2063                 c
+0000eb70: 6f6e 7469 6e75 650a 2020 2020 2020 2020  ontinue.        
+0000eb80: 2020 2020 6966 2028 0a20 2020 2020 2020      if (.       
+0000eb90: 2020 2020 2020 2020 206a 736f 6e5f 6461           json_da
+0000eba0: 7461 2e67 6574 2822 636d 6422 2c20 2222  ta.get("cmd", ""
+0000ebb0: 2920 3d3d 2022 4745 5443 4f4c 554d 4e53  ) == "GETCOLUMNS
+0000ebc0: 220a 2020 2020 2020 2020 2020 2020 2020  ".              
+0000ebd0: 2020 616e 6420 6a73 6f6e 5f64 6174 612e    and json_data.
+0000ebe0: 6765 7428 2273 7461 7469 6f6e 222c 2022  get("station", "
+0000ebf0: 2229 203d 3d20 706c 6174 666f 726d 2e6e  ") == platform.n
+0000ec00: 6f64 6528 290a 2020 2020 2020 2020 2020  ode().          
+0000ec10: 2020 293a 0a20 2020 2020 2020 2020 2020    ):.           
+0000ec20: 2020 2020 2069 6620 6861 7361 7474 7228       if hasattr(
+0000ec30: 7365 6c66 2e63 6f6e 7465 7374 2c20 2263  self.contest, "c
+0000ec40: 6f6c 756d 6e73 2229 3a0a 2020 2020 2020  olumns"):.      
+0000ec50: 2020 2020 2020 2020 2020 2020 2020 636d                cm
+0000ec60: 6420 3d20 7b7d 0a20 2020 2020 2020 2020  d = {}.         
+0000ec70: 2020 2020 2020 2020 2020 2063 6d64 5b22             cmd["
+0000ec80: 636d 6422 5d20 3d20 2253 484f 5743 4f4c  cmd"] = "SHOWCOL
+0000ec90: 554d 4e53 220a 2020 2020 2020 2020 2020  UMNS".          
+0000eca0: 2020 2020 2020 2020 2020 636d 645b 2273            cmd["s
+0000ecb0: 7461 7469 6f6e 225d 203d 2070 6c61 7466  tation"] = platf
+0000ecc0: 6f72 6d2e 6e6f 6465 2829 0a20 2020 2020  orm.node().     
+0000ecd0: 2020 2020 2020 2020 2020 2020 2020 2063                 c
+0000ece0: 6d64 5b22 434f 4c55 4d4e 5322 5d20 3d20  md["COLUMNS"] = 
+0000ecf0: 7365 6c66 2e63 6f6e 7465 7374 2e63 6f6c  self.contest.col
+0000ed00: 756d 6e73 0a20 2020 2020 2020 2020 2020  umns.           
+0000ed10: 2020 2020 2020 2020 2073 656c 662e 6d75           self.mu
+0000ed20: 6c74 6963 6173 745f 696e 7465 7266 6163  lticast_interfac
+0000ed30: 652e 7365 6e64 5f61 735f 6a73 6f6e 2863  e.send_as_json(c
+0000ed40: 6d64 290a 2020 2020 2020 2020 2020 2020  md).            
+0000ed50: 6966 2028 0a20 2020 2020 2020 2020 2020  if (.           
+0000ed60: 2020 2020 206a 736f 6e5f 6461 7461 2e67       json_data.g
+0000ed70: 6574 2822 636d 6422 2c20 2222 2920 3d3d  et("cmd", "") ==
+0000ed80: 2022 5455 4e45 220a 2020 2020 2020 2020   "TUNE".        
+0000ed90: 2020 2020 2020 2020 616e 6420 6a73 6f6e          and json
+0000eda0: 5f64 6174 612e 6765 7428 2273 7461 7469  _data.get("stati
+0000edb0: 6f6e 222c 2022 2229 203d 3d20 706c 6174  on", "") == plat
+0000edc0: 666f 726d 2e6e 6f64 6528 290a 2020 2020  form.node().    
+0000edd0: 2020 2020 2020 2020 293a 0a20 2020 2020          ):.     
+0000ede0: 2020 2020 2020 2020 2020 2023 2062 277b             # b'{
+0000edf0: 2263 6d64 223a 2022 5455 4e45 222c 2022  "cmd": "TUNE", "
+0000ee00: 6672 6571 223a 2037 2e30 3233 352c 2022  freq": 7.0235, "
+0000ee10: 7370 6f74 223a 2022 4d4d 3044 4749 227d  spot": "MM0DGI"}
+0000ee20: 270a 2020 2020 2020 2020 2020 2020 2020  '.              
+0000ee30: 2020 7666 6f20 3d20 6a73 6f6e 5f64 6174    vfo = json_dat
+0000ee40: 612e 6765 7428 2266 7265 7122 290a 2020  a.get("freq").  
+0000ee50: 2020 2020 2020 2020 2020 2020 2020 7666                vf
+0000ee60: 6f20 3d20 666c 6f61 7428 7666 6f29 202a  o = float(vfo) *
+0000ee70: 2031 3030 3030 3030 0a20 2020 2020 2020   1000000.       
+0000ee80: 2020 2020 2020 2020 2073 656c 662e 7261           self.ra
+0000ee90: 6469 6f5f 7374 6174 655b 2276 666f 6122  dio_state["vfoa"
+0000eea0: 5d20 3d20 696e 7428 7666 6f29 0a20 2020  ] = int(vfo).   
+0000eeb0: 2020 2020 2020 2020 2020 2020 2069 6620               if 
+0000eec0: 7365 6c66 2e72 6967 5f63 6f6e 7472 6f6c  self.rig_control
+0000eed0: 3a0a 2020 2020 2020 2020 2020 2020 2020  :.              
+0000eee0: 2020 2020 2020 7365 6c66 2e72 6967 5f63        self.rig_c
+0000eef0: 6f6e 7472 6f6c 2e73 6574 5f76 666f 2869  ontrol.set_vfo(i
+0000ef00: 6e74 2876 666f 2929 0a20 2020 2020 2020  nt(vfo)).       
+0000ef10: 2020 2020 2020 2020 2073 706f 7420 3d20           spot = 
+0000ef20: 6a73 6f6e 5f64 6174 612e 6765 7428 2273  json_data.get("s
+0000ef30: 706f 7422 2c20 2222 290a 2020 2020 2020  pot", "").      
+0000ef40: 2020 2020 2020 2020 2020 7365 6c66 2e63            self.c
+0000ef50: 616c 6c73 6967 6e2e 7365 7454 6578 7428  allsign.setText(
+0000ef60: 7370 6f74 290a 2020 2020 2020 2020 2020  spot).          
+0000ef70: 2020 2020 2020 7365 6c66 2e63 616c 6c73        self.calls
+0000ef80: 6967 6e5f 6368 616e 6765 6428 290a 2020  ign_changed().  
+0000ef90: 2020 2020 2020 2020 2020 2020 2020 7365                se
+0000efa0: 6c66 2e63 616c 6c73 6967 6e2e 7365 7446  lf.callsign.setF
+0000efb0: 6f63 7573 2829 0a20 2020 2020 2020 2020  ocus().         
+0000efc0: 2020 2020 2020 2073 656c 662e 6361 6c6c         self.call
+0000efd0: 7369 676e 2e61 6374 6976 6174 6557 696e  sign.activateWin
+0000efe0: 646f 7728 290a 2020 2020 2020 2020 2020  dow().          
+0000eff0: 2020 2020 2020 7769 6e64 6f77 2e72 6169        window.rai
+0000f000: 7365 5f28 290a 0a20 2020 2064 6566 2064  se_()..    def d
+0000f010: 6172 6b5f 6d6f 6465 5f73 7461 7465 5f63  ark_mode_state_c
+0000f020: 6861 6e67 6528 7365 6c66 293a 0a20 2020  hange(self):.   
+0000f030: 2020 2020 2022 2222 6461 726b 6d6f 6465       """darkmode
+0000f040: 2064 726f 7064 6f77 6e20 6368 6563 6b6d   dropdown checkm
+0000f050: 6172 6b20 6368 616e 6765 6422 2222 0a20  ark changed""". 
+0000f060: 2020 2020 2020 2073 656c 662e 7072 6566         self.pref
+0000f070: 5b22 6461 726b 5f6d 6f64 6522 5d20 3d20  ["dark_mode"] = 
+0000f080: 7365 6c66 2e61 6374 696f 6e44 6172 6b5f  self.actionDark_
+0000f090: 4d6f 6465 2e69 7343 6865 636b 6564 2829  Mode.isChecked()
+0000f0a0: 0a20 2020 2020 2020 2073 656c 662e 7772  .        self.wr
+0000f0b0: 6974 655f 7072 6566 6572 656e 6365 2829  ite_preference()
+0000f0c0: 0a20 2020 2020 2020 2073 656c 662e 6461  .        self.da
+0000f0d0: 726b 5f6d 6f64 6528 290a 0a20 2020 2064  rk_mode()..    d
+0000f0e0: 6566 2064 6172 6b5f 6d6f 6465 2873 656c  ef dark_mode(sel
+0000f0f0: 6629 3a0a 2020 2020 2020 2020 2222 2263  f):.        """c
+0000f100: 6861 6e67 6520 6469 7370 6c61 7920 6d6f  hange display mo
+0000f110: 6465 2222 220a 2020 2020 2020 2020 6966  de""".        if
+0000f120: 2073 656c 662e 7072 6566 2e67 6574 2822   self.pref.get("
+0000f130: 6461 726b 5f6d 6f64 6522 293a 0a20 2020  dark_mode"):.   
+0000f140: 2020 2020 2020 2020 2073 656c 662e 7365           self.se
+0000f150: 7453 7479 6c65 5368 6565 7428 4441 524b  tStyleSheet(DARK
+0000f160: 5f53 5459 4c45 5348 4545 5429 0a20 2020  _STYLESHEET).   
+0000f170: 2020 2020 2065 6c73 653a 0a20 2020 2020       else:.     
+0000f180: 2020 2020 2020 2073 656c 662e 7365 7453         self.setS
+0000f190: 7479 6c65 5368 6565 7428 2222 290a 0a20  tyleSheet("").. 
+0000f1a0: 2020 2064 6566 2063 775f 6d61 6372 6f73     def cw_macros
+0000f1b0: 5f73 7461 7465 5f63 6861 6e67 6564 2873  _state_changed(s
+0000f1c0: 656c 6629 3a0a 2020 2020 2020 2020 2222  elf):.        ""
+0000f1d0: 224d 656e 7520 6974 656d 2074 6f20 7368  "Menu item to sh
+0000f1e0: 6f77 2f68 6964 6520 6d61 6372 6f20 6275  ow/hide macro bu
+0000f1f0: 7474 6f6e 7322 2222 0a20 2020 2020 2020  ttons""".       
+0000f200: 2073 656c 662e 7072 6566 5b22 6377 5f6d   self.pref["cw_m
+0000f210: 6163 726f 7322 5d20 3d20 7365 6c66 2e61  acros"] = self.a
+0000f220: 6374 696f 6e43 575f 4d61 6372 6f73 2e69  ctionCW_Macros.i
+0000f230: 7343 6865 636b 6564 2829 0a20 2020 2020  sChecked().     
+0000f240: 2020 2073 656c 662e 7772 6974 655f 7072     self.write_pr
+0000f250: 6566 6572 656e 6365 2829 0a20 2020 2020  eference().     
+0000f260: 2020 2073 656c 662e 7368 6f77 5f43 575f     self.show_CW_
+0000f270: 6d61 6372 6f73 2829 0a0a 2020 2020 6465  macros()..    de
+0000f280: 6620 7368 6f77 5f43 575f 6d61 6372 6f73  f show_CW_macros
+0000f290: 2873 656c 6629 3a0a 2020 2020 2020 2020  (self):.        
+0000f2a0: 2222 226d 6163 726f 2062 7574 746f 6e20  """macro button 
+0000f2b0: 7374 6174 6520 6368 616e 6765 2222 220a  state change""".
+0000f2c0: 2020 2020 2020 2020 6966 2073 656c 662e          if self.
+0000f2d0: 7072 6566 2e67 6574 2822 6377 5f6d 6163  pref.get("cw_mac
+0000f2e0: 726f 7322 293a 0a20 2020 2020 2020 2020  ros"):.         
+0000f2f0: 2020 2073 656c 662e 4275 7474 6f6e 5f52     self.Button_R
+0000f300: 6f77 312e 7368 6f77 2829 0a20 2020 2020  ow1.show().     
+0000f310: 2020 2020 2020 2073 656c 662e 4275 7474         self.Butt
+0000f320: 6f6e 5f52 6f77 322e 7368 6f77 2829 0a20  on_Row2.show(). 
+0000f330: 2020 2020 2020 2065 6c73 653a 0a20 2020         else:.   
+0000f340: 2020 2020 2020 2020 2073 656c 662e 4275           self.Bu
+0000f350: 7474 6f6e 5f52 6f77 312e 6869 6465 2829  tton_Row1.hide()
+0000f360: 0a20 2020 2020 2020 2020 2020 2073 656c  .            sel
+0000f370: 662e 4275 7474 6f6e 5f52 6f77 322e 6869  f.Button_Row2.hi
+0000f380: 6465 2829 0a0a 2020 2020 6465 6620 636f  de()..    def co
+0000f390: 6d6d 616e 645f 6275 7474 6f6e 735f 7374  mmand_buttons_st
+0000f3a0: 6174 655f 6368 616e 6765 2873 656c 6629  ate_change(self)
+0000f3b0: 3a0a 2020 2020 2020 2020 2222 224d 656e  :.        """Men
+0000f3c0: 7520 6974 656d 2074 6f20 7368 6f77 2f68  u item to show/h
+0000f3d0: 6964 6520 636f 6d6d 616e 6420 6275 7474  ide command butt
+0000f3e0: 6f6e 7322 2222 0a20 2020 2020 2020 2073  ons""".        s
+0000f3f0: 656c 662e 7072 6566 5b22 636f 6d6d 616e  elf.pref["comman
+0000f400: 645f 6275 7474 6f6e 7322 5d20 3d20 7365  d_buttons"] = se
+0000f410: 6c66 2e61 6374 696f 6e43 6f6d 6d61 6e64  lf.actionCommand
+0000f420: 5f42 7574 746f 6e73 2e69 7343 6865 636b  _Buttons.isCheck
+0000f430: 6564 2829 0a20 2020 2020 2020 2073 656c  ed().        sel
+0000f440: 662e 7772 6974 655f 7072 6566 6572 656e  f.write_preferen
+0000f450: 6365 2829 0a20 2020 2020 2020 2073 656c  ce().        sel
+0000f460: 662e 7368 6f77 5f63 6f6d 6d61 6e64 5f62  f.show_command_b
+0000f470: 7574 746f 6e73 2829 0a0a 2020 2020 6465  uttons()..    de
+0000f480: 6620 7368 6f77 5f63 6f6d 6d61 6e64 5f62  f show_command_b
+0000f490: 7574 746f 6e73 2873 656c 6629 3a0a 2020  uttons(self):.  
+0000f4a0: 2020 2020 2020 2222 2263 6f6d 6d61 6e64        """command
+0000f4b0: 2062 7574 746f 6e20 7374 6174 6520 6368   button state ch
+0000f4c0: 616e 6765 2222 220a 2020 2020 2020 2020  ange""".        
+0000f4d0: 6966 2073 656c 662e 7072 6566 2e67 6574  if self.pref.get
+0000f4e0: 2822 636f 6d6d 616e 645f 6275 7474 6f6e  ("command_button
+0000f4f0: 7322 293a 0a20 2020 2020 2020 2020 2020  s"):.           
+0000f500: 2073 656c 662e 436f 6d6d 616e 645f 4275   self.Command_Bu
+0000f510: 7474 6f6e 732e 7368 6f77 2829 0a20 2020  ttons.show().   
+0000f520: 2020 2020 2065 6c73 653a 0a20 2020 2020       else:.     
+0000f530: 2020 2020 2020 2073 656c 662e 436f 6d6d         self.Comm
+0000f540: 616e 645f 4275 7474 6f6e 732e 6869 6465  and_Buttons.hide
+0000f550: 2829 0a0a 2020 2020 6465 6620 6973 5f66  ()..    def is_f
+0000f560: 6c6f 6174 6162 6c65 2873 656c 662c 2069  loatable(self, i
+0000f570: 7465 6d3a 2073 7472 2920 2d3e 2062 6f6f  tem: str) -> boo
+0000f580: 6c3a 0a20 2020 2020 2020 2022 2222 6368  l:.        """ch
+0000f590: 6563 6b20 746f 2073 6565 2069 6620 7374  eck to see if st
+0000f5a0: 7269 6e67 2063 616e 2062 6520 6120 666c  ring can be a fl
+0000f5b0: 6f61 7422 2222 0a20 2020 2020 2020 2069  oat""".        i
+0000f5c0: 6620 6974 656d 2e69 736e 756d 6572 6963  f item.isnumeric
+0000f5d0: 2829 3a0a 2020 2020 2020 2020 2020 2020  ():.            
+0000f5e0: 7265 7475 726e 2054 7275 650a 2020 2020  return True.    
+0000f5f0: 2020 2020 7472 793a 0a20 2020 2020 2020      try:.       
+0000f600: 2020 2020 205f 7465 7374 203d 2066 6c6f       _test = flo
+0000f610: 6174 2869 7465 6d29 0a20 2020 2020 2020  at(item).       
+0000f620: 2065 7863 6570 7420 5661 6c75 6545 7272   except ValueErr
+0000f630: 6f72 3a0a 2020 2020 2020 2020 2020 2020  or:.            
+0000f640: 7265 7475 726e 2046 616c 7365 0a20 2020  return False.   
+0000f650: 2020 2020 2072 6574 7572 6e20 5472 7565       return True
+0000f660: 0a0a 2020 2020 6465 6620 6f74 6865 725f  ..    def other_
+0000f670: 325f 6368 616e 6765 6428 7365 6c66 293a  2_changed(self):
+0000f680: 0a20 2020 2020 2020 2022 2222 4361 6c6c  .        """Call
+0000f690: 6564 2077 6865 6e20 7765 206e 6565 6420  ed when we need 
+0000f6a0: 746f 2070 6172 7365 2053 5320 6578 6368  to parse SS exch
+0000f6b0: 616e 6765 2e22 2222 0a20 2020 2020 2020  ange.""".       
+0000f6c0: 2069 6620 7365 6c66 2e63 6f6e 7465 7374   if self.contest
+0000f6d0: 3a0a 2020 2020 2020 2020 2020 2020 6966  :.            if
+0000f6e0: 2022 4152 524c 2053 7765 6570 7374 616b   "ARRL Sweepstak
+0000f6f0: 6573 2220 696e 2073 656c 662e 636f 6e74  es" in self.cont
+0000f700: 6573 742e 6e61 6d65 3a0a 2020 2020 2020  est.name:.      
+0000f710: 2020 2020 2020 2020 2020 7365 6c66 2e63            self.c
+0000f720: 6f6e 7465 7374 2e70 6172 7365 5f65 7863  ontest.parse_exc
+0000f730: 6861 6e67 6528 7365 6c66 290a 0a20 2020  hange(self)..   
+0000f740: 2064 6566 2063 616c 6c73 6967 6e5f 6368   def callsign_ch
+0000f750: 616e 6765 6428 7365 6c66 293a 0a20 2020  anged(self):.   
+0000f760: 2020 2020 2022 2222 4361 6c6c 6564 2077       """Called w
+0000f770: 6865 6e20 7465 7874 2069 6e20 7468 6520  hen text in the 
+0000f780: 6361 6c6c 7369 676e 2066 6965 6c64 2068  callsign field h
+0000f790: 6173 2063 6861 6e67 6564 2222 220a 2020  as changed""".  
+0000f7a0: 2020 2020 2020 7465 7874 203d 2073 656c        text = sel
+0000f7b0: 662e 6361 6c6c 7369 676e 2e74 6578 7428  f.callsign.text(
+0000f7c0: 290a 2020 2020 2020 2020 7465 7874 203d  ).        text =
+0000f7d0: 2074 6578 742e 7570 7065 7228 290a 2020   text.upper().  
+0000f7e0: 2020 2020 2020 706f 7369 7469 6f6e 203d        position =
+0000f7f0: 2073 656c 662e 6361 6c6c 7369 676e 2e63   self.callsign.c
+0000f800: 7572 736f 7250 6f73 6974 696f 6e28 290a  ursorPosition().
+0000f810: 2020 2020 2020 2020 7374 7269 7070 6564          stripped
+0000f820: 5f74 6578 7420 3d20 7465 7874 2e73 7472  _text = text.str
+0000f830: 6970 2829 2e72 6570 6c61 6365 2822 2022  ip().replace(" "
+0000f840: 2c20 2222 290a 2020 2020 2020 2020 7365  , "").        se
+0000f850: 6c66 2e63 616c 6c73 6967 6e2e 7365 7454  lf.callsign.setT
+0000f860: 6578 7428 7374 7269 7070 6564 5f74 6578  ext(stripped_tex
+0000f870: 7429 0a20 2020 2020 2020 2073 656c 662e  t).        self.
+0000f880: 6361 6c6c 7369 676e 2e73 6574 4375 7273  callsign.setCurs
+0000f890: 6f72 506f 7369 7469 6f6e 2870 6f73 6974  orPosition(posit
+0000f8a0: 696f 6e29 0a0a 2020 2020 2020 2020 6966  ion)..        if
+0000f8b0: 2022 2022 2069 6e20 7465 7874 3a0a 2020   " " in text:.  
+0000f8c0: 2020 2020 2020 2020 2020 6966 2073 7472            if str
+0000f8d0: 6970 7065 645f 7465 7874 203d 3d20 2243  ipped_text == "C
+0000f8e0: 5722 3a0a 2020 2020 2020 2020 2020 2020  W":.            
+0000f8f0: 2020 2020 7365 6c66 2e73 6574 6d6f 6465      self.setmode
+0000f900: 2822 4357 2229 0a20 2020 2020 2020 2020  ("CW").         
+0000f910: 2020 2020 2020 2073 656c 662e 7261 6469         self.radi
+0000f920: 6f5f 7374 6174 655b 226d 6f64 6522 5d20  o_state["mode"] 
+0000f930: 3d20 2243 5722 0a20 2020 2020 2020 2020  = "CW".         
+0000f940: 2020 2020 2020 2069 6620 7365 6c66 2e72         if self.r
+0000f950: 6967 5f63 6f6e 7472 6f6c 3a0a 2020 2020  ig_control:.    
+0000f960: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000f970: 6966 2073 656c 662e 7269 675f 636f 6e74  if self.rig_cont
+0000f980: 726f 6c2e 6f6e 6c69 6e65 3a0a 2020 2020  rol.online:.    
+0000f990: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000f9a0: 2020 2020 7365 6c66 2e72 6967 5f63 6f6e      self.rig_con
+0000f9b0: 7472 6f6c 2e73 6574 5f6d 6f64 6528 2243  trol.set_mode("C
+0000f9c0: 5722 290a 2020 2020 2020 2020 2020 2020  W").            
+0000f9d0: 2020 2020 7365 6c66 2e73 6574 5f77 696e      self.set_win
+0000f9e0: 646f 775f 7469 746c 6528 290a 2020 2020  dow_title().    
+0000f9f0: 2020 2020 2020 2020 2020 2020 7365 6c66              self
+0000fa00: 2e63 6c65 6172 696e 7075 7473 2829 0a20  .clearinputs(). 
+0000fa10: 2020 2020 2020 2020 2020 2020 2020 2073                 s
+0000fa20: 656c 662e 7265 6164 5f63 775f 6d61 6372  elf.read_cw_macr
+0000fa30: 6f73 2829 0a20 2020 2020 2020 2020 2020  os().           
+0000fa40: 2020 2020 2072 6574 7572 6e0a 2020 2020       return.    
+0000fa50: 2020 2020 2020 2020 6966 2073 7472 6970          if strip
+0000fa60: 7065 645f 7465 7874 203d 3d20 2252 5454  ped_text == "RTT
+0000fa70: 5922 3a0a 2020 2020 2020 2020 2020 2020  Y":.            
+0000fa80: 2020 2020 7365 6c66 2e73 6574 6d6f 6465      self.setmode
+0000fa90: 2822 5254 5459 2229 0a20 2020 2020 2020  ("RTTY").       
+0000faa0: 2020 2020 2020 2020 2069 6620 7365 6c66           if self
+0000fab0: 2e72 6967 5f63 6f6e 7472 6f6c 3a0a 2020  .rig_control:.  
+0000fac0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000fad0: 2020 6966 2073 656c 662e 7269 675f 636f    if self.rig_co
+0000fae0: 6e74 726f 6c2e 6f6e 6c69 6e65 3a0a 2020  ntrol.online:.  
+0000faf0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000fb00: 2020 2020 2020 7365 6c66 2e72 6967 5f63        self.rig_c
+0000fb10: 6f6e 7472 6f6c 2e73 6574 5f6d 6f64 6528  ontrol.set_mode(
+0000fb20: 2252 5454 5922 290a 2020 2020 2020 2020  "RTTY").        
+0000fb30: 2020 2020 2020 2020 2020 2020 656c 7365              else
+0000fb40: 3a0a 2020 2020 2020 2020 2020 2020 2020  :.              
+0000fb50: 2020 2020 2020 2020 2020 7365 6c66 2e72            self.r
+0000fb60: 6164 696f 5f73 7461 7465 5b22 6d6f 6465  adio_state["mode
+0000fb70: 225d 203d 2022 5254 5459 220a 2020 2020  "] = "RTTY".    
+0000fb80: 2020 2020 2020 2020 2020 2020 7365 6c66              self
+0000fb90: 2e73 6574 5f77 696e 646f 775f 7469 746c  .set_window_titl
+0000fba0: 6528 290a 2020 2020 2020 2020 2020 2020  e().            
+0000fbb0: 2020 2020 7365 6c66 2e63 6c65 6172 696e      self.clearin
+0000fbc0: 7075 7473 2829 0a20 2020 2020 2020 2020  puts().         
+0000fbd0: 2020 2020 2020 2072 6574 7572 6e0a 2020         return.  
+0000fbe0: 2020 2020 2020 2020 2020 6966 2073 7472            if str
+0000fbf0: 6970 7065 645f 7465 7874 203d 3d20 2253  ipped_text == "S
+0000fc00: 5342 223a 0a20 2020 2020 2020 2020 2020  SB":.           
+0000fc10: 2020 2020 2073 656c 662e 7365 746d 6f64       self.setmod
+0000fc20: 6528 2253 5342 2229 0a20 2020 2020 2020  e("SSB").       
+0000fc30: 2020 2020 2020 2020 2069 6620 696e 7428           if int(
+0000fc40: 7365 6c66 2e72 6164 696f 5f73 7461 7465  self.radio_state
+0000fc50: 2e67 6574 2822 7666 6f61 222c 2030 2929  .get("vfoa", 0))
+0000fc60: 203e 2031 3030 3030 3030 303a 0a20 2020   > 10000000:.   
+0000fc70: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000fc80: 2073 656c 662e 7261 6469 6f5f 7374 6174   self.radio_stat
+0000fc90: 655b 226d 6f64 6522 5d20 3d20 2255 5342  e["mode"] = "USB
+0000fca0: 220a 2020 2020 2020 2020 2020 2020 2020  ".              
+0000fcb0: 2020 656c 7365 3a0a 2020 2020 2020 2020    else:.        
+0000fcc0: 2020 2020 2020 2020 2020 2020 7365 6c66              self
+0000fcd0: 2e72 6164 696f 5f73 7461 7465 5b22 6d6f  .radio_state["mo
+0000fce0: 6465 225d 203d 2022 4c53 4222 0a20 2020  de"] = "LSB".   
+0000fcf0: 2020 2020 2020 2020 2020 2020 2073 656c               sel
+0000fd00: 662e 7365 745f 7769 6e64 6f77 5f74 6974  f.set_window_tit
+0000fd10: 6c65 2829 0a20 2020 2020 2020 2020 2020  le().           
+0000fd20: 2020 2020 2069 6620 7365 6c66 2e72 6967       if self.rig
+0000fd30: 5f63 6f6e 7472 6f6c 3a0a 2020 2020 2020  _control:.      
+0000fd40: 2020 2020 2020 2020 2020 2020 2020 7365                se
+0000fd50: 6c66 2e72 6967 5f63 6f6e 7472 6f6c 2e73  lf.rig_control.s
+0000fd60: 6574 5f6d 6f64 6528 7365 6c66 2e72 6164  et_mode(self.rad
+0000fd70: 696f 5f73 7461 7465 2e67 6574 2822 6d6f  io_state.get("mo
+0000fd80: 6465 2229 290a 2020 2020 2020 2020 2020  de")).          
+0000fd90: 2020 2020 2020 7365 6c66 2e63 6c65 6172        self.clear
+0000fda0: 696e 7075 7473 2829 0a20 2020 2020 2020  inputs().       
+0000fdb0: 2020 2020 2020 2020 2073 656c 662e 7265           self.re
+0000fdc0: 6164 5f63 775f 6d61 6372 6f73 2829 0a20  ad_cw_macros(). 
+0000fdd0: 2020 2020 2020 2020 2020 2020 2020 2072                 r
+0000fde0: 6574 7572 6e0a 2020 2020 2020 2020 2020  eturn.          
+0000fdf0: 2020 6966 2073 7472 6970 7065 645f 7465    if stripped_te
+0000fe00: 7874 203d 3d20 224f 504f 4e22 3a0a 2020  xt == "OPON":.  
+0000fe10: 2020 2020 2020 2020 2020 2020 2020 7365                se
+0000fe20: 6c66 2e67 6574 5f6f 706f 6e28 290a 2020  lf.get_opon().  
+0000fe30: 2020 2020 2020 2020 2020 2020 2020 7365                se
+0000fe40: 6c66 2e63 6c65 6172 696e 7075 7473 2829  lf.clearinputs()
+0000fe50: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+0000fe60: 2072 6574 7572 6e0a 2020 2020 2020 2020   return.        
+0000fe70: 2020 2020 6966 2073 7472 6970 7065 645f      if stripped_
+0000fe80: 7465 7874 203d 3d20 2254 4553 5422 3a0a  text == "TEST":.
+0000fe90: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000fea0: 7365 6c66 2e73 686f 775f 6d65 7373 6167  self.show_messag
+0000feb0: 655f 626f 7828 2254 6869 7320 6973 2061  e_box("This is a
+0000fec0: 2074 6573 7422 290a 2020 2020 2020 2020   test").        
+0000fed0: 2020 2020 2020 2020 7365 6c66 2e63 6c65          self.cle
+0000fee0: 6172 696e 7075 7473 2829 0a20 2020 2020  arinputs().     
+0000fef0: 2020 2020 2020 2020 2020 2072 6574 7572             retur
+0000ff00: 6e0a 2020 2020 2020 2020 2020 2020 6966  n.            if
+0000ff10: 2073 656c 662e 6973 5f66 6c6f 6174 6162   self.is_floatab
+0000ff20: 6c65 2873 7472 6970 7065 645f 7465 7874  le(stripped_text
+0000ff30: 293a 0a20 2020 2020 2020 2020 2020 2020  ):.             
+0000ff40: 2020 2076 666f 203d 2066 6c6f 6174 2873     vfo = float(s
+0000ff50: 7472 6970 7065 645f 7465 7874 290a 2020  tripped_text).  
+0000ff60: 2020 2020 2020 2020 2020 2020 2020 7666                vf
+0000ff70: 6f20 3d20 696e 7428 7666 6f20 2a20 3130  o = int(vfo * 10
+0000ff80: 3030 290a 2020 2020 2020 2020 2020 2020  00).            
+0000ff90: 2020 2020 6261 6e64 203d 2067 6574 6261      band = getba
+0000ffa0: 6e64 2873 7472 2876 666f 2929 0a20 2020  nd(str(vfo)).   
+0000ffb0: 2020 2020 2020 2020 2020 2020 2073 656c               sel
+0000ffc0: 662e 7365 745f 6261 6e64 5f69 6e64 6963  f.set_band_indic
+0000ffd0: 6174 6f72 2862 616e 6429 0a20 2020 2020  ator(band).     
+0000ffe0: 2020 2020 2020 2020 2020 2023 2073 656c             # sel
+0000fff0: 662e 636f 6e74 6163 745b 2242 616e 6422  f.contact["Band"
+00010000: 5d20 3d20 6765 745f 6c6f 6767 6564 5f62  ] = get_logged_b
+00010010: 616e 6428 7374 7228 7365 6c66 2e72 6164  and(str(self.rad
+00010020: 696f 5f73 7461 7465 2e67 6574 2822 7666  io_state.get("vf
+00010030: 6f61 222c 2030 2e30 2929 290a 2020 2020  oa", 0.0))).    
+00010040: 2020 2020 2020 2020 2020 2020 7365 6c66              self
+00010050: 2e72 6164 696f 5f73 7461 7465 5b22 7666  .radio_state["vf
+00010060: 6f61 225d 203d 2076 666f 0a20 2020 2020  oa"] = vfo.     
+00010070: 2020 2020 2020 2020 2020 2073 656c 662e             self.
+00010080: 7365 745f 7769 6e64 6f77 5f74 6974 6c65  set_window_title
+00010090: 2829 0a20 2020 2020 2020 2020 2020 2020  ().             
+000100a0: 2020 2073 656c 662e 636c 6561 7269 6e70     self.clearinp
+000100b0: 7574 7328 290a 2020 2020 2020 2020 2020  uts().          
+000100c0: 2020 2020 2020 6966 2073 656c 662e 7269        if self.ri
+000100d0: 675f 636f 6e74 726f 6c3a 0a20 2020 2020  g_control:.     
+000100e0: 2020 2020 2020 2020 2020 2020 2020 2073                 s
+000100f0: 656c 662e 7269 675f 636f 6e74 726f 6c2e  elf.rig_control.
+00010100: 7365 745f 7666 6f28 7666 6f29 0a20 2020  set_vfo(vfo).   
+00010110: 2020 2020 2020 2020 2020 2020 2072 6574               ret
+00010120: 7572 6e0a 0a20 2020 2020 2020 2020 2020  urn..           
+00010130: 2073 656c 662e 6368 6563 6b5f 6361 6c6c   self.check_call
+00010140: 7369 676e 2873 7472 6970 7065 645f 7465  sign(stripped_te
+00010150: 7874 290a 2020 2020 2020 2020 2020 2020  xt).            
+00010160: 6966 2073 656c 662e 6368 6563 6b5f 6475  if self.check_du
+00010170: 7065 2873 7472 6970 7065 645f 7465 7874  pe(stripped_text
+00010180: 293a 0a20 2020 2020 2020 2020 2020 2020  ):.             
+00010190: 2020 2073 656c 662e 6475 7065 5f69 6e64     self.dupe_ind
+000101a0: 6963 6174 6f72 2e73 686f 7728 290a 2020  icator.show().  
+000101b0: 2020 2020 2020 2020 2020 656c 7365 3a0a            else:.
+000101c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000101d0: 7365 6c66 2e64 7570 655f 696e 6469 6361  self.dupe_indica
+000101e0: 746f 722e 6869 6465 2829 0a20 2020 2020  tor.hide().     
+000101f0: 2020 2020 2020 205f 7468 6574 6872 6561         _thethrea
+00010200: 6420 3d20 7468 7265 6164 696e 672e 5468  d = threading.Th
+00010210: 7265 6164 280a 2020 2020 2020 2020 2020  read(.          
+00010220: 2020 2020 2020 7461 7267 6574 3d73 656c        target=sel
+00010230: 662e 6368 6563 6b5f 6361 6c6c 7369 676e  f.check_callsign
+00010240: 322c 0a20 2020 2020 2020 2020 2020 2020  2,.             
+00010250: 2020 2061 7267 733d 2874 6578 742c 292c     args=(text,),
+00010260: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00010270: 2064 6165 6d6f 6e3d 5472 7565 2c0a 2020   daemon=True,.  
+00010280: 2020 2020 2020 2020 2020 290a 2020 2020            ).    
+00010290: 2020 2020 2020 2020 5f74 6865 7468 7265          _thethre
+000102a0: 6164 2e73 7461 7274 2829 0a20 2020 2020  ad.start().     
+000102b0: 2020 2020 2020 2073 656c 662e 6e65 7874         self.next
+000102c0: 5f66 6965 6c64 2e73 6574 466f 6375 7328  _field.setFocus(
+000102d0: 290a 2020 2020 2020 2020 2020 2020 7265  ).            re
+000102e0: 7475 726e 0a20 2020 2020 2020 2063 6d64  turn.        cmd
+000102f0: 203d 207b 7d0a 2020 2020 2020 2020 636d   = {}.        cm
+00010300: 645b 2263 6d64 225d 203d 2022 4341 4c4c  d["cmd"] = "CALL
+00010310: 4348 414e 4745 4422 0a20 2020 2020 2020  CHANGED".       
+00010320: 2063 6d64 5b22 7374 6174 696f 6e22 5d20   cmd["station"] 
+00010330: 3d20 706c 6174 666f 726d 2e6e 6f64 6528  = platform.node(
+00010340: 290a 2020 2020 2020 2020 636d 645b 2263  ).        cmd["c
+00010350: 616c 6c22 5d20 3d20 7374 7269 7070 6564  all"] = stripped
+00010360: 5f74 6578 740a 2020 2020 2020 2020 7365  _text.        se
+00010370: 6c66 2e6d 756c 7469 6361 7374 5f69 6e74  lf.multicast_int
+00010380: 6572 6661 6365 2e73 656e 645f 6173 5f6a  erface.send_as_j
+00010390: 736f 6e28 636d 6429 0a20 2020 2020 2020  son(cmd).       
+000103a0: 2073 656c 662e 6368 6563 6b5f 6361 6c6c   self.check_call
+000103b0: 7369 676e 2873 7472 6970 7065 645f 7465  sign(stripped_te
+000103c0: 7874 290a 0a20 2020 2064 6566 2063 6865  xt)..    def che
+000103d0: 636b 5f63 616c 6c73 6967 6e28 7365 6c66  ck_callsign(self
+000103e0: 2c20 6361 6c6c 7369 676e 293a 0a20 2020  , callsign):.   
+000103f0: 2020 2020 2022 2222 4368 6563 6b20 6361       """Check ca
+00010400: 6c6c 2061 7320 656e 7465 7265 6422 2222  ll as entered"""
+00010410: 0a20 2020 2020 2020 2072 6573 756c 7420  .        result 
+00010420: 3d20 6374 795f 6c6f 6f6b 7570 2863 616c  = cty_lookup(cal
+00010430: 6c73 6967 6e29 0a20 2020 2020 2020 2064  lsign).        d
+00010440: 6562 7567 5f72 6573 756c 7420 3d20 6622  ebug_result = f"
+00010450: 7b72 6573 756c 747d 220a 2020 2020 2020  {result}".      
+00010460: 2020 6c6f 6767 6572 2e64 6562 7567 2822    logger.debug("
+00010470: 2573 222c 2064 6562 7567 5f72 6573 756c  %s", debug_resul
+00010480: 7429 0a20 2020 2020 2020 2069 6620 7265  t).        if re
+00010490: 7375 6c74 3a0a 2020 2020 2020 2020 2020  sult:.          
+000104a0: 2020 666f 7220 6120 696e 2072 6573 756c    for a in resul
+000104b0: 742e 6974 656d 7328 293a 0a20 2020 2020  t.items():.     
+000104c0: 2020 2020 2020 2020 2020 2065 6e74 6974             entit
+000104d0: 7920 3d20 615b 315d 2e67 6574 2822 656e  y = a[1].get("en
+000104e0: 7469 7479 222c 2022 2229 0a20 2020 2020  tity", "").     
+000104f0: 2020 2020 2020 2020 2020 2063 7120 3d20             cq = 
+00010500: 615b 315d 2e67 6574 2822 6371 222c 2022  a[1].get("cq", "
 00010510: 2229 0a20 2020 2020 2020 2020 2020 2020  ").             
-00010520: 2020 2063 6f6e 7469 6e65 6e74 203d 2061     continent = a
-00010530: 5b31 5d2e 6765 7428 2263 6f6e 7469 6e65  [1].get("contine
-00010540: 6e74 2229 0a20 2020 2020 2020 2020 2020  nt").           
-00010550: 2020 2020 206c 6174 203d 2066 6c6f 6174       lat = float
-00010560: 2861 5b31 5d2e 6765 7428 226c 6174 222c  (a[1].get("lat",
-00010570: 2022 302e 3022 2929 0a20 2020 2020 2020   "0.0")).       
-00010580: 2020 2020 2020 2020 206c 6f6e 203d 2066           lon = f
-00010590: 6c6f 6174 2861 5b31 5d2e 6765 7428 226c  loat(a[1].get("l
-000105a0: 6f6e 6722 2c20 2230 2e30 2229 290a 2020  ong", "0.0")).  
-000105b0: 2020 2020 2020 2020 2020 2020 2020 6c6f                lo
-000105c0: 6e20 3d20 6c6f 6e20 2a20 2d31 2020 2320  n = lon * -1  # 
-000105d0: 6374 792e 6461 7420 6669 6c65 2069 6e76  cty.dat file inv
-000105e0: 6572 7473 206c 6f6e 6769 7475 6465 730a  erts longitudes.
-000105f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00010600: 7072 696d 6172 795f 7066 7820 3d20 615b  primary_pfx = a[
-00010610: 315d 2e67 6574 2822 7072 696d 6172 795f  1].get("primary_
-00010620: 7066 7822 2c20 2222 290a 2020 2020 2020  pfx", "").      
-00010630: 2020 2020 2020 2020 2020 6865 6164 696e            headin
-00010640: 6720 3d20 6265 6172 696e 675f 7769 7468  g = bearing_with
-00010650: 5f6c 6174 6c6f 6e28 7365 6c66 2e73 7461  _latlon(self.sta
-00010660: 7469 6f6e 2e67 6574 2822 4772 6964 5371  tion.get("GridSq
-00010670: 7561 7265 2229 2c20 6c61 742c 206c 6f6e  uare"), lat, lon
-00010680: 290a 2020 2020 2020 2020 2020 2020 2020  ).              
-00010690: 2020 6b69 6c6f 6d65 7465 7273 203d 2064    kilometers = d
-000106a0: 6973 7461 6e63 655f 7769 7468 5f6c 6174  istance_with_lat
-000106b0: 6c6f 6e28 0a20 2020 2020 2020 2020 2020  lon(.           
-000106c0: 2020 2020 2020 2020 2073 656c 662e 7374           self.st
-000106d0: 6174 696f 6e2e 6765 7428 2247 7269 6453  ation.get("GridS
-000106e0: 7175 6172 6522 292c 206c 6174 2c20 6c6f  quare"), lat, lo
-000106f0: 6e0a 2020 2020 2020 2020 2020 2020 2020  n.              
-00010700: 2020 290a 2020 2020 2020 2020 2020 2020    ).            
-00010710: 2020 2020 7365 6c66 2e68 6561 6469 6e67      self.heading
-00010720: 5f64 6973 7461 6e63 652e 7365 7454 6578  _distance.setTex
-00010730: 7428 0a20 2020 2020 2020 2020 2020 2020  t(.             
-00010740: 2020 2020 2020 2066 2252 6567 696f 6e61         f"Regiona
-00010750: 6c20 4864 6720 7b68 6561 6469 6e67 7dc2  l Hdg {heading}.
-00010760: b020 4c50 207b 7265 6369 7072 6f63 6f6c  . LP {reciprocol
-00010770: 2868 6561 6469 6e67 297d c2b0 202f 2022  (heading)}.. / "
-00010780: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00010790: 2020 2020 2066 2264 6973 7461 6e63 6520       f"distance 
-000107a0: 7b69 6e74 286b 696c 6f6d 6574 6572 732a  {int(kilometers*
-000107b0: 302e 3632 3133 3731 297d 6d69 207b 6b69  0.621371)}mi {ki
-000107c0: 6c6f 6d65 7465 7273 7d6b 6d22 0a20 2020  lometers}km".   
-000107d0: 2020 2020 2020 2020 2020 2020 2029 0a20               ). 
-000107e0: 2020 2020 2020 2020 2020 2020 2020 2073                 s
-000107f0: 656c 662e 636f 6e74 6163 745b 2243 6f75  elf.contact["Cou
-00010800: 6e74 7279 5072 6566 6978 225d 203d 2070  ntryPrefix"] = p
-00010810: 7269 6d61 7279 5f70 6678 0a20 2020 2020  rimary_pfx.     
-00010820: 2020 2020 2020 2020 2020 2073 656c 662e             self.
-00010830: 636f 6e74 6163 745b 225a 4e22 5d20 3d20  contact["ZN"] = 
-00010840: 696e 7428 6371 290a 2020 2020 2020 2020  int(cq).        
-00010850: 2020 2020 2020 2020 7365 6c66 2e63 6f6e          self.con
-00010860: 7461 6374 5b22 436f 6e74 696e 656e 7422  tact["Continent"
-00010870: 5d20 3d20 636f 6e74 696e 656e 740a 2020  ] = continent.  
-00010880: 2020 2020 2020 2020 2020 2020 2020 7365                se
-00010890: 6c66 2e64 785f 656e 7469 7479 2e73 6574  lf.dx_entity.set
-000108a0: 5465 7874 280a 2020 2020 2020 2020 2020  Text(.          
-000108b0: 2020 2020 2020 2020 2020 6622 7b70 7269            f"{pri
-000108c0: 6d61 7279 5f70 6678 7d3a 207b 636f 6e74  mary_pfx}: {cont
-000108d0: 696e 656e 747d 2f7b 656e 7469 7479 7d20  inent}/{entity} 
-000108e0: 6371 3a7b 6371 7d20 6974 753a 7b69 7475  cq:{cq} itu:{itu
-000108f0: 7d22 0a20 2020 2020 2020 2020 2020 2020  }".             
-00010900: 2020 2029 0a20 2020 2020 2020 2020 2020     ).           
-00010910: 2020 2020 2069 6620 6c65 6e28 6361 6c6c       if len(call
-00010920: 7369 676e 2920 3e20 323a 0a20 2020 2020  sign) > 2:.     
+00010520: 2020 2069 7475 203d 2061 5b31 5d2e 6765     itu = a[1].ge
+00010530: 7428 2269 7475 222c 2022 2229 0a20 2020  t("itu", "").   
+00010540: 2020 2020 2020 2020 2020 2020 2063 6f6e               con
+00010550: 7469 6e65 6e74 203d 2061 5b31 5d2e 6765  tinent = a[1].ge
+00010560: 7428 2263 6f6e 7469 6e65 6e74 2229 0a20  t("continent"). 
+00010570: 2020 2020 2020 2020 2020 2020 2020 206c                 l
+00010580: 6174 203d 2066 6c6f 6174 2861 5b31 5d2e  at = float(a[1].
+00010590: 6765 7428 226c 6174 222c 2022 302e 3022  get("lat", "0.0"
+000105a0: 2929 0a20 2020 2020 2020 2020 2020 2020  )).             
+000105b0: 2020 206c 6f6e 203d 2066 6c6f 6174 2861     lon = float(a
+000105c0: 5b31 5d2e 6765 7428 226c 6f6e 6722 2c20  [1].get("long", 
+000105d0: 2230 2e30 2229 290a 2020 2020 2020 2020  "0.0")).        
+000105e0: 2020 2020 2020 2020 6c6f 6e20 3d20 6c6f          lon = lo
+000105f0: 6e20 2a20 2d31 2020 2320 6374 792e 6461  n * -1  # cty.da
+00010600: 7420 6669 6c65 2069 6e76 6572 7473 206c  t file inverts l
+00010610: 6f6e 6769 7475 6465 730a 2020 2020 2020  ongitudes.      
+00010620: 2020 2020 2020 2020 2020 7072 696d 6172            primar
+00010630: 795f 7066 7820 3d20 615b 315d 2e67 6574  y_pfx = a[1].get
+00010640: 2822 7072 696d 6172 795f 7066 7822 2c20  ("primary_pfx", 
+00010650: 2222 290a 2020 2020 2020 2020 2020 2020  "").            
+00010660: 2020 2020 6865 6164 696e 6720 3d20 6265      heading = be
+00010670: 6172 696e 675f 7769 7468 5f6c 6174 6c6f  aring_with_latlo
+00010680: 6e28 7365 6c66 2e73 7461 7469 6f6e 2e67  n(self.station.g
+00010690: 6574 2822 4772 6964 5371 7561 7265 2229  et("GridSquare")
+000106a0: 2c20 6c61 742c 206c 6f6e 290a 2020 2020  , lat, lon).    
+000106b0: 2020 2020 2020 2020 2020 2020 6b69 6c6f              kilo
+000106c0: 6d65 7465 7273 203d 2064 6973 7461 6e63  meters = distanc
+000106d0: 655f 7769 7468 5f6c 6174 6c6f 6e28 0a20  e_with_latlon(. 
+000106e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000106f0: 2020 2073 656c 662e 7374 6174 696f 6e2e     self.station.
+00010700: 6765 7428 2247 7269 6453 7175 6172 6522  get("GridSquare"
+00010710: 292c 206c 6174 2c20 6c6f 6e0a 2020 2020  ), lat, lon.    
+00010720: 2020 2020 2020 2020 2020 2020 290a 2020              ).  
+00010730: 2020 2020 2020 2020 2020 2020 2020 7365                se
+00010740: 6c66 2e68 6561 6469 6e67 5f64 6973 7461  lf.heading_dista
+00010750: 6e63 652e 7365 7454 6578 7428 0a20 2020  nce.setText(.   
+00010760: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00010770: 2066 2252 6567 696f 6e61 6c20 4864 6720   f"Regional Hdg 
+00010780: 7b68 6561 6469 6e67 7dc2 b020 4c50 207b  {heading}.. LP {
+00010790: 7265 6369 7072 6f63 6f6c 2868 6561 6469  reciprocol(headi
+000107a0: 6e67 297d c2b0 202f 2022 0a20 2020 2020  ng)}.. / ".     
+000107b0: 2020 2020 2020 2020 2020 2020 2020 2066                 f
+000107c0: 2264 6973 7461 6e63 6520 7b69 6e74 286b  "distance {int(k
+000107d0: 696c 6f6d 6574 6572 732a 302e 3632 3133  ilometers*0.6213
+000107e0: 3731 297d 6d69 207b 6b69 6c6f 6d65 7465  71)}mi {kilomete
+000107f0: 7273 7d6b 6d22 0a20 2020 2020 2020 2020  rs}km".         
+00010800: 2020 2020 2020 2029 0a20 2020 2020 2020         ).       
+00010810: 2020 2020 2020 2020 2073 656c 662e 636f           self.co
+00010820: 6e74 6163 745b 2243 6f75 6e74 7279 5072  ntact["CountryPr
+00010830: 6566 6978 225d 203d 2070 7269 6d61 7279  efix"] = primary
+00010840: 5f70 6678 0a20 2020 2020 2020 2020 2020  _pfx.           
+00010850: 2020 2020 2073 656c 662e 636f 6e74 6163       self.contac
+00010860: 745b 225a 4e22 5d20 3d20 696e 7428 6371  t["ZN"] = int(cq
+00010870: 290a 2020 2020 2020 2020 2020 2020 2020  ).              
+00010880: 2020 7365 6c66 2e63 6f6e 7461 6374 5b22    self.contact["
+00010890: 436f 6e74 696e 656e 7422 5d20 3d20 636f  Continent"] = co
+000108a0: 6e74 696e 656e 740a 2020 2020 2020 2020  ntinent.        
+000108b0: 2020 2020 2020 2020 7365 6c66 2e64 785f          self.dx_
+000108c0: 656e 7469 7479 2e73 6574 5465 7874 280a  entity.setText(.
+000108d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000108e0: 2020 2020 6622 7b70 7269 6d61 7279 5f70      f"{primary_p
+000108f0: 6678 7d3a 207b 636f 6e74 696e 656e 747d  fx}: {continent}
+00010900: 2f7b 656e 7469 7479 7d20 6371 3a7b 6371  /{entity} cq:{cq
+00010910: 7d20 6974 753a 7b69 7475 7d22 0a20 2020  } itu:{itu}".   
+00010920: 2020 2020 2020 2020 2020 2020 2029 0a20               ). 
 00010930: 2020 2020 2020 2020 2020 2020 2020 2069                 i
-00010940: 6620 7365 6c66 2e63 6f6e 7465 7374 3a0a  f self.contest:.
-00010950: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00010960: 2020 2020 2020 2020 7365 6c66 2e63 6f6e          self.con
-00010970: 7465 7374 2e70 7265 6669 6c6c 2873 656c  test.prefill(sel
-00010980: 6629 0a0a 2020 2020 6465 6620 6368 6563  f)..    def chec
-00010990: 6b5f 6361 6c6c 7369 676e 3228 7365 6c66  k_callsign2(self
-000109a0: 2c20 6361 6c6c 7369 676e 293a 0a20 2020  , callsign):.   
-000109b0: 2020 2020 2022 2222 4368 6563 6b20 6361       """Check ca
-000109c0: 6c6c 206f 6e63 6520 656e 7465 7265 6422  ll once entered"
-000109d0: 2222 0a20 2020 2020 2020 2063 616c 6c73  "".        calls
-000109e0: 6967 6e20 3d20 6361 6c6c 7369 676e 2e73  ign = callsign.s
-000109f0: 7472 6970 2829 0a20 2020 2020 2020 2064  trip().        d
-00010a00: 6562 7567 5f6c 6f6f 6b75 7020 3d20 6622  ebug_lookup = f"
-00010a10: 7b73 656c 662e 6c6f 6f6b 5f75 707d 220a  {self.look_up}".
-00010a20: 2020 2020 2020 2020 6c6f 6767 6572 2e64          logger.d
-00010a30: 6562 7567 2822 2573 2c20 2573 222c 2063  ebug("%s, %s", c
-00010a40: 616c 6c73 6967 6e2c 2064 6562 7567 5f6c  allsign, debug_l
-00010a50: 6f6f 6b75 7029 0a20 2020 2020 2020 2069  ookup).        i
-00010a60: 6620 6861 7361 7474 7228 7365 6c66 2e6c  f hasattr(self.l
-00010a70: 6f6f 6b5f 7570 2c20 2273 6573 7369 6f6e  ook_up, "session
-00010a80: 2229 3a0a 2020 2020 2020 2020 2020 2020  "):.            
-00010a90: 6966 2073 656c 662e 6c6f 6f6b 5f75 702e  if self.look_up.
-00010aa0: 7365 7373 696f 6e3a 0a20 2020 2020 2020  session:.       
-00010ab0: 2020 2020 2020 2020 2072 6573 706f 6e73           respons
-00010ac0: 6520 3d20 7365 6c66 2e6c 6f6f 6b5f 7570  e = self.look_up
-00010ad0: 2e6c 6f6f 6b75 7028 6361 6c6c 7369 676e  .lookup(callsign
-00010ae0: 290a 2020 2020 2020 2020 2020 2020 2020  ).              
-00010af0: 2020 6465 6275 675f 7265 7370 6f6e 7365    debug_response
-00010b00: 203d 2066 227b 7265 7370 6f6e 7365 7d22   = f"{response}"
-00010b10: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00010b20: 206c 6f67 6765 722e 6465 6275 6728 2254   logger.debug("T
-00010b30: 6865 2052 6573 706f 6e73 653a 2025 735c  he Response: %s\
-00010b40: 6e22 2c20 6465 6275 675f 7265 7370 6f6e  n", debug_respon
-00010b50: 7365 290a 2020 2020 2020 2020 2020 2020  se).            
-00010b60: 2020 2020 6966 2072 6573 706f 6e73 653a      if response:
-00010b70: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00010b80: 2020 2020 2074 6865 6972 6772 6964 203d       theirgrid =
-00010b90: 2072 6573 706f 6e73 652e 6765 7428 2267   response.get("g
-00010ba0: 7269 6422 290a 2020 2020 2020 2020 2020  rid").          
-00010bb0: 2020 2020 2020 2020 2020 7365 6c66 2e63            self.c
-00010bc0: 6f6e 7461 6374 5b22 4772 6964 5371 7561  ontact["GridSqua
-00010bd0: 7265 225d 203d 2074 6865 6972 6772 6964  re"] = theirgrid
-00010be0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00010bf0: 2020 2020 205f 7468 6569 7263 6f75 6e74       _theircount
-00010c00: 7279 203d 2072 6573 706f 6e73 652e 6765  ry = response.ge
-00010c10: 7428 2263 6f75 6e74 7279 2229 0a20 2020  t("country").   
-00010c20: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00010c30: 2069 6620 7365 6c66 2e73 7461 7469 6f6e   if self.station
-00010c40: 2e67 6574 2822 4772 6964 5371 7561 7265  .get("GridSquare
-00010c50: 222c 2022 2229 3a0a 2020 2020 2020 2020  ", ""):.        
-00010c60: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00010c70: 6865 6164 696e 6720 3d20 6265 6172 696e  heading = bearin
-00010c80: 6728 7365 6c66 2e73 7461 7469 6f6e 2e67  g(self.station.g
-00010c90: 6574 2822 4772 6964 5371 7561 7265 222c  et("GridSquare",
-00010ca0: 2022 2229 2c20 7468 6569 7267 7269 6429   ""), theirgrid)
-00010cb0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00010cc0: 2020 2020 2020 2020 206b 696c 6f6d 6574           kilomet
-00010cd0: 6572 7320 3d20 6469 7374 616e 6365 2873  ers = distance(s
-00010ce0: 656c 662e 7374 6174 696f 6e2e 6765 7428  elf.station.get(
-00010cf0: 2247 7269 6453 7175 6172 6522 292c 2074  "GridSquare"), t
-00010d00: 6865 6972 6772 6964 290a 2020 2020 2020  heirgrid).      
-00010d10: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00010d20: 2020 7365 6c66 2e68 6561 6469 6e67 5f64    self.heading_d
-00010d30: 6973 7461 6e63 652e 7365 7454 6578 7428  istance.setText(
-00010d40: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00010d50: 2020 2020 2020 2020 2020 2020 2066 227b               f"{
-00010d60: 7468 6569 7267 7269 647d 2048 6467 207b  theirgrid} Hdg {
-00010d70: 6865 6164 696e 677d c2b0 204c 5020 7b72  heading}.. LP {r
-00010d80: 6563 6970 726f 636f 6c28 6865 6164 696e  eciprocol(headin
-00010d90: 6729 7dc2 b020 2f20 220a 2020 2020 2020  g)}.. / ".      
-00010da0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00010db0: 2020 2020 2020 6622 6469 7374 616e 6365        f"distance
-00010dc0: 207b 696e 7428 6b69 6c6f 6d65 7465 7273   {int(kilometers
-00010dd0: 2a30 2e36 3231 3337 3129 7d6d 6920 7b6b  *0.621371)}mi {k
-00010de0: 696c 6f6d 6574 6572 737d 6b6d 220a 2020  ilometers}km".  
-00010df0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00010e00: 2020 2020 2020 290a 2020 2020 2020 2020        ).        
-00010e10: 2020 2020 2020 2020 2020 2020 2320 7365              # se
-00010e20: 6c66 2e64 785f 656e 7469 7479 2e73 6574  lf.dx_entity.set
-00010e30: 5465 7874 2866 227b 7468 6569 7263 6f75  Text(f"{theircou
-00010e40: 6e74 7279 7d22 290a 2020 2020 2020 2020  ntry}").        
-00010e50: 2020 2020 2020 2020 2320 656c 7365 3a0a          # else:.
-00010e60: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00010e70: 2320 7365 6c66 2e68 6561 6469 6e67 5f64  # self.heading_d
-00010e80: 6973 7461 6e63 652e 7365 7454 6578 7428  istance.setText(
-00010e90: 224c 6f6f 6b75 7020 6661 696c 6564 2e22  "Lookup failed."
-00010ea0: 290a 0a20 2020 2064 6566 2063 6865 636b  )..    def check
-00010eb0: 5f64 7570 6528 7365 6c66 2c20 6361 6c6c  _dupe(self, call
-00010ec0: 3a20 7374 7229 202d 3e20 626f 6f6c 3a0a  : str) -> bool:.
-00010ed0: 2020 2020 2020 2020 2222 2243 6865 636b          """Check
-00010ee0: 7320 6966 2061 2063 616c 6c73 6967 6e20  s if a callsign 
-00010ef0: 6973 2061 2064 7570 6520 6f6e 2063 7572  is a dupe on cur
-00010f00: 7265 6e74 2062 616e 642f 6d6f 6465 2e22  rent band/mode."
-00010f10: 2222 0a20 2020 2020 2020 2073 656c 662e  "".        self.
-00010f20: 636f 6e74 6573 742e 7072 6564 7570 6528  contest.predupe(
-00010f30: 7365 6c66 290a 2020 2020 2020 2020 6261  self).        ba
-00010f40: 6e64 203d 2066 6c6f 6174 2867 6574 5f6c  nd = float(get_l
-00010f50: 6f67 6765 645f 6261 6e64 2873 7472 2873  ogged_band(str(s
-00010f60: 656c 662e 7261 6469 6f5f 7374 6174 652e  elf.radio_state.
-00010f70: 6765 7428 2276 666f 6122 2c20 302e 3029  get("vfoa", 0.0)
-00010f80: 2929 290a 2020 2020 2020 2020 6d6f 6465  ))).        mode
-00010f90: 203d 2073 656c 662e 7261 6469 6f5f 7374   = self.radio_st
-00010fa0: 6174 652e 6765 7428 226d 6f64 6522 2c20  ate.get("mode", 
-00010fb0: 2222 290a 2020 2020 2020 2020 6465 6275  "").        debu
-00010fc0: 676c 696e 6520 3d20 280a 2020 2020 2020  gline = (.      
-00010fd0: 2020 2020 2020 6622 4361 6c6c 3a20 7b63        f"Call: {c
-00010fe0: 616c 6c7d 2042 616e 643a 207b 6261 6e64  all} Band: {band
-00010ff0: 7d20 4d6f 6465 3a20 7b6d 6f64 657d 2044  } Mode: {mode} D
-00011000: 7570 6574 7970 653a 207b 7365 6c66 2e63  upetype: {self.c
-00011010: 6f6e 7465 7374 2e64 7570 655f 7479 7065  ontest.dupe_type
-00011020: 7d22 0a20 2020 2020 2020 2029 0a20 2020  }".        ).   
-00011030: 2020 2020 206c 6f67 6765 722e 6465 6275       logger.debu
-00011040: 6728 2225 7322 2c20 6465 6275 676c 696e  g("%s", debuglin
-00011050: 6529 0a20 2020 2020 2020 2069 6620 7365  e).        if se
-00011060: 6c66 2e63 6f6e 7465 7374 2e64 7570 655f  lf.contest.dupe_
-00011070: 7479 7065 203d 3d20 313a 0a20 2020 2020  type == 1:.     
-00011080: 2020 2020 2020 2072 6573 756c 7420 3d20         result = 
-00011090: 7365 6c66 2e64 6174 6162 6173 652e 6368  self.database.ch
-000110a0: 6563 6b5f 6475 7065 2863 616c 6c29 0a20  eck_dupe(call). 
-000110b0: 2020 2020 2020 2069 6620 7365 6c66 2e63         if self.c
-000110c0: 6f6e 7465 7374 2e64 7570 655f 7479 7065  ontest.dupe_type
-000110d0: 203d 3d20 323a 0a20 2020 2020 2020 2020   == 2:.         
-000110e0: 2020 2072 6573 756c 7420 3d20 7365 6c66     result = self
-000110f0: 2e64 6174 6162 6173 652e 6368 6563 6b5f  .database.check_
-00011100: 6475 7065 5f6f 6e5f 6261 6e64 2863 616c  dupe_on_band(cal
-00011110: 6c2c 2062 616e 6429 0a20 2020 2020 2020  l, band).       
-00011120: 2069 6620 7365 6c66 2e63 6f6e 7465 7374   if self.contest
-00011130: 2e64 7570 655f 7479 7065 203d 3d20 333a  .dupe_type == 3:
-00011140: 0a20 2020 2020 2020 2020 2020 2072 6573  .            res
-00011150: 756c 7420 3d20 7365 6c66 2e64 6174 6162  ult = self.datab
-00011160: 6173 652e 6368 6563 6b5f 6475 7065 5f6f  ase.check_dupe_o
-00011170: 6e5f 6261 6e64 5f6d 6f64 6528 6361 6c6c  n_band_mode(call
-00011180: 2c20 6261 6e64 2c20 6d6f 6465 290a 2020  , band, mode).  
-00011190: 2020 2020 2020 6966 2073 656c 662e 636f        if self.co
-000111a0: 6e74 6573 742e 6475 7065 5f74 7970 6520  ntest.dupe_type 
-000111b0: 3d3d 2034 3a0a 2020 2020 2020 2020 2020  == 4:.          
-000111c0: 2020 7265 7375 6c74 203d 207b 2269 7364    result = {"isd
-000111d0: 7570 6522 3a20 4661 6c73 657d 0a20 2020  upe": False}.   
-000111e0: 2020 2020 2064 6562 7567 6c69 6e65 203d       debugline =
-000111f0: 2066 227b 7265 7375 6c74 7d22 0a20 2020   f"{result}".   
-00011200: 2020 2020 206c 6f67 6765 722e 6465 6275       logger.debu
-00011210: 6728 2225 7322 2c20 6465 6275 676c 696e  g("%s", debuglin
-00011220: 6529 0a20 2020 2020 2020 2072 6574 7572  e).        retur
-00011230: 6e20 7265 7375 6c74 2e67 6574 2822 6973  n result.get("is
-00011240: 6475 7065 222c 2046 616c 7365 290a 0a20  dupe", False).. 
-00011250: 2020 2064 6566 2073 6574 6d6f 6465 2873     def setmode(s
-00011260: 656c 662c 206d 6f64 653a 2073 7472 2920  elf, mode: str) 
-00011270: 2d3e 204e 6f6e 653a 0a20 2020 2020 2020  -> None:.       
-00011280: 2022 2222 7374 7562 2066 6f72 2077 6865   """stub for whe
-00011290: 6e20 7468 6520 6d6f 6465 2063 6861 6e67  n the mode chang
-000112a0: 6573 2e22 2222 0a20 2020 2020 2020 2069  es.""".        i
-000112b0: 6620 6d6f 6465 203d 3d20 2243 5722 3a0a  f mode == "CW":.
-000112c0: 2020 2020 2020 2020 2020 2020 7365 6c66              self
-000112d0: 2e63 7572 7265 6e74 5f6d 6f64 6520 3d20  .current_mode = 
-000112e0: 2243 5722 0a20 2020 2020 2020 2020 2020  "CW".           
-000112f0: 2023 2073 656c 662e 6d6f 6465 2e73 6574   # self.mode.set
-00011300: 5465 7874 2822 4357 2229 0a20 2020 2020  Text("CW").     
-00011310: 2020 2020 2020 2073 656c 662e 7365 6e74         self.sent
-00011320: 2e73 6574 5465 7874 2822 3539 3922 290a  .setText("599").
-00011330: 2020 2020 2020 2020 2020 2020 7365 6c66              self
-00011340: 2e72 6563 6569 7665 2e73 6574 5465 7874  .receive.setText
-00011350: 2822 3539 3922 290a 2020 2020 2020 2020  ("599").        
-00011360: 2020 2020 7365 6c66 2e72 6561 645f 6377      self.read_cw
-00011370: 5f6d 6163 726f 7328 290a 2020 2020 2020  _macros().      
-00011380: 2020 2020 2020 7265 7475 726e 0a20 2020        return.   
-00011390: 2020 2020 2069 6620 6d6f 6465 203d 3d20       if mode == 
-000113a0: 2253 5342 223a 0a20 2020 2020 2020 2020  "SSB":.         
-000113b0: 2020 2073 656c 662e 6375 7272 656e 745f     self.current_
-000113c0: 6d6f 6465 203d 2022 5353 4222 0a20 2020  mode = "SSB".   
-000113d0: 2020 2020 2020 2020 2023 2073 656c 662e           # self.
-000113e0: 6d6f 6465 2e73 6574 5465 7874 2822 5353  mode.setText("SS
-000113f0: 4222 290a 2020 2020 2020 2020 2020 2020  B").            
-00011400: 7365 6c66 2e73 656e 742e 7365 7454 6578  self.sent.setTex
-00011410: 7428 2235 3922 290a 2020 2020 2020 2020  t("59").        
-00011420: 2020 2020 7365 6c66 2e72 6563 6569 7665      self.receive
-00011430: 2e73 6574 5465 7874 2822 3539 2229 0a20  .setText("59"). 
-00011440: 2020 2020 2020 2020 2020 2073 656c 662e             self.
-00011450: 7265 6164 5f63 775f 6d61 6372 6f73 2829  read_cw_macros()
-00011460: 0a20 2020 2020 2020 2069 6620 6d6f 6465  .        if mode
-00011470: 203d 3d20 2252 5454 5922 3a0a 2020 2020   == "RTTY":.    
-00011480: 2020 2020 2020 2020 7365 6c66 2e63 7572          self.cur
-00011490: 7265 6e74 5f6d 6f64 6520 3d20 2252 5454  rent_mode = "RTT
-000114a0: 5922 0a20 2020 2020 2020 2020 2020 2023  Y".            #
-000114b0: 2073 656c 662e 6d6f 6465 2e73 6574 5465   self.mode.setTe
-000114c0: 7874 2822 5254 5459 2229 0a20 2020 2020  xt("RTTY").     
-000114d0: 2020 2020 2020 2073 656c 662e 7365 6e74         self.sent
-000114e0: 2e73 6574 5465 7874 2822 3539 2229 0a20  .setText("59"). 
-000114f0: 2020 2020 2020 2020 2020 2073 656c 662e             self.
-00011500: 7265 6365 6976 652e 7365 7454 6578 7428  receive.setText(
-00011510: 2235 3922 290a 0a20 2020 2064 6566 2067  "59")..    def g
-00011520: 6574 5f6f 706f 6e28 7365 6c66 293a 0a20  et_opon(self):. 
-00011530: 2020 2020 2020 2022 2222 4374 726c 2b4f         """Ctrl+O
-00011540: 206f 7220 4f50 4f4e 2064 6961 6c6f 6722   or OPON dialog"
-00011550: 2222 0a20 2020 2020 2020 2073 656c 662e  "".        self.
-00011560: 6f70 6f6e 5f64 6961 6c6f 6720 3d20 4f70  opon_dialog = Op
-00011570: 4f6e 2857 4f52 4b49 4e47 5f50 4154 4829  On(WORKING_PATH)
-00011580: 0a20 2020 2020 2020 2073 656c 662e 6f70  .        self.op
-00011590: 6f6e 5f64 6961 6c6f 672e 6163 6365 7074  on_dialog.accept
-000115a0: 6564 2e63 6f6e 6e65 6374 2873 656c 662e  ed.connect(self.
-000115b0: 6e65 775f 6f70 290a 2020 2020 2020 2020  new_op).        
-000115c0: 7365 6c66 2e6f 706f 6e5f 6469 616c 6f67  self.opon_dialog
-000115d0: 2e6f 7065 6e28 290a 0a20 2020 2064 6566  .open()..    def
-000115e0: 206e 6577 5f6f 7028 7365 6c66 293a 0a20   new_op(self):. 
-000115f0: 2020 2020 2020 2022 2222 5361 7665 206e         """Save n
-00011600: 6577 204f 5022 2222 0a20 2020 2020 2020  ew OP""".       
-00011610: 2069 6620 7365 6c66 2e6f 706f 6e5f 6469   if self.opon_di
-00011620: 616c 6f67 2e4e 6577 4f70 6572 6174 6f72  alog.NewOperator
-00011630: 2e74 6578 7428 293a 0a20 2020 2020 2020  .text():.       
-00011640: 2020 2020 2073 656c 662e 6375 7272 656e       self.curren
-00011650: 745f 6f70 203d 2073 656c 662e 6f70 6f6e  t_op = self.opon
-00011660: 5f64 6961 6c6f 672e 4e65 774f 7065 7261  _dialog.NewOpera
-00011670: 746f 722e 7465 7874 2829 2e75 7070 6572  tor.text().upper
-00011680: 2829 0a20 2020 2020 2020 2073 656c 662e  ().        self.
-00011690: 6f70 6f6e 5f64 6961 6c6f 672e 636c 6f73  opon_dialog.clos
-000116a0: 6528 290a 2020 2020 2020 2020 6c6f 6767  e().        logg
-000116b0: 6572 2e64 6562 7567 2822 4e65 7720 4f70  er.debug("New Op
-000116c0: 3a20 2573 222c 2073 656c 662e 6375 7272  : %s", self.curr
-000116d0: 656e 745f 6f70 290a 2020 2020 2020 2020  ent_op).        
-000116e0: 7365 6c66 2e6d 616b 655f 6f70 5f64 6972  self.make_op_dir
-000116f0: 2829 0a0a 2020 2020 6465 6620 6d61 6b65  ()..    def make
-00011700: 5f6f 705f 6469 7228 7365 6c66 293a 0a20  _op_dir(self):. 
-00011710: 2020 2020 2020 2022 2222 4372 6561 7465         """Create
-00011720: 204f 5020 6469 7265 6374 6f72 7920 6966   OP directory if
-00011730: 2069 7420 646f 6573 206e 6f74 2065 7869   it does not exi
-00011740: 7374 2e22 2222 0a20 2020 2020 2020 2069  st.""".        i
-00011750: 6620 7365 6c66 2e63 7572 7265 6e74 5f6f  f self.current_o
-00011760: 703a 0a20 2020 2020 2020 2020 2020 206f  p:.            o
-00011770: 705f 7061 7468 203d 2050 6174 6828 4441  p_path = Path(DA
-00011780: 5441 5f50 4154 4829 202f 2073 656c 662e  TA_PATH) / self.
-00011790: 6375 7272 656e 745f 6f70 0a20 2020 2020  current_op.     
-000117a0: 2020 2020 2020 206c 6f67 6765 722e 6465         logger.de
-000117b0: 6275 6728 226f 705f 7061 7468 3a20 2573  bug("op_path: %s
-000117c0: 222c 2073 7472 286f 705f 7061 7468 2929  ", str(op_path))
-000117d0: 0a20 2020 2020 2020 2020 2020 2069 6620  .            if 
-000117e0: 6f70 5f70 6174 682e 6973 5f64 6972 2829  op_path.is_dir()
-000117f0: 2069 7320 4661 6c73 653a 0a20 2020 2020   is False:.     
-00011800: 2020 2020 2020 2020 2020 206c 6f67 6765             logge
-00011810: 722e 6465 6275 6728 2243 7265 6174 696e  r.debug("Creatin
-00011820: 6720 4f70 2044 6972 6563 746f 7279 3a20  g Op Directory: 
-00011830: 2573 222c 2073 7472 286f 705f 7061 7468  %s", str(op_path
-00011840: 2929 0a20 2020 2020 2020 2020 2020 2020  )).             
-00011850: 2020 206f 732e 6d6b 6469 7228 7374 7228     os.mkdir(str(
-00011860: 6f70 5f70 6174 6829 290a 2020 2020 2020  op_path)).      
-00011870: 2020 2020 2020 6966 206f 705f 7061 7468        if op_path
-00011880: 2e69 735f 6469 7228 293a 0a20 2020 2020  .is_dir():.     
-00011890: 2020 2020 2020 2020 2020 2073 6f75 7263             sourc
-000118a0: 655f 7061 7468 203d 2050 6174 6828 574f  e_path = Path(WO
-000118b0: 524b 494e 475f 5041 5448 2920 2f20 2264  RKING_PATH) / "d
-000118c0: 6174 6122 202f 2022 7068 6f6e 6574 6963  ata" / "phonetic
-000118d0: 7322 0a20 2020 2020 2020 2020 2020 2020  s".             
-000118e0: 2020 206c 6f67 6765 722e 6465 6275 6728     logger.debug(
-000118f0: 2273 6f75 7263 655f 7061 7468 3a20 2573  "source_path: %s
-00011900: 222c 2073 7472 2873 6f75 7263 655f 7061  ", str(source_pa
-00011910: 7468 2929 0a20 2020 2020 2020 2020 2020  th)).           
-00011920: 2020 2020 2066 6f72 2063 6869 6c64 2069       for child i
-00011930: 6e20 736f 7572 6365 5f70 6174 682e 6974  n source_path.it
-00011940: 6572 6469 7228 293a 0a20 2020 2020 2020  erdir():.       
-00011950: 2020 2020 2020 2020 2020 2020 2064 6573               des
-00011960: 7469 6e61 7469 6f6e 5f66 696c 6520 3d20  tination_file = 
-00011970: 6f70 5f70 6174 6820 2f20 6368 696c 642e  op_path / child.
-00011980: 6e61 6d65 0a20 2020 2020 2020 2020 2020  name.           
-00011990: 2020 2020 2020 2020 2069 6620 6465 7374           if dest
-000119a0: 696e 6174 696f 6e5f 6669 6c65 2e69 735f  ination_file.is_
-000119b0: 6669 6c65 2829 2069 7320 4661 6c73 653a  file() is False:
-000119c0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-000119d0: 2020 2020 2020 2020 206c 6f67 6765 722e           logger.
-000119e0: 6465 6275 6728 2244 6573 7469 6e61 7469  debug("Destinati
-000119f0: 6f6e 3a20 2573 222c 2073 7472 2864 6573  on: %s", str(des
-00011a00: 7469 6e61 7469 6f6e 5f66 696c 6529 290a  tination_file)).
-00011a10: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00011a20: 2020 2020 2020 2020 6465 7374 696e 6174          destinat
-00011a30: 696f 6e5f 6669 6c65 2e77 7269 7465 5f62  ion_file.write_b
-00011a40: 7974 6573 2863 6869 6c64 2e72 6561 645f  ytes(child.read_
-00011a50: 6279 7465 7328 2929 0a0a 2020 2020 6465  bytes())..    de
-00011a60: 6620 706f 6c6c 5f72 6164 696f 2873 656c  f poll_radio(sel
-00011a70: 6629 3a0a 2020 2020 2020 2020 2222 2273  f):.        """s
-00011a80: 7475 6222 2222 0a20 2020 2020 2020 2069  tub""".        i
-00011a90: 6620 7365 6c66 2e72 6967 5f63 6f6e 7472  f self.rig_contr
-00011aa0: 6f6c 3a0a 2020 2020 2020 2020 2020 2020  ol:.            
-00011ab0: 6966 2073 656c 662e 7269 675f 636f 6e74  if self.rig_cont
-00011ac0: 726f 6c2e 6f6e 6c69 6e65 3a0a 2020 2020  rol.online:.    
-00011ad0: 2020 2020 2020 2020 2020 2020 7666 6f20              vfo 
-00011ae0: 3d20 7365 6c66 2e72 6967 5f63 6f6e 7472  = self.rig_contr
-00011af0: 6f6c 2e67 6574 5f76 666f 2829 0a20 2020  ol.get_vfo().   
-00011b00: 2020 2020 2020 2020 2020 2020 206d 6f64               mod
-00011b10: 6520 3d20 7365 6c66 2e72 6967 5f63 6f6e  e = self.rig_con
-00011b20: 7472 6f6c 2e67 6574 5f6d 6f64 6528 290a  trol.get_mode().
-00011b30: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00011b40: 6277 203d 2073 656c 662e 7269 675f 636f  bw = self.rig_co
-00011b50: 6e74 726f 6c2e 6765 745f 6277 2829 0a20  ntrol.get_bw(). 
-00011b60: 2020 2020 2020 2020 2020 2020 2020 2023                 #
-00011b70: 2073 656c 662e 7261 6469 6f5f 7374 6174   self.radio_stat
-00011b80: 655b 2270 7474 225d 203d 2073 656c 662e  e["ptt"] = self.
-00011b90: 7269 675f 636f 6e74 726f 6c2e 6765 745f  rig_control.get_
-00011ba0: 7074 7428 290a 2020 2020 2020 2020 2020  ptt().          
-00011bb0: 2020 2020 2020 2320 6966 2073 656c 662e        # if self.
-00011bc0: 7261 6469 6f5f 7374 6174 652e 6765 7428  radio_state.get(
-00011bd0: 2270 7474 222c 2030 2920 3d3d 2031 3a0a  "ptt", 0) == 1:.
-00011be0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00011bf0: 2320 2020 2020 7365 6c66 2e6c 6566 7464  #     self.leftd
-00011c00: 6f74 2e73 6574 5069 786d 6170 2873 656c  ot.setPixmap(sel
-00011c10: 662e 6772 6565 6e64 6f74 290a 2020 2020  f.greendot).    
-00011c20: 2020 2020 2020 2020 2020 2020 2320 656c              # el
-00011c30: 7365 3a0a 2020 2020 2020 2020 2020 2020  se:.            
-00011c40: 2020 2020 2320 2020 2020 7365 6c66 2e6c      #     self.l
-00011c50: 6566 7464 6f74 2e73 6574 5069 786d 6170  eftdot.setPixmap
-00011c60: 2873 656c 662e 7265 6464 6f74 290a 2020  (self.reddot).  
-00011c70: 2020 2020 2020 2020 2020 2020 2020 6966                if
-00011c80: 206d 6f64 6520 3d3d 2022 4357 223a 0a20   mode == "CW":. 
-00011c90: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00011ca0: 2020 2073 656c 662e 7365 746d 6f64 6528     self.setmode(
-00011cb0: 6d6f 6465 290a 2020 2020 2020 2020 2020  mode).          
-00011cc0: 2020 2020 2020 6966 206d 6f64 6520 3d3d        if mode ==
-00011cd0: 2022 4c53 4222 206f 7220 6d6f 6465 203d   "LSB" or mode =
-00011ce0: 3d20 2255 5342 223a 0a20 2020 2020 2020  = "USB":.       
-00011cf0: 2020 2020 2020 2020 2020 2020 2073 656c               sel
-00011d00: 662e 7365 746d 6f64 6528 2253 5342 2229  f.setmode("SSB")
-00011d10: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00011d20: 2069 6620 6d6f 6465 203d 3d20 2252 5454   if mode == "RTT
-00011d30: 5922 3a0a 2020 2020 2020 2020 2020 2020  Y":.            
-00011d40: 2020 2020 2020 2020 7365 6c66 2e73 6574          self.set
-00011d50: 6d6f 6465 2822 5254 5459 2229 0a20 2020  mode("RTTY").   
-00011d60: 2020 2020 2020 2020 2020 2020 2073 656c               sel
-00011d70: 662e 7261 6469 6f5f 7374 6174 655b 2276  f.radio_state["v
-00011d80: 666f 6122 5d20 3d20 7666 6f0a 2020 2020  foa"] = vfo.    
-00011d90: 2020 2020 2020 2020 2020 2020 6261 6e64              band
-00011da0: 203d 2067 6574 6261 6e64 2873 7472 2876   = getband(str(v
-00011db0: 666f 2929 0a20 2020 2020 2020 2020 2020  fo)).           
-00011dc0: 2020 2020 2073 656c 662e 7261 6469 6f5f       self.radio_
-00011dd0: 7374 6174 655b 2262 616e 6422 5d20 3d20  state["band"] = 
-00011de0: 6261 6e64 0a20 2020 2020 2020 2020 2020  band.           
-00011df0: 2020 2020 2073 656c 662e 636f 6e74 6163       self.contac
-00011e00: 745b 2242 616e 6422 5d20 3d20 6765 745f  t["Band"] = get_
-00011e10: 6c6f 6767 6564 5f62 616e 6428 7374 7228  logged_band(str(
-00011e20: 7666 6f29 290a 2020 2020 2020 2020 2020  vfo)).          
-00011e30: 2020 2020 2020 7365 6c66 2e73 6574 5f62        self.set_b
-00011e40: 616e 645f 696e 6469 6361 746f 7228 6261  and_indicator(ba
-00011e50: 6e64 290a 2020 2020 2020 2020 2020 2020  nd).            
-00011e60: 2020 2020 7365 6c66 2e72 6164 696f 5f73      self.radio_s
-00011e70: 7461 7465 5b22 6d6f 6465 225d 203d 206d  tate["mode"] = m
-00011e80: 6f64 650a 2020 2020 2020 2020 2020 2020  ode.            
-00011e90: 2020 2020 7365 6c66 2e72 6164 696f 5f73      self.radio_s
-00011ea0: 7461 7465 5b22 6277 225d 203d 2062 770a  tate["bw"] = bw.
-00011eb0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00011ec0: 6c6f 6767 6572 2e64 6562 7567 2822 5646  logger.debug("VF
-00011ed0: 4f3a 2025 7320 204d 4f44 453a 2025 7320  O: %s  MODE: %s 
-00011ee0: 4257 3a20 2573 222c 2076 666f 2c20 6d6f  BW: %s", vfo, mo
-00011ef0: 6465 2c20 6277 290a 2020 2020 2020 2020  de, bw).        
-00011f00: 2020 2020 2020 2020 7365 6c66 2e73 6574          self.set
-00011f10: 5f77 696e 646f 775f 7469 746c 6528 290a  _window_title().
-00011f20: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00011f30: 636d 6420 3d20 7b7d 0a20 2020 2020 2020  cmd = {}.       
-00011f40: 2020 2020 2020 2020 2063 6d64 5b22 636d           cmd["cm
-00011f50: 6422 5d20 3d20 2252 4144 494f 5f53 5441  d"] = "RADIO_STA
-00011f60: 5445 220a 2020 2020 2020 2020 2020 2020  TE".            
-00011f70: 2020 2020 636d 645b 2273 7461 7469 6f6e      cmd["station
-00011f80: 225d 203d 2070 6c61 7466 6f72 6d2e 6e6f  "] = platform.no
-00011f90: 6465 2829 0a20 2020 2020 2020 2020 2020  de().           
-00011fa0: 2020 2020 2063 6d64 5b22 6261 6e64 225d       cmd["band"]
-00011fb0: 203d 2062 616e 640a 2020 2020 2020 2020   = band.        
-00011fc0: 2020 2020 2020 2020 636d 645b 2276 666f          cmd["vfo
-00011fd0: 6122 5d20 3d20 7666 6f0a 2020 2020 2020  a"] = vfo.      
-00011fe0: 2020 2020 2020 2020 2020 636d 645b 226d            cmd["m
-00011ff0: 6f64 6522 5d20 3d20 6d6f 6465 0a20 2020  ode"] = mode.   
-00012000: 2020 2020 2020 2020 2020 2020 2063 6d64               cmd
-00012010: 5b22 6277 225d 203d 2062 770a 2020 2020  ["bw"] = bw.    
-00012020: 2020 2020 2020 2020 2020 2020 7365 6c66              self
-00012030: 2e6d 756c 7469 6361 7374 5f69 6e74 6572  .multicast_inter
-00012040: 6661 6365 2e73 656e 645f 6173 5f6a 736f  face.send_as_jso
-00012050: 6e28 636d 6429 0a0a 2020 2020 6465 6620  n(cmd)..    def 
-00012060: 6564 6974 5f63 775f 6d61 6372 6f73 2873  edit_cw_macros(s
-00012070: 656c 6629 202d 3e20 4e6f 6e65 3a0a 2020  elf) -> None:.  
-00012080: 2020 2020 2020 2222 220a 2020 2020 2020        """.      
-00012090: 2020 4361 6c6c 7320 7468 6520 6465 6661    Calls the defa
-000120a0: 756c 7420 7465 7874 2065 6469 746f 7220  ult text editor 
-000120b0: 746f 2065 6469 7420 7468 6520 4357 206d  to edit the CW m
-000120c0: 6163 726f 2066 696c 652e 0a20 2020 2020  acro file..     
-000120d0: 2020 2022 2222 0a20 2020 2020 2020 2069     """.        i
-000120e0: 6620 7365 6c66 2e72 6164 696f 5f73 7461  f self.radio_sta
-000120f0: 7465 2e67 6574 2822 6d6f 6465 2229 203d  te.get("mode") =
-00012100: 3d20 2243 5722 3a0a 2020 2020 2020 2020  = "CW":.        
-00012110: 2020 2020 6d61 6372 6f5f 6669 6c65 203d      macro_file =
-00012120: 2022 2f63 776d 6163 726f 732e 7478 7422   "/cwmacros.txt"
-00012130: 0a20 2020 2020 2020 2065 6c73 653a 0a20  .        else:. 
-00012140: 2020 2020 2020 2020 2020 206d 6163 726f             macro
-00012150: 5f66 696c 6520 3d20 222f 7373 626d 6163  _file = "/ssbmac
-00012160: 726f 732e 7478 7422 0a20 2020 2020 2020  ros.txt".       
-00012170: 2069 6620 6e6f 7420 5061 7468 2844 4154   if not Path(DAT
-00012180: 415f 5041 5448 202b 206d 6163 726f 5f66  A_PATH + macro_f
-00012190: 696c 6529 2e65 7869 7374 7328 293a 0a20  ile).exists():. 
-000121a0: 2020 2020 2020 2020 2020 206c 6f67 6765             logge
-000121b0: 722e 6465 6275 6728 2272 6561 645f 6377  r.debug("read_cw
-000121c0: 5f6d 6163 726f 733a 2063 6f70 7969 6e67  _macros: copying
-000121d0: 2064 6566 6175 6c74 206d 6163 726f 2066   default macro f
-000121e0: 696c 652e 2229 0a20 2020 2020 2020 2020  ile.").         
-000121f0: 2020 2063 6f70 7966 696c 6528 574f 524b     copyfile(WORK
-00012200: 494e 475f 5041 5448 202b 2022 2f64 6174  ING_PATH + "/dat
-00012210: 6122 202b 206d 6163 726f 5f66 696c 652c  a" + macro_file,
-00012220: 2044 4154 415f 5041 5448 202b 206d 6163   DATA_PATH + mac
-00012230: 726f 5f66 696c 6529 0a20 2020 2020 2020  ro_file).       
-00012240: 206f 732e 7379 7374 656d 2866 2278 6467   os.system(f"xdg
-00012250: 2d6f 7065 6e20 7b44 4154 415f 5041 5448  -open {DATA_PATH
-00012260: 7d7b 6d61 6372 6f5f 6669 6c65 7d22 290a  }{macro_file}").
-00012270: 0a20 2020 2064 6566 2072 6561 645f 6377  .    def read_cw
-00012280: 5f6d 6163 726f 7328 7365 6c66 2920 2d3e  _macros(self) ->
-00012290: 204e 6f6e 653a 0a20 2020 2020 2020 2022   None:.        "
-000122a0: 2222 0a20 2020 2020 2020 2052 6561 6473  "".        Reads
-000122b0: 2069 6e20 7468 6520 4357 206d 6163 726f   in the CW macro
-000122c0: 732c 2066 6972 7374 7320 6974 2063 6865  s, firsts it che
-000122d0: 636b 7320 746f 2073 6565 2069 6620 7468  cks to see if th
-000122e0: 6520 6669 6c65 2065 7869 7374 732e 2049  e file exists. I
-000122f0: 6620 6974 2064 6f65 7320 6e6f 742c 0a20  f it does not,. 
-00012300: 2020 2020 2020 2061 6e64 2074 6869 7320         and this 
-00012310: 6861 7320 6265 656e 2070 6163 6b61 6765  has been package
-00012320: 6420 7769 7468 2070 7969 6e73 7461 6c6c  d with pyinstall
-00012330: 6572 2069 7420 7769 6c6c 2063 6f70 7920  er it will copy 
-00012340: 7468 6520 6465 6661 756c 7420 6669 6c65  the default file
-00012350: 2066 726f 6d20 7468 650a 2020 2020 2020   from the.      
-00012360: 2020 7465 6d70 2064 6972 6563 746f 7279    temp directory
-00012370: 2074 6869 7320 6973 2072 756e 6e69 6e67   this is running
-00012380: 2066 726f 6d2e 2e2e 2049 6e20 7468 656f   from... In theo
-00012390: 7279 2e0a 2020 2020 2020 2020 2222 220a  ry..        """.
-000123a0: 0a20 2020 2020 2020 2069 6620 7365 6c66  .        if self
-000123b0: 2e72 6164 696f 5f73 7461 7465 2e67 6574  .radio_state.get
-000123c0: 2822 6d6f 6465 2229 203d 3d20 2243 5722  ("mode") == "CW"
-000123d0: 3a0a 2020 2020 2020 2020 2020 2020 6d61  :.            ma
-000123e0: 6372 6f5f 6669 6c65 203d 2022 2f63 776d  cro_file = "/cwm
-000123f0: 6163 726f 732e 7478 7422 0a20 2020 2020  acros.txt".     
-00012400: 2020 2065 6c73 653a 0a20 2020 2020 2020     else:.       
-00012410: 2020 2020 206d 6163 726f 5f66 696c 6520       macro_file 
-00012420: 3d20 222f 7373 626d 6163 726f 732e 7478  = "/ssbmacros.tx
-00012430: 7422 0a0a 2020 2020 2020 2020 6966 206e  t"..        if n
-00012440: 6f74 2050 6174 6828 4441 5441 5f50 4154  ot Path(DATA_PAT
-00012450: 4820 2b20 6d61 6372 6f5f 6669 6c65 292e  H + macro_file).
-00012460: 6578 6973 7473 2829 3a0a 2020 2020 2020  exists():.      
-00012470: 2020 2020 2020 6c6f 6767 6572 2e64 6562        logger.deb
-00012480: 7567 2822 7265 6164 5f63 775f 6d61 6372  ug("read_cw_macr
-00012490: 6f73 3a20 636f 7079 696e 6720 6465 6661  os: copying defa
-000124a0: 756c 7420 6d61 6372 6f20 6669 6c65 2e22  ult macro file."
-000124b0: 290a 2020 2020 2020 2020 2020 2020 636f  ).            co
-000124c0: 7079 6669 6c65 2857 4f52 4b49 4e47 5f50  pyfile(WORKING_P
-000124d0: 4154 4820 2b20 222f 6461 7461 2220 2b20  ATH + "/data" + 
-000124e0: 6d61 6372 6f5f 6669 6c65 2c20 4441 5441  macro_file, DATA
-000124f0: 5f50 4154 4820 2b20 6d61 6372 6f5f 6669  _PATH + macro_fi
-00012500: 6c65 290a 2020 2020 2020 2020 7769 7468  le).        with
-00012510: 206f 7065 6e28 4441 5441 5f50 4154 4820   open(DATA_PATH 
-00012520: 2b20 6d61 6372 6f5f 6669 6c65 2c20 2272  + macro_file, "r
-00012530: 222c 2065 6e63 6f64 696e 673d 2275 7466  ", encoding="utf
-00012540: 2d38 2229 2061 7320 6669 6c65 5f64 6573  -8") as file_des
-00012550: 6372 6970 746f 723a 0a20 2020 2020 2020  criptor:.       
-00012560: 2020 2020 2066 6f72 206c 696e 6520 696e       for line in
-00012570: 2066 696c 655f 6465 7363 7269 7074 6f72   file_descriptor
-00012580: 3a0a 2020 2020 2020 2020 2020 2020 2020  :.              
-00012590: 2020 7472 793a 0a20 2020 2020 2020 2020    try:.         
-000125a0: 2020 2020 2020 2020 2020 206d 6f64 652c             mode,
-000125b0: 2066 6b65 792c 2062 7574 746f 6e6e 616d   fkey, buttonnam
-000125c0: 652c 2063 7774 6578 7420 3d20 6c69 6e65  e, cwtext = line
-000125d0: 2e73 706c 6974 2822 7c22 290a 2020 2020  .split("|").    
-000125e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000125f0: 6966 206d 6f64 652e 7374 7269 7028 292e  if mode.strip().
-00012600: 7570 7065 7228 2920 3d3d 2022 5222 2061  upper() == "R" a
-00012610: 6e64 2073 656c 662e 7072 6566 2e67 6574  nd self.pref.get
-00012620: 2822 7275 6e5f 7374 6174 6522 293a 0a20  ("run_state"):. 
-00012630: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00012640: 2020 2020 2020 2073 656c 662e 666b 6579         self.fkey
-00012650: 735b 666b 6579 2e73 7472 6970 2829 5d20  s[fkey.strip()] 
-00012660: 3d20 2862 7574 746f 6e6e 616d 652e 7374  = (buttonname.st
-00012670: 7269 7028 292c 2063 7774 6578 742e 7374  rip(), cwtext.st
-00012680: 7269 7028 2929 0a20 2020 2020 2020 2020  rip()).         
-00012690: 2020 2020 2020 2020 2020 2069 6620 6d6f             if mo
-000126a0: 6465 2e73 7472 6970 2829 2e75 7070 6572  de.strip().upper
-000126b0: 2829 2021 3d20 2252 2220 616e 6420 6e6f  () != "R" and no
-000126c0: 7420 7365 6c66 2e70 7265 662e 6765 7428  t self.pref.get(
-000126d0: 2272 756e 5f73 7461 7465 2229 3a0a 2020  "run_state"):.  
-000126e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000126f0: 2020 2020 2020 7365 6c66 2e66 6b65 7973        self.fkeys
-00012700: 5b66 6b65 792e 7374 7269 7028 295d 203d  [fkey.strip()] =
-00012710: 2028 6275 7474 6f6e 6e61 6d65 2e73 7472   (buttonname.str
-00012720: 6970 2829 2c20 6377 7465 7874 2e73 7472  ip(), cwtext.str
-00012730: 6970 2829 290a 2020 2020 2020 2020 2020  ip()).          
-00012740: 2020 2020 2020 6578 6365 7074 2056 616c        except Val
-00012750: 7565 4572 726f 7220 6173 2065 7272 3a0a  ueError as err:.
+00010940: 6620 6c65 6e28 6361 6c6c 7369 676e 2920  f len(callsign) 
+00010950: 3e20 323a 0a20 2020 2020 2020 2020 2020  > 2:.           
+00010960: 2020 2020 2020 2020 2069 6620 7365 6c66           if self
+00010970: 2e63 6f6e 7465 7374 3a0a 2020 2020 2020  .contest:.      
+00010980: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00010990: 2020 7365 6c66 2e63 6f6e 7465 7374 2e70    self.contest.p
+000109a0: 7265 6669 6c6c 2873 656c 6629 0a0a 2020  refill(self)..  
+000109b0: 2020 6465 6620 6368 6563 6b5f 6361 6c6c    def check_call
+000109c0: 7369 676e 3228 7365 6c66 2c20 6361 6c6c  sign2(self, call
+000109d0: 7369 676e 293a 0a20 2020 2020 2020 2022  sign):.        "
+000109e0: 2222 4368 6563 6b20 6361 6c6c 206f 6e63  ""Check call onc
+000109f0: 6520 656e 7465 7265 6422 2222 0a20 2020  e entered""".   
+00010a00: 2020 2020 2063 616c 6c73 6967 6e20 3d20       callsign = 
+00010a10: 6361 6c6c 7369 676e 2e73 7472 6970 2829  callsign.strip()
+00010a20: 0a20 2020 2020 2020 2064 6562 7567 5f6c  .        debug_l
+00010a30: 6f6f 6b75 7020 3d20 6622 7b73 656c 662e  ookup = f"{self.
+00010a40: 6c6f 6f6b 5f75 707d 220a 2020 2020 2020  look_up}".      
+00010a50: 2020 6c6f 6767 6572 2e64 6562 7567 2822    logger.debug("
+00010a60: 2573 2c20 2573 222c 2063 616c 6c73 6967  %s, %s", callsig
+00010a70: 6e2c 2064 6562 7567 5f6c 6f6f 6b75 7029  n, debug_lookup)
+00010a80: 0a20 2020 2020 2020 2069 6620 6861 7361  .        if hasa
+00010a90: 7474 7228 7365 6c66 2e6c 6f6f 6b5f 7570  ttr(self.look_up
+00010aa0: 2c20 2273 6573 7369 6f6e 2229 3a0a 2020  , "session"):.  
+00010ab0: 2020 2020 2020 2020 2020 6966 2073 656c            if sel
+00010ac0: 662e 6c6f 6f6b 5f75 702e 7365 7373 696f  f.look_up.sessio
+00010ad0: 6e3a 0a20 2020 2020 2020 2020 2020 2020  n:.             
+00010ae0: 2020 2072 6573 706f 6e73 6520 3d20 7365     response = se
+00010af0: 6c66 2e6c 6f6f 6b5f 7570 2e6c 6f6f 6b75  lf.look_up.looku
+00010b00: 7028 6361 6c6c 7369 676e 290a 2020 2020  p(callsign).    
+00010b10: 2020 2020 2020 2020 2020 2020 6465 6275              debu
+00010b20: 675f 7265 7370 6f6e 7365 203d 2066 227b  g_response = f"{
+00010b30: 7265 7370 6f6e 7365 7d22 0a20 2020 2020  response}".     
+00010b40: 2020 2020 2020 2020 2020 206c 6f67 6765             logge
+00010b50: 722e 6465 6275 6728 2254 6865 2052 6573  r.debug("The Res
+00010b60: 706f 6e73 653a 2025 735c 6e22 2c20 6465  ponse: %s\n", de
+00010b70: 6275 675f 7265 7370 6f6e 7365 290a 2020  bug_response).  
+00010b80: 2020 2020 2020 2020 2020 2020 2020 6966                if
+00010b90: 2072 6573 706f 6e73 653a 0a20 2020 2020   response:.     
+00010ba0: 2020 2020 2020 2020 2020 2020 2020 2074                 t
+00010bb0: 6865 6972 6772 6964 203d 2072 6573 706f  heirgrid = respo
+00010bc0: 6e73 652e 6765 7428 2267 7269 6422 290a  nse.get("grid").
+00010bd0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00010be0: 2020 2020 7365 6c66 2e63 6f6e 7461 6374      self.contact
+00010bf0: 5b22 4772 6964 5371 7561 7265 225d 203d  ["GridSquare"] =
+00010c00: 2074 6865 6972 6772 6964 0a20 2020 2020   theirgrid.     
+00010c10: 2020 2020 2020 2020 2020 2020 2020 205f                 _
+00010c20: 7468 6569 7263 6f75 6e74 7279 203d 2072  theircountry = r
+00010c30: 6573 706f 6e73 652e 6765 7428 2263 6f75  esponse.get("cou
+00010c40: 6e74 7279 2229 0a20 2020 2020 2020 2020  ntry").         
+00010c50: 2020 2020 2020 2020 2020 2069 6620 7365             if se
+00010c60: 6c66 2e73 7461 7469 6f6e 2e67 6574 2822  lf.station.get("
+00010c70: 4772 6964 5371 7561 7265 222c 2022 2229  GridSquare", "")
+00010c80: 3a0a 2020 2020 2020 2020 2020 2020 2020  :.              
+00010c90: 2020 2020 2020 2020 2020 6865 6164 696e            headin
+00010ca0: 6720 3d20 6265 6172 696e 6728 7365 6c66  g = bearing(self
+00010cb0: 2e73 7461 7469 6f6e 2e67 6574 2822 4772  .station.get("Gr
+00010cc0: 6964 5371 7561 7265 222c 2022 2229 2c20  idSquare", ""), 
+00010cd0: 7468 6569 7267 7269 6429 0a20 2020 2020  theirgrid).     
+00010ce0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00010cf0: 2020 206b 696c 6f6d 6574 6572 7320 3d20     kilometers = 
+00010d00: 6469 7374 616e 6365 2873 656c 662e 7374  distance(self.st
+00010d10: 6174 696f 6e2e 6765 7428 2247 7269 6453  ation.get("GridS
+00010d20: 7175 6172 6522 292c 2074 6865 6972 6772  quare"), theirgr
+00010d30: 6964 290a 2020 2020 2020 2020 2020 2020  id).            
+00010d40: 2020 2020 2020 2020 2020 2020 7365 6c66              self
+00010d50: 2e68 6561 6469 6e67 5f64 6973 7461 6e63  .heading_distanc
+00010d60: 652e 7365 7454 6578 7428 0a20 2020 2020  e.setText(.     
+00010d70: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00010d80: 2020 2020 2020 2066 227b 7468 6569 7267         f"{theirg
+00010d90: 7269 647d 2048 6467 207b 6865 6164 696e  rid} Hdg {headin
+00010da0: 677d c2b0 204c 5020 7b72 6563 6970 726f  g}.. LP {recipro
+00010db0: 636f 6c28 6865 6164 696e 6729 7dc2 b020  col(heading)}.. 
+00010dc0: 2f20 220a 2020 2020 2020 2020 2020 2020  / ".            
+00010dd0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00010de0: 6622 6469 7374 616e 6365 207b 696e 7428  f"distance {int(
+00010df0: 6b69 6c6f 6d65 7465 7273 2a30 2e36 3231  kilometers*0.621
+00010e00: 3337 3129 7d6d 6920 7b6b 696c 6f6d 6574  371)}mi {kilomet
+00010e10: 6572 737d 6b6d 220a 2020 2020 2020 2020  ers}km".        
+00010e20: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00010e30: 290a 2020 2020 2020 2020 2020 2020 2020  ).              
+00010e40: 2020 2020 2020 2320 7365 6c66 2e64 785f        # self.dx_
+00010e50: 656e 7469 7479 2e73 6574 5465 7874 2866  entity.setText(f
+00010e60: 227b 7468 6569 7263 6f75 6e74 7279 7d22  "{theircountry}"
+00010e70: 290a 2020 2020 2020 2020 2020 2020 2020  ).              
+00010e80: 2020 2320 656c 7365 3a0a 2020 2020 2020    # else:.      
+00010e90: 2020 2020 2020 2020 2020 2320 7365 6c66            # self
+00010ea0: 2e68 6561 6469 6e67 5f64 6973 7461 6e63  .heading_distanc
+00010eb0: 652e 7365 7454 6578 7428 224c 6f6f 6b75  e.setText("Looku
+00010ec0: 7020 6661 696c 6564 2e22 290a 0a20 2020  p failed.")..   
+00010ed0: 2064 6566 2063 6865 636b 5f64 7570 6528   def check_dupe(
+00010ee0: 7365 6c66 2c20 6361 6c6c 3a20 7374 7229  self, call: str)
+00010ef0: 202d 3e20 626f 6f6c 3a0a 2020 2020 2020   -> bool:.      
+00010f00: 2020 2222 2243 6865 636b 7320 6966 2061    """Checks if a
+00010f10: 2063 616c 6c73 6967 6e20 6973 2061 2064   callsign is a d
+00010f20: 7570 6520 6f6e 2063 7572 7265 6e74 2062  upe on current b
+00010f30: 616e 642f 6d6f 6465 2e22 2222 0a20 2020  and/mode.""".   
+00010f40: 2020 2020 2073 656c 662e 636f 6e74 6573       self.contes
+00010f50: 742e 7072 6564 7570 6528 7365 6c66 290a  t.predupe(self).
+00010f60: 2020 2020 2020 2020 6261 6e64 203d 2066          band = f
+00010f70: 6c6f 6174 2867 6574 5f6c 6f67 6765 645f  loat(get_logged_
+00010f80: 6261 6e64 2873 7472 2873 656c 662e 7261  band(str(self.ra
+00010f90: 6469 6f5f 7374 6174 652e 6765 7428 2276  dio_state.get("v
+00010fa0: 666f 6122 2c20 302e 3029 2929 290a 2020  foa", 0.0)))).  
+00010fb0: 2020 2020 2020 6d6f 6465 203d 2073 656c        mode = sel
+00010fc0: 662e 7261 6469 6f5f 7374 6174 652e 6765  f.radio_state.ge
+00010fd0: 7428 226d 6f64 6522 2c20 2222 290a 2020  t("mode", "").  
+00010fe0: 2020 2020 2020 6465 6275 676c 696e 6520        debugline 
+00010ff0: 3d20 280a 2020 2020 2020 2020 2020 2020  = (.            
+00011000: 6622 4361 6c6c 3a20 7b63 616c 6c7d 2042  f"Call: {call} B
+00011010: 616e 643a 207b 6261 6e64 7d20 4d6f 6465  and: {band} Mode
+00011020: 3a20 7b6d 6f64 657d 2044 7570 6574 7970  : {mode} Dupetyp
+00011030: 653a 207b 7365 6c66 2e63 6f6e 7465 7374  e: {self.contest
+00011040: 2e64 7570 655f 7479 7065 7d22 0a20 2020  .dupe_type}".   
+00011050: 2020 2020 2029 0a20 2020 2020 2020 206c       ).        l
+00011060: 6f67 6765 722e 6465 6275 6728 2225 7322  ogger.debug("%s"
+00011070: 2c20 6465 6275 676c 696e 6529 0a20 2020  , debugline).   
+00011080: 2020 2020 2069 6620 7365 6c66 2e63 6f6e       if self.con
+00011090: 7465 7374 2e64 7570 655f 7479 7065 203d  test.dupe_type =
+000110a0: 3d20 313a 0a20 2020 2020 2020 2020 2020  = 1:.           
+000110b0: 2072 6573 756c 7420 3d20 7365 6c66 2e64   result = self.d
+000110c0: 6174 6162 6173 652e 6368 6563 6b5f 6475  atabase.check_du
+000110d0: 7065 2863 616c 6c29 0a20 2020 2020 2020  pe(call).       
+000110e0: 2069 6620 7365 6c66 2e63 6f6e 7465 7374   if self.contest
+000110f0: 2e64 7570 655f 7479 7065 203d 3d20 323a  .dupe_type == 2:
+00011100: 0a20 2020 2020 2020 2020 2020 2072 6573  .            res
+00011110: 756c 7420 3d20 7365 6c66 2e64 6174 6162  ult = self.datab
+00011120: 6173 652e 6368 6563 6b5f 6475 7065 5f6f  ase.check_dupe_o
+00011130: 6e5f 6261 6e64 2863 616c 6c2c 2062 616e  n_band(call, ban
+00011140: 6429 0a20 2020 2020 2020 2069 6620 7365  d).        if se
+00011150: 6c66 2e63 6f6e 7465 7374 2e64 7570 655f  lf.contest.dupe_
+00011160: 7479 7065 203d 3d20 333a 0a20 2020 2020  type == 3:.     
+00011170: 2020 2020 2020 2072 6573 756c 7420 3d20         result = 
+00011180: 7365 6c66 2e64 6174 6162 6173 652e 6368  self.database.ch
+00011190: 6563 6b5f 6475 7065 5f6f 6e5f 6261 6e64  eck_dupe_on_band
+000111a0: 5f6d 6f64 6528 6361 6c6c 2c20 6261 6e64  _mode(call, band
+000111b0: 2c20 6d6f 6465 290a 2020 2020 2020 2020  , mode).        
+000111c0: 6966 2073 656c 662e 636f 6e74 6573 742e  if self.contest.
+000111d0: 6475 7065 5f74 7970 6520 3d3d 2034 3a0a  dupe_type == 4:.
+000111e0: 2020 2020 2020 2020 2020 2020 7265 7375              resu
+000111f0: 6c74 203d 207b 2269 7364 7570 6522 3a20  lt = {"isdupe": 
+00011200: 4661 6c73 657d 0a20 2020 2020 2020 2064  False}.        d
+00011210: 6562 7567 6c69 6e65 203d 2066 227b 7265  ebugline = f"{re
+00011220: 7375 6c74 7d22 0a20 2020 2020 2020 206c  sult}".        l
+00011230: 6f67 6765 722e 6465 6275 6728 2225 7322  ogger.debug("%s"
+00011240: 2c20 6465 6275 676c 696e 6529 0a20 2020  , debugline).   
+00011250: 2020 2020 2072 6574 7572 6e20 7265 7375       return resu
+00011260: 6c74 2e67 6574 2822 6973 6475 7065 222c  lt.get("isdupe",
+00011270: 2046 616c 7365 290a 0a20 2020 2064 6566   False)..    def
+00011280: 2073 6574 6d6f 6465 2873 656c 662c 206d   setmode(self, m
+00011290: 6f64 653a 2073 7472 2920 2d3e 204e 6f6e  ode: str) -> Non
+000112a0: 653a 0a20 2020 2020 2020 2022 2222 7374  e:.        """st
+000112b0: 7562 2066 6f72 2077 6865 6e20 7468 6520  ub for when the 
+000112c0: 6d6f 6465 2063 6861 6e67 6573 2e22 2222  mode changes."""
+000112d0: 0a20 2020 2020 2020 2069 6620 6d6f 6465  .        if mode
+000112e0: 203d 3d20 2243 5722 3a0a 2020 2020 2020   == "CW":.      
+000112f0: 2020 2020 2020 7365 6c66 2e63 7572 7265        self.curre
+00011300: 6e74 5f6d 6f64 6520 3d20 2243 5722 0a20  nt_mode = "CW". 
+00011310: 2020 2020 2020 2020 2020 2023 2073 656c             # sel
+00011320: 662e 6d6f 6465 2e73 6574 5465 7874 2822  f.mode.setText("
+00011330: 4357 2229 0a20 2020 2020 2020 2020 2020  CW").           
+00011340: 2073 656c 662e 7365 6e74 2e73 6574 5465   self.sent.setTe
+00011350: 7874 2822 3539 3922 290a 2020 2020 2020  xt("599").      
+00011360: 2020 2020 2020 7365 6c66 2e72 6563 6569        self.recei
+00011370: 7665 2e73 6574 5465 7874 2822 3539 3922  ve.setText("599"
+00011380: 290a 2020 2020 2020 2020 2020 2020 7365  ).            se
+00011390: 6c66 2e72 6561 645f 6377 5f6d 6163 726f  lf.read_cw_macro
+000113a0: 7328 290a 2020 2020 2020 2020 2020 2020  s().            
+000113b0: 7265 7475 726e 0a20 2020 2020 2020 2069  return.        i
+000113c0: 6620 6d6f 6465 203d 3d20 2253 5342 223a  f mode == "SSB":
+000113d0: 0a20 2020 2020 2020 2020 2020 2073 656c  .            sel
+000113e0: 662e 6375 7272 656e 745f 6d6f 6465 203d  f.current_mode =
+000113f0: 2022 5353 4222 0a20 2020 2020 2020 2020   "SSB".         
+00011400: 2020 2023 2073 656c 662e 6d6f 6465 2e73     # self.mode.s
+00011410: 6574 5465 7874 2822 5353 4222 290a 2020  etText("SSB").  
+00011420: 2020 2020 2020 2020 2020 7365 6c66 2e73            self.s
+00011430: 656e 742e 7365 7454 6578 7428 2235 3922  ent.setText("59"
+00011440: 290a 2020 2020 2020 2020 2020 2020 7365  ).            se
+00011450: 6c66 2e72 6563 6569 7665 2e73 6574 5465  lf.receive.setTe
+00011460: 7874 2822 3539 2229 0a20 2020 2020 2020  xt("59").       
+00011470: 2020 2020 2073 656c 662e 7265 6164 5f63       self.read_c
+00011480: 775f 6d61 6372 6f73 2829 0a20 2020 2020  w_macros().     
+00011490: 2020 2069 6620 6d6f 6465 203d 3d20 2252     if mode == "R
+000114a0: 5454 5922 3a0a 2020 2020 2020 2020 2020  TTY":.          
+000114b0: 2020 7365 6c66 2e63 7572 7265 6e74 5f6d    self.current_m
+000114c0: 6f64 6520 3d20 2252 5454 5922 0a20 2020  ode = "RTTY".   
+000114d0: 2020 2020 2020 2020 2023 2073 656c 662e           # self.
+000114e0: 6d6f 6465 2e73 6574 5465 7874 2822 5254  mode.setText("RT
+000114f0: 5459 2229 0a20 2020 2020 2020 2020 2020  TY").           
+00011500: 2073 656c 662e 7365 6e74 2e73 6574 5465   self.sent.setTe
+00011510: 7874 2822 3539 2229 0a20 2020 2020 2020  xt("59").       
+00011520: 2020 2020 2073 656c 662e 7265 6365 6976       self.receiv
+00011530: 652e 7365 7454 6578 7428 2235 3922 290a  e.setText("59").
+00011540: 0a20 2020 2064 6566 2067 6574 5f6f 706f  .    def get_opo
+00011550: 6e28 7365 6c66 293a 0a20 2020 2020 2020  n(self):.       
+00011560: 2022 2222 4374 726c 2b4f 206f 7220 4f50   """Ctrl+O or OP
+00011570: 4f4e 2064 6961 6c6f 6722 2222 0a20 2020  ON dialog""".   
+00011580: 2020 2020 2073 656c 662e 6f70 6f6e 5f64       self.opon_d
+00011590: 6961 6c6f 6720 3d20 4f70 4f6e 2857 4f52  ialog = OpOn(WOR
+000115a0: 4b49 4e47 5f50 4154 4829 0a20 2020 2020  KING_PATH).     
+000115b0: 2020 2073 656c 662e 6f70 6f6e 5f64 6961     self.opon_dia
+000115c0: 6c6f 672e 6163 6365 7074 6564 2e63 6f6e  log.accepted.con
+000115d0: 6e65 6374 2873 656c 662e 6e65 775f 6f70  nect(self.new_op
+000115e0: 290a 2020 2020 2020 2020 7365 6c66 2e6f  ).        self.o
+000115f0: 706f 6e5f 6469 616c 6f67 2e6f 7065 6e28  pon_dialog.open(
+00011600: 290a 0a20 2020 2064 6566 206e 6577 5f6f  )..    def new_o
+00011610: 7028 7365 6c66 293a 0a20 2020 2020 2020  p(self):.       
+00011620: 2022 2222 5361 7665 206e 6577 204f 5022   """Save new OP"
+00011630: 2222 0a20 2020 2020 2020 2069 6620 7365  "".        if se
+00011640: 6c66 2e6f 706f 6e5f 6469 616c 6f67 2e4e  lf.opon_dialog.N
+00011650: 6577 4f70 6572 6174 6f72 2e74 6578 7428  ewOperator.text(
+00011660: 293a 0a20 2020 2020 2020 2020 2020 2073  ):.            s
+00011670: 656c 662e 6375 7272 656e 745f 6f70 203d  elf.current_op =
+00011680: 2073 656c 662e 6f70 6f6e 5f64 6961 6c6f   self.opon_dialo
+00011690: 672e 4e65 774f 7065 7261 746f 722e 7465  g.NewOperator.te
+000116a0: 7874 2829 2e75 7070 6572 2829 0a20 2020  xt().upper().   
+000116b0: 2020 2020 2073 656c 662e 6f70 6f6e 5f64       self.opon_d
+000116c0: 6961 6c6f 672e 636c 6f73 6528 290a 2020  ialog.close().  
+000116d0: 2020 2020 2020 6c6f 6767 6572 2e64 6562        logger.deb
+000116e0: 7567 2822 4e65 7720 4f70 3a20 2573 222c  ug("New Op: %s",
+000116f0: 2073 656c 662e 6375 7272 656e 745f 6f70   self.current_op
+00011700: 290a 2020 2020 2020 2020 7365 6c66 2e6d  ).        self.m
+00011710: 616b 655f 6f70 5f64 6972 2829 0a0a 2020  ake_op_dir()..  
+00011720: 2020 6465 6620 6d61 6b65 5f6f 705f 6469    def make_op_di
+00011730: 7228 7365 6c66 293a 0a20 2020 2020 2020  r(self):.       
+00011740: 2022 2222 4372 6561 7465 204f 5020 6469   """Create OP di
+00011750: 7265 6374 6f72 7920 6966 2069 7420 646f  rectory if it do
+00011760: 6573 206e 6f74 2065 7869 7374 2e22 2222  es not exist."""
+00011770: 0a20 2020 2020 2020 2069 6620 7365 6c66  .        if self
+00011780: 2e63 7572 7265 6e74 5f6f 703a 0a20 2020  .current_op:.   
+00011790: 2020 2020 2020 2020 206f 705f 7061 7468           op_path
+000117a0: 203d 2050 6174 6828 4441 5441 5f50 4154   = Path(DATA_PAT
+000117b0: 4829 202f 2073 656c 662e 6375 7272 656e  H) / self.curren
+000117c0: 745f 6f70 0a20 2020 2020 2020 2020 2020  t_op.           
+000117d0: 206c 6f67 6765 722e 6465 6275 6728 226f   logger.debug("o
+000117e0: 705f 7061 7468 3a20 2573 222c 2073 7472  p_path: %s", str
+000117f0: 286f 705f 7061 7468 2929 0a20 2020 2020  (op_path)).     
+00011800: 2020 2020 2020 2069 6620 6f70 5f70 6174         if op_pat
+00011810: 682e 6973 5f64 6972 2829 2069 7320 4661  h.is_dir() is Fa
+00011820: 6c73 653a 0a20 2020 2020 2020 2020 2020  lse:.           
+00011830: 2020 2020 206c 6f67 6765 722e 6465 6275       logger.debu
+00011840: 6728 2243 7265 6174 696e 6720 4f70 2044  g("Creating Op D
+00011850: 6972 6563 746f 7279 3a20 2573 222c 2073  irectory: %s", s
+00011860: 7472 286f 705f 7061 7468 2929 0a20 2020  tr(op_path)).   
+00011870: 2020 2020 2020 2020 2020 2020 206f 732e               os.
+00011880: 6d6b 6469 7228 7374 7228 6f70 5f70 6174  mkdir(str(op_pat
+00011890: 6829 290a 2020 2020 2020 2020 2020 2020  h)).            
+000118a0: 6966 206f 705f 7061 7468 2e69 735f 6469  if op_path.is_di
+000118b0: 7228 293a 0a20 2020 2020 2020 2020 2020  r():.           
+000118c0: 2020 2020 2073 6f75 7263 655f 7061 7468       source_path
+000118d0: 203d 2050 6174 6828 574f 524b 494e 475f   = Path(WORKING_
+000118e0: 5041 5448 2920 2f20 2264 6174 6122 202f  PATH) / "data" /
+000118f0: 2022 7068 6f6e 6574 6963 7322 0a20 2020   "phonetics".   
+00011900: 2020 2020 2020 2020 2020 2020 206c 6f67               log
+00011910: 6765 722e 6465 6275 6728 2273 6f75 7263  ger.debug("sourc
+00011920: 655f 7061 7468 3a20 2573 222c 2073 7472  e_path: %s", str
+00011930: 2873 6f75 7263 655f 7061 7468 2929 0a20  (source_path)). 
+00011940: 2020 2020 2020 2020 2020 2020 2020 2066                 f
+00011950: 6f72 2063 6869 6c64 2069 6e20 736f 7572  or child in sour
+00011960: 6365 5f70 6174 682e 6974 6572 6469 7228  ce_path.iterdir(
+00011970: 293a 0a20 2020 2020 2020 2020 2020 2020  ):.             
+00011980: 2020 2020 2020 2064 6573 7469 6e61 7469         destinati
+00011990: 6f6e 5f66 696c 6520 3d20 6f70 5f70 6174  on_file = op_pat
+000119a0: 6820 2f20 6368 696c 642e 6e61 6d65 0a20  h / child.name. 
+000119b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000119c0: 2020 2069 6620 6465 7374 696e 6174 696f     if destinatio
+000119d0: 6e5f 6669 6c65 2e69 735f 6669 6c65 2829  n_file.is_file()
+000119e0: 2069 7320 4661 6c73 653a 0a20 2020 2020   is False:.     
+000119f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00011a00: 2020 206c 6f67 6765 722e 6465 6275 6728     logger.debug(
+00011a10: 2244 6573 7469 6e61 7469 6f6e 3a20 2573  "Destination: %s
+00011a20: 222c 2073 7472 2864 6573 7469 6e61 7469  ", str(destinati
+00011a30: 6f6e 5f66 696c 6529 290a 2020 2020 2020  on_file)).      
+00011a40: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00011a50: 2020 6465 7374 696e 6174 696f 6e5f 6669    destination_fi
+00011a60: 6c65 2e77 7269 7465 5f62 7974 6573 2863  le.write_bytes(c
+00011a70: 6869 6c64 2e72 6561 645f 6279 7465 7328  hild.read_bytes(
+00011a80: 2929 0a0a 2020 2020 6465 6620 706f 6c6c  ))..    def poll
+00011a90: 5f72 6164 696f 2873 656c 6629 3a0a 2020  _radio(self):.  
+00011aa0: 2020 2020 2020 2222 2273 7475 6222 2222        """stub"""
+00011ab0: 0a20 2020 2020 2020 2069 6620 7365 6c66  .        if self
+00011ac0: 2e72 6967 5f63 6f6e 7472 6f6c 3a0a 2020  .rig_control:.  
+00011ad0: 2020 2020 2020 2020 2020 6966 2073 656c            if sel
+00011ae0: 662e 7269 675f 636f 6e74 726f 6c2e 6f6e  f.rig_control.on
+00011af0: 6c69 6e65 3a0a 2020 2020 2020 2020 2020  line:.          
+00011b00: 2020 2020 2020 7666 6f20 3d20 7365 6c66        vfo = self
+00011b10: 2e72 6967 5f63 6f6e 7472 6f6c 2e67 6574  .rig_control.get
+00011b20: 5f76 666f 2829 0a20 2020 2020 2020 2020  _vfo().         
+00011b30: 2020 2020 2020 206d 6f64 6520 3d20 7365         mode = se
+00011b40: 6c66 2e72 6967 5f63 6f6e 7472 6f6c 2e67  lf.rig_control.g
+00011b50: 6574 5f6d 6f64 6528 290a 2020 2020 2020  et_mode().      
+00011b60: 2020 2020 2020 2020 2020 6277 203d 2073            bw = s
+00011b70: 656c 662e 7269 675f 636f 6e74 726f 6c2e  elf.rig_control.
+00011b80: 6765 745f 6277 2829 0a20 2020 2020 2020  get_bw().       
+00011b90: 2020 2020 2020 2020 2023 2073 656c 662e           # self.
+00011ba0: 7261 6469 6f5f 7374 6174 655b 2270 7474  radio_state["ptt
+00011bb0: 225d 203d 2073 656c 662e 7269 675f 636f  "] = self.rig_co
+00011bc0: 6e74 726f 6c2e 6765 745f 7074 7428 290a  ntrol.get_ptt().
+00011bd0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00011be0: 2320 6966 2073 656c 662e 7261 6469 6f5f  # if self.radio_
+00011bf0: 7374 6174 652e 6765 7428 2270 7474 222c  state.get("ptt",
+00011c00: 2030 2920 3d3d 2031 3a0a 2020 2020 2020   0) == 1:.      
+00011c10: 2020 2020 2020 2020 2020 2320 2020 2020            #     
+00011c20: 7365 6c66 2e6c 6566 7464 6f74 2e73 6574  self.leftdot.set
+00011c30: 5069 786d 6170 2873 656c 662e 6772 6565  Pixmap(self.gree
+00011c40: 6e64 6f74 290a 2020 2020 2020 2020 2020  ndot).          
+00011c50: 2020 2020 2020 2320 656c 7365 3a0a 2020        # else:.  
+00011c60: 2020 2020 2020 2020 2020 2020 2020 2320                # 
+00011c70: 2020 2020 7365 6c66 2e6c 6566 7464 6f74      self.leftdot
+00011c80: 2e73 6574 5069 786d 6170 2873 656c 662e  .setPixmap(self.
+00011c90: 7265 6464 6f74 290a 2020 2020 2020 2020  reddot).        
+00011ca0: 2020 2020 2020 2020 6966 206d 6f64 6520          if mode 
+00011cb0: 3d3d 2022 4357 223a 0a20 2020 2020 2020  == "CW":.       
+00011cc0: 2020 2020 2020 2020 2020 2020 2073 656c               sel
+00011cd0: 662e 7365 746d 6f64 6528 6d6f 6465 290a  f.setmode(mode).
+00011ce0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00011cf0: 6966 206d 6f64 6520 3d3d 2022 4c53 4222  if mode == "LSB"
+00011d00: 206f 7220 6d6f 6465 203d 3d20 2255 5342   or mode == "USB
+00011d10: 223a 0a20 2020 2020 2020 2020 2020 2020  ":.             
+00011d20: 2020 2020 2020 2073 656c 662e 7365 746d         self.setm
+00011d30: 6f64 6528 2253 5342 2229 0a20 2020 2020  ode("SSB").     
+00011d40: 2020 2020 2020 2020 2020 2069 6620 6d6f             if mo
+00011d50: 6465 203d 3d20 2252 5454 5922 3a0a 2020  de == "RTTY":.  
+00011d60: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00011d70: 2020 7365 6c66 2e73 6574 6d6f 6465 2822    self.setmode("
+00011d80: 5254 5459 2229 0a20 2020 2020 2020 2020  RTTY").         
+00011d90: 2020 2020 2020 2073 656c 662e 7261 6469         self.radi
+00011da0: 6f5f 7374 6174 655b 2276 666f 6122 5d20  o_state["vfoa"] 
+00011db0: 3d20 7666 6f0a 2020 2020 2020 2020 2020  = vfo.          
+00011dc0: 2020 2020 2020 6261 6e64 203d 2067 6574        band = get
+00011dd0: 6261 6e64 2873 7472 2876 666f 2929 0a20  band(str(vfo)). 
+00011de0: 2020 2020 2020 2020 2020 2020 2020 2073                 s
+00011df0: 656c 662e 7261 6469 6f5f 7374 6174 655b  elf.radio_state[
+00011e00: 2262 616e 6422 5d20 3d20 6261 6e64 0a20  "band"] = band. 
+00011e10: 2020 2020 2020 2020 2020 2020 2020 2073                 s
+00011e20: 656c 662e 636f 6e74 6163 745b 2242 616e  elf.contact["Ban
+00011e30: 6422 5d20 3d20 6765 745f 6c6f 6767 6564  d"] = get_logged
+00011e40: 5f62 616e 6428 7374 7228 7666 6f29 290a  _band(str(vfo)).
+00011e50: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00011e60: 7365 6c66 2e73 6574 5f62 616e 645f 696e  self.set_band_in
+00011e70: 6469 6361 746f 7228 6261 6e64 290a 2020  dicator(band).  
+00011e80: 2020 2020 2020 2020 2020 2020 2020 7365                se
+00011e90: 6c66 2e72 6164 696f 5f73 7461 7465 5b22  lf.radio_state["
+00011ea0: 6d6f 6465 225d 203d 206d 6f64 650a 2020  mode"] = mode.  
+00011eb0: 2020 2020 2020 2020 2020 2020 2020 7365                se
+00011ec0: 6c66 2e72 6164 696f 5f73 7461 7465 5b22  lf.radio_state["
+00011ed0: 6277 225d 203d 2062 770a 2020 2020 2020  bw"] = bw.      
+00011ee0: 2020 2020 2020 2020 2020 6c6f 6767 6572            logger
+00011ef0: 2e64 6562 7567 2822 5646 4f3a 2025 7320  .debug("VFO: %s 
+00011f00: 204d 4f44 453a 2025 7320 4257 3a20 2573   MODE: %s BW: %s
+00011f10: 222c 2076 666f 2c20 6d6f 6465 2c20 6277  ", vfo, mode, bw
+00011f20: 290a 2020 2020 2020 2020 2020 2020 2020  ).              
+00011f30: 2020 7365 6c66 2e73 6574 5f77 696e 646f    self.set_windo
+00011f40: 775f 7469 746c 6528 290a 2020 2020 2020  w_title().      
+00011f50: 2020 2020 2020 2020 2020 636d 6420 3d20            cmd = 
+00011f60: 7b7d 0a20 2020 2020 2020 2020 2020 2020  {}.             
+00011f70: 2020 2063 6d64 5b22 636d 6422 5d20 3d20     cmd["cmd"] = 
+00011f80: 2252 4144 494f 5f53 5441 5445 220a 2020  "RADIO_STATE".  
+00011f90: 2020 2020 2020 2020 2020 2020 2020 636d                cm
+00011fa0: 645b 2273 7461 7469 6f6e 225d 203d 2070  d["station"] = p
+00011fb0: 6c61 7466 6f72 6d2e 6e6f 6465 2829 0a20  latform.node(). 
+00011fc0: 2020 2020 2020 2020 2020 2020 2020 2063                 c
+00011fd0: 6d64 5b22 6261 6e64 225d 203d 2062 616e  md["band"] = ban
+00011fe0: 640a 2020 2020 2020 2020 2020 2020 2020  d.              
+00011ff0: 2020 636d 645b 2276 666f 6122 5d20 3d20    cmd["vfoa"] = 
+00012000: 7666 6f0a 2020 2020 2020 2020 2020 2020  vfo.            
+00012010: 2020 2020 636d 645b 226d 6f64 6522 5d20      cmd["mode"] 
+00012020: 3d20 6d6f 6465 0a20 2020 2020 2020 2020  = mode.         
+00012030: 2020 2020 2020 2063 6d64 5b22 6277 225d         cmd["bw"]
+00012040: 203d 2062 770a 2020 2020 2020 2020 2020   = bw.          
+00012050: 2020 2020 2020 7365 6c66 2e6d 756c 7469        self.multi
+00012060: 6361 7374 5f69 6e74 6572 6661 6365 2e73  cast_interface.s
+00012070: 656e 645f 6173 5f6a 736f 6e28 636d 6429  end_as_json(cmd)
+00012080: 0a0a 2020 2020 6465 6620 6564 6974 5f63  ..    def edit_c
+00012090: 775f 6d61 6372 6f73 2873 656c 6629 202d  w_macros(self) -
+000120a0: 3e20 4e6f 6e65 3a0a 2020 2020 2020 2020  > None:.        
+000120b0: 2222 220a 2020 2020 2020 2020 4361 6c6c  """.        Call
+000120c0: 7320 7468 6520 6465 6661 756c 7420 7465  s the default te
+000120d0: 7874 2065 6469 746f 7220 746f 2065 6469  xt editor to edi
+000120e0: 7420 7468 6520 4357 206d 6163 726f 2066  t the CW macro f
+000120f0: 696c 652e 0a20 2020 2020 2020 2022 2222  ile..        """
+00012100: 0a20 2020 2020 2020 2069 6620 7365 6c66  .        if self
+00012110: 2e72 6164 696f 5f73 7461 7465 2e67 6574  .radio_state.get
+00012120: 2822 6d6f 6465 2229 203d 3d20 2243 5722  ("mode") == "CW"
+00012130: 3a0a 2020 2020 2020 2020 2020 2020 6d61  :.            ma
+00012140: 6372 6f5f 6669 6c65 203d 2022 2f63 776d  cro_file = "/cwm
+00012150: 6163 726f 732e 7478 7422 0a20 2020 2020  acros.txt".     
+00012160: 2020 2065 6c73 653a 0a20 2020 2020 2020     else:.       
+00012170: 2020 2020 206d 6163 726f 5f66 696c 6520       macro_file 
+00012180: 3d20 222f 7373 626d 6163 726f 732e 7478  = "/ssbmacros.tx
+00012190: 7422 0a20 2020 2020 2020 2069 6620 6e6f  t".        if no
+000121a0: 7420 5061 7468 2844 4154 415f 5041 5448  t Path(DATA_PATH
+000121b0: 202b 206d 6163 726f 5f66 696c 6529 2e65   + macro_file).e
+000121c0: 7869 7374 7328 293a 0a20 2020 2020 2020  xists():.       
+000121d0: 2020 2020 206c 6f67 6765 722e 6465 6275       logger.debu
+000121e0: 6728 2272 6561 645f 6377 5f6d 6163 726f  g("read_cw_macro
+000121f0: 733a 2063 6f70 7969 6e67 2064 6566 6175  s: copying defau
+00012200: 6c74 206d 6163 726f 2066 696c 652e 2229  lt macro file.")
+00012210: 0a20 2020 2020 2020 2020 2020 2063 6f70  .            cop
+00012220: 7966 696c 6528 574f 524b 494e 475f 5041  yfile(WORKING_PA
+00012230: 5448 202b 2022 2f64 6174 6122 202b 206d  TH + "/data" + m
+00012240: 6163 726f 5f66 696c 652c 2044 4154 415f  acro_file, DATA_
+00012250: 5041 5448 202b 206d 6163 726f 5f66 696c  PATH + macro_fil
+00012260: 6529 0a20 2020 2020 2020 206f 732e 7379  e).        os.sy
+00012270: 7374 656d 2866 2278 6467 2d6f 7065 6e20  stem(f"xdg-open 
+00012280: 7b44 4154 415f 5041 5448 7d7b 6d61 6372  {DATA_PATH}{macr
+00012290: 6f5f 6669 6c65 7d22 290a 0a20 2020 2064  o_file}")..    d
+000122a0: 6566 2072 6561 645f 6377 5f6d 6163 726f  ef read_cw_macro
+000122b0: 7328 7365 6c66 2920 2d3e 204e 6f6e 653a  s(self) -> None:
+000122c0: 0a20 2020 2020 2020 2022 2222 0a20 2020  .        """.   
+000122d0: 2020 2020 2052 6561 6473 2069 6e20 7468       Reads in th
+000122e0: 6520 4357 206d 6163 726f 732c 2066 6972  e CW macros, fir
+000122f0: 7374 7320 6974 2063 6865 636b 7320 746f  sts it checks to
+00012300: 2073 6565 2069 6620 7468 6520 6669 6c65   see if the file
+00012310: 2065 7869 7374 732e 2049 6620 6974 2064   exists. If it d
+00012320: 6f65 7320 6e6f 742c 0a20 2020 2020 2020  oes not,.       
+00012330: 2061 6e64 2074 6869 7320 6861 7320 6265   and this has be
+00012340: 656e 2070 6163 6b61 6765 6420 7769 7468  en packaged with
+00012350: 2070 7969 6e73 7461 6c6c 6572 2069 7420   pyinstaller it 
+00012360: 7769 6c6c 2063 6f70 7920 7468 6520 6465  will copy the de
+00012370: 6661 756c 7420 6669 6c65 2066 726f 6d20  fault file from 
+00012380: 7468 650a 2020 2020 2020 2020 7465 6d70  the.        temp
+00012390: 2064 6972 6563 746f 7279 2074 6869 7320   directory this 
+000123a0: 6973 2072 756e 6e69 6e67 2066 726f 6d2e  is running from.
+000123b0: 2e2e 2049 6e20 7468 656f 7279 2e0a 2020  .. In theory..  
+000123c0: 2020 2020 2020 2222 220a 0a20 2020 2020        """..     
+000123d0: 2020 2069 6620 7365 6c66 2e72 6164 696f     if self.radio
+000123e0: 5f73 7461 7465 2e67 6574 2822 6d6f 6465  _state.get("mode
+000123f0: 2229 203d 3d20 2243 5722 3a0a 2020 2020  ") == "CW":.    
+00012400: 2020 2020 2020 2020 6d61 6372 6f5f 6669          macro_fi
+00012410: 6c65 203d 2022 2f63 776d 6163 726f 732e  le = "/cwmacros.
+00012420: 7478 7422 0a20 2020 2020 2020 2065 6c73  txt".        els
+00012430: 653a 0a20 2020 2020 2020 2020 2020 206d  e:.            m
+00012440: 6163 726f 5f66 696c 6520 3d20 222f 7373  acro_file = "/ss
+00012450: 626d 6163 726f 732e 7478 7422 0a0a 2020  bmacros.txt"..  
+00012460: 2020 2020 2020 6966 206e 6f74 2050 6174        if not Pat
+00012470: 6828 4441 5441 5f50 4154 4820 2b20 6d61  h(DATA_PATH + ma
+00012480: 6372 6f5f 6669 6c65 292e 6578 6973 7473  cro_file).exists
+00012490: 2829 3a0a 2020 2020 2020 2020 2020 2020  ():.            
+000124a0: 6c6f 6767 6572 2e64 6562 7567 2822 7265  logger.debug("re
+000124b0: 6164 5f63 775f 6d61 6372 6f73 3a20 636f  ad_cw_macros: co
+000124c0: 7079 696e 6720 6465 6661 756c 7420 6d61  pying default ma
+000124d0: 6372 6f20 6669 6c65 2e22 290a 2020 2020  cro file.").    
+000124e0: 2020 2020 2020 2020 636f 7079 6669 6c65          copyfile
+000124f0: 2857 4f52 4b49 4e47 5f50 4154 4820 2b20  (WORKING_PATH + 
+00012500: 222f 6461 7461 2220 2b20 6d61 6372 6f5f  "/data" + macro_
+00012510: 6669 6c65 2c20 4441 5441 5f50 4154 4820  file, DATA_PATH 
+00012520: 2b20 6d61 6372 6f5f 6669 6c65 290a 2020  + macro_file).  
+00012530: 2020 2020 2020 7769 7468 206f 7065 6e28        with open(
+00012540: 4441 5441 5f50 4154 4820 2b20 6d61 6372  DATA_PATH + macr
+00012550: 6f5f 6669 6c65 2c20 2272 222c 2065 6e63  o_file, "r", enc
+00012560: 6f64 696e 673d 2275 7466 2d38 2229 2061  oding="utf-8") a
+00012570: 7320 6669 6c65 5f64 6573 6372 6970 746f  s file_descripto
+00012580: 723a 0a20 2020 2020 2020 2020 2020 2066  r:.            f
+00012590: 6f72 206c 696e 6520 696e 2066 696c 655f  or line in file_
+000125a0: 6465 7363 7269 7074 6f72 3a0a 2020 2020  descriptor:.    
+000125b0: 2020 2020 2020 2020 2020 2020 7472 793a              try:
+000125c0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+000125d0: 2020 2020 206d 6f64 652c 2066 6b65 792c       mode, fkey,
+000125e0: 2062 7574 746f 6e6e 616d 652c 2063 7774   buttonname, cwt
+000125f0: 6578 7420 3d20 6c69 6e65 2e73 706c 6974  ext = line.split
+00012600: 2822 7c22 290a 2020 2020 2020 2020 2020  ("|").          
+00012610: 2020 2020 2020 2020 2020 6966 206d 6f64            if mod
+00012620: 652e 7374 7269 7028 292e 7570 7065 7228  e.strip().upper(
+00012630: 2920 3d3d 2022 5222 2061 6e64 2073 656c  ) == "R" and sel
+00012640: 662e 7072 6566 2e67 6574 2822 7275 6e5f  f.pref.get("run_
+00012650: 7374 6174 6522 293a 0a20 2020 2020 2020  state"):.       
+00012660: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00012670: 2073 656c 662e 666b 6579 735b 666b 6579   self.fkeys[fkey
+00012680: 2e73 7472 6970 2829 5d20 3d20 2862 7574  .strip()] = (but
+00012690: 746f 6e6e 616d 652e 7374 7269 7028 292c  tonname.strip(),
+000126a0: 2063 7774 6578 742e 7374 7269 7028 2929   cwtext.strip())
+000126b0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+000126c0: 2020 2020 2069 6620 6d6f 6465 2e73 7472       if mode.str
+000126d0: 6970 2829 2e75 7070 6572 2829 2021 3d20  ip().upper() != 
+000126e0: 2252 2220 616e 6420 6e6f 7420 7365 6c66  "R" and not self
+000126f0: 2e70 7265 662e 6765 7428 2272 756e 5f73  .pref.get("run_s
+00012700: 7461 7465 2229 3a0a 2020 2020 2020 2020  tate"):.        
+00012710: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00012720: 7365 6c66 2e66 6b65 7973 5b66 6b65 792e  self.fkeys[fkey.
+00012730: 7374 7269 7028 295d 203d 2028 6275 7474  strip()] = (butt
+00012740: 6f6e 6e61 6d65 2e73 7472 6970 2829 2c20  onname.strip(), 
+00012750: 6377 7465 7874 2e73 7472 6970 2829 290a  cwtext.strip()).
 00012760: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00012770: 2020 2020 6c6f 6767 6572 2e69 6e66 6f28      logger.info(
-00012780: 2272 6561 645f 6377 5f6d 6163 726f 733a  "read_cw_macros:
-00012790: 2025 7322 2c20 6572 7229 0a20 2020 2020   %s", err).     
-000127a0: 2020 206b 6579 7320 3d20 7365 6c66 2e66     keys = self.f
-000127b0: 6b65 7973 2e6b 6579 7328 290a 2020 2020  keys.keys().    
-000127c0: 2020 2020 6966 2022 4631 2220 696e 206b      if "F1" in k
-000127d0: 6579 733a 0a20 2020 2020 2020 2020 2020  eys:.           
-000127e0: 2073 656c 662e 4631 2e73 6574 5465 7874   self.F1.setText
-000127f0: 2866 2246 313a 207b 7365 6c66 2e66 6b65  (f"F1: {self.fke
-00012800: 7973 5b27 4631 275d 5b30 5d7d 2229 0a20  ys['F1'][0]}"). 
-00012810: 2020 2020 2020 2020 2020 2073 656c 662e             self.
-00012820: 4631 2e73 6574 546f 6f6c 5469 7028 7365  F1.setToolTip(se
-00012830: 6c66 2e66 6b65 7973 5b22 4631 225d 5b31  lf.fkeys["F1"][1
-00012840: 5d29 0a20 2020 2020 2020 2069 6620 2246  ]).        if "F
-00012850: 3222 2069 6e20 6b65 7973 3a0a 2020 2020  2" in keys:.    
-00012860: 2020 2020 2020 2020 7365 6c66 2e46 322e          self.F2.
-00012870: 7365 7454 6578 7428 6622 4632 3a20 7b73  setText(f"F2: {s
-00012880: 656c 662e 666b 6579 735b 2746 3227 5d5b  elf.fkeys['F2'][
-00012890: 305d 7d22 290a 2020 2020 2020 2020 2020  0]}").          
-000128a0: 2020 7365 6c66 2e46 322e 7365 7454 6f6f    self.F2.setToo
-000128b0: 6c54 6970 2873 656c 662e 666b 6579 735b  lTip(self.fkeys[
-000128c0: 2246 3222 5d5b 315d 290a 2020 2020 2020  "F2"][1]).      
-000128d0: 2020 6966 2022 4633 2220 696e 206b 6579    if "F3" in key
-000128e0: 733a 0a20 2020 2020 2020 2020 2020 2073  s:.            s
-000128f0: 656c 662e 4633 2e73 6574 5465 7874 2866  elf.F3.setText(f
-00012900: 2246 333a 207b 7365 6c66 2e66 6b65 7973  "F3: {self.fkeys
-00012910: 5b27 4633 275d 5b30 5d7d 2229 0a20 2020  ['F3'][0]}").   
-00012920: 2020 2020 2020 2020 2073 656c 662e 4633           self.F3
-00012930: 2e73 6574 546f 6f6c 5469 7028 7365 6c66  .setToolTip(self
-00012940: 2e66 6b65 7973 5b22 4633 225d 5b31 5d29  .fkeys["F3"][1])
-00012950: 0a20 2020 2020 2020 2069 6620 2246 3422  .        if "F4"
-00012960: 2069 6e20 6b65 7973 3a0a 2020 2020 2020   in keys:.      
-00012970: 2020 2020 2020 7365 6c66 2e46 342e 7365        self.F4.se
-00012980: 7454 6578 7428 6622 4634 3a20 7b73 656c  tText(f"F4: {sel
-00012990: 662e 666b 6579 735b 2746 3427 5d5b 305d  f.fkeys['F4'][0]
-000129a0: 7d22 290a 2020 2020 2020 2020 2020 2020  }").            
-000129b0: 7365 6c66 2e46 342e 7365 7454 6f6f 6c54  self.F4.setToolT
-000129c0: 6970 2873 656c 662e 666b 6579 735b 2246  ip(self.fkeys["F
-000129d0: 3422 5d5b 315d 290a 2020 2020 2020 2020  4"][1]).        
-000129e0: 6966 2022 4635 2220 696e 206b 6579 733a  if "F5" in keys:
-000129f0: 0a20 2020 2020 2020 2020 2020 2073 656c  .            sel
-00012a00: 662e 4635 2e73 6574 5465 7874 2866 2246  f.F5.setText(f"F
-00012a10: 353a 207b 7365 6c66 2e66 6b65 7973 5b27  5: {self.fkeys['
-00012a20: 4635 275d 5b30 5d7d 2229 0a20 2020 2020  F5'][0]}").     
-00012a30: 2020 2020 2020 2073 656c 662e 4635 2e73         self.F5.s
-00012a40: 6574 546f 6f6c 5469 7028 7365 6c66 2e66  etToolTip(self.f
-00012a50: 6b65 7973 5b22 4635 225d 5b31 5d29 0a20  keys["F5"][1]). 
-00012a60: 2020 2020 2020 2069 6620 2246 3622 2069         if "F6" i
-00012a70: 6e20 6b65 7973 3a0a 2020 2020 2020 2020  n keys:.        
-00012a80: 2020 2020 7365 6c66 2e46 362e 7365 7454      self.F6.setT
-00012a90: 6578 7428 6622 4636 3a20 7b73 656c 662e  ext(f"F6: {self.
-00012aa0: 666b 6579 735b 2746 3627 5d5b 305d 7d22  fkeys['F6'][0]}"
-00012ab0: 290a 2020 2020 2020 2020 2020 2020 7365  ).            se
-00012ac0: 6c66 2e46 362e 7365 7454 6f6f 6c54 6970  lf.F6.setToolTip
-00012ad0: 2873 656c 662e 666b 6579 735b 2246 3622  (self.fkeys["F6"
-00012ae0: 5d5b 315d 290a 2020 2020 2020 2020 6966  ][1]).        if
-00012af0: 2022 4637 2220 696e 206b 6579 733a 0a20   "F7" in keys:. 
-00012b00: 2020 2020 2020 2020 2020 2073 656c 662e             self.
-00012b10: 4637 2e73 6574 5465 7874 2866 2246 373a  F7.setText(f"F7:
-00012b20: 207b 7365 6c66 2e66 6b65 7973 5b27 4637   {self.fkeys['F7
-00012b30: 275d 5b30 5d7d 2229 0a20 2020 2020 2020  '][0]}").       
-00012b40: 2020 2020 2073 656c 662e 4637 2e73 6574       self.F7.set
-00012b50: 546f 6f6c 5469 7028 7365 6c66 2e66 6b65  ToolTip(self.fke
-00012b60: 7973 5b22 4637 225d 5b31 5d29 0a20 2020  ys["F7"][1]).   
-00012b70: 2020 2020 2069 6620 2246 3822 2069 6e20       if "F8" in 
-00012b80: 6b65 7973 3a0a 2020 2020 2020 2020 2020  keys:.          
-00012b90: 2020 7365 6c66 2e46 382e 7365 7454 6578    self.F8.setTex
-00012ba0: 7428 6622 4638 3a20 7b73 656c 662e 666b  t(f"F8: {self.fk
-00012bb0: 6579 735b 2746 3827 5d5b 305d 7d22 290a  eys['F8'][0]}").
-00012bc0: 2020 2020 2020 2020 2020 2020 7365 6c66              self
-00012bd0: 2e46 382e 7365 7454 6f6f 6c54 6970 2873  .F8.setToolTip(s
-00012be0: 656c 662e 666b 6579 735b 2246 3822 5d5b  elf.fkeys["F8"][
-00012bf0: 315d 290a 2020 2020 2020 2020 6966 2022  1]).        if "
-00012c00: 4639 2220 696e 206b 6579 733a 0a20 2020  F9" in keys:.   
-00012c10: 2020 2020 2020 2020 2073 656c 662e 4639           self.F9
-00012c20: 2e73 6574 5465 7874 2866 2246 393a 207b  .setText(f"F9: {
-00012c30: 7365 6c66 2e66 6b65 7973 5b27 4639 275d  self.fkeys['F9']
-00012c40: 5b30 5d7d 2229 0a20 2020 2020 2020 2020  [0]}").         
-00012c50: 2020 2073 656c 662e 4639 2e73 6574 546f     self.F9.setTo
-00012c60: 6f6c 5469 7028 7365 6c66 2e66 6b65 7973  olTip(self.fkeys
-00012c70: 5b22 4639 225d 5b31 5d29 0a20 2020 2020  ["F9"][1]).     
-00012c80: 2020 2069 6620 2246 3130 2220 696e 206b     if "F10" in k
-00012c90: 6579 733a 0a20 2020 2020 2020 2020 2020  eys:.           
-00012ca0: 2073 656c 662e 4631 302e 7365 7454 6578   self.F10.setTex
-00012cb0: 7428 6622 4631 303a 207b 7365 6c66 2e66  t(f"F10: {self.f
-00012cc0: 6b65 7973 5b27 4631 3027 5d5b 305d 7d22  keys['F10'][0]}"
-00012cd0: 290a 2020 2020 2020 2020 2020 2020 7365  ).            se
-00012ce0: 6c66 2e46 3130 2e73 6574 546f 6f6c 5469  lf.F10.setToolTi
-00012cf0: 7028 7365 6c66 2e66 6b65 7973 5b22 4631  p(self.fkeys["F1
-00012d00: 3022 5d5b 315d 290a 2020 2020 2020 2020  0"][1]).        
-00012d10: 6966 2022 4631 3122 2069 6e20 6b65 7973  if "F11" in keys
-00012d20: 3a0a 2020 2020 2020 2020 2020 2020 7365  :.            se
-00012d30: 6c66 2e46 3131 2e73 6574 5465 7874 2866  lf.F11.setText(f
-00012d40: 2246 3131 3a20 7b73 656c 662e 666b 6579  "F11: {self.fkey
-00012d50: 735b 2746 3131 275d 5b30 5d7d 2229 0a20  s['F11'][0]}"). 
-00012d60: 2020 2020 2020 2020 2020 2073 656c 662e             self.
-00012d70: 4631 312e 7365 7454 6f6f 6c54 6970 2873  F11.setToolTip(s
-00012d80: 656c 662e 666b 6579 735b 2246 3131 225d  elf.fkeys["F11"]
-00012d90: 5b31 5d29 0a20 2020 2020 2020 2069 6620  [1]).        if 
-00012da0: 2246 3132 2220 696e 206b 6579 733a 0a20  "F12" in keys:. 
-00012db0: 2020 2020 2020 2020 2020 2073 656c 662e             self.
-00012dc0: 4631 322e 7365 7454 6578 7428 6622 4631  F12.setText(f"F1
-00012dd0: 323a 207b 7365 6c66 2e66 6b65 7973 5b27  2: {self.fkeys['
-00012de0: 4631 3227 5d5b 305d 7d22 290a 2020 2020  F12'][0]}").    
-00012df0: 2020 2020 2020 2020 7365 6c66 2e46 3132          self.F12
-00012e00: 2e73 6574 546f 6f6c 5469 7028 7365 6c66  .setToolTip(self
-00012e10: 2e66 6b65 7973 5b22 4631 3222 5d5b 315d  .fkeys["F12"][1]
-00012e20: 290a 0a20 2020 2064 6566 2067 656e 6572  )..    def gener
-00012e30: 6174 655f 6164 6966 2873 656c 6629 3a0a  ate_adif(self):.
-00012e40: 2020 2020 2020 2020 2222 2247 656e 6572          """Gener
-00012e50: 6174 6520 4144 4946 2222 220a 2020 2020  ate ADIF""".    
-00012e60: 2020 2020 6c6f 6767 6572 2e64 6562 7567      logger.debug
-00012e70: 2822 2a2a 2a2a 2a2a 4144 4946 2a2a 2a2a  ("******ADIF****
-00012e80: 2a22 290a 2020 2020 2020 2020 7365 6c66  *").        self
-00012e90: 2e63 6f6e 7465 7374 2e61 6469 6628 7365  .contest.adif(se
-00012ea0: 6c66 290a 0a20 2020 2064 6566 2067 656e  lf)..    def gen
-00012eb0: 6572 6174 655f 6361 6272 696c 6c6f 2873  erate_cabrillo(s
-00012ec0: 656c 6629 3a0a 2020 2020 2020 2020 2222  elf):.        ""
-00012ed0: 2247 656e 6572 6174 6573 2043 6162 7269  "Generates Cabri
-00012ee0: 6c6c 6f20 6669 6c65 2e20 4d61 7962 652e  llo file. Maybe.
-00012ef0: 2222 220a 2020 2020 2020 2020 2320 6874  """.        # ht
-00012f00: 7470 733a 2f2f 7777 772e 6371 7770 782e  tps://www.cqwpx.
-00012f10: 636f 6d2f 6361 6272 696c 6c6f 2e68 746d  com/cabrillo.htm
-00012f20: 0a20 2020 2020 2020 206c 6f67 6765 722e  .        logger.
-00012f30: 6465 6275 6728 222a 2a2a 2a2a 2a43 6162  debug("******Cab
-00012f40: 7269 6c6c 6f2a 2a2a 2a2a 2229 0a20 2020  rillo*****").   
-00012f50: 2020 2020 2073 656c 662e 636f 6e74 6573       self.contes
-00012f60: 742e 6361 6272 696c 6c6f 2873 656c 6629  t.cabrillo(self)
-00012f70: 0a0a 0a64 6566 206c 6f61 645f 666f 6e74  ...def load_font
-00012f80: 735f 6672 6f6d 5f64 6972 2864 6972 6563  s_from_dir(direc
-00012f90: 746f 7279 3a20 7374 7229 202d 3e20 7365  tory: str) -> se
-00012fa0: 743a 0a20 2020 2022 2222 0a20 2020 2057  t:.    """.    W
-00012fb0: 656c 6c20 6974 206c 6f61 6473 2066 6f6e  ell it loads fon
-00012fc0: 7473 2066 726f 6d20 6120 6469 7265 6374  ts from a direct
-00012fd0: 6f72 792e 2e2e 0a20 2020 2022 2222 0a20  ory....    """. 
-00012fe0: 2020 2066 6f6e 745f 6661 6d69 6c69 6573     font_families
-00012ff0: 203d 2073 6574 2829 0a20 2020 2066 6f72   = set().    for
-00013000: 205f 6669 2069 6e20 5144 6972 2864 6972   _fi in QDir(dir
-00013010: 6563 746f 7279 292e 656e 7472 7949 6e66  ectory).entryInf
-00013020: 6f4c 6973 7428 5b22 2a2e 7474 6622 2c20  oList(["*.ttf", 
-00013030: 222a 2e77 6f66 6622 2c20 222a 2e77 6f66  "*.woff", "*.wof
-00013040: 6632 225d 293a 0a20 2020 2020 2020 205f  f2"]):.        _
-00013050: 6964 203d 2051 466f 6e74 4461 7461 6261  id = QFontDataba
-00013060: 7365 2e61 6464 4170 706c 6963 6174 696f  se.addApplicatio
-00013070: 6e46 6f6e 7428 5f66 692e 6162 736f 6c75  nFont(_fi.absolu
-00013080: 7465 4669 6c65 5061 7468 2829 290a 2020  teFilePath()).  
-00013090: 2020 2020 2020 666f 6e74 5f66 616d 696c        font_famil
-000130a0: 6965 7320 7c3d 2073 6574 2851 466f 6e74  ies |= set(QFont
-000130b0: 4461 7461 6261 7365 2e61 7070 6c69 6361  Database.applica
-000130c0: 7469 6f6e 466f 6e74 4661 6d69 6c69 6573  tionFontFamilies
-000130d0: 285f 6964 2929 0a20 2020 2072 6574 7572  (_id)).    retur
-000130e0: 6e20 666f 6e74 5f66 616d 696c 6965 730a  n font_families.
-000130f0: 0a0a 6465 6620 696e 7374 616c 6c5f 6963  ..def install_ic
-00013100: 6f6e 7328 293a 0a20 2020 2022 2222 496e  ons():.    """In
-00013110: 7374 616c 6c20 6963 6f6e 7322 2222 0a20  stall icons""". 
-00013120: 2020 206f 732e 7379 7374 656d 280a 2020     os.system(.  
-00013130: 2020 2020 2020 2278 6467 2d69 636f 6e2d        "xdg-icon-
-00013140: 7265 736f 7572 6365 2069 6e73 7461 6c6c  resource install
-00013150: 202d 2d73 697a 6520 3332 202d 2d63 6f6e   --size 32 --con
-00013160: 7465 7874 2061 7070 7320 2d2d 6d6f 6465  text apps --mode
-00013170: 2075 7365 7220 220a 2020 2020 2020 2020   user ".        
-00013180: 6622 7b57 4f52 4b49 4e47 5f50 4154 487d  f"{WORKING_PATH}
-00013190: 2f64 6174 612f 6b36 6774 652e 6e6f 7431  /data/k6gte.not1
-000131a0: 6d6d 2d33 322e 706e 6720 6b36 6774 652d  mm-32.png k6gte-
-000131b0: 6e6f 7431 6d6d 220a 2020 2020 290a 2020  not1mm".    ).  
-000131c0: 2020 6f73 2e73 7973 7465 6d28 0a20 2020    os.system(.   
-000131d0: 2020 2020 2022 7864 672d 6963 6f6e 2d72       "xdg-icon-r
-000131e0: 6573 6f75 7263 6520 696e 7374 616c 6c20  esource install 
-000131f0: 2d2d 7369 7a65 2036 3420 2d2d 636f 6e74  --size 64 --cont
-00013200: 6578 7420 6170 7073 202d 2d6d 6f64 6520  ext apps --mode 
-00013210: 7573 6572 2022 0a20 2020 2020 2020 2066  user ".        f
-00013220: 227b 574f 524b 494e 475f 5041 5448 7d2f  "{WORKING_PATH}/
-00013230: 6461 7461 2f6b 3667 7465 2e6e 6f74 316d  data/k6gte.not1m
-00013240: 6d2d 3634 2e70 6e67 206b 3667 7465 2d6e  m-64.png k6gte-n
-00013250: 6f74 316d 6d22 0a20 2020 2029 0a20 2020  ot1mm".    ).   
-00013260: 206f 732e 7379 7374 656d 280a 2020 2020   os.system(.    
-00013270: 2020 2020 2278 6467 2d69 636f 6e2d 7265      "xdg-icon-re
-00013280: 736f 7572 6365 2069 6e73 7461 6c6c 202d  source install -
-00013290: 2d73 697a 6520 3132 3820 2d2d 636f 6e74  -size 128 --cont
-000132a0: 6578 7420 6170 7073 202d 2d6d 6f64 6520  ext apps --mode 
-000132b0: 7573 6572 2022 0a20 2020 2020 2020 2066  user ".        f
-000132c0: 227b 574f 524b 494e 475f 5041 5448 7d2f  "{WORKING_PATH}/
-000132d0: 6461 7461 2f6b 3667 7465 2e6e 6f74 316d  data/k6gte.not1m
-000132e0: 6d2d 3132 382e 706e 6720 6b36 6774 652d  m-128.png k6gte-
-000132f0: 6e6f 7431 6d6d 220a 2020 2020 290a 2020  not1mm".    ).  
-00013300: 2020 6f73 2e73 7973 7465 6d28 6622 7864    os.system(f"xd
-00013310: 672d 6465 736b 746f 702d 6d65 6e75 2069  g-desktop-menu i
-00013320: 6e73 7461 6c6c 207b 574f 524b 494e 475f  nstall {WORKING_
-00013330: 5041 5448 7d2f 6461 7461 2f6b 3667 7465  PATH}/data/k6gte
-00013340: 2d6e 6f74 316d 6d2e 6465 736b 746f 7022  -not1mm.desktop"
-00013350: 290a 0a0a 6465 6620 646f 696d 7028 6d6f  )...def doimp(mo
-00013360: 646e 616d 6529 3a0a 2020 2020 2222 2272  dname):.    """r
-00013370: 6574 7572 6e20 6d6f 6475 6c65 2070 6174  eturn module pat
-00013380: 6822 2222 0a20 2020 2072 6574 7572 6e20  h""".    return 
-00013390: 696d 706f 7274 6c69 622e 696d 706f 7274  importlib.import
-000133a0: 5f6d 6f64 756c 6528 6622 6e6f 7431 6d6d  _module(f"not1mm
-000133b0: 2e70 6c75 6769 6e73 2e7b 6d6f 646e 616d  .plugins.{modnam
-000133c0: 657d 2229 0a0a 0a64 6566 2072 756e 2829  e}")...def run()
-000133d0: 3a0a 2020 2020 2222 220a 2020 2020 4d61  :.    """.    Ma
-000133e0: 696e 2045 6e74 7279 0a20 2020 2022 2222  in Entry.    """
-000133f0: 0a0a 2020 2020 696e 7374 616c 6c5f 6963  ..    install_ic
-00013400: 6f6e 7328 290a 2020 2020 7469 6d65 722e  ons().    timer.
-00013410: 7374 6172 7428 3130 3029 0a20 2020 2074  start(100).    t
-00013420: 696d 6572 322e 7374 6172 7428 3235 3029  imer2.start(250)
-00013430: 0a0a 2020 2020 7379 732e 6578 6974 2861  ..    sys.exit(a
-00013440: 7070 2e65 7865 6328 2929 0a0a 0a6c 6f67  pp.exec())...log
-00013450: 6765 7220 3d20 6c6f 6767 696e 672e 6765  ger = logging.ge
-00013460: 744c 6f67 6765 7228 225f 5f6d 6169 6e5f  tLogger("__main_
-00013470: 5f22 290a 6861 6e64 6c65 7220 3d20 6c6f  _").handler = lo
-00013480: 6767 696e 672e 5374 7265 616d 4861 6e64  gging.StreamHand
-00013490: 6c65 7228 290a 666f 726d 6174 7465 7220  ler().formatter 
-000134a0: 3d20 6c6f 6767 696e 672e 466f 726d 6174  = logging.Format
-000134b0: 7465 7228 0a20 2020 2064 6174 6566 6d74  ter(.    datefmt
-000134c0: 3d22 2548 3a25 4d3a 2553 222c 0a20 2020  ="%H:%M:%S",.   
-000134d0: 2066 6d74 3d22 5b25 2861 7363 7469 6d65   fmt="[%(asctime
-000134e0: 2973 5d20 2528 6c65 7665 6c6e 616d 6529  )s] %(levelname)
-000134f0: 7320 2528 6d6f 6475 6c65 2973 202d 2025  s %(module)s - %
-00013500: 2866 756e 634e 616d 6529 7320 4c69 6e65  (funcName)s Line
-00013510: 2025 286c 696e 656e 6f29 643a 2025 286d   %(lineno)d: %(m
-00013520: 6573 7361 6765 2973 222c 0a29 0a68 616e  essage)s",.).han
-00013530: 646c 6572 2e73 6574 466f 726d 6174 7465  dler.setFormatte
-00013540: 7228 666f 726d 6174 7465 7229 0a6c 6f67  r(formatter).log
-00013550: 6765 722e 6164 6448 616e 646c 6572 2868  ger.addHandler(h
-00013560: 616e 646c 6572 290a 0a69 6620 5061 7468  andler)..if Path
-00013570: 2822 2e2f 6465 6275 6722 292e 6578 6973  ("./debug").exis
-00013580: 7473 2829 3a0a 2020 2020 6c6f 6767 6572  ts():.    logger
-00013590: 2e73 6574 4c65 7665 6c28 6c6f 6767 696e  .setLevel(loggin
-000135a0: 672e 4445 4255 4729 0a20 2020 206c 6f67  g.DEBUG).    log
-000135b0: 6765 722e 6465 6275 6728 2264 6562 7567  ger.debug("debug
-000135c0: 6769 6e67 206f 6e22 290a 656c 7365 3a0a  ging on").else:.
-000135d0: 2020 2020 6c6f 6767 6572 2e73 6574 4c65      logger.setLe
-000135e0: 7665 6c28 6c6f 6767 696e 672e 5741 524e  vel(logging.WARN
-000135f0: 494e 4729 0a20 2020 206c 6f67 6765 722e  ING).    logger.
-00013600: 7761 726e 696e 6728 2264 6562 7567 6769  warning("debuggi
-00013610: 6e67 206f 6666 2229 0a0a 6170 7020 3d20  ng off")..app = 
-00013620: 5174 5769 6467 6574 732e 5141 7070 6c69  QtWidgets.QAppli
-00013630: 6361 7469 6f6e 2873 7973 2e61 7267 7629  cation(sys.argv)
-00013640: 0a23 2061 7070 2e73 6574 5374 796c 6528  .# app.setStyle(
-00013650: 2246 7573 696f 6e22 290a 666f 6e74 5f70  "Fusion").font_p
-00013660: 6174 6820 3d20 574f 524b 494e 475f 5041  ath = WORKING_PA
-00013670: 5448 202b 2022 2f64 6174 6122 0a66 616d  TH + "/data".fam
-00013680: 696c 6965 7320 3d20 6c6f 6164 5f66 6f6e  ilies = load_fon
-00013690: 7473 5f66 726f 6d5f 6469 7228 6f73 2e66  ts_from_dir(os.f
-000136a0: 7370 6174 6828 666f 6e74 5f70 6174 6829  spath(font_path)
-000136b0: 290a 6c6f 6767 6572 2e69 6e66 6f28 6661  ).logger.info(fa
-000136c0: 6d69 6c69 6573 290a 7769 6e64 6f77 203d  milies).window =
-000136d0: 204d 6169 6e57 696e 646f 7728 290a 6865   MainWindow().he
-000136e0: 6967 6874 203d 2077 696e 646f 772e 7072  ight = window.pr
-000136f0: 6566 2e67 6574 2822 7769 6e64 6f77 5f68  ef.get("window_h
-00013700: 6569 6768 7422 2c20 3330 3029 0a77 6964  eight", 300).wid
-00013710: 7468 203d 2077 696e 646f 772e 7072 6566  th = window.pref
-00013720: 2e67 6574 2822 7769 6e64 6f77 5f77 6964  .get("window_wid
-00013730: 7468 222c 2037 3030 290a 7820 3d20 7769  th", 700).x = wi
-00013740: 6e64 6f77 2e70 7265 662e 6765 7428 2277  ndow.pref.get("w
-00013750: 696e 646f 775f 7822 2c20 2d31 290a 7920  indow_x", -1).y 
-00013760: 3d20 7769 6e64 6f77 2e70 7265 662e 6765  = window.pref.ge
-00013770: 7428 2277 696e 646f 775f 7922 2c20 2d31  t("window_y", -1
-00013780: 290a 7769 6e64 6f77 2e73 6574 4765 6f6d  ).window.setGeom
-00013790: 6574 7279 2878 2c20 792c 2077 6964 7468  etry(x, y, width
-000137a0: 2c20 6865 6967 6874 290a 2320 7769 6e64  , height).# wind
-000137b0: 6f77 2e73 6574 5769 6e64 6f77 5469 746c  ow.setWindowTitl
-000137c0: 6528 6622 4e6f 7431 4d4d 2076 7b5f 5f76  e(f"Not1MM v{__v
-000137d0: 6572 7369 6f6e 5f5f 7d22 290a 7769 6e64  ersion__}").wind
-000137e0: 6f77 2e63 616c 6c73 6967 6e2e 7365 7446  ow.callsign.setF
-000137f0: 6f63 7573 2829 0a77 696e 646f 772e 7368  ocus().window.sh
-00013800: 6f77 2829 0a74 696d 6572 203d 2051 7443  ow().timer = QtC
-00013810: 6f72 652e 5154 696d 6572 2829 0a74 696d  ore.QTimer().tim
-00013820: 6572 2e74 696d 656f 7574 2e63 6f6e 6e65  er.timeout.conne
-00013830: 6374 2877 696e 646f 772e 706f 6c6c 5f72  ct(window.poll_r
-00013840: 6164 696f 290a 7469 6d65 7232 203d 2051  adio).timer2 = Q
-00013850: 7443 6f72 652e 5154 696d 6572 2829 0a74  tCore.QTimer().t
-00013860: 696d 6572 322e 7469 6d65 6f75 742e 636f  imer2.timeout.co
-00013870: 6e6e 6563 7428 7769 6e64 6f77 2e63 6865  nnect(window.che
-00013880: 636b 5f75 6470 5f74 7261 6666 6963 290a  ck_udp_traffic).
-00013890: 0a69 6620 5f5f 6e61 6d65 5f5f 203d 3d20  .if __name__ == 
-000138a0: 225f 5f6d 6169 6e5f 5f22 3a0a 2020 2020  "__main__":.    
-000138b0: 7275 6e28 290a                           run().
+00012770: 6578 6365 7074 2056 616c 7565 4572 726f  except ValueErro
+00012780: 7220 6173 2065 7272 3a0a 2020 2020 2020  r as err:.      
+00012790: 2020 2020 2020 2020 2020 2020 2020 6c6f                lo
+000127a0: 6767 6572 2e69 6e66 6f28 2272 6561 645f  gger.info("read_
+000127b0: 6377 5f6d 6163 726f 733a 2025 7322 2c20  cw_macros: %s", 
+000127c0: 6572 7229 0a20 2020 2020 2020 206b 6579  err).        key
+000127d0: 7320 3d20 7365 6c66 2e66 6b65 7973 2e6b  s = self.fkeys.k
+000127e0: 6579 7328 290a 2020 2020 2020 2020 6966  eys().        if
+000127f0: 2022 4631 2220 696e 206b 6579 733a 0a20   "F1" in keys:. 
+00012800: 2020 2020 2020 2020 2020 2073 656c 662e             self.
+00012810: 4631 2e73 6574 5465 7874 2866 2246 313a  F1.setText(f"F1:
+00012820: 207b 7365 6c66 2e66 6b65 7973 5b27 4631   {self.fkeys['F1
+00012830: 275d 5b30 5d7d 2229 0a20 2020 2020 2020  '][0]}").       
+00012840: 2020 2020 2073 656c 662e 4631 2e73 6574       self.F1.set
+00012850: 546f 6f6c 5469 7028 7365 6c66 2e66 6b65  ToolTip(self.fke
+00012860: 7973 5b22 4631 225d 5b31 5d29 0a20 2020  ys["F1"][1]).   
+00012870: 2020 2020 2069 6620 2246 3222 2069 6e20       if "F2" in 
+00012880: 6b65 7973 3a0a 2020 2020 2020 2020 2020  keys:.          
+00012890: 2020 7365 6c66 2e46 322e 7365 7454 6578    self.F2.setTex
+000128a0: 7428 6622 4632 3a20 7b73 656c 662e 666b  t(f"F2: {self.fk
+000128b0: 6579 735b 2746 3227 5d5b 305d 7d22 290a  eys['F2'][0]}").
+000128c0: 2020 2020 2020 2020 2020 2020 7365 6c66              self
+000128d0: 2e46 322e 7365 7454 6f6f 6c54 6970 2873  .F2.setToolTip(s
+000128e0: 656c 662e 666b 6579 735b 2246 3222 5d5b  elf.fkeys["F2"][
+000128f0: 315d 290a 2020 2020 2020 2020 6966 2022  1]).        if "
+00012900: 4633 2220 696e 206b 6579 733a 0a20 2020  F3" in keys:.   
+00012910: 2020 2020 2020 2020 2073 656c 662e 4633           self.F3
+00012920: 2e73 6574 5465 7874 2866 2246 333a 207b  .setText(f"F3: {
+00012930: 7365 6c66 2e66 6b65 7973 5b27 4633 275d  self.fkeys['F3']
+00012940: 5b30 5d7d 2229 0a20 2020 2020 2020 2020  [0]}").         
+00012950: 2020 2073 656c 662e 4633 2e73 6574 546f     self.F3.setTo
+00012960: 6f6c 5469 7028 7365 6c66 2e66 6b65 7973  olTip(self.fkeys
+00012970: 5b22 4633 225d 5b31 5d29 0a20 2020 2020  ["F3"][1]).     
+00012980: 2020 2069 6620 2246 3422 2069 6e20 6b65     if "F4" in ke
+00012990: 7973 3a0a 2020 2020 2020 2020 2020 2020  ys:.            
+000129a0: 7365 6c66 2e46 342e 7365 7454 6578 7428  self.F4.setText(
+000129b0: 6622 4634 3a20 7b73 656c 662e 666b 6579  f"F4: {self.fkey
+000129c0: 735b 2746 3427 5d5b 305d 7d22 290a 2020  s['F4'][0]}").  
+000129d0: 2020 2020 2020 2020 2020 7365 6c66 2e46            self.F
+000129e0: 342e 7365 7454 6f6f 6c54 6970 2873 656c  4.setToolTip(sel
+000129f0: 662e 666b 6579 735b 2246 3422 5d5b 315d  f.fkeys["F4"][1]
+00012a00: 290a 2020 2020 2020 2020 6966 2022 4635  ).        if "F5
+00012a10: 2220 696e 206b 6579 733a 0a20 2020 2020  " in keys:.     
+00012a20: 2020 2020 2020 2073 656c 662e 4635 2e73         self.F5.s
+00012a30: 6574 5465 7874 2866 2246 353a 207b 7365  etText(f"F5: {se
+00012a40: 6c66 2e66 6b65 7973 5b27 4635 275d 5b30  lf.fkeys['F5'][0
+00012a50: 5d7d 2229 0a20 2020 2020 2020 2020 2020  ]}").           
+00012a60: 2073 656c 662e 4635 2e73 6574 546f 6f6c   self.F5.setTool
+00012a70: 5469 7028 7365 6c66 2e66 6b65 7973 5b22  Tip(self.fkeys["
+00012a80: 4635 225d 5b31 5d29 0a20 2020 2020 2020  F5"][1]).       
+00012a90: 2069 6620 2246 3622 2069 6e20 6b65 7973   if "F6" in keys
+00012aa0: 3a0a 2020 2020 2020 2020 2020 2020 7365  :.            se
+00012ab0: 6c66 2e46 362e 7365 7454 6578 7428 6622  lf.F6.setText(f"
+00012ac0: 4636 3a20 7b73 656c 662e 666b 6579 735b  F6: {self.fkeys[
+00012ad0: 2746 3627 5d5b 305d 7d22 290a 2020 2020  'F6'][0]}").    
+00012ae0: 2020 2020 2020 2020 7365 6c66 2e46 362e          self.F6.
+00012af0: 7365 7454 6f6f 6c54 6970 2873 656c 662e  setToolTip(self.
+00012b00: 666b 6579 735b 2246 3622 5d5b 315d 290a  fkeys["F6"][1]).
+00012b10: 2020 2020 2020 2020 6966 2022 4637 2220          if "F7" 
+00012b20: 696e 206b 6579 733a 0a20 2020 2020 2020  in keys:.       
+00012b30: 2020 2020 2073 656c 662e 4637 2e73 6574       self.F7.set
+00012b40: 5465 7874 2866 2246 373a 207b 7365 6c66  Text(f"F7: {self
+00012b50: 2e66 6b65 7973 5b27 4637 275d 5b30 5d7d  .fkeys['F7'][0]}
+00012b60: 2229 0a20 2020 2020 2020 2020 2020 2073  ").            s
+00012b70: 656c 662e 4637 2e73 6574 546f 6f6c 5469  elf.F7.setToolTi
+00012b80: 7028 7365 6c66 2e66 6b65 7973 5b22 4637  p(self.fkeys["F7
+00012b90: 225d 5b31 5d29 0a20 2020 2020 2020 2069  "][1]).        i
+00012ba0: 6620 2246 3822 2069 6e20 6b65 7973 3a0a  f "F8" in keys:.
+00012bb0: 2020 2020 2020 2020 2020 2020 7365 6c66              self
+00012bc0: 2e46 382e 7365 7454 6578 7428 6622 4638  .F8.setText(f"F8
+00012bd0: 3a20 7b73 656c 662e 666b 6579 735b 2746  : {self.fkeys['F
+00012be0: 3827 5d5b 305d 7d22 290a 2020 2020 2020  8'][0]}").      
+00012bf0: 2020 2020 2020 7365 6c66 2e46 382e 7365        self.F8.se
+00012c00: 7454 6f6f 6c54 6970 2873 656c 662e 666b  tToolTip(self.fk
+00012c10: 6579 735b 2246 3822 5d5b 315d 290a 2020  eys["F8"][1]).  
+00012c20: 2020 2020 2020 6966 2022 4639 2220 696e        if "F9" in
+00012c30: 206b 6579 733a 0a20 2020 2020 2020 2020   keys:.         
+00012c40: 2020 2073 656c 662e 4639 2e73 6574 5465     self.F9.setTe
+00012c50: 7874 2866 2246 393a 207b 7365 6c66 2e66  xt(f"F9: {self.f
+00012c60: 6b65 7973 5b27 4639 275d 5b30 5d7d 2229  keys['F9'][0]}")
+00012c70: 0a20 2020 2020 2020 2020 2020 2073 656c  .            sel
+00012c80: 662e 4639 2e73 6574 546f 6f6c 5469 7028  f.F9.setToolTip(
+00012c90: 7365 6c66 2e66 6b65 7973 5b22 4639 225d  self.fkeys["F9"]
+00012ca0: 5b31 5d29 0a20 2020 2020 2020 2069 6620  [1]).        if 
+00012cb0: 2246 3130 2220 696e 206b 6579 733a 0a20  "F10" in keys:. 
+00012cc0: 2020 2020 2020 2020 2020 2073 656c 662e             self.
+00012cd0: 4631 302e 7365 7454 6578 7428 6622 4631  F10.setText(f"F1
+00012ce0: 303a 207b 7365 6c66 2e66 6b65 7973 5b27  0: {self.fkeys['
+00012cf0: 4631 3027 5d5b 305d 7d22 290a 2020 2020  F10'][0]}").    
+00012d00: 2020 2020 2020 2020 7365 6c66 2e46 3130          self.F10
+00012d10: 2e73 6574 546f 6f6c 5469 7028 7365 6c66  .setToolTip(self
+00012d20: 2e66 6b65 7973 5b22 4631 3022 5d5b 315d  .fkeys["F10"][1]
+00012d30: 290a 2020 2020 2020 2020 6966 2022 4631  ).        if "F1
+00012d40: 3122 2069 6e20 6b65 7973 3a0a 2020 2020  1" in keys:.    
+00012d50: 2020 2020 2020 2020 7365 6c66 2e46 3131          self.F11
+00012d60: 2e73 6574 5465 7874 2866 2246 3131 3a20  .setText(f"F11: 
+00012d70: 7b73 656c 662e 666b 6579 735b 2746 3131  {self.fkeys['F11
+00012d80: 275d 5b30 5d7d 2229 0a20 2020 2020 2020  '][0]}").       
+00012d90: 2020 2020 2073 656c 662e 4631 312e 7365       self.F11.se
+00012da0: 7454 6f6f 6c54 6970 2873 656c 662e 666b  tToolTip(self.fk
+00012db0: 6579 735b 2246 3131 225d 5b31 5d29 0a20  eys["F11"][1]). 
+00012dc0: 2020 2020 2020 2069 6620 2246 3132 2220         if "F12" 
+00012dd0: 696e 206b 6579 733a 0a20 2020 2020 2020  in keys:.       
+00012de0: 2020 2020 2073 656c 662e 4631 322e 7365       self.F12.se
+00012df0: 7454 6578 7428 6622 4631 323a 207b 7365  tText(f"F12: {se
+00012e00: 6c66 2e66 6b65 7973 5b27 4631 3227 5d5b  lf.fkeys['F12'][
+00012e10: 305d 7d22 290a 2020 2020 2020 2020 2020  0]}").          
+00012e20: 2020 7365 6c66 2e46 3132 2e73 6574 546f    self.F12.setTo
+00012e30: 6f6c 5469 7028 7365 6c66 2e66 6b65 7973  olTip(self.fkeys
+00012e40: 5b22 4631 3222 5d5b 315d 290a 0a20 2020  ["F12"][1])..   
+00012e50: 2064 6566 2067 656e 6572 6174 655f 6164   def generate_ad
+00012e60: 6966 2873 656c 6629 3a0a 2020 2020 2020  if(self):.      
+00012e70: 2020 2222 2247 656e 6572 6174 6520 4144    """Generate AD
+00012e80: 4946 2222 220a 2020 2020 2020 2020 6c6f  IF""".        lo
+00012e90: 6767 6572 2e64 6562 7567 2822 2a2a 2a2a  gger.debug("****
+00012ea0: 2a2a 4144 4946 2a2a 2a2a 2a22 290a 2020  **ADIF*****").  
+00012eb0: 2020 2020 2020 7365 6c66 2e63 6f6e 7465        self.conte
+00012ec0: 7374 2e61 6469 6628 7365 6c66 290a 0a20  st.adif(self).. 
+00012ed0: 2020 2064 6566 2067 656e 6572 6174 655f     def generate_
+00012ee0: 6361 6272 696c 6c6f 2873 656c 6629 3a0a  cabrillo(self):.
+00012ef0: 2020 2020 2020 2020 2222 2247 656e 6572          """Gener
+00012f00: 6174 6573 2043 6162 7269 6c6c 6f20 6669  ates Cabrillo fi
+00012f10: 6c65 2e20 4d61 7962 652e 2222 220a 2020  le. Maybe.""".  
+00012f20: 2020 2020 2020 2320 6874 7470 733a 2f2f        # https://
+00012f30: 7777 772e 6371 7770 782e 636f 6d2f 6361  www.cqwpx.com/ca
+00012f40: 6272 696c 6c6f 2e68 746d 0a20 2020 2020  brillo.htm.     
+00012f50: 2020 206c 6f67 6765 722e 6465 6275 6728     logger.debug(
+00012f60: 222a 2a2a 2a2a 2a43 6162 7269 6c6c 6f2a  "******Cabrillo*
+00012f70: 2a2a 2a2a 2229 0a20 2020 2020 2020 2073  ****").        s
+00012f80: 656c 662e 636f 6e74 6573 742e 6361 6272  elf.contest.cabr
+00012f90: 696c 6c6f 2873 656c 6629 0a0a 0a64 6566  illo(self)...def
+00012fa0: 206c 6f61 645f 666f 6e74 735f 6672 6f6d   load_fonts_from
+00012fb0: 5f64 6972 2864 6972 6563 746f 7279 3a20  _dir(directory: 
+00012fc0: 7374 7229 202d 3e20 7365 743a 0a20 2020  str) -> set:.   
+00012fd0: 2022 2222 0a20 2020 2057 656c 6c20 6974   """.    Well it
+00012fe0: 206c 6f61 6473 2066 6f6e 7473 2066 726f   loads fonts fro
+00012ff0: 6d20 6120 6469 7265 6374 6f72 792e 2e2e  m a directory...
+00013000: 0a20 2020 2022 2222 0a20 2020 2066 6f6e  .    """.    fon
+00013010: 745f 6661 6d69 6c69 6573 203d 2073 6574  t_families = set
+00013020: 2829 0a20 2020 2066 6f72 205f 6669 2069  ().    for _fi i
+00013030: 6e20 5144 6972 2864 6972 6563 746f 7279  n QDir(directory
+00013040: 292e 656e 7472 7949 6e66 6f4c 6973 7428  ).entryInfoList(
+00013050: 5b22 2a2e 7474 6622 2c20 222a 2e77 6f66  ["*.ttf", "*.wof
+00013060: 6622 2c20 222a 2e77 6f66 6632 225d 293a  f", "*.woff2"]):
+00013070: 0a20 2020 2020 2020 205f 6964 203d 2051  .        _id = Q
+00013080: 466f 6e74 4461 7461 6261 7365 2e61 6464  FontDatabase.add
+00013090: 4170 706c 6963 6174 696f 6e46 6f6e 7428  ApplicationFont(
+000130a0: 5f66 692e 6162 736f 6c75 7465 4669 6c65  _fi.absoluteFile
+000130b0: 5061 7468 2829 290a 2020 2020 2020 2020  Path()).        
+000130c0: 666f 6e74 5f66 616d 696c 6965 7320 7c3d  font_families |=
+000130d0: 2073 6574 2851 466f 6e74 4461 7461 6261   set(QFontDataba
+000130e0: 7365 2e61 7070 6c69 6361 7469 6f6e 466f  se.applicationFo
+000130f0: 6e74 4661 6d69 6c69 6573 285f 6964 2929  ntFamilies(_id))
+00013100: 0a20 2020 2072 6574 7572 6e20 666f 6e74  .    return font
+00013110: 5f66 616d 696c 6965 730a 0a0a 6465 6620  _families...def 
+00013120: 696e 7374 616c 6c5f 6963 6f6e 7328 293a  install_icons():
+00013130: 0a20 2020 2022 2222 496e 7374 616c 6c20  .    """Install 
+00013140: 6963 6f6e 7322 2222 0a20 2020 206f 732e  icons""".    os.
+00013150: 7379 7374 656d 280a 2020 2020 2020 2020  system(.        
+00013160: 2278 6467 2d69 636f 6e2d 7265 736f 7572  "xdg-icon-resour
+00013170: 6365 2069 6e73 7461 6c6c 202d 2d73 697a  ce install --siz
+00013180: 6520 3332 202d 2d63 6f6e 7465 7874 2061  e 32 --context a
+00013190: 7070 7320 2d2d 6d6f 6465 2075 7365 7220  pps --mode user 
+000131a0: 220a 2020 2020 2020 2020 6622 7b57 4f52  ".        f"{WOR
+000131b0: 4b49 4e47 5f50 4154 487d 2f64 6174 612f  KING_PATH}/data/
+000131c0: 6b36 6774 652e 6e6f 7431 6d6d 2d33 322e  k6gte.not1mm-32.
+000131d0: 706e 6720 6b36 6774 652d 6e6f 7431 6d6d  png k6gte-not1mm
+000131e0: 220a 2020 2020 290a 2020 2020 6f73 2e73  ".    ).    os.s
+000131f0: 7973 7465 6d28 0a20 2020 2020 2020 2022  ystem(.        "
+00013200: 7864 672d 6963 6f6e 2d72 6573 6f75 7263  xdg-icon-resourc
+00013210: 6520 696e 7374 616c 6c20 2d2d 7369 7a65  e install --size
+00013220: 2036 3420 2d2d 636f 6e74 6578 7420 6170   64 --context ap
+00013230: 7073 202d 2d6d 6f64 6520 7573 6572 2022  ps --mode user "
+00013240: 0a20 2020 2020 2020 2066 227b 574f 524b  .        f"{WORK
+00013250: 494e 475f 5041 5448 7d2f 6461 7461 2f6b  ING_PATH}/data/k
+00013260: 3667 7465 2e6e 6f74 316d 6d2d 3634 2e70  6gte.not1mm-64.p
+00013270: 6e67 206b 3667 7465 2d6e 6f74 316d 6d22  ng k6gte-not1mm"
+00013280: 0a20 2020 2029 0a20 2020 206f 732e 7379  .    ).    os.sy
+00013290: 7374 656d 280a 2020 2020 2020 2020 2278  stem(.        "x
+000132a0: 6467 2d69 636f 6e2d 7265 736f 7572 6365  dg-icon-resource
+000132b0: 2069 6e73 7461 6c6c 202d 2d73 697a 6520   install --size 
+000132c0: 3132 3820 2d2d 636f 6e74 6578 7420 6170  128 --context ap
+000132d0: 7073 202d 2d6d 6f64 6520 7573 6572 2022  ps --mode user "
+000132e0: 0a20 2020 2020 2020 2066 227b 574f 524b  .        f"{WORK
+000132f0: 494e 475f 5041 5448 7d2f 6461 7461 2f6b  ING_PATH}/data/k
+00013300: 3667 7465 2e6e 6f74 316d 6d2d 3132 382e  6gte.not1mm-128.
+00013310: 706e 6720 6b36 6774 652d 6e6f 7431 6d6d  png k6gte-not1mm
+00013320: 220a 2020 2020 290a 2020 2020 6f73 2e73  ".    ).    os.s
+00013330: 7973 7465 6d28 6622 7864 672d 6465 736b  ystem(f"xdg-desk
+00013340: 746f 702d 6d65 6e75 2069 6e73 7461 6c6c  top-menu install
+00013350: 207b 574f 524b 494e 475f 5041 5448 7d2f   {WORKING_PATH}/
+00013360: 6461 7461 2f6b 3667 7465 2d6e 6f74 316d  data/k6gte-not1m
+00013370: 6d2e 6465 736b 746f 7022 290a 0a0a 6465  m.desktop")...de
+00013380: 6620 646f 696d 7028 6d6f 646e 616d 6529  f doimp(modname)
+00013390: 3a0a 2020 2020 2222 2272 6574 7572 6e20  :.    """return 
+000133a0: 6d6f 6475 6c65 2070 6174 6822 2222 0a20  module path""". 
+000133b0: 2020 2072 6574 7572 6e20 696d 706f 7274     return import
+000133c0: 6c69 622e 696d 706f 7274 5f6d 6f64 756c  lib.import_modul
+000133d0: 6528 6622 6e6f 7431 6d6d 2e70 6c75 6769  e(f"not1mm.plugi
+000133e0: 6e73 2e7b 6d6f 646e 616d 657d 2229 0a0a  ns.{modname}")..
+000133f0: 0a64 6566 2072 756e 2829 3a0a 2020 2020  .def run():.    
+00013400: 2222 220a 2020 2020 4d61 696e 2045 6e74  """.    Main Ent
+00013410: 7279 0a20 2020 2022 2222 0a0a 2020 2020  ry.    """..    
+00013420: 696e 7374 616c 6c5f 6963 6f6e 7328 290a  install_icons().
+00013430: 2020 2020 7469 6d65 722e 7374 6172 7428      timer.start(
+00013440: 3130 3029 0a20 2020 2074 696d 6572 322e  100).    timer2.
+00013450: 7374 6172 7428 3235 3029 0a0a 2020 2020  start(250)..    
+00013460: 7379 732e 6578 6974 2861 7070 2e65 7865  sys.exit(app.exe
+00013470: 6328 2929 0a0a 0a6c 6f67 6765 7220 3d20  c())...logger = 
+00013480: 6c6f 6767 696e 672e 6765 744c 6f67 6765  logging.getLogge
+00013490: 7228 225f 5f6d 6169 6e5f 5f22 290a 6861  r("__main__").ha
+000134a0: 6e64 6c65 7220 3d20 6c6f 6767 696e 672e  ndler = logging.
+000134b0: 5374 7265 616d 4861 6e64 6c65 7228 290a  StreamHandler().
+000134c0: 666f 726d 6174 7465 7220 3d20 6c6f 6767  formatter = logg
+000134d0: 696e 672e 466f 726d 6174 7465 7228 0a20  ing.Formatter(. 
+000134e0: 2020 2064 6174 6566 6d74 3d22 2548 3a25     datefmt="%H:%
+000134f0: 4d3a 2553 222c 0a20 2020 2066 6d74 3d22  M:%S",.    fmt="
+00013500: 5b25 2861 7363 7469 6d65 2973 5d20 2528  [%(asctime)s] %(
+00013510: 6c65 7665 6c6e 616d 6529 7320 2528 6d6f  levelname)s %(mo
+00013520: 6475 6c65 2973 202d 2025 2866 756e 634e  dule)s - %(funcN
+00013530: 616d 6529 7320 4c69 6e65 2025 286c 696e  ame)s Line %(lin
+00013540: 656e 6f29 643a 2025 286d 6573 7361 6765  eno)d: %(message
+00013550: 2973 222c 0a29 0a68 616e 646c 6572 2e73  )s",.).handler.s
+00013560: 6574 466f 726d 6174 7465 7228 666f 726d  etFormatter(form
+00013570: 6174 7465 7229 0a6c 6f67 6765 722e 6164  atter).logger.ad
+00013580: 6448 616e 646c 6572 2868 616e 646c 6572  dHandler(handler
+00013590: 290a 0a69 6620 5061 7468 2822 2e2f 6465  )..if Path("./de
+000135a0: 6275 6722 292e 6578 6973 7473 2829 3a0a  bug").exists():.
+000135b0: 2020 2020 6c6f 6767 6572 2e73 6574 4c65      logger.setLe
+000135c0: 7665 6c28 6c6f 6767 696e 672e 4445 4255  vel(logging.DEBU
+000135d0: 4729 0a20 2020 206c 6f67 6765 722e 6465  G).    logger.de
+000135e0: 6275 6728 2264 6562 7567 6769 6e67 206f  bug("debugging o
+000135f0: 6e22 290a 656c 7365 3a0a 2020 2020 6c6f  n").else:.    lo
+00013600: 6767 6572 2e73 6574 4c65 7665 6c28 6c6f  gger.setLevel(lo
+00013610: 6767 696e 672e 5741 524e 494e 4729 0a20  gging.WARNING). 
+00013620: 2020 206c 6f67 6765 722e 7761 726e 696e     logger.warnin
+00013630: 6728 2264 6562 7567 6769 6e67 206f 6666  g("debugging off
+00013640: 2229 0a0a 6170 7020 3d20 5174 5769 6467  ")..app = QtWidg
+00013650: 6574 732e 5141 7070 6c69 6361 7469 6f6e  ets.QApplication
+00013660: 2873 7973 2e61 7267 7629 0a23 2061 7070  (sys.argv).# app
+00013670: 2e73 6574 5374 796c 6528 2246 7573 696f  .setStyle("Fusio
+00013680: 6e22 290a 666f 6e74 5f70 6174 6820 3d20  n").font_path = 
+00013690: 574f 524b 494e 475f 5041 5448 202b 2022  WORKING_PATH + "
+000136a0: 2f64 6174 6122 0a66 616d 696c 6965 7320  /data".families 
+000136b0: 3d20 6c6f 6164 5f66 6f6e 7473 5f66 726f  = load_fonts_fro
+000136c0: 6d5f 6469 7228 6f73 2e66 7370 6174 6828  m_dir(os.fspath(
+000136d0: 666f 6e74 5f70 6174 6829 290a 6c6f 6767  font_path)).logg
+000136e0: 6572 2e69 6e66 6f28 6661 6d69 6c69 6573  er.info(families
+000136f0: 290a 7769 6e64 6f77 203d 204d 6169 6e57  ).window = MainW
+00013700: 696e 646f 7728 290a 6865 6967 6874 203d  indow().height =
+00013710: 2077 696e 646f 772e 7072 6566 2e67 6574   window.pref.get
+00013720: 2822 7769 6e64 6f77 5f68 6569 6768 7422  ("window_height"
+00013730: 2c20 3330 3029 0a77 6964 7468 203d 2077  , 300).width = w
+00013740: 696e 646f 772e 7072 6566 2e67 6574 2822  indow.pref.get("
+00013750: 7769 6e64 6f77 5f77 6964 7468 222c 2037  window_width", 7
+00013760: 3030 290a 7820 3d20 7769 6e64 6f77 2e70  00).x = window.p
+00013770: 7265 662e 6765 7428 2277 696e 646f 775f  ref.get("window_
+00013780: 7822 2c20 2d31 290a 7920 3d20 7769 6e64  x", -1).y = wind
+00013790: 6f77 2e70 7265 662e 6765 7428 2277 696e  ow.pref.get("win
+000137a0: 646f 775f 7922 2c20 2d31 290a 7769 6e64  dow_y", -1).wind
+000137b0: 6f77 2e73 6574 4765 6f6d 6574 7279 2878  ow.setGeometry(x
+000137c0: 2c20 792c 2077 6964 7468 2c20 6865 6967  , y, width, heig
+000137d0: 6874 290a 2320 7769 6e64 6f77 2e73 6574  ht).# window.set
+000137e0: 5769 6e64 6f77 5469 746c 6528 6622 4e6f  WindowTitle(f"No
+000137f0: 7431 4d4d 2076 7b5f 5f76 6572 7369 6f6e  t1MM v{__version
+00013800: 5f5f 7d22 290a 7769 6e64 6f77 2e63 616c  __}").window.cal
+00013810: 6c73 6967 6e2e 7365 7446 6f63 7573 2829  lsign.setFocus()
+00013820: 0a77 696e 646f 772e 7368 6f77 2829 0a74  .window.show().t
+00013830: 696d 6572 203d 2051 7443 6f72 652e 5154  imer = QtCore.QT
+00013840: 696d 6572 2829 0a74 696d 6572 2e74 696d  imer().timer.tim
+00013850: 656f 7574 2e63 6f6e 6e65 6374 2877 696e  eout.connect(win
+00013860: 646f 772e 706f 6c6c 5f72 6164 696f 290a  dow.poll_radio).
+00013870: 7469 6d65 7232 203d 2051 7443 6f72 652e  timer2 = QtCore.
+00013880: 5154 696d 6572 2829 0a74 696d 6572 322e  QTimer().timer2.
+00013890: 7469 6d65 6f75 742e 636f 6e6e 6563 7428  timeout.connect(
+000138a0: 7769 6e64 6f77 2e63 6865 636b 5f75 6470  window.check_udp
+000138b0: 5f74 7261 6666 6963 290a 0a69 6620 5f5f  _traffic)..if __
+000138c0: 6e61 6d65 5f5f 203d 3d20 225f 5f6d 6169  name__ == "__mai
+000138d0: 6e5f 5f22 3a0a 2020 2020 7275 6e28 290a  n__":.    run().
```

### Comparing `not1mm-23.5.9.1/not1mm/bandmap.py` & `not1mm-23.5.9.2/not1mm/bandmap.py`

 * *Files identical despite different names*

### Comparing `not1mm-23.5.9.1/not1mm/data/Combinear.qss` & `not1mm-23.5.9.2/not1mm/data/Combinear.qss`

 * *Files identical despite different names*

### Comparing `not1mm-23.5.9.1/not1mm/data/JetBrainsMono-Regular.ttf` & `not1mm-23.5.9.2/not1mm/data/JetBrainsMono-Regular.ttf`

 * *Files identical despite different names*

### Comparing `not1mm-23.5.9.1/not1mm/data/MASTER.SCP` & `not1mm-23.5.9.2/not1mm/data/MASTER.SCP`

 * *Files identical despite different names*

### Comparing `not1mm-23.5.9.1/not1mm/data/about.ui` & `not1mm-23.5.9.2/not1mm/data/about.ui`

 * *Files identical despite different names*

### Comparing `not1mm-23.5.9.1/not1mm/data/bandmap.ui` & `not1mm-23.5.9.2/not1mm/data/bandmap.ui`

 * *Files identical despite different names*

### Comparing `not1mm-23.5.9.1/not1mm/data/configuration.ui` & `not1mm-23.5.9.2/not1mm/data/configuration.ui`

 * *Files identical despite different names*

### Comparing `not1mm-23.5.9.1/not1mm/data/contests.sql` & `not1mm-23.5.9.2/not1mm/data/contests.sql`

 * *Files identical despite different names*

### Comparing `not1mm-23.5.9.1/not1mm/data/cty.json` & `not1mm-23.5.9.2/not1mm/data/cty.json`

 * *Files identical despite different names*

### Comparing `not1mm-23.5.9.1/not1mm/data/editcontact.ui` & `not1mm-23.5.9.2/not1mm/data/editcontact.ui`

 * *Files identical despite different names*

### Comparing `not1mm-23.5.9.1/not1mm/data/editmacro.ui` & `not1mm-23.5.9.2/not1mm/data/editmacro.ui`

 * *Files identical despite different names*

### Comparing `not1mm-23.5.9.1/not1mm/data/k6gte.not1mm-128.png` & `not1mm-23.5.9.2/not1mm/data/k6gte.not1mm-128.png`

 * *Files identical despite different names*

### Comparing `not1mm-23.5.9.1/not1mm/data/k6gte.not1mm-32.png` & `not1mm-23.5.9.2/not1mm/data/k6gte.not1mm-32.png`

 * *Files identical despite different names*

### Comparing `not1mm-23.5.9.1/not1mm/data/k6gte.not1mm-64.png` & `not1mm-23.5.9.2/not1mm/data/k6gte.not1mm-64.png`

 * *Files identical despite different names*

### Comparing `not1mm-23.5.9.1/not1mm/data/logwindow.ui` & `not1mm-23.5.9.2/not1mm/data/logwindow.ui`

 * *Files identical despite different names*

### Comparing `not1mm-23.5.9.1/not1mm/data/main.ui` & `not1mm-23.5.9.2/not1mm/data/main.ui`

 * *Files identical despite different names*

### Comparing `not1mm-23.5.9.1/not1mm/data/new_contest.ui` & `not1mm-23.5.9.2/not1mm/data/new_contest.ui`

 * *Files identical despite different names*

### Comparing `not1mm-23.5.9.1/not1mm/data/opon.ui` & `not1mm-23.5.9.2/not1mm/data/opon.ui`

 * *Files identical despite different names*

### Comparing `not1mm-23.5.9.1/not1mm/data/phonetics/0.wav` & `not1mm-23.5.9.2/not1mm/data/phonetics/0.wav`

 * *Files identical despite different names*

### Comparing `not1mm-23.5.9.1/not1mm/data/phonetics/1.wav` & `not1mm-23.5.9.2/not1mm/data/phonetics/1.wav`

 * *Files identical despite different names*

### Comparing `not1mm-23.5.9.1/not1mm/data/phonetics/2.wav` & `not1mm-23.5.9.2/not1mm/data/phonetics/2.wav`

 * *Files identical despite different names*

### Comparing `not1mm-23.5.9.1/not1mm/data/phonetics/3.wav` & `not1mm-23.5.9.2/not1mm/data/phonetics/3.wav`

 * *Files identical despite different names*

### Comparing `not1mm-23.5.9.1/not1mm/data/phonetics/4.wav` & `not1mm-23.5.9.2/not1mm/data/phonetics/4.wav`

 * *Files identical despite different names*

### Comparing `not1mm-23.5.9.1/not1mm/data/phonetics/5.wav` & `not1mm-23.5.9.2/not1mm/data/phonetics/5.wav`

 * *Files identical despite different names*

### Comparing `not1mm-23.5.9.1/not1mm/data/phonetics/6.wav` & `not1mm-23.5.9.2/not1mm/data/phonetics/6.wav`

 * *Files identical despite different names*

### Comparing `not1mm-23.5.9.1/not1mm/data/phonetics/7.wav` & `not1mm-23.5.9.2/not1mm/data/phonetics/7.wav`

 * *Files identical despite different names*

### Comparing `not1mm-23.5.9.1/not1mm/data/phonetics/73.wav` & `not1mm-23.5.9.2/not1mm/data/phonetics/73.wav`

 * *Files identical despite different names*

### Comparing `not1mm-23.5.9.1/not1mm/data/phonetics/8.wav` & `not1mm-23.5.9.2/not1mm/data/phonetics/8.wav`

 * *Files identical despite different names*

### Comparing `not1mm-23.5.9.1/not1mm/data/phonetics/9.wav` & `not1mm-23.5.9.2/not1mm/data/phonetics/9.wav`

 * *Files identical despite different names*

### Comparing `not1mm-23.5.9.1/not1mm/data/phonetics/a.wav` & `not1mm-23.5.9.2/not1mm/data/phonetics/a.wav`

 * *Files identical despite different names*

### Comparing `not1mm-23.5.9.1/not1mm/data/phonetics/again.wav` & `not1mm-23.5.9.2/not1mm/data/phonetics/again.wav`

 * *Files identical despite different names*

### Comparing `not1mm-23.5.9.1/not1mm/data/phonetics/b.wav` & `not1mm-23.5.9.2/not1mm/data/phonetics/b.wav`

 * *Files identical despite different names*

### Comparing `not1mm-23.5.9.1/not1mm/data/phonetics/c.wav` & `not1mm-23.5.9.2/not1mm/data/phonetics/c.wav`

 * *Files identical despite different names*

### Comparing `not1mm-23.5.9.1/not1mm/data/phonetics/contest.wav` & `not1mm-23.5.9.2/not1mm/data/phonetics/contest.wav`

 * *Files identical despite different names*

### Comparing `not1mm-23.5.9.1/not1mm/data/phonetics/cq.wav` & `not1mm-23.5.9.2/not1mm/data/phonetics/cq.wav`

 * *Files identical despite different names*

### Comparing `not1mm-23.5.9.1/not1mm/data/phonetics/d.wav` & `not1mm-23.5.9.2/not1mm/data/phonetics/d.wav`

 * *Files identical despite different names*

### Comparing `not1mm-23.5.9.1/not1mm/data/phonetics/e.wav` & `not1mm-23.5.9.2/not1mm/data/phonetics/e.wav`

 * *Files identical despite different names*

### Comparing `not1mm-23.5.9.1/not1mm/data/phonetics/f.wav` & `not1mm-23.5.9.2/not1mm/data/phonetics/f.wav`

 * *Files identical despite different names*

### Comparing `not1mm-23.5.9.1/not1mm/data/phonetics/g.wav` & `not1mm-23.5.9.2/not1mm/data/phonetics/g.wav`

 * *Files identical despite different names*

### Comparing `not1mm-23.5.9.1/not1mm/data/phonetics/h.wav` & `not1mm-23.5.9.2/not1mm/data/phonetics/h.wav`

 * *Files identical despite different names*

### Comparing `not1mm-23.5.9.1/not1mm/data/phonetics/i.wav` & `not1mm-23.5.9.2/not1mm/data/phonetics/i.wav`

 * *Files identical despite different names*

### Comparing `not1mm-23.5.9.1/not1mm/data/phonetics/j.wav` & `not1mm-23.5.9.2/not1mm/data/phonetics/j.wav`

 * *Files identical despite different names*

### Comparing `not1mm-23.5.9.1/not1mm/data/phonetics/k.wav` & `not1mm-23.5.9.2/not1mm/data/phonetics/k.wav`

 * *Files identical despite different names*

### Comparing `not1mm-23.5.9.1/not1mm/data/phonetics/k6gte.wav` & `not1mm-23.5.9.2/not1mm/data/phonetics/k6gte.wav`

 * *Files identical despite different names*

### Comparing `not1mm-23.5.9.1/not1mm/data/phonetics/l.wav` & `not1mm-23.5.9.2/not1mm/data/phonetics/l.wav`

 * *Files identical despite different names*

### Comparing `not1mm-23.5.9.1/not1mm/data/phonetics/m.wav` & `not1mm-23.5.9.2/not1mm/data/phonetics/m.wav`

 * *Files identical despite different names*

### Comparing `not1mm-23.5.9.1/not1mm/data/phonetics/mynumber.wav` & `not1mm-23.5.9.2/not1mm/data/phonetics/mynumber.wav`

 * *Files identical despite different names*

### Comparing `not1mm-23.5.9.1/not1mm/data/phonetics/n.wav` & `not1mm-23.5.9.2/not1mm/data/phonetics/n.wav`

 * *Files identical despite different names*

### Comparing `not1mm-23.5.9.1/not1mm/data/phonetics/nil.wav` & `not1mm-23.5.9.2/not1mm/data/phonetics/nil.wav`

 * *Files identical despite different names*

### Comparing `not1mm-23.5.9.1/not1mm/data/phonetics/o.wav` & `not1mm-23.5.9.2/not1mm/data/phonetics/o.wav`

 * *Files identical despite different names*

### Comparing `not1mm-23.5.9.1/not1mm/data/phonetics/p.wav` & `not1mm-23.5.9.2/not1mm/data/phonetics/p.wav`

 * *Files identical despite different names*

### Comparing `not1mm-23.5.9.1/not1mm/data/phonetics/q.wav` & `not1mm-23.5.9.2/not1mm/data/phonetics/q.wav`

 * *Files identical despite different names*

### Comparing `not1mm-23.5.9.1/not1mm/data/phonetics/r.wav` & `not1mm-23.5.9.2/not1mm/data/phonetics/r.wav`

 * *Files identical despite different names*

### Comparing `not1mm-23.5.9.1/not1mm/data/phonetics/roger.wav` & `not1mm-23.5.9.2/not1mm/data/phonetics/roger.wav`

 * *Files identical despite different names*

### Comparing `not1mm-23.5.9.1/not1mm/data/phonetics/s.wav` & `not1mm-23.5.9.2/not1mm/data/phonetics/s.wav`

 * *Files identical despite different names*

### Comparing `not1mm-23.5.9.1/not1mm/data/phonetics/space.wav` & `not1mm-23.5.9.2/not1mm/data/phonetics/space.wav`

 * *Files identical despite different names*

### Comparing `not1mm-23.5.9.1/not1mm/data/phonetics/t.wav` & `not1mm-23.5.9.2/not1mm/data/phonetics/t.wav`

 * *Files identical despite different names*

### Comparing `not1mm-23.5.9.1/not1mm/data/phonetics/thankyou.wav` & `not1mm-23.5.9.2/not1mm/data/phonetics/thankyou.wav`

 * *Files identical despite different names*

### Comparing `not1mm-23.5.9.1/not1mm/data/phonetics/thankyouqrz.wav` & `not1mm-23.5.9.2/not1mm/data/phonetics/thankyouqrz.wav`

 * *Files identical despite different names*

### Comparing `not1mm-23.5.9.1/not1mm/data/phonetics/u.wav` & `not1mm-23.5.9.2/not1mm/data/phonetics/u.wav`

 * *Files identical despite different names*

### Comparing `not1mm-23.5.9.1/not1mm/data/phonetics/v.wav` & `not1mm-23.5.9.2/not1mm/data/phonetics/v.wav`

 * *Files identical despite different names*

### Comparing `not1mm-23.5.9.1/not1mm/data/phonetics/w.wav` & `not1mm-23.5.9.2/not1mm/data/phonetics/w.wav`

 * *Files identical despite different names*

### Comparing `not1mm-23.5.9.1/not1mm/data/phonetics/x.wav` & `not1mm-23.5.9.2/not1mm/data/phonetics/x.wav`

 * *Files identical despite different names*

### Comparing `not1mm-23.5.9.1/not1mm/data/phonetics/y.wav` & `not1mm-23.5.9.2/not1mm/data/phonetics/y.wav`

 * *Files identical despite different names*

### Comparing `not1mm-23.5.9.1/not1mm/data/phonetics/yourcall.wav` & `not1mm-23.5.9.2/not1mm/data/phonetics/yourcall.wav`

 * *Files identical despite different names*

### Comparing `not1mm-23.5.9.1/not1mm/data/phonetics/z.wav` & `not1mm-23.5.9.2/not1mm/data/phonetics/z.wav`

 * *Files identical despite different names*

### Comparing `not1mm-23.5.9.1/not1mm/data/pickcontest.ui` & `not1mm-23.5.9.2/not1mm/data/pickcontest.ui`

 * *Files identical despite different names*

### Comparing `not1mm-23.5.9.1/not1mm/data/reddot.png` & `not1mm-23.5.9.2/not1mm/data/reddot.png`

 * *Files identical despite different names*

### Comparing `not1mm-23.5.9.1/not1mm/data/settings.ui` & `not1mm-23.5.9.2/not1mm/data/settings.ui`

 * *Files identical despite different names*

### Comparing `not1mm-23.5.9.1/not1mm/lib/cat_interface.py` & `not1mm-23.5.9.2/not1mm/lib/cat_interface.py`

 * *Files identical despite different names*

### Comparing `not1mm-23.5.9.1/not1mm/lib/cwinterface.py` & `not1mm-23.5.9.2/not1mm/lib/cwinterface.py`

 * *Files identical despite different names*

### Comparing `not1mm-23.5.9.1/not1mm/lib/database.py` & `not1mm-23.5.9.2/not1mm/lib/database.py`

 * *Files identical despite different names*

### Comparing `not1mm-23.5.9.1/not1mm/lib/edit_macro.py` & `not1mm-23.5.9.2/not1mm/lib/edit_macro.py`

 * *Files identical despite different names*

### Comparing `not1mm-23.5.9.1/not1mm/lib/edit_station.py` & `not1mm-23.5.9.2/not1mm/lib/edit_station.py`

 * *Files identical despite different names*

### Comparing `not1mm-23.5.9.1/not1mm/lib/ham_utility.py` & `not1mm-23.5.9.2/not1mm/lib/ham_utility.py`

 * *Files identical despite different names*

### Comparing `not1mm-23.5.9.1/not1mm/lib/lookup.py` & `not1mm-23.5.9.2/not1mm/lib/lookup.py`

 * *Files identical despite different names*

### Comparing `not1mm-23.5.9.1/not1mm/lib/multicast.py` & `not1mm-23.5.9.2/not1mm/lib/multicast.py`

 * *Files identical despite different names*

### Comparing `not1mm-23.5.9.1/not1mm/lib/n1mm.py` & `not1mm-23.5.9.2/not1mm/lib/n1mm.py`

 * *Files identical despite different names*

### Comparing `not1mm-23.5.9.1/not1mm/lib/settings.py` & `not1mm-23.5.9.2/not1mm/lib/settings.py`

 * *Files identical despite different names*

### Comparing `not1mm-23.5.9.1/not1mm/logwindow.py` & `not1mm-23.5.9.2/not1mm/logwindow.py`

 * *Files identical despite different names*

### Comparing `not1mm-23.5.9.1/not1mm/plugins/10_10_fall_cw.py` & `not1mm-23.5.9.2/not1mm/plugins/10_10_fall_cw.py`

 * *Files identical despite different names*

### Comparing `not1mm-23.5.9.1/not1mm/plugins/10_10_spring_cw.py` & `not1mm-23.5.9.2/not1mm/plugins/10_10_spring_cw.py`

 * *Files identical despite different names*

### Comparing `not1mm-23.5.9.1/not1mm/plugins/10_10_summer_phone.py` & `not1mm-23.5.9.2/not1mm/plugins/10_10_summer_phone.py`

 * *Files identical despite different names*

### Comparing `not1mm-23.5.9.1/not1mm/plugins/10_10_winter_phone.py` & `not1mm-23.5.9.2/not1mm/plugins/10_10_winter_phone.py`

 * *Files identical despite different names*

### Comparing `not1mm-23.5.9.1/not1mm/plugins/arrl_dx_cw.py` & `not1mm-23.5.9.2/not1mm/plugins/arrl_dx_cw.py`

 * *Files identical despite different names*

### Comparing `not1mm-23.5.9.1/not1mm/plugins/arrl_dx_ssb.py` & `not1mm-23.5.9.2/not1mm/plugins/arrl_dx_ssb.py`

 * *Files identical despite different names*

### Comparing `not1mm-23.5.9.1/not1mm/plugins/arrl_field_day.py` & `not1mm-23.5.9.2/not1mm/plugins/arrl_field_day.py`

 * *Files identical despite different names*

### Comparing `not1mm-23.5.9.1/not1mm/plugins/arrl_rtty_ru.py` & `not1mm-23.5.9.2/not1mm/plugins/arrl_rtty_ru.py`

 * *Files identical despite different names*

### Comparing `not1mm-23.5.9.1/not1mm/plugins/arrl_ss_cw.py` & `not1mm-23.5.9.2/not1mm/plugins/arrl_ss_cw.py`

 * *Files identical despite different names*

### Comparing `not1mm-23.5.9.1/not1mm/plugins/arrl_ss_phone.py` & `not1mm-23.5.9.2/not1mm/plugins/arrl_ss_phone.py`

 * *Files identical despite different names*

### Comparing `not1mm-23.5.9.1/not1mm/plugins/cq_wpx_cw.py` & `not1mm-23.5.9.2/not1mm/plugins/cq_wpx_cw.py`

 * *Files identical despite different names*

### Comparing `not1mm-23.5.9.1/not1mm/plugins/cq_wpx_ssb.py` & `not1mm-23.5.9.2/not1mm/plugins/cq_wpx_ssb.py`

 * *Files identical despite different names*

### Comparing `not1mm-23.5.9.1/not1mm/plugins/cq_ww_cw.py` & `not1mm-23.5.9.2/not1mm/plugins/cq_ww_cw.py`

 * *Files identical despite different names*

### Comparing `not1mm-23.5.9.1/not1mm/plugins/cq_ww_ssb.py` & `not1mm-23.5.9.2/not1mm/plugins/cq_ww_ssb.py`

 * *Files identical despite different names*

### Comparing `not1mm-23.5.9.1/not1mm/plugins/cwt.py` & `not1mm-23.5.9.2/not1mm/plugins/cwt.py`

 * *Files identical despite different names*

### Comparing `not1mm-23.5.9.1/not1mm/plugins/general_logging.py` & `not1mm-23.5.9.2/not1mm/plugins/general_logging.py`

 * *Files identical despite different names*

### Comparing `not1mm-23.5.9.1/not1mm/plugins/jidx_cw.py` & `not1mm-23.5.9.2/not1mm/plugins/jidx_cw.py`

 * *Files identical despite different names*

### Comparing `not1mm-23.5.9.1/not1mm/plugins/jidx_ph.py` & `not1mm-23.5.9.2/not1mm/plugins/jidx_ph.py`

 * *Files identical despite different names*

### Comparing `not1mm-23.5.9.1/not1mm/plugins/winter_field_day.py` & `not1mm-23.5.9.2/not1mm/plugins/winter_field_day.py`

 * *Files identical despite different names*

### Comparing `not1mm-23.5.9.1/not1mm/testing/test.py` & `not1mm-23.5.9.2/not1mm/testing/test.py`

 * *Files identical despite different names*

### Comparing `not1mm-23.5.9.1/not1mm.egg-info/PKG-INFO` & `not1mm-23.5.9.2/not1mm.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: not1mm
-Version: 23.5.9.1
+Version: 23.5.9.2
 Summary: NOT1MM Logger
 Author-email: Michael Bridak <michael.bridak@gmail.com>
 Project-URL: Homepage, https://github.com/mbridak/not1mm
 Project-URL: Bug Tracker, https://github.com/mbridak/not1mm/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: Development Status :: 4 - Beta
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
@@ -63,16 +63,16 @@
     - [Macro use with voice](#macro-use-with-voice)
   - [cty.dat and QRZ lookups for distance and bearing](#ctydat-and-qrz-lookups-for-distance-and-bearing)
   - [Other uses for the call field](#other-uses-for-the-call-field)
   - [Windows](#windows)
     - [The Main Window](#the-main-window)
       - [Keyboard commands](#keyboard-commands)
     - [Log Display](#log-display)
+      - [Editing a contact](#editing-a-contact)
     - [Bandmap](#bandmap)
-  - [Editing a contact](#editing-a-contact)
   - [Recalulate Mults](#recalulate-mults)
   - [Cabrillo](#cabrillo)
   - [ADIF](#adif)
   - [Dupe checking](#dupe-checking)
   - [Contest specific notes](#contest-specific-notes)
     - [ARRL Sweekstakes](#arrl-sweekstakes)
       - [The exchange parser](#the-exchange-parser)
@@ -114,15 +114,15 @@
 - CQ World Wide SSB
 - CWOps CWT
 - Japan International DX CW
 - Japan International DX SSB
 
 ## Changes of note
 
-- [23-5-9] Removed 1 second timers in the bandmap and log window, made them UDP readyRead(). Much smoother. Add CTRL-PgUp and CTRL-PgDown keys to jump to the next/prev spots in the bandmap. Fix: Voice not keying on LSB.
+- [23-5-9] Removed 1 second timers in the bandmap and log window, made them UDP readyRead(). Much smoother. Add CTRL-PgUp and CTRL-PgDown keys to jump to the next/prev spots in the bandmap. Fix: Voice not keying on LSB. Fix: calling pttoff when no CAT interface. Fix: Voice not keying on LSB
 - [23-5-8] Bandmap zoom in/out now centers scale to RX Freq.
 - [23-5-7] Added bandwidth marker to the bandmap.
 - [23-5-6] Added AR Cluster filter options for the bandmap. Added a station ID to the multicast packets. This will prevent erratic bevahiour if 2 stations are on the same network.
 - [23-5-5] Re-wrote most of the log window code. Added ARRL Sweepstakes.
 - [23-5-4] Fixed 'Operators' line in WPX cabrillo file. Fix window title not updating if no CAT control.
 - [23-5-3] Added '#' macro.
 - [23-5-1] Added 10 10 CW and Phone contests. Added a `Cluster` TAB for the AR Cluster server/port in the configuration settings.
@@ -412,36 +412,36 @@
 
 The Log display gets updated automatically when a contact is entered. The top half is a list of all contacts.
 
 ![Log Display Window](https://github.com/mbridak/not1mm/raw/master/pic/logdisplay.png)
 
 The bottom half of the log displays contacts sorted by what's currently in the call entry field. The columns displayed in the log window are dependant on what contests is currently active.
 
-### Bandmap
-
-`Window`>`Bandmap`
-
-Put your callsign in the top and press the connect button.
-
-The bandmap window is, as with everything, a work in progress. The bandmap now follows the VFO. VFO indicator now displays as small triangle in the frequency tickmarks. A small blue rectangle shows the receivers bandwidth. Clicked on spots now tune the radio and set the callsign field.
-
-![Bandmap Window](https://github.com/mbridak/not1mm/raw/master/pic/bandmap.png)
-
-## Editing a contact
+#### Editing a contact
 
 ![Editing a cell](https://github.com/mbridak/not1mm/raw/master/pic/edit_cell.png)
 
 You can double click a cell in the log window and edit its contents.
 
 You can also Right-Click on a cell to bring up the edit dialog.
 
 ![right click edit dialog](https://github.com/mbridak/not1mm/raw/master/pic/edit_dialog.png)
 
 You can not directly edit the multiplier status of a contact. Instead see the next section on recalculating mults. If you change the callsign make sure the `WPX` field is still valid.
 
+### Bandmap
+
+`Window`>`Bandmap`
+
+Put your callsign in the top and press the connect button.
+
+The bandmap window is, as with everything, a work in progress. The bandmap now follows the VFO. VFO indicator now displays as small triangle in the frequency tickmarks. A small blue rectangle shows the receivers bandwidth. Clicked on spots now tune the radio and set the callsign field.
+
+![Bandmap Window](https://github.com/mbridak/not1mm/raw/master/pic/bandmap.png)
+
 ## Recalulate Mults
 
 After editing a contact and before generating a Cabrillo file. There is a Misc menu option that will recalculate the multipliers incase an edit had caused a change.
 
 ## Cabrillo
 
 Click on `File` > `Generate Cabrillo`
```

### Comparing `not1mm-23.5.9.1/not1mm.egg-info/SOURCES.txt` & `not1mm-23.5.9.2/not1mm.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `not1mm-23.5.9.1/pyproject.toml` & `not1mm-23.5.9.2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "not1mm" 
-version = "23.5.9.1"
+version = "23.5.9.2"
 description = "NOT1MM Logger"
 readme = "README.md"
 requires-python = ">=3.9"
 authors = [
   { name="Michael Bridak", email="michael.bridak@gmail.com" },
 ]
 dependencies = [
```

### Comparing `not1mm-23.5.9.1/testing/test.py` & `not1mm-23.5.9.2/testing/test.py`

 * *Files identical despite different names*

