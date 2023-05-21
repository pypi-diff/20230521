# Comparing `tmp/copul-0.0.1.tar.gz` & `tmp/copul-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "copul-0.0.1.tar", last modified: Fri May 19 12:51:15 2023, max compression
+gzip compressed data, was "copul-0.0.2.tar", last modified: Sun May 21 19:39:29 2023, max compression
```

## Comparing `copul-0.0.1.tar` & `copul-0.0.2.tar`

### file list

```diff
@@ -1,69 +1,65 @@
-drwxrwxrwx   0        0        0        0 2023-05-19 12:51:15.229066 copul-0.0.1/
--rw-rw-rw-   0        0        0     1091 2023-03-29 13:31:36.000000 copul-0.0.1/LICENSE
--rw-rw-rw-   0        0        0       30 2023-03-30 13:31:03.000000 copul-0.0.1/MANIFEST.in
--rw-rw-rw-   0        0        0     1099 2023-05-19 12:51:15.230067 copul-0.0.1/PKG-INFO
--rw-rw-rw-   0        0        0      560 2023-05-19 10:23:29.000000 copul-0.0.1/README.md
-drwxrwxrwx   0        0        0        0 2023-05-19 12:51:15.120355 copul-0.0.1/copul/
--rw-rw-rw-   0        0        0     1967 2023-05-19 10:16:22.000000 copul-0.0.1/copul/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-19 12:51:15.136349 copul-0.0.1/copul/calculations/
--rw-rw-rw-   0        0        0        0 2023-03-09 12:10:27.000000 copul-0.0.1/copul/calculations/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-19 12:51:15.139325 copul-0.0.1/copul/calculations/copulas/
--rw-rw-rw-   0        0        0        0 2023-03-09 12:04:48.000000 copul-0.0.1/copul/calculations/copulas/__init__.py
--rw-rw-rw-   0        0        0     1237 2023-05-19 09:32:40.000000 copul-0.0.1/copul/calculations/copulas/abstract_copula.py
-drwxrwxrwx   0        0        0        0 2023-05-19 12:51:15.142297 copul-0.0.1/copul/calculations/copulas/families/
--rw-rw-rw-   0        0        0        0 2023-01-26 10:54:46.000000 copul-0.0.1/copul/calculations/copulas/families/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-19 12:51:15.195155 copul-0.0.1/copul/calculations/copulas/families/archimedean/
--rw-rw-rw-   0        0        0     4595 2023-05-19 12:40:26.000000 copul-0.0.1/copul/calculations/copulas/families/archimedean/__init__.py
--rw-rw-rw-   0        0        0      394 2023-05-19 10:13:51.000000 copul-0.0.1/copul/calculations/copulas/families/archimedean/ali_mikhail_hak.py
--rw-rw-rw-   0        0        0     4802 2023-05-19 09:32:40.000000 copul-0.0.1/copul/calculations/copulas/families/archimedean/archimedean_copula.py
--rw-rw-rw-   0        0        0      345 2023-03-30 13:31:03.000000 copul-0.0.1/copul/calculations/copulas/families/archimedean/clayton.py
--rw-rw-rw-   0        0        0     5288 2023-05-19 12:40:26.000000 copul-0.0.1/copul/calculations/copulas/families/archimedean/derivatives_overview_constructor.py
--rw-rw-rw-   0        0        0      378 2023-03-30 13:31:03.000000 copul-0.0.1/copul/calculations/copulas/families/archimedean/frank.py
--rw-rw-rw-   0        0        0      351 2023-03-30 13:31:03.000000 copul-0.0.1/copul/calculations/copulas/families/archimedean/genest_ghoudi.py
--rw-rw-rw-   0        0        0      329 2023-03-30 13:31:03.000000 copul-0.0.1/copul/calculations/copulas/families/archimedean/gumbell_barnett.py
--rw-rw-rw-   0        0        0      344 2023-03-30 13:31:03.000000 copul-0.0.1/copul/calculations/copulas/families/archimedean/gumbell_hougaard.py
--rw-rw-rw-   0        0        0      340 2023-03-30 13:31:03.000000 copul-0.0.1/copul/calculations/copulas/families/archimedean/joe.py
--rw-rw-rw-   0        0        0      320 2023-03-30 13:31:03.000000 copul-0.0.1/copul/calculations/copulas/families/archimedean/nelsen10.py
--rw-rw-rw-   0        0        0      315 2023-03-30 13:31:03.000000 copul-0.0.1/copul/calculations/copulas/families/archimedean/nelsen11.py
--rw-rw-rw-   0        0        0      414 2023-05-19 09:38:15.000000 copul-0.0.1/copul/calculations/copulas/families/archimedean/nelsen12.py
--rw-rw-rw-   0        0        0      343 2023-03-30 13:31:03.000000 copul-0.0.1/copul/calculations/copulas/families/archimedean/nelsen13.py
--rw-rw-rw-   0        0        0      442 2023-05-19 09:38:15.000000 copul-0.0.1/copul/calculations/copulas/families/archimedean/nelsen14.py
--rw-rw-rw-   0        0        0      816 2023-05-19 09:38:15.000000 copul-0.0.1/copul/calculations/copulas/families/archimedean/nelsen16.py
--rw-rw-rw-   0        0        0     2157 2023-05-19 09:38:15.000000 copul-0.0.1/copul/calculations/copulas/families/archimedean/nelsen17.py
--rw-rw-rw-   0        0        0      339 2023-03-30 13:31:03.000000 copul-0.0.1/copul/calculations/copulas/families/archimedean/nelsen18.py
--rw-rw-rw-   0        0        0      354 2023-03-30 13:31:03.000000 copul-0.0.1/copul/calculations/copulas/families/archimedean/nelsen19.py
--rw-rw-rw-   0        0        0      417 2023-05-19 09:38:15.000000 copul-0.0.1/copul/calculations/copulas/families/archimedean/nelsen2.py
--rw-rw-rw-   0        0        0      351 2023-03-30 13:31:03.000000 copul-0.0.1/copul/calculations/copulas/families/archimedean/nelsen20.py
--rw-rw-rw-   0        0        0      357 2023-03-30 13:31:03.000000 copul-0.0.1/copul/calculations/copulas/families/archimedean/nelsen21.py
--rw-rw-rw-   0        0        0      398 2023-05-19 09:38:15.000000 copul-0.0.1/copul/calculations/copulas/families/archimedean/nelsen22.py
--rw-rw-rw-   0        0        0      323 2023-03-30 13:31:03.000000 copul-0.0.1/copul/calculations/copulas/families/archimedean/nelsen7.py
--rw-rw-rw-   0        0        0      346 2023-03-30 13:31:03.000000 copul-0.0.1/copul/calculations/copulas/families/archimedean/nelsen8.py
-drwxrwxrwx   0        0        0        0 2023-05-19 12:51:15.217098 copul-0.0.1/copul/calculations/copulas/families/extreme_value/
--rw-rw-rw-   0        0        0        0 2023-03-08 12:27:47.000000 copul-0.0.1/copul/calculations/copulas/families/extreme_value/__init__.py
--rw-rw-rw-   0        0        0      671 2023-03-30 13:31:03.000000 copul-0.0.1/copul/calculations/copulas/families/extreme_value/bb5.py
--rw-rw-rw-   0        0        0     6098 2023-05-19 10:24:09.000000 copul-0.0.1/copul/calculations/copulas/families/extreme_value/extreme_value_copula.py
--rw-rw-rw-   0        0        0      640 2023-05-19 10:25:51.000000 copul-0.0.1/copul/calculations/copulas/families/extreme_value/galambos.py
--rw-rw-rw-   0        0        0      462 2023-05-19 09:11:02.000000 copul-0.0.1/copul/calculations/copulas/families/extreme_value/gumbel.py
--rw-rw-rw-   0        0        0      792 2023-03-30 13:31:03.000000 copul-0.0.1/copul/calculations/copulas/families/extreme_value/huesler_reiss.py
--rw-rw-rw-   0        0        0      888 2023-03-30 13:31:03.000000 copul-0.0.1/copul/calculations/copulas/families/extreme_value/joe.py
--rw-rw-rw-   0        0        0      548 2023-03-30 13:31:03.000000 copul-0.0.1/copul/calculations/copulas/families/extreme_value/marshall_olkin.py
--rw-rw-rw-   0        0        0      841 2023-05-19 09:32:40.000000 copul-0.0.1/copul/calculations/copulas/families/extreme_value/t_ev.py
--rw-rw-rw-   0        0        0      791 2023-03-30 13:31:03.000000 copul-0.0.1/copul/calculations/copulas/families/extreme_value/tawn.py
-drwxrwxrwx   0        0        0        0 2023-05-19 12:51:15.223082 copul-0.0.1/copul/calculations/copulas/families/other/
--rw-rw-rw-   0        0        0        0 2023-03-09 12:10:27.000000 copul-0.0.1/copul/calculations/copulas/families/other/__init__.py
--rw-rw-rw-   0        0        0      757 2023-03-30 13:31:03.000000 copul-0.0.1/copul/calculations/copulas/families/other/farlie_gumbell_morgenstern.py
--rw-rw-rw-   0        0        0     8892 2023-05-19 09:32:40.000000 copul-0.0.1/copul/calculations/copulas/families/other/plackett.py
-drwxrwxrwx   0        0        0        0 2023-05-19 12:51:15.225076 copul-0.0.1/copul/decorators/
--rw-rw-rw-   0        0        0        0 2022-08-05 21:37:55.000000 copul-0.0.1/copul/decorators/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-19 12:51:15.226075 copul-0.0.1/copul/docs/
--rw-rw-rw-   0        0        0        0 2023-03-30 13:31:03.000000 copul-0.0.1/copul/docs/.gitkeep
-drwxrwxrwx   0        0        0        0 2023-05-19 12:51:15.228081 copul-0.0.1/copul/simulations/
--rw-rw-rw-   0        0        0        0 2022-03-23 14:06:32.000000 copul-0.0.1/copul/simulations/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-19 12:51:15.133319 copul-0.0.1/copul.egg-info/
--rw-rw-rw-   0        0        0     1099 2023-05-19 12:51:15.000000 copul-0.0.1/copul.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     2811 2023-05-19 12:51:15.000000 copul-0.0.1/copul.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-19 12:51:15.000000 copul-0.0.1/copul.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      121 2023-05-19 12:51:15.000000 copul-0.0.1/copul.egg-info/requires.txt
--rw-rw-rw-   0        0        0        6 2023-05-19 12:51:15.000000 copul-0.0.1/copul.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      977 2023-05-19 12:50:54.000000 copul-0.0.1/pyproject.toml
--rw-rw-rw-   0        0        0       86 2023-05-19 12:51:15.232059 copul-0.0.1/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-05-21 19:39:29.155101 copul-0.0.2/
+-rw-rw-rw-   0        0        0     1091 2023-05-21 18:41:35.000000 copul-0.0.2/LICENSE
+-rw-rw-rw-   0        0        0       30 2023-05-17 14:16:18.000000 copul-0.0.2/MANIFEST.in
+-rw-rw-rw-   0        0        0     1869 2023-05-21 19:39:29.155101 copul-0.0.2/PKG-INFO
+-rw-rw-rw-   0        0        0     1332 2023-05-21 19:33:24.000000 copul-0.0.2/README.md
+drwxrwxrwx   0        0        0        0 2023-05-21 19:39:29.130564 copul-0.0.2/copul/
+-rw-rw-rw-   0        0        0      357 2023-05-21 18:51:19.000000 copul-0.0.2/copul/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-21 19:39:29.134070 copul-0.0.2/copul/docs/
+-rw-rw-rw-   0        0        0        0 2023-05-17 14:16:18.000000 copul-0.0.2/copul/docs/.gitkeep
+drwxrwxrwx   0        0        0        0 2023-05-21 19:39:29.135076 copul-0.0.2/copul/families/
+-rw-rw-rw-   0        0        0      236 2023-05-21 18:41:35.000000 copul-0.0.2/copul/families/__init__.py
+-rw-rw-rw-   0        0        0     1165 2023-05-21 18:41:35.000000 copul-0.0.2/copul/families/abstract_copula.py
+drwxrwxrwx   0        0        0        0 2023-05-21 19:39:29.147591 copul-0.0.2/copul/families/archimedean/
+-rw-rw-rw-   0        0        0     5839 2023-05-21 18:51:44.000000 copul-0.0.2/copul/families/archimedean/__init__.py
+-rw-rw-rw-   0        0        0     5321 2023-05-21 18:54:07.000000 copul-0.0.2/copul/families/archimedean/archimedean_copula.py
+-rw-rw-rw-   0        0        0     5160 2023-05-21 18:41:35.000000 copul-0.0.2/copul/families/archimedean/derivatives_overview_constructor.py
+-rw-rw-rw-   0        0        0      828 2023-05-21 18:52:04.000000 copul-0.0.2/copul/families/archimedean/nelsen1.py
+-rw-rw-rw-   0        0        0      299 2023-05-21 18:54:30.000000 copul-0.0.2/copul/families/archimedean/nelsen10.py
+-rw-rw-rw-   0        0        0      294 2023-05-21 18:54:30.000000 copul-0.0.2/copul/families/archimedean/nelsen11.py
+-rw-rw-rw-   0        0        0      393 2023-05-21 18:54:30.000000 copul-0.0.2/copul/families/archimedean/nelsen12.py
+-rw-rw-rw-   0        0        0      322 2023-05-21 18:54:30.000000 copul-0.0.2/copul/families/archimedean/nelsen13.py
+-rw-rw-rw-   0        0        0      421 2023-05-21 18:54:30.000000 copul-0.0.2/copul/families/archimedean/nelsen14.py
+-rw-rw-rw-   0        0        0      357 2023-05-21 18:54:30.000000 copul-0.0.2/copul/families/archimedean/nelsen15.py
+-rw-rw-rw-   0        0        0      778 2023-05-21 18:54:30.000000 copul-0.0.2/copul/families/archimedean/nelsen16.py
+-rw-rw-rw-   0        0        0     2111 2023-05-21 18:54:30.000000 copul-0.0.2/copul/families/archimedean/nelsen17.py
+-rw-rw-rw-   0        0        0      318 2023-05-21 18:54:30.000000 copul-0.0.2/copul/families/archimedean/nelsen18.py
+-rw-rw-rw-   0        0        0      333 2023-05-21 18:54:30.000000 copul-0.0.2/copul/families/archimedean/nelsen19.py
+-rw-rw-rw-   0        0        0      396 2023-05-21 18:54:14.000000 copul-0.0.2/copul/families/archimedean/nelsen2.py
+-rw-rw-rw-   0        0        0      330 2023-05-21 18:54:30.000000 copul-0.0.2/copul/families/archimedean/nelsen20.py
+-rw-rw-rw-   0        0        0      336 2023-05-21 18:54:30.000000 copul-0.0.2/copul/families/archimedean/nelsen21.py
+-rw-rw-rw-   0        0        0      377 2023-05-21 18:54:30.000000 copul-0.0.2/copul/families/archimedean/nelsen22.py
+-rw-rw-rw-   0        0        0      596 2023-05-21 18:54:44.000000 copul-0.0.2/copul/families/archimedean/nelsen3.py
+-rw-rw-rw-   0        0        0      354 2023-05-21 18:54:30.000000 copul-0.0.2/copul/families/archimedean/nelsen4.py
+-rw-rw-rw-   0        0        0      376 2023-05-21 18:54:30.000000 copul-0.0.2/copul/families/archimedean/nelsen5.py
+-rw-rw-rw-   0        0        0      336 2023-05-21 18:54:30.000000 copul-0.0.2/copul/families/archimedean/nelsen6.py
+-rw-rw-rw-   0        0        0      302 2023-05-21 18:54:30.000000 copul-0.0.2/copul/families/archimedean/nelsen7.py
+-rw-rw-rw-   0        0        0      325 2023-05-21 18:54:30.000000 copul-0.0.2/copul/families/archimedean/nelsen8.py
+-rw-rw-rw-   0        0        0      557 2023-05-21 18:54:44.000000 copul-0.0.2/copul/families/archimedean/nelsen9.py
+drwxrwxrwx   0        0        0        0 2023-05-21 19:39:29.152591 copul-0.0.2/copul/families/extreme_value/
+-rw-rw-rw-   0        0        0      386 2023-05-21 18:54:30.000000 copul-0.0.2/copul/families/extreme_value/__init__.py
+-rw-rw-rw-   0        0        0      650 2023-05-21 18:54:30.000000 copul-0.0.2/copul/families/extreme_value/bb5.py
+-rw-rw-rw-   0        0        0     6222 2023-05-21 18:41:35.000000 copul-0.0.2/copul/families/extreme_value/extreme_value_copula.py
+-rw-rw-rw-   0        0        0      619 2023-05-21 18:54:30.000000 copul-0.0.2/copul/families/extreme_value/galambos.py
+-rw-rw-rw-   0        0        0      441 2023-05-21 18:54:30.000000 copul-0.0.2/copul/families/extreme_value/gumbel.py
+-rw-rw-rw-   0        0        0      771 2023-05-21 18:54:30.000000 copul-0.0.2/copul/families/extreme_value/huesler_reiss.py
+-rw-rw-rw-   0        0        0      867 2023-05-21 18:54:30.000000 copul-0.0.2/copul/families/extreme_value/joe.py
+-rw-rw-rw-   0        0        0      527 2023-05-21 18:54:30.000000 copul-0.0.2/copul/families/extreme_value/marshall_olkin.py
+-rw-rw-rw-   0        0        0      820 2023-05-21 18:54:30.000000 copul-0.0.2/copul/families/extreme_value/t_ev.py
+-rw-rw-rw-   0        0        0      770 2023-05-21 18:54:30.000000 copul-0.0.2/copul/families/extreme_value/tawn.py
+drwxrwxrwx   0        0        0        0 2023-05-21 19:39:29.155101 copul-0.0.2/copul/families/other/
+-rw-rw-rw-   0        0        0        0 2023-05-21 18:41:35.000000 copul-0.0.2/copul/families/other/__init__.py
+-rw-rw-rw-   0        0        0      886 2023-05-21 18:54:30.000000 copul-0.0.2/copul/families/other/farlie_gumbell_morgenstern.py
+-rw-rw-rw-   0        0        0      557 2023-05-21 18:54:30.000000 copul-0.0.2/copul/families/other/frechet.py
+-rw-rw-rw-   0        0        0     9054 2023-05-21 18:54:44.000000 copul-0.0.2/copul/families/other/plackett.py
+drwxrwxrwx   0        0        0        0 2023-05-21 19:39:29.155101 copul-0.0.2/copul/simulations/
+-rw-rw-rw-   0        0        0        0 2023-05-17 14:16:18.000000 copul-0.0.2/copul/simulations/__init__.py
+-rw-rw-rw-   0        0        0     1080 2023-05-21 18:41:35.000000 copul-0.0.2/copul/sympy_wrapper.py
+drwxrwxrwx   0        0        0        0 2023-05-21 19:39:29.132564 copul-0.0.2/copul.egg-info/
+-rw-rw-rw-   0        0        0     1869 2023-05-21 19:39:29.000000 copul-0.0.2/copul.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1912 2023-05-21 19:39:29.000000 copul-0.0.2/copul.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-21 19:39:29.000000 copul-0.0.2/copul.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      115 2023-05-21 19:39:29.000000 copul-0.0.2/copul.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        6 2023-05-21 19:39:29.000000 copul-0.0.2/copul.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      977 2023-05-21 19:38:39.000000 copul-0.0.2/pyproject.toml
+-rw-rw-rw-   0        0        0       86 2023-05-21 19:39:29.156617 copul-0.0.2/setup.cfg
```

### Comparing `copul-0.0.1/LICENSE` & `copul-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `copul-0.0.1/copul/calculations/copulas/abstract_copula.py` & `copul-0.0.2/copul/families/abstract_copula.py`

 * *Files 5% similar despite different names*

```diff
@@ -6,17 +6,15 @@
 
     @property
     def cdf(self):
         return None
 
     @property
     def pdf(self):
-        cdf = self.cdf
-        diff_v = sympy.simplify(sympy.diff(cdf, self.v))
-        return sympy.simplify(sympy.diff(diff_v, self.u))
+        return sympy.simplify(sympy.diff(self.cdf, self.u, self.v))
 
     @property
     def log_pdf(self, expand_log=False):
         log_pdf = sympy.simplify(sympy.log(self.pdf))
         return concrete_expand_log(log_pdf) if expand_log else log_pdf
```

### Comparing `copul-0.0.1/copul/calculations/copulas/families/archimedean/__init__.py` & `copul-0.0.2/copul/families/archimedean/derivatives_overview_constructor.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,99 +1,112 @@
 import re
 
 import pandas as pd
 import sympy
 
-from copul.calculations.copulas.abstract_copula import round_expression
-from copul.calculations.copulas.families.archimedean.nelsen17 import Nelsen17
+import families.archimedean.nelsen2
 
 
-def cleanse_latex_str(latex_str):
-    def cleanse_this(input_str):
-        new_str = re.sub("\{(\\d)\}", "\\1", input_str)
-        output_str = re.sub("\^\{(.)\}", "^\\1", new_str)
-        return output_str
-
-    if isinstance(latex_str, pd.Series):
-        return latex_str.apply(lambda val: cleanse_this(val))
-    return cleanse_this(latex_str)
-
-
-def generate_notes_pdf(my_range):
-    cop = "C(u, v)"
-    gen = "$\\psi(y)$"
-    inv_gen = "$\\psi^{-1}(t)$"
-    inv_gen_max = "$\\psi^{-1}(0)$"
-    gen_der = "$\\psi'(y)$"
-    mustbeconv = "$\\log(-\\psi')(y)$"
-    log_der = "$(\\log(-\\psi'))'(y)$"
-    log_der2 = "$(\\log(-\\psi'))''(y)$"
-    gen_der2 = "$\\psi''(y)$"
-    mustbeconv2 = "$\\log(\\psi'')(y)$"
-    log2_der = "$(\\log(\\psi''))'(y)$"
-    log2_der2 = "$(\\log(\\psi''))''(y)$"
-    my_copula = Nelsen17(theta_min=0)
-    # conv_func, log_der_val, log_der2_val, local_min_point, local_min_val = my_copula.log2_der()
-    df = pd.DataFrame(index=my_range)
-    for i in my_range:
-        copula_str = f"Nelsen{str(i)}"
-        print(copula_str)
-        copula = locals()[copula_str](theta_min=0)
-        gen_val = copula.generator
-        gen_der_val = copula.get_first_deriv_of_generator()
-        gen_der2_val = copula.get_second_deriv_of_gen()
-        cop_val = copula.cdf
-        conv_func, log_der_val, log_der2_val, local_min_point, local_min_val = copula.log_der()
-        conv2_func, log2_deriv_val, log2_deriv2_val, local2_min_point, local2_min_val = copula.log2_der()
-        df.loc[i, cop] = "$" + sympy.latex(cop_val) + "$"
-        df.loc[i, "$\\theta$"] = str(copula.theta_interval)
-        df.loc[i, inv_gen] = "$" + sympy.latex(copula.inv_generator) + "$"
-        df.loc[i, inv_gen_max] = str(copula.compute_inv_gen_max())
-        df.loc[i, gen] = "$" + sympy.latex(gen_val) + "$"
-        df.loc[i, gen_der] = "$" + sympy.latex(gen_der_val) + "$"
-        df.loc[i, mustbeconv] = "$" + sympy.latex(conv_func) + "$"
-        df.loc[i, log_der] = "$" + sympy.latex(log_der_val) + "$"
-        df.loc[i, log_der2] = "$" + sympy.latex(log_der2_val) + "$"
-        df.loc[i, f"{log_der2}-min"] = "$" + sympy.latex((local_min_point, local_min_val)) + "$"
-        df.loc[i, gen_der2] = "$" + sympy.latex(gen_der2_val) + "$"
-        df.loc[i, mustbeconv2] = "$" + sympy.latex(conv2_func) + "$"
-        df.loc[i, log2_der] = "$" + sympy.latex(log2_deriv_val) + "$"
-        df.loc[i, log2_der2] = "$" + sympy.latex(log2_deriv2_val) + "$"
-        df.loc[i, f"{log2_der2}-min"] = (
-                "$" + sympy.latex((local2_min_point, local2_min_val)) + "$"
-        )
-    return df
+class DerivativesOverviewConstructor:
+
+    def __init__(self):
+        pass
+
+    @staticmethod
+    def _cleanse_latex_str(latex_str):
+
+        def cleanse_this(input_str):
+            new_str = re.sub("\{(\\d)\}", "\\1", input_str)
+            output_str = re.sub("\^\{(.)\}", "^\\1", new_str)
+            return output_str
+
+        if isinstance(latex_str, pd.Series):
+            return latex_str.apply(lambda val: cleanse_this(val))
+        return cleanse_this(latex_str)
+
+    @staticmethod
+    def _generate_notes_pdf(my_range):
+        cop = "C(u, v)"
+        gen = "$\\psi(y)$"
+        inv_gen = "$\\psi^{-1}(t)$"
+        inv_gen_max = "$\\psi^{-1}(0)$"
+        gen_der = "$\\psi'(y)$"
+        mustbeconv = "$\\log(-\\psi')(y)$"
+        log_der = "$(\\log(-\\psi'))'(y)$"
+        log_der2 = "$(\\log(-\\psi'))''(y)$"
+        gen_der2 = "$\\psi''(y)$"
+        mustbeconv2 = "$\\log(\\psi'')(y)$"
+        log2_der = "$(\\log(\\psi''))'(y)$"
+        log2_der2 = "$(\\log(\\psi''))''(y)$"
+        my_copula = families.archimedean.nelsen17.Nelsen17(theta_min=0)
+        # conv_func, log_der_val, log_der2_val, local_min_point, local_min_val = my_copula.log2_der()
+        df = pd.DataFrame(index=my_range)
+        for i in my_range:
+            copula_str = f"Nelsen{i}"
+            print(copula_str)
+            copula = locals()[copula_str](theta_min=0)
+            gen_val = copula.generator
+            gen_der_val = copula.first_deriv_of_generator()
+            gen_der2_val = copula.second_deriv_of_gen
+            cop_val = copula.cdf
+            conv_func, log_der_val, log_der2_val, local_min_point, local_min_val = copula.log_der()
+            conv2_func, log2_deriv_val, log2_deriv2_val, local2_min_point, local2_min_val = copula.log2_der()
+            df.loc[i, cop] = "$" + sympy.latex(cop_val) + "$"
+            df.loc[i, "$\\theta$"] = str(copula.theta_interval)
+            df.loc[i, inv_gen] = "$" + sympy.latex(copula.inverse_generator) + "$"
+            df.loc[i, inv_gen_max] = str(copula.compute_inv_gen_max())
+            df.loc[i, gen] = "$" + sympy.latex(gen_val) + "$"
+            df.loc[i, gen_der] = "$" + sympy.latex(gen_der_val) + "$"
+            df.loc[i, mustbeconv] = "$" + sympy.latex(conv_func) + "$"
+            df.loc[i, log_der] = "$" + sympy.latex(log_der_val) + "$"
+            df.loc[i, log_der2] = "$" + sympy.latex(log_der2_val) + "$"
+            df.loc[i, f"{log_der2}-min"] = f"${sympy.latex((local_min_point, local_min_val))}$"
+            df.loc[i, gen_der2] = f"${sympy.latex(gen_der2_val)}$"
+            df.loc[i, mustbeconv2] = f"${sympy.latex(conv2_func)}$"
+            df.loc[i, log2_der] = "$" + sympy.latex(log2_deriv_val) + "$"
+            df.loc[i, log2_der2] = "$" + sympy.latex(log2_deriv2_val) + "$"
+            df.loc[i, f"{log2_der2}-min"] = f"${sympy.latex((local2_min_point, local2_min_val))}$"
+        return df
+
+    def construct_extract(self):
+        my_range = list(range(16, 17))
+        df = self._generate_notes_pdf(my_range)
+        pd.set_option('display.max_colwidth', None)
+        tables = {f"Nelsen{i}": df.T[[i]].reset_index().rename(columns={i: "Value", "index": "Characteristic"}) for
+                  i in my_range}
+        table_strs = [self._cleanse_latex_str(v.to_latex(escape=False)) + "\\caption{" + k + "}\\label{tab:" + k + "}" for
+                      k, v in tables.items()]
+
+        def table_to_formula(k, v):
+            v = v.drop(v.index[[0, 1, 2, 3, 9, 14]])
+            return "\item " + k + ": \n\\begin{align}\n" + (v["Characteristic"] + " ~=~ & " + self._cleanse_latex_str(
+                v["Value"]) + ", \\nonumber\\\\").str.replace("$", "").str.cat(
+                sep="\n")[:-13] + "\\nonumber" + ".\n\\end{align}\n"
+
+        table_strs2 = {k: table_to_formula(k, v) for k, v in tables.items()}
+        start_str = "\\begin{table}[H]\\begin{center}"
+        end_str = "\\end{center}\\end{table}"
+        # full_table = "\n\n".join([start_str + tab + end_str for tab in table_strs])
+        # full_table2 = "\\begin{itemize}\n" + "\n\n".join([table_strs2[tab] for tab in table_strs2]) + "\\end{itemize}"
+
+
+def round_expression(expr):
+    expr = sympy.simplify(expr)
+    for a in sympy.preorder_traversal(expr):
+        if isinstance(a, sympy.Float):
+            expr = expr.subs(a, round(a, 2))
+    return expr
 
 
 if __name__ == "__main__":
-    cop = Nelsen17()
-    gen = cop.generator.subs(cop.theta, 5.5)
-    diff2 = round_expression(sympy.diff(gen, cop.y, 2))
-    diff3 = round_expression(sympy.diff(gen, cop.y, 3))
-    diff4 = round_expression(sympy.diff(gen, cop.y, 4))
-    diff5 = round_expression(sympy.diff(gen, cop.y, 5))
-    diff6 = round_expression(sympy.diff(gen, cop.y, 6))
-    diff7 = round_expression(sympy.diff(gen, cop.y, 7))
-    my_gen_plot = sympy.plotting.plot(diff2, (cop.y, 5, 20), show=False, legend=True)
-    my_gen_plot.show()
-    cdf = cop.cdf().subs(cop.theta, 0.5)
-    my_range = list(range(16, 17))
-    df = generate_notes_pdf(my_range)
-    pd.set_option('display.max_colwidth', None)
-    tables = {"Nelsen" + str(i): df.T[[i]].reset_index().rename(columns={i: "Value", "index": "Characteristic"}) for i
-              in my_range}
-    table_strs = [cleanse_latex_str(v.to_latex(escape=False)) + "\\caption{" + k + "}\\label{tab:" + k + "}" for k, v in
-                  tables.items()]
-
-
-    def table_to_formula(k, v):
-        v = v.drop(v.index[[0, 1, 2, 3, 9, 14]])
-        return "\item " + k + ": \n\\begin{align}\n" + (v["Characteristic"] + " ~=~ & " + cleanse_latex_str(
-            v["Value"]) + ", \\nonumber\\\\").str.replace("$", "").str.cat(
-            sep="\n")[:-13] + "\\nonumber" + ".\n\\end{align}\n"
-
-    table_strs2 = {k: table_to_formula(k, v) for k, v in tables.items()}
-    start_str = "\\begin{table}[H]\\begin{center}"
-    end_str = "\\end{center}\\end{table}"
-    full_table = "\n\n".join([start_str + tab + end_str for tab in table_strs])
-    full_table2 = "\\begin{itemize}\n" + "\n\n".join([table_strs2[tab] for tab in table_strs2]) + "\\end{itemize}"
+    my_cop = families.archimedean.nelsen2.Nelsen2()
+    # gen = cop.generator().subs(cop.theta, 5.5)
+    # diff2 = round_expression(sympy.diff(gen, cop.y, 2))
+    # diff3 = round_expression(sympy.diff(gen, cop.y, 3))
+    # diff4 = round_expression(sympy.diff(gen, cop.y, 4))
+    # diff5 = round_expression(sympy.diff(gen, cop.y, 5))
+    # diff6 = round_expression(sympy.diff(gen, cop.y, 6))
+    # diff7 = round_expression(sympy.diff(gen, cop.y, 7))
+    # my_gen_plot = sympy.plotting.plot(diff2, (cop.y, 5, 20), show=False, legend=True)
+    # my_gen_plot.show()
+    cdf = my_cop.cdf().subs(my_cop.theta, 2)
     exit()
```

### Comparing `copul-0.0.1/copul/calculations/copulas/families/archimedean/archimedean_copula.py` & `copul-0.0.2/copul/families/archimedean/archimedean_copula.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,12 +1,14 @@
 import numpy as np
 import sympy
 from scipy import optimize
 
-from copul.calculations.copulas.abstract_copula import AbstractCopula, concrete_expand_log
+from copul.families import get_simplified_solution
+from copul.families.abstract_copula import AbstractCopula, concrete_expand_log
+from copul.sympy_wrapper import SymPyFunctionWrapper
 
 
 class ArchimedeanCopula(AbstractCopula):
     _t_min = 0
     _t_max = 1
     y, t, theta = sympy.symbols("y t theta", positive=True)
     theta_interval = None
@@ -17,87 +19,105 @@
             self.theta_interval = sympy.Interval(theta_min, self.theta_max, left_open=self.theta_interval.left_open,
                                                  right_open=self.theta_interval.right_open)
         if theta_max is not None:
             self.theta_interval = sympy.Interval(self.theta_min, theta_max, left_open=self.theta_interval.left_open,
                                                  right_open=self.theta_interval.right_open)
 
     @property
-    def inv_generator(self):
-        return self._inv_generator
+    def inverse_generator(self):
+        return SymPyFunctionWrapper(self._inv_generator)
 
     @property
     def theta_max(self):
         return self.theta_interval.closure.end
 
     @property
     def theta_min(self):
         return self.theta_interval.closure.inf
 
-    @staticmethod
-    def _get_simplified_solution(sol):
-        simplified_sol = sympy.simplify(sol)
-        if isinstance(simplified_sol, sympy.core.containers.Tuple):
-            return simplified_sol[0]
-        else:
-            return simplified_sol
-
     @property
     def cdf(self):
+        """ Cumulative distribution function of the copula """
         gen = self.generator
-        cop = gen.subs(self.y, self._inv_generator.subs(self.t, self.u) + self._inv_generator.subs(self.t, self.v))
-        return self._get_simplified_solution(cop)
+        inv_gen_at_u = self._inv_generator.subs(self.t, self.u)
+        inv_gen_at_v = self._inv_generator.subs(self.t, self.v)
+        cdf = gen.subs(self.y, inv_gen_at_u + inv_gen_at_v)
+        return SymPyFunctionWrapper(get_simplified_solution(cdf.func))
+
+    @property
+    def pdf(self):
+        """ Probability density function of the copula """
+        cdf = self.cdf
+        first_diff = sympy.diff(cdf, self.u)
+        pdf = sympy.diff(first_diff, self.v)
+        return SymPyFunctionWrapper(get_simplified_solution(pdf.func))
 
     @property
     def generator(self):
         eq = sympy.Eq(self.y, self._inv_generator)
         sol = sympy.solve([eq, self.theta > 0, self.y > 0], self.t)
         my_sol = sol[self.t] if isinstance(sol, dict) else sol[0]
-        return self._get_simplified_solution(my_sol)
+        my_simplified_sol = get_simplified_solution(my_sol)
+        return SymPyFunctionWrapper(my_simplified_sol)
 
-    def get_first_deriv_of_generator(self):
-        gen = self.generator
-        return sympy.simplify(sympy.diff(gen, self.y))
+    @property
+    def first_deriv_of_generator(self):
+        diff = sympy.diff(self.generator.func, self.y)
+        return sympy.simplify(diff)
 
-    def get_second_deriv_of_gen(self):
-        return sympy.simplify(sympy.diff(self.get_first_deriv_of_generator(), self.y))
+    @property
+    def second_deriv_of_gen(self):
+        first_diff = self.first_deriv_of_generator
+        second_diff = sympy.diff(first_diff, self.y)
+        return sympy.simplify(second_diff)
 
-    def get_ci_char_function(self):
-        minus_gen_deriv = - self.get_first_deriv_of_generator()
-        return concrete_expand_log(sympy.simplify(sympy.log(minus_gen_deriv)))
+    @property
+    def ci_char(self):
+        minus_gen_deriv = - self.first_deriv_of_generator
+        beauty_deriv = concrete_expand_log(sympy.simplify(sympy.log(minus_gen_deriv)))
+        return SymPyFunctionWrapper(beauty_deriv)
 
-    def get_first_deriv_of_ci_char_function(self):
-        chi_char_func = self.get_ci_char_function()
+    @property
+    def first_deriv_of_ci_char(self):
+        chi_char_func = self.ci_char()
         return sympy.simplify(sympy.diff(chi_char_func, self.y))
 
-    def get_second_deriv_of_ci_char_function(self):
-        chi_char_func_deriv = self.get_first_deriv_of_ci_char_function()
+    @property
+    def second_deriv_of_ci_char(self):
+        chi_char_func_deriv = self.first_deriv_of_ci_char()
         return sympy.simplify(sympy.diff(chi_char_func_deriv, self.y))
 
-    def get_mtp2_char_function(self):
-        second_deriv = self.get_second_deriv_of_gen()
-        return concrete_expand_log(sympy.simplify(sympy.log(second_deriv)))
+    @property
+    def mtp2_char(self):
+        second_deriv = self.second_deriv_of_gen
+        beauty_2deriv = concrete_expand_log(sympy.simplify(sympy.log(second_deriv)))
+        return SymPyFunctionWrapper(beauty_2deriv)
 
-    def get_first_deriv_of_mtp2_char(self):
-        mtp2_char = self.get_mtp2_char_function()
+    @property
+    def first_deriv_of_mtp2_char(self):
+        mtp2_char = self.mtp2_char()
         return sympy.simplify(sympy.diff(mtp2_char, self.y))
 
-    def get_second_deriv_of_mtp2_char(self):
-        mtp2_char_deriv = self.get_first_deriv_of_mtp2_char()
+    @property
+    def second_deriv_of_mtp2_char(self):
+        mtp2_char_deriv = self.first_deriv_of_mtp2_char()
         return sympy.simplify(sympy.diff(mtp2_char_deriv, self.y))
 
+    @property
     def log_der(self):
-        minus_log_derivative = self.get_ci_char_function()
-        first_deriv = self.get_first_deriv_of_ci_char_function()
-        second_deriv = self.get_second_deriv_of_ci_char_function()
+        minus_log_derivative = self.ci_char()
+        first_deriv = self.first_deriv_of_ci_char()
+        second_deriv = self.second_deriv_of_ci_char()
         return self._compute_log2_der_of(first_deriv, minus_log_derivative, second_deriv)
 
+    @property
     def log2_der(self):
-        log_second_derivative = self.get_mtp2_char_function()
-        first_deriv = self.get_first_deriv_of_mtp2_char()
-        second_deriv = self.get_second_deriv_of_mtp2_char()
+        log_second_derivative = self.mtp2_char()
+        first_deriv = self.first_deriv_of_mtp2_char()
+        second_deriv = self.second_deriv_of_mtp2_char()
         return self._compute_log2_der_of(first_deriv, log_second_derivative, second_deriv)
 
     def _compute_log2_der_of(self, first_deriv, log_second_derivative, second_deriv):
         log_der_lambda = sympy.lambdify([(self.y, self.theta)], second_deriv)
         bounds = [(self._t_min, self._t_max), (self.theta_min, self.theta_max)]
         starting_point = np.array([min(self._t_min + 0.5, self._t_max), min(self.theta_min + 0.5, self.theta_max)])
         min_val = optimize.minimize(log_der_lambda, starting_point, bounds=bounds)
```

### Comparing `copul-0.0.1/copul/calculations/copulas/families/archimedean/derivatives_overview_constructor.py` & `copul-0.0.2/copul/families/archimedean/__init__.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,113 +1,121 @@
 import re
 
 import pandas as pd
 import sympy
 
-import calculations.copulas.families.archimedean.nelsen17
-import calculations.copulas.families.archimedean.nelsen2
+from copul.families.abstract_copula import round_expression
 
-
-class DerivativesOverviewConstructor:
-
-    def __init__(self):
-        pass
-
-    @staticmethod
-    def _cleanse_latex_str(latex_str):
-
-        def cleanse_this(input_str):
-            new_str = re.sub("\{(\\d)\}", "\\1", input_str)
-            output_str = re.sub("\^\{(.)\}", "^\\1", new_str)
-            return output_str
-
-        if isinstance(latex_str, pd.Series):
-            return latex_str.apply(lambda val: cleanse_this(val))
-        return cleanse_this(latex_str)
-
-    @staticmethod
-    def _generate_notes_pdf(my_range):
-        cop = "C(u, v)"
-        gen = "$\\psi(y)$"
-        inv_gen = "$\\psi^{-1}(t)$"
-        inv_gen_max = "$\\psi^{-1}(0)$"
-        gen_der = "$\\psi'(y)$"
-        mustbeconv = "$\\log(-\\psi')(y)$"
-        log_der = "$(\\log(-\\psi'))'(y)$"
-        log_der2 = "$(\\log(-\\psi'))''(y)$"
-        gen_der2 = "$\\psi''(y)$"
-        mustbeconv2 = "$\\log(\\psi'')(y)$"
-        log2_der = "$(\\log(\\psi''))'(y)$"
-        log2_der2 = "$(\\log(\\psi''))''(y)$"
-        my_copula = calculations.copulas.families.archimedean.nelsen17.Nelsen17(theta_min=0)
-        # conv_func, log_der_val, log_der2_val, local_min_point, local_min_val = my_copula.log2_der()
-        df = pd.DataFrame(index=my_range)
-        for i in my_range:
-            copula_str = f"Nelsen{i}"
-            print(copula_str)
-            copula = locals()[copula_str](theta_min=0)
-            gen_val = copula.generator
-            gen_der_val = copula.get_first_deriv_of_generator()
-            gen_der2_val = copula.get_second_deriv_of_gen()
-            cop_val = copula.cdf
-            conv_func, log_der_val, log_der2_val, local_min_point, local_min_val = copula.log_der()
-            conv2_func, log2_deriv_val, log2_deriv2_val, local2_min_point, local2_min_val = copula.log2_der()
-            df.loc[i, cop] = "$" + sympy.latex(cop_val) + "$"
-            df.loc[i, "$\\theta$"] = str(copula.theta_interval)
-            df.loc[i, inv_gen] = "$" + sympy.latex(copula.inv_generator) + "$"
-            df.loc[i, inv_gen_max] = str(copula.compute_inv_gen_max())
-            df.loc[i, gen] = "$" + sympy.latex(gen_val) + "$"
-            df.loc[i, gen_der] = "$" + sympy.latex(gen_der_val) + "$"
-            df.loc[i, mustbeconv] = "$" + sympy.latex(conv_func) + "$"
-            df.loc[i, log_der] = "$" + sympy.latex(log_der_val) + "$"
-            df.loc[i, log_der2] = "$" + sympy.latex(log_der2_val) + "$"
-            df.loc[i, f"{log_der2}-min"] = f"${sympy.latex((local_min_point, local_min_val))}$"
-            df.loc[i, gen_der2] = f"${sympy.latex(gen_der2_val)}$"
-            df.loc[i, mustbeconv2] = f"${sympy.latex(conv2_func)}$"
-            df.loc[i, log2_der] = "$" + sympy.latex(log2_deriv_val) + "$"
-            df.loc[i, log2_der2] = "$" + sympy.latex(log2_deriv2_val) + "$"
-            df.loc[i, f"{log2_der2}-min"] = f"${sympy.latex((local2_min_point, local2_min_val))}$"
-        return df
-
-    def construct_extract(self):
-        my_range = list(range(16, 17))
-        df = self._generate_notes_pdf(my_range)
-        pd.set_option('display.max_colwidth', None)
-        tables = {f"Nelsen{i}": df.T[[i]].reset_index().rename(columns={i: "Value", "index": "Characteristic"}) for
-                  i in my_range}
-        table_strs = [self._cleanse_latex_str(v.to_latex(escape=False)) + "\\caption{" + k + "}\\label{tab:" + k + "}" for
-                      k, v in tables.items()]
-
-        def table_to_formula(k, v):
-            v = v.drop(v.index[[0, 1, 2, 3, 9, 14]])
-            return "\item " + k + ": \n\\begin{align}\n" + (v["Characteristic"] + " ~=~ & " + self._cleanse_latex_str(
-                v["Value"]) + ", \\nonumber\\\\").str.replace("$", "").str.cat(
-                sep="\n")[:-13] + "\\nonumber" + ".\n\\end{align}\n"
-
-        table_strs2 = {k: table_to_formula(k, v) for k, v in tables.items()}
-        start_str = "\\begin{table}[H]\\begin{center}"
-        end_str = "\\end{center}\\end{table}"
-        # full_table = "\n\n".join([start_str + tab + end_str for tab in table_strs])
-        # full_table2 = "\\begin{itemize}\n" + "\n\n".join([table_strs2[tab] for tab in table_strs2]) + "\\end{itemize}"
-
-
-def round_expression(expr):
-    expr = sympy.simplify(expr)
-    for a in sympy.preorder_traversal(expr):
-        if isinstance(a, sympy.Float):
-            expr = expr.subs(a, round(a, 2))
-    return expr
+from copul.families.archimedean.nelsen1 import Nelsen1, Clayton
+from copul.families.archimedean.nelsen2 import Nelsen2
+from copul.families.archimedean.nelsen3 import Nelsen3, AliMikhailHak
+from copul.families.archimedean.nelsen4 import Nelsen4, GumbellHougaard
+from copul.families.archimedean.nelsen5 import Nelsen5, Frank
+from copul.families.archimedean.nelsen6 import Nelsen6, Joe
+from copul.families.archimedean.nelsen7 import Nelsen7
+from copul.families.archimedean.nelsen8 import Nelsen8
+from copul.families.archimedean.nelsen9 import Nelsen9, GumbellBarnett
+from copul.families.archimedean.nelsen10 import Nelsen10
+from copul.families.archimedean.nelsen11 import Nelsen11
+from copul.families.archimedean.nelsen12 import Nelsen12
+from copul.families.archimedean.nelsen13 import Nelsen13
+from copul.families.archimedean.nelsen14 import Nelsen14
+from copul.families.archimedean.nelsen15 import Nelsen15, GenestGhoudi
+from copul.families.archimedean.nelsen16 import Nelsen16
+from copul.families.archimedean.nelsen17 import Nelsen17
+from copul.families.archimedean.nelsen18 import Nelsen18
+from copul.families.archimedean.nelsen19 import Nelsen19
+from copul.families.archimedean.nelsen20 import Nelsen20
+from copul.families.archimedean.nelsen21 import Nelsen21
+from copul.families.archimedean.nelsen22 import Nelsen22
+
+
+def cleanse_latex_str(latex_str):
+    def cleanse_this(input_str):
+        new_str = re.sub("\{(\\d)\}", "\\1", input_str)
+        output_str = re.sub("\^\{(.)\}", "^\\1", new_str)
+        return output_str
+
+    if isinstance(latex_str, pd.Series):
+        return latex_str.apply(lambda val: cleanse_this(val))
+    return cleanse_this(latex_str)
+
+
+def generate_notes_pdf(my_range):
+    cop = "C(u, v)"
+    gen = "$\\psi(y)$"
+    inv_gen = "$\\psi^{-1}(t)$"
+    inv_gen_max = "$\\psi^{-1}(0)$"
+    gen_der = "$\\psi'(y)$"
+    mustbeconv = "$\\log(-\\psi')(y)$"
+    log_der = "$(\\log(-\\psi'))'(y)$"
+    log_der2 = "$(\\log(-\\psi'))''(y)$"
+    gen_der2 = "$\\psi''(y)$"
+    mustbeconv2 = "$\\log(\\psi'')(y)$"
+    log2_der = "$(\\log(\\psi''))'(y)$"
+    log2_der2 = "$(\\log(\\psi''))''(y)$"
+    my_copula = Nelsen17(theta_min=0)
+    # conv_func, log_der_val, log_der2_val, local_min_point, local_min_val = my_copula.log2_der()
+    df = pd.DataFrame(index=my_range)
+    for i in my_range:
+        copula_str = f"Nelsen{str(i)}"
+        print(copula_str)
+        copula = locals()[copula_str](theta_min=0)
+        gen_val = copula.generator
+        gen_der_val = copula.first_deriv_of_generator
+        gen_der2_val = copula.second_deriv_of_gen
+        cop_val = copula.cdf
+        conv_func, log_der_val, log_der2_val, local_min_point, local_min_val = copula.log_der()
+        conv2_func, log2_deriv_val, log2_deriv2_val, local2_min_point, local2_min_val = copula.log2_der()
+        df.loc[i, cop] = "$" + sympy.latex(cop_val) + "$"
+        df.loc[i, "$\\theta$"] = str(copula.theta_interval)
+        df.loc[i, inv_gen] = "$" + sympy.latex(copula.inverse_generator) + "$"
+        df.loc[i, inv_gen_max] = str(copula.compute_inv_gen_max())
+        df.loc[i, gen] = "$" + sympy.latex(gen_val) + "$"
+        df.loc[i, gen_der] = "$" + sympy.latex(gen_der_val) + "$"
+        df.loc[i, mustbeconv] = "$" + sympy.latex(conv_func) + "$"
+        df.loc[i, log_der] = "$" + sympy.latex(log_der_val) + "$"
+        df.loc[i, log_der2] = "$" + sympy.latex(log_der2_val) + "$"
+        df.loc[i, f"{log_der2}-min"] = "$" + sympy.latex((local_min_point, local_min_val)) + "$"
+        df.loc[i, gen_der2] = "$" + sympy.latex(gen_der2_val) + "$"
+        df.loc[i, mustbeconv2] = "$" + sympy.latex(conv2_func) + "$"
+        df.loc[i, log2_der] = "$" + sympy.latex(log2_deriv_val) + "$"
+        df.loc[i, log2_der2] = "$" + sympy.latex(log2_deriv2_val) + "$"
+        df.loc[i, f"{log2_der2}-min"] = (
+                "$" + sympy.latex((local2_min_point, local2_min_val)) + "$"
+        )
+    return df
 
 
 if __name__ == "__main__":
-    my_cop = calculations.copulas.families.archimedean.nelsen2.Nelsen2()
-    # gen = cop.generator().subs(cop.theta, 5.5)
-    # diff2 = round_expression(sympy.diff(gen, cop.y, 2))
-    # diff3 = round_expression(sympy.diff(gen, cop.y, 3))
-    # diff4 = round_expression(sympy.diff(gen, cop.y, 4))
-    # diff5 = round_expression(sympy.diff(gen, cop.y, 5))
-    # diff6 = round_expression(sympy.diff(gen, cop.y, 6))
-    # diff7 = round_expression(sympy.diff(gen, cop.y, 7))
-    # my_gen_plot = sympy.plotting.plot(diff2, (cop.y, 5, 20), show=False, legend=True)
-    # my_gen_plot.show()
-    cdf = my_cop.cdf().subs(my_cop.theta, 2)
+    cop = Nelsen17()
+    gen = cop.generator.subs(cop.theta, 5.5)
+    diff2 = round_expression(sympy.diff(gen, cop.y, 2))
+    diff3 = round_expression(sympy.diff(gen, cop.y, 3))
+    diff4 = round_expression(sympy.diff(gen, cop.y, 4))
+    diff5 = round_expression(sympy.diff(gen, cop.y, 5))
+    diff6 = round_expression(sympy.diff(gen, cop.y, 6))
+    diff7 = round_expression(sympy.diff(gen, cop.y, 7))
+    my_gen_plot = sympy.plotting.plot(diff2, (cop.y, 5, 20), show=False, legend=True)
+    my_gen_plot.show()
+    cdf = cop.cdf().subs(cop.theta, 0.5)
+    my_range = list(range(16, 17))
+    df = generate_notes_pdf(my_range)
+    pd.set_option('display.max_colwidth', None)
+    tables = {"Nelsen" + str(i): df.T[[i]].reset_index().rename(columns={i: "Value", "index": "Characteristic"}) for i
+              in my_range}
+    table_strs = [cleanse_latex_str(v.to_latex(escape=False)) + "\\caption{" + k + "}\\label{tab:" + k + "}" for k, v in
+                  tables.items()]
+
+
+    def table_to_formula(k, v):
+        v = v.drop(v.index[[0, 1, 2, 3, 9, 14]])
+        return "\item " + k + ": \n\\begin{align}\n" + (v["Characteristic"] + " ~=~ & " + cleanse_latex_str(
+            v["Value"]) + ", \\nonumber\\\\").str.replace("$", "").str.cat(
+            sep="\n")[:-13] + "\\nonumber" + ".\n\\end{align}\n"
+
+    table_strs2 = {k: table_to_formula(k, v) for k, v in tables.items()}
+    start_str = "\\begin{table}[H]\\begin{center}"
+    end_str = "\\end{center}\\end{table}"
+    full_table = "\n\n".join([start_str + tab + end_str for tab in table_strs])
+    full_table2 = "\\begin{itemize}\n" + "\n\n".join([table_strs2[tab] for tab in table_strs2]) + "\\end{itemize}"
     exit()
```

### Comparing `copul-0.0.1/copul/calculations/copulas/families/archimedean/nelsen16.py` & `copul-0.0.2/copul/families/archimedean/nelsen16.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 import numpy as np
 import sympy
 
-from copul.calculations.copulas.families.archimedean.archimedean_copula import ArchimedeanCopula
+from copul.families.archimedean.archimedean_copula import ArchimedeanCopula
 
 
 class Nelsen16(ArchimedeanCopula):
     ac = ArchimedeanCopula
     _inv_generator = (ac.theta / ac.t + 1) * (1 - ac.t)
     theta_interval = sympy.Interval(0, np.inf, left_open=True, right_open=True)
 
     def generator(self):
         return -self.theta / 2 - self.y / 2 + 1 / 2 + 1 / 2 * sympy.sqrt(
             (self.theta + self.y - 1) ** 2 + 4 * self.theta)
 
-    def get_first_deriv_of_generator(self):
+    def first_deriv_of_generator(self):
         return (self.theta + self.y - 1) / (2 * ((self.theta + self.y - 1) ** 2 + 4 * self.theta)) - 1 / 2
 
-    def get_ci_char_function(self):
+    def ci_char(self):
         return sympy.log(1 / 2 - (self.theta + self.y - 1) / (8 * self.theta + 2 * (self.theta + self.y - 1) ** 2))
```

### Comparing `copul-0.0.1/copul/calculations/copulas/families/archimedean/nelsen17.py` & `copul-0.0.2/copul/families/archimedean/nelsen17.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,38 +1,38 @@
 import numpy as np
 import sympy
 
-from copul.calculations.copulas.families.archimedean.archimedean_copula import ArchimedeanCopula
+from copul.families.archimedean.archimedean_copula import ArchimedeanCopula
 
 
 class Nelsen17(ArchimedeanCopula):
     ac = ArchimedeanCopula
     _inv_generator = -sympy.log(((1 + ac.t) ** (-ac.theta) - 1) / (2 ** (-ac.theta) - 1))
     theta_interval = sympy.Interval(-np.inf, np.inf, left_open=False, right_open=True)
 
-    def get_first_deriv_of_generator(self):
+    def first_deriv_of_generator(self):
         return sympy.simplify(
             (2 ** self.theta * sympy.exp(self.y) / (2 ** self.theta * sympy.exp(self.y) - 2 ** self.theta + 1)) ** (
                     1 / self.theta) *
             (2 ** self.theta * (- 2 ** self.theta + 1)) /
             (2 ** self.theta * self.theta * (2 ** self.theta * sympy.exp(self.y) - 2 ** self.theta + 1)))
 
-    def get_second_deriv_of_gen(self):
+    def second_deriv_of_gen(self):
         return sympy.simplify(
             (2 ** self.theta * sympy.exp(self.y) / (2 ** self.theta * sympy.exp(self.y) - 2 ** self.theta + 1)) ** (
                     1 / self.theta) *
             (2 ** self.theta * self.theta * (-2 ** self.theta + 1) * sympy.exp(self.y)
              - 2 ** (self.theta + 1) * self.theta * (- 2 ** self.theta + 1) * sympy.exp(self.y)
              + (2 ** self.theta - 1) ** 2) / (
                     self.theta ** 2 * (2 ** self.theta * sympy.exp(self.y) - 2 ** self.theta + 1) ** 2))
 
-    def get_first_deriv_of_ci_char_function(self):
+    def first_deriv_of_ci_char(self):
         return sympy.simplify((2 ** self.theta * (- 2 ** self.theta + 1) -
                                4 ** self.theta * self.theta * sympy.exp(self.y)) /
                               (2 ** self.theta * self.theta * (
                                       2 ** self.theta * sympy.exp(self.y) - 2 ** self.theta + 1)))
 
-    def get_first_deriv_of_mtp2_char(self):
+    def first_deriv_of_mtp2_char(self):
         return 1 / self.theta + 2 ** self.theta * sympy.exp(self.y) * (
                 1 / (2 ** self.theta * sympy.exp(self.y) - 2 ** self.theta + 1) +
                 self.theta / (2 ** self.theta * self.theta * sympy.exp(self.y) + 2 ** self.theta + 1) -
                 1 / (2 ** self.theta * self.theta * sympy.exp(self.y) - 2 ** self.theta * self.theta + self.theta))
```

### Comparing `copul-0.0.1/copul/calculations/copulas/families/extreme_value/bb5.py` & `copul-0.0.2/copul/families/archimedean/nelsen1.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,18 +1,25 @@
 import numpy as np
 import sympy
 
-from copul.calculations.copulas.families.extreme_value.extreme_value_copula import ExtremeValueCopula
+from copul.families.archimedean.archimedean_copula import ArchimedeanCopula
+from copul.sympy_wrapper import SymPyFunctionWrapper
 
 
-class BB5(ExtremeValueCopula):
-    theta, delta = sympy.symbols("theta delta")
+class Clayton(ArchimedeanCopula):
+    ac = ArchimedeanCopula
+    _inv_generator = ((1 / ac.t) ** ac.theta - 1) / ac.theta
+    theta_interval = sympy.Interval(0, np.inf, left_open=False, right_open=True)
 
-    def __init__(self):
-        def pickand(t, th, d):
-            return (t ** th + (1 - t) ** th - ((1 - t) ** (-th * d) + t ** (-th * d)) ** (-1 / d)) ** (1 / th)
+    @property
+    def cdf(self):
+        cdf = sympy.Max((self.u**(-self.theta) + self.v**(-self.theta) - 1)**(-1/self.theta), 0)
+        return SymPyFunctionWrapper(cdf)
 
-        self.pickand = pickand(self.t, self.theta, self.delta)
-        self.intervals = {
-            self.theta: sympy.Interval(1, np.inf, left_open=False, right_open=True),
-            self.delta: sympy.Interval(0, np.inf, left_open=True, right_open=True),
-        }
+    @property
+    def pdf(self):  # ToDo: check this
+        pdf = (self.u**(-self.theta) + self.v**(-self.theta) - 1)**(-1-2/self.theta) \
+            * self.u**(-self.theta-1) * self.v**(-self.theta-1)
+        return SymPyFunctionWrapper(pdf)
+
+
+Nelsen1 = Clayton
```

### Comparing `copul-0.0.1/copul/calculations/copulas/families/extreme_value/extreme_value_copula.py` & `copul-0.0.2/copul/families/extreme_value/extreme_value_copula.py`

 * *Files 2% similar despite different names*

```diff
@@ -17,27 +17,29 @@
         return self.pickand.free_symbols - {self.t}
 
     def sample_parameters(self, n=1):
         return {k: list(np.random.uniform(max(-10, v.start), min(10, v.end), n)) for k, v in self.intervals.items()}
 
     @property
     def cdf(self):
+        """ Cumulative distribution function of the copula """
         u, v = sympy.symbols("u v")
         cop = (u * v) ** self.pickand.subs(self.t, sympy.ln(v) / sympy.ln(u * v))
         cop = self._get_simplified_solution(cop)
         return cop
 
     def compute_pdf(self):
         cdf = self.cdf
         pdf = sympy.diff(sympy.diff(cdf, "u"), "v")
         pdf = self._get_simplified_solution(pdf)
         return pdf.doit()
 
     @property
     def pdf(self):
+        """ Probability density function of the copula """
         _xi_1, u, v = sympy.symbols("_xi_1 u v")
         pdf = (u * v) ** self.pickand.subs(self.t, log(v) / log(u * v)) * (-(
                 (log(v) - log(u * v)) * Subs(Derivative(self.pickand.subs(self.t, _xi_1), _xi_1), _xi_1,
                                              log(v) / log(u * v)) - self.pickand.subs(self.t, log(v) / log(u * v)) *
                 log(u * v)) * (self.pickand.subs(self.t, log(v) / log(u * v)) * log(u * v) - log(v) *
                                Subs(Derivative(self.pickand.subs(self.t, _xi_1), _xi_1), _xi_1, log(v) / log(u * v))) *
                                                                            log(u * v) + (log(v) - log(u * v)) * log(
```

### Comparing `copul-0.0.1/copul/calculations/copulas/families/extreme_value/galambos.py` & `copul-0.0.2/copul/families/extreme_value/galambos.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 import numpy as np
 import sympy
 
-from copul.calculations.copulas.families.extreme_value.extreme_value_copula import ExtremeValueCopula
+from copul.families.extreme_value.extreme_value_copula import ExtremeValueCopula
 
 
 class Galambos(ExtremeValueCopula):
     delta = sympy.symbols("delta")
 
     def __init__(self):
         self.pickand = 1 - (self.t ** (-self.delta) + (1 - self.t) ** (-self.delta)) ** (-1 / self.delta)
```

### Comparing `copul-0.0.1/copul/calculations/copulas/families/extreme_value/huesler_reiss.py` & `copul-0.0.2/copul/families/extreme_value/huesler_reiss.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import numpy as np
 import sympy
 from sympy import stats
 
-from copul.calculations.copulas.families.extreme_value.extreme_value_copula import ExtremeValueCopula
+from copul.families.extreme_value.extreme_value_copula import ExtremeValueCopula
 
 
 class HueslerReiss(ExtremeValueCopula):
     lambda_ = sympy.symbols("lambda")
 
     def __init__(self):
         z = lambda t: 1 / self.lambda_ + self.lambda_ / 2 * sympy.ln(t / (1 - t))
```

### Comparing `copul-0.0.1/copul/calculations/copulas/families/extreme_value/joe.py` & `copul-0.0.2/copul/families/extreme_value/joe.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 import numpy as np
 import sympy
 
-from copul.calculations.copulas.families.extreme_value.extreme_value_copula import ExtremeValueCopula
+from copul.families.extreme_value.extreme_value_copula import ExtremeValueCopula
 
 
 class Joe(ExtremeValueCopula):
     psi1, psi2, delta = sympy.symbols("psi1 psi2 delta")
 
     def __init__(self):
         self.pickand = 1 - ((self.psi1 * (1 - self.t)) ** (-self.delta) + (self.psi2 * self.t) ** (-self.delta)) ** (
```

### Comparing `copul-0.0.1/copul/calculations/copulas/families/extreme_value/marshall_olkin.py` & `copul-0.0.2/copul/families/extreme_value/marshall_olkin.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 import sympy
 
-from copul.calculations.copulas.families.extreme_value.extreme_value_copula import ExtremeValueCopula
+from copul.families.extreme_value.extreme_value_copula import ExtremeValueCopula
 
 
 class MarshallOlkin(ExtremeValueCopula):
     alpha1, alpha2 = sympy.symbols("alpha1 alpha2")
 
     def __init__(self):
         self.pickand = sympy.Max(1 - self.alpha1 * (1 - self.t), 1 - self.alpha2 * (1 - self.t))
```

### Comparing `copul-0.0.1/copul/calculations/copulas/families/extreme_value/t_ev.py` & `copul-0.0.2/copul/families/extreme_value/t_ev.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import numpy as np
 import sympy
 from sympy import stats
 
-from copul.calculations.copulas.families.extreme_value.extreme_value_copula import ExtremeValueCopula
+from copul.families.extreme_value.extreme_value_copula import ExtremeValueCopula
 
 
 # noinspection PyPep8Naming
 class tEV(ExtremeValueCopula):
     nu, rho = sympy.symbols("nu rho")
 
     def __init__(self):
```

### Comparing `copul-0.0.1/copul/calculations/copulas/families/extreme_value/tawn.py` & `copul-0.0.2/copul/families/extreme_value/tawn.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 import numpy as np
 import sympy
 
-from copul.calculations.copulas.families.extreme_value.extreme_value_copula import ExtremeValueCopula
+from copul.families.extreme_value.extreme_value_copula import ExtremeValueCopula
 
 
 class Tawn(ExtremeValueCopula):
     psi1, psi2, theta = sympy.symbols("psi1 psi2 theta")
 
     def __init__(self):
         self.pickand = (1 - self.psi1) * (1 - self.t) + (1 - self.psi2) * self.t \
```

### Comparing `copul-0.0.1/copul/calculations/copulas/families/other/farlie_gumbell_morgenstern.py` & `copul-0.0.2/copul/families/other/farlie_gumbell_morgenstern.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,19 +1,27 @@
 import sympy
 
-from copul.calculations.copulas import abstract_copula
-from copul.calculations.copulas.abstract_copula import AbstractCopula
+from copul.families import abstract_copula
+from copul.families.abstract_copula import AbstractCopula
 
 
 class FarlieGumbellMorgenstern(AbstractCopula):
     theta = sympy.symbols("theta", positive=True)
 
     def cdf(self):
         return self.u*self.v + self.theta*self.u*self.v*(1 - self.u)*(1 - self.v)
 
+    @property
+    def spearmans_rho(self):
+        return self.theta/3
+
+    @property
+    def kendalls_tau(self):
+        return 2*self.theta/9
+
 
 if __name__ == "__main__":
     farlie = FarlieGumbellMorgenstern()
     cdf = farlie.cdf
     pdf = farlie.log_pdf
     diff = sympy.simplify(sympy.diff(cdf, farlie.v))
     diff2 = sympy.simplify(sympy.diff(diff, farlie.v))
```

### Comparing `copul-0.0.1/copul/calculations/copulas/families/other/plackett.py` & `copul-0.0.2/copul/families/other/plackett.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,17 +1,30 @@
 import sympy
 
-from copul.calculations.copulas.abstract_copula import AbstractCopula
+from copul.families import get_simplified_solution
+from copul.families.abstract_copula import AbstractCopula
+from copul.sympy_wrapper import SymPyFunctionWrapper
 
 
 class Plackett(AbstractCopula):
-    theta = sympy.symbols("x", positive=True)
+    theta = sympy.symbols("theta", positive=True)
 
+    @property
     def cdf(self):
-        return (1+(self.theta - 1)*(self.u + self.v) - sympy.sqrt((1+(self.theta-1)*(self.u+self.v))**2 - 4*self.u*self.v*self.theta*(self.theta - 1)))/(2*(self.theta - 1))
+        cdf = (1+(self.theta - 1)*(self.u + self.v) - sympy.sqrt((1+(self.theta-1)*(self.u+self.v))**2 - 4*self.u*self.v*self.theta*(self.theta - 1)))/(2*(self.theta - 1))
+        return SymPyFunctionWrapper(get_simplified_solution(cdf))
+
+    @property
+    def pdf(self):
+        pdf = sympy.diff(self.cdf.func, self.u, self.v)
+        return SymPyFunctionWrapper(get_simplified_solution(pdf))
+
+    @property
+    def spearmans_rho(self):
+        return (self.theta+1)/(self.theta-1) - 4*self.theta*sympy.log(self.theta)/(self.theta-1)**2
 
     def get_density_of_density(self):
         # D_vu(pdf)
         return (-((2*self.u*self.theta - 2*self.u - self.theta + 1)*
                   (self.u**2*self.theta**2 - 2*self.u**2*self.theta + self.u**2
                    - 2*self.u*self.v*self.theta**2 + 2*self.u*self.v + 2*self.u*self.theta
                    - 2*self.u + self.v**2*self.theta**2 - 2*self.v**2*self.theta
@@ -88,16 +101,10 @@
                             -2 * self.u * self.v * self.theta + 2 * self.u * self.v + self.u * self.theta - self.u + self.v * self.theta - self.v + 1) * (
                             self.u ** 2 * self.theta ** 2 - 2 * self.u ** 2 * self.theta + self.u ** 2 - 2 * self.u * self.v * self.theta ** 2 + 2 * self.u * self.v + 2 * self.u * self.theta - 2 * self.u + self.v ** 2 * self.theta ** 2 - 2 * self.v ** 2 * self.theta + self.v ** 2 + 2 * self.v * self.theta - 2 * self.v + 1))
 
 
 if __name__ == "__main__":
     plackett = Plackett()
     cdf = plackett.cdf()
-    # pdf = plackett.get_log_pdf()
     explicit_num = plackett.get_numerator_double_density()
     print(str(sympy.expand_mul(explicit_num)).replace("**", "^"))
-    # diff = sympy.simplify(sympy.diff(cdf, plackett.v))
-    # diff2 = sympy.simplify(sympy.diff(diff, plackett.v))
-    # print(sympy.latex(diff2))
-    # special_diff = abstract_copula.round_expression(diff.subs(plackett.u, 0.5))
-    # sympy.plot(special_diff.subs(plackett.theta, 2))
     exit()
```

### Comparing `copul-0.0.1/pyproject.toml` & `copul-0.0.2/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,40 +1,40 @@
 [build-system]
 requires = [
     "build",
     "setuptools>=61.0",
+    "twine",
     "wheel",
 ]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "copul"
-version = "0.0.1"
+version = "0.0.2"
 authors = [
   { name="Marcus Rockel", email="marcus.rockel@finance.uni-freiburg.de" },
   { name="Eva Lütkebohmert-Holtz", email="eva.luetkebohmert@finance.uni-freiburg.de" },
   { name="Jonathan Ansari", email="jonathan.ansari@plus.ac.at" },
 ]
 description = "Risk analysis with copulas."
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
     "Programming Language :: Python :: 3",
     "Operating System :: OS Independent",
 ]
 dependencies = [
     "interval",
-    "matplotlib>=3.7.1",
-    "numpy>=1.24.2",
-    "pandas>=1.5.3",
+    "matplotlib>=3.6.0",
+    "numpy>=1.21.0",
+    "pandas>=1.4.4",
     "pillow>=9.4.0",
-    "scipy>=1.10.1",
-    "statsmodels",
+    "scipy>=1.8.0",
     "sympy",
-    "sympy_plot_backends",
+    "sympy_plot_backends>=1.6.0",
 ]
 
 [project.urls]
 "Homepage" = "https://github.com/Corrram/copulas_in_systemic_risk"
 
 [tool.setuptools.package-data]
 copul = ["docs/*"]
```

