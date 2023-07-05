# Comparing `tmp/india cities pincode-1.0.0.tar.gz` & `tmp/india_cities_pincode-1.0.1-py3-none-any.whl.zip`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "india cities pincode-1.0.0.tar", last modified: Wed Jul  5 18:08:51 2023, max compression
+Zip archive data, at least v2.0 to extract, compression method=deflate
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```

