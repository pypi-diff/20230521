# Comparing `tmp/pysubcipher-2.0.0.tar.gz` & `tmp/pysubcipher-2.0.1.tar.gz`

## Comparing `pysubcipher-2.0.0.tar` & `pysubcipher-2.0.1.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rw-r--r--   0        0        0      348 2020-02-02 00:00:00.000000 pysubcipher-2.0.0/src/pysubcipher/__init__.py
--rw-r--r--   0        0        0     5909 2020-02-02 00:00:00.000000 pysubcipher-2.0.0/src/pysubcipher/pysubcipher.py
--rw-r--r--   0        0        0     1089 2020-02-02 00:00:00.000000 pysubcipher-2.0.0/LICENSE
--rw-r--r--   0        0        0     5079 2020-02-02 00:00:00.000000 pysubcipher-2.0.0/README.md
--rw-r--r--   0        0        0      495 2020-02-02 00:00:00.000000 pysubcipher-2.0.0/pyproject.toml
--rw-r--r--   0        0        0     5401 2020-02-02 00:00:00.000000 pysubcipher-2.0.0/PKG-INFO
+-rw-r--r--   0        0        0      549 2020-02-02 00:00:00.000000 pysubcipher-2.0.1/src/pysubcipher/__init__.py
+-rw-r--r--   0        0        0     7955 2020-02-02 00:00:00.000000 pysubcipher-2.0.1/src/pysubcipher/pysubcipher.py
+-rw-r--r--   0        0        0     1089 2020-02-02 00:00:00.000000 pysubcipher-2.0.1/LICENSE
+-rw-r--r--   0        0        0     4726 2020-02-02 00:00:00.000000 pysubcipher-2.0.1/README.md
+-rw-r--r--   0        0        0      495 2020-02-02 00:00:00.000000 pysubcipher-2.0.1/pyproject.toml
+-rw-r--r--   0        0        0     4997 2020-02-02 00:00:00.000000 pysubcipher-2.0.1/PKG-INFO
```

### Comparing `pysubcipher-2.0.0/src/pysubcipher/pysubcipher.py` & `pysubcipher-2.0.1/src/pysubcipher/pysubcipher.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,8 +1,17 @@
-import base64, string, random, io, os
+import base64
+import string
+import random
+import pickle
+import io
+import os
+
+from .__init__ import HEXDIGITS
+
+from typing import Any
 
 class InvalidTokenFoundError(Exception):
     def __init__(self, character: str | None = None, /) -> None:
         """Raised if an invalid character or token is present within a string of text
         during the encryption / decryption phase.
 
         Args:
@@ -10,98 +19,70 @@
         """
         if character is None:
             super().__init__()
         else:
             super().__init__(f"Invalid token \"{character}\" is not defined as printable.")
 
 class _EncryptionKeys():
-    def __init__(self, __min_length: int, __max_length: int, /) -> None:
+    def __init__(self, __min_length: int, __max_length: int, /, *, seed: Any, charset: str) -> None:
         """Generates a pair of encryption and decryption keys at a desired length.
 
         Args:
-            __min_length (int, optional): The minimum length that a key should stand.
-            __max_length (int, optional): The maximum length that a key should stand.
+            __min_length (int): The minimum length of a key
+            __max_length (int): The maximum length of a key
+            seed (Any): The random seed that keys will be generated with
+            charset (str): The character set to generate keys with
         """
         self.__min_length: int = __min_length
         self.__max_length: int = __max_length
+        self.__seed: Any = seed
+        self.__charset: str = charset
         self._encryption_keys: dict[bytes, str] | None = None
         self._decryption_keys: dict[str, bytes] | None = None
-        self.__generate_keys(seed = os.urandom(1024))
+        self.__generate_keys(seed = self.__seed)
 
     def __generate_keys(self, *, seed: bytes) -> None:
         """
         Generates a list of keys bound to a list of characters which are defined in string's printable character list.
         Valid characters: 0123456789abcdefghijklmnopqrstuvwxyzABCDEFGHIJKLMNOPQRSTUVWXYZ!"#$%&'()*+,-./:;<=>?@[\]^_`{|}~
 
         Args:
             seed (bytes): The random seed to generate keys on.
         """
         random.seed(seed)
         encryption_keys: dict[bytes, str] = {}
         decryption_keys: dict[str, bytes] = {}
-        characters = string.hexdigits
+        characters = self.__charset
 
         for character in string.printable:
             key = ''.join([random.choice(characters) for _ in range(random.randint(self.__min_length, self.__max_length))])
             __char = base64.b64encode(bytes(character.encode().hex(), "UTF-8"))
             encryption_keys[__char] = key
             decryption_keys[key] = __char
 
         self._encryption_keys = encryption_keys
         self._decryption_keys = decryption_keys
         random.seed(None)
 
-class SecurityLevel():
-    def __init__(self, a: int, b: int, /) -> None:
-        """
-        Args:
-            a (int): Minimum key length.
-            b (int): Maximum key length.
-        """
-        self._a: int = a
-        self._b: int = b
-    @classmethod
-    def extremely_low(cls):
-        return cls(10, 15)
-    @classmethod
-    def very_low(cls):
-        return cls(10, 30)
-    @classmethod
-    def low(cls):
-        return cls(30, 75)
-    @classmethod
-    def medium(cls):
-        return cls(75, 150)
-    @classmethod
-    def high(cls):
-        return cls(150, 500)
-    @classmethod
-    def very_high(cls):
-        return cls(500, 1000)
-    @classmethod
-    def extremely_high(cls):
-        return cls(1000, 1500)
-    @classmethod
-    def custom(cls, _min: int, _max: int):
-        if _min > _max:
-            raise ValueError("Maximum key length must be a greater value than minimum key length.")
-        elif _min < 10:
-            raise ValueError("Minimum key length must be greater than or equal to 10.")
-        return cls(_min, _max)
-
 class SubstitutionCipher(_EncryptionKeys):
-    def __init__(self, security_level: SecurityLevel = SecurityLevel.medium()) -> None:
+    def __init__(self, min_key_length: int = 10, max_key_length: int = 20, *, seed: Any | None = os.urandom(1024), charset: str = HEXDIGITS) -> None:
         """A simple substitution cipher encryption tool to encode strings of text.
 
         Args:
-            security_level (SecurityLevel, optional): The security level (length) of each encryption / decryption key. Defaults to SecurityLevel.medium().
-        """
-        if not isinstance(security_level, SecurityLevel):
-            raise TypeError(f"Argument security_level cannot be of type {type(security_level)}")
-        super().__init__(security_level._a, security_level._b)
+            min_key_length (int): The minimum length of a cipher key
+            max_key_length (int): The maximum length of a cipher key
+            seed (Any | None, optional): The seed that cipher keys will be generated with. Defaults to os.urandom(1024).
+            charset (str, optional): The character set that cipher keys will be generated with. Defaults to HEXDIGITS.
+        """
+        self.__min_key_length: int = min_key_length
+        self.__max_key_length: int = max_key_length
+        self.__charset: str = charset
+        if not isinstance(charset, str):
+            raise TypeError(f"Parameter charset cannot be of type {type(charset)}")
+        super().__init__(min_key_length, max_key_length, seed = seed, charset = self.__charset)
     def encrypt(self, s: str, /) -> bytes:
         """Encrypts a string of text using an arrangement of encryption keys.
 
         Args:
             s (str): The string to encrypt.
 
         Raises:
@@ -136,8 +117,65 @@
                 if s.startswith(bytes(k, "UTF-8")):
                     __decrypted_string.write(bytearray.fromhex(base64.b64decode(self._decryption_keys[k].decode()).decode()).decode())
                     s = s[len(k):]
                     __match = True
                     break
             if not __match:
                 raise InvalidTokenFoundError()
-        return bytes(__decrypted_string.getvalue(), "UTF-8")
+        return bytes(__decrypted_string.getvalue(), "UTF-8")
+    def set_seed(self, seed: Any, /) -> None:
+        """Sets the seed that cipher keys will be generated with
+
+        Args:
+            seed (Any): The seed to override
+        """
+        super().__init__(self.__min_key_length, self.__max_key_length, seed = seed, charset = self.__charset)
+    def __test_keys(self, encryption_keys: Any, decryption_keys: Any) -> bool:
+        """Tests and validates encryption and decryption keys and returns if the keys are valid
+
+        Args:
+            encryption_keys (Any): The encryption keys to validate
+            decryption_keys (Any): The decryption keys to validate
+
+        Returns:
+            bool: Returns True if the keys are valid, and False if they are not
+        """
+        text = string.printable
+        cipher = SubstitutionCipher()
+        cipher._encryption_keys = encryption_keys
+        cipher._decryption_keys = decryption_keys
+        encrypted_text = cipher.encrypt(text)
+        decrypted_text = cipher.decrypt(encrypted_text)
+        if decrypted_text.decode() != text:
+            return False
+        return True
+    def save_keys(self, file: str, /, *, truncate: bool = False) -> None:
+        """Saves the current cipher keys to a file
+
+        Args:
+            file (str): The path to the file
+            truncate (bool, optional): If True, the file will be truncated before storing the keys. Defaults to False.
+        """
+        with open(file, "wb") as f:
+            if truncate:
+                f.truncate(0)
+            f.write(pickle.dumps([self._encryption_keys, self._decryption_keys]))
+    def load_keys(self, file: str, /) -> None:
+        """Loads cipher keys into the instance
+
+        Args:
+            file (str): The path to the file where the keys are stored
+
+        Raises:
+            InvalidTokenFoundError: If the keys are not valid, an InvalidTokenFoundError will be raised
+        """
+        with open(file, "rb") as f:
+            contents = f.read()
+            keys = pickle.loads(contents)
+            encryption_keys = keys[0]
+            decryption_keys = keys[1]
+            result: bool = self.__test_keys(encryption_keys, decryption_keys)
+            if result:
+                self._encryption_keys = encryption_keys
+                self._decryption_keys = decryption_keys
+            else:
+                raise InvalidTokenFoundError()
```

### Comparing `pysubcipher-2.0.0/LICENSE` & `pysubcipher-2.0.1/LICENSE`

 * *Files identical despite different names*

