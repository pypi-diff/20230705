# Comparing `tmp/stego_lsb-1.4.2.tar.gz` & `tmp/stego_lsb-1.4.3-py2.py3-none-any.whl.zip`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "stego_lsb-1.4.2.tar", last modified: Mon Jun 19 15:34:27 2023, max compression
+Zip archive data, at least v2.0 to extract, compression method=deflate
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```

