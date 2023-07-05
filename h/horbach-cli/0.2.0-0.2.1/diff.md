# Comparing `tmp/horbach_cli-0.2.0.tar.gz` & `tmp/horbach_cli-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "horbach_cli-0.2.0.tar", max compression
+gzip compressed data, was "horbach_cli-0.2.1.tar", max compression
```

## Comparing `horbach_cli-0.2.0.tar` & `horbach_cli-0.2.1.tar`

### file list

```diff
@@ -1,11 +1,11 @@
--rw-r--r--   0        0        0      129 2023-07-05 07:54:06.473194 horbach_cli-0.2.0/README.md
--rw-r--r--   0        0        0     2047 2023-07-05 07:54:06.473194 horbach_cli-0.2.0/horbach_cli/README.md
--rw-r--r--   0        0        0       22 2023-07-05 07:54:07.141243 horbach_cli-0.2.0/horbach_cli/__init__.py
--rw-r--r--   0        0        0     1326 2023-07-05 07:54:06.473194 horbach_cli-0.2.0/horbach_cli/converter.py
--rw-r--r--   0        0        0      998 2023-07-05 07:54:06.473194 horbach_cli-0.2.0/horbach_cli/deduplicator.py
--rw-r--r--   0        0        0        0 2023-07-05 07:54:06.473194 horbach_cli-0.2.0/horbach_cli/libs/__init__.py
--rw-r--r--   0        0        0      309 2023-07-05 07:54:06.473194 horbach_cli-0.2.0/horbach_cli/libs/common.py
--rw-r--r--   0        0        0     1326 2023-07-05 07:54:06.473194 horbach_cli-0.2.0/horbach_cli/libs/converter.py
--rw-r--r--   0        0        0     1295 2023-07-05 07:54:06.473194 horbach_cli-0.2.0/horbach_cli/main.py
--rw-r--r--   0        0        0      919 2023-07-05 07:54:07.149244 horbach_cli-0.2.0/pyproject.toml
--rw-r--r--   0        0        0      640 1970-01-01 00:00:00.000000 horbach_cli-0.2.0/PKG-INFO
+-rw-r--r--   0        0        0      129 2023-07-05 08:24:51.683225 horbach_cli-0.2.1/README.md
+-rw-r--r--   0        0        0     2047 2023-07-05 08:24:51.683225 horbach_cli-0.2.1/horbach_cli/README.md
+-rw-r--r--   0        0        0       22 2023-07-05 08:24:52.491243 horbach_cli-0.2.1/horbach_cli/__init__.py
+-rw-r--r--   0        0        0     1326 2023-07-05 08:24:51.683225 horbach_cli-0.2.1/horbach_cli/converter.py
+-rw-r--r--   0        0        0      998 2023-07-05 08:24:51.683225 horbach_cli-0.2.1/horbach_cli/deduplicator.py
+-rw-r--r--   0        0        0        0 2023-07-05 08:24:51.683225 horbach_cli-0.2.1/horbach_cli/libs/__init__.py
+-rw-r--r--   0        0        0      309 2023-07-05 08:24:51.683225 horbach_cli-0.2.1/horbach_cli/libs/common.py
+-rw-r--r--   0        0        0      687 2023-07-05 08:24:51.683225 horbach_cli-0.2.1/horbach_cli/libs/converter.py
+-rw-r--r--   0        0        0     1295 2023-07-05 08:24:51.683225 horbach_cli-0.2.1/horbach_cli/main.py
+-rw-r--r--   0        0        0      919 2023-07-05 08:24:52.499243 horbach_cli-0.2.1/pyproject.toml
+-rw-r--r--   0        0        0      640 1970-01-01 00:00:00.000000 horbach_cli-0.2.1/PKG-INFO
```

### Comparing `horbach_cli-0.2.0/horbach_cli/README.md` & `horbach_cli-0.2.1/horbach_cli/README.md`

 * *Files identical despite different names*

### Comparing `horbach_cli-0.2.0/horbach_cli/converter.py` & `horbach_cli-0.2.1/horbach_cli/converter.py`

 * *Files identical despite different names*

### Comparing `horbach_cli-0.2.0/horbach_cli/deduplicator.py` & `horbach_cli-0.2.1/horbach_cli/deduplicator.py`

 * *Files identical despite different names*

### Comparing `horbach_cli-0.2.0/horbach_cli/libs/converter.py` & `horbach_cli-0.2.1/horbach_cli/libs/converter.py`

 * *Files 9% similar despite different names*

```diff
@@ -14,23 +14,7 @@
         logging.debug(f"Processing with {file}")
         if file.endswith(allowed_formats):
             image = Image.open(os.path.join(images_folder, file))
             if image.mode == "RGBA":
                 image = image.convert("RGB")
             images.append(image)
     images[0].save(f"{images_folder}/{pdf_file}", save_all=True, append_images=images[1:])
-
-
-def convert_images_to_pdf(images_folder: str, pdf_file: str) -> None:
-    images = []
-    allowed_formats = (".jpg", ".png", ".jpeg")
-    files = os.listdir(images_folder)
-    files.sort()
-    logging.info(f"Files in the {images_folder} -> {files}")
-    for file in files:
-        logging.debug(f"Processing with {file}")
-        if file.endswith(allowed_formats):
-            image = Image.open(os.path.join(images_folder, file))
-            if image.mode == "RGBA":
-                image = image.convert("RGB")
-            images.append(image)
-    images[0].save(f"{images_folder}/{pdf_file}", save_all=True, append_images=images[1:])
```

### Comparing `horbach_cli-0.2.0/horbach_cli/main.py` & `horbach_cli-0.2.1/horbach_cli/main.py`

 * *Files identical despite different names*

### Comparing `horbach_cli-0.2.0/pyproject.toml` & `horbach_cli-0.2.1/pyproject.toml`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "horbach-cli"
-version = "0.2.0"
+version = "0.2.1"
 description = ""
 authors = ["Andrew Horbach <andrewhorbach@gmail.com>"]
 readme = "README.md"
 packages = [{include = "horbach_cli"}]
 
 [tool.poetry.scripts]
 h-cli = "horbach_cli.main:app"
```

### Comparing `horbach_cli-0.2.0/PKG-INFO` & `horbach_cli-0.2.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: horbach-cli
-Version: 0.2.0
+Version: 0.2.1
 Summary: 
 Author: Andrew Horbach
 Author-email: andrewhorbach@gmail.com
 Requires-Python: >=3.10,<3.12
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
```

