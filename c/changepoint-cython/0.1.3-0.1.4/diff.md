# Comparing `tmp/changepoint_cython-0.1.3.tar.gz` & `tmp/changepoint_cython-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/changepoint_cython-0.1.3.tar", last modified: Sun Jun 21 18:20:42 2020, max compression
+gzip compressed data, was "changepoint_cython-0.1.4.tar", max compression
```

## Comparing `changepoint_cython-0.1.3.tar` & `changepoint_cython-0.1.4.tar`

### file list

```diff
@@ -1,39 +1,15 @@
-drwxr-xr-x   0 brunedv   (1000) brunedv   (1000)        0 2020-06-21 18:20:42.000000 changepoint_cython-0.1.3/
-drwxr-xr-x   0 brunedv   (1000) brunedv   (1000)        0 2020-06-21 18:20:42.000000 changepoint_cython-0.1.3/changepoint_cython.egg-info/
--rw-r--r--   0 brunedv   (1000) brunedv   (1000)      856 2020-06-21 18:20:42.000000 changepoint_cython-0.1.3/changepoint_cython.egg-info/SOURCES.txt
--rw-r--r--   0 brunedv   (1000) brunedv   (1000)        1 2020-06-21 18:20:42.000000 changepoint_cython-0.1.3/changepoint_cython.egg-info/dependency_links.txt
--rw-r--r--   0 brunedv   (1000) brunedv   (1000)      292 2020-06-21 18:20:42.000000 changepoint_cython-0.1.3/changepoint_cython.egg-info/PKG-INFO
--rw-r--r--   0 brunedv   (1000) brunedv   (1000)       15 2020-06-21 18:20:42.000000 changepoint_cython-0.1.3/changepoint_cython.egg-info/top_level.txt
--rw-r--r--   0 brunedv   (1000) brunedv   (1000)       33 2020-06-21 18:20:42.000000 changepoint_cython-0.1.3/changepoint_cython.egg-info/requires.txt
-drwxr-xr-x   0 brunedv   (1000) brunedv   (1000)        0 2020-06-21 18:20:42.000000 changepoint_cython-0.1.3/pychangepoints/
--rw-r--r--   0 brunedv   (1000) brunedv   (1000)   287253 2020-06-21 18:20:41.000000 changepoint_cython-0.1.3/pychangepoints/pelt_cython.html
--rw-r--r--   0 brunedv   (1000) brunedv   (1000)     3851 2020-06-21 14:51:03.000000 changepoint_cython-0.1.3/pychangepoints/nppelt.pyx
--rw-r--r--   0 brunedv   (1000) brunedv   (1000)      499 2020-06-21 14:51:03.000000 changepoint_cython-0.1.3/pychangepoints/utils.pxd
--rw-r--r--   0 brunedv   (1000) brunedv   (1000)     3684 2020-06-21 14:51:03.000000 changepoint_cython-0.1.3/pychangepoints/cost_function.pxd
--rw-r--r--   0 brunedv   (1000) brunedv   (1000)   268674 2020-06-21 18:20:36.000000 changepoint_cython-0.1.3/pychangepoints/mutiple_algos.html
--rw-r--r--   0 brunedv   (1000) brunedv   (1000)    11407 2020-06-21 14:51:03.000000 changepoint_cython-0.1.3/pychangepoints/pelt_cython.pyx
--rw-r--r--   0 brunedv   (1000) brunedv   (1000)  1094260 2020-06-21 18:20:36.000000 changepoint_cython-0.1.3/pychangepoints/mutiple_algos.c
--rw-r--r--   0 brunedv   (1000) brunedv   (1000)     7766 2020-06-21 14:51:03.000000 changepoint_cython-0.1.3/pychangepoints/mutiple_algos.pyx
--rw-r--r--   0 brunedv   (1000) brunedv   (1000)   955772 2020-06-21 18:20:38.000000 changepoint_cython-0.1.3/pychangepoints/nppelt.c
--rw-r--r--   0 brunedv   (1000) brunedv   (1000)       67 2020-06-21 14:51:03.000000 changepoint_cython-0.1.3/pychangepoints/__init__.py
--rw-r--r--   0 brunedv   (1000) brunedv   (1000)  1129828 2020-06-21 18:20:41.000000 changepoint_cython-0.1.3/pychangepoints/pelt_cython.c
--rw-r--r--   0 brunedv   (1000) brunedv   (1000)     1289 2020-06-21 14:51:03.000000 changepoint_cython-0.1.3/pychangepoints/cost_function_multiple.pxd
--rw-r--r--   0 brunedv   (1000) brunedv   (1000)     5585 2020-06-21 14:51:03.000000 changepoint_cython-0.1.3/pychangepoints/algo_changepoints.py
--rw-r--r--   0 brunedv   (1000) brunedv   (1000)     1222 2020-06-21 14:51:03.000000 changepoint_cython-0.1.3/.gitignore
-drwxr-xr-x   0 brunedv   (1000) brunedv   (1000)        0 2020-06-21 18:20:42.000000 changepoint_cython-0.1.3/.github/
-drwxr-xr-x   0 brunedv   (1000) brunedv   (1000)        0 2020-06-21 18:20:42.000000 changepoint_cython-0.1.3/.github/workflows/
--rw-r--r--   0 brunedv   (1000) brunedv   (1000)     1317 2020-06-21 14:51:03.000000 changepoint_cython-0.1.3/.github/workflows/python-package.yml
--rw-r--r--   0 brunedv   (1000) brunedv   (1000)    35149 2020-06-21 14:51:03.000000 changepoint_cython-0.1.3/LICENSE
--rw-r--r--   0 brunedv   (1000) brunedv   (1000)       39 2020-06-21 14:51:03.000000 changepoint_cython-0.1.3/requirements.txt
--rw-r--r--   0 brunedv   (1000) brunedv   (1000)     1237 2020-06-21 18:19:32.000000 changepoint_cython-0.1.3/setup.py
--rw-r--r--   0 brunedv   (1000) brunedv   (1000)      292 2020-06-21 18:20:42.000000 changepoint_cython-0.1.3/PKG-INFO
--rw-r--r--   0 brunedv   (1000) brunedv   (1000)     1185 2020-06-21 14:51:03.000000 changepoint_cython-0.1.3/test_segmentation_multiple.py
--rw-r--r--   0 brunedv   (1000) brunedv   (1000)     1624 2020-06-21 14:51:03.000000 changepoint_cython-0.1.3/test_segmentation.py
-drwxr-xr-x   0 brunedv   (1000) brunedv   (1000)        0 2020-06-21 18:20:42.000000 changepoint_cython-0.1.3/data/
--rw-r--r--   0 brunedv   (1000) brunedv   (1000)  2585858 2020-06-21 14:51:03.000000 changepoint_cython-0.1.3/data/2120913D.las
--rw-r--r--   0 brunedv   (1000) brunedv   (1000)    48704 2020-06-21 14:51:03.000000 changepoint_cython-0.1.3/data/segmentation.png
--rw-r--r--   0 brunedv   (1000) brunedv   (1000)  6672412 2020-06-21 14:51:03.000000 changepoint_cython-0.1.3/segmentation example on well log data.ipynb
--rw-r--r--   0 brunedv   (1000) brunedv   (1000)       38 2020-06-21 18:20:42.000000 changepoint_cython-0.1.3/setup.cfg
-drwxr-xr-x   0 brunedv   (1000) brunedv   (1000)        0 2020-06-21 18:20:42.000000 changepoint_cython-0.1.3/tests/
--rw-r--r--   0 brunedv   (1000) brunedv   (1000)     1032 2020-06-21 14:51:03.000000 changepoint_cython-0.1.3/tests/test_seg.py
--rw-r--r--   0 brunedv   (1000) brunedv   (1000)     4474 2020-06-21 14:51:03.000000 changepoint_cython-0.1.3/README.md
+-rw-r--r--   0        0        0    35149 2023-05-21 14:15:30.689733 changepoint_cython-0.1.4/LICENSE
+-rw-r--r--   0        0        0     4474 2023-05-21 14:15:30.689733 changepoint_cython-0.1.4/README.md
+-rw-r--r--   0        0        0     1577 2023-05-21 14:15:30.689733 changepoint_cython-0.1.4/build.py
+-rw-r--r--   0        0        0       67 2023-05-21 14:15:30.701733 changepoint_cython-0.1.4/pychangepoints/__init__.py
+-rw-r--r--   0        0        0     5733 2023-05-21 14:15:30.701733 changepoint_cython-0.1.4/pychangepoints/algo_changepoints.py
+-rw-r--r--   0        0        0     3684 2023-05-21 14:15:30.701733 changepoint_cython-0.1.4/pychangepoints/cost_function.pxd
+-rw-r--r--   0        0        0     1289 2023-05-21 14:15:30.701733 changepoint_cython-0.1.4/pychangepoints/cost_function_multiple.pxd
+-rw-r--r--   0        0        0   220882 2023-05-21 14:15:30.701733 changepoint_cython-0.1.4/pychangepoints/mutiple_algos.html
+-rw-r--r--   0        0        0     7734 2023-05-21 14:15:30.701733 changepoint_cython-0.1.4/pychangepoints/mutiple_algos.pyx
+-rw-r--r--   0        0        0     3850 2023-05-21 14:15:30.701733 changepoint_cython-0.1.4/pychangepoints/nppelt.pyx
+-rw-r--r--   0        0        0   236694 2023-05-21 14:15:30.705733 changepoint_cython-0.1.4/pychangepoints/pelt_cython.html
+-rw-r--r--   0        0        0    11409 2023-05-21 14:15:30.705733 changepoint_cython-0.1.4/pychangepoints/pelt_cython.pyx
+-rw-r--r--   0        0        0      499 2023-05-21 14:15:30.705733 changepoint_cython-0.1.4/pychangepoints/utils.pxd
+-rw-r--r--   0        0        0      847 2023-05-21 14:15:30.705733 changepoint_cython-0.1.4/pyproject.toml
+-rw-r--r--   0        0        0     5058 1970-01-01 00:00:00.000000 changepoint_cython-0.1.4/PKG-INFO
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `changepoint_cython-0.1.3/pychangepoints/nppelt.pyx` & `changepoint_cython-0.1.4/pychangepoints/nppelt.pyx`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,15 @@
-import numpy as np 
-cimport numpy as np 
-import math 
-cimport cython
-from libc.math cimport sqrt, log, M_PI, fmax, isnan
+import numpy as np
+
+cimport numpy as np
 
+import math
+
+cimport cython
+from libc.math cimport M_PI, fmax, isnan, log, sqrt
 
 DTYPE = np.float64
 ITYPE = np.int64
 ctypedef np.float64_t DTYPE_t
 ctypedef np.int64_t ITYPE_t
 
 @cython.wraparound(False)
```

### Comparing `changepoint_cython-0.1.3/pychangepoints/cost_function.pxd` & `changepoint_cython-0.1.4/pychangepoints/cost_function.pxd`

 * *Files 2% similar despite different names*

```diff
@@ -1,18 +1,21 @@
-import numpy as np 
-cimport numpy as np 
-import math 
+import numpy as np
+
+cimport numpy as np
+
+import math
+
 cimport cython
 
 DTYPE = np.float64
 ITYPE = np.int64
 ctypedef np.float64_t DTYPE_t
 ctypedef np.int64_t ITYPE_t
 
-from libc.math cimport sqrt, log, M_PI, fmax, isnan
+from libc.math cimport M_PI, fmax, isnan, log, sqrt
 
 
 @cython.wraparound(False)
 @cython.boundscheck(False)
 @cython.cdivision(True)
 #@cython.cdivision(False) 
 cdef inline DTYPE_t mll_mean(DTYPE_t x, DTYPE_t x2, DTYPE_t x3, ITYPE_t n) nogil:
```

### Comparing `changepoint_cython-0.1.3/pychangepoints/pelt_cython.pyx` & `changepoint_cython-0.1.4/pychangepoints/pelt_cython.pyx`

 * *Files 2% similar despite different names*

```diff
@@ -1,21 +1,32 @@
-import numpy as np 
-cimport numpy as np 
-import math 
-cimport cython
+import numpy as np
 
-from libc.math cimport sqrt, log, M_PI, fmax, isnan
-cimport cost_function
-from cost_function cimport mll_mean, mll_var, mll_meanvar, mll_meanvar_exp, mll_meanvar_poisson, mbic_var, mbic_meanvar, mbic_mean, mbic_meanvar_exp, mbic_meanvar_poisson
-from cost_function cimport mll_nonparametric_ed, mll_nonparametric_ed_mbic
+cimport numpy as np
 
-cimport utils
-from utils cimport order_vec
-from cython.parallel import prange
+import math
 
+cimport cython
+from .cost_function cimport (
+    mbic_mean,
+    mbic_meanvar,
+    mbic_meanvar_exp,
+    mbic_meanvar_poisson,
+    mbic_var,
+    mll_mean,
+    mll_meanvar,
+    mll_meanvar_exp,
+    mll_meanvar_poisson,
+    mll_nonparametric_ed,
+    mll_nonparametric_ed_mbic,
+    mll_var,
+)
+from libc.math cimport M_PI, fmax, isnan, log, sqrt
+from .utils cimport order_vec
+
+from cython.parallel import prange
 
 DTYPE = np.float64
 ITYPE = np.int64
 ctypedef np.float64_t DTYPE_t
 ctypedef np.int64_t ITYPE_t
```

### Comparing `changepoint_cython-0.1.3/pychangepoints/mutiple_algos.pyx` & `changepoint_cython-0.1.4/pychangepoints/mutiple_algos.pyx`

 * *Files 2% similar despite different names*

```diff
@@ -1,16 +1,16 @@
-import math 
-import numpy as np 
-from libc.math cimport sqrt
+import math
+
+import numpy as np
 
-cimport numpy as np 
 cimport cython
-cimport cost_function_multiple
+cimport numpy as np
+from .cost_function_multiple cimport mbic_mean, mll_mean, order_vec
+from libc.math cimport sqrt
 
-from cost_function_multiple cimport mll_mean, mbic_mean, order_vec
 from cython.parallel import prange
 
 DTYPE = np.float64
 ITYPE = np.int64
 ctypedef np.float64_t DTYPE_t
 ctypedef np.int64_t ITYPE_t
```

### Comparing `changepoint_cython-0.1.3/pychangepoints/cost_function_multiple.pxd` & `changepoint_cython-0.1.4/pychangepoints/cost_function_multiple.pxd`

 * *Files 1% similar despite different names*

```diff
@@ -1,18 +1,21 @@
-import numpy as np 
-cimport numpy as np 
-import math 
+import numpy as np
+
+cimport numpy as np
+
+import math
+
 cimport cython
 
 DTYPE = np.float64
 ITYPE = np.int64
 ctypedef np.float64_t DTYPE_t
 ctypedef np.int64_t ITYPE_t
 
-from libc.math cimport sqrt, log, M_PI, fmax, isnan
+from libc.math cimport M_PI, fmax, isnan, log, sqrt
 
 
 @cython.wraparound(False)
 @cython.boundscheck(False)
 cdef inline DTYPE_t mll_mean(DTYPE_t x, DTYPE_t x2 , DTYPE_t x3, ITYPE_t n, ITYPE_t dim) nogil:
     return (x2-(x*x)*1/(n))
```

### Comparing `changepoint_cython-0.1.3/pychangepoints/algo_changepoints.py` & `changepoint_cython-0.1.4/pychangepoints/algo_changepoints.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,147 +1,163 @@
 """
 Main functions of the package linked with cython
 """
 import numpy as np
 import pandas as pd
-
 from sklearn.decomposition import PCA
 
-
-from .cython_pelt import cpelt, cbin_seg, cseg_neigh
+from .cython_pelt import cbin_seg, cpelt, cseg_neigh
 from .multiple_dim import cbin_seg_multiple, cpelt_multiple, cseg_neigh_multiple
 from .nonparametric import cnp_pelt
 
 
 def multiple_preprocessing(data_frame):
     """
     Preprocessing of the multivariate data before segmentation
     Standardization with PCA
     """
-    data_scale = data_frame.sub(data_frame.mean(0).values, axis=1)\
-        .div(data_frame.std(0).values, axis=1)
+    data_scale = data_frame.sub(data_frame.mean(0).values, axis=1).div(
+        data_frame.std(0).values, axis=1
+    )
     pca = PCA()
     pca.fit(data_scale)
     pca_scale = pca.transform(data_scale)
     pca_frame = pd.DataFrame(pca_scale)
-    pca_frame_scale = pca_frame.sub(pca_frame.mean(0), axis=1).div(pca_frame.std(0), axis=1)
+    pca_frame_scale = pca_frame.sub(pca_frame.mean(0), axis=1).div(
+        pca_frame.std(0), axis=1
+    )
     return pca_frame_scale
 
+
 def nonpamametric_ed_sumstat(data, n_stats=10):
     """
     Compute moments of the time series
     """
     ts_data = data.iloc[:, 0]
-    size_data = len(ts_data)-1
+    size_data = len(ts_data) - 1
     n_stats = min(n_stats, size_data)
-    resultat = np.zeros((n_stats, size_data+1))
+    resultat = np.zeros((n_stats, size_data + 1))
     ts_data_array = ts_data.sort_values(ascending=True).values
-    y_k = -1 + (2*np.arange(1, n_stats+1)/n_stats-1/n_stats)
-    log_size = -np.log(2*size_data-1)
-    p_k = (1+np.exp(log_size*y_k))**(-1)
+    y_k = -1 + (2 * np.arange(1, n_stats + 1) / n_stats - 1 / n_stats)
+    log_size = -np.log(2 * size_data - 1)
+    p_k = (1 + np.exp(log_size * y_k)) ** (-1)
     for i in range(1, n_stats):
-        j = int((size_data-1)*p_k[i] + 1)
-        resultat[i, :] = np.cumsum(ts_data.values < ts_data_array[j])+\
-            0.5*np.cumsum(ts_data.values == ts_data_array[j])
+        j = int((size_data - 1) * p_k[i] + 1)
+        resultat[i, :] = np.cumsum(ts_data.values < ts_data_array[j]) + 0.5 * np.cumsum(
+            ts_data.values == ts_data_array[j]
+        )
     return resultat
 
+
 def pelt(data, pen_, minseg, method):
     """
     Univariate Pelt algorithm
     """
     times_series = data.values
     size_ts = len(data.index)
-    stats_ts = np.zeros((size_ts+1, 3))
+    stats_ts = np.zeros((size_ts + 1, 3))
     mean = np.mean(times_series)
     stats_ts[:, 0] = np.append(0, times_series.cumsum())
     stats_ts[:, 1] = np.append(0, (times_series**2).cumsum())
-    stats_ts[:, 2] = np.append(0, ((times_series-mean)**2).cumsum())
+    stats_ts[:, 2] = np.append(0, ((times_series - mean) ** 2).cumsum())
 
     stats_ts_pelt = np.concatenate([stats_ts[:, 0], stats_ts[:, 1], stats_ts[:, 2]])
-    return  cpelt(stats_ts_pelt, pen_*np.log(size_ts), minseg, size_ts, method)
+    return cpelt(stats_ts_pelt, pen_ * np.log(size_ts), minseg, size_ts, method)
+
 
 def np_pelt(data, pen_, minseg=10, nquantiles=10, method="mbic_nonparametric_ed"):
     """
     Univariate Pelt non parametric algorithm
     """
     times_series = data.values
     size_ts = times_series.shape[0]
     method_ = method
-    nquantiles_ = int(2*np.log(size_ts))
+    nquantiles_ = int(2 * np.log(size_ts))
     sumstat = nonpamametric_ed_sumstat(data, nquantiles_)
-    return  cnp_pelt(sumstat, pen_, minseg, size_ts-1, nquantiles_, method_)
+    return cnp_pelt(sumstat, pen_, minseg, size_ts - 1, nquantiles_, method_)
+
 
 def segneigh(data, nb_cpts, method):
     """
     Univariate segmenttation neighboorhood algorithm
     """
     times_series = data.values
     mean = np.mean(times_series)
     size_ts = times_series.shape[0]
-    stats_ts = np.zeros((size_ts+1, 3))
+    stats_ts = np.zeros((size_ts + 1, 3))
     stats_ts[:, 0] = np.append(0, times_series.cumsum())
     stats_ts[:, 1] = np.append(0, (times_series**2).cumsum())
-    stats_ts[:, 2] = np.append(0, ((times_series-mean)**2).cumsum())
+    stats_ts[:, 2] = np.append(0, ((times_series - mean) ** 2).cumsum())
 
     return cseg_neigh(stats_ts, nb_cpts, method)
 
+
 def binseg(data, nb_cpts, minseg, method):
     """
     Univariate binary segmentation
     """
     times_series = data.values
     mean = np.mean(times_series)
     size_ts = times_series.shape[0]
-    stats_ts = np.zeros((size_ts+1, 3))
+    stats_ts = np.zeros((size_ts + 1, 3))
     stats_ts[:, 0] = np.append(0, times_series.cumsum())
     stats_ts[:, 1] = np.append(0, (times_series**2).cumsum())
-    stats_ts[:, 2] = np.append(0, ((times_series-mean)**2).cumsum())
+    stats_ts[:, 2] = np.append(0, ((times_series - mean) ** 2).cumsum())
 
     return cbin_seg(stats_ts, nb_cpts, minseg, method)
 
+
 def binseg_multiple(data, nb_cpts, minseg, method):
     """
     Multivariate binary segmentation
     """
     data_process = multiple_preprocessing(data)
     times_series = data_process.values
     mean = np.mean(times_series, axis=0)
     size_ts = times_series.shape[0]
     dim_ts = times_series.shape[1]
-    stats_ts = np.zeros((size_ts+1, 3, dim_ts))
+    stats_ts = np.zeros((size_ts + 1, 3, dim_ts))
     zeros = np.zeros(dim_ts)
     stats_ts[:, 0, :] = np.insert(times_series.cumsum(axis=0), 0, zeros, axis=0)
     stats_ts[:, 1, :] = np.insert((times_series**2).cumsum(axis=0), 0, zeros, axis=0)
-    stats_ts[:, 2, :] = np.insert(((times_series-mean)**2).cumsum(axis=0), 0, zeros, axis=0)
+    stats_ts[:, 2, :] = np.insert(
+        ((times_series - mean) ** 2).cumsum(axis=0), 0, zeros, axis=0
+    )
     return cbin_seg_multiple(stats_ts, nb_cpts, minseg, method)
 
+
 def pelt_multiple(data, pen_, minseg, method):
     """
     Multivariate PELT segmentation algorithm
     """
     data_process = multiple_preprocessing(data)
     times_series = data_process.values
     mean = np.mean(times_series, axis=0)
     size_ts = times_series.shape[0]
     dim_ts = times_series.shape[1]
-    stats_ts = np.zeros((size_ts+1, 3, dim_ts))
+    stats_ts = np.zeros((size_ts + 1, 3, dim_ts))
     zeros = np.zeros(dim_ts)
     stats_ts[:, 0, :] = np.insert(times_series.cumsum(axis=0), 0, zeros, axis=0)
     stats_ts[:, 1, :] = np.insert((times_series**2).cumsum(axis=0), 0, zeros, axis=0)
-    stats_ts[:, 2, :] = np.insert(((times_series-mean)**2).cumsum(axis=0), 0, zeros, axis=0)
-    return  cpelt_multiple(stats_ts, pen_*np.log(size_ts), minseg, size_ts, method)
+    stats_ts[:, 2, :] = np.insert(
+        ((times_series - mean) ** 2).cumsum(axis=0), 0, zeros, axis=0
+    )
+    return cpelt_multiple(stats_ts, pen_ * np.log(size_ts), minseg, size_ts, method)
+
 
 def segneigh_multiple(data, nb_cpts, method):
     """
     Multivariate Segmentation neigborhhod algorithm
     """
     data_process = multiple_preprocessing(data)
     times_series = data_process.values
     mean = np.mean(times_series, axis=0)
     size_ts = times_series.shape[0]
     dim_ts = times_series.shape[1]
-    stats_ts = np.zeros((size_ts+1, 3, dim_ts))
+    stats_ts = np.zeros((size_ts + 1, 3, dim_ts))
     zeros = np.zeros(dim_ts)
     stats_ts[:, 0, :] = np.insert(times_series.cumsum(axis=0), 0, zeros, axis=0)
     stats_ts[:, 1, :] = np.insert((times_series**2).cumsum(axis=0), 0, zeros, axis=0)
-    stats_ts[:, 2, :] = np.insert(((times_series-mean)**2).cumsum(axis=0), 0, zeros, axis=0)
-    return cseg_neigh_multiple(stats_ts, nb_cpts, method)
+    stats_ts[:, 2, :] = np.insert(
+        ((times_series - mean) ** 2).cumsum(axis=0), 0, zeros, axis=0
+    )
+    return cseg_neigh_multiple(stats_ts, nb_cpts, method)
```

### Comparing `changepoint_cython-0.1.3/LICENSE` & `changepoint_cython-0.1.4/LICENSE`

 * *Files identical despite different names*

### Comparing `changepoint_cython-0.1.3/README.md` & `changepoint_cython-0.1.4/README.md`

 * *Files identical despite different names*

