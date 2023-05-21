# Comparing `tmp/readonce-1.0.2.tar.gz` & `tmp/readonce-1.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "readonce-1.0.2.tar", last modified: Mon Dec  5 10:34:46 2022, max compression
+gzip compressed data, was "readonce-1.0.3.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `readonce-1.0.2.tar` & `readonce-1.0.3.tar`

### file list

```diff
@@ -1,16 +1,16 @@
--rw-r--r--   0        0        0      117 2022-12-05 10:34:43.245327 readonce-1.0.2/.flake8
--rw-r--r--   0        0        0      427 2022-12-05 10:34:43.245327 readonce-1.0.2/.github/workflows/lint.yml
--rw-r--r--   0        0        0      502 2022-12-05 10:34:43.245327 readonce-1.0.2/.github/workflows/release.yml
--rw-r--r--   0        0        0      374 2022-12-05 10:34:43.245327 readonce-1.0.2/.github/workflows/test.yml
--rw-r--r--   0        0        0     1805 2022-12-05 10:34:43.245327 readonce-1.0.2/.gitignore
--rw-r--r--   0        0        0     1073 2022-12-05 10:34:43.245327 readonce-1.0.2/LICENSE
--rw-r--r--   0        0        0      650 2022-12-05 10:34:43.245327 readonce-1.0.2/Makefile
--rw-r--r--   0        0        0    15641 2022-12-05 10:34:43.245327 readonce-1.0.2/README.md
--rw-r--r--   0        0        0      918 2022-12-05 10:34:43.245327 readonce-1.0.2/pyproject.toml
--rwxr-xr-x   0        0        0      156 2022-12-05 10:34:43.245327 readonce-1.0.2/scripts/format-imports.sh
--rwxr-xr-x   0        0        0      166 2022-12-05 10:34:43.245327 readonce-1.0.2/scripts/format.sh
--rwxr-xr-x   0        0        0      108 2022-12-05 10:34:43.245327 readonce-1.0.2/scripts/lint.sh
--rw-r--r--   0        0        0     4881 2022-12-05 10:34:43.245327 readonce-1.0.2/src/readonce.py
--rw-r--r--   0        0        0     3736 2022-12-05 10:34:43.245327 readonce-1.0.2/tests/conftest.py
--rw-r--r--   0        0        0     6707 2022-12-05 10:34:43.245327 readonce-1.0.2/tests/test_readonce.py
--rw-r--r--   0        0        0    16517 1970-01-01 00:00:00.000000 readonce-1.0.2/PKG-INFO
+-rw-r--r--   0        0        0      117 2023-05-21 14:27:51.727887 readonce-1.0.3/.flake8
+-rw-r--r--   0        0        0      427 2023-05-21 14:27:51.727887 readonce-1.0.3/.github/workflows/lint.yml
+-rw-r--r--   0        0        0      502 2023-05-21 14:27:51.727887 readonce-1.0.3/.github/workflows/release.yml
+-rw-r--r--   0        0        0      374 2023-05-21 14:27:51.727887 readonce-1.0.3/.github/workflows/test.yml
+-rw-r--r--   0        0        0     1805 2023-05-21 14:27:51.727887 readonce-1.0.3/.gitignore
+-rw-r--r--   0        0        0     1073 2023-05-21 14:27:51.727887 readonce-1.0.3/LICENSE
+-rw-r--r--   0        0        0      650 2023-05-21 14:27:51.727887 readonce-1.0.3/Makefile
+-rw-r--r--   0        0        0    17317 2023-05-21 14:27:51.727887 readonce-1.0.3/README.md
+-rw-r--r--   0        0        0      947 2023-05-21 14:27:51.727887 readonce-1.0.3/pyproject.toml
+-rwxr-xr-x   0        0        0      156 2023-05-21 14:27:51.727887 readonce-1.0.3/scripts/format-imports.sh
+-rwxr-xr-x   0        0        0      166 2023-05-21 14:27:51.727887 readonce-1.0.3/scripts/format.sh
+-rwxr-xr-x   0        0        0      108 2023-05-21 14:27:51.727887 readonce-1.0.3/scripts/lint.sh
+-rw-r--r--   0        0        0     6770 2023-05-21 14:27:51.727887 readonce-1.0.3/src/readonce.py
+-rw-r--r--   0        0        0     3736 2023-05-21 14:27:51.727887 readonce-1.0.3/tests/conftest.py
+-rw-r--r--   0        0        0     9209 2023-05-21 14:27:51.727887 readonce-1.0.3/tests/test_readonce.py
+-rw-r--r--   0        0        0    18230 1970-01-01 00:00:00.000000 readonce-1.0.3/PKG-INFO
```

### Comparing `readonce-1.0.2/.gitignore` & `readonce-1.0.3/.gitignore`

 * *Files identical despite different names*

### Comparing `readonce-1.0.2/LICENSE` & `readonce-1.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `readonce-1.0.2/Makefile` & `readonce-1.0.3/Makefile`

 * *Files identical despite different names*

### Comparing `readonce-1.0.2/README.md` & `readonce-1.0.3/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -22,14 +22,38 @@
 ```
 
 # About the Usage
 
 Imagine that you need to pass a password it to some kind of service, which is going to Login your user.
 The Login service will only require this password only once, so why not to restrict it to be read, used only Once?
 
+# Important information
+
+The ReadOnce object is not a cryptography library. 
+It is not responsible for encrypting/decrypting or dictating any type of cryptography methods to store and retrieve your secrets.
+
+The main idea behind the ReadOnce objects is hardening the access and allow only one time access to the stored secrets in the object.
+
+Question: Are the secrets stored in plain text?
+Answer: No, we use symmetric encryption from cryptography named [Fernet](https://cryptography.io/en/latest/fernet/).
+And we store passed secret data internally as so called fernet token(ciphertext+hash value).
+When you try to retrieve the secret back, it is decrypted with the same key and send back as a plain text.
+
+Question: Then we have an encryption+hashing of plaintext?
+Answer: Yes, but ReadOnce class expects already encrypted(+ peppered, salted, hashed etc.) string to be passed as a secret, 
+because when you retrieve the secret it will return what it was originally passed. 
+If you passed the secret as "12345" you will get back "12345".
+If you passed the secret something like "HmDVbz6N3MlXqZ4q3TvLakMQ9fQjI45yhuoRHyZWiM4=" you will get back the same string.
+
+Question: Then why you store the secret as a token(ciphertext+hash value)?
+Answer: It is an extra layer of hardening, if somehow, somebody could get the ReadOnce object and tries to steal the secret, lovely attacker should also have the key.
+Okay the key also stored in ReadOnce object, but it is a non-trivial to get the key back. 
+If the attacker tries to add new secret over old one, the encryption key also updated.
+
+
 ### Install using pip:
 
 `pip install readonce`
 
 Then just inherit from the `ReadOnce`:
 
 ```py
@@ -435,38 +459,34 @@
     reg = r"^(?=.*[a-z])(?=.*[A-Z])(?=.*\d)(?=.*[@$!%*#?&])[A-Za-z\d@$!#%*?&]{6,20}$"
     pattern = re.compile(reg)
     return bool(re.search(pattern, password))
 ```
 
 After writing down password requirements you can convert them to `pre-conditions` as part of your DbC approach.
 
-* I used these ideas in the `ReadOnce` implementation as well, such as:
+# Is it possible to monkeypatch the secret logic management?
 
-```py
-@icontract.ensure(lambda self: not self.__secrets and not self.__is_consumed)
-def __init__(self) -> None:
-    self.__reset_secrets()
-    self.__reset_is_consumed()
-```
+As far, as I have tested it, 
+it is really non-trivial and over-hardened to monkeypatch the secret storage and also the secret management methods.
 
-Here I make myself to be sure that everything was reset properly.
-
-Another important topic is the invariants. Thinking about `ReadOnce` object, 
-at its lifecycle there can be either zero secret or only and only one secret:
+For eg, following test clearly shows the consequences:
 
 ```py
-@icontract.invariant(
-    lambda self: len(self) == 0 or len(self) == 1,
-    "There can be no or only single secret data stored",
-)
-class ReadOnce(metaclass=Final):
-    ...
-```
+def test_monkeypatch_change_secrets_storage(get_password_obj, monkeypatch):
+    # Directly trying to monkeypatch will raise double UnsupportedOperationException;
+    # As monkeypatch in its default undo() section tries to again edit "_ReadOnce__secrets" which raises same exception
+    # That's why we use context() below
+
+    # with pytest.raises(UnsupportedOperationException):
+    #     monkeypatch.setattr(get_password_obj, "_ReadOnce__secrets", ["12345"], raising=False)
 
-If somebody tries to inject more than one data to the secret storage, it will fail as it is a clear invariant violation.
+    with pytest.raises(UnsupportedOperationException):
+        with monkeypatch.context() as m:
+            m.setattr(get_password_obj, "_ReadOnce__secrets", ["12345"], raising=True)
+```
 
 
 # How to install for development?
 
 ### Create and activate the virtualenv:
 
 * `python3.10 -m venv .venv`
@@ -485,13 +505,9 @@
 
 ### Installing for general showcase
 
 `make install` or `flit install --env --deps=develop` 
 
 ### Run all tests in verbose
 
-`make test` or `pytest -svv` 
-
-
-# TODO
+`make test` or `pytest -svv`
 
-* Design by Contract ideas for ReadOnce object validation
```

### Comparing `readonce-1.0.2/pyproject.toml` & `readonce-1.0.3/pyproject.toml`

 * *Files 20% similar despite different names*

```diff
@@ -8,29 +8,30 @@
 readme = "README.md"
 license = {file = "LICENSE"}
 classifiers = ["License :: OSI Approved :: MIT License"]
 dynamic = ["version", "description"]
 requires-python = ">=3.10"
 dependencies = [
     "icontract >=2.6.2",
+    "cryptography >=40.0.2",
 ]
 
 [project.optional-dependencies]
 dev = [
     "black >=22.3.0",
     "pylint >=2.12.2",
     "isort >=5.9.3",
     "autoflake >=1.4",
     "flake8 >=4.0.1",
     "pre-commit >=2.17.0",
     "pytype >=2022.1.31",
     "pydantic >=1.10.2",
     ]
 test = [
-    "pytest >=7.1.3",
+    "pytest >=7.3.1",
     "pytest-cov >= 3.0.0",
 ]
 
 [tool.isort]
 profile = "black"
 py_version = 310
 skip = [".gitignore", ".dockerignore"]
```

### Comparing `readonce-1.0.2/src/readonce.py` & `readonce-1.0.3/src/readonce.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,17 +1,18 @@
 """
 Read-Once Object implementation in Python - Inspired by Secure by Design book.
 """
 
 import inspect
-from typing import Any, Iterable, List
+from typing import Any, Iterable, List, Optional
 
 import icontract
+from cryptography.fernet import Fernet
 
-__version__ = "1.0.2"
+__version__ = "1.0.3"
 
 
 class UnsupportedOperationException(Exception):
     def __init__(self, *args: object) -> None:
         self.message = "Not allowed on sensitive value"
         super().__init__(self.message, *args)
 
@@ -36,61 +37,98 @@
     * Sensitive class - inherited from ReadOnce can not be further subclassed
     * Sensitive data can not be pickled
     * Sensitive data can not be JSON serialized
     * All properties, fields are hidden and can not be accessed directly - even from subclass
     * The secrets can not be updated directly from outside - even from subclass
     """
 
-    __secrets: List[str] = []
+    __secrets: List[bytes] = []
     __is_consumed: bool = False
+    __key: Optional[bytes] = None
 
-    @icontract.ensure(lambda self: not self.__secrets and not self.__is_consumed)
+    @icontract.ensure(
+        lambda self: not self.__secrets and not self.__is_consumed and not self.__key
+    )
     def __init__(self) -> None:
         self.__reset_secrets()
         self.__reset_is_consumed()
+        self.__reset_key()
 
     @classmethod
     def __reset_secrets(cls) -> None:
         cls.__secrets = []
 
     @classmethod
     def __reset_is_consumed(cls):
         cls.__is_consumed = False
 
     @classmethod
+    def __reset_key(cls):
+        cls.__key = None
+
+    @classmethod
     def __update_is_consumed(cls):
         cls.__is_consumed = True
 
-    def add_secret(self, *args):
+    @classmethod
+    def __update_key(cls, key: bytes):
+        cls.__key = key
+
+    def add_secret(self, secret: Any):
+        def __get_token():
+            key_ = Fernet.generate_key()
+            fernet = Fernet(key_)
+            return key_, fernet.encrypt(bytes(secret_, encoding="utf-8"))
+
         if self.__is_consumed:
             raise UnsupportedOperationException(
                 "Sensitive object exhausted; you can not use it twice"
             )
+        secret_ = str(secret)
         self.__reset_secrets()
-        self.__secrets.append(*args)
+        self.__reset_key()
+        key, token = __get_token()
+        self.__update_key(key)
+        if not self.__key:
+            raise UnsupportedOperationException(
+                "Missing encryption key; impossible to store the secret"
+            )
+        self.__secrets.append(token)
 
     def get_secret(self):
         frame = inspect.currentframe()
         # get two upper/back frame; one is getting back from icontract wrapper, second to get encoder default function
         function_name = frame.f_back.f_back.f_code.co_name
         if function_name == "default":
             raise UnsupportedOperationException("Sensitive data can not be serialized")
         if self.__secrets:
             self.__update_is_consumed()
-            return self.__secrets.pop()
+            if not self.__key:
+                raise UnsupportedOperationException(
+                    "Missing encryption key; impossible decrypt the secret"
+                )
+            fernet = Fernet(self.__key)
+            token = self.__secrets.pop()
+            secret = fernet.decrypt(token)
+            self.__reset_key()
+            return secret.decode(encoding="utf-8")
         raise UnsupportedOperationException("Sensitive data was already consumed")
 
     @property
     def secrets(self):
         return []
 
     @property
     def is_consumed(self):
         return None
 
+    @property
+    def key(self):
+        return None
+
     def __getattribute__(self, __name: str) -> Any:
         frame = inspect.currentframe()
         # get the outer frame or caller frame
         function_name = frame.f_back.f_code.co_name
         if __name == "_ReadOnce__secrets" and function_name not in (
             "add_secret",
             "get_secret",
@@ -101,14 +139,21 @@
         if __name == "_ReadOnce__is_consumed" and function_name not in (
             "add_secret",
             "get_secret",
             "__init__",
         ):
             return None
 
+        if __name == "_ReadOnce__key" and function_name not in (
+            "add_secret",
+            "get_secret",
+            "__init__",
+        ):
+            return None
+
         if __name == "_ReadOnce__update_is_consumed" and function_name not in (
             "get_secret",
         ):
             raise UnsupportedOperationException()
 
         if __name == "_ReadOnce__reset_secrets" and function_name not in (
             "add_secret",
@@ -117,14 +162,24 @@
             raise UnsupportedOperationException()
 
         if __name == "_ReadOnce__reset_is_consumed" and function_name not in (
             "__init__",
         ):
             raise UnsupportedOperationException()
 
+        if __name == "_ReadOnce__reset_key" and function_name not in (
+            "get_secret",
+            "add_secret",
+            "__init__",
+        ):
+            raise UnsupportedOperationException()
+
+        if __name == "_ReadOnce__update_key" and function_name not in ("add_secret",):
+            raise UnsupportedOperationException()
+
         return super().__getattribute__(__name)
 
     def __setattr__(self, __name: str, __value: str) -> Any:
         frame = inspect.currentframe()
         # get the outer frame or caller frame
         function_name = frame.f_back.f_code.co_name
 
@@ -136,14 +191,21 @@
 
         if __name == "_ReadOnce__is_consumed" and function_name not in (
             "get_secret",
             "__init__",
         ):
             raise UnsupportedOperationException()
 
+        if __name == "_ReadOnce__key" and function_name not in (
+            "get_secret",
+            "add_secret",
+            "__init__",
+        ):
+            raise UnsupportedOperationException()
+
     def __dir__(self) -> Iterable[str]:
         return []
 
     def __str__(self) -> str:
         return f"{__class__.__name__}[secrets=*****]"
 
     def __repr__(self) -> str:
```

### Comparing `readonce-1.0.2/tests/conftest.py` & `readonce-1.0.3/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `readonce-1.0.2/tests/test_readonce.py` & `readonce-1.0.3/tests/test_readonce.py`

 * *Files 21% similar despite different names*

```diff
@@ -115,15 +115,16 @@
     # This should fail with: "AttributeError: 'DBPassword' object has no attribute 'password'"
     with pytest.raises(AttributeError) as err:
         db = get_db_password_class("db-password")
 
 
 def test_use_sensitive_class_as_descriptor(get_db_credentials_with_desc_obj):
     db_port = get_db_credentials_with_desc_obj.port
-    assert db_port.get_secret() == 3306
+    # Integers are converted to strings
+    assert db_port.get_secret() == "3306"
     db_uri = get_db_credentials_with_desc_obj.uri
     assert db_uri.get_secret() == "mysql://"
 
     assert (
         get_db_credentials_with_desc_obj.__str__()
         == "DBCredentialsWithDescriptors(password=ReadOnce[secrets=*****], uri=ReadOnce[secrets=*****], port=ReadOnce[secrets=*****], host=ReadOnce[secrets=*****])"
     )
@@ -202,7 +203,71 @@
         get_invalid_db_credentials_model(
             comment="The Hacked Database",
             password=get_password_class("db-password"),  # valid length password
             uri=get_db_uri_class("mysql://"),
             host=get_db_host_class("localhost"),
             port=get_db_port(3306),
         )
+
+
+def test_monkeypatch_get_secret(get_password_obj, monkeypatch):
+    def mock_return():
+        return "12345"
+
+    get_password_obj.add_secret("new_secret")
+    monkeypatch.setattr(get_password_obj, "get_secret", mock_return)
+    # the original secret was not affected
+    assert get_password_obj.get_secret() != mock_return()
+
+
+def test_monkeypatch_add_secret(get_password_obj, monkeypatch):
+    def mock_return():
+        return "12345"
+
+    # basically has no effect on add_secret
+    monkeypatch.setattr(get_password_obj, "add_secret", mock_return)
+    get_password_obj.add_secret("fake")
+    monkeypatch.setattr(get_password_obj, "get_secret", mock_return)
+    # the original secret was not affected
+    assert get_password_obj.get_secret() != mock_return()
+
+
+def test_monkeypatch_change_secrets_property(get_password_obj, monkeypatch):
+    # It has no effect either for the secrets property
+    monkeypatch.setattr(get_password_obj, "secrets", ["12345"])
+    # Still original secret is there
+    assert get_password_obj.get_secret() != "12345"
+
+
+def test_monkeypatch_change_secrets_storage(get_password_obj, monkeypatch):
+    # Directly trying to monkeypatch will raise double UnsupportedOperationException;
+    # As monkeypatch in its default undo() section tries to again edit "_ReadOnce__secrets" which raises same exception
+    # That's why we use context() below
+
+    # with pytest.raises(UnsupportedOperationException):
+    #     monkeypatch.setattr(get_password_obj, "_ReadOnce__secrets", ["12345"], raising=False)
+
+    with pytest.raises(UnsupportedOperationException):
+        with monkeypatch.context() as m:
+            m.setattr(get_password_obj, "_ReadOnce__secrets", ["12345"], raising=True)
+
+
+def test_direct_access_to_key_field(get_password_obj):
+    assert get_password_obj.key is None
+    assert get_password_obj._ReadOnce__key is None
+
+    with pytest.raises(UnsupportedOperationException):
+        get_password_obj._ReadOnce__key = b"new key"
+
+    with pytest.raises(UnsupportedOperationException):
+        get_password_obj._ReadOnce__update_key(b"new key")
+
+    with pytest.raises(UnsupportedOperationException):
+        get_password_obj._ReadOnce__reset_key()
+
+
+def test_monkeypatch_the_key(get_password_obj, monkeypatch):
+    get_password_obj.add_secret("new_secret")
+
+    with pytest.raises(UnsupportedOperationException):
+        with monkeypatch.context() as m:
+            m.setattr(get_password_obj, "_ReadOnce__key", None)
```

### Comparing `readonce-1.0.2/PKG-INFO` & `readonce-1.0.3/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,25 +1,26 @@
 Metadata-Version: 2.1
 Name: readonce
-Version: 1.0.2
+Version: 1.0.3
 Summary: Read-Once Object implementation in Python - Inspired by Secure by Design book.
 Author-email: Shako Rzayev <rzayev.sehriyar@gmail.com>
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 Classifier: License :: OSI Approved :: MIT License
 Requires-Dist: icontract >=2.6.2
+Requires-Dist: cryptography >=40.0.2
 Requires-Dist: black >=22.3.0 ; extra == "dev"
 Requires-Dist: pylint >=2.12.2 ; extra == "dev"
 Requires-Dist: isort >=5.9.3 ; extra == "dev"
 Requires-Dist: autoflake >=1.4 ; extra == "dev"
 Requires-Dist: flake8 >=4.0.1 ; extra == "dev"
 Requires-Dist: pre-commit >=2.17.0 ; extra == "dev"
 Requires-Dist: pytype >=2022.1.31 ; extra == "dev"
 Requires-Dist: pydantic >=1.10.2 ; extra == "dev"
-Requires-Dist: pytest >=7.1.3 ; extra == "test"
+Requires-Dist: pytest >=7.3.1 ; extra == "test"
 Requires-Dist: pytest-cov >= 3.0.0 ; extra == "test"
 Provides-Extra: dev
 Provides-Extra: test
 
 # What is Read-Once object?
 
 This concept is defined and explained in [Secure by Design](https://www.manning.com/books/secure-by-design) book.
@@ -44,14 +45,38 @@
 ```
 
 # About the Usage
 
 Imagine that you need to pass a password it to some kind of service, which is going to Login your user.
 The Login service will only require this password only once, so why not to restrict it to be read, used only Once?
 
+# Important information
+
+The ReadOnce object is not a cryptography library. 
+It is not responsible for encrypting/decrypting or dictating any type of cryptography methods to store and retrieve your secrets.
+
+The main idea behind the ReadOnce objects is hardening the access and allow only one time access to the stored secrets in the object.
+
+Question: Are the secrets stored in plain text?
+Answer: No, we use symmetric encryption from cryptography named [Fernet](https://cryptography.io/en/latest/fernet/).
+And we store passed secret data internally as so called fernet token(ciphertext+hash value).
+When you try to retrieve the secret back, it is decrypted with the same key and send back as a plain text.
+
+Question: Then we have an encryption+hashing of plaintext?
+Answer: Yes, but ReadOnce class expects already encrypted(+ peppered, salted, hashed etc.) string to be passed as a secret, 
+because when you retrieve the secret it will return what it was originally passed. 
+If you passed the secret as "12345" you will get back "12345".
+If you passed the secret something like "HmDVbz6N3MlXqZ4q3TvLakMQ9fQjI45yhuoRHyZWiM4=" you will get back the same string.
+
+Question: Then why you store the secret as a token(ciphertext+hash value)?
+Answer: It is an extra layer of hardening, if somehow, somebody could get the ReadOnce object and tries to steal the secret, lovely attacker should also have the key.
+Okay the key also stored in ReadOnce object, but it is a non-trivial to get the key back. 
+If the attacker tries to add new secret over old one, the encryption key also updated.
+
+
 ### Install using pip:
 
 `pip install readonce`
 
 Then just inherit from the `ReadOnce`:
 
 ```py
@@ -457,38 +482,34 @@
     reg = r"^(?=.*[a-z])(?=.*[A-Z])(?=.*\d)(?=.*[@$!%*#?&])[A-Za-z\d@$!#%*?&]{6,20}$"
     pattern = re.compile(reg)
     return bool(re.search(pattern, password))
 ```
 
 After writing down password requirements you can convert them to `pre-conditions` as part of your DbC approach.
 
-* I used these ideas in the `ReadOnce` implementation as well, such as:
+# Is it possible to monkeypatch the secret logic management?
 
-```py
-@icontract.ensure(lambda self: not self.__secrets and not self.__is_consumed)
-def __init__(self) -> None:
-    self.__reset_secrets()
-    self.__reset_is_consumed()
-```
+As far, as I have tested it, 
+it is really non-trivial and over-hardened to monkeypatch the secret storage and also the secret management methods.
 
-Here I make myself to be sure that everything was reset properly.
-
-Another important topic is the invariants. Thinking about `ReadOnce` object, 
-at its lifecycle there can be either zero secret or only and only one secret:
+For eg, following test clearly shows the consequences:
 
 ```py
-@icontract.invariant(
-    lambda self: len(self) == 0 or len(self) == 1,
-    "There can be no or only single secret data stored",
-)
-class ReadOnce(metaclass=Final):
-    ...
-```
+def test_monkeypatch_change_secrets_storage(get_password_obj, monkeypatch):
+    # Directly trying to monkeypatch will raise double UnsupportedOperationException;
+    # As monkeypatch in its default undo() section tries to again edit "_ReadOnce__secrets" which raises same exception
+    # That's why we use context() below
+
+    # with pytest.raises(UnsupportedOperationException):
+    #     monkeypatch.setattr(get_password_obj, "_ReadOnce__secrets", ["12345"], raising=False)
 
-If somebody tries to inject more than one data to the secret storage, it will fail as it is a clear invariant violation.
+    with pytest.raises(UnsupportedOperationException):
+        with monkeypatch.context() as m:
+            m.setattr(get_password_obj, "_ReadOnce__secrets", ["12345"], raising=True)
+```
 
 
 # How to install for development?
 
 ### Create and activate the virtualenv:
 
 * `python3.10 -m venv .venv`
@@ -507,14 +528,10 @@
 
 ### Installing for general showcase
 
 `make install` or `flit install --env --deps=develop` 
 
 ### Run all tests in verbose
 
-`make test` or `pytest -svv` 
-
-
-# TODO
+`make test` or `pytest -svv`
 
-* Design by Contract ideas for ReadOnce object validation
```

