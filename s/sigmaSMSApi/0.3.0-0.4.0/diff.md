# Comparing `tmp/sigmaSMSApi-0.3.0.tar.gz` & `tmp/sigmaSMSApi-0.4.0-py3-none-any.whl.zip`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sigmaSMSApi-0.3.0.tar", last modified: Sun Jan 29 11:02:55 2023, max compression
+Zip archive data, at least v2.0 to extract, compression method=deflate
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```

