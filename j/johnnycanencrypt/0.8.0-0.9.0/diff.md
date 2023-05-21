# Comparing `tmp/johnnycanencrypt-0.8.0.tar.gz` & `tmp/johnnycanencrypt-0.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data
+gzip compressed data, was "johnnycanencrypt-0.9.0.tar", last modified: Tue Aug 30 12:56:57 2022, max compression
```

## Comparing `johnnycanencrypt-0.8.0.tar` & `johnnycanencrypt-0.9.0.tar`

### file list

```diff
@@ -1,57 +1,67 @@
--rw-r--r--   0        0        0     1776 1970-01-01 00:00:00.000000 johnnycanencrypt-0.8.0/Cargo.toml
--rw-r--r--   0     1000     1000     2896 2022-08-17 07:39:07.000000 johnnycanencrypt-0.8.0/.circleci/config.yml
--rw-r--r--   0     1000     1000       97 2021-12-27 09:28:41.000000 johnnycanencrypt-0.8.0/.gitignore
--rw-r--r--   0     1000     1000    35148 2021-12-27 09:28:41.000000 johnnycanencrypt-0.8.0/LICENSE
--rw-r--r--   0     1000     1000     1448 2022-08-17 07:39:07.000000 johnnycanencrypt-0.8.0/README.md
--rw-r--r--   0     1000     1000     3756 2022-08-18 18:44:38.000000 johnnycanencrypt-0.8.0/changelog.md
--rw-r--r--   0     1000     1000      582 2021-12-27 09:28:41.000000 johnnycanencrypt-0.8.0/dockerfiles/Dockerfile
--rw-r--r--   0     1000     1000      580 2021-12-27 09:28:41.000000 johnnycanencrypt-0.8.0/docs/Makefile
--rw-r--r--   0     1000     1000    11798 2022-08-18 18:44:38.000000 johnnycanencrypt-0.8.0/docs/api.rst
--rw-r--r--   0     1000     1000     1957 2021-12-27 09:28:41.000000 johnnycanencrypt-0.8.0/docs/build.rst
--rw-r--r--   0     1000     1000     5224 2022-08-18 18:44:38.000000 johnnycanencrypt-0.8.0/docs/conf.py
--rw-r--r--   0     1000     1000      763 2021-12-27 09:28:41.000000 johnnycanencrypt-0.8.0/docs/index.rst
--rw-r--r--   0     1000     1000     4312 2022-08-17 07:39:07.000000 johnnycanencrypt-0.8.0/docs/introduction.rst
--rw-r--r--   0     1000     1000     3630 2022-08-18 18:44:38.000000 johnnycanencrypt-0.8.0/docs/rustimplementation.rst
--rw-r--r--   0     1000     1000     7229 2022-08-18 18:44:38.000000 johnnycanencrypt-0.8.0/docs/smartcard.rst
--rw-r--r--   0     1000     1000    51324 2022-08-18 18:44:38.000000 johnnycanencrypt-0.8.0/johnnycanencrypt/__init__.py
--rw-r--r--   0     1000     1000       87 2021-12-27 09:28:41.000000 johnnycanencrypt-0.8.0/johnnycanencrypt/exceptions.py
--rw-r--r--   0     1000     1000     2135 2022-08-18 18:44:38.000000 johnnycanencrypt-0.8.0/johnnycanencrypt/utils.py
--rw-r--r--   0     1000     1000       65 2021-12-27 09:28:41.000000 johnnycanencrypt-0.8.0/mypy.ini
--rw-r--r--   0     1000     1000      111 2022-08-17 08:19:37.000000 johnnycanencrypt-0.8.0/pyproject.toml
--rw-r--r--   0     1000     1000       32 2021-12-27 09:28:41.000000 johnnycanencrypt-0.8.0/requirements-dev.txt
--rw-r--r--   0     1000     1000     8331 2021-12-27 09:28:41.000000 johnnycanencrypt-0.8.0/smartcardtests/2184DF8AF2CAFEB16357FE43E6F848F1DDC66C12.pub
--rw-r--r--   0     1000     1000    15474 2021-12-27 09:28:41.000000 johnnycanencrypt-0.8.0/smartcardtests/2184DF8AF2CAFEB16357FE43E6F848F1DDC66C12.sec
--rw-r--r--   0     1000     1000     2142 2021-12-27 09:28:41.000000 johnnycanencrypt-0.8.0/smartcardtests/5286C32E7C71E14C4C82F9AE0B207108925CB162.pub
--rw-r--r--   0     1000     1000     2495 2021-12-27 09:28:41.000000 johnnycanencrypt-0.8.0/smartcardtests/5286C32E7C71E14C4C82F9AE0B207108925CB162.sec
--rw-r--r--   0     1000     1000     4967 2022-08-17 07:39:07.000000 johnnycanencrypt-0.8.0/smartcardtests/smartcards.py
--rw-r--r--   0     1000     1000     1475 2022-08-18 18:44:38.000000 johnnycanencrypt-0.8.0/smartcardtests/smartcards_for_primary.py
--rw-r--r--   0     1000     1000    90447 2022-08-18 18:44:38.000000 johnnycanencrypt-0.8.0/src/lib.rs
--rw-r--r--   0     1000     1000    13889 2022-08-17 07:39:07.000000 johnnycanencrypt-0.8.0/src/scard.rs
--rw-r--r--   0     1000     1000        0 2021-12-27 09:28:41.000000 johnnycanencrypt-0.8.0/tests/__init__.py
--rw-r--r--   0     1000     1000      265 2021-12-27 09:28:41.000000 johnnycanencrypt-0.8.0/tests/conftest.py
--rw-r--r--   0     1000     1000     1016 2021-12-27 09:28:41.000000 johnnycanencrypt-0.8.0/tests/files/double_recipient.asc
--rw-r--r--   0     1000     1000     6262 2021-12-27 09:28:41.000000 johnnycanencrypt-0.8.0/tests/files/hellopublic.asc
--rw-r--r--   0     1000     1000    11595 2021-12-27 09:28:41.000000 johnnycanencrypt-0.8.0/tests/files/hellosecret.asc
--rw-r--r--   0     1000     1000     1301 2021-12-27 09:28:41.000000 johnnycanencrypt-0.8.0/tests/files/public.asc
--rw-r--r--   0     1000     1000     1544 2021-12-27 09:28:41.000000 johnnycanencrypt-0.8.0/tests/files/secret.asc
--rw-r--r--   0     1000     1000     1761 2021-12-27 09:28:41.000000 johnnycanencrypt-0.8.0/tests/files/store/FC3CE1AD6229F4CC89571D1CB4741BF4DDA4BA62.pub
--rw-r--r--   0     1000     1000     6262 2021-12-27 09:28:41.000000 johnnycanencrypt-0.8.0/tests/files/store/hellopublic.asc
--rw-r--r--   0     1000     1000    11595 2021-12-27 09:28:41.000000 johnnycanencrypt-0.8.0/tests/files/store/hellosecret.asc
--rw-r--r--   0     1000     1000    61440 2022-08-18 18:44:38.000000 johnnycanencrypt-0.8.0/tests/files/store/jce.db
--rw-r--r--   0     1000     1000    61894 2021-12-27 09:28:41.000000 johnnycanencrypt-0.8.0/tests/files/store/kushal_updated_key.asc
--rw-r--r--   0     1000     1000    57344 2021-12-27 09:28:41.000000 johnnycanencrypt-0.8.0/tests/files/store/oldjce.db
--rw-r--r--   0     1000     1000     9480 2021-12-27 09:28:41.000000 johnnycanencrypt-0.8.0/tests/files/store/pgp_keys.asc
--rw-r--r--   0     1000     1000     1301 2021-12-27 09:28:41.000000 johnnycanencrypt-0.8.0/tests/files/store/public.asc
--rw-r--r--   0     1000     1000     1544 2021-12-27 09:28:41.000000 johnnycanencrypt-0.8.0/tests/files/store/secret.asc
--rw-r--r--   0     1000     1000     9478 2021-12-27 09:28:41.000000 johnnycanencrypt-0.8.0/tests/files/test_fetch_key_by_email.yml
--rw-r--r--   0     1000     1000    24616 2021-12-27 09:28:41.000000 johnnycanencrypt-0.8.0/tests/files/test_fetch_key_by_fingerprint.yml
--rw-r--r--   0     1000     1000      869 2021-12-27 09:28:41.000000 johnnycanencrypt-0.8.0/tests/files/test_fetch_nonexistingkey_by_email.yml
--rw-r--r--   0     1000     1000      858 2021-12-27 09:28:41.000000 johnnycanencrypt-0.8.0/tests/files/test_fetch_nonexistingkey_by_fingerprint.yml
--rw-r--r--   0     1000     1000     3137 2021-12-27 09:28:41.000000 johnnycanencrypt-0.8.0/tests/files/test_journalist_key.pub
--rw-r--r--   0     1000     1000      187 2021-12-27 09:28:41.000000 johnnycanencrypt-0.8.0/tests/files/text.txt
--rw-r--r--   0     1000     1000     7615 2021-12-27 09:28:41.000000 johnnycanencrypt-0.8.0/tests/test_encrypt_decrypt.py
--rw-r--r--   0     1000     1000    21075 2022-08-18 18:44:38.000000 johnnycanencrypt-0.8.0/tests/test_keystore.py
--rw-r--r--   0     1000     1000     2608 2022-08-18 18:44:38.000000 johnnycanencrypt-0.8.0/tests/test_parse_cert.py
--rw-r--r--   0     1000     1000     3569 2022-08-17 07:39:07.000000 johnnycanencrypt-0.8.0/tests/test_sign_verify_bytes.py
--rw-r--r--   0     1000     1000      629 2021-12-27 09:28:41.000000 johnnycanencrypt-0.8.0/tests/utils.py
--rw-r--r--   0        0        0     2690 1970-01-01 00:00:00.000000 johnnycanencrypt-0.8.0/PKG-INFO
+drwxr-xr-x   0 kdas      (1000) kdas      (1000)        0 2022-08-30 12:56:57.908221 johnnycanencrypt-0.9.0/
+-rw-r--r--   0 kdas      (1000) kdas      (1000)     1776 2022-08-30 08:16:34.000000 johnnycanencrypt-0.9.0/Cargo.toml
+-rw-r--r--   0 kdas      (1000) kdas      (1000)    35148 2021-12-27 09:28:41.000000 johnnycanencrypt-0.9.0/LICENSE
+-rw-r--r--   0 kdas      (1000) kdas      (1000)      223 2022-08-30 12:16:07.000000 johnnycanencrypt-0.9.0/MANIFEST.in
+-rw-r--r--   0 kdas      (1000) kdas      (1000)     2406 2022-08-30 12:56:57.908221 johnnycanencrypt-0.9.0/PKG-INFO
+-rw-r--r--   0 kdas      (1000) kdas      (1000)     1446 2022-08-30 11:23:49.000000 johnnycanencrypt-0.9.0/README.md
+-rw-r--r--   0 kdas      (1000) kdas      (1000)     4050 2022-08-30 11:23:49.000000 johnnycanencrypt-0.9.0/changelog.md
+drwxr-xr-x   0 kdas      (1000) kdas      (1000)        0 2022-08-30 12:56:57.904221 johnnycanencrypt-0.9.0/docs/
+-rw-r--r--   0 kdas      (1000) kdas      (1000)      580 2021-12-27 09:28:41.000000 johnnycanencrypt-0.9.0/docs/Makefile
+-rw-r--r--   0 kdas      (1000) kdas      (1000)    12986 2022-08-30 08:16:34.000000 johnnycanencrypt-0.9.0/docs/api.rst
+-rw-r--r--   0 kdas      (1000) kdas      (1000)     1978 2022-08-30 08:16:34.000000 johnnycanencrypt-0.9.0/docs/build.rst
+-rw-r--r--   0 kdas      (1000) kdas      (1000)     5224 2022-08-30 11:23:49.000000 johnnycanencrypt-0.9.0/docs/conf.py
+-rw-r--r--   0 kdas      (1000) kdas      (1000)      763 2021-12-27 09:28:41.000000 johnnycanencrypt-0.9.0/docs/index.rst
+-rw-r--r--   0 kdas      (1000) kdas      (1000)     4312 2022-08-17 07:39:07.000000 johnnycanencrypt-0.9.0/docs/introduction.rst
+-rw-r--r--   0 kdas      (1000) kdas      (1000)     3630 2022-08-18 18:44:38.000000 johnnycanencrypt-0.9.0/docs/rustimplementation.rst
+-rw-r--r--   0 kdas      (1000) kdas      (1000)     7229 2022-08-18 18:44:38.000000 johnnycanencrypt-0.9.0/docs/smartcard.rst
+drwxr-xr-x   0 kdas      (1000) kdas      (1000)        0 2022-08-30 12:56:57.905221 johnnycanencrypt-0.9.0/johnnycanencrypt/
+-rw-r--r--   0 kdas      (1000) kdas      (1000)    56379 2022-08-30 08:16:34.000000 johnnycanencrypt-0.9.0/johnnycanencrypt/__init__.py
+-rw-r--r--   0 kdas      (1000) kdas      (1000)       87 2021-12-27 09:28:41.000000 johnnycanencrypt-0.9.0/johnnycanencrypt/exceptions.py
+-rw-r--r--   0 kdas      (1000) kdas      (1000)     2743 2022-08-30 08:16:34.000000 johnnycanencrypt-0.9.0/johnnycanencrypt/utils.py
+drwxr-xr-x   0 kdas      (1000) kdas      (1000)        0 2022-08-30 12:56:57.905221 johnnycanencrypt-0.9.0/johnnycanencrypt.egg-info/
+-rw-r--r--   0 kdas      (1000) kdas      (1000)     2406 2022-08-30 12:56:57.000000 johnnycanencrypt-0.9.0/johnnycanencrypt.egg-info/PKG-INFO
+-rw-r--r--   0 kdas      (1000) kdas      (1000)     1530 2022-08-30 12:56:57.000000 johnnycanencrypt-0.9.0/johnnycanencrypt.egg-info/SOURCES.txt
+-rw-r--r--   0 kdas      (1000) kdas      (1000)        1 2022-08-30 12:56:57.000000 johnnycanencrypt-0.9.0/johnnycanencrypt.egg-info/dependency_links.txt
+-rw-r--r--   0 kdas      (1000) kdas      (1000)        1 2022-08-30 11:24:16.000000 johnnycanencrypt-0.9.0/johnnycanencrypt.egg-info/not-zip-safe
+-rw-r--r--   0 kdas      (1000) kdas      (1000)        6 2022-08-30 12:56:57.000000 johnnycanencrypt-0.9.0/johnnycanencrypt.egg-info/requires.txt
+-rw-r--r--   0 kdas      (1000) kdas      (1000)       17 2022-08-30 12:56:57.000000 johnnycanencrypt-0.9.0/johnnycanencrypt.egg-info/top_level.txt
+-rw-r--r--   0 kdas      (1000) kdas      (1000)       65 2021-12-27 09:28:41.000000 johnnycanencrypt-0.9.0/mypy.ini
+-rw-r--r--   0 kdas      (1000) kdas      (1000)      971 2022-08-30 12:16:07.000000 johnnycanencrypt-0.9.0/pyproject.toml
+-rw-r--r--   0 kdas      (1000) kdas      (1000)       57 2022-08-30 08:16:34.000000 johnnycanencrypt-0.9.0/requirements-dev.txt
+-rw-r--r--   0 kdas      (1000) kdas      (1000)       38 2022-08-30 12:56:57.909221 johnnycanencrypt-0.9.0/setup.cfg
+-rw-r--r--   0 kdas      (1000) kdas      (1000)      355 2022-08-30 08:16:34.000000 johnnycanencrypt-0.9.0/setup.py
+drwxr-xr-x   0 kdas      (1000) kdas      (1000)        0 2022-08-30 12:56:57.905221 johnnycanencrypt-0.9.0/src/
+-rw-r--r--   0 kdas      (1000) kdas      (1000)    97301 2022-08-30 08:16:34.000000 johnnycanencrypt-0.9.0/src/lib.rs
+-rw-r--r--   0 kdas      (1000) kdas      (1000)    13906 2022-08-30 08:16:34.000000 johnnycanencrypt-0.9.0/src/scard.rs
+drwxr-xr-x   0 kdas      (1000) kdas      (1000)        0 2022-08-30 12:56:57.906221 johnnycanencrypt-0.9.0/tests/
+-rw-r--r--   0 kdas      (1000) kdas      (1000)        0 2021-12-27 09:28:41.000000 johnnycanencrypt-0.9.0/tests/__init__.py
+-rw-r--r--   0 kdas      (1000) kdas      (1000)      265 2021-12-27 09:28:41.000000 johnnycanencrypt-0.9.0/tests/conftest.py
+drwxr-xr-x   0 kdas      (1000) kdas      (1000)        0 2022-08-30 12:56:57.907221 johnnycanencrypt-0.9.0/tests/files/
+-rw-r--r--   0 kdas      (1000) kdas      (1000)     1016 2021-12-27 09:28:41.000000 johnnycanencrypt-0.9.0/tests/files/double_recipient.asc
+-rw-r--r--   0 kdas      (1000) kdas      (1000)     6262 2021-12-27 09:28:41.000000 johnnycanencrypt-0.9.0/tests/files/hellopublic.asc
+-rw-r--r--   0 kdas      (1000) kdas      (1000)    11595 2021-12-27 09:28:41.000000 johnnycanencrypt-0.9.0/tests/files/hellosecret.asc
+-rw-r--r--   0 kdas      (1000) kdas      (1000)     1325 2022-08-30 08:16:34.000000 johnnycanencrypt-0.9.0/tests/files/primary_with_sign.asc
+-rw-r--r--   0 kdas      (1000) kdas      (1000)     1192 2022-08-30 08:16:34.000000 johnnycanencrypt-0.9.0/tests/files/primary_with_sign_public.asc
+-rw-r--r--   0 kdas      (1000) kdas      (1000)     1301 2021-12-27 09:28:41.000000 johnnycanencrypt-0.9.0/tests/files/public.asc
+-rw-r--r--   0 kdas      (1000) kdas      (1000)     1544 2021-12-27 09:28:41.000000 johnnycanencrypt-0.9.0/tests/files/secret.asc
+drwxr-xr-x   0 kdas      (1000) kdas      (1000)        0 2022-08-30 12:56:57.908221 johnnycanencrypt-0.9.0/tests/files/store/
+-rw-r--r--   0 kdas      (1000) kdas      (1000)     1761 2021-12-27 09:28:41.000000 johnnycanencrypt-0.9.0/tests/files/store/FC3CE1AD6229F4CC89571D1CB4741BF4DDA4BA62.pub
+-rw-r--r--   0 kdas      (1000) kdas      (1000)     6262 2021-12-27 09:28:41.000000 johnnycanencrypt-0.9.0/tests/files/store/hellopublic.asc
+-rw-r--r--   0 kdas      (1000) kdas      (1000)    11595 2021-12-27 09:28:41.000000 johnnycanencrypt-0.9.0/tests/files/store/hellosecret.asc
+-rw-r--r--   0 kdas      (1000) kdas      (1000)    69632 2022-08-30 08:16:34.000000 johnnycanencrypt-0.9.0/tests/files/store/jce.db
+-rw-r--r--   0 kdas      (1000) kdas      (1000)    61894 2021-12-27 09:28:41.000000 johnnycanencrypt-0.9.0/tests/files/store/kushal_updated_key.asc
+-rw-r--r--   0 kdas      (1000) kdas      (1000)    57344 2021-12-27 09:28:41.000000 johnnycanencrypt-0.9.0/tests/files/store/oldjce.db
+-rw-r--r--   0 kdas      (1000) kdas      (1000)     9480 2021-12-27 09:28:41.000000 johnnycanencrypt-0.9.0/tests/files/store/pgp_keys.asc
+-rw-r--r--   0 kdas      (1000) kdas      (1000)     1301 2021-12-27 09:28:41.000000 johnnycanencrypt-0.9.0/tests/files/store/public.asc
+-rw-r--r--   0 kdas      (1000) kdas      (1000)     1544 2021-12-27 09:28:41.000000 johnnycanencrypt-0.9.0/tests/files/store/secret.asc
+-rw-r--r--   0 kdas      (1000) kdas      (1000)     9478 2021-12-27 09:28:41.000000 johnnycanencrypt-0.9.0/tests/files/test_fetch_key_by_email.yml
+-rw-r--r--   0 kdas      (1000) kdas      (1000)    24616 2021-12-27 09:28:41.000000 johnnycanencrypt-0.9.0/tests/files/test_fetch_key_by_fingerprint.yml
+-rw-r--r--   0 kdas      (1000) kdas      (1000)      869 2021-12-27 09:28:41.000000 johnnycanencrypt-0.9.0/tests/files/test_fetch_nonexistingkey_by_email.yml
+-rw-r--r--   0 kdas      (1000) kdas      (1000)      858 2021-12-27 09:28:41.000000 johnnycanencrypt-0.9.0/tests/files/test_fetch_nonexistingkey_by_fingerprint.yml
+-rw-r--r--   0 kdas      (1000) kdas      (1000)     3137 2021-12-27 09:28:41.000000 johnnycanencrypt-0.9.0/tests/files/test_journalist_key.pub
+-rw-r--r--   0 kdas      (1000) kdas      (1000)      187 2021-12-27 09:28:41.000000 johnnycanencrypt-0.9.0/tests/files/text.txt
+-rw-r--r--   0 kdas      (1000) kdas      (1000)     7615 2021-12-27 09:28:41.000000 johnnycanencrypt-0.9.0/tests/test_encrypt_decrypt.py
+-rw-r--r--   0 kdas      (1000) kdas      (1000)    22559 2022-08-30 08:16:34.000000 johnnycanencrypt-0.9.0/tests/test_keystore.py
+-rw-r--r--   0 kdas      (1000) kdas      (1000)     3673 2022-08-30 08:16:34.000000 johnnycanencrypt-0.9.0/tests/test_parse_cert.py
+-rw-r--r--   0 kdas      (1000) kdas      (1000)     3569 2022-08-17 07:39:07.000000 johnnycanencrypt-0.9.0/tests/test_sign_verify_bytes.py
+-rw-r--r--   0 kdas      (1000) kdas      (1000)      629 2021-12-27 09:28:41.000000 johnnycanencrypt-0.9.0/tests/utils.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `johnnycanencrypt-0.8.0/Cargo.toml` & `johnnycanencrypt-0.9.0/Cargo.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [package]
 name = "johnnycanencrypt"
-version = "0.8.0"
+version = "0.9.0"
 authors = ["Kushal Das <mail@kushaldas.in>"]
 edition = "2018"
 description = "Python module for OpenPGP."
 documentation = "https://johnnycanencrypt.readthedocs.io/en/latest/index.html"
 readme = "README.md"
 homepage = "https://johnnycanencrypt.readthedocs.io/en/latest/introduction.html"
 repository = "https://github.com/kushaldas/johnnycanencrypt"
@@ -23,15 +23,15 @@
 
 [dependencies]
 sequoia-openpgp = "1.0.0"
 anyhow = "1.0.62"
 chrono = "0.4.22"
 tempfile = "3.0.0"
 #talktosc = { git = "https://github.com/kushaldas/talktosc", branch="main"}
-talktosc = "0.1.2"
+talktosc = "0.1.3"
  
 [dependencies.pyo3]
 version = "0.16.4"
 
 
 [package.metadata.maturin]
 classifier = [
```

### Comparing `johnnycanencrypt-0.8.0/LICENSE` & `johnnycanencrypt-0.9.0/LICENSE`

 * *Files identical despite different names*

### Comparing `johnnycanencrypt-0.8.0/README.md` & `johnnycanencrypt-0.9.0/README.md`

 * *Files 22% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # Johnny can encrypt
 
-[![CircleCI branch](https://img.shields.io/circleci/project/github/kushaldas/johnnycanencrypt/master.svg)](https://circleci.com/gh/kushaldas/workflows/johnnycanencrypt/tree/master)
+[![CircleCI branch](https://img.shields.io/circleci/project/github/kushaldas/johnnycanencrypt/main.svg)](https://circleci.com/gh/kushaldas/workflows/johnnycanencrypt/tree/main)
 
 Johnnycanencrypt aka **jce** is a Python module written in Rust to do basic encryption and decryption, and detached signing operations.
 It uses amazing [sequoia-pgp](https://sequoia-pgp.org/) library for the actual OpenPGP operations.
 
 You can also use Yubikeys for the private key operations using this module.
 
 
@@ -14,37 +14,38 @@
 
 ### Build dependencies in Fedora
 
 ```
 sudo dnf install nettle clang clang-devel nettle-devel python3-devel pcsc-lite-devel
 ```
 
-### Build dependencies in Debian Buster
+### Build dependencies in Debian Bullseye
 
 ```
-sudo apt install -y python3-dev libnettle6 nettle-dev libhogweed4 python3-pip python3-venv clang libpcsclite-dev
+sudo apt install -y python3-dev libnettle8 nettle-dev libhogweed6 python3-pip python3-venv clang libpcsclite-dev libpcsclite1 libclang-9-dev
+
 ```
 
-Finally build the module using `maturin`.
 
 ```
 python3 -m venv .venv
 source .venv/bin/activate
 python3 -m pip install -r requirements-dev.txt
-maturin develop
+python setup.py develop
 ```
 
 For a release build use the following command.
 
 ```
-maturin build --release
+python setup.py bdist_wheel
 ```
 
 ## Introduction
 
 Please read the [Introduction](https://johnnycanencrypt.readthedocs.io/en/latest/introduction.html) documentation.
 
 ## API documentation
 
 Please go through the [full API documentation](https://johnnycanencrypt.readthedocs.io/en/latest/api.html) for detailed descriptions.
 
 ## LICENSE: GPLv3+
+
```

### Comparing `johnnycanencrypt-0.8.0/changelog.md` & `johnnycanencrypt-0.9.0/changelog.md`

 * *Files 16% similar despite different names*

```diff
@@ -1,9 +1,18 @@
 # Changlelog
 
+## [unreleased]
+
+## [0.9.0] - 2022-08-30
+
+- Adds `setuptools-rust` as build system.
+- Key.uids now contains the certification details of each user id.
+- `merge_keys` in rjce now takes a force boolean argument.
+- `certify_key` can sign/certify another key by both card and on disk primary key.
+
 ## [0.8.0] - 2022-08-18
 
 ### Added
 
 - #96 `create_key` can now have signing capability for primary key.
 - #97 `sync_smartcard` can identify if the primary key is on card.
 - `upload_primary_to_smartcard` function in rjce.
```

### Comparing `johnnycanencrypt-0.8.0/docs/Makefile` & `johnnycanencrypt-0.9.0/docs/Makefile`

 * *Files identical despite different names*

### Comparing `johnnycanencrypt-0.8.0/docs/api.rst` & `johnnycanencrypt-0.9.0/docs/api.rst`

 * *Files 5% similar despite different names*

```diff
@@ -9,33 +9,43 @@
         >>> import johnnycanencrypt as jce
 
 
 
 
 .. class:: KeyStore(path: str) -> None:
 
-        Returns a KeyStore object. This is the primary class of the module, and all high level usage is available via methods of this class.
-        It takes a path to the directory where it stores/reads the keys. Please make sure that only the **user** has read/write capability
-        to this path.
+        Returns a KeyStore object. This is the primary class of the module, and
+        all high level usage is available via methods of this class. It takes a
+        path to the directory where it stores/reads the keys. Please make sure
+        that only the **user** has read/write capability to this path.
+
+        The keys are represented inside the directory in the **jce.db** sqlite3
+        database. Every time there is any change in the DB schema, we
+        automatically create a temporary database called **jce_upgrade.db** in
+        the same path, and then reimport all the keys, and rename the file and
+        continue with the steps. This is one time operation when we do a new
+        release.
 
-        The keys are represented inside the directory in the **jce.db** sqlite3 database
-
-        If you can check for existance of any fingerprint (str) or `Key` object in the via `in` opertor.
+        You can check for existance of any fingerprint (str) or `Key` object in the via `in` opertor.
 
         ::
 
                 >>> ks = jce.KeyStore("/var/lib/myamazingapp")
                 >>> "HEXFINGERPRINT" in ks
 
 
         .. method:: add_userid(key: Key, userid: str, password: str) -> Key:
 
                 Returns the updated key with a new userid. If you need to upload the key to the https://keys.openpgp.org, then remember to
                 have to an email address in the user id.
 
+        .. method:: certify_key(key: Union[Key, str], otherkey: Union[Key, str], uids: List[str], sig_type: SignatureType = SignatureType.GenericCertification, password: str = "", oncard=False) -> Key:
+
+                This method signs the given list of userid(s) in `otherkey` using the primary key of the `key`, by default it signs as *SignatureType.GenericCertification*, but you can do other types too. If the primary key is on a smartcard, then pass `oncard=True`, default value is `False`.
+
         .. method:: create_key(password: str, uids: Optional[Union[List[str], str]] = [], ciphersuite: Cipher = Cipher.RSA4k, creation: Optional[datetime.datetime] = None, expiration: Optional[datetime.datetime] = None, subkeys_expiration= False, whichkeys = 7, can_primary_sign: bool = True) -> Key:
 
                 Returns the public part of the newly created `Key` in the store
                 directory. You can mention ciphersuite :class:`Cipher`  as
                 *Cipher.RSA2k* or *Cipher.RSA4k*, or *Cipher.Cv25519*, while
                 *Cipher.RSA4k* is the default. You can also provide
                 `datetime.datetime` objects for creation time and expiration
@@ -206,15 +216,15 @@
 
         .. attribute:: fingerprint
 
                 The string representation of the fingerprint
 
         .. attribute:: uids
 
-                A dictionary holding all uids from the key.
+                A dictionary holding all uids from the key, also stores related **certification** of the given uids.
 
         .. attribute:: creationtime
 
                 The datetime.datetime object mentioning when the key was created.
 
         .. attribute:: expirationtime
 
@@ -248,7 +258,12 @@
 
                 Returns a tuple with 3 boolean values as (got_enc, got_sign, got_auth) to tell us which all subkeys are available.
                 The subkeys will not be expired keys (based on the date of the system) and also not revoked.
 
 .. class:: KeyType() -> KeyType:
 
         Enum class to mark if a key is public or private. Possible values are **KeyType.PUBLIC** and **KeyType.SECRET**.
+
+.. class:: SignatureType() -> SignatureType:
+
+        Enum class to mark the kind of certification one can do on another key. Possible values are **SignatureType.GenericCertification**,
+        **SignatureType.PersonaCertification**, **SignatureType.CasualCertification**, **SignatureType.PositiveCertification**.
```

### Comparing `johnnycanencrypt-0.8.0/docs/build.rst` & `johnnycanencrypt-0.9.0/docs/build.rst`

 * *Files 16% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 Building this module requires Rust's nightly toolchain. You can install it following
 the instructions from `rustup.rs <https://rustup.rs>`_.
 
 You will need `libnettle` and `libnettle-dev` & `clang`, `libpcsclite1`, `libpcsclite-dev` (on Debian/Ubuntu) and `nettle` & `nettle-dev` `pcsc-lite-devel` & `clang` packages in Fedora.
 
 ::
 
-        sudo apt install -y python3-dev libnettle6 nettle-dev libhogweed4 python3-pip python3-venv clang libpcsclite-dev libpcsclite1
+        sudo apt install -y python3-dev libnettle8 nettle-dev libhogweed6 python3-pip python3-venv clang libpcsclite-dev libpcsclite1 libclang-9-dev
 
 ::
 
         sudo dnf install nettle clang clang-devel nettle-devel python3-devel pcsc-lite-devel 
 
 
 Then you can just use `pip` module to install in your virtualenvironment.
@@ -28,38 +28,38 @@
 
 After you have the dependencies mentioned above, you can follow the steps below to build a wheel.
 
 ::
 
         python3 -m venv .venv
         source .venv/bin/activate
-        python3 -m pip install -r requirements-dev.txt
-        maturin build --manylinux=off
+        python -m pip install -r requirements-dev.txt
+        python setup.py develop
 
 Only to build and test locally, you should execute
 
 ::
 
-        maturin develop
+        python setup.py develop
 
 
 To build a wheel use the following command.
 
 ::
 
-        maturin build --manylinux=off
+        python setup.py bdist_wheel
 
 How to run the tests?
 ----------------------
 
-After you did the `maturin develop` as mentioned above, execute the following command.
+After you did the `python setup.py develop` as mentioned above, execute the following command.
 
 ::
 
-        python3 -m pytest -vvv
+        python -m pytest -vvv
 
 
 How to run the smartcard related tests?
 ---------------------------------------
 
 .. warning:: The following test will reset any Yubikey or smartcard connected to the system. Use it carefully.
```

### Comparing `johnnycanencrypt-0.8.0/docs/conf.py` & `johnnycanencrypt-0.9.0/docs/conf.py`

 * *Files 1% similar despite different names*

```diff
@@ -20,17 +20,17 @@
 # -- Project information -----------------------------------------------------
 
 project = 'Johnny Can Encrypt'
 copyright = '2020-2022, Kushal Das'
 author = 'Kushal Das'
 
 # The short X.Y version
-version = '0.8.0'
+version = '0.9.0'
 # The full version, including alpha/beta/rc tags
-release = '0.8.0'
+release = '0.9.0'
 
 
 # -- General configuration ---------------------------------------------------
 
 # If your documentation needs a minimal Sphinx version, state it here.
 #
 # needs_sphinx = '1.0'
```

### Comparing `johnnycanencrypt-0.8.0/docs/index.rst` & `johnnycanencrypt-0.9.0/docs/index.rst`

 * *Files identical despite different names*

### Comparing `johnnycanencrypt-0.8.0/docs/introduction.rst` & `johnnycanencrypt-0.9.0/docs/introduction.rst`

 * *Files identical despite different names*

### Comparing `johnnycanencrypt-0.8.0/docs/rustimplementation.rst` & `johnnycanencrypt-0.9.0/docs/rustimplementation.rst`

 * *Files identical despite different names*

### Comparing `johnnycanencrypt-0.8.0/docs/smartcard.rst` & `johnnycanencrypt-0.9.0/docs/smartcard.rst`

 * *Files identical despite different names*

### Comparing `johnnycanencrypt-0.8.0/johnnycanencrypt/__init__.py` & `johnnycanencrypt-0.9.0/johnnycanencrypt/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -43,14 +43,23 @@
 
 class Cipher(Enum):
     RSA4k = "RSA4k"
     RSA2k = "RSA2k"
     Cv25519 = "Cv25519"
 
 
+class SignatureType(Enum):
+    """This is used for key signing via certification"""
+
+    GenericCertification = 0
+    PersonaCertification = 1
+    CasualCertification = 2
+    PositiveCertification = 3
+
+
 class Key:
     "Returns a Key object."
 
     def __init__(
         self,
         keyvalue: bytes,
         fingerprint: str,
@@ -229,14 +238,70 @@
             cursor = con.cursor()
             sql = "UPDATE keys set keyvalue=? where fingerprint=?"
             cursor.execute(sql, (cert, key.fingerprint))
         assert cert != key.keyvalue
         key.keyvalue = cert
         return key
 
+    def certify_key(
+        self,
+        key: Union[Key, str],
+        otherkey: Union[Key, str],
+        uids: List[str],
+        sig_type: SignatureType = SignatureType.GenericCertification,
+        password: str = "",
+        oncard=False,
+    ) -> Key:
+        """Certifies the given uids based on a list of values. Returns the new key.
+
+        :param key: Fingerprint or secret Key object using which we will certify.
+        :param other_key: Fingerprint or Key object whom we will certify.
+        :param uids: List of uid values which we will certify using the given SignatureType.
+        :param sig_type: SignatureType, default is SignatureType.GenericCertification
+        :param password: Password of the secret key file or the pin if on card.
+        """
+        if isinstance(key, str):  # Means we have a fingerprint
+            k = self.get_key(key)
+        else:
+            k = key
+
+        if isinstance(otherkey, str):  # Means we have a fingerprint
+            other_k = self.get_key(otherkey)
+        else:
+            other_k  = otherkey
+
+        cert = rjce.certify_key(
+            k.keyvalue, other_k.keyvalue, sig_type.value, uids, password, oncard
+        )
+        # Now if the otherkey is secret, then merge this new public key into the secret key
+        if other_k.keytype == KeyType.SECRET:
+            cert = rjce.merge_keys(other_k.keyvalue, cert, True)
+        # first remove the old one
+        self.delete_key(otherkey)
+        # Now add back the new updated key
+        (
+            uids,
+            fingerprint,
+            keytype,
+            expirationtime,
+            creationtime,
+            othervalues,
+        ) = parse_cert_bytes(cert)
+
+        self._save_key_info_to_db(
+            cert,
+            uids,
+            fingerprint,
+            keytype,
+            expirationtime,
+            creationtime,
+            othervalues,
+        )
+        return self.get_key(fingerprint)
+
     def add_key_file_to_db(
         self,
         fullpath,
         uids,
         fingerprint,
         keytype,
         expirationtime=None,
@@ -278,15 +343,15 @@
             if fromdb:  # Means a key is there in the db
                 key_id = fromdb["id"]
                 sql = "UPDATE keys SET keyvalue=?, keytype=?, expiration=?, creation=? WHERE id=?"
                 if (
                     fromdb["keytype"] == 0
                 ):  # only update if there is a public key in the store
                     key = self.get_key(fingerprint)
-                    newcert = merge_keys(key.keyvalue, cert)
+                    newcert = merge_keys(key.keyvalue, cert, False)
                     uids, fp, kt, et, ct, othervalues = parse_cert_bytes(newcert)
                     etime = str(et.timestamp()) if et else ""
                     ctime = str(ct.timestamp()) if ct else ""
                 else:  # Means another secret to replace
                     # We will not do anything, if you want reimport for a secret key
                     # delete the old one, and import the new one
                     # TODO: We should also raise SameKeyError here
@@ -328,14 +393,37 @@
             for uid in uids:
                 # First we will insert the value
                 if "value" in uid and uid["value"]:
                     revoked = 1 if uid["revoked"] else 0
                     sql = f"INSERT INTO uidvalues (value, revoked, key_id) values (?, ?, ?)"
                     cursor.execute(sql, (uid["value"], revoked, key_id))
                     value_id = cursor.lastrowid
+                    # After we added the value, we should check for certification
+                    if len(uid["certifications"]) > 0:
+                        for ucert in uid["certifications"]:
+                            ctime = (
+                                str(ucert["creationtime"].timestamp())
+                                if ucert["creationtime"]
+                                else ""
+                            )
+                            sql = f"INSERT INTO uidcerts (ctype, creation, key_id, value_id) values (?, ?, ?, ?)"
+                            cursor.execute(
+                                sql,
+                                (ucert["certification_type"], ctime, key_id, value_id),
+                            )
+                            # This is the ID of the certification we just added to the database
+                            ucert_id = cursor.lastrowid
+                            # Now time to loop over the details and add them
+                            for citem in ucert["certification_list"]:
+                                # citem is like [('fingerprint', 'F7FC698FAAE2D2EFBECDE98ED1B3ADC0E0238CA6'), ('keyid', 'D1B3ADC0E0238CA6')]
+                                sql = f"INSERT INTO uidcertlist (value, datatype, key_id, value_id, cert_id) values (?, ?, ?, ?, ?)"
+                                cursor.execute(
+                                    sql,
+                                    (citem[1], citem[0], key_id, value_id, ucert_id),
+                                )
                 else:
                     # If no value, then we can skip the rest
                     continue
                 for uid_keyname in ["name", "email", "uri"]:
                     if uid_keyname in uid and uid[uid_keyname]:
                         tablename = f"uid{uid_keyname}s"
                         value = uid[uid_keyname]
@@ -637,14 +725,15 @@
             if not result:
                 KeyNotFoundError(f"The key with keyid {keyid} is not found.")
             return result
 
     def _internal_build_key_list(self, rows, cursor):
         "Internal method to create a list of keys from db result rows"
         finalresult = []
+        sql_for_certs = "SELECT value, datatype FROM uidcertlist WHERE cert_id=?"
         for result in rows:
             if result:
                 key_id = result["id"]
                 cert = result["keyvalue"]
                 fingerprint = result["fingerprint"]
                 keyid = result["keyid"]
                 expirationtime = result["expiration"]
@@ -661,21 +750,43 @@
                 uids = []
                 for row in rows:
                     value_id = row["id"]
                     revoked = True if row["revoked"] == 1 else False
                     email = self._get_one_row_from_table(cursor, "uidemails", value_id)
                     name = self._get_one_row_from_table(cursor, "uidnames", value_id)
                     uri = self._get_one_row_from_table(cursor, "uiduris", value_id)
+                    # Now time to find any certification for the uid value
+                    # TODO: Write a join query in future please
+                    csql = "SELECT id, ctype, creation FROM uidcerts WHERE key_id=? and value_id=?"
+                    cursor.execute(csql, (key_id, value_id))
+                    certrows = cursor.fetchall()
+                    # let us loop over all the certs
+                    certifications = []
+                    for uidcert in certrows:
+                        cert_result = {}
+                        cert_result["creationtime"] = uidcert["creation"]
+                        cert_result["certification_type"] = uidcert["ctype"]
+                        ucertid = uidcert["id"]
+                        cert_issuers = cursor.execute(sql_for_certs, (ucertid,))
+                        issuers = []
+                        for cissuer in cert_issuers:
+                            issuers.append((cissuer["datatype"], cissuer["value"]))
+                        # now put it in the right place
+                        cert_result["certification_list"] = issuers
+                        # Now put all the data in the right place
+                        certifications.append(cert_result)
+
                     uids.append(
                         {
                             "value": row["value"],
                             "revoked": revoked,
                             "email": email,
                             "name": name,
                             "uri": uri,
+                            "certifications": certifications,
                         }
                     )
 
                 # Get the subkeys
                 sql = "SELECT fingerprint, keyid, expiration, creation, keytype, revoked FROM subkeys WHERE key_id=?"
                 cursor.execute(sql, (key_id,))
                 rows = cursor.fetchall()
```

### Comparing `johnnycanencrypt-0.8.0/johnnycanencrypt/utils.py` & `johnnycanencrypt-0.9.0/johnnycanencrypt/utils.py`

 * *Files 10% similar despite different names*

```diff
@@ -34,14 +34,46 @@
 	revoked INTEGER,
 	key_id INTEGER,
 	FOREIGN KEY (key_id)
 	REFERENCES keys (id)
 		ON DELETE CASCADE
 );
 
+CREATE TABLE uidcerts (
+	id INTEGER PRIMARY KEY,
+    ctype TEXT NOT NULL,
+	creation TEXT,
+	key_id INTEGER,
+	value_id INTEGER,
+	FOREIGN KEY (key_id)
+	REFERENCES keys (id)
+		ON DELETE CASCADE
+	FOREIGN KEY (value_id)
+	REFERENCES uidvalues (id)
+		ON DELETE CASCADE
+);
+
+CREATE TABLE uidcertlist (
+	id INTEGER PRIMARY KEY,
+	value TEXT,
+	datatype TEXT,
+	key_id INTEGER,
+	value_id INTEGER,
+	cert_id INTEGER,
+	FOREIGN KEY (key_id)
+	REFERENCES keys (id)
+		ON DELETE CASCADE
+	FOREIGN KEY (value_id)
+	REFERENCES uidvalues (id)
+		ON DELETE CASCADE
+	FOREIGN KEY (cert_id)
+	REFERENCES uidcerts (id)
+		ON DELETE CASCADE
+);
+
 CREATE TABLE uidemails (
 	id INTEGER PRIMARY KEY,
 	value TEXT,
 	key_id INTEGER,
 	value_id INTEGER,
 	FOREIGN KEY (key_id)
 	REFERENCES keys (id)
@@ -76,15 +108,15 @@
 	REFERENCES uidvalues (id)
 		ON DELETE CASCADE
 );
 
 CREATE TABLE dbupgrade (upgradedate TEXT)
 """
 
-DB_UPGRADE_DATE = "20220818"
+DB_UPGRADE_DATE = "20220828"
 
 
 def _get_cert_data(filepath):
     "Returns the filepath content as bytes"
     with open(filepath, "rb") as fobj:
         return fobj.read()
```

### Comparing `johnnycanencrypt-0.8.0/src/lib.rs` & `johnnycanencrypt-0.9.0/src/lib.rs`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,14 @@
+use openpgp::packet::Signature;
+use openpgp::KeyHandle;
 use pyo3::create_exception;
 use pyo3::exceptions::*;
 use pyo3::prelude::*;
 use pyo3::types::PyBytes;
+use pyo3::types::PyTuple;
 use pyo3::types::{PyDateTime, PyDict, PyList};
 use pyo3::wrap_pyfunction;
 
 use std::collections::HashMap;
 use std::fmt;
 use std::fs::File;
 use std::io;
@@ -946,29 +949,166 @@
     pin: Vec<u8>,
 ) -> Result<String> {
     let file = Path::new(str::from_utf8(&filepath[..])?);
     let mut localdata = File::open(file)?;
     sign_internal_detached_on_card(certdata, &mut localdata, pin)
 }
 
+#[pyfunction]
+#[pyo3(text_signature = "(certdata, othercertdata, sig_type, uids, password, oncard)")]
+fn certify_key(
+    py: Python,
+    certdata: Vec<u8>,
+    othercertdata: Vec<u8>,
+    sig_type: u8,
+    uids: Vec<String>,
+    password: Vec<u8>,
+    oncard: bool,
+) -> Result<PyObject> {
+    let policy = &P::new();
+
+    let cert = openpgp::Cert::from_bytes(&certdata)?;
+    let othercert = openpgp::Cert::from_bytes(&othercertdata)?;
+
+    let stype = match sig_type {
+        1 => SignatureType::PersonaCertification,
+        2 => SignatureType::CasualCertification,
+        3 => SignatureType::PositiveCertification,
+        _ => SignatureType::GenericCertification,
+    };
+
+    let mut cardkeys: Vec<scard::KeyPair> = Vec::new();
+    let mut keys = Vec::new();
+
+    // We will use this signer for signing.
+    let card_signer: Option<scard::KeyPair> = if oncard {
+        for ka in cert
+            .keys()
+            .with_policy(policy, None)
+            .alive()
+            .revoked(false)
+            .for_certification()
+        {
+            let key = ka.key();
+            let pair = scard::KeyPair::new(password.clone(), key)?;
+            cardkeys.push(pair);
+        }
+        if cardkeys.is_empty() {
+            return Err(JceError::new(format!(
+                "No key is available for certification in the public key."
+            )));
+        }
+        // Now we know for sure that there is a key
+        let key = cardkeys
+            .iter()
+            .next()
+            .expect("We must have a certification key by now");
+
+        Some(key.clone())
+    } else {
+        None
+    };
+
+    let disk_signer = if !oncard {
+        for key in cert
+            .keys()
+            .with_policy(policy, None)
+            .alive()
+            .revoked(false)
+            .for_certification()
+            .secret()
+            .map(|kd| kd.key())
+        {
+            let mut key = key.clone();
+            let algo = key.pk_algo();
+
+            key.secret_mut()
+                .decrypt_in_place(algo, &openpgp::crypto::Password::from(password.clone()))
+                .expect("decryption failed");
+            keys.push(key.into_keypair().unwrap());
+        }
+        if keys.is_empty() {
+            return Err(JceError::new(format!(
+                "No key is available for certification."
+            )));
+        }
+        // Now we know for sure that there is a key
+        let key = keys
+            .iter()
+            .next()
+            .expect("We must have a certification key by now");
+
+        Some(key.clone())
+    } else {
+        None
+    };
+
+    // To store the signatures till we insert them
+    let mut new_certificates: Vec<Signature> = Vec::new();
+    // Now let us find each of given user id values in the given key.
+    for uid in othercert.userids() {
+        if let Ok(userid_value) = std::str::from_utf8(uid.userid().value()) {
+            // Now loop over the given user id values as input
+            dbg!(userid_value.clone());
+            dbg!(uids.clone());
+            for userid in &uids {
+                if userid_value == userid {
+                    dbg!(format!(
+                        "We matched {} with {}",
+                        userid_value.clone(),
+                        userid.clone()
+                    ));
+                    let u = uid.userid();
+                    // Now certify
+                    let sig = match oncard {
+                        true => {
+                            let mut signer = card_signer.as_ref().unwrap().clone();
+                            u.certify(&mut signer, &othercert, stype.clone(), None, None)?
+                        }
+                        false => {
+                            let mut signer = disk_signer.as_ref().unwrap().clone();
+                            u.certify(&mut signer, &othercert, stype.clone(), None, None)?
+                        }
+                    };
+                    new_certificates.push(sig);
+                };
+            }
+        }
+    }
+
+    // Now let us to put the signatures back
+    let finalsig = othercert.insert_packets(new_certificates)?;
+    // Now let us return the secret key as Python Bytes
+    let mut buf = Vec::new();
+    let mut buffer = Vec::new();
+
+    let mut writer = Writer::new(&mut buf, Kind::PublicKey)?;
+    finalsig.as_tsk().serialize(&mut buffer)?;
+    writer.write_all(&buffer)?;
+    writer.finalize()?;
+
+    // Let us return the cert data which can be saved in the database
+    let res = PyBytes::new(py, &buf);
+    Ok(res.into())
+}
+
 // This is the internal function which signs either bytes or an input file on the smartcard
 fn sign_internal_detached_on_card(
     certdata: Vec<u8>,
     input: &mut dyn io::Read,
     pin: Vec<u8>,
 ) -> Result<String> {
     let policy = &P::new();
     // This is where we will store all the signing keys
     let mut keys: Vec<scard::KeyPair> = Vec::new();
     let cert = openpgp::Cert::from_bytes(&certdata)?;
     // Note: We are only selecting subkeys for signing via card
     for ka in cert
         .keys()
         .with_policy(policy, None)
-        .subkeys()
         .alive()
         .revoked(false)
         .for_signing()
     {
         let key = ka.key();
         let pair = scard::KeyPair::new(pin.clone(), key)?;
         keys.push(pair);
@@ -1033,15 +1173,14 @@
     let policy = &P::new();
     // This is where we will store all the signing keys
     let mut keys: Vec<scard::KeyPair> = Vec::new();
     // Note: We are only selecting subkeys for signing via card
     for ka in cert
         .keys()
         .with_policy(policy, None)
-        .subkeys()
         .alive()
         .revoked(false)
         .for_signing()
     {
         let key = ka.key();
         let pair = scard::KeyPair::new(pin.clone(), key)?;
         keys.push(pair);
@@ -1115,15 +1254,14 @@
     let policy = &P::new();
     // This is where we will store all the signing keys
     let mut keys: Vec<scard::KeyPair> = Vec::new();
     // Note: We are only selecting subkeys for signing via card
     for ka in cert
         .keys()
         .with_policy(policy, None)
-        .subkeys()
         .alive()
         .revoked(false)
         .for_signing()
     {
         let key = ka.key();
         let pair = scard::KeyPair::new(pin.clone(), key)?;
         keys.push(pair);
@@ -1331,18 +1469,23 @@
     sink.finalize().expect("Failed to write data");
 
     Ok(String::from_utf8(result)?)
 }
 
 #[pyfunction]
 #[pyo3(text_signature = "(certdata, newcertdata)")]
-fn merge_keys(_py: Python, certdata: Vec<u8>, newcertdata: Vec<u8>) -> Result<PyObject> {
+fn merge_keys(
+    _py: Python,
+    certdata: Vec<u8>,
+    newcertdata: Vec<u8>,
+    force: bool,
+) -> Result<PyObject> {
     let cert = openpgp::Cert::from_bytes(&certdata)?;
     let newcert = openpgp::Cert::from_bytes(&newcertdata)?;
-    if cert.as_tsk() == newcert.as_tsk() {
+    if cert.as_tsk() == newcert.as_tsk() && !force {
         return Err(JceError::new(
             "Both keys are same. Can not merge.".to_string(),
         ));
     }
     // Now let us merge the new one into old one.
     // Remember, the opposite is a security risk.
     let mergred_cert = cert.merge_public_and_secret(newcert)?;
@@ -1914,14 +2057,66 @@
         }
         let mut revoked = false;
         // Based on https://docs.sequoia-pgp.org/1.0.0/sequoia_openpgp/cert/struct.UserIDRevocationBuilder.html#examples
         if let RevocationStatus::Revoked(_) = ua.revocation_status(&p, None) {
             revoked = true;
         };
         pd.set_item("revoked", revoked)?;
+
+        // This list contains a list of dictionary
+        let certification_list = PyList::empty(py);
+        // Now we will deal with the certifications, that is if anyone else signed this UID.
+        for c in ua.certifications() {
+            // This is the type of certification
+            let c_type = match c.typ() {
+                SignatureType::GenericCertification => "generic",
+                SignatureType::CasualCertification => "casual",
+                SignatureType::PersonaCertification => "persona",
+                SignatureType::PositiveCertification => "postive",
+                _ => "unknown",
+            };
+
+            let creationtime = {
+                let sct = c.signature_creation_time();
+                match sct {
+                    Some(sct_value) => {
+                        let dt: DateTime<Utc> = DateTime::from(sct_value);
+                        Some(PyDateTime::from_timestamp(py, dt.timestamp() as f64, None)?)
+                    }
+                    None => None,
+                }
+            };
+
+            // Now we need a list of issuers for this certification
+            //
+            let issuer_list = PyList::empty(py);
+            for issuer in c.get_issuers() {
+                //let fp_keyid = PyTuple::new(py, &[issuer.])
+                match issuer {
+                    KeyHandle::Fingerprint(finger) => issuer_list.append(PyTuple::new(
+                        py,
+                        &["fingerprint".to_string(), finger.to_hex()],
+                    ))?,
+                    KeyHandle::KeyID(kid) => issuer_list
+                        .append(PyTuple::new(py, &["keyid".to_string(), kid.to_hex()]))?,
+                }
+            }
+
+            // Now add this one certification
+            let ud_dict = PyDict::new(py);
+            ud_dict.set_item("certification_type", c_type)?;
+            ud_dict.set_item("certification_list", issuer_list)?;
+            ud_dict.set_item("creationtime", creationtime)?;
+
+            certification_list.append(ud_dict)?;
+        }
+
+        // Now let us set the certifications for this user id
+        pd.set_item("certifications", certification_list)?;
+
         plist.append(pd)?;
     }
 
     let subkeys = PyList::empty(py);
     for ka in cert.keys().with_policy(&p, None).subkeys() {
         let expirationtime = match ka.key_expiration_time() {
             Some(etime) => {
@@ -2017,15 +2212,17 @@
 
     for uid in userids {
         crtbuilder = crtbuilder.add_userid(uid);
     }
 
     // To mark if our primary key needs to have signing capability
     let crtbuilder = match can_primary_sign {
-        true => crtbuilder.set_primary_key_flags(KeyFlags::empty().set_signing()),
+        true => {
+            crtbuilder.set_primary_key_flags(KeyFlags::empty().set_signing().set_certification())
+        }
         false => crtbuilder,
     };
 
     let crtbuilder = match creation {
         0 => crtbuilder,
         _ => {
             cdt = Some(DateTime::<Utc>::from_utc(
@@ -2103,14 +2300,15 @@
                 };
                 crtbuilder
             }
         }
     };
 
     let (cert, _) = crtbuilder.generate()?;
+
     let mut buf = Vec::new();
     let mut buffer = Vec::new();
 
     let mut writer = Writer::new(&mut buf, Kind::SecretKey)?;
     cert.as_tsk().serialize(&mut buffer)?;
     writer.write_all(&buffer)?;
     writer.finalize()?;
@@ -2697,12 +2895,13 @@
     m.add_wrapped(wrap_pyfunction!(encrypt_bytes_to_file))?;
     m.add_wrapped(wrap_pyfunction!(encrypt_bytes_to_bytes))?;
     m.add_wrapped(wrap_pyfunction!(encrypt_file_internal))?;
     m.add_wrapped(wrap_pyfunction!(update_password))?;
     m.add_wrapped(wrap_pyfunction!(add_uid_in_cert))?;
     m.add_wrapped(wrap_pyfunction!(revoke_uid_in_cert))?;
     m.add_wrapped(wrap_pyfunction!(update_subkeys_expiry_in_cert))?;
+    m.add_wrapped(wrap_pyfunction!(certify_key))?;
     m.add("CryptoError", _py.get_type::<CryptoError>())?;
     m.add("SameKeyError", _py.get_type::<SameKeyError>())?;
     m.add_class::<Johnny>()?;
     Ok(())
 }
```

### Comparing `johnnycanencrypt-0.8.0/src/scard.rs` & `johnnycanencrypt-0.9.0/src/scard.rs`

 * *Files 0% similar despite different names*

```diff
@@ -253,14 +253,15 @@
         resp = talktosc::send_and_parse(&card, apdu).unwrap();
         aiddata.extend(resp.get_data());
     }
     talktosc::disconnect(card);
     Ok(aiddata)
 }
 
+#[derive(Clone)]
 pub struct KeyPair<'a> {
     public: &'a Key<key::PublicParts, key::UnspecifiedRole>,
     pin: Vec<u8>,
 }
 
 impl<'a> KeyPair<'a> {
     /// Returns a `KeyPair` for `key` with the secret bits managed by
```

### Comparing `johnnycanencrypt-0.8.0/tests/files/double_recipient.asc` & `johnnycanencrypt-0.9.0/tests/files/double_recipient.asc`

 * *Files identical despite different names*

### Comparing `johnnycanencrypt-0.8.0/tests/files/hellopublic.asc` & `johnnycanencrypt-0.9.0/tests/files/hellopublic.asc`

 * *Files identical despite different names*

### Comparing `johnnycanencrypt-0.8.0/tests/files/hellosecret.asc` & `johnnycanencrypt-0.9.0/tests/files/hellosecret.asc`

 * *Files identical despite different names*

### Comparing `johnnycanencrypt-0.8.0/tests/files/public.asc` & `johnnycanencrypt-0.9.0/tests/files/public.asc`

 * *Files identical despite different names*

### Comparing `johnnycanencrypt-0.8.0/tests/files/secret.asc` & `johnnycanencrypt-0.9.0/tests/files/secret.asc`

 * *Files identical despite different names*

### Comparing `johnnycanencrypt-0.8.0/tests/files/store/FC3CE1AD6229F4CC89571D1CB4741BF4DDA4BA62.pub` & `johnnycanencrypt-0.9.0/tests/files/store/FC3CE1AD6229F4CC89571D1CB4741BF4DDA4BA62.pub`

 * *Files identical despite different names*

### Comparing `johnnycanencrypt-0.8.0/tests/files/store/hellopublic.asc` & `johnnycanencrypt-0.9.0/tests/files/store/hellopublic.asc`

 * *Files identical despite different names*

### Comparing `johnnycanencrypt-0.8.0/tests/files/store/hellosecret.asc` & `johnnycanencrypt-0.9.0/tests/files/store/hellosecret.asc`

 * *Files identical despite different names*

### Comparing `johnnycanencrypt-0.8.0/tests/files/store/jce.db` & `johnnycanencrypt-0.9.0/tests/files/store/oldjce.db`

 * *Files 3% similar despite different names*

#### sqlite3 {} .dump

```diff
@@ -4,21 +4,19 @@
 	id INTEGER PRIMARY KEY,
 	keyvalue BLOB NOT NULL,
 	fingerprint TEXT NOT NULL,
 	keyid TEXT NOT NULL,
 	expiration TEXT,
 	creation TEXT,
 	keytype INTEGER,
-	can_primary_sign INTEGER,
-    oncard TEXT,
-    primary_on_card TEXT
-);
-INSERT INTO keys VALUES(1,X'2d2d2d2d2d424547494e205047502050524956415445204b455920424c4f434b2d2d2d2d2d0a0a78595945583432675178594a4b7759424241486152773842415164412f646b442b5337304453696e733853774c44747a6373366c594838674e444565774672610a2f4d2f36556d542b43514d4934354548476a76727263332f4f3258664158707054524a4f395155735952525165794a552f3038776c376b5254484e4a4b47314e0a66744a744b683335486d5864626946366e794368666434775979655972586f597278612f705a533058614b626342685355464a78574d4b4442423857436741310a42594a666a6142444177734a42776b51785374434633685833586b4446516f4941707342416834424669454539504f49753747556b6c726a41666845785374430a4633685833586b41414661394151442f4c7652354f76644972725179676d6b5138446a7a4878763045686634376530483230673576536a555a5145417a46554d0a5665342f567671545752504e6d4532695664747165436541373347654e576772694b443371777a4e476e526c6333516764584e6c636941386447567a6445426e0a625746706243356a6232302b776f59454578594b41446746676c2b4e6f454d4443776b48435244464b3049586546666465514d56436767436d5145436d7745430a486745574951543038346937735a535357754d422b4554464b304958654666646551414174394942414e5258324c5875476468793530644b2f447566736d56360a334d39562b644965595a614f33444c537a54634a415039493169656b4e736d6e794353576753326758696a50363236372b366a774775466f5744654a5067524d0a4273654742462b4e6f454d574353734741515142326b635041514548514c43565a6d556b2b6e41786377614a687039436363386669793647353735585a4e727a0a6a4b625975632b452f676b4443506f536e5150516e536a482f316d66783177617537426d69792f2f754e4a51774e707736444a4a4a4a6a45456e4a54736370690a2f5774503248752b41634e4f5a4255424e5a72634844575842434244544e31312f46364747535869516e76626d43765537334c4b6a6d5843774449454742594b0a414b5146676c2b4e6f454d4a454d557251686434563931354170734341683442647141454752594b41436346676c2b4e6f454d4a454e2f5278566b6d5a4930760a4669454545433639493731644c5451507539344b3339484657535a6b6a53384141436938415030526e47326e51675a7547516f38756347617554784f746861740a4432632b4176645030644f746b6153313867442f6164614b6a54494657485863644a44377173542f7a42522b63656c784c33344c7a4241614a655033364163570a4951543038346937735a535357754d422b4554464b3049586546666465514141732b6f424150334a6c45356a6c6d65364e74486d5a5a2b4636436e416b744a4b0a6c384c6c335a6f2b534730736f6e4d6e4151444e69477149594f697637596930734544677451306e69682f7571735472476c704c3146764b6a7136644173654c0a42462b4e6f454d5343697347415151426c315542425145424230412f3468656f4b2b4d596f49624d577a4273726e434b356938432f6a6f68383767704235482f0a4a52745345514d4243416e2b43514d49364e6c39474f396e382f332f4a2f756454484561486f44364a534456485441684b514e617355596a754e5a57454146550a567149374e3147455573716e62636d355545716a4a7154436a675239396564696f4947754b7731535258615342307972582b53467450716c44384a37424267570a4367417442594a666a614244435244464b3049586546666465514b6243414965415259684250547a694c75786c4a4a6134774834524d557251686434563931350a414141644451443843526e535639755175314c676e3165356539657850763435506777524c574b574269437a7644616943337742414f456a47386c61302b45430a4e63463442344570685667495a79563452644b4e33446a3367776578535649430a3d666275430a2d2d2d2d2d454e44205047502050524956415445204b455920424c4f434b2d2d2d2d2d0a','F4F388BBB194925AE301F844C52B42177857DD79','C52B42177857DD79','','1603117123.0',1,0,NULL,'');
-INSERT INTO keys VALUES(2,X'2d2d2d2d2d424547494e205047502050524956415445204b455920424c4f434b2d2d2d2d2d0a0a7863614742462b4e6f4c5942454144453056514f4b74763776635338497841616c384c594c4457343639485963585a564c3336534d552b4c2f545854356248450a5261414a3278495454657a356a5942727458342b7a2b34395a655a45435a314f5957354c314853686843414756784d4b50397774356a48483851415a483243690a65492f5967777a503631367735694571353254494b614b584859494b5a316c57493537425339622f457737696e437a62683452416b554b4169636b575056722b0a45446d573164713938505a4551783741654656706d354569774a5144414e716d6b456336794d376562444e5762504161324f3652516c67774c317a74374d32740a5a6c2b7066552b58466b6e62776d5559343534754a5656506a78517074466a6c6e353967446a3661505a2f48654477495864353052775a4f32413344586261430a487653766d434c63346a364d3856352f37787451423776542b6b74472b36536f48376a2b744e5847374774336159757030586e6938306a4b656e7a7250686b320a366479436568664e5a74744d7572765753664c435775574649317458377178487136344744786e494e33387a687970575a6e7550766869773550486b777756620a726e6a69447a2b522f6435704b6b5575574450484f6b4b734932794d4747704531442f737078646f48416c414f6a31495762324a5749414b396534523450382f0a67544f3556746c482b59384a2f526e577068696457716f32387739645654565a526a78674835676d4d71656e3636776d564845614e5578496761616f544556540a377634635976506d5a62733670326164715267456e52375151326841636a4241476b42365168776e62306b31544e6f447078523839642f6762755661417950580a57794a524f6f384e7273312f4838695a2b706f6c2f584137594a33466e64525679752f4f636f696f38443650684e7048506b506b5271475579774152415141420a2f676b44434b447864455a6e7a7862522f34707477685a69653242523335586d705238797853763870544f424446636f6b7477676d48316b362b483857464b6c0a4f3155325779434e5749627634566777792f3771644d462b4b793145544e364b426d68366f73685a6c693647737048795a3667357372436749565477393379710a386c5a697463457941673674554b765a3554505259394b70753352314f6e6645305a68584b387867745168714f76644848327433704a326a454e6d4c4f5a6b410a5948454245326d7039427a77463867556b433953526a4f6632794e7a734e452f4b6a6951476a37344f4f356579702f4e72643769796f352f304143595871324d0a774f315446655957684332386d31745a43494e2b6d76316b4930657a624f69763453446c32657638307267444c6a564278387a52676d646f4837666152484a540a744e646261777949783475723771716e77546a735a502f30454b676b39542b577373617a5942373935626c64564d7a4f57744b764d464b58305a346f4e3556530a794979376f736c7461594f78442f44647465314a6e3031474a32646f70616e544d6e754d2b50676d572f3243506b35497265717941486657484238733855684a0a5456654d627759414b36707075547163504a79575249424b6e6971394e6956674d5233594743715a4d576654593968794e4465753136746d3647502f366a45310a632f3572762b53796f4a64582f6d6f4c31513569644c515370446368514f396b65396b30476f53432b78304f6f786b2b72374a736b38655046794a31595076440a4f447565376673356d346e4a56717747395246473034574f2f575874733737486f324c3476516e6a436a3636464c7253617853716e4a754652393859613543790a4d47676d6a4b744c5859473042766d426c7a556856395645646e6262445249716c4734506f7a45546570775744744d55456262717a34673576696a4a6c3867390a36442f69524e4a6348665368392f703543527a31617a4e79544c4563725630333363344e4a6c654c3361497936672f437862424b447543566b6d6e626e77426e0a6a4b682b3173676e31316d505747333261565372744c75516c6b594c44756d5654634d75394a4d58562b514d715676376c79302b514973726b42662b6a68706d0a6544635579335562417370552b4648485a31736c6c555762592f4373675a62362b7478662b726538394944324464554e685a416c4d73595061796b486c7841710a695845545a626c4b475a416b49446541316771362b6a774974692b6444593470497a6f67335a44466a346d394c5a6d7a4c364a6f327852767142542b583163790a587349594b637064465a766b64707146424f54416967477247444f687156754165663065352f3466553671526a36415a522b45335330487849675875527a6f510a2b38393077364578515a3744687655454b546368424d544e734b596568774567657046524d307a6834486654373673456e396c434f32596a394c4262364758490a6d565458447037774d433158507338372f4b6b4f595a4f4f4847556a7875434941587a544e3033506e774954336277586a4d7676786178516474734533524d6f0a53766777654c4434614a4b37656750346a58567461306f50505a71643649467375434735416b576e324c4363663873682b7950546447777932366a636e5366360a4f6448415058317556454d7078345a574f7943375a31484f394c446d614154336f306442772f57514c4b5773626856514474677a732b6b61355131582f68444a0a38425a59527a3972506d4a3134483438304d72786d7156634875314e476c354f44772f3771347748557342354c4952365832495964714d664c67794339752f330a484776442b352f706f386161746433386e367843426c46546e41366f415532317959577633677974495343585a6b366873682f3839456d684d2b694c4f5054540a756a6d396c716b5a37735258414a7a65596938725042525459422f7661534a6e4d635753514a554241314a334d5844346b722f474e7435762f4c6358786c55450a53533279662f553959356f513549635a57583178686252612f2f4474546f5a3961636f374c33396f7533742b5434685578644e4463446e6d5a6d6a5638365a6f0a4263574a7a59394769455264413346437a3746627068655461336136713341513651524e3257307241796e6e77612f3055652b53764458727a515a396f33304a0a7a4c6c32426e52775954646e455647373770725a63643564674d506a3676596c556459524777454c4b6534725a355453727a675078396c37724659484a6457670a584373456f644b7645424d446b557957576c5748363758326b466d626e615136436f5a707170732b464d52414a384749322f517149786563462b3050354c44730a616763785053595747534468443931435778425732785879574b2b7463545a51326d4b372f4944326458756565776a313143797a394d4843775945454877454b0a41445546676c2b4e6f4c594443776b484352436878634e6b3631756149414d56436767436d77454348674557495154314844454f4174776264334868647469680a78634e6b3631756149414141314f6f51414b2b46713839726e52424246795244325850306736627659636358643635664f7750446e45707830584e46772f48630a692b5046642b6a65356f444d54657a47586f4b4b4d364259626e7135363274544654577751543259762b7a4d2f715370312f6c67616c46416175584c495841620a6548526951336a46537551675758764535464a2b6a354f4b30473448437770715a62734b4d4463753062722b306d456f52626970742f752f684457484d7158460a794a41754c366f4b7446546f6b754d763470517341744248355a36595756566c66526566742b37696a783454513672324e5a5254726249334364307579522b4a0a37352f6a3942364732372f5066527162676864362f586f4c3430666a456f383773466345325242346439386d563465776955367133725078346b7a7a483271660a6d4d365947724663534c626a483657787546717944313543356e6b345250796735766e52577756787969344b61576b694d6e655274356d7a504c69386a3150360a625362424f487a6f644c4e2b634d48447246795073715153583741427842464f5264434d3161504b504b596b333564756d454d6644736b61614b74504a524a760a4b61643073772b566b586b577670385061724f2b54396c754c6748704e54687a6f49435348754b464563734f4c4e6d7a645375484431374c3674627a332f2f740a5a694570686164555561472b3777463767327072374a444d686c3250426744464d4d68776249354452395a3856684b70373346596643325844666b39696855720a37787352794632644b6e7a4972356f45436656626d337678664e61416b307855586257743859706f776572494e7a7269326f6e45446652667635654b6365357a0a4a32677a6d424b47556e626b344d4a307979656c66386f636c546446316464636d344366327444714c7a7a7868705965443951764a7262595a4349797a5239550a5a584e304946567a5a584979494478795957356b623231415a586868625842735a53356a6232302b7773474542424d424367413442594a666a6143324177734a0a42776b516f6358445a4f74626d69414446516f4941706b424170734241683442466945453952777844674c6347336478345862596f6358445a4f74626d6941410a414e6c54442f396e4c702f4b576f7553784b4472366d75714938697759516b45502f4a64684e307769384e6a51543055364f5873387a342b616d645675722f4a0a4b3177416356506e742f62377145745a4d6a7466455331686d774248434a326d427667525a707472314e59346f4c4d683049737457432f612b77757736366e410a5a3343554970665669334f2b2f33436844543273444355634b5a6458714232344239675763485378746a3335483973694352593577323265636676444f6b52780a48552f7774743454585a5258305a4961426f2f54346257397876516d5257694f6661576e47326b5a30383139666476326c36314d67776851644f5445756c4c460a6b6f636678724d5732745a6c727a796e6b69497a623975387773415577714c303876396b466162574e6462504e71713444376b45436251666e65575850377a4d0a4668784769546e743978306c78336d666a706f6a75486754534c4f3356316a6f31446e67646572742b573839702f4f6962546e5848414c774c6e7239386a554c0a504a796736506469796375706f5050456470575a395450303265713377522b343770444d5a3844425a6778362b385874494e774736784b326b6e6248796d36470a55687431714b73694e724b2f4b79664163447469555637654a55356532512b4364507067707632694243354a58354d4e3841624844552b64644b386a4c5a656d0a715a4e747532525669554679526842556e37484c624f32667558564c73753544453274556b427a5a464155546b6b5272716d597079334a66687142536c4e302f0a47673548695378564549334f6b3463526a486d73714a5737553878337a71453144384246734a4e4d414675376250386a366c5252795858666333324f486b4a550a6f7176555a50623132374a6d71733237472f56364f36513565576d7a4d754f695861457a4944474f43423571624a4d6958636647686752666a614332415241410a716f422f714d446836652b6249412b4f7754616c6a4f515757647a4f594a684178656559564e6168524b57646e61476e7858766851637979692f4973793659760a335933674b4362496443343639376361654530476e4137497145654d54546a746869645a4537415a4e424c664a5157572f75765972692b557141576773704a4d0a655175447a667a79666e2b3746596e6d426f67727469546d4c744967486f692f6f59486a34314a50436368726e6876524369744d6132684954304c57675947790a4b6368565448414736464b78596d6a4b497662586653467753494b63497070694a2b365a546a6b6249564b6d67536c386a654942796e614c53394b746c6f42370a352f594a77707756415a4234646d76456c7557474e3939516a456c47355a2b374244563431623238326e524f51462b54517553614f586c48643771664f4162300a7458755a453170347a2f3766364771485479453365624f6d69685463396563676f6a42657a576c2b616a5070585155523066517859366a6c5730795653495a770a6a4a746a6e2f734c6e4657314c52314a4e57364254716d58644237714b6a6665656a6276586a577447454a656f2b5967614d55575563797930646e777935446d0a3246652f55555a476c4d546c32677671724f384c7652304177704d536e4f6d467958447235393475472f316f3461464d355044594d4665674e6d2b483435306e0a647a682f316b384f4e747868624a682f58364f587a784e3451773073644f4c5a736649485265435837554b74427963456154575278597a3642673250575537780a74506a6c716459686e58456233496d2b61354571734c477458666251595469747465494d46362b3768764f4235597275317235546c68446467767a31617073380a7650464945336d51492b697272596378666f706764347170684c555a466a782b525a4e347867667758616341455145414166344a4177696d77355166305a58760a5966387449533551544b784b3331616f385356325153342f4c6774445631326c3549562f4d4b74634a77687143795158486b4752494d76656f4443507767794e0a2b45716277366746767867546b32644f3150385a487a614e6f6e762f69766e4d2b30444b69365377337a64354c516971574f4c6e4e4f50445a33494c323342440a456e68347a624465625839327636764f56356177667a4172756d786c6f736642537668597a4162594f5830505558565278546d714e375144634b5641306a546b0a44306d486a6141526374617048417a374f724f4b776e63514a467959554d454176514d2b4b734b4456536d7553357558514e72726e6f357739746d4e6f5967540a327a6e35546578475563793059586847704d343742484b70324d3373584139677a3377782b2b2f57784d4963794649307339484e7a793853456455555a6b46580a4a554465777073387654304f4b4369504f62434a3666476a4f33656f51305450655966526b73334b6946766536526f7563477a46744e76797a55665550612b630a375a62492f627a4f34636d4166354858547858526463494f416d435262376d7a68634f74506e314844587476587056364f4d6643667059644f7467595055376e0a756333457867493634313975556a3039437570496f2b316e354e744f7869475173586c4a6a777735797a79554244755363323571426538384f6f46794b6f6e300a697053535175767649584731436146514e7848576c5842624276566f78362f63332b555339425a4e463739323135535664544e6974516a4164312b30346538780a775972425955413831593957477875503972686a646d48564d4531332b7a42356758635230504559704b627443694f424d385242415a696c72522b49456f69590a51482b4756524763317a634c654868492f386a624d32377949694f4c6831763966346546736d757854716e654355315a50314c534967526275596330423366560a697652425344764550414843664c72596c356e3243734e4376757a49597074457a374534415a33544c5366417947792f76494174743376696f6d6e47547143330a573663457a4b6e652b6e65564e704b78753130384d73616e44336859325a7a6677546847394c6432634c326847687a6c446762474b3134612f6b454e4e546c470a4257447170574d66644647627255394147323849793371536a4b635452684b666359494d38466e79423277655a686d736b59305a554c7846692b69764d3853320a69772b68416633394a4462747962716741342b304a5a524a42786148633266386b67445853795736303955345374486e396c2b74564d736a44356f777a386b570a45326241464747646678706c45634b366a61304934497251414966312b304c6e4e475a7971734b69576a376546433267365972697871674f78323477576632390a4b7457547858506739677853656271564930726d322f4c544a62375853314c6552305950465658747458726a734f456756437071472b3555416f4e77485067480a2f6e7754716e5162535a4d304a5664327365496d33335547794747755257586436544b59497835544f35667754355654624d6161366554596c58316a777750530a734f75627143454764735648724e7869495271553862576e4634623056655461655a2b7a4d304f70316351486d61776e675553764a51502f4f534c77446764390a796b3144696768646d5748775764514e77442f494734374b3976524f356d386f6b59317067704853423846484a6173576866657154756d7a69564c64502b58640a6c6f482b496c4242317641467444453153317634543952674948533476524173464e66447252366779464a513979316d515a524f32426f6a58744b7a387658420a4f484a56464952685857587a767835337252786a37525574434736626f64544b53322f3663626f78596678444e5653654a355177416f777163757a4a572f4a6e0a3467316b562b7a6c4d46694b57624b6543323838454475354349704f417a443238762b3144585a784a7278484b2f4c2f33786d65566264595471304d746e666f0a58305a366276476e487832343349762b6235356d31366e30504665774852326170327271685a642b674433533743642b39664f715730507956554839625268790a354d5968464156716553377773425a526948323730374d3574795566593247444859716c372f3068514c65565a374c4176493271557871383542573053766d450a494172683457396e74444b324443487031684d556942474a6d74453574355666486a303654336f554438534b59312b2b395662506a332f2b4c7272704b4c5a4b0a516a797a6b703865396465574536744443576b4c675a7557324f67303159627043546e3136555465696c6151764a5670316c6974376b7854714b4445746b69380a41614647487270646478565164336d4d48737752536d705a42317464797443365966434f7032737877734635424267424367417442594a666a614332435243680a78634e6b3631756149414b624341496541525968425055634d5134433342743363654632324b48467732547257356f67414144722b772f384467442b7265334a0a4448763268685944353971685a306870444f313369744b586b4241587774767273572b456571424a767564684f697a564e6e794947336266767349424355486a0a306a515a563241384c4939435a5556615953784842526c314876702f70726441624534543839447961515a6a2b4d796b755a412f302b753451714972554d62570a4d6559557061366a66754a44347273767245646336556b6372686c536a61356578466b39386f4d4747772b7a5276636f49746e6c6e4c494c6d77347a52316f6e0a566e565a4e557563616165617146687442465a746c4176687742364c62545579737530707a5167766c445949546b46462f6e4e494958364b763850743970656d0a42726a4677656862675463524461713058732b43655a706964787668334c37796c33767a667274374e6f714d58314167416b786d6174486254305558737441350a717672585058425a4a5a4c30666c48576978342f58347176506d593535335866446c466b6b704547706548515137766e48655147766a2f79616631754a347a4e0a5271684131307a732f6d4755364e753859737744674e77376556704d53687a7758736538646d523147424f72592b5a723073566649467564514f452b32592b700a4b2b342b6c4336634276684533776d33386162547865754d6a36334d69426562454f486b703137484c6c3166592b344a41326c324a4131627755746e41556c6e0a4770363469564e4143442f33454e57495034594664484761556b6d2f692f46307a6d2b68716c6f4a317334614953726958346a51624c4d3677564d43303033700a56774e556d47735a534c35793159644132524676795342736c7637474f67385a504a384556463636317745757634744a4a79572b426d554c4f787a6b395a2b6a0a354663734f676b6d7356314764474f554f505046487a422f78454673392b7868784c5048786f59455834326774674551414e424a336b6d316472396a34702f2f0a59317939704e69686a424757315569704671322f324a78584936624772364f6638502f676d487870307750494f686334535455646c776b6a686d36397268344a0a4d4c484e517974776266374f6259714f6a6a3339316874666c343346644c4f39504d67495650524231376d4e6378717a67713067706255684e68796e6558384b0a696e647163734278486777537044643679416f342f437a42594435537461336f39376a673143776f506f4754765176414638576173454b654c687453747a556d0a2f4f79666a656157645a446670566139465a7a707471476370706c31664152657a4c764d505542343259554b35707949317437786c725773717979756f3076670a4949653744766c2f5448654f63716b71576978456f714333593732797233684a2f694d637552742b496c356347656e47717a49463071415552325346797538790a3668354265762b4f657158557639664a69354c3930686730356f3432575a346a54556f32482b4a3278556657645348775862742f786a6d534c6a5a7a2f436e790a38685741505635497545447747766e4f3872795547762b7177357a706e44393649664f332f374a487130453037704a466b7575697333502f5a474253357147360a53446544362b33417a514f425949733270475855715a653034654b365a436d7450496635316478452b723348637859307559544a32574e7842357058634f74460a336f39312f465839446a3269535a574d52702b766c4b7752506d4b396254445431744a465a38536b306e6133456b79504e342f4779444d375838566c4d4439430a5761485357346174744265586d676b6d4534637772522b6951656679304b597834443566463765534f6f3273414f4b797343674c6f3079677935304c754f694a0a6f78322b725271364b71745a412f644a7a47327a556d47576c504d74414245424141482b43514d497833476a754172554834502f335a783559497369454452470a635871786775344b53476565575a54483352736c765a3034545577766771485a4979337937376e4665584f4568794f2b59347539356664435653427131685a6f0a77745979767368735659796d7476507578485478716c6d68774373516b61467170614b465667492b35726c31306b636961507473413367534f653665715654330a4d7366314346714538753637443631685859667270714744754f584e564f615a72734e2b77476e59424f4e614a586336625139553733736639314571433330350a58566e4d45313148574b54773056384c7a46494f463646454a547130374b644939766e3344496f4f636f436d636f71704e33457a4c4962514b62326c704f70530a392b6c4841326a62727838564575767669577a6d7a586c3133706a516a674c7477425032713937443046486b71432b746a4a6c787a4f4b546c737969464b33640a2f45774c51477758303159544343526f6444316d6e437074694557386f58765677456b794952364b4771385a557071633479654774395541794f4776755276410a3937317a4842594d4c56567a67564371764f4357714e492b364a43742b74594b4c56457758735a64515278313254777949555a422b7854564354396757795a5a0a34705174783231716a7761306b69765a333071587237514c57484d336477675331566f4f546f6c7452504e497552686a6a69507468476e7865624831373259470a626d666f375541755561305a73364b36496a556e50745945355666784d576d747666457158667441416d334c6f324a41527479476b4a7a453046776a323636610a72387157375751384b3044314474546434526e58505247525444654c717931494a387a7444724c59434471674c4648506d312f686d784e44334d6173624a65520a71793548594454395544394b506e5a372f67533371494a2f794269724f367946356b6b6250776936326c69696d614942353072782b6c4f6a41784636635542660a642f38334b482b636369334a6f686c2b6862422b54734a49787532526430796a622b75354335437568495737482f79656d67414374466c4143684550727632470a38636a754e7934746a677a357952677a342f674f7169365978457849576b366467766e4a59735a326c644d7a686d64365848476e334e49566b6e3949422b76680a6344575353376e4977736f3443662b4b47424a776959432b494a48416c555556412f2f3863677630756d554a553578722f6c68706a48766a4b74454e426f4c560a4669563970425555576e2f61496166562b502b4a4b72355371726a4f386c494735444943705239394a663938654b79657443726a6b61556d6a634879375039390a3855454155535662472b572f4f674f793856562f623250336d764b5062332b645a5a6e2f654f71466f645a43494f2b71697a4a566b6a364f78593930736d43660a524c6f6a73636e37542f504253374a7561794c4d7578416466596f555351417731544e6e316b4139497a315567374d334e33635a4a442b796a6b7441394562550a6d3778643764763754675057647358716b684339375745475353395a2b6a5741676f466f33596735756542483073614c615756564d6a7954735a35616f3756300a475633685776357051374a6f7234734f745553496e4c705046374a694f466e37397232426d6d4b3851684251726c42694b706e5274713649314f5061425649390a5051586b6a304e703873794266784c4e55507264335973317043494e7452676b59684c41564a73666147303652753549584c73736b70332b36396f52724e726f0a473165764152416f506d646539517238597576434b714b423776576936634d6344516a586b774c792b75615975786642514d645a4130746f4b634e4f315a67370a3272764c38774b3846426168375a4c38384f6643707a55556e49693666747659676c4931367262434e735461323678516c6b455531596d6649364432494234570a426f4330684559526959555432503375453058502b49557a4f454270526b71426d6865536d695141724c6477766e79394a766e4837386c6d786d645461674c490a6b394155632f4c2b7647517254346658364f557972427a7a65396e6f4e3945787962416573366b32783444384a504d4d564b707632776b4278567755435068660a755a6d324d7a774b384f79433464506335576a6a5a784a72676a4f4973497446454f7a624b6f5333362b505844684357555a314f69425471475a5a4e747a6b420a5375506139465337354566395563667678704c524258593154486e3433616551475a315a553254706b67356d657a462f6e356649684f33542b784871414673590a303171336c2b54697279487141735349516c7236366e6852397a5a6a5066776156674f4942616168344355694e6761545030544346376e557459744c707577330a68674b33477865556141546b616b447750564c5534373279784d4c447277515941516f43597757435834326774676b516f6358445a4f74626d6941436d7749430a48674842644b41454751454b41436346676c2b4e6f4c594a454133465a31677175514773466945455555506c6e70674973566f6e464473754463566e574371350a4161774141425864442f30597a73654d2f6753724f34466477633035616f5a3568464d5949746b666a5643725a6a6c4e5a48757867742b53507930716474654b0a7331477663757a6f2f4462467643743238535768322f722b6e5678324a4c70532f585251706543565a536a44446247314f42634171446f496b625642507851580a424d467543505946344b564b32764453694652674a704b39444f43786563334c6436516e786a5477495577736f427a425649494a6c6f497742545249373667390a57746a6875437758754d342b694d356e34547951727a77427247446b663241416776594f757a4e6d4966726f744a58543550332b37566e50446674794f4b5a500a5872513772526c4d55416737384d3943706a445330616d595750716c556b4e7166713877696c6554466c3957346e51746c4346375a6839494a786e554f43354a0a712b684949536c61374364695a4e316e397864496a625a425337685a44594f73756443613479643337384b796b53363239696c513252442f74714f516f495a340a614a6d527573377857763975766c76427a6d5534534e653238624365337a385570644352316a4268445a4c3061454d39454d7a465a75586e6d2f6c59376a79410a4a6d797244417861685a657567394c7952654a6e3734324b6171364e635a476349364a6934396c6e426a5a434f6832514764525a636442706b744c3339315a730a676161734c676b3476665231412f506e4d6c33344d68316c78444362377830764f7a61414149426837656963715a4f6967636a78743549326c4a644269376d720a635a4d7a544d4361675164783770745772544736796d4b537454355a397831454d2b564a594d552f37546278786330384152425a50526f6e32634c79542f34670a61716c6d34346f45723939496b5354525559386f527170494c496c6248357362774b454b5346676e774552722f6f7665544f457147785968425055634d5134430a3342743363654632324b48467732547257356f6741414241376841417736417232526452584f542f50636e627a6679646d5861676a6733474877725966664b380a517031596e6d43473948356b5a354a6d45626a5069564d752b776334537a6e3956794c4548432b797352517a453254696c63544f365157522b30686f526b2b640a6a6f4935544a444549384c57466a5a594730347a6568467869554d7a566d35526a4a364a584b5a496b626f41375a78694663555a314c3932754d4978532b4c6e0a4775704455644c2b67346536386959564e696e76445a684e6a75356a394262716c734c33564733343335536a39727435466250674164343665456156695a55790a4b35493551796264523457424e46326d6d4a5a6e7270554153683630494e36487372753352662b675342507531786b744d526f4648764947525637326254312f0a37434554344d303539326b78625a677637616b70477a3546477a52465a3335776e2b794b3463736d4e3931423832473761445368486b444751544a4e744842340a7271514d6f43557376426e464e694759515650327555467469394958386e346a6e586966425356436456306c686946776d434d69645a4a716837654e576842700a54386a4861736a72654356424b556f704d37716e31584a5977643153376b5673414e34384c5a692b53665876716e594446797a5649375141707449624d4261640a4a5748795953472f396a4d69493566745a415576483457734e6b346861785570726e632f4d36424833765a58506f4c4b706a387662557565533673356f4661780a765839666548377274584250524a4156786936557671494e4d63344278666b6e4776736c426844436c4d78613530502b677638665a71723856695038734744750a6771793378663954623941703665616e44463370675a664e782b78712b475732676343526a39686f413075736565686b565771366b31762f2b7a506b797a33690a6b7268736831343d0a3d364255590a2d2d2d2d2d454e44205047502050524956415445204b455920424c4f434b2d2d2d2d2d0a','F51C310E02DC1B7771E176D8A1C5C364EB5B9A20','A1C5C364EB5B9A20','','1603117238.0',1,0,NULL,'');
-INSERT INTO keys VALUES(3,X'2d2d2d2d2d424547494e20504750205055424c4943204b455920424c4f434b2d2d2d2d2d0a0a6d51494e42466e6d49494d424541444b636e41477469387959646e49396873372f31336a7331456c722f516b6b46415132547a513159383056564d454668684e0a6e697a7966387572783933707151336f2b2b77455841414c5a504a72764230546534436b6f58776233562f39386a79707749366b4841696d45323833754f656d0a4c4467516f6f42435158316b464b6b584b74765548416372634e76335769734379523632786c666d496e4a64735358736370766a454a4c464a5a5a637a504e330a62563076626665487267575a414d37756371463474724a725373524b787337723773357767774f36383846354e45514c7064743061544c4c2f304f4c305054320a47464a6861466831614649533268793652586f5548627856557969474d336850516236303731566c69476e426a7174696e31777337455866387163514445344a0a737869454f677544314f78586246794e6d39306f456d6263674749665844664a774e59385a2f4444394b746b747957744e594a31416630526c51374c672f36420a6c717a31626133316d744965557a6b6537414237644d58326a434f6263656d45725435486a6b56534336764e677947464f6556466e583162314f7570495a4c340a4454615a7131797775596e6c5873657972494d7754542b674d612b554f6c30462f7764775931524544556b4a31636d42582f75514839755354496a51725a56370a754445726e4f7941394c766568717a47366963746a313771726e5553304c4178506f6139475a786643363439366c4966645a68497336634b76592f4672714a390a6948543573306b7959554455574f472f523070733661425741766173445757675769494b3169354168706e415a4e46355167764871447a346d2b56452f6a59790a51586b446830426b75704a7277585835503079677a5642614b6a656a55625a4362374b6551366c7a4f77554e582b6c4c5a357a6c416b524773774152415141420a7443464c64584e6f595777675247467a4944787264584e6f595778415a6e4a6c5a57527662533577636d567a637a364a416c6345457745494145454347774d460a4351576a6d6f414643776b49427749474651674a43677343424259434177454348674543463441574951536f582f4e32645a795a536f6f52614e6a59495a794d0a512f624634515543576559686f41495a4151414b43524459495a794d512f62463464374745414357576f6e6d527658495a655050655273612f475a43567277780a554137335a466744783630674c306f32776179716859697743365475515061343234554c63694c5770465179346c62385977415a2b6d4d3979517a664d622f300a747642396377643675717a4e497a31514479483239754451724d386b4a6e454668757866496e592f574e6163513831364636616e4f6c545271316a4d65434b610a44375567747a596a5a2b3347546f32554a7168497059426d4c6d2b68324e63366d475a46567149706a7a7347522f64526a5a4b4e4639646c4d2f387a6d6448500a5a7244416b3953634747757a4f7752514468716d38345845737564504236374b6533584774303134595a62756b7146744a6e78614b2f33796763317a4a4c35510a614a4236786e79756c485542396775533556614454732b4234747334622b436a34506b674539497553307859434369545151642f314c58304b444853497477320a434c4c4b31714d476a584e65544557497153496d7a787a475273394a3537684157724c4e754a707665685564675879366c486d6751744e79744e455576536d440a3059466d6d2f74336a673755504f48634e4a614f4d765743547271796a55576438317670594b75315551514747366e6279792f364a6b58774641714c55536b510a545062636e3752546c4e6e363856672f304f4270776642564764484d6542425335544475394a6a6471776442746e70624446357a4336614d5777346b435946540a3532412b473869627079453266792f532b5a4359314a65574a77755746634f49686a7178482b634742657278552b69544c4d6e5a2f32473176356973776265770a6169567a4847614e6c4f5345552b2b59572f554255337858644d354d496e442f4d6f39576d6566723130694a6b624e2f644c713245394a30427a416a7650676d0a5757554439496f6b383532744777456c677251655333567a614746734945526863794138625746706245427264584e6f5957786b59584d756157342b69514a550a42424d424341412b4669454571462f7a646e57636d55714b45576a59324347636a45503278654546416c6e6d49554d4347774d464351576a6d6f414643776b490a427749474651674a436773434242594341774543486745434634414143676b51324347636a455032786548763542414170432f44646c3076457a4b664b3952770a793253494c4d534e326d4e3133375a756877306d674635512b42383556583258504947394f4751517143344156597635682b444b556c485332696448705838550a38344c5373476864304a66416863623758635538694a685045477a624c7579675633427267364556663065525042324d496c39346278767361417a36443454610a76494d2f4f3553716b7379675139644e6f6f472b79312b786b507378485a4c516c6c5131505a394a477531747666316c67677236765a41535974764e565430350a436d6667376b7a714f2b392b4f6e4b3641496d6355722b746e7837694743435976456d696369356563356f72785158344d3044714e2b75496b397632757544670a6858594a554a787537643670676632755432336b587439666442372b4c684e51737150453645556576472f516e693934397168374f4e434f6d716f72516f6f450a4f367253305a4859426b65532f796878546754472b644b357430362f2f7852596c34624a6f31574d30412b2b577235392f36353549734d65467833464e6638450a416d4d434d6b622f78424c66377345694443484a3531636e5a4156757332683969696f435a41664e59326852307539547634305066756575344139626f6a55700a7734467243513161356a4c4353304d763639346b54664733595730647555754c2b515761472f644d4957626f4c3331545175666346587676696d51472b5279420a73376436426166384270787a50464d706766356d33623930326149397748306b326434383038564170384b372b6c7353565a4a374773757673596258507948360a673579555a625368554654457859373469644547476374566e625963695952586947697745554f5445395742695932576476504d4f636643453347347848494a0a45444e516c464f5a7a7a53656c4c4353464f547553753750756c4b3049457431633268686243424559584d675047743163326868624752686330426e625746700a6243356a6232302b69514a5542424d424341412b4669454571462f7a646e57636d55714b45576a59324347636a45503278654546416c6e6d49566b4347774d460a4351576a6d6f414643776b49427749474651674a436773434242594341774543486745434634414143676b51324347636a4550327865455a71672f2f576e56450a55757643646c3164397331674d4355574c6a5645626f6a41645a5755614638724d6d33586d4136446a55394c4a4c4f57424c5273734e41327764506d707436690a43625a4f4b41683563436b457054376c42427967553244677342394e6a4c656543517474574b736d53656c546c644b3932414e706149496355523437344c32750a38563742373642596b774b3773417a38426f374e36344d4d6a384b4754386f4e6d6570697844412f61684e4c6d4d6339525654483832647945535675567261620a79387255365844474264662b494879597266754d696e7039725255316f4c6b2b444e592b7a4743584646377646455451336e335476414954557361654a694d4c0a6e6144795a4e74743269423674654d3173512f41573175747179396f49514c45434c4c4b785a495a5866304c6e495043336356424b3478456667516758647a540a6f76465155447448416f4d6e6b5065427978614c7770786c69565854737268302f49736751676244594b6b426b506c34776a35504971665250374b2b55712f590a792b72374a434a6b75777a4e556a6f4134446458614b682b7543595976776a46674335444258427570333758596a44676237384a4358774d632b527a2f454e450a4a7a326d6a6c676f432b3134644256614b38614b39444454486349725031655664333348654c34676d573267446f446d7652314d646a3443343853417a4153640a6c48454850415035324d755479766a774a446d58716a79567936634e486a6653587461775958575a724a50482b4e543359765277727767797a5a457a3477616b0a78516448384f7449416f5a313344744d5863767264745944635a556c6d6550566b6e564b794777326f784b4473764d6e33346a4e6d3452336e33506f71426f2b0a623972385835787567492f636e417a4c5a546c756d526c56566f56334b34446972615173503875304a557431633268686243424559584d6750477431633268680a6245426d5a575276636d4677636d39715a574e304c6d39795a7a364a416c514545774549414434574951536f582f4e32645a795a536f6f52614e6a59495a794d0a512f624634515543576559686b7749624177554a42614f616741554c435167484167595643416b4b437749454667494441514965415149586741414b435244590a495a794d512f62463452524d454143764b514c374e706e4a463950654867726d684a69566c4a576d46764c70624e486a753161622b50535a6d6551494f5437470a543849496d2b5355464e7a782b79795a64746a63427a746969335575684866374a47396a6b3553635038656f3059764b6733517647687a4d4f77707a347041490a445370675447697364505a2f537163774675337349716951314a566a54494e7a51704b37577253536456446c5154454f485a54416650735044644369686964740a7975722f6937554b41422b584b32716f346939346948702f3547656e3966494261724b62766b4c533168596c746371494a6643694c2b4453516b3073394643300a7941363751702b54626d685964582b70416d50576b776f512f71763269624b77543269584b7a432b6d58494c4a4b4b335a4e496267792b6a583072344f6950440a695356716d773356617a6d65594f31326979685046526652574c3433354b69464c792b4e523665554a4e6567346f64336452754156387a366b7a6b77396337660a782f6c354a326935466c2f5879474a77526d50576e544830666c78484d2f654332794c7050684c656e34754f496c76554e692b645235393473365174304b6d4e0a4b63555a3176744a432b592b626c4261626a3156597046306f51736342723148776b4a6543354c79325a3264776a73454e575568506b576a536b6b39777077530a366c646a357a7331635a2f3378686a2b385a705a74486d67305547796437736479616a36516949776b7a52736b4547724148357656582b52732f6c535173344f0a4c4a5943374f624e32785a6a7041343545724f5443363331716f7877417542424f4477394d5344353275315937446d6f6b2f534c44544171585a596874726c610a32446477644767786f3257326554304c633732384c4566584b6a6a46395a516457446e39545154716e3950397a586936586a31495350595662726b434451525a0a3569482f4152414173566b7a513545302f6f4b5945486c665945382b43424568656d31374466696c7957466971326979526c494f354b6e7853464f6845316a2b0a6631773077514f68704b2f6131655173626669584a415777736b6974656f685a58557652446d61474c39787a374e6f4458526d742b33646134594d78454a412b0a3270656358533245596952463768376965544d446c4a555971334c423977316d373042365457694b624b3677324c36672f417737574c553865797458387541590a72314b4b714a7a52777450785654706253537574374e55564f36684476695a7a70556c64623153586e6579685036324559424a42757a693956437174374c36650a476865417a43434b6c6b514b6e6566756d64726249726b46347253565933504d5136717454485179646e6e2b77646159452f4d43536a44424a635330542f664d0a7474456b3068714e4a504b7035546a637233574345482b5a3946753850744473666c346659577631767153505248563551706d68327a52464d7744456253504d0a6350687345356d4e705a4c74796d4230413362494b665a4177683178585470527a5254665445517745304469364c4270552b7a3831676c5666386e4d4870666b0a4b6635314e674e736e574b692b3774544331697a48303576536c4268706149754b6166394d62466b683141536e38306a7059466379457748656552416e6456650a5138784f5a6c7a786264774c4431796e6563517357684834387131434176506e2b596b373630496c554d6332376530613579664a3873516f794d7148544c43430a37575a6353746e5246597957622b7863596e655354643857486e79664e6c484343667867476b6c44674a7a44594a43342f625876615270572b6d57346534544d0a71677938686161755734696150736a7245506b367358687346466c37794f597272576479776e774e753065516e6a714f467673414551454141596b45636751590a415167414a685968424b686638335a316e4a6c4b6968466f324e67686e4978443973586842514a5a3569482f4168734342516b466f357141416b414a454e67680a6e497844397358687758516742426b42434141644669454543384531456c36792f356f50694f3463786c2f77423864585a753046416c6e6d4966384143676b510a786c2f77423864585a7532686c6841416d503745524d5771784c66426b61665143586636336957694a355037414f306e6e5152596a52534948317264747436500a727042413958783176756a357645683268754d76346e3730612b4d346c533452456c4443672f6e447a6c4872466b50422f36534f347a456148397946444b4c410a71714d7863386649476b62762f5230526f6b516d6271774b59414a646e536e6b7a64333350515650342b47423545553868667074316337643854473631632b480a7339317573734d414b4637454247622b38735a48394a797a46765a2f30364c4e484a6b3172546f75394d4b3277505a33676f7739567a633861754544734d51700a5455324953796c48614c417064493642726b74632f753636514c463247496f4275365044485675776f70647852345339544730727a344b78376149642b3935770a783057695a7a4e43635835524a615842596a32416931514b644a437a6c484c6e42367737413348554f5471422f79657646567a506f516f69794f54373637434e0a4b3875427934647131714c6f596336664e524e6f427930574f3457756f31726f7877534d5a3048764447477956452b64524973655754584245675236685430660a625658535771557479574665612b6e546f5a783868495a4635514d54357441373975436c56654e3443544b6a7a5032786f684b7150324772782f6279466d6f590a2b2b4c412b6e552f79397075424d5a4b4c4135456f52614c384d6a5742776570667577584d2b5a6836507767787963427a7a78637543767a544d516f42686a550a615a7a556e61413544384e6b4a6b4e63426e2f6467347467653735575776747a32316b2f36515a44686f41425948464a344b745442582f356557566c49642b6b0a4444484e5043737350364b4b6c5956737142597365556a4e70506644537836486a484e7536794a523255326f726c4a314170367a4e62713962434e2f43412f370a426c576d59334266756f2f43424b503673694e614c36547955576464493352776349326e6c4b643775757167647643575a3668426777507345773845655844760a696b41333371432f58775632384b3331383056674c337754656f4a754230786c6878585a38583866564a447964484968444c487832523377556f3068644a716b0a6d556449324354375576364a796f32524833474d563145506e584d317038726735424370516d492b6556645734594c737572535252474c7a2b59524e395879700a704e6d364f715a64766b4a7a5a546f477970354f5a4835737339556e6b4d584968485768332f737648375279397042485a765155536272774b63624b68766c480a485242744e4541456a49733631664e437867714469625a4d452b5748525171754f5a575357596d7563546a374c6c5a33446b5837574f36584565357649564f780a76466f5851614e31555a396f766d53443652766d6c34624b6c657635326133547761706769614c523276436577506a626634417a7741736b59316b35652b35580a43677645593378306a74796c38684a507741334630775676526d786d453262644e7834652f4473396c3435646f75756f32596a654739505144324241517549410a32306d6a4b78346d784d6f646b7479794934757a476c634b57795772504478716753487a323856305a4d41747754586e416a4a51644b6e396d687358782f4e610a36796a5863697045747339363343376c72682f51686a493845395243414350455146562b30302b4e4f327956326a355a7548695479687666564b764c6b30577a0a2f334d77502f6d6b73517a6e5054316632586175554c694f794679684f70346d3752525967696b4c497570337a5176522b6a494955746d4458366b752b772b6b0a377a67622b52596661567a6f48392f6a5935666b5a6235526d69454a39595037504452663732354e5367613541673045576559694a774551414a786e4d32522f0a6f6c54613447456148422f42356b594679654359684751526b306e73616d38356845434263696561434c4273715433357349624254393269446b5137763074750a4e783456575435617462382b755a74543535413949716d4d6b4c64456130795931707550586642515164365a65534f37586431366b776f4c2f68757a43356e690a456f41575164637237476b346d6a30752b337063477961473730516847386659356d506b7463786c38725a536641395566454853534330566f6c394c585069460a58513854786a3978553665316d5377515056574e36644e30733645564e57656a68364b704c53456f5845506e706872326f5158614a50454e4872707136446a740a6e6a4b614455416e32582f2f6d723030587553627335542b4247617a385a705738713037327355534f6d64623236346642766f2b4f562b4a554353434b30632f0a5235356452466d6d67556a2b576c435566666730454f355a784667704c66564d69614330522f7a3559623652753279774d682f34336f5477596b4348506a5a440a5a506a5362325a50766b6568782b794c7362434756332f503539555a757353327a7034375535374538736255624f3168345641493375725a3676786e7a6256730a4533515648306f763957774b4c6653736856546d534378557759584d4b6b5841334c474f5a496941426e424c6e592b775a4e4a6e493439763447754f566333770a3868635870566b3659702f527377474e477542786a2f4e7453755a2b4f4f2b524a45565643344e6644454f30726478624b79646c4c68772b424d4b756c65662b0a6c70556f314f61764c396738794d796f34503271433152356b50776a7344724b2f504a686d612b366269377969317438675a70373179757167623664383230700a5364714f32356d50584a65444c2b484e43473846426b5663786148655269736a564c4378414245424141474a416a774547414549414359574951536f582f4e320a645a795a536f6f52614e6a59495a794d512f624634515543576559694a7749624441554a42614f616741414b43524459495a794d512f624634556f42454143490a356e42537a6658537a542b6b4d6b667a45564a35354e5736774b7166442f48736f6f574d5237355631613074734a3349766f6f49344a6b7736554c6d585032780a4555477168536352644f2f6d594b61554b395668567a45717574446f6f416e6664517464675a47654a627841703875623931653744332b387a7131784a534d740a2f5a665a7050514266394a3152504d4776774e4b2b73315435446c4339475273766a556f3245457075486542416f717454556754357679734d587a2b457a6e670a35447033755137456d4e6c6c49537072634651334f432f30513378416f6579667841634168416f705379303236762f434946727243705a7258305777674f4e410a77636b4e342f32355156716770666b622b4673585368576b75367776774b414a5352633351796679617a3348544a6f77344d6f4951674675545a7a73435741730a524f6c41476164735466385a76475167556b754967544e3836747944567a776661335941356f496e4367766d77387349446145642b4b32316d666a63623570370a614c4a35517531705a36597244346c6344784f305a6d7a6a4a5370733757346e34566a45414f3271426b4b3679622f61584b7a6a7236716441786f6f5334454d0a776962775061554b357a73726a5a2b7347393578334c796b346f353970327268704c675832705072637769414a725361372f48674e53596c444b724f4e4258730a677248396a45462b5a512f637531687172794d6574425337757338436b6f6c67784f63526c5261314f4a36657068523452374852314245362b4c574f495541360a7565707479696b52713165556d6665762f6b736f2b536e4a6b4a6f744f765666735839624e37374e616f753955766d6b6865745343684761506d78384e2b58530a6641464e4c585a4e4c454e6665435865574a392b464e34594e6e39487a6a507a374a33704f2f794d4a4c6b434451525a35694a55415241417171545233312f630a546c754e5a4a64764d49486d527876374d32415a58616e35615276423150506a676d65696566766d4f46707268344a6631756d737131433756467369686463750a30644b6e48664d482b664478634754442f7251496436596f3962776b6f68566d4c345a4b76572b664c4a6852386838764757365a3353675873524b3654636f410a3748627374486e4d4e734d4b6851324a2f4242374e375a37736b39476666563046556e4463356170533051444d5779343868727178556f4b6c343548726663350a4132312b696f5a4b3873596745786b4b7064497079616f714e6b70447878324a4e6e304b7054654856366639614237426136686e39754f35773139376a5370360a757865366b315778706839336f564d335052366e555a31464263317345775a2f31526c5073336c47684c515562565873492f347168744c7970614e79773575530a71664378473452692f50464a5a6755455479456d5747664235764a634a48446770383137332f594c716361467841716d416f59573872444d2b756a717341424b0a5a565236785161676857744c53472b714b666f565a427872685631764b70556b32707678744979775359555a546c3362694b383539765a6a3459565a4e6455300a4d61724653765934745555687663696d697352493445754d2f7a4f42693944613031476c546e51313051364e5733795235624465533071415539414d4c6e6b410a6f49346e6d5554514a3050617a78447754502b55526c4b7672302f2f3773366a6a7657784e59736f497357354d6b59756850742b6346367061473051797643520a48686743694863774f6a5345366b4677787854364e534c4a71794778326f4d6a6c456e78395547455a42744a4d69475154334a6f3859334c2b464c597a5277460a5971566c5858486b75786146625a356a36613843582f3459454f37694c423266673263414551454141596b4350415159415167414a685968424b686638335a310a6e4a6c4b6968466f324e67686e4978443973586842514a5a35694a554168736742516b466f35714141416f4a454e67686e49784439735868506d4551414947770a50485157425033426c7872613747736f71314958545a3271676f762b465537744646333950734e505533357242786763356a49594e6c78635a717a394d6845590a6174365944334c535269752f664735585149326e304d6f6d414159482f494a4865386a4d53434458722b56383575336164552f47564b43464a7a6e314a766f420a51724e3242597573575a4f6f58714e2b79306d49677353524f33764644466c435564666b6f5963562b663846703073546a32454d6c452f6b67313779515470480a6c516d72755163417634763659497a6a4d52776753437776676571383879537672785766386361635a654e33506d6f45776a586c4135505145496834707747390a4568714653555653464c774b6c5352374a696f485262595a586f4d6452724473656f4373725849336f70782f6f324d7a562b306241384450614a53396a334e4a0a67744469642b4a342b3344356274587961646b6d716e3672397a63373545345441666b2f32707349576c736e697a455a67456a6f3947533031463466725945770a37596d74774a37556c744632715464612b78306d55723136723955613577382f66325134556d72706b74746f6c4d37622f79357467597067437a2f362f4172340a6876376254696f3336396b4e674549587a626c4e766662757363734c5855586b74596d5370667976736253314d454e746a61682f725a73664c546845696f507a0a7553625469756a766945326669456272682b42314471636d75555968794b57736146386c333470436770482f585a505378675832586a786a774656705478682b0a6347682b4a6158475231614f734e4949642b3046526843717342787248534b3742516149775a4647413253783262377636556a505551654746453739374c64690a617649584b6b654b48544171796142784d4a6c4d7869444575312b622b704d68784b394973504f6c0a3d65445a740a2d2d2d2d2d454e4420504750205055424c4943204b455920424c4f434b2d2d2d2d2d0a','A85FF376759C994A8A1168D8D8219C8C43F6C5E1','D8219C8C43F6C5E1','1602861827.0','1508253827.0',0,1,NULL,'');
+    oncard TEXT
+);
+INSERT INTO keys VALUES(1,X'2d2d2d2d2d424547494e205047502050524956415445204b455920424c4f434b2d2d2d2d2d0a0a78595945583432675178594a4b7759424241486152773842415164412f646b442b5337304453696e733853774c44747a6373366c594838674e444565774672610a2f4d2f36556d542b43514d4934354548476a76727263332f4f3258664158707054524a4f395155735952525165794a552f3038776c376b5254484e4a4b47314e0a66744a744b683335486d5864626946366e794368666434775979655972586f597278612f705a533058614b626342685355464a78574d4b4442423857436741310a42594a666a6142444177734a42776b51785374434633685833586b4446516f4941707342416834424669454539504f49753747556b6c726a41666845785374430a4633685833586b41414661394151442f4c7652354f76644972725179676d6b5138446a7a4878763045686634376530483230673576536a555a5145417a46554d0a5665342f567671545752504e6d4532695664747165436541373347654e576772694b443371777a4e476e526c6333516764584e6c636941386447567a6445426e0a625746706243356a6232302b776f59454578594b41446746676c2b4e6f454d4443776b48435244464b3049586546666465514d56436767436d5145436d7745430a486745574951543038346937735a535357754d422b4554464b304958654666646551414174394942414e5258324c5875476468793530644b2f447566736d56360a334d39562b644965595a614f33444c537a54634a415039493169656b4e736d6e794353576753326758696a50363236372b366a774775466f5744654a5067524d0a4273654742462b4e6f454d574353734741515142326b635041514548514c43565a6d556b2b6e41786377614a687039436363386669793647353735585a4e727a0a6a4b625975632b452f676b4443506f536e5150516e536a482f316d66783177617537426d69792f2f754e4a51774e707736444a4a4a4a6a45456e4a54736370690a2f5774503248752b41634e4f5a4255424e5a72634844575842434244544e31312f46364747535869516e76626d43765537334c4b6a6d5843774449454742594b0a414b5146676c2b4e6f454d4a454d557251686434563931354170734341683442647141454752594b41436346676c2b4e6f454d4a454e2f5278566b6d5a4930760a4669454545433639493731644c5451507539344b3339484657535a6b6a53384141436938415030526e47326e51675a7547516f38756347617554784f746861740a4432632b4176645030644f746b6153313867442f6164614b6a54494657485863644a44377173542f7a42522b63656c784c33344c7a4241614a655033364163570a4951543038346937735a535357754d422b4554464b3049586546666465514141732b6f424150334a6c45356a6c6d65364e74486d5a5a2b4636436e416b744a4b0a6c384c6c335a6f2b534730736f6e4d6e4151444e69477149594f697637596930734544677451306e69682f7571735472476c704c3146764b6a7136644173654c0a42462b4e6f454d5343697347415151426c315542425145424230412f3468656f4b2b4d596f49624d577a4273726e434b356938432f6a6f68383767704235482f0a4a52745345514d4243416e2b43514d49364e6c39474f396e382f332f4a2f756454484561486f44364a534456485441684b514e617355596a754e5a57454146550a567149374e3147455573716e62636d355545716a4a7154436a675239396564696f4947754b7731535258615342307972582b53467450716c44384a37424267570a4367417442594a666a614244435244464b3049586546666465514b6243414965415259684250547a694c75786c4a4a6134774834524d557251686434563931350a414141644451443843526e535639755175314c676e3165356539657850763435506777524c574b574269437a7644616943337742414f456a47386c61302b45430a4e63463442344570685667495a79563452644b4e33446a3367776578535649430a3d666275430a2d2d2d2d2d454e44205047502050524956415445204b455920424c4f434b2d2d2d2d2d0a','F4F388BBB194925AE301F844C52B42177857DD79','C52B42177857DD79','','1603117123.0',1,NULL);
+INSERT INTO keys VALUES(2,X'2d2d2d2d2d424547494e205047502050524956415445204b455920424c4f434b2d2d2d2d2d0a0a7863614742462b4e6f4c5942454144453056514f4b74763776635338497841616c384c594c4457343639485963585a564c3336534d552b4c2f545854356248450a5261414a3278495454657a356a5942727458342b7a2b34395a655a45435a314f5957354c314853686843414756784d4b50397774356a48483851415a483243690a65492f5967777a503631367735694571353254494b614b584859494b5a316c57493537425339622f457737696e437a62683452416b554b4169636b575056722b0a45446d573164713938505a4551783741654656706d354569774a5144414e716d6b456336794d376562444e5762504161324f3652516c67774c317a74374d32740a5a6c2b7066552b58466b6e62776d5559343534754a5656506a78517074466a6c6e353967446a3661505a2f48654477495864353052775a4f32413344586261430a487653766d434c63346a364d3856352f37787451423776542b6b74472b36536f48376a2b744e5847374774336159757030586e6938306a4b656e7a7250686b320a366479436568664e5a74744d7572765753664c435775574649317458377178487136344744786e494e33387a687970575a6e7550766869773550486b777756620a726e6a69447a2b522f6435704b6b5575574450484f6b4b734932794d4747704531442f737078646f48416c414f6a31495762324a5749414b396534523450382f0a67544f3556746c482b59384a2f526e577068696457716f32387739645654565a526a78674835676d4d71656e3636776d564845614e5578496761616f544556540a377634635976506d5a62733670326164715267456e52375151326841636a4241476b42365168776e62306b31544e6f447078523839642f6762755661417950580a57794a524f6f384e7273312f4838695a2b706f6c2f584137594a33466e64525679752f4f636f696f38443650684e7048506b506b5271475579774152415141420a2f676b44434b447864455a6e7a7862522f34707477685a69653242523335586d705238797853763870544f424446636f6b7477676d48316b362b483857464b6c0a4f3155325779434e5749627634566777792f3771644d462b4b793145544e364b426d68366f73685a6c693647737048795a3667357372436749565477393379710a386c5a697463457941673674554b765a3554505259394b70753352314f6e6645305a68584b387867745168714f76644848327433704a326a454e6d4c4f5a6b410a5948454245326d7039427a77463867556b433953526a4f6632794e7a734e452f4b6a6951476a37344f4f356579702f4e72643769796f352f304143595871324d0a774f315446655957684332386d31745a43494e2b6d76316b4930657a624f69763453446c32657638307267444c6a564278387a52676d646f4837666152484a540a744e646261777949783475723771716e77546a735a502f30454b676b39542b577373617a5942373935626c64564d7a4f57744b764d464b58305a346f4e3556530a794979376f736c7461594f78442f44647465314a6e3031474a32646f70616e544d6e754d2b50676d572f3243506b35497265717941486657484238733855684a0a5456654d627759414b36707075547163504a79575249424b6e6971394e6956674d5233594743715a4d576654593968794e4465753136746d3647502f366a45310a632f3572762b53796f4a64582f6d6f4c31513569644c515370446368514f396b65396b30476f53432b78304f6f786b2b72374a736b38655046794a31595076440a4f447565376673356d346e4a56717747395246473034574f2f575874733737486f324c3476516e6a436a3636464c7253617853716e4a754652393859613543790a4d47676d6a4b744c5859473042766d426c7a556856395645646e6262445249716c4734506f7a45546570775744744d55456262717a34673576696a4a6c3867390a36442f69524e4a6348665368392f703543527a31617a4e79544c4563725630333363344e4a6c654c3361497936672f437862424b447543566b6d6e626e77426e0a6a4b682b3173676e31316d505747333261565372744c75516c6b594c44756d5654634d75394a4d58562b514d715676376c79302b514973726b42662b6a68706d0a6544635579335562417370552b4648485a31736c6c555762592f4373675a62362b7478662b726538394944324464554e685a416c4d73595061796b486c7841710a695845545a626c4b475a416b49446541316771362b6a774974692b6444593470497a6f67335a44466a346d394c5a6d7a4c364a6f327852767142542b583163790a587349594b637064465a766b64707146424f54416967477247444f687156754165663065352f3466553671526a36415a522b45335330487849675875527a6f510a2b38393077364578515a3744687655454b546368424d544e734b596568774567657046524d307a6834486654373673456e396c434f32596a394c4262364758490a6d565458447037774d433158507338372f4b6b4f595a4f4f4847556a7875434941587a544e3033506e774954336277586a4d7676786178516474734533524d6f0a53766777654c4434614a4b37656750346a58567461306f50505a71643649467375434735416b576e324c4363663873682b7950546447777932366a636e5366360a4f6448415058317556454d7078345a574f7943375a31484f394c446d614154336f306442772f57514c4b5773626856514474677a732b6b61355131582f68444a0a38425a59527a3972506d4a3134483438304d72786d7156634875314e476c354f44772f3771347748557342354c4952365832495964714d664c67794339752f330a484776442b352f706f386161746433386e367843426c46546e41366f415532317959577633677974495343585a6b366873682f3839456d684d2b694c4f5054540a756a6d396c716b5a37735258414a7a65596938725042525459422f7661534a6e4d635753514a554241314a334d5844346b722f474e7435762f4c6358786c55450a53533279662f553959356f513549635a57583178686252612f2f4474546f5a3961636f374c33396f7533742b5434685578644e4463446e6d5a6d6a5638365a6f0a4263574a7a59394769455264413346437a3746627068655461336136713341513651524e3257307241796e6e77612f3055652b53764458727a515a396f33304a0a7a4c6c32426e52775954646e455647373770725a63643564674d506a3676596c556459524777454c4b6534725a355453727a675078396c37724659484a6457670a584373456f644b7645424d446b557957576c5748363758326b466d626e615136436f5a707170732b464d52414a384749322f517149786563462b3050354c44730a616763785053595747534468443931435778425732785879574b2b7463545a51326d4b372f4944326458756565776a313143797a394d4843775945454877454b0a41445546676c2b4e6f4c594443776b484352436878634e6b3631756149414d56436767436d77454348674557495154314844454f4174776264334868647469680a78634e6b3631756149414141314f6f51414b2b46713839726e52424246795244325850306736627659636358643635664f7750446e45707830584e46772f48630a692b5046642b6a65356f444d54657a47586f4b4b4d364259626e7135363274544654577751543259762b7a4d2f715370312f6c67616c46416175584c495841620a6548526951336a46537551675758764535464a2b6a354f4b30473448437770715a62734b4d4463753062722b306d456f52626970742f752f684457484d7158460a794a41754c366f4b7446546f6b754d763470517341744248355a36595756566c66526566742b37696a783454513672324e5a5254726249334364307579522b4a0a37352f6a3942364732372f5066527162676864362f586f4c3430666a456f383773466345325242346439386d563465776955367133725078346b7a7a483271660a6d4d365947724663534c626a483657787546717944313543356e6b345250796735766e52577756787969344b61576b694d6e655274356d7a504c69386a3150360a625362424f487a6f644c4e2b634d48447246795073715153583741427842464f5264434d3161504b504b596b333564756d454d6644736b61614b74504a524a760a4b61643073772b566b586b577670385061724f2b54396c754c6748704e54687a6f49435348754b464563734f4c4e6d7a645375484431374c3674627a332f2f740a5a694570686164555561472b3777463767327072374a444d686c3250426744464d4d68776249354452395a3856684b70373346596643325844666b39696855720a37787352794632644b6e7a4972356f45436656626d337678664e61416b307855586257743859706f776572494e7a7269326f6e45446652667635654b6365357a0a4a32677a6d424b47556e626b344d4a307979656c66386f636c546446316464636d344366327444714c7a7a7868705965443951764a7262595a4349797a5239550a5a584e304946567a5a584979494478795957356b623231415a586868625842735a53356a6232302b7773474542424d424367413442594a666a6143324177734a0a42776b516f6358445a4f74626d69414446516f4941706b424170734241683442466945453952777844674c6347336478345862596f6358445a4f74626d6941410a414e6c54442f396e4c702f4b576f7553784b4472366d75714938697759516b45502f4a64684e307769384e6a51543055364f5873387a342b616d645675722f4a0a4b3177416356506e742f62377145745a4d6a7466455331686d774248434a326d427667525a707472314e59346f4c4d683049737457432f612b77757736366e410a5a3343554970665669334f2b2f33436844543273444355634b5a6458714232344239675763485378746a3335483973694352593577323265636676444f6b52780a48552f7774743454585a5258305a4961426f2f54346257397876516d5257694f6661576e47326b5a30383139666476326c36314d67776851644f5445756c4c460a6b6f636678724d5732745a6c727a796e6b69497a623975387773415577714c303876396b466162574e6462504e71713444376b45436251666e65575850377a4d0a4668784769546e743978306c78336d666a706f6a75486754534c4f3356316a6f31446e67646572742b573839702f4f6962546e5848414c774c6e7239386a554c0a504a796736506469796375706f5050456470575a395450303265713377522b343770444d5a3844425a6778362b385874494e774736784b326b6e6248796d36470a55687431714b73694e724b2f4b79664163447469555637654a55356532512b4364507067707632694243354a58354d4e3841624844552b64644b386a4c5a656d0a715a4e747532525669554679526842556e37484c624f32667558564c73753544453274556b427a5a464155546b6b5272716d597079334a66687142536c4e302f0a47673548695378564549334f6b3463526a486d73714a5737553878337a71453144384246734a4e4d414675376250386a366c5252795858666333324f486b4a550a6f7176555a50623132374a6d71733237472f56364f36513565576d7a4d754f695861457a4944474f43423571624a4d6958636647686752666a614332415241410a716f422f714d446836652b6249412b4f7754616c6a4f515757647a4f594a684178656559564e6168524b57646e61476e7858766851637979692f4973793659760a335933674b4362496443343639376361654530476e4137497145654d54546a746869645a4537415a4e424c664a5157572f75765972692b557141576773704a4d0a655175447a667a79666e2b3746596e6d426f67727469546d4c744967486f692f6f59486a34314a50436368726e6876524369744d6132684954304c57675947790a4b6368565448414736464b78596d6a4b497662586653467753494b63497070694a2b365a546a6b6249564b6d67536c386a654942796e614c53394b746c6f42370a352f594a77707756415a4234646d76456c7557474e3939516a456c47355a2b374244563431623238326e524f51462b54517553614f586c48643771664f4162300a7458755a453170347a2f3766364771485479453365624f6d69685463396563676f6a42657a576c2b616a5070585155523066517859366a6c5730795653495a770a6a4a746a6e2f734c6e4657314c52314a4e57364254716d58644237714b6a6665656a6276586a577447454a656f2b5967614d55575563797930646e777935446d0a3246652f55555a476c4d546c32677671724f384c7652304177704d536e4f6d467958447235393475472f316f3461464d355044594d4665674e6d2b483435306e0a647a682f316b384f4e747868624a682f58364f587a784e3451773073644f4c5a736649485265435837554b74427963456154575278597a3642673250575537780a74506a6c716459686e58456233496d2b61354571734c477458666251595469747465494d46362b3768764f4235597275317235546c68446467767a31617073380a7650464945336d51492b697272596378666f706764347170684c555a466a782b525a4e347867667758616341455145414166344a4177696d77355166305a58760a5966387449533551544b784b3331616f385356325153342f4c6774445631326c3549562f4d4b74634a77687143795158486b4752494d76656f4443507767794e0a2b45716277366746767867546b32644f3150385a487a614e6f6e762f69766e4d2b30444b69365377337a64354c516971574f4c6e4e4f50445a33494c323342440a456e68347a624465625839327636764f56356177667a4172756d786c6f736642537668597a4162594f5830505558565278546d714e375144634b5641306a546b0a44306d486a6141526374617048417a374f724f4b776e63514a467959554d454176514d2b4b734b4456536d7553357558514e72726e6f357739746d4e6f5967540a327a6e35546578475563793059586847704d343742484b70324d3373584139677a3377782b2b2f57784d4963794649307339484e7a793853456455555a6b46580a4a554465777073387654304f4b4369504f62434a3666476a4f33656f51305450655966526b73334b6946766536526f7563477a46744e76797a55665550612b630a375a62492f627a4f34636d4166354858547858526463494f416d435262376d7a68634f74506e314844587476587056364f4d6643667059644f7467595055376e0a756333457867493634313975556a3039437570496f2b316e354e744f7869475173586c4a6a777735797a79554244755363323571426538384f6f46794b6f6e300a697053535175767649584731436146514e7848576c5842624276566f78362f63332b555339425a4e463739323135535664544e6974516a4164312b30346538780a775972425955413831593957477875503972686a646d48564d4531332b7a42356758635230504559704b627443694f424d385242415a696c72522b49456f69590a51482b4756524763317a634c654868492f386a624d32377949694f4c6831763966346546736d757854716e654355315a50314c534967526275596330423366560a697652425344764550414843664c72596c356e3243734e4376757a49597074457a374534415a33544c5366417947792f76494174743376696f6d6e47547143330a573663457a4b6e652b6e65564e704b78753130384d73616e44336859325a7a6677546847394c6432634c326847687a6c446762474b3134612f6b454e4e546c470a4257447170574d66644647627255394147323849793371536a4b635452684b666359494d38466e79423277655a686d736b59305a554c7846692b69764d3853320a69772b68416633394a4462747962716741342b304a5a524a42786148633266386b67445853795736303955345374486e396c2b74564d736a44356f777a386b570a45326241464747646678706c45634b366a61304934497251414966312b304c6e4e475a7971734b69576a376546433267365972697871674f78323477576632390a4b7457547858506739677853656271564930726d322f4c544a62375853314c6552305950465658747458726a734f456756437071472b3555416f4e77485067480a2f6e7754716e5162535a4d304a5664327365496d33335547794747755257586436544b59497835544f35667754355654624d6161366554596c58316a777750530a734f75627143454764735648724e7869495271553862576e4634623056655461655a2b7a4d304f70316351486d61776e675553764a51502f4f534c77446764390a796b3144696768646d5748775764514e77442f494734374b3976524f356d386f6b59317067704853423846484a6173576866657154756d7a69564c64502b58640a6c6f482b496c4242317641467444453153317634543952674948533476524173464e66447252366779464a513979316d515a524f32426f6a58744b7a387658420a4f484a56464952685857587a767835337252786a37525574434736626f64544b53322f3663626f78596678444e5653654a355177416f777163757a4a572f4a6e0a3467316b562b7a6c4d46694b57624b6543323838454475354349704f417a443238762b3144585a784a7278484b2f4c2f33786d65566264595471304d746e666f0a58305a366276476e487832343349762b6235356d31366e30504665774852326170327271685a642b674433533743642b39664f715730507956554839625268790a354d5968464156716553377773425a526948323730374d3574795566593247444859716c372f3068514c65565a374c4176493271557871383542573053766d450a494172683457396e74444b324443487031684d556942474a6d74453574355666486a303654336f554438534b59312b2b395662506a332f2b4c7272704b4c5a4b0a516a797a6b703865396465574536744443576b4c675a7557324f67303159627043546e3136555465696c6151764a5670316c6974376b7854714b4445746b69380a41614647487270646478565164336d4d48737752536d705a42317464797443365966434f7032737877734635424267424367417442594a666a614332435243680a78634e6b3631756149414b624341496541525968425055634d5134433342743363654632324b48467732547257356f67414144722b772f384467442b7265334a0a4448763268685944353971685a306870444f313369744b586b4241587774767273572b456571424a767564684f697a564e6e794947336266767349424355486a0a306a515a563241384c4939435a5556615953784842526c314876702f70726441624534543839447961515a6a2b4d796b755a412f302b753451714972554d62570a4d6559557061366a66754a44347273767245646336556b6372686c536a61356578466b39386f4d4747772b7a5276636f49746e6c6e4c494c6d77347a52316f6e0a566e565a4e557563616165617146687442465a746c4176687742364c62545579737530707a5167766c445949546b46462f6e4e494958364b763850743970656d0a42726a4677656862675463524461713058732b43655a706964787668334c37796c33767a667274374e6f714d58314167416b786d6174486254305558737441350a717672585058425a4a5a4c30666c48576978342f58347176506d593535335866446c466b6b704547706548515137766e48655147766a2f79616631754a347a4e0a5271684131307a732f6d4755364e753859737744674e77376556704d53687a7758736538646d523147424f72592b5a723073566649467564514f452b32592b700a4b2b342b6c4336634276684533776d33386162547865754d6a36334d69426562454f486b703137484c6c3166592b344a41326c324a4131627755746e41556c6e0a4770363469564e4143442f33454e57495034594664484761556b6d2f692f46307a6d2b68716c6f4a317334614953726958346a51624c4d3677564d43303033700a56774e556d47735a534c35793159644132524676795342736c7637474f67385a504a384556463636317745757634744a4a79572b426d554c4f787a6b395a2b6a0a354663734f676b6d7356314764474f554f505046487a422f78454673392b7868784c5048786f59455834326774674551414e424a336b6d316472396a34702f2f0a59317939704e69686a424757315569704671322f324a78584936624772364f6638502f676d487870307750494f686334535455646c776b6a686d36397268344a0a4d4c484e517974776266374f6259714f6a6a3339316874666c343346644c4f39504d67495650524231376d4e6378717a67713067706255684e68796e6558384b0a696e647163734278486777537044643679416f342f437a42594435537461336f39376a673143776f506f4754765176414638576173454b654c687453747a556d0a2f4f79666a656157645a446670566139465a7a707471476370706c31664152657a4c764d505542343259554b35707949317437786c725773717979756f3076670a4949653744766c2f5448654f63716b71576978456f714333593732797233684a2f694d637552742b496c356347656e47717a49463071415552325346797538790a3668354265762b4f657158557639664a69354c3930686730356f3432575a346a54556f32482b4a3278556657645348775862742f786a6d534c6a5a7a2f436e790a38685741505635497545447747766e4f3872795547762b7177357a706e44393649664f332f374a487130453037704a466b7575697333502f5a474253357147360a53446544362b33417a514f425949733270475855715a653034654b365a436d7450496635316478452b723348637859307559544a32574e7842357058634f74460a336f39312f465839446a3269535a574d52702b766c4b7752506d4b396254445431744a465a38536b306e6133456b79504e342f4779444d375838566c4d4439430a5761485357346174744265586d676b6d4534637772522b6951656679304b597834443566463765534f6f3273414f4b797343674c6f3079677935304c754f694a0a6f78322b725271364b71745a412f644a7a47327a556d47576c504d74414245424141482b43514d497833476a754172554834502f335a783559497369454452470a635871786775344b53476565575a54483352736c765a3034545577766771485a4979337937376e4665584f4568794f2b59347539356664435653427131685a6f0a77745979767368735659796d7476507578485478716c6d68774373516b61467170614b465667492b35726c31306b636961507473413367534f653665715654330a4d7366314346714538753637443631685859667270714744754f584e564f615a72734e2b77476e59424f4e614a586336625139553733736639314571433330350a58566e4d45313148574b54773056384c7a46494f463646454a547130374b644939766e3344496f4f636f436d636f71704e33457a4c4962514b62326c704f70530a392b6c4841326a62727838564575767669577a6d7a586c3133706a516a674c7477425032713937443046486b71432b746a4a6c787a4f4b546c737969464b33640a2f45774c51477758303159544343526f6444316d6e437074694557386f58765677456b794952364b4771385a557071633479654774395541794f4776755276410a3937317a4842594d4c56567a67564371764f4357714e492b364a43742b74594b4c56457758735a64515278313254777949555a422b7854564354396757795a5a0a34705174783231716a7761306b69765a333071587237514c57484d336477675331566f4f546f6c7452504e497552686a6a69507468476e7865624831373259470a626d666f375541755561305a73364b36496a556e50745945355666784d576d747666457158667441416d334c6f324a41527479476b4a7a453046776a323636610a72387157375751384b3044314474546434526e58505247525444654c717931494a387a7444724c59434471674c4648506d312f686d784e44334d6173624a65520a71793548594454395544394b506e5a372f67533371494a2f794269724f367946356b6b6250776936326c69696d614942353072782b6c4f6a41784636635542660a642f38334b482b636369334a6f686c2b6862422b54734a49787532526430796a622b75354335437568495737482f79656d67414374466c4143684550727632470a38636a754e7934746a677a357952677a342f674f7169365978457849576b366467766e4a59735a326c644d7a686d64365848476e334e49566b6e3949422b76680a6344575353376e4977736f3443662b4b47424a776959432b494a48416c555556412f2f3863677630756d554a553578722f6c68706a48766a4b74454e426f4c560a4669563970425555576e2f61496166562b502b4a4b72355371726a4f386c494735444943705239394a663938654b79657443726a6b61556d6a634879375039390a3855454155535662472b572f4f674f793856562f623250336d764b5062332b645a5a6e2f654f71466f645a43494f2b71697a4a566b6a364f78593930736d43660a524c6f6a73636e37542f504253374a7561794c4d7578416466596f555351417731544e6e316b4139497a315567374d334e33635a4a442b796a6b7441394562550a6d3778643764763754675057647358716b684339375745475353395a2b6a5741676f466f33596735756542483073614c615756564d6a7954735a35616f3756300a475633685776357051374a6f7234734f745553496e4c705046374a694f466e37397232426d6d4b3851684251726c42694b706e5274713649314f5061425649390a5051586b6a304e703873794266784c4e55507264335973317043494e7452676b59684c41564a73666147303652753549584c73736b70332b36396f52724e726f0a473165764152416f506d646539517238597576434b714b423776576936634d6344516a586b774c792b75615975786642514d645a4130746f4b634e4f315a67370a3272764c38774b3846426168375a4c38384f6643707a55556e49693666747659676c4931367262434e735461323678516c6b455531596d6649364432494234570a426f4330684559526959555432503375453058502b49557a4f454270526b71426d6865536d695141724c6477766e79394a766e4837386c6d786d645461674c490a6b394155632f4c2b7647517254346658364f557972427a7a65396e6f4e3945787962416573366b32783444384a504d4d564b707632776b4278567755435068660a755a6d324d7a774b384f79433464506335576a6a5a784a72676a4f4973497446454f7a624b6f5333362b505844684357555a314f69425471475a5a4e747a6b420a5375506139465337354566395563667678704c524258593154486e3433616551475a315a553254706b67356d657a462f6e356649684f33542b784871414673590a303171336c2b54697279487141735349516c7236366e6852397a5a6a5066776156674f4942616168344355694e6761545030544346376e557459744c707577330a68674b33477865556141546b616b447750564c5534373279784d4c447277515941516f43597757435834326774676b516f6358445a4f74626d6941436d7749430a48674842644b41454751454b41436346676c2b4e6f4c594a454133465a31677175514773466945455555506c6e70674973566f6e464473754463566e574371350a4161774141425864442f30597a73654d2f6753724f34466477633035616f5a3568464d5949746b666a5643725a6a6c4e5a48757867742b53507930716474654b0a7331477663757a6f2f4462467643743238535768322f722b6e5678324a4c70532f585251706543565a536a44446247314f42634171446f496b625642507851580a424d467543505946344b564b32764453694652674a704b39444f43786563334c6436516e786a5477495577736f427a425649494a6c6f497742545249373667390a57746a6875437758754d342b694d356e34547951727a77427247446b663241416776594f757a4e6d4966726f744a58543550332b37566e50446674794f4b5a500a5872513772526c4d55416737384d3943706a445330616d595750716c556b4e7166713877696c6554466c3957346e51746c4346375a6839494a786e554f43354a0a712b684949536c61374364695a4e316e397864496a625a425337685a44594f73756443613479643337384b796b53363239696c513252442f74714f516f495a340a614a6d527573377857763975766c76427a6d5534534e653238624365337a385570644352316a4268445a4c3061454d39454d7a465a75586e6d2f6c59376a79410a4a6d797244417861685a657567394c7952654a6e3734324b6171364e635a476349364a6934396c6e426a5a434f6832514764525a636442706b744c3339315a730a676161734c676b3476665231412f506e4d6c33344d68316c78444362377830764f7a61414149426837656963715a4f6967636a78743549326c4a644269376d720a635a4d7a544d4361675164783770745772544736796d4b537454355a397831454d2b564a594d552f37546278786330384152425a50526f6e32634c79542f34670a61716c6d34346f45723939496b5354525559386f527170494c496c6248357362774b454b5346676e774552722f6f7665544f457147785968425055634d5134430a3342743363654632324b48467732547257356f6741414241376841417736417232526452584f542f50636e627a6679646d5861676a6733474877725966664b380a517031596e6d43473948356b5a354a6d45626a5069564d752b776334537a6e3956794c4548432b797352517a453254696c63544f365157522b30686f526b2b640a6a6f4935544a444549384c57466a5a594730347a6568467869554d7a566d35526a4a364a584b5a496b626f41375a78694663555a314c3932754d4978532b4c6e0a4775704455644c2b67346536386959564e696e76445a684e6a75356a394262716c734c33564733343335536a39727435466250674164343665456156695a55790a4b35493551796264523457424e46326d6d4a5a6e7270554153683630494e36487372753352662b675342507531786b744d526f4648764947525637326254312f0a37434554344d303539326b78625a677637616b70477a3546477a52465a3335776e2b794b3463736d4e3931423832473761445368486b444751544a4e744842340a7271514d6f43557376426e464e694759515650327555467469394958386e346a6e586966425356436456306c686946776d434d69645a4a716837654e576842700a54386a4861736a72654356424b556f704d37716e31584a5977643153376b5673414e34384c5a692b53665876716e594446797a5649375141707449624d4261640a4a5748795953472f396a4d69493566745a415576483457734e6b346861785570726e632f4d36424833765a58506f4c4b706a387662557565533673356f4661780a765839666548377274584250524a4156786936557671494e4d63344278666b6e4776736c426844436c4d78613530502b677638665a71723856695038734744750a6771793378663954623941703665616e44463370675a664e782b78712b475732676343526a39686f413075736565686b565771366b31762f2b7a506b797a33690a6b7268736831343d0a3d364255590a2d2d2d2d2d454e44205047502050524956415445204b455920424c4f434b2d2d2d2d2d0a','F51C310E02DC1B7771E176D8A1C5C364EB5B9A20','A1C5C364EB5B9A20','','1603117238.0',1,NULL);
+INSERT INTO keys VALUES(3,X'2d2d2d2d2d424547494e20504750205055424c4943204b455920424c4f434b2d2d2d2d2d0a0a6d51494e42466e6d49494d424541444b636e41477469387959646e49396873372f31336a7331456c722f516b6b46415132547a513159383056564d454668684e0a6e697a7966387572783933707151336f2b2b77455841414c5a504a72764230546534436b6f58776233562f39386a79707749366b4841696d45323833754f656d0a4c4467516f6f42435158316b464b6b584b74765548416372634e76335769734379523632786c666d496e4a64735358736370766a454a4c464a5a5a637a504e330a62563076626665487267575a414d37756371463474724a725373524b787337723773357767774f36383846354e45514c7064743061544c4c2f304f4c305054320a47464a6861466831614649533268793652586f5548627856557969474d336850516236303731566c69476e426a7174696e31777337455866387163514445344a0a737869454f677544314f78586246794e6d39306f456d6263674749665844664a774e59385a2f4444394b746b747957744e594a31416630526c51374c672f36420a6c717a31626133316d744965557a6b6537414237644d58326a434f6263656d45725435486a6b56534336764e677947464f6556466e583162314f7570495a4c340a4454615a7131797775596e6c5873657972494d7754542b674d612b554f6c30462f7764775931524544556b4a31636d42582f75514839755354496a51725a56370a754445726e4f7941394c766568717a47366963746a313771726e5553304c4178506f6139475a786643363439366c4966645a68497336634b76592f4672714a390a6948543573306b7959554455574f472f523070733661425741766173445757675769494b3169354168706e415a4e46355167764871447a346d2b56452f6a59790a51586b446830426b75704a7277585835503079677a5642614b6a656a55625a4362374b6551366c7a4f77554e582b6c4c5a357a6c416b524773774152415141420a7443464c64584e6f595777675247467a4944787264584e6f595778415a6e4a6c5a57527662533577636d567a637a364a416c6345457745494145454347774d460a4351576a6d6f414643776b49427749474651674a43677343424259434177454348674543463441574951536f582f4e32645a795a536f6f52614e6a59495a794d0a512f624634515543576559686f41495a4151414b43524459495a794d512f62463464374745414357576f6e6d527658495a655050655273612f475a43567277780a554137335a466744783630674c306f32776179716859697743365475515061343234554c63694c5770465179346c62385977415a2b6d4d3979517a664d622f300a747642396377643675717a4e497a31514479483239754451724d386b4a6e454668757866496e592f574e6163513831364636616e4f6c545271316a4d65434b610a44375567747a596a5a2b3347546f32554a7168497059426d4c6d2b68324e63366d475a46567149706a7a7347522f64526a5a4b4e4639646c4d2f387a6d6448500a5a7244416b3953634747757a4f7752514468716d38345845737564504236374b6533584774303134595a62756b7146744a6e78614b2f33796763317a4a4c35510a614a4236786e79756c485542396775533556614454732b4234747334622b436a34506b674539497553307859434369545151642f314c58304b444853497477320a434c4c4b31714d476a584e65544557497153496d7a787a475273394a3537684157724c4e754a707665685564675879366c486d6751744e79744e455576536d440a3059466d6d2f74336a673755504f48634e4a614f4d765743547271796a55576438317670594b75315551514747366e6279792f364a6b58774641714c55536b510a545062636e3752546c4e6e363856672f304f4270776642564764484d6542425335544475394a6a6471776442746e70624446357a4336614d5777346b435946540a3532412b473869627079453266792f532b5a4359314a65574a77755746634f49686a7178482b634742657278552b69544c4d6e5a2f32473176356973776265770a6169567a4847614e6c4f5345552b2b59572f554255337858644d354d496e442f4d6f39576d6566723130694a6b624e2f644c713245394a30427a416a7650676d0a5757554439496f6b383532744777456c677251655333567a614746734945526863794138625746706245427264584e6f5957786b59584d756157342b69514a550a42424d424341412b4669454571462f7a646e57636d55714b45576a59324347636a45503278654546416c6e6d49554d4347774d464351576a6d6f414643776b490a427749474651674a436773434242594341774543486745434634414143676b51324347636a455032786548763542414170432f44646c3076457a4b664b3952770a793253494c4d534e326d4e3133375a756877306d674635512b42383556583258504947394f4751517143344156597635682b444b556c485332696448705838550a38344c5373476864304a66416863623758635538694a685045477a624c7579675633427267364556663065525042324d496c39346278767361417a36443454610a76494d2f4f3553716b7379675139644e6f6f472b79312b786b507378485a4c516c6c5131505a394a477531747666316c67677236765a41535974764e565430350a436d6667376b7a714f2b392b4f6e4b3641496d6355722b746e7837694743435976456d696369356563356f72785158344d3044714e2b75496b397632757544670a6858594a554a787537643670676632755432336b587439666442372b4c684e51737150453645556576472f516e693934397168374f4e434f6d716f72516f6f450a4f367253305a4859426b65532f796878546754472b644b357430362f2f7852596c34624a6f31574d30412b2b577235392f36353549734d65467833464e6638450a416d4d434d6b622f78424c66377345694443484a3531636e5a4156757332683969696f435a41664e59326852307539547634305066756575344139626f6a55700a7734467243513161356a4c4353304d763639346b54664733595730647555754c2b515761472f644d4957626f4c3331545175666346587676696d51472b5279420a73376436426166384270787a50464d706766356d33623930326149397748306b326434383038564170384b372b6c7353565a4a374773757673596258507948360a673579555a625368554654457859373469644547476374566e625963695952586947697745554f5445395742695932576476504d4f636643453347347848494a0a45444e516c464f5a7a7a53656c4c4353464f547553753750756c4b3049457431633268686243424559584d675047743163326868624752686330426e625746700a6243356a6232302b69514a5542424d424341412b4669454571462f7a646e57636d55714b45576a59324347636a45503278654546416c6e6d49566b4347774d460a4351576a6d6f414643776b49427749474651674a436773434242594341774543486745434634414143676b51324347636a4550327865455a71672f2f576e56450a55757643646c3164397331674d4355574c6a5645626f6a41645a5755614638724d6d33586d4136446a55394c4a4c4f57424c5273734e41327764506d707436690a43625a4f4b41683563436b457054376c42427967553244677342394e6a4c656543517474574b736d53656c546c644b3932414e706149496355523437344c32750a38563742373642596b774b3773417a38426f374e36344d4d6a384b4754386f4e6d6570697844412f61684e4c6d4d6339525654483832647945535675567261620a79387255365844474264662b494879597266754d696e7039725255316f4c6b2b444e592b7a4743584646377646455451336e335476414954557361654a694d4c0a6e6144795a4e74743269423674654d3173512f41573175747179396f49514c45434c4c4b785a495a5866304c6e495043336356424b3478456667516758647a540a6f76465155447448416f4d6e6b5065427978614c7770786c69565854737268302f49736751676244594b6b426b506c34776a35504971665250374b2b55712f590a792b72374a434a6b75777a4e556a6f4134446458614b682b7543595976776a46674335444258427570333758596a44676237384a4358774d632b527a2f454e450a4a7a326d6a6c676f432b3134644256614b38614b39444454486349725031655664333348654c34676d573267446f446d7652314d646a3443343853417a4153640a6c48454850415035324d755479766a774a446d58716a79567936634e486a6653587461775958575a724a50482b4e543359765277727767797a5a457a3477616b0a78516448384f7449416f5a313344744d5863767264745944635a556c6d6550566b6e564b794777326f784b4473764d6e33346a4e6d3452336e33506f71426f2b0a623972385835787567492f636e417a4c5a546c756d526c56566f56334b34446972615173503875304a557431633268686243424559584d6750477431633268680a6245426d5a575276636d4677636d39715a574e304c6d39795a7a364a416c514545774549414434574951536f582f4e32645a795a536f6f52614e6a59495a794d0a512f624634515543576559686b7749624177554a42614f616741554c435167484167595643416b4b437749454667494441514965415149586741414b435244590a495a794d512f62463452524d454143764b514c374e706e4a463950654867726d684a69566c4a576d46764c70624e486a753161622b50535a6d6551494f5437470a543849496d2b5355464e7a782b79795a64746a63427a746969335575684866374a47396a6b3553635038656f3059764b6733517647687a4d4f77707a347041490a445370675447697364505a2f537163774675337349716951314a566a54494e7a51704b37577253536456446c5154454f485a54416650735044644369686964740a7975722f6937554b41422b584b32716f346939346948702f3547656e3966494261724b62766b4c533168596c746371494a6643694c2b4453516b3073394643300a7941363751702b54626d685964582b70416d50576b776f512f71763269624b77543269584b7a432b6d58494c4a4b4b335a4e496267792b6a583072344f6950440a695356716d773356617a6d65594f31326979685046526652574c3433354b69464c792b4e523665554a4e6567346f64336452754156387a366b7a6b77396337660a782f6c354a326935466c2f5879474a77526d50576e544830666c78484d2f654332794c7050684c656e34754f496c76554e692b645235393473365174304b6d4e0a4b63555a3176744a432b592b626c4261626a3156597046306f51736342723148776b4a6543354c79325a3264776a73454e575568506b576a536b6b39777077530a366c646a357a7331635a2f3378686a2b385a705a74486d67305547796437736479616a36516949776b7a52736b4547724148357656582b52732f6c535173344f0a4c4a5943374f624e32785a6a7041343545724f5443363331716f7877417542424f4477394d5344353275315937446d6f6b2f534c44544171585a596874726c610a32446477644767786f3257326554304c633732384c4566584b6a6a46395a516457446e39545154716e3950397a586936586a31495350595662726b434451525a0a3569482f4152414173566b7a513545302f6f4b5945486c665945382b43424568656d31374466696c7957466971326979526c494f354b6e7853464f6845316a2b0a6631773077514f68704b2f6131655173626669584a415777736b6974656f685a58557652446d61474c39787a374e6f4458526d742b33646134594d78454a412b0a3270656358533245596952463768376965544d446c4a555971334c423977316d373042365457694b624b3677324c36672f417737574c553865797458387541590a72314b4b714a7a52777450785654706253537574374e55564f36684476695a7a70556c64623153586e6579685036324559424a42757a693956437174374c36650a476865417a43434b6c6b514b6e6566756d64726249726b46347253565933504d5136717454485179646e6e2b77646159452f4d43536a44424a635330542f664d0a7474456b3068714e4a504b7035546a637233574345482b5a3946753850744473666c346659577631767153505248563551706d68327a52464d7744456253504d0a6350687345356d4e705a4c74796d4230413362494b665a4177683178585470527a5254665445517745304469364c4270552b7a3831676c5666386e4d4870666b0a4b6635314e674e736e574b692b3774544331697a48303576536c4268706149754b6166394d62466b683141536e38306a7059466379457748656552416e6456650a5138784f5a6c7a786264774c4431796e6563517357684834387131434176506e2b596b373630496c554d6332376530613579664a3873516f794d7148544c43430a37575a6353746e5246597957622b7863596e655354643857486e79664e6c484343667867476b6c44674a7a44594a43342f625876615270572b6d57346534544d0a71677938686161755734696150736a7245506b367358687346466c37794f597272576479776e774e753065516e6a714f467673414551454141596b45636751590a415167414a685968424b686638335a316e4a6c4b6968466f324e67686e4978443973586842514a5a3569482f4168734342516b466f357141416b414a454e67680a6e497844397358687758516742426b42434141644669454543384531456c36792f356f50694f3463786c2f77423864585a753046416c6e6d4966384143676b510a786c2f77423864585a7532686c6841416d503745524d5771784c66426b61665143586636336957694a355037414f306e6e5152596a52534948317264747436500a727042413958783176756a357645683268754d76346e3730612b4d346c533452456c4443672f6e447a6c4872466b50422f36534f347a456148397946444b4c410a71714d7863386649476b62762f5230526f6b516d6271774b59414a646e536e6b7a64333350515650342b47423545553868667074316337643854473631632b480a7339317573734d414b4637454247622b38735a48394a797a46765a2f30364c4e484a6b3172546f75394d4b3277505a33676f7739567a633861754544734d51700a5455324953796c48614c417064493642726b74632f753636514c463247496f4275365044485675776f70647852345339544730727a344b78376149642b3935770a783057695a7a4e43635835524a615842596a32416931514b644a437a6c484c6e42367737413348554f5471422f79657646567a506f516f69794f54373637434e0a4b3875427934647131714c6f596336664e524e6f427930574f3457756f31726f7877534d5a3048764447477956452b64524973655754584245675236685430660a625658535771557479574665612b6e546f5a783868495a4635514d54357441373975436c56654e3443544b6a7a5032786f684b7150324772782f6279466d6f590a2b2b4c412b6e552f79397075424d5a4b4c4135456f52614c384d6a5742776570667577584d2b5a6836507767787963427a7a78637543767a544d516f42686a550a615a7a556e61413544384e6b4a6b4e63426e2f6467347467653735575776747a32316b2f36515a44686f41425948464a344b745442582f356557566c49642b6b0a4444484e5043737350364b4b6c5956737142597365556a4e70506644537836486a484e7536794a523255326f726c4a314170367a4e62713962434e2f43412f370a426c576d59334266756f2f43424b503673694e614c36547955576464493352776349326e6c4b643775757167647643575a3668426777507345773845655844760a696b41333371432f58775632384b3331383056674c337754656f4a754230786c6878585a38583866564a447964484968444c487832523377556f3068644a716b0a6d556449324354375576364a796f32524833474d563145506e584d317038726735424370516d492b6556645734594c737572535252474c7a2b59524e395879700a704e6d364f715a64766b4a7a5a546f477970354f5a4835737339556e6b4d584968485768332f737648375279397042485a765155536272774b63624b68766c480a485242744e4541456a49733631664e437867714469625a4d452b5748525171754f5a575357596d7563546a374c6c5a33446b5837574f36584565357649564f780a76466f5851614e31555a396f766d53443652766d6c34624b6c657635326133547761706769614c523276436577506a626634417a7741736b59316b35652b35580a43677645593378306a74796c38684a507741334630775676526d786d453262644e7834652f4473396c3435646f75756f32596a654739505144324241517549410a32306d6a4b78346d784d6f646b7479794934757a476c634b57795772504478716753487a323856305a4d41747754586e416a4a51644b6e396d687358782f4e610a36796a5863697045747339363343376c72682f51686a493845395243414350455146562b30302b4e4f327956326a355a7548695479687666564b764c6b30577a0a2f334d77502f6d6b73517a6e5054316632586175554c694f794679684f70346d3752525967696b4c497570337a5176522b6a494955746d4458366b752b772b6b0a377a67622b52596661567a6f48392f6a5935666b5a6235526d69454a39595037504452663732354e5367613541673045576559694a774551414a786e4d32522f0a6f6c54613447456148422f42356b594679654359684751526b306e73616d38356845434263696561434c4273715433357349624254393269446b5137763074750a4e783456575435617462382b755a74543535413949716d4d6b4c64456130795931707550586642515164365a65534f37586431366b776f4c2f68757a43356e690a456f41575164637237476b346d6a30752b337063477961473730516847386659356d506b7463786c38725a536641395566454853534330566f6c394c585069460a58513854786a3978553665316d5377515056574e36644e30733645564e57656a68364b704c53456f5845506e706872326f5158614a50454e4872707136446a740a6e6a4b614455416e32582f2f6d723030587553627335542b4247617a385a705738713037327355534f6d64623236346642766f2b4f562b4a554353434b30632f0a5235356452466d6d67556a2b576c435566666730454f355a784667704c66564d69614330522f7a3559623652753279774d682f34336f5477596b4348506a5a440a5a506a5362325a50766b6568782b794c7362434756332f503539555a757353327a7034375535374538736255624f3168345641493375725a3676786e7a6256730a4533515648306f763957774b4c6653736856546d534378557759584d4b6b5841334c474f5a496941426e424c6e592b775a4e4a6e493439763447754f566333770a3868635870566b3659702f527377474e477542786a2f4e7453755a2b4f4f2b524a45565643344e6644454f30726478624b79646c4c68772b424d4b756c65662b0a6c70556f314f61764c396738794d796f34503271433152356b50776a7344724b2f504a686d612b366269377969317438675a70373179757167623664383230700a5364714f32356d50584a65444c2b484e43473846426b5663786148655269736a564c4378414245424141474a416a774547414549414359574951536f582f4e320a645a795a536f6f52614e6a59495a794d512f624634515543576559694a7749624441554a42614f616741414b43524459495a794d512f624634556f42454143490a356e42537a6658537a542b6b4d6b667a45564a35354e5736774b7166442f48736f6f574d5237355631613074734a3349766f6f49344a6b7736554c6d585032780a4555477168536352644f2f6d594b61554b395668567a45717574446f6f416e6664517464675a47654a627841703875623931653744332b387a7131784a534d740a2f5a665a7050514266394a3152504d4776774e4b2b73315435446c4339475273766a556f3245457075486542416f717454556754357679734d587a2b457a6e670a35447033755137456d4e6c6c49537072634651334f432f30513378416f6579667841634168416f705379303236762f434946727243705a7258305777674f4e410a77636b4e342f32355156716770666b622b4673585368576b75367776774b414a5352633351796679617a3348544a6f77344d6f4951674675545a7a73435741730a524f6c41476164735466385a76475167556b754967544e3836747944567a776661335941356f496e4367766d77387349446145642b4b32316d666a63623570370a614c4a35517531705a36597244346c6344784f305a6d7a6a4a5370733757346e34566a45414f3271426b4b3679622f61584b7a6a7236716441786f6f5334454d0a776962775061554b357a73726a5a2b7347393578334c796b346f353970327268704c675832705072637769414a725361372f48674e53596c444b724f4e4258730a677248396a45462b5a512f637531687172794d6574425337757338436b6f6c67784f63526c5261314f4a36657068523452374852314245362b4c574f495541360a7565707479696b52713165556d6665762f6b736f2b536e4a6b4a6f744f765666735839624e37374e616f753955766d6b6865745343684761506d78384e2b58530a6641464e4c585a4e4c454e6665435865574a392b464e34594e6e39487a6a507a374a33704f2f794d4a4c6b434451525a35694a55415241417171545233312f630a546c754e5a4a64764d49486d527876374d32415a58616e35615276423150506a676d65696566766d4f46707268344a6631756d737131433756467369686463750a30644b6e48664d482b664478634754442f7251496436596f3962776b6f68566d4c345a4b76572b664c4a6852386838764757365a3353675873524b3654636f410a3748627374486e4d4e734d4b6851324a2f4242374e375a37736b39476666563046556e4463356170533051444d5779343868727178556f4b6c343548726663350a4132312b696f5a4b3873596745786b4b7064497079616f714e6b70447878324a4e6e304b7054654856366639614237426136686e39754f35773139376a5370360a757865366b315778706839336f564d335052366e555a31464263317345775a2f31526c5073336c47684c515562565873492f347168744c7970614e79773575530a71664378473452692f50464a5a6755455479456d5747664235764a634a48446770383137332f594c716361467841716d416f59573872444d2b756a717341424b0a5a565236785161676857744c53472b714b666f565a427872685631764b70556b32707678744979775359555a546c3362694b383539765a6a3459565a4e6455300a4d61724653765934745555687663696d697352493445754d2f7a4f42693944613031476c546e51313051364e5733795235624465533071415539414d4c6e6b410a6f49346e6d5554514a3050617a78447754502b55526c4b7672302f2f3773366a6a7657784e59736f497357354d6b59756850742b6346367061473051797643520a48686743694863774f6a5345366b4677787854364e534c4a71794778326f4d6a6c456e78395547455a42744a4d69475154334a6f3859334c2b464c597a5277460a5971566c5858486b75786146625a356a36613843582f3459454f37694c423266673263414551454141596b4350415159415167414a685968424b686638335a310a6e4a6c4b6968466f324e67686e4978443973586842514a5a35694a554168736742516b466f35714141416f4a454e67686e49784439735868506d4551414947770a50485157425033426c7872613747736f71314958545a3271676f762b465537744646333950734e505533357242786763356a49594e6c78635a717a394d6845590a6174365944334c535269752f664735585149326e304d6f6d414159482f494a4865386a4d53434458722b56383575336164552f47564b43464a7a6e314a766f420a51724e3242597573575a4f6f58714e2b79306d49677353524f33764644466c435564666b6f5963562b663846703073546a32454d6c452f6b67313779515470480a6c516d72755163417634763659497a6a4d52776753437776676571383879537672785766386361635a654e33506d6f45776a586c4135505145496834707747390a4568714653555653464c774b6c5352374a696f485262595a586f4d6452724473656f4373725849336f70782f6f324d7a562b306241384450614a53396a334e4a0a67744469642b4a342b3344356274587961646b6d716e3672397a63373545345441666b2f32707349576c736e697a455a67456a6f3947533031463466725945770a37596d74774a37556c744632715464612b78306d55723136723955613577382f66325134556d72706b74746f6c4d37622f79357467597067437a2f362f4172340a6876376254696f3336396b4e674549587a626c4e766662757363734c5855586b74596d5370667976736253314d454e746a61682f725a73664c546845696f507a0a7553625469756a766945326669456272682b42314471636d75555968794b57736146386c333470436770482f585a505378675832586a786a774656705478682b0a6347682b4a6158475231614f734e4949642b3046526843717342787248534b3742516149775a4647413253783262377636556a505551654746453739374c64690a617649584b6b654b48544171796142784d4a6c4d7869444575312b622b704d68784b394973504f6c0a3d65445a740a2d2d2d2d2d454e4420504750205055424c4943204b455920424c4f434b2d2d2d2d2d0a','A85FF376759C994A8A1168D8D8219C8C43F6C5E1','D8219C8C43F6C5E1','1602861827.0','1508253827.0',0,NULL);
 CREATE TABLE subkeys (
 	id INTEGER PRIMARY KEY,
 	key_id INTEGER,
 	fingerprint TEXT NOT NULL,
 	keyid TEXT NOT NULL,
 	expiration TEXT,
 	creation TEXT,
@@ -34,26 +32,25 @@
 INSERT INTO subkeys VALUES(4,2,'5143E59E9808B15A27143B2E0DC567582AB901AC','0DC567582AB901AC','','1603117238.0','signing',0);
 INSERT INTO subkeys VALUES(5,3,'D2BAF6212E4CDE548C330C3DFB82AA5D326DA75D','FB82AA5D326DA75D','1602862247.0','1508254247.0','encryption',0);
 INSERT INTO subkeys VALUES(6,3,'621B1339CDB831479A4DEB4F7C90F2749E085E1D','7C90F2749E085E1D','1602862292.0','1508254292.0','authentication',0);
 INSERT INTO subkeys VALUES(7,3,'0BC135125EB2FF9A0F88EE1CC65FF007C75766ED','C65FF007C75766ED','1602862207.0','1508254207.0','signing',0);
 CREATE TABLE uidvalues (
 	id INTEGER PRIMARY KEY,
 	value TEXT,
-	revoked INTEGER,
 	key_id INTEGER,
 	FOREIGN KEY (key_id)
 	REFERENCES keys (id)
 		ON DELETE CASCADE
 );
-INSERT INTO uidvalues VALUES(1,'test user <test@gmail.com>',0,1);
-INSERT INTO uidvalues VALUES(2,'Test User2 <random@example.com>',0,2);
-INSERT INTO uidvalues VALUES(3,'Kushal Das <kushal@fedoraproject.org>',0,3);
-INSERT INTO uidvalues VALUES(4,'Kushal Das <kushal@freedom.press>',0,3);
-INSERT INTO uidvalues VALUES(5,'Kushal Das <kushaldas@gmail.com>',0,3);
-INSERT INTO uidvalues VALUES(6,'Kushal Das <mail@kushaldas.in>',0,3);
+INSERT INTO uidvalues VALUES(1,'test user <test@gmail.com>',1);
+INSERT INTO uidvalues VALUES(2,'Test User2 <random@example.com>',2);
+INSERT INTO uidvalues VALUES(3,'Kushal Das <kushal@fedoraproject.org>',3);
+INSERT INTO uidvalues VALUES(4,'Kushal Das <kushal@freedom.press>',3);
+INSERT INTO uidvalues VALUES(5,'Kushal Das <kushaldas@gmail.com>',3);
+INSERT INTO uidvalues VALUES(6,'Kushal Das <mail@kushaldas.in>',3);
 CREATE TABLE uidemails (
 	id INTEGER PRIMARY KEY,
 	value TEXT,
 	key_id INTEGER,
 	value_id INTEGER,
 	FOREIGN KEY (key_id)
 	REFERENCES keys (id)
@@ -94,10 +91,8 @@
 	FOREIGN KEY (key_id)
 	REFERENCES keys (id)
 		ON DELETE CASCADE
 	FOREIGN KEY (value_id)
 	REFERENCES uidvalues (id)
 		ON DELETE CASCADE
 );
-CREATE TABLE dbupgrade (upgradedate TEXT);
-INSERT INTO dbupgrade VALUES('20220818');
 COMMIT;
```

### Comparing `johnnycanencrypt-0.8.0/tests/files/store/kushal_updated_key.asc` & `johnnycanencrypt-0.9.0/tests/files/store/kushal_updated_key.asc`

 * *Files identical despite different names*

### Comparing `johnnycanencrypt-0.8.0/tests/files/store/oldjce.db` & `johnnycanencrypt-0.9.0/tests/files/store/jce.db`

 * *Files 15% similar despite different names*

#### sqlite3 {} .dump

```diff
@@ -4,19 +4,21 @@
 	id INTEGER PRIMARY KEY,
 	keyvalue BLOB NOT NULL,
 	fingerprint TEXT NOT NULL,
 	keyid TEXT NOT NULL,
 	expiration TEXT,
 	creation TEXT,
 	keytype INTEGER,
-    oncard TEXT
-);
-INSERT INTO keys VALUES(1,X'2d2d2d2d2d424547494e205047502050524956415445204b455920424c4f434b2d2d2d2d2d0a0a78595945583432675178594a4b7759424241486152773842415164412f646b442b5337304453696e733853774c44747a6373366c594838674e444565774672610a2f4d2f36556d542b43514d4934354548476a76727263332f4f3258664158707054524a4f395155735952525165794a552f3038776c376b5254484e4a4b47314e0a66744a744b683335486d5864626946366e794368666434775979655972586f597278612f705a533058614b626342685355464a78574d4b4442423857436741310a42594a666a6142444177734a42776b51785374434633685833586b4446516f4941707342416834424669454539504f49753747556b6c726a41666845785374430a4633685833586b41414661394151442f4c7652354f76644972725179676d6b5138446a7a4878763045686634376530483230673576536a555a5145417a46554d0a5665342f567671545752504e6d4532695664747165436541373347654e576772694b443371777a4e476e526c6333516764584e6c636941386447567a6445426e0a625746706243356a6232302b776f59454578594b41446746676c2b4e6f454d4443776b48435244464b3049586546666465514d56436767436d5145436d7745430a486745574951543038346937735a535357754d422b4554464b304958654666646551414174394942414e5258324c5875476468793530644b2f447566736d56360a334d39562b644965595a614f33444c537a54634a415039493169656b4e736d6e794353576753326758696a50363236372b366a774775466f5744654a5067524d0a4273654742462b4e6f454d574353734741515142326b635041514548514c43565a6d556b2b6e41786377614a687039436363386669793647353735585a4e727a0a6a4b625975632b452f676b4443506f536e5150516e536a482f316d66783177617537426d69792f2f754e4a51774e707736444a4a4a4a6a45456e4a54736370690a2f5774503248752b41634e4f5a4255424e5a72634844575842434244544e31312f46364747535869516e76626d43765537334c4b6a6d5843774449454742594b0a414b5146676c2b4e6f454d4a454d557251686434563931354170734341683442647141454752594b41436346676c2b4e6f454d4a454e2f5278566b6d5a4930760a4669454545433639493731644c5451507539344b3339484657535a6b6a53384141436938415030526e47326e51675a7547516f38756347617554784f746861740a4432632b4176645030644f746b6153313867442f6164614b6a54494657485863644a44377173542f7a42522b63656c784c33344c7a4241614a655033364163570a4951543038346937735a535357754d422b4554464b3049586546666465514141732b6f424150334a6c45356a6c6d65364e74486d5a5a2b4636436e416b744a4b0a6c384c6c335a6f2b534730736f6e4d6e4151444e69477149594f697637596930734544677451306e69682f7571735472476c704c3146764b6a7136644173654c0a42462b4e6f454d5343697347415151426c315542425145424230412f3468656f4b2b4d596f49624d577a4273726e434b356938432f6a6f68383767704235482f0a4a52745345514d4243416e2b43514d49364e6c39474f396e382f332f4a2f756454484561486f44364a534456485441684b514e617355596a754e5a57454146550a567149374e3147455573716e62636d355545716a4a7154436a675239396564696f4947754b7731535258615342307972582b53467450716c44384a37424267570a4367417442594a666a614244435244464b3049586546666465514b6243414965415259684250547a694c75786c4a4a6134774834524d557251686434563931350a414141644451443843526e535639755175314c676e3165356539657850763435506777524c574b574269437a7644616943337742414f456a47386c61302b45430a4e63463442344570685667495a79563452644b4e33446a3367776578535649430a3d666275430a2d2d2d2d2d454e44205047502050524956415445204b455920424c4f434b2d2d2d2d2d0a','F4F388BBB194925AE301F844C52B42177857DD79','C52B42177857DD79','','1603117123.0',1,NULL);
-INSERT INTO keys VALUES(2,X'2d2d2d2d2d424547494e205047502050524956415445204b455920424c4f434b2d2d2d2d2d0a0a7863614742462b4e6f4c5942454144453056514f4b74763776635338497841616c384c594c4457343639485963585a564c3336534d552b4c2f545854356248450a5261414a3278495454657a356a5942727458342b7a2b34395a655a45435a314f5957354c314853686843414756784d4b50397774356a48483851415a483243690a65492f5967777a503631367735694571353254494b614b584859494b5a316c57493537425339622f457737696e437a62683452416b554b4169636b575056722b0a45446d573164713938505a4551783741654656706d354569774a5144414e716d6b456336794d376562444e5762504161324f3652516c67774c317a74374d32740a5a6c2b7066552b58466b6e62776d5559343534754a5656506a78517074466a6c6e353967446a3661505a2f48654477495864353052775a4f32413344586261430a487653766d434c63346a364d3856352f37787451423776542b6b74472b36536f48376a2b744e5847374774336159757030586e6938306a4b656e7a7250686b320a366479436568664e5a74744d7572765753664c435775574649317458377178487136344744786e494e33387a687970575a6e7550766869773550486b777756620a726e6a69447a2b522f6435704b6b5575574450484f6b4b734932794d4747704531442f737078646f48416c414f6a31495762324a5749414b396534523450382f0a67544f3556746c482b59384a2f526e577068696457716f32387739645654565a526a78674835676d4d71656e3636776d564845614e5578496761616f544556540a377634635976506d5a62733670326164715267456e52375151326841636a4241476b42365168776e62306b31544e6f447078523839642f6762755661417950580a57794a524f6f384e7273312f4838695a2b706f6c2f584137594a33466e64525679752f4f636f696f38443650684e7048506b506b5271475579774152415141420a2f676b44434b447864455a6e7a7862522f34707477685a69653242523335586d705238797853763870544f424446636f6b7477676d48316b362b483857464b6c0a4f3155325779434e5749627634566777792f3771644d462b4b793145544e364b426d68366f73685a6c693647737048795a3667357372436749565477393379710a386c5a697463457941673674554b765a3554505259394b70753352314f6e6645305a68584b387867745168714f76644848327433704a326a454e6d4c4f5a6b410a5948454245326d7039427a77463867556b433953526a4f6632794e7a734e452f4b6a6951476a37344f4f356579702f4e72643769796f352f304143595871324d0a774f315446655957684332386d31745a43494e2b6d76316b4930657a624f69763453446c32657638307267444c6a564278387a52676d646f4837666152484a540a744e646261777949783475723771716e77546a735a502f30454b676b39542b577373617a5942373935626c64564d7a4f57744b764d464b58305a346f4e3556530a794979376f736c7461594f78442f44647465314a6e3031474a32646f70616e544d6e754d2b50676d572f3243506b35497265717941486657484238733855684a0a5456654d627759414b36707075547163504a79575249424b6e6971394e6956674d5233594743715a4d576654593968794e4465753136746d3647502f366a45310a632f3572762b53796f4a64582f6d6f4c31513569644c515370446368514f396b65396b30476f53432b78304f6f786b2b72374a736b38655046794a31595076440a4f447565376673356d346e4a56717747395246473034574f2f575874733737486f324c3476516e6a436a3636464c7253617853716e4a754652393859613543790a4d47676d6a4b744c5859473042766d426c7a556856395645646e6262445249716c4734506f7a45546570775744744d55456262717a34673576696a4a6c3867390a36442f69524e4a6348665368392f703543527a31617a4e79544c4563725630333363344e4a6c654c3361497936672f437862424b447543566b6d6e626e77426e0a6a4b682b3173676e31316d505747333261565372744c75516c6b594c44756d5654634d75394a4d58562b514d715676376c79302b514973726b42662b6a68706d0a6544635579335562417370552b4648485a31736c6c555762592f4373675a62362b7478662b726538394944324464554e685a416c4d73595061796b486c7841710a695845545a626c4b475a416b49446541316771362b6a774974692b6444593470497a6f67335a44466a346d394c5a6d7a4c364a6f327852767142542b583163790a587349594b637064465a766b64707146424f54416967477247444f687156754165663065352f3466553671526a36415a522b45335330487849675875527a6f510a2b38393077364578515a3744687655454b546368424d544e734b596568774567657046524d307a6834486654373673456e396c434f32596a394c4262364758490a6d565458447037774d433158507338372f4b6b4f595a4f4f4847556a7875434941587a544e3033506e774954336277586a4d7676786178516474734533524d6f0a53766777654c4434614a4b37656750346a58567461306f50505a71643649467375434735416b576e324c4363663873682b7950546447777932366a636e5366360a4f6448415058317556454d7078345a574f7943375a31484f394c446d614154336f306442772f57514c4b5773626856514474677a732b6b61355131582f68444a0a38425a59527a3972506d4a3134483438304d72786d7156634875314e476c354f44772f3771347748557342354c4952365832495964714d664c67794339752f330a484776442b352f706f386161746433386e367843426c46546e41366f415532317959577633677974495343585a6b366873682f3839456d684d2b694c4f5054540a756a6d396c716b5a37735258414a7a65596938725042525459422f7661534a6e4d635753514a554241314a334d5844346b722f474e7435762f4c6358786c55450a53533279662f553959356f513549635a57583178686252612f2f4474546f5a3961636f374c33396f7533742b5434685578644e4463446e6d5a6d6a5638365a6f0a4263574a7a59394769455264413346437a3746627068655461336136713341513651524e3257307241796e6e77612f3055652b53764458727a515a396f33304a0a7a4c6c32426e52775954646e455647373770725a63643564674d506a3676596c556459524777454c4b6534725a355453727a675078396c37724659484a6457670a584373456f644b7645424d446b557957576c5748363758326b466d626e615136436f5a707170732b464d52414a384749322f517149786563462b3050354c44730a616763785053595747534468443931435778425732785879574b2b7463545a51326d4b372f4944326458756565776a313143797a394d4843775945454877454b0a41445546676c2b4e6f4c594443776b484352436878634e6b3631756149414d56436767436d77454348674557495154314844454f4174776264334868647469680a78634e6b3631756149414141314f6f51414b2b46713839726e52424246795244325850306736627659636358643635664f7750446e45707830584e46772f48630a692b5046642b6a65356f444d54657a47586f4b4b4d364259626e7135363274544654577751543259762b7a4d2f715370312f6c67616c46416175584c495841620a6548526951336a46537551675758764535464a2b6a354f4b30473448437770715a62734b4d4463753062722b306d456f52626970742f752f684457484d7158460a794a41754c366f4b7446546f6b754d763470517341744248355a36595756566c66526566742b37696a783454513672324e5a5254726249334364307579522b4a0a37352f6a3942364732372f5066527162676864362f586f4c3430666a456f383773466345325242346439386d563465776955367133725078346b7a7a483271660a6d4d365947724663534c626a483657787546717944313543356e6b345250796735766e52577756787969344b61576b694d6e655274356d7a504c69386a3150360a625362424f487a6f644c4e2b634d48447246795073715153583741427842464f5264434d3161504b504b596b333564756d454d6644736b61614b74504a524a760a4b61643073772b566b586b577670385061724f2b54396c754c6748704e54687a6f49435348754b464563734f4c4e6d7a645375484431374c3674627a332f2f740a5a694570686164555561472b3777463767327072374a444d686c3250426744464d4d68776249354452395a3856684b70373346596643325844666b39696855720a37787352794632644b6e7a4972356f45436656626d337678664e61416b307855586257743859706f776572494e7a7269326f6e45446652667635654b6365357a0a4a32677a6d424b47556e626b344d4a307979656c66386f636c546446316464636d344366327444714c7a7a7868705965443951764a7262595a4349797a5239550a5a584e304946567a5a584979494478795957356b623231415a586868625842735a53356a6232302b7773474542424d424367413442594a666a6143324177734a0a42776b516f6358445a4f74626d69414446516f4941706b424170734241683442466945453952777844674c6347336478345862596f6358445a4f74626d6941410a414e6c54442f396e4c702f4b576f7553784b4472366d75714938697759516b45502f4a64684e307769384e6a51543055364f5873387a342b616d645675722f4a0a4b3177416356506e742f62377145745a4d6a7466455331686d774248434a326d427667525a707472314e59346f4c4d683049737457432f612b77757736366e410a5a3343554970665669334f2b2f33436844543273444355634b5a6458714232344239675763485378746a3335483973694352593577323265636676444f6b52780a48552f7774743454585a5258305a4961426f2f54346257397876516d5257694f6661576e47326b5a30383139666476326c36314d67776851644f5445756c4c460a6b6f636678724d5732745a6c727a796e6b69497a623975387773415577714c303876396b466162574e6462504e71713444376b45436251666e65575850377a4d0a4668784769546e743978306c78336d666a706f6a75486754534c4f3356316a6f31446e67646572742b573839702f4f6962546e5848414c774c6e7239386a554c0a504a796736506469796375706f5050456470575a395450303265713377522b343770444d5a3844425a6778362b385874494e774736784b326b6e6248796d36470a55687431714b73694e724b2f4b79664163447469555637654a55356532512b4364507067707632694243354a58354d4e3841624844552b64644b386a4c5a656d0a715a4e747532525669554679526842556e37484c624f32667558564c73753544453274556b427a5a464155546b6b5272716d597079334a66687142536c4e302f0a47673548695378564549334f6b3463526a486d73714a5737553878337a71453144384246734a4e4d414675376250386a366c5252795858666333324f486b4a550a6f7176555a50623132374a6d71733237472f56364f36513565576d7a4d754f695861457a4944474f43423571624a4d6958636647686752666a614332415241410a716f422f714d446836652b6249412b4f7754616c6a4f515757647a4f594a684178656559564e6168524b57646e61476e7858766851637979692f4973793659760a335933674b4362496443343639376361654530476e4137497145654d54546a746869645a4537415a4e424c664a5157572f75765972692b557141576773704a4d0a655175447a667a79666e2b3746596e6d426f67727469546d4c744967486f692f6f59486a34314a50436368726e6876524369744d6132684954304c57675947790a4b6368565448414736464b78596d6a4b497662586653467753494b63497070694a2b365a546a6b6249564b6d67536c386a654942796e614c53394b746c6f42370a352f594a77707756415a4234646d76456c7557474e3939516a456c47355a2b374244563431623238326e524f51462b54517553614f586c48643771664f4162300a7458755a453170347a2f3766364771485479453365624f6d69685463396563676f6a42657a576c2b616a5070585155523066517859366a6c5730795653495a770a6a4a746a6e2f734c6e4657314c52314a4e57364254716d58644237714b6a6665656a6276586a577447454a656f2b5967614d55575563797930646e777935446d0a3246652f55555a476c4d546c32677671724f384c7652304177704d536e4f6d467958447235393475472f316f3461464d355044594d4665674e6d2b483435306e0a647a682f316b384f4e747868624a682f58364f587a784e3451773073644f4c5a736649485265435837554b74427963456154575278597a3642673250575537780a74506a6c716459686e58456233496d2b61354571734c477458666251595469747465494d46362b3768764f4235597275317235546c68446467767a31617073380a7650464945336d51492b697272596378666f706764347170684c555a466a782b525a4e347867667758616341455145414166344a4177696d77355166305a58760a5966387449533551544b784b3331616f385356325153342f4c6774445631326c3549562f4d4b74634a77687143795158486b4752494d76656f4443507767794e0a2b45716277366746767867546b32644f3150385a487a614e6f6e762f69766e4d2b30444b69365377337a64354c516971574f4c6e4e4f50445a33494c323342440a456e68347a624465625839327636764f56356177667a4172756d786c6f736642537668597a4162594f5830505558565278546d714e375144634b5641306a546b0a44306d486a6141526374617048417a374f724f4b776e63514a467959554d454176514d2b4b734b4456536d7553357558514e72726e6f357739746d4e6f5967540a327a6e35546578475563793059586847704d343742484b70324d3373584139677a3377782b2b2f57784d4963794649307339484e7a793853456455555a6b46580a4a554465777073387654304f4b4369504f62434a3666476a4f33656f51305450655966526b73334b6946766536526f7563477a46744e76797a55665550612b630a375a62492f627a4f34636d4166354858547858526463494f416d435262376d7a68634f74506e314844587476587056364f4d6643667059644f7467595055376e0a756333457867493634313975556a3039437570496f2b316e354e744f7869475173586c4a6a777735797a79554244755363323571426538384f6f46794b6f6e300a697053535175767649584731436146514e7848576c5842624276566f78362f63332b555339425a4e463739323135535664544e6974516a4164312b30346538780a775972425955413831593957477875503972686a646d48564d4531332b7a42356758635230504559704b627443694f424d385242415a696c72522b49456f69590a51482b4756524763317a634c654868492f386a624d32377949694f4c6831763966346546736d757854716e654355315a50314c534967526275596330423366560a697652425344764550414843664c72596c356e3243734e4376757a49597074457a374534415a33544c5366417947792f76494174743376696f6d6e47547143330a573663457a4b6e652b6e65564e704b78753130384d73616e44336859325a7a6677546847394c6432634c326847687a6c446762474b3134612f6b454e4e546c470a4257447170574d66644647627255394147323849793371536a4b635452684b666359494d38466e79423277655a686d736b59305a554c7846692b69764d3853320a69772b68416633394a4462747962716741342b304a5a524a42786148633266386b67445853795736303955345374486e396c2b74564d736a44356f777a386b570a45326241464747646678706c45634b366a61304934497251414966312b304c6e4e475a7971734b69576a376546433267365972697871674f78323477576632390a4b7457547858506739677853656271564930726d322f4c544a62375853314c6552305950465658747458726a734f456756437071472b3555416f4e77485067480a2f6e7754716e5162535a4d304a5664327365496d33335547794747755257586436544b59497835544f35667754355654624d6161366554596c58316a777750530a734f75627143454764735648724e7869495271553862576e4634623056655461655a2b7a4d304f70316351486d61776e675553764a51502f4f534c77446764390a796b3144696768646d5748775764514e77442f494734374b3976524f356d386f6b59317067704853423846484a6173576866657154756d7a69564c64502b58640a6c6f482b496c4242317641467444453153317634543952674948533476524173464e66447252366779464a513979316d515a524f32426f6a58744b7a387658420a4f484a56464952685857587a767835337252786a37525574434736626f64544b53322f3663626f78596678444e5653654a355177416f777163757a4a572f4a6e0a3467316b562b7a6c4d46694b57624b6543323838454475354349704f417a443238762b3144585a784a7278484b2f4c2f33786d65566264595471304d746e666f0a58305a366276476e487832343349762b6235356d31366e30504665774852326170327271685a642b674433533743642b39664f715730507956554839625268790a354d5968464156716553377773425a526948323730374d3574795566593247444859716c372f3068514c65565a374c4176493271557871383542573053766d450a494172683457396e74444b324443487031684d556942474a6d74453574355666486a303654336f554438534b59312b2b395662506a332f2b4c7272704b4c5a4b0a516a797a6b703865396465574536744443576b4c675a7557324f67303159627043546e3136555465696c6151764a5670316c6974376b7854714b4445746b69380a41614647487270646478565164336d4d48737752536d705a42317464797443365966434f7032737877734635424267424367417442594a666a614332435243680a78634e6b3631756149414b624341496541525968425055634d5134433342743363654632324b48467732547257356f67414144722b772f384467442b7265334a0a4448763268685944353971685a306870444f313369744b586b4241587774767273572b456571424a767564684f697a564e6e794947336266767349424355486a0a306a515a563241384c4939435a5556615953784842526c314876702f70726441624534543839447961515a6a2b4d796b755a412f302b753451714972554d62570a4d6559557061366a66754a44347273767245646336556b6372686c536a61356578466b39386f4d4747772b7a5276636f49746e6c6e4c494c6d77347a52316f6e0a566e565a4e557563616165617146687442465a746c4176687742364c62545579737530707a5167766c445949546b46462f6e4e494958364b763850743970656d0a42726a4677656862675463524461713058732b43655a706964787668334c37796c33767a667274374e6f714d58314167416b786d6174486254305558737441350a717672585058425a4a5a4c30666c48576978342f58347176506d593535335866446c466b6b704547706548515137766e48655147766a2f79616631754a347a4e0a5271684131307a732f6d4755364e753859737744674e77376556704d53687a7758736538646d523147424f72592b5a723073566649467564514f452b32592b700a4b2b342b6c4336634276684533776d33386162547865754d6a36334d69426562454f486b703137484c6c3166592b344a41326c324a4131627755746e41556c6e0a4770363469564e4143442f33454e57495034594664484761556b6d2f692f46307a6d2b68716c6f4a317334614953726958346a51624c4d3677564d43303033700a56774e556d47735a534c35793159644132524676795342736c7637474f67385a504a384556463636317745757634744a4a79572b426d554c4f787a6b395a2b6a0a354663734f676b6d7356314764474f554f505046487a422f78454673392b7868784c5048786f59455834326774674551414e424a336b6d316472396a34702f2f0a59317939704e69686a424757315569704671322f324a78584936624772364f6638502f676d487870307750494f686334535455646c776b6a686d36397268344a0a4d4c484e517974776266374f6259714f6a6a3339316874666c343346644c4f39504d67495650524231376d4e6378717a67713067706255684e68796e6558384b0a696e647163734278486777537044643679416f342f437a42594435537461336f39376a673143776f506f4754765176414638576173454b654c687453747a556d0a2f4f79666a656157645a446670566139465a7a707471476370706c31664152657a4c764d505542343259554b35707949317437786c725773717979756f3076670a4949653744766c2f5448654f63716b71576978456f714333593732797233684a2f694d637552742b496c356347656e47717a49463071415552325346797538790a3668354265762b4f657158557639664a69354c3930686730356f3432575a346a54556f32482b4a3278556657645348775862742f786a6d534c6a5a7a2f436e790a38685741505635497545447747766e4f3872795547762b7177357a706e44393649664f332f374a487130453037704a466b7575697333502f5a474253357147360a53446544362b33417a514f425949733270475855715a653034654b365a436d7450496635316478452b723348637859307559544a32574e7842357058634f74460a336f39312f465839446a3269535a574d52702b766c4b7752506d4b396254445431744a465a38536b306e6133456b79504e342f4779444d375838566c4d4439430a5761485357346174744265586d676b6d4534637772522b6951656679304b597834443566463765534f6f3273414f4b797343674c6f3079677935304c754f694a0a6f78322b725271364b71745a412f644a7a47327a556d47576c504d74414245424141482b43514d497833476a754172554834502f335a783559497369454452470a635871786775344b53476565575a54483352736c765a3034545577766771485a4979337937376e4665584f4568794f2b59347539356664435653427131685a6f0a77745979767368735659796d7476507578485478716c6d68774373516b61467170614b465667492b35726c31306b636961507473413367534f653665715654330a4d7366314346714538753637443631685859667270714744754f584e564f615a72734e2b77476e59424f4e614a586336625139553733736639314571433330350a58566e4d45313148574b54773056384c7a46494f463646454a547130374b644939766e3344496f4f636f436d636f71704e33457a4c4962514b62326c704f70530a392b6c4841326a62727838564575767669577a6d7a586c3133706a516a674c7477425032713937443046486b71432b746a4a6c787a4f4b546c737969464b33640a2f45774c51477758303159544343526f6444316d6e437074694557386f58765677456b794952364b4771385a557071633479654774395541794f4776755276410a3937317a4842594d4c56567a67564371764f4357714e492b364a43742b74594b4c56457758735a64515278313254777949555a422b7854564354396757795a5a0a34705174783231716a7761306b69765a333071587237514c57484d336477675331566f4f546f6c7452504e497552686a6a69507468476e7865624831373259470a626d666f375541755561305a73364b36496a556e50745945355666784d576d747666457158667441416d334c6f324a41527479476b4a7a453046776a323636610a72387157375751384b3044314474546434526e58505247525444654c717931494a387a7444724c59434471674c4648506d312f686d784e44334d6173624a65520a71793548594454395544394b506e5a372f67533371494a2f794269724f367946356b6b6250776936326c69696d614942353072782b6c4f6a41784636635542660a642f38334b482b636369334a6f686c2b6862422b54734a49787532526430796a622b75354335437568495737482f79656d67414374466c4143684550727632470a38636a754e7934746a677a357952677a342f674f7169365978457849576b366467766e4a59735a326c644d7a686d64365848476e334e49566b6e3949422b76680a6344575353376e4977736f3443662b4b47424a776959432b494a48416c555556412f2f3863677630756d554a553578722f6c68706a48766a4b74454e426f4c560a4669563970425555576e2f61496166562b502b4a4b72355371726a4f386c494735444943705239394a663938654b79657443726a6b61556d6a634879375039390a3855454155535662472b572f4f674f793856562f623250336d764b5062332b645a5a6e2f654f71466f645a43494f2b71697a4a566b6a364f78593930736d43660a524c6f6a73636e37542f504253374a7561794c4d7578416466596f555351417731544e6e316b4139497a315567374d334e33635a4a442b796a6b7441394562550a6d3778643764763754675057647358716b684339375745475353395a2b6a5741676f466f33596735756542483073614c615756564d6a7954735a35616f3756300a475633685776357051374a6f7234734f745553496e4c705046374a694f466e37397232426d6d4b3851684251726c42694b706e5274713649314f5061425649390a5051586b6a304e703873794266784c4e55507264335973317043494e7452676b59684c41564a73666147303652753549584c73736b70332b36396f52724e726f0a473165764152416f506d646539517238597576434b714b423776576936634d6344516a586b774c792b75615975786642514d645a4130746f4b634e4f315a67370a3272764c38774b3846426168375a4c38384f6643707a55556e49693666747659676c4931367262434e735461323678516c6b455531596d6649364432494234570a426f4330684559526959555432503375453058502b49557a4f454270526b71426d6865536d695141724c6477766e79394a766e4837386c6d786d645461674c490a6b394155632f4c2b7647517254346658364f557972427a7a65396e6f4e3945787962416573366b32783444384a504d4d564b707632776b4278567755435068660a755a6d324d7a774b384f79433464506335576a6a5a784a72676a4f4973497446454f7a624b6f5333362b505844684357555a314f69425471475a5a4e747a6b420a5375506139465337354566395563667678704c524258593154486e3433616551475a315a553254706b67356d657a462f6e356649684f33542b784871414673590a303171336c2b54697279487141735349516c7236366e6852397a5a6a5066776156674f4942616168344355694e6761545030544346376e557459744c707577330a68674b33477865556141546b616b447750564c5534373279784d4c447277515941516f43597757435834326774676b516f6358445a4f74626d6941436d7749430a48674842644b41454751454b41436346676c2b4e6f4c594a454133465a31677175514773466945455555506c6e70674973566f6e464473754463566e574371350a4161774141425864442f30597a73654d2f6753724f34466477633035616f5a3568464d5949746b666a5643725a6a6c4e5a48757867742b53507930716474654b0a7331477663757a6f2f4462467643743238535768322f722b6e5678324a4c70532f585251706543565a536a44446247314f42634171446f496b625642507851580a424d467543505946344b564b32764453694652674a704b39444f43786563334c6436516e786a5477495577736f427a425649494a6c6f497742545249373667390a57746a6875437758754d342b694d356e34547951727a77427247446b663241416776594f757a4e6d4966726f744a58543550332b37566e50446674794f4b5a500a5872513772526c4d55416737384d3943706a445330616d595750716c556b4e7166713877696c6554466c3957346e51746c4346375a6839494a786e554f43354a0a712b684949536c61374364695a4e316e397864496a625a425337685a44594f73756443613479643337384b796b53363239696c513252442f74714f516f495a340a614a6d527573377857763975766c76427a6d5534534e653238624365337a385570644352316a4268445a4c3061454d39454d7a465a75586e6d2f6c59376a79410a4a6d797244417861685a657567394c7952654a6e3734324b6171364e635a476349364a6934396c6e426a5a434f6832514764525a636442706b744c3339315a730a676161734c676b3476665231412f506e4d6c33344d68316c78444362377830764f7a61414149426837656963715a4f6967636a78743549326c4a644269376d720a635a4d7a544d4361675164783770745772544736796d4b537454355a397831454d2b564a594d552f37546278786330384152425a50526f6e32634c79542f34670a61716c6d34346f45723939496b5354525559386f527170494c496c6248357362774b454b5346676e774552722f6f7665544f457147785968425055634d5134430a3342743363654632324b48467732547257356f6741414241376841417736417232526452584f542f50636e627a6679646d5861676a6733474877725966664b380a517031596e6d43473948356b5a354a6d45626a5069564d752b776334537a6e3956794c4548432b797352517a453254696c63544f365157522b30686f526b2b640a6a6f4935544a444549384c57466a5a594730347a6568467869554d7a566d35526a4a364a584b5a496b626f41375a78694663555a314c3932754d4978532b4c6e0a4775704455644c2b67346536386959564e696e76445a684e6a75356a394262716c734c33564733343335536a39727435466250674164343665456156695a55790a4b35493551796264523457424e46326d6d4a5a6e7270554153683630494e36487372753352662b675342507531786b744d526f4648764947525637326254312f0a37434554344d303539326b78625a677637616b70477a3546477a52465a3335776e2b794b3463736d4e3931423832473761445368486b444751544a4e744842340a7271514d6f43557376426e464e694759515650327555467469394958386e346a6e586966425356436456306c686946776d434d69645a4a716837654e576842700a54386a4861736a72654356424b556f704d37716e31584a5977643153376b5673414e34384c5a692b53665876716e594446797a5649375141707449624d4261640a4a5748795953472f396a4d69493566745a415576483457734e6b346861785570726e632f4d36424833765a58506f4c4b706a387662557565533673356f4661780a765839666548377274584250524a4156786936557671494e4d63344278666b6e4776736c426844436c4d78613530502b677638665a71723856695038734744750a6771793378663954623941703665616e44463370675a664e782b78712b475732676343526a39686f413075736565686b565771366b31762f2b7a506b797a33690a6b7268736831343d0a3d364255590a2d2d2d2d2d454e44205047502050524956415445204b455920424c4f434b2d2d2d2d2d0a','F51C310E02DC1B7771E176D8A1C5C364EB5B9A20','A1C5C364EB5B9A20','','1603117238.0',1,NULL);
-INSERT INTO keys VALUES(3,X'2d2d2d2d2d424547494e20504750205055424c4943204b455920424c4f434b2d2d2d2d2d0a0a6d51494e42466e6d49494d424541444b636e41477469387959646e49396873372f31336a7331456c722f516b6b46415132547a513159383056564d454668684e0a6e697a7966387572783933707151336f2b2b77455841414c5a504a72764230546534436b6f58776233562f39386a79707749366b4841696d45323833754f656d0a4c4467516f6f42435158316b464b6b584b74765548416372634e76335769734379523632786c666d496e4a64735358736370766a454a4c464a5a5a637a504e330a62563076626665487267575a414d37756371463474724a725373524b787337723773357767774f36383846354e45514c7064743061544c4c2f304f4c305054320a47464a6861466831614649533268793652586f5548627856557969474d336850516236303731566c69476e426a7174696e31777337455866387163514445344a0a737869454f677544314f78586246794e6d39306f456d6263674749665844664a774e59385a2f4444394b746b747957744e594a31416630526c51374c672f36420a6c717a31626133316d744965557a6b6537414237644d58326a434f6263656d45725435486a6b56534336764e677947464f6556466e583162314f7570495a4c340a4454615a7131797775596e6c5873657972494d7754542b674d612b554f6c30462f7764775931524544556b4a31636d42582f75514839755354496a51725a56370a754445726e4f7941394c766568717a47366963746a313771726e5553304c4178506f6139475a786643363439366c4966645a68497336634b76592f4672714a390a6948543573306b7959554455574f472f523070733661425741766173445757675769494b3169354168706e415a4e46355167764871447a346d2b56452f6a59790a51586b446830426b75704a7277585835503079677a5642614b6a656a55625a4362374b6551366c7a4f77554e582b6c4c5a357a6c416b524773774152415141420a7443464c64584e6f595777675247467a4944787264584e6f595778415a6e4a6c5a57527662533577636d567a637a364a416c6345457745494145454347774d460a4351576a6d6f414643776b49427749474651674a43677343424259434177454348674543463441574951536f582f4e32645a795a536f6f52614e6a59495a794d0a512f624634515543576559686f41495a4151414b43524459495a794d512f62463464374745414357576f6e6d527658495a655050655273612f475a43567277780a554137335a466744783630674c306f32776179716859697743365475515061343234554c63694c5770465179346c62385977415a2b6d4d3979517a664d622f300a747642396377643675717a4e497a31514479483239754451724d386b4a6e454668757866496e592f574e6163513831364636616e4f6c545271316a4d65434b610a44375567747a596a5a2b3347546f32554a7168497059426d4c6d2b68324e63366d475a46567149706a7a7347522f64526a5a4b4e4639646c4d2f387a6d6448500a5a7244416b3953634747757a4f7752514468716d38345845737564504236374b6533584774303134595a62756b7146744a6e78614b2f33796763317a4a4c35510a614a4236786e79756c485542396775533556614454732b4234747334622b436a34506b674539497553307859434369545151642f314c58304b444853497477320a434c4c4b31714d476a584e65544557497153496d7a787a475273394a3537684157724c4e754a707665685564675879366c486d6751744e79744e455576536d440a3059466d6d2f74336a673755504f48634e4a614f4d765743547271796a55576438317670594b75315551514747366e6279792f364a6b58774641714c55536b510a545062636e3752546c4e6e363856672f304f4270776642564764484d6542425335544475394a6a6471776442746e70624446357a4336614d5777346b435946540a3532412b473869627079453266792f532b5a4359314a65574a77755746634f49686a7178482b634742657278552b69544c4d6e5a2f32473176356973776265770a6169567a4847614e6c4f5345552b2b59572f554255337858644d354d496e442f4d6f39576d6566723130694a6b624e2f644c713245394a30427a416a7650676d0a5757554439496f6b383532744777456c677251655333567a614746734945526863794138625746706245427264584e6f5957786b59584d756157342b69514a550a42424d424341412b4669454571462f7a646e57636d55714b45576a59324347636a45503278654546416c6e6d49554d4347774d464351576a6d6f414643776b490a427749474651674a436773434242594341774543486745434634414143676b51324347636a455032786548763542414170432f44646c3076457a4b664b3952770a793253494c4d534e326d4e3133375a756877306d674635512b42383556583258504947394f4751517143344156597635682b444b556c485332696448705838550a38344c5373476864304a66416863623758635538694a685045477a624c7579675633427267364556663065525042324d496c39346278767361417a36443454610a76494d2f4f3553716b7379675139644e6f6f472b79312b786b507378485a4c516c6c5131505a394a477531747666316c67677236765a41535974764e565430350a436d6667376b7a714f2b392b4f6e4b3641496d6355722b746e7837694743435976456d696369356563356f72785158344d3044714e2b75496b397632757544670a6858594a554a787537643670676632755432336b587439666442372b4c684e51737150453645556576472f516e693934397168374f4e434f6d716f72516f6f450a4f367253305a4859426b65532f796878546754472b644b357430362f2f7852596c34624a6f31574d30412b2b577235392f36353549734d65467833464e6638450a416d4d434d6b622f78424c66377345694443484a3531636e5a4156757332683969696f435a41664e59326852307539547634305066756575344139626f6a55700a7734467243513161356a4c4353304d763639346b54664733595730647555754c2b515761472f644d4957626f4c3331545175666346587676696d51472b5279420a73376436426166384270787a50464d706766356d33623930326149397748306b326434383038564170384b372b6c7353565a4a374773757673596258507948360a673579555a625368554654457859373469644547476374566e625963695952586947697745554f5445395742695932576476504d4f636643453347347848494a0a45444e516c464f5a7a7a53656c4c4353464f547553753750756c4b3049457431633268686243424559584d675047743163326868624752686330426e625746700a6243356a6232302b69514a5542424d424341412b4669454571462f7a646e57636d55714b45576a59324347636a45503278654546416c6e6d49566b4347774d460a4351576a6d6f414643776b49427749474651674a436773434242594341774543486745434634414143676b51324347636a4550327865455a71672f2f576e56450a55757643646c3164397331674d4355574c6a5645626f6a41645a5755614638724d6d33586d4136446a55394c4a4c4f57424c5273734e41327764506d707436690a43625a4f4b41683563436b457054376c42427967553244677342394e6a4c656543517474574b736d53656c546c644b3932414e706149496355523437344c32750a38563742373642596b774b3773417a38426f374e36344d4d6a384b4754386f4e6d6570697844412f61684e4c6d4d6339525654483832647945535675567261620a79387255365844474264662b494879597266754d696e7039725255316f4c6b2b444e592b7a4743584646377646455451336e335476414954557361654a694d4c0a6e6144795a4e74743269423674654d3173512f41573175747179396f49514c45434c4c4b785a495a5866304c6e495043336356424b3478456667516758647a540a6f76465155447448416f4d6e6b5065427978614c7770786c69565854737268302f49736751676244594b6b426b506c34776a35504971665250374b2b55712f590a792b72374a434a6b75777a4e556a6f4134446458614b682b7543595976776a46674335444258427570333758596a44676237384a4358774d632b527a2f454e450a4a7a326d6a6c676f432b3134644256614b38614b39444454486349725031655664333348654c34676d573267446f446d7652314d646a3443343853417a4153640a6c48454850415035324d755479766a774a446d58716a79567936634e486a6653587461775958575a724a50482b4e543359765277727767797a5a457a3477616b0a78516448384f7449416f5a313344744d5863767264745944635a556c6d6550566b6e564b794777326f784b4473764d6e33346a4e6d3452336e33506f71426f2b0a623972385835787567492f636e417a4c5a546c756d526c56566f56334b34446972615173503875304a557431633268686243424559584d6750477431633268680a6245426d5a575276636d4677636d39715a574e304c6d39795a7a364a416c514545774549414434574951536f582f4e32645a795a536f6f52614e6a59495a794d0a512f624634515543576559686b7749624177554a42614f616741554c435167484167595643416b4b437749454667494441514965415149586741414b435244590a495a794d512f62463452524d454143764b514c374e706e4a463950654867726d684a69566c4a576d46764c70624e486a753161622b50535a6d6551494f5437470a543849496d2b5355464e7a782b79795a64746a63427a746969335575684866374a47396a6b3553635038656f3059764b6733517647687a4d4f77707a347041490a445370675447697364505a2f537163774675337349716951314a566a54494e7a51704b37577253536456446c5154454f485a54416650735044644369686964740a7975722f6937554b41422b584b32716f346939346948702f3547656e3966494261724b62766b4c533168596c746371494a6643694c2b4453516b3073394643300a7941363751702b54626d685964582b70416d50576b776f512f71763269624b77543269584b7a432b6d58494c4a4b4b335a4e496267792b6a583072344f6950440a695356716d773356617a6d65594f31326979685046526652574c3433354b69464c792b4e523665554a4e6567346f64336452754156387a366b7a6b77396337660a782f6c354a326935466c2f5879474a77526d50576e544830666c78484d2f654332794c7050684c656e34754f496c76554e692b645235393473365174304b6d4e0a4b63555a3176744a432b592b626c4261626a3156597046306f51736342723148776b4a6543354c79325a3264776a73454e575568506b576a536b6b39777077530a366c646a357a7331635a2f3378686a2b385a705a74486d67305547796437736479616a36516949776b7a52736b4547724148357656582b52732f6c535173344f0a4c4a5943374f624e32785a6a7041343545724f5443363331716f7877417542424f4477394d5344353275315937446d6f6b2f534c44544171585a596874726c610a32446477644767786f3257326554304c633732384c4566584b6a6a46395a516457446e39545154716e3950397a586936586a31495350595662726b434451525a0a3569482f4152414173566b7a513545302f6f4b5945486c665945382b43424568656d31374466696c7957466971326979526c494f354b6e7853464f6845316a2b0a6631773077514f68704b2f6131655173626669584a415777736b6974656f685a58557652446d61474c39787a374e6f4458526d742b33646134594d78454a412b0a3270656358533245596952463768376965544d446c4a555971334c423977316d373042365457694b624b3677324c36672f417737574c553865797458387541590a72314b4b714a7a52777450785654706253537574374e55564f36684476695a7a70556c64623153586e6579685036324559424a42757a693956437174374c36650a476865417a43434b6c6b514b6e6566756d64726249726b46347253565933504d5136717454485179646e6e2b77646159452f4d43536a44424a635330542f664d0a7474456b3068714e4a504b7035546a637233574345482b5a3946753850744473666c346659577631767153505248563551706d68327a52464d7744456253504d0a6350687345356d4e705a4c74796d4230413362494b665a4177683178585470527a5254665445517745304469364c4270552b7a3831676c5666386e4d4870666b0a4b6635314e674e736e574b692b3774544331697a48303576536c4268706149754b6166394d62466b683141536e38306a7059466379457748656552416e6456650a5138784f5a6c7a786264774c4431796e6563517357684834387131434176506e2b596b373630496c554d6332376530613579664a3873516f794d7148544c43430a37575a6353746e5246597957622b7863596e655354643857486e79664e6c484343667867476b6c44674a7a44594a43342f625876615270572b6d57346534544d0a71677938686161755734696150736a7245506b367358687346466c37794f597272576479776e774e753065516e6a714f467673414551454141596b45636751590a415167414a685968424b686638335a316e4a6c4b6968466f324e67686e4978443973586842514a5a3569482f4168734342516b466f357141416b414a454e67680a6e497844397358687758516742426b42434141644669454543384531456c36792f356f50694f3463786c2f77423864585a753046416c6e6d4966384143676b510a786c2f77423864585a7532686c6841416d503745524d5771784c66426b61665143586636336957694a355037414f306e6e5152596a52534948317264747436500a727042413958783176756a357645683268754d76346e3730612b4d346c533452456c4443672f6e447a6c4872466b50422f36534f347a456148397946444b4c410a71714d7863386649476b62762f5230526f6b516d6271774b59414a646e536e6b7a64333350515650342b47423545553868667074316337643854473631632b480a7339317573734d414b4637454247622b38735a48394a797a46765a2f30364c4e484a6b3172546f75394d4b3277505a33676f7739567a633861754544734d51700a5455324953796c48614c417064493642726b74632f753636514c463247496f4275365044485675776f70647852345339544730727a344b78376149642b3935770a783057695a7a4e43635835524a615842596a32416931514b644a437a6c484c6e42367737413348554f5471422f79657646567a506f516f69794f54373637434e0a4b3875427934647131714c6f596336664e524e6f427930574f3457756f31726f7877534d5a3048764447477956452b64524973655754584245675236685430660a625658535771557479574665612b6e546f5a783868495a4635514d54357441373975436c56654e3443544b6a7a5032786f684b7150324772782f6279466d6f590a2b2b4c412b6e552f79397075424d5a4b4c4135456f52614c384d6a5742776570667577584d2b5a6836507767787963427a7a78637543767a544d516f42686a550a615a7a556e61413544384e6b4a6b4e63426e2f6467347467653735575776747a32316b2f36515a44686f41425948464a344b745442582f356557566c49642b6b0a4444484e5043737350364b4b6c5956737142597365556a4e70506644537836486a484e7536794a523255326f726c4a314170367a4e62713962434e2f43412f370a426c576d59334266756f2f43424b503673694e614c36547955576464493352776349326e6c4b643775757167647643575a3668426777507345773845655844760a696b41333371432f58775632384b3331383056674c337754656f4a754230786c6878585a38583866564a447964484968444c487832523377556f3068644a716b0a6d556449324354375576364a796f32524833474d563145506e584d317038726735424370516d492b6556645734594c737572535252474c7a2b59524e395879700a704e6d364f715a64766b4a7a5a546f477970354f5a4835737339556e6b4d584968485768332f737648375279397042485a765155536272774b63624b68766c480a485242744e4541456a49733631664e437867714469625a4d452b5748525171754f5a575357596d7563546a374c6c5a33446b5837574f36584565357649564f780a76466f5851614e31555a396f766d53443652766d6c34624b6c657635326133547761706769614c523276436577506a626634417a7741736b59316b35652b35580a43677645593378306a74796c38684a507741334630775676526d786d453262644e7834652f4473396c3435646f75756f32596a654739505144324241517549410a32306d6a4b78346d784d6f646b7479794934757a476c634b57795772504478716753487a323856305a4d41747754586e416a4a51644b6e396d687358782f4e610a36796a5863697045747339363343376c72682f51686a493845395243414350455146562b30302b4e4f327956326a355a7548695479687666564b764c6b30577a0a2f334d77502f6d6b73517a6e5054316632586175554c694f794679684f70346d3752525967696b4c497570337a5176522b6a494955746d4458366b752b772b6b0a377a67622b52596661567a6f48392f6a5935666b5a6235526d69454a39595037504452663732354e5367613541673045576559694a774551414a786e4d32522f0a6f6c54613447456148422f42356b594679654359684751526b306e73616d38356845434263696561434c4273715433357349624254393269446b5137763074750a4e783456575435617462382b755a74543535413949716d4d6b4c64456130795931707550586642515164365a65534f37586431366b776f4c2f68757a43356e690a456f41575164637237476b346d6a30752b337063477961473730516847386659356d506b7463786c38725a536641395566454853534330566f6c394c585069460a58513854786a3978553665316d5377515056574e36644e30733645564e57656a68364b704c53456f5845506e706872326f5158614a50454e4872707136446a740a6e6a4b614455416e32582f2f6d723030587553627335542b4247617a385a705738713037327355534f6d64623236346642766f2b4f562b4a554353434b30632f0a5235356452466d6d67556a2b576c435566666730454f355a784667704c66564d69614330522f7a3559623652753279774d682f34336f5477596b4348506a5a440a5a506a5362325a50766b6568782b794c7362434756332f503539555a757353327a7034375535374538736255624f3168345641493375725a3676786e7a6256730a4533515648306f763957774b4c6653736856546d534378557759584d4b6b5841334c474f5a496941426e424c6e592b775a4e4a6e493439763447754f566333770a3868635870566b3659702f527377474e477542786a2f4e7453755a2b4f4f2b524a45565643344e6644454f30726478624b79646c4c68772b424d4b756c65662b0a6c70556f314f61764c396738794d796f34503271433152356b50776a7344724b2f504a686d612b366269377969317438675a70373179757167623664383230700a5364714f32356d50584a65444c2b484e43473846426b5663786148655269736a564c4378414245424141474a416a774547414549414359574951536f582f4e320a645a795a536f6f52614e6a59495a794d512f624634515543576559694a7749624441554a42614f616741414b43524459495a794d512f624634556f42454143490a356e42537a6658537a542b6b4d6b667a45564a35354e5736774b7166442f48736f6f574d5237355631613074734a3349766f6f49344a6b7736554c6d585032780a4555477168536352644f2f6d594b61554b395668567a45717574446f6f416e6664517464675a47654a627841703875623931653744332b387a7131784a534d740a2f5a665a7050514266394a3152504d4776774e4b2b73315435446c4339475273766a556f3245457075486542416f717454556754357679734d587a2b457a6e670a35447033755137456d4e6c6c49537072634651334f432f30513378416f6579667841634168416f705379303236762f434946727243705a7258305777674f4e410a77636b4e342f32355156716770666b622b4673585368576b75367776774b414a5352633351796679617a3348544a6f77344d6f4951674675545a7a73435741730a524f6c41476164735466385a76475167556b754967544e3836747944567a776661335941356f496e4367766d77387349446145642b4b32316d666a63623570370a614c4a35517531705a36597244346c6344784f305a6d7a6a4a5370733757346e34566a45414f3271426b4b3679622f61584b7a6a7236716441786f6f5334454d0a776962775061554b357a73726a5a2b7347393578334c796b346f353970327268704c675832705072637769414a725361372f48674e53596c444b724f4e4258730a677248396a45462b5a512f637531687172794d6574425337757338436b6f6c67784f63526c5261314f4a36657068523452374852314245362b4c574f495541360a7565707479696b52713165556d6665762f6b736f2b536e4a6b4a6f744f765666735839624e37374e616f753955766d6b6865745343684761506d78384e2b58530a6641464e4c585a4e4c454e6665435865574a392b464e34594e6e39487a6a507a374a33704f2f794d4a4c6b434451525a35694a55415241417171545233312f630a546c754e5a4a64764d49486d527876374d32415a58616e35615276423150506a676d65696566766d4f46707268344a6631756d737131433756467369686463750a30644b6e48664d482b664478634754442f7251496436596f3962776b6f68566d4c345a4b76572b664c4a6852386838764757365a3353675873524b3654636f410a3748627374486e4d4e734d4b6851324a2f4242374e375a37736b39476666563046556e4463356170533051444d5779343868727178556f4b6c343548726663350a4132312b696f5a4b3873596745786b4b7064497079616f714e6b70447878324a4e6e304b7054654856366639614237426136686e39754f35773139376a5370360a757865366b315778706839336f564d335052366e555a31464263317345775a2f31526c5073336c47684c515562565873492f347168744c7970614e79773575530a71664378473452692f50464a5a6755455479456d5747664235764a634a48446770383137332f594c716361467841716d416f59573872444d2b756a717341424b0a5a565236785161676857744c53472b714b666f565a427872685631764b70556b32707678744979775359555a546c3362694b383539765a6a3459565a4e6455300a4d61724653765934745555687663696d697352493445754d2f7a4f42693944613031476c546e51313051364e5733795235624465533071415539414d4c6e6b410a6f49346e6d5554514a3050617a78447754502b55526c4b7672302f2f3773366a6a7657784e59736f497357354d6b59756850742b6346367061473051797643520a48686743694863774f6a5345366b4677787854364e534c4a71794778326f4d6a6c456e78395547455a42744a4d69475154334a6f3859334c2b464c597a5277460a5971566c5858486b75786146625a356a36613843582f3459454f37694c423266673263414551454141596b4350415159415167414a685968424b686638335a310a6e4a6c4b6968466f324e67686e4978443973586842514a5a35694a554168736742516b466f35714141416f4a454e67686e49784439735868506d4551414947770a50485157425033426c7872613747736f71314958545a3271676f762b465537744646333950734e505533357242786763356a49594e6c78635a717a394d6845590a6174365944334c535269752f664735585149326e304d6f6d414159482f494a4865386a4d53434458722b56383575336164552f47564b43464a7a6e314a766f420a51724e3242597573575a4f6f58714e2b79306d49677353524f33764644466c435564666b6f5963562b663846703073546a32454d6c452f6b67313779515470480a6c516d72755163417634763659497a6a4d52776753437776676571383879537672785766386361635a654e33506d6f45776a586c4135505145496834707747390a4568714653555653464c774b6c5352374a696f485262595a586f4d6452724473656f4373725849336f70782f6f324d7a562b306241384450614a53396a334e4a0a67744469642b4a342b3344356274587961646b6d716e3672397a63373545345441666b2f32707349576c736e697a455a67456a6f3947533031463466725945770a37596d74774a37556c744632715464612b78306d55723136723955613577382f66325134556d72706b74746f6c4d37622f79357467597067437a2f362f4172340a6876376254696f3336396b4e674549587a626c4e766662757363734c5855586b74596d5370667976736253314d454e746a61682f725a73664c546845696f507a0a7553625469756a766945326669456272682b42314471636d75555968794b57736146386c333470436770482f585a505378675832586a786a774656705478682b0a6347682b4a6158475231614f734e4949642b3046526843717342787248534b3742516149775a4647413253783262377636556a505551654746453739374c64690a617649584b6b654b48544171796142784d4a6c4d7869444575312b622b704d68784b394973504f6c0a3d65445a740a2d2d2d2d2d454e4420504750205055424c4943204b455920424c4f434b2d2d2d2d2d0a','A85FF376759C994A8A1168D8D8219C8C43F6C5E1','D8219C8C43F6C5E1','1602861827.0','1508253827.0',0,NULL);
+    can_primary_sign INTEGER,
+    oncard TEXT,
+    primary_on_card TEXT
+);
+INSERT INTO keys VALUES(1,X'2d2d2d2d2d424547494e205047502050524956415445204b455920424c4f434b2d2d2d2d2d0a0a78595945583432675178594a4b7759424241486152773842415164412f646b442b5337304453696e733853774c44747a6373366c594838674e444565774672610a2f4d2f36556d542b43514d4934354548476a76727263332f4f3258664158707054524a4f395155735952525165794a552f3038776c376b5254484e4a4b47314e0a66744a744b683335486d5864626946366e794368666434775979655972586f597278612f705a533058614b626342685355464a78574d4b4442423857436741310a42594a666a6142444177734a42776b51785374434633685833586b4446516f4941707342416834424669454539504f49753747556b6c726a41666845785374430a4633685833586b41414661394151442f4c7652354f76644972725179676d6b5138446a7a4878763045686634376530483230673576536a555a5145417a46554d0a5665342f567671545752504e6d4532695664747165436541373347654e576772694b443371777a4e476e526c6333516764584e6c636941386447567a6445426e0a625746706243356a6232302b776f59454578594b41446746676c2b4e6f454d4443776b48435244464b3049586546666465514d56436767436d5145436d7745430a486745574951543038346937735a535357754d422b4554464b304958654666646551414174394942414e5258324c5875476468793530644b2f447566736d56360a334d39562b644965595a614f33444c537a54634a415039493169656b4e736d6e794353576753326758696a50363236372b366a774775466f5744654a5067524d0a4273654742462b4e6f454d574353734741515142326b635041514548514c43565a6d556b2b6e41786377614a687039436363386669793647353735585a4e727a0a6a4b625975632b452f676b4443506f536e5150516e536a482f316d66783177617537426d69792f2f754e4a51774e707736444a4a4a4a6a45456e4a54736370690a2f5774503248752b41634e4f5a4255424e5a72634844575842434244544e31312f46364747535869516e76626d43765537334c4b6a6d5843774449454742594b0a414b5146676c2b4e6f454d4a454d557251686434563931354170734341683442647141454752594b41436346676c2b4e6f454d4a454e2f5278566b6d5a4930760a4669454545433639493731644c5451507539344b3339484657535a6b6a53384141436938415030526e47326e51675a7547516f38756347617554784f746861740a4432632b4176645030644f746b6153313867442f6164614b6a54494657485863644a44377173542f7a42522b63656c784c33344c7a4241614a655033364163570a4951543038346937735a535357754d422b4554464b3049586546666465514141732b6f424150334a6c45356a6c6d65364e74486d5a5a2b4636436e416b744a4b0a6c384c6c335a6f2b534730736f6e4d6e4151444e69477149594f697637596930734544677451306e69682f7571735472476c704c3146764b6a7136644173654c0a42462b4e6f454d5343697347415151426c315542425145424230412f3468656f4b2b4d596f49624d577a4273726e434b356938432f6a6f68383767704235482f0a4a52745345514d4243416e2b43514d49364e6c39474f396e382f332f4a2f756454484561486f44364a534456485441684b514e617355596a754e5a57454146550a567149374e3147455573716e62636d355545716a4a7154436a675239396564696f4947754b7731535258615342307972582b53467450716c44384a37424267570a4367417442594a666a614244435244464b3049586546666465514b6243414965415259684250547a694c75786c4a4a6134774834524d557251686434563931350a414141644451443843526e535639755175314c676e3165356539657850763435506777524c574b574269437a7644616943337742414f456a47386c61302b45430a4e63463442344570685667495a79563452644b4e33446a3367776578535649430a3d666275430a2d2d2d2d2d454e44205047502050524956415445204b455920424c4f434b2d2d2d2d2d0a','F4F388BBB194925AE301F844C52B42177857DD79','C52B42177857DD79','','1603117123.0',1,0,NULL,'');
+INSERT INTO keys VALUES(2,X'2d2d2d2d2d424547494e205047502050524956415445204b455920424c4f434b2d2d2d2d2d0a0a7863614742462b4e6f4c5942454144453056514f4b74763776635338497841616c384c594c4457343639485963585a564c3336534d552b4c2f545854356248450a5261414a3278495454657a356a5942727458342b7a2b34395a655a45435a314f5957354c314853686843414756784d4b50397774356a48483851415a483243690a65492f5967777a503631367735694571353254494b614b584859494b5a316c57493537425339622f457737696e437a62683452416b554b4169636b575056722b0a45446d573164713938505a4551783741654656706d354569774a5144414e716d6b456336794d376562444e5762504161324f3652516c67774c317a74374d32740a5a6c2b7066552b58466b6e62776d5559343534754a5656506a78517074466a6c6e353967446a3661505a2f48654477495864353052775a4f32413344586261430a487653766d434c63346a364d3856352f37787451423776542b6b74472b36536f48376a2b744e5847374774336159757030586e6938306a4b656e7a7250686b320a366479436568664e5a74744d7572765753664c435775574649317458377178487136344744786e494e33387a687970575a6e7550766869773550486b777756620a726e6a69447a2b522f6435704b6b5575574450484f6b4b734932794d4747704531442f737078646f48416c414f6a31495762324a5749414b396534523450382f0a67544f3556746c482b59384a2f526e577068696457716f32387739645654565a526a78674835676d4d71656e3636776d564845614e5578496761616f544556540a377634635976506d5a62733670326164715267456e52375151326841636a4241476b42365168776e62306b31544e6f447078523839642f6762755661417950580a57794a524f6f384e7273312f4838695a2b706f6c2f584137594a33466e64525679752f4f636f696f38443650684e7048506b506b5271475579774152415141420a2f676b44434b447864455a6e7a7862522f34707477685a69653242523335586d705238797853763870544f424446636f6b7477676d48316b362b483857464b6c0a4f3155325779434e5749627634566777792f3771644d462b4b793145544e364b426d68366f73685a6c693647737048795a3667357372436749565477393379710a386c5a697463457941673674554b765a3554505259394b70753352314f6e6645305a68584b387867745168714f76644848327433704a326a454e6d4c4f5a6b410a5948454245326d7039427a77463867556b433953526a4f6632794e7a734e452f4b6a6951476a37344f4f356579702f4e72643769796f352f304143595871324d0a774f315446655957684332386d31745a43494e2b6d76316b4930657a624f69763453446c32657638307267444c6a564278387a52676d646f4837666152484a540a744e646261777949783475723771716e77546a735a502f30454b676b39542b577373617a5942373935626c64564d7a4f57744b764d464b58305a346f4e3556530a794979376f736c7461594f78442f44647465314a6e3031474a32646f70616e544d6e754d2b50676d572f3243506b35497265717941486657484238733855684a0a5456654d627759414b36707075547163504a79575249424b6e6971394e6956674d5233594743715a4d576654593968794e4465753136746d3647502f366a45310a632f3572762b53796f4a64582f6d6f4c31513569644c515370446368514f396b65396b30476f53432b78304f6f786b2b72374a736b38655046794a31595076440a4f447565376673356d346e4a56717747395246473034574f2f575874733737486f324c3476516e6a436a3636464c7253617853716e4a754652393859613543790a4d47676d6a4b744c5859473042766d426c7a556856395645646e6262445249716c4734506f7a45546570775744744d55456262717a34673576696a4a6c3867390a36442f69524e4a6348665368392f703543527a31617a4e79544c4563725630333363344e4a6c654c3361497936672f437862424b447543566b6d6e626e77426e0a6a4b682b3173676e31316d505747333261565372744c75516c6b594c44756d5654634d75394a4d58562b514d715676376c79302b514973726b42662b6a68706d0a6544635579335562417370552b4648485a31736c6c555762592f4373675a62362b7478662b726538394944324464554e685a416c4d73595061796b486c7841710a695845545a626c4b475a416b49446541316771362b6a774974692b6444593470497a6f67335a44466a346d394c5a6d7a4c364a6f327852767142542b583163790a587349594b637064465a766b64707146424f54416967477247444f687156754165663065352f3466553671526a36415a522b45335330487849675875527a6f510a2b38393077364578515a3744687655454b546368424d544e734b596568774567657046524d307a6834486654373673456e396c434f32596a394c4262364758490a6d565458447037774d433158507338372f4b6b4f595a4f4f4847556a7875434941587a544e3033506e774954336277586a4d7676786178516474734533524d6f0a53766777654c4434614a4b37656750346a58567461306f50505a71643649467375434735416b576e324c4363663873682b7950546447777932366a636e5366360a4f6448415058317556454d7078345a574f7943375a31484f394c446d614154336f306442772f57514c4b5773626856514474677a732b6b61355131582f68444a0a38425a59527a3972506d4a3134483438304d72786d7156634875314e476c354f44772f3771347748557342354c4952365832495964714d664c67794339752f330a484776442b352f706f386161746433386e367843426c46546e41366f415532317959577633677974495343585a6b366873682f3839456d684d2b694c4f5054540a756a6d396c716b5a37735258414a7a65596938725042525459422f7661534a6e4d635753514a554241314a334d5844346b722f474e7435762f4c6358786c55450a53533279662f553959356f513549635a57583178686252612f2f4474546f5a3961636f374c33396f7533742b5434685578644e4463446e6d5a6d6a5638365a6f0a4263574a7a59394769455264413346437a3746627068655461336136713341513651524e3257307241796e6e77612f3055652b53764458727a515a396f33304a0a7a4c6c32426e52775954646e455647373770725a63643564674d506a3676596c556459524777454c4b6534725a355453727a675078396c37724659484a6457670a584373456f644b7645424d446b557957576c5748363758326b466d626e615136436f5a707170732b464d52414a384749322f517149786563462b3050354c44730a616763785053595747534468443931435778425732785879574b2b7463545a51326d4b372f4944326458756565776a313143797a394d4843775945454877454b0a41445546676c2b4e6f4c594443776b484352436878634e6b3631756149414d56436767436d77454348674557495154314844454f4174776264334868647469680a78634e6b3631756149414141314f6f51414b2b46713839726e52424246795244325850306736627659636358643635664f7750446e45707830584e46772f48630a692b5046642b6a65356f444d54657a47586f4b4b4d364259626e7135363274544654577751543259762b7a4d2f715370312f6c67616c46416175584c495841620a6548526951336a46537551675758764535464a2b6a354f4b30473448437770715a62734b4d4463753062722b306d456f52626970742f752f684457484d7158460a794a41754c366f4b7446546f6b754d763470517341744248355a36595756566c66526566742b37696a783454513672324e5a5254726249334364307579522b4a0a37352f6a3942364732372f5066527162676864362f586f4c3430666a456f383773466345325242346439386d563465776955367133725078346b7a7a483271660a6d4d365947724663534c626a483657787546717944313543356e6b345250796735766e52577756787969344b61576b694d6e655274356d7a504c69386a3150360a625362424f487a6f644c4e2b634d48447246795073715153583741427842464f5264434d3161504b504b596b333564756d454d6644736b61614b74504a524a760a4b61643073772b566b586b577670385061724f2b54396c754c6748704e54687a6f49435348754b464563734f4c4e6d7a645375484431374c3674627a332f2f740a5a694570686164555561472b3777463767327072374a444d686c3250426744464d4d68776249354452395a3856684b70373346596643325844666b39696855720a37787352794632644b6e7a4972356f45436656626d337678664e61416b307855586257743859706f776572494e7a7269326f6e45446652667635654b6365357a0a4a32677a6d424b47556e626b344d4a307979656c66386f636c546446316464636d344366327444714c7a7a7868705965443951764a7262595a4349797a5239550a5a584e304946567a5a584979494478795957356b623231415a586868625842735a53356a6232302b7773474542424d424367413442594a666a6143324177734a0a42776b516f6358445a4f74626d69414446516f4941706b424170734241683442466945453952777844674c6347336478345862596f6358445a4f74626d6941410a414e6c54442f396e4c702f4b576f7553784b4472366d75714938697759516b45502f4a64684e307769384e6a51543055364f5873387a342b616d645675722f4a0a4b3177416356506e742f62377145745a4d6a7466455331686d774248434a326d427667525a707472314e59346f4c4d683049737457432f612b77757736366e410a5a3343554970665669334f2b2f33436844543273444355634b5a6458714232344239675763485378746a3335483973694352593577323265636676444f6b52780a48552f7774743454585a5258305a4961426f2f54346257397876516d5257694f6661576e47326b5a30383139666476326c36314d67776851644f5445756c4c460a6b6f636678724d5732745a6c727a796e6b69497a623975387773415577714c303876396b466162574e6462504e71713444376b45436251666e65575850377a4d0a4668784769546e743978306c78336d666a706f6a75486754534c4f3356316a6f31446e67646572742b573839702f4f6962546e5848414c774c6e7239386a554c0a504a796736506469796375706f5050456470575a395450303265713377522b343770444d5a3844425a6778362b385874494e774736784b326b6e6248796d36470a55687431714b73694e724b2f4b79664163447469555637654a55356532512b4364507067707632694243354a58354d4e3841624844552b64644b386a4c5a656d0a715a4e747532525669554679526842556e37484c624f32667558564c73753544453274556b427a5a464155546b6b5272716d597079334a66687142536c4e302f0a47673548695378564549334f6b3463526a486d73714a5737553878337a71453144384246734a4e4d414675376250386a366c5252795858666333324f486b4a550a6f7176555a50623132374a6d71733237472f56364f36513565576d7a4d754f695861457a4944474f43423571624a4d6958636647686752666a614332415241410a716f422f714d446836652b6249412b4f7754616c6a4f515757647a4f594a684178656559564e6168524b57646e61476e7858766851637979692f4973793659760a335933674b4362496443343639376361654530476e4137497145654d54546a746869645a4537415a4e424c664a5157572f75765972692b557141576773704a4d0a655175447a667a79666e2b3746596e6d426f67727469546d4c744967486f692f6f59486a34314a50436368726e6876524369744d6132684954304c57675947790a4b6368565448414736464b78596d6a4b497662586653467753494b63497070694a2b365a546a6b6249564b6d67536c386a654942796e614c53394b746c6f42370a352f594a77707756415a4234646d76456c7557474e3939516a456c47355a2b374244563431623238326e524f51462b54517553614f586c48643771664f4162300a7458755a453170347a2f3766364771485479453365624f6d69685463396563676f6a42657a576c2b616a5070585155523066517859366a6c5730795653495a770a6a4a746a6e2f734c6e4657314c52314a4e57364254716d58644237714b6a6665656a6276586a577447454a656f2b5967614d55575563797930646e777935446d0a3246652f55555a476c4d546c32677671724f384c7652304177704d536e4f6d467958447235393475472f316f3461464d355044594d4665674e6d2b483435306e0a647a682f316b384f4e747868624a682f58364f587a784e3451773073644f4c5a736649485265435837554b74427963456154575278597a3642673250575537780a74506a6c716459686e58456233496d2b61354571734c477458666251595469747465494d46362b3768764f4235597275317235546c68446467767a31617073380a7650464945336d51492b697272596378666f706764347170684c555a466a782b525a4e347867667758616341455145414166344a4177696d77355166305a58760a5966387449533551544b784b3331616f385356325153342f4c6774445631326c3549562f4d4b74634a77687143795158486b4752494d76656f4443507767794e0a2b45716277366746767867546b32644f3150385a487a614e6f6e762f69766e4d2b30444b69365377337a64354c516971574f4c6e4e4f50445a33494c323342440a456e68347a624465625839327636764f56356177667a4172756d786c6f736642537668597a4162594f5830505558565278546d714e375144634b5641306a546b0a44306d486a6141526374617048417a374f724f4b776e63514a467959554d454176514d2b4b734b4456536d7553357558514e72726e6f357739746d4e6f5967540a327a6e35546578475563793059586847704d343742484b70324d3373584139677a3377782b2b2f57784d4963794649307339484e7a793853456455555a6b46580a4a554465777073387654304f4b4369504f62434a3666476a4f33656f51305450655966526b73334b6946766536526f7563477a46744e76797a55665550612b630a375a62492f627a4f34636d4166354858547858526463494f416d435262376d7a68634f74506e314844587476587056364f4d6643667059644f7467595055376e0a756333457867493634313975556a3039437570496f2b316e354e744f7869475173586c4a6a777735797a79554244755363323571426538384f6f46794b6f6e300a697053535175767649584731436146514e7848576c5842624276566f78362f63332b555339425a4e463739323135535664544e6974516a4164312b30346538780a775972425955413831593957477875503972686a646d48564d4531332b7a42356758635230504559704b627443694f424d385242415a696c72522b49456f69590a51482b4756524763317a634c654868492f386a624d32377949694f4c6831763966346546736d757854716e654355315a50314c534967526275596330423366560a697652425344764550414843664c72596c356e3243734e4376757a49597074457a374534415a33544c5366417947792f76494174743376696f6d6e47547143330a573663457a4b6e652b6e65564e704b78753130384d73616e44336859325a7a6677546847394c6432634c326847687a6c446762474b3134612f6b454e4e546c470a4257447170574d66644647627255394147323849793371536a4b635452684b666359494d38466e79423277655a686d736b59305a554c7846692b69764d3853320a69772b68416633394a4462747962716741342b304a5a524a42786148633266386b67445853795736303955345374486e396c2b74564d736a44356f777a386b570a45326241464747646678706c45634b366a61304934497251414966312b304c6e4e475a7971734b69576a376546433267365972697871674f78323477576632390a4b7457547858506739677853656271564930726d322f4c544a62375853314c6552305950465658747458726a734f456756437071472b3555416f4e77485067480a2f6e7754716e5162535a4d304a5664327365496d33335547794747755257586436544b59497835544f35667754355654624d6161366554596c58316a777750530a734f75627143454764735648724e7869495271553862576e4634623056655461655a2b7a4d304f70316351486d61776e675553764a51502f4f534c77446764390a796b3144696768646d5748775764514e77442f494734374b3976524f356d386f6b59317067704853423846484a6173576866657154756d7a69564c64502b58640a6c6f482b496c4242317641467444453153317634543952674948533476524173464e66447252366779464a513979316d515a524f32426f6a58744b7a387658420a4f484a56464952685857587a767835337252786a37525574434736626f64544b53322f3663626f78596678444e5653654a355177416f777163757a4a572f4a6e0a3467316b562b7a6c4d46694b57624b6543323838454475354349704f417a443238762b3144585a784a7278484b2f4c2f33786d65566264595471304d746e666f0a58305a366276476e487832343349762b6235356d31366e30504665774852326170327271685a642b674433533743642b39664f715730507956554839625268790a354d5968464156716553377773425a526948323730374d3574795566593247444859716c372f3068514c65565a374c4176493271557871383542573053766d450a494172683457396e74444b324443487031684d556942474a6d74453574355666486a303654336f554438534b59312b2b395662506a332f2b4c7272704b4c5a4b0a516a797a6b703865396465574536744443576b4c675a7557324f67303159627043546e3136555465696c6151764a5670316c6974376b7854714b4445746b69380a41614647487270646478565164336d4d48737752536d705a42317464797443365966434f7032737877734635424267424367417442594a666a614332435243680a78634e6b3631756149414b624341496541525968425055634d5134433342743363654632324b48467732547257356f67414144722b772f384467442b7265334a0a4448763268685944353971685a306870444f313369744b586b4241587774767273572b456571424a767564684f697a564e6e794947336266767349424355486a0a306a515a563241384c4939435a5556615953784842526c314876702f70726441624534543839447961515a6a2b4d796b755a412f302b753451714972554d62570a4d6559557061366a66754a44347273767245646336556b6372686c536a61356578466b39386f4d4747772b7a5276636f49746e6c6e4c494c6d77347a52316f6e0a566e565a4e557563616165617146687442465a746c4176687742364c62545579737530707a5167766c445949546b46462f6e4e494958364b763850743970656d0a42726a4677656862675463524461713058732b43655a706964787668334c37796c33767a667274374e6f714d58314167416b786d6174486254305558737441350a717672585058425a4a5a4c30666c48576978342f58347176506d593535335866446c466b6b704547706548515137766e48655147766a2f79616631754a347a4e0a5271684131307a732f6d4755364e753859737744674e77376556704d53687a7758736538646d523147424f72592b5a723073566649467564514f452b32592b700a4b2b342b6c4336634276684533776d33386162547865754d6a36334d69426562454f486b703137484c6c3166592b344a41326c324a4131627755746e41556c6e0a4770363469564e4143442f33454e57495034594664484761556b6d2f692f46307a6d2b68716c6f4a317334614953726958346a51624c4d3677564d43303033700a56774e556d47735a534c35793159644132524676795342736c7637474f67385a504a384556463636317745757634744a4a79572b426d554c4f787a6b395a2b6a0a354663734f676b6d7356314764474f554f505046487a422f78454673392b7868784c5048786f59455834326774674551414e424a336b6d316472396a34702f2f0a59317939704e69686a424757315569704671322f324a78584936624772364f6638502f676d487870307750494f686334535455646c776b6a686d36397268344a0a4d4c484e517974776266374f6259714f6a6a3339316874666c343346644c4f39504d67495650524231376d4e6378717a67713067706255684e68796e6558384b0a696e647163734278486777537044643679416f342f437a42594435537461336f39376a673143776f506f4754765176414638576173454b654c687453747a556d0a2f4f79666a656157645a446670566139465a7a707471476370706c31664152657a4c764d505542343259554b35707949317437786c725773717979756f3076670a4949653744766c2f5448654f63716b71576978456f714333593732797233684a2f694d637552742b496c356347656e47717a49463071415552325346797538790a3668354265762b4f657158557639664a69354c3930686730356f3432575a346a54556f32482b4a3278556657645348775862742f786a6d534c6a5a7a2f436e790a38685741505635497545447747766e4f3872795547762b7177357a706e44393649664f332f374a487130453037704a466b7575697333502f5a474253357147360a53446544362b33417a514f425949733270475855715a653034654b365a436d7450496635316478452b723348637859307559544a32574e7842357058634f74460a336f39312f465839446a3269535a574d52702b766c4b7752506d4b396254445431744a465a38536b306e6133456b79504e342f4779444d375838566c4d4439430a5761485357346174744265586d676b6d4534637772522b6951656679304b597834443566463765534f6f3273414f4b797343674c6f3079677935304c754f694a0a6f78322b725271364b71745a412f644a7a47327a556d47576c504d74414245424141482b43514d497833476a754172554834502f335a783559497369454452470a635871786775344b53476565575a54483352736c765a3034545577766771485a4979337937376e4665584f4568794f2b59347539356664435653427131685a6f0a77745979767368735659796d7476507578485478716c6d68774373516b61467170614b465667492b35726c31306b636961507473413367534f653665715654330a4d7366314346714538753637443631685859667270714744754f584e564f615a72734e2b77476e59424f4e614a586336625139553733736639314571433330350a58566e4d45313148574b54773056384c7a46494f463646454a547130374b644939766e3344496f4f636f436d636f71704e33457a4c4962514b62326c704f70530a392b6c4841326a62727838564575767669577a6d7a586c3133706a516a674c7477425032713937443046486b71432b746a4a6c787a4f4b546c737969464b33640a2f45774c51477758303159544343526f6444316d6e437074694557386f58765677456b794952364b4771385a557071633479654774395541794f4776755276410a3937317a4842594d4c56567a67564371764f4357714e492b364a43742b74594b4c56457758735a64515278313254777949555a422b7854564354396757795a5a0a34705174783231716a7761306b69765a333071587237514c57484d336477675331566f4f546f6c7452504e497552686a6a69507468476e7865624831373259470a626d666f375541755561305a73364b36496a556e50745945355666784d576d747666457158667441416d334c6f324a41527479476b4a7a453046776a323636610a72387157375751384b3044314474546434526e58505247525444654c717931494a387a7444724c59434471674c4648506d312f686d784e44334d6173624a65520a71793548594454395544394b506e5a372f67533371494a2f794269724f367946356b6b6250776936326c69696d614942353072782b6c4f6a41784636635542660a642f38334b482b636369334a6f686c2b6862422b54734a49787532526430796a622b75354335437568495737482f79656d67414374466c4143684550727632470a38636a754e7934746a677a357952677a342f674f7169365978457849576b366467766e4a59735a326c644d7a686d64365848476e334e49566b6e3949422b76680a6344575353376e4977736f3443662b4b47424a776959432b494a48416c555556412f2f3863677630756d554a553578722f6c68706a48766a4b74454e426f4c560a4669563970425555576e2f61496166562b502b4a4b72355371726a4f386c494735444943705239394a663938654b79657443726a6b61556d6a634879375039390a3855454155535662472b572f4f674f793856562f623250336d764b5062332b645a5a6e2f654f71466f645a43494f2b71697a4a566b6a364f78593930736d43660a524c6f6a73636e37542f504253374a7561794c4d7578416466596f555351417731544e6e316b4139497a315567374d334e33635a4a442b796a6b7441394562550a6d3778643764763754675057647358716b684339375745475353395a2b6a5741676f466f33596735756542483073614c615756564d6a7954735a35616f3756300a475633685776357051374a6f7234734f745553496e4c705046374a694f466e37397232426d6d4b3851684251726c42694b706e5274713649314f5061425649390a5051586b6a304e703873794266784c4e55507264335973317043494e7452676b59684c41564a73666147303652753549584c73736b70332b36396f52724e726f0a473165764152416f506d646539517238597576434b714b423776576936634d6344516a586b774c792b75615975786642514d645a4130746f4b634e4f315a67370a3272764c38774b3846426168375a4c38384f6643707a55556e49693666747659676c4931367262434e735461323678516c6b455531596d6649364432494234570a426f4330684559526959555432503375453058502b49557a4f454270526b71426d6865536d695141724c6477766e79394a766e4837386c6d786d645461674c490a6b394155632f4c2b7647517254346658364f557972427a7a65396e6f4e3945787962416573366b32783444384a504d4d564b707632776b4278567755435068660a755a6d324d7a774b384f79433464506335576a6a5a784a72676a4f4973497446454f7a624b6f5333362b505844684357555a314f69425471475a5a4e747a6b420a5375506139465337354566395563667678704c524258593154486e3433616551475a315a553254706b67356d657a462f6e356649684f33542b784871414673590a303171336c2b54697279487141735349516c7236366e6852397a5a6a5066776156674f4942616168344355694e6761545030544346376e557459744c707577330a68674b33477865556141546b616b447750564c5534373279784d4c447277515941516f43597757435834326774676b516f6358445a4f74626d6941436d7749430a48674842644b41454751454b41436346676c2b4e6f4c594a454133465a31677175514773466945455555506c6e70674973566f6e464473754463566e574371350a4161774141425864442f30597a73654d2f6753724f34466477633035616f5a3568464d5949746b666a5643725a6a6c4e5a48757867742b53507930716474654b0a7331477663757a6f2f4462467643743238535768322f722b6e5678324a4c70532f585251706543565a536a44446247314f42634171446f496b625642507851580a424d467543505946344b564b32764453694652674a704b39444f43786563334c6436516e786a5477495577736f427a425649494a6c6f497742545249373667390a57746a6875437758754d342b694d356e34547951727a77427247446b663241416776594f757a4e6d4966726f744a58543550332b37566e50446674794f4b5a500a5872513772526c4d55416737384d3943706a445330616d595750716c556b4e7166713877696c6554466c3957346e51746c4346375a6839494a786e554f43354a0a712b684949536c61374364695a4e316e397864496a625a425337685a44594f73756443613479643337384b796b53363239696c513252442f74714f516f495a340a614a6d527573377857763975766c76427a6d5534534e653238624365337a385570644352316a4268445a4c3061454d39454d7a465a75586e6d2f6c59376a79410a4a6d797244417861685a657567394c7952654a6e3734324b6171364e635a476349364a6934396c6e426a5a434f6832514764525a636442706b744c3339315a730a676161734c676b3476665231412f506e4d6c33344d68316c78444362377830764f7a61414149426837656963715a4f6967636a78743549326c4a644269376d720a635a4d7a544d4361675164783770745772544736796d4b537454355a397831454d2b564a594d552f37546278786330384152425a50526f6e32634c79542f34670a61716c6d34346f45723939496b5354525559386f527170494c496c6248357362774b454b5346676e774552722f6f7665544f457147785968425055634d5134430a3342743363654632324b48467732547257356f6741414241376841417736417232526452584f542f50636e627a6679646d5861676a6733474877725966664b380a517031596e6d43473948356b5a354a6d45626a5069564d752b776334537a6e3956794c4548432b797352517a453254696c63544f365157522b30686f526b2b640a6a6f4935544a444549384c57466a5a594730347a6568467869554d7a566d35526a4a364a584b5a496b626f41375a78694663555a314c3932754d4978532b4c6e0a4775704455644c2b67346536386959564e696e76445a684e6a75356a394262716c734c33564733343335536a39727435466250674164343665456156695a55790a4b35493551796264523457424e46326d6d4a5a6e7270554153683630494e36487372753352662b675342507531786b744d526f4648764947525637326254312f0a37434554344d303539326b78625a677637616b70477a3546477a52465a3335776e2b794b3463736d4e3931423832473761445368486b444751544a4e744842340a7271514d6f43557376426e464e694759515650327555467469394958386e346a6e586966425356436456306c686946776d434d69645a4a716837654e576842700a54386a4861736a72654356424b556f704d37716e31584a5977643153376b5673414e34384c5a692b53665876716e594446797a5649375141707449624d4261640a4a5748795953472f396a4d69493566745a415576483457734e6b346861785570726e632f4d36424833765a58506f4c4b706a387662557565533673356f4661780a765839666548377274584250524a4156786936557671494e4d63344278666b6e4776736c426844436c4d78613530502b677638665a71723856695038734744750a6771793378663954623941703665616e44463370675a664e782b78712b475732676343526a39686f413075736565686b565771366b31762f2b7a506b797a33690a6b7268736831343d0a3d364255590a2d2d2d2d2d454e44205047502050524956415445204b455920424c4f434b2d2d2d2d2d0a','F51C310E02DC1B7771E176D8A1C5C364EB5B9A20','A1C5C364EB5B9A20','','1603117238.0',1,0,NULL,'');
+INSERT INTO keys VALUES(3,X'2d2d2d2d2d424547494e20504750205055424c4943204b455920424c4f434b2d2d2d2d2d0a0a6d51494e42466e6d49494d424541444b636e41477469387959646e49396873372f31336a7331456c722f516b6b46415132547a513159383056564d454668684e0a6e697a7966387572783933707151336f2b2b77455841414c5a504a72764230546534436b6f58776233562f39386a79707749366b4841696d45323833754f656d0a4c4467516f6f42435158316b464b6b584b74765548416372634e76335769734379523632786c666d496e4a64735358736370766a454a4c464a5a5a637a504e330a62563076626665487267575a414d37756371463474724a725373524b787337723773357767774f36383846354e45514c7064743061544c4c2f304f4c305054320a47464a6861466831614649533268793652586f5548627856557969474d336850516236303731566c69476e426a7174696e31777337455866387163514445344a0a737869454f677544314f78586246794e6d39306f456d6263674749665844664a774e59385a2f4444394b746b747957744e594a31416630526c51374c672f36420a6c717a31626133316d744965557a6b6537414237644d58326a434f6263656d45725435486a6b56534336764e677947464f6556466e583162314f7570495a4c340a4454615a7131797775596e6c5873657972494d7754542b674d612b554f6c30462f7764775931524544556b4a31636d42582f75514839755354496a51725a56370a754445726e4f7941394c766568717a47366963746a313771726e5553304c4178506f6139475a786643363439366c4966645a68497336634b76592f4672714a390a6948543573306b7959554455574f472f523070733661425741766173445757675769494b3169354168706e415a4e46355167764871447a346d2b56452f6a59790a51586b446830426b75704a7277585835503079677a5642614b6a656a55625a4362374b6551366c7a4f77554e582b6c4c5a357a6c416b524773774152415141420a7443464c64584e6f595777675247467a4944787264584e6f595778415a6e4a6c5a57527662533577636d567a637a364a416c6345457745494145454347774d460a4351576a6d6f414643776b49427749474651674a43677343424259434177454348674543463441574951536f582f4e32645a795a536f6f52614e6a59495a794d0a512f624634515543576559686f41495a4151414b43524459495a794d512f62463464374745414357576f6e6d527658495a655050655273612f475a43567277780a554137335a466744783630674c306f32776179716859697743365475515061343234554c63694c5770465179346c62385977415a2b6d4d3979517a664d622f300a747642396377643675717a4e497a31514479483239754451724d386b4a6e454668757866496e592f574e6163513831364636616e4f6c545271316a4d65434b610a44375567747a596a5a2b3347546f32554a7168497059426d4c6d2b68324e63366d475a46567149706a7a7347522f64526a5a4b4e4639646c4d2f387a6d6448500a5a7244416b3953634747757a4f7752514468716d38345845737564504236374b6533584774303134595a62756b7146744a6e78614b2f33796763317a4a4c35510a614a4236786e79756c485542396775533556614454732b4234747334622b436a34506b674539497553307859434369545151642f314c58304b444853497477320a434c4c4b31714d476a584e65544557497153496d7a787a475273394a3537684157724c4e754a707665685564675879366c486d6751744e79744e455576536d440a3059466d6d2f74336a673755504f48634e4a614f4d765743547271796a55576438317670594b75315551514747366e6279792f364a6b58774641714c55536b510a545062636e3752546c4e6e363856672f304f4270776642564764484d6542425335544475394a6a6471776442746e70624446357a4336614d5777346b435946540a3532412b473869627079453266792f532b5a4359314a65574a77755746634f49686a7178482b634742657278552b69544c4d6e5a2f32473176356973776265770a6169567a4847614e6c4f5345552b2b59572f554255337858644d354d496e442f4d6f39576d6566723130694a6b624e2f644c713245394a30427a416a7650676d0a5757554439496f6b383532744777456c677251655333567a614746734945526863794138625746706245427264584e6f5957786b59584d756157342b69514a550a42424d424341412b4669454571462f7a646e57636d55714b45576a59324347636a45503278654546416c6e6d49554d4347774d464351576a6d6f414643776b490a427749474651674a436773434242594341774543486745434634414143676b51324347636a455032786548763542414170432f44646c3076457a4b664b3952770a793253494c4d534e326d4e3133375a756877306d674635512b42383556583258504947394f4751517143344156597635682b444b556c485332696448705838550a38344c5373476864304a66416863623758635538694a685045477a624c7579675633427267364556663065525042324d496c39346278767361417a36443454610a76494d2f4f3553716b7379675139644e6f6f472b79312b786b507378485a4c516c6c5131505a394a477531747666316c67677236765a41535974764e565430350a436d6667376b7a714f2b392b4f6e4b3641496d6355722b746e7837694743435976456d696369356563356f72785158344d3044714e2b75496b397632757544670a6858594a554a787537643670676632755432336b587439666442372b4c684e51737150453645556576472f516e693934397168374f4e434f6d716f72516f6f450a4f367253305a4859426b65532f796878546754472b644b357430362f2f7852596c34624a6f31574d30412b2b577235392f36353549734d65467833464e6638450a416d4d434d6b622f78424c66377345694443484a3531636e5a4156757332683969696f435a41664e59326852307539547634305066756575344139626f6a55700a7734467243513161356a4c4353304d763639346b54664733595730647555754c2b515761472f644d4957626f4c3331545175666346587676696d51472b5279420a73376436426166384270787a50464d706766356d33623930326149397748306b326434383038564170384b372b6c7353565a4a374773757673596258507948360a673579555a625368554654457859373469644547476374566e625963695952586947697745554f5445395742695932576476504d4f636643453347347848494a0a45444e516c464f5a7a7a53656c4c4353464f547553753750756c4b3049457431633268686243424559584d675047743163326868624752686330426e625746700a6243356a6232302b69514a5542424d424341412b4669454571462f7a646e57636d55714b45576a59324347636a45503278654546416c6e6d49566b4347774d460a4351576a6d6f414643776b49427749474651674a436773434242594341774543486745434634414143676b51324347636a4550327865455a71672f2f576e56450a55757643646c3164397331674d4355574c6a5645626f6a41645a5755614638724d6d33586d4136446a55394c4a4c4f57424c5273734e41327764506d707436690a43625a4f4b41683563436b457054376c42427967553244677342394e6a4c656543517474574b736d53656c546c644b3932414e706149496355523437344c32750a38563742373642596b774b3773417a38426f374e36344d4d6a384b4754386f4e6d6570697844412f61684e4c6d4d6339525654483832647945535675567261620a79387255365844474264662b494879597266754d696e7039725255316f4c6b2b444e592b7a4743584646377646455451336e335476414954557361654a694d4c0a6e6144795a4e74743269423674654d3173512f41573175747179396f49514c45434c4c4b785a495a5866304c6e495043336356424b3478456667516758647a540a6f76465155447448416f4d6e6b5065427978614c7770786c69565854737268302f49736751676244594b6b426b506c34776a35504971665250374b2b55712f590a792b72374a434a6b75777a4e556a6f4134446458614b682b7543595976776a46674335444258427570333758596a44676237384a4358774d632b527a2f454e450a4a7a326d6a6c676f432b3134644256614b38614b39444454486349725031655664333348654c34676d573267446f446d7652314d646a3443343853417a4153640a6c48454850415035324d755479766a774a446d58716a79567936634e486a6653587461775958575a724a50482b4e543359765277727767797a5a457a3477616b0a78516448384f7449416f5a313344744d5863767264745944635a556c6d6550566b6e564b794777326f784b4473764d6e33346a4e6d3452336e33506f71426f2b0a623972385835787567492f636e417a4c5a546c756d526c56566f56334b34446972615173503875304a557431633268686243424559584d6750477431633268680a6245426d5a575276636d4677636d39715a574e304c6d39795a7a364a416c514545774549414434574951536f582f4e32645a795a536f6f52614e6a59495a794d0a512f624634515543576559686b7749624177554a42614f616741554c435167484167595643416b4b437749454667494441514965415149586741414b435244590a495a794d512f62463452524d454143764b514c374e706e4a463950654867726d684a69566c4a576d46764c70624e486a753161622b50535a6d6551494f5437470a543849496d2b5355464e7a782b79795a64746a63427a746969335575684866374a47396a6b3553635038656f3059764b6733517647687a4d4f77707a347041490a445370675447697364505a2f537163774675337349716951314a566a54494e7a51704b37577253536456446c5154454f485a54416650735044644369686964740a7975722f6937554b41422b584b32716f346939346948702f3547656e3966494261724b62766b4c533168596c746371494a6643694c2b4453516b3073394643300a7941363751702b54626d685964582b70416d50576b776f512f71763269624b77543269584b7a432b6d58494c4a4b4b335a4e496267792b6a583072344f6950440a695356716d773356617a6d65594f31326979685046526652574c3433354b69464c792b4e523665554a4e6567346f64336452754156387a366b7a6b77396337660a782f6c354a326935466c2f5879474a77526d50576e544830666c78484d2f654332794c7050684c656e34754f496c76554e692b645235393473365174304b6d4e0a4b63555a3176744a432b592b626c4261626a3156597046306f51736342723148776b4a6543354c79325a3264776a73454e575568506b576a536b6b39777077530a366c646a357a7331635a2f3378686a2b385a705a74486d67305547796437736479616a36516949776b7a52736b4547724148357656582b52732f6c535173344f0a4c4a5943374f624e32785a6a7041343545724f5443363331716f7877417542424f4477394d5344353275315937446d6f6b2f534c44544171585a596874726c610a32446477644767786f3257326554304c633732384c4566584b6a6a46395a516457446e39545154716e3950397a586936586a31495350595662726b434451525a0a3569482f4152414173566b7a513545302f6f4b5945486c665945382b43424568656d31374466696c7957466971326979526c494f354b6e7853464f6845316a2b0a6631773077514f68704b2f6131655173626669584a415777736b6974656f685a58557652446d61474c39787a374e6f4458526d742b33646134594d78454a412b0a3270656358533245596952463768376965544d446c4a555971334c423977316d373042365457694b624b3677324c36672f417737574c553865797458387541590a72314b4b714a7a52777450785654706253537574374e55564f36684476695a7a70556c64623153586e6579685036324559424a42757a693956437174374c36650a476865417a43434b6c6b514b6e6566756d64726249726b46347253565933504d5136717454485179646e6e2b77646159452f4d43536a44424a635330542f664d0a7474456b3068714e4a504b7035546a637233574345482b5a3946753850744473666c346659577631767153505248563551706d68327a52464d7744456253504d0a6350687345356d4e705a4c74796d4230413362494b665a4177683178585470527a5254665445517745304469364c4270552b7a3831676c5666386e4d4870666b0a4b6635314e674e736e574b692b3774544331697a48303576536c4268706149754b6166394d62466b683141536e38306a7059466379457748656552416e6456650a5138784f5a6c7a786264774c4431796e6563517357684834387131434176506e2b596b373630496c554d6332376530613579664a3873516f794d7148544c43430a37575a6353746e5246597957622b7863596e655354643857486e79664e6c484343667867476b6c44674a7a44594a43342f625876615270572b6d57346534544d0a71677938686161755734696150736a7245506b367358687346466c37794f597272576479776e774e753065516e6a714f467673414551454141596b45636751590a415167414a685968424b686638335a316e4a6c4b6968466f324e67686e4978443973586842514a5a3569482f4168734342516b466f357141416b414a454e67680a6e497844397358687758516742426b42434141644669454543384531456c36792f356f50694f3463786c2f77423864585a753046416c6e6d4966384143676b510a786c2f77423864585a7532686c6841416d503745524d5771784c66426b61665143586636336957694a355037414f306e6e5152596a52534948317264747436500a727042413958783176756a357645683268754d76346e3730612b4d346c533452456c4443672f6e447a6c4872466b50422f36534f347a456148397946444b4c410a71714d7863386649476b62762f5230526f6b516d6271774b59414a646e536e6b7a64333350515650342b47423545553868667074316337643854473631632b480a7339317573734d414b4637454247622b38735a48394a797a46765a2f30364c4e484a6b3172546f75394d4b3277505a33676f7739567a633861754544734d51700a5455324953796c48614c417064493642726b74632f753636514c463247496f4275365044485675776f70647852345339544730727a344b78376149642b3935770a783057695a7a4e43635835524a615842596a32416931514b644a437a6c484c6e42367737413348554f5471422f79657646567a506f516f69794f54373637434e0a4b3875427934647131714c6f596336664e524e6f427930574f3457756f31726f7877534d5a3048764447477956452b64524973655754584245675236685430660a625658535771557479574665612b6e546f5a783868495a4635514d54357441373975436c56654e3443544b6a7a5032786f684b7150324772782f6279466d6f590a2b2b4c412b6e552f79397075424d5a4b4c4135456f52614c384d6a5742776570667577584d2b5a6836507767787963427a7a78637543767a544d516f42686a550a615a7a556e61413544384e6b4a6b4e63426e2f6467347467653735575776747a32316b2f36515a44686f41425948464a344b745442582f356557566c49642b6b0a4444484e5043737350364b4b6c5956737142597365556a4e70506644537836486a484e7536794a523255326f726c4a314170367a4e62713962434e2f43412f370a426c576d59334266756f2f43424b503673694e614c36547955576464493352776349326e6c4b643775757167647643575a3668426777507345773845655844760a696b41333371432f58775632384b3331383056674c337754656f4a754230786c6878585a38583866564a447964484968444c487832523377556f3068644a716b0a6d556449324354375576364a796f32524833474d563145506e584d317038726735424370516d492b6556645734594c737572535252474c7a2b59524e395879700a704e6d364f715a64766b4a7a5a546f477970354f5a4835737339556e6b4d584968485768332f737648375279397042485a765155536272774b63624b68766c480a485242744e4541456a49733631664e437867714469625a4d452b5748525171754f5a575357596d7563546a374c6c5a33446b5837574f36584565357649564f780a76466f5851614e31555a396f766d53443652766d6c34624b6c657635326133547761706769614c523276436577506a626634417a7741736b59316b35652b35580a43677645593378306a74796c38684a507741334630775676526d786d453262644e7834652f4473396c3435646f75756f32596a654739505144324241517549410a32306d6a4b78346d784d6f646b7479794934757a476c634b57795772504478716753487a323856305a4d41747754586e416a4a51644b6e396d687358782f4e610a36796a5863697045747339363343376c72682f51686a493845395243414350455146562b30302b4e4f327956326a355a7548695479687666564b764c6b30577a0a2f334d77502f6d6b73517a6e5054316632586175554c694f794679684f70346d3752525967696b4c497570337a5176522b6a494955746d4458366b752b772b6b0a377a67622b52596661567a6f48392f6a5935666b5a6235526d69454a39595037504452663732354e5367613541673045576559694a774551414a786e4d32522f0a6f6c54613447456148422f42356b594679654359684751526b306e73616d38356845434263696561434c4273715433357349624254393269446b5137763074750a4e783456575435617462382b755a74543535413949716d4d6b4c64456130795931707550586642515164365a65534f37586431366b776f4c2f68757a43356e690a456f41575164637237476b346d6a30752b337063477961473730516847386659356d506b7463786c38725a536641395566454853534330566f6c394c585069460a58513854786a3978553665316d5377515056574e36644e30733645564e57656a68364b704c53456f5845506e706872326f5158614a50454e4872707136446a740a6e6a4b614455416e32582f2f6d723030587553627335542b4247617a385a705738713037327355534f6d64623236346642766f2b4f562b4a554353434b30632f0a5235356452466d6d67556a2b576c435566666730454f355a784667704c66564d69614330522f7a3559623652753279774d682f34336f5477596b4348506a5a440a5a506a5362325a50766b6568782b794c7362434756332f503539555a757353327a7034375535374538736255624f3168345641493375725a3676786e7a6256730a4533515648306f763957774b4c6653736856546d534378557759584d4b6b5841334c474f5a496941426e424c6e592b775a4e4a6e493439763447754f566333770a3868635870566b3659702f527377474e477542786a2f4e7453755a2b4f4f2b524a45565643344e6644454f30726478624b79646c4c68772b424d4b756c65662b0a6c70556f314f61764c396738794d796f34503271433152356b50776a7344724b2f504a686d612b366269377969317438675a70373179757167623664383230700a5364714f32356d50584a65444c2b484e43473846426b5663786148655269736a564c4378414245424141474a416a774547414549414359574951536f582f4e320a645a795a536f6f52614e6a59495a794d512f624634515543576559694a7749624441554a42614f616741414b43524459495a794d512f624634556f42454143490a356e42537a6658537a542b6b4d6b667a45564a35354e5736774b7166442f48736f6f574d5237355631613074734a3349766f6f49344a6b7736554c6d585032780a4555477168536352644f2f6d594b61554b395668567a45717574446f6f416e6664517464675a47654a627841703875623931653744332b387a7131784a534d740a2f5a665a7050514266394a3152504d4776774e4b2b73315435446c4339475273766a556f3245457075486542416f717454556754357679734d587a2b457a6e670a35447033755137456d4e6c6c49537072634651334f432f30513378416f6579667841634168416f705379303236762f434946727243705a7258305777674f4e410a77636b4e342f32355156716770666b622b4673585368576b75367776774b414a5352633351796679617a3348544a6f77344d6f4951674675545a7a73435741730a524f6c41476164735466385a76475167556b754967544e3836747944567a776661335941356f496e4367766d77387349446145642b4b32316d666a63623570370a614c4a35517531705a36597244346c6344784f305a6d7a6a4a5370733757346e34566a45414f3271426b4b3679622f61584b7a6a7236716441786f6f5334454d0a776962775061554b357a73726a5a2b7347393578334c796b346f353970327268704c675832705072637769414a725361372f48674e53596c444b724f4e4258730a677248396a45462b5a512f637531687172794d6574425337757338436b6f6c67784f63526c5261314f4a36657068523452374852314245362b4c574f495541360a7565707479696b52713165556d6665762f6b736f2b536e4a6b4a6f744f765666735839624e37374e616f753955766d6b6865745343684761506d78384e2b58530a6641464e4c585a4e4c454e6665435865574a392b464e34594e6e39487a6a507a374a33704f2f794d4a4c6b434451525a35694a55415241417171545233312f630a546c754e5a4a64764d49486d527876374d32415a58616e35615276423150506a676d65696566766d4f46707268344a6631756d737131433756467369686463750a30644b6e48664d482b664478634754442f7251496436596f3962776b6f68566d4c345a4b76572b664c4a6852386838764757365a3353675873524b3654636f410a3748627374486e4d4e734d4b6851324a2f4242374e375a37736b39476666563046556e4463356170533051444d5779343868727178556f4b6c343548726663350a4132312b696f5a4b3873596745786b4b7064497079616f714e6b70447878324a4e6e304b7054654856366639614237426136686e39754f35773139376a5370360a757865366b315778706839336f564d335052366e555a31464263317345775a2f31526c5073336c47684c515562565873492f347168744c7970614e79773575530a71664378473452692f50464a5a6755455479456d5747664235764a634a48446770383137332f594c716361467841716d416f59573872444d2b756a717341424b0a5a565236785161676857744c53472b714b666f565a427872685631764b70556b32707678744979775359555a546c3362694b383539765a6a3459565a4e6455300a4d61724653765934745555687663696d697352493445754d2f7a4f42693944613031476c546e51313051364e5733795235624465533071415539414d4c6e6b410a6f49346e6d5554514a3050617a78447754502b55526c4b7672302f2f3773366a6a7657784e59736f497357354d6b59756850742b6346367061473051797643520a48686743694863774f6a5345366b4677787854364e534c4a71794778326f4d6a6c456e78395547455a42744a4d69475154334a6f3859334c2b464c597a5277460a5971566c5858486b75786146625a356a36613843582f3459454f37694c423266673263414551454141596b4350415159415167414a685968424b686638335a310a6e4a6c4b6968466f324e67686e4978443973586842514a5a35694a554168736742516b466f35714141416f4a454e67686e49784439735868506d4551414947770a50485157425033426c7872613747736f71314958545a3271676f762b465537744646333950734e505533357242786763356a49594e6c78635a717a394d6845590a6174365944334c535269752f664735585149326e304d6f6d414159482f494a4865386a4d53434458722b56383575336164552f47564b43464a7a6e314a766f420a51724e3242597573575a4f6f58714e2b79306d49677353524f33764644466c435564666b6f5963562b663846703073546a32454d6c452f6b67313779515470480a6c516d72755163417634763659497a6a4d52776753437776676571383879537672785766386361635a654e33506d6f45776a586c4135505145496834707747390a4568714653555653464c774b6c5352374a696f485262595a586f4d6452724473656f4373725849336f70782f6f324d7a562b306241384450614a53396a334e4a0a67744469642b4a342b3344356274587961646b6d716e3672397a63373545345441666b2f32707349576c736e697a455a67456a6f3947533031463466725945770a37596d74774a37556c744632715464612b78306d55723136723955613577382f66325134556d72706b74746f6c4d37622f79357467597067437a2f362f4172340a6876376254696f3336396b4e674549587a626c4e766662757363734c5855586b74596d5370667976736253314d454e746a61682f725a73664c546845696f507a0a7553625469756a766945326669456272682b42314471636d75555968794b57736146386c333470436770482f585a505378675832586a786a774656705478682b0a6347682b4a6158475231614f734e4949642b3046526843717342787248534b3742516149775a4647413253783262377636556a505551654746453739374c64690a617649584b6b654b48544171796142784d4a6c4d7869444575312b622b704d68784b394973504f6c0a3d65445a740a2d2d2d2d2d454e4420504750205055424c4943204b455920424c4f434b2d2d2d2d2d0a','A85FF376759C994A8A1168D8D8219C8C43F6C5E1','D8219C8C43F6C5E1','1602861827.0','1508253827.0',0,1,NULL,'');
 CREATE TABLE subkeys (
 	id INTEGER PRIMARY KEY,
 	key_id INTEGER,
 	fingerprint TEXT NOT NULL,
 	keyid TEXT NOT NULL,
 	expiration TEXT,
 	creation TEXT,
@@ -32,25 +34,56 @@
 INSERT INTO subkeys VALUES(4,2,'5143E59E9808B15A27143B2E0DC567582AB901AC','0DC567582AB901AC','','1603117238.0','signing',0);
 INSERT INTO subkeys VALUES(5,3,'D2BAF6212E4CDE548C330C3DFB82AA5D326DA75D','FB82AA5D326DA75D','1602862247.0','1508254247.0','encryption',0);
 INSERT INTO subkeys VALUES(6,3,'621B1339CDB831479A4DEB4F7C90F2749E085E1D','7C90F2749E085E1D','1602862292.0','1508254292.0','authentication',0);
 INSERT INTO subkeys VALUES(7,3,'0BC135125EB2FF9A0F88EE1CC65FF007C75766ED','C65FF007C75766ED','1602862207.0','1508254207.0','signing',0);
 CREATE TABLE uidvalues (
 	id INTEGER PRIMARY KEY,
 	value TEXT,
+	revoked INTEGER,
 	key_id INTEGER,
 	FOREIGN KEY (key_id)
 	REFERENCES keys (id)
 		ON DELETE CASCADE
 );
-INSERT INTO uidvalues VALUES(1,'test user <test@gmail.com>',1);
-INSERT INTO uidvalues VALUES(2,'Test User2 <random@example.com>',2);
-INSERT INTO uidvalues VALUES(3,'Kushal Das <kushal@fedoraproject.org>',3);
-INSERT INTO uidvalues VALUES(4,'Kushal Das <kushal@freedom.press>',3);
-INSERT INTO uidvalues VALUES(5,'Kushal Das <kushaldas@gmail.com>',3);
-INSERT INTO uidvalues VALUES(6,'Kushal Das <mail@kushaldas.in>',3);
+INSERT INTO uidvalues VALUES(1,'test user <test@gmail.com>',0,1);
+INSERT INTO uidvalues VALUES(2,'Test User2 <random@example.com>',0,2);
+INSERT INTO uidvalues VALUES(3,'Kushal Das <kushal@fedoraproject.org>',0,3);
+INSERT INTO uidvalues VALUES(4,'Kushal Das <kushal@freedom.press>',0,3);
+INSERT INTO uidvalues VALUES(5,'Kushal Das <kushaldas@gmail.com>',0,3);
+INSERT INTO uidvalues VALUES(6,'Kushal Das <mail@kushaldas.in>',0,3);
+CREATE TABLE uidcerts (
+	id INTEGER PRIMARY KEY,
+    ctype TEXT NOT NULL,
+	creation TEXT,
+	key_id INTEGER,
+	value_id INTEGER,
+	FOREIGN KEY (key_id)
+	REFERENCES keys (id)
+		ON DELETE CASCADE
+	FOREIGN KEY (value_id)
+	REFERENCES uidvalues (id)
+		ON DELETE CASCADE
+);
+CREATE TABLE uidcertlist (
+	id INTEGER PRIMARY KEY,
+	value TEXT,
+	datatype TEXT,
+	key_id INTEGER,
+	value_id INTEGER,
+	cert_id INTEGER,
+	FOREIGN KEY (key_id)
+	REFERENCES keys (id)
+		ON DELETE CASCADE
+	FOREIGN KEY (value_id)
+	REFERENCES uidvalues (id)
+		ON DELETE CASCADE
+	FOREIGN KEY (cert_id)
+	REFERENCES uidcerts (id)
+		ON DELETE CASCADE
+);
 CREATE TABLE uidemails (
 	id INTEGER PRIMARY KEY,
 	value TEXT,
 	key_id INTEGER,
 	value_id INTEGER,
 	FOREIGN KEY (key_id)
 	REFERENCES keys (id)
@@ -91,8 +124,10 @@
 	FOREIGN KEY (key_id)
 	REFERENCES keys (id)
 		ON DELETE CASCADE
 	FOREIGN KEY (value_id)
 	REFERENCES uidvalues (id)
 		ON DELETE CASCADE
 );
+CREATE TABLE dbupgrade (upgradedate TEXT);
+INSERT INTO dbupgrade VALUES('20220828');
 COMMIT;
```

### Comparing `johnnycanencrypt-0.8.0/tests/files/store/pgp_keys.asc` & `johnnycanencrypt-0.9.0/tests/files/store/pgp_keys.asc`

 * *Files identical despite different names*

### Comparing `johnnycanencrypt-0.8.0/tests/files/store/public.asc` & `johnnycanencrypt-0.9.0/tests/files/store/public.asc`

 * *Files identical despite different names*

### Comparing `johnnycanencrypt-0.8.0/tests/files/store/secret.asc` & `johnnycanencrypt-0.9.0/tests/files/store/secret.asc`

 * *Files identical despite different names*

### Comparing `johnnycanencrypt-0.8.0/tests/files/test_fetch_key_by_email.yml` & `johnnycanencrypt-0.9.0/tests/files/test_fetch_key_by_email.yml`

 * *Files identical despite different names*

### Comparing `johnnycanencrypt-0.8.0/tests/files/test_fetch_key_by_fingerprint.yml` & `johnnycanencrypt-0.9.0/tests/files/test_fetch_key_by_fingerprint.yml`

 * *Files identical despite different names*

### Comparing `johnnycanencrypt-0.8.0/tests/files/test_fetch_nonexistingkey_by_email.yml` & `johnnycanencrypt-0.9.0/tests/files/test_fetch_nonexistingkey_by_email.yml`

 * *Files identical despite different names*

### Comparing `johnnycanencrypt-0.8.0/tests/files/test_fetch_nonexistingkey_by_fingerprint.yml` & `johnnycanencrypt-0.9.0/tests/files/test_fetch_nonexistingkey_by_fingerprint.yml`

 * *Files identical despite different names*

### Comparing `johnnycanencrypt-0.8.0/tests/files/test_journalist_key.pub` & `johnnycanencrypt-0.9.0/tests/files/test_journalist_key.pub`

 * *Files identical despite different names*

### Comparing `johnnycanencrypt-0.8.0/tests/test_encrypt_decrypt.py` & `johnnycanencrypt-0.9.0/tests/test_encrypt_decrypt.py`

 * *Files identical despite different names*

### Comparing `johnnycanencrypt-0.8.0/tests/test_keystore.py` & `johnnycanencrypt-0.9.0/tests/test_keystore.py`

 * *Files 3% similar despite different names*

```diff
@@ -34,19 +34,27 @@
 
 
 def test_no_such_key():
     with pytest.raises(jce.KeyNotFoundError):
         ks = jce.KeyStore("tests/files/store")
         key = ks.get_key("A4F388BBB194925AE301F844C52B42177857DD79")
 
+
 def test_create_primary_key_with_encryption():
     ks = jce.KeyStore(tmpdirname.name)
-    newkey = ks.create_key("redhat", "test key42 <42@example.com>", jce.Cipher.RSA4k, whichkeys=1, can_primary_sign=True)
+    newkey = ks.create_key(
+        "redhat",
+        "test key42 <42@example.com>",
+        jce.Cipher.RSA4k,
+        whichkeys=1,
+        can_primary_sign=True,
+    )
     assert newkey.can_primary_sign == True
 
+
 def test_keystore_lifecycle():
     # Before anything let us first delete if any existing db
     pathname = os.path.join(tmpdirname.name, "jce.db")
     if os.path.exists(pathname):
         os.remove(pathname)
     # Now create a fresh db
     ks = jce.KeyStore(tmpdirname.name)
@@ -318,14 +326,51 @@
     key = "F51C310E02DC1B7771E176D8A1C5C364EB5B9A20"
     file_to_be_signed = os.path.join(tempdir.name, "text.txt")
     signed = ks.sign_file_detached(key, file_to_be_signed, "redhat", write=True)
     assert signed.startswith("-----BEGIN PGP SIGNATURE-----\n")
     assert ks.verify_file_detached(key, file_to_be_signed, file_to_be_signed + ".asc")
 
 
+def test_ks_userid_signing():
+    pathname = os.path.join(tmpdirname.name, "jce.db")
+    if os.path.exists(pathname):
+        os.remove(pathname)
+    # Now create a fresh db
+    ks = jce.KeyStore(tmpdirname.name)
+    k = ks.import_key("tests/files/store/pgp_keys.asc")
+    t2 = ks.import_key("tests/files/store/secret.asc")
+
+    # now let us sign the keys in kushal's uids
+    k = ks.certify_key(
+        t2,
+        k,
+        ["Kushal Das <kushaldas@gmail.com>", "Kushal Das <kushal@fedoraproject.org>"],
+        jce.SignatureType.PersonaCertification,
+        password="redhat".encode("utf-8"),
+    )
+    # k now contains the new updated key
+    for uid in k.uids:
+        if (
+            uid["value"] == "Kushal Das <kushaldas@gmail.com>"
+            or uid["value"] == "Kushal Das <kushal@fedoraproject.org>"
+        ):
+            certs = uid["certifications"]
+            # Only the new certification
+            assert len(certs) == 1
+            cert = certs[0]
+            assert cert["certification_type"] == "persona"
+            for data in cert["certification_list"]:
+                if data[0] == "fingerprint":
+                    assert data[1] == "F4F388BBB194925AE301F844C52B42177857DD79"
+                if data[0] == "keyid":
+                    assert data[1] == "C52B42177857DD79"
+        else:
+            assert len(uid["certifications"]) == 0
+
+
 def test_ks_creation_expiration_time():
     """
     Tests via Kushal's key and a new key
     """
     # These two are known values from kushal
     etime = datetime.datetime(2020, 10, 16, 20, 53, 47)
     ctime = datetime.datetime(2017, 10, 17, 20, 53, 47)
@@ -516,14 +561,15 @@
     # First we will check if this db schema is old or not
     with con:
         cursor = con.cursor()
         sql = "SELECT * from dbupgrade"
         cursor.execute(sql)
         fromdb = cursor.fetchone()
         assert fromdb["upgradedate"] == jce.DB_UPGRADE_DATE
+    # TODO: Now verify the keys inside of the new db, in full.
 
 
 def test_ks_upgrade_failure():
     "tests db upgrade failure from an old db because of existing file"
     tempdir = tempfile.TemporaryDirectory()
     shutil.copy("tests/files/store/oldjce.db", os.path.join(tempdir.name, "jce.db"))
     shutil.copy(
```

### Comparing `johnnycanencrypt-0.8.0/tests/test_sign_verify_bytes.py` & `johnnycanencrypt-0.9.0/tests/test_sign_verify_bytes.py`

 * *Files identical despite different names*

### Comparing `johnnycanencrypt-0.8.0/tests/utils.py` & `johnnycanencrypt-0.9.0/tests/utils.py`

 * *Files identical despite different names*

### Comparing `johnnycanencrypt-0.8.0/PKG-INFO` & `johnnycanencrypt-0.9.0/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,37 +1,31 @@
 Metadata-Version: 2.1
 Name: johnnycanencrypt
-Version: 0.8.0
+Version: 0.9.0
+Author-email: Kushal Das <mail@kushaldas.in>
+Project-URL: Homepage, https://github.com/kushaldas/johnnycanencrypt
+Project-URL: Bug Tracker, https://github.com/kushaldas/johnnycanencrypt/issues
 Classifier: Development Status :: 4 - Beta
 Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
 Classifier: Programming Language :: Rust
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3 :: Only
-Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Topic :: Software Development :: Libraries
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
-Requires-Dist: httpx
-Summary: Python module for OpenPGP.
-Home-Page: https://johnnycanencrypt.readthedocs.io/en/latest/introduction.html
-Author: Kushal Das <mail@kushaldas.in>
-Author-email: Kushal Das <mail@kushaldas.in>
-Maintainer: Kushal Das
-Maintainer-email: mail@kushaldas.in
-Requires-Python: >=3.7
-Description-Content-Type: text/markdown; charset=UTF-8; variant=GFM
-Project-URL: Github, https://github.com/kushaldas/johnnycanencrypt
-Project-URL: Source Code, https://github.com/kushaldas/johnnycanencrypt
+Requires-Python: >=3.8
+Description-Content-Type: text/markdown
+License-File: LICENSE
 
 # Johnny can encrypt
 
-[![CircleCI branch](https://img.shields.io/circleci/project/github/kushaldas/johnnycanencrypt/master.svg)](https://circleci.com/gh/kushaldas/workflows/johnnycanencrypt/tree/master)
+[![CircleCI branch](https://img.shields.io/circleci/project/github/kushaldas/johnnycanencrypt/main.svg)](https://circleci.com/gh/kushaldas/workflows/johnnycanencrypt/tree/main)
 
 Johnnycanencrypt aka **jce** is a Python module written in Rust to do basic encryption and decryption, and detached signing operations.
 It uses amazing [sequoia-pgp](https://sequoia-pgp.org/) library for the actual OpenPGP operations.
 
 You can also use Yubikeys for the private key operations using this module.
 
 
@@ -41,33 +35,33 @@
 
 ### Build dependencies in Fedora
 
 ```
 sudo dnf install nettle clang clang-devel nettle-devel python3-devel pcsc-lite-devel
 ```
 
-### Build dependencies in Debian Buster
+### Build dependencies in Debian Bullseye
 
 ```
-sudo apt install -y python3-dev libnettle6 nettle-dev libhogweed4 python3-pip python3-venv clang libpcsclite-dev
+sudo apt install -y python3-dev libnettle8 nettle-dev libhogweed6 python3-pip python3-venv clang libpcsclite-dev libpcsclite1 libclang-9-dev
+
 ```
 
-Finally build the module using `maturin`.
 
 ```
 python3 -m venv .venv
 source .venv/bin/activate
 python3 -m pip install -r requirements-dev.txt
-maturin develop
+python setup.py develop
 ```
 
 For a release build use the following command.
 
 ```
-maturin build --release
+python setup.py bdist_wheel
 ```
 
 ## Introduction
 
 Please read the [Introduction](https://johnnycanencrypt.readthedocs.io/en/latest/introduction.html) documentation.
 
 ## API documentation
```

