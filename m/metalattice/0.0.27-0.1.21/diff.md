# Comparing `tmp/metalattice-0.0.27.tar.gz` & `tmp/metalattice-0.1.21.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "metalattice-0.0.27.tar", last modified: Sun May 21 17:46:39 2023, max compression
+gzip compressed data, was "metalattice-0.1.21.tar", last modified: Wed May 17 07:43:07 2023, max compression
```

## Comparing `metalattice-0.0.27.tar` & `metalattice-0.1.21.tar`

### file list

```diff
@@ -1,49 +1,25 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 17:46:39.294357 metalattice-0.0.27/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 17:46:39.286357 metalattice-0.0.27/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 17:46:39.290357 metalattice-0.0.27/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)     1342 2023-05-21 17:46:28.000000 metalattice-0.0.27/.github/workflows/python-package.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1078 2023-05-21 17:46:28.000000 metalattice-0.0.27/.github/workflows/python-publish.yml
--rw-r--r--   0 runner    (1001) docker     (123)    11071 2023-05-21 17:46:28.000000 metalattice-0.0.27/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)     1082 2023-05-21 17:46:28.000000 metalattice-0.0.27/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     1753 2023-05-21 17:46:39.294357 metalattice-0.0.27/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)       77 2023-05-21 17:46:28.000000 metalattice-0.0.27/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      748 2023-05-21 17:46:28.000000 metalattice-0.0.27/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-21 17:46:39.294357 metalattice-0.0.27/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 17:46:39.286357 metalattice-0.0.27/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 17:46:39.290357 metalattice-0.0.27/src/metalattice/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-21 17:46:28.000000 metalattice-0.0.27/src/metalattice/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      162 2023-05-21 17:46:39.000000 metalattice-0.0.27/src/metalattice/_version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 17:46:39.290357 metalattice-0.0.27/src/metalattice/abaqus/
--rw-r--r--   0 runner    (1001) docker     (123)      131 2023-05-21 17:46:28.000000 metalattice-0.0.27/src/metalattice/abaqus/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 17:46:39.290357 metalattice-0.0.27/src/metalattice/abaqus/fortran/
--rw-r--r--   0 runner    (1001) docker     (123)     1206 2023-05-21 17:46:28.000000 metalattice-0.0.27/src/metalattice/abaqus/fortran/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 17:46:39.290357 metalattice-0.0.27/src/metalattice/abaqus/fortran/code/
--rw-r--r--   0 runner    (1001) docker     (123)     3069 2023-05-21 17:46:28.000000 metalattice-0.0.27/src/metalattice/abaqus/fortran/code/custom_lattice.f
--rw-r--r--   0 runner    (1001) docker     (123)     3384 2023-05-21 17:46:28.000000 metalattice-0.0.27/src/metalattice/abaqus/fortran/code/cylin_lattice.f
--rw-r--r--   0 runner    (1001) docker     (123)     6585 2023-05-21 17:46:28.000000 metalattice-0.0.27/src/metalattice/abaqus/fortran/code/kshape20h.f
--rw-r--r--   0 runner    (1001) docker     (123)     4123 2023-05-21 17:46:28.000000 metalattice-0.0.27/src/metalattice/abaqus/fortran/code/kshape8h.f
--rw-r--r--   0 runner    (1001) docker     (123)     8304 2023-05-21 17:46:28.000000 metalattice-0.0.27/src/metalattice/abaqus/fortran/code/lattice.f
--rw-r--r--   0 runner    (1001) docker     (123)     5537 2023-05-21 17:46:28.000000 metalattice-0.0.27/src/metalattice/abaqus/fortran/code/mpc3d.f
--rw-r--r--   0 runner    (1001) docker     (123)      227 2023-05-21 17:46:28.000000 metalattice-0.0.27/src/metalattice/abaqus/fortran/code/namelist_element.f
--rw-r--r--   0 runner    (1001) docker     (123)      130 2023-05-21 17:46:28.000000 metalattice-0.0.27/src/metalattice/abaqus/fortran/code/namelist_info.f
--rw-r--r--   0 runner    (1001) docker     (123)     3069 2023-05-21 17:46:28.000000 metalattice-0.0.27/src/metalattice/abaqus/fortran/code/rect_lattice.f
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-21 17:46:28.000000 metalattice-0.0.27/src/metalattice/abaqus/fortran/lib.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 17:46:39.290357 metalattice-0.0.27/src/metalattice/abaqus/scripts/
--rw-r--r--   0 runner    (1001) docker     (123)      473 2023-05-21 17:46:28.000000 metalattice-0.0.27/src/metalattice/abaqus/scripts/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2166 2023-05-21 17:46:28.000000 metalattice-0.0.27/src/metalattice/abaqus/scripts/generate_inp.py
--rw-r--r--   0 runner    (1001) docker     (123)      304 2023-05-21 17:46:28.000000 metalattice-0.0.27/src/metalattice/abaqus/step.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 17:46:39.290357 metalattice-0.0.27/src/metalattice/lattice/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-21 17:46:28.000000 metalattice-0.0.27/src/metalattice/lattice/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    12965 2023-05-21 17:46:28.000000 metalattice-0.0.27/src/metalattice/lattice/lattice.py
--rw-r--r--   0 runner    (1001) docker     (123)      339 2023-05-21 17:46:28.000000 metalattice-0.0.27/src/metalattice/material.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 17:46:39.290357 metalattice-0.0.27/src/metalattice.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1753 2023-05-21 17:46:39.000000 metalattice-0.0.27/src/metalattice.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1262 2023-05-21 17:46:39.000000 metalattice-0.0.27/src/metalattice.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-21 17:46:39.000000 metalattice-0.0.27/src/metalattice.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       29 2023-05-21 17:46:39.000000 metalattice-0.0.27/src/metalattice.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       12 2023-05-21 17:46:39.000000 metalattice-0.0.27/src/metalattice.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 17:46:39.294357 metalattice-0.0.27/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-21 17:46:28.000000 metalattice-0.0.27/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      964 2023-05-21 17:46:28.000000 metalattice-0.0.27/tests/test_lattice_defination.py
--rw-r--r--   0 runner    (1001) docker     (123)      918 2023-05-21 17:46:28.000000 metalattice-0.0.27/tests/test_math_constants.py
--rw-r--r--   0 runner    (1001) docker     (123)     1609 2023-05-21 17:46:28.000000 metalattice-0.0.27/tests/test_output_to_abaqus.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 07:43:07.590173 metalattice-0.1.21/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 07:43:07.586173 metalattice-0.1.21/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 07:43:07.590173 metalattice-0.1.21/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)     1360 2023-05-17 07:42:52.000000 metalattice-0.1.21/.github/workflows/python-package.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1050 2023-05-17 07:42:52.000000 metalattice-0.1.21/.github/workflows/python-publish.yml
+-rw-r--r--   0 runner    (1001) docker     (123)    10467 2023-05-17 07:42:52.000000 metalattice-0.1.21/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)     1082 2023-05-17 07:42:52.000000 metalattice-0.1.21/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     2812 2023-05-17 07:43:07.590173 metalattice-0.1.21/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1175 2023-05-17 07:42:52.000000 metalattice-0.1.21/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      668 2023-05-17 07:42:52.000000 metalattice-0.1.21/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-17 07:42:52.000000 metalattice-0.1.21/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-17 07:43:07.590173 metalattice-0.1.21/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 07:43:07.586173 metalattice-0.1.21/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 07:43:07.590173 metalattice-0.1.21/src/metalattice/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-17 07:42:52.000000 metalattice-0.1.21/src/metalattice/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      162 2023-05-17 07:43:07.000000 metalattice-0.1.21/src/metalattice/_version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 07:43:07.590173 metalattice-0.1.21/src/metalattice.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2812 2023-05-17 07:43:07.000000 metalattice-0.1.21/src/metalattice.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      427 2023-05-17 07:43:07.000000 metalattice-0.1.21/src/metalattice.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-17 07:43:07.000000 metalattice-0.1.21/src/metalattice.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-05-17 07:43:07.000000 metalattice-0.1.21/src/metalattice.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-05-17 07:43:07.000000 metalattice-0.1.21/src/metalattice.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 07:43:07.590173 metalattice-0.1.21/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)       99 2023-05-17 07:42:52.000000 metalattice-0.1.21/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      368 2023-05-17 07:42:52.000000 metalattice-0.1.21/tests/test_import.py
```

### Comparing `metalattice-0.0.27/.github/workflows/python-package.yml` & `metalattice-0.1.21/.github/workflows/python-package.yml`

 * *Files 4% similar despite different names*

```diff
@@ -25,15 +25,16 @@
       with:
         python-version: ${{ matrix.python-version }}
     - name: Install dependencies
       run: |
         python -m pip install --upgrade pip
         python -m pip install flake8 pytest
         if [ -f requirements.txt ]; then pip install -r requirements.txt; fi
-        python -m pip install -e .
+    - name: Build package
+      run: python -m build
     - name: Lint with flake8
       run: |
         # stop the build if there are Python syntax errors or undefined names
         flake8 . --count --select=E9,F63,F7,F82 --show-source --statistics
         # exit-zero treats all errors as warnings. The GitHub editor is 127 chars wide
         flake8 . --count --exit-zero --max-complexity=10 --max-line-length=127 --statistics
     - name: Test with pytest
```

### Comparing `metalattice-0.0.27/.github/workflows/python-publish.yml` & `metalattice-0.1.21/.github/workflows/python-publish.yml`

 * *Files 10% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 # For more information see: https://docs.github.com/en/actions/automating-builds-and-tests/building-and-testing-python#publishing-to-package-registries
 
 # This workflow uses actions that are not certified by GitHub.
 # They are provided by a third-party and are governed by
 # separate terms of service, privacy policy, and support
 # documentation.
 
-name: Publish on PyPI
+name: Upload Python Package
 
 on:
   release:
     types: [published]
 
 permissions:
   contents: read
@@ -29,11 +29,11 @@
     - name: Install dependencies
       run: |
         python -m pip install --upgrade pip
         pip install build
     - name: Build package
       run: python -m build
     - name: Publish package
-      uses: pypa/gh-action-pypi-publish@27b31702a0e7fc50959f5ad993c78deac1bdfc29
+      uses: pypa/gh-action-pypi-publish@master
       with:
         user: __token__
         password: ${{ secrets.PYPI_API_TOKEN }}
```

### Comparing `metalattice-0.0.27/.gitignore` & `metalattice-0.1.21/.gitignore`

 * *Files 19% similar despite different names*

```diff
@@ -1,235 +1,8 @@
-# Created by https://www.toptal.com/developers/gitignore/api/python,fortran,visualstudio,visualstudiocode
-# Edit at https://www.toptal.com/developers/gitignore?templates=python,fortran,visualstudio,visualstudiocode
-
-### Fortran ###
-# Prerequisites
-*.d
-
-# Compiled Object files
-*.slo
-*.lo
-*.o
-*.obj
-
-# Precompiled Headers
-*.gch
-*.pch
-
-# Compiled Dynamic libraries
-*.so
-*.dylib
-*.dll
-
-# Fortran module files
-*.mod
-*.smod
-
-# Compiled Static libraries
-*.lai
-*.la
-*.a
-*.lib
-
-# Executables
-*.exe
-*.out
-*.app
-
-### Python ###
-# Byte-compiled / optimized / DLL files
-__pycache__/
-*.py[cod]
-*$py.class
-
-# C extensions
-
-# Distribution / packaging
-.Python
-build/
-develop-eggs/
-dist/
-downloads/
-eggs/
-.eggs/
-lib/
-lib64/
-parts/
-sdist/
-var/
-wheels/
-share/python-wheels/
-*.egg-info/
-.installed.cfg
-*.egg
-MANIFEST
-
-# PyInstaller
-#  Usually these files are written by a python script from a template
-#  before PyInstaller builds the exe, so as to inject date/other infos into it.
-*.manifest
-*.spec
-
-# Installer logs
-pip-log.txt
-pip-delete-this-directory.txt
-
-# Unit test / coverage reports
-htmlcov/
-.tox/
-.nox/
-.coverage
-.coverage.*
-.cache
-nosetests.xml
-coverage.xml
-*.cover
-*.py,cover
-.hypothesis/
-.pytest_cache/
-cover/
-
-# Translations
-*.mo
-*.pot
-
-# Django stuff:
-*.log
-local_settings.py
-db.sqlite3
-db.sqlite3-journal
-
-# Flask stuff:
-instance/
-.webassets-cache
-
-# Scrapy stuff:
-.scrapy
-
-# Sphinx documentation
-docs/_build/
-
-# PyBuilder
-.pybuilder/
-target/
-
-# Jupyter Notebook
-.ipynb_checkpoints
-
-# IPython
-profile_default/
-ipython_config.py
-
-# pyenv
-#   For a library or package, you might want to ignore these files since the code is
-#   intended to run in multiple environments; otherwise, check them in:
-# .python-version
-
-# pipenv
-#   According to pypa/pipenv#598, it is recommended to include Pipfile.lock in version control.
-#   However, in case of collaboration, if having platform-specific dependencies or dependencies
-#   having no cross-platform support, pipenv may install dependencies that don't work, or not
-#   install all needed dependencies.
-#Pipfile.lock
-
-# poetry
-#   Similar to Pipfile.lock, it is generally recommended to include poetry.lock in version control.
-#   This is especially recommended for binary packages to ensure reproducibility, and is more
-#   commonly ignored for libraries.
-#   https://python-poetry.org/docs/basic-usage/#commit-your-poetrylock-file-to-version-control
-#poetry.lock
-
-# pdm
-#   Similar to Pipfile.lock, it is generally recommended to include pdm.lock in version control.
-#pdm.lock
-#   pdm stores project-wide configurations in .pdm.toml, but it is recommended to not include it
-#   in version control.
-#   https://pdm.fming.dev/#use-with-ide
-.pdm.toml
-
-# PEP 582; used by e.g. github.com/David-OConnor/pyflow and github.com/pdm-project/pdm
-__pypackages__/
-
-# Celery stuff
-celerybeat-schedule
-celerybeat.pid
-
-# SageMath parsed files
-*.sage.py
-
-# Environments
-.env
-.venv
-env/
-venv/
-ENV/
-env.bak/
-venv.bak/
-
-# Spyder project settings
-.spyderproject
-.spyproject
-
-# Rope project settings
-.ropeproject
-
-# mkdocs documentation
-/site
-
-# mypy
-.mypy_cache/
-.dmypy.json
-dmypy.json
-
-# Pyre type checker
-.pyre/
-
-# pytype static type analyzer
-.pytype/
-
-# Cython debug symbols
-cython_debug/
-
-# PyCharm
-#  JetBrains specific template is maintained in a separate JetBrains.gitignore that can
-#  be found at https://github.com/github/gitignore/blob/main/Global/JetBrains.gitignore
-#  and can be added to the global gitignore or merged into this file.  For a more nuclear
-#  option (not recommended) you can uncomment the following to ignore the entire idea folder.
-#.idea/
-
-### Python Patch ###
-# Poetry local configuration file - https://python-poetry.org/docs/configuration/#local-configuration
-poetry.toml
-
-# ruff
-.ruff_cache/
-
-# LSP config files
-pyrightconfig.json
-
-### VisualStudioCode ###
-.vscode/*
-!.vscode/settings.json
-!.vscode/tasks.json
-!.vscode/launch.json
-!.vscode/extensions.json
-!.vscode/*.code-snippets
-
-# Local History for Visual Studio Code
-.history/
-
-# Built Visual Studio Code Extensions
-*.vsix
-
-### VisualStudioCode Patch ###
-# Ignore all local history of files
-.history
-.ionide
-
-### VisualStudio ###
+# VisualStudio*******************************************************************
 ## Ignore Visual Studio temporary files, build results, and
 ## files generated by popular Visual Studio add-ons.
 ##
 ## Get latest from https://github.com/github/gitignore/blob/main/VisualStudio.gitignore
 
 # User-specific files
 *.rsuser
@@ -298,27 +71,30 @@
 
 # Files built by Visual Studio
 *_i.c
 *_p.c
 *_h.h
 *.ilk
 *.meta
+*.obj
 *.iobj
+*.pch
 *.pdb
 *.ipdb
 *.pgc
 *.pgd
 *.rsp
 *.sbr
 *.tlb
 *.tli
 *.tlh
 *.tmp
 *.tmp_proj
 *_wpftmp.csproj
+*.log
 *.tlog
 *.vspscc
 *.vssscc
 .builds
 *.pidb
 *.svclog
 *.scc
@@ -523,14 +299,16 @@
 *.vbp
 
 # Visual Studio 6 workspace and project file (working project files containing files to include in project)
 *.dsw
 *.dsp
 
 # Visual Studio 6 technical files
+*.ncb
+*.aps
 
 # Visual Studio LightSwitch build output
 **/*.HTMLClient/GeneratedArtifacts
 **/*.DesktopClient/GeneratedArtifacts
 **/*.DesktopClient/ModelManifest.xml
 **/*.Server/GeneratedArtifacts
 **/*.Server/ModelManifest.xml
@@ -543,14 +321,15 @@
 # FAKE - F# Make
 .fake/
 
 # CodeRush personal settings
 .cr/personal
 
 # Python Tools for Visual Studio (PTVS)
+__pycache__/
 *.pyc
 
 # Cake - Uncomment if you are using it
 # tools/**
 # !tools/packages.config
 
 # Tabs Studio
@@ -595,28 +374,222 @@
 # Ionide (cross platform F# VS Code tools) working folder
 .ionide/
 
 # Fody - auto-generated XML schema
 FodyWeavers.xsd
 
 # VS Code files for those working on multiple tools
+.vscode/*
+!.vscode/settings.json
+!.vscode/tasks.json
+!.vscode/launch.json
+!.vscode/extensions.json
 *.code-workspace
 
 # Local History for Visual Studio Code
+.history/
 
 # Windows Installer files from build outputs
 *.cab
 *.msi
 *.msix
 *.msm
 *.msp
 
 # JetBrains Rider
 *.sln.iml
+# Python*************************************************************************
+# Byte-compiled / optimized / DLL files
+__pycache__/
+*.py[cod]
+*$py.class
+
+# C extensions
+*.so
+
+# Distribution / packaging
+.Python
+build/
+develop-eggs/
+dist/
+downloads/
+eggs/
+.eggs/
+lib/
+lib64/
+parts/
+sdist/
+var/
+wheels/
+share/python-wheels/
+*.egg-info/
+.installed.cfg
+*.egg
+MANIFEST
 
-### VisualStudio Patch ###
-# Additional files built by Visual Studio
+# PyInstaller
+#  Usually these files are written by a python script from a template
+#  before PyInstaller builds the exe, so as to inject date/other infos into it.
+*.manifest
+*.spec
+
+# Installer logs
+pip-log.txt
+pip-delete-this-directory.txt
+
+# Unit test / coverage reports
+htmlcov/
+.tox/
+.nox/
+.coverage
+.coverage.*
+.cache
+nosetests.xml
+coverage.xml
+*.cover
+*.py,cover
+.hypothesis/
+.pytest_cache/
+cover/
+
+# Translations
+*.mo
+*.pot
+
+# Django stuff:
+*.log
+local_settings.py
+db.sqlite3
+db.sqlite3-journal
+
+# Flask stuff:
+instance/
+.webassets-cache
+
+# Scrapy stuff:
+.scrapy
+
+# Sphinx documentation
+docs/_build/
+
+# PyBuilder
+.pybuilder/
+target/
+
+# Jupyter Notebook
+.ipynb_checkpoints
+
+# IPython
+profile_default/
+ipython_config.py
+
+# pyenv
+#   For a library or package, you might want to ignore these files since the code is
+#   intended to run in multiple environments; otherwise, check them in:
+# .python-version
+
+# pipenv
+#   According to pypa/pipenv#598, it is recommended to include Pipfile.lock in version control.
+#   However, in case of collaboration, if having platform-specific dependencies or dependencies
+#   having no cross-platform support, pipenv may install dependencies that don't work, or not
+#   install all needed dependencies.
+#Pipfile.lock
+
+# poetry
+#   Similar to Pipfile.lock, it is generally recommended to include poetry.lock in version control.
+#   This is especially recommended for binary packages to ensure reproducibility, and is more
+#   commonly ignored for libraries.
+#   https://python-poetry.org/docs/basic-usage/#commit-your-poetrylock-file-to-version-control
+#poetry.lock
+
+# pdm
+#   Similar to Pipfile.lock, it is generally recommended to include pdm.lock in version control.
+#pdm.lock
+#   pdm stores project-wide configurations in .pdm.toml, but it is recommended to not include it
+#   in version control.
+#   https://pdm.fming.dev/#use-with-ide
+.pdm.toml
+
+# PEP 582; used by e.g. github.com/David-OConnor/pyflow and github.com/pdm-project/pdm
+__pypackages__/
+
+# Celery stuff
+celerybeat-schedule
+celerybeat.pid
+
+# SageMath parsed files
+*.sage.py
+
+# Environments
+.env
+.venv
+env/
+venv/
+ENV/
+env.bak/
+venv.bak/
+
+# Spyder project settings
+.spyderproject
+.spyproject
+
+# Rope project settings
+.ropeproject
+
+# mkdocs documentation
+/site
+
+# mypy
+.mypy_cache/
+.dmypy.json
+dmypy.json
+
+# Pyre type checker
+.pyre/
+
+# pytype static type analyzer
+.pytype/
+
+# Cython debug symbols
+cython_debug/
+
+# PyCharm
+#  JetBrains specific template is maintained in a separate JetBrains.gitignore that can
+#  be found at https://github.com/github/gitignore/blob/main/Global/JetBrains.gitignore
+#  and can be added to the global gitignore or merged into this file.  For a more nuclear
+#  option (not recommended) you can uncomment the following to ignore the entire idea folder.
+#.idea/
+# Fortran************************************************************************
+# Prerequisites
+*.d
+
+# Compiled Object files
+*.slo
+*.lo
+*.o
+*.obj
+
+# Precompiled Headers
+*.gch
+*.pch
+
+# Compiled Dynamic libraries
+*.so
+*.dylib
+*.dll
+
+# Fortran module files
+*.mod
+*.smod
+
+# Compiled Static libraries
+*.lai
+*.la
+*.a
+*.lib
+
+# Executables
+*.exe
+*.out
+*.app
 
-# End of https://www.toptal.com/developers/gitignore/api/python,fortran,visualstudio,visualstudiocode
-src/metalattice/_version.py
-*.metalattice.*
-*.inp
+_version.py
```

### Comparing `metalattice-0.0.27/LICENSE` & `metalattice-0.1.21/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `metalattice-0.0.27/pyproject.toml` & `metalattice-0.1.21/pyproject.toml`

 * *Files 9% similar despite different names*

```diff
@@ -1,30 +1,26 @@
 [build-system]
 requires = ["setuptools", "setuptools-scm"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "metalattice"
 authors = [
-    {name = "Huang Lihao", email = "huang-lihao@outlook.com"},
+    {name = "HUANG Lihao", email = "huang-lihao@outlook.com"},
 ]
 description = "A Python package to model lattice metamaterials, using Abaqus."
 readme = "README.md"
 requires-python = ">=3.7"
-keywords = ["lattice metamaterial", "micropolar", "cosserat", "abaqus"]
-license = {file = "LICENSE"}
+keywords = ["micropolar", "cosserat", "lattice metamaterial", "abaqus"]
+license = {file = "LICENSE.txt"}
 classifiers = [
-    "Development Status :: 3 - Alpha",
     "Programming Language :: Python :: 3",
 ]
 dependencies = [
-    "cython",
-    "f90nml",
-    "gfort2py",
     "numpy",
 ]
 dynamic = ["version"]
 
 # pyproject.toml
 [tool.setuptools_scm]
 write_to = "src/metalattice/_version.py"
-local_scheme = "no-local-version"
+local_scheme = "no-local-version"
```

