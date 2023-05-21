# Comparing `tmp/mpl-markers-0.0.1.tar.gz` & `tmp/mpl-markers-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mpl-markers-0.0.1.tar", last modified: Sat May 13 22:44:50 2023, max compression
+gzip compressed data, was "mpl-markers-0.0.2.tar", last modified: Sun May 21 03:55:25 2023, max compression
```

## Comparing `mpl-markers-0.0.1.tar` & `mpl-markers-0.0.2.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxrwxrwx   0        0        0        0 2023-05-13 22:44:50.565604 mpl-markers-0.0.1/
--rw-rw-rw-   0        0        0     1058 2023-05-13 20:27:08.000000 mpl-markers-0.0.1/LICENSE.txt
--rw-rw-rw-   0        0        0       34 2023-05-13 21:15:24.000000 mpl-markers-0.0.1/MANIFEST.in
--rw-rw-rw-   0        0        0     1431 2023-05-13 22:44:50.565604 mpl-markers-0.0.1/PKG-INFO
--rw-rw-rw-   0        0        0      865 2023-05-13 20:27:08.000000 mpl-markers-0.0.1/README.md
-drwxrwxrwx   0        0        0        0 2023-05-13 22:44:50.549965 mpl-markers-0.0.1/mpl_markers/
--rw-rw-rw-   0        0        0       23 2023-05-13 20:27:08.000000 mpl-markers-0.0.1/mpl_markers/__init__.py
--rw-rw-rw-   0        0        0    25733 2023-05-13 22:20:19.000000 mpl-markers-0.0.1/mpl_markers/artists.py
--rw-rw-rw-   0        0        0     3103 2023-05-13 20:27:08.000000 mpl-markers-0.0.1/mpl_markers/interactive.py
--rw-rw-rw-   0        0        0    23494 2023-05-13 20:27:08.000000 mpl-markers-0.0.1/mpl_markers/markers.py
-drwxrwxrwx   0        0        0        0 2023-05-13 22:44:50.565604 mpl-markers-0.0.1/mpl_markers/style/
--rw-rw-rw-   0        0        0      872 2023-05-13 20:27:08.000000 mpl-markers-0.0.1/mpl_markers/style/default.json
--rw-rw-rw-   0        0        0     2959 2023-05-13 20:27:08.000000 mpl-markers-0.0.1/mpl_markers/utils.py
-drwxrwxrwx   0        0        0        0 2023-05-13 22:44:50.565604 mpl-markers-0.0.1/mpl_markers.egg-info/
--rw-rw-rw-   0        0        0     1431 2023-05-13 22:44:50.000000 mpl-markers-0.0.1/mpl_markers.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      402 2023-05-13 22:44:50.000000 mpl-markers-0.0.1/mpl_markers.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-13 22:44:50.000000 mpl-markers-0.0.1/mpl_markers.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       51 2023-05-13 22:44:50.000000 mpl-markers-0.0.1/mpl_markers.egg-info/requires.txt
--rw-rw-rw-   0        0        0       12 2023-05-13 22:44:50.000000 mpl-markers-0.0.1/mpl_markers.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      837 2023-05-13 22:42:54.000000 mpl-markers-0.0.1/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-05-13 22:44:50.565604 mpl-markers-0.0.1/setup.cfg
--rw-rw-rw-   0        0        0       53 2023-05-13 20:27:08.000000 mpl-markers-0.0.1/setup.py
-drwxrwxrwx   0        0        0        0 2023-05-13 22:44:50.565604 mpl-markers-0.0.1/tests/
--rw-rw-rw-   0        0        0     5892 2023-05-13 20:27:08.000000 mpl-markers-0.0.1/tests/test_markers.py
+drwxrwxrwx   0        0        0        0 2023-05-21 03:55:25.350354 mpl-markers-0.0.2/
+-rw-rw-rw-   0        0        0     1058 2023-05-13 20:27:08.000000 mpl-markers-0.0.2/LICENSE.txt
+-rw-rw-rw-   0        0        0       34 2023-05-13 21:15:24.000000 mpl-markers-0.0.2/MANIFEST.in
+-rw-rw-rw-   0        0        0     1457 2023-05-21 03:55:25.350354 mpl-markers-0.0.2/PKG-INFO
+-rw-rw-rw-   0        0        0      889 2023-05-21 03:49:28.000000 mpl-markers-0.0.2/README.md
+drwxrwxrwx   0        0        0        0 2023-05-21 03:55:25.334731 mpl-markers-0.0.2/mpl_markers/
+-rw-rw-rw-   0        0        0       23 2023-05-13 20:27:08.000000 mpl-markers-0.0.2/mpl_markers/__init__.py
+-rw-rw-rw-   0        0        0    25476 2023-05-21 03:01:12.000000 mpl-markers-0.0.2/mpl_markers/artists.py
+-rw-rw-rw-   0        0        0     3103 2023-05-13 20:27:08.000000 mpl-markers-0.0.2/mpl_markers/interactive.py
+-rw-rw-rw-   0        0        0    23441 2023-05-21 02:10:26.000000 mpl-markers-0.0.2/mpl_markers/markers.py
+drwxrwxrwx   0        0        0        0 2023-05-21 03:55:25.350354 mpl-markers-0.0.2/mpl_markers/style/
+-rw-rw-rw-   0        0        0      936 2023-05-21 03:41:57.000000 mpl-markers-0.0.2/mpl_markers/style/default.json
+-rw-rw-rw-   0        0        0     3501 2023-05-21 02:56:31.000000 mpl-markers-0.0.2/mpl_markers/utils.py
+drwxrwxrwx   0        0        0        0 2023-05-21 03:55:25.350354 mpl-markers-0.0.2/mpl_markers.egg-info/
+-rw-rw-rw-   0        0        0     1457 2023-05-21 03:55:25.000000 mpl-markers-0.0.2/mpl_markers.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      402 2023-05-21 03:55:25.000000 mpl-markers-0.0.2/mpl_markers.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-21 03:55:25.000000 mpl-markers-0.0.2/mpl_markers.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       51 2023-05-21 03:55:25.000000 mpl-markers-0.0.2/mpl_markers.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       12 2023-05-21 03:55:25.000000 mpl-markers-0.0.2/mpl_markers.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      837 2023-05-21 03:53:59.000000 mpl-markers-0.0.2/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-05-21 03:55:25.350354 mpl-markers-0.0.2/setup.cfg
+-rw-rw-rw-   0        0        0       53 2023-05-13 20:27:08.000000 mpl-markers-0.0.2/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-21 03:55:25.350354 mpl-markers-0.0.2/tests/
+-rw-rw-rw-   0        0        0     5882 2023-05-21 03:09:53.000000 mpl-markers-0.0.2/tests/test_markers.py
```

### Comparing `mpl-markers-0.0.1/LICENSE.txt` & `mpl-markers-0.0.2/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `mpl-markers-0.0.1/PKG-INFO` & `mpl-markers-0.0.2/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mpl-markers
-Version: 0.0.1
+Version: 0.0.2
 Summary: interactive marker support for matplotlib
 Author-email: Rick Lyon <rlyon14@gmail.com>
 Project-URL: repository, https://github.com/ricklyon/mpl_markers
 Keywords: matplotlib,markers,interactive
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
@@ -31,14 +31,16 @@
 
 Add a marker attached to plotted data lines:
 ```python
 import numpy as np
 import matplotlib.pyplot as plt
 
 plt.style.use('ggplot')
+plt.rc('font', size=7)
+
 fig, ax = plt.subplots(1,1)
 x1 = np.linspace(-2*np.pi, 2*np.pi, 1000)
 
 ax.plot(x1, np.sin(x1)*np.cos(x1)**2)
 
 mplm.data_marker(x=0)
 ```
```

### Comparing `mpl-markers-0.0.1/README.md` & `mpl-markers-0.0.2/README.md`

 * *Files 15% similar despite different names*

```diff
@@ -16,14 +16,16 @@
 
 Add a marker attached to plotted data lines:
 ```python
 import numpy as np
 import matplotlib.pyplot as plt
 
 plt.style.use('ggplot')
+plt.rc('font', size=7)
+
 fig, ax = plt.subplots(1,1)
 x1 = np.linspace(-2*np.pi, 2*np.pi, 1000)
 
 ax.plot(x1, np.sin(x1)*np.cos(x1)**2)
 
 mplm.data_marker(x=0)
 ```
```

### Comparing `mpl-markers-0.0.1/mpl_markers/artists.py` & `mpl-markers-0.0.2/mpl_markers/artists.py`

 * *Files 2% similar despite different names*

```diff
@@ -206,18 +206,14 @@
         if ylabel:
             # change the edge color of the text box to the line color
             ylabel = dcopy(ylabel)
             ylabel["bbox"]["edgecolor"] = data_line.get_color()
 
             # initalize text box as the label
             self.ylabel = MarkerLabel(axes=axes, transform=None, verticalalignment="bottom", **ylabel)
-
-            # set text formatter
-            if ylabel_formatter is None:
-                self.ylabel_formatter = utils.yformatter
         
         if xydot:
             # initalize marker dot at data point
             self.xydot = MarkerLine(axes=data_line.axes, color=data_line.get_color(), **xydot)
 
         if yline:
             self.yline = MarkerLine(axes=data_line.axes, **yline)
@@ -267,15 +263,15 @@
 
         # set label to left side of axes if yline is active
         xl = 0 if self.yline else xl
             
         if self.ylabel:
             # set the x position to the data point location plus a small pad (in display coordinates)
             xd_lbl = self._alias_xdata[idx] if np.any(self._alias_xdata) else self._xd 
-            txt = self.ylabel_formatter(xd_lbl, self._yd, idx=self._idx, axes=self.axes)
+            txt = utils.yformatter(xd_lbl, self._yd, self._idx, self.axes, self.ylabel_formatter)
 
             self.ylabel.set_position((xl, yl), txt, anchor='center left', disp=True, offset=(label_xpad, 0))
             # get the text label from the formatter
         
         if self.yline:
             self.yline.set_data(self.axes.get_xlim(), [self._yd]*2)
 
@@ -335,26 +331,20 @@
         self.ref_marker = ref_marker
 
         if xline:
             self.xline = MarkerLine(axes=axes, **xline)
 
         if xlabel:
             self.xlabel = MarkerLabel(axes=axes, transform=None, verticalalignment="bottom", **xlabel)
-            # set text formatter
-            if xlabel_formatter is None:
-                self.xlabel_formatter = utils.xformatter
 
         if yline:
             self.yline = MarkerLine(axes=axes, **yline)
 
         if ylabel:
             self.ylabel = MarkerLabel(axes=axes, transform=None, verticalalignment="bottom", **ylabel)
-            # set text formatter
-            if ylabel_formatter is None:
-                self.ylabel_formatter = utils.yformatter
 
         if xymark and xline and yline:
             # initalize marker dot at data point
             self.xymark = MarkerLine(axes=axes, **xymark)
 
         self._xd = 0
         self._yd = 0
@@ -387,17 +377,18 @@
             self._xd = x if not x_alias else x_alias
 
             if self.xlabel:
                 # use reference data if available
                 if self.ref_marker:
                     lbl_xd = self._xd - self.ref_marker._xd
                     lbl_sgn = '$\Delta$ +' if lbl_xd > 0 else '$\Delta$ -'
-                    lbl = lbl_sgn + self.xlabel_formatter(np.abs(lbl_xd), self._yd, axes=self.axes)
+                    txt = utils.xformatter(np.abs(lbl_xd), self._yd, None, self.axes, self.xlabel_formatter)
+                    lbl = lbl_sgn + txt
                 else:
-                    lbl = self.xlabel_formatter(self._xd, self._yd, axes=self.axes)
+                    lbl = utils.xformatter(self._xd, self._yd, None, self.axes, self.xlabel_formatter)
 
                 xl, _ = utils.data2display(self.axes, (x, 0))
                 self.xlabel.set_position((xl, 0), lbl, anchor='lower center', disp=True)
 
             if self.xline:
                 self.xline.set_data([x]*2, self.axes.get_ylim())
 
@@ -410,17 +401,18 @@
             _, yl = utils.data2display(self.axes, (0, y))
 
             if self.ylabel:
                 # use reference data if available
                 if self.ref_marker:
                     lbl_yd = self._yd - self.ref_marker._yd
                     lbl_sgn = '$\Delta$ +' if lbl_yd > 0 else '$\Delta -$'
-                    lbl = lbl_sgn + self.ylabel_formatter(self._xd, np.abs(lbl_yd), axes=self.axes)
+                    txt = utils.yformatter(self._xd, np.abs(lbl_yd), None, self.axes, self.ylabel_formatter)
+                    lbl = lbl_sgn + txt
                 else:
-                    lbl = self.ylabel_formatter(self._xd, self._yd, axes=self.axes)
+                    lbl = utils.yformatter(self._xd, self._yd, None, self.axes, self.ylabel_formatter)
 
                 self.ylabel.set_position((0, yl), lbl, anchor='center left', disp=True)
 
             if self.yline:
                 self.yline.set_data(self.axes.get_xlim(), [y]*2)
 
         if x is not None and y is not None and self.xymark:
```

### Comparing `mpl-markers-0.0.1/mpl_markers/interactive.py` & `mpl-markers-0.0.2/mpl_markers/interactive.py`

 * *Files identical despite different names*

### Comparing `mpl-markers-0.0.1/mpl_markers/markers.py` & `mpl-markers-0.0.2/mpl_markers/markers.py`

 * *Files 1% similar despite different names*

```diff
@@ -207,15 +207,14 @@
 
 
     if xformatter is None and axes._marker_xformatter:
         xformatter = axes._marker_xformatter
     if yformatter is None and axes._marker_yformatter:
         yformatter = axes._marker_yformatter
 
-    # TODO: add hollow circle where lines intersect
     m = artists.AxisLabel(axes, xlabel_formatter=xformatter, ylabel_formatter=yformatter, ref_marker=ref_marker, **properties)
     m.set_position(x, y)
 
     # create new marker and append to the axes marker list
     axes.markers.append(m)
     axes.marker_active = m
```

### Comparing `mpl-markers-0.0.1/mpl_markers/utils.py` & `mpl-markers-0.0.2/mpl_markers/utils.py`

 * *Files 15% similar despite different names*

```diff
@@ -8,44 +8,60 @@
 
 def axes2display(axes, point):
     return axes.transAxes.transform(point)
 
 def display2data(axes, point):
     return axes.transData.inverted().transform(point)
 
-def yformatter(xd: float, yd: float, idx: int=None, axes: Axes=None) -> str:
+def yformatter(xd: float, yd: float, idx: int, axes: Axes, custom: Callable= None) -> str:
     """
     Returns a formatted string for the y-label marker at the data points xd, yd.
     """
-    yformatter = axes.yaxis.get_major_formatter()
+    tick_yformatter = axes.yaxis.get_major_formatter()
     ret = ""
-    
+
+    if custom:
+        # try calling with the x, y data points first
+        try:
+            return custom(xd, yd, idx)
+        # call with just the y-data if above failed
+        except TypeError:
+            return custom(yd)
+
     # use ticker formatter if scalar or fixed formatter
     if (
-        not isinstance(yformatter, (ticker.ScalarFormatter, ticker.FixedFormatter))
+        not isinstance(tick_yformatter, (ticker.ScalarFormatter, ticker.FixedFormatter))
     ):
-        ret = yformatter(yd)
+        ret = tick_yformatter(yd)
 
     # otherwise default to basic format
     if not len(ret):
         return "{:.3f}".format(yd)
 
 
-def xformatter(xd:float, idx: int=None, axes: Axes=None) -> str:
+def xformatter(xd: float, yd: float, idx: int, axes: Axes, custom: Callable= None) -> str:
     """
     Returns a formatted string for the x-label marker at the data point xd.
     """
-    xformatter = axes.xaxis.get_major_formatter()
+    tick_xformatter = axes.xaxis.get_major_formatter()
     ret = ""
 
+    if custom:
+        # try calling with the x, y data points first
+        try:
+            return custom(xd, yd, idx)
+        # call with just the x-data if above failed
+        except TypeError:
+            return custom(xd)
+
     # use ticker formatter if scalar or fixed formatter
     if (
-        not isinstance(xformatter, (ticker.ScalarFormatter, ticker.FixedFormatter))
+        not isinstance(tick_xformatter, (ticker.ScalarFormatter, ticker.FixedFormatter))
     ):
-        return xformatter(xd)
+        return tick_xformatter(xd)
     
     # otherwise default to basic format
     if not len(ret):
         return "{:.3f}".format(xd)
 
 def get_artist_bbox(artist, padding:Tuple[float, float]=None):
     """
```

### Comparing `mpl-markers-0.0.1/mpl_markers.egg-info/PKG-INFO` & `mpl-markers-0.0.2/mpl_markers.egg-info/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mpl-markers
-Version: 0.0.1
+Version: 0.0.2
 Summary: interactive marker support for matplotlib
 Author-email: Rick Lyon <rlyon14@gmail.com>
 Project-URL: repository, https://github.com/ricklyon/mpl_markers
 Keywords: matplotlib,markers,interactive
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
@@ -31,14 +31,16 @@
 
 Add a marker attached to plotted data lines:
 ```python
 import numpy as np
 import matplotlib.pyplot as plt
 
 plt.style.use('ggplot')
+plt.rc('font', size=7)
+
 fig, ax = plt.subplots(1,1)
 x1 = np.linspace(-2*np.pi, 2*np.pi, 1000)
 
 ax.plot(x1, np.sin(x1)*np.cos(x1)**2)
 
 mplm.data_marker(x=0)
 ```
```

### Comparing `mpl-markers-0.0.1/pyproject.toml` & `mpl-markers-0.0.2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires      = ["setuptools>=61.0.0", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "mpl-markers"
-version = "0.0.1"
+version = "0.0.2"
 description = "interactive marker support for matplotlib"
 readme = "README.md"
 authors = [{ name = "Rick Lyon", email = "rlyon14@gmail.com" }]
 license = { file = "LICENSE" }
 classifiers = [
     "License :: OSI Approved :: MIT License",
     "Programming Language :: Python",
```

### Comparing `mpl-markers-0.0.1/tests/test_markers.py` & `mpl-markers-0.0.2/tests/test_markers.py`

 * *Files 2% similar despite different names*

```diff
@@ -74,18 +74,18 @@
         # d[700:750]  = np.nan
 
         ax1.plot(np.real(d), np.imag(d))
 
         # set marker to angle. The xdata for the marker is the real component of d, so to set the angle we need to specify the index
         angle = 3/4
 
-        def yfmt(x, y, **kwargs):
-            return '{:.3f}$\pi$'.format(x)
+        def yfmt(x, y, idx):
+            return '{:.3f}$\pi$'.format(y)
 
-        def xfmt(x, y, **kwargs):
+        def xfmt(x, y, idx):
             return '{:.3f}$\pi$'.format(x)
 
         m = mplm.data_marker(x=angle, yline=True, alias_xdata=x1_pi, yformatter=yfmt, xformatter=xfmt)
 
         plt.show()
 
     # @unittest.skip
```

