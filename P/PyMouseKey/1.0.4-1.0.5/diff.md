# Comparing `tmp/PyMouseKey-1.0.4-py3-none-any.whl.zip` & `tmp/PyMouseKey-1.0.5-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,7 +1,7 @@
-Zip file size: 5981 bytes, number of entries: 5
--rw-rw-rw-  2.0 fat    18668 b- defN 23-May-21 20:34 pymousekey/__init__.py
--rw-rw-rw-  2.0 fat      444 b- defN 23-May-21 20:49 PyMouseKey-1.0.4.dist-info/METADATA
--rw-rw-rw-  2.0 fat       92 b- defN 23-May-21 20:49 PyMouseKey-1.0.4.dist-info/WHEEL
--rw-rw-rw-  2.0 fat       11 b- defN 23-May-21 20:49 PyMouseKey-1.0.4.dist-info/top_level.txt
--rw-rw-r--  2.0 fat      389 b- defN 23-May-21 20:49 PyMouseKey-1.0.4.dist-info/RECORD
-5 files, 19604 bytes uncompressed, 5255 bytes compressed:  73.2%
+Zip file size: 5971 bytes, number of entries: 5
+-rw-rw-rw-  2.0 fat    18647 b- defN 23-May-21 21:22 pymousekey/__init__.py
+-rw-rw-rw-  2.0 fat      443 b- defN 23-May-21 21:25 PyMouseKey-1.0.5.dist-info/METADATA
+-rw-rw-rw-  2.0 fat       92 b- defN 23-May-21 21:25 PyMouseKey-1.0.5.dist-info/WHEEL
+-rw-rw-rw-  2.0 fat       11 b- defN 23-May-21 21:25 PyMouseKey-1.0.5.dist-info/top_level.txt
+-rw-rw-r--  2.0 fat      389 b- defN 23-May-21 21:25 PyMouseKey-1.0.5.dist-info/RECORD
+5 files, 19582 bytes uncompressed, 5245 bytes compressed:  73.2%
```

## zipnote {}

```diff
@@ -1,16 +1,16 @@
 Filename: pymousekey/__init__.py
 Comment: 
 
-Filename: PyMouseKey-1.0.4.dist-info/METADATA
+Filename: PyMouseKey-1.0.5.dist-info/METADATA
 Comment: 
 
-Filename: PyMouseKey-1.0.4.dist-info/WHEEL
+Filename: PyMouseKey-1.0.5.dist-info/WHEEL
 Comment: 
 
-Filename: PyMouseKey-1.0.4.dist-info/top_level.txt
+Filename: PyMouseKey-1.0.5.dist-info/top_level.txt
 Comment: 
 
-Filename: PyMouseKey-1.0.4.dist-info/RECORD
+Filename: PyMouseKey-1.0.5.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## pymousekey/__init__.py

```diff
@@ -614,10 +614,7 @@
         ctypes.windll.user32.PostMessageW(handle, WM_RBUTTONDOWN, MK_RBUTTON, lparam)
         ctypes.windll.user32.PostMessageW(handle, WM_RBUTTONUP, MK_RBUTTON, lparam)
 
     elif button == 'middle':
         ctypes.windll.user32.PostMessageW(handle, WM_NCHITTEST, 0, lparam)
         ctypes.windll.user32.PostMessageW(handle, WM_MBUTTONDOWN, MK_MBUTTON, lparam)
         ctypes.windll.user32.PostMessageW(handle, WM_MBUTTONUP, MK_MBUTTON, lparam)
-
-
-press('capslock')
```

