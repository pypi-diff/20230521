# Comparing `tmp/rdkit_to_params-1.2.3.tar.gz` & `tmp/rdkit_to_params-1.2.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rdkit_to_params-1.2.3.tar", last modified: Mon Jan  9 16:35:32 2023, max compression
+gzip compressed data, was "rdkit_to_params-1.2.4.tar", last modified: Sun May 21 16:16:33 2023, max compression
```

## Comparing `rdkit_to_params-1.2.3.tar` & `rdkit_to_params-1.2.4.tar`

### file list

```diff
@@ -1,31 +1,31 @@
-drwxr-xr-x   0 matteo     (502) staff       (20)        0 2023-01-09 16:35:32.501210 rdkit_to_params-1.2.3/
--rw-r--r--   0 matteo     (502) staff       (20)     1069 2023-01-09 15:32:57.000000 rdkit_to_params-1.2.3/LICENSE
--rw-r--r--   0 matteo     (502) staff       (20)    18155 2023-01-09 16:35:32.499680 rdkit_to_params-1.2.3/PKG-INFO
--rw-r--r--   0 matteo     (502) staff       (20)    17342 2023-01-09 15:32:57.000000 rdkit_to_params-1.2.3/README.md
-drwxr-xr-x   0 matteo     (502) staff       (20)        0 2023-01-09 16:35:32.459335 rdkit_to_params-1.2.3/rdkit_to_params/
--rw-r--r--   0 matteo     (502) staff       (20)    17168 2023-01-09 15:32:57.000000 rdkit_to_params-1.2.3/rdkit_to_params/__init__.py
--rw-r--r--   0 matteo     (502) staff       (20)     3120 2023-01-09 15:32:57.000000 rdkit_to_params-1.2.3/rdkit_to_params/_init_mixin.py
--rw-r--r--   0 matteo     (502) staff       (20)     3945 2023-01-09 15:32:57.000000 rdkit_to_params-1.2.3/rdkit_to_params/_io_mixin.py
--rw-r--r--   0 matteo     (502) staff       (20)     3827 2023-01-09 15:32:57.000000 rdkit_to_params-1.2.3/rdkit_to_params/_pyrosetta_mixin.py
-drwxr-xr-x   0 matteo     (502) staff       (20)        0 2023-01-09 16:35:32.468415 rdkit_to_params-1.2.3/rdkit_to_params/cli/
--rw-r--r--   0 matteo     (502) staff       (20)     1114 2023-01-09 15:32:57.000000 rdkit_to_params-1.2.3/rdkit_to_params/cli/__init__.py
--rw-r--r--   0 matteo     (502) staff       (20)    17294 2023-01-09 15:51:42.000000 rdkit_to_params-1.2.3/rdkit_to_params/constraint.py
--rw-r--r--   0 matteo     (502) staff       (20)    23873 2023-01-09 15:32:57.000000 rdkit_to_params-1.2.3/rdkit_to_params/entries.py
-drwxr-xr-x   0 matteo     (502) staff       (20)        0 2023-01-09 16:35:32.491738 rdkit_to_params-1.2.3/rdkit_to_params/rdkitside/
--rw-r--r--   0 matteo     (502) staff       (20)      877 2023-01-09 15:32:57.000000 rdkit_to_params-1.2.3/rdkit_to_params/rdkitside/__init__.py
--rw-r--r--   0 matteo     (502) staff       (20)    22103 2023-01-09 15:51:42.000000 rdkit_to_params-1.2.3/rdkit_to_params/rdkitside/_rdkit_convert.py
--rw-r--r--   0 matteo     (502) staff       (20)     6316 2023-01-09 15:32:57.000000 rdkit_to_params-1.2.3/rdkit_to_params/rdkitside/_rdkit_inits.py
--rw-r--r--   0 matteo     (502) staff       (20)    31173 2023-01-09 15:51:42.000000 rdkit_to_params-1.2.3/rdkit_to_params/rdkitside/_rdkit_prep.py
--rw-r--r--   0 matteo     (502) staff       (20)     9736 2023-01-09 15:32:57.000000 rdkit_to_params-1.2.3/rdkit_to_params/rdkitside/_rdkit_rename.py
--rw-r--r--   0 matteo     (502) staff       (20)     3695 2023-01-09 15:32:57.000000 rdkit_to_params-1.2.3/rdkit_to_params/rdkitside/utilities.py
--rw-r--r--   0 matteo     (502) staff       (20)      217 2023-01-09 16:34:47.000000 rdkit_to_params-1.2.3/rdkit_to_params/version.py
-drwxr-xr-x   0 matteo     (502) staff       (20)        0 2023-01-09 16:35:32.467682 rdkit_to_params-1.2.3/rdkit_to_params.egg-info/
--rw-r--r--   0 matteo     (502) staff       (20)    18155 2023-01-09 16:35:32.000000 rdkit_to_params-1.2.3/rdkit_to_params.egg-info/PKG-INFO
--rw-r--r--   0 matteo     (502) staff       (20)      729 2023-01-09 16:35:32.000000 rdkit_to_params-1.2.3/rdkit_to_params.egg-info/SOURCES.txt
--rw-r--r--   0 matteo     (502) staff       (20)        1 2023-01-09 16:35:32.000000 rdkit_to_params-1.2.3/rdkit_to_params.egg-info/dependency_links.txt
--rw-r--r--   0 matteo     (502) staff       (20)       64 2023-01-09 16:35:32.000000 rdkit_to_params-1.2.3/rdkit_to_params.egg-info/entry_points.txt
--rw-r--r--   0 matteo     (502) staff       (20)       22 2023-01-09 16:35:32.000000 rdkit_to_params-1.2.3/rdkit_to_params.egg-info/top_level.txt
--rw-r--r--   0 matteo     (502) staff       (20)       38 2023-01-09 16:35:32.501533 rdkit_to_params-1.2.3/setup.cfg
--rw-r--r--   0 matteo     (502) staff       (20)     3080 2023-01-09 16:34:47.000000 rdkit_to_params-1.2.3/setup.py
-drwxr-xr-x   0 matteo     (502) staff       (20)        0 2023-01-09 16:35:32.495349 rdkit_to_params-1.2.3/tests/
--rw-r--r--   0 matteo     (502) staff       (20)     1617 2023-01-09 16:05:14.000000 rdkit_to_params-1.2.3/tests/__init__.py
+drwxr-xr-x   0 user       (502) staff       (20)        0 2023-05-21 16:16:33.329975 rdkit_to_params-1.2.4/
+-rw-r--r--   0 user       (502) staff       (20)     1069 2023-05-21 13:24:25.000000 rdkit_to_params-1.2.4/LICENSE
+-rw-r--r--   0 user       (502) staff       (20)    18257 2023-05-21 16:16:33.329233 rdkit_to_params-1.2.4/PKG-INFO
+-rw-r--r--   0 user       (502) staff       (20)    17342 2023-05-21 13:24:25.000000 rdkit_to_params-1.2.4/README.md
+drwxr-xr-x   0 user       (502) staff       (20)        0 2023-05-21 16:16:33.307039 rdkit_to_params-1.2.4/rdkit_to_params/
+-rw-r--r--   0 user       (502) staff       (20)    17168 2023-05-21 13:24:25.000000 rdkit_to_params-1.2.4/rdkit_to_params/__init__.py
+-rw-r--r--   0 user       (502) staff       (20)     3120 2023-05-21 13:24:25.000000 rdkit_to_params-1.2.4/rdkit_to_params/_init_mixin.py
+-rw-r--r--   0 user       (502) staff       (20)     3945 2023-05-21 13:24:25.000000 rdkit_to_params-1.2.4/rdkit_to_params/_io_mixin.py
+-rw-r--r--   0 user       (502) staff       (20)     3827 2023-05-21 13:24:25.000000 rdkit_to_params-1.2.4/rdkit_to_params/_pyrosetta_mixin.py
+drwxr-xr-x   0 user       (502) staff       (20)        0 2023-05-21 16:16:33.315839 rdkit_to_params-1.2.4/rdkit_to_params/cli/
+-rw-r--r--   0 user       (502) staff       (20)     1114 2023-05-21 13:24:25.000000 rdkit_to_params-1.2.4/rdkit_to_params/cli/__init__.py
+-rw-r--r--   0 user       (502) staff       (20)    17294 2023-05-21 13:24:25.000000 rdkit_to_params-1.2.4/rdkit_to_params/constraint.py
+-rw-r--r--   0 user       (502) staff       (20)    23873 2023-05-21 13:24:25.000000 rdkit_to_params-1.2.4/rdkit_to_params/entries.py
+drwxr-xr-x   0 user       (502) staff       (20)        0 2023-05-21 16:16:33.327493 rdkit_to_params-1.2.4/rdkit_to_params/rdkitside/
+-rw-r--r--   0 user       (502) staff       (20)      877 2023-05-21 13:24:25.000000 rdkit_to_params-1.2.4/rdkit_to_params/rdkitside/__init__.py
+-rw-r--r--   0 user       (502) staff       (20)    22111 2023-05-21 16:12:20.000000 rdkit_to_params-1.2.4/rdkit_to_params/rdkitside/_rdkit_convert.py
+-rw-r--r--   0 user       (502) staff       (20)     6316 2023-05-21 13:24:25.000000 rdkit_to_params-1.2.4/rdkit_to_params/rdkitside/_rdkit_inits.py
+-rw-r--r--   0 user       (502) staff       (20)    31173 2023-05-21 14:07:44.000000 rdkit_to_params-1.2.4/rdkit_to_params/rdkitside/_rdkit_prep.py
+-rw-r--r--   0 user       (502) staff       (20)     9736 2023-05-21 13:24:25.000000 rdkit_to_params-1.2.4/rdkit_to_params/rdkitside/_rdkit_rename.py
+-rw-r--r--   0 user       (502) staff       (20)     3695 2023-05-21 13:24:25.000000 rdkit_to_params-1.2.4/rdkit_to_params/rdkitside/utilities.py
+-rw-r--r--   0 user       (502) staff       (20)      217 2023-05-21 16:15:44.000000 rdkit_to_params-1.2.4/rdkit_to_params/version.py
+drwxr-xr-x   0 user       (502) staff       (20)        0 2023-05-21 16:16:33.313614 rdkit_to_params-1.2.4/rdkit_to_params.egg-info/
+-rw-r--r--   0 user       (502) staff       (20)    18257 2023-05-21 16:16:33.000000 rdkit_to_params-1.2.4/rdkit_to_params.egg-info/PKG-INFO
+-rw-r--r--   0 user       (502) staff       (20)      729 2023-05-21 16:16:33.000000 rdkit_to_params-1.2.4/rdkit_to_params.egg-info/SOURCES.txt
+-rw-r--r--   0 user       (502) staff       (20)        1 2023-05-21 16:16:33.000000 rdkit_to_params-1.2.4/rdkit_to_params.egg-info/dependency_links.txt
+-rw-r--r--   0 user       (502) staff       (20)       64 2023-05-21 16:16:33.000000 rdkit_to_params-1.2.4/rdkit_to_params.egg-info/entry_points.txt
+-rw-r--r--   0 user       (502) staff       (20)       22 2023-05-21 16:16:33.000000 rdkit_to_params-1.2.4/rdkit_to_params.egg-info/top_level.txt
+-rw-r--r--   0 user       (502) staff       (20)       38 2023-05-21 16:16:33.330109 rdkit_to_params-1.2.4/setup.cfg
+-rw-r--r--   0 user       (502) staff       (20)     2802 2023-05-21 16:15:44.000000 rdkit_to_params-1.2.4/setup.py
+drwxr-xr-x   0 user       (502) staff       (20)        0 2023-05-21 16:16:33.328262 rdkit_to_params-1.2.4/tests/
+-rw-r--r--   0 user       (502) staff       (20)     1644 2023-05-21 14:06:49.000000 rdkit_to_params-1.2.4/tests/__init__.py
```

### Comparing `rdkit_to_params-1.2.3/LICENSE` & `rdkit_to_params-1.2.4/LICENSE`

 * *Files identical despite different names*

### Comparing `rdkit_to_params-1.2.3/PKG-INFO` & `rdkit_to_params-1.2.4/rdkit_to_params.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,23 +1,25 @@
 Metadata-Version: 2.1
-Name: rdkit_to_params
-Version: 1.2.3
+Name: rdkit-to-params
+Version: 1.2.4
 Summary: Create or modify Rosetta params files (topology files) from scratch, RDKit mols or another params file.
 Home-page: https://github.com/matteoferla/rdkit_to_params
 Author: Matteo Ferla
 Author-email: matteo.ferla@gmail.com
 License: MIT
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Science/Research
 Classifier: Topic :: Scientific/Engineering :: Bio-Informatics
 Classifier: Topic :: Scientific/Engineering :: Chemistry
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Requires-Python: >3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # RDKit to params
 Create or modify Rosetta params files (topology files) from scratch, RDKit mols or another params file.
```

### Comparing `rdkit_to_params-1.2.3/README.md` & `rdkit_to_params-1.2.4/README.md`

 * *Files identical despite different names*

### Comparing `rdkit_to_params-1.2.3/rdkit_to_params/__init__.py` & `rdkit_to_params-1.2.4/rdkit_to_params/__init__.py`

 * *Files identical despite different names*

### Comparing `rdkit_to_params-1.2.3/rdkit_to_params/_init_mixin.py` & `rdkit_to_params-1.2.4/rdkit_to_params/_init_mixin.py`

 * *Files identical despite different names*

### Comparing `rdkit_to_params-1.2.3/rdkit_to_params/_io_mixin.py` & `rdkit_to_params-1.2.4/rdkit_to_params/_io_mixin.py`

 * *Files identical despite different names*

### Comparing `rdkit_to_params-1.2.3/rdkit_to_params/_pyrosetta_mixin.py` & `rdkit_to_params-1.2.4/rdkit_to_params/_pyrosetta_mixin.py`

 * *Files identical despite different names*

### Comparing `rdkit_to_params-1.2.3/rdkit_to_params/cli/__init__.py` & `rdkit_to_params-1.2.4/rdkit_to_params/cli/__init__.py`

 * *Files identical despite different names*

### Comparing `rdkit_to_params-1.2.3/rdkit_to_params/constraint.py` & `rdkit_to_params-1.2.4/rdkit_to_params/constraint.py`

 * *Files identical despite different names*

### Comparing `rdkit_to_params-1.2.3/rdkit_to_params/entries.py` & `rdkit_to_params-1.2.4/rdkit_to_params/entries.py`

 * *Files identical despite different names*

### Comparing `rdkit_to_params-1.2.3/rdkit_to_params/rdkitside/__init__.py` & `rdkit_to_params-1.2.4/rdkit_to_params/rdkitside/__init__.py`

 * *Files identical despite different names*

### Comparing `rdkit_to_params-1.2.3/rdkit_to_params/rdkitside/_rdkit_convert.py` & `rdkit_to_params-1.2.4/rdkit_to_params/rdkitside/_rdkit_convert.py`

 * *Files 1% similar despite different names*

```diff
@@ -55,15 +55,15 @@
         # SMILES
         self.comments.append(Chem.MolToSmiles(self.mol))
         if len(self.TYPE) == 0:
             self.TYPE.append('LIGAND')
         # remove all previous entries.
         for attr_name in Entries.choices:
             # do not blank these:
-            if attr_name in ['#', 'comment','IO_STRING', 'ROTAMER_AA', 'AA', 'PROPERTIES', 'VARIANT', '<UNKNOWN>']:
+            if attr_name in ['#', 'TYPE', 'comment','IO_STRING', 'ROTAMER_AA', 'AA', 'PROPERTIES', 'VARIANT', '<UNKNOWN>']:
                 continue
             elif not hasattr(self, attr_name):
                 continue
             else:
                 getattr(self, attr_name).clear()
         # correct for ions
         if self.mol.GetNumAtoms() >= 3:
```

### Comparing `rdkit_to_params-1.2.3/rdkit_to_params/rdkitside/_rdkit_inits.py` & `rdkit_to_params-1.2.4/rdkit_to_params/rdkitside/_rdkit_inits.py`

 * *Files identical despite different names*

### Comparing `rdkit_to_params-1.2.3/rdkit_to_params/rdkitside/_rdkit_prep.py` & `rdkit_to_params-1.2.4/rdkit_to_params/rdkitside/_rdkit_prep.py`

 * *Files identical despite different names*

### Comparing `rdkit_to_params-1.2.3/rdkit_to_params/rdkitside/_rdkit_rename.py` & `rdkit_to_params-1.2.4/rdkit_to_params/rdkitside/_rdkit_rename.py`

 * *Files identical despite different names*

### Comparing `rdkit_to_params-1.2.3/rdkit_to_params/rdkitside/utilities.py` & `rdkit_to_params-1.2.4/rdkit_to_params/rdkitside/utilities.py`

 * *Files identical despite different names*

### Comparing `rdkit_to_params-1.2.3/rdkit_to_params.egg-info/PKG-INFO` & `rdkit_to_params-1.2.4/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,23 +1,25 @@
 Metadata-Version: 2.1
-Name: rdkit-to-params
-Version: 1.2.3
+Name: rdkit_to_params
+Version: 1.2.4
 Summary: Create or modify Rosetta params files (topology files) from scratch, RDKit mols or another params file.
 Home-page: https://github.com/matteoferla/rdkit_to_params
 Author: Matteo Ferla
 Author-email: matteo.ferla@gmail.com
 License: MIT
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Science/Research
 Classifier: Topic :: Scientific/Engineering :: Bio-Informatics
 Classifier: Topic :: Scientific/Engineering :: Chemistry
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Requires-Python: >3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # RDKit to params
 Create or modify Rosetta params files (topology files) from scratch, RDKit mols or another params file.
```

### Comparing `rdkit_to_params-1.2.3/rdkit_to_params.egg-info/SOURCES.txt` & `rdkit_to_params-1.2.4/rdkit_to_params.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `rdkit_to_params-1.2.3/setup.py` & `rdkit_to_params-1.2.4/setup.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 ########################################################################################################################
 __doc__ = 'README.md'
 __author__ = "Matteo Ferla"
 __url__ = "https://github.com/matteoferla/rdkit_to_params"
 __email__ = "matteo.ferla@gmail.com"
 __date__ = "29 January 2021 A.D."
 __license__ = "MIT"
-__version__ = "1.2.3"
+__version__ = "1.2.4"
 __citation__ = "https://advances.sciencemag.org/content/7/16/eabf8711 (Fragmenstein)"
 
 # ---------- imports  --------------------------------------------------------------------------------------------------
 # remember it's `python setup.py sdist` and `python -m twine upload dist/rdkit_to_params-1.0.5.tar.gz`
 
 from setuptools import setup, find_packages
 from warnings import warn
@@ -23,22 +23,14 @@
 else:
     long_description = __doc__
 
 description = 'Create or modify Rosetta params files (topology files) from scratch, RDKit mols or another params file.'
 
 # ---------- Non pip modules  ------------------------------------------------------------------------------------------
 
-if not util.find_spec('rdkit'):
-    warn('Albeit optional, a lot of this code relies on rdkit which cannot be pip installed.' +
-               'To install try either ' +
-               'conda install -c conda-forge rdkit or ' +
-               'sudo apt-get/brew install python3-rdkit or visit rdkit documentation.' +
-         'or use the new pip install rdkit-pypi'
-         )
-
 if not util.find_spec('pyrosetta'):
     warn('The minimisation part of this code uses pyrosetta, which has to be downloaded from ' +
          'the Rosetta software site due to licencing. Without it only the classes Monster and Rectifier will work')
 
 # ---------- setuptools.setup ------------------------------------------------------------------------------------------
 
 setup(
@@ -64,9 +56,11 @@
         'Intended Audience :: Science/Research',
         'Topic :: Scientific/Engineering :: Bio-Informatics',
         'Topic :: Scientific/Engineering :: Chemistry',
         'License :: OSI Approved :: MIT License',
         'Programming Language :: Python :: 3.7',
         'Programming Language :: Python :: 3.8',
         'Programming Language :: Python :: 3.9',
+        'Programming Language :: Python :: 3.10',
+        'Programming Language :: Python :: 3.11',
     ],
 )
```

### Comparing `rdkit_to_params-1.2.3/tests/__init__.py` & `rdkit_to_params-1.2.4/tests/__init__.py`

 * *Files 16% similar despite different names*

```diff
@@ -21,19 +21,19 @@
         pose = p.test()
         buffer = pyrosetta.rosetta.std.stringbuf()
         pose.dump_pdb(pyrosetta.rosetta.std.ostream(buffer))
         pdbblock = buffer.str()
         self.assertIsNotNone(Chem.MolFromPDBBlock(pdbblock))
 
     def test_aa_smiles(self):
-        p = Params.from_smiles('*OC(=O)C(Cc1ccccc1)N*',  # recognised as amino acid.
+        p = Params.from_smiles('*C(=O)C(Cc1ccccc1)N*',  # recognised as amino acid.
                                name='PHX',  # optional.
                                # atomnames={4: 'CZ'}  # optional, rando atom name for CB
                                )
-        self.assertTrue(p.is_aminoacid())
+        self.assertTrue(p.is_aminoacid(), 'Should be an amino acid.')
 
     def test_renames(self):
         p = Params.from_smiles('CC(ONC)O', atomnames=['CA', 'CB', 'OX', 'ON', 'CX', 'CG'])
         p.rename_atom_by_name('CA', 'CZ')
         self.assertEqual(p.mol.GetAtomWithIdx(0).GetPDBResidueInfo().GetName(), ' CZ ')
         self.assertEqual(p.ATOM[0].name, ' CZ ')
         p.test()
```

