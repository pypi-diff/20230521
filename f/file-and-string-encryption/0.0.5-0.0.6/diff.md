# Comparing `tmp/file_and_string_encryption-0.0.5.tar.gz` & `tmp/file_and_string_encryption-0.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "file_and_string_encryption-0.0.5.tar", last modified: Sat May 20 17:49:41 2023, max compression
+gzip compressed data, was "file_and_string_encryption-0.0.6.tar", last modified: Sun May 21 20:46:44 2023, max compression
```

## Comparing `file_and_string_encryption-0.0.5.tar` & `file_and_string_encryption-0.0.6.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxrwx   0        0        0        0 2023-05-20 17:49:41.546239 file_and_string_encryption-0.0.5/
--rw-rw-rw-   0        0        0     1095 2023-01-07 18:45:09.000000 file_and_string_encryption-0.0.5/LICENSE
--rw-rw-rw-   0        0        0       85 2023-05-14 19:46:17.000000 file_and_string_encryption-0.0.5/MANIFEST.in
--rw-rw-rw-   0        0        0     1198 2023-05-20 17:49:41.546239 file_and_string_encryption-0.0.5/PKG-INFO
--rw-rw-rw-   0        0        0      539 2023-05-14 19:59:38.000000 file_and_string_encryption-0.0.5/README.md
-drwxrwxrwx   0        0        0        0 2023-05-20 17:49:41.534522 file_and_string_encryption-0.0.5/file_and_string_encryption/
--rw-rw-rw-   0        0        0      614 2023-05-20 17:47:55.000000 file_and_string_encryption-0.0.5/file_and_string_encryption/__init__.py
--rw-rw-rw-   0        0        0    20750 2023-05-20 17:47:18.000000 file_and_string_encryption-0.0.5/file_and_string_encryption/file_and_string_encryption.py
-drwxrwxrwx   0        0        0        0 2023-05-20 17:49:41.544235 file_and_string_encryption-0.0.5/file_and_string_encryption.egg-info/
--rw-rw-rw-   0        0        0     1198 2023-05-20 17:49:41.000000 file_and_string_encryption-0.0.5/file_and_string_encryption.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      383 2023-05-20 17:49:41.000000 file_and_string_encryption-0.0.5/file_and_string_encryption.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-20 17:49:41.000000 file_and_string_encryption-0.0.5/file_and_string_encryption.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       32 2023-05-20 17:49:41.000000 file_and_string_encryption-0.0.5/file_and_string_encryption.egg-info/requires.txt
--rw-rw-rw-   0        0        0       27 2023-05-20 17:49:41.000000 file_and_string_encryption-0.0.5/file_and_string_encryption.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-05-20 17:49:41.546239 file_and_string_encryption-0.0.5/setup.cfg
--rw-rw-rw-   0        0        0     1739 2023-05-20 17:47:54.000000 file_and_string_encryption-0.0.5/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-21 20:46:44.515056 file_and_string_encryption-0.0.6/
+-rw-rw-rw-   0        0        0     1095 2023-01-07 18:45:09.000000 file_and_string_encryption-0.0.6/LICENSE
+-rw-rw-rw-   0        0        0       85 2023-05-14 19:46:17.000000 file_and_string_encryption-0.0.6/MANIFEST.in
+-rw-rw-rw-   0        0        0     1198 2023-05-21 20:46:44.515056 file_and_string_encryption-0.0.6/PKG-INFO
+-rw-rw-rw-   0        0        0      539 2023-05-14 19:59:38.000000 file_and_string_encryption-0.0.6/README.md
+drwxrwxrwx   0        0        0        0 2023-05-21 20:46:44.504629 file_and_string_encryption-0.0.6/file_and_string_encryption/
+-rw-rw-rw-   0        0        0      678 2023-05-21 20:45:35.000000 file_and_string_encryption-0.0.6/file_and_string_encryption/__init__.py
+-rw-rw-rw-   0        0        0    25256 2023-05-21 20:44:55.000000 file_and_string_encryption-0.0.6/file_and_string_encryption/file_and_string_encryption.py
+drwxrwxrwx   0        0        0        0 2023-05-21 20:46:44.512850 file_and_string_encryption-0.0.6/file_and_string_encryption.egg-info/
+-rw-rw-rw-   0        0        0     1198 2023-05-21 20:46:44.000000 file_and_string_encryption-0.0.6/file_and_string_encryption.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      383 2023-05-21 20:46:44.000000 file_and_string_encryption-0.0.6/file_and_string_encryption.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-21 20:46:44.000000 file_and_string_encryption-0.0.6/file_and_string_encryption.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       50 2023-05-21 20:46:44.000000 file_and_string_encryption-0.0.6/file_and_string_encryption.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       27 2023-05-21 20:46:44.000000 file_and_string_encryption-0.0.6/file_and_string_encryption.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-05-21 20:46:44.515056 file_and_string_encryption-0.0.6/setup.cfg
+-rw-rw-rw-   0        0        0     1804 2023-05-21 20:35:30.000000 file_and_string_encryption-0.0.6/setup.py
```

### Comparing `file_and_string_encryption-0.0.5/LICENSE` & `file_and_string_encryption-0.0.6/LICENSE`

 * *Files identical despite different names*

### Comparing `file_and_string_encryption-0.0.5/PKG-INFO` & `file_and_string_encryption-0.0.6/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: file_and_string_encryption
-Version: 0.0.5
+Version: 0.0.6
 Summary: Simple encryption functions. Do not simply trust this code! Pay attention to how you handle sensitive information!
 Author: André Herber
 Author-email: andre.herber.programming@gmail.com
 Keywords: python
 Classifier: Development Status :: 1 - Planning
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
```

### Comparing `file_and_string_encryption-0.0.5/README.md` & `file_and_string_encryption-0.0.6/README.md`

 * *Files identical despite different names*

### Comparing `file_and_string_encryption-0.0.5/file_and_string_encryption/__init__.py` & `file_and_string_encryption-0.0.6/file_and_string_encryption/__init__.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,23 +1,25 @@
 from .file_and_string_encryption import (
     bytes_to_data_using_pickle,
     data_to_bytes_using_pickle,
     decrypt_data,
     decrypt_directory,
     decrypt_file,
     decrypt_file_with_password,
+    decrypt_hidden_directory,
     decrypt_string_with_password,
     derive_key_from_password,
+    encrypt_and_hide_directory,
     encrypt_data,
     encrypt_directory,
     encrypt_file,
     encrypt_file_with_password,
     encrypt_string_with_password,
     generate_password,
     get_random_key,
     hash_password_with_argon2,
     load_password_encrypted_key,
     save_password_encrypted_key,
     verfiy_hashed_password_with_argon2,
 )
 
-__version__ = "0.0.5"
+__version__ = "0.0.6"
```

### Comparing `file_and_string_encryption-0.0.5/file_and_string_encryption/file_and_string_encryption.py` & `file_and_string_encryption-0.0.6/file_and_string_encryption/file_and_string_encryption.py`

 * *Files 15% similar despite different names*

```diff
@@ -6,29 +6,31 @@
 von: https://stackoverflow.com/questions/2490334/simple-way-to-encode-a-string-according-to-a-password
 """
 
 
 ### Fernet with password – key derived from password, weakens the security somewhat
 # https://stackoverflow.com/questions/2490334/simple-way-to-encode-a-string-according-to-a-password
 
+import os
+import pickle
 from base64 import urlsafe_b64decode as b64d
 from base64 import urlsafe_b64encode as b64e
-import os
-from pathlib import Path
-import binascii
-from secrets import token_bytes as secrets_token_bytes, choice as secrets_choice
-from string import ascii_letters, digits, punctuation
+from random import choice
+from secrets import choice as secrets_choice
+from secrets import token_bytes as secrets_token_bytes
+from string import ascii_letters, ascii_uppercase, digits, punctuation
 
 from cryptography.fernet import Fernet
 from cryptography.hazmat.backends import default_backend
 from cryptography.hazmat.primitives import hashes
 from cryptography.hazmat.primitives.kdf.pbkdf2 import PBKDF2HMAC
 from passlib.context import CryptContext
-from easy_tasks import main_and_sub_progress_printer
-import pickle
+
+from colorful_terminal import *
+from easy_tasks import main_and_sub_progress_printer, pickle_pack, pickle_unpack
 
 backend = default_backend()
 
 
 def bytes_to_data_using_pickle(data):
     return pickle.loads(data)
 
@@ -75,23 +77,23 @@
     return decrypted
 
 
 def decrypt_directory(
     target_dir_path: str,
     enc_dir_path: str,
     keypath: str | None | bytes,
-    error_if_target_is_file: bool = True,
+    override_target: bool = True,
 ):
     """Decrypts all files in a directory. Keeps the original directory structure.
 
     Args:
         - target_dir_path (str): Path for the decrypted directory.
         - enc_dir_path (str): Path to the encrypted directory.
         - keypath (str | None | bytes): Path to the key or alternativley the key itself.
-        - error_if_target_is_file (bool, optional): Raise an exception if target_filepath is already a file. Defaults to True.
+        - override_target (bool, optional): Override the target files if they already exist. Defaults to False.
     """
     enc_dir_path = os.path.normpath(enc_dir_path)
 
     l1 = len(list(os.walk(enc_dir_path)))
 
     main_and_sub_progress_printer(
         0,
@@ -104,42 +106,39 @@
     for main_index, (root, dirs, files) in enumerate(os.walk(enc_dir_path)):
         sub_path = root.replace(enc_dir_path, "")
         sub_path = sub_path.lstrip("\\")
         l2 = len(files)
         for sub_index, f in enumerate(files):
             fp = os.path.join(root, f)
             nfp = os.path.join(target_dir_path, sub_path, f)
-            decrypt_file(nfp, fp, keypath, error_if_target_is_file)
+            decrypt_file(nfp, fp, keypath, override_target)
             main_and_sub_progress_printer(
                 main_index + 1,
                 l1,
                 sub_index + 1,
                 l2,
                 mainpre_string="Progress on dirpaths: ",
                 subpre_string="Progress on files in current dir: ",
             )
 
 
 def decrypt_file(
     to_be_filepath: str,
     enc_filepath: str,
     keypath: str | bytes,
-    error_if_target_is_file: bool = True,
+    override_target: bool = False,
 ):
     """Decrypt a file using the generated key. The file was decrypted with encrypt_file.
 
     Args:
         - to_be_filepath (str): The path at which the file shall be generated, including the filename.
         - enc_filepath (str): The path to the encrypted file.
         - keypath (str | bytes): The path to the key or alternativley the key itself.
+        - override_target (bool, optional): Override the target file if it already exists. Defaults to False.
     """
-    if error_if_target_is_file and os.path.isfile(to_be_filepath):
-        raise FileExistsError(
-            f"There is already a file in the to_be_filepath location.\n\tto_be_filepath: {to_be_filepath}"
-        )
     if isinstance(keypath, str):
         with open(keypath, "rb") as f:
             key = f.read()
     else:
         key = keypath
     fernet = Fernet(key)
     with open(enc_filepath, "rb") as encrypted_file:
@@ -150,27 +149,35 @@
     if not os.path.isdir(basepath):
         os.makedirs(basepath)
     pre_filepath = os.path.join(basepath, filename)
     with open(pre_filepath, "wb") as decrypted_file:
         decrypted_file.write(decrypted)
     if os.path.isdir(to_be_filepath):
         os.removedirs(to_be_filepath)
+    if override_target:
+        if os.path.isfile(to_be_filepath):
+            os.remove(to_be_filepath)
     os.rename(pre_filepath, to_be_filepath)
 
 
 def decrypt_file_with_password(
-    to_be_filepath: str, enc_filepath: str, keypath: str, password: str
+    to_be_filepath: str,
+    enc_filepath: str,
+    keypath: str,
+    password: str,
+    override_target: bool = False,
 ):
     """Decrypt a file using a password. The file was decrypted using encrypt_file_with_password.
 
     Args:
         - to_be_filepath (str): The path at which the file shall be generated, including the filename.
         - enc_filepath (str): The path to the encrypted file.
         - keypath (str): The path to the encrypted key.
         - password (str): The password to decrypt the actual key.
+        - override_target (bool, optional): Override the target file if it already exists. Defaults to False.
     """
     with open(keypath, "rb") as f:
         enc_key = f.read()
     key = decrypt_string_with_password(enc_key, password)
     fernet = Fernet(key)
     with open(enc_filepath, "rb") as encrypted_file:
         encrypted = encrypted_file.read()
@@ -180,17 +187,63 @@
     if not os.path.isdir(basepath):
         os.makedirs(basepath)
     pre_filepath = os.path.join(basepath, filename)
     with open(pre_filepath, "wb") as decrypted_file:
         decrypted_file.write(decrypted)
     if os.path.isdir(to_be_filepath):
         os.removedirs(to_be_filepath)
+    if override_target:
+        if os.path.isfile(to_be_filepath):
+            os.remove(to_be_filepath)
     os.rename(pre_filepath, to_be_filepath)
 
 
+def decrypt_hidden_directory(
+    target_dir_path: str,
+    enc_dir_path: str,
+    enc_rename_path: str,
+    keypath: str | bytes = None,
+):
+    """Decrypt a hidden directory. This is the decrytion function to `encrypt_and_hide_directory`.
+
+    Args:
+        target_dir_path (str): Path for the decrypted directory.
+        enc_dir_path (str): Path to the encrypted directory.
+        enc_rename_path (str): Path for the encrypted file containing the directory which has the new and the old file and directory names.
+        keypath (str | bytes, optional): Path to the key or alternativley the key itself. Defaults to None.
+    """
+    colored_print(Fore.GREEN + "decrypt_hidden_directory")
+    print("Reading names for directory contents...")
+
+    if isinstance(keypath, str):
+        with open(keypath, "rb") as f:
+            key = f.read()
+    elif isinstance(keypath, bytes):
+        key = keypath
+
+    renamed_to_path_enc = pickle_unpack(enc_rename_path)
+    renamed_to_path_bytes = decrypt_data(renamed_to_path_enc, key)
+    renamed_to_path = bytes_to_data_using_pickle(renamed_to_path_bytes)
+    renamed_to_path: dict[str, str]
+
+    print("Renaming directory contents...")
+    for seq, fp in list(renamed_to_path.items())[::-1]:
+        os.rename(seq, fp)
+
+    print("Decrypting directory...")
+    decrypt_directory(target_dir_path, enc_dir_path, key, True)
+
+    if target_dir_path != enc_dir_path:
+        print("Renaming directory contents...")
+        for seq, fp in renamed_to_path.items():
+            os.rename(fp, seq)
+
+    print("Decryption done.\n")
+
+
 def decrypt_secret(encrypted_secret, password: str, salt):
     kdf = PBKDF2HMAC(
         algorithm=hashes.SHA256(),
         length=32,
         salt=salt,
         iterations=400000,
     )
@@ -219,14 +272,74 @@
     salt, iter, token = decoded[:16], decoded[16:20], b64e(decoded[20:])
     iterations = int.from_bytes(iter, "big")
     key = derive_key_from_password(password.encode(), salt, iterations)
     pw = Fernet(key).decrypt(token).decode()
     return pw
 
 
+def encrypt_and_hide_directory(
+    dir_path: str,
+    enc_dir_path: str,
+    enc_rename_path: str,
+    key: bytes = None,
+    keypath: str = None,
+):
+    """Encrypt and hide a directory. You might want to encrypt the key with a password using `save_password_encrypted_key`.
+
+    Args:
+        dir_path (str): Path to the directory to be encypted.
+        enc_dir_path (str): Target path to the encrypted directory.
+        enc_rename_path (str): Path for the encrypted file containing the directory which has the new and the old file and directory names.
+        key (bytes, optional): You can provide your own key. Defaults to None.
+        keypath (str, optional): Path for the file containing the unprotected key. Defaults to None.
+
+    Returns:
+        bytes: Returns the used key.
+    """
+    colored_print(Fore.GREEN + "encrypt_and_hide_directory")
+    print("Encrypting directory...")
+
+    key = encrypt_directory(
+        dir_path,
+        enc_dir_path,
+        keypath,
+        key,
+        error_if_enc_is_file=False,
+    )
+
+    print("Directory encrypted.")
+
+    print("Getting new names for directory contents...")
+
+    seq_to_path = {}
+    for dirpath, dirnames, filenames in os.walk(enc_dir_path, topdown=False):
+        for f in filenames:
+            fp = os.path.join(dirpath, f)
+            seq = get_seq_for_seq_to_path(dirpath, seq_to_path)
+            seq_to_path[seq] = fp
+        for f in dirnames:
+            fp = os.path.join(dirpath, f)
+            seq = get_seq_for_seq_to_path(dirpath, seq_to_path)
+            seq_to_path[seq] = fp
+
+    seq_to_path_bytes = data_to_bytes_using_pickle(seq_to_path)
+    seq_to_path_enc, k = encrypt_data(seq_to_path_bytes, key)
+
+    print("Saving new names for directory contents...")
+    # pickle_pack(seq_to_path, rename_path)
+    pickle_pack(seq_to_path_enc, enc_rename_path)
+
+    print("Renaming directory contents...")
+    for seq, fp in seq_to_path.items():
+        os.rename(fp, seq)
+
+    print("Encryption done.\n")
+    return key
+
+
 def encrypt_data(data: bytes, key: bytes = None) -> tuple[bytes]:
     """Encypt data using a key. The data must be bytes. You can provide your own key if you want.
      Data can be converted to bytes using pickle. For convenience there is a `data_to_bytes_using_pickle` function which literally is `pickle.dumps(data)`.
 
     Args:
         - data (bytes): Data to encrypt.
         - key (bytes, optional): Specified key to use. Defaults to None.
@@ -442,23 +555,37 @@
             and any(punctuation)
         ):
             break
 
     return password
 
 
+def generate_random_alphanumeric_string(length=25):
+    chars = ascii_uppercase + digits
+    random_str = "".join(choice(chars) for _ in range(length))
+    return random_str
+
+
 def get_random_key():
     """Generate a random key.
 
     Returns:
         bytes: The key generated by Fernet.generate_key()
     """
     return Fernet.generate_key()
 
 
+def get_seq_for_seq_to_path(dirpath, seq_to_path=None):
+    "A function for `encrypt_and_hide_directory`"
+    seq = os.path.join(dirpath, generate_random_alphanumeric_string())
+    # while seq in seq_to_path.keys():
+    #     seq = os.path.join(dirpath, generate_random_alphanumeric_string())
+    return seq
+
+
 def hash_password_with_argon2(password: str, argon2_default_rounds=55):
     """Hash a password using argon2. Hashed passwords can be used to ckeck wheather you know the real password with the help of the function `verfiy_hashed_password_with_argon2`.
 
     Args:
         - password (str): Password to hash.
         - argon2_default_rounds (int, optional): Rounds of the default argon2 hash function. Defaults to 55.
 
@@ -477,23 +604,23 @@
 def load_password_encrypted_key(
     keypath: str,
     password: str | None = None,
 ):
     """Load the password encrypted key from a file.
 
     Args:
-        keypath (str): Path to the file containing the password encrypted key.
-        password (str | None, optional): If the key is password encrypted, you obviously need the password. Defaults to None.
+        - keypath (str): Path to the file containing the password encrypted key.
+        - password (str | None, optional): If the key is password encrypted, you obviously need the password. Defaults to None.
 
     Returns:
         str: The decrypted key.
     """
     with open(keypath, "rb") as f:
         encrypted_key = f.read()
-    return decrypt_string_with_password(encrypted_key, password)
+    return decrypt_string_with_password(encrypted_key, password).encode()
 
 
 def password_decrypt_non_string(token: bytes, password: str):
     decoded = b64d(token)
     salt, iter, token = decoded[:16], decoded[16:20], b64e(decoded[20:])
     iterations = int.from_bytes(iter, "big")
     key = derive_key_from_password(password.encode(), salt, iterations)
```

### Comparing `file_and_string_encryption-0.0.5/file_and_string_encryption.egg-info/PKG-INFO` & `file_and_string_encryption-0.0.6/file_and_string_encryption.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: file-and-string-encryption
-Version: 0.0.5
+Version: 0.0.6
 Summary: Simple encryption functions. Do not simply trust this code! Pay attention to how you handle sensitive information!
 Author: André Herber
 Author-email: andre.herber.programming@gmail.com
 Keywords: python
 Classifier: Development Status :: 1 - Planning
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
```

### Comparing `file_and_string_encryption-0.0.5/setup.py` & `file_and_string_encryption-0.0.6/setup.py`

 * *Files 7% similar despite different names*

```diff
@@ -20,30 +20,35 @@
 import os
 
 here = os.path.abspath(os.path.dirname(__file__))
 
 with codecs.open(os.path.join(here, "README.md"), encoding="utf-8") as fh:
     long_description = "\n" + fh.read()
 
-VERSION = "0.0.5"
+VERSION = "0.0.6"
 DESCRIPTION = "Simple encryption functions. Do not simply trust this code! Pay attention to how you handle sensitive information!"
 
 # Setting up
 setup(
     name="file_and_string_encryption",
     version=VERSION,
     author="André Herber",
     author_email="andre.herber.programming@gmail.com",
     description=DESCRIPTION,
     long_description_content_type="text/markdown",
     long_description=long_description,
     packages=find_packages(),
     package_data={},
     include_package_data=True,
-    install_requires=["cryptography", "easy_tasks", "passlib"],
+    install_requires=[
+        "cryptography",
+        "passlib",
+        "colorful_terminal",
+        "easy_tasks",
+    ],
     keywords=["python"],
     classifiers=[
         "Development Status :: 1 - Planning",
         "Intended Audience :: Developers",
         "Programming Language :: Python :: 3",
         "Operating System :: Unix",
         "Operating System :: MacOS :: MacOS X",
```

