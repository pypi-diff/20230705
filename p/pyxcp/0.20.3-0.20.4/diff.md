# Comparing `tmp/pyxcp-0.20.3.tar.gz` & `tmp/pyxcp-0.20.4-cp39-cp39-win32.whl.zip`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyxcp-0.20.3.tar", last modified: Mon Mar 27 06:43:07 2023, max compression
+Zip archive data, at least v2.0 to extract, compression method=deflate
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```

