# Comparing `tmp/SIOTCommon-0.1.tar.gz` & `tmp/SIOTCommon-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "SIOTCommon-0.1.tar", last modified: Sun May 21 17:30:03 2023, max compression
+gzip compressed data, was "SIOTCommon-0.1.1.tar", last modified: Sun May 21 19:26:17 2023, max compression
```

## Comparing `SIOTCommon-0.1.tar` & `SIOTCommon-0.1.1.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxrwx   0        0        0        0 2023-05-21 17:30:03.287532 SIOTCommon-0.1/
--rw-rw-rw-   0        0        0      337 2023-05-21 17:30:03.286527 SIOTCommon-0.1/PKG-INFO
--rw-rw-rw-   0        0        0        0 2023-04-11 20:29:38.000000 SIOTCommon-0.1/README.txt
-drwxrwxrwx   0        0        0        0 2023-05-21 17:30:03.274526 SIOTCommon-0.1/SIOTC/
--rw-rw-rw-   0        0        0     1843 2023-04-20 13:29:33.000000 SIOTCommon-0.1/SIOTC/DatabaseLayer.py
--rw-rw-rw-   0        0        0     7546 2023-05-21 17:28:45.000000 SIOTCommon-0.1/SIOTC/Operations.py
--rw-rw-rw-   0        0        0      484 2023-04-20 13:32:21.000000 SIOTCommon-0.1/SIOTC/__init__.py
--rw-rw-rw-   0        0        0     2738 2023-05-05 13:45:10.000000 SIOTCommon-0.1/SIOTC/helperhttps.py
-drwxrwxrwx   0        0        0        0 2023-05-21 17:30:03.285526 SIOTCommon-0.1/SIOTCommon.egg-info/
--rw-rw-rw-   0        0        0      337 2023-05-21 17:30:02.000000 SIOTCommon-0.1/SIOTCommon.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      270 2023-05-21 17:30:02.000000 SIOTCommon-0.1/SIOTCommon.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-21 17:30:02.000000 SIOTCommon-0.1/SIOTCommon.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      636 2023-05-21 17:30:02.000000 SIOTCommon-0.1/SIOTCommon.egg-info/requires.txt
--rw-rw-rw-   0        0        0        6 2023-05-21 17:30:02.000000 SIOTCommon-0.1/SIOTCommon.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-05-21 17:30:03.288526 SIOTCommon-0.1/setup.cfg
--rw-rw-rw-   0        0        0      579 2023-05-21 17:29:50.000000 SIOTCommon-0.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-21 19:26:17.886474 SIOTCommon-0.1.1/
+-rw-rw-rw-   0        0        0      339 2023-05-21 19:26:17.885475 SIOTCommon-0.1.1/PKG-INFO
+-rw-rw-rw-   0        0        0        0 2023-04-11 20:29:38.000000 SIOTCommon-0.1.1/README.txt
+drwxrwxrwx   0        0        0        0 2023-05-21 19:26:17.874472 SIOTCommon-0.1.1/SIOTC/
+-rw-rw-rw-   0        0        0     1843 2023-04-20 13:29:33.000000 SIOTCommon-0.1.1/SIOTC/DatabaseLayer.py
+-rw-rw-rw-   0        0        0     7748 2023-05-21 19:25:53.000000 SIOTCommon-0.1.1/SIOTC/Operations.py
+-rw-rw-rw-   0        0        0      484 2023-04-20 13:32:21.000000 SIOTCommon-0.1.1/SIOTC/__init__.py
+-rw-rw-rw-   0        0        0     2738 2023-05-05 13:45:10.000000 SIOTCommon-0.1.1/SIOTC/helperhttps.py
+drwxrwxrwx   0        0        0        0 2023-05-21 19:26:17.883489 SIOTCommon-0.1.1/SIOTCommon.egg-info/
+-rw-rw-rw-   0        0        0      339 2023-05-21 19:26:17.000000 SIOTCommon-0.1.1/SIOTCommon.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      270 2023-05-21 19:26:17.000000 SIOTCommon-0.1.1/SIOTCommon.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-21 19:26:17.000000 SIOTCommon-0.1.1/SIOTCommon.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      636 2023-05-21 19:26:17.000000 SIOTCommon-0.1.1/SIOTCommon.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        6 2023-05-21 19:26:17.000000 SIOTCommon-0.1.1/SIOTCommon.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-05-21 19:26:17.886474 SIOTCommon-0.1.1/setup.cfg
+-rw-rw-rw-   0        0        0      581 2023-05-21 19:26:09.000000 SIOTCommon-0.1.1/setup.py
```

### Comparing `SIOTCommon-0.1/SIOTC/DatabaseLayer.py` & `SIOTCommon-0.1.1/SIOTC/DatabaseLayer.py`

 * *Files identical despite different names*

### Comparing `SIOTCommon-0.1/SIOTC/Operations.py` & `SIOTCommon-0.1.1/SIOTC/Operations.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,12 @@
 from SIOTC import DatabaseLayer
 from sqlalchemy.exc import SQLAlchemyError, IntegrityError
 from sqlalchemy.sql import select, delete
+import logging
+logger = logging.getLogger(__name__)
 dl = DatabaseLayer
 
 def executeQuery(query_func, *args, **kwargs):
     # Get a database session and the SQLAlchemy Base object
     session, base = dl.GetSession()
     try:
         # Execute the query function with the session and additional arguments as arguments
@@ -12,15 +14,15 @@
         # Print a success message to indicate that the query was successful
         print('Success')
         # Return the result
         return result
     except (SQLAlchemyError, IntegrityError, ValueError, AssertionError, TypeError, AttributeError) as e:
         # If an error occurs, rollback the session and return None
         session.rollback()
-        print(str(e))
+        logger.error(str(e))
         return None
     finally:
         # Close the session
         session.close()
 
 def GetSpecificFromColumnInTable(value, column, table):
     def queryFunc(session, base, value, column, table):
@@ -28,15 +30,16 @@
         assert value is not None, "Error: No value provided"
         # Get all rows from the specified table and column
         theTable = getattr(base.classes, table, None)
         result = session.query(theTable).filter_by(id=value).first()
         # Check if an error occurred during retrieval
         if result is None:
             print('Error: No table exists with provided values')
-            return None, 'Error: No table exists with provided values'
+            logger.error('Error: No table exists with provided values')
+            return None
         # If no error, query the row that matches the provided value
         else:
             return str(result.__dict__[column])
     return executeQuery(queryFunc, value, column, table)
 
 # Add to any table to the database. Currently checks if missing columns and database constraints
 def InsertToTable(table, values):
@@ -74,15 +77,16 @@
 def GetFromTable(table, id):
     def queryFunc(session, base, table, id):
         # Get the table model from the metadata based on the provided table name
         name = "public." + table
         tableModel = base.metadata.tables.get(name)
         # Check if the table exists in the metadata
         if tableModel is None:
-            return None, 'Error: Table not found'
+            logger.error('Error: Table not found')
+            return None
         # Ensure that an ID is provided
         assert id is not None, "Error: No ID provided"
         # Create a query to get a row with the given ID from the table
         query = select([tableModel]).where(tableModel.c.id == id)
         # Execute the query and return the result
         result = session.execute(query)
         return result.first()
@@ -107,45 +111,50 @@
     return executeQuery(queryFunc, table, id)
 
 def GetAllObjectsInModel(modelName):
     # Connect to database
     session, base = dl.GetSession()
     # If session or base is None, return error message
     if session is None or base is None:
-        return None, 'Unable to connect to the database'
+        logger.error('Unable to connect to the database')
+        return None
     try:
         # Retrieve all rows from the specified database model
         rows = session.query(dl.GetModel(modelName)).all()
         # If there are no rows, return error message
         if not rows:
-            return None, 'The list is empty'
+            logger.error('The list is empty')
+            return None
         # Return the rows
         return rows
     except (SQLAlchemyError, IntegrityError, ValueError, AssertionError, TypeError) as e:
         # If there is an error, rollback the session, print the error, and return it
         session.rollback()
         print("Error:", e)
-        return None, e
+        logger.error(e)
+        return None
     finally:
         # Close the session
         session.close()
 
 def GetAllFromTable(tableName):
     def queryFunc(session, base, tableName):
         # Construct the full table name
         realName = "public." + tableName
         # Get the table object for the specified table name
         tableObject = base.metadata.tables.get(realName)
         # Check if the table object exists
         if tableObject is None:
-            return None, 'Error: Table not found'
+            logger.error('Error: Table not found')
+            return None
         # Query the table object and return the results
         objects = session.query(tableObject).all()
         if not objects:
-            return None, 'Error: The provided table is empty'
+            logger.error('The list is empty')
+            return None
         return objects
     return executeQuery(queryFunc, tableName)
 
 def GetTable(tableName):
     def queryFunc(session, base, tableName):
         # Construct the full table name (including schema) and use it to create a table object
         realName = "public." + tableName
@@ -156,16 +165,18 @@
 
 def GetAllOfColumnFromTable(tableName, columnName):
     def queryFunc(session, base, tableName, columnName):
         realName = "public." + tableName
         # Get the Table object for the specified table name
         table = base.metadata.tables.get(realName)
         if table is None:
-            return None, 'Table "{}" does not exist'.format(tableName)
+            logger.error('Error: Table not found')
+            return None
         # Get the Column object for the specified column name
         column = table.columns.get(columnName)
         if column is None:
-            return None, 'Column "{}" does not exist in table "{}"'.format(columnName, tableName)
+            logger.error('Error: Column not found')
+            return None
         # Query the database to retrieve all values in the specified column
         result = session.query(column).all()
         return result
     return executeQuery(queryFunc, tableName, columnName)
```

### Comparing `SIOTCommon-0.1/SIOTC/helperhttps.py` & `SIOTCommon-0.1.1/SIOTC/helperhttps.py`

 * *Files identical despite different names*

### Comparing `SIOTCommon-0.1/SIOTCommon.egg-info/requires.txt` & `SIOTCommon-0.1.1/SIOTCommon.egg-info/requires.txt`

 * *Files identical despite different names*

### Comparing `SIOTCommon-0.1/setup.py` & `SIOTCommon-0.1.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup, find_packages
 
 with open('requirements.txt') as f:
     requirements = f.read().splitlines()
 
 setup(
     name='SIOTCommon',
-    version='0.1',
+    version='0.1.1',
     packages=find_packages(),
     install_requires=requirements,
     author='Anton Persson',
     author_email='Antonnilspersson@gmail.com',
     description='Common operations for sweiot microservices',
     url='https://github.com/AntonNPersson/SweIoTServices.git',
     classifiers=[
```

