# Comparing `tmp/efax-1.9.0.tar.gz` & `tmp/efax-1.9.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "efax-1.9.0.tar", max compression
+gzip compressed data, was "efax-1.9.1.tar", max compression
```

## Comparing `efax-1.9.0.tar` & `efax-1.9.1.tar`

### file list

```diff
@@ -1,55 +1,55 @@
--rw-r--r--   0        0        0     1069 2022-04-08 21:16:21.970328 efax-1.9.0/LICENSE
--rw-r--r--   0        0        0    10629 2022-08-16 20:34:32.877242 efax-1.9.0/README.rst
--rw-r--r--   0        0        0     3659 2022-09-14 15:50:53.366489 efax-1.9.0/efax/__init__.py
--rw-r--r--   0        0        0      278 2022-09-14 15:50:53.354488 efax-1.9.0/efax/_src/__init__.py
--rw-r--r--   0        0        0     1562 2022-09-14 15:50:53.366489 efax-1.9.0/efax/_src/conjugate_prior.py
--rw-r--r--   0        0        0      506 2022-09-14 15:50:53.358488 efax-1.9.0/efax/_src/distributions/__init__.py
--rw-r--r--   0        0        0     2819 2022-09-29 00:35:04.447741 efax-1.9.0/efax/_src/distributions/bernoulli.py
--rw-r--r--   0        0        0     1866 2022-09-29 00:35:17.311788 efax-1.9.0/efax/_src/distributions/beta.py
--rw-r--r--   0        0        0     2022 2022-09-14 15:50:53.354488 efax-1.9.0/efax/_src/distributions/chi.py
--rw-r--r--   0        0        0     2412 2022-09-14 15:50:53.358488 efax-1.9.0/efax/_src/distributions/chi_square.py
--rw-r--r--   0        0        0      136 2022-09-14 15:50:53.358488 efax-1.9.0/efax/_src/distributions/cmvn/__init__.py
--rw-r--r--   0        0        0     3600 2022-09-29 00:35:42.767881 efax-1.9.0/efax/_src/distributions/cmvn/circularly_symmetric.py
--rw-r--r--   0        0        0     3937 2022-09-14 15:53:34.100902 efax-1.9.0/efax/_src/distributions/cmvn/unit.py
--rw-r--r--   0        0        0     3502 2022-09-14 15:50:53.358488 efax-1.9.0/efax/_src/distributions/complex_normal.py
--rw-r--r--   0        0        0     1248 2022-09-14 15:50:53.358488 efax-1.9.0/efax/_src/distributions/dirichlet.py
--rw-r--r--   0        0        0     2985 2022-09-14 15:53:34.100902 efax-1.9.0/efax/_src/distributions/dirichlet_common.py
--rw-r--r--   0        0        0     2496 2022-09-14 15:53:34.100902 efax-1.9.0/efax/_src/distributions/exponential.py
--rw-r--r--   0        0        0     3292 2022-09-14 15:53:47.853107 efax-1.9.0/efax/_src/distributions/gamma.py
--rw-r--r--   0        0        0     4657 2022-09-14 15:50:53.366489 efax-1.9.0/efax/_src/distributions/gen_dirichlet.py
--rw-r--r--   0        0        0     1242 2022-09-14 15:50:53.358488 efax-1.9.0/efax/_src/distributions/geometric.py
--rw-r--r--   0        0        0     2965 2022-09-14 15:50:53.358488 efax-1.9.0/efax/_src/distributions/logarithmic.py
--rw-r--r--   0        0        0     4519 2022-09-14 15:53:34.100902 efax-1.9.0/efax/_src/distributions/multinomial.py
--rw-r--r--   0        0        0      124 2022-09-14 15:50:53.358488 efax-1.9.0/efax/_src/distributions/multivariate_normal/__init__.py
--rw-r--r--   0        0        0     4784 2022-09-29 00:35:56.655932 efax-1.9.0/efax/_src/distributions/multivariate_normal/arbitrary.py
--rw-r--r--   0        0        0     4574 2022-09-14 15:53:34.100902 efax-1.9.0/efax/_src/distributions/multivariate_normal/diagonal.py
--rw-r--r--   0        0        0     4545 2022-09-14 15:53:34.100902 efax-1.9.0/efax/_src/distributions/multivariate_normal/fixed_variance.py
--rw-r--r--   0        0        0     3560 2022-09-14 15:53:34.100902 efax-1.9.0/efax/_src/distributions/multivariate_normal/isotropic.py
--rw-r--r--   0        0        0     3712 2022-09-14 15:53:34.100902 efax-1.9.0/efax/_src/distributions/multivariate_normal/unit.py
--rw-r--r--   0        0        0     1456 2022-09-14 15:50:53.358488 efax-1.9.0/efax/_src/distributions/negative_binomial.py
--rw-r--r--   0        0        0     1855 2022-09-14 15:50:53.358488 efax-1.9.0/efax/_src/distributions/negative_binomial_common.py
--rw-r--r--   0        0        0     2725 2022-09-14 15:53:34.100902 efax-1.9.0/efax/_src/distributions/normal.py
--rw-r--r--   0        0        0     2263 2022-09-29 00:35:26.823823 efax-1.9.0/efax/_src/distributions/poisson.py
--rw-r--r--   0        0        0     2036 2022-09-14 15:50:53.358488 efax-1.9.0/efax/_src/distributions/rayleigh.py
--rw-r--r--   0        0        0     4066 2022-09-14 15:53:32.476877 efax-1.9.0/efax/_src/distributions/von_mises.py
--rw-r--r--   0        0        0     2517 2022-09-29 00:36:07.551972 efax-1.9.0/efax/_src/distributions/weibull.py
--rw-r--r--   0        0        0     5771 2022-09-14 15:50:53.366489 efax-1.9.0/efax/_src/exp_to_nat.py
--rw-r--r--   0        0        0     2568 2022-09-14 15:50:53.354488 efax-1.9.0/efax/_src/expectation_parametrization.py
--rw-r--r--   0        0        0      223 2022-09-14 15:50:53.354488 efax-1.9.0/efax/_src/multidimensional.py
--rw-r--r--   0        0        0     5523 2022-09-14 15:50:53.354488 efax-1.9.0/efax/_src/natural_parametrization.py
--rw-r--r--   0        0        0     5307 2022-09-14 15:50:53.366489 efax-1.9.0/efax/_src/parameter.py
--rw-r--r--   0        0        0     5997 2022-09-14 15:50:53.354488 efax-1.9.0/efax/_src/parametrization.py
--rw-r--r--   0        0        0      313 2022-09-14 15:53:34.100902 efax-1.9.0/efax/_src/samplable.py
--rw-r--r--   0        0        0      158 2022-09-14 15:50:53.354488 efax-1.9.0/efax/_src/scipy_replacement/__init__.py
--rw-r--r--   0        0        0     6497 2022-09-29 00:36:50.032127 efax-1.9.0/efax/_src/scipy_replacement/complex_multivariate_normal.py
--rw-r--r--   0        0        0     6258 2022-09-29 00:45:48.874097 efax-1.9.0/efax/_src/scipy_replacement/complex_normal.py
--rw-r--r--   0        0        0     3070 2022-09-29 00:38:30.864496 efax-1.9.0/efax/_src/scipy_replacement/dirichlet.py
--rw-r--r--   0        0        0     1898 2022-09-29 00:38:47.480556 efax-1.9.0/efax/_src/scipy_replacement/multivariate_normal.py
--rw-r--r--   0        0        0     1757 2022-09-29 00:34:43.959667 efax-1.9.0/efax/_src/scipy_replacement/shaped_distribution.py
--rw-r--r--   0        0        0      904 2022-09-29 00:38:55.992587 efax-1.9.0/efax/_src/scipy_replacement/von_mises.py
--rw-r--r--   0        0        0     2527 2022-09-29 00:45:48.870097 efax-1.9.0/efax/_src/tools.py
--rw-r--r--   0        0        0     2738 2022-09-14 15:50:53.366489 efax-1.9.0/efax/_src/transformed_parametrization.py
--rw-r--r--   0        0        0        0 2022-04-08 21:16:21.970328 efax-1.9.0/efax/py.typed
--rw-r--r--   0        0        0     3066 2022-09-29 00:46:31.206252 efax-1.9.0/pyproject.toml
--rw-r--r--   0        0        0    11501 1970-01-01 00:00:00.000000 efax-1.9.0/setup.py
--rw-r--r--   0        0        0    11656 1970-01-01 00:00:00.000000 efax-1.9.0/PKG-INFO
+-rw-r--r--   0        0        0     1069 2022-04-08 21:16:21.970328 efax-1.9.1/LICENSE
+-rw-r--r--   0        0        0    10624 2022-11-15 21:41:38.827624 efax-1.9.1/README.rst
+-rw-r--r--   0        0        0     3659 2022-09-14 15:50:53.366489 efax-1.9.1/efax/__init__.py
+-rw-r--r--   0        0        0      278 2022-09-14 15:50:53.354488 efax-1.9.1/efax/_src/__init__.py
+-rw-r--r--   0        0        0     1562 2022-09-14 15:50:53.366489 efax-1.9.1/efax/_src/conjugate_prior.py
+-rw-r--r--   0        0        0      506 2022-09-14 15:50:53.358488 efax-1.9.1/efax/_src/distributions/__init__.py
+-rw-r--r--   0        0        0     2819 2022-09-29 00:35:04.447741 efax-1.9.1/efax/_src/distributions/bernoulli.py
+-rw-r--r--   0        0        0     1866 2022-09-29 00:35:17.311788 efax-1.9.1/efax/_src/distributions/beta.py
+-rw-r--r--   0        0        0     2022 2022-09-14 15:50:53.354488 efax-1.9.1/efax/_src/distributions/chi.py
+-rw-r--r--   0        0        0     2412 2022-09-14 15:50:53.358488 efax-1.9.1/efax/_src/distributions/chi_square.py
+-rw-r--r--   0        0        0      136 2022-09-14 15:50:53.358488 efax-1.9.1/efax/_src/distributions/cmvn/__init__.py
+-rw-r--r--   0        0        0     3600 2022-09-29 00:35:42.767881 efax-1.9.1/efax/_src/distributions/cmvn/circularly_symmetric.py
+-rw-r--r--   0        0        0     3937 2022-09-14 15:53:34.100902 efax-1.9.1/efax/_src/distributions/cmvn/unit.py
+-rw-r--r--   0        0        0     3502 2022-09-14 15:50:53.358488 efax-1.9.1/efax/_src/distributions/complex_normal.py
+-rw-r--r--   0        0        0     1248 2022-09-14 15:50:53.358488 efax-1.9.1/efax/_src/distributions/dirichlet.py
+-rw-r--r--   0        0        0     2985 2022-09-14 15:53:34.100902 efax-1.9.1/efax/_src/distributions/dirichlet_common.py
+-rw-r--r--   0        0        0     2496 2022-09-14 15:53:34.100902 efax-1.9.1/efax/_src/distributions/exponential.py
+-rw-r--r--   0        0        0     3292 2022-09-14 15:53:47.853107 efax-1.9.1/efax/_src/distributions/gamma.py
+-rw-r--r--   0        0        0     4657 2022-09-14 15:50:53.366489 efax-1.9.1/efax/_src/distributions/gen_dirichlet.py
+-rw-r--r--   0        0        0     1242 2022-09-14 15:50:53.358488 efax-1.9.1/efax/_src/distributions/geometric.py
+-rw-r--r--   0        0        0     2965 2022-09-14 15:50:53.358488 efax-1.9.1/efax/_src/distributions/logarithmic.py
+-rw-r--r--   0        0        0     4519 2022-09-14 15:53:34.100902 efax-1.9.1/efax/_src/distributions/multinomial.py
+-rw-r--r--   0        0        0      124 2022-09-14 15:50:53.358488 efax-1.9.1/efax/_src/distributions/multivariate_normal/__init__.py
+-rw-r--r--   0        0        0     4784 2022-09-29 00:35:56.655932 efax-1.9.1/efax/_src/distributions/multivariate_normal/arbitrary.py
+-rw-r--r--   0        0        0     4574 2022-09-14 15:53:34.100902 efax-1.9.1/efax/_src/distributions/multivariate_normal/diagonal.py
+-rw-r--r--   0        0        0     4545 2022-09-14 15:53:34.100902 efax-1.9.1/efax/_src/distributions/multivariate_normal/fixed_variance.py
+-rw-r--r--   0        0        0     3560 2022-09-14 15:53:34.100902 efax-1.9.1/efax/_src/distributions/multivariate_normal/isotropic.py
+-rw-r--r--   0        0        0     3712 2022-09-14 15:53:34.100902 efax-1.9.1/efax/_src/distributions/multivariate_normal/unit.py
+-rw-r--r--   0        0        0     1456 2022-09-14 15:50:53.358488 efax-1.9.1/efax/_src/distributions/negative_binomial.py
+-rw-r--r--   0        0        0     1885 2022-11-15 21:32:40.391431 efax-1.9.1/efax/_src/distributions/negative_binomial_common.py
+-rw-r--r--   0        0        0     2725 2022-09-14 15:53:34.100902 efax-1.9.1/efax/_src/distributions/normal.py
+-rw-r--r--   0        0        0     2263 2022-09-29 00:35:26.823823 efax-1.9.1/efax/_src/distributions/poisson.py
+-rw-r--r--   0        0        0     2036 2022-09-14 15:50:53.358488 efax-1.9.1/efax/_src/distributions/rayleigh.py
+-rw-r--r--   0        0        0     4066 2022-09-14 15:53:32.476877 efax-1.9.1/efax/_src/distributions/von_mises.py
+-rw-r--r--   0        0        0     2517 2022-09-29 00:36:07.551972 efax-1.9.1/efax/_src/distributions/weibull.py
+-rw-r--r--   0        0        0     5771 2022-09-14 15:50:53.366489 efax-1.9.1/efax/_src/exp_to_nat.py
+-rw-r--r--   0        0        0     2568 2022-09-14 15:50:53.354488 efax-1.9.1/efax/_src/expectation_parametrization.py
+-rw-r--r--   0        0        0      223 2022-09-14 15:50:53.354488 efax-1.9.1/efax/_src/multidimensional.py
+-rw-r--r--   0        0        0     5523 2022-09-14 15:50:53.354488 efax-1.9.1/efax/_src/natural_parametrization.py
+-rw-r--r--   0        0        0     5307 2022-09-14 15:50:53.366489 efax-1.9.1/efax/_src/parameter.py
+-rw-r--r--   0        0        0     5997 2022-09-14 15:50:53.354488 efax-1.9.1/efax/_src/parametrization.py
+-rw-r--r--   0        0        0      313 2022-09-14 15:53:34.100902 efax-1.9.1/efax/_src/samplable.py
+-rw-r--r--   0        0        0      158 2022-09-14 15:50:53.354488 efax-1.9.1/efax/_src/scipy_replacement/__init__.py
+-rw-r--r--   0        0        0     6497 2022-09-29 00:36:50.032127 efax-1.9.1/efax/_src/scipy_replacement/complex_multivariate_normal.py
+-rw-r--r--   0        0        0     6258 2022-09-29 00:45:48.874097 efax-1.9.1/efax/_src/scipy_replacement/complex_normal.py
+-rw-r--r--   0        0        0     3070 2022-09-29 00:38:30.864496 efax-1.9.1/efax/_src/scipy_replacement/dirichlet.py
+-rw-r--r--   0        0        0     1898 2022-09-29 00:38:47.480556 efax-1.9.1/efax/_src/scipy_replacement/multivariate_normal.py
+-rw-r--r--   0        0        0     1757 2022-09-29 00:34:43.959667 efax-1.9.1/efax/_src/scipy_replacement/shaped_distribution.py
+-rw-r--r--   0        0        0      904 2022-09-29 00:38:55.992587 efax-1.9.1/efax/_src/scipy_replacement/von_mises.py
+-rw-r--r--   0        0        0     2527 2022-09-29 00:45:48.870097 efax-1.9.1/efax/_src/tools.py
+-rw-r--r--   0        0        0     2738 2022-09-14 15:50:53.366489 efax-1.9.1/efax/_src/transformed_parametrization.py
+-rw-r--r--   0        0        0        0 2022-04-08 21:16:21.970328 efax-1.9.1/efax/py.typed
+-rw-r--r--   0        0        0     3066 2022-11-15 21:42:20.844391 efax-1.9.1/pyproject.toml
+-rw-r--r--   0        0        0    11496 1970-01-01 00:00:00.000000 efax-1.9.1/setup.py
+-rw-r--r--   0        0        0    11654 1970-01-01 00:00:00.000000 efax-1.9.1/PKG-INFO
```

### Comparing `efax-1.9.0/LICENSE` & `efax-1.9.1/LICENSE`

 * *Files identical despite different names*

### Comparing `efax-1.9.0/README.rst` & `efax-1.9.1/README.rst`

 * *Files 0% similar despite different names*

```diff
@@ -279,13 +279,10 @@
 - Add the new distribution to the tests by adding it to `create_info <https://github.com/NeilGirdhar/efax/blob/master/tests/create_info.py>`_.)
 
 Implementation should respect PEP8.
 The tests can be run using :bash:`pytest . -n auto`.
 There are a few tools to clean and check the source:
 
 - :bash:`isort .`
-
-- :bash:`pylint efax`
-
-- :bash:`flake8 efax`
-
-- :bash:`mypy efax`
+- :bash:`mypy .`
+- :bash:`pylint efax tests`
+- :bash:`pflake8 .`
```

### Comparing `efax-1.9.0/efax/__init__.py` & `efax-1.9.1/efax/__init__.py`

 * *Files identical despite different names*

### Comparing `efax-1.9.0/efax/_src/conjugate_prior.py` & `efax-1.9.1/efax/_src/conjugate_prior.py`

 * *Files identical despite different names*

### Comparing `efax-1.9.0/efax/_src/distributions/bernoulli.py` & `efax-1.9.1/efax/_src/distributions/bernoulli.py`

 * *Files identical despite different names*

### Comparing `efax-1.9.0/efax/_src/distributions/beta.py` & `efax-1.9.1/efax/_src/distributions/beta.py`

 * *Files identical despite different names*

### Comparing `efax-1.9.0/efax/_src/distributions/chi.py` & `efax-1.9.1/efax/_src/distributions/chi.py`

 * *Files identical despite different names*

### Comparing `efax-1.9.0/efax/_src/distributions/chi_square.py` & `efax-1.9.1/efax/_src/distributions/chi_square.py`

 * *Files identical despite different names*

### Comparing `efax-1.9.0/efax/_src/distributions/cmvn/circularly_symmetric.py` & `efax-1.9.1/efax/_src/distributions/cmvn/circularly_symmetric.py`

 * *Files identical despite different names*

### Comparing `efax-1.9.0/efax/_src/distributions/cmvn/unit.py` & `efax-1.9.1/efax/_src/distributions/cmvn/unit.py`

 * *Files identical despite different names*

### Comparing `efax-1.9.0/efax/_src/distributions/complex_normal.py` & `efax-1.9.1/efax/_src/distributions/complex_normal.py`

 * *Files identical despite different names*

### Comparing `efax-1.9.0/efax/_src/distributions/dirichlet.py` & `efax-1.9.1/efax/_src/distributions/dirichlet.py`

 * *Files identical despite different names*

### Comparing `efax-1.9.0/efax/_src/distributions/dirichlet_common.py` & `efax-1.9.1/efax/_src/distributions/dirichlet_common.py`

 * *Files identical despite different names*

### Comparing `efax-1.9.0/efax/_src/distributions/exponential.py` & `efax-1.9.1/efax/_src/distributions/exponential.py`

 * *Files identical despite different names*

### Comparing `efax-1.9.0/efax/_src/distributions/gamma.py` & `efax-1.9.1/efax/_src/distributions/gamma.py`

 * *Files identical despite different names*

### Comparing `efax-1.9.0/efax/_src/distributions/gen_dirichlet.py` & `efax-1.9.1/efax/_src/distributions/gen_dirichlet.py`

 * *Files identical despite different names*

### Comparing `efax-1.9.0/efax/_src/distributions/geometric.py` & `efax-1.9.1/efax/_src/distributions/geometric.py`

 * *Files identical despite different names*

### Comparing `efax-1.9.0/efax/_src/distributions/logarithmic.py` & `efax-1.9.1/efax/_src/distributions/logarithmic.py`

 * *Files identical despite different names*

### Comparing `efax-1.9.0/efax/_src/distributions/multinomial.py` & `efax-1.9.1/efax/_src/distributions/multinomial.py`

 * *Files identical despite different names*

### Comparing `efax-1.9.0/efax/_src/distributions/multivariate_normal/arbitrary.py` & `efax-1.9.1/efax/_src/distributions/multivariate_normal/arbitrary.py`

 * *Files identical despite different names*

### Comparing `efax-1.9.0/efax/_src/distributions/multivariate_normal/diagonal.py` & `efax-1.9.1/efax/_src/distributions/multivariate_normal/diagonal.py`

 * *Files identical despite different names*

### Comparing `efax-1.9.0/efax/_src/distributions/multivariate_normal/fixed_variance.py` & `efax-1.9.1/efax/_src/distributions/multivariate_normal/fixed_variance.py`

 * *Files identical despite different names*

### Comparing `efax-1.9.0/efax/_src/distributions/multivariate_normal/isotropic.py` & `efax-1.9.1/efax/_src/distributions/multivariate_normal/isotropic.py`

 * *Files identical despite different names*

### Comparing `efax-1.9.0/efax/_src/distributions/multivariate_normal/unit.py` & `efax-1.9.1/efax/_src/distributions/multivariate_normal/unit.py`

 * *Files identical despite different names*

### Comparing `efax-1.9.0/efax/_src/distributions/negative_binomial.py` & `efax-1.9.1/efax/_src/distributions/negative_binomial.py`

 * *Files identical despite different names*

### Comparing `efax-1.9.0/efax/_src/distributions/negative_binomial_common.py` & `efax-1.9.1/efax/_src/distributions/negative_binomial_common.py`

 * *Files 11% similar despite different names*

```diff
@@ -18,15 +18,15 @@
 
     # Implemented methods --------------------------------------------------------------------------
     @property
     def shape(self) -> Shape:
         return self.log_not_p.shape
 
     def log_normalizer(self) -> RealArray:
-        return -self.failures * jnp.log1p(-jnp.exp(self.log_not_p))
+        return -self.failures * jnp.log1p(-jnp.exp(self.log_not_p))  # type: ignore[return-value]
 
     def carrier_measure(self, x: RealArray) -> RealArray:
         a = x + self.failures - 1
         # Return log(a choose x).
         return gammaln(a + 1) - gammaln(x + 1) - gammaln(a - x + 1)
 
     # Private methods ------------------------------------------------------------------------------
```

### Comparing `efax-1.9.0/efax/_src/distributions/normal.py` & `efax-1.9.1/efax/_src/distributions/normal.py`

 * *Files identical despite different names*

### Comparing `efax-1.9.0/efax/_src/distributions/poisson.py` & `efax-1.9.1/efax/_src/distributions/poisson.py`

 * *Files identical despite different names*

### Comparing `efax-1.9.0/efax/_src/distributions/rayleigh.py` & `efax-1.9.1/efax/_src/distributions/rayleigh.py`

 * *Files identical despite different names*

### Comparing `efax-1.9.0/efax/_src/distributions/von_mises.py` & `efax-1.9.1/efax/_src/distributions/von_mises.py`

 * *Files identical despite different names*

### Comparing `efax-1.9.0/efax/_src/distributions/weibull.py` & `efax-1.9.1/efax/_src/distributions/weibull.py`

 * *Files identical despite different names*

### Comparing `efax-1.9.0/efax/_src/exp_to_nat.py` & `efax-1.9.1/efax/_src/exp_to_nat.py`

 * *Files identical despite different names*

### Comparing `efax-1.9.0/efax/_src/expectation_parametrization.py` & `efax-1.9.1/efax/_src/expectation_parametrization.py`

 * *Files identical despite different names*

### Comparing `efax-1.9.0/efax/_src/natural_parametrization.py` & `efax-1.9.1/efax/_src/natural_parametrization.py`

 * *Files identical despite different names*

### Comparing `efax-1.9.0/efax/_src/parameter.py` & `efax-1.9.1/efax/_src/parameter.py`

 * *Files identical despite different names*

### Comparing `efax-1.9.0/efax/_src/parametrization.py` & `efax-1.9.1/efax/_src/parametrization.py`

 * *Files identical despite different names*

### Comparing `efax-1.9.0/efax/_src/scipy_replacement/complex_multivariate_normal.py` & `efax-1.9.1/efax/_src/scipy_replacement/complex_multivariate_normal.py`

 * *Files identical despite different names*

### Comparing `efax-1.9.0/efax/_src/scipy_replacement/complex_normal.py` & `efax-1.9.1/efax/_src/scipy_replacement/complex_normal.py`

 * *Files identical despite different names*

### Comparing `efax-1.9.0/efax/_src/scipy_replacement/dirichlet.py` & `efax-1.9.1/efax/_src/scipy_replacement/dirichlet.py`

 * *Files identical despite different names*

### Comparing `efax-1.9.0/efax/_src/scipy_replacement/multivariate_normal.py` & `efax-1.9.1/efax/_src/scipy_replacement/multivariate_normal.py`

 * *Files identical despite different names*

### Comparing `efax-1.9.0/efax/_src/scipy_replacement/shaped_distribution.py` & `efax-1.9.1/efax/_src/scipy_replacement/shaped_distribution.py`

 * *Files identical despite different names*

### Comparing `efax-1.9.0/efax/_src/scipy_replacement/von_mises.py` & `efax-1.9.1/efax/_src/scipy_replacement/von_mises.py`

 * *Files identical despite different names*

### Comparing `efax-1.9.0/efax/_src/tools.py` & `efax-1.9.1/efax/_src/tools.py`

 * *Files identical despite different names*

### Comparing `efax-1.9.0/efax/_src/transformed_parametrization.py` & `efax-1.9.1/efax/_src/transformed_parametrization.py`

 * *Files identical despite different names*

### Comparing `efax-1.9.0/pyproject.toml` & `efax-1.9.1/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ['setuptools', 'poetry_core>=1.0']
 build-backend = 'poetry.core.masonry.api'
 
 [tool.poetry]
 name = 'efax'
-version = "1.9.0"
+version = "1.9.1"
 description = "Exponential families for JAX"
 license = 'MIT'
 authors = ['Neil Girdhar <mistersheik@gmail.com>']
 readme = 'README.rst'
 repository = 'https://github.com/NeilGirdhar/efax'
 classifiers = [
     'Development Status :: 5 - Production/Stable',
```

### Comparing `efax-1.9.0/setup.py` & `efax-1.9.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -17,17 +17,17 @@
  'numpy>=1.22',
  'scipy>=1.4,<2.0',
  'tensorflow_probability>=0.15',
  'tjax>=0.21.3']
 
 setup_kwargs = {
     'name': 'efax',
-    'version': '1.9.0',
+    'version': '1.9.1',
     'description': 'Exponential families for JAX',
-    'long_description': "=================================\nEFAX: Exponential Families in JAX\n=================================\n.. image:: https://badge.fury.io/py/efax.svg\n    :target: https://badge.fury.io/py/efax\n\n.. role:: bash(code)\n    :language: bash\n\n.. role:: python(code)\n   :language: python\n\nThis library provides a set of tools for working with *exponential family distributions* in the\ndifferential programming library `JAX <https://github.com/google/jax/>`_.\n\nThe *exponential families* are an important class of probability distributions that include the\nnormal, gamma, beta, exponential, Poisson, binomial, and Bernoulli distributions.\nFor an explanation of the fundamental ideas behind this library, see our `overview on exponential\nfamilies <https://github.com/NeilGirdhar/efax/blob/master/expfam.pdf>`_.\n\nThe main motivation for using EFAX over a library like tensorflow-probability or the basic functions\nin JAX is that EFAX provides the two most important parametrizations for each exponential family—the\nnatural and expectation parametrizations—and a uniform interface to efficient implementations of the\nmain functions used in machine learning.  An example of why this matters is that the most efficient\nway to implement cross entropy between X and Y relies on X being in the expectation parametrization\nand Y in the natural parametrization.\n\nFramework\n=========\nRepresentation\n--------------\nEFAX has a single base class for its objects: :python:`Parametrization` whose type encodes the\ndistribution family.\n\nEach parametrization object has a shape, and so it can store any number of distributions.\nOperations on these objects are vectorized.\nThis is unlike SciPy where each distribution is represented by a single object, and so a thousand\ndistributions need a thousand objects, and corresponding calls to functions that operate on them.\n\nAll parametrization objects are dataclasses using :python:`tjax.dataclass`.  These dataclasses are\na modification of Python's dataclasses to support JAX's “PyTree” type registration.\n\nEach of the fields of a parametrization object stores a parameter over a specified support.\nSome parameters are marked as “fixed”, which means that they are fixed with respect to the\nexponential family.  An example of a fixed parameter is the failure number of the negative binomial\ndistribution.\n\nFor example:\n\n.. code:: python\n\n    @dataclass\n    class MultivariateNormalNP(NaturalParametrization['MultivariateNormalEP']):\n        mean_times_precision: RealArray = distribution_parameter(VectorSupport())\n        negative_half_precision: RealArray = distribution_parameter(SymmetricMatrixSupport())\n\nIn this case, we see that there are two natural parameters for the multivariate normal distribution.\nObjects of this type can hold any number of distributions:  if such an object :python:`x` has shape\n:python:`s`, then the shape of\n:python:`x.mean_times_precision` is :python:`(*s, n)` and the shape of\n:python:`x.negative_half_precision` is :python:`(*s, n, n)`.\n\nParametrizations\n----------------\nEach exponential family distribution has two special parametrizations: the natural and the\nexpectation parametrization.  (These are described in the overview pdf.)\nConsequently, every distribution has at least two base classes, one inheriting from\n:python:`NaturalParametrization` and one from :python:`ExpectationParametrization`.\n\nThe motivation for the natural parametrization is combining and scaling independent predictive\nevidence.  In the natural parametrization, these operations correspond to scaling and addition.\n\nThe motivation for the expectation parametrization is combining independent observations into the\nmaximum likelihood distribution that could have produced them.  In the expectation parametrization,\nthis is an expected value.\n\nEFAX provides conversions between the two parametrizations through the\n:python:`NaturalParametrization.to_exp` and :python:`ExpectationParametrization.to_nat` methods.\n\nImportant methods\n-----------------\nEFAX aims to provide the main methods used in machine learning.\n\nEvery :python:`Parametrization` has methods to flatten and unflatten the parameters into a single\narray: :python:`flattened` and :python:`unflattened`.  Typically, array-valued signals in a machine\nlearning model would be unflattened into a distribution object, operated on, and then flattened\nbefore being sent back to the model.  Flattening is careful with distributions with symmetric (or Hermitian) matrix-valued parameters.  It only stores the upper triangular elements.\n\nEvery :python:`NaturalParametrization` has methods:\n\n- :python:`sufficient_statistics` to produce the sufficient statistics given an observation (used in\n  maximum likelihood estimation),\n- :python:`pdf`, which is the density or mass function,\n- :python:`fisher_information`, which is the Fisher information matrix, and\n- :python:`entropy`, which is the Shannon entropy.\n\nEvery :python:`ExpectationParametrization` has methods:\n\n- :python:`cross_entropy` that is an efficient cross entropy armed with a numerically optimized\n  custom JAX gradient.  This is possible because the gradient of the cross entropy is the difference\n  of expectation parameters plus the expected carrier measure.\n\nNumerical optimization\n----------------------\nBecause of the nature of the log-normalizer and carrier measure, some methods for some distributions\nrequire numerical optimization.  These are the conversion from expectation parameters to natural\nones, the entropy, and the cross entropy.\n\nDistributions\n=============\nEFAX supports the following distributions:\n\n- normal:\n\n  - univariate real\n  - univariate complex\n  - multivariate real:\n\n    - with fixed unit variance\n    - with fixed variance\n    - with isotropic variance\n    - with diagonal variance\n    - with general variance\n\n  - multivariate complex:\n\n    - with unit variance and zero pseudo-variance\n    - circularly symmetric\n\n- on a finite set:\n\n  - Bernoulli\n  - multinomial\n\n- on the nonnegative integers:\n\n  - geometric\n  - logarithmic\n  - negative binomial\n  - Poisson\n\n- on the positive reals:\n\n  - chi\n  - chi-square\n  - exponential\n  - gamma\n  - Rayleigh\n  - Weibull\n\n- on the simplex:\n\n  - beta\n  - Dirichlet\n  - generalized Dirichlet\n\n- on the n-sphere:\n\n  - von Mises-Fisher\n\nUsage\n=====\nBasic usage\n-----------\nA basic use of the two parametrizations:\n\n.. code:: python\n\n    from jax import numpy as jnp\n\n    from efax import BernoulliEP, BernoulliNP\n\n    # p is the expectation parameters of three Bernoulli distributions having probabilities 0.4, 0.5,\n    # and 0.6.\n    p = BernoulliEP(jnp.array([0.4, 0.5, 0.6]))\n\n    # q is the natural parameters of three Bernoulli distributions having log-odds 0, which is\n    # probability 0.5.\n    q = BernoulliNP(jnp.zeros(3))\n\n    print(p.cross_entropy(q))\n    # [0.6931472 0.6931472 0.6931472]\n\n    # q2 is natural parameters of Bernoulli distributions having a probability of 0.3.\n    p2 = BernoulliEP(0.3 * jnp.ones(3))\n    q2 = p2.to_nat()\n\n    print(p.cross_entropy(q2))\n    # [0.6955941  0.78032386 0.86505365]\n    # A Bernoulli distribution with probability 0.3 predicts a Bernoulli observation with probability\n    # 0.4 better than the other observations.\n\nOptimization\n------------\nUsing the cross entropy to iteratively optimize a prediction is simple:\n\n.. code:: python\n\n    import jax.numpy as jnp\n    from jax import grad, jit, lax\n    from jax.tree_util import tree_map, tree_reduce\n    from tjax import BooleanNumeric, RealArray, RealNumeric\n\n    from efax import BernoulliEP, BernoulliNP\n\n\n    def cross_entropy_loss(p: BernoulliEP, q: BernoulliNP) -> RealNumeric:\n        return jnp.sum(p.cross_entropy(q))\n\n\n    gce = jit(grad(cross_entropy_loss, 1))\n\n\n    def apply(x: RealArray, x_bar: RealArray) -> RealArray:\n        return x - 1e-4 * x_bar\n\n\n    def body_fun(q: BernoulliNP) -> BernoulliNP:\n        q_bar = gce(some_p, q)\n        return tree_map(apply, q, q_bar)\n\n\n    def cond_fun(q: BernoulliNP) -> BooleanNumeric:\n        q_bar = gce(some_p, q)\n        total = tree_reduce(jnp.sum,\n                            tree_map(lambda x: jnp.sum(jnp.square(x)), q_bar))\n        return total > 1e-6\n\n\n    # some_p are expectation parameters of a Bernoulli distribution corresponding\n    # to probabilities 0.3, 0.4, and 0.7.\n    some_p = BernoulliEP(jnp.array([0.3, 0.4, 0.7]))\n\n    # some_q are natural parameters of a Bernoulli distribution corresponding to\n    # log-odds 0, which is probability 0.5.\n    some_q = BernoulliNP(jnp.zeros(3))\n\n    # Optimize the predictive distribution iteratively, and output the natural parameters of the\n    # prediction.\n    optimized_q = lax.while_loop(cond_fun, body_fun, some_q)\n    print(optimized_q)\n    # BernoulliNP\n    #     log_odds=Jax Array (3,) float32\n    #            -0.8440     -0.4047      0.8440\n\n    # Compare with the true value.\n    print(some_p.to_nat())\n    # BernoulliNP\n    #     log_odds=Jax Array (3,) float32\n    #            -0.8473     -0.4055      0.8473\n\n    # Print optimized natural parameters as expectation parameters.\n    print(optimized_q.to_exp())\n    # BernoulliEP\n    #     probability=Jax Array (3,) float32\n    #             0.3007      0.4002      0.6993\n\nContribution guidelines\n=======================\n\nContributions are welcome!\n\nIt's not hard to add a new distribution.  The steps are:\n\n- Create an issue for the new distribution.\n\n- Solve for or research the equations needed to fill the blanks in the overview pdf, and put them in\n  the issue.  I'll add them to the pdf for you.\n\n- Implement the natural and expectation parametrizations, either:\n\n  - directly like in the Bernoulli distribution, or\n  - as a transformation of an existing exponential family like the Rayleigh distribution.\n\n- Implement the conversion from the expectation to the natural parametrization.  If this has no\n  analytical solution, then there's a mixin that implements a numerical solution.  This can be seen\n  in the Dirichlet distribution.\n\n- Add the new distribution to the tests by adding it to `create_info <https://github.com/NeilGirdhar/efax/blob/master/tests/create_info.py>`_.)\n\nImplementation should respect PEP8.\nThe tests can be run using :bash:`pytest . -n auto`.\nThere are a few tools to clean and check the source:\n\n- :bash:`isort .`\n\n- :bash:`pylint efax`\n\n- :bash:`flake8 efax`\n\n- :bash:`mypy efax`\n",
+    'long_description': "=================================\nEFAX: Exponential Families in JAX\n=================================\n.. image:: https://badge.fury.io/py/efax.svg\n    :target: https://badge.fury.io/py/efax\n\n.. role:: bash(code)\n    :language: bash\n\n.. role:: python(code)\n   :language: python\n\nThis library provides a set of tools for working with *exponential family distributions* in the\ndifferential programming library `JAX <https://github.com/google/jax/>`_.\n\nThe *exponential families* are an important class of probability distributions that include the\nnormal, gamma, beta, exponential, Poisson, binomial, and Bernoulli distributions.\nFor an explanation of the fundamental ideas behind this library, see our `overview on exponential\nfamilies <https://github.com/NeilGirdhar/efax/blob/master/expfam.pdf>`_.\n\nThe main motivation for using EFAX over a library like tensorflow-probability or the basic functions\nin JAX is that EFAX provides the two most important parametrizations for each exponential family—the\nnatural and expectation parametrizations—and a uniform interface to efficient implementations of the\nmain functions used in machine learning.  An example of why this matters is that the most efficient\nway to implement cross entropy between X and Y relies on X being in the expectation parametrization\nand Y in the natural parametrization.\n\nFramework\n=========\nRepresentation\n--------------\nEFAX has a single base class for its objects: :python:`Parametrization` whose type encodes the\ndistribution family.\n\nEach parametrization object has a shape, and so it can store any number of distributions.\nOperations on these objects are vectorized.\nThis is unlike SciPy where each distribution is represented by a single object, and so a thousand\ndistributions need a thousand objects, and corresponding calls to functions that operate on them.\n\nAll parametrization objects are dataclasses using :python:`tjax.dataclass`.  These dataclasses are\na modification of Python's dataclasses to support JAX's “PyTree” type registration.\n\nEach of the fields of a parametrization object stores a parameter over a specified support.\nSome parameters are marked as “fixed”, which means that they are fixed with respect to the\nexponential family.  An example of a fixed parameter is the failure number of the negative binomial\ndistribution.\n\nFor example:\n\n.. code:: python\n\n    @dataclass\n    class MultivariateNormalNP(NaturalParametrization['MultivariateNormalEP']):\n        mean_times_precision: RealArray = distribution_parameter(VectorSupport())\n        negative_half_precision: RealArray = distribution_parameter(SymmetricMatrixSupport())\n\nIn this case, we see that there are two natural parameters for the multivariate normal distribution.\nObjects of this type can hold any number of distributions:  if such an object :python:`x` has shape\n:python:`s`, then the shape of\n:python:`x.mean_times_precision` is :python:`(*s, n)` and the shape of\n:python:`x.negative_half_precision` is :python:`(*s, n, n)`.\n\nParametrizations\n----------------\nEach exponential family distribution has two special parametrizations: the natural and the\nexpectation parametrization.  (These are described in the overview pdf.)\nConsequently, every distribution has at least two base classes, one inheriting from\n:python:`NaturalParametrization` and one from :python:`ExpectationParametrization`.\n\nThe motivation for the natural parametrization is combining and scaling independent predictive\nevidence.  In the natural parametrization, these operations correspond to scaling and addition.\n\nThe motivation for the expectation parametrization is combining independent observations into the\nmaximum likelihood distribution that could have produced them.  In the expectation parametrization,\nthis is an expected value.\n\nEFAX provides conversions between the two parametrizations through the\n:python:`NaturalParametrization.to_exp` and :python:`ExpectationParametrization.to_nat` methods.\n\nImportant methods\n-----------------\nEFAX aims to provide the main methods used in machine learning.\n\nEvery :python:`Parametrization` has methods to flatten and unflatten the parameters into a single\narray: :python:`flattened` and :python:`unflattened`.  Typically, array-valued signals in a machine\nlearning model would be unflattened into a distribution object, operated on, and then flattened\nbefore being sent back to the model.  Flattening is careful with distributions with symmetric (or Hermitian) matrix-valued parameters.  It only stores the upper triangular elements.\n\nEvery :python:`NaturalParametrization` has methods:\n\n- :python:`sufficient_statistics` to produce the sufficient statistics given an observation (used in\n  maximum likelihood estimation),\n- :python:`pdf`, which is the density or mass function,\n- :python:`fisher_information`, which is the Fisher information matrix, and\n- :python:`entropy`, which is the Shannon entropy.\n\nEvery :python:`ExpectationParametrization` has methods:\n\n- :python:`cross_entropy` that is an efficient cross entropy armed with a numerically optimized\n  custom JAX gradient.  This is possible because the gradient of the cross entropy is the difference\n  of expectation parameters plus the expected carrier measure.\n\nNumerical optimization\n----------------------\nBecause of the nature of the log-normalizer and carrier measure, some methods for some distributions\nrequire numerical optimization.  These are the conversion from expectation parameters to natural\nones, the entropy, and the cross entropy.\n\nDistributions\n=============\nEFAX supports the following distributions:\n\n- normal:\n\n  - univariate real\n  - univariate complex\n  - multivariate real:\n\n    - with fixed unit variance\n    - with fixed variance\n    - with isotropic variance\n    - with diagonal variance\n    - with general variance\n\n  - multivariate complex:\n\n    - with unit variance and zero pseudo-variance\n    - circularly symmetric\n\n- on a finite set:\n\n  - Bernoulli\n  - multinomial\n\n- on the nonnegative integers:\n\n  - geometric\n  - logarithmic\n  - negative binomial\n  - Poisson\n\n- on the positive reals:\n\n  - chi\n  - chi-square\n  - exponential\n  - gamma\n  - Rayleigh\n  - Weibull\n\n- on the simplex:\n\n  - beta\n  - Dirichlet\n  - generalized Dirichlet\n\n- on the n-sphere:\n\n  - von Mises-Fisher\n\nUsage\n=====\nBasic usage\n-----------\nA basic use of the two parametrizations:\n\n.. code:: python\n\n    from jax import numpy as jnp\n\n    from efax import BernoulliEP, BernoulliNP\n\n    # p is the expectation parameters of three Bernoulli distributions having probabilities 0.4, 0.5,\n    # and 0.6.\n    p = BernoulliEP(jnp.array([0.4, 0.5, 0.6]))\n\n    # q is the natural parameters of three Bernoulli distributions having log-odds 0, which is\n    # probability 0.5.\n    q = BernoulliNP(jnp.zeros(3))\n\n    print(p.cross_entropy(q))\n    # [0.6931472 0.6931472 0.6931472]\n\n    # q2 is natural parameters of Bernoulli distributions having a probability of 0.3.\n    p2 = BernoulliEP(0.3 * jnp.ones(3))\n    q2 = p2.to_nat()\n\n    print(p.cross_entropy(q2))\n    # [0.6955941  0.78032386 0.86505365]\n    # A Bernoulli distribution with probability 0.3 predicts a Bernoulli observation with probability\n    # 0.4 better than the other observations.\n\nOptimization\n------------\nUsing the cross entropy to iteratively optimize a prediction is simple:\n\n.. code:: python\n\n    import jax.numpy as jnp\n    from jax import grad, jit, lax\n    from jax.tree_util import tree_map, tree_reduce\n    from tjax import BooleanNumeric, RealArray, RealNumeric\n\n    from efax import BernoulliEP, BernoulliNP\n\n\n    def cross_entropy_loss(p: BernoulliEP, q: BernoulliNP) -> RealNumeric:\n        return jnp.sum(p.cross_entropy(q))\n\n\n    gce = jit(grad(cross_entropy_loss, 1))\n\n\n    def apply(x: RealArray, x_bar: RealArray) -> RealArray:\n        return x - 1e-4 * x_bar\n\n\n    def body_fun(q: BernoulliNP) -> BernoulliNP:\n        q_bar = gce(some_p, q)\n        return tree_map(apply, q, q_bar)\n\n\n    def cond_fun(q: BernoulliNP) -> BooleanNumeric:\n        q_bar = gce(some_p, q)\n        total = tree_reduce(jnp.sum,\n                            tree_map(lambda x: jnp.sum(jnp.square(x)), q_bar))\n        return total > 1e-6\n\n\n    # some_p are expectation parameters of a Bernoulli distribution corresponding\n    # to probabilities 0.3, 0.4, and 0.7.\n    some_p = BernoulliEP(jnp.array([0.3, 0.4, 0.7]))\n\n    # some_q are natural parameters of a Bernoulli distribution corresponding to\n    # log-odds 0, which is probability 0.5.\n    some_q = BernoulliNP(jnp.zeros(3))\n\n    # Optimize the predictive distribution iteratively, and output the natural parameters of the\n    # prediction.\n    optimized_q = lax.while_loop(cond_fun, body_fun, some_q)\n    print(optimized_q)\n    # BernoulliNP\n    #     log_odds=Jax Array (3,) float32\n    #            -0.8440     -0.4047      0.8440\n\n    # Compare with the true value.\n    print(some_p.to_nat())\n    # BernoulliNP\n    #     log_odds=Jax Array (3,) float32\n    #            -0.8473     -0.4055      0.8473\n\n    # Print optimized natural parameters as expectation parameters.\n    print(optimized_q.to_exp())\n    # BernoulliEP\n    #     probability=Jax Array (3,) float32\n    #             0.3007      0.4002      0.6993\n\nContribution guidelines\n=======================\n\nContributions are welcome!\n\nIt's not hard to add a new distribution.  The steps are:\n\n- Create an issue for the new distribution.\n\n- Solve for or research the equations needed to fill the blanks in the overview pdf, and put them in\n  the issue.  I'll add them to the pdf for you.\n\n- Implement the natural and expectation parametrizations, either:\n\n  - directly like in the Bernoulli distribution, or\n  - as a transformation of an existing exponential family like the Rayleigh distribution.\n\n- Implement the conversion from the expectation to the natural parametrization.  If this has no\n  analytical solution, then there's a mixin that implements a numerical solution.  This can be seen\n  in the Dirichlet distribution.\n\n- Add the new distribution to the tests by adding it to `create_info <https://github.com/NeilGirdhar/efax/blob/master/tests/create_info.py>`_.)\n\nImplementation should respect PEP8.\nThe tests can be run using :bash:`pytest . -n auto`.\nThere are a few tools to clean and check the source:\n\n- :bash:`isort .`\n- :bash:`mypy .`\n- :bash:`pylint efax tests`\n- :bash:`pflake8 .`\n",
     'author': 'Neil Girdhar',
     'author_email': 'mistersheik@gmail.com',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'https://github.com/NeilGirdhar/efax',
     'packages': packages,
     'package_data': package_data,
```

### Comparing `efax-1.9.0/PKG-INFO` & `efax-1.9.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: efax
-Version: 1.9.0
+Version: 1.9.1
 Summary: Exponential families for JAX
 Home-page: https://github.com/NeilGirdhar/efax
 License: MIT
 Author: Neil Girdhar
 Author-email: mistersheik@gmail.com
 Requires-Python: >=3.8,<3.11
 Classifier: Development Status :: 5 - Production/Stable
@@ -312,14 +312,11 @@
 - Add the new distribution to the tests by adding it to `create_info <https://github.com/NeilGirdhar/efax/blob/master/tests/create_info.py>`_.)
 
 Implementation should respect PEP8.
 The tests can be run using :bash:`pytest . -n auto`.
 There are a few tools to clean and check the source:
 
 - :bash:`isort .`
-
-- :bash:`pylint efax`
-
-- :bash:`flake8 efax`
-
-- :bash:`mypy efax`
+- :bash:`mypy .`
+- :bash:`pylint efax tests`
+- :bash:`pflake8 .`
```

