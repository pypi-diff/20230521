# Comparing `tmp/rapidocr_web-0.1.5-py3-none-any.whl.zip` & `tmp/rapidocr_web-0.1.6-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,15 +1,14 @@
-Zip file size: 42990 bytes, number of entries: 13
--rw-r--r--  2.0 unx       73 b- defN 23-May-14 02:33 rapidocr_web/__init__.py
--rw-r--r--  2.0 unx     2030 b- defN 23-May-14 02:33 rapidocr_web/api.py
--rw-r--r--  2.0 unx     1179 b- defN 23-May-14 02:33 rapidocr_web/ocrweb.py
--rw-r--r--  2.0 unx     3043 b- defN 23-May-14 02:33 rapidocr_web/task.py
--rw-r--r--  2.0 unx    16958 b- defN 23-May-14 02:33 rapidocr_web/static/css/favicon.ico
--rw-r--r--  2.0 unx     2065 b- defN 23-May-14 02:33 rapidocr_web/static/css/main.css
--rw-r--r--  2.0 unx    86341 b- defN 23-May-14 02:33 rapidocr_web/static/js/jquery-3.0.0.min.js
--rw-r--r--  2.0 unx     8202 b- defN 23-May-14 02:33 rapidocr_web/templates/index.html
--rw-r--r--  2.0 unx     5065 b- defN 23-May-14 02:34 rapidocr_web-0.1.5.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 23-May-14 02:34 rapidocr_web-0.1.5.dist-info/WHEEL
--rw-r--r--  2.0 unx       96 b- defN 23-May-14 02:34 rapidocr_web-0.1.5.dist-info/entry_points.txt
--rw-r--r--  2.0 unx       13 b- defN 23-May-14 02:34 rapidocr_web-0.1.5.dist-info/top_level.txt
--rw-rw-r--  2.0 unx     1101 b- defN 23-May-14 02:34 rapidocr_web-0.1.5.dist-info/RECORD
-13 files, 126258 bytes uncompressed, 41140 bytes compressed:  67.4%
+Zip file size: 41043 bytes, number of entries: 12
+-rw-r--r--  2.0 unx       73 b- defN 23-May-21 13:22 rapidocr_web/__init__.py
+-rw-r--r--  2.0 unx     1264 b- defN 23-May-21 13:22 rapidocr_web/ocrweb.py
+-rw-r--r--  2.0 unx     3043 b- defN 23-May-21 13:22 rapidocr_web/task.py
+-rw-r--r--  2.0 unx    16958 b- defN 23-May-21 13:22 rapidocr_web/static/css/favicon.ico
+-rw-r--r--  2.0 unx     2065 b- defN 23-May-21 13:22 rapidocr_web/static/css/main.css
+-rw-r--r--  2.0 unx    86341 b- defN 23-May-21 13:22 rapidocr_web/static/js/jquery-3.0.0.min.js
+-rw-r--r--  2.0 unx     8202 b- defN 23-May-21 13:22 rapidocr_web/templates/index.html
+-rw-r--r--  2.0 unx     1909 b- defN 23-May-21 13:22 rapidocr_web-0.1.6.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 23-May-21 13:22 rapidocr_web-0.1.6.dist-info/WHEEL
+-rw-r--r--  2.0 unx       59 b- defN 23-May-21 13:22 rapidocr_web-0.1.6.dist-info/entry_points.txt
+-rw-r--r--  2.0 unx       13 b- defN 23-May-21 13:22 rapidocr_web-0.1.6.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx     1025 b- defN 23-May-21 13:22 rapidocr_web-0.1.6.dist-info/RECORD
+12 files, 121044 bytes uncompressed, 39307 bytes compressed:  67.5%
```

## zipnote {}

```diff
@@ -1,13 +1,10 @@
 Filename: rapidocr_web/__init__.py
 Comment: 
 
-Filename: rapidocr_web/api.py
-Comment: 
-
 Filename: rapidocr_web/ocrweb.py
 Comment: 
 
 Filename: rapidocr_web/task.py
 Comment: 
 
 Filename: rapidocr_web/static/css/favicon.ico
@@ -18,23 +15,23 @@
 
 Filename: rapidocr_web/static/js/jquery-3.0.0.min.js
 Comment: 
 
 Filename: rapidocr_web/templates/index.html
 Comment: 
 
-Filename: rapidocr_web-0.1.5.dist-info/METADATA
+Filename: rapidocr_web-0.1.6.dist-info/METADATA
 Comment: 
 
-Filename: rapidocr_web-0.1.5.dist-info/WHEEL
+Filename: rapidocr_web-0.1.6.dist-info/WHEEL
 Comment: 
 
-Filename: rapidocr_web-0.1.5.dist-info/entry_points.txt
+Filename: rapidocr_web-0.1.6.dist-info/entry_points.txt
 Comment: 
 
-Filename: rapidocr_web-0.1.5.dist-info/top_level.txt
+Filename: rapidocr_web-0.1.6.dist-info/top_level.txt
 Comment: 
 
-Filename: rapidocr_web-0.1.5.dist-info/RECORD
+Filename: rapidocr_web-0.1.6.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## rapidocr_web/ocrweb.py

```diff
@@ -36,13 +36,14 @@
     parser = argparse.ArgumentParser('rapidocr_web')
     parser.add_argument('-ip', '--ip', type=str, default='0.0.0.0',
                         help='IP Address')
     parser.add_argument('-p', '--port', type=int, default=9003,
                         help='IP port')
     args = parser.parse_args()
 
+    print(f'Successfully launched and visit https://{args.ip}:{args.port} to view.')
     server = make_server(args.ip, args.port, app)
     server.serve_forever()
 
 
 if __name__ == '__main__':
     main()
```

## Comparing `rapidocr_web-0.1.5.dist-info/RECORD` & `rapidocr_web-0.1.6.dist-info/RECORD`

 * *Files 10% similar despite different names*

```diff
@@ -1,13 +1,12 @@
 rapidocr_web/__init__.py,sha256=JmySAOGOURKrbjdme2lVdTbDKaclr00IBKeVIa0_n30,73
-rapidocr_web/api.py,sha256=57p1b0HrWEU1UNmTmm_l9qK85wMC4ugYiUJzs9mk1-Y,2030
-rapidocr_web/ocrweb.py,sha256=Tl5a_ujmZ47WUFyHJ02u0kI--6HWGrizDlcJ9X9Nqmg,1179
+rapidocr_web/ocrweb.py,sha256=2YUp91COzzuJW5_XKwfng0-9VwtGXeRSOA3Kw_DAyfg,1264
 rapidocr_web/task.py,sha256=UVgdPds1NeZTtBnh_hjZiULUKOs_J1cU_hcQDm1Y5ts,3043
 rapidocr_web/static/css/favicon.ico,sha256=CBE1NF6iiIax8WqZVR-vPRaPTcmWjlTWsk1fzEbSd8c,16958
 rapidocr_web/static/css/main.css,sha256=2HcVvoa5oSQONnuC6IjjmBd127Jv9Y5EFJGy32nTEZk,2065
 rapidocr_web/static/js/jquery-3.0.0.min.js,sha256=JmvOoLtYsmqlsWxa7mDSLMwa6dZ9rrIdtrrVYRnDRH0,86341
 rapidocr_web/templates/index.html,sha256=xUe3Xce289Of4XTfeafPTX5JMRsOTdgv2Md5EQwxm48,8202
-rapidocr_web-0.1.5.dist-info/METADATA,sha256=m76vYV6b6n6s-rvRF-jVooEl6Gd-PDnujYX-KMEGP-0,5065
-rapidocr_web-0.1.5.dist-info/WHEEL,sha256=pkctZYzUS4AYVn6dJ-7367OJZivF2e8RA9b_ZBjif18,92
-rapidocr_web-0.1.5.dist-info/entry_points.txt,sha256=gKWhYdRif2OyYYQBX6An49Q7XaLO-nuCR2AoIp6LrS8,96
-rapidocr_web-0.1.5.dist-info/top_level.txt,sha256=dArjxF38AFvTF1Ae-mGaxBhwnETUJ4sLF_nQ93HC5A4,13
-rapidocr_web-0.1.5.dist-info/RECORD,,
+rapidocr_web-0.1.6.dist-info/METADATA,sha256=HHoTfnj004peOoL7lrdjXE7L6R2b232ujIFFU8QGxaY,1909
+rapidocr_web-0.1.6.dist-info/WHEEL,sha256=pkctZYzUS4AYVn6dJ-7367OJZivF2e8RA9b_ZBjif18,92
+rapidocr_web-0.1.6.dist-info/entry_points.txt,sha256=ivlPn9JP6ziblPQyG6N4H4cXfrJZ9FD5rvSYhnEc8cU,59
+rapidocr_web-0.1.6.dist-info/top_level.txt,sha256=dArjxF38AFvTF1Ae-mGaxBhwnETUJ4sLF_nQ93HC5A4,13
+rapidocr_web-0.1.6.dist-info/RECORD,,
```

