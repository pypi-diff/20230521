# Comparing `tmp/pyfixest-0.5.2.tar.gz` & `tmp/pyfixest-0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyfixest-0.5.2.tar", max compression
+gzip compressed data, was "pyfixest-0.6.tar", max compression
```

## Comparing `pyfixest-0.5.2.tar` & `pyfixest-0.6.tar`

### file list

```diff
@@ -1,10 +1,10 @@
--rw-r--r--   0        0        0     1096 2022-11-19 12:53:04.921992 pyfixest-0.5.2/LICENSE.md
--rw-r--r--   0        0        0       26 2023-03-16 21:51:51.234748 pyfixest-0.5.2/pyfixest/__init__.py
--rw-r--r--   0        0        0    18071 2023-05-14 09:06:59.564643 pyfixest-0.5.2/pyfixest/feols.py
--rw-r--r--   0        0        0    39786 2023-05-14 09:06:59.566819 pyfixest-0.5.2/pyfixest/fixest.py
--rw-r--r--   0        0        0    17794 2023-05-13 20:24:52.625359 pyfixest-0.5.2/pyfixest/FormulaParser.py
--rw-r--r--   0        0        0     3426 2023-04-27 19:03:35.062476 pyfixest-0.5.2/pyfixest/ssc_utils.py
--rw-r--r--   0        0        0     1172 2023-05-13 20:24:52.632640 pyfixest-0.5.2/pyfixest/utils.py
--rw-r--r--   0        0        0      863 2023-05-14 09:13:14.061103 pyfixest-0.5.2/pyproject.toml
--rw-r--r--   0        0        0     2684 2023-05-13 20:24:52.634902 pyfixest-0.5.2/readme.md
--rw-r--r--   0        0        0     3535 1970-01-01 00:00:00.000000 pyfixest-0.5.2/PKG-INFO
+-rw-r--r--   0        0        0     1096 2022-11-19 12:53:04.921992 pyfixest-0.6/LICENSE.md
+-rw-r--r--   0        0        0       26 2023-03-16 21:51:51.234748 pyfixest-0.6/pyfixest/__init__.py
+-rw-r--r--   0        0        0    20564 2023-05-21 16:38:34.330335 pyfixest-0.6/pyfixest/feols.py
+-rw-r--r--   0        0        0    44096 2023-05-21 16:38:34.332330 pyfixest-0.6/pyfixest/fixest.py
+-rw-r--r--   0        0        0    19550 2023-05-21 16:38:34.319816 pyfixest-0.6/pyfixest/FormulaParser.py
+-rw-r--r--   0        0        0     3426 2023-04-27 19:03:35.062476 pyfixest-0.6/pyfixest/ssc_utils.py
+-rw-r--r--   0        0        0     1312 2023-05-21 16:38:34.333327 pyfixest-0.6/pyfixest/utils.py
+-rw-r--r--   0        0        0      894 2023-05-21 16:38:34.334501 pyfixest-0.6/pyproject.toml
+-rw-r--r--   0        0        0     2684 2023-05-21 16:38:31.130088 pyfixest-0.6/readme.md
+-rw-r--r--   0        0        0     3566 1970-01-01 00:00:00.000000 pyfixest-0.6/PKG-INFO
```

### Comparing `pyfixest-0.5.2/LICENSE.md` & `pyfixest-0.6/LICENSE.md`

 * *Files identical despite different names*

### Comparing `pyfixest-0.5.2/pyfixest/feols.py` & `pyfixest-0.6/pyfixest/feols.py`

 * *Files 14% similar despite different names*

```diff
@@ -50,41 +50,56 @@
     AssertionError
         If the vcov argument is not a dict, a string, or a list.
 
     """
 
     def __init__(self, Y: np.ndarray, X: np.ndarray, Z: np.ndarray) -> None:
 
-        if not isinstance(Y, (np.ndarray)):
-            raise TypeError("Y must be a numpy array.")
-        if not isinstance(X, (np.ndarray)):
-            raise TypeError("X must be a numpy array.")
+
+        _feols_input_checks(Y, X, Z)
 
         self.Y = Y
         self.X = X
         self.Z = Z
 
-        if self.X.ndim != 2:
-            raise ValueError("X must be a 2D array")
-        if self.Z.ndim != 2:
-            raise ValueError("Z must be a 2D array")
-
         self.N, self.k = X.shape
 
-    def get_fit(self) -> None:
+    def get_fit(self, estimator = "ols") -> None:
         '''
         Regression estimation for a single model, via ordinary least squares (OLS).
+        Args: estimator (str): Estimator to use. Can be one of "ols", "iv", or "2sls".
+                If "ols", then the estimator is (X'X)^{-1}X'Y.
+                If "iv", then the estimator is (Z'X)^{-1}Z'Y.
+                If "2sls", then the estimator is (X'Z(Z'Z)^{-1}Z'X)^{-1}X'Z(Z'Z)^{-1}Z'Y.
+        Returns:
+            None
+
         '''
 
-        self.tZX = np.transpose(self.Z) @ self.X
-        self.tZXinv = np.linalg.inv(self.tZX)
+        assert estimator in ["ols", "iv", "2sls"], "estimator must be one of 'ols', 'iv', or '2sls'."
 
+        self.tZX = np.transpose(self.Z) @ self.X
         self.tZy = (np.transpose(self.Z) @ self.Y)
-        beta_hat = self.tZXinv @ self.tZy
-        self.beta_hat = beta_hat.flatten()
+
+        if estimator in ["ols", "iv"]:
+
+            self.tZXinv = np.linalg.inv(self.tZX)
+            self.beta_hat = (self.tZXinv @ self.tZy).flatten()
+
+            if estimator == "iv":
+
+                self.tZZinv = np.linalg.inv(np.transpose(self.Z) @ self.Z)
+
+
+        else:
+
+            self.tXZ = np.transpose(self.X) @ self.Z
+            self.tZZinv = np.linalg.inv(np.transpose(self.Z) @ self.Z)
+            self.beta_hat = (np.linalg.inv(self.tXZ @ self.tZZinv @ self.tZX) @ self.tXZ @ self.tZZinv @ self.tZy).flatten()
+
         self.Y_hat = (self.X @ self.beta_hat)
         self.u_hat = (self.Y.flatten() - self.Y_hat)
 
     def get_vcov(self, vcov: Union[str, Dict[str, str], List[str]]) -> None:
         '''
         Compute covariance matrices for an estimated regression model.
 
@@ -119,48 +134,17 @@
 
         Returns
         -------
         None
 
         '''
 
-        assert isinstance(vcov, (dict, str, list)), "vcov must be a dict, string or list"
-        if isinstance(vcov, dict):
-            assert list(vcov.keys())[0] in ["CRV1", "CRV3"], "vcov dict key must be CRV1 or CRV3"
-            assert isinstance(list(vcov.values())[0], str), "vcov dict value must be a string"
-            assert list(vcov.values())[0] in self.data.columns, "vcov dict value must be a column in the data"
-        if isinstance(vcov, list):
-            assert all(isinstance(v, str) for v in vcov), "vcov list must contain strings"
-            assert all(v in self.data.columns for v in vcov), "vcov list must contain columns in the data"
-        if isinstance(vcov, str):
-            assert vcov in ["iid", "hetero", "HC1", "HC2", "HC3"], "vcov string must be iid, hetero, HC1, HC2, or HC3"
-
-        if isinstance(vcov, dict):
-            vcov_type_detail = list(vcov.keys())[0]
-            self.clustervar = list(vcov.values())[0]
-        elif isinstance(vcov, list):
-            vcov_type_detail = vcov
-        elif isinstance(vcov, str):
-            vcov_type_detail = vcov
-        else:
-            assert False, "arg vcov needs to be a dict, string or list"
-
-        if vcov_type_detail == "iid":
-            self.vcov_type = "iid"
-            self.is_clustered = False
-        elif vcov_type_detail in ["hetero", "HC1", "HC2", "HC3"]:
-            self.vcov_type = "hetero"
-            self.is_clustered = False
-            if vcov_type_detail in ["HC2", "HC3"]:
-                if self.has_fixef:
-                    raise ValueError("HC2 and HC3 inference types are not supported for regressions with fixed effects.")
-        elif vcov_type_detail in ["CRV1", "CRV3"]:
-            self.vcov_type = "CRV"
-            self.is_clustered = True
+        _check_vcov_input(vcov, self.data)
 
+        self.vcov_type, self.vcov_type_detail, self.is_clustered, self.clustervar = _deparse_vcov_input(vcov, self.has_fixef)
 
         if self.is_iv:
             if self.vcov_type in ["CRV3"]:
                 raise ValueError("CRV3 inference is not supported for IV regressions.")
 
         # compute vcov
         if self.vcov_type == 'iid':
@@ -175,50 +159,45 @@
             )
 
             # only relevant factor for iid in ssc: fixef.K
             if self.is_iv == False:
                 self.vcov =  self.ssc * self.tZXinv * (np.sum(self.u_hat ** 2) / (self.N - 1))
             else:
                 sigma2 = (np.sum(self.u_hat ** 2) / (self.N - 1))
-                tZZinv = np.linalg.inv(np.transpose(self.Z) @ self.Z) # k x k
-                tXZ = np.transpose(self.X) @ self.Z
-                self.vcov = self.ssc * np.linalg.inv(tXZ @ tZZinv @ self.tZX ) * sigma2 #
+                self.vcov = self.ssc * np.linalg.inv(self.tXZ @ self.tZZinv @ self.tZX ) * sigma2
 
         elif self.vcov_type == 'hetero':
 
             self.ssc = get_ssc(
                 ssc_dict = self.ssc_dict,
                 N = self.N,
                 k = self.k,
                 G = 1,
                 vcov_sign = 1,
                 vcov_type = "hetero"
             )
 
-            if vcov_type_detail in ["hetero", "HC1"]:
+            if self.vcov_type_detail in ["hetero", "HC1"]:
                 u = self.u_hat
-            elif vcov_type_detail in ["HC2", "HC3"]:
+            elif self.vcov_type_detail in ["HC2", "HC3"]:
                 leverage = np.sum(self.X * (self.X @ self.tZXinv), axis=1)
-                if vcov_type_detail == "HC2":
+                if self.vcov_type_detail == "HC2":
                     u = self.u_hat / np.sqrt(1 - leverage)
                 else:
                     u = self.u_hat / (1-leverage)
 
             if self.is_iv == False:
                 meat = np.transpose(self.Z) * (u ** 2) @ self.Z
-                # set off diagonal elements to zero
                 self.vcov =  self.ssc * self.tZXinv @ meat @  self.tZXinv
             else:
-                tZZinv = np.linalg.inv(np.transpose(self.Z) @ self.Z)  # k x k
-                tXZ = np.transpose(self.X) @ self.Z # k x k
                 if u.ndim == 1:
                     u = u.reshape((self.N,1))
                 Omega = np.transpose(self.Z) @ (self.Z * (u ** 2))  # k x k
-                meat = tXZ @ tZZinv  @ Omega  @ tZZinv @ self.tZX # k x k
-                bread = np.linalg.inv(tXZ @ tZZinv @ self.tZX)
+                meat = self.tXZ @ self.tZZinv  @ Omega  @ self.tZZinv @ self.tZX # k x k
+                bread = np.linalg.inv(self.tXZ @ self.tZZinv @ self.tZX)
                 self.vcov = self.ssc * bread @ meat @ bread
 
 
 
         elif self.vcov_type == "CRV":
 
             cluster_df = self.data[self.clustervar]
@@ -226,51 +205,48 @@
 
             if cluster_df.dtype != "category":
                 cluster_df = pd.Categorical(cluster_df)
 
             if cluster_df.isna().any():
                 raise ValueError("CRV inference not supported with missing values in the cluster variable. Please drop missing values before running the regression.")
 
-            cluster_mat, clustid = pd.factorize(cluster_df)
-            #cluster_mat = cluster_df.to_numpy()
+            _, clustid = pd.factorize(cluster_df)
 
-            #clustid = np.unique(cluster_mat)
             self.G = len(clustid)
 
             self.ssc = get_ssc(
                 ssc_dict = self.ssc_dict,
                 N = self.N,
                 k = self.k,
                 G = self.G,
                 vcov_sign = 1,
                 vcov_type = "CRV"
             )
 
-            if vcov_type_detail == "CRV1":
+            if self.vcov_type_detail == "CRV1":
 
 
-                meat = np.zeros((self.k, self.k))
+                k_instruments = self.Z.shape[1]
+                meat = np.zeros((k_instruments, k_instruments))
 
                 for _, g, in enumerate(clustid):
 
                     Zg = self.Z[np.where(cluster_df == g)]
                     ug = self.u_hat[np.where(cluster_df == g)]
-                    score_g = (np.transpose(Zg) @ ug).reshape((self.k, 1))
+                    score_g = (np.transpose(Zg) @ ug).reshape((k_instruments, 1))
                     meat += np.dot(score_g, score_g.transpose())
 
                 if self.is_iv == False:
                     self.vcov = self.ssc * self.tZXinv @ meat @ self.tZXinv
                 else:
-                    tZZinv = np.linalg.inv(np.transpose(self.Z) @ self.Z)  # k x k
-                    tXZ = np.transpose(self.X) @ self.Z # k x k
-                    meat = tXZ @ tZZinv @ meat @ tZZinv @ self.tZX
-                    bread = np.linalg.inv(tXZ @ tZZinv @ self.tZX)
+                    meat = self.tXZ @ self.tZZinv @ meat @ self.tZZinv @ self.tZX
+                    bread = np.linalg.inv(self.tXZ @ self.tZZinv @ self.tZX)
                     self.vcov = self.ssc * bread @ meat @ bread
 
-            elif vcov_type_detail == "CRV3":
+            elif self.vcov_type_detail == "CRV3":
 
                 # check: is fixed effect cluster fixed effect?
                 # if not, either error or turn fixefs into dummies
                 # for now: don't allow for use with fixed effects
 
                 #if self.has_fixef:
                 #    raise ValueError("CRV3 inference is currently not supported with fixed effects.")
@@ -353,35 +329,54 @@
             np.sqrt(np.diagonal(self.vcov))
         )
 
         self.tstat = (
             self.beta_hat / self.se
         )
 
-        #if self.vcov_type in ['iid', 'CRV']:
-            # t(G-1) distribution for clustered errors
         if self.vcov_type in ["iid", "hetero"]:
             df = self.N - self.k
         else:
             df = self.G - 1
         self.pvalue = (
             2*(1-t.cdf(np.abs(self.tstat), df))
         )
-        #else:
-        #    # normal distribution for non-clustered errors
-        #    self.pvalue = (
-        #            2*(1-norm.cdf(np.abs(self.tstat)))
-        #    )
 
         z = norm.ppf(1 - (alpha / 2))
         self.conf_int = (
             np.array([z * self.se - self.beta_hat, z * self.se + self.beta_hat])
         )
 
 
+    def get_Ftest(self, vcov, is_iv = False):
+
+        '''
+        compute an F-test statistic of the form H0: R*beta = q
+        Args: is_iv (bool): If True, the F-test is computed for the first stage regression of an IV model. Default is False.
+        Returns: None
+        '''
+
+        R = np.ones(self.k).reshape((1, self.k))
+        q = 0
+        beta = self.beta_hat
+        Rbetaq = R @ beta - q
+        #Rbetaq = self.beta_hat
+
+        if self.is_iv:
+            first_stage = Feols(self.Y, self.Z, self.Z)
+            first_stage.get_fit()
+            first_stage.get_vcov(vcov = vcov)
+            vcov = first_stage.vcov
+        else:
+            vcov = self.vcov
+
+
+        self.F_stat = Rbetaq @ np.linalg.inv(R @ self.vcov @ np.transpose(R)) @ Rbetaq
+
+
     def get_wildboottest(self, B:int, cluster : Union[np.ndarray, pd.Series, pd.DataFrame, None], param : Union[str, None], weights_type: str, impose_null: bool , bootstrap_type: str, seed: Union[str, None] , adj: bool , cluster_adj: bool):
 
         '''
         Run a wild cluster bootstrap based on an object of type "Feols"
 
         Args:
 
@@ -473,7 +468,104 @@
         '''
         Compute multiple additional measures commonly reported with linear regression output.
         '''
 
         self.r_squared = 1 - np.sum(self.u_hat ** 2) / \
             np.sum((self.Y - np.mean(self.Y))**2)
         self.adj_r_squared = (self.N - 1) / (self.N - self.k) * self.r_squared
+
+
+
+def _check_vcov_input(vcov, data):
+
+    '''
+    Check the input for the vcov argument in the Feols class.
+    Args:
+        vcov (dict, str, list): The vcov argument passed to the Feols class.
+        data (pd.DataFrame): The data passed to the Feols class.
+    Returns:
+        None
+    '''
+
+    assert isinstance(vcov, (dict, str, list)), "vcov must be a dict, string or list"
+    if isinstance(vcov, dict):
+        assert list(vcov.keys())[0] in ["CRV1", "CRV3"], "vcov dict key must be CRV1 or CRV3"
+        assert isinstance(list(vcov.values())[0], str), "vcov dict value must be a string"
+        assert list(vcov.values())[0] in data.columns, "vcov dict value must be a column in the data"
+    if isinstance(vcov, list):
+        assert all(isinstance(v, str) for v in vcov), "vcov list must contain strings"
+        assert all(v in data.columns for v in vcov), "vcov list must contain columns in the data"
+    if isinstance(vcov, str):
+        assert vcov in ["iid", "hetero", "HC1", "HC2", "HC3"], "vcov string must be iid, hetero, HC1, HC2, or HC3"
+
+
+def _deparse_vcov_input(vcov, has_fixef):
+
+    '''
+    Deparse the vcov argument passed to the Feols class.
+
+    Args:
+        vcov (dict, str, list): The vcov argument passed to the Feols class.
+        has_fixef (bool): Whether the regression has fixed effects.
+    Returns:
+        vcov_type (str): The type of vcov to be used. Either "iid", "hetero", or "CRV"
+        vcov_type_detail (str, list): The type of vcov to be used, with more detail. Either "iid", "hetero", "HC1", "HC2", "HC3", "CRV1", or "CRV3"
+        is_clustered (bool): Whether the vcov is clustered.
+        clustervar (str): The name of the cluster variable.
+    '''
+
+    if isinstance(vcov, dict):
+        vcov_type_detail = list(vcov.keys())[0]
+        clustervar = list(vcov.values())[0]
+    elif isinstance(vcov, list):
+        vcov_type_detail = vcov
+    elif isinstance(vcov, str):
+        vcov_type_detail = vcov
+    else:
+        assert False, "arg vcov needs to be a dict, string or list"
+
+    if vcov_type_detail == "iid":
+        vcov_type = "iid"
+        is_clustered = False
+    elif vcov_type_detail in ["hetero", "HC1", "HC2", "HC3"]:
+        vcov_type = "hetero"
+        is_clustered = False
+        if vcov_type_detail in ["HC2", "HC3"]:
+            if has_fixef:
+                raise ValueError("HC2 and HC3 inference types are not supported for regressions with fixed effects.")
+    elif vcov_type_detail in ["CRV1", "CRV3"]:
+        vcov_type = "CRV"
+        is_clustered = True
+
+    if is_clustered:
+        clustervar = list(vcov.values())[0]
+    else:
+        clustervar = None
+
+    return vcov_type, vcov_type_detail, is_clustered, clustervar
+
+
+def _feols_input_checks(Y, X, Z):
+
+    '''
+    Some basic checks on the input matrices Y, X, and Z.
+    Args:
+        Y (np.ndarray): FEOLS input matrix Y
+        X (np.ndarray): FEOLS input matrix X
+        Z (np.ndarray): FEOLS input matrix Z
+    Returns:
+        None
+    '''
+
+    if not isinstance(Y, (np.ndarray)):
+        raise TypeError("Y must be a numpy array.")
+    if not isinstance(X, (np.ndarray)):
+        raise TypeError("X must be a numpy array.")
+    if not isinstance(Z, (np.ndarray)):
+        raise TypeError("Z must be a numpy array.")
+
+    if X.ndim != 2:
+        raise ValueError("X must be a 2D array")
+    if Z.ndim != 2:
+        raise ValueError("Z must be a 2D array")
+
+
```

### Comparing `pyfixest-0.5.2/pyfixest/fixest.py` & `pyfixest-0.6/pyfixest/fixest.py`

 * *Files 5% similar despite different names*

```diff
@@ -99,25 +99,25 @@
                 covar2 = covar
                 depvar2 = depvar
 
                 fml = depvar2 + " ~ " + covar2
 
                 if self.is_iv:
                     instruments2 = dict2fe_iv.get(depvar)[0]
-                    endogvar = list(set(covar2.split("+")) - set(instruments2.split("+")))[0]
-                    instrument = list(set(instruments2.split("+")) - set(covar2.split("+")))[0]
+                    endogvar_list = list(set(covar2.split("+")) - set(instruments2.split("+")))#[0]
+                    instrument_list = list(set(instruments2.split("+")) - set(covar2.split("+")))#[0]
 
-                    if len([instrument]) > 1 or len([endogvar]) > 1:
-                        raise ValueError("Currently, IV estimation is only supported with one endogeneous variable and one instrument.")
+                    #if len(instrument_list) > 1 or len(endogvar_list) > 1:
+                    #    raise ValueError("Currently, IV estimation is only supported with one endogeneous variable and one instrument.")
 
-                    fml2 = instrument + "+" + fml
+                    fml2 = "+".join(instrument_list) + "+" + fml
                     rhs, lhs = model_matrix(fml2, data)
 
                     Y = rhs[[depvar]]
-                    I = rhs[[instrument]]
+                    I = rhs[instrument_list]
                     X = lhs
                 else:
                     Y, X = model_matrix(fml, data)
 
                 na_index = list(set(data.index) - set(Y.index))
 
                 if self.ivars is not None:
@@ -128,16 +128,16 @@
                 x_names = list(X.columns)
                 yxz_names = list(y_names) + list(x_names)
                 if self.is_iv:
                     iv_names = list(I.columns)
                     #z_varnames = list(set(x_names) - set([endogvar]))
                     #z_varnames.append(instrument)
                     x_names_copy = x_names.copy()
-                    x_names_copy.remove(endogvar)
-                    z_names = x_names_copy + [instrument]
+                    x_names_copy = [x for x in x_names_copy if x not in endogvar_list]
+                    z_names = x_names_copy + instrument_list
                     cols = yxz_names + iv_names
                 else:
                     iv_names = None
                     z_names = None
                     cols = yxz_names
 
                 if self.ivars is not None:
@@ -150,16 +150,16 @@
                 Y = Y.to_numpy()
                 #if Y.ndim != 1:
                 #    Y = Y.reshape((len(Y), 1))
                 #.reshape((len(Y), 1))
                 X = X.to_numpy()
                 if self.is_iv:
                     I = I.to_numpy()
-                    if I.ndim != 1:
-                        I = I.reshape((len(I), 1))
+                    #if I.ndim != 1:
+                    #    I = I.reshape((len(I), 1))
 
                 if Y.shape[1] > 1:
                     raise ValueError(
                         "Dependent variable must be a single column. Please make sure that the dependent variable" + depvar2 + "is of a numeric type (int or float).")
 
                 # variant 1: if there are fixed effects to be projected out
                 if fe is not None:
@@ -356,45 +356,20 @@
             self.var_dict_iv = self.var_dict
             self.fml_dict2_iv = self.fml_dict2
 
         self.ivars = fxst_fml.ivars
 
 
         self.ssc_dict = ssc
-        if fixef_rm == "singleton":
-            self.drop_singletons = True
-        else:
-            self.drop_singletons = False
+        self.drop_singletons = _drop_singletons(fixef_rm)
 
         # get all fixed effects combinations
         fixef_keys = list(self.var_dict.keys())
 
-        if self.ivars is not None:
-
-            if list(self.ivars.keys())[0] is not None:
-                ref = list(self.ivars.keys())[0]
-                ivars = self.ivars[ref]
-                drop_ref = ivars[0] + "[T." + ref + "]" + ":" + ivars[1]
-            else:
-                ivars = self.ivars[None]
-                drop_ref = None
-
-            # type checking
-            i0_type = self.data[ivars[0]].dtype
-            i1_type = self.data[ivars[1]].dtype
-            if not i0_type in ['category', "O"]:
-                raise ValueError("Column " + ivars[0] + " is not of type 'O' or 'category', which is required in the first position of i(). Instead it is of type " +
-                                 i0_type.name + ". If a reference level is set, it is required that the variable in the first position of 'i()' is of type 'O' or 'category'.")
-            if not i1_type in ['int64', 'float64', 'int32', 'float32']:
-                raise ValueError("Column " + ivars[1] + " is not of type 'int' or 'float', which is required in the second position of i(). Instead it is of type " +
-                                 i1_type.name + ". If a reference level is set, iti is required that the variable in the second position of 'i()' is of type 'int' or 'float'.")
-
-        else:
-            ivars = None
-            drop_ref = None
+        ivars, drop_ref = _clean_ivars(self.ivars, self.data)
 
         # dropped_data_dict and demeaned_data_dict are
         # dictionaries with keys for each fixed effects combination and
         # has values of lists of demeaned dataframes
         # the list is a singelton list unless split sample estimation is used
         # e.g it looks like this (without split estimation):
         # {'fe1': [demeaned_data_df], 'fe1+fe2': [demeaned_data_df]}
@@ -408,40 +383,20 @@
         self.yxz_name_dict = dict()
 
         estimate_full_model = True
         estimate_split_model = False
         # currently no fsplit allowed
         fsplit = None
 
-        if self.split is not None:
-            if fsplit is not None:
-                raise ValueError(
-                    "Cannot specify both split and fsplit. Please specify only one of the two.")
-            else:
-                self.splitvar = self.data[self.split]
-                estimate_full_model = False
-                estimate_split_model = True
-                splitvar_name = self.split
-        elif fsplit is not None:
-            self.splitvar = self.data[fsplit]
-            splitvar_name = fsplit
-            estimate_split_model = True
-        else:
-            self.splitvar = None
-
-        if self.splitvar is not None:
-            self.split_categories = np.unique(self.splitvar)
-            if splitvar_name not in self.data.columns:
-                raise ValueError("Split variable " +
-                                 self.splitvar + " not found in data.")
-            if splitvar_name in self.var_dict.keys():
-                raise ValueError("Split variable " + self.splitvar +
-                                 " cannot be a fixed effect variable.")
-            if self.splitvar.dtype.name != "category":
-                self.splitvar = pd.Categorical(self.splitvar)
+        self.splitvar, _, estimate_split_model, estimate_full_model = _prepare_split_estimation(
+            self.split,
+            fsplit,
+            self.data,
+            self.var_dict
+        )
 
         if estimate_full_model:
             for _, fval in enumerate(fixef_keys):
                 self.demeaned_data_dict[fval] = []
                 self.dropped_data_dict[fval] = []
                 self.yxz_name_dict[fval] = []
                 data = self.data
@@ -460,18 +415,29 @@
                     sub_data = self.data[x == self.splitvar]
                     demeaned_data, dropped_data, yxz_name_dict = self._demean(
                         sub_data, fval, ivars, drop_ref)
                     self.demeaned_data_dict[fval].append(demeaned_data)
                     self.dropped_data_dict[fval].append(dropped_data)
                     self.yxz_name_dict[fval].append(yxz_name_dict)
 
+        self.is_fixef_multi = False
+        if len(self.fml_dict.keys()) > 1:
+            self.is_fixef_multi = True
+        elif len(self.fml_dict.keys()) == 1:
+            first_key = next(iter(self.fml_dict))
+            if len(self.fml_dict[first_key]) > 1:
+                self.is_fixef_multi = True
+
+        if self.is_fixef_multi and self.is_iv:
+            raise ValueError("Multiple Estimations is currently not supported with IV. This is mostly due to insufficient testing and will be possible with the next release of PyFixest.")
+
         # estimate models based on demeaned model matrix and dependent variables
         for _, fval in enumerate(self.fml_dict.keys()):
             model_splits = self.demeaned_data_dict[fval]
-            for x, split in enumerate(model_splits):
+            for x, _ in enumerate(model_splits):
                 model_frames = model_splits[x]
                 for _, fml in enumerate(model_frames):
 
                     # get the (demeaned) model frame. key is fml without fixed effects
                     model_frame = model_frames[fml]
 
                     # update formula with fixed effect. fval is "0" for no fixed effect
@@ -507,50 +473,36 @@
                     X = X.to_numpy()
                     Z = Z.to_numpy()
 
                     N = X.shape[0]
                     k = X.shape[1]
 
                     # check for multicollinearity
-                    if np.linalg.matrix_rank(X) < min(X.shape):
-                        if self.ivars is not None:
-                            raise ValueError("The design Matrix X does not have full rank for the regression with fml" + fml2 +
-                                             ". The model is skipped. As you are running a regression via `i()` syntax, maybe you need to drop a level via i(var1, var2, ref = ...)?")
-                        else:
-                            raise ValueError(
-                                "The design Matrizx X does not have full rank for the regression with fml" + fml2 + ". The model is skipped. ")
+                    _multicollinearity_checks(X, Z, ivars, fml2)
 
                     FEOLS = Feols(Y, X, Z)
                     FEOLS.is_iv = self.is_iv
                     FEOLS.fml = fml2
                     FEOLS.ssc_dict = self.ssc_dict
-                    FEOLS.get_fit()
+                    if self.is_iv:
+                        FEOLS.get_fit(estimator = "2sls")
+                    else:
+                        FEOLS.get_fit(estimator = "ols")
                     FEOLS.na_index = self.dropped_data_dict[fval][x][fml]
                     FEOLS.data = self.data.iloc[~self.data.index.isin(
                         FEOLS.na_index), :]
                     FEOLS.N = N
                     FEOLS.k = k
                     if fval != "0":
                         FEOLS.has_fixef = True
                         FEOLS.fixef = fval
                     else:
                         FEOLS.has_fixef = False
 
-                    # FEOLS.get_nobs()
-
-                    if vcov is None:
-                        # iid if no fixed effects
-                        if fval == "0":
-                            vcov_type = "iid"
-                        else:
-                            # CRV1 inference, clustered by first fixed effect
-                            first_fe = fval.split("+")[0]
-                            vcov_type = {"CRV1": first_fe}
-                    else:
-                        vcov_type = vcov
+                    vcov_type = _get_vcov_type(vcov, fval)
 
                     FEOLS.vcov_log = vcov_type
                     FEOLS.split_log = x
                     FEOLS.get_vcov(vcov=vcov_type)
                     FEOLS.get_inference()
                     FEOLS.coefnames = colnames
                     if self.icovars is not None:
@@ -948,7 +900,182 @@
             ax.axvline(xintercept, color='red', linestyle='--', alpha=0.5)
         ax.set_ylabel('Coefficients')
         ax.set_title(model)
         ax.tick_params(axis='x', rotation=rotate_xticks)
 
         plt.show()
         plt.close()
+
+def _check_ivars(data, ivars):
+
+    '''
+    Checks if the variables in the i() syntax are of the correct type.
+    Args:
+        data (pandas.DataFrame): The dataframe containing the data used for the model fitting.
+        ivars (list): The list of variables specified in the i() syntax.
+    Returns:
+        None
+    '''
+
+    i0_type = data[ivars[0]].dtype
+    i1_type = data[ivars[1]].dtype
+    if not i0_type in ['category', "O"]:
+        raise ValueError("Column " + ivars[0] + " is not of type 'O' or 'category', which is required in the first position of i(). Instead it is of type " +
+                        i0_type.name + ". If a reference level is set, it is required that the variable in the first position of 'i()' is of type 'O' or 'category'.")
+        if not i1_type in ['int64', 'float64', 'int32', 'float32']:
+            raise ValueError("Column " + ivars[1] + " is not of type 'int' or 'float', which is required in the second position of i(). Instead it is of type " +
+                            i1_type.name + ". If a reference level is set, iti is required that the variable in the second position of 'i()' is of type 'int' or 'float'.")
+
+
+def _prepare_split_estimation(split, fsplit, data, var_dict):
+
+    '''
+    Cleans the input for the split estimation.
+    Checks if the split variables are of the correct type.
+
+    Args:
+        split (str): The name of the variable used for the split estimation.
+        fsplit (str): The name of the variable used for the fixed split estimation.
+        data (pandas.DataFrame): The dataframe containing the data used for the model fitting.
+        var_dict (dict): The dictionary containing the variables used in the model.
+    Returns:
+        splitvar (pandas.Series): The series containing the split variable.
+        splitvar_name (str): The name of the split variable. Either equal to split or fsplit.
+        estimate_split_model (bool): Whether to estimate the split model.
+        estimate_full_model (bool): Whether to estimate the full model.
+    '''
+
+    if split is not None:
+        if fsplit is not None:
+            raise ValueError(
+                "Cannot specify both split and fsplit. Please specify only one of the two.")
+        else:
+            splitvar = data[split]
+            estimate_full_model = False
+            estimate_split_model = True
+            splitvar_name = split
+    elif fsplit is not None:
+        splitvar = data[fsplit]
+        splitvar_name = fsplit
+        estimate_full_model = False
+        estimate_split_model = True
+    else:
+        splitvar = None
+        splitvar_name = None
+        estimate_split_model = False
+        estimate_full_model = True
+
+
+    if splitvar is not None:
+        split_categories = np.unique(splitvar)
+        if splitvar_name not in data.columns:
+            raise ValueError("Split variable " +
+                            splitvar + " not found in data.")
+        if splitvar_name in var_dict.keys():
+            raise ValueError("Split variable " + splitvar +
+                            " cannot be a fixed effect variable.")
+        if splitvar.dtype.name != "category":
+            splitvar = pd.Categorical(splitvar)
+
+    return splitvar, splitvar_name, estimate_split_model, estimate_full_model
+
+def _multicollinearity_checks(X, Z, ivars, fml2):
+
+    '''
+    Checks for multicollinearity in the design matrices X and Z.
+    Args:
+        X (numpy.ndarray): The design matrix X.
+        Z (numpy.ndarray): The design matrix (with instruments) Z.
+        ivars (list): The list of variables specified in the i() syntax.
+        fml2 (str): The formula string.
+
+    '''
+
+    if np.linalg.matrix_rank(X) < min(X.shape):
+        if ivars is not None:
+            raise ValueError("The design Matrix X does not have full rank for the regression with fml" + fml2 +
+                            ". The model is skipped. As you are running a regression via `i()` syntax, maybe you need to drop a level via i(var1, var2, ref = ...)?")
+        else:
+            raise ValueError(
+                    "The design Matrizx X does not have full rank for the regression with fml" + fml2 + ". The model is skipped. ")
+
+    if np.linalg.matrix_rank(Z) < min(Z.shape):
+        if ivars is not None:
+            raise ValueError("The design Matrix Z does not have full rank for the regression with fml" + fml2 +
+                            ". The model is skipped. As you are running a regression via `i()` syntax, maybe you need to drop a level via i(var1, var2, ref = ...)?")
+        else:
+            raise ValueError(
+                    "The design Matrix Z does not have full rank for the regression with fml" + fml2 + ". The model is skipped. ")
+
+def _get_vcov_type(vcov, fval):
+
+
+    '''
+    Passes the specified vcov type. If no vcov type specified, sets the default vcov type as iid if no fixed effect
+    is included in the model, and CRV1 clustered by the first fixed effect if a fixed effect is included in the model.
+    Args:
+        vcov (str): The specified vcov type.
+        fval (str): The specified fixed effects. (i.e. "X1+X2")
+    Returns:
+        vcov_type (str): The specified vcov type.
+    '''
+
+    if vcov is None:
+        # iid if no fixed effects
+        if fval == "0":
+            vcov_type = "iid"
+        else:
+            # CRV1 inference, clustered by first fixed effect
+            first_fe = fval.split("+")[0]
+            vcov_type = {"CRV1": first_fe}
+    else:
+        vcov_type = vcov
+
+    return vcov_type
+
+
+def _clean_ivars(ivars, data):
+
+    '''
+    Clean variables interacted via i(X1, X2, ref = a) syntax.
+
+    Args:
+        ivars (list): The list of variables specified in the i() syntax.
+        data (pandas.DataFrame): The dataframe containing the data used for the model fitting.
+    Returns:
+        ivars (list): The list of variables specified in the i() syntax minus the reference level
+        drop_ref (str): The dropped reference level specified in the i() syntax. None if no level is dropped
+    '''
+
+    if ivars is not None:
+
+        if list(ivars.keys())[0] is not None:
+            ref = list(ivars.keys())[0]
+            ivars = ivars[ref]
+            drop_ref = ivars[0] + "[T." + ref + "]" + ":" + ivars[1]
+        else:
+            ivars = ivars[None]
+            drop_ref = None
+
+        # type checking for ivars variable
+        _check_ivars(data, ivars)
+
+    else:
+        ivars = None
+        drop_ref = None
+
+    return ivars, drop_ref
+
+def _drop_singletons(fixef_rm):
+
+    '''
+    Checks if the fixef_rm argument is set to "singleton". If so, returns True, else False.
+    Args:
+        fixef_rm (str): The fixef_rm argument.
+    Returns:
+        drop_singletons (bool): Whether to drop singletons.
+    '''
+
+    if fixef_rm == "singleton":
+        return True
+    else:
+        return False
```

### Comparing `pyfixest-0.5.2/pyfixest/FormulaParser.py` & `pyfixest-0.6/pyfixest/FormulaParser.py`

 * *Files 10% similar despite different names*

```diff
@@ -46,36 +46,65 @@
 
         # Clean up the formula string
         fml = "".join(fml.split())
 
         # Split the formula string into its components
         fml_split = fml.split('|')
         depvars, covars = fml_split[0].split("~")
-
+          
         if len(fml_split) == 1:
             fevars = "0"
             endogvars = None
             instruments = None
         elif len(fml_split) == 2:
             if "~" in fml_split[1]:
                 fevars = "0"
                 endogvars, instruments = fml_split[1].split("~")
+                # add endogeneous variable to "covars" - yes, bad naming
+                
+                
+                # check if any of the instruments or endogeneous variables are also specified 
+                # as covariates
+                if any(element in covars.split("+") for element in endogvars.split("+")):
+                    raise ValueError("Endogeneous variables are specified as covariates in the first part of the three-part formula. This is not allowed.")
+                
+                if any(element in covars.split("+") for element in instruments.split("+")):
+                    raise ValueError("Instruments are specified as covariates in the first part of the three-part formula. This is not allowed.")
+                
+                if covars == "1": 
+                    covars = endogvars
+                else: 
+                    covars = endogvars + "+" +  covars
             else:
                 fevars = fml_split[1]
                 endogvars = None
                 instruments = None
         elif len(fml_split) == 3:
             fevars = fml_split[1]
             endogvars, instruments = fml_split[2].split("~")
 
+            # check if any of the instruments or endogeneous variables are also specified 
+            # as covariates
+            if any(element in covars.split("+") for element in endogvars.split("+")):
+                raise ValueError("Endogeneous variables are specified as covariates in the first part of the three-part formula. This is not allowed.")
+                
+            if any(element in covars.split("+") for element in instruments.split("+")):
+                raise ValueError("Instruments are specified as covariates in the first part of the three-part formula. This is not allowed.")
+
+            # add endogeneous variable to "covars" - yes, bad naming
+            if covars == "1": 
+                covars = endogvars
+            else: 
+                covars = endogvars + "+" +  covars
+
         if endogvars is not None:
             if len(endogvars) > len(instruments):
                 raise ValueError("The IV system is underdetermined. Only fully determined systems are allowed. Please provide as many instruments as endogenous variables.")
-            elif len(endogvars) < len(instruments):
-                raise ValueError("The IV system is overdetermined. Only fully determined systems are allowed. Please provide as many instruments as endogenous variables.")
+            #elif len(endogvars) < len(instruments):
+            #    raise ValueError("The IV system is overdetermined. Only fully determined systems are allowed. Please provide as many instruments as endogenous variables.")
             else:
                 pass
 
         # Parse all individual formula components into lists
         self.depvars = depvars.split("+")
         self.covars = _unpack_fml(covars)
         self.fevars = _unpack_fml(fevars)
```

### Comparing `pyfixest-0.5.2/pyfixest/ssc_utils.py` & `pyfixest-0.6/pyfixest/ssc_utils.py`

 * *Files identical despite different names*

### Comparing `pyfixest-0.5.2/pyfixest/utils.py` & `pyfixest-0.6/pyfixest/utils.py`

 * *Files 10% similar despite different names*

```diff
@@ -37,11 +37,14 @@
     data['group_id'] = cluster
     data['Y2'] = data.Y + np.random.normal(0, 1, N)
 
     data['Y'][0] = np.nan
     data['X1'][1] = np.nan
 
     data["Z1"] = data["X1"] + np.random.normal(0, 1, data.shape[0])
+    data["Z2"] = data["X2"] + np.random.normal(0, 1, data.shape[0])
+    data["Z3"] = data["X3"] + np.random.normal(0, 1, data.shape[0])
+
     #data['X2'][2] = np.nan
 
 
     return data
```

### Comparing `pyfixest-0.5.2/pyproject.toml` & `pyfixest-0.6/pyproject.toml`

 * *Files 14% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 [tool.poetry]
 name = "pyfixest"
-version = "0.5.2"
+version = "0.6"
 
-description = "Experimental draft package for high dimensional fixed effect estimation"
+description = "Experimental draft package for high dimensional fixed effect estimation. Supports OLS and IV estimation."
 authors = ["Alexander Fischer <alexander-fischer1801@t-online.de>"]
 license = "MIT"
 readme = "readme.md"
 homepage = "https://s3alfisc.github.io/pyfixest/"
 repository = "https://github.com/s3alfisc/pyfixest"
 
 [tool.poetry.dependencies]
```

### Comparing `pyfixest-0.5.2/readme.md` & `pyfixest-0.6/readme.md`

 * *Files identical despite different names*

### Comparing `pyfixest-0.5.2/PKG-INFO` & `pyfixest-0.6/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: pyfixest
-Version: 0.5.2
-Summary: Experimental draft package for high dimensional fixed effect estimation
+Version: 0.6
+Summary: Experimental draft package for high dimensional fixed effect estimation. Supports OLS and IV estimation.
 Home-page: https://s3alfisc.github.io/pyfixest/
 License: MIT
 Author: Alexander Fischer
 Author-email: alexander-fischer1801@t-online.de
 Requires-Python: >=3.8,<3.11
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

