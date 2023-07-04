# Comparing `tmp/ApiLogicServer-9.0.0.tar.gz` & `tmp/ApiLogicServer-9.1.0-py3-none-any.whl.zip`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ApiLogicServer-9.0.0.tar", last modified: Thu Jun 22 21:17:52 2023, max compression
+Zip archive data, at least v2.0 to extract, compression method=deflate
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```

