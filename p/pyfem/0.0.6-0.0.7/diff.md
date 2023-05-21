# Comparing `tmp/pyfem-0.0.6.tar.gz` & `tmp/pyfem-0.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyfem-0.0.6.tar", last modified: Fri May 12 06:44:37 2023, max compression
+gzip compressed data, was "pyfem-0.0.7.tar", last modified: Sun May 21 14:43:31 2023, max compression
```

## Comparing `pyfem-0.0.6.tar` & `pyfem-0.0.7.tar`

### file list

```diff
@@ -1,52 +1,67 @@
-drwxrwxrwx   0        0        0        0 2023-05-12 06:44:37.328904 pyfem-0.0.6/
--rw-rw-rw-   0        0        0    11525 2023-05-04 02:49:52.000000 pyfem-0.0.6/LICENSE
--rw-rw-rw-   0        0        0      791 2023-05-12 06:44:37.328904 pyfem-0.0.6/PKG-INFO
--rw-rw-rw-   0        0        0      266 2023-05-04 08:32:11.000000 pyfem-0.0.6/README.md
--rw-rw-rw-   0        0        0       42 2023-05-12 06:44:37.329904 pyfem-0.0.6/setup.cfg
--rw-rw-rw-   0        0        0      941 2023-05-12 06:43:54.000000 pyfem-0.0.6/setup.py
-drwxrwxrwx   0        0        0        0 2023-05-12 06:44:37.289904 pyfem-0.0.6/src/
-drwxrwxrwx   0        0        0        0 2023-05-12 06:44:37.297913 pyfem-0.0.6/src/pyfem/
--rw-rw-rw-   0        0        0        0 2023-05-04 02:49:52.000000 pyfem-0.0.6/src/pyfem/__init__.py
--rw-rw-rw-   0        0        0      492 2023-05-08 04:08:44.000000 pyfem-0.0.6/src/pyfem/__main__.py
-drwxrwxrwx   0        0        0        0 2023-05-12 06:44:37.303913 pyfem-0.0.6/src/pyfem/assembly/
--rw-rw-rw-   0        0        0        0 2023-05-04 02:49:52.000000 pyfem-0.0.6/src/pyfem/assembly/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-12 06:44:37.306904 pyfem-0.0.6/src/pyfem/elements/
--rw-rw-rw-   0        0        0     1958 2023-05-12 06:17:04.000000 pyfem-0.0.6/src/pyfem/elements/BaseElement.py
--rw-rw-rw-   0        0        0     1793 2023-05-12 01:45:39.000000 pyfem-0.0.6/src/pyfem/elements/IsoElementDiagram.py
--rw-rw-rw-   0        0        0    19159 2023-05-12 05:44:36.000000 pyfem-0.0.6/src/pyfem/elements/IsoElementShape.py
--rw-rw-rw-   0        0        0        0 2023-05-04 02:49:52.000000 pyfem-0.0.6/src/pyfem/elements/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-12 06:44:37.309904 pyfem-0.0.6/src/pyfem/fem/
--rw-rw-rw-   0        0        0     2846 2023-05-10 03:32:54.000000 pyfem-0.0.6/src/pyfem/fem/ElementSet.py
--rw-rw-rw-   0        0        0     3373 2023-05-12 06:40:50.000000 pyfem-0.0.6/src/pyfem/fem/NodeSet.py
--rw-rw-rw-   0        0        0        0 2023-05-04 02:49:52.000000 pyfem-0.0.6/src/pyfem/fem/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-12 06:44:37.318904 pyfem-0.0.6/src/pyfem/io/
--rw-rw-rw-   0        0        0      569 2023-05-11 04:23:28.000000 pyfem-0.0.6/src/pyfem/io/BC.py
--rw-rw-rw-   0        0        0      528 2023-05-11 04:23:28.000000 pyfem-0.0.6/src/pyfem/io/Dofs.py
--rw-rw-rw-   0        0        0      548 2023-05-11 04:23:28.000000 pyfem-0.0.6/src/pyfem/io/Material.py
--rw-rw-rw-   0        0        0      498 2023-05-11 04:23:28.000000 pyfem-0.0.6/src/pyfem/io/Mesh.py
--rw-rw-rw-   0        0        0      515 2023-05-11 04:23:28.000000 pyfem-0.0.6/src/pyfem/io/Output.py
--rw-rw-rw-   0        0        0     8646 2023-05-12 06:21:10.000000 pyfem-0.0.6/src/pyfem/io/Properties.py
--rw-rw-rw-   0        0        0      589 2023-05-12 03:51:11.000000 pyfem-0.0.6/src/pyfem/io/Section.py
--rw-rw-rw-   0        0        0      484 2023-05-11 04:23:28.000000 pyfem-0.0.6/src/pyfem/io/Solver.py
--rw-rw-rw-   0        0        0        0 2023-05-04 02:49:52.000000 pyfem-0.0.6/src/pyfem/io/__init__.py
--rw-rw-rw-   0        0        0     1334 2023-05-10 03:32:54.000000 pyfem-0.0.6/src/pyfem/io/arguments.py
-drwxrwxrwx   0        0        0        0 2023-05-12 06:44:37.321904 pyfem-0.0.6/src/pyfem/materials/
--rw-rw-rw-   0        0        0     1118 2023-05-11 04:23:28.000000 pyfem-0.0.6/src/pyfem/materials/BaseMaterial.py
--rw-rw-rw-   0        0        0     3785 2023-05-04 08:54:43.000000 pyfem-0.0.6/src/pyfem/materials/MaterialManager.py
--rw-rw-rw-   0        0        0        0 2023-05-04 02:49:52.000000 pyfem-0.0.6/src/pyfem/materials/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-12 06:44:37.322912 pyfem-0.0.6/src/pyfem/mesh/
--rw-rw-rw-   0        0        0        0 2023-05-04 02:49:52.000000 pyfem-0.0.6/src/pyfem/mesh/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-12 06:44:37.322912 pyfem-0.0.6/src/pyfem/solvers/
--rw-rw-rw-   0        0        0        0 2023-05-04 02:49:52.000000 pyfem-0.0.6/src/pyfem/solvers/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-12 06:44:37.327912 pyfem-0.0.6/src/pyfem/utils/
--rw-rw-rw-   0        0        0     2259 2023-05-12 06:39:24.000000 pyfem-0.0.6/src/pyfem/utils/IntKeyDict.py
--rw-rw-rw-   0        0        0        0 2023-05-04 02:49:52.000000 pyfem-0.0.6/src/pyfem/utils/__init__.py
--rw-rw-rw-   0        0        0      540 2023-05-11 04:23:28.000000 pyfem-0.0.6/src/pyfem/utils/colors.py
--rw-rw-rw-   0        0        0     1516 2023-05-08 04:08:44.000000 pyfem-0.0.6/src/pyfem/utils/logger.py
--rw-rw-rw-   0        0        0     5352 2023-05-11 06:46:50.000000 pyfem-0.0.6/src/pyfem/utils/shape_functions.py
-drwxrwxrwx   0        0        0        0 2023-05-12 06:44:37.302905 pyfem-0.0.6/src/pyfem.egg-info/
--rw-rw-rw-   0        0        0      791 2023-05-12 06:44:37.000000 pyfem-0.0.6/src/pyfem.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1034 2023-05-12 06:44:37.000000 pyfem-0.0.6/src/pyfem.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-12 06:44:37.000000 pyfem-0.0.6/src/pyfem.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       46 2023-05-12 06:44:37.000000 pyfem-0.0.6/src/pyfem.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0        6 2023-05-12 06:44:37.000000 pyfem-0.0.6/src/pyfem.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-05-21 14:43:31.562430 pyfem-0.0.7/
+-rw-rw-rw-   0        0        0    11524 2023-05-03 09:58:16.000000 pyfem-0.0.7/LICENSE
+-rw-rw-rw-   0        0        0      793 2023-05-21 14:43:31.561438 pyfem-0.0.7/PKG-INFO
+-rw-rw-rw-   0        0        0      270 2023-05-19 11:01:17.000000 pyfem-0.0.7/README.md
+-rw-rw-rw-   0        0        0       42 2023-05-21 14:43:31.562430 pyfem-0.0.7/setup.cfg
+-rw-rw-rw-   0        0        0      941 2023-05-21 14:39:32.000000 pyfem-0.0.7/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-21 14:43:31.466622 pyfem-0.0.7/src/
+drwxrwxrwx   0        0        0        0 2023-05-21 14:43:31.479603 pyfem-0.0.7/src/pyfem/
+-rw-rw-rw-   0        0        0        0 2023-04-13 12:04:13.000000 pyfem-0.0.7/src/pyfem/__init__.py
+-rw-rw-rw-   0        0        0      927 2023-05-21 14:38:58.000000 pyfem-0.0.7/src/pyfem/__main__.py
+drwxrwxrwx   0        0        0        0 2023-05-21 14:43:31.491554 pyfem-0.0.7/src/pyfem/assembly/
+-rw-rw-rw-   0        0        0     8732 2023-05-20 17:12:32.000000 pyfem-0.0.7/src/pyfem/assembly/Assembly.py
+-rw-rw-rw-   0        0        0        0 2023-04-13 12:04:13.000000 pyfem-0.0.7/src/pyfem/assembly/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-21 14:43:31.498903 pyfem-0.0.7/src/pyfem/bc/
+-rw-rw-rw-   0        0        0      781 2023-05-19 11:01:17.000000 pyfem-0.0.7/src/pyfem/bc/BaseBC.py
+-rw-rw-rw-   0        0        0     2262 2023-05-19 14:23:03.000000 pyfem-0.0.7/src/pyfem/bc/DirichletBC.py
+-rw-rw-rw-   0        0        0        0 2023-05-19 11:01:17.000000 pyfem-0.0.7/src/pyfem/bc/__init__.py
+-rw-rw-rw-   0        0        0      876 2023-05-19 11:01:17.000000 pyfem-0.0.7/src/pyfem/bc/get_bc_data.py
+drwxrwxrwx   0        0        0        0 2023-05-21 14:43:31.510827 pyfem-0.0.7/src/pyfem/elements/
+-rw-rw-rw-   0        0        0     4293 2023-05-20 15:49:28.000000 pyfem-0.0.7/src/pyfem/elements/BaseElement.py
+-rw-rw-rw-   0        0        0     1793 2023-05-18 15:11:46.000000 pyfem-0.0.7/src/pyfem/elements/IsoElementDiagram.py
+-rw-rw-rw-   0        0        0    19983 2023-05-19 11:01:17.000000 pyfem-0.0.7/src/pyfem/elements/IsoElementShape.py
+-rw-rw-rw-   0        0        0     4367 2023-05-20 16:49:40.000000 pyfem-0.0.7/src/pyfem/elements/SolidPlaneSmallStrain.py
+-rw-rw-rw-   0        0        0        0 2023-04-13 12:04:13.000000 pyfem-0.0.7/src/pyfem/elements/__init__.py
+-rw-rw-rw-   0        0        0     1894 2023-05-18 11:01:59.000000 pyfem-0.0.7/src/pyfem/elements/get_element_data.py
+-rw-rw-rw-   0        0        0     1793 2023-05-17 14:10:35.000000 pyfem-0.0.7/src/pyfem/elements/get_iso_element_type.py
+drwxrwxrwx   0        0        0        0 2023-05-21 14:43:31.512315 pyfem-0.0.7/src/pyfem/fem/
+-rw-rw-rw-   0        0        0        0 2023-04-13 12:04:13.000000 pyfem-0.0.7/src/pyfem/fem/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-21 14:43:31.531134 pyfem-0.0.7/src/pyfem/io/
+-rw-rw-rw-   0        0        0      679 2023-05-19 11:01:17.000000 pyfem-0.0.7/src/pyfem/io/BC.py
+-rw-rw-rw-   0        0        0      577 2023-05-18 14:20:30.000000 pyfem-0.0.7/src/pyfem/io/Dof.py
+-rw-rw-rw-   0        0        0     2299 2023-05-18 15:11:46.000000 pyfem-0.0.7/src/pyfem/io/Material.py
+-rw-rw-rw-   0        0        0      520 2023-05-18 14:20:30.000000 pyfem-0.0.7/src/pyfem/io/Mesh.py
+-rw-rw-rw-   0        0        0      575 2023-05-20 17:12:32.000000 pyfem-0.0.7/src/pyfem/io/Output.py
+-rw-rw-rw-   0        0        0    10304 2023-05-21 14:35:56.000000 pyfem-0.0.7/src/pyfem/io/Properties.py
+-rw-rw-rw-   0        0        0      815 2023-05-18 14:20:30.000000 pyfem-0.0.7/src/pyfem/io/Section.py
+-rw-rw-rw-   0        0        0      466 2023-05-18 14:20:30.000000 pyfem-0.0.7/src/pyfem/io/Solver.py
+-rw-rw-rw-   0        0        0        0 2023-04-19 14:26:23.000000 pyfem-0.0.7/src/pyfem/io/__init__.py
+-rw-rw-rw-   0        0        0     1704 2023-05-21 14:40:55.000000 pyfem-0.0.7/src/pyfem/io/arguments.py
+-rw-rw-rw-   0        0        0     3657 2023-05-21 14:31:44.000000 pyfem-0.0.7/src/pyfem/io/write_vtk.py
+drwxrwxrwx   0        0        0        0 2023-05-21 14:43:31.538161 pyfem-0.0.7/src/pyfem/materials/
+-rw-rw-rw-   0        0        0      840 2023-05-18 15:34:49.000000 pyfem-0.0.7/src/pyfem/materials/BaseMaterial.py
+-rw-rw-rw-   0        0        0     6168 2023-05-18 11:01:59.000000 pyfem-0.0.7/src/pyfem/materials/ElasticIsotropic.py
+-rw-rw-rw-   0        0        0        0 2023-04-13 12:04:13.000000 pyfem-0.0.7/src/pyfem/materials/__init__.py
+-rw-rw-rw-   0        0        0     1129 2023-05-18 15:11:46.000000 pyfem-0.0.7/src/pyfem/materials/get_material_data.py
+drwxrwxrwx   0        0        0        0 2023-05-21 14:43:31.543121 pyfem-0.0.7/src/pyfem/mesh/
+-rw-rw-rw-   0        0        0     3282 2023-05-21 14:35:56.000000 pyfem-0.0.7/src/pyfem/mesh/ElementSet.py
+-rw-rw-rw-   0        0        0     3478 2023-05-21 14:35:56.000000 pyfem-0.0.7/src/pyfem/mesh/NodeSet.py
+-rw-rw-rw-   0        0        0        0 2023-04-13 12:04:13.000000 pyfem-0.0.7/src/pyfem/mesh/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-21 14:43:31.549570 pyfem-0.0.7/src/pyfem/solvers/
+-rw-rw-rw-   0        0        0      887 2023-05-20 17:07:22.000000 pyfem-0.0.7/src/pyfem/solvers/BaseSolver.py
+-rw-rw-rw-   0        0        0      973 2023-05-20 17:12:32.000000 pyfem-0.0.7/src/pyfem/solvers/LinearSolver.py
+-rw-rw-rw-   0        0        0        0 2023-04-13 12:04:13.000000 pyfem-0.0.7/src/pyfem/solvers/__init__.py
+-rw-rw-rw-   0        0        0      920 2023-05-20 14:12:09.000000 pyfem-0.0.7/src/pyfem/solvers/get_solver_data.py
+drwxrwxrwx   0        0        0        0 2023-05-21 14:43:31.559980 pyfem-0.0.7/src/pyfem/utils/
+-rw-rw-rw-   0        0        0     2313 2023-05-18 11:01:59.000000 pyfem-0.0.7/src/pyfem/utils/IntKeyDict.py
+-rw-rw-rw-   0        0        0        0 2023-04-13 12:04:13.000000 pyfem-0.0.7/src/pyfem/utils/__init__.py
+-rw-rw-rw-   0        0        0      707 2023-05-18 14:59:47.000000 pyfem-0.0.7/src/pyfem/utils/colors.py
+-rw-rw-rw-   0        0        0     1516 2023-05-06 15:26:11.000000 pyfem-0.0.7/src/pyfem/utils/logger.py
+-rw-rw-rw-   0        0        0     1738 2023-05-19 11:01:17.000000 pyfem-0.0.7/src/pyfem/utils/visualization.py
+-rw-rw-rw-   0        0        0      982 2023-05-18 15:11:46.000000 pyfem-0.0.7/src/pyfem/utils/wrappers.py
+drwxrwxrwx   0        0        0        0 2023-05-21 14:43:31.488082 pyfem-0.0.7/src/pyfem.egg-info/
+-rw-rw-rw-   0        0        0      793 2023-05-21 14:43:31.000000 pyfem-0.0.7/src/pyfem.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1493 2023-05-21 14:43:31.000000 pyfem-0.0.7/src/pyfem.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-21 14:43:31.000000 pyfem-0.0.7/src/pyfem.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       46 2023-05-21 14:43:31.000000 pyfem-0.0.7/src/pyfem.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0        6 2023-05-21 14:43:31.000000 pyfem-0.0.7/src/pyfem.egg-info/top_level.txt
```

### Comparing `pyfem-0.0.6/LICENSE` & `pyfem-0.0.7/LICENSE`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -194,8 +194,8 @@
 
        http://www.apache.org/licenses/LICENSE-2.0
 
    Unless required by applicable law or agreed to in writing, software
    distributed under the License is distributed on an "AS IS" BASIS,
    WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
    See the License for the specific language governing permissions and
-   limitations under the License.
+   limitations under the License.
```

### Comparing `pyfem-0.0.6/PKG-INFO` & `pyfem-0.0.7/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,19 +1,20 @@
 Metadata-Version: 2.1
 Name: pyfem
-Version: 0.0.6
+Version: 0.0.7
 Summary: A finite element package for learning
 Home-page: https://github.com/sunwhale/pyfem
 Author: Jingyu Sun
 Author-email: sun.jingyu@outlook.com
 Project-URL: Bug Tracker, https://github.com/sunwhale/pyfem/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # pyfem
+
 A finite element package in python.
 
 [![Codacy Badge](https://app.codacy.com/project/badge/Grade/ab5bca55d85d45d4aa4336ccae058316)](https://app.codacy.com/gh/sunwhale/pyfem/dashboard?utm_source=gh&utm_medium=referral&utm_content=&utm_campaign=Badge_grade)
```

### Comparing `pyfem-0.0.6/setup.py` & `pyfem-0.0.7/setup.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="pyfem",
-    version="0.0.6",
+    version="0.0.7",
     author="Jingyu Sun",
     author_email="sun.jingyu@outlook.com",
     description="A finite element package for learning",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/sunwhale/pyfem",
     project_urls={
```

### Comparing `pyfem-0.0.6/src/pyfem/elements/IsoElementDiagram.py` & `pyfem-0.0.7/src/pyfem/elements/IsoElementDiagram.py`

 * *Files identical despite different names*

### Comparing `pyfem-0.0.6/src/pyfem/elements/IsoElementShape.py` & `pyfem-0.0.7/src/pyfem/elements/IsoElementShape.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,38 +1,34 @@
-from typing import Tuple, Any, Callable
+from typing import Tuple, Callable
 
-from numpy import (empty, meshgrid, outer, column_stack, array, ndarray, dtype, float64)
+from numpy import (empty, meshgrid, outer, column_stack, array, ndarray)
 from numpy.polynomial.legendre import leggauss
 
 from pyfem.elements.IsoElementDiagram import IsoElementDiagram
-from pyfem.utils.colors import error_style, BLUE, GREEN, END
-
-
-def insert_spaces(n: int, text: str) -> str:
-    lines = text.split('\n')
-    indented_lines = [' ' * n + line for line in lines]
-    return '\n'.join(indented_lines)
+from pyfem.utils.colors import error_style
+from pyfem.utils.visualization import object_dict_to_string_ndarray
 
 
 class IsoElementShape:
     """
     等参单元类，设置等参单元的形函数和积分点等信息
     """
     allowed_element_type = ['empty', 'line2', 'line3', 'tria3', 'quad4', 'quad8', 'tetra4', 'hex8']
 
-    def __init__(self, element_type: str):
+    def __init__(self, element_type: str) -> None:
         """
         当前支持的单元类型 ['empty', 'line2', 'line3', 'tria3', 'quad4', 'quad8', 'tetra4', 'hex8']
         """
         self.element_type: str = ''
         self.diagram: str = ''
         self.dimension: int = 0
-        self.number_of_nodes: int = 0
+        self.nodes_number: int = 0
         self.order: int = 0
         self.shape_function: Callable = get_shape_empty
+        self.gp_number = 0
         self.gp_coords: ndarray = empty(0)
         self.gp_weights: ndarray = empty(0)
         self.gp_shape_values: ndarray = empty(0)
         self.gp_shape_gradients: ndarray = empty(0)
 
         if element_type == 'empty':
             self.element_type = element_type
@@ -58,179 +54,178 @@
             self.element_type = element_type
             self.set_hex8()
         else:
             error_msg = f'Unsupported element type {element_type}'
             raise NotImplementedError(error_style(error_msg))
 
     def to_string(self, level: int = 1) -> str:
-        msg = BLUE + self.__str__() + END
-        msg += '\n'
-        for key, item in self.__dict__.items():
-            if isinstance(item, ndarray):
-                msg += '  ' * level + GREEN + f'|- {key}: ' + END + f'{type(item)} with shape = {item.shape} \n'
-                msg += insert_spaces(5, f'{item}') + '\n'
-            else:
-                msg += '  ' * level + GREEN + f'|- {key}: ' + END + f'{item}\n'
-        return msg[:-1]
+        return object_dict_to_string_ndarray(self, level)
+
+    def show(self) -> None:
+        print(self.to_string())
 
     def set_line2(self) -> None:
         self.dimension = 1
-        self.number_of_nodes = 2
+        self.nodes_number = 2
         self.order = 1
         self.gp_coords, self.gp_weights = get_gauss_points(dimension=self.dimension, order=self.order)
+        self.gp_number = len(self.gp_weights)
         self.shape_function = get_shape_line2
         gp_shape_values = []
         gp_shape_gradients = []
         for gp_coord in self.gp_coords:
             h, dhdxi = self.shape_function(gp_coord)
             gp_shape_values.append(h)
             gp_shape_gradients.append(dhdxi)
         self.gp_shape_values = array(gp_shape_values)
         self.gp_shape_gradients = array(gp_shape_gradients)
         self.diagram = IsoElementDiagram.line2
 
     def set_line3(self) -> None:
         self.dimension = 1
-        self.number_of_nodes = 3
+        self.nodes_number = 3
         self.order = 2
         self.gp_coords, self.gp_weights = get_gauss_points(dimension=self.dimension, order=self.order)
+        self.gp_number = len(self.gp_weights)
         self.shape_function = get_shape_line3
         gp_shape_values = []
         gp_shape_gradients = []
         for gp_coord in self.gp_coords:
             h, dhdxi = self.shape_function(gp_coord)
             gp_shape_values.append(h)
             gp_shape_gradients.append(dhdxi)
         self.gp_shape_values = array(gp_shape_values)
         self.gp_shape_gradients = array(gp_shape_gradients)
         self.diagram = IsoElementDiagram.line3
 
     def set_quad4(self) -> None:
         self.dimension = 2
-        self.number_of_nodes = 4
+        self.nodes_number = 4
         self.order = 2
         self.gp_coords, self.gp_weights = get_gauss_points(dimension=self.dimension, order=self.order)
+        self.gp_number = len(self.gp_weights)
         self.shape_function = get_shape_quad4
         gp_shape_values = []
         gp_shape_gradients = []
         for gp_coord in self.gp_coords:
             h, dhdxi = self.shape_function(gp_coord)
             gp_shape_values.append(h)
             gp_shape_gradients.append(dhdxi)
         self.gp_shape_values = array(gp_shape_values)
         self.gp_shape_gradients = array(gp_shape_gradients)
         self.diagram = IsoElementDiagram.quad4
 
     def set_quad8(self) -> None:
         self.dimension = 2
-        self.number_of_nodes = 8
+        self.nodes_number = 8
         self.order = 3
         self.gp_coords, self.gp_weights = get_gauss_points(dimension=self.dimension, order=self.order)
+        self.gp_number = len(self.gp_weights)
         self.shape_function = get_shape_quad8
         gp_shape_values = []
         gp_shape_gradients = []
         for gp_coord in self.gp_coords:
             h, dhdxi = self.shape_function(gp_coord)
             gp_shape_values.append(h)
             gp_shape_gradients.append(dhdxi)
         self.gp_shape_values = array(gp_shape_values)
         self.gp_shape_gradients = array(gp_shape_gradients)
         self.diagram = IsoElementDiagram.quad8
 
     def set_tria3(self) -> None:
         self.dimension = 2
-        self.number_of_nodes = 3
+        self.nodes_number = 3
         self.order = 1
         self.gp_coords, self.gp_weights = get_gauss_points_triangle(order=self.order)
+        self.gp_number = len(self.gp_weights)
         self.shape_function = get_shape_tria3
         gp_shape_values = []
         gp_shape_gradients = []
         for gp_coord in self.gp_coords:
             h, dhdxi = self.shape_function(gp_coord)
             gp_shape_values.append(h)
             gp_shape_gradients.append(dhdxi)
         self.gp_shape_values = array(gp_shape_values)
         self.gp_shape_gradients = array(gp_shape_gradients)
         self.diagram = IsoElementDiagram.tria3
 
     def set_tetra4(self) -> None:
         self.dimension = 3
-        self.number_of_nodes = 4
+        self.nodes_number = 4
         self.order = 1
         self.gp_coords, self.gp_weights = get_gauss_points_tetra(order=self.order)
+        self.gp_number = len(self.gp_weights)
         self.shape_function = get_shape_tetra4
         gp_shape_values = []
         gp_shape_gradients = []
         for gp_coord in self.gp_coords:
             h, dhdxi = self.shape_function(gp_coord)
             gp_shape_values.append(h)
             gp_shape_gradients.append(dhdxi)
         self.gp_shape_values = array(gp_shape_values)
         self.gp_shape_gradients = array(gp_shape_gradients)
         self.diagram = IsoElementDiagram.tetra4
 
     def set_hex8(self) -> None:
         self.dimension = 3
-        self.number_of_nodes = 8
+        self.nodes_number = 8
         self.order = 2
         self.gp_coords, self.gp_weights = get_gauss_points(dimension=self.dimension, order=self.order)
+        self.gp_number = len(self.gp_weights)
         self.shape_function = get_shape_hex8
         gp_shape_values = []
         gp_shape_gradients = []
         for gp_coord in self.gp_coords:
             h, dhdxi = self.shape_function(gp_coord)
             gp_shape_values.append(h)
             gp_shape_gradients.append(dhdxi)
         self.gp_shape_values = array(gp_shape_values)
         self.gp_shape_gradients = array(gp_shape_gradients)
         self.diagram = IsoElementDiagram.hex8
 
 
-def get_shape_empty(xi: ndarray[Any, dtype[float64]]) -> Tuple[
-    ndarray[Any, dtype[float64]], ndarray[Any, dtype[float64]]]:
+def get_shape_empty(xi: ndarray) -> Tuple[ndarray, ndarray]:
     h = empty(0)
     dhdxi = empty(shape=(0, 0))
 
     return h, dhdxi
 
 
-def get_shape_line2(xi: ndarray[Any, dtype[float64]]) -> Tuple[
-    ndarray[Any, dtype[float64]], ndarray[Any, dtype[float64]]]:
+def get_shape_line2(xi: ndarray) -> Tuple[ndarray, ndarray]:
     """
     两节点直线单元
     """
 
     # 0---------------1
     #         +-->x0
 
-    if type(xi) != float and type(xi) != float64:
+    if len(xi) != 1:
         raise NotImplementedError(error_style(f'coordinate {xi} must be dimension 1'))
 
     h = empty(2)
     dhdxi = empty(shape=(2, 1))
 
     h[0] = 0.5 * (1.0 - xi)
     h[1] = 0.5 * (1.0 + xi)
 
     dhdxi[0, 0] = -0.5
     dhdxi[1, 0] = 0.5
 
     return h, dhdxi
 
 
-def get_shape_line3(xi: ndarray[Any, dtype[float64]]) -> Tuple[
-    ndarray[Any, dtype[float64]], ndarray[Any, dtype[float64]]]:
+def get_shape_line3(xi: ndarray) -> Tuple[ndarray, ndarray]:
     """
     三节点直线单元
     """
 
     # 0-------1-------2
     #         +-->x0
 
-    if type(xi) != float and type(xi) != float64:
+    if len(xi) != 1:
         raise NotImplementedError(error_style(f'coordinate {xi} must be dimension 1'))
 
     h = empty(3)
     dhdxi = empty(shape=(1, 3))
 
     h[0] = 0.5 * (1.0 - xi) - 0.5 * (1.0 - xi * xi)
     h[1] = 1 - xi * xi
@@ -239,16 +234,15 @@
     dhdxi[0, 0] = -0.5 + xi
     dhdxi[0, 1] = -2.0 * xi
     dhdxi[0, 2] = 0.5 + xi
 
     return h, dhdxi
 
 
-def get_shape_tria3(xi: ndarray[Any, dtype[float64]]) -> Tuple[
-    ndarray[Any, dtype[float64]], ndarray[Any, dtype[float64]]]:
+def get_shape_tria3(xi: ndarray) -> Tuple[ndarray, ndarray]:
     """
     三节点三角形单元
     """
 
     # 2
     # * *
     # *   *
@@ -275,16 +269,15 @@
     dhdxi[0, 1] = -1.0
     dhdxi[1, 1] = 0.0
     dhdxi[2, 1] = 1.0
 
     return h, dhdxi
 
 
-def get_shape_quad4(xi: ndarray[Any, dtype[float64]]) -> Tuple[
-    ndarray[Any, dtype[float64]], ndarray[Any, dtype[float64]]]:
+def get_shape_quad4(xi: ndarray) -> Tuple[ndarray, ndarray]:
     """
     四节点四边形单元
     """
 
     # 3---------------2
     # |       x1      |
     # |       |       |
@@ -313,16 +306,15 @@
     dhdxi[1, 1] = -0.25 * (1.0 + xi[0])
     dhdxi[2, 1] = 0.25 * (1.0 + xi[0])
     dhdxi[3, 1] = 0.25 * (1.0 - xi[0])
 
     return h, dhdxi
 
 
-def get_shape_quad8(xi: ndarray[Any, dtype[float64]]) -> Tuple[
-    ndarray[Any, dtype[float64]], ndarray[Any, dtype[float64]]]:
+def get_shape_quad8(xi: ndarray) -> Tuple[ndarray, ndarray]:
     """
     八节点四边形单元
     """
 
     # 3-------6-------2
     # |       x1      |
     # |       |       |
@@ -363,16 +355,15 @@
     dhdxi[5, 1] = -0.5 * (1.0 + xi[0]) * (-1.0 + xi[0])
     dhdxi[6, 1] = -0.25 * (-1.0 + xi[0]) * (-xi[0] + 2.0 * xi[1])
     dhdxi[7, 1] = xi[1] * (-1.0 + xi[0])
 
     return h, dhdxi
 
 
-def get_shape_tetra4(xi: ndarray[Any, dtype[float64]]) -> Tuple[
-    ndarray[Any, dtype[float64]], ndarray[Any, dtype[float64]]]:
+def get_shape_tetra4(xi: ndarray) -> Tuple[ndarray, ndarray]:
     """
     四节点四面体单元
     """
 
     # 3
     # * **
     # *   * *
@@ -408,16 +399,15 @@
     dhdxi[1, 2] = 0.0
     dhdxi[2, 2] = 0.0
     dhdxi[3, 2] = 1.0
 
     return h, dhdxi
 
 
-def get_shape_hex8(xi: ndarray[Any, dtype[float64]]) -> Tuple[
-    ndarray[Any, dtype[float64]], ndarray[Any, dtype[float64]]]:
+def get_shape_hex8(xi: ndarray) -> Tuple[ndarray, ndarray]:
     """
     八节点六面体单元
     """
 
     #     7---------------6
     #    /|              /|
     #   / |     x2 x1   / |
@@ -471,18 +461,19 @@
     dhdxi[5, 2] = 0.125 * (1.0 + xi[0]) * (1.0 - xi[1])
     dhdxi[6, 2] = 0.125 * (1.0 + xi[0]) * (1.0 + xi[1])
     dhdxi[7, 2] = 0.125 * (1.0 - xi[0]) * (1.0 + xi[1])
 
     return h, dhdxi
 
 
-def get_gauss_points(dimension: int, order: int) -> Tuple[ndarray[Any, dtype[float64]], ndarray[Any, dtype[float64]]]:
+def get_gauss_points(dimension: int, order: int) -> Tuple[ndarray, ndarray]:
     xi, weight = leggauss(order)
     if dimension == 1:
-        xi = xi
+        xi = xi.reshape(len(xi), -1)
+        weight = weight.reshape(len(weight), -1)
 
     elif dimension == 2:
         xi1, xi2 = meshgrid(xi, xi)
         xi1 = xi1.ravel()
         xi2 = xi2.ravel()
         xi = column_stack((xi1, xi2))
         weight = outer(weight, weight)
@@ -496,15 +487,15 @@
         xi = column_stack((xi1, xi2, xi3))
         weight = outer(outer(weight, weight), weight)
         weight = weight.ravel()
 
     return xi, weight
 
 
-def get_gauss_points_triangle(order: int) -> Tuple[ndarray[Any, dtype[float64]], ndarray[Any, dtype[float64]]]:
+def get_gauss_points_triangle(order: int) -> Tuple[ndarray, ndarray]:
     if order == 1:
         xi = [[1.0 / 3.0, 1.0 / 3.0]]
         weight = [0.5]
 
     elif order == 3:
         r1 = 1.0 / 6.0
         r2 = 2.0 / 3.0
@@ -526,35 +517,81 @@
 
     else:
         raise NotImplementedError(error_style('Order must be 1, 3 or 7'))
 
     return array(xi), array(weight)
 
 
-def get_gauss_points_tetra(order: int) -> Tuple[ndarray[Any, dtype[float64]], ndarray[Any, dtype[float64]]]:
+def get_gauss_points_tetra(order: int) -> Tuple[ndarray, ndarray]:
     if order == 1:
         third = 1.0 / 3.0
         xi = [[third, third, third]]
         weight = [0.5 * third]
     else:
         raise NotImplementedError(error_style('Only order 1 integration implemented'))
 
     return array(xi), array(weight)
 
 
-def get_gauss_points_pyramid(order: int) -> Tuple[ndarray[Any, dtype[float64]], ndarray[Any, dtype[float64]]]:
+def get_gauss_points_pyramid(order: int) -> Tuple[ndarray, ndarray]:
     if order == 1:
         xi = [[0., 0., -0.5]]
         weight = [128.0 / 27.0]
     else:
         raise NotImplementedError(error_style('Only order 1 integration implemented'))
 
     return array(xi), array(weight)
 
 
+def get_default_element_type(node_coords: ndarray) -> str:
+    num_element_nodes = node_coords.shape[0]
+    dimension = node_coords.shape[1]
+
+    if dimension == 1:
+        if num_element_nodes == 2:
+            return "line2"
+        elif num_element_nodes == 3:
+            return "line3"
+        else:
+            error_msg = f'No 1D element with {num_element_nodes} nodes available'
+            raise NotImplementedError(error_style(error_msg))
+    elif dimension == 2:
+        if num_element_nodes == 3:
+            return "tria3"
+        elif num_element_nodes == 4:
+            return "quad4"
+        elif num_element_nodes == 6:
+            return "tria6"
+        elif num_element_nodes == 8:
+            return "quad8"
+        elif num_element_nodes == 9:
+            return "quad9"
+        else:
+            error_msg = f'No 2D element with {num_element_nodes} nodes available'
+            raise NotImplementedError(error_style(error_msg))
+    elif dimension == 3:
+        if num_element_nodes == 4:
+            return "tetra4"
+        elif num_element_nodes == 5:
+            return "pyramid5"
+        elif num_element_nodes == 6:
+            return "prism6"
+        elif num_element_nodes == 8:
+            return "hex8"
+        elif num_element_nodes == 18:
+            return "prism18"
+        elif num_element_nodes == 20:
+            return "hex20"
+        else:
+            error_msg = f'No 3D element with {num_element_nodes} nodes available'
+            raise NotImplementedError(error_style(error_msg))
+    else:
+        raise NotImplementedError(error_style(f'Unsupported dimension {dimension}'))
+
+
 if __name__ == "__main__":
     # iso_element_shape = IsoElementShape('tria3')
     # iso_element_shape = IsoElementShape('quad4')
     # iso_element_shape = IsoElementShape('hex8')
     # iso_element_shape = IsoElementShape('quad8')
     # iso_element_shape = IsoElementShape('tetra4')
     # iso_element_shape = IsoElementShape('line2')
```

### Comparing `pyfem-0.0.6/src/pyfem/fem/NodeSet.py` & `pyfem-0.0.7/src/pyfem/mesh/NodeSet.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,28 +1,30 @@
 import os
-from typing import List, Any
+from pathlib import Path
+from typing import List, Any, Dict, Union
 
 import meshio  # type: ignore
 import numpy as np
 
 from pyfem.utils.IntKeyDict import IntKeyDict
 from pyfem.utils.logger import get_logger
+from pyfem.utils.wrappers import show_running_time
 
 logger = get_logger()
 
 
 class NodeSet(IntKeyDict):
 
-    def __init__(self):
+    def __init__(self) -> None:
         super().__init__()
-        self.dimension = -1  # int
-        self.node_sets = {}  # Dict[str, List[int]]
+        self.dimension: int = -1
+        self.node_sets: Dict[str, List[int]] = {}
 
     def show(self) -> None:
-        logger.info(self.to_string(level=0))
+        print(self.to_string(0))
 
     def to_string(self, level=1) -> str:
         msg = 'Number of nodes ............ %6d\n' % len(self)
         space = '   ' * level
         if len(self.node_sets) > 0:
             msg += space + '  Number of node_sets ........ %6d\n' % len(self.node_sets)
             msg += space + '  -----------------------------------\n'
@@ -30,18 +32,19 @@
             msg += space + '    ---------------------------------\n'
 
             for name in self.node_sets:
                 msg += space + '    %-16s           %6d\n' % (name, len(self.node_sets[name]))
 
         return msg[:-1]
 
-    def read_gmsh_file(self, file_name: str) -> None:
-        logger.info(f"Reading nodes from {file_name}")
+    @show_running_time
+    def read_gmsh_file(self, filename: Union[Path, str]) -> None:
+        logger.info(f"Reading nodes from {filename}")
 
-        mesh = meshio.read(file_name, file_format='gmsh')
+        mesh = meshio.read(filename, file_format='gmsh')
 
         # 可以通过以下命令查看支持的单元类型
         # print(meshio.gmsh.meshio_to_gmsh_type)
         # print(meshio.gmsh.gmsh_to_meshio_type)
 
         keywords_1d = ['line']
         keywords_2d = ['triangle', 'quad']
@@ -81,14 +84,14 @@
 
 if __name__ == "__main__":
     from pyfem.utils.logger import set_logger
 
     set_logger()
 
     nodes = NodeSet()
-    os.chdir(r'F:\Github\pyfem\examples\rectangle')
-    # nodes.read_gmsh_file('rectangle.msh')
+    os.chdir(r'/examples/rectangle')
+    # nodes.read_gmsh_file('rectangle100.msh')
     nodes.read_gmsh_file('rectangle10000.msh')
     # print(nodes.dimension)
     # print(nodes.node_sets)
     print(nodes.get_coords_by_ids([0, 1, 2]))
     nodes.show()
```

### Comparing `pyfem-0.0.6/src/pyfem/io/arguments.py` & `pyfem-0.0.7/src/pyfem/io/arguments.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,39 +1,51 @@
-import argparse
 import sys
-from typing import Tuple
+from argparse import ArgumentParser, Namespace, SUPPRESS
 
 
-def get_arguments() -> Tuple[str, str, str]:
+def get_arguments() -> Namespace:
+    logo = r"""
+                     ____             
+        ____  __  __/ __/__  ____ ___ 
+       / __ \/ / / / /_/ _ \/ __ `__ \
+      / /_/ / /_/ / __/  __/ / / / / /
+     / .___/\__, /_/  \___/_/ /_/ /_/ 
+    /_/    /____/                     
+    """
+
+    print(logo)
+
     # 创建一个 argparse 解析器对象
-    parser = argparse.ArgumentParser(add_help=False)
+    parser = ArgumentParser(add_help=False)
 
     # 添加程序输入文件选项
     parser.add_argument('-i', metavar='input', type=str,
                         help='Identify the input file.')
 
     # 添加程序输出文件选项
     parser.add_argument('-o', metavar='output', type=str,
                         help='Identify the output file.')
 
     # 添加参数选项
     parser.add_argument('-p', metavar='parameter', type=str,
                         help='Parameter to pass to the program.')
 
     # 添加帮助选项
-    parser.add_argument('-h', '--help', action='help', default=argparse.SUPPRESS,
+    parser.add_argument('-h', '--help', action='help', default=SUPPRESS,
                         help='Show this help message and exit.')
 
     # 添加版本选项
     parser.add_argument('-v', '--version', action='version', help='Show program\'s version number and exit.',
-                        version='%(prog)s 0.0.5')
+                        version='pyfem 0.0.7')
 
     # 解析命令行参数
     args = parser.parse_args()
 
     # 如果未指定程序输入文件，则打印帮助并退出
     if not args.i:
-        print('error: the input file is required.')
+        print('--------------------------------------')
+        print('>>> error: the input file is required.')
+        print('--------------------------------------')
         parser.print_help()
         sys.exit()
 
-    return args.i, args.o, args.p
+    return args
```

### Comparing `pyfem-0.0.6/src/pyfem/utils/IntKeyDict.py` & `pyfem-0.0.7/src/pyfem/utils/IntKeyDict.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,31 +1,31 @@
-from typing import List, Any
+from typing import Dict, List, Any
 
 
 class IntKeyDict(dict):
     """
     关键字只能为整数（Integer）类型的字典，已经存在的键值无法通过赋值方法（__setitem__）更改。
     """
 
-    def __init__(self):
+    def __init__(self) -> None:
         super().__init__()
-        self.indices_to_ids = {}
-        self.ids_to_indices = {}
+        self.indices_to_ids: Dict[int, int] = {}
+        self.ids_to_indices: Dict[int, int] = {}
         self.update_indices()
 
     def __setitem__(self, key: int, value: Any) -> None:
         if isinstance(key, int):
             if key in self:
                 raise KeyError(f"Key {key} already exists")
             else:
                 super().__setitem__(key, value)
         else:
             raise TypeError("Key must be an integer")
 
-    def update_indices(self):
+    def update_indices(self) -> None:
         list_of_keys = list(self.keys())
         self.ids_to_indices = {key: i for i, key in enumerate(list_of_keys)}
         self.indices_to_ids = {i: key for i, key in enumerate(list_of_keys)}
 
     def add_item_by_id(self, id_: int, item: Any) -> None:
         self[id_] = item
```

### Comparing `pyfem-0.0.6/src/pyfem/utils/colors.py` & `pyfem-0.0.7/src/pyfem/utils/colors.py`

 * *Files 18% similar despite different names*

```diff
@@ -21,8 +21,16 @@
     RED = ''
     BOLD = ''
     UNDERLINE = ''
     END = ''
 
 
 def error_style(error_msg: str) -> str:
-    return MAGENTA + BOLD + error_msg + END
+    return RED + BOLD + error_msg + END
+
+
+def info_style(info_msg: str) -> str:
+    return GREEN + BOLD + info_msg + END
+
+
+def warn_style(info_msg: str) -> str:
+    return YELLOW + BOLD + info_msg + END
```

### Comparing `pyfem-0.0.6/src/pyfem/utils/logger.py` & `pyfem-0.0.7/src/pyfem/utils/logger.py`

 * *Files identical despite different names*

### Comparing `pyfem-0.0.6/src/pyfem.egg-info/PKG-INFO` & `pyfem-0.0.7/src/pyfem.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,19 +1,20 @@
 Metadata-Version: 2.1
 Name: pyfem
-Version: 0.0.6
+Version: 0.0.7
 Summary: A finite element package for learning
 Home-page: https://github.com/sunwhale/pyfem
 Author: Jingyu Sun
 Author-email: sun.jingyu@outlook.com
 Project-URL: Bug Tracker, https://github.com/sunwhale/pyfem/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # pyfem
+
 A finite element package in python.
 
 [![Codacy Badge](https://app.codacy.com/project/badge/Grade/ab5bca55d85d45d4aa4336ccae058316)](https://app.codacy.com/gh/sunwhale/pyfem/dashboard?utm_source=gh&utm_medium=referral&utm_content=&utm_campaign=Badge_grade)
```

