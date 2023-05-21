# Comparing `tmp/Cryptem-0.0.4.tar.gz` & `tmp/Cryptem-0.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "Cryptem-0.0.4.tar", last modified: Sat May 20 09:29:52 2023, max compression
+gzip compressed data, was "Cryptem-0.1.0.tar", last modified: Sun May 21 10:19:54 2023, max compression
```

## Comparing `Cryptem-0.0.4.tar` & `Cryptem-0.1.0.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxrwxr-x   0 llearuin  (1000) llearuin  (1000)        0 2023-05-20 09:29:52.148277 Cryptem-0.0.4/
-drwxrwxr-x   0 llearuin  (1000) llearuin  (1000)        0 2023-05-20 09:29:52.148277 Cryptem-0.0.4/Cryptem.egg-info/
--rw-rw-rw-   0 llearuin  (1000) llearuin  (1000)     6566 2023-05-20 09:29:51.000000 Cryptem-0.0.4/Cryptem.egg-info/PKG-INFO
--rw-rw-rw-   0 llearuin  (1000) llearuin  (1000)      198 2023-05-20 09:29:52.000000 Cryptem-0.0.4/Cryptem.egg-info/SOURCES.txt
--rw-rw-rw-   0 llearuin  (1000) llearuin  (1000)        1 2023-05-20 09:29:51.000000 Cryptem-0.0.4/Cryptem.egg-info/dependency_links.txt
--rw-rw-rw-   0 llearuin  (1000) llearuin  (1000)       31 2023-05-20 09:29:51.000000 Cryptem-0.0.4/Cryptem.egg-info/requires.txt
--rw-rw-rw-   0 llearuin  (1000) llearuin  (1000)        8 2023-05-20 09:29:51.000000 Cryptem-0.0.4/Cryptem.egg-info/top_level.txt
--rw-rw-rw-   0 llearuin  (1000) llearuin  (1000)     7689 2023-05-20 09:27:49.000000 Cryptem-0.0.4/Cryptem.py
--rw-rw-r--   0 llearuin  (1000) llearuin  (1000)     6566 2023-05-20 09:29:52.148277 Cryptem-0.0.4/PKG-INFO
--rw-rw-rw-   0 llearuin  (1000) llearuin  (1000)     6021 2022-10-19 12:50:25.000000 Cryptem-0.0.4/README.md
--rw-rw-rw-   0 llearuin  (1000) llearuin  (1000)      104 2022-08-06 05:09:46.000000 Cryptem-0.0.4/pyproject.toml
--rw-rw-r--   0 llearuin  (1000) llearuin  (1000)       38 2023-05-20 09:29:52.148277 Cryptem-0.0.4/setup.cfg
--rw-rw-rw-   0 llearuin  (1000) llearuin  (1000)      907 2023-05-20 09:28:59.000000 Cryptem-0.0.4/setup.py
+drwxrwxr-x   0 llearuin  (1000) llearuin  (1000)        0 2023-05-21 10:19:54.334720 Cryptem-0.1.0/
+drwxrwxr-x   0 llearuin  (1000) llearuin  (1000)        0 2023-05-21 10:19:54.334720 Cryptem-0.1.0/Cryptem.egg-info/
+-rw-rw-rw-   0 llearuin  (1000) llearuin  (1000)     6578 2023-05-21 10:19:54.000000 Cryptem-0.1.0/Cryptem.egg-info/PKG-INFO
+-rw-rw-rw-   0 llearuin  (1000) llearuin  (1000)      199 2023-05-21 10:19:54.000000 Cryptem-0.1.0/Cryptem.egg-info/SOURCES.txt
+-rw-rw-rw-   0 llearuin  (1000) llearuin  (1000)        1 2023-05-21 10:19:54.000000 Cryptem-0.1.0/Cryptem.egg-info/dependency_links.txt
+-rw-rw-rw-   0 llearuin  (1000) llearuin  (1000)       31 2023-05-21 10:19:54.000000 Cryptem-0.1.0/Cryptem.egg-info/requires.txt
+-rw-rw-rw-   0 llearuin  (1000) llearuin  (1000)       16 2023-05-21 10:19:54.000000 Cryptem-0.1.0/Cryptem.egg-info/top_level.txt
+-rw-rw-r--   0 llearuin  (1000) llearuin  (1000)     4437 2023-05-21 10:00:39.000000 Cryptem-0.1.0/Cryptem.py
+-rw-rw-r--   0 llearuin  (1000) llearuin  (1000)     6578 2023-05-21 10:19:54.334720 Cryptem-0.1.0/PKG-INFO
+-rw-rw-r--   0 llearuin  (1000) llearuin  (1000)     7447 2023-05-21 09:21:02.000000 Cryptem-0.1.0/cryptem.py
+-rw-rw-rw-   0 llearuin  (1000) llearuin  (1000)      104 2022-08-06 05:09:46.000000 Cryptem-0.1.0/pyproject.toml
+-rw-rw-r--   0 llearuin  (1000) llearuin  (1000)       38 2023-05-21 10:19:54.334720 Cryptem-0.1.0/setup.cfg
+-rw-rw-rw-   0 llearuin  (1000) llearuin  (1000)     1182 2023-05-21 10:10:07.000000 Cryptem-0.1.0/setup.py
```

### Comparing `Cryptem-0.0.4/Cryptem.egg-info/PKG-INFO` & `Cryptem-0.1.0/Cryptem.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 Metadata-Version: 2.1
 Name: Cryptem
-Version: 0.0.4
+Version: 0.1.0
 Summary: Cryptographic applications library based on elliptic curve cryptography
 Home-page: https://ipfs.io/ipns/k2k4r8ld8q6344t8dop0rwuk8f3vhpo42un6zrnrffogaayr7xv59p83
 Author: emendir
 License: UNKNOWN
 Project-URL: Source Code on IPFS, https://ipfs.io/ipns/k2k4r8ld8q6344t8dop0rwuk8f3vhpo42un6zrnrffogaayr7xv59p83
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 
 An easy-to-use object-oriented API for working with cryptography: encrypting/decrypting data and files as well as signing data and verifying signatures.  
 Can be used for asymmetric and symmetric cryptography, signature verification, and supports password-like private keys.
-Uses elliptic curve cryptography for the data encryption and data signing, the file encryption however uses AES.  
+Cryptem uses elliptic curve cryptography for the data encryption and data signing, the file encryption however uses AES.  
 Built on the eciespy, cryptography, coincurve and hashlib modules.
 
 ## Classes `Crypt` and `Encryptor`:
 The `Crypt` class is a cryptographic tool used by the holder of a private key for encrypting and signing data. It's counterpart is the `Encryptor` class, which using a specific public key can ecrypt data and verify signatures.  
 These classes also include functionality for more efficient file encryption using AES secret keys, where the secret key is automatically asymmetrically encrypted and embedded in the symmetrically encrypted file. This means that the usage of this file encryption system is asymmetric (private & public key), although the encryption of the file itself is not.   
 Can be used for single-session asymmetric (public-key/private-key) cryptography
 as well as for (optionally password secured) multi-session (i.e. reused keys) asymmetric (public-key/private-key) or symetric (private-key-only) cryptography.  
@@ -37,102 +37,102 @@
   Give `public_key` (the public key) to Sender (the code in the program below).
 
 Communication Sender/Encryptor:
   
     # Object-Oriented Approach:
     from Cryptem import Encryptor
     encryptor = Encryptor(public_key)  # crete Encryptor object with Receiver's public key
-    cipher = encryptor.Encrypt("Hello there!".encode('utf-8')) # encrypt a message
+    cipher = encryptor.encrypt("Hello there!".encode('utf-8')) # encrypt a message
     
     # Functional Approach:
-    cipher = Encrypt("Hello there!".encode('utf-8'), public_key)
+    cipher = encrypt("Hello there!".encode('utf-8'), public_key)
 
   Transmit `cipher` to Receiver.
 
 Communication Receiver:
   
     # continued from above
-    plaintext = crypt.Decrypt(cipher).decode('utf-8') # decrypt message
+    plaintext = crypt.decrypt(cipher).decode('utf-8') # decrypt message
 
 ### - __Multi-Session Asymetric Encryption__ (public-key and private-key):  
 Communication Receiver:
     
     crypt = Crypt("mypassword")   # create Crypt object with a password, from which private and ublic keys are generated
     public_key = crypt.public_key # read public key
       
 Give `public_key` to Sender.
 
 Communication Sender/Encryptor:
     
     encryptor = Encryptor(public_key)  # crete Encryptor object with Receiver's public key
-    cipher = encryptor.Encrypt("Hello there!".encode('utf-8')) # encrypt a message
+    cipher = encryptor.encrypt("Hello there!".encode('utf-8')) # encrypt a message
 
 Transmit `cipher` to Receiver.
 
 Communication Receiver/Decryptor:
 
     # continued from above
-    plaintext = crypt.Decrypt(cipher).decode('utf-8') # decrypt message
+    plaintext = crypt.decrypt(cipher).decode('utf-8') # decrypt message
 
 
 ###  - __Multi-Session Symmetric Enryption__ (private-key only):  
   Sender/Encryptor:
   
       crypt = Crypt("our_password")
-      cipher = crypt.Encrypt("Hello there!".encode('utf-8'))
+      cipher = crypt.encrypt("Hello there!".encode('utf-8'))
   
   SECURELY & PRIVATELY transmit the password to the Receiver (this is the downside and weakness of symmetric encryption).
   
   Transmit `cipher` to other Receiver.
   
   Receiver:
   
       # continued from aboveplaintext
       crypt = Crypt("our_password")
-      plaintext = crypt.Decrypt(cipher).decode('utf-8')
+      plaintext = crypt.decrypt(cipher).decode('utf-8')
 ## File Encryption:
 Because the encryption technologies used above are rather inefficient when applied to larger quantities of data, the Crypt and Encryptor classes have fcuntions that implement symmetric AES encryption. The secret AES key is encrypted with asymmetric elliptic curve cryptography (exactly as the encryption methods above) and embedded into the file, so that the API user (programmer) need not worry about it, and can use the file encryption functionality in exactly the same way as the bytearray-encryption function above.
 
 Sender/Encryptor:
 
     crypt = Crypt() # create Crypt object with new random public and private keys
     public_key = crypt.public_key # read public key
 
   Give `public_key` (the public key) to Sender (the code in the program below).
 
   Communication Sender/Encryptor:
 
     # Object-Oriented Approach:
     encryptor = Encryptor(public_key)  # crete Encryptor object with Receiver's public key
-    encryptor.EncryptFile("/path/to/file", "/where/to/save/encrypted/file") # encrypt a file
+    encryptor.encrypt_file("/path/to/file", "/where/to/save/encrypted/file") # encrypt a file
 
     # Functional Approach:
-    EncryptFile("/path/to/file", "/where/to/save/encrypted/file", public_key)
+    encrypt_file("/path/to/file", "/where/to/save/encrypted/file", public_key)
 
   Transmit the encrypted file to Receiver.
 
   Communication Receiver:
 
     # continued from above
-    plaintext = crypt.DecryptFile("/path/to/encrypted/file", "/path/to/decrypted/file") # decrypt file
+    plaintext = crypt.decrypt_file("/path/to/encrypted/file", "/path/to/decrypted/file") # decrypt file
 
 # Signing
 Digital cryptographic signing data means creating a signature from and for a piece of data using a certain private key (in this case a password). Anybody can verify that the signature was indeed created using the private key by using the corresponding public key.
 
   Sender/Signer:
   
     data = "hello there!".encode("utf-8")
     
     crypt = Crypt("my_password")  # create a Crypt object using a password
     public_key = crypt.public_key # this is the public key you should share with others
-    signature = crypt.Sign(data)  # creating a signature for data
+    signature = crypt.sign(data)  # creating a signature for data
     
   Transmit `data`, `public_key` and `signature` to Receiver/Verifier.
   
   Receiver/Verifier:
   
     encryptor = Encryptor(public_key)
-    assert(encryptor.VerifySignature(data, signature)) # checking the validity of data's signature using the signer's public key
+    assert(encryptor.verify_signature(data, signature)) # checking the validity of data's signature using the signer's public key
```

### Comparing `Cryptem-0.0.4/Cryptem.py` & `Cryptem-0.1.0/cryptem.py`

 * *Files 5% similar despite different names*

```diff
@@ -5,16 +5,16 @@
 Built on the eciespy, coincurve and hashlib modules.
 """
 
 import hashlib
 import os
 import traceback
 from ecies.utils import generate_key
-from ecies import encrypt, decrypt
-from coincurve import PrivateKey, PublicKey, verify_signature
+import ecies
+import coincurve
 from cryptography.fernet import Fernet
 
 
 class Crypt:
     """Encryption/decryption engine for bytearrays.
     Can be used for single-session public-key/private-key cryptography
     as well as for password secured multi-session public-key/private-key or private-key-only cryptography.
@@ -28,191 +28,184 @@
             codec = Crypt()
             public_key = codec.public_key
 
             ## give public_key to Sender
 
             # Communication Sender:
             codec2 = Encryptor(public_key)
-            cipher = codec2.Encrypt("Hello there!".encode('utf-8'))
+            cipher = codec2.encrypt("Hello there!".encode('utf-8'))
 
             ## transmit cipher to Receiver
 
             # Communication Receiver:
-            plaintext = codec.Decrypt(cipher).decode('utf-8')
+            plaintext = codec.decrypt(cipher).decode('utf-8')
 
         - As Multi-Session Asymetric Encryption System (public-key and private-key):
             # Communication Receiver:
             codec = Crypt("mypassword")   # KEEP PASSWORD PRIVATE AND SAFE
             public_key = codec.public_key
 
             ## give public_key to Sender
 
             # Communication Sender:
             codec2 = Encryptor(public_key)
-            cipher = codec2.Encrypt("Hello there!".encode('utf-8'))
+            cipher = codec2.encrypt("Hello there!".encode('utf-8'))
 
             ## transmit cipher to Receiver
 
             # Communication Receiver:
-            plaintext = codec.Decrypt(cipher).decode('utf-8')
+            plaintext = codec.decrypt(cipher).decode('utf-8')
 
 
         - As Multisession Symetric Enryption System (private-key only):
             codec = Crypt("my_password")   # KEEP PASSWORD PRIVATE AND SAFE
-            cipher = codec.Encrypt("Hello there!".encode('utf-8'))
+            cipher = codec.encrypt("Hello there!".encode('utf-8'))
 
             ## transmit cipher to other person
 
             codec2 = Crypt("my_password")
-            plaintext = codec2.Decrypt(cipher).decode('utf-8')
+            plaintext = codec2.decrypt(cipher).decode('utf-8')
     """
 
     public_key = ""  # string
-    __private_key = ""  # coincurve.keys.PrivateKey
+    __private_key = ""  # coincurve.keys.coincurve.PrivateKey
 
     def __init__(self, password=None):
         if password == None:
             key = generate_key()    # generate new random key
         else:
             # creating a cryptographic hash from the password, to create a larger encryption key from it
             hashGen = hashlib.sha256()
             hashGen.update(password.encode())
             hash = hashGen.hexdigest()
 
-            key = PrivateKey.from_hex(hash)
+            key = coincurve.PrivateKey.from_hex(hash)
 
         self.__private_key = key
         self.public_key = key.public_key.format(False).hex()
 
-    def Encrypt(self, data_to_encrypt: bytearray):
-        return Encrypt(data_to_encrypt, self.public_key)
+    def encrypt(self, data_to_encrypt: bytearray):
+        return encrypt(data_to_encrypt, self.public_key)
 
-    def Decrypt(self, encrypted_data: bytearray):
+    def decrypt(self, encrypted_data: bytearray):
         try:
             if(type(encrypted_data) == bytearray):
                 encrypted_data = bytes(encrypted_data)
-            decrypted_data = decrypt(
+            decrypted_data = ecies.decrypt(
                 self.__private_key.to_hex(), encrypted_data)
             return decrypted_data
         except Exception as e:
             print("Failed at decryption.")
             print(e)
             print("----------------------------------------------------")
             traceback.print_exc()  # printing stack trace
             print("----------------------------------------------------")
             print("")
             # print(encrypted_data)
             return None
 
-    def EncryptFile(self, plain_file, encrypted_file):
-        return EncryptFile(plain_file, encrypted_file, self.public_key)
+    def encrypt_file(self, plain_file, encrypted_file):
+        return encrypt_file(plain_file, encrypted_file, self.public_key)
 
-    def DecryptFile(self, encrypted_file, decrypted_file):
+    def decrypt_file(self, encrypted_file, decrypted_file):
 
         with open(encrypted_file, 'rb') as file:
             encrypted_data = file.read()
         key = encrypted_data[:141]   # extract encrypted key from file
         encrypted_data = encrypted_data[141:]    # remove encrypted key from file
 
         # decrypt encrypted key and create file-decrypting Fernet object from it
-        f = Fernet(self.Decrypt(key))
+        f = Fernet(self.decrypt(key))
 
         decrypted_data = f.decrypt(encrypted_data)  # decrypt file
 
         with open(decrypted_file, 'wb') as file:
             file.write(decrypted_data)
 
-    def Sign(self, data: bytes):
+    def sign(self, data: bytes):
         return self.__private_key.sign(data)
 
-    def SignSmall(self, data: bytearray):
-        hashGen = hashlib.sha256()
-        hashGen.update(self.Sign(data))
-        return hashGen.hexdigest()
-
-    def VerifySignature(self, data: bytes, signature: bytes):
-        return VerifySignature(data, self.public_key, signature)
+    def verify_signature(self, data: bytes, signature: bytes):
+        return verify_signature(data, self.public_key, signature)
 
 
 class Encryptor:
     def __init__(self, public_key):
         self.public_key = public_key
 
-    def Encrypt(self, data):
-        return Encrypt(data, self.public_key)
+    def encrypt(self, data):
+        return encrypt(data, self.public_key)
 
-    def EncryptFile(self, plain_file, encrypted_file):
-        return EncryptFile(plain_file, encrypted_file, self.public_key)
+    def encrypt_file(self, plain_file, encrypted_file):
+        return encrypt_file(plain_file, encrypted_file, self.public_key)
 
-    def VerifySignature(self, data, signature):
-        pk = PublicKey(self.public_key)
-        return pk.verify(signature, data)
-        return verify_signature(signature, data, self.public_key)
+    def verify_signature(self, data, signature):
+        return verify_signature(data, self.public_key, signature)
 
 
-def Encrypt(data_to_encrypt: bytearray, public_key):
+def encrypt(data_to_encrypt: bytearray, public_key):
     """Encryption-only engine for bytearrays, based on public-key.
     Usage:
         # Communication Receiver:
         codec = Crypt()
         public_key = codec.public_key
 
         ## give public_key to Sender
 
         # Communication Sender:
-        cipher = Encrypt("Hello there!".encode('utf-8'), public_key)
+        cipher = encrypt("Hello there!".encode('utf-8'), public_key)
 
         ## transmit cipher to Receiver
 
         # Communication Receiver:
-        plaintext = codec.Decrypt(cipher).decode('utf-8')
+        plaintext = codec.decrypt(cipher).decode('utf-8')
     """
     try:
-        if type(data_to_encrypt) == str:
+        if isinstance(data_to_encrypt, str):
             print("data to encrypt must be of type bytearray")
-        if type(public_key) == bytearray:
+        if isinstance(public_key, bytearray):
             public_key = public_key.hex()
-        encrypted_data = encrypt(public_key, data_to_encrypt)
+        encrypted_data = ecies.encrypt(public_key, data_to_encrypt)
         return encrypted_data
     except Exception as e:
         print("Failed at encryption.")
         print(e)
         print("----------------------------------------------------")
         traceback.print_exc()  # printing stack trace
         print("----------------------------------------------------")
         print("")
         print("public key: " + public_key)
         print("")
         return None
 
 
-def EncryptFile(plain_file, encrypted_file, public_key):
+def encrypt_file(plain_file, encrypted_file, public_key):
     """
-    Encrypt a file.
+    encrypt a file.
     Parameters:
         plain_file: the path of the file to encrypt
         encrypted_file: where the encrypted file should be saved
     """
     key = Fernet.generate_key()
     f = Fernet(key)
 
     with open(plain_file, 'rb') as file:
         plain_data = file.read()
     encrypted_data = f.encrypt(plain_data)
 
-    key_encrypted = Encrypt(key, public_key)
+    key_encrypted = encrypt(key, public_key)
 
     encrypted_data = key_encrypted + encrypted_data
     with open(encrypted_file, 'wb') as file:
         file.write(encrypted_data)
 
 
-def VerifySignature(data: bytes, public_key: bytes, signature: bytes):
+def verify_signature(data: bytes, public_key: bytes, signature: bytes):
     if isinstance(public_key, str):
         public_key = bytes(bytearray.fromhex(public_key))
     elif isinstance(data, bytearray):
         public_key = bytes(public_key)
     if isinstance(data, bytearray):
         data = bytes(data)
     if isinstance(signature, bytearray):
         signature = bytes(signature)
-    return verify_signature(signature, data, public_key)
+    return coincurve.verify_signature(signature, data, public_key)
```

### Comparing `Cryptem-0.0.4/PKG-INFO` & `Cryptem-0.1.0/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 Metadata-Version: 2.1
 Name: Cryptem
-Version: 0.0.4
+Version: 0.1.0
 Summary: Cryptographic applications library based on elliptic curve cryptography
 Home-page: https://ipfs.io/ipns/k2k4r8ld8q6344t8dop0rwuk8f3vhpo42un6zrnrffogaayr7xv59p83
 Author: emendir
 License: UNKNOWN
 Project-URL: Source Code on IPFS, https://ipfs.io/ipns/k2k4r8ld8q6344t8dop0rwuk8f3vhpo42un6zrnrffogaayr7xv59p83
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 
 An easy-to-use object-oriented API for working with cryptography: encrypting/decrypting data and files as well as signing data and verifying signatures.  
 Can be used for asymmetric and symmetric cryptography, signature verification, and supports password-like private keys.
-Uses elliptic curve cryptography for the data encryption and data signing, the file encryption however uses AES.  
+Cryptem uses elliptic curve cryptography for the data encryption and data signing, the file encryption however uses AES.  
 Built on the eciespy, cryptography, coincurve and hashlib modules.
 
 ## Classes `Crypt` and `Encryptor`:
 The `Crypt` class is a cryptographic tool used by the holder of a private key for encrypting and signing data. It's counterpart is the `Encryptor` class, which using a specific public key can ecrypt data and verify signatures.  
 These classes also include functionality for more efficient file encryption using AES secret keys, where the secret key is automatically asymmetrically encrypted and embedded in the symmetrically encrypted file. This means that the usage of this file encryption system is asymmetric (private & public key), although the encryption of the file itself is not.   
 Can be used for single-session asymmetric (public-key/private-key) cryptography
 as well as for (optionally password secured) multi-session (i.e. reused keys) asymmetric (public-key/private-key) or symetric (private-key-only) cryptography.  
@@ -37,102 +37,102 @@
   Give `public_key` (the public key) to Sender (the code in the program below).
 
 Communication Sender/Encryptor:
   
     # Object-Oriented Approach:
     from Cryptem import Encryptor
     encryptor = Encryptor(public_key)  # crete Encryptor object with Receiver's public key
-    cipher = encryptor.Encrypt("Hello there!".encode('utf-8')) # encrypt a message
+    cipher = encryptor.encrypt("Hello there!".encode('utf-8')) # encrypt a message
     
     # Functional Approach:
-    cipher = Encrypt("Hello there!".encode('utf-8'), public_key)
+    cipher = encrypt("Hello there!".encode('utf-8'), public_key)
 
   Transmit `cipher` to Receiver.
 
 Communication Receiver:
   
     # continued from above
-    plaintext = crypt.Decrypt(cipher).decode('utf-8') # decrypt message
+    plaintext = crypt.decrypt(cipher).decode('utf-8') # decrypt message
 
 ### - __Multi-Session Asymetric Encryption__ (public-key and private-key):  
 Communication Receiver:
     
     crypt = Crypt("mypassword")   # create Crypt object with a password, from which private and ublic keys are generated
     public_key = crypt.public_key # read public key
       
 Give `public_key` to Sender.
 
 Communication Sender/Encryptor:
     
     encryptor = Encryptor(public_key)  # crete Encryptor object with Receiver's public key
-    cipher = encryptor.Encrypt("Hello there!".encode('utf-8')) # encrypt a message
+    cipher = encryptor.encrypt("Hello there!".encode('utf-8')) # encrypt a message
 
 Transmit `cipher` to Receiver.
 
 Communication Receiver/Decryptor:
 
     # continued from above
-    plaintext = crypt.Decrypt(cipher).decode('utf-8') # decrypt message
+    plaintext = crypt.decrypt(cipher).decode('utf-8') # decrypt message
 
 
 ###  - __Multi-Session Symmetric Enryption__ (private-key only):  
   Sender/Encryptor:
   
       crypt = Crypt("our_password")
-      cipher = crypt.Encrypt("Hello there!".encode('utf-8'))
+      cipher = crypt.encrypt("Hello there!".encode('utf-8'))
   
   SECURELY & PRIVATELY transmit the password to the Receiver (this is the downside and weakness of symmetric encryption).
   
   Transmit `cipher` to other Receiver.
   
   Receiver:
   
       # continued from aboveplaintext
       crypt = Crypt("our_password")
-      plaintext = crypt.Decrypt(cipher).decode('utf-8')
+      plaintext = crypt.decrypt(cipher).decode('utf-8')
 ## File Encryption:
 Because the encryption technologies used above are rather inefficient when applied to larger quantities of data, the Crypt and Encryptor classes have fcuntions that implement symmetric AES encryption. The secret AES key is encrypted with asymmetric elliptic curve cryptography (exactly as the encryption methods above) and embedded into the file, so that the API user (programmer) need not worry about it, and can use the file encryption functionality in exactly the same way as the bytearray-encryption function above.
 
 Sender/Encryptor:
 
     crypt = Crypt() # create Crypt object with new random public and private keys
     public_key = crypt.public_key # read public key
 
   Give `public_key` (the public key) to Sender (the code in the program below).
 
   Communication Sender/Encryptor:
 
     # Object-Oriented Approach:
     encryptor = Encryptor(public_key)  # crete Encryptor object with Receiver's public key
-    encryptor.EncryptFile("/path/to/file", "/where/to/save/encrypted/file") # encrypt a file
+    encryptor.encrypt_file("/path/to/file", "/where/to/save/encrypted/file") # encrypt a file
 
     # Functional Approach:
-    EncryptFile("/path/to/file", "/where/to/save/encrypted/file", public_key)
+    encrypt_file("/path/to/file", "/where/to/save/encrypted/file", public_key)
 
   Transmit the encrypted file to Receiver.
 
   Communication Receiver:
 
     # continued from above
-    plaintext = crypt.DecryptFile("/path/to/encrypted/file", "/path/to/decrypted/file") # decrypt file
+    plaintext = crypt.decrypt_file("/path/to/encrypted/file", "/path/to/decrypted/file") # decrypt file
 
 # Signing
 Digital cryptographic signing data means creating a signature from and for a piece of data using a certain private key (in this case a password). Anybody can verify that the signature was indeed created using the private key by using the corresponding public key.
 
   Sender/Signer:
   
     data = "hello there!".encode("utf-8")
     
     crypt = Crypt("my_password")  # create a Crypt object using a password
     public_key = crypt.public_key # this is the public key you should share with others
-    signature = crypt.Sign(data)  # creating a signature for data
+    signature = crypt.sign(data)  # creating a signature for data
     
   Transmit `data`, `public_key` and `signature` to Receiver/Verifier.
   
   Receiver/Verifier:
   
     encryptor = Encryptor(public_key)
-    assert(encryptor.VerifySignature(data, signature)) # checking the validity of data's signature using the signer's public key
+    assert(encryptor.verify_signature(data, signature)) # checking the validity of data's signature using the signer's public key
```

