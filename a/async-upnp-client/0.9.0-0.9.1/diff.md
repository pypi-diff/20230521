# Comparing `tmp/async_upnp_client-0.9.0.tar.gz` & `tmp/async_upnp_client-0.9.1-py3-none-any.whl.zip`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/async_upnp_client-0.9.0.tar", last modified: Sun Mar 18 16:25:34 2018, max compression
+Zip archive data, at least v2.0 to extract, compression method=deflate
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```

