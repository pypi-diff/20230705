# Comparing `tmp/starfyre-0.6.3.tar.gz` & `tmp/starfyre-0.7.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "starfyre-0.6.3.tar", max compression
+gzip compressed data, was "starfyre-0.7.0.tar", max compression
```

## Comparing `starfyre-0.6.3.tar` & `starfyre-0.7.0.tar`

### file list

```diff
@@ -1,13 +1,13 @@
--rw-r--r--   0        0        0     4382 2023-06-29 18:21:17.921291 starfyre-0.6.3/README.md
--rw-r--r--   0        0        0      454 2023-06-29 18:21:17.921291 starfyre-0.6.3/pyproject.toml
--rw-r--r--   0        0        0      949 2023-06-29 18:21:17.921291 starfyre-0.6.3/starfyre/__init__.py
--rw-r--r--   0        0        0     1637 2023-06-29 18:21:17.921291 starfyre-0.6.3/starfyre/__main__.py
--rw-r--r--   0        0        0     4539 2023-06-29 18:21:17.921291 starfyre-0.6.3/starfyre/compiler.py
--rw-r--r--   0        0        0      535 2023-06-29 18:21:17.925291 starfyre-0.6.3/starfyre/component.py
--rw-r--r--   0        0        0     3550 2023-06-29 18:21:17.925291 starfyre-0.6.3/starfyre/dom_methods.py
--rw-r--r--   0        0        0      126 2023-06-29 18:21:17.925291 starfyre-0.6.3/starfyre/global_components.py
--rw-r--r--   0        0        0        0 2023-06-29 18:21:17.925291 starfyre-0.6.3/starfyre/js/__init__.py
--rw-r--r--   0        0        0     1093 2023-06-29 18:21:17.925291 starfyre-0.6.3/starfyre/js/store.js
--rw-r--r--   0        0        0     9071 2023-06-29 18:21:17.925291 starfyre-0.6.3/starfyre/parser.py
--rw-r--r--   0        0        0     3544 2023-06-29 18:21:17.925291 starfyre-0.6.3/starfyre/transpiler.py
--rw-r--r--   0        0        0     4920 1970-01-01 00:00:00.000000 starfyre-0.6.3/PKG-INFO
+-rw-r--r--   0        0        0     4382 2023-07-05 07:48:48.829507 starfyre-0.7.0/README.md
+-rw-r--r--   0        0        0      454 2023-07-05 07:48:48.829507 starfyre-0.7.0/pyproject.toml
+-rw-r--r--   0        0        0      949 2023-07-05 07:48:48.829507 starfyre-0.7.0/starfyre/__init__.py
+-rw-r--r--   0        0        0     1981 2023-07-05 07:48:48.829507 starfyre-0.7.0/starfyre/__main__.py
+-rw-r--r--   0        0        0     4539 2023-07-05 07:48:48.829507 starfyre-0.7.0/starfyre/compiler.py
+-rw-r--r--   0        0        0      535 2023-07-05 07:48:48.829507 starfyre-0.7.0/starfyre/component.py
+-rw-r--r--   0        0        0     3550 2023-07-05 07:48:48.829507 starfyre-0.7.0/starfyre/dom_methods.py
+-rw-r--r--   0        0        0      126 2023-07-05 07:48:48.829507 starfyre-0.7.0/starfyre/global_components.py
+-rw-r--r--   0        0        0        0 2023-07-05 07:48:48.833507 starfyre-0.7.0/starfyre/js/__init__.py
+-rw-r--r--   0        0        0     1093 2023-07-05 07:48:48.833507 starfyre-0.7.0/starfyre/js/store.js
+-rw-r--r--   0        0        0     9071 2023-07-05 07:48:48.833507 starfyre-0.7.0/starfyre/parser.py
+-rw-r--r--   0        0        0     3544 2023-07-05 07:48:48.833507 starfyre-0.7.0/starfyre/transpiler.py
+-rw-r--r--   0        0        0     4920 1970-01-01 00:00:00.000000 starfyre-0.7.0/PKG-INFO
```

### Comparing `starfyre-0.6.3/README.md` & `starfyre-0.7.0/README.md`

 * *Files identical despite different names*

### Comparing `starfyre-0.6.3/starfyre/__init__.py` & `starfyre-0.7.0/starfyre/__init__.py`

 * *Files identical despite different names*

### Comparing `starfyre-0.6.3/starfyre/__main__.py` & `starfyre-0.7.0/starfyre/__main__.py`

 * *Files 13% similar despite different names*

```diff
@@ -37,25 +37,40 @@
         f.write("<script src='store.js'></script>")
         f.write(app)
 """
         )
 
 
 @click.command()
-@click.option("--path", default=".", help="Path to the project")
-@click.option("--dev", default=False, help="Start the compilation and generate the build package.")
-@click.option("--build", default=False, help="Start the build package")
-def main(path, dev, build):
-    if dev:
-        path_ = path + "/__init__.py"
-        # get absolute path
-        path = os.path.abspath(path_)
-        compile(path)
-        create_main_file(os.path.dirname(path))
+@click.option("--path", help="Path to the project")
+@click.option("--build", is_flag=True, help="Compile and build package")
+def main(path, build):
+    """
+    Command-line interface to compile and build a Starfyre project.
+
+    Args:
+
+        path (str): Path to the project directory.\n
+        build (bool): Whether to start the build package.
+    """
+    if not path:
+        click.echo(
+            "Error: Please provide a valid path using the --path flag.\nUse --help for more details")
+        return
+
+    # Convert path to absolute path
+    absolute_path = Path(path).resolve()
+
     if build:
+        # Compile and build project
+        init_file_path = absolute_path / "__init__.py"
+        compile(init_file_path.resolve())
+        create_main_file(str(absolute_path))
+
+        # Start/run project
         subprocess.run(
             [sys.executable, "-m", "build"],
             cwd=path,
             stdout=subprocess.PIPE,
             stderr=subprocess.PIPE,
         )
```

### Comparing `starfyre-0.6.3/starfyre/compiler.py` & `starfyre-0.7.0/starfyre/compiler.py`

 * *Files identical despite different names*

### Comparing `starfyre-0.6.3/starfyre/component.py` & `starfyre-0.7.0/starfyre/component.py`

 * *Files identical despite different names*

### Comparing `starfyre-0.6.3/starfyre/dom_methods.py` & `starfyre-0.7.0/starfyre/dom_methods.py`

 * *Files identical despite different names*

### Comparing `starfyre-0.6.3/starfyre/js/store.js` & `starfyre-0.7.0/starfyre/js/store.js`

 * *Files identical despite different names*

### Comparing `starfyre-0.6.3/starfyre/parser.py` & `starfyre-0.7.0/starfyre/parser.py`

 * *Files identical despite different names*

### Comparing `starfyre-0.6.3/starfyre/transpiler.py` & `starfyre-0.7.0/starfyre/transpiler.py`

 * *Files identical despite different names*

### Comparing `starfyre-0.6.3/PKG-INFO` & `starfyre-0.7.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: starfyre
-Version: 0.6.3
+Version: 0.7.0
 Summary: A Python Framework for writing Reactive web Front-Ends
 License: BSD 2.0
 Author: Sanskar Jethi
 Author-email: sansyrox@gmail.com
 Requires-Python: >=3.10,<4.0
 Classifier: License :: Other/Proprietary License
 Classifier: Programming Language :: Python :: 3
```

