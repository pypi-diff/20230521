# Comparing `tmp/basinmaker-3.0.3a0.tar.gz` & `tmp/basinmaker-3.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "basinmaker-3.0.3a0.tar", last modified: Mon Apr 17 22:51:00 2023, max compression
+gzip compressed data, was "basinmaker-3.1.0.tar", last modified: Sat May 20 23:18:55 2023, max compression
```

## Comparing `basinmaker-3.0.3a0.tar` & `basinmaker-3.1.0.tar`

### file list

```diff
@@ -1,141 +1,144 @@
-drwxrwxrwx   0        0        0        0 2023-04-17 22:51:00.040775 basinmaker-3.0.3a0/
--rw-rw-rw-   0        0        0     8852 2022-07-20 16:58:36.000000 basinmaker-3.0.3a0/LICENSE
--rw-rw-rw-   0        0        0       22 2022-07-20 16:58:36.000000 basinmaker-3.0.3a0/MANIFEST.in
--rw-rw-rw-   0        0        0     5507 2023-04-17 22:51:00.041781 basinmaker-3.0.3a0/PKG-INFO
--rw-rw-rw-   0        0        0     5014 2022-07-20 16:58:36.000000 basinmaker-3.0.3a0/README.md
-drwxrwxrwx   0        0        0        0 2023-04-17 22:50:59.756533 basinmaker-3.0.3a0/basinmaker/
--rw-rw-rw-   0        0        0        0 2022-07-20 16:58:36.000000 basinmaker-3.0.3a0/basinmaker/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-17 22:50:59.802410 basinmaker-3.0.3a0/basinmaker/addattributes/
--rw-rw-rw-   0        0        0        0 2022-08-17 20:01:16.000000 basinmaker-3.0.3a0/basinmaker/addattributes/__init__.py
--rw-rw-rw-   0        0        0    13278 2023-03-04 13:49:59.000000 basinmaker-3.0.3a0/basinmaker/addattributes/addattributestocatchments.py
--rw-rw-rw-   0        0        0     2915 2022-08-17 20:01:16.000000 basinmaker-3.0.3a0/basinmaker/addattributes/addgaugeattributesqgis.py
--rw-rw-rw-   0        0        0     6980 2022-08-17 20:01:16.000000 basinmaker-3.0.3a0/basinmaker/addattributes/addlakeattributesqgis.py
--rw-rw-rw-   0        0        0    12534 2022-12-18 02:16:17.000000 basinmaker-3.0.3a0/basinmaker/addattributes/calbkfwidthdepthqgis.py
--rw-rw-rw-   0        0        0    17015 2022-12-18 02:16:17.000000 basinmaker-3.0.3a0/basinmaker/addattributes/calculatebasicattributesqgis.py
--rw-rw-rw-   0        0        0     3919 2022-08-17 20:01:16.000000 basinmaker-3.0.3a0/basinmaker/addattributes/calfloodmanningnqgis.py
--rw-rw-rw-   0        0        0    21271 2023-04-17 21:45:20.000000 basinmaker-3.0.3a0/basinmaker/addattributes/createattributestemplatearcgis.py
--rw-rw-rw-   0        0        0     1403 2022-08-17 20:01:16.000000 basinmaker-3.0.3a0/basinmaker/addattributes/createattributestemplateqgis.py
--rw-rw-rw-   0        0        0     5634 2023-03-04 13:50:28.000000 basinmaker-3.0.3a0/basinmaker/addattributes/exportoutputsqgis.py
--rw-rw-rw-   0        0        0     2844 2022-08-17 20:01:16.000000 basinmaker-3.0.3a0/basinmaker/addattributes/joinpandastoattributesqgis.py
-drwxrwxrwx   0        0        0        0 2023-04-17 22:50:59.832331 basinmaker-3.0.3a0/basinmaker/addlakeandobs/
--rw-rw-rw-   0        0        0        0 2022-08-17 20:01:16.000000 basinmaker-3.0.3a0/basinmaker/addlakeandobs/__init__.py
--rw-rw-rw-   0        0        0    10672 2022-12-18 02:16:17.000000 basinmaker-3.0.3a0/basinmaker/addlakeandobs/addlakeandobsintowatershed.py
--rw-rw-rw-   0        0        0     7245 2023-03-27 15:33:34.000000 basinmaker-3.0.3a0/basinmaker/addlakeandobs/addlakesarcgis.py
--rw-rw-rw-   0        0        0    14219 2022-12-12 16:45:02.000000 basinmaker-3.0.3a0/basinmaker/addlakeandobs/addlakesqgis.py
--rw-rw-rw-   0        0        0     3984 2023-02-09 00:34:07.000000 basinmaker-3.0.3a0/basinmaker/addlakeandobs/addobsarcgis.py
--rw-rw-rw-   0        0        0     6701 2022-08-17 20:01:16.000000 basinmaker-3.0.3a0/basinmaker/addlakeandobs/addobsqgis.py
--rw-rw-rw-   0        0        0     5535 2022-12-18 02:16:17.000000 basinmaker-3.0.3a0/basinmaker/addlakeandobs/definecatrivarcgis.py
--rw-rw-rw-   0        0        0     6490 2022-12-12 17:39:29.000000 basinmaker-3.0.3a0/basinmaker/addlakeandobs/definecatrivqgis.py
--rw-rw-rw-   0        0        0     1859 2022-08-17 20:01:16.000000 basinmaker-3.0.3a0/basinmaker/addlakeandobs/definelaketypeqgis.py
--rw-rw-rw-   0        0        0     4943 2022-08-17 20:01:16.000000 basinmaker-3.0.3a0/basinmaker/addlakeandobs/filterlakesqgis.py
--rw-rw-rw-   0        0        0    31231 2022-08-17 20:01:16.000000 basinmaker-3.0.3a0/basinmaker/addlakeandobs/modifyfdr.py
--rw-rw-rw-   0        0        0     3281 2022-08-17 20:01:16.000000 basinmaker-3.0.3a0/basinmaker/addlakeandobs/modifystr.py
--rw-rw-rw-   0        0        0    16301 2022-08-17 20:01:16.000000 basinmaker-3.0.3a0/basinmaker/addlakeandobs/pourpointsqgis.py
-drwxrwxrwx   0        0        0        0 2023-04-17 22:50:59.845295 basinmaker-3.0.3a0/basinmaker/arcgisguiwarpper/
--rw-rw-rw-   0        0        0        0 2022-08-17 20:01:16.000000 basinmaker-3.0.3a0/basinmaker/arcgisguiwarpper/__init__.py
--rw-rw-rw-   0        0        0     1826 2022-08-17 20:01:16.000000 basinmaker-3.0.3a0/basinmaker/arcgisguiwarpper/generatehru_arcgis_wrapper.py
--rw-rw-rw-   0        0        0     1141 2022-08-17 20:01:16.000000 basinmaker-3.0.3a0/basinmaker/arcgisguiwarpper/generateraveninput_arcgis_wrapper.py
--rw-rw-rw-   0        0        0     1377 2022-08-17 20:01:16.000000 basinmaker-3.0.3a0/basinmaker/arcgisguiwarpper/selectprod_arcgis_wrapper.py
--rw-rw-rw-   0        0        0      626 2022-08-17 20:01:17.000000 basinmaker-3.0.3a0/basinmaker/arcgisguiwarpper/simplyda_arcgis_wrapper.py
--rw-rw-rw-   0        0        0     1194 2022-08-17 20:01:17.000000 basinmaker-3.0.3a0/basinmaker/arcgisguiwarpper/simplylakes_arcgis_wrapper.py
--rw-rw-rw-   0        0        0    68582 2023-04-17 22:26:13.000000 basinmaker-3.0.3a0/basinmaker/basinmaker.py
-drwxrwxrwx   0        0        0        0 2023-04-17 22:50:59.864244 basinmaker-3.0.3a0/basinmaker/delineationnolake/
--rw-rw-rw-   0        0        0        0 2022-08-17 20:01:17.000000 basinmaker-3.0.3a0/basinmaker/delineationnolake/__init__.py
--rw-rw-rw-   0        0        0     8657 2023-01-03 01:23:58.000000 basinmaker-3.0.3a0/basinmaker/delineationnolake/watdelineationwithoutlake.py
--rw-rw-rw-   0        0        0     3000 2022-08-17 20:01:17.000000 basinmaker-3.0.3a0/basinmaker/delineationnolake/watusingdemarcgis.py
--rw-rw-rw-   0        0        0     2079 2022-08-17 20:01:17.000000 basinmaker-3.0.3a0/basinmaker/delineationnolake/watusingdemqgis.py
--rw-rw-rw-   0        0        0     3018 2022-11-27 20:34:05.000000 basinmaker-3.0.3a0/basinmaker/delineationnolake/watusingfacqgis.py
--rw-rw-rw-   0        0        0     3282 2023-04-02 02:37:44.000000 basinmaker-3.0.3a0/basinmaker/delineationnolake/watusingfdrarcgis.py
--rw-rw-rw-   0        0        0     2915 2023-01-03 01:24:50.000000 basinmaker-3.0.3a0/basinmaker/delineationnolake/watusingfdrqgis.py
--rw-rw-rw-   0        0        0     2339 2022-08-17 20:01:17.000000 basinmaker-3.0.3a0/basinmaker/delineationnolake/watusingsubregionddata.py
-drwxrwxrwx   0        0        0        0 2023-04-17 22:50:59.880202 basinmaker-3.0.3a0/basinmaker/extent/
--rw-rw-rw-   0        0        0        0 2022-08-17 20:01:17.000000 basinmaker-3.0.3a0/basinmaker/extent/__init__.py
--rw-rw-rw-   0        0        0     7764 2022-12-18 02:16:17.000000 basinmaker-3.0.3a0/basinmaker/extent/projectextent.py
--rw-rw-rw-   0        0        0     3492 2022-12-18 02:16:17.000000 basinmaker-3.0.3a0/basinmaker/extent/usingdemarcgis.py
--rw-rw-rw-   0        0        0     4841 2022-12-18 02:16:17.000000 basinmaker-3.0.3a0/basinmaker/extent/usingdemqgis.py
--rw-rw-rw-   0        0        0     4900 2022-08-17 20:01:17.000000 basinmaker-3.0.3a0/basinmaker/extent/usinghybasinplyarcgis.py
--rw-rw-rw-   0        0        0     7193 2022-08-17 20:01:18.000000 basinmaker-3.0.3a0/basinmaker/extent/usinghybasinplyqgis.py
--rw-rw-rw-   0        0        0     6027 2022-08-17 20:01:18.000000 basinmaker-3.0.3a0/basinmaker/extent/usinginputplyqgis.py
--rw-rw-rw-   0        0        0     6861 2022-08-17 20:01:18.000000 basinmaker-3.0.3a0/basinmaker/extent/usingoutletpointqgis.py
-drwxrwxrwx   0        0        0        0 2023-04-17 22:50:59.901145 basinmaker-3.0.3a0/basinmaker/func/
--rw-rw-rw-   0        0        0        0 2022-08-17 20:01:18.000000 basinmaker-3.0.3a0/basinmaker/func/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-17 22:50:59.925083 basinmaker-3.0.3a0/basinmaker/func/__pycache__/
--rw-rw-rw-   0        0        0      164 2022-08-17 20:03:20.000000 basinmaker-3.0.3a0/basinmaker/func/__pycache__/__init__.cpython-39.pyc
--rw-rw-rw-   0        0        0    18510 2023-02-27 03:41:01.000000 basinmaker-3.0.3a0/basinmaker/func/__pycache__/arcgis.cpython-39.pyc
--rw-rw-rw-   0        0        0     6084 2022-08-17 20:05:59.000000 basinmaker-3.0.3a0/basinmaker/func/__pycache__/fgdal.cpython-39.pyc
--rw-rw-rw-   0        0        0    15904 2022-08-18 02:30:26.000000 basinmaker-3.0.3a0/basinmaker/func/__pycache__/grassgis.cpython-39.pyc
--rw-rw-rw-   0        0        0    47805 2023-04-01 13:38:31.000000 basinmaker-3.0.3a0/basinmaker/func/__pycache__/pdtable.cpython-39.pyc
--rw-rw-rw-   0        0        0    10323 2023-04-16 18:06:34.000000 basinmaker-3.0.3a0/basinmaker/func/__pycache__/purepy.cpython-39.pyc
--rw-rw-rw-   0        0        0    26797 2022-08-18 02:30:27.000000 basinmaker-3.0.3a0/basinmaker/func/__pycache__/qgis.cpython-39.pyc
--rw-rw-rw-   0        0        0    12224 2022-08-18 02:30:32.000000 basinmaker-3.0.3a0/basinmaker/func/__pycache__/rarray.cpython-39.pyc
--rw-rw-rw-   0        0        0    35090 2023-02-27 03:39:45.000000 basinmaker-3.0.3a0/basinmaker/func/arcgis.py
--rw-rw-rw-   0        0        0     9448 2022-08-17 20:01:18.000000 basinmaker-3.0.3a0/basinmaker/func/fgdal.py
--rw-rw-rw-   0        0        0    27465 2022-08-17 20:01:18.000000 basinmaker-3.0.3a0/basinmaker/func/grassgis.py
--rw-rw-rw-   0        0        0   139946 2023-04-01 13:38:19.000000 basinmaker-3.0.3a0/basinmaker/func/pdtable.py
--rw-rw-rw-   0        0        0    17567 2023-04-10 21:29:09.000000 basinmaker-3.0.3a0/basinmaker/func/purepy.py
--rw-rw-rw-   0        0        0    42623 2022-08-17 20:01:18.000000 basinmaker-3.0.3a0/basinmaker/func/qgis.py
--rw-rw-rw-   0        0        0    25878 2022-08-17 20:01:18.000000 basinmaker-3.0.3a0/basinmaker/func/rarray.py
-drwxrwxrwx   0        0        0        0 2023-04-17 22:50:59.930074 basinmaker-3.0.3a0/basinmaker/hymodin/
--rw-rw-rw-   0        0        0        0 2022-08-17 20:01:18.000000 basinmaker-3.0.3a0/basinmaker/hymodin/__init__.py
--rw-rw-rw-   0        0        0    92339 2022-11-17 01:32:01.000000 basinmaker-3.0.3a0/basinmaker/hymodin/raveninput.py
-drwxrwxrwx   0        0        0        0 2023-04-17 22:50:59.983925 basinmaker-3.0.3a0/basinmaker/postprocessing/
--rw-rw-rw-   0        0        0        0 2022-08-17 20:01:18.000000 basinmaker-3.0.3a0/basinmaker/postprocessing/__init__.py
--rw-rw-rw-   0        0        0    10250 2023-04-01 13:38:13.000000 basinmaker-3.0.3a0/basinmaker/postprocessing/assigninterestsites.py
--rw-rw-rw-   0        0        0     6500 2023-03-04 13:51:54.000000 basinmaker-3.0.3a0/basinmaker/postprocessing/combine.py
--rw-rw-rw-   0        0        0     6538 2023-03-04 13:52:08.000000 basinmaker-3.0.3a0/basinmaker/postprocessing/combinearcgis.py
--rw-rw-rw-   0        0        0     5693 2023-03-04 13:52:19.000000 basinmaker-3.0.3a0/basinmaker/postprocessing/combinepurepy.py
--rw-rw-rw-   0        0        0     7412 2023-04-01 14:30:36.000000 basinmaker-3.0.3a0/basinmaker/postprocessing/downloadpd.py
--rw-rw-rw-   0        0        0     2836 2022-08-17 20:01:18.000000 basinmaker-3.0.3a0/basinmaker/postprocessing/downloadpdptspurepy.py
--rw-rw-rw-   0        0        0    21586 2022-08-17 20:01:18.000000 basinmaker-3.0.3a0/basinmaker/postprocessing/gridweight.py
--rw-rw-rw-   0        0        0     3482 2022-08-17 20:01:18.000000 basinmaker-3.0.3a0/basinmaker/postprocessing/gridweightarcgis.py
--rw-rw-rw-   0        0        0    59494 2022-08-17 20:01:18.000000 basinmaker-3.0.3a0/basinmaker/postprocessing/hru.py
--rw-rw-rw-   0        0        0    40585 2022-09-07 02:20:09.000000 basinmaker-3.0.3a0/basinmaker/postprocessing/hruarcgis.py
--rw-rw-rw-   0        0        0    38578 2022-11-27 18:54:39.000000 basinmaker-3.0.3a0/basinmaker/postprocessing/hrupurepy.py
--rw-rw-rw-   0        0        0    10971 2023-03-04 13:53:00.000000 basinmaker-3.0.3a0/basinmaker/postprocessing/increaseda.py
--rw-rw-rw-   0        0        0     9072 2023-03-04 14:14:28.000000 basinmaker-3.0.3a0/basinmaker/postprocessing/increasedaarcgis.py
--rw-rw-rw-   0        0        0     8693 2023-03-04 13:53:46.000000 basinmaker-3.0.3a0/basinmaker/postprocessing/increasedapurepy.py
--rw-rw-rw-   0        0        0     3303 2022-09-11 18:50:03.000000 basinmaker-3.0.3a0/basinmaker/postprocessing/inversetopology.py
--rw-rw-rw-   0        0        0     8035 2023-04-01 13:38:19.000000 basinmaker-3.0.3a0/basinmaker/postprocessing/plotleaflet.py
--rw-rw-rw-   0        0        0    15290 2023-02-05 00:48:12.000000 basinmaker-3.0.3a0/basinmaker/postprocessing/postprocessingfunctions.py
--rw-rw-rw-   0        0        0    10902 2023-03-04 14:03:13.000000 basinmaker-3.0.3a0/basinmaker/postprocessing/selectlake.py
--rw-rw-rw-   0        0        0     8912 2023-03-04 14:08:34.000000 basinmaker-3.0.3a0/basinmaker/postprocessing/selectlakearcgis.py
--rw-rw-rw-   0        0        0     8114 2023-03-04 14:09:00.000000 basinmaker-3.0.3a0/basinmaker/postprocessing/selectlakepurepy.py
--rw-rw-rw-   0        0        0    11957 2023-03-04 14:09:12.000000 basinmaker-3.0.3a0/basinmaker/postprocessing/selectprod.py
--rw-rw-rw-   0        0        0    11211 2023-03-04 14:09:22.000000 basinmaker-3.0.3a0/basinmaker/postprocessing/selectprodarcgis.py
--rw-rw-rw-   0        0        0     7266 2023-04-01 13:38:19.000000 basinmaker-3.0.3a0/basinmaker/postprocessing/selectprodpurepy.py
-drwxrwxrwx   0        0        0        0 2023-04-17 22:50:59.997888 basinmaker-3.0.3a0/basinmaker/preprocessing/
--rw-rw-rw-   0        0        0        0 2022-08-17 20:01:19.000000 basinmaker-3.0.3a0/basinmaker/preprocessing/__init__.py
--rw-rw-rw-   0        0        0     1180 2022-08-17 20:01:19.000000 basinmaker-3.0.3a0/basinmaker/preprocessing/preinputpolygonqgis.py
--rw-rw-rw-   0        0        0     3446 2022-08-17 20:01:19.000000 basinmaker-3.0.3a0/basinmaker/preprocessing/preprocessinglakeply.py
--rw-rw-rw-   0        0        0     1363 2022-08-17 20:01:19.000000 basinmaker-3.0.3a0/basinmaker/preprocessing/preprocessingobs.py
--rw-rw-rw-   0        0        0     2665 2022-08-17 20:01:19.000000 basinmaker-3.0.3a0/basinmaker/preprocessing/preprocessrasterqgis.py
--rw-rw-rw-   0        0        0     4187 2022-08-17 20:01:19.000000 basinmaker-3.0.3a0/basinmaker/preprocessing/rasterizevectorsandloadtodbqgis.py
--rw-rw-rw-   0        0        0     3610 2022-08-17 20:01:19.000000 basinmaker-3.0.3a0/basinmaker/preprocessing/reprojectandclipvectorbyplyqgis.py
-drwxrwxrwx   0        0        0        0 2023-04-17 22:51:00.002875 basinmaker-3.0.3a0/basinmaker/subreg/
--rw-rw-rw-   0        0        0        0 2022-08-17 20:01:19.000000 basinmaker-3.0.3a0/basinmaker/subreg/__init__.py
--rw-rw-rw-   0        0        0     3612 2022-08-17 20:01:19.000000 basinmaker-3.0.3a0/basinmaker/subreg/defsubreg.py
--rw-rw-rw-   0        0        0    38989 2022-11-23 01:59:53.000000 basinmaker-3.0.3a0/basinmaker/subreg/generatesubregionqgis.py
-drwxrwxrwx   0        0        0        0 2023-04-17 22:51:00.007861 basinmaker-3.0.3a0/basinmaker/utilities/
--rw-rw-rw-   0        0        0        0 2022-08-17 20:01:19.000000 basinmaker-3.0.3a0/basinmaker/utilities/__init__.py
--rw-rw-rw-   0        0        0     7554 2022-11-27 20:24:39.000000 basinmaker-3.0.3a0/basinmaker/utilities/utilities.py
-drwxrwxrwx   0        0        0        0 2023-04-17 22:50:59.773491 basinmaker-3.0.3a0/basinmaker.egg-info/
--rw-rw-rw-   0        0        0     5507 2023-04-17 22:50:59.000000 basinmaker-3.0.3a0/basinmaker.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     5345 2023-04-17 22:50:59.000000 basinmaker-3.0.3a0/basinmaker.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-17 22:50:59.000000 basinmaker-3.0.3a0/basinmaker.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       11 2023-04-17 22:50:59.000000 basinmaker-3.0.3a0/basinmaker.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      108 2022-07-20 16:58:37.000000 basinmaker-3.0.3a0/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-04-17 22:51:00.044761 basinmaker-3.0.3a0/setup.cfg
--rw-rw-rw-   0        0        0      829 2023-04-17 22:49:07.000000 basinmaker-3.0.3a0/setup.py
-drwxrwxrwx   0        0        0        0 2023-04-17 22:51:00.038778 basinmaker-3.0.3a0/tests/
--rw-rw-rw-   0        0        0     5251 2022-07-20 16:58:37.000000 basinmaker-3.0.3a0/tests/test_RoutingTool_AutomatedWatershedsandLakesFilterToolset.py
--rw-rw-rw-   0        0        0     6085 2022-07-20 16:58:37.000000 basinmaker-3.0.3a0/tests/test_RoutingTool_Generateinputdata.py
--rw-rw-rw-   0        0        0     6187 2022-07-20 16:58:37.000000 basinmaker-3.0.3a0/tests/test_RoutingTool_Generatmaskregion.py
--rw-rw-rw-   0        0        0     5729 2022-07-20 16:58:37.000000 basinmaker-3.0.3a0/tests/test_RoutingTool_PostProcessing_Customize_Routing_Topology.py
--rw-rw-rw-   0        0        0     2298 2022-07-20 16:58:37.000000 basinmaker-3.0.3a0/tests/test_RoutingTool_PostProcessing_Define_Final_Catchment.py
--rw-rw-rw-   0        0        0     3378 2022-07-20 16:58:37.000000 basinmaker-3.0.3a0/tests/test_RoutingTool_PostProcessing_GenerateHRUS.py
--rw-rw-rw-   0        0        0     3474 2022-07-20 16:58:37.000000 basinmaker-3.0.3a0/tests/test_RoutingTool_PostProcessing_GenerateRavenInput.py
--rw-rw-rw-   0        0        0     1966 2022-07-20 16:58:37.000000 basinmaker-3.0.3a0/tests/test_RoutingTool_PostProcessing_Locate_subid_needsbyuser.py
--rw-rw-rw-   0        0        0     4695 2022-07-20 16:58:37.000000 basinmaker-3.0.3a0/tests/test_RoutingTool_PostProcessing_SelectLakes.py
--rw-rw-rw-   0        0        0     7034 2022-07-20 16:58:37.000000 basinmaker-3.0.3a0/tests/test_RoutingTool_PostProcessing_Select_Routing_product_based_SubId.py
--rw-rw-rw-   0        0        0     5916 2022-07-20 16:58:37.000000 basinmaker-3.0.3a0/tests/test_RoutingTool_RoutingNetworkTopologyUpdateToolset_riv.py
--rw-rw-rw-   0        0        0     6998 2022-07-20 16:58:37.000000 basinmaker-3.0.3a0/tests/test_RoutingTool_WatershedDiscretizationToolset.py
+drwxrwxrwx   0        0        0        0 2023-05-20 23:18:55.709609 basinmaker-3.1.0/
+-rw-rw-rw-   0        0        0     8852 2022-07-20 16:58:36.000000 basinmaker-3.1.0/LICENSE
+-rw-rw-rw-   0        0        0       22 2022-07-20 16:58:36.000000 basinmaker-3.1.0/MANIFEST.in
+-rw-rw-rw-   0        0        0     5505 2023-05-20 23:18:55.710607 basinmaker-3.1.0/PKG-INFO
+-rw-rw-rw-   0        0        0     5014 2022-07-20 16:58:36.000000 basinmaker-3.1.0/README.md
+drwxrwxrwx   0        0        0        0 2023-05-20 23:18:55.420865 basinmaker-3.1.0/basinmaker/
+-rw-rw-rw-   0        0        0        0 2022-07-20 16:58:36.000000 basinmaker-3.1.0/basinmaker/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-20 23:18:55.473722 basinmaker-3.1.0/basinmaker/addattributes/
+-rw-rw-rw-   0        0        0        0 2022-08-17 20:01:16.000000 basinmaker-3.1.0/basinmaker/addattributes/__init__.py
+-rw-rw-rw-   0        0        0    13278 2023-03-04 13:49:59.000000 basinmaker-3.1.0/basinmaker/addattributes/addattributestocatchments.py
+-rw-rw-rw-   0        0        0     2915 2022-08-17 20:01:16.000000 basinmaker-3.1.0/basinmaker/addattributes/addgaugeattributesqgis.py
+-rw-rw-rw-   0        0        0     6980 2022-08-17 20:01:16.000000 basinmaker-3.1.0/basinmaker/addattributes/addlakeattributesqgis.py
+-rw-rw-rw-   0        0        0    12534 2022-12-18 02:16:17.000000 basinmaker-3.1.0/basinmaker/addattributes/calbkfwidthdepthqgis.py
+-rw-rw-rw-   0        0        0    17015 2022-12-18 02:16:17.000000 basinmaker-3.1.0/basinmaker/addattributes/calculatebasicattributesqgis.py
+-rw-rw-rw-   0        0        0     3919 2022-08-17 20:01:16.000000 basinmaker-3.1.0/basinmaker/addattributes/calfloodmanningnqgis.py
+-rw-rw-rw-   0        0        0    24582 2023-05-19 01:38:46.000000 basinmaker-3.1.0/basinmaker/addattributes/createattributestemplatearcgis.py
+-rw-rw-rw-   0        0        0     1403 2022-08-17 20:01:16.000000 basinmaker-3.1.0/basinmaker/addattributes/createattributestemplateqgis.py
+-rw-rw-rw-   0        0        0     5634 2023-03-04 13:50:28.000000 basinmaker-3.1.0/basinmaker/addattributes/exportoutputsqgis.py
+-rw-rw-rw-   0        0        0     2844 2022-08-17 20:01:16.000000 basinmaker-3.1.0/basinmaker/addattributes/joinpandastoattributesqgis.py
+drwxrwxrwx   0        0        0        0 2023-05-20 23:18:55.502650 basinmaker-3.1.0/basinmaker/addlakeandobs/
+-rw-rw-rw-   0        0        0        0 2022-08-17 20:01:16.000000 basinmaker-3.1.0/basinmaker/addlakeandobs/__init__.py
+-rw-rw-rw-   0        0        0    10672 2022-12-18 02:16:17.000000 basinmaker-3.1.0/basinmaker/addlakeandobs/addlakeandobsintowatershed.py
+-rw-rw-rw-   0        0        0     7245 2023-03-27 15:33:34.000000 basinmaker-3.1.0/basinmaker/addlakeandobs/addlakesarcgis.py
+-rw-rw-rw-   0        0        0    14219 2022-12-12 16:45:02.000000 basinmaker-3.1.0/basinmaker/addlakeandobs/addlakesqgis.py
+-rw-rw-rw-   0        0        0     3984 2023-02-09 00:34:07.000000 basinmaker-3.1.0/basinmaker/addlakeandobs/addobsarcgis.py
+-rw-rw-rw-   0        0        0     6701 2022-08-17 20:01:16.000000 basinmaker-3.1.0/basinmaker/addlakeandobs/addobsqgis.py
+-rw-rw-rw-   0        0        0     5535 2022-12-18 02:16:17.000000 basinmaker-3.1.0/basinmaker/addlakeandobs/definecatrivarcgis.py
+-rw-rw-rw-   0        0        0     6490 2022-12-12 17:39:29.000000 basinmaker-3.1.0/basinmaker/addlakeandobs/definecatrivqgis.py
+-rw-rw-rw-   0        0        0     1859 2022-08-17 20:01:16.000000 basinmaker-3.1.0/basinmaker/addlakeandobs/definelaketypeqgis.py
+-rw-rw-rw-   0        0        0     4943 2022-08-17 20:01:16.000000 basinmaker-3.1.0/basinmaker/addlakeandobs/filterlakesqgis.py
+-rw-rw-rw-   0        0        0    31231 2022-08-17 20:01:16.000000 basinmaker-3.1.0/basinmaker/addlakeandobs/modifyfdr.py
+-rw-rw-rw-   0        0        0     3281 2022-08-17 20:01:16.000000 basinmaker-3.1.0/basinmaker/addlakeandobs/modifystr.py
+-rw-rw-rw-   0        0        0    16301 2022-08-17 20:01:16.000000 basinmaker-3.1.0/basinmaker/addlakeandobs/pourpointsqgis.py
+drwxrwxrwx   0        0        0        0 2023-05-20 23:18:55.517604 basinmaker-3.1.0/basinmaker/arcgisguiwarpper/
+-rw-rw-rw-   0        0        0        0 2022-08-17 20:01:16.000000 basinmaker-3.1.0/basinmaker/arcgisguiwarpper/__init__.py
+-rw-rw-rw-   0        0        0     1826 2022-08-17 20:01:16.000000 basinmaker-3.1.0/basinmaker/arcgisguiwarpper/generatehru_arcgis_wrapper.py
+-rw-rw-rw-   0        0        0     1141 2022-08-17 20:01:16.000000 basinmaker-3.1.0/basinmaker/arcgisguiwarpper/generateraveninput_arcgis_wrapper.py
+-rw-rw-rw-   0        0        0     1377 2022-08-17 20:01:16.000000 basinmaker-3.1.0/basinmaker/arcgisguiwarpper/selectprod_arcgis_wrapper.py
+-rw-rw-rw-   0        0        0      626 2022-08-17 20:01:17.000000 basinmaker-3.1.0/basinmaker/arcgisguiwarpper/simplyda_arcgis_wrapper.py
+-rw-rw-rw-   0        0        0     1194 2022-08-17 20:01:17.000000 basinmaker-3.1.0/basinmaker/arcgisguiwarpper/simplylakes_arcgis_wrapper.py
+-rw-rw-rw-   0        0        0    70144 2023-05-19 01:38:46.000000 basinmaker-3.1.0/basinmaker/basinmaker.py
+drwxrwxrwx   0        0        0        0 2023-05-20 23:18:55.534561 basinmaker-3.1.0/basinmaker/delineationnolake/
+-rw-rw-rw-   0        0        0        0 2022-08-17 20:01:17.000000 basinmaker-3.1.0/basinmaker/delineationnolake/__init__.py
+-rw-rw-rw-   0        0        0     8657 2023-01-03 01:23:58.000000 basinmaker-3.1.0/basinmaker/delineationnolake/watdelineationwithoutlake.py
+-rw-rw-rw-   0        0        0     3000 2022-08-17 20:01:17.000000 basinmaker-3.1.0/basinmaker/delineationnolake/watusingdemarcgis.py
+-rw-rw-rw-   0        0        0     2079 2022-08-17 20:01:17.000000 basinmaker-3.1.0/basinmaker/delineationnolake/watusingdemqgis.py
+-rw-rw-rw-   0        0        0     3018 2022-11-27 20:34:05.000000 basinmaker-3.1.0/basinmaker/delineationnolake/watusingfacqgis.py
+-rw-rw-rw-   0        0        0     3431 2023-05-16 23:13:55.000000 basinmaker-3.1.0/basinmaker/delineationnolake/watusingfdrarcgis.py
+-rw-rw-rw-   0        0        0     2915 2023-01-03 01:24:50.000000 basinmaker-3.1.0/basinmaker/delineationnolake/watusingfdrqgis.py
+-rw-rw-rw-   0        0        0     2339 2022-08-17 20:01:17.000000 basinmaker-3.1.0/basinmaker/delineationnolake/watusingsubregionddata.py
+drwxrwxrwx   0        0        0        0 2023-05-20 23:18:55.553511 basinmaker-3.1.0/basinmaker/extent/
+-rw-rw-rw-   0        0        0        0 2022-08-17 20:01:17.000000 basinmaker-3.1.0/basinmaker/extent/__init__.py
+-rw-rw-rw-   0        0        0     7764 2022-12-18 02:16:17.000000 basinmaker-3.1.0/basinmaker/extent/projectextent.py
+-rw-rw-rw-   0        0        0     3492 2022-12-18 02:16:17.000000 basinmaker-3.1.0/basinmaker/extent/usingdemarcgis.py
+-rw-rw-rw-   0        0        0     4841 2022-12-18 02:16:17.000000 basinmaker-3.1.0/basinmaker/extent/usingdemqgis.py
+-rw-rw-rw-   0        0        0     4900 2022-08-17 20:01:17.000000 basinmaker-3.1.0/basinmaker/extent/usinghybasinplyarcgis.py
+-rw-rw-rw-   0        0        0     7193 2022-08-17 20:01:18.000000 basinmaker-3.1.0/basinmaker/extent/usinghybasinplyqgis.py
+-rw-rw-rw-   0        0        0     6027 2022-08-17 20:01:18.000000 basinmaker-3.1.0/basinmaker/extent/usinginputplyqgis.py
+-rw-rw-rw-   0        0        0     6861 2022-08-17 20:01:18.000000 basinmaker-3.1.0/basinmaker/extent/usingoutletpointqgis.py
+drwxrwxrwx   0        0        0        0 2023-05-20 23:18:55.558635 basinmaker-3.1.0/basinmaker/func/
+-rw-rw-rw-   0        0        0        0 2022-08-17 20:01:18.000000 basinmaker-3.1.0/basinmaker/func/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-20 23:18:55.596913 basinmaker-3.1.0/basinmaker/func/__pycache__/
+-rw-rw-rw-   0        0        0      182 2023-05-19 01:19:58.000000 basinmaker-3.1.0/basinmaker/func/__pycache__/__init__.cpython-311.pyc
+-rw-rw-rw-   0        0        0      164 2022-08-17 20:03:20.000000 basinmaker-3.1.0/basinmaker/func/__pycache__/__init__.cpython-39.pyc
+-rw-rw-rw-   0        0        0    18805 2023-05-19 01:39:54.000000 basinmaker-3.1.0/basinmaker/func/__pycache__/arcgis.cpython-39.pyc
+-rw-rw-rw-   0        0        0     6084 2022-08-17 20:05:59.000000 basinmaker-3.1.0/basinmaker/func/__pycache__/fgdal.cpython-39.pyc
+-rw-rw-rw-   0        0        0    15904 2022-08-18 02:30:26.000000 basinmaker-3.1.0/basinmaker/func/__pycache__/grassgis.cpython-39.pyc
+-rw-rw-rw-   0        0        0   119683 2023-05-19 01:39:22.000000 basinmaker-3.1.0/basinmaker/func/__pycache__/pdtable.cpython-311.pyc
+-rw-rw-rw-   0        0        0    50497 2023-05-19 01:40:07.000000 basinmaker-3.1.0/basinmaker/func/__pycache__/pdtable.cpython-39.pyc
+-rw-rw-rw-   0        0        0    23556 2023-05-19 01:39:22.000000 basinmaker-3.1.0/basinmaker/func/__pycache__/purepy.cpython-311.pyc
+-rw-rw-rw-   0        0        0    11733 2023-05-20 00:54:02.000000 basinmaker-3.1.0/basinmaker/func/__pycache__/purepy.cpython-39.pyc
+-rw-rw-rw-   0        0        0    26797 2022-08-18 02:30:27.000000 basinmaker-3.1.0/basinmaker/func/__pycache__/qgis.cpython-39.pyc
+-rw-rw-rw-   0        0        0    12224 2022-08-18 02:30:32.000000 basinmaker-3.1.0/basinmaker/func/__pycache__/rarray.cpython-39.pyc
+-rw-rw-rw-   0        0        0    36287 2023-05-19 01:38:46.000000 basinmaker-3.1.0/basinmaker/func/arcgis.py
+-rw-rw-rw-   0        0        0     9448 2022-08-17 20:01:18.000000 basinmaker-3.1.0/basinmaker/func/fgdal.py
+-rw-rw-rw-   0        0        0    27465 2022-08-17 20:01:18.000000 basinmaker-3.1.0/basinmaker/func/grassgis.py
+-rw-rw-rw-   0        0        0   152240 2023-05-19 01:38:46.000000 basinmaker-3.1.0/basinmaker/func/pdtable.py
+-rw-rw-rw-   0        0        0    21348 2023-05-20 00:52:31.000000 basinmaker-3.1.0/basinmaker/func/purepy.py
+-rw-rw-rw-   0        0        0    42623 2022-08-17 20:01:18.000000 basinmaker-3.1.0/basinmaker/func/qgis.py
+-rw-rw-rw-   0        0        0    25878 2022-08-17 20:01:18.000000 basinmaker-3.1.0/basinmaker/func/rarray.py
+drwxrwxrwx   0        0        0        0 2023-05-20 23:18:55.599903 basinmaker-3.1.0/basinmaker/hymodin/
+-rw-rw-rw-   0        0        0        0 2022-08-17 20:01:18.000000 basinmaker-3.1.0/basinmaker/hymodin/__init__.py
+-rw-rw-rw-   0        0        0    92339 2022-11-17 01:32:01.000000 basinmaker-3.1.0/basinmaker/hymodin/raveninput.py
+drwxrwxrwx   0        0        0        0 2023-05-20 23:18:55.655753 basinmaker-3.1.0/basinmaker/postprocessing/
+-rw-rw-rw-   0        0        0        0 2022-08-17 20:01:18.000000 basinmaker-3.1.0/basinmaker/postprocessing/__init__.py
+-rw-rw-rw-   0        0        0    13196 2023-05-19 01:38:46.000000 basinmaker-3.1.0/basinmaker/postprocessing/assigninterestsites.py
+-rw-rw-rw-   0        0        0     6500 2023-03-04 13:51:54.000000 basinmaker-3.1.0/basinmaker/postprocessing/combine.py
+-rw-rw-rw-   0        0        0     6538 2023-03-04 13:52:08.000000 basinmaker-3.1.0/basinmaker/postprocessing/combinearcgis.py
+-rw-rw-rw-   0        0        0     6061 2023-05-19 01:38:46.000000 basinmaker-3.1.0/basinmaker/postprocessing/combinepurepy.py
+-rw-rw-rw-   0        0        0     7548 2023-05-16 23:13:55.000000 basinmaker-3.1.0/basinmaker/postprocessing/downloadpd.py
+-rw-rw-rw-   0        0        0     2836 2022-08-17 20:01:18.000000 basinmaker-3.1.0/basinmaker/postprocessing/downloadpdptspurepy.py
+-rw-rw-rw-   0        0        0    21586 2022-08-17 20:01:18.000000 basinmaker-3.1.0/basinmaker/postprocessing/gridweight.py
+-rw-rw-rw-   0        0        0     3482 2022-08-17 20:01:18.000000 basinmaker-3.1.0/basinmaker/postprocessing/gridweightarcgis.py
+-rw-rw-rw-   0        0        0    59494 2022-08-17 20:01:18.000000 basinmaker-3.1.0/basinmaker/postprocessing/hru.py
+-rw-rw-rw-   0        0        0    40585 2022-09-07 02:20:09.000000 basinmaker-3.1.0/basinmaker/postprocessing/hruarcgis.py
+-rw-rw-rw-   0        0        0    38641 2023-05-19 01:38:46.000000 basinmaker-3.1.0/basinmaker/postprocessing/hrupurepy.py
+-rw-rw-rw-   0        0        0    10971 2023-03-04 13:53:00.000000 basinmaker-3.1.0/basinmaker/postprocessing/increaseda.py
+-rw-rw-rw-   0        0        0     9072 2023-03-04 14:14:28.000000 basinmaker-3.1.0/basinmaker/postprocessing/increasedaarcgis.py
+-rw-rw-rw-   0        0        0     9104 2023-05-19 01:38:46.000000 basinmaker-3.1.0/basinmaker/postprocessing/increasedapurepy.py
+-rw-rw-rw-   0        0        0     3303 2022-09-11 18:50:03.000000 basinmaker-3.1.0/basinmaker/postprocessing/inversetopology.py
+-rw-rw-rw-   0        0        0     8035 2023-04-01 13:38:19.000000 basinmaker-3.1.0/basinmaker/postprocessing/plotleaflet.py
+-rw-rw-rw-   0        0        0    15295 2023-05-19 01:38:46.000000 basinmaker-3.1.0/basinmaker/postprocessing/postprocessingfunctions.py
+-rw-rw-rw-   0        0        0    10902 2023-03-04 14:03:13.000000 basinmaker-3.1.0/basinmaker/postprocessing/selectlake.py
+-rw-rw-rw-   0        0        0     8912 2023-03-04 14:08:34.000000 basinmaker-3.1.0/basinmaker/postprocessing/selectlakearcgis.py
+-rw-rw-rw-   0        0        0     8114 2023-03-04 14:09:00.000000 basinmaker-3.1.0/basinmaker/postprocessing/selectlakepurepy.py
+-rw-rw-rw-   0        0        0    11957 2023-03-04 14:09:12.000000 basinmaker-3.1.0/basinmaker/postprocessing/selectprod.py
+-rw-rw-rw-   0        0        0    11211 2023-03-04 14:09:22.000000 basinmaker-3.1.0/basinmaker/postprocessing/selectprodarcgis.py
+-rw-rw-rw-   0        0        0     7266 2023-04-01 13:38:19.000000 basinmaker-3.1.0/basinmaker/postprocessing/selectprodpurepy.py
+drwxrwxrwx   0        0        0        0 2023-05-20 23:18:55.669716 basinmaker-3.1.0/basinmaker/preprocessing/
+-rw-rw-rw-   0        0        0        0 2022-08-17 20:01:19.000000 basinmaker-3.1.0/basinmaker/preprocessing/__init__.py
+-rw-rw-rw-   0        0        0     1180 2022-08-17 20:01:19.000000 basinmaker-3.1.0/basinmaker/preprocessing/preinputpolygonqgis.py
+-rw-rw-rw-   0        0        0     3446 2022-08-17 20:01:19.000000 basinmaker-3.1.0/basinmaker/preprocessing/preprocessinglakeply.py
+-rw-rw-rw-   0        0        0     1363 2022-08-17 20:01:19.000000 basinmaker-3.1.0/basinmaker/preprocessing/preprocessingobs.py
+-rw-rw-rw-   0        0        0     2665 2022-08-17 20:01:19.000000 basinmaker-3.1.0/basinmaker/preprocessing/preprocessrasterqgis.py
+-rw-rw-rw-   0        0        0     4187 2022-08-17 20:01:19.000000 basinmaker-3.1.0/basinmaker/preprocessing/rasterizevectorsandloadtodbqgis.py
+-rw-rw-rw-   0        0        0     3610 2022-08-17 20:01:19.000000 basinmaker-3.1.0/basinmaker/preprocessing/reprojectandclipvectorbyplyqgis.py
+drwxrwxrwx   0        0        0        0 2023-05-20 23:18:55.675700 basinmaker-3.1.0/basinmaker/subreg/
+-rw-rw-rw-   0        0        0        0 2022-08-17 20:01:19.000000 basinmaker-3.1.0/basinmaker/subreg/__init__.py
+-rw-rw-rw-   0        0        0     3612 2022-08-17 20:01:19.000000 basinmaker-3.1.0/basinmaker/subreg/defsubreg.py
+-rw-rw-rw-   0        0        0    38989 2022-11-23 01:59:53.000000 basinmaker-3.1.0/basinmaker/subreg/generatesubregionqgis.py
+drwxrwxrwx   0        0        0        0 2023-05-20 23:18:55.679690 basinmaker-3.1.0/basinmaker/utilities/
+-rw-rw-rw-   0        0        0        0 2022-08-17 20:01:19.000000 basinmaker-3.1.0/basinmaker/utilities/__init__.py
+-rw-rw-rw-   0        0        0     8012 2023-05-19 01:38:46.000000 basinmaker-3.1.0/basinmaker/utilities/utilities.py
+drwxrwxrwx   0        0        0        0 2023-05-20 23:18:55.447792 basinmaker-3.1.0/basinmaker.egg-info/
+-rw-rw-rw-   0        0        0     5505 2023-05-20 23:18:55.000000 basinmaker-3.1.0/basinmaker.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     5501 2023-05-20 23:18:55.000000 basinmaker-3.1.0/basinmaker.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-20 23:18:55.000000 basinmaker-3.1.0/basinmaker.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       11 2023-05-20 23:18:55.000000 basinmaker-3.1.0/basinmaker.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      108 2022-07-20 16:58:37.000000 basinmaker-3.1.0/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-05-20 23:18:55.711604 basinmaker-3.1.0/setup.cfg
+-rw-rw-rw-   0        0        0      828 2023-05-19 01:38:46.000000 basinmaker-3.1.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-20 23:18:55.708613 basinmaker-3.1.0/tests/
+-rw-rw-rw-   0        0        0     5251 2022-07-20 16:58:37.000000 basinmaker-3.1.0/tests/test_RoutingTool_AutomatedWatershedsandLakesFilterToolset.py
+-rw-rw-rw-   0        0        0     6085 2022-07-20 16:58:37.000000 basinmaker-3.1.0/tests/test_RoutingTool_Generateinputdata.py
+-rw-rw-rw-   0        0        0     6187 2022-07-20 16:58:37.000000 basinmaker-3.1.0/tests/test_RoutingTool_Generatmaskregion.py
+-rw-rw-rw-   0        0        0     5729 2022-07-20 16:58:37.000000 basinmaker-3.1.0/tests/test_RoutingTool_PostProcessing_Customize_Routing_Topology.py
+-rw-rw-rw-   0        0        0     2298 2022-07-20 16:58:37.000000 basinmaker-3.1.0/tests/test_RoutingTool_PostProcessing_Define_Final_Catchment.py
+-rw-rw-rw-   0        0        0     3378 2022-07-20 16:58:37.000000 basinmaker-3.1.0/tests/test_RoutingTool_PostProcessing_GenerateHRUS.py
+-rw-rw-rw-   0        0        0     3474 2022-07-20 16:58:37.000000 basinmaker-3.1.0/tests/test_RoutingTool_PostProcessing_GenerateRavenInput.py
+-rw-rw-rw-   0        0        0     1966 2022-07-20 16:58:37.000000 basinmaker-3.1.0/tests/test_RoutingTool_PostProcessing_Locate_subid_needsbyuser.py
+-rw-rw-rw-   0        0        0     4695 2022-07-20 16:58:37.000000 basinmaker-3.1.0/tests/test_RoutingTool_PostProcessing_SelectLakes.py
+-rw-rw-rw-   0        0        0     7034 2022-07-20 16:58:37.000000 basinmaker-3.1.0/tests/test_RoutingTool_PostProcessing_Select_Routing_product_based_SubId.py
+-rw-rw-rw-   0        0        0     5916 2022-07-20 16:58:37.000000 basinmaker-3.1.0/tests/test_RoutingTool_RoutingNetworkTopologyUpdateToolset_riv.py
+-rw-rw-rw-   0        0        0     6998 2022-07-20 16:58:37.000000 basinmaker-3.1.0/tests/test_RoutingTool_WatershedDiscretizationToolset.py
```

### Comparing `basinmaker-3.0.3a0/LICENSE` & `basinmaker-3.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `basinmaker-3.0.3a0/PKG-INFO` & `basinmaker-3.1.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: basinmaker
-Version: 3.0.3a0
+Version: 3.1.0
 Summary: An automated GIS toolbox for watershed delineation with lakes
 Home-page: https://github.com/dustming/basinmaker
 Author: basinmaker development team
 Author-email: m43han@uwaterloo.ca
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `basinmaker-3.0.3a0/README.md` & `basinmaker-3.1.0/README.md`

 * *Files identical despite different names*

### Comparing `basinmaker-3.0.3a0/basinmaker/addattributes/addattributestocatchments.py` & `basinmaker-3.1.0/basinmaker/addattributes/addattributestocatchments.py`

 * *Files identical despite different names*

### Comparing `basinmaker-3.0.3a0/basinmaker/addattributes/addgaugeattributesqgis.py` & `basinmaker-3.1.0/basinmaker/addattributes/addgaugeattributesqgis.py`

 * *Files identical despite different names*

### Comparing `basinmaker-3.0.3a0/basinmaker/addattributes/addlakeattributesqgis.py` & `basinmaker-3.1.0/basinmaker/addattributes/addlakeattributesqgis.py`

 * *Files identical despite different names*

### Comparing `basinmaker-3.0.3a0/basinmaker/addattributes/calbkfwidthdepthqgis.py` & `basinmaker-3.1.0/basinmaker/addattributes/calbkfwidthdepthqgis.py`

 * *Files identical despite different names*

### Comparing `basinmaker-3.0.3a0/basinmaker/addattributes/calculatebasicattributesqgis.py` & `basinmaker-3.1.0/basinmaker/addattributes/calculatebasicattributesqgis.py`

 * *Files identical despite different names*

### Comparing `basinmaker-3.0.3a0/basinmaker/addattributes/calfloodmanningnqgis.py` & `basinmaker-3.1.0/basinmaker/addattributes/calfloodmanningnqgis.py`

 * *Files identical despite different names*

### Comparing `basinmaker-3.0.3a0/basinmaker/addattributes/createattributestemplatearcgis.py` & `basinmaker-3.1.0/basinmaker/addattributes/createattributestemplatearcgis.py`

 * *Files 7% similar despite different names*

```diff
@@ -56,15 +56,15 @@
                        'DrainArea' : pd.Series(dtype='int64'),
                        'Strahler'  : pd.Series(dtype='int'),
                        'Seg_ID'    : pd.Series(dtype='int'),
                        'Seg_order' : pd.Series(dtype='int'),
                        # 'Max_DEM'   : pd.Series(dtype='float'),
                        # 'Min_DEM'   : pd.Series(dtype='float'),
                        'DA_Obs'    : pd.Series(dtype='float'),
-                       'DA_error'  : pd.Series(dtype='float'),
+                       'DA_Diff'  : pd.Series(dtype='float'),
                        # 'Obs_NM'    : pd.Series(dtype='float'),
                        # 'SRC_obs'   : pd.Series(dtype='float'),
                        # 'centroid_x': pd.Series(dtype='float'),
                        # 'centroid_y': pd.Series(dtype='float'),
                        'DA_Chn_L'  : pd.Series(dtype='float'),
                        'DA_Slope'  : pd.Series(dtype='float'),
                        'DA_Chn_Slp': pd.Series(dtype='float'),
@@ -203,22 +203,35 @@
     outlet_mask = final_pourpoints['DowSubId'] == final_pourpoints['SubId']
     final_pourpoints.loc[outlet_mask,'DowSubId'] = -1
 
     final_pourpoints["HyLakeId"] = final_pourpoints["cl_lake_id"]
     final_pourpoints.loc[final_pourpoints['HyLakeId'].isnull(),'HyLakeId'] = final_pourpoints.loc[final_pourpoints['HyLakeId'].isnull(),'ncl_kake_id']
 
     alllake123 = pd.DataFrame.spatial.from_featureclass("all_lakes_v")
-    alllake123['HyLakeId'] = alllake123[lake_attributes[0]]
-    alllake123 = alllake123[lake_attributes + ['HyLakeId']]
+    alllake123['HyLakeId'] = pd.to_numeric(alllake123[lake_attributes[0]])
+    alllake123 =alllake123[lake_attributes + ['HyLakeId']]
+
     obs_v123 = pd.DataFrame.spatial.from_featureclass("obs_clip")
-    obs_v123["obsid"] = obs_v123[obs_attributes[0]]
+    obs_v123["obsid"]       = pd.to_numeric(obs_v123[obs_attributes[0]])
+    obs_v123['obsid']       = obs_v123['obsid'].fillna(0)
+    obs_v123['obsid']       = obs_v123['obsid'].astype(int)
+
     obs_v123 = obs_v123[obs_attributes + ['obsid']]
+    
+    final_pourpoints['HyLakeId'] = pd.to_numeric(final_pourpoints['HyLakeId'])
+    final_pourpoints['HyLakeId']  = final_pourpoints['HyLakeId'].fillna(0)
+    final_pourpoints['HyLakeId'] = final_pourpoints['HyLakeId'].astype(int)
+
+    final_pourpoints['obsid'] = pd.to_numeric(final_pourpoints['obsid'])
+    final_pourpoints['obsid']  = final_pourpoints['obsid'].fillna(0)
+    final_pourpoints['obsid'] = final_pourpoints['obsid'].astype(int)
 
     final_pourpoints = final_pourpoints.merge(alllake123,on='HyLakeId',how='left')
     final_pourpoints = final_pourpoints.merge(obs_v123,on='obsid',how='left')
+
     final_pourpoints.spatial.to_featureclass(location=os.path.join(work_folder,"arcgis.gdb","final_pp_with_routing"),overwrite=True,sanitize_columns=False)
 
     final_pourpoints = final_pourpoints.sort_values(by='SubId', ascending=True)
 
     attri_table['SubId'] = final_pourpoints['SubId']
     attri_table = attri_table.fillna(-1.2345)
     attri_table['DowSubId'] = final_pourpoints['DowSubId'].fillna(0).astype(int)
@@ -227,22 +240,21 @@
     attri_table['LakeVol']  = final_pourpoints[lake_attributes[3]].fillna(0)
     attri_table['LakeDepth'] = final_pourpoints[lake_attributes[4]].fillna(0)
     attri_table['LakeArea'] =final_pourpoints[lake_attributes[2]].fillna(0)*1000*1000
     attri_table['Laketype'] = final_pourpoints[lake_attributes[1]].fillna(0)
     attri_table.loc[~final_pourpoints['ncl_kake_id'].isnull(),'Lake_Cat'] = 2
     attri_table.loc[~final_pourpoints['cl_lake_id'].isnull(),'Lake_Cat'] = 1
     attri_table['Has_POI'] = int(0)
-    attri_table.loc[~final_pourpoints['obsid'].isnull(),'Has_POI'] = int(1)
+    attri_table.loc[final_pourpoints['obsid'] != 0,'Has_POI'] = int(1)
     attri_table['DA_Obs'] = final_pourpoints[obs_attributes[2]].fillna(0)
     attri_table['Obs_NM'] = final_pourpoints[obs_attributes[1]].astype('str').fillna(" ")
     attri_table['SRC_obs'] = final_pourpoints[obs_attributes[3]].astype('str').fillna(" ")
     attri_table['outletLng'] = final_pourpoints['outletLng'].fillna(-1.2345)
     attri_table['outletLat'] = final_pourpoints['outletLat'].fillna(-1.2345)
 
-
     sub_attri = read_table_as_pandas("sub_degree",['Value','MEAN'],work_folder)
     sub_attri['BasSlope'] = sub_attri['MEAN'].fillna(-1.2345)
     sub_attri['SubId'] = sub_attri['Value']
     sub_attri = sub_attri.drop(columns=['MEAN', 'Value'])
     attri_table = attri_table.merge(sub_attri,on='SubId',how='left')
 
 
@@ -285,56 +297,120 @@
     riv_line['RivLength'] = riv_line['Length_m'].fillna(-1.2345)
     riv_line2 = riv_line[['SubId','RivLength']].copy(deep=True)
     attri_table = attri_table.merge(riv_line2,on='SubId',how='left')
 #    print(len(attri_table),"d")
 
 
     riv_attri = read_table_as_pandas("riv_slope",['Value','MEAN'],work_folder)
-    riv_attri['RivSlope'] = (riv_attri['MEAN']/100).fillna(-1.2345)
     riv_attri['SubId'] = riv_attri['Value']
     riv_attri = riv_attri.drop(columns=['MEAN', 'Value'])
     attri_table = attri_table.merge(riv_attri,on='SubId',how='left')
 #    print(len(attri_table),"c")
     riv_dem = read_table_as_pandas("riv_dem",['Value','MIN','MAX'],work_folder)
     riv_dem['Max_DEM'] = riv_dem['MAX'].fillna(-1.2345)
     riv_dem['Min_DEM'] = riv_dem['MIN'].fillna(-1.2345)
     riv_dem['SubId'] = riv_dem['Value']
     riv_dem = riv_dem.drop(columns=['MIN', 'MAX','Value'])
     attri_table = attri_table.merge(riv_dem,on='SubId',how='left')
+    attri_table['RivSlope'] = (attri_table['Max_DEM'] - attri_table['Min_DEM']) / attri_table['RivLength']
 #    print(len(attri_table),"b")
     riv_landuse = read_table_as_pandas("riv_landuse",['Value','MEAN'],work_folder)
     riv_landuse['FloodP_n'] = riv_landuse['MEAN'] / 1000.0
     riv_landuse['FloodP_n'] = riv_landuse['FloodP_n'].fillna(-1.2345)
     riv_landuse['SubId'] = riv_landuse['Value']
     riv_landuse = riv_landuse.drop(columns=['MEAN','Value'])
     attri_table = attri_table.merge(riv_landuse,on='SubId',how='left')
 
     attri_table = attri_table.drop_duplicates(subset=['SubId'], keep='first')
     attri_table = streamorderanddrainagearea(attri_table)
     attri_table = calculate_bkf_width_depth(attri_table)
 
     attri_table = update_non_connected_catchment_info(attri_table)
-    attri_table.loc[attri_table['DA_Obs'] > 0,'DA_error'] = (attri_table.loc[attri_table['DA_Obs'] > 0,'DrainArea']/1000/1000)/attri_table.loc[attri_table['DA_Obs'] > 0,'DA_Obs']
+    attri_table.loc[attri_table['DA_Obs'] > 0,'DA_Diff'] = (attri_table.loc[attri_table['DA_Obs'] > 0,'DrainArea']/1000/1000 - attri_table.loc[attri_table['DA_Obs'] > 0,'DA_Obs'])/attri_table.loc[attri_table['DA_Obs'] > 0,'DA_Obs']
+    attri_table.loc[attri_table['DA_Obs'] <= 0,'DA_Diff'] = -999
+    # non-null values are shown as percentage
+    attri_table['DA_Diff'] = attri_table['DA_Diff'].apply(lambda x: f"{x*100:.3f}%" if x != -999 else "<NA>")
+
+    attri_table.loc[attri_table['DA_Obs'] <= 0, 'DA_Obs'] = -1.2345
+    # print(attri_table['DA_Diff'].values)
+    
     attri_table.loc[attri_table['RivLength'] == -1.2345,'RivSlope'] = -1.2345
     attri_table.loc[attri_table['RivLength'] == -1.2345,'FloodP_n'] = -1.2345
     attri_table.loc[attri_table['RivLength'] == -1.2345,'Max_DEM'] = -1.2345
     attri_table.loc[attri_table['RivLength'] == -1.2345,'Min_DEM'] = -1.2345
     attri_table.loc[attri_table['RivLength'] == -1.2345,'Ch_n'] = -1.2345
-
+    attri_table = attri_table[[
+                       'SubId'    ,
+                       'DowSubId' ,
+                       'RivSlope' ,
+                       'RivLength' ,
+                       'BasSlope'  ,
+                       'BasAspect',
+                       'BasArea'   ,
+                       'BkfWidth'  ,
+                       'BkfDepth' ,
+                       'Lake_Cat'  ,
+                       'HyLakeId'  ,
+                       'LakeVol'  ,
+                       'LakeDepth' ,
+                       'LakeArea'  ,
+                       'Laketype'  ,
+                       'Has_POI'   ,
+                       'MeanElev'  ,
+                       'FloodP_n' ,
+                       'Q_Mean'    ,
+                       'Ch_n'      ,
+                       'DrainArea' ,
+                       'Strahler'  ,
+                       'Seg_ID'   ,
+                       'Seg_order',
+                       'Max_DEM'  ,
+                       'Min_DEM'  ,
+                       'DA_Obs'    ,
+                       'DA_Diff' ,
+                       'Obs_NM'    ,
+                       'SRC_obs'  ,
+                       'centroid_x',
+                       'centroid_y',
+                       'DA_Chn_L' ,
+                       'DA_Slope'  ,
+                       'DA_Chn_Slp',
+                       'outletLat' ,
+                       'outletLng' ,
+                       'k'         ,
+                       'c'        
+    ]]
+    attri_table.to_csv(os.path.join(work_folder,"attri_table.csv"),index=False) 
     cat_ply= cat_ply[['SubId','SHAPE']]
+    cat_ply['SubId']  = pd.to_numeric(cat_ply['SubId'])
+    cat_ply['SubId']  = cat_ply['SubId'].fillna(0)
+    cat_ply['SubId']  = cat_ply['SubId'].astype(int)
+
     cat_ply = cat_ply.merge(attri_table,on='SubId',how='left')
-    cat_ply = cat_ply.fillna(-1.2345)
+    for col_i in cat_ply.columns:
+        # DA_Diff use np.nan for null values
+        if col_i != "DA_Diff":
+            cat_ply[col_i] = cat_ply[col_i].fillna(-1.2345)
     cat_ply['Obs_NM'] = cat_ply['Obs_NM'].astype('str')
     cat_ply['SRC_obs'] = cat_ply['SRC_obs'].astype('str')
     cat_ply = cat_ply.drop_duplicates(subset=['SubId'], keep='first')
+
     cat_ply.spatial.to_featureclass(location=os.path.join(output_folder,catchment_without_merging_lakes+"_v1-0"),overwrite=True,sanitize_columns=False)
 
     riv_line= riv_line[['SubId','SHAPE']]
+    riv_line['SubId']  = pd.to_numeric(riv_line['SubId'])
+    riv_line['SubId']  = riv_line['SubId'].fillna(0)
+    riv_line['SubId']  = riv_line['SubId'].astype(int)
+
     riv_line = riv_line.merge(attri_table,on='SubId',how='left')
-    riv_line = riv_line.fillna(-1.2345)
+    for col_i in riv_line.columns:
+        # DA_Diff use np.nan for null values
+        if col_i != "DA_Diff":
+            riv_line[col_i] = riv_line[col_i].fillna(-1.2345)
+
     riv_line['Obs_NM'] = riv_line['Obs_NM'].astype('str')
     riv_line['SRC_obs'] = riv_line['SRC_obs'].astype('str')
     riv_line = riv_line.drop_duplicates(subset=['SubId'], keep='first')
     riv_line.spatial.to_featureclass(location=os.path.join(output_folder,river_without_merging_lakes+"_v1-0"),overwrite=True,sanitize_columns=False)
 
     
     arcpy.FeatureClassToFeatureClass_conversion("sl_connected_lake_v", output_folder,"sl_connected_lake_v1-0.shp")
@@ -352,18 +428,20 @@
     obs_v2 = pd.DataFrame.spatial.from_featureclass("obs_clip")
     obs_v2['obsid'] = obs_v2['Obs_ID']
     obs_v_missing = obs_v2[~obs_v2['obsid'].isin(final_pourpoints['obsid'].values)].copy(deep=True)
 
     final_pourpoints_2 = final_pourpoints[['obsid','SubId']]
     obs_v = obs_v.merge(final_pourpoints_2,on='obsid',how='left')
     obs_v = obs_v[['SubId','SHAPE']]
-    cat_ply_att = cat_ply[['SubId','DA_Obs','SRC_obs','DrainArea','DA_error','Obs_NM']]
+    cat_ply_att = cat_ply[['SubId','DA_Obs','SRC_obs','DrainArea','DA_Diff','Obs_NM']]
     obs_v = obs_v.merge(cat_ply_att,on='SubId',how='left')
-    obs_v = obs_v[['SubId','DA_Obs','SRC_obs','DrainArea','DA_error','Obs_NM','SHAPE']]
-    obs_v.spatial.to_featureclass(location=os.path.join(output_folder,"poi_v1-0.shp"),overwrite=True,sanitize_columns=False)
+    obs_v['Use_region'] = 1
+    obs_v = obs_v[['SubId','Obs_NM','DA_Obs','DrainArea','DA_Diff','SRC_obs','Use_region','SHAPE']]
+    if len(obs_v) > 0:
+        obs_v.spatial.to_featureclass(location=os.path.join(output_folder,"poi_v1-0.shp"),overwrite=True,sanitize_columns=False)
     if len(obs_v_missing) > 0:
         obs_v_missing.spatial.to_featureclass(location=os.path.join(output_folder,"poi_missing.shp"),overwrite=True,sanitize_columns=False)
 
     arcpy.DeleteField_management(os.path.join(output_folder,"poi_v1-0.shp"),
                              ["Id"])
     arcpy.DeleteField_management(os.path.join(output_folder,catchment_without_merging_lakes+"_v1-0"),
                              ["Id"])
```

### Comparing `basinmaker-3.0.3a0/basinmaker/addattributes/createattributestemplateqgis.py` & `basinmaker-3.1.0/basinmaker/addattributes/createattributestemplateqgis.py`

 * *Files identical despite different names*

### Comparing `basinmaker-3.0.3a0/basinmaker/addattributes/exportoutputsqgis.py` & `basinmaker-3.1.0/basinmaker/addattributes/exportoutputsqgis.py`

 * *Files identical despite different names*

### Comparing `basinmaker-3.0.3a0/basinmaker/addattributes/joinpandastoattributesqgis.py` & `basinmaker-3.1.0/basinmaker/addattributes/joinpandastoattributesqgis.py`

 * *Files identical despite different names*

### Comparing `basinmaker-3.0.3a0/basinmaker/addlakeandobs/addlakeandobsintowatershed.py` & `basinmaker-3.1.0/basinmaker/addlakeandobs/addlakeandobsintowatershed.py`

 * *Files identical despite different names*

### Comparing `basinmaker-3.0.3a0/basinmaker/addlakeandobs/addlakesarcgis.py` & `basinmaker-3.1.0/basinmaker/addlakeandobs/addlakesarcgis.py`

 * *Files identical despite different names*

### Comparing `basinmaker-3.0.3a0/basinmaker/addlakeandobs/addlakesqgis.py` & `basinmaker-3.1.0/basinmaker/addlakeandobs/addlakesqgis.py`

 * *Files identical despite different names*

### Comparing `basinmaker-3.0.3a0/basinmaker/addlakeandobs/addobsarcgis.py` & `basinmaker-3.1.0/basinmaker/addlakeandobs/addobsarcgis.py`

 * *Files identical despite different names*

### Comparing `basinmaker-3.0.3a0/basinmaker/addlakeandobs/addobsqgis.py` & `basinmaker-3.1.0/basinmaker/addlakeandobs/addobsqgis.py`

 * *Files identical despite different names*

### Comparing `basinmaker-3.0.3a0/basinmaker/addlakeandobs/definecatrivarcgis.py` & `basinmaker-3.1.0/basinmaker/addlakeandobs/definecatrivarcgis.py`

 * *Files identical despite different names*

### Comparing `basinmaker-3.0.3a0/basinmaker/addlakeandobs/definecatrivqgis.py` & `basinmaker-3.1.0/basinmaker/addlakeandobs/definecatrivqgis.py`

 * *Files identical despite different names*

### Comparing `basinmaker-3.0.3a0/basinmaker/addlakeandobs/definelaketypeqgis.py` & `basinmaker-3.1.0/basinmaker/addlakeandobs/definelaketypeqgis.py`

 * *Files identical despite different names*

### Comparing `basinmaker-3.0.3a0/basinmaker/addlakeandobs/filterlakesqgis.py` & `basinmaker-3.1.0/basinmaker/addlakeandobs/filterlakesqgis.py`

 * *Files identical despite different names*

### Comparing `basinmaker-3.0.3a0/basinmaker/addlakeandobs/modifyfdr.py` & `basinmaker-3.1.0/basinmaker/addlakeandobs/modifyfdr.py`

 * *Files identical despite different names*

### Comparing `basinmaker-3.0.3a0/basinmaker/addlakeandobs/modifystr.py` & `basinmaker-3.1.0/basinmaker/addlakeandobs/modifystr.py`

 * *Files identical despite different names*

### Comparing `basinmaker-3.0.3a0/basinmaker/addlakeandobs/pourpointsqgis.py` & `basinmaker-3.1.0/basinmaker/addlakeandobs/pourpointsqgis.py`

 * *Files identical despite different names*

### Comparing `basinmaker-3.0.3a0/basinmaker/arcgisguiwarpper/generatehru_arcgis_wrapper.py` & `basinmaker-3.1.0/basinmaker/arcgisguiwarpper/generatehru_arcgis_wrapper.py`

 * *Files identical despite different names*

### Comparing `basinmaker-3.0.3a0/basinmaker/arcgisguiwarpper/generateraveninput_arcgis_wrapper.py` & `basinmaker-3.1.0/basinmaker/arcgisguiwarpper/generateraveninput_arcgis_wrapper.py`

 * *Files identical despite different names*

### Comparing `basinmaker-3.0.3a0/basinmaker/arcgisguiwarpper/selectprod_arcgis_wrapper.py` & `basinmaker-3.1.0/basinmaker/arcgisguiwarpper/selectprod_arcgis_wrapper.py`

 * *Files identical despite different names*

### Comparing `basinmaker-3.0.3a0/basinmaker/arcgisguiwarpper/simplyda_arcgis_wrapper.py` & `basinmaker-3.1.0/basinmaker/arcgisguiwarpper/simplyda_arcgis_wrapper.py`

 * *Files identical despite different names*

### Comparing `basinmaker-3.0.3a0/basinmaker/arcgisguiwarpper/simplylakes_arcgis_wrapper.py` & `basinmaker-3.1.0/basinmaker/arcgisguiwarpper/simplylakes_arcgis_wrapper.py`

 * *Files identical despite different names*

### Comparing `basinmaker-3.0.3a0/basinmaker/basinmaker.py` & `basinmaker-3.1.0/basinmaker/basinmaker.py`

 * *Files 2% similar despite different names*

```diff
@@ -184,14 +184,15 @@
         self,
         path_output_folder="#",
         routing_product_folder  = '#',
         connected_lake_area_thresthold=-1,
         non_connected_lake_area_thresthold =-1,
         selected_lake_ids=[],
         area_thresthold = 10*30*30/1000/1000,
+        length_thresthold=0.01,
         gis_platform="qgis",
     ):
         """This function is to simplify the hydrologic routing network by removing
         lakes.
 
         Parameters
         ----------
@@ -293,24 +294,26 @@
             combine_catchments_covered_by_the_same_lake_method,
         )
 
         combine_catchments_covered_by_the_same_lake_method(
             Routing_Product_Folder = path_output_folder,
             qgis_prefix_path=self.qgispp,
             area_thresthold = area_thresthold,
+            length_thresthold = length_thresthold,
             gis_platform=gis_platform,
         )
 
 
     def Decrease_River_Network_Resolution(
         self,
         path_output_folder="#",
         routing_product_folder = '#',
         gis_platform="qgis",
         minimum_subbasin_drainage_area=-1,
+        length_thresthold = 0.01,
         area_thresthold = 10*30*30/1000/1000,
     ):
         """ This function is to simplify the hydrologic routing network by
         removing subbasins/river reaches with their drainage area below user provided
         drainage area thresthold.
 
         Parameters
@@ -397,70 +400,86 @@
             combine_catchments_covered_by_the_same_lake_method,
         )
 
         combine_catchments_covered_by_the_same_lake_method(
             Routing_Product_Folder = path_output_folder,
             qgis_prefix_path=self.qgispp,
             area_thresthold = area_thresthold,
+            length_thresthold = length_thresthold,
             gis_platform=gis_platform,
         )
 
     def Add_Point_Of_Interest_Sites_In_Routing_Product(
         self,
         routing_product_folder= '#',
         path_to_points_of_interest_points = '#',
         path_output_folder="#",
         clean_exist_pois = True,
         gis_platform="purepy",
         area_thresthold = 10*30*30/1000/1000,
+        length_thresthold = 1,
     ):
-        """ The function allows the user to modify point of interest (POI) 
-        related attributes in the routing product. The function is particularly
-        useful when the user wants to add new POI sites, remove existing POI 
-        sites,or modify the location of existing POI sites in the developed 
-        routing products. If the user observes a small subbasin that cannot 
-        be removed by the Decrease_River_Network_Resolution function due 
-        to it representing an unexpected POI, they can use this function to 
-        remove the POI from the routing product and then 
-        apply the Decrease_River_Network_Resolution function.
+        """This function allows the user to modify point of interest (POI) 
+        sites in a pre-existing BasinMaker-generated user input hydrologic 
+        routing network/product. Specific modifications this function can 
+        make are to add new POI sites, remove existing POI sites, or modify
+        the location of existing POI sites in the input routing network. 
+        This function will use the location of the provided POI and link 
+        them to the subbasins in the routing network. At least one POI 
+        should be provided in the point shapefile. 
 
         Parameters
         ----------
         path_output_folder                   : string
             is the folder path that stores generated outputs
         routing_product_folder         : string
             is the folder path where the input hydrologic routing network is stored
         path_to_points_of_interest_points                : string
-            is the path to the point shapefile that contains the point of 
-            interest (POI) sites. The shapefile must have an attribute table that includes 
-            the following columns:
-              - Obs_NM (string): This column should contain the name or ID of the POI site.
+            is the path to the point shapefile that contains the point of interest (POI) sites. 
+            The shapefile must have an attribute table that includes the following columns:
+             
+              - Obs_NM (string): This column should contain the name or ID of the POI site. 
+                When the provided POI has the same Obs_NM as the existing POI in the routing
+                product, this function will assume that the user wants to relocate the existing 
+                POI. Otherwise, the clean_exist_pois variable below controls whether the new POI 
+                sites fully replace existing POI sites or augment the existing POI sites.
+              
               - DA_Obs (float): This column should contain the drainage area of the POI site.
+              
               - SRC_obs (string): This column should contain the source of the POI site.
+              
+              - Type (string): This column should contain the type of the POI site. Each POI 
+                can only have one type. The following types are currently supported: "Lake": the 
+                POI is located on a lake waterbody surface. "River": the POI is located on a 
+                river channel. Note that the "Lake" type POI should be located within a lake 
+                subbasin and the "River" type POI should be located within a non-lake subbasin. 
+                The POI located in the wrong subbasin will be ignored and not added to the routing 
+                product. The “River” type POI will be linked to a non-lake subbasin that contains 
+                the POI. The “Lake” type POI will be linked to the lake subbasin that contains the POI. 
+        
         gis_platform                   : string
             is the parameter indicating which gis platform is used. Currenly, only "purepy" 
             is allowed for this parameter.
         clean_exist_pois                : boolean
-            Indicate if user want to remove all existing POI in the input routing product.
-        area_thresthold             : float (optional)
-            This parameter sets a subbasin area threshold in square kilometers (km²). 
-            Subbasins with an area below this threshold will be merged with downstream 
-            or upstream subbasins, depending on their location within the river network. 
-            This can be useful for simplifying the river network and reducing computational
-            requirements. The parameter is optional and has a default value of 0.009 km2. 
-            If the parameter is set to 0, no subbasin merging will be performed.
+            Indicates if the user wants to remove all existing POI in the input routing product. 
+            When it is true, all existing POI will be removed, and only the POI sites provided in
+            the path_to_points_of_interest_points will be added to the input routing network. 
 
         Returns
         -------
 
         Notes
         -----
-        This function has no return values, The modified hydrological routing
-        network will be generated in the path_output_folder including following
-        files:
+        This function does not return any values. If the user only wants to add POI to the routing 
+        product, they should set clean_exist_pois to False. This will keep the existing POI and 
+        add the provided POI to the routing product. If the user wants to remove all existing POI 
+        and add new POI, they should set clean_exist_pois to True. This will remove all existing 
+        POI from the routing product and then add the provided POI to the routing product. 
+        The modified hydrological routing network will be generated in the path_output_folder 
+        and will include the following files:
 
         finalcat_info.shp                     : shapefile
             The finalized hydrologic routing network. the GIS layer containing
             subbasin polygons which respect the lake inflow and outflow routing
             structures. This layer contains all the necessary information for
             hydrologic routing through the lake-river network.
         finalcat_info_riv.shp                 : shapefile
@@ -512,14 +531,15 @@
             combine_catchments_covered_by_the_same_lake_method,
         )
 
         combine_catchments_covered_by_the_same_lake_method(
             Routing_Product_Folder = path_output_folder,
             qgis_prefix_path=self.qgispp,
             area_thresthold = area_thresthold,
+            length_thresthold = length_thresthold,
             gis_platform=gis_platform,
         )
 
     def Select_Subregion_Of_Routing_Structure(
         self,
         path_output_folder="#",
         routing_product_folder = '#',
@@ -1429,14 +1449,15 @@
         )
 
     def Combine_Subbasins_Covered_by_The_Same_Lake(
         self,
         routing_product_folder='#',
         gis_platform="qgis",
         area_thresthold = 10*30*30/1000/1000,
+        length_thresthold = 1,
     ):
         """Finalize a incomplete hydrologic routing network by merging subbasin
         polygons that are covered by the same lake.
 
         Parameters
         ----------
         routing_product_folder         : string
@@ -1470,8 +1491,9 @@
         )
 
         combine_catchments_covered_by_the_same_lake_method(
             Routing_Product_Folder = routing_product_folder,
             qgis_prefix_path=self.qgispp,
             gis_platform=gis_platform,
             area_thresthold = area_thresthold,
+            length_thresthold = length_thresthold,
         )
```

### Comparing `basinmaker-3.0.3a0/basinmaker/delineationnolake/watdelineationwithoutlake.py` & `basinmaker-3.1.0/basinmaker/delineationnolake/watdelineationwithoutlake.py`

 * *Files identical despite different names*

### Comparing `basinmaker-3.0.3a0/basinmaker/delineationnolake/watusingdemarcgis.py` & `basinmaker-3.1.0/basinmaker/delineationnolake/watusingdemarcgis.py`

 * *Files identical despite different names*

### Comparing `basinmaker-3.0.3a0/basinmaker/delineationnolake/watusingdemqgis.py` & `basinmaker-3.1.0/basinmaker/delineationnolake/watusingdemqgis.py`

 * *Files identical despite different names*

### Comparing `basinmaker-3.0.3a0/basinmaker/delineationnolake/watusingfacqgis.py` & `basinmaker-3.1.0/basinmaker/delineationnolake/watusingfacqgis.py`

 * *Files identical despite different names*

### Comparing `basinmaker-3.0.3a0/basinmaker/delineationnolake/watusingfdrarcgis.py` & `basinmaker-3.1.0/basinmaker/delineationnolake/watusingfdrarcgis.py`

 * *Files 7% similar despite different names*

```diff
@@ -39,25 +39,28 @@
     arcpy.env.extent = arcpy.Describe(dem).extent
     arcpy.env.snapRaster =  dem
 
     outFlowDirection = ExtractByMask(fdr_path, mask)
     dirraster = SetNull(Raster(outFlowDirection) < 1, Raster(outFlowDirection))
     dirraster.save(fdr_arcgis)
 
-    # outFlowAccumulation= ExtractByMask(fac_path, mask)
-    # outFlowAccumulation.save("acc_to_str")
-
     finalacc = FlowAccumulation(in_flow_direction_raster = fdr_arcgis, data_type = "INTEGER" )
     finalacc.save(acc)
 
     #
     # outFlowAccumulation = FlowAccumulation(dirraster)
     # outFlowAccumulation.save(acc)
 
-    StreamRaster = SetNull(Raster(finalacc) < acc_thresold, Raster(finalacc))
+    if fac_path != '#':
+        outFlowAccumulation= ExtractByMask(fac_path, mask)
+        outFlowAccumulation.save("acc_to_str")
+        StreamRaster = SetNull(Raster(outFlowAccumulation) < acc_thresold, Raster(outFlowAccumulation))
+    else:
+        StreamRaster = SetNull(Raster(finalacc) < acc_thresold, Raster(finalacc))
+
     StreamRaster = Con(StreamRaster >= 0, 1, 0)
     StreamRaster.save("str_1")
 
     Strlink = StreamLink(StreamRaster, dirraster)
     Strlink.save(str_r)
 
     Catchment = Watershed(dirraster,Strlink)
```

### Comparing `basinmaker-3.0.3a0/basinmaker/delineationnolake/watusingfdrqgis.py` & `basinmaker-3.1.0/basinmaker/delineationnolake/watusingfdrqgis.py`

 * *Files identical despite different names*

### Comparing `basinmaker-3.0.3a0/basinmaker/delineationnolake/watusingsubregionddata.py` & `basinmaker-3.1.0/basinmaker/delineationnolake/watusingsubregionddata.py`

 * *Files identical despite different names*

### Comparing `basinmaker-3.0.3a0/basinmaker/extent/projectextent.py` & `basinmaker-3.1.0/basinmaker/extent/projectextent.py`

 * *Files identical despite different names*

### Comparing `basinmaker-3.0.3a0/basinmaker/extent/usingdemarcgis.py` & `basinmaker-3.1.0/basinmaker/extent/usingdemarcgis.py`

 * *Files identical despite different names*

### Comparing `basinmaker-3.0.3a0/basinmaker/extent/usingdemqgis.py` & `basinmaker-3.1.0/basinmaker/extent/usingdemqgis.py`

 * *Files identical despite different names*

### Comparing `basinmaker-3.0.3a0/basinmaker/extent/usinghybasinplyarcgis.py` & `basinmaker-3.1.0/basinmaker/extent/usinghybasinplyarcgis.py`

 * *Files identical despite different names*

### Comparing `basinmaker-3.0.3a0/basinmaker/extent/usinghybasinplyqgis.py` & `basinmaker-3.1.0/basinmaker/extent/usinghybasinplyqgis.py`

 * *Files identical despite different names*

### Comparing `basinmaker-3.0.3a0/basinmaker/extent/usinginputplyqgis.py` & `basinmaker-3.1.0/basinmaker/extent/usinginputplyqgis.py`

 * *Files identical despite different names*

### Comparing `basinmaker-3.0.3a0/basinmaker/extent/usingoutletpointqgis.py` & `basinmaker-3.1.0/basinmaker/extent/usingoutletpointqgis.py`

 * *Files identical despite different names*

### Comparing `basinmaker-3.0.3a0/basinmaker/func/__pycache__/arcgis.cpython-39.pyc` & `basinmaker-3.1.0/basinmaker/func/__pycache__/arcgis.cpython-39.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.9, timestamp-based, .py timestamp: Mon Feb 27 03:39:45 2023 UTC, .py size: 35090 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 10% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 610d 0d0a 0000 0000 0126 fc63 1289 0000  a........&.c....
+00000000: 610d 0d0a 0000 0000 26d3 6664 bf8d 0000  a.......&.fd....
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0003 0000 0040 0000 0073 2e01 0000 6400  .....@...s....d.
 00000030: 6401 6c00 6d01 5a01 0100 6400 6402 6c02  d.l.m.Z...d.d.l.
 00000040: 6d03 5a03 6d04 5a04 0100 6400 6403 6c05  m.Z.m.Z...d.d.l.
 00000050: 5a05 6400 6404 6c05 6d06 5a06 0100 6400  Z.d.d.l.m.Z...d.
 00000060: 6405 6c07 5400 6400 6403 6c08 5a09 6400  d.l.T.d.d.l.Z.d.
 00000070: 6403 6c0a 5a0a 6400 6403 6c0b 5a0c 6400  d.l.Z.d.d.l.Z.d.
@@ -33,28 +33,28 @@
 00000200: 7c04 7402 7c02 7c05 1900 8301 1700 7d04  |.t.|.|.......}.
 00000210: 711e 7c04 6404 1700 7402 7c02 7c05 1900  q.|.d...t.|.|...
 00000220: 8301 1700 7d04 711e 7c04 6405 1700 7d04  ....}.q.|.d...}.
 00000230: 7403 a004 7c00 7c03 7c04 a103 0100 6400  t...|.|.|.....d.
 00000240: 5300 2906 4e7a 0722 2573 2220 494e 7a02  S.).Nz."%s" INz.
 00000250: 2028 7201 0000 00fa 012c fa01 2929 05da   (r......,..))..
 00000260: 0572 616e 6765 da03 6c65 6eda 0373 7472  .range..len..str
-00000270: da05 6172 6370 79da 0f53 656c 6563 745f  ..arcpy..Select_
+00000270: da05 6172 6370 795a 0f53 656c 6563 745f  ..arcpyZ.Select_
 00000280: 616e 616c 7973 6973 2906 da05 696e 7075  analysis)...inpu
 00000290: 745a 0841 7474 7269 5f4e 4d5a 0741 7474  tZ.Attri_NMZ.Att
-000002a0: 7269 5f76 da06 6f75 7470 7574 da0c 7768  ri_v..output..wh
+000002a0: 7269 5f76 da06 6f75 7470 7574 5a0c 7768  ri_v..outputZ.wh
 000002b0: 6572 655f 636c 6175 7365 da01 69a9 0072  ere_clause..i..r
-000002c0: 1500 0000 fa47 633a 5c75 7365 7273 5c6d  .....Gc:\users\m
+000002c0: 1300 0000 fa47 633a 5c75 7365 7273 5c6d  .....Gc:\users\m
 000002d0: 3433 6861 6e5f 325c 646f 6375 6d65 6e74  43han_2\document
 000002e0: 735c 6769 7468 7562 5c62 6173 696e 6d61  s\github\basinma
 000002f0: 6b65 725c 6261 7369 6e6d 616b 6572 5c66  ker\basinmaker\f
 00000300: 756e 635c 6172 6367 6973 2e70 79da 2373  unc\arcgis.py.#s
 00000310: 656c 6563 745f 6665 6174 7572 655f 6279  elect_feature_by
 00000320: 5f61 7474 7269 6275 7465 735f 6172 6367  _attributes_arcg
 00000330: 6973 1700 0000 7312 0000 0000 0108 0108  is....s.........
-00000340: 0112 0108 0112 0216 0108 020e 0172 1700  .............r..
+00000340: 0112 0108 0112 0216 0108 020e 0172 1500  .............r..
 00000350: 0000 6302 0000 0000 0000 0000 0000 0005  ..c.............
 00000360: 0000 0005 0000 0043 0000 0073 8400 0000  .......C...s....
 00000370: 7400 a001 7c00 6401 1900 a002 7c01 a101  t...|.d.....|...
 00000380: a101 7d02 7c00 6402 1900 6403 6b03 7d03  ..}.|.d...d.k.}.
 00000390: 7400 a003 7c02 7c03 a102 7d04 6404 7c00  t...|.|...}.d.|.
 000003a0: 6a04 7c04 6401 6602 3c00 6404 7c00 6a04  j.|.d.f.<.d.|.j.
 000003b0: 7c04 6405 6602 3c00 6404 7c00 6a04 7c04  |.d.f.<.d.|.j.|.
@@ -74,30 +74,30 @@
 00000490: 7475 726e 733a 0a20 2020 202d 2d2d 2d2d  turns:.    -----
 000004a0: 2d2d 0a20 2020 2020 2020 204e 6f6e 652c  --.        None,
 000004b0: 2074 6865 2061 7474 7269 6275 7465 2074   the attribute t
 000004c0: 6162 6c65 206f 6620 5061 7468 5f73 6870  able of Path_shp
 000004d0: 6669 6c65 2077 696c 6c20 6265 2075 7064  file will be upd
 000004e0: 6174 6564 0a20 2020 20da 0848 794c 616b  ated.    ..HyLak
 000004f0: 6549 64da 084c 616b 655f 4361 74e9 0200  eId..Lake_Cat...
-00000500: 0000 7201 0000 005a 074c 616b 6556 6f6c  ..r....Z.LakeVol
-00000510: 5a08 4c61 6b65 4172 6561 5a09 4c61 6b65  Z.LakeAreaZ.Lake
-00000520: 4465 7074 685a 084c 616b 6574 7970 6529  DepthZ.Laketype)
+00000500: 0000 7201 0000 00da 074c 616b 6556 6f6c  ..r......LakeVol
+00000510: da08 4c61 6b65 4172 6561 da09 4c61 6b65  ..LakeArea..Lake
+00000520: 4465 7074 68da 084c 616b 6574 7970 6529  Depth..Laketype)
 00000530: 05da 026e 70da 0b6c 6f67 6963 616c 5f6e  ...np..logical_n
 00000540: 6f74 da04 6973 696e da0b 6c6f 6769 6361  ot..isin..logica
-00000550: 6c5f 616e 64da 036c 6f63 2905 5a0c 6669  l_and..loc).Z.fi
-00000560: 6e61 6c63 6174 5f70 6c79 5a0d 436f 6e6e  nalcat_plyZ.Conn
+00000550: 6c5f 616e 64da 036c 6f63 2905 da0c 6669  l_and..loc)...fi
+00000560: 6e61 6c63 6174 5f70 6c79 da0d 436f 6e6e  nalcat_ply..Conn
 00000570: 5f4c 616b 655f 4964 73da 056d 6173 6b31  _Lake_Ids..mask1
-00000580: da05 6d61 736b 32da 046d 6173 6b72 1500  ..mask2..maskr..
-00000590: 0000 7215 0000 0072 1600 0000 da37 5265  ..r....r.....7Re
+00000580: da05 6d61 736b 32da 046d 6173 6b72 1300  ..mask2..maskr..
+00000590: 0000 7213 0000 0072 1400 0000 da37 5265  ..r....r.....7Re
 000005a0: 6d6f 7665 5f55 6e73 656c 6563 7465 645f  move_Unselected_
 000005b0: 4c61 6b65 5f41 7474 7269 6275 7465 5f49  Lake_Attribute_I
 000005c0: 6e5f 4669 6e61 6c63 6174 696e 666f 5f41  n_Finalcatinfo_A
 000005d0: 7263 6769 7326 0000 0073 1400 0000 000d  rcgis&...s......
 000005e0: 1401 0c01 0c02 0e01 0e01 0e01 0e01 0e01  ................
-000005f0: 0e02 7223 0000 00da 0553 7562 4964 6307  ..r#.....SubIdc.
+000005f0: 0e02 7227 0000 00da 0553 7562 4964 6307  ..r'.....SubIdc.
 00000600: 0000 0000 0000 0000 0000 000c 0000 0009  ................
 00000610: 0000 0043 0000 0073 3802 0000 7c00 6a00  ...C...s8...|.j.
 00000620: 6a01 7402 6a03 a004 7c01 6401 a102 6402  j.t.j...|.d...d.
 00000630: 6403 6404 8d03 0100 7405 a006 7402 6a03  d.d.....t...t.j.
 00000640: a004 7c01 6401 a102 7402 6a03 a004 7c02  ..|.d...t.j...|.
 00000650: 7c03 a102 7c06 6701 a103 0100 7405 a007  |...|.g.....t...
 00000660: 7402 6a03 a004 7c02 7c03 a102 7c06 7402  t.j...|.|...|.t.
@@ -130,98 +130,98 @@
 00000810: 0100 7405 a007 7402 6a03 a004 7c02 7c04  ..t...t.j...|.|.
 00000820: a102 6417 7402 6a03 a004 7c01 641f a102  ..d.t.j...|.d...
 00000830: 6417 a104 0100 7405 a008 7402 6a03 a004  d.....t...t.j...
 00000840: 7c02 7c04 a102 6700 6420 a201 a102 0100  |.|...g.d ......
 00000850: 6400 5300 2921 4e7a 0f75 7064 6174 6561  d.S.)!Nz.updatea
 00000860: 7474 7269 2e73 6870 5446 a903 da08 6c6f  ttri.shpTF....lo
 00000870: 6361 7469 6f6e da09 6f76 6572 7772 6974  cation..overwrit
-00000880: 65da 1073 616e 6974 697a 655f 636f 6c75  e..sanitize_colu
+00000880: 655a 1073 616e 6974 697a 655f 636f 6c75  eZ.sanitize_colu
 00000890: 6d6e 7329 0eda 0753 7562 4964 5f31 da02  mns)...SubId_1..
 000008a0: 4964 da07 6e73 7562 6964 32da 066e 7375  Id..nsubid2..nsu
 000008b0: 6269 64da 0a6e 646f 776e 7375 6269 64da  bid..ndownsubid.
 000008c0: 094f 6c64 5f53 7562 4964 da0a 4f6c 645f  .Old_SubId..Old_
 000008d0: 446f 7753 7562 da0a 4a6f 696e 5f43 6f75  DowSub..Join_Cou
-000008e0: 6e74 da0a 5441 5247 4554 5f46 4944 722a  nt..TARGET_FIDr*
+000008e0: 6e74 da0a 5441 5247 4554 5f46 4944 722d  nt..TARGET_FIDr-
 000008f0: 0000 00da 0a53 7562 4944 5f4f 6c64 72da  .....SubID_Oldr.
 00000900: 0a48 5255 5f49 445f 4e5f 31da 0a48 5255  .HRU_ID_N_1..HRU
 00000910: 5f49 445f 4e5f 32da 0766 6163 7465 7273  _ID_N_2..facters
 00000920: 5a03 4e49 44da 0131 da07 5059 5448 4f4e  Z.NID..1..PYTHON
 00000930: 33da 00da 0454 4558 545a 124e 4f5f 454e  3....TEXTZ.NO_EN
 00000940: 464f 5243 455f 444f 4d41 494e 537a 0b6f  FORCE_DOMAINSz.o
 00000950: 7574 6c69 6e65 2e73 6870 5a0b 5349 4e47  utline.shpZ.SING
 00000960: 4c45 5f50 4152 54fa 0123 da0a 6365 6e74  LE_PART..#..cent
 00000970: 726f 6964 5f78 5a0a 4345 4e54 524f 4944  roid_xZ.CENTROID
 00000980: 5f58 da0a 6365 6e74 726f 6964 5f79 5a0a  _X..centroid_yZ.
 00000990: 4345 4e54 524f 4944 5f59 e9e6 1000 0029  CENTROID_Y.....)
 000009a0: 01da 1163 6f6f 7264 696e 6174 655f 7379  ...coordinate_sy
-000009b0: 7374 656d 290f da05 5348 4150 4572 2900  stem)...SHAPEr).
-000009c0: 0000 722a 0000 0072 2b00 0000 722c 0000  ..r*...r+...r,..
-000009d0: 0072 2d00 0000 722f 0000 0072 3000 0000  .r-...r/...r0...
-000009e0: 7231 0000 0072 2a00 0000 7232 0000 0072  r1...r*...r2...r
-000009f0: 3300 0000 7234 0000 0072 3500 0000 5a0c  3...r4...r5...Z.
+000009b0: 7374 656d 290f da05 5348 4150 4572 2c00  stem)...SHAPEr,.
+000009c0: 0000 722d 0000 0072 2e00 0000 722f 0000  ..r-...r....r/..
+000009d0: 0072 3000 0000 7232 0000 0072 3300 0000  .r0...r2...r3...
+000009e0: 7234 0000 0072 2d00 0000 7235 0000 0072  r4...r-...r5...r
+000009f0: 3600 0000 7237 0000 0072 3800 0000 da0c  6...r7...r8.....
 00000a00: 4f6c 645f 446f 7753 7562 4964 a901 da07  Old_DowSubId....
-00000a10: 636f 6c75 6d6e 7372 2400 0000 722e 0000  columnsr$...r...
-00000a20: 0072 3f00 0000 da04 6c65 6674 a902 da02  .r?.....left....
+00000a10: 636f 6c75 6d6e 7372 2800 0000 7231 0000  columnsr(...r1..
+00000a20: 0072 4200 0000 da04 6c65 6674 a902 da02  .rB.....left....
 00000a30: 6f6e da03 686f 77da 0952 6976 4c65 6e67  on..how..RivLeng
-00000a40: 7468 7201 0000 0072 1900 0000 7a0d 7269  thr....r....z.ri
-00000a50: 765f 6174 7472 692e 7368 7029 1072 2900  v_attri.shp).r).
-00000a60: 0000 722a 0000 0072 2b00 0000 722c 0000  ..r*...r+...r,..
-00000a70: 0072 2d00 0000 722e 0000 0072 2f00 0000  .r-...r....r/...
-00000a80: 7230 0000 0072 3100 0000 722a 0000 0072  r0...r1...r*...r
-00000a90: 3200 0000 7233 0000 0072 3400 0000 7235  2...r3...r4...r5
-00000aa0: 0000 0072 3b00 0000 723c 0000 0029 19da  ...r;...r<...)..
+00000a40: 7468 7201 0000 0072 1700 0000 7a0d 7269  thr....r....z.ri
+00000a50: 765f 6174 7472 692e 7368 7029 1072 2c00  v_attri.shp).r,.
+00000a60: 0000 722d 0000 0072 2e00 0000 722f 0000  ..r-...r....r/..
+00000a70: 0072 3000 0000 7231 0000 0072 3200 0000  .r0...r1...r2...
+00000a80: 7233 0000 0072 3400 0000 722d 0000 0072  r3...r4...r-...r
+00000a90: 3500 0000 7236 0000 0072 3700 0000 7238  5...r6...r7...r8
+00000aa0: 0000 0072 3e00 0000 723f 0000 0029 19da  ...r>...r?...)..
 00000ab0: 0773 7061 7469 616c da0f 746f 5f66 6561  .spatial..to_fea
 00000ac0: 7475 7265 636c 6173 73da 026f 73da 0470  tureclass..os..p
-00000ad0: 6174 68da 046a 6f69 6e72 0f00 0000 da13  ath..joinr......
+00000ad0: 6174 68da 046a 6f69 6e72 0f00 0000 5a13  ath..joinr....Z.
 00000ae0: 4469 7373 6f6c 7665 5f6d 616e 6167 656d  Dissolve_managem
-00000af0: 656e 74da 144a 6f69 6e46 6965 6c64 5f6d  ent..JoinField_m
-00000b00: 616e 6167 656d 656e 74da 1644 656c 6574  anagement..Delet
+00000af0: 656e 745a 144a 6f69 6e46 6965 6c64 5f6d  entZ.JoinField_m
+00000b00: 616e 6167 656d 656e 745a 1644 656c 6574  anagementZ.Delet
 00000b10: 6546 6965 6c64 5f6d 616e 6167 656d 656e  eField_managemen
-00000b20: 74da 0a6d 616e 6167 656d 656e 74da 0e43  t..management..C
+00000b20: 74da 0a6d 616e 6167 656d 656e 745a 0e43  t..managementZ.C
 00000b30: 616c 6375 6c61 7465 4669 656c 64da 0861  alculateField..a
-00000b40: 6e61 6c79 7369 73da 1050 6169 7277 6973  nalysis..Pairwis
-00000b50: 6544 6973 736f 6c76 65da 2643 616c 6375  eDissolve.&Calcu
+00000b40: 6e61 6c79 7369 735a 1050 6169 7277 6973  nalysisZ.Pairwis
+00000b50: 6544 6973 736f 6c76 655a 2643 616c 6375  eDissolveZ&Calcu
 00000b60: 6c61 7465 4765 6f6d 6574 7279 4174 7472  lateGeometryAttr
 00000b70: 6962 7574 6573 5f6d 616e 6167 656d 656e  ibutes_managemen
 00000b80: 74da 1053 7061 7469 616c 5265 6665 7265  t..SpatialRefere
-00000b90: 6e63 6572 4100 0000 721d 0000 00da 0464  ncerA...r......d
+00000b90: 6e63 6572 4500 0000 721f 0000 00da 0464  ncerE...r......d
 00000ba0: 726f 70da 0270 64da 0944 6174 6146 7261  rop..pd..DataFra
 00000bb0: 6d65 da11 6672 6f6d 5f66 6561 7475 7265  me..from_feature
-00000bc0: 636c 6173 73da 056d 6572 6765 721b 0000  class..merger...
+00000bc0: 636c 6173 73da 056d 6572 6765 721d 0000  class..merger...
 00000bd0: 00da 0a6c 6f67 6963 616c 5f6f 7272 0d00  ...logical_orr..
 00000be0: 0000 290c da0e 6d61 706f 6c64 6e65 775f  ..)...mapoldnew_
 00000bf0: 696e 666f da0a 7465 6d70 666f 6c64 6572  info..tempfolder
 00000c00: da0c 4f75 7470 7574 466f 6c64 6572 da08  ..OutputFolder..
 00000c10: 6361 745f 6e61 6d65 da08 7269 765f 6e61  cat_name..riv_na
 00000c20: 6d65 da0e 5061 7468 5f66 696e 616c 5f72  me..Path_final_r
-00000c30: 6976 5a0c 6469 735f 636f 6c5f 6e61 6d65  ivZ.dis_col_name
-00000c40: 5a0a 6361 745f 636f 6c6e 6d73 5a0f 6472  Z.cat_colnmsZ.dr
-00000c50: 6f70 5f63 6174 5f63 6f6c 6e6d 735a 0663  op_cat_colnmsZ.c
-00000c60: 6174 5f70 645a 0672 6976 5f70 6472 2200  at_pdZ.riv_pdr".
-00000c70: 0000 7215 0000 0072 1500 0000 7216 0000  ..r....r....r...
+00000c30: 6976 da0c 6469 735f 636f 6c5f 6e61 6d65  iv..dis_col_name
+00000c40: da0a 6361 745f 636f 6c6e 6d73 da0f 6472  ..cat_colnms..dr
+00000c50: 6f70 5f63 6174 5f63 6f6c 6e6d 73da 0663  op_cat_colnms..c
+00000c60: 6174 5f70 64da 0672 6976 5f70 6472 2600  at_pd..riv_pdr&.
+00000c70: 0000 7213 0000 0072 1300 0000 7214 0000  ..r....r....r...
 00000c80: 00da 2373 6176 655f 6d6f 6469 6669 6564  ..#save_modified
 00000c90: 5f61 7474 7269 6275 7465 735f 746f 5f6f  _attributes_to_o
 00000ca0: 7574 7075 7473 4100 0000 733a 0000 0000  utputsA...s:....
 00000cb0: 021c 0124 0124 0110 0106 ff04 0322 012a  ...$.$.......".*
 00000cc0: 030a 012c 0106 0112 010c 020a 010e 010c  ...,............
 00000cd0: 020c 0112 020e 011c 0108 010e 0110 011c  ................
-00000ce0: 0124 0124 0110 0106 ff72 6100 0000 6302  .$.$.....ra...c.
+00000ce0: 0124 0124 0110 0106 ff72 6400 0000 6302  .$.$.....rd...c.
 00000cf0: 0000 0000 0000 0000 0000 0003 0000 0007  ................
 00000d00: 0000 0043 0000 0073 2a00 0000 7c00 6a00  ...C...s*...|.j.
 00000d10: 7401 a002 7401 a003 7c00 6a00 7c01 a102  t...t...|.j.|...
 00000d20: a101 1900 7d02 7c00 6a04 7c02 6401 8d01  ....}.|.j.|.d...
-00000d30: 7d00 7c00 5300 2902 4e72 4000 0000 2905  }.|.S.).Nr@...).
-00000d40: 7241 0000 0072 1b00 0000 721c 0000 0072  rA...r....r....r
-00000d50: 1d00 0000 7255 0000 0029 03da 0574 6162  ....rU...)...tab
-00000d60: 6c65 da05 6e61 6d65 735a 1372 656d 6f76  le..namesZ.remov
-00000d70: 655f 636f 6c75 6d6e 5f6e 616d 6573 7215  e_column_namesr.
-00000d80: 0000 0072 1500 0000 7216 0000 00da 1b63  ...r....r......c
+00000d30: 7d00 7c00 5300 2902 4e72 4400 0000 2905  }.|.S.).NrD...).
+00000d40: 7245 0000 0072 1d00 0000 721e 0000 0072  rE...r....r....r
+00000d50: 1f00 0000 7253 0000 0029 03da 0574 6162  ....rS...)...tab
+00000d60: 6c65 da05 6e61 6d65 73da 1372 656d 6f76  le..names..remov
+00000d70: 655f 636f 6c75 6d6e 5f6e 616d 6573 7213  e_column_namesr.
+00000d80: 0000 0072 1300 0000 7214 0000 00da 1b63  ...r....r......c
 00000d90: 6c65 616e 5f61 7474 7269 6275 7465 5f6e  lean_attribute_n
 00000da0: 616d 655f 6172 6367 6973 6900 0000 7306  ame_arcgisi...s.
-00000db0: 0000 0000 011a 010c 0172 6400 0000 6301  .........rd...c.
+00000db0: 0000 0000 011a 010c 0172 6800 0000 6301  .........rh...c.
 00000dc0: 0000 0000 0000 0000 0000 001a 0000 000a  ................
 00000dd0: 0000 0043 0000 0073 de03 0000 6401 7400  ...C...s....d.t.
 00000de0: 6a01 5f02 7403 6a04 a005 7c00 a101 7d01  j._.t.j...|...}.
 00000df0: 7403 6a04 a006 7c00 a101 a007 6402 a101  t.j...|.....d...
 00000e00: 7d02 7408 7c02 8301 7d03 7c02 7c03 6403  }.t.|...}.|.|.d.
 00000e10: 1800 1900 6404 6405 8502 1900 7d04 6700  ....d.d.....}.g.
 00000e20: 6406 a201 7d05 6407 7d06 6408 7d07 6409  d...}.d.}.d.}.d.
@@ -288,109 +288,109 @@
 000011f0: ae47 e17a 743f 677b 14ae 47e1 7a84 3f67  .G.zt?g{..G.z.?g
 00001200: 9a99 9999 9999 a93f da0d 6669 6e61 6c63  .......?..finalc
 00001210: 6174 5f69 6e66 6fda 1166 696e 616c 6361  at_info..finalca
 00001220: 745f 696e 666f 5f72 6976 da11 736c 5f63  t_info_riv..sl_c
 00001230: 6f6e 6e65 6374 6564 5f6c 616b 65da 1573  onnected_lake..s
 00001240: 6c5f 6e6f 6e5f 636f 6e6e 6563 7465 645f  l_non_connected_
 00001250: 6c61 6b65 da01 767a 042e 7368 707a 082e  lake..vz..shpz..
-00001260: 6765 6f6a 736f 6e5a 0e63 6f6e 6e65 6374  geojsonZ.connect
+00001260: 6765 6f6a 736f 6eda 0e63 6f6e 6e65 6374  geojson..connect
 00001270: 6564 5f6c 616b 657a 1069 6e70 7574 5f77  ed_lakez.input_w
-00001280: 6773 5f38 342e 7368 7072 3d00 0000 5a07  gs_84.shpr=...Z.
-00001290: 7276 684e 616d 6572 3900 0000 7a1b 2773  rvhNamer9...z.'s
+00001280: 6773 5f38 342e 7368 7072 4000 0000 da07  gs_84.shpr@.....
+00001290: 7276 684e 616d 6572 3c00 0000 7a1b 2773  rvhNamer<...z.'s
 000012a0: 7562 2720 2b20 7374 7228 696e 7428 2221  ub' + str(int("!
-000012b0: 5375 6249 6421 2229 2972 3700 0000 7a19  SubId!"))r7...z.
+000012b0: 5375 6249 6421 2229 2972 3a00 0000 7a19  SubId!"))r:...z.
 000012c0: 696e 7075 745f 7767 735f 3834 5f73 696d  input_wgs_84_sim
 000012d0: 706c 6966 792e 7368 705a 0c50 4f49 4e54  plify.shpZ.POINT
 000012e0: 5f52 454d 4f56 455a 0946 4f52 4d41 5454  _REMOVEZ.FORMATT
 000012f0: 4544 5a0b 4e4f 5f5a 5f56 414c 5545 535a  EDZ.NO_Z_VALUESZ
-00001300: 0b4e 4f5f 4d5f 5641 4c55 4553 da07 4745  .NO_M_VALUES..GE
+00001300: 0b4e 4f5f 4d5f 5641 4c55 4553 5a07 4745  .NO_M_VALUESZ.GE
 00001310: 4f4a 534f 4e69 0004 0000 e964 0000 0069  OJSONi.....d...i
 00001320: f401 0000 da08 6665 6174 7572 6573 da0a  ......features..
-00001330: 7072 6f70 6572 7469 6573 7219 0000 007a  propertiesr....z
+00001330: 7072 6f70 6572 7469 6573 7217 0000 007a  propertiesr....z
 00001340: 2272 6f75 7469 6e67 5f70 726f 6475 6374  "routing_product
 00001350: 5f6c 616b 655f 7269 7665 722e 6765 6f6a  _lake_river.geoj
 00001360: 736f 6eda 0177 7a05 7574 662d 3829 01da  son..wz.utf-8)..
 00001370: 0865 6e63 6f64 696e 6746 2902 da0c 656e  .encodingF)...en
 00001380: 7375 7265 5f61 7363 6969 da06 696e 6465  sure_ascii..inde
 00001390: 6e74 2923 720f 0000 0072 0500 0000 da0f  nt)#r....r......
 000013a0: 6f76 6572 7772 6974 654f 7574 7075 7472  overwriteOutputr
-000013b0: 4900 0000 724a 0000 00da 0764 6972 6e61  I...rJ.....dirna
+000013b0: 4d00 0000 724e 0000 00da 0764 6972 6e61  M...rN.....dirna
 000013c0: 6d65 da08 6261 7365 6e61 6d65 da05 7370  me..basename..sp
-000013d0: 6c69 7472 0d00 0000 720c 0000 0072 4b00  litr....r....rK.
+000013d0: 6c69 7472 0d00 0000 720c 0000 0072 4f00  litr....r....rO.
 000013e0: 0000 da06 6578 6973 7473 da06 6170 7065  ....exists..appe
 000013f0: 6e64 da08 7465 6d70 6669 6c65 da0a 6765  nd..tempfile..ge
 00001400: 7474 656d 7064 6972 da12 5072 6f6a 6563  ttempdir..Projec
-00001410: 745f 6d61 6e61 6765 6d65 6e74 7254 0000  t_managementrT..
-00001420: 00da 0369 6e74 da13 4164 6446 6965 6c64  ...int..AddField
-00001430: 5f6d 616e 6167 656d 656e 74da 1943 616c  _management..Cal
+00001410: 745f 6d61 6e61 6765 6d65 6e74 7252 0000  t_managementrR..
+00001420: 00da 0369 6e74 5a13 4164 6446 6965 6c64  ...intZ.AddField
+00001430: 5f6d 616e 6167 656d 656e 745a 1943 616c  _managementZ.Cal
 00001440: 6375 6c61 7465 4669 656c 645f 6d61 6e61  culateField_mana
-00001450: 6765 6d65 6e74 da19 5265 7061 6972 4765  gement..RepairGe
+00001450: 6765 6d65 6e74 5a19 5265 7061 6972 4765  gementZ.RepairGe
 00001460: 6f6d 6574 7279 5f6d 616e 6167 656d 656e  ometry_managemen
-00001470: 74da 0645 7869 7374 73da 1144 656c 6574  t..Exists..Delet
+00001470: 745a 0645 7869 7374 735a 1144 656c 6574  tZ.ExistsZ.Delet
 00001480: 655f 6d61 6e61 6765 6d65 6e74 da02 4341  e_management..CA
-00001490: da0f 5369 6d70 6c69 6679 506f 6c79 676f  ..SimplifyPolygo
-000014a0: 6eda 0c53 696d 706c 6966 794c 696e 65da  n..SimplifyLine.
+00001490: 5a0f 5369 6d70 6c69 6679 506f 6c79 676f  Z.SimplifyPolygo
+000014a0: 6e5a 0c53 696d 706c 6966 794c 696e 655a  nZ.SimplifyLineZ
 000014b0: 1946 6561 7475 7265 7354 6f4a 534f 4e5f  .FeaturesToJSON_
 000014c0: 636f 6e76 6572 7369 6f6e da04 7374 6174  conversion..stat
 000014d0: da07 7374 5f73 697a 6572 0700 0000 da04  ..st_sizer......
 000014e0: 6f70 656e da04 6a73 6f6e da04 6475 6d70  open..json..dump
 000014f0: da06 7368 7574 696c da04 636f 7079 291a  ..shutil..copy).
-00001500: 5a12 496e 7075 745f 506f 6c79 676f 6e5f  Z.Input_Polygon_
-00001510: 7061 7468 5a0b 7072 6f64 7563 745f 6469  pathZ.product_di
-00001520: 725a 084e 616d 6573 5f69 6e5a 076e 5f63  rZ.Names_inZ.n_c
-00001530: 6861 7263 da07 7665 7273 696f 6e5a 0a54  harc..versionZ.T
-00001540: 4f4c 4552 414e 4345 735a 0d68 6561 645f  OLERANCEsZ.head_
-00001550: 6e61 6d65 5f63 6174 5a0d 6865 6164 5f6e  name_catZ.head_n
-00001560: 616d 655f 7269 765a 0f68 6561 645f 6e61  ame_rivZ.head_na
-00001570: 6d65 5f73 6c61 6b65 5a0f 6865 6164 5f6e  me_slakeZ.head_n
-00001580: 616d 655f 6e6c 616b 655a 0f49 6e70 7574  ame_nlakeZ.Input
-00001590: 5f66 696c 655f 6e61 6d65 5a10 4f75 7470  _file_nameZ.Outp
-000015a0: 7574 5f66 696c 655f 6e61 6d65 5a13 6372  ut_file_nameZ.cr
+00001500: da12 496e 7075 745f 506f 6c79 676f 6e5f  ..Input_Polygon_
+00001510: 7061 7468 da0b 7072 6f64 7563 745f 6469  path..product_di
+00001520: 72da 084e 616d 6573 5f69 6eda 076e 5f63  r..Names_in..n_c
+00001530: 6861 7263 da07 7665 7273 696f 6eda 0a54  harc..version..T
+00001540: 4f4c 4552 414e 4345 73da 0d68 6561 645f  OLERANCEs..head_
+00001550: 6e61 6d65 5f63 6174 da0d 6865 6164 5f6e  name_cat..head_n
+00001560: 616d 655f 7269 76da 0f68 6561 645f 6e61  ame_riv..head_na
+00001570: 6d65 5f73 6c61 6b65 da0f 6865 6164 5f6e  me_slake..head_n
+00001580: 616d 655f 6e6c 616b 65da 0f49 6e70 7574  ame_nlake..Input
+00001590: 5f66 696c 655f 6e61 6d65 da10 4f75 7470  _file_name..Outp
+000015a0: 7574 5f66 696c 655f 6e61 6d65 da13 6372  ut_file_name..cr
 000015b0: 6561 7465 645f 6a61 736f 6e5f 6669 6c65  eated_jason_file
-000015c0: 735a 1c63 7265 6174 6564 5f6a 6173 6f6e  sZ.created_jason
+000015c0: 73da 1c63 7265 6174 6564 5f6a 6173 6f6e  s..created_jason
 000015d0: 5f66 696c 6573 5f6c 616b 655f 7269 7672  _files_lake_rivr
-000015e0: 1400 0000 da0a 696e 7075 745f 7061 7468  ......input_path
-000015f0: 5a11 6f75 7470 7574 5f6a 6173 6f6e 5f70  Z.output_jason_p
-00001600: 6174 685a 0c69 6e70 7574 5f77 6773 5f38  athZ.input_wgs_8
-00001610: 345a 0954 4f4c 4552 414e 4345 5a15 696e  4Z.TOLERANCEZ.in
+000015e0: 1200 0000 da0a 696e 7075 745f 7061 7468  ......input_path
+000015f0: da11 6f75 7470 7574 5f6a 6173 6f6e 5f70  ..output_jason_p
+00001600: 6174 68da 0c69 6e70 7574 5f77 6773 5f38  ath..input_wgs_8
+00001610: 34da 0954 4f4c 4552 414e 4345 5a15 696e  4..TOLERANCEZ.in
 00001620: 7075 745f 7767 735f 3834 5f73 696d 706c  put_wgs_84_simpl
-00001630: 6966 795a 0e6a 736f 6e5f 6669 6c65 5f73  ifyZ.json_file_s
-00001640: 697a 655a 0769 6e6a 736f 6e32 5a0c 6e65  izeZ.injson2Z.ne
+00001630: 6966 79da 0e6a 736f 6e5f 6669 6c65 5f73  ify..json_file_s
+00001640: 697a 65da 0769 6e6a 736f 6e32 da0c 6e65  ize..injson2..ne
 00001650: 775f 6665 6174 7572 6573 da07 656c 656d  w_features..elem
-00001660: 656e 745a 156f 7574 7075 745f 6a61 736f  entZ.output_jaso
-00001670: 6e5f 6c61 6b65 5f72 6976 da01 6672 1500  n_lake_riv..fr..
-00001680: 0000 7215 0000 0072 1600 0000 da15 6372  ..r....r......cr
+00001660: 656e 74da 156f 7574 7075 745f 6a61 736f  ent..output_jaso
+00001670: 6e5f 6c61 6b65 5f72 6976 da01 6672 1300  n_lake_riv..fr..
+00001680: 0000 7213 0000 0072 1400 0000 da15 6372  ..r....r......cr
 00001690: 6561 7465 5f67 656f 5f6a 6173 6f6e 5f66  eate_geo_jason_f
 000016a0: 696c 6570 0000 0073 9c00 0000 0002 0801  ilep...s........
 000016b0: 0c01 1201 0801 1401 0803 0401 0401 0401  ................
 000016c0: 0402 0401 0401 0802 0e01 0e01 0e01 0efc  ................
 000016d0: 0407 0e01 0e01 0e01 0efc 0608 0601 0601  ................
 000016e0: 0601 06fc 0407 0601 0601 0601 06fc 0406  ................
 000016f0: 0401 0402 1401 1201 1201 0e01 0401 0a02  ................
 00001700: 1c01 0a03 1201 1803 1c01 0e01 1002 0a02  ................
 00001710: 0801 1201 0c01 0a03 0e01 1202 1002 0601  ................
 00001720: 0aff 0403 1401 0a01 0e02 3601 1201 1001  ..........6.....
 00001730: 0e01 0401 0c01 1201 0e01 0802 0a01 0602  ................
-00001740: 1802 1a01 3402 1a04 7293 0000 0063 0300  ....4...r....c..
+00001740: 1802 1a01 3402 1a04 72a4 0000 0063 0300  ....4...r....c..
 00001750: 0000 0000 0000 0000 0000 0500 0000 0400  ................
 00001760: 0000 4300 0000 732e 0000 0074 006a 01a0  ..C...s....t.j..
 00001770: 027c 0264 01a1 0274 036a 045f 0574 036a  .|.d...t.j._.t.j
 00001780: 06a0 077c 007c 01a1 027d 0374 08a0 097c  ...|.|...}.t...|
 00001790: 03a1 017d 047c 0453 0029 024e fa0a 6172  ...}.|.S.).N..ar
-000017a0: 6367 6973 2e67 6462 290a 7249 0000 0072  cgis.gdb).rI...r
-000017b0: 4a00 0000 724b 0000 0072 0f00 0000 7205  J...rK...r....r.
+000017a0: 6367 6973 2e67 6462 290a 724d 0000 0072  cgis.gdb).rM...r
+000017b0: 4e00 0000 724f 0000 0072 0f00 0000 7205  N...rO...r....r.
 000017c0: 0000 00da 0977 6f72 6b73 7061 6365 da02  .....workspace..
-000017d0: 6461 da11 5461 626c 6554 6f4e 756d 5079  da..TableToNumPy
-000017e0: 4172 7261 7972 5600 0000 7257 0000 0029  ArrayrV...rW...)
-000017f0: 0572 6200 0000 da09 636f 6c5f 6e61 6d65  .rb.....col_name
+000017d0: 6461 5a11 5461 626c 6554 6f4e 756d 5079  daZ.TableToNumPy
+000017e0: 4172 7261 7972 5400 0000 7255 0000 0029  ArrayrT...rU...)
+000017f0: 0572 6500 0000 da09 636f 6c5f 6e61 6d65  .re.....col_name
 00001800: 73da 0b77 6f72 6b5f 666f 6c64 6572 da03  s..work_folder..
-00001810: 6172 72da 0264 6672 1500 0000 7215 0000  arr..dfr....r...
-00001820: 0072 1600 0000 da14 7265 6164 5f74 6162  .r......read_tab
+00001810: 6172 72da 0264 6672 1300 0000 7213 0000  arr..dfr....r...
+00001820: 0072 1400 0000 da14 7265 6164 5f74 6162  .r......read_tab
 00001830: 6c65 5f61 735f 7061 6e64 6173 dd00 0000  le_as_pandas....
-00001840: 7308 0000 0000 0112 010e 010a 0172 9c00  s............r..
+00001840: 7308 0000 0000 0112 010e 010a 0172 ac00  s............r..
 00001850: 0000 6308 0000 0000 0000 0000 0000 0010  ..c.............
 00001860: 0000 0008 0000 0043 0000 0073 0802 0000  .......C...s....
 00001870: 7400 6a01 a002 7c06 6401 a102 7403 6a04  t.j...|.d...t.j.
 00001880: 5f05 6402 7403 6a04 5f06 7c04 7403 6a04  _.d.t.j._.|.t.j.
 00001890: 5f07 7c04 7403 6a03 6a04 5f08 7403 a009  _.|.t.j.j._.t...
 000018a0: 740a 7c05 6a0b 8301 a101 7403 6a04 5f0c  t.|.j.....t.j._.
 000018b0: 7403 a00d 7c07 a101 6a0e 7403 6a04 5f0e  t...|...j.t.j._.
@@ -417,69 +417,69 @@
 00001a00: 7c03 6411 6b02 9001 72ac 7c0f 6a20 6408  |.d.k...r.|.j d.
 00001a10: 6701 6412 6413 8d02 7d0f 6e10 7c0f 6a20  g.d.d...}.n.|.j 
 00001a20: 6408 6701 6414 6413 8d02 7d0f 7c0f 6a17  d.g.d.d...}.|.j.
 00001a30: 6a21 7400 6a01 a002 7c06 6401 7c02 6407  j!t.j...|.d.|.d.
 00001a40: 1700 a103 6402 6415 6416 8d03 0100 7403  ....d.d.d.....t.
 00001a50: a022 7c02 6407 1700 6408 7c02 6406 1700  ."|.d...d.|.d...
 00001a60: a103 0100 7c02 6406 1700 7c02 6407 1700  ....|.d...|.d...
-00001a70: 6602 5300 6400 5300 2917 4e72 9400 0000  f.S.d.S.).Nr....
+00001a70: 6602 5300 6400 5300 2917 4e72 a500 0000  f.S.d.S.).Nr....
 00001a80: 54da 0556 414c 5545 da06 4e4f 4441 5441  T..VALUE..NODATA
 00001a90: 678d edb5 a0f7 c6b0 3eda 025f 72da 025f  g.......>.._r.._
 00001aa0: 76da 0967 7269 645f 636f 6465 7201 0000  v..grid_coder...
-00001ab0: 00da 044e 4f4e 4572 6c00 0000 7a07 6c6f  ...NONErl...z.lo
+00001ab0: 00da 044e 4f4e 4572 7000 0000 7a07 6c6f  ...NONErp...z.lo
 00001ac0: 672e 7478 74da 0161 7a32 4368 6563 6b20  g.txt..az2Check 
 00001ad0: 5375 6249 6420 616e 6420 446f 776e 5375  SubId and DownSu
 00001ae0: 6249 6420 6f66 2066 6f6c 6c6f 7769 6e67  bId of following
 00001af0: 2073 7562 6261 7369 6e73 200a 7a03 2569   subbasins .z.%i
-00001b00: 0a29 02da 0262 79da 0961 7363 656e 6469  .)...by..ascendi
+00001b00: 0aa9 02da 0262 79da 0961 7363 656e 6469  .....by..ascendi
 00001b10: 6e67 da07 4d41 5849 4d55 4dda 046c 6173  ng..MAXIMUM..las
-00001b20: 7429 02da 0673 7562 7365 74da 046b 6565  t)...subset..kee
-00001b30: 70da 0566 6972 7374 4672 2500 0000 2923  p..firstFr%...)#
-00001b40: 7249 0000 0072 4a00 0000 724b 0000 0072  rI...rJ...rK...r
-00001b50: 0f00 0000 7205 0000 0072 9500 0000 7275  ....r....r....ru
+00001b20: 74a9 02da 0673 7562 7365 74da 046b 6565  t....subset..kee
+00001b30: 70da 0566 6972 7374 4672 2900 0000 2923  p..firstFr)...)#
+00001b40: 724d 0000 0072 4e00 0000 724f 0000 0072  rM...rN...rO...r
+00001b50: 0f00 0000 7205 0000 0072 a600 0000 727a  ....r....r....rz
 00001b60: 0000 00da 0b58 5954 6f6c 6572 616e 6365  .....XYTolerance
-00001b70: da08 6365 6c6c 5369 7a65 7254 0000 0072  ..cellSizerT...r
-00001b80: 7e00 0000 da0b 6661 6374 6f72 7943 6f64  ~.....factoryCod
+00001b70: da08 6365 6c6c 5369 7a65 7252 0000 0072  ..cellSizerR...r
+00001b80: 8300 0000 da0b 6661 6374 6f72 7943 6f64  ......factoryCod
 00001b90: 65da 166f 7574 7075 7443 6f6f 7264 696e  e..outputCoordin
 00001ba0: 6174 6553 7973 7465 6dda 0844 6573 6372  ateSystem..Descr
 00001bb0: 6962 65da 0665 7874 656e 74da 0a73 6e61  ibe..extent..sna
-00001bc0: 7052 6173 7465 72da 0f5a 6f6e 616c 5374  pRaster..ZonalSt
-00001bd0: 6174 6973 7469 6373 da03 436f 6eda 0341  atistics..Con..A
+00001bc0: 7052 6173 7465 725a 0f5a 6f6e 616c 5374  pRasterZ.ZonalSt
+00001bd0: 6174 6973 7469 6373 da03 436f 6e5a 0341  atistics..ConZ.A
 00001be0: 6273 da04 7361 7665 da18 5261 7374 6572  bs..save..Raster
 00001bf0: 546f 506f 696e 745f 636f 6e76 6572 7369  ToPoint_conversi
-00001c00: 6f6e 7256 0000 0072 5700 0000 7247 0000  onrV...rW...rG..
-00001c10: 0072 5800 0000 da0a 6475 706c 6963 6174  .rX.....duplicat
+00001c00: 6f6e 7254 0000 0072 5500 0000 724b 0000  onrT...rU...rK..
+00001c10: 0072 5600 0000 da0a 6475 706c 6963 6174  .rV.....duplicat
 00001c20: 6564 720d 0000 00da 1a45 7874 7261 6374  edr......Extract
 00001c30: 4d75 6c74 6956 616c 7565 7354 6f50 6f69  MultiValuesToPoi
-00001c40: 6e74 7372 8a00 0000 da05 7772 6974 65da  ntsr......write.
+00001c40: 6e74 7372 8700 0000 da05 7772 6974 65da  ntsr......write.
 00001c50: 0676 616c 7565 73da 0b73 6f72 745f 7661  .values..sort_va
 00001c60: 6c75 6573 da0f 6472 6f70 5f64 7570 6c69  lues..drop_dupli
-00001c70: 6361 7465 7372 4800 0000 da18 506f 696e  catesrH.....Poin
+00001c70: 6361 7465 7372 4c00 0000 5a18 506f 696e  catesrL...Z.Poin
 00001c80: 7454 6f52 6173 7465 725f 636f 6e76 6572  tToRaster_conver
 00001c90: 7369 6f6e 2910 5a0c 7a6f 6e61 6c5f 7261  sion).Z.zonal_ra
 00001ca0: 7374 6572 5a0a 7661 6c5f 7261 7374 6572  sterZ.val_raster
-00001cb0: 5a07 6f75 746e 616d 65da 0f73 7461 7469  Z.outname..stati
-00001cc0: 7374 6963 735f 7479 7065 72ac 0000 00da  stics_typer.....
-00001cd0: 0953 7074 6169 6c52 6566 7299 0000 0072  .SptailRefr....r
-00001ce0: b100 0000 5a14 6d61 7861 6363 5f76 616c  ....Z.maxacc_val
+00001cb0: 5a07 6f75 746e 616d 655a 0f73 7461 7469  Z.outnameZ.stati
+00001cc0: 7374 6963 735f 7479 7065 72be 0000 00da  stics_typer.....
+00001cd0: 0953 7074 6169 6c52 6566 72a9 0000 0072  .SptailRefr....r
+00001ce0: c300 0000 5a14 6d61 7861 6363 5f76 616c  ....Z.maxacc_val
 00001cf0: 7565 5f69 6e5f 7a6f 6e65 5a0d 6f75 746c  ue_in_zoneZ.outl
 00001d00: 6574 5f70 6f69 6e74 735a 076f 7574 6c65  et_pointsZ.outle
 00001d10: 7473 5a0a 6475 706c 695f 6d61 736b 5a0b  tsZ.dupli_maskZ.
 00001d20: 6f75 746c 6574 735f 6475 705a 076c 6f67  outlets_dupZ.log
 00001d30: 6669 6c65 da04 6974 656d 5a09 6f75 746c  file..itemZ.outl
-00001d40: 6574 735f 6e72 1500 0000 7215 0000 0072  ets_nr....r....r
-00001d50: 1600 0000 da31 6669 6e64 5f7a 6f6e 616c  .....1find_zonal
+00001d40: 6574 735f 6e72 1300 0000 7213 0000 0072  ets_nr....r....r
+00001d50: 1400 0000 da31 6669 6e64 5f7a 6f6e 616c  .....1find_zonal
 00001d60: 5f6d 6178 696d 756d 5f6f 725f 6d69 6e69  _maximum_or_mini
 00001d70: 6d75 6d5f 706f 696e 745f 6f6e 5f74 6865  mum_point_on_the
 00001d80: 5f72 6173 7465 72e4 0000 0073 4000 0000  _raster....s@...
 00001d90: 0001 1201 0801 0801 0a01 1401 1001 0802  ................
 00001da0: 0801 04ff 0402 1601 0e01 1601 1203 0c01  ................
 00001db0: 0801 0c01 1601 1002 1601 0a01 0e01 3203  ..............2.
 00001dc0: 1602 1201 0e01 0a01 1202 1001 2201 1603  ............"...
-00001dd0: 72c1 0000 0063 0900 0000 0000 0000 0000  r....c..........
+00001dd0: 72cf 0000 0063 0900 0000 0000 0000 0000  r....c..........
 00001de0: 0000 0e00 0000 0a00 0000 4300 0000 73bc  ..........C...s.
 00001df0: 0200 0074 006a 01a0 027c 0764 01a1 0274  ...t.j...|.d...t
 00001e00: 036a 045f 0564 0274 036a 045f 067c 0574  .j._.d.t.j._.|.t
 00001e10: 036a 045f 077c 0574 036a 036a 045f 0874  .j._.|.t.j.j._.t
 00001e20: 03a0 0974 0a7c 066a 0b83 01a1 0174 036a  ...t.|.j.....t.j
 00001e30: 045f 0c74 03a0 0d7c 08a1 016a 0e74 036a  ._.t...|...j.t.j
 00001e40: 045f 0e7c 0874 036a 045f 0f74 03a0 107c  ._.|.t.j._.t...|
@@ -517,81 +517,81 @@
 00002040: 0074 03a0 227c 0164 2017 007c 0264 2419  .t.."|.d ..|.d$.
 00002050: 007c 0164 2517 0064 2664 007c 08a1 0601  .|.d%..d&d.|....
 00002060: 0074 03a0 237c 0364 2017 007c 0264 2419  .t..#|.d ..|.d$.
 00002070: 007c 0364 2717 0064 2864 007c 08a1 0601  .|.d'..d(d.|....
 00002080: 0074 2474 257c 0364 2717 0083 017c 0164  .t$t%|.d'....|.d
 00002090: 2517 007c 0364 2717 0083 037d 0d7c 0da0  %..|.d'....}.|..
 000020a0: 267c 0164 2717 00a1 0101 0064 0053 0029  &|.d'......d.S.)
-000020b0: 294e 7294 0000 0054 7a0d 6c61 6b65 5f70  )Nr....Tz.lake_p
-000020c0: 726f 6a2e 7368 705a 045f 706c 79da 055f  roj.shpZ._ply.._
+000020b0: 294e 72a5 0000 0054 7a0d 6c61 6b65 5f70  )Nr....Tz.lake_p
+000020c0: 726f 6a2e 7368 70da 045f 706c 79da 055f  roj.shp.._ply.._
 000020d0: 6c69 6e65 7a0c 6d61 736b 5f70 6c79 2e73  linez.mask_ply.s
 000020e0: 6870 e700 0000 0000 00e0 3ffa 0820 204d  hp........?..  M
 000020f0: 6574 6572 735a 0446 554c 4c5a 0552 4f55  etersZ.FULLZ.ROU
-00002100: 4e44 72a2 0000 00da 0650 4c41 4e41 527a  NDr......PLANARz
-00002110: 0d6e 6577 6172 6561 3120 4152 4541 7238  .newarea1 AREAr8
+00002100: 4e44 72b2 0000 00da 0650 4c41 4e41 527a  NDr......PLANARz
+00002110: 0d6e 6577 6172 6561 3120 4152 4541 723b  .newarea1 AREAr;
 00002120: 0000 005a 1153 5155 4152 455f 4b49 4c4f  ...Z.SQUARE_KILO
 00002130: 4d45 5445 5253 5a0d 5341 4d45 5f41 535f  METERSZ.SAME_AS_
 00002140: 494e 5055 547a 0d6c 616b 655f 636c 6970  INPUTz.lake_clip
 00002150: 2e73 6870 7a0d 6e65 7761 7265 6130 2041  .shpz.newarea0 A
 00002160: 5245 417a 106c 616b 655f 636c 6970 5f62  REAz.lake_clip_b
-00002170: 662e 7368 7072 6600 0000 7267 0000 00da  f.shprf...rg....
-00002180: 0847 454f 4445 5349 43a9 04da 0b69 6e5f  .GEODESIC....in_
-00002190: 6665 6174 7572 6573 da11 6f75 745f 6665  features..out_fe
-000021a0: 6174 7572 655f 636c 6173 73da 1862 7566  ature_class..buf
+00002170: 662e 7368 7072 6a00 0000 726b 0000 005a  f.shprj...rk...Z
+00002180: 0847 454f 4445 5349 43a9 045a 0b69 6e5f  .GEODESIC..Z.in_
+00002190: 6665 6174 7572 6573 5a11 6f75 745f 6665  featuresZ.out_fe
+000021a0: 6174 7572 655f 636c 6173 735a 1862 7566  ature_classZ.buf
 000021b0: 6665 725f 6469 7374 616e 6365 5f6f 725f  fer_distance_or_
 000021c0: 6669 656c 64da 066d 6574 686f 647a 156c  field..methodz.l
 000021d0: 616b 655f 636c 6970 5f62 665f 636c 6970  ake_clip_bf_clip
 000021e0: 2e73 6870 5a11 6c61 6b65 5f63 6c69 705f  .shpZ.lake_clip_
 000021f0: 6266 5f63 6c69 705a 086e 6577 6172 6561  bf_clipZ.newarea
 00002200: 305a 086e 6577 6172 6561 315a 0a61 7265  0Z.newarea1Z.are
 00002210: 615f 7261 7469 6f67 9a99 9999 9999 f13f  a_ratiog.......?
 00002220: 67cd cccc cccc ccec 3fa9 01da 0464 6565  g.......?....dee
-00002230: 7072 a000 0000 4672 2500 0000 7a0c 302e  pr....Fr%...z.0.
+00002230: 7072 b000 0000 4672 2900 0000 7a0c 302e  pr....Fr)...z.0.
 00002240: 3030 3120 4d65 7465 7273 7201 0000 005a  001 Metersr....Z
 00002250: 035f 7274 da15 4d41 5849 4d55 4d5f 434f  ._rt..MAXIMUM_CO
-00002260: 4d42 494e 4544 5f41 5245 4172 9f00 0000  MBINED_AREAr....
+00002260: 4d42 494e 4544 5f41 5245 4172 af00 0000  MBINED_AREAr....
 00002270: 5a17 4d41 5849 4d55 4d5f 434f 4d42 494e  Z.MAXIMUM_COMBIN
-00002280: 4544 5f4c 454e 4754 4829 2772 4900 0000  ED_LENGTH)'rI...
-00002290: 724a 0000 0072 4b00 0000 720f 0000 0072  rJ...rK...r....r
-000022a0: 0500 0000 7295 0000 0072 7500 0000 72ab  ....r....ru...r.
-000022b0: 0000 0072 ac00 0000 7254 0000 0072 7e00  ...r....rT...r~.
-000022c0: 0000 72ad 0000 0072 ae00 0000 72af 0000  ..r....r....r...
-000022d0: 0072 b000 0000 72b1 0000 0072 7d00 0000  .r....r....r}...
-000022e0: da18 4665 6174 7572 6554 6f4c 696e 655f  ..FeatureToLine_
+00002280: 4544 5f4c 454e 4754 4829 2772 4d00 0000  ED_LENGTH)'rM...
+00002290: 724e 0000 0072 4f00 0000 720f 0000 0072  rN...rO...r....r
+000022a0: 0500 0000 72a6 0000 0072 7a00 0000 72bd  ....r....rz...r.
+000022b0: 0000 0072 be00 0000 7252 0000 0072 8300  ...r....rR...r..
+000022c0: 0000 72bf 0000 0072 c000 0000 72c1 0000  ..r....r....r...
+000022d0: 0072 c200 0000 72c3 0000 0072 8200 0000  .r....r....r....
+000022e0: 5a18 4665 6174 7572 6554 6f4c 696e 655f  Z.FeatureToLine_
 000022f0: 6d61 6e61 6765 6d65 6e74 7251 0000 00da  managementrQ....
-00002300: 0642 7566 6665 7272 0e00 0000 724f 0000  .Bufferr....rO..
-00002310: 00da 1b43 616c 6375 6c61 7465 4765 6f6d  ...CalculateGeom
-00002320: 6574 7279 4174 7472 6962 7574 6573 da0c  etryAttributes..
+00002300: 0642 7566 6665 7272 0e00 0000 7250 0000  .Bufferr....rP..
+00002310: 005a 1b43 616c 6375 6c61 7465 4765 6f6d  .Z.CalculateGeom
+00002320: 6574 7279 4174 7472 6962 7574 6573 5a0c  etryAttributesZ.
 00002330: 5061 6972 7769 7365 436c 6970 da0a 636f  PairwiseClip..co
-00002340: 6e76 6572 7369 6f6e da19 4665 6174 7572  nversion..Featur
+00002340: 6e76 6572 7369 6f6e 5a19 4665 6174 7572  nversionZ.Featur
 00002350: 6543 6c61 7373 546f 4765 6f64 6174 6162  eClassToGeodatab
-00002360: 6173 6572 5600 0000 7257 0000 0072 4700  aserV...rW...rG.
-00002370: 0000 7258 0000 0072 1b00 0000 721e 0000  ..rX...r....r...
-00002380: 0072 8e00 0000 7248 0000 00da 1a50 6f6c  .r....rH.....Pol
+00002360: 6173 6572 5400 0000 7255 0000 0072 4b00  aserT...rU...rK.
+00002370: 0000 7256 0000 0072 1d00 0000 7220 0000  ..rV...r....r ..
+00002380: 0072 8b00 0000 724c 0000 00da 1a50 6f6c  .r....rL.....Pol
 00002390: 7967 6f6e 546f 5261 7374 6572 5f63 6f6e  ygonToRaster_con
-000023a0: 7665 7273 696f 6eda 1b50 6f6c 796c 696e  version..Polylin
+000023a0: 7665 7273 696f 6e5a 1b50 6f6c 796c 696e  versionZ.Polylin
 000023b0: 6554 6f52 6173 7465 725f 636f 6e76 6572  eToRaster_conver
-000023c0: 7369 6f6e 72b3 0000 00da 0649 734e 756c  sionr......IsNul
-000023d0: 6c72 b500 0000 290e da10 7061 7468 5f6c  lr....)...path_l
+000023c0: 7369 6f6e 72c4 0000 00da 0649 734e 756c  sionr......IsNul
+000023d0: 6c72 c500 0000 290e da10 7061 7468 5f6c  lr....)...path_l
 000023e0: 616b 6566 696c 655f 696e da07 616c 6c6c  akefile_in..alll
 000023f0: 616b 65da 0f6c 616b 655f 6174 7472 6962  ake..lake_attrib
 00002400: 7574 6573 da0d 6c61 6b65 5f62 6f75 6e64  utes..lake_bound
-00002410: 6172 7972 2200 0000 72ac 0000 0072 bf00  aryr"...r....r..
-00002420: 0000 7299 0000 0072 b100 0000 5a10 616c  ..r....r....Z.al
-00002430: 6c5f 636c 6970 6564 5f6c 616b 6573 7220  l_cliped_lakesr 
-00002440: 0000 0072 2100 0000 5a0b 7365 6c65 6374  ...r!...Z.select
-00002450: 5f6c 616b 655a 064f 7574 5261 7372 1500  _lakeZ.OutRasr..
-00002460: 0000 7215 0000 0072 1600 0000 da18 7072  ..r....r......pr
+00002410: 6172 7972 2600 0000 72be 0000 0072 cd00  aryr&...r....r..
+00002420: 0000 72a9 0000 0072 c300 0000 5a10 616c  ..r....r....Z.al
+00002430: 6c5f 636c 6970 6564 5f6c 616b 6573 7224  l_cliped_lakesr$
+00002440: 0000 0072 2500 0000 5a0b 7365 6c65 6374  ...r%...Z.select
+00002450: 5f6c 616b 655a 064f 7574 5261 7372 1300  _lakeZ.OutRasr..
+00002460: 0000 7213 0000 0072 1400 0000 da18 7072  ..r....r......pr
 00002470: 655f 7072 6f63 6573 735f 6c61 6b65 5f70  e_process_lake_p
 00002480: 6f6c 7967 6f6e 1001 0000 734a 0000 0000  olygon....sJ....
 00002490: 0212 0108 0108 010a 0114 0110 0108 0204  ................
 000024a0: 0102 010c 010e fd04 0514 0236 0220 0130  ...........6. .0
 000024b0: 0220 0138 0130 0222 040e 0114 010c 010c  . .8.0."........
 000024c0: 010c 0110 0222 0116 0216 0106 ff04 0216  ....."..........
-000024d0: 0106 ff04 031c 010e 0472 dc00 0000 630d  .........r....c.
+000024d0: 0106 ff04 031c 010e 0472 e200 0000 630d  .........r....c.
 000024e0: 0000 0000 0000 0000 0000 0021 0000 0007  ...........!....
 000024f0: 0000 0043 0000 0073 c202 0000 7400 6a01  ...C...s....t.j.
 00002500: a002 7c0b 6401 a102 7403 6a04 5f05 6402  ..|.d...t.j._.d.
 00002510: 7403 6a04 5f06 7c09 7403 6a04 5f07 7c09  t.j._.|.t.j._.|.
 00002520: 7403 6a03 6a04 5f08 7403 a009 740a 7c0a  t.j.j._.t...t.|.
 00002530: 6a0b 8301 a101 7403 6a04 5f0c 7403 a00d  j.....t.j._.t...
 00002540: 7c0c a101 6a0e 7403 6a04 5f0e 7c0c 7403  |...j.t.j._.|.t.
@@ -630,71 +630,71 @@
 00002750: 6402 640a 8d01 7d1f 7c1f 6a1e 6a24 7400  d.d...}.|.j.j$t.
 00002760: 6a01 a002 7c0b 6401 7c03 6406 1700 a103  j...|.d.|.d.....
 00002770: 6402 640b 640c 8d03 0100 7c16 7c16 7c06  d.d.d.....|.|.|.
 00002780: 6408 1900 1900 a01b 7c1c a101 1900 6a19  d.......|.....j.
 00002790: 6402 640a 8d01 7d20 7c20 6a1e 6a24 7400  d.d...} | j.j$t.
 000027a0: 6a01 a002 7c0b 6401 7c04 6406 1700 a103  j...|.d.|.d.....
 000027b0: 6402 640b 640c 8d03 0100 6400 5300 290d  d.d.d.....d.S.).
-000027c0: 4e72 9400 0000 54e9 f1d8 ffff 729f 0000  Nr....T.....r...
-000027d0: 00a9 01da 0f6e 6f64 6174 615f 746f 5f76  .....nodata_to_v
-000027e0: 616c 7565 72a0 0000 0072 1a00 0000 7201  aluer....r....r.
-000027f0: 0000 00a9 01da 0f76 616c 7565 5f74 6f5f  .......value_to_
-00002800: 6e6f 6461 7461 72cc 0000 0046 7225 0000  nodatar....Fr%..
-00002810: 0029 2572 4900 0000 724a 0000 0072 4b00  .)%rI...rJ...rK.
-00002820: 0000 720f 0000 0072 0500 0000 7295 0000  ..r....r....r...
-00002830: 0072 7500 0000 72ab 0000 0072 ac00 0000  .ru...r....r....
-00002840: 7254 0000 0072 7e00 0000 72ad 0000 0072  rT...r~...r....r
-00002850: ae00 0000 72af 0000 0072 b000 0000 72b1  ....r....r....r.
+000027c0: 4e72 a500 0000 54e9 f1d8 ffff 72af 0000  Nr....T.....r...
+000027d0: 00a9 015a 0f6e 6f64 6174 615f 746f 5f76  ...Z.nodata_to_v
+000027e0: 616c 7565 72b0 0000 0072 1800 0000 7201  aluer....r....r.
+000027f0: 0000 00a9 015a 0f76 616c 7565 5f74 6f5f  .....Z.value_to_
+00002800: 6e6f 6461 7461 72d7 0000 0046 7229 0000  nodatar....Fr)..
+00002810: 0029 2572 4d00 0000 724e 0000 0072 4f00  .)%rM...rN...rO.
+00002820: 0000 720f 0000 0072 0500 0000 72a6 0000  ..r....r....r...
+00002830: 0072 7a00 0000 72bd 0000 0072 be00 0000  .rz...r....r....
+00002840: 7252 0000 0072 8300 0000 72bf 0000 0072  rR...r....r....r
+00002850: c000 0000 72c1 0000 0072 c200 0000 72c3  ....r....r....r.
 00002860: 0000 00da 0550 6f69 6e74 da04 584d 696e  .....Point..XMin
-00002870: da04 594d 696e 72b3 0000 0072 d700 0000  ..YMinr....r....
-00002880: 72b5 0000 00da 1252 6173 7465 7254 6f4e  r......RasterToN
-00002890: 756d 5079 4172 7261 7972 1b00 0000 da06  umPyArrayr......
-000028a0: 756e 6971 7565 728e 0000 00da 0864 6565  uniquer......dee
-000028b0: 7063 6f70 7972 1d00 0000 7256 0000 0072  pcopyr....rV...r
-000028c0: 5700 0000 7247 0000 0072 5800 0000 72ba  W...rG...rX...r.
+00002870: da04 594d 696e 72c4 0000 0072 dd00 0000  ..YMinr....r....
+00002880: 72c5 0000 00da 1252 6173 7465 7254 6f4e  r......RasterToN
+00002890: 756d 5079 4172 7261 7972 1d00 0000 da06  umPyArrayr......
+000028a0: 756e 6971 7565 728b 0000 00da 0864 6565  uniquer......dee
+000028b0: 7063 6f70 7972 1f00 0000 7254 0000 0072  pcopyr....rT...r
+000028c0: 5500 0000 724b 0000 0072 5600 0000 72ca  U...rK...rV...r.
 000028d0: 0000 0072 0d00 0000 da12 4e75 6d50 7941  ...r......NumPyA
 000028e0: 7272 6179 546f 5261 7374 6572 da0b 636f  rrayToRaster..co
-000028f0: 6e63 6174 656e 6174 6572 4800 0000 2921  ncatenaterH...)!
-00002900: da05 7374 725f 7272 d900 0000 da12 7374  ..str_rr......st
+000028f0: 6e63 6174 656e 6174 6572 4c00 0000 2921  ncatenaterL...)!
+00002900: da05 7374 725f 7272 df00 0000 da12 7374  ..str_rr......st
 00002910: 725f 636f 6e6e 6563 7465 645f 6c61 6b65  r_connected_lake
-00002920: 726a 0000 0072 6b00 0000 da08 736c 5f6c  rj...rk.....sl_l
-00002930: 616b 6573 72da 0000 00da 1274 6872 6573  akesr......thres
+00002920: 726e 0000 0072 6f00 0000 da08 736c 5f6c  rn...ro.....sl_l
+00002930: 616b 6573 72e0 0000 00da 1274 6872 6573  akesr......thres
 00002940: 686f 6c64 5f63 6f6e 5f6c 616b 65da 1674  hold_con_lake..t
 00002950: 6872 6573 686f 6c64 5f6e 6f6e 5f63 6f6e  hreshold_non_con
-00002960: 5f6c 616b 6572 ac00 0000 72bf 0000 0072  _laker....r....r
-00002970: 9900 0000 72b1 0000 00da 096c 6f77 6572  ....r......lower
+00002960: 5f6c 616b 6572 be00 0000 72cd 0000 0072  _laker....r....r
+00002970: a900 0000 72c3 0000 00da 096c 6f77 6572  ....r......lower
 00002980: 4c65 6674 5a16 7374 725f 636f 6e6e 6563  LeftZ.str_connec
 00002990: 7465 645f 6c61 6b65 5f76 6172 5a16 7374  ted_lake_varZ.st
 000029a0: 725f 636f 6e6e 6563 7465 645f 6c61 6b65  r_connected_lake
 000029b0: 5f61 7272 5a0c 616c 6c5f 6c61 6b65 5f61  _arrZ.all_lake_a
 000029c0: 7272 5a10 436f 6e6e 6563 745f 4c61 6b65  rrZ.Connect_Lake
 000029d0: 5f49 6473 5a0b 636c 5f6c 616b 655f 6172  _IdsZ.cl_lake_ar
 000029e0: 725a 0c6e 636c 5f6c 616b 655f 6172 725a  rZ.ncl_lake_arrZ
-000029f0: 0b73 6c5f 6c61 6b65 5f61 7272 7222 0000  .sl_lake_arrr"..
+000029f0: 0b73 6c5f 6c61 6b65 5f61 7272 7226 0000  .sl_lake_arrr&..
 00002a00: 005a 0f61 6c6c 5f6c 616b 6573 5f74 6162  .Z.all_lakes_tab
 00002a10: 6c65 5a11 756e 5f73 6c5f 636f 6e5f 6c61  leZ.un_sl_con_la
 00002a20: 6b65 6964 735a 1475 6e5f 736c 5f6e 6f6e  keidsZ.un_sl_non
 00002a30: 636f 6e5f 6c61 6b65 6964 735a 0a6e 636c  con_lakeidsZ.ncl
 00002a40: 5f6c 616b 655f 725a 0963 6c5f 6c61 6b65  _lake_rZ.cl_lake
 00002a50: 5f72 5a0b 636c 5f6c 616b 655f 6964 735a  _rZ.cl_lake_idsZ
 00002a60: 0c6e 636c 5f6c 616b 655f 6964 735a 0b73  .ncl_lake_idsZ.s
 00002a70: 6c5f 6c61 6b65 5f69 6473 5a09 736c 5f6c  l_lake_idsZ.sl_l
 00002a80: 616b 655f 725a 0963 6c5f 6c61 6b65 5f76  ake_rZ.cl_lake_v
-00002a90: 5a0a 6e63 6c5f 6c61 6b65 5f76 7215 0000  Z.ncl_lake_vr...
-00002aa0: 0072 1500 0000 7216 0000 00da 1764 6566  .r....r......def
+00002a90: 5a0a 6e63 6c5f 6c61 6b65 5f76 7213 0000  Z.ncl_lake_vr...
+00002aa0: 0072 1300 0000 7214 0000 00da 1764 6566  .r....r......def
 00002ab0: 696e 655f 636c 5f61 6e64 5f6e 636c 5f6c  ine_cl_and_ncl_l
 00002ac0: 616b 6573 4501 0000 7378 0000 0000 0212  akesE...sx......
 00002ad0: 0108 0108 010a 0114 0110 0108 0120 0214  ............. ..
 00002ae0: 010a 020e 0112 010a 010c 010a 010a 010a  ................
 00002af0: 010c 0108 010a 0212 0102 010e ff02 0206  ................
 00002b00: fe06 0302 010e ff02 0206 fe06 040e 010c  ................
 00002b10: 0108 010e 010c 0108 020a 0102 ff06 020e  ................
 00002b20: 010a 0102 ff06 020e 020a 010a 020e 010c  ................
 00002b30: 010c 010a 010a 0102 ff06 020e 011e 0122  ..............."
-00002b40: 021e 0122 0272 f000 0000 6305 0000 0000  ...".r....c.....
+00002b40: 021e 0122 0272 f400 0000 6305 0000 0000  ...".r....c.....
 00002b50: 0000 0000 0000 000c 0000 0007 0000 0043  ...............C
 00002b60: 0000 0073 c001 0000 7400 6a01 a002 7c03  ...s....t.j...|.
 00002b70: 6401 a102 7403 6a04 5f05 6402 7403 6a04  d...t.j._.d.t.j.
 00002b80: 5f06 7c01 7403 6a04 5f07 7c01 7403 6a03  _.|.t.j._.|.t.j.
 00002b90: 6a04 5f08 7403 a009 740a 7c02 6a0b 8301  j._.t...t.|.j...
 00002ba0: a101 7403 6a04 5f0c 7403 a00d 7c04 a101  ..t.j._.t...|...
 00002bb0: 6a0e 7403 6a04 5f0e 7c04 7403 6a04 5f0f  j.t.j._.|.t.j._.
@@ -716,80 +716,80 @@
 00002cb0: 7c07 6405 6602 3c00 741b 7c0b 8301 640a  |.d.f.<.t.|...d.
 00002cc0: 6b04 9001 7272 741b 7c0a 8301 7c06 6a1a  k...rrt.|...|.j.
 00002cd0: 7c07 6406 6602 3c00 71ac 640a 7c06 6a1a  |.d.f.<.q.d.|.j.
 00002ce0: 7c07 6406 6602 3c00 71ac 7c06 6a15 6a1d  |.d.f.<.q.|.j.j.
 00002cf0: 7400 6a01 a002 7c03 6401 7c00 640d 1700  t.j...|.d.|.d...
 00002d00: a103 6402 640e 640f 8d03 0100 7c06 7c06  ..d.d.d.....|.|.
 00002d10: 6405 1900 640b 6b03 1900 7d06 7c06 6700  d...d.k...}.|.g.
-00002d20: 6410 a201 1900 5300 2911 4e72 9400 0000  d.....S.).Nr....
-00002d30: 5472 a100 0000 7224 0000 00da 0844 6f77  Tr....r$.....Dow
+00002d20: 6410 a201 1900 5300 2911 4e72 a500 0000  d.....S.).Nr....
+00002d30: 5472 b100 0000 7228 0000 00da 0844 6f77  Tr....r(.....Dow
 00002d40: 5375 6249 64da 086e 5f75 705f 7375 62da  SubId..n_up_sub.
 00002d50: 0774 6f5f 6e6f 6465 da09 6672 6f6d 5f6e  .to_node..from_n
-00002d60: 6f64 6572 6600 0000 7201 0000 00e7 8d97  oderf...r.......
+00002d60: 6f64 6572 6a00 0000 7201 0000 00e7 8d97  oderj...r.......
 00002d70: 6e12 83c0 f3bf e9ff ffff ff5a 055f 726f  n..........Z._ro
-00002d80: 7574 4672 2500 0000 2903 7224 0000 0072  utFr%...).r$...r
-00002d90: f100 0000 72f2 0000 0029 1e72 4900 0000  ....r....).rI...
-00002da0: 724a 0000 0072 4b00 0000 720f 0000 0072  rJ...rK...r....r
-00002db0: 0500 0000 7295 0000 0072 7500 0000 72ab  ....r....ru...r.
-00002dc0: 0000 0072 ac00 0000 7254 0000 0072 7e00  ...r....rT...r~.
-00002dd0: 0000 72ad 0000 0072 ae00 0000 72af 0000  ..r....r....r...
-00002de0: 0072 b000 0000 72b1 0000 0072 e200 0000  .r....r....r....
-00002df0: 72e3 0000 0072 e400 0000 7256 0000 0072  r....r....rV...r
-00002e00: 5700 0000 7247 0000 0072 5800 0000 721b  W...rG...rX...r.
+00002d80: 7574 4672 2900 0000 2903 7228 0000 0072  utFr)...).r(...r
+00002d90: f500 0000 72f6 0000 0029 1e72 4d00 0000  ....r....).rM...
+00002da0: 724e 0000 0072 4f00 0000 720f 0000 0072  rN...rO...r....r
+00002db0: 0500 0000 72a6 0000 0072 7a00 0000 72bd  ....r....rz...r.
+00002dc0: 0000 0072 be00 0000 7252 0000 0072 8300  ...r....rR...r..
+00002dd0: 0000 72bf 0000 0072 c000 0000 72c1 0000  ..r....r....r...
+00002de0: 0072 c200 0000 72c3 0000 0072 e600 0000  .r....r....r....
+00002df0: 72e7 0000 0072 e800 0000 7254 0000 0072  r....r....rT...r
+00002e00: 5500 0000 724b 0000 0072 5600 0000 721d  U...rK...rV...r.
 00002e10: 0000 00da 036e 616e da05 696e 6465 7872  .....nan..indexr
-00002e20: 1f00 0000 720d 0000 0072 ba00 0000 7248  ....r....r....rH
-00002e30: 0000 0029 0cda 0573 7472 5f76 72ac 0000  ...)...str_vr...
-00002e40: 0072 bf00 0000 7299 0000 0072 b100 0000  .r....r....r....
-00002e50: 72ef 0000 005a 0873 7472 5f76 5f70 64da  r....Z.str_v_pd.
-00002e60: 0369 6478 72f3 0000 0072 f400 0000 5a0a  .idxr....r....Z.
+00002e20: 2100 0000 720d 0000 0072 ca00 0000 724c  !...r....r....rL
+00002e30: 0000 0029 0cda 0573 7472 5f76 72be 0000  ...)...str_vr...
+00002e40: 0072 cd00 0000 72a9 0000 0072 c300 0000  .r....r....r....
+00002e50: 72f3 0000 005a 0873 7472 5f76 5f70 64da  r....Z.str_v_pd.
+00002e60: 0369 6478 72f7 0000 0072 f800 0000 5a0a  .idxr....r....Z.
 00002e70: 646f 7773 7562 696e 666f 5a09 7570 7375  dowsubinfoZ.upsu
-00002e80: 6269 6e66 6f72 1500 0000 7215 0000 0072  binfor....r....r
-00002e90: 1600 0000 da1f 7265 7475 726e 5f72 6f75  ......return_rou
+00002e80: 6269 6e66 6f72 1300 0000 7213 0000 0072  binfor....r....r
+00002e90: 1400 0000 da1f 7265 7475 726e 5f72 6f75  ......return_rou
 00002ea0: 7469 6e67 5f69 6e66 6f5f 7573 696e 675f  ting_info_using_
 00002eb0: 7374 725f 7687 0100 0073 3800 0000 0001  str_v....s8.....
 00002ec0: 1201 0801 0801 0a01 1401 1001 0801 2002  .............. .
 00002ed0: 0e01 0c01 0a01 0a01 0a01 0e01 0e01 1001  ................
 00002ee0: 1001 0e01 1e01 1002 1a02 0e02 0e01 1402  ................
-00002ef0: 1002 2201 1002 72fb 0000 0063 0700 0000  .."...r....c....
+00002ef0: 1002 2201 1002 72ff 0000 0063 0700 0000  .."...r....c....
 00002f00: 0000 0000 0000 0000 0b00 0000 0600 0000  ................
 00002f10: 4300 0000 73ca 0000 0074 006a 01a0 027c  C...s....t.j...|
 00002f20: 0564 01a1 0274 036a 045f 0564 0274 036a  .d...t.j._.d.t.j
 00002f30: 045f 067c 0374 036a 045f 077c 0374 036a  ._.|.t.j._.|.t.j
 00002f40: 036a 045f 0874 03a0 0974 0a7c 046a 0b83  .j._.t...t.|.j..
 00002f50: 01a1 0174 036a 045f 0c74 03a0 0d7c 06a1  ...t.j._.t...|..
 00002f60: 016a 0e74 036a 045f 0e7c 0674 036a 045f  .j.t.j._.|.t.j._
 00002f70: 0f74 03a0 1074 03a0 0d7c 06a1 016a 0e6a  .t...t...|...j.j
 00002f80: 1174 03a0 0d7c 06a1 016a 0e6a 12a1 027d  .t...|...j.j...}
 00002f90: 0774 036a 137c 0064 0364 048d 027d 0874  .t.j.|.d.d...}.t
 00002fa0: 147c 0283 0164 056b 0472 a674 15a0 167c  .|...d.k.r.t...|
 00002fb0: 087c 02a1 027d 0964 037c 087c 093c 0074  .|...}.d.|.|.<.t
 00002fc0: 036a 177c 087c 077c 0364 0364 068d 047d  .j.|.|.|.d.d...}
 00002fd0: 0a7c 0aa0 187c 01a1 0101 007c 0a7c 0866  .|...|.....|.|.f
-00002fe0: 0253 0029 074e 7294 0000 0054 72dd 0000  .S.).Nr....Tr...
-00002ff0: 0072 de00 0000 7201 0000 0072 e000 0000  .r....r....r....
-00003000: 2919 7249 0000 0072 4a00 0000 724b 0000  ).rI...rJ...rK..
-00003010: 0072 0f00 0000 7205 0000 0072 9500 0000  .r....r....r....
-00003020: 7275 0000 0072 ab00 0000 72ac 0000 0072  ru...r....r....r
-00003030: 5400 0000 727e 0000 0072 ad00 0000 72ae  T...r~...r....r.
-00003040: 0000 0072 af00 0000 72b0 0000 0072 b100  ...r....r....r..
-00003050: 0000 72e2 0000 0072 e300 0000 72e4 0000  ..r....r....r...
-00003060: 0072 e500 0000 720d 0000 0072 1b00 0000  .r....r....r....
-00003070: 721d 0000 0072 e800 0000 72b5 0000 0029  r....r....r....)
-00003080: 0b72 1100 0000 7212 0000 0072 ba00 0000  .r....r....r....
-00003090: 72ac 0000 0072 bf00 0000 7299 0000 0072  r....r....r....r
-000030a0: b100 0000 72ef 0000 005a 0969 6e70 7574  ....r....Z.input
-000030b0: 5f61 7272 7222 0000 00da 0c69 6e70 7574  _arrr".....input
-000030c0: 5f72 6173 7465 7272 1500 0000 7215 0000  _rasterr....r...
-000030d0: 0072 1600 0000 da1b 6172 6367 6973 5f72  .r......arcgis_r
+00002fe0: 0253 0029 074e 72a5 0000 0054 72e3 0000  .S.).Nr....Tr...
+00002ff0: 0072 e400 0000 7201 0000 0072 e500 0000  .r....r....r....
+00003000: 2919 724d 0000 0072 4e00 0000 724f 0000  ).rM...rN...rO..
+00003010: 0072 0f00 0000 7205 0000 0072 a600 0000  .r....r....r....
+00003020: 727a 0000 0072 bd00 0000 72be 0000 0072  rz...r....r....r
+00003030: 5200 0000 7283 0000 0072 bf00 0000 72c0  R...r....r....r.
+00003040: 0000 0072 c100 0000 72c2 0000 0072 c300  ...r....r....r..
+00003050: 0000 72e6 0000 0072 e700 0000 72e8 0000  ..r....r....r...
+00003060: 0072 e900 0000 720d 0000 0072 1d00 0000  .r....r....r....
+00003070: 721f 0000 0072 ec00 0000 72c5 0000 0029  r....r....r....)
+00003080: 0b72 1000 0000 7211 0000 0072 ca00 0000  .r....r....r....
+00003090: 72be 0000 0072 cd00 0000 72a9 0000 0072  r....r....r....r
+000030a0: c300 0000 72f3 0000 005a 0969 6e70 7574  ....r....Z.input
+000030b0: 5f61 7272 7226 0000 005a 0c69 6e70 7574  _arrr&...Z.input
+000030c0: 5f72 6173 7465 7272 1300 0000 7213 0000  _rasterr....r...
+000030d0: 0072 1400 0000 da1b 6172 6367 6973 5f72  .r......arcgis_r
 000030e0: 6173 7465 725f 7365 746e 756c 6c5f 6172  aster_setnull_ar
 000030f0: 7261 79ad 0100 0073 2200 0000 0001 1201  ray....s".......
 00003100: 0801 0801 0a01 1401 1001 0801 2002 0e01  ............ ...
-00003110: 0c01 0c01 0802 0a01 02ff 0602 0a01 72fd  ..............r.
-00003120: 0000 0063 0e00 0000 0000 0000 0000 0000  ...c............
-00003130: 2600 0000 0900 0000 4300 0000 7378 0300  &.......C...sx..
+00003110: 0c01 0c01 0802 0a01 02ff 0602 0a01 7200  ..............r.
+00003120: 0100 0063 0e00 0000 0000 0000 0000 0000  ...c............
+00003130: 2800 0000 0900 0000 4300 0000 7316 0400  (.......C...s...
 00003140: 0074 006a 01a0 027c 0c64 01a1 0274 036a  .t.j...|.d...t.j
 00003150: 045f 0564 0274 036a 045f 067c 0a74 036a  ._.d.t.j._.|.t.j
 00003160: 045f 077c 0a74 036a 036a 045f 0874 03a0  ._.|.t.j.j._.t..
 00003170: 0974 0a7c 0b6a 0b83 01a1 0174 036a 045f  .t.|.j.....t.j._
 00003180: 0c74 03a0 0d7c 0da1 016a 0e74 036a 045f  .t...|...j.t.j._
 00003190: 0e7c 0d74 036a 045f 0f74 03a0 1074 03a0  .|.t.j._.t...t..
 000031a0: 0d7c 0da1 016a 0e6a 1174 03a0 0d7c 0da1  .|...j.j.t...|..
@@ -823,335 +823,354 @@
 00003360: 1c64 2164 2264 2364 007c 0da1 0601 007c  .d!d"d#d.|.....|
 00003370: 0f7c 0f64 1119 00a0 247c 19a1 010f 0019  .|.d....$|......
 00003380: 0064 1119 006a 207d 1a74 2164 1564 247c  .d...j }.t!d.d$|
 00003390: 1a7c 0a7c 0b7c 0c7c 0d83 0701 0074 2974  .|.|.|.|.....t)t
 000033a0: 2a64 2483 0164 1a64 2283 037d 1b74 2974  *d$..d.d"..}.t)t
 000033b0: 2a7c 0364 0317 0083 017c 1b64 1a83 037d  *|.d.....|.d...}
 000033c0: 1c74 2b7c 1c7c 1c64 2583 037d 1d7c 1da0  .t+|.|.d%..}.|..
-000033d0: 1764 26a1 0101 0074 1464 267c 057c 0764  .d&....t.d&|.|.d
-000033e0: 047c 0a7c 0b7c 0c7c 0d83 0801 0074 03a0  .|.|.|.|.....t..
-000033f0: 2c7c 097c 0964 2717 0064 28a1 0301 0074  ,|.|.d'..d(....t
-00003400: 196a 1a6a 1ba0 1c7c 0964 2717 00a1 017d  .j.j...|.d'....}
-00003410: 1e74 196a 1a6a 1ba0 1c7c 0764 2717 00a1  .t.j.j...|.d'...
-00003420: 017d 1f74 196a 1a6a 1ba0 1c7c 0864 2717  .}.t.j.j...|.d'.
-00003430: 00a1 017d 2074 196a 2d7c 1e7c 1f7c 2067  ...} t.j-|.|.| g
-00003440: 0364 0264 298d 027d 217c 21a0 2ea1 007d  .d.d)..}!|!....}
-00003450: 217c 216a 2f64 2a17 007c 2164 113c 007c  !|!j/d*..|!d.<.|
-00003460: 2164 1164 2b67 0219 007d 217c 216a 1b6a  !d.d+g...}!|!j.j
-00003470: 3074 006a 01a0 027c 0c64 017c 0664 2717  0t.j...|.d.|.d'.
-00003480: 00a1 0364 0264 2c64 2d8d 0301 007c 1164  ...d.d,d-....|.d
-00003490: 1519 006a 207d 227c 1164 1619 006a 207d  ...j }"|.d...j }
-000034a0: 2374 317c 237c 227c 0f83 035c 027d 247d  #t1|#|"|...\.}$}
-000034b0: 257c 247c 2566 0253 0029 2e4e 7294 0000  %|$|%f.S.).Nr...
-000034c0: 0054 729f 0000 0072 a600 0000 5a0a 7375  .Tr....r....Z.su
-000034d0: 625f 6f75 746c 6574 5a09 7375 625f 696e  b_outletZ.sub_in
-000034e0: 6c65 74da 074d 494e 494d 554d 5a0b 7375  let..MINIMUMZ.su
-000034f0: 625f 696e 6c65 745f 76da 0873 6c5f 636c  b_inlet_v..sl_cl
-00003500: 5f69 64da 0849 4c5f 5375 6249 64da 0a4d  _id..IL_SubId..M
-00003510: 6178 4163 635f 6361 7472 a200 0000 5a0f  axAcc_catr....Z.
-00003520: 756e 6971 7565 5f6c 616b 655f 7374 7229  unique_lake_str)
-00003530: 03da 0576 616c 7565 72ea 0000 00da 1073  ...valuer......s
-00003540: 656c 6563 7465 645f 6c61 6b65 735f 7229  elected_lakes_r)
-00003550: 0372 0001 0000 72ff 0000 0072 0101 0000  .r....r....r....
-00003560: 72f6 0000 0072 2400 0000 7242 0000 0072  r....r$...rB...r
-00003570: 4300 0000 7202 0100 0072 ea00 0000 7203  C...r....r....r.
-00003580: 0100 005a 0c73 7562 5f6f 7574 6c65 745f  ...Z.sub_outlet_
-00003590: 725a 1675 6e69 7175 655f 6c61 6b65 5f73  rZ.unique_lake_s
-000035a0: 7472 5f69 6e66 6c6f 775a 116c 616b 655f  tr_inflowZ.lake_
-000035b0: 696e 6c65 745f 696e 6c61 6b65 72dd 0000  inlet_inlaker...
-000035c0: 005a 136c 616b 655f 696e 6c65 745f 696e  .Z.lake_inlet_in
-000035d0: 6c61 6b65 5f76 5a15 6c61 6b65 5f69 6e6c  lake_vZ.lake_inl
-000035e0: 6574 5f69 6e6c 616b 655f 7662 6667 0000  et_inlake_vbfg..
-000035f0: 0000 0000 0440 72c4 0000 0072 c500 0000  .....@r....r....
-00003600: 72c7 0000 0072 a100 0000 5a16 7374 725f  r....r....Z.str_
-00003610: 6172 6f75 6e64 5f6c 616b 655f 696e 6c65  around_lake_inle
-00003620: 7473 72ce 0000 005a 0f6c 616b 655f 696e  tsr....Z.lake_in
-00003630: 666c 6f77 5f73 7472 7a0d 5641 4c55 4520  flow_strz.VALUE 
-00003640: 3d20 2d39 3939 395a 1c6c 616b 655f 696e  = -9999Z.lake_in
-00003650: 666c 6f77 5f73 6567 5f6f 7574 7369 6465  flow_seg_outside
-00003660: 5f6c 616b 6572 a000 0000 729d 0000 0029  _laker....r....)
-00003670: 01da 0c69 676e 6f72 655f 696e 6465 7872  ...ignore_indexr
-00003680: 6600 0000 723f 0000 0046 7225 0000 0029  f...r?...Fr%...)
-00003690: 3272 4900 0000 724a 0000 0072 4b00 0000  2rI...rJ...rK...
-000036a0: 720f 0000 0072 0500 0000 7295 0000 0072  r....r....r....r
-000036b0: 7500 0000 72ab 0000 0072 ac00 0000 7254  u...r....r....rT
-000036c0: 0000 0072 7e00 0000 72ad 0000 0072 ae00  ...r~...r....r..
-000036d0: 0000 72af 0000 0072 b000 0000 72b1 0000  ..r....r....r...
-000036e0: 0072 e200 0000 72e3 0000 0072 e400 0000  .r....r....r....
-000036f0: 72fb 0000 0072 c100 0000 72b8 0000 00da  r....r....r.....
-00003700: 0743 6f6d 6269 6e65 72b5 0000 0072 9c00  .Combiner....r..
-00003710: 0000 7256 0000 0072 5700 0000 7247 0000  ..rV...rW...rG..
-00003720: 0072 5800 0000 da06 6669 6c6c 6e61 7259  .rX.....fillnarY
-00003730: 0000 005a 3172 6574 7572 6e5f 6e6f 6e5f  ...Z1return_non_
-00003740: 6c61 6b65 5f69 6e66 6c6f 775f 7365 6773  lake_inflow_segs
-00003750: 5f61 6e64 5f73 6567 735f 7769 7468 696e  _and_segs_within
-00003760: 5f6c 616b 6573 72ba 0000 0072 fd00 0000  _lakesr....r....
-00003770: 721b 0000 0072 e600 0000 721d 0000 0072  r....r....r....r
-00003780: 5100 0000 72d0 0000 0072 0e00 0000 72d5  Q...r....r....r.
-00003790: 0000 0072 b300 0000 72d7 0000 00da 0753  ...r....r......S
-000037a0: 6574 4e75 6c6c 72b6 0000 00da 0663 6f6e  etNullr......con
-000037b0: 6361 74da 0b72 6573 6574 5f69 6e64 6578  cat..reset_index
-000037c0: 72f8 0000 0072 4800 0000 5a1f 4368 6563  r....rH...Z.Chec
-000037d0: 6b5f 4966 5f4c 616b 655f 4861 7665 5f4d  k_If_Lake_Have_M
-000037e0: 756c 7469 5f4f 7574 4c65 7429 2672 ea00  ulti_OutLet)&r..
-000037f0: 0000 72f9 0000 00da 0b63 6174 5f6e 6f5f  ..r......cat_no_
-00003800: 6c61 6b65 72ec 0000 0072 6a00 0000 da03  laker....rj.....
-00003810: 6163 635a 1570 6f75 7270 6f69 6e74 735f  accZ.pourpoints_
-00003820: 7769 7468 5f6c 616b 6573 5a16 6c61 6b65  with_lakesZ.lake
-00003830: 5f69 6e66 6c6f 775f 706f 7572 706f 696e  _inflow_pourpoin
-00003840: 7473 da17 6c61 6b65 5f6f 7574 666c 6f77  ts..lake_outflow
-00003850: 5f70 6f75 7270 6f69 6e74 735a 2163 6174  _pourpointsZ!cat
-00003860: 6368 6d65 6e74 5f70 6f75 7270 6f69 6e74  chment_pourpoint
-00003870: 735f 6f75 7473 6964 655f 6c61 6b65 72ac  s_outside_laker.
-00003880: 0000 0072 bf00 0000 7299 0000 0072 b100  ...r....r....r..
-00003890: 0000 72ef 0000 005a 0c72 6f75 7469 6e67  ..r....Z.routing
-000038a0: 5f69 6e66 6f5a 104f 7665 726c 6179 5f73  _infoZ.Overlay_s
-000038b0: 7472 5f6c 616b 655a 1075 6e69 715f 6c61  tr_lakeZ.uniq_la
-000038c0: 6b65 5f73 7472 5f70 645a 1373 7472 5f73  ke_str_pdZ.str_s
-000038d0: 7461 7274 5f70 745f 6c61 6b65 6964 5a13  tart_pt_lakeidZ.
-000038e0: 7374 725f 6964 5f77 6974 6869 6e5f 6c61  str_id_within_la
-000038f0: 6b65 735a 146e 6f6e 5f6c 616b 655f 696e  kesZ.non_lake_in
-00003900: 666c 6f77 5f73 6567 735a 1273 7472 5f69  flow_segsZ.str_i
-00003910: 645f 6c61 6b65 5f69 6e6c 666f 77da 0474  d_lake_inlfow..t
-00003920: 656d 705a 206c 616b 655f 696e 666c 6f77  empZ lake_inflow
-00003930: 5f75 6e69 7175 655f 6c61 6b65 7374 725f  _unique_lakestr_
-00003940: 6172 7261 795a 1e6c 616b 655f 696e 666c  arrayZ.lake_infl
-00003950: 6f77 5f75 6e69 7175 655f 6c61 6b65 7374  ow_unique_lakest
-00003960: 725f 6964 735a 116c 616b 655f 696e 6c65  r_idsZ.lake_inle
-00003970: 745f 7375 6269 6473 5a0a 6578 636c 7564  t_subidsZ.exclud
-00003980: 6569 6473 5a23 7265 6d6f 7665 5f76 616c  eidsZ#remove_val
-00003990: 7565 5f6e 6f74 5f6f 6e5f 6c61 6b65 5f69  ue_not_on_lake_i
-000039a0: 6e66 6c6f 775f 7374 725a 1972 656d 6f76  nflow_strZ.remov
-000039b0: 655f 7661 6c75 655f 696e 7369 6465 5f6c  e_value_inside_l
-000039c0: 616b 6573 5a1f 7265 6d6f 7665 5f76 616c  akesZ.remove_val
-000039d0: 7565 5f69 6e73 6964 655f 6c61 6b65 735f  ue_inside_lakes_
-000039e0: 6e6f 3939 395a 0a63 6174 5f6f 7574 6c65  no999Z.cat_outle
-000039f0: 745a 0b6c 616b 655f 696e 6c65 7473 5a0c  tZ.lake_inletsZ.
-00003a00: 6c61 6b65 5f6f 7574 6c65 7473 5a17 706f  lake_outletsZ.po
-00003a10: 7572 706f 696e 7473 5f77 6974 686c 616b  urpoints_withlak
-00003a20: 655f 7661 725a 0653 7472 5f49 645a 0543  e_varZ.Str_IdZ.C
-00003a30: 4c5f 4964 5a17 4c61 6b65 735f 5749 7468  L_IdZ.Lakes_WIth
-00003a40: 5f4d 756c 7469 5f4f 7574 6c65 745a 0a52  _Multi_OutletZ.R
-00003a50: 656d 6f76 655f 5374 7272 1500 0000 7215  emove_Strr....r.
-00003a60: 0000 0072 1600 0000 da1d 6372 6561 7465  ...r......create
-00003a70: 5f70 6f75 725f 706f 696e 7473 5f77 6974  _pour_points_wit
-00003a80: 685f 6c61 6b65 73c2 0100 0073 7800 0000  h_lakes....sx...
-00003a90: 0004 1201 0801 0801 0a01 1401 1001 0801  ................
-00003aa0: 2003 1002 1a01 1601 1604 2201 1001 0a02   .........".....
-00003ab0: 1001 0e01 0c01 0a01 0c02 1005 0201 24ff  ..............$.
-00003ac0: 02fc 0201 0201 0201 0206 1403 1803 1603  ................
-00003ad0: 0a01 0c02 1803 2003 0a01 06ff 0404 1a01  ...... .........
-00003ae0: 1402 1001 1401 0c01 0a01 1602 1202 1201  ................
-00003af0: 1201 1202 1401 0801 0e01 0c01 2202 0a01  ............"...
-00003b00: 0a02 0201 06ff 0804 720e 0100 0063 0100  ........r....c..
-00003b10: 0000 0000 0000 0000 0000 2a00 0000 0700  ..........*.....
-00003b20: 0000 4300 0000 73c0 0600 007c 006a 007d  ..C...s....|.j.}
-00003b30: 0174 0164 0174 027c 0183 0183 0244 0090  .t.d.t.|.....D..
-00003b40: 015d 1c7d 027c 017c 0219 007d 037c 006a  .].}.|.|...}.|.j
-00003b50: 037c 0364 0266 0219 0064 031b 0064 031b  .|.d.f...d...d..
-00003b60: 007d 047c 006a 037c 0364 0466 0219 007d  .}.|.j.|.d.f...}
-00003b70: 057c 006a 037c 0364 0566 0219 007d 067c  .|.j.|.d.f...}.|
-00003b80: 006a 037c 0364 0666 0219 007d 077c 0664  .j.|.d.f...}.|.d
-00003b90: 016b 0072 7464 077d 0864 087d 096e 187c  .k.rtd.}.d.}.n.|
-00003ba0: 067d 087c 077d 097c 0864 016b 0072 8c64  .}.|.}.|.d.k.r.d
-00003bb0: 077d 0864 087d 0974 047c 047c 087c 0983  .}.d.}.t.|.|.|..
-00003bc0: 037d 0a74 0564 097c 0a64 0a13 0014 0074  .}.t.d.|.d.....t
-00003bd0: 0683 027c 006a 037c 0364 0b66 023c 0074  ...|.j.|.d.f.<.t
-00003be0: 0564 0c7c 0a64 0d13 0014 0074 0783 027c  .d.|.d.....t...|
-00003bf0: 006a 037c 0364 0e66 023c 007c 0a7c 006a  .j.|.d.f.<.|.|.j
-00003c00: 037c 0364 0f66 023c 007c 006a 037c 0364  .|.d.f.<.|.j.|.d
-00003c10: 1066 0219 0064 116b 0072 147c 006a 037c  .f...d.k.r.|.j.|
-00003c20: 0364 1266 0219 0064 016b 0072 147c 006a  .d.f...d.k.r.|.j
-00003c30: 037c 0364 1366 0219 007c 006a 037c 0364  .|.d.f...|.j.|.d
-00003c40: 1266 023c 007c 006a 037c 0364 1366 0219  .f.<.|.j.|.d.f..
-00003c50: 007c 006a 037c 0364 1466 023c 0071 147c  .|.j.|.d.f.<.q.|
-00003c60: 006a 037c 0064 1019 0064 116b 007c 0064  .j.|.d...d.k.|.d
-00003c70: 1519 0064 166b 0340 0019 006a 0864 1764  ...d.k.@...j.d.d
-00003c80: 188d 017d 0b7c 0b64 1919 006a 097d 0c74  ...}.|.d...j.}.t
-00003c90: 0aa0 0b7c 0ca1 017d 0c74 0164 0174 027c  ...|...}.t.d.t.|
-00003ca0: 0c83 0183 0244 0090 055d 007d 0d7c 0c7c  .....D...].}.|.|
-00003cb0: 0d19 007d 0e7c 0b7c 0b64 1919 007c 0e6b  ...}.|.|.d...|.k
-00003cc0: 0219 007d 0f74 027c 0f64 1519 006a 097c  ...}.t.|.d...j.|
-00003cd0: 0f64 1519 006a 0964 016b 0419 0083 0164  .d...j.d.k.....d
-00003ce0: 016b 0490 0172 dc74 0aa0 0c7c 0f64 1519  .k...r.t...|.d..
-00003cf0: 006a 097c 0f64 1519 006a 0964 016b 0419  .j.|.d...j.d.k..
-00003d00: 00a1 017d 106e 0464 1a7d 1074 0aa0 0d7c  ...}.n.d.}.t...|
-00003d10: 0f64 0f19 006a 097c 0f64 0f19 006a 0964  .d...j.|.d...j.d
-00003d20: 016b 0419 00a1 017d 1174 0aa0 0d7c 0f64  .k.....}.t...|.d
-00003d30: 0b19 006a 097c 0f64 0b19 006a 0964 016b  ...j.|.d...j.d.k
-00003d40: 0419 00a1 017d 1274 0aa0 0d7c 0f64 0e19  .....}.t...|.d..
-00003d50: 006a 097c 0f64 0e19 006a 0964 016b 0419  .j.|.d...j.d.k..
-00003d60: 00a1 017d 1374 0aa0 0d7c 0f64 1b19 006a  ...}.t...|.d...j
-00003d70: 097c 0f64 1b19 006a 0964 016b 0419 00a1  .|.d...j.d.k....
-00003d80: 017d 1474 0aa0 0d7c 0f64 1c19 006a 097c  .}.t...|.d...j.|
-00003d90: 0f64 1c19 006a 0964 016b 0419 00a1 017d  .d...j.d.k.....}
-00003da0: 1574 0aa0 0d7c 0f64 1d19 006a 097c 0f64  .t...|.d...j.|.d
-00003db0: 1d19 006a 0964 016b 0419 00a1 017d 1674  ...j.d.k.....}.t
-00003dc0: 0aa0 0d7c 0f64 1319 006a 097c 0f64 1319  ...|.d...j.|.d..
-00003dd0: 006a 0964 016b 0419 00a1 017d 1774 027c  .j.d.k.....}.t.|
-00003de0: 0f64 1219 006a 097c 0f64 1219 006a 0964  .d...j.|.d...j.d
-00003df0: 1e6b 0419 0083 0164 016b 0490 0372 1274  .k.....d.k...r.t
-00003e00: 0aa0 057c 0f64 1219 006a 097c 0f64 1219  ...|.d...j.|.d..
-00003e10: 006a 0964 1f6b 0419 00a1 017d 1874 0aa0  .j.d.k.....}.t..
-00003e20: 0e7c 0f64 1419 006a 097c 0f64 1419 006a  .|.d...j.|.d...j
-00003e30: 0964 1f6b 0419 00a1 017d 196e 087c 177d  .d.k.....}.n.|.}
-00003e40: 187c 177d 197c 187c 1918 007c 101b 007d  .|.}.|.|...|...}
-00003e50: 1a7c 1a64 206b 0090 0372 3474 0f7d 1a74  .|.d k...r4t.}.t
-00003e60: 107c 127c 137c 117c 1a83 047d 1b74 0164  .|.|.|.|...}.t.d
-00003e70: 0174 027c 0f83 0183 0244 0090 035d 287d  .t.|.....D...](}
-00003e80: 027c 0f64 0419 006a 097c 0219 007d 1c7c  .|.d...j.|...}.|
-00003e90: 0f64 1219 006a 097c 0219 007d 1d7c 0f64  .d...j.|...}.|.d
-00003ea0: 1419 006a 097c 0219 007d 1e74 057c 0f64  ...j.|...}.t.|.d
-00003eb0: 1519 006a 097c 0219 0074 1183 027d 1f7c  ...j.|...t...}.|
-00003ec0: 0f64 0f19 006a 097c 0219 007d 207c 0f64  .d...j.|...} |.d
-00003ed0: 0b19 006a 097c 0219 007d 217c 0f64 0e19  ...j.|...}!|.d..
-00003ee0: 006a 097c 0219 007d 227c 0f64 1b19 006a  .j.|...}"|.d...j
-00003ef0: 097c 0219 007d 237c 1e64 216b 0090 0372  .|...}#|.d!k...r
-00003f00: fe7c 0f64 1319 006a 097c 0219 0064 216b  .|.d...j.|...d!k
-00003f10: 0490 0372 fa7c 0f64 1319 006a 097c 0219  ...r.|.d...j.|..
-00003f20: 007d 1e6e 047c 177d 1e7c 1d64 216b 0090  .}.n.|.}.|.d!k..
-00003f30: 0472 307c 0f64 1319 006a 097c 0219 0064  .r0|.d...j.|...d
-00003f40: 216b 0490 0472 2c7c 0f64 1319 006a 097c  !k...r,|.d...j.|
-00003f50: 0219 007d 1d6e 047c 177d 1d7c 0f64 2219  ...}.n.|.}.|.d".
-00003f60: 006a 097c 0219 007d 247c 2474 0f6b 0090  .j.|...}$|$t.k..
-00003f70: 0473 527c 2474 126b 0490 0472 6a7c 1a74  .sR|$t.k...rj|.t
-00003f80: 0f6b 0590 0472 6a7c 1a74 126b 0190 0472  .k...rj|.t.k...r
-00003f90: 6a7c 1a7d 2474 057c 2474 0f83 027d 2474  j|.}$t.|$t...}$t
-00003fa0: 0e7c 2474 1283 027d 2474 107c 217c 227c  .|$t...}$t.|!|"|
-00003fb0: 207c 2483 047d 257c 2574 136b 0090 0473   |$..}%|%t.k...s
-00003fc0: a07c 2574 146b 0490 0472 b87c 1b74 136b  .|%t.k...r.|.t.k
-00003fd0: 0590 0472 b87c 1b74 146b 0190 0472 b87c  ...r.|.t.k...r.|
-00003fe0: 1b7d 2574 057c 2574 1383 027d 2574 0e7c  .}%t.|%t...}%t.|
-00003ff0: 2574 1483 027d 257c 247c 006a 037c 0064  %t...}%|$|.j.|.d
-00004000: 0419 007c 1c6b 0264 2266 023c 007c 257c  ...|.k.d"f.<.|%|
-00004010: 006a 037c 0064 0419 007c 1c6b 0264 2366  .j.|.d...|.k.d#f
-00004020: 023c 007c 1f7c 006a 037c 0064 0419 007c  .<.|.|.j.|.d...|
-00004030: 1c6b 0264 1566 023c 007c 2364 016b 0090  .k.d.f.<.|#d.k..
-00004040: 0572 2c7c 1464 016b 0490 0572 287c 147d  .r,|.d.k...r(|.}
-00004050: 236e 0474 157d 2374 057c 237c 2583 027d  #n.t.}#t.|#|%..}
-00004060: 237c 237c 006a 037c 0064 0419 007c 1c6b  #|#|.j.|.d...|.k
-00004070: 0264 1b66 023c 007c 1d7c 006a 037c 0064  .d.f.<.|.|.j.|.d
-00004080: 0419 007c 1c6b 0264 1266 023c 007c 1e7c  ...|.k.d.f.<.|.|
-00004090: 006a 037c 0064 0419 007c 1c6b 0264 1466  .j.|.d...|.k.d.f
-000040a0: 023c 007c 0f64 1c19 006a 097c 0219 0064  .<.|.d...j.|...d
-000040b0: 016b 0190 0572 c47c 1564 016b 0490 0572  .k...r.|.d.k...r
-000040c0: ae7c 157c 006a 037c 0064 0419 007c 1c6b  .|.|.j.|.d...|.k
-000040d0: 0264 1c66 023c 006e 1664 017c 006a 037c  .d.f.<.n.d.|.j.|
-000040e0: 0064 0419 007c 1c6b 0264 1c66 023c 007c  .d...|.k.d.f.<.|
-000040f0: 0f64 1d19 006a 097c 0219 0064 016b 0190  .d...j.|...d.k..
-00004100: 0672 107c 1664 016b 0490 0572 fa7c 167c  .r.|.d.k...r.|.|
-00004110: 006a 037c 0064 0419 007c 1c6b 0264 1d66  .j.|.d...|.k.d.f
-00004120: 023c 006e 1664 017c 006a 037c 0064 0419  .<.n.d.|.j.|.d..
-00004130: 007c 1c6b 0264 1d66 023c 007c 0f64 1319  .|.k.d.f.<.|.d..
-00004140: 006a 097c 0219 0064 016b 0090 0372 507c  .j.|...d.k...rP|
-00004150: 1764 016b 0490 0672 467c 177c 006a 037c  .d.k...rF|.|.j.|
-00004160: 0064 0419 007c 1c6b 0264 1366 023c 006e  .d...|.k.d.f.<.n
-00004170: 327c 0064 1319 006a 097d 267c 267c 2664  2|.d...j.}&|&|&d
-00004180: 016b 0419 007d 2674 0aa0 0d7c 26a1 017c  .k...}&t...|&..|
-00004190: 006a 037c 0064 0419 007c 1c6b 0264 1366  .j.|.d...|.k.d.f
-000041a0: 023c 0090 0371 5090 0171 7c7c 0064 2419  .<...qP..q||.d$.
-000041b0: 0074 0f6b 007d 277c 0064 2419 0074 126b  .t.k.}'|.d$..t.k
-000041c0: 047d 2874 0aa0 167c 277c 28a1 027d 297c  .}(t...|'|(..})|
-000041d0: 006a 037c 2964 2266 0219 007c 006a 037c  .j.|)d"f...|.j.|
-000041e0: 2964 2466 023c 007c 0053 0029 254e 7201  )d$f.<.|.S.)%Nr.
-000041f0: 0000 00da 0944 7261 696e 4172 6561 69e8  .....DrainAreai.
-00004200: 0300 0072 2400 0000 da01 6bda 0163 67c1  ...r$.....k..cg.
-00004210: ab27 eb1e 7672 3f67 9972 1121 a68b ef3f  .'..vr?g.r.!...?
-00004220: 67cd cccc cccc cc1c 4072 c300 0000 5a08  g.......@r....Z.
-00004230: 426b 6657 6964 7468 6748 e17a 14ae 47d1  BkfWidthgH.z..G.
-00004240: 3f67 3333 3333 3333 d33f 5a08 426b 6644  ?g333333.?Z.BkfD
-00004250: 6570 7468 5a06 515f 4d65 616e 7219 0000  epthZ.Q_Meanr...
-00004260: 0072 1a00 0000 5a07 4d61 785f 4445 4d5a  .r....Z.Max_DEMZ
-00004270: 084d 6561 6e45 6c65 765a 074d 696e 5f44  .MeanElevZ.Min_D
-00004280: 454d 7246 0000 0072 f500 0000 5472 cc00  EMrF...r....Tr..
-00004290: 0000 da06 5365 675f 4944 7266 0000 005a  ....Seg_IDrf...Z
-000042a0: 0846 6c6f 6f64 505f 6e5a 0842 6173 536c  .FloodP_nZ.BasSl
-000042b0: 6f70 655a 0942 6173 4173 7065 6374 6cfc  opeZ.BasAspectl.
-000042c0: ffff ffff 7fc7 4ece 5a05 6f6c fcff ffff  ......N.Z.ol....
-000042d0: ff7f 815f c91b 1c01 6795 d626 e80b 2e11  ..._....g..&....
-000042e0: 3e69 30f8 ffff 5a08 5269 7653 6c6f 7065  >i0...Z.RivSlope
-000042f0: 5a04 4368 5f6e 5a0a 4441 5f43 686e 5f53  Z.Ch_nZ.DA_Chn_S
-00004300: 6c70 2917 72f8 0000 0072 0c00 0000 720d  lp).r....r....r.
-00004310: 0000 0072 1f00 0000 5a09 6675 6e63 5f51  ...r....Z.func_Q
-00004320: 5f44 41da 036d 6178 5a0d 6d69 6e5f 626b  _DA..maxZ.min_bk
-00004330: 665f 7769 6474 685a 0d6d 696e 5f62 6b66  f_widthZ.min_bkf
-00004340: 5f64 6570 7468 728e 0000 0072 ba00 0000  _depthr....r....
-00004350: 721b 0000 0072 e600 0000 da03 7375 6dda  r....r......sum.
-00004360: 0761 7665 7261 6765 da03 6d69 6e5a 0d6d  .average..minZ.m
-00004370: 696e 5f72 6976 5f73 6c6f 7065 5a11 6361  in_riv_slopeZ.ca
-00004380: 6c63 756c 6174 6543 6861 6e6e 616c 6e5a  lculateChannalnZ
-00004390: 0d6d 696e 5f72 6976 5f6c 656e 7468 5a0d  .min_riv_lenthZ.
-000043a0: 6d61 785f 7269 765f 736c 6f70 655a 0d6d  max_riv_slopeZ.m
-000043b0: 696e 5f6d 616e 6e69 6e67 5f6e 5a0d 6d61  in_manning_nZ.ma
-000043c0: 785f 6d61 6e6e 696e 675f 6e5a 0f44 4546  x_manning_nZ.DEF
-000043d0: 414c 5554 5f46 4c4f 4f44 5f4e 725a 0000  ALUT_FLOOD_NrZ..
-000043e0: 0029 2a5a 0763 6174 696e 666f 72fa 0000  .)*Z.catinfor...
-000043f0: 0072 1400 0000 5a05 6964 785f 6972 9600  .r....Z.idx_ir..
-00004400: 0000 5a05 6361 7469 6472 1001 0000 7211  ..Z.catidr....r.
-00004410: 0100 005a 056b 5f73 7562 5a05 635f 7375  ...Z.k_subZ.c_su
-00004420: 62da 0171 5a0b 6361 7469 6e66 6f5f 7269  b..qZ.catinfo_ri
-00004430: 765a 0753 6567 5f49 4453 5a04 6973 6567  vZ.Seg_IDSZ.iseg
-00004440: 5a08 695f 7365 675f 6964 5a0a 695f 7365  Z.i_seg_idZ.i_se
-00004450: 675f 696e 666f 5a0a 6c65 6e67 7468 5f73  g_infoZ.length_s
-00004460: 6567 5a09 716d 6561 6e5f 7365 675a 0977  egZ.qmean_segZ.w
-00004470: 6964 7468 5f73 6567 5a09 6465 7074 685f  idth_segZ.depth_
-00004480: 5365 675a 0a66 6c6f 6f64 6e5f 5365 675a  SegZ.floodn_SegZ
-00004490: 0a62 6173 736c 705f 5365 675a 0a62 6173  .basslp_SegZ.bas
-000044a0: 6173 705f 5365 675a 0a62 6173 656c 765f  asp_SegZ.baselv_
-000044b0: 5365 675a 0c6d 6178 5f65 6c76 655f 7365  SegZ.max_elve_se
-000044c0: 675a 0c6d 696e 5f65 6c76 655f 7365 675a  gZ.min_elve_segZ
-000044d0: 0973 6c6f 7065 5f73 6567 5a05 6e5f 7365  .slope_segZ.n_se
-000044e0: 67da 0573 7562 6964 5a0c 6d61 785f 656c  g..subidZ.max_el
-000044f0: 7665 5f72 6368 5a0c 6d69 6e5f 656c 7665  ve_rchZ.min_elve
-00004500: 5f72 6368 5a0a 6c65 6e67 7468 5f72 6368  _rchZ.length_rch
-00004510: 5a09 716d 6561 6e5f 7263 685a 0977 6964  Z.qmean_rchZ.wid
-00004520: 7468 5f72 6368 5a09 6465 7074 685f 7263  th_rchZ.depth_rc
-00004530: 685a 0a66 6c6f 6f64 6e5f 7263 685a 0973  hZ.floodn_rchZ.s
-00004540: 6c6f 7065 5f72 6368 5a05 6e5f 7263 685a  lope_rchZ.n_rchZ
-00004550: 0663 6174 656c 7672 2000 0000 7221 0000  .catelvr ...r!..
-00004560: 0072 2200 0000 7215 0000 0072 1500 0000  .r"...r....r....
-00004570: 7216 0000 00da 1963 616c 6375 6c61 7465  r......calculate
-00004580: 5f62 6b66 5f77 6964 7468 5f64 6570 7468  _bkf_width_depth
-00004590: 2102 0000 73d6 0000 0000 0106 0114 0108  !...s...........
-000045a0: 0116 010e 010e 010e 0208 0104 0106 0204  ................
-000045b0: 0104 0108 0104 0104 020c 011c 011c 010e  ................
-000045c0: 0212 0112 0118 011a 0226 020a 010a 0214  .........&......
-000045d0: 0108 0110 0122 0120 0204 011e 011e 011e  .....". ........
-000045e0: 011e 011e 011e 011e 0222 011e 0120 0204  ........."... ..
-000045f0: 0104 020c 010a 0104 020e 0214 010e 010e  ................
-00004600: 010e 0114 010e 010e 010e 010e 020a 0114  ................
-00004610: 0110 0204 020a 0114 0110 0204 020e 0214  ................
-00004620: 0114 0104 020a 010a 020e 0214 0114 0104  ................
-00004630: 020a 010a 0216 0116 0116 070a 010a 0106  ................
-00004640: 0204 020a 0116 0116 0116 0614 010a 0118  ................
-00004650: 0216 0214 010a 0118 0216 0214 010a 0118  ................
-00004660: 020a 010c 0124 040c 010c 010c 0118 0272  .....$.........r
-00004670: 1901 0000 2901 7224 0000 0029 2bda 0661  ....).r$...)+..a
-00004680: 7263 6769 7372 0200 0000 da0f 6172 6367  rcgisr......arcg
-00004690: 6973 2e66 6561 7475 7265 7372 0300 0000  is.featuresr....
-000046a0: 7204 0000 0072 0f00 0000 7205 0000 00da  r....r....r.....
-000046b0: 0861 7263 7079 2e73 61da 056e 756d 7079  .arcpy.sa..numpy
-000046c0: 721b 0000 0072 4900 0000 da06 7061 6e64  r....rI.....pand
-000046d0: 6173 7256 0000 0072 7b00 0000 5a11 6172  asrV...r{...Z.ar
-000046e0: 6370 792e 6361 7274 6f67 7261 7068 79da  cpy.cartography.
-000046f0: 0b63 6172 746f 6772 6170 6879 7284 0000  .cartographyr...
-00004700: 0072 8b00 0000 7207 0000 0072 0800 0000  .r....r....r....
-00004710: 728d 0000 0072 8e00 0000 da17 6261 7369  r....r......basi
-00004720: 6e6d 616b 6572 2e66 756e 632e 7064 7461  nmaker.func.pdta
-00004730: 626c 655a 1662 6173 696e 6d61 6b65 722e  bleZ.basinmaker.
-00004740: 6675 6e63 2e72 6172 7261 795a 1e62 6173  func.rarrayZ.bas
-00004750: 696e 6d61 6b65 722e 7574 696c 6974 6965  inmaker.utilitie
-00004760: 732e 7574 696c 6974 6965 73da 076f 7074  s.utilities..opt
-00004770: 696f 6e73 da04 6d6f 6465 da12 6368 6169  ions..mode..chai
-00004780: 6e65 645f 6173 7369 676e 6d65 6e74 7275  ned_assignmentru
-00004790: 0000 00da 1143 6865 636b 4f75 7445 7874  .....CheckOutExt
-000047a0: 656e 7369 6f6e 7217 0000 0072 2300 0000  ensionr....r#...
-000047b0: 7261 0000 0072 6400 0000 7293 0000 0072  ra...rd...r....r
-000047c0: 9c00 0000 72c1 0000 0072 dc00 0000 72f0  ....r....r....r.
-000047d0: 0000 0072 fb00 0000 72fd 0000 0072 0e01  ...r....r....r..
-000047e0: 0000 7219 0100 0072 1500 0000 7215 0000  ..r....r....r...
-000047f0: 0072 1500 0000 7216 0000 00da 083c 6d6f  .r....r......<mo
-00004800: 6475 6c65 3e01 0000 0073 4000 0000 0c01  dule>....s@.....
-00004810: 1001 0801 0c01 0801 0801 0801 0801 0801  ................
-00004820: 0c01 1001 0801 0801 0801 0801 0801 0801  ................
-00004830: 0a02 0801 0a02 080f 081b 0a28 0807 086d  ...........(...m
-00004840: 0807 082c 0835 0842 0826 0815 085f       ...,.5.B.&..._
+000033d0: 1764 26a1 0101 0074 03a0 2c64 2664 2764  .d&....t..,d&d'd
+000033e0: 28a1 0301 0074 1564 277c 0564 0c83 0301  (....t.d'|.d....
+000033f0: 0074 196a 1a6a 1ba0 1c64 1ba1 017d 1e7c  .t.j.j...d...}.|
+00003400: 1e64 2919 007c 1e64 2a3c 007c 1e64 2164  .d)..|.d*<.|.d!d
+00003410: 2a67 0219 007d 1e74 196a 1a6a 1ba0 1c64  *g...}.t.j.j...d
+00003420: 27a1 017d 1f7c 1f6a 1e7c 1e64 2164 1264  '..}.|.j.|.d!d.d
+00003430: 138d 037d 1f7c 1f7c 1f64 2919 007c 1f64  ...}.|.|.d)..|.d
+00003440: 2a19 006b 0019 007d 1f7c 1f6a 2d64 2967  *..k...}.|.j-d)g
+00003450: 0164 2b64 2c8d 027d 1f7c 1f6a 2e64 2167  .d+d,..}.|.j.d!g
+00003460: 0164 2d64 2e8d 027d 1f7c 1f6a 1b6a 2f74  .d-d...}.|.j.j/t
+00003470: 006a 01a0 027c 0c64 017c 0764 2f17 00a1  .j...|.d.|.d/...
+00003480: 0364 0264 2b64 308d 0301 0074 03a0 2c7c  .d.d+d0....t..,|
+00003490: 097c 0964 2f17 0064 28a1 0301 0074 196a  .|.d/..d(....t.j
+000034a0: 1a6a 1ba0 1c7c 0964 2f17 00a1 017d 2074  .j...|.d/....} t
+000034b0: 196a 1a6a 1ba0 1c7c 0764 2f17 00a1 017d  .j.j...|.d/....}
+000034c0: 2174 196a 1a6a 1ba0 1c7c 0864 2f17 00a1  !t.j.j...|.d/...
+000034d0: 017d 2274 196a 307c 207c 217c 2267 0364  .}"t.j0| |!|"g.d
+000034e0: 0264 318d 027d 237c 23a0 31a1 007d 237c  .d1..}#|#.1..}#|
+000034f0: 236a 3264 3217 007c 2364 113c 007c 2364  #j2d2..|#d.<.|#d
+00003500: 1164 3367 0219 007d 237c 236a 1b6a 2f74  .d3g...}#|#j.j/t
+00003510: 006a 01a0 027c 0c64 017c 0664 2f17 00a1  .j...|.d.|.d/...
+00003520: 0364 0264 2b64 308d 0301 007c 1164 1519  .d.d+d0....|.d..
+00003530: 006a 207d 247c 1164 1619 006a 207d 2574  .j }$|.d...j }%t
+00003540: 337c 257c 247c 0f83 035c 027d 267d 277c  3|%|$|...\.}&}'|
+00003550: 267c 2766 0253 0029 344e 72a5 0000 0054  &|'f.S.)4Nr....T
+00003560: 72af 0000 0072 b700 0000 5a0a 7375 625f  r....r....Z.sub_
+00003570: 6f75 746c 6574 5a09 7375 625f 696e 6c65  outletZ.sub_inle
+00003580: 745a 074d 494e 494d 554d 5a0b 7375 625f  tZ.MINIMUMZ.sub_
+00003590: 696e 6c65 745f 76da 0873 6c5f 636c 5f69  inlet_v..sl_cl_i
+000035a0: 64da 0849 4c5f 5375 6249 64da 0a4d 6178  d..IL_SubId..Max
+000035b0: 4163 635f 6361 7472 b200 0000 5a0f 756e  Acc_catr....Z.un
+000035c0: 6971 7565 5f6c 616b 655f 7374 7229 03da  ique_lake_str)..
+000035d0: 0576 616c 7565 72ee 0000 00da 1073 656c  .valuer......sel
+000035e0: 6563 7465 645f 6c61 6b65 735f 7229 0372  ected_lakes_r).r
+000035f0: 0201 0000 7201 0100 0072 0301 0000 72fa  ....r....r....r.
+00003600: 0000 0072 2800 0000 7246 0000 0072 4700  ...r(...rF...rG.
+00003610: 0000 7204 0100 0072 ee00 0000 7205 0100  ..r....r....r...
+00003620: 005a 0c73 7562 5f6f 7574 6c65 745f 725a  .Z.sub_outlet_rZ
+00003630: 1675 6e69 7175 655f 6c61 6b65 5f73 7472  .unique_lake_str
+00003640: 5f69 6e66 6c6f 775a 116c 616b 655f 696e  _inflowZ.lake_in
+00003650: 6c65 745f 696e 6c61 6b65 72e3 0000 005a  let_inlaker....Z
+00003660: 136c 616b 655f 696e 6c65 745f 696e 6c61  .lake_inlet_inla
+00003670: 6b65 5f76 5a15 6c61 6b65 5f69 6e6c 6574  ke_vZ.lake_inlet
+00003680: 5f69 6e6c 616b 655f 7662 6667 0000 0000  _inlake_vbfg....
+00003690: 0000 0440 72d3 0000 0072 d400 0000 72d5  ...@r....r....r.
+000036a0: 0000 0072 b100 0000 5a16 7374 725f 6172  ...r....Z.str_ar
+000036b0: 6f75 6e64 5f6c 616b 655f 696e 6c65 7473  ound_lake_inlets
+000036c0: 72d9 0000 005a 0f6c 616b 655f 696e 666c  r....Z.lake_infl
+000036d0: 6f77 5f73 7472 7a0d 5641 4c55 4520 3d20  ow_strz.VALUE = 
+000036e0: 2d39 3939 395a 1c6c 616b 655f 696e 666c  -9999Z.lake_infl
+000036f0: 6f77 5f73 6567 5f6f 7574 7369 6465 5f6c  ow_seg_outside_l
+00003700: 616b 655a 1e6c 616b 655f 696e 666c 6f77  akeZ.lake_inflow
+00003710: 5f73 6567 5f6f 7574 7369 6465 5f6c 616b  _seg_outside_lak
+00003720: 655f 7672 ad00 0000 da03 6163 635a 0761  e_vr......accZ.a
+00003730: 6363 5f6d 6178 4672 b400 0000 72bc 0000  cc_maxFr....r...
+00003740: 0072 b900 0000 72b0 0000 0072 2900 0000  .r....r....r)...
+00003750: 2901 da0c 6967 6e6f 7265 5f69 6e64 6578  )...ignore_index
+00003760: 726a 0000 0072 4200 0000 2934 724d 0000  rj...rB...)4rM..
+00003770: 0072 4e00 0000 724f 0000 0072 0f00 0000  .rN...rO...r....
+00003780: 7205 0000 0072 a600 0000 727a 0000 0072  r....r....rz...r
+00003790: bd00 0000 72be 0000 0072 5200 0000 7283  ....r....rR...r.
+000037a0: 0000 0072 bf00 0000 72c0 0000 0072 c100  ...r....r....r..
+000037b0: 0000 72c2 0000 0072 c300 0000 72e6 0000  ..r....r....r...
+000037c0: 0072 e700 0000 72e8 0000 0072 ff00 0000  .r....r....r....
+000037d0: 72cf 0000 0072 c800 0000 5a07 436f 6d62  r....r....Z.Comb
+000037e0: 696e 6572 c500 0000 72ac 0000 0072 5400  iner....r....rT.
+000037f0: 0000 7255 0000 0072 4b00 0000 7256 0000  ..rU...rK...rV..
+00003800: 00da 0666 696c 6c6e 6172 5700 0000 5a31  ...fillnarW...Z1
+00003810: 7265 7475 726e 5f6e 6f6e 5f6c 616b 655f  return_non_lake_
+00003820: 696e 666c 6f77 5f73 6567 735f 616e 645f  inflow_segs_and_
+00003830: 7365 6773 5f77 6974 6869 6e5f 6c61 6b65  segs_within_lake
+00003840: 7372 ca00 0000 7200 0100 0072 1d00 0000  sr....r....r....
+00003850: 72ea 0000 0072 1f00 0000 7251 0000 0072  r....r....rQ...r
+00003860: da00 0000 720e 0000 0072 dc00 0000 72c4  ....r....r....r.
+00003870: 0000 0072 dd00 0000 5a07 5365 744e 756c  ...r....Z.SetNul
+00003880: 6c72 c600 0000 72cb 0000 0072 cc00 0000  lr....r....r....
+00003890: 724c 0000 00da 0663 6f6e 6361 74da 0b72  rL.....concat..r
+000038a0: 6573 6574 5f69 6e64 6578 72fc 0000 005a  eset_indexr....Z
+000038b0: 1f43 6865 636b 5f49 665f 4c61 6b65 5f48  .Check_If_Lake_H
+000038c0: 6176 655f 4d75 6c74 695f 4f75 744c 6574  ave_Multi_OutLet
+000038d0: 2928 72ee 0000 0072 fd00 0000 da0b 6361  )(r....r......ca
+000038e0: 745f 6e6f 5f6c 616b 6572 f000 0000 726e  t_no_laker....rn
+000038f0: 0000 0072 0601 0000 5a15 706f 7572 706f  ...r....Z.pourpo
+00003900: 696e 7473 5f77 6974 685f 6c61 6b65 735a  ints_with_lakesZ
+00003910: 166c 616b 655f 696e 666c 6f77 5f70 6f75  .lake_inflow_pou
+00003920: 7270 6f69 6e74 73da 176c 616b 655f 6f75  rpoints..lake_ou
+00003930: 7466 6c6f 775f 706f 7572 706f 696e 7473  tflow_pourpoints
+00003940: 5a21 6361 7463 686d 656e 745f 706f 7572  Z!catchment_pour
+00003950: 706f 696e 7473 5f6f 7574 7369 6465 5f6c  points_outside_l
+00003960: 616b 6572 be00 0000 72cd 0000 0072 a900  aker....r....r..
+00003970: 0000 72c3 0000 0072 f300 0000 5a0c 726f  ..r....r....Z.ro
+00003980: 7574 696e 675f 696e 666f 5a10 4f76 6572  uting_infoZ.Over
+00003990: 6c61 795f 7374 725f 6c61 6b65 5a10 756e  lay_str_lakeZ.un
+000039a0: 6971 5f6c 616b 655f 7374 725f 7064 5a13  iq_lake_str_pdZ.
+000039b0: 7374 725f 7374 6172 745f 7074 5f6c 616b  str_start_pt_lak
+000039c0: 6569 645a 1373 7472 5f69 645f 7769 7468  eidZ.str_id_with
+000039d0: 696e 5f6c 616b 6573 5a14 6e6f 6e5f 6c61  in_lakesZ.non_la
+000039e0: 6b65 5f69 6e66 6c6f 775f 7365 6773 5a12  ke_inflow_segsZ.
+000039f0: 7374 725f 6964 5f6c 616b 655f 696e 6c66  str_id_lake_inlf
+00003a00: 6f77 da04 7465 6d70 5a20 6c61 6b65 5f69  ow..tempZ lake_i
+00003a10: 6e66 6c6f 775f 756e 6971 7565 5f6c 616b  nflow_unique_lak
+00003a20: 6573 7472 5f61 7272 6179 5a1e 6c61 6b65  estr_arrayZ.lake
+00003a30: 5f69 6e66 6c6f 775f 756e 6971 7565 5f6c  _inflow_unique_l
+00003a40: 616b 6573 7472 5f69 6473 5a11 6c61 6b65  akestr_idsZ.lake
+00003a50: 5f69 6e6c 6574 5f73 7562 6964 735a 0a65  _inlet_subidsZ.e
+00003a60: 7863 6c75 6465 6964 735a 2372 656d 6f76  xcludeidsZ#remov
+00003a70: 655f 7661 6c75 655f 6e6f 745f 6f6e 5f6c  e_value_not_on_l
+00003a80: 616b 655f 696e 666c 6f77 5f73 7472 5a19  ake_inflow_strZ.
+00003a90: 7265 6d6f 7665 5f76 616c 7565 5f69 6e73  remove_value_ins
+00003aa0: 6964 655f 6c61 6b65 735a 1f72 656d 6f76  ide_lakesZ.remov
+00003ab0: 655f 7661 6c75 655f 696e 7369 6465 5f6c  e_value_inside_l
+00003ac0: 616b 6573 5f6e 6f39 3939 5a12 696e 6c65  akes_no999Z.inle
+00003ad0: 745f 696e 6c61 6b65 5f74 6162 6c65 5a18  t_inlake_tableZ.
+00003ae0: 696e 6c65 745f 6f75 7473 6964 655f 6c61  inlet_outside_la
+00003af0: 6b65 5f74 6162 6c65 5a0a 6361 745f 6f75  ke_tableZ.cat_ou
+00003b00: 746c 6574 5a0b 6c61 6b65 5f69 6e6c 6574  tletZ.lake_inlet
+00003b10: 735a 0c6c 616b 655f 6f75 746c 6574 735a  sZ.lake_outletsZ
+00003b20: 1770 6f75 7270 6f69 6e74 735f 7769 7468  .pourpoints_with
+00003b30: 6c61 6b65 5f76 6172 5a06 5374 725f 4964  lake_varZ.Str_Id
+00003b40: 5a05 434c 5f49 645a 174c 616b 6573 5f57  Z.CL_IdZ.Lakes_W
+00003b50: 4974 685f 4d75 6c74 695f 4f75 746c 6574  Ith_Multi_Outlet
+00003b60: 5a0a 5265 6d6f 7665 5f53 7472 7213 0000  Z.Remove_Strr...
+00003b70: 0072 1300 0000 7214 0000 00da 1d63 7265  .r....r......cre
+00003b80: 6174 655f 706f 7572 5f70 6f69 6e74 735f  ate_pour_points_
+00003b90: 7769 7468 5f6c 616b 6573 c201 0000 738c  with_lakes....s.
+00003ba0: 0000 0000 0412 0108 0108 010a 0114 0110  ................
+00003bb0: 0108 0120 0310 021a 0116 0116 0422 0110  ... ........."..
+00003bc0: 010a 0210 010e 010c 010a 010c 0210 0502  ................
+00003bd0: 0124 ff02 fc02 0102 0102 0102 0614 0318  .$..............
+00003be0: 0316 030a 010c 0218 0320 030a 0106 ff04  ......... ......
+00003bf0: 041a 0114 0210 0114 010c 010a 030e 010c  ................
+00003c00: 030e 010c 010c 010e 0210 0114 0210 0110  ................
+00003c10: 0122 0412 0212 0112 0112 0214 0108 010e  ."..............
+00003c20: 010c 0122 020a 010a 0202 0106 ff08 0472  ..."...........r
+00003c30: 0e01 0000 6301 0000 0000 0000 0000 0000  ....c...........
+00003c40: 002a 0000 0007 0000 0043 0000 0073 c006  .*.......C...s..
+00003c50: 0000 7c00 6a00 7d01 7401 6401 7402 7c01  ..|.j.}.t.d.t.|.
+00003c60: 8301 8302 4400 9001 5d1c 7d02 7c01 7c02  ....D...].}.|.|.
+00003c70: 1900 7d03 7c00 6a03 7c03 6402 6602 1900  ..}.|.j.|.d.f...
+00003c80: 6403 1b00 6403 1b00 7d04 7c00 6a03 7c03  d...d...}.|.j.|.
+00003c90: 6404 6602 1900 7d05 7c00 6a03 7c03 6405  d.f...}.|.j.|.d.
+00003ca0: 6602 1900 7d06 7c00 6a03 7c03 6406 6602  f...}.|.j.|.d.f.
+00003cb0: 1900 7d07 7c06 6401 6b00 7274 6407 7d08  ..}.|.d.k.rtd.}.
+00003cc0: 6408 7d09 6e18 7c06 7d08 7c07 7d09 7c08  d.}.n.|.}.|.}.|.
+00003cd0: 6401 6b00 728c 6407 7d08 6408 7d09 7404  d.k.r.d.}.d.}.t.
+00003ce0: 7c04 7c08 7c09 8303 7d0a 7405 6409 7c0a  |.|.|...}.t.d.|.
+00003cf0: 640a 1300 1400 7406 8302 7c00 6a03 7c03  d.....t...|.j.|.
+00003d00: 640b 6602 3c00 7405 640c 7c0a 640d 1300  d.f.<.t.d.|.d...
+00003d10: 1400 7407 8302 7c00 6a03 7c03 640e 6602  ..t...|.j.|.d.f.
+00003d20: 3c00 7c0a 7c00 6a03 7c03 640f 6602 3c00  <.|.|.j.|.d.f.<.
+00003d30: 7c00 6a03 7c03 6410 6602 1900 6411 6b00  |.j.|.d.f...d.k.
+00003d40: 7214 7c00 6a03 7c03 6412 6602 1900 6401  r.|.j.|.d.f...d.
+00003d50: 6b00 7214 7c00 6a03 7c03 6413 6602 1900  k.r.|.j.|.d.f...
+00003d60: 7c00 6a03 7c03 6412 6602 3c00 7c00 6a03  |.j.|.d.f.<.|.j.
+00003d70: 7c03 6413 6602 1900 7c00 6a03 7c03 6414  |.d.f...|.j.|.d.
+00003d80: 6602 3c00 7114 7c00 6a03 7c00 6410 1900  f.<.q.|.j.|.d...
+00003d90: 6411 6b00 7c00 6415 1900 6416 6b03 4000  d.k.|.d...d.k.@.
+00003da0: 1900 6a08 6417 6418 8d01 7d0b 7c0b 6419  ..j.d.d...}.|.d.
+00003db0: 1900 6a09 7d0c 740a a00b 7c0c a101 7d0c  ..j.}.t...|...}.
+00003dc0: 7401 6401 7402 7c0c 8301 8302 4400 9005  t.d.t.|.....D...
+00003dd0: 5d00 7d0d 7c0c 7c0d 1900 7d0e 7c0b 7c0b  ].}.|.|...}.|.|.
+00003de0: 6419 1900 7c0e 6b02 1900 7d0f 7402 7c0f  d...|.k...}.t.|.
+00003df0: 6415 1900 6a09 7c0f 6415 1900 6a09 6401  d...j.|.d...j.d.
+00003e00: 6b04 1900 8301 6401 6b04 9001 72dc 740a  k.....d.k...r.t.
+00003e10: a00c 7c0f 6415 1900 6a09 7c0f 6415 1900  ..|.d...j.|.d...
+00003e20: 6a09 6401 6b04 1900 a101 7d10 6e04 641a  j.d.k.....}.n.d.
+00003e30: 7d10 740a a00d 7c0f 640f 1900 6a09 7c0f  }.t...|.d...j.|.
+00003e40: 640f 1900 6a09 6401 6b04 1900 a101 7d11  d...j.d.k.....}.
+00003e50: 740a a00d 7c0f 640b 1900 6a09 7c0f 640b  t...|.d...j.|.d.
+00003e60: 1900 6a09 6401 6b04 1900 a101 7d12 740a  ..j.d.k.....}.t.
+00003e70: a00d 7c0f 640e 1900 6a09 7c0f 640e 1900  ..|.d...j.|.d...
+00003e80: 6a09 6401 6b04 1900 a101 7d13 740a a00d  j.d.k.....}.t...
+00003e90: 7c0f 641b 1900 6a09 7c0f 641b 1900 6a09  |.d...j.|.d...j.
+00003ea0: 6401 6b04 1900 a101 7d14 740a a00d 7c0f  d.k.....}.t...|.
+00003eb0: 641c 1900 6a09 7c0f 641c 1900 6a09 6401  d...j.|.d...j.d.
+00003ec0: 6b04 1900 a101 7d15 740a a00d 7c0f 641d  k.....}.t...|.d.
+00003ed0: 1900 6a09 7c0f 641d 1900 6a09 6401 6b04  ..j.|.d...j.d.k.
+00003ee0: 1900 a101 7d16 740a a00d 7c0f 6413 1900  ....}.t...|.d...
+00003ef0: 6a09 7c0f 6413 1900 6a09 6401 6b04 1900  j.|.d...j.d.k...
+00003f00: a101 7d17 7402 7c0f 6412 1900 6a09 7c0f  ..}.t.|.d...j.|.
+00003f10: 6412 1900 6a09 641e 6b04 1900 8301 6401  d...j.d.k.....d.
+00003f20: 6b04 9003 7212 740a a005 7c0f 6412 1900  k...r.t...|.d...
+00003f30: 6a09 7c0f 6412 1900 6a09 641f 6b04 1900  j.|.d...j.d.k...
+00003f40: a101 7d18 740a a00e 7c0f 6414 1900 6a09  ..}.t...|.d...j.
+00003f50: 7c0f 6414 1900 6a09 641f 6b04 1900 a101  |.d...j.d.k.....
+00003f60: 7d19 6e08 7c17 7d18 7c17 7d19 7c18 7c19  }.n.|.}.|.}.|.|.
+00003f70: 1800 7c10 1b00 7d1a 7c1a 6420 6b00 9003  ..|...}.|.d k...
+00003f80: 7234 740f 7d1a 7410 7c12 7c13 7c11 7c1a  r4t.}.t.|.|.|.|.
+00003f90: 8304 7d1b 7401 6401 7402 7c0f 8301 8302  ..}.t.d.t.|.....
+00003fa0: 4400 9003 5d28 7d02 7c0f 6404 1900 6a09  D...](}.|.d...j.
+00003fb0: 7c02 1900 7d1c 7c0f 6412 1900 6a09 7c02  |...}.|.d...j.|.
+00003fc0: 1900 7d1d 7c0f 6414 1900 6a09 7c02 1900  ..}.|.d...j.|...
+00003fd0: 7d1e 7405 7c0f 6415 1900 6a09 7c02 1900  }.t.|.d...j.|...
+00003fe0: 7411 8302 7d1f 7c0f 640f 1900 6a09 7c02  t...}.|.d...j.|.
+00003ff0: 1900 7d20 7c0f 640b 1900 6a09 7c02 1900  ..} |.d...j.|...
+00004000: 7d21 7c0f 640e 1900 6a09 7c02 1900 7d22  }!|.d...j.|...}"
+00004010: 7c0f 641b 1900 6a09 7c02 1900 7d23 7c1e  |.d...j.|...}#|.
+00004020: 6421 6b00 9003 72fe 7c0f 6413 1900 6a09  d!k...r.|.d...j.
+00004030: 7c02 1900 6421 6b04 9003 72fa 7c0f 6413  |...d!k...r.|.d.
+00004040: 1900 6a09 7c02 1900 7d1e 6e04 7c17 7d1e  ..j.|...}.n.|.}.
+00004050: 7c1d 6421 6b00 9004 7230 7c0f 6413 1900  |.d!k...r0|.d...
+00004060: 6a09 7c02 1900 6421 6b04 9004 722c 7c0f  j.|...d!k...r,|.
+00004070: 6413 1900 6a09 7c02 1900 7d1d 6e04 7c17  d...j.|...}.n.|.
+00004080: 7d1d 7c0f 6422 1900 6a09 7c02 1900 7d24  }.|.d"..j.|...}$
+00004090: 7c24 740f 6b00 9004 7352 7c24 7412 6b04  |$t.k...sR|$t.k.
+000040a0: 9004 726a 7c1a 740f 6b05 9004 726a 7c1a  ..rj|.t.k...rj|.
+000040b0: 7412 6b01 9004 726a 7c1a 7d24 7405 7c24  t.k...rj|.}$t.|$
+000040c0: 740f 8302 7d24 740e 7c24 7412 8302 7d24  t...}$t.|$t...}$
+000040d0: 7410 7c21 7c22 7c20 7c24 8304 7d25 7c25  t.|!|"| |$..}%|%
+000040e0: 7413 6b00 9004 73a0 7c25 7414 6b04 9004  t.k...s.|%t.k...
+000040f0: 72b8 7c1b 7413 6b05 9004 72b8 7c1b 7414  r.|.t.k...r.|.t.
+00004100: 6b01 9004 72b8 7c1b 7d25 7405 7c25 7413  k...r.|.}%t.|%t.
+00004110: 8302 7d25 740e 7c25 7414 8302 7d25 7c24  ..}%t.|%t...}%|$
+00004120: 7c00 6a03 7c00 6404 1900 7c1c 6b02 6422  |.j.|.d...|.k.d"
+00004130: 6602 3c00 7c25 7c00 6a03 7c00 6404 1900  f.<.|%|.j.|.d...
+00004140: 7c1c 6b02 6423 6602 3c00 7c1f 7c00 6a03  |.k.d#f.<.|.|.j.
+00004150: 7c00 6404 1900 7c1c 6b02 6415 6602 3c00  |.d...|.k.d.f.<.
+00004160: 7c23 6401 6b00 9005 722c 7c14 6401 6b04  |#d.k...r,|.d.k.
+00004170: 9005 7228 7c14 7d23 6e04 7415 7d23 7405  ..r(|.}#n.t.}#t.
+00004180: 7c23 7c25 8302 7d23 7c23 7c00 6a03 7c00  |#|%..}#|#|.j.|.
+00004190: 6404 1900 7c1c 6b02 641b 6602 3c00 7c1d  d...|.k.d.f.<.|.
+000041a0: 7c00 6a03 7c00 6404 1900 7c1c 6b02 6412  |.j.|.d...|.k.d.
+000041b0: 6602 3c00 7c1e 7c00 6a03 7c00 6404 1900  f.<.|.|.j.|.d...
+000041c0: 7c1c 6b02 6414 6602 3c00 7c0f 641c 1900  |.k.d.f.<.|.d...
+000041d0: 6a09 7c02 1900 6401 6b01 9005 72c4 7c15  j.|...d.k...r.|.
+000041e0: 6401 6b04 9005 72ae 7c15 7c00 6a03 7c00  d.k...r.|.|.j.|.
+000041f0: 6404 1900 7c1c 6b02 641c 6602 3c00 6e16  d...|.k.d.f.<.n.
+00004200: 6401 7c00 6a03 7c00 6404 1900 7c1c 6b02  d.|.j.|.d...|.k.
+00004210: 641c 6602 3c00 7c0f 641d 1900 6a09 7c02  d.f.<.|.d...j.|.
+00004220: 1900 6401 6b01 9006 7210 7c16 6401 6b04  ..d.k...r.|.d.k.
+00004230: 9005 72fa 7c16 7c00 6a03 7c00 6404 1900  ..r.|.|.j.|.d...
+00004240: 7c1c 6b02 641d 6602 3c00 6e16 6401 7c00  |.k.d.f.<.n.d.|.
+00004250: 6a03 7c00 6404 1900 7c1c 6b02 641d 6602  j.|.d...|.k.d.f.
+00004260: 3c00 7c0f 6413 1900 6a09 7c02 1900 6401  <.|.d...j.|...d.
+00004270: 6b00 9003 7250 7c17 6401 6b04 9006 7246  k...rP|.d.k...rF
+00004280: 7c17 7c00 6a03 7c00 6404 1900 7c1c 6b02  |.|.j.|.d...|.k.
+00004290: 6413 6602 3c00 6e32 7c00 6413 1900 6a09  d.f.<.n2|.d...j.
+000042a0: 7d26 7c26 7c26 6401 6b04 1900 7d26 740a  }&|&|&d.k...}&t.
+000042b0: a00d 7c26 a101 7c00 6a03 7c00 6404 1900  ..|&..|.j.|.d...
+000042c0: 7c1c 6b02 6413 6602 3c00 9003 7150 9001  |.k.d.f.<...qP..
+000042d0: 717c 7c00 6424 1900 740f 6b00 7d27 7c00  q||.d$..t.k.}'|.
+000042e0: 6424 1900 7412 6b04 7d28 740a a016 7c27  d$..t.k.}(t...|'
+000042f0: 7c28 a102 7d29 7c00 6a03 7c29 6422 6602  |(..})|.j.|)d"f.
+00004300: 1900 7c00 6a03 7c29 6424 6602 3c00 7c00  ..|.j.|)d$f.<.|.
+00004310: 5300 2925 4e72 0100 0000 5a09 4472 6169  S.)%Nr....Z.Drai
+00004320: 6e41 7265 6169 e803 0000 7228 0000 00da  nAreai....r(....
+00004330: 016b da01 6367 c1ab 27eb 1e76 723f 6799  .k..cg..'..vr?g.
+00004340: 7211 21a6 8bef 3f67 cdcc cccc cccc 1c40  r.!...?g.......@
+00004350: 72d2 0000 005a 0842 6b66 5769 6474 6867  r....Z.BkfWidthg
+00004360: 48e1 7a14 ae47 d13f 6733 3333 3333 33d3  H.z..G.?g333333.
+00004370: 3f5a 0842 6b66 4465 7074 685a 0651 5f4d  ?Z.BkfDepthZ.Q_M
+00004380: 6561 6e72 1700 0000 7218 0000 00da 074d  eanr....r......M
+00004390: 6178 5f44 454d 5a08 4d65 616e 456c 6576  ax_DEMZ.MeanElev
+000043a0: da07 4d69 6e5f 4445 4d72 4a00 0000 72f9  ..Min_DEMrJ...r.
+000043b0: 0000 0054 72d7 0000 005a 0653 6567 5f49  ...Tr....Z.Seg_I
+000043c0: 4472 6a00 0000 da08 466c 6f6f 6450 5f6e  Drj.....FloodP_n
+000043d0: 5a08 4261 7353 6c6f 7065 5a09 4261 7341  Z.BasSlopeZ.BasA
+000043e0: 7370 6563 746c fcff ffff ff7f c74e ce5a  spectl.......N.Z
+000043f0: 056f 6cfc ffff ffff 7f81 5fc9 1b1c 0167  .ol......._....g
+00004400: 95d6 26e8 0b2e 113e 6930 f8ff ffda 0852  ..&....>i0.....R
+00004410: 6976 536c 6f70 65da 0443 685f 6e5a 0a44  ivSlope..Ch_nZ.D
+00004420: 415f 4368 6e5f 536c 7029 1772 fc00 0000  A_Chn_Slp).r....
+00004430: 720c 0000 0072 0d00 0000 7221 0000 005a  r....r....r!...Z
+00004440: 0966 756e 635f 515f 4441 da03 6d61 785a  .func_Q_DA..maxZ
+00004450: 0d6d 696e 5f62 6b66 5f77 6964 7468 5a0d  .min_bkf_widthZ.
+00004460: 6d69 6e5f 626b 665f 6465 7074 6872 8b00  min_bkf_depthr..
+00004470: 0000 72ca 0000 0072 1d00 0000 72ea 0000  ..r....r....r...
+00004480: 00da 0373 756d da07 6176 6572 6167 65da  ...sum..average.
+00004490: 036d 696e 5a0d 6d69 6e5f 7269 765f 736c  .minZ.min_riv_sl
+000044a0: 6f70 655a 1163 616c 6375 6c61 7465 4368  opeZ.calculateCh
+000044b0: 616e 6e61 6c6e 5a0d 6d69 6e5f 7269 765f  annalnZ.min_riv_
+000044c0: 6c65 6e74 685a 0d6d 6178 5f72 6976 5f73  lenthZ.max_riv_s
+000044d0: 6c6f 7065 5a0d 6d69 6e5f 6d61 6e6e 696e  lopeZ.min_mannin
+000044e0: 675f 6e5a 0d6d 6178 5f6d 616e 6e69 6e67  g_nZ.max_manning
+000044f0: 5f6e 5a0f 4445 4641 4c55 545f 464c 4f4f  _nZ.DEFALUT_FLOO
+00004500: 445f 4e72 5800 0000 292a 5a07 6361 7469  D_NrX...)*Z.cati
+00004510: 6e66 6f72 fe00 0000 7212 0000 005a 0569  nfor....r....Z.i
+00004520: 6478 5f69 72a7 0000 005a 0563 6174 6964  dx_ir....Z.catid
+00004530: 720f 0100 0072 1001 0000 5a05 6b5f 7375  r....r....Z.k_su
+00004540: 625a 0563 5f73 7562 da01 715a 0b63 6174  bZ.c_sub..qZ.cat
+00004550: 696e 666f 5f72 6976 5a07 5365 675f 4944  info_rivZ.Seg_ID
+00004560: 535a 0469 7365 675a 0869 5f73 6567 5f69  SZ.isegZ.i_seg_i
+00004570: 645a 0a69 5f73 6567 5f69 6e66 6f5a 0a6c  dZ.i_seg_infoZ.l
+00004580: 656e 6774 685f 7365 675a 0971 6d65 616e  ength_segZ.qmean
+00004590: 5f73 6567 5a09 7769 6474 685f 7365 675a  _segZ.width_segZ
+000045a0: 0964 6570 7468 5f53 6567 5a0a 666c 6f6f  .depth_SegZ.floo
+000045b0: 646e 5f53 6567 5a0a 6261 7373 6c70 5f53  dn_SegZ.basslp_S
+000045c0: 6567 5a0a 6261 7361 7370 5f53 6567 5a0a  egZ.basasp_SegZ.
+000045d0: 6261 7365 6c76 5f53 6567 5a0c 6d61 785f  baselv_SegZ.max_
+000045e0: 656c 7665 5f73 6567 5a0c 6d69 6e5f 656c  elve_segZ.min_el
+000045f0: 7665 5f73 6567 5a09 736c 6f70 655f 7365  ve_segZ.slope_se
+00004600: 675a 056e 5f73 6567 da05 7375 6269 645a  gZ.n_seg..subidZ
+00004610: 0c6d 6178 5f65 6c76 655f 7263 685a 0c6d  .max_elve_rchZ.m
+00004620: 696e 5f65 6c76 655f 7263 685a 0a6c 656e  in_elve_rchZ.len
+00004630: 6774 685f 7263 685a 0971 6d65 616e 5f72  gth_rchZ.qmean_r
+00004640: 6368 5a09 7769 6474 685f 7263 685a 0964  chZ.width_rchZ.d
+00004650: 6570 7468 5f72 6368 5a0a 666c 6f6f 646e  epth_rchZ.floodn
+00004660: 5f72 6368 5a09 736c 6f70 655f 7263 685a  _rchZ.slope_rchZ
+00004670: 056e 5f72 6368 5a06 6361 7465 6c76 7224  .n_rchZ.catelvr$
+00004680: 0000 0072 2500 0000 7226 0000 0072 1300  ...r%...r&...r..
+00004690: 0000 7213 0000 0072 1400 0000 da19 6361  ..r....r......ca
+000046a0: 6c63 756c 6174 655f 626b 665f 7769 6474  lculate_bkf_widt
+000046b0: 685f 6465 7074 6833 0200 0073 d600 0000  h_depth3...s....
+000046c0: 0001 0601 1401 0801 1601 0e01 0e01 0e02  ................
+000046d0: 0801 0401 0602 0401 0401 0801 0401 0402  ................
+000046e0: 0c01 1c01 1c01 0e02 1201 1201 1801 1a02  ................
+000046f0: 2602 0a01 0a02 1401 0801 1001 2201 2002  &...........". .
+00004700: 0401 1e01 1e01 1e01 1e01 1e01 1e01 1e02  ................
+00004710: 2201 1e01 2002 0401 0402 0c01 0a01 0402  "... ...........
+00004720: 0e02 1401 0e01 0e01 0e01 1401 0e01 0e01  ................
+00004730: 0e01 0e02 0a01 1401 1002 0402 0a01 1401  ................
+00004740: 1002 0402 0e02 1401 1401 0402 0a01 0a02  ................
+00004750: 0e02 1401 1401 0402 0a01 0a02 1601 1601  ................
+00004760: 1607 0a01 0a01 0602 0402 0a01 1601 1601  ................
+00004770: 1606 1401 0a01 1802 1602 1401 0a01 1802  ................
+00004780: 1602 1401 0a01 1802 0a01 0c01 2404 0c01  ............$...
+00004790: 0c01 0c01 1802 721c 0100 0029 0172 2800  ......r....).r(.
+000047a0: 0000 292b da06 6172 6367 6973 7202 0000  ..)+..arcgisr...
+000047b0: 005a 0f61 7263 6769 732e 6665 6174 7572  .Z.arcgis.featur
+000047c0: 6573 7203 0000 0072 0400 0000 720f 0000  esr....r....r...
+000047d0: 0072 0500 0000 5a08 6172 6370 792e 7361  .r....Z.arcpy.sa
+000047e0: da05 6e75 6d70 7972 1d00 0000 724d 0000  ..numpyr....rM..
+000047f0: 00da 0670 616e 6461 7372 5400 0000 7280  ...pandasrT...r.
+00004800: 0000 005a 1161 7263 7079 2e63 6172 746f  ...Z.arcpy.carto
+00004810: 6772 6170 6879 5a0b 6361 7274 6f67 7261  graphyZ.cartogra
+00004820: 7068 7972 8400 0000 7288 0000 0072 0700  phyr....r....r..
+00004830: 0000 7208 0000 0072 8a00 0000 728b 0000  ..r....r....r...
+00004840: 00da 1762 6173 696e 6d61 6b65 722e 6675  ...basinmaker.fu
+00004850: 6e63 2e70 6474 6162 6c65 da16 6261 7369  nc.pdtable..basi
+00004860: 6e6d 616b 6572 2e66 756e 632e 7261 7272  nmaker.func.rarr
+00004870: 6179 da1e 6261 7369 6e6d 616b 6572 2e75  ay..basinmaker.u
+00004880: 7469 6c69 7469 6573 2e75 7469 6c69 7469  tilities.utiliti
+00004890: 6573 da07 6f70 7469 6f6e 73da 046d 6f64  es..options..mod
+000048a0: 65da 1263 6861 696e 6564 5f61 7373 6967  e..chained_assig
+000048b0: 6e6d 656e 7472 7a00 0000 da11 4368 6563  nmentrz.....Chec
+000048c0: 6b4f 7574 4578 7465 6e73 696f 6e72 1500  kOutExtensionr..
+000048d0: 0000 7227 0000 0072 6400 0000 7268 0000  ..r'...rd...rh..
+000048e0: 0072 a400 0000 72ac 0000 0072 cf00 0000  .r....r....r....
+000048f0: 72e2 0000 0072 f400 0000 72ff 0000 0072  r....r....r....r
+00004900: 0001 0000 720e 0100 0072 1c01 0000 7213  ....r....r....r.
+00004910: 0000 0072 1300 0000 7213 0000 0072 1400  ...r....r....r..
+00004920: 0000 da08 3c6d 6f64 756c 653e 0100 0000  ....<module>....
+00004930: 7340 0000 000c 0110 0108 010c 0108 0108  s@..............
+00004940: 0108 0108 0108 010c 0110 0108 0108 0108  ................
+00004950: 0108 0108 0108 010a 0208 010a 0208 0f08  ................
+00004960: 1b0a 2808 0708 6d08 0708 2c08 3508 4208  ..(...m...,.5.B.
+00004970: 2608 1508 71                             &...q
```

### Comparing `basinmaker-3.0.3a0/basinmaker/func/__pycache__/fgdal.cpython-39.pyc` & `basinmaker-3.1.0/basinmaker/func/__pycache__/fgdal.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `basinmaker-3.0.3a0/basinmaker/func/__pycache__/grassgis.cpython-39.pyc` & `basinmaker-3.1.0/basinmaker/func/__pycache__/grassgis.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `basinmaker-3.0.3a0/basinmaker/func/__pycache__/pdtable.cpython-39.pyc` & `basinmaker-3.1.0/basinmaker/func/__pycache__/pdtable.cpython-39.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.9, timestamp-based, .py timestamp: Sat Apr  1 13:38:19 2023 UTC, .py size: 139946 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 6% similar despite different names*

```diff
@@ -1,2988 +1,3157 @@
-00000000: 610d 0d0a 0000 0000 cb33 2864 aa22 0200  a........3(d."..
+00000000: 610d 0d0a 0000 0000 26d3 6664 b052 0200  a.......&.fd.R..
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
-00000020: 0006 0000 0040 0000 0073 9601 0000 6400  .....@...s....d.
+00000020: 0006 0000 0040 0000 0073 ae01 0000 6400  .....@...s....d.
 00000030: 6401 6c00 5a00 6400 6401 6c01 5a02 6400  d.l.Z.d.d.l.Z.d.
 00000040: 6401 6c03 5a04 6400 6402 6c05 6d06 5a06  d.l.Z.d.d.l.m.Z.
 00000050: 0100 6400 6403 6c07 5400 6400 6401 6c08  ..d.d.l.T.d.d.l.
 00000060: 5a08 6400 6404 6c09 6d0a 5a0a 6d0b 5a0b  Z.d.d.l.m.Z.m.Z.
 00000070: 0100 6400 6401 6c0c 5a0c 6401 6504 6a0d  ..d.d.l.Z.d.e.j.
 00000080: 6a0e 5f0f 6405 6406 8400 5a10 6407 6408  j._.d.d...Z.d.d.
 00000090: 8400 5a11 6409 640a 8400 5a12 640b 640c  ..Z.d.d...Z.d.d.
 000000a0: 8400 5a13 640d 640e 8400 5a14 640f 6410  ..Z.d.d...Z.d.d.
 000000b0: 8400 5a15 6411 6412 8400 5a16 6413 6414  ..Z.d.d...Z.d.d.
-000000c0: 8400 5a17 6451 6416 6417 8401 5a18 6418  ..Z.dQd.d...Z.d.
-000000d0: 6418 6418 6701 6418 6701 6418 6418 6606  d.d.g.d.g.d.d.f.
-000000e0: 6419 641a 8401 5a19 6452 641c 641d 8401  d.d...Z.dRd.d...
-000000f0: 5a1a 6453 641e 641f 8401 5a1b 6420 6421  Z.dSd.d...Z.d d!
-00000100: 8400 5a1c 6422 6423 8400 5a1d 6424 6425  ..Z.d"d#..Z.d$d%
-00000110: 8400 5a1e 6426 6427 8400 5a1f 6428 6429  ..Z.d&d'..Z.d(d)
-00000120: 8400 5a20 642a 642b 8400 5a21 642c 642d  ..Z d*d+..Z!d,d-
-00000130: 8400 5a22 642e 642f 8400 5a23 6430 6431  ..Z"d.d/..Z#d0d1
-00000140: 8400 5a24 6432 6433 8400 5a25 6434 6435  ..Z$d2d3..Z%d4d5
-00000150: 8400 5a26 6436 6437 8400 5a27 6438 6439  ..Z&d6d7..Z'd8d9
-00000160: 8400 5a28 643a 643b 8400 5a29 643c 643d  ..Z(d:d;..Z)d<d=
-00000170: 8400 5a2a 643e 643f 8400 5a2b 6440 6441  ..Z*d>d?..Z+d@dA
-00000180: 8400 5a2c 6454 6442 6443 8401 5a2d 6444  ..Z,dTdBdC..Z-dD
-00000190: 6445 8400 5a2e 6446 6447 8400 5a2f 6448  dE..Z.dFdG..Z/dH
-000001a0: 6449 8400 5a30 6455 644b 644c 8401 5a31  dI..Z0dUdKdL..Z1
-000001b0: 644d 644e 8400 5a32 644f 6450 8400 5a33  dMdN..Z2dOdP..Z3
-000001c0: 6401 5300 2956 e900 0000 004e 2901 da09  d.S.)V.....N)...
-000001d0: 6375 7276 655f 6669 7429 01da 012a 2902  curve_fit)...*).
-000001e0: da08 5061 7261 6c6c 656c da07 6465 6c61  ..Parallel..dela
-000001f0: 7965 6463 0400 0000 0000 0000 0000 0000  yedc............
-00000200: 1200 0000 0600 0000 4300 0000 7352 0100  ........C...sR..
-00000210: 0064 017d 0464 017d 0564 017d 0664 017d  .d.}.d.}.d.}.d.}
-00000220: 077c 007c 0064 0219 00a0 007c 0064 0319  .|.|.d.....|.d..
-00000230: 006a 01a1 010f 0019 007d 087c 0864 0219  .j.......}.|.d..
-00000240: 00a0 007c 01a1 016a 0264 0464 058d 017d  ...|...j.d.d...}
-00000250: 097c 087c 0919 007d 0a74 037c 0a83 0164  .|.|...}.t.|...d
-00000260: 066b 0172 5e7c 017c 027c 0766 0353 007c  .k.r^|.|.|.f.S.|
-00000270: 0a7c 0a64 0319 00a0 007c 01a1 010f 0019  .|.d.....|......
-00000280: 006a 0264 0464 058d 017d 0b74 037c 0b83  .j.d.d...}.t.|..
-00000290: 0164 066b 0172 907c 017c 027c 0766 0353  .d.k.r.|.|.|.f.S
-000002a0: 007c 0064 0364 0267 0219 00a0 0464 07a1  .|.d.d.g.....d..
-000002b0: 016a 017d 0c7c 0b64 0319 006a 0144 005d  .j.}.|.d...j.D.]
-000002c0: 947d 0d74 057c 0c7c 0d83 027d 0e7c 007c  .}.t.|.|...}.|.|
-000002d0: 0064 0319 00a0 007c 0ea1 0119 007d 0f7c  .d.....|.....}.|
-000002e0: 026a 067c 0f64 0364 0864 098d 037d 027c  .j.|.d.d.d...}.|
-000002f0: 0264 0319 00a0 007c 0ea1 017d 107c 026a  .d.....|...}.|.j
-00000300: 077c 1064 0266 0219 006a 017c 026a 077c  .|.d.f...j.|.j.|
-00000310: 1064 0a66 023c 007c 0264 0364 0a67 0219  .d.f.<.|.d.d.g..
-00000320: 00a0 0464 07a1 016a 017d 0374 057c 037c  ...d...j.}.t.|.|
-00000330: 0d83 027d 1174 086a 097c 017c 1166 0264  ...}.t.j.|.|.f.d
-00000340: 0664 0b8d 027d 017c 026a 0a64 0264 0c8d  .d...}.|.j.d.d..
-00000350: 017d 0271 ae64 047d 077c 017c 027c 0766  .}.q.d.}.|.|.|.f
-00000360: 0353 0029 0d4e 465a 0c53 6563 5f44 6f77  .S.).NFZ.Sec_Dow
-00000370: 5375 6249 64da 0553 7562 4964 54a9 01da  SubId..SubIdT...
-00000380: 0464 6565 7072 0100 0000 da05 696e 7433  .deepr......int3
-00000390: 32da 046c 6566 7429 02da 026f 6eda 0368  2..left)...on..h
-000003a0: 6f77 da08 446f 7753 7562 4964 a901 da04  ow..DowSubId....
-000003b0: 6178 6973 a901 da07 636f 6c75 6d6e 7329  axis....columns)
-000003c0: 0bda 0469 7369 6eda 0676 616c 7565 73da  ...isin..values.
-000003d0: 0463 6f70 79da 036c 656e da06 6173 7479  .copy..len..asty
-000003e0: 7065 da06 6465 6663 6174 da05 6d65 7267  pe..defcat..merg
-000003f0: 65da 036c 6f63 da02 6e70 da0b 636f 6e63  e..loc..np..conc
-00000400: 6174 656e 6174 65da 0464 726f 7029 12da  atenate..drop)..
-00000410: 1073 6563 5f64 6f77 6e5f 7375 6269 6e66  .sec_down_subinf
-00000420: 6fda 0d75 7073 7472 6561 6d5f 7375 6273  o..upstream_subs
-00000430: da07 6361 745f 706c 79da 0968 7973 6864  ..cat_ply..hyshd
-00000440: 696e 666f 5a23 6973 5f73 6563 5f64 6f77  infoZ#is_sec_dow
-00000450: 6e5f 7375 6269 645f 696e 5f73 656c 6563  n_subid_in_selec
-00000460: 7465 645f 7375 6269 645a 2b69 735f 7375  ted_subidZ+is_su
-00000470: 6269 645f 6f66 5f73 6563 5f64 6f77 6e73  bid_of_sec_downs
-00000480: 7562 6964 5f69 6e5f 7365 6c65 6374 6564  ubid_in_selected
-00000490: 5f73 7562 6964 da25 7570 6461 7465 5f64  _subid.%update_d
-000004a0: 6f77 6e73 7562 6964 735f 7573 696e 675f  ownsubids_using_
-000004b0: 7365 635f 646f 776e 7375 6269 64da 0f75  sec_downsubid..u
-000004c0: 7064 6174 655f 746f 706f 6c6f 6779 5a19  pdate_topologyZ.
-000004d0: 7365 635f 646f 776e 5f73 7562 696e 666f  sec_down_subinfo
-000004e0: 5f6d 6f73 7464 6f77 6e5a 2073 6563 5f64  _mostdownZ sec_d
-000004f0: 6f77 6e5f 7375 6269 645f 696e 5f73 656c  own_subid_in_sel
-00000500: 6563 7465 645f 7375 6269 645a 2473 6563  ected_subidZ$sec
-00000510: 5f64 6f77 6e5f 7375 6269 6e66 6f5f 646f  _down_subinfo_do
-00000520: 776e 7375 625f 696e 5f73 656c 6563 7465  wnsub_in_selecte
-00000530: 645a 1a6d 6973 7369 6e67 5f73 7562 6964  dZ.missing_subid
-00000540: 5f69 6e5f 7365 635f 7461 626c 655a 0d68  _in_sec_tableZ.h
-00000550: 7973 6864 696e 666f 5f73 6563 5a09 7375  yshdinfo_secZ.su
-00000560: 6269 645f 7365 635a 1175 7073 7472 6561  bid_secZ.upstrea
-00000570: 6d5f 7375 6273 5f73 6563 5a16 7365 635f  m_subs_secZ.sec_
-00000580: 646f 776e 5f73 7562 696e 666f 7365 6c65  down_subinfosele
-00000590: 6374 da04 6d61 736b 5a19 7570 7374 7265  ct..maskZ.upstre
-000005a0: 616d 5f73 7562 735f 6e65 775f 7375 625f  am_subs_new_sub_
-000005b0: 7365 63a9 0072 2400 0000 fa48 633a 5c75  sec..r$....Hc:\u
-000005c0: 7365 7273 5c6d 3433 6861 6e5f 325c 646f  sers\m43han_2\do
-000005d0: 6375 6d65 6e74 735c 6769 7468 7562 5c62  cuments\github\b
-000005e0: 6173 696e 6d61 6b65 725c 6261 7369 6e6d  asinmaker\basinm
-000005f0: 616b 6572 5c66 756e 635c 7064 7461 626c  aker\func\pdtabl
-00000600: 652e 7079 da29 7570 6461 7465 5f73 656c  e.py.)update_sel
-00000610: 6563 7465 645f 7375 6269 645f 7573 696e  ected_subid_usin
-00000620: 675f 7365 635f 646f 776e 7375 6269 640d  g_sec_downsubid.
-00000630: 0000 0073 3200 0000 0001 0401 0401 0401  ...s2...........
-00000640: 0402 1a01 1605 0802 0c01 0a07 1c02 0c01  ................
-00000650: 0a03 1401 0e02 0a01 1202 1001 0e01 1a02  ................
-00000660: 1401 0a02 1201 0e01 0401 7226 0000 0063  ..........r&...c
-00000670: 0400 0000 0000 0000 0000 0000 1000 0000  ................
-00000680: 0600 0000 4300 0000 733a 0100 0064 017d  ....C...s:...d.}
-00000690: 0464 017d 057c 0064 0264 0367 0219 00a0  .d.}.|.d.d.g....
-000006a0: 0064 04a1 016a 017d 0664 057d 0764 057d  .d...j.}.d.}.d.}
-000006b0: 0874 0264 0574 037c 0183 0183 0244 005d  .t.d.t.|.....D.]
-000006c0: 487d 097c 017c 0919 007d 0a74 047c 0a7c  H}.|.|...}.t.|.|
-000006d0: 067c 037c 0083 045c 037d 0b7d 007d 087c  .|.|...\.}.}.}.|
-000006e0: 077c 0817 007d 077c 0964 056b 0272 687c  .|...}.|.d.k.rh|
-000006f0: 0b7d 0c71 3274 056a 067c 0c7c 0b66 0264  .}.q2t.j.|.|.f.d
-00000700: 0564 068d 027d 0c71 3274 05a0 077c 0ca1  .d...}.q2t...|..
-00000710: 017d 0c74 056a 0864 0574 0964 078d 027d  .}.t.j.d.t.d...}
-00000720: 0d74 0264 0574 037c 0283 0183 0244 005d  .t.d.t.|.....D.]
-00000730: 4a7d 0e7c 027c 0e19 007d 0a7c 0a64 056b  J}.|.|...}.|.d.k
-00000740: 0072 b871 a274 047c 0a7c 067c 037c 0083  .r.q.t.|.|.|.|..
-00000750: 045c 037d 0b7d 007d 087c 0e64 056b 0272  .\.}.}.}.|.d.k.r
-00000760: da7c 0b7d 0d71 a274 056a 067c 0d7c 0b66  .|.}.q.t.j.|.|.f
-00000770: 0264 0564 068d 027d 0d71 a274 037c 0d83  .d.d...}.q.t.|..
-00000780: 0164 056b 0490 0172 1c74 05a0 077c 0da1  .d.k...r.t...|..
-00000790: 017d 0d74 05a0 0a7c 0c7c 0da1 020f 007d  .}.t...|.|.....}
-000007a0: 0f7c 0c7c 0f19 007d 0c7c 0764 086b 0590  .|.|...}.|.d.k..
-000007b0: 0172 2c64 097d 086e 0464 017d 087c 0c7c  .r,d.}.n.d.}.|.|
-000007c0: 007c 0866 0353 0029 0a4e 4672 0600 0000  .|.f.S.).NFr....
-000007d0: 720d 0000 0072 0900 0000 7201 0000 0072  r....r....r....r
-000007e0: 0e00 0000 2901 da05 6474 7970 65e9 0100  ....)...dtype...
-000007f0: 0000 5429 0b72 1600 0000 7213 0000 00da  ..T).r....r.....
-00000800: 0572 616e 6765 7215 0000 00da 1f72 6574  .ranger......ret
-00000810: 7572 6e5f 7375 6269 6473 5f64 7261 696e  urn_subids_drain
-00000820: 6167 655f 746f 5f73 7562 6964 721a 0000  age_to_subidr...
-00000830: 0072 1b00 0000 da06 756e 6971 7565 da05  .r......unique..
-00000840: 656d 7074 79da 0369 6e74 da04 696e 3164  empty..int..in1d
-00000850: 2910 721f 0000 00da 0a6d 6f73 7464 6f77  ).r......mostdow
-00000860: 6e69 64da 0e6d 6f73 7475 7073 7472 6561  nid..mostupstrea
-00000870: 6d69 6472 1d00 0000 5a0f 6861 735f 7365  midr....Z.has_se
-00000880: 635f 646f 776e 7375 6272 2100 0000 7220  c_downsubr!...r 
-00000890: 0000 005a 1373 756d 5f75 7064 6174 655f  ...Z.sum_update_
-000008a0: 746f 706f 6c6f 6779 7222 0000 005a 0669  topologyr"...Z.i
-000008b0: 5f64 6f77 6eda 0974 6172 5f73 7562 6964  _down..tar_subid
-000008c0: 721e 0000 005a 0d73 656c 6563 7465 645f  r....Z.selected_
-000008d0: 7375 6273 5a0b 7265 6d6f 7665 5f73 7562  subsZ.remove_sub
-000008e0: 735a 0469 5f75 7072 2300 0000 7224 0000  sZ.i_upr#...r$..
-000008f0: 0072 2400 0000 7225 0000 00da 1772 6574  .r$...r%.....ret
-00000900: 7572 6e5f 6578 7472 6163 7465 645f 7375  urn_extracted_su
-00000910: 6269 6473 3b00 0000 733c 0000 0000 0304  bids;...s<......
-00000920: 0104 0214 0104 0104 0212 0208 0214 0108  ................
-00000930: 0108 0106 0214 020a 030e 0212 0208 0208  ................
-00000940: 0102 0214 0208 0106 0214 020e 010a 020e  ................
-00000950: 0208 010a 0106 0204 0172 3200 0000 6304  .........r2...c.
-00000960: 0000 0000 0000 0000 0000 0006 0000 0005  ................
-00000970: 0000 0043 0000 0073 3800 0000 7400 7c01  ...C...s8...t.|.
-00000980: 7c00 8302 7d04 6401 7d05 7401 7c02 8301  |...}.d.}.t.|...
-00000990: 6401 6b04 722e 7402 7c02 7c04 7c03 7c01  d.k.r.t.|.|.|.|.
-000009a0: 8304 5c03 7d04 7d03 7d05 7c04 7c03 7c05  ..\.}.}.}.|.|.|.
-000009b0: 6603 5300 2902 4e72 0100 0000 2903 7217  f.S.).Nr....).r.
-000009c0: 0000 0072 1500 0000 7226 0000 0029 0672  ...r....r&...).r
-000009d0: 3100 0000 7220 0000 0072 1d00 0000 721f  1...r ...r....r.
-000009e0: 0000 0072 1e00 0000 7222 0000 0072 2400  ...r....r"...r$.
-000009f0: 0000 7224 0000 0072 2500 0000 722a 0000  ..r$...r%...r*..
-00000a00: 0073 0000 0073 0a00 0000 0003 0a01 0402  .s...s..........
-00000a10: 0c01 1402 722a 0000 0063 0400 0000 0000  ....r*...c......
-00000a20: 0000 0000 0000 0d00 0000 0500 0000 4300  ..............C.
-00000a30: 0000 7334 0100 007c 0064 016b 0172 0c7c  ..s4...|.d.k.r.|
-00000a40: 0153 007c 0164 027c 0364 0367 0319 006a  .S.|.d.|.d.g...j
-00000a50: 0064 0464 058d 017d 047c 046a 0164 0364  .d.d...}.|.j.d.d
-00000a60: 0669 0164 078d 017d 047c 046a 0264 027c  .i.d...}.|.j.d.|
-00000a70: 0367 0264 0864 098d 02a0 03a1 007d 0474  .g.d.d.......}.t
-00000a80: 046a 057c 047c 0264 0264 0a8d 037d 047c  .j.|.|.d.d...}.|
-00000a90: 0464 0619 007c 0464 0b19 001b 007c 0464  .d...|.d.....|.d
-00000aa0: 0c3c 007c 046a 0664 0264 0667 0264 0864  .<.|.j.d.d.g.d.d
-00000ab0: 0d8d 027d 047c 046a 0764 0267 0164 0e64  ...}.|.j.d.g.d.d
-00000ac0: 0f8d 026a 0064 0464 058d 017d 057c 047c  ...j.d.d...}.|.|
-00000ad0: 0464 0c19 007c 006b 0019 0064 027c 0367  .d...|.k...d.|.g
-00000ae0: 0219 006a 0064 0464 058d 017d 0674 0864  ...j.d.d...}.t.d
-00000af0: 0174 097c 0683 0183 0244 005d 6a7d 077c  .t.|.....D.]j}.|
-00000b00: 0664 0219 006a 0a7c 0719 007d 087c 067c  .d...j.|...}.|.|
-00000b10: 0319 006a 0a7c 0719 007d 097c 0164 0219  ...j.|...}.|.d..
-00000b20: 007c 086b 027d 0a7c 017c 0319 007c 096b  .|.k.}.|.|...|.k
-00000b30: 027d 0b74 0ba0 0c7c 0a7c 0ba1 027d 0c7c  .}.t...|.|...}.|
-00000b40: 056a 0d7c 0564 0219 007c 086b 0219 007c  .j.|.d...|.k...|
-00000b50: 0319 006a 0a64 0119 007c 016a 0d7c 0c7c  ...j.d...|.j.|.|
-00000b60: 0366 023c 0071 c47c 0153 0029 104e 7201  .f.<.q.|.S.).Nr.
-00000b70: 0000 0072 0600 0000 da08 4852 555f 4172  ...r......HRU_Ar
-00000b80: 6561 5472 0700 0000 5a09 496e 7075 745f  eaTr....Z.Input_
-00000b90: 415f 4772 1000 0000 46a9 01da 0861 735f  A_Gr....F....as_
-00000ba0: 696e 6465 7829 0172 0b00 0000 da07 4261  index).r......Ba
-00000bb0: 735f 415f 475a 0a41 7265 615f 7261 7469  s_A_GZ.Area_rati
-00000bc0: 6fa9 02da 0262 79da 0961 7363 656e 6469  o....by..ascendi
-00000bd0: 6e67 da05 6669 7273 7429 02da 0673 7562  ng..first)...sub
-00000be0: 7365 74da 046b 6565 7029 0e72 1400 0000  set..keep).r....
-00000bf0: da06 7265 6e61 6d65 da07 6772 6f75 7062  ..rename..groupb
-00000c00: 79da 0373 756d da02 7064 7218 0000 00da  y..sum..pdr.....
-00000c10: 0b73 6f72 745f 7661 6c75 6573 da0f 6472  .sort_values..dr
-00000c20: 6f70 5f64 7570 6c69 6361 7465 7372 2900  op_duplicatesr).
-00000c30: 0000 7215 0000 0072 1300 0000 721a 0000  ..r....r....r...
-00000c40: 00da 0b6c 6f67 6963 616c 5f61 6e64 7219  ...logical_andr.
-00000c50: 0000 0029 0dda 0d6c 616e 6475 7365 5f74  ...)...landuse_t
-00000c60: 6872 6573 da07 6872 7569 6e66 6fda 0873  hres..hruinfo..s
-00000c70: 7562 5f61 7265 61da 0a4c 616e 6475 7365  ub_area..Landuse
-00000c80: 5f49 445a 0a73 7562 696e 666f 5f6c 755a  _IDZ.subinfo_luZ
-00000c90: 1473 7562 696e 666f 5f6c 755f 646f 6d69  .subinfo_lu_domi
-00000ca0: 6e61 7465 645a 1673 7562 696e 666f 5f6c  natedZ.subinfo_l
-00000cb0: 755f 6e65 6564 5f63 6861 6e67 65da 0169  u_need_change..i
-00000cc0: da05 7375 6269 645a 076c 616e 6475 7365  ..subidZ.landuse
-00000cd0: da05 6d61 736b 31da 056d 6173 6b32 7223  ..mask1..mask2r#
-00000ce0: 0000 0072 2400 0000 7224 0000 0072 2500  ...r$...r$...r%.
-00000cf0: 0000 da27 7265 6d6f 7665 5f6c 616e 6475  ...'remove_landu
-00000d00: 7365 5f74 7970 655f 696e 7075 745f 6261  se_type_input_ba
-00000d10: 7365 645f 6f6e 5f61 7265 617e 0000 0073  sed_on_area~...s
-00000d20: 2400 0000 0002 0801 0402 1601 1001 1603  $...............
-00000d30: 1001 1403 1201 1803 2002 1201 0e01 0e01  ........ .......
-00000d40: 0c01 0c01 0c01 2802 724c 0000 0063 0700  ......(.rL...c..
-00000d50: 0000 0000 0000 0000 0000 0e00 0000 0600  ................
-00000d60: 0000 4300 0000 73c2 0000 007c 016a 007c  ..C...s....|.j.|
-00000d70: 0164 0119 0064 026b 0419 00a0 01a1 007d  .d...d.k.......}
-00000d80: 077c 016a 007c 0164 0119 0064 026b 0119  .|.j.|.d...d.k..
-00000d90: 00a0 01a1 007d 087c 0164 0364 0467 0219  .....}.|.d.d.g..
-00000da0: 006a 0164 0564 068d 017d 097c 096a 0264  .j.d.d...}.|.j.d
-00000db0: 0464 0769 0164 088d 017d 097c 096a 0364  .d.i.d...}.|.j.d
-00000dc0: 0367 0164 0964 0a8d 02a0 04a1 007d 097c  .g.d.d.......}.|
-00000dd0: 0064 0219 007d 0a7c 027c 037c 0567 037d  .d...}.|.|.|.g.}
-00000de0: 0b74 0564 0274 067c 0b83 0183 0244 005d  .t.d.t.|.....D.]
-00000df0: 227d 0c7c 0b7c 0c19 007d 0d7c 007c 0c19  "}.|.|...}.|.|..
-00000e00: 007d 0a74 077c 0a7c 087c 097c 0d83 047d  .}.t.|.|.|.|...}
-00000e10: 0871 847c 087c 0219 007c 087c 043c 007c  .q.|.|...|.|.<.|
-00000e20: 07a0 087c 08a1 017d 017c 0153 0029 0b4e  ...|...}.|.S.).N
-00000e30: da0a 4852 555f 4973 4c61 6b65 7201 0000  ..HRU_IsLaker...
-00000e40: 0072 0600 0000 7233 0000 0054 7207 0000  .r....r3...Tr...
-00000e50: 0072 3600 0000 7210 0000 0046 7234 0000  .r6...r....Fr4..
-00000e60: 0029 0972 1900 0000 7214 0000 0072 3d00  .).r....r....r=.
-00000e70: 0000 723e 0000 0072 3f00 0000 7229 0000  ..r>...r?...r)..
-00000e80: 0072 1500 0000 724c 0000 00da 0661 7070  .r....rL.....app
-00000e90: 656e 6429 0eda 1561 7265 615f 7261 7469  end)...area_rati
-00000ea0: 6f5f 7468 7265 7368 6f6c 6473 7245 0000  o_thresholdsrE..
-00000eb0: 0072 4700 0000 da07 536f 696c 5f49 44da  .rG.....Soil_ID.
-00000ec0: 0656 6567 5f49 44da 0e4f 7468 6572 5f50  .Veg_ID..Other_P
-00000ed0: 6c79 5f49 445f 31da 0e4f 7468 6572 5f50  ly_ID_1..Other_P
-00000ee0: 6c79 5f49 445f 325a 0d68 7275 5f6c 616b  ly_ID_2Z.hru_lak
-00000ef0: 655f 696e 666f 5a0d 6872 755f 6c61 6e64  e_infoZ.hru_land
-00000f00: 5f69 6e66 6f72 4600 0000 7244 0000 00da  _inforF...rD....
-00000f10: 046c 6973 7472 4800 0000 da04 4974 656d  .listrH.....Item
-00000f20: 7224 0000 0072 2400 0000 7225 0000 00da  r$...r$...r%....
-00000f30: 1573 696d 706c 6966 795f 6872 7573 5f6d  .simplify_hrus_m
-00000f40: 6574 686f 6432 9c00 0000 731c 0000 0000  ethod2....s.....
-00000f50: 0316 0116 0214 0110 0114 0308 010a 0112  ................
-00000f60: 0108 0108 0110 010c 020a 0272 5600 0000  ...........rV...
-00000f70: 6303 0000 0000 0000 0000 0000 001d 0000  c...............
-00000f80: 0009 0000 0043 0000 0073 8e02 0000 7c01  .....C...s....|.
-00000f90: 6401 1900 7c01 6402 3c00 7400 a001 7c01  d...|.d.<.t...|.
-00000fa0: 6403 1900 6a02 a101 7d03 7403 6404 7404  d...j...}.t.d.t.
-00000fb0: 7c03 8301 8302 4400 9002 5d4e 7d04 7c03  |.....D...]N}.|.
-00000fc0: 7c04 1900 7d05 7c01 6a05 7c01 6403 1900  |...}.|.j.|.d...
-00000fd0: 7c05 6b02 1900 6a06 6405 6406 8d01 7d06  |.k...j.d.d...}.
-00000fe0: 7400 a007 7c06 6407 1900 6a02 a101 7d07  t...|.d...j...}.
-00000ff0: 7c00 7c07 1400 7d08 7c06 6a05 7c06 6407  |.|...}.|.j.|.d.
-00001000: 1900 7c08 6b00 1900 a006 a100 7d09 7c06  ..|.k.......}.|.
-00001010: 6a05 7c06 6407 1900 7c08 6b05 1900 a006  j.|.d...|.k.....
-00001020: a100 7d0a 7c0a 6a08 7d0b 7c0b 7c0b 6402  ..}.|.j.}.|.|.d.
-00001030: 6b03 1900 7d0b 7c02 6404 1900 7d0c 7c09  k...}.|.d...}.|.
-00001040: 6a06 6405 6406 8d01 7d0d 7400 a001 7c0d  j.d.d...}.t...|.
-00001050: 7c0c 1900 6a02 a101 7d0e 7403 6404 7404  |...j...}.t.d.t.
-00001060: 7c0e 8301 8302 4400 5dbc 7d0f 7c0e 7c0f  |.....D.].}.|.|.
-00001070: 1900 7d10 7c0d 6a05 7c0d 7c0c 1900 7c10  ..}.|.j.|.|...|.
-00001080: 6b02 1900 6a06 6405 6406 8d01 7d11 7400  k...j.d.d...}.t.
-00001090: a007 7c11 6407 1900 6a02 a101 7d12 7c12  ..|.d...j...}.|.
-000010a0: 7c08 6b05 72da 7c11 6a09 6407 6701 6408  |.k.r.|.j.d.g.d.
-000010b0: 6409 8d02 7d11 7403 6404 7404 7c0b 8301  d...}.t.d.t.|...
-000010c0: 8302 4400 5d44 7d13 7c0b 7c13 1900 7d14  ..D.]D}.|.|...}.
-000010d0: 7c14 640a 6b02 9001 7250 9001 7136 7c11  |.d.k...rP..q6|.
-000010e0: 7c14 1900 6a02 6404 1900 7c01 6a05 7c01  |...j.d...|.j.|.
-000010f0: 6402 1900 a00a 7c11 6402 1900 6a02 a101  d.....|.d...j...
-00001100: 7c14 6602 3c00 9001 7136 7c09 7c09 6402  |.f.<...q6|.|.d.
-00001110: 1900 a00a 7c11 6402 1900 6a02 a101 0f00  ....|.d...j.....
-00001120: 1900 7d09 71da 7c09 6a0b 7d15 7403 6404  ..}.q.|.j.}.t.d.
-00001130: 7404 7c15 8301 8302 4400 5dcc 7d16 7c15  t.|.....D.].}.|.
-00001140: 7c16 1900 7d17 7c09 6a05 7c17 6402 6602  |...}.|.j.|.d.f.
-00001150: 1900 7d18 7403 6404 7404 7c02 8301 8302  ..}.t.d.t.|.....
-00001160: 4400 5da0 7d19 7c02 7c19 1900 7d1a 7c09  D.].}.|.|...}.|.
-00001170: 6a05 7c17 7c1a 6602 1900 7d1b 7c0a 6a05  j.|.|.f...}.|.j.
-00001180: 7c0a 7c1a 1900 7c1b 6b02 1900 a006 a100  |.|...|.k.......
-00001190: 7d1c 7404 7c1c 8301 6404 6b04 9001 72d4  }.t.|...d.k...r.
-000011a0: 7c1c 6a09 6407 6408 6409 8d02 7d1c 7403  |.j.d.d.d...}.t.
-000011b0: 6404 7404 7c0b 8301 8302 4400 5d3c 7d13  d.t.|.....D.]<}.
-000011c0: 7c0b 7c13 1900 7d14 7c14 640a 6b02 9002  |.|...}.|.d.k...
-000011d0: 7248 9002 712e 7c1c 7c14 1900 6a02 6404  rH..q.|.|...j.d.
-000011e0: 1900 7c01 6a05 7c01 6402 1900 7c18 6b02  ..|.j.|.d...|.k.
-000011f0: 7c14 6602 3c00 9002 712e 6e04 9001 71d4  |.f.<...q.n...q.
-00001200: 9001 71d4 9001 71ac 712a 7c01 6a0c 6402  ..q...q.q*|.j.d.
-00001210: 6701 640b 8d01 7d01 7c01 5300 290c 4eda  g.d...}.|.S.).N.
-00001220: 0a48 5255 5f49 445f 4e65 775a 0b48 5255  .HRU_ID_NewZ.HRU
-00001230: 5f49 445f 4e65 7732 7206 0000 0072 0100  _ID_New2r....r..
-00001240: 0000 5472 0700 0000 7233 0000 0046 7237  ..Tr....r3...Fr7
-00001250: 0000 00da 0553 4841 5045 7210 0000 0029  .....SHAPEr....)
-00001260: 0d72 1a00 0000 722b 0000 0072 1300 0000  .r....r+...r....
-00001270: 7229 0000 0072 1500 0000 7219 0000 0072  r)...r....r....r
-00001280: 1400 0000 723f 0000 0072 1100 0000 7241  ....r?...r....rA
-00001290: 0000 0072 1200 0000 da05 696e 6465 7872  ...r......indexr
-000012a0: 1c00 0000 291d da14 6d69 6e5f 6872 755f  ....)...min_hru_
-000012b0: 7063 745f 7375 625f 6172 6561 7245 0000  pct_sub_arearE..
-000012c0: 00da 1069 6d70 6f72 7461 6e63 655f 6f72  ...importance_or
-000012d0: 6465 72da 0673 7562 6964 7372 4800 0000  der..subidsrH...
-000012e0: 7249 0000 005a 0c73 7562 5f68 7275 5f69  rI...Z.sub_hru_i
-000012f0: 6e66 6f5a 0873 7562 6173 7265 615a 0c73  nfoZ.subasreaZ.s
-00001300: 7562 6172 6561 5f74 6872 735a 106e 6565  ubarea_thrsZ.nee
-00001310: 645f 7265 6d6f 7665 5f68 7275 735a 0967  d_remove_hrusZ.g
-00001320: 6f6f 645f 6872 7573 5a0b 6872 755f 636f  ood_hrusZ.hru_co
-00001330: 6c75 6d6e 735a 0663 6f6c 6e6d 315a 1c69  lumnsZ.colnm1Z.i
-00001340: 6d70 6f72 7431 5f41 7265 615f 6e65 6564  mport1_Area_need
-00001350: 5f72 656d 6f76 655f 6872 755a 0e75 6e69  _remove_hruZ.uni
-00001360: 7175 655f 696d 706f 7274 315a 0869 5f69  que_import1Z.i_i
-00001370: 6d70 6f72 745a 0869 5f63 6f6c 6e6d 315a  mportZ.i_colnm1Z
-00001380: 1e69 5f69 6d70 6f72 7431 5f41 7265 615f  .i_import1_Area_
-00001390: 6e65 6564 5f72 656d 6f76 655f 6872 755a  need_remove_hruZ
-000013a0: 2774 6f74 616c 5f61 7265 615f 695f 696d  'total_area_i_im
-000013b0: 706f 7274 5f69 6e5f 6e65 6564 5f72 656d  port_in_need_rem
-000013c0: 6f76 655f 6872 7573 5a04 695f 6e6d 5a0a  ove_hrusZ.i_nmZ.
-000013d0: 636f 6c75 6d6e 6e61 6d65 da07 696e 6465  columnname..inde
-000013e0: 7865 73da 016a da03 6964 78da 0568 7275  xes..j..idx..hru
-000013f0: 6964 da01 6b5a 0563 6f6c 6e6d 5a10 6174  id..kZ.colnmZ.at
-00001400: 7472 695f 7265 6d6f 7665 5f68 7275 5a0b  tri_remove_hruZ.
-00001410: 676f 6f64 5f68 7275 735f 6b72 2400 0000  good_hrus_kr$...
-00001420: 7224 0000 0072 2500 0000 da0e 7369 6d70  r$...r%.....simp
-00001430: 6c69 6466 795f 6872 7573 b500 0000 7358  lidfy_hrus....sX
-00001440: 0000 0000 020c 0210 0314 0108 021a 0210  ................
-00001450: 0108 0316 0216 0206 020c 0308 010c 0110  ................
-00001460: 0512 0108 011a 0110 0508 0310 0112 0108  ................
-00001470: 010a 0104 022c 031c 0206 0412 0108 010e  .....,..........
-00001480: 0412 0108 020e 0316 020e 020e 0112 0108  ................
-00001490: 010a 0104 0226 020e 010e 0172 6200 0000  .....&.....rb...
-000014a0: 6301 0000 0000 0000 0000 0000 000b 0000  c...............
-000014b0: 0005 0000 0043 0000 0073 ba02 0000 7c00  .....C...s....|.
-000014c0: 6401 6402 6702 1900 a000 6403 a101 6a01  d.d.g.....d...j.
-000014d0: 7d01 7c00 6a02 7c00 6404 1900 6405 6b02  }.|.j.|.d...d.k.
-000014e0: 1900 a003 a100 7d02 7c02 6401 1900 a003  ......}.|.d.....
-000014f0: a100 7d03 7c00 6406 1900 a004 a100 7d04  ..}.|.d.......}.
-00001500: 6407 7c00 6a02 7c00 6401 1900 a005 7c03  d.|.j.|.d.....|.
-00001510: a101 6408 6602 3c00 7406 6409 7407 7c02  ..d.f.<.t.d.t.|.
-00001520: 8301 8302 4400 9002 5d4a 7d05 7c02 6401  ....D...]J}.|.d.
-00001530: 1900 6a01 7c05 1900 7d06 7c02 6402 1900  ..j.|...}.|.d...
-00001540: 6a01 7c05 1900 7d07 7c00 6a02 7c00 6401  j.|...}.|.j.|.d.
-00001550: 1900 7c07 6b02 1900 a003 a100 7d08 7c07  ..|.k.......}.|.
-00001560: 7d09 7407 7c08 8301 640a 6b00 72fc 640a  }.t.|...d.k.r.d.
-00001570: 7c00 6a02 7c00 6401 1900 7c06 6b02 640b  |.j.|.d...|.k.d.
-00001580: 6602 3c00 7c04 7c05 1700 640a 1700 7c00  f.<.|.|...d...|.
-00001590: 6a02 7c00 6401 1900 7c06 6b02 6406 6602  j.|.d...|.k.d.f.
-000015a0: 3c00 640a 7c00 6a02 7c00 6401 1900 7c06  <.d.|.j.|.d...|.
-000015b0: 6b02 640c 6602 3c00 7168 7c08 6404 1900  k.d.f.<.qh|.d...
-000015c0: 6a01 6409 1900 6405 6b02 9001 728c 7c00  j.d...d.k...r.|.
-000015d0: 6a02 7c00 6401 1900 7c09 6b02 1900 a003  j.|.d...|.k.....
-000015e0: a100 7d0a 7c0a 6402 1900 6a01 6409 1900  ..}.|.d...j.d...
-000015f0: 7d07 7c00 6a02 7c00 6401 1900 7c07 6b02  }.|.j.|.d...|.k.
-00001600: 1900 a003 a100 7d08 7407 7c08 8301 640a  ......}.t.|...d.
-00001610: 6b00 9001 7260 640d 7d09 9001 718c 7c09  k...r`d.}...q.|.
-00001620: 7c08 6402 1900 6a01 6409 1900 6b02 9001  |.d...j.d...k...
-00001630: 7286 7408 7c09 7c07 8302 0100 640d 7d09  r.t.|.|.....d.}.
-00001640: 9001 718c 7c07 7d09 71fc 7c09 640d 6b02  ..q.|.}.q.|.d.k.
-00001650: 9001 7298 7168 640e 7c00 6a02 7c00 6401  ..r.qhd.|.j.|.d.
-00001660: 1900 7c06 6b02 640f 6602 3c00 640e 7c00  ..|.k.d.f.<.d.|.
-00001670: 6a02 7c00 6401 1900 7c06 6b02 6410 6602  j.|.d...|.k.d.f.
-00001680: 3c00 640e 7c00 6a02 7c00 6401 1900 7c06  <.d.|.j.|.d...|.
-00001690: 6b02 6408 6602 3c00 640e 7c00 6a02 7c00  k.d.f.<.d.|.j.|.
-000016a0: 6401 1900 7c06 6b02 6411 6602 3c00 640e  d...|.k.d.f.<.d.
-000016b0: 7c00 6a02 7c00 6401 1900 7c06 6b02 6412  |.j.|.d...|.k.d.
-000016c0: 6602 3c00 640e 7c00 6a02 7c00 6401 1900  f.<.d.|.j.|.d...
-000016d0: 7c06 6b02 6413 6602 3c00 6414 7c00 6a09  |.k.d.f.<.d.|.j.
-000016e0: 7600 9002 7254 640e 7c00 6a02 7c00 6401  v...rTd.|.j.|.d.
-000016f0: 1900 7c06 6b02 6414 6602 3c00 640e 7c00  ..|.k.d.f.<.d.|.
-00001700: 6a02 7c00 6401 1900 7c06 6b02 6415 6602  j.|.d...|.k.d.f.
-00001710: 3c00 7c08 640b 1900 6a01 6409 1900 7c00  <.|.d...j.d...|.
-00001720: 6a02 7c00 6401 1900 7c06 6b02 640b 6602  j.|.d...|.k.d.f.
-00001730: 3c00 7c08 6406 1900 6a01 6409 1900 7c00  <.|.d...j.d...|.
-00001740: 6a02 7c00 6401 1900 7c06 6b02 6406 6602  j.|.d...|.k.d.f.
-00001750: 3c00 7c08 640c 1900 6a01 6409 1900 7c00  <.|.d...j.d...|.
-00001760: 6a02 7c00 6401 1900 7c06 6b02 640c 6602  j.|.d...|.k.d.f.
-00001770: 3c00 7168 7c00 5300 2916 4e72 0600 0000  <.qh|.S.).Nr....
-00001780: 720d 0000 00da 0566 6c6f 6174 da08 4c61  r......float..La
-00001790: 6b65 5f43 6174 e902 0000 00da 0653 6567  ke_Cat.......Seg
-000017a0: 5f49 44e7 0000 0000 0000 0000 da09 5269  _ID...........Ri
-000017b0: 764c 656e 6774 6872 0100 0000 7228 0000  vLengthr....r(..
-000017c0: 00da 0853 7472 6168 6c65 72da 0953 6567  ...Strahler..Seg
-000017d0: 5f6f 7264 6572 e9ff ffff ffe7 8d97 6e12  _order........n.
-000017e0: 83c0 f3bf da08 5269 7653 6c6f 7065 da04  ......RivSlope..
-000017f0: 4368 5f6e da07 4d69 6e5f 4445 4dda 074d  Ch_n..Min_DEM..M
-00001800: 6178 5f44 454d da08 466c 6f6f 6450 5f6e  ax_DEM..FloodP_n
-00001810: da08 4441 5f43 686e 5f4c da0a 4441 5f43  ..DA_Chn_L..DA_C
-00001820: 686e 5f53 6c70 290a 7216 0000 0072 1300  hn_Slp).r....r..
-00001830: 0000 7219 0000 0072 1400 0000 da03 6d61  ..r....r......ma
-00001840: 7872 1200 0000 7229 0000 0072 1500 0000  xr....r)...r....
-00001850: da05 7072 696e 7472 1100 0000 290b da07  ..printr....)...
-00001860: 6361 7469 6e66 6fda 0c72 6f75 7469 6e67  catinfo..routing
-00001870: 5f69 6e66 6f5a 1563 6174 696e 666f 5f6e  _infoZ.catinfo_n
-00001880: 6f6e 5f63 6f6e 6e65 6374 6564 5a09 6361  on_connectedZ.ca
-00001890: 7469 6473 5f6e 635a 0a6d 6178 5f73 6567  tids_ncZ.max_seg
-000018a0: 5f69 6472 4800 0000 5a07 635f 7375 6269  _idrH...Z.c_subi
-000018b0: 645a 0764 5f73 7562 6964 5a0a 645f 7375  dZ.d_subidZ.d_su
-000018c0: 625f 696e 666f 5a08 6c63 5f73 7562 6964  b_infoZ.lc_subid
-000018d0: 5a0d 6c63 5f73 7562 6964 5f69 6e66 6f72  Z.lc_subid_infor
-000018e0: 2400 0000 7224 0000 0072 2500 0000 da23  $...r$...r%....#
-000018f0: 7570 6461 7465 5f6e 6f6e 5f63 6f6e 6e65  update_non_conne
-00001900: 6374 6564 5f63 6174 6368 6d65 6e74 5f69  cted_catchment_i
-00001910: 6e66 6f0c 0100 0073 7200 0000 0001 1401  nfo....sr.......
-00001920: 1602 0c01 0c03 02fe 0401 10ff 0204 1401  ................
-00001930: 0e01 0e01 1602 040a 0c01 1601 1e01 1601  ................
-00001940: 0206 1401 1601 0e01 1601 0e01 0401 0401  ................
-00001950: 1401 0a01 0401 0401 0602 0a01 0202 1601  ................
-00001960: 1601 1601 1601 1601 1601 0c01 1601 160c  ................
-00001970: 0201 02ff 0402 02fe 1603 0201 02ff 0402  ................
-00001980: 02fe 1603 0201 02ff 0402 02fe 1804 7278  ..............rx
-00001990: 0000 0063 0100 0000 0000 0000 0000 0000  ...c............
-000019a0: 1000 0000 0600 0000 4300 0000 73be 0100  ........C...s...
-000019b0: 007c 006a 0064 0167 0164 0264 038d 027d  .|.j.d.g.d.d...}
-000019c0: 0174 01a0 0264 0464 05a1 027d 0264 067d  .t...d.d...}.d.}
-000019d0: 0374 01a0 0264 0764 08a1 027d 047c 0164  .t...d.d...}.|.d
-000019e0: 0919 006a 0364 0519 007d 0564 067d 067c  ...j.d...}.d.}.|
-000019f0: 057c 047c 0364 0618 003c 0074 047c 047c  .|.|.d...<.t.|.|
-00001a00: 0464 056b 0419 0083 0164 056b 0490 0172  .d.k.....d.k...r
-00001a10: b274 01a0 0264 0764 08a1 027d 077c 067d  .t...d.d...}.|.}
-00001a20: 0374 0564 057c 0683 0244 0090 015d 2a7d  .t.d.|...D...]*}
-00001a30: 087c 047c 0819 007d 097c 0964 056b 0072  .|.|...}.|.d.k.r
-00001a40: 9271 7a7c 016a 067c 0164 0919 007c 096b  .qz|.j.|.d...|.k
-00001a50: 0264 0a66 0219 007c 027c 0819 0017 007c  .d.f...|.|.....|
-00001a60: 027c 083c 007c 016a 067c 0164 0919 007c  .|.<.|.j.|.d...|
-00001a70: 096b 0264 0b66 0219 006a 0364 0519 007d  .k.d.f...j.d...}
-00001a80: 0a7c 016a 067c 0164 0c19 007c 096b 0219  .|.j.|.d...|.k..
-00001a90: 007d 0b74 047c 0b83 0164 056b 0172 f071  .}.t.|...d.k.r.q
-00001aa0: 7a7c 0b6a 067c 0b64 0b19 007c 0a6b 0219  z|.j.|.d...|.k..
-00001ab0: 007d 0c74 047c 0c83 0164 056b 0490 0172  .}.t.|...d.k...r
-00001ac0: 267c 0c64 0919 006a 0364 0519 007c 077c  &|.d...j.d...|.|
-00001ad0: 083c 0071 7a71 7a7c 0b6a 067c 0b64 0b19  .<.qzqz|.j.|.d..
-00001ae0: 007c 0a64 0618 006b 0219 007d 0d74 0564  .|.d...k...}.t.d
-00001af0: 0574 047c 0d83 0183 0244 005d 5a7d 0e7c  .t.|.....D.]Z}.|
-00001b00: 0e64 056b 0290 0172 6c7c 0d64 0919 006a  .d.k...rl|.d...j
-00001b10: 037c 0e19 007c 077c 083c 006e 367c 0d64  .|...|.|.<.n6|.d
-00001b20: 0919 006a 037c 0e19 007c 077c 0364 0617  ...j.|...|.|.d..
-00001b30: 0064 0618 003c 007c 027c 0819 007c 027c  .d...<.|.|...|.|
-00001b40: 0364 0617 0064 0618 003c 007c 0364 0617  .d...d...<.|.d..
-00001b50: 007d 0390 0171 4a71 7a7c 077d 047c 037d  .}...qJqz|.}.|.}
-00001b60: 0671 4a74 077c 0283 017d 0f7c 0f53 0029  .qJt.|...}.|.S.)
-00001b70: 0d4e da09 4472 6169 6e41 7265 6146 a901  .N..DrainAreaF..
-00001b80: 7239 0000 00e9 6400 0000 7201 0000 0072  r9....d...r....r
-00001b90: 2800 0000 e9e8 0300 0072 6b00 0000 7206  (........rk...r.
-00001ba0: 0000 0072 6800 0000 7269 0000 0072 0d00  ...rh...ri...r..
-00001bb0: 0000 2908 7241 0000 0072 1a00 0000 da04  ..).rA...r......
-00001bc0: 6675 6c6c 7213 0000 0072 1500 0000 7229  fullr....r....r)
-00001bd0: 0000 0072 1900 0000 7274 0000 0029 10da  ...r....rt...)..
-00001be0: 116d 6169 6e72 6976 5f6d 6572 675f 696e  .mainriv_merg_in
-00001bf0: 666f 5a16 6d61 696e 7269 765f 6d65 7267  foZ.mainriv_merg
-00001c00: 5f69 6e66 6f5f 736f 7274 5a13 6c6f 6e67  _info_sortZ.long
-00001c10: 6573 745f 666c 6f77 5f70 6174 6865 735a  est_flow_pathesZ
-00001c20: 056e 7061 7468 5a06 5061 7468 6964 7249  .npathZ.PathidrI
-00001c30: 0000 005a 0d6e 7061 7468 5f63 7572 7265  ...Z.npath_curre
-00001c40: 6e74 5a07 6e50 6174 6869 645a 0569 7061  ntZ.nPathidZ.ipa
-00001c50: 7468 5a0d 635f 7375 6269 645f 6970 6174  thZ.c_subid_ipat
-00001c60: 685a 1453 7472 6168 6c65 725f 6f72 6465  hZ.Strahler_orde
-00001c70: 725f 6970 6174 685a 1275 7073 7472 6561  r_ipathZ.upstrea
-00001c80: 6d5f 7375 625f 696e 666f 735a 1e75 7073  m_sub_infosZ.ups
-00001c90: 7472 6561 6d5f 7375 625f 696e 666f 735f  tream_sub_infos_
-00001ca0: 6571 5f53 7472 6168 6c65 725a 2075 7073  eq_StrahlerZ ups
-00001cb0: 7472 6561 6d5f 7375 625f 696e 666f 735f  tream_sub_infos_
-00001cc0: 6571 5f53 7472 6168 6c65 725f 315a 0669  eq_Strahler_1Z.i
-00001cd0: 6e70 6174 685a 0b4c 6f6e 6765 7374 7061  npathZ.Longestpa
-00001ce0: 7468 7224 0000 0072 2400 0000 7225 0000  thr$...r$...r%..
-00001cf0: 00da 1a43 616c 6375 6c61 7465 5f4c 6f6e  ...Calculate_Lon
-00001d00: 6765 7374 5f66 6c6f 7770 6174 6860 0100  gest_flowpath`..
-00001d10: 0073 7c00 0000 0001 1002 0c02 0403 0c01  .s|.............
-00001d20: 0e01 0401 0c02 1601 0c01 0405 1001 0803  ................
-00001d30: 06ff 0203 0203 0401 0eff 0203 06fd 02ff  ................
-00001d40: 0606 0401 0eff 0402 02fe 0404 0401 0aff  ................
-00001d50: 0405 0aff 0204 0205 0401 0aff 0405 0aff  ................
-00001d60: 0403 0801 02ff 0803 0402 0401 0eff 0404  ................
-00001d70: 1202 0a01 0201 02ff 0402 02fe 0a05 0201  ................
-00001d80: 02ff 0402 02fe 1003 1402 0e02 0401 0601  ................
-00001d90: 0802 727f 0000 0072 2800 0000 6302 0000  ..r....r(...c...
-00001da0: 0000 0000 0000 0000 0021 0000 0008 0000  .........!......
-00001db0: 0043 0000 0073 5805 0000 7c00 6a00 6401  .C...sX...|.j.d.
-00001dc0: 6402 8d01 7d02 6403 7d03 6403 7c00 6a01  d...}.d.}.d.|.j.
-00001dd0: 7601 721e 6404 7d03 7c00 7c00 6405 1900  v.r.d.}.|.|.d...
-00001de0: 6406 1b00 6406 1b00 7c01 6b00 1900 6a00  d...d...|.k...j.
-00001df0: 6401 6402 8d01 7d04 7c04 7c04 6407 1900  d.d...}.|.|.d...
-00001e00: 6408 6b02 1900 6a00 6401 6402 8d01 7d04  d.k...j.d.d...}.
-00001e10: 7c04 7c04 7c03 1900 6408 6b02 1900 6a00  |.|.|...d.k...j.
-00001e20: 6401 6402 8d01 7d04 7c04 6409 1900 6a02  d.d...}.|.d...j.
-00001e30: 7d05 7403 6408 7404 7c04 8301 8302 4400  }.t.d.t.|.....D.
-00001e40: 9004 5dca 7d06 7c04 6409 1900 6a02 7c06  ..].}.|.d...j.|.
-00001e50: 1900 7d07 7c04 640a 1900 6a02 7c06 1900  ..}.|.d...j.|...
-00001e60: 7d08 7c04 640b 1900 6a02 7c06 1900 7d09  }.|.d...j.|...}.
-00001e70: 7404 7c00 7c00 640a 1900 7c07 6b02 1900  t.|.|.d...|.k...
-00001e80: 8301 6408 6b02 7d0a 7c04 6407 1900 6a02  ..d.k.}.|.d...j.
-00001e90: 7c06 1900 6408 6b02 7d0b 7c04 7c03 1900  |...d.k.}.|.|...
-00001ea0: 6a02 7c06 1900 6408 6b01 7d0c 7c00 7c00  j.|...d.k.}.|.|.
-00001eb0: 6409 1900 7c08 6b02 1900 6a00 6401 6402  d...|.k...j.d.d.
-00001ec0: 8d01 7d0d 7c00 7c00 640a 1900 7c07 6b02  ..}.|.|.d...|.k.
-00001ed0: 1900 6a00 6401 6402 8d01 7d0e 7c0e 7c0e  ..j.d.d...}.|.|.
-00001ee0: 640b 1900 7c09 6b02 1900 6a00 6401 6402  d...|.k...j.d.d.
-00001ef0: 8d01 7d0f 7404 7c0d 8301 6408 6b04 9001  ..}.t.|...d.k...
-00001f00: 726c 6401 7d10 7c0d 640b 1900 6a02 6408  rld.}.|.d...j.d.
-00001f10: 1900 7c09 6b02 9001 7266 6401 7d11 6e04  ..|.k...rfd.}.n.
-00001f20: 640c 7d11 6e08 640c 7d10 640c 7d11 7404  d.}.n.d.}.d.}.t.
-00001f30: 7c0e 8301 6408 6b04 9001 72b4 6401 7d12  |...d.k...r.d.}.
-00001f40: 7404 7c0f 8301 6408 6b04 9001 72ae 7c0f  t.|...d.k...r.|.
-00001f50: 7c03 1900 6a02 6408 1900 6408 6b02 9001  |...j.d...d.k...
-00001f60: 72ae 6401 7d13 6e04 640c 7d13 6e08 640c  r.d.}.n.d.}.n.d.
-00001f70: 7d12 640c 7d13 7c10 9002 722c 7c11 9002  }.d.}.|...r,|...
-00001f80: 722c 7c0b 9002 722c 7c0c 9002 722c 7c02  r,|...r,|...r,|.
-00001f90: 7c02 6409 1900 7c0d 6409 1900 6a02 6408  |.d...|.d...j.d.
-00001fa0: 1900 6b02 1900 6a00 6401 6402 8d01 7d14  ..k...j.d.d...}.
-00001fb0: 6401 7d15 7c02 7c02 6409 1900 7c0d 6409  d.}.|.|.d...|.d.
-00001fc0: 1900 6a02 6408 1900 6b02 1900 6a00 6401  ..j.d...k...j.d.
-00001fd0: 6402 8d01 7d16 7c16 640a 1900 6a02 6408  d...}.|.d...j.d.
-00001fe0: 1900 7d17 6ede 7c12 9002 7292 7c13 9002  ..}.n.|...r.|...
-00001ff0: 7292 7c0b 9002 7292 7c0c 9002 7292 7c02  r.|...r.|...r.|.
-00002000: 7c02 6409 1900 7c0f 6409 1900 6a02 6408  |.d...|.d...j.d.
-00002010: 1900 6b02 1900 6a00 6401 6402 8d01 7d14  ..k...j.d.d...}.
-00002020: 6401 7d15 7c02 7c02 6409 1900 7c07 6b02  d.}.|.|.d...|.k.
-00002030: 1900 6a00 6401 6402 8d01 7d18 7c18 640a  ..j.d.d...}.|.d.
-00002040: 1900 6a02 6408 1900 7d17 6e78 7404 7c00  ..j.d...}.nxt.|.
-00002050: 7c00 640b 1900 7c09 6b02 1900 8301 640d  |.d...|.k.....d.
-00002060: 6b02 9003 7200 7c10 9003 7200 7c02 7c02  k...r.|...r.|.|.
-00002070: 6409 1900 7c0d 6409 1900 6a02 6408 1900  d...|.d...j.d...
-00002080: 6b02 1900 6a00 6401 6402 8d01 7d14 6401  k...j.d.d...}.d.
-00002090: 7d15 7c02 7c02 6409 1900 7c08 6b02 1900  }.|.|.d...|.k...
-000020a0: 6a00 6401 6402 8d01 7d16 7c16 640a 1900  j.d.d...}.|.d...
-000020b0: 6a02 6408 1900 7d17 6e0a 640c 7d15 6700  j.d...}.n.d.}.g.
-000020c0: 7d14 7186 7c15 7286 7404 7c00 7c00 640a  }.q.|.r.t.|.|.d.
-000020d0: 1900 7c14 6409 1900 6a02 6408 1900 6b02  ..|.d...j.d...k.
-000020e0: 1900 8301 6408 6b02 7d19 7404 7c00 7c00  ....d.k.}.t.|.|.
-000020f0: 640a 1900 7c14 6409 1900 6a02 6408 1900  d...|.d...j.d...
-00002100: 6b02 7c00 6407 1900 640e 6b00 4000 1900  k.|.d...d.k.@...
-00002110: 8301 640d 6b01 7d1a 7c02 6409 1900 7c07  ..d.k.}.|.d...|.
-00002120: 6b02 7d1b 7c02 640f 1900 7c07 6b02 7d1c  k.}.|.d...|.k.}.
-00002130: 7c02 640f 1900 7c14 640f 1900 6a02 6408  |.d...|.d...j.d.
-00002140: 1900 6b02 7d1d 7405 a006 7c1b 7c1d a102  ..k.}.t...|.|...
-00002150: 7d1e 7405 a006 7c1e 7c1c a102 7d1f 7404  }.t...|.|...}.t.
-00002160: 7c14 8301 640d 6b04 9003 72e6 7404 7405  |...d.k...r.t.t.
-00002170: a007 7c14 6410 1900 6a02 a101 8301 640d  ..|.d...j.....d.
-00002180: 6b04 9003 72e6 7408 7c07 7c09 8302 0100  k...r.t.|.|.....
-00002190: 7408 7c14 6700 6411 a201 1900 8301 0100  t.|.g.d.........
-000021a0: 7c14 6a01 4400 5ddc 7d20 7c20 6405 6b02  |.j.D.].} | d.k.
-000021b0: 9004 722e 7405 a009 7c14 6405 1900 6a02  ..r.t...|.d...j.
-000021c0: 6408 1900 7c02 6a0a 7c1b 6405 6602 1900  d...|.j.|.d.f...
-000021d0: 6a02 6408 1900 1700 a101 7c02 6a0a 7c1f  j.d.......|.j.|.
-000021e0: 7c20 6602 3c00 6e98 7c20 6409 6b02 9004  | f.<.n.| d.k...
-000021f0: 7252 7c14 640f 1900 6a02 6408 1900 7c02  rR|.d...j.d...|.
-00002200: 6a0a 7c1f 640f 6602 3c00 6e74 7c20 640a  j.|.d.f.<.nt| d.
-00002210: 6b02 9004 726c 7c17 7c02 6a0a 7c1f 7c20  k...rl|.|.j.|.| 
-00002220: 6602 3c00 6e5a 7c20 640f 6b02 9003 73ec  f.<.nZ| d.k...s.
-00002230: 7c20 6412 6b02 9003 73ec 7c20 6413 6b02  | d.k...s.| d.k.
-00002240: 9003 73ec 7c20 6414 6b02 9003 73ec 7c20  ..s.| d.k...s.| 
-00002250: 6415 6b02 9003 73ec 7c20 6416 6b02 9004  d.k...s.| d.k...
-00002260: 72ae 9003 71ec 6e18 7c14 7c20 1900 6a02  r...q.n.|.| ..j.
-00002270: 6408 1900 7c02 6a0a 7c1f 7c20 6602 3c00  d...|.j.|.| f.<.
-00002280: 9003 71ec 7c19 9004 73d4 7c0a 7286 7c1a  ..q.|...s.|.r.|.
-00002290: 7286 6417 7c02 6a0a 7c1f 6418 6602 3c00  r.d.|.j.|.d.f.<.
-000022a0: 6417 7c02 6a0a 7c1f 6419 6602 3c00 6417  d.|.j.|.d.f.<.d.
-000022b0: 7c02 6a0a 7c1f 641a 6602 3c00 6417 7c02  |.j.|.d.f.<.d.|.
-000022c0: 6a0a 7c1f 641b 6602 3c00 6417 7c02 6a0a  j.|.d.f.<.d.|.j.
-000022d0: 7c1f 641c 6602 3c00 6417 7c02 6a0a 7c1f  |.d.f.<.d.|.j.|.
-000022e0: 641d 6602 3c00 641e 7c02 6a01 7600 7286  d.f.<.d.|.j.v.r.
-000022f0: 6417 7c02 6a0a 7c1f 641e 6602 3c00 6417  d.|.j.|.d.f.<.d.
-00002300: 7c02 6a0a 7c1f 641f 6602 3c00 7186 7c02  |.j.|.d.f.<.q.|.
-00002310: 5300 2920 4e54 7207 0000 00da 0748 6173  S.) NTr......Has
-00002320: 5f50 4f49 da09 4861 735f 4761 7567 65da  _POI..Has_Gauge.
-00002330: 0742 6173 4172 6561 727c 0000 0072 6400  .BasArear|...rd.
-00002340: 0000 7201 0000 0072 0600 0000 720d 0000  ..r....r....r...
-00002350: 0072 6600 0000 4672 2800 0000 7265 0000  .rf...Fr(...re..
-00002360: 00da 066e 7375 6269 64da 0848 794c 616b  ...nsubid..HyLak
-00002370: 6549 6429 0472 0600 0000 720d 0000 0072  eId).r....r....r
-00002380: 6600 0000 7284 0000 00da 0a6e 646f 776e  f...r......ndown
-00002390: 7375 6269 64da 094f 6c64 5f53 7562 4964  subid..Old_SubId
-000023a0: da0c 4f6c 645f 446f 7753 7562 4964 7258  ..Old_DowSubIdrX
-000023b0: 0000 00da 0867 656f 6d65 7472 7972 6c00  .....geometryrl.
-000023c0: 0000 726d 0000 0072 6800 0000 7271 0000  ..rm...rh...rq..
-000023d0: 0072 6e00 0000 726f 0000 0072 7000 0000  .rn...ro...rp...
-000023e0: 7272 0000 0072 7300 0000 290b 7214 0000  rr...rs...).r...
-000023f0: 0072 1100 0000 7213 0000 0072 2900 0000  .r....r....r)...
-00002400: 7215 0000 0072 1a00 0000 da0a 6c6f 6769  r....r......logi
-00002410: 6361 6c5f 6f72 722b 0000 0072 7500 0000  cal_orr+...ru...
-00002420: 723f 0000 0072 1900 0000 2921 da0e 6d61  r?...r....)!..ma
-00002430: 706f 6c64 6e65 775f 696e 666f da0f 6172  poldnew_info..ar
-00002440: 6561 5f74 6872 6573 7468 6f6c 645a 126d  ea_threstholdZ.m
-00002450: 6170 6f6c 646e 6577 5f69 6e66 6f5f 6e65  apoldnew_info_ne
-00002460: 77da 0e47 6175 6765 5f63 6f6c 5f4e 616d  w..Gauge_col_Nam
-00002470: 655a 1273 6d61 6c6c 5f73 7562 5f6e 6f6e  eZ.small_sub_non
-00002480: 5f6c 616b 655a 1873 6d61 6c6c 5f73 7562  _lakeZ.small_sub
-00002490: 5f6e 6f6e 5f6c 616b 655f 7375 6269 6472  _non_lake_subidr
-000024a0: 4800 0000 5a0c 736d 616c 6c5f 7375 625f  H...Z.small_sub_
-000024b0: 6964 5a10 736d 616c 6c5f 646f 776e 7375  idZ.small_downsu
-000024c0: 625f 6964 5a10 736d 616c 6c5f 7375 625f  b_idZ.small_sub_
-000024d0: 7365 675f 6964 5a1b 736d 616c 6c5f 7375  seg_idZ.small_su
-000024e0: 625f 6973 5f68 6561 645f 7761 7465 725f  b_is_head_water_
-000024f0: 7375 625a 1573 6d61 6c6c 5f73 7562 5f69  subZ.small_sub_i
-00002500: 735f 6e6f 745f 4c61 6b65 5a16 736d 616c  s_not_LakeZ.smal
-00002510: 6c5f 7375 625f 6973 5f6e 6f74 5f67 6175  l_sub_is_not_gau
-00002520: 6765 5a0d 646f 776e 5f73 7562 5f69 6e66  geZ.down_sub_inf
-00002530: 6f5a 1175 7073 7472 6561 6d5f 7375 625f  oZ.upstream_sub_
-00002540: 696e 666f 5a1a 7570 7374 7265 616d 5f73  infoZ.upstream_s
-00002550: 7562 5f69 6e66 6f5f 7361 6d65 5f73 6567  ub_info_same_seg
-00002560: 5a0c 6861 735f 646f 776e 5f73 7562 5a18  Z.has_down_subZ.
-00002570: 646f 776e 5f73 7562 5f68 6173 5f73 616d  down_sub_has_sam
-00002580: 655f 7365 675f 6964 5a0c 6861 735f 7570  e_seg_idZ.has_up
-00002590: 7374 7265 616d 5a16 7570 5f73 7562 5f68  streamZ.up_sub_h
-000025a0: 6173 5f73 616d 655f 7365 675f 6964 da07  as_same_seg_id..
-000025b0: 7461 7269 6e66 6fda 066d 6f64 6966 795a  tarinfo..modifyZ
-000025c0: 0f64 6f77 6e5f 7375 625f 696e 666f 5f32  .down_sub_info_2
-000025d0: 5a0b 6e64 6f77 6e5f 7375 6269 645a 1263  Z.ndown_subidZ.c
-000025e0: 7572 7265 6e74 5f73 7562 5f69 6e66 6f5f  urrent_sub_info_
-000025f0: 325a 1c74 6172 6765 745f 7375 625f 6973  2Z.target_sub_is
-00002600: 5f68 6561 645f 7761 7465 725f 7375 625a  _head_water_subZ
-00002610: 2174 6172 6765 745f 7375 625f 6861 735f  !target_sub_has_
-00002620: 6c65 7373 5f6f 6e65 5f75 705f 7374 7265  less_one_up_stre
-00002630: 616d 724a 0000 005a 056d 6173 6b33 724b  amrJ...Z.mask3rK
-00002640: 0000 005a 086d 6173 6b74 656d 7072 2300  ...Z.masktempr#.
-00002650: 0000 da03 636f 6c72 2400 0000 7224 0000  ....colr$...r$..
-00002660: 0072 2500 0000 da1f 7265 6d6f 7665 5f70  .r%.....remove_p
-00002670: 6f73 7369 626c 655f 736d 616c 6c5f 7375  ossible_small_su
-00002680: 6262 6173 696e 73b8 0100 0073 bc00 0000  bbasins....s....
-00002690: 0001 0c03 0401 0a01 0403 2001 1801 1802  .......... .....
-000026a0: 0a03 1401 0e01 0e01 0e02 1802 1201 1202  ................
-000026b0: 1801 1801 1804 0e01 0401 1401 0602 0602  ................
-000026c0: 0401 0403 0e01 0402 2201 0602 0603 0401  ........".......
-000026d0: 0403 1803 2201 0401 2201 1002 1803 2201  ...."...".....".
-000026e0: 0401 1801 1002 2003 2201 0401 1801 1003  ...... .".......
-000026f0: 0401 0401 0202 0401 2201 2e02 0c01 0c01  ........".......
-00002700: 1601 0c01 0c02 2801 0a01 100c 0a01 0a02  ......(.........
-00002710: 3402 0a02 1a02 0a01 1002 06ff 0402 06fe  4...............
-00002720: 0403 06fd 0404 06fc 0405 06fb 0406 06fa  ................
-00002730: 0408 0602 1c02 0a01 0401 0e01 0e01 0e01  ................
-00002740: 0e01 0e01 0e01 0a01 0e01 100a 7290 0000  ............r...
-00002750: 0072 6b00 0000 6309 0000 0000 0000 0000  .rk...c.........
-00002760: 0000 0016 0000 0005 0000 0043 0000 0073  ...........C...s
-00002770: de04 0000 6401 7d09 7c01 6401 6402 6702  ....d.}.|.d.d.g.
-00002780: 1900 a000 6403 a101 6a01 7d0a 7c04 6404  ....d...j.}.|.d.
-00002790: 6b00 725e 7402 7c0a 7c00 8302 7d0b 7c03  k.r^t.|.|...}.|.
-000027a0: 6404 6b04 7258 7402 7c0a 7c03 8302 7d0c  d.k.rXt.|.|...}.
-000027b0: 7403 a004 7c0b 7c0c a102 7d0d 7c0b 7403  t...|.|...}.|.t.
-000027c0: a005 7c0d a101 1900 7d0e 7162 7c0b 7d0e  ..|.....}.qb|.}.
-000027d0: 6e04 7c05 7d0e 7c01 7c01 7c09 1900 a006  n.|.}.|.|.|.....
-000027e0: 7c0e a101 1900 a007 a100 7d0f 7c01 7c01  |.........}.|.|.
-000027f0: 7c09 1900 7c00 6b02 1900 a007 a100 7d10  |...|.k.......}.
-00002800: 7c06 6a08 7c06 6401 1900 a006 7c0e a101  |.j.|.d.....|...
-00002810: 1900 a007 a100 7d11 7c11 6a08 7c11 6405  ......}.|.j.|.d.
-00002820: 1900 6404 6b04 1900 a007 a100 7d11 7c10  ..d.k.......}.|.
-00002830: 6a09 6404 1900 7d12 740a 7c11 8301 6404  j.d...}.t.|...d.
-00002840: 6b04 9001 72e4 7403 a00b 7c11 6405 1900  k...r.t...|.d...
-00002850: 6a01 a101 7c10 6a08 7c12 6405 6602 3c00  j...|.j.|.d.f.<.
-00002860: 7403 6a0c 7c11 6406 1900 6a01 7c11 6405  t.j.|.d...j.|.d.
-00002870: 1900 6a01 6407 8d02 7c10 6a08 7c12 6406  ..j.d...|.j.|.d.
-00002880: 6602 3c00 7403 6a0c 7c11 6408 1900 6a01  f.<.t.j.|.d...j.
-00002890: 7c11 6405 1900 6a01 6407 8d02 7c10 6a08  |.d...j.d...|.j.
-000028a0: 7c12 6408 6602 3c00 7403 6a0c 7c11 6409  |.d.f.<.t.j.|.d.
-000028b0: 1900 6a01 7c11 6405 1900 6a01 6407 8d02  ..j.|.d...j.d...
-000028c0: 7c10 6a08 7c12 6409 6602 3c00 7403 6a0c  |.j.|.d.f.<.t.j.
-000028d0: 7c11 640a 1900 6a01 7c11 6405 1900 6a01  |.d...j.|.d...j.
-000028e0: 6407 8d02 7c10 6a08 7c12 640a 6602 3c00  d...|.j.|.d.f.<.
-000028f0: 7403 a00d 7c11 640b 1900 6a01 a101 7c10  t...|.d...j...|.
-00002900: 6a08 7c12 640b 6602 3c00 7403 a00d 7c11  j.|.d.f.<.t...|.
-00002910: 640c 1900 6a01 a101 7c10 6a08 7c12 640c  d...j...|.j.|.d.
-00002920: 6602 3c00 7403 a00d 7c11 640d 1900 6a01  f.<.t...|.d...j.
-00002930: a101 7c10 6a08 7c12 640d 6602 3c00 7403  ..|.j.|.d.f.<.t.
-00002940: a00e 7c11 640e 1900 6a01 a101 7c10 6a08  ..|.d...j...|.j.
-00002950: 7c12 640e 6602 3c00 7403 a00b 7c0f 640f  |.d.f.<.t...|.d.
-00002960: 1900 6a01 a101 7c10 6a08 7c12 640f 6602  ..j...|.j.|.d.f.
-00002970: 3c00 740a 7c0f 8301 6404 6b04 9002 7278  <.t.|...d.k...rx
-00002980: 7403 6a0c 7c0f 6410 1900 6a01 7c0f 640f  t.j.|.d...j.|.d.
-00002990: 1900 6a01 6407 8d02 7c10 6a08 7c12 6410  ..j.d...|.j.|.d.
-000029a0: 6602 3c00 7403 6a0c 7c0f 6411 1900 6a01  f.<.t.j.|.d...j.
-000029b0: 7c0f 640f 1900 6a01 6407 8d02 7c10 6a08  |.d...j.d...|.j.
-000029c0: 7c12 6411 6602 3c00 7403 6a0c 7c0f 6412  |.d.f.<.t.j.|.d.
-000029d0: 1900 6a01 7c0f 640f 1900 6a01 6407 8d02  ..j.|.d...j.d...
-000029e0: 7c10 6a08 7c12 6412 6602 3c00 7c07 6413  |.j.|.d.f.<.|.d.
-000029f0: 6b02 9003 7200 6414 7c10 6a08 7c12 6406  k...r.d.|.j.|.d.
-00002a00: 6602 3c00 6414 7c10 6a08 7c12 6405 6602  f.<.d.|.j.|.d.f.
-00002a10: 3c00 6414 7c10 6a08 7c12 6408 6602 3c00  <.d.|.j.|.d.f.<.
-00002a20: 6414 7c10 6a08 7c12 640a 6602 3c00 6414  d.|.j.|.d.f.<.d.
-00002a30: 7c10 6a08 7c12 640e 6602 3c00 6414 7c10  |.j.|.d.f.<.d.|.
-00002a40: 6a08 7c12 640d 6602 3c00 6415 7c10 6a0f  j.|.d.f.<.d.|.j.
-00002a50: 7600 9003 72f4 6414 7c10 6a08 7c12 6415  v...r.d.|.j.|.d.
-00002a60: 6602 3c00 6414 7c10 6a08 7c12 6416 6602  f.<.d.|.j.|.d.f.
-00002a70: 3c00 6ef4 7c07 6417 6b02 9003 7296 6414  <.n.|.d.k...r.d.
-00002a80: 7c10 6a08 7c12 6406 6602 3c00 6414 7c10  |.j.|.d.f.<.d.|.
-00002a90: 6a08 7c12 6405 6602 3c00 6414 7c10 6a08  j.|.d.f.<.d.|.j.
-00002aa0: 7c12 6408 6602 3c00 6414 7c10 6a08 7c12  |.d.f.<.d.|.j.|.
-00002ab0: 640a 6602 3c00 6414 7c10 6a08 7c12 640e  d.f.<.d.|.j.|.d.
-00002ac0: 6602 3c00 6414 7c10 6a08 7c12 640d 6602  f.<.d.|.j.|.d.f.
-00002ad0: 3c00 6415 7c10 6a0f 7600 9003 7286 6414  <.d.|.j.v...r.d.
-00002ae0: 7c10 6a08 7c12 6415 6602 3c00 6414 7c10  |.j.|.d.f.<.d.|.
-00002af0: 6a08 7c12 6416 6602 3c00 6417 7c10 6a08  j.|.d.f.<.d.|.j.
-00002b00: 7c12 6418 6602 3c00 6e5e 7c07 6404 6b01  |.d.f.<.n^|.d.k.
-00002b10: 9003 72f4 6404 7c10 6a08 7c12 6419 6602  ..r.d.|.j.|.d.f.
-00002b20: 3c00 6404 7c10 6a08 7c12 641a 6602 3c00  <.d.|.j.|.d.f.<.
-00002b30: 6404 7c10 6a08 7c12 641b 6602 3c00 6404  d.|.j.|.d.f.<.d.
-00002b40: 7c10 6a08 7c12 641c 6602 3c00 6404 7c10  |.j.|.d.f.<.d.|.
-00002b50: 6a08 7c12 641d 6602 3c00 6404 7c10 6a08  j.|.d.f.<.d.|.j.
-00002b60: 7c12 6418 6602 3c00 6414 7c10 6a08 7c12  |.d.f.<.d.|.j.|.
-00002b70: 641e 6602 3c00 6414 7c10 6a08 7c12 641f  d.f.<.d.|.j.|.d.
-00002b80: 6602 3c00 7c08 6404 6b04 9004 7228 7c08  f.<.|.d.k...r(|.
-00002b90: 7c10 6a08 7c12 6420 6602 3c00 7c02 6401  |.j.|.d f.<.|.d.
-00002ba0: 1900 a006 7c0e a101 7d13 7c02 6421 1900  ....|...}.|.d!..
-00002bb0: 7c00 6b02 7d14 7403 a010 7c13 7c14 a102  |.k.}.t...|.|...
-00002bc0: 7d0d 7c10 6a0f 4400 5d84 7d15 7c15 6401  }.|.j.D.].}.|.d.
-00002bd0: 6b02 9004 727c 7c10 7c15 1900 6a01 6404  k...r||.|...j.d.
-00002be0: 1900 7c02 6a08 7c0d 6421 6602 3c00 6e5a  ..|.j.|.d!f.<.nZ
-00002bf0: 7c15 6421 6b02 9004 7354 7c15 6422 6b02  |.d!k...sT|.d"k.
-00002c00: 9004 7354 7c15 6423 6b02 9004 7354 7c15  ..sT|.d#k...sT|.
-00002c10: 6424 6b02 9004 7354 7c15 6425 6b02 9004  d$k...sT|.d%k...
-00002c20: 7354 7c15 6426 6b02 9004 72be 9004 7154  sT|.d&k...r...qT
-00002c30: 6e18 7c10 7c15 1900 6a01 6404 1900 7c02  n.|.|...j.d...|.
-00002c40: 6a08 7c0d 7c15 6602 3c00 9004 7154 7c02  j.|.|.f.<...qT|.
-00002c50: 5300 2927 4e72 0600 0000 720d 0000 0072  S.)'Nr....r....r
-00002c60: 0900 0000 7201 0000 0072 6800 0000 726d  ....r....rh...rm
-00002c70: 0000 00a9 01da 0777 6569 6768 7473 7271  .......weightsrq
-00002c80: 0000 005a 0651 5f4d 6561 6e72 6e00 0000  ...Z.Q_Meanrn...
-00002c90: 5a08 426b 6657 6964 7468 5a08 426b 6644  Z.BkfWidthZ.BkfD
-00002ca0: 6570 7468 7270 0000 0072 6f00 0000 7282  epthrp...ro...r.
-00002cb0: 0000 00da 0842 6173 536c 6f70 655a 084d  .....BasSlopeZ.M
-00002cc0: 6561 6e45 6c65 765a 0942 6173 4173 7065  eanElevZ.BasAspe
-00002cd0: 6374 7228 0000 0072 6c00 0000 7272 0000  ctr(...rl...rr..
-00002ce0: 0072 7300 0000 7265 0000 0072 6400 0000  .rs...re...rd...
-00002cf0: 7284 0000 00da 074c 616b 6556 6f6c da08  r......LakeVol..
-00002d00: 4c61 6b65 4172 6561 da09 4c61 6b65 4465  LakeArea..LakeDe
-00002d10: 7074 68da 084c 616b 6574 7970 65da 0a63  pth..Laketype..c
-00002d20: 656e 7472 6f69 645f 78da 0a63 656e 7472  entroid_x..centr
-00002d30: 6f69 645f 7972 6a00 0000 7283 0000 0072  oid_yrj...r....r
-00002d40: 8500 0000 7286 0000 0072 8700 0000 7258  ....r....r....rX
-00002d50: 0000 0072 8800 0000 2911 7216 0000 0072  ...r....).r....r
-00002d60: 1300 0000 7217 0000 0072 1a00 0000 722e  ....r....r....r.
-00002d70: 0000 00da 0b6c 6f67 6963 616c 5f6e 6f74  .....logical_not
-00002d80: 7212 0000 0072 1400 0000 7219 0000 0072  r....r....r....r
-00002d90: 5900 0000 7215 0000 0072 3f00 0000 da07  Y...r....r?.....
-00002da0: 6176 6572 6167 6572 7400 0000 da03 6d69  averagert.....mi
-00002db0: 6e72 1100 0000 7289 0000 0029 1672 4900  nr....r....).rI.
-00002dc0: 0000 da0d 6361 7463 686d 656e 7469 6e66  ....catchmentinf
-00002dd0: 6f72 8a00 0000 5a07 7570 7375 6269 64da  or....Z.upsubid.
-00002de0: 0a69 736d 6f64 6966 6964 73da 0a6d 6f64  .ismodifids..mod
-00002df0: 6966 6969 6469 6eda 076d 6169 6e72 6976  ifiidin..mainriv
-00002e00: 7264 0000 00da 0973 6567 5f6f 7264 6572  rd.....seg_order
-00002e10: da09 7375 625f 636f 6c6e 6d72 7700 0000  ..sub_colnmrw...
-00002e20: 5a0e 4d6f 6469 6679 5f73 7562 6964 7331  Z.Modify_subids1
-00002e30: 5a0e 4d6f 6469 6679 5f73 7562 6964 7332  Z.Modify_subids2
-00002e40: 7223 0000 005a 0d4d 6f64 6966 795f 7375  r#...Z.Modify_su
-00002e50: 6269 6473 5a07 6362 7261 6e63 6872 8d00  bidsZ.cbranchr..
-00002e60: 0000 727e 0000 0072 5f00 0000 724a 0000  ..r~...r_...rJ..
-00002e70: 0072 4b00 0000 728f 0000 0072 2400 0000  .rK...r....r$...
-00002e80: 7224 0000 0072 2500 0000 da15 4e65 775f  r$...r%.....New_
-00002e90: 5375 6249 645f 546f 5f44 6973 736f 6c76  SubId_To_Dissolv
-00002ea0: 6553 0200 0073 da00 0000 000b 0401 1401  eS...s..........
-00002eb0: 0801 0201 04ff 0403 0801 0a01 0c01 1002  ................
-00002ec0: 0603 0404 1601 0201 0aff 0804 1801 1601  ................
-00002ed0: 0a02 0e01 1a01 0401 0801 08fe 1004 0401  ................
-00002ee0: 0801 08fe 1004 0401 0801 08fe 1004 0401  ................
-00002ef0: 0801 08fe 1004 1a01 1a02 1a01 1a02 1a02  ................
-00002f00: 0e01 0401 10ff 1003 0401 10ff 1003 0401  ................
-00002f10: 10ff 1005 06ff 0404 0e01 0e01 0e01 0e01  ................
-00002f20: 0e01 0e01 0c01 0e01 1002 0a01 0e01 0e01  ................
-00002f30: 0e01 0e01 0e01 0e01 0c01 0e01 0e01 1001  ................
-00002f40: 0a05 0e01 0e01 0e01 0e01 0e01 0e02 0e01  ................
-00002f50: 0e02 0a01 0e02 0801 02ff 0404 0aff 0203  ................
-00002f60: 0c03 0a01 0a02 1a03 06ff 0402 06fe 0403  ................
-00002f70: 06fd 0404 06fc 0405 06fb 0406 06fa 0408  ................
-00002f80: 0602 1c03 72a3 0000 0072 0600 0000 6303  ....r....r....c.
-00002f90: 0000 0000 0000 0000 0000 0008 0000 0004  ................
-00002fa0: 0000 0043 0000 0073 a400 0000 7c00 6a00  ...C...s....|.j.
-00002fb0: 7c01 6a00 6b03 a001 a100 7228 7402 7c00  |.j.k.....r(t.|.
-00002fc0: 6a00 8301 0100 7402 7c01 6a00 8301 0100  j.....t.|.j.....
-00002fd0: 6401 5300 6402 7d03 7c00 6a00 4400 5d62  d.S.d.}.|.j.D.]b
-00002fe0: 7d04 7c04 6403 6b02 7248 7c03 6404 1700  }.|.d.k.rH|.d...
-00002ff0: 7d03 7132 7c00 7c04 1900 6a03 7d05 7c01  }.q2|.|...j.}.|.
-00003000: 7c04 1900 6a03 7d06 7c05 7c06 6b03 a001  |...j.}.|.|.k...
-00003010: a100 728c 7402 7c04 8301 0100 7c05 7c06  ..r.t.|.....|.|.
-00003020: 6b03 7d07 7402 7c00 7c02 1900 6a03 7c07  k.}.t.|.|...j.|.
-00003030: 1900 8301 0100 7132 7c03 6404 1700 7d03  ......q2|.d...}.
-00003040: 7132 7c03 7404 7c00 6a00 8301 6b02 5300  q2|.t.|.j...k.S.
-00003050: 2905 4e46 7201 0000 00da 0648 5255 5f49  ).NFr......HRU_I
-00003060: 4472 2800 0000 2905 7211 0000 00da 0361  Dr(...).r......a
-00003070: 6c6c 7275 0000 0072 1300 0000 7215 0000  llru...r....r...
-00003080: 0029 085a 0845 7870 6563 7465 645a 0652  .).Z.ExpectedZ.R
-00003090: 6573 756c 745a 0c43 6865 636b 5f43 6f6c  esultZ.Check_Col
-000030a0: 5f4e 4d5a 046e 6571 6c72 8f00 0000 5a0c  _NMZ.neqlr....Z.
-000030b0: 4172 7261 795f 6578 7065 6374 5a0c 4172  Array_expectZ.Ar
-000030c0: 7261 795f 7265 7375 6c74 7223 0000 0072  ray_resultr#...r
-000030d0: 2400 0000 7224 0000 0072 2500 0000 da17  $...r$...r%.....
-000030e0: 4576 616c 7561 7465 5f54 776f 5f44 6174  Evaluate_Two_Dat
-000030f0: 6166 7261 6d65 73e7 0200 0073 2200 0000  aframes....s"...
-00003100: 0002 1001 0a01 0a01 0401 0402 0a01 0801  ................
-00003110: 0801 0201 0a01 0a01 0c01 0801 0801 1402  ................
-00003120: 0a02 72a6 0000 0063 0300 0000 0000 0000  ..r....c........
-00003130: 0000 0000 0b00 0000 0500 0000 4300 0000  ............C...
-00003140: 73ac 0100 007c 006a 007d 037c 0264 016b  s....|.j.}.|.d.k
-00003150: 0472 e274 0164 0174 027c 0383 0183 0244  .r.t.d.t.|.....D
-00003160: 005d 8c7d 047c 006a 037c 037c 0419 0064  .].}.|.j.|.|...d
-00003170: 0266 0219 007d 057c 006a 037c 037c 0419  .f...}.|.j.|.|..
-00003180: 0064 0366 0219 007d 067c 006a 037c 037c  .d.f...}.|.j.|.|
-00003190: 0419 0064 0466 0219 007d 077c 006a 037c  ...d.f...}.|.j.|
-000031a0: 0064 0319 007c 076b 0219 00a0 04a1 007d  .d...|.k.......}
-000031b0: 0874 027c 0883 0164 016b 0472 967c 0864  .t.|...d.k.r.|.d
-000031c0: 0219 006a 0564 0119 007c 006a 037c 037c  ...j.d...|.j.|.|
-000031d0: 0419 0064 0566 023c 0071 1c64 067c 006a  ...d.f.<.q.d.|.j
-000031e0: 037c 037c 0419 0064 0566 023c 0071 1c7c  .|.|...d.f.<.q.|
-000031f0: 0064 0319 006a 057c 0064 073c 007c 0064  .d...j.|.d.<.|.d
-00003200: 0419 006a 057c 0064 083c 007c 0064 0219  ...j.|.d.<.|.d..
-00003210: 006a 057c 0064 033c 007c 0064 0519 006a  .j.|.d.<.|.d...j
-00003220: 057c 0064 043c 007c 0164 016b 0072 ee7c  .|.d.<.|.d.k.r.|
-00003230: 0053 007c 006a 0664 0364 0964 0a8d 027d  .S.|.j.d.d.d...}
-00003240: 0974 077c 0983 017d 0974 0164 0174 027c  .t.|...}.t.d.t.|
-00003250: 0983 0183 0244 005d 947d 047c 0964 0319  .....D.].}.|.d..
-00003260: 006a 057c 0419 007d 0a7c 0964 0b19 006a  .j.|...}.|.d...j
-00003270: 057c 0419 007c 006a 037c 0064 0319 007c  .|...|.j.|.d...|
-00003280: 0a6b 0264 0b66 023c 007c 0964 0c19 006a  .k.d.f.<.|.d...j
-00003290: 057c 0419 007c 006a 037c 0064 0319 007c  .|...|.j.|.d...|
-000032a0: 0a6b 0264 0c66 023c 007c 0964 0d19 006a  .k.d.f.<.|.d...j
-000032b0: 057c 0419 007c 006a 037c 0064 0319 007c  .|...|.j.|.d...|
-000032c0: 0a6b 0264 0d66 023c 007c 0964 0e19 006a  .k.d.f.<.|.d...j
-000032d0: 057c 0419 007c 006a 037c 0064 0319 007c  .|...|.j.|.d...|
-000032e0: 0a6b 0264 0e66 023c 0090 0171 127c 0053  .k.d.f.<...q.|.S
-000032f0: 0029 0ffa df46 756e 6374 696f 6e73 2077  .)...Functions w
-00003300: 696c 6c20 7570 6461 7465 2073 7562 6964  ill update subid
-00003310: 2c64 6f77 6e73 7562 6964 2c20 6361 6c63  ,downsubid, calc
-00003320: 7561 7465 2073 7472 6561 6d20 6f72 6465  uate stream orde
-00003330: 7220 616e 640a 2020 2020 2020 2020 7570  r and.        up
-00003340: 6461 7465 2064 7261 696e 6167 6520 6172  date drainage ar
-00003350: 6561 2069 6e20 7468 6520 6174 7472 6962  ea in the attrib
-00003360: 7574 6520 7461 626c 6520 6d61 706f 6c64  ute table mapold
-00003370: 6e65 775f 696e 666f 0a20 2020 202d 2d2d  new_info.    ---
-00003380: 2d2d 2d2d 2d2d 2d0a 0a20 2020 204e 6f74  -------..    Not
-00003390: 6573 0a20 2020 202d 2d2d 2d2d 2d2d 0a0a  es.    -------..
-000033a0: 2020 2020 5265 7475 726e 733a 0a20 2020      Returns:.   
-000033b0: 202d 2d2d 2d2d 2d2d 0a20 2020 2020 2020   -------.       
-000033c0: 206d 6170 6f6c 646e 6577 5f69 6e66 6f0a   mapoldnew_info.
-000033d0: 2020 2020 7201 0000 0072 8300 0000 7206      r....r....r.
-000033e0: 0000 0072 0d00 0000 7285 0000 0072 6b00  ...r....r....rk.
-000033f0: 0000 7286 0000 0072 8700 0000 723a 0000  ..r....r....r:..
-00003400: 00a9 0172 3c00 0000 7269 0000 0072 6600  ...r<...ri...rf.
-00003410: 0000 726a 0000 0072 7900 0000 2908 7259  ..rj...ry...).rY
-00003420: 0000 0072 2900 0000 7215 0000 0072 1900  ...r)...r....r..
-00003430: 0000 7214 0000 0072 1300 0000 7242 0000  ..r....r....rB..
-00003440: 00da 1a73 7472 6561 6d6f 7264 6572 616e  ...streamorderan
-00003450: 6464 7261 696e 6167 6561 7265 6129 0b72  ddrainagearea).r
-00003460: 8a00 0000 da11 5570 6461 7465 5374 7265  ......UpdateStre
-00003470: 616d 6f72 6465 72da 0b55 7064 6174 6553  amorder..UpdateS
-00003480: 7562 4964 725f 0000 0072 4800 0000 7283  ubIdr_...rH...r.
-00003490: 0000 0072 4900 0000 da0a 6f64 6f77 6e73  ...rI.....odowns
-000034a0: 7562 6964 da0c 646f 6e73 7562 6964 696e  ubid..donsubidin
-000034b0: 666f da15 6d61 706f 6c64 6e65 775f 696e  fo..mapoldnew_in
-000034c0: 666f 5f75 6e69 7175 65da 0669 7375 6269  fo_unique..isubi
-000034d0: 6472 2400 0000 7224 0000 0072 2500 0000  dr$...r$...r%...
-000034e0: da0e 5570 6461 7465 546f 706f 6c6f 6779  ..UpdateTopology
-000034f0: ff02 0000 7356 0000 0000 0d06 0208 0112  ....sV..........
-00003500: 0112 0112 0112 0204 010a ff08 040c 0102  ................
-00003510: 0102 ff04 0202 fe14 0414 020e 010e 010e  ................
-00003520: 020e 0208 0104 020e 0208 0212 010e 030c  ................
-00003530: fe04 010e ff02 050c fe04 010e ff02 050c  ................
-00003540: fe04 010e ff02 050c fe04 010e ff06 0472  ...............r
-00003550: b000 0000 6303 0000 0000 0000 0000 0000  ....c...........
-00003560: 0008 0000 0005 0000 0043 0000 0073 8a00  .........C...s..
-00003570: 0000 6401 7c00 6402 1b00 6402 1b00 6403  ..d.|.d...d...d.
-00003580: 1300 1400 7d03 6404 7c01 6402 1b00 1400  ....}.d.|.d.....
-00003590: 7c00 6402 1b00 6402 1b00 6405 1300 1400  |.d...d...d.....
-000035a0: 7c02 6406 1300 1400 7d04 6407 7c01 6402  |.d.....}.d.|.d.
-000035b0: 1b00 6408 1300 1400 7c02 6409 1300 1400  ..d.....|.d.....
-000035c0: 7d05 640a 7c01 6402 1b00 7c02 6403 1300  }.d.|.d...|.d...
-000035d0: 1b00 640b 1300 1400 7d06 640c 7c01 7c02  ..d.....}.d.|.|.
-000035e0: 6403 1300 1b00 640d 1300 1400 7d07 7c03  d.....d.....}.|.
-000035f0: 7c04 7c05 7c06 7c07 6605 5300 290e 4e67  |.|.|.|.f.S.).Ng
-00003600: 9a99 9999 9999 e53f 727c 0000 00e7 0000  .......?r|......
-00003610: 0000 0000 e03f 6793 3a01 4d84 0dcf 3f67  .....?g.:.M...?g
-00003620: 9a99 9999 9999 b9bf 679a 9999 9999 99c9  ........g.......
-00003630: bf67 3333 3333 3333 d33f 6752 b81e 85eb  .g333333.?gR....
-00003640: 51e8 3f67 52b8 1e85 eb51 c8bf 67ab aaaa  Q.?gR....Q..g...
-00003650: aaaa aa12 4067 14ae 47e1 7a14 de3f 67c2  ....@g..G.z..?g.
-00003660: 0fe1 72cf cd41 3f67 48e1 7a14 ae47 e93f  ..r..A?gH.z..G.?
-00003670: 7224 0000 0029 0872 7900 0000 7272 0000  r$...).ry...rr..
-00003680: 0072 7300 0000 5a04 5443 5f31 5a04 5443  .rs...Z.TC_1Z.TC
-00003690: 5f32 5a04 5443 5f33 5a04 5443 5f34 5a04  _2Z.TC_3Z.TC_4Z.
-000036a0: 5443 5f35 7224 0000 0072 2400 0000 7225  TC_5r$...r$...r%
-000036b0: 0000 00da 0c63 616c 6375 6c61 7465 5f54  .....calculate_T
-000036c0: 633d 0300 0073 0c00 0000 0002 1401 2401  c=...s........$.
-000036d0: 1801 1801 1401 72b2 0000 0063 0100 0000  ......r....c....
-000036e0: 0000 0000 0000 0000 1800 0000 0700 0000  ................
-000036f0: 4300 0000 73be 0900 0064 017d 0164 017c  C...s....d.}.d.|
-00003700: 006a 0076 0172 1264 027d 017c 006a 017c  .j.v.r.d.}.|.j.|
-00003710: 0064 0319 0064 046b 0319 00a0 02a1 007d  .d...d.k.......}
-00003720: 027c 006a 017c 0064 0319 0064 046b 0219  .|.j.|.d...d.k..
-00003730: 00a0 02a1 007d 037c 0364 0564 0667 0219  .....}.|.d.d.g..
-00003740: 00a0 0364 07a1 016a 047d 0474 05a0 0674  ...d...j.}.t...t
-00003750: 077c 0283 0164 08a1 027d 0564 097d 0664  .|...d...}.d.}.d
-00003760: 0a7d 0774 0864 0974 077c 0283 0183 0244  .}.t.d.t.|.....D
-00003770: 0090 015d fc7d 087c 026a 097c 0819 007d  ...].}.|.j.|...}
-00003780: 097c 0264 0519 006a 047c 0819 007c 0264  .|.d...j.|...|.d
-00003790: 0619 006a 047c 0819 006b 0272 b264 0b7c  ...j.|...k.r.d.|
-000037a0: 026a 017c 0964 0666 023c 007c 0264 0519  .j.|.d.f.<.|.d..
-000037b0: 006a 047c 0819 007d 0a74 077c 027c 0264  .j.|...}.t.|.|.d
-000037c0: 0619 007c 0a6b 0219 0083 0164 096b 0272  ...|.k.....d.k.r
-000037d0: 7874 0a7c 0264 0619 006a 047c 0819 0083  xt.|.d...j.|....
-000037e0: 017c 057c 063c 0074 077c 0483 0164 096b  .|.|.<.t.|...d.k
-000037f0: 0290 0172 0664 0c7d 0b64 0c7d 0c6e 6274  ...r.d.}.d.}.nbt
-00003800: 0b7c 047c 0a83 027d 0d7c 036a 017c 0364  .|.|...}.|.j.|.d
-00003810: 0519 00a0 0c7c 0da1 0119 00a0 02a1 007d  .....|.........}
-00003820: 0e74 077c 0e83 0164 096b 0490 0172 6074  .t.|...d.k...r`t
-00003830: 0d7c 0e64 0d19 006a 0483 017d 0b74 056a  .|.d...j...}.t.j
-00003840: 0e7c 0e64 0e19 006a 047c 0e64 0d19 006a  .|.d...j.|.d...j
-00003850: 0464 0f8d 027d 0c6e 0864 0c7d 0b64 0c7d  .d...}.n.d.}.d.}
-00003860: 0c7c 0b7c 0264 0d19 006a 047c 0819 0017  .|.|.d...j.|....
-00003870: 007c 026a 017c 0964 1066 023c 0064 0a7c  .|.j.|.d.f.<.d.|
-00003880: 026a 017c 0964 1166 023c 0064 0a7c 026a  .j.|.d.f.<.d.|.j
-00003890: 017c 0964 1266 023c 007c 077c 026a 017c  .|.d.f.<.|.|.j.|
-000038a0: 0964 1366 023c 0064 147c 026a 0076 0090  .d.f.<.d.|.j.v..
-000038b0: 0172 d664 157c 026a 017c 0964 1466 023c  .r.d.|.j.|.d.f.<
-000038c0: 0064 157c 026a 017c 0964 1666 023c 0064  .d.|.j.|.d.f.<.d
-000038d0: 157c 026a 017c 0964 1766 023c 0064 157c  .|.j.|.d.f.<.d.|
-000038e0: 026a 017c 0964 1866 023c 0064 157c 026a  .j.|.d.f.<.d.|.j
-000038f0: 017c 0964 1966 023c 0064 157c 026a 017c  .|.d.f.<.d.|.j.|
-00003900: 0964 1a66 023c 0064 157c 026a 017c 0964  .d.f.<.d.|.j.|.d
-00003910: 1b66 023c 0064 157c 026a 017c 0964 1c66  .f.<.d.|.j.|.d.f
-00003920: 023c 007c 0264 0e19 006a 047c 0819 007c  .<.|.d...j.|...|
-00003930: 0264 0d19 006a 047c 0819 0014 007c 0b7c  .d...j.|.....|.|
-00003940: 0c14 0017 007c 026a 017c 0964 1066 0219  .....|.j.|.d.f..
-00003950: 001b 007c 026a 017c 0964 1d66 023c 007c  ...|.j.|.d.f.<.|
-00003960: 0664 0a17 007d 067c 0764 0a17 007d 0771  .d...}.|.d...}.q
-00003970: 7874 05a0 0f7c 05a1 017d 057c 057c 0564  xt...|...}.|.|.d
-00003980: 096b 0419 007d 0574 05a0 0674 077c 0283  .k...}.t...t.|..
-00003990: 0164 08a1 027d 0f64 097d 1074 0864 0974  .d...}.d.}.t.d.t
-000039a0: 077c 0583 0183 0244 0090 045d a27d 087c  .|.....D...].}.|
-000039b0: 057c 0819 007d 0a64 0a7d 117c 1164 0a6b  .|...}.d.}.|.d.k
-000039c0: 0290 0272 b07c 0a64 096b 0490 0272 b07c  ...r.|.d.k...r.|
-000039d0: 026a 017c 0264 0619 007c 0a6b 0219 00a0  .j.|.d...|.k....
-000039e0: 02a1 007d 127c 026a 017c 0264 0519 007c  ...}.|.j.|.d...|
-000039f0: 0a6b 0219 00a0 02a1 007d 137c 0264 0519  .k.......}.|.d..
-00003a00: 007c 0a6b 027d 1474 077c 0483 0164 096b  .|.k.}.t.|...d.k
-00003a10: 0290 0372 2664 0c7d 0b64 0c7d 0c6e 6274  ...r&d.}.d.}.nbt
-00003a20: 0b7c 047c 0a83 027d 0d7c 036a 017c 0364  .|.|...}.|.j.|.d
-00003a30: 0519 00a0 0c7c 0da1 0119 00a0 02a1 007d  .....|.........}
-00003a40: 0e74 077c 0e83 0164 096b 0490 0372 8074  .t.|...d.k...r.t
-00003a50: 0d7c 0e64 0d19 006a 0483 017d 0b74 056a  .|.d...j...}.t.j
-00003a60: 0e7c 0e64 0e19 006a 047c 0e64 0d19 006a  .|.d...j.|.d...j
-00003a70: 0464 0f8d 027d 0c6e 0864 0c7d 0b64 0c7d  .d...}.n.d.}.d.}
-00003a80: 0c74 077c 1383 0164 096b 0190 0372 9a90  .t.|...d.k...r..
-00003a90: 0271 b074 077c 1283 0164 0a6b 0290 0572  .q.t.|...d.k...r
-00003aa0: 267c 1364 0d19 006a 0464 0919 007c 1264  &|.d...j.d...|.d
-00003ab0: 1019 006a 0464 0919 0017 007c 0b17 007c  ...j.d.....|...|
-00003ac0: 026a 017c 1464 1066 023c 007c 1264 1119  .j.|.d.f.<.|.d..
-00003ad0: 006a 0464 0919 007c 026a 017c 1464 1166  .j.d...|.j.|.d.f
-00003ae0: 023c 007c 1264 1219 006a 0464 0919 0064  .<.|.d...j.d...d
-00003af0: 0a17 007c 026a 017c 1464 1266 023c 007c  ...|.j.|.d.f.<.|
-00003b00: 1264 1319 006a 0464 0919 007c 026a 017c  .d...j.d...|.j.|
-00003b10: 1464 1366 023c 0064 147c 026a 0076 0090  .d.f.<.d.|.j.v..
-00003b20: 0572 1074 05a0 107c 1264 1419 006a 0464  .r.t...|.d...j.d
-00003b30: 0919 0064 09a1 027c 1364 1719 006a 0464  ...d...|.d...j.d
-00003b40: 0919 0017 007c 026a 017c 1464 1466 023c  .....|.j.|.d.f.<
-00003b50: 007c 1364 1819 006a 0464 0919 0074 05a0  .|.d...j.d...t..
-00003b60: 107c 1364 1719 006a 0464 0919 0064 09a1  .|.d...j.d...d..
-00003b70: 0214 007c 1264 1419 006a 0464 0919 0074  ...|.d...j.d...t
-00003b80: 05a0 107c 1264 1619 006a 0464 0919 0064  ...|.d...j.d...d
-00003b90: 09a1 0214 0017 007c 026a 017c 1464 1466  .......|.j.|.d.f
-00003ba0: 0219 001b 007c 026a 017c 1464 1666 023c  .....|.j.|.d.f.<
-00003bb0: 007c 1364 0e19 006a 0464 0919 007c 1364  .|.d...j.d...|.d
-00003bc0: 0d19 006a 0464 0919 0014 007c 0b7c 0c14  ...j.d.....|.|..
-00003bd0: 0017 007c 1264 1d19 006a 0464 0919 007c  ...|.d...j.d...|
-00003be0: 1264 1019 006a 0464 0919 0014 0017 007c  .d...j.d.......|
-00003bf0: 026a 017c 1464 1066 0219 001b 007c 026a  .j.|.d.f.....|.j
-00003c00: 017c 1464 1d66 023c 0074 0a7c 1364 0619  .|.d.f.<.t.|.d..
-00003c10: 006a 0464 0919 0083 017d 0a90 0271 c274  .j.d.....}...q.t
-00003c20: 05a0 117c 1264 1119 006a 04a1 0164 096b  ...|.d...j...d.k
-00003c30: 0490 0772 3664 147c 126a 0076 0090 0572  ...r6d.|.j.v...r
-00003c40: 567c 126a 1264 1464 1e64 1f8d 027d 127c  V|.j.d.d.d...}.|
-00003c50: 1364 0d19 006a 0464 0919 0074 05a0 0d7c  .d...j.d...t...|
-00003c60: 1264 1019 006a 04a1 0117 007c 0b17 007c  .d...j.....|...|
-00003c70: 026a 017c 1464 1066 023c 0064 147c 026a  .j.|.d.f.<.d.|.j
-00003c80: 0076 0090 0672 7474 05a0 107c 1264 1419  .v...rtt...|.d..
-00003c90: 006a 0464 0919 0064 09a1 027c 1364 1719  .j.d...d...|.d..
-00003ca0: 006a 0464 0919 0017 007c 026a 017c 1464  .j.d.....|.j.|.d
-00003cb0: 1466 023c 007c 1364 1819 006a 0464 0919  .f.<.|.d...j.d..
-00003cc0: 0074 05a0 107c 1364 1719 006a 0464 0919  .t...|.d...j.d..
-00003cd0: 0064 09a1 0214 007c 1264 1419 006a 0464  .d.....|.d...j.d
-00003ce0: 0919 0074 05a0 107c 1264 1619 006a 0464  ...t...|.d...j.d
-00003cf0: 0919 0064 09a1 0214 0017 007c 026a 017c  ...d.......|.j.|
-00003d00: 1464 1466 0219 001b 007c 026a 017c 1464  .d.f.....|.j.|.d
-00003d10: 1666 023c 007c 1364 0e19 006a 0464 0919  .f.<.|.d...j.d..
-00003d20: 007c 1364 0d19 006a 0464 0919 0014 007c  .|.d...j.d.....|
-00003d30: 0b7c 0c14 0017 007c 1264 1d19 006a 0464  .|.....|.d...j.d
-00003d40: 0919 007c 1264 1019 006a 0464 0919 0014  ...|.d...j.d....
-00003d50: 0017 007c 026a 017c 1464 1066 0219 001b  ...|.j.|.d.f....
-00003d60: 007c 026a 017c 1464 1d66 023c 0074 05a0  .|.j.|.d.f.<.t..
-00003d70: 117c 1264 1119 006a 04a1 0174 05a0 137c  .|.d...j...t...|
-00003d80: 1264 1119 006a 04a1 016b 0290 0672 dc7c  .d...j...k...r.|
-00003d90: 1264 1119 006a 0464 0919 0064 0a17 007c  .d...j.d...d...|
-00003da0: 026a 017c 1464 1166 023c 0064 0a7c 026a  .j.|.d.f.<.d.|.j
-00003db0: 017c 1464 1266 023c 007c 0764 0a17 007c  .|.d.f.<.|.d...|
-00003dc0: 026a 017c 1464 1366 023c 007c 0764 0a17  .j.|.d.f.<.|.d..
-00003dd0: 007d 076e 4674 05a0 137c 1264 1119 006a  .}.nFt...|.d...j
-00003de0: 04a1 017d 157c 157c 026a 017c 1464 1166  ...}.|.|.j.|.d.f
-00003df0: 023c 0064 0a7c 026a 017c 1464 1266 023c  .<.d.|.j.|.d.f.<
-00003e00: 007c 0764 0a17 007c 026a 017c 1464 1366  .|.d...|.j.|.d.f
-00003e10: 023c 007c 0764 0a17 007d 0774 0a7c 1364  .<.|.d...}.t.|.d
-00003e20: 0619 006a 0464 0919 0083 017d 0a6e 1874  ...j.d.....}.n.t
-00003e30: 0a7c 0a83 017c 0f7c 103c 007c 1064 0a17  .|...|.|.<.|.d..
-00003e40: 007d 1064 097d 1190 0271 c290 0271 b07c  .}.d.}...q...q.|
-00003e50: 0064 0519 00a0 0c7c 0264 0519 006a 04a1  .d.....|.d...j..
-00003e60: 017d 167c 0264 1319 006a 047c 006a 017c  .}.|.d...j.|.j.|
-00003e70: 1664 1366 023c 007c 0264 1219 006a 047c  .d.f.<.|.d...j.|
-00003e80: 006a 017c 1664 1266 023c 007c 0264 1119  .j.|.d.f.<.|.d..
-00003e90: 006a 047c 006a 017c 1664 1166 023c 007c  .j.|.j.|.d.f.<.|
-00003ea0: 0264 1319 006a 047c 006a 017c 1664 1366  .d...j.|.j.|.d.f
-00003eb0: 023c 007c 0264 1019 006a 047c 006a 017c  .<.|.d...j.|.j.|
-00003ec0: 1664 1066 023c 0064 147c 006a 0076 0090  .d.f.<.d.|.j.v..
-00003ed0: 0872 167c 0264 1419 006a 047c 006a 017c  .r.|.d...j.|.j.|
-00003ee0: 1664 1466 023c 007c 0264 1d19 006a 047c  .d.f.<.|.d...j.|
-00003ef0: 006a 017c 1664 1d66 023c 007c 0264 1619  .j.|.d.f.<.|.d..
-00003f00: 006a 047c 006a 017c 1664 1666 023c 007c  .j.|.j.|.d.f.<.|
-00003f10: 0264 1719 006a 047c 006a 017c 1664 1766  .d...j.|.j.|.d.f
-00003f20: 023c 007c 0264 1819 006a 047c 006a 017c  .<.|.d...j.|.j.|
-00003f30: 1664 1866 023c 0074 0864 0974 077c 0083  .d.f.<.t.d.t.|..
-00003f40: 0183 0244 0090 015d 6a7d 087c 006a 097c  ...D...]j}.|.j.|
-00003f50: 0819 007d 097c 007c 0119 006a 047c 0819  ...}.|.|...j.|..
-00003f60: 0064 096b 0490 0872 b27c 0064 2019 006a  .d.k...r.|.d ..j
-00003f70: 047c 0819 0064 096b 0490 0872 b27c 0064  .|...d.k...r.|.d
-00003f80: 1019 006a 047c 0819 0064 211b 0064 211b  ...j.|...d!..d!.
-00003f90: 007c 0064 2019 006a 047c 0819 001b 007c  .|.d ..j.|.....|
-00003fa0: 006a 017c 0964 2266 023c 007c 0064 0319  .j.|.d"f.<.|.d..
-00003fb0: 006a 047c 0819 0064 046b 0290 0872 4c7c  .j.|...d.k...rL|
-00003fc0: 0064 0519 006a 047c 0819 007d 0a74 0b7c  .d...j.|...}.t.|
-00003fd0: 047c 0a83 027d 0d7c 036a 017c 0364 0519  .|...}.|.j.|.d..
-00003fe0: 00a0 0c7c 0da1 0119 006a 0264 2364 248d  ...|.....j.d#d$.
-00003ff0: 017d 0e74 0d7c 0e64 0d19 006a 0483 017d  .}.t.|.d...j...}
-00004000: 177c 177c 006a 017c 0964 1066 023c 0074  .|.|.j.|.d.f.<.t
-00004010: 056a 0e7c 0e64 0e19 006a 047c 0e64 0d19  .j.|.d...j.|.d..
-00004020: 006a 0464 0f8d 027c 006a 017c 0964 1d66  .j.d...|.j.|.d.f
-00004030: 023c 0064 157c 006a 017c 0964 1766 023c  .<.d.|.j.|.d.f.<
-00004040: 0064 157c 006a 017c 0964 1866 023c 0064  .d.|.j.|.d.f.<.d
-00004050: 157c 006a 017c 0964 1966 023c 0064 157c  .|.j.|.d.f.<.d.|
-00004060: 006a 017c 0964 1c66 023c 0064 157c 006a  .j.|.d.f.<.d.|.j
-00004070: 017c 0964 1a66 023c 0064 157c 006a 017c  .|.d.f.<.d.|.j.|
-00004080: 0964 1b66 023c 0064 147c 006a 0076 0090  .d.f.<.d.|.j.v..
-00004090: 0872 4c64 157c 006a 017c 0964 1666 023c  .rLd.|.j.|.d.f.<
-000040a0: 0064 157c 006a 017c 0964 1466 023c 0090  .d.|.j.|.d.f.<..
-000040b0: 0871 4c7c 0053 0029 257a c046 756e 6374  .qL|.S.)%z.Funct
-000040c0: 696f 6e73 2077 696c 6c20 2063 616c 6375  ions will  calcu
-000040d0: 6174 6520 7374 7265 616d 206f 7264 6572  ate stream order
-000040e0: 2061 6e64 0a20 2020 2020 2020 2075 7064   and.        upd
-000040f0: 6174 6520 6472 6169 6e61 6765 2061 7265  ate drainage are
-00004100: 6120 696e 2074 6865 2061 7474 7269 6275  a in the attribu
-00004110: 7465 2074 6162 6c65 2063 6174 696e 666f  te table catinfo
-00004120: 616c 6c0a 2020 2020 2d2d 2d2d 2d2d 2d2d  all.    --------
-00004130: 2d2d 0a0a 2020 2020 4e6f 7465 730a 2020  --..    Notes.  
-00004140: 2020 2d2d 2d2d 2d2d 2d0a 0a20 2020 2052    -------..    R
-00004150: 6574 7572 6e73 3a0a 2020 2020 2d2d 2d2d  eturns:.    ----
-00004160: 2d2d 2d0a 2020 2020 2020 2020 6361 7469  ---.        cati
-00004170: 6e66 6f61 6c6c 0a20 2020 2072 8000 0000  nfoall.    r....
-00004180: 7281 0000 0072 6400 0000 7265 0000 0072  r....rd...re...r
-00004190: 0600 0000 720d 0000 0072 6300 0000 69f7  ....r....rc...i.
-000041a0: ffff ff72 0100 0000 7228 0000 0072 6b00  ...r....r(...rk.
-000041b0: 0000 7267 0000 0072 8200 0000 7293 0000  ..rg...r....r...
-000041c0: 0072 9100 0000 7279 0000 0072 6900 0000  .r....ry...ri...
-000041d0: 726a 0000 0072 6600 0000 7272 0000 0072  rj...rf...rr...r
-000041e0: 6c00 0000 7273 0000 0072 6800 0000 726d  l...rs...rh...rm
-000041f0: 0000 0072 6f00 0000 7271 0000 0072 6e00  ...ro...rq...rn.
-00004200: 0000 7270 0000 005a 0844 415f 536c 6f70  ..rp...Z.DA_Slop
-00004210: 6546 7237 0000 00da 0644 415f 4f62 73e7  eFr7.....DA_Obs.
-00004220: 0000 0000 0040 8f40 da08 4441 5f65 7272  .....@.@..DA_err
-00004230: 6f72 5472 0700 0000 2914 7211 0000 0072  orTr....).r....r
-00004240: 1900 0000 7214 0000 0072 1600 0000 7213  ....r....r....r.
-00004250: 0000 0072 1a00 0000 727d 0000 0072 1500  ...r....r}...r..
-00004260: 0000 7229 0000 0072 5900 0000 722d 0000  ..r)...rY...r-..
-00004270: 0072 1700 0000 7212 0000 0072 3f00 0000  .r....r....r?...
-00004280: 729b 0000 0072 2b00 0000 da07 6d61 7869  r....r+.....maxi
-00004290: 6d75 6d72 9c00 0000 7241 0000 0072 7400  mumr....rA...rt.
-000042a0: 0000 2918 5a0a 6361 7469 6e66 6f61 6c6c  ..).Z.catinfoall
-000042b0: 728c 0000 0072 7600 0000 5a0b 6361 7469  r....rv...Z.cati
-000042c0: 6e66 6f5f 6e63 6c5a 0b72 6f75 7469 6e67  nfo_nclZ.routing
-000042d0: 5f6e 636c 5a07 6361 746c 6973 745a 0469  _nclZ.catlistZ.i
-000042e0: 6361 74da 0469 7365 6772 4800 0000 725f  cat..isegrH...r_
-000042f0: 0000 00da 0563 6174 6964 5a06 4441 5f6e  .....catidZ.DA_n
-00004300: 636c 5a07 736c 705f 6e63 6c5a 0c55 7073  clZ.slp_nclZ.Ups
-00004310: 7472 6561 6d63 6174 735a 0b55 705f 6361  treamcatsZ.Up_ca
-00004320: 745f 696e 666f 5a0a 6e65 7763 6174 6c69  t_infoZ.newcatli
-00004330: 7374 5a09 696e 6577 7374 6172 745a 0b46  stZ.inewstartZ.F
-00004340: 5f69 6e74 6572 7365 6374 5a0f 5570 5f52  _intersectZ.Up_R
-00004350: 6561 6368 6573 5f69 6e66 6f5a 0e63 7572  eaches_infoZ.cur
-00004360: 5f52 6561 6368 5f69 6e66 6f5a 0a63 7572  _Reach_infoZ.cur
-00004370: 6361 745f 6964 785a 0d6d 6178 5f73 7472  cat_idxZ.max_str
-00004380: 616f 7264 6572 7223 0000 005a 0244 4172  aorderr#...Z.DAr
-00004390: 2400 0000 7224 0000 0072 2500 0000 72a9  $...r$...r%...r.
-000043a0: 0000 0047 0300 0073 6001 0000 000c 0401  ...G...s`.......
-000043b0: 0a01 0402 1601 1601 1402 1001 0401 0402  ................
-000043c0: 1401 0a01 1c01 0e01 0e01 1801 1603 0e01  ................
-000043d0: 0401 0602 0a01 0401 0cff 0804 0e01 0e01  ................
-000043e0: 1c02 0401 0402 1c01 0e01 0e01 0e02 0c01  ................
-000043f0: 0e01 0e01 0e01 0e01 0e01 0e01 0e01 0e01  ................
-00004400: 3c0b 0801 0a02 0a01 0c03 1001 0402 1401  <...............
-00004410: 0801 0402 1401 1601 1601 0c03 0e01 0401  ................
-00004420: 0605 0a01 0401 0cff 0803 0e01 0e01 1c02  ................
-00004430: 0401 0403 0aff 0403 0402 0e02 0c01 0cff  ................
-00004440: 0202 02fe 02ff 0c05 0201 02ff 0402 02fe  ................
-00004450: 0e04 10ff 0c05 1802 0c01 2e02 2201 22ff  ............".".
-00004460: 0202 0cfe 0e04 1a01 06ff 0202 1afe 0203  ................
-00004470: 0cfd 0e10 1602 1602 0c01 0e03 0c01 0eff  ................
-00004480: 0202 02fe 02ff 0c06 0c01 2e02 2201 22ff  ............".".
-00004490: 0202 0cfe 0e05 1a01 06ff 0202 1afe 0203  ................
-000044a0: 0cfd 0e0e 1201 08ff 0804 10ff 0c03 0e01  ................
-000044b0: 1201 0a03 1001 0e01 0e01 1201 0802 1402  ................
-000044c0: 0c01 0801 0c02 1401 1401 1401 1401 1401  ................
-000044d0: 1401 0c01 1401 1401 1401 1401 1409 1401  ................
-000044e0: 0a04 1401 1402 1401 0cfe 0e06 1401 0e02  ................
-000044f0: 0a01 1c01 0e01 0e02 2403 0e01 0e01 0e01  ........$.......
-00004500: 0e01 0e01 0e02 0c01 0e01 120c 72a9 0000  ............r...
-00004510: 0063 0200 0000 0000 0000 0000 0000 0b00  .c..............
-00004520: 0000 0600 0000 4300 0000 7320 0100 0074  ......C...s ...t
-00004530: 00a0 0164 017c 01a1 027d 0274 00a0 0174  ...d.|...}.t...t
-00004540: 027c 0083 0164 0217 0064 0266 0264 03a1  .|...d...d.f.d..
-00004550: 027d 0364 047d 0474 03a0 037c 00a1 017d  .}.d.}.t...|...}
-00004560: 0574 027c 0283 0164 046b 0490 0172 0674  .t.|...d.k...r.t
-00004570: 00a0 0174 027c 0083 0164 0217 0064 0266  ...t.|...d...d.f
-00004580: 0264 03a1 027d 0664 047d 0774 0464 0474  .d...}.d.}.t.d.t
-00004590: 027c 0283 0183 0244 005d 827d 087c 027c  .|.....D.].}.|.|
-000045a0: 0819 007c 037c 043c 007c 0464 0217 007d  ...|.|.<.|.d...}
-000045b0: 0474 00a0 057c 0564 0564 0585 0264 0266  .t...|.d.d...d.f
-000045c0: 0219 007c 027c 0819 006b 02a1 01a0 0674  ...|.|...k.....t
-000045d0: 07a1 017d 0974 0464 0474 027c 0983 0183  ...}.t.d.t.|....
-000045e0: 0244 005d 367d 0a7c 057c 097c 0a19 0064  .D.]6}.|.|.|...d
-000045f0: 0466 0219 007c 0376 0072 ce71 b47c 057c  .f...|.v.r.q.|.|
-00004600: 097c 0a19 0064 0466 0219 007c 067c 073c  .|...d.f...|.|.<
-00004610: 007c 0764 0217 007d 0771 b471 6a74 00a0  .|.d...}.q.qjt..
-00004620: 087c 06a1 017d 067c 067c 0664 046b 0519  .|...}.|.|.d.k..
-00004630: 007d 0271 3274 00a0 087c 03a1 017d 037c  .}.q2t...|...}.|
-00004640: 037c 0364 046b 0519 007d 037c 0353 0029  .|.d.k...}.|.S.)
-00004650: 067a 9f46 756e 6374 696f 6e73 2077 696c  .z.Functions wil
-00004660: 6c20 7265 7475 726e 2075 7073 7472 6561  l return upstrea
-00004670: 6d20 6964 7320 696e 206f 7574 2074 6168  m ids in out tah
-00004680: 7420 6472 6169 6e61 6765 0a20 2020 2020  t drainage.     
-00004690: 2020 2074 6f20 6f75 746c 6574 6964 0a20     to outletid. 
-000046a0: 2020 202d 2d2d 2d2d 2d2d 2d2d 2d0a 0a20     ----------.. 
-000046b0: 2020 204e 6f74 6573 0a20 2020 202d 2d2d     Notes.    ---
-000046c0: 2d2d 2d2d 0a0a 2020 2020 5265 7475 726e  ----..    Return
-000046d0: 733a 0a20 2020 202d 2d2d 2d2d 2d2d 0a20  s:.    -------. 
-000046e0: 2020 2020 2020 2053 6865 6469 640a 2020         Shedid.  
-000046f0: 2020 2902 7228 0000 0072 2800 0000 7228    ).r(...r(...r(
-00004700: 0000 006c fdff ffff ff67 ed10 5d00 7201  ...l.....g..].r.
-00004710: 0000 004e 2909 721a 0000 0072 7d00 0000  ...N).r....r}...
-00004720: 7215 0000 0072 1400 0000 7229 0000 00da  r....r....r)....
-00004730: 0861 7267 7768 6572 6572 1600 0000 722d  .argwherer....r-
-00004740: 0000 0072 2b00 0000 290b da03 6f75 74da  ...r+...)...out.
-00004750: 086f 7574 6c65 7469 645a 076f 7473 6865  .outletidZ.otshe
-00004760: 6473 5a06 5368 6564 6964 5a04 7073 6964  dsZ.ShedidZ.psid
-00004770: da04 726f 7574 5a07 6e6f 7574 7368 645a  ..routZ.noutshdZ
-00004780: 0770 6f73 6864 6964 7248 0000 005a 0469  .poshdidrH...Z.i
-00004790: 726f 7772 5e00 0000 7224 0000 0072 2400  rowr^...r$...r$.
-000047a0: 0000 7225 0000 0072 1700 0000 6104 0000  ..r%...r....a...
-000047b0: 732a 0000 0000 0c0c 0118 0104 010a 010e  s*..............
-000047c0: 0118 0104 0212 030c 0308 0124 0212 0214  ...........$....
-000047d0: 0102 0114 010c 010a 010e 010a 010c 0172  ...............r
-000047e0: 1700 0000 6303 0000 0000 0000 0000 0000  ....c...........
-000047f0: 000d 0000 0006 0000 0043 0000 0073 a601  .........C...s..
-00004800: 0000 7c02 6401 6402 6702 1900 a000 6403  ..|.d.d.g.....d.
-00004810: a101 6a01 7d03 7402 6404 7403 7c02 8301  ..j.}.t.d.t.|...
-00004820: 8302 4400 9001 5d78 7d04 7c02 6401 1900  ..D...]x}.|.d...
-00004830: 6a01 7c04 1900 7d05 7c02 6405 1900 6a01  j.|...}.|.d...j.
-00004840: 7c04 1900 7d06 7c00 6a04 7c00 6406 1900  |...}.|.j.|.d...
-00004850: 7c05 6b02 1900 a005 a100 7d07 7403 7406  |.k.......}.t.t.
-00004860: 7c03 7c05 8302 8301 7c02 6a04 7c02 6401  |.|.....|.j.|.d.
-00004870: 1900 7c05 6b02 6407 6602 3c00 7403 7c07  ..|.k.d.f.<.t.|.
-00004880: 8301 6404 6b01 7288 7122 7c07 6408 1900  ..d.k.r.q"|.d...
-00004890: 6409 6b02 7d08 7c07 6a04 7c08 640a 6602  d.k.}.|.j.|.d.f.
-000048a0: 1900 6a01 6404 1900 7d09 7c09 7c02 6a04  ..j.d...}.|.|.j.
-000048b0: 7c02 6401 1900 7c05 6b02 640b 6602 3c00  |.d...|.k.d.f.<.
-000048c0: 7c02 6402 1900 6a01 7c04 1900 7d0a 7c0a  |.d...j.|...}.|.
-000048d0: 6404 6b00 72d6 7122 7c01 6a04 7c01 6405  d.k.r.q"|.j.|.d.
-000048e0: 1900 7c06 6b02 1900 a005 a100 7d0b 7403  ..|.k.......}.t.
-000048f0: 7c0b 8301 640c 6b02 9001 722a 7c0a 640d  |...d.k...r*|.d.
-00004900: 6b03 9001 722a 7c0b 640a 1900 6a01 6404  k...r*|.d...j.d.
-00004910: 1900 7d0c 7c0c 7c00 6a04 7c00 640a 1900  ..}.|.|.j.|.d...
-00004920: 7c09 6b02 6408 6602 3c00 7122 7c0a 640d  |.k.d.f.<.q"|.d.
-00004930: 6b02 9001 724c 6409 7c00 6a04 7c00 640a  k...rLd.|.j.|.d.
-00004940: 1900 7c09 6b02 6408 6602 3c00 7122 7407  ..|.k.d.f.<.q"t.
-00004950: 640e 8301 0100 7407 640f 7c05 6410 7c0a  d.....t.d.|.d.|.
-00004960: 8304 0100 7407 7c0a 7c06 8302 0100 7407  ....t.|.|.....t.
-00004970: 7c0b 8301 0100 7407 7c09 8301 0100 7407  |.....t.|.....t.
-00004980: 7c01 6405 640a 6702 1900 8301 0100 7407  |.d.d.g.......t.
-00004990: 6411 8301 0100 7407 640e 8301 0100 7122  d.....t.d.....q"
-000049a0: 7c00 7c02 6602 5300 2912 612b 0400 004d  |.|.f.S.).a+...M
-000049b0: 6f64 6966 7920 6f75 746c 6574 2073 7562  odify outlet sub
-000049c0: 6261 7369 6e27 7320 646f 776e 7374 7265  basin's downstre
-000049d0: 616d 2073 7562 6261 7369 6e20 4944 2066  am subbasin ID f
-000049e0: 6f72 2065 6163 6820 7375 6272 6567 696f  or each subregio
-000049f0: 6e0a 2020 2020 5061 7261 6d65 7465 7273  n.    Parameters
-00004a00: 0a20 2020 202d 2d2d 2d2d 2d2d 2d2d 2d0a  .    ----------.
-00004a10: 2020 2020 416c 6c43 6174 696e 666f 2020      AllCatinfo  
-00004a20: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00004a30: 2020 2020 2020 3a20 6461 7461 6672 616d        : datafram
-00004a40: 650a 2020 2020 2020 2020 6974 2069 7320  e.        it is 
-00004a50: 6120 6461 7461 6672 616d 6520 6f66 2074  a dataframe of t
-00004a60: 6865 2061 7474 7269 6275 7465 2074 6162  he attribute tab
-00004a70: 6c65 2072 6561 6465 6420 6672 6f6d 2066  le readed from f
-00004a80: 696e 616c 6361 745f 696e 666f 0a20 2020  inalcat_info.   
-00004a90: 2020 2020 202e 7368 7020 6f72 2066 696e       .shp or fin
-00004aa0: 616c 7269 7670 6c79 5f69 6e66 6f2e 7368  alrivply_info.sh
-00004ab0: 700a 2020 2020 446f 776e 4361 7469 6e66  p.    DownCatinf
-00004ac0: 6f20 2020 2020 2020 2020 2020 2020 2020  o               
-00004ad0: 2020 2020 2020 2020 3a20 6461 7461 6672          : datafr
-00004ae0: 616d 650a 2020 2020 2020 2020 4974 2069  ame.        It i
-00004af0: 7320 6120 6461 7461 6672 616d 6520 696e  s a dataframe in
-00004b00: 636c 7564 6573 2074 776f 2063 6f6c 756d  cludes two colum
-00004b10: 6e73 3a0a 2020 2020 2020 2020 2753 7562  ns:.        'Sub
-00004b20: 5f52 6567 5f49 4427 3a20 7468 6520 7375  _Reg_ID': the su
-00004b30: 6272 6567 696f 6e20 6964 0a20 2020 2020  bregion id.     
-00004b40: 2020 2027 446f 775f 5375 625f 5265 675f     'Dow_Sub_Reg_
-00004b50: 4964 273a 2064 6f77 6e73 7472 6561 6d20  Id': downstream 
-00004b60: 7375 6262 6173 696e 2069 6420 6f66 2074  subbasin id of t
-00004b70: 6865 206f 7574 6c65 7420 7375 6262 6173  he outlet subbas
-00004b80: 696e 2069 6e0a 2020 2020 2020 2020 7468  in in.        th
-00004b90: 6973 2073 7562 7265 6769 6f6e 0a20 2020  is subregion.   
-00004ba0: 2053 7562 5f52 6567 696f 6e5f 696e 666f   Sub_Region_info
-00004bb0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00004bc0: 2020 203a 2064 6174 6166 7261 6d65 0a20     : dataframe. 
-00004bd0: 2020 2020 2020 2049 7420 6973 2061 2064         It is a d
-00004be0: 6174 6166 7261 6d65 2069 6e63 6c75 6465  ataframe include
-00004bf0: 7320 7375 6272 6567 696f 6e20 696e 666f  s subregion info
-00004c00: 726d 6174 696f 6e73 2c20 7769 7468 2066  rmations, with f
-00004c10: 6f6c 6c6f 7769 6e67 0a20 2020 2020 2020  ollowing.       
-00004c20: 2063 6f6c 756d 6e73 3a0a 2020 2020 2020   columns:.      
-00004c30: 2020 2753 7562 5f52 6567 5f49 4427 203a    'Sub_Reg_ID' :
-00004c40: 2074 6865 2073 7562 7265 6769 6f6e 2069   the subregion i
-00004c50: 640a 2020 2020 2020 2020 2744 6f77 5f53  d.        'Dow_S
-00004c60: 7562 5f52 6567 5f49 6427 3a20 7468 6520  ub_Reg_Id': the 
-00004c70: 646f 776e 7374 7265 616d 2073 7562 7265  downstream subre
-00004c80: 6769 6f6e 2069 640a 0a20 2020 204e 6f74  gion id..    Not
-00004c90: 6573 0a20 2020 202d 2d2d 2d2d 2d2d 0a0a  es.    -------..
-00004ca0: 2020 2020 5265 7475 726e 733a 0a20 2020      Returns:.   
-00004cb0: 202d 2d2d 2d2d 2d2d 0a20 2020 2020 2020   -------.       
-00004cc0: 2053 7562 5f52 6567 696f 6e5f 696e 666f   Sub_Region_info
-00004cd0: 2020 2020 2020 3a20 6461 7461 6672 616d        : datafram
-00004ce0: 650a 2020 2020 2020 2020 2020 2020 416e  e.            An
-00004cf0: 206e 6577 2063 6f6c 756d 6e73 2069 6e64   new columns ind
-00004d00: 6963 6174 6520 7468 6520 6f75 746c 6574  icate the outlet
-00004d10: 2073 7562 6261 7369 6e20 6964 206f 6620   subbasin id of 
-00004d20: 7468 6520 7375 6220 7265 6769 6f6e 0a20  the sub region. 
-00004d30: 2020 2020 2020 2020 2020 2077 696c 6c20             will 
-00004d40: 6265 2061 6464 6564 0a20 2020 2020 2020  be added.       
-00004d50: 2041 6c6c 4361 7469 6e66 6f20 2020 2020   AllCatinfo     
-00004d60: 2020 2020 2020 3a20 6461 7461 6672 616d        : datafram
-00004d70: 650a 2020 2020 2020 2020 2020 2020 446f  e.            Do
-00004d80: 776e 7374 7265 616d 2073 7562 6261 7369  wnstream subbasi
-00004d90: 6e20 4944 206f 6620 6561 6368 2073 7562  n ID of each sub
-00004da0: 7265 6769 6f6e 2773 206f 7574 6c65 7420  region's outlet 
-00004db0: 7375 6262 6173 696e 2077 696c 6c0a 2020  subbasin will.  
-00004dc0: 2020 2020 2020 2020 2020 6265 2075 7064            be upd
-00004dd0: 6174 6564 2e0a 2020 2020 da0a 5375 625f  ated..    ..Sub_
-00004de0: 5265 675f 4944 da0e 446f 775f 5375 625f  Reg_ID..Dow_Sub_
-00004df0: 5265 675f 4964 7263 0000 0072 0100 0000  Reg_Idrc...r....
-00004e00: da07 494c 7074 5f49 44da 0952 6567 696f  ..ILpt_ID..Regio
-00004e10: 6e5f 4944 da0e 4e5f 5570 5f53 7562 5265  n_ID..N_Up_SubRe
-00004e20: 6769 6f6e 720d 0000 0072 6b00 0000 7206  gionr....rk...r.
-00004e30: 0000 00da 0c4f 7574 6c65 745f 5375 6249  .....Outlet_SubI
-00004e40: 6472 2800 0000 e97f 3801 007a 3223 2323  dr(.....8..z2###
-00004e50: 2323 2323 2323 2323 2323 2323 2323 2323  ################
-00004e60: 2323 2323 2323 2323 2323 2323 2323 2323  ################
-00004e70: 2323 2323 2323 2323 2323 2323 2323 237a  ###############z
-00004e80: 0c53 7562 7265 6769 6f6e 203a 207a 0720  .Subregion : z. 
-00004e90: 2020 546f 2020 7a1a 4e65 6564 2062 6520    To  z.Need be 
-00004ea0: 6d61 6e75 616c 6c79 2063 6f6e 6e65 6374  manually connect
-00004eb0: 6564 2908 7216 0000 0072 1300 0000 7229  ed).r....r....r)
-00004ec0: 0000 0072 1500 0000 7219 0000 0072 1400  ...r....r....r..
-00004ed0: 0000 7217 0000 0072 7500 0000 290d da0a  ..r....ru...)...
-00004ee0: 416c 6c43 6174 696e 666f 5a0b 446f 776e  AllCatinfoZ.Down
-00004ef0: 4361 7469 6e66 6fda 0f53 7562 5f52 6567  Catinfo..Sub_Reg
-00004f00: 696f 6e5f 696e 666f 7277 0000 0072 4800  ion_inforw...rH.
-00004f10: 0000 5a0a 6973 7562 7265 6769 6f6e 72bf  ..Z.isubregionr.
-00004f20: 0000 005a 1353 7562 5f52 6567 696f 6e5f  ...Z.Sub_Region_
-00004f30: 6361 745f 696e 666f 5a0b 6f75 746c 6574  cat_infoZ.outlet
-00004f40: 5f6d 6173 6b5a 1169 5265 675f 4f75 746c  _maskZ.iReg_Outl
-00004f50: 6574 5f53 7562 6964 5a11 446f 775f 5375  et_SubidZ.Dow_Su
-00004f60: 625f 5265 6769 6f6e 5f69 64da 0d44 6f77  b_Region_id..Dow
-00004f70: 6e5f 5375 625f 696e 666f 5a09 446f 776e  n_Sub_infoZ.Down
-00004f80: 5375 6269 6472 2400 0000 7224 0000 0072  Subidr$...r$...r
-00004f90: 2500 0000 da22 436f 6e6e 6563 745f 5375  %...."Connect_Su
-00004fa0: 6252 6567 696f 6e5f 5570 6461 7465 5f44  bRegion_Update_D
-00004fb0: 6f77 6e53 7562 4964 8b04 0000 7352 0000  ownSubId....sR..
-00004fc0: 0000 2312 ff02 0314 030e 020e 0204 010a  ..#.............
-00004fd0: ff08 060c fe04 010e ff02 050c 0102 030c  ................
-00004fe0: 0114 0402 fe04 010e ff02 040e 0408 0102  ................
-00004ff0: 0316 0218 010e 0302 fe04 010e ff04 060a  ................
-00005000: 0118 0208 010e 010a 0108 0108 0110 0108  ................
-00005010: 010a 0172 c700 0000 6304 0000 0000 0000  ...r....c.......
-00005020: 0000 0000 0019 0000 000a 0000 0043 0000  .............C..
-00005030: 0073 0605 0000 7c01 7c01 6401 1900 6402  .s....|.|.d...d.
-00005040: 6b02 1900 6403 1900 6a00 7d04 7401 a002  k...d...j.}.t...
-00005050: 7c04 a101 7d04 7c04 a003 a100 7d04 7404  |...}.|.....}.t.
-00005060: 7c00 6a05 7c00 6404 1900 6405 6b02 1900  |.j.|.d...d.k...
-00005070: 8301 6402 6b04 7264 7406 6406 8301 0100  ..d.k.rdt.d.....
-00005080: 7406 7c00 6a05 7c00 6404 1900 6405 6b02  t.|.j.|.d...d.k.
-00005090: 1900 8301 0100 7c00 5300 7404 7c00 6a05  ......|.S.t.|.j.
-000050a0: 7c00 6404 1900 6405 6b02 1900 8301 6407  |.d...d.k.....d.
-000050b0: 6b02 728a 7406 6408 8301 0100 7c00 5300  k.r.t.d.....|.S.
-000050c0: 7c00 6a05 7c00 6404 1900 6405 6b02 1900  |.j.|.d...d.k...
-000050d0: 6409 1900 6a00 6407 1900 a007 7408 a101  d...j.d.....t...
-000050e0: 7d05 640a 7d06 7409 6407 7404 7c01 8301  }.d.}.t.d.t.|...
-000050f0: 8302 4400 5d94 7d07 7c01 640b 1900 6a00  ..D.].}.|.d...j.
-00005100: 7c07 1900 7d08 7c06 7c00 6a05 7c00 6409  |...}.|.|.j.|.d.
-00005110: 1900 7c08 6b02 1900 640c 1900 6a00 6407  ..|.k...d...j.d.
-00005120: 1900 1700 7d06 7406 640d 7c01 6403 1900  ....}.t.d.|.d...
-00005130: 6a00 7c07 1900 8302 0100 7406 640e 7c00  j.|.......t.d.|.
-00005140: 6a05 7c00 6409 1900 7c08 6b02 1900 640c  j.|.d...|.k...d.
-00005150: 1900 6a00 6407 1900 8302 0100 7406 640f  ..j.d.......t.d.
-00005160: 740a 7c00 6a05 7c00 6410 1900 7c01 6403  t.|.j.|.d...|.d.
-00005170: 1900 6a00 7c07 1900 6b02 1900 6411 1900  ..j.|...k...d...
-00005180: 6a00 8301 8302 0100 71be 6402 7d09 7404  j.......q.d.}.t.
-00005190: 7c04 8301 6407 6b04 9004 72b6 7406 6412  |...d.k...r.t.d.
-000051a0: 7c09 8302 0100 7406 7c04 8301 0100 740b  |.....t.|.....t.
-000051b0: a00b 7c04 a101 7d0a 6700 7d04 7409 6407  ..|...}.g.}.t.d.
-000051c0: 7404 7c0a 8301 8302 4400 9003 5d06 7d07  t.|.....D...].}.
-000051d0: 7c0a 7c07 1900 7d0b 7c0b 6413 6b02 9001  |.|...}.|.d.k...
-000051e0: 72b0 9001 7194 7c01 7c01 6403 1900 7c0b  r...q.|.|.d...|.
-000051f0: 6b02 1900 6414 1900 6a00 6407 1900 7d0c  k...d...j.d...}.
-00005200: 7c04 a00c 7c0c a101 0100 7c01 7c01 6403  |...|.....|.|.d.
-00005210: 1900 7c0b 6b02 1900 640b 1900 6a00 6407  ..|.k...d...j.d.
-00005220: 1900 7d08 7c00 6a05 7c00 6409 1900 7c08  ..}.|.j.|.d...|.
-00005230: 6b02 1900 a00b a100 7d0d 7c0d 6404 1900  k.......}.|.d...
-00005240: 6a00 6407 1900 7d0e 7404 7c00 6a05 7c00  j.d...}.t.|.j.|.
-00005250: 6409 1900 7c0e 6b02 1900 8301 6407 6b01  d...|.k.....d.k.
-00005260: 9002 726c 7408 7c0b 8301 7408 7c05 8301  ..rlt.|...t.|...
-00005270: 6b03 9001 7294 7406 6415 7c0b 8302 0100  k...r.t.d.|.....
-00005280: 7406 6416 7c08 6417 7c0e 7c05 7408 7c0b  t.d.|.d.|.|.t.|.
-00005290: 8301 7408 7c05 8301 6b03 8306 0100 9001  ..t.|...k.......
-000052a0: 7194 7c00 6a05 7c00 6409 1900 7c0e 6b02  q.|.j.|.d...|.k.
-000052b0: 1900 6410 1900 6a00 6407 1900 7d0f 7406  ..d...j.d...}.t.
-000052c0: 6415 7c0b 7c0f 7c0c 7c0e 8305 0100 7c0f  d.|.|.|.|.....|.
-000052d0: 7c0c 6b03 9002 72b4 7406 6415 7c0b 6418  |.k...r.t.d.|.d.
-000052e0: 7c0c 8304 0100 9001 7194 7c0f 7c0c 6b02  |.......q.|.|.k.
-000052f0: 9001 7294 7c0e 7d10 7406 6415 7c0b 7c0f  ..r.|.}.t.d.|.|.
-00005300: 7c0c 7c0e 7c10 8306 0100 7c00 6a05 7c00  |.|.|.....|.j.|.
-00005310: 6409 1900 7c10 6b02 1900 a00b a100 7d11  d...|.k.......}.
-00005320: 7c00 6a05 7c00 6404 1900 7c10 6b02 1900  |.j.|.d...|.k...
-00005330: a00b a100 7d12 7c11 6411 1900 6a00 6407  ....}.|.d...j.d.
-00005340: 1900 740a 7c12 640c 1900 6a00 8301 1700  ..t.|.d...j.....
-00005350: 7d13 7c12 6419 1900 6a00 7d14 740d 7c14  }.|.d...j.}.t.|.
-00005360: 8301 7d15 7401 a00a 7c14 7c15 6b02 a101  ..}.t...|.|.k...
-00005370: 641a 6b05 9003 724c 7c15 6402 1700 7d16  d.k...rL|.d...}.
-00005380: 6e04 7c15 7d16 7c16 7c00 6a05 7c00 6409  n.|.}.|.|.j.|.d.
-00005390: 1900 7c10 6b02 6419 6602 3c00 7c13 7c00  ..|.k.d.f.<.|.|.
-000053a0: 6a05 7c00 6409 1900 7c10 6b02 640c 6602  j.|.d...|.k.d.f.
-000053b0: 3c00 7c00 7c00 6409 1900 7c10 6b02 1900  <.|.|.d...|.k...
-000053c0: 641b 1900 6a00 6407 1900 6407 6b04 9004  d...j.d...d.k...
-000053d0: 7212 7c00 7c00 6409 1900 7c10 6b02 1900  r.|.|.d...|.k...
-000053e0: 641b 1900 6a00 6407 1900 7d17 7c00 7c00  d...j.d...}.|.|.
-000053f0: 6409 1900 7c10 6b02 1900 640c 1900 6a00  d...|.k...d...j.
-00005400: 6407 1900 641c 1b00 641c 1b00 7d18 7c17  d...d...d...}.|.
-00005410: 6407 6b04 9004 7212 7c18 7c17 1b00 7c00  d.k...r.|.|...|.
-00005420: 6a05 7c00 6409 1900 7c10 6b02 641d 6602  j.|.d...|.k.d.f.
-00005430: 3c00 6402 7c00 6a05 7c00 6409 1900 7c10  <.d.|.j.|.d...|.
-00005440: 6b02 641e 6602 3c00 7c11 6404 1900 6a00  k.d.f.<.|.d...j.
-00005450: 6407 1900 7d0e 7404 7c00 6a05 7c00 6409  d...}.t.|.j.|.d.
-00005460: 1900 7c0e 6b02 1900 8301 6407 6b01 9004  ..|.k.....d.k...
-00005470: 727a 7408 7c10 8301 7408 7c05 8301 6b03  rzt.|...t.|...k.
-00005480: 9004 729a 7406 6415 7c0c 8302 0100 7406  ..r.t.d.|.....t.
-00005490: 6416 7c10 6417 7c0e 7c05 7408 7c10 8301  d.|.d.|.|.t.|...
-000054a0: 7408 7c05 8301 6b03 8306 0100 9001 7194  t.|...k.......q.
-000054b0: 7c00 6a05 7c00 6409 1900 7c0e 6b02 1900  |.j.|.d...|.k...
-000054c0: 6410 1900 6a00 6407 1900 7d0f 9002 71b4  d...j.d...}...q.
-000054d0: 9001 7194 740e 740f 7c04 8301 8301 7d04  ..q.t.t.|.....}.
-000054e0: 7c09 6402 1700 7d09 9001 7158 7406 641f  |.d...}...qXt.d.
-000054f0: 8301 0100 7406 6420 740a 7c00 6411 1900  ....t.d t.|.d...
-00005500: 6a00 8301 8302 0100 7406 6421 7c00 6a05  j.......t.d!|.j.
-00005510: 7c00 6409 1900 7408 7c05 8301 6b02 1900  |.d...t.|...k...
-00005520: 640c 1900 6a00 6407 1900 8302 0100 7406  d...j.d.......t.
-00005530: 6422 7c06 8302 0100 7c00 5300 2923 6115  d"|.....|.S.)#a.
-00005540: 0300 0055 7064 6174 6520 4472 6169 6e61  ...Update Draina
-00005550: 6765 2061 7265 612c 2073 7472 6168 6c65  ge area, strahle
-00005560: 7220 6f72 6465 7220 6f66 2073 7562 6261  r order of subba
-00005570: 696e 730a 0a20 2020 2055 7064 6174 6520  ins..    Update 
-00005580: 6472 6169 6e61 6765 2061 7265 6120 616e  drainage area an
-00005590: 6420 7374 7261 686c 6572 206f 7264 6572  d strahler order
-000055a0: 2066 6f72 2063 6f6d 6269 6e65 6420 726f   for combined ro
-000055b0: 7574 696e 6720 7072 6f64 7563 740a 2020  uting product.  
-000055c0: 2020 6f66 2065 6163 6820 7375 6272 6567    of each subreg
-000055d0: 696f 6e73 0a20 2020 2050 6172 616d 6574  ions.    Paramet
-000055e0: 6572 730a 2020 2020 2d2d 2d2d 2d2d 2d2d  ers.    --------
-000055f0: 2d2d 0a20 2020 2041 6c6c 4361 7469 6e66  --.    AllCatinf
-00005600: 6f20 2020 2020 2020 2020 2020 2020 2020  o               
-00005610: 2020 2020 2020 2020 203a 2064 6174 6166           : dataf
-00005620: 7261 6d65 0a20 2020 2020 2020 2069 7420  rame.        it 
-00005630: 6973 2061 2064 6174 6166 7261 6d65 206f  is a dataframe o
-00005640: 6620 7468 6520 6174 7472 6962 7574 6520  f the attribute 
-00005650: 7461 626c 6520 7265 6164 6564 2066 726f  table readed fro
-00005660: 6d20 6669 6e61 6c63 6174 5f69 6e66 6f0a  m finalcat_info.
-00005670: 2020 2020 2020 2020 2e73 6870 206f 7220          .shp or 
-00005680: 6669 6e61 6c72 6976 706c 795f 696e 666f  finalrivply_info
-00005690: 2e73 6870 0a20 2020 2053 7562 5f52 6567  .shp.    Sub_Reg
-000056a0: 696f 6e5f 696e 666f 2020 2020 2020 2020  ion_info        
-000056b0: 2020 2020 2020 2020 2020 203a 2064 6174             : dat
-000056c0: 6166 7261 6d65 0a20 2020 2020 2020 2049  aframe.        I
-000056d0: 7420 6973 2061 2064 6174 6166 7261 6d65  t is a dataframe
-000056e0: 2069 6e63 6c75 6465 7320 7375 6272 6567   includes subreg
-000056f0: 696f 6e20 696e 666f 726d 6174 696f 6e73  ion informations
-00005700: 2c20 7769 7468 2066 6f6c 6c6f 7769 6e67  , with following
-00005710: 0a20 2020 2020 2020 2063 6f6c 756d 6e73  .        columns
-00005720: 3a0a 2020 2020 2020 2020 2753 7562 5f52  :.        'Sub_R
-00005730: 6567 5f49 4427 203a 2074 6865 2073 7562  eg_ID' : the sub
-00005740: 7265 6769 6f6e 2069 640a 2020 2020 2020  region id.      
-00005750: 2020 2744 6f77 5f53 7562 5f52 6567 5f49    'Dow_Sub_Reg_I
-00005760: 6427 3a20 7468 6520 646f 776e 7374 7265  d': the downstre
-00005770: 616d 2073 7562 7265 6769 6f6e 2069 640a  am subregion id.
-00005780: 0a20 2020 204e 6f74 6573 0a20 2020 202d  .    Notes.    -
-00005790: 2d2d 2d2d 2d2d 0a0a 2020 2020 5265 7475  ------..    Retu
-000057a0: 726e 733a 0a20 2020 202d 2d2d 2d2d 2d2d  rns:.    -------
-000057b0: 0a20 2020 2041 6c6c 4361 7469 6e66 6f20  .    AllCatinfo 
-000057c0: 2020 2020 2020 2020 2020 3a20 6461 7461            : data
-000057d0: 6672 616d 650a 2020 2020 2020 2020 446f  frame.        Do
-000057e0: 776e 7374 7265 616d 2044 4120 616e 6420  wnstream DA and 
-000057f0: 7374 7261 686c 6572 206f 7264 6572 206f  strahler order o
-00005800: 6620 6561 6368 2073 7562 7265 6769 6f6e  f each subregion
-00005810: 2061 6c6f 6e67 2074 6865 2066 6c6f 770a   along the flow.
-00005820: 2020 2020 2020 2020 7061 7468 7761 7920          pathway 
-00005830: 6265 7477 6565 6e20 7375 6272 6567 696f  between subregio
-00005840: 6e73 2077 696c 6c20 6265 2075 7064 6174  ns will be updat
-00005850: 6564 2e0a 2020 2020 72c1 0000 0072 2800  ed..    r....r(.
-00005860: 0000 72bd 0000 0072 0d00 0000 726b 0000  ..r....r....rk..
-00005870: 007a 1f57 6174 6865 7273 6564 2068 6173  .z.Wathersed has
-00005880: 206d 756c 7469 706c 6520 6f75 746c 6574   multiple outlet
-00005890: 2020 7201 0000 007a 1757 6174 6572 7368    r....z.Watersh
-000058a0: 6564 2068 6173 206e 6f20 6f75 746c 6574  ed has no outlet
-000058b0: 7206 0000 0072 6700 0000 72c2 0000 0072  r....rg...r....r
-000058c0: 7900 0000 7a26 2323 2323 2323 4172 6561  y...z&######Area
-000058d0: 2061 6e64 2044 4120 6368 6563 6b20 666f   and DA check fo
-000058e0: 7220 7375 6272 6567 696f 6e20 7a21 4441  r subregion z!DA
-000058f0: 2061 7420 7468 6520 7375 6272 6567 696f   at the subregio
-00005900: 6e20 6f75 746c 6574 2069 7320 2020 207a  n outlet is    z
-00005910: 2154 6f74 616c 2073 7562 7265 6769 6f6e  !Total subregion
-00005920: 2061 7265 6120 6973 2020 2020 2020 2020   area is        
-00005930: 2020 72c0 0000 0072 8200 0000 7a06 6c6f    r....r....z.lo
-00005940: 6f70 2020 72c3 0000 0072 be00 0000 7a0d  op  r....r....z.
-00005950: 5375 6272 6567 696f 6e3a 2020 207a 0953  Subregion:   z.S
-00005960: 7562 4964 2069 7320 7a0f 2044 6f77 6e53  ubId is z. DownS
-00005970: 7562 4964 2069 7320 207a 1c20 2064 6964  ubId is  z.  did
-00005980: 206e 6f74 2063 6f6e 6e65 6374 6564 2077   not connected w
-00005990: 6974 6820 2020 2072 6900 0000 7265 0000  ith    ri...re..
-000059a0: 0072 b300 0000 72b4 0000 0072 b500 0000  .r....r....r....
-000059b0: 5a0a 5573 655f 7265 6769 6f6e 7a14 4368  Z.Use_regionz.Ch
-000059c0: 6563 6b20 6472 6169 6e61 6765 2061 7265  eck drainage are
-000059d0: 613a 7a21 546f 7461 6c20 6261 7369 6e20  a:z!Total basin 
-000059e0: 6172 6561 2069 7320 2020 2020 2020 2020  area is         
-000059f0: 2020 2020 207a 2144 4120 6f66 2074 6865       z!DA of the
-00005a00: 2077 6174 6572 7365 6864 206f 7574 6c65   watersehd outle
-00005a10: 7420 6973 2020 2020 7a21 546f 7461 6c20  t is    z!Total 
-00005a20: 4441 206f 6620 6561 6368 2073 7562 7265  DA of each subre
-00005a30: 6769 6f6e 2020 2020 2020 2029 1072 1300  gion       ).r..
-00005a40: 0000 721a 0000 0072 2b00 0000 da06 746f  ..r....r+.....to
-00005a50: 6c69 7374 7215 0000 0072 1900 0000 7275  listr....r....ru
-00005a60: 0000 0072 1600 0000 722d 0000 0072 2900  ...r....r-...r).
-00005a70: 0000 723f 0000 0072 1400 0000 724e 0000  ..r?...r....rN..
-00005a80: 0072 7400 0000 7254 0000 00da 0373 6574  .rt...rT.....set
-00005a90: 2919 72c4 0000 0072 c500 0000 7261 0000  ).r....r....ra..
-00005aa0: 00da 0163 5a0e 5375 6272 6567 696f 6e5f  ...cZ.Subregion_
-00005ab0: 6c69 7374 5a14 5761 7465 7273 6865 646f  listZ.Watershedo
-00005ac0: 7574 6c65 7473 7562 6964 5a12 546f 7461  utletsubidZ.Tota
-00005ad0: 6c5f 4441 5f53 7562 7265 6769 6f6e 7248  l_DA_SubregionrH
-00005ae0: 0000 005a 114f 7574 6c65 7473 7562 6964  ...Z.Outletsubid
-00005af0: 5f63 7375 6272 5a05 696c 6f6f 705a 1163  _csubrZ.iloopZ.c
-00005b00: 7572 7265 6e74 5f6c 6f6f 705f 6c69 7374  urrent_loop_list
-00005b10: 5a09 635f 7375 6272 5f69 645a 0964 5f73  Z.c_subr_idZ.d_s
-00005b20: 7562 725f 6964 5a0e 4f75 746c 6574 7375  ubr_idZ.Outletsu
-00005b30: 625f 696e 666f da09 646f 776e 7375 6269  b_info..downsubi
-00005b40: 645a 0e64 6f77 6e73 7562 5f72 6567 5f69  dZ.downsub_reg_i
-00005b50: 64da 0663 7375 6269 645a 0a43 5f73 7562  d..csubidZ.C_sub
-00005b60: 5f69 6e66 6f5a 0e55 7070 6572 5f73 7562  _infoZ.Upper_sub
-00005b70: 5f69 6e66 6f5a 054e 6577 4441 5a09 5374  _infoZ.NewDAZ.St
-00005b80: 7261 686c 6572 735a 0b6d 6178 5374 7261  rahlersZ.maxStra
-00005b90: 686c 6572 5a0b 6e65 7753 7472 6168 6c65  hlerZ.newStrahle
-00005ba0: 725a 0664 615f 6f62 735a 0664 615f 7369  rZ.da_obsZ.da_si
-00005bb0: 6d72 2400 0000 7224 0000 0072 2500 0000  mr$...r$...r%...
-00005bc0: da26 5570 6461 7465 5f44 415f 5374 7261  .&Update_DA_Stra
-00005bd0: 686c 6572 5f46 6f72 5f43 6f6d 6269 6e65  hler_For_Combine
-00005be0: 645f 5265 7375 6c74 eb04 0000 731e 0100  d_Result....s...
-00005bf0: 0000 1a0e 0102 ff06 030a 0108 051a 0108  ................
-00005c00: 0116 0104 011a 0108 0104 0320 ff02 0504  ........... ....
-00005c10: 0112 010e 0202 011a ff02 ff02 0402 0102  ................
-00005c20: 010c fe04 0402 0102 011a fe04 0402 0102  ................
-00005c30: 0102 0104 0114 ff02 0202 fe04 ff02 fe06  ................
-00005c40: 0904 010e 010a 0108 010a 0104 0214 0208  ................
-00005c50: 020a 0104 020e 0102 ff04 0202 fe04 040a  ................
-00005c60: 0302 010a ff02 0202 fe04 0202 fe04 0404  ................
-00005c70: 010a ff08 040e 031c 0112 010a 0102 0102  ................
-00005c80: 0102 0102 0102 0102 010e fa04 0804 0210  ................
-00005c90: 0102 ff04 0202 fe04 0410 020a 0102 0102  ................
-00005ca0: 0102 0102 0102 fc04 0604 020a 0104 0112  ................
-00005cb0: 0216 0216 040e 0108 ff06 060a 0108 0114  ................
-00005cc0: 010a 0204 0216 0116 0220 011a 0122 010a  ......... ..."..
-00005cd0: 011a 0116 150e 031c 0112 010a 0102 0102  ................
-00005ce0: 0102 0102 0102 0102 010e fa04 0804 0210  ................
-00005cf0: 0102 ff04 0202 fe0c 050c 010c 0308 0114  ................
-00005d00: 0102 0102 011a 0102 ff02 fe04 060a 0172  ...............r
-00005d10: cd00 0000 6301 0000 0000 0000 0000 0000  ....c...........
-00005d20: 0012 0000 0008 0000 0043 0000 0073 e002  .........C...s..
-00005d30: 0000 6401 7d01 6402 7d02 6403 7d03 7400  ..d.}.d.}.d.}.t.
-00005d40: 7c00 7c01 1900 6a01 8301 7d04 7402 7c00  |.|...j...}.t.|.
-00005d50: 8301 7d05 6404 7d06 7403 a004 7c05 6405  ..}.d.}.t...|.d.
-00005d60: 1700 7403 6a05 a102 7d07 7403 a004 7c05  ..t.j...}.t...|.
-00005d70: 6405 1700 7403 6a05 a102 7d08 7406 6406  d...t.j...}.t.d.
-00005d80: 7402 7c00 8301 8302 4400 9001 5d6a 7d09  t.|.....D...]j}.
-00005d90: 7c00 7c01 1900 6a01 7c09 1900 7d0a 7c00  |.|...j.|...}.|.
-00005da0: 7c03 1900 6a01 7c09 1900 7d0b 7c00 7c02  |...j.|...}.|.|.
-00005db0: 1900 6a01 7c09 1900 7d0c 7a0c 7407 7c0a  ..j.|...}.z.t.|.
-00005dc0: 8301 7d0d 5700 6e1e 0100 0100 0100 6407  ..}.W.n.......d.
-00005dd0: 7d0d 6407 7c00 6a08 7c09 7c01 6602 3c00  }.d.|.j.|.|.f.<.
-00005de0: 5900 6e02 3000 7a0c 7407 7c0b 8301 7d0e  Y.n.0.z.t.|...}.
-00005df0: 5700 6e1e 0100 0100 0100 6407 7d0e 6407  W.n.......d.}.d.
-00005e00: 7c00 6a08 7c09 7c03 6602 3c00 5900 6e02  |.j.|.|.f.<.Y.n.
-00005e10: 3000 7a0c 7407 7c0c 8301 7d0f 5700 6e1e  0.z.t.|...}.W.n.
-00005e20: 0100 0100 0100 6407 7d0f 6407 7c00 6a08  ......d.}.d.|.j.
-00005e30: 7c09 7c02 6602 3c00 5900 6e02 3000 7c0d  |.|.f.<.Y.n.0.|.
-00005e40: 6406 6b00 9001 7218 7158 7c0f 6406 6b01  d.k...r.qX|.d.k.
-00005e50: 9001 7234 7c0d 7d10 6407 7c00 6a08 7c09  ..r4|.}.d.|.j.|.
-00005e60: 6408 6602 3c00 7c0f 6406 6b04 9001 727a  d.f.<.|.d.k...rz
-00005e70: 7c0e 7c0f 6b02 9001 7264 7c0d 7c04 1700  |.|.k...rd|.|...
-00005e80: 6409 1700 7d10 6404 7c00 6a08 7c09 6408  d...}.d.|.j.|.d.
-00005e90: 6602 3c00 6e16 7407 7c0d 8301 7d10 6407  f.<.n.t.|...}.d.
-00005ea0: 7c00 6a08 7c09 6408 6602 3c00 7c10 7c08  |.j.|.d.f.<.|.|.
-00005eb0: 7601 9001 72a4 7c06 7c00 6a08 7c09 640a  v...r.|.|.j.|.d.
-00005ec0: 6602 3c00 7c10 7c08 7c06 3c00 7c06 6404  f.<.|.|.|.<.|.d.
-00005ed0: 1700 7d06 7158 7409 7403 a00a 7c08 7c10  ..}.qXt.t...|.|.
-00005ee0: 6b02 a101 6406 1900 8301 7c00 6a08 7c09  k...d.....|.j.|.
-00005ef0: 640a 6602 3c00 7158 7406 6406 7402 7c00  d.f.<.qXt.d.t.|.
-00005f00: 8301 8302 4400 9001 5d04 7d09 7c00 7c01  ....D...].}.|.|.
-00005f10: 1900 6a01 7c09 1900 7d0d 7c00 7c03 1900  ..j.|...}.|.|...
-00005f20: 6a01 7c09 1900 7d0e 7c00 7c02 1900 6a01  j.|...}.|.|...j.
-00005f30: 7c09 1900 7d0f 7c0d 6406 6b04 9002 7212  |...}.|.d.k...r.
-00005f40: 9001 71d4 7c0e 6406 6b01 9002 723e 740b  ..q.|.d.k...r>t.
-00005f50: 640b 8301 0100 740b 7c00 6a08 7c09 640c  d.....t.|.j.|.d.
-00005f60: 640c 8502 6602 1900 8301 0100 9001 71d4  d...f.........q.
-00005f70: 7c00 6a08 7c00 7c03 1900 7c0e 6b02 7c00  |.j.|.|...|.k.|.
-00005f80: 6408 1900 6406 6b04 4000 1900 7d11 7402  d...d.k.@...}.t.
-00005f90: 7c11 8301 6406 6b01 9002 7278 740b 640d  |...d.k...rxt.d.
-00005fa0: 7c0e 8302 0100 9001 71d4 7c11 7c01 1900  |.......q.|.|...
-00005fb0: 6a01 6406 1900 7c00 6a08 7c09 7c01 6602  j.d...|.j.|.|.f.
-00005fc0: 3c00 7c11 6408 1900 6a01 6406 1900 7c00  <.|.d...j.d...|.
-00005fd0: 6a08 7c09 6408 6602 3c00 7c11 640a 1900  j.|.d.f.<.|.d...
-00005fe0: 6a01 6406 1900 7c00 6a08 7c09 640a 6602  j.d...|.j.|.d.f.
-00005ff0: 3c00 7c11 7c02 1900 6a01 6406 1900 7c00  <.|.|...j.d...|.
-00006000: 6a08 7c09 7c02 6602 3c00 9001 71d4 7c00  j.|.|.f.<...q.|.
-00006010: 5300 290e 7aa1 4675 6e63 7469 6f6e 2074  S.).z.Function t
-00006020: 6f20 6465 7465 726d 696e 2068 7275 6964  o determin hruid
-00006030: 2061 6674 6572 2063 6f6d 6269 6e65 206c   after combine l
-00006040: 616b 6520 706f 6c79 676f 6e0a 2020 2020  ake polygon.    
-00006050: 616e 6420 7375 6262 6173 696e 2070 6f6c  and subbasin pol
-00006060: 7967 6f6e 0a20 2020 202d 2d2d 2d2d 2d2d  ygon.    -------
-00006070: 2d2d 2d0a 0a20 2020 204e 6f74 6573 0a20  ---..    Notes. 
-00006080: 2020 202d 2d2d 2d2d 2d2d 0a0a 2020 2020     -------..    
-00006090: 5265 7475 726e 733a 0a20 2020 202d 2d2d  Returns:.    ---
-000060a0: 2d2d 2d2d 0a20 2020 2020 2020 204e 6f6e  ----.        Non
-000060b0: 652c 0a20 2020 2072 0600 0000 7284 0000  e,.    r....r...
-000060c0: 00da 0848 796c 616b 5f69 6472 2800 0000  ...Hylak_idr(...
-000060d0: 727b 0000 0072 0100 0000 726b 0000 0072  r{...r....rk...r
-000060e0: 4d00 0000 e90a 0000 00da 0a48 5255 4c61  M..........HRULa
-000060f0: 6b65 5f49 447a 1a6c 616b 6520 6861 7320  ke_IDz.lake has 
-00006100: 756e 6578 7065 6374 6564 2068 6f6c 6573  unexpected holes
-00006110: 204e 7a16 4c61 6b65 6964 2064 6f20 6e6f   Nz.Lakeid do no
-00006120: 7420 6578 6973 7420 2020 290c 7274 0000  t exist   ).rt..
-00006130: 0072 1300 0000 7215 0000 0072 1a00 0000  .r....r....r....
-00006140: 727d 0000 00da 036e 616e 7229 0000 0072  r}.....nanr)...r
-00006150: 6300 0000 7219 0000 0072 2d00 0000 72b9  c...r....r-...r.
-00006160: 0000 0072 7500 0000 2912 5a0f 4174 7472  ...ru...).Z.Attr
-00006170: 6962 7574 655f 5461 626c 65da 0653 7562  ibute_Table..Sub
-00006180: 5f49 44da 0b53 7562 5f4c 616b 655f 4944  _ID..Sub_Lake_ID
-00006190: da07 4c61 6b65 5f49 645a 0f6d 6178 5f73  ..Lake_IdZ.max_s
-000061a0: 7562 6261 7369 6e5f 6964 5a0e 4e5f 6e65  ubbasin_idZ.N_ne
-000061b0: 775f 6665 6174 7572 6573 5a09 6e65 775f  w_featuresZ.new_
-000061c0: 6872 7569 645a 0e6e 6577 5f68 7275 6964  hruidZ.new_hruid
-000061d0: 5f6c 6973 745a 116f 6c64 5f6e 6577 6872  _listZ.old_newhr
-000061e0: 7569 645f 6c69 7374 7248 0000 005a 0c73  uid_listrH...Z.s
-000061f0: 7562 6964 5f73 665f 6f62 6a5a 116c 616b  ubid_sf_objZ.lak
-00006200: 656c 616b 6569 645f 7366 5f6f 626a 5a11  elakeid_sf_objZ.
-00006210: 5375 625f 4c61 6b65 6964 5f73 665f 6f62  Sub_Lakeid_sf_ob
-00006220: 6a5a 0873 7562 6964 5f73 665a 0d6c 616b  jZ.subid_sfZ.lak
-00006230: 656c 616b 6569 645f 7366 5a0d 5375 625f  elakeid_sfZ.Sub_
-00006240: 4c61 6b65 6964 5f73 665a 0d6f 6c64 5f6e  Lakeid_sfZ.old_n
-00006250: 6577 5f68 7275 6964 5a08 7461 725f 696e  ew_hruidZ.tar_in
-00006260: 666f 7224 0000 0072 2400 0000 7225 0000  for$...r$...r%..
-00006270: 00da 1544 6574 6572 6d69 6e65 5f4c 616b  ...Determine_Lak
-00006280: 655f 4852 555f 4964 c805 0000 7390 0000  e_HRU_Id....s...
-00006290: 0000 0d04 0104 0104 030e 0208 0104 0112  ................
-000062a0: 0112 0b14 010e 010e 010e 0402 010c 0106  ................
-000062b0: 0104 010e 0106 0202 010c 0106 0104 010e  ................
-000062c0: 0106 0202 010c 0106 0104 010e 0106 040a  ................
-000062d0: 0102 030a 0104 010e 020a 0206 ff04 030c  ................
-000062e0: 0110 0208 010e 030a 010e 0108 010a 0302  ................
-000062f0: 0110 ff10 0814 010e 010e 010e 010a 0104  ................
-00006300: 010a 0108 0116 0104 0204 010a 010a ff02  ................
-00006310: ff04 040e 010a 0104 0118 0118 0118 011c  ................
-00006320: 0272 d500 0000 6304 0000 0000 0000 0000  .r....c.........
-00006330: 0000 0006 0000 0004 0000 0043 0000 0073  ...........C...s
-00006340: 8a00 0000 7c00 6a00 7c00 7c02 1900 6401  ....|.j.|.|...d.
-00006350: 6b03 1900 7d04 7401 7c04 8301 6401 6b04  k...}.t.|...d.k.
-00006360: 722e 7c04 7c02 1900 6a02 6401 1900 7d05  r.|.|...j.d...}.
-00006370: 6e58 7c01 6a00 7c01 7c02 1900 6401 6b03  nX|.j.|.|...d.k.
-00006380: 1900 7d01 7c01 6a03 6402 6403 6404 8d02  ..}.|.j.d.d.d...
-00006390: 7d01 7401 7c01 8301 6401 6b04 726a 7c01  }.t.|...d.k.rj|.
-000063a0: 7c02 1900 6a02 6401 1900 7d05 6e1c 7c03  |...j.d...}.n.|.
-000063b0: 6a00 7c03 7c02 1900 6401 6b03 1900 7c02  j.|.|...d.k...|.
-000063c0: 1900 6a02 6401 1900 7d05 7c05 5300 2905  ..j.d...}.|.S.).
-000063d0: 4e72 0100 0000 7233 0000 0046 7237 0000  Nr....r3...Fr7..
-000063e0: 0029 0472 1900 0000 7215 0000 0072 1300  .).r....r....r..
-000063f0: 0000 7241 0000 0029 06da 1641 7474 7269  ..rA...)...Attri
-00006400: 5f74 6162 6c65 5f4c 616b 655f 4852 555f  _table_Lake_HRU_
-00006410: 69da 0753 7562 496e 666f da06 436f 6c5f  i..SubInfo..Col_
-00006420: 4e4d 5a09 696e 666f 5f64 6174 615a 0d69  NMZ.info_dataZ.i
-00006430: 6e66 6f5f 6c61 6b65 5f68 7275 5a0b 5570  nfo_lake_hruZ.Up
-00006440: 6461 7465 7661 6c75 6572 2400 0000 7224  datevaluer$...r$
-00006450: 0000 0072 2500 0000 da1f 5265 7472 756e  ...r%.....Retrun
-00006460: 5f56 616c 6964 6174 655f 4174 7472 6962  _Validate_Attrib
-00006470: 7574 655f 5661 6c75 6543 0600 0073 1400  ute_ValueC...s..
-00006480: 0000 0002 1202 0aff 0203 1002 1201 0e01  ................
-00006490: 0c01 1002 1c03 72d9 0000 0063 0a00 0000  ......r....c....
-000064a0: 0000 0000 0000 0000 1a00 0000 0700 0000  ................
-000064b0: 4300 0000 735e 0400 007c 007c 0119 0064  C...s^...|.|...d
-000064c0: 016b 017d 0a7c 007c 0219 0064 016b 017c  .k.}.|.|...d.k.|
-000064d0: 007c 0219 0064 026b 0340 007d 0b7c 007c  .|...d.k.@.}.|.|
-000064e0: 0319 0064 016b 017c 007c 0319 0064 026b  ...d.k.|.|...d.k
-000064f0: 0340 007d 0c7c 007c 0419 0064 016b 017c  .@.}.|.|...d.k.|
-00006500: 007c 0419 0064 026b 0340 007d 0d7c 007c  .|...d.k.@.}.|.|
-00006510: 0619 0064 016b 017c 007c 0619 0064 026b  ...d.k.|.|...d.k
-00006520: 0340 007d 0e7c 0a7c 0b42 007c 0c42 007c  .@.}.|.|.B.|.B.|
-00006530: 0d42 007c 0e42 007d 0f74 00a0 017c 006a  .B.|.B.}.t...|.j
-00006540: 027c 0f64 0366 0219 006a 03a1 017d 107c  .|.d.f...j...}.|
-00006550: 107c 1064 016b 0419 007d 1074 0464 0174  .|.d.k...}.t.d.t
-00006560: 057c 1083 0183 0244 0090 025d f27d 117c  .|.....D...].}.|
-00006570: 107c 1119 007d 127c 1264 016b 0272 c871  .|...}.|.d.k.r.q
-00006580: b07c 006a 027c 0064 0319 007c 126b 0219  .|.j.|.d...|.k..
-00006590: 007d 137c 136a 0664 0464 0564 068d 027d  .}.|.j.d.d.d...}
-000065a0: 137c 1364 0719 006a 0364 0119 007d 147c  .|.d...j.d...}.|
-000065b0: 006a 027c 0064 0719 007c 146b 0219 007d  .j.|.d...|.k...}
-000065c0: 1574 0464 0174 057c 1383 0183 0244 0090  .t.d.t.|.....D..
-000065d0: 025d 8a7d 167c 1364 0819 006a 037c 1619  .].}.|.d...j.|..
-000065e0: 007d 177c 1364 0919 006a 037c 1619 007d  .}.|.d...j.|...}
-000065f0: 187c 1864 016b 0490 0272 887c 137c 0319  .|.d.k...r.|.|..
-00006600: 006a 0364 0119 0064 016b 0290 0172 7c74  .j.d...d.k...r|t
-00006610: 077c 137c 157c 037c 0883 047d 197c 197c  .|.|.|.|...}.|.|
-00006620: 006a 027c 0064 0819 007c 176b 027c 0366  .j.|.d...|.k.|.f
-00006630: 023c 006e 207c 137c 0319 006a 0364 0119  .<.n |.|...j.d..
-00006640: 007c 006a 027c 0064 0819 007c 176b 027c  .|.j.|.d...|.k.|
-00006650: 0366 023c 007c 137c 0519 006a 0364 0119  .f.<.|.|...j.d..
-00006660: 0064 016b 0290 0172 d674 077c 137c 157c  .d.k...r.t.|.|.|
-00006670: 057c 0083 047d 197c 197c 006a 027c 0064  .|...}.|.|.j.|.d
-00006680: 0819 007c 176b 027c 0566 023c 006e 207c  ...|.k.|.f.<.n |
-00006690: 137c 0519 006a 0364 0119 007c 006a 027c  .|...j.d...|.j.|
-000066a0: 0064 0819 007c 176b 027c 0566 023c 007c  .d...|.k.|.f.<.|
-000066b0: 137c 0619 006a 0364 0119 0064 016b 0290  .|...j.d...d.k..
-000066c0: 0272 3074 077c 137c 157c 067c 0083 047d  .r0t.|.|.|.|...}
-000066d0: 197c 197c 006a 027c 0064 0819 007c 176b  .|.|.j.|.d...|.k
-000066e0: 027c 0666 023c 006e 207c 137c 0619 006a  .|.f.<.n |.|...j
-000066f0: 0364 0119 007c 006a 027c 0064 0819 007c  .d...|.j.|.d...|
-00006700: 176b 027c 0666 023c 0074 0864 0283 017c  .k.|.f.<.t.d...|
-00006710: 006a 027c 0064 0819 007c 176b 027c 0266  .j.|.d...|.k.|.f
-00006720: 023c 0074 0864 0283 017c 006a 027c 0064  .<.t.d...|.j.|.d
-00006730: 0819 007c 176b 027c 0466 023c 0090 0171  ...|.k.|.f.<...q
-00006740: 167c 137c 0319 006a 037c 1619 0064 016b  .|.|...j.|...d.k
-00006750: 0290 0272 c074 077c 137c 157c 037c 0883  ...r.t.|.|.|.|..
-00006760: 047d 197c 197c 006a 027c 0064 0819 007c  .}.|.|.j.|.d...|
-00006770: 176b 027c 0366 023c 007c 137c 0219 006a  .k.|.f.<.|.|...j
-00006780: 037c 1619 0064 016b 0290 0272 f874 077c  .|...d.k...r.t.|
-00006790: 137c 157c 027c 0783 047d 197c 197c 006a  .|.|.|...}.|.|.j
-000067a0: 027c 0064 0819 007c 176b 027c 0266 023c  .|.d...|.k.|.f.<
-000067b0: 007c 137c 0419 006a 037c 1619 0064 016b  .|.|...j.|...d.k
-000067c0: 0290 0372 3074 077c 137c 157c 047c 0983  ...r0t.|.|.|.|..
-000067d0: 047d 197c 197c 006a 027c 0064 0819 007c  .}.|.|.j.|.d...|
-000067e0: 176b 027c 0466 023c 007c 137c 0519 006a  .k.|.f.<.|.|...j
-000067f0: 037c 1619 0064 016b 0290 0372 6874 077c  .|...d.k...rht.|
-00006800: 137c 157c 057c 0083 047d 197c 197c 006a  .|.|.|...}.|.|.j
-00006810: 027c 0064 0819 007c 176b 027c 0566 023c  .|.d...|.k.|.f.<
-00006820: 007c 137c 0619 006a 037c 1619 0064 016b  .|.|...j.|...d.k
-00006830: 0290 0172 1674 077c 137c 157c 067c 0083  ...r.t.|.|.|.|..
-00006840: 047d 197c 197c 006a 027c 0064 0819 007c  .}.|.|.j.|.d...|
-00006850: 176b 027c 0666 023c 0090 0171 1671 b07c  .k.|.f.<...q.q.|
-00006860: 006a 0967 0064 0aa2 0164 0b8d 017d 0074  .j.g.d...d...}.t
-00006870: 0a6a 0b7c 007c 0764 0c7c 0264 0d8d 046a  .j.|.|.d.|.d...j
-00006880: 0c64 0e64 0f8d 017d 0074 0a6a 0b7c 007c  .d.d...}.t.j.|.|
-00006890: 0864 0c7c 0364 0d8d 046a 0c64 0e64 0f8d  .d.|.d...j.d.d..
-000068a0: 017d 0074 0a6a 0b7c 007c 0964 0c7c 0464  .}.t.j.|.|.d.|.d
-000068b0: 0d8d 046a 0c64 0e64 0f8d 017d 007c 0064  ...j.d.d...}.|.d
-000068c0: 0319 00a0 0d74 0ea1 017c 007c 0219 00a0  .....t...|.|....
-000068d0: 0d74 0ea1 0117 007c 007c 0319 00a0 0d74  .t.....|.|.....t
-000068e0: 0ea1 0117 007c 007c 0519 00a0 0d74 0ea1  .....|.|.....t..
-000068f0: 0117 007c 0064 103c 0074 0aa0 0f7c 0064  ...|.d.<.t...|.d
-00006900: 1019 00a1 0164 0119 0064 1117 007c 0064  .....d...d...|.d
-00006910: 123c 007c 0053 0029 137a ab46 756e 6374  .<.|.S.).z.Funct
-00006920: 696f 6e20 746f 2064 6574 6572 6d69 6e65  ion to determine
-00006930: 206c 616e 6475 7365 2c73 6f69 6c2c 616e   landuse,soil,an
-00006940: 6420 7665 6720 616e 6420 6f74 6865 7220  d veg and other 
-00006950: 7072 6f70 6572 7469 6573 2061 6674 6572  properties after
-00006960: 2075 6e69 6f6e 2061 6c6c 2070 6f6c 7967   union all polyg
-00006970: 6f6e 730a 2020 2020 2d2d 2d2d 2d2d 2d2d  ons.    --------
-00006980: 2d2d 0a0a 2020 2020 4e6f 7465 730a 2020  --..    Notes.  
-00006990: 2020 2d2d 2d2d 2d2d 2d0a 0a20 2020 2052    -------..    R
-000069a0: 6574 7572 6e73 3a0a 2020 2020 2d2d 2d2d  eturns:.    ----
-000069b0: 2d2d 2d0a 2020 2020 2020 2020 4e6f 6e65  ---.        None
-000069c0: 2c0a 2020 2020 7201 0000 0072 6b00 0000  ,.    r....rk...
-000069d0: 72d0 0000 0072 3300 0000 4672 3700 0000  r....r3...Fr7...
-000069e0: 7206 0000 0072 a400 0000 724d 0000 0029  r....r....rM...)
-000069f0: 035a 0a4c 414e 445f 5553 455f 435a 0556  .Z.LAND_USE_CZ.V
-00006a00: 4547 5f43 5a09 534f 494c 5f50 524f 4672  EG_CZ.SOIL_PROFr
-00006a10: 1000 0000 da05 696e 6e65 7229 0272 0c00  ......inner).r..
-00006a20: 0000 720b 0000 0054 7207 0000 00da 0766  ..r....Tr......f
-00006a30: 6163 7465 7273 7228 0000 0072 5700 0000  actersr(...rW...
-00006a40: 2910 721a 0000 0072 2b00 0000 7219 0000  ).r....r+...r...
-00006a50: 0072 1300 0000 7229 0000 0072 1500 0000  .r....r)...r....
-00006a60: 7241 0000 0072 d900 0000 722d 0000 0072  rA...r....r-...r
-00006a70: 1c00 0000 7240 0000 0072 1800 0000 7214  ....r@...r....r.
-00006a80: 0000 0072 1600 0000 da03 7374 72da 0966  ...r......str..f
-00006a90: 6163 746f 7269 7a65 291a 5a0b 4174 7472  actorize).Z.Attr
-00006aa0: 695f 7461 626c 6572 d200 0000 7247 0000  i_tabler....rG..
-00006ab0: 0072 5000 0000 7251 0000 0072 5200 0000  .rP...rQ...rR...
-00006ac0: 7253 0000 005a 114c 616e 6475 7365 5f69  rS...Z.Landuse_i
-00006ad0: 6e66 6f5f 6461 7461 5a0e 536f 696c 5f69  nfo_dataZ.Soil_i
-00006ae0: 6e66 6f5f 6461 7461 5a0d 5665 675f 696e  nfo_dataZ.Veg_in
-00006af0: 666f 5f64 6174 615a 0969 6e76 616c 5f73  fo_dataZ.inval_s
-00006b00: 7562 5a0d 696e 7661 6c5f 6c61 6e64 7573  ubZ.inval_landus
-00006b10: 655a 0a69 6e76 616c 5f73 6f69 6c5a 0969  eZ.inval_soilZ.i
-00006b20: 6e76 616c 5f76 6567 5a08 696e 7661 6c5f  nval_vegZ.inval_
-00006b30: 6f32 5a0a 696e 7661 6c5f 726f 7773 5a0c  o2Z.inval_rowsZ.
-00006b40: 4c61 6b65 5f48 5255 5f49 4453 7248 0000  Lake_HRU_IDSrH..
-00006b50: 005a 0c69 6c61 6b65 5f68 7275 5f69 6472  .Z.ilake_hru_idr
-00006b60: d600 0000 5a05 5375 6269 6472 d700 0000  ....Z.Subidr....
-00006b70: 725e 0000 005a 0769 6872 755f 6964 5a07  r^...Z.ihru_idZ.
-00006b80: 6973 5f4c 616b 655a 0a56 616c 695f 5661  is_LakeZ.Vali_Va
-00006b90: 6c75 6572 2400 0000 7224 0000 0072 2500  luer$...r$...r%.
-00006ba0: 0000 da18 4465 7465 726d 696e 655f 4852  ....Determine_HR
-00006bb0: 555f 4174 7472 6962 7574 6573 5606 0000  U_AttributesV...
-00006bc0: 73f8 0000 0000 180c 0118 0118 0118 0118  s...............
-00006bd0: 0214 0116 010c 0314 0108 0108 0102 0204  ................
-00006be0: 010a ff04 0304 0104 ff06 030e 0112 0114  ................
-00006bf0: 010e 010e 010a 0310 ff04 0302 0108 ff04  ................
-00006c00: 0502 fe04 010e ff04 060c fe04 010e ff02  ................
-00006c10: 0510 ff04 0302 0108 ff04 0502 fe04 010e  ................
-00006c20: ff04 060c fe04 010e ff02 0510 ff04 0302  ................
-00006c30: 0108 ff04 0502 fe04 010e ff04 060c fe04  ................
-00006c40: 010e ff02 041a 011e 0410 ff04 0302 0108  ................
-00006c50: ff04 0502 fe04 010e ff02 0410 ff04 0302  ................
-00006c60: 0108 ff04 0502 fe04 010e ff02 0410 ff04  ................
-00006c70: 0302 0108 ff04 0502 fe04 010e ff02 0410  ................
-00006c80: ff04 0302 0108 ff04 0502 fe04 010e ff02  ................
-00006c90: 0410 ff04 0302 0108 ff04 0502 fe04 010e  ................
-00006ca0: ff08 0410 011a 011a 011a 580c 010c ff02  ..........X.....
-00006cb0: 020c fe02 040c fc02 ff06 081a 0172 de00  .............r..
-00006cc0: 0000 6303 0000 0000 0000 0000 0000 0041  ..c............A
-00006cd0: 0000 000c 0000 0043 0000 0073 440b 0000  .......C...sD...
-00006ce0: 6401 7d03 6402 7d04 6403 7d05 6404 7d06  d.}.d.}.d.}.d.}.
-00006cf0: 6405 7d07 6405 7c00 6a00 7601 7222 6406  d.}.d.|.j.v.r"d.
-00006d00: 7d07 7c00 6a01 6407 6408 8d01 7d08 6409  }.|.j.d.d...}.d.
-00006d10: 7c08 640a 3c00 6409 7c08 640b 3c00 7c08  |.d.<.d.|.d.<.|.
-00006d20: 6a02 6407 6407 640c 8d02 0100 7403 a004  j.d.d.d.....t...
-00006d30: 7c08 6403 1900 6a05 a101 7d09 7c02 640d  |.d...j...}.|.d.
-00006d40: 1400 640d 1400 7c09 6b04 728c 7c09 640e  ..d...|.k.r.|.d.
-00006d50: 1b00 640e 1b00 640f 1800 7d02 6409 7c08  ..d...d...}.d.|.
-00006d60: 7c07 3c00 6409 7c00 7c07 3c00 7c00 6a06  |.<.d.|.|.<.|.j.
-00006d70: 7c00 7c05 1900 7c02 640d 1400 640d 1400  |.|...|.d...d...
-00006d80: 6b05 1900 a001 a100 7d0a 7407 7c0a 6409  k.......}.t.|.d.
-00006d90: 6410 8d02 7d0a 7c0a 6a08 6411 6701 6407  d...}.|.j.d.g.d.
-00006da0: 6412 8d02 7d0a 7c0a 6a06 7c0a 6413 1900  d...}.|.j.|.d...
-00006db0: 6414 6b03 1900 a001 a100 7d0a 7c0a 7c03  d.k.......}.|.|.
-00006dc0: 1900 6a05 7d0b 7c0a 6a06 7c0a 6413 1900  ..j.}.|.j.|.d...
-00006dd0: 640f 6b02 1900 6415 1900 6a05 7d0c 7403  d.k...d...j.}.t.
-00006de0: a009 7c0c 7c0c 6416 6b04 1900 a101 7d0c  ..|.|.d.k.....}.
-00006df0: 7c00 6a06 7c00 6415 1900 a00a 7c0c a101  |.j.|.d.....|...
-00006e00: 1900 a001 a100 7d0d 7c0d 7c03 1900 6a05  ......}.|.|...j.
-00006e10: 7d0e 7c00 6a06 7c00 6401 1900 a00a 7c0b  }.|.j.|.d.....|.
-00006e20: a101 0f00 7c00 7c07 1900 6416 6b04 4000  ....|.|...d.k.@.
-00006e30: 1900 6a01 6407 6408 8d01 7d0f 7c0f 6a06  ..j.d.d...}.|.j.
-00006e40: 7c0f 6415 1900 6416 6b01 1900 6401 1900  |.d...d.k...d...
-00006e50: 6a05 7d10 7c00 6a01 6407 6408 8d01 7d11  j.}.|.j.d.d...}.
-00006e60: 7c11 6401 1900 a00a 7c10 a101 7d12 7c11  |.d.....|...}.|.
-00006e70: 6415 1900 640f 6b00 7d13 7403 a00b 7c12  d...d.k.}.t...|.
-00006e80: 7c13 a102 7d14 7c11 6a06 7c11 6401 1900  |...}.|.j.|.d...
-00006e90: a00a 7c10 a101 6401 6602 1900 0b00 7c11  ..|...d.f.....|.
-00006ea0: 6a06 7c14 6415 6602 3c00 7c11 6a06 7c11  j.|.d.f.<.|.j.|.
-00006eb0: 6401 1900 a00a 7c10 a101 6415 6602 1900  d.....|...d.f...
-00006ec0: 6a05 7d15 7c01 6417 1900 6a05 7d16 7403  j.}.|.d...j.}.t.
-00006ed0: a00c 7c16 7c0c a102 7d14 7c16 7403 a00d  ..|.|...}.|.t...
-00006ee0: 7c14 a101 1900 a001 a100 7d17 7c11 6a06  |.........}.|.j.
-00006ef0: 7c11 6415 1900 a00a 7c17 a101 7c11 6415  |.d.....|...|.d.
-00006f00: 1900 a00a 7c15 a101 4200 1900 a001 a100  ....|...B.......
-00006f10: 7d18 7c00 6a06 7c00 6413 1900 6414 6b02  }.|.j.|.d...d.k.
-00006f20: 1900 6401 1900 6a05 7d19 7403 a009 7c19  ..d...j.}.t...|.
-00006f30: 7c19 6416 6b04 1900 a101 7d19 7c00 6a06  |.d.k.....}.|.j.
-00006f40: 7c00 6413 1900 6414 6b02 1900 6415 1900  |.d...d.k...d...
-00006f50: 6a05 7d1a 7403 a009 7c1a 7c1a 6416 6b04  j.}.t...|.|.d.k.
-00006f60: 1900 a101 7d1a 7403 a009 7c0b a101 7d1b  ....}.t...|...}.
-00006f70: 7c00 6401 6402 6702 1900 a00e 6418 a101  |.d.d.g.....d...
-00006f80: 6a05 7d1c 7c0a 6404 1900 6a05 7d1d 7403  j.}.|.d...j.}.t.
-00006f90: a009 7c1d a101 7d1d 7c08 6a06 7c08 6413  ..|...}.|.j.|.d.
-00006fa0: 1900 6414 6b02 1900 6401 1900 6a05 7c08  ..d.k...d...j.|.
-00006fb0: 6a06 7c08 6413 1900 6414 6b02 640a 6602  j.|.d...d.k.d.f.
-00006fc0: 3c00 7c18 a00f 6415 6701 a101 6403 1900  <.|...d.g...d...
-00006fd0: a010 7404 a101 7c18 6403 1900 6b02 7d1e  ..t...|.d...k.}.
-00006fe0: 7c18 7c1e 1900 7d1f 7c1f 6a08 6411 6403  |.|...}.|.j.d.d.
-00006ff0: 6702 6407 6407 6702 6412 8d02 7d1f 7c00  g.d.d.g.d...}.|.
-00007000: 7c00 6402 1900 6416 6b00 1900 6a01 6407  |.d...d.k...j.d.
-00007010: 6408 8d01 7d20 7411 6416 7412 7c20 8301  d...} t.d.t.| ..
-00007020: 8302 4400 5d50 7d21 7c20 6403 1900 6a05  ..D.]P}!| d...j.
-00007030: 7c21 1900 7c02 640d 1400 640d 1400 6b01  |!..|.d...d...k.
-00007040: 9003 7244 7c20 6401 1900 6a05 7c21 1900  ..rD| d...j.|!..
-00007050: 7d22 7413 7c1c 7c22 8302 7d23 7414 7c22  }"t.|.|"..}#t.|"
-00007060: 7c00 7c08 640f 7c00 7c23 6409 6419 8d07  |.|.d.|.|#d.d...
-00007070: 7d08 9003 7144 7411 6416 7412 7c1f 8301  }...qDt.d.t.|...
-00007080: 8302 4400 9001 5d08 7d21 7403 a009 7c08  ..D...].}!t...|.
-00007090: 6a06 7c08 640a 1900 6416 6b04 1900 7c03  j.|.d...d.k...|.
-000070a0: 1900 6a05 a101 7d24 7c1f 6415 1900 6a05  ..j...}$|.d...j.
-000070b0: 7c21 1900 7d25 7c11 7c11 6415 1900 7c25  |!..}%|.|.d...|%
-000070c0: 6b02 1900 7d26 7403 a009 7c26 6404 1900  k...}&t...|&d...
-000070d0: 6a05 a101 7d27 6700 7d28 7411 6416 7412  j...}'g.}(t.d.t.
-000070e0: 7c27 8301 8302 4400 5d82 7d29 7c27 7c29  |'....D.].})|'|)
-000070f0: 1900 7d2a 7c26 6a06 7c26 6404 1900 7c2a  ..}*|&j.|&d...|*
-00007100: 6b02 1900 a001 a100 7d2b 7c2b 6a08 6403  k.......}+|+j.d.
-00007110: 6701 641a 6412 8d02 7d2b 7c2b 6401 1900  g.d.d...}+|+d...
-00007120: 6a05 6416 1900 7d22 7413 7c1c 7c22 8302  j.d...}"t.|.|"..
-00007130: 7d23 7c23 7c23 6416 6b04 1900 7d23 7403  }#|#|#d.k...}#t.
-00007140: a00c 7c23 7c24 a102 7d14 7c23 7403 a00d  ..|#|$..}.|#t...
-00007150: 7c14 a101 1900 7d2c 6700 7c28 a201 7c2c  |.....},g.|(..|,
-00007160: a015 a100 a201 7d28 9004 7108 7403 a016  ......}(..q.t...
-00007170: 7c28 a101 7d28 7414 7c22 7c11 7c08 640f  |(..}(t.|"|.|.d.
-00007180: 7c11 7c28 6414 6419 8d07 7d08 9003 71a4  |.|(d.d...}...q.
-00007190: 7411 6416 7412 7c1d 8301 8302 4400 9005  t.d.t.|.....D...
-000071a0: 5df0 7d2d 7c1d 7c2d 1900 7d2e 7c0a 6a06  ].}-|.|-..}.|.j.
-000071b0: 7c0a 6404 1900 7c2e 6b02 1900 a001 a100  |.d...|.k.......
-000071c0: 7d2f 7c2f 6a08 641b 6701 6407 6412 8d02  }/|/j.d.g.d.d...
-000071d0: 7d2f 6416 7d30 6700 7d28 640f 7d31 7411  }/d.}0g.}(d.}1t.
-000071e0: 6416 7412 7c2f 8301 8302 4400 9005 5d9e  d.t.|/....D...].
-000071f0: 7d32 7c2f 6401 1900 6a05 7c32 1900 7d22  }2|/d...j.|2..}"
-00007200: 7c2f 6415 1900 6a05 7c32 1900 7d33 7c28  |/d...j.|2..}3|(
-00007210: a017 7c22 a101 0100 7403 a009 7c08 6a06  ..|"....t...|.j.
-00007220: 7c08 640a 1900 6416 6b04 1900 7c03 1900  |.d...d.k...|...
-00007230: 6a05 a101 7d24 7c30 7c2f 641c 1900 6a05  j...}$|0|/d...j.
-00007240: 7c32 1900 1700 7d30 7c32 7412 7c2f 8301  |2....}0|2t.|/..
-00007250: 640f 1800 6b03 9005 729c 7c2f 6415 1900  d...k...r.|/d...
-00007260: 6a05 7c32 1900 7c2f 6415 1900 6a05 7c32  j.|2..|/d...j.|2
-00007270: 640f 1700 1900 6b02 7d34 6e04 641a 7d34  d.....k.}4n.d.}4
-00007280: 7c2f 7c07 1900 6a05 7c32 1900 6416 6b01  |/|...j.|2..d.k.
-00007290: 7d35 7c32 7412 7c2f 8301 6414 1800 6b01  }5|2t.|/..d...k.
-000072a0: 9005 72f4 7c2f 641c 1900 6a05 7c32 640f  ..r.|/d...j.|2d.
-000072b0: 1700 1900 641d 6b00 9005 72e2 6407 7d36  ....d.k...r.d.}6
-000072c0: 6e10 7c30 7c02 640d 1400 640d 1400 6b00  n.|0|.d...d...k.
-000072d0: 7d36 6e10 7c30 7c02 640d 1400 640d 1400  }6n.|0|.d...d...
-000072e0: 6b00 7d36 7c30 641d 6b00 7d37 7c32 640f  k.}6|0d.k.}7|2d.
-000072f0: 6b05 9006 727e 7c32 7412 7c2f 8301 6414  k...r~|2t.|/..d.
-00007300: 1800 6b01 9006 727e 7c2f 6415 1900 6a05  ..k...r~|/d...j.
-00007310: 7c32 640f 1800 1900 7c2f 6415 1900 6a05  |2d.....|/d...j.
-00007320: 7c32 1900 6b03 7d38 7c2f 6415 1900 6a05  |2..k.}8|/d...j.
-00007330: 7c32 1900 7c2f 6415 1900 6a05 7c32 640f  |2..|/d...j.|2d.
-00007340: 1700 1900 6b03 7d39 7c2f 6415 1900 6a05  ....k.}9|/d...j.
-00007350: 7c32 1900 6416 6b01 7d3a 641a 7d37 7c32  |2..d.k.}:d.}7|2
-00007360: 6416 6b02 9006 72d4 7c32 7412 7c2f 8301  d.k...r.|2t.|/..
-00007370: 640f 1800 6b00 9006 72d4 6407 7d38 7c2f  d...k...r.d.}8|/
-00007380: 6415 1900 6a05 7c32 1900 7c2f 6415 1900  d...j.|2..|/d...
-00007390: 6a05 7c32 640f 1700 1900 6b03 7d39 7c2f  j.|2d.....k.}9|/
-000073a0: 6415 1900 6a05 7c32 1900 6416 6b01 7d3a  d...j.|2..d.k.}:
-000073b0: 641a 7d37 7c32 7412 7c2f 8301 6414 1800  d.}7|2t.|/..d...
-000073c0: 6b02 9008 720e 7c2f 6415 1900 6a05 7c32  k...r.|/d...j.|2
-000073d0: 1900 6416 6b04 9008 720e 6407 7d38 7c2f  ..d.k...r.d.}8|/
-000073e0: 6415 1900 6a05 7c32 1900 7c2f 6415 1900  d...j.|2..|/d...
-000073f0: 6a05 7c32 640f 1700 1900 6b03 7d39 7c2f  j.|2d.....k.}9|/
-00007400: 6415 1900 6a05 7c32 1900 6416 6b04 7d3a  d...j.|2..d.k.}:
-00007410: 7c2f 6402 1900 6a05 7c32 1900 7d3b 641a  |/d...j.|2..};d.
-00007420: 7d37 7c37 9008 720e 7c39 9008 720e 7c2f  }7|7..r.|9..r.|/
-00007430: 6415 1900 6a05 7c32 1900 7c00 6a06 7c00  d...j.|2..|.j.|.
-00007440: 6401 1900 7c3b 6b02 6415 6602 3c00 7c2f  d...|;k.d.f.<.|/
-00007450: 6413 1900 6a05 7c32 1900 7c00 6a06 7c00  d...j.|2..|.j.|.
-00007460: 6401 1900 7c3b 6b02 6413 6602 3c00 7c2f  d...|;k.d.f.<.|/
-00007470: 641e 1900 6a05 7c32 1900 7c00 6a06 7c00  d...j.|2..|.j.|.
-00007480: 6401 1900 7c3b 6b02 641e 6602 3c00 7c2f  d...|;k.d.f.<.|/
-00007490: 641f 1900 6a05 7c32 1900 7c00 6a06 7c00  d...j.|2..|.j.|.
-000074a0: 6401 1900 7c3b 6b02 641f 6602 3c00 7c2f  d...|;k.d.f.<.|/
-000074b0: 6420 1900 6a05 7c32 1900 7c00 6a06 7c00  d ..j.|2..|.j.|.
-000074c0: 6401 1900 7c3b 6b02 6420 6602 3c00 7c2f  d...|;k.d f.<.|/
-000074d0: 6421 1900 6a05 7c32 1900 7c00 6a06 7c00  d!..j.|2..|.j.|.
-000074e0: 6401 1900 7c3b 6b02 6421 6602 3c00 7c32  d...|;k.d!f.<.|2
-000074f0: 7412 7c2f 8301 640f 1800 6b02 9008 722c  t.|/..d...k...r,
-00007500: 6407 7d38 641a 7d39 6407 7d3a 7c32 7412  d.}8d.}9d.}:|2t.
-00007510: 7c2f 8301 640f 1800 6b02 9009 7256 6416  |/..d...k...rVd.
-00007520: 7d30 7403 a016 7c28 a101 7d2c 7c33 6416  }0t...|(..},|3d.
-00007530: 6b04 9008 72aa 7c00 6a06 7c00 6415 1900  k...r.|.j.|.d...
-00007540: 7c33 6b02 1900 a001 a100 7d3c 7c3c 6401  |3k.......}<|<d.
-00007550: 6402 6702 1900 a00e 6418 a101 6a05 7d3d  d.g.....d...j.}=
-00007560: 7413 7c3d 7c22 8302 7d3e 7403 a009 7403  t.|=|"..}>t...t.
-00007570: a018 7c2c 7c3e 6702 a101 a101 7d2c 7c2c  ..|,|>g.....},|,
-00007580: 7c2c 6416 6b04 1900 7d2c 7413 7c1c 7c22  |,d.k...},t.|.|"
-00007590: 8302 7d23 7c23 7c23 6416 6b04 1900 7d23  ..}#|#|#d.k...}#
-000075a0: 7403 a00c 7c23 7c0b a102 7d12 7c23 7403  t...|#|...}.|#t.
-000075b0: a00d 7c12 a101 1900 7d3f 7403 a009 7403  ..|.....}?t...t.
-000075c0: a018 7c2c 7c3f 6702 a101 a101 7d2c 7c2c  ..|,|?g.....},|,
-000075d0: 7c2c 6416 6b04 1900 7d2c 7403 a00c 7c2c  |,d.k...},t...|,
-000075e0: 7c24 a102 7d14 7c2c 7403 a00d 7c14 a101  |$..}.|,t...|...
-000075f0: 1900 7d2c 7403 a00c 7c2c 7c19 a102 7d40  ..},t...|,|...}@
-00007600: 7c2c 7403 a00d 7c40 a101 1900 7d2c 7414  |,t...|@....},t.
-00007610: 7c22 7c00 7c08 640f 7c2c 7c0a 6422 7c31  |"|.|.d.|,|.d"|1
-00007620: 6423 8d08 7d08 6700 7d28 7c31 640f 1700  d#..}.g.}(|1d...
-00007630: 7d31 9005 710c 7c38 9009 727c 7c39 9009  }1..q.|8..r||9..
-00007640: 727c 7c3a 9009 727c 7c35 9009 727c 7c37  r||:..r||5..r||7
-00007650: 9009 727c 9005 710c 9005 710c 7c34 9009  ..r|..q...q.|4..
-00007660: 7296 7c35 9009 7296 7c36 9009 7296 9005  r.|5..r.|6..r...
-00007670: 710c 9005 710c 6416 7d30 7403 a016 7c28  q...q.d.}0t...|(
-00007680: a101 7d2c 7c33 6416 6b04 900a 7202 7c00  ..},|3d.k...r.|.
-00007690: 6a06 7c00 6415 1900 7c33 6b02 1900 a001  j.|.d...|3k.....
-000076a0: a100 7d3c 7c3c 6401 6402 6702 1900 a00e  ..}<|<d.d.g.....
-000076b0: 6418 a101 6a05 7d3d 7413 7c3d 7c22 8302  d...j.}=t.|=|"..
-000076c0: 7d3e 7403 a009 7403 a018 7c2c 7c3e 6702  }>t...t...|,|>g.
-000076d0: a101 a101 7d2c 7c2c 7c2c 6416 6b04 1900  ....},|,|,d.k...
-000076e0: 7d2c 7413 7c1c 7c22 8302 7d23 7c23 7c23  },t.|.|"..}#|#|#
-000076f0: 6416 6b04 1900 7d23 7403 a00c 7c23 7c0b  d.k...}#t...|#|.
-00007700: a102 7d12 7c23 7403 a00d 7c12 a101 1900  ..}.|#t...|.....
-00007710: 7d3f 7403 a009 7403 a018 7c2c 7c3f 6702  }?t...t...|,|?g.
-00007720: a101 a101 7d2c 7c2c 7c2c 6416 6b04 1900  ....},|,|,d.k...
-00007730: 7d2c 7403 a00c 7c2c 7c24 a102 7d14 7c2c  },t...|,|$..}.|,
-00007740: 7403 a00d 7c14 a101 1900 7d2c 7403 a00c  t...|.....},t...
-00007750: 7c2c 7c19 a102 7d40 7c2c 7403 a00d 7c40  |,|...}@|,t...|@
-00007760: a101 1900 7d2c 7414 7c22 7c00 7c08 640f  ....},t.|"|.|.d.
-00007770: 7c2c 7c0a 6422 7c31 6423 8d08 7d08 6700  |,|.d"|1d#..}.g.
-00007780: 7d28 7c31 640f 1700 7d31 9005 710c 9004  }(|1d...}1..q...
-00007790: 71be 6416 7c08 6a06 7c08 6415 1900 6416  q.d.|.j.|.d...d.
-000077a0: 6b01 6415 6602 3c00 6416 7c08 6a06 7c08  k.d.f.<.d.|.j.|.
-000077b0: 6415 1900 6416 6b01 6413 6602 3c00 6416  d...d.k.d.f.<.d.
-000077c0: 7c08 6a06 7c08 6415 1900 6416 6b01 641e  |.j.|.d...d.k.d.
-000077d0: 6602 3c00 6416 7c08 6a06 7c08 6415 1900  f.<.d.|.j.|.d...
-000077e0: 6416 6b01 641f 6602 3c00 6416 7c08 6a06  d.k.d.f.<.d.|.j.
-000077f0: 7c08 6415 1900 6416 6b01 6420 6602 3c00  |.d...d.k.d f.<.
-00007800: 6416 7c08 6a06 7c08 6415 1900 6416 6b01  d.|.j.|.d...d.k.
-00007810: 6421 6602 3c00 7c08 7c1b 7c0c 7c1a 7c17  d!f.<.|.|.|.|.|.
-00007820: 6605 5300 2924 7aac 4d6f 6469 6679 2061  f.S.)$z.Modify a
-00007830: 7474 7269 6275 7465 2074 6162 6c65 206d  ttribute table m
-00007840: 6170 6f6c 646e 6577 5f69 6e66 6f2c 2063  apoldnew_info, c
-00007850: 7265 6174 6520 6e65 7720 7375 6220 6964  reate new sub id
-00007860: 2066 6f72 2073 7562 6261 7369 6e20 6e65   for subbasin ne
-00007870: 6564 7320 746f 2062 6520 6d65 7267 6564  eds to be merged
-00007880: 2e0a 2020 2020 2d2d 2d2d 2d2d 2d2d 2d2d  ..    ----------
-00007890: 0a0a 2020 2020 4e6f 7465 730a 2020 2020  ..    Notes.    
-000078a0: 2d2d 2d2d 2d2d 2d0a 0a20 2020 2052 6574  -------..    Ret
-000078b0: 7572 6e73 3a0a 2020 2020 2d2d 2d2d 2d2d  urns:.    ------
-000078c0: 2d0a 2020 2020 2020 2020 4e6f 6e65 2c0a  -.        None,.
-000078d0: 2020 2020 7206 0000 0072 0d00 0000 7279      r....r....ry
-000078e0: 0000 0072 6600 0000 7280 0000 0072 8100  ...rf...r....r..
-000078f0: 0000 5472 0700 0000 726b 0000 0072 8300  ..Tr....rk...r..
-00007900: 0000 7285 0000 00a9 0272 1c00 0000 da07  ..r......r......
-00007910: 696e 706c 6163 6572 7c00 0000 72b4 0000  inplacer|...r...
-00007920: 0072 2800 0000 2901 72ab 0000 0072 6900  .r(...).r....ri.
-00007930: 0000 727a 0000 0072 6400 0000 7265 0000  ..rz...rd...re..
-00007940: 0072 8400 0000 7201 0000 0072 ce00 0000  .r....r....r....
-00007950: 7263 0000 0029 0772 4900 0000 729d 0000  rc...).rI...r...
-00007960: 0072 8a00 0000 729e 0000 0072 a000 0000  .r....r....r....
-00007970: 729f 0000 0072 6400 0000 4672 6a00 0000  r....rd...Frj...
-00007980: 7282 0000 0069 8096 9800 7294 0000 0072  r....i....r....r
-00007990: 9600 0000 7295 0000 0072 9700 0000 e903  ....r....r......
-000079a0: 0000 00a9 0872 4900 0000 729d 0000 0072  .....rI...r....r
-000079b0: 8a00 0000 729e 0000 0072 9f00 0000 72a0  ....r....r....r.
-000079c0: 0000 0072 6400 0000 72a1 0000 0029 1972  ...rd...r....).r
-000079d0: 1100 0000 7214 0000 00da 0b72 6573 6574  ....r......reset
-000079e0: 5f69 6e64 6578 721a 0000 0072 7400 0000  _indexr....rt...
-000079f0: 7213 0000 0072 1900 0000 72b0 0000 0072  r....r....r....r
-00007a00: 4100 0000 722b 0000 0072 1200 0000 7243  A...r+...r....rC
-00007a10: 0000 0072 2e00 0000 729a 0000 0072 1600  ...r....r....r..
-00007a20: 0000 723e 0000 00da 0974 7261 6e73 666f  ..r>.....transfo
-00007a30: 726d 7229 0000 0072 1500 0000 7217 0000  rmr)...r....r...
-00007a40: 0072 a300 0000 72c8 0000 00da 0761 7361  .r....r......asa
-00007a50: 7272 6179 724e 0000 0072 1b00 0000 2941  rrayrN...r....)A
-00007a60: 5a0d 6669 6e61 6c72 6976 5f69 6e66 6f5a  Z.finalriv_infoZ
-00007a70: 0e43 6f6e 6e5f 4c61 6b65 735f 706c 79da  .Conn_Lakes_ply.
-00007a80: 0841 7265 615f 4d69 6e72 a200 0000 da0a  .Area_Minr......
-00007a90: 646f 776e 5f63 6f6c 6e6d 5a08 4441 5f63  down_colnmZ.DA_c
-00007aa0: 6f6c 6e6d 5a0b 5365 6749 445f 636f 6c6e  olnmZ.SegID_coln
-00007ab0: 6d72 8c00 0000 728a 0000 005a 066d 6178  mr....r....Z.max
-00007ac0: 5f64 615a 0c53 656c 6563 7465 645f 7269  _daZ.Selected_ri
-00007ad0: 765a 0a53 7562 6964 5f6d 6169 6e5a 1643  vZ.Subid_mainZ.C
-00007ae0: 6f6e 6e65 6374 6564 5f4c 616b 655f 4d61  onnected_Lake_Ma
-00007af0: 696e 7269 765a 0d4c 616b 6563 6f76 6572  inrivZ.Lakecover
-00007b00: 5f72 6976 5a0b 5375 6269 645f 6c61 6b65  _rivZ.Subid_lake
-00007b10: 735a 1d75 6e73 656c 6563 7465 645f 6761  sZ.unselected_ga
-00007b20: 7567 6573 5f73 7562 6964 735f 696e 666f  uges_subids_info
-00007b30: 5a18 756e 7365 6c65 6374 6564 5f67 6175  Z.unselected_gau
-00007b40: 6765 735f 7375 6269 6473 5a11 6669 6e61  ges_subidsZ.fina
-00007b50: 6c72 6976 5f69 6e66 6f5f 6e63 6c72 4a00  lriv_info_nclrJ.
-00007b60: 0000 724b 0000 0072 2300 0000 5a12 6661  ..rK...r#...Z.fa
-00007b70: 6b65 5f6f 6273 5f68 7961 6c6b 6569 6473  ke_obs_hyalkeids
-00007b80: 5a10 416c 6c5f 436f 6e6e 5f4c 616b 6569  Z.All_Conn_Lakei
-00007b90: 6473 5a15 436f 6e6e 5f54 6f5f 4e6f 6e43  dsZ.Conn_To_NonC
-00007ba0: 6f6e 6c61 6b65 6964 735a 1743 6f6e 6e5f  onlakeidsZ.Conn_
-00007bb0: 546f 5f4e 6f6e 436f 6e6c 616b 655f 696e  To_NonConlake_in
-00007bc0: 666f 5a16 4f6c 645f 4e6f 6e5f 436f 6e6e  foZ.Old_Non_Conn
-00007bd0: 6563 745f 5375 6249 6473 5a17 4f6c 645f  ect_SubIdsZ.Old_
-00007be0: 4e6f 6e5f 436f 6e6e 6563 745f 4c61 6b65  Non_Connect_Lake
-00007bf0: 4964 735a 1053 656c 6563 7465 645f 7269  IdsZ.Selected_ri
-00007c00: 765f 6964 7372 7700 0000 da07 5365 675f  v_idsrw.....Seg_
-00007c10: 4944 5372 5f00 0000 5a1e 436f 6e6e 5f54  IDSr_...Z.Conn_T
-00007c20: 6f5f 4e6f 6e43 6f6e 6c61 6b65 5f69 6e66  o_NonConlake_inf
-00007c30: 6f5f 6f75 746c 6574 5a13 616c 6c5f 6f75  o_outletZ.all_ou
-00007c40: 746c 6574 5f73 7562 5f69 6e66 6f72 4800  tlet_sub_inforH.
-00007c50: 0000 da06 7473 7562 6964 5a0d 416c 6c5f  ....tsubidZ.All_
-00007c60: 7570 5f73 7562 6964 735a 0f70 726f 6365  up_subidsZ.proce
-00007c70: 7373 6564 5f73 7562 6964 5a0c 435f 545f  ssed_subidZ.C_T_
-00007c80: 4e5f 4c61 6b65 6964 5a0d 4c61 6b65 5f43  N_LakeidZ.Lake_C
-00007c90: 6174 5f69 6e66 6f5a 0b52 6976 5f53 6567  at_infoZ.Riv_Seg
-00007ca0: 5f49 4453 da0c 6d6f 6469 6679 7375 6269  _IDS..modifysubi
-00007cb0: 6473 725e 0000 005a 0869 7269 765f 7365  dsr^...Z.iriv_se
-00007cc0: 675a 114c 616b 655f 4361 745f 7365 675f  gZ.Lake_Cat_seg_
-00007cd0: 696e 666f da0b 7365 675f 7375 625f 6964  info..seg_sub_id
-00007ce0: 7372 b700 0000 da08 695f 7365 675f 6964  sr......i_seg_id
-00007cf0: da0a 695f 7365 675f 696e 666f 5a08 7375  ..i_seg_infoZ.su
-00007d00: 6d5f 6172 6561 72a1 0000 00da 0669 6f72  m_arear......ior
-00007d10: 6465 725a 0d69 6f72 6465 725f 4c61 6b65  derZ.iorder_Lake
-00007d20: 6964 5a08 636f 6e5f 6c61 6b65 5a09 636f  idZ.con_lakeZ.co
-00007d30: 6e5f 6761 7567 655a 0863 6f6e 5f61 7265  n_gaugeZ.con_are
-00007d40: 615a 0d63 6f6e 5f61 7265 615f 6c61 6b65  aZ.con_area_lake
-00007d50: 5a0b 636f 6e5f 6c61 6b65 5f75 705a 0d63  Z.con_lake_upZ.c
-00007d60: 6f6e 5f6c 616b 655f 646f 776e 5a07 6973  on_lake_downZ.is
-00007d70: 5f6c 616b 6572 cb00 0000 5a13 7375 6269  _laker....Z.subi
-00007d80: 645f 6375 725f 6c61 6b65 5f69 6e66 6f5a  d_cur_lake_infoZ
-00007d90: 1172 6f75 7469 6e67 5f69 6e66 6f5f 6c61  .routing_info_la
-00007da0: 6b65 5a0f 5570 7374 7265 616d 4c61 6b65  keZ.UpstreamLake
-00007db0: 6964 735a 1541 6c6c 5f75 705f 7375 6269  idsZ.All_up_subi
-00007dc0: 6473 5f6e 6f5f 6d61 696e 5a10 6d61 736b  ds_no_mainZ.mask
-00007dd0: 5f6f 6c64 5f6e 6f6e 4c61 6b65 7224 0000  _old_nonLaker$..
-00007de0: 0072 2400 0000 7225 0000 00da 4743 6861  .r$...r%....GCha
-00007df0: 6e67 655f 4174 7472 6962 7574 655f 5661  nge_Attribute_Va
-00007e00: 6c75 6573 5f46 6f72 5f43 6174 6368 6d65  lues_For_Catchme
-00007e10: 6e74 735f 4e65 6564 5f54 6f5f 4265 5f4d  nts_Need_To_Be_M
-00007e20: 6572 6765 645f 4279 5f49 6e63 7265 6173  erged_By_Increas
-00007e30: 655f 4441 4d07 0000 7362 0200 0000 0d04  e_DAM...sb......
-00007e40: 0104 0104 0104 0204 010a 0104 070c 0108  ................
-00007e50: 0108 010e 0110 0310 0110 0108 0108 0404  ................
-00007e60: 0112 ff08 050c 0104 0106 ff06 0316 010a  ................
-00007e70: 0310 0102 ff06 0304 010a ff04 0304 010c  ................
-00007e80: ff08 030a 0504 010e 010a ff02 ff04 0302  ................
-00007e90: fd06 0418 020c 020e 010c 010c 0124 011a  .............$..
-00007ea0: 040a 010c 0112 0104 010c 010c ff02 ff08  ................
-00007eb0: 0a10 0102 ff06 0304 010a ff04 0310 0102  ................
-00007ec0: ff06 0304 010a ff04 0504 0102 ff04 0314  ................
-00007ed0: 010a 010a 0304 010a ff02 0202 fe18 0614  ................
-00007ee0: 0106 ff02 ff02 0408 0204 010c ff06 0618  ................
-00007ef0: 0212 011c 010e 010a 0202 0102 0102 0102  ................
-00007f00: 0102 0102 0102 0102 f90a 0d14 0104 0116  ................
-00007f10: ff04 040e 0110 0110 0104 0112 0208 0104  ................
-00007f20: 010a ff08 0310 010e 020a 010c 020c 010e  ................
-00007f30: 0202 0102 ff02 0206 fe08 050a 0202 0102  ................
-00007f40: 0102 0102 0102 0102 0102 0102 f90a 0b14  ................
-00007f50: 0208 0116 0110 0104 0104 0104 0114 010e  ................
-00007f60: 010e 010a 0104 0116 ff04 0312 0412 0122  ..............."
-00007f70: 0204 0212 0312 0118 0106 0212 0210 0308  ................
-00007f80: 021c 0220 0220 0212 0204 021c 0204 0220  ... . ......... 
-00007f90: 0212 0204 0226 0204 0220 0212 050e 0204  .....&... ......
-00007fa0: 020c 020c ff04 010e ff02 030c ff04 010e  ................
-00007fb0: ff02 030c ff04 010e ff02 030c ff04 010e  ................
-00007fc0: ff02 030c ff04 010e ff02 030c ff04 010e  ................
-00007fd0: ff02 0312 0104 0104 0104 0712 0104 010a  ................
-00007fe0: 020a 0104 010a ff08 040c 0102 ff04 ff02  ................
-00007ff0: 050a 0104 010c ff04 030c 030a 010c 0104  ................
-00008000: 0104 ff04 030e 0204 010c ff04 030c 010c  ................
-00008010: 010e 020c 010e 0202 0102 0102 0102 0102  ................
-00008020: 0102 0102 0102 0102 f806 0b04 010c 021e  ................
-00008030: 0108 0212 0108 0304 010a 020a 0104 010a  ................
-00008040: ff08 040c 0102 ff04 ff02 050a 0104 010c  ................
-00008050: ff04 030c 020a 010c 0104 0104 ff04 030e  ................
-00008060: 0204 010c ff04 030c 010c 010e 020c 010e  ................
-00008070: 0302 0102 0102 0102 0102 0102 0102 0102  ................
-00008080: 0102 f806 0a04 0110 0216 0116 0116 0116  ................
-00008090: 0116 0116 0302 0102 0102 0102 0102 fb72  ...............r
-000080a0: ef00 0000 6304 0000 0000 0000 0000 0000  ....c...........
-000080b0: 0016 0000 0007 0000 0043 0000 0073 0002  .........C...s..
-000080c0: 0000 7c00 6401 1900 a000 7401 a101 7c00  ..|.d.....t...|.
-000080d0: 6401 3c00 7c00 6402 1900 a000 7402 a101  d.<.|.d.....t...
-000080e0: 7c00 6402 3c00 7c00 6403 1900 a000 7402  |.d.<.|.d.....t.
-000080f0: a101 7c00 6403 3c00 7c00 6a03 7c00 6404  ..|.d.<.|.j.|.d.
-00008100: 1900 6405 6b02 1900 6a04 6406 6407 8d01  ..d.k...j.d.d...
-00008110: 7d04 7c00 6a03 7c00 6404 1900 6408 6b02  }.|.j.|.d...d.k.
-00008120: 1900 6a04 6406 6407 8d01 7d05 6409 7c00  ..j.d.d...}.d.|.
-00008130: 6a05 7600 727a 6409 7d06 6e04 640a 7d06  j.v.rzd.}.n.d.}.
-00008140: 7c05 6401 1900 7c01 6b05 7d07 7c05 7c06  |.d...|.k.}.|.|.
-00008150: 1900 6408 6b02 7d08 7406 a007 7c07 7c08  ..d.k.}.t...|.|.
-00008160: a102 7d09 7c05 6a03 7c09 1900 6402 1900  ..}.|.j.|...d...
-00008170: 6a08 7d0a 7c0a 7c0a 640b 6b04 1900 7d0a  j.}.|.|.d.k...}.
-00008180: 7406 a009 7c0a a101 7d0a 7c04 6401 1900  t...|...}.|.d...
-00008190: 7c02 6b05 7d07 7c04 7c06 1900 6408 6b02  |.k.}.|.|...d.k.
-000081a0: 7d08 7406 a007 7c07 7c08 a102 7d09 7c04  }.t...|.|...}.|.
-000081b0: 7c09 1900 6402 1900 6a08 7d0b 7c0b 7c0b  |...d...j.}.|.|.
-000081c0: 640b 6b04 1900 7d0b 7406 a009 7c0b a101  d.k...}.t...|...
-000081d0: 7d0b 740a 7c03 8301 640b 6b04 9001 7224  }.t.|...d.k...r$
-000081e0: 7c03 7d0c 6e06 640c 6701 7d0c 7c05 6402  |.}.n.d.g.}.|.d.
-000081f0: 1900 6a08 7d0d 7c04 6402 1900 6a08 7d0e  ..j.}.|.d...j.}.
-00008200: 7406 a00b 7c0c a101 7d0f 7406 a00c 7c0d  t...|...}.t...|.
-00008210: 7c0f a102 7d10 7406 a00c 7c0e 7c0f a102  |...}.t...|.|...
-00008220: 7d11 7c0d 7c10 1900 7d12 7406 a009 7c12  }.|.|...}.t...|.
-00008230: a101 7d12 7c0e 7c11 1900 7d13 7406 a009  ..}.|.|...}.t...
-00008240: 7c13 a101 7d13 7406 6a0d 7c0b 7c13 6602  |...}.t.j.|.|.f.
-00008250: 640b 640d 8d02 7d0b 7406 6a0d 7c0a 7c12  d.d...}.t.j.|.|.
-00008260: 6602 640b 640d 8d02 7d0a 7c00 6a03 7c00  f.d.d...}.|.j.|.
-00008270: 6404 1900 6408 6b02 7406 a00e 7c00 6402  d...d.k.t...|.d.
-00008280: 1900 a00f 7c0a a101 a101 4000 1900 7d14  ....|.....@...}.
-00008290: 7c00 6a03 7c00 6404 1900 6405 6b02 7406  |.j.|.d...d.k.t.
-000082a0: a00e 7c00 6402 1900 a00f 7c0b a101 a101  ..|.d.....|.....
-000082b0: 4000 1900 7d15 7c0b 7c0a 7c14 7c15 6604  @...}.|.|.|.|.f.
-000082c0: 5300 290e 7a80 5265 7472 756e 2073 656c  S.).z.Retrun sel
-000082d0: 6563 7465 6420 6c61 6b65 2773 2061 7474  ected lake's att
-000082e0: 7269 6275 7465 2074 6162 6c65 2061 6e64  ribute table and
-000082f0: 2049 440a 2020 2020 2d2d 2d2d 2d2d 2d2d   ID.    --------
-00008300: 2d2d 0a0a 2020 2020 4e6f 7465 730a 2020  --..    Notes.  
-00008310: 2020 2d2d 2d2d 2d2d 2d0a 0a20 2020 2052    -------..    R
-00008320: 6574 7572 6e73 3a0a 2020 2020 2d2d 2d2d  eturns:.    ----
-00008330: 2d2d 2d0a 2020 2020 2020 2020 4e6f 6e65  ---.        None
-00008340: 2c0a 2020 2020 7295 0000 0072 8400 0000  ,.    r....r....
-00008350: 7266 0000 0072 6400 0000 7265 0000 0054  rf...rd...re...T
-00008360: 7207 0000 0072 2800 0000 7280 0000 0072  r....r(...r....r
-00008370: 8100 0000 7201 0000 0069 8169 67ff 720e  ....r....i.ig.r.
-00008380: 0000 0029 1072 1600 0000 7263 0000 0072  ...).r....rc...r
-00008390: 2d00 0000 7219 0000 0072 1400 0000 7211  -...r....r....r.
-000083a0: 0000 0072 1a00 0000 7289 0000 0072 1300  ...r....r....r..
-000083b0: 0000 722b 0000 0072 1500 0000 da05 6172  ..r+...r......ar
-000083c0: 7261 7972 2e00 0000 721b 0000 0072 9a00  rayr....r....r..
-000083d0: 0000 7212 0000 0029 16da 0d66 696e 616c  ..r....)...final
-000083e0: 6361 745f 696e 666f da15 5468 7265 735f  cat_info..Thres_
-000083f0: 4172 6561 5f43 6f6e 6e5f 4c61 6b65 73da  Area_Conn_Lakes.
-00008400: 1954 6872 6573 5f41 7265 615f 4e6f 6e5f  .Thres_Area_Non_
-00008410: 436f 6e6e 5f4c 616b 6573 da15 5365 6c65  Conn_Lakes..Sele
-00008420: 6374 6564 5f4c 616b 655f 4c69 7374 5f69  cted_Lake_List_i
-00008430: 6e5a 0e4e 6f6e 5f43 6f6e 6e4c 5f69 6e66  nZ.Non_ConnL_inf
-00008440: 6f5a 0a43 6f6e 6e4c 5f69 6e66 6f72 8c00  oZ.ConnL_infor..
-00008450: 0000 724a 0000 0072 4b00 0000 7223 0000  ..rJ...rK...r#..
-00008460: 005a 1253 656c 6563 7465 645f 436f 6e6e  .Z.Selected_Conn
-00008470: 4c61 6b65 735a 1653 656c 6563 7465 645f  LakesZ.Selected_
-00008480: 4e6f 6e5f 436f 6e6e 4c61 6b65 735a 1253  Non_ConnLakesZ.S
-00008490: 656c 6563 7465 645f 4c61 6b65 5f4c 6973  elected_Lake_Lis
-000084a0: 745a 0941 6c6c 5f43 6f6e 6e4c 5a0d 416c  tZ.All_ConnLZ.Al
-000084b0: 6c5f 4e6f 6e5f 436f 6e6e 4c5a 1b53 656c  l_Non_ConnLZ.Sel
-000084c0: 6563 7465 645f 4c61 6b65 5f4c 6973 745f  ected_Lake_List_
-000084d0: 696e 5f61 7272 6179 5a07 6d61 736b 5f43  in_arrayZ.mask_C
-000084e0: 4c5a 086d 6173 6b5f 4e43 4c5a 1753 656c  LZ.mask_NCLZ.Sel
-000084f0: 6563 7465 645f 436f 6e6e 4c61 6b65 735f  ected_ConnLakes_
-00008500: 4c69 7374 5a1b 5365 6c65 6374 6564 5f4e  ListZ.Selected_N
-00008510: 6f6e 5f43 6f6e 6e4c 616b 6573 5f4c 6973  on_ConnLakes_Lis
-00008520: 74da 1a55 6e5f 5365 6c65 6374 6564 5f43  t..Un_Selected_C
-00008530: 6f6e 6e4c 616b 6573 5f69 6e66 6fda 1a55  onnLakes_info..U
-00008540: 6e5f 5365 6c65 6374 6564 5f4e 6f6e 5f43  n_Selected_Non_C
-00008550: 6f6e 6e4c 5f69 6e66 6f72 2400 0000 7224  onnL_infor$...r$
-00008560: 0000 0072 2500 0000 da2c 5265 7475 726e  ...r%....,Return
-00008570: 5f53 656c 6563 7465 645f 4c61 6b65 735f  _Selected_Lakes_
-00008580: 4174 7472 6962 7574 655f 5461 626c 655f  Attribute_Table_
-00008590: 416e 645f 4964 ef08 0000 7372 0000 0000  And_Id....sr....
-000085a0: 1012 0112 0112 021a 011a 020a 0106 0204  ................
-000085b0: 030c 010c 010c 0104 0102 ff02 0202 fe06  ................
-000085c0: 040c 010a 030c 010c 010c 0202 0102 ff02  ................
-000085d0: 0202 fe06 030c 010a 040e 0106 0306 010a  ................
-000085e0: 010a 010a 020c 010c 0208 010a 0108 010a  ................
-000085f0: 0312 0112 0204 010a 0112 ff02 ff04 0404  ................
-00008600: 010a 0112 ff02 ff04 0602 0102 0102 0102  ................
-00008610: fc72 f700 0000 6302 0000 0000 0000 0000  .r....c.........
-00008620: 0000 000e 0000 000c 0000 0043 0000 0073  ...........C...s
-00008630: 2202 0000 7c00 6a00 6401 6402 8d01 7d02  "...|.j.d.d...}.
-00008640: 6403 7c02 6404 3c00 6403 7c02 6405 3c00  d.|.d.<.d.|.d.<.
-00008650: 7c02 6406 1900 7c02 6407 3c00 7c02 6a01  |.d...|.d.<.|.j.
-00008660: 6401 6401 6408 8d02 0100 6409 7d03 6409  d.d.d.....d.}.d.
-00008670: 7c02 6a02 7601 7248 640a 7d03 7c01 640b  |.j.v.rHd.}.|.d.
-00008680: 1900 6a03 7d04 7404 a005 7c04 a101 7d04  ..j.}.t...|...}.
-00008690: 7406 640c 7407 7c04 8301 8302 4400 9001  t.d.t.|.....D...
-000086a0: 5db0 7d05 7c04 7c05 1900 7d06 7c00 6a08  ].}.|.|...}.|.j.
-000086b0: 7c00 640b 1900 7c06 6b02 7c00 640d 1900  |.d...|.k.|.d...
-000086c0: 640e 6b03 4000 1900 a000 a100 7d07 7c07  d.k.@.......}.|.
-000086d0: 6a09 640f 6701 6401 6410 8d02 7d07 7404  j.d.g.d.d...}.t.
-000086e0: a005 7c07 6411 1900 6a03 a101 7d08 7407  ..|.d...j...}.t.
-000086f0: 7c07 8301 7407 7c08 8301 6b02 72cc 716a  |...t.|...k.r.qj
-00008700: 7404 a00a 7c08 a101 9001 7226 7404 a00a  t...|.....r&t...
-00008710: 7c07 7c03 1900 6a03 a101 640c 6b01 9001  |.|...j...d.k...
-00008720: 7226 7c07 6406 1900 6a03 7407 7c07 8301  r&|.d...j.t.|...
-00008730: 6412 1800 1900 7d09 7c07 6406 1900 6a03  d.....}.|.d...j.
-00008740: 7d0a 740b 7c09 7c00 7c02 6412 7c0a 7c00  }.t.|.|.|.d.|.|.
-00008750: 6403 6412 6413 8d08 7d02 6700 7d0b 6412  d.d.d...}.g.}.d.
-00008760: 7d0c 7406 640c 7407 7c07 8301 8302 4400  }.t.d.t.|.....D.
-00008770: 5dde 7d0d 7c07 6406 1900 6a03 7c0d 1900  ].}.|.d...j.|...
-00008780: 7d09 7c0b a00c 7c09 a101 0100 7c0d 7407  }.|...|.....|.t.
-00008790: 7c07 8301 6412 1800 6b02 9001 72a4 7404  |...d...k...r.t.
-000087a0: a00d 7c0b a101 7d0a 740b 7c09 7c00 7c02  ..|...}.t.|.|.|.
-000087b0: 6412 7c0a 7c00 7c07 6411 1900 6a03 7c0d  d.|.|.|.d...j.|.
-000087c0: 1900 7c0c 6413 8d08 7d02 6700 7d0b 7c0c  ..|.d...}.g.}.|.
-000087d0: 6412 1700 7d0c 6e74 7c07 6411 1900 6a03  d...}.nt|.d...j.
-000087e0: 7c0d 1900 7c07 6411 1900 6a03 7c0d 6412  |...|.d...j.|.d.
-000087f0: 1700 1900 6b02 9001 72e0 7c07 7c03 1900  ....k...r.|.|...
-00008800: 6a03 7c0d 1900 640c 6b01 9001 72e0 9001  j.|...d.k...r...
-00008810: 713c 6e38 7404 a00d 7c0b a101 7d0a 740b  q<n8t...|...}.t.
-00008820: 7c09 7c00 7c02 6412 7c0a 7c00 7c07 6411  |.|.|.d.|.|.|.d.
-00008830: 1900 6a03 7c0d 1900 7c0c 6413 8d08 7d02  ..j.|...|.d...}.
-00008840: 6700 7d0b 7c0c 6412 1700 7d0c 9001 713c  g.}.|.d...}...q<
-00008850: 716a 7c02 5300 2914 7ab1 4368 616e 6765  qj|.S.).z.Change
-00008860: 2061 7474 7269 6275 7465 7320 666f 7220   attributes for 
-00008870: 6361 7463 686d 656e 7473 2074 6861 7420  catchments that 
-00008880: 6e65 6564 7320 746f 2062 6520 6d65 7267  needs to be merg
-00008890: 6564 2064 7565 2074 6f20 7265 6d6f 7665  ed due to remove
-000088a0: 0a20 2020 2020 2020 2063 6f6e 6e65 6374  .        connect
-000088b0: 6564 206c 616b 6573 0a20 2020 202d 2d2d  ed lakes.    ---
-000088c0: 2d2d 2d2d 2d2d 2d0a 0a20 2020 204e 6f74  -------..    Not
-000088d0: 6573 0a20 2020 202d 2d2d 2d2d 2d2d 0a0a  es.    -------..
-000088e0: 2020 2020 5265 7475 726e 733a 0a20 2020      Returns:.   
-000088f0: 202d 2d2d 2d2d 2d2d 0a20 2020 2020 2020   -------.       
-00008900: 204e 6f6e 652c 0a20 2020 2054 7207 0000   None,.    Tr...
-00008910: 0072 6b00 0000 7283 0000 0072 8500 0000  .rk...r....r....
-00008920: 7206 0000 00da 076e 7375 6269 6432 72df  r......nsubid2r.
-00008930: 0000 0072 8000 0000 7281 0000 0072 6600  ...r....r....rf.
-00008940: 0000 7201 0000 0072 6400 0000 7265 0000  ..r....rd...re..
-00008950: 0072 6a00 0000 727a 0000 0072 8400 0000  .rj...rz...r....
-00008960: 7228 0000 0072 e200 0000 290e 7214 0000  r(...r....).r...
-00008970: 0072 e300 0000 7211 0000 0072 1300 0000  .r....r....r....
-00008980: 721a 0000 0072 2b00 0000 7229 0000 0072  r....r+...r)...r
-00008990: 1500 0000 7219 0000 0072 4100 0000 7274  ....r....rA...rt
-000089a0: 0000 0072 a300 0000 724e 0000 0072 e500  ...r....rN...r..
-000089b0: 0000 290e da12 6669 6e61 6c63 6174 5f69  ..)...finalcat_i
-000089c0: 6e66 6f5f 7465 6d70 72f5 0000 0072 8a00  nfo_tempr....r..
-000089d0: 0000 728c 0000 0072 e800 0000 72b7 0000  ..r....r....r...
-000089e0: 0072 ec00 0000 72ed 0000 005a 0a4e 5f48  .r....r....Z.N_H
-000089f0: 796c 616b 6569 6472 e900 0000 72eb 0000  ylakeidr....r...
-00008a00: 0072 ea00 0000 72a1 0000 0072 ee00 0000  .r....r....r....
-00008a10: 7224 0000 0072 2400 0000 7225 0000 00da  r$...r$...r%....
-00008a20: 4543 6861 6e67 655f 4174 7472 6962 7574  EChange_Attribut
-00008a30: 655f 5661 6c75 6573 5f46 6f72 5f43 6174  e_Values_For_Cat
-00008a40: 6368 6d65 6e74 735f 4e65 6564 5f54 6f5f  chments_Need_To_
-00008a50: 4265 5f4d 6572 6765 645f 4279 5f52 656d  Be_Merged_By_Rem
-00008a60: 6f76 655f 434c 4909 0000 7394 0000 0000  ove_CLI...s.....
-00008a70: 0e0c 0108 0108 010c 010e 0304 010a 0104  ................
-00008a80: 030a 010a 0114 0208 0104 010a 010a ff02  ................
-00008a90: ff08 0410 0310 0110 0102 0322 0116 010a  ..........."....
-00008aa0: 0102 0102 0102 0102 0102 0102 0102 0102  ................
-00008ab0: 0102 f806 0c04 0104 0112 010e 010a 0312  ................
-00008ac0: 010a 0102 0102 0102 0102 0102 0102 0102  ................
-00008ad0: 010c 0102 f806 0a04 010a 030c 0110 ff02  ................
-00008ae0: ff04 0310 fd04 0506 020a 0102 0102 0102  ................
-00008af0: 0102 0102 0102 0102 010c 0102 f806 0a04  ................
-00008b00: 010e 0172 fa00 0000 6303 0000 0000 0000  ...r....c.......
-00008b10: 0000 0000 000f 0000 000a 0000 0043 0000  .............C..
-00008b20: 0073 0002 0000 7c02 6a00 6401 6701 6402  .s....|.j.d.g.d.
-00008b30: 6701 6403 8d02 7d02 7401 6404 7402 7c02  g.d...}.t.d.t.|.
-00008b40: 8301 8302 4400 9001 5da4 7d03 7c02 6405  ....D...].}.|.d.
-00008b50: 1900 6a03 7c03 1900 7d04 7c01 6a04 7c01  ..j.|...}.|.j.|.
-00008b60: 6405 1900 7c04 6b02 1900 a005 a100 7d05  d...|.k.......}.
-00008b70: 7402 7c05 8301 6406 6b03 7268 7406 6407  t.|...d.k.rht.d.
-00008b80: 8301 0100 7406 7c05 8301 0100 7120 6700  ....t.|.....q g.
-00008b90: 7d06 7c05 6408 1900 6a03 6404 1900 7d07  }.|.d...j.d...}.
-00008ba0: 7c05 6409 1900 6a03 6404 1900 7d08 7c06  |.d...j.d...}.|.
-00008bb0: a007 7c07 a101 0100 640a 7d09 6404 7d0a  ..|.....d.}.d.}.
-00008bc0: 7c01 6a04 7c01 6408 1900 7c08 6b02 1900  |.j.|.d...|.k...
-00008bd0: a005 a100 7d0b 7402 7c0b 8301 6404 6b02  ....}.t.|...d.k.
-00008be0: 72c6 7c08 6404 6b00 72c6 7120 7c0b 640b  r.|.d.k.r.q |.d.
-00008bf0: 1900 6a03 6404 1900 640c 6b03 9001 7228  ..j.d...d.k...r(
-00008c00: 7c00 6a04 7c00 6408 1900 7c08 6b02 1900  |.j.|.d...|.k...
-00008c10: 640d 1900 6a03 6404 1900 7d0c 7c0c 6404  d...j.d...}.|.d.
-00008c20: 6b04 9001 7214 7c0c 7d09 6406 7d0a 7c06  k...r.|.}.d.}.|.
-00008c30: a007 7c09 a101 0100 6e12 7c08 7d09 640a  ..|.....n.|.}.d.
-00008c40: 7d0a 7c06 a007 7c09 a101 0100 6e4c 7c00  }.|...|.....nL|.
-00008c50: 6a04 7c00 6408 1900 7c08 6b02 1900 640d  j.|.d...|.k...d.
-00008c60: 1900 6a03 6404 1900 7d0c 7c0c 6404 6b04  ..j.d...}.|.d.k.
-00008c70: 9001 7262 7c0c 7d09 6406 7d0a 7c06 a007  ..rb|.}.d.}.|...
-00008c80: 7c09 a101 0100 6e12 7c08 7d09 640a 7d0a  |.....n.|.}.d.}.
-00008c90: 7c06 a007 7c09 a101 0100 7c00 7c00 6408  |...|.....|.|.d.
-00008ca0: 1900 7c09 6b02 1900 6405 1900 6a03 6404  ..|.k...d...j.d.
-00008cb0: 1900 7d0d 7c0a 6404 6b04 9001 72b0 7408  ..}.|.d.k...r.t.
-00008cc0: 7c09 7c00 7c00 6406 7c06 7c01 7c0d 640e  |.|.|.d.|.|.|.d.
-00008cd0: 8d07 7d00 7120 7408 7c09 7c00 7c00 6406  ..}.q t.|.|.|.d.
-00008ce0: 7c06 7c01 7c0d 640e 8d07 7d00 7120 7c00  |.|.|.d...}.q |.
-00008cf0: 640d 1900 6404 6b01 7d0e 7c00 6a04 7c0e  d...d.k.}.|.j.|.
-00008d00: 640f 6602 1900 6a03 7c00 6a04 7c0e 640d  d.f...j.|.j.|.d.
-00008d10: 6602 3c00 7c00 6a09 640f 6701 6410 8d01  f.<.|.j.d.g.d...
-00008d20: 0100 7c00 5300 2911 7ab5 4368 616e 6765  ..|.S.).z.Change
-00008d30: 2061 7474 7269 6275 7465 7320 666f 7220   attributes for 
-00008d40: 6361 7463 686d 656e 7473 2074 6861 7420  catchments that 
-00008d50: 6e65 6564 7320 746f 2062 6520 6d65 7267  needs to be merg
-00008d60: 6564 2064 7565 2074 6f20 7265 6d6f 7665  ed due to remove
-00008d70: 0a20 2020 2020 2020 206e 6f6e 2063 6f6e  .        non con
-00008d80: 6e65 6374 6564 206c 616b 6573 0a20 2020  nected lakes.   
-00008d90: 202d 2d2d 2d2d 2d2d 2d2d 2d0a 0a20 2020   ----------..   
-00008da0: 204e 6f74 6573 0a20 2020 202d 2d2d 2d2d   Notes.    -----
-00008db0: 2d2d 0a0a 2020 2020 5265 7475 726e 733a  --..    Returns:
-00008dc0: 0a20 2020 202d 2d2d 2d2d 2d2d 0a20 2020  .    -------.   
-00008dd0: 2020 2020 204e 6f6e 652c 0a20 2020 2072       None,.    r
-00008de0: 7900 0000 4672 7a00 0000 7201 0000 0072  y...Frz...r....r
-00008df0: 8400 0000 7228 0000 007a 2849 7420 6973  ....r(...z(It is
-00008e00: 206e 6f74 2061 206e 6f6e 2063 6f6e 6e65   not a non conne
-00008e10: 6374 6564 206c 616b 6520 6361 7463 686d  cted lake catchm
-00008e20: 656e 7472 0600 0000 720d 0000 0072 6b00  entr....r....rk.
-00008e30: 0000 7264 0000 0072 6500 0000 7283 0000  ..rd...re...r...
-00008e40: 00a9 0772 4900 0000 729d 0000 0072 8a00  ...rI...r....r..
-00008e50: 0000 729e 0000 0072 9f00 0000 72a0 0000  ..r....r....r...
-00008e60: 0072 6400 0000 72f8 0000 0072 1000 0000  .rd...r....r....
-00008e70: 290a 7241 0000 0072 2900 0000 7215 0000  ).rA...r)...r...
-00008e80: 0072 1300 0000 7219 0000 0072 1400 0000  .r....r....r....
-00008e90: 7275 0000 0072 4e00 0000 72a3 0000 0072  ru...rN...r....r
-00008ea0: 1c00 0000 290f 728a 0000 0072 f900 0000  ....).r....r....
-00008eb0: 72f6 0000 0072 4800 0000 5a17 5265 6d6f  r....rH...Z.Remo
-00008ec0: 7665 5f4e 6f6e 5f43 6f6e 6e4c 5f4c 616b  ve_Non_ConnL_Lak
-00008ed0: 6569 645a 1e52 656d 6f76 655f 4e6f 6e5f  eidZ.Remove_Non_
-00008ee0: 436f 6e6e 4c5f 4c61 6b65 5f53 7562 5f69  ConnL_Lake_Sub_i
-00008ef0: 6e66 6f72 ea00 0000 72cc 0000 0072 cb00  nfor....r....r..
-00008f00: 0000 72e9 0000 005a 0f69 735f 7072 655f  ..r....Z.is_pre_
-00008f10: 6d6f 6469 6669 6564 72c6 0000 0072 8300  modifiedr....r..
-00008f20: 0000 5a0b 5461 725f 4c61 6b65 5f49 645a  ..Z.Tar_Lake_IdZ
-00008f30: 0f75 6e70 726f 6365 7373 6564 6d61 736b  .unprocessedmask
-00008f40: 7224 0000 0072 2400 0000 7225 0000 00da  r$...r$...r%....
-00008f50: 4643 6861 6e67 655f 4174 7472 6962 7574  FChange_Attribut
-00008f60: 655f 5661 6c75 6573 5f46 6f72 5f43 6174  e_Values_For_Cat
-00008f70: 6368 6d65 6e74 735f 4e65 6564 5f54 6f5f  chments_Need_To_
-00008f80: 4265 5f4d 6572 6765 645f 4279 5f52 656d  Be_Merged_By_Rem
-00008f90: 6f76 655f 4e43 4cb0 0900 0073 a400 0000  ove_NCL....s....
-00008fa0: 000f 0401 08ff 0603 1401 0801 02ff 0403  ................
-00008fb0: 0401 0aff 0803 0c01 0801 0801 0201 0401  ................
-00008fc0: 0e01 0801 02ff 0403 0a01 0401 0402 0401  ................
-00008fd0: 0aff 0803 1401 0201 1402 1001 02ff 0403  ................
-00008fe0: 02fd 0406 0a01 0401 0401 0c02 0401 0401  ................
-00008ff0: 0c04 1001 02ff 0402 02fe 0403 0a01 0401  ................
-00009000: 0401 0c02 0402 0401 0a02 0e01 02ff 0402  ................
-00009010: 02fe 0404 0a01 0201 0201 0201 0201 0201  ................
-00009020: 0201 0201 02f9 080a 0201 0201 0201 0201  ................
-00009030: 0201 0201 0201 02f9 080a 0c02 0401 06ff  ................
-00009040: 1004 0e02 72fc 0000 0063 0100 0000 0000  ....r....c......
-00009050: 0000 0000 0000 0900 0000 0a00 0000 4300  ..............C.
-00009060: 0000 73cc 0000 0064 017d 017c 006a 0064  ..s....d.}.|.j.d
-00009070: 0264 038d 017d 027c 0264 0119 006a 017c  .d...}.|.d...j.|
-00009080: 0264 043c 007c 0264 0419 00a0 0264 05a1  .d.<.|.d.....d..
-00009090: 017c 0264 043c 007c 0064 0619 006a 017d  .|.d.<.|.d...j.}
-000090a0: 037c 037c 0364 076b 0419 007d 0374 03a0  .|.|.d.k...}.t..
-000090b0: 047c 03a1 017d 0374 0564 0774 067c 0383  .|...}.t.d.t.|..
-000090c0: 0183 0244 005d 687d 047c 037c 0419 007d  ...D.]h}.|.|...}
-000090d0: 057c 006a 077c 0064 0619 007c 056b 0219  .|.j.|.d...|.k..
-000090e0: 007d 067c 066a 0864 0867 0164 0964 0a8d  .}.|.j.d.g.d.d..
-000090f0: 027d 067c 067c 0119 006a 0164 0719 007d  .}.|.|...j.d...}
-00009100: 077c 067c 0119 006a 017d 0874 067c 0883  .|.|...j.}.t.|..
-00009110: 0164 0b6b 0472 5e74 097c 077c 007c 0264  .d.k.r^t.|.|.|.d
-00009120: 0b7c 087c 0064 0b64 0c8d 077d 0271 5e7c  .|.|.d.d...}.q^|
-00009130: 0253 0029 0de1 2c01 0000 4368 616e 6765  .S.)..,...Change
-00009140: 2061 7474 7269 6275 7465 7320 666f 7220   attributes for 
-00009150: 6361 7463 686d 656e 7473 2074 6861 7420  catchments that 
-00009160: 636f 7665 7265 6420 6279 2074 6865 2073  covered by the s
-00009170: 616d 6520 6c61 6b65 2e0a 2020 2020 2d2d  ame lake..    --
-00009180: 2d2d 2d2d 2d2d 2d2d 0a0a 2020 2020 4e6f  --------..    No
-00009190: 7465 730a 2020 2020 2d2d 2d2d 2d2d 2d0a  tes.    -------.
-000091a0: 2020 2020 2020 2020 466f 7220 6578 616d          For exam
-000091b0: 706c 652c 206c 616b 6520 276c 6127 2063  ple, lake 'la' c
-000091c0: 6f76 6572 696e 6720 6361 7463 686d 656e  overing catchmen
-000091d0: 7420 612c 622c 632e 2074 6865 206c 616b  t a,b,c. the lak
-000091e0: 6520 6f75 746c 6574 2063 6174 6368 6d65  e outlet catchme
-000091f0: 6e74 0a20 2020 2020 2020 2069 7320 612e  nt.        is a.
-00009200: 2074 6865 6e20 7468 6973 2066 756e 6374   then this funct
-00009210: 696f 6e20 7769 6c6c 2063 6861 6e67 6520  ion will change 
-00009220: 6174 7472 6962 7574 6520 6f66 2062 2061  attribute of b a
-00009230: 6e64 2063 2074 6f20 612e 0a20 2020 2052  nd c to a..    R
-00009240: 6574 7572 6e73 3a0a 2020 2020 2d2d 2d2d  eturns:.    ----
-00009250: 2d2d 2d0a 2020 2020 2020 2020 4e6f 6e65  ---.        None
-00009260: 2c0a 2020 2020 7206 0000 0054 7207 0000  ,.    r....Tr...
-00009270: 0072 8300 0000 7209 0000 0072 8400 0000  .r....r....r....
-00009280: 7201 0000 0072 7900 0000 4672 7a00 0000  r....ry...Frz...
-00009290: 7228 0000 0072 fb00 0000 290a 7214 0000  r(...r....).r...
-000092a0: 0072 1300 0000 7216 0000 0072 1a00 0000  .r....r....r....
-000092b0: 722b 0000 0072 2900 0000 7215 0000 0072  r+...r)...r....r
-000092c0: 1900 0000 7241 0000 0072 a300 0000 a909  ....rA...r......
-000092d0: 5a10 6669 6e61 6c72 6976 706c 795f 696e  Z.finalrivply_in
-000092e0: 666f 72a2 0000 0072 8a00 0000 5a11 416c  for....r....Z.Al
-000092f0: 6c43 6f6e 6e65 6374 4c61 6b65 4944 5372  lConnectLakeIDSr
-00009300: 4800 0000 5a06 6c61 6b65 6964 5a0c 4c61  H...Z.lakeidZ.La
-00009310: 6b65 7375 625f 696e 666f 72e9 0000 005a  kesub_infor....Z
-00009320: 0a6c 616b 6573 7562 6964 7372 2400 0000  .lakesubidsr$...
-00009330: 7224 0000 0072 2500 0000 da3b 4368 616e  r$...r%....;Chan
-00009340: 6765 5f41 7474 7269 6275 7465 5f56 616c  ge_Attribute_Val
-00009350: 7565 735f 466f 725f 4361 7463 686d 656e  ues_For_Catchmen
-00009360: 7473 5f43 6f76 6572 6564 5f42 795f 5361  ts_Covered_By_Sa
-00009370: 6d65 5f4c 616b 651f 0a00 0073 3400 0000  me_Lake....s4...
-00009380: 000d 0401 0c01 0e01 1201 0a01 0c01 0a03  ................
-00009390: 1201 0801 1201 1001 0801 02ff 0403 0a01  ................
-000093a0: 0c01 0201 0201 0201 0201 0201 0201 0201  ................
-000093b0: 02f9 0809 72ff 0000 0063 0300 0000 0000  ....r....c......
-000093c0: 0000 0000 0000 0800 0000 0600 0000 4300  ..............C.
-000093d0: 0000 7368 0000 0074 007c 007c 0183 027d  ..sh...t.|.|...}
-000093e0: 037c 0264 016b 0472 6074 007c 007c 0283  .|.d.k.r`t.|.|..
-000093f0: 027d 0474 0174 027c 0483 0183 0144 005d  .}.t.t.|.....D.]
-00009400: 307d 057c 047c 0519 007c 026b 0272 3a71  0}.|.|...|.k.r:q
-00009410: 2874 03a0 047c 037c 047c 0519 006b 02a1  (t...|.|.|...k..
-00009420: 017d 0674 03a0 057c 037c 06a1 027d 0371  .}.t...|.|...}.q
-00009430: 287c 037d 076e 047c 037d 077c 0753 0029  (|.}.n.|.}.|.S.)
-00009440: 027a 9552 6574 7572 6e20 7375 6269 6420  .z.Return subid 
-00009450: 6f66 2073 7562 6261 7369 6e73 2062 6574  of subbasins bet
-00009460: 7765 656e 2074 776f 2073 7562 6964 2069  ween two subid i
-00009470: 6e20 7468 6520 726f 7574 696e 6720 6e65  n the routing ne
-00009480: 7477 6f72 6b0a 2020 2020 2d2d 2d2d 2d2d  twork.    ------
-00009490: 2d2d 2d2d 0a0a 2020 2020 4e6f 7465 730a  ----..    Notes.
-000094a0: 2020 2020 2d2d 2d2d 2d2d 2d0a 0a20 2020      -------..   
-000094b0: 2052 6574 7572 6e73 3a0a 2020 2020 2d2d   Returns:.    --
-000094c0: 2d2d 2d2d 2d0a 2020 2020 2020 2020 4e6f  -----.        No
-000094d0: 6e65 2c0a 2020 2020 7201 0000 0029 0672  ne,.    r....).r
-000094e0: 1700 0000 7229 0000 0072 1500 0000 721a  ....r)...r....r.
-000094f0: 0000 0072 b900 0000 da06 6465 6c65 7465  ...r......delete
-00009500: 2908 7277 0000 005a 1073 7562 6964 5f64  ).rw...Z.subid_d
-00009510: 6f77 6e73 7472 6561 6d5a 0e73 7562 6964  ownstreamZ.subid
-00009520: 5f75 7073 7472 6561 6dda 0c48 7964 726f  _upstream..Hydro
-00009530: 4261 7369 6e73 315a 0c48 7964 726f 4261  Basins1Z.HydroBa
-00009540: 7369 6e73 3272 4800 0000 da04 726f 7773  sins2rH.....rows
-00009550: da0b 4879 6472 6f42 6173 696e 7372 2400  ..HydroBasinsr$.
-00009560: 0000 7224 0000 0072 2500 0000 da35 5265  ..r$...r%....5Re
-00009570: 7475 726e 5f53 7562 4964 735f 4265 7477  turn_SubIds_Betw
-00009580: 6565 6e5f 5477 6f5f 5375 6262 6173 696e  een_Two_Subbasin
-00009590: 735f 496e 5f52 6f75 696e 675f 4e65 7477  s_In_Rouing_Netw
-000095a0: 6f72 6b4a 0a00 0073 1a00 0000 000e 0201  orkJ...s........
-000095b0: 04ff 0404 0801 0a01 1001 0c01 0201 1201  ................
-000095c0: 0e01 0602 0402 7204 0100 0063 0600 0000  ......r....c....
-000095d0: 0000 0000 0000 0000 2000 0000 0800 0000  ........ .......
-000095e0: 4300 0000 7344 0400 007c 0464 0164 0267  C...sD...|.d.d.g
-000095f0: 0219 00a0 0064 03a1 016a 017d 0674 02a0  .....d...j.}.t..
-00009600: 037c 007c 0166 02a1 017d 077c 077c 0764  .|.|.f...}.|.|.d
-00009610: 0064 0085 0264 0466 0219 00a0 04a1 0019  .d...d.f........
-00009620: 007d 0774 02a0 037c 027c 0366 02a1 017d  .}.t...|.|.f...}
-00009630: 087c 087c 0864 0064 0085 0264 0466 0219  .|.|.d.d...d.f..
-00009640: 00a0 04a1 0019 007d 0874 026a 057c 077c  .......}.t.j.|.|
-00009650: 0864 0564 068d 037d 0774 02a0 0674 02a0  .d.d...}.t...t..
-00009660: 077c 0764 0064 0085 0264 0566 0219 00a1  .|.d.d...d.f....
-00009670: 01a1 017d 0974 02a0 0674 02a0 077c 0764  ...}.t...t...|.d
-00009680: 0064 0085 0264 0766 0219 00a1 01a1 017d  .d...d.f.......}
-00009690: 0a74 02a0 0874 097c 0783 0164 0566 0274  .t...t.|...d.f.t
-000096a0: 026a 0aa1 027d 0b74 0b64 0474 097c 0983  .j...}.t.d.t.|..
-000096b0: 0183 0244 005d 407d 0c7c 097c 0c19 007d  ...D.]@}.|.|...}
-000096c0: 0d7c 046a 0c7c 0464 0119 007c 0d6b 0219  .|.j.|.d...|.k..
-000096d0: 0064 0819 006a 0164 0419 007d 0e7c 0e7c  .d...j.d...}.|.|
-000096e0: 0b7c 0764 0064 0085 0264 0566 0219 007c  .|.d.d...d.f...|
-000096f0: 0d6b 023c 0071 cc74 026a 057c 077c 0b64  .k.<.q.t.j.|.|.d
-00009700: 0564 068d 037d 0767 007d 0f67 007d 1067  .d...}.g.}.g.}.g
-00009710: 007d 1174 0b64 0474 097c 0a83 0183 0244  .}.t.d.t.|.....D
-00009720: 0090 025d e67d 0c7c 0a7c 0c19 007d 037c  ...].}.|.|...}.|
-00009730: 077c 0764 0064 0085 0264 0766 0219 007c  .|.d.d...d.f...|
-00009740: 036b 0219 007d 127c 127c 1264 0064 0085  .k...}.|.|.d.d..
-00009750: 0264 0966 0219 00a0 04a1 0019 007d 127c  .d.f.........}.|
-00009760: 1274 097c 1283 0164 0518 0064 0566 0219  .t.|...d...d.f..
-00009770: 007d 137c 046a 0c7c 0464 0119 00a0 0d7c  .}.|.j.|.d.....|
-00009780: 1264 0064 0085 0264 0566 0219 00a1 0119  .d.d...d.f......
-00009790: 007d 1474 097c 1283 0164 056b 0290 0272  .}.t.|...d.k...r
-000097a0: 0c7c 1264 0a19 007d 157c 056a 0c7c 0564  .|.d...}.|.j.|.d
-000097b0: 0b19 007c 156b 0219 0064 0c19 006a 0164  ...|.k...d...j.d
-000097c0: 0419 007c 036b 0390 0172 f67c 10a0 0574  ...|.k...r.|...t
-000097d0: 0e7c 1264 0a19 0083 01a1 0101 006e 127c  .|.d.........n.|
-000097e0: 0fa0 0574 0e7c 1264 0d19 0083 01a1 0101  ...t.|.d........
-000097f0: 0090 0171 3874 0f7c 067c 1383 027d 1674  ...q8t.|.|...}.t
-00009800: 02a0 067c 1264 0064 0085 0264 0566 0219  ...|.d.d...d.f..
-00009810: 00a1 017d 1774 0b64 0474 097c 1283 0183  ...}.t.d.t.|....
-00009820: 0244 0090 015d e07d 187c 127c 1864 0566  .D...].}.|.|.d.f
-00009830: 0219 007d 157c 157c 136b 0390 0372 667c  ...}.|.|.k...rf|
-00009840: 11a0 0574 0e7c 127c 1864 0566 0219 0083  ...t.|.|.d.f....
-00009850: 01a1 0101 0074 097c 046a 0c7c 0464 0119  .....t.|.j.|.d..
-00009860: 007c 156b 0219 0083 0164 046b 0490 0372  .|.k.....d.k...r
-00009870: 667c 046a 0c7c 0464 0119 007c 156b 0219  f|.j.|.d...|.k..
-00009880: 0064 0219 006a 0164 0419 007d 197c 197c  .d...j.d...}.|.|
-00009890: 1676 0090 0372 667c 197c 1264 0064 0085  .v...rf|.|.d.d..
-000098a0: 0264 0566 0219 0076 0190 0372 667c 11a0  .d.f...v...rf|..
-000098b0: 0574 0e7c 1983 01a1 0101 007c 197d 1a64  .t.|.......|.}.d
-000098c0: 047d 1b7c 1b64 0e6b 0090 0372 667c 1b64  .}.|.d.k...rf|.d
-000098d0: 0517 007d 1b74 097c 046a 0c7c 0464 0119  ...}.t.|.j.|.d..
-000098e0: 007c 1a6b 0219 0083 0164 046b 0490 0372  .|.k.....d.k...r
-000098f0: 667c 046a 0c7c 0464 0119 007c 1a6b 0219  f|.j.|.d...|.k..
-00009900: 0064 0219 006a 0164 0419 007d 1c7c 1c7c  .d...j.d...}.|.|
-00009910: 1264 0064 0085 0264 0566 0219 0076 0190  .d.d...d.f...v..
-00009920: 0372 667c 1c7c 1676 0090 0372 667c 11a0  .rf|.|.v...rf|..
-00009930: 0574 0e7c 1c83 01a1 0101 007c 1c7d 1a6e  .t.|.......|.}.n
-00009940: 0490 0371 666e 0490 0371 6690 0271 da74  ...qfn...qf..q.t
-00009950: 0f7c 067c 1583 027d 1d74 097c 1d83 0164  .|.|...}.t.|...d
-00009960: 046b 0490 0372 a474 02a0 0d7c 1d7c 17a1  .k...r.t...|.|..
-00009970: 027d 1e74 107c 1e83 0164 0f6b 0590 0372  .}.t.|...d.k...r
-00009980: 9e64 107d 1f6e 0464 117d 1f6e 0464 117d  .d.}.n.d.}.n.d.}
-00009990: 1f74 097c 146a 0c7c 1464 0219 007c 156b  .t.|.j.|.d...|.k
-000099a0: 0219 0083 0164 046b 0490 0373 ec7c 056a  .....d.k...s.|.j
-000099b0: 0c7c 0564 0b19 007c 156b 0219 0064 0c19  .|.d...|.k...d..
-000099c0: 006a 0164 0419 007c 036b 0290 0373 ec7c  .j.d...|.k...s.|
-000099d0: 1f90 0472 047c 0fa0 0574 0e7c 127c 1864  ...r.|...t.|.|.d
-000099e0: 0466 0219 0083 01a1 0101 006e 167c 10a0  .f.........n.|..
-000099f0: 0574 0e7c 127c 1864 0566 0219 0083 01a1  .t.|.|.d.f......
-00009a00: 0101 0090 0271 3a90 0171 3874 1174 127c  .....q:..q8t.t.|
-00009a10: 1183 0183 0174 1174 127c 0f83 0183 0174  .....t.t.|.....t
-00009a20: 1174 127c 1083 0183 0166 0353 0029 124e  .t.|.....f.S.).N
-00009a30: 7206 0000 0072 0d00 0000 722d 0000 0072  r....r....r-...r
-00009a40: 0100 0000 7228 0000 0072 0e00 0000 72e1  ....r(...r....r.
-00009a50: 0000 00da 0a4d 6178 4163 635f 6361 74e9  .....MaxAcc_cat.
-00009a60: 0400 0000 2902 7201 0000 0072 2800 0000  ....).r....r(...
-00009a70: 5a08 494c 5f53 7562 4964 5a08 736c 5f63  Z.IL_SubIdZ.sl_c
-00009a80: 6c5f 6964 2902 7201 0000 0072 0100 0000  l_id).r....r....
-00009a90: 727b 0000 0072 6500 0000 5446 2913 7216  r{...re...TF).r.
-00009aa0: 0000 0072 1300 0000 721a 0000 00da 0c63  ...r....r......c
-00009ab0: 6f6c 756d 6e5f 7374 6163 6bda 0761 7267  olumn_stack..arg
-00009ac0: 736f 7274 724e 0000 0072 2b00 0000 72f0  sortrN...r+...r.
-00009ad0: 0000 0072 7d00 0000 7215 0000 0072 d100  ...r}...r....r..
-00009ae0: 0000 7229 0000 0072 1900 0000 7212 0000  ..r)...r....r...
-00009af0: 0072 2d00 0000 7217 0000 0072 3f00 0000  .r-...r....r?...
-00009b00: 7254 0000 0072 c900 0000 2920 5a0b 7269  rT...r....) Z.ri
-00009b10: 765f 6c61 6b65 5f69 645a 0673 7472 5f69  v_lake_idZ.str_i
-00009b20: 645a 0c72 6976 5f6c 616b 655f 6964 325a  dZ.riv_lake_id2Z
-00009b30: 0563 6c5f 6964 7277 0000 005a 1373 7472  .cl_idrw...Z.str
-00009b40: 5f73 7461 7274 5f70 745f 6c61 6b65 6964  _start_pt_lakeid
-00009b50: 5a11 726f 7574 696e 675f 696e 666f 5f72  Z.routing_info_r
-00009b60: 6f75 745a 0872 6976 5f6c 616b 655a 0b72  outZ.riv_lakeZ.r
-00009b70: 6976 5f6c 616b 655f 636c 5a0d 7374 725f  iv_lake_clZ.str_
-00009b80: 6964 5f75 6e69 7175 655a 0c63 6c5f 6964  id_uniqueZ.cl_id
-00009b90: 5f75 6e69 7175 655a 0a61 6363 5f73 7472  _uniqueZ.acc_str
-00009ba0: 5f63 6c72 4800 0000 da05 7374 7269 64da  _clrH.....strid.
-00009bb0: 066d 6178 6163 635a 146e 6f6e 5f6c 616b  .maxaccZ.non_lak
-00009bc0: 655f 696e 666c 6f77 5f73 6567 735a 1273  e_inflow_segsZ.s
-00009bd0: 7472 5f69 645f 6c61 6b65 5f69 6e6c 666f  tr_id_lake_inlfo
-00009be0: 775a 1373 7472 5f69 645f 7769 7468 696e  wZ.str_id_within
-00009bf0: 5f6c 616b 6573 5a0b 7269 765f 6c61 6b65  _lakesZ.riv_lake
-00009c00: 5f69 6c5a 0a6f 7574 6c65 745f 7374 725a  _ilZ.outlet_strZ
-00009c10: 1073 7562 5f72 6f75 7469 6e67 5f69 6e66  .sub_routing_inf
-00009c20: 6f5a 0b73 7472 5f69 645f 636c 5f6a 5a13  oZ.str_id_cl_jZ.
-00009c30: 7374 7273 5f74 6f5f 6c61 6b65 5f6f 7574  strs_to_lake_out
-00009c40: 6c65 745a 1875 6e69 7175 655f 7374 725f  letZ.unique_str_
-00009c50: 6964 5f63 765f 6279 5f6c 616b 6572 5e00  id_cv_by_laker^.
-00009c60: 0000 5a1a 646f 776e 5f73 756e 5f6f 665f  ..Z.down_sun_of_
-00009c70: 6c61 6b65 5f63 6f76 6572 5f73 7472 5a06  lake_cover_strZ.
-00009c80: 6373 7472 6964 5a03 6b5f 645a 0764 7374  cstridZ.k_dZ.dst
-00009c90: 725f 6964 5a0b 7570 5f73 7472 5f63 6c5f  r_idZ.up_str_cl_
-00009ca0: 6a72 2300 0000 5a11 6861 735f 7570 5f73  jr#...Z.has_up_s
-00009cb0: 7472 5f69 6e6c 616b 6572 2400 0000 7224  tr_inlaker$...r$
-00009cc0: 0000 0072 2500 0000 da31 7265 7475 726e  ...r%....1return
-00009cd0: 5f6e 6f6e 5f6c 616b 655f 696e 666c 6f77  _non_lake_inflow
-00009ce0: 5f73 6567 735f 616e 645f 7365 6773 5f77  _segs_and_segs_w
-00009cf0: 6974 6869 6e5f 6c61 6b65 736a 0a00 0073  ithin_lakesj...s
-00009d00: ae00 0000 0004 1402 0e01 1801 0e01 1801  ................
-00009d10: 1003 1c01 1c02 1601 1201 0803 1601 02ff  ................
-00009d20: 0403 1a01 1005 0401 0401 0401 1402 0802  ................
-00009d30: 1801 1801 1401 0401 18ff 0405 0e01 0803  ................
-00009d40: 1001 02ff 0402 02fe 0203 02fd 02ff 0406  ................
-00009d50: 1402 1201 0402 0a07 1602 1401 0c03 0a01  ................
-00009d60: 1602 1c02 1c03 2003 0e02 0401 0401 0a01  ...... .........
-00009d70: 0801 1c01 1c02 2001 0e01 0602 0602 0803  ...... .........
-00009d80: 0a02 0e04 0c01 0e01 0602 0602 0403 1401  ................
-00009d90: 02ff 02ff 0403 0401 0aff 0202 02fe 0402  ................
-00009da0: 02fe 0203 02fd 02fd 0407 02f9 040b 1802  ................
-00009db0: 1e02 720b 0100 0063 0300 0000 0000 0000  ..r....c........
-00009dc0: 0000 0000 1500 0000 0600 0000 4300 0000  ............C...
-00009dd0: 73d8 0100 0067 007d 0367 007d 0474 00a0  s....g.}.g.}.t..
-00009de0: 017c 007c 0166 02a1 017d 0574 00a0 0274  .|.|.f...}.t...t
-00009df0: 00a0 037c 01a1 01a1 017d 0674 00a0 0274  ...|.....}.t...t
-00009e00: 00a0 037c 00a1 01a1 017d 0774 00a0 0474  ...|.....}.t...t
-00009e10: 057c 0583 0164 0166 0274 006a 06a1 027d  .|...d.f.t.j...}
-00009e20: 0874 0764 0274 057c 0683 0183 0244 005d  .t.d.t.|.....D.]
-00009e30: 407d 097c 067c 0919 007d 0a7c 026a 087c  @}.|.|...}.|.j.|
-00009e40: 0264 0319 007c 0a6b 0219 0064 0419 006a  .d...|.k...d...j
-00009e50: 0964 0219 007d 0b7c 0b7c 087c 0564 0064  .d...}.|.|.|.d.d
-00009e60: 0085 0264 0166 0219 007c 0a6b 023c 0071  ...d.f...|.k.<.q
-00009e70: 5a74 006a 0a7c 057c 0864 0164 058d 037d  Zt.j.|.|.d.d...}
-00009e80: 057c 057c 0564 0064 0085 0264 0666 0219  .|.|.d.d...d.f..
-00009e90: 00a0 0ba1 0019 007d 057c 0264 0364 0767  .......}.|.d.d.g
-00009ea0: 0219 00a0 0c64 08a1 016a 097d 0c74 0764  .....d...j.}.t.d
-00009eb0: 0274 057c 0783 0183 0244 005d e87d 097c  .t.|.....D.].}.|
-00009ec0: 077c 0919 007d 0d7c 057c 0564 0064 0085  .|...}.|.|.d.d..
-00009ed0: 0264 0266 0219 007c 0d6b 0219 007d 0e74  .d.f...|.k...}.t
-00009ee0: 057c 0e83 0164 016b 0190 0172 1a71 e67c  .|...d.k...r.q.|
-00009ef0: 0e74 057c 0e83 0164 0118 0064 0166 0219  .t.|...d...d.f..
-00009f00: 007d 0f74 0d7c 0c7c 0f83 027d 1074 00a0  .}.t.|.|...}.t..
-00009f10: 0e7c 0e64 0064 0085 0264 0166 0219 007c  .|.d.d...d.f...|
-00009f20: 10a1 027d 1167 007d 1274 057c 117c 1164  ...}.g.}.t.|.|.d
-00009f30: 096b 0219 0083 0174 057c 0e64 0064 0085  .k.....t.|.d.d..
-00009f40: 0264 0166 0219 0083 016b 0072 e67c 0e74  .d.f.....k.r.|.t
-00009f50: 00a0 0f7c 11a1 0164 0166 0219 007d 1374  ...|...d.f...}.t
-00009f60: 0764 0274 057c 1383 0183 0244 005d 227d  .d.t.|.....D.]"}
-00009f70: 147c 137c 1419 007d 0a7c 0a7c 0f6b 0390  .|.|...}.|.|.k..
-00009f80: 0172 987c 12a0 0a7c 0aa1 0101 0090 0171  .r.|...|.......q
-00009f90: 987c 047c 1217 007d 047c 03a0 0a7c 0da1  .|.|...}.|...|..
-00009fa0: 0101 0071 e67c 037c 0466 0253 0029 0a4e  ...q.|.|.f.S.).N
-00009fb0: 7228 0000 0072 0100 0000 7206 0000 0072  r(...r....r....r
-00009fc0: 0501 0000 720e 0000 0072 6500 0000 720d  ....r....re...r.
-00009fd0: 0000 0072 2d00 0000 5429 1072 1a00 0000  ...r-...T).r....
-00009fe0: 7207 0100 0072 2b00 0000 72f0 0000 0072  r....r+...r....r
-00009ff0: 7d00 0000 7215 0000 0072 d100 0000 7229  }...r....r....r)
-0000a000: 0000 0072 1900 0000 7213 0000 0072 4e00  ...r....r....rN.
-0000a010: 0000 7208 0100 0072 1600 0000 7217 0000  ..r....r....r...
-0000a020: 0072 1200 0000 729a 0000 0029 155a 0543  .r....r....).Z.C
-0000a030: 4c5f 4964 5a06 5374 725f 4964 5a0c 526f  L_IdZ.Str_IdZ.Ro
-0000a040: 7574 696e 675f 696e 666f 5a17 4c61 6b65  uting_infoZ.Lake
-0000a050: 735f 5749 7468 5f4d 756c 7469 5f4f 7574  s_WIth_Multi_Out
-0000a060: 6c65 745a 0a52 656d 6f76 655f 5374 725a  letZ.Remove_StrZ
-0000a070: 0643 4c5f 5374 725a 0d53 7472 5f49 645f  .CL_StrZ.Str_Id_
-0000a080: 756e 6971 7565 5a0c 434c 5f49 645f 756e  uniqueZ.CL_Id_un
-0000a090: 6971 7565 5a0a 4163 635f 5374 725f 434c  iqueZ.Acc_Str_CL
-0000a0a0: 7248 0000 0072 0901 0000 720a 0100 005a  rH...r....r....Z
-0000a0b0: 1172 6f75 7469 6e67 5f69 6e66 6f5f 6f6e  .routing_info_on
-0000a0c0: 6c79 5a07 6c61 6b65 5f69 645a 0869 5f43  lyZ.lake_idZ.i_C
-0000a0d0: 4c5f 5374 725a 0b73 7472 5f6d 6178 5f61  L_StrZ.str_max_a
-0000a0e0: 6363 5a12 7374 725f 746f 5f73 7472 5f6d  ccZ.str_to_str_m
-0000a0f0: 6178 5f61 6363 7223 0000 005a 0c52 656d  ax_accr#...Z.Rem
-0000a100: 6f76 655f 5374 725f 695a 1873 7472 5f6e  ove_Str_iZ.str_n
-0000a110: 6f74 666c 6f77 746f 5f6c 616b 656f 7574  otflowto_lakeout
-0000a120: 6c65 745a 0469 7374 7272 2400 0000 7224  letZ.istrr$...r$
-0000a130: 0000 0072 2500 0000 da1f 4368 6563 6b5f  ...r%.....Check_
-0000a140: 4966 5f4c 616b 655f 4861 7665 5f4d 756c  If_Lake_Have_Mul
-0000a150: 7469 5f4f 7574 4c65 74ef 0a00 0073 4200  ti_OutLet....sB.
-0000a160: 0000 0003 0401 0402 0e02 1002 1003 1601  ................
-0000a170: 1201 0801 1601 02ff 0403 1a01 1003 1803  ................
-0000a180: 1403 1202 0802 1803 0e01 0208 1403 0a08  ................
-0000a190: 1804 0403 2402 1202 1202 0805 0a01 0e05  ....$...........
-0000a1a0: 0801 0c02 720c 0100 0063 0100 0000 0000  ....r....c......
-0000a1b0: 0000 0000 0000 0900 0000 0a00 0000 4300  ..............C.
-0000a1c0: 0000 73ba 0000 0064 017d 017c 006a 0064  ..s....d.}.|.j.d
-0000a1d0: 0264 038d 017d 027c 0264 0119 006a 017c  .d...}.|.d...j.|
-0000a1e0: 0264 043c 007c 0064 0519 006a 017d 037c  .d.<.|.d...j.}.|
-0000a1f0: 037c 0364 066b 0419 007d 0374 02a0 037c  .|.d.k...}.t...|
-0000a200: 03a1 017d 0374 0464 0674 057c 0383 0183  ...}.t.d.t.|....
-0000a210: 0244 005d 687d 047c 037c 0419 007d 057c  .D.]h}.|.|...}.|
-0000a220: 006a 067c 0064 0519 007c 056b 0219 007d  .j.|.d...|.k...}
-0000a230: 067c 066a 0764 0767 0164 0864 098d 027d  .|.j.d.g.d.d...}
-0000a240: 067c 067c 0119 006a 0164 0619 007d 077c  .|.|...j.d...}.|
-0000a250: 067c 0119 006a 017d 0874 057c 0883 0164  .|...j.}.t.|...d
-0000a260: 0a6b 0472 4c74 087c 077c 007c 0264 0a7c  .k.rLt.|.|.|.d.|
-0000a270: 087c 0064 0a64 0b8d 077d 0271 4c7c 0253  .|.d.d...}.qL|.S
-0000a280: 0029 0c72 fd00 0000 7206 0000 0054 7207  .).r....r....Tr.
-0000a290: 0000 0072 8300 0000 7284 0000 0072 0100  ...r....r....r..
-0000a2a0: 0000 7279 0000 0046 727a 0000 0072 2800  ..ry...Frz...r(.
-0000a2b0: 0000 72fb 0000 0029 0972 1400 0000 7213  ..r....).r....r.
-0000a2c0: 0000 0072 1a00 0000 722b 0000 0072 2900  ...r....r+...r).
-0000a2d0: 0000 7215 0000 0072 1900 0000 7241 0000  ..r....r....rA..
-0000a2e0: 0072 a300 0000 72fe 0000 0072 2400 0000  .r....r....r$...
-0000a2f0: 7224 0000 0072 2500 0000 da3b 6368 616e  r$...r%....;chan
-0000a300: 6765 5f61 7474 7269 6275 7465 5f76 616c  ge_attribute_val
-0000a310: 7565 735f 666f 725f 6361 7463 686d 656e  ues_for_catchmen
-0000a320: 7473 5f63 6f76 6572 6564 5f62 795f 7361  ts_covered_by_sa
-0000a330: 6d65 5f6c 616b 6545 0b00 0073 3200 0000  me_lakeE...s2...
-0000a340: 000d 0401 0c01 0e01 0a01 0c01 0a03 1201  ................
-0000a350: 0801 1201 1001 0801 02ff 0403 0a01 0c01  ................
-0000a360: 0201 0201 0201 0201 0201 0201 0201 02f9  ................
-0000a370: 0809 720d 0100 0063 0300 0000 0000 0000  ..r....c........
-0000a380: 0000 0000 0d00 0000 0500 0000 4300 0000  ............C...
-0000a390: 73a8 0200 007c 006a 007d 037c 0264 016b  s....|.j.}.|.d.k
-0000a3a0: 0490 0172 dc74 0164 0174 027c 0383 0183  ...r.t.d.t.|....
-0000a3b0: 0244 005d dc7d 047c 006a 037c 037c 0419  .D.].}.|.j.|.|..
-0000a3c0: 0064 0266 0219 007d 057c 006a 037c 037c  .d.f...}.|.j.|.|
-0000a3d0: 0419 0064 0366 0219 007d 067c 006a 037c  ...d.f...}.|.j.|
-0000a3e0: 037c 0419 0064 0466 0219 007d 077c 006a  .|...d.f...}.|.j
-0000a3f0: 037c 0064 0319 007c 076b 0219 00a0 04a1  .|.d...|.k......
-0000a400: 007d 0874 027c 0883 0164 016b 0472 987c  .}.t.|...d.k.r.|
-0000a410: 0864 0219 006a 0564 0119 007c 006a 037c  .d...j.d...|.j.|
-0000a420: 037c 0419 0064 0566 023c 006e 1264 067c  .|...d.f.<.n.d.|
-0000a430: 006a 037c 037c 0419 0064 0566 023c 007c  .j.|.|...d.f.<.|
-0000a440: 057c 006a 037c 037c 0419 0064 0566 0219  .|.j.|.|...d.f..
-0000a450: 006b 0272 d264 067c 006a 037c 037c 0419  .k.r.d.|.j.|.|..
-0000a460: 0064 0566 023c 007c 057c 006a 037c 037c  .d.f.<.|.|.j.|.|
-0000a470: 0419 0064 0566 0219 006b 0272 1e64 067c  ...d.f...k.r.d.|
-0000a480: 006a 037c 037c 0419 0064 0566 023c 0071  .j.|.|...d.f.<.q
-0000a490: 1e7c 0064 0319 006a 057c 0064 073c 007c  .|.d...j.|.d.<.|
-0000a4a0: 0064 0419 006a 057c 0064 083c 007c 0064  .d...j.|.d.<.|.d
-0000a4b0: 0219 006a 057c 0064 033c 007c 0064 0519  ...j.|.d.<.|.d..
-0000a4c0: 006a 057c 0064 043c 007c 007c 0064 0919  .j.|.d.<.|.|.d..
-0000a4d0: 0064 0a6b 0319 006a 0464 0b64 0c8d 017d  .d.k...j.d.d...}
-0000a4e0: 097c 0064 0319 00a0 067c 0964 0419 00a1  .|.d.....|.d....
-0000a4f0: 010f 007d 0a64 0d7c 006a 0776 0090 0172  ...}.d.|.j.v...r
-0000a500: 8864 0e7c 006a 037c 0a64 0d66 023c 0064  .d.|.j.|.d.f.<.d
-0000a510: 0e7c 006a 037c 0a64 0f66 023c 0064 0e7c  .|.j.|.d.f.<.d.|
-0000a520: 006a 037c 0a64 1066 023c 0064 0e7c 006a  .j.|.d.f.<.d.|.j
-0000a530: 037c 0a64 1166 023c 0064 0e7c 006a 037c  .|.d.f.<.d.|.j.|
-0000a540: 0a64 1266 023c 0064 0e7c 006a 037c 0a64  .d.f.<.d.|.j.|.d
-0000a550: 1366 023c 0064 0e7c 006a 037c 0a64 1466  .f.<.d.|.j.|.d.f
-0000a560: 023c 0064 0e7c 006a 037c 0a64 1566 023c  .<.d.|.j.|.d.f.<
-0000a570: 007c 0164 016b 0090 0172 ea7c 0053 007c  .|.d.k...r.|.S.|
-0000a580: 006a 0864 0364 1664 178d 027d 0b74 097c  .j.d.d.d...}.t.|
-0000a590: 0b83 017d 0b74 0164 0174 027c 0b83 0183  ...}.t.d.t.|....
-0000a5a0: 0244 005d 947d 047c 0b64 0319 006a 057c  .D.].}.|.d...j.|
-0000a5b0: 0419 007d 0c7c 0b64 1819 006a 057c 0419  ...}.|.d...j.|..
-0000a5c0: 007c 006a 037c 0064 0319 007c 0c6b 0264  .|.j.|.d...|.k.d
-0000a5d0: 1866 023c 007c 0b64 1919 006a 057c 0419  .f.<.|.d...j.|..
-0000a5e0: 007c 006a 037c 0064 0319 007c 0c6b 0264  .|.j.|.d...|.k.d
-0000a5f0: 1966 023c 007c 0b64 1a19 006a 057c 0419  .f.<.|.d...j.|..
-0000a600: 007c 006a 037c 0064 0319 007c 0c6b 0264  .|.j.|.d...|.k.d
-0000a610: 1a66 023c 007c 0b64 1b19 006a 057c 0419  .f.<.|.d...j.|..
-0000a620: 007c 006a 037c 0064 0319 007c 0c6b 0264  .|.j.|.d...|.k.d
-0000a630: 1b66 023c 0090 0271 0e7c 0053 0029 1c72  .f.<...q.|.S.).r
-0000a640: a700 0000 7201 0000 0072 8300 0000 7206  ....r....r....r.
-0000a650: 0000 0072 0d00 0000 7285 0000 0072 6b00  ...r....r....rk.
-0000a660: 0000 7286 0000 0072 8700 0000 7264 0000  ..r....r....rd..
-0000a670: 0072 6500 0000 5472 0700 0000 7272 0000  .re...Tr....rr..
-0000a680: 0072 6c00 0000 7273 0000 0072 6800 0000  .rl...rs...rh...
-0000a690: 726d 0000 0072 7100 0000 726e 0000 0072  rm...rq...rn...r
-0000a6a0: 7000 0000 726f 0000 0072 3a00 0000 72a8  p...ro...r:...r.
-0000a6b0: 0000 0072 6900 0000 7266 0000 0072 6a00  ...ri...rf...rj.
-0000a6c0: 0000 7279 0000 0029 0a72 5900 0000 7229  ..ry...).rY...r)
-0000a6d0: 0000 0072 1500 0000 7219 0000 0072 1400  ...r....r....r..
-0000a6e0: 0000 7213 0000 0072 1200 0000 7211 0000  ..r....r....r...
-0000a6f0: 0072 4200 0000 5a1a 5374 7265 616d 6f72  .rB...Z.Streamor
-0000a700: 6465 7261 6e64 6472 6169 6e61 6765 6172  deranddrainagear
-0000a710: 6561 290d 728a 0000 0072 aa00 0000 72ab  ea).r....r....r.
-0000a720: 0000 0072 5f00 0000 7248 0000 0072 8300  ...r_...rH...r..
-0000a730: 0000 7249 0000 0072 ac00 0000 72ad 0000  ..rI...r....r...
-0000a740: 00da 1972 6976 5f70 645f 6e6e 636c 735f  ...riv_pd_nncls_
-0000a750: 726f 7574 696e 675f 696e 666f 7223 0000  routing_infor#..
-0000a760: 0072 ae00 0000 72af 0000 0072 2400 0000  .r....r....r$...
-0000a770: 7224 0000 0072 2500 0000 7222 0000 006f  r$...r%...r"...o
-0000a780: 0b00 0073 7400 0000 000d 0602 0a01 1201  ...st...........
-0000a790: 1201 1201 1202 0401 0aff 0804 0c01 0201  ................
-0000a7a0: 02ff 0402 02fe 1404 1202 1601 1202 1601  ................
-0000a7b0: 1402 0e01 0e01 0e02 0e03 1801 1402 0c01  ................
-0000a7c0: 0e01 0e01 0e01 0e01 0e01 0e01 0e01 0e03  ................
-0000a7d0: 0a01 0402 0e02 0802 1201 0e03 0cfe 0401  ................
-0000a7e0: 0eff 0205 0cfe 0401 0eff 0205 0cfe 0401  ................
-0000a7f0: 0eff 0205 0cfe 0401 0eff 0604 7222 0000  ............r"..
-0000a800: 0063 0300 0000 0000 0000 0000 0000 0300  .c..............
-0000a810: 0000 0300 0000 4300 0000 730c 0000 007c  ......C...s....|
-0000a820: 017c 007c 0213 0014 0053 0029 014e 7224  .|.|.....S.).Nr$
-0000a830: 0000 0029 03da 0141 7261 0000 0072 ca00  ...)...Ara...r..
-0000a840: 0000 7224 0000 0072 2400 0000 7225 0000  ..r$...r$...r%..
-0000a850: 00da 0966 756e 635f 515f 4441 c30b 0000  ...func_Q_DA....
-0000a860: 7302 0000 0000 0172 1001 0000 6301 0000  s......r....c...
-0000a870: 0000 0000 0000 0000 0003 0000 0008 0000  ................
-0000a880: 0043 0000 0073 6400 0000 7a2c 7400 7401  .C...sd...z,t.t.
-0000a890: 7c00 6400 6400 8502 6401 6602 1900 7c00  |.d.d...d.f...|.
-0000a8a0: 6400 6400 8502 6402 6602 1900 8303 5c02  d.d...d.f.....\.
-0000a8b0: 7d01 7d02 5700 6e26 0400 7402 7952 0100  }.}.W.n&..t.yR..
-0000a8c0: 0100 0100 7403 6403 8301 0100 7404 a005  ....t.d.....t...
-0000a8d0: 6404 6405 a102 7d01 5900 6e02 3000 7c01  d.d...}.Y.n.0.|.
-0000a8e0: 6401 1900 7c01 6402 1900 6602 5300 2906  d...|.d...f.S.).
-0000a8f0: 4e72 0100 0000 7228 0000 007a 3723 2323  Nr....r(...z7###
-0000a900: 2323 2323 2323 2323 2323 2323 2323 2323  ################
-0000a910: 2323 2323 2323 2323 2323 2323 2323 2323  ################
-0000a920: 2323 2323 2323 2323 2323 2323 2323 2323  ################
-0000a930: 2323 2323 7265 0000 0072 6b00 0000 2906  ####re...rk...).
-0000a940: 7202 0000 0072 1001 0000 da0c 5275 6e74  r....r......Runt
-0000a950: 696d 6545 7272 6f72 7275 0000 0072 1a00  imeErrorru...r..
-0000a960: 0000 727d 0000 0029 035a 0464 615f 715a  ..r}...).Z.da_qZ
-0000a970: 0570 6f70 7432 5a05 7063 6f76 3272 2400  .popt2Z.pcov2r$.
-0000a980: 0000 7224 0000 0072 2500 0000 da23 7265  ..r$...r%....#re
-0000a990: 7475 726e 5f6b 5f61 6e64 5f63 5f69 6e5f  turn_k_and_c_in_
-0000a9a0: 715f 6461 5f72 656c 6174 696f 6e73 6869  q_da_relationshi
-0000a9b0: 70c7 0b00 0073 0c00 0000 0002 0201 2c01  p....s........,.
-0000a9c0: 0c01 0801 1202 7212 0100 0063 0400 0000  ......r....c....
-0000a9d0: 0000 0000 0000 0000 0d00 0000 0500 0000  ................
-0000a9e0: 4300 0000 73c2 0000 0064 017d 047c 047c  C...s....d.}.|.|
-0000a9f0: 0114 007d 0564 027d 067c 0064 017c 0514  ...}.d.}.|.d.|..
-0000aa00: 0018 007d 077c 0764 036b 0072 4464 047c  ...}.|.d.k.rDd.|
-0000aa10: 0014 007d 0764 057c 0014 007d 057c 007c  ...}.d.|...}.|.|
-0000aa20: 0718 0064 011b 007c 011b 007d 047c 077c  ...d...|...}.|.|
-0000aa30: 0114 0064 017c 0414 007c 0114 007c 0114  ...d.|...|...|..
-0000aa40: 0064 011b 0017 007d 087c 0764 017c 0114  .d.....}.|.d.|..
-0000aa50: 0064 067c 0464 0113 0017 0064 0413 0014  .d.|.d.....d....
-0000aa60: 0017 007d 0974 007c 0883 0174 007c 0983  ...}.t.|...t.|..
-0000aa70: 011b 007d 0a74 007c 0283 0174 007c 0883  ...}.t.|...t.|..
-0000aa80: 011b 007d 0b7c 0b64 036b 0472 ba7c 0a64  ...}.|.d.k.r.|.d
-0000aa90: 0713 007c 0364 0413 0014 007c 0b1b 007d  ...|.d.....|...}
-0000aaa0: 0c6e 0464 087d 0c7c 0c53 0029 094e 7265  .n.d.}.|.S.).Nre
-0000aab0: 0000 007a 0a20 2020 2020 2020 2020 2072  ...z.          r
-0000aac0: 0100 0000 72b1 0000 0067 0000 0000 0000  ....r....g......
-0000aad0: d03f 7228 0000 0067 5555 5555 5555 e53f  .?r(...gUUUUUU.?
-0000aae0: 726c 0000 0029 0172 6300 0000 290d da05  rl...).rc...)...
-0000aaf0: 7769 6474 68da 0564 6570 7468 da01 515a  width..depth..QZ
-0000ab00: 0573 6c6f 7065 5a03 7a63 685a 0573 6964  .slopeZ.zchZ.sid
-0000ab10: 7764 da03 7461 625a 0562 6f74 7764 5a03  wd..tabZ.botwdZ.
-0000ab20: 4163 685a 0350 6368 5a03 5263 68da 0156  AchZ.PchZ.Rch..V
-0000ab30: da01 6e72 2400 0000 7224 0000 0072 2500  ..nr$...r$...r%.
-0000ab40: 0000 da11 6361 6c63 756c 6174 6543 6861  ....calculateCha
-0000ab50: 6e6e 616c 6ed2 0b00 0073 2000 0000 0001  nnaln....s .....
-0000ab60: 0401 0801 0401 0c01 0801 0801 0801 1001  ................
-0000ab70: 1c07 1c01 1001 1001 0801 1602 0401 7219  ..............r.
-0000ab80: 0100 00fa 0123 6303 0000 0000 0000 0000  .....#c.........
-0000ab90: 0000 0010 0000 0007 0000 0043 0000 0073  ...........C...s
-0000aba0: c801 0000 7c01 6401 6b00 720c 7c00 5300  ....|.d.k.r.|.S.
-0000abb0: 7c00 6402 6403 6702 1900 a000 6404 a101  |.d.d.g.....d...
-0000abc0: 6a01 7d03 6405 7d04 6405 7c00 6a02 7601  j.}.d.}.d.|.j.v.
-0000abd0: 7232 6406 7d04 7c02 6407 6b03 9001 7264  r2d.}.|.d.k...rd
-0000abe0: 7403 7c02 8301 6408 1900 6a01 7d05 7404  t.|...d...j.}.t.
-0000abf0: a005 7c05 a101 7d06 7c06 7c06 6401 6b04  ..|...}.|.|.d.k.
-0000ac00: 1900 7d06 7c00 6a06 7c00 7c04 1900 a007  ..}.|.j.|.|.....
-0000ac10: 7c06 a101 1900 7d07 6409 7d08 7c01 6401  |.....}.d.}.|.d.
-0000ac20: 6b00 728c 7408 640a 8301 0100 7c00 5300  k.r.t.d.....|.S.
-0000ac30: 7c00 6a06 7c00 7c04 1900 7c01 6b02 1900  |.j.|.|...|.k...
-0000ac40: 7d09 7409 7c09 8301 6401 6b04 72ba 7c09  }.t.|...d.k.r.|.
-0000ac50: 6402 1900 6a01 6401 1900 7d08 6e0e 7408  d...j.d...}.n.t.
-0000ac60: 640b 7c09 8302 0100 7c00 5300 740a 7c03  d.|.....|.S.t.|.
-0000ac70: 7c08 8302 7d0a 7409 7c07 8301 640c 6b05  |...}.t.|...d.k.
-0000ac80: 9001 7248 740b 6401 7409 7c07 8301 8302  ..rHt.d.t.|.....
-0000ac90: 4400 5d58 7d0b 7c07 6402 1900 6a01 7c0b  D.]X}.|.d...j.|.
-0000aca0: 1900 7d0c 7c0c 7c08 6b02 73ee 7404 a00c  ..}.|.|.k.s.t...
-0000acb0: 7404 a00d 7c0a 7c0c a102 a101 640d 6b00  t...|.|.....d.k.
-0000acc0: 9001 7222 71ee 740a 7c03 7c0c 8302 7d0d  ..r"q.t.|.|...}.
-0000acd0: 7404 a00d 7c0a 7c0d a102 7d0e 7c0a 7404  t...|.|...}.|.t.
-0000ace0: a00e 7c0e a101 1900 7d0a 71ee 7c0a 7d0f  ..|.....}.q.|.}.
-0000acf0: 7c00 6a06 7c00 6402 1900 a007 7c0f a101  |.j.|.d.....|...
-0000ad00: 1900 7d00 7c00 5300 6409 7d08 7c00 6a06  ..}.|.S.d.}.|.j.
-0000ad10: 7c00 7c04 1900 7c01 6b02 1900 7d09 7409  |.|...|.k...}.t.
-0000ad20: 7c09 8301 6401 6b04 9001 72a2 7c09 6402  |...d.k...r.|.d.
-0000ad30: 1900 6a01 6401 1900 7d08 740a 7c03 7c08  ..j.d...}.t.|.|.
-0000ad40: 8302 7d0f 6e0a 7c00 6402 1900 6a01 7d0f  ..}.n.|.d...j.}.
-0000ad50: 7c00 6a06 7c00 6402 1900 a007 7c0f a101  |.j.|.d.....|...
-0000ad60: 1900 7d00 7c00 5300 6400 5300 290e 4e72  ..}.|.S.d.S.).Nr
-0000ad70: 0100 0000 7206 0000 0072 0d00 0000 7263  ....r....r....rc
-0000ad80: 0000 0072 8000 0000 7281 0000 0072 1a01  ...r....r....r..
-0000ad90: 0000 5a09 7265 675f 7375 6269 6472 6b00  ..Z.reg_subidrk.
-0000ada0: 0000 7a41 546f 2075 7365 2073 7562 7265  ..zATo use subre
-0000adb0: 6769 6f6e 2c20 7468 6520 5375 6272 6567  gion, the Subreg
-0000adc0: 696f 6e20 4964 204d 5553 5420 7072 6f76  ion Id MUST prov
-0000add0: 6964 6564 2061 7320 4f75 746c 6574 5f4f  ided as Outlet_O
-0000ade0: 6273 5f49 447a 284e 6f20 4f75 746c 6574  bs_IDz(No Outlet
-0000adf0: 2069 6420 6973 2066 6f75 6e64 6564 2066   id is founded f
-0000ae00: 6f72 2073 7562 7265 6769 6f6e 2020 2072  or subregion   r
-0000ae10: 6500 0000 7228 0000 0029 0f72 1600 0000  e...r(...).r....
-0000ae20: 7213 0000 0072 1100 0000 5a10 4462 665f  r....r....Z.Dbf_
-0000ae30: 546f 5f44 6174 6166 7261 6d65 721a 0000  To_Dataframer...
-0000ae40: 0072 2b00 0000 7219 0000 0072 1200 0000  .r+...r....r....
-0000ae50: 7275 0000 0072 1500 0000 7217 0000 0072  ru...r....r....r
-0000ae60: 2900 0000 723f 0000 0072 2e00 0000 729a  )...r?...r....r.
-0000ae70: 0000 0029 1072 7600 0000 da0d 6f75 746c  ...).rv.....outl
-0000ae80: 6574 5f6f 6273 5f69 64da 1670 6174 685f  et_obs_id..path_
-0000ae90: 7375 625f 7265 675f 6f75 746c 6574 735f  sub_reg_outlets_
-0000aea0: 7672 7700 0000 728c 0000 005a 0f53 7562  vrw...r....Z.Sub
-0000aeb0: 5f72 6567 5f6f 7574 6c65 7473 5a13 5375  _reg_outletsZ.Su
-0000aec0: 625f 7265 675f 6f75 746c 6574 735f 6964  b_reg_outlets_id
-0000aed0: 735a 0f72 6567 5f6f 7574 6c65 745f 696e  sZ.reg_outlet_in
-0000aee0: 666f 72bb 0000 005a 0d6f 7574 6c65 7449  for....Z.outletI
-0000aef0: 445f 696e 666f 7201 0100 0072 4800 0000  D_infor....rH...
-0000af00: 5a07 7570 7265 6769 645a 1248 7964 726f  Z.upregidZ.Hydro
-0000af10: 4261 7369 6e73 5f72 656d 6f76 6572 2300  Basins_remover#.
-0000af20: 0000 7203 0100 0072 2400 0000 7224 0000  ..r....r$...r$..
-0000af30: 0072 2500 0000 da1f 7265 7475 726e 5f69  .r%.....return_i
-0000af40: 6e74 6572 6573 745f 6361 7463 686d 656e  nterest_catchmen
-0000af50: 7473 5f69 6e66 6fec 0b00 0073 5400 0000  ts_info....sT...
-0000af60: 0002 0801 0402 1402 0401 0a01 0402 0a02  ................
-0000af70: 0e01 0a01 0c03 1403 0402 0801 0801 0402  ................
-0000af80: 1201 0c01 1002 0a01 0403 0a04 0e02 1201  ................
-0000af90: 0e02 2001 0201 0a01 0401 04ff 0403 1001  .. .............
-0000afa0: 0402 1401 0403 0401 1201 0e01 0e02 0c02  ................
-0000afb0: 0a02 1401 721d 0100 0063 0200 0000 0000  ....r....c......
-0000afc0: 0000 0000 0000 0c00 0000 0500 0000 0300  ................
-0000afd0: 0000 7352 0100 0067 007d 0288 0164 0119  ..sR...g.}...d..
-0000afe0: 006a 007d 0374 01a0 027c 03a1 017d 0367  .j.}.t...|...}.g
-0000aff0: 007d 0274 03a0 04a1 0074 056a 0664 023c  .}.t.....t.j.d.<
-0000b000: 007c 02a0 0764 03a1 0101 007c 02a0 0764  .|...d.....|...d
-0000b010: 04a1 0101 007c 02a0 0764 05a1 0101 0074  .....|...d.....t
-0000b020: 087c 0383 017d 047c 02a0 0764 0674 097c  .|...}.|...d.t.|
-0000b030: 0483 0117 00a1 0101 0074 0a7c 0164 0719  .........t.|.d..
-0000b040: 006a 0083 0164 0817 0074 0a7c 0164 0919  .j...d...t.|.d..
-0000b050: 006a 0083 0164 0817 0014 007d 057c 02a0  .j...d.....}.|..
-0000b060: 0764 0a74 097c 0583 0117 00a1 0101 007c  .d.t.|.........|
-0000b070: 02a0 0764 0ba1 0101 007c 02a0 0764 0ca1  ...d.....|...d..
-0000b080: 0101 0074 0a7c 0164 0919 006a 0083 0189  ...t.|.d...j....
-0000b090: 027c 0164 0d19 006a 0089 0074 0b74 087c  .|.d...j...t.t.|
-0000b0a0: 0383 0164 0e1b 0083 017d 0674 087c 0383  ...d.....}.t.|..
-0000b0b0: 0164 0f6b 0472 ee74 01a0 0c7c 037c 06a1  .d.k.r.t...|.|..
-0000b0c0: 027d 076e 067c 0367 017d 0774 0d64 1074  .}.n.|.g.}.t.d.t
-0000b0d0: 087c 0783 0183 0244 005d 367d 087c 077c  .|.....D.]6}.|.|
-0000b0e0: 0819 007d 0974 0e64 1164 128d 0187 0087  ...}.t.d.d......
-0000b0f0: 0187 0266 0364 1364 1484 087c 0944 0083  ...f.d.d...|.D..
-0000b100: 0183 017d 0a7c 027c 0a17 007d 0290 0171  ...}.|.|...}...q
-0000b110: 027c 02a0 0764 15a1 0101 0064 16a0 0f7c  .|...d.....d...|
-0000b120: 02a1 017d 0b7c 0b53 0029 174e 72a4 0000  ...}.|.S.).Nr...
-0000b130: 005a 124a 4f42 4c49 425f 5445 4d50 5f46  .Z.JOBLIB_TEMP_F
-0000b140: 4f4c 4445 527a 0c3a 4772 6964 5765 6967  OLDERz.:GridWeig
-0000b150: 6874 737a 0a20 2020 2320 2020 2020 207a  htsz.   #      z
-0000b160: 0d20 2020 2320 5b23 2048 5255 735d 7a15  .   # [# HRUs]z.
-0000b170: 2020 203a 4e75 6d62 6572 4852 5573 2020     :NumberHRUs  
-0000b180: 2020 2020 205a 0352 6f77 7228 0000 00da       Z.Rowr(....
-0000b190: 0343 6f6c 7a15 2020 203a 4e75 6d62 6572  .Colz.   :Number
-0000b1a0: 4772 6964 4365 6c6c 7320 207a 1020 2020  GridCells  z.   
-0000b1b0: 2320 2020 2020 2020 2020 2020 207a 1d20  #            z. 
-0000b1c0: 2020 2320 5b48 5255 2049 445d 205b 4365    # [HRU ID] [Ce
-0000b1d0: 6c6c 2023 5d20 5b77 5f6b 6c5d 5a04 4647  ll #] [w_kl]Z.FG
-0000b1e0: 4944 72cf 0000 0072 7c00 0000 7201 0000  IDr....r|...r...
-0000b1f0: 0072 0601 0000 2901 5a06 6e5f 6a6f 6273  .r....).Z.n_jobs
-0000b200: 6301 0000 0000 0000 0000 0000 0002 0000  c...............
-0000b210: 0006 0000 0033 0000 0073 2800 0000 7c00  .....3...s(...|.
-0000b220: 5d20 7d01 7400 7401 8301 7c01 8801 6a02  ] }.t.t...|...j.
-0000b230: 6400 6401 8d01 8800 8802 8304 5600 0100  d.d.........V...
-0000b240: 7102 6402 5300 2903 5472 0700 0000 4e29  q.d.S.).Tr....N)
-0000b250: 0372 0500 0000 da16 6372 6561 7465 5f67  .r......create_g
-0000b260: 7269 645f 7765 6967 6874 5f68 7275 7214  rid_weight_hrur.
-0000b270: 0000 0029 02da 022e 3072 4800 0000 a903  ...)....0rH.....
-0000b280: da07 4176 6166 6769 64da 0a4d 6170 666f  ..Avafgid..Mapfo
-0000b290: 7263 696e 67da 076d 6178 5f63 6f6c 7224  rcing..max_colr$
-0000b2a0: 0000 0072 2500 0000 da09 3c67 656e 6578  ...r%.....<genex
-0000b2b0: 7072 3e55 0c00 00f3 0000 0000 7a2a 6372  pr>U........z*cr
-0000b2c0: 6561 7465 5f67 7269 645f 7765 6967 6874  eate_grid_weight
-0000b2d0: 5f6d 6169 6e2e 3c6c 6f63 616c 733e 2e3c  _main.<locals>.<
-0000b2e0: 6765 6e65 7870 723e 7a0f 3a45 6e64 4772  genexpr>z.:EndGr
-0000b2f0: 6964 5765 6967 6874 73da 010a 2910 7213  idWeights...).r.
-0000b300: 0000 0072 1a00 0000 722b 0000 00da 0874  ...r....r+.....t
-0000b310: 656d 7066 696c 65da 0a67 6574 7465 6d70  empfile..gettemp
-0000b320: 6469 72da 026f 73da 0765 6e76 6972 6f6e  dir..os..environ
-0000b330: 724e 0000 0072 1500 0000 72dc 0000 0072  rN...r....r....r
-0000b340: 7400 0000 722d 0000 00da 0b61 7272 6179  t...r-.....array
-0000b350: 5f73 706c 6974 7229 0000 0072 0400 0000  _splitr)...r....
-0000b360: da04 6a6f 696e 290c 7223 0100 005a 0846  ..join).r#...Z.F
-0000b370: 6f72 6369 6e66 6f5a 1767 7269 645f 7765  orcinfoZ.grid_we
-0000b380: 6967 6874 5f73 7472 696e 675f 6c69 7374  ight_string_list
-0000b390: 5a06 6872 7569 6473 5a05 734e 6872 755a  Z.hruidsZ.sNhruZ
-0000b3a0: 0673 4e63 656c 6c5a 0b6e 5f68 7275 5f67  .sNcellZ.n_hru_g
-0000b3b0: 726f 7570 5a0e 6872 755f 6964 735f 6772  roupZ.hru_ids_gr
-0000b3c0: 6f75 7073 7248 0000 005a 0b69 5f68 7275  oupsrH...Z.i_hru
-0000b3d0: 5f67 726f 7570 5a18 6772 6964 5f77 6569  _groupZ.grid_wei
-0000b3e0: 6768 745f 7374 7269 6e67 5f68 7275 7369  ght_string_hrusi
-0000b3f0: 5a12 6772 6964 5f77 6569 6768 745f 7374  Z.grid_weight_st
-0000b400: 7269 6e67 7224 0000 0072 2101 0000 7225  ringr$...r!...r%
-0000b410: 0000 00da 1763 7265 6174 655f 6772 6964  .....create_grid
-0000b420: 5f77 6569 6768 745f 6d61 696e 310c 0000  _weight_main1...
-0000b430: 7336 0000 0000 0204 010a 010a 0204 020e  s6..............
-0000b440: 030a 010a 010a 0208 0112 0224 0112 010a  ...........$....
-0000b450: 010a 010e 010a 0410 020c 010e 0206 0212  ................
-0000b460: 0108 0120 010c 020a 010a 0172 2e01 0000  ... .......r....
-0000b470: 6304 0000 0000 0000 0000 0000 000e 0000  c...............
-0000b480: 0006 0000 0043 0000 0073 1602 0000 6401  .....C...s....d.
-0000b490: 7d04 7c01 6a00 7c01 6402 1900 7c00 6b02  }.|.j.|.d...|.k.
-0000b4a0: 1900 6a01 6403 6404 8d01 7d05 7402 7c05  ..j.d.d...}.t.|.
-0000b4b0: 8301 6405 6b01 725c 7c01 6a00 7c01 6402  ..d.k.r\|.j.|.d.
-0000b4c0: 1900 7c00 6b02 1900 6a01 6403 6404 8d01  ..|.k...j.d.d...
-0000b4d0: 7d05 7403 6406 8301 0100 7403 7c05 6407  }.t.d.....t.|.d.
-0000b4e0: 1900 8301 0100 7c04 5300 7404 7c05 6408  ......|.S.t.|.d.
-0000b4f0: 1900 6a05 8301 7d06 7c05 6407 1900 6a05  ..j...}.|.d...j.
-0000b500: 7d07 7406 a007 7c07 a101 7d07 6409 7d08  }.t...|...}.d.}.
-0000b510: 7408 6405 7402 7c07 8301 8302 4400 9001  t.d.t.|.....D...
-0000b520: 5d7e 7d09 7c05 7c05 6407 1900 7c07 7c09  ]~}.|.|.d...|.|.
-0000b530: 1900 6b02 1900 7d0a 7c09 7402 7c07 8301  ..k...}.|.t.|...
-0000b540: 640a 1800 6b00 72e2 7404 7c0a 6408 1900  d...k.r.t.|.d...
-0000b550: 6a05 8301 7d0b 7409 7c0b 8301 7409 7c06  j...}.t.|...t.|.
-0000b560: 8301 1b00 7d0c 7c08 7c0c 1700 7d08 6e08  ....}.|.|...}.n.
-0000b570: 640a 7c08 1800 7d0c 7402 7c0a 640b 1900  d.|...}.t.|.d...
-0000b580: 6a05 8301 640a 6b04 9001 7240 7403 740a  j...d.k...r@t.t.
-0000b590: 740b 8301 640c 1700 8301 0100 740a 740c  t...d.......t.t.
-0000b5a0: 7c0a 640b 1900 6a05 6405 1900 7c03 640a  |.d...j.d...|.d.
-0000b5b0: 1700 1400 7c0a 640d 1900 6a05 6405 1900  ....|.d...j.d...
-0000b5c0: 1700 8301 8301 640e 1700 7d0d 6e30 740a  ......d...}.n0t.
-0000b5d0: 740c 7c0a 640b 1900 6a05 6405 1900 7c03  t.|.d...j.d...|.
-0000b5e0: 640a 1700 1400 7c0a 640d 1900 6a05 6405  d.....|.d...j.d.
-0000b5f0: 1900 1700 8301 8301 640e 1700 7d0d 7402  ........d...}.t.
-0000b600: 7c07 8301 640a 6b02 9001 72a8 7c04 640f  |...d.k...r.|.d.
-0000b610: 1700 740a 740c 7c00 8301 8301 1700 6410  ..t.t.|.......d.
-0000b620: 1700 7c0d 1700 640e 1700 740a 7c0c 8301  ..|...d...t.|...
-0000b630: 1700 7d04 7190 7c09 7402 7c07 8301 640a  ..}.q.|.t.|...d.
-0000b640: 1800 6b02 9001 72e4 7c04 640f 1700 740a  ..k...r.|.d...t.
-0000b650: 740c 7c00 8301 8301 1700 6410 1700 7c0d  t.|.......d...|.
-0000b660: 1700 640e 1700 740a 7c0c 8301 1700 7d04  ..d...t.|.....}.
-0000b670: 7190 7c04 640f 1700 740a 740c 7c00 8301  q.|.d...t.t.|...
-0000b680: 8301 1700 6410 1700 7c0d 1700 640e 1700  ....d...|...d...
-0000b690: 740a 7c0c 8301 1700 6411 1700 7d04 7190  t.|.....d...}.q.
-0000b6a0: 7c04 5300 2912 4efa 0120 72a4 0000 0054  |.S.).N.. r....T
-0000b6b0: 7207 0000 0072 0100 0000 7a28 466f 6c6c  r....r....z(Foll
-0000b6c0: 6f77 696e 6720 4772 6964 2068 6173 2074  owing Grid has t
-0000b6d0: 6f20 6265 2069 6e6c 7564 6564 3a2e 2e2e  o be inluded:...
-0000b6e0: 2e2e 2e2e 5a08 4d61 705f 4647 4944 5a06  ....Z.Map_FGIDZ.
-0000b6f0: 735f 6172 6561 7267 0000 0072 2800 0000  s_arearg...r(...
-0000b700: 5a07 4d61 705f 526f 777a 3d65 7272 6f72  Z.Map_Rowz=error
-0000b710: 3a20 3120 6872 752c 2031 2067 7269 642c  : 1 hru, 1 grid,
-0000b720: 2070 726f 6475 6365 206d 7574 6920 706f   produce muti po
-0000b730: 6c79 676f 6e20 6e65 6564 2074 6f20 6265  lygon need to be
-0000b740: 206d 6572 6765 6420 5a07 4d61 705f 436f   merged Z.Map_Co
-0000b750: 6c7a 0620 2020 2020 207a 0420 2020 207a  lz.      z.    z
-0000b760: 0520 2020 2020 7227 0100 0029 0d72 1900  .     r'...).r..
-0000b770: 0000 7214 0000 0072 1500 0000 7275 0000  ..r....r....ru..
-0000b780: 0072 3f00 0000 7213 0000 0072 1a00 0000  .r?...r....r....
-0000b790: 722b 0000 0072 2900 0000 7263 0000 0072  r+...r)...rc...r
-0000b7a0: dc00 0000 72b8 0000 0072 2d00 0000 290e  ....r....r-...).
-0000b7b0: 7260 0000 0072 2301 0000 7222 0100 0072  r`...r#...r"...r
-0000b7c0: 2401 0000 5a16 6772 6964 5f77 6569 6768  $...Z.grid_weigh
-0000b7d0: 745f 7374 7269 6e67 5f68 7275 da04 6361  t_string_hru..ca
-0000b7e0: 7473 5a05 7461 7265 615a 0466 6964 735a  tsZ.tareaZ.fidsZ
-0000b7f0: 0573 756d 7774 725e 0000 005a 0473 6361  .sumwtr^...Z.sca
-0000b800: 745a 0573 6172 6561 da02 7774 5a09 5374  tZ.sarea..wtZ.St
-0000b810: 7263 656c 6c69 6472 2400 0000 7224 0000  rcellidr$...r$..
-0000b820: 0072 2500 0000 721f 0100 005c 0c00 0073  .r%...r....\...s
-0000b830: 6c00 0000 0002 0402 1a04 0c01 1a01 0801  l...............
-0000b840: 0c01 0402 0e01 0a01 0a01 0401 1401 1401  ................
-0000b850: 1001 0e01 1001 0a02 0802 1401 0201 0601  ................
-0000b860: 02ff 02ff 0405 0201 0201 0c01 06ff 0202  ................
-0000b870: 0cfe 02ff 02ff 0207 02f9 02ff 040c 0201  ................
-0000b880: 0201 0c01 06ff 0202 0cfe 02ff 02ff 0207  ................
-0000b890: 02f9 02ff 020a 0e01 2a02 1201 2a02 2e02  ........*...*...
-0000b8a0: 721f 0100 0029 0172 2800 0000 2901 7206  r....).r(...).r.
-0000b8b0: 0000 0029 0272 2800 0000 7228 0000 0029  ...).r(...r(...)
-0000b8c0: 0272 2800 0000 7228 0000 0029 0172 1a01  .r(...r(...).r..
-0000b8d0: 0000 2934 7214 0000 00da 056e 756d 7079  ..)4r......numpy
-0000b8e0: 721a 0000 00da 0670 616e 6461 7372 4000  r......pandasr@.
-0000b8f0: 0000 5a0e 7363 6970 792e 6f70 7469 6d69  ..Z.scipy.optimi
-0000b900: 7a65 7202 0000 005a 1e62 6173 696e 6d61  zer....Z.basinma
-0000b910: 6b65 722e 7574 696c 6974 6965 732e 7574  ker.utilities.ut
-0000b920: 696c 6974 6965 73da 076e 756d 6265 7273  ilities..numbers
-0000b930: 5a06 6a6f 626c 6962 7204 0000 0072 0500  Z.joblibr....r..
-0000b940: 0000 7228 0100 00da 076f 7074 696f 6e73  ..r(.....options
-0000b950: da04 6d6f 6465 da12 6368 6169 6e65 645f  ..mode..chained_
-0000b960: 6173 7369 676e 6d65 6e74 7226 0000 0072  assignmentr&...r
-0000b970: 3200 0000 722a 0000 0072 4c00 0000 7256  2...r*...rL...rV
-0000b980: 0000 0072 6200 0000 7278 0000 0072 7f00  ...rb...rx...r..
-0000b990: 0000 7290 0000 0072 a300 0000 72a6 0000  ..r....r....r...
-0000b9a0: 0072 b000 0000 72b2 0000 0072 a900 0000  .r....r....r....
-0000b9b0: 7217 0000 0072 c700 0000 72cd 0000 0072  r....r....r....r
-0000b9c0: d500 0000 72d9 0000 0072 de00 0000 72ef  ....r....r....r.
-0000b9d0: 0000 0072 f700 0000 72fa 0000 0072 fc00  ...r....r....r..
-0000b9e0: 0000 72ff 0000 0072 0401 0000 720b 0100  ..r....r....r...
-0000b9f0: 0072 0c01 0000 720d 0100 0072 2200 0000  .r....r....r"...
-0000ba00: 7210 0100 0072 1201 0000 7219 0100 0072  r....r....r....r
-0000ba10: 1d01 0000 722e 0100 0072 1f01 0000 7224  ....r....r....r$
-0000ba20: 0000 0072 2400 0000 7224 0000 0072 2500  ...r$...r$...r%.
-0000ba30: 0000 da08 3c6d 6f64 756c 653e 0100 0000  ....<module>....
-0000ba40: 7378 0000 0008 0208 0108 010c 0108 0108  sx..............
-0000ba50: 0110 0108 010a 0308 2e08 3808 0b08 1e08  ..........8.....
-0000ba60: 1908 5708 5408 580a 7f00 2002 0102 0104  ..W.T.X... .....
-0000ba70: 0104 0102 0102 f70a 7f00 150a 180a 3e08  ..............>.
-0000ba80: 0a08 7f00 7f00 1c08 2a08 6008 7f00 5e08  ........*.`...^.
-0000ba90: 7b08 1308 7f00 7808 7f00 7f00 7f00 2508  {.....x.......%.
-0000baa0: 5a08 6708 6f08 2b08 2008 7f00 0608 5608  Z.g.o.+. .....V.
-0000bab0: 2a0a 5408 0408 0b08 1a0a 4508 2b         *.T.......E.+
+000000c0: 8400 5a17 6459 6417 6418 8401 5a18 6419  ..Z.dYd.d...Z.d.
+000000d0: 6419 6419 6701 6419 6701 6419 6419 6606  d.d.g.d.g.d.d.f.
+000000e0: 641a 641b 8401 5a19 645a 641d 641e 8401  d.d...Z.dZd.d...
+000000f0: 5a1a 645b 6420 6421 8401 5a1b 6422 6423  Z.d[d d!..Z.d"d#
+00000100: 8400 5a1c 6424 6425 8400 5a1d 6426 6427  ..Z.d$d%..Z.d&d'
+00000110: 8400 5a1e 6428 6429 8400 5a1f 642a 642b  ..Z.d(d)..Z.d*d+
+00000120: 8400 5a20 642c 642d 8400 5a21 642e 642f  ..Z d,d-..Z!d.d/
+00000130: 8400 5a22 6430 6431 8400 5a23 6432 6433  ..Z"d0d1..Z#d2d3
+00000140: 8400 5a24 6434 6435 8400 5a25 6436 6437  ..Z$d4d5..Z%d6d7
+00000150: 8400 5a26 6438 6439 8400 5a27 643a 643b  ..Z&d8d9..Z'd:d;
+00000160: 8400 5a28 643c 643d 8400 5a29 643e 643f  ..Z(d<d=..Z)d>d?
+00000170: 8400 5a2a 6440 6441 8400 5a2b 6442 6443  ..Z*d@dA..Z+dBdC
+00000180: 8400 5a2c 6444 6445 8400 5a2d 6446 6447  ..Z,dDdE..Z-dFdG
+00000190: 8400 5a2e 6448 6449 8400 5a2f 645c 644a  ..Z.dHdI..Z/d\dJ
+000001a0: 644b 8401 5a30 644c 644d 8400 5a31 644e  dK..Z0dLdM..Z1dN
+000001b0: 644f 8400 5a32 6450 6451 8400 5a33 645d  dO..Z2dPdQ..Z3d]
+000001c0: 6453 6454 8401 5a34 6455 6456 8400 5a35  dSdT..Z4dUdV..Z5
+000001d0: 6457 6458 8400 5a36 6401 5300 295e e900  dWdX..Z6d.S.)^..
+000001e0: 0000 004e 2901 da09 6375 7276 655f 6669  ...N)...curve_fi
+000001f0: 7429 01da 012a 2902 da08 5061 7261 6c6c  t)...*)...Parall
+00000200: 656c da07 6465 6c61 7965 6463 0400 0000  el..delayedc....
+00000210: 0000 0000 0000 0000 1200 0000 0600 0000  ................
+00000220: 4300 0000 7352 0100 0064 017d 0464 017d  C...sR...d.}.d.}
+00000230: 0564 017d 0664 017d 077c 007c 0064 0219  .d.}.d.}.|.|.d..
+00000240: 00a0 007c 0064 0319 006a 01a1 010f 0019  ...|.d...j......
+00000250: 007d 087c 0864 0219 00a0 007c 01a1 016a  .}.|.d.....|...j
+00000260: 0264 0464 058d 017d 097c 087c 0919 007d  .d.d...}.|.|...}
+00000270: 0a74 037c 0a83 0164 066b 0172 5e7c 017c  .t.|...d.k.r^|.|
+00000280: 027c 0766 0353 007c 0a7c 0a64 0319 00a0  .|.f.S.|.|.d....
+00000290: 007c 01a1 010f 0019 006a 0264 0464 058d  .|.......j.d.d..
+000002a0: 017d 0b74 037c 0b83 0164 066b 0172 907c  .}.t.|...d.k.r.|
+000002b0: 017c 027c 0766 0353 007c 0064 0364 0267  .|.|.f.S.|.d.d.g
+000002c0: 0219 00a0 0464 07a1 016a 017d 0c7c 0b64  .....d...j.}.|.d
+000002d0: 0319 006a 0144 005d 947d 0d74 057c 0c7c  ...j.D.].}.t.|.|
+000002e0: 0d83 027d 0e7c 007c 0064 0319 00a0 007c  ...}.|.|.d.....|
+000002f0: 0ea1 0119 007d 0f7c 026a 067c 0f64 0364  .....}.|.j.|.d.d
+00000300: 0864 098d 037d 027c 0264 0319 00a0 007c  .d...}.|.d.....|
+00000310: 0ea1 017d 107c 026a 077c 1064 0266 0219  ...}.|.j.|.d.f..
+00000320: 006a 017c 026a 077c 1064 0a66 023c 007c  .j.|.j.|.d.f.<.|
+00000330: 0264 0364 0a67 0219 00a0 0464 07a1 016a  .d.d.g.....d...j
+00000340: 017d 0374 057c 037c 0d83 027d 1174 086a  .}.t.|.|...}.t.j
+00000350: 097c 017c 1166 0264 0664 0b8d 027d 017c  .|.|.f.d.d...}.|
+00000360: 026a 0a64 0264 0c8d 017d 0271 ae64 047d  .j.d.d...}.q.d.}
+00000370: 077c 017c 027c 0766 0353 0029 0d4e 465a  .|.|.|.f.S.).NFZ
+00000380: 0c53 6563 5f44 6f77 5375 6249 64da 0553  .Sec_DowSubId..S
+00000390: 7562 4964 54a9 01da 0464 6565 7072 0100  ubIdT....deepr..
+000003a0: 0000 da05 696e 7433 32da 046c 6566 7429  ....int32..left)
+000003b0: 02da 026f 6eda 0368 6f77 da08 446f 7753  ...on..how..DowS
+000003c0: 7562 4964 a901 da04 6178 6973 a901 da07  ubId....axis....
+000003d0: 636f 6c75 6d6e 7329 0bda 0469 7369 6eda  columns)...isin.
+000003e0: 0676 616c 7565 73da 0463 6f70 79da 036c  .values..copy..l
+000003f0: 656e da06 6173 7479 7065 da06 6465 6663  en..astype..defc
+00000400: 6174 da05 6d65 7267 65da 036c 6f63 da02  at..merge..loc..
+00000410: 6e70 da0b 636f 6e63 6174 656e 6174 65da  np..concatenate.
+00000420: 0464 726f 7029 12da 1073 6563 5f64 6f77  .drop)...sec_dow
+00000430: 6e5f 7375 6269 6e66 6fda 0d75 7073 7472  n_subinfo..upstr
+00000440: 6561 6d5f 7375 6273 da07 6361 745f 706c  eam_subs..cat_pl
+00000450: 79da 0968 7973 6864 696e 666f 5a23 6973  y..hyshdinfoZ#is
+00000460: 5f73 6563 5f64 6f77 6e5f 7375 6269 645f  _sec_down_subid_
+00000470: 696e 5f73 656c 6563 7465 645f 7375 6269  in_selected_subi
+00000480: 645a 2b69 735f 7375 6269 645f 6f66 5f73  dZ+is_subid_of_s
+00000490: 6563 5f64 6f77 6e73 7562 6964 5f69 6e5f  ec_downsubid_in_
+000004a0: 7365 6c65 6374 6564 5f73 7562 6964 da25  selected_subid.%
+000004b0: 7570 6461 7465 5f64 6f77 6e73 7562 6964  update_downsubid
+000004c0: 735f 7573 696e 675f 7365 635f 646f 776e  s_using_sec_down
+000004d0: 7375 6269 64da 0f75 7064 6174 655f 746f  subid..update_to
+000004e0: 706f 6c6f 6779 5a19 7365 635f 646f 776e  pologyZ.sec_down
+000004f0: 5f73 7562 696e 666f 5f6d 6f73 7464 6f77  _subinfo_mostdow
+00000500: 6e5a 2073 6563 5f64 6f77 6e5f 7375 6269  nZ sec_down_subi
+00000510: 645f 696e 5f73 656c 6563 7465 645f 7375  d_in_selected_su
+00000520: 6269 645a 2473 6563 5f64 6f77 6e5f 7375  bidZ$sec_down_su
+00000530: 6269 6e66 6f5f 646f 776e 7375 625f 696e  binfo_downsub_in
+00000540: 5f73 656c 6563 7465 645a 1a6d 6973 7369  _selectedZ.missi
+00000550: 6e67 5f73 7562 6964 5f69 6e5f 7365 635f  ng_subid_in_sec_
+00000560: 7461 626c 655a 0d68 7973 6864 696e 666f  tableZ.hyshdinfo
+00000570: 5f73 6563 5a09 7375 6269 645f 7365 635a  _secZ.subid_secZ
+00000580: 1175 7073 7472 6561 6d5f 7375 6273 5f73  .upstream_subs_s
+00000590: 6563 5a16 7365 635f 646f 776e 5f73 7562  ecZ.sec_down_sub
+000005a0: 696e 666f 7365 6c65 6374 da04 6d61 736b  infoselect..mask
+000005b0: 5a19 7570 7374 7265 616d 5f73 7562 735f  Z.upstream_subs_
+000005c0: 6e65 775f 7375 625f 7365 63a9 0072 2400  new_sub_sec..r$.
+000005d0: 0000 fa48 633a 5c75 7365 7273 5c6d 3433  ...Hc:\users\m43
+000005e0: 6861 6e5f 325c 646f 6375 6d65 6e74 735c  han_2\documents\
+000005f0: 6769 7468 7562 5c62 6173 696e 6d61 6b65  github\basinmake
+00000600: 725c 6261 7369 6e6d 616b 6572 5c66 756e  r\basinmaker\fun
+00000610: 635c 7064 7461 626c 652e 7079 da29 7570  c\pdtable.py.)up
+00000620: 6461 7465 5f73 656c 6563 7465 645f 7375  date_selected_su
+00000630: 6269 645f 7573 696e 675f 7365 635f 646f  bid_using_sec_do
+00000640: 776e 7375 6269 640d 0000 0073 5e00 0000  wnsubid....s^...
+00000650: 0001 0401 0401 0401 0402 0a01 08ff 0802  ................
+00000660: 0801 02ff 0401 02ff 0606 0201 02ff 0403  ................
+00000670: 0c01 0a07 0a01 02ff 0801 02ff 0603 0c01  ................
+00000680: 0a03 0201 04ff 0601 02ff 0602 0e02 0a01  ................
+00000690: 0a01 02ff 0603 1001 0e01 0601 02ff 1203  ................
+000006a0: 1401 0a02 0401 08ff 0602 0e01 0401 7226  ..............r&
+000006b0: 0000 0063 0400 0000 0000 0000 0000 0000  ...c............
+000006c0: 1000 0000 0600 0000 4300 0000 733a 0100  ........C...s:..
+000006d0: 0064 017d 0464 017d 057c 0064 0264 0367  .d.}.d.}.|.d.d.g
+000006e0: 0219 00a0 0064 04a1 016a 017d 0664 057d  .....d...j.}.d.}
+000006f0: 0764 057d 0874 0264 0574 037c 0183 0183  .d.}.t.d.t.|....
+00000700: 0244 005d 487d 097c 017c 0919 007d 0a74  .D.]H}.|.|...}.t
+00000710: 047c 0a7c 067c 037c 0083 045c 037d 0b7d  .|.|.|.|...\.}.}
+00000720: 007d 087c 077c 0817 007d 077c 0964 056b  .}.|.|...}.|.d.k
+00000730: 0272 687c 0b7d 0c71 3274 056a 067c 0c7c  .rh|.}.q2t.j.|.|
+00000740: 0b66 0264 0564 068d 027d 0c71 3274 05a0  .f.d.d...}.q2t..
+00000750: 077c 0ca1 017d 0c74 056a 0864 0574 0964  .|...}.t.j.d.t.d
+00000760: 078d 027d 0d74 0264 0574 037c 0283 0183  ...}.t.d.t.|....
+00000770: 0244 005d 4a7d 0e7c 027c 0e19 007d 0a7c  .D.]J}.|.|...}.|
+00000780: 0a64 056b 0072 b871 a274 047c 0a7c 067c  .d.k.r.q.t.|.|.|
+00000790: 037c 0083 045c 037d 0b7d 007d 087c 0e64  .|...\.}.}.}.|.d
+000007a0: 056b 0272 da7c 0b7d 0d71 a274 056a 067c  .k.r.|.}.q.t.j.|
+000007b0: 0d7c 0b66 0264 0564 068d 027d 0d71 a274  .|.f.d.d...}.q.t
+000007c0: 037c 0d83 0164 056b 0490 0172 1c74 05a0  .|...d.k...r.t..
+000007d0: 077c 0da1 017d 0d74 05a0 0a7c 0c7c 0da1  .|...}.t...|.|..
+000007e0: 020f 007d 0f7c 0c7c 0f19 007d 0c7c 0764  ...}.|.|...}.|.d
+000007f0: 086b 0590 0172 2c64 097d 086e 0464 017d  .k...r,d.}.n.d.}
+00000800: 087c 0c7c 007c 0866 0353 0029 0a4e 4672  .|.|.|.f.S.).NFr
+00000810: 0600 0000 720d 0000 0072 0900 0000 7201  ....r....r....r.
+00000820: 0000 0072 0e00 0000 2901 da05 6474 7970  ...r....)...dtyp
+00000830: 65e9 0100 0000 5429 0b72 1600 0000 7213  e.....T).r....r.
+00000840: 0000 00da 0572 616e 6765 7215 0000 00da  .....ranger.....
+00000850: 1f72 6574 7572 6e5f 7375 6269 6473 5f64  .return_subids_d
+00000860: 7261 696e 6167 655f 746f 5f73 7562 6964  rainage_to_subid
+00000870: 721a 0000 0072 1b00 0000 da06 756e 6971  r....r......uniq
+00000880: 7565 da05 656d 7074 79da 0369 6e74 da04  ue..empty..int..
+00000890: 696e 3164 2910 721f 0000 00da 0a6d 6f73  in1d).r......mos
+000008a0: 7464 6f77 6e69 645a 0e6d 6f73 7475 7073  tdownidZ.mostups
+000008b0: 7472 6561 6d69 6472 1d00 0000 5a0f 6861  treamidr....Z.ha
+000008c0: 735f 7365 635f 646f 776e 7375 6272 2100  s_sec_downsubr!.
+000008d0: 0000 7220 0000 005a 1373 756d 5f75 7064  ..r ...Z.sum_upd
+000008e0: 6174 655f 746f 706f 6c6f 6779 7222 0000  ate_topologyr"..
+000008f0: 005a 0669 5f64 6f77 6eda 0974 6172 5f73  .Z.i_down..tar_s
+00000900: 7562 6964 721e 0000 005a 0d73 656c 6563  ubidr....Z.selec
+00000910: 7465 645f 7375 6273 5a0b 7265 6d6f 7665  ted_subsZ.remove
+00000920: 5f73 7562 735a 0469 5f75 7072 2300 0000  _subsZ.i_upr#...
+00000930: 7224 0000 0072 2400 0000 7225 0000 00da  r$...r$...r%....
+00000940: 1772 6574 7572 6e5f 6578 7472 6163 7465  .return_extracte
+00000950: 645f 7375 6269 6473 4400 0000 7348 0000  d_subidsD...sH..
+00000960: 0000 0304 0104 0214 0104 0104 0212 0208  ................
+00000970: 0202 0108 ff0a 0208 0108 0106 0204 0108  ................
+00000980: ff08 030a 030e 0212 0208 0208 0102 0202  ................
+00000990: 0108 ff0a 0308 0106 0214 020e 010a 020e  ................
+000009a0: 0208 010a 0106 0204 0172 3100 0000 6304  .........r1...c.
+000009b0: 0000 0000 0000 0000 0000 0006 0000 0005  ................
+000009c0: 0000 0043 0000 0073 3800 0000 7400 7c01  ...C...s8...t.|.
+000009d0: 7c00 8302 7d04 6401 7d05 7401 7c02 8301  |...}.d.}.t.|...
+000009e0: 6401 6b04 722e 7402 7c02 7c04 7c03 7c01  d.k.r.t.|.|.|.|.
+000009f0: 8304 5c03 7d04 7d03 7d05 7c04 7c03 7c05  ..\.}.}.}.|.|.|.
+00000a00: 6603 5300 2902 4e72 0100 0000 2903 7217  f.S.).Nr....).r.
+00000a10: 0000 0072 1500 0000 7226 0000 0029 0672  ...r....r&...).r
+00000a20: 3000 0000 7220 0000 0072 1d00 0000 721f  0...r ...r....r.
+00000a30: 0000 0072 1e00 0000 7222 0000 0072 2400  ...r....r"...r$.
+00000a40: 0000 7224 0000 0072 2500 0000 722a 0000  ..r$...r%...r*..
+00000a50: 007c 0000 0073 0e00 0000 0003 0a01 0402  .|...s..........
+00000a60: 0c01 0201 08ff 0a03 722a 0000 0063 0400  ........r*...c..
+00000a70: 0000 0000 0000 0000 0000 0d00 0000 0500  ................
+00000a80: 0000 4300 0000 7334 0100 007c 0064 016b  ..C...s4...|.d.k
+00000a90: 0172 0c7c 0153 007c 0164 027c 0364 0367  .r.|.S.|.d.|.d.g
+00000aa0: 0319 006a 0064 0464 058d 017d 047c 046a  ...j.d.d...}.|.j
+00000ab0: 0164 0364 0669 0164 078d 017d 047c 046a  .d.d.i.d...}.|.j
+00000ac0: 0264 027c 0367 0264 0864 098d 02a0 03a1  .d.|.g.d.d......
+00000ad0: 007d 0474 046a 057c 047c 0264 0264 0a8d  .}.t.j.|.|.d.d..
+00000ae0: 037d 047c 0464 0619 007c 0464 0b19 001b  .}.|.d...|.d....
+00000af0: 007c 0464 0c3c 007c 046a 0664 0264 0667  .|.d.<.|.j.d.d.g
+00000b00: 0264 0864 0d8d 027d 047c 046a 0764 0267  .d.d...}.|.j.d.g
+00000b10: 0164 0e64 0f8d 026a 0064 0464 058d 017d  .d.d...j.d.d...}
+00000b20: 057c 047c 0464 0c19 007c 006b 0019 0064  .|.|.d...|.k...d
+00000b30: 027c 0367 0219 006a 0064 0464 058d 017d  .|.g...j.d.d...}
+00000b40: 0674 0864 0174 097c 0683 0183 0244 005d  .t.d.t.|.....D.]
+00000b50: 6a7d 077c 0664 0219 006a 0a7c 0719 007d  j}.|.d...j.|...}
+00000b60: 087c 067c 0319 006a 0a7c 0719 007d 097c  .|.|...j.|...}.|
+00000b70: 0164 0219 007c 086b 027d 0a7c 017c 0319  .d...|.k.}.|.|..
+00000b80: 007c 096b 027d 0b74 0ba0 0c7c 0a7c 0ba1  .|.k.}.t...|.|..
+00000b90: 027d 0c7c 056a 0d7c 0564 0219 007c 086b  .}.|.j.|.d...|.k
+00000ba0: 0219 007c 0319 006a 0a64 0119 007c 016a  ...|...j.d...|.j
+00000bb0: 0d7c 0c7c 0366 023c 0071 c47c 0153 0029  .|.|.f.<.q.|.S.)
+00000bc0: 104e 7201 0000 0072 0600 0000 da08 4852  .Nr....r......HR
+00000bd0: 555f 4172 6561 5472 0700 0000 5a09 496e  U_AreaTr....Z.In
+00000be0: 7075 745f 415f 4772 1000 0000 46a9 01da  put_A_Gr....F...
+00000bf0: 0861 735f 696e 6465 7829 0172 0b00 0000  .as_index).r....
+00000c00: da07 4261 735f 415f 475a 0a41 7265 615f  ..Bas_A_GZ.Area_
+00000c10: 7261 7469 6fa9 02da 0262 79da 0961 7363  ratio....by..asc
+00000c20: 656e 6469 6e67 da05 6669 7273 7429 02da  ending..first)..
+00000c30: 0673 7562 7365 74da 046b 6565 7029 0e72  .subset..keep).r
+00000c40: 1400 0000 da06 7265 6e61 6d65 da07 6772  ......rename..gr
+00000c50: 6f75 7062 79da 0373 756d da02 7064 7218  oupby..sum..pdr.
+00000c60: 0000 00da 0b73 6f72 745f 7661 6c75 6573  .....sort_values
+00000c70: da0f 6472 6f70 5f64 7570 6c69 6361 7465  ..drop_duplicate
+00000c80: 7372 2900 0000 7215 0000 0072 1300 0000  sr)...r....r....
+00000c90: 721a 0000 00da 0b6c 6f67 6963 616c 5f61  r......logical_a
+00000ca0: 6e64 7219 0000 0029 0dda 0d6c 616e 6475  ndr....)...landu
+00000cb0: 7365 5f74 6872 6573 da07 6872 7569 6e66  se_thres..hruinf
+00000cc0: 6fda 0873 7562 5f61 7265 61da 0a4c 616e  o..sub_area..Lan
+00000cd0: 6475 7365 5f49 445a 0a73 7562 696e 666f  duse_IDZ.subinfo
+00000ce0: 5f6c 755a 1473 7562 696e 666f 5f6c 755f  _luZ.subinfo_lu_
+00000cf0: 646f 6d69 6e61 7465 645a 1673 7562 696e  dominatedZ.subin
+00000d00: 666f 5f6c 755f 6e65 6564 5f63 6861 6e67  fo_lu_need_chang
+00000d10: 65da 0169 da05 7375 6269 645a 076c 616e  e..i..subidZ.lan
+00000d20: 6475 7365 da05 6d61 736b 31da 056d 6173  duse..mask1..mas
+00000d30: 6b32 7223 0000 0072 2400 0000 7224 0000  k2r#...r$...r$..
+00000d40: 0072 2500 0000 da27 7265 6d6f 7665 5f6c  .r%....'remove_l
+00000d50: 616e 6475 7365 5f74 7970 655f 696e 7075  anduse_type_inpu
+00000d60: 745f 6261 7365 645f 6f6e 5f61 7265 6189  t_based_on_area.
+00000d70: 0000 0073 4800 0000 0002 0801 0402 1601  ...sH...........
+00000d80: 1001 0401 08ff 0a04 1001 1403 0401 08ff  ................
+00000d90: 0602 0401 06ff 0601 02ff 0604 0e01 04ff  ................
+00000da0: 0601 02ff 0603 1201 0e01 0e01 0c01 0c01  ................
+00000db0: 0c01 0a01 02ff 0401 02ff 0401 02ff 1003  ................
+00000dc0: 724b 0000 0063 0700 0000 0000 0000 0000  rK...c..........
+00000dd0: 0000 0e00 0000 0600 0000 4300 0000 73c2  ..........C...s.
+00000de0: 0000 007c 016a 007c 0164 0119 0064 026b  ...|.j.|.d...d.k
+00000df0: 0419 00a0 01a1 007d 077c 016a 007c 0164  .......}.|.j.|.d
+00000e00: 0119 0064 026b 0119 00a0 01a1 007d 087c  ...d.k.......}.|
+00000e10: 0164 0364 0467 0219 006a 0164 0564 068d  .d.d.g...j.d.d..
+00000e20: 017d 097c 096a 0264 0464 0769 0164 088d  .}.|.j.d.d.i.d..
+00000e30: 017d 097c 096a 0364 0367 0164 0964 0a8d  .}.|.j.d.g.d.d..
+00000e40: 02a0 04a1 007d 097c 0064 0219 007d 0a7c  .....}.|.d...}.|
+00000e50: 027c 037c 0567 037d 0b74 0564 0274 067c  .|.|.g.}.t.d.t.|
+00000e60: 0b83 0183 0244 005d 227d 0c7c 0b7c 0c19  .....D.]"}.|.|..
+00000e70: 007d 0d7c 007c 0c19 007d 0a74 077c 0a7c  .}.|.|...}.t.|.|
+00000e80: 087c 097c 0d83 047d 0871 847c 087c 0219  .|.|...}.q.|.|..
+00000e90: 007c 087c 043c 007c 07a0 087c 08a1 017d  .|.|.<.|...|...}
+00000ea0: 017c 0153 0029 0b4e da0a 4852 555f 4973  .|.S.).N..HRU_Is
+00000eb0: 4c61 6b65 7201 0000 0072 0600 0000 7232  Laker....r....r2
+00000ec0: 0000 0054 7207 0000 0072 3500 0000 7210  ...Tr....r5...r.
+00000ed0: 0000 0046 7233 0000 0029 0972 1900 0000  ...Fr3...).r....
+00000ee0: 7214 0000 0072 3c00 0000 723d 0000 0072  r....r<...r=...r
+00000ef0: 3e00 0000 7229 0000 0072 1500 0000 724b  >...r)...r....rK
+00000f00: 0000 00da 0661 7070 656e 6429 0eda 1561  .....append)...a
+00000f10: 7265 615f 7261 7469 6f5f 7468 7265 7368  rea_ratio_thresh
+00000f20: 6f6c 6473 7244 0000 0072 4600 0000 da07  oldsrD...rF.....
+00000f30: 536f 696c 5f49 44da 0656 6567 5f49 44da  Soil_ID..Veg_ID.
+00000f40: 0e4f 7468 6572 5f50 6c79 5f49 445f 31da  .Other_Ply_ID_1.
+00000f50: 0e4f 7468 6572 5f50 6c79 5f49 445f 325a  .Other_Ply_ID_2Z
+00000f60: 0d68 7275 5f6c 616b 655f 696e 666f 5a0d  .hru_lake_infoZ.
+00000f70: 6872 755f 6c61 6e64 5f69 6e66 6f72 4500  hru_land_inforE.
+00000f80: 0000 7243 0000 00da 046c 6973 7472 4700  ..rC.....listrG.
+00000f90: 0000 da04 4974 656d 7224 0000 0072 2400  ....Itemr$...r$.
+00000fa0: 0000 7225 0000 00da 1573 696d 706c 6966  ..r%.....simplif
+00000fb0: 795f 6872 7573 5f6d 6574 686f 6432 ad00  y_hrus_method2..
+00000fc0: 0000 7320 0000 0000 0316 0116 0214 0110  ..s ............
+00000fd0: 0114 0308 010a 0112 0108 0108 0102 0108  ................
+00000fe0: ff06 020c 020a 0272 5500 0000 6303 0000  .......rU...c...
+00000ff0: 0000 0000 0000 0000 001d 0000 0009 0000  ................
+00001000: 0043 0000 0073 8e02 0000 7c01 6401 1900  .C...s....|.d...
+00001010: 7c01 6402 3c00 7400 a001 7c01 6403 1900  |.d.<.t...|.d...
+00001020: 6a02 a101 7d03 7403 6404 7404 7c03 8301  j...}.t.d.t.|...
+00001030: 8302 4400 9002 5d4e 7d04 7c03 7c04 1900  ..D...]N}.|.|...
+00001040: 7d05 7c01 6a05 7c01 6403 1900 7c05 6b02  }.|.j.|.d...|.k.
+00001050: 1900 6a06 6405 6406 8d01 7d06 7400 a007  ..j.d.d...}.t...
+00001060: 7c06 6407 1900 6a02 a101 7d07 7c00 7c07  |.d...j...}.|.|.
+00001070: 1400 7d08 7c06 6a05 7c06 6407 1900 7c08  ..}.|.j.|.d...|.
+00001080: 6b00 1900 a006 a100 7d09 7c06 6a05 7c06  k.......}.|.j.|.
+00001090: 6407 1900 7c08 6b05 1900 a006 a100 7d0a  d...|.k.......}.
+000010a0: 7c0a 6a08 7d0b 7c0b 7c0b 6402 6b03 1900  |.j.}.|.|.d.k...
+000010b0: 7d0b 7c02 6404 1900 7d0c 7c09 6a06 6405  }.|.d...}.|.j.d.
+000010c0: 6406 8d01 7d0d 7400 a001 7c0d 7c0c 1900  d...}.t...|.|...
+000010d0: 6a02 a101 7d0e 7403 6404 7404 7c0e 8301  j...}.t.d.t.|...
+000010e0: 8302 4400 5dbc 7d0f 7c0e 7c0f 1900 7d10  ..D.].}.|.|...}.
+000010f0: 7c0d 6a05 7c0d 7c0c 1900 7c10 6b02 1900  |.j.|.|...|.k...
+00001100: 6a06 6405 6406 8d01 7d11 7400 a007 7c11  j.d.d...}.t...|.
+00001110: 6407 1900 6a02 a101 7d12 7c12 7c08 6b05  d...j...}.|.|.k.
+00001120: 72da 7c11 6a09 6407 6701 6408 6409 8d02  r.|.j.d.g.d.d...
+00001130: 7d11 7403 6404 7404 7c0b 8301 8302 4400  }.t.d.t.|.....D.
+00001140: 5d44 7d13 7c0b 7c13 1900 7d14 7c14 640a  ]D}.|.|...}.|.d.
+00001150: 6b02 9001 7250 9001 7136 7c11 7c14 1900  k...rP..q6|.|...
+00001160: 6a02 6404 1900 7c01 6a05 7c01 6402 1900  j.d...|.j.|.d...
+00001170: a00a 7c11 6402 1900 6a02 a101 7c14 6602  ..|.d...j...|.f.
+00001180: 3c00 9001 7136 7c09 7c09 6402 1900 a00a  <...q6|.|.d.....
+00001190: 7c11 6402 1900 6a02 a101 0f00 1900 7d09  |.d...j.......}.
+000011a0: 71da 7c09 6a0b 7d15 7403 6404 7404 7c15  q.|.j.}.t.d.t.|.
+000011b0: 8301 8302 4400 5dcc 7d16 7c15 7c16 1900  ....D.].}.|.|...
+000011c0: 7d17 7c09 6a05 7c17 6402 6602 1900 7d18  }.|.j.|.d.f...}.
+000011d0: 7403 6404 7404 7c02 8301 8302 4400 5da0  t.d.t.|.....D.].
+000011e0: 7d19 7c02 7c19 1900 7d1a 7c09 6a05 7c17  }.|.|...}.|.j.|.
+000011f0: 7c1a 6602 1900 7d1b 7c0a 6a05 7c0a 7c1a  |.f...}.|.j.|.|.
+00001200: 1900 7c1b 6b02 1900 a006 a100 7d1c 7404  ..|.k.......}.t.
+00001210: 7c1c 8301 6404 6b04 9001 72d4 7c1c 6a09  |...d.k...r.|.j.
+00001220: 6407 6408 6409 8d02 7d1c 7403 6404 7404  d.d.d...}.t.d.t.
+00001230: 7c0b 8301 8302 4400 5d3c 7d13 7c0b 7c13  |.....D.]<}.|.|.
+00001240: 1900 7d14 7c14 640a 6b02 9002 7248 9002  ..}.|.d.k...rH..
+00001250: 712e 7c1c 7c14 1900 6a02 6404 1900 7c01  q.|.|...j.d...|.
+00001260: 6a05 7c01 6402 1900 7c18 6b02 7c14 6602  j.|.d...|.k.|.f.
+00001270: 3c00 9002 712e 6e04 9001 71d4 9001 71d4  <...q.n...q...q.
+00001280: 9001 71ac 712a 7c01 6a0c 6402 6701 640b  ..q.q*|.j.d.g.d.
+00001290: 8d01 7d01 7c01 5300 290c 4eda 0a48 5255  ..}.|.S.).N..HRU
+000012a0: 5f49 445f 4e65 775a 0b48 5255 5f49 445f  _ID_NewZ.HRU_ID_
+000012b0: 4e65 7732 7206 0000 0072 0100 0000 5472  New2r....r....Tr
+000012c0: 0700 0000 7232 0000 0046 7236 0000 00da  ....r2...Fr6....
+000012d0: 0553 4841 5045 7210 0000 0029 0d72 1a00  .SHAPEr....).r..
+000012e0: 0000 722b 0000 0072 1300 0000 7229 0000  ..r+...r....r)..
+000012f0: 0072 1500 0000 7219 0000 0072 1400 0000  .r....r....r....
+00001300: 723e 0000 0072 1100 0000 7240 0000 0072  r>...r....r@...r
+00001310: 1200 0000 da05 696e 6465 7872 1c00 0000  ......indexr....
+00001320: 291d 5a14 6d69 6e5f 6872 755f 7063 745f  ).Z.min_hru_pct_
+00001330: 7375 625f 6172 6561 7244 0000 00da 1069  sub_arearD.....i
+00001340: 6d70 6f72 7461 6e63 655f 6f72 6465 725a  mportance_orderZ
+00001350: 0673 7562 6964 7372 4700 0000 7248 0000  .subidsrG...rH..
+00001360: 005a 0c73 7562 5f68 7275 5f69 6e66 6f5a  .Z.sub_hru_infoZ
+00001370: 0873 7562 6173 7265 615a 0c73 7562 6172  .subasreaZ.subar
+00001380: 6561 5f74 6872 735a 106e 6565 645f 7265  ea_thrsZ.need_re
+00001390: 6d6f 7665 5f68 7275 735a 0967 6f6f 645f  move_hrusZ.good_
+000013a0: 6872 7573 5a0b 6872 755f 636f 6c75 6d6e  hrusZ.hru_column
+000013b0: 735a 0663 6f6c 6e6d 315a 1c69 6d70 6f72  sZ.colnm1Z.impor
+000013c0: 7431 5f41 7265 615f 6e65 6564 5f72 656d  t1_Area_need_rem
+000013d0: 6f76 655f 6872 755a 0e75 6e69 7175 655f  ove_hruZ.unique_
+000013e0: 696d 706f 7274 315a 0869 5f69 6d70 6f72  import1Z.i_impor
+000013f0: 745a 0869 5f63 6f6c 6e6d 315a 1e69 5f69  tZ.i_colnm1Z.i_i
+00001400: 6d70 6f72 7431 5f41 7265 615f 6e65 6564  mport1_Area_need
+00001410: 5f72 656d 6f76 655f 6872 755a 2774 6f74  _remove_hruZ'tot
+00001420: 616c 5f61 7265 615f 695f 696d 706f 7274  al_area_i_import
+00001430: 5f69 6e5f 6e65 6564 5f72 656d 6f76 655f  _in_need_remove_
+00001440: 6872 7573 5a04 695f 6e6d 5a0a 636f 6c75  hrusZ.i_nmZ.colu
+00001450: 6d6e 6e61 6d65 da07 696e 6465 7865 73da  mnname..indexes.
+00001460: 016a da03 6964 78da 0568 7275 6964 da01  .j..idx..hruid..
+00001470: 6b5a 0563 6f6c 6e6d 5a10 6174 7472 695f  kZ.colnmZ.attri_
+00001480: 7265 6d6f 7665 5f68 7275 5a0b 676f 6f64  remove_hruZ.good
+00001490: 5f68 7275 735f 6b72 2400 0000 7224 0000  _hrus_kr$...r$..
+000014a0: 0072 2500 0000 da0e 7369 6d70 6c69 6466  .r%.....simplidf
+000014b0: 795f 6872 7573 c600 0000 7384 0000 0000  y_hrus....s.....
+000014c0: 020c 0210 0314 0108 021a 0210 0108 0316  ................
+000014d0: 030a 0102 ff0a 0306 020c 0308 010c 0110  ................
+000014e0: 0512 0108 0112 0102 ff06 0204 0108 ff04  ................
+000014f0: 0608 0304 0106 ff06 0212 0108 010a 0104  ................
+00001500: 030c ff0c 0108 ff02 0102 ff08 040a 0108  ................
+00001510: ff0a 0306 0412 0108 010e 0412 0108 020e  ................
+00001520: 030a 0102 ff0a 030e 0204 0104 ff06 0212  ................
+00001530: 0108 010a 0104 030c ff0e 0102 ff0a 030e  ................
+00001540: 010e 0172 5f00 0000 6301 0000 0000 0000  ...r_...c.......
+00001550: 0000 0000 000b 0000 0005 0000 0043 0000  .............C..
+00001560: 0073 e601 0000 7c00 6401 6402 6702 1900  .s....|.d.d.g...
+00001570: a000 6403 a101 6a01 7d01 7c00 6a02 7c00  ..d...j.}.|.j.|.
+00001580: 6404 1900 6405 6b02 1900 a003 a100 7d02  d...d.k.......}.
+00001590: 7c02 6401 1900 a003 a100 7d03 7c00 6406  |.d.......}.|.d.
+000015a0: 1900 a004 a100 7d04 7405 6407 7406 7c02  ......}.t.d.t.|.
+000015b0: 8301 8302 4400 9001 5d8e 7d05 7c02 6401  ....D...].}.|.d.
+000015c0: 1900 6a01 7c05 1900 7d06 7c02 6402 1900  ..j.|...}.|.d...
+000015d0: 6a01 7c05 1900 7d07 7c00 6a02 7c00 6401  j.|...}.|.j.|.d.
+000015e0: 1900 7c07 6b02 1900 a003 a100 7d08 7c07  ..|.k.......}.|.
+000015f0: 7d09 7406 7c08 8301 6408 6b00 72e4 6408  }.t.|...d.k.r.d.
+00001600: 7c00 6a02 7c00 6401 1900 7c06 6b02 6409  |.j.|.d...|.k.d.
+00001610: 6602 3c00 7c04 7c05 1700 6408 1700 7c00  f.<.|.|...d...|.
+00001620: 6a02 7c00 6401 1900 7c06 6b02 6406 6602  j.|.d...|.k.d.f.
+00001630: 3c00 6408 7c00 6a02 7c00 6401 1900 7c06  <.d.|.j.|.d...|.
+00001640: 6b02 640a 6602 3c00 7150 7c08 6404 1900  k.d.f.<.qP|.d...
+00001650: 6a01 6407 1900 6405 6b02 9001 7274 7c00  j.d...d.k...rt|.
+00001660: 6a02 7c00 6401 1900 7c09 6b02 1900 a003  j.|.d...|.k.....
+00001670: a100 7d0a 7c0a 6402 1900 6a01 6407 1900  ..}.|.d...j.d...
+00001680: 7d07 7c00 6a02 7c00 6401 1900 7c07 6b02  }.|.j.|.d...|.k.
+00001690: 1900 a003 a100 7d08 7406 7c08 8301 6408  ......}.t.|...d.
+000016a0: 6b00 9001 7248 640b 7d09 9001 7174 7c09  k...rHd.}...qt|.
+000016b0: 7c08 6402 1900 6a01 6407 1900 6b02 9001  |.d...j.d...k...
+000016c0: 726e 7407 7c09 7c07 8302 0100 640b 7d09  rnt.|.|.....d.}.
+000016d0: 9001 7174 7c07 7d09 71e4 7c09 640b 6b02  ..qt|.}.q.|.d.k.
+000016e0: 9001 7280 7150 7c08 6409 1900 6a01 6407  ..r.qP|.d...j.d.
+000016f0: 1900 7c00 6a02 7c00 6401 1900 7c06 6b02  ..|.j.|.d...|.k.
+00001700: 6409 6602 3c00 7c08 6406 1900 6a01 6407  d.f.<.|.d...j.d.
+00001710: 1900 7c00 6a02 7c00 6401 1900 7c06 6b02  ..|.j.|.d...|.k.
+00001720: 6406 6602 3c00 7c08 640a 1900 6a01 6407  d.f.<.|.d...j.d.
+00001730: 1900 7c00 6a02 7c00 6401 1900 7c06 6b02  ..|.j.|.d...|.k.
+00001740: 640a 6602 3c00 7150 7c00 5300 290c 4e72  d.f.<.qP|.S.).Nr
+00001750: 0600 0000 720d 0000 00da 0566 6c6f 6174  ....r......float
+00001760: da08 4c61 6b65 5f43 6174 e902 0000 00da  ..Lake_Cat......
+00001770: 0653 6567 5f49 4472 0100 0000 7228 0000  .Seg_IDr....r(..
+00001780: 00da 0853 7472 6168 6c65 72da 0953 6567  ...Strahler..Seg
+00001790: 5f6f 7264 6572 e9ff ffff ff29 0872 1600  _order.....).r..
+000017a0: 0000 7213 0000 0072 1900 0000 7214 0000  ..r....r....r...
+000017b0: 00da 036d 6178 7229 0000 0072 1500 0000  ...maxr)...r....
+000017c0: da05 7072 696e 7429 0bda 0763 6174 696e  ..print)...catin
+000017d0: 666f da0c 726f 7574 696e 675f 696e 666f  fo..routing_info
+000017e0: 5a15 6361 7469 6e66 6f5f 6e6f 6e5f 636f  Z.catinfo_non_co
+000017f0: 6e6e 6563 7465 645a 0963 6174 6964 735f  nnectedZ.catids_
+00001800: 6e63 5a0a 6d61 785f 7365 675f 6964 7247  ncZ.max_seg_idrG
+00001810: 0000 005a 0763 5f73 7562 6964 5a07 645f  ...Z.c_subidZ.d_
+00001820: 7375 6269 645a 0a64 5f73 7562 5f69 6e66  subidZ.d_sub_inf
+00001830: 6f5a 086c 635f 7375 6269 645a 0d6c 635f  oZ.lc_subidZ.lc_
+00001840: 7375 6269 645f 696e 666f 7224 0000 0072  subid_infor$...r
+00001850: 2400 0000 7225 0000 00da 2375 7064 6174  $...r%....#updat
+00001860: 655f 6e6f 6e5f 636f 6e6e 6563 7465 645f  e_non_connected_
+00001870: 6361 7463 686d 656e 745f 696e 666f 2701  catchment_info'.
+00001880: 0000 735e 0000 0000 0114 0116 020c 010c  ..s^............
+00001890: 0514 010e 010e 0116 0204 0a0c 0116 020a  ................
+000018a0: ff0e 0102 ff04 0216 0102 0614 0116 010e  ................
+000018b0: 0116 010e 0104 0104 0114 010a 0104 0104  ................
+000018c0: 0106 020a 0102 1502 0102 ff04 0202 fe16  ................
+000018d0: 0302 0102 ff04 0202 fe16 0302 0102 ff04  ................
+000018e0: 0202 fe18 0472 6b00 0000 6301 0000 0000  .....rk...c.....
+000018f0: 0000 0000 0000 0010 0000 0006 0000 0043  ...............C
+00001900: 0000 0073 be01 0000 7c00 6a00 6401 6701  ...s....|.j.d.g.
+00001910: 6402 6403 8d02 7d01 7401 a002 6404 6405  d.d...}.t...d.d.
+00001920: a102 7d02 6406 7d03 7401 a002 6407 6408  ..}.d.}.t...d.d.
+00001930: a102 7d04 7c01 6409 1900 6a03 6405 1900  ..}.|.d...j.d...
+00001940: 7d05 6406 7d06 7c05 7c04 7c03 6406 1800  }.d.}.|.|.|.d...
+00001950: 3c00 7404 7c04 7c04 6405 6b04 1900 8301  <.t.|.|.d.k.....
+00001960: 6405 6b04 9001 72b2 7401 a002 6407 6408  d.k...r.t...d.d.
+00001970: a102 7d07 7c06 7d03 7405 6405 7c06 8302  ..}.|.}.t.d.|...
+00001980: 4400 9001 5d2a 7d08 7c04 7c08 1900 7d09  D...]*}.|.|...}.
+00001990: 7c09 6405 6b00 7292 717a 7c01 6a06 7c01  |.d.k.r.qz|.j.|.
+000019a0: 6409 1900 7c09 6b02 640a 6602 1900 7c02  d...|.k.d.f...|.
+000019b0: 7c08 1900 1700 7c02 7c08 3c00 7c01 6a06  |.....|.|.<.|.j.
+000019c0: 7c01 6409 1900 7c09 6b02 640b 6602 1900  |.d...|.k.d.f...
+000019d0: 6a03 6405 1900 7d0a 7c01 6a06 7c01 640c  j.d...}.|.j.|.d.
+000019e0: 1900 7c09 6b02 1900 7d0b 7404 7c0b 8301  ..|.k...}.t.|...
+000019f0: 6405 6b01 72f0 717a 7c0b 6a06 7c0b 640b  d.k.r.qz|.j.|.d.
+00001a00: 1900 7c0a 6b02 1900 7d0c 7404 7c0c 8301  ..|.k...}.t.|...
+00001a10: 6405 6b04 9001 7226 7c0c 6409 1900 6a03  d.k...r&|.d...j.
+00001a20: 6405 1900 7c07 7c08 3c00 717a 717a 7c0b  d...|.|.<.qzqz|.
+00001a30: 6a06 7c0b 640b 1900 7c0a 6406 1800 6b02  j.|.d...|.d...k.
+00001a40: 1900 7d0d 7405 6405 7404 7c0d 8301 8302  ..}.t.d.t.|.....
+00001a50: 4400 5d5a 7d0e 7c0e 6405 6b02 9001 726c  D.]Z}.|.d.k...rl
+00001a60: 7c0d 6409 1900 6a03 7c0e 1900 7c07 7c08  |.d...j.|...|.|.
+00001a70: 3c00 6e36 7c0d 6409 1900 6a03 7c0e 1900  <.n6|.d...j.|...
+00001a80: 7c07 7c03 6406 1700 6406 1800 3c00 7c02  |.|.d...d...<.|.
+00001a90: 7c08 1900 7c02 7c03 6406 1700 6406 1800  |...|.|.d...d...
+00001aa0: 3c00 7c03 6406 1700 7d03 9001 714a 717a  <.|.d...}...qJqz
+00001ab0: 7c07 7d04 7c03 7d06 714a 7407 7c02 8301  |.}.|.}.qJt.|...
+00001ac0: 7d0f 7c0f 5300 290d 4eda 0944 7261 696e  }.|.S.).N..Drain
+00001ad0: 4172 6561 46a9 0172 3800 0000 e964 0000  AreaF..r8....d..
+00001ae0: 0072 0100 0000 7228 0000 00e9 e803 0000  .r....r(........
+00001af0: 7266 0000 0072 0600 0000 da09 5269 764c  rf...r......RivL
+00001b00: 656e 6774 6872 6400 0000 720d 0000 0029  engthrd...r....)
+00001b10: 0872 4000 0000 721a 0000 00da 0466 756c  .r@...r......ful
+00001b20: 6c72 1300 0000 7215 0000 0072 2900 0000  lr....r....r)...
+00001b30: 7219 0000 0072 6700 0000 2910 da11 6d61  r....rg...)...ma
+00001b40: 696e 7269 765f 6d65 7267 5f69 6e66 6f5a  inriv_merg_infoZ
+00001b50: 166d 6169 6e72 6976 5f6d 6572 675f 696e  .mainriv_merg_in
+00001b60: 666f 5f73 6f72 745a 136c 6f6e 6765 7374  fo_sortZ.longest
+00001b70: 5f66 6c6f 775f 7061 7468 6573 da05 6e70  _flow_pathes..np
+00001b80: 6174 685a 0650 6174 6869 6472 4800 0000  athZ.PathidrH...
+00001b90: 5a0d 6e70 6174 685f 6375 7272 656e 745a  Z.npath_currentZ
+00001ba0: 076e 5061 7468 6964 da05 6970 6174 685a  .nPathid..ipathZ
+00001bb0: 0d63 5f73 7562 6964 5f69 7061 7468 5a14  .c_subid_ipathZ.
+00001bc0: 5374 7261 686c 6572 5f6f 7264 6572 5f69  Strahler_order_i
+00001bd0: 7061 7468 5a12 7570 7374 7265 616d 5f73  pathZ.upstream_s
+00001be0: 7562 5f69 6e66 6f73 5a1e 7570 7374 7265  ub_infosZ.upstre
+00001bf0: 616d 5f73 7562 5f69 6e66 6f73 5f65 715f  am_sub_infos_eq_
+00001c00: 5374 7261 686c 6572 5a20 7570 7374 7265  StrahlerZ upstre
+00001c10: 616d 5f73 7562 5f69 6e66 6f73 5f65 715f  am_sub_infos_eq_
+00001c20: 5374 7261 686c 6572 5f31 5a06 696e 7061  Strahler_1Z.inpa
+00001c30: 7468 5a0b 4c6f 6e67 6573 7470 6174 6872  thZ.Longestpathr
+00001c40: 2400 0000 7224 0000 0072 2500 0000 da1a  $...r$...r%.....
+00001c50: 4361 6c63 756c 6174 655f 4c6f 6e67 6573  Calculate_Longes
+00001c60: 745f 666c 6f77 7061 7468 7b01 0000 7386  t_flowpath{...s.
+00001c70: 0000 0000 0104 0106 ff06 030c 0204 030c  ................
+00001c80: 010e 0104 010c 0216 010c 0104 0510 0108  ................
+00001c90: 0306 ff02 0302 0304 010e ff02 0306 fd02  ................
+00001ca0: ff06 0604 010e ff04 0202 fe04 0404 010a  ................
+00001cb0: ff04 050a ff02 0402 0504 010a ff04 050a  ................
+00001cc0: ff04 0308 0102 ff08 0304 0204 010e ff04  ................
+00001cd0: 0412 020a 0102 0102 ff04 0202 fe0a 0502  ................
+00001ce0: 0102 ff04 0202 fe10 0406 ff08 0102 ff04  ................
+00001cf0: 030e 0204 0106 0108 0272 7500 0000 e932  .........ru....2
+00001d00: 0000 00e9 0f00 0000 6303 0000 0000 0000  ........c.......
+00001d10: 0000 0000 0024 0000 000c 0000 0043 0000  .....$.......C..
+00001d20: 0073 6e06 0000 7c00 6a00 6401 6402 8d01  .sn...|.j.d.d...
+00001d30: 7d03 6403 7d04 6403 7c00 6a01 7601 721e  }.d.}.d.|.j.v.r.
+00001d40: 6404 7d04 7c00 6405 1900 6406 1b00 6406  d.}.|.d...d...d.
+00001d50: 1b00 7c01 6b00 7d05 7c00 6407 1900 6406  ..|.k.}.|.d...d.
+00001d60: 1b00 7c02 6b00 7d06 7c00 7402 a003 7c05  ..|.k.}.|.t...|.
+00001d70: 7c06 a102 1900 6a00 6401 6402 8d01 7d07  |.....j.d.d...}.
+00001d80: 7c07 7c07 6408 1900 6409 6b02 1900 6a00  |.|.d...d.k...j.
+00001d90: 6401 6402 8d01 7d07 7c07 7c07 7c04 1900  d.d...}.|.|.|...
+00001da0: 6409 6b02 1900 6a00 6401 6402 8d01 7d07  d.k...j.d.d...}.
+00001db0: 7c07 6a04 640a 640b 6702 6401 640c 8d02  |.j.d.d.g.d.d...
+00001dc0: 7d07 7405 6409 7406 7c07 8301 8302 4400  }.t.d.t.|.....D.
+00001dd0: 9005 5dbc 7d08 7c07 640d 1900 6a07 7c08  ..].}.|.d...j.|.
+00001de0: 1900 7d09 7c07 640e 1900 6a07 7c08 1900  ..}.|.d...j.|...
+00001df0: 7d0a 7c07 640f 1900 6a07 7c08 1900 7d0b  }.|.d...j.|...}.
+00001e00: 7c07 6408 1900 6a07 7c08 1900 6409 6b02  |.d...j.|...d.k.
+00001e10: 7d0c 7c07 7c04 1900 6a07 7c08 1900 6409  }.|.|...j.|...d.
+00001e20: 6b01 7d0d 7c00 7c00 640d 1900 7c0a 6b02  k.}.|.|.d...|.k.
+00001e30: 1900 6a00 6401 6402 8d01 7d0e 7c00 7c00  ..j.d.d...}.|.|.
+00001e40: 640e 1900 7c09 6b02 1900 6a00 6401 6402  d...|.k...j.d.d.
+00001e50: 8d01 7d0f 7406 7c0e 8301 6409 6b04 9001  ..}.t.|...d.k...
+00001e60: 727e 6401 7d10 7c0e 640f 1900 6a07 6409  r~d.}.|.d...j.d.
+00001e70: 1900 7c0b 6b02 9001 725a 6401 7d11 6e04  ..|.k...rZd.}.n.
+00001e80: 6410 7d11 7c0e 6408 1900 6a07 6409 1900  d.}.|.d...j.d...
+00001e90: 6409 6b04 9001 7278 6401 7d12 6e04 6410  d.k...rxd.}.n.d.
+00001ea0: 7d12 6e0c 6410 7d10 6410 7d11 6410 7d12  }.n.d.}.d.}.d.}.
+00001eb0: 6411 7d13 7c10 9002 7208 7c11 9002 7208  d.}.|...r.|...r.
+00001ec0: 7c0c 9002 7208 7c0d 9002 7208 7c03 7c03  |...r.|...r.|.|.
+00001ed0: 640d 1900 7c0e 640d 1900 6a07 6409 1900  d...|.d...j.d...
+00001ee0: 6b02 1900 6a00 6401 6402 8d01 7d14 6401  k...j.d.d...}.d.
+00001ef0: 7d15 7c03 7c03 640d 1900 7c0e 640d 1900  }.|.|.d...|.d...
+00001f00: 6a07 6409 1900 6b02 1900 6a00 6401 6402  j.d...k...j.d.d.
+00001f10: 8d01 7d16 7c16 640e 1900 6a07 6409 1900  ..}.|.d...j.d...
+00001f20: 7d17 6401 7d18 6412 7d13 9001 6ea0 7c12  }.d.}.d.}...n.|.
+00001f30: 9002 727c 7c10 9002 727c 7c13 6411 6b02  ..r||...r||.d.k.
+00001f40: 9002 727c 7c03 7c03 640d 1900 7c0e 640d  ..r||.|.d...|.d.
+00001f50: 1900 6a07 6409 1900 6b02 1900 6a00 6401  ..j.d...k...j.d.
+00001f60: 6402 8d01 7d14 6401 7d15 7c03 7c03 640d  d...}.d.}.|.|.d.
+00001f70: 1900 7c0e 640d 1900 6a07 6409 1900 6b02  ..|.d...j.d...k.
+00001f80: 1900 6a00 6401 6402 8d01 7d16 7c16 640e  ..j.d.d...}.|.d.
+00001f90: 1900 6a07 6409 1900 7d17 6410 7d18 9001  ..j.d...}.d.}...
+00001fa0: 6e2c 7c10 9003 7270 7c13 6411 6b02 9003  n,|...rp|.d.k...
+00001fb0: 7270 7c03 7c03 640d 1900 7c0e 640d 1900  rp|.|.d...|.d...
+00001fc0: 6a07 6409 1900 6b02 1900 6a00 6401 6402  j.d...k...j.d.d.
+00001fd0: 8d01 7d14 7c03 7c03 640d 1900 7c0e 640d  ..}.|.|.d...|.d.
+00001fe0: 1900 6a07 6409 1900 6b02 1900 6a00 6401  ..j.d...k...j.d.
+00001ff0: 6402 8d01 7d16 7c16 640e 1900 6a07 6409  d...}.|.d...j.d.
+00002000: 1900 7d17 7c00 7c00 640e 1900 7c0a 6b02  ..}.|.|.d...|.k.
+00002010: 1900 6a00 6401 6402 8d01 7d19 7402 a008  ..j.d.d...}.t...
+00002020: 7c19 640d 1900 6a07 a101 7d1a 7402 a009  |.d...j...}.t...
+00002030: 7c1a 7c07 640d 1900 6a07 a102 7d1b 7406  |.|.d...j...}.t.
+00002040: 7c1b 8301 6412 6b02 9003 7230 6401 7d18  |...d.k...r0d.}.
+00002050: 6401 7d15 6e3e 7c19 7c19 640d 1900 a00a  d.}.n>|.|.d.....
+00002060: 7c1b a101 1900 6a04 640b 6410 640c 8d02  |.....j.d.d.d...
+00002070: 7d1c 7c09 7c1c 640d 1900 6a07 6409 1900  }.|.|.d...j.d...
+00002080: 6b03 9003 7266 6410 7d18 6e04 6401 7d18  k...rfd.}.n.d.}.
+00002090: 6401 7d15 6e38 6410 7d15 7c0a 6409 6b04  d.}.n8d.}.|.d.k.
+000020a0: 9003 72a2 740b 7c09 7c10 7c11 7c0c 7c0d  ..r.t.|.|.|.|.|.
+000020b0: 7c10 7406 7c00 7c00 640f 1900 7c0b 6b02  |.t.|.|.d...|.k.
+000020c0: 1900 8301 8307 0100 6700 7d14 71aa 7c15  ........g.}.q.|.
+000020d0: 72aa 7c03 640d 1900 7c09 6b02 7d1d 7c03  r.|.d...|.k.}.|.
+000020e0: 6413 1900 7c09 6b02 7d1e 7c03 6413 1900  d...|.k.}.|.d...
+000020f0: 7c14 6413 1900 6a07 6409 1900 6b02 7d1f  |.d...j.d...k.}.
+00002100: 7402 a003 7c1d 7c1f a102 7d20 7402 a003  t...|.|...} t...
+00002110: 7c20 7c1e a102 7d21 7406 7c14 8301 6412  | |...}!t.|...d.
+00002120: 6b04 9004 7234 7406 7402 a008 7c14 6414  k...r4t.t...|.d.
+00002130: 1900 6a07 a101 8301 6412 6b04 9004 7234  ..j.....d.k...r4
+00002140: 740b 7c09 7c0b 8302 0100 740b 7c14 6700  t.|.|.....t.|.g.
+00002150: 6415 a201 1900 8301 0100 7c03 7c03 640d  d.........|.|.d.
+00002160: 1900 a00a 7c09 7c0e 640d 1900 6a07 6409  ....|.|.d...j.d.
+00002170: 1900 6702 a101 1900 7d22 7402 a00c 7c22  ..g.....}"t...|"
+00002180: 6405 1900 6a07 a101 7c03 6a0d 7c21 6405  d...j...|.j.|!d.
+00002190: 6602 3c00 7402 6a0e 7c22 6416 1900 6a07  f.<.t.j.|"d...j.
+000021a0: 7c22 6405 1900 6a07 6417 8d02 7c03 6a0d  |"d...j.d...|.j.
+000021b0: 7c21 6416 6602 3c00 7402 6a0e 7c22 6418  |!d.f.<.t.j.|"d.
+000021c0: 1900 6a07 7c22 6405 1900 6a07 6417 8d02  ..j.|"d...j.d...
+000021d0: 7c03 6a0d 7c21 6418 6602 3c00 7402 6a0e  |.j.|!d.f.<.t.j.
+000021e0: 7c22 6419 1900 6a07 7c22 6405 1900 6a07  |"d...j.|"d...j.
+000021f0: 6417 8d02 7c03 6a0d 7c21 6419 6602 3c00  d...|.j.|!d.f.<.
+00002200: 7c14 6a01 4400 9001 5d84 7d23 7c23 6407  |.j.D...].}#|#d.
+00002210: 6b02 9005 7214 7c18 9005 7214 7402 a00c  k...r.|...r.t...
+00002220: 7c22 6407 1900 6a07 a101 7c03 6a0d 7c21  |"d...j...|.j.|!
+00002230: 6407 6602 3c00 9004 71e0 7c23 641a 7600  d.f.<...q.|#d.v.
+00002240: 9005 724c 7c18 9005 724c 7402 6a0e 7c22  ..rL|...rLt.j.|"
+00002250: 7c23 1900 6a07 7c22 7c23 1900 6a07 6417  |#..j.|"|#..j.d.
+00002260: 8d02 7c03 6a0d 7c21 7c23 6602 3c00 9004  ..|.j.|!|#f.<...
+00002270: 71e0 7c23 641b 7600 9005 7278 7c18 9005  q.|#d.v...rx|...
+00002280: 7278 7402 a00f 7c22 7c23 1900 6a07 a101  rxt...|"|#..j...
+00002290: 7c03 6a0d 7c21 7c23 6602 3c00 6eec 7c23  |.j.|!|#f.<.n.|#
+000022a0: 641c 7600 9005 72a4 7c18 9005 72a4 7402  d.v...r.|...r.t.
+000022b0: a010 7c22 7c23 1900 6a07 a101 7c03 6a0d  ..|"|#..j...|.j.
+000022c0: 7c21 7c23 6602 3c00 6ec0 7c23 640d 6b02  |!|#f.<.n.|#d.k.
+000022d0: 9005 72c8 7c14 6413 1900 6a07 6409 1900  ..r.|.d...j.d...
+000022e0: 7c03 6a0d 7c21 6413 6602 3c00 6e9c 7c23  |.j.|!d.f.<.n.|#
+000022f0: 640e 6b02 9005 72e2 7c17 7c03 6a0d 7c21  d.k...r.|.|.j.|!
+00002300: 7c23 6602 3c00 6e82 7c23 6413 6b02 9004  |#f.<.n.|#d.k...
+00002310: 73e0 7c23 641d 6b02 9004 73e0 7c23 641e  s.|#d.k...s.|#d.
+00002320: 6b02 9004 73e0 7c23 641f 6b02 9004 73e0  k...s.|#d.k...s.
+00002330: 7c23 6420 6b02 9004 73e0 7c23 6421 6b02  |#d k...s.|#d!k.
+00002340: 9004 73e0 7c23 6405 6b02 9004 73e0 7c23  ..s.|#d.k...s.|#
+00002350: 6416 6b02 9004 73e0 7c23 6418 6b02 9004  d.k...s.|#d.k...
+00002360: 73e0 7c23 6419 6b02 9006 724c 9004 71e0  s.|#d.k...rL..q.
+00002370: 6e18 7c14 7c23 1900 6a07 6409 1900 7c03  n.|.|#..j.d...|.
+00002380: 6a0d 7c21 7c23 6602 3c00 9004 71e0 71aa  j.|!|#f.<...q.q.
+00002390: 7c03 5300 2922 4e54 7207 0000 00da 0748  |.S.)"NTr......H
+000023a0: 6173 5f50 4f49 da09 4861 735f 4761 7567  as_POI..Has_Gaug
+000023b0: 65da 0742 6173 4172 6561 726f 0000 0072  e..BasArearo...r
+000023c0: 7000 0000 7261 0000 0072 0100 0000 7264  p...ra...r....rd
+000023d0: 0000 0072 6c00 0000 726d 0000 0072 0600  ...rl...rm...r..
+000023e0: 0000 720d 0000 0072 6300 0000 4672 6600  ..r....rc...Frf.
+000023f0: 0000 7228 0000 00da 066e 7375 6269 64da  ..r(.....nsubid.
+00002400: 0848 794c 616b 6549 6429 0472 0600 0000  .HyLakeId).r....
+00002410: 720d 0000 0072 6300 0000 727c 0000 00da  r....rc...r|....
+00002420: 0842 6173 536c 6f70 65a9 01da 0777 6569  .BasSlope....wei
+00002430: 6768 7473 da08 4d65 616e 456c 6576 da09  ghts..MeanElev..
+00002440: 4261 7341 7370 6563 7429 04da 0852 6976  BasAspect)...Riv
+00002450: 536c 6f70 65da 0846 6c6f 6f64 505f 6eda  Slope..FloodP_n.
+00002460: 0651 5f4d 6561 6eda 0443 685f 6e29 01da  .Q_Mean..Ch_n)..
+00002470: 074d 6178 5f44 454d 2901 da07 4d69 6e5f  .Max_DEM)...Min_
+00002480: 4445 4dda 0a6e 646f 776e 7375 6269 64da  DEM..ndownsubid.
+00002490: 094f 6c64 5f53 7562 4964 da0c 4f6c 645f  .Old_SubId..Old_
+000024a0: 446f 7753 7562 4964 7257 0000 00da 0867  DowSubIdrW.....g
+000024b0: 656f 6d65 7472 7929 1172 1400 0000 7211  eometry).r....r.
+000024c0: 0000 0072 1a00 0000 da0a 6c6f 6769 6361  ...r......logica
+000024d0: 6c5f 6f72 7240 0000 0072 2900 0000 7215  l_orr@...r)...r.
+000024e0: 0000 0072 1300 0000 722b 0000 00da 0b69  ...r....r+.....i
+000024f0: 6e74 6572 7365 6374 3164 7212 0000 0072  ntersect1dr....r
+00002500: 6800 0000 723e 0000 0072 1900 0000 da07  h...r>...r......
+00002510: 6176 6572 6167 6572 6700 0000 da03 6d69  averagerg.....mi
+00002520: 6e29 24da 0e6d 6170 6f6c 646e 6577 5f69  n)$..mapoldnew_i
+00002530: 6e66 6fda 0f61 7265 615f 7468 7265 7374  nfo..area_threst
+00002540: 686f 6c64 da11 6c65 6e67 7468 5f74 6872  hold..length_thr
+00002550: 6573 7468 6f6c 645a 126d 6170 6f6c 646e  estholdZ.mapoldn
+00002560: 6577 5f69 6e66 6f5f 6e65 77da 0e47 6175  ew_info_new..Gau
+00002570: 6765 5f63 6f6c 5f4e 616d 655a 0b61 7265  ge_col_NameZ.are
+00002580: 615f 6669 6c74 6572 5a0d 6c65 6e67 7468  a_filterZ.length
+00002590: 5f66 696c 7465 725a 1273 6d61 6c6c 5f73  _filterZ.small_s
+000025a0: 7562 5f6e 6f6e 5f6c 616b 6572 4700 0000  ub_non_lakerG...
+000025b0: 5a0c 736d 616c 6c5f 7375 625f 6964 5a10  Z.small_sub_idZ.
+000025c0: 736d 616c 6c5f 646f 776e 7375 625f 6964  small_downsub_id
+000025d0: 5a10 736d 616c 6c5f 7375 625f 7365 675f  Z.small_sub_seg_
+000025e0: 6964 5a15 736d 616c 6c5f 7375 625f 6973  idZ.small_sub_is
+000025f0: 5f6e 6f74 5f4c 616b 655a 1673 6d61 6c6c  _not_LakeZ.small
+00002600: 5f73 7562 5f69 735f 6e6f 745f 6761 7567  _sub_is_not_gaug
+00002610: 655a 0d64 6f77 6e5f 7375 625f 696e 666f  eZ.down_sub_info
+00002620: 5a11 7570 7374 7265 616d 5f73 7562 5f69  Z.upstream_sub_i
+00002630: 6e66 6f5a 0c68 6173 5f64 6f77 6e5f 7375  nfoZ.has_down_su
+00002640: 625a 1864 6f77 6e5f 7375 625f 6861 735f  bZ.down_sub_has_
+00002650: 7361 6d65 5f73 6567 5f69 645a 1064 6f77  same_seg_idZ.dow
+00002660: 6e5f 7375 625f 6973 5f6c 616b 65da 0463  n_sub_is_lake..c
+00002670: 6173 65da 0774 6172 696e 666f da06 6d6f  ase..tarinfo..mo
+00002680: 6469 6679 5a0f 646f 776e 5f73 7562 5f69  difyZ.down_sub_i
+00002690: 6e66 6f5f 325a 0b6e 646f 776e 5f73 7562  nfo_2Z.ndown_sub
+000026a0: 6964 5a0c 7570 6461 7465 5f72 6976 6572  idZ.update_river
+000026b0: 5a14 7461 7267 6574 5f75 7073 7472 6561  Z.target_upstrea
+000026c0: 6d5f 696e 666f 5a12 7570 7374 7265 616d  m_infoZ.upstream
+000026d0: 5f73 7562 6964 5f74 6172 5a0f 636f 6d6d  _subid_tarZ.comm
+000026e0: 6f6e 5f65 6c65 6d65 6e74 735a 1a75 7073  on_elementsZ.ups
+000026f0: 7472 6561 6d5f 7375 6269 645f 6e65 6564  tream_subid_need
+00002700: 5f6d 6f64 6966 7972 4900 0000 5a05 6d61  _modifyrI...Z.ma
+00002710: 736b 3372 4a00 0000 5a08 6d61 736b 7465  sk3rJ...Z.maskte
+00002720: 6d70 7223 0000 00da 0a61 7474 7269 6275  mpr#.....attribu
+00002730: 7465 73da 0363 6f6c 7224 0000 0072 2400  tes..colr$...r$.
+00002740: 0000 7225 0000 00da 1f72 656d 6f76 655f  ..r%.....remove_
+00002750: 706f 7373 6962 6c65 5f73 6d61 6c6c 5f73  possible_small_s
+00002760: 7562 6261 7369 6e73 d601 0000 7382 0100  ubbasins....s...
+00002770: 0000 010c 0204 010a 0104 0314 0110 0106  ................
+00002780: 0104 ff06 0102 ff06 0210 0102 ff06 0210  ................
+00002790: 0102 ff06 0212 0214 010e 010e 010e 0212  ................
+000027a0: 0112 0210 0102 ff06 0210 0102 ff06 040e  ................
+000027b0: 0104 0114 0106 0204 0114 0106 0206 0204  ................
+000027c0: 0104 0104 0104 0318 0308 010c ff06 0102  ................
+000027d0: ff06 0204 0108 010c ff06 0102 ff06 020e  ................
+000027e0: 0104 0108 0216 0308 010c ff06 0102 ff06  ................
+000027f0: 0204 0108 010c ff06 0102 ff06 020e 0108  ................
+00002800: 0210 0308 010c ff06 0102 ff06 0208 010c  ................
+00002810: ff06 0102 ff06 020e 0210 0102 ff06 0204  ................
+00002820: 0108 ff04 0304 010a ff04 030e 0104 0106  ................
+00002830: 020a 0102 ff06 0104 ff06 0214 0106 0204  ................
+00002840: 0106 0304 010a 0102 0102 0102 0102 0102  ................
+00002850: 0102 0102 010a 0102 ff06 f904 0a04 0102  ................
+00002860: 0204 010c 010c 0206 010c ff04 020c 010c  ................
+00002870: 0228 010a 0110 020a 0110 ff06 0204 0108  .(..............
+00002880: ff0e 0204 0110 ff10 0304 0110 ff10 0304  ................
+00002890: 0110 ff10 030c 0110 0104 0108 ff12 0210  ................
+000028a0: 0104 0108 0108 fe14 0410 0104 0108 ff10  ................
+000028b0: 0310 0104 0108 ff10 040a 030c ff06 0102  ................
+000028c0: ff06 030a 0110 0206 ff04 0206 fe04 0306  ................
+000028d0: fd04 0406 fc04 0506 fb04 0606 fa04 0706  ................
+000028e0: f904 0806 f804 0906 f704 0a06 f604 0c06  ................
+000028f0: 021e 0272 9900 0000 7266 0000 0063 0900  ...r....rf...c..
+00002900: 0000 0000 0000 0000 0000 1700 0000 0500  ................
+00002910: 0000 4300 0000 73ea 0300 0064 017d 097c  ..C...s....d.}.|
+00002920: 0164 0164 0267 0219 00a0 0064 03a1 016a  .d.d.g.....d...j
+00002930: 017d 0a7c 0464 046b 0072 5e74 027c 0a7c  .}.|.d.k.r^t.|.|
+00002940: 0083 027d 0b7c 0364 046b 0472 5874 027c  ...}.|.d.k.rXt.|
+00002950: 0a7c 0383 027d 0c74 03a0 047c 0b7c 0ca1  .|...}.t...|.|..
+00002960: 027d 0d7c 0b74 03a0 057c 0da1 0119 007d  .}.|.t...|.....}
+00002970: 0e71 627c 0b7d 0e6e 047c 057d 0e7c 017c  .qb|.}.n.|.}.|.|
+00002980: 017c 0919 00a0 067c 0ea1 0119 00a0 07a1  .|.....|........
+00002990: 007d 0f7c 017c 017c 0919 007c 006b 0219  .}.|.|.|...|.k..
+000029a0: 00a0 07a1 007d 107c 066a 087c 0664 0119  .....}.|.j.|.d..
+000029b0: 00a0 067c 0ea1 0119 00a0 07a1 007d 117c  ...|.........}.|
+000029c0: 116a 087c 1164 0519 0064 046b 0419 00a0  .j.|.d...d.k....
+000029d0: 07a1 007d 117c 106a 0964 0419 007d 1274  ...}.|.j.d...}.t
+000029e0: 0a7c 1183 0164 046b 0490 0172 e474 03a0  .|...d.k...r.t..
+000029f0: 0b7c 1164 0519 006a 01a1 017c 106a 087c  .|.d...j...|.j.|
+00002a00: 1264 0566 023c 0074 036a 0c7c 1164 0619  .d.f.<.t.j.|.d..
+00002a10: 006a 017c 1164 0519 006a 0164 078d 027c  .j.|.d...j.d...|
+00002a20: 106a 087c 1264 0666 023c 0074 036a 0c7c  .j.|.d.f.<.t.j.|
+00002a30: 1164 0819 006a 017c 1164 0519 006a 0164  .d...j.|.d...j.d
+00002a40: 078d 027c 106a 087c 1264 0866 023c 0074  ...|.j.|.d.f.<.t
+00002a50: 036a 0c7c 1164 0919 006a 017c 1164 0519  .j.|.d...j.|.d..
+00002a60: 006a 0164 078d 027c 106a 087c 1264 0966  .j.d...|.j.|.d.f
+00002a70: 023c 0074 036a 0c7c 1164 0a19 006a 017c  .<.t.j.|.d...j.|
+00002a80: 1164 0519 006a 0164 078d 027c 106a 087c  .d...j.d...|.j.|
+00002a90: 1264 0a66 023c 0074 03a0 0d7c 1164 0b19  .d.f.<.t...|.d..
+00002aa0: 006a 01a1 017c 106a 087c 1264 0b66 023c  .j...|.j.|.d.f.<
+00002ab0: 0074 03a0 0d7c 1164 0c19 006a 01a1 017c  .t...|.d...j...|
+00002ac0: 106a 087c 1264 0c66 023c 0074 03a0 0d7c  .j.|.d.f.<.t...|
+00002ad0: 1164 0d19 006a 01a1 017c 106a 087c 1264  .d...j...|.j.|.d
+00002ae0: 0d66 023c 0074 03a0 0e7c 1164 0e19 006a  .f.<.t...|.d...j
+00002af0: 01a1 017c 106a 087c 1264 0e66 023c 0074  ...|.j.|.d.f.<.t
+00002b00: 03a0 0b7c 0f64 0f19 006a 01a1 017c 106a  ...|.d...j...|.j
+00002b10: 087c 1264 0f66 023c 0074 0a7c 0f83 0164  .|.d.f.<.t.|...d
+00002b20: 046b 0490 0272 7874 036a 0c7c 0f64 1019  .k...rxt.j.|.d..
+00002b30: 006a 017c 0f64 0f19 006a 0164 078d 027c  .j.|.d...j.d...|
+00002b40: 106a 087c 1264 1066 023c 0074 036a 0c7c  .j.|.d.f.<.t.j.|
+00002b50: 0f64 1119 006a 017c 0f64 0f19 006a 0164  .d...j.|.d...j.d
+00002b60: 078d 027c 106a 087c 1264 1166 023c 0074  ...|.j.|.d.f.<.t
+00002b70: 036a 0c7c 0f64 1219 006a 017c 0f64 0f19  .j.|.d...j.|.d..
+00002b80: 006a 0164 078d 027c 106a 087c 1264 1266  .j.d...|.j.|.d.f
+00002b90: 023c 007c 0764 136b 0290 0272 8864 137d  .<.|.d.k...r.d.}
+00002ba0: 136e 787c 0764 146b 0290 0272 a264 147c  .nx|.d.k...r.d.|
+00002bb0: 106a 087c 1264 1566 023c 006e 5e7c 0764  .j.|.d.f.<.n^|.d
+00002bc0: 046b 0190 0372 0064 047c 106a 087c 1264  .k...r.d.|.j.|.d
+00002bd0: 1666 023c 0064 047c 106a 087c 1264 1766  .f.<.d.|.j.|.d.f
+00002be0: 023c 0064 047c 106a 087c 1264 1866 023c  .<.d.|.j.|.d.f.<
+00002bf0: 0064 047c 106a 087c 1264 1966 023c 0064  .d.|.j.|.d.f.<.d
+00002c00: 047c 106a 087c 1264 1a66 023c 0064 047c  .|.j.|.d.f.<.d.|
+00002c10: 106a 087c 1264 1566 023c 0064 1b7c 106a  .j.|.d.f.<.d.|.j
+00002c20: 087c 1264 1c66 023c 0064 1b7c 106a 087c  .|.d.f.<.d.|.j.|
+00002c30: 1264 1d66 023c 007c 0864 046b 0490 0372  .d.f.<.|.d.k...r
+00002c40: 347c 087c 106a 087c 1264 1e66 023c 007c  4|.|.j.|.d.f.<.|
+00002c50: 0264 0119 00a0 067c 0ea1 017d 147c 0264  .d.....|...}.|.d
+00002c60: 1f19 007c 006b 027d 1574 03a0 0f7c 147c  ...|.k.}.t...|.|
+00002c70: 15a1 027d 0d7c 106a 1044 005d 847d 167c  ...}.|.j.D.].}.|
+00002c80: 1664 016b 0290 0372 887c 107c 1619 006a  .d.k...r.|.|...j
+00002c90: 0164 0419 007c 026a 087c 0d64 1f66 023c  .d...|.j.|.d.f.<
+00002ca0: 006e 5a7c 1664 1f6b 0290 0373 607c 1664  .nZ|.d.k...s`|.d
+00002cb0: 206b 0290 0373 607c 1664 216b 0290 0373   k...s`|.d!k...s
+00002cc0: 607c 1664 226b 0290 0373 607c 1664 236b  `|.d"k...s`|.d#k
+00002cd0: 0290 0373 607c 1664 246b 0290 0372 ca90  ...s`|.d$k...r..
+00002ce0: 0371 606e 187c 107c 1619 006a 0164 0419  .q`n.|.|...j.d..
+00002cf0: 007c 026a 087c 0d7c 1666 023c 0090 0371  .|.j.|.|.f.<...q
+00002d00: 607c 0253 0029 254e 7206 0000 0072 0d00  `|.S.)%Nr....r..
+00002d10: 0000 7209 0000 0072 0100 0000 7270 0000  ..r....r....rp..
+00002d20: 0072 8200 0000 727e 0000 0072 8300 0000  .r....r~...r....
+00002d30: 7284 0000 0072 8500 0000 da08 426b 6657  r....r......BkfW
+00002d40: 6964 7468 da08 426b 6644 6570 7468 7286  idth..BkfDepthr.
+00002d50: 0000 0072 8700 0000 727a 0000 0072 7d00  ...r....rz...r}.
+00002d60: 0000 7280 0000 0072 8100 0000 7228 0000  ..r....r....r(..
+00002d70: 0072 6200 0000 7261 0000 0072 7c00 0000  .rb...ra...r|...
+00002d80: da07 4c61 6b65 566f 6cda 084c 616b 6541  ..LakeVol..LakeA
+00002d90: 7265 61da 094c 616b 6544 6570 7468 da08  rea..LakeDepth..
+00002da0: 4c61 6b65 7479 7065 e78d 976e 1283 c0f3  Laketype...n....
+00002db0: bfda 0a63 656e 7472 6f69 645f 78da 0a63  ...centroid_x..c
+00002dc0: 656e 7472 6f69 645f 7972 6500 0000 727b  entroid_yre...r{
+00002dd0: 0000 0072 8800 0000 7289 0000 0072 8a00  ...r....r....r..
+00002de0: 0000 7257 0000 0072 8b00 0000 2911 7216  ..rW...r....).r.
+00002df0: 0000 0072 1300 0000 7217 0000 0072 1a00  ...r....r....r..
+00002e00: 0000 722e 0000 00da 0b6c 6f67 6963 616c  ..r......logical
+00002e10: 5f6e 6f74 7212 0000 0072 1400 0000 7219  _notr....r....r.
+00002e20: 0000 0072 5800 0000 7215 0000 0072 3e00  ...rX...r....r>.
+00002e30: 0000 728e 0000 0072 6700 0000 728f 0000  ..r....rg...r...
+00002e40: 0072 8c00 0000 7211 0000 0029 1772 4800  .r....r....).rH.
+00002e50: 0000 da0d 6361 7463 686d 656e 7469 6e66  ....catchmentinf
+00002e60: 6f72 9000 0000 5a07 7570 7375 6269 64da  or....Z.upsubid.
+00002e70: 0a69 736d 6f64 6966 6964 73da 0a6d 6f64  .ismodifids..mod
+00002e80: 6966 6969 6469 6eda 076d 6169 6e72 6976  ifiidin..mainriv
+00002e90: 7261 0000 00da 0973 6567 5f6f 7264 6572  ra.....seg_order
+00002ea0: da09 7375 625f 636f 6c6e 6d72 6a00 0000  ..sub_colnmrj...
+00002eb0: 5a0e 4d6f 6469 6679 5f73 7562 6964 7331  Z.Modify_subids1
+00002ec0: 5a0e 4d6f 6469 6679 5f73 7562 6964 7332  Z.Modify_subids2
+00002ed0: 7223 0000 005a 0d4d 6f64 6966 795f 7375  r#...Z.Modify_su
+00002ee0: 6269 6473 5a07 6362 7261 6e63 6872 9500  bidsZ.cbranchr..
+00002ef0: 0000 7272 0000 0072 5c00 0000 5a0a 646f  ..rr...r\...Z.do
+00002f00: 5f6e 6f74 6869 6e67 7249 0000 0072 4a00  _nothingrI...rJ.
+00002f10: 0000 7298 0000 0072 2400 0000 7224 0000  ..r....r$...r$..
+00002f20: 0072 2500 0000 da15 4e65 775f 5375 6249  .r%.....New_SubI
+00002f30: 645f 546f 5f44 6973 736f 6c76 6591 0200  d_To_Dissolve...
+00002f40: 0073 d400 0000 000b 0401 1401 0801 0201  .s..............
+00002f50: 04ff 0403 0801 0a01 0c01 1002 0603 0404  ................
+00002f60: 0a01 02ff 0a02 0201 0aff 0804 0c01 02ff  ................
+00002f70: 0a02 1602 0a02 0e01 0401 08ff 0e02 0401  ................
+00002f80: 0801 08fe 1004 0401 0801 08fe 1004 0401  ................
+00002f90: 0801 08fe 1004 0401 0801 08fe 1004 0401  ................
+00002fa0: 08ff 0e02 0401 08ff 0e03 0401 08ff 0e02  ................
+00002fb0: 0401 08ff 0e03 1a02 0e01 0401 10ff 1003  ................
+00002fc0: 0401 10ff 1003 0401 10ff 1005 06ff 040d  ................
+00002fd0: 0602 0a0a 1001 0a05 0e01 0e01 0e01 0e01  ................
+00002fe0: 0e01 0e02 0e01 0e02 0a01 0e02 0801 02ff  ................
+00002ff0: 0404 0aff 0203 0c03 0a01 0a02 1a03 06ff  ................
+00003000: 0402 06fe 0403 06fd 0404 06fc 0405 06fb  ................
+00003010: 0406 06fa 0408 0602 1c03 72aa 0000 0072  ..........r....r
+00003020: 0600 0000 6303 0000 0000 0000 0000 0000  ....c...........
+00003030: 0008 0000 0004 0000 0043 0000 0073 a400  .........C...s..
+00003040: 0000 7c00 6a00 7c01 6a00 6b03 a001 a100  ..|.j.|.j.k.....
+00003050: 7228 7402 7c00 6a00 8301 0100 7402 7c01  r(t.|.j.....t.|.
+00003060: 6a00 8301 0100 6401 5300 6402 7d03 7c00  j.....d.S.d.}.|.
+00003070: 6a00 4400 5d62 7d04 7c04 6403 6b02 7248  j.D.]b}.|.d.k.rH
+00003080: 7c03 6404 1700 7d03 7132 7c00 7c04 1900  |.d...}.q2|.|...
+00003090: 6a03 7d05 7c01 7c04 1900 6a03 7d06 7c05  j.}.|.|...j.}.|.
+000030a0: 7c06 6b03 a001 a100 728c 7402 7c04 8301  |.k.....r.t.|...
+000030b0: 0100 7c05 7c06 6b03 7d07 7402 7c00 7c02  ..|.|.k.}.t.|.|.
+000030c0: 1900 6a03 7c07 1900 8301 0100 7132 7c03  ..j.|.......q2|.
+000030d0: 6404 1700 7d03 7132 7c03 7404 7c00 6a00  d...}.q2|.t.|.j.
+000030e0: 8301 6b02 5300 2905 4e46 7201 0000 00da  ..k.S.).NFr.....
+000030f0: 0648 5255 5f49 4472 2800 0000 2905 7211  .HRU_IDr(...).r.
+00003100: 0000 00da 0361 6c6c 7268 0000 0072 1300  .....allrh...r..
+00003110: 0000 7215 0000 0029 08da 0845 7870 6563  ..r....)...Expec
+00003120: 7465 64da 0652 6573 756c 745a 0c43 6865  ted..ResultZ.Che
+00003130: 636b 5f43 6f6c 5f4e 4d5a 046e 6571 6c72  ck_Col_NMZ.neqlr
+00003140: 9800 0000 5a0c 4172 7261 795f 6578 7065  ....Z.Array_expe
+00003150: 6374 5a0c 4172 7261 795f 7265 7375 6c74  ctZ.Array_result
+00003160: 7223 0000 0072 2400 0000 7224 0000 0072  r#...r$...r$...r
+00003170: 2500 0000 da17 4576 616c 7561 7465 5f54  %.....Evaluate_T
+00003180: 776f 5f44 6174 6166 7261 6d65 732e 0300  wo_Dataframes...
+00003190: 0073 2200 0000 0002 1001 0a01 0a01 0401  .s".............
+000031a0: 0402 0a01 0801 0801 0201 0a01 0a01 0c01  ................
+000031b0: 0801 0801 1402 0a02 72af 0000 0072 2800  ........r....r(.
+000031c0: 0000 6303 0000 0000 0000 0000 0000 000b  ..c.............
+000031d0: 0000 0005 0000 0043 0000 0073 ac01 0000  .......C...s....
+000031e0: 7c00 6a00 7d03 7c02 6401 6b04 72e2 7401  |.j.}.|.d.k.r.t.
+000031f0: 6401 7402 7c03 8301 8302 4400 5d8c 7d04  d.t.|.....D.].}.
+00003200: 7c00 6a03 7c03 7c04 1900 6402 6602 1900  |.j.|.|...d.f...
+00003210: 7d05 7c00 6a03 7c03 7c04 1900 6403 6602  }.|.j.|.|...d.f.
+00003220: 1900 7d06 7c00 6a03 7c03 7c04 1900 6404  ..}.|.j.|.|...d.
+00003230: 6602 1900 7d07 7c00 6a03 7c00 6403 1900  f...}.|.j.|.d...
+00003240: 7c07 6b02 1900 a004 a100 7d08 7402 7c08  |.k.......}.t.|.
+00003250: 8301 6401 6b04 7296 7c08 6402 1900 6a05  ..d.k.r.|.d...j.
+00003260: 6401 1900 7c00 6a03 7c03 7c04 1900 6405  d...|.j.|.|...d.
+00003270: 6602 3c00 711c 6406 7c00 6a03 7c03 7c04  f.<.q.d.|.j.|.|.
+00003280: 1900 6405 6602 3c00 711c 7c00 6403 1900  ..d.f.<.q.|.d...
+00003290: 6a05 7c00 6407 3c00 7c00 6404 1900 6a05  j.|.d.<.|.d...j.
+000032a0: 7c00 6408 3c00 7c00 6402 1900 6a05 7c00  |.d.<.|.d...j.|.
+000032b0: 6403 3c00 7c00 6405 1900 6a05 7c00 6404  d.<.|.d...j.|.d.
+000032c0: 3c00 7c01 6401 6b00 72ee 7c00 5300 7c00  <.|.d.k.r.|.S.|.
+000032d0: 6a06 6403 6409 640a 8d02 7d09 7407 7c09  j.d.d.d...}.t.|.
+000032e0: 8301 7d09 7401 6401 7402 7c09 8301 8302  ..}.t.d.t.|.....
+000032f0: 4400 5d94 7d04 7c09 6403 1900 6a05 7c04  D.].}.|.d...j.|.
+00003300: 1900 7d0a 7c09 640b 1900 6a05 7c04 1900  ..}.|.d...j.|...
+00003310: 7c00 6a03 7c00 6403 1900 7c0a 6b02 640b  |.j.|.d...|.k.d.
+00003320: 6602 3c00 7c09 640c 1900 6a05 7c04 1900  f.<.|.d...j.|...
+00003330: 7c00 6a03 7c00 6403 1900 7c0a 6b02 640c  |.j.|.d...|.k.d.
+00003340: 6602 3c00 7c09 640d 1900 6a05 7c04 1900  f.<.|.d...j.|...
+00003350: 7c00 6a03 7c00 6403 1900 7c0a 6b02 640d  |.j.|.d...|.k.d.
+00003360: 6602 3c00 7c09 640e 1900 6a05 7c04 1900  f.<.|.d...j.|...
+00003370: 7c00 6a03 7c00 6403 1900 7c0a 6b02 640e  |.j.|.d...|.k.d.
+00003380: 6602 3c00 9001 7112 7c00 5300 290f fadf  f.<...q.|.S.)...
+00003390: 4675 6e63 7469 6f6e 7320 7769 6c6c 2075  Functions will u
+000033a0: 7064 6174 6520 7375 6269 642c 646f 776e  pdate subid,down
+000033b0: 7375 6269 642c 2063 616c 6375 6174 6520  subid, calcuate 
+000033c0: 7374 7265 616d 206f 7264 6572 2061 6e64  stream order and
+000033d0: 0a20 2020 2020 2020 2075 7064 6174 6520  .        update 
+000033e0: 6472 6169 6e61 6765 2061 7265 6120 696e  drainage area in
+000033f0: 2074 6865 2061 7474 7269 6275 7465 2074   the attribute t
+00003400: 6162 6c65 206d 6170 6f6c 646e 6577 5f69  able mapoldnew_i
+00003410: 6e66 6f0a 2020 2020 2d2d 2d2d 2d2d 2d2d  nfo.    --------
+00003420: 2d2d 0a0a 2020 2020 4e6f 7465 730a 2020  --..    Notes.  
+00003430: 2020 2d2d 2d2d 2d2d 2d0a 0a20 2020 2052    -------..    R
+00003440: 6574 7572 6e73 3a0a 2020 2020 2d2d 2d2d  eturns:.    ----
+00003450: 2d2d 2d0a 2020 2020 2020 2020 6d61 706f  ---.        mapo
+00003460: 6c64 6e65 775f 696e 666f 0a20 2020 2072  ldnew_info.    r
+00003470: 0100 0000 727b 0000 0072 0600 0000 720d  ....r{...r....r.
+00003480: 0000 0072 8800 0000 7266 0000 0072 8900  ...r....rf...r..
+00003490: 0000 728a 0000 0072 3900 0000 a901 723b  ..r....r9.....r;
+000034a0: 0000 0072 6400 0000 7263 0000 0072 6500  ...rd...rc...re.
+000034b0: 0000 726c 0000 0029 0872 5800 0000 7229  ..rl...).rX...r)
+000034c0: 0000 0072 1500 0000 7219 0000 0072 1400  ...r....r....r..
+000034d0: 0000 7213 0000 0072 4100 0000 da1a 7374  ..r....rA.....st
+000034e0: 7265 616d 6f72 6465 7261 6e64 6472 6169  reamorderanddrai
+000034f0: 6e61 6765 6172 6561 290b 7290 0000 00da  nagearea).r.....
+00003500: 1155 7064 6174 6553 7472 6561 6d6f 7264  .UpdateStreamord
+00003510: 6572 da0b 5570 6461 7465 5375 6249 6472  er..UpdateSubIdr
+00003520: 5c00 0000 7247 0000 0072 7b00 0000 7248  \...rG...r{...rH
+00003530: 0000 00da 0a6f 646f 776e 7375 6269 64da  .....odownsubid.
+00003540: 0c64 6f6e 7375 6269 6469 6e66 6fda 156d  .donsubidinfo..m
+00003550: 6170 6f6c 646e 6577 5f69 6e66 6f5f 756e  apoldnew_info_un
+00003560: 6971 7565 da06 6973 7562 6964 7224 0000  ique..isubidr$..
+00003570: 0072 2400 0000 7225 0000 00da 0e55 7064  .r$...r%.....Upd
+00003580: 6174 6554 6f70 6f6c 6f67 7946 0300 0073  ateTopologyF...s
+00003590: 5a00 0000 000d 0602 0801 1201 1201 1201  Z...............
+000035a0: 1202 0401 0aff 0804 0c01 0201 02ff 0402  ................
+000035b0: 02fe 1404 1402 0e01 0e01 0e02 0e02 0801  ................
+000035c0: 0402 0401 04ff 0603 0802 1201 0e03 0cfe  ................
+000035d0: 0401 0eff 0205 0cfe 0401 0eff 0205 0cfe  ................
+000035e0: 0401 0eff 0205 0cfe 0401 0eff 0604 72b9  ..............r.
+000035f0: 0000 0063 0300 0000 0000 0000 0000 0000  ...c............
+00003600: 0800 0000 0500 0000 4300 0000 738a 0000  ........C...s...
+00003610: 0064 017c 0064 021b 0064 021b 0064 0313  .d.|.d...d...d..
+00003620: 0014 007d 0364 047c 0164 021b 0014 007c  ...}.d.|.d.....|
+00003630: 0064 021b 0064 021b 0064 0513 0014 007c  .d...d...d.....|
+00003640: 0264 0613 0014 007d 0464 077c 0164 021b  .d.....}.d.|.d..
+00003650: 0064 0813 0014 007c 0264 0913 0014 007d  .d.....|.d.....}
+00003660: 0564 0a7c 0164 021b 007c 0264 0313 001b  .d.|.d...|.d....
+00003670: 0064 0b13 0014 007d 0664 0c7c 017c 0264  .d.....}.d.|.|.d
+00003680: 0313 001b 0064 0d13 0014 007d 077c 037c  .....d.....}.|.|
+00003690: 047c 057c 067c 0766 0553 0029 0e4e 679a  .|.|.|.f.S.).Ng.
+000036a0: 9999 9999 99e5 3f72 6f00 0000 e700 0000  ......?ro.......
+000036b0: 0000 00e0 3f67 933a 014d 840d cf3f 679a  ....?g.:.M...?g.
+000036c0: 9999 9999 99b9 bf67 9a99 9999 9999 c9bf  .......g........
+000036d0: 6733 3333 3333 33d3 3f67 52b8 1e85 eb51  g333333.?gR....Q
+000036e0: e83f 6752 b81e 85eb 51c8 bf67 abaa aaaa  .?gR....Q..g....
+000036f0: aaaa 1240 6714 ae47 e17a 14de 3f67 c20f  ...@g..G.z..?g..
+00003700: e172 cfcd 413f 6748 e17a 14ae 47e9 3f72  .r..A?gH.z..G.?r
+00003710: 2400 0000 2908 726c 0000 00da 0844 415f  $...).rl.....DA_
+00003720: 4368 6e5f 4cda 0a44 415f 4368 6e5f 536c  Chn_L..DA_Chn_Sl
+00003730: 705a 0454 435f 315a 0454 435f 325a 0454  pZ.TC_1Z.TC_2Z.T
+00003740: 435f 335a 0454 435f 345a 0454 435f 3572  C_3Z.TC_4Z.TC_5r
+00003750: 2400 0000 7224 0000 0072 2500 0000 da0c  $...r$...r%.....
+00003760: 6361 6c63 756c 6174 655f 5463 8603 0000  calculate_Tc....
+00003770: 7314 0000 0000 0214 0114 0102 ff04 0106  s...............
+00003780: ff04 0218 0118 0114 0172 bd00 0000 6301  .........r....c.
+00003790: 0000 0000 0000 0000 0000 0018 0000 0007  ................
+000037a0: 0000 0043 0000 0073 c408 0000 6401 7d01  ...C...s....d.}.
+000037b0: 6401 7c00 6a00 7601 7212 6402 7d01 7c00  d.|.j.v.r.d.}.|.
+000037c0: 6a01 7c00 6403 1900 6404 6b03 1900 a002  j.|.d...d.k.....
+000037d0: a100 7d02 7c00 6a01 7c00 6403 1900 6404  ..}.|.j.|.d...d.
+000037e0: 6b02 1900 a002 a100 7d03 7c03 6405 6406  k.......}.|.d.d.
+000037f0: 6702 1900 a003 6407 a101 6a04 7d04 7405  g.....d...j.}.t.
+00003800: a006 7407 7c02 8301 6408 a102 7d05 6409  ..t.|...d...}.d.
+00003810: 7d06 640a 7d07 7408 6409 7407 7c02 8301  }.d.}.t.d.t.|...
+00003820: 8302 4400 9001 5d80 7d08 7c02 6a09 7c08  ..D...].}.|.j.|.
+00003830: 1900 7d09 7c02 6405 1900 6a04 7c08 1900  ..}.|.d...j.|...
+00003840: 7c02 6406 1900 6a04 7c08 1900 6b02 72b2  |.d...j.|...k.r.
+00003850: 640b 7c02 6a01 7c09 6406 6602 3c00 7c02  d.|.j.|.d.f.<.|.
+00003860: 6405 1900 6a04 7c08 1900 7d0a 7407 7c02  d...j.|...}.t.|.
+00003870: 7c02 6406 1900 7c0a 6b02 1900 8301 6409  |.d...|.k.....d.
+00003880: 6b02 7278 740a 7c02 6406 1900 6a04 7c08  k.rxt.|.d...j.|.
+00003890: 1900 8301 7c05 7c06 3c00 7407 7c04 8301  ....|.|.<.t.|...
+000038a0: 6409 6b02 9001 7206 640c 7d0b 640c 7d0c  d.k...r.d.}.d.}.
+000038b0: 6e62 740b 7c04 7c0a 8302 7d0d 7c03 6a01  nbt.|.|...}.|.j.
+000038c0: 7c03 6405 1900 a00c 7c0d a101 1900 a002  |.d.....|.......
+000038d0: a100 7d0e 7407 7c0e 8301 6409 6b04 9001  ..}.t.|...d.k...
+000038e0: 7260 740d 7c0e 640d 1900 6a04 8301 7d0b  r`t.|.d...j...}.
+000038f0: 7405 6a0e 7c0e 640e 1900 6a04 7c0e 640d  t.j.|.d...j.|.d.
+00003900: 1900 6a04 640f 8d02 7d0c 6e08 640c 7d0b  ..j.d...}.n.d.}.
+00003910: 640c 7d0c 7c0b 7c02 640d 1900 6a04 7c08  d.}.|.|.d...j.|.
+00003920: 1900 1700 7c02 6a01 7c09 6410 6602 3c00  ....|.j.|.d.f.<.
+00003930: 640a 7c02 6a01 7c09 6411 6602 3c00 640a  d.|.j.|.d.f.<.d.
+00003940: 7c02 6a01 7c09 6412 6602 3c00 7c07 7c02  |.j.|.d.f.<.|.|.
+00003950: 6a01 7c09 6413 6602 3c00 7c02 640e 1900  j.|.d.f.<.|.d...
+00003960: 6a04 7c08 1900 7c02 640d 1900 6a04 7c08  j.|...|.d...j.|.
+00003970: 1900 1400 7c0b 7c0c 1400 1700 7c02 6a01  ....|.|.....|.j.
+00003980: 7c09 6410 6602 1900 1b00 7c02 6a01 7c09  |.d.f.....|.j.|.
+00003990: 6414 6602 3c00 7c06 640a 1700 7d06 7c07  d.f.<.|.d...}.|.
+000039a0: 640a 1700 7d07 7178 7405 a00f 7c05 a101  d...}.qxt...|...
+000039b0: 7d05 7c05 7c05 6409 6b04 1900 7d05 7405  }.|.|.d.k...}.t.
+000039c0: a006 7407 7c02 8301 6408 a102 7d0f 6409  ..t.|...d...}.d.
+000039d0: 7d10 7408 6409 7407 7c05 8301 8302 4400  }.t.d.t.|.....D.
+000039e0: 9004 5da2 7d08 7c05 7c08 1900 7d0a 640a  ..].}.|.|...}.d.
+000039f0: 7d11 7c11 640a 6b02 9002 7234 7c0a 6409  }.|.d.k...r4|.d.
+00003a00: 6b04 9002 7234 7c02 6a01 7c02 6406 1900  k...r4|.j.|.d...
+00003a10: 7c0a 6b02 1900 a002 a100 7d12 7c02 6a01  |.k.......}.|.j.
+00003a20: 7c02 6405 1900 7c0a 6b02 1900 a002 a100  |.d...|.k.......
+00003a30: 7d13 7c02 6405 1900 7c0a 6b02 7d14 7407  }.|.d...|.k.}.t.
+00003a40: 7c04 8301 6409 6b02 9002 72aa 640c 7d0b  |...d.k...r.d.}.
+00003a50: 640c 7d0c 6e62 740b 7c04 7c0a 8302 7d0d  d.}.nbt.|.|...}.
+00003a60: 7c03 6a01 7c03 6405 1900 a00c 7c0d a101  |.j.|.d.....|...
+00003a70: 1900 a002 a100 7d0e 7407 7c0e 8301 6409  ......}.t.|...d.
+00003a80: 6b04 9003 7204 740d 7c0e 640d 1900 6a04  k...r.t.|.d...j.
+00003a90: 8301 7d0b 7405 6a0e 7c0e 640e 1900 6a04  ..}.t.j.|.d...j.
+00003aa0: 7c0e 640d 1900 6a04 640f 8d02 7d0c 6e08  |.d...j.d...}.n.
+00003ab0: 640c 7d0b 640c 7d0c 7407 7c13 8301 6409  d.}.d.}.t.|...d.
+00003ac0: 6b01 9003 721e 9002 7134 7407 7c12 8301  k...r...q4t.|...
+00003ad0: 640a 6b02 9004 72aa 7c13 640d 1900 6a04  d.k...r.|.d...j.
+00003ae0: 6409 1900 7c12 6410 1900 6a04 6409 1900  d...|.d...j.d...
+00003af0: 1700 7c0b 1700 7c02 6a01 7c14 6410 6602  ..|...|.j.|.d.f.
+00003b00: 3c00 7c12 6411 1900 6a04 6409 1900 7c02  <.|.d...j.d...|.
+00003b10: 6a01 7c14 6411 6602 3c00 7c12 6412 1900  j.|.d.f.<.|.d...
+00003b20: 6a04 6409 1900 640a 1700 7c02 6a01 7c14  j.d...d...|.j.|.
+00003b30: 6412 6602 3c00 7c12 6413 1900 6a04 6409  d.f.<.|.d...j.d.
+00003b40: 1900 7c02 6a01 7c14 6413 6602 3c00 6415  ..|.j.|.d.f.<.d.
+00003b50: 7c02 6a00 7600 9004 7294 7405 a010 7c12  |.j.v...r.t...|.
+00003b60: 6415 1900 6a04 6409 1900 6409 a102 7c13  d...j.d...d...|.
+00003b70: 6416 1900 6a04 6409 1900 1700 7c02 6a01  d...j.d.....|.j.
+00003b80: 7c14 6415 6602 3c00 7c13 6417 1900 6a04  |.d.f.<.|.d...j.
+00003b90: 6409 1900 7405 a010 7c13 6416 1900 6a04  d...t...|.d...j.
+00003ba0: 6409 1900 6409 a102 1400 7c12 6415 1900  d...d.....|.d...
+00003bb0: 6a04 6409 1900 7405 a010 7c12 6418 1900  j.d...t...|.d...
+00003bc0: 6a04 6409 1900 6409 a102 1400 1700 7c02  j.d...d.......|.
+00003bd0: 6a01 7c14 6415 6602 1900 1b00 7c02 6a01  j.|.d.f.....|.j.
+00003be0: 7c14 6418 6602 3c00 7c13 640e 1900 6a04  |.d.f.<.|.d...j.
+00003bf0: 6409 1900 7c13 640d 1900 6a04 6409 1900  d...|.d...j.d...
+00003c00: 1400 7c0b 7c0c 1400 1700 7c12 6414 1900  ..|.|.....|.d...
+00003c10: 6a04 6409 1900 7c12 6410 1900 6a04 6409  j.d...|.d...j.d.
+00003c20: 1900 1400 1700 7c02 6a01 7c14 6410 6602  ......|.j.|.d.f.
+00003c30: 1900 1b00 7c02 6a01 7c14 6414 6602 3c00  ....|.j.|.d.f.<.
+00003c40: 740a 7c13 6406 1900 6a04 6409 1900 8301  t.|.d...j.d.....
+00003c50: 7d0a 9002 7146 7405 a011 7c12 6411 1900  }...qFt...|.d...
+00003c60: 6a04 a101 6409 6b04 9006 72ba 6415 7c12  j...d.k...r.d.|.
+00003c70: 6a00 7600 9004 72da 7c12 6a12 6415 6419  j.v...r.|.j.d.d.
+00003c80: 641a 8d02 7d12 7c13 640d 1900 6a04 6409  d...}.|.d...j.d.
+00003c90: 1900 7405 a00d 7c12 6410 1900 6a04 a101  ..t...|.d...j...
+00003ca0: 1700 7c0b 1700 7c02 6a01 7c14 6410 6602  ..|...|.j.|.d.f.
+00003cb0: 3c00 6415 7c02 6a00 7600 9005 72f8 7405  <.d.|.j.v...r.t.
+00003cc0: a010 7c12 6415 1900 6a04 6409 1900 6409  ..|.d...j.d...d.
+00003cd0: a102 7c13 6416 1900 6a04 6409 1900 1700  ..|.d...j.d.....
+00003ce0: 7c02 6a01 7c14 6415 6602 3c00 7c13 6417  |.j.|.d.f.<.|.d.
+00003cf0: 1900 6a04 6409 1900 7405 a010 7c13 6416  ..j.d...t...|.d.
+00003d00: 1900 6a04 6409 1900 6409 a102 1400 7c12  ..j.d...d.....|.
+00003d10: 6415 1900 6a04 6409 1900 7405 a010 7c12  d...j.d...t...|.
+00003d20: 6418 1900 6a04 6409 1900 6409 a102 1400  d...j.d...d.....
+00003d30: 1700 7c02 6a01 7c14 6415 6602 1900 1b00  ..|.j.|.d.f.....
+00003d40: 7c02 6a01 7c14 6418 6602 3c00 7c13 640e  |.j.|.d.f.<.|.d.
+00003d50: 1900 6a04 6409 1900 7c13 640d 1900 6a04  ..j.d...|.d...j.
+00003d60: 6409 1900 1400 7c0b 7c0c 1400 1700 7c12  d.....|.|.....|.
+00003d70: 6414 1900 6a04 6409 1900 7c12 6410 1900  d...j.d...|.d...
+00003d80: 6a04 6409 1900 1400 1700 7c02 6a01 7c14  j.d.......|.j.|.
+00003d90: 6410 6602 1900 1b00 7c02 6a01 7c14 6414  d.f.....|.j.|.d.
+00003da0: 6602 3c00 7405 a011 7c12 6411 1900 6a04  f.<.t...|.d...j.
+00003db0: a101 7405 a013 7c12 6411 1900 6a04 a101  ..t...|.d...j...
+00003dc0: 6b02 9006 7260 7c12 6411 1900 6a04 6409  k...r`|.d...j.d.
+00003dd0: 1900 640a 1700 7c02 6a01 7c14 6411 6602  ..d...|.j.|.d.f.
+00003de0: 3c00 640a 7c02 6a01 7c14 6412 6602 3c00  <.d.|.j.|.d.f.<.
+00003df0: 7c07 640a 1700 7c02 6a01 7c14 6413 6602  |.d...|.j.|.d.f.
+00003e00: 3c00 7c07 640a 1700 7d07 6e46 7405 a013  <.|.d...}.nFt...
+00003e10: 7c12 6411 1900 6a04 a101 7d15 7c15 7c02  |.d...j...}.|.|.
+00003e20: 6a01 7c14 6411 6602 3c00 640a 7c02 6a01  j.|.d.f.<.d.|.j.
+00003e30: 7c14 6412 6602 3c00 7c07 640a 1700 7c02  |.d.f.<.|.d...|.
+00003e40: 6a01 7c14 6413 6602 3c00 7c07 640a 1700  j.|.d.f.<.|.d...
+00003e50: 7d07 740a 7c13 6406 1900 6a04 6409 1900  }.t.|.d...j.d...
+00003e60: 8301 7d0a 6e18 740a 7c0a 8301 7c0f 7c10  ..}.n.t.|...|.|.
+00003e70: 3c00 7c10 640a 1700 7d10 6409 7d11 9002  <.|.d...}.d.}...
+00003e80: 7146 9002 7134 7c00 6405 1900 a00c 7c02  qF..q4|.d.....|.
+00003e90: 6405 1900 6a04 a101 7d16 7c02 6413 1900  d...j...}.|.d...
+00003ea0: 6a04 7c00 6a01 7c16 6413 6602 3c00 7c02  j.|.j.|.d.f.<.|.
+00003eb0: 6412 1900 6a04 7c00 6a01 7c16 6412 6602  d...j.|.j.|.d.f.
+00003ec0: 3c00 7c02 6411 1900 6a04 7c00 6a01 7c16  <.|.d...j.|.j.|.
+00003ed0: 6411 6602 3c00 7c02 6413 1900 6a04 7c00  d.f.<.|.d...j.|.
+00003ee0: 6a01 7c16 6413 6602 3c00 7c02 6410 1900  j.|.d.f.<.|.d...
+00003ef0: 6a04 7c00 6a01 7c16 6410 6602 3c00 6415  j.|.j.|.d.f.<.d.
+00003f00: 7c00 6a00 7600 9007 729a 7c02 6415 1900  |.j.v...r.|.d...
+00003f10: 6a04 7c00 6a01 7c16 6415 6602 3c00 7c02  j.|.j.|.d.f.<.|.
+00003f20: 6414 1900 6a04 7c00 6a01 7c16 6414 6602  d...j.|.j.|.d.f.
+00003f30: 3c00 7c02 6418 1900 6a04 7c00 6a01 7c16  <.|.d...j.|.j.|.
+00003f40: 6418 6602 3c00 7c02 6416 1900 6a04 7c00  d.f.<.|.d...j.|.
+00003f50: 6a01 7c16 6416 6602 3c00 7c02 6417 1900  j.|.d.f.<.|.d...
+00003f60: 6a04 7c00 6a01 7c16 6417 6602 3c00 7408  j.|.j.|.d.f.<.t.
+00003f70: 6409 7407 7c00 8301 8302 4400 5dee 7d08  d.t.|.....D.].}.
+00003f80: 7c00 6a09 7c08 1900 7d09 7c00 7c01 1900  |.j.|...}.|.|...
+00003f90: 6a04 7c08 1900 6409 6b04 9008 7234 7c00  j.|...d.k...r4|.
+00003fa0: 641b 1900 6a04 7c08 1900 6409 6b04 9008  d...j.|...d.k...
+00003fb0: 7234 7c00 6410 1900 6a04 7c08 1900 641c  r4|.d...j.|...d.
+00003fc0: 1b00 641c 1b00 7c00 641b 1900 6a04 7c08  ..d...|.d...j.|.
+00003fd0: 1900 1b00 7c00 6a01 7c09 641d 6602 3c00  ....|.j.|.d.f.<.
+00003fe0: 7c00 6403 1900 6a04 7c08 1900 6404 6b02  |.d...j.|...d.k.
+00003ff0: 9007 72d0 7c00 6405 1900 6a04 7c08 1900  ..r.|.d...j.|...
+00004000: 7d0a 740b 7c04 7c0a 8302 7d0d 7c03 6a01  }.t.|.|...}.|.j.
+00004010: 7c03 6405 1900 a00c 7c0d a101 1900 6a02  |.d.....|.....j.
+00004020: 641e 641f 8d01 7d0e 740d 7c0e 640d 1900  d.d...}.t.|.d...
+00004030: 6a04 8301 7d17 7c17 7c00 6a01 7c09 6410  j...}.|.|.j.|.d.
+00004040: 6602 3c00 7405 6a0e 7c0e 640e 1900 6a04  f.<.t.j.|.d...j.
+00004050: 7c0e 640d 1900 6a04 640f 8d02 7c00 6a01  |.d...j.d...|.j.
+00004060: 7c09 6414 6602 3c00 9007 71d0 7c00 5300  |.d.f.<...q.|.S.
+00004070: 2920 7ac0 4675 6e63 7469 6f6e 7320 7769  ) z.Functions wi
+00004080: 6c6c 2020 6361 6c63 7561 7465 2073 7472  ll  calcuate str
+00004090: 6561 6d20 6f72 6465 7220 616e 640a 2020  eam order and.  
+000040a0: 2020 2020 2020 7570 6461 7465 2064 7261        update dra
+000040b0: 696e 6167 6520 6172 6561 2069 6e20 7468  inage area in th
+000040c0: 6520 6174 7472 6962 7574 6520 7461 626c  e attribute tabl
+000040d0: 6520 6361 7469 6e66 6f61 6c6c 0a20 2020  e catinfoall.   
+000040e0: 202d 2d2d 2d2d 2d2d 2d2d 2d0a 0a20 2020   ----------..   
+000040f0: 204e 6f74 6573 0a20 2020 202d 2d2d 2d2d   Notes.    -----
+00004100: 2d2d 0a0a 2020 2020 5265 7475 726e 733a  --..    Returns:
+00004110: 0a20 2020 202d 2d2d 2d2d 2d2d 0a20 2020  .    -------.   
+00004120: 2020 2020 2063 6174 696e 666f 616c 6c0a       catinfoall.
+00004130: 2020 2020 7278 0000 0072 7900 0000 7261      rx...ry...ra
+00004140: 0000 0072 6200 0000 7206 0000 0072 0d00  ...rb...r....r..
+00004150: 0000 7260 0000 0069 f7ff ffff 7201 0000  ..r`...i....r...
+00004160: 0072 2800 0000 7266 0000 00e7 0000 0000  .r(...rf........
+00004170: 0000 0000 727a 0000 0072 7d00 0000 727e  ....rz...r}...r~
+00004180: 0000 0072 6c00 0000 7264 0000 0072 6500  ...rl...rd...re.
+00004190: 0000 7263 0000 005a 0844 415f 536c 6f70  ..rc...Z.DA_Slop
+000041a0: 6572 bb00 0000 7270 0000 0072 8200 0000  er....rp...r....
+000041b0: 72bc 0000 0046 7236 0000 00da 0644 415f  r....Fr6.....DA_
+000041c0: 4f62 73e7 0000 0000 0040 8f40 da08 4441  Obs......@.@..DA
+000041d0: 5f65 7272 6f72 5472 0700 0000 2914 7211  _errorTr....).r.
+000041e0: 0000 0072 1900 0000 7214 0000 0072 1600  ...r....r....r..
+000041f0: 0000 7213 0000 0072 1a00 0000 7271 0000  ..r....r....rq..
+00004200: 0072 1500 0000 7229 0000 0072 5800 0000  .r....r)...rX...
+00004210: 722d 0000 0072 1700 0000 7212 0000 0072  r-...r....r....r
+00004220: 3e00 0000 728e 0000 0072 2b00 0000 da07  >...r....r+.....
+00004230: 6d61 7869 6d75 6d72 8f00 0000 7240 0000  maximumr....r@..
+00004240: 0072 6700 0000 2918 5a0a 6361 7469 6e66  .rg...).Z.catinf
+00004250: 6f61 6c6c 7293 0000 0072 6900 0000 5a0b  oallr....ri...Z.
+00004260: 6361 7469 6e66 6f5f 6e63 6c5a 0b72 6f75  catinfo_nclZ.rou
+00004270: 7469 6e67 5f6e 636c 5a07 6361 746c 6973  ting_nclZ.catlis
+00004280: 745a 0469 6361 74da 0469 7365 6772 4700  tZ.icat..isegrG.
+00004290: 0000 725c 0000 00da 0563 6174 6964 5a06  ..r\.....catidZ.
+000042a0: 4441 5f6e 636c 5a07 736c 705f 6e63 6c5a  DA_nclZ.slp_nclZ
+000042b0: 0c55 7073 7472 6561 6d63 6174 735a 0b55  .UpstreamcatsZ.U
+000042c0: 705f 6361 745f 696e 666f 5a0a 6e65 7763  p_cat_infoZ.newc
+000042d0: 6174 6c69 7374 5a09 696e 6577 7374 6172  atlistZ.inewstar
+000042e0: 745a 0b46 5f69 6e74 6572 7365 6374 5a0f  tZ.F_intersectZ.
+000042f0: 5570 5f52 6561 6368 6573 5f69 6e66 6f5a  Up_Reaches_infoZ
+00004300: 0e63 7572 5f52 6561 6368 5f69 6e66 6f5a  .cur_Reach_infoZ
+00004310: 0a63 7572 6361 745f 6964 785a 0d6d 6178  .curcat_idxZ.max
+00004320: 5f73 7472 616f 7264 6572 7223 0000 005a  _straorderr#...Z
+00004330: 0244 4172 2400 0000 7224 0000 0072 2500  .DAr$...r$...r%.
+00004340: 0000 72b2 0000 0091 0300 0073 7c01 0000  ..r........s|...
+00004350: 000c 0401 0a01 0403 1601 1601 1402 1001  ................
+00004360: 0401 0402 1401 0a01 1c01 0e01 0e02 1802  ................
+00004370: 1603 0e01 0401 0602 0a01 0401 0cff 0804  ................
+00004380: 0e01 0e01 0401 10ff 0803 0401 0402 0201  ................
+00004390: 0cff 0e02 0e01 0e01 0e0c 2eff 0e0b 0801  ................
+000043a0: 0a02 0a01 0c03 1001 0402 1401 0801 0402  ................
+000043b0: 1401 1601 1601 0c03 0e01 0401 0605 0a01  ................
+000043c0: 0401 0cff 0803 0e01 0e01 0401 10ff 0803  ................
+000043d0: 0401 0403 0aff 0403 0402 0e02 0c01 0cff  ................
+000043e0: 0202 02fe 02ff 0c05 0201 02ff 0402 02fe  ................
+000043f0: 0e04 10ff 0c05 0cff 0601 02ff 0403 0c01  ................
+00004400: 0401 0eff 0201 0cff 0e03 2201 1001 0eff  ..........".....
+00004410: 04ff 0203 0cfd 0e05 1a01 06ff 0202 1afe  ................
+00004420: 0203 0cfd 0e0e 1603 1602 0c01 0401 04ff  ................
+00004430: 0604 0c01 0eff 0202 02fe 02ff 0c06 0c01  ................
+00004440: 0401 0eff 0201 0cff 0e03 2201 1001 0eff  ..........".....
+00004450: 04ff 0203 0cfd 0e05 1a01 06ff 0202 1afe  ................
+00004460: 0203 0cfd 0e0d 1201 08ff 0804 10ff 0c03  ................
+00004470: 0e01 1201 0a03 0401 08ff 0402 0e01 0e01  ................
+00004480: 1201 0802 1402 0c01 0801 0c02 1401 1401  ................
+00004490: 1401 1401 1401 1401 0c01 1401 1401 1401  ................
+000044a0: 1401 1409 1201 0a04 1401 1402 1401 0cfe  ................
+000044b0: 0e06 1401 0e03 0a01 0c01 02ff 0601 02ff  ................
+000044c0: 0602 0e01 0e02 0401 10ff 1416 72b2 0000  ............r...
+000044d0: 0063 0200 0000 0000 0000 0000 0000 0b00  .c..............
+000044e0: 0000 0600 0000 4300 0000 7320 0100 0074  ......C...s ...t
+000044f0: 00a0 0164 017c 01a1 027d 0274 00a0 0174  ...d.|...}.t...t
+00004500: 027c 0083 0164 0217 0064 0266 0264 03a1  .|...d...d.f.d..
+00004510: 027d 0364 047d 0474 03a0 037c 00a1 017d  .}.d.}.t...|...}
+00004520: 0574 027c 0283 0164 046b 0490 0172 0674  .t.|...d.k...r.t
+00004530: 00a0 0174 027c 0083 0164 0217 0064 0266  ...t.|...d...d.f
+00004540: 0264 03a1 027d 0664 047d 0774 0464 0474  .d...}.d.}.t.d.t
+00004550: 027c 0283 0183 0244 005d 827d 087c 027c  .|.....D.].}.|.|
+00004560: 0819 007c 037c 043c 007c 0464 0217 007d  ...|.|.<.|.d...}
+00004570: 0474 00a0 057c 0564 0564 0585 0264 0266  .t...|.d.d...d.f
+00004580: 0219 007c 027c 0819 006b 02a1 01a0 0674  ...|.|...k.....t
+00004590: 07a1 017d 0974 0464 0474 027c 0983 0183  ...}.t.d.t.|....
+000045a0: 0244 005d 367d 0a7c 057c 097c 0a19 0064  .D.]6}.|.|.|...d
+000045b0: 0466 0219 007c 0376 0072 ce71 b47c 057c  .f...|.v.r.q.|.|
+000045c0: 097c 0a19 0064 0466 0219 007c 067c 073c  .|...d.f...|.|.<
+000045d0: 007c 0764 0217 007d 0771 b471 6a74 00a0  .|.d...}.q.qjt..
+000045e0: 087c 06a1 017d 067c 067c 0664 046b 0519  .|...}.|.|.d.k..
+000045f0: 007d 0271 3274 00a0 087c 03a1 017d 037c  .}.q2t...|...}.|
+00004600: 037c 0364 046b 0519 007d 037c 0353 0029  .|.d.k...}.|.S.)
+00004610: 067a 9f46 756e 6374 696f 6e73 2077 696c  .z.Functions wil
+00004620: 6c20 7265 7475 726e 2075 7073 7472 6561  l return upstrea
+00004630: 6d20 6964 7320 696e 206f 7574 2074 6168  m ids in out tah
+00004640: 7420 6472 6169 6e61 6765 0a20 2020 2020  t drainage.     
+00004650: 2020 2074 6f20 6f75 746c 6574 6964 0a20     to outletid. 
+00004660: 2020 202d 2d2d 2d2d 2d2d 2d2d 2d0a 0a20     ----------.. 
+00004670: 2020 204e 6f74 6573 0a20 2020 202d 2d2d     Notes.    ---
+00004680: 2d2d 2d2d 0a0a 2020 2020 5265 7475 726e  ----..    Return
+00004690: 733a 0a20 2020 202d 2d2d 2d2d 2d2d 0a20  s:.    -------. 
+000046a0: 2020 2020 2020 2053 6865 6469 640a 2020         Shedid.  
+000046b0: 2020 2902 7228 0000 0072 2800 0000 7228    ).r(...r(...r(
+000046c0: 0000 006c fdff ffff ff67 ed10 5d00 7201  ...l.....g..].r.
+000046d0: 0000 004e 2909 721a 0000 0072 7100 0000  ...N).r....rq...
+000046e0: 7215 0000 0072 1400 0000 7229 0000 00da  r....r....r)....
+000046f0: 0861 7267 7768 6572 6572 1600 0000 722d  .argwherer....r-
+00004700: 0000 0072 2b00 0000 290b da03 6f75 74da  ...r+...)...out.
+00004710: 086f 7574 6c65 7469 645a 076f 7473 6865  .outletidZ.otshe
+00004720: 6473 5a06 5368 6564 6964 5a04 7073 6964  dsZ.ShedidZ.psid
+00004730: da04 726f 7574 5a07 6e6f 7574 7368 645a  ..routZ.noutshdZ
+00004740: 0770 6f73 6864 6964 7247 0000 005a 0469  .poshdidrG...Z.i
+00004750: 726f 7772 5b00 0000 7224 0000 0072 2400  rowr[...r$...r$.
+00004760: 0000 7225 0000 0072 1700 0000 b404 0000  ..r%...r........
+00004770: 732a 0000 0000 0c0c 0118 0104 010a 010e  s*..............
+00004780: 0118 0104 0212 030c 0308 0124 0212 0214  ...........$....
+00004790: 0102 0114 010c 010a 010e 010a 010c 0172  ...............r
+000047a0: 1700 0000 6303 0000 0000 0000 0000 0000  ....c...........
+000047b0: 000d 0000 0006 0000 0043 0000 0073 a601  .........C...s..
+000047c0: 0000 7c02 6401 6402 6702 1900 a000 6403  ..|.d.d.g.....d.
+000047d0: a101 6a01 7d03 7402 6404 7403 7c02 8301  ..j.}.t.d.t.|...
+000047e0: 8302 4400 9001 5d78 7d04 7c02 6401 1900  ..D...]x}.|.d...
+000047f0: 6a01 7c04 1900 7d05 7c02 6405 1900 6a01  j.|...}.|.d...j.
+00004800: 7c04 1900 7d06 7c00 6a04 7c00 6406 1900  |...}.|.j.|.d...
+00004810: 7c05 6b02 1900 a005 a100 7d07 7403 7406  |.k.......}.t.t.
+00004820: 7c03 7c05 8302 8301 7c02 6a04 7c02 6401  |.|.....|.j.|.d.
+00004830: 1900 7c05 6b02 6407 6602 3c00 7403 7c07  ..|.k.d.f.<.t.|.
+00004840: 8301 6404 6b01 7288 7122 7c07 6408 1900  ..d.k.r.q"|.d...
+00004850: 6409 6b02 7d08 7c07 6a04 7c08 640a 6602  d.k.}.|.j.|.d.f.
+00004860: 1900 6a01 6404 1900 7d09 7c09 7c02 6a04  ..j.d...}.|.|.j.
+00004870: 7c02 6401 1900 7c05 6b02 640b 6602 3c00  |.d...|.k.d.f.<.
+00004880: 7c02 6402 1900 6a01 7c04 1900 7d0a 7c0a  |.d...j.|...}.|.
+00004890: 6404 6b00 72d6 7122 7c01 6a04 7c01 6405  d.k.r.q"|.j.|.d.
+000048a0: 1900 7c06 6b02 1900 a005 a100 7d0b 7403  ..|.k.......}.t.
+000048b0: 7c0b 8301 640c 6b02 9001 722a 7c0a 640d  |...d.k...r*|.d.
+000048c0: 6b03 9001 722a 7c0b 640a 1900 6a01 6404  k...r*|.d...j.d.
+000048d0: 1900 7d0c 7c0c 7c00 6a04 7c00 640a 1900  ..}.|.|.j.|.d...
+000048e0: 7c09 6b02 6408 6602 3c00 7122 7c0a 640d  |.k.d.f.<.q"|.d.
+000048f0: 6b02 9001 724c 6409 7c00 6a04 7c00 640a  k...rLd.|.j.|.d.
+00004900: 1900 7c09 6b02 6408 6602 3c00 7122 7407  ..|.k.d.f.<.q"t.
+00004910: 640e 8301 0100 7407 640f 7c05 6410 7c0a  d.....t.d.|.d.|.
+00004920: 8304 0100 7407 7c0a 7c06 8302 0100 7407  ....t.|.|.....t.
+00004930: 7c0b 8301 0100 7407 7c09 8301 0100 7407  |.....t.|.....t.
+00004940: 7c01 6405 640a 6702 1900 8301 0100 7407  |.d.d.g.......t.
+00004950: 6411 8301 0100 7407 640e 8301 0100 7122  d.....t.d.....q"
+00004960: 7c00 7c02 6602 5300 2912 612b 0400 004d  |.|.f.S.).a+...M
+00004970: 6f64 6966 7920 6f75 746c 6574 2073 7562  odify outlet sub
+00004980: 6261 7369 6e27 7320 646f 776e 7374 7265  basin's downstre
+00004990: 616d 2073 7562 6261 7369 6e20 4944 2066  am subbasin ID f
+000049a0: 6f72 2065 6163 6820 7375 6272 6567 696f  or each subregio
+000049b0: 6e0a 2020 2020 5061 7261 6d65 7465 7273  n.    Parameters
+000049c0: 0a20 2020 202d 2d2d 2d2d 2d2d 2d2d 2d0a  .    ----------.
+000049d0: 2020 2020 416c 6c43 6174 696e 666f 2020      AllCatinfo  
+000049e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000049f0: 2020 2020 2020 3a20 6461 7461 6672 616d        : datafram
+00004a00: 650a 2020 2020 2020 2020 6974 2069 7320  e.        it is 
+00004a10: 6120 6461 7461 6672 616d 6520 6f66 2074  a dataframe of t
+00004a20: 6865 2061 7474 7269 6275 7465 2074 6162  he attribute tab
+00004a30: 6c65 2072 6561 6465 6420 6672 6f6d 2066  le readed from f
+00004a40: 696e 616c 6361 745f 696e 666f 0a20 2020  inalcat_info.   
+00004a50: 2020 2020 202e 7368 7020 6f72 2066 696e       .shp or fin
+00004a60: 616c 7269 7670 6c79 5f69 6e66 6f2e 7368  alrivply_info.sh
+00004a70: 700a 2020 2020 446f 776e 4361 7469 6e66  p.    DownCatinf
+00004a80: 6f20 2020 2020 2020 2020 2020 2020 2020  o               
+00004a90: 2020 2020 2020 2020 3a20 6461 7461 6672          : datafr
+00004aa0: 616d 650a 2020 2020 2020 2020 4974 2069  ame.        It i
+00004ab0: 7320 6120 6461 7461 6672 616d 6520 696e  s a dataframe in
+00004ac0: 636c 7564 6573 2074 776f 2063 6f6c 756d  cludes two colum
+00004ad0: 6e73 3a0a 2020 2020 2020 2020 2753 7562  ns:.        'Sub
+00004ae0: 5f52 6567 5f49 4427 3a20 7468 6520 7375  _Reg_ID': the su
+00004af0: 6272 6567 696f 6e20 6964 0a20 2020 2020  bregion id.     
+00004b00: 2020 2027 446f 775f 5375 625f 5265 675f     'Dow_Sub_Reg_
+00004b10: 4964 273a 2064 6f77 6e73 7472 6561 6d20  Id': downstream 
+00004b20: 7375 6262 6173 696e 2069 6420 6f66 2074  subbasin id of t
+00004b30: 6865 206f 7574 6c65 7420 7375 6262 6173  he outlet subbas
+00004b40: 696e 2069 6e0a 2020 2020 2020 2020 7468  in in.        th
+00004b50: 6973 2073 7562 7265 6769 6f6e 0a20 2020  is subregion.   
+00004b60: 2053 7562 5f52 6567 696f 6e5f 696e 666f   Sub_Region_info
+00004b70: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00004b80: 2020 203a 2064 6174 6166 7261 6d65 0a20     : dataframe. 
+00004b90: 2020 2020 2020 2049 7420 6973 2061 2064         It is a d
+00004ba0: 6174 6166 7261 6d65 2069 6e63 6c75 6465  ataframe include
+00004bb0: 7320 7375 6272 6567 696f 6e20 696e 666f  s subregion info
+00004bc0: 726d 6174 696f 6e73 2c20 7769 7468 2066  rmations, with f
+00004bd0: 6f6c 6c6f 7769 6e67 0a20 2020 2020 2020  ollowing.       
+00004be0: 2063 6f6c 756d 6e73 3a0a 2020 2020 2020   columns:.      
+00004bf0: 2020 2753 7562 5f52 6567 5f49 4427 203a    'Sub_Reg_ID' :
+00004c00: 2074 6865 2073 7562 7265 6769 6f6e 2069   the subregion i
+00004c10: 640a 2020 2020 2020 2020 2744 6f77 5f53  d.        'Dow_S
+00004c20: 7562 5f52 6567 5f49 6427 3a20 7468 6520  ub_Reg_Id': the 
+00004c30: 646f 776e 7374 7265 616d 2073 7562 7265  downstream subre
+00004c40: 6769 6f6e 2069 640a 0a20 2020 204e 6f74  gion id..    Not
+00004c50: 6573 0a20 2020 202d 2d2d 2d2d 2d2d 0a0a  es.    -------..
+00004c60: 2020 2020 5265 7475 726e 733a 0a20 2020      Returns:.   
+00004c70: 202d 2d2d 2d2d 2d2d 0a20 2020 2020 2020   -------.       
+00004c80: 2053 7562 5f52 6567 696f 6e5f 696e 666f   Sub_Region_info
+00004c90: 2020 2020 2020 3a20 6461 7461 6672 616d        : datafram
+00004ca0: 650a 2020 2020 2020 2020 2020 2020 416e  e.            An
+00004cb0: 206e 6577 2063 6f6c 756d 6e73 2069 6e64   new columns ind
+00004cc0: 6963 6174 6520 7468 6520 6f75 746c 6574  icate the outlet
+00004cd0: 2073 7562 6261 7369 6e20 6964 206f 6620   subbasin id of 
+00004ce0: 7468 6520 7375 6220 7265 6769 6f6e 0a20  the sub region. 
+00004cf0: 2020 2020 2020 2020 2020 2077 696c 6c20             will 
+00004d00: 6265 2061 6464 6564 0a20 2020 2020 2020  be added.       
+00004d10: 2041 6c6c 4361 7469 6e66 6f20 2020 2020   AllCatinfo     
+00004d20: 2020 2020 2020 3a20 6461 7461 6672 616d        : datafram
+00004d30: 650a 2020 2020 2020 2020 2020 2020 446f  e.            Do
+00004d40: 776e 7374 7265 616d 2073 7562 6261 7369  wnstream subbasi
+00004d50: 6e20 4944 206f 6620 6561 6368 2073 7562  n ID of each sub
+00004d60: 7265 6769 6f6e 2773 206f 7574 6c65 7420  region's outlet 
+00004d70: 7375 6262 6173 696e 2077 696c 6c0a 2020  subbasin will.  
+00004d80: 2020 2020 2020 2020 2020 6265 2075 7064            be upd
+00004d90: 6174 6564 2e0a 2020 2020 da0a 5375 625f  ated..    ..Sub_
+00004da0: 5265 675f 4944 da0e 446f 775f 5375 625f  Reg_ID..Dow_Sub_
+00004db0: 5265 675f 4964 7260 0000 0072 0100 0000  Reg_Idr`...r....
+00004dc0: da07 494c 7074 5f49 44da 0952 6567 696f  ..ILpt_ID..Regio
+00004dd0: 6e5f 4944 da0e 4e5f 5570 5f53 7562 5265  n_ID..N_Up_SubRe
+00004de0: 6769 6f6e 720d 0000 0072 6600 0000 7206  gionr....rf...r.
+00004df0: 0000 00da 0c4f 7574 6c65 745f 5375 6249  .....Outlet_SubI
+00004e00: 6472 2800 0000 e97f 3801 007a 3223 2323  dr(.....8..z2###
+00004e10: 2323 2323 2323 2323 2323 2323 2323 2323  ################
+00004e20: 2323 2323 2323 2323 2323 2323 2323 2323  ################
+00004e30: 2323 2323 2323 2323 2323 2323 2323 237a  ###############z
+00004e40: 0c53 7562 7265 6769 6f6e 203a 207a 0720  .Subregion : z. 
+00004e50: 2020 546f 2020 7a1a 4e65 6564 2062 6520    To  z.Need be 
+00004e60: 6d61 6e75 616c 6c79 2063 6f6e 6e65 6374  manually connect
+00004e70: 6564 2908 7216 0000 0072 1300 0000 7229  ed).r....r....r)
+00004e80: 0000 0072 1500 0000 7219 0000 0072 1400  ...r....r....r..
+00004e90: 0000 7217 0000 0072 6800 0000 290d da0a  ..r....rh...)...
+00004ea0: 416c 6c43 6174 696e 666f 5a0b 446f 776e  AllCatinfoZ.Down
+00004eb0: 4361 7469 6e66 6fda 0f53 7562 5f52 6567  Catinfo..Sub_Reg
+00004ec0: 696f 6e5f 696e 666f 726a 0000 0072 4700  ion_inforj...rG.
+00004ed0: 0000 5a0a 6973 7562 7265 6769 6f6e 72cb  ..Z.isubregionr.
+00004ee0: 0000 005a 1353 7562 5f52 6567 696f 6e5f  ...Z.Sub_Region_
+00004ef0: 6361 745f 696e 666f 5a0b 6f75 746c 6574  cat_infoZ.outlet
+00004f00: 5f6d 6173 6b5a 1169 5265 675f 4f75 746c  _maskZ.iReg_Outl
+00004f10: 6574 5f53 7562 6964 5a11 446f 775f 5375  et_SubidZ.Dow_Su
+00004f20: 625f 5265 6769 6f6e 5f69 64da 0d44 6f77  b_Region_id..Dow
+00004f30: 6e5f 5375 625f 696e 666f 5a09 446f 776e  n_Sub_infoZ.Down
+00004f40: 5375 6269 6472 2400 0000 7224 0000 0072  Subidr$...r$...r
+00004f50: 2500 0000 da22 436f 6e6e 6563 745f 5375  %...."Connect_Su
+00004f60: 6252 6567 696f 6e5f 5570 6461 7465 5f44  bRegion_Update_D
+00004f70: 6f77 6e53 7562 4964 de04 0000 7368 0000  ownSubId....sh..
+00004f80: 0000 230c 0102 ff04 ff02 0414 030e 020e  ..#.............
+00004f90: 0204 010a ff08 060c fe04 010e ff02 050c  ................
+00004fa0: 0102 030c 0106 0102 ff06 0102 ff04 0502  ................
+00004fb0: fe04 010e ff02 040e 0408 0102 0316 0318  ................
+00004fc0: 010e 0302 fe04 010e ff04 060a 0202 ff0a  ................
+00004fd0: 0102 ff02 0102 ff06 0308 010e 010a 0108  ................
+00004fe0: 0108 0110 0108 010a 0172 d300 0000 6304  .........r....c.
+00004ff0: 0000 0000 0000 0000 0000 0019 0000 000a  ................
+00005000: 0000 0043 0000 0073 0605 0000 7c01 7c01  ...C...s....|.|.
+00005010: 6401 1900 6402 6b02 1900 6403 1900 6a00  d...d.k...d...j.
+00005020: 7d04 7401 a002 7c04 a101 7d04 7c04 a003  }.t...|...}.|...
+00005030: a100 7d04 7404 7c00 6a05 7c00 6404 1900  ..}.t.|.j.|.d...
+00005040: 6405 6b02 1900 8301 6402 6b04 7264 7406  d.k.....d.k.rdt.
+00005050: 6406 8301 0100 7406 7c00 6a05 7c00 6404  d.....t.|.j.|.d.
+00005060: 1900 6405 6b02 1900 8301 0100 7c00 5300  ..d.k.......|.S.
+00005070: 7404 7c00 6a05 7c00 6404 1900 6405 6b02  t.|.j.|.d...d.k.
+00005080: 1900 8301 6407 6b02 728a 7406 6408 8301  ....d.k.r.t.d...
+00005090: 0100 7c00 5300 7c00 6a05 7c00 6404 1900  ..|.S.|.j.|.d...
+000050a0: 6405 6b02 1900 6409 1900 6a00 6407 1900  d.k...d...j.d...
+000050b0: a007 7408 a101 7d05 640a 7d06 7409 6407  ..t...}.d.}.t.d.
+000050c0: 7404 7c01 8301 8302 4400 5d94 7d07 7c01  t.|.....D.].}.|.
+000050d0: 640b 1900 6a00 7c07 1900 7d08 7c06 7c00  d...j.|...}.|.|.
+000050e0: 6a05 7c00 6409 1900 7c08 6b02 1900 640c  j.|.d...|.k...d.
+000050f0: 1900 6a00 6407 1900 1700 7d06 7406 640d  ..j.d.....}.t.d.
+00005100: 7c01 6403 1900 6a00 7c07 1900 8302 0100  |.d...j.|.......
+00005110: 7406 640e 7c00 6a05 7c00 6409 1900 7c08  t.d.|.j.|.d...|.
+00005120: 6b02 1900 640c 1900 6a00 6407 1900 8302  k...d...j.d.....
+00005130: 0100 7406 640f 740a 7c00 6a05 7c00 6410  ..t.d.t.|.j.|.d.
+00005140: 1900 7c01 6403 1900 6a00 7c07 1900 6b02  ..|.d...j.|...k.
+00005150: 1900 6411 1900 6a00 8301 8302 0100 71be  ..d...j.......q.
+00005160: 6402 7d09 7404 7c04 8301 6407 6b04 9004  d.}.t.|...d.k...
+00005170: 72b6 7406 6412 7c09 8302 0100 7406 7c04  r.t.d.|.....t.|.
+00005180: 8301 0100 740b a00b 7c04 a101 7d0a 6700  ....t...|...}.g.
+00005190: 7d04 7409 6407 7404 7c0a 8301 8302 4400  }.t.d.t.|.....D.
+000051a0: 9003 5d06 7d07 7c0a 7c07 1900 7d0b 7c0b  ..].}.|.|...}.|.
+000051b0: 6413 6b02 9001 72b0 9001 7194 7c01 7c01  d.k...r...q.|.|.
+000051c0: 6403 1900 7c0b 6b02 1900 6414 1900 6a00  d...|.k...d...j.
+000051d0: 6407 1900 7d0c 7c04 a00c 7c0c a101 0100  d...}.|...|.....
+000051e0: 7c01 7c01 6403 1900 7c0b 6b02 1900 640b  |.|.d...|.k...d.
+000051f0: 1900 6a00 6407 1900 7d08 7c00 6a05 7c00  ..j.d...}.|.j.|.
+00005200: 6409 1900 7c08 6b02 1900 a00b a100 7d0d  d...|.k.......}.
+00005210: 7c0d 6404 1900 6a00 6407 1900 7d0e 7404  |.d...j.d...}.t.
+00005220: 7c00 6a05 7c00 6409 1900 7c0e 6b02 1900  |.j.|.d...|.k...
+00005230: 8301 6407 6b01 9002 726c 7408 7c0b 8301  ..d.k...rlt.|...
+00005240: 7408 7c05 8301 6b03 9001 7294 7406 6415  t.|...k...r.t.d.
+00005250: 7c0b 8302 0100 7406 6416 7c08 6417 7c0e  |.....t.d.|.d.|.
+00005260: 7c05 7408 7c0b 8301 7408 7c05 8301 6b03  |.t.|...t.|...k.
+00005270: 8306 0100 9001 7194 7c00 6a05 7c00 6409  ......q.|.j.|.d.
+00005280: 1900 7c0e 6b02 1900 6410 1900 6a00 6407  ..|.k...d...j.d.
+00005290: 1900 7d0f 7406 6415 7c0b 7c0f 7c0c 7c0e  ..}.t.d.|.|.|.|.
+000052a0: 8305 0100 7c0f 7c0c 6b03 9002 72b4 7406  ....|.|.k...r.t.
+000052b0: 6415 7c0b 6418 7c0c 8304 0100 9001 7194  d.|.d.|.......q.
+000052c0: 7c0f 7c0c 6b02 9001 7294 7c0e 7d10 7406  |.|.k...r.|.}.t.
+000052d0: 6415 7c0b 7c0f 7c0c 7c0e 7c10 8306 0100  d.|.|.|.|.|.....
+000052e0: 7c00 6a05 7c00 6409 1900 7c10 6b02 1900  |.j.|.d...|.k...
+000052f0: a00b a100 7d11 7c00 6a05 7c00 6404 1900  ....}.|.j.|.d...
+00005300: 7c10 6b02 1900 a00b a100 7d12 7c11 6411  |.k.......}.|.d.
+00005310: 1900 6a00 6407 1900 740a 7c12 640c 1900  ..j.d...t.|.d...
+00005320: 6a00 8301 1700 7d13 7c12 6419 1900 6a00  j.....}.|.d...j.
+00005330: 7d14 740d 7c14 8301 7d15 7401 a00a 7c14  }.t.|...}.t...|.
+00005340: 7c15 6b02 a101 641a 6b05 9003 724c 7c15  |.k...d.k...rL|.
+00005350: 6402 1700 7d16 6e04 7c15 7d16 7c16 7c00  d...}.n.|.}.|.|.
+00005360: 6a05 7c00 6409 1900 7c10 6b02 6419 6602  j.|.d...|.k.d.f.
+00005370: 3c00 7c13 7c00 6a05 7c00 6409 1900 7c10  <.|.|.j.|.d...|.
+00005380: 6b02 640c 6602 3c00 7c00 7c00 6409 1900  k.d.f.<.|.|.d...
+00005390: 7c10 6b02 1900 641b 1900 6a00 6407 1900  |.k...d...j.d...
+000053a0: 6407 6b04 9004 7212 7c00 7c00 6409 1900  d.k...r.|.|.d...
+000053b0: 7c10 6b02 1900 641b 1900 6a00 6407 1900  |.k...d...j.d...
+000053c0: 7d17 7c00 7c00 6409 1900 7c10 6b02 1900  }.|.|.d...|.k...
+000053d0: 640c 1900 6a00 6407 1900 641c 1b00 641c  d...j.d...d...d.
+000053e0: 1b00 7d18 7c17 6407 6b04 9004 7212 7c18  ..}.|.d.k...r.|.
+000053f0: 7c17 1b00 7c00 6a05 7c00 6409 1900 7c10  |...|.j.|.d...|.
+00005400: 6b02 641d 6602 3c00 6402 7c00 6a05 7c00  k.d.f.<.d.|.j.|.
+00005410: 6409 1900 7c10 6b02 641e 6602 3c00 7c11  d...|.k.d.f.<.|.
+00005420: 6404 1900 6a00 6407 1900 7d0e 7404 7c00  d...j.d...}.t.|.
+00005430: 6a05 7c00 6409 1900 7c0e 6b02 1900 8301  j.|.d...|.k.....
+00005440: 6407 6b01 9004 727a 7408 7c10 8301 7408  d.k...rzt.|...t.
+00005450: 7c05 8301 6b03 9004 729a 7406 6415 7c0c  |...k...r.t.d.|.
+00005460: 8302 0100 7406 6416 7c10 6417 7c0e 7c05  ....t.d.|.d.|.|.
+00005470: 7408 7c10 8301 7408 7c05 8301 6b03 8306  t.|...t.|...k...
+00005480: 0100 9001 7194 7c00 6a05 7c00 6409 1900  ....q.|.j.|.d...
+00005490: 7c0e 6b02 1900 6410 1900 6a00 6407 1900  |.k...d...j.d...
+000054a0: 7d0f 9002 71b4 9001 7194 740e 740f 7c04  }...q...q.t.t.|.
+000054b0: 8301 8301 7d04 7c09 6402 1700 7d09 9001  ....}.|.d...}...
+000054c0: 7158 7406 641f 8301 0100 7406 6420 740a  qXt.d.....t.d t.
+000054d0: 7c00 6411 1900 6a00 8301 8302 0100 7406  |.d...j.......t.
+000054e0: 6421 7c00 6a05 7c00 6409 1900 7408 7c05  d!|.j.|.d...t.|.
+000054f0: 8301 6b02 1900 640c 1900 6a00 6407 1900  ..k...d...j.d...
+00005500: 8302 0100 7406 6422 7c06 8302 0100 7c00  ....t.d"|.....|.
+00005510: 5300 2923 6115 0300 0055 7064 6174 6520  S.)#a....Update 
+00005520: 4472 6169 6e61 6765 2061 7265 612c 2073  Drainage area, s
+00005530: 7472 6168 6c65 7220 6f72 6465 7220 6f66  trahler order of
+00005540: 2073 7562 6261 696e 730a 0a20 2020 2055   subbains..    U
+00005550: 7064 6174 6520 6472 6169 6e61 6765 2061  pdate drainage a
+00005560: 7265 6120 616e 6420 7374 7261 686c 6572  rea and strahler
+00005570: 206f 7264 6572 2066 6f72 2063 6f6d 6269   order for combi
+00005580: 6e65 6420 726f 7574 696e 6720 7072 6f64  ned routing prod
+00005590: 7563 740a 2020 2020 6f66 2065 6163 6820  uct.    of each 
+000055a0: 7375 6272 6567 696f 6e73 0a20 2020 2050  subregions.    P
+000055b0: 6172 616d 6574 6572 730a 2020 2020 2d2d  arameters.    --
+000055c0: 2d2d 2d2d 2d2d 2d2d 0a20 2020 2041 6c6c  --------.    All
+000055d0: 4361 7469 6e66 6f20 2020 2020 2020 2020  Catinfo         
+000055e0: 2020 2020 2020 2020 2020 2020 2020 203a                 :
+000055f0: 2064 6174 6166 7261 6d65 0a20 2020 2020   dataframe.     
+00005600: 2020 2069 7420 6973 2061 2064 6174 6166     it is a dataf
+00005610: 7261 6d65 206f 6620 7468 6520 6174 7472  rame of the attr
+00005620: 6962 7574 6520 7461 626c 6520 7265 6164  ibute table read
+00005630: 6564 2066 726f 6d20 6669 6e61 6c63 6174  ed from finalcat
+00005640: 5f69 6e66 6f0a 2020 2020 2020 2020 2e73  _info.        .s
+00005650: 6870 206f 7220 6669 6e61 6c72 6976 706c  hp or finalrivpl
+00005660: 795f 696e 666f 2e73 6870 0a20 2020 2053  y_info.shp.    S
+00005670: 7562 5f52 6567 696f 6e5f 696e 666f 2020  ub_Region_info  
+00005680: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00005690: 203a 2064 6174 6166 7261 6d65 0a20 2020   : dataframe.   
+000056a0: 2020 2020 2049 7420 6973 2061 2064 6174       It is a dat
+000056b0: 6166 7261 6d65 2069 6e63 6c75 6465 7320  aframe includes 
+000056c0: 7375 6272 6567 696f 6e20 696e 666f 726d  subregion inform
+000056d0: 6174 696f 6e73 2c20 7769 7468 2066 6f6c  ations, with fol
+000056e0: 6c6f 7769 6e67 0a20 2020 2020 2020 2063  lowing.        c
+000056f0: 6f6c 756d 6e73 3a0a 2020 2020 2020 2020  olumns:.        
+00005700: 2753 7562 5f52 6567 5f49 4427 203a 2074  'Sub_Reg_ID' : t
+00005710: 6865 2073 7562 7265 6769 6f6e 2069 640a  he subregion id.
+00005720: 2020 2020 2020 2020 2744 6f77 5f53 7562          'Dow_Sub
+00005730: 5f52 6567 5f49 6427 3a20 7468 6520 646f  _Reg_Id': the do
+00005740: 776e 7374 7265 616d 2073 7562 7265 6769  wnstream subregi
+00005750: 6f6e 2069 640a 0a20 2020 204e 6f74 6573  on id..    Notes
+00005760: 0a20 2020 202d 2d2d 2d2d 2d2d 0a0a 2020  .    -------..  
+00005770: 2020 5265 7475 726e 733a 0a20 2020 202d    Returns:.    -
+00005780: 2d2d 2d2d 2d2d 0a20 2020 2041 6c6c 4361  ------.    AllCa
+00005790: 7469 6e66 6f20 2020 2020 2020 2020 2020  tinfo           
+000057a0: 3a20 6461 7461 6672 616d 650a 2020 2020  : dataframe.    
+000057b0: 2020 2020 446f 776e 7374 7265 616d 2044      Downstream D
+000057c0: 4120 616e 6420 7374 7261 686c 6572 206f  A and strahler o
+000057d0: 7264 6572 206f 6620 6561 6368 2073 7562  rder of each sub
+000057e0: 7265 6769 6f6e 2061 6c6f 6e67 2074 6865  region along the
+000057f0: 2066 6c6f 770a 2020 2020 2020 2020 7061   flow.        pa
+00005800: 7468 7761 7920 6265 7477 6565 6e20 7375  thway between su
+00005810: 6272 6567 696f 6e73 2077 696c 6c20 6265  bregions will be
+00005820: 2075 7064 6174 6564 2e0a 2020 2020 72cd   updated..    r.
+00005830: 0000 0072 2800 0000 72c9 0000 0072 0d00  ...r(...r....r..
+00005840: 0000 7266 0000 007a 1f57 6174 6865 7273  ..rf...z.Wathers
+00005850: 6564 2068 6173 206d 756c 7469 706c 6520  ed has multiple 
+00005860: 6f75 746c 6574 2020 7201 0000 007a 1757  outlet  r....z.W
+00005870: 6174 6572 7368 6564 2068 6173 206e 6f20  atershed has no 
+00005880: 6f75 746c 6574 7206 0000 0072 be00 0000  outletr....r....
+00005890: 72ce 0000 0072 6c00 0000 7a26 2323 2323  r....rl...z&####
+000058a0: 2323 4172 6561 2061 6e64 2044 4120 6368  ##Area and DA ch
+000058b0: 6563 6b20 666f 7220 7375 6272 6567 696f  eck for subregio
+000058c0: 6e20 7a21 4441 2061 7420 7468 6520 7375  n z!DA at the su
+000058d0: 6272 6567 696f 6e20 6f75 746c 6574 2069  bregion outlet i
+000058e0: 7320 2020 207a 2154 6f74 616c 2073 7562  s    z!Total sub
+000058f0: 7265 6769 6f6e 2061 7265 6120 6973 2020  region area is  
+00005900: 2020 2020 2020 2020 72cc 0000 0072 7a00          r....rz.
+00005910: 0000 7a06 6c6f 6f70 2020 72cf 0000 0072  ..z.loop  r....r
+00005920: ca00 0000 7a0d 5375 6272 6567 696f 6e3a  ....z.Subregion:
+00005930: 2020 207a 0953 7562 4964 2069 7320 7a0f     z.SubId is z.
+00005940: 2044 6f77 6e53 7562 4964 2069 7320 207a   DownSubId is  z
+00005950: 1c20 2064 6964 206e 6f74 2063 6f6e 6e65  .  did not conne
+00005960: 6374 6564 2077 6974 6820 2020 2072 6400  cted with    rd.
+00005970: 0000 7262 0000 0072 bf00 0000 72c0 0000  ..rb...r....r...
+00005980: 0072 c100 0000 5a0a 5573 655f 7265 6769  .r....Z.Use_regi
+00005990: 6f6e 7a14 4368 6563 6b20 6472 6169 6e61  onz.Check draina
+000059a0: 6765 2061 7265 613a 7a21 546f 7461 6c20  ge area:z!Total 
+000059b0: 6261 7369 6e20 6172 6561 2069 7320 2020  basin area is   
+000059c0: 2020 2020 2020 2020 2020 207a 2144 4120             z!DA 
+000059d0: 6f66 2074 6865 2077 6174 6572 7365 6864  of the watersehd
+000059e0: 206f 7574 6c65 7420 6973 2020 2020 7a21   outlet is    z!
+000059f0: 546f 7461 6c20 4441 206f 6620 6561 6368  Total DA of each
+00005a00: 2073 7562 7265 6769 6f6e 2020 2020 2020   subregion      
+00005a10: 2029 1072 1300 0000 721a 0000 0072 2b00   ).r....r....r+.
+00005a20: 0000 da06 746f 6c69 7374 7215 0000 0072  ....tolistr....r
+00005a30: 1900 0000 7268 0000 0072 1600 0000 722d  ....rh...r....r-
+00005a40: 0000 0072 2900 0000 723e 0000 0072 1400  ...r)...r>...r..
+00005a50: 0000 724d 0000 0072 6700 0000 7253 0000  ..rM...rg...rS..
+00005a60: 00da 0373 6574 2919 72d0 0000 0072 d100  ...set).r....r..
+00005a70: 0000 725e 0000 00da 0163 5a0e 5375 6272  ..r^.....cZ.Subr
+00005a80: 6567 696f 6e5f 6c69 7374 5a14 5761 7465  egion_listZ.Wate
+00005a90: 7273 6865 646f 7574 6c65 7473 7562 6964  rshedoutletsubid
+00005aa0: 5a12 546f 7461 6c5f 4441 5f53 7562 7265  Z.Total_DA_Subre
+00005ab0: 6769 6f6e 7247 0000 005a 114f 7574 6c65  gionrG...Z.Outle
+00005ac0: 7473 7562 6964 5f63 7375 6272 5a05 696c  tsubid_csubrZ.il
+00005ad0: 6f6f 705a 1163 7572 7265 6e74 5f6c 6f6f  oopZ.current_loo
+00005ae0: 705f 6c69 7374 5a09 635f 7375 6272 5f69  p_listZ.c_subr_i
+00005af0: 645a 0964 5f73 7562 725f 6964 5a0e 4f75  dZ.d_subr_idZ.Ou
+00005b00: 746c 6574 7375 625f 696e 666f da09 646f  tletsub_info..do
+00005b10: 776e 7375 6269 645a 0e64 6f77 6e73 7562  wnsubidZ.downsub
+00005b20: 5f72 6567 5f69 64da 0663 7375 6269 645a  _reg_id..csubidZ
+00005b30: 0a43 5f73 7562 5f69 6e66 6f5a 0e55 7070  .C_sub_infoZ.Upp
+00005b40: 6572 5f73 7562 5f69 6e66 6f5a 054e 6577  er_sub_infoZ.New
+00005b50: 4441 5a09 5374 7261 686c 6572 735a 0b6d  DAZ.StrahlersZ.m
+00005b60: 6178 5374 7261 686c 6572 5a0b 6e65 7753  axStrahlerZ.newS
+00005b70: 7472 6168 6c65 725a 0664 615f 6f62 735a  trahlerZ.da_obsZ
+00005b80: 0664 615f 7369 6d72 2400 0000 7224 0000  .da_simr$...r$..
+00005b90: 0072 2500 0000 da26 5570 6461 7465 5f44  .r%....&Update_D
+00005ba0: 415f 5374 7261 686c 6572 5f46 6f72 5f43  A_Strahler_For_C
+00005bb0: 6f6d 6269 6e65 645f 5265 7375 6c74 4205  ombined_ResultB.
+00005bc0: 0000 739a 0100 0000 1a0e 0102 ff06 030a  ..s.............
+00005bd0: 0108 051a 0108 0116 0104 011a 0108 0104  ................
+00005be0: 030a 0102 ff04 0102 ff04 0102 ff04 0102  ................
+00005bf0: ff02 ff02 0604 0112 010e 0202 010a 0102  ................
+00005c00: ff04 0102 ff04 0102 ff02 ff02 ff02 0502  ................
+00005c10: 0102 010c fe04 0402 0102 010a 0102 ff04  ................
+00005c20: 0102 ff04 0102 ff02 fe04 0502 0102 0102  ................
+00005c30: 0104 0114 ff02 0202 fe04 ff02 fe06 0904  ................
+00005c40: 010e 010a 0108 010a 0104 0214 0208 020a  ................
+00005c50: 0104 020e 0102 ff04 0202 fe04 040a 0302  ................
+00005c60: 010a ff02 0202 fe04 0202 fe04 0404 010a  ................
+00005c70: ff08 040e 031c 0112 010a 0102 0102 0102  ................
+00005c80: 0102 0102 0102 010e fa04 0804 0210 0102  ................
+00005c90: ff04 0202 fe04 0406 0106 ff04 030a 0102  ................
+00005ca0: 0102 0102 0102 0102 fc04 0604 020a 0104  ................
+00005cb0: 0108 0106 ff04 0316 0316 050e 0108 ff06  ................
+00005cc0: 060a 0108 0114 010a 0204 0302 ff0a 0102  ................
+00005cd0: ff02 0102 ff04 0302 ff0a 0102 ff02 0102  ................
+00005ce0: ff04 0320 0108 0102 ff04 0102 ff04 0102  ... ............
+00005cf0: ff04 0208 0102 ff04 0102 ff04 0102 ff02  ................
+00005d00: 0102 ff02 0102 ff04 020a 0206 ff0a 0102  ................
+00005d10: ff02 0102 ff04 0302 ff0a 0102 ff02 0102  ................
+00005d20: ff04 140e 031c 0112 010a 0102 0102 0102  ................
+00005d30: 0102 0102 0102 010e fa04 0804 0210 0102  ................
+00005d40: ff04 0202 fe0c 050c 010c 0208 0104 010c  ................
+00005d50: ff04 0202 0102 011a 0102 ff02 fe04 060a  ................
+00005d60: 0172 d900 0000 6301 0000 0000 0000 0000  .r....c.........
+00005d70: 0000 0012 0000 0008 0000 0043 0000 0073  ...........C...s
+00005d80: e002 0000 6401 7d01 6402 7d02 6403 7d03  ....d.}.d.}.d.}.
+00005d90: 7400 7c00 7c01 1900 6a01 8301 7d04 7402  t.|.|...j...}.t.
+00005da0: 7c00 8301 7d05 6404 7d06 7403 a004 7c05  |...}.d.}.t...|.
+00005db0: 6405 1700 7403 6a05 a102 7d07 7403 a004  d...t.j...}.t...
+00005dc0: 7c05 6405 1700 7403 6a05 a102 7d08 7406  |.d...t.j...}.t.
+00005dd0: 6406 7402 7c00 8301 8302 4400 9001 5d6a  d.t.|.....D...]j
+00005de0: 7d09 7c00 7c01 1900 6a01 7c09 1900 7d0a  }.|.|...j.|...}.
+00005df0: 7c00 7c03 1900 6a01 7c09 1900 7d0b 7c00  |.|...j.|...}.|.
+00005e00: 7c02 1900 6a01 7c09 1900 7d0c 7a0c 7407  |...j.|...}.z.t.
+00005e10: 7c0a 8301 7d0d 5700 6e1e 0100 0100 0100  |...}.W.n.......
+00005e20: 6407 7d0d 6407 7c00 6a08 7c09 7c01 6602  d.}.d.|.j.|.|.f.
+00005e30: 3c00 5900 6e02 3000 7a0c 7407 7c0b 8301  <.Y.n.0.z.t.|...
+00005e40: 7d0e 5700 6e1e 0100 0100 0100 6407 7d0e  }.W.n.......d.}.
+00005e50: 6407 7c00 6a08 7c09 7c03 6602 3c00 5900  d.|.j.|.|.f.<.Y.
+00005e60: 6e02 3000 7a0c 7407 7c0c 8301 7d0f 5700  n.0.z.t.|...}.W.
+00005e70: 6e1e 0100 0100 0100 6407 7d0f 6407 7c00  n.......d.}.d.|.
+00005e80: 6a08 7c09 7c02 6602 3c00 5900 6e02 3000  j.|.|.f.<.Y.n.0.
+00005e90: 7c0d 6406 6b00 9001 7218 7158 7c0f 6406  |.d.k...r.qX|.d.
+00005ea0: 6b01 9001 7234 7c0d 7d10 6407 7c00 6a08  k...r4|.}.d.|.j.
+00005eb0: 7c09 6408 6602 3c00 7c0f 6406 6b04 9001  |.d.f.<.|.d.k...
+00005ec0: 727a 7c0e 7c0f 6b02 9001 7264 7c0d 7c04  rz|.|.k...rd|.|.
+00005ed0: 1700 6409 1700 7d10 6404 7c00 6a08 7c09  ..d...}.d.|.j.|.
+00005ee0: 6408 6602 3c00 6e16 7407 7c0d 8301 7d10  d.f.<.n.t.|...}.
+00005ef0: 6407 7c00 6a08 7c09 6408 6602 3c00 7c10  d.|.j.|.d.f.<.|.
+00005f00: 7c08 7601 9001 72a4 7c06 7c00 6a08 7c09  |.v...r.|.|.j.|.
+00005f10: 640a 6602 3c00 7c10 7c08 7c06 3c00 7c06  d.f.<.|.|.|.<.|.
+00005f20: 6404 1700 7d06 7158 7409 7403 a00a 7c08  d...}.qXt.t...|.
+00005f30: 7c10 6b02 a101 6406 1900 8301 7c00 6a08  |.k...d.....|.j.
+00005f40: 7c09 640a 6602 3c00 7158 7406 6406 7402  |.d.f.<.qXt.d.t.
+00005f50: 7c00 8301 8302 4400 9001 5d04 7d09 7c00  |.....D...].}.|.
+00005f60: 7c01 1900 6a01 7c09 1900 7d0d 7c00 7c03  |...j.|...}.|.|.
+00005f70: 1900 6a01 7c09 1900 7d0e 7c00 7c02 1900  ..j.|...}.|.|...
+00005f80: 6a01 7c09 1900 7d0f 7c0d 6406 6b04 9002  j.|...}.|.d.k...
+00005f90: 7212 9001 71d4 7c0e 6406 6b01 9002 723e  r...q.|.d.k...r>
+00005fa0: 740b 640b 8301 0100 740b 7c00 6a08 7c09  t.d.....t.|.j.|.
+00005fb0: 640c 640c 8502 6602 1900 8301 0100 9001  d.d...f.........
+00005fc0: 71d4 7c00 6a08 7c00 7c03 1900 7c0e 6b02  q.|.j.|.|...|.k.
+00005fd0: 7c00 6408 1900 6406 6b04 4000 1900 7d11  |.d...d.k.@...}.
+00005fe0: 7402 7c11 8301 6406 6b01 9002 7278 740b  t.|...d.k...rxt.
+00005ff0: 640d 7c0e 8302 0100 9001 71d4 7c11 7c01  d.|.......q.|.|.
+00006000: 1900 6a01 6406 1900 7c00 6a08 7c09 7c01  ..j.d...|.j.|.|.
+00006010: 6602 3c00 7c11 6408 1900 6a01 6406 1900  f.<.|.d...j.d...
+00006020: 7c00 6a08 7c09 6408 6602 3c00 7c11 640a  |.j.|.d.f.<.|.d.
+00006030: 1900 6a01 6406 1900 7c00 6a08 7c09 640a  ..j.d...|.j.|.d.
+00006040: 6602 3c00 7c11 7c02 1900 6a01 6406 1900  f.<.|.|...j.d...
+00006050: 7c00 6a08 7c09 7c02 6602 3c00 9001 71d4  |.j.|.|.f.<...q.
+00006060: 7c00 5300 290e 7aa1 4675 6e63 7469 6f6e  |.S.).z.Function
+00006070: 2074 6f20 6465 7465 726d 696e 2068 7275   to determin hru
+00006080: 6964 2061 6674 6572 2063 6f6d 6269 6e65  id after combine
+00006090: 206c 616b 6520 706f 6c79 676f 6e0a 2020   lake polygon.  
+000060a0: 2020 616e 6420 7375 6262 6173 696e 2070    and subbasin p
+000060b0: 6f6c 7967 6f6e 0a20 2020 202d 2d2d 2d2d  olygon.    -----
+000060c0: 2d2d 2d2d 2d0a 0a20 2020 204e 6f74 6573  -----..    Notes
+000060d0: 0a20 2020 202d 2d2d 2d2d 2d2d 0a0a 2020  .    -------..  
+000060e0: 2020 5265 7475 726e 733a 0a20 2020 202d    Returns:.    -
+000060f0: 2d2d 2d2d 2d2d 0a20 2020 2020 2020 204e  ------.        N
+00006100: 6f6e 652c 0a20 2020 2072 0600 0000 727c  one,.    r....r|
+00006110: 0000 00da 0848 796c 616b 5f69 6472 2800  .....Hylak_idr(.
+00006120: 0000 726e 0000 0072 0100 0000 7266 0000  ..rn...r....rf..
+00006130: 0072 4c00 0000 e90a 0000 00da 0a48 5255  .rL..........HRU
+00006140: 4c61 6b65 5f49 447a 1a6c 616b 6520 6861  Lake_IDz.lake ha
+00006150: 7320 756e 6578 7065 6374 6564 2068 6f6c  s unexpected hol
+00006160: 6573 204e 7a16 4c61 6b65 6964 2064 6f20  es Nz.Lakeid do 
+00006170: 6e6f 7420 6578 6973 7420 2020 290c 7267  not exist   ).rg
+00006180: 0000 0072 1300 0000 7215 0000 0072 1a00  ...r....r....r..
+00006190: 0000 7271 0000 00da 036e 616e 7229 0000  ..rq.....nanr)..
+000061a0: 0072 6000 0000 7219 0000 0072 2d00 0000  .r`...r....r-...
+000061b0: 72c5 0000 0072 6800 0000 2912 5a0f 4174  r....rh...).Z.At
+000061c0: 7472 6962 7574 655f 5461 626c 65da 0653  tribute_Table..S
+000061d0: 7562 5f49 44da 0b53 7562 5f4c 616b 655f  ub_ID..Sub_Lake_
+000061e0: 4944 da07 4c61 6b65 5f49 645a 0f6d 6178  ID..Lake_IdZ.max
+000061f0: 5f73 7562 6261 7369 6e5f 6964 5a0e 4e5f  _subbasin_idZ.N_
+00006200: 6e65 775f 6665 6174 7572 6573 5a09 6e65  new_featuresZ.ne
+00006210: 775f 6872 7569 645a 0e6e 6577 5f68 7275  w_hruidZ.new_hru
+00006220: 6964 5f6c 6973 745a 116f 6c64 5f6e 6577  id_listZ.old_new
+00006230: 6872 7569 645f 6c69 7374 7247 0000 005a  hruid_listrG...Z
+00006240: 0c73 7562 6964 5f73 665f 6f62 6a5a 116c  .subid_sf_objZ.l
+00006250: 616b 656c 616b 6569 645f 7366 5f6f 626a  akelakeid_sf_obj
+00006260: 5a11 5375 625f 4c61 6b65 6964 5f73 665f  Z.Sub_Lakeid_sf_
+00006270: 6f62 6a5a 0873 7562 6964 5f73 665a 0d6c  objZ.subid_sfZ.l
+00006280: 616b 656c 616b 6569 645f 7366 5a0d 5375  akelakeid_sfZ.Su
+00006290: 625f 4c61 6b65 6964 5f73 665a 0d6f 6c64  b_Lakeid_sfZ.old
+000062a0: 5f6e 6577 5f68 7275 6964 5a08 7461 725f  _new_hruidZ.tar_
+000062b0: 696e 666f 7224 0000 0072 2400 0000 7225  infor$...r$...r%
+000062c0: 0000 00da 1544 6574 6572 6d69 6e65 5f4c  .....Determine_L
+000062d0: 616b 655f 4852 555f 4964 2a06 0000 7390  ake_HRU_Id*...s.
+000062e0: 0000 0000 0d04 0104 0104 030e 0208 0104  ................
+000062f0: 0112 0112 0b14 010e 010e 010e 0402 010c  ................
+00006300: 0106 0104 010e 0106 0202 010c 0106 0104  ................
+00006310: 010e 0106 0202 010c 0106 0104 010e 0106  ................
+00006320: 040a 0102 030a 0104 010e 020a 0206 ff04  ................
+00006330: 030c 0110 0208 010e 030a 010e 0108 010a  ................
+00006340: 0302 0110 ff10 0814 010e 010e 010e 010a  ................
+00006350: 0104 010a 0108 0116 0104 0204 010a 010a  ................
+00006360: ff02 ff04 040e 010a 0104 0118 0118 0118  ................
+00006370: 011c 0272 e100 0000 6304 0000 0000 0000  ...r....c.......
+00006380: 0000 0000 0006 0000 0004 0000 0043 0000  .............C..
+00006390: 0073 8a00 0000 7c00 6a00 7c00 7c02 1900  .s....|.j.|.|...
+000063a0: 6401 6b03 1900 7d04 7401 7c04 8301 6401  d.k...}.t.|...d.
+000063b0: 6b04 722e 7c04 7c02 1900 6a02 6401 1900  k.r.|.|...j.d...
+000063c0: 7d05 6e58 7c01 6a00 7c01 7c02 1900 6401  }.nX|.j.|.|...d.
+000063d0: 6b03 1900 7d01 7c01 6a03 6402 6403 6404  k...}.|.j.d.d.d.
+000063e0: 8d02 7d01 7401 7c01 8301 6401 6b04 726a  ..}.t.|...d.k.rj
+000063f0: 7c01 7c02 1900 6a02 6401 1900 7d05 6e1c  |.|...j.d...}.n.
+00006400: 7c03 6a00 7c03 7c02 1900 6401 6b03 1900  |.j.|.|...d.k...
+00006410: 7c02 1900 6a02 6401 1900 7d05 7c05 5300  |...j.d...}.|.S.
+00006420: 2905 4e72 0100 0000 7232 0000 0046 7236  ).Nr....r2...Fr6
+00006430: 0000 0029 0472 1900 0000 7215 0000 0072  ...).r....r....r
+00006440: 1300 0000 7240 0000 0029 06da 1641 7474  ....r@...)...Att
+00006450: 7269 5f74 6162 6c65 5f4c 616b 655f 4852  ri_table_Lake_HR
+00006460: 555f 69da 0753 7562 496e 666f 5a06 436f  U_i..SubInfoZ.Co
+00006470: 6c5f 4e4d 5a09 696e 666f 5f64 6174 615a  l_NMZ.info_dataZ
+00006480: 0d69 6e66 6f5f 6c61 6b65 5f68 7275 5a0b  .info_lake_hruZ.
+00006490: 5570 6461 7465 7661 6c75 6572 2400 0000  Updatevaluer$...
+000064a0: 7224 0000 0072 2500 0000 da1f 5265 7472  r$...r%.....Retr
+000064b0: 756e 5f56 616c 6964 6174 655f 4174 7472  un_Validate_Attr
+000064c0: 6962 7574 655f 5661 6c75 65a5 0600 0073  ibute_Value....s
+000064d0: 2000 0000 0002 1202 0aff 0203 1002 1201   ...............
+000064e0: 0e01 0c01 1002 0a01 02ff 0401 02ff 0401  ................
+000064f0: 02ff 0404 72e4 0000 0063 0a00 0000 0000  ....r....c......
+00006500: 0000 0000 0000 1a00 0000 0700 0000 4300  ..............C.
+00006510: 0000 735e 0400 007c 007c 0119 0064 016b  ..s^...|.|...d.k
+00006520: 017d 0a7c 007c 0219 0064 016b 017c 007c  .}.|.|...d.k.|.|
+00006530: 0219 0064 026b 0340 007d 0b7c 007c 0319  ...d.k.@.}.|.|..
+00006540: 0064 016b 017c 007c 0319 0064 026b 0340  .d.k.|.|...d.k.@
+00006550: 007d 0c7c 007c 0419 0064 016b 017c 007c  .}.|.|...d.k.|.|
+00006560: 0419 0064 026b 0340 007d 0d7c 007c 0619  ...d.k.@.}.|.|..
+00006570: 0064 016b 017c 007c 0619 0064 026b 0340  .d.k.|.|...d.k.@
+00006580: 007d 0e7c 0a7c 0b42 007c 0c42 007c 0d42  .}.|.|.B.|.B.|.B
+00006590: 007c 0e42 007d 0f74 00a0 017c 006a 027c  .|.B.}.t...|.j.|
+000065a0: 0f64 0366 0219 006a 03a1 017d 107c 107c  .d.f...j...}.|.|
+000065b0: 1064 016b 0419 007d 1074 0464 0174 057c  .d.k...}.t.d.t.|
+000065c0: 1083 0183 0244 0090 025d f27d 117c 107c  .....D...].}.|.|
+000065d0: 1119 007d 127c 1264 016b 0272 c871 b07c  ...}.|.d.k.r.q.|
+000065e0: 006a 027c 0064 0319 007c 126b 0219 007d  .j.|.d...|.k...}
+000065f0: 137c 136a 0664 0464 0564 068d 027d 137c  .|.j.d.d.d...}.|
+00006600: 1364 0719 006a 0364 0119 007d 147c 006a  .d...j.d...}.|.j
+00006610: 027c 0064 0719 007c 146b 0219 007d 1574  .|.d...|.k...}.t
+00006620: 0464 0174 057c 1383 0183 0244 0090 025d  .d.t.|.....D...]
+00006630: 8a7d 167c 1364 0819 006a 037c 1619 007d  .}.|.d...j.|...}
+00006640: 177c 1364 0919 006a 037c 1619 007d 187c  .|.d...j.|...}.|
+00006650: 1864 016b 0490 0272 887c 137c 0319 006a  .d.k...r.|.|...j
+00006660: 0364 0119 0064 016b 0290 0172 7c74 077c  .d...d.k...r|t.|
+00006670: 137c 157c 037c 0883 047d 197c 197c 006a  .|.|.|...}.|.|.j
+00006680: 027c 0064 0819 007c 176b 027c 0366 023c  .|.d...|.k.|.f.<
+00006690: 006e 207c 137c 0319 006a 0364 0119 007c  .n |.|...j.d...|
+000066a0: 006a 027c 0064 0819 007c 176b 027c 0366  .j.|.d...|.k.|.f
+000066b0: 023c 007c 137c 0519 006a 0364 0119 0064  .<.|.|...j.d...d
+000066c0: 016b 0290 0172 d674 077c 137c 157c 057c  .k...r.t.|.|.|.|
+000066d0: 0083 047d 197c 197c 006a 027c 0064 0819  ...}.|.|.j.|.d..
+000066e0: 007c 176b 027c 0566 023c 006e 207c 137c  .|.k.|.f.<.n |.|
+000066f0: 0519 006a 0364 0119 007c 006a 027c 0064  ...j.d...|.j.|.d
+00006700: 0819 007c 176b 027c 0566 023c 007c 137c  ...|.k.|.f.<.|.|
+00006710: 0619 006a 0364 0119 0064 016b 0290 0272  ...j.d...d.k...r
+00006720: 3074 077c 137c 157c 067c 0083 047d 197c  0t.|.|.|.|...}.|
+00006730: 197c 006a 027c 0064 0819 007c 176b 027c  .|.j.|.d...|.k.|
+00006740: 0666 023c 006e 207c 137c 0619 006a 0364  .f.<.n |.|...j.d
+00006750: 0119 007c 006a 027c 0064 0819 007c 176b  ...|.j.|.d...|.k
+00006760: 027c 0666 023c 0074 0864 0283 017c 006a  .|.f.<.t.d...|.j
+00006770: 027c 0064 0819 007c 176b 027c 0266 023c  .|.d...|.k.|.f.<
+00006780: 0074 0864 0283 017c 006a 027c 0064 0819  .t.d...|.j.|.d..
+00006790: 007c 176b 027c 0466 023c 0090 0171 167c  .|.k.|.f.<...q.|
+000067a0: 137c 0319 006a 037c 1619 0064 016b 0290  .|...j.|...d.k..
+000067b0: 0272 c074 077c 137c 157c 037c 0883 047d  .r.t.|.|.|.|...}
+000067c0: 197c 197c 006a 027c 0064 0819 007c 176b  .|.|.j.|.d...|.k
+000067d0: 027c 0366 023c 007c 137c 0219 006a 037c  .|.f.<.|.|...j.|
+000067e0: 1619 0064 016b 0290 0272 f874 077c 137c  ...d.k...r.t.|.|
+000067f0: 157c 027c 0783 047d 197c 197c 006a 027c  .|.|...}.|.|.j.|
+00006800: 0064 0819 007c 176b 027c 0266 023c 007c  .d...|.k.|.f.<.|
+00006810: 137c 0419 006a 037c 1619 0064 016b 0290  .|...j.|...d.k..
+00006820: 0372 3074 077c 137c 157c 047c 0983 047d  .r0t.|.|.|.|...}
+00006830: 197c 197c 006a 027c 0064 0819 007c 176b  .|.|.j.|.d...|.k
+00006840: 027c 0466 023c 007c 137c 0519 006a 037c  .|.f.<.|.|...j.|
+00006850: 1619 0064 016b 0290 0372 6874 077c 137c  ...d.k...rht.|.|
+00006860: 157c 057c 0083 047d 197c 197c 006a 027c  .|.|...}.|.|.j.|
+00006870: 0064 0819 007c 176b 027c 0566 023c 007c  .d...|.k.|.f.<.|
+00006880: 137c 0619 006a 037c 1619 0064 016b 0290  .|...j.|...d.k..
+00006890: 0172 1674 077c 137c 157c 067c 0083 047d  .r.t.|.|.|.|...}
+000068a0: 197c 197c 006a 027c 0064 0819 007c 176b  .|.|.j.|.d...|.k
+000068b0: 027c 0666 023c 0090 0171 1671 b07c 006a  .|.f.<...q.q.|.j
+000068c0: 0967 0064 0aa2 0164 0b8d 017d 0074 0a6a  .g.d...d...}.t.j
+000068d0: 0b7c 007c 0764 0c7c 0264 0d8d 046a 0c64  .|.|.d.|.d...j.d
+000068e0: 0e64 0f8d 017d 0074 0a6a 0b7c 007c 0864  .d...}.t.j.|.|.d
+000068f0: 0c7c 0364 0d8d 046a 0c64 0e64 0f8d 017d  .|.d...j.d.d...}
+00006900: 0074 0a6a 0b7c 007c 0964 0c7c 0464 0d8d  .t.j.|.|.d.|.d..
+00006910: 046a 0c64 0e64 0f8d 017d 007c 0064 0319  .j.d.d...}.|.d..
+00006920: 00a0 0d74 0ea1 017c 007c 0219 00a0 0d74  ...t...|.|.....t
+00006930: 0ea1 0117 007c 007c 0319 00a0 0d74 0ea1  .....|.|.....t..
+00006940: 0117 007c 007c 0519 00a0 0d74 0ea1 0117  ...|.|.....t....
+00006950: 007c 0064 103c 0074 0aa0 0f7c 0064 1019  .|.d.<.t...|.d..
+00006960: 00a1 0164 0119 0064 1117 007c 0064 123c  ...d...d...|.d.<
+00006970: 007c 0053 0029 137a ab46 756e 6374 696f  .|.S.).z.Functio
+00006980: 6e20 746f 2064 6574 6572 6d69 6e65 206c  n to determine l
+00006990: 616e 6475 7365 2c73 6f69 6c2c 616e 6420  anduse,soil,and 
+000069a0: 7665 6720 616e 6420 6f74 6865 7220 7072  veg and other pr
+000069b0: 6f70 6572 7469 6573 2061 6674 6572 2075  operties after u
+000069c0: 6e69 6f6e 2061 6c6c 2070 6f6c 7967 6f6e  nion all polygon
+000069d0: 730a 2020 2020 2d2d 2d2d 2d2d 2d2d 2d2d  s.    ----------
+000069e0: 0a0a 2020 2020 4e6f 7465 730a 2020 2020  ..    Notes.    
+000069f0: 2d2d 2d2d 2d2d 2d0a 0a20 2020 2052 6574  -------..    Ret
+00006a00: 7572 6e73 3a0a 2020 2020 2d2d 2d2d 2d2d  urns:.    ------
+00006a10: 2d0a 2020 2020 2020 2020 4e6f 6e65 2c0a  -.        None,.
+00006a20: 2020 2020 7201 0000 0072 6600 0000 72dc      r....rf...r.
+00006a30: 0000 0072 3200 0000 4672 3600 0000 7206  ...r2...Fr6...r.
+00006a40: 0000 0072 ab00 0000 724c 0000 0029 035a  ...r....rL...).Z
+00006a50: 0a4c 414e 445f 5553 455f 435a 0556 4547  .LAND_USE_CZ.VEG
+00006a60: 5f43 5a09 534f 494c 5f50 524f 4672 1000  _CZ.SOIL_PROFr..
+00006a70: 0000 da05 696e 6e65 7229 0272 0c00 0000  ....inner).r....
+00006a80: 720b 0000 0054 7207 0000 00da 0766 6163  r....Tr......fac
+00006a90: 7465 7273 7228 0000 0072 5600 0000 2910  tersr(...rV...).
+00006aa0: 721a 0000 0072 2b00 0000 7219 0000 0072  r....r+...r....r
+00006ab0: 1300 0000 7229 0000 0072 1500 0000 7240  ....r)...r....r@
+00006ac0: 0000 0072 e400 0000 722d 0000 0072 1c00  ...r....r-...r..
+00006ad0: 0000 723f 0000 0072 1800 0000 7214 0000  ..r?...r....r...
+00006ae0: 0072 1600 0000 da03 7374 72da 0966 6163  .r......str..fac
+00006af0: 746f 7269 7a65 291a 5a0b 4174 7472 695f  torize).Z.Attri_
+00006b00: 7461 626c 6572 de00 0000 7246 0000 0072  tabler....rF...r
+00006b10: 4f00 0000 7250 0000 0072 5100 0000 7252  O...rP...rQ...rR
+00006b20: 0000 005a 114c 616e 6475 7365 5f69 6e66  ...Z.Landuse_inf
+00006b30: 6f5f 6461 7461 5a0e 536f 696c 5f69 6e66  o_dataZ.Soil_inf
+00006b40: 6f5f 6461 7461 5a0d 5665 675f 696e 666f  o_dataZ.Veg_info
+00006b50: 5f64 6174 615a 0969 6e76 616c 5f73 7562  _dataZ.inval_sub
+00006b60: 5a0d 696e 7661 6c5f 6c61 6e64 7573 655a  Z.inval_landuseZ
+00006b70: 0a69 6e76 616c 5f73 6f69 6c5a 0969 6e76  .inval_soilZ.inv
+00006b80: 616c 5f76 6567 5a08 696e 7661 6c5f 6f32  al_vegZ.inval_o2
+00006b90: 5a0a 696e 7661 6c5f 726f 7773 5a0c 4c61  Z.inval_rowsZ.La
+00006ba0: 6b65 5f48 5255 5f49 4453 7247 0000 005a  ke_HRU_IDSrG...Z
+00006bb0: 0c69 6c61 6b65 5f68 7275 5f69 6472 e200  .ilake_hru_idr..
+00006bc0: 0000 5a05 5375 6269 6472 e300 0000 725b  ..Z.Subidr....r[
+00006bd0: 0000 005a 0769 6872 755f 6964 5a07 6973  ...Z.ihru_idZ.is
+00006be0: 5f4c 616b 655a 0a56 616c 695f 5661 6c75  _LakeZ.Vali_Valu
+00006bf0: 6572 2400 0000 7224 0000 0072 2500 0000  er$...r$...r%...
+00006c00: da18 4465 7465 726d 696e 655f 4852 555f  ..Determine_HRU_
+00006c10: 4174 7472 6962 7574 6573 b906 0000 7330  Attributes....s0
+00006c20: 0100 0000 180c 010a 010a ff04 0218 0118  ................
+00006c30: 010a 010a ff04 0314 0116 010c 0314 0108  ................
+00006c40: 0108 0102 0204 010a ff04 0304 0104 ff06  ................
+00006c50: 030e 0112 0114 010e 010e 010a 0310 ff04  ................
+00006c60: 0302 0108 ff04 0502 fe04 010e ff04 060c  ................
+00006c70: fe04 010e ff02 0510 ff04 0302 0108 ff04  ................
+00006c80: 0502 fe04 010e ff04 060c fe04 010e ff02  ................
+00006c90: 0510 ff04 0302 0108 ff04 0502 fe04 010e  ................
+00006ca0: ff04 060c fe04 010e ff02 0506 ff0a 0102  ................
+00006cb0: ff02 0102 ff04 0306 ff0a 0102 ff02 0102  ................
+00006cc0: ff08 0510 ff04 0302 0108 ff04 0502 fe04  ................
+00006cd0: 010e ff02 0410 ff04 0302 0108 ff04 0502  ................
+00006ce0: fe04 010e ff02 0410 ff04 0302 0108 ff04  ................
+00006cf0: 0502 fe04 010e ff02 0410 ff04 0302 0108  ................
+00006d00: ff04 0502 fe04 010e ff02 0410 ff04 0302  ................
+00006d10: 0108 ff04 0502 fe04 010e ff08 0404 0106  ................
+00006d20: ff06 0208 0104 ff06 0102 ff06 0208 0104  ................
+00006d30: ff06 0102 ff06 0208 0104 ff06 0102 ff06  ................
+00006d40: 590c 010c ff02 020c fe02 040c fc02 ff06  Y...............
+00006d50: 081a 0172 e900 0000 6303 0000 0000 0000  ...r....c.......
+00006d60: 0000 0000 0041 0000 000c 0000 0043 0000  .....A.......C..
+00006d70: 0073 4e0b 0000 6401 7d03 6402 7d04 6403  .sN...d.}.d.}.d.
+00006d80: 7d05 6404 7d06 6405 7d07 6405 7c00 6a00  }.d.}.d.}.d.|.j.
+00006d90: 7601 7222 6406 7d07 7c00 6a01 6407 6408  v.r"d.}.|.j.d.d.
+00006da0: 8d01 7d08 6409 7c08 640a 3c00 6409 7c08  ..}.d.|.d.<.d.|.
+00006db0: 640b 3c00 7c08 6a02 6407 6407 640c 8d02  d.<.|.j.d.d.d...
+00006dc0: 0100 7403 a004 7c08 6403 1900 6a05 a101  ..t...|.d...j...
+00006dd0: 7d09 7c02 640d 1400 640d 1400 7c09 6b04  }.|.d...d...|.k.
+00006de0: 728c 7c09 640e 1b00 640e 1b00 640f 1800  r.|.d...d...d...
+00006df0: 7d02 6409 7c08 7c07 3c00 6409 7c00 7c07  }.d.|.|.<.d.|.|.
+00006e00: 3c00 7c00 6a06 7c00 7c05 1900 7c02 640d  <.|.j.|.|...|.d.
+00006e10: 1400 640d 1400 6b05 1900 a001 a100 7d0a  ..d...k.......}.
+00006e20: 7407 7c0a 7c08 8302 7d0a 7408 7c0a 6409  t.|.|...}.t.|.d.
+00006e30: 6410 8d02 7d0a 7c0a 6a09 6411 6701 6407  d...}.|.j.d.g.d.
+00006e40: 6412 8d02 7d0a 7c0a 6a06 7c0a 6413 1900  d...}.|.j.|.d...
+00006e50: 6414 6b03 1900 a001 a100 7d0a 7c0a 7c03  d.k.......}.|.|.
+00006e60: 1900 6a05 7d0b 7c0a 6a06 7c0a 6413 1900  ..j.}.|.j.|.d...
+00006e70: 640f 6b02 1900 6415 1900 6a05 7d0c 7403  d.k...d...j.}.t.
+00006e80: a00a 7c0c 7c0c 6416 6b04 1900 a101 7d0c  ..|.|.d.k.....}.
+00006e90: 7c00 6a06 7c00 6415 1900 a00b 7c0c a101  |.j.|.d.....|...
+00006ea0: 1900 a001 a100 7d0d 7c0d 7c03 1900 6a05  ......}.|.|...j.
+00006eb0: 7d0e 7c00 6a06 7c00 6401 1900 a00b 7c0b  }.|.j.|.d.....|.
+00006ec0: a101 0f00 7c00 7c07 1900 6416 6b04 4000  ....|.|...d.k.@.
+00006ed0: 1900 6a01 6407 6408 8d01 7d0f 7c0f 6a06  ..j.d.d...}.|.j.
+00006ee0: 7c0f 6415 1900 6416 6b01 1900 6401 1900  |.d...d.k...d...
+00006ef0: 6a05 7d10 7c00 6a01 6407 6408 8d01 7d11  j.}.|.j.d.d...}.
+00006f00: 7c11 6401 1900 a00b 7c10 a101 7d12 7c11  |.d.....|...}.|.
+00006f10: 6415 1900 640f 6b00 7d13 7403 a00c 7c12  d...d.k.}.t...|.
+00006f20: 7c13 a102 7d14 7c11 6a06 7c11 6401 1900  |...}.|.j.|.d...
+00006f30: a00b 7c10 a101 6401 6602 1900 0b00 7c11  ..|...d.f.....|.
+00006f40: 6a06 7c14 6415 6602 3c00 7c11 6a06 7c11  j.|.d.f.<.|.j.|.
+00006f50: 6401 1900 a00b 7c10 a101 6415 6602 1900  d.....|...d.f...
+00006f60: 6a05 7d15 7c01 6417 1900 6a05 7d16 7403  j.}.|.d...j.}.t.
+00006f70: a00d 7c16 7c0c a102 7d14 7c16 7403 a00e  ..|.|...}.|.t...
+00006f80: 7c14 a101 1900 a001 a100 7d17 7c11 6a06  |.........}.|.j.
+00006f90: 7c11 6415 1900 a00b 7c17 a101 7c11 6415  |.d.....|...|.d.
+00006fa0: 1900 a00b 7c15 a101 4200 1900 a001 a100  ....|...B.......
+00006fb0: 7d18 7c00 6a06 7c00 6413 1900 6414 6b02  }.|.j.|.d...d.k.
+00006fc0: 1900 6401 1900 6a05 7d19 7403 a00a 7c19  ..d...j.}.t...|.
+00006fd0: 7c19 6416 6b04 1900 a101 7d19 7c00 6a06  |.d.k.....}.|.j.
+00006fe0: 7c00 6413 1900 6414 6b02 1900 6415 1900  |.d...d.k...d...
+00006ff0: 6a05 7d1a 7403 a00a 7c1a 7c1a 6416 6b04  j.}.t...|.|.d.k.
+00007000: 1900 a101 7d1a 7403 a00a 7c0b a101 7d1b  ....}.t...|...}.
+00007010: 7c00 6401 6402 6702 1900 a00f 6418 a101  |.d.d.g.....d...
+00007020: 6a05 7d1c 7c0a 6404 1900 6a05 7d1d 7403  j.}.|.d...j.}.t.
+00007030: a00a 7c1d a101 7d1d 7c08 6a06 7c08 6413  ..|...}.|.j.|.d.
+00007040: 1900 6414 6b02 1900 6401 1900 6a05 7c08  ..d.k...d...j.|.
+00007050: 6a06 7c08 6413 1900 6414 6b02 640a 6602  j.|.d...d.k.d.f.
+00007060: 3c00 7c18 a010 6415 6701 a101 6403 1900  <.|...d.g...d...
+00007070: a011 7404 a101 7c18 6403 1900 6b02 7d1e  ..t...|.d...k.}.
+00007080: 7c18 7c1e 1900 7d1f 7c1f 6a09 6411 6403  |.|...}.|.j.d.d.
+00007090: 6702 6407 6407 6702 6412 8d02 7d1f 7c00  g.d.d.g.d...}.|.
+000070a0: 7c00 6402 1900 6416 6b00 1900 6a01 6407  |.d...d.k...j.d.
+000070b0: 6408 8d01 7d20 7412 6416 7413 7c20 8301  d...} t.d.t.| ..
+000070c0: 8302 4400 5d50 7d21 7c20 6403 1900 6a05  ..D.]P}!| d...j.
+000070d0: 7c21 1900 7c02 640d 1400 640d 1400 6b01  |!..|.d...d...k.
+000070e0: 9003 724e 7c20 6401 1900 6a05 7c21 1900  ..rN| d...j.|!..
+000070f0: 7d22 7414 7c1c 7c22 8302 7d23 7415 7c22  }"t.|.|"..}#t.|"
+00007100: 7c00 7c08 640f 7c00 7c23 6409 6419 8d07  |.|.d.|.|#d.d...
+00007110: 7d08 9003 714e 7412 6416 7413 7c1f 8301  }...qNt.d.t.|...
+00007120: 8302 4400 9001 5d08 7d21 7403 a00a 7c08  ..D...].}!t...|.
+00007130: 6a06 7c08 640a 1900 6416 6b04 1900 7c03  j.|.d...d.k...|.
+00007140: 1900 6a05 a101 7d24 7c1f 6415 1900 6a05  ..j...}$|.d...j.
+00007150: 7c21 1900 7d25 7c11 7c11 6415 1900 7c25  |!..}%|.|.d...|%
+00007160: 6b02 1900 7d26 7403 a00a 7c26 6404 1900  k...}&t...|&d...
+00007170: 6a05 a101 7d27 6700 7d28 7412 6416 7413  j...}'g.}(t.d.t.
+00007180: 7c27 8301 8302 4400 5d82 7d29 7c27 7c29  |'....D.].})|'|)
+00007190: 1900 7d2a 7c26 6a06 7c26 6404 1900 7c2a  ..}*|&j.|&d...|*
+000071a0: 6b02 1900 a001 a100 7d2b 7c2b 6a09 6403  k.......}+|+j.d.
+000071b0: 6701 641a 6412 8d02 7d2b 7c2b 6401 1900  g.d.d...}+|+d...
+000071c0: 6a05 6416 1900 7d22 7414 7c1c 7c22 8302  j.d...}"t.|.|"..
+000071d0: 7d23 7c23 7c23 6416 6b04 1900 7d23 7403  }#|#|#d.k...}#t.
+000071e0: a00d 7c23 7c24 a102 7d14 7c23 7403 a00e  ..|#|$..}.|#t...
+000071f0: 7c14 a101 1900 7d2c 6700 7c28 a201 7c2c  |.....},g.|(..|,
+00007200: a016 a100 a201 7d28 9004 7112 7403 a017  ......}(..q.t...
+00007210: 7c28 a101 7d28 7415 7c22 7c11 7c08 640f  |(..}(t.|"|.|.d.
+00007220: 7c11 7c28 6414 6419 8d07 7d08 9003 71ae  |.|(d.d...}...q.
+00007230: 7412 6416 7413 7c1d 8301 8302 4400 9005  t.d.t.|.....D...
+00007240: 5df0 7d2d 7c1d 7c2d 1900 7d2e 7c0a 6a06  ].}-|.|-..}.|.j.
+00007250: 7c0a 6404 1900 7c2e 6b02 1900 a001 a100  |.d...|.k.......
+00007260: 7d2f 7c2f 6a09 641b 6701 6407 6412 8d02  }/|/j.d.g.d.d...
+00007270: 7d2f 6416 7d30 6700 7d28 640f 7d31 7412  }/d.}0g.}(d.}1t.
+00007280: 6416 7413 7c2f 8301 8302 4400 9005 5d9e  d.t.|/....D...].
+00007290: 7d32 7c2f 6401 1900 6a05 7c32 1900 7d22  }2|/d...j.|2..}"
+000072a0: 7c2f 6415 1900 6a05 7c32 1900 7d33 7c28  |/d...j.|2..}3|(
+000072b0: a018 7c22 a101 0100 7403 a00a 7c08 6a06  ..|"....t...|.j.
+000072c0: 7c08 640a 1900 6416 6b04 1900 7c03 1900  |.d...d.k...|...
+000072d0: 6a05 a101 7d24 7c30 7c2f 641c 1900 6a05  j...}$|0|/d...j.
+000072e0: 7c32 1900 1700 7d30 7c32 7413 7c2f 8301  |2....}0|2t.|/..
+000072f0: 640f 1800 6b03 9005 72a6 7c2f 6415 1900  d...k...r.|/d...
+00007300: 6a05 7c32 1900 7c2f 6415 1900 6a05 7c32  j.|2..|/d...j.|2
+00007310: 640f 1700 1900 6b02 7d34 6e04 641a 7d34  d.....k.}4n.d.}4
+00007320: 7c2f 7c07 1900 6a05 7c32 1900 6416 6b01  |/|...j.|2..d.k.
+00007330: 7d35 7c32 7413 7c2f 8301 6414 1800 6b01  }5|2t.|/..d...k.
+00007340: 9005 72fe 7c2f 641c 1900 6a05 7c32 640f  ..r.|/d...j.|2d.
+00007350: 1700 1900 641d 6b00 9005 72ec 6407 7d36  ....d.k...r.d.}6
+00007360: 6e10 7c30 7c02 640d 1400 640d 1400 6b00  n.|0|.d...d...k.
+00007370: 7d36 6e10 7c30 7c02 640d 1400 640d 1400  }6n.|0|.d...d...
+00007380: 6b00 7d36 7c30 641d 6b00 7d37 7c32 640f  k.}6|0d.k.}7|2d.
+00007390: 6b05 9006 7288 7c32 7413 7c2f 8301 6414  k...r.|2t.|/..d.
+000073a0: 1800 6b01 9006 7288 7c2f 6415 1900 6a05  ..k...r.|/d...j.
+000073b0: 7c32 640f 1800 1900 7c2f 6415 1900 6a05  |2d.....|/d...j.
+000073c0: 7c32 1900 6b03 7d38 7c2f 6415 1900 6a05  |2..k.}8|/d...j.
+000073d0: 7c32 1900 7c2f 6415 1900 6a05 7c32 640f  |2..|/d...j.|2d.
+000073e0: 1700 1900 6b03 7d39 7c2f 6415 1900 6a05  ....k.}9|/d...j.
+000073f0: 7c32 1900 6416 6b01 7d3a 641a 7d37 7c32  |2..d.k.}:d.}7|2
+00007400: 6416 6b02 9006 72de 7c32 7413 7c2f 8301  d.k...r.|2t.|/..
+00007410: 640f 1800 6b00 9006 72de 6407 7d38 7c2f  d...k...r.d.}8|/
+00007420: 6415 1900 6a05 7c32 1900 7c2f 6415 1900  d...j.|2..|/d...
+00007430: 6a05 7c32 640f 1700 1900 6b03 7d39 7c2f  j.|2d.....k.}9|/
+00007440: 6415 1900 6a05 7c32 1900 6416 6b01 7d3a  d...j.|2..d.k.}:
+00007450: 641a 7d37 7c32 7413 7c2f 8301 6414 1800  d.}7|2t.|/..d...
+00007460: 6b02 9008 7218 7c2f 6415 1900 6a05 7c32  k...r.|/d...j.|2
+00007470: 1900 6416 6b04 9008 7218 6407 7d38 7c2f  ..d.k...r.d.}8|/
+00007480: 6415 1900 6a05 7c32 1900 7c2f 6415 1900  d...j.|2..|/d...
+00007490: 6a05 7c32 640f 1700 1900 6b03 7d39 7c2f  j.|2d.....k.}9|/
+000074a0: 6415 1900 6a05 7c32 1900 6416 6b04 7d3a  d...j.|2..d.k.}:
+000074b0: 7c2f 6402 1900 6a05 7c32 1900 7d3b 641a  |/d...j.|2..};d.
+000074c0: 7d37 7c37 9008 7218 7c39 9008 7218 7c2f  }7|7..r.|9..r.|/
+000074d0: 6415 1900 6a05 7c32 1900 7c00 6a06 7c00  d...j.|2..|.j.|.
+000074e0: 6401 1900 7c3b 6b02 6415 6602 3c00 7c2f  d...|;k.d.f.<.|/
+000074f0: 6413 1900 6a05 7c32 1900 7c00 6a06 7c00  d...j.|2..|.j.|.
+00007500: 6401 1900 7c3b 6b02 6413 6602 3c00 7c2f  d...|;k.d.f.<.|/
+00007510: 641e 1900 6a05 7c32 1900 7c00 6a06 7c00  d...j.|2..|.j.|.
+00007520: 6401 1900 7c3b 6b02 641e 6602 3c00 7c2f  d...|;k.d.f.<.|/
+00007530: 641f 1900 6a05 7c32 1900 7c00 6a06 7c00  d...j.|2..|.j.|.
+00007540: 6401 1900 7c3b 6b02 641f 6602 3c00 7c2f  d...|;k.d.f.<.|/
+00007550: 6420 1900 6a05 7c32 1900 7c00 6a06 7c00  d ..j.|2..|.j.|.
+00007560: 6401 1900 7c3b 6b02 6420 6602 3c00 7c2f  d...|;k.d f.<.|/
+00007570: 6421 1900 6a05 7c32 1900 7c00 6a06 7c00  d!..j.|2..|.j.|.
+00007580: 6401 1900 7c3b 6b02 6421 6602 3c00 7c32  d...|;k.d!f.<.|2
+00007590: 7413 7c2f 8301 640f 1800 6b02 9008 7236  t.|/..d...k...r6
+000075a0: 6407 7d38 641a 7d39 6407 7d3a 7c32 7413  d.}8d.}9d.}:|2t.
+000075b0: 7c2f 8301 640f 1800 6b02 9009 7260 6416  |/..d...k...r`d.
+000075c0: 7d30 7403 a017 7c28 a101 7d2c 7c33 6416  }0t...|(..},|3d.
+000075d0: 6b04 9008 72b4 7c00 6a06 7c00 6415 1900  k...r.|.j.|.d...
+000075e0: 7c33 6b02 1900 a001 a100 7d3c 7c3c 6401  |3k.......}<|<d.
+000075f0: 6402 6702 1900 a00f 6418 a101 6a05 7d3d  d.g.....d...j.}=
+00007600: 7414 7c3d 7c22 8302 7d3e 7403 a00a 7403  t.|=|"..}>t...t.
+00007610: a019 7c2c 7c3e 6702 a101 a101 7d2c 7c2c  ..|,|>g.....},|,
+00007620: 7c2c 6416 6b04 1900 7d2c 7414 7c1c 7c22  |,d.k...},t.|.|"
+00007630: 8302 7d23 7c23 7c23 6416 6b04 1900 7d23  ..}#|#|#d.k...}#
+00007640: 7403 a00d 7c23 7c0b a102 7d12 7c23 7403  t...|#|...}.|#t.
+00007650: a00e 7c12 a101 1900 7d3f 7403 a00a 7403  ..|.....}?t...t.
+00007660: a019 7c2c 7c3f 6702 a101 a101 7d2c 7c2c  ..|,|?g.....},|,
+00007670: 7c2c 6416 6b04 1900 7d2c 7403 a00d 7c2c  |,d.k...},t...|,
+00007680: 7c24 a102 7d14 7c2c 7403 a00e 7c14 a101  |$..}.|,t...|...
+00007690: 1900 7d2c 7403 a00d 7c2c 7c19 a102 7d40  ..},t...|,|...}@
+000076a0: 7c2c 7403 a00e 7c40 a101 1900 7d2c 7415  |,t...|@....},t.
+000076b0: 7c22 7c00 7c08 640f 7c2c 7c0a 6422 7c31  |"|.|.d.|,|.d"|1
+000076c0: 6423 8d08 7d08 6700 7d28 7c31 640f 1700  d#..}.g.}(|1d...
+000076d0: 7d31 9005 7116 7c38 9009 7286 7c39 9009  }1..q.|8..r.|9..
+000076e0: 7286 7c3a 9009 7286 7c35 9009 7286 7c37  r.|:..r.|5..r.|7
+000076f0: 9009 7286 9005 7116 9005 7116 7c34 9009  ..r...q...q.|4..
+00007700: 72a0 7c35 9009 72a0 7c36 9009 72a0 9005  r.|5..r.|6..r...
+00007710: 7116 9005 7116 6416 7d30 7403 a017 7c28  q...q.d.}0t...|(
+00007720: a101 7d2c 7c33 6416 6b04 900a 720c 7c00  ..},|3d.k...r.|.
+00007730: 6a06 7c00 6415 1900 7c33 6b02 1900 a001  j.|.d...|3k.....
+00007740: a100 7d3c 7c3c 6401 6402 6702 1900 a00f  ..}<|<d.d.g.....
+00007750: 6418 a101 6a05 7d3d 7414 7c3d 7c22 8302  d...j.}=t.|=|"..
+00007760: 7d3e 7403 a00a 7403 a019 7c2c 7c3e 6702  }>t...t...|,|>g.
+00007770: a101 a101 7d2c 7c2c 7c2c 6416 6b04 1900  ....},|,|,d.k...
+00007780: 7d2c 7414 7c1c 7c22 8302 7d23 7c23 7c23  },t.|.|"..}#|#|#
+00007790: 6416 6b04 1900 7d23 7403 a00d 7c23 7c0b  d.k...}#t...|#|.
+000077a0: a102 7d12 7c23 7403 a00e 7c12 a101 1900  ..}.|#t...|.....
+000077b0: 7d3f 7403 a00a 7403 a019 7c2c 7c3f 6702  }?t...t...|,|?g.
+000077c0: a101 a101 7d2c 7c2c 7c2c 6416 6b04 1900  ....},|,|,d.k...
+000077d0: 7d2c 7403 a00d 7c2c 7c24 a102 7d14 7c2c  },t...|,|$..}.|,
+000077e0: 7403 a00e 7c14 a101 1900 7d2c 7403 a00d  t...|.....},t...
+000077f0: 7c2c 7c19 a102 7d40 7c2c 7403 a00e 7c40  |,|...}@|,t...|@
+00007800: a101 1900 7d2c 7415 7c22 7c00 7c08 640f  ....},t.|"|.|.d.
+00007810: 7c2c 7c0a 6422 7c31 6423 8d08 7d08 6700  |,|.d"|1d#..}.g.
+00007820: 7d28 7c31 640f 1700 7d31 9005 7116 9004  }(|1d...}1..q...
+00007830: 71c8 6416 7c08 6a06 7c08 6415 1900 6416  q.d.|.j.|.d...d.
+00007840: 6b01 6415 6602 3c00 6416 7c08 6a06 7c08  k.d.f.<.d.|.j.|.
+00007850: 6415 1900 6416 6b01 6413 6602 3c00 6416  d...d.k.d.f.<.d.
+00007860: 7c08 6a06 7c08 6415 1900 6416 6b01 641e  |.j.|.d...d.k.d.
+00007870: 6602 3c00 6416 7c08 6a06 7c08 6415 1900  f.<.d.|.j.|.d...
+00007880: 6416 6b01 641f 6602 3c00 6416 7c08 6a06  d.k.d.f.<.d.|.j.
+00007890: 7c08 6415 1900 6416 6b01 6420 6602 3c00  |.d...d.k.d f.<.
+000078a0: 6416 7c08 6a06 7c08 6415 1900 6416 6b01  d.|.j.|.d...d.k.
+000078b0: 6421 6602 3c00 7c08 7c1b 7c0c 7c1a 7c17  d!f.<.|.|.|.|.|.
+000078c0: 6605 5300 2924 7aac 4d6f 6469 6679 2061  f.S.)$z.Modify a
+000078d0: 7474 7269 6275 7465 2074 6162 6c65 206d  ttribute table m
+000078e0: 6170 6f6c 646e 6577 5f69 6e66 6f2c 2063  apoldnew_info, c
+000078f0: 7265 6174 6520 6e65 7720 7375 6220 6964  reate new sub id
+00007900: 2066 6f72 2073 7562 6261 7369 6e20 6e65   for subbasin ne
+00007910: 6564 7320 746f 2062 6520 6d65 7267 6564  eds to be merged
+00007920: 2e0a 2020 2020 2d2d 2d2d 2d2d 2d2d 2d2d  ..    ----------
+00007930: 0a0a 2020 2020 4e6f 7465 730a 2020 2020  ..    Notes.    
+00007940: 2d2d 2d2d 2d2d 2d0a 0a20 2020 2052 6574  -------..    Ret
+00007950: 7572 6e73 3a0a 2020 2020 2d2d 2d2d 2d2d  urns:.    ------
+00007960: 2d0a 2020 2020 2020 2020 4e6f 6e65 2c0a  -.        None,.
+00007970: 2020 2020 7206 0000 0072 0d00 0000 726c      r....r....rl
+00007980: 0000 0072 6300 0000 7278 0000 0072 7900  ...rc...rx...ry.
+00007990: 0000 5472 0700 0000 7266 0000 0072 7b00  ..Tr....rf...r{.
+000079a0: 0000 7288 0000 00a9 0272 1c00 0000 da07  ..r......r......
+000079b0: 696e 706c 6163 6572 6f00 0000 72c0 0000  inplacero...r...
+000079c0: 0072 2800 0000 2901 72b4 0000 0072 6400  .r(...).r....rd.
+000079d0: 0000 726d 0000 0072 6100 0000 7262 0000  ..rm...ra...rb..
+000079e0: 0072 7c00 0000 7201 0000 0072 da00 0000  .r|...r....r....
+000079f0: 7260 0000 0029 0772 4800 0000 72a4 0000  r`...).rH...r...
+00007a00: 0072 9000 0000 72a5 0000 0072 a700 0000  .r....r....r....
+00007a10: 72a6 0000 0072 6100 0000 4672 6500 0000  r....ra...Fre...
+00007a20: 727a 0000 0069 8096 9800 729c 0000 0072  rz...i....r....r
+00007a30: 9e00 0000 729d 0000 0072 9f00 0000 e903  ....r....r......
+00007a40: 0000 00a9 0872 4800 0000 72a4 0000 0072  .....rH...r....r
+00007a50: 9000 0000 72a5 0000 0072 a600 0000 72a7  ....r....r....r.
+00007a60: 0000 0072 6100 0000 72a8 0000 0029 1a72  ...ra...r....).r
+00007a70: 1100 0000 7214 0000 00da 0b72 6573 6574  ....r......reset
+00007a80: 5f69 6e64 6578 721a 0000 0072 6700 0000  _indexr....rg...
+00007a90: 7213 0000 0072 1900 0000 da3a 7570 6461  r....r.....:upda
+00007aa0: 7465 5f74 6865 5f73 656c 6563 7465 645f  te_the_selected_
+00007ab0: 7269 7665 725f 746f 5f63 6f6e 6e65 6374  river_to_connect
+00007ac0: 5f75 7073 7562 5f77 6974 685f 6c61 7267  _upsub_with_larg
+00007ad0: 6573 745f 6461 72b9 0000 0072 4000 0000  est_dar....r@...
+00007ae0: 722b 0000 0072 1200 0000 7242 0000 0072  r+...r....rB...r
+00007af0: 2e00 0000 72a3 0000 0072 1600 0000 723d  ....r....r....r=
+00007b00: 0000 00da 0974 7261 6e73 666f 726d 7229  .....transformr)
+00007b10: 0000 0072 1500 0000 7217 0000 0072 aa00  ...r....r....r..
+00007b20: 0000 72d4 0000 00da 0761 7361 7272 6179  ..r......asarray
+00007b30: 724d 0000 0072 1b00 0000 2941 5a0d 6669  rM...r....)AZ.fi
+00007b40: 6e61 6c72 6976 5f69 6e66 6f5a 0e43 6f6e  nalriv_infoZ.Con
+00007b50: 6e5f 4c61 6b65 735f 706c 79da 0841 7265  n_Lakes_ply..Are
+00007b60: 615f 4d69 6e72 a900 0000 5a0a 646f 776e  a_Minr....Z.down
+00007b70: 5f63 6f6c 6e6d 5a08 4441 5f63 6f6c 6e6d  _colnmZ.DA_colnm
+00007b80: 5a0b 5365 6749 445f 636f 6c6e 6d72 9300  Z.SegID_colnmr..
+00007b90: 0000 7290 0000 005a 066d 6178 5f64 61da  ..r....Z.max_da.
+00007ba0: 0c53 656c 6563 7465 645f 7269 765a 0a53  .Selected_rivZ.S
+00007bb0: 7562 6964 5f6d 6169 6e5a 1643 6f6e 6e65  ubid_mainZ.Conne
+00007bc0: 6374 6564 5f4c 616b 655f 4d61 696e 7269  cted_Lake_Mainri
+00007bd0: 765a 0d4c 616b 6563 6f76 6572 5f72 6976  vZ.Lakecover_riv
+00007be0: 5a0b 5375 6269 645f 6c61 6b65 735a 1d75  Z.Subid_lakesZ.u
+00007bf0: 6e73 656c 6563 7465 645f 6761 7567 6573  nselected_gauges
+00007c00: 5f73 7562 6964 735f 696e 666f 5a18 756e  _subids_infoZ.un
+00007c10: 7365 6c65 6374 6564 5f67 6175 6765 735f  selected_gauges_
+00007c20: 7375 6269 6473 5a11 6669 6e61 6c72 6976  subidsZ.finalriv
+00007c30: 5f69 6e66 6f5f 6e63 6c72 4900 0000 724a  _info_nclrI...rJ
+00007c40: 0000 0072 2300 0000 5a12 6661 6b65 5f6f  ...r#...Z.fake_o
+00007c50: 6273 5f68 7961 6c6b 6569 6473 5a10 416c  bs_hyalkeidsZ.Al
+00007c60: 6c5f 436f 6e6e 5f4c 616b 6569 6473 5a15  l_Conn_LakeidsZ.
+00007c70: 436f 6e6e 5f54 6f5f 4e6f 6e43 6f6e 6c61  Conn_To_NonConla
+00007c80: 6b65 6964 735a 1743 6f6e 6e5f 546f 5f4e  keidsZ.Conn_To_N
+00007c90: 6f6e 436f 6e6c 616b 655f 696e 666f 5a16  onConlake_infoZ.
+00007ca0: 4f6c 645f 4e6f 6e5f 436f 6e6e 6563 745f  Old_Non_Connect_
+00007cb0: 5375 6249 6473 5a17 4f6c 645f 4e6f 6e5f  SubIdsZ.Old_Non_
+00007cc0: 436f 6e6e 6563 745f 4c61 6b65 4964 73da  Connect_LakeIds.
+00007cd0: 1053 656c 6563 7465 645f 7269 765f 6964  .Selected_riv_id
+00007ce0: 7372 6a00 0000 da07 5365 675f 4944 5372  srj.....Seg_IDSr
+00007cf0: 5c00 0000 5a1e 436f 6e6e 5f54 6f5f 4e6f  \...Z.Conn_To_No
+00007d00: 6e43 6f6e 6c61 6b65 5f69 6e66 6f5f 6f75  nConlake_info_ou
+00007d10: 746c 6574 5a13 616c 6c5f 6f75 746c 6574  tletZ.all_outlet
+00007d20: 5f73 7562 5f69 6e66 6f72 4700 0000 da06  _sub_inforG.....
+00007d30: 7473 7562 6964 5a0d 416c 6c5f 7570 5f73  tsubidZ.All_up_s
+00007d40: 7562 6964 735a 0f70 726f 6365 7373 6564  ubidsZ.processed
+00007d50: 5f73 7562 6964 5a0c 435f 545f 4e5f 4c61  _subidZ.C_T_N_La
+00007d60: 6b65 6964 5a0d 4c61 6b65 5f43 6174 5f69  keidZ.Lake_Cat_i
+00007d70: 6e66 6f5a 0b52 6976 5f53 6567 5f49 4453  nfoZ.Riv_Seg_IDS
+00007d80: da0c 6d6f 6469 6679 7375 6269 6473 725b  ..modifysubidsr[
+00007d90: 0000 005a 0869 7269 765f 7365 675a 114c  ...Z.iriv_segZ.L
+00007da0: 616b 655f 4361 745f 7365 675f 696e 666f  ake_Cat_seg_info
+00007db0: da0b 7365 675f 7375 625f 6964 7372 c300  ..seg_sub_idsr..
+00007dc0: 0000 da08 695f 7365 675f 6964 da0a 695f  ....i_seg_id..i_
+00007dd0: 7365 675f 696e 666f 5a08 7375 6d5f 6172  seg_infoZ.sum_ar
+00007de0: 6561 72a8 0000 00da 0669 6f72 6465 725a  ear......iorderZ
+00007df0: 0d69 6f72 6465 725f 4c61 6b65 6964 5a08  .iorder_LakeidZ.
+00007e00: 636f 6e5f 6c61 6b65 5a09 636f 6e5f 6761  con_lakeZ.con_ga
+00007e10: 7567 655a 0863 6f6e 5f61 7265 615a 0d63  ugeZ.con_areaZ.c
+00007e20: 6f6e 5f61 7265 615f 6c61 6b65 5a0b 636f  on_area_lakeZ.co
+00007e30: 6e5f 6c61 6b65 5f75 705a 0d63 6f6e 5f6c  n_lake_upZ.con_l
+00007e40: 616b 655f 646f 776e 5a07 6973 5f6c 616b  ake_downZ.is_lak
+00007e50: 6572 d700 0000 5a13 7375 6269 645f 6375  er....Z.subid_cu
+00007e60: 725f 6c61 6b65 5f69 6e66 6f5a 1172 6f75  r_lake_infoZ.rou
+00007e70: 7469 6e67 5f69 6e66 6f5f 6c61 6b65 5a0f  ting_info_lakeZ.
+00007e80: 5570 7374 7265 616d 4c61 6b65 6964 735a  UpstreamLakeidsZ
+00007e90: 1541 6c6c 5f75 705f 7375 6269 6473 5f6e  .All_up_subids_n
+00007ea0: 6f5f 6d61 696e 5a10 6d61 736b 5f6f 6c64  o_mainZ.mask_old
+00007eb0: 5f6e 6f6e 4c61 6b65 7224 0000 0072 2400  _nonLaker$...r$.
+00007ec0: 0000 7225 0000 00da 4743 6861 6e67 655f  ..r%....GChange_
+00007ed0: 4174 7472 6962 7574 655f 5661 6c75 6573  Attribute_Values
+00007ee0: 5f46 6f72 5f43 6174 6368 6d65 6e74 735f  _For_Catchments_
+00007ef0: 4e65 6564 5f54 6f5f 4265 5f4d 6572 6765  Need_To_Be_Merge
+00007f00: 645f 4279 5f49 6e63 7265 6173 655f 4441  d_By_Increase_DA
+00007f10: b807 0000 73aa 0200 0000 0d04 0104 0104  ....s...........
+00007f20: 0104 0204 010a 0104 070c 0108 0108 010e  ................
+00007f30: 0110 0310 0110 0108 0108 0304 0112 ff08  ................
+00007f40: 0402 0104 ff04 040c 0104 0106 ff06 0316  ................
+00007f50: 010a 0310 0102 ff06 0304 010a ff04 0304  ................
+00007f60: 010c ff08 030a 0504 010e 010a ff02 ff04  ................
+00007f70: 0302 fd06 0404 010a ff02 0102 ff06 030c  ................
+00007f80: 020e 010c 010c 020c 0102 ff02 0102 ff04  ................
+00007f90: ff0e 030c 0102 ff02 0102 ff08 050a 010c  ................
+00007fa0: 0112 0104 010c 010c ff02 ff08 0610 0102  ................
+00007fb0: ff06 0304 010a ff04 0310 0102 ff06 0304  ................
+00007fc0: 010a ff04 0504 0102 ff04 0314 010a 010a  ................
+00007fd0: 0304 010a ff02 0202 fe18 0604 0104 ff02  ................
+00007fe0: 0102 ff04 0102 ff02 0206 fe02 ff02 0508  ................
+00007ff0: 0204 010c ff06 0510 0102 ff06 0312 011c  ................
+00008000: 010e 010a 0202 0102 0102 0102 0102 0102  ................
+00008010: 0102 0102 f90a 0b14 0104 0116 ff04 040e  ................
+00008020: 0108 0102 ff06 0210 0104 0112 0208 0104  ................
+00008030: 010a ff08 0304 0106 ff06 020e 020a 010c  ................
+00008040: 020c 010e 0202 0102 ff02 0206 fe08 050a  ................
+00008050: 0202 0102 0102 0102 0102 0102 0102 0102  ................
+00008060: f90a 0b14 0208 0116 0210 0104 0104 0104  ................
+00008070: 0114 010e 010e 010a 0104 010a 0102 ff04  ................
+00008080: 0102 ff04 ff04 0412 0412 0122 0204 0212  ..........."....
+00008090: 0312 0118 0106 0212 0210 0208 021c 020a  ................
+000080a0: 0102 ff04 010c ff04 0320 0212 0304 021c  ......... ......
+000080b0: 0204 0220 0212 0304 0226 0204 0220 0212  ... .....&... ..
+000080c0: 050e 0304 020c 020c ff04 010e ff02 030c  ................
+000080d0: ff04 010e ff02 030c ff04 010e ff02 030c  ................
+000080e0: ff04 010e ff02 030c ff04 010e ff02 030c  ................
+000080f0: ff04 010e ff02 0312 0104 0104 0104 0612  ................
+00008100: 0104 010a 020a 0104 010a ff08 040c 0102  ................
+00008110: ff04 ff02 050a 0104 010c ff04 030c 030a  ................
+00008120: 010c 0104 0104 ff04 030e 0204 010c ff04  ................
+00008130: 030c 010c 010e 020c 010e 0202 0102 0102  ................
+00008140: 0102 0102 0102 0102 0102 0102 f806 0b04  ................
+00008150: 010c 021e 0108 0212 0108 0304 010a 020a  ................
+00008160: 0104 010a ff08 040c 0102 ff04 ff02 050a  ................
+00008170: 0104 010c ff04 030c 020a 010c 0104 0104  ................
+00008180: ff04 030e 0204 010c ff04 030c 010c 010e  ................
+00008190: 020c 010e 0202 0102 0102 0102 0102 0102  ................
+000081a0: 0102 0102 0102 f806 0a04 0110 0216 0116  ................
+000081b0: 0116 0116 0116 0116 0302 0102 0102 0102  ................
+000081c0: 0102 fb72 fc00 0000 6302 0000 0000 0000  ...r....c.......
+000081d0: 0000 0000 000f 0000 0006 0000 0043 0000  .............C..
+000081e0: 0073 9a01 0000 7400 a001 7c00 6401 1900  .s....t...|.d...
+000081f0: 6a02 a101 7d02 7400 a001 7c00 6402 1900  j...}.t...|.d...
+00008200: 6a02 a101 7d03 7c03 7c03 6403 6b04 1900  j...}.|.|.d.k...
+00008210: 7d03 7400 a003 7c01 6404 1900 6405 6b02  }.t...|.d...d.k.
+00008220: 7c01 6402 1900 a004 7c03 a101 0f00 a102  |.d.....|.......
+00008230: 7d04 7c01 6406 1900 6403 6b04 7d05 7c01  }.|.d...d.k.}.|.
+00008240: 7400 a005 7c04 7c05 a102 1900 6a06 6407  t...|.|.....j.d.
+00008250: 6408 8d01 7d06 7c06 7c06 6401 1900 a004  d...}.|.|.d.....
+00008260: 7c02 a101 0f00 1900 7d06 7400 a001 7c06  |.......}.t...|.
+00008270: 6401 1900 6a02 a101 7d07 7c07 4400 5dea  d...j...}.|.D.].
+00008280: 7d08 7c01 7c01 6401 1900 7c08 6b02 1900  }.|.|.d...|.k...
+00008290: 6a06 6407 6408 8d01 7d09 7c09 7c09 6401  j.d.d...}.|.|.d.
+000082a0: 1900 a004 7c02 a101 1900 7d0a 7407 7c0a  ....|.....}.t.|.
+000082b0: 8301 6403 6b04 7398 7407 7c09 8301 6403  ..d.k.s.t.|...d.
+000082c0: 6b02 72e0 7198 7400 a008 7c02 7c08 a102  k.r.q.t...|.|...
+000082d0: 7d02 7c09 6a09 6409 640a 640b 8d02 7d09  }.|.j.d.d.d...}.
+000082e0: 7c09 6401 1900 6a02 6403 1900 7d0b 7c01  |.d...j.d...}.|.
+000082f0: 7c01 6401 1900 7c0b 6b02 1900 640c 1900  |.d...|.k...d...
+00008300: 6a02 6403 1900 7d0c 7c0c 7c02 7601 7298  j.d...}.|.|.v.r.
+00008310: 7c0c 640d 6b03 7298 7400 a008 7c02 7c0c  |.d.k.r.t...|.|.
+00008320: a102 7d02 7c01 7c01 6401 1900 7c0c 6b02  ..}.|.|.d...|.k.
+00008330: 1900 6a06 6407 6408 8d01 7d0d 7407 7c0d  ..j.d.d...}.t.|.
+00008340: 8301 6403 6b01 9001 7270 740a 640e 7c0c  ..d.k...rpt.d.|.
+00008350: 8302 0100 7198 7c0d 640c 1900 6a02 6403  ....q.|.d...j.d.
+00008360: 1900 7d0c 9001 7122 7198 7c01 7c01 6401  ..}...q"q.|.|.d.
+00008370: 1900 a004 7c02 a101 1900 7d0e 7c0e 5300  ....|.....}.|.S.
+00008380: 290f 4e72 0600 0000 727c 0000 0072 0100  ).Nr....r|...r..
+00008390: 0000 7261 0000 0072 2800 0000 7278 0000  ..ra...r(...rx..
+000083a0: 0054 7207 0000 0072 6c00 0000 4672 3600  .Tr....rl...Fr6.
+000083b0: 0000 720d 0000 0072 6600 0000 fa11 6368  ..r....rf.....ch
+000083c0: 6563 6b20 7468 6973 2073 7562 6964 2029  eck this subid )
+000083d0: 0b72 1a00 0000 722b 0000 0072 1300 0000  .r....r+...r....
+000083e0: 7242 0000 0072 1200 0000 728c 0000 0072  rB...r....r....r
+000083f0: 1400 0000 7215 0000 0072 4d00 0000 7240  ....r....rM...r@
+00008400: 0000 0072 6800 0000 290f 72f3 0000 0072  ...rh...).r....r
+00008410: 9000 0000 72f4 0000 005a 156c 616b 6569  ....r....Z.lakei
+00008420: 645f 696e 5f6e 6577 5f6e 6574 776f 726b  d_in_new_network
+00008430: 5a0a 6d61 736b 5f6c 616b 6573 5a09 6d61  Z.mask_lakesZ.ma
+00008440: 736b 5f70 6f69 735a 1770 6f74 656e 7469  sk_poisZ.potenti
+00008450: 616c 5f73 7562 5f74 6f5f 6578 7465 6e64  al_sub_to_extend
+00008460: da13 7375 6269 645f 7769 7468 5f75 7073  ..subid_with_ups
+00008470: 7472 6561 6d72 f600 0000 da0c 7570 7374  treamr......upst
+00008480: 7265 616d 5f73 7562 da16 7570 7374 7265  ream_sub..upstre
+00008490: 616d 5f73 7562 5f77 6974 6872 6976 6572  am_sub_withriver
+000084a0: da09 6375 725f 7375 6269 64da 0d63 7572  ..cur_subid..cur
+000084b0: 5f64 6f77 6e73 7562 6964 da0b 6375 725f  _downsubid..cur_
+000084c0: 7375 6269 6e66 6f5a 1053 656c 6563 7465  subinfoZ.Selecte
+000084d0: 645f 7269 765f 6f75 7472 2400 0000 7224  d_riv_outr$...r$
+000084e0: 0000 0072 2500 0000 72ef 0000 0060 0900  ...r%...r....`..
+000084f0: 0073 6400 0000 0001 1004 1001 0c02 0401  .sd.............
+00008500: 18ff 0403 0c02 0601 04ff 0601 02ff 0603  ................
+00008510: 0a01 02ff 0803 1001 0803 1001 02ff 0604  ................
+00008520: 0a01 02ff 0604 1801 0203 0c04 0401 04ff  ................
+00008530: 0603 0e06 0801 02ff 0401 02ff 0401 02ff  ................
+00008540: 0403 1002 0c01 1001 02ff 0602 0e01 0a01  ................
+00008550: 0201 1401 0a01 02ff 0602 72ef 0000 0063  ..........r....c
+00008560: 0300 0000 0000 0000 0000 0000 0c00 0000  ................
+00008570: 0700 0000 4300 0000 7346 0100 007c 0064  ....C...sF...|.d
+00008580: 0119 00a0 007c 0064 0219 006a 01a1 017d  .....|.d...j...}
+00008590: 037c 007c 0319 006a 0264 0364 048d 017d  .|.|...j.d.d...}
+000085a0: 0474 03a0 047c 0464 0119 006a 01a1 017d  .t...|.d...j...}
+000085b0: 057c 0544 005d f87d 067c 007c 0064 0219  .|.D.].}.|.|.d..
+000085c0: 007c 066b 0219 006a 0264 0364 048d 017d  .|.k...j.d.d...}
+000085d0: 077c 077c 0764 0119 00a0 007c 01a1 0119  .|.|.d.....|....
+000085e0: 007d 0874 057c 0883 0164 056b 0472 7471  .}.t.|...d.k.rtq
+000085f0: 3874 03a0 007c 017c 007c 0064 0119 007c  8t...|.|.|.d...|
+00008600: 066b 0219 0064 0619 006a 01a1 027d 037c  .k...d...j...}.|
+00008610: 017c 030f 0019 007d 017c 076a 0664 0764  .|.....}.|.j.d.d
+00008620: 0864 098d 027d 077c 0764 0119 006a 0164  .d...}.|.d...j.d
+00008630: 0519 007d 097c 027c 0264 0119 007c 096b  ...}.|.|.d...|.k
+00008640: 0219 0064 0219 006a 0164 0519 007d 0a7c  ...d...j.d...}.|
+00008650: 0a7c 0176 0172 387c 0a64 0a6b 0372 3874  .|.v.r8|.d.k.r8t
+00008660: 03a0 077c 017c 0aa1 027d 017c 027c 0264  ...|.|...}.|.|.d
+00008670: 0119 007c 0a6b 0219 006a 0264 0364 048d  ...|.k...j.d.d..
+00008680: 017d 0b74 057c 0b83 0164 056b 0190 0172  .}.t.|...d.k...r
+00008690: 2074 0864 0b7c 0a83 0201 0071 387c 0b64   t.d.|.....q8|.d
+000086a0: 0219 006a 0164 0519 007d 0a71 d271 3874  ...j.d...}.q.q8t
+000086b0: 097c 017c 007c 0283 037d 007c 017c 0066  .|.|.|...}.|.|.f
+000086c0: 0253 0029 0c4e 7206 0000 0072 0d00 0000  .S.).Nr....r....
+000086d0: 5472 0700 0000 7201 0000 0072 8900 0000  Tr....r....r....
+000086e0: 726c 0000 0046 7236 0000 0072 6600 0000  rl...Fr6...rf...
+000086f0: 72fd 0000 0029 0a72 1200 0000 7213 0000  r....).r....r...
+00008700: 0072 1400 0000 721a 0000 0072 2b00 0000  .r....r....r+...
+00008710: 7215 0000 0072 4000 0000 724d 0000 0072  r....r@...rM...r
+00008720: 6800 0000 da19 7570 6461 7465 5f63 6861  h.....update_cha
+00008730: 6e6e 656c 5f61 7474 7269 6275 7465 7329  nnel_attributes)
+00008740: 0c72 9000 0000 72f4 0000 00da 1066 696e  .r....r......fin
+00008750: 616c 7269 765f 696e 666f 706c 7972 2300  alriv_infoplyr#.
+00008760: 0000 5a11 7375 625f 7769 7468 5f75 7073  ..Z.sub_with_ups
+00008770: 7472 6561 6d72 fe00 0000 72f6 0000 0072  treamr....r....r
+00008780: ff00 0000 7200 0100 0072 0101 0000 7202  ....r....r....r.
+00008790: 0100 0072 0301 0000 7224 0000 0072 2400  ...r....r$...r$.
+000087a0: 0000 7225 0000 00da 3041 6464 5f52 6976  ..r%....0Add_Riv
+000087b0: 6572 5f53 6567 6d65 6e74 5f42 6574 7765  er_Segment_Betwe
+000087c0: 656e 5f4c 616b 6573 5f41 6e64 5f4f 6273  en_Lakes_And_Obs
+000087d0: 6572 7661 7469 6f6e 73a1 0900 0073 5000  ervations....sP.
+000087e0: 0000 000f 1401 1002 1001 0803 1001 02ff  ................
+000087f0: 0604 0a01 02ff 0604 0c01 0203 0401 16ff  ................
+00008800: 0402 0a05 0401 04ff 0602 0e06 0801 02ff  ................
+00008810: 0401 02ff 0401 02ff 0403 1002 0c01 1001  ................
+00008820: 02ff 0602 0e01 0a01 0201 1203 0201 06ff  ................
+00008830: 0402 7206 0100 0063 0300 0000 0000 0000  ..r....c........
+00008840: 0000 0000 0900 0000 0600 0000 4300 0000  ............C...
+00008850: 7390 0100 0074 00a0 017c 017c 0164 0119  s....t...|.|.d..
+00008860: 00a0 027c 00a1 0119 0064 0219 006a 03a1  ...|.....d...j..
+00008870: 017d 037c 027c 0264 0219 00a0 027c 00a1  .}.|.|.d.....|..
+00008880: 0119 007d 047c 0344 0090 015d 547d 057c  ...}.|.D...]T}.|
+00008890: 0164 0219 007c 056b 027d 0674 00a0 017c  .d...|.k.}.t...|
+000088a0: 017c 0619 0064 0119 006a 03a1 017d 077c  .|...d...j...}.|
+000088b0: 047c 0464 0219 00a0 027c 07a1 0119 007d  .|.d.....|.....}
+000088c0: 0874 047c 0883 0164 036b 0472 3474 00a0  .t.|...d.k.r4t..
+000088d0: 057c 0864 0419 006a 03a1 017c 016a 067c  .|.d...j...|.j.|
+000088e0: 0664 0466 023c 0074 006a 077c 0864 0519  .d.f.<.t.j.|.d..
+000088f0: 006a 037c 0864 0419 006a 0364 068d 027c  .j.|.d...j.d...|
+00008900: 016a 067c 0664 0566 023c 0074 006a 077c  .j.|.d.f.<.t.j.|
+00008910: 0864 0719 006a 037c 0864 0419 006a 0364  .d...j.|.d...j.d
+00008920: 068d 027c 016a 067c 0664 0766 023c 0074  ...|.j.|.d.f.<.t
+00008930: 006a 077c 0864 0819 006a 037c 0864 0419  .j.|.d...j.|.d..
+00008940: 006a 0364 068d 027c 016a 067c 0664 0866  .j.d...|.j.|.d.f
+00008950: 023c 0074 006a 077c 0864 0919 006a 037c  .<.t.j.|.d...j.|
+00008960: 0864 0419 006a 0364 068d 027c 016a 067c  .d...j.d...|.j.|
+00008970: 0664 0966 023c 0074 00a0 087c 0864 0a19  .d.f.<.t...|.d..
+00008980: 006a 03a1 017c 016a 067c 0664 0a66 023c  .j...|.j.|.d.f.<
+00008990: 0074 00a0 087c 0864 0b19 006a 03a1 017c  .t...|.d...j...|
+000089a0: 016a 067c 0664 0b66 023c 0074 00a0 087c  .j.|.d.f.<.t...|
+000089b0: 0864 0c19 006a 03a1 017c 016a 067c 0664  .d...j...|.j.|.d
+000089c0: 0c66 023c 0074 00a0 097c 0864 0d19 006a  .f.<.t...|.d...j
+000089d0: 03a1 017c 016a 067c 0664 0d66 023c 0071  ...|.j.|.d.f.<.q
+000089e0: 347c 0153 0029 0e4e 7289 0000 0072 0600  4|.S.).Nr....r..
+000089f0: 0000 7201 0000 0072 7000 0000 7282 0000  ..r....rp...r...
+00008a00: 0072 7e00 0000 7283 0000 0072 8400 0000  .r~...r....r....
+00008a10: 7285 0000 0072 9a00 0000 729b 0000 0072  r....r....r....r
+00008a20: 8600 0000 7287 0000 0029 0a72 1a00 0000  ....r....).r....
+00008a30: 722b 0000 0072 1200 0000 7213 0000 0072  r+...r....r....r
+00008a40: 1500 0000 723e 0000 0072 1900 0000 728e  ....r>...r....r.
+00008a50: 0000 0072 6700 0000 728f 0000 0029 0972  ...rg...r....).r
+00008a60: f400 0000 7290 0000 0072 0501 0000 5a10  ....r....r....Z.
+00008a70: 7375 6269 645f 7570 6461 7465 5f72 6976  subid_update_riv
+00008a80: 5a12 616c 6c5f 7269 7665 725f 7365 676d  Z.all_river_segm
+00008a90: 656e 7473 72f6 0000 005a 086d 6173 6b5f  entsr....Z.mask_
+00008aa0: 6e65 775a 0a6f 6c64 5f73 7562 6964 735a  newZ.old_subidsZ
+00008ab0: 0e72 6976 5f69 6e5f 6e65 775f 7375 6272  .riv_in_new_subr
+00008ac0: 2400 0000 7224 0000 0072 2500 0000 7204  $...r$...r%...r.
+00008ad0: 0100 00e5 0900 0073 5a00 0000 0004 0401  .......sZ.......
+00008ae0: 16ff 0402 0a01 02ff 0602 0a01 0c01 1401  ................
+00008af0: 0a01 02ff 0603 0c01 0401 08ff 0e02 0401  ................
+00008b00: 0801 08fe 1004 0401 0801 08fe 1004 0401  ................
+00008b10: 0801 08fe 1004 0401 0801 08fe 1004 0401  ................
+00008b20: 08ff 0e02 0401 08ff 0e03 0401 08ff 0e02  ................
+00008b30: 0401 08ff 1002 7204 0100 0063 0400 0000  ......r....c....
+00008b40: 0000 0000 0000 0000 1600 0000 0700 0000  ................
+00008b50: 4300 0000 7300 0200 007c 0064 0119 00a0  C...s....|.d....
+00008b60: 0074 01a1 017c 0064 013c 007c 0064 0219  .t...|.d.<.|.d..
+00008b70: 00a0 0074 02a1 017c 0064 023c 007c 0064  ...t...|.d.<.|.d
+00008b80: 0319 00a0 0074 02a1 017c 0064 033c 007c  .....t...|.d.<.|
+00008b90: 006a 037c 0064 0419 0064 056b 0219 006a  .j.|.d...d.k...j
+00008ba0: 0464 0664 078d 017d 047c 006a 037c 0064  .d.d...}.|.j.|.d
+00008bb0: 0419 0064 086b 0219 006a 0464 0664 078d  ...d.k...j.d.d..
+00008bc0: 017d 0564 097c 006a 0576 0072 7a64 097d  .}.d.|.j.v.rzd.}
+00008bd0: 066e 0464 0a7d 067c 0564 0119 007c 016b  .n.d.}.|.d...|.k
+00008be0: 057d 077c 057c 0619 0064 086b 027d 0874  .}.|.|...d.k.}.t
+00008bf0: 06a0 077c 077c 08a1 027d 097c 056a 037c  ...|.|...}.|.j.|
+00008c00: 0919 0064 0219 006a 087d 0a7c 0a7c 0a64  ...d...j.}.|.|.d
+00008c10: 0b6b 0419 007d 0a74 06a0 097c 0aa1 017d  .k...}.t...|...}
+00008c20: 0a7c 0464 0119 007c 026b 057d 077c 047c  .|.d...|.k.}.|.|
+00008c30: 0619 0064 086b 027d 0874 06a0 077c 077c  ...d.k.}.t...|.|
+00008c40: 08a1 027d 097c 047c 0919 0064 0219 006a  ...}.|.|...d...j
+00008c50: 087d 0b7c 0b7c 0b64 0b6b 0419 007d 0b74  .}.|.|.d.k...}.t
+00008c60: 06a0 097c 0ba1 017d 0b74 0a7c 0383 0164  ...|...}.t.|...d
+00008c70: 0b6b 0490 0172 247c 037d 0c6e 0664 0c67  .k...r$|.}.n.d.g
+00008c80: 017d 0c7c 0564 0219 006a 087d 0d7c 0464  .}.|.d...j.}.|.d
+00008c90: 0219 006a 087d 0e74 06a0 0b7c 0ca1 017d  ...j.}.t...|...}
+00008ca0: 0f74 06a0 0c7c 0d7c 0fa1 027d 1074 06a0  .t...|.|...}.t..
+00008cb0: 0c7c 0e7c 0fa1 027d 117c 0d7c 1019 007d  .|.|...}.|.|...}
+00008cc0: 1274 06a0 097c 12a1 017d 127c 0e7c 1119  .t...|...}.|.|..
+00008cd0: 007d 1374 06a0 097c 13a1 017d 1374 066a  .}.t...|...}.t.j
+00008ce0: 0d7c 0b7c 1366 0264 0b64 0d8d 027d 0b74  .|.|.f.d.d...}.t
+00008cf0: 066a 0d7c 0a7c 1266 0264 0b64 0d8d 027d  .j.|.|.f.d.d...}
+00008d00: 0a7c 006a 037c 0064 0419 0064 086b 0274  .|.j.|.d...d.k.t
+00008d10: 06a0 0e7c 0064 0219 00a0 0f7c 0aa1 01a1  ...|.d.....|....
+00008d20: 0140 0019 007d 147c 006a 037c 0064 0419  .@...}.|.j.|.d..
+00008d30: 0064 056b 0274 06a0 0e7c 0064 0219 00a0  .d.k.t...|.d....
+00008d40: 0f7c 0ba1 01a1 0140 0019 007d 157c 0b7c  .|.....@...}.|.|
+00008d50: 0a7c 147c 1566 0453 0029 0e7a 8052 6574  .|.|.f.S.).z.Ret
+00008d60: 7275 6e20 7365 6c65 6374 6564 206c 616b  run selected lak
+00008d70: 6527 7320 6174 7472 6962 7574 6520 7461  e's attribute ta
+00008d80: 626c 6520 616e 6420 4944 0a20 2020 202d  ble and ID.    -
+00008d90: 2d2d 2d2d 2d2d 2d2d 2d0a 0a20 2020 204e  ---------..    N
+00008da0: 6f74 6573 0a20 2020 202d 2d2d 2d2d 2d2d  otes.    -------
+00008db0: 0a0a 2020 2020 5265 7475 726e 733a 0a20  ..    Returns:. 
+00008dc0: 2020 202d 2d2d 2d2d 2d2d 0a20 2020 2020     -------.     
+00008dd0: 2020 204e 6f6e 652c 0a20 2020 2072 9d00     None,.    r..
+00008de0: 0000 727c 0000 0072 6300 0000 7261 0000  ..r|...rc...ra..
+00008df0: 0072 6200 0000 5472 0700 0000 7228 0000  .rb...Tr....r(..
+00008e00: 0072 7800 0000 7279 0000 0072 0100 0000  .rx...ry...r....
+00008e10: 6981 6967 ff72 0e00 0000 2910 7216 0000  i.ig.r....).r...
+00008e20: 0072 6000 0000 722d 0000 0072 1900 0000  .r`...r-...r....
+00008e30: 7214 0000 0072 1100 0000 721a 0000 0072  r....r....r....r
+00008e40: 8c00 0000 7213 0000 0072 2b00 0000 7215  ....r....r+...r.
+00008e50: 0000 00da 0561 7272 6179 722e 0000 0072  .....arrayr....r
+00008e60: 1b00 0000 72a3 0000 0072 1200 0000 2916  ....r....r....).
+00008e70: da0d 6669 6e61 6c63 6174 5f69 6e66 6fda  ..finalcat_info.
+00008e80: 1554 6872 6573 5f41 7265 615f 436f 6e6e  .Thres_Area_Conn
+00008e90: 5f4c 616b 6573 da19 5468 7265 735f 4172  _Lakes..Thres_Ar
+00008ea0: 6561 5f4e 6f6e 5f43 6f6e 6e5f 4c61 6b65  ea_Non_Conn_Lake
+00008eb0: 73da 1553 656c 6563 7465 645f 4c61 6b65  s..Selected_Lake
+00008ec0: 5f4c 6973 745f 696e 5a0e 4e6f 6e5f 436f  _List_inZ.Non_Co
+00008ed0: 6e6e 4c5f 696e 666f 5a0a 436f 6e6e 4c5f  nnL_infoZ.ConnL_
+00008ee0: 696e 666f 7293 0000 0072 4900 0000 724a  infor....rI...rJ
+00008ef0: 0000 0072 2300 0000 5a12 5365 6c65 6374  ...r#...Z.Select
+00008f00: 6564 5f43 6f6e 6e4c 616b 6573 5a16 5365  ed_ConnLakesZ.Se
+00008f10: 6c65 6374 6564 5f4e 6f6e 5f43 6f6e 6e4c  lected_Non_ConnL
+00008f20: 616b 6573 5a12 5365 6c65 6374 6564 5f4c  akesZ.Selected_L
+00008f30: 616b 655f 4c69 7374 5a09 416c 6c5f 436f  ake_ListZ.All_Co
+00008f40: 6e6e 4c5a 0d41 6c6c 5f4e 6f6e 5f43 6f6e  nnLZ.All_Non_Con
+00008f50: 6e4c 5a1b 5365 6c65 6374 6564 5f4c 616b  nLZ.Selected_Lak
+00008f60: 655f 4c69 7374 5f69 6e5f 6172 7261 795a  e_List_in_arrayZ
+00008f70: 076d 6173 6b5f 434c 5a08 6d61 736b 5f4e  .mask_CLZ.mask_N
+00008f80: 434c 5a17 5365 6c65 6374 6564 5f43 6f6e  CLZ.Selected_Con
+00008f90: 6e4c 616b 6573 5f4c 6973 745a 1b53 656c  nLakes_ListZ.Sel
+00008fa0: 6563 7465 645f 4e6f 6e5f 436f 6e6e 4c61  ected_Non_ConnLa
+00008fb0: 6b65 735f 4c69 7374 da1a 556e 5f53 656c  kes_List..Un_Sel
+00008fc0: 6563 7465 645f 436f 6e6e 4c61 6b65 735f  ected_ConnLakes_
+00008fd0: 696e 666f da1a 556e 5f53 656c 6563 7465  info..Un_Selecte
+00008fe0: 645f 4e6f 6e5f 436f 6e6e 4c5f 696e 666f  d_Non_ConnL_info
+00008ff0: 7224 0000 0072 2400 0000 7225 0000 00da  r$...r$...r%....
+00009000: 2c52 6574 7572 6e5f 5365 6c65 6374 6564  ,Return_Selected
+00009010: 5f4c 616b 6573 5f41 7474 7269 6275 7465  _Lakes_Attribute
+00009020: 5f54 6162 6c65 5f41 6e64 5f49 6412 0a00  _Table_And_Id...
+00009030: 0073 8200 0000 0010 1201 1201 1202 1201  .s..............
+00009040: 02ff 0602 1201 02ff 0603 0a01 0602 0403  ................
+00009050: 0c01 0c01 0c01 0401 02ff 0202 02fe 0604  ................
+00009060: 0c01 0a02 0c01 0c01 0c02 0201 02ff 0202  ................
+00009070: 02fe 0603 0c01 0a03 0e01 0603 0601 0a01  ................
+00009080: 0a01 0a02 0c01 0c02 0801 0a01 0801 0a03  ................
+00009090: 0401 08ff 0602 0401 08ff 0603 0401 0a01  ................
+000090a0: 12ff 02ff 0404 0401 0a01 12ff 02ff 0406  ................
+000090b0: 0201 0201 0201 02fc 720e 0100 0063 0200  ........r....c..
+000090c0: 0000 0000 0000 0000 0000 0e00 0000 0c00  ................
+000090d0: 0000 4300 0000 7322 0200 007c 006a 0064  ..C...s"...|.j.d
+000090e0: 0164 028d 017d 0264 037c 0264 043c 0064  .d...}.d.|.d.<.d
+000090f0: 037c 0264 053c 007c 0264 0619 007c 0264  .|.d.<.|.d...|.d
+00009100: 073c 007c 026a 0164 0164 0164 088d 0201  .<.|.j.d.d.d....
+00009110: 0064 097d 0364 097c 026a 0276 0172 4864  .d.}.d.|.j.v.rHd
+00009120: 0a7d 037c 0164 0b19 006a 037d 0474 04a0  .}.|.d...j.}.t..
+00009130: 057c 04a1 017d 0474 0664 0c74 077c 0483  .|...}.t.d.t.|..
+00009140: 0183 0244 0090 015d b07d 057c 047c 0519  ...D...].}.|.|..
+00009150: 007d 067c 006a 087c 0064 0b19 007c 066b  .}.|.j.|.d...|.k
+00009160: 027c 0064 0d19 0064 0e6b 0340 0019 00a0  .|.d...d.k.@....
+00009170: 00a1 007d 077c 076a 0964 0f67 0164 0164  ...}.|.j.d.g.d.d
+00009180: 108d 027d 0774 04a0 057c 0764 1119 006a  ...}.t...|.d...j
+00009190: 03a1 017d 0874 077c 0783 0174 077c 0883  ...}.t.|...t.|..
+000091a0: 016b 0272 cc71 6a74 04a0 0a7c 08a1 0190  .k.r.qjt...|....
+000091b0: 0172 2674 04a0 0a7c 077c 0319 006a 03a1  .r&t...|.|...j..
+000091c0: 0164 0c6b 0190 0172 267c 0764 0619 006a  .d.k...r&|.d...j
+000091d0: 0374 077c 0783 0164 1218 0019 007d 097c  .t.|...d.....}.|
+000091e0: 0764 0619 006a 037d 0a74 0b7c 097c 007c  .d...j.}.t.|.|.|
+000091f0: 0264 127c 0a7c 0064 0364 1264 138d 087d  .d.|.|.d.d.d...}
+00009200: 0267 007d 0b64 127d 0c74 0664 0c74 077c  .g.}.d.}.t.d.t.|
+00009210: 0783 0183 0244 005d de7d 0d7c 0764 0619  .....D.].}.|.d..
+00009220: 006a 037c 0d19 007d 097c 0ba0 0c7c 09a1  .j.|...}.|...|..
+00009230: 0101 007c 0d74 077c 0783 0164 1218 006b  ...|.t.|...d...k
+00009240: 0290 0172 a474 04a0 0d7c 0ba1 017d 0a74  ...r.t...|...}.t
+00009250: 0b7c 097c 007c 0264 127c 0a7c 007c 0764  .|.|.|.d.|.|.|.d
+00009260: 1119 006a 037c 0d19 007c 0c64 138d 087d  ...j.|...|.d...}
+00009270: 0267 007d 0b7c 0c64 1217 007d 0c6e 747c  .g.}.|.d...}.nt|
+00009280: 0764 1119 006a 037c 0d19 007c 0764 1119  .d...j.|...|.d..
+00009290: 006a 037c 0d64 1217 0019 006b 0290 0172  .j.|.d.....k...r
+000092a0: e07c 077c 0319 006a 037c 0d19 0064 0c6b  .|.|...j.|...d.k
+000092b0: 0190 0172 e090 0171 3c6e 3874 04a0 0d7c  ...r...q<n8t...|
+000092c0: 0ba1 017d 0a74 0b7c 097c 007c 0264 127c  ...}.t.|.|.|.d.|
+000092d0: 0a7c 007c 0764 1119 006a 037c 0d19 007c  .|.|.d...j.|...|
+000092e0: 0c64 138d 087d 0267 007d 0b7c 0c64 1217  .d...}.g.}.|.d..
+000092f0: 007d 0c90 0171 3c71 6a7c 0253 0029 147a  .}...q<qj|.S.).z
+00009300: b143 6861 6e67 6520 6174 7472 6962 7574  .Change attribut
+00009310: 6573 2066 6f72 2063 6174 6368 6d65 6e74  es for catchment
+00009320: 7320 7468 6174 206e 6565 6473 2074 6f20  s that needs to 
+00009330: 6265 206d 6572 6765 6420 6475 6520 746f  be merged due to
+00009340: 2072 656d 6f76 650a 2020 2020 2020 2020   remove.        
+00009350: 636f 6e6e 6563 7465 6420 6c61 6b65 730a  connected lakes.
+00009360: 2020 2020 2d2d 2d2d 2d2d 2d2d 2d2d 0a0a      ----------..
+00009370: 2020 2020 4e6f 7465 730a 2020 2020 2d2d      Notes.    --
+00009380: 2d2d 2d2d 2d0a 0a20 2020 2052 6574 7572  -----..    Retur
+00009390: 6e73 3a0a 2020 2020 2d2d 2d2d 2d2d 2d0a  ns:.    -------.
+000093a0: 2020 2020 2020 2020 4e6f 6e65 2c0a 2020          None,.  
+000093b0: 2020 5472 0700 0000 7266 0000 0072 7b00    Tr....rf...r{.
+000093c0: 0000 7288 0000 0072 0600 0000 da07 6e73  ..r....r......ns
+000093d0: 7562 6964 3272 ea00 0000 7278 0000 0072  ubid2r....rx...r
+000093e0: 7900 0000 7263 0000 0072 0100 0000 7261  y...rc...r....ra
+000093f0: 0000 0072 6200 0000 7265 0000 0072 6d00  ...rb...re...rm.
+00009400: 0000 727c 0000 0072 2800 0000 72ed 0000  ..r|...r(...r...
+00009410: 0029 0e72 1400 0000 72ee 0000 0072 1100  .).r....r....r..
+00009420: 0000 7213 0000 0072 1a00 0000 722b 0000  ..r....r....r+..
+00009430: 0072 2900 0000 7215 0000 0072 1900 0000  .r)...r....r....
+00009440: 7240 0000 0072 6700 0000 72aa 0000 0072  r@...rg...r....r
+00009450: 4d00 0000 72f1 0000 0029 0eda 1266 696e  M...r....)...fin
+00009460: 616c 6361 745f 696e 666f 5f74 656d 7072  alcat_info_tempr
+00009470: 0c01 0000 7290 0000 0072 9300 0000 72f5  ....r....r....r.
+00009480: 0000 0072 c300 0000 72f9 0000 0072 fa00  ...r....r....r..
+00009490: 0000 5a0a 4e5f 4879 6c61 6b65 6964 72f6  ..Z.N_Hylakeidr.
+000094a0: 0000 0072 f800 0000 72f7 0000 0072 a800  ...r....r....r..
+000094b0: 0000 72fb 0000 0072 2400 0000 7224 0000  ..r....r$...r$..
+000094c0: 0072 2500 0000 da45 4368 616e 6765 5f41  .r%....EChange_A
+000094d0: 7474 7269 6275 7465 5f56 616c 7565 735f  ttribute_Values_
+000094e0: 466f 725f 4361 7463 686d 656e 7473 5f4e  For_Catchments_N
+000094f0: 6565 645f 546f 5f42 655f 4d65 7267 6564  eed_To_Be_Merged
+00009500: 5f42 795f 5265 6d6f 7665 5f43 4c6e 0a00  _By_Remove_CLn..
+00009510: 0073 9400 0000 000e 0c01 0801 0801 0c01  .s..............
+00009520: 0e03 0401 0a01 0402 0a01 0a01 1402 0801  ................
+00009530: 0401 0a01 0aff 02ff 0804 1003 1001 1001  ................
+00009540: 0203 2201 1601 0a01 0201 0201 0201 0201  ..".............
+00009550: 0201 0201 0201 0201 02f8 060c 0401 0401  ................
+00009560: 1201 0e01 0a03 1201 0a01 0201 0201 0201  ................
+00009570: 0201 0201 0201 0201 0c01 02f8 060a 0401  ................
+00009580: 0a03 0c01 10ff 02ff 0403 10fd 0405 0602  ................
+00009590: 0a01 0201 0201 0201 0201 0201 0201 0201  ................
+000095a0: 0c01 02f8 060a 0401 0e01 7211 0100 0063  ..........r....c
+000095b0: 0300 0000 0000 0000 0000 0000 0f00 0000  ................
+000095c0: 0a00 0000 4300 0000 7300 0200 007c 026a  ....C...s....|.j
+000095d0: 0064 0167 0164 0267 0164 038d 027d 0274  .d.g.d.g.d...}.t
+000095e0: 0164 0474 027c 0283 0183 0244 0090 015d  .d.t.|.....D...]
+000095f0: a47d 037c 0264 0519 006a 037c 0319 007d  .}.|.d...j.|...}
+00009600: 047c 016a 047c 0164 0519 007c 046b 0219  .|.j.|.d...|.k..
+00009610: 00a0 05a1 007d 0574 027c 0583 0164 066b  .....}.t.|...d.k
+00009620: 0372 6874 0664 0783 0101 0074 067c 0583  .rht.d.....t.|..
+00009630: 0101 0071 2067 007d 067c 0564 0819 006a  ...q g.}.|.d...j
+00009640: 0364 0419 007d 077c 0564 0919 006a 0364  .d...}.|.d...j.d
+00009650: 0419 007d 087c 06a0 077c 07a1 0101 0064  ...}.|...|.....d
+00009660: 0a7d 0964 047d 0a7c 016a 047c 0164 0819  .}.d.}.|.j.|.d..
+00009670: 007c 086b 0219 00a0 05a1 007d 0b74 027c  .|.k.......}.t.|
+00009680: 0b83 0164 046b 0272 c67c 0864 046b 0072  ...d.k.r.|.d.k.r
+00009690: c671 207c 0b64 0b19 006a 0364 0419 0064  .q |.d...j.d...d
+000096a0: 0c6b 0390 0172 287c 006a 047c 0064 0819  .k...r(|.j.|.d..
+000096b0: 007c 086b 0219 0064 0d19 006a 0364 0419  .|.k...d...j.d..
+000096c0: 007d 0c7c 0c64 046b 0490 0172 147c 0c7d  .}.|.d.k...r.|.}
+000096d0: 0964 067d 0a7c 06a0 077c 09a1 0101 006e  .d.}.|...|.....n
+000096e0: 127c 087d 0964 0a7d 0a7c 06a0 077c 09a1  .|.}.d.}.|...|..
+000096f0: 0101 006e 4c7c 006a 047c 0064 0819 007c  ...nL|.j.|.d...|
+00009700: 086b 0219 0064 0d19 006a 0364 0419 007d  .k...d...j.d...}
+00009710: 0c7c 0c64 046b 0490 0172 627c 0c7d 0964  .|.d.k...rb|.}.d
+00009720: 067d 0a7c 06a0 077c 09a1 0101 006e 127c  .}.|...|.....n.|
+00009730: 087d 0964 0a7d 0a7c 06a0 077c 09a1 0101  .}.d.}.|...|....
+00009740: 007c 007c 0064 0819 007c 096b 0219 0064  .|.|.d...|.k...d
+00009750: 0519 006a 0364 0419 007d 0d7c 0a64 046b  ...j.d...}.|.d.k
+00009760: 0490 0172 b074 087c 097c 007c 0064 067c  ...r.t.|.|.|.d.|
+00009770: 067c 007c 0d64 0e8d 077d 0071 2074 087c  .|.|.d...}.q t.|
+00009780: 097c 007c 0064 067c 067c 017c 0d64 0e8d  .|.|.d.|.|.|.d..
+00009790: 077d 0071 207c 0064 0d19 0064 046b 017d  .}.q |.d...d.k.}
+000097a0: 0e7c 006a 047c 0e64 0f66 0219 006a 037c  .|.j.|.d.f...j.|
+000097b0: 006a 047c 0e64 0d66 023c 007c 006a 0964  .j.|.d.f.<.|.j.d
+000097c0: 0f67 0164 108d 0101 007c 0053 0029 117a  .g.d.....|.S.).z
+000097d0: b543 6861 6e67 6520 6174 7472 6962 7574  .Change attribut
+000097e0: 6573 2066 6f72 2063 6174 6368 6d65 6e74  es for catchment
+000097f0: 7320 7468 6174 206e 6565 6473 2074 6f20  s that needs to 
+00009800: 6265 206d 6572 6765 6420 6475 6520 746f  be merged due to
+00009810: 2072 656d 6f76 650a 2020 2020 2020 2020   remove.        
+00009820: 6e6f 6e20 636f 6e6e 6563 7465 6420 6c61  non connected la
+00009830: 6b65 730a 2020 2020 2d2d 2d2d 2d2d 2d2d  kes.    --------
+00009840: 2d2d 0a0a 2020 2020 4e6f 7465 730a 2020  --..    Notes.  
+00009850: 2020 2d2d 2d2d 2d2d 2d0a 0a20 2020 2052    -------..    R
+00009860: 6574 7572 6e73 3a0a 2020 2020 2d2d 2d2d  eturns:.    ----
+00009870: 2d2d 2d0a 2020 2020 2020 2020 4e6f 6e65  ---.        None
+00009880: 2c0a 2020 2020 726c 0000 0046 726d 0000  ,.    rl...Frm..
+00009890: 0072 0100 0000 727c 0000 0072 2800 0000  .r....r|...r(...
+000098a0: 7a28 4974 2069 7320 6e6f 7420 6120 6e6f  z(It is not a no
+000098b0: 6e20 636f 6e6e 6563 7465 6420 6c61 6b65  n connected lake
+000098c0: 2063 6174 6368 6d65 6e74 7206 0000 0072   catchmentr....r
+000098d0: 0d00 0000 7266 0000 0072 6100 0000 7262  ....rf...ra...rb
+000098e0: 0000 0072 7b00 0000 a907 7248 0000 0072  ...r{.....rH...r
+000098f0: a400 0000 7290 0000 0072 a500 0000 72a6  ....r....r....r.
+00009900: 0000 0072 a700 0000 7261 0000 0072 0f01  ...r....ra...r..
+00009910: 0000 7210 0000 0029 0a72 4000 0000 7229  ..r....).r@...r)
+00009920: 0000 0072 1500 0000 7213 0000 0072 1900  ...r....r....r..
+00009930: 0000 7214 0000 0072 6800 0000 724d 0000  ..r....rh...rM..
+00009940: 0072 aa00 0000 721c 0000 0029 0f72 9000  .r....r....).r..
+00009950: 0000 7210 0100 0072 0d01 0000 7247 0000  ..r....r....rG..
+00009960: 005a 1752 656d 6f76 655f 4e6f 6e5f 436f  .Z.Remove_Non_Co
+00009970: 6e6e 4c5f 4c61 6b65 6964 5a1e 5265 6d6f  nnL_LakeidZ.Remo
+00009980: 7665 5f4e 6f6e 5f43 6f6e 6e4c 5f4c 616b  ve_Non_ConnL_Lak
+00009990: 655f 5375 625f 696e 666f 72f7 0000 0072  e_Sub_infor....r
+000099a0: d800 0000 72d7 0000 0072 f600 0000 5a0f  ....r....r....Z.
+000099b0: 6973 5f70 7265 5f6d 6f64 6966 6965 6472  is_pre_modifiedr
+000099c0: d200 0000 727b 0000 005a 0b54 6172 5f4c  ....r{...Z.Tar_L
+000099d0: 616b 655f 4964 5a0f 756e 7072 6f63 6573  ake_IdZ.unproces
+000099e0: 7365 646d 6173 6b72 2400 0000 7224 0000  sedmaskr$...r$..
+000099f0: 0072 2500 0000 da46 4368 616e 6765 5f41  .r%....FChange_A
+00009a00: 7474 7269 6275 7465 5f56 616c 7565 735f  ttribute_Values_
+00009a10: 466f 725f 4361 7463 686d 656e 7473 5f4e  For_Catchments_N
+00009a20: 6565 645f 546f 5f42 655f 4d65 7267 6564  eed_To_Be_Merged
+00009a30: 5f42 795f 5265 6d6f 7665 5f4e 434c d40a  _By_Remove_NCL..
+00009a40: 0000 73a4 0000 0000 0f04 0108 ff06 0314  ..s.............
+00009a50: 0108 0102 ff04 0304 010a ff08 030c 0108  ................
+00009a60: 0108 0102 0104 020e 0108 0102 ff04 030a  ................
+00009a70: 0104 0104 0204 010a ff08 0314 0102 0114  ................
+00009a80: 0210 0102 ff04 0302 fd04 060a 0104 0104  ................
+00009a90: 010c 0204 0104 010c 0410 0102 ff04 0202  ................
+00009aa0: fe04 030a 0104 0104 010c 0204 0204 010a  ................
+00009ab0: 020e 0102 ff04 0202 fe04 040a 0102 0102  ................
+00009ac0: 0102 0102 0102 0102 0102 0102 f908 0a02  ................
+00009ad0: 0102 0102 0102 0102 0102 0102 0102 f908  ................
+00009ae0: 0a0c 0204 0106 ff10 040e 0272 1301 0000  ...........r....
+00009af0: 6301 0000 0000 0000 0000 0000 0009 0000  c...............
+00009b00: 000a 0000 0043 0000 0073 cc00 0000 6401  .....C...s....d.
+00009b10: 7d01 7c00 6a00 6402 6403 8d01 7d02 7c02  }.|.j.d.d...}.|.
+00009b20: 6401 1900 6a01 7c02 6404 3c00 7c02 6404  d...j.|.d.<.|.d.
+00009b30: 1900 a002 6405 a101 7c02 6404 3c00 7c00  ....d...|.d.<.|.
+00009b40: 6406 1900 6a01 7d03 7c03 7c03 6407 6b04  d...j.}.|.|.d.k.
+00009b50: 1900 7d03 7403 a004 7c03 a101 7d03 7405  ..}.t...|...}.t.
+00009b60: 6407 7406 7c03 8301 8302 4400 5d68 7d04  d.t.|.....D.]h}.
+00009b70: 7c03 7c04 1900 7d05 7c00 6a07 7c00 6406  |.|...}.|.j.|.d.
+00009b80: 1900 7c05 6b02 1900 7d06 7c06 6a08 6408  ..|.k...}.|.j.d.
+00009b90: 6701 6409 640a 8d02 7d06 7c06 7c01 1900  g.d.d...}.|.|...
+00009ba0: 6a01 6407 1900 7d07 7c06 7c01 1900 6a01  j.d...}.|.|...j.
+00009bb0: 7d08 7406 7c08 8301 640b 6b04 725e 7409  }.t.|...d.k.r^t.
+00009bc0: 7c07 7c00 7c02 640b 7c08 7c00 640b 640c  |.|.|.d.|.|.d.d.
+00009bd0: 8d07 7d02 715e 7c02 5300 290d e12c 0100  ..}.q^|.S.)..,..
+00009be0: 0043 6861 6e67 6520 6174 7472 6962 7574  .Change attribut
+00009bf0: 6573 2066 6f72 2063 6174 6368 6d65 6e74  es for catchment
+00009c00: 7320 7468 6174 2063 6f76 6572 6564 2062  s that covered b
+00009c10: 7920 7468 6520 7361 6d65 206c 616b 652e  y the same lake.
+00009c20: 0a20 2020 202d 2d2d 2d2d 2d2d 2d2d 2d0a  .    ----------.
+00009c30: 0a20 2020 204e 6f74 6573 0a20 2020 202d  .    Notes.    -
+00009c40: 2d2d 2d2d 2d2d 0a20 2020 2020 2020 2046  ------.        F
+00009c50: 6f72 2065 7861 6d70 6c65 2c20 6c61 6b65  or example, lake
+00009c60: 2027 6c61 2720 636f 7665 7269 6e67 2063   'la' covering c
+00009c70: 6174 6368 6d65 6e74 2061 2c62 2c63 2e20  atchment a,b,c. 
+00009c80: 7468 6520 6c61 6b65 206f 7574 6c65 7420  the lake outlet 
+00009c90: 6361 7463 686d 656e 740a 2020 2020 2020  catchment.      
+00009ca0: 2020 6973 2061 2e20 7468 656e 2074 6869    is a. then thi
+00009cb0: 7320 6675 6e63 7469 6f6e 2077 696c 6c20  s function will 
+00009cc0: 6368 616e 6765 2061 7474 7269 6275 7465  change attribute
+00009cd0: 206f 6620 6220 616e 6420 6320 746f 2061   of b and c to a
+00009ce0: 2e0a 2020 2020 5265 7475 726e 733a 0a20  ..    Returns:. 
+00009cf0: 2020 202d 2d2d 2d2d 2d2d 0a20 2020 2020     -------.     
+00009d00: 2020 204e 6f6e 652c 0a20 2020 2072 0600     None,.    r..
+00009d10: 0000 5472 0700 0000 727b 0000 0072 0900  ..Tr....r{...r..
+00009d20: 0000 727c 0000 0072 0100 0000 726c 0000  ..r|...r....rl..
+00009d30: 0046 726d 0000 0072 2800 0000 7212 0100  .Frm...r(...r...
+00009d40: 0029 0a72 1400 0000 7213 0000 0072 1600  .).r....r....r..
+00009d50: 0000 721a 0000 0072 2b00 0000 7229 0000  ..r....r+...r)..
+00009d60: 0072 1500 0000 7219 0000 0072 4000 0000  .r....r....r@...
+00009d70: 72aa 0000 00a9 095a 1066 696e 616c 7269  r......Z.finalri
+00009d80: 7670 6c79 5f69 6e66 6f72 a900 0000 7290  vply_infor....r.
+00009d90: 0000 005a 1141 6c6c 436f 6e6e 6563 744c  ...Z.AllConnectL
+00009da0: 616b 6549 4453 7247 0000 005a 066c 616b  akeIDSrG...Z.lak
+00009db0: 6569 645a 0c4c 616b 6573 7562 5f69 6e66  eidZ.Lakesub_inf
+00009dc0: 6f72 f600 0000 5a0a 6c61 6b65 7375 6269  or....Z.lakesubi
+00009dd0: 6473 7224 0000 0072 2400 0000 7225 0000  dsr$...r$...r%..
+00009de0: 00da 3b43 6861 6e67 655f 4174 7472 6962  ..;Change_Attrib
+00009df0: 7574 655f 5661 6c75 6573 5f46 6f72 5f43  ute_Values_For_C
+00009e00: 6174 6368 6d65 6e74 735f 436f 7665 7265  atchments_Covere
+00009e10: 645f 4279 5f53 616d 655f 4c61 6b65 440b  d_By_Same_LakeD.
+00009e20: 0000 7338 0000 0000 0d04 010c 010e 0112  ..s8............
+00009e30: 010a 010c 010a 0312 0108 0112 0104 0106  ................
+00009e40: ff06 0208 0102 ff04 030a 010c 0102 0102  ................
+00009e50: 0102 0102 0102 0102 0102 0102 f908 0972  ...............r
+00009e60: 1601 0000 6303 0000 0000 0000 0000 0000  ....c...........
+00009e70: 0008 0000 0006 0000 0043 0000 0073 6800  .........C...sh.
+00009e80: 0000 7400 7c00 7c01 8302 7d03 7c02 6401  ..t.|.|...}.|.d.
+00009e90: 6b04 7260 7400 7c00 7c02 8302 7d04 7401  k.r`t.|.|...}.t.
+00009ea0: 7402 7c04 8301 8301 4400 5d30 7d05 7c04  t.|.....D.]0}.|.
+00009eb0: 7c05 1900 7c02 6b02 723a 7128 7403 a004  |...|.k.r:q(t...
+00009ec0: 7c03 7c04 7c05 1900 6b02 a101 7d06 7403  |.|.|...k...}.t.
+00009ed0: a005 7c03 7c06 a102 7d03 7128 7c03 7d07  ..|.|...}.q(|.}.
+00009ee0: 6e04 7c03 7d07 7c07 5300 2902 7a95 5265  n.|.}.|.S.).z.Re
+00009ef0: 7475 726e 2073 7562 6964 206f 6620 7375  turn subid of su
+00009f00: 6262 6173 696e 7320 6265 7477 6565 6e20  bbasins between 
+00009f10: 7477 6f20 7375 6269 6420 696e 2074 6865  two subid in the
+00009f20: 2072 6f75 7469 6e67 206e 6574 776f 726b   routing network
+00009f30: 0a20 2020 202d 2d2d 2d2d 2d2d 2d2d 2d0a  .    ----------.
+00009f40: 0a20 2020 204e 6f74 6573 0a20 2020 202d  .    Notes.    -
+00009f50: 2d2d 2d2d 2d2d 0a0a 2020 2020 5265 7475  ------..    Retu
+00009f60: 726e 733a 0a20 2020 202d 2d2d 2d2d 2d2d  rns:.    -------
+00009f70: 0a20 2020 2020 2020 204e 6f6e 652c 0a20  .        None,. 
+00009f80: 2020 2072 0100 0000 2906 7217 0000 0072     r....).r....r
+00009f90: 2900 0000 7215 0000 0072 1a00 0000 72c5  )...r....r....r.
+00009fa0: 0000 00da 0664 656c 6574 6529 0872 6a00  .....delete).rj.
+00009fb0: 0000 5a10 7375 6269 645f 646f 776e 7374  ..Z.subid_downst
+00009fc0: 7265 616d 5a0e 7375 6269 645f 7570 7374  reamZ.subid_upst
+00009fd0: 7265 616d da0c 4879 6472 6f42 6173 696e  ream..HydroBasin
+00009fe0: 7331 5a0c 4879 6472 6f42 6173 696e 7332  s1Z.HydroBasins2
+00009ff0: 7247 0000 00da 0472 6f77 73da 0b48 7964  rG.....rows..Hyd
+0000a000: 726f 4261 7369 6e73 7224 0000 0072 2400  roBasinsr$...r$.
+0000a010: 0000 7225 0000 00da 3552 6574 7572 6e5f  ..r%....5Return_
+0000a020: 5375 6249 6473 5f42 6574 7765 656e 5f54  SubIds_Between_T
+0000a030: 776f 5f53 7562 6261 7369 6e73 5f49 6e5f  wo_Subbasins_In_
+0000a040: 526f 7569 6e67 5f4e 6574 776f 726b 700b  Rouing_Networkp.
+0000a050: 0000 731a 0000 0000 0e02 0104 ff04 0408  ..s.............
+0000a060: 010a 0110 010c 0102 0112 010e 0106 0204  ................
+0000a070: 0272 1b01 0000 6306 0000 0000 0000 0000  .r....c.........
+0000a080: 0000 0020 0000 0008 0000 0043 0000 0073  ... .......C...s
+0000a090: 4404 0000 7c04 6401 6402 6702 1900 a000  D...|.d.d.g.....
+0000a0a0: 6403 a101 6a01 7d06 7402 a003 7c00 7c01  d...j.}.t...|.|.
+0000a0b0: 6602 a101 7d07 7c07 7c07 6400 6400 8502  f...}.|.|.d.d...
+0000a0c0: 6404 6602 1900 a004 a100 1900 7d07 7402  d.f.........}.t.
+0000a0d0: a003 7c02 7c03 6602 a101 7d08 7c08 7c08  ..|.|.f...}.|.|.
+0000a0e0: 6400 6400 8502 6404 6602 1900 a004 a100  d.d...d.f.......
+0000a0f0: 1900 7d08 7402 6a05 7c07 7c08 6405 6406  ..}.t.j.|.|.d.d.
+0000a100: 8d03 7d07 7402 a006 7402 a007 7c07 6400  ..}.t...t...|.d.
+0000a110: 6400 8502 6405 6602 1900 a101 a101 7d09  d...d.f.......}.
+0000a120: 7402 a006 7402 a007 7c07 6400 6400 8502  t...t...|.d.d...
+0000a130: 6407 6602 1900 a101 a101 7d0a 7402 a008  d.f.......}.t...
+0000a140: 7409 7c07 8301 6405 6602 7402 6a0a a102  t.|...d.f.t.j...
+0000a150: 7d0b 740b 6404 7409 7c09 8301 8302 4400  }.t.d.t.|.....D.
+0000a160: 5d40 7d0c 7c09 7c0c 1900 7d0d 7c04 6a0c  ]@}.|.|...}.|.j.
+0000a170: 7c04 6401 1900 7c0d 6b02 1900 6408 1900  |.d...|.k...d...
+0000a180: 6a01 6404 1900 7d0e 7c0e 7c0b 7c07 6400  j.d...}.|.|.|.d.
+0000a190: 6400 8502 6405 6602 1900 7c0d 6b02 3c00  d...d.f...|.k.<.
+0000a1a0: 71cc 7402 6a05 7c07 7c0b 6405 6406 8d03  q.t.j.|.|.d.d...
+0000a1b0: 7d07 6700 7d0f 6700 7d10 6700 7d11 740b  }.g.}.g.}.g.}.t.
+0000a1c0: 6404 7409 7c0a 8301 8302 4400 9002 5de6  d.t.|.....D...].
+0000a1d0: 7d0c 7c0a 7c0c 1900 7d03 7c07 7c07 6400  }.|.|...}.|.|.d.
+0000a1e0: 6400 8502 6407 6602 1900 7c03 6b02 1900  d...d.f...|.k...
+0000a1f0: 7d12 7c12 7c12 6400 6400 8502 6409 6602  }.|.|.d.d...d.f.
+0000a200: 1900 a004 a100 1900 7d12 7c12 7409 7c12  ........}.|.t.|.
+0000a210: 8301 6405 1800 6405 6602 1900 7d13 7c04  ..d...d.f...}.|.
+0000a220: 6a0c 7c04 6401 1900 a00d 7c12 6400 6400  j.|.d.....|.d.d.
+0000a230: 8502 6405 6602 1900 a101 1900 7d14 7409  ..d.f.......}.t.
+0000a240: 7c12 8301 6405 6b02 9002 720c 7c12 640a  |...d.k...r.|.d.
+0000a250: 1900 7d15 7c05 6a0c 7c05 640b 1900 7c15  ..}.|.j.|.d...|.
+0000a260: 6b02 1900 640c 1900 6a01 6404 1900 7c03  k...d...j.d...|.
+0000a270: 6b03 9001 72f6 7c10 a005 740e 7c12 640a  k...r.|...t.|.d.
+0000a280: 1900 8301 a101 0100 6e12 7c0f a005 740e  ........n.|...t.
+0000a290: 7c12 640d 1900 8301 a101 0100 9001 7138  |.d...........q8
+0000a2a0: 740f 7c06 7c13 8302 7d16 7402 a006 7c12  t.|.|...}.t...|.
+0000a2b0: 6400 6400 8502 6405 6602 1900 a101 7d17  d.d...d.f.....}.
+0000a2c0: 740b 6404 7409 7c12 8301 8302 4400 9001  t.d.t.|.....D...
+0000a2d0: 5de0 7d18 7c12 7c18 6405 6602 1900 7d15  ].}.|.|.d.f...}.
+0000a2e0: 7c15 7c13 6b03 9003 7266 7c11 a005 740e  |.|.k...rf|...t.
+0000a2f0: 7c12 7c18 6405 6602 1900 8301 a101 0100  |.|.d.f.........
+0000a300: 7409 7c04 6a0c 7c04 6401 1900 7c15 6b02  t.|.j.|.d...|.k.
+0000a310: 1900 8301 6404 6b04 9003 7266 7c04 6a0c  ....d.k...rf|.j.
+0000a320: 7c04 6401 1900 7c15 6b02 1900 6402 1900  |.d...|.k...d...
+0000a330: 6a01 6404 1900 7d19 7c19 7c16 7600 9003  j.d...}.|.|.v...
+0000a340: 7266 7c19 7c12 6400 6400 8502 6405 6602  rf|.|.d.d...d.f.
+0000a350: 1900 7601 9003 7266 7c11 a005 740e 7c19  ..v...rf|...t.|.
+0000a360: 8301 a101 0100 7c19 7d1a 6404 7d1b 7c1b  ......|.}.d.}.|.
+0000a370: 640e 6b00 9003 7266 7c1b 6405 1700 7d1b  d.k...rf|.d...}.
+0000a380: 7409 7c04 6a0c 7c04 6401 1900 7c1a 6b02  t.|.j.|.d...|.k.
+0000a390: 1900 8301 6404 6b04 9003 7266 7c04 6a0c  ....d.k...rf|.j.
+0000a3a0: 7c04 6401 1900 7c1a 6b02 1900 6402 1900  |.d...|.k...d...
+0000a3b0: 6a01 6404 1900 7d1c 7c1c 7c12 6400 6400  j.d...}.|.|.d.d.
+0000a3c0: 8502 6405 6602 1900 7601 9003 7266 7c1c  ..d.f...v...rf|.
+0000a3d0: 7c16 7600 9003 7266 7c11 a005 740e 7c1c  |.v...rf|...t.|.
+0000a3e0: 8301 a101 0100 7c1c 7d1a 6e04 9003 7166  ......|.}.n...qf
+0000a3f0: 6e04 9003 7166 9002 71da 740f 7c06 7c15  n...qf..q.t.|.|.
+0000a400: 8302 7d1d 7409 7c1d 8301 6404 6b04 9003  ..}.t.|...d.k...
+0000a410: 72a4 7402 a00d 7c1d 7c17 a102 7d1e 7410  r.t...|.|...}.t.
+0000a420: 7c1e 8301 640f 6b05 9003 729e 6410 7d1f  |...d.k...r.d.}.
+0000a430: 6e04 6411 7d1f 6e04 6411 7d1f 7409 7c14  n.d.}.n.d.}.t.|.
+0000a440: 6a0c 7c14 6402 1900 7c15 6b02 1900 8301  j.|.d...|.k.....
+0000a450: 6404 6b04 9003 73ec 7c05 6a0c 7c05 640b  d.k...s.|.j.|.d.
+0000a460: 1900 7c15 6b02 1900 640c 1900 6a01 6404  ..|.k...d...j.d.
+0000a470: 1900 7c03 6b02 9003 73ec 7c1f 9004 7204  ..|.k...s.|...r.
+0000a480: 7c0f a005 740e 7c12 7c18 6404 6602 1900  |...t.|.|.d.f...
+0000a490: 8301 a101 0100 6e16 7c10 a005 740e 7c12  ......n.|...t.|.
+0000a4a0: 7c18 6405 6602 1900 8301 a101 0100 9002  |.d.f...........
+0000a4b0: 713a 9001 7138 7411 7412 7c11 8301 8301  q:..q8t.t.|.....
+0000a4c0: 7411 7412 7c0f 8301 8301 7411 7412 7c10  t.t.|.....t.t.|.
+0000a4d0: 8301 8301 6603 5300 2912 4e72 0600 0000  ....f.S.).Nr....
+0000a4e0: 720d 0000 0072 2d00 0000 7201 0000 0072  r....r-...r....r
+0000a4f0: 2800 0000 720e 0000 0072 ec00 0000 da0a  (...r....r......
+0000a500: 4d61 7841 6363 5f63 6174 e904 0000 0029  MaxAcc_cat.....)
+0000a510: 0272 0100 0000 7228 0000 00da 0849 4c5f  .r....r(.....IL_
+0000a520: 5375 6249 64da 0873 6c5f 636c 5f69 6429  SubId..sl_cl_id)
+0000a530: 0272 0100 0000 7201 0000 0072 6e00 0000  .r....r....rn...
+0000a540: 7262 0000 0054 4629 1372 1600 0000 7213  rb...TF).r....r.
+0000a550: 0000 0072 1a00 0000 da0c 636f 6c75 6d6e  ...r......column
+0000a560: 5f73 7461 636b da07 6172 6773 6f72 7472  _stack..argsortr
+0000a570: 4d00 0000 722b 0000 0072 0701 0000 7271  M...r+...r....rq
+0000a580: 0000 0072 1500 0000 72dd 0000 0072 2900  ...r....r....r).
+0000a590: 0000 7219 0000 0072 1200 0000 722d 0000  ..r....r....r-..
+0000a5a0: 0072 1700 0000 723e 0000 0072 5300 0000  .r....r>...rS...
+0000a5b0: 72d5 0000 0029 205a 0b72 6976 5f6c 616b  r....) Z.riv_lak
+0000a5c0: 655f 6964 5a06 7374 725f 6964 5a0c 7269  e_idZ.str_idZ.ri
+0000a5d0: 765f 6c61 6b65 5f69 6432 5a05 636c 5f69  v_lake_id2Z.cl_i
+0000a5e0: 6472 6a00 0000 da13 7374 725f 7374 6172  drj.....str_star
+0000a5f0: 745f 7074 5f6c 616b 6569 645a 1172 6f75  t_pt_lakeidZ.rou
+0000a600: 7469 6e67 5f69 6e66 6f5f 726f 7574 5a08  ting_info_routZ.
+0000a610: 7269 765f 6c61 6b65 5a0b 7269 765f 6c61  riv_lakeZ.riv_la
+0000a620: 6b65 5f63 6c5a 0d73 7472 5f69 645f 756e  ke_clZ.str_id_un
+0000a630: 6971 7565 5a0c 636c 5f69 645f 756e 6971  iqueZ.cl_id_uniq
+0000a640: 7565 5a0a 6163 635f 7374 725f 636c 7247  ueZ.acc_str_clrG
+0000a650: 0000 00da 0573 7472 6964 da06 6d61 7861  .....strid..maxa
+0000a660: 6363 da14 6e6f 6e5f 6c61 6b65 5f69 6e66  cc..non_lake_inf
+0000a670: 6c6f 775f 7365 6773 da12 7374 725f 6964  low_segs..str_id
+0000a680: 5f6c 616b 655f 696e 6c66 6f77 da13 7374  _lake_inlfow..st
+0000a690: 725f 6964 5f77 6974 6869 6e5f 6c61 6b65  r_id_within_lake
+0000a6a0: 735a 0b72 6976 5f6c 616b 655f 696c 5a0a  sZ.riv_lake_ilZ.
+0000a6b0: 6f75 746c 6574 5f73 7472 5a10 7375 625f  outlet_strZ.sub_
+0000a6c0: 726f 7574 696e 675f 696e 666f 5a0b 7374  routing_infoZ.st
+0000a6d0: 725f 6964 5f63 6c5f 6a5a 1373 7472 735f  r_id_cl_jZ.strs_
+0000a6e0: 746f 5f6c 616b 655f 6f75 746c 6574 5a18  to_lake_outletZ.
+0000a6f0: 756e 6971 7565 5f73 7472 5f69 645f 6376  unique_str_id_cv
+0000a700: 5f62 795f 6c61 6b65 725b 0000 005a 1a64  _by_laker[...Z.d
+0000a710: 6f77 6e5f 7375 6e5f 6f66 5f6c 616b 655f  own_sun_of_lake_
+0000a720: 636f 7665 725f 7374 725a 0663 7374 7269  cover_strZ.cstri
+0000a730: 645a 036b 5f64 5a07 6473 7472 5f69 645a  dZ.k_dZ.dstr_idZ
+0000a740: 0b75 705f 7374 725f 636c 5f6a 7223 0000  .up_str_cl_jr#..
+0000a750: 005a 1168 6173 5f75 705f 7374 725f 696e  .Z.has_up_str_in
+0000a760: 6c61 6b65 7224 0000 0072 2400 0000 7225  laker$...r$...r%
+0000a770: 0000 00da 3172 6574 7572 6e5f 6e6f 6e5f  ....1return_non_
+0000a780: 6c61 6b65 5f69 6e66 6c6f 775f 7365 6773  lake_inflow_segs
+0000a790: 5f61 6e64 5f73 6567 735f 7769 7468 696e  _and_segs_within
+0000a7a0: 5f6c 616b 6573 900b 0000 73d2 0000 0000  _lakes....s.....
+0000a7b0: 0402 0104 ff06 0102 ff06 030e 0118 010e  ................
+0000a7c0: 0118 0110 031c 011c 0216 0112 0108 0316  ................
+0000a7d0: 0102 ff04 031a 0110 0504 0104 0104 0114  ................
+0000a7e0: 0208 0218 0118 0114 0104 0118 ff04 050e  ................
+0000a7f0: 0108 0310 0102 ff04 0202 fe02 0302 fd02  ................
+0000a800: ff04 0614 0212 0104 020a 0716 0214 010c  ................
+0000a810: 030a 0116 021c 020a 0102 ff04 0102 ff04  ................
+0000a820: 0102 ff04 0420 0304 0106 ff04 0304 0104  ..... ..........
+0000a830: 010a 0108 011c 010a 0102 ff04 0102 ff04  ................
+0000a840: 0102 ff04 0320 010e 0106 0206 0208 030a  ..... ..........
+0000a850: 020e 040c 010e 0106 0206 0204 0314 0102  ................
+0000a860: ff02 ff04 0304 010a ff02 0202 fe04 0202  ................
+0000a870: fe02 0302 fd02 fd04 0702 f904 0b18 021e  ................
+0000a880: 0272 2801 0000 6303 0000 0000 0000 0000  .r(...c.........
+0000a890: 0000 0015 0000 0006 0000 0043 0000 0073  ...........C...s
+0000a8a0: d801 0000 6700 7d03 6700 7d04 7400 a001  ....g.}.g.}.t...
+0000a8b0: 7c00 7c01 6602 a101 7d05 7400 a002 7400  |.|.f...}.t...t.
+0000a8c0: a003 7c01 a101 a101 7d06 7400 a002 7400  ..|.....}.t...t.
+0000a8d0: a003 7c00 a101 a101 7d07 7400 a004 7405  ..|.....}.t...t.
+0000a8e0: 7c05 8301 6401 6602 7400 6a06 a102 7d08  |...d.f.t.j...}.
+0000a8f0: 7407 6402 7405 7c06 8301 8302 4400 5d40  t.d.t.|.....D.]@
+0000a900: 7d09 7c06 7c09 1900 7d0a 7c02 6a08 7c02  }.|.|...}.|.j.|.
+0000a910: 6403 1900 7c0a 6b02 1900 6404 1900 6a09  d...|.k...d...j.
+0000a920: 6402 1900 7d0b 7c0b 7c08 7c05 6400 6400  d...}.|.|.|.d.d.
+0000a930: 8502 6401 6602 1900 7c0a 6b02 3c00 715a  ..d.f...|.k.<.qZ
+0000a940: 7400 6a0a 7c05 7c08 6401 6405 8d03 7d05  t.j.|.|.d.d...}.
+0000a950: 7c05 7c05 6400 6400 8502 6406 6602 1900  |.|.d.d...d.f...
+0000a960: a00b a100 1900 7d05 7c02 6403 6407 6702  ......}.|.d.d.g.
+0000a970: 1900 a00c 6408 a101 6a09 7d0c 7407 6402  ....d...j.}.t.d.
+0000a980: 7405 7c07 8301 8302 4400 5de8 7d09 7c07  t.|.....D.].}.|.
+0000a990: 7c09 1900 7d0d 7c05 7c05 6400 6400 8502  |...}.|.|.d.d...
+0000a9a0: 6402 6602 1900 7c0d 6b02 1900 7d0e 7405  d.f...|.k...}.t.
+0000a9b0: 7c0e 8301 6401 6b01 9001 721a 71e6 7c0e  |...d.k...r.q.|.
+0000a9c0: 7405 7c0e 8301 6401 1800 6401 6602 1900  t.|...d...d.f...
+0000a9d0: 7d0f 740d 7c0c 7c0f 8302 7d10 7400 a00e  }.t.|.|...}.t...
+0000a9e0: 7c0e 6400 6400 8502 6401 6602 1900 7c10  |.d.d...d.f...|.
+0000a9f0: a102 7d11 6700 7d12 7405 7c11 7c11 6409  ..}.g.}.t.|.|.d.
+0000aa00: 6b02 1900 8301 7405 7c0e 6400 6400 8502  k.....t.|.d.d...
+0000aa10: 6401 6602 1900 8301 6b00 72e6 7c0e 7400  d.f.....k.r.|.t.
+0000aa20: a00f 7c11 a101 6401 6602 1900 7d13 7407  ..|...d.f...}.t.
+0000aa30: 6402 7405 7c13 8301 8302 4400 5d22 7d14  d.t.|.....D.]"}.
+0000aa40: 7c13 7c14 1900 7d0a 7c0a 7c0f 6b03 9001  |.|...}.|.|.k...
+0000aa50: 7298 7c12 a00a 7c0a a101 0100 9001 7198  r.|...|.......q.
+0000aa60: 7c04 7c12 1700 7d04 7c03 a00a 7c0d a101  |.|...}.|...|...
+0000aa70: 0100 71e6 7c03 7c04 6602 5300 290a 4e72  ..q.|.|.f.S.).Nr
+0000aa80: 2800 0000 7201 0000 0072 0600 0000 721c  (...r....r....r.
+0000aa90: 0100 0072 0e00 0000 7262 0000 0072 0d00  ...r....rb...r..
+0000aaa0: 0000 722d 0000 0054 2910 721a 0000 0072  ..r-...T).r....r
+0000aab0: 2001 0000 722b 0000 0072 0701 0000 7271   ...r+...r....rq
+0000aac0: 0000 0072 1500 0000 72dd 0000 0072 2900  ...r....r....r).
+0000aad0: 0000 7219 0000 0072 1300 0000 724d 0000  ..r....r....rM..
+0000aae0: 0072 2101 0000 7216 0000 0072 1700 0000  .r!...r....r....
+0000aaf0: 7212 0000 0072 a300 0000 2915 da05 434c  r....r....)...CL
+0000ab00: 5f49 64da 0653 7472 5f49 645a 0c52 6f75  _Id..Str_IdZ.Rou
+0000ab10: 7469 6e67 5f69 6e66 6fda 174c 616b 6573  ting_info..Lakes
+0000ab20: 5f57 4974 685f 4d75 6c74 695f 4f75 746c  _WIth_Multi_Outl
+0000ab30: 6574 da0a 5265 6d6f 7665 5f53 7472 5a06  et..Remove_StrZ.
+0000ab40: 434c 5f53 7472 5a0d 5374 725f 4964 5f75  CL_StrZ.Str_Id_u
+0000ab50: 6e69 7175 655a 0c43 4c5f 4964 5f75 6e69  niqueZ.CL_Id_uni
+0000ab60: 7175 655a 0a41 6363 5f53 7472 5f43 4c72  queZ.Acc_Str_CLr
+0000ab70: 4700 0000 7223 0100 0072 2401 0000 5a11  G...r#...r$...Z.
+0000ab80: 726f 7574 696e 675f 696e 666f 5f6f 6e6c  routing_info_onl
+0000ab90: 795a 076c 616b 655f 6964 5a08 695f 434c  yZ.lake_idZ.i_CL
+0000aba0: 5f53 7472 5a0b 7374 725f 6d61 785f 6163  _StrZ.str_max_ac
+0000abb0: 635a 1273 7472 5f74 6f5f 7374 725f 6d61  cZ.str_to_str_ma
+0000abc0: 785f 6163 6372 2300 0000 5a0c 5265 6d6f  x_accr#...Z.Remo
+0000abd0: 7665 5f53 7472 5f69 5a18 7374 725f 6e6f  ve_Str_iZ.str_no
+0000abe0: 7466 6c6f 7774 6f5f 6c61 6b65 6f75 746c  tflowto_lakeoutl
+0000abf0: 6574 5a04 6973 7472 7224 0000 0072 2400  etZ.istrr$...r$.
+0000ac00: 0000 7225 0000 00da 1f43 6865 636b 5f49  ..r%.....Check_I
+0000ac10: 665f 4c61 6b65 5f48 6176 655f 4d75 6c74  f_Lake_Have_Mult
+0000ac20: 695f 4f75 744c 6574 190c 0000 734a 0000  i_OutLet....sJ..
+0000ac30: 0000 0304 0104 020e 0210 0210 0316 0112  ................
+0000ac40: 0108 0116 0102 ff04 031a 0110 0318 0302  ................
+0000ac50: 0104 ff06 0102 ff06 0412 0208 0218 030e  ................
+0000ac60: 0102 0814 030a 0818 0404 0324 0212 0212  ...........$....
+0000ac70: 0208 050a 010e 0508 010c 0272 2d01 0000  ...........r-...
+0000ac80: 6301 0000 0000 0000 0000 0000 0009 0000  c...............
+0000ac90: 000a 0000 0043 0000 0073 ba00 0000 6401  .....C...s....d.
+0000aca0: 7d01 7c00 6a00 6402 6403 8d01 7d02 7c02  }.|.j.d.d...}.|.
+0000acb0: 6401 1900 6a01 7c02 6404 3c00 7c00 6405  d...j.|.d.<.|.d.
+0000acc0: 1900 6a01 7d03 7c03 7c03 6406 6b04 1900  ..j.}.|.|.d.k...
+0000acd0: 7d03 7402 a003 7c03 a101 7d03 7404 6406  }.t...|...}.t.d.
+0000ace0: 7405 7c03 8301 8302 4400 5d68 7d04 7c03  t.|.....D.]h}.|.
+0000acf0: 7c04 1900 7d05 7c00 6a06 7c00 6405 1900  |...}.|.j.|.d...
+0000ad00: 7c05 6b02 1900 7d06 7c06 6a07 6407 6701  |.k...}.|.j.d.g.
+0000ad10: 6408 6409 8d02 7d06 7c06 7c01 1900 6a01  d.d...}.|.|...j.
+0000ad20: 6406 1900 7d07 7c06 7c01 1900 6a01 7d08  d...}.|.|...j.}.
+0000ad30: 7405 7c08 8301 640a 6b04 724c 7408 7c07  t.|...d.k.rLt.|.
+0000ad40: 7c00 7c02 640a 7c08 7c00 640a 640b 8d07  |.|.d.|.|.d.d...
+0000ad50: 7d02 714c 7c02 5300 290c 7214 0100 0072  }.qL|.S.).r....r
+0000ad60: 0600 0000 5472 0700 0000 727b 0000 0072  ....Tr....r{...r
+0000ad70: 7c00 0000 7201 0000 0072 6c00 0000 4672  |...r....rl...Fr
+0000ad80: 6d00 0000 7228 0000 0072 1201 0000 2909  m...r(...r....).
+0000ad90: 7214 0000 0072 1300 0000 721a 0000 0072  r....r....r....r
+0000ada0: 2b00 0000 7229 0000 0072 1500 0000 7219  +...r)...r....r.
+0000adb0: 0000 0072 4000 0000 72aa 0000 0072 1501  ...r@...r....r..
+0000adc0: 0000 7224 0000 0072 2400 0000 7225 0000  ..r$...r$...r%..
+0000add0: 00da 3b63 6861 6e67 655f 6174 7472 6962  ..;change_attrib
+0000ade0: 7574 655f 7661 6c75 6573 5f66 6f72 5f63  ute_values_for_c
+0000adf0: 6174 6368 6d65 6e74 735f 636f 7665 7265  atchments_covere
+0000ae00: 645f 6279 5f73 616d 655f 6c61 6b65 700c  d_by_same_lakep.
+0000ae10: 0000 7336 0000 0000 0d04 010c 010e 010a  ..s6............
+0000ae20: 010c 010a 0312 0108 0112 0104 0106 ff06  ................
+0000ae30: 0208 0102 ff04 030a 010c 0102 0102 0102  ................
+0000ae40: 0102 0102 0102 0102 0102 f908 0972 2e01  .............r..
+0000ae50: 0000 6303 0000 0000 0000 0000 0000 000d  ..c.............
+0000ae60: 0000 0005 0000 0043 0000 0073 2c02 0000  .......C...s,...
+0000ae70: 7c00 6a00 7d03 7c02 6401 6b04 9001 7260  |.j.}.|.d.k...r`
+0000ae80: 7401 6401 7402 7c03 8301 8302 4400 5ddc  t.d.t.|.....D.].
+0000ae90: 7d04 7c00 6a03 7c03 7c04 1900 6402 6602  }.|.j.|.|...d.f.
+0000aea0: 1900 7d05 7c00 6a03 7c03 7c04 1900 6403  ..}.|.j.|.|...d.
+0000aeb0: 6602 1900 7d06 7c00 6a03 7c03 7c04 1900  f...}.|.j.|.|...
+0000aec0: 6404 6602 1900 7d07 7c00 6a03 7c00 6403  d.f...}.|.j.|.d.
+0000aed0: 1900 7c07 6b02 1900 a004 a100 7d08 7402  ..|.k.......}.t.
+0000aee0: 7c08 8301 6401 6b04 7298 7c08 6402 1900  |...d.k.r.|.d...
+0000aef0: 6a05 6401 1900 7c00 6a03 7c03 7c04 1900  j.d...|.j.|.|...
+0000af00: 6405 6602 3c00 6e12 6406 7c00 6a03 7c03  d.f.<.n.d.|.j.|.
+0000af10: 7c04 1900 6405 6602 3c00 7c05 7c00 6a03  |...d.f.<.|.|.j.
+0000af20: 7c03 7c04 1900 6405 6602 1900 6b02 72d2  |.|...d.f...k.r.
+0000af30: 6406 7c00 6a03 7c03 7c04 1900 6405 6602  d.|.j.|.|...d.f.
+0000af40: 3c00 7c05 7c00 6a03 7c03 7c04 1900 6405  <.|.|.j.|.|...d.
+0000af50: 6602 1900 6b02 721e 6406 7c00 6a03 7c03  f...k.r.d.|.j.|.
+0000af60: 7c04 1900 6405 6602 3c00 711e 7c00 6403  |...d.f.<.q.|.d.
+0000af70: 1900 6a05 7c00 6407 3c00 7c00 6404 1900  ..j.|.d.<.|.d...
+0000af80: 6a05 7c00 6408 3c00 7c00 6402 1900 6a05  j.|.d.<.|.d...j.
+0000af90: 7c00 6403 3c00 7c00 6405 1900 6a05 7c00  |.d.<.|.d...j.|.
+0000afa0: 6404 3c00 7c00 7c00 6409 1900 640a 6b03  d.<.|.|.d...d.k.
+0000afb0: 1900 6a04 640b 640c 8d01 7d09 7c00 6403  ..j.d.d...}.|.d.
+0000afc0: 1900 a006 7c09 6404 1900 a101 0f00 7d0a  ....|.d.......}.
+0000afd0: 7c01 6401 6b00 9001 726e 7c00 5300 7c00  |.d.k...rn|.S.|.
+0000afe0: 6a07 6403 640d 640e 8d02 7d0b 7408 7c0b  j.d.d.d...}.t.|.
+0000aff0: 8301 7d0b 7401 6401 7402 7c0b 8301 8302  ..}.t.d.t.|.....
+0000b000: 4400 5d94 7d04 7c0b 6403 1900 6a05 7c04  D.].}.|.d...j.|.
+0000b010: 1900 7d0c 7c0b 640f 1900 6a05 7c04 1900  ..}.|.d...j.|...
+0000b020: 7c00 6a03 7c00 6403 1900 7c0c 6b02 640f  |.j.|.d...|.k.d.
+0000b030: 6602 3c00 7c0b 6410 1900 6a05 7c04 1900  f.<.|.d...j.|...
+0000b040: 7c00 6a03 7c00 6403 1900 7c0c 6b02 6410  |.j.|.d...|.k.d.
+0000b050: 6602 3c00 7c0b 6411 1900 6a05 7c04 1900  f.<.|.d...j.|...
+0000b060: 7c00 6a03 7c00 6403 1900 7c0c 6b02 6411  |.j.|.d...|.k.d.
+0000b070: 6602 3c00 7c0b 6412 1900 6a05 7c04 1900  f.<.|.d...j.|...
+0000b080: 7c00 6a03 7c00 6403 1900 7c0c 6b02 6412  |.j.|.d...|.k.d.
+0000b090: 6602 3c00 9001 7192 7c00 5300 2913 72b0  f.<...q.|.S.).r.
+0000b0a0: 0000 0072 0100 0000 727b 0000 0072 0600  ...r....r{...r..
+0000b0b0: 0000 720d 0000 0072 8800 0000 7266 0000  ..r....r....rf..
+0000b0c0: 0072 8900 0000 728a 0000 0072 6100 0000  .r....r....ra...
+0000b0d0: 7262 0000 0054 7207 0000 0072 3900 0000  rb...Tr....r9...
+0000b0e0: 72b1 0000 0072 6400 0000 7263 0000 0072  r....rd...rc...r
+0000b0f0: 6500 0000 726c 0000 0029 0972 5800 0000  e...rl...).rX...
+0000b100: 7229 0000 0072 1500 0000 7219 0000 0072  r)...r....r....r
+0000b110: 1400 0000 7213 0000 0072 1200 0000 7241  ....r....r....rA
+0000b120: 0000 0072 b200 0000 290d 7290 0000 0072  ...r....).r....r
+0000b130: b300 0000 72b4 0000 0072 5c00 0000 7247  ....r....r\...rG
+0000b140: 0000 0072 7b00 0000 7248 0000 0072 b500  ...r{...rH...r..
+0000b150: 0000 72b6 0000 00da 1972 6976 5f70 645f  ..r......riv_pd_
+0000b160: 6e6e 636c 735f 726f 7574 696e 675f 696e  nncls_routing_in
+0000b170: 666f 7223 0000 0072 b700 0000 72b8 0000  for#...r....r...
+0000b180: 0072 2400 0000 7224 0000 0072 2500 0000  .r$...r$...r%...
+0000b190: 7222 0000 009b 0c00 0073 6e00 0000 000d  r".......sn.....
+0000b1a0: 0602 0a01 1201 1201 1201 1202 0401 0aff  ................
+0000b1b0: 0804 0c01 0201 02ff 0402 02fe 1404 1202  ................
+0000b1c0: 1601 1202 1601 1402 0e01 0e01 0e02 0e02  ................
+0000b1d0: 1001 02ff 0602 0801 06ff 060d 0a01 0402  ................
+0000b1e0: 0401 04ff 0603 0802 1201 0e03 0cfe 0401  ................
+0000b1f0: 0eff 0205 0cfe 0401 0eff 0205 0cfe 0401  ................
+0000b200: 0eff 0205 0cfe 0401 0eff 0604 7222 0000  ............r"..
+0000b210: 0063 0300 0000 0000 0000 0000 0000 0300  .c..............
+0000b220: 0000 0300 0000 4300 0000 730c 0000 007c  ......C...s....|
+0000b230: 017c 007c 0213 0014 0053 0029 014e 7224  .|.|.....S.).Nr$
+0000b240: 0000 0029 03da 0141 725e 0000 0072 d600  ...)...Ar^...r..
+0000b250: 0000 7224 0000 0072 2400 0000 7225 0000  ..r$...r$...r%..
+0000b260: 00da 0966 756e 635f 515f 4441 f00c 0000  ...func_Q_DA....
+0000b270: 7302 0000 0000 0172 3101 0000 6301 0000  s......r1...c...
+0000b280: 0000 0000 0000 0000 0003 0000 0008 0000  ................
+0000b290: 0043 0000 0073 6400 0000 7a2c 7400 7401  .C...sd...z,t.t.
+0000b2a0: 7c00 6400 6400 8502 6401 6602 1900 7c00  |.d.d...d.f...|.
+0000b2b0: 6400 6400 8502 6402 6602 1900 8303 5c02  d.d...d.f.....\.
+0000b2c0: 7d01 7d02 5700 6e26 0400 7402 7952 0100  }.}.W.n&..t.yR..
+0000b2d0: 0100 0100 7403 6403 8301 0100 7404 a005  ....t.d.....t...
+0000b2e0: 6404 6405 a102 7d01 5900 6e02 3000 7c01  d.d...}.Y.n.0.|.
+0000b2f0: 6401 1900 7c01 6402 1900 6602 5300 2906  d...|.d...f.S.).
+0000b300: 4e72 0100 0000 7228 0000 007a 3723 2323  Nr....r(...z7###
+0000b310: 2323 2323 2323 2323 2323 2323 2323 2323  ################
+0000b320: 2323 2323 2323 2323 2323 2323 2323 2323  ################
+0000b330: 2323 2323 2323 2323 2323 2323 2323 2323  ################
+0000b340: 2323 2323 7262 0000 0072 6600 0000 2906  ####rb...rf...).
+0000b350: 7202 0000 0072 3101 0000 da0c 5275 6e74  r....r1.....Runt
+0000b360: 696d 6545 7272 6f72 7268 0000 0072 1a00  imeErrorrh...r..
+0000b370: 0000 7271 0000 0029 035a 0464 615f 715a  ..rq...).Z.da_qZ
+0000b380: 0570 6f70 7432 5a05 7063 6f76 3272 2400  .popt2Z.pcov2r$.
+0000b390: 0000 7224 0000 0072 2500 0000 da23 7265  ..r$...r%....#re
+0000b3a0: 7475 726e 5f6b 5f61 6e64 5f63 5f69 6e5f  turn_k_and_c_in_
+0000b3b0: 715f 6461 5f72 656c 6174 696f 6e73 6869  q_da_relationshi
+0000b3c0: 70f4 0c00 0073 0c00 0000 0002 0201 2c01  p....s........,.
+0000b3d0: 0c01 0801 1202 7233 0100 0063 0400 0000  ......r3...c....
+0000b3e0: 0000 0000 0000 0000 0d00 0000 0500 0000  ................
+0000b3f0: 4300 0000 73c2 0000 0064 017d 047c 047c  C...s....d.}.|.|
+0000b400: 0114 007d 0564 027d 067c 0064 017c 0514  ...}.d.}.|.d.|..
+0000b410: 0018 007d 077c 0764 036b 0072 4464 047c  ...}.|.d.k.rDd.|
+0000b420: 0014 007d 0764 057c 0014 007d 057c 007c  ...}.d.|...}.|.|
+0000b430: 0718 0064 011b 007c 011b 007d 047c 077c  ...d...|...}.|.|
+0000b440: 0114 0064 017c 0414 007c 0114 007c 0114  ...d.|...|...|..
+0000b450: 0064 011b 0017 007d 087c 0764 017c 0114  .d.....}.|.d.|..
+0000b460: 0064 067c 0464 0113 0017 0064 0413 0014  .d.|.d.....d....
+0000b470: 0017 007d 0974 007c 0883 0174 007c 0983  ...}.t.|...t.|..
+0000b480: 011b 007d 0a74 007c 0283 0174 007c 0883  ...}.t.|...t.|..
+0000b490: 011b 007d 0b7c 0b64 036b 0472 ba7c 0a64  ...}.|.d.k.r.|.d
+0000b4a0: 0713 007c 0364 0413 0014 007c 0b1b 007d  ...|.d.....|...}
+0000b4b0: 0c6e 0464 087d 0c7c 0c53 0029 094e 7262  .n.d.}.|.S.).Nrb
+0000b4c0: 0000 007a 0a20 2020 2020 2020 2020 2072  ...z.          r
+0000b4d0: 0100 0000 72ba 0000 0067 0000 0000 0000  ....r....g......
+0000b4e0: d03f 7228 0000 0067 5555 5555 5555 e53f  .?r(...gUUUUUU.?
+0000b4f0: 72a0 0000 0029 0172 6000 0000 290d da05  r....).r`...)...
+0000b500: 7769 6474 68da 0564 6570 7468 da01 51da  width..depth..Q.
+0000b510: 0573 6c6f 7065 5a03 7a63 685a 0573 6964  .slopeZ.zchZ.sid
+0000b520: 7764 da03 7461 625a 0562 6f74 7764 5a03  wd..tabZ.botwdZ.
+0000b530: 4163 685a 0350 6368 5a03 5263 68da 0156  AchZ.PchZ.Rch..V
+0000b540: da01 6e72 2400 0000 7224 0000 0072 2500  ..nr$...r$...r%.
+0000b550: 0000 da11 6361 6c63 756c 6174 6543 6861  ....calculateCha
+0000b560: 6e6e 616c 6eff 0c00 0073 2000 0000 0001  nnaln....s .....
+0000b570: 0401 0801 0401 0c01 0801 0801 0801 1001  ................
+0000b580: 1c07 1c01 1001 1001 0801 1602 0401 723b  ..............r;
+0000b590: 0100 00fa 0123 6303 0000 0000 0000 0000  .....#c.........
+0000b5a0: 0000 0010 0000 0007 0000 0043 0000 0073  ...........C...s
+0000b5b0: c801 0000 7c01 6401 6b00 720c 7c00 5300  ....|.d.k.r.|.S.
+0000b5c0: 7c00 6402 6403 6702 1900 a000 6404 a101  |.d.d.g.....d...
+0000b5d0: 6a01 7d03 6405 7d04 6405 7c00 6a02 7601  j.}.d.}.d.|.j.v.
+0000b5e0: 7232 6406 7d04 7c02 6407 6b03 9001 7264  r2d.}.|.d.k...rd
+0000b5f0: 7403 7c02 8301 6408 1900 6a01 7d05 7404  t.|...d...j.}.t.
+0000b600: a005 7c05 a101 7d06 7c06 7c06 6401 6b04  ..|...}.|.|.d.k.
+0000b610: 1900 7d06 7c00 6a06 7c00 7c04 1900 a007  ..}.|.j.|.|.....
+0000b620: 7c06 a101 1900 7d07 6409 7d08 7c01 6401  |.....}.d.}.|.d.
+0000b630: 6b00 728c 7408 640a 8301 0100 7c00 5300  k.r.t.d.....|.S.
+0000b640: 7c00 6a06 7c00 7c04 1900 7c01 6b02 1900  |.j.|.|...|.k...
+0000b650: 7d09 7409 7c09 8301 6401 6b04 72ba 7c09  }.t.|...d.k.r.|.
+0000b660: 6402 1900 6a01 6401 1900 7d08 6e0e 7408  d...j.d...}.n.t.
+0000b670: 640b 7c09 8302 0100 7c00 5300 740a 7c03  d.|.....|.S.t.|.
+0000b680: 7c08 8302 7d0a 7409 7c07 8301 640c 6b05  |...}.t.|...d.k.
+0000b690: 9001 7248 740b 6401 7409 7c07 8301 8302  ..rHt.d.t.|.....
+0000b6a0: 4400 5d58 7d0b 7c07 6402 1900 6a01 7c0b  D.]X}.|.d...j.|.
+0000b6b0: 1900 7d0c 7c0c 7c08 6b02 73ee 7404 a00c  ..}.|.|.k.s.t...
+0000b6c0: 7404 a00d 7c0a 7c0c a102 a101 640d 6b00  t...|.|.....d.k.
+0000b6d0: 9001 7222 71ee 740a 7c03 7c0c 8302 7d0d  ..r"q.t.|.|...}.
+0000b6e0: 7404 a00d 7c0a 7c0d a102 7d0e 7c0a 7404  t...|.|...}.|.t.
+0000b6f0: a00e 7c0e a101 1900 7d0a 71ee 7c0a 7d0f  ..|.....}.q.|.}.
+0000b700: 7c00 6a06 7c00 6402 1900 a007 7c0f a101  |.j.|.d.....|...
+0000b710: 1900 7d00 7c00 5300 6409 7d08 7c00 6a06  ..}.|.S.d.}.|.j.
+0000b720: 7c00 7c04 1900 7c01 6b02 1900 7d09 7409  |.|...|.k...}.t.
+0000b730: 7c09 8301 6401 6b04 9001 72a2 7c09 6402  |...d.k...r.|.d.
+0000b740: 1900 6a01 6401 1900 7d08 740a 7c03 7c08  ..j.d...}.t.|.|.
+0000b750: 8302 7d0f 6e0a 7c00 6402 1900 6a01 7d0f  ..}.n.|.d...j.}.
+0000b760: 7c00 6a06 7c00 6402 1900 a007 7c0f a101  |.j.|.d.....|...
+0000b770: 1900 7d00 7c00 5300 6400 5300 290e 4e72  ..}.|.S.d.S.).Nr
+0000b780: 0100 0000 7206 0000 0072 0d00 0000 7260  ....r....r....r`
+0000b790: 0000 0072 7800 0000 7279 0000 0072 3c01  ...rx...ry...r<.
+0000b7a0: 0000 5a09 7265 675f 7375 6269 6472 6600  ..Z.reg_subidrf.
+0000b7b0: 0000 7a41 546f 2075 7365 2073 7562 7265  ..zATo use subre
+0000b7c0: 6769 6f6e 2c20 7468 6520 5375 6272 6567  gion, the Subreg
+0000b7d0: 696f 6e20 4964 204d 5553 5420 7072 6f76  ion Id MUST prov
+0000b7e0: 6964 6564 2061 7320 4f75 746c 6574 5f4f  ided as Outlet_O
+0000b7f0: 6273 5f49 447a 284e 6f20 4f75 746c 6574  bs_IDz(No Outlet
+0000b800: 2069 6420 6973 2066 6f75 6e64 6564 2066   id is founded f
+0000b810: 6f72 2073 7562 7265 6769 6f6e 2020 2072  or subregion   r
+0000b820: 6200 0000 7228 0000 0029 0f72 1600 0000  b...r(...).r....
+0000b830: 7213 0000 0072 1100 0000 5a10 4462 665f  r....r....Z.Dbf_
+0000b840: 546f 5f44 6174 6166 7261 6d65 721a 0000  To_Dataframer...
+0000b850: 0072 2b00 0000 7219 0000 0072 1200 0000  .r+...r....r....
+0000b860: 7268 0000 0072 1500 0000 7217 0000 0072  rh...r....r....r
+0000b870: 2900 0000 723e 0000 0072 2e00 0000 72a3  )...r>...r....r.
+0000b880: 0000 0029 1072 6900 0000 da0d 6f75 746c  ...).ri.....outl
+0000b890: 6574 5f6f 6273 5f69 64da 1670 6174 685f  et_obs_id..path_
+0000b8a0: 7375 625f 7265 675f 6f75 746c 6574 735f  sub_reg_outlets_
+0000b8b0: 7672 6a00 0000 7293 0000 005a 0f53 7562  vrj...r....Z.Sub
+0000b8c0: 5f72 6567 5f6f 7574 6c65 7473 5a13 5375  _reg_outletsZ.Su
+0000b8d0: 625f 7265 675f 6f75 746c 6574 735f 6964  b_reg_outlets_id
+0000b8e0: 735a 0f72 6567 5f6f 7574 6c65 745f 696e  sZ.reg_outlet_in
+0000b8f0: 666f 72c7 0000 005a 0d6f 7574 6c65 7449  for....Z.outletI
+0000b900: 445f 696e 666f 7218 0100 0072 4700 0000  D_infor....rG...
+0000b910: 5a07 7570 7265 6769 645a 1248 7964 726f  Z.upregidZ.Hydro
+0000b920: 4261 7369 6e73 5f72 656d 6f76 6572 2300  Basins_remover#.
+0000b930: 0000 721a 0100 0072 2400 0000 7224 0000  ..r....r$...r$..
+0000b940: 0072 2500 0000 da1f 7265 7475 726e 5f69  .r%.....return_i
+0000b950: 6e74 6572 6573 745f 6361 7463 686d 656e  nterest_catchmen
+0000b960: 7473 5f69 6e66 6f19 0d00 0073 5c00 0000  ts_info....s\...
+0000b970: 0002 0801 0402 1402 0401 0a01 0402 0a02  ................
+0000b980: 0601 02ff 0602 0a01 0c03 0c01 02ff 0604  ................
+0000b990: 0402 0801 0801 0402 1201 0c01 1002 0a01  ................
+0000b9a0: 0403 0a04 0e02 1201 0e02 2001 0201 0a01  .......... .....
+0000b9b0: 0401 04ff 0403 1001 0402 1401 0403 0401  ................
+0000b9c0: 1201 0e01 0e02 0c02 0a02 1401 723f 0100  ............r?..
+0000b9d0: 0063 0200 0000 0000 0000 0000 0000 0c00  .c..............
+0000b9e0: 0000 0500 0000 0300 0000 7352 0100 0067  ..........sR...g
+0000b9f0: 007d 0288 0164 0119 006a 007d 0374 01a0  .}...d...j.}.t..
+0000ba00: 027c 03a1 017d 0367 007d 0274 03a0 04a1  .|...}.g.}.t....
+0000ba10: 0074 056a 0664 023c 007c 02a0 0764 03a1  .t.j.d.<.|...d..
+0000ba20: 0101 007c 02a0 0764 04a1 0101 007c 02a0  ...|...d.....|..
+0000ba30: 0764 05a1 0101 0074 087c 0383 017d 047c  .d.....t.|...}.|
+0000ba40: 02a0 0764 0674 097c 0483 0117 00a1 0101  ...d.t.|........
+0000ba50: 0074 0a7c 0164 0719 006a 0083 0164 0817  .t.|.d...j...d..
+0000ba60: 0074 0a7c 0164 0919 006a 0083 0164 0817  .t.|.d...j...d..
+0000ba70: 0014 007d 057c 02a0 0764 0a74 097c 0583  ...}.|...d.t.|..
+0000ba80: 0117 00a1 0101 007c 02a0 0764 0ba1 0101  .......|...d....
+0000ba90: 007c 02a0 0764 0ca1 0101 0074 0a7c 0164  .|...d.....t.|.d
+0000baa0: 0919 006a 0083 0189 027c 0164 0d19 006a  ...j.....|.d...j
+0000bab0: 0089 0074 0b74 087c 0383 0164 0e1b 0083  ...t.t.|...d....
+0000bac0: 017d 0674 087c 0383 0164 0f6b 0472 ee74  .}.t.|...d.k.r.t
+0000bad0: 01a0 0c7c 037c 06a1 027d 076e 067c 0367  ...|.|...}.n.|.g
+0000bae0: 017d 0774 0d64 1074 087c 0783 0183 0244  .}.t.d.t.|.....D
+0000baf0: 005d 367d 087c 077c 0819 007d 0974 0e64  .]6}.|.|...}.t.d
+0000bb00: 1164 128d 0187 0087 0187 0266 0364 1364  .d.........f.d.d
+0000bb10: 1484 087c 0944 0083 0183 017d 0a7c 027c  ...|.D.....}.|.|
+0000bb20: 0a17 007d 0290 0171 027c 02a0 0764 15a1  ...}...q.|...d..
+0000bb30: 0101 0064 16a0 0f7c 02a1 017d 0b7c 0b53  ...d...|...}.|.S
+0000bb40: 0029 174e 72ab 0000 005a 124a 4f42 4c49  .).Nr....Z.JOBLI
+0000bb50: 425f 5445 4d50 5f46 4f4c 4445 527a 0c3a  B_TEMP_FOLDERz.:
+0000bb60: 4772 6964 5765 6967 6874 737a 0a20 2020  GridWeightsz.   
+0000bb70: 2320 2020 2020 207a 0d20 2020 2320 5b23  #      z.   # [#
+0000bb80: 2048 5255 735d 7a15 2020 203a 4e75 6d62   HRUs]z.   :Numb
+0000bb90: 6572 4852 5573 2020 2020 2020 20da 0352  erHRUs       ..R
+0000bba0: 6f77 7228 0000 00da 0343 6f6c 7a15 2020  owr(.....Colz.  
+0000bbb0: 203a 4e75 6d62 6572 4772 6964 4365 6c6c   :NumberGridCell
+0000bbc0: 7320 207a 1020 2020 2320 2020 2020 2020  s  z.   #       
+0000bbd0: 2020 2020 207a 1d20 2020 2320 5b48 5255       z.   # [HRU
+0000bbe0: 2049 445d 205b 4365 6c6c 2023 5d20 5b77   ID] [Cell #] [w
+0000bbf0: 5f6b 6c5d 5a04 4647 4944 72db 0000 0072  _kl]Z.FGIDr....r
+0000bc00: 6f00 0000 7201 0000 0072 1d01 0000 2901  o...r....r....).
+0000bc10: 5a06 6e5f 6a6f 6273 6301 0000 0000 0000  Z.n_jobsc.......
+0000bc20: 0000 0000 0002 0000 0006 0000 0033 0000  .............3..
+0000bc30: 0073 2800 0000 7c00 5d20 7d01 7400 7401  .s(...|.] }.t.t.
+0000bc40: 8301 7c01 8801 6a02 6400 6401 8d01 8800  ..|...j.d.d.....
+0000bc50: 8802 8304 5600 0100 7102 6402 5300 2903  ....V...q.d.S.).
+0000bc60: 5472 0700 0000 4e29 0372 0500 0000 da16  Tr....N).r......
+0000bc70: 6372 6561 7465 5f67 7269 645f 7765 6967  create_grid_weig
+0000bc80: 6874 5f68 7275 7214 0000 0029 02da 022e  ht_hrur....)....
+0000bc90: 3072 4700 0000 a903 da07 4176 6166 6769  0rG.......Avafgi
+0000bca0: 64da 0a4d 6170 666f 7263 696e 67da 076d  d..Mapforcing..m
+0000bcb0: 6178 5f63 6f6c 7224 0000 0072 2500 0000  ax_colr$...r%...
+0000bcc0: da09 3c67 656e 6578 7072 3e85 0d00 0073  ..<genexpr>....s
+0000bcd0: 0800 0000 0401 02ff 0601 10ff 7a2a 6372  ............z*cr
+0000bce0: 6561 7465 5f67 7269 645f 7765 6967 6874  eate_grid_weight
+0000bcf0: 5f6d 6169 6e2e 3c6c 6f63 616c 733e 2e3c  _main.<locals>.<
+0000bd00: 6765 6e65 7870 723e 7a0f 3a45 6e64 4772  genexpr>z.:EndGr
+0000bd10: 6964 5765 6967 6874 73da 010a 2910 7213  idWeights...).r.
+0000bd20: 0000 0072 1a00 0000 722b 0000 00da 0874  ...r....r+.....t
+0000bd30: 656d 7066 696c 65da 0a67 6574 7465 6d70  empfile..gettemp
+0000bd40: 6469 72da 026f 73da 0765 6e76 6972 6f6e  dir..os..environ
+0000bd50: 724d 0000 0072 1500 0000 72e7 0000 0072  rM...r....r....r
+0000bd60: 6700 0000 722d 0000 00da 0b61 7272 6179  g...r-.....array
+0000bd70: 5f73 706c 6974 7229 0000 0072 0400 0000  _splitr)...r....
+0000bd80: da04 6a6f 696e 290c 7246 0100 005a 0846  ..join).rF...Z.F
+0000bd90: 6f72 6369 6e66 6f5a 1767 7269 645f 7765  orcinfoZ.grid_we
+0000bda0: 6967 6874 5f73 7472 696e 675f 6c69 7374  ight_string_list
+0000bdb0: 5a06 6872 7569 6473 5a05 734e 6872 755a  Z.hruidsZ.sNhruZ
+0000bdc0: 0673 4e63 656c 6c5a 0b6e 5f68 7275 5f67  .sNcellZ.n_hru_g
+0000bdd0: 726f 7570 5a0e 6872 755f 6964 735f 6772  roupZ.hru_ids_gr
+0000bde0: 6f75 7073 7247 0000 005a 0b69 5f68 7275  oupsrG...Z.i_hru
+0000bdf0: 5f67 726f 7570 5a18 6772 6964 5f77 6569  _groupZ.grid_wei
+0000be00: 6768 745f 7374 7269 6e67 5f68 7275 7369  ght_string_hrusi
+0000be10: 5a12 6772 6964 5f77 6569 6768 745f 7374  Z.grid_weight_st
+0000be20: 7269 6e67 7224 0000 0072 4401 0000 7225  ringr$...rD...r%
+0000be30: 0000 00da 1763 7265 6174 655f 6772 6964  .....create_grid
+0000be40: 5f77 6569 6768 745f 6d61 696e 610d 0000  _weight_maina...
+0000be50: 733e 0000 0000 0204 010a 010a 0204 020e  s>..............
+0000be60: 020a 010a 010a 0208 0112 0210 0110 ff04  ................
+0000be70: 0212 010a 010a 010e 010a 0410 020c 010e  ................
+0000be80: 0206 0212 0108 0116 0102 ff08 020c 020a  ................
+0000be90: 010a 0172 5001 0000 6304 0000 0000 0000  ...rP...c.......
+0000bea0: 0000 0000 000e 0000 0006 0000 0043 0000  .............C..
+0000beb0: 0073 1602 0000 6401 7d04 7c01 6a00 7c01  .s....d.}.|.j.|.
+0000bec0: 6402 1900 7c00 6b02 1900 6a01 6403 6404  d...|.k...j.d.d.
+0000bed0: 8d01 7d05 7402 7c05 8301 6405 6b01 725c  ..}.t.|...d.k.r\
+0000bee0: 7c01 6a00 7c01 6402 1900 7c00 6b02 1900  |.j.|.d...|.k...
+0000bef0: 6a01 6403 6404 8d01 7d05 7403 6406 8301  j.d.d...}.t.d...
+0000bf00: 0100 7403 7c05 6407 1900 8301 0100 7c04  ..t.|.d.......|.
+0000bf10: 5300 7404 7c05 6408 1900 6a05 8301 7d06  S.t.|.d...j...}.
+0000bf20: 7c05 6407 1900 6a05 7d07 7406 a007 7c07  |.d...j.}.t...|.
+0000bf30: a101 7d07 6409 7d08 7408 6405 7402 7c07  ..}.d.}.t.d.t.|.
+0000bf40: 8301 8302 4400 9001 5d7e 7d09 7c05 7c05  ....D...]~}.|.|.
+0000bf50: 6407 1900 7c07 7c09 1900 6b02 1900 7d0a  d...|.|...k...}.
+0000bf60: 7c09 7402 7c07 8301 640a 1800 6b00 72e2  |.t.|...d...k.r.
+0000bf70: 7404 7c0a 6408 1900 6a05 8301 7d0b 7409  t.|.d...j...}.t.
+0000bf80: 7c0b 8301 7409 7c06 8301 1b00 7d0c 7c08  |...t.|.....}.|.
+0000bf90: 7c0c 1700 7d08 6e08 640a 7c08 1800 7d0c  |...}.n.d.|...}.
+0000bfa0: 7402 7c0a 640b 1900 6a05 8301 640a 6b04  t.|.d...j...d.k.
+0000bfb0: 9001 7240 7403 740a 740b 8301 640c 1700  ..r@t.t.t...d...
+0000bfc0: 8301 0100 740a 740c 7c0a 640b 1900 6a05  ....t.t.|.d...j.
+0000bfd0: 6405 1900 7c03 640a 1700 1400 7c0a 640d  d...|.d.....|.d.
+0000bfe0: 1900 6a05 6405 1900 1700 8301 8301 640e  ..j.d.........d.
+0000bff0: 1700 7d0d 6e30 740a 740c 7c0a 640b 1900  ..}.n0t.t.|.d...
+0000c000: 6a05 6405 1900 7c03 640a 1700 1400 7c0a  j.d...|.d.....|.
+0000c010: 640d 1900 6a05 6405 1900 1700 8301 8301  d...j.d.........
+0000c020: 640e 1700 7d0d 7402 7c07 8301 640a 6b02  d...}.t.|...d.k.
+0000c030: 9001 72a8 7c04 640f 1700 740a 740c 7c00  ..r.|.d...t.t.|.
+0000c040: 8301 8301 1700 6410 1700 7c0d 1700 640e  ......d...|...d.
+0000c050: 1700 740a 7c0c 8301 1700 7d04 7190 7c09  ..t.|.....}.q.|.
+0000c060: 7402 7c07 8301 640a 1800 6b02 9001 72e4  t.|...d...k...r.
+0000c070: 7c04 640f 1700 740a 740c 7c00 8301 8301  |.d...t.t.|.....
+0000c080: 1700 6410 1700 7c0d 1700 640e 1700 740a  ..d...|...d...t.
+0000c090: 7c0c 8301 1700 7d04 7190 7c04 640f 1700  |.....}.q.|.d...
+0000c0a0: 740a 740c 7c00 8301 8301 1700 6410 1700  t.t.|.......d...
+0000c0b0: 7c0d 1700 640e 1700 740a 7c0c 8301 1700  |...d...t.|.....
+0000c0c0: 6411 1700 7d04 7190 7c04 5300 2912 4efa  d...}.q.|.S.).N.
+0000c0d0: 0120 72ab 0000 0054 7207 0000 0072 0100  . r....Tr....r..
+0000c0e0: 0000 7a28 466f 6c6c 6f77 696e 6720 4772  ..z(Following Gr
+0000c0f0: 6964 2068 6173 2074 6f20 6265 2069 6e6c  id has to be inl
+0000c100: 7564 6564 3a2e 2e2e 2e2e 2e2e 5a08 4d61  uded:.......Z.Ma
+0000c110: 705f 4647 4944 5a06 735f 6172 6561 72be  p_FGIDZ.s_arear.
+0000c120: 0000 0072 2800 0000 5a07 4d61 705f 526f  ...r(...Z.Map_Ro
+0000c130: 777a 3d65 7272 6f72 3a20 3120 6872 752c  wz=error: 1 hru,
+0000c140: 2031 2067 7269 642c 2070 726f 6475 6365   1 grid, produce
+0000c150: 206d 7574 6920 706f 6c79 676f 6e20 6e65   muti polygon ne
+0000c160: 6564 2074 6f20 6265 206d 6572 6765 6420  ed to be merged 
+0000c170: 5a07 4d61 705f 436f 6c7a 0620 2020 2020  Z.Map_Colz.     
+0000c180: 207a 0420 2020 207a 0520 2020 2020 7249   z.    z.     rI
+0000c190: 0100 0029 0d72 1900 0000 7214 0000 0072  ...).r....r....r
+0000c1a0: 1500 0000 7268 0000 0072 3e00 0000 7213  ....rh...r>...r.
+0000c1b0: 0000 0072 1a00 0000 722b 0000 0072 2900  ...r....r+...r).
+0000c1c0: 0000 7260 0000 0072 e700 0000 72c4 0000  ..r`...r....r...
+0000c1d0: 0072 2d00 0000 290e 725d 0000 0072 4601  .r-...).r]...rF.
+0000c1e0: 0000 7245 0100 0072 4701 0000 5a16 6772  ..rE...rG...Z.gr
+0000c1f0: 6964 5f77 6569 6768 745f 7374 7269 6e67  id_weight_string
+0000c200: 5f68 7275 da04 6361 7473 5a05 7461 7265  _hru..catsZ.tare
+0000c210: 61da 0466 6964 735a 0573 756d 7774 725b  a..fidsZ.sumwtr[
+0000c220: 0000 005a 0473 6361 745a 0573 6172 6561  ...Z.scatZ.sarea
+0000c230: da02 7774 5a09 5374 7263 656c 6c69 6472  ..wtZ.Strcellidr
+0000c240: 2400 0000 7224 0000 0072 2500 0000 7242  $...r$...r%...rB
+0000c250: 0100 008e 0d00 0073 ac00 0000 0002 0402  .......s........
+0000c260: 1a04 0c01 1a01 0801 0c01 0402 0e01 0a01  ................
+0000c270: 0a01 0401 1401 1401 1001 0e01 1001 0a02  ................
+0000c280: 0802 1401 0201 0601 02ff 02ff 0405 0201  ................
+0000c290: 0201 0c01 06ff 0202 0cfe 02ff 02ff 0207  ................
+0000c2a0: 02f9 02ff 040c 0201 0201 0c01 06ff 0202  ................
+0000c2b0: 0cfe 02ff 02ff 0207 02f9 02ff 020a 0e01  ................
+0000c2c0: 0601 0aff 0201 02ff 0201 02ff 0201 02ff  ................
+0000c2d0: 0201 06ff 0603 1201 0601 0aff 0201 02ff  ................
+0000c2e0: 0201 02ff 0201 02ff 0201 06ff 0603 0601  ................
+0000c2f0: 0aff 0201 02ff 0201 02ff 0202 02fe 0202  ................
+0000c300: 06fe 0202 02fe 0604 7242 0100 0029 0272  ........rB...).r
+0000c310: 7600 0000 7277 0000 0029 0172 0600 0000  v...rw...).r....
+0000c320: 2902 7228 0000 0072 2800 0000 2902 7228  ).r(...r(...).r(
+0000c330: 0000 0072 2800 0000 2901 723c 0100 0029  ...r(...).r<...)
+0000c340: 3772 1400 0000 da05 6e75 6d70 7972 1a00  7r......numpyr..
+0000c350: 0000 da06 7061 6e64 6173 723f 0000 005a  ....pandasr?...Z
+0000c360: 0e73 6369 7079 2e6f 7074 696d 697a 6572  .scipy.optimizer
+0000c370: 0200 0000 da1e 6261 7369 6e6d 616b 6572  ......basinmaker
+0000c380: 2e75 7469 6c69 7469 6573 2e75 7469 6c69  .utilities.utili
+0000c390: 7469 6573 da07 6e75 6d62 6572 735a 066a  ties..numbersZ.j
+0000c3a0: 6f62 6c69 6272 0400 0000 7205 0000 0072  oblibr....r....r
+0000c3b0: 4a01 0000 da07 6f70 7469 6f6e 73da 046d  J.....options..m
+0000c3c0: 6f64 65da 1263 6861 696e 6564 5f61 7373  ode..chained_ass
+0000c3d0: 6967 6e6d 656e 7472 2600 0000 7231 0000  ignmentr&...r1..
+0000c3e0: 0072 2a00 0000 724b 0000 0072 5500 0000  .r*...rK...rU...
+0000c3f0: 725f 0000 0072 6b00 0000 7275 0000 0072  r_...rk...ru...r
+0000c400: 9900 0000 72aa 0000 0072 af00 0000 72b9  ....r....r....r.
+0000c410: 0000 0072 bd00 0000 72b2 0000 0072 1700  ...r....r....r..
+0000c420: 0000 72d3 0000 0072 d900 0000 72e1 0000  ..r....r....r...
+0000c430: 0072 e400 0000 72e9 0000 0072 fc00 0000  .r....r....r....
+0000c440: 72ef 0000 0072 0601 0000 7204 0100 0072  r....r....r....r
+0000c450: 0e01 0000 7211 0100 0072 1301 0000 7216  ....r....r....r.
+0000c460: 0100 0072 1b01 0000 7228 0100 0072 2d01  ...r....r(...r-.
+0000c470: 0000 722e 0100 0072 2200 0000 7231 0100  ..r....r"...r1..
+0000c480: 0072 3301 0000 723b 0100 0072 3f01 0000  .r3...r;...r?...
+0000c490: 7250 0100 0072 4201 0000 7224 0000 0072  rP...rB...r$...r
+0000c4a0: 2400 0000 7224 0000 0072 2500 0000 da08  $...r$...r%.....
+0000c4b0: 3c6d 6f64 756c 653e 0100 0000 7380 0000  <module>....s...
+0000c4c0: 0008 0208 0108 010c 0108 0108 0110 0108  ................
+0000c4d0: 010a 0308 3708 3808 0d08 2408 1908 6108  ....7.8...$...a.
+0000c4e0: 5408 5b0a 7f00 4002 0102 0104 0104 0102  T.[...@.........
+0000c4f0: 0102 f70a 7f00 1e0a 180a 4008 0b08 7f00  ..........@.....
+0000c500: 7f00 2508 2a08 6408 7f00 6908 7b08 1408  ..%.*.d...i.{...
+0000c510: 7f00 7f00 0108 7f00 7f00 7f00 2b08 4108  ............+.A.
+0000c520: 4408 2d08 5c08 6608 7008 2c08 2008 7f00  D.-.\.f.p.,. ...
+0000c530: 0a08 5708 2b0a 5508 0408 0b08 1a0a 4808  ..W.+.U.......H.
+0000c540: 2d                                       -
```

### Comparing `basinmaker-3.0.3a0/basinmaker/func/__pycache__/purepy.cpython-39.pyc` & `basinmaker-3.1.0/basinmaker/func/__pycache__/purepy.cpython-39.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.9, timestamp-based, .py timestamp: Mon Apr 10 21:29:09 2023 UTC, .py size: 17567 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 13% similar despite different names*

```diff
@@ -1,646 +1,734 @@
-00000000: 610d 0d0a 0000 0000 a57f 3464 9f44 0000  a.........4d.D..
+00000000: 610d 0d0a 0000 0000 cf19 6864 6453 0000  a.........hddS..
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
-00000020: 0003 0000 0040 0000 0073 c600 0000 6400  .....@...s....d.
+00000020: 0003 0000 0040 0000 0073 de00 0000 6400  .....@...s....d.
 00000030: 6401 6c00 5a00 6400 6401 6c01 5a02 6400  d.l.Z.d.d.l.Z.d.
 00000040: 6401 6c03 5a03 6400 6401 6c04 5a05 6400  d.l.Z.d.d.l.Z.d.
 00000050: 6402 6c06 6d07 5a07 6d08 5a08 0100 6400  d.l.m.Z.m.Z...d.
 00000060: 6401 6c06 5a06 6400 6401 6c09 5a09 6400  d.l.Z.d.d.l.Z.d.
 00000070: 6401 6c0a 5a0a 6400 6403 6c0b 6d0c 5a0c  d.l.Z.d.d.l.m.Z.
 00000080: 6d0d 5a0d 0100 6400 6404 6c0e 6d0f 5a0f  m.Z...d.d.l.m.Z.
 00000090: 0100 6405 6406 8400 5a10 6407 6408 8400  ..d.d...Z.d.d...
-000000a0: 5a11 641e 640a 640b 8401 5a12 641f 640d  Z.d.d.d...Z.d.d.
+000000a0: 5a11 6424 640a 640b 8401 5a12 6425 640d  Z.d$d.d...Z.d%d.
 000000b0: 640e 8401 5a13 640f 6410 8400 5a14 6411  d...Z.d.d...Z.d.
-000000c0: 6412 8400 5a15 6413 6414 8400 5a16 6420  d...Z.d.d...Z.d 
+000000c0: 6412 8400 5a15 6413 6414 8400 5a16 6426  d...Z.d.d...Z.d&
 000000d0: 6416 6417 8401 5a17 6418 6419 8400 5a18  d.d...Z.d.d...Z.
 000000e0: 641a 641b 8400 5a19 641c 641d 8400 5a1a  d.d...Z.d.d...Z.
-000000f0: 6401 5300 2921 e900 0000 004e 2902 da04  d.S.)!.....N)...
-00000100: 6c6f 6164 da0b 4a53 4f4e 456e 636f 6465  load..JSONEncode
-00000110: 7229 02da 0467 6461 6cda 036f 6772 2901  r)...gdal..ogr).
-00000120: da0b 7a6f 6e61 6c5f 7374 6174 7363 0400  ..zonal_statsc..
-00000130: 0000 0000 0000 0000 0000 0700 0000 0700  ................
-00000140: 0000 0300 0000 7336 0000 0074 007c 007c  ......s6...t.|.|
-00000150: 017c 0264 0164 0164 028d 057d 0474 0174  .|.d.d.d...}.t.t
-00000160: 0287 0066 0164 0364 0484 087c 0483 0283  ...f.d.d...|....
-00000170: 017d 0574 03a0 047c 05a1 017d 067c 0653  .}.t...|...}.|.S
-00000180: 0029 054e 5429 03da 0573 7461 7473 5a0b  .).NT)...statsZ.
-00000190: 6765 6f6a 736f 6e5f 6f75 745a 0b61 6c6c  geojson_outZ.all
-000001a0: 5f74 6f75 6368 6564 6301 0000 0000 0000  _touchedc.......
-000001b0: 0000 0000 0001 0000 0005 0000 0013 0000  ................
-000001c0: 0073 1c00 0000 8800 7c00 6401 1900 8800  .s......|.d.....
-000001d0: 1900 6402 7c00 6401 1900 6402 1900 6902  ..d.|.d...d...i.
-000001e0: 5300 2903 4eda 0a70 726f 7065 7274 6965  S.).N..propertie
-000001f0: 73da 046d 6561 6ea9 0029 01da 0178 a901  s..mean..)...x..
-00000200: da03 6b65 7972 0a00 0000 fa47 633a 5c75  ..keyr.....Gc:\u
-00000210: 7365 7273 5c6d 3433 6861 6e5f 325c 646f  sers\m43han_2\do
-00000220: 6375 6d65 6e74 735c 6769 7468 7562 5c62  cuments\github\b
-00000230: 6173 696e 6d61 6b65 725c 6261 7369 6e6d  asinmaker\basinm
-00000240: 616b 6572 5c66 756e 635c 7075 7265 7079  aker\func\purepy
-00000250: 2e70 79da 083c 6c61 6d62 6461 3e12 0000  .py..<lambda>...
-00000260: 00f3 0000 0000 7a20 7a6f 6e61 6c5f 7374  ......z zonal_st
-00000270: 6174 735f 7064 2e3c 6c6f 6361 6c73 3e2e  ats_pd.<locals>.
-00000280: 3c6c 616d 6264 613e 2905 7206 0000 00da  <lambda>).r.....
-00000290: 046c 6973 74da 036d 6170 da02 7064 da09  .list..map..pd..
-000002a0: 4461 7461 4672 616d 6529 07da 0773 6870  DataFrame)...shp
-000002b0: 5f67 7064 da06 7261 7374 6572 7207 0000  _gpd..rasterr...
-000002c0: 0072 0d00 0000 da06 7265 7375 6c74 5a0f  .r......resultZ.
-000002d0: 7265 6175 6c74 5f6c 6973 745f 6469 63da  reault_list_dic.
-000002e0: 0972 6561 756c 745f 7064 720a 0000 0072  .reault_pdr....r
-000002f0: 0c00 0000 720e 0000 00da 0e7a 6f6e 616c  ....r......zonal
-00000300: 5f73 7461 7473 5f70 640e 0000 0073 0800  _stats_pd....s..
-00000310: 0000 0002 1202 1602 0a02 7219 0000 0063  ..........r....c
-00000320: 0500 0000 0000 0000 0000 0000 0b00 0000  ................
-00000330: 0500 0000 4300 0000 73ce 0000 007c 006a  ....C...s....|.j
-00000340: 0064 0164 028d 017d 0564 037d 0674 017c  .d.d...}.d.}.t.|
-00000350: 0583 0164 036b 0472 a87c 0664 046b 0172  ...d.k.r.|.d.k.r
-00000360: a874 027c 057c 017c 027c 0383 047d 077c  .t.|.|.|.|...}.|
-00000370: 077c 0764 0519 0064 036b 040f 0019 0064  .|.d...d.k.....d
-00000380: 0619 007d 087c 057c 0564 0619 00a0 037c  ...}.|.|.d.....|
-00000390: 08a1 0119 006a 0064 0164 028d 017d 057c  .....j.d.d...}.|
-000003a0: 0664 036b 0272 847c 077c 0764 0519 0064  .d.k.r.|.|.d...d
-000003b0: 036b 0419 007d 097c 0664 0717 007d 0671  .k...}.|.d...}.q
-000003c0: 107c 0664 0717 007d 067c 077c 0764 0519  .|.d...}.|.|.d..
-000003d0: 0064 036b 0419 007d 0a7c 09a0 047c 0aa1  .d.k...}.|...|..
-000003e0: 017d 0971 1074 017c 0583 0164 036b 0472  .}.q.t.|...d.k.r
-000003f0: ca7c 057c 0419 007c 0564 053c 007c 09a0  .|.|...|.d.<.|..
-00000400: 047c 05a1 017d 097c 0953 0029 084e 54a9  .|...}.|.S.).NT.
-00000410: 01da 0464 6565 7072 0100 0000 e905 0000  ...deepr........
-00000420: 0072 0900 0000 da0a 4852 555f 4944 5f4e  .r......HRU_ID_N
-00000430: 6577 e901 0000 0029 05da 0463 6f70 79da  ew.....)...copy.
-00000440: 036c 656e 7219 0000 00da 0469 7369 6eda  .lenr......isin.
-00000450: 0661 7070 656e 6429 0b72 1500 0000 7216  .append).r....r.
-00000460: 0000 0072 0700 0000 720d 0000 00da 0363  ...r....r......c
-00000470: 6f6c 5a09 6e6f 6461 7461 5f70 64da 0169  olZ.nodata_pd..i
-00000480: 5a07 7465 6d70 5f70 645a 0e62 6164 5f68  Z.temp_pdZ.bad_h
-00000490: 7275 5f76 616c 7565 7372 1800 0000 5a07  ru_valuesr....Z.
-000004a0: 676f 6f64 5f70 6472 0a00 0000 720a 0000  good_pdr....r...
-000004b0: 0072 0e00 0000 da0a 5a6f 6e61 6c53 7461  .r......ZonalSta
-000004c0: 7473 1a00 0000 7320 0000 0000 060c 0104  ts....s ........
-000004d0: 0114 010e 0116 011a 0108 0110 010a 0208  ................
-000004e0: 0110 010c 020c 010c 010a 0272 2500 0000  ...........r%...
-000004f0: fa01 2363 0600 0000 0000 0000 0000 0000  ..#c............
-00000500: 0d00 0000 0600 0000 4300 0000 730a 0100  ........C...s...
-00000510: 007c 036a 007d 0674 01a0 027c 00a1 017d  .|.j.}.t...|...}
-00000520: 077c 07a0 037c 06a1 017d 087c 086a 0464  .|...|...}.|.j.d
-00000530: 0164 028d 017d 087c 08a0 057c 03a1 017d  .d...}.|...|...}
-00000540: 0974 067c 0964 0383 027d 0a7c 0464 046b  .t.|.d...}.|.d.k
-00000550: 0390 0172 067c 017c 096a 0776 0172 6074  ...r.|.|.j.v.r`t
-00000560: 087c 0164 0583 0201 0074 09a0 0aa1 0001  .|.d.....t......
-00000570: 007c 017c 056a 0776 0172 7c74 087c 0164  .|.|.j.v.r|t.|.d
-00000580: 0683 0201 0074 09a0 0aa1 0001 007c 047c  .....t.......|.|
-00000590: 056a 0776 0172 9874 087c 0464 0683 0201  .j.v.r.t.|.d....
-000005a0: 0074 09a0 0aa1 0001 007c 056a 0b64 0164  .t.......|.j.d.d
-000005b0: 078d 017d 0b7c 0b6a 0c7c 0467 0164 0864  ...}.|.j.|.g.d.d
-000005c0: 0164 098d 037d 0b7c 0b7c 0119 007c 0b64  .d...}.|.|...|.d
-000005d0: 0a3c 007c 0b7c 0464 0a67 0219 007d 0b74  .<.|.|.d.g...}.t
-000005e0: 0d6a 0e7c 057c 0b64 0b7c 0464 0c8d 046a  .j.|.|.d.|.d...j
-000005f0: 0b64 0164 078d 017d 0c74 0d6a 0e7c 0a7c  .d.d...}.t.j.|.|
-00000600: 0c64 0b7c 0164 0c8d 047d 0a7c 0a64 0a19  .d.|.d...}.|.d..
-00000610: 007c 0a7c 013c 007c 0a53 0029 0d61 b205  .|.|.<.|.S.).a..
-00000620: 0000 5072 6570 726f 6365 7373 2075 7365  ..Preprocess use
-00000630: 7220 7072 6f76 6964 6564 2070 6f6c 7967  r provided polyg
-00000640: 6f6e 730a 0a20 2020 2046 756e 6374 696f  ons..    Functio
-00000650: 6e20 7468 6174 2077 696c 6c20 7265 7072  n that will repr
-00000660: 6f6a 6563 7420 636c 6970 2069 6e70 7574  oject clip input
-00000670: 2070 6f6c 7967 6f6e 2077 6974 6820 7375   polygon with su
-00000680: 6262 6173 696e 2070 6f6c 7967 6f6e 0a20  bbasin polygon. 
-00000690: 2020 2061 6e64 2077 696c 6c20 6469 7373     and will diss
-000006a0: 6f6c 7665 2074 6865 2069 6e70 7574 2070  olve the input p
-000006b0: 6f6c 7967 6f6e 2062 6173 6564 206f 6e20  olygon based on 
-000006c0: 7468 6569 7220 4944 2c20 7375 6368 2061  their ID, such a
-000006d0: 7320 6c61 6e64 7573 6520 6964 0a20 2020  s landuse id.   
-000006e0: 206f 7220 736f 696c 2069 642e 0a0a 2020   or soil id...  
-000006f0: 2020 5061 7261 6d65 7465 7273 0a20 2020    Parameters.   
-00000700: 202d 2d2d 2d2d 2d2d 2d2d 2d0a 2020 2020   ----------.    
-00000710: 7072 6f63 6573 7369 6e67 2020 2020 2020  processing      
-00000720: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00000730: 2020 3a20 7167 6973 206f 626a 6563 740a    : qgis object.
-00000740: 2020 2020 636f 6e74 6578 7420 2020 2020      context     
-00000750: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00000760: 2020 2020 2020 3a20 7167 6973 206f 626a        : qgis obj
-00000770: 6563 740a 2020 2020 6c61 7965 725f 7061  ect.    layer_pa
-00000780: 7468 2020 2020 2020 2020 2020 2020 2020  th              
-00000790: 2020 2020 2020 2020 2020 3a20 7374 7269            : stri
-000007a0: 6e67 0a20 2020 2020 2020 2054 6865 2070  ng.        The p
-000007b0: 6174 6820 746f 2061 2073 7065 6369 6669  ath to a specifi
-000007c0: 6320 706f 6c79 676f 6e2c 2066 6f72 2065  c polygon, for e
-000007d0: 7861 6d70 6c65 2070 6174 6820 746f 206c  xample path to l
-000007e0: 616e 6475 7365 206c 6179 6572 0a20 2020  anduse layer.   
-000007f0: 2050 726f 6a65 6374 5f63 7273 2020 2020   Project_crs    
-00000800: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00000810: 2020 203a 2073 7472 696e 670a 2020 2020     : string.    
-00000820: 2020 2020 7468 6520 4550 5347 2063 6f64      the EPSG cod
-00000830: 6520 6f66 2061 2070 726f 6a65 6374 6564  e of a projected
-00000840: 2063 6f6f 6469 6e61 7465 2073 7973 7465   coodinate syste
-00000850: 6d20 7468 6174 2077 696c 6c20 6265 2075  m that will be u
-00000860: 7365 6420 746f 0a20 2020 2020 2020 2063  sed to.        c
-00000870: 616c 6375 6174 6520 4852 5520 6172 6561  alcuate HRU area
-00000880: 2061 6e64 2073 6c6f 7065 2e0a 2020 2020   and slope..    
-00000890: 7472 675f 6372 7320 2020 2020 2020 2020  trg_crs         
-000008a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000008b0: 2020 3a20 7374 7269 6e67 0a20 2020 2020    : string.     
-000008c0: 2020 2074 6865 2045 5053 4720 636f 6465     the EPSG code
-000008d0: 206f 6620 6120 2063 6f6f 6469 6e61 7465   of a  coodinate
-000008e0: 2073 7973 7465 6d20 7468 6174 2077 696c   system that wil
-000008f0: 6c20 6265 2075 7365 6420 746f 0a20 2020  l be used to.   
-00000900: 2020 2020 2063 616c 6375 6174 6520 7265       calcuate re
-00000910: 7072 6f6a 6563 7420 696e 7075 7420 706f  project input po
-00000920: 6c79 676f 6e0a 2020 2020 436c 6173 735f  lygon.    Class_
-00000930: 436f 6c20 2020 2020 2020 2020 2020 2020  Col             
-00000940: 2020 2020 2020 2020 2020 2020 3a20 7374              : st
-00000950: 7269 6e67 0a20 2020 2020 2020 2074 6865  ring.        the
-00000960: 2063 6f6c 756d 6e20 6e61 6d65 2069 6e20   column name in 
-00000970: 7468 6520 696e 7075 7420 706f 6c79 676f  the input polygo
-00000980: 6e20 286c 6179 6572 5f70 6174 6829 2074  n (layer_path) t
-00000990: 6861 7420 636f 6e74 6169 6e73 0a20 2020  hat contains.   
-000009a0: 2020 2020 2074 6865 6972 2049 442c 2066       their ID, f
-000009b0: 6f72 2065 7861 6d70 6c65 206c 616e 6420  or example land 
-000009c0: 7573 6520 4944 206f 7220 736f 696c 2049  use ID or soil I
-000009d0: 442e 0a20 2020 204c 6179 6572 5f63 6c69  D..    Layer_cli
-000009e0: 7020 2020 2020 2020 2020 2020 2020 2020  p               
-000009f0: 2020 2020 2020 2020 203a 2071 6769 7320           : qgis 
-00000a00: 6f62 6a65 6374 0a20 2020 2020 2020 2041  object.        A
-00000a10: 2073 6870 6669 6c65 2077 6974 6820 6578   shpfile with ex
-00000a20: 7465 6e74 206f 6620 7468 6520 7761 7465  tent of the wate
-00000a30: 7273 6865 642c 2077 696c 6c20 6265 2075  rshed, will be u
-00000a40: 7365 6420 746f 2063 6c69 7020 696e 7075  sed to clip inpu
-00000a50: 740a 2020 2020 2020 2020 696e 7075 7420  t.        input 
-00000a60: 706f 6c79 676f 6e0a 2020 2020 4e6f 7465  polygon.    Note
-00000a70: 730a 2020 2020 2d2d 2d2d 2d2d 2d0a 2020  s.    -------.  
-00000a80: 2020 2020 2020 2320 544f 444f 3a20 4d61        # TODO: Ma
-00000a90: 7920 6265 2061 6464 2073 6f6d 6520 6675  y be add some fu
-00000aa0: 6e63 7469 6f6e 2074 6f20 7369 6d70 6c69  nction to simpli
-00000ab0: 6679 2074 6865 2069 6e70 7574 2070 6f6c  fy the input pol
-00000ac0: 7967 6f6e 730a 2020 2020 2020 2020 2020  ygons.          
-00000ad0: 2020 2020 2020 666f 7220 6578 616d 706c        for exampl
-00000ae0: 652c 2072 656d 6f76 6520 7468 6520 6c61  e, remove the la
-00000af0: 6e64 7573 6520 7479 7065 2077 6974 6820  nduse type with 
-00000b00: 736d 616c 6c20 6172 6561 730a 2020 2020  small areas.    
-00000b10: 2020 2020 2020 2020 2020 2020 6f72 206d              or m
-00000b20: 6572 6765 2073 6d61 6c6c 206c 616e 6475  erge small landu
-00000b30: 7365 2070 6f6c 7967 6f6e 2069 6e74 6f20  se polygon into 
-00000b40: 7468 6520 7375 7272 6f75 6e64 696e 6720  the surrounding 
-00000b50: 706f 6c79 676f 6e0a 0a20 2020 2052 6574  polygon..    Ret
-00000b60: 7572 6e73 3a0a 2020 2020 2d2d 2d2d 2d2d  urns:.    ------
-00000b70: 2d0a 2020 2020 2020 2020 6c61 7965 725f  -.        layer_
-00000b80: 6469 7320 2020 2020 2020 2020 2020 2020  dis             
-00000b90: 2020 2020 203a 2071 6769 7320 6f62 6a65       : qgis obje
-00000ba0: 6374 0a20 2020 2020 2020 2020 2020 2069  ct.            i
-00000bb0: 7420 6973 2061 2070 6f6c 7967 6f6e 2061  t is a polygon a
-00000bc0: 6674 6572 2070 7265 7072 6f63 6573 730a  fter preprocess.
-00000bd0: 2020 2020 5429 01da 0c69 676e 6f72 655f      T)...ignore_
-00000be0: 696e 6465 7872 1e00 0000 7226 0000 007a  indexr....r&...z
-00000bf0: 3120 6e6f 7420 696e 2074 6865 2061 7474  1 not in the att
-00000c00: 7269 6275 7465 2074 6162 6c65 206f 6620  ribute table of 
-00000c10: 7072 6f76 6964 6564 2073 6861 7065 6669  provided shapefi
-00000c20: 6c65 7a32 206e 6f74 2069 6e20 7468 6520  lez2 not in the 
-00000c30: 6174 7472 6962 7574 6520 7461 626c 6520  attribute table 
-00000c40: 6f66 2070 726f 7669 6465 6420 696e 666f  of provided info
-00000c50: 2074 6162 6c65 721a 0000 00da 046c 6173   tabler......las
-00000c60: 7429 03da 0673 7562 7365 74da 046b 6565  t)...subset..kee
-00000c70: 7072 2700 0000 5a06 4e65 775f 4944 da05  pr'...Z.New_ID..
-00000c80: 696e 6e65 7229 02da 0368 6f77 da02 6f6e  inner)...how..on
-00000c90: 290f da03 6372 73da 0967 656f 7061 6e64  )...crs..geopand
-00000ca0: 6173 da09 7265 6164 5f66 696c 65da 0674  as..read_file..t
-00000cb0: 6f5f 6372 73da 0765 7870 6c6f 6465 da04  o_crs..explode..
-00000cc0: 636c 6970 da15 636c 6561 6e5f 6765 6f6d  clip..clean_geom
-00000cd0: 6574 7279 5f70 7572 6570 79da 0763 6f6c  etry_purepy..col
-00000ce0: 756d 6e73 da05 7072 696e 74da 0373 7973  umns..print..sys
-00000cf0: da04 6578 6974 721f 0000 00da 0f64 726f  ..exitr......dro
-00000d00: 705f 6475 706c 6963 6174 6573 7213 0000  p_duplicatesr...
-00000d10: 00da 056d 6572 6765 290d da0a 6c61 7965  ...merge)...laye
-00000d20: 725f 7061 7468 da09 436c 6173 735f 436f  r_path..Class_Co
-00000d30: 6cda 0a74 656d 7066 6f6c 6465 72da 0a6d  l..tempfolder..m
-00000d40: 6173 6b5f 6c61 7965 72da 0c43 6c61 7373  ask_layer..Class
-00000d50: 5f4e 4d5f 436f 6cda 0a69 6e66 6f5f 7461  _NM_Col..info_ta
-00000d60: 626c 655a 076e 6577 5f63 7273 da04 6461  bleZ.new_crs..da
-00000d70: 7461 5a09 7072 6f6a 6563 7465 64da 0763  taZ.projected..c
-00000d80: 6c69 7070 6564 da07 636c 6561 6e65 645a  lipped..cleanedZ
-00000d90: 0f69 6e66 6f5f 7461 626c 655f 636f 7079  .info_table_copy
-00000da0: 5a10 696e 666f 5f74 6162 6c65 5f63 6f70  Z.info_table_cop
-00000db0: 7932 720a 0000 0072 0a00 0000 720e 0000  y2r....r....r...
-00000dc0: 00da 2c52 6570 726f 6a5f 436c 6970 5f44  ..,Reproj_Clip_D
-00000dd0: 6973 736f 6c76 655f 5369 6d70 6c69 6679  issolve_Simplify
-00000de0: 5f50 6f6c 7967 6f6e 5f70 7572 6570 7935  _Polygon_purepy5
-00000df0: 0000 0073 3000 0000 0027 0601 0a02 0a01  ...s0....'......
-00000e00: 0c01 0a03 0a01 0a01 0a01 0a01 0801 0a01  ................
-00000e10: 0a01 0801 0a01 0a01 0802 0c01 1201 0c01  ................
-00000e20: 0c01 1a02 1201 0c06 7244 0000 00da 0553  ........rD.....S
-00000e30: 7562 4964 6307 0000 0000 0000 0000 0000  ubIdc...........
-00000e40: 0014 0000 0008 0000 0043 0000 0073 2604  .........C...s&.
-00000e50: 0000 6700 6401 a201 7d07 6402 7c00 6a00  ..g.d...}.d.|.j.
-00000e60: 7600 7218 6403 7d08 6e04 6404 7d08 7401  v.r.d.}.n.d.}.t.
-00000e70: a002 7c08 a101 7d09 7403 7404 6a05 a006  ..|...}.t.t.j...
-00000e80: 7c02 6405 a102 6406 8302 8f1c 7d0a 7c0a  |.d...d.....}.|.
-00000e90: a007 7c09 6a08 a101 0100 5700 6400 0400  ..|.j.....W.d...
-00000ea0: 0400 8303 0100 6e10 3100 735c 3000 0100  ......n.1.s\0...
-00000eb0: 0100 0100 5900 0100 7c04 6407 6b03 9002  ....Y...|.d.k...
-00000ec0: 72c4 7c05 6407 6b03 728e 7409 a00a 7c05  r.|.d.k.r.t...|.
-00000ed0: a101 7d0b 7c0b 6408 1900 7c0b 6409 3c00  ..}.|.d...|.d.<.
-00000ee0: 7c00 6a0b 640a 640b 8d01 6a0c 640c 640d  |.j.d.d...j.d.d.
-00000ef0: 8d01 7d0c 7c05 6407 6b03 72d8 7c0b 640a  ..}.|.d.k.r.|.d.
-00000f00: 6409 6702 1900 7d0b 740d 6a0e 7c0b 7c0c  d.g...}.t.j.|.|.
-00000f10: 6409 640e 640f 8d04 7d0b 7c0b 6a0f 7c06  d.d.d...}.|.j.|.
-00000f20: 6410 6411 6412 8d03 7d0b 7c00 6a0f 7c06  d.d.d...}.|.j.|.
-00000f30: 6410 6411 6412 8d03 7d00 7410 7c00 6413  d.d.d...}.t.|.d.
-00000f40: 6414 8303 7d00 7c00 6414 6413 6702 1900  d...}.|.d.d.g...
-00000f50: 6a0c 640c 640d 8d01 7d0d 7c05 6407 6b03  j.d.d...}.|.d.k.
-00000f60: 9001 722c 7c0b 6a0b 6414 6413 6702 640b  ..r,|.j.d.d.g.d.
-00000f70: 8d01 7d0b 7c0b a006 7c0d a101 7d0b 7c00  ..}.|...|...}.|.
-00000f80: 7c00 6415 1900 6416 6b03 1900 6408 6417  |.d...d.k...d.d.
-00000f90: 6702 1900 6a0c 640c 640d 8d01 7d0e 6700  g...j.d.d...}.g.
-00000fa0: 7d0f 7c0e 6408 1900 6a11 4400 5d20 7d10  }.|.d...j.D.] }.
-00000fb0: 7c10 7c0e 6417 1900 6a11 7601 9001 725a  |.|.d...j.v...rZ
-00000fc0: 7c0f a012 7c10 a101 0100 9001 715a 7c05  |...|.......qZ|.
-00000fd0: 6407 6b03 9001 72da 7c0b 7c0b 6a13 a014  d.k...r.|.|.j...
-00000fe0: 7c0f a101 0f00 1900 7d0b 7c0b 6a00 7d11  |.......}.|.j.}.
-00000ff0: 7c11 7c11 a014 7c07 a101 1900 7d12 7c0b  |.|...|.....}.|.
-00001000: 6a0b 7c12 640b 8d01 7d0b 7415 7c0b 8301  j.|.d...}.t.|...
-00001010: 6418 6b04 9001 72da 7c0b a016 7404 6a05  d.k...r.|...t.j.
-00001020: a006 7c02 7c04 a102 a101 0100 6419 7c00  ..|.|.......d.|.
-00001030: 6a17 7c00 6a13 a014 7c0f a101 641a 6602  j.|.j...|...d.f.
-00001040: 3c00 6419 7c00 6a17 7c00 6a13 a014 7c0f  <.d.|.j.|.j...|.
-00001050: a101 641b 6602 3c00 6419 7c00 6a17 7c00  ..d.f.<.d.|.j.|.
-00001060: 6a13 a014 7c0f a101 641c 6602 3c00 6419  j...|...d.f.<.d.
-00001070: 7c00 6a17 7c00 6a13 a014 7c0f a101 641d  |.j.|.j...|...d.
-00001080: 6602 3c00 6419 7c00 6a17 7c00 6a13 a014  f.<.d.|.j.|.j...
-00001090: 7c0f a101 641e 6602 3c00 6419 7c00 6a17  |...d.f.<.d.|.j.
-000010a0: 7c00 6a13 a014 7c0f a101 641f 6602 3c00  |.j...|...d.f.<.
-000010b0: 7c00 6a00 7d11 7c11 7c11 a014 7c07 a101  |.j.}.|.|...|...
-000010c0: 1900 7d12 7c00 6a0b 7c12 640b 8d01 7d00  ..}.|.j.|.d...}.
-000010d0: 7c00 a016 7404 6a05 a006 7c02 7c03 a102  |...t.j...|.|...
-000010e0: a101 0100 7418 7c00 8301 7d13 7c13 a016  ....t.|...}.|...
-000010f0: 7404 6a05 a006 7c02 6420 a102 a101 0100  t.j...|.d ......
-00001100: 7419 7404 6a05 a006 7c02 7c03 a102 8301  t.t.j...|.|.....
-00001110: 0100 9001 6e5e 7c00 6a0f 7c06 6410 6411  ....n^|.j.|.d.d.
-00001120: 6412 8d03 7d00 6414 7c00 6a00 7600 9003  d...}.d.|.j.v...
-00001130: 72ca 7410 7c00 6413 6414 8303 7d00 7c00  r.t.|.d.d...}.|.
-00001140: 6a1a 7c00 6408 3c00 7c00 7c00 6415 1900  j.|.d.<.|.|.d...
-00001150: 6416 6b03 1900 6408 6417 6702 1900 6a0c  d.k...d.d.g...j.
-00001160: 640c 640d 8d01 7d0e 6700 7d0f 7c0e 6408  d.d...}.g.}.|.d.
-00001170: 1900 6a11 4400 5d20 7d10 7c10 7c0e 6417  ..j.D.] }.|.|.d.
-00001180: 1900 6a11 7601 9003 7224 7c0f a012 7c10  ..j.v...r$|...|.
-00001190: a101 0100 9003 7124 6419 7c00 6a17 7c00  ......q$d.|.j.|.
-000011a0: 6a13 a014 7c0f a101 641a 6602 3c00 6419  j...|...d.f.<.d.
-000011b0: 7c00 6a17 7c00 6a13 a014 7c0f a101 641b  |.j.|.j...|...d.
-000011c0: 6602 3c00 6419 7c00 6a17 7c00 6a13 a014  f.<.d.|.j.|.j...
-000011d0: 7c0f a101 641c 6602 3c00 6419 7c00 6a17  |...d.f.<.d.|.j.
-000011e0: 7c00 6a13 a014 7c0f a101 641d 6602 3c00  |.j...|...d.f.<.
-000011f0: 6419 7c00 6a17 7c00 6a13 a014 7c0f a101  d.|.j.|.j...|...
-00001200: 641e 6602 3c00 6419 7c00 6a17 7c00 6a13  d.f.<.d.|.j.|.j.
-00001210: a014 7c0f a101 641f 6602 3c00 7c00 6a00  ..|...d.f.<.|.j.
-00001220: 7d11 7c11 7c11 a014 6700 6421 a201 a101  }.|.|...g.d!....
-00001230: 1900 7d12 7c00 6a0b 7c12 640b 8d01 7d00  ..}.|.j.|.d...}.
-00001240: 7c00 a016 7404 6a05 a006 7c02 7c03 a102  |...t.j...|.|...
-00001250: a101 0100 7418 7c00 8301 7d13 7c13 a016  ....t.|...}.|...
-00001260: 7404 6a05 a006 7c02 6420 a102 a101 0100  t.j...|.d ......
-00001270: 7c00 5300 6400 5300 2922 4e29 10da 0753  |.S.d.S.)"N)...S
-00001280: 7562 4964 5f31 da02 4964 da07 6e73 7562  ubId_1..Id..nsub
-00001290: 6964 32da 066e 7375 6269 64da 0a6e 646f  id2..nsubid..ndo
-000012a0: 776e 7375 6269 64da 094f 6c64 5f53 7562  wnsubid..Old_Sub
-000012b0: 4964 da0a 4f6c 645f 446f 7753 7562 da0a  Id..Old_DowSub..
-000012c0: 4a6f 696e 5f43 6f75 6e74 da0a 5441 5247  Join_Count..TARG
-000012d0: 4554 5f46 4944 7247 0000 00da 0a53 7562  ET_FIDrG.....Sub
-000012e0: 4944 5f4f 6c64 72da 0a48 5255 5f49 445f  ID_Oldr..HRU_ID_
-000012f0: 4e5f 31da 0a48 5255 5f49 445f 4e5f 32da  N_1..HRU_ID_N_2.
-00001300: 0766 6163 7465 7273 da0c 4f6c 645f 446f  .facters..Old_Do
-00001310: 7753 7562 4964 5a07 5375 6249 6474 325a  wSubIdZ.SubIdt2Z
-00001320: 0844 415f 4368 6e5f 4c7a 4168 7474 7073  .DA_Chn_LzAhttps
-00001330: 3a2f 2f67 6974 6875 622e 636f 6d2f 6475  ://github.com/du
-00001340: 7374 6d69 6e67 2f52 6f75 7469 6e67 546f  stming/RoutingTo
-00001350: 6f6c 2f77 696b 692f 4669 6c65 732f 5245  ol/wiki/Files/RE
-00001360: 4144 4d45 5f4f 4948 2e70 6466 7a40 6874  ADME_OIH.pdfz@ht
-00001370: 7470 733a 2f2f 6769 7468 7562 2e63 6f6d  tps://github.com
-00001380: 2f64 7573 746d 696e 672f 526f 7574 696e  /dustming/Routin
-00001390: 6754 6f6f 6c2f 7769 6b69 2f46 696c 6573  gTool/wiki/Files
-000013a0: 2f52 4541 444d 455f 4e41 2e70 6466 7a0a  /README_NA.pdfz.
-000013b0: 5245 4144 4d45 2e70 6466 da02 7762 7226  README.pdf..wbr&
-000013c0: 0000 0072 4500 0000 724b 0000 00da 0867  ...rE...rK.....g
-000013d0: 656f 6d65 7472 79a9 0172 3500 0000 5472  eometry..r5...Tr
-000013e0: 1a00 0000 da04 6c65 6674 2902 722d 0000  ......left).r-..
-000013f0: 0072 2c00 0000 da05 6669 7273 7446 a903  .r,.....firstF..
-00001400: da02 6279 da07 6167 6766 756e 63da 0861  ..by..aggfunc..a
-00001410: 735f 696e 6465 785a 0a63 656e 7472 6f69  s_indexZ.centroi
-00001420: 645f 785a 0a63 656e 7472 6f69 645f 79da  d_xZ.centroid_y.
-00001430: 084c 616b 655f 4361 74e9 0200 0000 5a08  .Lake_Cat.....Z.
-00001440: 446f 7753 7562 4964 7201 0000 0067 8d97  DowSubIdr....g..
-00001450: 6e12 83c0 f3bf 5a08 5269 7653 6c6f 7065  n.....Z.RivSlope
-00001460: 5a09 5269 764c 656e 6774 685a 0846 6c6f  Z.RivLengthZ.Flo
-00001470: 6f64 505f 6e5a 0443 685f 6e5a 074d 6178  odP_nZ.Ch_nZ.Max
-00001480: 5f44 454d 5a07 4d69 6e5f 4445 4d7a 0b6f  _DEMZ.Min_DEMz.o
-00001490: 7574 6c69 6e65 2e73 6870 290f 5a05 5348  utline.shp).Z.SH
-000014a0: 4150 4572 4600 0000 7247 0000 0072 4800  APErF...rG...rH.
-000014b0: 0000 7249 0000 0072 4a00 0000 724c 0000  ..rI...rJ...rL..
-000014c0: 0072 4d00 0000 724e 0000 0072 4700 0000  .rM...rN...rG...
-000014d0: 724f 0000 0072 5000 0000 7251 0000 0072  rO...rP...rQ...r
-000014e0: 5200 0000 7253 0000 0029 1b72 3500 0000  R...rS...).r5...
-000014f0: da08 7265 7175 6573 7473 da03 6765 74da  ..requests..get.
-00001500: 046f 7065 6eda 026f 73da 0470 6174 68da  .open..os..path.
-00001510: 046a 6f69 6eda 0577 7269 7465 da07 636f  .join..write..co
-00001520: 6e74 656e 7472 2f00 0000 7230 0000 00da  ntentr/...r0....
-00001530: 0464 726f 7072 1f00 0000 7213 0000 0072  .dropr....r....r
-00001540: 3a00 0000 da08 6469 7373 6f6c 7665 da15  :.....dissolve..
-00001550: 6164 645f 6365 6e74 726f 6964 5f69 6e5f  add_centroid_in_
-00001560: 7767 7338 34da 0676 616c 7565 7372 2200  wgs84..valuesr".
-00001570: 0000 7245 0000 0072 2100 0000 7220 0000  ..rE...r!...r ..
-00001580: 00da 0774 6f5f 6669 6c65 da03 6c6f 63da  ...to_file..loc.
-00001590: 1963 7265 6174 655f 7761 7465 7273 6865  .create_watershe
-000015a0: 645f 626f 756e 6461 7279 da15 6372 6561  d_boundary..crea
-000015b0: 7465 5f67 656f 5f6a 6173 6f6e 5f66 696c  te_geo_jason_fil
-000015c0: 65da 0569 6e64 6578 2914 da0e 6d61 706f  e..index)...mapo
-000015d0: 6c64 6e65 775f 696e 666f 723d 0000 00da  ldnew_infor=....
-000015e0: 0c4f 7574 7075 7446 6f6c 6465 72da 0863  .OutputFolder..c
-000015f0: 6174 5f6e 616d 65da 0872 6976 5f6e 616d  at_name..riv_nam
-00001600: 65da 0e50 6174 685f 6669 6e61 6c5f 7269  e..Path_final_ri
-00001610: 76da 0c64 6973 5f63 6f6c 5f6e 616d 655a  v..dis_col_nameZ
-00001620: 124e 4545 445f 544f 5f52 454d 4f56 455f  .NEED_TO_REMOVE_
-00001630: 4944 53da 0375 726c da08 7265 7370 6f6e  IDS..url..respon
-00001640: 7365 da01 665a 0672 6976 5f70 645a 0663  se..fZ.riv_pdZ.c
-00001650: 6174 5f70 645a 0963 6174 5f63 5f78 5f79  at_pdZ.cat_c_x_y
-00001660: 5a19 7269 765f 7064 5f6e 6e63 6c73 5f72  Z.riv_pd_nncls_r
-00001670: 6f75 7469 6e67 5f69 6e66 6f5a 0e72 656d  outing_infoZ.rem
-00001680: 6f76 655f 6368 616e 6e65 6cda 0573 7562  ove_channel..sub
-00001690: 6964 5a0a 6361 745f 636f 6c6e 6d73 5a0f  idZ.cat_colnmsZ.
-000016a0: 6472 6f70 5f63 6174 5f63 6f6c 6e6d 73da  drop_cat_colnms.
-000016b0: 076f 7574 6c69 6e65 720a 0000 0072 0a00  .outliner....r..
-000016c0: 0000 720e 0000 00da 2373 6176 655f 6d6f  ..r.....#save_mo
-000016d0: 6469 6669 6564 5f61 7474 7269 6275 7465  dified_attribute
-000016e0: 735f 746f 5f6f 7574 7075 7473 8000 0000  s_to_outputs....
-000016f0: 738a 0000 0000 0308 030a 0106 0204 020a  s...............
-00001700: 0116 012a 020a 0208 010a 010c 0214 0208  ...*............
-00001710: 010c 0112 0110 0310 010c 0214 010a 0110  ................
-00001720: 010a 0220 0104 010e 0110 010e 010a 0112  ... ............
-00001730: 0106 010e 010c 010e 0114 0216 0116 0116  ................
-00001740: 0116 0116 0116 0206 010e 010c 0114 0208  ................
-00001750: 0114 0116 0410 020c 020c 010a 0120 0104  ............. ..
-00001760: 010e 0110 010e 0216 0116 0116 0116 0116  ................
-00001770: 0116 0306 0112 010c 0114 0108 0114 0172  ...............r
-00001780: 7b00 0000 6301 0000 0000 0000 0000 0000  {...c...........
-00001790: 0002 0000 0005 0000 0043 0000 0073 2e00  .........C...s..
-000017a0: 0000 7c00 6a00 6401 6402 8d01 6403 6701  ..|.j.d.d...d.g.
-000017b0: 1900 7d01 6404 7c01 6405 3c00 7c01 6a01  ..}.d.|.d.<.|.j.
-000017c0: 6405 6406 6407 6408 8d03 7d01 7c01 5300  d.d.d.d...}.|.S.
-000017d0: 2909 4e54 721a 0000 0072 5500 0000 721e  ).NTr....rU...r.
-000017e0: 0000 005a 0249 4472 5800 0000 4672 5900  ...Z.IDrX...FrY.
-000017f0: 0000 2902 721f 0000 0072 6800 0000 2902  ..).r....rh...).
-00001800: 7270 0000 0072 5400 0000 720a 0000 0072  rp...rT...r....r
-00001810: 0a00 0000 720e 0000 0072 6d00 0000 e000  ....r....rm.....
-00001820: 0000 7308 0000 0000 0112 0108 0110 0172  ..s............r
-00001830: 6d00 0000 6302 0000 0000 0000 0000 0000  m...c...........
-00001840: 0005 0000 0005 0000 0043 0000 0073 8400  .........C...s..
-00001850: 0000 7400 a001 7c00 6401 1900 a002 7c01  ..t...|.d.....|.
-00001860: a101 a101 7d02 7c00 6402 1900 6403 6b03  ....}.|.d...d.k.
-00001870: 7d03 7400 a003 7c02 7c03 a102 7d04 6404  }.t...|.|...}.d.
-00001880: 7c00 6a04 7c04 6401 6602 3c00 6404 7c00  |.j.|.d.f.<.d.|.
-00001890: 6a04 7c04 6405 6602 3c00 6404 7c00 6a04  j.|.d.f.<.d.|.j.
-000018a0: 7c04 6406 6602 3c00 6404 7c00 6a04 7c04  |.d.f.<.d.|.j.|.
-000018b0: 6407 6602 3c00 6404 7c00 6a04 7c04 6408  d.f.<.d.|.j.|.d.
-000018c0: 6602 3c00 6404 7c00 6a04 7c04 6402 6602  f.<.d.|.j.|.d.f.
-000018d0: 3c00 7c00 5300 2909 7af1 4675 6e63 7469  <.|.S.).z.Functi
-000018e0: 6f6e 7320 7769 6c6c 2073 6574 206c 616b  ons will set lak
-000018f0: 6520 6964 206e 6f74 2069 6e20 436f 6e6e  e id not in Conn
-00001900: 5f4c 616b 655f 4964 7320 746f 202d 312e  _Lake_Ids to -1.
-00001910: 3233 3435 2069 6e20 6174 7472 6962 7574  2345 in attribut
-00001920: 650a 2020 2020 2020 2020 7461 626c 6520  e.        table 
-00001930: 6f66 2050 6174 685f 4669 6e61 6c63 6174  of Path_Finalcat
-00001940: 696e 666f 0a20 2020 202d 2d2d 2d2d 2d2d  info.    -------
-00001950: 2d2d 2d0a 0a20 2020 204e 6f74 6573 0a20  ---..    Notes. 
-00001960: 2020 202d 2d2d 2d2d 2d2d 0a0a 2020 2020     -------..    
-00001970: 5265 7475 726e 733a 0a20 2020 202d 2d2d  Returns:.    ---
-00001980: 2d2d 2d2d 0a20 2020 2020 2020 204e 6f6e  ----.        Non
-00001990: 652c 2074 6865 2061 7474 7269 6275 7465  e, the attribute
-000019a0: 2074 6162 6c65 206f 6620 5061 7468 5f73   table of Path_s
-000019b0: 6870 6669 6c65 2077 696c 6c20 6265 2075  hpfile will be u
-000019c0: 7064 6174 6564 0a20 2020 20da 0848 794c  pdated.    ..HyL
-000019d0: 616b 6549 6472 5d00 0000 725e 0000 0072  akeIdr]...r^...r
-000019e0: 0100 0000 5a07 4c61 6b65 566f 6c5a 084c  ....Z.LakeVolZ.L
-000019f0: 616b 6541 7265 615a 094c 616b 6544 6570  akeAreaZ.LakeDep
-00001a00: 7468 5a08 4c61 6b65 7479 7065 2905 da02  thZ.Laketype)...
-00001a10: 6e70 da0b 6c6f 6769 6361 6c5f 6e6f 7472  np..logical_notr
-00001a20: 2100 0000 da0b 6c6f 6769 6361 6c5f 616e  !.....logical_an
-00001a30: 6472 6c00 0000 2905 5a0c 6669 6e61 6c63  drl...).Z.finalc
-00001a40: 6174 5f70 6c79 5a0d 436f 6e6e 5f4c 616b  at_plyZ.Conn_Lak
-00001a50: 655f 4964 73da 056d 6173 6b31 da05 6d61  e_Ids..mask1..ma
-00001a60: 736b 32da 046d 6173 6b72 0a00 0000 720a  sk2..maskr....r.
-00001a70: 0000 0072 0e00 0000 da37 5265 6d6f 7665  ...r.....7Remove
-00001a80: 5f55 6e73 656c 6563 7465 645f 4c61 6b65  _Unselected_Lake
-00001a90: 5f41 7474 7269 6275 7465 5f49 6e5f 4669  _Attribute_In_Fi
-00001aa0: 6e61 6c63 6174 696e 666f 5f70 7572 6570  nalcatinfo_purep
-00001ab0: 79e6 0000 0073 1400 0000 000d 1401 0c01  y....s..........
-00001ac0: 0c02 0e01 0e01 0e01 0e01 0e01 0e02 7283  ..............r.
-00001ad0: 0000 0063 0200 0000 0000 0000 0000 0000  ...c............
-00001ae0: 0300 0000 0700 0000 4300 0000 732a 0000  ........C...s*..
-00001af0: 007c 006a 0074 01a0 0274 01a0 037c 006a  .|.j.t...t...|.j
-00001b00: 007c 01a1 02a1 0119 007d 027c 006a 047c  .|.......}.|.j.|
-00001b10: 0264 018d 017d 007c 0053 0029 024e 7256  .d...}.|.S.).NrV
-00001b20: 0000 0029 0572 3500 0000 727d 0000 0072  ...).r5...r}...r
-00001b30: 7e00 0000 7221 0000 0072 6700 0000 2903  ~...r!...rg...).
-00001b40: da05 7461 626c 65da 056e 616d 6573 5a13  ..table..namesZ.
-00001b50: 7265 6d6f 7665 5f63 6f6c 756d 6e5f 6e61  remove_column_na
-00001b60: 6d65 7372 0a00 0000 720a 0000 0072 0e00  mesr....r....r..
-00001b70: 0000 da1b 636c 6561 6e5f 6174 7472 6962  ....clean_attrib
-00001b80: 7574 655f 6e61 6d65 5f70 7572 6570 7900  ute_name_purepy.
-00001b90: 0100 0073 0600 0000 0001 1a01 0c01 7286  ...s..........r.
-00001ba0: 0000 00e9 ffff ffff 6302 0000 0000 0000  ........c.......
-00001bb0: 0000 0000 0007 0000 0004 0000 0043 0000  .............C..
-00001bc0: 0073 ca00 0000 7c01 6401 6b04 721a 7c00  .s....|.d.k.r.|.
-00001bd0: 6402 1900 a000 6403 a101 7c00 6402 3c00  d.....d...|.d.<.
-00001be0: 7c00 6402 1900 a001 a100 0f00 7d02 7c00  |.d.........}.|.
-00001bf0: 6a02 0f00 7d03 7c00 6a03 6401 6b04 7d04  j...}.|.j.d.k.}.
-00001c00: 7404 a005 7c02 7c03 a102 7d05 7404 a005  t...|.|...}.t...
-00001c10: 7c04 7c05 a102 7d06 7c00 6a06 7c06 1900  |.|...}.|.j.|...
-00001c20: 7d00 7c00 6a06 7c00 6a07 6404 6b03 1900  }.|.j.|.j.d.k...
-00001c30: 7d00 7408 7c00 6a06 7c00 6a07 6405 6b02  }.t.|.j.|.j.d.k.
-00001c40: 1900 8301 6401 6b04 72b0 7409 6406 8301  ....d.k.r.t.d...
-00001c50: 0100 7409 6407 8301 0100 7409 7c00 6a06  ..t.d.....t.|.j.
-00001c60: 7c00 6a07 6405 6b02 1900 8301 0100 7409  |.j.d.k.......t.
-00001c70: 6406 8301 0100 7c00 6a06 7c00 6a07 6405  d.....|.j.|.j.d.
-00001c80: 6b03 1900 7d00 7c00 6a0a 0100 7c00 5300  k...}.|.j...|.S.
-00001c90: 2908 4e72 0100 0000 7255 0000 0067 9564  ).Nr....rU...g.d
-00001ca0: 79e1 7ffd a53d da05 506f 696e 74da 1247  y....=..Point..G
-00001cb0: 656f 6d65 7472 7943 6f6c 6c65 6374 696f  eometryCollectio
-00001cc0: 6e7a 1b23 2323 2323 2323 2323 2323 2323  nz.#############
-00001cd0: 2323 2323 2323 2323 2323 2323 2323 7a1c  ##############z.
-00001ce0: 6368 6563 6b20 7468 6520 666f 6c6c 6f77  check the follow
-00001cf0: 696e 6720 6665 6174 7572 6573 290b da06  ing features)...
-00001d00: 6275 6666 6572 da04 6973 6e61 da08 6973  buffer..isna..is
-00001d10: 5f65 6d70 7479 da04 6172 6561 727d 0000  _empty..arear}..
-00001d20: 0072 7f00 0000 726c 0000 00da 0967 656f  .r....rl.....geo
-00001d30: 6d5f 7479 7065 7220 0000 0072 3600 0000  m_typer ...r6...
-00001d40: da06 7369 6e64 6578 2907 7241 0000 00da  ..sindex).rA....
-00001d50: 0d73 6574 5f70 7265 6369 7369 6f6e 5a05  .set_precisionZ.
-00001d60: 6e61 726f 775a 0565 6d72 6f77 5a07 6172  narowZ.emrowZ.ar
-00001d70: 6561 726f 775a 0472 6f77 315a 0972 6f77  earowZ.row1Z.row
-00001d80: 7365 6c65 6374 720a 0000 0072 0a00 0000  selectr....r....
-00001d90: 720e 0000 0072 3400 0000 0501 0000 7322  r....r4.......s"
-00001da0: 0000 0000 0308 0112 060e 0208 020a 030c  ................
-00001db0: 010c 030a 0210 0118 0108 0108 0114 0108  ................
-00001dc0: 0210 0106 0272 3400 0000 6303 0000 0000  .....r4...c.....
-00001dd0: 0000 0000 0000 0006 0000 0003 0000 0043  ...............C
-00001de0: 0000 0073 3800 0000 7c00 6a00 7d03 7c00  ...s8...|.j.}.|.
-00001df0: a001 a100 7d04 7c00 a002 7c01 a101 7d04  ....}.|...|...}.
-00001e00: 7c04 6a03 7c04 7c02 3c00 7c04 6a01 6401  |.j.|.|.<.|.j.d.
-00001e10: 6402 8d01 a002 7c03 a101 7d05 7c05 5300  d.....|...}.|.S.
-00001e20: 2903 4e54 721a 0000 0029 0472 2e00 0000  ).NTr....).r....
-00001e30: 721f 0000 0072 3100 0000 728d 0000 0029  r....r1...r....)
-00001e40: 0672 4100 0000 da07 7072 6a5f 6372 735a  .rA.....prj_crsZ
-00001e50: 0861 7265 615f 636f 6cda 0773 7263 5f73  .area_col..src_s
-00001e60: 7263 da04 746f 7374 da03 6f75 7472 0a00  rc..tost..outr..
-00001e70: 0000 720a 0000 0072 0e00 0000 da0e 6164  ..r....r......ad
-00001e80: 645f 6172 6561 5f69 6e5f 6d32 2801 0000  d_area_in_m2(...
-00001e90: 730c 0000 0000 0106 0108 020a 010a 0212  s...............
-00001ea0: 0272 9500 0000 6303 0000 0000 0000 0000  .r....c.........
-00001eb0: 0000 0006 0000 0003 0000 0043 0000 0073  ...........C...s
-00001ec0: 4a00 0000 7c00 6a00 7d03 7c00 a001 a100  J...|.j.}.|.....
-00001ed0: 7d04 7c04 a002 6401 a101 7d04 7c04 6a03  }.|...d...}.|.j.
-00001ee0: 6a04 6a05 7c04 7c02 3c00 7c04 6a03 6a04  j.j.|.|.<.|.j.j.
-00001ef0: 6a06 7c04 7c01 3c00 7c04 6a01 6402 6403  j.|.|.<.|.j.d.d.
-00001f00: 8d01 a002 7c03 a101 7d05 7c05 5300 2904  ....|...}.|.S.).
-00001f10: 4efa 0945 5053 473a 3433 3236 5472 1a00  N..EPSG:4326Tr..
-00001f20: 0000 2907 722e 0000 0072 1f00 0000 7231  ..).r....r....r1
-00001f30: 0000 0072 5500 0000 da08 6365 6e74 726f  ...rU.....centro
-00001f40: 6964 da01 7972 0b00 0000 2906 7241 0000  id..yr....).rA..
-00001f50: 005a 0463 6f6c 785a 0463 6f6c 7972 9200  .Z.colxZ.colyr..
-00001f60: 0000 7293 0000 0072 9400 0000 720a 0000  ..r....r....r...
-00001f70: 0072 0a00 0000 720e 0000 0072 6900 0000  .r....r....ri...
-00001f80: 3301 0000 730e 0000 0000 0106 0108 020a  3...s...........
-00001f90: 020e 010e 0212 0272 6900 0000 6301 0000  .......ri...c...
-00001fa0: 0000 0000 0000 0000 001c 0000 0008 0000  ................
-00001fb0: 0043 0000 0073 7e03 0000 6401 7c00 7601  .C...s~...d.|.v.
-00001fc0: 720c 6400 5300 7400 6a01 a002 7c00 a101  r.d.S.t.j...|...
-00001fd0: 7d01 7400 6a01 a003 7c00 a101 a004 6402  }.t.j...|.....d.
-00001fe0: a101 7d02 7405 7c02 8301 7d03 7c02 7c03  ..}.t.|...}.|.|.
-00001ff0: 6403 1800 1900 6404 6405 8502 1900 7d04  d.....d.d.....}.
-00002000: 6406 6407 6702 7d05 6401 7d06 6408 7d07  d.d.g.}.d.}.d.}.
-00002010: 6409 7d08 640a 7d09 6700 7d0a 6700 7d0b  d.}.d.}.g.}.g.}.
-00002020: 640b 7c04 7600 72e8 7c06 6402 1700 7c04  d.|.v.r.|.d...|.
-00002030: 1700 640c 1700 7c07 6402 1700 7c04 1700  ..d...|.d...|...
-00002040: 640c 1700 7c08 6402 1700 7c04 1700 640c  d...|.d...|...d.
-00002050: 1700 7c09 6402 1700 7c04 1700 640c 1700  ..|.d...|...d...
-00002060: 6704 7d0a 7c06 6402 1700 7c04 1700 640d  g.}.|.d...|...d.
-00002070: 1700 7c07 6402 1700 7c04 1700 640d 1700  ..|.d...|...d...
-00002080: 7c08 6402 1700 7c04 1700 640d 1700 7c09  |.d...|...d...|.
-00002090: 6402 1700 7c04 1700 640d 1700 6704 7d0b  d...|...d...g.}.
-000020a0: 6e38 7c06 640c 1700 7c07 640c 1700 7c08  n8|.d...|.d...|.
-000020b0: 640c 1700 7c09 640c 1700 6704 7d0a 7c06  d...|.d...g.}.|.
-000020c0: 640d 1700 7c07 640d 1700 7c08 640d 1700  d...|.d...|.d...
-000020d0: 7c09 640d 1700 6704 7d0b 6700 7d0c 6700  |.d...g.}.g.}.g.
-000020e0: 7d0d 7406 6404 7405 7c0a 8301 8302 4400  }.t.d.t.|.....D.
-000020f0: 9001 5d2e 7d0e 7400 6a01 a007 7c01 7c0a  ..].}.t.j...|.|.
-00002100: 7c0e 1900 a102 7d0f 7400 6a01 a007 7c01  |.....}.t.j...|.
-00002110: 7c0b 7c0e 1900 a102 7d10 7400 6a01 a008  |.|.....}.t.j...
-00002120: 7c0f a101 9001 7372 9001 7136 7c0c a009  |.....sr..q6|...
-00002130: 7c10 a101 0100 6408 7c0a 7c0e 1900 7600  |.....d.|.|...v.
-00002140: 9001 7398 640e 7c0a 7c0e 1900 7600 9001  ..s.d.|.|...v...
-00002150: 72a2 7c0d a009 7c10 a101 0100 740a a00b  r.|...|.....t...
-00002160: 7c0f a101 7d11 7c11 a00c 640f a101 7d12  |...}.|...d...}.
-00002170: 6401 7c0a 7c0e 1900 7600 9001 73d2 6408  d.|.|...v...s.d.
-00002180: 7c0a 7c0e 1900 7600 9002 7214 7c12 6410  |.|...v...r.|.d.
-00002190: 1900 a00d 740e a101 a00d 740f a101 7c12  ....t.....t...|.
-000021a0: 6411 3c00 7c12 6a10 4400 5d22 7d13 6412  d.<.|.j.D.]"}.d.
-000021b0: 7c12 6a11 7c13 6411 6602 1900 1700 7c12  |.j.|.d.f.....|.
-000021c0: 6a11 7c13 6411 6602 3c00 9001 71f0 7c12  j.|.d.f.<...q.|.
-000021d0: 7d14 7c05 4400 5d46 7d15 7c14 a012 7c15  }.|.D.]F}.|...|.
-000021e0: a101 7c14 6413 3c00 7c14 6a13 7c10 6414  ..|.d.<.|.j.|.d.
-000021f0: 6415 8d02 0100 7400 a014 7c10 a101 6a15  d.....t...|...j.
-00002200: 6416 1b00 6416 1b00 7d16 7c16 6417 6b01  d...d...}.|.d.k.
-00002210: 9002 721c 0100 9001 7136 9002 711c 9001  ..r.....q6..q...
-00002220: 7136 7405 7c0d 8301 6403 6b04 9003 727a  q6t.|...d.k...rz
-00002230: 7400 a014 7400 6a01 a007 7c01 7c0b 6404  t...t.j...|.|.d.
-00002240: 1900 a102 a101 6a15 6416 1b00 6416 1b00  ......j.d...d...
-00002250: 6418 6b00 9003 727a 7406 6404 7405 7c0d  d.k...rzt.d.t.|.
-00002260: 8301 8302 4400 5d80 7d0e 7416 7417 7c0d  ....D.].}.t.t.|.
-00002270: 7c0e 1900 8301 8301 7d17 6408 7c0d 7c0e  |.......}.d.|.|.
-00002280: 1900 7600 9003 7206 6700 7d18 7c17 6419  ..v...r.g.}.|.d.
-00002290: 1900 4400 5d22 7d19 7c19 641a 1900 641b  ..D.]"}.|.d...d.
-000022a0: 1900 6404 6b02 9002 72da 7c18 a009 7c19  ..d.k...r.|...|.
-000022b0: a101 0100 9002 71da 7c18 7c17 6419 3c00  ......q.|.|.d.<.
-000022c0: 7c0e 6404 6b02 9003 7216 7c17 7d1a 6e14  |.d.k...r.|.}.n.
-000022d0: 7c1a 6419 0500 1900 7c17 6419 1900 3700  |.d.....|.d...7.
-000022e0: 0300 3c00 9002 71ac 7417 7400 6a01 a007  ..<...q.t.t.j...
-000022f0: 7c01 641c a102 641d 641e 641f 8d03 8f22  |.d...d.d.d...."
-00002300: 7d1b 7418 6a19 7c1a 7c1b 6420 6405 6421  }.t.j.|.|.d d.d!
-00002310: 8d04 0100 5700 6400 0400 0400 8303 0100  ....W.d.........
-00002320: 6e12 3100 9003 7370 3000 0100 0100 0100  n.1...sp0.......
-00002330: 5900 0100 6400 5300 2922 4e5a 0d66 696e  Y...d.S.)"NZ.fin
-00002340: 616c 6361 745f 696e 666f da01 5f72 1e00  alcat_info.._r..
-00002350: 0000 7201 0000 00e9 0400 0000 672d 431c  ..r.........g-C.
-00002360: ebe2 361a 3f67 7b14 ae47 e17a 743f 5a11  ..6.?g{..G.zt?Z.
-00002370: 6669 6e61 6c63 6174 5f69 6e66 6f5f 7269  finalcat_info_ri
-00002380: 76da 1173 6c5f 636f 6e6e 6563 7465 645f  v..sl_connected_
-00002390: 6c61 6b65 da15 736c 5f6e 6f6e 5f63 6f6e  lake..sl_non_con
-000023a0: 6e65 6374 6564 5f6c 616b 65da 0176 7a04  nected_lake..vz.
-000023b0: 2e73 6870 7a08 2e67 656f 6a73 6f6e 5a0e  .shpz..geojsonZ.
-000023c0: 636f 6e6e 6563 7465 645f 6c61 6b65 7296  connected_laker.
-000023d0: 0000 0072 4500 0000 5a07 7276 684e 616d  ...rE...Z.rvhNam
-000023e0: 65da 0373 7562 7255 0000 00da 0747 656f  e..subrU.....Geo
-000023f0: 4a53 4f4e 2901 da06 6472 6976 6572 6900  JSON)...driveri.
-00002400: 0400 00e9 6400 0000 69f4 0100 00da 0866  ....d...i......f
-00002410: 6561 7475 7265 7372 0800 0000 725d 0000  eaturesr....r]..
-00002420: 007a 2272 6f75 7469 6e67 5f70 726f 6475  .z"routing_produ
-00002430: 6374 5f6c 616b 655f 7269 7665 722e 6765  ct_lake_river.ge
-00002440: 6f6a 736f 6eda 0177 7a05 7574 662d 3829  ojson..wz.utf-8)
-00002450: 01da 0865 6e63 6f64 696e 6746 2902 da0c  ...encodingF)...
-00002460: 656e 7375 7265 5f61 7363 6969 da06 696e  ensure_ascii..in
-00002470: 6465 6e74 291a 7262 0000 0072 6300 0000  dent).rb...rc...
-00002480: da07 6469 726e 616d 65da 0862 6173 656e  ..dirname..basen
-00002490: 616d 65da 0573 706c 6974 7220 0000 00da  ame..splitr ....
-000024a0: 0572 616e 6765 7264 0000 00da 0665 7869  .rangerd.....exi
-000024b0: 7374 7372 2200 0000 722f 0000 0072 3000  stsr"...r/...r0.
-000024c0: 0000 7231 0000 00da 0661 7374 7970 65da  ..r1.....astype.
-000024d0: 0369 6e74 da03 7374 7272 6f00 0000 726c  .int..strro...rl
-000024e0: 0000 00da 0873 696d 706c 6966 7972 6b00  .....simplifyrk.
-000024f0: 0000 da04 7374 6174 da07 7374 5f73 697a  ....stat..st_siz
-00002500: 6572 0200 0000 7261 0000 00da 046a 736f  er....ra.....jso
-00002510: 6eda 0464 756d 7029 1c5a 1249 6e70 7574  n..dump).Z.Input
-00002520: 5f50 6f6c 7967 6f6e 5f70 6174 685a 0b70  _Polygon_pathZ.p
-00002530: 726f 6475 6374 5f64 6972 5a08 4e61 6d65  roduct_dirZ.Name
-00002540: 735f 696e 5a07 6e5f 6368 6172 63da 0776  s_inZ.n_charc..v
-00002550: 6572 7369 6f6e da0a 544f 4c45 5241 4e43  ersion..TOLERANC
-00002560: 4573 5a0d 6865 6164 5f6e 616d 655f 6361  EsZ.head_name_ca
-00002570: 745a 0d68 6561 645f 6e61 6d65 5f72 6976  tZ.head_name_riv
-00002580: 5a0f 6865 6164 5f6e 616d 655f 736c 616b  Z.head_name_slak
-00002590: 655a 0f68 6561 645f 6e61 6d65 5f6e 6c61  eZ.head_name_nla
-000025a0: 6b65 5a0f 496e 7075 745f 6669 6c65 5f6e  keZ.Input_file_n
-000025b0: 616d 655a 104f 7574 7075 745f 6669 6c65  ameZ.Output_file
-000025c0: 5f6e 616d 655a 1363 7265 6174 6564 5f6a  _nameZ.created_j
-000025d0: 6173 6f6e 5f66 696c 6573 5a1c 6372 6561  ason_filesZ.crea
-000025e0: 7465 645f 6a61 736f 6e5f 6669 6c65 735f  ted_jason_files_
-000025f0: 6c61 6b65 5f72 6976 7224 0000 005a 0a69  lake_rivr$...Z.i
-00002600: 6e70 7574 5f70 6174 68da 116f 7574 7075  nput_path..outpu
-00002610: 745f 6a61 736f 6e5f 7061 7468 5a08 696e  t_jason_pathZ.in
-00002620: 7075 745f 7064 5a0c 696e 7075 745f 7767  put_pdZ.input_wg
-00002630: 735f 3834 da03 6964 785a 0c69 6e70 7574  s_84..idxZ.input
-00002640: 5f74 6f6a 736f 6eda 0954 4f4c 4552 414e  _tojson..TOLERAN
-00002650: 4345 da0e 6a73 6f6e 5f66 696c 655f 7369  CE..json_file_si
-00002660: 7a65 5a07 696e 6a73 6f6e 325a 0c6e 6577  zeZ.injson2Z.new
-00002670: 5f66 6561 7475 7265 73da 0765 6c65 6d65  _features..eleme
-00002680: 6e74 5a15 6f75 7470 7574 5f6a 6173 6f6e  ntZ.output_jason
-00002690: 5f6c 616b 655f 7269 7672 7800 0000 720a  _lake_rivrx...r.
-000026a0: 0000 0072 0a00 0000 720e 0000 0072 6e00  ...r....r....rn.
-000026b0: 0000 4101 0000 7390 0000 0000 0208 0204  ..A...s.........
-000026c0: 020c 0112 0108 0114 0108 0304 0104 0104  ................
-000026d0: 0104 0204 0104 0108 020e 010e 010e 010e  ................
-000026e0: fc04 070e 010e 010e 010e fc06 0806 0106  ................
-000026f0: 0106 0106 fc04 0706 0106 0106 0106 fc04  ................
-00002700: 0604 0104 0214 0112 0112 010e 0104 010a  ................
-00002710: 021c 010a 030a 020a 041c 0118 010a 0120  ............... 
-00002720: 0304 0208 010e 010e 0214 010a 010e 0236  ...............6
-00002730: 0112 0110 010e 0104 010c 0112 010e 0108  ................
-00002740: 020a 0106 0218 021a 0132 0272 6e00 0000  .........2.rn...
-00002750: 2902 7226 0000 0072 2600 0000 2901 7245  ).r&...r&...).rE
-00002760: 0000 0029 0172 8700 0000 291b 722f 0000  ...).r....).r/..
-00002770: 00da 056e 756d 7079 727d 0000 0072 6200  ...numpyr}...rb.
-00002780: 0000 da06 7061 6e64 6173 7213 0000 0072  ....pandasr....r
-00002790: b200 0000 7202 0000 0072 0300 0000 725f  ....r....r....r_
-000027a0: 0000 0072 3700 0000 da05 6f73 6765 6f72  ...r7.....osgeor
-000027b0: 0400 0000 7205 0000 005a 0b72 6173 7465  ....r....Z.raste
-000027c0: 7273 7461 7473 7206 0000 0072 1900 0000  rstatsr....r....
-000027d0: 7225 0000 0072 4400 0000 727b 0000 0072  r%...rD...r{...r
-000027e0: 6d00 0000 7283 0000 0072 8600 0000 7234  m...r....r....r4
-000027f0: 0000 0072 9500 0000 7269 0000 0072 6e00  ...r....ri...rn.
-00002800: 0000 720a 0000 0072 0a00 0000 720a 0000  ..r....r....r...
-00002810: 0072 0e00 0000 da08 3c6d 6f64 756c 653e  .r......<module>
-00002820: 0100 0000 732a 0000 0008 0108 0108 0108  ....s*..........
-00002830: 0110 0108 0108 0108 0310 010c 0208 0c08  ................
-00002840: 1c00 ff0a 4b0a 6008 0608 1a08 050a 2308  ....K.`.......#.
-00002850: 0b08 0e                                  ...
+000000f0: 641e 641f 8400 5a1b 6420 6421 8400 5a1c  d.d...Z.d d!..Z.
+00000100: 6422 6423 8400 5a1d 6401 5300 2927 e900  d"d#..Z.d.S.)'..
+00000110: 0000 004e 2902 da04 6c6f 6164 da0b 4a53  ...N)...load..JS
+00000120: 4f4e 456e 636f 6465 7229 02da 0467 6461  ONEncoder)...gda
+00000130: 6cda 036f 6772 2901 da0b 7a6f 6e61 6c5f  l..ogr)...zonal_
+00000140: 7374 6174 7363 0400 0000 0000 0000 0000  statsc..........
+00000150: 0000 0700 0000 0700 0000 0300 0000 7336  ..............s6
+00000160: 0000 0074 007c 007c 017c 0264 0164 0164  ...t.|.|.|.d.d.d
+00000170: 028d 057d 0474 0174 0287 0066 0164 0364  ...}.t.t...f.d.d
+00000180: 0484 087c 0483 0283 017d 0574 03a0 047c  ...|.....}.t...|
+00000190: 05a1 017d 067c 0653 0029 054e 5429 03da  ...}.|.S.).NT)..
+000001a0: 0573 7461 7473 5a0b 6765 6f6a 736f 6e5f  .statsZ.geojson_
+000001b0: 6f75 745a 0b61 6c6c 5f74 6f75 6368 6564  outZ.all_touched
+000001c0: 6301 0000 0000 0000 0000 0000 0001 0000  c...............
+000001d0: 0005 0000 0013 0000 0073 1c00 0000 8800  .........s......
+000001e0: 7c00 6401 1900 8800 1900 6402 7c00 6401  |.d.......d.|.d.
+000001f0: 1900 6402 1900 6902 5300 2903 4eda 0a70  ..d...i.S.).N..p
+00000200: 726f 7065 7274 6965 73da 046d 6561 6ea9  roperties..mean.
+00000210: 0029 01da 0178 a901 da03 6b65 7972 0a00  .)...x....keyr..
+00000220: 0000 fa47 633a 5c75 7365 7273 5c6d 3433  ...Gc:\users\m43
+00000230: 6861 6e5f 325c 646f 6375 6d65 6e74 735c  han_2\documents\
+00000240: 6769 7468 7562 5c62 6173 696e 6d61 6b65  github\basinmake
+00000250: 725c 6261 7369 6e6d 616b 6572 5c66 756e  r\basinmaker\fun
+00000260: 635c 7075 7265 7079 2e70 79da 083c 6c61  c\purepy.py..<la
+00000270: 6d62 6461 3e11 0000 00f3 0000 0000 7a20  mbda>.........z 
+00000280: 7a6f 6e61 6c5f 7374 6174 735f 7064 2e3c  zonal_stats_pd.<
+00000290: 6c6f 6361 6c73 3e2e 3c6c 616d 6264 613e  locals>.<lambda>
+000002a0: 2905 7206 0000 00da 046c 6973 74da 036d  ).r......list..m
+000002b0: 6170 da02 7064 da09 4461 7461 4672 616d  ap..pd..DataFram
+000002c0: 6529 07da 0773 6870 5f67 7064 da06 7261  e)...shp_gpd..ra
+000002d0: 7374 6572 7207 0000 0072 0d00 0000 da06  sterr....r......
+000002e0: 7265 7375 6c74 5a0f 7265 6175 6c74 5f6c  resultZ.reault_l
+000002f0: 6973 745f 6469 63da 0972 6561 756c 745f  ist_dic..reault_
+00000300: 7064 720a 0000 0072 0c00 0000 720e 0000  pdr....r....r...
+00000310: 00da 0e7a 6f6e 616c 5f73 7461 7473 5f70  ...zonal_stats_p
+00000320: 640d 0000 0073 0800 0000 0002 1202 1602  d....s..........
+00000330: 0a02 7219 0000 0063 0500 0000 0000 0000  ..r....c........
+00000340: 0000 0000 0b00 0000 0500 0000 4300 0000  ............C...
+00000350: 73ce 0000 007c 006a 0064 0164 028d 017d  s....|.j.d.d...}
+00000360: 0564 037d 0674 017c 0583 0164 036b 0472  .d.}.t.|...d.k.r
+00000370: a87c 0664 046b 0172 a874 027c 057c 017c  .|.d.k.r.t.|.|.|
+00000380: 027c 0383 047d 077c 077c 0764 0519 0064  .|...}.|.|.d...d
+00000390: 036b 040f 0019 0064 0619 007d 087c 057c  .k.....d...}.|.|
+000003a0: 0564 0619 00a0 037c 08a1 0119 006a 0064  .d.....|.....j.d
+000003b0: 0164 028d 017d 057c 0664 036b 0272 847c  .d...}.|.d.k.r.|
+000003c0: 077c 0764 0519 0064 036b 0419 007d 097c  .|.d...d.k...}.|
+000003d0: 0664 0717 007d 0671 107c 0664 0717 007d  .d...}.q.|.d...}
+000003e0: 067c 077c 0764 0519 0064 036b 0419 007d  .|.|.d...d.k...}
+000003f0: 0a7c 09a0 047c 0aa1 017d 0971 1074 017c  .|...|...}.q.t.|
+00000400: 0583 0164 036b 0472 ca7c 057c 0419 007c  ...d.k.r.|.|...|
+00000410: 0564 053c 007c 09a0 047c 05a1 017d 097c  .d.<.|...|...}.|
+00000420: 0953 0029 084e 54a9 01da 0464 6565 7072  .S.).NT....deepr
+00000430: 0100 0000 e905 0000 0072 0900 0000 da0a  .........r......
+00000440: 4852 555f 4944 5f4e 6577 e901 0000 0029  HRU_ID_New.....)
+00000450: 05da 0463 6f70 79da 036c 656e 7219 0000  ...copy..lenr...
+00000460: 00da 0469 7369 6eda 0661 7070 656e 6429  ...isin..append)
+00000470: 0b72 1500 0000 7216 0000 0072 0700 0000  .r....r....r....
+00000480: 720d 0000 00da 0363 6f6c 5a09 6e6f 6461  r......colZ.noda
+00000490: 7461 5f70 64da 0169 5a07 7465 6d70 5f70  ta_pd..iZ.temp_p
+000004a0: 645a 0e62 6164 5f68 7275 5f76 616c 7565  dZ.bad_hru_value
+000004b0: 7372 1800 0000 5a07 676f 6f64 5f70 6472  sr....Z.good_pdr
+000004c0: 0a00 0000 720a 0000 0072 0e00 0000 da0a  ....r....r......
+000004d0: 5a6f 6e61 6c53 7461 7473 1900 0000 7320  ZonalStats....s 
+000004e0: 0000 0000 060c 0104 0114 010e 0116 011a  ................
+000004f0: 0108 0110 010a 0208 0110 010c 020c 010c  ................
+00000500: 010a 0272 2500 0000 fa01 2363 0600 0000  ...r%.....#c....
+00000510: 0000 0000 0000 0000 0d00 0000 0600 0000  ................
+00000520: 4300 0000 730a 0100 007c 036a 007d 0674  C...s....|.j.}.t
+00000530: 01a0 027c 00a1 017d 077c 07a0 037c 06a1  ...|...}.|...|..
+00000540: 017d 087c 086a 0464 0164 028d 017d 087c  .}.|.j.d.d...}.|
+00000550: 08a0 057c 03a1 017d 0974 067c 0964 0383  ...|...}.t.|.d..
+00000560: 027d 0a7c 0464 046b 0390 0172 067c 017c  .}.|.d.k...r.|.|
+00000570: 096a 0776 0172 6074 087c 0164 0583 0201  .j.v.r`t.|.d....
+00000580: 0074 09a0 0aa1 0001 007c 017c 056a 0776  .t.......|.|.j.v
+00000590: 0172 7c74 087c 0164 0683 0201 0074 09a0  .r|t.|.d.....t..
+000005a0: 0aa1 0001 007c 047c 056a 0776 0172 9874  .....|.|.j.v.r.t
+000005b0: 087c 0464 0683 0201 0074 09a0 0aa1 0001  .|.d.....t......
+000005c0: 007c 056a 0b64 0164 078d 017d 0b7c 0b6a  .|.j.d.d...}.|.j
+000005d0: 0c7c 0467 0164 0864 0164 098d 037d 0b7c  .|.g.d.d.d...}.|
+000005e0: 0b7c 0119 007c 0b64 0a3c 007c 0b7c 0464  .|...|.d.<.|.|.d
+000005f0: 0a67 0219 007d 0b74 0d6a 0e7c 057c 0b64  .g...}.t.j.|.|.d
+00000600: 0b7c 0464 0c8d 046a 0b64 0164 078d 017d  .|.d...j.d.d...}
+00000610: 0c74 0d6a 0e7c 0a7c 0c64 0b7c 0164 0c8d  .t.j.|.|.d.|.d..
+00000620: 047d 0a7c 0a64 0a19 007c 0a7c 013c 007c  .}.|.d...|.|.<.|
+00000630: 0a53 0029 0d61 b205 0000 5072 6570 726f  .S.).a....Prepro
+00000640: 6365 7373 2075 7365 7220 7072 6f76 6964  cess user provid
+00000650: 6564 2070 6f6c 7967 6f6e 730a 0a20 2020  ed polygons..   
+00000660: 2046 756e 6374 696f 6e20 7468 6174 2077   Function that w
+00000670: 696c 6c20 7265 7072 6f6a 6563 7420 636c  ill reproject cl
+00000680: 6970 2069 6e70 7574 2070 6f6c 7967 6f6e  ip input polygon
+00000690: 2077 6974 6820 7375 6262 6173 696e 2070   with subbasin p
+000006a0: 6f6c 7967 6f6e 0a20 2020 2061 6e64 2077  olygon.    and w
+000006b0: 696c 6c20 6469 7373 6f6c 7665 2074 6865  ill dissolve the
+000006c0: 2069 6e70 7574 2070 6f6c 7967 6f6e 2062   input polygon b
+000006d0: 6173 6564 206f 6e20 7468 6569 7220 4944  ased on their ID
+000006e0: 2c20 7375 6368 2061 7320 6c61 6e64 7573  , such as landus
+000006f0: 6520 6964 0a20 2020 206f 7220 736f 696c  e id.    or soil
+00000700: 2069 642e 0a0a 2020 2020 5061 7261 6d65   id...    Parame
+00000710: 7465 7273 0a20 2020 202d 2d2d 2d2d 2d2d  ters.    -------
+00000720: 2d2d 2d0a 2020 2020 7072 6f63 6573 7369  ---.    processi
+00000730: 6e67 2020 2020 2020 2020 2020 2020 2020  ng              
+00000740: 2020 2020 2020 2020 2020 3a20 7167 6973            : qgis
+00000750: 206f 626a 6563 740a 2020 2020 636f 6e74   object.    cont
+00000760: 6578 7420 2020 2020 2020 2020 2020 2020  ext             
+00000770: 2020 2020 2020 2020 2020 2020 2020 3a20                : 
+00000780: 7167 6973 206f 626a 6563 740a 2020 2020  qgis object.    
+00000790: 6c61 7965 725f 7061 7468 2020 2020 2020  layer_path      
+000007a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000007b0: 2020 3a20 7374 7269 6e67 0a20 2020 2020    : string.     
+000007c0: 2020 2054 6865 2070 6174 6820 746f 2061     The path to a
+000007d0: 2073 7065 6369 6669 6320 706f 6c79 676f   specific polygo
+000007e0: 6e2c 2066 6f72 2065 7861 6d70 6c65 2070  n, for example p
+000007f0: 6174 6820 746f 206c 616e 6475 7365 206c  ath to landuse l
+00000800: 6179 6572 0a20 2020 2050 726f 6a65 6374  ayer.    Project
+00000810: 5f63 7273 2020 2020 2020 2020 2020 2020  _crs            
+00000820: 2020 2020 2020 2020 2020 203a 2073 7472             : str
+00000830: 696e 670a 2020 2020 2020 2020 7468 6520  ing.        the 
+00000840: 4550 5347 2063 6f64 6520 6f66 2061 2070  EPSG code of a p
+00000850: 726f 6a65 6374 6564 2063 6f6f 6469 6e61  rojected coodina
+00000860: 7465 2073 7973 7465 6d20 7468 6174 2077  te system that w
+00000870: 696c 6c20 6265 2075 7365 6420 746f 0a20  ill be used to. 
+00000880: 2020 2020 2020 2063 616c 6375 6174 6520         calcuate 
+00000890: 4852 5520 6172 6561 2061 6e64 2073 6c6f  HRU area and slo
+000008a0: 7065 2e0a 2020 2020 7472 675f 6372 7320  pe..    trg_crs 
+000008b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000008c0: 2020 2020 2020 2020 2020 3a20 7374 7269            : stri
+000008d0: 6e67 0a20 2020 2020 2020 2074 6865 2045  ng.        the E
+000008e0: 5053 4720 636f 6465 206f 6620 6120 2063  PSG code of a  c
+000008f0: 6f6f 6469 6e61 7465 2073 7973 7465 6d20  oodinate system 
+00000900: 7468 6174 2077 696c 6c20 6265 2075 7365  that will be use
+00000910: 6420 746f 0a20 2020 2020 2020 2063 616c  d to.        cal
+00000920: 6375 6174 6520 7265 7072 6f6a 6563 7420  cuate reproject 
+00000930: 696e 7075 7420 706f 6c79 676f 6e0a 2020  input polygon.  
+00000940: 2020 436c 6173 735f 436f 6c20 2020 2020    Class_Col     
+00000950: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00000960: 2020 2020 3a20 7374 7269 6e67 0a20 2020      : string.   
+00000970: 2020 2020 2074 6865 2063 6f6c 756d 6e20       the column 
+00000980: 6e61 6d65 2069 6e20 7468 6520 696e 7075  name in the inpu
+00000990: 7420 706f 6c79 676f 6e20 286c 6179 6572  t polygon (layer
+000009a0: 5f70 6174 6829 2074 6861 7420 636f 6e74  _path) that cont
+000009b0: 6169 6e73 0a20 2020 2020 2020 2074 6865  ains.        the
+000009c0: 6972 2049 442c 2066 6f72 2065 7861 6d70  ir ID, for examp
+000009d0: 6c65 206c 616e 6420 7573 6520 4944 206f  le land use ID o
+000009e0: 7220 736f 696c 2049 442e 0a20 2020 204c  r soil ID..    L
+000009f0: 6179 6572 5f63 6c69 7020 2020 2020 2020  ayer_clip       
+00000a00: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00000a10: 203a 2071 6769 7320 6f62 6a65 6374 0a20   : qgis object. 
+00000a20: 2020 2020 2020 2041 2073 6870 6669 6c65         A shpfile
+00000a30: 2077 6974 6820 6578 7465 6e74 206f 6620   with extent of 
+00000a40: 7468 6520 7761 7465 7273 6865 642c 2077  the watershed, w
+00000a50: 696c 6c20 6265 2075 7365 6420 746f 2063  ill be used to c
+00000a60: 6c69 7020 696e 7075 740a 2020 2020 2020  lip input.      
+00000a70: 2020 696e 7075 7420 706f 6c79 676f 6e0a    input polygon.
+00000a80: 2020 2020 4e6f 7465 730a 2020 2020 2d2d      Notes.    --
+00000a90: 2d2d 2d2d 2d0a 2020 2020 2020 2020 2320  -----.        # 
+00000aa0: 544f 444f 3a20 4d61 7920 6265 2061 6464  TODO: May be add
+00000ab0: 2073 6f6d 6520 6675 6e63 7469 6f6e 2074   some function t
+00000ac0: 6f20 7369 6d70 6c69 6679 2074 6865 2069  o simplify the i
+00000ad0: 6e70 7574 2070 6f6c 7967 6f6e 730a 2020  nput polygons.  
+00000ae0: 2020 2020 2020 2020 2020 2020 2020 666f                fo
+00000af0: 7220 6578 616d 706c 652c 2072 656d 6f76  r example, remov
+00000b00: 6520 7468 6520 6c61 6e64 7573 6520 7479  e the landuse ty
+00000b10: 7065 2077 6974 6820 736d 616c 6c20 6172  pe with small ar
+00000b20: 6561 730a 2020 2020 2020 2020 2020 2020  eas.            
+00000b30: 2020 2020 6f72 206d 6572 6765 2073 6d61      or merge sma
+00000b40: 6c6c 206c 616e 6475 7365 2070 6f6c 7967  ll landuse polyg
+00000b50: 6f6e 2069 6e74 6f20 7468 6520 7375 7272  on into the surr
+00000b60: 6f75 6e64 696e 6720 706f 6c79 676f 6e0a  ounding polygon.
+00000b70: 0a20 2020 2052 6574 7572 6e73 3a0a 2020  .    Returns:.  
+00000b80: 2020 2d2d 2d2d 2d2d 2d0a 2020 2020 2020    -------.      
+00000b90: 2020 6c61 7965 725f 6469 7320 2020 2020    layer_dis     
+00000ba0: 2020 2020 2020 2020 2020 2020 203a 2071               : q
+00000bb0: 6769 7320 6f62 6a65 6374 0a20 2020 2020  gis object.     
+00000bc0: 2020 2020 2020 2069 7420 6973 2061 2070         it is a p
+00000bd0: 6f6c 7967 6f6e 2061 6674 6572 2070 7265  olygon after pre
+00000be0: 7072 6f63 6573 730a 2020 2020 5429 01da  process.    T)..
+00000bf0: 0c69 676e 6f72 655f 696e 6465 7872 1e00  .ignore_indexr..
+00000c00: 0000 7226 0000 007a 3120 6e6f 7420 696e  ..r&...z1 not in
+00000c10: 2074 6865 2061 7474 7269 6275 7465 2074   the attribute t
+00000c20: 6162 6c65 206f 6620 7072 6f76 6964 6564  able of provided
+00000c30: 2073 6861 7065 6669 6c65 7a32 206e 6f74   shapefilez2 not
+00000c40: 2069 6e20 7468 6520 6174 7472 6962 7574   in the attribut
+00000c50: 6520 7461 626c 6520 6f66 2070 726f 7669  e table of provi
+00000c60: 6465 6420 696e 666f 2074 6162 6c65 721a  ded info tabler.
+00000c70: 0000 00da 046c 6173 7429 03da 0673 7562  .....last)...sub
+00000c80: 7365 74da 046b 6565 7072 2700 0000 5a06  set..keepr'...Z.
+00000c90: 4e65 775f 4944 da05 696e 6e65 7229 02da  New_ID..inner)..
+00000ca0: 0368 6f77 da02 6f6e 290f da03 6372 73da  .how..on)...crs.
+00000cb0: 0967 656f 7061 6e64 6173 da09 7265 6164  .geopandas..read
+00000cc0: 5f66 696c 65da 0674 6f5f 6372 73da 0765  _file..to_crs..e
+00000cd0: 7870 6c6f 6465 da04 636c 6970 da15 636c  xplode..clip..cl
+00000ce0: 6561 6e5f 6765 6f6d 6574 7279 5f70 7572  ean_geometry_pur
+00000cf0: 6570 79da 0763 6f6c 756d 6e73 da05 7072  epy..columns..pr
+00000d00: 696e 74da 0373 7973 da04 6578 6974 721f  int..sys..exitr.
+00000d10: 0000 00da 0f64 726f 705f 6475 706c 6963  .....drop_duplic
+00000d20: 6174 6573 7213 0000 00da 056d 6572 6765  atesr......merge
+00000d30: 290d 5a0a 6c61 7965 725f 7061 7468 5a09  ).Z.layer_pathZ.
+00000d40: 436c 6173 735f 436f 6cda 0a74 656d 7066  Class_Col..tempf
+00000d50: 6f6c 6465 72da 0a6d 6173 6b5f 6c61 7965  older..mask_laye
+00000d60: 725a 0c43 6c61 7373 5f4e 4d5f 436f 6c5a  rZ.Class_NM_ColZ
+00000d70: 0a69 6e66 6f5f 7461 626c 655a 076e 6577  .info_tableZ.new
+00000d80: 5f63 7273 da04 6461 7461 5a09 7072 6f6a  _crs..dataZ.proj
+00000d90: 6563 7465 64da 0763 6c69 7070 6564 da07  ected..clipped..
+00000da0: 636c 6561 6e65 645a 0f69 6e66 6f5f 7461  cleanedZ.info_ta
+00000db0: 626c 655f 636f 7079 5a10 696e 666f 5f74  ble_copyZ.info_t
+00000dc0: 6162 6c65 5f63 6f70 7932 720a 0000 0072  able_copy2r....r
+00000dd0: 0a00 0000 720e 0000 00da 2c52 6570 726f  ....r.....,Repro
+00000de0: 6a5f 436c 6970 5f44 6973 736f 6c76 655f  j_Clip_Dissolve_
+00000df0: 5369 6d70 6c69 6679 5f50 6f6c 7967 6f6e  Simplify_Polygon
+00000e00: 5f70 7572 6570 7934 0000 0073 3000 0000  _purepy4...s0...
+00000e10: 0027 0601 0a02 0a01 0c01 0a03 0a01 0a01  .'..............
+00000e20: 0a01 0a01 0801 0a01 0a01 0801 0a01 0a01  ................
+00000e30: 0802 0c01 1201 0c01 0c01 1a02 1201 0c06  ................
+00000e40: 7240 0000 00da 0553 7562 4964 6307 0000  r@.....SubIdc...
+00000e50: 0000 0000 0000 0000 0014 0000 0006 0000  ................
+00000e60: 0043 0000 0073 7804 0000 6700 6401 a201  .C...sx...g.d...
+00000e70: 7d07 6402 7d08 6403 7c00 6a00 7600 721a  }.d.}.d.|.j.v.r.
+00000e80: 6403 7d08 6404 7c00 6a00 7600 722a 6405  d.}.d.|.j.v.r*d.
+00000e90: 7d09 6e04 6406 7d09 7c04 6407 6b03 9003  }.n.d.}.|.d.k...
+00000ea0: 7216 7c05 6407 6b03 7256 7401 a002 7c05  r.|.d.k.rVt...|.
+00000eb0: a101 7d0a 7c0a 6408 1900 7c0a 6409 3c00  ..}.|.d...|.d.<.
+00000ec0: 7c00 6a03 640a 640b 8d01 6a04 640c 640d  |.j.d.d...j.d.d.
+00000ed0: 8d01 7d0b 7c05 6407 6b03 72a0 7c0a 640a  ..}.|.d.k.r.|.d.
+00000ee0: 6409 6702 1900 7d0a 7405 6a06 7c0a 7c0b  d.g...}.t.j.|.|.
+00000ef0: 6409 640e 640f 8d04 7d0a 7c0a 6a07 7c06  d.d.d...}.|.j.|.
+00000f00: 6410 6411 6412 8d03 7d0a 7c00 6a07 7c06  d.d.d...}.|.j.|.
+00000f10: 6410 6411 6412 8d03 7d00 7408 7c00 6413  d.d.d...}.t.|.d.
+00000f20: 6414 8303 7d00 7c00 6414 6413 6702 1900  d...}.|.d.d.g...
+00000f30: 6a04 640c 640d 8d01 7d0c 7c05 6407 6b03  j.d.d...}.|.d.k.
+00000f40: 72fc 7c0a 6a03 6414 6413 6702 640b 8d01  r.|.j.d.d.g.d...
+00000f50: 7d0a 7c0a a009 7c0c a101 7d0a 7c0a 7c00  }.|...|...}.|.|.
+00000f60: 6a00 1900 7d0a 6415 6701 7d0d 6416 7c04  j...}.d.g.}.d.|.
+00000f70: 7601 9001 7240 7c00 6408 6417 6702 1900  v...r@|.d.d.g...
+00000f80: 6a04 640c 640d 8d01 7d0e 7c0e 7c0e 6408  j.d.d...}.|.|.d.
+00000f90: 1900 a00a 7c00 6417 1900 6a0b a101 0f00  ....|.d...j.....
+00000fa0: 1900 6408 1900 6a0b 7d0d 7c05 6407 6b03  ..d...j.}.|.d.k.
+00000fb0: 9001 729e 7c0a 7c0a 6a0c a00a 7c0d a101  ..r.|.|.j...|...
+00000fc0: 0f00 1900 7d0a 7c0a 6a00 7d0f 7c0f 7c0f  ....}.|.j.}.|.|.
+00000fd0: a00a 7c07 a101 1900 7d10 7c0a 6a03 7c10  ..|.....}.|.j.|.
+00000fe0: 640b 8d01 7d0a 740d 7c0a 8301 6418 6b04  d...}.t.|...d.k.
+00000ff0: 9001 729e 7c0a a00e 740f 6a10 a009 7c02  ..r.|...t.j...|.
+00001000: 7c04 a102 a101 0100 6419 7c03 7600 9002  |.......d.|.v...
+00001010: 72b0 641a 7c00 6a11 7c00 6a0c a00a 7c0d  r.d.|.j.|.j...|.
+00001020: a101 641b 6602 3c00 641a 7c00 6a11 7c00  ..d.f.<.d.|.j.|.
+00001030: 6a0c a00a 7c0d a101 641c 6602 3c00 641a  j...|...d.f.<.d.
+00001040: 7c00 6a11 7c00 6a0c a00a 7c0d a101 641d  |.j.|.j...|...d.
+00001050: 6602 3c00 641a 7c00 6a11 7c00 6a0c a00a  f.<.d.|.j.|.j...
+00001060: 7c0d a101 641e 6602 3c00 641a 7c00 6a11  |...d.f.<.d.|.j.
+00001070: 7c00 6a0c a00a 7c0d a101 641f 6602 3c00  |.j...|...d.f.<.
+00001080: 641a 7c00 6a11 7c00 6a0c a00a 7c0d a101  d.|.j.|.j...|...
+00001090: 6420 6602 3c00 641a 7c00 6a11 7c00 6421  d f.<.d.|.j.|.d!
+000010a0: 1900 6418 6b04 641b 6602 3c00 641a 7c00  ..d.k.d.f.<.d.|.
+000010b0: 6a11 7c00 6421 1900 6418 6b04 641c 6602  j.|.d!..d.k.d.f.
+000010c0: 3c00 641a 7c00 6a11 7c00 6421 1900 6418  <.d.|.j.|.d!..d.
+000010d0: 6b04 641d 6602 3c00 641a 7c00 6a11 7c00  k.d.f.<.d.|.j.|.
+000010e0: 6421 1900 6418 6b04 641e 6602 3c00 641a  d!..d.k.d.f.<.d.
+000010f0: 7c00 6a11 7c00 6421 1900 6418 6b04 641f  |.j.|.d!..d.k.d.
+00001100: 6602 3c00 641a 7c00 6a11 7c00 6421 1900  f.<.d.|.j.|.d!..
+00001110: 6418 6b04 6420 6602 3c00 7c00 6a00 7d0f  d.k.d f.<.|.j.}.
+00001120: 7c0f 7c0f a00a 7c07 a101 1900 7d10 7c00  |.|...|.....}.|.
+00001130: 6a03 7c10 640b 8d01 7d00 7c00 a00e 740f  j.|.d...}.|...t.
+00001140: 6a10 a009 7c02 7c03 a102 a101 0100 7412  j...|.|.......t.
+00001150: 7c00 8301 7d11 7c11 a00e 740f 6a10 a009  |...}.|...t.j...
+00001160: 7c02 6422 a102 a101 0100 7413 740f 6a10  |.d"......t.t.j.
+00001170: a009 7c02 7c03 a102 8301 0100 9001 6e5e  ..|.|.........n^
+00001180: 7c00 6a07 7c06 6410 6411 6412 8d03 7d00  |.j.|.d.d.d...}.
+00001190: 6414 7c00 6a00 7600 9004 721c 7408 7c00  d.|.j.v...r.t.|.
+000011a0: 6413 6414 8303 7d00 7c00 6a14 7c00 6408  d.d...}.|.j.|.d.
+000011b0: 3c00 7c00 7c00 6421 1900 6423 6b03 1900  <.|.|.d!..d#k...
+000011c0: 6408 6417 6702 1900 6a04 640c 640d 8d01  d.d.g...j.d.d...
+000011d0: 7d0e 6700 7d12 7c0e 6408 1900 6a0b 4400  }.g.}.|.d...j.D.
+000011e0: 5d20 7d13 7c13 7c0e 6417 1900 6a0b 7601  ] }.|.|.d...j.v.
+000011f0: 9003 7276 7c12 a015 7c13 a101 0100 9003  ..rv|...|.......
+00001200: 7176 641a 7c00 6a11 7c00 6a0c a00a 7c12  qvd.|.j.|.j...|.
+00001210: a101 641b 6602 3c00 641a 7c00 6a11 7c00  ..d.f.<.d.|.j.|.
+00001220: 6a0c a00a 7c12 a101 641c 6602 3c00 641a  j...|...d.f.<.d.
+00001230: 7c00 6a11 7c00 6a0c a00a 7c12 a101 641d  |.j.|.j...|...d.
+00001240: 6602 3c00 641a 7c00 6a11 7c00 6a0c a00a  f.<.d.|.j.|.j...
+00001250: 7c12 a101 641e 6602 3c00 641a 7c00 6a11  |...d.f.<.d.|.j.
+00001260: 7c00 6a0c a00a 7c12 a101 641f 6602 3c00  |.j...|...d.f.<.
+00001270: 641a 7c00 6a11 7c00 6a0c a00a 7c12 a101  d.|.j.|.j...|...
+00001280: 6420 6602 3c00 7c00 6a00 7d0f 7c0f 7c0f  d f.<.|.j.}.|.|.
+00001290: a00a 6700 6424 a201 a101 1900 7d10 7c00  ..g.d$......}.|.
+000012a0: 6a03 7c10 640b 8d01 7d00 7c00 a00e 740f  j.|.d...}.|...t.
+000012b0: 6a10 a009 7c02 7c03 a102 a101 0100 7412  j...|.|.......t.
+000012c0: 7c00 8301 7d11 7c11 a00e 740f 6a10 a009  |...}.|...t.j...
+000012d0: 7c02 6422 a102 a101 0100 7c00 5300 6400  |.d"......|.S.d.
+000012e0: 5300 2925 4e29 10da 0753 7562 4964 5f31  S.)%N)...SubId_1
+000012f0: da02 4964 da07 6e73 7562 6964 32da 066e  ..Id..nsubid2..n
+00001300: 7375 6269 64da 0a6e 646f 776e 7375 6269  subid..ndownsubi
+00001310: 64da 094f 6c64 5f53 7562 4964 da0a 4f6c  d..Old_SubId..Ol
+00001320: 645f 446f 7753 7562 da0a 4a6f 696e 5f43  d_DowSub..Join_C
+00001330: 6f75 6e74 da0a 5441 5247 4554 5f46 4944  ount..TARGET_FID
+00001340: 7243 0000 00da 0a53 7562 4944 5f4f 6c64  rC.....SubID_Old
+00001350: 72da 0a48 5255 5f49 445f 4e5f 31da 0a48  r..HRU_ID_N_1..H
+00001360: 5255 5f49 445f 4e5f 32da 0766 6163 7465  RU_ID_N_2..facte
+00001370: 7273 da0c 4f6c 645f 446f 7753 7562 4964  rs..Old_DowSubId
+00001380: 5a07 5375 6249 6474 32da 0844 415f 6572  Z.SubIdt2..DA_er
+00001390: 726f 725a 0744 415f 4469 6666 da08 4441  rorZ.DA_Diff..DA
+000013a0: 5f43 686e 5f4c 7a41 6874 7470 733a 2f2f  _Chn_LzAhttps://
+000013b0: 6769 7468 7562 2e63 6f6d 2f64 7573 746d  github.com/dustm
+000013c0: 696e 672f 526f 7574 696e 6754 6f6f 6c2f  ing/RoutingTool/
+000013d0: 7769 6b69 2f46 696c 6573 2f52 4541 444d  wiki/Files/READM
+000013e0: 455f 4f49 482e 7064 667a 4068 7474 7073  E_OIH.pdfz@https
+000013f0: 3a2f 2f67 6974 6875 622e 636f 6d2f 6475  ://github.com/du
+00001400: 7374 6d69 6e67 2f52 6f75 7469 6e67 546f  stming/RoutingTo
+00001410: 6f6c 2f77 696b 692f 4669 6c65 732f 5245  ol/wiki/Files/RE
+00001420: 4144 4d45 5f4e 412e 7064 6672 2600 0000  ADME_NA.pdfr&...
+00001430: 7241 0000 0072 4700 0000 da08 6765 6f6d  rA...rG.....geom
+00001440: 6574 7279 a901 7235 0000 0054 721a 0000  etry..r5...Tr...
+00001450: 00da 046c 6566 7429 0272 2d00 0000 722c  ...left).r-...r,
+00001460: 0000 00da 0566 6972 7374 46a9 03da 0262  .....firstF....b
+00001470: 79da 0761 6767 6675 6e63 da08 6173 5f69  y..aggfunc..as_i
+00001480: 6e64 6578 da0a 6365 6e74 726f 6964 5f78  ndex..centroid_x
+00001490: da0a 6365 6e74 726f 6964 5f79 69f1 d8ff  ..centroid_yi...
+000014a0: ffda 1b72 6976 6572 5f77 6974 686f 7574  ...river_without
+000014b0: 5f6d 6572 6769 6e67 5f6c 616b 6573 da08  _merging_lakes..
+000014c0: 446f 7753 7562 4964 7201 0000 00da 0d66  DowSubIdr......f
+000014d0: 696e 616c 6361 745f 696e 666f 678d 976e  inalcat_infog..n
+000014e0: 1283 c0f3 bfda 0852 6976 536c 6f70 65da  .......RivSlope.
+000014f0: 0952 6976 4c65 6e67 7468 da08 466c 6f6f  .RivLength..Floo
+00001500: 6450 5f6e da04 4368 5f6e da07 4d61 785f  dP_n..Ch_n..Max_
+00001510: 4445 4dda 074d 696e 5f44 454d da08 4c61  DEM..Min_DEM..La
+00001520: 6b65 5f43 6174 7a0b 6f75 746c 696e 652e  ke_Catz.outline.
+00001530: 7368 70e9 0200 0000 290f da05 5348 4150  shp.....)...SHAP
+00001540: 4572 4200 0000 7243 0000 0072 4400 0000  ErB...rC...rD...
+00001550: 7245 0000 0072 4600 0000 7248 0000 0072  rE...rF...rH...r
+00001560: 4900 0000 724a 0000 0072 4300 0000 724b  I...rJ...rC...rK
+00001570: 0000 0072 4c00 0000 724d 0000 0072 4e00  ...rL...rM...rN.
+00001580: 0000 724f 0000 0029 1672 3500 0000 722f  ..rO...).r5...r/
+00001590: 0000 0072 3000 0000 da04 6472 6f70 721f  ...r0.....dropr.
+000015a0: 0000 0072 1300 0000 723a 0000 00da 0864  ...r....r:.....d
+000015b0: 6973 736f 6c76 65da 1561 6464 5f63 656e  issolve..add_cen
+000015c0: 7472 6f69 645f 696e 5f77 6773 3834 da04  troid_in_wgs84..
+000015d0: 6a6f 696e 7221 0000 00da 0676 616c 7565  joinr!.....value
+000015e0: 7372 4100 0000 7220 0000 00da 0774 6f5f  srA...r .....to_
+000015f0: 6669 6c65 da02 6f73 da04 7061 7468 da03  file..os..path..
+00001600: 6c6f 63da 1963 7265 6174 655f 7761 7465  loc..create_wate
+00001610: 7273 6865 645f 626f 756e 6461 7279 da15  rshed_boundary..
+00001620: 6372 6561 7465 5f67 656f 5f6a 6173 6f6e  create_geo_jason
+00001630: 5f66 696c 65da 0569 6e64 6578 7222 0000  _file..indexr"..
+00001640: 0029 14da 0e6d 6170 6f6c 646e 6577 5f69  .)...mapoldnew_i
+00001650: 6e66 6f72 3b00 0000 da0c 4f75 7470 7574  nfor;.....Output
+00001660: 466f 6c64 6572 da08 6361 745f 6e61 6d65  Folder..cat_name
+00001670: da08 7269 765f 6e61 6d65 da0e 5061 7468  ..riv_name..Path
+00001680: 5f66 696e 616c 5f72 6976 5a0c 6469 735f  _final_rivZ.dis_
+00001690: 636f 6c5f 6e61 6d65 5a12 4e45 4544 5f54  col_nameZ.NEED_T
+000016a0: 4f5f 5245 4d4f 5645 5f49 4453 5a0e 6f62  O_REMOVE_IDSZ.ob
+000016b0: 735f 6572 726f 725f 6e61 6d65 da03 7572  s_error_name..ur
+000016c0: 6c5a 0672 6976 5f70 645a 0663 6174 5f70  lZ.riv_pdZ.cat_p
+000016d0: 645a 0963 6174 5f63 5f78 5f79 5a0d 7265  dZ.cat_c_x_yZ.re
+000016e0: 6d6f 7665 5f73 7562 6964 73da 1972 6976  move_subids..riv
+000016f0: 5f70 645f 6e6e 636c 735f 726f 7574 696e  _pd_nncls_routin
+00001700: 675f 696e 666f 5a0a 6361 745f 636f 6c6e  g_infoZ.cat_coln
+00001710: 6d73 5a0f 6472 6f70 5f63 6174 5f63 6f6c  msZ.drop_cat_col
+00001720: 6e6d 73da 076f 7574 6c69 6e65 5a0e 7265  nms..outlineZ.re
+00001730: 6d6f 7665 5f63 6861 6e6e 656c da05 7375  move_channel..su
+00001740: 6269 6472 0a00 0000 720a 0000 0072 0e00  bidr....r....r..
+00001750: 0000 da23 7361 7665 5f6d 6f64 6966 6965  ...#save_modifie
+00001760: 645f 6174 7472 6962 7574 6573 5f74 6f5f  d_attributes_to_
+00001770: 6f75 7470 7574 737f 0000 0073 9800 0000  outputs....s....
+00001780: 0003 0801 0401 0a01 0403 0a01 0602 0406  ................
+00001790: 0a02 0801 0a01 0c02 1402 0801 0c01 1201  ................
+000017a0: 1003 1001 0c02 1401 0801 1001 0a01 0a01  ................
+000017b0: 0602 0a01 1401 2001 0a01 1201 0601 0e01  ...... .........
+000017c0: 0c01 0e01 1402 0a01 1601 1601 1601 1601  ................
+000017d0: 1601 1601 1601 1601 1601 1601 1601 1602  ................
+000017e0: 0601 0e01 0c01 1402 0801 1401 1604 1002  ................
+000017f0: 0c02 0c01 0a01 2001 0401 0e01 1001 0e02  ...... .........
+00001800: 1601 1601 1601 1601 1601 1602 0601 1201  ................
+00001810: 0c01 1401 0801 1401 727d 0000 0063 0100  ........r}...c..
+00001820: 0000 0000 0000 0000 0000 0200 0000 0500  ................
+00001830: 0000 4300 0000 732e 0000 007c 006a 0064  ..C...s....|.j.d
+00001840: 0164 028d 0164 0367 0119 007d 0164 047c  .d...d.g...}.d.|
+00001850: 0164 053c 007c 016a 0164 0564 0664 0764  .d.<.|.j.d.d.d.d
+00001860: 088d 037d 017c 0153 0029 094e 5472 1a00  ...}.|.S.).NTr..
+00001870: 0000 7252 0000 0072 1e00 0000 da02 4944  ..rR...r......ID
+00001880: 7255 0000 0046 7256 0000 0029 0272 1f00  rU...FrV...).r..
+00001890: 0000 7269 0000 0029 0272 7400 0000 da02  ..ri...).rt.....
+000018a0: 7762 720a 0000 0072 0a00 0000 720e 0000  wbr....r....r...
+000018b0: 0072 7100 0000 e800 0000 7308 0000 0000  .rq.......s.....
+000018c0: 0112 0108 0110 0172 7100 0000 6302 0000  .......rq...c...
+000018d0: 0000 0000 0000 0000 0005 0000 0005 0000  ................
+000018e0: 0043 0000 0073 8400 0000 7400 a001 7c00  .C...s....t...|.
+000018f0: 6401 1900 a002 7c01 a101 a101 7d02 7c00  d.....|.....}.|.
+00001900: 6402 1900 6403 6b03 7d03 7400 a003 7c02  d...d.k.}.t...|.
+00001910: 7c03 a102 7d04 6404 7c00 6a04 7c04 6401  |...}.d.|.j.|.d.
+00001920: 6602 3c00 6404 7c00 6a04 7c04 6405 6602  f.<.d.|.j.|.d.f.
+00001930: 3c00 6404 7c00 6a04 7c04 6406 6602 3c00  <.d.|.j.|.d.f.<.
+00001940: 6404 7c00 6a04 7c04 6407 6602 3c00 6404  d.|.j.|.d.f.<.d.
+00001950: 7c00 6a04 7c04 6408 6602 3c00 6404 7c00  |.j.|.d.f.<.d.|.
+00001960: 6a04 7c04 6402 6602 3c00 7c00 5300 2909  j.|.d.f.<.|.S.).
+00001970: 7af1 4675 6e63 7469 6f6e 7320 7769 6c6c  z.Functions will
+00001980: 2073 6574 206c 616b 6520 6964 206e 6f74   set lake id not
+00001990: 2069 6e20 436f 6e6e 5f4c 616b 655f 4964   in Conn_Lake_Id
+000019a0: 7320 746f 202d 312e 3233 3435 2069 6e20  s to -1.2345 in 
+000019b0: 6174 7472 6962 7574 650a 2020 2020 2020  attribute.      
+000019c0: 2020 7461 626c 6520 6f66 2050 6174 685f    table of Path_
+000019d0: 4669 6e61 6c63 6174 696e 666f 0a20 2020  Finalcatinfo.   
+000019e0: 202d 2d2d 2d2d 2d2d 2d2d 2d0a 0a20 2020   ----------..   
+000019f0: 204e 6f74 6573 0a20 2020 202d 2d2d 2d2d   Notes.    -----
+00001a00: 2d2d 0a0a 2020 2020 5265 7475 726e 733a  --..    Returns:
+00001a10: 0a20 2020 202d 2d2d 2d2d 2d2d 0a20 2020  .    -------.   
+00001a20: 2020 2020 204e 6f6e 652c 2074 6865 2061       None, the a
+00001a30: 7474 7269 6275 7465 2074 6162 6c65 206f  ttribute table o
+00001a40: 6620 5061 7468 5f73 6870 6669 6c65 2077  f Path_shpfile w
+00001a50: 696c 6c20 6265 2075 7064 6174 6564 0a20  ill be updated. 
+00001a60: 2020 20da 0848 794c 616b 6549 6472 6500     ..HyLakeIdre.
+00001a70: 0000 7266 0000 0072 0100 0000 da07 4c61  ..rf...r......La
+00001a80: 6b65 566f 6cda 084c 616b 6541 7265 61da  keVol..LakeArea.
+00001a90: 094c 616b 6544 6570 7468 da08 4c61 6b65  .LakeDepth..Lake
+00001aa0: 7479 7065 2905 da02 6e70 da0b 6c6f 6769  type)...np..logi
+00001ab0: 6361 6c5f 6e6f 7472 2100 0000 da0b 6c6f  cal_notr!.....lo
+00001ac0: 6769 6361 6c5f 616e 6472 7000 0000 2905  gical_andrp...).
+00001ad0: 5a0c 6669 6e61 6c63 6174 5f70 6c79 da0d  Z.finalcat_ply..
+00001ae0: 436f 6e6e 5f4c 616b 655f 4964 73da 056d  Conn_Lake_Ids..m
+00001af0: 6173 6b31 da05 6d61 736b 32da 046d 6173  ask1..mask2..mas
+00001b00: 6b72 0a00 0000 720a 0000 0072 0e00 0000  kr....r....r....
+00001b10: da37 5265 6d6f 7665 5f55 6e73 656c 6563  .7Remove_Unselec
+00001b20: 7465 645f 4c61 6b65 5f41 7474 7269 6275  ted_Lake_Attribu
+00001b30: 7465 5f49 6e5f 4669 6e61 6c63 6174 696e  te_In_Finalcatin
+00001b40: 666f 5f70 7572 6570 79ee 0000 0073 1400  fo_purepy....s..
+00001b50: 0000 000d 1401 0c01 0c02 0e01 0e01 0e01  ................
+00001b60: 0e01 0e01 0e02 728c 0000 0063 0200 0000  ......r....c....
+00001b70: 0000 0000 0000 0000 0300 0000 0700 0000  ................
+00001b80: 4300 0000 732a 0000 007c 006a 0074 01a0  C...s*...|.j.t..
+00001b90: 0274 01a0 037c 006a 007c 01a1 02a1 0119  .t...|.j.|......
+00001ba0: 007d 027c 006a 047c 0264 018d 017d 007c  .}.|.j.|.d...}.|
+00001bb0: 0053 0029 024e 7253 0000 0029 0572 3500  .S.).NrS...).r5.
+00001bc0: 0000 7285 0000 0072 8600 0000 7221 0000  ..r....r....r!..
+00001bd0: 0072 6800 0000 2903 da05 7461 626c 65da  .rh...)...table.
+00001be0: 056e 616d 6573 5a13 7265 6d6f 7665 5f63  .namesZ.remove_c
+00001bf0: 6f6c 756d 6e5f 6e61 6d65 7372 0a00 0000  olumn_namesr....
+00001c00: 720a 0000 0072 0e00 0000 da1b 636c 6561  r....r......clea
+00001c10: 6e5f 6174 7472 6962 7574 655f 6e61 6d65  n_attribute_name
+00001c20: 5f70 7572 6570 7908 0100 0073 0600 0000  _purepy....s....
+00001c30: 0001 1a01 0c01 728f 0000 00e9 ffff ffff  ......r.........
+00001c40: 6302 0000 0000 0000 0000 0000 0007 0000  c...............
+00001c50: 0004 0000 0043 0000 0073 ca00 0000 7c01  .....C...s....|.
+00001c60: 6401 6b04 721a 7c00 6402 1900 a000 6403  d.k.r.|.d.....d.
+00001c70: a101 7c00 6402 3c00 7c00 6402 1900 a001  ..|.d.<.|.d.....
+00001c80: a100 0f00 7d02 7c00 6a02 0f00 7d03 7c00  ....}.|.j...}.|.
+00001c90: 6a03 6401 6b04 7d04 7404 a005 7c02 7c03  j.d.k.}.t...|.|.
+00001ca0: a102 7d05 7404 a005 7c04 7c05 a102 7d06  ..}.t...|.|...}.
+00001cb0: 7c00 6a06 7c06 1900 7d00 7c00 6a06 7c00  |.j.|...}.|.j.|.
+00001cc0: 6a07 6404 6b03 1900 7d00 7408 7c00 6a06  j.d.k...}.t.|.j.
+00001cd0: 7c00 6a07 6405 6b02 1900 8301 6401 6b04  |.j.d.k.....d.k.
+00001ce0: 72b0 7409 6406 8301 0100 7409 6407 8301  r.t.d.....t.d...
+00001cf0: 0100 7409 7c00 6a06 7c00 6a07 6405 6b02  ..t.|.j.|.j.d.k.
+00001d00: 1900 8301 0100 7409 6406 8301 0100 7c00  ......t.d.....|.
+00001d10: 6a06 7c00 6a07 6405 6b03 1900 7d00 7c00  j.|.j.d.k...}.|.
+00001d20: 6a0a 0100 7c00 5300 2908 4e72 0100 0000  j...|.S.).Nr....
+00001d30: 7252 0000 0067 9564 79e1 7ffd a53d da05  rR...g.dy....=..
+00001d40: 506f 696e 74da 1247 656f 6d65 7472 7943  Point..GeometryC
+00001d50: 6f6c 6c65 6374 696f 6e7a 1b23 2323 2323  ollectionz.#####
+00001d60: 2323 2323 2323 2323 2323 2323 2323 2323  ################
+00001d70: 2323 2323 2323 7a1c 6368 6563 6b20 7468  ######z.check th
+00001d80: 6520 666f 6c6c 6f77 696e 6720 6665 6174  e following feat
+00001d90: 7572 6573 290b da06 6275 6666 6572 da04  ures)...buffer..
+00001da0: 6973 6e61 da08 6973 5f65 6d70 7479 da04  isna..is_empty..
+00001db0: 6172 6561 7285 0000 0072 8700 0000 7270  arear....r....rp
+00001dc0: 0000 005a 0967 656f 6d5f 7479 7065 7220  ...Z.geom_typer 
+00001dd0: 0000 0072 3600 0000 5a06 7369 6e64 6578  ...r6...Z.sindex
+00001de0: 2907 723d 0000 005a 0d73 6574 5f70 7265  ).r=...Z.set_pre
+00001df0: 6369 7369 6f6e 5a05 6e61 726f 775a 0565  cisionZ.narowZ.e
+00001e00: 6d72 6f77 5a07 6172 6561 726f 775a 0472  mrowZ.arearowZ.r
+00001e10: 6f77 315a 0972 6f77 7365 6c65 6374 720a  ow1Z.rowselectr.
+00001e20: 0000 0072 0a00 0000 720e 0000 0072 3400  ...r....r....r4.
+00001e30: 0000 0d01 0000 7322 0000 0000 0308 0112  ......s"........
+00001e40: 060e 0208 020a 030c 010c 030a 0210 0118  ................
+00001e50: 0108 0108 0114 0108 0210 0106 0272 3400  .............r4.
+00001e60: 0000 6303 0000 0000 0000 0000 0000 0006  ..c.............
+00001e70: 0000 0003 0000 0043 0000 0073 3800 0000  .......C...s8...
+00001e80: 7c00 6a00 7d03 7c00 a001 a100 7d04 7c00  |.j.}.|.....}.|.
+00001e90: a002 7c01 a101 7d04 7c04 6a03 7c04 7c02  ..|...}.|.j.|.|.
+00001ea0: 3c00 7c04 6a01 6401 6402 8d01 a002 7c03  <.|.j.d.d.....|.
+00001eb0: a101 7d05 7c05 5300 2903 4e54 721a 0000  ..}.|.S.).NTr...
+00001ec0: 0029 0472 2e00 0000 721f 0000 0072 3100  .).r....r....r1.
+00001ed0: 0000 7296 0000 0029 0672 3d00 0000 5a07  ..r....).r=...Z.
+00001ee0: 7072 6a5f 6372 735a 0861 7265 615f 636f  prj_crsZ.area_co
+00001ef0: 6cda 0773 7263 5f73 7263 da04 746f 7374  l..src_src..tost
+00001f00: da03 6f75 7472 0a00 0000 720a 0000 0072  ..outr....r....r
+00001f10: 0e00 0000 da0e 6164 645f 6172 6561 5f69  ......add_area_i
+00001f20: 6e5f 6d32 3001 0000 730c 0000 0000 0106  n_m20...s.......
+00001f30: 0108 020a 010a 0212 0272 9a00 0000 6303  .........r....c.
+00001f40: 0000 0000 0000 0000 0000 0006 0000 0003  ................
+00001f50: 0000 0043 0000 0073 4a00 0000 7c00 6a00  ...C...sJ...|.j.
+00001f60: 7d03 7c00 a001 a100 7d04 7c04 a002 6401  }.|.....}.|...d.
+00001f70: a101 7d04 7c04 6a03 6a04 6a05 7c04 7c02  ..}.|.j.j.j.|.|.
+00001f80: 3c00 7c04 6a03 6a04 6a06 7c04 7c01 3c00  <.|.j.j.j.|.|.<.
+00001f90: 7c04 6a01 6402 6403 8d01 a002 7c03 a101  |.j.d.d.....|...
+00001fa0: 7d05 7c05 5300 2904 4efa 0945 5053 473a  }.|.S.).N..EPSG:
+00001fb0: 3433 3236 5472 1a00 0000 2907 722e 0000  4326Tr....).r...
+00001fc0: 0072 1f00 0000 7231 0000 0072 5200 0000  .r....r1...rR...
+00001fd0: da08 6365 6e74 726f 6964 da01 7972 0b00  ..centroid..yr..
+00001fe0: 0000 2906 723d 0000 005a 0463 6f6c 785a  ..).r=...Z.colxZ
+00001ff0: 0463 6f6c 7972 9700 0000 7298 0000 0072  .colyr....r....r
+00002000: 9900 0000 720a 0000 0072 0a00 0000 720e  ....r....r....r.
+00002010: 0000 0072 6a00 0000 3b01 0000 730e 0000  ...rj...;...s...
+00002020: 0000 0106 0108 020a 020e 010e 0212 0272  ...............r
+00002030: 6a00 0000 6301 0000 0000 0000 0000 0000  j...c...........
+00002040: 001c 0000 0008 0000 0043 0000 0073 7e03  .........C...s~.
+00002050: 0000 6401 7c00 7601 720c 6400 5300 7400  ..d.|.v.r.d.S.t.
+00002060: 6a01 a002 7c00 a101 7d01 7400 6a01 a003  j...|...}.t.j...
+00002070: 7c00 a101 a004 6402 a101 7d02 7405 7c02  |.....d...}.t.|.
+00002080: 8301 7d03 7c02 7c03 6403 1800 1900 6404  ..}.|.|.d.....d.
+00002090: 6405 8502 1900 7d04 6406 6407 6702 7d05  d.....}.d.d.g.}.
+000020a0: 6401 7d06 6408 7d07 6409 7d08 640a 7d09  d.}.d.}.d.}.d.}.
+000020b0: 6700 7d0a 6700 7d0b 640b 7c04 7600 72e8  g.}.g.}.d.|.v.r.
+000020c0: 7c06 6402 1700 7c04 1700 640c 1700 7c07  |.d...|...d...|.
+000020d0: 6402 1700 7c04 1700 640c 1700 7c08 6402  d...|...d...|.d.
+000020e0: 1700 7c04 1700 640c 1700 7c09 6402 1700  ..|...d...|.d...
+000020f0: 7c04 1700 640c 1700 6704 7d0a 7c06 6402  |...d...g.}.|.d.
+00002100: 1700 7c04 1700 640d 1700 7c07 6402 1700  ..|...d...|.d...
+00002110: 7c04 1700 640d 1700 7c08 6402 1700 7c04  |...d...|.d...|.
+00002120: 1700 640d 1700 7c09 6402 1700 7c04 1700  ..d...|.d...|...
+00002130: 640d 1700 6704 7d0b 6e38 7c06 640c 1700  d...g.}.n8|.d...
+00002140: 7c07 640c 1700 7c08 640c 1700 7c09 640c  |.d...|.d...|.d.
+00002150: 1700 6704 7d0a 7c06 640d 1700 7c07 640d  ..g.}.|.d...|.d.
+00002160: 1700 7c08 640d 1700 7c09 640d 1700 6704  ..|.d...|.d...g.
+00002170: 7d0b 6700 7d0c 6700 7d0d 7406 6404 7405  }.g.}.g.}.t.d.t.
+00002180: 7c0a 8301 8302 4400 9001 5d2e 7d0e 7400  |.....D...].}.t.
+00002190: 6a01 a007 7c01 7c0a 7c0e 1900 a102 7d0f  j...|.|.|.....}.
+000021a0: 7400 6a01 a007 7c01 7c0b 7c0e 1900 a102  t.j...|.|.|.....
+000021b0: 7d10 7400 6a01 a008 7c0f a101 9001 7372  }.t.j...|.....sr
+000021c0: 9001 7136 7c0c a009 7c10 a101 0100 6408  ..q6|...|.....d.
+000021d0: 7c0a 7c0e 1900 7600 9001 7398 640e 7c0a  |.|...v...s.d.|.
+000021e0: 7c0e 1900 7600 9001 72a2 7c0d a009 7c10  |...v...r.|...|.
+000021f0: a101 0100 740a a00b 7c0f a101 7d11 7c11  ....t...|...}.|.
+00002200: a00c 640f a101 7d12 6401 7c0a 7c0e 1900  ..d...}.d.|.|...
+00002210: 7600 9001 73d2 6408 7c0a 7c0e 1900 7600  v...s.d.|.|...v.
+00002220: 9002 7214 7c12 6410 1900 a00d 740e a101  ..r.|.d.....t...
+00002230: a00d 740f a101 7c12 6411 3c00 7c12 6a10  ..t...|.d.<.|.j.
+00002240: 4400 5d22 7d13 6412 7c12 6a11 7c13 6411  D.]"}.d.|.j.|.d.
+00002250: 6602 1900 1700 7c12 6a11 7c13 6411 6602  f.....|.j.|.d.f.
+00002260: 3c00 9001 71f0 7c12 7d14 7c05 4400 5d46  <...q.|.}.|.D.]F
+00002270: 7d15 7c14 a012 7c15 a101 7c14 6413 3c00  }.|...|...|.d.<.
+00002280: 7c14 6a13 7c10 6414 6415 8d02 0100 7400  |.j.|.d.d.....t.
+00002290: a014 7c10 a101 6a15 6416 1b00 6416 1b00  ..|...j.d...d...
+000022a0: 7d16 7c16 6417 6b01 9002 721c 0100 9001  }.|.d.k...r.....
+000022b0: 7136 9002 711c 9001 7136 7405 7c0d 8301  q6..q...q6t.|...
+000022c0: 6403 6b04 9003 727a 7400 a014 7400 6a01  d.k...rzt...t.j.
+000022d0: a007 7c01 7c0b 6404 1900 a102 a101 6a15  ..|.|.d.......j.
+000022e0: 6416 1b00 6416 1b00 6418 6b00 9003 727a  d...d...d.k...rz
+000022f0: 7406 6404 7405 7c0d 8301 8302 4400 5d80  t.d.t.|.....D.].
+00002300: 7d0e 7416 7417 7c0d 7c0e 1900 8301 8301  }.t.t.|.|.......
+00002310: 7d17 6408 7c0d 7c0e 1900 7600 9003 7206  }.d.|.|...v...r.
+00002320: 6700 7d18 7c17 6419 1900 4400 5d22 7d19  g.}.|.d...D.]"}.
+00002330: 7c19 641a 1900 641b 1900 6404 6b02 9002  |.d...d...d.k...
+00002340: 72da 7c18 a009 7c19 a101 0100 9002 71da  r.|...|.......q.
+00002350: 7c18 7c17 6419 3c00 7c0e 6404 6b02 9003  |.|.d.<.|.d.k...
+00002360: 7216 7c17 7d1a 6e14 7c1a 6419 0500 1900  r.|.}.n.|.d.....
+00002370: 7c17 6419 1900 3700 0300 3c00 9002 71ac  |.d...7...<...q.
+00002380: 7417 7400 6a01 a007 7c01 641c a102 641d  t.t.j...|.d...d.
+00002390: 641e 641f 8d03 8f22 7d1b 7418 6a19 7c1a  d.d...."}.t.j.|.
+000023a0: 7c1b 6420 6405 6421 8d04 0100 5700 6400  |.d d.d!....W.d.
+000023b0: 0400 0400 8303 0100 6e12 3100 9003 7370  ........n.1...sp
+000023c0: 3000 0100 0100 0100 5900 0100 6400 5300  0.......Y...d.S.
+000023d0: 2922 4e72 5e00 0000 da01 5f72 1e00 0000  )"Nr^....._r....
+000023e0: 7201 0000 00e9 0400 0000 672d 431c ebe2  r.........g-C...
+000023f0: 361a 3f67 7b14 ae47 e17a 743f da11 6669  6.?g{..G.zt?..fi
+00002400: 6e61 6c63 6174 5f69 6e66 6f5f 7269 76da  nalcat_info_riv.
+00002410: 1173 6c5f 636f 6e6e 6563 7465 645f 6c61  .sl_connected_la
+00002420: 6b65 da15 736c 5f6e 6f6e 5f63 6f6e 6e65  ke..sl_non_conne
+00002430: 6374 6564 5f6c 616b 65da 0176 7a04 2e73  cted_lake..vz..s
+00002440: 6870 7a08 2e67 656f 6a73 6f6e da0e 636f  hpz..geojson..co
+00002450: 6e6e 6563 7465 645f 6c61 6b65 729b 0000  nnected_laker...
+00002460: 0072 4100 0000 da07 7276 684e 616d 65da  .rA.....rvhName.
+00002470: 0373 7562 7252 0000 005a 0747 656f 4a53  .subrR...Z.GeoJS
+00002480: 4f4e 2901 da06 6472 6976 6572 6900 0400  ON)...driveri...
+00002490: 00e9 6400 0000 69f4 0100 00da 0866 6561  ..d...i......fea
+000024a0: 7475 7265 7372 0800 0000 7265 0000 007a  turesr....re...z
+000024b0: 2272 6f75 7469 6e67 5f70 726f 6475 6374  "routing_product
+000024c0: 5f6c 616b 655f 7269 7665 722e 6765 6f6a  _lake_river.geoj
+000024d0: 736f 6eda 0177 7a05 7574 662d 3829 01da  son..wz.utf-8)..
+000024e0: 0865 6e63 6f64 696e 6746 2902 da0c 656e  .encodingF)...en
+000024f0: 7375 7265 5f61 7363 6969 da06 696e 6465  sure_ascii..inde
+00002500: 6e74 291a 726e 0000 0072 6f00 0000 da07  nt).rn...ro.....
+00002510: 6469 726e 616d 65da 0862 6173 656e 616d  dirname..basenam
+00002520: 65da 0573 706c 6974 7220 0000 00da 0572  e..splitr .....r
+00002530: 616e 6765 726b 0000 00da 0665 7869 7374  angerk.....exist
+00002540: 7372 2200 0000 722f 0000 0072 3000 0000  sr"...r/...r0...
+00002550: 7231 0000 00da 0661 7374 7970 65da 0369  r1.....astype..i
+00002560: 6e74 da03 7374 7272 7300 0000 7270 0000  nt..strrs...rp..
+00002570: 00da 0873 696d 706c 6966 7972 6d00 0000  ...simplifyrm...
+00002580: da04 7374 6174 da07 7374 5f73 697a 6572  ..stat..st_sizer
+00002590: 0200 0000 da04 6f70 656e da04 6a73 6f6e  ......open..json
+000025a0: da04 6475 6d70 291c da12 496e 7075 745f  ..dump)...Input_
+000025b0: 506f 6c79 676f 6e5f 7061 7468 da0b 7072  Polygon_path..pr
+000025c0: 6f64 7563 745f 6469 72da 084e 616d 6573  oduct_dir..Names
+000025d0: 5f69 6eda 076e 5f63 6861 7263 da07 7665  _in..n_charc..ve
+000025e0: 7273 696f 6eda 0a54 4f4c 4552 414e 4345  rsion..TOLERANCE
+000025f0: 73da 0d68 6561 645f 6e61 6d65 5f63 6174  s..head_name_cat
+00002600: da0d 6865 6164 5f6e 616d 655f 7269 76da  ..head_name_riv.
+00002610: 0f68 6561 645f 6e61 6d65 5f73 6c61 6b65  .head_name_slake
+00002620: da0f 6865 6164 5f6e 616d 655f 6e6c 616b  ..head_name_nlak
+00002630: 65da 0f49 6e70 7574 5f66 696c 655f 6e61  e..Input_file_na
+00002640: 6d65 da10 4f75 7470 7574 5f66 696c 655f  me..Output_file_
+00002650: 6e61 6d65 da13 6372 6561 7465 645f 6a61  name..created_ja
+00002660: 736f 6e5f 6669 6c65 73da 1c63 7265 6174  son_files..creat
+00002670: 6564 5f6a 6173 6f6e 5f66 696c 6573 5f6c  ed_jason_files_l
+00002680: 616b 655f 7269 7672 2400 0000 da0a 696e  ake_rivr$.....in
+00002690: 7075 745f 7061 7468 da11 6f75 7470 7574  put_path..output
+000026a0: 5f6a 6173 6f6e 5f70 6174 685a 0869 6e70  _jason_pathZ.inp
+000026b0: 7574 5f70 64da 0c69 6e70 7574 5f77 6773  ut_pd..input_wgs
+000026c0: 5f38 34da 0369 6478 da0c 696e 7075 745f  _84..idx..input_
+000026d0: 746f 6a73 6f6e da09 544f 4c45 5241 4e43  tojson..TOLERANC
+000026e0: 45da 0e6a 736f 6e5f 6669 6c65 5f73 697a  E..json_file_siz
+000026f0: 65da 0769 6e6a 736f 6e32 da0c 6e65 775f  e..injson2..new_
+00002700: 6665 6174 7572 6573 da07 656c 656d 656e  features..elemen
+00002710: 74da 156f 7574 7075 745f 6a61 736f 6e5f  t..output_jason_
+00002720: 6c61 6b65 5f72 6976 da01 6672 0a00 0000  lake_riv..fr....
+00002730: 720a 0000 0072 0e00 0000 7272 0000 0049  r....r....rr...I
+00002740: 0100 0073 9000 0000 0002 0802 0402 0c01  ...s............
+00002750: 1201 0801 1401 0803 0401 0401 0401 0402  ................
+00002760: 0401 0401 0802 0e01 0e01 0e01 0efc 0407  ................
+00002770: 0e01 0e01 0e01 0efc 0608 0601 0601 0601  ................
+00002780: 06fc 0407 0601 0601 0601 06fc 0406 0401  ................
+00002790: 0402 1401 1201 1201 0e01 0401 0a02 1c01  ................
+000027a0: 0a03 0a02 0a04 1c01 1801 0a01 2003 0402  ............ ...
+000027b0: 0801 0e01 0e02 1401 0a01 0e02 3601 1201  ............6...
+000027c0: 1001 0e01 0401 0c01 1201 0e01 0802 0a01  ................
+000027d0: 0602 1802 1a01 3202 7272 0000 0063 0200  ......2.rr...c..
+000027e0: 0000 0000 0000 0000 0000 0a00 0000 0300  ................
+000027f0: 0000 4300 0000 7398 0000 0074 00a0 017c  ..C...s....t...|
+00002800: 00a1 016a 0264 0167 0164 028d 017d 0274  ...j.d.g.d...}.t
+00002810: 037c 0283 017d 0374 047c 0264 0319 0083  .|...}.t.|.d....
+00002820: 017d 0474 047c 0264 0419 0083 017d 0574  .}.t.|.d.....}.t
+00002830: 00a0 017c 01a1 016a 0264 0167 0164 028d  ...|...j.d.g.d..
+00002840: 017d 0674 037c 0683 017d 0774 047c 0664  .}.t.|...}.t.|.d
+00002850: 0319 0083 017d 0874 047c 0664 0419 0083  .....}.t.|.d....
+00002860: 017d 097c 037c 076b 0273 744a 0082 017c  .}.|.|.k.stJ...|
+00002870: 047c 0818 0064 056b 0073 844a 0082 017c  .|...d.k.s.J...|
+00002880: 057c 0918 0064 066b 0073 944a 0082 0164  .|...d.k.s.J...d
+00002890: 0753 0029 087a 6d74 6573 7420 6675 6e63  .S.).zmtest func
+000028a0: 7469 6f6e 2074 6861 7420 7769 6c6c 3a0a  tion that will:.
+000028b0: 2020 2020 4675 6e63 7469 6f6e 2074 6861      Function tha
+000028c0: 7420 7573 6564 2074 6f20 636f 6d70 6172  t used to compar
+000028d0: 6520 7477 6f20 6361 7463 686d 656e 7420  e two catchment 
+000028e0: 6669 6c65 730a 2020 2020 6672 6f6d 2072  files.    from r
+000028f0: 6f75 7469 6e67 2070 726f 6475 6374 730a  outing products.
+00002900: 2020 2020 7241 0000 00a9 0172 5700 0000      rA.....rW...
+00002910: 7260 0000 00da 0742 6173 4172 6561 721e  r`.....BasArear.
+00002920: 0000 00e9 0a00 0000 4ea9 0572 2f00 0000  ........N..r/...
+00002930: 7230 0000 00da 0b73 6f72 745f 7661 6c75  r0.....sort_valu
+00002940: 6573 7220 0000 00da 0373 756d 290a 5a05  esr .....sum).Z.
+00002950: 6361 745f 615a 0563 6174 5f62 5a18 4578  cat_aZ.cat_bZ.Ex
+00002960: 7065 6374 5f46 696e 616c 7269 765f 696e  pect_Finalriv_in
+00002970: 666f 5f70 6c79 5a0c 4578 7065 6374 5f4e  fo_plyZ.Expect_N
+00002980: 5f43 6174 5a0e 4578 7065 6374 5f6c 656e  _CatZ.Expect_len
+00002990: 5f52 6976 5a0f 4578 7065 6374 5f42 6173  _RivZ.Expect_Bas
+000029a0: 5f41 7265 61da 1852 6573 756c 745f 4669  _Area..Result_Fi
+000029b0: 6e61 6c72 6976 5f69 6e66 6f5f 706c 795a  nalriv_info_plyZ
+000029c0: 0c52 6573 756c 745f 4e5f 4361 745a 0e52  .Result_N_CatZ.R
+000029d0: 6573 756c 745f 6c65 6e5f 5269 765a 0f52  esult_len_RivZ.R
+000029e0: 6573 756c 745f 4261 735f 4172 6561 720a  esult_Bas_Arear.
+000029f0: 0000 0072 0a00 0000 720e 0000 00da 1163  ...r....r......c
+00002a00: 6f6d 7061 7265 5f63 6174 6368 6d65 6e74  ompare_catchment
+00002a10: b001 0000 7316 0000 0000 0714 0208 020c  ....s...........
+00002a20: 020c 0314 0208 020c 020c 030c 0210 0172  ...............r
+00002a30: dd00 0000 6302 0000 0000 0000 0000 0000  ....c...........
+00002a40: 0002 0000 0006 0000 0043 0000 0073 5600  .........C...sV.
+00002a50: 0000 7400 7401 6a02 a003 7c00 6401 a102  ..t.t.j...|.d...
+00002a60: 7401 6a02 a003 7c01 6401 a102 8302 0100  t.j...|.d.......
+00002a70: 7401 6a02 a004 7401 6a02 a003 7c00 6402  t.j...t.j...|.d.
+00002a80: a102 a101 7252 7400 7401 6a02 a003 7c00  ....rRt.t.j...|.
+00002a90: 6402 a102 7401 6a02 a003 7c01 6402 a102  d...t.j...|.d...
+00002aa0: 8302 0100 6400 5300 2903 4e7a 2863 6174  ....d.S.).Nz(cat
+00002ab0: 6368 6d65 6e74 5f77 6974 686f 7574 5f6d  chment_without_m
+00002ac0: 6572 6769 6e67 5f6c 616b 6573 5f76 312d  erging_lakes_v1-
+00002ad0: 302e 7368 707a 1666 696e 616c 6361 745f  0.shpz.finalcat_
+00002ae0: 696e 666f 5f76 312d 302e 7368 7029 0572  info_v1-0.shp).r
+00002af0: dd00 0000 726e 0000 0072 6f00 0000 726b  ....rn...ro...rk
+00002b00: 0000 0072 b200 0000 2902 5a10 7072 6f64  ...r....).Z.prod
+00002b10: 7563 745f 666f 6c64 6572 5f61 5a10 7072  uct_folder_aZ.pr
+00002b20: 6f64 7563 745f 666f 6c64 6572 5f62 720a  oduct_folder_br.
+00002b30: 0000 0072 0a00 0000 720e 0000 00da 1063  ...r....r......c
+00002b40: 6f6d 7061 7265 5f70 726f 6475 6374 73ce  ompare_products.
+00002b50: 0100 0073 0600 0000 0001 1e02 1601 72de  ...s..........r.
+00002b60: 0000 0063 0200 0000 0000 0000 0000 0000  ...c............
+00002b70: 0800 0000 0300 0000 4300 0000 7370 0000  ........C...sp..
+00002b80: 0074 00a0 017c 00a1 016a 0264 0167 0164  .t...|...j.d.g.d
+00002b90: 028d 017d 0274 037c 0283 017d 0374 047c  ...}.t.|...}.t.|
+00002ba0: 0264 0319 0083 017d 0474 00a0 017c 01a1  .d.....}.t...|..
+00002bb0: 016a 0264 0167 0164 028d 017d 0574 037c  .j.d.g.d...}.t.|
+00002bc0: 0583 017d 0674 047c 0564 0319 0083 017d  ...}.t.|.d.....}
+00002bd0: 077c 037c 066b 0273 5c4a 0082 017c 047c  .|.|.k.s\J...|.|
+00002be0: 0718 0064 046b 0073 6c4a 0082 0164 0053  ...d.k.slJ...d.S
+00002bf0: 0029 054e da06 4852 555f 4944 72d6 0000  .).N..HRU_IDr...
+00002c00: 00da 0848 5255 5f41 7265 6172 1e00 0000  ...HRU_Arear....
+00002c10: 72d9 0000 0029 085a 0c68 7275 5f66 6f6c  r....).Z.hru_fol
+00002c20: 6465 725f 615a 0c68 7275 5f66 6f6c 6465  der_aZ.hru_folde
+00002c30: 725f 625a 0568 7275 5f61 5a0c 4578 7065  r_bZ.hru_aZ.Expe
+00002c40: 6374 5f4e 5f48 5255 5a0f 4578 7065 6374  ct_N_HRUZ.Expect
+00002c50: 5f48 5255 5f41 7265 6172 dc00 0000 5a0c  _HRU_Arear....Z.
+00002c60: 5265 7375 6c74 5f4e 5f48 5255 5a0f 5265  Result_N_HRUZ.Re
+00002c70: 7375 6c74 5f48 5255 5f41 7265 6172 0a00  sult_HRU_Arear..
+00002c80: 0000 720a 0000 0072 0e00 0000 da0c 636f  ..r....r......co
+00002c90: 6d70 6172 655f 6872 7573 d501 0000 7310  mpare_hrus....s.
+00002ca0: 0000 0000 0214 0208 020c 0314 0208 020c  ................
+00002cb0: 030c 0272 e100 0000 2902 7226 0000 0072  ...r....).r&...r
+00002cc0: 2600 0000 2901 7241 0000 0029 0172 9000  &...).rA...).r..
+00002cd0: 0000 291e 722f 0000 00da 056e 756d 7079  ..).r/.....numpy
+00002ce0: 7285 0000 0072 6e00 0000 da06 7061 6e64  r....rn.....pand
+00002cf0: 6173 7213 0000 0072 ba00 0000 7202 0000  asr....r....r...
+00002d00: 0072 0300 0000 5a08 7265 7175 6573 7473  .r....Z.requests
+00002d10: 7237 0000 00da 056f 7367 656f 7204 0000  r7.....osgeor...
+00002d20: 0072 0500 0000 5a0b 7261 7374 6572 7374  .r....Z.rasterst
+00002d30: 6174 7372 0600 0000 7219 0000 0072 2500  atsr....r....r%.
+00002d40: 0000 7240 0000 0072 7d00 0000 7271 0000  ..r@...r}...rq..
+00002d50: 0072 8c00 0000 728f 0000 0072 3400 0000  .r....r....r4...
+00002d60: 729a 0000 0072 6a00 0000 7272 0000 0072  r....rj...rr...r
+00002d70: dd00 0000 72de 0000 0072 e100 0000 720a  ....r....r....r.
+00002d80: 0000 0072 0a00 0000 720a 0000 0072 0e00  ...r....r....r..
+00002d90: 0000 da08 3c6d 6f64 756c 653e 0100 0000  ....<module>....
+00002da0: 7330 0000 0008 0108 0108 0108 0110 0108  s0..............
+00002db0: 0108 0108 0310 010c 0108 0c08 1c00 ff0a  ................
+00002dc0: 4b0a 6908 0608 1a08 050a 2308 0b08 0e08  K.i.......#.....
+00002dd0: 6708 1e08 07                             g....
```

### Comparing `basinmaker-3.0.3a0/basinmaker/func/__pycache__/qgis.cpython-39.pyc` & `basinmaker-3.1.0/basinmaker/func/__pycache__/qgis.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `basinmaker-3.0.3a0/basinmaker/func/__pycache__/rarray.cpython-39.pyc` & `basinmaker-3.1.0/basinmaker/func/__pycache__/rarray.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `basinmaker-3.0.3a0/basinmaker/func/arcgis.py` & `basinmaker-3.1.0/basinmaker/func/arcgis.py`

 * *Files 5% similar despite different names*

```diff
@@ -514,15 +514,33 @@
     excludeids = routing_info[~routing_info["SubId"].isin(lake_inlet_subids)]["SubId"].values
     arcgis_raster_setnull_array("str_r","lake_inflow_str",excludeids,cellSize,SptailRef,work_folder,snapRaster)
 
     remove_value_not_on_lake_inflow_str = Con(IsNull("lake_inflow_str"),-9999,"str_around_lake_inlets")
     remove_value_inside_lakes = Con(IsNull(sl_lakes+"_r"),remove_value_not_on_lake_inflow_str,-9999)
     remove_value_inside_lakes_no999 = SetNull(remove_value_inside_lakes,remove_value_inside_lakes,"VALUE = -9999")
     remove_value_inside_lakes_no999.save("lake_inflow_seg_outside_lake")
-    find_zonal_maximum_or_minimum_point_on_the_raster("lake_inflow_seg_outside_lake",acc,lake_inflow_pourpoints,"MAXIMUM",cellSize,SptailRef,work_folder,snapRaster)
+
+    # arcgis potential inflow point raster to points
+    arcpy.RasterToPoint_conversion("lake_inflow_seg_outside_lake", "lake_inflow_seg_outside_lake_v", "VALUE")
+    ExtractMultiValuesToPoints("lake_inflow_seg_outside_lake_v",acc,"NONE")
+
+
+    inlet_inlake_table = pd.DataFrame.spatial.from_featureclass("lake_inlet_inlake_v")
+    inlet_inlake_table['acc_max'] = inlet_inlake_table['acc']
+    inlet_inlake_table = inlet_inlake_table[['grid_code','acc_max']]
+    inlet_outside_lake_table = pd.DataFrame.spatial.from_featureclass("lake_inflow_seg_outside_lake_v")
+
+    inlet_outside_lake_table = inlet_outside_lake_table.merge(inlet_inlake_table,on='grid_code',how='left')
+    inlet_outside_lake_table = inlet_outside_lake_table[inlet_outside_lake_table['acc'] < inlet_outside_lake_table['acc_max']]
+
+    inlet_outside_lake_table = inlet_outside_lake_table.sort_values(by=['acc'],ascending = False)
+    inlet_outside_lake_table = inlet_outside_lake_table.drop_duplicates(subset=['grid_code'], keep='first')
+    inlet_outside_lake_table.spatial.to_featureclass(location=os.path.join(work_folder,"arcgis.gdb",lake_inflow_pourpoints + "_v"),overwrite=True,sanitize_columns=False)
+
+#    find_zonal_maximum_or_minimum_point_on_the_raster("lake_inflow_seg_outside_lake",acc,lake_inflow_pourpoints,"MAXIMUM",cellSize,SptailRef,work_folder,snapRaster)
 
     arcpy.RasterToPoint_conversion(catchment_pourpoints_outside_lake, catchment_pourpoints_outside_lake + "_v", "VALUE")
 
     cat_outlet =  pd.DataFrame.spatial.from_featureclass(catchment_pourpoints_outside_lake + "_v")
     lake_inlets =  pd.DataFrame.spatial.from_featureclass(lake_inflow_pourpoints + "_v")
     lake_outlets =  pd.DataFrame.spatial.from_featureclass(lake_outflow_pourpoints + "_v")
```

### Comparing `basinmaker-3.0.3a0/basinmaker/func/fgdal.py` & `basinmaker-3.1.0/basinmaker/func/fgdal.py`

 * *Files identical despite different names*

### Comparing `basinmaker-3.0.3a0/basinmaker/func/grassgis.py` & `basinmaker-3.1.0/basinmaker/func/grassgis.py`

 * *Files identical despite different names*

### Comparing `basinmaker-3.0.3a0/basinmaker/func/pdtable.py` & `basinmaker-3.1.0/basinmaker/func/pdtable.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,94 +6,106 @@
 from basinmaker.utilities.utilities import *
 import numbers
 from joblib import Parallel, delayed
 import tempfile
 pd.options.mode.chained_assignment = None
 
 
-def update_selected_subid_using_sec_downsubid(sec_down_subinfo,upstream_subs,cat_ply,hyshdinfo):
+def update_selected_subid_using_sec_downsubid(sec_down_subinfo, upstream_subs, cat_ply, hyshdinfo):
     is_sec_down_subid_in_selected_subid = False
     is_subid_of_sec_downsubid_in_selected_subid = False
     update_downsubids_using_sec_downsubid = False
     update_topology = False
     # identify sec_down_subinfo subbains that downsubid is not in the subid list
-    sec_down_subinfo_mostdown = sec_down_subinfo[~sec_down_subinfo['Sec_DowSubId'].isin(sec_down_subinfo['SubId'].values)]
-    sec_down_subid_in_selected_subid = sec_down_subinfo_mostdown['Sec_DowSubId'].isin(upstream_subs).copy(deep=True)
+    sec_down_subinfo_mostdown = sec_down_subinfo[~sec_down_subinfo['Sec_DowSubId'].isin(
+        sec_down_subinfo['SubId'].values)]
+    sec_down_subid_in_selected_subid = sec_down_subinfo_mostdown['Sec_DowSubId'].isin(
+        upstream_subs).copy(deep=True)
 
     # check if downsubid in the secondary downsubid list exist in the selected subbasin
     # if not means the secondary downsubid has no impact on this area
     # return the input directly
-    sec_down_subinfo_downsub_in_selected = sec_down_subinfo_mostdown[sec_down_subid_in_selected_subid]
+    sec_down_subinfo_downsub_in_selected = sec_down_subinfo_mostdown[
+        sec_down_subid_in_selected_subid]
 
     if len(sec_down_subinfo_downsub_in_selected) <= 0:
-        return upstream_subs,cat_ply,update_topology
+        return upstream_subs, cat_ply, update_topology
 
     # check subid of secondary downsub id that are in the selected subids
     # is in the selected subid or not
     # if they all inlucded in the selected subid
     # means the secondary downsubid has no impact on this area
     # return the input directly
-    missing_subid_in_sec_table = sec_down_subinfo_downsub_in_selected[~sec_down_subinfo_downsub_in_selected['SubId'].isin(upstream_subs)].copy(deep=True)
+    missing_subid_in_sec_table = sec_down_subinfo_downsub_in_selected[~sec_down_subinfo_downsub_in_selected['SubId'].isin(
+        upstream_subs)].copy(deep=True)
 
     if len(missing_subid_in_sec_table) <= 0:
-        return upstream_subs,cat_ply,update_topology
+        return upstream_subs, cat_ply, update_topology
 
     # obtain routing topology for secondary table
-    hyshdinfo_sec = sec_down_subinfo[['SubId', 'Sec_DowSubId']].astype("int32").values
+    hyshdinfo_sec = sec_down_subinfo[[
+        'SubId', 'Sec_DowSubId']].astype("int32").values
     for subid_sec in missing_subid_in_sec_table['SubId'].values:
-        #obtain subids in the sec_down_subinfo drainage to this  subid_sec
+        # obtain subids in the sec_down_subinfo drainage to this  subid_sec
         upstream_subs_sec = defcat(hyshdinfo_sec, subid_sec)
-        sec_down_subinfoselect = sec_down_subinfo[sec_down_subinfo['SubId'].isin(upstream_subs_sec)]
+        sec_down_subinfoselect = sec_down_subinfo[sec_down_subinfo['SubId'].isin(
+            upstream_subs_sec)]
         # update the DownSubId in the cat_ply using using Sec_DowSubId for upstream_subs
-        cat_ply = cat_ply.merge(sec_down_subinfoselect,on='SubId',how='left')
+        cat_ply = cat_ply.merge(sec_down_subinfoselect, on='SubId', how='left')
         mask = cat_ply['SubId'].isin(upstream_subs_sec)
-        cat_ply.loc[mask,'DowSubId'] = cat_ply.loc[mask,'Sec_DowSubId'].values
+        cat_ply.loc[mask, 'DowSubId'] = cat_ply.loc[mask,
+                                                    'Sec_DowSubId'].values
         # update the routing topology and get the subbasin drainage to this subid_sec
         hyshdinfo = cat_ply[['SubId', 'DowSubId']].astype("int32").values
         upstream_subs_new_sub_sec = defcat(hyshdinfo, subid_sec)
         # add the new subids into the eixisting upstream subids
-        upstream_subs = np.concatenate((upstream_subs, upstream_subs_new_sub_sec), axis=0)
+        upstream_subs = np.concatenate(
+            (upstream_subs, upstream_subs_new_sub_sec), axis=0)
         cat_ply = cat_ply.drop(columns='Sec_DowSubId')
     update_topology = True
-    return upstream_subs,cat_ply,update_topology
+    return upstream_subs, cat_ply, update_topology
 
-def return_extracted_subids(cat_ply,mostdownid,mostupstreamid,sec_down_subinfo):
+
+def return_extracted_subids(cat_ply, mostdownid, mostupstreamid, sec_down_subinfo):
 
     # flags for sec down subid
     has_sec_downsub = False
     update_downsubids_using_sec_downsubid = False
 
     hyshdinfo = cat_ply[['SubId', 'DowSubId']].astype("int32").values
     sum_update_topology = 0
     update_topology = 0
-    ## find all subid control by this subid
-    for i_down in range(0,len(mostdownid)):
-        ### Loop for each downstream id
+    # find all subid control by this subid
+    for i_down in range(0, len(mostdownid)):
+        # Loop for each downstream id
         tar_subid = mostdownid[i_down]
 
-        upstream_subs,cat_ply,update_topology = return_subids_drainage_to_subid(tar_subid,hyshdinfo,sec_down_subinfo,cat_ply)
+        upstream_subs, cat_ply, update_topology = return_subids_drainage_to_subid(
+            tar_subid, hyshdinfo, sec_down_subinfo, cat_ply)
         sum_update_topology = sum_update_topology + update_topology
         if i_down == 0:
             selected_subs = upstream_subs
         else:
-            selected_subs = np.concatenate((selected_subs, upstream_subs), axis=0)
+            selected_subs = np.concatenate(
+                (selected_subs, upstream_subs), axis=0)
 
     selected_subs = np.unique(selected_subs)
 
-    ## find all subid control by this subid
+    # find all subid control by this subid
     remove_subs = np.empty(0, dtype=int)
 
-    for i_up in range(0,len(mostupstreamid)):
-        ### Loop for each downstream id
+    for i_up in range(0, len(mostupstreamid)):
+        # Loop for each downstream id
         tar_subid = mostupstreamid[i_up]
 
         if tar_subid < 0:
             continue
 
-        upstream_subs,cat_ply,update_topology = return_subids_drainage_to_subid(tar_subid,hyshdinfo,sec_down_subinfo,cat_ply)
+        upstream_subs, cat_ply, update_topology = return_subids_drainage_to_subid(
+            tar_subid, hyshdinfo, sec_down_subinfo, cat_ply)
 
         if i_up == 0:
             remove_subs = upstream_subs
         else:
             remove_subs = np.concatenate((remove_subs, upstream_subs), axis=0)
 
     if len(remove_subs) > 0:
@@ -102,182 +114,197 @@
         mask = ~np.in1d(selected_subs, remove_subs)
 
         selected_subs = selected_subs[mask]
     if sum_update_topology >= 1:
         update_topology = True
     else:
         update_topology = False
-    return selected_subs,cat_ply,update_topology
-
-
-
+    return selected_subs, cat_ply, update_topology
 
 
-def return_subids_drainage_to_subid(tar_subid,hyshdinfo,sec_down_subinfo,cat_ply):
+def return_subids_drainage_to_subid(tar_subid, hyshdinfo, sec_down_subinfo, cat_ply):
 
-    ## find all subid control by this subid
+    # find all subid control by this subid
     upstream_subs = defcat(hyshdinfo, tar_subid)
     update_topology = 0
     # check if has sencondary down subid
     if len(sec_down_subinfo) > 0:
-        upstream_subs,cat_ply,update_topology = update_selected_subid_using_sec_downsubid(sec_down_subinfo,upstream_subs,cat_ply,hyshdinfo)
+        upstream_subs, cat_ply, update_topology = update_selected_subid_using_sec_downsubid(
+            sec_down_subinfo, upstream_subs, cat_ply, hyshdinfo)
 
-    return upstream_subs,cat_ply,update_topology
+    return upstream_subs, cat_ply, update_topology
 
-def remove_landuse_type_input_based_on_area(landuse_thres,hruinfo,sub_area,Landuse_ID):
+
+def remove_landuse_type_input_based_on_area(landuse_thres, hruinfo, sub_area, Landuse_ID):
 
     if landuse_thres <= 0:
         return hruinfo
     # calculate the landuse area of each landuse group in each subbasin
-    subinfo_lu = hruinfo[['SubId',Landuse_ID,'HRU_Area']].copy(deep=True)
+    subinfo_lu = hruinfo[['SubId', Landuse_ID, 'HRU_Area']].copy(deep=True)
     subinfo_lu = subinfo_lu.rename(columns={"HRU_Area": "Input_A_G"})
-    subinfo_lu = subinfo_lu.groupby(['SubId',Landuse_ID],as_index = False).sum()
+    subinfo_lu = subinfo_lu.groupby(
+        ['SubId', Landuse_ID], as_index=False).sum()
 
-    #calcuate landuse area ratio
+    # calcuate landuse area ratio
     subinfo_lu = pd.merge(subinfo_lu, sub_area, on='SubId')
     subinfo_lu['Area_ratio'] = subinfo_lu["Input_A_G"]/subinfo_lu['Bas_A_G']
 
     # obtain dominated landuse ID
-    subinfo_lu = subinfo_lu.sort_values(by=['SubId','Input_A_G'], ascending=False)
-    subinfo_lu_dominated = subinfo_lu.drop_duplicates(subset=['SubId'], keep='first').copy(deep=True)
+    subinfo_lu = subinfo_lu.sort_values(
+        by=['SubId', 'Input_A_G'], ascending=False)
+    subinfo_lu_dominated = subinfo_lu.drop_duplicates(
+        subset=['SubId'], keep='first').copy(deep=True)
 
     # find sub
-    subinfo_lu_need_change = subinfo_lu[subinfo_lu['Area_ratio'] < landuse_thres][['SubId',Landuse_ID]].copy(deep=True)
+    subinfo_lu_need_change = subinfo_lu[subinfo_lu['Area_ratio'] < landuse_thres][[
+        'SubId', Landuse_ID]].copy(deep=True)
 
-    for i in range(0,len(subinfo_lu_need_change)):
+    for i in range(0, len(subinfo_lu_need_change)):
         subid = subinfo_lu_need_change['SubId'].values[i]
         landuse = subinfo_lu_need_change[Landuse_ID].values[i]
         mask1 = hruinfo['SubId'] == subid
         mask2 = hruinfo[Landuse_ID] == landuse
-        mask = np.logical_and(mask1,mask2)
-        hruinfo.loc[mask,Landuse_ID] = subinfo_lu_dominated.loc[subinfo_lu_dominated['SubId'] == subid][Landuse_ID].values[0]
+        mask = np.logical_and(mask1, mask2)
+        hruinfo.loc[mask, Landuse_ID] = subinfo_lu_dominated.loc[subinfo_lu_dominated['SubId']
+                                                                 == subid][Landuse_ID].values[0]
 
     return hruinfo
 
-def simplify_hrus_method2(area_ratio_thresholds,hruinfo, Landuse_ID,
-                          Soil_ID,Veg_ID,Other_Ply_ID_1,Other_Ply_ID_2):
+
+def simplify_hrus_method2(area_ratio_thresholds, hruinfo, Landuse_ID,
+                          Soil_ID, Veg_ID, Other_Ply_ID_1, Other_Ply_ID_2):
 
     hru_lake_info = hruinfo.loc[hruinfo['HRU_IsLake'] > 0].copy()
     hru_land_info = hruinfo.loc[hruinfo['HRU_IsLake'] <= 0].copy()
 
-    sub_area = hruinfo[['SubId','HRU_Area']].copy(deep=True)
+    sub_area = hruinfo[['SubId', 'HRU_Area']].copy(deep=True)
     sub_area = sub_area.rename(columns={"HRU_Area": "Bas_A_G"})
-    sub_area = sub_area.groupby(['SubId'],as_index = False).sum()
+    sub_area = sub_area.groupby(['SubId'], as_index=False).sum()
 #    hruinfo = pd.merge(hruinfo, subinfo, on='SubId')
 
     landuse_thres = area_ratio_thresholds[0]
-    list = [Landuse_ID,Soil_ID,Other_Ply_ID_1]
-    for i in range(0,len(list)):
+    list = [Landuse_ID, Soil_ID, Other_Ply_ID_1]
+    for i in range(0, len(list)):
         Item = list[i]
         landuse_thres = area_ratio_thresholds[i]
-        hru_land_info = remove_landuse_type_input_based_on_area(landuse_thres,hru_land_info,sub_area,Item)
+        hru_land_info = remove_landuse_type_input_based_on_area(
+            landuse_thres, hru_land_info, sub_area, Item)
     hru_land_info[Veg_ID] = hru_land_info[Landuse_ID]
 
     hruinfo = hru_lake_info.append(hru_land_info)
 
     return hruinfo
 
 
-
-def simplidfy_hrus(min_hru_pct_sub_area,hruinfo,importance_order):
+def simplidfy_hrus(min_hru_pct_sub_area, hruinfo, importance_order):
 
     hruinfo['HRU_ID_New2'] = hruinfo['HRU_ID_New']
 
     subids = np.unique(hruinfo['SubId'].values)
 
     # loop for each subbasin
-    for i in range(0,len(subids)):
+    for i in range(0, len(subids)):
         subid = subids[i]
         # hrus in this subbasin
-        sub_hru_info = hruinfo.loc[hruinfo['SubId'] == subid].copy(deep = True)
+        sub_hru_info = hruinfo.loc[hruinfo['SubId'] == subid].copy(deep=True)
         # calculate area and subbasin minimum hur ares
         subasrea = np.sum(sub_hru_info['HRU_Area'].values)
         subarea_thrs = min_hru_pct_sub_area * subasrea
 
         # obtain hru need to be removed
-        need_remove_hrus = sub_hru_info.loc[sub_hru_info['HRU_Area'] < subarea_thrs].copy()
+        need_remove_hrus = sub_hru_info.loc[sub_hru_info['HRU_Area'] < subarea_thrs].copy(
+        )
         # obtain hrus that will be keepted
-        good_hrus = sub_hru_info.loc[sub_hru_info['HRU_Area'] >= subarea_thrs].copy()
+        good_hrus = sub_hru_info.loc[sub_hru_info['HRU_Area']
+                                     >= subarea_thrs].copy()
 
         hru_columns = good_hrus.columns
         # do not modify this columns
         hru_columns = hru_columns[hru_columns != 'HRU_ID_New2']
         # check if the need_remove_hru can merge togeher for importance order
         # 1
         colnm1 = importance_order[0]
         import1_Area_need_remove_hru = need_remove_hrus.copy(deep=True)
         unique_import1 = np.unique(import1_Area_need_remove_hru[colnm1].values)
         # if subid == 116:
         #     print(subarea_thrs,min_hru_pct_sub_area,subasrea)
         #     print(need_remove_hrus[['HRU_ID_New2','HRU_Area',colnm1]])
 
-        for i_import in range(0,len(unique_import1)):
+        for i_import in range(0, len(unique_import1)):
             i_colnm1 = unique_import1[i_import]
-            i_import1_Area_need_remove_hru = import1_Area_need_remove_hru.loc[import1_Area_need_remove_hru[colnm1] == i_colnm1].copy(deep=True)
-            total_area_i_import_in_need_remove_hrus = np.sum(i_import1_Area_need_remove_hru['HRU_Area'].values)
-            ## check total area of the most important column in the importance list
-            ## if it is larger than area threthold,
-            ## then merge them together
+            i_import1_Area_need_remove_hru = import1_Area_need_remove_hru.loc[import1_Area_need_remove_hru[colnm1] == i_colnm1].copy(
+                deep=True)
+            total_area_i_import_in_need_remove_hrus = np.sum(
+                i_import1_Area_need_remove_hru['HRU_Area'].values)
+            # check total area of the most important column in the importance list
+            # if it is larger than area threthold,
+            # then merge them together
 
             if total_area_i_import_in_need_remove_hrus >= subarea_thrs:
 
-                #merge to the hru with largest area in the list
-                i_import1_Area_need_remove_hru = i_import1_Area_need_remove_hru.sort_values(by=['HRU_Area'],ascending=False)
-                for i_nm in range(0,len(hru_columns)):
+                # merge to the hru with largest area in the list
+                i_import1_Area_need_remove_hru = i_import1_Area_need_remove_hru.sort_values(
+                    by=['HRU_Area'], ascending=False)
+                for i_nm in range(0, len(hru_columns)):
                     columnname = hru_columns[i_nm]
                     if columnname == 'SHAPE':
                         continue
                     # modify the hru attributes to good hru attribute
-                    hruinfo.loc[hruinfo['HRU_ID_New2'].isin(i_import1_Area_need_remove_hru['HRU_ID_New2'].values),columnname] = i_import1_Area_need_remove_hru[columnname].values[0]
+                    hruinfo.loc[hruinfo['HRU_ID_New2'].isin(
+                        i_import1_Area_need_remove_hru['HRU_ID_New2'].values), columnname] = i_import1_Area_need_remove_hru[columnname].values[0]
 
                 # remove modified HRU from need removed hru list
-                need_remove_hrus = need_remove_hrus[~need_remove_hrus['HRU_ID_New2'].isin(i_import1_Area_need_remove_hru['HRU_ID_New2'].values)]
+                need_remove_hrus = need_remove_hrus[~need_remove_hrus['HRU_ID_New2'].isin(
+                    i_import1_Area_need_remove_hru['HRU_ID_New2'].values)]
         # loop for each
         indexes = need_remove_hrus.index
         # if subid == 116:
         #     print(need_remove_hrus[['HRU_ID_New2','HRU_Area',colnm1]])
 
-        for j in range(0,len(indexes)):
+        for j in range(0, len(indexes)):
             idx = indexes[j]
-            hruid = need_remove_hrus.loc[idx,'HRU_ID_New2']
+            hruid = need_remove_hrus.loc[idx, 'HRU_ID_New2']
             # find a target hru from good_hrus, and merge them by change attribute
 
             # loop the importance_order,
-            for k in range(0,len(importance_order)):
+            for k in range(0, len(importance_order)):
                 colnm = importance_order[k]
                 # find the attribute value of the problem hru for this column
-                attri_remove_hru = need_remove_hrus.loc[idx,colnm]
+                attri_remove_hru = need_remove_hrus.loc[idx, colnm]
 
                 # check if there is good hrus has the same attribute value
-                good_hrus_k  = good_hrus.loc[good_hrus[colnm] == attri_remove_hru].copy()
+                good_hrus_k = good_hrus.loc[good_hrus[colnm]
+                                            == attri_remove_hru].copy()
 
                 if len(good_hrus_k) > 0:
                     # sort by hru areas
-                    good_hrus_k = good_hrus_k.sort_values(by='HRU_Area', ascending=False)
-                    for i_nm in range(0,len(hru_columns)):
+                    good_hrus_k = good_hrus_k.sort_values(
+                        by='HRU_Area', ascending=False)
+                    for i_nm in range(0, len(hru_columns)):
                         columnname = hru_columns[i_nm]
                         if columnname == 'SHAPE':
                             continue
                         # modify the hru attributes to good hru attribute
-                        hruinfo.loc[hruinfo['HRU_ID_New2'] == hruid,columnname] = good_hrus_k[columnname].values[0]
+                        hruinfo.loc[hruinfo['HRU_ID_New2'] == hruid,
+                                    columnname] = good_hrus_k[columnname].values[0]
                 else:
                     continue
     hruinfo = hruinfo.drop(columns=['HRU_ID_New2'])
     return hruinfo
 
 
 def update_non_connected_catchment_info(catinfo):
     routing_info = catinfo[["SubId", "DowSubId"]].astype("float").values
     catinfo_non_connected = catinfo.loc[catinfo["Lake_Cat"] == 2].copy()
 
     catids_nc = catinfo_non_connected["SubId"].copy()
     max_seg_id = catinfo["Seg_ID"].max()
-    catinfo.loc[
-        catinfo["SubId"].isin(catids_nc), "RivLength"
-    ] = 0.0  ## no reiver length since not connected.
+    # catinfo.loc[
+    #     catinfo["SubId"].isin(catids_nc), "RivLength"
+    # ] = 0.0  ## no reiver length since not connected.
 
     for i in range(0, len(catinfo_non_connected)):
         c_subid = catinfo_non_connected["SubId"].values[i]
         d_subid = catinfo_non_connected["DowSubId"].values[i]
         d_sub_info = catinfo.loc[catinfo["SubId"] == d_subid].copy()
 
         lc_subid = d_subid
@@ -288,48 +315,48 @@
         #
         # DA = sum(Up_cat_info["BasArea"].values)
         #
         # catinfo.loc[catinfo["SubId"] == c_subid, "DrainArea"] = DA
 
         if len(d_sub_info) < 1:
             catinfo.loc[catinfo["SubId"] == c_subid, "Strahler"] = 1
-            catinfo.loc[catinfo["SubId"] == c_subid, "Seg_ID"] = max_seg_id + i + 1
+            catinfo.loc[catinfo["SubId"] == c_subid,
+                        "Seg_ID"] = max_seg_id + i + 1
             catinfo.loc[catinfo["SubId"] == c_subid, "Seg_order"] = 1
             continue
 
-        ## add nonconnected lake catchment area to downsubbasin drinage area
+        # add nonconnected lake catchment area to downsubbasin drinage area
         #        if d_sub_info['Lake_Cat'].values[0]  != 2:
         #            catinfo.loc[catinfo['SubId'] == d_subid,'DA'] = d_sub_info['DA'].values[0] + DA
 
         while d_sub_info["Lake_Cat"].values[0] == 2:
             lc_subid_info = catinfo.loc[catinfo["SubId"] == lc_subid].copy()
             d_subid = lc_subid_info["DowSubId"].values[0]
             d_sub_info = catinfo.loc[catinfo["SubId"] == d_subid].copy()
             if len(d_sub_info) < 1:
                 lc_subid = -1
                 break
             if lc_subid == d_sub_info['DowSubId'].values[0]:
-                print(lc_subid,d_subid)
+                print(lc_subid, d_subid)
                 lc_subid = -1
                 break
             lc_subid = d_subid
 
         if lc_subid == -1:
             continue
 
-        catinfo.loc[catinfo["SubId"] == c_subid, "RivSlope"] = -1.2345
-        catinfo.loc[catinfo["SubId"] == c_subid, "Ch_n"] = -1.2345
-        catinfo.loc[catinfo["SubId"] == c_subid, "RivLength"] = -1.2345
-        catinfo.loc[catinfo["SubId"] == c_subid, "Min_DEM"] = -1.2345
-        catinfo.loc[catinfo["SubId"] == c_subid, "Max_DEM"] = -1.2345
-        catinfo.loc[catinfo["SubId"] == c_subid, "FloodP_n"] = -1.2345
-        if "DA_Chn_L" in catinfo.columns:
-            catinfo.loc[catinfo["SubId"] == c_subid, "DA_Chn_L"] = -1.2345
-            catinfo.loc[catinfo["SubId"] == c_subid, "DA_Chn_Slp"] = -1.2345
-
+        # catinfo.loc[catinfo["SubId"] == c_subid, "RivSlope"] = -1.2345
+        # catinfo.loc[catinfo["SubId"] == c_subid, "Ch_n"] = -1.2345
+        # catinfo.loc[catinfo["SubId"] == c_subid, "RivLength"] = -1.2345
+        # catinfo.loc[catinfo["SubId"] == c_subid, "Min_DEM"] = -1.2345
+        # catinfo.loc[catinfo["SubId"] == c_subid, "Max_DEM"] = -1.2345
+        # catinfo.loc[catinfo["SubId"] == c_subid, "FloodP_n"] = -1.2345
+        # if "DA_Chn_L" in catinfo.columns:
+        #     catinfo.loc[catinfo["SubId"] == c_subid, "DA_Chn_L"] = -1.2345
+        #     catinfo.loc[catinfo["SubId"] == c_subid, "DA_Chn_Slp"] = -1.2345
 
         # catinfo.loc[catinfo["SubId"] == c_subid, "Q_Mean"] = d_sub_info[
         #     "Q_Mean"
         # ].values[0]
         # catinfo.loc[catinfo["SubId"] == c_subid, "BkfWidth"] = d_sub_info[
         #     "BkfWidth"
         # ].values[0]
@@ -346,21 +373,22 @@
             "Seg_order"
         ].values[0]
 
     return catinfo
 
 
 def Calculate_Longest_flowpath(mainriv_merg_info):
-    mainriv_merg_info_sort = mainriv_merg_info.sort_values(["DrainArea"], ascending=(False))
+    mainriv_merg_info_sort = mainriv_merg_info.sort_values(
+        ["DrainArea"], ascending=(False))
     #    print(mainriv_merg_info_sort[['SubId','DowSubId','DA','Strahler','RivLength']])
     longest_flow_pathes = np.full(100, 0)
     #    print(longest_flow_pathes)
     npath = 1
 
-    #### loop upstream to find longest flow path
+    # loop upstream to find longest flow path
     Pathid = np.full(1000, -1)
     subid = mainriv_merg_info_sort["SubId"].values[0]
     npath_current = 1
     Pathid[npath - 1] = subid
     #    print('####################################################################################')
     while len(Pathid[Pathid > 0]) > 0:
         nPathid = np.full(1000, -1)
@@ -370,229 +398,263 @@
         #        print(npath,Pathid[0:npath])
         #        print('###################################')
         for ipath in range(0, npath_current):
             c_subid_ipath = Pathid[ipath]
 
             if (
                 c_subid_ipath < 0
-            ):  ### means this path has been closed due to no more subbasin within the lake domain
+            ):  # means this path has been closed due to no more subbasin within the lake domain
                 continue
 
             longest_flow_pathes[ipath] = (
                 mainriv_merg_info_sort.loc[
                     mainriv_merg_info_sort["SubId"] == c_subid_ipath, "RivLength"
                 ]
                 + longest_flow_pathes[ipath]
-            )  ## add river length to current path
+            )  # add river length to current path
             Strahler_order_ipath = mainriv_merg_info_sort.loc[
                 mainriv_merg_info_sort["SubId"] == c_subid_ipath, "Strahler"
             ].values[0]
 
             upstream_sub_infos = mainriv_merg_info_sort.loc[
                 mainriv_merg_info_sort["DowSubId"] == c_subid_ipath
-            ]  ## get upstream info
+            ]  # get upstream info
 
             if (
                 len(upstream_sub_infos) <= 0
-            ):  ## no more upstream catchment within the domain of the lake
+            ):  # no more upstream catchment within the domain of the lake
                 #                print("path        closed        ",ipath)
                 continue
 
-            ## look for upstream catchment has the same upstream_sub_infos_eq_Strahler first
+            # look for upstream catchment has the same upstream_sub_infos_eq_Strahler first
             #            print(Strahler_order_ipath)
             #            print(upstream_sub_infos['Strahler'])
             upstream_sub_infos_eq_Strahler = upstream_sub_infos.loc[
                 upstream_sub_infos["Strahler"] == Strahler_order_ipath
             ]
 
             if (
                 len(upstream_sub_infos_eq_Strahler) > 0
-            ):  ### has a upstream river has the saem strahler id, no new path will be added
+            ):  # has a upstream river has the saem strahler id, no new path will be added
                 nPathid[ipath] = upstream_sub_infos_eq_Strahler["SubId"].values[
                     0
-                ]  ### add this upstream id to nPathid
+                ]  # add this upstream id to nPathid
                 continue
             else:
                 upstream_sub_infos_eq_Strahler_1 = upstream_sub_infos.loc[
                     upstream_sub_infos["Strahler"] == Strahler_order_ipath - 1
                 ]
 
                 for inpath in range(0, len(upstream_sub_infos_eq_Strahler_1)):
-                    ### this brance sperate into two or several reaches, the starting river length for all of them are the same
+                    # this brance sperate into two or several reaches, the starting river length for all of them are the same
                     if inpath == 0:
                         nPathid[ipath] = upstream_sub_infos_eq_Strahler_1[
                             "SubId"
                         ].values[inpath]
                     #                        print(nPathid[ipath],ipath,upstream_sub_infos_eq_Strahler_1['SubId'].values[inpath],'aaaaa',range(0,len(upstream_sub_infos_eq_Strahler_1)))
                     else:
                         nPathid[npath + 1 - 1] = upstream_sub_infos_eq_Strahler_1[
                             "SubId"
                         ].values[inpath]
-                        longest_flow_pathes[npath + 1 - 1] = longest_flow_pathes[ipath]
+                        longest_flow_pathes[npath + 1 -
+                                            1] = longest_flow_pathes[ipath]
                         #                        print(npath + 1 - 1,longest_flow_pathes[npath + 1 - 1],nPathid[npath + 1 - 1],'bbbbb',range(0,len(upstream_sub_infos_eq_Strahler_1)))
                         npath = npath + 1
 
         Pathid = nPathid
         npath_current = npath
     Longestpath = max(longest_flow_pathes)
 
     return Longestpath
 
-def remove_possible_small_subbasins(mapoldnew_info, area_thresthold = 1):
-    mapoldnew_info_new = mapoldnew_info.copy(deep=True)
 
+def remove_possible_small_subbasins(mapoldnew_info, area_thresthold=50, length_thresthold=15):
+    mapoldnew_info_new = mapoldnew_info.copy(deep=True)
     # check the gauge column name, in case it is v2.1 using Has_Gauge
     Gauge_col_Name = "Has_POI"
     if "Has_POI" not in mapoldnew_info.columns:
         Gauge_col_Name = "Has_Gauge"
 
     # get small subbasin that is not lake
-    small_sub_non_lake = mapoldnew_info[mapoldnew_info['BasArea']/1000/1000 < area_thresthold].copy(deep=True)
-    small_sub_non_lake = small_sub_non_lake[small_sub_non_lake['Lake_Cat'] == 0].copy(deep=True)
-    small_sub_non_lake = small_sub_non_lake[small_sub_non_lake[Gauge_col_Name] == 0].copy(deep=True)
-
-    small_sub_non_lake_subid =small_sub_non_lake['SubId'].values
-
-    ### process connected lakes  merge polygons
+    area_filter = mapoldnew_info['BasArea'] / 1000/1000 < area_thresthold
+    length_filter = mapoldnew_info['RivLength'] / 1000 < length_thresthold
+    small_sub_non_lake = mapoldnew_info[np.logical_or(
+        area_filter, length_filter)].copy(deep=True)
+    small_sub_non_lake = small_sub_non_lake[small_sub_non_lake['Lake_Cat'] == 0].copy(
+        deep=True)
+    small_sub_non_lake = small_sub_non_lake[small_sub_non_lake[Gauge_col_Name] == 0].copy(
+        deep=True)
+    small_sub_non_lake = small_sub_non_lake.sort_values(['Strahler','DrainArea'], ascending=True)
+    # process connected lakes  merge polygons
     for i in range(0, len(small_sub_non_lake)):
         small_sub_id = small_sub_non_lake['SubId'].values[i]
         small_downsub_id = small_sub_non_lake['DowSubId'].values[i]
         small_sub_seg_id = small_sub_non_lake['Seg_ID'].values[i]
 
-        small_sub_is_head_water_sub = len(mapoldnew_info[mapoldnew_info['DowSubId'] == small_sub_id]) == 0
-
         small_sub_is_not_Lake = small_sub_non_lake['Lake_Cat'].values[i] == 0
         small_sub_is_not_gauge = small_sub_non_lake[Gauge_col_Name].values[i] <= 0
 
-        down_sub_info = mapoldnew_info[mapoldnew_info['SubId'] == small_downsub_id].copy(deep = True)
-        upstream_sub_info =  mapoldnew_info[mapoldnew_info['DowSubId'] == small_sub_id].copy(deep = True)
-        upstream_sub_info_same_seg = upstream_sub_info[upstream_sub_info['Seg_ID'] == small_sub_seg_id].copy(deep=True)
-
+        down_sub_info = mapoldnew_info[mapoldnew_info['SubId'] == small_downsub_id].copy(
+            deep=True)
+        upstream_sub_info = mapoldnew_info[mapoldnew_info['DowSubId'] == small_sub_id].copy(
+            deep=True)
 
         # check if it has the same segment id with downstream subbasin
         if len(down_sub_info) > 0:
             has_down_sub = True
             if down_sub_info['Seg_ID'].values[0] == small_sub_seg_id:
                 down_sub_has_same_seg_id = True
             else:
                 down_sub_has_same_seg_id = False
+            if down_sub_info['Lake_Cat'].values[0] > 0:
+                down_sub_is_lake = True
+            else:
+                down_sub_is_lake = False
         else:
             has_down_sub = False
             down_sub_has_same_seg_id = False
-
-        # check if it has the same segment id with upstream subbasin
-        if len(upstream_sub_info) > 0:
-            has_upstream = True
-
-            if len(upstream_sub_info_same_seg) > 0 and upstream_sub_info_same_seg[Gauge_col_Name].values[0] == 0:
-                up_sub_has_same_seg_id = True
-            else:
-                up_sub_has_same_seg_id = False
-
-        else:
-            has_upstream = False
-            up_sub_has_same_seg_id = False
+            down_sub_is_lake = False
+        case = -1
 
         # if down stream sub is a lake sub, the seg_id was changed to the lake outlet subid
         if has_down_sub and down_sub_has_same_seg_id and small_sub_is_not_Lake and small_sub_is_not_gauge:
-#            tarinfo = down_sub_info
+            #            tarinfo = down_sub_info
             # merge to downstream subbasin id
-            tarinfo =  mapoldnew_info_new[mapoldnew_info_new['SubId'] == down_sub_info['SubId'].values[0]].copy(deep = True)
+            tarinfo = mapoldnew_info_new[mapoldnew_info_new['SubId']
+                                         == down_sub_info['SubId'].values[0]].copy(deep=True)
             modify = True
-            down_sub_info_2 = mapoldnew_info_new[mapoldnew_info_new['SubId'] == down_sub_info['SubId'].values[0]].copy(deep = True)
+            down_sub_info_2 = mapoldnew_info_new[mapoldnew_info_new['SubId']
+                                                 == down_sub_info['SubId'].values[0]].copy(deep=True)
             ndown_subid = down_sub_info_2['DowSubId'].values[0]
+            update_river = True
+            case = 1
 
-        elif has_upstream and up_sub_has_same_seg_id and small_sub_is_not_Lake and small_sub_is_not_gauge:
-#            tarinfo = upstream_sub_info_same_seg
-            # merge to upstream subbasin id
-            tarinfo = mapoldnew_info_new[mapoldnew_info_new['SubId'] == upstream_sub_info_same_seg['SubId'].values[0]].copy(deep = True)
+        elif down_sub_is_lake and has_down_sub and case == -1:
+            # merge to downstream subbasin id
+            #            tarinfo = down_sub_info
+            tarinfo = mapoldnew_info_new[mapoldnew_info_new['SubId']
+                                         == down_sub_info['SubId'].values[0]].copy(deep=True)
             modify = True
-            current_sub_info_2 = mapoldnew_info_new[mapoldnew_info_new['SubId'] == small_sub_id].copy(deep = True)
-            ndown_subid = current_sub_info_2['DowSubId'].values[0]
+            down_sub_info_2 = mapoldnew_info_new[mapoldnew_info_new['SubId']
+                                                 == down_sub_info['SubId'].values[0]].copy(deep=True)
+            ndown_subid = down_sub_info_2['DowSubId'].values[0]
+            update_river = False
 
-        elif len(mapoldnew_info[mapoldnew_info['Seg_ID'] == small_sub_seg_id]) == 1 and has_down_sub:
+        elif has_down_sub and case == -1:
             # merge to downstream subbasin id
-#            tarinfo = down_sub_info
-            tarinfo =  mapoldnew_info_new[mapoldnew_info_new['SubId'] == down_sub_info['SubId'].values[0]].copy(deep = True)
-            modify = True
-            down_sub_info_2 = mapoldnew_info_new[mapoldnew_info_new['SubId'] == small_downsub_id].copy(deep = True)
+            #            tarinfo = down_sub_info
+            tarinfo = mapoldnew_info_new[mapoldnew_info_new['SubId']
+                                         == down_sub_info['SubId'].values[0]].copy(deep=True)
+            down_sub_info_2 = mapoldnew_info_new[mapoldnew_info_new['SubId']
+                                                 == down_sub_info['SubId'].values[0]].copy(deep=True)
             ndown_subid = down_sub_info_2['DowSubId'].values[0]
 
+            target_upstream_info = mapoldnew_info[mapoldnew_info['DowSubId'] == small_downsub_id].copy(
+                deep=True)
+            upstream_subid_tar = np.unique(
+                target_upstream_info['SubId'].values)
+
+            common_elements = np.intersect1d(
+                upstream_subid_tar, small_sub_non_lake['SubId'].values)
+
+            if len(common_elements) == 1:
+                update_river = True
+                modify = True
+            else:
+                upstream_subid_need_modify = target_upstream_info[target_upstream_info['SubId'].isin(
+                    common_elements)].sort_values('DrainArea', ascending=False)
+                if small_sub_id != upstream_subid_need_modify['SubId'].values[0]:
+                    update_river = False
+                else:
+                    update_river = True
+                modify = True
+
         else:
             modify = False
+            if small_downsub_id > 0:
+                print(
+                    small_sub_id,
+                    has_down_sub,
+                    down_sub_has_same_seg_id,
+                    small_sub_is_not_Lake,
+                    small_sub_is_not_gauge,
+                    has_down_sub,
+                    len(mapoldnew_info[mapoldnew_info['Seg_ID']
+                        == small_sub_seg_id])
+                )
             tarinfo = []
             continue
 
-        if  modify:
-            target_sub_is_head_water_sub =  len(mapoldnew_info[mapoldnew_info['DowSubId'] == tarinfo['SubId'].values[0]]) == 0
-            target_sub_has_less_one_up_stream = len(mapoldnew_info[ (mapoldnew_info['DowSubId'] == tarinfo['SubId'].values[0]) & (mapoldnew_info['Lake_Cat']  < 2)]) <= 1
-
+        if modify:
             mask1 = mapoldnew_info_new['SubId'] == small_sub_id
             mask3 = mapoldnew_info_new['nsubid'] == small_sub_id
-            mask2 = (mapoldnew_info_new["nsubid"] == tarinfo["nsubid"].values[0])  ###for subbasin already processed to drainage into this target catchment
+            # for subbasin already processed to drainage into this target catchment
+            mask2 = (mapoldnew_info_new["nsubid"]
+                     == tarinfo["nsubid"].values[0])
             masktemp = np.logical_or(mask1, mask2)
-            mask = np.logical_or(masktemp,mask3)
+            mask = np.logical_or(masktemp, mask3)
 
             if len(tarinfo) > 1 and len(np.unique(tarinfo['HyLakeId'].values)) > 1:
-                print(small_sub_id,small_sub_seg_id)
-                print(tarinfo[['SubId','DowSubId','Seg_ID','HyLakeId']])
-
-            # print("###################################a")
-            # print(small_sub_id)
-            # print(tarinfo["nsubid"].values[0])
-            # print(mapoldnew_info_new.loc[mask,"nsubid"].values)
-            # print(mapoldnew_info_new.loc[mask,"SubId"].values)
-            # print(mapoldnew_info_new.loc[mask,"DowSubId"].values)
-            # print(mapoldnew_info_new.loc[mask,"BasArea"].values)
-            # print(ndown_subid)
-            # print("###################################a")
+                print(small_sub_id, small_sub_seg_id)
+                print(tarinfo[['SubId', 'DowSubId', 'Seg_ID', 'HyLakeId']])
 
+            attributes = mapoldnew_info_new[mapoldnew_info_new['SubId'].isin(
+                [small_sub_id, down_sub_info['SubId'].values[0]])]
+            mapoldnew_info_new.loc[mask, 'BasArea'] = np.sum(
+                attributes["BasArea"].values)
+            mapoldnew_info_new.loc[mask, "BasSlope"] = np.average(
+                attributes["BasSlope"].values, weights=attributes["BasArea"].values
+            )
+            mapoldnew_info_new.loc[mask, "MeanElev"] = np.average(
+                attributes["MeanElev"].values, weights=attributes["BasArea"].values
+            )
+            mapoldnew_info_new.loc[mask, "BasAspect"] = np.average(
+                attributes["BasAspect"].values, weights=attributes["BasArea"].values
+            )
             for col in tarinfo.columns:
-                if col == "BasArea":
-
-                    mapoldnew_info_new.loc[mask, col] = np.sum(tarinfo["BasArea"].values[0] + mapoldnew_info_new.loc[mask1,"BasArea"].values[0])
+                if col == "RivLength" and update_river:
+                    mapoldnew_info_new.loc[mask, "RivLength"] = np.sum(
+                        attributes["RivLength"].values)
+                elif col in ["RivSlope", "FloodP_n", "Q_Mean", "Ch_n"] and update_river:
+                    mapoldnew_info_new.loc[mask, col] = np.average(
+                        attributes[col].values,
+                        weights=attributes[col].values,
+                    )
+                elif col in ["Max_DEM"] and update_river:
+                    mapoldnew_info_new.loc[mask, col] = np.max(
+                        attributes[col].values
+                    )
+                elif col in ["Min_DEM"] and update_river:
+                    mapoldnew_info_new.loc[mask, col] = np.min(
+                        attributes[col].values
+                    )
 
                 elif col == 'SubId':
 
-                    mapoldnew_info_new.loc[mask,"nsubid"] = tarinfo["nsubid"].values[0]
+                    mapoldnew_info_new.loc[mask,
+                                           "nsubid"] = tarinfo["nsubid"].values[0]
 
                 elif col == 'DowSubId':
-                    mapoldnew_info_new.loc[mask,col] = ndown_subid
+                    mapoldnew_info_new.loc[mask, col] = ndown_subid
                 elif (
                     col == "nsubid"
                     or col == "ndownsubid"
                     or col == "Old_SubId"
                     or col == "Old_DowSubId"
                     or col == "SHAPE"
                     or col == "geometry"
+                    or col == 'BasArea'
+                    or col == 'BasSlope'
+                    or col == 'MeanElev'
+                    or col == 'BasAspect'
                 ):
                     continue
                 else:
                     mapoldnew_info_new.loc[mask, col] = tarinfo[col].values[0]
 
-            if target_sub_is_head_water_sub or small_sub_is_head_water_sub:
-                if target_sub_has_less_one_up_stream:
-                    mapoldnew_info_new.loc[mask, "RivSlope"] = -1.2345
-                    mapoldnew_info_new.loc[mask, "RivLength"] = -1.2345
-                    mapoldnew_info_new.loc[mask, "FloodP_n"] = -1.2345
-                    mapoldnew_info_new.loc[mask, "Ch_n"] = -1.2345
-                    mapoldnew_info_new.loc[mask, "Min_DEM"] = -1.2345
-                    mapoldnew_info_new.loc[mask, "Max_DEM"] = -1.2345
-                    if "DA_Chn_L" in mapoldnew_info_new.columns:
-                        mapoldnew_info_new.loc[mask, "DA_Chn_L"] = -1.2345
-                        mapoldnew_info_new.loc[mask, "DA_Chn_Slp"] = -1.2345
-
-            # print("###################################b")
-            # print(small_sub_id)
-            # print(mapoldnew_info_new.loc[mask,"nsubid"].values)
-            # print(mapoldnew_info_new.loc[mask,"SubId"].values)
-            # print(mapoldnew_info_new.loc[mask,"DowSubId"].values)
-            # print(mapoldnew_info_new.loc[mask,"BasArea"].values)
-            # print("###################################b")
-
     return mapoldnew_info_new
 
 
 def New_SubId_To_Dissolve(
     subid,
     catchmentinfo,
     mapoldnew_info,
@@ -604,38 +666,42 @@
     seg_order=-1,
 ):
     sub_colnm = "SubId"
     routing_info = catchmentinfo[["SubId", "DowSubId"]].astype("int32").values
     if ismodifids < 0:
         Modify_subids1 = defcat(
             routing_info, subid
-        )  ### find all subids drainage to this subid
+        )  # find all subids drainage to this subid
         if upsubid > 0:
             Modify_subids2 = defcat(routing_info, upsubid)
             mask = np.in1d(Modify_subids1, Modify_subids2)
             Modify_subids = Modify_subids1[np.logical_not(mask)]
         else:
             Modify_subids = Modify_subids1
 
     else:
         Modify_subids = modifiidin
     #    print("##########################################")
     #    print(subid)
     #    print(Modify_subids)
-    cbranch = catchmentinfo[catchmentinfo[sub_colnm].isin(Modify_subids)].copy()
+    cbranch = catchmentinfo[catchmentinfo[sub_colnm].isin(
+        Modify_subids)].copy()
     tarinfo = catchmentinfo[
         catchmentinfo[sub_colnm] == subid
-    ].copy()  ### define these subs attributes
-    ### average river slope info
-    mainriv_merg_info = mainriv.loc[mainriv["SubId"].isin(Modify_subids)].copy()
-    mainriv_merg_info = mainriv_merg_info.loc[mainriv_merg_info["RivLength"] > 0].copy()
+    ].copy()  # define these subs attributes
+    # average river slope info
+    mainriv_merg_info = mainriv.loc[mainriv["SubId"].isin(
+        Modify_subids)].copy()
+    mainriv_merg_info = mainriv_merg_info.loc[mainriv_merg_info["RivLength"] > 0].copy(
+    )
     idx = tarinfo.index[0]
     #    print(tarinfo.loc[idx,'BasArea'],"1")
     if len(mainriv_merg_info) > 0:
-        tarinfo.loc[idx, "RivLength"] = np.sum(mainriv_merg_info["RivLength"].values)
+        tarinfo.loc[idx, "RivLength"] = np.sum(
+            mainriv_merg_info["RivLength"].values)
         tarinfo.loc[idx, "RivSlope"] = np.average(
             mainriv_merg_info["RivSlope"].values,
             weights=mainriv_merg_info["RivLength"].values,
         )
         tarinfo.loc[idx, "FloodP_n"] = np.average(
             mainriv_merg_info["FloodP_n"].values,
             weights=mainriv_merg_info["RivLength"].values,
@@ -644,19 +710,23 @@
             mainriv_merg_info["Q_Mean"].values,
             weights=mainriv_merg_info["RivLength"].values,
         )
         tarinfo.loc[idx, "Ch_n"] = np.average(
             mainriv_merg_info["Ch_n"].values,
             weights=mainriv_merg_info["RivLength"].values,
         )
-        tarinfo.loc[idx, "BkfWidth"] = np.max(mainriv_merg_info["BkfWidth"].values)
-        tarinfo.loc[idx, "BkfDepth"] = np.max(mainriv_merg_info["BkfDepth"].values)
-
-        tarinfo.loc[idx, "Max_DEM"] = np.max(mainriv_merg_info["Max_DEM"].values)
-        tarinfo.loc[idx, "Min_DEM"] = np.min(mainriv_merg_info["Min_DEM"].values)
+        tarinfo.loc[idx, "BkfWidth"] = np.max(
+            mainriv_merg_info["BkfWidth"].values)
+        tarinfo.loc[idx, "BkfDepth"] = np.max(
+            mainriv_merg_info["BkfDepth"].values)
+
+        tarinfo.loc[idx, "Max_DEM"] = np.max(
+            mainriv_merg_info["Max_DEM"].values)
+        tarinfo.loc[idx, "Min_DEM"] = np.min(
+            mainriv_merg_info["Min_DEM"].values)
 
     tarinfo.loc[idx, "BasArea"] = np.sum(cbranch["BasArea"].values)
     #    tarinfo.loc[idx,'NonLDArea']     = np.sum(cbranch['NonLDArea'].values)
     if len(cbranch) > 0:
         tarinfo.loc[idx, "BasSlope"] = np.average(
             cbranch["BasSlope"].values, weights=cbranch["BasArea"].values
         )
@@ -665,36 +735,37 @@
         )
         tarinfo.loc[idx, "BasAspect"] = np.average(
             cbranch["BasAspect"].values, weights=cbranch["BasArea"].values
         )
     #    print(tarinfo.loc[idx,'BasArea'],"2")
     if (
         Lake_Cat == 1
-    ):  ## Meger subbasin covered by lakes, Keep lake outlet catchment  DA, stream order info
+    ):  # Meger subbasin covered by lakes, Keep lake outlet catchment  DA, stream order info
         #        Longestpath = Calculate_Longest_flowpath(mainriv_merg_info)
-        tarinfo.loc[idx, "RivSlope"] = -1.2345  # Longestpath
-        tarinfo.loc[idx, "RivLength"] = -1.2345  # Longestpath
-        tarinfo.loc[idx, "FloodP_n"] = -1.2345  # Longestpath
-        tarinfo.loc[idx, "Ch_n"] = -1.2345  # Longestpath
-        tarinfo.loc[idx, "Min_DEM"] = -1.2345  # Longestpath
-        tarinfo.loc[idx, "Max_DEM"] = -1.2345  # Longestpath
-        if "DA_Chn_L" in tarinfo.columns:
-            tarinfo.loc[idx, "DA_Chn_L"] = -1.2345  # Longestpath
-            tarinfo.loc[idx, "DA_Chn_Slp"] = -1.2345  # Longestpath
+        # tarinfo.loc[idx, "RivSlope"] = -1.2345  # Longestpath
+        # tarinfo.loc[idx, "RivLength"] = -1.2345  # Longestpath
+        # tarinfo.loc[idx, "FloodP_n"] = -1.2345  # Longestpath
+        # tarinfo.loc[idx, "Ch_n"] = -1.2345  # Longestpath
+        # tarinfo.loc[idx, "Min_DEM"] = -1.2345  # Longestpath
+        # tarinfo.loc[idx, "Max_DEM"] = -1.2345  # Longestpath
+        # if "DA_Chn_L" in tarinfo.columns:
+        #     tarinfo.loc[idx, "DA_Chn_L"] = -1.2345  # Longestpath
+        #     tarinfo.loc[idx, "DA_Chn_Slp"] = -1.2345  # Longestpath
+        do_nothing = 1
 
     elif Lake_Cat == 2:
-        tarinfo.loc[idx, "RivSlope"] = -1.2345  # Longestpath
-        tarinfo.loc[idx, "RivLength"] = -1.2345  # Longestpath
-        tarinfo.loc[idx, "FloodP_n"] = -1.2345  # Longestpath
-        tarinfo.loc[idx, "Ch_n"] = -1.2345  # Longestpath
-        tarinfo.loc[idx, "Min_DEM"] = -1.2345  # Longestpath
-        tarinfo.loc[idx, "Max_DEM"] = -1.2345  # Longestpath
-        if "DA_Chn_L" in tarinfo.columns:
-            tarinfo.loc[idx, "DA_Chn_L"] = -1.2345  # Longestpath
-            tarinfo.loc[idx, "DA_Chn_Slp"] = -1.2345  # Longestpath
+        # tarinfo.loc[idx, "RivSlope"] = -1.2345  # Longestpath
+        # tarinfo.loc[idx, "RivLength"] = -1.2345  # Longestpath
+        # tarinfo.loc[idx, "FloodP_n"] = -1.2345  # Longestpath
+        # tarinfo.loc[idx, "Ch_n"] = -1.2345  # Longestpath
+        # tarinfo.loc[idx, "Min_DEM"] = -1.2345  # Longestpath
+        # tarinfo.loc[idx, "Max_DEM"] = -1.2345  # Longestpath
+        # if "DA_Chn_L" in tarinfo.columns:
+        #     tarinfo.loc[idx, "DA_Chn_L"] = -1.2345  # Longestpath
+        #     tarinfo.loc[idx, "DA_Chn_Slp"] = -1.2345  # Longestpath
         tarinfo.loc[idx, "Lake_Cat"] = 2
     elif Lake_Cat <= 0:
         #        tarinfo.loc[idx,'Strahler']      = -1.2345
         #        tarinfo.loc[idx,'Seg_ID']        = -1.2345
         #        tarinfo.loc[idx,'Seg_order']     = -1.2345
         #        tarinfo.loc[idx,'DA']            = -1.2345
         tarinfo.loc[idx, "HyLakeId"] = 0
@@ -708,21 +779,21 @@
     tarinfo.loc[idx, "centroid_y"] = -1.2345
 
     if seg_order > 0:
         tarinfo.loc[idx, "Seg_order"] = seg_order
 
     mask1 = mapoldnew_info["SubId"].isin(
         Modify_subids
-    )  ## catchment newly determined to be merged to target catchment
+    )  # catchment newly determined to be merged to target catchment
     mask2 = (
         mapoldnew_info["nsubid"] == subid
-    )  ###for subbasin already processed to drainage into this target catchment
+    )  # for subbasin already processed to drainage into this target catchment
     mask = np.logical_or(mask1, mask2)
 
-    ### the old downsub id of the dissolved polygon is stored in DowSubId
+    # the old downsub id of the dissolved polygon is stored in DowSubId
     for col in tarinfo.columns:
         if col == "SubId":
             #            print(tarinfo[col].values[0])
             mapoldnew_info.loc[mask, "nsubid"] = tarinfo[col].values[0]
         #            print(mapoldnew_info.loc[mask,'nsubid'])
         elif (
             col == "nsubid"
@@ -737,21 +808,21 @@
             mapoldnew_info.loc[mask, col] = tarinfo[col].values[0]
     #    print(mapoldnew_info.loc[mask1,['BasArea','nsubid','SubId']])
     #    print(mapoldnew_info.loc[mapoldnew_info['nsubid'] == subid,['BasArea','nsubid','SubId']])
     return mapoldnew_info
 
 
 def Evaluate_Two_Dataframes(Expected, Result, Check_Col_NM="SubId"):
-    ## check if two have the same column names
+    # check if two have the same column names
     if (Expected.columns != Result.columns).all():
         print(Expected.columns)
         print(Result.columns)
         return False
     neql = 0
-    ## check for each column two dataframe has the same value
+    # check for each column two dataframe has the same value
     for col in Expected.columns:
         if col == "HRU_ID":
             neql = neql + 1
             continue
         Array_expect = Expected[col].values
         Array_result = Result[col].values
         if (Array_expect != Array_result).all():
@@ -801,15 +872,16 @@
         mapoldnew_info["SubId"] = mapoldnew_info["nsubid"].values
 
         mapoldnew_info["DowSubId"] = mapoldnew_info["ndownsubid"].values
 
     if UpdateStreamorder < 0:
         return mapoldnew_info
 
-    mapoldnew_info_unique = mapoldnew_info.drop_duplicates("SubId", keep="first")
+    mapoldnew_info_unique = mapoldnew_info.drop_duplicates(
+        "SubId", keep="first")
 
     mapoldnew_info_unique = streamorderanddrainagearea(mapoldnew_info_unique)
 
     for i in range(0, len(mapoldnew_info_unique)):
         isubid = mapoldnew_info_unique["SubId"].values[i]
         mapoldnew_info.loc[
             mapoldnew_info["SubId"] == isubid, "Strahler"
@@ -822,22 +894,24 @@
         ] = mapoldnew_info_unique["Seg_order"].values[i]
         mapoldnew_info.loc[
             mapoldnew_info["SubId"] == isubid, "DrainArea"
         ] = mapoldnew_info_unique["DrainArea"].values[i]
 
     return mapoldnew_info
 
-def calculate_Tc(DrainArea,DA_Chn_L,DA_Chn_Slp):
+
+def calculate_Tc(DrainArea, DA_Chn_L, DA_Chn_Slp):
 
     TC_1 = 0.675*(DrainArea/1000/1000)**0.5
-    TC_2 = 0.2426 * ( DA_Chn_L/1000 )*( (DrainArea/1000/1000)**(-0.1) ) * ( DA_Chn_Slp**(-0.2) )
-    TC_3= 0.3 * ( (DA_Chn_L/1000)**0.76 ) * ( DA_Chn_Slp**(-0.19) )
-    TC_4 = (1/0.6)*2.8*( (DA_Chn_L/1000) / (DA_Chn_Slp**(0.5)) )**0.47
-    TC_5 = (1/0.6)*0.000326*( (DA_Chn_L) / (DA_Chn_Slp**(0.5)) )**0.79
-    return TC_1,TC_2,TC_3,TC_4,TC_5
+    TC_2 = 0.2426 * (DA_Chn_L/1000)*((DrainArea/1000/1000)
+                                     ** (-0.1)) * (DA_Chn_Slp**(-0.2))
+    TC_3 = 0.3 * ((DA_Chn_L/1000)**0.76) * (DA_Chn_Slp**(-0.19))
+    TC_4 = (1/0.6)*2.8*((DA_Chn_L/1000) / (DA_Chn_Slp**(0.5)))**0.47
+    TC_5 = (1/0.6)*0.000326*((DA_Chn_L) / (DA_Chn_Slp**(0.5)))**0.79
+    return TC_1, TC_2, TC_3, TC_4, TC_5
 
 
 def streamorderanddrainagearea(catinfoall):
     """Functions will  calcuate stream order and
         update drainage area in the attribute table catinfoall
     ----------
 
@@ -848,208 +922,217 @@
     -------
         catinfoall
     """
     Gauge_col_Name = "Has_POI"
     if "Has_POI" not in catinfoall.columns:
         Gauge_col_Name = "Has_Gauge"
 
-    catinfo = catinfoall.loc[catinfoall["Lake_Cat"] != 2].copy()  ### remove none connected lake catchments, which do not connected to the river system
+    # remove none connected lake catchments, which do not connected to the river system
+    catinfo = catinfoall.loc[catinfoall["Lake_Cat"] != 2].copy()
     catinfo_ncl = catinfoall.loc[catinfoall["Lake_Cat"] == 2].copy()
     routing_ncl = catinfo_ncl[["SubId", "DowSubId"]].astype("float").values
 
     catlist = np.full((len(catinfo)), -9)
     icat = 0
     iseg = 1
-    ### find first segments of all reaches, no upstream reaches
+    # find first segments of all reaches, no upstream reaches
     for i in range(0, len(catinfo)):
         idx = catinfo.index[i]
         if catinfo["SubId"].values[i] == catinfo["DowSubId"].values[i]:
             catinfo.loc[idx, "DowSubId"] = -1
         catid = catinfo["SubId"].values[i]
-        if (len(catinfo[catinfo["DowSubId"] == catid]) == 0):  ### the river seg has no upstream segment
-            catlist[icat] = int(catinfo["DowSubId"].values[i])  #### store next reach segment
+        # the river seg has no upstream segment
+        if (len(catinfo[catinfo["DowSubId"] == catid]) == 0):
+            # store next reach segment
+            catlist[icat] = int(catinfo["DowSubId"].values[i])
 
-            #### calculate DA of head watershed include None connected lakes
+            # calculate DA of head watershed include None connected lakes
             if len(routing_ncl) == 0:
                 DA_ncl = 0.0
                 slp_ncl = 0.0
             else:
-                Upstreamcats = defcat(routing_ncl, catid)  ### alll subuds
+                Upstreamcats = defcat(routing_ncl, catid)  # alll subuds
                 Up_cat_info = catinfo_ncl.loc[
                     catinfo_ncl["SubId"].isin(Upstreamcats)
                 ].copy()
 
                 if len(Up_cat_info) > 0:
                     DA_ncl = sum(Up_cat_info["BasArea"].values)
-                    slp_ncl = np.average(Up_cat_info["BasSlope"].values,weights = Up_cat_info["BasArea"].values)
+                    slp_ncl = np.average(
+                        Up_cat_info["BasSlope"].values, weights=Up_cat_info["BasArea"].values)
                 else:
                     DA_ncl = 0.0
                     slp_ncl = 0.0
 
-            catinfo.loc[idx, "DrainArea"] = DA_ncl + catinfo["BasArea"].values[i]
+            catinfo.loc[idx, "DrainArea"] = DA_ncl + \
+                catinfo["BasArea"].values[i]
             catinfo.loc[idx, "Strahler"] = 1
             catinfo.loc[idx, "Seg_order"] = 1
             catinfo.loc[idx, "Seg_ID"] = iseg
-            #head watershed
-            if "DA_Chn_L" in catinfo.columns:
-                catinfo.loc[idx, "DA_Chn_L"] = -1.2345
-                catinfo.loc[idx, "DA_Chn_Slp"] = -1.2345
-            catinfo.loc[idx, "RivLength"] = -1.2345
-            catinfo.loc[idx, "RivSlope"] = -1.2345
-            catinfo.loc[idx, "Min_DEM"] = -1.2345
-            catinfo.loc[idx, "FloodP_n"] = -1.2345
-            catinfo.loc[idx, "Ch_n"] = -1.2345
-            catinfo.loc[idx, "Max_DEM"] = -1.2345
-            catinfo.loc[idx, "DA_Slope"] = (catinfo["BasSlope"].values[i]*catinfo["BasArea"].values[i]+DA_ncl*slp_ncl)/catinfo.loc[idx, "DrainArea"]
+            # head watershed
+            # if "DA_Chn_L" in catinfo.columns:
+            #     catinfo.loc[idx, "DA_Chn_L"] = -1.2345
+            #     catinfo.loc[idx, "DA_Chn_Slp"] = -1.2345
+            # catinfo.loc[idx, "RivLength"] = -1.2345
+            # catinfo.loc[idx, "RivSlope"] = -1.2345
+            # catinfo.loc[idx, "Min_DEM"] = -1.2345
+            # catinfo.loc[idx, "FloodP_n"] = -1.2345
+            # catinfo.loc[idx, "Ch_n"] = -1.2345
+            # catinfo.loc[idx, "Max_DEM"] = -1.2345
+            catinfo.loc[idx, "DA_Slope"] = (
+                catinfo["BasSlope"].values[i]*catinfo["BasArea"].values[i]+DA_ncl*slp_ncl)/catinfo.loc[idx, "DrainArea"]
 
             # TC_1,TC_2,TC_3,TC_4,TC_5 = calculate_Tc(catinfo.loc[idx, "DrainArea"],catinfo.loc[idx, "DA_Chn_L"],catinfo.loc[idx, "DA_Chn_Slp"])
             #
             # catinfo.loc[idx, "Tc_1"] = TC_1
             # catinfo.loc[idx, "Tc_2"] = TC_2
             # catinfo.loc[idx, "Tc_3"] = TC_3
             # catinfo.loc[idx, "Tc_4"] = TC_4
             # catinfo.loc[idx, "Tc_5"] = TC_5
 
-
             icat = icat + 1
             iseg = iseg + 1
 
     catlist = np.unique(catlist)
     catlist = catlist[catlist > 0]
     #    print(catlist)
-    ### Loop for each first reach, until go to reach intersection
+    # Loop for each first reach, until go to reach intersection
     newcatlist = np.full((len(catinfo)), -9)
     inewstart = 0
 
     for i in range(0, len(catlist)):
         catid = catlist[i]
         F_intersect = 1
         #        print("new start            ",i,catid)
         while F_intersect == 1 and catid > 0:
             Up_Reaches_info = catinfo.loc[catinfo["DowSubId"] == catid].copy()
             cur_Reach_info = catinfo.loc[catinfo["SubId"] == catid].copy()
             curcat_idx = catinfo["SubId"] == catid
 
-            #### calculate DA of None connected lakes
+            # calculate DA of None connected lakes
             if len(routing_ncl) == 0:
                 DA_ncl = 0.0
                 slp_ncl = 0.0
             else:
                 #                print("aaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaa")
                 #                print(catid)
                 #                print(routing_ncl)
-                Upstreamcats = defcat(routing_ncl, catid)  ### alll subuds
+                Upstreamcats = defcat(routing_ncl, catid)  # alll subuds
                 Up_cat_info = catinfo_ncl.loc[
                     catinfo_ncl["SubId"].isin(Upstreamcats)
                 ].copy()
                 if len(Up_cat_info) > 0:
                     DA_ncl = sum(Up_cat_info["BasArea"].values)
-                    slp_ncl =  np.average(Up_cat_info["BasSlope"].values,weights = Up_cat_info["BasArea"].values)
+                    slp_ncl = np.average(
+                        Up_cat_info["BasSlope"].values, weights=Up_cat_info["BasArea"].values)
                 else:
                     DA_ncl = 0.0
                     slp_ncl = 0.0
 
             if (
                 len(cur_Reach_info) <= 0
-            ):  ### reach the most downstream of the watersheds
+            ):  # reach the most downstream of the watersheds
                 break
 
-            if len(Up_Reaches_info) == 1:  ### only have one upstream
+            if len(Up_Reaches_info) == 1:  # only have one upstream
                 catinfo.loc[curcat_idx, "DrainArea"] = (
                     cur_Reach_info["BasArea"].values[0]
                     + Up_Reaches_info["DrainArea"].values[0]
                     + DA_ncl
                 )
                 catinfo.loc[curcat_idx, "Strahler"] = Up_Reaches_info[
                     "Strahler"
                 ].values[0]
                 catinfo.loc[curcat_idx, "Seg_order"] = (
                     Up_Reaches_info["Seg_order"].values[0] + 1
                 )
 
-
-                catinfo.loc[curcat_idx, "Seg_ID"] = Up_Reaches_info["Seg_ID"].values[0]
+                catinfo.loc[curcat_idx,
+                            "Seg_ID"] = Up_Reaches_info["Seg_ID"].values[0]
 
                 if "DA_Chn_L" in catinfo.columns:
-                    catinfo.loc[curcat_idx, "DA_Chn_L"] = np.maximum(Up_Reaches_info["DA_Chn_L"].values[0],0) + cur_Reach_info["RivLength"].values[0]
+                    catinfo.loc[curcat_idx, "DA_Chn_L"] = np.maximum(
+                        Up_Reaches_info["DA_Chn_L"].values[0], 0) + cur_Reach_info["RivLength"].values[0]
 
-                    catinfo.loc[curcat_idx, "DA_Chn_Slp"] = ( cur_Reach_info["RivSlope"].values[0]  * np.maximum(cur_Reach_info["RivLength"].values[0],0)
-                                                           +  Up_Reaches_info["DA_Chn_L"].values[0] * np.maximum(Up_Reaches_info["DA_Chn_Slp"].values[0],0)
+                    catinfo.loc[curcat_idx, "DA_Chn_Slp"] = (cur_Reach_info["RivSlope"].values[0] * np.maximum(cur_Reach_info["RivLength"].values[0], 0)
+                                                             + Up_Reaches_info["DA_Chn_L"].values[0] * np.maximum(
+                                                                 Up_Reaches_info["DA_Chn_Slp"].values[0], 0)
                                                              ) / catinfo.loc[curcat_idx, "DA_Chn_L"]
 
                     catinfo.loc[curcat_idx, "DA_Slope"] = (cur_Reach_info["BasSlope"].values[0]*cur_Reach_info["BasArea"].values[0]
                                                            + DA_ncl * slp_ncl
                                                            + Up_Reaches_info["DA_Slope"].values[0] * Up_Reaches_info["DrainArea"].values[0]
                                                            )/catinfo.loc[curcat_idx, "DrainArea"]
 
-
                 # TC_1,TC_2,TC_3,TC_4,TC_5 = calculate_Tc(catinfo.loc[curcat_idx, "DrainArea"],catinfo.loc[curcat_idx, "DA_Chn_L"],catinfo.loc[curcat_idx, "DA_Chn_Slp"])
                 #
                 # catinfo.loc[curcat_idx, "Tc_1"] = TC_1
                 # catinfo.loc[curcat_idx, "Tc_2"] = TC_2
                 # catinfo.loc[curcat_idx, "Tc_3"] = TC_3
                 # catinfo.loc[curcat_idx, "Tc_4"] = TC_4
                 # catinfo.loc[curcat_idx, "Tc_5"] = TC_5
 
-
                 #                print('1',catid,catinfo.loc[curcat_idx,'DA'].values,catinfo.loc[curcat_idx,'Strahler'].values,catinfo.loc[curcat_idx,'Sub_order'].values)
                 catid = int(cur_Reach_info["DowSubId"].values[0])
-            else:  ### has mutiple upstram
-                if (np.min(Up_Reaches_info["Strahler"].values) > 0):  ### all upstream has been processed
+            else:  # has mutiple upstram
+                # all upstream has been processed
+                if (np.min(Up_Reaches_info["Strahler"].values) > 0):
 
                     if 'DA_Chn_L' in Up_Reaches_info.columns:
-                        Up_Reaches_info = Up_Reaches_info.sort_values(by='DA_Chn_L', ascending=False)
+                        Up_Reaches_info = Up_Reaches_info.sort_values(
+                            by='DA_Chn_L', ascending=False)
 
                     catinfo.loc[curcat_idx, "DrainArea"] = (
                         cur_Reach_info["BasArea"].values[0]
                         + np.sum(Up_Reaches_info["DrainArea"].values)
                         + DA_ncl
                     )
 
                     if "DA_Chn_L" in catinfo.columns:
-                        catinfo.loc[curcat_idx, "DA_Chn_L"] = np.maximum(Up_Reaches_info["DA_Chn_L"].values[0],0) + cur_Reach_info["RivLength"].values[0]
-
-                        catinfo.loc[curcat_idx, "DA_Chn_Slp"] = ( cur_Reach_info["RivSlope"].values[0]  * np.maximum(cur_Reach_info["RivLength"].values[0],0)
-                                                               +  Up_Reaches_info["DA_Chn_L"].values[0] * np.maximum(Up_Reaches_info["DA_Chn_Slp"].values[0],0)
-                                                                 ) /catinfo.loc[curcat_idx, "DA_Chn_L"]
+                        catinfo.loc[curcat_idx, "DA_Chn_L"] = np.maximum(
+                            Up_Reaches_info["DA_Chn_L"].values[0], 0) + cur_Reach_info["RivLength"].values[0]
 
+                        catinfo.loc[curcat_idx, "DA_Chn_Slp"] = (cur_Reach_info["RivSlope"].values[0] * np.maximum(cur_Reach_info["RivLength"].values[0], 0)
+                                                                 + Up_Reaches_info["DA_Chn_L"].values[0] * np.maximum(
+                                                                     Up_Reaches_info["DA_Chn_Slp"].values[0], 0)
+                                                                 ) / catinfo.loc[curcat_idx, "DA_Chn_L"]
 
                         catinfo.loc[curcat_idx, "DA_Slope"] = (cur_Reach_info["BasSlope"].values[0]*cur_Reach_info["BasArea"].values[0]
                                                                + DA_ncl * slp_ncl
                                                                + Up_Reaches_info["DA_Slope"].values[0] * Up_Reaches_info["DrainArea"].values[0]
                                                                )/catinfo.loc[curcat_idx, "DrainArea"]
 
-
                     # TC_1,TC_2,TC_3,TC_4,TC_5 = calculate_Tc(catinfo.loc[curcat_idx, "DrainArea"],catinfo.loc[curcat_idx, "DA_Chn_L"],catinfo.loc[curcat_idx, "DA_Chn_Slp"])
                     #
                     # catinfo.loc[curcat_idx, "Tc_1"] = TC_1
                     # catinfo.loc[curcat_idx, "Tc_2"] = TC_2
                     # catinfo.loc[curcat_idx, "Tc_3"] = TC_3
                     # catinfo.loc[curcat_idx, "Tc_4"] = TC_4
                     # catinfo.loc[curcat_idx, "Tc_5"] = TC_5
 
                     if np.min(Up_Reaches_info["Strahler"].values) == np.max(
                         Up_Reaches_info["Strahler"].values
-                    ):  ### two reach has the same order
+                    ):  # two reach has the same order
                         catinfo.loc[curcat_idx, "Strahler"] = (
                             Up_Reaches_info["Strahler"].values[0] + 1
                         )
                         catinfo.loc[curcat_idx, "Seg_order"] = 1
                         catinfo.loc[curcat_idx, "Seg_ID"] = iseg + 1
                         iseg = iseg + 1
                     #                        print('2',catid,catinfo.loc[catinfo['SubId'] == catid,'DA'].values,catinfo.loc[catinfo['SubId'] == catid,'Strahler'].values,catinfo.loc[catinfo['SubId'] == catid,'Sub_order'].values)
                     else:
-                        max_straorder = np.max(Up_Reaches_info["Strahler"].values)
+                        max_straorder = np.max(
+                            Up_Reaches_info["Strahler"].values)
                         catinfo.loc[curcat_idx, "Strahler"] = max_straorder
                         catinfo.loc[curcat_idx, "Seg_order"] = 1
                         catinfo.loc[curcat_idx, "Seg_ID"] = iseg + 1
                         iseg = iseg + 1
                     #                        print('3',catid,catinfo.loc[catinfo['SubId'] == catid,'DA'].values,catinfo.loc[catinfo['SubId'] == catid,'Strahler'].values,catinfo.loc[catinfo['SubId'] == catid,'Sub_order'].values)
                     catid = int(cur_Reach_info["DowSubId"].values[0])
-                else:  ## there are some reach has not been processed, save id to the list and wait for another loob
+                else:  # there are some reach has not been processed, save id to the list and wait for another loob
                     newcatlist[inewstart] = int(catid)
                     inewstart = inewstart + 1
                     F_intersect = 0
 
     mask = catinfoall["SubId"].isin(catinfo["SubId"].values)
     catinfoall.loc[mask, "Seg_ID"] = catinfo["Seg_ID"].values
     catinfoall.loc[mask, "Seg_order"] = catinfo["Seg_order"].values
@@ -1065,15 +1148,15 @@
 
     # catinfoall.loc[mask, "Tc_1"] = catinfo["Tc_1"].values
     # catinfoall.loc[mask, "Tc_2"] = catinfo["Tc_2"].values
     # catinfoall.loc[mask, "Tc_3"] = catinfo["Tc_3"].values
     # catinfoall.loc[mask, "Tc_4"] = catinfo["Tc_4"].values
     # catinfoall.loc[mask, "Tc_5"] = catinfo["Tc_5"].values
 
-    ### calcuate channel manning's coefficient
+    # calcuate channel manning's coefficient
     for i in range(0, len(catinfoall)):
         idx = catinfoall.index[i]
         # if catinfo['BkfWidth'].values[i] > 0 and catinfo['RivSlope'].values[i] > 0 :
         #     catinfo.loc[idx,'Ch_n'] = calculateChannaln(catinfo['BkfWidth'].values[i],catinfo['BkfDepth'].values[i],
         #                       catinfo['Q_Mean'].values[i],catinfo['RivSlope'].values[i])
         if catinfoall[Gauge_col_Name].values[i] > 0:
             if catinfoall["DA_Obs"].values[i] > 0:
@@ -1082,43 +1165,43 @@
                 ) / catinfoall["DA_Obs"].values[i]
 
         # calcuate drainage area of each non connected lake
 
         if catinfoall["Lake_Cat"].values[i] == 2:
             catid = catinfoall["SubId"].values[i]
 
-            Upstreamcats = defcat(routing_ncl, catid)  ### ncl subs to this ncl sub
-            Up_cat_info = catinfo_ncl.loc[catinfo_ncl["SubId"].isin(Upstreamcats)].copy(deep=True)
+            # ncl subs to this ncl sub
+            Upstreamcats = defcat(routing_ncl, catid)
+            Up_cat_info = catinfo_ncl.loc[catinfo_ncl["SubId"].isin(
+                Upstreamcats)].copy(deep=True)
             DA = sum(Up_cat_info["BasArea"].values)
             catinfoall.loc[idx, "DrainArea"] = DA
 
-            catinfoall.loc[idx, "DA_Slope"] = np.average(Up_cat_info["BasSlope"].values,weights = Up_cat_info["BasArea"].values)
-
-
-            catinfoall.loc[idx, "RivLength"] = -1.2345
-            catinfoall.loc[idx, "RivSlope"] = -1.2345
-            catinfoall.loc[idx, "Min_DEM"] = -1.2345
-            catinfoall.loc[idx, "Max_DEM"] = -1.2345
-            catinfoall.loc[idx, "FloodP_n"] = -1.2345
-            catinfoall.loc[idx, "Ch_n"] = -1.2345
-
-            if "DA_Chn_L" in catinfoall.columns:
-                catinfoall.loc[idx, "DA_Chn_Slp"] = -1.2345
-                catinfoall.loc[idx, "DA_Chn_L"] = -1.2345
+            catinfoall.loc[idx, "DA_Slope"] = np.average(
+                Up_cat_info["BasSlope"].values, weights=Up_cat_info["BasArea"].values)
 
+            # catinfoall.loc[idx, "RivLength"] = -1.2345
+            # catinfoall.loc[idx, "RivSlope"] = -1.2345
+            # catinfoall.loc[idx, "Min_DEM"] = -1.2345
+            # catinfoall.loc[idx, "Max_DEM"] = -1.2345
+            # catinfoall.loc[idx, "FloodP_n"] = -1.2345
+            # catinfoall.loc[idx, "Ch_n"] = -1.2345
+
+            # if "DA_Chn_L" in catinfoall.columns:
+            #     catinfoall.loc[idx, "DA_Chn_Slp"] = -1.2345
+            #     catinfoall.loc[idx, "DA_Chn_L"] = -1.2345
 
             # TC_1,TC_2,TC_3,TC_4,TC_5 = calculate_Tc(catinfoall.loc[idx, "DrainArea"],catinfoall.loc[idx, "DA_Chn_L"],catinfoall.loc[idx, "DA_Chn_Slp"])
             #
             # catinfoall.loc[idx, "Tc_1"] = TC_1
             # catinfoall.loc[idx, "Tc_2"] = TC_2
             # catinfoall.loc[idx, "Tc_3"] = TC_3
             # catinfoall.loc[idx, "Tc_4"] = TC_4
             # catinfoall.loc[idx, "Tc_5"] = TC_5
 
-
     return catinfoall
 
 
 def defcat(out, outletid):
     """Functions will return upstream ids in out taht drainage
         to outletid
     ----------
@@ -1144,15 +1227,15 @@
             Shedid[psid] = otsheds[i]
             #            print(Shedid[psid],otsheds[i])
             #            print("##################################################b")
             psid = psid + 1
             irow = np.argwhere(rout[:, 1] == otsheds[i]).astype(int)
             #            print(len(irow))
             for j in range(0, len(irow)):
-                #### if the catchment id already processed skip
+                # if the catchment id already processed skip
                 if rout[irow[j], 0] in Shedid:
                     continue
                 noutshd[poshdid] = rout[irow[j], 0]
                 poshdid = poshdid + 1
         noutshd = np.unique(noutshd)
         otsheds = noutshd[noutshd >= 0]
     Shedid = np.unique(Shedid)
@@ -1187,80 +1270,84 @@
             An new columns indicate the outlet subbasin id of the sub region
             will be added
         AllCatinfo           : dataframe
             Downstream subbasin ID of each subregion's outlet subbasin will
             be updated.
     """
 
-    ### update downsteam subbasin id for each subregion outlet subbasins
-    ### current value is -1, updated to connected downstream subbasin ID
-    ###loop for each subregion
+    # update downsteam subbasin id for each subregion outlet subbasins
+    # current value is -1, updated to connected downstream subbasin ID
+    # loop for each subregion
     routing_info = (
-        Sub_Region_info[["Sub_Reg_ID", "Dow_Sub_Reg_Id"]].astype("float").values
+        Sub_Region_info[["Sub_Reg_ID", "Dow_Sub_Reg_Id"]].astype(
+            "float").values
     )
     for i in range(0, len(Sub_Region_info)):
 
-        ### obtain all subbasin data for i isubregion
+        # obtain all subbasin data for i isubregion
         isubregion = Sub_Region_info["Sub_Reg_ID"].values[i]
         # get link id for corresponding down stream sub region inlet point
         ILpt_ID = Sub_Region_info["ILpt_ID"].values[i]
 
         Sub_Region_cat_info = AllCatinfo.loc[
             AllCatinfo["Region_ID"] == isubregion
         ].copy()
 
         Sub_Region_info.loc[
             Sub_Region_info["Sub_Reg_ID"] == isubregion, "N_Up_SubRegion"
         ] = len(defcat(routing_info, isubregion))
 
-        ### check if this subregion exist in merged data
+        # check if this subregion exist in merged data
         if len(Sub_Region_cat_info) <= 0:
             continue
 
-        ### Subregion outlet subbasin ID
+        # Subregion outlet subbasin ID
         outlet_mask = Sub_Region_cat_info["DowSubId"] == -1
-        iReg_Outlet_Subid = Sub_Region_cat_info.loc[outlet_mask, "SubId"].values[0]
+        iReg_Outlet_Subid = Sub_Region_cat_info.loc[outlet_mask,
+                                                    "SubId"].values[0]
         # (isubregion - 80000) * 200000 - 1
         Sub_Region_info.loc[
             Sub_Region_info["Sub_Reg_ID"] == isubregion, "Outlet_SubId"
         ] = iReg_Outlet_Subid
-        ### find downstream subregion id of current subregion
+        # find downstream subregion id of current subregion
         Dow_Sub_Region_id = Sub_Region_info["Dow_Sub_Reg_Id"].values[i]
 
-        ### if this region has no down subregions. do not need to
-        ### modify the dowsubid of the outlet subbasin of this subregion
+        # if this region has no down subregions. do not need to
+        # modify the dowsubid of the outlet subbasin of this subregion
         if Dow_Sub_Region_id < 0:
             continue
 
-        ### find downstrem subbasin id of outlet subbasin
-        Down_Sub_info = DownCatinfo.loc[DownCatinfo["ILpt_ID"] == ILpt_ID].copy()
+        # find downstrem subbasin id of outlet subbasin
+        Down_Sub_info = DownCatinfo.loc[DownCatinfo["ILpt_ID"] == ILpt_ID].copy(
+        )
 
-        if len(Down_Sub_info) == 1 and Dow_Sub_Region_id != 79999:  ###
+        if len(Down_Sub_info) == 1 and Dow_Sub_Region_id != 79999:
             DownSubid = Down_Sub_info["SubId"].values[0]
             AllCatinfo.loc[
                 AllCatinfo["SubId"] == iReg_Outlet_Subid, "DowSubId"
             ] = DownSubid
-        ### two subregion drainage to the same downstream subregion,
-        ### the Down_Sub_info only contains one upper subregion
-        ### the rest do not exist in Down_Sub_info
+        # two subregion drainage to the same downstream subregion,
+        # the Down_Sub_info only contains one upper subregion
+        # the rest do not exist in Down_Sub_info
         elif Dow_Sub_Region_id == 79999:
-            AllCatinfo.loc[AllCatinfo["SubId"] == iReg_Outlet_Subid, "DowSubId"] = -1
+            AllCatinfo.loc[AllCatinfo["SubId"] ==
+                           iReg_Outlet_Subid, "DowSubId"] = -1
         else:
             print("##################################################")
             print("Subregion : ", isubregion, "   To  ", Dow_Sub_Region_id)
-            print(Dow_Sub_Region_id,ILpt_ID)
+            print(Dow_Sub_Region_id, ILpt_ID)
             print(Down_Sub_info)
             print(iReg_Outlet_Subid)
-            print(DownCatinfo[["ILpt_ID","SubId"]])
+            print(DownCatinfo[["ILpt_ID", "SubId"]])
             print("Need be manually connected")
             print("##################################################")
     return AllCatinfo, Sub_Region_info
 
 
-def Update_DA_Strahler_For_Combined_Result(AllCatinfo, Sub_Region_info,k,c):
+def Update_DA_Strahler_For_Combined_Result(AllCatinfo, Sub_Region_info, k, c):
     """Update Drainage area, strahler order of subbains
 
     Update drainage area and strahler order for combined routing product
     of each subregions
     Parameters
     ----------
     AllCatinfo                        : dataframe
@@ -1277,15 +1364,15 @@
 
     Returns:
     -------
     AllCatinfo           : dataframe
         Downstream DA and strahler order of each subregion along the flow
         pathway between subregions will be updated.
     """
-    ### start from head subregions with no upstream subregion
+    # start from head subregions with no upstream subregion
     Subregion_list = Sub_Region_info[Sub_Region_info["N_Up_SubRegion"] == 1][
         "Sub_Reg_ID"
     ].values
     Subregion_list = np.unique(Subregion_list)
     Subregion_list = Subregion_list.tolist()
 
     # loop until Subregion_list has no subregions
@@ -1296,32 +1383,35 @@
         print(AllCatinfo.loc[AllCatinfo["DowSubId"] == -1])
         return AllCatinfo
     elif len(AllCatinfo.loc[AllCatinfo["DowSubId"] == -1]) == 0:
         print("Watershed has no outlet")
         return AllCatinfo
     else:
         Watershedoutletsubid = (
-            AllCatinfo.loc[AllCatinfo["DowSubId"] == -1]["SubId"].values[0].astype(int)
+            AllCatinfo.loc[AllCatinfo["DowSubId"]
+                           == -1]["SubId"].values[0].astype(int)
         )
 
-    ### Area and DA check
+    # Area and DA check
     Total_DA_Subregion = 0.0
     for i in range(0, len(Sub_Region_info)):
         Outletsubid_csubr = Sub_Region_info["Outlet_SubId"].values[i]
         Total_DA_Subregion = (
             Total_DA_Subregion
-            + AllCatinfo.loc[AllCatinfo["SubId"] == Outletsubid_csubr]["DrainArea"].values[0]
+            + AllCatinfo.loc[AllCatinfo["SubId"] ==
+                             Outletsubid_csubr]["DrainArea"].values[0]
         )
         print(
             "######Area and DA check for subregion ",
             Sub_Region_info["Sub_Reg_ID"].values[i],
         )
         print(
             "DA at the subregion outlet is    ",
-            AllCatinfo.loc[AllCatinfo["SubId"] == Outletsubid_csubr]["DrainArea"].values[0],
+            AllCatinfo.loc[AllCatinfo["SubId"] ==
+                           Outletsubid_csubr]["DrainArea"].values[0],
         )
         print(
             "Total subregion area is          ",
             sum(
                 AllCatinfo.loc[
                     AllCatinfo["Region_ID"] == Sub_Region_info["Sub_Reg_ID"].values[i]
                 ]["BasArea"].values
@@ -1330,40 +1420,40 @@
 
     iloop = 1
     while len(Subregion_list) > 0:
         print("loop  ", iloop)
         print(Subregion_list)
         current_loop_list = copy.copy(Subregion_list)
         Subregion_list = []
-        ### loop for current subregion list
+        # loop for current subregion list
         for i in range(0, len(current_loop_list)):
-            ### current subregion id
+            # current subregion id
             c_subr_id = current_loop_list[i]
-            ### down subregion id of current subregion
+            # down subregion id of current subregion
             if c_subr_id == 79999:
                 continue
 
             d_subr_id = Sub_Region_info[Sub_Region_info["Sub_Reg_ID"] == c_subr_id][
                 "Dow_Sub_Reg_Id"
             ].values[0]
-            ### add down subregon id to the list for next while loop
+            # add down subregon id to the list for next while loop
             Subregion_list.append(d_subr_id)
 
-            ### obtain outlet subid of this region
+            # obtain outlet subid of this region
             Outletsubid_csubr = Sub_Region_info[
                 Sub_Region_info["Sub_Reg_ID"] == c_subr_id
             ]["Outlet_SubId"].values[0]
-            ### obtain outlet sub info
+            # obtain outlet sub info
             Outletsub_info = AllCatinfo.loc[
                 AllCatinfo["SubId"] == Outletsubid_csubr
             ].copy()
-            ### obtain down subid of the outlet subbasin
+            # obtain down subid of the outlet subbasin
             downsubid = Outletsub_info["DowSubId"].values[0]
 
-            ### downsubid did not exist.....
+            # downsubid did not exist.....
             if len(AllCatinfo.loc[AllCatinfo["SubId"] == downsubid]) <= 0:
                 if int(c_subr_id) != int(Watershedoutletsubid):
                     print("Subregion:   ", c_subr_id)
                     print(
                         "SubId is ",
                         Outletsubid_csubr,
                         " DownSubId is  ",
@@ -1373,57 +1463,67 @@
                     )
                 continue
 
             downsub_reg_id = AllCatinfo.loc[AllCatinfo["SubId"] == downsubid][
                 "Region_ID"
             ].values[0]
 
-            print("Subregion:   ", c_subr_id,downsub_reg_id,d_subr_id,downsubid)
+            print("Subregion:   ", c_subr_id,
+                  downsub_reg_id, d_subr_id, downsubid)
 
             if downsub_reg_id != d_subr_id:
                 print(
                     "Subregion:   ",
                     c_subr_id,
                     "  did not connected with    ",
                     d_subr_id,
                 )
                 continue
 
             while downsub_reg_id == d_subr_id:
-                csubid = downsubid  ### update DA and Strahler for this subbasin
-                print("Subregion:   ", c_subr_id,downsub_reg_id,d_subr_id,downsubid,csubid)
-                ### current subid info
-                C_sub_info = AllCatinfo.loc[AllCatinfo["SubId"] == csubid].copy()
-                ### find all subbasin drainge to this csubid
-                Upper_sub_info = AllCatinfo.loc[AllCatinfo["DowSubId"] == csubid].copy()
+                csubid = downsubid  # update DA and Strahler for this subbasin
+                print("Subregion:   ", c_subr_id, downsub_reg_id,
+                      d_subr_id, downsubid, csubid)
+                # current subid info
+                C_sub_info = AllCatinfo.loc[AllCatinfo["SubId"] == csubid].copy(
+                )
+                # find all subbasin drainge to this csubid
+                Upper_sub_info = AllCatinfo.loc[AllCatinfo["DowSubId"] == csubid].copy(
+                )
 
-                ### ## new DA = basin area + DA of upper subregions
+                # new DA = basin area + DA of upper subregions
 
                 NewDA = C_sub_info["BasArea"].values[0] + sum(
                     Upper_sub_info["DrainArea"].values
                 )
 
-                ### calculate new Strahler orders
-                ## up stream Strahler orders
+                # calculate new Strahler orders
+                # up stream Strahler orders
                 Strahlers = Upper_sub_info["Strahler"].values
                 maxStrahler = max(Strahlers)
                 if np.sum(Strahlers == maxStrahler) >= 2:
                     newStrahler = maxStrahler + 1
                 else:
                     newStrahler = maxStrahler
-                #### updateAllCatinfo
-                AllCatinfo.loc[AllCatinfo["SubId"] == csubid, "Strahler"] = newStrahler
-                AllCatinfo.loc[AllCatinfo["SubId"] == csubid, "DrainArea"] = NewDA
+                # updateAllCatinfo
+                AllCatinfo.loc[AllCatinfo["SubId"] ==
+                               csubid, "Strahler"] = newStrahler
+                AllCatinfo.loc[AllCatinfo["SubId"]
+                               == csubid, "DrainArea"] = NewDA
 
                 if AllCatinfo[AllCatinfo["SubId"] == csubid]["DA_Obs"].values[0] > 0:
-                    da_obs = AllCatinfo[AllCatinfo["SubId"] == csubid]["DA_Obs"].values[0]
-                    da_sim = AllCatinfo[AllCatinfo["SubId"] == csubid]["DrainArea"].values[0]/1000.0/1000.0
+                    da_obs = AllCatinfo[AllCatinfo["SubId"]
+                                        == csubid]["DA_Obs"].values[0]
+                    da_sim = AllCatinfo[AllCatinfo["SubId"] ==
+                                        csubid]["DrainArea"].values[0]/1000.0/1000.0
                     if da_obs > 0:
-                        AllCatinfo.loc[AllCatinfo["SubId"] == csubid, "DA_error"] = da_sim/da_obs
-                        AllCatinfo.loc[AllCatinfo["SubId"] == csubid, "Use_region"] = 1
+                        AllCatinfo.loc[AllCatinfo["SubId"] ==
+                                       csubid, "DA_error"] = da_sim/da_obs
+                        AllCatinfo.loc[AllCatinfo["SubId"]
+                                       == csubid, "Use_region"] = 1
 
                 # da = AllCatinfo.loc[AllCatinfo["SubId"] == csubid, "DrainArea"].values[0] / 1000 / 1000  # m2 to km2
                 # q = func_Q_DA(da, k, c)
                 # bk_w= 7.2 * q ** 0.5
                 # bk_d = 0.27 * q ** 0.3
                 # bk_q = q
                 # bk_slope = AllCatinfo.loc[AllCatinfo["SubId"] == csubid, "RivSlope"].values[0]
@@ -1433,20 +1533,18 @@
                 # if n_rch > max_manning_n:
                 #     nrch = max_manning_n
                 # AllCatinfo.loc[AllCatinfo["SubId"] == csubid, "BkfWidth"] = 7.2 * q ** 0.5
                 # AllCatinfo.loc[AllCatinfo["SubId"] == csubid, "BkfDepth"] = 0.27 * q ** 0.3
                 # AllCatinfo.loc[AllCatinfo["SubId"] == csubid, "Q_Mean"] = q
                 # AllCatinfo.loc[AllCatinfo["SubId"] == csubid, "Ch_n"] = n_rch
 
-
-
-                ####find next downsubbasin id
+                # find next downsubbasin id
                 downsubid = C_sub_info["DowSubId"].values[0]
 
-                ### downsubid did not exist.....
+                # downsubid did not exist.....
                 if len(AllCatinfo.loc[AllCatinfo["SubId"] == downsubid]) <= 0:
                     if int(csubid) != int(Watershedoutletsubid):
                         print("Subregion:   ", d_subr_id)
                         print(
                             "SubId is ",
                             csubid,
                             " DownSubId is  ",
@@ -1456,21 +1554,21 @@
                         )
                     break
 
                 downsub_reg_id = AllCatinfo.loc[AllCatinfo["SubId"] == downsubid][
                     "Region_ID"
                 ].values[0]
 
-            ### update list for next loop
+            # update list for next loop
         Subregion_list = list(set(Subregion_list))
         iloop = iloop + 1
 
-
     print("Check drainage area:")
-    print("Total basin area is              ", sum(AllCatinfo["BasArea"].values))
+    print("Total basin area is              ",
+          sum(AllCatinfo["BasArea"].values))
     print(
         "DA of the watersehd outlet is    ",
         AllCatinfo.loc[AllCatinfo["SubId"] == int(Watershedoutletsubid)]["DrainArea"].values[
             0
         ],
     )
     print("Total DA of each subregion       ", Total_DA_Subregion)
@@ -1512,16 +1610,16 @@
     #  then this feature is not covered by the lake the new hru id  = old subid
 
     for i in range(0, len(Attribute_Table)):
         subid_sf_obj = Attribute_Table[Sub_ID].values[i]
         lakelakeid_sf_obj = Attribute_Table[Lake_Id].values[i]
         Sub_Lakeid_sf_obj = Attribute_Table[Sub_Lake_ID].values[i]
 
-        ### the null value in the attribute table is not convertable try and set
-        ### to -1
+        # the null value in the attribute table is not convertable try and set
+        # to -1
         try:
             subid_sf = float(subid_sf_obj)
         except:
             subid_sf = -1
             Attribute_Table.loc[i, Sub_ID] = -1
             pass
 
@@ -1548,18 +1646,18 @@
         if Sub_Lakeid_sf <= 0:
             old_new_hruid = subid_sf
             Attribute_Table.loc[i, "HRU_IsLake"] = -1
 
         if Sub_Lakeid_sf > 0:
             if (
                 lakelakeid_sf == Sub_Lakeid_sf
-            ):  ### the lakeid from lake polygon = lake id in subbasin polygon
+            ):  # the lakeid from lake polygon = lake id in subbasin polygon
                 old_new_hruid = subid_sf + max_subbasin_id + 10
                 Attribute_Table.loc[i, "HRU_IsLake"] = 1
-            else:  ### the lakeid from lake polygon != lake id in subbasin polygon, this lake do not belong to this subbasin, this part of subbasin treat as non lake hru
+            else:  # the lakeid from lake polygon != lake id in subbasin polygon, this lake do not belong to this subbasin, this part of subbasin treat as non lake hru
                 old_new_hruid = float(subid_sf)
                 Attribute_Table.loc[i, "HRU_IsLake"] = -1
 
         # if it is a new hru id
         if old_new_hruid not in old_newhruid_list:
             Attribute_Table.loc[i, "HRULake_ID"] = new_hruid
             old_newhruid_list[new_hruid] = old_new_hruid
@@ -1580,15 +1678,15 @@
         Sub_Lakeid_sf = Attribute_Table[Sub_Lake_ID].values[i]
         if subid_sf > 0:
             continue
         if lakelakeid_sf <= 0:
             print("lake has unexpected holes ")
             print(Attribute_Table.loc[i, :])
             continue
-        ### find the subid of lakelakeid_sf
+        # find the subid of lakelakeid_sf
         tar_info = Attribute_Table.loc[
             (Attribute_Table[Lake_Id] == lakelakeid_sf)
             & (Attribute_Table["HRU_IsLake"] > 0)
         ]
         if len(tar_info) <= 0:
             print('Lakeid do not exist   ', lakelakeid_sf)
             continue
@@ -1603,21 +1701,22 @@
 def Retrun_Validate_Attribute_Value(Attri_table_Lake_HRU_i, SubInfo, Col_NM, info_data):
 
     info_lake_hru = Attri_table_Lake_HRU_i.loc[Attri_table_Lake_HRU_i[Col_NM] != 0]
     if (
         len(info_lake_hru) > 0
     ):  # other part of this lake hru has validate soilid use the one with maximum area
         Updatevalue = info_lake_hru[Col_NM].values[0]
-    else:  ### check if the subbasin has a valid soil id
+    else:  # check if the subbasin has a valid soil id
         SubInfo = SubInfo.loc[SubInfo[Col_NM] != 0]
         SubInfo = SubInfo.sort_values(by="HRU_Area", ascending=False)
         if len(SubInfo) > 0:
             Updatevalue = SubInfo[Col_NM].values[0]
         else:
-            Updatevalue = info_data.loc[info_data[Col_NM] != 0][Col_NM].values[0]
+            Updatevalue = info_data.loc[info_data[Col_NM]
+                                        != 0][Col_NM].values[0]
     #            print("asdfasdfsadf2",Updatevalue)
     #    print("asdfasdfsadf1",Updatevalue)
     return Updatevalue
 
 
 def Determine_HRU_Attributes(
     Attri_table,
@@ -1640,23 +1739,25 @@
     Returns:
     -------
         None,
     """
 
     # find invald rows
     inval_sub = Attri_table[Sub_ID] <= 0
-    inval_landuse = (Attri_table[Landuse_ID] <= 0) & (Attri_table[Landuse_ID] != -1)
+    inval_landuse = (Attri_table[Landuse_ID] <= 0) & (
+        Attri_table[Landuse_ID] != -1)
     inval_soil = (Attri_table[Soil_ID] <= 0) & (Attri_table[Soil_ID] != -1)
     inval_veg = (Attri_table[Veg_ID] <= 0) & (Attri_table[Veg_ID] != -1)
-    inval_o2 = (Attri_table[Other_Ply_ID_2] <= 0) & (Attri_table[Other_Ply_ID_2] != -1)
+    inval_o2 = (Attri_table[Other_Ply_ID_2] <= 0) & (
+        Attri_table[Other_Ply_ID_2] != -1)
 
     inval_rows = inval_sub | inval_landuse | inval_soil | inval_veg | inval_o2
-    Lake_HRU_IDS = np.unique(Attri_table.loc[inval_rows,"HRULake_ID"].values)
+    Lake_HRU_IDS = np.unique(Attri_table.loc[inval_rows, "HRULake_ID"].values)
     Lake_HRU_IDS = Lake_HRU_IDS[Lake_HRU_IDS > 0]
-    ### landuse,soil,and veg and other properties for lake hrus
+    # landuse,soil,and veg and other properties for lake hrus
 
     for i in range(0, len(Lake_HRU_IDS)):
         ilake_hru_id = Lake_HRU_IDS[i]
         if ilake_hru_id == 0:
             continue
         # obtain i lake hru attributes
         Attri_table_Lake_HRU_i = Attri_table.loc[
@@ -1670,108 +1771,114 @@
         for j in range(0, len(Attri_table_Lake_HRU_i)):
             ihru_id = Attri_table_Lake_HRU_i["HRU_ID"].values[j]
             is_Lake = Attri_table_Lake_HRU_i["HRU_IsLake"].values[j]
             if is_Lake > 0:
 
                 if (
                     Attri_table_Lake_HRU_i[Soil_ID].values[0] == 0
-                ):  ###  the current hru has invalidate soil id
+                ):  # the current hru has invalidate soil id
                     Vali_Value = Retrun_Validate_Attribute_Value(
                         Attri_table_Lake_HRU_i, SubInfo, Soil_ID, Soil_info_data
                     )
                     Attri_table.loc[
                         Attri_table["HRU_ID"] == ihru_id, Soil_ID
                     ] = Vali_Value
                 else:
                     Attri_table.loc[
                         Attri_table["HRU_ID"] == ihru_id, Soil_ID
                     ] = Attri_table_Lake_HRU_i[Soil_ID].values[0]
 
                 if (
                     Attri_table_Lake_HRU_i[Other_Ply_ID_1].values[0] == 0
-                ):  ###  the current hru has invalidate soil id
+                ):  # the current hru has invalidate soil id
                     Vali_Value = Retrun_Validate_Attribute_Value(
                         Attri_table_Lake_HRU_i, SubInfo, Other_Ply_ID_1, Attri_table
                     )
                     Attri_table.loc[
                         Attri_table["HRU_ID"] == ihru_id, Other_Ply_ID_1
                     ] = Vali_Value
                 else:
                     Attri_table.loc[
                         Attri_table["HRU_ID"] == ihru_id, Other_Ply_ID_1
                     ] = Attri_table_Lake_HRU_i[Other_Ply_ID_1].values[0]
 
                 if (
                     Attri_table_Lake_HRU_i[Other_Ply_ID_2].values[0] == 0
-                ):  ###  the current hru has invalidate soil id
+                ):  # the current hru has invalidate soil id
                     Vali_Value = Retrun_Validate_Attribute_Value(
                         Attri_table_Lake_HRU_i, SubInfo, Other_Ply_ID_2, Attri_table
                     )
                     Attri_table.loc[
                         Attri_table["HRU_ID"] == ihru_id, Other_Ply_ID_2
                     ] = Vali_Value
                 else:
                     Attri_table.loc[
                         Attri_table["HRU_ID"] == ihru_id, Other_Ply_ID_2
                     ] = Attri_table_Lake_HRU_i[Other_Ply_ID_2].values[0]
 
-                Attri_table.loc[Attri_table["HRU_ID"] == ihru_id, Landuse_ID] = int(-1)
-                Attri_table.loc[Attri_table["HRU_ID"] == ihru_id, Veg_ID] = int(-1)
+                Attri_table.loc[Attri_table["HRU_ID"]
+                                == ihru_id, Landuse_ID] = int(-1)
+                Attri_table.loc[Attri_table["HRU_ID"]
+                                == ihru_id, Veg_ID] = int(-1)
 
             else:
                 if (
                     Attri_table_Lake_HRU_i[Soil_ID].values[j] == 0
-                ):  ###  the current hru has invalidate soil id
+                ):  # the current hru has invalidate soil id
                     Vali_Value = Retrun_Validate_Attribute_Value(
                         Attri_table_Lake_HRU_i, SubInfo, Soil_ID, Soil_info_data
                     )
                     Attri_table.loc[
                         Attri_table["HRU_ID"] == ihru_id, Soil_ID
                     ] = Vali_Value
                 if (
                     Attri_table_Lake_HRU_i[Landuse_ID].values[j] == 0
-                ):  ###  the current hru has invalidate soil id
+                ):  # the current hru has invalidate soil id
                     Vali_Value = Retrun_Validate_Attribute_Value(
                         Attri_table_Lake_HRU_i, SubInfo, Landuse_ID, Landuse_info_data
                     )
                     Attri_table.loc[
                         Attri_table["HRU_ID"] == ihru_id, Landuse_ID
                     ] = Vali_Value
                 if (
                     Attri_table_Lake_HRU_i[Veg_ID].values[j] == 0
-                ):  ###  the current hru has invalidate soil id
+                ):  # the current hru has invalidate soil id
                     Vali_Value = Retrun_Validate_Attribute_Value(
                         Attri_table_Lake_HRU_i, SubInfo, Veg_ID, Veg_info_data
                     )
                     Attri_table.loc[
                         Attri_table["HRU_ID"] == ihru_id, Veg_ID
                     ] = Vali_Value
                 if (
                     Attri_table_Lake_HRU_i[Other_Ply_ID_1].values[j] == 0
-                ):  ###  the current hru has invalidate soil id
+                ):  # the current hru has invalidate soil id
                     Vali_Value = Retrun_Validate_Attribute_Value(
                         Attri_table_Lake_HRU_i, SubInfo, Other_Ply_ID_1, Attri_table
                     )
                     Attri_table.loc[
                         Attri_table["HRU_ID"] == ihru_id, Other_Ply_ID_1
                     ] = Vali_Value
                 if (
                     Attri_table_Lake_HRU_i[Other_Ply_ID_2].values[j] == 0
-                ):  ###  the current hru has invalidate soil id
+                ):  # the current hru has invalidate soil id
                     Vali_Value = Retrun_Validate_Attribute_Value(
                         Attri_table_Lake_HRU_i, SubInfo, Other_Ply_ID_2, Attri_table
                     )
                     Attri_table.loc[
                         Attri_table["HRU_ID"] == ihru_id, Other_Ply_ID_2
                     ] = Vali_Value
 
-    Attri_table = Attri_table.drop(columns=['LAND_USE_C', 'VEG_C','SOIL_PROF'])
-    Attri_table = pd.merge(Attri_table, Landuse_info_data, how='inner', on = Landuse_ID).copy(deep=True)
-    Attri_table = pd.merge(Attri_table, Soil_info_data, how='inner', on = Soil_ID).copy(deep=True)
-    Attri_table = pd.merge(Attri_table, Veg_info_data, how='inner', on = Veg_ID).copy(deep=True)
+    Attri_table = Attri_table.drop(
+        columns=['LAND_USE_C', 'VEG_C', 'SOIL_PROF'])
+    Attri_table = pd.merge(Attri_table, Landuse_info_data,
+                           how='inner', on=Landuse_ID).copy(deep=True)
+    Attri_table = pd.merge(Attri_table, Soil_info_data,
+                           how='inner', on=Soil_ID).copy(deep=True)
+    Attri_table = pd.merge(Attri_table, Veg_info_data,
+                           how='inner', on=Veg_ID).copy(deep=True)
 
     # for i in range(0, len(Attri_table)):
     #     if Attri_table["HRULake_ID"].values[i] == 0:
     #         continue
     #     Is_lake_hru = Attri_table["HRU_IsLake"].values[i]
     #     lake_hru_ID = Attri_table["HRULake_ID"].values[i]
     #     hruid = Attri_table["HRU_ID"].values[i]
@@ -1854,17 +1961,17 @@
     #         Attri_table.loc[i, "SOIL_PROF"] = int(0)
     #         Attri_table.loc[i, "SubId"] = int(0)
 
     Attri_table["facters"] = (
         Attri_table["HRULake_ID"].astype(str)
         + Attri_table[Landuse_ID].astype(str)
         + Attri_table[Soil_ID].astype(str)
-#        + Attri_table[Veg_ID].astype(str)
+        #        + Attri_table[Veg_ID].astype(str)
         + Attri_table[Other_Ply_ID_1].astype(str)
-#        + Attri_table[Other_Ply_ID_2].astype(str)
+        #        + Attri_table[Other_Ply_ID_2].astype(str)
     )
     Attri_table["HRU_ID_New"] = pd.factorize(Attri_table["facters"])[0] + 1
     return Attri_table
 
 
 def Change_Attribute_Values_For_Catchments_Need_To_Be_Merged_By_Increase_DA(
     finalriv_info, Conn_Lakes_ply, Area_Min
@@ -1884,207 +1991,212 @@
     DA_colnm = "DrainArea"
     SegID_colnm = "Seg_ID"
 
     Gauge_col_Name = "Has_POI"
     if "Has_POI" not in finalriv_info.columns:
         Gauge_col_Name = "Has_Gauge"
 
-    ### Modify attribute table mapoldnew_info, create new sub id for
-    ### 1. catchment needs to be merged due to meet the drainage area thresthold
-    ### 2. connected lake catchment are transfered into non-connected lake catchment
+    # Modify attribute table mapoldnew_info, create new sub id for
+    # 1. catchment needs to be merged due to meet the drainage area thresthold
+    # 2. connected lake catchment are transfered into non-connected lake catchment
 
     # copy attribute tabke and create two column to store new subid
     mapoldnew_info = finalriv_info.copy(deep=True)
     mapoldnew_info["nsubid"] = -1
     mapoldnew_info["ndownsubid"] = -1
     mapoldnew_info.reset_index(drop=True, inplace=True)
     max_da = np.max(mapoldnew_info['DrainArea'].values)
 
-    ## stupid larege drainage area are provied
+    # stupid larege drainage area are provied
     if Area_Min * 1000 * 1000 > max_da:
         Area_Min = max_da/1000.0/1000.0 - 1
-        mapoldnew_info[Gauge_col_Name] =  -1
+        mapoldnew_info[Gauge_col_Name] = -1
         finalriv_info[Gauge_col_Name] = -1
 
-
     # select catchment segment that meet the drainage area
     Selected_riv = finalriv_info.loc[
         finalriv_info[DA_colnm] >= Area_Min * 1000 * 1000
     ].copy()  # find river with drainage area larger than area thresthold
 
+    Selected_riv = update_the_selected_river_to_connect_upsub_with_largest_da(
+        Selected_riv, mapoldnew_info)
+
     # calcuate topology for the selected catchment
     Selected_riv = UpdateTopology(Selected_riv, UpdateSubId=-1)
     Selected_riv = Selected_riv.sort_values(
         ["Strahler"], ascending=(True)
-    )  ###sort selected river by Strahler stream order
+    )  # sort selected river by Strahler stream order
     Selected_riv = Selected_riv.loc[Selected_riv['Lake_Cat'] != 2].copy()
     Subid_main = Selected_riv[sub_colnm].values
 
-    ### Obtain connected lakes based on current river segment
+    # Obtain connected lakes based on current river segment
     Connected_Lake_Mainriv = Selected_riv.loc[Selected_riv["Lake_Cat"] == 1][
         "HyLakeId"
     ].values
     Connected_Lake_Mainriv = np.unique(
         Connected_Lake_Mainriv[Connected_Lake_Mainriv > 0]
     )
     Lakecover_riv = finalriv_info.loc[
         finalriv_info["HyLakeId"].isin(Connected_Lake_Mainriv)
     ].copy()
     Subid_lakes = Lakecover_riv[sub_colnm].values
     #####
 
     ###
-    ## add removed gauges and remove gauge if gauge located within a lake on the main river
+    # add removed gauges and remove gauge if gauge located within a lake on the main river
     unselected_gauges_subids_info = finalriv_info.loc[
         (~finalriv_info["SubId"].isin(Subid_main)) &
-        (finalriv_info[Gauge_col_Name] > 0 )
+        (finalriv_info[Gauge_col_Name] > 0)
     ].copy(deep=True)
-    unselected_gauges_subids = unselected_gauges_subids_info.loc[unselected_gauges_subids_info["HyLakeId"] <= 0]["SubId"].values
+    unselected_gauges_subids = unselected_gauges_subids_info.loc[
+        unselected_gauges_subids_info["HyLakeId"] <= 0]["SubId"].values
 
     finalriv_info_ncl = finalriv_info.copy(deep=True)
     # make unselected gauge to be a false lake
     mask1 = finalriv_info_ncl['SubId'].isin(unselected_gauges_subids)
     mask2 = finalriv_info_ncl['HyLakeId'] < 1
-    mask = np.logical_and(mask1,mask2)
-    finalriv_info_ncl.loc[mask,'HyLakeId'] = - finalriv_info_ncl.loc[finalriv_info_ncl['SubId'].isin(unselected_gauges_subids),'SubId']
-    fake_obs_hyalkeids =  finalriv_info_ncl.loc[finalriv_info_ncl['SubId'].isin(unselected_gauges_subids),'HyLakeId'].values
+    mask = np.logical_and(mask1, mask2)
+    finalriv_info_ncl.loc[mask, 'HyLakeId'] = - \
+        finalriv_info_ncl.loc[finalriv_info_ncl['SubId'].isin(
+            unselected_gauges_subids), 'SubId']
+    fake_obs_hyalkeids = finalriv_info_ncl.loc[finalriv_info_ncl['SubId'].isin(
+        unselected_gauges_subids), 'HyLakeId'].values
     ##
     ###
     # identify which connected lake will be moved to non connected lake due to remove of river network
     All_Conn_Lakeids = Conn_Lakes_ply["Hylak_id"].values
     mask = np.in1d(All_Conn_Lakeids, Connected_Lake_Mainriv)
     Conn_To_NonConlakeids = All_Conn_Lakeids[np.logical_not(mask)].copy()
     Conn_To_NonConlake_info = finalriv_info_ncl.loc[
         (finalriv_info_ncl["HyLakeId"].isin(Conn_To_NonConlakeids)) |
         (finalriv_info_ncl["HyLakeId"].isin(fake_obs_hyalkeids))
     ].copy()
 
-
-
-
-
     # Get origional non connected lake subid and lake id
     Old_Non_Connect_SubIds = finalriv_info.loc[finalriv_info["Lake_Cat"] == 2][
         "SubId"
     ].values
     Old_Non_Connect_SubIds = np.unique(
         Old_Non_Connect_SubIds[Old_Non_Connect_SubIds > 0]
     )
     Old_Non_Connect_LakeIds = finalriv_info.loc[finalriv_info["Lake_Cat"] == 2][
         "HyLakeId"
     ].values
     Old_Non_Connect_LakeIds = np.unique(
         Old_Non_Connect_LakeIds[Old_Non_Connect_LakeIds > 0]
     )
 
-    ### obtain rivsegments that covered by remaining lakes
+    # obtain rivsegments that covered by remaining lakes
     Selected_riv_ids = np.unique(
         Subid_main
     )  # np.unique(np.concatenate([Subid_main,Subid_lakes]))
     routing_info = finalriv_info[["SubId", "DowSubId"]].astype("float").values
     Seg_IDS = Selected_riv["Seg_ID"].values
     Seg_IDS = np.unique(Seg_IDS)
 
-    ##### for Non connected lakes, catchment polygon do not need to change
+    # for Non connected lakes, catchment polygon do not need to change
     mapoldnew_info.loc[mapoldnew_info["Lake_Cat"] == 2, "nsubid"] = mapoldnew_info.loc[
         mapoldnew_info["Lake_Cat"] == 2
     ]["SubId"].values
 
-    #####for catchment polygon flow to lake with is changed from connected lake to non connected lakes
+    # for catchment polygon flow to lake with is changed from connected lake to non connected lakes
     idx = (
-        Conn_To_NonConlake_info.groupby(["HyLakeId"])["DrainArea"].transform(max)
+        Conn_To_NonConlake_info.groupby(
+            ["HyLakeId"])["DrainArea"].transform(max)
         == Conn_To_NonConlake_info["DrainArea"]
     )
     Conn_To_NonConlake_info_outlet = Conn_To_NonConlake_info[idx]
 
     Conn_To_NonConlake_info_outlet = Conn_To_NonConlake_info_outlet.sort_values(
         ["Strahler", "DrainArea"], ascending=[True, True]
     )
 
-
     ###
-    all_outlet_sub_info = finalriv_info[finalriv_info["DowSubId"] < 0 ].copy(deep=True)
+    all_outlet_sub_info = finalriv_info[finalriv_info["DowSubId"] < 0].copy(
+        deep=True)
 
-    for i in range(0,len(all_outlet_sub_info)):
+    for i in range(0, len(all_outlet_sub_info)):
         if all_outlet_sub_info['DrainArea'].values[i] <= Area_Min * 1000 * 1000:
             tsubid = all_outlet_sub_info['SubId'].values[i]
             All_up_subids = defcat(routing_info, tsubid)
 
             mapoldnew_info = New_SubId_To_Dissolve(
                 subid=tsubid,
                 catchmentinfo=finalriv_info,
                 mapoldnew_info=mapoldnew_info,
                 ismodifids=1,
                 mainriv=finalriv_info,
                 modifiidin=All_up_subids,
                 Lake_Cat=-1,
             )
 
-
-
-    ### process fron upstream lake to down stream lake
+    # process fron upstream lake to down stream lake
     for i in range(0, len(Conn_To_NonConlake_info_outlet)):
         processed_subid = np.unique(
             mapoldnew_info.loc[mapoldnew_info["nsubid"] > 0][sub_colnm].values
         )
 
         C_T_N_Lakeid = Conn_To_NonConlake_info_outlet["HyLakeId"].values[i]
-        Lake_Cat_info = finalriv_info_ncl[finalriv_info_ncl["HyLakeId"] == C_T_N_Lakeid]
+        Lake_Cat_info = finalriv_info_ncl[finalriv_info_ncl["HyLakeId"]
+                                          == C_T_N_Lakeid]
         Riv_Seg_IDS = np.unique(Lake_Cat_info["Seg_ID"].values)
         modifysubids = []
         for j in range(0, len(Riv_Seg_IDS)):
 
             iriv_seg = Riv_Seg_IDS[j]
             Lake_Cat_seg_info = Lake_Cat_info.loc[
                 Lake_Cat_info["Seg_ID"] == iriv_seg
             ].copy()
-            Lake_Cat_seg_info = Lake_Cat_seg_info.sort_values(["DrainArea"], ascending=(False))
+            Lake_Cat_seg_info = Lake_Cat_seg_info.sort_values(
+                ["DrainArea"], ascending=(False))
             tsubid = Lake_Cat_seg_info["SubId"].values[0]
 
             All_up_subids = defcat(routing_info, tsubid)
             All_up_subids = All_up_subids[All_up_subids > 0]
 
             mask = np.in1d(All_up_subids, processed_subid)
             seg_sub_ids = All_up_subids[np.logical_not(mask)]
 
             modifysubids = [
                 *modifysubids,
                 *seg_sub_ids.tolist(),
-            ]  ### combine two list not sum
+            ]  # combine two list not sum
 
         modifysubids = np.asarray(modifysubids)
 
         mapoldnew_info = New_SubId_To_Dissolve(
             subid=tsubid,
             catchmentinfo=finalriv_info_ncl,
             mapoldnew_info=mapoldnew_info,
             ismodifids=1,
             mainriv=finalriv_info_ncl,
             modifiidin=modifysubids,
             Lake_Cat=2,
         )
-        ####################3 for rest of the polygons dissolve to main river
+        # 3 for rest of the polygons dissolve to main river
 
     for iseg in range(0, len(Seg_IDS)):
         #            print('#########################################################################################33333')
         i_seg_id = Seg_IDS[iseg]
-        i_seg_info = Selected_riv.loc[Selected_riv["Seg_ID"] == i_seg_id].copy()
+        i_seg_info = Selected_riv.loc[Selected_riv["Seg_ID"] == i_seg_id].copy(
+        )
         i_seg_info = i_seg_info.sort_values(["Seg_order"], ascending=(True))
         sum_area = 0
         modifysubids = []
         seg_order = 1
         for iorder in range(0, len(i_seg_info)):
             tsubid = i_seg_info["SubId"].values[iorder]
             iorder_Lakeid = i_seg_info["HyLakeId"].values[iorder]
             modifysubids.append(tsubid)
             processed_subid = np.unique(
-                mapoldnew_info.loc[mapoldnew_info["nsubid"] > 0][sub_colnm].values
+                mapoldnew_info.loc[mapoldnew_info["nsubid"]
+                                   > 0][sub_colnm].values
             )
             sum_area = sum_area + i_seg_info["BasArea"].values[iorder]
-            ### two seg has the same HyLakeId id, can be merged
+            # two seg has the same HyLakeId id, can be merged
 
             # if has the same lake attribute with down stream subasins
             if iorder != len(i_seg_info) - 1:
                 con_lake = i_seg_info["HyLakeId"].values[iorder] == i_seg_info["HyLakeId"].values[iorder + 1]
             else:
                 con_lake = False
             # if do not have the gauge
@@ -2095,80 +2207,82 @@
                 if i_seg_info["BasArea"].values[iorder + 1] < 10 * 1000 * 1000:
                     con_area = True
                 else:
                     con_area = sum_area < Area_Min * 1000 * 1000
             else:
                 con_area = sum_area < Area_Min * 1000 * 1000
 
-
             con_area_lake = sum_area < 10 * 1000 * 1000
             # conditions check if subbasin is between two lakes
             if iorder >= 1 and iorder <= len(i_seg_info) - 2:
                 # if not havve the same attribute with upstream lake
-                con_lake_up = i_seg_info["HyLakeId"].values[iorder - 1] != i_seg_info["HyLakeId"].values[iorder]
+                con_lake_up = i_seg_info["HyLakeId"].values[iorder -
+                                                            1] != i_seg_info["HyLakeId"].values[iorder]
                 # if not havve the same attribute with down lake
                 con_lake_down = i_seg_info["HyLakeId"].values[iorder] != i_seg_info["HyLakeId"].values[iorder + 1]
                 # if this is not a lake subbasin
                 is_lake = i_seg_info["HyLakeId"].values[iorder] <= 0
 
-                con_area_lake = False #i_seg_info["BasArea"].values[iorder] < 10 * 1000 * 1000
+                # i_seg_info["BasArea"].values[iorder] < 10 * 1000 * 1000
+                con_area_lake = False
 
             if iorder == 0 and iorder < len(i_seg_info) - 1:
                 # if not havve the same attribute with upstream lake
                 con_lake_up = True
                 # if not havve the same attribute with down lake
                 con_lake_down = i_seg_info["HyLakeId"].values[iorder] != i_seg_info["HyLakeId"].values[iorder + 1]
                 # if this is not a lake subbasin
                 is_lake = i_seg_info["HyLakeId"].values[iorder] <= 0
 
-                con_area_lake = False #i_seg_info["BasArea"].values[iorder] < 10 * 1000 * 1000
+                # i_seg_info["BasArea"].values[iorder] < 10 * 1000 * 1000
+                con_area_lake = False
 
             if iorder == len(i_seg_info) - 2 and i_seg_info["HyLakeId"].values[iorder] > 0:
                 # if not havve the same attribute with upstream lake
                 con_lake_up = True
                 # if not havve the same attribute with down lake
                 con_lake_down = i_seg_info["HyLakeId"].values[iorder] != i_seg_info["HyLakeId"].values[iorder + 1]
                 # if this is not a lake subbasin
                 is_lake = i_seg_info["HyLakeId"].values[iorder] > 0
 
                 # if tsubid == 9023607:
                 #     print(con_lake_up,con_lake_down,is_lake,iorder,len(i_seg_info) - 2,i_seg_info["HyLakeId"].values[iorder] > 0)
                 # change add lake to downstream info
                 downsubid = i_seg_info["DowSubId"].values[iorder]
 
-                con_area_lake = False #i_seg_info["BasArea"].values[iorder +1] < 10 * 1000 * 1000
+                # i_seg_info["BasArea"].values[iorder +1] < 10 * 1000 * 1000
+                con_area_lake = False
 
                 if con_area_lake and con_lake_down:
                     finalriv_info.loc[
-                        finalriv_info["SubId"] == downsubid,'HyLakeId'] = i_seg_info["HyLakeId"].values[iorder]
+                        finalriv_info["SubId"] == downsubid, 'HyLakeId'] = i_seg_info["HyLakeId"].values[iorder]
                     finalriv_info.loc[
-                        finalriv_info["SubId"] == downsubid,'Lake_Cat'] = i_seg_info["Lake_Cat"].values[iorder]
+                        finalriv_info["SubId"] == downsubid, 'Lake_Cat'] = i_seg_info["Lake_Cat"].values[iorder]
                     finalriv_info.loc[
-                        finalriv_info["SubId"] == downsubid,'LakeVol'] = i_seg_info["LakeVol"].values[iorder]
+                        finalriv_info["SubId"] == downsubid, 'LakeVol'] = i_seg_info["LakeVol"].values[iorder]
                     finalriv_info.loc[
-                        finalriv_info["SubId"] == downsubid,'LakeDepth'] = i_seg_info["LakeDepth"].values[iorder]
+                        finalriv_info["SubId"] == downsubid, 'LakeDepth'] = i_seg_info["LakeDepth"].values[iorder]
                     finalriv_info.loc[
-                        finalriv_info["SubId"] == downsubid,'LakeArea'] = i_seg_info["LakeArea"].values[iorder]
+                        finalriv_info["SubId"] == downsubid, 'LakeArea'] = i_seg_info["LakeArea"].values[iorder]
                     finalriv_info.loc[
-                        finalriv_info["SubId"] == downsubid,'Laketype'] = i_seg_info["Laketype"].values[iorder]
+                        finalriv_info["SubId"] == downsubid, 'Laketype'] = i_seg_info["Laketype"].values[iorder]
 
             if iorder == len(i_seg_info) - 1:
                 con_lake_up = True
                 con_lake_down = False
                 is_lake = True
 
             # if tsubid == 4703912:
             #     print(con_lake_up,con_lake_down,is_lake,iorder,len(i_seg_info) - 2,i_seg_info["HyLakeId"].values[iorder] > 0)
             #     asdf
 
-
             if iorder == len(i_seg_info) - 1:
                 sum_area = 0
                 seg_sub_ids = np.asarray(modifysubids)
-                ## if needs to add lake sub around the main stream
+                # if needs to add lake sub around the main stream
                 if iorder_Lakeid > 0:
                     subid_cur_lake_info = finalriv_info.loc[
                         finalriv_info["HyLakeId"] == iorder_Lakeid
                     ].copy()
                     routing_info_lake = (
                         subid_cur_lake_info[["SubId", "DowSubId"]]
                         .astype("float")
@@ -2176,20 +2290,20 @@
                     )
                     UpstreamLakeids = defcat(routing_info_lake, tsubid)
                     seg_sub_ids = np.unique(
                         np.concatenate([seg_sub_ids, UpstreamLakeids])
                     )
                     seg_sub_ids = seg_sub_ids[seg_sub_ids > 0]
 
-                    ### merge all subbasin not connected to the main river but drainarge to this tsubid
+                    # merge all subbasin not connected to the main river but drainarge to this tsubid
                 All_up_subids = defcat(routing_info, tsubid)
                 All_up_subids = All_up_subids[All_up_subids > 0]
                 mask1 = np.in1d(
                     All_up_subids, Subid_main
-                )  ### exluced ids that belongs to main river stream
+                )  # exluced ids that belongs to main river stream
                 All_up_subids_no_main = All_up_subids[np.logical_not(mask1)]
 
                 seg_sub_ids = np.unique(
                     np.concatenate([seg_sub_ids, All_up_subids_no_main])
                 )
                 seg_sub_ids = seg_sub_ids[seg_sub_ids > 0]
                 mask = np.in1d(seg_sub_ids, processed_subid)
@@ -2217,15 +2331,15 @@
 
             elif con_lake and con_gauge and con_area:
                 continue
 
             else:
                 sum_area = 0
                 seg_sub_ids = np.asarray(modifysubids)
-                ## if needs to add lake sub around the main stream
+                # if needs to add lake sub around the main stream
                 if iorder_Lakeid > 0:
                     subid_cur_lake_info = finalriv_info.loc[
                         finalriv_info["HyLakeId"] == iorder_Lakeid
                     ].copy()
                     routing_info_lake = (
                         subid_cur_lake_info[["SubId", "DowSubId"]]
                         .astype("float")
@@ -2237,57 +2351,234 @@
                     )
                     seg_sub_ids = seg_sub_ids[seg_sub_ids > 0]
 
                 All_up_subids = defcat(routing_info, tsubid)
                 All_up_subids = All_up_subids[All_up_subids > 0]
                 mask1 = np.in1d(
                     All_up_subids, Subid_main
-                )  ### exluced ids that belongs to main river stream
+                )  # exluced ids that belongs to main river stream
                 All_up_subids_no_main = All_up_subids[np.logical_not(mask1)]
 
                 seg_sub_ids = np.unique(
                     np.concatenate([seg_sub_ids, All_up_subids_no_main])
                 )
                 seg_sub_ids = seg_sub_ids[seg_sub_ids > 0]
                 mask = np.in1d(seg_sub_ids, processed_subid)
                 seg_sub_ids = seg_sub_ids[np.logical_not(mask)]
 
                 mask_old_nonLake = np.in1d(seg_sub_ids, Old_Non_Connect_SubIds)
                 seg_sub_ids = seg_sub_ids[np.logical_not(mask_old_nonLake)]
 
-
                 mapoldnew_info = New_SubId_To_Dissolve(
                     subid=tsubid,
                     catchmentinfo=finalriv_info,
                     mapoldnew_info=mapoldnew_info,
                     ismodifids=1,
                     modifiidin=seg_sub_ids,
                     mainriv=Selected_riv,
                     Lake_Cat=3,
                     seg_order=seg_order,
                 )
                 modifysubids = []
                 seg_order = seg_order + 1
 
-    mapoldnew_info.loc[mapoldnew_info['HyLakeId'] <= 0,'HyLakeId'] = 0
-    mapoldnew_info.loc[mapoldnew_info['HyLakeId'] <= 0,'Lake_Cat'] = 0
-    mapoldnew_info.loc[mapoldnew_info['HyLakeId'] <= 0,'LakeVol'] = 0
-    mapoldnew_info.loc[mapoldnew_info['HyLakeId'] <= 0,'LakeDepth'] = 0
-    mapoldnew_info.loc[mapoldnew_info['HyLakeId'] <= 0,'LakeArea'] = 0
-    mapoldnew_info.loc[mapoldnew_info['HyLakeId'] <= 0,'Laketype'] = 0
+    mapoldnew_info.loc[mapoldnew_info['HyLakeId'] <= 0, 'HyLakeId'] = 0
+    mapoldnew_info.loc[mapoldnew_info['HyLakeId'] <= 0, 'Lake_Cat'] = 0
+    mapoldnew_info.loc[mapoldnew_info['HyLakeId'] <= 0, 'LakeVol'] = 0
+    mapoldnew_info.loc[mapoldnew_info['HyLakeId'] <= 0, 'LakeDepth'] = 0
+    mapoldnew_info.loc[mapoldnew_info['HyLakeId'] <= 0, 'LakeArea'] = 0
+    mapoldnew_info.loc[mapoldnew_info['HyLakeId'] <= 0, 'Laketype'] = 0
 
     return (
         mapoldnew_info,
         Selected_riv_ids,
         Connected_Lake_Mainriv,
         Old_Non_Connect_LakeIds,
         Conn_To_NonConlakeids,
     )
 
 
+def update_the_selected_river_to_connect_upsub_with_largest_da(Selected_riv, mapoldnew_info):
+    Selected_riv_ids = np.unique(Selected_riv['SubId'].values)
+
+    # target to find all subid has do not have subbasins
+    # in the selected river network.
+    lakeid_in_new_network = np.unique(Selected_riv['HyLakeId'].values)
+    lakeid_in_new_network = lakeid_in_new_network[lakeid_in_new_network > 0]
+
+    mask_lakes = np.logical_and(
+        mapoldnew_info['Lake_Cat'] == 1, ~mapoldnew_info['HyLakeId'].isin(lakeid_in_new_network))
+
+    mask_pois = mapoldnew_info['Has_POI'] > 0
+
+    potential_sub_to_extend = mapoldnew_info[np.logical_or(
+        mask_lakes, mask_pois)].copy(deep=True)
+
+    potential_sub_to_extend = potential_sub_to_extend[~potential_sub_to_extend['SubId'].isin(
+        Selected_riv_ids)]
+    # extend each headwater stream
+    subid_with_upstream = np.unique(potential_sub_to_extend['SubId'].values)
+    for tsubid in subid_with_upstream:
+
+        # find all upstream subbasins
+        upstream_sub = mapoldnew_info[mapoldnew_info['SubId'] == tsubid].copy(
+            deep=True)
+
+        # check if one of the upstream subbasin already have river network
+        upstream_sub_withriver = upstream_sub[upstream_sub['SubId'].isin(
+            Selected_riv_ids)]
+
+        # if one of the upstream subbasin already have river network, skip
+        if len(upstream_sub_withriver) > 0 or len(upstream_sub) == 0:
+            continue
+
+        # remove channels all channels in this sub
+        Selected_riv_ids = np.append(Selected_riv_ids, tsubid)
+        # create new channel for this sub
+        # sort upstream subbasins by DrainArea
+        # the new channel start from a upstream subbasin with largest drainage area
+        upstream_sub = upstream_sub.sort_values(
+            by='DrainArea', ascending=False)
+
+        cur_subid = upstream_sub['SubId'].values[0]
+        # if tsubid == 17313:
+        #     print(mapoldnew_info.columns)
+        #     print(Selected_riv_ids)
+        #     print(mapoldnew_info[mapoldnew_info['SubId'] == tsubid][['Old_SubId','Old_DowSubId','SubId','DowSubId','nsubid', 'ndownsubid']])
+        # get the first channel which is the downsubid if the
+        cur_downsubid = mapoldnew_info[mapoldnew_info['SubId']
+                                       == cur_subid]['DowSubId'].values[0]
+        # print(tsubid,cur_downsubid,cur_downsubid not in Selected_riv_ids)
+        while cur_downsubid not in Selected_riv_ids and cur_downsubid != -1:
+            # print(tsubid,cur_downsubid)
+            Selected_riv_ids = np.append(Selected_riv_ids, cur_downsubid)
+            cur_subinfo = mapoldnew_info[mapoldnew_info['SubId'] == cur_downsubid].copy(
+                deep=True)
+            if len(cur_subinfo) <= 0:
+                print("check this subid ", cur_downsubid)
+                break
+            cur_downsubid = cur_subinfo['DowSubId'].values[0]
+    Selected_riv_out = mapoldnew_info[mapoldnew_info['SubId'].isin(
+        Selected_riv_ids)]
+    return Selected_riv_out
+
+
+def Add_River_Segment_Between_Lakes_And_Observations(mapoldnew_info, Selected_riv_ids, finalriv_infoply):
+    # function to add river network between lake or poi subbasin to non lake/poi subbasins
+    # used attributes in mapoldnew_info
+    # nsubid the new sub id for each subbasin
+    # ndownsubid the new dowsubid for each subbasin
+    # Selected_riv_ids is the river segment already included in the network
+    # mapoldnew_info["Old_SubId"] = mapoldnew_info["SubId"].values
+    # mapoldnew_info["Old_DowSubId"] = mapoldnew_info["DowSubId"].values
+    # mapoldnew_info["SubId"] = mapoldnew_info["nsubid"].values
+
+    # mapoldnew_info["DowSubId"] = mapoldnew_info["ndownsubid"].values
+
+    # target to find all subid has upstream subbasins
+    # and none upstream subbains have river network
+    # get all subbasins have a upstream subbasin
+    mask = mapoldnew_info['SubId'].isin(mapoldnew_info['DowSubId'].values)
+    sub_with_upstream = mapoldnew_info[mask].copy(deep=True)
+
+    subid_with_upstream = np.unique(sub_with_upstream['SubId'].values)
+    for tsubid in subid_with_upstream:
+
+        # find all upstream subbasins
+        upstream_sub = mapoldnew_info[mapoldnew_info['DowSubId'] == tsubid].copy(
+            deep=True)
+
+        # check if one of the upstream subbasin already have river network
+        upstream_sub_withriver = upstream_sub[upstream_sub['SubId'].isin(
+            Selected_riv_ids)]
+
+        # if one of the upstream subbasin already have river network, skip
+        if len(upstream_sub_withriver) > 0:
+            continue
+
+        # remove channels all channels in this sub
+        mask = np.isin(
+            Selected_riv_ids, mapoldnew_info[mapoldnew_info['SubId'] == tsubid]['Old_SubId'].values)
+        Selected_riv_ids = Selected_riv_ids[~mask]
+
+        # create new channel for this sub
+        # sort upstream subbasins by DrainArea
+        # the new channel start from a upstream subbasin with largest drainage area
+        upstream_sub = upstream_sub.sort_values(
+            by='DrainArea', ascending=False)
+        cur_subid = upstream_sub['SubId'].values[0]
+        # if tsubid == 17313:
+        #     print(mapoldnew_info.columns)
+        #     print(Selected_riv_ids)
+        #     print(mapoldnew_info[mapoldnew_info['SubId'] == tsubid][['Old_SubId','Old_DowSubId','SubId','DowSubId','nsubid', 'ndownsubid']])
+        # get the first channel which is the downsubid if the
+        cur_downsubid = finalriv_infoply[finalriv_infoply['SubId']
+                                         == cur_subid]['DowSubId'].values[0]
+        # print(tsubid,cur_downsubid,cur_downsubid not in Selected_riv_ids)
+        while cur_downsubid not in Selected_riv_ids and cur_downsubid != -1:
+            # print(tsubid,cur_downsubid)
+            Selected_riv_ids = np.append(Selected_riv_ids, cur_downsubid)
+            cur_subinfo = finalriv_infoply[finalriv_infoply['SubId'] == cur_downsubid].copy(
+                deep=True)
+            if len(cur_subinfo) <= 0:
+                print("check this subid ", cur_downsubid)
+                break
+            cur_downsubid = cur_subinfo['DowSubId'].values[0]
+    # print(17313 in Selected_riv_ids)
+    # remove all subid that are already included in the river network
+    mapoldnew_info = update_channel_attributes(
+        Selected_riv_ids, mapoldnew_info, finalriv_infoply)
+    return Selected_riv_ids, mapoldnew_info
+
+
+def update_channel_attributes(Selected_riv_ids, mapoldnew_info, finalriv_infoply):
+
+    # obtain subid in the new network that needs to be updated
+
+    subid_update_riv = np.unique(
+        mapoldnew_info[mapoldnew_info['Old_SubId'].isin(Selected_riv_ids)]['SubId'].values)
+    all_river_segments = finalriv_infoply[finalriv_infoply['SubId'].isin(
+        Selected_riv_ids)]
+    for tsubid in subid_update_riv:
+        mask_new = mapoldnew_info['SubId'] == tsubid
+        old_subids = np.unique(mapoldnew_info[mask_new]['Old_SubId'].values)
+        riv_in_new_sub = all_river_segments[all_river_segments['SubId'].isin(
+            old_subids)]
+
+        if len(riv_in_new_sub) > 0:
+            mapoldnew_info.loc[mask_new, "RivLength"] = np.sum(
+                riv_in_new_sub["RivLength"].values)
+            mapoldnew_info.loc[mask_new, "RivSlope"] = np.average(
+                riv_in_new_sub["RivSlope"].values,
+                weights=riv_in_new_sub["RivLength"].values,
+            )
+            mapoldnew_info.loc[mask_new, "FloodP_n"] = np.average(
+                riv_in_new_sub["FloodP_n"].values,
+                weights=riv_in_new_sub["RivLength"].values,
+            )
+            mapoldnew_info.loc[mask_new, "Q_Mean"] = np.average(
+                riv_in_new_sub["Q_Mean"].values,
+                weights=riv_in_new_sub["RivLength"].values,
+            )
+            mapoldnew_info.loc[mask_new, "Ch_n"] = np.average(
+                riv_in_new_sub["Ch_n"].values,
+                weights=riv_in_new_sub["RivLength"].values,
+            )
+            mapoldnew_info.loc[mask_new, "BkfWidth"] = np.max(
+                riv_in_new_sub["BkfWidth"].values)
+            mapoldnew_info.loc[mask_new, "BkfDepth"] = np.max(
+                riv_in_new_sub["BkfDepth"].values)
+
+            mapoldnew_info.loc[mask_new, "Max_DEM"] = np.max(
+                riv_in_new_sub["Max_DEM"].values)
+            mapoldnew_info.loc[mask_new, "Min_DEM"] = np.min(
+                riv_in_new_sub["Min_DEM"].values)
+    return mapoldnew_info
+
+
 def Return_Selected_Lakes_Attribute_Table_And_Id(
     finalcat_info,
     Thres_Area_Conn_Lakes,
     Thres_Area_Non_Conn_Lakes,
     Selected_Lake_List_in,
 ):
     """Retrun selected lake's attribute table and ID
@@ -2300,66 +2591,68 @@
     -------
         None,
     """
     finalcat_info["LakeArea"] = finalcat_info["LakeArea"].astype(float)
     finalcat_info["HyLakeId"] = finalcat_info["HyLakeId"].astype(int)
     finalcat_info["Seg_ID"] = finalcat_info["Seg_ID"].astype(int)
 
-    Non_ConnL_info = finalcat_info.loc[finalcat_info["Lake_Cat"] == 2].copy(deep=True)
-    ConnL_info = finalcat_info.loc[finalcat_info["Lake_Cat"] == 1].copy(deep=True)
+    Non_ConnL_info = finalcat_info.loc[finalcat_info["Lake_Cat"] == 2].copy(
+        deep=True)
+    ConnL_info = finalcat_info.loc[finalcat_info["Lake_Cat"] == 1].copy(
+        deep=True)
 
     if "Has_POI" in finalcat_info.columns:
         Gauge_col_Name = "Has_POI"
     else:
         Gauge_col_Name = "Has_Gauge"
     # first obtain selected lakes based on lake area
-    ### process connected lakes first
+    # process connected lakes first
     mask1 = ConnL_info["LakeArea"] >= Thres_Area_Conn_Lakes
     mask2 = ConnL_info[Gauge_col_Name] == 1
-    mask = np.logical_or(mask1,mask2)
+    mask = np.logical_or(mask1, mask2)
     Selected_ConnLakes = ConnL_info.loc[
-       mask
+        mask
     ]["HyLakeId"].values
 
     Selected_ConnLakes = Selected_ConnLakes[Selected_ConnLakes > 0]
     Selected_ConnLakes = np.unique(Selected_ConnLakes)
 
-
     mask1 = Non_ConnL_info["LakeArea"] >= Thres_Area_Non_Conn_Lakes
     mask2 = Non_ConnL_info[Gauge_col_Name] == 1
-    mask = np.logical_or(mask1,mask2)
-    ### process non connected selected lakes
+    mask = np.logical_or(mask1, mask2)
+    # process non connected selected lakes
     Selected_Non_ConnLakes = Non_ConnL_info[
         mask
     ]["HyLakeId"].values
     Selected_Non_ConnLakes = Selected_Non_ConnLakes[Selected_Non_ConnLakes > 0]
     Selected_Non_ConnLakes = np.unique(Selected_Non_ConnLakes)
 
-
     # selecte lake by list
     if len(Selected_Lake_List_in) > 0:
         Selected_Lake_List = Selected_Lake_List_in
     else:
         # invalide lake id, no lake will be selected by list
-        Selected_Lake_List  = [-9999999]
+        Selected_Lake_List = [-9999999]
     All_ConnL = ConnL_info["HyLakeId"].values
     All_Non_ConnL = Non_ConnL_info["HyLakeId"].values
     Selected_Lake_List_in_array = np.array(Selected_Lake_List)
 
     mask_CL = np.in1d(All_ConnL, Selected_Lake_List_in_array)
     mask_NCL = np.in1d(All_Non_ConnL, Selected_Lake_List_in_array)
 
     Selected_ConnLakes_List = All_ConnL[mask_CL]
     Selected_ConnLakes_List = np.unique(Selected_ConnLakes_List)
     Selected_Non_ConnLakes_List = All_Non_ConnL[mask_NCL]
     Selected_Non_ConnLakes_List = np.unique(Selected_Non_ConnLakes_List)
 
     # combine lake from list and area
-    Selected_Non_ConnLakes = np.concatenate((Selected_Non_ConnLakes, Selected_Non_ConnLakes_List), axis=0)
-    Selected_ConnLakes = np.concatenate((Selected_ConnLakes, Selected_ConnLakes_List), axis=0)
+    Selected_Non_ConnLakes = np.concatenate(
+        (Selected_Non_ConnLakes, Selected_Non_ConnLakes_List), axis=0)
+    Selected_ConnLakes = np.concatenate(
+        (Selected_ConnLakes, Selected_ConnLakes_List), axis=0)
 
     Un_Selected_ConnLakes_info = finalcat_info.loc[
         (finalcat_info["Lake_Cat"] == 1)
         & (np.logical_not(finalcat_info["HyLakeId"].isin(Selected_ConnLakes)))
     ]
     Un_Selected_Non_ConnL_info = finalcat_info.loc[
         (finalcat_info["Lake_Cat"] == 2)
@@ -2389,60 +2682,59 @@
         None,
     """
     mapoldnew_info = finalcat_info_temp.copy(deep=True)
     mapoldnew_info["nsubid"] = -1
     mapoldnew_info["ndownsubid"] = -1
     mapoldnew_info["nsubid2"] = mapoldnew_info["SubId"]
     mapoldnew_info.reset_index(drop=True, inplace=True)
-    ### Loop each unselected lake stream seg
+    # Loop each unselected lake stream seg
 
     Gauge_col_Name = "Has_POI"
     if "Has_POI" not in mapoldnew_info.columns:
         Gauge_col_Name = "Has_Gauge"
 
-
     Seg_IDS = Un_Selected_ConnLakes_info["Seg_ID"].values
     Seg_IDS = np.unique(Seg_IDS)
     for iseg in range(0, len(Seg_IDS)):
         #            print('#########################################################################################33333')
         i_seg_id = Seg_IDS[iseg]
         i_seg_info = finalcat_info_temp.loc[
             (finalcat_info_temp["Seg_ID"] == i_seg_id)
             & (finalcat_info_temp["Lake_Cat"] != 2)
         ].copy()
         i_seg_info = i_seg_info.sort_values(["Seg_order"], ascending=(True))
 
-        ###each part of the segment are not avaiable to be merged
+        # each part of the segment are not avaiable to be merged
         N_Hylakeid = np.unique(i_seg_info["HyLakeId"].values)
         if len(i_seg_info) == len(N_Hylakeid):
             continue
 
-        ### All lakes in this segment are removed
-        if np.max(N_Hylakeid) and np.max(i_seg_info[Gauge_col_Name].values) <= 0:  ##
+        # All lakes in this segment are removed
+        if np.max(N_Hylakeid) and np.max(i_seg_info[Gauge_col_Name].values) <= 0:
             tsubid = i_seg_info["SubId"].values[len(i_seg_info) - 1]
             seg_sub_ids = i_seg_info["SubId"].values
             mapoldnew_info = New_SubId_To_Dissolve(
                 subid=tsubid,
                 catchmentinfo=finalcat_info_temp,
                 mapoldnew_info=mapoldnew_info,
                 ismodifids=1,
                 modifiidin=seg_sub_ids,
                 mainriv=finalcat_info_temp,
                 Lake_Cat=-1,
                 seg_order=1,
             )
 
-        ### loop from the first order of the current segment
+        # loop from the first order of the current segment
         modifysubids = []
         seg_order = 1
         for iorder in range(0, len(i_seg_info)):
             tsubid = i_seg_info["SubId"].values[iorder]
             modifysubids.append(tsubid)
 
-            ### two seg has the same HyLakeId id, can be merged
+            # two seg has the same HyLakeId id, can be merged
             if iorder == len(i_seg_info) - 1:
                 seg_sub_ids = np.asarray(modifysubids)
                 mapoldnew_info = New_SubId_To_Dissolve(
                     subid=tsubid,
                     catchmentinfo=finalcat_info_temp,
                     mapoldnew_info=mapoldnew_info,
                     ismodifids=1,
@@ -2494,54 +2786,55 @@
 
     Un_Selected_Non_ConnL_info = Un_Selected_Non_ConnL_info.sort_values(
         ["DrainArea"], ascending=[False]
     )
     for i in range(0, len(Un_Selected_Non_ConnL_info)):
         Remove_Non_ConnL_Lakeid = Un_Selected_Non_ConnL_info["HyLakeId"].values[
             i
-        ]  ##select one non connected lake
+        ]  # select one non connected lake
         Remove_Non_ConnL_Lake_Sub_info = finalcat_info_temp.loc[
             finalcat_info_temp["HyLakeId"] == Remove_Non_ConnL_Lakeid
-        ].copy()  ## obtain cat info of this non connected lake catchment
+        ].copy()  # obtain cat info of this non connected lake catchment
         if len(Remove_Non_ConnL_Lake_Sub_info) != 1:
             print("It is not a non connected lake catchment")
             print(Remove_Non_ConnL_Lake_Sub_info)
             continue
-        modifysubids = []  ##array store all catchment id needs to be merged
-        csubid = Remove_Non_ConnL_Lake_Sub_info["SubId"].values[0]  ### intial subid
+        modifysubids = []  # array store all catchment id needs to be merged
+        # intial subid
+        csubid = Remove_Non_ConnL_Lake_Sub_info["SubId"].values[0]
         downsubid = Remove_Non_ConnL_Lake_Sub_info["DowSubId"].values[
             0
-        ]  ### downstream subid
-        modifysubids.append(csubid)  ### add inital subid into the list
+        ]  # downstream subid
+        modifysubids.append(csubid)  # add inital subid into the list
         tsubid = -1
         is_pre_modified = 0
 
         Down_Sub_info = finalcat_info_temp.loc[
             finalcat_info_temp["SubId"] == downsubid
-        ].copy()  ###obtain downstream infomation
+        ].copy()  # obtain downstream infomation
         if len(Down_Sub_info) == 0 and downsubid < 0:
             continue
         if Down_Sub_info["Lake_Cat"].values[0] != 2:
-            ### check if this downsubid has a new subid
+            # check if this downsubid has a new subid
             nsubid = mapoldnew_info.loc[mapoldnew_info["SubId"] == downsubid][
                 "nsubid"
             ].values[
                 0
-            ]  ## check if this catchment has modified: either merged to other catchment
+            ]  # check if this catchment has modified: either merged to other catchment
 
-            if nsubid > 0:  ### if it been already processed
-                tsubid = nsubid  ### the target catchment id will be the newsunid
-                is_pre_modified = 1  ### set is modifed to 1
-                modifysubids.append(tsubid)  ### add this subid to the list
+            if nsubid > 0:  # if it been already processed
+                tsubid = nsubid  # the target catchment id will be the newsunid
+                is_pre_modified = 1  # set is modifed to 1
+                modifysubids.append(tsubid)  # add this subid to the list
             else:
                 tsubid = downsubid
                 is_pre_modified = -1
                 modifysubids.append(tsubid)
 
-        else:  ### down stream cat is a non connected lake cat
+        else:  # down stream cat is a non connected lake cat
 
             nsubid = mapoldnew_info.loc[mapoldnew_info["SubId"] == downsubid][
                 "nsubid"
             ].values[0]
             if nsubid > 0:
                 tsubid = nsubid
                 is_pre_modified = 1
@@ -2559,15 +2852,15 @@
         if is_pre_modified > 0:
             mapoldnew_info = New_SubId_To_Dissolve(
                 subid=tsubid,
                 catchmentinfo=mapoldnew_info,
                 mapoldnew_info=mapoldnew_info,
                 ismodifids=1,
                 modifiidin=modifysubids,
-                mainriv=finalcat_info_temp,
+                mainriv=mapoldnew_info,
                 Lake_Cat=Tar_Lake_Id,
             )
         else:
             mapoldnew_info = New_SubId_To_Dissolve(
                 subid=tsubid,
                 catchmentinfo=mapoldnew_info,
                 mapoldnew_info=mapoldnew_info,
@@ -2605,24 +2898,25 @@
     mapoldnew_info = finalrivply_info.copy(deep=True)
     mapoldnew_info["nsubid"] = mapoldnew_info["SubId"].values
     mapoldnew_info['nsubid'] = mapoldnew_info['nsubid'].astype('int32')
     AllConnectLakeIDS = finalrivply_info["HyLakeId"].values
     AllConnectLakeIDS = AllConnectLakeIDS[AllConnectLakeIDS > 0]
     AllConnectLakeIDS = np.unique(AllConnectLakeIDS)
 
-    ### process connected lakes  merge polygons
+    # process connected lakes  merge polygons
     for i in range(0, len(AllConnectLakeIDS)):
         lakeid = AllConnectLakeIDS[i]
         Lakesub_info = finalrivply_info.loc[finalrivply_info["HyLakeId"] == lakeid]
-        Lakesub_info = Lakesub_info.sort_values(["DrainArea"], ascending=(False))
+        Lakesub_info = Lakesub_info.sort_values(
+            ["DrainArea"], ascending=(False))
         tsubid = Lakesub_info[sub_colnm].values[
             0
-        ]  ### outlet subbasin id with highest acc
+        ]  # outlet subbasin id with highest acc
         lakesubids = Lakesub_info[sub_colnm].values
-        if len(lakesubids) > 1:  ## only for connected lakes
+        if len(lakesubids) > 1:  # only for connected lakes
             mapoldnew_info = New_SubId_To_Dissolve(
                 subid=tsubid,
                 catchmentinfo=finalrivply_info,
                 mapoldnew_info=mapoldnew_info,
                 ismodifids=1,
                 modifiidin=lakesubids,
                 mainriv=finalrivply_info,
@@ -2643,15 +2937,15 @@
     Returns:
     -------
         None,
     """
 
     HydroBasins1 = defcat(
         routing_info, subid_downstream
-    )  ### return fid of polygons that needs to be select
+    )  # return fid of polygons that needs to be select
 
     if subid_upstream > 0:
         HydroBasins2 = defcat(routing_info, subid_upstream)
         for i in range(len(HydroBasins2)):
             if HydroBasins2[i] == subid_upstream:
                 continue
             rows = np.argwhere(HydroBasins1 == HydroBasins2[i])
@@ -2663,15 +2957,16 @@
     return HydroBasins
 
 
 def return_non_lake_inflow_segs_and_segs_within_lakes(
     riv_lake_id, str_id, riv_lake_id2, cl_id, routing_info, str_start_pt_lakeid
 ):
 
-    routing_info_rout = routing_info[["SubId", "DowSubId"]].astype("int").values
+    routing_info_rout = routing_info[[
+        "SubId", "DowSubId"]].astype("int").values
     # combine river lake id and str id and lake id
     riv_lake = np.column_stack((riv_lake_id, str_id))
     riv_lake = riv_lake[riv_lake[:, 0].argsort()]
     riv_lake_cl = np.column_stack((riv_lake_id2, cl_id))
     riv_lake_cl = riv_lake_cl[riv_lake_cl[:, 0].argsort()]
     riv_lake = np.append(riv_lake, riv_lake_cl, axis=1)
 
@@ -2686,16 +2981,16 @@
         # print(routing_info.loc[routing_info["SubId"] == strid])
         maxacc = routing_info.loc[routing_info["SubId"] == strid]["MaxAcc_cat"].values[
             0
         ]
         acc_str_cl[riv_lake[:, 1] == strid] = maxacc
     riv_lake = np.append(riv_lake, acc_str_cl, axis=1)
 
-    ## loop for each lake, identify, outlet seg, and inlet segs
-    ## and segs between outlet and inlet segs
+    # loop for each lake, identify, outlet seg, and inlet segs
+    # and segs between outlet and inlet segs
 
     non_lake_inflow_segs = []
     str_id_lake_inlfow = []
     str_id_within_lakes = []
     for i in range(0, len(cl_id_unique)):
         # obtain current lakeid
         cl_id = cl_id_unique[i]
@@ -2736,28 +3031,31 @@
             # check if there is any upstream river id in the str covered by the lake and there is some upstream
             # and the begining of the str is not located in current lake
             if str_id_cl_j != outlet_str:
                 str_id_within_lakes.append(int(riv_lake_il[j, 1]))
                 # check down stream id of the currunt str covered by the lake
                 if len(routing_info.loc[routing_info['SubId'] == str_id_cl_j]) > 0:
                     # get down stream of the corrent str covered by the lake
-                    down_sun_of_lake_cover_str = routing_info.loc[routing_info['SubId'] == str_id_cl_j]['DowSubId'].values[0]
+                    down_sun_of_lake_cover_str = routing_info.loc[routing_info['SubId']
+                                                                  == str_id_cl_j]['DowSubId'].values[0]
                     # if the it is also flow to the lake outlet , remove it
                     # and it is not already in the list
                     if down_sun_of_lake_cover_str in strs_to_lake_outlet and down_sun_of_lake_cover_str not in riv_lake_il[:, 1]:
                         # remove all dnow str unitl it reach to a lake coverd str_r
                         # or a str already be removed
-                        str_id_within_lakes.append(int(down_sun_of_lake_cover_str))
+                        str_id_within_lakes.append(
+                            int(down_sun_of_lake_cover_str))
                         #
                         cstrid = down_sun_of_lake_cover_str
-                        k_d =0
+                        k_d = 0
                         while k_d < 100:
                             k_d = k_d + 1
                             if len(routing_info.loc[routing_info['SubId'] == cstrid]) > 0:
-                                dstr_id = routing_info.loc[routing_info['SubId'] == cstrid]['DowSubId'].values[0]
+                                dstr_id = routing_info.loc[routing_info['SubId']
+                                                           == cstrid]['DowSubId'].values[0]
                                 # check if it reach a lake covered str id
                                 if dstr_id not in riv_lake_il[:, 1] and dstr_id in strs_to_lake_outlet:
                                     str_id_within_lakes.append(int(dstr_id))
                                     cstrid = dstr_id
                                 else:
                                     break
                             else:
@@ -2766,15 +3064,15 @@
             # obtain all upstream of current lake str
             up_str_cl_j = defcat(routing_info_rout, str_id_cl_j)
 
             if len(up_str_cl_j) > 0:
                 # check if there is more than 1 up stream is
                 # covreed by the lake
                 #
-                mask = np.isin(up_str_cl_j,unique_str_id_cv_by_lake)
+                mask = np.isin(up_str_cl_j, unique_str_id_cv_by_lake)
                 if sum(mask) >= 2:
                     has_up_str_inlake = True
                 else:
                     has_up_str_inlake = False
             else:
                 has_up_str_inlake = False
 
@@ -2789,90 +3087,91 @@
             ):
                 # there is some str drainge to this str,
                 # so this lake-riv seg is not the lake inflow segment
                 non_lake_inflow_segs.append(int(riv_lake_il[j, 0]))
             else:
                 str_id_lake_inlfow.append(int(riv_lake_il[j, 1]))
 
-    return list(set(str_id_within_lakes)),list(set(non_lake_inflow_segs)),list(set(str_id_lake_inlfow))
+    return list(set(str_id_within_lakes)), list(set(non_lake_inflow_segs)), list(set(str_id_lake_inlfow))
 
 
 def Check_If_Lake_Have_Multi_OutLet(CL_Id, Str_Id, Routing_info):
 
-    ### create a emppty array to store lake id with multi outlet
+    # create a emppty array to store lake id with multi outlet
     Lakes_WIth_Multi_Outlet = []
     Remove_Str = []
-    #### combine lake id and coresponding str id into two dim array
+    # combine lake id and coresponding str id into two dim array
     CL_Str = np.column_stack((CL_Id, Str_Id))
-    #### obtain unique str id
+    # obtain unique str id
     Str_Id_unique = np.unique(np.array(Str_Id))
-    #### obtain unique lake ids
+    # obtain unique lake ids
     CL_Id_unique = np.unique(np.array(CL_Id))
 
-    #### add maxacc of each str to CL_str
+    # add maxacc of each str to CL_str
     Acc_Str_CL = np.full((len(CL_Str), 1), np.nan)
     for i in range(0, len(Str_Id_unique)):
         strid = Str_Id_unique[i]
         maxacc = Routing_info.loc[Routing_info["SubId"] == strid]["MaxAcc_cat"].values[
             0
         ]
         Acc_Str_CL[CL_Str[:, 1] == strid] = maxacc
     CL_Str = np.append(CL_Str, Acc_Str_CL, axis=1)
 
-    ### sort CL_str based on max acc of
+    # sort CL_str based on max acc of
     CL_Str = CL_Str[CL_Str[:, 2].argsort()]
 
-    ### routing info
-    routing_info_only = Routing_info[["SubId", "DowSubId"]].astype("int").values
+    # routing info
+    routing_info_only = Routing_info[[
+        "SubId", "DowSubId"]].astype("int").values
     #    print(routing_info_only)
-    ### check if lakes have multi outlet
+    # check if lakes have multi outlet
     for i in range(0, len(CL_Id_unique)):
-        ### got lake id
+        # got lake id
         lake_id = CL_Id_unique[i]
-        ### got all str overlaied by this lake id
+        # got all str overlaied by this lake id
         i_CL_Str = CL_Str[CL_Str[:, 0] == lake_id]
 
-        ### lake is overlaied by one str, so must only have one lake outlet
+        # lake is overlaied by one str, so must only have one lake outlet
         if len(i_CL_Str) <= 1:
             continue
 
-        ### len(i_CL_Str)>1
-        ### check if all str covered by this lake will drainage to the str with
-        ### maximum acc. if it is ture than lake has only one outelt,
-        ### if not the lake have multi outlet
+        # len(i_CL_Str)>1
+        # check if all str covered by this lake will drainage to the str with
+        # maximum acc. if it is ture than lake has only one outelt,
+        # if not the lake have multi outlet
 
-        ###obtain str id with max acc among strs covered by the lake
+        # obtain str id with max acc among strs covered by the lake
         str_max_acc = i_CL_Str[len(i_CL_Str) - 1, 1]
         #        print(str_max_acc,len(routing_info_only),"#################")
-        ### obtain all upstream str id of max acc str
+        # obtain all upstream str id of max acc str
         str_to_str_max_acc = defcat(routing_info_only, str_max_acc)
 
         #        if len(str_to_str_max_acc) <= 1:
         #            str_to_str_max_acc = defcat(
         #                routing_info_only, i_CL_Str[len(i_CL_Str) - 2, 1]
         #            )
-        ### create a mask for i_CL_Str[:,1], it will be true for in positon
-        ### where it's value in str_to_str_max_acc
+        # create a mask for i_CL_Str[:,1], it will be true for in positon
+        # where it's value in str_to_str_max_acc
         mask = np.isin(i_CL_Str[:, 1], str_to_str_max_acc)
-        #### not all element in i_CL_Str[:,1] exist in str_to_str_max_acc
-        #### the lake have muli outlet
+        # not all element in i_CL_Str[:,1] exist in str_to_str_max_acc
+        # the lake have muli outlet
 
         Remove_Str_i = []
 
-        ### if not all str drainage to outlet str
+        # if not all str drainage to outlet str
         if len(mask[mask == True]) < len(i_CL_Str[:, 1]):
-            ### obtain strids of str not drainage to outlet str
+            # obtain strids of str not drainage to outlet str
             str_notflowto_lakeoutlet = i_CL_Str[np.logical_not(mask), 1]
-            ### loop for strids of str not drainage to outlet str
+            # loop for strids of str not drainage to outlet str
             for istr in range(0, len(str_notflowto_lakeoutlet)):
-                ### get i str id
+                # get i str id
                 strid = str_notflowto_lakeoutlet[istr]
-                ### check  streams drainage to current str
+                # check  streams drainage to current str
                 #                upstrs  = Defcat(routing_info_only,strid)
-                #### no upstream str, ### remove str instead remove lake
+                # no upstream str, ### remove str instead remove lake
                 #                if len(upstrs) == 1:
                 if strid != str_max_acc:
                     Remove_Str_i.append(strid)
 
             # if len(Remove_Str_i) == len(str_notflowto_lakeoutlet):
             #     Remove_Str = Remove_Str + Remove_Str_i
             # else:
@@ -2898,24 +3197,25 @@
     sub_colnm = "SubId"
     mapoldnew_info = finalrivply_info.copy(deep=True)
     mapoldnew_info["nsubid"] = mapoldnew_info["SubId"].values
     AllConnectLakeIDS = finalrivply_info["HyLakeId"].values
     AllConnectLakeIDS = AllConnectLakeIDS[AllConnectLakeIDS > 0]
     AllConnectLakeIDS = np.unique(AllConnectLakeIDS)
 
-    ### process connected lakes  merge polygons
+    # process connected lakes  merge polygons
     for i in range(0, len(AllConnectLakeIDS)):
         lakeid = AllConnectLakeIDS[i]
         Lakesub_info = finalrivply_info.loc[finalrivply_info["HyLakeId"] == lakeid]
-        Lakesub_info = Lakesub_info.sort_values(["DrainArea"], ascending=(False))
+        Lakesub_info = Lakesub_info.sort_values(
+            ["DrainArea"], ascending=(False))
         tsubid = Lakesub_info[sub_colnm].values[
             0
-        ]  ### outlet subbasin id with highest acc
+        ]  # outlet subbasin id with highest acc
         lakesubids = Lakesub_info[sub_colnm].values
-        if len(lakesubids) > 1:  ## only for connected lakes
+        if len(lakesubids) > 1:  # only for connected lakes
             mapoldnew_info = New_SubId_To_Dissolve(
                 subid=tsubid,
                 catchmentinfo=finalrivply_info,
                 mapoldnew_info=mapoldnew_info,
                 ismodifids=1,
                 modifiidin=lakesubids,
                 mainriv=finalrivply_info,
@@ -2964,35 +3264,36 @@
 
         mapoldnew_info["Old_SubId"] = mapoldnew_info["SubId"].values
         mapoldnew_info["Old_DowSubId"] = mapoldnew_info["DowSubId"].values
         mapoldnew_info["SubId"] = mapoldnew_info["nsubid"].values
 
         mapoldnew_info["DowSubId"] = mapoldnew_info["ndownsubid"].values
 
-
-        riv_pd_nncls_routing_info = mapoldnew_info[mapoldnew_info['Lake_Cat'] != 2].copy(deep=True)
-        mask = ~mapoldnew_info['SubId'].isin(riv_pd_nncls_routing_info['DowSubId'])
-
-        if "DA_Chn_L" in mapoldnew_info.columns:
-            mapoldnew_info.loc[mask, "DA_Chn_L"] = -1.2345
-            mapoldnew_info.loc[mask, "DA_Chn_Slp"] = -1.2345
-        mapoldnew_info.loc[mask, "RivLength"] = -1.2345
-        mapoldnew_info.loc[mask, "RivSlope"] = -1.2345
-        mapoldnew_info.loc[mask, "FloodP_n"] = -1.2345
-        mapoldnew_info.loc[mask, "Ch_n"] = -1.2345
-        mapoldnew_info.loc[mask, "Max_DEM"] = -1.2345
-        mapoldnew_info.loc[mask, "Min_DEM"] = -1.2345
-
+        riv_pd_nncls_routing_info = mapoldnew_info[mapoldnew_info['Lake_Cat'] != 2].copy(
+            deep=True)
+        mask = ~mapoldnew_info['SubId'].isin(
+            riv_pd_nncls_routing_info['DowSubId'])
+
+        # if "DA_Chn_L" in mapoldnew_info.columns:
+        #     mapoldnew_info.loc[mask, "DA_Chn_L"] = -1.2345
+        #     mapoldnew_info.loc[mask, "DA_Chn_Slp"] = -1.2345
+        # mapoldnew_info.loc[mask, "RivLength"] = -1.2345
+        # mapoldnew_info.loc[mask, "RivSlope"] = -1.2345
+        # mapoldnew_info.loc[mask, "FloodP_n"] = -1.2345
+        # mapoldnew_info.loc[mask, "Ch_n"] = -1.2345
+        # mapoldnew_info.loc[mask, "Max_DEM"] = -1.2345
+        # mapoldnew_info.loc[mask, "Min_DEM"] = -1.2345
 
     if UpdateStreamorder < 0:
         return mapoldnew_info
 
-    mapoldnew_info_unique = mapoldnew_info.drop_duplicates("SubId", keep="first")
+    mapoldnew_info_unique = mapoldnew_info.drop_duplicates(
+        "SubId", keep="first")
 
-    mapoldnew_info_unique = Streamorderanddrainagearea(mapoldnew_info_unique)
+    mapoldnew_info_unique = streamorderanddrainagearea(mapoldnew_info_unique)
 
     for i in range(0, len(mapoldnew_info_unique)):
         isubid = mapoldnew_info_unique["SubId"].values[i]
         mapoldnew_info.loc[
             mapoldnew_info["SubId"] == isubid, "Strahler"
         ] = mapoldnew_info_unique["Strahler"].values[i]
         mapoldnew_info.loc[
@@ -3021,30 +3322,30 @@
         popt2 = np.full(2, -1)
 
     return popt2[0], popt2[1]
 
 
 def calculateChannaln(width, depth, Q, slope):
     zch = 2
-    sidwd = zch * depth  ###river side width
+    sidwd = zch * depth  # river side width
     tab = "          "
-    botwd = width - 2 * sidwd  ### river
+    botwd = width - 2 * sidwd  # river
     if botwd < 0:
         botwd = 0.5 * width
         sidwd = 0.5 * 0.5 * width
         zch = (width - botwd) / 2 / depth
     Ach = botwd * depth + 2 * zch * depth * depth / 2
     #    arcpy.AddMessage(depth)
     #    arcpy.AddMessage(zch)
     #    arcpy.AddMessage(botwd)
     #    arcpy.AddMessage(width)
     #    arcpy.AddMessage(slope)
 
     Pch = botwd + 2 * depth * (1 + zch ** 2) ** 0.5
-    Rch = float(Ach) / float(Pch)  ### in meter
+    Rch = float(Ach) / float(Pch)  # in meter
     V = float(Q) / float(Ach)
     if V > 0:
         n = (Rch ** (2.0 / 3.0)) * (slope ** (1.0 / 2.0)) / V
     else:
         n = -1.2345
     return n
 
@@ -3058,89 +3359,92 @@
 
     Gauge_col_Name = "Has_POI"
     if "Has_POI" not in catinfo.columns:
         Gauge_col_Name = "Has_Gauge"
 
     if path_sub_reg_outlets_v != "#":
 
-        Sub_reg_outlets = Dbf_To_Dataframe(path_sub_reg_outlets_v)["reg_subid"].values
+        Sub_reg_outlets = Dbf_To_Dataframe(path_sub_reg_outlets_v)[
+            "reg_subid"].values
         Sub_reg_outlets_ids = np.unique(Sub_reg_outlets)
         Sub_reg_outlets_ids = Sub_reg_outlets_ids[Sub_reg_outlets_ids > 0]
 
-        #### Find all obervation id that is subregion outlet
-        reg_outlet_info = catinfo.loc[catinfo[Gauge_col_Name].isin(Sub_reg_outlets_ids)]
+        # Find all obervation id that is subregion outlet
+        reg_outlet_info = catinfo.loc[catinfo[Gauge_col_Name].isin(
+            Sub_reg_outlets_ids)]
 
-        #### Define outlet ID
+        # Define outlet ID
         outletid = -1
 
         if outlet_obs_id < 0:
             print("To use subregion, the Subregion Id MUST provided as Outlet_Obs_ID")
             return catinfo
 
         outletID_info = catinfo.loc[catinfo[Gauge_col_Name] == outlet_obs_id]
         if len(outletID_info) > 0:
             outletid = outletID_info["SubId"].values[0]
         else:
             print("No Outlet id is founded for subregion   ", outletID_info)
             return catinfo
 
-        ### find all subregion drainge to this outlet id
+        # find all subregion drainge to this outlet id
         HydroBasins1 = defcat(routing_info, outletid)
-        ### if there is other subregion outlet included in current sturcture
-        ### remove subbasins drainge to them
+        # if there is other subregion outlet included in current sturcture
+        # remove subbasins drainge to them
 
-        if len(reg_outlet_info) >= 2:  ### has upstream regin outlet s
-            ### remove subbains drainage to upstream regin outlet s
+        if len(reg_outlet_info) >= 2:  # has upstream regin outlet s
+            # remove subbains drainage to upstream regin outlet s
             for i in range(0, len(reg_outlet_info)):
                 upregid = reg_outlet_info["SubId"].values[i]
-                ### the subregion ouetlet not within the target domain neglect
+                # the subregion ouetlet not within the target domain neglect
                 if upregid == outletid or np.sum(np.in1d(HydroBasins1, upregid)) < 1:
                     continue
                 HydroBasins_remove = defcat(routing_info, upregid)
                 mask = np.in1d(
                     HydroBasins1, HydroBasins_remove
-                )  ### exluced ids that belongs to main river stream
+                )  # exluced ids that belongs to main river stream
                 HydroBasins1 = HydroBasins1[np.logical_not(mask)]
         HydroBasins = HydroBasins1
 
         catinfo = catinfo.loc[catinfo["SubId"].isin(HydroBasins)]
         return catinfo
-    ### selected based on observation guage obs id
+    # selected based on observation guage obs id
     else:
         outletid = -1
         outletID_info = catinfo.loc[catinfo[Gauge_col_Name] == outlet_obs_id]
         if len(outletID_info) > 0:
             outletid = outletID_info["SubId"].values[0]
-            ##find upsteam catchment id
+            # find upsteam catchment id
             HydroBasins = defcat(routing_info, outletid)
         else:
             HydroBasins = catinfo["SubId"].values
 
         catinfo = catinfo.loc[catinfo["SubId"].isin(HydroBasins)]
         return catinfo
 
-def create_grid_weight_main(Mapforcing,Forcinfo):
+
+def create_grid_weight_main(Mapforcing, Forcinfo):
 
     grid_weight_string_list = []
     hruids = Mapforcing["HRU_ID"].values
     hruids = np.unique(hruids)
     #    Lakeids = np.unique(Lakeids)
     grid_weight_string_list = []
 
     os.environ["JOBLIB_TEMP_FOLDER"] = tempfile.gettempdir()
 
-
     grid_weight_string_list.append(":GridWeights")
     grid_weight_string_list.append("   #      ")
     grid_weight_string_list.append("   # [# HRUs]")
 
     sNhru = len(hruids)
     grid_weight_string_list.append("   :NumberHRUs       " + str(sNhru))
 
-    sNcell = (max(Forcinfo["Row"].values) + 1) * (max(Forcinfo["Col"].values) + 1)
+    sNcell = (max(Forcinfo["Row"].values) + 1) * \
+        (max(Forcinfo["Col"].values) + 1)
     grid_weight_string_list.append("   :NumberGridCells  " + str(sNcell))
     grid_weight_string_list.append("   #            ")
     grid_weight_string_list.append("   # [HRU ID] [Cell #] [w_kl]")
     max_col = max(Forcinfo["Col"].values)
     Avafgid = Forcinfo["FGID"].values
     # for id in hruids:
     #     grid_weight_string_ihru = create_grid_weight_hru(i,Mapforcing,Forcinfo)
@@ -3148,24 +3452,26 @@
     n_hru_group = int(len(hruids)/10)
 
     if len(hruids) > 1000:
         hru_ids_groups = np.array_split(hruids, n_hru_group)
     else:
         hru_ids_groups = [hruids]
 
-    for i in range(0,len(hru_ids_groups)):
+    for i in range(0, len(hru_ids_groups)):
         i_hru_group = hru_ids_groups[i]
-        grid_weight_string_hrusi = Parallel(n_jobs=4)(delayed(create_grid_weight_hru)(i,Mapforcing.copy(deep=True),Avafgid,max_col) for i in i_hru_group)
+        grid_weight_string_hrusi = Parallel(n_jobs=4)(delayed(create_grid_weight_hru)(
+            i, Mapforcing.copy(deep=True), Avafgid, max_col) for i in i_hru_group)
         grid_weight_string_list = grid_weight_string_list + grid_weight_string_hrusi
 
     grid_weight_string_list.append(":EndGridWeights")
     grid_weight_string = "\n".join(grid_weight_string_list)
     return grid_weight_string
 
-def create_grid_weight_hru(hruid,Mapforcing,Avafgid,max_col):
+
+def create_grid_weight_hru(hruid, Mapforcing, Avafgid, max_col):
 
     grid_weight_string_hru = ' '
 
     cats = Mapforcing.loc[Mapforcing["HRU_ID"] == hruid].copy(deep=True)
 
 #    cats = cats_hru[cats_hru["Map_FGID"].isin(Avafgid)].copy(deep=True)
 
@@ -3184,15 +3490,15 @@
         if j < len(fids) - 1:
             sarea = sum(scat["s_area"].values)
             wt = float(sarea) / float(tarea)
             sumwt = sumwt + wt
         else:
             wt = 1 - sumwt
 
-        if len(scat["Map_Row"].values) > 1:  ## should be 1
+        if len(scat["Map_Row"].values) > 1:  # should be 1
             print(
                 str(catid)
                 + "error: 1 hru, 1 grid, produce muti polygon need to be merged "
             )
             Strcellid = (
                 str(
                     int(
@@ -3211,15 +3517,19 @@
                         * (max_col + 1)
                         + scat["Map_Col"].values[0]
                     )
                 )
                 + "      "
             )
         if len(fids) == 1:
-            grid_weight_string_hru = grid_weight_string_hru + "    " + str(int(hruid)) + "     " + Strcellid + "      " + str(wt)
+            grid_weight_string_hru = grid_weight_string_hru + "    " + \
+                str(int(hruid)) + "     " + Strcellid + "      " + str(wt)
         else:
-            if j  == len(fids) - 1:
-                grid_weight_string_hru = grid_weight_string_hru + "    " + str(int(hruid)) + "     " + Strcellid + "      " + str(wt)
+            if j == len(fids) - 1:
+                grid_weight_string_hru = grid_weight_string_hru + "    " + \
+                    str(int(hruid)) + "     " + Strcellid + "      " + str(wt)
             else:
-                grid_weight_string_hru = grid_weight_string_hru + "    " + str(int(hruid)) + "     " + Strcellid + "      " + str(wt) + "\n"
+                grid_weight_string_hru = grid_weight_string_hru + "    " + \
+                    str(int(hruid)) + "     " + Strcellid + \
+                    "      " + str(wt) + "\n"
 
     return grid_weight_string_hru
```

### Comparing `basinmaker-3.0.3a0/basinmaker/func/purepy.py` & `basinmaker-3.1.0/basinmaker/func/purepy.py`

 * *Files 27% similar despite different names*

```diff
@@ -6,15 +6,14 @@
 import json
 import requests
 import sys
 #import shapely.wkt
 #import pygeos as pg
 from osgeo import gdal, ogr
 from rasterstats import zonal_stats
-
 def zonal_stats_pd(shp_gpd,raster,stats,key):
 
     result = zonal_stats(shp_gpd, raster, stats = stats,geojson_out=True,all_touched=True)
 
     reault_list_dic = list(map(lambda x : {key:x['properties'][key],'mean':x['properties']['mean']}, result))
 
     reault_pd = pd.DataFrame(reault_list_dic)
@@ -125,24 +124,27 @@
     return cleaned
 
 
 def save_modified_attributes_to_outputs(mapoldnew_info,tempfolder,OutputFolder,cat_name,riv_name,Path_final_riv,dis_col_name='SubId'):
 
 
     NEED_TO_REMOVE_IDS = ["SubId_1", "Id","nsubid2", "nsubid","ndownsubid","Old_SubId","Old_DowSub","Join_Count","TARGET_FID","Id","SubID_Oldr","HRU_ID_N_1","HRU_ID_N_2","facters","Old_DowSubId","SubIdt2"]
-
+    obs_error_name = 'DA_error'
+    if 'DA_Diff' in mapoldnew_info.columns:
+        obs_error_name = 'DA_Diff'
+    
     #obtain readme file
     if "DA_Chn_L" in  mapoldnew_info.columns:
         url = 'https://github.com/dustming/RoutingTool/wiki/Files/README_OIH.pdf'
     else:
         url = 'https://github.com/dustming/RoutingTool/wiki/Files/README_NA.pdf'
 
-    response = requests.get(url)
-    with open(os.path.join(OutputFolder,"README.pdf"), 'wb') as f:
-        f.write(response.content)
+    # response = requests.get(url)
+    # with open(os.path.join(OutputFolder,"README.pdf"), 'wb') as f:
+    #     f.write(response.content)
 
     if riv_name != '#':
 
         if Path_final_riv != '#':
             riv_pd = geopandas.read_file(Path_final_riv)
             riv_pd['Old_SubId'] = riv_pd['SubId']
 
@@ -157,34 +159,41 @@
         mapoldnew_info = mapoldnew_info.dissolve(by=dis_col_name, aggfunc='first',as_index=False)
         mapoldnew_info = add_centroid_in_wgs84(mapoldnew_info,"centroid_x","centroid_y")
 
         cat_c_x_y = mapoldnew_info[["centroid_y","centroid_x"]].copy(deep=True)
         if Path_final_riv != '#':
             riv_pd = riv_pd.drop(columns = ["centroid_y","centroid_x"])
             riv_pd = riv_pd.join(cat_c_x_y)
-
-        riv_pd_nncls_routing_info = mapoldnew_info[mapoldnew_info['Lake_Cat'] != 2][['SubId','DowSubId']].copy(deep=True)
-        remove_channel = []
-        for subid in riv_pd_nncls_routing_info['SubId'].values:
-            if subid not in riv_pd_nncls_routing_info['DowSubId'].values:
-                remove_channel.append(subid)
+            riv_pd = riv_pd[mapoldnew_info.columns]        
+        remove_subids = [-9999]
+        
+        if 'river_without_merging_lakes' not in riv_name:
+            riv_pd_nncls_routing_info = mapoldnew_info[['SubId','DowSubId']].copy(deep=True)
+            remove_subids = riv_pd_nncls_routing_info[ ~riv_pd_nncls_routing_info['SubId'].isin(mapoldnew_info['DowSubId'].values)]['SubId'].values
         if Path_final_riv != '#':
-            riv_pd = riv_pd[~riv_pd.SubId.isin(remove_channel)]
+            riv_pd = riv_pd[~riv_pd.SubId.isin(remove_subids)]
             cat_colnms = riv_pd.columns
             drop_cat_colnms = cat_colnms[cat_colnms.isin(NEED_TO_REMOVE_IDS)]
             riv_pd = riv_pd.drop(columns=drop_cat_colnms)
             if len(riv_pd) > 0:
                 riv_pd.to_file(os.path.join(OutputFolder,riv_name))
 
-        mapoldnew_info.loc[mapoldnew_info.SubId.isin(remove_channel),'RivSlope'] = -1.2345
-        mapoldnew_info.loc[mapoldnew_info.SubId.isin(remove_channel),'RivLength'] = -1.2345
-        mapoldnew_info.loc[mapoldnew_info.SubId.isin(remove_channel),'FloodP_n'] = -1.2345
-        mapoldnew_info.loc[mapoldnew_info.SubId.isin(remove_channel),'Ch_n'] = -1.2345
-        mapoldnew_info.loc[mapoldnew_info.SubId.isin(remove_channel),'Max_DEM'] = -1.2345
-        mapoldnew_info.loc[mapoldnew_info.SubId.isin(remove_channel),'Min_DEM'] = -1.2345
+        if 'finalcat_info' in cat_name:                
+            mapoldnew_info.loc[mapoldnew_info.SubId.isin(remove_subids),'RivSlope'] = -1.2345
+            mapoldnew_info.loc[mapoldnew_info.SubId.isin(remove_subids),'RivLength'] = -1.2345
+            mapoldnew_info.loc[mapoldnew_info.SubId.isin(remove_subids),'FloodP_n'] = -1.2345
+            mapoldnew_info.loc[mapoldnew_info.SubId.isin(remove_subids),'Ch_n'] = -1.2345
+            mapoldnew_info.loc[mapoldnew_info.SubId.isin(remove_subids),'Max_DEM'] = -1.2345
+            mapoldnew_info.loc[mapoldnew_info.SubId.isin(remove_subids),'Min_DEM'] = -1.2345
+            mapoldnew_info.loc[mapoldnew_info['Lake_Cat'] > 0,'RivSlope'] = -1.2345
+            mapoldnew_info.loc[mapoldnew_info['Lake_Cat'] > 0,'RivLength'] = -1.2345
+            mapoldnew_info.loc[mapoldnew_info['Lake_Cat'] > 0,'FloodP_n'] = -1.2345
+            mapoldnew_info.loc[mapoldnew_info['Lake_Cat'] > 0,'Ch_n'] = -1.2345
+            mapoldnew_info.loc[mapoldnew_info['Lake_Cat'] > 0,'Max_DEM'] = -1.2345
+            mapoldnew_info.loc[mapoldnew_info['Lake_Cat'] > 0,'Min_DEM'] = -1.2345
 
         cat_colnms = mapoldnew_info.columns
         drop_cat_colnms = cat_colnms[cat_colnms.isin(NEED_TO_REMOVE_IDS)]
         mapoldnew_info = mapoldnew_info.drop(columns=drop_cat_colnms)
         mapoldnew_info.to_file(os.path.join(OutputFolder,cat_name))
 
         outline = create_watershed_boundary(mapoldnew_info)
@@ -208,15 +217,14 @@
             mapoldnew_info.loc[mapoldnew_info.SubId.isin(remove_channel),'RivSlope'] = -1.2345
             mapoldnew_info.loc[mapoldnew_info.SubId.isin(remove_channel),'RivLength'] = -1.2345
             mapoldnew_info.loc[mapoldnew_info.SubId.isin(remove_channel),'FloodP_n'] = -1.2345
             mapoldnew_info.loc[mapoldnew_info.SubId.isin(remove_channel),'Ch_n'] = -1.2345
             mapoldnew_info.loc[mapoldnew_info.SubId.isin(remove_channel),'Max_DEM'] = -1.2345
             mapoldnew_info.loc[mapoldnew_info.SubId.isin(remove_channel),'Min_DEM'] = -1.2345
 
-
         cat_colnms = mapoldnew_info.columns
         drop_cat_colnms = cat_colnms[cat_colnms.isin(["SHAPE","SubId_1", "Id","nsubid2", "nsubid","ndownsubid","Old_DowSub","Join_Count","TARGET_FID","Id","SubID_Oldr","HRU_ID_N_1","HRU_ID_N_2","facters","Old_DowSubId"])]
         mapoldnew_info = mapoldnew_info.drop(columns=drop_cat_colnms)
         mapoldnew_info.to_file(os.path.join(OutputFolder,cat_name))
         outline = create_watershed_boundary(mapoldnew_info)
         outline.to_file(os.path.join(OutputFolder,"outline.shp"))
         return mapoldnew_info
@@ -415,7 +423,66 @@
             else:
                 output_jason_lake_riv['features'] += injson2['features']
 
         with open(os.path.join(product_dir,'routing_product_lake_river.geojson'), 'w', encoding='utf-8') as f:
             json.dump(output_jason_lake_riv, f, ensure_ascii=False, indent=4)
 
     return
+
+
+def compare_catchment(cat_a,cat_b):
+    """test function that will:
+    Function that used to compare two catchment files
+    from routing products
+    """
+
+    ### transfer expected siplified product into pandas dataframe
+    Expect_Finalriv_info_ply = geopandas.read_file(cat_a).sort_values(by=["SubId"])
+    ### calcuate expected total number of catchment:Expect_N_Cat
+    Expect_N_Cat = len(Expect_Finalriv_info_ply)
+    ### calcuate expected total river length :Expect_len_Riv
+    Expect_len_Riv = sum(Expect_Finalriv_info_ply["RivLength"])
+    ### calcuate expected total basin area :Expect_Bas_Area
+    Expect_Bas_Area = sum(Expect_Finalriv_info_ply["BasArea"])
+
+    ### transfer resulted siplified product into pandas dataframe
+    Result_Finalriv_info_ply = geopandas.read_file(cat_b).sort_values(by=["SubId"])
+    ### calcuate resulted total number of catchment:Result_N_Cat
+    Result_N_Cat = len(Result_Finalriv_info_ply)
+    ### calcuate resulted total river length :Result_len_Riv
+    Result_len_Riv = sum(Result_Finalriv_info_ply["RivLength"])
+    ### calcuate resulted total basin area :Result_Bas_Area
+    Result_Bas_Area = sum(Result_Finalriv_info_ply["BasArea"])
+
+    ### compare Expect_N_Cat and Result_N_Cat
+    assert Expect_N_Cat == Result_N_Cat
+    ### compare Expect_len_Riv and Result_len_Riv
+    assert (Expect_len_Riv  - Result_len_Riv) < 1    ### compare Expect_Bas_Area and Result_Bas_Area
+    assert (Expect_Bas_Area - Result_Bas_Area) < 10
+    
+def compare_products(product_folder_a,product_folder_b):
+    compare_catchment(os.path.join(product_folder_a,'catchment_without_merging_lakes_v1-0.shp'),os.path.join(product_folder_b,'catchment_without_merging_lakes_v1-0.shp'))
+
+    if os.path.exists(os.path.join(product_folder_a,'finalcat_info_v1-0.shp')):
+        compare_catchment(os.path.join(product_folder_a,'finalcat_info_v1-0.shp'),os.path.join(product_folder_b,'finalcat_info_v1-0.shp'))
+
+
+def compare_hrus(hru_folder_a,hru_folder_b):
+        ### transfer expected siplified product into pandas dataframe
+    hru_a = geopandas.read_file(hru_folder_a).sort_values(by=["HRU_ID"])
+    ### calcuate expected total number of catchment:Expect_N_Cat
+    Expect_N_HRU = len(hru_a)
+    ### calcuate expected total basin area :Expect_Bas_Area
+    Expect_HRU_Area = sum(hru_a["HRU_Area"])
+
+    ### transfer resulted siplified product into pandas dataframe
+    Result_Finalriv_info_ply = geopandas.read_file(hru_folder_b).sort_values(by=["HRU_ID"])
+    ### calcuate resulted total number of catchment:Result_N_Cat
+    Result_N_HRU = len(Result_Finalriv_info_ply)
+    ### calcuate resulted total basin area :Result_Bas_Area
+    Result_HRU_Area = sum(Result_Finalriv_info_ply["HRU_Area"])
+
+    ### compare Expect_N_Cat and Result_N_Cat
+    assert Expect_N_HRU == Result_N_HRU
+    ### compare Expect_len_Riv and Result_len_Riv
+    assert (Expect_HRU_Area  - Result_HRU_Area) < 1    ### compare Expect_Bas_Area and Result_Bas_Area
+
```

### Comparing `basinmaker-3.0.3a0/basinmaker/func/qgis.py` & `basinmaker-3.1.0/basinmaker/func/qgis.py`

 * *Files identical despite different names*

### Comparing `basinmaker-3.0.3a0/basinmaker/func/rarray.py` & `basinmaker-3.1.0/basinmaker/func/rarray.py`

 * *Files identical despite different names*

### Comparing `basinmaker-3.0.3a0/basinmaker/hymodin/raveninput.py` & `basinmaker-3.1.0/basinmaker/hymodin/raveninput.py`

 * *Files identical despite different names*

### Comparing `basinmaker-3.0.3a0/basinmaker/postprocessing/assigninterestsites.py` & `basinmaker-3.1.0/basinmaker/postprocessing/assigninterestsites.py`

 * *Files 13% similar despite different names*

```diff
@@ -63,29 +63,44 @@
     # read attribute table, and
     Path_final_rviply = Path_final_riv_ply
     Path_final_riv = Path_final_riv
     Path_Conl_ply = Path_Con_Lake_ply
     Path_Non_ConL_ply = Path_NonCon_Lake_ply
 
     finalriv_infoply = geopandas.read_file(Path_final_rviply)
-    cat_ply = finalriv_infoply.drop(columns=['DA_Obs','SRC_obs','Obs_NM']).copy(deep=True)
+
+    # For ECCC and other product we still use DA_error
+    DA_ERR_COL = 'DA_error'
+    if DA_ERR_COL not in finalriv_infoply.columns:
+        DA_ERR_COL = 'DA_Diff'
+
+    # Remove DA_Obs and DA_Diff columns from subbasin layer
+    for col in ['DA_Obs', DA_ERR_COL]:
+        if col in finalriv_infoply.columns:
+            finalriv_infoply = finalriv_infoply.drop(columns=[col])
+        else:
+            pass
+
+    cat_ply = finalriv_infoply.drop(columns=['Obs_NM', 'SRC_obs']).copy(deep=True)
 
     if clean_exist_pois:
         finalriv_infoply["Has_POI"] = 0
         finalriv_infoply["SRC_obs"] = "nan"
         finalriv_infoply["Obs_NM"]  = "nan"
-        finalriv_infoply["DA_Obs"] = 0
-        finalriv_infoply["DA_error"] = -1.2345
+        # finalriv_infoply["DA_Obs"] = -1.2345
+        # finalriv_infoply[DA_ERR_COL] = -999
 
     interest_site = geopandas.read_file(path_to_points_of_interest_points)
     interest_site = interest_site.to_crs(cat_ply.crs)
     interest_site = interest_site.sjoin(cat_ply, how="left")
     non_lake = interest_site[interest_site["Type"] == "River"].copy(deep=True)
     lake     = interest_site[interest_site["Type"] == "Lake"].copy(deep=True)
 
+    # print(interest_site.columns)
+
     if len(non_lake) > 0:
         if len(non_lake[non_lake["Lake_Cat"] == 1]) > 0:
             print("Folllowing river gauges are located in the lake, they will be ignored")
             print(non_lake[non_lake["Lake_Cat"] == 1]["Obs_NM"].values)
             non_lake = non_lake[non_lake["Lake_Cat"] == 0].copy(deep=True)
 
     if len(lake) > 0:
@@ -101,48 +116,55 @@
     sub_of_interested_lake_outlet = sub_of_interested_lake.drop_duplicates(subset=['HyLakeId'],keep='first')
     interest_subids_lake = sub_of_interested_lake_outlet[["SubId","HyLakeId"]]
     interest_subids_lake["Lake_Outlet"] = interest_subids_lake["SubId"]
     interest_subids_lake = interest_subids_lake.drop(columns='SubId')
     lake = lake.merge(interest_subids_lake,on='HyLakeId',how='left')
     lake["SubId"] = lake["Lake_Outlet"]
     lake = lake.drop(columns='Lake_Outlet')
-    poi_subs = non_lake.append(lake)
+    poi_subs = pd.concat([non_lake, lake])
     poi_subs = poi_subs.reset_index()
 
     if Path_obs_gauge_point != "#":
         exist_poi = geopandas.read_file(Path_obs_gauge_point)
         exist_poi = exist_poi[["Obs_NM","geometry",'DA_Obs','SRC_obs','DrainArea']].copy(deep=True)
         cat_table = finalriv_infoply[['Obs_NM','SubId']].copy(deep=True)
         exist_poi = exist_poi.merge(cat_table,on='Obs_NM',how='left')
-
     else:
         exist_poi = poi_subs[["Obs_NM","geometry",'DA_Obs','SRC_obs','DrainArea','SubId']].copy(deep=True)
 
     for index in poi_subs.index:
 
         trg_SubId = poi_subs.loc[index,"SubId"]
         SRC_obs_in = poi_subs.loc[index,"SRC_obs"]
         Obs_NM_in =  poi_subs.loc[index,"Obs_NM"]
-        DA_Obs_in =  poi_subs.loc[index,"DA_Obs"]
+        # DA_Obs_in =  poi_subs.loc[index,"DA_Obs"]
         row = poi_subs[poi_subs.index == index]
-
+        if np.isnan(trg_SubId):
+            print("POI: ",Obs_NM_in,"   is not located in any subbasin, please check the location of this POI")
+            continue
         trg_sub_info = finalriv_infoply[finalriv_infoply["SubId"] == trg_SubId].copy(deep=True)
         Cur_SRC_obs  =  trg_sub_info.loc[finalriv_infoply["SubId"] == trg_SubId,"SRC_obs"].values[0]
         Cur_Obs_NM   =  trg_sub_info.loc[finalriv_infoply["SubId"] == trg_SubId,"Obs_NM"].values[0]
 
+        # Initialze this variable
+        # DAerror_in   = -999    
         # no point is here
         if len(exist_poi) < 0:
             finalriv_infoply.loc[finalriv_infoply["SubId"] == trg_SubId,"SRC_obs"] = SRC_obs_in
             finalriv_infoply.loc[finalriv_infoply["SubId"] == trg_SubId,"Obs_NM"] = Obs_NM_in
-            finalriv_infoply.loc[finalriv_infoply["SubId"] == trg_SubId,"SRC_obs"] = DA_Obs_in
+            # finalriv_infoply.loc[finalriv_infoply["SubId"] == trg_SubId,"DA_Obs"] = DA_Obs_in
             finalriv_infoply.loc[finalriv_infoply["SubId"] == trg_SubId,"Has_POI"] = 1
-            if DA_Obs_in > 0 :
-                DAerror_in = finalriv_infoply.loc[finalriv_infoply["SubId"] == trg_SubId,"DrainArea"]/1000/1000/DA_Obs_in
-                finalriv_infoply.loc[finalriv_infoply["SubId"] == trg_SubId,"DA_error"] = DAerror_in
-            continue
+            # if DA_Obs_in > 0 :
+            #     da_sim = finalriv_infoply.loc[finalriv_infoply["SubId"] == trg_SubId,"DrainArea"].values[0]
+            #     if DA_ERR_COL == 'DA_error':
+            #         DAerror_in = da_sim/1000/1000/DA_Obs_in
+            #     else:
+            #         DAerror_in = (da_sim/1000/1000 - DA_Obs_in)/DA_Obs_in
+            #     finalriv_infoply.loc[finalriv_infoply["SubId"] == trg_SubId,DA_ERR_COL] = DAerror_in
+            # continue
 
         # the subbasin already contain the ObsNM
         if Obs_NM_in in Cur_Obs_NM:
             print("The POI ",Obs_NM_in,"Already exists")
             continue
 
         # Obs_NM not in current subbasin but in other subbasins
@@ -154,52 +176,92 @@
             exist_poi = exist_poi.reset_index(drop=True)
 
             mask_point = exist_poi["Obs_NM"] == Obs_NM_in
 
             finalriv_infoply.loc[mask_cat,"Obs_NM"] = "nan"
             finalriv_infoply.loc[mask_cat,"SRC_obs"] = "nan"
             finalriv_infoply.loc[mask_cat,"Has_POI"] = 0
-            finalriv_infoply.loc[mask_cat,"DA_Obs"] = 0
-            finalriv_infoply.loc[mask_cat,"DA_error"] = -1.2345
+            # finalriv_infoply.loc[mask_cat,"DA_Obs"] = -1.2345
+            # finalriv_infoply.loc[mask_cat,DA_ERR_COL] = -999
             exist_poi=exist_poi.drop(exist_poi.index[mask_point])
             print("The existing : ",Obs_NM_in," in the product is removed")
 
         if trg_sub_info["Has_POI"].values[0] <= 0:
             finalriv_infoply.loc[finalriv_infoply["SubId"] == trg_SubId,"SRC_obs"] = SRC_obs_in
             finalriv_infoply.loc[finalriv_infoply["SubId"] == trg_SubId,"Obs_NM"] = Obs_NM_in
-            finalriv_infoply.loc[finalriv_infoply["SubId"] == trg_SubId,"DA_Obs"] = DA_Obs_in
             finalriv_infoply.loc[finalriv_infoply["SubId"] == trg_SubId,"Has_POI"] = 1
-            if DA_Obs_in > 0 :
-                DAerror_in = finalriv_infoply.loc[finalriv_infoply["SubId"] == trg_SubId,"DrainArea"]/1000/1000/DA_Obs_in
-                finalriv_infoply.loc[finalriv_infoply["SubId"] == trg_SubId,"DA_error"] = DAerror_in
-            exist_poi = exist_poi.append(row[["Obs_NM","geometry",'DA_Obs','SRC_obs','DrainArea','SubId']])
+            
+            # finalriv_infoply.loc[finalriv_infoply["SubId"] == trg_SubId,"DA_Obs"] = DA_Obs_in
+            # finalriv_infoply.loc[finalriv_infoply["SubId"] == trg_SubId,"Has_POI"] = 1
+            # if DA_Obs_in > 0 :
+            #     da_sim = finalriv_infoply.loc[finalriv_infoply["SubId"] == trg_SubId,"DrainArea"].values[0]
+            #     if DA_ERR_COL == 'DA_error':
+            #         DAerror_in = da_sim/1000/1000/DA_Obs_in
+            #     else:
+            #         DAerror_in = (da_sim/1000/1000 - DA_Obs_in)/DA_Obs_in
+            #     finalriv_infoply.loc[finalriv_infoply["SubId"] == trg_SubId,DA_ERR_COL] = DAerror_in
+
+
+            exist_poi = pd.concat([exist_poi, row[["Obs_NM","geometry",'DA_Obs','SRC_obs','DrainArea','SubId']]])
             print("Add the POI : ",Obs_NM_in," into the routing product ")
 
         else:
+            ## POI in this subbasin
 
-            if SRC_obs_in != "nan":
-                SRC_obs_in  =  Cur_SRC_obs+"&" + SRC_obs_in
-            else:
-                SRC_obs_in  = Cur_SRC_obs
+            SRC_obs_in  =  Cur_SRC_obs+ "&" + SRC_obs_in
+            Obs_NM_in   =   Cur_Obs_NM + "&" + Obs_NM_in
 
-            Obs_NM_in   =   Cur_Obs_NM+"&" + Obs_NM_in
 
             finalriv_infoply.loc[finalriv_infoply["SubId"] == trg_SubId,"SRC_obs"] = SRC_obs_in
             finalriv_infoply.loc[finalriv_infoply["SubId"] == trg_SubId,"Obs_NM"] = Obs_NM_in
             finalriv_infoply.loc[finalriv_infoply["SubId"] == trg_SubId,"Has_POI"] = 1
-#            row["Obs_NM"] = Obs_NM_in
-#            exist_poi.loc[exist_poi["Obs_NM"] == Cur_Obs_NM ,"Obs_NM"] = Obs_NM_in
-            exist_poi = exist_poi.append(row[["Obs_NM","geometry",'DA_Obs','SRC_obs','DrainArea','SubId']])
-            print("Append the POI : ",Obs_NM_in," into the routing product ")
 
+            # finalriv_infoply.loc[finalriv_infoply["SubId"] == trg_SubId,"DA_Obs"] = DA_Obs_in
+            # finalriv_infoply.loc[finalriv_infoply["SubId"] == trg_SubId,"Has_POI"] = 1
+            # if DA_Obs_in > 0 :
+            #     da_sim = finalriv_infoply.loc[finalriv_infoply["SubId"] == trg_SubId,"DrainArea"].values[0]
+            #     if DA_ERR_COL == 'DA_error':
+            #         DAerror_in = da_sim/1000/1000/DA_Obs_in
+            #     else:
+            #         DAerror_in = (da_sim/1000/1000 - DA_Obs_in)/DA_Obs_in
+
+            #     finalriv_infoply.loc[finalriv_infoply["SubId"] == trg_SubId,DA_ERR_COL] = DAerror_in
+
+            # else:
+            #     finalriv_infoply.loc[finalriv_infoply["SubId"] == trg_SubId,DA_ERR_COL] = -999
+
+            # row["Obs_NM"] = Obs_NM_in
+            # exist_poi.loc[exist_poi["Obs_NM"] == Cur_Obs_NM ,"Obs_NM"] = Obs_NM_in
+
+            exist_poi = pd.concat([exist_poi, row[["Obs_NM","geometry",'DA_Obs','SRC_obs','DrainArea','SubId']]])
+
+            print("Append POI : ", Obs_NM_in , ',' ,  SRC_obs_in )
+    
+    # Output subbasin layer
     finalriv_infoply.to_file(os.path.join(OutputFolder,os.path.basename(Path_final_riv_ply)))
 
     # cat_table = finalriv_infoply.drop(columns=["geometry",'DA_Obs','SRC_obs','DrainArea'])
     # exist_poi = exist_poi.merge(cat_table,on='Obs_NM',how='left')
-    exist_poi = exist_poi[["geometry",'DA_Obs','SRC_obs','Obs_NM','SubId','DrainArea']].copy(deep=True)
+    exist_poi['Use_region'] = 1
+    exist_poi[DA_ERR_COL]   = -999
+    mask = exist_poi["DA_Obs"] > 0 
+
+    if DA_ERR_COL == 'DA_error':
+        exist_poi.loc[mask,DA_ERR_COL] = exist_poi.loc[mask,'DrainArea']/1000/1000/exist_poi.loc[mask,'DA_Obs']                                                                           
+    else:
+        exist_poi.loc[mask,DA_ERR_COL] = (exist_poi.loc[mask,'DrainArea']/1000/1000 - exist_poi.loc[mask,'DA_Obs'])/exist_poi.loc[mask,'DA_Obs']                                                                          
+
+    exist_poi = exist_poi[['SubId','Obs_NM','DA_Obs','DrainArea',DA_ERR_COL,'SRC_obs','Use_region','geometry']].copy(deep=True)
+
+    # Revise DA_Diff column type and value format
+    exist_poi.loc[exist_poi['DA_Obs'] <= 0,DA_ERR_COL] = -999
+    # non-null values are shown as percentage
+    if DA_ERR_COL == 'DA_Diff':
+        exist_poi[DA_ERR_COL] = exist_poi[DA_ERR_COL].apply(lambda x: f"{x*100:.3f}%" if x != -999 else "<NA>")
+    exist_poi.loc[exist_poi['DA_Obs'] <= 0, 'DA_Obs'] = -1.2345
 
     if Path_obs_gauge_point != "#":
         exist_poi.to_file(os.path.join(OutputFolder,os.path.basename(Path_obs_gauge_point)))
     else:
         exist_poi.to_file(os.path.join(OutputFolder,"poi"+"_v1-0"+".shp"))
```

### Comparing `basinmaker-3.0.3a0/basinmaker/postprocessing/combine.py` & `basinmaker-3.1.0/basinmaker/postprocessing/combine.py`

 * *Files identical despite different names*

### Comparing `basinmaker-3.0.3a0/basinmaker/postprocessing/combinearcgis.py` & `basinmaker-3.1.0/basinmaker/postprocessing/combinearcgis.py`

 * *Files identical despite different names*

### Comparing `basinmaker-3.0.3a0/basinmaker/postprocessing/combinepurepy.py` & `basinmaker-3.1.0/basinmaker/postprocessing/selectlakepurepy.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,82 +1,117 @@
 import numpy as np
 import sys
 import os
 import csv
 import tempfile
 import copy
 import pandas as pd
+import shutil
 import geopandas
 
 import sys, os
 sys.path.append(os.path.join(os.path.dirname(__file__), '..'))
 
 from basinmaker.func.purepy import *
 from basinmaker.func.pdtable import *
 
-def combine_catchments_covered_by_the_same_lake_purepy(
-    Routing_Product_Folder,
-    area_thresthold = 10*30*30/1000/1000,
+def simplify_routing_structure_by_filter_lakes_purepy(
+    Routing_Product_Folder = '#',
+    Thres_Area_Conn_Lakes=-1,
+    Thres_Area_Non_Conn_Lakes=-1,
+    Selected_Lake_List_in=[],
+    OutputFolder="#",
+    qgis_prefix_path="#",
+    gis_platform="arcgis",
 ):
-    """Define final lake river routing structure
+    """Simplify the routing product by lake area
 
-    Generate the final lake river routing structure by merging subbasin
-    polygons that are covered by the same lake.
-    The input are the catchment polygons and river segements
-    before merging for lakes. The input files can be output of
-    any of following functions:
-    SelectLakes, Select_Routing_product_based_SubId,
-    Customize_Routing_Topology,RoutingNetworkTopologyUpdateToolset_riv
-    The result is the final catchment polygon that ready to be used for
-    hydrological modeling
+    Function that used to simplify the routing product by user
+    provided lake area thresthold.
+    The input catchment polygons is the routing product before
+    merging for lakes. It is provided with the routing product.
+    The result is the simplified catchment polygons. But
+    result from this fuction still not merging catchment
+    covering by the same lake. Thus, The result generated
+    from this tools need further processed by
+    Define_Final_Catchment, or can be further processed by
+    Customize_Routing_Topology
 
     Parameters
     ----------
-    OutputFolder                   : string
-        Folder name that stores generated extracted routing product
+
     Path_final_riv_ply             : string
         Path to the catchment polygon which is the routing product
         before merging lakes catchments and need to be processed before
         used. It is the input for simplify the routing product based
         on lake area or drianage area.
-        routing product and can be directly used.
     Path_final_riv                 : string
         Path to the river polyline which is the routing product
         before merging lakes catchments and need to be processed before
         used. It is the input for simplify the routing product based
         on lake area or drianage area.
+    Path_Con_Lake_ply              : string
+        Path to a connected lake polygon. Connected lakes are lakes that
+        are connected by Path_final_riv.
+    Path_NonCon_Lake_ply           : string
+        Path to a non connected lake polygon. Connected lakes are lakes
+        that are not connected by Path_final_riv.
+    Thres_Area_Conn_Lakes          : float (optional)
+        It is the lake area threshold for connated lakes, in km2
+    Thres_Area_Non_Conn_Lakes      : float (optional)
+        It is the lake area threshold for non connated lakes, in km2
+    Selection_Method               : string
+        It is a string indicate lake selection methods
+        "ByArea" means lake in the routing product will be selected based
+        on two lake area thresthold Thres_Area_Conn_Lakes and
+        Thres_Area_Non_Conn_Lakes
+        "ByLakelist" means lake in the routing product will be selected
+        based on user provided hydrolake id, in Selected_Lake_List_in
+    Selected_Lake_List_in          : list
+        A list of lake ids that will be keeped in the routing product.
+        Lakes not in the list will be removed from routing product.
+    OutputFolder                   : string
+        Folder name that stores generated extracted routing product
 
     Notes
     -------
     This function has no return values, instead will generate following
-    files. They are catchment polygons and river polylines that can be
-    used for hydrological modeling.
-    os.path.join(OutputFolder,'finalcat_info.shp')
-    os.path.join(OutputFolder,'finalcat_info_riv.shp')
+    files. The output tpye will be the same as inputs, but the routing
+    network will be simplified by removing lakes.
+
+    os.path.join(OutputFolder,os.path.basename(Path_final_riv_ply))
+    os.path.join(OutputFolder,os.path.basename(Path_final_riv))
+    os.path.join(OutputFolder,os.path.basename(Path_Con_Lake_ply))
+    os.path.join(OutputFolder,os.path.basename(Path_NonCon_Lake_ply))
 
     Returns:
     -------
     None
 
     Examples
     -------
 
     """
+    if not os.path.exists(OutputFolder):
+        os.makedirs(OutputFolder)
 
-
-    sub_colnm = "SubId"
+    tempfolder = os.path.join(
+        tempfile.gettempdir(),
+        "basinmaker_sllake_" + str(np.random.randint(1, 10000 + 1)),
+    )
+    if not os.path.exists(tempfolder):
+        os.makedirs(tempfolder)
 
     Path_Catchment_Polygon="#"
     Path_River_Polyline="#"
     Path_Con_Lake_ply="#"
     Path_NonCon_Lake_ply="#"
     Path_obs_gauge_point="#"
     Path_final_cat_ply="#"
     Path_final_cat_riv="#"
-
     ##define input files from routing prodcut
     for file in os.listdir(Routing_Product_Folder):
         if file.endswith(".shp"):
             if 'catchment_without_merging_lakes' in file:
                 Path_Catchment_Polygon = os.path.join(Routing_Product_Folder, file)
             if 'river_without_merging_lakes' in file:
                 Path_River_Polyline = os.path.join(Routing_Product_Folder, file)
@@ -87,67 +122,85 @@
             if 'obs_gauges' in file or 'poi' in file:
                 Path_obs_gauge_point = os.path.join(Routing_Product_Folder, file)
             if 'finalcat_info' in file:
                 Path_final_cat_ply = os.path.join(Routing_Product_Folder, file)
             if 'finalcat_info_riv' in file:
                 Path_final_cat_riv = os.path.join(Routing_Product_Folder, file)
 
-    if Path_Catchment_Polygon == '#':
+    if Path_Catchment_Polygon == '#' or  Path_River_Polyline =='#':
         print("Invalid routing product folder ")
 
-
-    OutputFolder = Routing_Product_Folder
-
-
-    Path_final_rivply = Path_Catchment_Polygon
+    Path_final_riv_ply = Path_Catchment_Polygon
     Path_final_riv = Path_River_Polyline
 
-    if not os.path.exists(OutputFolder):
-        os.makedirs(OutputFolder)
-
-    tempfolder = os.path.join(
-        tempfile.gettempdir(), "basinmaker_" + str(np.random.randint(1, 10000 + 1))
-    )
-    if not os.path.exists(tempfolder):
-        os.makedirs(tempfolder)
-
-    ### create a copy of shapfiles in temp folder
-    Path_Temp_final_rviply = os.path.join(OutputFolder,"temp_finalriv_ply" + str(np.random.randint(1, 10000 + 1)) + ".shp")
+    ## copy obs_gauges to output folder
+    for file in os.listdir(Routing_Product_Folder):
+        if 'obs_gauges' in file or 'poi' in file:
+            shutil.copy(os.path.join(Routing_Product_Folder, file), os.path.join(OutputFolder, file))
 
-    Path_Temp_final_rvi = os.path.join(OutputFolder,"temp_finalriv_riv" + str(np.random.randint(1, 10000 + 1)) + ".shp")
 
-    ### read riv ply info
     ### read attribute table
+    finalcat_info = geopandas.read_file(Path_final_riv_ply)
 
-    finalrivply_info = geopandas.read_file(Path_final_rivply)
-    # change attribute table for lake covered catchments,
-    finalrivply_info['SubId'] = finalrivply_info['SubId'].astype('int32')
-    finalrivply_info['DowSubId'] = finalrivply_info['DowSubId'].astype('int32')
-    finalrivply_info['HyLakeId'] = finalrivply_info['HyLakeId'].astype('int32')
-#    finalrivply_info['DrainArea'] = finalrivply_info['DrainArea'].astype('float')
-
-    mapoldnew_info = change_attribute_values_for_catchments_covered_by_same_lake(
-        finalrivply_info
+    ### Obtain selected lake's attribute info
+    ### Obtain selected lake's attribute info
+    (
+        Selected_Non_ConnLakes,
+        Selected_ConnLakes,
+        Un_Selected_ConnLakes_info,
+        Un_Selected_Non_ConnL_info,
+    ) = Return_Selected_Lakes_Attribute_Table_And_Id(
+        finalcat_info,
+        Thres_Area_Conn_Lakes*1000*1000,
+        Thres_Area_Non_Conn_Lakes*1000*1000,
+        Selected_Lake_List_in,
     )
 
-    mapoldnew_info = remove_possible_small_subbasins(mapoldnew_info = mapoldnew_info, area_thresthold = area_thresthold)
-    # update topology for new attribute table
-    mapoldnew_info = update_topology(mapoldnew_info, UpdateStreamorder=-1)
+    ### Extract lake polygons
+    if len(Selected_Non_ConnLakes) > 0:
+        sl_con_lakes = geopandas.read_file(Path_NonCon_Lake_ply)
+        sl_con_lakes = sl_con_lakes.loc[sl_con_lakes['Hylak_id'].isin(Selected_Non_ConnLakes)]
+        sl_con_lakes.to_file(os.path.join(OutputFolder,os.path.basename(Path_NonCon_Lake_ply)))
+
+    if len(Selected_ConnLakes) > 0:
+        sl_con_lakes = geopandas.read_file(Path_Con_Lake_ply)
+        sl_con_lakes = sl_con_lakes.loc[sl_con_lakes['Hylak_id'].isin(Selected_ConnLakes)]
+        sl_con_lakes.to_file(os.path.join(OutputFolder,os.path.basename(Path_Con_Lake_ply)))
+
+    print(" Obtain selected Lake IDs done")
+
+    finalcat_ply = geopandas.read_file(Path_final_riv_ply)
+    # change lake related attribute for un selected connected lake
+    # catchment to -1.2345
+    finalcat_ply = Remove_Unselected_Lake_Attribute_In_Finalcatinfo_purepy(
+        finalcat_ply, Selected_ConnLakes
+    )
+    # remove lake attribute
 
-    mapoldnew_info['DowSubId'] = mapoldnew_info['DowSubId'].astype('int32')
+    # Modify attribute table to merge un selected lake catchment if needed
+    # change attributes for catchment due to remove of connected lakes
+    mapoldnew_info = (
+        Change_Attribute_Values_For_Catchments_Need_To_Be_Merged_By_Remove_CL(
+            finalcat_ply, Un_Selected_ConnLakes_info
+        )
+    )
+    # change attribute for catchment due to remove of non connected lakes
+    mapoldnew_info = (
+        Change_Attribute_Values_For_Catchments_Need_To_Be_Merged_By_Remove_NCL(
+            mapoldnew_info, finalcat_ply, Un_Selected_Non_ConnL_info
+        )
+    )
 
-    if len(os.path.basename(Path_Catchment_Polygon).split('_')) == 5:
-        cat_name = "finalcat_info_"+os.path.basename(Path_Catchment_Polygon).split('_')[4]
-        riv_name = "finalcat_info_riv_"+os.path.basename(Path_Catchment_Polygon).split('_')[4]
-    else:
-        cat_name =  "finalcat_info.shp"
-        riv_name =  "finalcat_info_riv.shp"
+    # update topology for new attribute table
+    mapoldnew_info = UpdateTopology(mapoldnew_info, UpdateStreamorder=-1)
+    mapoldnew_info = update_non_connected_catchment_info(mapoldnew_info)
 
     save_modified_attributes_to_outputs(
         mapoldnew_info=mapoldnew_info,
         tempfolder=tempfolder,
         OutputFolder=OutputFolder,
-        cat_name=cat_name,
-        riv_name =riv_name,
+        cat_name=os.path.basename(Path_final_riv_ply),
+        riv_name = os.path.basename(Path_final_riv),
         Path_final_riv = Path_final_riv,
     )
+
     return
```

### Comparing `basinmaker-3.0.3a0/basinmaker/postprocessing/downloadpd.py` & `basinmaker-3.1.0/basinmaker/postprocessing/downloadpd.py`

 * *Ordering differences only*

 * *Files 10% similar despite different names*

```diff
@@ -1,136 +1,136 @@
-
-import os
-import wget
-import pandas as pd
-import numpy as np
-import gdown
-# define function two download routing product for a given gauge
-def Download_Routing_Product_For_One_Gauge(product_name,gauge_name = "#",region='#',subreg = '#'):
-    if product_name == 'NALRP':
-        version = 'v2-1'
-        if gauge_name != '#':
-            gauge_info = pd.read_csv("https://github.com/dustming/RoutingTool/wiki/Files/obs_gauges_NA_v2-1.csv")
-            gauge_info_sl = gauge_info[gauge_info['Obs_NM'] == gauge_name]
-            if len(gauge_info_sl) < 1:
-                print("The gauge ",gauge_name,"is not included in the routing product ")
-                SubId = -1
-                product_path = '#'
-            else:
-                if gauge_info_sl['Use_region'].values[0] < 1:
-#                    print(gauge_info_sl)
-#                    print(gauge_info_sl['Region'].values[0],gauge_info_sl['Sub_Reg'].values[0])
-                    region_id = int(gauge_info_sl['Region'].values[0])
-                    subreg_id = int(gauge_info_sl['Sub_Reg'].values[0])
-                    url = "http://hydrology.uwaterloo.ca/basinmaker/data/original/drainage_region_%s_%s_v2-1.zip" % (str(region_id).zfill(4),str(subreg_id).zfill(5))
-                    wget.download(url)
-                    os.system('unzip drainage_region_%s_%s_%s.zip' % (str(region_id).zfill(4),str(subreg_id).zfill(5),version))
-                    SubId =  gauge_info_sl['SubId'].values[0]
-                    product_name = "drainage_region_%s_%s_%s" % (str(region_id).zfill(4),str(subreg_id).zfill(5),version)
-                    product_path = os.path.join(os.getcwd(),product_name)
-                    print("The needed product locates at:",product_path)
-                    print("The Subbasin Id of the interested gauge is:",SubId)
-                else:
-#                    print(gauge_info_sl)
-#                    print(gauge_info_sl['Region'].values[0],gauge_info_sl['Sub_Reg'].values[0])
-                    region_id = int(gauge_info_sl['Region'].values[0])
-#                    subreg_id = int(gauge_info_sl['Sub_Reg'].values[0])
-                    url = "http://hydrology.uwaterloo.ca/basinmaker/data/original/drainage_region_%s_v2-1.zip" % (str(region_id).zfill(4))
-                    wget.download(url)
-                    os.system('unzip drainage_region_%s_v2-1.zip' % (str(region_id).zfill(4)))
-                    SubId =  gauge_info_sl['SubId'].values[0]
-                    product_name = "drainage_region_%s_v2-1" % (str(region_id).zfill(4))
-                    product_path = os.path.join(os.getcwd(),product_name)
-                    print("The needed product locates at:",product_path)
-                    print("The Subbasin Id of the interested gauge is:",SubId)
-
-        elif region != '#' and subreg =='#':
-            region_id = region
-            subreg_id = '-'
-            url = "http://hydrology.uwaterloo.ca/basinmaker/data/original/drainage_region_%s_v2-1.zip" % (str(region_id).zfill(4))
-            wget.download(url)
-            os.system('unzip drainage_region_%s_v2-1.zip' % (str(region_id).zfill(4)))
-            product_name =  "drainage_region_%s_v2-1" % (str(region_id).zfill(4))
-            product_path = os.path.join(os.getcwd(),product_name)
-            SubId =  -1
-
-        elif region != '#' and subreg !='#':
-            print("todo")
-        else:
-            print("Wrong option provided")
-
-
-    if product_name == 'OLRP':
-        version = 'v1-0'
-        gauge_info = pd.read_csv("https://github.com/dustming/RoutingTool/wiki/Files/OIH_gauge_info.csv")
-        productinfo = pd.read_csv("https://github.com/dustming/RoutingTool/wiki/Files/OLRRP.csv")
-        if gauge_name != '#':
-            gauge_info_sl = gauge_info[gauge_info['Obs_NM'] == gauge_name]
-            if len(gauge_info_sl) < 1 or gauge_info_sl['SubId'].values[0] < 0:
-                print("The gauge ",gauge_name,"is not included in the routing product ")
-                SubId = -1
-                product_path = '#'
-            else:
-                if gauge_info_sl['Use_region'].values[0] < 1:
-                    region_id = gauge_info_sl['Region'].values[0]
-                    subreg_id = gauge_info_sl['Sub_Reg'].values[0]
-                    mask1 = productinfo['Region'] == region_id
-                    mask2 = productinfo['Sub_Reg'] == subreg_id
-                    mask = np.logical_and(mask1,mask2)
-                    url_veiw = productinfo.loc[mask,'Download'].values[0]
-
-                    url_veiw = url_veiw.split("/")
-                    url = "https://drive.google.com/u/0/uc?id=%s&export=download"%(url_veiw[5])
-                    output = 'drainage_region_%s_%s_%s.zip' % (region_id,subreg_id,version)
-
-                    os.system('gdown %s -O %s' % (url_veiw[5],output))
-
-                    os.system('unzip drainage_region_%s_%s_%s.zip' % (region_id,subreg_id,version))
-                    SubId =  gauge_info_sl['SubId'].values[0]
-                    product_name = 'drainage_region_%s_%s_%s' % (region_id,subreg_id,version)
-                    product_path = os.path.join(os.getcwd(),product_name)
-                    print("The needed product locates at:",product_path)
-                    print("The Subbasin Id of the interested gauge is:",SubId)
-                else:
-                    region_id = gauge_info_sl['Region'].values[0]
-                    subreg_id = '-'
-                    mask1 = productinfo['Region'] == region_id
-                    mask2 = productinfo['Sub_Reg'] == subreg_id
-                    mask = np.logical_and(mask1,mask2)
-                    url_veiw = productinfo.loc[mask,'Download'].values[0]
-                    url_veiw = url_veiw.split("/")
-                    url = "https://drive.google.com/u/0/uc?id=%s&export=download"%(url_veiw[5])
-                    output = 'drainage_region_%s_%s.zip' % (region_id,version)
-
-                    os.system('gdown %s -O %s' % (url_veiw[5],output))
-
-                    os.system('unzip drainage_region_%s_%s.zip' % (region_id,version))
-                    SubId =  gauge_info_sl['SubId'].values[0]
-                    product_name ='drainage_region_%s_%s' % (region_id,version)
-                    product_path = os.path.join(os.getcwd(),product_name)
-                    print("The needed product locates at:",product_path)
-                    print("The Subbasin Id of the interested gauge is:",SubId)
-
-        elif region != '#' and subreg =='#':
-            region_id = region
-            subreg_id = '-'
-            mask1 = productinfo['Region'] == region_id
-            mask2 = productinfo['Sub_Reg'] == subreg_id
-            mask = np.logical_and(mask1,mask2)
-            url_veiw = productinfo.loc[mask,'Download'].values[0]
-            url_veiw = url_veiw.split("/")
-            url = "https://drive.google.com/u/0/uc?id=%s&export=download"%(url_veiw[5])
-            output = 'drainage_region_%s_%s.zip' % (region_id,version)
-
-            os.system('gdown %s -O %s' % (url_veiw[5],output))
-
-            os.system('unzip drainage_region_%s_%s.zip' % (region_id,version))
-            SubId =  -1
-            product_name ='drainage_region_%s_%s' % (region_id,version)
-            product_path = os.path.join(os.getcwd(),product_name)
-
-        elif region != '#' and subreg !='#':
-            print("todo")
-        else:
-            print("Wrong option provided")
-
-    return SubId,product_path
+
+import os
+import wget
+import pandas as pd
+import numpy as np
+import gdown
+# define function two download routing product for a given gauge
+def Download_Routing_Product_For_One_Gauge(product_name,gauge_name = "#",region='#',subreg = '#'):
+    if product_name == 'NALRP':
+        version = 'v2-1'
+        if gauge_name != '#':
+            gauge_info = pd.read_csv("https://github.com/dustming/RoutingTool/wiki/Files/obs_gauges_NA_v2-1.csv")
+            gauge_info_sl = gauge_info[gauge_info['Obs_NM'] == gauge_name]
+            if len(gauge_info_sl) < 1:
+                print("The gauge ",gauge_name,"is not included in the routing product ")
+                SubId = -1
+                product_path = '#'
+            else:
+                if gauge_info_sl['Use_region'].values[0] < 1:
+#                    print(gauge_info_sl)
+#                    print(gauge_info_sl['Region'].values[0],gauge_info_sl['Sub_Reg'].values[0])
+                    region_id = int(gauge_info_sl['Region'].values[0])
+                    subreg_id = int(gauge_info_sl['Sub_Reg'].values[0])
+                    url = "http://hydrology.uwaterloo.ca/basinmaker/data/original/drainage_region_%s_%s_v2-1.zip" % (str(region_id).zfill(4),str(subreg_id).zfill(5))
+                    wget.download(url)
+                    os.system('unzip drainage_region_%s_%s_%s.zip' % (str(region_id).zfill(4),str(subreg_id).zfill(5),version))
+                    SubId =  gauge_info_sl['SubId'].values[0]
+                    product_name = "drainage_region_%s_%s_%s" % (str(region_id).zfill(4),str(subreg_id).zfill(5),version)
+                    product_path = os.path.join(os.getcwd(),product_name)
+                    print("The needed product locates at:",product_path)
+                    print("The Subbasin Id of the interested gauge is:",SubId)
+                else:
+#                    print(gauge_info_sl)
+#                    print(gauge_info_sl['Region'].values[0],gauge_info_sl['Sub_Reg'].values[0])
+                    region_id = int(gauge_info_sl['Region'].values[0])
+#                    subreg_id = int(gauge_info_sl['Sub_Reg'].values[0])
+                    url = "http://hydrology.uwaterloo.ca/basinmaker/data/original/drainage_region_%s_v2-1.zip" % (str(region_id).zfill(4))
+                    wget.download(url)
+                    os.system('unzip drainage_region_%s_v2-1.zip' % (str(region_id).zfill(4)))
+                    SubId =  gauge_info_sl['SubId'].values[0]
+                    product_name = "drainage_region_%s_v2-1" % (str(region_id).zfill(4))
+                    product_path = os.path.join(os.getcwd(),product_name)
+                    print("The needed product locates at:",product_path)
+                    print("The Subbasin Id of the interested gauge is:",SubId)
+
+        elif region != '#' and subreg =='#':
+            region_id = region
+            subreg_id = '-'
+            url = "http://hydrology.uwaterloo.ca/basinmaker/data/original/drainage_region_%s_v2-1.zip" % (str(region_id).zfill(4))
+            wget.download(url)
+            os.system('unzip drainage_region_%s_v2-1.zip' % (str(region_id).zfill(4)))
+            product_name =  "drainage_region_%s_v2-1" % (str(region_id).zfill(4))
+            product_path = os.path.join(os.getcwd(),product_name)
+            SubId =  -1
+
+        elif region != '#' and subreg !='#':
+            print("todo")
+        else:
+            print("Wrong option provided")
+
+
+    if product_name == 'OLRP':
+        version = 'v1-0'
+        gauge_info = pd.read_csv("https://github.com/dustming/RoutingTool/wiki/Files/OIH_gauge_info.csv")
+        productinfo = pd.read_csv("https://github.com/dustming/RoutingTool/wiki/Files/OLRRP.csv")
+        if gauge_name != '#':
+            gauge_info_sl = gauge_info[gauge_info['Obs_NM'] == gauge_name]
+            if len(gauge_info_sl) < 1 or gauge_info_sl['SubId'].values[0] < 0:
+                print("The gauge ",gauge_name,"is not included in the routing product ")
+                SubId = -1
+                product_path = '#'
+            else:
+                if gauge_info_sl['Use_region'].values[0] < 1:
+                    region_id = gauge_info_sl['Region'].values[0]
+                    subreg_id = gauge_info_sl['Sub_Reg'].values[0]
+                    mask1 = productinfo['Region'] == region_id
+                    mask2 = productinfo['Sub_Reg'] == subreg_id
+                    mask = np.logical_and(mask1,mask2)
+                    url_veiw = productinfo.loc[mask,'Download'].values[0]
+
+                    url_veiw = url_veiw.split("/")
+                    url = "https://drive.google.com/u/0/uc?id=%s&export=download"%(url_veiw[5])
+                    output = 'drainage_region_%s_%s_%s.zip' % (region_id,subreg_id,version)
+
+                    os.system('gdown %s -O %s' % (url_veiw[5],output))
+
+                    os.system('unzip drainage_region_%s_%s_%s.zip' % (region_id,subreg_id,version))
+                    SubId =  gauge_info_sl['SubId'].values[0]
+                    product_name = 'drainage_region_%s_%s_%s' % (region_id,subreg_id,version)
+                    product_path = os.path.join(os.getcwd(),product_name)
+                    print("The needed product locates at:",product_path)
+                    print("The Subbasin Id of the interested gauge is:",SubId)
+                else:
+                    region_id = gauge_info_sl['Region'].values[0]
+                    subreg_id = '-'
+                    mask1 = productinfo['Region'] == region_id
+                    mask2 = productinfo['Sub_Reg'] == subreg_id
+                    mask = np.logical_and(mask1,mask2)
+                    url_veiw = productinfo.loc[mask,'Download'].values[0]
+                    url_veiw = url_veiw.split("/")
+                    url = "https://drive.google.com/u/0/uc?id=%s&export=download"%(url_veiw[5])
+                    output = 'drainage_region_%s_%s.zip' % (region_id,version)
+
+                    os.system('gdown %s -O %s' % (url_veiw[5],output))
+
+                    os.system('unzip drainage_region_%s_%s.zip' % (region_id,version))
+                    SubId =  gauge_info_sl['SubId'].values[0]
+                    product_name ='drainage_region_%s_%s' % (region_id,version)
+                    product_path = os.path.join(os.getcwd(),product_name)
+                    print("The needed product locates at:",product_path)
+                    print("The Subbasin Id of the interested gauge is:",SubId)
+
+        elif region != '#' and subreg =='#':
+            region_id = region
+            subreg_id = '-'
+            mask1 = productinfo['Region'] == region_id
+            mask2 = productinfo['Sub_Reg'] == subreg_id
+            mask = np.logical_and(mask1,mask2)
+            url_veiw = productinfo.loc[mask,'Download'].values[0]
+            url_veiw = url_veiw.split("/")
+            url = "https://drive.google.com/u/0/uc?id=%s&export=download"%(url_veiw[5])
+            output = 'drainage_region_%s_%s.zip' % (region_id,version)
+
+            os.system('gdown %s -O %s' % (url_veiw[5],output))
+
+            os.system('unzip drainage_region_%s_%s.zip' % (region_id,version))
+            SubId =  -1
+            product_name ='drainage_region_%s_%s' % (region_id,version)
+            product_path = os.path.join(os.getcwd(),product_name)
+
+        elif region != '#' and subreg !='#':
+            print("todo")
+        else:
+            print("Wrong option provided")
+
+    return SubId,product_path
```

### Comparing `basinmaker-3.0.3a0/basinmaker/postprocessing/downloadpdptspurepy.py` & `basinmaker-3.1.0/basinmaker/postprocessing/downloadpdptspurepy.py`

 * *Files identical despite different names*

### Comparing `basinmaker-3.0.3a0/basinmaker/postprocessing/gridweight.py` & `basinmaker-3.1.0/basinmaker/postprocessing/gridweight.py`

 * *Files identical despite different names*

### Comparing `basinmaker-3.0.3a0/basinmaker/postprocessing/gridweightarcgis.py` & `basinmaker-3.1.0/basinmaker/postprocessing/gridweightarcgis.py`

 * *Files identical despite different names*

### Comparing `basinmaker-3.0.3a0/basinmaker/postprocessing/hru.py` & `basinmaker-3.1.0/basinmaker/postprocessing/hru.py`

 * *Files identical despite different names*

### Comparing `basinmaker-3.0.3a0/basinmaker/postprocessing/hruarcgis.py` & `basinmaker-3.1.0/basinmaker/postprocessing/hruarcgis.py`

 * *Files identical despite different names*

### Comparing `basinmaker-3.0.3a0/basinmaker/postprocessing/hrupurepy.py` & `basinmaker-3.1.0/basinmaker/postprocessing/hrupurepy.py`

 * *Files 0% similar despite different names*

```diff
@@ -459,15 +459,17 @@
     for TOLERANCE in TOLERANCEs:
         HRU_draf_final_wgs_84['geometry'] = HRU_draf_final_wgs_84.simplify(TOLERANCE)
         HRU_draf_final_wgs_84.to_file(output_jason_path,driver="GeoJSON")
 
         json_file_size = os.stat(output_jason_path).st_size/1024/1024 #to MB
         if json_file_size <= 100:
             break
-
+    
+    # Clean up temp folder
+    shutil.rmtree(tempfolder)
 
 def GeneratelandandlakeHRUS(
     OutputFolder,
     tempfolder,
     Path_Subbasin_ply,
     Path_Connect_Lake_ply="#",
     Path_Non_Connect_Lake_ply="#",
```

### Comparing `basinmaker-3.0.3a0/basinmaker/postprocessing/increaseda.py` & `basinmaker-3.1.0/basinmaker/postprocessing/increaseda.py`

 * *Files identical despite different names*

### Comparing `basinmaker-3.0.3a0/basinmaker/postprocessing/increasedaarcgis.py` & `basinmaker-3.1.0/basinmaker/postprocessing/increasedaarcgis.py`

 * *Files identical despite different names*

### Comparing `basinmaker-3.0.3a0/basinmaker/postprocessing/increasedapurepy.py` & `basinmaker-3.1.0/basinmaker/postprocessing/increasedapurepy.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,26 +1,26 @@
+from basinmaker.func.pdtable import *
+from basinmaker.func.purepy import *
 import numpy as np
 import sys
 import os
 import csv
 import tempfile
 import copy
 import pandas as pd
 import shutil
 import geopandas
 
-import sys, os
+import sys
+import os
 sys.path.append(os.path.join(os.path.dirname(__file__), '..'))
 
-from basinmaker.func.purepy import *
-from basinmaker.func.pdtable import *
-
 
 def simplify_routing_structure_by_drainage_area_purepy(
-    Routing_Product_Folder= '#',
+    Routing_Product_Folder='#',
     Area_Min=-1,
     OutputFolder="#",
 ):
     """Simplify the routing product by drainage area
 
     Function that used to simplify the routing product by
     using user provided minimum subbasin drainage area.
@@ -73,15 +73,15 @@
     -------
     None
 
     Examples
     -------
 
     """
-    #### generate river catchments based on minmum area.
+    # generate river catchments based on minmum area.
 
     sub_colnm = "SubId"
     down_colnm = "DowSubId"
     DA_colnm = "DrainArea"
     SegID_colnm = "Seg_ID"
 
     if not os.path.exists(OutputFolder):
@@ -89,51 +89,55 @@
 
     tempfolder = os.path.join(
         tempfile.gettempdir(), "basinmaker_inda_" + str(np.random.randint(1, 10000 + 1))
     )
     if not os.path.exists(tempfolder):
         os.makedirs(tempfolder)
 
-    Path_Catchment_Polygon="#"
-    Path_River_Polyline="#"
-    Path_Con_Lake_ply="#"
-    Path_NonCon_Lake_ply="#"
-    Path_obs_gauge_point="#"
-    Path_final_cat_ply="#"
-    Path_final_cat_riv="#"
+    Path_Catchment_Polygon = "#"
+    Path_River_Polyline = "#"
+    Path_Con_Lake_ply = "#"
+    Path_NonCon_Lake_ply = "#"
+    Path_obs_gauge_point = "#"
+    Path_final_cat_ply = "#"
+    Path_final_cat_riv = "#"
 
-    ##define input files from routing prodcut
+    # define input files from routing prodcut
     for file in os.listdir(Routing_Product_Folder):
         if file.endswith(".shp"):
             if 'catchment_without_merging_lakes' in file:
-                Path_Catchment_Polygon = os.path.join(Routing_Product_Folder, file)
+                Path_Catchment_Polygon = os.path.join(
+                    Routing_Product_Folder, file)
             if 'river_without_merging_lakes' in file:
-                Path_River_Polyline = os.path.join(Routing_Product_Folder, file)
+                Path_River_Polyline = os.path.join(
+                    Routing_Product_Folder, file)
             if 'sl_connected_lake' in file:
                 Path_Con_Lake_ply = os.path.join(Routing_Product_Folder, file)
             if 'sl_non_connected_lake' in file:
-                Path_NonCon_Lake_ply = os.path.join(Routing_Product_Folder, file)
+                Path_NonCon_Lake_ply = os.path.join(
+                    Routing_Product_Folder, file)
             if 'obs_gauges' in file or 'poi' in file:
-                Path_obs_gauge_point = os.path.join(Routing_Product_Folder, file)
+                Path_obs_gauge_point = os.path.join(
+                    Routing_Product_Folder, file)
             if 'finalcat_info' in file:
                 Path_final_cat_ply = os.path.join(Routing_Product_Folder, file)
             if 'finalcat_info_riv' in file:
                 Path_final_cat_riv = os.path.join(Routing_Product_Folder, file)
 
-    if Path_Catchment_Polygon == '#' or  Path_River_Polyline =='#':
+    if Path_Catchment_Polygon == '#' or Path_River_Polyline == '#':
         print("Invalid routing product folder ")
 
     Path_final_riv_ply = Path_Catchment_Polygon
     Path_final_riv = Path_River_Polyline
 
-    ## copy obs_gauges to output folder
+    # copy obs_gauges to output folder
     for file in os.listdir(Routing_Product_Folder):
         if 'obs_gauges' in file or 'poi' in file:
-            shutil.copy(os.path.join(Routing_Product_Folder, file), os.path.join(OutputFolder, file))
-
+            shutil.copy(os.path.join(Routing_Product_Folder, file),
+                        os.path.join(OutputFolder, file))
 
     # overall procedure,
     # 1. first get product attribute table
     # 2. determine which features needs to be merged together to increage
     #    drainage area of the sub basin, for example sub a, b c needs to be merged
     # 3. in the attribute table, change sub a b c 's content to a, assuming sub b and c drainge to a.
     # 4. copy modified attribute table to shafiles
@@ -148,69 +152,79 @@
 
     finalriv_infoply = geopandas.read_file(Path_final_rviply)
     finalriv_inforiv = geopandas.read_file(Path_final_riv)
 
     if Path_Conl_ply != '#':
         Conn_Lakes_ply = geopandas.read_file(Path_Conl_ply)
     else:
-        Conn_Lakes_ply = pd.DataFrame(np.full((10,1),-9999),columns=["Hylak_id"])
-
-
+        Conn_Lakes_ply = pd.DataFrame(
+            np.full((10, 1), -9999), columns=["Hylak_id"])
 
     # change attribute table
     (
         mapoldnew_info,
         Selected_riv_ids,
         Connected_Lake_Mainriv,
         Old_Non_Connect_LakeIds,
         Conn_To_NonConlakeids,
     ) = Change_Attribute_Values_For_Catchments_Need_To_Be_Merged_By_Increase_DA(
         finalriv_infoply, Conn_Lakes_ply, Area_Min
     )
 
-    finalriv_inforiv_main = finalriv_inforiv.loc[finalriv_inforiv['SubId'].isin(Selected_riv_ids)]
-    finalriv_inforiv_main.to_file(os.path.join(tempfolder,'selected_riv.shp'))
-
     UpdateTopology(mapoldnew_info)
     mapoldnew_info = update_non_connected_catchment_info(mapoldnew_info)
 
+    # Selected_riv_ids, mapoldnew_info = Add_River_Segment_Between_Lakes_And_Observations(
+    #     mapoldnew_info, Selected_riv_ids, finalriv_infoply)
+
+    finalriv_inforiv_main = finalriv_inforiv.loc[finalriv_inforiv['SubId'].isin(
+        Selected_riv_ids)]
+    finalriv_inforiv_main.to_file(os.path.join(tempfolder, 'selected_riv.shp'))
+
     save_modified_attributes_to_outputs(
         mapoldnew_info=mapoldnew_info,
         tempfolder=tempfolder,
         OutputFolder=OutputFolder,
         cat_name=os.path.basename(Path_final_riv_ply),
-        riv_name = os.path.basename(Path_final_riv),
-        Path_final_riv = os.path.join(tempfolder,'selected_riv.shp'),
+        riv_name=os.path.basename(Path_final_riv),
+        Path_final_riv=os.path.join(tempfolder, 'selected_riv.shp'),
     )
 
     # export lakes
     if Path_Conl_ply == '#':
         Conn_Lakes_ply_select = []
         Conn_Lakes_ply_not_select = []
     else:
         Conn_Lakes_ply = geopandas.read_file(Path_Conl_ply)
         lake_mask = Conn_Lakes_ply['Hylak_id'].isin(Connected_Lake_Mainriv)
         Conn_Lakes_ply_select = Conn_Lakes_ply.loc[lake_mask].copy()
-        Conn_Lakes_ply_not_select = Conn_Lakes_ply.loc[np.logical_not(lake_mask)].copy()
+        Conn_Lakes_ply_not_select = Conn_Lakes_ply.loc[np.logical_not(
+            lake_mask)].copy()
 
     # export lake polygons
     # export connected lake polygon
     if len(Conn_Lakes_ply_select) > 0:
-        Conn_Lakes_ply_select.to_file(os.path.join(OutputFolder,os.path.basename(Path_Conl_ply)))
+        Conn_Lakes_ply_select.to_file(os.path.join(
+            OutputFolder, os.path.basename(Path_Conl_ply)))
 
     # export non connected polygon
-    if len(Conn_Lakes_ply_not_select) >0 and Path_NonCon_Lake_ply != '#':
+    if len(Conn_Lakes_ply_not_select) > 0 and Path_NonCon_Lake_ply != '#':
         non_conn_Lakes_ply = geopandas.read_file(Path_NonCon_Lake_ply)
-        new_non_connected_lake = pd.concat([non_conn_Lakes_ply, Conn_Lakes_ply_not_select], ignore_index=True)
-        new_non_connected_lake.to_file(os.path.join(OutputFolder,os.path.basename(Path_NonCon_Lake_ply)))
+        new_non_connected_lake = pd.concat(
+            [non_conn_Lakes_ply, Conn_Lakes_ply_not_select], ignore_index=True)
+        new_non_connected_lake.to_file(os.path.join(
+            OutputFolder, os.path.basename(Path_NonCon_Lake_ply)))
     if len(Conn_Lakes_ply_not_select) <= 0 and Path_NonCon_Lake_ply != '#':
         non_conn_Lakes_ply = geopandas.read_file(Path_NonCon_Lake_ply)
-        non_conn_Lakes_ply.to_file(os.path.join(OutputFolder,os.path.basename(Path_NonCon_Lake_ply)))
+        non_conn_Lakes_ply.to_file(os.path.join(
+            OutputFolder, os.path.basename(Path_NonCon_Lake_ply)))
     if len(Conn_Lakes_ply_not_select) > 0 and Path_NonCon_Lake_ply == '#':
         if len(os.path.basename(Path_Conl_ply).split('_')) == 4:
-            outlake_name = 'sl_non_connected_lake_' + os.path.basename(Path_Conl_ply).split('_')[3]
+            outlake_name = 'sl_non_connected_lake_' + \
+                os.path.basename(Path_Conl_ply).split('_')[3]
         else:
             outlake_name = 'sl_non_connected_lake.shp'
 
-        Conn_Lakes_ply_not_select.to_file(os.path.join(OutputFolder,outlake_name))
+        Conn_Lakes_ply_not_select.to_file(
+            os.path.join(OutputFolder, outlake_name))
 
     return
```

### Comparing `basinmaker-3.0.3a0/basinmaker/postprocessing/inversetopology.py` & `basinmaker-3.1.0/basinmaker/postprocessing/inversetopology.py`

 * *Files identical despite different names*

### Comparing `basinmaker-3.0.3a0/basinmaker/postprocessing/plotleaflet.py` & `basinmaker-3.1.0/basinmaker/postprocessing/plotleaflet.py`

 * *Files identical despite different names*

### Comparing `basinmaker-3.0.3a0/basinmaker/postprocessing/postprocessingfunctions.py` & `basinmaker-3.1.0/basinmaker/postprocessing/postprocessingfunctions.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,29 +1,30 @@
 import os
 
 
 def combine_catchments_covered_by_the_same_lake_method(
-    Routing_Product_Folder = '#',
+    Routing_Product_Folder='#',
     qgis_prefix_path="#",
-    area_thresthold = 10*30*30/1000/1000,
+    area_thresthold=10*30*30/1000/1000,
+    length_thresthold=1,
     gis_platform="qgis",
 ):
 
     if gis_platform == "qgis":
         assert (
             qgis_prefix_path != "#"
         ), "qgis prefix path is needed, when gis_platform = qgis"
         from basinmaker.postprocessing.combine import (
             combine_catchments_covered_by_the_same_lake_qgis,
         )
 
         combine_catchments_covered_by_the_same_lake_qgis(
             # Path_final_rivply=Path_final_rivply,
             # Path_final_riv=Path_final_riv,
-            Routing_Product_Folder = Routing_Product_Folder,
+            Routing_Product_Folder=Routing_Product_Folder,
             qgis_prefix_path=qgis_prefix_path,
         )
     if gis_platform == "arcgis":
         from basinmaker.postprocessing.combinearcgis import (
             combine_catchments_covered_by_the_same_lake_arcgis,
         )
 
@@ -34,24 +35,25 @@
     if gis_platform == "purepy":
         from basinmaker.postprocessing.combinepurepy import (
             combine_catchments_covered_by_the_same_lake_purepy,
         )
 
         combine_catchments_covered_by_the_same_lake_purepy(
             Routing_Product_Folder=Routing_Product_Folder,
-            area_thresthold = area_thresthold,
+            area_thresthold=area_thresthold,
+            length_thresthold=length_thresthold,
         )
 
 
 def simplify_routing_structure_by_filter_lakes_method(
     Path_final_riv_ply="#",
     Path_final_riv="#",
     Path_Con_Lake_ply="#",
     Path_NonCon_Lake_ply="#",
-    Routing_Product_Folder = '#',
+    Routing_Product_Folder='#',
     Thres_Area_Conn_Lakes=-1,
     Thres_Area_Non_Conn_Lakes=-1,
     Selected_Lake_List_in=[],
     OutputFolder="#",
     qgis_prefix_path="#",
     gis_platform="qgis",
 ):
@@ -61,44 +63,44 @@
             qgis_prefix_path != "#"
         ), "qgis prefix path is needed, when gis_platform = qgis"
         from basinmaker.postprocessing.selectlake import (
             simplify_routing_structure_by_filter_lakes_qgis,
         )
 
         simplify_routing_structure_by_filter_lakes_qgis(
-            Routing_Product_Folder = Routing_Product_Folder,
+            Routing_Product_Folder=Routing_Product_Folder,
             Thres_Area_Conn_Lakes=Thres_Area_Conn_Lakes,
             Thres_Area_Non_Conn_Lakes=Thres_Area_Non_Conn_Lakes,
             Selected_Lake_List_in=Selected_Lake_List_in,
             OutputFolder=OutputFolder,
             qgis_prefix_path=qgis_prefix_path,
             gis_platform=gis_platform,
         )
     if gis_platform == "arcgis":
         from basinmaker.postprocessing.selectlakearcgis import (
             simplify_routing_structure_by_filter_lakes_arcgis,
         )
 
         simplify_routing_structure_by_filter_lakes_arcgis(
-            Routing_Product_Folder = Routing_Product_Folder,
+            Routing_Product_Folder=Routing_Product_Folder,
             Thres_Area_Conn_Lakes=Thres_Area_Conn_Lakes,
             Thres_Area_Non_Conn_Lakes=Thres_Area_Non_Conn_Lakes,
             Selected_Lake_List_in=Selected_Lake_List_in,
             OutputFolder=OutputFolder,
             qgis_prefix_path=qgis_prefix_path,
             gis_platform=gis_platform,
         )
 
     if gis_platform == "purepy":
         from basinmaker.postprocessing.selectlakepurepy import (
             simplify_routing_structure_by_filter_lakes_purepy,
         )
 
         simplify_routing_structure_by_filter_lakes_purepy(
-            Routing_Product_Folder = Routing_Product_Folder,
+            Routing_Product_Folder=Routing_Product_Folder,
             Thres_Area_Conn_Lakes=Thres_Area_Conn_Lakes,
             Thres_Area_Non_Conn_Lakes=Thres_Area_Non_Conn_Lakes,
             Selected_Lake_List_in=Selected_Lake_List_in,
             OutputFolder=OutputFolder,
             qgis_prefix_path=qgis_prefix_path,
             gis_platform=gis_platform,
         )
@@ -117,73 +119,75 @@
             qgis_prefix_path != "#"
         ), "qgis prefix path is needed, when gis_platform = qgis"
         from basinmaker.postprocessing.increaseda import (
             simplify_routing_structure_by_drainage_area_qgis,
         )
 
         simplify_routing_structure_by_drainage_area_qgis(
-            Routing_Product_Folder = Routing_Product_Folder,
+            Routing_Product_Folder=Routing_Product_Folder,
             Area_Min=Area_Min,
             OutputFolder=OutputFolder,
             qgis_prefix_path=qgis_prefix_path,
         )
 
     if gis_platform == "arcgis":
         from basinmaker.postprocessing.increasedaarcgis import (
             simplify_routing_structure_by_drainage_area_arcgis,
         )
 
         simplify_routing_structure_by_drainage_area_arcgis(
-            Routing_Product_Folder = Routing_Product_Folder,
+            Routing_Product_Folder=Routing_Product_Folder,
             Area_Min=Area_Min,
             OutputFolder=OutputFolder,
         )
 
     if gis_platform == "purepy":
         from basinmaker.postprocessing.increasedapurepy import (
             simplify_routing_structure_by_drainage_area_purepy,
         )
 
         simplify_routing_structure_by_drainage_area_purepy(
-            Routing_Product_Folder = Routing_Product_Folder,
+            Routing_Product_Folder=Routing_Product_Folder,
             Area_Min=Area_Min,
             OutputFolder=OutputFolder,
         )
 
+
 def add_point_of_interest_sites_in_routing_product_method(
-    routing_product_folder= '#',
-    path_to_points_of_interest_points = '#',
-    clean_exist_pois = True,
-    path_output_folder = "#",
+    routing_product_folder='#',
+    path_to_points_of_interest_points='#',
+    clean_exist_pois=True,
+    path_output_folder="#",
     gis_platform="qgis",
 ):
     if gis_platform == "purepy":
         from basinmaker.postprocessing.assigninterestsites import (
             define_interest_sites,
         )
         define_interest_sites(
-            routing_product_folder= routing_product_folder,
-            path_to_points_of_interest_points = path_to_points_of_interest_points,
-            clean_exist_pois = clean_exist_pois,
-            path_output_folder = path_output_folder,
+            routing_product_folder=routing_product_folder,
+            path_to_points_of_interest_points=path_to_points_of_interest_points,
+            clean_exist_pois=clean_exist_pois,
+            path_output_folder=path_output_folder,
         )
     return
 
+
 def select_part_of_routing_product_method(
     Path_Points,
     Gauge_NMS,
     OutputFolder,
     mostdownid,
     mostupid,
     Path_Catchment_Polygon="#",
     Path_River_Polyline="#",
     Path_Con_Lake_ply="#",
     Path_NonCon_Lake_ply="#",
     qgis_prefix_path="#",
-    Routing_Product_Folder = '#',
+    Routing_Product_Folder='#',
     gis_platform="qgis",
 ):
 
     if gis_platform == "qgis":
         from basinmaker.postprocessing.selectprod import (
             Locate_subid_needsbyuser_qgis,
             Select_Routing_product_based_SubId_qgis,
@@ -217,38 +221,38 @@
                 OutputFolder=OutputFolder,
                 # Path_Catchment_Polygon=Path_Catchment_Polygon,
                 # Path_River_Polyline=Path_River_Polyline,
                 # Path_Con_Lake_ply=Path_Con_Lake_ply,
                 # Path_NonCon_Lake_ply=Path_NonCon_Lake_ply,
                 mostdownid=mostdownid,
                 mostupstreamid=mostupid,
-                Routing_Product_Folder = Routing_Product_Folder,
+                Routing_Product_Folder=Routing_Product_Folder,
                 qgis_prefix_path=qgis_prefix_path,
             )
 
     if gis_platform == "arcgis":
         from basinmaker.postprocessing.selectprodarcgis import (
-        Select_Routing_product_based_SubId_arcgis
+            Select_Routing_product_based_SubId_arcgis
         )
         Select_Routing_product_based_SubId_arcgis(
             OutputFolder=OutputFolder,
             mostdownid=mostdownid,
             mostupstreamid=mostupid,
-            Routing_Product_Folder = Routing_Product_Folder,
+            Routing_Product_Folder=Routing_Product_Folder,
         )
 
     if gis_platform == "purepy":
         from basinmaker.postprocessing.selectprodpurepy import (
-        Select_Routing_product_based_SubId_purepy
+            Select_Routing_product_based_SubId_purepy
         )
         Select_Routing_product_based_SubId_purepy(
             OutputFolder=OutputFolder,
             mostdownid=mostdownid,
             mostupstreamid=mostupid,
-            Routing_Product_Folder = Routing_Product_Folder,
+            Routing_Product_Folder=Routing_Product_Folder,
         )
 
     return
 
 
 def generate_hrus_method(
     Path_Subbasin_Ply,
@@ -267,22 +271,22 @@
     Path_Veg_Ply="#",
     Veg_ID="Veg_ID",
     Path_Other_Ply_1="#",
     Other_Ply_ID_1="O_ID_1",
     Path_Other_Ply_2="#",
     Other_Ply_ID_2="O_ID_2",
     DEM="#",
-    Inmportance_order = ["Hylak_id","Landuse_ID"],
-    min_hru_area_pct_sub = 0.2,
+    Inmportance_order=["Hylak_id", "Landuse_ID"],
+    min_hru_area_pct_sub=0.2,
     Project_crs="EPSG:3573",
     OutputFolder="#",
     qgis_prefix_path="#",
     gis_platform="qgis",
-    pixel_size = 30,
-    area_ratio_thresholds = [0,0,0]
+    pixel_size=30,
+    area_ratio_thresholds=[0, 0, 0]
 ):
     if gis_platform == "qgis":
         from basinmaker.postprocessing.hru import GenerateHRUS_qgis
 
         GenerateHRUS_qgis(
             Path_Subbasin_Ply=Path_Subbasin_Ply,
             Landuse_info=Landuse_info,
@@ -303,16 +307,16 @@
             Other_Ply_ID_1=Other_Ply_ID_1,
             Path_Other_Ply_2=Path_Other_Ply_2,
             Other_Ply_ID_2=Other_Ply_ID_2,
             DEM=DEM,
             Project_crs=Project_crs,
             OutputFolder=OutputFolder,
             qgis_prefix_path=qgis_prefix_path,
-            importance_order = Inmportance_order,
-            min_hru_pct_sub_area = min_hru_area_pct_sub,
+            importance_order=Inmportance_order,
+            min_hru_pct_sub_area=min_hru_area_pct_sub,
         )
 
     if gis_platform == "arcgis":
         from basinmaker.postprocessing.hruarcgis import GenerateHRUS_arcgis
 
         GenerateHRUS_arcgis(
             Path_Subbasin_Ply=Path_Subbasin_Ply,
@@ -330,22 +334,21 @@
             Soil_ID=Soil_ID,
             Path_Veg_Ply=Path_Veg_Ply,
             Veg_ID=Veg_ID,
             Path_Other_Ply_1=Path_Other_Ply_1,
             Other_Ply_ID_1=Other_Ply_ID_1,
             Path_Other_Ply_2=Path_Other_Ply_2,
             Other_Ply_ID_2=Other_Ply_ID_2,
-            Inmportance_order = Inmportance_order,
-            min_hru_area_pct_sub = min_hru_area_pct_sub,
+            Inmportance_order=Inmportance_order,
+            min_hru_area_pct_sub=min_hru_area_pct_sub,
             DEM=DEM,
             Project_crs=Project_crs,
             OutputFolder=OutputFolder,
         )
 
-
     if gis_platform == "purepy":
         from basinmaker.postprocessing.hrupurepy import GenerateHRUS_purepy
 
         GenerateHRUS_purepy(
             Path_Subbasin_Ply=Path_Subbasin_Ply,
             Landuse_info=Landuse_info,
             Soil_info=Soil_info,
@@ -361,24 +364,23 @@
             Soil_ID=Soil_ID,
             Path_Veg_Ply=Path_Veg_Ply,
             Veg_ID=Veg_ID,
             Path_Other_Ply_1=Path_Other_Ply_1,
             Other_Ply_ID_1=Other_Ply_ID_1,
             Path_Other_Ply_2=Path_Other_Ply_2,
             Other_Ply_ID_2=Other_Ply_ID_2,
-            Inmportance_order = Inmportance_order,
-            min_hru_area_pct_sub = min_hru_area_pct_sub,
+            Inmportance_order=Inmportance_order,
+            min_hru_area_pct_sub=min_hru_area_pct_sub,
             DEM=DEM,
             Project_crs=Project_crs,
             OutputFolder=OutputFolder,
-            pixel_size = pixel_size,
-            area_ratio_thresholds = area_ratio_thresholds,
+            pixel_size=pixel_size,
+            area_ratio_thresholds=area_ratio_thresholds,
         )
 
-
     return
 
 
 def obtain_grids_polygon_from_netcdf_file(
     qgis_prefix_path,
     netcdf_path="#",
     output_folder="#",
@@ -386,19 +388,17 @@
     coor_y_nm="lat",
     is_rotated_grid=1,
     r_coor_x_nm="rlon",
     r_coor_y_nm="rlat",
     spatial_ref="EPSG:4326",
     x_add=-360,
     y_add=0,
-    gis_platform = "qgis",
+    gis_platform="qgis",
 ):
 
-
-
     if gis_platform == "qgis":
         from basinmaker.postprocessing.gridweight import (
             Generate_Grid_Poly_From_NetCDF_QGIS,
         )
         Generate_Grid_Poly_From_NetCDF_QGIS(
             NetCDF_Path=netcdf_path,
             Output_Folder=output_folder,
@@ -410,34 +410,33 @@
             SpatialRef=spatial_ref,
             x_add=x_add,
             y_add=y_add,
             qgis_prefix_path=qgis_prefix_path,
         )
 
 
-
 def generate_area_weight_of_two_polygons(
     target_polygon_path="#",
     mapping_polygon_path="#",
     col_nm="HRU_ID",
     output_folder="#",
-    qgis_prefix_path = '#',
-    gis_platform = "qgis"
+    qgis_prefix_path='#',
+    gis_platform="qgis"
 ):
 
     if gis_platform == "qgis":
         from basinmaker.postprocessing.gridweight import (
             Area_Weighted_Mapping_Between_Two_Polygons_QGIS,
         )
         Area_Weighted_Mapping_Between_Two_Polygons_QGIS(
             Target_Ply_Path=target_polygon_path,
             Mapping_Ply_Path=mapping_polygon_path,
             Col_NM=col_nm,
             Output_Folder=output_folder,
-            qgis_prefix_path = qgis_prefix_path,
+            qgis_prefix_path=qgis_prefix_path,
         )
 
     if gis_platform == "arcgis":
         from basinmaker.postprocessing.gridweightarcgis import (
             Area_Weighted_Mapping_Between_Two_Polygons_Arcgis,
         )
         Area_Weighted_Mapping_Between_Two_Polygons_Arcgis(
```

### Comparing `basinmaker-3.0.3a0/basinmaker/postprocessing/selectlake.py` & `basinmaker-3.1.0/basinmaker/postprocessing/selectlake.py`

 * *Files identical despite different names*

### Comparing `basinmaker-3.0.3a0/basinmaker/postprocessing/selectlakearcgis.py` & `basinmaker-3.1.0/basinmaker/postprocessing/selectlakearcgis.py`

 * *Files identical despite different names*

### Comparing `basinmaker-3.0.3a0/basinmaker/postprocessing/selectprod.py` & `basinmaker-3.1.0/basinmaker/postprocessing/selectprod.py`

 * *Files identical despite different names*

### Comparing `basinmaker-3.0.3a0/basinmaker/postprocessing/selectprodarcgis.py` & `basinmaker-3.1.0/basinmaker/postprocessing/selectprodarcgis.py`

 * *Files identical despite different names*

### Comparing `basinmaker-3.0.3a0/basinmaker/postprocessing/selectprodpurepy.py` & `basinmaker-3.1.0/basinmaker/postprocessing/selectprodpurepy.py`

 * *Files identical despite different names*

### Comparing `basinmaker-3.0.3a0/basinmaker/preprocessing/preinputpolygonqgis.py` & `basinmaker-3.1.0/basinmaker/preprocessing/preinputpolygonqgis.py`

 * *Files identical despite different names*

### Comparing `basinmaker-3.0.3a0/basinmaker/preprocessing/preprocessinglakeply.py` & `basinmaker-3.1.0/basinmaker/preprocessing/preprocessinglakeply.py`

 * *Files identical despite different names*

### Comparing `basinmaker-3.0.3a0/basinmaker/preprocessing/preprocessingobs.py` & `basinmaker-3.1.0/basinmaker/preprocessing/preprocessingobs.py`

 * *Files identical despite different names*

### Comparing `basinmaker-3.0.3a0/basinmaker/preprocessing/preprocessrasterqgis.py` & `basinmaker-3.1.0/basinmaker/preprocessing/preprocessrasterqgis.py`

 * *Files identical despite different names*

### Comparing `basinmaker-3.0.3a0/basinmaker/preprocessing/rasterizevectorsandloadtodbqgis.py` & `basinmaker-3.1.0/basinmaker/preprocessing/rasterizevectorsandloadtodbqgis.py`

 * *Files identical despite different names*

### Comparing `basinmaker-3.0.3a0/basinmaker/preprocessing/reprojectandclipvectorbyplyqgis.py` & `basinmaker-3.1.0/basinmaker/preprocessing/reprojectandclipvectorbyplyqgis.py`

 * *Files identical despite different names*

### Comparing `basinmaker-3.0.3a0/basinmaker/subreg/defsubreg.py` & `basinmaker-3.1.0/basinmaker/subreg/defsubreg.py`

 * *Files identical despite different names*

### Comparing `basinmaker-3.0.3a0/basinmaker/subreg/generatesubregionqgis.py` & `basinmaker-3.1.0/basinmaker/subreg/generatesubregionqgis.py`

 * *Files identical despite different names*

### Comparing `basinmaker-3.0.3a0/basinmaker.egg-info/PKG-INFO` & `basinmaker-3.1.0/basinmaker.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: basinmaker
-Version: 3.0.3a0
+Version: 3.1.0
 Summary: An automated GIS toolbox for watershed delineation with lakes
 Home-page: https://github.com/dustming/basinmaker
 Author: basinmaker development team
 Author-email: m43han@uwaterloo.ca
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `basinmaker-3.0.3a0/basinmaker.egg-info/SOURCES.txt` & `basinmaker-3.1.0/basinmaker.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -60,19 +60,22 @@
 basinmaker/func/arcgis.py
 basinmaker/func/fgdal.py
 basinmaker/func/grassgis.py
 basinmaker/func/pdtable.py
 basinmaker/func/purepy.py
 basinmaker/func/qgis.py
 basinmaker/func/rarray.py
+basinmaker/func/__pycache__/__init__.cpython-311.pyc
 basinmaker/func/__pycache__/__init__.cpython-39.pyc
 basinmaker/func/__pycache__/arcgis.cpython-39.pyc
 basinmaker/func/__pycache__/fgdal.cpython-39.pyc
 basinmaker/func/__pycache__/grassgis.cpython-39.pyc
+basinmaker/func/__pycache__/pdtable.cpython-311.pyc
 basinmaker/func/__pycache__/pdtable.cpython-39.pyc
+basinmaker/func/__pycache__/purepy.cpython-311.pyc
 basinmaker/func/__pycache__/purepy.cpython-39.pyc
 basinmaker/func/__pycache__/qgis.cpython-39.pyc
 basinmaker/func/__pycache__/rarray.cpython-39.pyc
 basinmaker/hymodin/__init__.py
 basinmaker/hymodin/raveninput.py
 basinmaker/postprocessing/__init__.py
 basinmaker/postprocessing/assigninterestsites.py
```

### Comparing `basinmaker-3.0.3a0/setup.py` & `basinmaker-3.1.0/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="basinmaker",
-    version="3.0.3a",
+    version="3.1.0",
     author="basinmaker development team",
     author_email="m43han@uwaterloo.ca",
     description="An automated GIS toolbox for watershed delineation with lakes",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/dustming/basinmaker",
     packages = setuptools.find_packages(
```

### Comparing `basinmaker-3.0.3a0/tests/test_RoutingTool_AutomatedWatershedsandLakesFilterToolset.py` & `basinmaker-3.1.0/tests/test_RoutingTool_AutomatedWatershedsandLakesFilterToolset.py`

 * *Files identical despite different names*

### Comparing `basinmaker-3.0.3a0/tests/test_RoutingTool_Generateinputdata.py` & `basinmaker-3.1.0/tests/test_RoutingTool_Generateinputdata.py`

 * *Files identical despite different names*

### Comparing `basinmaker-3.0.3a0/tests/test_RoutingTool_Generatmaskregion.py` & `basinmaker-3.1.0/tests/test_RoutingTool_Generatmaskregion.py`

 * *Files identical despite different names*

### Comparing `basinmaker-3.0.3a0/tests/test_RoutingTool_PostProcessing_Customize_Routing_Topology.py` & `basinmaker-3.1.0/tests/test_RoutingTool_PostProcessing_Customize_Routing_Topology.py`

 * *Files identical despite different names*

### Comparing `basinmaker-3.0.3a0/tests/test_RoutingTool_PostProcessing_Define_Final_Catchment.py` & `basinmaker-3.1.0/tests/test_RoutingTool_PostProcessing_Define_Final_Catchment.py`

 * *Files identical despite different names*

### Comparing `basinmaker-3.0.3a0/tests/test_RoutingTool_PostProcessing_GenerateHRUS.py` & `basinmaker-3.1.0/tests/test_RoutingTool_PostProcessing_GenerateHRUS.py`

 * *Files identical despite different names*

### Comparing `basinmaker-3.0.3a0/tests/test_RoutingTool_PostProcessing_GenerateRavenInput.py` & `basinmaker-3.1.0/tests/test_RoutingTool_PostProcessing_GenerateRavenInput.py`

 * *Files identical despite different names*

### Comparing `basinmaker-3.0.3a0/tests/test_RoutingTool_PostProcessing_Locate_subid_needsbyuser.py` & `basinmaker-3.1.0/tests/test_RoutingTool_PostProcessing_Locate_subid_needsbyuser.py`

 * *Files identical despite different names*

### Comparing `basinmaker-3.0.3a0/tests/test_RoutingTool_PostProcessing_SelectLakes.py` & `basinmaker-3.1.0/tests/test_RoutingTool_PostProcessing_SelectLakes.py`

 * *Files identical despite different names*

### Comparing `basinmaker-3.0.3a0/tests/test_RoutingTool_PostProcessing_Select_Routing_product_based_SubId.py` & `basinmaker-3.1.0/tests/test_RoutingTool_PostProcessing_Select_Routing_product_based_SubId.py`

 * *Files identical despite different names*

### Comparing `basinmaker-3.0.3a0/tests/test_RoutingTool_RoutingNetworkTopologyUpdateToolset_riv.py` & `basinmaker-3.1.0/tests/test_RoutingTool_RoutingNetworkTopologyUpdateToolset_riv.py`

 * *Files identical despite different names*

### Comparing `basinmaker-3.0.3a0/tests/test_RoutingTool_WatershedDiscretizationToolset.py` & `basinmaker-3.1.0/tests/test_RoutingTool_WatershedDiscretizationToolset.py`

 * *Files identical despite different names*

