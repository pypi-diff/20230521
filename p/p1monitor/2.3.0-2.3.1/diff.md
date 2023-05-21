# Comparing `tmp/p1monitor-2.3.0.tar.gz` & `tmp/p1monitor-2.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "p1monitor-2.3.0.tar", max compression
+gzip compressed data, was "p1monitor-2.3.1.tar", max compression
```

## Comparing `p1monitor-2.3.0.tar` & `p1monitor-2.3.1.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rw-r--r--   0        0        0     1077 2023-02-09 21:27:49.731855 p1monitor-2.3.0/LICENSE
--rw-r--r--   0        0        0     7259 2023-02-09 21:27:49.731855 p1monitor-2.3.0/README.md
--rw-r--r--   0        0        0      419 2023-02-09 21:27:49.731855 p1monitor-2.3.0/p1monitor/__init__.py
--rw-r--r--   0        0        0      287 2023-02-09 21:27:49.731855 p1monitor-2.3.0/p1monitor/exceptions.py
--rw-r--r--   0        0        0     6167 2023-02-09 21:27:49.731855 p1monitor-2.3.0/p1monitor/models.py
--rw-r--r--   0        0        0     5553 2023-02-09 21:27:49.731855 p1monitor-2.3.0/p1monitor/p1monitor.py
--rw-r--r--   0        0        0     3840 2023-02-09 21:28:04.291662 p1monitor-2.3.0/pyproject.toml
--rw-r--r--   0        0        0     8192 1970-01-01 00:00:00.000000 p1monitor-2.3.0/setup.py
--rw-r--r--   0        0        0     8775 1970-01-01 00:00:00.000000 p1monitor-2.3.0/PKG-INFO
+-rw-r--r--   0        0        0     1077 2023-05-21 10:19:48.636788 p1monitor-2.3.1/LICENSE
+-rw-r--r--   0        0        0     7259 2023-05-21 10:19:48.636788 p1monitor-2.3.1/README.md
+-rw-r--r--   0        0        0      419 2023-05-21 10:19:48.636788 p1monitor-2.3.1/p1monitor/__init__.py
+-rw-r--r--   0        0        0      287 2023-05-21 10:19:48.636788 p1monitor-2.3.1/p1monitor/exceptions.py
+-rw-r--r--   0        0        0     6261 2023-05-21 10:19:48.636788 p1monitor-2.3.1/p1monitor/models.py
+-rw-r--r--   0        0        0     5568 2023-05-21 10:19:48.636788 p1monitor-2.3.1/p1monitor/p1monitor.py
+-rw-r--r--   0        0        0        0 2023-05-21 10:19:48.636788 p1monitor-2.3.1/p1monitor/py.typed
+-rw-r--r--   0        0        0     3710 2023-05-21 10:20:13.636803 p1monitor-2.3.1/pyproject.toml
+-rw-r--r--   0        0        0     8575 1970-01-01 00:00:00.000000 p1monitor-2.3.1/PKG-INFO
```

### Comparing `p1monitor-2.3.0/LICENSE` & `p1monitor-2.3.1/LICENSE`

 * *Files identical despite different names*

### Comparing `p1monitor-2.3.0/README.md` & `p1monitor-2.3.1/README.md`

 * *Files identical despite different names*

### Comparing `p1monitor-2.3.0/p1monitor/models.py` & `p1monitor-2.3.1/p1monitor/models.py`

 * *Files 5% similar despite different names*

```diff
@@ -29,28 +29,30 @@
     energy_production_low: float | None
 
     @staticmethod
     def from_dict(data: dict[str | int, Any]) -> SmartMeter:
         """Return SmartMeter object from the P1 Monitor API response.
 
         Args:
+        ----
             data: The data from the P1 Monitor API.
 
-        Returns
+        Returns:
         -------
             A SmartMeter object.
         """
 
         def energy_tariff(tariff: str) -> EnergyTariff:
             """Return API energy_tariff information.
 
             Args:
+            ----
                 tariff: The provided tariff code from the API.
 
-            Returns
+            Returns:
             -------
                 The energy tariff period class.
             """
             if tariff == "P":
                 return EnergyTariff.HIGH
             return EnergyTariff.LOW
 
@@ -80,17 +82,18 @@
     energy_production_price_low: float | None
 
     @staticmethod
     def from_dict(data: dict[str, Any]) -> Settings:
         """Return Settings object from the P1 Monitor API response.
 
         Args:
+        ----
             data: The data from the P1 Monitor API.
 
-        Returns
+        Returns:
         -------
             A Settings object.
         """
         return Settings(
             gas_consumption_price=search(15, data, "conf"),
             energy_consumption_price_low=search(1, data, "conf"),
             energy_consumption_price_high=search(2, data, "conf"),
@@ -120,17 +123,18 @@
     power_produced_phase_l3: int | None
 
     @staticmethod
     def from_dict(data: dict[str | int, Any]) -> Phases:
         """Return Phases object from the P1 Monitor API response.
 
         Args:
+        ----
             data: The data from the P1 Monitor API.
 
-        Returns
+        Returns:
         -------
             A Phases object.
         """
         return Phases(
             voltage_phase_l1=search(103, data, "status"),
             voltage_phase_l2=search(104, data, "status"),
             voltage_phase_l3=search(105, data, "status"),
@@ -155,17 +159,18 @@
     pulse_count: int | None
 
     @staticmethod
     def from_dict(data: dict[str | int, Any]) -> WaterMeter:
         """Return WaterMeter object from the P1 Monitor API response.
 
         Args:
+        ----
             data: The data from the P1 Monitor API.
 
-        Returns
+        Returns:
         -------
             A WaterMeter object.
         """
         data = data[0]
         return WaterMeter(
             consumption_day=data.get("WATERMETER_CONSUMPTION_LITER"),
             consumption_total=data.get("WATERMETER_CONSUMPTION_TOTAL_M3"),
@@ -173,19 +178,20 @@
         )
 
 
 def search(position: int, data: Any, service: str) -> float:
     """Find the correct value in the json data file.
 
     Args:
+    ----
         position: The position ID number.
         data: The JSON list which is requested from the API.
         service: Type of dataclass.
 
-    Returns
+    Returns:
     -------
         The value that corresponds to the specified position.
     """
     value: float
     for i in data:
         if service == "conf" and i["CONFIGURATION_ID"] == position:
             value = float(i["PARAMETER"])
@@ -194,14 +200,15 @@
     return value
 
 
 def convert(value: float) -> int:
     """Convert values from kW to W.
 
     Args:
+    ----
         value: The current value.
 
-    Returns
+    Returns:
     -------
         Value in Watt (W).
     """
     return int(float(value) * 1000)
```

### Comparing `p1monitor-2.3.0/p1monitor/p1monitor.py` & `p1monitor-2.3.1/p1monitor/p1monitor.py`

 * *Files 1% similar despite different names*

```diff
@@ -35,24 +35,25 @@
         *,
         method: str = METH_GET,
         params: Mapping[str, Any] | None = None,
     ) -> Any:
         """Handle a request to a P1 Monitor device.
 
         Args:
+        ----
             uri: Request URI, without '/api/', for example, 'status'
             method: HTTP Method to use.
             params: Extra options to improve or limit the response.
 
-        Returns
+        Returns:
         -------
             A Python dictionary (JSON decoded) with the response from
             the P1 Monitor API.
 
-        Raises
+        Raises:
         ------
             P1MonitorConnectionError: An error occurred while communicating
                 with the P1 Monitor.
             P1MonitorError: Received an unexpected response from the P1 Monitor API.
         """
         version = metadata.version(__package__)
         url = URL.build(scheme="http", host=self.host, path="/api/").join(URL(uri))
```

### Comparing `p1monitor-2.3.0/pyproject.toml` & `p1monitor-2.3.1/pyproject.toml`

 * *Files 11% similar despite different names*

```diff
@@ -1,143 +1,133 @@
 [tool.poetry]
 name = "p1monitor"
-version = "2.3.0"
+version = "2.3.1"
 description = "Asynchronous Python client for the P1 Monitor"
 authors = ["Klaas Schoute <hello@student-techlife.com>"]
 maintainers = ["Klaas Schoute <hello@student-techlife.com>"]
 license = "MIT"
 readme = "README.md"
 homepage = "https://github.com/klaasnicolaas/python-p1monitor"
 repository = "https://github.com/klaasnicolaas/python-p1monitor"
 documentation = "https://github.com/klaasnicolaas/python-p1monitor"
 keywords = ["p1", "monitor", "power", "energy", "api", "async", "client"]
 classifiers = [
-    "Development Status :: 5 - Production/Stable",
-    "Framework :: AsyncIO",
-    "Intended Audience :: Developers",
-    "License :: OSI Approved :: MIT License",
-    "Natural Language :: English",
-    "Programming Language :: Python :: 3.9",
-    "Programming Language :: Python :: 3.10",
-    "Programming Language :: Python :: 3.11",
-    "Programming Language :: Python :: 3",
-    "Topic :: Software Development :: Libraries :: Python Modules",
+  "Development Status :: 5 - Production/Stable",
+  "Framework :: AsyncIO",
+  "Intended Audience :: Developers",
+  "License :: OSI Approved :: MIT License",
+  "Natural Language :: English",
+  "Programming Language :: Python :: 3.9",
+  "Programming Language :: Python :: 3.10",
+  "Programming Language :: Python :: 3.11",
+  "Programming Language :: Python :: 3",
+  "Topic :: Software Development :: Libraries :: Python Modules",
 ]
 packages = [
-    { include = "p1monitor" },
+  { include = "p1monitor" },
 ]
 
 [tool.poetry.dependencies]
 aiohttp = ">=3.0.0"
 python = "^3.9"
 yarl = ">=1.6.0"
 
 [tool.poetry.urls]
 "Bug Tracker" = "https://github.com/klaasnicolaas/python-p1monitor/issues"
 Changelog = "https://github.com/klaasnicolaas/python-p1monitor/releases"
 
 [tool.poetry.group.dev.dependencies]
-ruff = "^0.0.244"
-aresponses = "^2.1.6"
-black = "^22.12"
-blacken-docs = "^1.13.0"
-codespell = "^2.2.2"
-coverage = {version = "^6.5", extras = ["toml"]}
-mypy = "^0.991"
-pre-commit = "^3.0.3"
-pre-commit-hooks = "^4.4.0"
-pylint = "^2.16.1"
-pytest = "^7.2.1"
-pytest-asyncio = "^0.20.3"
-pytest-cov = "^4.0.0"
-safety = "^2.3.5"
-yamllint = "^1.29.0"
-covdefaults = "^2.2.2"
-
-[tool.black]
-target-version = ['py39']
-
-[tool.coverage.paths]
-source = ["p1monitor"]
+aresponses = "2.1.6"
+black = "23.3.0"
+blacken-docs = "1.13.0"
+codespell = "2.2.4"
+covdefaults = "2.3.0"
+coverage = {version = "7.2.5", extras = ["toml"]}
+mypy = "1.3.0"
+pre-commit = "3.3.2"
+pre-commit-hooks = "4.4.0"
+pylint = "2.17.4"
+pytest = "7.3.1"
+pytest-asyncio = "0.21.0"
+pytest-cov = "4.0.0"
+ruff = "0.0.269"
+yamllint = "1.31.0"
 
 [tool.coverage.run]
 plugins = ["covdefaults"]
 source = ["p1monitor"]
 
 [tool.coverage.report]
 fail_under = 90
+show_missing = true
 
 [tool.mypy]
 # Specify the target platform details in config, so your developers are
 # free to run mypy on Windows, Linux, or macOS and get consistent
 # results.
 platform = "linux"
 python_version = "3.9"
 
+# flake8-mypy expects the two following for sensible formatting
+show_column_numbers = true
+
 # show error messages from unrelated files
 follow_imports = "normal"
 
 # suppress errors about unsatisfied imports
 ignore_missing_imports = true
 
 # be strict
 check_untyped_defs = true
 disallow_any_generics = true
 disallow_incomplete_defs = true
 disallow_subclassing_any = true
 disallow_untyped_calls = true
-disallow_untyped_defs = true
 disallow_untyped_decorators = true
+disallow_untyped_defs = true
 no_implicit_optional = true
 no_implicit_reexport = true
 strict_optional = true
 warn_incomplete_stub = true
 warn_no_return = true
 warn_redundant_casts = true
 warn_return_any = true
 warn_unused_configs = true
 warn_unused_ignores = true
 
-[tool.pylint.MASTER]
-extension-pkg-whitelist = [
-  "pydantic"
-]
-ignore= [
-  "tests"
-]
-
 [tool.pylint.BASIC]
 good-names = [
-    "_",
-    "ex",
-    "fp",
-    "i",
-    "id",
-    "j",
-    "k",
-    "on",
-    "Run",
-    "T",
+  "_",
+  "ex",
+  "fp",
+  "i",
+  "id",
+  "j",
+  "k",
+  "on",
+  "Run",
+  "T",
+  "vw",
 ]
 
-[tool.pylint.DESIGN]
-max-attributes = 15
-
 [tool.pylint."MESSAGES CONTROL"]
 disable= [
-    "duplicate-code",
-    "format",
-    "unsubscriptable-object",
+  "duplicate-code",
+  "format",
+  "unsubscriptable-object",
 ]
 
 [tool.pylint.SIMILARITIES]
 ignore-imports = true
 
 [tool.pylint.FORMAT]
-max-line-length=88
+max-line-length = 88
+
+[tool.pylint.DESIGN]
+max-attributes = 15
 
 [tool.pytest.ini_options]
 addopts = "--cov"
 asyncio_mode = "auto"
 
 [tool.ruff]
 select = ["ALL"]
@@ -151,15 +141,15 @@
 ]
 
 [tool.ruff.flake8-pytest-style]
 mark-parentheses = false
 fixture-parentheses = false
 
 [tool.ruff.isort]
-known-first-party = ["easyenergy"]
+known-first-party = ["p1monitor"]
 
 [tool.ruff.mccabe]
 max-complexity = 25
 
 [build-system]
-requires = ["poetry-core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
+requires = ["poetry-core>=1.0.0"]
```

### Comparing `p1monitor-2.3.0/setup.py` & `p1monitor-2.3.1/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,30 +1,233 @@
-# -*- coding: utf-8 -*-
-from setuptools import setup
+Metadata-Version: 2.1
+Name: p1monitor
+Version: 2.3.1
+Summary: Asynchronous Python client for the P1 Monitor
+Home-page: https://github.com/klaasnicolaas/python-p1monitor
+License: MIT
+Keywords: p1,monitor,power,energy,api,async,client
+Author: Klaas Schoute
+Author-email: hello@student-techlife.com
+Maintainer: Klaas Schoute
+Maintainer-email: hello@student-techlife.com
+Requires-Python: >=3.9,<4.0
+Classifier: Development Status :: 5 - Production/Stable
+Classifier: Framework :: AsyncIO
+Classifier: Intended Audience :: Developers
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Natural Language :: English
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Topic :: Software Development :: Libraries :: Python Modules
+Requires-Dist: aiohttp (>=3.0.0)
+Requires-Dist: yarl (>=1.6.0)
+Project-URL: Bug Tracker, https://github.com/klaasnicolaas/python-p1monitor/issues
+Project-URL: Changelog, https://github.com/klaasnicolaas/python-p1monitor/releases
+Project-URL: Documentation, https://github.com/klaasnicolaas/python-p1monitor
+Project-URL: Repository, https://github.com/klaasnicolaas/python-p1monitor
+Description-Content-Type: text/markdown
+
+<!-- Banner -->
+![alt Banner of the P1 Monitor package](https://raw.githubusercontent.com/klaasnicolaas/python-p1monitor/main/assets/header_p1monitor-min.png)
+
+<!-- PROJECT SHIELDS -->
+[![GitHub Release][releases-shield]][releases]
+[![Python Versions][python-versions-shield]][pypi]
+![Project Stage][project-stage-shield]
+![Project Maintenance][maintenance-shield]
+[![License][license-shield]](LICENSE)
+
+[![GitHub Activity][commits-shield]][commits-url]
+[![PyPi Downloads][downloads-shield]][downloads-url]
+[![GitHub Last Commit][last-commit-shield]][commits-url]
+[![Stargazers][stars-shield]][stars-url]
+[![Issues][issues-shield]][issues-url]
+
+[![Code Quality][code-quality-shield]][code-quality]
+[![Build Status][build-shield]][build-url]
+[![Typing Status][typing-shield]][typing-url]
+
+[![Maintainability][maintainability-shield]][maintainability-url]
+[![Code Coverage][codecov-shield]][codecov-url]
+
+Asynchronous Python client for the P1 Monitor API.
+
+## About
+
+There are many ways to read the serial port (P1) of your smart meter and what you do with the data that comes out. With this python library your platform can read [P1 Monitor][p1-monitor] via the API and use the data for example for an integration in [Home Assistant][home-assistant].
+
+## Installation
+
+```bash
+pip install p1monitor
+```
+
+## Usage
+
+```python
+import asyncio
+
+from p1monitor import P1Monitor
+
+
+async def main():
+    """Show example on getting P1 Monitor data."""
+    async with P1Monitor(host="example_host") as client:
+        smartmeter = await client.smartmeter()
+        watermeter = await client.watermeter()
+        settings = await client.settings()
+        phases = await client.phases()
+        print(smartmeter)
+        print(watermeter)
+        print(settings)
+        print(phases)
+
+
+if __name__ == "__main__":
+    asyncio.run(main())
+```
+
+## Data
+
+There is a lot of data that you can read via the API:
+
+### SmartMeter
+- Gas Consumption
+- Power Consumption / Production
+- Energy Consumption Low/High
+- Energy Production Low/High
+- Energy Tariff Period
+
+### Phases
+- Voltage phases L1/2/3
+- Current Phases L1/2/3
+- Power consumed phases L1/2/3
+- Power Produced phases L1/2/3
+
+### WaterMeter
+> **_NOTE:_**  WaterMeter is only available when you run version 1.1.0 or higher due the use of the new v2 API url.
+
+- Day Consumption (liters)
+- Total Consumption (m3)
+- Day Pulse count
+
+### Settings
+- Gas Consumption Price
+- Energy Consumption Price Low/High
+- Energy Production Price Low/High
+
+## Contributing
+
+This is an active open-source project. We are always open to people who want to
+use the code or contribute to it.
+
+We've set up a separate document for our
+[contribution guidelines](CONTRIBUTING.md).
+
+Thank you for being involved! :heart_eyes:
+
+## Setting up development environment
+
+This Python project is fully managed using the [Poetry][poetry] dependency
+manager.
+
+You need at least:
+
+- Python 3.9+
+- [Poetry][poetry-install]
+
+Install all packages, including all development requirements:
+
+```bash
+poetry install
+```
+
+Poetry creates by default an virtual environment where it installs all
+necessary pip packages, to enter or exit the venv run the following commands:
+
+```bash
+poetry shell
+exit
+```
+
+Setup the pre-commit check, you must run this inside the virtual environment:
+
+```bash
+pre-commit install
+```
+
+*Now you're all set to get started!*
+
+As this repository uses the [pre-commit][pre-commit] framework, all changes
+are linted and tested with each commit. You can run all checks and tests
+manually, using the following command:
+
+```bash
+poetry run pre-commit run --all-files
+```
+
+To run just the Python tests:
+
+```bash
+poetry run pytest
+```
+
+## License
+
+MIT License
+
+Copyright (c) 2021-2023 Klaas Schoute
+
+Permission is hereby granted, free of charge, to any person obtaining a copy
+of this software and associated documentation files (the "Software"), to deal
+in the Software without restriction, including without limitation the rights
+to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
+copies of the Software, and to permit persons to whom the Software is
+furnished to do so, subject to the following conditions:
+
+The above copyright notice and this permission notice shall be included in all
+copies or substantial portions of the Software.
+
+THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
+IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
+FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
+AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
+LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
+OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
+SOFTWARE.
+
+<!-- MARKDOWN LINKS & IMAGES -->
+[build-shield]: https://github.com/klaasnicolaas/python-p1monitor/actions/workflows/tests.yaml/badge.svg
+[build-url]: https://github.com/klaasnicolaas/python-p1monitor/actions/workflows/tests.yaml
+[code-quality-shield]: https://github.com/klaasnicolaas/python-p1monitor/actions/workflows/codeql.yaml/badge.svg
+[code-quality]: https://github.com/klaasnicolaas/python-p1monitor/actions/workflows/codeql.yaml
+[commits-shield]: https://img.shields.io/github/commit-activity/y/klaasnicolaas/python-p1monitor.svg
+[commits-url]: https://github.com/klaasnicolaas/python-p1monitor/commits/main
+[codecov-shield]: https://codecov.io/gh/klaasnicolaas/python-p1monitor/branch/main/graph/badge.svg?token=G4FIVHJVZR
+[codecov-url]: https://codecov.io/gh/klaasnicolaas/python-p1monitor
+[downloads-shield]: https://img.shields.io/pypi/dm/p1monitor
+[downloads-url]: https://pypistats.org/packages/p1monitor
+[issues-shield]: https://img.shields.io/github/issues/klaasnicolaas/python-p1monitor.svg
+[issues-url]: https://github.com/klaasnicolaas/python-p1monitor/issues
+[license-shield]: https://img.shields.io/github/license/klaasnicolaas/python-p1monitor.svg
+[last-commit-shield]: https://img.shields.io/github/last-commit/klaasnicolaas/python-p1monitor.svg
+[maintenance-shield]: https://img.shields.io/maintenance/yes/2023.svg
+[maintainability-shield]: https://api.codeclimate.com/v1/badges/443c476612a574d82467/maintainability
+[maintainability-url]: https://codeclimate.com/github/klaasnicolaas/python-p1monitor/maintainability
+[project-stage-shield]: https://img.shields.io/badge/project%20stage-production%20ready-brightgreen.svg
+[pypi]: https://pypi.org/project/p1monitor/
+[python-versions-shield]: https://img.shields.io/pypi/pyversions/p1monitor
+[typing-shield]: https://github.com/klaasnicolaas/python-p1monitor/actions/workflows/typing.yaml/badge.svg
+[typing-url]: https://github.com/klaasnicolaas/python-p1monitor/actions/workflows/typing.yaml
+[releases-shield]: https://img.shields.io/github/release/klaasnicolaas/python-p1monitor.svg
+[releases]: https://github.com/klaasnicolaas/python-p1monitor/releases
+[stars-shield]: https://img.shields.io/github/stars/klaasnicolaas/python-p1monitor.svg
+[stars-url]: https://github.com/klaasnicolaas/python-p1monitor/stargazers
+
+[p1-monitor]: https://www.ztatz.nl/p1-monitor
+[home-assistant]: https://www.home-assistant.io
+[poetry-install]: https://python-poetry.org/docs/#installation
+[poetry]: https://python-poetry.org
+[pre-commit]: https://pre-commit.com
 
-packages = \
-['p1monitor']
-
-package_data = \
-{'': ['*']}
-
-install_requires = \
-['aiohttp>=3.0.0', 'yarl>=1.6.0']
-
-setup_kwargs = {
-    'name': 'p1monitor',
-    'version': '2.3.0',
-    'description': 'Asynchronous Python client for the P1 Monitor',
-    'long_description': '<!-- Banner -->\n![alt Banner of the P1 Monitor package](https://raw.githubusercontent.com/klaasnicolaas/python-p1monitor/main/assets/header_p1monitor-min.png)\n\n<!-- PROJECT SHIELDS -->\n[![GitHub Release][releases-shield]][releases]\n[![Python Versions][python-versions-shield]][pypi]\n![Project Stage][project-stage-shield]\n![Project Maintenance][maintenance-shield]\n[![License][license-shield]](LICENSE)\n\n[![GitHub Activity][commits-shield]][commits-url]\n[![PyPi Downloads][downloads-shield]][downloads-url]\n[![GitHub Last Commit][last-commit-shield]][commits-url]\n[![Stargazers][stars-shield]][stars-url]\n[![Issues][issues-shield]][issues-url]\n\n[![Code Quality][code-quality-shield]][code-quality]\n[![Build Status][build-shield]][build-url]\n[![Typing Status][typing-shield]][typing-url]\n\n[![Maintainability][maintainability-shield]][maintainability-url]\n[![Code Coverage][codecov-shield]][codecov-url]\n\nAsynchronous Python client for the P1 Monitor API.\n\n## About\n\nThere are many ways to read the serial port (P1) of your smart meter and what you do with the data that comes out. With this python library your platform can read [P1 Monitor][p1-monitor] via the API and use the data for example for an integration in [Home Assistant][home-assistant].\n\n## Installation\n\n```bash\npip install p1monitor\n```\n\n## Usage\n\n```python\nimport asyncio\n\nfrom p1monitor import P1Monitor\n\n\nasync def main():\n    """Show example on getting P1 Monitor data."""\n    async with P1Monitor(host="example_host") as client:\n        smartmeter = await client.smartmeter()\n        watermeter = await client.watermeter()\n        settings = await client.settings()\n        phases = await client.phases()\n        print(smartmeter)\n        print(watermeter)\n        print(settings)\n        print(phases)\n\n\nif __name__ == "__main__":\n    asyncio.run(main())\n```\n\n## Data\n\nThere is a lot of data that you can read via the API:\n\n### SmartMeter\n- Gas Consumption\n- Power Consumption / Production\n- Energy Consumption Low/High\n- Energy Production Low/High\n- Energy Tariff Period\n\n### Phases\n- Voltage phases L1/2/3\n- Current Phases L1/2/3\n- Power consumed phases L1/2/3\n- Power Produced phases L1/2/3\n\n### WaterMeter\n> **_NOTE:_**  WaterMeter is only available when you run version 1.1.0 or higher due the use of the new v2 API url.\n\n- Day Consumption (liters)\n- Total Consumption (m3)\n- Day Pulse count\n\n### Settings\n- Gas Consumption Price\n- Energy Consumption Price Low/High\n- Energy Production Price Low/High\n\n## Contributing\n\nThis is an active open-source project. We are always open to people who want to\nuse the code or contribute to it.\n\nWe\'ve set up a separate document for our\n[contribution guidelines](CONTRIBUTING.md).\n\nThank you for being involved! :heart_eyes:\n\n## Setting up development environment\n\nThis Python project is fully managed using the [Poetry][poetry] dependency\nmanager.\n\nYou need at least:\n\n- Python 3.9+\n- [Poetry][poetry-install]\n\nInstall all packages, including all development requirements:\n\n```bash\npoetry install\n```\n\nPoetry creates by default an virtual environment where it installs all\nnecessary pip packages, to enter or exit the venv run the following commands:\n\n```bash\npoetry shell\nexit\n```\n\nSetup the pre-commit check, you must run this inside the virtual environment:\n\n```bash\npre-commit install\n```\n\n*Now you\'re all set to get started!*\n\nAs this repository uses the [pre-commit][pre-commit] framework, all changes\nare linted and tested with each commit. You can run all checks and tests\nmanually, using the following command:\n\n```bash\npoetry run pre-commit run --all-files\n```\n\nTo run just the Python tests:\n\n```bash\npoetry run pytest\n```\n\n## License\n\nMIT License\n\nCopyright (c) 2021-2023 Klaas Schoute\n\nPermission is hereby granted, free of charge, to any person obtaining a copy\nof this software and associated documentation files (the "Software"), to deal\nin the Software without restriction, including without limitation the rights\nto use, copy, modify, merge, publish, distribute, sublicense, and/or sell\ncopies of the Software, and to permit persons to whom the Software is\nfurnished to do so, subject to the following conditions:\n\nThe above copyright notice and this permission notice shall be included in all\ncopies or substantial portions of the Software.\n\nTHE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR\nIMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,\nFITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE\nAUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER\nLIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,\nOUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE\nSOFTWARE.\n\n<!-- MARKDOWN LINKS & IMAGES -->\n[build-shield]: https://github.com/klaasnicolaas/python-p1monitor/actions/workflows/tests.yaml/badge.svg\n[build-url]: https://github.com/klaasnicolaas/python-p1monitor/actions/workflows/tests.yaml\n[code-quality-shield]: https://github.com/klaasnicolaas/python-p1monitor/actions/workflows/codeql.yaml/badge.svg\n[code-quality]: https://github.com/klaasnicolaas/python-p1monitor/actions/workflows/codeql.yaml\n[commits-shield]: https://img.shields.io/github/commit-activity/y/klaasnicolaas/python-p1monitor.svg\n[commits-url]: https://github.com/klaasnicolaas/python-p1monitor/commits/main\n[codecov-shield]: https://codecov.io/gh/klaasnicolaas/python-p1monitor/branch/main/graph/badge.svg?token=G4FIVHJVZR\n[codecov-url]: https://codecov.io/gh/klaasnicolaas/python-p1monitor\n[downloads-shield]: https://img.shields.io/pypi/dm/p1monitor\n[downloads-url]: https://pypistats.org/packages/p1monitor\n[issues-shield]: https://img.shields.io/github/issues/klaasnicolaas/python-p1monitor.svg\n[issues-url]: https://github.com/klaasnicolaas/python-p1monitor/issues\n[license-shield]: https://img.shields.io/github/license/klaasnicolaas/python-p1monitor.svg\n[last-commit-shield]: https://img.shields.io/github/last-commit/klaasnicolaas/python-p1monitor.svg\n[maintenance-shield]: https://img.shields.io/maintenance/yes/2023.svg\n[maintainability-shield]: https://api.codeclimate.com/v1/badges/443c476612a574d82467/maintainability\n[maintainability-url]: https://codeclimate.com/github/klaasnicolaas/python-p1monitor/maintainability\n[project-stage-shield]: https://img.shields.io/badge/project%20stage-production%20ready-brightgreen.svg\n[pypi]: https://pypi.org/project/p1monitor/\n[python-versions-shield]: https://img.shields.io/pypi/pyversions/p1monitor\n[typing-shield]: https://github.com/klaasnicolaas/python-p1monitor/actions/workflows/typing.yaml/badge.svg\n[typing-url]: https://github.com/klaasnicolaas/python-p1monitor/actions/workflows/typing.yaml\n[releases-shield]: https://img.shields.io/github/release/klaasnicolaas/python-p1monitor.svg\n[releases]: https://github.com/klaasnicolaas/python-p1monitor/releases\n[stars-shield]: https://img.shields.io/github/stars/klaasnicolaas/python-p1monitor.svg\n[stars-url]: https://github.com/klaasnicolaas/python-p1monitor/stargazers\n\n[p1-monitor]: https://www.ztatz.nl/p1-monitor\n[home-assistant]: https://www.home-assistant.io\n[poetry-install]: https://python-poetry.org/docs/#installation\n[poetry]: https://python-poetry.org\n[pre-commit]: https://pre-commit.com\n',
-    'author': 'Klaas Schoute',
-    'author_email': 'hello@student-techlife.com',
-    'maintainer': 'Klaas Schoute',
-    'maintainer_email': 'hello@student-techlife.com',
-    'url': 'https://github.com/klaasnicolaas/python-p1monitor',
-    'packages': packages,
-    'package_data': package_data,
-    'install_requires': install_requires,
-    'python_requires': '>=3.9,<4.0',
-}
-
-
-setup(**setup_kwargs)
```

