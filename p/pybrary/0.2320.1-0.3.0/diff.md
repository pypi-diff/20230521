# Comparing `tmp/pybrary-0.2320.1.tar.gz` & `tmp/pybrary-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pybrary-0.2320.1.tar", last modified: Sun May 21 13:47:56 2023, max compression
+gzip compressed data, was "dist/pybrary-0.3.0.tar", last modified: Mon Aug 24 11:17:19 2020, max compression
```

## Comparing `pybrary-0.2320.1.tar` & `pybrary-0.3.0.tar`

### file list

```diff
@@ -1,33 +1,21 @@
-drwxr-xr-x   0 louis     (4444) louis     (4444)        0 2023-05-21 13:47:56.773561 pybrary-0.2320.1/
--rw-r--r--   0 louis     (4444) louis     (4444)     1090 2023-03-15 11:12:32.000000 pybrary-0.2320.1/LICENSE
--rw-r--r--   0 louis     (4444) louis     (4444)      777 2023-05-21 13:47:56.773561 pybrary-0.2320.1/PKG-INFO
--rw-r--r--   0 louis     (4444) louis     (4444)      128 2023-05-18 09:05:26.000000 pybrary-0.2320.1/README.md
-drwxr-xr-x   0 louis     (4444) louis     (4444)        0 2023-05-21 13:47:56.773561 pybrary-0.2320.1/pybrary/
--rw-r--r--   0 louis     (4444) louis     (4444)      245 2023-05-18 09:08:40.000000 pybrary-0.2320.1/pybrary/__init__.py
--rwxr-xr-x   0 louis     (4444) louis     (4444)      778 2023-03-15 11:12:32.000000 pybrary-0.2320.1/pybrary/ascii.py
--rw-r--r--   0 louis     (4444) louis     (4444)     9933 2023-03-15 11:12:32.000000 pybrary-0.2320.1/pybrary/command.py
--rw-r--r--   0 louis     (4444) louis     (4444)     1576 2023-03-15 11:12:32.000000 pybrary-0.2320.1/pybrary/commandparams.py
--rw-r--r--   0 louis     (4444) louis     (4444)      609 2023-03-15 11:12:32.000000 pybrary-0.2320.1/pybrary/commands.py
--rw-r--r--   0 louis     (4444) louis     (4444)      843 2023-03-15 11:12:32.000000 pybrary-0.2320.1/pybrary/config.py
--rw-r--r--   0 louis     (4444) louis     (4444)     1738 2023-03-15 11:12:32.000000 pybrary-0.2320.1/pybrary/contract.py
--rw-r--r--   0 louis     (4444) louis     (4444)      555 2023-03-15 11:12:32.000000 pybrary-0.2320.1/pybrary/fernet.py
--rw-r--r--   0 louis     (4444) louis     (4444)     1514 2023-05-19 07:57:43.000000 pybrary-0.2320.1/pybrary/files.py
--rw-r--r--   0 louis     (4444) louis     (4444)     1172 2023-03-15 11:12:32.000000 pybrary-0.2320.1/pybrary/func.py
--rwxr-xr-x   0 louis     (4444) louis     (4444)     1813 2023-03-15 11:12:32.000000 pybrary-0.2320.1/pybrary/html.py
--rw-r--r--   0 louis     (4444) louis     (4444)      498 2023-03-15 11:12:32.000000 pybrary-0.2320.1/pybrary/logger.py
--rw-r--r--   0 louis     (4444) louis     (4444)      672 2023-05-18 09:05:35.000000 pybrary-0.2320.1/pybrary/main.py
--rw-r--r--   0 louis     (4444) louis     (4444)      381 2023-03-15 11:12:32.000000 pybrary-0.2320.1/pybrary/modules.py
--rw-r--r--   0 louis     (4444) louis     (4444)     1681 2023-04-21 10:02:39.000000 pybrary-0.2320.1/pybrary/net.py
--rw-r--r--   0 louis     (4444) louis     (4444)     1336 2023-03-15 11:12:32.000000 pybrary-0.2320.1/pybrary/primes.py
--rw-r--r--   0 louis     (4444) louis     (4444)     1186 2023-04-21 10:02:39.000000 pybrary-0.2320.1/pybrary/shell.py
--rwxr-xr-x   0 louis     (4444) louis     (4444)     5747 2023-03-15 11:12:32.000000 pybrary-0.2320.1/pybrary/ssh.py
--rw-r--r--   0 louis     (4444) louis     (4444)     8364 2023-05-21 09:12:51.000000 pybrary-0.2320.1/pybrary/tracer.py
-drwxr-xr-x   0 louis     (4444) louis     (4444)        0 2023-05-21 13:47:56.773561 pybrary-0.2320.1/pybrary.egg-info/
--rw-r--r--   0 louis     (4444) louis     (4444)      777 2023-05-21 13:47:56.000000 pybrary-0.2320.1/pybrary.egg-info/PKG-INFO
--rw-r--r--   0 louis     (4444) louis     (4444)      562 2023-05-21 13:47:56.000000 pybrary-0.2320.1/pybrary.egg-info/SOURCES.txt
--rw-r--r--   0 louis     (4444) louis     (4444)        1 2023-05-21 13:47:56.000000 pybrary-0.2320.1/pybrary.egg-info/dependency_links.txt
--rw-r--r--   0 louis     (4444) louis     (4444)       46 2023-05-21 13:47:56.000000 pybrary-0.2320.1/pybrary.egg-info/entry_points.txt
--rw-r--r--   0 louis     (4444) louis     (4444)       13 2023-05-21 13:47:56.000000 pybrary-0.2320.1/pybrary.egg-info/requires.txt
--rw-r--r--   0 louis     (4444) louis     (4444)       13 2023-05-21 13:47:56.000000 pybrary-0.2320.1/pybrary.egg-info/top_level.txt
--rw-r--r--   0 louis     (4444) louis     (4444)      954 2023-05-19 09:53:27.000000 pybrary-0.2320.1/pyproject.toml
--rw-r--r--   0 louis     (4444) louis     (4444)       38 2023-05-21 13:47:56.773561 pybrary-0.2320.1/setup.cfg
+drwxr-xr-x   0 louis     (4444) louis     (4444)        0 2020-08-24 11:17:19.000000 pybrary-0.3.0/
+-rw-r--r--   0 louis     (4444) louis     (4444)     1000 2020-08-24 11:17:19.000000 pybrary-0.3.0/PKG-INFO
+-rw-r--r--   0 louis     (4444) louis     (4444)      245 2020-07-29 10:22:37.000000 pybrary-0.3.0/README.rst
+drwxr-xr-x   0 louis     (4444) louis     (4444)        0 2020-08-24 11:17:19.000000 pybrary-0.3.0/pybrary/
+-rw-r--r--   0 louis     (4444) louis     (4444)       22 2020-08-24 11:16:54.000000 pybrary-0.3.0/pybrary/__init__.py
+-rwxr-xr-x   0 louis     (4444) louis     (4444)      648 2020-08-24 11:16:54.000000 pybrary-0.3.0/pybrary/ascii.py
+-rw-r--r--   0 louis     (4444) louis     (4444)     1738 2020-07-29 10:24:22.000000 pybrary-0.3.0/pybrary/contract.py
+-rw-r--r--   0 louis     (4444) louis     (4444)     1068 2020-07-29 10:24:22.000000 pybrary-0.3.0/pybrary/func.py
+-rw-r--r--   0 louis     (4444) louis     (4444)      227 2020-08-24 11:16:54.000000 pybrary-0.3.0/pybrary/net.py
+drwxr-xr-x   0 louis     (4444) louis     (4444)        0 2020-08-24 11:17:19.000000 pybrary-0.3.0/pybrary.egg-info/
+-rw-r--r--   0 louis     (4444) louis     (4444)     1000 2020-08-24 11:17:19.000000 pybrary-0.3.0/pybrary.egg-info/PKG-INFO
+-rw-r--r--   0 louis     (4444) louis     (4444)      318 2020-08-24 11:17:19.000000 pybrary-0.3.0/pybrary.egg-info/SOURCES.txt
+-rw-r--r--   0 louis     (4444) louis     (4444)        1 2020-08-24 11:17:19.000000 pybrary-0.3.0/pybrary.egg-info/dependency_links.txt
+-rw-r--r--   0 louis     (4444) louis     (4444)        8 2020-08-24 11:17:19.000000 pybrary-0.3.0/pybrary.egg-info/top_level.txt
+-rw-r--r--   0 louis     (4444) louis     (4444)       80 2020-08-24 11:17:19.000000 pybrary-0.3.0/setup.cfg
+-rw-r--r--   0 louis     (4444) louis     (4444)      923 2020-07-29 10:22:37.000000 pybrary-0.3.0/setup.py
+drwxr-xr-x   0 louis     (4444) louis     (4444)        0 2020-08-24 11:17:19.000000 pybrary-0.3.0/test/
+-rw-r--r--   0 louis     (4444) louis     (4444)     1625 2020-08-19 08:33:34.000000 pybrary-0.3.0/test/test_contract.py
+-rw-r--r--   0 louis     (4444) louis     (4444)      675 2020-07-29 10:24:22.000000 pybrary-0.3.0/test/test_fqn.py
+-rw-r--r--   0 louis     (4444) louis     (4444)      653 2020-07-29 10:24:22.000000 pybrary-0.3.0/test/test_func.py
+-rw-r--r--   0 louis     (4444) louis     (4444)      313 2020-07-29 10:24:22.000000 pybrary-0.3.0/test/test_string.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive
+POSIX tar archive (GNU)
```

### Comparing `pybrary-0.2320.1/pybrary/ascii.py` & `pybrary-0.3.0/pybrary/ascii.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,24 +1,17 @@
-from functools import partial
 from re import compile as rec
+from functools import partial
 
 
 # remove ansi codes
 rm_ansi_codes = partial(rec(
-    r'\x1B\[([0-9]{1,3}(;[0-9]{1,2})?)?[mGKJH](\x0F)?'
+    r'\x1B\[([0-9]{1,3}(;[0-9]{1,2})?)?[mGK](\x0F)?'
 ).sub, '')
 
 
-# make valid name
-clean_name_re = partial(rec(r'\W').sub, '_')
-
-def clean_name(txt):
-    return clean_name_re(txt).strip('_')
-
-
 # Convert file permissions from str to oct
 def oct_mod(str_mod):
     assert len(str_mod)==9, f'bad mode : {str_mod} ({len(str_mod)})'
 
     def digit(str_bits):
         assert len(str_bits)==3, f'bad bits : {str_bits}'
         value = sum(
```

### Comparing `pybrary-0.2320.1/pybrary/commandparams.py` & `pybrary-0.3.0/pybrary/contract.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,61 +1,69 @@
-from pathlib import Path
+from warnings import warn
 
-from pybrary.command import Param, ValidationError
+from pybrary.func import caller
 
 
-class ParamInt(Param):
-    '''Int
-    '''
-    def verify(self, value):
-        try:
-            return int(value)
-        except Exception as x:
-            raise ValidationError(f'{value}') from x
+class ContractError(Exception):
+    ''' Contract Error '''
 
+class PreError(ContractError):
+    ''' Contract Pre Error '''
 
-class ParamPath(Param):
-    '''Path
-    '''
-    def __init__(self, *a, **k):
-        self.create = k.pop('create', False)
-        super().__init__(*a, **k)
+class ResultError(ContractError):
+    ''' Contract Result Error '''
 
+class PostError(ContractError):
+    ''' Contract Post Error '''
 
-class ParamFile(ParamPath):
-    '''File
-    '''
-    def verify(self, value):
-        try:
-            path = Path(value)
-        except Exception as x:
-            raise ValidationError(f'{value}') from x
-        if path.is_file():
-            return path
-        elif self.create:
-            try:
-                path.open('x')
-            except Exception as x:
-                raise ValidationError(f'{value}') from x
-        else:
-            raise ValidationError(f'"{self.name}" File not found : {value}')
 
+class Contract:
+    def __init__(self, main):
+        self.main = main
+        self.name = self.__class__.__name__
+        self.func = f'{main.__module__}.{main.__name__}'
+
+    def warn(self):
+        warn(f'\n\n ? "{caller()}" not defined for Contract "{self.name}"\n')
 
-class ParamDir(ParamPath):
-    '''Dir
-    '''
-    def verify(self, value):
+    def pre(self, *a, **k):
+        self.warn()
+
+    def alt(self, *a, **k):
+        self.warn()
+        return 'no_alt'
+
+    def _run(self, *a, **k):
+        r = self.main(*a, **k)
+        x = self.alt(*a, **k)
+        if x!='no_alt':
+            aa = ', '.join(map(str, a)) if a else ''
+            kk = ', '+str(k) if k else ''
+            assert r == x, f'{self.name} results mismatch {self.func}({aa}{kk}) returned {r} expected {x}'
+        return r
+
+    def post(self, result, *a, **k):
+        self.warn()
+
+    def __call__(self, *a, **k):
         try:
-            path = Path(value)
+            self.pre(*a, **k)
         except Exception as x:
-            raise ValidationError(f'\n{value}') from x
-        if path.is_dir():
-            return path
-        elif self.create:
+            raise PreError(f'\n\n ! {x} !')
+        else:
             try:
-                path.mkdir(parents=True)
+                r = self._run(*a, **k)
             except Exception as x:
-                raise ValidationError(f'{value}') from x
-        elif path.exists():
-            raise ValidationError(f'"{self.name}" : {value} is not a dir')
-        else:
-            raise ValidationError(f'"{self.name}" dir not found : {value}')
+                raise ResultError(f'\n\n ! {x} !')
+            else:
+                try:
+                    self.post(r, *a, **k)
+                except Exception as x:
+                    raise PostError(f'\n\n ! {x} !')
+                else:
+                    return r
+
+
+def contract(cls):
+    def deco(fct):
+        return cls(fct) if __debug__ else fct
+    return deco
```

