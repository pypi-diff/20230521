# Comparing `tmp/dratio-0.0.8.tar.gz` & `tmp/dratio-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dratio-0.0.8.tar", last modified: Sun Oct 23 11:06:42 2022, max compression
+gzip compressed data, was "dratio-0.0.9.tar", last modified: Tue Nov  1 17:05:54 2022, max compression
```

## Comparing `dratio-0.0.8.tar` & `dratio-0.0.9.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-23 11:06:42.675741 dratio-0.0.8/
--rw-r--r--   0 runner    (1001) docker     (121)    11357 2022-10-23 11:06:29.000000 dratio-0.0.8/LICENSE
--rw-r--r--   0 runner    (1001) docker     (121)     4556 2022-10-23 11:06:42.675741 dratio-0.0.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     3654 2022-10-23 11:06:29.000000 dratio-0.0.8/README.md
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-23 11:06:42.671741 dratio-0.0.8/dratio/
--rw-r--r--   0 runner    (1001) docker     (121)      864 2022-10-23 11:06:29.000000 dratio-0.0.8/dratio/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)    12158 2022-10-23 11:06:29.000000 dratio-0.0.8/dratio/base.py
--rw-r--r--   0 runner    (1001) docker     (121)     6071 2022-10-23 11:06:29.000000 dratio-0.0.8/dratio/client.py
--rw-r--r--   0 runner    (1001) docker     (121)     1175 2022-10-23 11:06:29.000000 dratio-0.0.8/dratio/exceptions.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-23 11:06:42.671741 dratio-0.0.8/dratio.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)     4556 2022-10-23 11:06:42.000000 dratio-0.0.8/dratio.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      247 2022-10-23 11:06:42.000000 dratio-0.0.8/dratio.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-10-23 11:06:42.000000 dratio-0.0.8/dratio.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)       72 2022-10-23 11:06:42.000000 dratio-0.0.8/dratio.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)        7 2022-10-23 11:06:42.000000 dratio-0.0.8/dratio.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (121)       38 2022-10-23 11:06:42.675741 dratio-0.0.8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)     1319 2022-10-23 11:06:29.000000 dratio-0.0.8/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-01 17:05:54.587813 dratio-0.0.9/
+-rw-r--r--   0 runner    (1001) docker     (121)    11357 2022-11-01 17:05:39.000000 dratio-0.0.9/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (121)     4556 2022-11-01 17:05:54.583813 dratio-0.0.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (121)     3654 2022-11-01 17:05:39.000000 dratio-0.0.9/README.md
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-01 17:05:54.583813 dratio-0.0.9/dratio/
+-rw-r--r--   0 runner    (1001) docker     (121)      864 2022-11-01 17:05:39.000000 dratio-0.0.9/dratio/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)    16175 2022-11-01 17:05:39.000000 dratio-0.0.9/dratio/base.py
+-rw-r--r--   0 runner    (1001) docker     (121)     6071 2022-11-01 17:05:39.000000 dratio-0.0.9/dratio/client.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1175 2022-11-01 17:05:39.000000 dratio-0.0.9/dratio/exceptions.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-01 17:05:54.583813 dratio-0.0.9/dratio.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (121)     4556 2022-11-01 17:05:54.000000 dratio-0.0.9/dratio.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (121)      247 2022-11-01 17:05:54.000000 dratio-0.0.9/dratio.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (121)        1 2022-11-01 17:05:54.000000 dratio-0.0.9/dratio.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (121)       72 2022-11-01 17:05:54.000000 dratio-0.0.9/dratio.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (121)        7 2022-11-01 17:05:54.000000 dratio-0.0.9/dratio.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (121)       38 2022-11-01 17:05:54.587813 dratio-0.0.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (121)     1319 2022-11-01 17:05:39.000000 dratio-0.0.9/setup.py
```

### Comparing `dratio-0.0.8/LICENSE` & `dratio-0.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `dratio-0.0.8/PKG-INFO` & `dratio-0.0.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dratio
-Version: 0.0.8
+Version: 0.0.9
 Summary: Python client library for dratio.io API Web services
 Author: dratio.io
 Author-email: info@dratio.io
 License: Apache 2.0
 Project-URL: Home, https://dratio.io
 Project-URL: GitHub, https://github.com/dratio-io/dratio-python
 Project-URL: Docs, https://dratio.readthedocs.io/
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: dratio Version: 0.0.8 Summary: Python client
+Metadata-Version: 2.1 Name: dratio Version: 0.0.9 Summary: Python client
 library for dratio.io API Web services Author: dratio.io Author-email:
 info@dratio.io License: Apache 2.0 Project-URL: Home, https://dratio.io
 Project-URL: GitHub, https://github.com/dratio-io/dratio-python Project-URL:
 Docs, https://dratio.readthedocs.io/ Platform: Posix; MacOS X; Windows
 Classifier: Development Status :: 1 - Planning Classifier: Intended Audience ::
 Developers Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent Classifier: Programming Language
```

### Comparing `dratio-0.0.8/README.md` & `dratio-0.0.9/README.md`

 * *Files identical despite different names*

### Comparing `dratio-0.0.8/dratio/__init__.py` & `dratio-0.0.9/dratio/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -17,12 +17,12 @@
 #
 # The use of the services offered by this client must be in accordance with
 # dratio's terms and conditions. You may obtain a copy of the terms at
 #
 #     https://dratio.io/legal/terms
 #
 
-__version__ = "0.0.8"
+__version__ = "0.0.9"
 
 from .client import Client
 
 __all__ = ["Client"]
```

### Comparing `dratio-0.0.8/dratio/base.py` & `dratio-0.0.9/dratio/base.py`

 * *Files 23% similar despite different names*

```diff
@@ -19,15 +19,15 @@
 # dratio's terms and conditions. You may obtain a copy of the terms at
 #
 #     https://dratio.io/legal/terms
 #
 import io
 from typing import Any, Dict, List, Optional
 
-try: # Compatibility with Python 3.7
+try:  # Compatibility with Python 3.7
     from typing import Literal
 except ImportError:
     from typing_extensions import Literal
 
 import pandas as pd
 import requests
 
@@ -74,16 +74,15 @@
 
     def __repr__(self) -> str:
         """Returns a string representation of the object"""
         return f"{self.__class__.__name__}('{self.code}')"
 
     @property
     def metadata(self) -> Dict[str, Any]:
-        """Information associated (metadata) to the object referenced in the database
-        (`Dict[str, Any]`, read-only).
+        """Information associated (metadata) (`Dict[str, Any]`, read-only).
 
         Notes
         -----
         The first time the property is accessed, a request is made to the server to
         obtain the information. In successive accesses the previously loaded information
         is returned. In case of needing to update the information, a new object
         must be created.
@@ -143,16 +142,153 @@
     code : str
        Unique identifier of the feature in the database.
     client: Client
         Client object used to perform requests to the database.
     **kwargs
         Additional keyword arguments used to initialize the metadata information.
 
+    Examples
+    --------
+
+    Initialize a client object and get a dataset object
+
+    >>> from dratio import Client
+    >>> client = Client("YOUR_API_KEY")
+    >>> dataset = client.get("municipalities")
+
+    Obtain a feature from the dataset features dictionary by column name
+
+    >>> feature = dataset.features.get("municipality_id")
+    >>> feature
+    Feature('municipalities__municipality-id')
+
+    Get feature's attributes
+
+    >>> feature.name
+    'Municipality ID'
+    >>> feature.description
+    'Municipality code (int format) assigned by the National Statistics Institute...'
+
+    Obtain all metadata associated with the feature
+
+    >>> feature.metadata
+    {'code': 'municipalities__municipality-id', ...}
+
     """
-    _URL = "upload/feature/"
+    _URL = "marketplace/token/features/"
+
+    @property
+    def name(self) -> str:
+        """Name of the feature (`str`, read-only).
+
+        Examples
+        --------
+        Obtain the name of a feature.
+
+        >>> feature.name
+        'Municipality ID'
+        """
+        return self.metadata['name']
+
+    @property
+    def description(self) -> str:
+        """Description of the feature (`str`, read-only).
+
+        Examples
+        --------
+        Obtain the description of a feature.
+
+        >>> feature.description
+        'Municipality code (int format) assigned by the National Statistics Institute...'
+
+        """
+        return self.metadata['description']
+
+    @property
+    def column(self) -> str:
+        """Name of the column in the dataset (`str`, read-only).
+
+        Examples
+        --------
+        Obtain the column name of a feature.
+
+        >>> feature.description
+        'municipality_id'
+        """
+        return self.metadata['column']
+
+    @property
+    def feature_type(self) -> str:
+        """Type of the feature (`str`, read-only).
+
+        Examples
+        --------
+        Obtain the type of a feature.
+
+        >>> feature.feature_type
+        'identifier'
+
+        """
+        return self.metadata['feature_type']
+
+    @property
+    def data_type(self) -> str:
+        """Data type of the feature (`str`, read-only).
+
+        Examples
+        --------
+        Obtain the data type of a feature.
+
+        >>> feature.data_type
+        'int'
+
+        """
+        return self.metadata['data_type']
+
+    @property
+    def last_update(self) -> str:
+        """Date of the last update of the feature (`str`, read-only).
+
+        Examples
+        --------
+        Obtain the last update date of a feature.
+
+        >>> feature.last_update
+        '2022-10-21'
+
+        """
+        return self.metadata['last_update']
+
+    @property
+    def next_update(self) -> str:
+        """Date of the next update of the feature (`str`, read-only).
+
+        Examples
+        --------
+        Obtain the schedule of the next update for the feature.
+
+        >>> feature.next_update
+        '2024-01-01'
+
+        """
+        return self.metadata['next_update']
+
+    @property
+    def update_frequency(self) -> str:
+        """Frequency of the updates of the feature (`str`, read-only).
+
+        Examples
+        --------
+        Obtain the update frequency of a feature.
+
+        >>> feature.update_frequency
+        'yearly'
+
+        """
+        return self.metadata['update_frequency']
 
 
 class File(BaseDBObject):
     """File of a dataset in the database
 
     Parameters
     ----------
@@ -246,38 +382,44 @@
 
 
     Examples
     --------
     Retrieve a dataset from the dratio.io marketplace:
 
     >>> from dratio import Client
-    >>> client = Client(key='<your_api_key>')
-    >>> dataset = client.get(code='unemployment-municipality')
+    >>> client = Client('YOUR_API_KEY')
+    >>> dataset = client.get('municipalities')
     >>> dataset
-    Dataset('unemployment-municipality')
+    Dataset('municipalities')
 
     Access fields included in the metadata of the dataset:
-
-    >>> dataset["description"]
-    'Monthly data on the number of unemployed persons by municipality, ...'
+    
+    >>> dataset.name
+    'Municipalities'
+    >>> dataset.description
+    'Municipalities of Spain according to the name under which they are registered ...'
 
     Get a dictionary with all metadata:
 
     >>> dataset.metadata
-    {'code': 'unemployment-municipality', 'name': 'Unemployment, contracts and ...', ...}
+    {'code': 'municipalities', 'name': 'Municipalities', 'description': ...}
 
 
     Get current version of the dataset
 
     >>> dataset.version
-    Version('unemployment-municipality-v1')
+    Version('municipalities-v1')
 
     Download a dataset as a pandas dataframe:
 
     >>> df = dataset.to_pandas()
+
+    Download as a geopandas dataframe (for geospatial datasets):
+
+    >>> gdf = dataset.to_geopandas()
     """
     _URL = "marketplace/token/datasets/"
 
     def __init__(self, client, code: str, version: Optional[str] = None):
         """Initializes the Dataset object"""
         super().__init__(code=code, client=client)
         if version is not None:
@@ -289,15 +431,17 @@
         self._features = None
 
     def _fetch_features(self) -> None:
         """Fetches information of the dataset features"""
         params = {"dataset": self.code}
         features = self._client._perform_request(
             Feature._URL, params=params)
-        self._features = features.json()
+        features = features.json()
+        self._features = {
+            feature["column"]: Feature(client=self._client, code=feature["code"]) for feature in features}
 
     def fetch(self) -> "Dataset":
         """Updates the metadata dictionary of the dataset.
 
         This method perform an HTTP request to the server to obtain the information.
 
         Returns
@@ -308,47 +452,52 @@
         Notes
         -----
         This method modifies the object's metadata attribute.
 
 
         Raises
         ------
-            requests.exceptions.RequestException.
-                If the request fails due to an HTTP or Conection Error..
-            ObjectNotFound.
-                If the object is not found in the database.
+        requests.exceptions.RequestException.
+            If the request fails due to an HTTP or Conection Error..
+        ObjectNotFound.
+            If the object is not found in the database.
 
         """
         super().fetch()
         self._fetch_features()
 
         return self
 
     @property
-    def features(self) -> List[Feature]:
-        """Return a list with all the features of the dataset (List[Feature], read-only)."""
+    def features(self) -> Dict[str, Feature]:
+        """Dictionary with features indexed by column name (Dict[str, Feature], read-only)."""
         if not self._fetched:
             self.fetch()
         return self._features
 
     @property
+    def columns(self) -> List[str]:
+        """Return a list with all the columns of the dataset (List[str], read-only)."""
+        return list(self.features.keys())
+
+    @property
     def version(self) -> Version:
         """Return the current version of the dataset (Version, read-only)."""
         if self._version is None:
             v = self._client._perform_request(url=Version._URL, params=dict(
                 dataset=self.code)).json()
 
             if len(v) != 1:
                 raise ObjectNotFound("Version", self.code)
 
             self._version = Version(client=self._client, **v[0])
 
         return self._version
 
-    def to_pandas(self):
+    def to_pandas(self) -> 'pd.DataFrame':
         """Downloads the dataset as a pandas dataframe.
 
         Returns
         -------
         pandas.DataFrame
             Dataframe with the dataset.
 
@@ -370,28 +519,30 @@
             df_list.append(df)
 
         if len(df_list) > 1:
             df = pd.concat(df_list)
 
         return df
 
-    def to_geopandas(self):
+    def to_geopandas(self) -> 'gpd.GeoDataFrame':
         """Downloads the dataset as a geopandas geodataframe.
 
         Returns
         -------
         geopandas.GeoDataFrame
             GeoDataFrame with the dataset.
 
         Notes
         -----
         This method requires the geopandas library to be installed.
 
         Raises
         ------
+        ImportError.
+            If the geopandas library is not installed. You can install it using `pip install dratio[geo]`.
         requests.exceptions.RequestException.
             If the request fails due to an HTTP or Conection Error.
         """
         if not _has_geopandas:
             raise ImportError(
                 "geopandas is required to load a dataset with geometries")
 
@@ -410,7 +561,20 @@
             gdf = gpd.read_parquet(f)
             gdf_list.append(gdf)
 
         if len(gdf_list) > 1:
             gdf = pd.concat(gdf_list)
 
         return gdf
+
+
+    @property
+    def name(self) -> str:
+        """Name of the dataset (str, read-only)."""
+        return self.metadata["name"]
+
+    @property
+    def description(self) -> str:
+        """Description of the dataset (str, read-only)."""
+        return self.metadata["description"]
+
+
```

### Comparing `dratio-0.0.8/dratio/client.py` & `dratio-0.0.9/dratio/client.py`

 * *Files identical despite different names*

### Comparing `dratio-0.0.8/dratio/exceptions.py` & `dratio-0.0.9/dratio/exceptions.py`

 * *Files identical despite different names*

### Comparing `dratio-0.0.8/dratio.egg-info/PKG-INFO` & `dratio-0.0.9/dratio.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dratio
-Version: 0.0.8
+Version: 0.0.9
 Summary: Python client library for dratio.io API Web services
 Author: dratio.io
 Author-email: info@dratio.io
 License: Apache 2.0
 Project-URL: Home, https://dratio.io
 Project-URL: GitHub, https://github.com/dratio-io/dratio-python
 Project-URL: Docs, https://dratio.readthedocs.io/
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: dratio Version: 0.0.8 Summary: Python client
+Metadata-Version: 2.1 Name: dratio Version: 0.0.9 Summary: Python client
 library for dratio.io API Web services Author: dratio.io Author-email:
 info@dratio.io License: Apache 2.0 Project-URL: Home, https://dratio.io
 Project-URL: GitHub, https://github.com/dratio-io/dratio-python Project-URL:
 Docs, https://dratio.readthedocs.io/ Platform: Posix; MacOS X; Windows
 Classifier: Development Status :: 1 - Planning Classifier: Intended Audience ::
 Developers Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent Classifier: Programming Language
```

### Comparing `dratio-0.0.8/setup.py` & `dratio-0.0.9/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 
 with open("README.md") as f:
     readme = f.read()
 
 
 setup(
     name="dratio",
-    version="0.0.8",
+    version="0.0.9",
     description="Python client library for dratio.io API Web services",
     long_description=readme,
     long_description_content_type="text/markdown",
     author="dratio.io",
     author_email="info@dratio.io",
     scripts=[],
     project_urls={
```

