# Comparing `tmp/opentok-3.6.0.tar.gz` & `tmp/opentok-3.6.1-py2.py3-none-any.whl.zip`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/opentok-3.6.0.tar", last modified: Wed Jun  7 11:57:44 2023, max compression
+Zip archive data, at least v2.0 to extract, compression method=deflate
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```

