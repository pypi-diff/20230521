# Comparing `tmp/Bonsu-3.6.1.tar.gz` & `tmp/Bonsu-3.6.2-cp310-cp310-win_amd64.whl.zip`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "Bonsu-3.6.1.tar", last modified: Sun Mar 12 10:05:37 2023, max compression
+Zip archive data, at least v2.0 to extract, compression method=deflate
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```

