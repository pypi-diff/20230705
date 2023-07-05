# Comparing `tmp/FAIRSave-0.0.6.7.tar.gz` & `tmp/FAIRSave-0.0.6.8-py3-none-any.whl.zip`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "FAIRSave-0.0.6.7.tar", last modified: Tue Jun 27 08:56:15 2023, max compression
+Zip archive data, at least v2.0 to extract, compression method=deflate
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```

