# Comparing `tmp/pain001-0.0.8.tar.gz` & `tmp/pain001-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pain001-0.0.8.tar", last modified: Sat Mar 18 15:45:27 2023, max compression
+gzip compressed data, was "pain001-0.0.9.tar", last modified: Sun Mar 19 00:40:31 2023, max compression
```

## Comparing `pain001-0.0.8.tar` & `pain001-0.0.9.tar`

### file list

```diff
@@ -1,22 +1,34 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-18 15:45:27.194480 pain001-0.0.8/
--rw-r--r--   0 runner    (1001) docker     (123)    10870 2023-03-18 15:45:20.000000 pain001-0.0.8/LICENSE-APACHE
--rw-r--r--   0 runner    (1001) docker     (123)     1080 2023-03-18 15:45:20.000000 pain001-0.0.8/LICENSE-MIT
--rw-r--r--   0 runner    (1001) docker     (123)       42 2023-03-18 15:45:20.000000 pain001-0.0.8/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     1541 2023-03-18 15:45:27.194480 pain001-0.0.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4893 2023-03-18 15:45:20.000000 pain001-0.0.8/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-18 15:45:27.194480 pain001-0.0.8/pain001/
--rw-r--r--   0 runner    (1001) docker     (123)      661 2023-03-18 15:45:20.000000 pain001-0.0.8/pain001/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2578 2023-03-18 15:45:20.000000 pain001-0.0.8/pain001/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    12955 2023-03-18 15:45:20.000000 pain001-0.0.8/pain001/core.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-18 15:45:27.194480 pain001-0.0.8/pain001.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1541 2023-03-18 15:45:27.000000 pain001-0.0.8/pain001.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      373 2023-03-18 15:45:27.000000 pain001-0.0.8/pain001.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-18 15:45:27.000000 pain001-0.0.8/pain001.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       86 2023-03-18 15:45:27.000000 pain001-0.0.8/pain001.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-03-18 15:45:27.000000 pain001-0.0.8/pain001.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1208 2023-03-18 15:45:27.198480 pain001-0.0.8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2515 2023-03-18 15:45:20.000000 pain001-0.0.8/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-18 15:45:27.194480 pain001-0.0.8/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     1625 2023-03-18 15:45:20.000000 pain001-0.0.8/tests/test_create_xml_element.py
--rw-r--r--   0 runner    (1001) docker     (123)     3122 2023-03-18 15:45:20.000000 pain001-0.0.8/tests/test_validate_csv_data.py
--rw-r--r--   0 runner    (1001) docker     (123)     1685 2023-03-18 15:45:20.000000 pain001-0.0.8/tests/test_validate_via_xsd.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-19 00:40:31.959917 pain001-0.0.9/
+-rw-r--r--   0 runner    (1001) docker     (123)    10870 2023-03-19 00:40:26.000000 pain001-0.0.9/LICENSE-APACHE
+-rw-r--r--   0 runner    (1001) docker     (123)     1080 2023-03-19 00:40:26.000000 pain001-0.0.9/LICENSE-MIT
+-rw-r--r--   0 runner    (1001) docker     (123)       42 2023-03-19 00:40:26.000000 pain001-0.0.9/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     1448 2023-03-19 00:40:31.959917 pain001-0.0.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4893 2023-03-19 00:40:26.000000 pain001-0.0.9/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-19 00:40:31.959917 pain001-0.0.9/pain001/
+-rw-r--r--   0 runner    (1001) docker     (123)      663 2023-03-19 00:40:26.000000 pain001-0.0.9/pain001/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2754 2023-03-19 00:40:26.000000 pain001-0.0.9/pain001/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2716 2023-03-19 00:40:26.000000 pain001-0.0.9/pain001/core.py
+-rw-r--r--   0 runner    (1001) docker     (123)      591 2023-03-19 00:40:26.000000 pain001-0.0.9/pain001/create_root_element.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1009 2023-03-19 00:40:26.000000 pain001-0.0.9/pain001/create_xml_element.py
+-rw-r--r--   0 runner    (1001) docker     (123)      216 2023-03-19 00:40:26.000000 pain001-0.0.9/pain001/generate_updated_xml_file_path.py
+-rw-r--r--   0 runner    (1001) docker     (123)      457 2023-03-19 00:40:26.000000 pain001-0.0.9/pain001/load_csv_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)      439 2023-03-19 00:40:26.000000 pain001-0.0.9/pain001/register_namespaces.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3030 2023-03-19 00:40:26.000000 pain001-0.0.9/pain001/validate_csv_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)      515 2023-03-19 00:40:26.000000 pain001-0.0.9/pain001/validate_via_xsd.py
+-rw-r--r--   0 runner    (1001) docker     (123)      452 2023-03-19 00:40:26.000000 pain001-0.0.9/pain001/write_xml_to_file.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7690 2023-03-19 00:40:26.000000 pain001-0.0.9/pain001/xml_generator.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-19 00:40:31.959917 pain001-0.0.9/pain001.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1448 2023-03-19 00:40:31.000000 pain001-0.0.9/pain001.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      750 2023-03-19 00:40:31.000000 pain001-0.0.9/pain001.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-19 00:40:31.000000 pain001-0.0.9/pain001.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       86 2023-03-19 00:40:31.000000 pain001-0.0.9/pain001.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-03-19 00:40:31.000000 pain001-0.0.9/pain001.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1208 2023-03-19 00:40:31.959917 pain001-0.0.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2508 2023-03-19 00:40:26.000000 pain001-0.0.9/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-19 00:40:31.959917 pain001-0.0.9/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      820 2023-03-19 00:40:26.000000 pain001-0.0.9/tests/test_create_root_element.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1687 2023-03-19 00:40:26.000000 pain001-0.0.9/tests/test_create_xml_element.py
+-rw-r--r--   0 runner    (1001) docker     (123)      438 2023-03-19 00:40:26.000000 pain001-0.0.9/tests/test_generate_updated_xml_file_path.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1031 2023-03-19 00:40:26.000000 pain001-0.0.9/tests/test_load_csv_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4570 2023-03-19 00:40:26.000000 pain001-0.0.9/tests/test_validate_csv_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1877 2023-03-19 00:40:26.000000 pain001-0.0.9/tests/test_validate_via_xsd.py
```

### Comparing `pain001-0.0.8/LICENSE-APACHE` & `pain001-0.0.9/LICENSE-APACHE`

 * *Files identical despite different names*

### Comparing `pain001-0.0.8/LICENSE-MIT` & `pain001-0.0.9/LICENSE-MIT`

 * *Files identical despite different names*

### Comparing `pain001-0.0.8/PKG-INFO` & `pain001-0.0.9/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 Metadata-Version: 2.1
 Name: pain001
-Version: 0.0.8
-Summary: pain001 is a Python library for generating Customer-to-Bank Credit Transfer payloads in the ISO 20022 Standard's Pain.001.001.03 format from CSV files.
+Version: 0.0.9
+Summary: pain001 is a Python library that makes it easy to automate the creation
 Home-page: https://github.com/sebastienrousseau/Pain001
 Author: Sebastien Rousseau
 Author-email: sebastian.rousseau@gmail.com
 License: Apache Software License
-Keywords: command line interface cli python pain001 interactive bash tool
+Keywords: command line interface cli csv python pain001 sepa
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
```

### Comparing `pain001-0.0.8/README.md` & `pain001-0.0.9/README.md`

 * *Files identical despite different names*

### Comparing `pain001-0.0.8/pain001/__init__.py` & `pain001-0.0.9/pain001/__init__.py`

 * *Files 5% similar despite different names*

```diff
@@ -4,14 +4,15 @@
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 # http://www.apache.org/licenses/LICENSE-2.0
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
-# WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
+# WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or
+# implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 """The Python pain001 module."""
-__all__ = ['pain001']
-__version__ = '0.0.8'
+__all__ = ["pain001"]
+__version__ = "0.0.9"
```

### Comparing `pain001-0.0.8/pain001/__main__.py` & `pain001-0.0.9/pain001/__main__.py`

 * *Files 13% similar despite different names*

```diff
@@ -4,70 +4,87 @@
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 # http://www.apache.org/licenses/LICENSE-2.0
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
-# WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
+# WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or
+# implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 # pylint: disable=invalid-name
-"""Enables use of Python Pain001 as a "main" function (i.e. "python -m pain001").
+"""
+Enables use of Python Pain001 as a "main" function (i.e.
+"python3 -m pain001 <xml_file_path> <xsd_file_path> <csv_file_path>").
 
-This allows using Pain001 with third-party libraries without modifying their code.
+This allows using Pain001 with third-party libraries without modifying
+their code.
 """
 
 from . import core
 
 import os
 import sys
 import argparse
 
 cli_string = """
 
-usage: python3 -m pain001 <xml_file_path> <xsd_file_path> <csv_file_path>
+usage:
+python3 -m pain001 <xml_file_path> <xsd_file_path> <csv_file_path>
 
 Python Pain001 is a Python package that generates a Customer-to-Bank
 Credit Transfer payload in the pain.001.001.03 format from a CSV file.
 The package is named after the standard file format for SEPA and
 non-SEPA Credit Transfer, which is the Pain (payment initiation)
 format 001.001.03. The Pain001 library provides a convenient way for
 developers to create payment files in this format and to validate
 the generated files against the XSD schema.
 
 Usage:
 python3 -m pain001 <xml_file_path> <xsd_file_path> <csv_file_path>
 
 The first argument is the path of the XML template file. The second
-argument is the path of the XSD template file. The third argument is the
-path of the CSV file containing the payment data."""
+argument is the path of the XSD template file. The third argument is
+the path of the CSV file containing the payment data."""
 
 
 def main():
-    """Entrypoint for pain001 when invoked as a module with python -m pain001."""
+    """
+    Entrypoint for pain001 when invoked as a module with
+    python3 -m pain001 <xml_file_path> <xsd_file_path> <csv_file_path>.
+    """
 
     parser = argparse.ArgumentParser(
-        description='Generate Pain.001 file from CSV data')
-    parser.add_argument('xml_file_path', help='Path to XML template file')
-    parser.add_argument('xsd_file_path', help='Path to XSD template file')
-    parser.add_argument('csv_file_path', help='Path to CSV data file')
+        description="Generate Pain.001 file from CSV data"
+    )
+    parser.add_argument(
+        "xml_file_path", help="Path to XML template file"
+    )
+    parser.add_argument(
+        "xsd_file_path", help="Path to XSD template file"
+    )
+    parser.add_argument(
+        "csv_file_path", help="Path to CSV data file"
+    )
     args = parser.parse_args()
 
     if not os.path.isfile(args.xml_file_path):
-        print('The XML template file does not exist.')
+        print("The XML template file does not exist.")
         sys.exit(1)
 
     if not os.path.isfile(args.xsd_file_path):
-        print('The XSD template file does not exist.')
+        print("The XSD template file does not exist.")
         sys.exit(1)
 
     if not os.path.isfile(args.csv_file_path):
-        print('The CSV file does not exist.')
+        print("The CSV file does not exist.")
         sys.exit(1)
 
-    core.main(args.xml_file_path, args.xsd_file_path, args.csv_file_path)
+    core.main(
+        args.xml_file_path, args.xsd_file_path, args.csv_file_path
+    )
 
 
-if __name__ == '__main__':
+if __name__ == "__main__":
     main()
```

### Comparing `pain001-0.0.8/pain001.egg-info/PKG-INFO` & `pain001-0.0.9/pain001.egg-info/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 Metadata-Version: 2.1
 Name: pain001
-Version: 0.0.8
-Summary: pain001 is a Python library for generating Customer-to-Bank Credit Transfer payloads in the ISO 20022 Standard's Pain.001.001.03 format from CSV files.
+Version: 0.0.9
+Summary: pain001 is a Python library that makes it easy to automate the creation
 Home-page: https://github.com/sebastienrousseau/Pain001
 Author: Sebastien Rousseau
 Author-email: sebastian.rousseau@gmail.com
 License: Apache Software License
-Keywords: command line interface cli python pain001 interactive bash tool
+Keywords: command line interface cli csv python pain001 sepa
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
```

### Comparing `pain001-0.0.8/setup.cfg` & `pain001-0.0.9/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = pain001
-version = 0.0.8
+version = 0.0.9
 author = Sebastian Rousseau
 author_email = sebastian.rousseau@gmail.com
 description = Pain001 is a Python library for generating Customer-to-Bank Credit Transfer payloads in the ISO 20022 Standard''s Pain.001.001.03 format from CSV files.
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://github.com/sebastienrousseau/Pain001
 license = Apache Software License
```

### Comparing `pain001-0.0.8/setup.py` & `pain001-0.0.9/setup.py`

 * *Files 18% similar despite different names*

```diff
@@ -4,15 +4,17 @@
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 # http://www.apache.org/licenses/LICENSE-2.0
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
-# WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
+# WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or
+# implied.
+#
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 """The setup.py file for Python pain001."""
 
 from setuptools import setup
 
@@ -25,26 +27,29 @@
 The package is named after the standard file format for SEPA and non-
 SEPA Credit Transfer, which is the Pain (payment initiation) format
 001.001.03. The pain001 library provides a convenient way for developers
 to create payment files in this format.
 """.strip()
 
 SHORT_DESCRIPTION = """
-pain001 is a Python library for generating Customer-to-Bank Credit Transfer payloads in the ISO 20022 Standard's Pain.001.001.03 format from CSV files.""".strip()
+pain001 is a Python library that makes it easy to automate the creation
+of ISO 20022 compliant payment files (XML PAIN.001.03) directly from a
+CSV file.
+""".strip()
 
 DEPENDENCIES = [
     'python-dateutil>=2.8.2',
     'xmlschema>=1.8.0',
 ]
 
 TEST_DEPENDENCIES = [
     'xmlschema>=1.8.0',
 ]
 
-VERSION = '0.0.8'
+VERSION = '0.0.9'
 URL = 'https://github.com/sebastienrousseau/Pain001'
 
 setup(
     name='pain001',
     version=VERSION,
     description=SHORT_DESCRIPTION,
     long_description=LONG_DESCRIPTION,
@@ -70,15 +75,15 @@
 
         'Operating System :: OS Independent',
         'Operating System :: POSIX',
         'Operating System :: MacOS',
         'Operating System :: Unix',
     ],
 
-    keywords='command line interface cli python pain001 interactive bash tool',
+    keywords='command line interface cli csv python pain001 sepa',
 
     packages=['pain001'],
 
 
     install_requires=DEPENDENCIES,
     tests_require=TEST_DEPENDENCIES,
 )
```

### Comparing `pain001-0.0.8/tests/test_create_xml_element.py` & `pain001-0.0.9/tests/test_create_xml_element.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,12 @@
 import unittest
 import xml.etree.ElementTree as ET
-from pain001.core import create_xml_element
+from pain001.create_xml_element import create_xml_element
+
+# Test if the XML element is created correctly
 
 
 class TestCreateXmlElement(unittest.TestCase):
 
     def test_create_element_with_tag_only(self):
         root = ET.Element('root')
         elem = create_xml_element(root, 'test')
```

### Comparing `pain001-0.0.8/tests/test_validate_via_xsd.py` & `pain001-0.0.9/tests/test_validate_via_xsd.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,11 +1,12 @@
-from pain001.core import validate_via_xsd
 import unittest
 import os
-import xml.etree.ElementTree as ET
+from pain001.validate_via_xsd import validate_via_xsd
+
+# Test if the XML file is validated correctly against the XSD schema
 
 
 class TestValidateViaXsd(unittest.TestCase):
 
     def setUp(self):
         self.valid_xml_file = 'valid_test.xml'
         self.invalid_xml_file = 'invalid_test.xml'
@@ -15,33 +16,43 @@
         with open(self.valid_xml_file, 'w') as f:
             f.write('''<root>
                             <element>Valid data</element>
                         </root>''')
 
         # Create invalid XML test file
         with open(self.invalid_xml_file, 'w') as f:
-            f.write('''<root>
-                            <invalidElement>Invalid data</invalidElement>
-                        </root>''')
+            f.write('''
+            <root>
+                <invalidElement>Invalid data</invalidElement>
+            </root>
+            ''')
 
         # Create test XSD schema file
         with open(self.xsd_file, 'w') as f:
-            f.write('''<xs:schema xmlns:xs="http://www.w3.org/2001/XMLSchema">
-                            <xs:element name="root">
-                                <xs:complexType>
-                                    <xs:sequence>
-                                        <xs:element name="element" type="xs:string" />
-                                    </xs:sequence>
-                                </xs:complexType>
+            f.write('''
+            <xs:schema xmlns:xs="http://www.w3.org/2001/XMLSchema">
+                <xs:element name="root">
+                    <xs:complexType>
+                        <xs:sequence>
+                            <xs:element name="element">
+                                <xs:simpleType>
+                                    <xs:restriction base="xs:string"/>
+                                </xs:simpleType>
                             </xs:element>
-                        </xs:schema>''')
+                        </xs:sequence>
+                    </xs:complexType>
+                </xs:element>
+            </xs:schema>
+            ''')
 
     def tearDown(self):
         os.remove(self.valid_xml_file)
         os.remove(self.invalid_xml_file)
         os.remove(self.xsd_file)
 
     def test_valid_xml(self):
         assert validate_via_xsd(self.valid_xml_file, self.xsd_file)
 
     def test_invalid_xml(self):
-        assert not validate_via_xsd(self.invalid_xml_file, self.xsd_file)
+        assert not validate_via_xsd(
+            self.invalid_xml_file, self.xsd_file
+        )
```

