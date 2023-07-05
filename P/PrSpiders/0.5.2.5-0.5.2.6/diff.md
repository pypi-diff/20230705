# Comparing `tmp/PrSpiders-0.5.2.5.tar.gz` & `tmp/PrSpiders-0.5.2.6-py3.8.egg`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "PrSpiders-0.5.2.5.tar", last modified: Thu Jun  8 09:10:06 2023, max compression
+Zip archive data, at least v2.0 to extract, compression method=deflate
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```

