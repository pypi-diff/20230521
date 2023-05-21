# Comparing `tmp/django-minio-storage-0.5.3.tar.gz` & `tmp/django-minio-storage-0.5.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django-minio-storage-0.5.3.tar", last modified: Mon May 15 18:27:11 2023, max compression
+gzip compressed data, was "django-minio-storage-0.5.4.tar", last modified: Sun May 21 14:48:33 2023, max compression
```

## Comparing `django-minio-storage-0.5.3.tar` & `django-minio-storage-0.5.4.tar`

### file list

```diff
@@ -1,70 +1,70 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 18:27:11.318951 django-minio-storage-0.5.3/
--rw-r--r--   0 runner    (1001) docker     (123)      282 2023-05-15 18:27:01.000000 django-minio-storage-0.5.3/.editorconfig
--rw-r--r--   0 runner    (1001) docker     (123)      104 2023-05-15 18:27:01.000000 django-minio-storage-0.5.3/.flake8rc
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 18:27:11.310950 django-minio-storage-0.5.3/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 18:27:11.314951 django-minio-storage-0.5.3/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)      716 2023-05-15 18:27:01.000000 django-minio-storage-0.5.3/.github/workflows/release.yml
--rw-r--r--   0 runner    (1001) docker     (123)      939 2023-05-15 18:27:01.000000 django-minio-storage-0.5.3/.github/workflows/tox.yml
--rw-r--r--   0 runner    (1001) docker     (123)      126 2023-05-15 18:27:01.000000 django-minio-storage-0.5.3/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)       71 2023-05-15 18:27:01.000000 django-minio-storage-0.5.3/.isort.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      368 2023-05-15 18:27:01.000000 django-minio-storage-0.5.3/.readthedocs.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     3361 2023-05-15 18:27:01.000000 django-minio-storage-0.5.3/CHANGELOG.md
--rw-r--r--   0 runner    (1001) docker     (123)       43 2023-05-15 18:27:01.000000 django-minio-storage-0.5.3/CONTRIBUTING.md
--rw-r--r--   0 runner    (1001) docker     (123)    11004 2023-05-15 18:27:01.000000 django-minio-storage-0.5.3/LICENSE-APACHE
--rw-r--r--   0 runner    (1001) docker     (123)     1102 2023-05-15 18:27:01.000000 django-minio-storage-0.5.3/LICENSE-MIT
--rw-r--r--   0 runner    (1001) docker     (123)     1702 2023-05-15 18:27:11.318951 django-minio-storage-0.5.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      958 2023-05-15 18:27:01.000000 django-minio-storage-0.5.3/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      105 2023-05-15 18:27:01.000000 django-minio-storage-0.5.3/dev-requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 18:27:11.314951 django-minio-storage-0.5.3/django_minio_storage.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1702 2023-05-15 18:27:11.000000 django-minio-storage-0.5.3/django_minio_storage.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1479 2023-05-15 18:27:11.000000 django-minio-storage-0.5.3/django_minio_storage.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-15 18:27:11.000000 django-minio-storage-0.5.3/django_minio_storage.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-05-15 18:27:11.000000 django-minio-storage-0.5.3/django_minio_storage.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       75 2023-05-15 18:27:11.000000 django-minio-storage-0.5.3/django_minio_storage.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      249 2023-05-15 18:27:01.000000 django-minio-storage-0.5.3/docker-compose.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 18:27:11.314951 django-minio-storage-0.5.3/docs/
--rw-r--r--   0 runner    (1001) docker     (123)      244 2023-05-15 18:27:01.000000 django-minio-storage-0.5.3/docs/contributing.md
--rw-r--r--   0 runner    (1001) docker     (123)      670 2023-05-15 18:27:01.000000 django-minio-storage-0.5.3/docs/development.md
--rw-r--r--   0 runner    (1001) docker     (123)      770 2023-05-15 18:27:01.000000 django-minio-storage-0.5.3/docs/index.md
--rw-r--r--   0 runner    (1001) docker     (123)    12348 2023-05-15 18:27:01.000000 django-minio-storage-0.5.3/docs/licences.md
--rw-r--r--   0 runner    (1001) docker     (123)     5617 2023-05-15 18:27:01.000000 django-minio-storage-0.5.3/docs/usage.md
--rw-r--r--   0 runner    (1001) docker     (123)       14 2023-05-15 18:27:01.000000 django-minio-storage-0.5.3/docs-requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 18:27:11.318951 django-minio-storage-0.5.3/minio_storage/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-15 18:27:01.000000 django-minio-storage-0.5.3/minio_storage/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      102 2023-05-15 18:27:01.000000 django-minio-storage-0.5.3/minio_storage/apps.py
--rw-r--r--   0 runner    (1001) docker     (123)      407 2023-05-15 18:27:01.000000 django-minio-storage-0.5.3/minio_storage/errors.py
--rw-r--r--   0 runner    (1001) docker     (123)     4498 2023-05-15 18:27:01.000000 django-minio-storage-0.5.3/minio_storage/files.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 18:27:11.318951 django-minio-storage-0.5.3/minio_storage/management/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-15 18:27:01.000000 django-minio-storage-0.5.3/minio_storage/management/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 18:27:11.318951 django-minio-storage-0.5.3/minio_storage/management/commands/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-15 18:27:01.000000 django-minio-storage-0.5.3/minio_storage/management/commands/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8346 2023-05-15 18:27:01.000000 django-minio-storage-0.5.3/minio_storage/management/commands/minio.py
--rw-r--r--   0 runner    (1001) docker     (123)     4108 2023-05-15 18:27:01.000000 django-minio-storage-0.5.3/minio_storage/policy.py
--rw-r--r--   0 runner    (1001) docker     (123)    16538 2023-05-15 18:27:01.000000 django-minio-storage-0.5.3/minio_storage/storage.py
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-05-15 18:27:11.000000 django-minio-storage-0.5.3/minio_storage/version.py
--rw-r--r--   0 runner    (1001) docker     (123)      197 2023-05-15 18:27:01.000000 django-minio-storage-0.5.3/mkdocs.yml
--rw-r--r--   0 runner    (1001) docker     (123)       40 2023-05-15 18:27:01.000000 django-minio-storage-0.5.3/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      416 2023-05-15 18:27:01.000000 django-minio-storage-0.5.3/pyrightconfig.json
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-15 18:27:11.318951 django-minio-storage-0.5.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1349 2023-05-15 18:27:01.000000 django-minio-storage-0.5.3/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 18:27:11.318951 django-minio-storage-0.5.3/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-15 18:27:01.000000 django-minio-storage-0.5.3/tests/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 18:27:11.318951 django-minio-storage-0.5.3/tests/django_minio_storage_tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-15 18:27:01.000000 django-minio-storage-0.5.3/tests/django_minio_storage_tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4156 2023-05-15 18:27:01.000000 django-minio-storage-0.5.3/tests/django_minio_storage_tests/settings.py
--rw-r--r--   0 runner    (1001) docker     (123)      770 2023-05-15 18:27:01.000000 django-minio-storage-0.5.3/tests/django_minio_storage_tests/urls.py
--rw-r--r--   0 runner    (1001) docker     (123)      429 2023-05-15 18:27:01.000000 django-minio-storage-0.5.3/tests/django_minio_storage_tests/wsgi.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      283 2023-05-15 18:27:01.000000 django-minio-storage-0.5.3/tests/manage.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 18:27:11.318951 django-minio-storage-0.5.3/tests/test_app/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-15 18:27:01.000000 django-minio-storage-0.5.3/tests/test_app/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 18:27:11.318951 django-minio-storage-0.5.3/tests/test_app/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-15 18:27:01.000000 django-minio-storage-0.5.3/tests/test_app/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6121 2023-05-15 18:27:01.000000 django-minio-storage-0.5.3/tests/test_app/tests/bucket_tests.py
--rw-r--r--   0 runner    (1001) docker     (123)     4594 2023-05-15 18:27:01.000000 django-minio-storage-0.5.3/tests/test_app/tests/custom_storage_class_tests.py
--rw-r--r--   0 runner    (1001) docker     (123)     1656 2023-05-15 18:27:01.000000 django-minio-storage-0.5.3/tests/test_app/tests/delete_tests.py
--rw-r--r--   0 runner    (1001) docker     (123)     5365 2023-05-15 18:27:01.000000 django-minio-storage-0.5.3/tests/test_app/tests/managementcommand_tests.py
--rw-r--r--   0 runner    (1001) docker     (123)     9634 2023-05-15 18:27:01.000000 django-minio-storage-0.5.3/tests/test_app/tests/retrieve_tests.py
--rw-r--r--   0 runner    (1001) docker     (123)     4117 2023-05-15 18:27:01.000000 django-minio-storage-0.5.3/tests/test_app/tests/upload_tests.py
--rw-r--r--   0 runner    (1001) docker     (123)     1785 2023-05-15 18:27:01.000000 django-minio-storage-0.5.3/tests/test_app/tests/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    79300 2023-05-15 18:27:01.000000 django-minio-storage-0.5.3/tests/watermelon-cat.jpg
--rw-r--r--   0 runner    (1001) docker     (123)     2081 2023-05-15 18:27:01.000000 django-minio-storage-0.5.3/tox.ini
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 14:48:33.892261 django-minio-storage-0.5.4/
+-rw-r--r--   0 runner    (1001) docker     (123)      282 2023-05-21 14:48:24.000000 django-minio-storage-0.5.4/.editorconfig
+-rw-r--r--   0 runner    (1001) docker     (123)      129 2023-05-21 14:48:24.000000 django-minio-storage-0.5.4/.flake8rc
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 14:48:33.884261 django-minio-storage-0.5.4/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 14:48:33.888261 django-minio-storage-0.5.4/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)      716 2023-05-21 14:48:24.000000 django-minio-storage-0.5.4/.github/workflows/release.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      939 2023-05-21 14:48:24.000000 django-minio-storage-0.5.4/.github/workflows/tox.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      126 2023-05-21 14:48:24.000000 django-minio-storage-0.5.4/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)       71 2023-05-21 14:48:24.000000 django-minio-storage-0.5.4/.isort.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      368 2023-05-21 14:48:24.000000 django-minio-storage-0.5.4/.readthedocs.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     3416 2023-05-21 14:48:24.000000 django-minio-storage-0.5.4/CHANGELOG.md
+-rw-r--r--   0 runner    (1001) docker     (123)       43 2023-05-21 14:48:24.000000 django-minio-storage-0.5.4/CONTRIBUTING.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1102 2023-05-21 14:48:24.000000 django-minio-storage-0.5.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    11004 2023-05-21 14:48:24.000000 django-minio-storage-0.5.4/LICENSE-APACHE
+-rw-r--r--   0 runner    (1001) docker     (123)     3174 2023-05-21 14:48:33.892261 django-minio-storage-0.5.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      958 2023-05-21 14:48:24.000000 django-minio-storage-0.5.4/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      105 2023-05-21 14:48:24.000000 django-minio-storage-0.5.4/dev-requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 14:48:33.888261 django-minio-storage-0.5.4/django_minio_storage.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3174 2023-05-21 14:48:33.000000 django-minio-storage-0.5.4/django_minio_storage.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1485 2023-05-21 14:48:33.000000 django-minio-storage-0.5.4/django_minio_storage.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-21 14:48:33.000000 django-minio-storage-0.5.4/django_minio_storage.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       26 2023-05-21 14:48:33.000000 django-minio-storage-0.5.4/django_minio_storage.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       14 2023-05-21 14:48:33.000000 django-minio-storage-0.5.4/django_minio_storage.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      249 2023-05-21 14:48:24.000000 django-minio-storage-0.5.4/docker-compose.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 14:48:33.888261 django-minio-storage-0.5.4/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)      244 2023-05-21 14:48:24.000000 django-minio-storage-0.5.4/docs/contributing.md
+-rw-r--r--   0 runner    (1001) docker     (123)      670 2023-05-21 14:48:24.000000 django-minio-storage-0.5.4/docs/development.md
+-rw-r--r--   0 runner    (1001) docker     (123)      770 2023-05-21 14:48:24.000000 django-minio-storage-0.5.4/docs/index.md
+-rw-r--r--   0 runner    (1001) docker     (123)    12348 2023-05-21 14:48:24.000000 django-minio-storage-0.5.4/docs/licences.md
+-rw-r--r--   0 runner    (1001) docker     (123)     5617 2023-05-21 14:48:24.000000 django-minio-storage-0.5.4/docs/usage.md
+-rw-r--r--   0 runner    (1001) docker     (123)       14 2023-05-21 14:48:24.000000 django-minio-storage-0.5.4/docs-requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 14:48:33.888261 django-minio-storage-0.5.4/minio_storage/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-21 14:48:24.000000 django-minio-storage-0.5.4/minio_storage/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      102 2023-05-21 14:48:24.000000 django-minio-storage-0.5.4/minio_storage/apps.py
+-rw-r--r--   0 runner    (1001) docker     (123)      407 2023-05-21 14:48:24.000000 django-minio-storage-0.5.4/minio_storage/errors.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4498 2023-05-21 14:48:24.000000 django-minio-storage-0.5.4/minio_storage/files.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 14:48:33.888261 django-minio-storage-0.5.4/minio_storage/management/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-21 14:48:24.000000 django-minio-storage-0.5.4/minio_storage/management/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 14:48:33.888261 django-minio-storage-0.5.4/minio_storage/management/commands/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-21 14:48:24.000000 django-minio-storage-0.5.4/minio_storage/management/commands/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8346 2023-05-21 14:48:24.000000 django-minio-storage-0.5.4/minio_storage/management/commands/minio.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4108 2023-05-21 14:48:24.000000 django-minio-storage-0.5.4/minio_storage/policy.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16538 2023-05-21 14:48:24.000000 django-minio-storage-0.5.4/minio_storage/storage.py
+-rw-r--r--   0 runner    (1001) docker     (123)       21 2023-05-21 14:48:33.000000 django-minio-storage-0.5.4/minio_storage/version.py
+-rw-r--r--   0 runner    (1001) docker     (123)      197 2023-05-21 14:48:24.000000 django-minio-storage-0.5.4/mkdocs.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1272 2023-05-21 14:48:24.000000 django-minio-storage-0.5.4/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      416 2023-05-21 14:48:24.000000 django-minio-storage-0.5.4/pyrightconfig.json
+-rw-r--r--   0 runner    (1001) docker     (123)      117 2023-05-21 14:48:33.892261 django-minio-storage-0.5.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-21 14:48:24.000000 django-minio-storage-0.5.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 14:48:33.888261 django-minio-storage-0.5.4/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-21 14:48:24.000000 django-minio-storage-0.5.4/tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 14:48:33.888261 django-minio-storage-0.5.4/tests/django_minio_storage_tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-21 14:48:24.000000 django-minio-storage-0.5.4/tests/django_minio_storage_tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4156 2023-05-21 14:48:24.000000 django-minio-storage-0.5.4/tests/django_minio_storage_tests/settings.py
+-rw-r--r--   0 runner    (1001) docker     (123)      770 2023-05-21 14:48:24.000000 django-minio-storage-0.5.4/tests/django_minio_storage_tests/urls.py
+-rw-r--r--   0 runner    (1001) docker     (123)      429 2023-05-21 14:48:24.000000 django-minio-storage-0.5.4/tests/django_minio_storage_tests/wsgi.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      283 2023-05-21 14:48:24.000000 django-minio-storage-0.5.4/tests/manage.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 14:48:33.888261 django-minio-storage-0.5.4/tests/test_app/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-21 14:48:24.000000 django-minio-storage-0.5.4/tests/test_app/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 14:48:33.892261 django-minio-storage-0.5.4/tests/test_app/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-21 14:48:24.000000 django-minio-storage-0.5.4/tests/test_app/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6121 2023-05-21 14:48:24.000000 django-minio-storage-0.5.4/tests/test_app/tests/bucket_tests.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4594 2023-05-21 14:48:24.000000 django-minio-storage-0.5.4/tests/test_app/tests/custom_storage_class_tests.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1656 2023-05-21 14:48:24.000000 django-minio-storage-0.5.4/tests/test_app/tests/delete_tests.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5365 2023-05-21 14:48:24.000000 django-minio-storage-0.5.4/tests/test_app/tests/managementcommand_tests.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9634 2023-05-21 14:48:24.000000 django-minio-storage-0.5.4/tests/test_app/tests/retrieve_tests.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4117 2023-05-21 14:48:24.000000 django-minio-storage-0.5.4/tests/test_app/tests/upload_tests.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1785 2023-05-21 14:48:24.000000 django-minio-storage-0.5.4/tests/test_app/tests/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    79300 2023-05-21 14:48:24.000000 django-minio-storage-0.5.4/tests/watermelon-cat.jpg
+-rw-r--r--   0 runner    (1001) docker     (123)     2081 2023-05-21 14:48:24.000000 django-minio-storage-0.5.4/tox.ini
```

### Comparing `django-minio-storage-0.5.3/.github/workflows/release.yml` & `django-minio-storage-0.5.4/.github/workflows/release.yml`

 * *Files identical despite different names*

### Comparing `django-minio-storage-0.5.3/.github/workflows/tox.yml` & `django-minio-storage-0.5.4/.github/workflows/tox.yml`

 * *Files identical despite different names*

### Comparing `django-minio-storage-0.5.3/CHANGELOG.md` & `django-minio-storage-0.5.4/CHANGELOG.md`

 * *Files 3% similar despite different names*

```diff
@@ -1,7 +1,11 @@
+## 0.5.3
+
+Migrate package meta data to pyproject.toml
+
 ## 0.5.2
 
 Add/fix more type hints.
 
 ## 0.5.1
 
 Fix type hints
```

### Comparing `django-minio-storage-0.5.3/LICENSE-APACHE` & `django-minio-storage-0.5.4/LICENSE-APACHE`

 * *Files identical despite different names*

### Comparing `django-minio-storage-0.5.3/LICENSE-MIT` & `django-minio-storage-0.5.4/LICENSE`

 * *Files identical despite different names*

### Comparing `django-minio-storage-0.5.3/README.md` & `django-minio-storage-0.5.4/README.md`

 * *Files identical despite different names*

### Comparing `django-minio-storage-0.5.3/django_minio_storage.egg-info/SOURCES.txt` & `django-minio-storage-0.5.4/django_minio_storage.egg-info/SOURCES.txt`

 * *Files 4% similar despite different names*

```diff
@@ -1,23 +1,24 @@
 .editorconfig
 .flake8rc
 .gitignore
 .isort.cfg
 .readthedocs.yaml
 CHANGELOG.md
 CONTRIBUTING.md
+LICENSE
 LICENSE-APACHE
-LICENSE-MIT
 README.md
 dev-requirements.txt
 docker-compose.yml
 docs-requirements.txt
 mkdocs.yml
 pyproject.toml
 pyrightconfig.json
+setup.cfg
 setup.py
 tox.ini
 .github/workflows/release.yml
 .github/workflows/tox.yml
 django_minio_storage.egg-info/PKG-INFO
 django_minio_storage.egg-info/SOURCES.txt
 django_minio_storage.egg-info/dependency_links.txt
```

### Comparing `django-minio-storage-0.5.3/docs/development.md` & `django-minio-storage-0.5.4/docs/development.md`

 * *Files identical despite different names*

### Comparing `django-minio-storage-0.5.3/docs/index.md` & `django-minio-storage-0.5.4/docs/index.md`

 * *Files identical despite different names*

### Comparing `django-minio-storage-0.5.3/docs/licences.md` & `django-minio-storage-0.5.4/docs/licences.md`

 * *Files identical despite different names*

### Comparing `django-minio-storage-0.5.3/docs/usage.md` & `django-minio-storage-0.5.4/docs/usage.md`

 * *Files identical despite different names*

### Comparing `django-minio-storage-0.5.3/minio_storage/files.py` & `django-minio-storage-0.5.4/minio_storage/files.py`

 * *Files identical despite different names*

### Comparing `django-minio-storage-0.5.3/minio_storage/management/commands/minio.py` & `django-minio-storage-0.5.4/minio_storage/management/commands/minio.py`

 * *Files identical despite different names*

### Comparing `django-minio-storage-0.5.3/minio_storage/policy.py` & `django-minio-storage-0.5.4/minio_storage/policy.py`

 * *Files identical despite different names*

### Comparing `django-minio-storage-0.5.3/minio_storage/storage.py` & `django-minio-storage-0.5.4/minio_storage/storage.py`

 * *Files identical despite different names*

### Comparing `django-minio-storage-0.5.3/tests/django_minio_storage_tests/settings.py` & `django-minio-storage-0.5.4/tests/django_minio_storage_tests/settings.py`

 * *Files identical despite different names*

### Comparing `django-minio-storage-0.5.3/tests/django_minio_storage_tests/urls.py` & `django-minio-storage-0.5.4/tests/django_minio_storage_tests/urls.py`

 * *Files identical despite different names*

### Comparing `django-minio-storage-0.5.3/tests/test_app/tests/bucket_tests.py` & `django-minio-storage-0.5.4/tests/test_app/tests/bucket_tests.py`

 * *Files identical despite different names*

### Comparing `django-minio-storage-0.5.3/tests/test_app/tests/custom_storage_class_tests.py` & `django-minio-storage-0.5.4/tests/test_app/tests/custom_storage_class_tests.py`

 * *Files identical despite different names*

### Comparing `django-minio-storage-0.5.3/tests/test_app/tests/delete_tests.py` & `django-minio-storage-0.5.4/tests/test_app/tests/delete_tests.py`

 * *Files identical despite different names*

### Comparing `django-minio-storage-0.5.3/tests/test_app/tests/managementcommand_tests.py` & `django-minio-storage-0.5.4/tests/test_app/tests/managementcommand_tests.py`

 * *Files identical despite different names*

### Comparing `django-minio-storage-0.5.3/tests/test_app/tests/retrieve_tests.py` & `django-minio-storage-0.5.4/tests/test_app/tests/retrieve_tests.py`

 * *Files identical despite different names*

### Comparing `django-minio-storage-0.5.3/tests/test_app/tests/upload_tests.py` & `django-minio-storage-0.5.4/tests/test_app/tests/upload_tests.py`

 * *Files identical despite different names*

### Comparing `django-minio-storage-0.5.3/tests/test_app/tests/utils.py` & `django-minio-storage-0.5.4/tests/test_app/tests/utils.py`

 * *Files identical despite different names*

### Comparing `django-minio-storage-0.5.3/tests/watermelon-cat.jpg` & `django-minio-storage-0.5.4/tests/watermelon-cat.jpg`

 * *Files identical despite different names*

### Comparing `django-minio-storage-0.5.3/tox.ini` & `django-minio-storage-0.5.4/tox.ini`

 * *Files identical despite different names*

