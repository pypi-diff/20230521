# Comparing `tmp/sigmaSMSApi-0.5.0-py3-none-any.whl.zip` & `tmp/sigmaSMSApi-0.5.1-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,11 +1,11 @@
-Zip file size: 4608 bytes, number of entries: 9
+Zip file size: 4623 bytes, number of entries: 9
 -rw-r--r--  2.0 unx      107 b- defN 23-May-21 09:58 sigmaSMSApi/__init__.py
 -rw-r--r--  2.0 unx      144 b- defN 23-May-21 08:20 sigmaSMSApi/exceptions.py
 -rw-r--r--  2.0 unx      785 b- defN 23-Jan-22 07:06 sigmaSMSApi/models.py
--rw-r--r--  2.0 unx     7172 b- defN 23-May-21 12:55 sigmaSMSApi/sigmasms.py
--rw-r--r--  2.0 unx     1116 b- defN 23-May-21 13:15 sigmaSMSApi-0.5.0.dist-info/LICENSE.txt
--rw-r--r--  2.0 unx      413 b- defN 23-May-21 13:15 sigmaSMSApi-0.5.0.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 23-May-21 13:15 sigmaSMSApi-0.5.0.dist-info/WHEEL
--rw-r--r--  2.0 unx       12 b- defN 23-May-21 13:15 sigmaSMSApi-0.5.0.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx      726 b- defN 23-May-21 13:15 sigmaSMSApi-0.5.0.dist-info/RECORD
-9 files, 10567 bytes uncompressed, 3352 bytes compressed:  68.3%
+-rw-r--r--  2.0 unx     7247 b- defN 23-May-21 13:30 sigmaSMSApi/sigmasms.py
+-rw-r--r--  2.0 unx     1116 b- defN 23-May-21 13:30 sigmaSMSApi-0.5.1.dist-info/LICENSE.txt
+-rw-r--r--  2.0 unx      413 b- defN 23-May-21 13:30 sigmaSMSApi-0.5.1.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 23-May-21 13:30 sigmaSMSApi-0.5.1.dist-info/WHEEL
+-rw-r--r--  2.0 unx       12 b- defN 23-May-21 13:30 sigmaSMSApi-0.5.1.dist-info/top_level.txt
+?rw-rw-r--  2.0 unx      726 b- defN 23-May-21 13:30 sigmaSMSApi-0.5.1.dist-info/RECORD
+9 files, 10642 bytes uncompressed, 3367 bytes compressed:  68.4%
```

## zipnote {}

```diff
@@ -6,23 +6,23 @@
 
 Filename: sigmaSMSApi/models.py
 Comment: 
 
 Filename: sigmaSMSApi/sigmasms.py
 Comment: 
 
-Filename: sigmaSMSApi-0.5.0.dist-info/LICENSE.txt
+Filename: sigmaSMSApi-0.5.1.dist-info/LICENSE.txt
 Comment: 
 
-Filename: sigmaSMSApi-0.5.0.dist-info/METADATA
+Filename: sigmaSMSApi-0.5.1.dist-info/METADATA
 Comment: 
 
-Filename: sigmaSMSApi-0.5.0.dist-info/WHEEL
+Filename: sigmaSMSApi-0.5.1.dist-info/WHEEL
 Comment: 
 
-Filename: sigmaSMSApi-0.5.0.dist-info/top_level.txt
+Filename: sigmaSMSApi-0.5.1.dist-info/top_level.txt
 Comment: 
 
-Filename: sigmaSMSApi-0.5.0.dist-info/RECORD
+Filename: sigmaSMSApi-0.5.1.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## sigmaSMSApi/sigmasms.py

```diff
@@ -33,15 +33,19 @@
             params['$offset'] = offset
         if limit:
             params['$limit'] = limit
         return params
 
     def _get_response(self, response) -> Response:
         content = json.loads(response.content)
+
         message = content.get('message', None)
+        if not message:
+            message = content.get('error', None)
+
         if message:
             raise SigmaSmsException(message)
         else:
             return Response(response.status_code, content)
 
     def send_sms(self, recipient: str | List[str], text: str) -> Response:
         """
```

## Comparing `sigmaSMSApi-0.5.0.dist-info/LICENSE.txt` & `sigmaSMSApi-0.5.1.dist-info/LICENSE.txt`

 * *Files identical despite different names*

## Comparing `sigmaSMSApi-0.5.0.dist-info/RECORD` & `sigmaSMSApi-0.5.1.dist-info/RECORD`

 * *Files 26% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 sigmaSMSApi/__init__.py,sha256=5brw6r2Y5B3B55S6-LDJRUFFnmcdg4vdcXEnOmI3ebc,107
 sigmaSMSApi/exceptions.py,sha256=G2Y1XAkzyiLAE_6lk62tT89GZp6my7-BfTX-yHhuONM,144
 sigmaSMSApi/models.py,sha256=DjVTt5c2Zg3l29tH4uDYGpBb560XLzBjWO0dcH4b7EE,785
-sigmaSMSApi/sigmasms.py,sha256=EjI5FxIA5GW71xurSq05VAgWWoBkw58gnjTNTrRTbGU,7172
-sigmaSMSApi-0.5.0.dist-info/LICENSE.txt,sha256=kkW5fiParWP5ArUEIcXJvGbF5686rp5SpS-mzIVa73g,1116
-sigmaSMSApi-0.5.0.dist-info/METADATA,sha256=pvD6E07Cs5WwWAmwliPw9FkJ90Oj51SllRtK0DUdjto,413
-sigmaSMSApi-0.5.0.dist-info/WHEEL,sha256=2wepM1nk4DS4eFpYrW1TTqPcoGNfHhhO_i5m4cOimbo,92
-sigmaSMSApi-0.5.0.dist-info/top_level.txt,sha256=yewa_UMLU6jrbk2WgoYXhGWdby2zJwjRJ98vu3-kiq4,12
-sigmaSMSApi-0.5.0.dist-info/RECORD,,
+sigmaSMSApi/sigmasms.py,sha256=iB6gmmanc-dmvel7QwnSNFjFhzPeaImmA2eKkwSsg-U,7247
+sigmaSMSApi-0.5.1.dist-info/LICENSE.txt,sha256=kkW5fiParWP5ArUEIcXJvGbF5686rp5SpS-mzIVa73g,1116
+sigmaSMSApi-0.5.1.dist-info/METADATA,sha256=2ybKVzjSW4StpILtHaBrDvcu1HyF_9al5q1a9ZHNx4g,413
+sigmaSMSApi-0.5.1.dist-info/WHEEL,sha256=2wepM1nk4DS4eFpYrW1TTqPcoGNfHhhO_i5m4cOimbo,92
+sigmaSMSApi-0.5.1.dist-info/top_level.txt,sha256=yewa_UMLU6jrbk2WgoYXhGWdby2zJwjRJ98vu3-kiq4,12
+sigmaSMSApi-0.5.1.dist-info/RECORD,,
```

