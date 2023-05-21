# Comparing `tmp/aa-charlink-0.3.0.tar.gz` & `tmp/aa_charlink-0.4.0-py2.py3-none-any.whl.zip`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aa-charlink-0.3.0.tar", last modified: Sun Apr 30 13:58:52 2023, max compression
+Zip archive data, at least v2.0 to extract, compression method=deflate
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```

