# Comparing `tmp/naneos-devices-0.3.tar.gz` & `tmp/naneos_devices-0.4-py3-none-any.whl.zip`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "naneos-devices-0.3.tar", last modified: Tue Jul  4 15:51:17 2023, max compression
+Zip archive data, at least v2.0 to extract, compression method=deflate
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```

