# Comparing `tmp/horbach_cli-0.1.6.tar.gz` & `tmp/horbach_cli-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "horbach_cli-0.1.6.tar", max compression
+gzip compressed data, was "horbach_cli-0.2.0.tar", max compression
```

## Comparing `horbach_cli-0.1.6.tar` & `horbach_cli-0.2.0.tar`

### file list

```diff
@@ -1,11 +1,11 @@
--rw-r--r--   0        0        0      129 2023-04-05 15:51:27.504830 horbach_cli-0.1.6/README.md
--rw-r--r--   0        0        0     2047 2023-04-05 15:51:27.504830 horbach_cli-0.1.6/horbach_cli/README.md
--rw-r--r--   0        0        0       22 2023-04-05 15:51:28.296837 horbach_cli-0.1.6/horbach_cli/__init__.py
--rw-r--r--   0        0        0      882 2023-04-05 15:51:27.504830 horbach_cli-0.1.6/horbach_cli/converter.py
--rw-r--r--   0        0        0      998 2023-04-05 15:51:27.504830 horbach_cli-0.1.6/horbach_cli/deduplicator.py
--rw-r--r--   0        0        0        0 2023-04-05 15:51:27.504830 horbach_cli-0.1.6/horbach_cli/libs/__init__.py
--rw-r--r--   0        0        0      309 2023-04-05 15:51:27.504830 horbach_cli-0.1.6/horbach_cli/libs/common.py
--rw-r--r--   0        0        0      687 2023-04-05 15:51:27.504830 horbach_cli-0.1.6/horbach_cli/libs/converter.py
--rw-r--r--   0        0        0     1205 2023-04-05 15:51:27.504830 horbach_cli-0.1.6/horbach_cli/main.py
--rw-r--r--   0        0        0      899 2023-04-05 15:51:28.304837 horbach_cli-0.1.6/pyproject.toml
--rw-r--r--   0        0        0      599 1970-01-01 00:00:00.000000 horbach_cli-0.1.6/PKG-INFO
+-rw-r--r--   0        0        0      129 2023-07-05 07:54:06.473194 horbach_cli-0.2.0/README.md
+-rw-r--r--   0        0        0     2047 2023-07-05 07:54:06.473194 horbach_cli-0.2.0/horbach_cli/README.md
+-rw-r--r--   0        0        0       22 2023-07-05 07:54:07.141243 horbach_cli-0.2.0/horbach_cli/__init__.py
+-rw-r--r--   0        0        0     1326 2023-07-05 07:54:06.473194 horbach_cli-0.2.0/horbach_cli/converter.py
+-rw-r--r--   0        0        0      998 2023-07-05 07:54:06.473194 horbach_cli-0.2.0/horbach_cli/deduplicator.py
+-rw-r--r--   0        0        0        0 2023-07-05 07:54:06.473194 horbach_cli-0.2.0/horbach_cli/libs/__init__.py
+-rw-r--r--   0        0        0      309 2023-07-05 07:54:06.473194 horbach_cli-0.2.0/horbach_cli/libs/common.py
+-rw-r--r--   0        0        0     1326 2023-07-05 07:54:06.473194 horbach_cli-0.2.0/horbach_cli/libs/converter.py
+-rw-r--r--   0        0        0     1295 2023-07-05 07:54:06.473194 horbach_cli-0.2.0/horbach_cli/main.py
+-rw-r--r--   0        0        0      919 2023-07-05 07:54:07.149244 horbach_cli-0.2.0/pyproject.toml
+-rw-r--r--   0        0        0      640 1970-01-01 00:00:00.000000 horbach_cli-0.2.0/PKG-INFO
```

### Comparing `horbach_cli-0.1.6/horbach_cli/README.md` & `horbach_cli-0.2.0/horbach_cli/README.md`

 * *Files identical despite different names*

### Comparing `horbach_cli-0.1.6/horbach_cli/deduplicator.py` & `horbach_cli-0.2.0/horbach_cli/deduplicator.py`

 * *Files identical despite different names*

### Comparing `horbach_cli-0.1.6/horbach_cli/libs/converter.py` & `horbach_cli-0.2.0/horbach_cli/libs/converter.py`

 * *Files 9% similar despite different names*

```diff
@@ -14,7 +14,23 @@
         logging.debug(f"Processing with {file}")
         if file.endswith(allowed_formats):
             image = Image.open(os.path.join(images_folder, file))
             if image.mode == "RGBA":
                 image = image.convert("RGB")
             images.append(image)
     images[0].save(f"{images_folder}/{pdf_file}", save_all=True, append_images=images[1:])
+
+
+def convert_images_to_pdf(images_folder: str, pdf_file: str) -> None:
+    images = []
+    allowed_formats = (".jpg", ".png", ".jpeg")
+    files = os.listdir(images_folder)
+    files.sort()
+    logging.info(f"Files in the {images_folder} -> {files}")
+    for file in files:
+        logging.debug(f"Processing with {file}")
+        if file.endswith(allowed_formats):
+            image = Image.open(os.path.join(images_folder, file))
+            if image.mode == "RGBA":
+                image = image.convert("RGB")
+            images.append(image)
+    images[0].save(f"{images_folder}/{pdf_file}", save_all=True, append_images=images[1:])
```

### Comparing `horbach_cli-0.1.6/horbach_cli/main.py` & `horbach_cli-0.2.0/horbach_cli/main.py`

 * *Files 8% similar despite different names*

```diff
@@ -18,23 +18,38 @@
         print(f":speech_balloon: h-cli Version: {version}")
         raise typer.Exit()
 
 
 @app.callback()
 def main(
     verbose: str = typer.Option(
-        "INFO", "--verbose", "-v", callback=log_lvl_callback, help=f":mag: `LOG_LEVEL` one of: {', '.join(LOG_LVL)}"
+        "INFO",
+        "--verbose",
+        "-v",
+        callback=log_lvl_callback,
+        help=f":mag: `LOG_LEVEL` one of: {', '.join(LOG_LVL)}",
     ),
     version: t.Optional[bool] = typer.Option(None, "--version", callback=version_callback, is_eager=True),
 ):
     logging.basicConfig(
-        level=verbose, format="%(message)s", datefmt="[%X]", handlers=[RichHandler(rich_tracebacks=True)]
+        level=verbose,
+        format="%(message)s",
+        datefmt="[%X]",
+        handlers=[RichHandler(rich_tracebacks=True)],
     )
 
 
-app.add_typer(converter.app, name="converter", help=":rocket: manipulates files and etc.", rich_help_panel="Hacks")
 app.add_typer(
-    deduplicator.app, name="dedub", help=":two_men_holding_hands: dedublicates something.", rich_help_panel="Hacks"
+    converter.app,
+    name="converter",
+    help=":rocket: manipulates files and etc.",
+    rich_help_panel="Hacks",
+)
+app.add_typer(
+    deduplicator.app,
+    name="dedub",
+    help=":two_men_holding_hands: dedublicates something.",
+    rich_help_panel="Hacks",
 )
 
 if __name__ == "__main__":
     app(prog_name="h-cli")
```

### Comparing `horbach_cli-0.1.6/pyproject.toml` & `horbach_cli-0.2.0/pyproject.toml`

 * *Files 5% similar despite different names*

```diff
@@ -1,23 +1,24 @@
 [tool.poetry]
 name = "horbach-cli"
-version = "0.1.6"
+version = "0.2.0"
 description = ""
 authors = ["Andrew Horbach <andrewhorbach@gmail.com>"]
 readme = "README.md"
 packages = [{include = "horbach_cli"}]
 
 [tool.poetry.scripts]
 h-cli = "horbach_cli.main:app"
 
 [tool.poetry.dependencies]
 python = ">=3.10,<3.12"
 pillow = "^9.5.0"
 difpy = "^3.0.10"
 typer = {extras = ["all"], version = "^0.7.0"}
+pymupdf = "^1.22.5"
 
 [tool.poetry.group.dev.dependencies]
 typer-cli = "^0.0.13"
 python-semantic-release = "^7.33.2"
 black = "^23.3.0"
 flake8 = "^6.0.0"
 yamllint = "^1.30.0"
```

### Comparing `horbach_cli-0.1.6/PKG-INFO` & `horbach_cli-0.2.0/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,19 +1,20 @@
 Metadata-Version: 2.1
 Name: horbach-cli
-Version: 0.1.6
+Version: 0.2.0
 Summary: 
 Author: Andrew Horbach
 Author-email: andrewhorbach@gmail.com
 Requires-Python: >=3.10,<3.12
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: difpy (>=3.0.10,<4.0.0)
 Requires-Dist: pillow (>=9.5.0,<10.0.0)
+Requires-Dist: pymupdf (>=1.22.5,<2.0.0)
 Requires-Dist: typer[all] (>=0.7.0,<0.8.0)
 Description-Content-Type: text/markdown
 
 # h-cli
 
 - [cli-documentation](./horbach_cli/README.md)
 - run in docker `docker run ghcr.io/karma-git/h-cli/h-cli:latest --help`
```

