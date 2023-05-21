# Comparing `tmp/pytest-django-ifactory-0.5.0.tar.gz` & `tmp/pytest-django-ifactory-1.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pytest-django-ifactory-0.5.0.tar", last modified: Wed Feb  9 12:32:40 2022, max compression
+gzip compressed data, was "pytest-django-ifactory-1.0.0.tar", last modified: Sun May 21 17:37:31 2023, max compression
```

## Comparing `pytest-django-ifactory-0.5.0.tar` & `pytest-django-ifactory-1.0.0.tar`

### file list

```diff
@@ -1,42 +1,42 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-02-09 12:32:40.949349 pytest-django-ifactory-0.5.0/
--rw-rw-rw-   0 root         (0) root         (0)     2323 2022-02-09 12:32:35.000000 pytest-django-ifactory-0.5.0/.gitlab-ci.yml
--rw-rw-rw-   0 root         (0) root         (0)      583 2022-02-09 12:32:35.000000 pytest-django-ifactory-0.5.0/.pre-commit-config.yaml
--rw-rw-rw-   0 root         (0) root         (0)      867 2022-02-09 12:32:35.000000 pytest-django-ifactory-0.5.0/CHANGES.md
--rw-rw-rw-   0 root         (0) root         (0)     1517 2022-02-09 12:32:35.000000 pytest-django-ifactory-0.5.0/LICENSE
--rw-rw-rw-   0 root         (0) root         (0)      216 2022-02-09 12:32:35.000000 pytest-django-ifactory-0.5.0/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     7107 2022-02-09 12:32:40.949349 pytest-django-ifactory-0.5.0/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)     6230 2022-02-09 12:32:35.000000 pytest-django-ifactory-0.5.0/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-02-09 12:32:40.946348 pytest-django-ifactory-0.5.0/docker/
--rw-rw-rw-   0 root         (0) root         (0)      200 2022-02-09 12:32:35.000000 pytest-django-ifactory-0.5.0/docker/Dockerfile
--rwxrwxrwx   0 root         (0) root         (0)      279 2022-02-09 12:32:35.000000 pytest-django-ifactory-0.5.0/docker/push.sh
--rw-rw-rw-   0 root         (0) root         (0)      133 2022-02-09 12:32:35.000000 pytest-django-ifactory-0.5.0/pyproject.toml
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-02-09 12:32:40.947348 pytest-django-ifactory-0.5.0/pytest_django_ifactory/
--rw-rw-rw-   0 root         (0) root         (0)      251 2022-02-09 12:32:35.000000 pytest-django-ifactory-0.5.0/pytest_django_ifactory/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     4629 2022-02-09 12:32:35.000000 pytest-django-ifactory-0.5.0/pytest_django_ifactory/defaults.py
--rw-rw-rw-   0 root         (0) root         (0)     6015 2022-02-09 12:32:35.000000 pytest-django-ifactory-0.5.0/pytest_django_ifactory/ifactory.py
--rw-rw-rw-   0 root         (0) root         (0)      763 2022-02-09 12:32:35.000000 pytest-django-ifactory-0.5.0/pytest_django_ifactory/plugin.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-02-09 12:32:40.948348 pytest-django-ifactory-0.5.0/pytest_django_ifactory.egg-info/
--rw-r--r--   0 root         (0) root         (0)     7107 2022-02-09 12:32:40.000000 pytest-django-ifactory-0.5.0/pytest_django_ifactory.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      891 2022-02-09 12:32:40.000000 pytest-django-ifactory-0.5.0/pytest_django_ifactory.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2022-02-09 12:32:40.000000 pytest-django-ifactory-0.5.0/pytest_django_ifactory.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       60 2022-02-09 12:32:40.000000 pytest-django-ifactory-0.5.0/pytest_django_ifactory.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)       14 2022-02-09 12:32:40.000000 pytest-django-ifactory-0.5.0/pytest_django_ifactory.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       23 2022-02-09 12:32:40.000000 pytest-django-ifactory-0.5.0/pytest_django_ifactory.egg-info/top_level.txt
--rw-rw-rw-   0 root         (0) root         (0)      185 2022-02-09 12:32:35.000000 pytest-django-ifactory-0.5.0/requirements.txt
--rw-rw-rw-   0 root         (0) root         (0)      167 2022-02-09 12:32:40.950348 pytest-django-ifactory-0.5.0/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)     1274 2022-02-09 12:32:35.000000 pytest-django-ifactory-0.5.0/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-02-09 12:32:40.948348 pytest-django-ifactory-0.5.0/tests/
--rw-rw-rw-   0 root         (0) root         (0)      790 2022-02-09 12:32:35.000000 pytest-django-ifactory-0.5.0/tests/conftest.py
--rw-rw-rw-   0 root         (0) root         (0)      697 2022-02-09 12:32:35.000000 pytest-django-ifactory-0.5.0/tests/djangosettings.py
--rw-rw-rw-   0 root         (0) root         (0)     7643 2022-02-09 12:32:35.000000 pytest-django-ifactory-0.5.0/tests/test_defaults.py
--rw-rw-rw-   0 root         (0) root         (0)     4104 2022-02-09 12:32:35.000000 pytest-django-ifactory-0.5.0/tests/test_ifactory.py
--rw-rw-rw-   0 root         (0) root         (0)     1436 2022-02-09 12:32:35.000000 pytest-django-ifactory-0.5.0/tests/test_plugin.py
--rw-rw-rw-   0 root         (0) root         (0)     1616 2022-02-09 12:32:35.000000 pytest-django-ifactory-0.5.0/tests/test_readme_examples.py
--rw-rw-rw-   0 root         (0) root         (0)      176 2022-02-09 12:32:35.000000 pytest-django-ifactory-0.5.0/tests/test_toplevel.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-02-09 12:32:40.949349 pytest-django-ifactory-0.5.0/tests/testapp/
--rw-rw-rw-   0 root         (0) root         (0)        0 2022-02-09 12:32:35.000000 pytest-django-ifactory-0.5.0/tests/testapp/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)       89 2022-02-09 12:32:35.000000 pytest-django-ifactory-0.5.0/tests/testapp/apps.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-02-09 12:32:40.949349 pytest-django-ifactory-0.5.0/tests/testapp/migrations/
--rw-rw-rw-   0 root         (0) root         (0)     3333 2022-02-09 12:32:35.000000 pytest-django-ifactory-0.5.0/tests/testapp/migrations/0001_initial.py
--rw-rw-rw-   0 root         (0) root         (0)        0 2022-02-09 12:32:35.000000 pytest-django-ifactory-0.5.0/tests/testapp/migrations/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1701 2022-02-09 12:32:35.000000 pytest-django-ifactory-0.5.0/tests/testapp/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-21 17:37:31.919160 pytest-django-ifactory-1.0.0/
+-rw-rw-rw-   0 root         (0) root         (0)     2173 2023-05-21 17:37:27.000000 pytest-django-ifactory-1.0.0/.gitlab-ci.yml
+-rw-rw-rw-   0 root         (0) root         (0)      582 2023-05-21 17:37:27.000000 pytest-django-ifactory-1.0.0/.pre-commit-config.yaml
+-rw-rw-rw-   0 root         (0) root         (0)      991 2023-05-21 17:37:27.000000 pytest-django-ifactory-1.0.0/CHANGES.md
+-rw-rw-rw-   0 root         (0) root         (0)     1517 2023-05-21 17:37:27.000000 pytest-django-ifactory-1.0.0/LICENSE
+-rw-rw-rw-   0 root         (0) root         (0)      216 2023-05-21 17:37:27.000000 pytest-django-ifactory-1.0.0/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     7113 2023-05-21 17:37:31.919160 pytest-django-ifactory-1.0.0/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)     6142 2023-05-21 17:37:27.000000 pytest-django-ifactory-1.0.0/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-21 17:37:31.915160 pytest-django-ifactory-1.0.0/docker/
+-rw-rw-rw-   0 root         (0) root         (0)      200 2023-05-21 17:37:27.000000 pytest-django-ifactory-1.0.0/docker/Dockerfile
+-rwxrwxrwx   0 root         (0) root         (0)      289 2023-05-21 17:37:27.000000 pytest-django-ifactory-1.0.0/docker/push.sh
+-rw-rw-rw-   0 root         (0) root         (0)      133 2023-05-21 17:37:27.000000 pytest-django-ifactory-1.0.0/pyproject.toml
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-21 17:37:31.915160 pytest-django-ifactory-1.0.0/pytest_django_ifactory/
+-rw-rw-rw-   0 root         (0) root         (0)      251 2023-05-21 17:37:27.000000 pytest-django-ifactory-1.0.0/pytest_django_ifactory/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     4606 2023-05-21 17:37:27.000000 pytest-django-ifactory-1.0.0/pytest_django_ifactory/defaults.py
+-rw-rw-rw-   0 root         (0) root         (0)     6015 2023-05-21 17:37:27.000000 pytest-django-ifactory-1.0.0/pytest_django_ifactory/ifactory.py
+-rw-rw-rw-   0 root         (0) root         (0)      763 2023-05-21 17:37:27.000000 pytest-django-ifactory-1.0.0/pytest_django_ifactory/plugin.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-21 17:37:31.917160 pytest-django-ifactory-1.0.0/pytest_django_ifactory.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     7113 2023-05-21 17:37:31.000000 pytest-django-ifactory-1.0.0/pytest_django_ifactory.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      891 2023-05-21 17:37:31.000000 pytest-django-ifactory-1.0.0/pytest_django_ifactory.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-05-21 17:37:31.000000 pytest-django-ifactory-1.0.0/pytest_django_ifactory.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       59 2023-05-21 17:37:31.000000 pytest-django-ifactory-1.0.0/pytest_django_ifactory.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)       14 2023-05-21 17:37:31.000000 pytest-django-ifactory-1.0.0/pytest_django_ifactory.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       23 2023-05-21 17:37:31.000000 pytest-django-ifactory-1.0.0/pytest_django_ifactory.egg-info/top_level.txt
+-rw-rw-rw-   0 root         (0) root         (0)      184 2023-05-21 17:37:27.000000 pytest-django-ifactory-1.0.0/requirements.txt
+-rw-rw-rw-   0 root         (0) root         (0)      167 2023-05-21 17:37:31.920160 pytest-django-ifactory-1.0.0/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)     1386 2023-05-21 17:37:27.000000 pytest-django-ifactory-1.0.0/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-21 17:37:31.918160 pytest-django-ifactory-1.0.0/tests/
+-rw-rw-rw-   0 root         (0) root         (0)      790 2023-05-21 17:37:27.000000 pytest-django-ifactory-1.0.0/tests/conftest.py
+-rw-rw-rw-   0 root         (0) root         (0)      697 2023-05-21 17:37:27.000000 pytest-django-ifactory-1.0.0/tests/djangosettings.py
+-rw-rw-rw-   0 root         (0) root         (0)     7642 2023-05-21 17:37:27.000000 pytest-django-ifactory-1.0.0/tests/test_defaults.py
+-rw-rw-rw-   0 root         (0) root         (0)     4104 2023-05-21 17:37:27.000000 pytest-django-ifactory-1.0.0/tests/test_ifactory.py
+-rw-rw-rw-   0 root         (0) root         (0)     1436 2023-05-21 17:37:27.000000 pytest-django-ifactory-1.0.0/tests/test_plugin.py
+-rw-rw-rw-   0 root         (0) root         (0)     1616 2023-05-21 17:37:27.000000 pytest-django-ifactory-1.0.0/tests/test_readme_examples.py
+-rw-rw-rw-   0 root         (0) root         (0)      176 2023-05-21 17:37:27.000000 pytest-django-ifactory-1.0.0/tests/test_toplevel.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-21 17:37:31.919160 pytest-django-ifactory-1.0.0/tests/testapp/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-05-21 17:37:27.000000 pytest-django-ifactory-1.0.0/tests/testapp/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)       89 2023-05-21 17:37:27.000000 pytest-django-ifactory-1.0.0/tests/testapp/apps.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-21 17:37:31.919160 pytest-django-ifactory-1.0.0/tests/testapp/migrations/
+-rw-rw-rw-   0 root         (0) root         (0)     3333 2023-05-21 17:37:27.000000 pytest-django-ifactory-1.0.0/tests/testapp/migrations/0001_initial.py
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-05-21 17:37:27.000000 pytest-django-ifactory-1.0.0/tests/testapp/migrations/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1701 2023-05-21 17:37:27.000000 pytest-django-ifactory-1.0.0/tests/testapp/models.py
```

### Comparing `pytest-django-ifactory-0.5.0/.gitlab-ci.yml` & `pytest-django-ifactory-1.0.0/.gitlab-ci.yml`

 * *Files 11% similar despite different names*

```diff
@@ -29,49 +29,43 @@
     SPATIALITE_LIBRARY_PATH: mod_spatialite
     TEST_DEPENDENCIES: pillow psycopg2-binary pytest-cov
   before_script:
     - pip install --no-cache-dir $TEST_DEPENDENCIES django~=$DJANGO_VERSION -e .
   script:
     - pytest --cov=pytest_django_ifactory
 
-test-py37-django22:
-  extends: .test
-  variables:
-    DJANGO_VERSION: 2.2.17
-  image: registry.gitlab.com/gorilladev/pytest-django-ifactory/python:3.7
-
 test-py37-django32:
   extends: .test
   variables:
-    DJANGO_VERSION: 3.2.12
+    DJANGO_VERSION: 3.2.19
   image: registry.gitlab.com/gorilladev/pytest-django-ifactory/python:3.7
 
-test-py38-django22:
+test-py38-django32:
   extends: .test
   variables:
-    DJANGO_VERSION: 2.2.17
+    DJANGO_VERSION: 3.2.19
   image: registry.gitlab.com/gorilladev/pytest-django-ifactory/python:3.8
 
-test-py38-django32:
+test-py39-django32:
   extends: .test
   variables:
-    DJANGO_VERSION: 3.2.12
-  image: registry.gitlab.com/gorilladev/pytest-django-ifactory/python:3.8
+    DJANGO_VERSION: 3.2.19
+  image: registry.gitlab.com/gorilladev/pytest-django-ifactory/python:3.9
 
-test-py39-django22:
+test-py310-django42:
   extends: .test
   variables:
-    DJANGO_VERSION: 2.2.17
-  image: registry.gitlab.com/gorilladev/pytest-django-ifactory/python:3.9
+    DJANGO_VERSION: 4.2.1
+  image: registry.gitlab.com/gorilladev/pytest-django-ifactory/python:3.10
 
-test-py39-django32:
+test-py311-django42:
   extends: .test
   variables:
-    DJANGO_VERSION: 3.2.12
-  image: registry.gitlab.com/gorilladev/pytest-django-ifactory/python:3.9
+    DJANGO_VERSION: 4.2.1
+  image: registry.gitlab.com/gorilladev/pytest-django-ifactory/python:3.11
 
 
 build:
   stage: build
   before_script:
     - pip install --upgrade setuptools wheel
   script:
```

### Comparing `pytest-django-ifactory-0.5.0/.pre-commit-config.yaml` & `pytest-django-ifactory-1.0.0/.pre-commit-config.yaml`

 * *Files 24% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 repos:
-  - repo: https://github.com/ambv/black
-    rev: "22.1.0"
+  - repo: https://github.com/psf/black
+    rev: "23.3.0"
     hooks:
       - id: black
         exclude: tests/testapp/migrations
   - repo: https://github.com/pre-commit/pre-commit-hooks
-    rev: "v4.1.0"
+    rev: "v4.4.0"
     hooks:
       - id: check-merge-conflict
       - id: debug-statements
       - id: end-of-file-fixer
       - id: trailing-whitespace
   - repo: https://github.com/pycqa/flake8
-    rev: "4.0.1"
+    rev: "6.0.0"
     hooks:
       - id: flake8
         exclude: tests/testapp/migrations
   - repo: https://github.com/mgedmin/check-manifest
-    rev: "0.47"
+    rev: "0.49"
     hooks:
       - id: check-manifest
```

### Comparing `pytest-django-ifactory-0.5.0/CHANGES.md` & `pytest-django-ifactory-1.0.0/CHANGES.md`

 * *Files 14% similar despite different names*

```diff
@@ -1,9 +1,17 @@
 # Change log
 
+## 1.0.0
+
+2023-05-21
+
+* Drop support for Django 2.2.
+* Add support for Django 4.2.
+* Add support for Python 3.10 and 3.11.
+
 ## 0.5.0
 
 2022-02-09
 
 * Drop support for Python 3.6.
 * Drop support for Django 3.0 and 3.1.
 * Add support for Django 3.2.
```

### Comparing `pytest-django-ifactory-0.5.0/LICENSE` & `pytest-django-ifactory-1.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `pytest-django-ifactory-0.5.0/PKG-INFO` & `pytest-django-ifactory-1.0.0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,27 +1,28 @@
 Metadata-Version: 2.1
 Name: pytest-django-ifactory
-Version: 0.5.0
+Version: 1.0.0
 Summary: A model instance factory for pytest-django
 Home-page: https://gitlab.com/gorilladev/pytest-django-ifactory
 Author: Mattias Jakobsson
 Author-email: mjakob422@gmail.com
 License: BSD-3-Clause
 Keywords: pytest django database testing
-Platform: UNKNOWN
-Classifier: Development Status :: 3 - Alpha
+Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Plugins
 Classifier: Framework :: Django
 Classifier: Framework :: Pytest
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Software Development :: Testing
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 [![pipeline status](https://gitlab.com/gorilladev/pytest-django-ifactory/badges/develop/pipeline.svg)](https://gitlab.com/gorilladev/pytest-django-ifactory/commits/develop)
 [![coverage report](https://gitlab.com/gorilladev/pytest-django-ifactory/badges/develop/coverage.svg)](https://gitlab.com/gorilladev/pytest-django-ifactory/commits/develop)
 
@@ -53,17 +54,14 @@
 tries to come up with acceptable defaults for the fields you don't
 care about. This includes generating unique values for fields marked
 as unique and to create related instances for non-nullable foreign
 keys.
 
 ## Usage
 
-**Note that this library is very much in alpha and its API may change
-in future versions.**
-
 This plugin comes with two fixtures: `ifactory` and
 `transactional_ifactory`.  Use them when you need to put model
 instances in the database.  `ifactory` and `transactional_ifactory`
 are identical except that the latter uses [pytest-django][]'s
 `transactional_db` fixture instead of the `db` fixture.  See
 pytest-django's and Django's documentation for when you would want to
 use it.  Below is a contrived example to test a function that finds
@@ -153,16 +151,16 @@
 except the unit tests will be run everytime a commit is made. The unit
 tests are run manually with pytest
 
 ```console
 $ pytest
 ```
 
-Gitlab CI is configured to run the tests with Python 3.7-3.9 and all
-supported Django versions.
+Gitlab CI is configured to run the tests with Python 3.7-3.11 and all
+supported Django LTS versions.
 
 If you want to install all development requirements to run them
 manually (and without using `pre-commit run --all-files`), use the
 [requirements.txt](requirements.txt) file:
 
 ```console
 $ pip install -r requirements.txt
@@ -174,9 +172,7 @@
 [pre-commit]: https://github.com/pre-commit/pre-commit
 [pytest]: http://pytest.org/
 
 ## License
 
 Like [pytest-django][], pytest-django-ifactory is released under the
 [BSD 3-clause](LICENSE) license.
-
-
```

### Comparing `pytest-django-ifactory-0.5.0/README.md` & `pytest-django-ifactory-1.0.0/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -29,17 +29,14 @@
 tries to come up with acceptable defaults for the fields you don't
 care about. This includes generating unique values for fields marked
 as unique and to create related instances for non-nullable foreign
 keys.
 
 ## Usage
 
-**Note that this library is very much in alpha and its API may change
-in future versions.**
-
 This plugin comes with two fixtures: `ifactory` and
 `transactional_ifactory`.  Use them when you need to put model
 instances in the database.  `ifactory` and `transactional_ifactory`
 are identical except that the latter uses [pytest-django][]'s
 `transactional_db` fixture instead of the `db` fixture.  See
 pytest-django's and Django's documentation for when you would want to
 use it.  Below is a contrived example to test a function that finds
@@ -129,16 +126,16 @@
 except the unit tests will be run everytime a commit is made. The unit
 tests are run manually with pytest
 
 ```console
 $ pytest
 ```
 
-Gitlab CI is configured to run the tests with Python 3.7-3.9 and all
-supported Django versions.
+Gitlab CI is configured to run the tests with Python 3.7-3.11 and all
+supported Django LTS versions.
 
 If you want to install all development requirements to run them
 manually (and without using `pre-commit run --all-files`), use the
 [requirements.txt](requirements.txt) file:
 
 ```console
 $ pip install -r requirements.txt
```

### Comparing `pytest-django-ifactory-0.5.0/pytest_django_ifactory/defaults.py` & `pytest-django-ifactory-1.0.0/pytest_django_ifactory/defaults.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,15 +1,14 @@
 """Default value generation for model fields."""
 
 import datetime
 import itertools
 import string
 
 from django.core.exceptions import ImproperlyConfigured
-from django.utils import timezone
 
 try:
     from django.contrib.gis.db import models
 except ImproperlyConfigured:
     from django.db import models
 
 try:
@@ -75,16 +74,17 @@
         return lambda: datetime.date.fromtimestamp(next(it))
     return datetime.date.fromtimestamp(0)
 
 
 @register(models.DateTimeField)
 def date_time_field_default(field, unique=False):
     def todatetime(timestamp):
-        t = datetime.datetime.utcfromtimestamp(timestamp)
-        return timezone.make_aware(t, timezone.utc)
+        return datetime.datetime.utcfromtimestamp(timestamp).replace(
+            tzinfo=datetime.timezone.utc
+        )
 
     if field.auto_now or field.auto_now_add:
         return None
     if unique or field.unique:
         it = itertools.count(step=60**2)
         return lambda: todatetime(next(it))
     return todatetime(0)
```

### Comparing `pytest-django-ifactory-0.5.0/pytest_django_ifactory/ifactory.py` & `pytest-django-ifactory-1.0.0/pytest_django_ifactory/ifactory.py`

 * *Files identical despite different names*

### Comparing `pytest-django-ifactory-0.5.0/pytest_django_ifactory/plugin.py` & `pytest-django-ifactory-1.0.0/pytest_django_ifactory/plugin.py`

 * *Files identical despite different names*

### Comparing `pytest-django-ifactory-0.5.0/pytest_django_ifactory.egg-info/PKG-INFO` & `pytest-django-ifactory-1.0.0/pytest_django_ifactory.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,27 +1,28 @@
 Metadata-Version: 2.1
 Name: pytest-django-ifactory
-Version: 0.5.0
+Version: 1.0.0
 Summary: A model instance factory for pytest-django
 Home-page: https://gitlab.com/gorilladev/pytest-django-ifactory
 Author: Mattias Jakobsson
 Author-email: mjakob422@gmail.com
 License: BSD-3-Clause
 Keywords: pytest django database testing
-Platform: UNKNOWN
-Classifier: Development Status :: 3 - Alpha
+Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Plugins
 Classifier: Framework :: Django
 Classifier: Framework :: Pytest
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Software Development :: Testing
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 [![pipeline status](https://gitlab.com/gorilladev/pytest-django-ifactory/badges/develop/pipeline.svg)](https://gitlab.com/gorilladev/pytest-django-ifactory/commits/develop)
 [![coverage report](https://gitlab.com/gorilladev/pytest-django-ifactory/badges/develop/coverage.svg)](https://gitlab.com/gorilladev/pytest-django-ifactory/commits/develop)
 
@@ -53,17 +54,14 @@
 tries to come up with acceptable defaults for the fields you don't
 care about. This includes generating unique values for fields marked
 as unique and to create related instances for non-nullable foreign
 keys.
 
 ## Usage
 
-**Note that this library is very much in alpha and its API may change
-in future versions.**
-
 This plugin comes with two fixtures: `ifactory` and
 `transactional_ifactory`.  Use them when you need to put model
 instances in the database.  `ifactory` and `transactional_ifactory`
 are identical except that the latter uses [pytest-django][]'s
 `transactional_db` fixture instead of the `db` fixture.  See
 pytest-django's and Django's documentation for when you would want to
 use it.  Below is a contrived example to test a function that finds
@@ -153,16 +151,16 @@
 except the unit tests will be run everytime a commit is made. The unit
 tests are run manually with pytest
 
 ```console
 $ pytest
 ```
 
-Gitlab CI is configured to run the tests with Python 3.7-3.9 and all
-supported Django versions.
+Gitlab CI is configured to run the tests with Python 3.7-3.11 and all
+supported Django LTS versions.
 
 If you want to install all development requirements to run them
 manually (and without using `pre-commit run --all-files`), use the
 [requirements.txt](requirements.txt) file:
 
 ```console
 $ pip install -r requirements.txt
@@ -174,9 +172,7 @@
 [pre-commit]: https://github.com/pre-commit/pre-commit
 [pytest]: http://pytest.org/
 
 ## License
 
 Like [pytest-django][], pytest-django-ifactory is released under the
 [BSD 3-clause](LICENSE) license.
-
-
```

### Comparing `pytest-django-ifactory-0.5.0/pytest_django_ifactory.egg-info/SOURCES.txt` & `pytest-django-ifactory-1.0.0/pytest_django_ifactory.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pytest-django-ifactory-0.5.0/setup.py` & `pytest-django-ifactory-1.0.0/setup.py`

 * *Files 14% similar despite different names*

```diff
@@ -3,33 +3,35 @@
 from setuptools import setup, find_packages
 
 with open("README.md", "r") as stream:
     long_description = stream.read()
 
 setup(
     name="pytest-django-ifactory",
-    version="0.5.0",
+    version="1.0.0",
     author="Mattias Jakobsson",
     author_email="mjakob422@gmail.com",
     description="A model instance factory for pytest-django",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://gitlab.com/gorilladev/pytest-django-ifactory",
     license="BSD-3-Clause",
     classifiers=[
-        "Development Status :: 3 - Alpha",
+        "Development Status :: 5 - Production/Stable",
         "Environment :: Plugins",
         "Framework :: Django",
         "Framework :: Pytest",
         "Intended Audience :: Developers",
         "License :: OSI Approved :: BSD License",
         "Programming Language :: Python :: 3",
         "Programming Language :: Python :: 3.7",
         "Programming Language :: Python :: 3.8",
         "Programming Language :: Python :: 3.9",
+        "Programming Language :: Python :: 3.10",
+        "Programming Language :: Python :: 3.11",
         "Topic :: Software Development :: Testing",
     ],
     keywords="pytest django database testing",
     packages=find_packages(exclude=["tests*"]),
     install_requires=["pytest-django"],
     entry_points={"pytest11": ["django-ifactory = pytest_django_ifactory.plugin"]},
 )
```

### Comparing `pytest-django-ifactory-0.5.0/tests/conftest.py` & `pytest-django-ifactory-1.0.0/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `pytest-django-ifactory-0.5.0/tests/djangosettings.py` & `pytest-django-ifactory-1.0.0/tests/djangosettings.py`

 * *Files identical despite different names*

### Comparing `pytest-django-ifactory-0.5.0/tests/test_defaults.py` & `pytest-django-ifactory-1.0.0/tests/test_defaults.py`

 * *Files 0% similar despite different names*

```diff
@@ -146,15 +146,15 @@
         assert default() == 1
 
 
 class TestTimeFieldDefault:
     def test_nonunique(self):
         field = models.TimeField()
         default = generate_default_value(field)
-        assert default == parse_time("00:00Z")
+        assert default == parse_time("00:00")
 
     @pytest.mark.parametrize("field_is_unique", [True, False])
     def test_unique(self, field_is_unique):
         field = models.TimeField(unique=field_is_unique)
         default = generate_default_value(field, unique=not field_is_unique)
         assert isinstance(default, abc.Callable)
         assert default() == parse_time("00:00:00")
```

### Comparing `pytest-django-ifactory-0.5.0/tests/test_ifactory.py` & `pytest-django-ifactory-1.0.0/tests/test_ifactory.py`

 * *Files identical despite different names*

### Comparing `pytest-django-ifactory-0.5.0/tests/test_plugin.py` & `pytest-django-ifactory-1.0.0/tests/test_plugin.py`

 * *Files identical despite different names*

### Comparing `pytest-django-ifactory-0.5.0/tests/test_readme_examples.py` & `pytest-django-ifactory-1.0.0/tests/test_readme_examples.py`

 * *Files identical despite different names*

### Comparing `pytest-django-ifactory-0.5.0/tests/testapp/migrations/0001_initial.py` & `pytest-django-ifactory-1.0.0/tests/testapp/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `pytest-django-ifactory-0.5.0/tests/testapp/models.py` & `pytest-django-ifactory-1.0.0/tests/testapp/models.py`

 * *Files identical despite different names*

