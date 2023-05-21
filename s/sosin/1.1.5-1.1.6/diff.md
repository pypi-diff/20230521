# Comparing `tmp/sosin-1.1.5.tar.gz` & `tmp/sosin-1.1.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sosin-1.1.5.tar", last modified: Mon May 15 08:04:26 2023, max compression
+gzip compressed data, was "sosin-1.1.6.tar", last modified: Sun May 21 13:59:45 2023, max compression
```

## Comparing `sosin-1.1.5.tar` & `sosin-1.1.6.tar`

### file list

```diff
@@ -1,31 +1,31 @@
-drwxr-xr-x   0 sosin      (501) staff       (20)        0 2023-05-15 08:04:26.463348 sosin-1.1.5/
--rwx------   0 sosin      (501) staff       (20)     1083 2023-04-17 11:46:46.000000 sosin-1.1.5/LICENSE
--rw-r--r--   0 sosin      (501) staff       (20)     1250 2023-05-15 08:04:26.463136 sosin-1.1.5/PKG-INFO
--rwx------   0 sosin      (501) staff       (20)      863 2023-04-17 11:46:46.000000 sosin-1.1.5/README.md
--rw-r--r--   0 sosin      (501) staff       (20)       38 2023-05-15 08:04:26.463416 sosin-1.1.5/setup.cfg
--rwx------   0 sosin      (501) staff       (20)      984 2023-05-15 08:02:34.000000 sosin-1.1.5/setup.py
-drwxr-xr-x   0 sosin      (501) staff       (20)        0 2023-05-15 08:04:26.458250 sosin-1.1.5/sosin/
--rwx------   0 sosin      (501) staff       (20)      302 2023-05-15 08:02:38.000000 sosin-1.1.5/sosin/__init__.py
-drwxr-xr-x   0 sosin      (501) staff       (20)        0 2023-05-15 08:04:26.459341 sosin-1.1.5/sosin/databases/
--rwx------   0 sosin      (501) staff       (20)     4934 2023-04-24 10:38:48.000000 sosin-1.1.5/sosin/databases/fs.py
--rwx------   0 sosin      (501) staff       (20)     9763 2023-05-14 01:57:45.000000 sosin-1.1.5/sosin/databases/rdb.py
-drwxr-xr-x   0 sosin      (501) staff       (20)        0 2023-05-15 08:04:26.459745 sosin-1.1.5/sosin/rpa/
--rwx------   0 sosin      (501) staff       (20)    11055 2023-05-15 08:02:12.000000 sosin-1.1.5/sosin/rpa/email_mgr.py
--rwx------   0 sosin      (501) staff       (20)     3698 2023-05-10 06:56:55.000000 sosin-1.1.5/sosin/rpa/sms_mgr.py
-drwxr-xr-x   0 sosin      (501) staff       (20)        0 2023-05-15 08:04:26.460739 sosin-1.1.5/sosin/utils/
--rwx------   0 sosin      (501) staff       (20)     1797 2023-05-14 01:57:45.000000 sosin-1.1.5/sosin/utils/currency.py
--rwx------   0 sosin      (501) staff       (20)      304 2023-04-17 11:46:46.000000 sosin-1.1.5/sosin/utils/log.py
--rwx------   0 sosin      (501) staff       (20)      527 2023-04-17 11:46:46.000000 sosin-1.1.5/sosin/utils/progress.py
--rwx------   0 sosin      (501) staff       (20)      385 2023-04-17 11:46:46.000000 sosin-1.1.5/sosin/utils/secret.py
--rwx------   0 sosin      (501) staff       (20)      885 2023-05-10 06:56:55.000000 sosin-1.1.5/sosin/utils/zip.py
-drwxr-xr-x   0 sosin      (501) staff       (20)        0 2023-05-15 08:04:26.462799 sosin-1.1.5/sosin/web/
--rwx------   0 sosin      (501) staff       (20)     1055 2023-04-18 14:49:45.000000 sosin-1.1.5/sosin/web/content.py
--rwx------   0 sosin      (501) staff       (20)     5506 2023-05-14 01:57:26.000000 sosin-1.1.5/sosin/web/session.py
--rwx------   0 sosin      (501) staff       (20)     1051 2023-05-14 01:57:45.000000 sosin-1.1.5/sosin/web/translate.py
--rwx------   0 sosin      (501) staff       (20)     4394 2023-05-14 01:57:45.000000 sosin-1.1.5/sosin/web/virtual.py
-drwxr-xr-x   0 sosin      (501) staff       (20)        0 2023-05-15 08:04:26.459011 sosin-1.1.5/sosin.egg-info/
--rw-r--r--   0 sosin      (501) staff       (20)     1250 2023-05-15 08:04:26.000000 sosin-1.1.5/sosin.egg-info/PKG-INFO
--rw-r--r--   0 sosin      (501) staff       (20)      471 2023-05-15 08:04:26.000000 sosin-1.1.5/sosin.egg-info/SOURCES.txt
--rw-r--r--   0 sosin      (501) staff       (20)        1 2023-05-15 08:04:26.000000 sosin-1.1.5/sosin.egg-info/dependency_links.txt
--rw-r--r--   0 sosin      (501) staff       (20)       27 2023-05-15 08:04:26.000000 sosin-1.1.5/sosin.egg-info/requires.txt
--rw-r--r--   0 sosin      (501) staff       (20)        6 2023-05-15 08:04:26.000000 sosin-1.1.5/sosin.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-05-21 13:59:45.245981 sosin-1.1.6/
+-rw-rw-rw-   0        0        0     1083 2023-04-17 11:46:46.000000 sosin-1.1.6/LICENSE
+-rw-rw-rw-   0        0        0     1268 2023-05-21 13:59:45.244981 sosin-1.1.6/PKG-INFO
+-rw-rw-rw-   0        0        0      863 2023-04-17 11:46:46.000000 sosin-1.1.6/README.md
+-rw-rw-rw-   0        0        0       42 2023-05-21 13:59:45.245981 sosin-1.1.6/setup.cfg
+-rw-rw-rw-   0        0        0      984 2023-05-21 13:58:42.000000 sosin-1.1.6/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-21 13:59:45.191923 sosin-1.1.6/sosin/
+-rw-rw-rw-   0        0        0      302 2023-05-21 13:58:51.000000 sosin-1.1.6/sosin/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-21 13:59:45.229620 sosin-1.1.6/sosin/databases/
+-rw-rw-rw-   0        0        0     4934 2023-04-24 10:38:48.000000 sosin-1.1.6/sosin/databases/fs.py
+-rw-rw-rw-   0        0        0    13108 2023-05-21 13:58:00.000000 sosin-1.1.6/sosin/databases/rdb.py
+drwxrwxrwx   0        0        0        0 2023-05-21 13:59:45.232622 sosin-1.1.6/sosin/rpa/
+-rw-rw-rw-   0        0        0    11055 2023-05-15 08:13:19.000000 sosin-1.1.6/sosin/rpa/email_mgr.py
+-rw-rw-rw-   0        0        0     3698 2023-05-10 06:56:55.000000 sosin-1.1.6/sosin/rpa/sms_mgr.py
+drwxrwxrwx   0        0        0        0 2023-05-21 13:59:45.238621 sosin-1.1.6/sosin/utils/
+-rw-rw-rw-   0        0        0     1797 2023-05-14 01:57:45.000000 sosin-1.1.6/sosin/utils/currency.py
+-rw-rw-rw-   0        0        0      304 2023-04-17 11:46:46.000000 sosin-1.1.6/sosin/utils/log.py
+-rw-rw-rw-   0        0        0      527 2023-04-17 11:46:46.000000 sosin-1.1.6/sosin/utils/progress.py
+-rw-rw-rw-   0        0        0      385 2023-04-17 11:46:46.000000 sosin-1.1.6/sosin/utils/secret.py
+-rw-rw-rw-   0        0        0      885 2023-05-10 06:56:55.000000 sosin-1.1.6/sosin/utils/zip.py
+drwxrwxrwx   0        0        0        0 2023-05-21 13:59:45.243974 sosin-1.1.6/sosin/web/
+-rw-rw-rw-   0        0        0     1055 2023-04-18 14:49:45.000000 sosin-1.1.6/sosin/web/content.py
+-rw-rw-rw-   0        0        0     5506 2023-05-14 01:57:26.000000 sosin-1.1.6/sosin/web/session.py
+-rw-rw-rw-   0        0        0     1051 2023-05-14 01:57:45.000000 sosin-1.1.6/sosin/web/translate.py
+-rw-rw-rw-   0        0        0     4394 2023-05-14 01:57:45.000000 sosin-1.1.6/sosin/web/virtual.py
+drwxrwxrwx   0        0        0        0 2023-05-21 13:59:45.214621 sosin-1.1.6/sosin.egg-info/
+-rw-rw-rw-   0        0        0     1268 2023-05-21 13:59:44.000000 sosin-1.1.6/sosin.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      471 2023-05-21 13:59:45.000000 sosin-1.1.6/sosin.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-21 13:59:44.000000 sosin-1.1.6/sosin.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       27 2023-05-21 13:59:44.000000 sosin-1.1.6/sosin.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        6 2023-05-21 13:59:44.000000 sosin-1.1.6/sosin.egg-info/top_level.txt
```

### Comparing `sosin-1.1.5/LICENSE` & `sosin-1.1.6/LICENSE`

 * *Files identical despite different names*

### Comparing `sosin-1.1.5/PKG-INFO` & `sosin-1.1.6/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,41 +1,38 @@
-Metadata-Version: 2.1
-Name: sosin
-Version: 1.1.5
-Summary: Python utils for general works
-Home-page: https://github.com/devsosin/sosin
-Author: Jason Choi
-Author-email: svstar94@gmail.com
-License: MIT
-Platform: UNKNOWN
-Classifier: Programming Language :: Python :: 3
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Operating System :: OS Independent
-Requires-Python: >=3.9
-License-File: LICENSE
-
-# sosin: easy to use Python utils for general works
-
-[![PyPI Latest Release](https://img.shields.io/pypi/v/sosin.svg)](https://pypi.org/project/sosin/)
-[![License](https://img.shields.io/pypi/l/sosin.svg)](https://github.com/devsosin/sosin/blob/main/LICENSE)
-[![Downloads](https://static.pepy.tech/personalized-badge/sosin?period=month&units=international_system&left_color=black&right_color=orange&left_text=PyPI%20downloads%20per%20month)](https://pepy.tech/project/sosin)
-
-----
-
-## Dependencies
-![Python](https://img.shields.io/badge/python->=3.9-blue)
-![MariaDB](https://img.shields.io/badge/MariaDB->=10.3-yellow)
-![Chrome](https://img.shields.io/badge/Chrome--red)
-
-## Installation
-```bash
-# PyPI
-pip install sosin
-```
-
-## License
-[MIT](LICENSE)
-
-## Getting Help
-For usage questions, Please contact [me](https://github.com/devsosin)
-
-
+Metadata-Version: 2.1
+Name: sosin
+Version: 1.1.6
+Summary: Python utils for general works
+Home-page: https://github.com/devsosin/sosin
+Author: Jason Choi
+Author-email: svstar94@gmail.com
+License: MIT
+Classifier: Programming Language :: Python :: 3
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Operating System :: OS Independent
+Requires-Python: >=3.9
+License-File: LICENSE
+
+# sosin: easy to use Python utils for general works
+
+[![PyPI Latest Release](https://img.shields.io/pypi/v/sosin.svg)](https://pypi.org/project/sosin/)
+[![License](https://img.shields.io/pypi/l/sosin.svg)](https://github.com/devsosin/sosin/blob/main/LICENSE)
+[![Downloads](https://static.pepy.tech/personalized-badge/sosin?period=month&units=international_system&left_color=black&right_color=orange&left_text=PyPI%20downloads%20per%20month)](https://pepy.tech/project/sosin)
+
+----
+
+## Dependencies
+![Python](https://img.shields.io/badge/python->=3.9-blue)
+![MariaDB](https://img.shields.io/badge/MariaDB->=10.3-yellow)
+![Chrome](https://img.shields.io/badge/Chrome--red)
+
+## Installation
+```bash
+# PyPI
+pip install sosin
+```
+
+## License
+[MIT](LICENSE)
+
+## Getting Help
+For usage questions, Please contact [me](https://github.com/devsosin)
```

### Comparing `sosin-1.1.5/README.md` & `sosin-1.1.6/README.md`

 * *Files identical despite different names*

### Comparing `sosin-1.1.5/setup.py` & `sosin-1.1.6/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import setuptools
 
 setuptools.setup(
     name                                = "sosin",
-    version                             = "1.1.5",
+    version                             = "1.1.6",
     license                             = 'MIT',
     author                              = "Jason Choi",
     author_email                        = "svstar94@gmail.com",
     description                         = "Python utils for general works",
     long_description                    = open('README.md').read(),
     url                                 = "https://github.com/devsosin/sosin",
     install_requires                    = ['requests', 'requests-toolbelt'],
```

### Comparing `sosin-1.1.5/sosin/databases/fs.py` & `sosin-1.1.6/sosin/databases/fs.py`

 * *Files identical despite different names*

### Comparing `sosin-1.1.5/sosin/rpa/email_mgr.py` & `sosin-1.1.6/sosin/rpa/email_mgr.py`

 * *Files identical despite different names*

### Comparing `sosin-1.1.5/sosin/rpa/sms_mgr.py` & `sosin-1.1.6/sosin/rpa/sms_mgr.py`

 * *Files identical despite different names*

### Comparing `sosin-1.1.5/sosin/utils/currency.py` & `sosin-1.1.6/sosin/utils/currency.py`

 * *Files identical despite different names*

### Comparing `sosin-1.1.5/sosin/utils/progress.py` & `sosin-1.1.6/sosin/utils/progress.py`

 * *Files identical despite different names*

### Comparing `sosin-1.1.5/sosin/utils/zip.py` & `sosin-1.1.6/sosin/utils/zip.py`

 * *Files identical despite different names*

### Comparing `sosin-1.1.5/sosin/web/content.py` & `sosin-1.1.6/sosin/web/content.py`

 * *Files identical despite different names*

### Comparing `sosin-1.1.5/sosin/web/session.py` & `sosin-1.1.6/sosin/web/session.py`

 * *Files identical despite different names*

### Comparing `sosin-1.1.5/sosin/web/translate.py` & `sosin-1.1.6/sosin/web/translate.py`

 * *Files identical despite different names*

### Comparing `sosin-1.1.5/sosin/web/virtual.py` & `sosin-1.1.6/sosin/web/virtual.py`

 * *Files identical despite different names*

### Comparing `sosin-1.1.5/sosin.egg-info/PKG-INFO` & `sosin-1.1.6/sosin.egg-info/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,41 +1,38 @@
-Metadata-Version: 2.1
-Name: sosin
-Version: 1.1.5
-Summary: Python utils for general works
-Home-page: https://github.com/devsosin/sosin
-Author: Jason Choi
-Author-email: svstar94@gmail.com
-License: MIT
-Platform: UNKNOWN
-Classifier: Programming Language :: Python :: 3
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Operating System :: OS Independent
-Requires-Python: >=3.9
-License-File: LICENSE
-
-# sosin: easy to use Python utils for general works
-
-[![PyPI Latest Release](https://img.shields.io/pypi/v/sosin.svg)](https://pypi.org/project/sosin/)
-[![License](https://img.shields.io/pypi/l/sosin.svg)](https://github.com/devsosin/sosin/blob/main/LICENSE)
-[![Downloads](https://static.pepy.tech/personalized-badge/sosin?period=month&units=international_system&left_color=black&right_color=orange&left_text=PyPI%20downloads%20per%20month)](https://pepy.tech/project/sosin)
-
-----
-
-## Dependencies
-![Python](https://img.shields.io/badge/python->=3.9-blue)
-![MariaDB](https://img.shields.io/badge/MariaDB->=10.3-yellow)
-![Chrome](https://img.shields.io/badge/Chrome--red)
-
-## Installation
-```bash
-# PyPI
-pip install sosin
-```
-
-## License
-[MIT](LICENSE)
-
-## Getting Help
-For usage questions, Please contact [me](https://github.com/devsosin)
-
-
+Metadata-Version: 2.1
+Name: sosin
+Version: 1.1.6
+Summary: Python utils for general works
+Home-page: https://github.com/devsosin/sosin
+Author: Jason Choi
+Author-email: svstar94@gmail.com
+License: MIT
+Classifier: Programming Language :: Python :: 3
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Operating System :: OS Independent
+Requires-Python: >=3.9
+License-File: LICENSE
+
+# sosin: easy to use Python utils for general works
+
+[![PyPI Latest Release](https://img.shields.io/pypi/v/sosin.svg)](https://pypi.org/project/sosin/)
+[![License](https://img.shields.io/pypi/l/sosin.svg)](https://github.com/devsosin/sosin/blob/main/LICENSE)
+[![Downloads](https://static.pepy.tech/personalized-badge/sosin?period=month&units=international_system&left_color=black&right_color=orange&left_text=PyPI%20downloads%20per%20month)](https://pepy.tech/project/sosin)
+
+----
+
+## Dependencies
+![Python](https://img.shields.io/badge/python->=3.9-blue)
+![MariaDB](https://img.shields.io/badge/MariaDB->=10.3-yellow)
+![Chrome](https://img.shields.io/badge/Chrome--red)
+
+## Installation
+```bash
+# PyPI
+pip install sosin
+```
+
+## License
+[MIT](LICENSE)
+
+## Getting Help
+For usage questions, Please contact [me](https://github.com/devsosin)
```

