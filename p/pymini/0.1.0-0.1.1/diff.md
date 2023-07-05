# Comparing `tmp/pymini-0.1.0.tar.gz` & `tmp/pymini-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pymini-0.1.0.tar", last modified: Wed Jul  5 06:29:52 2023, max compression
+gzip compressed data, was "pymini-0.1.1.tar", last modified: Wed Jul  5 06:37:15 2023, max compression
```

## Comparing `pymini-0.1.0.tar` & `pymini-0.1.1.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 alvinwan   (501) staff       (20)        0 2023-07-05 06:29:52.265503 pymini-0.1.0/
--rw-r--r--   0 alvinwan   (501) staff       (20)     1517 2022-11-24 01:24:51.000000 pymini-0.1.0/LICENSE
--rw-r--r--   0 alvinwan   (501) staff       (20)     2830 2023-07-05 06:29:52.265002 pymini-0.1.0/PKG-INFO
--rw-r--r--   0 alvinwan   (501) staff       (20)     2356 2023-07-05 06:19:38.000000 pymini-0.1.0/README.md
-drwxr-xr-x   0 alvinwan   (501) staff       (20)        0 2023-07-05 06:29:52.260608 pymini-0.1.0/pymini.egg-info/
--rw-r--r--   0 alvinwan   (501) staff       (20)     2830 2023-07-05 06:29:52.000000 pymini-0.1.0/pymini.egg-info/PKG-INFO
--rw-r--r--   0 alvinwan   (501) staff       (20)      273 2023-07-05 06:29:52.000000 pymini-0.1.0/pymini.egg-info/SOURCES.txt
--rw-r--r--   0 alvinwan   (501) staff       (20)        1 2023-07-05 06:29:52.000000 pymini-0.1.0/pymini.egg-info/dependency_links.txt
--rw-r--r--   0 alvinwan   (501) staff       (20)       43 2023-07-05 06:29:52.000000 pymini-0.1.0/pymini.egg-info/entry_points.txt
--rw-r--r--   0 alvinwan   (501) staff       (20)        7 2023-07-05 06:29:52.000000 pymini-0.1.0/pymini.egg-info/top_level.txt
--rw-r--r--   0 alvinwan   (501) staff       (20)      664 2023-07-05 06:29:13.000000 pymini-0.1.0/pyproject.toml
--rw-r--r--   0 alvinwan   (501) staff       (20)       38 2023-07-05 06:29:52.265662 pymini-0.1.0/setup.cfg
-drwxr-xr-x   0 alvinwan   (501) staff       (20)        0 2023-07-05 06:29:52.261429 pymini-0.1.0/tests/
--rw-r--r--   0 alvinwan   (501) staff       (20)      318 2023-07-02 05:22:34.000000 pymini-0.1.0/tests/test_reduction.py
-drwxr-xr-x   0 alvinwan   (501) staff       (20)        0 2023-07-05 06:29:52.264106 pymini-0.1.0/uglipy/
--rw-r--r--   0 alvinwan   (501) staff       (20)        0 2022-12-03 11:14:20.000000 pymini-0.1.0/uglipy/__init__.py
--rw-r--r--   0 alvinwan   (501) staff       (20)     1406 2023-07-05 06:08:00.000000 pymini-0.1.0/uglipy/cli.py
--rw-r--r--   0 alvinwan   (501) staff       (20)    28603 2023-07-05 06:12:58.000000 pymini-0.1.0/uglipy/ugli.py
--rw-r--r--   0 alvinwan   (501) staff       (20)     1232 2022-12-07 17:14:06.000000 pymini-0.1.0/uglipy/utils.py
+drwxr-xr-x   0 alvinwan   (501) staff       (20)        0 2023-07-05 06:37:15.939849 pymini-0.1.1/
+-rw-r--r--   0 alvinwan   (501) staff       (20)    11338 2023-07-05 06:32:55.000000 pymini-0.1.1/LICENSE
+-rw-r--r--   0 alvinwan   (501) staff       (20)     2831 2023-07-05 06:37:15.939480 pymini-0.1.1/PKG-INFO
+-rw-r--r--   0 alvinwan   (501) staff       (20)     2357 2023-07-05 06:31:12.000000 pymini-0.1.1/README.md
+drwxr-xr-x   0 alvinwan   (501) staff       (20)        0 2023-07-05 06:37:15.936157 pymini-0.1.1/pymini/
+-rw-r--r--   0 alvinwan   (501) staff       (20)        0 2022-12-03 11:14:20.000000 pymini-0.1.1/pymini/__init__.py
+-rw-r--r--   0 alvinwan   (501) staff       (20)     1463 2023-07-05 06:35:31.000000 pymini-0.1.1/pymini/cli.py
+-rw-r--r--   0 alvinwan   (501) staff       (20)    28603 2023-07-05 06:33:49.000000 pymini-0.1.1/pymini/pymini.py
+-rw-r--r--   0 alvinwan   (501) staff       (20)     1232 2022-12-07 17:14:06.000000 pymini-0.1.1/pymini/utils.py
+drwxr-xr-x   0 alvinwan   (501) staff       (20)        0 2023-07-05 06:37:15.938501 pymini-0.1.1/pymini.egg-info/
+-rw-r--r--   0 alvinwan   (501) staff       (20)     2831 2023-07-05 06:37:15.000000 pymini-0.1.1/pymini.egg-info/PKG-INFO
+-rw-r--r--   0 alvinwan   (501) staff       (20)      275 2023-07-05 06:37:15.000000 pymini-0.1.1/pymini.egg-info/SOURCES.txt
+-rw-r--r--   0 alvinwan   (501) staff       (20)        1 2023-07-05 06:37:15.000000 pymini-0.1.1/pymini.egg-info/dependency_links.txt
+-rw-r--r--   0 alvinwan   (501) staff       (20)       43 2023-07-05 06:37:15.000000 pymini-0.1.1/pymini.egg-info/entry_points.txt
+-rw-r--r--   0 alvinwan   (501) staff       (20)        7 2023-07-05 06:37:15.000000 pymini-0.1.1/pymini.egg-info/top_level.txt
+-rw-r--r--   0 alvinwan   (501) staff       (20)      664 2023-07-05 06:36:52.000000 pymini-0.1.1/pyproject.toml
+-rw-r--r--   0 alvinwan   (501) staff       (20)       38 2023-07-05 06:37:15.939957 pymini-0.1.1/setup.cfg
+drwxr-xr-x   0 alvinwan   (501) staff       (20)        0 2023-07-05 06:37:15.938939 pymini-0.1.1/tests/
+-rw-r--r--   0 alvinwan   (501) staff       (20)      320 2023-07-05 06:34:04.000000 pymini-0.1.1/tests/test_reduction.py
```

### Comparing `pymini-0.1.0/PKG-INFO` & `pymini-0.1.1/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,38 +1,38 @@
 Metadata-Version: 2.1
 Name: pymini
-Version: 0.1.0
+Version: 0.1.1
 Summary: Minify python
 Author-email: Alvin Wan <hi@alvinwan.com>
-Project-URL: Homepage, https://github.com/alvinwan/uglipy
-Project-URL: Bug Tracker, https://github.com/alvinwan/uglipy/issues
+Project-URL: Homepage, https://github.com/alvinwan/pymini
+Project-URL: Bug Tracker, https://github.com/alvinwan/pymini/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
-# ugli.py
+# pymini
 
 Python minifier. Built to operate on entire libraries, persisting and supporting minification across files.
 
 ## Installation
 
-    pip install ugli
+    pip install pymini
 
 ## Usage
 
-    uglipy [options] <file>
+    pymini [options] <file>
 
 To uglify a library, use the following options to preserve
 your ability to import and use the library's publicly-facing
 utilities.
 
-    uglipy --keep-module-names --keep-global-variables <file>
+    pymini --keep-module-names --keep-global-variables <file>
 
 ## Comparison
 
 We run comparisons against the following:
 
 - pyminify - https://github.com/dflook/python-minifier
 - pyminifier - https://github.com/liftoff/pyminifier
@@ -40,15 +40,15 @@
 
 To repeat our results, run the following to setup.
 
 ```
 pip install python-minifier
 pip install setuptools==57.5.0 && pip install pyminifier  # hack to get pyminifer to install
 pip install mnfy  # if you're running python3.4
-pip install uglipy  # ours
+pip install pymini  # ours
 ```
 
 Then, run the following to get mini'd versions of the sample file `sample/test.py`, which comes from `pyminifer`'s repository.
 
 ```
 mkdir -p out
 pyminify --rename-globals --remove-literal-statements sample/test.py > out/pyminify.py
```

### Comparing `pymini-0.1.0/README.md` & `pymini-0.1.1/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,24 +1,24 @@
-# ugli.py
+# pymini
 
 Python minifier. Built to operate on entire libraries, persisting and supporting minification across files.
 
 ## Installation
 
-    pip install ugli
+    pip install pymini
 
 ## Usage
 
-    uglipy [options] <file>
+    pymini [options] <file>
 
 To uglify a library, use the following options to preserve
 your ability to import and use the library's publicly-facing
 utilities.
 
-    uglipy --keep-module-names --keep-global-variables <file>
+    pymini --keep-module-names --keep-global-variables <file>
 
 ## Comparison
 
 We run comparisons against the following:
 
 - pyminify - https://github.com/dflook/python-minifier
 - pyminifier - https://github.com/liftoff/pyminifier
@@ -26,15 +26,15 @@
 
 To repeat our results, run the following to setup.
 
 ```
 pip install python-minifier
 pip install setuptools==57.5.0 && pip install pyminifier  # hack to get pyminifer to install
 pip install mnfy  # if you're running python3.4
-pip install uglipy  # ours
+pip install pymini  # ours
 ```
 
 Then, run the following to get mini'd versions of the sample file `sample/test.py`, which comes from `pyminifer`'s repository.
 
 ```
 mkdir -p out
 pyminify --rename-globals --remove-literal-statements sample/test.py > out/pyminify.py
```

### Comparing `pymini-0.1.0/pymini.egg-info/PKG-INFO` & `pymini-0.1.1/pymini.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,38 +1,38 @@
 Metadata-Version: 2.1
 Name: pymini
-Version: 0.1.0
+Version: 0.1.1
 Summary: Minify python
 Author-email: Alvin Wan <hi@alvinwan.com>
-Project-URL: Homepage, https://github.com/alvinwan/uglipy
-Project-URL: Bug Tracker, https://github.com/alvinwan/uglipy/issues
+Project-URL: Homepage, https://github.com/alvinwan/pymini
+Project-URL: Bug Tracker, https://github.com/alvinwan/pymini/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
-# ugli.py
+# pymini
 
 Python minifier. Built to operate on entire libraries, persisting and supporting minification across files.
 
 ## Installation
 
-    pip install ugli
+    pip install pymini
 
 ## Usage
 
-    uglipy [options] <file>
+    pymini [options] <file>
 
 To uglify a library, use the following options to preserve
 your ability to import and use the library's publicly-facing
 utilities.
 
-    uglipy --keep-module-names --keep-global-variables <file>
+    pymini --keep-module-names --keep-global-variables <file>
 
 ## Comparison
 
 We run comparisons against the following:
 
 - pyminify - https://github.com/dflook/python-minifier
 - pyminifier - https://github.com/liftoff/pyminifier
@@ -40,15 +40,15 @@
 
 To repeat our results, run the following to setup.
 
 ```
 pip install python-minifier
 pip install setuptools==57.5.0 && pip install pyminifier  # hack to get pyminifer to install
 pip install mnfy  # if you're running python3.4
-pip install uglipy  # ours
+pip install pymini  # ours
 ```
 
 Then, run the following to get mini'd versions of the sample file `sample/test.py`, which comes from `pyminifer`'s repository.
 
 ```
 mkdir -p out
 pyminify --rename-globals --remove-literal-statements sample/test.py > out/pyminify.py
```

### Comparing `pymini-0.1.0/pyproject.toml` & `pymini-0.1.1/pyproject.toml`

 * *Files 25% similar despite different names*

```diff
@@ -1,29 +1,29 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "pymini"
-version = "0.1.0"
+version = "0.1.1"
 authors = [
   { name="Alvin Wan", email="hi@alvinwan.com" },
 ]
 description = "Minify python"
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
     "Programming Language :: Python :: 3",
     "License :: OSI Approved :: MIT License",
     "Operating System :: OS Independent",
 ]
 dependencies = []
 
 [tool.setuptools.packages.find]
-include = ["uglipy"]
+include = ["pymini"]
 
 [project.scripts]
-uglipy = "uglipy.cli:main"
+pymini = "pymini.cli:main"
 
 [project.urls]
-"Homepage" = "https://github.com/alvinwan/uglipy"
-"Bug Tracker" = "https://github.com/alvinwan/uglipy/issues"
+"Homepage" = "https://github.com/alvinwan/pymini"
+"Bug Tracker" = "https://github.com/alvinwan/pymini/issues"
```

### Comparing `pymini-0.1.0/uglipy/cli.py` & `pymini-0.1.1/pymini/cli.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,34 +1,35 @@
 import glob
-import sys
 from pathlib import Path
-from uglipy.ugli import uglipy
+from pymini.pymini import minify
 from argparse import ArgumentParser
 
 def main():
     parser = ArgumentParser()
-    parser.add_argument('path', help='Path to the file or directory to uglipy')
+    parser.add_argument('path', help='Path to the file or directory to minify')
     parser.add_argument('--keep-module-names', action='store_true', help='Keep module names as they are. Useful for compressing libraries')
     parser.add_argument('--keep-global-variables', action='store_true', help='Keep global variables as they are. Useful for compressing libraries')
     parser.add_argument('--single-file', action='store_true', help='Concatenate all outputs into a single file')
     parser.add_argument('-o', '--output', help='Path to the output directory', default='./')
     args = parser.parse_args()
 
     sources, modules = [], []
     for path in glob.iglob(args.path):
         if not path.endswith('.py') or '.ugli.' in path:
             continue
         with open(path) as f:
             sources.append(f.read())
         modules.append(Path(path).stem)
-    cleaned, modules = uglipy(
+    cleaned, modules = minify(
         sources, modules, keep_module_names=args.keep_module_names,
         keep_global_variables=args.keep_global_variables,
         output_single_file=args.single_file
     )
+    output = Path(args.output)
+    output.mkdir(parents=True, exist_ok=True)
     for source, module in zip(cleaned, modules):
-        with open(Path(args.output) / f'{module}.py', 'w') as f:
+        with open(output / f'{module}.py', 'w') as f:
             f.write(source)
 
 
 if __name__ == '__main__':
     main()
```

### Comparing `pymini-0.1.0/uglipy/ugli.py` & `pymini-0.1.1/pymini/pymini.py`

 * *Files 0% similar despite different names*

```diff
@@ -690,15 +690,15 @@
                 else:
                     tokens.append(token)
                 last_token = token
             lines.append(' '.join(tokens))
         return '\n'.join(lines)
 
 
-def uglipy(sources, modules='main', keep_module_names=False,
+def minify(sources, modules='main', keep_module_names=False,
            keep_global_variables=False, output_single_file=False,):
     """Uglify source code. Simplify, minify, and obfuscate.
 
     >>> sources, modules = uglipy(['''a = 3
     ... def square(x):
     ...     return x ** 2
     ... ''', '''from main import square
```

### Comparing `pymini-0.1.0/uglipy/utils.py` & `pymini-0.1.1/pymini/utils.py`

 * *Files identical despite different names*

