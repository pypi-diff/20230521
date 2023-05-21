# Comparing `tmp/fastapi_react_admin-2.0.1.tar.gz` & `tmp/fastapi_react_admin-2.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fastapi_react_admin-2.0.1.tar", max compression
+gzip compressed data, was "fastapi_react_admin-2.0.2.tar", max compression
```

## Comparing `fastapi_react_admin-2.0.1.tar` & `fastapi_react_admin-2.0.2.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0       35 2023-05-17 17:29:31.844703 fastapi_react_admin-2.0.1/fastapi_react_admin/__init__.py
--rw-r--r--   0        0        0     7650 2023-05-21 09:10:18.466156 fastapi_react_admin-2.0.1/fastapi_react_admin/react_admin.py
--rw-r--r--   0        0        0      149 2023-05-18 08:55:36.202042 fastapi_react_admin-2.0.1/fastapi_react_admin/schemas.py
--rw-r--r--   0        0        0      426 2023-05-21 09:10:32.971603 fastapi_react_admin-2.0.1/pyproject.toml
--rw-r--r--   0        0        0     5045 2023-05-19 07:47:11.756747 fastapi_react_admin-2.0.1/README.md
--rw-r--r--   0        0        0     5752 1970-01-01 00:00:00.000000 fastapi_react_admin-2.0.1/setup.py
--rw-r--r--   0        0        0     5407 1970-01-01 00:00:00.000000 fastapi_react_admin-2.0.1/PKG-INFO
+-rw-r--r--   0        0        0       35 2023-05-17 17:29:31.844703 fastapi_react_admin-2.0.2/fastapi_react_admin/__init__.py
+-rw-r--r--   0        0        0     7698 2023-05-21 09:14:53.617773 fastapi_react_admin-2.0.2/fastapi_react_admin/react_admin.py
+-rw-r--r--   0        0        0      149 2023-05-18 08:55:36.202042 fastapi_react_admin-2.0.2/fastapi_react_admin/schemas.py
+-rw-r--r--   0        0        0      426 2023-05-21 09:15:15.319515 fastapi_react_admin-2.0.2/pyproject.toml
+-rw-r--r--   0        0        0     5045 2023-05-19 07:47:11.756747 fastapi_react_admin-2.0.2/README.md
+-rw-r--r--   0        0        0     5752 1970-01-01 00:00:00.000000 fastapi_react_admin-2.0.2/setup.py
+-rw-r--r--   0        0        0     5407 1970-01-01 00:00:00.000000 fastapi_react_admin-2.0.2/PKG-INFO
```

### Comparing `fastapi_react_admin-2.0.1/fastapi_react_admin/react_admin.py` & `fastapi_react_admin-2.0.2/fastapi_react_admin/react_admin.py`

 * *Files 2% similar despite different names*

```diff
@@ -109,23 +109,24 @@
     
     async def _get_one(self, id: Union[int, str]):
         async with self.Session() as session:
             result = await session.get(self.table, id)
             return RaResponseModel(data=result)
     
     async def _get_many(self, filter: Json = Query()):
+        internal_filter = {}
         if self.deleted_filed and self.exclude_deleted:
-            filter[self.deleted_filed] = False
+            internal_filter[self.deleted_filed] = False
 
         async with self.Session() as session:
             result = await session.execute(
                 select(self.table).where(
                     self.table.id.in_(filter['id'])
                 ).filter_by(
-                    **filter
+                    **internal_filter
                 )
             )
         
             return RaResponseModel(data=result)
 
     async def _create(self, request: Request):
         async with self.Session() as session:
```

### Comparing `fastapi_react_admin-2.0.1/README.md` & `fastapi_react_admin-2.0.2/README.md`

 * *Files identical despite different names*

### Comparing `fastapi_react_admin-2.0.1/setup.py` & `fastapi_react_admin-2.0.2/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 {'': ['*']}
 
 install_requires = \
 ['fastapi>=0.95.2,<0.96.0', 'sqlalchemy>=2.0.13,<3.0.0']
 
 setup_kwargs = {
     'name': 'fastapi-react-admin',
-    'version': '2.0.1',
+    'version': '2.0.2',
     'description': 'Module to automaticly generate fastapi routes for using react admin',
     'long_description': '# FastAPI React Admin\n\nThis module provides a class ReactAdmin that allows for the automatic generation of routes for React Admin in a FastAPI application.\n\n## Installation\n```console\npip install fastapi-react-admin\n```\n\n## Base usage\n\nFatstAPI part: \n```python\nfrom fastapi import FastAPI\n\nfrom schemas import MyTableModel\nfrom fastapi_react_admin import ReactAdmin\n\napp = FastAPI()\nrouter = app.router\nSession = async_sessionmaker(AsyncSession)\n\nReactAdmin(\n    table=MyTableModel,  \n    session=Session\n).mount(router)\n```\n\nReact Admin data provider:\n```js\nexport const sendPost = async (resource: string, method: string, body?: any) => {\n    const response = await axios({\n        method: \'post\',\n        url: resource + "/ra" + method,\n        data: body,\n        headers: {\n            "Admin-Token": sessionStorage.getItem(\'token\')\n        }\n    })\n\n    return response.data\n}\n\nconst dataProvider: DataProvider = {\n    getList: (resource: string, params: any) => {\n        const { page, perPage } = params.pagination\n        const { field, order } = params.sort\n\n        const query = {\n            sort: JSON.stringify([field, order]),\n            range_: JSON.stringify([(page - 1) * perPage, page * perPage - 1]),\n            filter: JSON.stringify(params.filter),\n        }\n\n        return sendPost(resource, `/getList?${queryString.stringify(query)}`)\n    },\n\n    getOne: async (resource: string, params: any) => {\n        return await sendPost(resource, \'/getOne/\' + params.id)\n    },\n\n    getMany: (resource: string, params: any) => {\n        const query = {\n            filter: JSON.stringify({ id: params.ids}),\n        }\n\n        return sendPost(resource, `/getMany?${queryString.stringify(query)}`)\n    },\n\n    getManyReference: (resource: string, params: any): any => {\n        const { page, perPage } = params.pagination\n        const { field, order } = params.sort\n\n        const query = {\n            sort: JSON.stringify([field, order]),\n            range_: JSON.stringify([(page - 1) * perPage, page * perPage - 1]),\n            filter: JSON.stringify(params.filter),\n        }\n\n        return sendPost(params.target, `/getList?${queryString.stringify(query)}`)\n    },\n\n    create: async (resource: string, params: any) => {\n        return await sendPost(resource, \'/create\', { \n            ...params.data\n        })\n    },\n\n    update: async (resource: string, params: any) => {\n        return await sendPost(resource, \'/update/\' + params.id, params.data)\n    },\n\n    updateMany: async (resource: string, params: any) => {\n        const query = {\n            filter: JSON.stringify({ id: params.ids}),\n        }\n\n        return await sendPost(resource, `/updateMany?${queryString.stringify(query)}`, params.data)\n    },\n\n    delete: (resource: string, params: any) => {\n        return sendPost(resource, \'/delete/\' + params.id)\n    },\n\n    deleteMany: (resource: string, params: any) => {\n        const query = {\n            filter: JSON.stringify({ id: params.ids}),\n        }\n\n        return sendPost(resource, `/deleteMany?${queryString.stringify(query)}` )\n    },\n}\n\n```\n\n\n### ReactAdmin class params\n- table (required): The SQLAlchemy model representing the database table.\n\n- session (required): The async_sessionmaker[AsyncSession] for the database session.\n\n- deleted_field (optional): The name of the field of the table to mark deleted fields (e.g., \'is_deleted\'). Default is None.\n\n- exclude_deleted (optional): Whether to exclude deleted records. Default is True.\n\n- include_in_schema (optional): Whether to include the routes in the generated schema. Default is False.\n\n### ReactAdmin mount params\n- router (required): The APIRouter instance to mount the routes.\n\n- depends (optional): The sequence of the dependencies\n\n- prefix (optional): The URL prefix for the React Admin routes. Default is \'/ra\'.\n\n- tags (optional): The FastAPI tags.\n\n- include_* (optional): The params to include/exclude specific route. (For example: include_create=false)\n\n### Route Endpoints\nThe following routes are automatically generated by the `ReactAdmin` class:\n\n- POST /ra/getList: Get a list of records from the table. Accepts JSON payload with sort, filter, and range parameters.\n- POST /ra/getOne/{id}: Get a single record by ID.\n- POST /ra/getMany/{id}: Get multiple records by ID. Accepts JSON payload with id parameter.\n- POST /ra/create: Create a new record. Accepts JSON payload with the record data.\n- POST /ra/update/{id}: Update a record by ID. Accepts JSON payload with the updated data.\n- POST /ra/updateMany: Update multiple records. Accepts JSON payload with id parameter and updated data.\n- POST /ra/delete/{id}: Delete a record by ID.\n- POST /ra/deleteMany: Delete multiple records. Accepts JSON payload with id parameter.\n\n### Response Format\nThe response format for all routes is a JSON object with a data field. The data field contains the response data.',
     'author': 'Enveloss',
     'author_email': 'None',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'None',
```

### Comparing `fastapi_react_admin-2.0.1/PKG-INFO` & `fastapi_react_admin-2.0.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fastapi-react-admin
-Version: 2.0.1
+Version: 2.0.2
 Summary: Module to automaticly generate fastapi routes for using react admin
 Author: Enveloss
 Requires-Python: >=3.9,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
```

