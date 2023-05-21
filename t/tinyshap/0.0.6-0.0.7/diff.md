# Comparing `tmp/tinyshap-0.0.6.tar.gz` & `tmp/tinyshap-0.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tinyshap-0.0.6.tar", last modified: Sat May 20 20:00:48 2023, max compression
+gzip compressed data, was "tinyshap-0.0.7.tar", last modified: Sun May 21 15:51:46 2023, max compression
```

## Comparing `tinyshap-0.0.6.tar` & `tinyshap-0.0.7.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxrwxrwx   0 tsitsimis  (1000) tsitsimis  (1000)        0 2023-05-20 20:00:50.054555 tinyshap-0.0.6/
--rwxrwxrwx   0 tsitsimis  (1000) tsitsimis  (1000)     1089 2023-04-29 16:41:09.000000 tinyshap-0.0.6/LICENCE
--rwxrwxrwx   0 tsitsimis  (1000) tsitsimis  (1000)     1791 2023-05-20 20:00:50.054555 tinyshap-0.0.6/PKG-INFO
--rwxrwxrwx   0 tsitsimis  (1000) tsitsimis  (1000)      946 2023-05-18 16:22:52.000000 tinyshap-0.0.6/README.md
--rwxrwxrwx   0 tsitsimis  (1000) tsitsimis  (1000)     1144 2023-05-20 19:59:07.000000 tinyshap-0.0.6/pyproject.toml
--rwxrwxrwx   0 tsitsimis  (1000) tsitsimis  (1000)       38 2023-05-20 20:00:50.054555 tinyshap-0.0.6/setup.cfg
-drwxrwxrwx   0 tsitsimis  (1000) tsitsimis  (1000)        0 2023-05-20 20:00:49.679554 tinyshap-0.0.6/src/
-drwxrwxrwx   0 tsitsimis  (1000) tsitsimis  (1000)        0 2023-05-20 20:00:49.820179 tinyshap-0.0.6/src/tinyshap/
--rwxrwxrwx   0 tsitsimis  (1000) tsitsimis  (1000)       46 2023-04-24 17:25:47.000000 tinyshap-0.0.6/src/tinyshap/__init__.py
--rwxrwxrwx   0 tsitsimis  (1000) tsitsimis  (1000)     4036 2023-05-20 19:59:07.000000 tinyshap-0.0.6/src/tinyshap/explainer.py
-drwxrwxrwx   0 tsitsimis  (1000) tsitsimis  (1000)        0 2023-05-20 20:00:49.992053 tinyshap-0.0.6/src/tinyshap.egg-info/
--rwxrwxrwx   0 tsitsimis  (1000) tsitsimis  (1000)     1791 2023-05-20 20:00:49.000000 tinyshap-0.0.6/src/tinyshap.egg-info/PKG-INFO
--rwxrwxrwx   0 tsitsimis  (1000) tsitsimis  (1000)      286 2023-05-20 20:00:49.000000 tinyshap-0.0.6/src/tinyshap.egg-info/SOURCES.txt
--rwxrwxrwx   0 tsitsimis  (1000) tsitsimis  (1000)        1 2023-05-20 20:00:49.000000 tinyshap-0.0.6/src/tinyshap.egg-info/dependency_links.txt
--rwxrwxrwx   0 tsitsimis  (1000) tsitsimis  (1000)       55 2023-05-20 20:00:49.000000 tinyshap-0.0.6/src/tinyshap.egg-info/requires.txt
--rwxrwxrwx   0 tsitsimis  (1000) tsitsimis  (1000)        9 2023-05-20 20:00:49.000000 tinyshap-0.0.6/src/tinyshap.egg-info/top_level.txt
-drwxrwxrwx   0 tsitsimis  (1000) tsitsimis  (1000)        0 2023-05-20 20:00:50.023304 tinyshap-0.0.6/tests/
--rwxrwxrwx   0 tsitsimis  (1000) tsitsimis  (1000)     2634 2023-05-20 19:59:07.000000 tinyshap-0.0.6/tests/test_explainer.py
+drwxrwxrwx   0 tsitsimis  (1000) tsitsimis  (1000)        0 2023-05-21 15:51:46.163189 tinyshap-0.0.7/
+-rwxrwxrwx   0 tsitsimis  (1000) tsitsimis  (1000)     1089 2023-04-29 16:41:09.000000 tinyshap-0.0.7/LICENCE
+-rwxrwxrwx   0 tsitsimis  (1000) tsitsimis  (1000)     2154 2023-05-21 15:51:46.156188 tinyshap-0.0.7/PKG-INFO
+-rwxrwxrwx   0 tsitsimis  (1000) tsitsimis  (1000)     1316 2023-05-20 20:04:45.000000 tinyshap-0.0.7/README.md
+-rwxrwxrwx   0 tsitsimis  (1000) tsitsimis  (1000)     1144 2023-05-21 15:50:21.000000 tinyshap-0.0.7/pyproject.toml
+-rwxrwxrwx   0 tsitsimis  (1000) tsitsimis  (1000)       38 2023-05-21 15:51:46.168192 tinyshap-0.0.7/setup.cfg
+drwxrwxrwx   0 tsitsimis  (1000) tsitsimis  (1000)        0 2023-05-21 15:51:44.931242 tinyshap-0.0.7/src/
+drwxrwxrwx   0 tsitsimis  (1000) tsitsimis  (1000)        0 2023-05-21 15:51:45.611373 tinyshap-0.0.7/src/tinyshap/
+-rwxrwxrwx   0 tsitsimis  (1000) tsitsimis  (1000)       46 2023-04-24 17:25:47.000000 tinyshap-0.0.7/src/tinyshap/__init__.py
+-rwxrwxrwx   0 tsitsimis  (1000) tsitsimis  (1000)     4034 2023-05-21 15:47:22.000000 tinyshap-0.0.7/src/tinyshap/explainer.py
+drwxrwxrwx   0 tsitsimis  (1000) tsitsimis  (1000)        0 2023-05-21 15:51:46.000581 tinyshap-0.0.7/src/tinyshap.egg-info/
+-rwxrwxrwx   0 tsitsimis  (1000) tsitsimis  (1000)     2154 2023-05-21 15:51:44.000000 tinyshap-0.0.7/src/tinyshap.egg-info/PKG-INFO
+-rwxrwxrwx   0 tsitsimis  (1000) tsitsimis  (1000)      286 2023-05-21 15:51:44.000000 tinyshap-0.0.7/src/tinyshap.egg-info/SOURCES.txt
+-rwxrwxrwx   0 tsitsimis  (1000) tsitsimis  (1000)        1 2023-05-21 15:51:44.000000 tinyshap-0.0.7/src/tinyshap.egg-info/dependency_links.txt
+-rwxrwxrwx   0 tsitsimis  (1000) tsitsimis  (1000)       55 2023-05-21 15:51:44.000000 tinyshap-0.0.7/src/tinyshap.egg-info/requires.txt
+-rwxrwxrwx   0 tsitsimis  (1000) tsitsimis  (1000)        9 2023-05-21 15:51:44.000000 tinyshap-0.0.7/src/tinyshap.egg-info/top_level.txt
+drwxrwxrwx   0 tsitsimis  (1000) tsitsimis  (1000)        0 2023-05-21 15:51:46.058574 tinyshap-0.0.7/tests/
+-rwxrwxrwx   0 tsitsimis  (1000) tsitsimis  (1000)     2634 2023-05-20 19:59:07.000000 tinyshap-0.0.7/tests/test_explainer.py
```

### Comparing `tinyshap-0.0.6/LICENCE` & `tinyshap-0.0.7/LICENCE`

 * *Files identical despite different names*

### Comparing `tinyshap-0.0.6/README.md` & `tinyshap-0.0.7/README.md`

 * *Files 19% similar despite different names*

```diff
@@ -1,60 +1,83 @@
-00000000: 2320 7469 6e79 7368 6170 0d0a 215b 5d28  # tinyshap..![](
-00000010: 2e2f 6173 7365 7473 2f64 656d 6f2d 6465  ./assets/demo-de
-00000020: 7065 6e64 656e 6379 2d70 6c6f 742e 706e  pendency-plot.pn
-00000030: 6729 0d0a 0d0a 4120 6d69 6e69 6d61 6c20  g)....A minimal 
-00000040: 696d 706c 656d 656e 7461 7469 6f6e 206f  implementation o
-00000050: 6620 7468 6520 5348 4150 2061 6c67 6f72  f the SHAP algor
-00000060: 6974 686d 2075 7369 6e67 2074 6865 204b  ithm using the K
-00000070: 6572 6e65 6c53 4841 5020 6d65 7468 6f64  ernelSHAP method
-00000080: 2e20 496e 206c 6573 7320 7468 656e 2031  . In less then 1
-00000090: 3030 206c 696e 6573 206f 6620 636f 6465  00 lines of code
-000000a0: 2c20 7468 6973 2072 6570 6f20 7365 7276  , this repo serv
-000000b0: 6573 2061 7320 616e 2065 6475 6361 7469  es as an educati
-000000c0: 6f6e 616c 2072 6573 6f75 7263 6520 746f  onal resource to
-000000d0: 2075 6e64 6572 7374 616e 6420 686f 7720   understand how 
-000000e0: 5348 4150 2077 6f72 6b73 2077 6974 686f  SHAP works witho
-000000f0: 7574 2061 6c6c 2074 6865 2063 6f6d 706c  ut all the compl
-00000100: 6578 6974 6965 7320 6f66 2061 2070 726f  exities of a pro
-00000110: 6475 6374 696f 6e2d 6c65 7665 6c20 7061  duction-level pa
-00000120: 636b 6167 652e 0d0a 0d0a 2323 2049 6e73  ckage.....## Ins
-00000130: 7461 6c6c 6174 696f 6e0d 0a60 6060 6261  tallation..```ba
-00000140: 7368 0d0a 7069 7020 696e 7374 616c 6c20  sh..pip install 
-00000150: 7469 6e79 7368 6170 0d0a 6060 600d 0a0d  tinyshap..```...
-00000160: 0a23 2320 4578 616d 706c 6520 7573 6167  .## Example usag
-00000170: 650d 0a60 6060 7079 7468 6f6e 0d0a 6672  e..```python..fr
-00000180: 6f6d 2074 696e 7973 6861 7020 696d 706f  om tinyshap impo
-00000190: 7274 2053 4841 5045 7870 6c61 696e 6572  rt SHAPExplainer
-000001a0: 0d0a 0d0a 2320 5472 6169 6e20 6d6f 6465  ....# Train mode
-000001b0: 6c0d 0a6d 6f64 656c 203d 2047 7261 6469  l..model = Gradi
-000001c0: 656e 7442 6f6f 7374 696e 6752 6567 7265  entBoostingRegre
-000001d0: 7373 6f72 2829 0d0a 6d6f 6465 6c2e 6669  ssor()..model.fi
-000001e0: 7428 585f 7472 6169 6e2c 2079 5f74 7261  t(X_train, y_tra
-000001f0: 696e 290d 0a0d 0a23 2045 7870 6c61 696e  in)....# Explain
-00000200: 2070 7265 6469 6374 696f 6e73 0d0a 6578   predictions..ex
-00000210: 706c 6169 6e65 7220 3d20 5348 4150 4578  plainer = SHAPEx
-00000220: 706c 6169 6e65 7228 6d6f 6465 6c2e 7072  plainer(model.pr
-00000230: 6564 6963 742c 2058 3d58 5f74 7261 696e  edict, X=X_train
-00000240: 2e6d 6561 6e28 292e 746f 5f66 7261 6d65  .mean().to_frame
-00000250: 2829 2e54 290d 0a63 6f6e 7472 6962 7574  ().T)..contribut
-00000260: 696f 6e73 203d 2065 7870 6c61 696e 6572  ions = explainer
-00000270: 2e73 6861 705f 7661 6c75 6573 2858 290d  .shap_values(X).
-00000280: 0a60 6060 0d0a 0d0a 5365 6520 636f 6d70  .```....See comp
-00000290: 6c65 7465 205b 6e6f 7465 626f 6f6b 5d28  lete [notebook](
-000002a0: 2e2f 6e6f 7465 626f 6f6b 732f 6465 6d6f  ./notebooks/demo
-000002b0: 2e69 7079 6e62 290d 0a0d 0a23 2320 5265  .ipynb)....## Re
-000002c0: 736f 7572 6365 730d 0a2a 205b 4120 556e  sources..* [A Un
-000002d0: 6966 6965 6420 4170 7072 6f61 6368 2074  ified Approach t
-000002e0: 6f20 496e 7465 7270 7265 7469 6e67 204d  o Interpreting M
-000002f0: 6f64 656c 2050 7265 6469 6374 696f 6e73  odel Predictions
-00000300: 2028 6172 5869 7629 5d28 6874 7470 733a   (arXiv)](https:
-00000310: 2f2f 6172 7869 762e 6f72 672f 6162 732f  //arxiv.org/abs/
-00000320: 3137 3035 2e30 3738 3734 290d 0a2a 205b  1705.07874)..* [
-00000330: 496e 7465 7270 7265 7461 626c 6520 4d61  Interpretable Ma
-00000340: 6368 696e 6520 4c65 6172 6e69 6e67 5d28  chine Learning](
-00000350: 6874 7470 733a 2f2f 6368 7269 7374 6f70  https://christop
-00000360: 686d 2e67 6974 6875 622e 696f 2f69 6e74  hm.github.io/int
-00000370: 6572 7072 6574 6162 6c65 2d6d 6c2d 626f  erpretable-ml-bo
-00000380: 6f6b 2f73 6861 702e 6874 6d6c 236b 6572  ok/shap.html#ker
-00000390: 6e65 6c73 6861 7029 0d0a 0d0a 0d0a 2323  nelshap)......##
-000003a0: 204c 6963 656e 6365 0d0a 4d49 540d 0a20   Licence..MIT.. 
-000003b0: 0d0a                                     ..
+00000000: 2320 7469 6e79 7368 6170 0d0a 3c61 2068  # tinyshap..<a h
+00000010: 7265 663d 2268 7474 7073 3a2f 2f70 7970  ref="https://pyp
+00000020: 692e 6f72 672f 7072 6f6a 6563 742f 7469  i.org/project/ti
+00000030: 6e79 7368 6170 2220 7461 7267 6574 3d22  nyshap" target="
+00000040: 5f62 6c61 6e6b 223e 0d0a 2020 2020 3c69  _blank">..    <i
+00000050: 6d67 2073 7263 3d22 6874 7470 733a 2f2f  mg src="https://
+00000060: 696d 672e 7368 6965 6c64 732e 696f 2f70  img.shields.io/p
+00000070: 7970 692f 762f 7469 6e79 7368 6170 3f63  ypi/v/tinyshap?c
+00000080: 6f6c 6f72 3d25 3233 3334 4430 3538 266c  olor=%2334D058&l
+00000090: 6162 656c 3d70 7970 6925 3230 7061 636b  abel=pypi%20pack
+000000a0: 6167 6522 2061 6c74 3d22 5061 636b 6167  age" alt="Packag
+000000b0: 6520 7665 7273 696f 6e22 3e0d 0a3c 2f61  e version">..</a
+000000c0: 3e0d 0a3c 6120 6872 6566 3d22 6874 7470  >..<a href="http
+000000d0: 733a 2f2f 7079 7069 2e6f 7267 2f70 726f  s://pypi.org/pro
+000000e0: 6a65 6374 2f74 696e 7973 6861 7022 2074  ject/tinyshap" t
+000000f0: 6172 6765 743d 225f 626c 616e 6b22 3e0d  arget="_blank">.
+00000100: 0a20 2020 203c 696d 6720 7372 633d 2268  .    <img src="h
+00000110: 7474 7073 3a2f 2f69 6d67 2e73 6869 656c  ttps://img.shiel
+00000120: 6473 2e69 6f2f 7079 7069 2f70 7976 6572  ds.io/pypi/pyver
+00000130: 7369 6f6e 732f 7469 6e79 7368 6170 2e73  sions/tinyshap.s
+00000140: 7667 3f63 6f6c 6f72 3d25 3233 3334 4430  vg?color=%2334D0
+00000150: 3538 2220 616c 743d 2253 7570 706f 7274  58" alt="Support
+00000160: 6564 2050 7974 686f 6e20 7665 7273 696f  ed Python versio
+00000170: 6e73 223e 0d0a 3c2f 613e 0d0a 0d0a 215b  ns">..</a>....![
+00000180: 5d28 2e2f 6173 7365 7473 2f64 656d 6f2d  ](./assets/demo-
+00000190: 6465 7065 6e64 656e 6379 2d70 6c6f 742e  dependency-plot.
+000001a0: 706e 6729 0d0a 0d0a 4120 6d69 6e69 6d61  png)....A minima
+000001b0: 6c20 696d 706c 656d 656e 7461 7469 6f6e  l implementation
+000001c0: 206f 6620 7468 6520 5348 4150 2061 6c67   of the SHAP alg
+000001d0: 6f72 6974 686d 2075 7369 6e67 2074 6865  orithm using the
+000001e0: 204b 6572 6e65 6c53 4841 5020 6d65 7468   KernelSHAP meth
+000001f0: 6f64 2e20 496e 206c 6573 7320 7468 656e  od. In less then
+00000200: 2031 3030 206c 696e 6573 206f 6620 636f   100 lines of co
+00000210: 6465 2c20 7468 6973 2072 6570 6f20 7365  de, this repo se
+00000220: 7276 6573 2061 7320 616e 2065 6475 6361  rves as an educa
+00000230: 7469 6f6e 616c 2072 6573 6f75 7263 6520  tional resource 
+00000240: 746f 2075 6e64 6572 7374 616e 6420 686f  to understand ho
+00000250: 7720 5348 4150 2077 6f72 6b73 2077 6974  w SHAP works wit
+00000260: 686f 7574 2061 6c6c 2074 6865 2063 6f6d  hout all the com
+00000270: 706c 6578 6974 6965 7320 6f66 2061 2070  plexities of a p
+00000280: 726f 6475 6374 696f 6e2d 6c65 7665 6c20  roduction-level 
+00000290: 7061 636b 6167 652e 0d0a 0d0a 2323 2049  package.....## I
+000002a0: 6e73 7461 6c6c 6174 696f 6e0d 0a60 6060  nstallation..```
+000002b0: 6261 7368 0d0a 7069 7020 696e 7374 616c  bash..pip instal
+000002c0: 6c20 7469 6e79 7368 6170 0d0a 6060 600d  l tinyshap..```.
+000002d0: 0a0d 0a23 2320 4578 616d 706c 6520 7573  ...## Example us
+000002e0: 6167 650d 0a60 6060 7079 7468 6f6e 0d0a  age..```python..
+000002f0: 6672 6f6d 2074 696e 7973 6861 7020 696d  from tinyshap im
+00000300: 706f 7274 2053 4841 5045 7870 6c61 696e  port SHAPExplain
+00000310: 6572 0d0a 0d0a 2320 5472 6169 6e20 6d6f  er....# Train mo
+00000320: 6465 6c0d 0a6d 6f64 656c 203d 2047 7261  del..model = Gra
+00000330: 6469 656e 7442 6f6f 7374 696e 6752 6567  dientBoostingReg
+00000340: 7265 7373 6f72 2829 0d0a 6d6f 6465 6c2e  ressor()..model.
+00000350: 6669 7428 585f 7472 6169 6e2c 2079 5f74  fit(X_train, y_t
+00000360: 7261 696e 290d 0a0d 0a23 2045 7870 6c61  rain)....# Expla
+00000370: 696e 2070 7265 6469 6374 696f 6e73 0d0a  in predictions..
+00000380: 6578 706c 6169 6e65 7220 3d20 5348 4150  explainer = SHAP
+00000390: 4578 706c 6169 6e65 7228 6d6f 6465 6c2e  Explainer(model.
+000003a0: 7072 6564 6963 742c 2058 3d58 5f74 7261  predict, X=X_tra
+000003b0: 696e 2e6d 6561 6e28 292e 746f 5f66 7261  in.mean().to_fra
+000003c0: 6d65 2829 2e54 290d 0a63 6f6e 7472 6962  me().T)..contrib
+000003d0: 7574 696f 6e73 203d 2065 7870 6c61 696e  utions = explain
+000003e0: 6572 2e73 6861 705f 7661 6c75 6573 2858  er.shap_values(X
+000003f0: 290d 0a60 6060 0d0a 0d0a 5365 6520 636f  )..```....See co
+00000400: 6d70 6c65 7465 205b 6e6f 7465 626f 6f6b  mplete [notebook
+00000410: 5d28 2e2f 6e6f 7465 626f 6f6b 732f 6465  ](./notebooks/de
+00000420: 6d6f 2e69 7079 6e62 290d 0a0d 0a23 2320  mo.ipynb)....## 
+00000430: 5265 736f 7572 6365 730d 0a2a 205b 4120  Resources..* [A 
+00000440: 556e 6966 6965 6420 4170 7072 6f61 6368  Unified Approach
+00000450: 2074 6f20 496e 7465 7270 7265 7469 6e67   to Interpreting
+00000460: 204d 6f64 656c 2050 7265 6469 6374 696f   Model Predictio
+00000470: 6e73 2028 6172 5869 7629 5d28 6874 7470  ns (arXiv)](http
+00000480: 733a 2f2f 6172 7869 762e 6f72 672f 6162  s://arxiv.org/ab
+00000490: 732f 3137 3035 2e30 3738 3734 290d 0a2a  s/1705.07874)..*
+000004a0: 205b 496e 7465 7270 7265 7461 626c 6520   [Interpretable 
+000004b0: 4d61 6368 696e 6520 4c65 6172 6e69 6e67  Machine Learning
+000004c0: 5d28 6874 7470 733a 2f2f 6368 7269 7374  ](https://christ
+000004d0: 6f70 686d 2e67 6974 6875 622e 696f 2f69  ophm.github.io/i
+000004e0: 6e74 6572 7072 6574 6162 6c65 2d6d 6c2d  nterpretable-ml-
+000004f0: 626f 6f6b 2f73 6861 702e 6874 6d6c 236b  book/shap.html#k
+00000500: 6572 6e65 6c73 6861 7029 0d0a 0d0a 0d0a  ernelshap)......
+00000510: 2323 204c 6963 656e 6365 0d0a 4d49 540d  ## Licence..MIT.
+00000520: 0a20 0d0a                                . ..
```

### Comparing `tinyshap-0.0.6/pyproject.toml` & `tinyshap-0.0.7/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = 'tinyshap'
-version = '0.0.6'
+version = '0.0.7'
 description = 'Minimal implementation of approximate Kernel SHAP algorithm'
 readme = 'README.md'
 authors = [
   { name = 'Theodore Tsitsimis', email='th.tsitsimis@gmail.com' },
 ]
 license = {file = 'LICENSE'}
 requires-python = '>=3.7'
 dependencies = [
   "pandas>=1.4.0",
   "scikit-learn>=1.1.1",
-  "constrainedlr>=0.0.8"
+  "constrainedlr>=0.1.0"
 ]
 classifiers = [
     'Development Status :: 3 - Alpha',
     'Intended Audience :: Developers',
     'License :: OSI Approved :: MIT License',
     'Operating System :: OS Independent',
     'Programming Language :: Python',
```

### Comparing `tinyshap-0.0.6/src/tinyshap/explainer.py` & `tinyshap-0.0.7/src/tinyshap/explainer.py`

 * *Files 2% similar despite different names*

```diff
@@ -80,15 +80,15 @@
 
         coalitions = self._generate_coalitions()
         feature_values = self._get_feature_values(coalitions, x_test)
         predictions = self.model(feature_values)
         weights = self._get_coalition_weights(coalitions)
 
         lr = ConstrainedLinearRegression(fit_intercept=True)
-        lr.fit(coalitions, predictions, sample_weight=weights, features_sum_constraint_equal=model_prediction)
+        lr.fit(coalitions, predictions, sample_weight=weights, coefficients_sum_constraint=model_prediction)
         shap_values = pd.Series(data=lr.coef_, index=self.X.columns)
         shap_values["avg_prediction"] = lr.intercept_
         return shap_values
 
     def shap_values(self, X: pd.DataFrame) -> pd.DataFrame:
         """
         Calculates SHAP values of multiple samples in `X`
```

### Comparing `tinyshap-0.0.6/tests/test_explainer.py` & `tinyshap-0.0.7/tests/test_explainer.py`

 * *Files identical despite different names*

