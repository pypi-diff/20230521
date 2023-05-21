# Comparing `tmp/dearwatson-0.7.4.tar.gz` & `tmp/dearwatson-0.7.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dearwatson-0.7.4.tar", last modified: Thu May 18 13:57:23 2023, max compression
+gzip compressed data, was "dearwatson-0.7.5.tar", last modified: Sun May 21 14:05:01 2023, max compression
```

## Comparing `dearwatson-0.7.4.tar` & `dearwatson-0.7.5.tar`

### file list

```diff
@@ -1,34 +1,34 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 13:57:23.947231 dearwatson-0.7.4/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-05-18 13:57:11.000000 dearwatson-0.7.4/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       39 2023-05-18 13:57:11.000000 dearwatson-0.7.4/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     2413 2023-05-18 13:57:23.947231 dearwatson-0.7.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1666 2023-05-18 13:57:11.000000 dearwatson-0.7.4/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 13:57:23.943231 dearwatson-0.7.4/dearwatson.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2413 2023-05-18 13:57:23.000000 dearwatson-0.7.4/dearwatson.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      629 2023-05-18 13:57:23.000000 dearwatson-0.7.4/dearwatson.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-18 13:57:23.000000 dearwatson-0.7.4/dearwatson.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      191 2023-05-18 13:57:23.000000 dearwatson-0.7.4/dearwatson.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-05-18 13:57:23.000000 dearwatson-0.7.4/dearwatson.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-18 13:57:23.947231 dearwatson-0.7.4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1344 2023-05-18 13:57:12.000000 dearwatson-0.7.4/setup.py
--rw-r--r--   0 runner    (1001) docker     (123)      265 2023-05-18 13:57:12.000000 dearwatson-0.7.4/tox.ini
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 13:57:23.943231 dearwatson-0.7.4/watson/
--rw-r--r--   0 runner    (1001) docker     (123)       21 2023-05-18 13:57:12.000000 dearwatson-0.7.4/watson/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       56 2023-05-18 13:57:12.000000 dearwatson-0.7.4/watson/constants.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 13:57:23.943231 dearwatson-0.7.4/watson/data_validation_report/
--rw-r--r--   0 runner    (1001) docker     (123)     5666 2023-05-18 13:57:12.000000 dearwatson-0.7.4/watson/data_validation_report/DvrPreparer.py
--rw-r--r--   0 runner    (1001) docker     (123)      106 2023-05-18 13:57:12.000000 dearwatson-0.7.4/watson/data_validation_report/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    13706 2023-05-18 13:57:12.000000 dearwatson-0.7.4/watson/neighbours.py
--rw-r--r--   0 runner    (1001) docker     (123)    18515 2023-05-18 13:57:12.000000 dearwatson-0.7.4/watson/report.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 13:57:23.943231 dearwatson-0.7.4/watson/resources/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 13:57:23.947231 dearwatson-0.7.4/watson/resources/images/
--rw-r--r--   0 runner    (1001) docker     (123)   524520 2023-05-18 13:57:12.000000 dearwatson-0.7.4/watson/resources/images/sherlock3.png
--rw-r--r--   0 runner    (1001) docker     (123)   738619 2023-05-18 13:57:12.000000 dearwatson-0.7.4/watson/resources/images/watson.png
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 13:57:23.947231 dearwatson-0.7.4/watson/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-18 13:57:13.000000 dearwatson-0.7.4/watson/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5929 2023-05-18 13:57:13.000000 dearwatson-0.7.4/watson/tests/test_watson.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 13:57:23.947231 dearwatson-0.7.4/watson/tpfplotterSub/
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-18 13:57:13.000000 dearwatson-0.7.4/watson/tpfplotterSub/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    16155 2023-05-18 13:57:13.000000 dearwatson-0.7.4/watson/tpfplotterSub/tpfplotter.py
--rw-r--r--   0 runner    (1001) docker     (123)    13698 2023-05-18 13:57:13.000000 dearwatson-0.7.4/watson/tpfplotterSub/tpfplotter_py2.py
--rw-r--r--   0 runner    (1001) docker     (123)   107144 2023-05-18 13:57:13.000000 dearwatson-0.7.4/watson/watson.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 14:05:01.492133 dearwatson-0.7.5/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-05-21 14:04:47.000000 dearwatson-0.7.5/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       39 2023-05-21 14:04:47.000000 dearwatson-0.7.5/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     4135 2023-05-21 14:05:01.492133 dearwatson-0.7.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3156 2023-05-21 14:04:47.000000 dearwatson-0.7.5/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 14:05:01.488132 dearwatson-0.7.5/dearwatson.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4135 2023-05-21 14:05:01.000000 dearwatson-0.7.5/dearwatson.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      629 2023-05-21 14:05:01.000000 dearwatson-0.7.5/dearwatson.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-21 14:05:01.000000 dearwatson-0.7.5/dearwatson.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      191 2023-05-21 14:05:01.000000 dearwatson-0.7.5/dearwatson.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-05-21 14:05:01.000000 dearwatson-0.7.5/dearwatson.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-21 14:05:01.492133 dearwatson-0.7.5/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1344 2023-05-21 14:04:48.000000 dearwatson-0.7.5/setup.py
+-rw-r--r--   0 runner    (1001) docker     (123)      265 2023-05-21 14:04:48.000000 dearwatson-0.7.5/tox.ini
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 14:05:01.488132 dearwatson-0.7.5/watson/
+-rw-r--r--   0 runner    (1001) docker     (123)       21 2023-05-21 14:04:48.000000 dearwatson-0.7.5/watson/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       56 2023-05-21 14:04:48.000000 dearwatson-0.7.5/watson/constants.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 14:05:01.488132 dearwatson-0.7.5/watson/data_validation_report/
+-rw-r--r--   0 runner    (1001) docker     (123)     5666 2023-05-21 14:04:48.000000 dearwatson-0.7.5/watson/data_validation_report/DvrPreparer.py
+-rw-r--r--   0 runner    (1001) docker     (123)      106 2023-05-21 14:04:48.000000 dearwatson-0.7.5/watson/data_validation_report/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13706 2023-05-21 14:04:48.000000 dearwatson-0.7.5/watson/neighbours.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18515 2023-05-21 14:04:48.000000 dearwatson-0.7.5/watson/report.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 14:05:01.488132 dearwatson-0.7.5/watson/resources/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 14:05:01.488132 dearwatson-0.7.5/watson/resources/images/
+-rw-r--r--   0 runner    (1001) docker     (123)   524520 2023-05-21 14:04:48.000000 dearwatson-0.7.5/watson/resources/images/sherlock3.png
+-rw-r--r--   0 runner    (1001) docker     (123)   738619 2023-05-21 14:04:48.000000 dearwatson-0.7.5/watson/resources/images/watson.png
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 14:05:01.492133 dearwatson-0.7.5/watson/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-21 14:04:48.000000 dearwatson-0.7.5/watson/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5929 2023-05-21 14:04:48.000000 dearwatson-0.7.5/watson/tests/test_watson.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 14:05:01.492133 dearwatson-0.7.5/watson/tpfplotterSub/
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-21 14:04:49.000000 dearwatson-0.7.5/watson/tpfplotterSub/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16155 2023-05-21 14:04:49.000000 dearwatson-0.7.5/watson/tpfplotterSub/tpfplotter.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13698 2023-05-21 14:04:49.000000 dearwatson-0.7.5/watson/tpfplotterSub/tpfplotter_py2.py
+-rw-r--r--   0 runner    (1001) docker     (123)   107124 2023-05-21 14:04:48.000000 dearwatson-0.7.5/watson/watson.py
```

### Comparing `dearwatson-0.7.4/LICENSE` & `dearwatson-0.7.5/LICENSE`

 * *Files identical despite different names*

### Comparing `dearwatson-0.7.4/dearwatson.egg-info/SOURCES.txt` & `dearwatson-0.7.5/dearwatson.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `dearwatson-0.7.4/setup.py` & `dearwatson-0.7.5/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import setuptools
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
-version = "0.7.4"
+version = "0.7.5"
 setuptools.setup(
     name="dearwatson", # Replace with your own username
     version=version,
     author="M. Dévora-Pajares",
     author_email="mdevorapajares@protonmail.com",
     description="Visual Vetting and Analysis of Transits from Space ObservatioNs",
     long_description=long_description,
```

### Comparing `dearwatson-0.7.4/watson/data_validation_report/DvrPreparer.py` & `dearwatson-0.7.5/watson/data_validation_report/DvrPreparer.py`

 * *Files identical despite different names*

### Comparing `dearwatson-0.7.4/watson/neighbours.py` & `dearwatson-0.7.5/watson/neighbours.py`

 * *Files identical despite different names*

### Comparing `dearwatson-0.7.4/watson/report.py` & `dearwatson-0.7.5/watson/report.py`

 * *Files identical despite different names*

### Comparing `dearwatson-0.7.4/watson/resources/images/sherlock3.png` & `dearwatson-0.7.5/watson/resources/images/sherlock3.png`

 * *Files identical despite different names*

### Comparing `dearwatson-0.7.4/watson/resources/images/watson.png` & `dearwatson-0.7.5/watson/resources/images/watson.png`

 * *Files identical despite different names*

### Comparing `dearwatson-0.7.4/watson/tests/test_watson.py` & `dearwatson-0.7.5/watson/tests/test_watson.py`

 * *Files identical despite different names*

### Comparing `dearwatson-0.7.4/watson/tpfplotterSub/tpfplotter.py` & `dearwatson-0.7.5/watson/tpfplotterSub/tpfplotter.py`

 * *Files identical despite different names*

### Comparing `dearwatson-0.7.4/watson/tpfplotterSub/tpfplotter_py2.py` & `dearwatson-0.7.5/watson/tpfplotterSub/tpfplotter_py2.py`

 * *Files identical despite different names*

### Comparing `dearwatson-0.7.4/watson/watson.py` & `dearwatson-0.7.5/watson/watson.py`

 * *Files 0% similar despite different names*

```diff
@@ -943,20 +943,20 @@
                     nanmask = np.isnan(pixel_flux)
                     pixel_flux[nanmask] = np.nanmedian(pixel_flux)
                     if aperture[i, j]:
                         core_flux = core_flux + pixel_flux
                     if halo_aperture[i, j]:
                         halo_flux = halo_flux + pixel_flux
         core_flux = core_flux / len(np.argwhere(aperture == True))
-        core_flux = wotan.flatten(tpf.time.value, core_flux, duration_to_period * 4, method='biweight')
+        core_flux = wotan.flatten(tpf.time.value, core_flux, duration * 4, method='biweight')
         halo_flux = halo_flux / len(np.argwhere(halo_aperture == True))
         if len(np.argwhere(~np.isnan(halo_flux))) == 0:
             halo_flux = core_flux
         else:
-            halo_flux = wotan.flatten(tpf.time.value, halo_flux, duration_to_period * 4, method='biweight')
+            halo_flux = wotan.flatten(tpf.time.value, halo_flux, duration * 4, method='biweight')
         return (tpf.time.value, core_flux, halo_flux)
 
     @staticmethod
     def compute_centroids_for_tpf(ra, dec, lc_data, tpf, wcs, period, epoch, duration_to_period):
         df = lc_data[(lc_data['time'] >= tpf.time.value[0]) & (lc_data['time'] <= tpf.time.value[-1])].dropna()
         time = df["time"].to_numpy()
         df['time_folded'] = foldedleastsquares.fold(time, period, epoch + period / 2)
```

