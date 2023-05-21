# Comparing `tmp/cuvec-2.8.0.tar.gz` & `tmp/cuvec-2.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cuvec-2.8.0.tar", last modified: Mon Nov  1 21:54:26 2021, max compression
+gzip compressed data, was "cuvec-2.9.0.tar", last modified: Mon Nov 22 22:28:10 2021, max compression
```

## Comparing `cuvec-2.8.0.tar` & `cuvec-2.9.0.tar`

### file list

```diff
@@ -1,49 +1,49 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-11-01 21:54:26.762180 cuvec-2.8.0/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-11-01 21:54:26.754180 cuvec-2.8.0/.github/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-11-01 21:54:26.758180 cuvec-2.8.0/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (121)     2059 2021-11-01 21:54:10.000000 cuvec-2.8.0/.github/workflows/comment-bot.yml
--rw-r--r--   0 runner    (1001) docker     (121)     5138 2021-11-01 21:54:10.000000 cuvec-2.8.0/.github/workflows/test.yml
--rw-r--r--   0 runner    (1001) docker     (121)      224 2021-11-01 21:54:10.000000 cuvec-2.8.0/.gitignore
--rw-r--r--   0 runner    (1001) docker     (121)     1533 2021-11-01 21:54:10.000000 cuvec-2.8.0/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (121)      326 2021-11-01 21:54:10.000000 cuvec-2.8.0/.zenodo.json
--rw-r--r--   0 runner    (1001) docker     (121)      563 2021-11-01 21:54:10.000000 cuvec-2.8.0/CONTRIBUTING.md
--rw-r--r--   0 runner    (1001) docker     (121)    16488 2021-11-01 21:54:10.000000 cuvec-2.8.0/LICENCE
--rw-r--r--   0 runner    (1001) docker     (121)     5809 2021-11-01 21:54:26.762180 cuvec-2.8.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     4227 2021-11-01 21:54:10.000000 cuvec-2.8.0/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-11-01 21:54:26.758180 cuvec-2.8.0/cuvec/
--rw-r--r--   0 runner    (1001) docker     (121)     5381 2021-11-01 21:54:10.000000 cuvec-2.8.0/cuvec/CMakeLists.txt
--rw-r--r--   0 runner    (1001) docker     (121)      438 2021-11-01 21:54:10.000000 cuvec-2.8.0/cuvec/Config.cmake.in
--rw-r--r--   0 runner    (1001) docker     (121)     1279 2021-11-01 21:54:10.000000 cuvec-2.8.0/cuvec/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-11-01 21:54:26.758180 cuvec-2.8.0/cuvec/include/
--rw-r--r--   0 runner    (1001) docker     (121)     3223 2021-11-01 21:54:10.000000 cuvec-2.8.0/cuvec/include/cuvec.cuh
--rw-r--r--   0 runner    (1001) docker     (121)      285 2021-11-01 21:54:10.000000 cuvec-2.8.0/cuvec/include/cuvec.i
--rw-r--r--   0 runner    (1001) docker     (121)    10784 2021-11-01 21:54:10.000000 cuvec-2.8.0/cuvec/include/pycuvec.cuh
--rw-r--r--   0 runner    (1001) docker     (121)     4312 2021-11-01 21:54:10.000000 cuvec-2.8.0/cuvec/pycuvec.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-11-01 21:54:26.758180 cuvec-2.8.0/cuvec/src/
--rw-r--r--   0 runner    (1001) docker     (121)     2750 2021-11-01 21:54:10.000000 cuvec-2.8.0/cuvec/src/cuvec.cu
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-11-01 21:54:26.758180 cuvec-2.8.0/cuvec/src/example_mod/
--rw-r--r--   0 runner    (1001) docker     (121)     1140 2021-11-01 21:54:10.000000 cuvec-2.8.0/cuvec/src/example_mod/CMakeLists.txt
--rw-r--r--   0 runner    (1001) docker     (121)     3418 2021-11-01 21:54:10.000000 cuvec-2.8.0/cuvec/src/example_mod/example_mod.cu
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-11-01 21:54:26.758180 cuvec-2.8.0/cuvec/src/example_swig/
--rw-r--r--   0 runner    (1001) docker     (121)     1643 2021-11-01 21:54:10.000000 cuvec-2.8.0/cuvec/src/example_swig/CMakeLists.txt
--rw-r--r--   0 runner    (1001) docker     (121)     2272 2021-11-01 21:54:10.000000 cuvec-2.8.0/cuvec/src/example_swig/example_swig.cu
--rw-r--r--   0 runner    (1001) docker     (121)      494 2021-11-01 21:54:10.000000 cuvec-2.8.0/cuvec/src/example_swig/example_swig.i
--rw-r--r--   0 runner    (1001) docker     (121)     1526 2021-11-01 21:54:10.000000 cuvec-2.8.0/cuvec/src/swvec.i
--rw-r--r--   0 runner    (1001) docker     (121)     6873 2021-11-01 21:54:10.000000 cuvec-2.8.0/cuvec/swigcuvec.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-11-01 21:54:26.758180 cuvec-2.8.0/docs/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-11-01 21:54:26.754180 cuvec-2.8.0/docs/custom_theme/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-11-01 21:54:26.762180 cuvec-2.8.0/docs/custom_theme/js/
--rw-r--r--   0 runner    (1001) docker     (121)      517 2021-11-01 21:54:10.000000 cuvec-2.8.0/docs/custom_theme/js/extra.js
--rw-r--r--   0 runner    (1001) docker     (121)    14856 2021-11-01 21:54:10.000000 cuvec-2.8.0/docs/index.md
--rw-r--r--   0 runner    (1001) docker     (121)      744 2021-11-01 21:54:10.000000 cuvec-2.8.0/docs/licence.md
--rw-r--r--   0 runner    (1001) docker     (121)     2449 2021-11-01 21:54:10.000000 cuvec-2.8.0/docs/pydoc-markdown.yml
--rw-r--r--   0 runner    (1001) docker     (121)      138 2021-11-01 21:54:10.000000 cuvec-2.8.0/docs/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (121)      283 2021-11-01 21:54:10.000000 cuvec-2.8.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (121)     2403 2021-11-01 21:54:10.000000 cuvec-2.8.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)     1452 2021-11-01 21:54:10.000000 cuvec-2.8.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-11-01 21:54:26.762180 cuvec-2.8.0/tests/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2021-11-01 21:54:10.000000 cuvec-2.8.0/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      435 2021-11-01 21:54:10.000000 cuvec-2.8.0/tests/test_cuvec.py
--rw-r--r--   0 runner    (1001) docker     (121)     3425 2021-11-01 21:54:10.000000 cuvec-2.8.0/tests/test_perf.py
--rw-r--r--   0 runner    (1001) docker     (121)     4027 2021-11-01 21:54:10.000000 cuvec-2.8.0/tests/test_pycuvec.py
--rw-r--r--   0 runner    (1001) docker     (121)     4207 2021-11-01 21:54:10.000000 cuvec-2.8.0/tests/test_swigcuvec.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-11-22 22:28:10.211901 cuvec-2.9.0/
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-11-22 22:28:10.207901 cuvec-2.9.0/.github/
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-11-22 22:28:10.211901 cuvec-2.9.0/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (121)     2059 2021-11-22 22:27:54.000000 cuvec-2.9.0/.github/workflows/comment-bot.yml
+-rw-r--r--   0 runner    (1001) docker     (121)     5138 2021-11-22 22:27:54.000000 cuvec-2.9.0/.github/workflows/test.yml
+-rw-r--r--   0 runner    (1001) docker     (121)      224 2021-11-22 22:27:54.000000 cuvec-2.9.0/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (121)     1533 2021-11-22 22:27:54.000000 cuvec-2.9.0/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (121)      326 2021-11-22 22:27:54.000000 cuvec-2.9.0/.zenodo.json
+-rw-r--r--   0 runner    (1001) docker     (121)      563 2021-11-22 22:27:54.000000 cuvec-2.9.0/CONTRIBUTING.md
+-rw-r--r--   0 runner    (1001) docker     (121)    16488 2021-11-22 22:27:54.000000 cuvec-2.9.0/LICENCE
+-rw-r--r--   0 runner    (1001) docker     (121)     5809 2021-11-22 22:28:10.211901 cuvec-2.9.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (121)     4227 2021-11-22 22:27:54.000000 cuvec-2.9.0/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-11-22 22:28:10.211901 cuvec-2.9.0/cuvec/
+-rw-r--r--   0 runner    (1001) docker     (121)     5381 2021-11-22 22:27:54.000000 cuvec-2.9.0/cuvec/CMakeLists.txt
+-rw-r--r--   0 runner    (1001) docker     (121)      438 2021-11-22 22:27:54.000000 cuvec-2.9.0/cuvec/Config.cmake.in
+-rw-r--r--   0 runner    (1001) docker     (121)     1279 2021-11-22 22:27:54.000000 cuvec-2.9.0/cuvec/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-11-22 22:28:10.211901 cuvec-2.9.0/cuvec/include/
+-rw-r--r--   0 runner    (1001) docker     (121)     3223 2021-11-22 22:27:54.000000 cuvec-2.9.0/cuvec/include/cuvec.cuh
+-rw-r--r--   0 runner    (1001) docker     (121)      285 2021-11-22 22:27:54.000000 cuvec-2.9.0/cuvec/include/cuvec.i
+-rw-r--r--   0 runner    (1001) docker     (121)    12414 2021-11-22 22:27:54.000000 cuvec-2.9.0/cuvec/include/pycuvec.cuh
+-rw-r--r--   0 runner    (1001) docker     (121)     4312 2021-11-22 22:27:54.000000 cuvec-2.9.0/cuvec/pycuvec.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-11-22 22:28:10.211901 cuvec-2.9.0/cuvec/src/
+-rw-r--r--   0 runner    (1001) docker     (121)     2750 2021-11-22 22:27:54.000000 cuvec-2.9.0/cuvec/src/cuvec.cu
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-11-22 22:28:10.211901 cuvec-2.9.0/cuvec/src/example_mod/
+-rw-r--r--   0 runner    (1001) docker     (121)     1140 2021-11-22 22:27:54.000000 cuvec-2.9.0/cuvec/src/example_mod/CMakeLists.txt
+-rw-r--r--   0 runner    (1001) docker     (121)     3418 2021-11-22 22:27:54.000000 cuvec-2.9.0/cuvec/src/example_mod/example_mod.cu
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-11-22 22:28:10.211901 cuvec-2.9.0/cuvec/src/example_swig/
+-rw-r--r--   0 runner    (1001) docker     (121)     1643 2021-11-22 22:27:54.000000 cuvec-2.9.0/cuvec/src/example_swig/CMakeLists.txt
+-rw-r--r--   0 runner    (1001) docker     (121)     2272 2021-11-22 22:27:54.000000 cuvec-2.9.0/cuvec/src/example_swig/example_swig.cu
+-rw-r--r--   0 runner    (1001) docker     (121)      494 2021-11-22 22:27:54.000000 cuvec-2.9.0/cuvec/src/example_swig/example_swig.i
+-rw-r--r--   0 runner    (1001) docker     (121)     1526 2021-11-22 22:27:54.000000 cuvec-2.9.0/cuvec/src/swvec.i
+-rw-r--r--   0 runner    (1001) docker     (121)     6873 2021-11-22 22:27:54.000000 cuvec-2.9.0/cuvec/swigcuvec.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-11-22 22:28:10.211901 cuvec-2.9.0/docs/
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-11-22 22:28:10.207901 cuvec-2.9.0/docs/custom_theme/
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-11-22 22:28:10.211901 cuvec-2.9.0/docs/custom_theme/js/
+-rw-r--r--   0 runner    (1001) docker     (121)      517 2021-11-22 22:27:54.000000 cuvec-2.9.0/docs/custom_theme/js/extra.js
+-rw-r--r--   0 runner    (1001) docker     (121)    14856 2021-11-22 22:27:54.000000 cuvec-2.9.0/docs/index.md
+-rw-r--r--   0 runner    (1001) docker     (121)      744 2021-11-22 22:27:54.000000 cuvec-2.9.0/docs/licence.md
+-rw-r--r--   0 runner    (1001) docker     (121)     2449 2021-11-22 22:27:54.000000 cuvec-2.9.0/docs/pydoc-markdown.yml
+-rw-r--r--   0 runner    (1001) docker     (121)      138 2021-11-22 22:27:54.000000 cuvec-2.9.0/docs/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (121)      283 2021-11-22 22:27:54.000000 cuvec-2.9.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (121)     2403 2021-11-22 22:27:54.000000 cuvec-2.9.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (121)     1452 2021-11-22 22:27:54.000000 cuvec-2.9.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-11-22 22:28:10.211901 cuvec-2.9.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2021-11-22 22:27:54.000000 cuvec-2.9.0/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)      435 2021-11-22 22:27:54.000000 cuvec-2.9.0/tests/test_cuvec.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3425 2021-11-22 22:27:54.000000 cuvec-2.9.0/tests/test_perf.py
+-rw-r--r--   0 runner    (1001) docker     (121)     4440 2021-11-22 22:27:54.000000 cuvec-2.9.0/tests/test_pycuvec.py
+-rw-r--r--   0 runner    (1001) docker     (121)     4207 2021-11-22 22:27:54.000000 cuvec-2.9.0/tests/test_swigcuvec.py
```

### Comparing `cuvec-2.8.0/.github/workflows/comment-bot.yml` & `cuvec-2.9.0/.github/workflows/comment-bot.yml`

 * *Files identical despite different names*

### Comparing `cuvec-2.8.0/.github/workflows/test.yml` & `cuvec-2.9.0/.github/workflows/test.yml`

 * *Files identical despite different names*

### Comparing `cuvec-2.8.0/.pre-commit-config.yaml` & `cuvec-2.9.0/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `cuvec-2.8.0/CONTRIBUTING.md` & `cuvec-2.9.0/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `cuvec-2.8.0/LICENCE` & `cuvec-2.9.0/LICENCE`

 * *Files identical despite different names*

### Comparing `cuvec-2.8.0/PKG-INFO` & `cuvec-2.9.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cuvec
-Version: 2.8.0
+Version: 2.9.0
 Summary: Unifying Python/C++/CUDA memory: Python buffered array -> C++11 `std::vector` -> CUDA managed memory
 Home-page: https://github.com/AMYPAD/CuVec
 Author: Casper da Costa-Luis
 Author-email: casper.dcl@physics.org
 License: MPL 2.0
 Project-URL: Changelog, https://github.com/AMYPAD/CuVec/releases
 Project-URL: Documentation, https://amypad.github.io/CuVec
```

### Comparing `cuvec-2.8.0/README.rst` & `cuvec-2.9.0/README.rst`

 * *Files identical despite different names*

### Comparing `cuvec-2.8.0/cuvec/CMakeLists.txt` & `cuvec-2.9.0/cuvec/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `cuvec-2.8.0/cuvec/__init__.py` & `cuvec-2.9.0/cuvec/__init__.py`

 * *Files identical despite different names*

### Comparing `cuvec-2.8.0/cuvec/include/cuvec.cuh` & `cuvec-2.9.0/cuvec/include/cuvec.cuh`

 * *Files identical despite different names*

### Comparing `cuvec-2.8.0/cuvec/include/pycuvec.cuh` & `cuvec-2.9.0/cuvec/include/pycuvec.cuh`

 * *Files 13% similar despite different names*

```diff
@@ -25,36 +25,38 @@
 #include <sstream>   // std::stringstream
 #include <typeinfo>  // typeid
 #include <vector>    // std::vector
 
 namespace cuvec {
 template <typename T> struct PyType {
   static const char *format() { return typeid(T).name(); }
+  static const char *npchr() { return ""; }
 };
-#define _PYCVEC_TPCHR(T, typestr)                                                                 \
+#define _PYCUVEC_TPCHR(T, typestr, npy_char)                                                      \
   template <> struct PyType<T> {                                                                  \
     static const char *format() { return typestr; }                                               \
+    static const char *npchr() { return npy_char; }                                               \
   }
-_PYCVEC_TPCHR(char, "c");
-_PYCVEC_TPCHR(signed char, "b");
-_PYCVEC_TPCHR(unsigned char, "B");
+_PYCUVEC_TPCHR(char, "c", "S");
+_PYCUVEC_TPCHR(signed char, "b", "b");
+_PYCUVEC_TPCHR(unsigned char, "B", "B");
 #ifdef _Bool
-_PYCVEC_TPCHR(_Bool, "?");
+_PYCUVEC_TPCHR(_Bool, "?", "?");
 #endif
-_PYCVEC_TPCHR(short, "h");
-_PYCVEC_TPCHR(unsigned short, "H");
-_PYCVEC_TPCHR(int, "i");
-_PYCVEC_TPCHR(unsigned int, "I");
-_PYCVEC_TPCHR(long long, "q");
-_PYCVEC_TPCHR(unsigned long long, "Q");
+_PYCUVEC_TPCHR(short, "h", "h");
+_PYCUVEC_TPCHR(unsigned short, "H", "H");
+_PYCUVEC_TPCHR(int, "i", "i");
+_PYCUVEC_TPCHR(unsigned int, "I", "I");
+_PYCUVEC_TPCHR(long long, "q", "l");
+_PYCUVEC_TPCHR(unsigned long long, "Q", "L");
 #ifdef _CUVEC_HALF
-_PYCVEC_TPCHR(_CUVEC_HALF, "e");
+_PYCUVEC_TPCHR(_CUVEC_HALF, "e", "e");
 #endif
-_PYCVEC_TPCHR(float, "f");
-_PYCVEC_TPCHR(double, "d");
+_PYCUVEC_TPCHR(float, "f", "f");
+_PYCUVEC_TPCHR(double, "d", "d");
 } // namespace cuvec
 
 /** classes */
 /// class PyCuVec<T>
 template <class T> struct PyCuVec {
   PyObject_HEAD CuVec<T> vec; // PyObject_HEAD has an implicit `;` after it
   std::vector<Py_ssize_t> shape;
@@ -229,38 +231,75 @@
   self->strides = other->strides;
   return self;
 }
 /// returns `getattr(o, 'cuvec', o) or NULL` without altering refcount
 template <class T> PyCuVec<T> *asPyCuVec(PyObject *o) {
   if (!o || Py_None == o) return NULL;
   if (PyObject_HasAttrString(o, "cuvec")) {
+    // NumPy type checking
+    PyObject *dtype = PyObject_GetAttrString(o, "dtype");
+    PyObject *c = PyObject_GetAttrString(dtype, "char");
+    Py_XDECREF(dtype);
+    if (PyUnicode_Check(c)) {
+      char *npchr = (char *)PyUnicode_1BYTE_DATA(c);
+      if (*npchr != *cuvec::PyType<T>::npchr()) {
+        PyErr_Format(PyExc_TypeError,
+                     "cannot convert underlying dtype('%s') to requested dtype('%s')", npchr,
+                     cuvec::PyType<T>::npchr());
+        Py_DECREF(c);
+        return NULL;
+      }
+    }
+    Py_XDECREF(c);
+    // return cuvec
     o = PyObject_GetAttrString(o, "cuvec");
     if (!o) return NULL;
     Py_DECREF(o);
   }
   return (PyCuVec<T> *)o;
 }
 template <class T> PyCuVec<T> *asPyCuVec(PyCuVec<T> *o) {
   if (!o || Py_None == (PyObject *)o) return NULL;
   if (PyObject_HasAttrString((PyObject *)o, "cuvec")) {
+    // NumPy type checking
+    PyObject *dtype = PyObject_GetAttrString((PyObject *)o, "dtype");
+    PyObject *c = PyObject_GetAttrString(dtype, "char");
+    Py_XDECREF(dtype);
+    if (PyUnicode_Check(c)) {
+      char *npchr = (char *)PyUnicode_1BYTE_DATA(c);
+      if (*npchr != *cuvec::PyType<T>::npchr()) {
+        PyErr_Format(PyExc_TypeError,
+                     "cannot convert underlying dtype('%s') to requested dtype('%s')", npchr,
+                     cuvec::PyType<T>::npchr());
+        Py_DECREF(c);
+        return NULL;
+      }
+    }
+    Py_XDECREF(c);
+    // return cuvec
     o = (PyCuVec<T> *)PyObject_GetAttrString((PyObject *)o, "cuvec");
     if (!o) return NULL;
     Py_DECREF((PyObject *)o);
   }
   return o;
 }
 /// conversion functions for PyArg_Parse...(..., "O&", ...)
 #define ASCUVEC(T, typechar)                                                                      \
   int asPyCuVec_##typechar(PyObject *object, void **address) {                                    \
-    *address = (void *)asPyCuVec<T>(object);                                                      \
+    PyCuVec<T> *o = asPyCuVec<T>(object);                                                         \
+    if (!o) return 0;                                                                             \
+    *address = (void *)o;                                                                         \
     return 1;                                                                                     \
   }
 ASCUVEC(signed char, b)
 ASCUVEC(unsigned char, B)
 ASCUVEC(char, c)
+#ifdef _Bool
+ASCUVEC(_Bool, "?", "?");
+#endif
 ASCUVEC(short, h)
 ASCUVEC(unsigned short, H)
 ASCUVEC(int, i)
 ASCUVEC(unsigned int, I)
 ASCUVEC(long long, q)
 ASCUVEC(unsigned long long, Q)
 #ifdef _CUVEC_HALF
```

### Comparing `cuvec-2.8.0/cuvec/pycuvec.py` & `cuvec-2.9.0/cuvec/pycuvec.py`

 * *Files identical despite different names*

### Comparing `cuvec-2.8.0/cuvec/src/cuvec.cu` & `cuvec-2.9.0/cuvec/src/cuvec.cu`

 * *Files identical despite different names*

### Comparing `cuvec-2.8.0/cuvec/src/example_mod/CMakeLists.txt` & `cuvec-2.9.0/cuvec/src/example_mod/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `cuvec-2.8.0/cuvec/src/example_mod/example_mod.cu` & `cuvec-2.9.0/cuvec/src/example_mod/example_mod.cu`

 * *Files identical despite different names*

### Comparing `cuvec-2.8.0/cuvec/src/example_swig/CMakeLists.txt` & `cuvec-2.9.0/cuvec/src/example_swig/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `cuvec-2.8.0/cuvec/src/example_swig/example_swig.cu` & `cuvec-2.9.0/cuvec/src/example_swig/example_swig.cu`

 * *Files identical despite different names*

### Comparing `cuvec-2.8.0/cuvec/src/swvec.i` & `cuvec-2.9.0/cuvec/src/swvec.i`

 * *Files identical despite different names*

### Comparing `cuvec-2.8.0/cuvec/swigcuvec.py` & `cuvec-2.9.0/cuvec/swigcuvec.py`

 * *Files identical despite different names*

### Comparing `cuvec-2.8.0/docs/custom_theme/js/extra.js` & `cuvec-2.9.0/docs/custom_theme/js/extra.js`

 * *Files identical despite different names*

### Comparing `cuvec-2.8.0/docs/index.md` & `cuvec-2.9.0/docs/index.md`

 * *Files identical despite different names*

### Comparing `cuvec-2.8.0/docs/licence.md` & `cuvec-2.9.0/docs/licence.md`

 * *Files identical despite different names*

### Comparing `cuvec-2.8.0/docs/pydoc-markdown.yml` & `cuvec-2.9.0/docs/pydoc-markdown.yml`

 * *Files identical despite different names*

### Comparing `cuvec-2.8.0/setup.cfg` & `cuvec-2.9.0/setup.cfg`

 * *Files identical despite different names*

### Comparing `cuvec-2.8.0/setup.py` & `cuvec-2.9.0/setup.py`

 * *Files identical despite different names*

### Comparing `cuvec-2.8.0/tests/test_perf.py` & `cuvec-2.9.0/tests/test_perf.py`

 * *Files identical despite different names*

### Comparing `cuvec-2.8.0/tests/test_pycuvec.py` & `cuvec-2.9.0/tests/test_pycuvec.py`

 * *Files 13% similar despite different names*

```diff
@@ -146,7 +146,20 @@
     from cuvec.example_mod import increment2d_f
     a = cu.zeros((1337, 42), 'f')
     assert (a == 0).all()
     res = cu.asarray(increment2d_f(a, a))
     assert (a == 1).all()
     del a
     assert (res == 1).all()
+
+
+def test_np_types():
+    from cuvec.example_mod import increment2d_f
+    f = cu.zeros((1337, 42), 'f')
+    d = cu.zeros((1337, 42), 'd')
+    cu.asarray(increment2d_f(f))
+    cu.asarray(increment2d_f(f, f))
+    with raises(TypeError):
+        cu.asarray(increment2d_f(d))
+    with raises(SystemError):
+        # the TypeError is suppressed since a new output is generated
+        cu.asarray(increment2d_f(f, d))
```

### Comparing `cuvec-2.8.0/tests/test_swigcuvec.py` & `cuvec-2.9.0/tests/test_swigcuvec.py`

 * *Files identical despite different names*

