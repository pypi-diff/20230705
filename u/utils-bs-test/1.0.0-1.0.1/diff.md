# Comparing `tmp/utils_bs_test-1.0.0.tar.gz` & `tmp/utils_bs_test-1.0.1-py3-none-any.whl.zip`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "utils_bs_test-1.0.0.tar", last modified: Thu Jun 29 09:57:35 2023, max compression
+Zip archive data, at least v2.0 to extract, compression method=deflate
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```

