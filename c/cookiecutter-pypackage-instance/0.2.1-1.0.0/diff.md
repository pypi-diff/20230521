# Comparing `tmp/cookiecutter-pypackage-instance-0.2.1.tar.gz` & `tmp/cookiecutter_pypackage_instance-1.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cookiecutter-pypackage-instance-0.2.1.tar", max compression
+gzip compressed data, was "cookiecutter_pypackage_instance-1.0.0.tar", max compression
```

## Comparing `cookiecutter-pypackage-instance-0.2.1.tar` & `cookiecutter_pypackage_instance-1.0.0.tar`

### file list

```diff
@@ -1,8 +1,7 @@
--rw-r--r--   0        0        0     1089 2022-05-16 21:57:56.545060 cookiecutter-pypackage-instance-0.2.1/LICENSE
--rw-r--r--   0        0        0     4592 2022-05-16 21:57:56.545060 cookiecutter-pypackage-instance-0.2.1/README.md
--rw-r--r--   0        0        0     4657 2022-05-16 21:57:57.241080 cookiecutter-pypackage-instance-0.2.1/pyproject.toml
--rw-r--r--   0        0        0       82 2022-05-16 21:57:56.549060 cookiecutter-pypackage-instance-0.2.1/src/cookiecutter_pypackage_instance/__init__.py
--rw-r--r--   0        0        0      417 2022-05-16 21:57:56.549060 cookiecutter-pypackage-instance-0.2.1/src/cookiecutter_pypackage_instance/cookiecutter_pypackage_instance.py
--rw-r--r--   0        0        0        0 2022-05-16 21:57:56.549060 cookiecutter-pypackage-instance-0.2.1/src/cookiecutter_pypackage_instance/py.typed
--rw-r--r--   0        0        0     5463 2022-05-16 21:58:06.098589 cookiecutter-pypackage-instance-0.2.1/setup.py
--rw-r--r--   0        0        0     5692 2022-05-16 21:58:06.098956 cookiecutter-pypackage-instance-0.2.1/PKG-INFO
+-rw-r--r--   0        0        0     1089 2023-05-21 10:56:56.390727 cookiecutter_pypackage_instance-1.0.0/LICENSE
+-rw-r--r--   0        0        0     4136 2023-05-21 10:56:56.390727 cookiecutter_pypackage_instance-1.0.0/README.md
+-rw-r--r--   0        0        0     4321 2023-05-21 10:56:57.310728 cookiecutter_pypackage_instance-1.0.0/pyproject.toml
+-rw-r--r--   0        0        0       82 2023-05-21 10:56:56.390727 cookiecutter_pypackage_instance-1.0.0/src/cookiecutter_pypackage_instance/__init__.py
+-rw-r--r--   0        0        0      417 2023-05-21 10:56:56.390727 cookiecutter_pypackage_instance-1.0.0/src/cookiecutter_pypackage_instance/cookiecutter_pypackage_instance.py
+-rw-r--r--   0        0        0        0 2023-05-21 10:56:56.390727 cookiecutter_pypackage_instance-1.0.0/src/cookiecutter_pypackage_instance/py.typed
+-rw-r--r--   0        0        0     5137 1970-01-01 00:00:00.000000 cookiecutter_pypackage_instance-1.0.0/PKG-INFO
```

### Comparing `cookiecutter-pypackage-instance-0.2.1/LICENSE` & `cookiecutter_pypackage_instance-1.0.0/LICENSE`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 MIT License
 
-Copyright (c) 2022-2022 Vasilis Sioros (billsioros)
+Copyright (c) 2023-2023 Vasilis Sioros (billsioros)
 
 Permission is hereby granted, free of charge, to any person obtaining a copy
 of this software and associated documentation files (the "Software"), to deal
 in the Software without restriction, including without limitation the rights
 to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
 copies of the Software, and to permit persons to whom the Software is
 furnished to do so, subject to the following conditions:
```

### Comparing `cookiecutter-pypackage-instance-0.2.1/README.md` & `cookiecutter_pypackage_instance-1.0.0/README.md`

 * *Files 7% similar despite different names*

```diff
@@ -69,63 +69,47 @@
     <img
       src="https://app.fossa.com/api/projects/git%2Bgithub.com%2Fbillsioros%2Fcookiecutter-pypackage-instance.svg?type=shield"
       alt="FOSSA Status"
     />
   </a>
 </p>
 
-## :bulb: Example
+## :cd: Installation
 
-```python
->>> from cookiecutter_pypackage_instance import cookiecutter_pypackage_instance
+```bash
+pip install cookiecutter-pypackage-instance
 ```
 
-## :rocket: Features
+In order to locally set up the project please follow the instructions below:
 
-- TODO
+```shell
+# Set up the GitHub repository
+git init
+git config --local user.name Vasilis Sioros
+git config --local user.email billsioros97@gmail.com
+git add .
+git commit -m "feat: initial commit"
+git remote add origin https://github.com/billsioros/cookiecutter-pypackage-instance
+
+# Create a virtual environment using poetry and install the required dependencies
+poetry shell
+poetry install
+
+# Install pre-commit hooks
+pre-commit install --install-hooks
+```
 
 ## :book: Documentation
 
 The project's documentation can be found [here](https://billsioros.github.io/cookiecutter-pypackage-instance/).
 
-## :cd: Installation
-
-```bash
-pip install cookiecutter-pypackage-instance
-```
-
 ## :heart: Support the project
 
 Feel free to [**Buy me a coffee! ☕**](https://www.buymeacoffee.com/billsioros).
 
 ## :sparkles: Contributing
 
 If you would like to contribute to the project, please go through the [Contributing Guidelines](https://billsioros.github.io/cookiecutter-pypackage-instance/latest/CONTRIBUTING/) first.
 
-Thanks goes to these wonderful people ([emoji key](https://allcontributors.org/docs/en/emoji-key)):
-
-<!-- ALL-CONTRIBUTORS-LIST:START - Do not remove or modify this section -->
-<!-- prettier-ignore-start -->
-<!-- markdownlint-disable -->
-
-<!-- markdownlint-restore -->
-<!-- prettier-ignore-end -->
-<!-- ALL-CONTRIBUTORS-LIST:END -->
-
-This project follows the [all-contributors](https://github.com/all-contributors/all-contributors) specification. Contributions of any kind welcome!
-
-## :bookmark_tabs: Citation
-
-```bibtex
-@misc{cookiecutter-pypackage-instance,
-  author = {Vasilis Sioros},
-  title = {🐍 An awesome python package by the name Cookiecutter Pypackage Instance},
-  year = {2022},
-  publisher = {GitHub},
-  journal = {GitHub repository},
-  howpublished = {\url{https://github.com/billsioros/cookiecutter-pypackage-instance}}
-}
-```
-
 ## :label: Credits
 
 This project was generated with [`billsioros/cookiecutter-pypackage`](https://github.com/billsioros/cookiecutter-pypackage) cookiecutter template.
```

#### html2text {}

```diff
@@ -1,25 +1,22 @@
                  ****** Cookiecutter Pypackage Instance ******
   ð An awesome python package by the name Cookiecutter Pypackage Instance
 [PyPI_-_Python_Version] [PyPI] [CI] [CD] [pre-commit.ci_status] [Test_Coverage]
 [PyPI_-_License] [Open_on_Gitpod] [Cookiecutter_Template] [Renovate_-_Enabled]
                        [Buy_me_a_coffee] [FOSSA_Status]
-## :bulb: Example ```python >>> from cookiecutter_pypackage_instance import
-cookiecutter_pypackage_instance ``` ## :rocket: Features - TODO ## :book:
+## :cd: Installation ```bash pip install cookiecutter-pypackage-instance ``` In
+order to locally set up the project please follow the instructions below:
+```shell # Set up the GitHub repository git init git config --local user.name
+Vasilis Sioros git config --local user.email billsioros97@gmail.com git add .
+git commit -m "feat: initial commit" git remote add origin https://github.com/
+billsioros/cookiecutter-pypackage-instance # Create a virtual environment using
+poetry and install the required dependencies poetry shell poetry install #
+Install pre-commit hooks pre-commit install --install-hooks ``` ## :book:
 Documentation The project's documentation can be found [here](https://
-billsioros.github.io/cookiecutter-pypackage-instance/). ## :cd: Installation
-```bash pip install cookiecutter-pypackage-instance ``` ## :heart: Support the
+billsioros.github.io/cookiecutter-pypackage-instance/). ## :heart: Support the
 project Feel free to [**Buy me a coffee! â**](https://www.buymeacoffee.com/
 billsioros). ## :sparkles: Contributing If you would like to contribute to the
 project, please go through the [Contributing Guidelines](https://
 billsioros.github.io/cookiecutter-pypackage-instance/latest/CONTRIBUTING/
-) first. Thanks goes to these wonderful people ([emoji key](https://
-allcontributors.org/docs/en/emoji-key)):       This project follows the [all-
-contributors](https://github.com/all-contributors/all-contributors)
-specification. Contributions of any kind welcome! ## :bookmark_tabs: Citation
-```bibtex @misc{cookiecutter-pypackage-instance, author = {Vasilis Sioros},
-title = {ð An awesome python package by the name Cookiecutter Pypackage
-Instance}, year = {2022}, publisher = {GitHub}, journal = {GitHub repository},
-howpublished = {\url{https://github.com/billsioros/cookiecutter-pypackage-
-instance}} } ``` ## :label: Credits This project was generated with
-[`billsioros/cookiecutter-pypackage`](https://github.com/billsioros/
-cookiecutter-pypackage) cookiecutter template.
+) first. ## :label: Credits This project was generated with [`billsioros/
+cookiecutter-pypackage`](https://github.com/billsioros/cookiecutter-pypackage)
+cookiecutter template.
```

### Comparing `cookiecutter-pypackage-instance-0.2.1/pyproject.toml` & `cookiecutter_pypackage_instance-1.0.0/pyproject.toml`

 * *Files 13% similar despite different names*

```diff
@@ -1,63 +1,56 @@
 [build-system]
 requires = ["poetry-core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry]
 name = "cookiecutter-pypackage-instance"
-version = "0.2.1"
+version = "1.0.0"
 description = "🐍 An awesome python package by the name Cookiecutter Pypackage Instance"
 readme = "README.md"
 authors = ["Vasilis Sioros <billsioros97@gmail.com>"]
 license = "MIT"
 homepage = "https://billsioros.github.io/cookiecutter-pypackage-instance"
 repository = "https://github.com/billsioros/cookiecutter-pypackage-instance"
 keywords = []
 classifiers = [
     "Programming Language :: Python",
     "Programming Language :: Python :: 3",
     "Programming Language :: Python :: 3 :: Only",
-    "Programming Language :: Python :: 3.6",
-    "Programming Language :: Python :: 3.7",
-    "Programming Language :: Python :: 3.8",
     "Programming Language :: Python :: 3.9",
 ]
 
 [tool.poetry.urls]
 "Bug Tracker" = "https://github.com/billsioros/cookiecutter-pypackage-instance/issues"
 "Changelog" = "https://github.com/billsioros/cookiecutter-pypackage-instance/releases"
 
 [tool.poetry.dependencies]
-python = "^3.7"
+python = "^3.9"
 
 [tool.poetry.dev-dependencies]
-python-semantic-release = "^7.15.3"
-wemake-python-styleguide = "0.16.1"
-flakeheaven = "^0.11.1"
-isort = "^5.9.3"
-mypy = "^0.910"
-black = "^22.3.0"
-pre-commit = "^2.12.1"
-poethepoet = "^0.10.0"
-coverage = {extras = ["toml"], version = "^5.5"}
-pytest = "^6.2.4"
-pytest-cov = "^2.12.1"
-pytest-sugar = "^0.9.4"
-pytest-clarity = "^1.0.1"
-tox = "^3.23.0"
-tox-poetry-installer = { extras = ["poetry"], version = "^0.8.0" }
-tox-gh-actions = "^2.5.0"
-tox-pyenv = "^1.1.0"
-mkdocs = "^1.1.2"
-mkdocs-material = "^7.1.3"
-mkdocs-minify-plugin = "^0.4.0"
-mkdocs-redirects = "^1.0.3"
-mkdocstrings = "^0.15.0"
-mdx-truly-sane-lists = "^1.2"
-mike = "^1.0.1"
+python-semantic-release = "*"
+wemake-python-styleguide = "*"
+flakeheaven = "*"
+isort = "*"
+mypy = "*"
+black = "*"
+pre-commit = "*"
+poethepoet = "*"
+coverage = {extras = ["toml"], version = "*" }
+pytest = "*"
+pytest-cov = "*"
+pytest-sugar = "*"
+pytest-clarity = "*"
+mkdocs = "*"
+mkdocs-material = "*"
+mkdocs-minify-plugin = "*"
+mkdocs-redirects = "*"
+mkdocstrings = "*"
+mdx-truly-sane-lists = "*"
+mike = "*"
 
 [tool.semantic_release]
 version_toml = "pyproject.toml:tool.poetry.version"
 changelog_components = "semantic_release.changelog.changelog_headers,semantic_release.changelog.compare_url"
 build_command = "python -m pip install poetry && poetry build"
 
 [tool.vulture]
@@ -123,15 +116,14 @@
 
 [tool.flakeheaven]
 exclude = [
   ".git",
   ".github",
   ".mypy_cache",
   ".pytest_cache",
-  ".tox",
   ".vscode",
   ".venv",
   "build",
   "dist",
   "docs",
   "tests",
   "__pycache__",
@@ -151,7 +143,10 @@
 "flake8-*" = ["+*"]
 mccabe = ["+*"]
 nitpick = ["+*"]
 "pep8-naming" = ["+*"]
 pycodestyle = ["+*"]
 pyflakes = ["+*"]
 "wemake-python-styleguide" = ["+*"]
+
+[tool.pydocstyle]
+convention = "google"
```

### Comparing `cookiecutter-pypackage-instance-0.2.1/setup.py` & `cookiecutter_pypackage_instance-1.0.0/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,30 +1,137 @@
-# -*- coding: utf-8 -*-
-from setuptools import setup
+Metadata-Version: 2.1
+Name: cookiecutter-pypackage-instance
+Version: 1.0.0
+Summary: 🐍 An awesome python package by the name Cookiecutter Pypackage Instance
+Home-page: https://billsioros.github.io/cookiecutter-pypackage-instance
+License: MIT
+Author: Vasilis Sioros
+Author-email: billsioros97@gmail.com
+Requires-Python: >=3.9,<4.0
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Programming Language :: Python
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3 :: Only
+Project-URL: Bug Tracker, https://github.com/billsioros/cookiecutter-pypackage-instance/issues
+Project-URL: Changelog, https://github.com/billsioros/cookiecutter-pypackage-instance/releases
+Project-URL: Repository, https://github.com/billsioros/cookiecutter-pypackage-instance
+Description-Content-Type: text/markdown
+
+<h1 align="center">Cookiecutter Pypackage Instance</h1>
+
+<p align="center"><em>🐍 An awesome python package by the name Cookiecutter Pypackage Instance</em></p>
+
+<p align="center">
+  <a href="https://www.python.org/">
+    <img
+      src="https://img.shields.io/pypi/pyversions/cookiecutter-pypackage-instance"
+      alt="PyPI - Python Version"
+    />
+  </a>
+  <a href="https://pypi.org/project/cookiecutter-pypackage-instance/">
+    <img
+      src="https://img.shields.io/pypi/v/cookiecutter-pypackage-instance"
+      alt="PyPI"
+    />
+  </a>
+  <a href="https://github.com/billsioros/cookiecutter-pypackage-instance/actions/workflows/ci.yml">
+    <img
+      src="https://github.com/billsioros/cookiecutter-pypackage-instance/actions/workflows/ci.yml/badge.svg"
+      alt="CI"
+    />
+  </a>
+  <a href="https://github.com/billsioros/cookiecutter-pypackage-instance/actions/workflows/cd.yml">
+    <img
+      src="https://github.com/billsioros/cookiecutter-pypackage-instance/actions/workflows/cd.yml/badge.svg"
+      alt="CD"
+    />
+  </a>
+  <a href="https://results.pre-commit.ci/latest/github/billsioros/cookiecutter-pypackage-instance/master">
+    <img
+      src="https://results.pre-commit.ci/badge/github/billsioros/cookiecutter-pypackage-instance/master.svg"
+      alt="pre-commit.ci status"
+    />
+  </a>
+  <a href="https://codecov.io/gh/billsioros/cookiecutter-pypackage-instance">
+    <img
+      src="https://codecov.io/gh/billsioros/cookiecutter-pypackage-instance/branch/master/graph/badge.svg?token=coLOL0j6Ap"
+      alt="Test Coverage"/>
+  </a>
+  <a href="https://opensource.org/licenses/MIT">
+    <img
+      src="https://img.shields.io/pypi/l/cookiecutter-pypackage-instance"
+      alt="PyPI - License"
+    />
+  </a>
+  <a href="https://gitpod.io/from-referrer/">
+    <img
+      src="https://img.shields.io/badge/Open%20on-Gitpod-blue?logo=gitpod&style=flat"
+      alt="Open on Gitpod"
+    />
+  </a>
+  <a href="https://github.com/billsioros/cookiecutter-pypackage">
+    <img
+      src="https://img.shields.io/badge/cookiecutter-template-D4AA00.svg?style=flat&logo=cookiecutter"
+      alt="Cookiecutter Template">
+  </a>
+  <a href="https://app.renovatebot.com/dashboard#github/billsioros/cookiecutter-pypackage-instance">
+    <img
+      src="https://img.shields.io/badge/renovate-enabled-brightgreen.svg?style=flat&logo=renovatebot"
+      alt="Renovate - Enabled">
+  </a>
+  <a href="https://www.buymeacoffee.com/billsioros">
+    <img
+      src="https://img.shields.io/badge/Buy%20me%20a-coffee-FFDD00.svg?style=flat&logo=buymeacoffee"
+      alt="Buy me a coffee">
+  </a>
+  <a href="https://app.fossa.com/projects/git%2Bgithub.com%2Fbillsioros%2Fcookiecutter-pypackage-instance?ref=badge_shield">
+    <img
+      src="https://app.fossa.com/api/projects/git%2Bgithub.com%2Fbillsioros%2Fcookiecutter-pypackage-instance.svg?type=shield"
+      alt="FOSSA Status"
+    />
+  </a>
+</p>
+
+## :cd: Installation
+
+```bash
+pip install cookiecutter-pypackage-instance
+```
+
+In order to locally set up the project please follow the instructions below:
+
+```shell
+# Set up the GitHub repository
+git init
+git config --local user.name Vasilis Sioros
+git config --local user.email billsioros97@gmail.com
+git add .
+git commit -m "feat: initial commit"
+git remote add origin https://github.com/billsioros/cookiecutter-pypackage-instance
+
+# Create a virtual environment using poetry and install the required dependencies
+poetry shell
+poetry install
+
+# Install pre-commit hooks
+pre-commit install --install-hooks
+```
+
+## :book: Documentation
+
+The project's documentation can be found [here](https://billsioros.github.io/cookiecutter-pypackage-instance/).
+
+## :heart: Support the project
+
+Feel free to [**Buy me a coffee! ☕**](https://www.buymeacoffee.com/billsioros).
 
-package_dir = \
-{'': 'src'}
+## :sparkles: Contributing
 
-packages = \
-['cookiecutter_pypackage_instance']
+If you would like to contribute to the project, please go through the [Contributing Guidelines](https://billsioros.github.io/cookiecutter-pypackage-instance/latest/CONTRIBUTING/) first.
 
-package_data = \
-{'': ['*']}
-
-setup_kwargs = {
-    'name': 'cookiecutter-pypackage-instance',
-    'version': '0.2.1',
-    'description': '🐍 An awesome python package by the name Cookiecutter Pypackage Instance',
-    'long_description': '<h1 align="center">Cookiecutter Pypackage Instance</h1>\n\n<p align="center"><em>🐍 An awesome python package by the name Cookiecutter Pypackage Instance</em></p>\n\n<p align="center">\n  <a href="https://www.python.org/">\n    <img\n      src="https://img.shields.io/pypi/pyversions/cookiecutter-pypackage-instance"\n      alt="PyPI - Python Version"\n    />\n  </a>\n  <a href="https://pypi.org/project/cookiecutter-pypackage-instance/">\n    <img\n      src="https://img.shields.io/pypi/v/cookiecutter-pypackage-instance"\n      alt="PyPI"\n    />\n  </a>\n  <a href="https://github.com/billsioros/cookiecutter-pypackage-instance/actions/workflows/ci.yml">\n    <img\n      src="https://github.com/billsioros/cookiecutter-pypackage-instance/actions/workflows/ci.yml/badge.svg"\n      alt="CI"\n    />\n  </a>\n  <a href="https://github.com/billsioros/cookiecutter-pypackage-instance/actions/workflows/cd.yml">\n    <img\n      src="https://github.com/billsioros/cookiecutter-pypackage-instance/actions/workflows/cd.yml/badge.svg"\n      alt="CD"\n    />\n  </a>\n  <a href="https://results.pre-commit.ci/latest/github/billsioros/cookiecutter-pypackage-instance/master">\n    <img\n      src="https://results.pre-commit.ci/badge/github/billsioros/cookiecutter-pypackage-instance/master.svg"\n      alt="pre-commit.ci status"\n    />\n  </a>\n  <a href="https://codecov.io/gh/billsioros/cookiecutter-pypackage-instance">\n    <img\n      src="https://codecov.io/gh/billsioros/cookiecutter-pypackage-instance/branch/master/graph/badge.svg?token=coLOL0j6Ap"\n      alt="Test Coverage"/>\n  </a>\n  <a href="https://opensource.org/licenses/MIT">\n    <img\n      src="https://img.shields.io/pypi/l/cookiecutter-pypackage-instance"\n      alt="PyPI - License"\n    />\n  </a>\n  <a href="https://gitpod.io/from-referrer/">\n    <img\n      src="https://img.shields.io/badge/Open%20on-Gitpod-blue?logo=gitpod&style=flat"\n      alt="Open on Gitpod"\n    />\n  </a>\n  <a href="https://github.com/billsioros/cookiecutter-pypackage">\n    <img\n      src="https://img.shields.io/badge/cookiecutter-template-D4AA00.svg?style=flat&logo=cookiecutter"\n      alt="Cookiecutter Template">\n  </a>\n  <a href="https://app.renovatebot.com/dashboard#github/billsioros/cookiecutter-pypackage-instance">\n    <img\n      src="https://img.shields.io/badge/renovate-enabled-brightgreen.svg?style=flat&logo=renovatebot"\n      alt="Renovate - Enabled">\n  </a>\n  <a href="https://www.buymeacoffee.com/billsioros">\n    <img\n      src="https://img.shields.io/badge/Buy%20me%20a-coffee-FFDD00.svg?style=flat&logo=buymeacoffee"\n      alt="Buy me a coffee">\n  </a>\n  <a href="https://app.fossa.com/projects/git%2Bgithub.com%2Fbillsioros%2Fcookiecutter-pypackage-instance?ref=badge_shield">\n    <img\n      src="https://app.fossa.com/api/projects/git%2Bgithub.com%2Fbillsioros%2Fcookiecutter-pypackage-instance.svg?type=shield"\n      alt="FOSSA Status"\n    />\n  </a>\n</p>\n\n## :bulb: Example\n\n```python\n>>> from cookiecutter_pypackage_instance import cookiecutter_pypackage_instance\n```\n\n## :rocket: Features\n\n- TODO\n\n## :book: Documentation\n\nThe project\'s documentation can be found [here](https://billsioros.github.io/cookiecutter-pypackage-instance/).\n\n## :cd: Installation\n\n```bash\npip install cookiecutter-pypackage-instance\n```\n\n## :heart: Support the project\n\nFeel free to [**Buy me a coffee! ☕**](https://www.buymeacoffee.com/billsioros).\n\n## :sparkles: Contributing\n\nIf you would like to contribute to the project, please go through the [Contributing Guidelines](https://billsioros.github.io/cookiecutter-pypackage-instance/latest/CONTRIBUTING/) first.\n\nThanks goes to these wonderful people ([emoji key](https://allcontributors.org/docs/en/emoji-key)):\n\n<!-- ALL-CONTRIBUTORS-LIST:START - Do not remove or modify this section -->\n<!-- prettier-ignore-start -->\n<!-- markdownlint-disable -->\n\n<!-- markdownlint-restore -->\n<!-- prettier-ignore-end -->\n<!-- ALL-CONTRIBUTORS-LIST:END -->\n\nThis project follows the [all-contributors](https://github.com/all-contributors/all-contributors) specification. Contributions of any kind welcome!\n\n## :bookmark_tabs: Citation\n\n```bibtex\n@misc{cookiecutter-pypackage-instance,\n  author = {Vasilis Sioros},\n  title = {🐍 An awesome python package by the name Cookiecutter Pypackage Instance},\n  year = {2022},\n  publisher = {GitHub},\n  journal = {GitHub repository},\n  howpublished = {\\url{https://github.com/billsioros/cookiecutter-pypackage-instance}}\n}\n```\n\n## :label: Credits\n\nThis project was generated with [`billsioros/cookiecutter-pypackage`](https://github.com/billsioros/cookiecutter-pypackage) cookiecutter template.\n',
-    'author': 'Vasilis Sioros',
-    'author_email': 'billsioros97@gmail.com',
-    'maintainer': None,
-    'maintainer_email': None,
-    'url': 'https://billsioros.github.io/cookiecutter-pypackage-instance',
-    'package_dir': package_dir,
-    'packages': packages,
-    'package_data': package_data,
-    'python_requires': '>=3.7,<4.0',
-}
+## :label: Credits
 
+This project was generated with [`billsioros/cookiecutter-pypackage`](https://github.com/billsioros/cookiecutter-pypackage) cookiecutter template.
 
-setup(**setup_kwargs)
```

#### html2text {}

```diff
@@ -1,58 +1,36 @@
-# -*- coding: utf-8 -*- from setuptools import setup package_dir = \ {'':
-'src'} packages = \ ['cookiecutter_pypackage_instance'] package_data = \ {'':
-['*']} setup_kwargs = { 'name': 'cookiecutter-pypackage-instance', 'version':
-'0.2.1', 'description': 'ð An awesome python package by the name
-Cookiecutter Pypackage Instance', 'long_description': '
+Metadata-Version: 2.1 Name: cookiecutter-pypackage-instance Version: 1.0.0
+Summary: ð An awesome python package by the name Cookiecutter Pypackage
+Instance Home-page: https://billsioros.github.io/cookiecutter-pypackage-
+instance License: MIT Author: Vasilis Sioros Author-email:
+billsioros97@gmail.com Requires-Python: >=3.9,<4.0 Classifier: License :: OSI
+Approved :: MIT License Classifier: Programming Language :: Python Classifier:
+Programming Language :: Python :: 3 Classifier: Programming Language :: Python
+:: 3.9 Classifier: Programming Language :: Python :: 3.10 Classifier:
+Programming Language :: Python :: 3.11 Classifier: Programming Language ::
+Python :: 3 :: Only Project-URL: Bug Tracker, https://github.com/billsioros/
+cookiecutter-pypackage-instance/issues Project-URL: Changelog, https://
+github.com/billsioros/cookiecutter-pypackage-instance/releases Project-URL:
+Repository, https://github.com/billsioros/cookiecutter-pypackage-instance
+Description-Content-Type: text/markdown
                  ****** Cookiecutter Pypackage Instance ******
-\n\n
   ð An awesome python package by the name Cookiecutter Pypackage Instance
-\n\n
-  \n \n_n_src="https://img.shields.io/pypi/pyversions/cookiecutter-pypackage-
-      instance"\n_alt="PyPI_-_Python_Version"\n_/>\n\n \n_n_src="https://
-img.shields.io/pypi/v/cookiecutter-pypackage-instance"\n_alt="PyPI"\n_/>\n\n \n
- n_src="https://github.com/billsioros/cookiecutter-pypackage-instance/actions/
- workflows/ci.yml/badge.svg"\n_alt="CI"\n_/>\n\n \n_n_src="https://github.com/
-     billsioros/cookiecutter-pypackage-instance/actions/workflows/cd.yml/
- badge.svg"\n_alt="CD"\n_/>\n\n \n_n_src="https://results.pre-commit.ci/badge/
-   github/billsioros/cookiecutter-pypackage-instance/master.svg"\n_alt="pre-
-    commit.ci_status"\n_/>\n\n \n_n_src="https://codecov.io/gh/billsioros/
-             cookiecutter-pypackage-instance/branch/master/graph/
-  badge.svg?token=coLOL0j6Ap"\n_alt="Test_Coverage"/>\n\n \n_n_src="https://
-img.shields.io/pypi/l/cookiecutter-pypackage-instance"\n_alt="PyPI_-_License"\n
-        />\n\n \n_n_src="https://img.shields.io/badge/Open%20on-Gitpod-
-blue?logo=gitpod&style=flat"\n_alt="Open_on_Gitpod"\n_/>\n\n \n_n_src="https://
-                  img.shields.io/badge/cookiecutter-template-
-D4AA00.svg?style=flat&logo=cookiecutter"\n_alt="Cookiecutter_Template">\n\n \n
-             n_src="https://img.shields.io/badge/renovate-enabled-
-brightgreen.svg?style=flat&logo=renovatebot"\n_alt="Renovate_-_Enabled">\n\n \n
-           n_src="https://img.shields.io/badge/Buy%20me%20a-coffee-
-  FFDD00.svg?style=flat&logo=buymeacoffee"\n_alt="Buy_me_a_coffee">\n\n \n_n
-                   src="https://app.fossa.com/api/projects/
-            git%2Bgithub.com%2Fbillsioros%2Fcookiecutter-pypackage-
-            instance.svg?type=shield"\n_alt="FOSSA_Status"\n_/>\n\n
-\n\n## :bulb: Example\n\n```python\n>>> from cookiecutter_pypackage_instance
-import cookiecutter_pypackage_instance\n```\n\n## :rocket: Features\n\n-
-TODO\n\n## :book: Documentation\n\nThe project\'s documentation can be found
-[here](https://billsioros.github.io/cookiecutter-pypackage-instance/).\n\n## :
-cd: Installation\n\n```bash\npip install cookiecutter-pypackage-
-instance\n```\n\n## :heart: Support the project\n\nFeel free to [**Buy me a
-coffee! â**](https://www.buymeacoffee.com/billsioros).\n\n## :sparkles:
-Contributing\n\nIf you would like to contribute to the project, please go
-through the [Contributing Guidelines](https://billsioros.github.io/
-cookiecutter-pypackage-instance/latest/CONTRIBUTING/) first.\n\nThanks goes to
-these wonderful people ([emoji key](https://allcontributors.org/docs/en/emoji-
-key)):\n\n\n\n\n\n\n\n\n\nThis project follows the [all-contributors](https://
-github.com/all-contributors/all-contributors) specification. Contributions of
-any kind welcome!\n\n## :bookmark_tabs: Citation\n\n```bibtex\n@misc
-{cookiecutter-pypackage-instance,\n author = {Vasilis Sioros},\n title = {ð
-An awesome python package by the name Cookiecutter Pypackage Instance},\n year
-= {2022},\n publisher = {GitHub},\n journal = {GitHub repository},\n
-howpublished = {\\url{https://github.com/billsioros/cookiecutter-pypackage-
-instance}}\n}\n```\n\n## :label: Credits\n\nThis project was generated with
-[`billsioros/cookiecutter-pypackage`](https://github.com/billsioros/
-cookiecutter-pypackage) cookiecutter template.\n', 'author': 'Vasilis Sioros',
-'author_email': 'billsioros97@gmail.com', 'maintainer': None,
-'maintainer_email': None, 'url': 'https://billsioros.github.io/cookiecutter-
-pypackage-instance', 'package_dir': package_dir, 'packages': packages,
-'package_data': package_data, 'python_requires': '>=3.7,<4.0', } setup
-(**setup_kwargs)
+[PyPI_-_Python_Version] [PyPI] [CI] [CD] [pre-commit.ci_status] [Test_Coverage]
+[PyPI_-_License] [Open_on_Gitpod] [Cookiecutter_Template] [Renovate_-_Enabled]
+                       [Buy_me_a_coffee] [FOSSA_Status]
+## :cd: Installation ```bash pip install cookiecutter-pypackage-instance ``` In
+order to locally set up the project please follow the instructions below:
+```shell # Set up the GitHub repository git init git config --local user.name
+Vasilis Sioros git config --local user.email billsioros97@gmail.com git add .
+git commit -m "feat: initial commit" git remote add origin https://github.com/
+billsioros/cookiecutter-pypackage-instance # Create a virtual environment using
+poetry and install the required dependencies poetry shell poetry install #
+Install pre-commit hooks pre-commit install --install-hooks ``` ## :book:
+Documentation The project's documentation can be found [here](https://
+billsioros.github.io/cookiecutter-pypackage-instance/). ## :heart: Support the
+project Feel free to [**Buy me a coffee! â**](https://www.buymeacoffee.com/
+billsioros). ## :sparkles: Contributing If you would like to contribute to the
+project, please go through the [Contributing Guidelines](https://
+billsioros.github.io/cookiecutter-pypackage-instance/latest/CONTRIBUTING/
+) first. ## :label: Credits This project was generated with [`billsioros/
+cookiecutter-pypackage`](https://github.com/billsioros/cookiecutter-pypackage)
+cookiecutter template.
```

