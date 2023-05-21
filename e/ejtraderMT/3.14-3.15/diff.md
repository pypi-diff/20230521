# Comparing `tmp/ejtraderMT-3.14.tar.gz` & `tmp/ejtraderMT-3.15.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ejtraderMT-3.14.tar", last modified: Sat May 20 18:00:26 2023, max compression
+gzip compressed data, was "ejtraderMT-3.15.tar", last modified: Sun May 21 06:18:16 2023, max compression
```

## Comparing `ejtraderMT-3.14.tar` & `ejtraderMT-3.15.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 18:00:26.631152 ejtraderMT-3.14/
--rw-r--r--   0 runner    (1001) docker     (123)    35128 2023-05-20 18:00:05.000000 ejtraderMT-3.14/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       64 2023-05-20 18:00:05.000000 ejtraderMT-3.14/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)    15024 2023-05-20 18:00:26.631152 ejtraderMT-3.14/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    13728 2023-05-20 18:00:05.000000 ejtraderMT-3.14/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 18:00:26.627152 ejtraderMT-3.14/ejtraderMT/
--rw-r--r--   0 runner    (1001) docker     (123)       37 2023-05-20 18:00:05.000000 ejtraderMT-3.14/ejtraderMT/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 18:00:26.631152 ejtraderMT-3.14/ejtraderMT/api/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-20 18:00:05.000000 ejtraderMT-3.14/ejtraderMT/api/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    29827 2023-05-20 18:00:05.000000 ejtraderMT-3.14/ejtraderMT/api/mql.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 18:00:26.631152 ejtraderMT-3.14/ejtraderMT.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    15024 2023-05-20 18:00:26.000000 ejtraderMT-3.14/ejtraderMT.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      306 2023-05-20 18:00:26.000000 ejtraderMT-3.14/ejtraderMT.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-20 18:00:26.000000 ejtraderMT-3.14/ejtraderMT.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      107 2023-05-20 18:00:26.000000 ejtraderMT-3.14/ejtraderMT.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       11 2023-05-20 18:00:26.000000 ejtraderMT-3.14/ejtraderMT.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      110 2023-05-20 18:00:05.000000 ejtraderMT-3.14/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)       79 2023-05-20 18:00:26.631152 ejtraderMT-3.14/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2094 2023-05-20 18:00:05.000000 ejtraderMT-3.14/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 06:18:16.615424 ejtraderMT-3.15/
+-rw-r--r--   0 runner    (1001) docker     (123)    35128 2023-05-21 06:17:56.000000 ejtraderMT-3.15/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       64 2023-05-21 06:17:56.000000 ejtraderMT-3.15/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)    15024 2023-05-21 06:18:16.615424 ejtraderMT-3.15/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    13728 2023-05-21 06:17:56.000000 ejtraderMT-3.15/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 06:18:16.615424 ejtraderMT-3.15/ejtraderMT/
+-rw-r--r--   0 runner    (1001) docker     (123)       37 2023-05-21 06:17:56.000000 ejtraderMT-3.15/ejtraderMT/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 06:18:16.615424 ejtraderMT-3.15/ejtraderMT/api/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-21 06:17:56.000000 ejtraderMT-3.15/ejtraderMT/api/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    29901 2023-05-21 06:17:56.000000 ejtraderMT-3.15/ejtraderMT/api/mql.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 06:18:16.615424 ejtraderMT-3.15/ejtraderMT.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    15024 2023-05-21 06:18:16.000000 ejtraderMT-3.15/ejtraderMT.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      306 2023-05-21 06:18:16.000000 ejtraderMT-3.15/ejtraderMT.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-21 06:18:16.000000 ejtraderMT-3.15/ejtraderMT.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      107 2023-05-21 06:18:16.000000 ejtraderMT-3.15/ejtraderMT.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       11 2023-05-21 06:18:16.000000 ejtraderMT-3.15/ejtraderMT.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      110 2023-05-21 06:17:56.000000 ejtraderMT-3.15/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       79 2023-05-21 06:18:16.615424 ejtraderMT-3.15/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2094 2023-05-21 06:17:56.000000 ejtraderMT-3.15/setup.py
```

### Comparing `ejtraderMT-3.14/LICENSE` & `ejtraderMT-3.15/LICENSE`

 * *Files identical despite different names*

### Comparing `ejtraderMT-3.14/PKG-INFO` & `ejtraderMT-3.15/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ejtraderMT
-Version: 3.14
+Version: 3.15
 Summary: Metatrader API
 Home-page: https://ejtraderMT.readthedocs.io/
 Download-URL: https://ejtrader.com
 Author: Emerson Pedroso
 Author-email: support@ejtrader.com
 License: GPL-3.0
 Project-URL: Bug Reports, https://github.com/traderpedroso/ejtraderMT/issues
```

### Comparing `ejtraderMT-3.14/README.md` & `ejtraderMT-3.15/README.md`

 * *Files identical despite different names*

### Comparing `ejtraderMT-3.14/ejtraderMT/api/mql.py` & `ejtraderMT-3.15/ejtraderMT/api/mql.py`

 * *Files 3% similar despite different names*

```diff
@@ -362,20 +362,16 @@
                 df = df.set_index("date")
                 df.index = pd.to_datetime(df.index)
             except:
                 pass
             appended_data.append(df)
             start_date += delta
         pbar.close()
-        # Your code goes here
-        if len(appended_data) > 0:
-            df = pd.concat(appended_data)
-        else:
-            logging.error("No received data, check date")
-            stop()
+
+        df = pd.concat(appended_data)
 
         if self.__database:
             start(self.__save_to_db, data=[df], repeat=1, max_threads=20)
         else:
             try:
                 self.__set_utc_or_localtime_tz_df(df)
                 self.__calendarQ.put(df)
@@ -654,74 +650,73 @@
         self.__database = database
         self.fromDate = fromDate
         self.toDate = toDate
         self.__historyQ = Queue()
         self.dataframe = dataframe
         if isinstance(symbol, tuple):
             for symbols in symbol:
-                self._symbol = symbols
-                logging.info(symbols)
+                self.__symbol = symbols
+                print(symbols)
         elif isinstance(symbol, list):
-            self._symbol = symbol
+            self.__symbol = symbol
         else:
-            self._symbol = symbol
+            self.__symbol = [symbol]
 
         if chartTF:
             if self.__database:
                 try:
                     start(self.__historyThread_save, repeat=1, max_threads=20)
                 except:
-                    logging.info("Error: unable to start History thread")
+                    print("Error: unable to start History thread")
             else:
                 try:
                     start(self.__historyThread_save, repeat=1, max_threads=20)
                 except:
-                    logging.info("Error: unable to start History thread")
+                    print("Error: unable to start History thread")
                 return self.__historyQ.get()
         else:
             q = DictSQLite("history")
             if isinstance(symbol, list):
                 try:
                     if self.dbtype == "SQLITE":
-                        df = q[f"{self._symbol[0]}"]
+                        df = q[f"{self.__symbol[0]}"]
                     else:
-                        df = self.__client.query(f"select * from {self._symbol[0]}")
-                        df = df[self._symbol[0]]
+                        df = self.__client.query(f"select * from {self.__symbol[0]}")
+                        df = df[self.__symbol[0]]
 
                         df.index.name = "date"
                 except KeyError:
-                    df = f" {self._symbol[0]}  isn't on database"
+                    df = f" {self.__symbol[0]}  isn't on database"
                     pass
             else:
                 try:
                     if self.dbtype == "SQLITE":
-                        df = q[f"{self._symbol}"]
+                        df = q[f"{self.__symbol}"]
                     else:
-                        df = self.__client.query(f"select * from {self._symbol}")
-                        df = df[self._symbol]
+                        df = self.__client.query(f"select * from {self.__symbol}")
+                        df = df[self.__symbol]
 
                         df.index.name = "date"
                 except KeyError:
-                    df = f" {self._symbol}  isn't on database"
+                    df = f" {self.__symbol}  isn't on database"
                     pass
             return df
 
     def __historyThread_save(self, data):
-        actives = self._symbol
+        actives = self.__symbol
         chartTF = self.chartTF
         fromDate = self.fromDate
         toDate = self.toDate
         main = pd.DataFrame()
         current = pd.DataFrame()
         self._count = 0
-        if self.__database:
-            try:
-                os.makedirs("DataBase")
-            except OSError:
-                pass
+        try:
+            os.makedirs("DataBase")
+        except OSError:
+            pass
         # count data
         if not isinstance(fromDate, int):
             start_date = datetime.strptime(fromDate, "%d/%m/%Y")
         else:
             start_date = self.__brokerTimeDelta(fromDate)
         if not toDate:
             end_date = self.__brokerTimeDelta(0)
@@ -736,24 +731,21 @@
         appended_data = []
         while start_date <= end_date:
             pbar.update(delta.days)
             fromDate = start_date.strftime("%d/%m/%Y")
             toDate = start_date
             toDate += delta2
             toDate = toDate.strftime("%d/%m/%Y")
-            active = None
-            # if chartTF == "TICK":
-            #     chartConvert = 60
-            # else:
-            #     chartConvert = self.__timeframe_to_sec(chartTF)
-            if isinstance(actives, list):
-                for active in actives:
-                    self._count += 1
+
+            if chartTF == "TICK":
+                chartConvert = 60
             else:
-                active = actives
+                chartConvert = self.__timeframe_to_sec(chartTF)
+            for active in actives:
+                self._count += 1
 
                 # the first symbol on list is the main and the rest will merge
                 if active == actives[0]:
                     self.__active_name = active
                     # get data
                     if fromDate and toDate:
                         data = self.__api.Command(
@@ -798,22 +790,34 @@
                                 "close",
                                 "volume",
                                 "spread",
                             ]
                     except KeyError:
                         pass
                 else:
-                    data = self.__api.Command(
-                        action="HISTORY",
-                        actionType="DATA",
-                        symbol=active,
-                        chartTF=chartTF,
-                        fromDate=self.__date_to_timestamp(fromDate),
-                        toDate=self.__date_to_timestamp(toDate),
-                    )
+                    # get data
+                    if fromDate and toDate:
+                        data = self.__api.Command(
+                            action="HISTORY",
+                            actionType="DATA",
+                            symbol=active,
+                            chartTF=chartTF,
+                            fromDate=self.__date_to_timestamp(fromDate),
+                            toDate=self.__date_to_timestamp(toDate),
+                        )
+
+                    elif isinstance(fromDate, str) and toDate == None:
+                        data = self.__api.Command(
+                            action="HISTORY",
+                            actionType="DATA",
+                            symbol=active,
+                            chartTF=chartTF,
+                            fromDate=self.__date_to_timestamp(fromDate),
+                            toDate=self.__date_to_timestamp(toDate),
+                        )
 
                     self.__api.Command(action="RESET")
                     try:
                         current = pd.DataFrame(data["data"])
                         current = current.set_index([0])
                         current.index.name = "date"
                         active = active.lower()
@@ -844,21 +848,15 @@
                         pass
 
             main = main.loc[~main.index.duplicated(keep="first")]
             appended_data.append(main)
 
             start_date += delta
         pbar.close()
-        # Your code goes here
-        if len(appended_data) > 0:
-            df = pd.concat(appended_data)
-        else:
-            logging.error("No received data, check date")
-            stop()
-
+        df = pd.concat(appended_data)
         if self.__database:
             start(self.__save_to_db, data=[df], repeat=1, max_threads=20)
         else:
             try:
                 self.__set_utc_or_localtime_tz_df(df)
                 self.__historyQ.put(df)
```

### Comparing `ejtraderMT-3.14/ejtraderMT.egg-info/PKG-INFO` & `ejtraderMT-3.15/ejtraderMT.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ejtraderMT
-Version: 3.14
+Version: 3.15
 Summary: Metatrader API
 Home-page: https://ejtraderMT.readthedocs.io/
 Download-URL: https://ejtrader.com
 Author: Emerson Pedroso
 Author-email: support@ejtrader.com
 License: GPL-3.0
 Project-URL: Bug Reports, https://github.com/traderpedroso/ejtraderMT/issues
```

### Comparing `ejtraderMT-3.14/setup.py` & `ejtraderMT-3.15/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -15,15 +15,15 @@
             reqs.append(line.strip())
     return reqs
 
 
 # Version: 3.14
 setup(
     name="ejtraderMT",
-    version="3.14",
+    version="3.15",
     packages=find_packages(),
     url="https://ejtraderMT.readthedocs.io/",
     download_url="https://ejtrader.com",
     license="GPL-3.0",
     author="Emerson Pedroso",
     author_email="support@ejtrader.com",
     description="Metatrader API",
```

