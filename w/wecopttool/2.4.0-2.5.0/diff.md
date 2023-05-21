# Comparing `tmp/wecopttool-2.4.0.tar.gz` & `tmp/wecopttool-2.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "wecopttool-2.4.0.tar", last modified: Fri Apr 14 16:11:47 2023, max compression
+gzip compressed data, was "wecopttool-2.5.0.tar", last modified: Sun May 21 07:14:41 2023, max compression
```

## Comparing `wecopttool-2.4.0.tar` & `wecopttool-2.5.0.tar`

### file list

```diff
@@ -1,26 +1,26 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 16:11:47.452280 wecopttool-2.4.0/
--rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-04-14 16:11:36.000000 wecopttool-2.4.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      811 2023-04-14 16:11:36.000000 wecopttool-2.4.0/NOTICE
--rw-r--r--   0 runner    (1001) docker     (123)     3314 2023-04-14 16:11:47.452280 wecopttool-2.4.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2738 2023-04-14 16:11:36.000000 wecopttool-2.4.0/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     1033 2023-04-14 16:11:36.000000 wecopttool-2.4.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-14 16:11:47.452280 wecopttool-2.4.0/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 16:11:47.448280 wecopttool-2.4.0/tests/
--rw-r--r--   0 runner    (1001) docker     (123)    50582 2023-04-14 16:11:36.000000 wecopttool-2.4.0/tests/test_core.py
--rw-r--r--   0 runner    (1001) docker     (123)     6130 2023-04-14 16:11:36.000000 wecopttool-2.4.0/tests/test_hydrostatics.py
--rw-r--r--   0 runner    (1001) docker     (123)    12231 2023-04-14 16:11:36.000000 wecopttool-2.4.0/tests/test_integration.py
--rw-r--r--   0 runner    (1001) docker     (123)     8032 2023-04-14 16:11:36.000000 wecopttool-2.4.0/tests/test_pto.py
--rw-r--r--   0 runner    (1001) docker     (123)    16883 2023-04-14 16:11:36.000000 wecopttool-2.4.0/tests/test_waves.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 16:11:47.452280 wecopttool-2.4.0/wecopttool/
--rw-r--r--   0 runner    (1001) docker     (123)     2795 2023-04-14 16:11:36.000000 wecopttool-2.4.0/wecopttool/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    82645 2023-04-14 16:11:36.000000 wecopttool-2.4.0/wecopttool/core.py
--rw-r--r--   0 runner    (1001) docker     (123)     7957 2023-04-14 16:11:36.000000 wecopttool-2.4.0/wecopttool/geom.py
--rw-r--r--   0 runner    (1001) docker     (123)     5224 2023-04-14 16:11:36.000000 wecopttool-2.4.0/wecopttool/hydrostatics.py
--rw-r--r--   0 runner    (1001) docker     (123)    34521 2023-04-14 16:11:36.000000 wecopttool-2.4.0/wecopttool/pto.py
--rw-r--r--   0 runner    (1001) docker     (123)    17475 2023-04-14 16:11:36.000000 wecopttool-2.4.0/wecopttool/waves.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 16:11:47.452280 wecopttool-2.4.0/wecopttool.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3314 2023-04-14 16:11:47.000000 wecopttool-2.4.0/wecopttool.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      444 2023-04-14 16:11:47.000000 wecopttool-2.4.0/wecopttool.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-14 16:11:47.000000 wecopttool-2.4.0/wecopttool.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      230 2023-04-14 16:11:47.000000 wecopttool-2.4.0/wecopttool.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       11 2023-04-14 16:11:47.000000 wecopttool-2.4.0/wecopttool.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 07:14:41.319364 wecopttool-2.5.0/
+-rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-05-21 07:14:27.000000 wecopttool-2.5.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      811 2023-05-21 07:14:27.000000 wecopttool-2.5.0/NOTICE
+-rw-r--r--   0 runner    (1001) docker     (123)     3274 2023-05-21 07:14:41.319364 wecopttool-2.5.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2702 2023-05-21 07:14:27.000000 wecopttool-2.5.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1029 2023-05-21 07:14:27.000000 wecopttool-2.5.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-21 07:14:41.319364 wecopttool-2.5.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 07:14:41.315364 wecopttool-2.5.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)    55413 2023-05-21 07:14:27.000000 wecopttool-2.5.0/tests/test_core.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6130 2023-05-21 07:14:27.000000 wecopttool-2.5.0/tests/test_hydrostatics.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12237 2023-05-21 07:14:27.000000 wecopttool-2.5.0/tests/test_integration.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8007 2023-05-21 07:14:27.000000 wecopttool-2.5.0/tests/test_pto.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16883 2023-05-21 07:14:27.000000 wecopttool-2.5.0/tests/test_waves.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 07:14:41.315364 wecopttool-2.5.0/wecopttool/
+-rw-r--r--   0 runner    (1001) docker     (123)     2787 2023-05-21 07:14:27.000000 wecopttool-2.5.0/wecopttool/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    85594 2023-05-21 07:14:27.000000 wecopttool-2.5.0/wecopttool/core.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7957 2023-05-21 07:14:27.000000 wecopttool-2.5.0/wecopttool/geom.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5224 2023-05-21 07:14:27.000000 wecopttool-2.5.0/wecopttool/hydrostatics.py
+-rw-r--r--   0 runner    (1001) docker     (123)    34338 2023-05-21 07:14:27.000000 wecopttool-2.5.0/wecopttool/pto.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18012 2023-05-21 07:14:27.000000 wecopttool-2.5.0/wecopttool/waves.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 07:14:41.315364 wecopttool-2.5.0/wecopttool.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3274 2023-05-21 07:14:41.000000 wecopttool-2.5.0/wecopttool.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      444 2023-05-21 07:14:41.000000 wecopttool-2.5.0/wecopttool.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-21 07:14:41.000000 wecopttool-2.5.0/wecopttool.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      230 2023-05-21 07:14:41.000000 wecopttool-2.5.0/wecopttool.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       11 2023-05-21 07:14:41.000000 wecopttool-2.5.0/wecopttool.egg-info/top_level.txt
```

### Comparing `wecopttool-2.4.0/LICENSE` & `wecopttool-2.5.0/LICENSE`

 * *Files identical despite different names*

### Comparing `wecopttool-2.4.0/NOTICE` & `wecopttool-2.5.0/NOTICE`

 * *Files identical despite different names*

### Comparing `wecopttool-2.4.0/PKG-INFO` & `wecopttool-2.5.0/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,34 +1,34 @@
 Metadata-Version: 2.1
 Name: wecopttool
-Version: 2.4.0
+Version: 2.5.0
 Summary: WEC Design Optimization Toolbox
 Author: Sandia National Laboratories
 License: GNU General Public License v3 (GPLv3)
-Project-URL: Documentation, https://snl-waterpower.github.io/WecOptTool/
+Project-URL: Documentation, https://sandialabs.github.io/WecOptTool/
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 Provides-Extra: dev
 Provides-Extra: geometry
 License-File: LICENSE
 License-File: NOTICE
 
-[![Test-WecOptTool](https://github.com/SNL-WaterPower/WecOptTool/actions/workflows/push.yml/badge.svg)](https://github.com/SNL-WaterPower/WecOptTool/actions/workflows/push.yml)
-[![Coverage Status](https://coveralls.io/repos/github/SNL-WaterPower/WecOptTool/badge.svg?branch=main)](https://coveralls.io/github/SNL-WaterPower/WecOptTool?branch=main)
+[![Test-WecOptTool](https://github.com/sandialabs/WecOptTool/actions/workflows/push.yml/badge.svg)](https://github.com/sandialabs/WecOptTool/actions/workflows/push.yml)
+[![Coverage Status](https://coveralls.io/repos/github/sandialabs/WecOptTool/badge.svg?branch=main)](https://coveralls.io/github/sandialabs/WecOptTool?branch=main)
 
 # WecOptTool
 The Wave Energy Converter Design Optimization Toolbox (WecOptTool) allows users to perform wave energy converter (WEC) device design optimization studies with constrained optimal control.
 
 **NOTE:** If you are looking for the WecOptTool code used in previous published work (MATLAB version) please see [WecOptTool-MATLAB](https://github.com/SNL-WaterPower/WecOptTool-MATLAB).
 
 ## Project Information
-Refer to [WecOptTool documentation](https://snl-waterpower.github.io/WecOptTool/) for more information, including project overview, tutorials, theory, and API documentation.
+Refer to [WecOptTool documentation](https://sandialabs.github.io/WecOptTool/) for more information, including project overview, tutorials, theory, and API documentation.
 
 ## Getting started
 WecOptTool requires Python >= 3.8. Python 3.9 & 3.10 are supported.
 It is strongly recommended you create a dedicated virtual environment (e.g., using `conda`, `venv`, etc.) before installing `wecopttool`.
 
 **Option 1** - using `Conda`:
 
@@ -61,18 +61,18 @@
 
 ## Tutorials
 The tutorials can be found in the `examples` directory and are written as [Jupyter Notebooks](https://jupyter.org/).
 To run the tutorials, first download the notebook files and then, from the directory containing the notebooks, run `jupyter notebook`.
 Using `git` to obtain the notebooks this can be done by running
 
 ```bash
-git clone https://github.com/SNL-WaterPower/WecOptTool.git
+git clone https://github.com/sandialabs/WecOptTool.git
 cd WecOptTool/examples
 jupyter notebook
 ```
 
 ## Getting help
-To report bugs, use WecOptTool's [issues page](https://github.com/SNL-WaterPower/WecOptTool/issues).
-For general discussion, use WecOptTool's [discussion page](https://github.com/SNL-WaterPower/WecOptTool/discussions)
+To report bugs, use WecOptTool's [issues page](https://github.com/sandialabs/WecOptTool/issues).
+For general discussion, use WecOptTool's [discussion page](https://github.com/sandialabs/WecOptTool/discussions)
 
 ## Contributing
-If you are interested in contributing to WecOptTool, see our [contribution guidelines](https://github.com/SNL-WaterPower/WecOptTool/blob/main/.github/CONTRIBUTING.md).
+If you are interested in contributing to WecOptTool, see our [contribution guidelines](https://github.com/sandialabs/WecOptTool/blob/main/.github/CONTRIBUTING.md).
```

### Comparing `wecopttool-2.4.0/README.md` & `wecopttool-2.5.0/README.md`

 * *Files 10% similar despite different names*

```diff
@@ -1,17 +1,17 @@
-[![Test-WecOptTool](https://github.com/SNL-WaterPower/WecOptTool/actions/workflows/push.yml/badge.svg)](https://github.com/SNL-WaterPower/WecOptTool/actions/workflows/push.yml)
-[![Coverage Status](https://coveralls.io/repos/github/SNL-WaterPower/WecOptTool/badge.svg?branch=main)](https://coveralls.io/github/SNL-WaterPower/WecOptTool?branch=main)
+[![Test-WecOptTool](https://github.com/sandialabs/WecOptTool/actions/workflows/push.yml/badge.svg)](https://github.com/sandialabs/WecOptTool/actions/workflows/push.yml)
+[![Coverage Status](https://coveralls.io/repos/github/sandialabs/WecOptTool/badge.svg?branch=main)](https://coveralls.io/github/sandialabs/WecOptTool?branch=main)
 
 # WecOptTool
 The Wave Energy Converter Design Optimization Toolbox (WecOptTool) allows users to perform wave energy converter (WEC) device design optimization studies with constrained optimal control.
 
 **NOTE:** If you are looking for the WecOptTool code used in previous published work (MATLAB version) please see [WecOptTool-MATLAB](https://github.com/SNL-WaterPower/WecOptTool-MATLAB).
 
 ## Project Information
-Refer to [WecOptTool documentation](https://snl-waterpower.github.io/WecOptTool/) for more information, including project overview, tutorials, theory, and API documentation.
+Refer to [WecOptTool documentation](https://sandialabs.github.io/WecOptTool/) for more information, including project overview, tutorials, theory, and API documentation.
 
 ## Getting started
 WecOptTool requires Python >= 3.8. Python 3.9 & 3.10 are supported.
 It is strongly recommended you create a dedicated virtual environment (e.g., using `conda`, `venv`, etc.) before installing `wecopttool`.
 
 **Option 1** - using `Conda`:
 
@@ -44,18 +44,18 @@
 
 ## Tutorials
 The tutorials can be found in the `examples` directory and are written as [Jupyter Notebooks](https://jupyter.org/).
 To run the tutorials, first download the notebook files and then, from the directory containing the notebooks, run `jupyter notebook`.
 Using `git` to obtain the notebooks this can be done by running
 
 ```bash
-git clone https://github.com/SNL-WaterPower/WecOptTool.git
+git clone https://github.com/sandialabs/WecOptTool.git
 cd WecOptTool/examples
 jupyter notebook
 ```
 
 ## Getting help
-To report bugs, use WecOptTool's [issues page](https://github.com/SNL-WaterPower/WecOptTool/issues).
-For general discussion, use WecOptTool's [discussion page](https://github.com/SNL-WaterPower/WecOptTool/discussions)
+To report bugs, use WecOptTool's [issues page](https://github.com/sandialabs/WecOptTool/issues).
+For general discussion, use WecOptTool's [discussion page](https://github.com/sandialabs/WecOptTool/discussions)
 
 ## Contributing
-If you are interested in contributing to WecOptTool, see our [contribution guidelines](https://github.com/SNL-WaterPower/WecOptTool/blob/main/.github/CONTRIBUTING.md).
+If you are interested in contributing to WecOptTool, see our [contribution guidelines](https://github.com/sandialabs/WecOptTool/blob/main/.github/CONTRIBUTING.md).
```

### Comparing `wecopttool-2.4.0/pyproject.toml` & `wecopttool-2.5.0/pyproject.toml`

 * *Files 19% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 [build-system]
 requires = ["setuptools"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "wecopttool"
-version = "2.4.0"
+version = "2.5.0"
 description = "WEC Design Optimization Toolbox"
 readme = "README.md"
 authors = [
     {name = "Sandia National Laboratories"},
 ]
-urls = {Documentation = "https://snl-waterpower.github.io/WecOptTool/"}
+urls = {Documentation = "https://sandialabs.github.io/WecOptTool/"}
 requires-python = ">=3.8"
 license = {text = "GNU General Public License v3 (GPLv3)"}
 classifiers = [
     "Programming Language :: Python :: 3",
     "License :: OSI Approved :: GNU General Public License v3 (GPLv3)",
     "Operating System :: OS Independent",
 ]
```

### Comparing `wecopttool-2.4.0/tests/test_core.py` & `wecopttool-2.5.0/tests/test_core.py`

 * *Files 3% similar despite different names*

```diff
@@ -430,16 +430,18 @@
         x = 1.2 + 3.4j
         X = np.reshape([0, np.real(x), np.imag(x)], [-1,1])[:-1]
         x_t = time_mat @ X
         t = wot.time(f, 1)
         assert np.allclose(x_t.squeeze(), np.real(x*np.exp(1j*w*t)))
 
 
-class TestDerivativeMat:
-    """Test function :python:`derivative_mat`."""
+class TestDerivativeMats:
+    """Test functions :python:`derivative_mat`
+    and :python:`derivative2_mat`.
+    """
 
     @pytest.fixture(scope="class")
     def f1_dm(self,):
         """Fundamental frequency [Hz] for the synthetic derivative
         matrix.
         """
         return 0.5
@@ -458,26 +460,48 @@
         mat = np.array([
             [0,  0,   0,    0],
             [0,  0, -w0,    0],
             [0, w0,   0,    0],
             [0,  0,   0,    0],
         ])
         return mat
+    
+    @pytest.fixture(scope="class")
+    def derivative2_mat(self, f1_dm):
+        """Correct/expected second derivative matrix."""
+        w0 = 2*np.pi*f1_dm
+        mat = np.array([
+            [0,      0,      0,          0],
+            [0, -w0**2,      0,          0],
+            [0,      0, -w0**2,          0],
+            [0,      0,      0, -(2*w0)**2],
+        ])
+        return mat
 
     def test_derivative_mat(self, derivative_mat, f1_dm, nfreq_dm):
         """Test the default created derivative matrix."""
         calculated = wot.derivative_mat(f1_dm, nfreq_dm)
         assert calculated==approx(derivative_mat)
 
-    def test_no_mean(self, derivative_mat, f1_dm, nfreq_dm):
+    def test_derivative2_mat(self, derivative2_mat, f1_dm, nfreq_dm):
+        """Test the default created second derivative matrix."""
+        calculated = wot.derivative2_mat(f1_dm, nfreq_dm)
+        assert calculated==approx(derivative2_mat)
+
+    def test_dmat_no_mean(self, derivative_mat, f1_dm, nfreq_dm):
         """Test the derivative matrix without the mean component."""
         calculated = wot.derivative_mat(f1_dm, nfreq_dm, False)
         assert calculated==approx(derivative_mat[1:, 1:])
 
-    def test_behavior(self,):
+    def test_d2mat_no_mean(self, derivative2_mat, f1_dm, nfreq_dm):
+        """Test the second derivative matrix without the mean component."""
+        calculated = wot.derivative2_mat(f1_dm, nfreq_dm, False)
+        assert calculated==approx(derivative2_mat[1:, 1:])
+
+    def test_dmat_behavior(self,):
         """Test that when the derivative matrix multiplies a
         state-vector it results in the correct state-vector for the
         derivative of the input response.
         """
         f = 0.1
         w = 2*np.pi*f
         x = np.array([1 + 2j,
@@ -491,14 +515,36 @@
         ])
         V = derivative_mat @ X
         v = np.sum(V[1::2]) + 1j*np.sum(V[2::2])
         expected = np.sum(
             [[(i+1) * 1j * w * x[i]] for i in range(np.size(x)-1)])
         assert np.allclose(v, expected)
 
+    def test_d2mat_behavior(self,):
+        """Test that when the second derivative matrix multiplies a
+        state-vector it results in the correct state-vector for the
+        second derivative of the input response.
+        """
+        f = 0.1
+        w = 2*np.pi*f
+        x = np.array([1 + 2j,
+                        3 + 4j,
+                        5 + 6j])
+        derivative2_mat = wot.derivative2_mat(f, np.size(x))
+        X = np.concatenate([
+            [0.],
+            np.reshape([[np.real(i), np.imag(i)] for i in x[:-1]], -1),
+            [np.real(x[-1])]
+        ])
+        V = derivative2_mat @ X
+        v = np.sum(V[1::2]) + 1j*np.sum(V[2::2])
+        expected = np.sum(
+            [[-(i * w)**2 * x[i]] for i in range(np.size(x)-1)]
+            + np.real(np.size(x) * w)**2 * x[-1])
+
 
 class TestMIMOTransferMat:
     """Test function :python:`mimo_transfer_mat`."""
 
     def test_mimo_transfer_mat(self, rao, mimo):
         """Test the function produces the correct MIMO transfer matrix.
         """
@@ -665,23 +711,27 @@
         assert np.allclose(real_1d_calculated, real_1d)
 
 
 class TestFDToTDToFD:
     """Test functions :python:`fd_to_td` and :python:`td_to_fd`."""
 
     @pytest.fixture(scope="class")
-    def components(self, nfreq):
+    def components(self):
         """Values of the two non-zero components of the response."""
         a0r, a0i = 1, 2
         a1r, a1i = 3, 4
         return (a0r, a0i, a1r, a1i)
 
     @pytest.fixture(scope="class")
     def idx(self, nfreq):
-        return np.random.randint(1, nfreq)
+        return np.random.randint(1, nfreq-1)
+    
+    @pytest.fixture(scope="class")
+    def dc(self):
+        return np.random.randint(1, 5)
 
     @pytest.fixture(scope="class")
     def fd(self, nfreq, components, idx):
         """Sample frequency domain response. There are two degrees of
         freedom and the response is zero at all but one (random)
         frequency. The non-zero values are set based on
         :python:`components`.
@@ -721,22 +771,67 @@
         """
         (a0r, a0i, _, _) = components
         freq = wot.frequency(f1, nfreq)
         time = wot.time(f1, nfreq)
         wt  = 2*np.pi*freq[idx]*time
         return a0r*np.cos(wt) - a0i*np.sin(wt)
 
+    @pytest.fixture(scope="class")
+    def fd_topfreq(self, nfreq, components):
+        """Sample frequency domain response with the nonzero components
+        in the highest (Nyquist) frequency."""
+        (a0r, _, a1r, _) = components
+        fd = np.zeros([nfreq+1, 2], dtype=complex)
+        fd[-1, 0] = a0r + 0j
+        fd[-1, 1] = a1r + 0j
+        return fd
+    
+    @pytest.fixture(scope="class")
+    def td_topfreq(self, nfreq, f1, components):
+        """Corresponding sample time domain response for the frequency
+        vector with a nonzero top (Nyquist) frequency."""
+        freq = wot.frequency(f1, nfreq)
+        time = wot.time(f1, nfreq)
+        wt  = 2*np.pi*freq[-1]*time
+        (a0r, a0i, a1r, a1i) = components
+        td = np.zeros([len(time), 2])
+        td[:, 0] = a0r*np.cos(wt) - a0i*np.sin(wt)
+        td[:, 1] = a1r*np.cos(wt) - a1i*np.sin(wt)
+        return td
+    
+    @pytest.fixture(scope="class")
+    def fd_nzmean(self, nfreq, components, idx, dc):
+        """Sample frequency domain response with a nonzero mean."""
+        (a0r, a0i, a1r, a1i) = components
+        fd = np.zeros([nfreq+1, 2], dtype=complex)
+        fd[0, :] = dc
+        fd[idx, 0] = a0r + a0i*1j
+        fd[idx, 1] = a1r + a1i*1j
+        return fd
+
+    @pytest.fixture(scope="class")
+    def td_nzmean(self, nfreq, f1, components, idx, dc):
+        """Corresponding sample time domain response with a nonzero mean."""
+        freq = wot.frequency(f1, nfreq)
+        time = wot.time(f1, nfreq)
+        wt  = 2*np.pi*freq[idx]*time
+        (a0r, a0i, a1r, a1i) = components
+        td = np.zeros([len(time), 2])
+        td[:, 0] = a0r*np.cos(wt) - a0i*np.sin(wt) + dc
+        td[:, 1] = a1r*np.cos(wt) - a1i*np.sin(wt) + dc
+        return td
+
     def test_fd_to_td(self, fd, td, f1, nfreq):
         """Test the :python:`fd_to_td` function outputs."""
         calculated = wot.fd_to_td(fd, f1, nfreq)
         assert calculated.shape==(2*nfreq, 2) and np.allclose(calculated, td)
 
-    def test_td_to_fd(self, fd, td, f1, nfreq):
+    def test_td_to_fd(self, fd, td, nfreq):
         """Test the :python:`td_to_fd` function outputs."""
-        calculated = wot.td_to_fd(td, f1, nfreq)
+        calculated = wot.td_to_fd(td)
         assert calculated.shape==(nfreq+1, 2) and np.allclose(calculated, fd)
 
     def test_fft(self, fd, td, nfreq):
         """Test the :python:`fd_to_td` function outputs when using FFT.
         """
         calculated = wot.fd_to_td(fd)
         assert calculated.shape==(2*nfreq, 2) and np.allclose(calculated, td)
@@ -746,32 +841,60 @@
         case.
         """
         calculated = wot.fd_to_td(fd_1dof, f1, nfreq)
         shape = (2*nfreq, 1)
         calc_flat = calculated.squeeze()
         assert calculated.shape==shape and np.allclose(calc_flat, td_1dof)
 
-    def test_td_to_fd_1dof(self, fd_1dof, td_1dof, f1, nfreq):
+    def test_td_to_fd_1dof(self, fd_1dof, td_1dof, nfreq):
         """Test the :python:`td_to_fd` function outputs for the 1 DOF
         case.
         """
-        calculated = wot.td_to_fd(td_1dof.squeeze(), f1, nfreq)
+        calculated = wot.td_to_fd(td_1dof.squeeze())
         shape = (nfreq+1, 1)
         calc_flat = calculated.squeeze()
         assert calculated.shape==shape and np.allclose(calc_flat, fd_1dof)
 
     def test_fft_1dof(self, fd_1dof, td_1dof, nfreq):
         """Test the :python:`fd_to_td` function outputs when using FFT
         for the 1 DOF.
         """
         calculated = wot.fd_to_td(fd_1dof)
         shape = (2*nfreq, 1)
         calc_flat = calculated.squeeze()
         assert calculated.shape==shape and np.allclose(calc_flat, td_1dof)
 
+    def test_fd_to_td_nzmean(self, fd_nzmean, td_nzmean, f1, nfreq):
+        """Test the :python: `td_to_fd` function outputs with a 
+        nonzero mean value.
+        """
+        calculated = wot.fd_to_td(fd_nzmean, f1, nfreq)
+        assert calculated.shape==(2*nfreq, 2) and np.allclose(calculated, td_nzmean)
+
+    def test_td_to_fd_nzmean(self, fd_nzmean, td_nzmean, nfreq):
+        """Test the :python: `td_to_fd` function outputs with a
+        nonzero mean value.
+        """
+        calculated = wot.td_to_fd(td_nzmean)
+        assert calculated.shape==(nfreq+1, 2) and np.allclose(calculated, fd_nzmean)
+
+    def test_fd_to_td_nzmean(self, fd_nzmean, td_nzmean, f1, nfreq):
+        """Test the :python: `td_to_fd` function outputs with the top (Nyquist)
+        frequency vector.
+        """
+        calculated = wot.fd_to_td(fd_nzmean, f1, nfreq)
+        assert calculated.shape==(2*nfreq, 2) and np.allclose(calculated, td_nzmean)
+
+    def test_td_to_fd_topfreq(self, fd_topfreq, td_topfreq, nfreq):
+        """Test the :python: `td_to_fd` function outputs for the
+        Nyquist frequency.
+        """
+        calculated = wot.td_to_fd(td_topfreq)
+        assert calculated.shape==(nfreq+1, 2) and np.allclose(calculated, fd_topfreq)
+
 
 class TestReadWriteNetCDF:
     """Test functions :python:`read_netcdf` and :python:`write_netcdf`.
     """
 
     @pytest.fixture(scope="class")
     def hydro_data_new(self, hydro_data):
```

### Comparing `wecopttool-2.4.0/tests/test_hydrostatics.py` & `wecopttool-2.5.0/tests/test_hydrostatics.py`

 * *Files identical despite different names*

### Comparing `wecopttool-2.4.0/tests/test_integration.py` & `wecopttool-2.5.0/tests/test_integration.py`

 * *Files 1% similar despite different names*

```diff
@@ -53,25 +53,24 @@
     return pto
 
 
 @pytest.fixture(scope="module")
 def fb():
     """Capytaine FloatingBody object"""
     try:
-        import wot.geom as geom
+        import wecopttool.geom as geom
     except ImportError:
         pytest.skip(
             'Skipping integration tests due to missing optional geometry ' +
             'dependencies. Run `pip install wecopttool[geometry]` to run ' +
             'these tests.'
             )
     mesh_size_factor = 0.5
     wb = geom.WaveBot()
     mesh = wb.mesh(mesh_size_factor)
-
     fb = cpy.FloatingBody.from_meshio(mesh, name="WaveBot")
     fb.add_translation_dof(name="Heave")
     return fb
 
 
 @pytest.fixture(scope="module")
 def bem(f1, nfreq, fb):
```

### Comparing `wecopttool-2.4.0/tests/test_pto.py` & `wecopttool-2.5.0/tests/test_pto.py`

 * *Files 2% similar despite different names*

```diff
@@ -127,49 +127,48 @@
         expected = np.zeros([2*ndof*n, 2*ndof*n])
         # 0,0
         imp = abcd[0, 0, :]
         r0 = np.real(imp[0])
         i0 = np.imag(imp[0])
         r1 = np.real(imp[1])
         expected[:n, :n] = np.array([
-            [0, 0,    0, 0],
+            [r0, 0,    0, 0],
             [0, r0, -i0, 0],
             [0, i0,  r0, 0],
             [0, 0,    0, r1],
         ])
         # 0,1
         imp = abcd[0, 1, :]
         r0 = np.real(imp[0])
         i0 = np.imag(imp[0])
         r1 = np.real(imp[1])
-        i1 = np.imag(imp[1])
         expected[:n, n:] = np.array([
-            [0, 0,    0, 0],
+            [r0, 0,    0, 0],
             [0, r0, -i0, 0],
             [0, i0,  r0, 0],
             [0, 0,    0, r1],
         ])
         # 1,0
         imp = abcd[1, 0, :]
         r0 = np.real(imp[0])
         i0 = np.imag(imp[0])
         r1 = np.real(imp[1])
         expected[n:, :n] = np.array([
-            [0, 0,    0, 0],
+            [r0, 0,    0, 0],
             [0, r0, -i0, 0],
             [0, i0,  r0, 0],
             [0, 0,    0, r1],
         ])
         # 1,1
         imp = abcd[1, 1, :]
         r0 = np.real(imp[0])
         i0 = np.imag(imp[0])
         r1 = np.real(imp[1])
         expected[n:, n:] = np.array([
-            [0, 0,    0, 0],
+            [r0, 0,    0, 0],
             [0, r0, -i0, 0],
             [0, i0,  r0, 0],
             [0, 0,    0, r1],
         ])
         # test
         assert np.allclose(mimo, expected)
```

### Comparing `wecopttool-2.4.0/tests/test_waves.py` & `wecopttool-2.5.0/tests/test_waves.py`

 * *Files identical despite different names*

### Comparing `wecopttool-2.4.0/wecopttool/__init__.py` & `wecopttool-2.5.0/wecopttool/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 """
 WEC Design Optimization Toolbox (*WecOptTool*) developed by
 Sandia National Laboratories. See
-`snl-waterpower.github.io/WecOptTool/ <https://snl-waterpower.github.io/WecOptTool/>`_.
+`sandialabs.github.io/WecOptTool/ <https://sandialabs.github.io/WecOptTool/>`_.
 
 The top-level :python:`wecopttool` module contains:
 
 * The :python:`wecopttool.WEC` class, which is the main way to interact
   with *WecOptTool*.
 * Support functions for basic functionality, accessed as
   :python:`wecoptool.<function>`.
```

### Comparing `wecopttool-2.4.0/wecopttool/core.py` & `wecopttool-2.5.0/wecopttool/core.py`

 * *Files 1% similar despite different names*

```diff
@@ -17,14 +17,15 @@
 __all__ = [
     "WEC",
     "ncomponents",
     "frequency",
     "time",
     "time_mat",
     "derivative_mat",
+    "derivative2_mat",
     "mimo_transfer_mat",
     "vec_to_dofmat",
     "dofmat_to_vec",
     "real_to_complex",
     "complex_to_real",
     "fd_to_td",
     "td_to_fd",
@@ -204,14 +205,15 @@
             Initialize a :py:class:`wecopttool.WEC` object from an
             intrinsic impedance array and excitation coefficients.
         """
         self._freq = frequency(f1, nfreq)
         self._time = time(f1, nfreq)
         self._time_mat = time_mat(f1, nfreq)
         self._derivative_mat = derivative_mat(f1, nfreq)
+        self._derivative2_mat = derivative2_mat(f1, nfreq)
         self._forces = forces
         constraints = list(constraints) if (constraints is not None) else []
         self._constraints = constraints
 
         # inertia options
         self._inertia_in_forces = inertia_in_forces
 
@@ -616,15 +618,16 @@
         use_grad: Optional[bool] = True,
         maximize: Optional[bool] = False,
         bounds_wec: Optional[Bounds] = None,
         bounds_opt: Optional[Bounds] = None,
         callback: Optional[TStateFunction] = None,
         ) -> tuple[Dataset, Dataset, OptimizeResult]:
         """Simulate WEC dynamics using a pseudo-spectral solution
-        method.
+        method and returns the raw results dictionary produced by 
+        :py:func:`scipy.optimize.minimize`.
 
         Parameters
         ----------
         waves
             :py:class:`xarray.Dataset` with the structure and elements
             shown by :py:mod:`wecopttool.waves`.
         obj_fun
@@ -669,32 +672,38 @@
             See :py:func:`scipy.optimize.minimize`.
         callback
             Function called after each iteration, must have signature
             :python:`fun(wec, x_wec, x_opt, waves)`. The default
             provides status reports at each iteration via logging at the
             INFO level.
 
-        Returns
-        -------
-        res_fd
-            Dynamic responses in the frequency-domain.
-        res_td
-            Dynamic responses in the time-domain.
-        res
-            Results produced by :py:func:`scipy.optimize.minimize`.
-
         Raises
         ------
         ValueError
             If :python:`scale_x_opt` is a scalar and
             :python:`nstate_opt` is not provided.
         Exception
             If the optimizer fails for any reason other than maximum
             number of states, i.e. for exit modes other than 0 or 9.
             See :py:mod:`scipy.optimize` for exit mode details.
+            
+        Examples
+        --------
+        The :py:meth:`wecopttool.WEC.solve` method only returns the
+        raw results dictionary produced by :py:func:`scipy.optimize.minimize`.
+
+        >>> res_opt = wec.solve(waves=wave,
+                                obj_fun=pto.average_power,
+                                nstate_opt=2*nfreq+1)
+
+        To get the post-processed results for the
+        :py:class:`wecopttool.pto.PTO`, you may call
+
+        >>> res_wec_fd, res_wec_td = wec.post_process(wec,res_opt)
+        >>> res_pto_fd, res_pto_td = pto.post_process(wec,res_opt)
 
         See Also
         --------
         wecopttool.waves,
         """
 
         _log.info("Solving pseudo-spectral control problem.")
@@ -847,14 +856,29 @@
 
         Returns
         -------
         results_fd
             Dynamic responses in the frequency-domain.
         results_td
             Dynamic responses in the time-domain.
+            
+        Examples
+        --------
+        The :py:meth:`wecopttool.WEC.solve` method only returns the
+        raw results dictionary produced by :py:func:`scipy.optimize.minimize`.
+
+        >>> res_opt = wec.solve(waves=wave,
+                                obj_fun=pto.average_power,
+                                nstate_opt=2*nfreq+1)
+
+        To get the post-processed results for the
+        :py:class:`wecopttool.pto.PTO`, you may call
+
+        >>> res_wec_fd, res_wec_td = wec.post_process(wec,res_opt)
+        >>> res_pto_fd, res_pto_td = pto.post_process(wec,res_opt)
         """
         create_time = f"{datetime.utcnow()}"
 
         pos_attr = {'long_name': 'Position', 'units': 'm or rad'}
         vel_attr = {'long_name': 'Velocity', 'units': 'm/s or rad/s'}
         acc_attr = {'long_name': 'Acceleration', 'units': 'm/s^2 or rad/s^2'}
         omega_attr = {'long_name': 'Radial frequency', 'units': 'rad/s'}
@@ -870,15 +894,15 @@
         period_coord = ("omega", self.period, period_attr)
         dof_coord = ("influenced_dof", self.dof_names, dof_attr)
 
         # frequency domain
         force_da_list = []
         for name, force in self.forces.items():
             force_td_tmp = force(self, x_wec, x_opt, waves)
-            force_fd = self.td_to_fd(force_td_tmp, fft=True)
+            force_fd = self.td_to_fd(force_td_tmp)
             force_da = DataArray(data=force_fd,
                                  dims=["omega", "influenced_dof"],
                                  coords={
                                      'omega': omega_coord,
                                      'freq': freq_coord,
                                      'period': period_coord,
                                      'influenced_dof': dof_coord},
@@ -893,15 +917,15 @@
 
         pos = self.vec_to_dofmat(x_wec)
         pos_fd = real_to_complex(pos)
 
         vel = self.derivative_mat @ pos
         vel_fd = real_to_complex(vel)
 
-        acc = self.derivative_mat @ vel
+        acc = self.derivative2_mat @ pos
         acc_fd = real_to_complex(acc)
 
         fd_state = Dataset(
             data_vars={
                 'pos': (['omega', 'influenced_dof'], pos_fd, pos_attr),
                 'vel': (['omega', 'influenced_dof'], vel_fd, vel_attr),
                 'acc': (['omega', 'influenced_dof'], acc_fd, acc_attr)},
@@ -1042,14 +1066,27 @@
         :python:`(2*nfreq, ndof)`, the Fourier coefficients of the
         derivative of :python:`x` are obtained via
         :python:`derivative_mat @ x`.
         """
         return self._derivative_mat
 
     @property
+    def derivative2_mat(self) -> ndarray:
+        """Matrix to create Fourier coefficients of the second derivative of
+        some quantity.
+
+        For some array of Fourier coefficients :python:`x`
+        (excluding the sine component of the highest freequency), size
+        :python:`(2*nfreq, ndof)`, the Fourier coefficients of the
+        second derivative of :python:`x` are obtained via
+        :python:`derivative2_mat @ x`.
+        """
+        return self._derivative2_mat
+
+    @property
     def dt(self) -> float:
         """Time spacing [s]."""
         return self._time[1]
 
     @property
     def tf(self) -> float:
         """Final time (repeat period) [s]. Not included in
@@ -1399,14 +1436,50 @@
     blocks = [block(n+1) for n in range(nfreq)]
     if zero_freq:
         blocks = [0.0] + blocks
     deriv_mat = block_diag(*blocks)
     return deriv_mat[:-1, :-1] # remove 2pt wave sine component
 
 
+def derivative2_mat(
+    f1: float,
+    nfreq: int,
+    zero_freq: Optional[bool] = True,
+) -> ndarray:
+    """Assemble the second derivative matrix that converts the state vector of
+    a response to the state vector of its second derivative.
+
+    For a state :math:`x` consisting of the mean (DC) component
+    followed by the real and imaginary components of the Fourier
+    coefficients (excluding the imaginary component of the 2-point wave) as
+    :math:`x=[X0, Re(X1), Im(X1), ..., Re(Xn)]`,
+    the state of its second derivative is given as :math:`(DD)x`, where
+    :math:`DD` is the second derivative matrix.
+
+    The time matrix has size :python:`(nfreq*2, nfreq*2)`.
+
+    If :python:`zero_freq = False` (not default), the mean (DC) component
+    :python:`X0` is excluded, and the matrix/vector length is reduced by 1.
+
+    Parameters
+    ---------
+    f1
+        Fundamental frequency :python:`f1` [:math:`Hz`].
+    nfreq
+        Number of frequencies.
+    zero_freq
+        Whether the first frequency should be zero.
+    """
+    vals = [((n+1)*f1 * 2*np.pi)**2 for n in range(nfreq)]
+    diagonal = np.repeat(-np.ones(nfreq) * vals, 2)[:-1] # remove 2pt wave sine
+    if zero_freq:
+        diagonal = np.concatenate(([0.0], diagonal))
+    return np.diag(diagonal)
+
+
 def mimo_transfer_mat(
     transfer_mat: ArrayLike,
     zero_freq: Optional[bool] = True,
 ) -> ndarray:
     """Create a block matrix of the MIMO transfer function.
 
     The input is a complex transfer matrix that relates the complex
@@ -1706,14 +1779,15 @@
     """
     td= atleast_2d(td)
     n = td.shape[0]
     if fft:
         fd = np.fft.rfft(td*2, n=n, axis=0, norm='forward')
     else:
         fd = np.dot(dft(n, 'n')[:n//2+1, :], td*2)
+    fd = np.concatenate((fd[:1, :]/2, fd[1:-1, :], fd[-1:, :]/2))
     if not zero_freq:
         fd = fd[1:, :]
     return fd
 
 
 def read_netcdf(fpath: Union[str, Path]) -> Dataset:
     """Read a *NetCDF* file with possibly complex entries as a
```

### Comparing `wecopttool-2.4.0/wecopttool/geom.py` & `wecopttool-2.5.0/wecopttool/geom.py`

 * *Files identical despite different names*

### Comparing `wecopttool-2.4.0/wecopttool/hydrostatics.py` & `wecopttool-2.5.0/wecopttool/hydrostatics.py`

 * *Files identical despite different names*

### Comparing `wecopttool-2.4.0/wecopttool/pto.py` & `wecopttool-2.5.0/wecopttool/pto.py`

 * *Files 2% similar despite different names*

```diff
@@ -306,16 +306,15 @@
             shown by :py:mod:`wecopttool.waves`.
         nsubsteps
             Number of steps between the default (implied) time steps.
             A value of :python:`1` corresponds to the default step
             length.
         """
         pos_wec = wec.vec_to_dofmat(x_wec)
-        vel_wec = np.dot(wec.derivative_mat, pos_wec)
-        acc_wec = np.dot(wec.derivative_mat, vel_wec)
+        acc_wec = np.dot(wec.derivative2_mat, pos_wec)
         return self._fkinematics(acc_wec, wec, x_wec, x_opt, waves, nsubsteps)
 
     def force_on_wec(self,
         wec: TWEC,
         x_wec: ndarray,
         x_opt: ndarray,
         waves: Optional[Dataset] = None,
@@ -508,21 +507,14 @@
             A value of :python:`1` corresponds to the default step
             length.
         """
         q2_td, e2_td = self.power_variables(wec, x_wec,
                                             x_opt, waves, nsubsteps)
         # power
         power_out = q2_td * e2_td
-        if self.impedance is not None:
-            z_12 = self.impedance[:self.ndof, self.ndof:, 0] # Fi
-            z_22 = self.impedance[self.ndof:, self.ndof:, 0] # Vi
-            z_12_inv = np.linalg.inv(z_12.T).T
-            x_opt_0 = vec_to_dofmat(x_opt, self.ndof)[0:1, :]
-            transduced_flow = np.dot(np.real(z_12_inv), x_opt_0.T)
-            power_out = power_out + (np.dot(np.real(z_22), transduced_flow**2)).T
         if self.loss is not None:
             power_out = power_out + self.loss(q2_td, e2_td)
         return power_out
 
     def energy(self,
         wec: TWEC,
         x_wec: ndarray,
@@ -670,24 +662,24 @@
     ) -> tuple[Dataset, Dataset]:
         """Transform the results from optimization solution to a form
         that the user can work with directly.
 
         Examples
         --------
         The :py:meth:`wecopttool.WEC.solve` method only returns the
-        post-processed results for the :py:class:`wecopttool.WEC`
-        object.
+        raw results dictionary produced by :py:func:`scipy.optimize.minimize`.
 
-        >>> res_wec_fd, res_wec_td, res_opt = wec.solve(waves=wave,
-                                              obj_fun=pto.average_power,
-                                              nstate_opt=2*nfreq+1)
+        >>> res_opt = wec.solve(waves=wave,
+                                obj_fun=pto.average_power,
+                                nstate_opt=2*nfreq+1)
 
         To get the post-processed results for the
         :py:class:`wecopttool.pto.PTO`, you may call
 
+        >>> res_wec_fd, res_wec_td = wec.post_process(wec,res_opt)
         >>> res_pto_fd, res_pto_td = pto.post_process(wec,res_opt)
 
         For smoother plots, you can set :python:`nsubsteps` to a value
         greater than 1.
 
         >>> res_pto_fd, res_pto_td = pto.post_process(wec,res_opt,
                                                       nsubsteps=4)
@@ -838,15 +830,18 @@
     z_12_inv = np.linalg.inv(z_12.T).T
 
     mmult = lambda a,b: np.einsum('mnr,mnr->mnr', a, b)
     abcd_11 = -1 * mmult(z_12_inv, z_11)
     abcd_12 = z_12_inv
     abcd_21 = z_21 - mmult(z_22, mmult(z_12_inv, z_11))
     abcd_22 = mmult(z_22, z_12_inv)
-    return np.block([[[abcd_11], [abcd_12]], [[abcd_21], [abcd_22]]])
+
+    row_1 = np.hstack([abcd_11, abcd_12])
+    row_2 = np.hstack([abcd_21, abcd_22])
+    return np.vstack([row_1, row_2])
 
 
 def _make_mimo_transfer_mat(
     impedance_abcd: ndarray,
     ndof: int,
 ) -> np.ndarray:
     """Create a block matrix of a MIMO transfer function.
@@ -854,26 +849,33 @@
     Parameters
     ----------
     impedance
         PTO impedance in ABCD form.
     ndof
         Number of degrees of freedom.
     """
-    elem = [[None]*2*ndof for _ in range(2*ndof)]
     def block(re, im): return np.array([[re, -im], [im, re]])
     for idof in range(2*ndof):
         for jdof in range(2*ndof):
             Zp = impedance_abcd[idof, jdof, :]
             re = np.real(Zp)
             im = np.imag(Zp)
             # Exclude the sine component of the 2-point wave
             blocks = [block(ire, iim) for (ire, iim) in zip(re[:-1], im[:-1])]
-            blocks = [0.0] + blocks + [re[-1]]
-            elem[idof][jdof] = block_diag(*blocks)
-    return np.block(elem)
+            # re[0] added for the zero frequency power loss (DC), could be re[n]
+            blocks = [re[0]] + blocks + [re[-1]]
+            if jdof==0:
+                row = block_diag(*blocks)
+            else:
+                row = np.hstack([row, block_diag(*blocks)])
+        if idof==0:
+            mat = row
+        else:
+            mat = np.vstack([mat, row])
+    return mat
 
 
 # controllers
 def controller_unstructured(
     pto: TPTO,
     wec: TWEC,
     x_wec: ndarray,
@@ -898,16 +900,16 @@
         :py:class:`xarray.Dataset` with the structure and elements
         shown by :py:mod:`wecopttool.waves`.
     nsubsteps
         Number of steps between the default (implied) time steps.
         A value of :python:`1` corresponds to the default step
         length.
     """
-    x_opt = np.reshape(x_opt, (-1, pto.ndof), order='F')
     tmat = pto._tmat(wec, nsubsteps)
+    x_opt = np.reshape(x_opt[:len(tmat[0])*pto.ndof], (-1, pto.ndof), order='F')
     return np.dot(tmat, x_opt)
 
 
 def controller_pid(
     pto: TPTO,
     wec: TWEC,
     x_wec: ndarray,
```

### Comparing `wecopttool-2.4.0/wecopttool/waves.py` & `wecopttool-2.5.0/wecopttool/waves.py`

 * *Files 3% similar despite different names*

```diff
@@ -52,15 +52,16 @@
 
 def elevation_fd(
     f1: float,
     nfreq: int,
     directions: Union[float, ArrayLike],
     amplitudes: Optional[ArrayLike] = None,
     phases: Optional[ArrayLike] = None,
-    attr: Optional[Mapping] = None
+    attr: Optional[Mapping] = None,
+    seed: Optional[float] = None,
 ) -> DataArray:
     """Construct the complex wave elevation
     :py:class:`xarray.DataArray`.
 
     This is the complex wave elevation (m) indexed by radial frequency
     (rad/s) and wave direction (rad).
     The coordinate units and names match those from *Capytaine*.
@@ -77,14 +78,17 @@
     amplitudes:
         Wave elevation amplitude in meters.
     phases:
         Wave phases in degrees.
     attr:
         Additional attributes (metadata) to include in the
         :py:class:`xarray.DataArray`.
+    seed
+        Seed for random number generator. Used for reproducibility.
+        Generally should not be used except for testing.
     """
     directions = np.atleast_1d(degrees_to_radians(directions, sort=False))
     ndirections = len(directions)
     freq = frequency(f1, nfreq, False)
     omega = freq*2*np.pi
 
     dims = ('omega', 'wave_direction')
@@ -95,15 +99,15 @@
               'freq': (dims[0], freq, freq_attr),
               'wave_direction': (dims[1], directions, dir_attr)}
 
     if amplitudes is None:
         amplitudes = np.zeros([nfreq, ndirections])
 
     if phases is None:
-        phases = random_phase([nfreq, ndirections])
+        phases = random_phase([nfreq, ndirections],seed)
     else:
         phases = degrees_to_radians(phases, False)
 
     camplitude = amplitudes * np.exp(1j*phases)
 
     attr = {} if attr is None else attr
     attrs = {'units': 'm', 'long_name': 'Wave elevation'} | attr
@@ -177,14 +181,15 @@
 
     return waves
 
 
 def long_crested_wave(
     efth: DataArray,
     direction: Optional[float] = 0.0,
+    seed: Optional[float] = None,
 ) -> DataArray:
     """Create a complex frequency-domain wave elevation from an
     omnidirectional spectrum.
 
     The omnidirectional spectrum is in the
     :py:class:`wavespectra.SpecArray` format.
 
@@ -196,32 +201,35 @@
     Parameters
     ----------
     efth
         Omnidirection wave spectrum in units of m^2/Hz, in the format
         used by :py:class:`wavespectra.SpecArray`.
     direction
         Direction (in degrees) of the long-crested wave.
-
+    seed
+        Seed for random number generator. Used for reproducibility.
+        Generally should not be used except for testing.
     """
     f1, nfreq = frequency_parameters(efth.freq.values, False)
     df = f1
 
     values = efth.values
     values[values<0] = np.nan
     amplitudes = np.sqrt(2 * values * df)
 
     attr = {
         'Wave type': 'Long-crested irregular',
         'Direction (degrees)': direction,
     }
 
-    return elevation_fd(f1, nfreq, direction, amplitudes, None, attr)
+    return elevation_fd(f1, nfreq, direction, amplitudes, None, attr, seed)
 
 
-def irregular_wave(efth: DataArray) -> DataArray:
+def irregular_wave(efth: DataArray,
+                   seed: Optional[float] = None,) -> DataArray:
     """Create a complex frequency-domain wave elevation from a spectrum.
 
     The omnidirectional spectrum is in the
     :py:class:`wavespectra.SpecArray` format.
 
     .. note:: The frequencies must be evenly-spaced with spacing equal
               to the first frequency. This is not always the case when
@@ -231,27 +239,30 @@
     .. note:: The wave directions must also be evenly spaced.
 
     Parameters
     ----------
     efth
         Wave spectrum in units of m^2/Hz/deg, in the format used by
         :py:class:`wavespectra.SpecArray`.
+    seed
+        Seed for random number generator. Used for reproducibility.
+        Generally should not be used except for testing.
     """
     f1, nfreq = frequency_parameters(efth.freq.values, False)
     directions = efth.dir.values
     df = f1
     dd = np.sort(directions)[1]-np.sort(directions)[0]
 
     values = efth.values
     values[values<0] = np.nan
     amplitudes = np.sqrt(2 * values * df * dd)
 
     attr = {'Wave type': 'Irregular'}
 
-    return elevation_fd(f1, nfreq, directions, amplitudes, None, attr)
+    return elevation_fd(f1, nfreq, directions, amplitudes, None, attr, seed)
 
 
 def random_phase(
     shape: Optional[Union[Iterable[int], int]] = None,
     seed: Optional[float] = None,
 ) -> Union[float , ndarray]:
     """Generate random phases in range [-π, π) radians.
```

### Comparing `wecopttool-2.4.0/wecopttool.egg-info/PKG-INFO` & `wecopttool-2.5.0/wecopttool.egg-info/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,34 +1,34 @@
 Metadata-Version: 2.1
 Name: wecopttool
-Version: 2.4.0
+Version: 2.5.0
 Summary: WEC Design Optimization Toolbox
 Author: Sandia National Laboratories
 License: GNU General Public License v3 (GPLv3)
-Project-URL: Documentation, https://snl-waterpower.github.io/WecOptTool/
+Project-URL: Documentation, https://sandialabs.github.io/WecOptTool/
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 Provides-Extra: dev
 Provides-Extra: geometry
 License-File: LICENSE
 License-File: NOTICE
 
-[![Test-WecOptTool](https://github.com/SNL-WaterPower/WecOptTool/actions/workflows/push.yml/badge.svg)](https://github.com/SNL-WaterPower/WecOptTool/actions/workflows/push.yml)
-[![Coverage Status](https://coveralls.io/repos/github/SNL-WaterPower/WecOptTool/badge.svg?branch=main)](https://coveralls.io/github/SNL-WaterPower/WecOptTool?branch=main)
+[![Test-WecOptTool](https://github.com/sandialabs/WecOptTool/actions/workflows/push.yml/badge.svg)](https://github.com/sandialabs/WecOptTool/actions/workflows/push.yml)
+[![Coverage Status](https://coveralls.io/repos/github/sandialabs/WecOptTool/badge.svg?branch=main)](https://coveralls.io/github/sandialabs/WecOptTool?branch=main)
 
 # WecOptTool
 The Wave Energy Converter Design Optimization Toolbox (WecOptTool) allows users to perform wave energy converter (WEC) device design optimization studies with constrained optimal control.
 
 **NOTE:** If you are looking for the WecOptTool code used in previous published work (MATLAB version) please see [WecOptTool-MATLAB](https://github.com/SNL-WaterPower/WecOptTool-MATLAB).
 
 ## Project Information
-Refer to [WecOptTool documentation](https://snl-waterpower.github.io/WecOptTool/) for more information, including project overview, tutorials, theory, and API documentation.
+Refer to [WecOptTool documentation](https://sandialabs.github.io/WecOptTool/) for more information, including project overview, tutorials, theory, and API documentation.
 
 ## Getting started
 WecOptTool requires Python >= 3.8. Python 3.9 & 3.10 are supported.
 It is strongly recommended you create a dedicated virtual environment (e.g., using `conda`, `venv`, etc.) before installing `wecopttool`.
 
 **Option 1** - using `Conda`:
 
@@ -61,18 +61,18 @@
 
 ## Tutorials
 The tutorials can be found in the `examples` directory and are written as [Jupyter Notebooks](https://jupyter.org/).
 To run the tutorials, first download the notebook files and then, from the directory containing the notebooks, run `jupyter notebook`.
 Using `git` to obtain the notebooks this can be done by running
 
 ```bash
-git clone https://github.com/SNL-WaterPower/WecOptTool.git
+git clone https://github.com/sandialabs/WecOptTool.git
 cd WecOptTool/examples
 jupyter notebook
 ```
 
 ## Getting help
-To report bugs, use WecOptTool's [issues page](https://github.com/SNL-WaterPower/WecOptTool/issues).
-For general discussion, use WecOptTool's [discussion page](https://github.com/SNL-WaterPower/WecOptTool/discussions)
+To report bugs, use WecOptTool's [issues page](https://github.com/sandialabs/WecOptTool/issues).
+For general discussion, use WecOptTool's [discussion page](https://github.com/sandialabs/WecOptTool/discussions)
 
 ## Contributing
-If you are interested in contributing to WecOptTool, see our [contribution guidelines](https://github.com/SNL-WaterPower/WecOptTool/blob/main/.github/CONTRIBUTING.md).
+If you are interested in contributing to WecOptTool, see our [contribution guidelines](https://github.com/sandialabs/WecOptTool/blob/main/.github/CONTRIBUTING.md).
```

