# Comparing `tmp/sail-0.3.1.tar.gz` & `tmp/sail-0.5.1-py3-none-any.whl.zip`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sail-0.3.1.tar", last modified: Tue Jun 20 12:46:39 2023, max compression
+Zip archive data, at least v2.0 to extract, compression method=deflate
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```

