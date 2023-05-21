# Comparing `tmp/hstsparser-1.1.4.tar.gz` & `tmp/hstsparser-1.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hstsparser-1.1.4.tar", last modified: Sat Jan 18 15:06:04 2020, max compression
+gzip compressed data, was "hstsparser-1.1.5.tar", max compression
```

## Comparing `hstsparser-1.1.4.tar` & `hstsparser-1.1.5.tar`

### file list

```diff
@@ -1,6 +1,5 @@
--rw-r--r--   0        0        0     6405 2020-01-18 15:05:27.175202 hstsparser-1.1.4/hstsparser.py
--rw-r--r--   0        0        0     1091 2020-01-18 15:05:27.175202 hstsparser-1.1.4/LICENSE
--rw-r--r--   0        0        0     1289 2020-01-18 15:05:47.679726 hstsparser-1.1.4/pyproject.toml
--rw-r--r--   0        0        0     3156 2020-01-18 15:05:27.175202 hstsparser-1.1.4/README.md
--rw-r--r--   0        0        0     3927 2020-01-18 15:06:04.939581 hstsparser-1.1.4/setup.py
--rw-r--r--   0        0        0     3917 2020-01-18 15:06:04.939581 hstsparser-1.1.4/PKG-INFO
+-rw-r--r--   0        0        0     1070 2023-05-21 01:15:54.056178 hstsparser-1.1.5/LICENSE
+-rw-r--r--   0        0        0     2727 2023-05-21 01:15:54.056178 hstsparser-1.1.5/README.md
+-rw-r--r--   0        0        0     6257 2023-05-21 01:15:54.056178 hstsparser-1.1.5/hstsparser.py
+-rw-r--r--   0        0        0     1351 2023-05-21 01:16:15.856489 hstsparser-1.1.5/pyproject.toml
+-rw-r--r--   0        0        0     3642 1970-01-01 00:00:00.000000 hstsparser-1.1.5/PKG-INFO
```

### Comparing `hstsparser-1.1.4/hstsparser.py` & `hstsparser-1.1.5/hstsparser.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,194 +1,196 @@
-import csv
-import datetime
-import json
-import os
-import re
-import typing
-from argparse import ArgumentParser, Namespace
-from base64 import b64encode
-from hashlib import sha256
-
-from prettytable import PrettyTable
-
-
-def convert_domain(domain: str) -> str:
-    """Convert string to the Google Chrome domain format"""
-    output = [chr(0)]
-    idx = 0
-    for char in reversed(domain):
-        if char == ".":
-            output.append(chr(idx))
-            idx = 0
-        else:
-            output.append(char)
-            idx += 1
-    output.append(chr(idx))
-    return b64encode(sha256("".join(reversed(output)).encode("utf-8")).digest())
-
-
-def print_db(database: list, field_names: list) -> None:
-    """Print the database in a formatted table"""
-    table = PrettyTable()
-    table.field_names = field_names
-    for i in database:
-        table.add_row(i)
-    print(table)
-
-
-def serial_date_to_string(srl_no: str) -> str:
-    """Convert serial date object to printable string"""
-    new_date = datetime.datetime.utcfromtimestamp(0) + datetime.timedelta(int(srl_no))
-    return new_date.strftime("%Y-%m-%d")
-
-
-def is_valid_file(parser: ArgumentParser, arg: str) -> typing.TextIO:
-    """Check that file already exists"""
-    if not os.path.exists(arg):
-        parser.error(f"The file {arg} does not exist!")
-    else:
-        return open(arg, "r")
-
-
-def file_already_exists(parser: ArgumentParser, arg: str) -> typing.TextIO:
-    """Check that the file does not already exist"""
-    if os.path.exists(arg):
-        parser.error(f"The file {arg} already exists!")
-    else:
-        return open(arg, "w", newline="")
-
-
-def print_if_no_args(args: Namespace, database: list, field_names: list) -> None:
-    """Print database if no output file has been specified"""
-    if not args.csv_file:
-        print_db(database, field_names)
-    else:
-        file_write(args, database, field_names)
-
-
-def file_write(args: Namespace, database: list, field_names: list) -> None:
-    """Write to a CSV file"""
-    if args.csv_file:
-        with args.csv_file as csvfile:
-            csvfile = csv.writer(csvfile)
-            csvfile.writerow(field_names)
-            for i in database:
-                csvfile.writerow(i)
-
-
-def date_round(date: datetime.datetime) -> datetime.datetime:
-    """Round `datetime` object"""
-    return date - datetime.timedelta(
-        minutes=date.minute % 10, seconds=date.second, microseconds=date.microsecond
-    )
-
-
-parser = ArgumentParser(description="Process HSTS databases")
-parser.add_argument(
-    dest="database_file",
-    help="The path to the database to be processed",
-    metavar="FILE",
-    type=lambda x: is_valid_file(parser, x),
-)
-parser.add_argument(
-    "-w",
-    dest="wordlist_file",
-    help="The path to the database to be processed",
-    metavar="WORDLIST",
-    type=lambda x: is_valid_file(parser, x),
-)
-parser.add_argument(
-    "--csv",
-    dest="csv_file",
-    help="Output to a CSV file",
-    metavar="CSV",
-    type=lambda x: file_already_exists(parser, x),
-)
-group = parser.add_mutually_exclusive_group(required=True)
-group.add_argument("--firefox", action="store_true", help="Process a Firefox database")
-group.add_argument("--chrome", action="store_true", help="Process a Chrome database")
-
-
-def main() -> None:
-    """Entry point for command line alias."""
-    args = parser.parse_args()
-
-    dirtydb = args.database_file.read()
-    database = []
-
-    if args.firefox:
-        dirtydb = dirtydb.split("\n")
-        for i in dirtydb:
-            if i != "":
-                record = re.split(r"\t+", i)
-                record.append(record[0][-4:])
-                record[0] = re.search(r"^([^:\^]+)", record[0]).group(0)
-                record[2] = serial_date_to_string(record[2])
-                cleaned = record[3].split(",")
-                try:
-                    record[3] = datetime.datetime.fromtimestamp(int(cleaned[0]) / 1000)
-                except (OSError, ValueError):
-                    record[3] = datetime.datetime.fromtimestamp(32503680000)  # 3000-01-01 00:00:00
-                if int(cleaned[2]):
-                    record.append("Yes")
-                else:
-                    record.append("No")
-                if args.csv_file:
-                    record[3] = date_round(record[3])
-                database.append(record)
-        print_if_no_args(
-            args,
-            database,
-            ["URL", "Visits", "Last Accessed", "Expiry", "Type", "Include Subdomains"],
-        )
-
-    if args.chrome:
-        dirtydb = json.loads(dirtydb)
-        for i in dirtydb:
-            current = dirtydb[i]
-            if "expect_ct" not in current:
-                if bool(current["sts_include_subdomains"]):
-                    subdomains = "Yes"
-                else:
-                    subdomains = "No"
-                record = [
-                    i,
-                    datetime.datetime.fromtimestamp(current["expiry"]),
-                    subdomains,
-                    datetime.datetime.fromtimestamp(current["sts_observed"]),
-                ]
-                if args.csv_file:
-                    record[1] = date_round(record[1])
-                    record[3] = date_round(record[3])
-                database.append(record)
-        if args.wordlist_file:
-            wordlist = args.wordlist_file.read().splitlines()
-            rainbow = []
-            for i in wordlist:
-                rainbow.append(convert_domain(i))
-            for i in database:
-                for j in range(0, len(rainbow)):
-                    if i[0] == rainbow[j].decode("utf-8"):
-                        i.append(wordlist[j])
-                if len(i) == 4:
-                    i.append("")
-            print_if_no_args(
-                args,
-                database,
-                [
-                    "Base64 URL Hash",
-                    "Expiry",
-                    "Include Subdomains",
-                    "Last Observed",
-                    "Cracked Hash",
-                ],
-            )
-        else:
-            print_if_no_args(
-                args,
-                database,
-                ["Base64 URL Hash", "Expiry", "Include Subdomains", "Last Observed"],
-            )
-
-
-if __name__ == '__main__':
-    main()
+import csv
+import datetime
+import json
+import os
+import re
+import typing
+from argparse import ArgumentParser, Namespace
+from base64 import b64encode
+from hashlib import sha256
+
+from prettytable import PrettyTable
+
+
+def convert_domain(domain: str) -> str:
+    """Convert string to the Google Chrome domain format"""
+    output = [chr(0)]
+    idx = 0
+    for char in reversed(domain):
+        if char == ".":
+            output.append(chr(idx))
+            idx = 0
+        else:
+            output.append(char)
+            idx += 1
+    output.append(chr(idx))
+    return b64encode(sha256("".join(reversed(output)).encode("utf-8")).digest())
+
+
+def print_db(database: list, field_names: list) -> None:
+    """Print the database in a formatted table"""
+    table = PrettyTable()
+    table.field_names = field_names
+    for i in database:
+        table.add_row(i)
+    print(table)
+
+
+def serial_date_to_string(srl_no: str) -> str:
+    """Convert serial date object to printable string"""
+    new_date = datetime.datetime.utcfromtimestamp(0) + datetime.timedelta(int(srl_no))
+    return new_date.strftime("%Y-%m-%d")
+
+
+def is_valid_file(parser: ArgumentParser, arg: str) -> typing.TextIO:
+    """Check that file already exists"""
+    if not os.path.exists(arg):
+        parser.error(f"The file {arg} does not exist!")
+    else:
+        return open(arg, "r")
+
+
+def file_already_exists(parser: ArgumentParser, arg: str) -> typing.TextIO:
+    """Check that the file does not already exist"""
+    if os.path.exists(arg):
+        parser.error(f"The file {arg} already exists!")
+    else:
+        return open(arg, "w", newline="")
+
+
+def print_if_no_args(args: Namespace, database: list, field_names: list) -> None:
+    """Print database if no output file has been specified"""
+    if not args.csv_file:
+        print_db(database, field_names)
+    else:
+        file_write(args, database, field_names)
+
+
+def file_write(args: Namespace, database: list, field_names: list) -> None:
+    """Write to a CSV file"""
+    if args.csv_file:
+        with args.csv_file as csvfile:
+            csvfile = csv.writer(csvfile)
+            csvfile.writerow(field_names)
+            for i in database:
+                csvfile.writerow(i)
+
+
+def date_round(date: datetime.datetime) -> datetime.datetime:
+    """Round `datetime` object"""
+    return date - datetime.timedelta(
+        minutes=date.minute % 10, seconds=date.second, microseconds=date.microsecond
+    )
+
+
+parser = ArgumentParser(description="Process HSTS databases")
+parser.add_argument(
+    dest="database_file",
+    help="The path to the database to be processed",
+    metavar="FILE",
+    type=lambda x: is_valid_file(parser, x),
+)
+parser.add_argument(
+    "-w",
+    dest="wordlist_file",
+    help="The path to the database to be processed",
+    metavar="WORDLIST",
+    type=lambda x: is_valid_file(parser, x),
+)
+parser.add_argument(
+    "--csv",
+    dest="csv_file",
+    help="Output to a CSV file",
+    metavar="CSV",
+    type=lambda x: file_already_exists(parser, x),
+)
+group = parser.add_mutually_exclusive_group(required=True)
+group.add_argument("--firefox", action="store_true", help="Process a Firefox database")
+group.add_argument("--chrome", action="store_true", help="Process a Chrome database")
+
+
+def main() -> None:
+    """Entry point for command line alias."""
+    args = parser.parse_args()
+
+    dirtydb = args.database_file.read()
+    database = []
+
+    if args.firefox:
+        dirtydb = dirtydb.split("\n")
+        for i in dirtydb:
+            if i != "":
+                record = re.split(r"\t+", i)
+                record.append(record[0][-4:])
+                record[0] = re.search(r"^([^:\^]+)", record[0]).group(0)
+                record[2] = serial_date_to_string(record[2])
+                cleaned = record[3].split(",")
+                try:
+                    record[3] = datetime.datetime.fromtimestamp(int(cleaned[0]) / 1000)
+                except (OSError, ValueError):
+                    record[3] = datetime.datetime.fromtimestamp(
+                        32503680000
+                    )  # 3000-01-01 00:00:00
+                if int(cleaned[2]):
+                    record.append("Yes")
+                else:
+                    record.append("No")
+                if args.csv_file:
+                    record[3] = date_round(record[3])
+                database.append(record)
+        print_if_no_args(
+            args,
+            database,
+            ["URL", "Visits", "Last Accessed", "Expiry", "Type", "Include Subdomains"],
+        )
+
+    if args.chrome:
+        dirtydb = json.loads(dirtydb)
+        for i in dirtydb:
+            current = dirtydb[i]
+            if "expect_ct" not in current:
+                if bool(current["sts_include_subdomains"]):
+                    subdomains = "Yes"
+                else:
+                    subdomains = "No"
+                record = [
+                    i,
+                    datetime.datetime.fromtimestamp(current["expiry"]),
+                    subdomains,
+                    datetime.datetime.fromtimestamp(current["sts_observed"]),
+                ]
+                if args.csv_file:
+                    record[1] = date_round(record[1])
+                    record[3] = date_round(record[3])
+                database.append(record)
+        if args.wordlist_file:
+            wordlist = args.wordlist_file.read().splitlines()
+            rainbow = []
+            for i in wordlist:
+                rainbow.append(convert_domain(i))
+            for i in database:
+                for j in range(0, len(rainbow)):
+                    if i[0] == rainbow[j].decode("utf-8"):
+                        i.append(wordlist[j])
+                if len(i) == 4:
+                    i.append("")
+            print_if_no_args(
+                args,
+                database,
+                [
+                    "Base64 URL Hash",
+                    "Expiry",
+                    "Include Subdomains",
+                    "Last Observed",
+                    "Cracked Hash",
+                ],
+            )
+        else:
+            print_if_no_args(
+                args,
+                database,
+                ["Base64 URL Hash", "Expiry", "Include Subdomains", "Last Observed"],
+            )
+
+
+if __name__ == "__main__":
+    main()
```

### Comparing `hstsparser-1.1.4/LICENSE` & `hstsparser-1.1.5/LICENSE`

 * *Ordering differences only*

 * *Files 23% similar despite different names*

```diff
@@ -1,21 +1,21 @@
-MIT License
-
-Copyright (c) 2019 Daniel Milnes
-
-Permission is hereby granted, free of charge, to any person obtaining a copy
-of this software and associated documentation files (the "Software"), to deal
-in the Software without restriction, including without limitation the rights
-to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
-copies of the Software, and to permit persons to whom the Software is
-furnished to do so, subject to the following conditions:
-
-The above copyright notice and this permission notice shall be included in all
-copies or substantial portions of the Software.
-
-THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
-IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
-FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
-AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
-LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
-OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
-SOFTWARE.
+MIT License
+
+Copyright (c) 2019 Daniel Milnes
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
```

### Comparing `hstsparser-1.1.4/README.md` & `hstsparser-1.1.5/README.md`

 * *Files 21% similar despite different names*

```diff
@@ -1,88 +1,74 @@
-# HSTS Parser
-
-[![Build Status](https://dev.azure.com/thebeanogamer/HSTSparser/_apis/build/status/Lint%20Pipeline?branchName=master)](https://dev.azure.com/thebeanogamer/HSTSparser/_build/latest?definitionId=2&branchName=master) [![Release Status](https://dev.azure.com/thebeanogamer/HSTSparser/_apis/build/status/Release%20Pipeline?branchName=master)](https://dev.azure.com/thebeanogamer/HSTSparser/_build/latest?definitionId=7&branchName=master) [![Licence](https://img.shields.io/github/license/thebeanogamer/hstsparser)](./LICENSE) ![Python 3.8.x](https://img.shields.io/badge/python-3.8.x-yellow.svg) [![PyPI](https://img.shields.io/pypi/v/hstsparser)](https://pypi.org/project/hstsparser)
-
-HSTS Parser is a simple tool to parse Firefox and Chrome's HSTS databases into actually helpful forensic artifacts! You can read more about the research behind this tool and potential uses for it over on [my blog](https://blog.daniel-milnes.uk/hsts-for-forensics-you-can-run-but-you-cant)!
-
-## Installation
-
-HSTS Parser can be installed via pip, or with [Poetry](https://python-poetry.org/).
-
-### From PyPi
-
-```bash
-pip install hstsparser
-```
-
-### Poetry (Linux)
-
-```bash
-curl -sSL https://raw.githubusercontent.com/python-poetry/poetry/master/get-poetry.py | python
-poetry install --no-dev
-```
-
-### Poetry (Windows)
-
-```powershell
-(Invoke-WebRequest -Uri https://raw.githubusercontent.com/python-poetry/poetry/master/get-poetry.py -UseBasicParsing).Content | python
-poetry install --no-dev
-```
-
-Alternatively, if you're using Windows, you can use the executables on the [releases page](https://github.com/thebeanogamer/hstsparser/releases/latest) to not need to install anything at all.
-
-## Usage
-
-All of the below documentation is written for the Python version rather than the standalone executable, but the commands will be the same.
-
-```shell
-$ hstsparser -h
-usage: hstsparser [-h] [-w WORDLIST] [--csv CSV] (--firefox | --chrome) FILE
-
-Process HSTS databases
-
-positional arguments:
-  FILE         The path to the database to be processed
-
-optional arguments:
-  -h, --help   show this help message and exit
-  -w WORDLIST  The path to the database to be processed
-  --csv CSV    Output to a CSV file
-  --firefox    Process a Firefox database
-  --chrome     Process a Chrome database
-```
-
-### Examples
-
-#### Firefox
-
-```shell
-hstsparser --firefox SiteSecurityServiceState.txt
-```
-
-#### Chrome
-
-```shell
-hstsparser --chrome TransportSecurity
-```
-
-#### Chrome with Wordlist
-
-```shell
-hstsparser -w wordlist.txt --chrome TransportSecurity
-```
-
-## Screenshots
-
-### Firefox
-
-![Screenshot of Firefox Processing](https://blog.daniel-milnes.uk/content/images/2019/11/image-3.png)
-
-### Chrome with Wordlist
-
-![Screenshot of Chrome Processing with a wordlist](https://blog.daniel-milnes.uk/content/images/2019/11/image-4.png)
-
-## Links
-
-- [My Blog Post](https://blog.daniel-milnes.uk/hsts-for-forensics-you-can-run-but-you-cant)
-- [MDN - HSTS](https://developer.mozilla.org/en-US/docs/Web/HTTP/Headers/Strict-Transport-Security)
-- [Chromium - HSTS](https://www.chromium.org/sts)
+# HSTS Parser
+
+[![Lint Codebase](https://github.com/thebeanogamer/hstsparser/actions/workflows/lint.yaml/badge.svg)](https://github.com/thebeanogamer/hstsparser/actions/workflows/lint.yaml) [![Build Releases](https://github.com/thebeanogamer/hstsparser/actions/workflows/build.yaml/badge.svg)](https://github.com/thebeanogamer/hstsparser/actions/workflows/build.yaml) [![Licence](https://img.shields.io/github/license/thebeanogamer/hstsparser)](./LICENSE) ![Python 3.11.x](https://img.shields.io/badge/python-3.11.x-yellow.svg) [![PyPI](https://img.shields.io/pypi/v/hstsparser)](https://pypi.org/project/hstsparser) [![Downloads](https://pepy.tech/badge/hstsparser)](https://pepy.tech/project/hstsparser)
+
+HSTS Parser is a simple tool to parse Firefox and Chrome's HSTS databases into actually helpful forensic artifacts! You can read more about the research behind this tool and potential uses for it over on [my blog](https://blog.daniel-milnes.uk/hsts-for-forensics-you-can-run-but-you-cant)!
+
+## Installation
+
+HSTS Parser can be installed via pip, or with [Poetry](https://python-poetry.org/).
+
+### From PyPi
+
+```bash
+pip install hstsparser
+```
+
+Alternatively, if you're using Windows, you can use the executables on the [releases page](https://github.com/thebeanogamer/hstsparser/releases/latest) to not need to install anything at all.
+
+## Usage
+
+All of the below documentation is written for the Python version rather than the standalone executable, but the commands will be the same.
+
+```shell
+$ hstsparser -h
+usage: hstsparser [-h] [-w WORDLIST] [--csv CSV] (--firefox | --chrome) FILE
+
+Process HSTS databases
+
+positional arguments:
+  FILE         The path to the database to be processed
+
+optional arguments:
+  -h, --help   show this help message and exit
+  -w WORDLIST  The path to the database to be processed
+  --csv CSV    Output to a CSV file
+  --firefox    Process a Firefox database
+  --chrome     Process a Chrome database
+```
+
+### Examples
+
+#### Firefox
+
+```shell
+hstsparser --firefox SiteSecurityServiceState.txt
+```
+
+#### Chrome
+
+```shell
+hstsparser --chrome TransportSecurity
+```
+
+#### Chrome with Wordlist
+
+```shell
+hstsparser -w wordlist.txt --chrome TransportSecurity
+```
+
+## Screenshots
+
+### Firefox
+
+![Screenshot of Firefox Processing](https://blog.daniel-milnes.uk/content/images/2019/11/image-3.png)
+
+### Chrome with Wordlist
+
+![Screenshot of Chrome Processing with a wordlist](https://blog.daniel-milnes.uk/content/images/2019/11/image-4.png)
+
+## Links
+
+- [My Blog Post](https://blog.daniel-milnes.uk/hsts-for-forensics-you-can-run-but-you-cant)
+- [MDN - HSTS](https://developer.mozilla.org/en-US/docs/Web/HTTP/Headers/Strict-Transport-Security)
+- [Chromium - HSTS](https://www.chromium.org/sts)
```

### Comparing `hstsparser-1.1.4/PKG-INFO` & `hstsparser-1.1.5/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,59 +1,46 @@
 Metadata-Version: 2.1
 Name: hstsparser
-Version: 1.1.4
+Version: 1.1.5
 Summary: A tool to parse Firefox and Chrome HSTS databases into forensic artifacts.
 Home-page: https://github.com/thebeanogamer/hstsparser
 License: MIT
 Keywords: chrome,firefox,dfir,forensics,hsts
 Author: Daniel Milnes
-Author-email: thebeanogamer@gmail.com
-Requires-Python: >=3.8,<4.0
+Author-email: daniel@daniel-milnes.uk
+Requires-Python: >=3.9,<3.12
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Natural Language :: English
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Security
 Classifier: Topic :: Utilities
 Requires-Dist: PTable (>=0.9.2,<0.10.0)
-Requires-Dist: argparse (>=1.4,<2.0)
 Project-URL: Documentation, https://github.com/thebeanogamer/hstsparser
 Project-URL: Repository, https://github.com/thebeanogamer/hstsparser
 Description-Content-Type: text/markdown
 
 # HSTS Parser
 
-[![Build Status](https://dev.azure.com/thebeanogamer/HSTSparser/_apis/build/status/Lint%20Pipeline?branchName=master)](https://dev.azure.com/thebeanogamer/HSTSparser/_build/latest?definitionId=2&branchName=master) [![Release Status](https://dev.azure.com/thebeanogamer/HSTSparser/_apis/build/status/Release%20Pipeline?branchName=master)](https://dev.azure.com/thebeanogamer/HSTSparser/_build/latest?definitionId=7&branchName=master) [![Licence](https://img.shields.io/github/license/thebeanogamer/hstsparser)](./LICENSE) ![Python 3.8.x](https://img.shields.io/badge/python-3.8.x-yellow.svg) [![PyPI](https://img.shields.io/pypi/v/hstsparser)](https://pypi.org/project/hstsparser)
+[![Lint Codebase](https://github.com/thebeanogamer/hstsparser/actions/workflows/lint.yaml/badge.svg)](https://github.com/thebeanogamer/hstsparser/actions/workflows/lint.yaml) [![Build Releases](https://github.com/thebeanogamer/hstsparser/actions/workflows/build.yaml/badge.svg)](https://github.com/thebeanogamer/hstsparser/actions/workflows/build.yaml) [![Licence](https://img.shields.io/github/license/thebeanogamer/hstsparser)](./LICENSE) ![Python 3.11.x](https://img.shields.io/badge/python-3.11.x-yellow.svg) [![PyPI](https://img.shields.io/pypi/v/hstsparser)](https://pypi.org/project/hstsparser) [![Downloads](https://pepy.tech/badge/hstsparser)](https://pepy.tech/project/hstsparser)
 
 HSTS Parser is a simple tool to parse Firefox and Chrome's HSTS databases into actually helpful forensic artifacts! You can read more about the research behind this tool and potential uses for it over on [my blog](https://blog.daniel-milnes.uk/hsts-for-forensics-you-can-run-but-you-cant)!
 
 ## Installation
 
 HSTS Parser can be installed via pip, or with [Poetry](https://python-poetry.org/).
 
 ### From PyPi
 
 ```bash
 pip install hstsparser
 ```
 
-### Poetry (Linux)
-
-```bash
-curl -sSL https://raw.githubusercontent.com/python-poetry/poetry/master/get-poetry.py | python
-poetry install --no-dev
-```
-
-### Poetry (Windows)
-
-```powershell
-(Invoke-WebRequest -Uri https://raw.githubusercontent.com/python-poetry/poetry/master/get-poetry.py -UseBasicParsing).Content | python
-poetry install --no-dev
-```
-
 Alternatively, if you're using Windows, you can use the executables on the [releases page](https://github.com/thebeanogamer/hstsparser/releases/latest) to not need to install anything at all.
 
 ## Usage
 
 All of the below documentation is written for the Python version rather than the standalone executable, but the commands will be the same.
 
 ```shell
```

