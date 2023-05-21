# Comparing `tmp/pysubcipher-2.0.1.tar.gz` & `tmp/pysubcipher-2.1.0.tar.gz`

## Comparing `pysubcipher-2.0.1.tar` & `pysubcipher-2.1.0.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rw-r--r--   0        0        0      549 2020-02-02 00:00:00.000000 pysubcipher-2.0.1/src/pysubcipher/__init__.py
--rw-r--r--   0        0        0     7955 2020-02-02 00:00:00.000000 pysubcipher-2.0.1/src/pysubcipher/pysubcipher.py
--rw-r--r--   0        0        0     1089 2020-02-02 00:00:00.000000 pysubcipher-2.0.1/LICENSE
--rw-r--r--   0        0        0     4726 2020-02-02 00:00:00.000000 pysubcipher-2.0.1/README.md
--rw-r--r--   0        0        0      495 2020-02-02 00:00:00.000000 pysubcipher-2.0.1/pyproject.toml
--rw-r--r--   0        0        0     4997 2020-02-02 00:00:00.000000 pysubcipher-2.0.1/PKG-INFO
+-rw-r--r--   0        0        0      549 2020-02-02 00:00:00.000000 pysubcipher-2.1.0/src/pysubcipher/__init__.py
+-rw-r--r--   0        0        0    10370 2020-02-02 00:00:00.000000 pysubcipher-2.1.0/src/pysubcipher/pysubcipher.py
+-rw-r--r--   0        0        0     1089 2020-02-02 00:00:00.000000 pysubcipher-2.1.0/LICENSE
+-rw-r--r--   0        0        0     7884 2020-02-02 00:00:00.000000 pysubcipher-2.1.0/README.md
+-rw-r--r--   0        0        0      586 2020-02-02 00:00:00.000000 pysubcipher-2.1.0/pyproject.toml
+-rw-r--r--   0        0        0     8161 2020-02-02 00:00:00.000000 pysubcipher-2.1.0/PKG-INFO
```

### Comparing `pysubcipher-2.0.1/src/pysubcipher/__init__.py` & `pysubcipher-2.1.0/src/pysubcipher/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 """
 PySubCipher allows you to encode and decode strings of text using a substitution cipher algorithm.
 
-:copyright: (c) 2023-present Mxngo
+:copyright: (c) 2023-present mxngo
 :license: MIT, see LICENSE for more details.
 """
 
 __title__ = "pysubcipher"
 __author__ = "mxngo"
-__copyright__ = ":copyright: (c) 2023-present Mxngo"
+__copyright__ = ":copyright: (c) 2023-present mxngo"
 __license__ = "MIT"
 
 import string
 from typing import Final
 
 from .pysubcipher import *
```

### Comparing `pysubcipher-2.0.1/src/pysubcipher/pysubcipher.py` & `pysubcipher-2.1.0/src/pysubcipher/pysubcipher.py`

 * *Files 24% similar despite different names*

```diff
@@ -5,177 +5,236 @@
 import io
 import os
 
 from .__init__ import HEXDIGITS
 
 from typing import Any
 
-class InvalidTokenFoundError(Exception):
-    def __init__(self, character: str | None = None, /) -> None:
-        """Raised if an invalid character or token is present within a string of text
-        during the encryption / decryption phase.
+class InvalidCharacterError(ValueError):
+    def __init__(self, character: str, /) -> None:
+        """Raised if an invalid token is present within a string of text while encrypting or decrypting a value.
 
         Args:
-            character (str | None, optional): The invalid token that was present. Defaults to None.
+            character (str): The invalid character.
         """
-        if character is None:
-            super().__init__()
-        else:
-            super().__init__(f"Invalid token \"{character}\" is not defined as printable.")
+        super().__init__(f"\"{character}\" is not recognised.")
+
+class EncryptedStringInvalidError(ValueError):
+    def __init__(self, token: str) -> None:
+        """Raised if an encrypted string is invalid while attempting to decrypt it.
+
+        Args:
+            token (str): Unmatched token.
+        """
+        if len(token) > 18:
+            token = f"{token[:18]}..."
+        super().__init__(f"Encrypted string is not valid: decryption keys did not match token \"{token}\"")
+
+class InvalidKeysError(ValueError):
+    def __init__(self) -> None:
+        """Raised if invalid keys are loaded into a SubstitutionCipher instance."""
+        super().__init__(f"Cipher keys failed validation")
 
 class _EncryptionKeys():
     def __init__(self, __min_length: int, __max_length: int, /, *, seed: Any, charset: str) -> None:
-        """Generates a pair of encryption and decryption keys at a desired length.
+        """Generates a pair of encryption and decryption keys.
 
         Args:
-            __min_length (int): The minimum length of a key
-            __max_length (int): The maximum length of a key
-            seed (Any): The random seed that keys will be generated with
-            charset (str): The character set to generate keys with
+            __min_length (int): The minimum length of a key.
+            __max_length (int): The maximum length of a key.
+            seed (Any): The random seed that keys will be generated with.
+            charset (str): The character set to generate keys with.
         """
         self.__min_length: int = __min_length
         self.__max_length: int = __max_length
         self.__seed: Any = seed
         self.__charset: str = charset
         self._encryption_keys: dict[bytes, str] | None = None
         self._decryption_keys: dict[str, bytes] | None = None
         self.__generate_keys(seed = self.__seed)
 
     def __generate_keys(self, *, seed: bytes) -> None:
         """
-        Generates a list of keys bound to a list of characters which are defined in string's printable character list.
-        Valid characters: 0123456789abcdefghijklmnopqrstuvwxyzABCDEFGHIJKLMNOPQRSTUVWXYZ!"#$%&'()*+,-./:;<=>?@[\]^_`{|}~
+        Generates a list of keys bound to a list of characters.
 
         Args:
-            seed (bytes): The random seed to generate keys on.
+            seed (bytes): The random seed to generate keys with.
         """
         random.seed(seed)
         encryption_keys: dict[bytes, str] = {}
         decryption_keys: dict[str, bytes] = {}
         characters = self.__charset
 
         for character in string.printable:
             key = ''.join([random.choice(characters) for _ in range(random.randint(self.__min_length, self.__max_length))])
-            __char = base64.b64encode(bytes(character.encode().hex(), "UTF-8"))
+            __char = base64.b64encode(character.encode().hex().encode())
             encryption_keys[__char] = key
             decryption_keys[key] = __char
 
         self._encryption_keys = encryption_keys
         self._decryption_keys = decryption_keys
         random.seed(None)
 
 class SubstitutionCipher(_EncryptionKeys):
     def __init__(self, min_key_length: int = 10, max_key_length: int = 20, *, seed: Any | None = os.urandom(1024), charset: str = HEXDIGITS) -> None:
         """A simple substitution cipher encryption tool to encode strings of text.
 
         Args:
-            min_key_length (int): The minimum length of a cipher key
-            max_key_length (int): The maximum length of a cipher key
+            min_key_length (int): The minimum length of a cipher key.
+            max_key_length (int): The maximum length of a cipher key.
             seed (Any | None, optional): The seed that cipher keys will be generated with. Defaults to os.urandom(1024).
             charset (str, optional): The character set that cipher keys will be generated with. Defaults to HEXDIGITS.
         """
         self.__min_key_length: int = min_key_length
         self.__max_key_length: int = max_key_length
         self.__charset: str = charset
         if not isinstance(charset, str):
             raise TypeError(f"Parameter charset cannot be of type {type(charset)}")
         super().__init__(min_key_length, max_key_length, seed = seed, charset = self.__charset)
     def encrypt(self, s: str, /) -> bytes:
-        """Encrypts a string of text using an arrangement of encryption keys.
+        """Encrypts a string of text using pre-defined cipher keys.
 
         Args:
             s (str): The string to encrypt.
 
         Raises:
-            InvalidTokenFoundError: If an unidentified character is present within the string (s), an InvalidTokenFoundError will be raised.
+            InvalidCharacterError: Raised if a non-printable character is present within the string.
 
         Returns:
-            bytes: An encrypted byte-string of the original text (s).
+            bytes: An encrypted byte string of the original string.
         """
         __encrypted_string: io.StringIO = io.StringIO()
         for character in s:
             character = base64.b64encode(character.encode().hex().encode())
             if character not in self._encryption_keys:
-                raise InvalidTokenFoundError(character) 
+                raise InvalidCharacterError(bytearray.fromhex(base64.b64decode(character).decode()).decode()) 
             __encrypted_string.write(self._encryption_keys.get(character))
-        return bytes(__encrypted_string.getvalue(), "UTF-8")
+        return __encrypted_string.getvalue().encode()
     def decrypt(self, s: bytes, /) -> bytes:
-        """Decrypts a string of text using an arrangement of decryption keys.
+        """Decrypts a string of text using pre-defined cipher keys.
 
         Args:
             s (bytes): The string to decrypt.
 
         Raises:
-            InvalidTokenFoundError: If an invalid token (or key) is present within the string (s), an InvalidTokenFoundError will be raised.
+            TypeError: Raised if s is not an instance of <class 'bytes'>.
+            EncryptedStringInvalidError: Raised if the encrypted string is invalid.
 
         Returns:
-            bytes: An unencrypted byte-string of the original encrypted text (s).
+            bytes: An unencrypted byte string of the original encrypted string.
         """
+        if not isinstance(s, bytes):
+            raise TypeError(f"s must be of type bytes, not {type(s)}")
         __decrypted_string: io.StringIO = io.StringIO()
         while s:
             __match = False
             for k in self._decryption_keys:
-                if s.startswith(bytes(k, "UTF-8")):
+                if s.startswith(k.encode()):
                     __decrypted_string.write(bytearray.fromhex(base64.b64decode(self._decryption_keys[k].decode()).decode()).decode())
                     s = s[len(k):]
                     __match = True
                     break
             if not __match:
-                raise InvalidTokenFoundError()
-        return bytes(__decrypted_string.getvalue(), "UTF-8")
+                raise EncryptedStringInvalidError(s.decode())
+        return __decrypted_string.getvalue().encode()
     def set_seed(self, seed: Any, /) -> None:
-        """Sets the seed that cipher keys will be generated with
+        """Sets the random seed for cipher keys to be generated with.
 
         Args:
-            seed (Any): The seed to override
+            seed (Any): The seed to override.
         """
         super().__init__(self.__min_key_length, self.__max_key_length, seed = seed, charset = self.__charset)
     def __test_keys(self, encryption_keys: Any, decryption_keys: Any) -> bool:
-        """Tests and validates encryption and decryption keys and returns if the keys are valid
+        """Tests and validates cipher keys.
 
         Args:
-            encryption_keys (Any): The encryption keys to validate
-            decryption_keys (Any): The decryption keys to validate
+            encryption_keys (Any): The encryption keys to validate.
+            decryption_keys (Any): The decryption keys to validate.
 
         Returns:
-            bool: Returns True if the keys are valid, and False if they are not
+            bool: Returns True if cipher keys are valid, and False if not.
         """
         text = string.printable
         cipher = SubstitutionCipher()
         cipher._encryption_keys = encryption_keys
         cipher._decryption_keys = decryption_keys
         encrypted_text = cipher.encrypt(text)
         decrypted_text = cipher.decrypt(encrypted_text)
         if decrypted_text.decode() != text:
             return False
         return True
     def save_keys(self, file: str, /, *, truncate: bool = False) -> None:
-        """Saves the current cipher keys to a file
+        """Saves the current cipher keys to a file.
 
         Args:
-            file (str): The path to the file
-            truncate (bool, optional): If True, the file will be truncated before storing the keys. Defaults to False.
+            file (str): The filepath.
+            truncate (bool, optional): If True, file will be truncated prematurely before storing the keys. Defaults to False.
         """
         with open(file, "wb") as f:
             if truncate:
                 f.truncate(0)
             f.write(pickle.dumps([self._encryption_keys, self._decryption_keys]))
     def load_keys(self, file: str, /) -> None:
-        """Loads cipher keys into the instance
+        """Loads cipher keys into the current instance.
 
         Args:
-            file (str): The path to the file where the keys are stored
+            file (str): The path to the file where the keys are stored.
 
         Raises:
-            InvalidTokenFoundError: If the keys are not valid, an InvalidTokenFoundError will be raised
+            InvalidKeysError: Raised if the cipher keys are not valid.
         """
         with open(file, "rb") as f:
             contents = f.read()
-            keys = pickle.loads(contents)
+            try:
+                keys = pickle.loads(contents)
+            except pickle.UnpicklingError:
+                raise InvalidKeysError()
             encryption_keys = keys[0]
             decryption_keys = keys[1]
             result: bool = self.__test_keys(encryption_keys, decryption_keys)
             if result:
                 self._encryption_keys = encryption_keys
                 self._decryption_keys = decryption_keys
             else:
-                raise InvalidTokenFoundError()
+                raise InvalidKeysError()
+
+class FileSubstitutionCipher(SubstitutionCipher):
+    def __init__(self, min_key_length: int = 10, max_key_length: int = 20, *, seed: Any | None = os.urandom(1024), charset: str = HEXDIGITS) -> None:
+        self.__min_key_length: int = min_key_length
+        self.__max_key_length: int = max_key_length
+        self.__seed: Any = seed
+        self.__charset: str = charset
+        super().__init__(self.__min_key_length, self.__max_key_length, seed = self.__seed, charset = self.__charset)
+    def encrypt(self, filepath: str, /, *, write: bool = False) -> bytes | None:
+        """Encrypts the contents of a file and returns the encrypted contents.
+
+        Args:
+            filepath (str): The path to the file that will be encrypted.
+            write (bool, optional): Override the file's contents. Defaults to False.
+
+        Returns:
+            bytes | None: Returns the encrypted contents if write is False, otherwise returns None.
+        """
+        encrypted_contents: bytes = super().encrypt(open(filepath).read())
+        if write:
+            with open(filepath, "wb") as file:
+                file.truncate(0)
+                file.write(encrypted_contents)
+        else:
+            return encrypted_contents
+    def decrypt(self, filepath: str, /, *, write: bool = False) -> bytes | None:
+        """Decrypts the contents of a file and returns the decrypted contents.
+
+        Args:
+            filepath (str): The path to the file that will be decrypted.
+            write (bool, optional): Override the file's contents. Defaults to False.
+
+        Returns:
+            bytes | None: Returns the decrypted contents if write is False, otherwise returns None.
+        """
+        decrypted_contents: bytes = super().decrypt(open(filepath).read().encode())
+        if write:
+            with open(filepath, "wb") as file:
+                file.truncate(0)
+                file.write(decrypted_contents)
+        else:
+            return decrypted_contents
```

### Comparing `pysubcipher-2.0.1/LICENSE` & `pysubcipher-2.1.0/LICENSE`

 * *Files identical despite different names*

