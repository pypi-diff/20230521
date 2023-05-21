# Comparing `tmp/pyclean-2.7.2.tar.gz` & `tmp/pyclean-2.7.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyclean-2.7.2.tar", last modified: Thu May 11 22:32:58 2023, max compression
+gzip compressed data, was "pyclean-2.7.3.tar", last modified: Sun May 21 21:02:45 2023, max compression
```

## Comparing `pyclean-2.7.2.tar` & `pyclean-2.7.3.tar`

### file list

```diff
@@ -1,30 +1,30 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 22:32:58.096481 pyclean-2.7.2/
--rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-05-11 22:32:44.000000 pyclean-2.7.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       35 2023-05-11 22:32:44.000000 pyclean-2.7.2/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     9074 2023-05-11 22:32:58.096481 pyclean-2.7.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     7861 2023-05-11 22:32:44.000000 pyclean-2.7.2/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 22:32:58.092481 pyclean-2.7.2/pyclean/
--rw-r--r--   0 runner    (1001) docker     (123)       98 2023-05-11 22:32:44.000000 pyclean-2.7.2/pyclean/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      139 2023-05-11 22:32:44.000000 pyclean-2.7.2/pyclean/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4733 2023-05-11 22:32:44.000000 pyclean-2.7.2/pyclean/cli.py
--rw-r--r--   0 runner    (1001) docker     (123)     1153 2023-05-11 22:32:44.000000 pyclean-2.7.2/pyclean/compat.py
--rw-r--r--   0 runner    (1001) docker     (123)     7229 2023-05-11 22:32:44.000000 pyclean-2.7.2/pyclean/modern.py
--rw-r--r--   0 runner    (1001) docker     (123)     2541 2023-05-11 22:32:44.000000 pyclean-2.7.2/pyclean/py2clean.py
--rw-r--r--   0 runner    (1001) docker     (123)     6132 2023-05-11 22:32:44.000000 pyclean-2.7.2/pyclean/py3clean.py
--rw-r--r--   0 runner    (1001) docker     (123)     6209 2023-05-11 22:32:44.000000 pyclean-2.7.2/pyclean/pypyclean.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 22:32:58.092481 pyclean-2.7.2/pyclean.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     9074 2023-05-11 22:32:58.000000 pyclean-2.7.2/pyclean.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      492 2023-05-11 22:32:58.000000 pyclean-2.7.2/pyclean.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-11 22:32:58.000000 pyclean-2.7.2/pyclean.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      143 2023-05-11 22:32:58.000000 pyclean-2.7.2/pyclean.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-05-11 22:32:58.000000 pyclean-2.7.2/pyclean.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      678 2023-05-11 22:32:44.000000 pyclean-2.7.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-11 22:32:58.096481 pyclean-2.7.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1950 2023-05-11 22:32:44.000000 pyclean-2.7.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 22:32:58.096481 pyclean-2.7.2/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     7183 2023-05-11 22:32:44.000000 pyclean-2.7.2/tests/test_cli.py
--rw-r--r--   0 runner    (1001) docker     (123)     1159 2023-05-11 22:32:44.000000 pyclean-2.7.2/tests/test_compat.py
--rw-r--r--   0 runner    (1001) docker     (123)      434 2023-05-11 22:32:44.000000 pyclean-2.7.2/tests/test_directory.py
--rw-r--r--   0 runner    (1001) docker     (123)    11647 2023-05-11 22:32:44.000000 pyclean-2.7.2/tests/test_modern.py
--rw-r--r--   0 runner    (1001) docker     (123)     1146 2023-05-11 22:32:44.000000 pyclean-2.7.2/tests/test_package.py
--rw-r--r--   0 runner    (1001) docker     (123)     1968 2023-05-11 22:32:44.000000 pyclean-2.7.2/tests/test_version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 21:02:45.665949 pyclean-2.7.3/
+-rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-05-21 21:02:31.000000 pyclean-2.7.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       35 2023-05-21 21:02:31.000000 pyclean-2.7.3/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     9142 2023-05-21 21:02:45.665949 pyclean-2.7.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     7903 2023-05-21 21:02:31.000000 pyclean-2.7.3/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 21:02:45.665949 pyclean-2.7.3/pyclean/
+-rw-r--r--   0 runner    (1001) docker     (123)       98 2023-05-21 21:02:31.000000 pyclean-2.7.3/pyclean/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      139 2023-05-21 21:02:31.000000 pyclean-2.7.3/pyclean/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4741 2023-05-21 21:02:31.000000 pyclean-2.7.3/pyclean/cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1153 2023-05-21 21:02:31.000000 pyclean-2.7.3/pyclean/compat.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7302 2023-05-21 21:02:31.000000 pyclean-2.7.3/pyclean/modern.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2541 2023-05-21 21:02:31.000000 pyclean-2.7.3/pyclean/py2clean.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6132 2023-05-21 21:02:31.000000 pyclean-2.7.3/pyclean/py3clean.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6209 2023-05-21 21:02:31.000000 pyclean-2.7.3/pyclean/pypyclean.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 21:02:45.665949 pyclean-2.7.3/pyclean.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     9142 2023-05-21 21:02:45.000000 pyclean-2.7.3/pyclean.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      492 2023-05-21 21:02:45.000000 pyclean-2.7.3/pyclean.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-21 21:02:45.000000 pyclean-2.7.3/pyclean.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      143 2023-05-21 21:02:45.000000 pyclean-2.7.3/pyclean.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-05-21 21:02:45.000000 pyclean-2.7.3/pyclean.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      678 2023-05-21 21:02:31.000000 pyclean-2.7.3/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-21 21:02:45.665949 pyclean-2.7.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1982 2023-05-21 21:02:31.000000 pyclean-2.7.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 21:02:45.665949 pyclean-2.7.3/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     7254 2023-05-21 21:02:31.000000 pyclean-2.7.3/tests/test_cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1159 2023-05-21 21:02:31.000000 pyclean-2.7.3/tests/test_compat.py
+-rw-r--r--   0 runner    (1001) docker     (123)      434 2023-05-21 21:02:31.000000 pyclean-2.7.3/tests/test_directory.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11983 2023-05-21 21:02:31.000000 pyclean-2.7.3/tests/test_modern.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1146 2023-05-21 21:02:31.000000 pyclean-2.7.3/tests/test_package.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1968 2023-05-21 21:02:31.000000 pyclean-2.7.3/tests/test_version.py
```

### Comparing `pyclean-2.7.2/LICENSE` & `pyclean-2.7.3/LICENSE`

 * *Files identical despite different names*

### Comparing `pyclean-2.7.2/PKG-INFO` & `pyclean-2.7.3/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 Metadata-Version: 2.1
 Name: pyclean
-Version: 2.7.2
+Version: 2.7.3
 Summary: Pure Python cross-platform pyclean. Clean up your Python bytecode.
 Home-page: https://github.com/bittner/pyclean
 Author: Peter Bittner
 Author-email: django@bittner.it
+License: GPL-3.0-or-later
 Keywords: python,bytecode,cli,tools
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 2
 Classifier: Programming Language :: Python :: 2.7
@@ -162,14 +163,15 @@
 Python bytecode. The following topics are currently covered:
 
 - Cache (general purpose folder for several tools, e.g. Python eggs, legacy Pytest)
 - Coverage (coverage database, and supported file formats)
 - Packaging (build files and folders)
 - Pytest (build files and folders)
 - Jupyter (notebook checkpoints) – *optional*
+- Mypy (mypy cache folder) – *optional*
 - Tox (tox environments) – *optional*
 
 *Example:* Dry-run a cleanup of bytecode and tool debris in verbose mode
 (to see what would be deleted):
 
 .. code:: console
```

### Comparing `pyclean-2.7.2/README.rst` & `pyclean-2.7.3/README.rst`

 * *Files 0% similar despite different names*

```diff
@@ -134,14 +134,15 @@
 Python bytecode. The following topics are currently covered:
 
 - Cache (general purpose folder for several tools, e.g. Python eggs, legacy Pytest)
 - Coverage (coverage database, and supported file formats)
 - Packaging (build files and folders)
 - Pytest (build files and folders)
 - Jupyter (notebook checkpoints) – *optional*
+- Mypy (mypy cache folder) – *optional*
 - Tox (tox environments) – *optional*
 
 *Example:* Dry-run a cleanup of bytecode and tool debris in verbose mode
 (to see what would be deleted):
 
 .. code:: console
```

### Comparing `pyclean-2.7.2/pyclean/cli.py` & `pyclean-2.7.3/pyclean/cli.py`

 * *Files 4% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 
 
 def parse_arguments():
     """
     Parse and handle CLI arguments
     """
     debris_default_topics = ['cache', 'coverage', 'package', 'pytest']
-    debris_optional_topics = ['jupyter', 'tox']
+    debris_optional_topics = ['jupyter', 'mypy', 'tox']
     debris_choices = ['all'] + debris_default_topics + debris_optional_topics
     ignore_default_items = ['.git', '.hg', '.svn', '.tox', '.venv', 'node_modules']
 
     parser = argparse.ArgumentParser(
         description='Remove byte-compiled files for a package or project.',
     )
```

### Comparing `pyclean-2.7.2/pyclean/compat.py` & `pyclean-2.7.3/pyclean/compat.py`

 * *Files identical despite different names*

### Comparing `pyclean-2.7.2/pyclean/modern.py` & `pyclean-2.7.3/pyclean/modern.py`

 * *Files 2% similar despite different names*

```diff
@@ -24,14 +24,18 @@
         'htmlcov/**/*',
         'htmlcov/',
     ],
     'jupyter': [
         '.ipynb_checkpoints/**/*',
         '.ipynb_checkpoints/',
     ],
+    'mypy': [
+        '.mypy_cache/**/*',
+        '.mypy_cache/',
+    ],
     'package': [
         'build/bdist.*/**/*',
         'build/bdist.*/',
         'build/lib/**/*',
         'build/lib/',
         'build/',
         'dist/**/*',
```

### Comparing `pyclean-2.7.2/pyclean/py2clean.py` & `pyclean-2.7.3/pyclean/py2clean.py`

 * *Files identical despite different names*

### Comparing `pyclean-2.7.2/pyclean/py3clean.py` & `pyclean-2.7.3/pyclean/py3clean.py`

 * *Files identical despite different names*

### Comparing `pyclean-2.7.2/pyclean/pypyclean.py` & `pyclean-2.7.3/pyclean/pypyclean.py`

 * *Files identical despite different names*

### Comparing `pyclean-2.7.2/pyclean.egg-info/PKG-INFO` & `pyclean-2.7.3/pyclean.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 Metadata-Version: 2.1
 Name: pyclean
-Version: 2.7.2
+Version: 2.7.3
 Summary: Pure Python cross-platform pyclean. Clean up your Python bytecode.
 Home-page: https://github.com/bittner/pyclean
 Author: Peter Bittner
 Author-email: django@bittner.it
+License: GPL-3.0-or-later
 Keywords: python,bytecode,cli,tools
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 2
 Classifier: Programming Language :: Python :: 2.7
@@ -162,14 +163,15 @@
 Python bytecode. The following topics are currently covered:
 
 - Cache (general purpose folder for several tools, e.g. Python eggs, legacy Pytest)
 - Coverage (coverage database, and supported file formats)
 - Packaging (build files and folders)
 - Pytest (build files and folders)
 - Jupyter (notebook checkpoints) – *optional*
+- Mypy (mypy cache folder) – *optional*
 - Tox (tox environments) – *optional*
 
 *Example:* Dry-run a cleanup of bytecode and tool debris in verbose mode
 (to see what would be deleted):
 
 .. code:: console
```

### Comparing `pyclean-2.7.2/pyproject.toml` & `pyclean-2.7.3/pyproject.toml`

 * *Files identical despite different names*

### Comparing `pyclean-2.7.2/setup.py` & `pyclean-2.7.3/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -22,14 +22,15 @@
     author_email='django@bittner.it',
     description=package.__doc__.strip(),
     long_description=read_file('README.rst'),
     long_description_content_type='text/x-rst',
     url='https://github.com/bittner/pyclean',
     packages=find_packages(exclude=['test*']),
     include_package_data=True,
+    license='GPL-3.0-or-later',
     keywords=['python', 'bytecode', 'cli', 'tools'],
     classifiers=[
         'Development Status :: 5 - Production/Stable',
         'Intended Audience :: Developers',
         'License :: OSI Approved :: GNU General Public License v3 (GPLv3)',
         'Programming Language :: Python',
         'Programming Language :: Python :: 2',
```

### Comparing `pyclean-2.7.2/tests/test_cli.py` & `pyclean-2.7.3/tests/test_cli.py`

 * *Files 2% similar despite different names*

```diff
@@ -162,15 +162,23 @@
 def test_debris_all():
     """
     Does calling `pyclean --debris all` pick all topics?
     """
     with ArgvContext('pyclean', 'foo', '--debris', 'all'):
         args = pyclean.cli.parse_arguments()
 
-    assert args.debris == ['cache', 'coverage', 'package', 'pytest', 'jupyter', 'tox']
+    assert args.debris == [
+        'cache',
+        'coverage',
+        'package',
+        'pytest',
+        'jupyter',
+        'mypy',
+        'tox',
+    ]
 
 
 def test_debris_explicit_args():
     """
     Does calling `pyclean --debris` with explicit arguments provide those?
     """
     with ArgvContext('pyclean', 'foo', '--debris', 'package', 'pytest'):
```

### Comparing `pyclean-2.7.2/tests/test_compat.py` & `pyclean-2.7.3/tests/test_compat.py`

 * *Files identical despite different names*

### Comparing `pyclean-2.7.2/tests/test_modern.py` & `pyclean-2.7.3/tests/test_modern.py`

 * *Files 3% similar despite different names*

```diff
@@ -248,14 +248,15 @@
 
 @pytest.mark.parametrize(
     'options,scanned_topics',
     [
         ([], []),
         (['-d'], ['cache', 'coverage', 'package', 'pytest']),
         (['-d', 'coverage', 'package'], ['coverage', 'package']),
+        (['-d', 'jupyter', 'mypy', 'tox'], ['jupyter', 'mypy', 'tox']),
     ]
 )
 @patch('pyclean.modern.remove_freeform_targets')
 @patch('pyclean.modern.remove_debris_for')
 @patch('pyclean.modern.descend_and_clean')
 def test_debris_option(mock_descend, mock_debris, mock_erase, options, scanned_topics):
     """
@@ -284,27 +285,38 @@
     erase_calls = [call_args[0][0] for call_args in mock_erase.call_args_list]
 
     assert mock_descend.called
     assert not mock_debris.called
     assert erase_calls == [['tmp/**/*', 'tmp/']]
 
 
+@pytest.mark.parametrize(
+    'debris_topic',
+    [
+        'cache',
+        'coverage',
+        'package',
+        'pytest',
+        'jupyter',
+        'mypy',
+        'tox',
+    ]
+)
 @patch('pyclean.modern.delete_filesystem_objects')
-def test_debris_loop(mock_delete_fs_obj):
+def test_debris_loop(mock_delete_fs_obj, debris_topic):
     """
     Does ``remove_debris_for()`` call filesystem object removal?
     """
-    pyclean.modern.DEBRIS_TOPICS = {'foo': ['somedir/']}
+    fileobject_globs = pyclean.modern.DEBRIS_TOPICS[debris_topic]
     directory = Path('.')
+    expected_calls = [call(directory, pattern) for pattern in fileobject_globs]
 
-    remove_debris_for('foo', directory)
+    remove_debris_for(debris_topic, directory)
 
-    assert mock_delete_fs_obj.call_args_list == [
-        call(directory, 'somedir/'),
-    ]
+    assert mock_delete_fs_obj.call_args_list == expected_calls
 
 
 @patch('pyclean.modern.delete_filesystem_objects')
 def test_erase_loop(mock_delete_fs_obj):
     """
     Does ``remove_freeform_targets()`` call filesystem object removal?
     """
```

### Comparing `pyclean-2.7.2/tests/test_package.py` & `pyclean-2.7.3/tests/test_package.py`

 * *Files identical despite different names*

### Comparing `pyclean-2.7.2/tests/test_version.py` & `pyclean-2.7.3/tests/test_version.py`

 * *Files identical despite different names*

