# Comparing `tmp/pudu-0.1.0.tar.gz` & `tmp/pudu-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pudu-0.1.0.tar", last modified: Mon Mar 20 11:07:33 2023, max compression
+gzip compressed data, was "pudu-0.2.0.tar", last modified: Wed Jul  5 21:23:20 2023, max compression
```

## Comparing `pudu-0.1.0.tar` & `pudu-0.2.0.tar`

### file list

```diff
@@ -1,20 +1,25 @@
-drwxrwxrwx   0        0        0        0 2023-03-20 11:07:33.808420 pudu-0.1.0/
--rw-rw-rw-   0        0        0     1124 2022-11-22 08:22:56.000000 pudu-0.1.0/LICENSE
--rw-rw-rw-   0        0        0      129 2022-11-04 23:37:34.000000 pudu-0.1.0/MANIFEST.in
--rw-rw-rw-   0        0        0     4196 2023-03-20 11:07:33.808916 pudu-0.1.0/PKG-INFO
--rw-rw-rw-   0        0        0     3360 2023-03-20 09:20:12.000000 pudu-0.1.0/README.md
--rw-rw-rw-   0        0        0     3399 2022-12-23 11:18:40.000000 pudu-0.1.0/README.rst
-drwxrwxrwx   0        0        0        0 2023-03-20 11:07:33.786100 pudu-0.1.0/pudu/
--rw-rw-rw-   0        0        0      137 2023-03-20 10:59:18.000000 pudu-0.1.0/pudu/__init__.py
--rw-rw-rw-   0        0        0    19446 2023-03-20 08:48:38.000000 pudu-0.1.0/pudu/pudu.py
-drwxrwxrwx   0        0        0        0 2023-03-20 11:07:33.807428 pudu-0.1.0/pudu.egg-info/
--rw-rw-rw-   0        0        0     4196 2023-03-20 11:07:33.000000 pudu-0.1.0/pudu.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      287 2023-03-20 11:07:33.000000 pudu-0.1.0/pudu.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0       51 2023-03-20 11:07:33.000000 pudu-0.1.0/pudu.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        2 2022-11-22 10:14:32.000000 pudu-0.1.0/pudu.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0       51 2023-03-20 11:07:33.000000 pudu-0.1.0/pudu.egg-info/requires.txt
--rw-rw-rw-   0        0        0        5 2023-03-20 11:07:33.000000 pudu-0.1.0/pudu.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      164 2022-02-13 18:34:42.000000 pudu-0.1.0/pyproject.toml
--rw-rw-rw-   0        0        0       54 2023-01-15 22:54:26.000000 pudu-0.1.0/requirements.txt
--rw-rw-rw-   0        0        0      449 2023-03-20 11:07:33.810404 pudu-0.1.0/setup.cfg
--rw-rw-rw-   0        0        0     1844 2023-03-20 10:58:23.000000 pudu-0.1.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-05 21:23:20.718939 pudu-0.2.0/
+-rw-rw-rw-   0        0        0     1124 2022-11-22 08:22:56.000000 pudu-0.2.0/LICENSE
+-rw-rw-rw-   0        0        0      129 2022-11-04 23:37:34.000000 pudu-0.2.0/MANIFEST.in
+-rw-rw-rw-   0        0        0     4517 2023-07-05 21:23:20.719357 pudu-0.2.0/PKG-INFO
+-rw-rw-rw-   0        0        0     3681 2023-05-17 09:45:31.000000 pudu-0.2.0/README.md
+-rw-rw-rw-   0        0        0     3721 2023-05-17 09:45:54.000000 pudu-0.2.0/README.rst
+drwxrwxrwx   0        0        0        0 2023-07-05 21:23:20.667771 pudu-0.2.0/pudu/
+-rw-rw-rw-   0        0        0      137 2023-07-05 21:23:10.000000 pudu-0.2.0/pudu/__init__.py
+-rw-rw-rw-   0        0        0     4607 2023-06-30 15:11:22.000000 pudu-0.2.0/pudu/error_handler.py
+-rw-rw-rw-   0        0        0     2817 2023-06-27 11:07:42.000000 pudu-0.2.0/pudu/masks.py
+-rw-rw-rw-   0        0        0     3790 2023-06-29 13:55:14.000000 pudu-0.2.0/pudu/perturbation.py
+-rw-rw-rw-   0        0        0    13365 2023-07-04 13:45:49.000000 pudu-0.2.0/pudu/plots.py
+-rw-rw-rw-   0        0        0    29322 2023-07-05 21:10:22.000000 pudu-0.2.0/pudu/pudu.py
+-rw-rw-rw-   0        0        0     3842 2023-06-30 07:53:45.000000 pudu-0.2.0/pudu/standards.py
+drwxrwxrwx   0        0        0        0 2023-07-05 21:23:20.716988 pudu-0.2.0/pudu.egg-info/
+-rw-rw-rw-   0        0        0     4517 2023-07-05 21:23:20.000000 pudu-0.2.0/pudu.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      376 2023-07-05 21:23:20.000000 pudu-0.2.0/pudu.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0       62 2023-07-05 21:23:20.000000 pudu-0.2.0/pudu.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        2 2022-11-22 10:14:32.000000 pudu-0.2.0/pudu.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0       62 2023-07-05 21:23:20.000000 pudu-0.2.0/pudu.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        5 2023-07-05 21:23:20.000000 pudu-0.2.0/pudu.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      164 2022-02-13 18:34:42.000000 pudu-0.2.0/pyproject.toml
+-rw-rw-rw-   0        0        0       66 2023-06-28 13:59:09.000000 pudu-0.2.0/requirements.txt
+-rw-rw-rw-   0        0        0      449 2023-07-05 21:23:20.723419 pudu-0.2.0/setup.cfg
+-rw-rw-rw-   0        0        0     1844 2023-07-05 21:21:28.000000 pudu-0.2.0/setup.py
```

### Comparing `pudu-0.1.0/LICENSE` & `pudu-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `pudu-0.1.0/PKG-INFO` & `pudu-0.2.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pudu
-Version: 0.1.0
+Version: 0.2.0
 Summary: A Python library for explainability of machine learinng algorithms in an agnostic, deterministic, and simple way.
 Home-page: https://github.com/pudu-py/pudu
 Author: pudu
 Author-email: puduhola@gmail.com
 License: MIT license
 Keywords: pudu
 Classifier: Development Status :: 2 - Pre-Alpha
@@ -62,17 +62,24 @@
 
 2. Install this library using ``conda-forge``::
 
         conda install -c conda-forge pudu
 
 3. Test it by running one of the examples in the ``docs``.
 
-4. If you find this library useful, please consider a reference or citation as:
+4. If you find this library useful, please consider a reference or citation as::
 
-        ...
+        @misc{Grau-Luque2023Pudu,
+        author = {E. Grau-Luque, I. Becerril-Romero, A. Perez-Rodriguez, M. Guc, V. Izquierdo-Roca},
+        title = {pudu},
+        year = {2023},
+        publisher = {GitHub},
+        journal = {GitHub repository},
+        howpublished = {\url{https://github.com/pudu-py/pudu}},
+        }
 
 5. Stay up-to-date by updating the library using::
 
        conda update pudu
        pip install --update pudu
 
 6. If you encounter problems when updating, try uninstalling and then re-installing::
```

### Comparing `pudu-0.1.0/README.md` & `pudu-0.2.0/README.md`

 * *Files 11% similar despite different names*

```diff
@@ -40,17 +40,24 @@
 
 2. Install this library using ``conda-forge``::
 
         conda install -c conda-forge pudu
 
 3. Test it by running one of the examples in the ``docs``.
 
-4. If you find this library useful, please consider a reference or citation as:
+4. If you find this library useful, please consider a reference or citation as::
 
-        ...
+        @misc{Grau-Luque2023Pudu,
+        author = {E. Grau-Luque, I. Becerril-Romero, A. Perez-Rodriguez, M. Guc, V. Izquierdo-Roca},
+        title = {pudu},
+        year = {2023},
+        publisher = {GitHub},
+        journal = {GitHub repository},
+        howpublished = {\url{https://github.com/pudu-py/pudu}},
+        }
 
 5. Stay up-to-date by updating the library using::
 
        conda update pudu
        pip install --update pudu
 
 6. If you encounter problems when updating, try uninstalling and then re-installing::
```

### Comparing `pudu-0.1.0/README.rst` & `pudu-0.2.0/README.rst`

 * *Files 6% similar despite different names*

```diff
@@ -55,15 +55,23 @@
 
         conda install -c conda-forge pudu
 
 3. Test it by running one of the examples in the ``docs``.
 
 4. If you find this library useful, please consider a reference or citation as:
 
-        ...
+        @misc{Grau-Luque2023Pudu,
+        author = {E. Grau-Luque, I. Becerril-Romero, A. Perez-Rodriguez, M. Guc, V. Izquierdo-Roca},
+        title = {pudu},
+        year = {2023},
+        publisher = {GitHub},
+        journal = {GitHub repository},
+        howpublished = {\url{https://github.com/pudu-py/pudu}},
+        }
+
 
 5. Stay up-to-date by updating the library using:
 
        conda update pudu
        pip install --update pudu
 
 6. If you encounter problems when updating, try uninstalling and then re-installing::
```

### Comparing `pudu-0.1.0/pudu.egg-info/PKG-INFO` & `pudu-0.2.0/pudu.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pudu
-Version: 0.1.0
+Version: 0.2.0
 Summary: A Python library for explainability of machine learinng algorithms in an agnostic, deterministic, and simple way.
 Home-page: https://github.com/pudu-py/pudu
 Author: pudu
 Author-email: puduhola@gmail.com
 License: MIT license
 Keywords: pudu
 Classifier: Development Status :: 2 - Pre-Alpha
@@ -62,17 +62,24 @@
 
 2. Install this library using ``conda-forge``::
 
         conda install -c conda-forge pudu
 
 3. Test it by running one of the examples in the ``docs``.
 
-4. If you find this library useful, please consider a reference or citation as:
+4. If you find this library useful, please consider a reference or citation as::
 
-        ...
+        @misc{Grau-Luque2023Pudu,
+        author = {E. Grau-Luque, I. Becerril-Romero, A. Perez-Rodriguez, M. Guc, V. Izquierdo-Roca},
+        title = {pudu},
+        year = {2023},
+        publisher = {GitHub},
+        journal = {GitHub repository},
+        howpublished = {\url{https://github.com/pudu-py/pudu}},
+        }
 
 5. Stay up-to-date by updating the library using::
 
        conda update pudu
        pip install --update pudu
 
 6. If you encounter problems when updating, try uninstalling and then re-installing::
```

### Comparing `pudu-0.1.0/setup.py` & `pudu-0.2.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -49,10 +49,10 @@
     keywords='pudu',
     name='pudu',
     packages=find_packages(include=['pudu', 'pudu.*']),
     setup_requires=setup_requirements,
     test_suite='tests',
     tests_require=test_requirements,
     url='https://github.com/pudu-py/pudu',
-    version='0.1.0',
+    version='0.2.0',
     zip_safe=False,
 )
```

