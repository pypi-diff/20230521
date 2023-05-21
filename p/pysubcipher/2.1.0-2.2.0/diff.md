# Comparing `tmp/pysubcipher-2.1.0.tar.gz` & `tmp/pysubcipher-2.2.0.tar.gz`

## Comparing `pysubcipher-2.1.0.tar` & `pysubcipher-2.2.0.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rw-r--r--   0        0        0      549 2020-02-02 00:00:00.000000 pysubcipher-2.1.0/src/pysubcipher/__init__.py
--rw-r--r--   0        0        0    10370 2020-02-02 00:00:00.000000 pysubcipher-2.1.0/src/pysubcipher/pysubcipher.py
--rw-r--r--   0        0        0     1089 2020-02-02 00:00:00.000000 pysubcipher-2.1.0/LICENSE
--rw-r--r--   0        0        0     7884 2020-02-02 00:00:00.000000 pysubcipher-2.1.0/README.md
--rw-r--r--   0        0        0      586 2020-02-02 00:00:00.000000 pysubcipher-2.1.0/pyproject.toml
--rw-r--r--   0        0        0     8161 2020-02-02 00:00:00.000000 pysubcipher-2.1.0/PKG-INFO
+-rw-r--r--   0        0        0     1830 2020-02-02 00:00:00.000000 pysubcipher-2.2.0/src/pysubcipher/__init__.py
+-rw-r--r--   0        0        0    11647 2020-02-02 00:00:00.000000 pysubcipher-2.2.0/src/pysubcipher/pysubcipher.py
+-rw-r--r--   0        0        0     1089 2020-02-02 00:00:00.000000 pysubcipher-2.2.0/LICENSE
+-rw-r--r--   0        0        0     8051 2020-02-02 00:00:00.000000 pysubcipher-2.2.0/README.md
+-rw-r--r--   0        0        0      577 2020-02-02 00:00:00.000000 pysubcipher-2.2.0/pyproject.toml
+-rw-r--r--   0        0        0     8315 2020-02-02 00:00:00.000000 pysubcipher-2.2.0/PKG-INFO
```

### Comparing `pysubcipher-2.1.0/src/pysubcipher/pysubcipher.py` & `pysubcipher-2.2.0/src/pysubcipher/pysubcipher.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import base64
 import string
 import random
 import pickle
 import io
 import os
 
-from .__init__ import HEXDIGITS
+from .__init__ import HEXDIGITS, PRINTABLE
 
 from typing import Any
 
 class InvalidCharacterError(ValueError):
     def __init__(self, character: str, /) -> None:
         """Raised if an invalid token is present within a string of text while encrypting or decrypting a value.
 
@@ -31,26 +31,26 @@
 
 class InvalidKeysError(ValueError):
     def __init__(self) -> None:
         """Raised if invalid keys are loaded into a SubstitutionCipher instance."""
         super().__init__(f"Cipher keys failed validation")
 
 class _EncryptionKeys():
-    def __init__(self, __min_length: int, __max_length: int, /, *, seed: Any, charset: str) -> None:
+    def __init__(self, __min_length: int, __max_length: int, /, *, seed: int | float | str | bytes | bytearray | None, charset: str) -> None:
         """Generates a pair of encryption and decryption keys.
 
         Args:
             __min_length (int): The minimum length of a key.
             __max_length (int): The maximum length of a key.
-            seed (Any): The random seed that keys will be generated with.
+            seed (int | float | str | bytes | bytearray | None): The random seed that keys will be generated with.
             charset (str): The character set to generate keys with.
         """
         self.__min_length: int = __min_length
         self.__max_length: int = __max_length
-        self.__seed: Any = seed
+        self.__seed: int | float | str | bytes | bytearray | None = seed
         self.__charset: str = charset
         self._encryption_keys: dict[bytes, str] | None = None
         self._decryption_keys: dict[str, bytes] | None = None
         self.__generate_keys(seed = self.__seed)
 
     def __generate_keys(self, *, seed: bytes) -> None:
         """
@@ -60,32 +60,32 @@
             seed (bytes): The random seed to generate keys with.
         """
         random.seed(seed)
         encryption_keys: dict[bytes, str] = {}
         decryption_keys: dict[str, bytes] = {}
         characters = self.__charset
 
-        for character in string.printable:
+        for character in PRINTABLE:
             key = ''.join([random.choice(characters) for _ in range(random.randint(self.__min_length, self.__max_length))])
             __char = base64.b64encode(character.encode().hex().encode())
             encryption_keys[__char] = key
             decryption_keys[key] = __char
 
         self._encryption_keys = encryption_keys
         self._decryption_keys = decryption_keys
         random.seed(None)
 
 class SubstitutionCipher(_EncryptionKeys):
-    def __init__(self, min_key_length: int = 10, max_key_length: int = 20, *, seed: Any | None = os.urandom(1024), charset: str = HEXDIGITS) -> None:
-        """A simple substitution cipher encryption tool to encode strings of text.
+    def __init__(self, min_key_length: int = 10, max_key_length: int = 20, *, seed: int | float | str | bytes | bytearray | None | None = os.urandom(1024), charset: str = HEXDIGITS) -> None:
+        """A simple substitution cipher encryption tool to encrypt strings of text.
 
         Args:
             min_key_length (int): The minimum length of a cipher key.
             max_key_length (int): The maximum length of a cipher key.
-            seed (Any | None, optional): The seed that cipher keys will be generated with. Defaults to os.urandom(1024).
+            seed (int | float | str | bytes | bytearray | None, optional): The seed that cipher keys will be generated with. Defaults to os.urandom(1024).
             charset (str, optional): The character set that cipher keys will be generated with. Defaults to HEXDIGITS.
         """
         self.__min_key_length: int = min_key_length
         self.__max_key_length: int = max_key_length
         self.__charset: str = charset
         if not isinstance(charset, str):
             raise TypeError(f"Parameter charset cannot be of type {type(charset)}")
@@ -132,21 +132,28 @@
                     __decrypted_string.write(bytearray.fromhex(base64.b64decode(self._decryption_keys[k].decode()).decode()).decode())
                     s = s[len(k):]
                     __match = True
                     break
             if not __match:
                 raise EncryptedStringInvalidError(s.decode())
         return __decrypted_string.getvalue().encode()
-    def set_seed(self, seed: Any, /) -> None:
+    def set_seed(self, seed: int | float | str | bytes | bytearray | None, /) -> None:
         """Sets the random seed for cipher keys to be generated with.
 
         Args:
-            seed (Any): The seed to override.
+            seed (int | float | str | bytes | bytearray | None): The seed to override.
         """
         super().__init__(self.__min_key_length, self.__max_key_length, seed = seed, charset = self.__charset)
+    def regenerate_keys(self, seed: int | float | str | bytes | bytearray | None = os.urandom(1024), /) -> None:
+        """Regenerates encryption and decryption keys.
+
+        Args:
+            seed (int | float | str | bytes | bytearray | None, optional): The seed to generate cipher keys with. Defaults to os.urandom(1024).
+        """
+        self.set_seed(seed)
     def __test_keys(self, encryption_keys: Any, decryption_keys: Any) -> bool:
         """Tests and validates cipher keys.
 
         Args:
             encryption_keys (Any): The encryption keys to validate.
             decryption_keys (Any): The decryption keys to validate.
 
@@ -194,18 +201,26 @@
             if result:
                 self._encryption_keys = encryption_keys
                 self._decryption_keys = decryption_keys
             else:
                 raise InvalidKeysError()
 
 class FileSubstitutionCipher(SubstitutionCipher):
-    def __init__(self, min_key_length: int = 10, max_key_length: int = 20, *, seed: Any | None = os.urandom(1024), charset: str = HEXDIGITS) -> None:
+    def __init__(self, min_key_length: int = 10, max_key_length: int = 20, *, seed: int | float | str | bytes | bytearray | None = os.urandom(1024), charset: str = HEXDIGITS) -> None:
+        """A simple substitution cipher encryption tool to encrypt file's and their contents.
+
+        Args:
+            min_key_length (int): The minimum length of a cipher key.
+            max_key_length (int): The maximum length of a cipher key.
+            seed (int | float | str | bytes | bytearray | None, optional): The seed that cipher keys will be generated with. Defaults to os.urandom(1024).
+            charset (str, optional): The character set that cipher keys will be generated with. Defaults to HEXDIGITS.
+        """
         self.__min_key_length: int = min_key_length
         self.__max_key_length: int = max_key_length
-        self.__seed: Any = seed
+        self.__seed: int | float | str | bytes | bytearray | None = seed
         self.__charset: str = charset
         super().__init__(self.__min_key_length, self.__max_key_length, seed = self.__seed, charset = self.__charset)
     def encrypt(self, filepath: str, /, *, write: bool = False) -> bytes | None:
         """Encrypts the contents of a file and returns the encrypted contents.
 
         Args:
             filepath (str): The path to the file that will be encrypted.
```

### Comparing `pysubcipher-2.1.0/LICENSE` & `pysubcipher-2.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `pysubcipher-2.1.0/README.md` & `pysubcipher-2.2.0/README.md`

 * *Files 7% similar despite different names*

```diff
@@ -2,15 +2,14 @@
 ![SupportedVersions]
 ![License]
 
 [PyPiVersion]: https://img.shields.io/pypi/v/pysubcipher
 [SupportedVersions]: https://img.shields.io/badge/python-3.9%20%7C%203.10%20%7C%203.11-orange
 [License]: https://img.shields.io/badge/license-MIT-yellow
 
-# `pysubcipher==2.1.0`
 `pysubcipher` is a python module built on `Python 3.10` which allows users to encrypt and decrypt strings of text using a substitution cipher algorithm.
 
 # Installation
 Tested on Python 3.9 and above.<br>
 No requirements apart from the standard module.
 ```py
 pip install pysubcipher
@@ -41,24 +40,24 @@
 ### Output
 ```py
 b'e41BF3d8ebD5c0F34D2ce0caC5FCD2fbFAc576aB91bFAc576aB91E38cD3Da83deCEa8eeafc5AD23FC63Bacc983cBBFe02D4eAb46DeCaabd4E5Dda1E38cD3Da83deCEa8eeaDa487daD01Afe0abFAc576aB91F557edbaBe4e6052F0B41C11184'
 b'Hello, World!'
 ```
 # SubstitutionCipher
 ```py
-def __init__(self, min_key_length: int = 10, max_key_length: int = 20, *, seed: Any | None = os.urandom(1024), charset: str = HEXDIGITS) -> None:
+def __init__(self, min_key_length: int = 10, max_key_length: int = 20, *, seed: int | float | str | bytes | bytearray | None = os.urandom(1024), charset: str = HEXDIGITS) -> None:
     ...
 ```
 ```py
 """A simple substitution cipher encryption tool to encode strings of text.
 
 Args:
     min_key_length (int): The minimum length of a cipher key
     max_key_length (int): The maximum length of a cipher key
-    seed (Any | None, optional): The seed that cipher keys will be generated with. Defaults to os.urandom(1024).
+    seed (int | float | str | bytes | bytearray | None, optional): The seed that cipher keys will be generated with. Defaults to os.urandom(1024).
     charset (str, optional): The character set that cipher keys will be generated with. Defaults to HEXDIGITS.
 """
 ```
 # Using built-in character sets
 - BASE_2
 - HEXDIGITS
 - OCTDIGITS
@@ -117,15 +116,15 @@
 ```
 ```py
 from pysubcipher import SubstitutionCipher
 
 subcipher = SubstitutionCipher()
 subcipher.save_keys("cipher_keys.dat")
 ```
-# Loading keys into a SubstitutionCipher instance
+# Loading saved keys from a file
 ```py
 """Loads cipher keys into the instance
 
 Args:
     file (str): The path to the file where the keys are stored
 
 Raises:
@@ -135,21 +134,37 @@
 ```py
 from pysubcipher import SubstitutionCipher
 
 subcipher = SubstitutionCipher()
 subcipher.load_keys("cipher_keys.dat")
 ```
 # Setting a custom seed
-If you don't intend on storing cipher keys in a file, you can always use a set seed so the cipher keys are the same every time. Seeds will always be generated upon creating a new instance of the SubstitutionCipher class and will be set to `os.urandom(1024)`.
+```py
+def set_seed(self, seed: int | float | str | bytes | bytearray | None, /) -> None:
+    ...
+```
+If you don't intend on storing cipher keys in a file, you can always use a set seed so the cipher keys are the same every time you run your program.
 ```py
 from pysubcipher import SubstitutionCipher
 
 subcipher = SubstitutionCipher()
 subcipher.set_seed("my_amazing_seed")
 ```
+# Regenerating cipher keys
+```py
+def regenerate_keys(self, seed: int | float | str | bytes | bytearray | None | None = None, /) -> None:
+    ...
+```
+```py
+"""Regenerates encryption and decryption keys.
+
+Args:
+    seed (int | float | str | bytes | bytearray | None, optional): The seed to generate cipher keys with. Defaults to os.urandom(1024).
+"""
+```
 # Encrypting and decrypting a file
 The `FileSubstitutionCipher` class can be used to encrypt and decrypt files easily.
 ### Encrypting
 ```py
 def encrypt(self, filepath: str, /, *, write: bool = False) -> bytes | None:
     ...
 ```
@@ -210,17 +225,15 @@
 
 # Exceptions and error handling
 ## `InvalidCharacterError`
 ```py
 def __init__(self, character: str, /) -> None:
     ...
 ```
-Raised if an invalid token is present within a string of text while encrypting or decrypting a value.<br><br>
-**Note: `pysubcipher==2.1.0` currently only supports the following characters:**<br>
-<code>0123456789abcdefghijklmnopqrstuvwxyzABCDEFGHIJKLMNOPQRSTUVWXYZ!"#$%&\'()*+,-./:;<=>?@[\\]^_`{|}~ \t\n\r\x0b\x0c</code>
+Raised if an invalid token is present within a string of text while encrypting or decrypting a value.
 
 ## `EncryptedStringInvalidError`
 ```py
 def __init__(self, token: str) -> None:
     ...
 ```
 Raised while decrypting a string of text if the encrypted string is not valid or does not match any decryption keys.
```

### Comparing `pysubcipher-2.1.0/pyproject.toml` & `pysubcipher-2.2.0/pyproject.toml`

 * *Files 22% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "pysubcipher"
-version = "2.1.0"
+version = "2.2.0"
 authors = [
-  { name="mxngo", email="" },
+  {name = "mxngo", email = ""}
 ]
 description = "pysubcipher allows for simple encryption and decryption of text using a basic substitution cipher algorithm."
 readme = "README.md"
 requires-python = ">=3.9"
 classifiers = [
-    "Development Status :: 3 - Alpha",
-    "Topic :: Security :: Cryptography",
-    "Programming Language :: Python :: 3",
-    "License :: OSI Approved :: MIT License",
-    "Operating System :: OS Independent"
+  "Development Status :: 3 - Alpha",
+  "Topic :: Security :: Cryptography",
+  "Programming Language :: Python :: 3",
+  "License :: OSI Approved :: MIT License",
+  "Operating System :: OS Independent"
 ]
```

### Comparing `pysubcipher-2.1.0/PKG-INFO` & `pysubcipher-2.2.0/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pysubcipher
-Version: 2.1.0
+Version: 2.2.0
 Summary: pysubcipher allows for simple encryption and decryption of text using a basic substitution cipher algorithm.
 Author: mxngo
 License-File: LICENSE
 Classifier: Development Status :: 3 - Alpha
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
@@ -16,15 +16,14 @@
 ![SupportedVersions]
 ![License]
 
 [PyPiVersion]: https://img.shields.io/pypi/v/pysubcipher
 [SupportedVersions]: https://img.shields.io/badge/python-3.9%20%7C%203.10%20%7C%203.11-orange
 [License]: https://img.shields.io/badge/license-MIT-yellow
 
-# `pysubcipher==2.1.0`
 `pysubcipher` is a python module built on `Python 3.10` which allows users to encrypt and decrypt strings of text using a substitution cipher algorithm.
 
 # Installation
 Tested on Python 3.9 and above.<br>
 No requirements apart from the standard module.
 ```py
 pip install pysubcipher
@@ -55,24 +54,24 @@
 ### Output
 ```py
 b'e41BF3d8ebD5c0F34D2ce0caC5FCD2fbFAc576aB91bFAc576aB91E38cD3Da83deCEa8eeafc5AD23FC63Bacc983cBBFe02D4eAb46DeCaabd4E5Dda1E38cD3Da83deCEa8eeaDa487daD01Afe0abFAc576aB91F557edbaBe4e6052F0B41C11184'
 b'Hello, World!'
 ```
 # SubstitutionCipher
 ```py
-def __init__(self, min_key_length: int = 10, max_key_length: int = 20, *, seed: Any | None = os.urandom(1024), charset: str = HEXDIGITS) -> None:
+def __init__(self, min_key_length: int = 10, max_key_length: int = 20, *, seed: int | float | str | bytes | bytearray | None = os.urandom(1024), charset: str = HEXDIGITS) -> None:
     ...
 ```
 ```py
 """A simple substitution cipher encryption tool to encode strings of text.
 
 Args:
     min_key_length (int): The minimum length of a cipher key
     max_key_length (int): The maximum length of a cipher key
-    seed (Any | None, optional): The seed that cipher keys will be generated with. Defaults to os.urandom(1024).
+    seed (int | float | str | bytes | bytearray | None, optional): The seed that cipher keys will be generated with. Defaults to os.urandom(1024).
     charset (str, optional): The character set that cipher keys will be generated with. Defaults to HEXDIGITS.
 """
 ```
 # Using built-in character sets
 - BASE_2
 - HEXDIGITS
 - OCTDIGITS
@@ -131,15 +130,15 @@
 ```
 ```py
 from pysubcipher import SubstitutionCipher
 
 subcipher = SubstitutionCipher()
 subcipher.save_keys("cipher_keys.dat")
 ```
-# Loading keys into a SubstitutionCipher instance
+# Loading saved keys from a file
 ```py
 """Loads cipher keys into the instance
 
 Args:
     file (str): The path to the file where the keys are stored
 
 Raises:
@@ -149,21 +148,37 @@
 ```py
 from pysubcipher import SubstitutionCipher
 
 subcipher = SubstitutionCipher()
 subcipher.load_keys("cipher_keys.dat")
 ```
 # Setting a custom seed
-If you don't intend on storing cipher keys in a file, you can always use a set seed so the cipher keys are the same every time. Seeds will always be generated upon creating a new instance of the SubstitutionCipher class and will be set to `os.urandom(1024)`.
+```py
+def set_seed(self, seed: int | float | str | bytes | bytearray | None, /) -> None:
+    ...
+```
+If you don't intend on storing cipher keys in a file, you can always use a set seed so the cipher keys are the same every time you run your program.
 ```py
 from pysubcipher import SubstitutionCipher
 
 subcipher = SubstitutionCipher()
 subcipher.set_seed("my_amazing_seed")
 ```
+# Regenerating cipher keys
+```py
+def regenerate_keys(self, seed: int | float | str | bytes | bytearray | None | None = None, /) -> None:
+    ...
+```
+```py
+"""Regenerates encryption and decryption keys.
+
+Args:
+    seed (int | float | str | bytes | bytearray | None, optional): The seed to generate cipher keys with. Defaults to os.urandom(1024).
+"""
+```
 # Encrypting and decrypting a file
 The `FileSubstitutionCipher` class can be used to encrypt and decrypt files easily.
 ### Encrypting
 ```py
 def encrypt(self, filepath: str, /, *, write: bool = False) -> bytes | None:
     ...
 ```
@@ -224,17 +239,15 @@
 
 # Exceptions and error handling
 ## `InvalidCharacterError`
 ```py
 def __init__(self, character: str, /) -> None:
     ...
 ```
-Raised if an invalid token is present within a string of text while encrypting or decrypting a value.<br><br>
-**Note: `pysubcipher==2.1.0` currently only supports the following characters:**<br>
-<code>0123456789abcdefghijklmnopqrstuvwxyzABCDEFGHIJKLMNOPQRSTUVWXYZ!"#$%&\'()*+,-./:;<=>?@[\\]^_`{|}~ \t\n\r\x0b\x0c</code>
+Raised if an invalid token is present within a string of text while encrypting or decrypting a value.
 
 ## `EncryptedStringInvalidError`
 ```py
 def __init__(self, token: str) -> None:
     ...
 ```
 Raised while decrypting a string of text if the encrypted string is not valid or does not match any decryption keys.
```

