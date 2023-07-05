# Comparing `tmp/datawhispers-0.2.8.3.tar.gz` & `tmp/datawhispers-0.2.8.4-py2.py3-none-any.whl.zip`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "datawhispers-0.2.8.3.tar", last modified: Tue Jul  4 11:33:27 2023, max compression
+Zip archive data, at least v2.0 to extract, compression method=deflate
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```

