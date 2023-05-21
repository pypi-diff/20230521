# Comparing `tmp/Orange3-Tools-0.0.4.tar.gz` & `tmp/Orange3-Tools-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "Orange3-Tools-0.0.4.tar", last modified: Sat May 20 11:33:29 2023, max compression
+gzip compressed data, was "Orange3-Tools-0.0.5.tar", last modified: Sun May 21 09:28:59 2023, max compression
```

## Comparing `Orange3-Tools-0.0.4.tar` & `Orange3-Tools-0.0.5.tar`

### file list

```diff
@@ -1,37 +1,37 @@
-drwxr-xr-x   0 julioj.melero   (501) staff       (20)        0 2023-05-20 11:33:29.180518 Orange3-Tools-0.0.4/
--rw-rw-rw-   0 julioj.melero   (501) staff       (20)    35801 2023-03-07 11:54:58.000000 Orange3-Tools-0.0.4/LICENSE
-drwxr-xr-x   0 julioj.melero   (501) staff       (20)        0 2023-05-20 11:33:29.172482 Orange3-Tools-0.0.4/Orange3_Tools.egg-info/
--rw-r--r--   0 julioj.melero   (501) staff       (20)      336 2023-05-20 11:33:29.000000 Orange3-Tools-0.0.4/Orange3_Tools.egg-info/PKG-INFO
--rw-r--r--   0 julioj.melero   (501) staff       (20)     1092 2023-05-20 11:33:29.000000 Orange3-Tools-0.0.4/Orange3_Tools.egg-info/SOURCES.txt
--rw-r--r--   0 julioj.melero   (501) staff       (20)        1 2023-05-20 11:33:29.000000 Orange3-Tools-0.0.4/Orange3_Tools.egg-info/dependency_links.txt
--rw-r--r--   0 julioj.melero   (501) staff       (20)       98 2023-05-20 11:33:29.000000 Orange3-Tools-0.0.4/Orange3_Tools.egg-info/entry_points.txt
--rw-r--r--   0 julioj.melero   (501) staff       (20)        1 2023-05-17 10:38:08.000000 Orange3-Tools-0.0.4/Orange3_Tools.egg-info/not-zip-safe
--rw-r--r--   0 julioj.melero   (501) staff       (20)      200 2023-05-20 11:33:29.000000 Orange3-Tools-0.0.4/Orange3_Tools.egg-info/requires.txt
--rw-r--r--   0 julioj.melero   (501) staff       (20)       14 2023-05-20 11:33:29.000000 Orange3-Tools-0.0.4/Orange3_Tools.egg-info/top_level.txt
--rw-r--r--   0 julioj.melero   (501) staff       (20)      336 2023-05-20 11:33:29.180402 Orange3-Tools-0.0.4/PKG-INFO
--rw-rw-rw-   0 julioj.melero   (501) staff       (20)      100 2023-04-13 16:55:45.000000 Orange3-Tools-0.0.4/README.md
-drwxr-xr-x   0 julioj.melero   (501) staff       (20)        0 2023-05-20 11:33:29.173043 Orange3-Tools-0.0.4/orangecontrib/
--rw-rw-rw-   0 julioj.melero   (501) staff       (20)      169 2023-04-11 17:27:18.000000 Orange3-Tools-0.0.4/orangecontrib/__init__.py
--rw-r--r--   0 julioj.melero   (501) staff       (20)    20713 2023-05-18 08:25:22.000000 Orange3-Tools-0.0.4/orangecontrib/functions.py
-drwxr-xr-x   0 julioj.melero   (501) staff       (20)        0 2023-05-20 11:33:29.173398 Orange3-Tools-0.0.4/orangecontrib/tools/
--rw-rw-rw-   0 julioj.melero   (501) staff       (20)      654 2023-04-11 19:26:01.000000 Orange3-Tools-0.0.4/orangecontrib/tools/__init__.py
-drwxr-xr-x   0 julioj.melero   (501) staff       (20)        0 2023-05-20 11:33:29.176891 Orange3-Tools-0.0.4/orangecontrib/tools/widgets/
--rw-rw-rw-   0 julioj.melero   (501) staff       (20)     6713 2023-04-16 09:22:31.000000 Orange3-Tools-0.0.4/orangecontrib/tools/widgets/MySqlOrange.py
--rw-r--r--   0 julioj.melero   (501) staff       (20)     9754 2023-04-16 15:10:09.000000 Orange3-Tools-0.0.4/orangecontrib/tools/widgets/Pairsplot.py
--rw-r--r--   0 julioj.melero   (501) staff       (20)     7281 2023-04-16 09:57:24.000000 Orange3-Tools-0.0.4/orangecontrib/tools/widgets/Scatterplot.py
--rw-rw-rw-   0 julioj.melero   (501) staff       (20)     1091 2023-04-13 17:01:11.000000 Orange3-Tools-0.0.4/orangecontrib/tools/widgets/__init__.py
-drwxr-xr-x   0 julioj.melero   (501) staff       (20)        0 2023-05-20 11:33:29.180080 Orange3-Tools-0.0.4/orangecontrib/tools/widgets/icons/
--rw-r--r--   0 julioj.melero   (501) staff       (20)    14469 2023-05-17 10:00:19.000000 Orange3-Tools-0.0.4/orangecontrib/tools/widgets/icons/ARIMA.svg
--rw-------   0 julioj.melero   (501) staff       (20)     1513 2023-04-16 09:12:55.000000 Orange3-Tools-0.0.4/orangecontrib/tools/widgets/icons/Barchart.svg
--rw-r--r--   0 julioj.melero   (501) staff       (20)     9756 2023-05-17 10:00:19.000000 Orange3-Tools-0.0.4/orangecontrib/tools/widgets/icons/Correlogram.svg
--rw-------   0 julioj.melero   (501) staff       (20)    15156 2023-04-16 09:04:28.000000 Orange3-Tools-0.0.4/orangecontrib/tools/widgets/icons/Pairs.svg
--rw-rw-rw-   0 julioj.melero   (501) staff       (20)     5586 2023-04-11 16:37:34.000000 Orange3-Tools-0.0.4/orangecontrib/tools/widgets/icons/Simple_scatterplot.svg
--rw-r--r--   0 julioj.melero   (501) staff       (20)    10454 2023-04-16 09:14:11.000000 Orange3-Tools-0.0.4/orangecontrib/tools/widgets/icons/category.svg
--rw-rw-rw-   0 julioj.melero   (501) staff       (20)     3595 2023-03-08 12:27:13.000000 Orange3-Tools-0.0.4/orangecontrib/tools/widgets/icons/mysql-orange.svg
--rw-r--r--   0 julioj.melero   (501) staff       (20)     4964 2023-04-11 17:00:16.000000 Orange3-Tools-0.0.4/orangecontrib/tools/widgets/icons/sscater.svg
--rw-r--r--   0 julioj.melero   (501) staff       (20)     5175 2023-05-18 08:35:35.000000 Orange3-Tools-0.0.4/orangecontrib/tools/widgets/owcorrelogram.py
--rw-r--r--   0 julioj.melero   (501) staff       (20)    30238 2023-05-19 17:23:52.000000 Orange3-Tools-0.0.4/orangecontrib/tools/widgets/owsarima.py
--rw-r--r--   0 julioj.melero   (501) staff       (20)     9733 2023-05-20 11:28:08.000000 Orange3-Tools-0.0.4/orangecontrib/tools/widgets/owstationarity.py
--rw-r--r--   0 julioj.melero   (501) staff       (20)     2212 2023-04-13 16:39:56.000000 Orange3-Tools-0.0.4/orangecontrib/tools/widgets/utils.py
--rw-r--r--   0 julioj.melero   (501) staff       (20)       38 2023-05-20 11:33:29.180559 Orange3-Tools-0.0.4/setup.cfg
--rw-rw-rw-   0 julioj.melero   (501) staff       (20)     3576 2023-05-20 11:33:19.000000 Orange3-Tools-0.0.4/setup.py
+drwxr-xr-x   0 julioj.melero   (501) staff       (20)        0 2023-05-21 09:28:59.017232 Orange3-Tools-0.0.5/
+-rw-rw-rw-   0 julioj.melero   (501) staff       (20)    35801 2023-03-07 11:54:58.000000 Orange3-Tools-0.0.5/LICENSE
+drwxr-xr-x   0 julioj.melero   (501) staff       (20)        0 2023-05-21 09:28:59.010184 Orange3-Tools-0.0.5/Orange3_Tools.egg-info/
+-rw-r--r--   0 julioj.melero   (501) staff       (20)      336 2023-05-21 09:28:58.000000 Orange3-Tools-0.0.5/Orange3_Tools.egg-info/PKG-INFO
+-rw-r--r--   0 julioj.melero   (501) staff       (20)     1092 2023-05-21 09:28:58.000000 Orange3-Tools-0.0.5/Orange3_Tools.egg-info/SOURCES.txt
+-rw-r--r--   0 julioj.melero   (501) staff       (20)        1 2023-05-21 09:28:58.000000 Orange3-Tools-0.0.5/Orange3_Tools.egg-info/dependency_links.txt
+-rw-r--r--   0 julioj.melero   (501) staff       (20)       98 2023-05-21 09:28:58.000000 Orange3-Tools-0.0.5/Orange3_Tools.egg-info/entry_points.txt
+-rw-r--r--   0 julioj.melero   (501) staff       (20)        1 2023-05-17 10:38:08.000000 Orange3-Tools-0.0.5/Orange3_Tools.egg-info/not-zip-safe
+-rw-r--r--   0 julioj.melero   (501) staff       (20)      200 2023-05-21 09:28:58.000000 Orange3-Tools-0.0.5/Orange3_Tools.egg-info/requires.txt
+-rw-r--r--   0 julioj.melero   (501) staff       (20)       14 2023-05-21 09:28:58.000000 Orange3-Tools-0.0.5/Orange3_Tools.egg-info/top_level.txt
+-rw-r--r--   0 julioj.melero   (501) staff       (20)      336 2023-05-21 09:28:59.017091 Orange3-Tools-0.0.5/PKG-INFO
+-rw-rw-rw-   0 julioj.melero   (501) staff       (20)      100 2023-04-13 16:55:45.000000 Orange3-Tools-0.0.5/README.md
+drwxr-xr-x   0 julioj.melero   (501) staff       (20)        0 2023-05-21 09:28:59.010615 Orange3-Tools-0.0.5/orangecontrib/
+-rw-rw-rw-   0 julioj.melero   (501) staff       (20)      169 2023-04-11 17:27:18.000000 Orange3-Tools-0.0.5/orangecontrib/__init__.py
+-rw-r--r--   0 julioj.melero   (501) staff       (20)    20713 2023-05-18 08:25:22.000000 Orange3-Tools-0.0.5/orangecontrib/functions.py
+drwxr-xr-x   0 julioj.melero   (501) staff       (20)        0 2023-05-21 09:28:59.010983 Orange3-Tools-0.0.5/orangecontrib/tools/
+-rw-rw-rw-   0 julioj.melero   (501) staff       (20)      654 2023-04-11 19:26:01.000000 Orange3-Tools-0.0.5/orangecontrib/tools/__init__.py
+drwxr-xr-x   0 julioj.melero   (501) staff       (20)        0 2023-05-21 09:28:59.013987 Orange3-Tools-0.0.5/orangecontrib/tools/widgets/
+-rw-rw-rw-   0 julioj.melero   (501) staff       (20)     6713 2023-04-16 09:22:31.000000 Orange3-Tools-0.0.5/orangecontrib/tools/widgets/MySqlOrange.py
+-rw-r--r--   0 julioj.melero   (501) staff       (20)     9754 2023-04-16 15:10:09.000000 Orange3-Tools-0.0.5/orangecontrib/tools/widgets/Pairsplot.py
+-rw-r--r--   0 julioj.melero   (501) staff       (20)     7281 2023-04-16 09:57:24.000000 Orange3-Tools-0.0.5/orangecontrib/tools/widgets/Scatterplot.py
+-rw-rw-rw-   0 julioj.melero   (501) staff       (20)     1091 2023-04-13 17:01:11.000000 Orange3-Tools-0.0.5/orangecontrib/tools/widgets/__init__.py
+drwxr-xr-x   0 julioj.melero   (501) staff       (20)        0 2023-05-21 09:28:59.016785 Orange3-Tools-0.0.5/orangecontrib/tools/widgets/icons/
+-rw-r--r--   0 julioj.melero   (501) staff       (20)    14469 2023-05-17 10:00:19.000000 Orange3-Tools-0.0.5/orangecontrib/tools/widgets/icons/ARIMA.svg
+-rw-------   0 julioj.melero   (501) staff       (20)     1513 2023-04-16 09:12:55.000000 Orange3-Tools-0.0.5/orangecontrib/tools/widgets/icons/Barchart.svg
+-rw-r--r--   0 julioj.melero   (501) staff       (20)     9756 2023-05-17 10:00:19.000000 Orange3-Tools-0.0.5/orangecontrib/tools/widgets/icons/Correlogram.svg
+-rw-------   0 julioj.melero   (501) staff       (20)    15156 2023-04-16 09:04:28.000000 Orange3-Tools-0.0.5/orangecontrib/tools/widgets/icons/Pairs.svg
+-rw-rw-rw-   0 julioj.melero   (501) staff       (20)     5586 2023-04-11 16:37:34.000000 Orange3-Tools-0.0.5/orangecontrib/tools/widgets/icons/Simple_scatterplot.svg
+-rw-r--r--   0 julioj.melero   (501) staff       (20)    10454 2023-04-16 09:14:11.000000 Orange3-Tools-0.0.5/orangecontrib/tools/widgets/icons/category.svg
+-rw-rw-rw-   0 julioj.melero   (501) staff       (20)     3595 2023-03-08 12:27:13.000000 Orange3-Tools-0.0.5/orangecontrib/tools/widgets/icons/mysql-orange.svg
+-rw-r--r--   0 julioj.melero   (501) staff       (20)     4964 2023-04-11 17:00:16.000000 Orange3-Tools-0.0.5/orangecontrib/tools/widgets/icons/sscater.svg
+-rw-r--r--   0 julioj.melero   (501) staff       (20)     5418 2023-05-21 09:26:14.000000 Orange3-Tools-0.0.5/orangecontrib/tools/widgets/owcorrelogram.py
+-rw-r--r--   0 julioj.melero   (501) staff       (20)    30238 2023-05-19 17:23:52.000000 Orange3-Tools-0.0.5/orangecontrib/tools/widgets/owsarima.py
+-rw-r--r--   0 julioj.melero   (501) staff       (20)     9733 2023-05-20 11:28:08.000000 Orange3-Tools-0.0.5/orangecontrib/tools/widgets/owstationarity.py
+-rw-r--r--   0 julioj.melero   (501) staff       (20)     2212 2023-04-13 16:39:56.000000 Orange3-Tools-0.0.5/orangecontrib/tools/widgets/utils.py
+-rw-r--r--   0 julioj.melero   (501) staff       (20)       38 2023-05-21 09:28:59.017277 Orange3-Tools-0.0.5/setup.cfg
+-rw-rw-rw-   0 julioj.melero   (501) staff       (20)     3576 2023-05-21 09:28:46.000000 Orange3-Tools-0.0.5/setup.py
```

### Comparing `Orange3-Tools-0.0.4/LICENSE` & `Orange3-Tools-0.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `Orange3-Tools-0.0.4/Orange3_Tools.egg-info/SOURCES.txt` & `Orange3-Tools-0.0.5/Orange3_Tools.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `Orange3-Tools-0.0.4/orangecontrib/functions.py` & `Orange3-Tools-0.0.5/orangecontrib/functions.py`

 * *Files identical despite different names*

### Comparing `Orange3-Tools-0.0.4/orangecontrib/tools/__init__.py` & `Orange3-Tools-0.0.5/orangecontrib/tools/__init__.py`

 * *Files identical despite different names*

### Comparing `Orange3-Tools-0.0.4/orangecontrib/tools/widgets/MySqlOrange.py` & `Orange3-Tools-0.0.5/orangecontrib/tools/widgets/MySqlOrange.py`

 * *Files identical despite different names*

### Comparing `Orange3-Tools-0.0.4/orangecontrib/tools/widgets/Pairsplot.py` & `Orange3-Tools-0.0.5/orangecontrib/tools/widgets/Pairsplot.py`

 * *Files identical despite different names*

### Comparing `Orange3-Tools-0.0.4/orangecontrib/tools/widgets/Scatterplot.py` & `Orange3-Tools-0.0.5/orangecontrib/tools/widgets/Scatterplot.py`

 * *Files identical despite different names*

### Comparing `Orange3-Tools-0.0.4/orangecontrib/tools/widgets/__init__.py` & `Orange3-Tools-0.0.5/orangecontrib/tools/widgets/__init__.py`

 * *Files identical despite different names*

### Comparing `Orange3-Tools-0.0.4/orangecontrib/tools/widgets/icons/ARIMA.svg` & `Orange3-Tools-0.0.5/orangecontrib/tools/widgets/icons/ARIMA.svg`

 * *Files identical despite different names*

### Comparing `Orange3-Tools-0.0.4/orangecontrib/tools/widgets/icons/Barchart.svg` & `Orange3-Tools-0.0.5/orangecontrib/tools/widgets/icons/Barchart.svg`

 * *Files identical despite different names*

### Comparing `Orange3-Tools-0.0.4/orangecontrib/tools/widgets/icons/Correlogram.svg` & `Orange3-Tools-0.0.5/orangecontrib/tools/widgets/icons/Correlogram.svg`

 * *Files identical despite different names*

### Comparing `Orange3-Tools-0.0.4/orangecontrib/tools/widgets/icons/Pairs.svg` & `Orange3-Tools-0.0.5/orangecontrib/tools/widgets/icons/Pairs.svg`

 * *Files identical despite different names*

### Comparing `Orange3-Tools-0.0.4/orangecontrib/tools/widgets/icons/Simple_scatterplot.svg` & `Orange3-Tools-0.0.5/orangecontrib/tools/widgets/icons/Simple_scatterplot.svg`

 * *Files identical despite different names*

### Comparing `Orange3-Tools-0.0.4/orangecontrib/tools/widgets/icons/category.svg` & `Orange3-Tools-0.0.5/orangecontrib/tools/widgets/icons/category.svg`

 * *Files identical despite different names*

### Comparing `Orange3-Tools-0.0.4/orangecontrib/tools/widgets/icons/mysql-orange.svg` & `Orange3-Tools-0.0.5/orangecontrib/tools/widgets/icons/mysql-orange.svg`

 * *Files identical despite different names*

### Comparing `Orange3-Tools-0.0.4/orangecontrib/tools/widgets/icons/sscater.svg` & `Orange3-Tools-0.0.5/orangecontrib/tools/widgets/icons/sscater.svg`

 * *Files identical despite different names*

### Comparing `Orange3-Tools-0.0.4/orangecontrib/tools/widgets/owcorrelogram.py` & `Orange3-Tools-0.0.5/orangecontrib/tools/widgets/owcorrelogram.py`

 * *Files 3% similar despite different names*

```diff
@@ -50,15 +50,15 @@
     -------
     acf: array
         Autocorrelation function.
     confint: array, optional
         Confidence intervals if alpha kwarg provided.
     """
     from statsmodels.tsa.stattools import acf
-    if nlags is None:
+    if nlags is 0:
 #        nlags = int(.9 * len(x))
         nlags = int(10 * math.log10(len(x)))
     corr = acf(x, *args, nlags=nlags, fft=fft, **kwargs)
     return _significant_acf(corr, kwargs.get('alpha'))
 
 
 def partial_autocorrelation(x, *args, nlags=None, method='ldb', **kwargs):
@@ -79,61 +79,64 @@
     -------
     acf: array
         Partioal autocorrelation function.
     confint : optional
         As returned by `statsmodels.tsa.stattools.pacf`.
     """
     from statsmodels.tsa.stattools import pacf
-    if nlags is None:
+    if nlags is 0:
         nlags = min(len(x)//2 - 1, len(x) - 1)
     corr = pacf(x, *args, nlags=nlags, method=method, **kwargs)
     return _significant_acf(corr, kwargs.get('alpha'))
 
 
 class OWCorrelogram(OWPeriodBase):
     # TODO: allow computing cross-correlation of two distinct series
     name = 'Correlogram_mod'
     description = "Visualize variables' auto-correlation."
     icon = 'icons/Correlogram.svg'
     priority = 110
-
+    lags = Setting(0)
     use_pacf = Setting(False)
     use_confint = Setting(True)
 
     yrange = (-1, 1)
 
     def __init__(self):
         super().__init__()
         gui.separator(self.controlArea)
+        gui.spin(widget=self.controlArea, master=self, value='lags', minv=0, maxv=300, step=1, label="Lags:",
+                 alignment=Qt.AlignRight, controlWidth=80, callback=self.replot)
         gui.checkBox(self.controlArea, self, 'use_pacf',
                      label='Compute partial auto-correlation',
                      callback=self.replot)
         gui.checkBox(self.controlArea, self, 'use_confint',
                      label='Plot 95% significance interval',
                      callback=self.replot)
 
-    def acf(self, attr, pacf, confint):
-        key = (attr, pacf, confint)
+
+    def acf(self, attr, lags,pacf, confint):
+        key = (attr, pacf,lags, confint)
         if key not in self._cached:
             x = self.data.interp(attr).ravel()
             func = partial_autocorrelation if pacf else autocorrelation
-            self._cached[key] = func(x, alpha=.05 if confint else None)
+            self._cached[key] = func(x, nlags=self.lags,alpha=.05 if confint else None)
         return self._cached[key]
 
     def replot(self):
         self.plot.clear()
         if not self.selection:
             return
 
         self.plot_widget.addItem(pg.InfiniteLine(0, 0, pen=pg.mkPen(0., width=2)))
 
         palette = self.get_palette()
         for i, attr in enumerate(self.selection):
             color = palette.value_to_qcolor(i)
-            x, acf = np.array(self.acf(attr, self.use_pacf, False)).T
+            x, acf = np.array(self.acf(attr, self.lags,self.use_pacf, False)).T
             x = np.repeat(x, 2)
             y = np.vstack((np.zeros(len(acf)), acf)).T.flatten()
             item = pg.PlotCurveItem(
                 x=x, y=y, connect="pairs", antialias=True,
                 pen=pg.mkPen(color, width=5))
             self.plot_widget.addItem(item)
```

### Comparing `Orange3-Tools-0.0.4/orangecontrib/tools/widgets/owsarima.py` & `Orange3-Tools-0.0.5/orangecontrib/tools/widgets/owsarima.py`

 * *Files identical despite different names*

### Comparing `Orange3-Tools-0.0.4/orangecontrib/tools/widgets/owstationarity.py` & `Orange3-Tools-0.0.5/orangecontrib/tools/widgets/owstationarity.py`

 * *Files identical despite different names*

### Comparing `Orange3-Tools-0.0.4/orangecontrib/tools/widgets/utils.py` & `Orange3-Tools-0.0.5/orangecontrib/tools/widgets/utils.py`

 * *Files identical despite different names*

### Comparing `Orange3-Tools-0.0.4/setup.py` & `Orange3-Tools-0.0.5/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from os import path, walk
 from setuptools import setup, find_packages
 from setuptools.dist import Distribution
 
 NAME = "Orange3-Tools"
 
-VERSION = "0.0.4"
+VERSION = "0.0.5"
 
 DESCRIPTION = "Tools para Asignatura Big Data Master EERR"
 LONG_DESCRIPTION = ""
 
 LICENSE = "GPL-3.0"
 
 KEYWORDS = (
```

