# Comparing `tmp/pilmoji-2.0.2.tar.gz` & `tmp/pilmoji-2.0.3-py3-none-any.whl.zip`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pilmoji-2.0.2.tar", last modified: Sat Aug 20 17:55:32 2022, max compression
+Zip archive data, at least v2.0 to extract, compression method=deflate
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```

