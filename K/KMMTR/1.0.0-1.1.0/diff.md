# Comparing `tmp/KMMTR-1.0.0.tar.gz` & `tmp/KMMTR-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "KMMTR-1.0.0.tar", last modified: Tue May 16 11:24:16 2023, max compression
+gzip compressed data, was "KMMTR-1.1.0.tar", last modified: Sun May 21 00:09:29 2023, max compression
```

## Comparing `KMMTR-1.0.0.tar` & `KMMTR-1.1.0.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 jacob      (501) staff       (20)        0 2023-05-16 11:24:16.108692 KMMTR-1.0.0/
-drwxr-xr-x   0 jacob      (501) staff       (20)        0 2023-05-16 11:24:16.107832 KMMTR-1.0.0/KMMTR/
--rwxr-xr-x   0 jacob      (501) staff       (20)     6689 2023-05-16 11:23:50.000000 KMMTR-1.0.0/KMMTR/KMM.py
--rwxr-xr-x   0 jacob      (501) staff       (20)     6510 2023-05-16 11:11:43.000000 KMMTR-1.0.0/KMMTR/KMMTR.py
--rwxr-xr-x   0 jacob      (501) staff       (20)      386 2023-04-19 10:18:26.000000 KMMTR-1.0.0/KMMTR/__init__.py
-drwxr-xr-x   0 jacob      (501) staff       (20)        0 2023-05-16 11:24:16.108406 KMMTR-1.0.0/KMMTR.egg-info/
--rw-r--r--   0 jacob      (501) staff       (20)     1453 2023-05-16 11:24:16.000000 KMMTR-1.0.0/KMMTR.egg-info/PKG-INFO
--rw-r--r--   0 jacob      (501) staff       (20)      208 2023-05-16 11:24:16.000000 KMMTR-1.0.0/KMMTR.egg-info/SOURCES.txt
--rw-r--r--   0 jacob      (501) staff       (20)        1 2023-05-16 11:24:16.000000 KMMTR-1.0.0/KMMTR.egg-info/dependency_links.txt
--rw-r--r--   0 jacob      (501) staff       (20)       33 2023-05-16 11:24:16.000000 KMMTR-1.0.0/KMMTR.egg-info/requires.txt
--rw-r--r--   0 jacob      (501) staff       (20)        6 2023-05-16 11:24:16.000000 KMMTR-1.0.0/KMMTR.egg-info/top_level.txt
--rw-r--r--   0 jacob      (501) staff       (20)     1453 2023-05-16 11:24:16.108567 KMMTR-1.0.0/PKG-INFO
--rw-r--r--   0 jacob      (501) staff       (20)      859 2023-04-20 09:04:07.000000 KMMTR-1.0.0/README.md
--rw-r--r--   0 jacob      (501) staff       (20)       38 2023-05-16 11:24:16.108730 KMMTR-1.0.0/setup.cfg
--rw-r--r--   0 jacob      (501) staff       (20)     1381 2023-05-16 11:24:07.000000 KMMTR-1.0.0/setup.py
+drwxr-xr-x   0 jacob      (501) staff       (20)        0 2023-05-21 00:09:29.770659 KMMTR-1.1.0/
+drwxr-xr-x   0 jacob      (501) staff       (20)        0 2023-05-21 00:09:29.769792 KMMTR-1.1.0/KMMTR/
+-rwxr-xr-x   0 jacob      (501) staff       (20)     6822 2023-05-21 00:08:04.000000 KMMTR-1.1.0/KMMTR/KMM.py
+-rwxr-xr-x   0 jacob      (501) staff       (20)     6660 2023-05-21 00:08:25.000000 KMMTR-1.1.0/KMMTR/KMMTR.py
+-rwxr-xr-x   0 jacob      (501) staff       (20)      386 2023-04-19 10:18:26.000000 KMMTR-1.1.0/KMMTR/__init__.py
+drwxr-xr-x   0 jacob      (501) staff       (20)        0 2023-05-21 00:09:29.770366 KMMTR-1.1.0/KMMTR.egg-info/
+-rw-r--r--   0 jacob      (501) staff       (20)     1453 2023-05-21 00:09:29.000000 KMMTR-1.1.0/KMMTR.egg-info/PKG-INFO
+-rw-r--r--   0 jacob      (501) staff       (20)      208 2023-05-21 00:09:29.000000 KMMTR-1.1.0/KMMTR.egg-info/SOURCES.txt
+-rw-r--r--   0 jacob      (501) staff       (20)        1 2023-05-21 00:09:29.000000 KMMTR-1.1.0/KMMTR.egg-info/dependency_links.txt
+-rw-r--r--   0 jacob      (501) staff       (20)       33 2023-05-21 00:09:29.000000 KMMTR-1.1.0/KMMTR.egg-info/requires.txt
+-rw-r--r--   0 jacob      (501) staff       (20)        6 2023-05-21 00:09:29.000000 KMMTR-1.1.0/KMMTR.egg-info/top_level.txt
+-rw-r--r--   0 jacob      (501) staff       (20)     1453 2023-05-21 00:09:29.770532 KMMTR-1.1.0/PKG-INFO
+-rw-r--r--   0 jacob      (501) staff       (20)      859 2023-04-20 09:04:07.000000 KMMTR-1.1.0/README.md
+-rw-r--r--   0 jacob      (501) staff       (20)       38 2023-05-21 00:09:29.770698 KMMTR-1.1.0/setup.cfg
+-rw-r--r--   0 jacob      (501) staff       (20)     1381 2023-05-21 00:08:51.000000 KMMTR-1.1.0/setup.py
```

### Comparing `KMMTR-1.0.0/KMMTR/KMM.py` & `KMMTR-1.1.0/KMMTR/KMM.py`

 * *Files 3% similar despite different names*

```diff
@@ -2,15 +2,14 @@
 import copy
 import warnings
 from cvxopt import solvers, matrix 
 from sklearn.gaussian_process import GaussianProcessRegressor as GPR
 from sklearn.gaussian_process.kernels import DotProduct, WhiteKernel, RBF, Matern 
 
 
-
 class KernelMeanMatching():
     def __init__(self,kernel,source_data,target_data,target_response):
         """
         Constructor for KernelMeanMatching class.
         
         Args:
             kernel (str): Name of the kernel function to use.
@@ -85,20 +84,22 @@
         para = np.exp(GPr_fit.kernel_.theta)
         print('Trained length scale :', para)
 
         Inst_kernel = self.call_kernel(para)
         return Inst_kernel
 
 
-    def cal_beta(self, B,tao = None):
+    def cal_beta(self, B, S_expt,tao = None):
         """
         Helper function to calculate the beta values that balance the source and target data distributions.
         
         Args:
             B (float): Bound on the beta values. Defaults to 1.
+            S_expt (float): the expected weights of source domain data
+            tao (float): the tolerance of weights 
         
         Returns:
             A numpy array containing the calculated beta values.
         """
         
         n = len(self.source_data)
         m = len(self.target_data)
@@ -158,15 +159,15 @@
         M_G1_U = copy.deepcopy(matrix(M_G1))
         M_G2_U = copy.deepcopy(matrix(M_G2))
         M_A1 = matrix(M_A1)
         M_A2 = matrix(M_A2)
         V_h1_U = copy.deepcopy(matrix(V_h1))
         V_h2_U = copy.deepcopy(matrix(V_h2))
         M_G = matrix(np.r_[M_G1_U, M_G2_U,M_A1,M_A2])
-        h1 = matrix(0.99+tao)
-        h2 = matrix(tao-0.99)
+        h1 = matrix(S_expt+tao)
+        h2 = matrix(tao-S_expt)
         h = matrix(np.r_[V_h1_U, V_h2_U,h1,h2])
 
         solvers.options['show_progress'] = True
         sol = solvers.qp(M_P,V_q,M_G,h)
         beta = sol['x']
         return np.array(beta)
```

### Comparing `KMMTR-1.0.0/KMMTR/KMMTR.py` & `KMMTR-1.1.0/KMMTR/KMMTR.py`

 * *Files 2% similar despite different names*

```diff
@@ -32,38 +32,41 @@
 
     Methods
     -------
     fit(source_dataset,target_dataset,test_data)
         Fit the transfer learning regression model to the source dataset and target dataset, and predict the target variable
         on the test dataset.
     """
-    def __init__(self, Regressor='RF',UpBound=2,kernel = 'RBF', Targets = 1):
+    def __init__(self, Regressor='RF',UpBound=1,kernel = 'RBF', S_expt=.5,Targets = 1):
         """
         Initialize KMMTransferReg model.
 
         Parameters
         ----------
         Regressor : str or object, default='RF'
             A regression model used to fit the mapped data. If a string is passed, it should be one of {'RF', 'LR'}
             representing RandomForestRegressor and LinearRegression, respectively. Otherwise, an object with fit and
             predict methods that implements a regression algorithm can be passed.
         UpBound : float, default=1
             The upper bound for beta coefficients. 
         kernel : str, default='RBF'
             The kernel to use for KMM. Can be 'RBF', 'DotProduct', 'WhiteKernel', 'Matern'.
+        S_expt : float, default=0.5 
+            the expected weights of source domain data
         Targets : int, default=1
             The number of target variables in the dataset.
         """
         # A sklearn regression model 
         if type(Regressor) == str:
             self.Regressor = GenerateReg(Regressor)
         else:
             self.Regressor = Regressor
         self.UpBound = UpBound
         self.kernel = kernel
+        self.S_expt = S_expt
         self.Targets = Targets
         warnings.filterwarnings('ignore')
 
 
     def fit(self,source_dataset,target_dataset,test_data,tao=None):
         """
         Fit the transfer model on source and target datasets and return the predictions
@@ -92,15 +95,15 @@
         """
         source_data = np.array(source_dataset)[:, :-self.Targets]
         source_response = np.array(source_dataset)[:, -self.Targets:]
         target_data = np.array(target_dataset)[:, :-self.Targets]
         target_response = np.array(target_dataset)[:, -self.Targets:]
 
         KMM = KernelMeanMatching(self.kernel,source_data,target_data,target_response)
-        beta = KMM.cal_beta(B = self.UpBound,tao=tao)
+        beta = KMM.cal_beta(B = self.UpBound,S_expt=self.S_expt,tao=tao)
 
         X = np.concatenate((source_data, target_data), axis=0)
         Y = np.concatenate((source_response, target_response), axis=0)
 
         # test the Regressor
         attribute_list = ['fit', 'predict',]
         check_attributes(self.Regressor, attribute_list)
```

### Comparing `KMMTR-1.0.0/KMMTR.egg-info/PKG-INFO` & `KMMTR-1.1.0/KMMTR.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: KMMTR
-Version: 1.0.0
+Version: 1.1.0
 Summary: a transfer learning regression model based on Kernel Mean Matching (KMM) algorithm
 Home-page: https://github.com/Bin-Cao/KMMTransferRegressor
 Author: CaoBin
 Author-email: bcao@shu.edu.com
 Maintainer: CaoBin
 Maintainer-email: binjacobcao@gmail.com
 License: MIT License
```

### Comparing `KMMTR-1.0.0/PKG-INFO` & `KMMTR-1.1.0/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: KMMTR
-Version: 1.0.0
+Version: 1.1.0
 Summary: a transfer learning regression model based on Kernel Mean Matching (KMM) algorithm
 Home-page: https://github.com/Bin-Cao/KMMTransferRegressor
 Author: CaoBin
 Author-email: bcao@shu.edu.com
 Maintainer: CaoBin
 Maintainer-email: binjacobcao@gmail.com
 License: MIT License
```

### Comparing `KMMTR-1.0.0/README.md` & `KMMTR-1.1.0/README.md`

 * *Files identical despite different names*

### Comparing `KMMTR-1.0.0/setup.py` & `KMMTR-1.1.0/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from setuptools import setup, find_packages
 setup(
     name='KMMTR',  # 包名
-    version='1.0.0',  # 版本
+    version='1.1.0',  # 版本
     description="a transfer learning regression model based on Kernel Mean Matching (KMM) algorithm",  # 包简介
     long_description=open('README.md',encoding='utf-8').read(),  # 读取文件中介绍包的详细内容
     include_package_data=True,  # 是否允许上传资源文件
     author='CaoBin',  # 作者
     author_email='bcao@shu.edu.com',  # 作者邮件
     maintainer='CaoBin',  # 维护者
     maintainer_email='binjacobcao@gmail.com',  # 维护者邮件
```

