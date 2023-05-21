# Comparing `tmp/readable_number-0.1.2.tar.gz` & `tmp/readable_number-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "readable_number-0.1.2.tar", last modified: Sat May  6 00:47:14 2023, max compression
+gzip compressed data, was "readable_number-0.1.3.tar", last modified: Sun May 21 10:46:31 2023, max compression
```

## Comparing `readable_number-0.1.2.tar` & `readable_number-0.1.3.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 00:47:14.132539 readable_number-0.1.2/
--rw-r--r--   0 runner    (1001) docker     (123)     1061 2023-05-06 00:46:57.000000 readable_number-0.1.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       16 2023-05-06 00:46:57.000000 readable_number-0.1.2/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     3504 2023-05-06 00:47:14.132539 readable_number-0.1.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2833 2023-05-06 00:46:57.000000 readable_number-0.1.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 00:47:14.132539 readable_number-0.1.2/readable_number/
--rw-r--r--   0 runner    (1001) docker     (123)       84 2023-05-06 00:46:57.000000 readable_number-0.1.2/readable_number/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    14705 2023-05-06 00:46:57.000000 readable_number-0.1.2/readable_number/readable_number.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 00:47:14.132539 readable_number-0.1.2/readable_number.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3504 2023-05-06 00:47:14.000000 readable_number-0.1.2/readable_number.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      297 2023-05-06 00:47:14.000000 readable_number-0.1.2/readable_number.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-06 00:47:14.000000 readable_number-0.1.2/readable_number.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       16 2023-05-06 00:47:14.000000 readable_number-0.1.2/readable_number.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      871 2023-05-06 00:47:14.132539 readable_number-0.1.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)       74 2023-05-06 00:46:57.000000 readable_number-0.1.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 00:47:14.132539 readable_number-0.1.2/tests/
--rw-r--r--   0 runner    (1001) docker     (123)    20334 2023-05-06 00:46:57.000000 readable_number-0.1.2/tests/test_readable_number.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 10:46:31.019865 readable_number-0.1.3/
+-rw-r--r--   0 runner    (1001) docker     (123)     1061 2023-05-21 10:46:20.000000 readable_number-0.1.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       16 2023-05-21 10:46:20.000000 readable_number-0.1.3/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     4591 2023-05-21 10:46:31.019865 readable_number-0.1.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3920 2023-05-21 10:46:20.000000 readable_number-0.1.3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 10:46:31.019865 readable_number-0.1.3/readable_number/
+-rw-r--r--   0 runner    (1001) docker     (123)      112 2023-05-21 10:46:20.000000 readable_number-0.1.3/readable_number/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24032 2023-05-21 10:46:20.000000 readable_number-0.1.3/readable_number/readable_number.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 10:46:31.019865 readable_number-0.1.3/readable_number.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4591 2023-05-21 10:46:31.000000 readable_number-0.1.3/readable_number.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      297 2023-05-21 10:46:31.000000 readable_number-0.1.3/readable_number.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-21 10:46:31.000000 readable_number-0.1.3/readable_number.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       16 2023-05-21 10:46:31.000000 readable_number-0.1.3/readable_number.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      871 2023-05-21 10:46:31.019865 readable_number-0.1.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)       74 2023-05-21 10:46:20.000000 readable_number-0.1.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 10:46:31.019865 readable_number-0.1.3/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)    31527 2023-05-21 10:46:20.000000 readable_number-0.1.3/tests/test_readable_number.py
```

### Comparing `readable_number-0.1.2/LICENSE` & `readable_number-0.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `readable_number-0.1.2/PKG-INFO` & `readable_number-0.1.3/README.md`

 * *Files 23% similar despite different names*

```diff
@@ -1,105 +1,152 @@
-Metadata-Version: 2.1
-Name: readable_number
-Version: 0.1.2
-Summary: A Python library to print numbers in human readable format
-Home-page: https://github.com/jsh9/readable-number
-License: MIT
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Programming Language :: Python
-Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.7
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
-Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.11
-Requires-Python: >=3.7
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
 # readable-number
+
 A Python library to print numbers in human readable format
 
 ## 1. Installation
 
 ```
 pip install readable-number
 ```
 
 This library does not depend on any third-party libraries, so installing it will not break your Python environment.
 
 ## 2. Usage
 
+### 2.1. Import and basic usage
+
 ```python
 from readable_number import ReadableNumber
 
-### Print digit in groups
+str(ReadableNumber(-1.23))  # -1.23
+str(ReadableNumber(-123))  # -123
+```
+
+Print many numbers with the same config:
+
+```python
+rn = ReadableNumber(precision=2, digit_group_size=4)
+rn.of(123456789)  # 1,2345,6789
+rn.of(0.123456789)  # 0.12
+rn.of(1e15)  # 1000,0000,0000,0000
+```
+
+### 2.2. Print large integers
+
+#### 2.2.1. Print in groups
+
+```python
 str(ReadableNumber(-123))  # -123
 str(ReadableNumber(-1234))  # -1,234
 str(ReadableNumber(-123456789))  # -123,456,789
 str(ReadableNumber(-12345.6789))  # -12,345.6789
 str(ReadableNumber(-1.23456e18))  # -1,234,560,000,000,000,000
+```
+
+#### 2.2.2. Custom grouping (in locales other than en-US)
 
-### Custom grouping (in other locales)
+```python
 str(ReadableNumber(-123456789, digit_group_size=4))  # -1,2345,6789
 str(ReadableNumber(-123456789, digit_group_delimiter='|'))  # -123|456|789
+```
 
-### Convert to human-readable shortform (with k, M, B, and T as unit)
+#### 2.2.3. Print in shortform
+
+```python
 str(ReadableNumber(12345, use_shortform=True))  # 12k
 str(ReadableNumber(12345, use_shortform=True, precision=1))  # 12.3k
 str(ReadableNumber(12345678, use_shortform=True))  # 12M
 str(ReadableNumber(12345678, use_shortform=True, precision=2))  # 12.35M
+str(ReadableNumber(1234567890, use_shortform=True, precision=2))  # 1.23B
+```
+
+### 2.3. Setting precision or significant figures
+
+#### 2.3.1. Without setting precision or significant figures
+
+Numbers are printed in a "natural" way:
 
-### Numbers with small absolute values
+```python
 str(ReadableNumber(0.12345))  # 0.12345
 str(ReadableNumber(0.0000012345))  # 0.0000012345
+```
+
+#### 2.3.2. Precision
+
+```python
 str(ReadableNumber(0.12345, precision=None))  # 0.12345
 str(ReadableNumber(0.12345, precision=2))  # 0.12
 str(ReadableNumber(0.12345, precision=20))  # 0.123450000000000
+```
 
-### Digits beyond double-precision limit are discarded
-str(ReadableNumber(0.12345678901234567890, precision=90))  # 0.123456789012346
-str(ReadableNumber(1.23e-20, precision=90))  # 0.000000000000000
+#### 2.3.3. Significant figures
 
-### Print many numbers with the same config
-rn = ReadableNumber(precision=2, digit_group_size=4)
-rn.of(123456789)  # 1,2345,6789
-rn.of(0.123456789)  # 0.12
-rn.of(1e15)  # 1000,0000,0000,0000
+```python
+str(ReadableNumber(0.12345, significant_figures_after_decimal_point=3))  # 0.123
+str(ReadableNumber(12345, significant_figures_after_decimal_point=3))  # 12,345
+str(ReadableNumber(0.00012345, significant_figures_after_decimal_point=3))  # 0.000123
+str(ReadableNumber(-1.2345e-50, significant_figures_after_decimal_point=3))
+# -0.0000000000000000000000000000000000000000000000000123
+```
+
+### 2.4. Exponential notations
 
-### Print large numbers in exponantial notation
+#### 2.4.1. Print large numbers in exponential notation
+
+```python
 str(ReadableNumber(1234567890, use_exponent_for_large_numbers=True))  # 1.234568e+09
+
 str(ReadableNumber(
     1234567890,
     use_exponent_for_large_numbers=True,
     precision=2,
 ))  # 1.23e+09
+
 str(ReadableNumber(
     1234567890,
     use_exponent_for_large_numbers=True,
     precision=None,
 ))  # 1.23456789e+09
+
 str(ReadableNumber(
     1234567890,
     use_exponent_for_large_numbers=True,
     large_number_threshold=1e20,  # only show in exp if we exceed this
     precision=None,
 ))  # 1,234,567,890
 
-### Print small numbers in exponential notation
+str(ReadableNumber(
+    1234567890,
+    use_exponent_for_large_numbers=True,
+    large_number_threshold=1e20,  # only show in exp if we exceed this
+    significant_figures_after_decimal_point=5,
+))  # 1.2346e+09
+```
+
+#### 2.4.2. Print small numbers in exponential notation
+
+```python
 str(ReadableNumber(0.000000012, use_exponent_for_small_numbers=True))  # 1.200000e-08
+
 str(ReadableNumber(
     -0.000000123456,
     use_exponent_for_small_numbers=True,
     precision=2,
 ))  # -1.23e-07
+
 str(ReadableNumber(
     -0.000012345,
     use_exponent_for_small_numbers=True,
     precision=None,
     small_number_threshold=1e-2,
 ))  # -1.2345e-05
+
+str(ReadableNumber(
+    -0.00000012345,
+    use_exponent_for_small_numbers=True,
+    significant_figures_after_decimal_point=2,
+))  # -1.23e-07
 ```
 
 ## 3. Full API documentation
 
 Please visit this site: https://readable-number.readthedocs.io/en/stable/
```

### Comparing `readable_number-0.1.2/setup.cfg` & `readable_number-0.1.3/setup.cfg`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = readable_number
-version = v0.1.2
+version = v0.1.3
 description = A Python library to print numbers in human readable format
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://github.com/jsh9/readable-number
 license = MIT
 license_file = LICENSE
 classifiers =
```

