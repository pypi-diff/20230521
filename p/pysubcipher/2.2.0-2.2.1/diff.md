# Comparing `tmp/pysubcipher-2.2.0.tar.gz` & `tmp/pysubcipher-2.2.1.tar.gz`

## Comparing `pysubcipher-2.2.0.tar` & `pysubcipher-2.2.1.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rw-r--r--   0        0        0     1830 2020-02-02 00:00:00.000000 pysubcipher-2.2.0/src/pysubcipher/__init__.py
--rw-r--r--   0        0        0    11647 2020-02-02 00:00:00.000000 pysubcipher-2.2.0/src/pysubcipher/pysubcipher.py
--rw-r--r--   0        0        0     1089 2020-02-02 00:00:00.000000 pysubcipher-2.2.0/LICENSE
--rw-r--r--   0        0        0     8051 2020-02-02 00:00:00.000000 pysubcipher-2.2.0/README.md
--rw-r--r--   0        0        0      577 2020-02-02 00:00:00.000000 pysubcipher-2.2.0/pyproject.toml
--rw-r--r--   0        0        0     8315 2020-02-02 00:00:00.000000 pysubcipher-2.2.0/PKG-INFO
+-rw-r--r--   0        0        0     1830 2020-02-02 00:00:00.000000 pysubcipher-2.2.1/src/pysubcipher/__init__.py
+-rw-r--r--   0        0        0    11647 2020-02-02 00:00:00.000000 pysubcipher-2.2.1/src/pysubcipher/pysubcipher.py
+-rw-r--r--   0        0        0     1089 2020-02-02 00:00:00.000000 pysubcipher-2.2.1/LICENSE
+-rw-r--r--   0        0        0     8005 2020-02-02 00:00:00.000000 pysubcipher-2.2.1/README.md
+-rw-r--r--   0        0        0      577 2020-02-02 00:00:00.000000 pysubcipher-2.2.1/pyproject.toml
+-rw-r--r--   0        0        0     8269 2020-02-02 00:00:00.000000 pysubcipher-2.2.1/PKG-INFO
```

### Comparing `pysubcipher-2.2.0/src/pysubcipher/__init__.py` & `pysubcipher-2.2.1/src/pysubcipher/__init__.py`

 * *Files identical despite different names*

### Comparing `pysubcipher-2.2.0/src/pysubcipher/pysubcipher.py` & `pysubcipher-2.2.1/src/pysubcipher/pysubcipher.py`

 * *Files identical despite different names*

### Comparing `pysubcipher-2.2.0/LICENSE` & `pysubcipher-2.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `pysubcipher-2.2.0/README.md` & `pysubcipher-2.2.1/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -80,15 +80,15 @@
 ```py
 b'100001111110110000010100001011011110101010100010110111101010101001111001011010110111000110100100000011110100010010001000001001111001011000001111001111101010110111101010101001111101101101001111001001010'
 b'Hello, World!'
 ```
 # Using a custom character set
 Character sets are provided as strings of text, and will be used to generate cipher keys.
 
-**Note: if the character set is not unique enough, an InvalidTokenFoundError will be raised as there would not be enough possible combinations to encrypt that string of text.**
+**Note: if the character set is not unique enough, an exception will be raised as there would not be enough possible combinations to encrypt that string of text.**
 For example, if you wanted to use BASE_2 as your character set, but only allowed for the minimum key length to be 3 and the maximum key length to be 4, there would not be enough combinations to account for the entirety of the string.
 ```py
 from pysubcipher import SubstitutionCipher
 
 subcipher = SubstitutionCipher(charset = "abcde1234")
 
 my_text = "Hello, World!"
@@ -124,15 +124,15 @@
 ```py
 """Loads cipher keys into the instance
 
 Args:
     file (str): The path to the file where the keys are stored
 
 Raises:
-    InvalidTokenFoundError: If the keys are not valid, an InvalidTokenFoundError will be raised
+    InvalidKeysError: Raised if the cipher keys are not valid.
 """
 ```
 ```py
 from pysubcipher import SubstitutionCipher
 
 subcipher = SubstitutionCipher()
 subcipher.load_keys("cipher_keys.dat")
```

### Comparing `pysubcipher-2.2.0/pyproject.toml` & `pysubcipher-2.2.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "pysubcipher"
-version = "2.2.0"
+version = "2.2.1"
 authors = [
   {name = "mxngo", email = ""}
 ]
 description = "pysubcipher allows for simple encryption and decryption of text using a basic substitution cipher algorithm."
 readme = "README.md"
 requires-python = ">=3.9"
 classifiers = [
```

### Comparing `pysubcipher-2.2.0/PKG-INFO` & `pysubcipher-2.2.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pysubcipher
-Version: 2.2.0
+Version: 2.2.1
 Summary: pysubcipher allows for simple encryption and decryption of text using a basic substitution cipher algorithm.
 Author: mxngo
 License-File: LICENSE
 Classifier: Development Status :: 3 - Alpha
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
@@ -94,15 +94,15 @@
 ```py
 b'100001111110110000010100001011011110101010100010110111101010101001111001011010110111000110100100000011110100010010001000001001111001011000001111001111101010110111101010101001111101101101001111001001010'
 b'Hello, World!'
 ```
 # Using a custom character set
 Character sets are provided as strings of text, and will be used to generate cipher keys.
 
-**Note: if the character set is not unique enough, an InvalidTokenFoundError will be raised as there would not be enough possible combinations to encrypt that string of text.**
+**Note: if the character set is not unique enough, an exception will be raised as there would not be enough possible combinations to encrypt that string of text.**
 For example, if you wanted to use BASE_2 as your character set, but only allowed for the minimum key length to be 3 and the maximum key length to be 4, there would not be enough combinations to account for the entirety of the string.
 ```py
 from pysubcipher import SubstitutionCipher
 
 subcipher = SubstitutionCipher(charset = "abcde1234")
 
 my_text = "Hello, World!"
@@ -138,15 +138,15 @@
 ```py
 """Loads cipher keys into the instance
 
 Args:
     file (str): The path to the file where the keys are stored
 
 Raises:
-    InvalidTokenFoundError: If the keys are not valid, an InvalidTokenFoundError will be raised
+    InvalidKeysError: Raised if the cipher keys are not valid.
 """
 ```
 ```py
 from pysubcipher import SubstitutionCipher
 
 subcipher = SubstitutionCipher()
 subcipher.load_keys("cipher_keys.dat")
```

