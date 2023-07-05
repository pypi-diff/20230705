# Comparing `tmp/flask_validators-0.2.tar.gz` & `tmp/flask_validators-0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "flask_validators-0.2.tar", last modified: Wed Jul  5 13:34:13 2023, max compression
+gzip compressed data, was "flask_validators-0.3.tar", last modified: Wed Jul  5 13:35:23 2023, max compression
```

## Comparing `flask_validators-0.2.tar` & `flask_validators-0.3.tar`

### file list

```diff
@@ -1,29 +1,29 @@
-drwxr-xr-x   0 mikef0x   (1000) mikef0x   (1000)        0 2023-07-05 13:34:13.143343 flask_validators-0.2/
--rw-r--r--   0 mikef0x   (1000) mikef0x   (1000)     6826 2023-07-05 13:34:13.143343 flask_validators-0.2/PKG-INFO
--rw-r--r--   0 mikef0x   (1000) mikef0x   (1000)     6446 2023-07-05 13:24:53.000000 flask_validators-0.2/README.md
-drwxr-xr-x   0 mikef0x   (1000) mikef0x   (1000)        0 2023-07-05 13:34:13.143343 flask_validators-0.2/flask_validators/
--rw-r--r--   0 mikef0x   (1000) mikef0x   (1000)      241 2023-07-05 13:15:14.000000 flask_validators-0.2/flask_validators/__init__.py
-drwxr-xr-x   0 mikef0x   (1000) mikef0x   (1000)        0 2023-07-05 13:34:13.143343 flask_validators-0.2/flask_validators/controllers/
--rw-r--r--   0 mikef0x   (1000) mikef0x   (1000)        0 2023-07-04 11:49:26.000000 flask_validators-0.2/flask_validators/controllers/__init__.py
--rw-r--r--   0 mikef0x   (1000) mikef0x   (1000)      151 2023-07-04 11:51:41.000000 flask_validators-0.2/flask_validators/controllers/error_handler.py
--rw-r--r--   0 mikef0x   (1000) mikef0x   (1000)      586 2023-07-04 12:16:58.000000 flask_validators-0.2/flask_validators/controllers/validator.py
-drwxr-xr-x   0 mikef0x   (1000) mikef0x   (1000)        0 2023-07-05 13:34:13.143343 flask_validators-0.2/flask_validators/decorators/
--rw-r--r--   0 mikef0x   (1000) mikef0x   (1000)        0 2023-07-04 11:48:52.000000 flask_validators-0.2/flask_validators/decorators/__init__.py
--rw-r--r--   0 mikef0x   (1000) mikef0x   (1000)     3228 2023-07-05 13:19:21.000000 flask_validators-0.2/flask_validators/decorators/validation_decorator.py
-drwxr-xr-x   0 mikef0x   (1000) mikef0x   (1000)        0 2023-07-05 13:34:13.143343 flask_validators-0.2/flask_validators/models/
--rw-r--r--   0 mikef0x   (1000) mikef0x   (1000)        0 2023-07-04 11:49:06.000000 flask_validators-0.2/flask_validators/models/__init__.py
--rw-r--r--   0 mikef0x   (1000) mikef0x   (1000)     5102 2023-07-05 10:16:41.000000 flask_validators-0.2/flask_validators/models/fields.py
--rw-r--r--   0 mikef0x   (1000) mikef0x   (1000)     4838 2023-07-05 10:16:47.000000 flask_validators-0.2/flask_validators/models/schema.py
-drwxr-xr-x   0 mikef0x   (1000) mikef0x   (1000)        0 2023-07-05 13:34:13.143343 flask_validators-0.2/flask_validators.egg-info/
--rw-r--r--   0 mikef0x   (1000) mikef0x   (1000)     6826 2023-07-05 13:34:13.000000 flask_validators-0.2/flask_validators.egg-info/PKG-INFO
--rw-r--r--   0 mikef0x   (1000) mikef0x   (1000)      657 2023-07-05 13:34:13.000000 flask_validators-0.2/flask_validators.egg-info/SOURCES.txt
--rw-r--r--   0 mikef0x   (1000) mikef0x   (1000)        1 2023-07-05 13:34:13.000000 flask_validators-0.2/flask_validators.egg-info/dependency_links.txt
--rw-r--r--   0 mikef0x   (1000) mikef0x   (1000)        6 2023-07-05 13:34:13.000000 flask_validators-0.2/flask_validators.egg-info/requires.txt
--rw-r--r--   0 mikef0x   (1000) mikef0x   (1000)       23 2023-07-05 13:34:13.000000 flask_validators-0.2/flask_validators.egg-info/top_level.txt
--rw-r--r--   0 mikef0x   (1000) mikef0x   (1000)       38 2023-07-05 13:34:13.143343 flask_validators-0.2/setup.cfg
--rw-r--r--   0 mikef0x   (1000) mikef0x   (1000)      683 2023-07-05 13:34:00.000000 flask_validators-0.2/setup.py
-drwxr-xr-x   0 mikef0x   (1000) mikef0x   (1000)        0 2023-07-05 13:34:13.143343 flask_validators-0.2/tests/
--rw-r--r--   0 mikef0x   (1000) mikef0x   (1000)        0 2023-07-04 11:49:42.000000 flask_validators-0.2/tests/__init__.py
--rw-r--r--   0 mikef0x   (1000) mikef0x   (1000)      675 2023-07-05 13:19:02.000000 flask_validators-0.2/tests/test_flask.py
--rw-r--r--   0 mikef0x   (1000) mikef0x   (1000)      107 2023-07-04 11:59:50.000000 flask_validators-0.2/tests/test_schemas.py
--rw-r--r--   0 mikef0x   (1000) mikef0x   (1000)     3470 2023-07-05 09:52:23.000000 flask_validators-0.2/tests/test_validations.py
+drwxr-xr-x   0 mikef0x   (1000) mikef0x   (1000)        0 2023-07-05 13:35:23.661429 flask_validators-0.3/
+-rw-r--r--   0 mikef0x   (1000) mikef0x   (1000)     6742 2023-07-05 13:35:23.661429 flask_validators-0.3/PKG-INFO
+-rw-r--r--   0 mikef0x   (1000) mikef0x   (1000)     6446 2023-07-05 13:24:53.000000 flask_validators-0.3/README.md
+drwxr-xr-x   0 mikef0x   (1000) mikef0x   (1000)        0 2023-07-05 13:35:23.661429 flask_validators-0.3/flask_validators/
+-rw-r--r--   0 mikef0x   (1000) mikef0x   (1000)      241 2023-07-05 13:15:14.000000 flask_validators-0.3/flask_validators/__init__.py
+drwxr-xr-x   0 mikef0x   (1000) mikef0x   (1000)        0 2023-07-05 13:35:23.661429 flask_validators-0.3/flask_validators/controllers/
+-rw-r--r--   0 mikef0x   (1000) mikef0x   (1000)        0 2023-07-04 11:49:26.000000 flask_validators-0.3/flask_validators/controllers/__init__.py
+-rw-r--r--   0 mikef0x   (1000) mikef0x   (1000)      151 2023-07-04 11:51:41.000000 flask_validators-0.3/flask_validators/controllers/error_handler.py
+-rw-r--r--   0 mikef0x   (1000) mikef0x   (1000)      586 2023-07-04 12:16:58.000000 flask_validators-0.3/flask_validators/controllers/validator.py
+drwxr-xr-x   0 mikef0x   (1000) mikef0x   (1000)        0 2023-07-05 13:35:23.661429 flask_validators-0.3/flask_validators/decorators/
+-rw-r--r--   0 mikef0x   (1000) mikef0x   (1000)        0 2023-07-04 11:48:52.000000 flask_validators-0.3/flask_validators/decorators/__init__.py
+-rw-r--r--   0 mikef0x   (1000) mikef0x   (1000)     3228 2023-07-05 13:19:21.000000 flask_validators-0.3/flask_validators/decorators/validation_decorator.py
+drwxr-xr-x   0 mikef0x   (1000) mikef0x   (1000)        0 2023-07-05 13:35:23.661429 flask_validators-0.3/flask_validators/models/
+-rw-r--r--   0 mikef0x   (1000) mikef0x   (1000)        0 2023-07-04 11:49:06.000000 flask_validators-0.3/flask_validators/models/__init__.py
+-rw-r--r--   0 mikef0x   (1000) mikef0x   (1000)     5102 2023-07-05 10:16:41.000000 flask_validators-0.3/flask_validators/models/fields.py
+-rw-r--r--   0 mikef0x   (1000) mikef0x   (1000)     4838 2023-07-05 10:16:47.000000 flask_validators-0.3/flask_validators/models/schema.py
+drwxr-xr-x   0 mikef0x   (1000) mikef0x   (1000)        0 2023-07-05 13:35:23.661429 flask_validators-0.3/flask_validators.egg-info/
+-rw-r--r--   0 mikef0x   (1000) mikef0x   (1000)     6742 2023-07-05 13:35:23.000000 flask_validators-0.3/flask_validators.egg-info/PKG-INFO
+-rw-r--r--   0 mikef0x   (1000) mikef0x   (1000)      657 2023-07-05 13:35:23.000000 flask_validators-0.3/flask_validators.egg-info/SOURCES.txt
+-rw-r--r--   0 mikef0x   (1000) mikef0x   (1000)        1 2023-07-05 13:35:23.000000 flask_validators-0.3/flask_validators.egg-info/dependency_links.txt
+-rw-r--r--   0 mikef0x   (1000) mikef0x   (1000)        6 2023-07-05 13:35:23.000000 flask_validators-0.3/flask_validators.egg-info/requires.txt
+-rw-r--r--   0 mikef0x   (1000) mikef0x   (1000)       23 2023-07-05 13:35:23.000000 flask_validators-0.3/flask_validators.egg-info/top_level.txt
+-rw-r--r--   0 mikef0x   (1000) mikef0x   (1000)       38 2023-07-05 13:35:23.661429 flask_validators-0.3/setup.cfg
+-rw-r--r--   0 mikef0x   (1000) mikef0x   (1000)      687 2023-07-05 13:35:20.000000 flask_validators-0.3/setup.py
+drwxr-xr-x   0 mikef0x   (1000) mikef0x   (1000)        0 2023-07-05 13:35:23.661429 flask_validators-0.3/tests/
+-rw-r--r--   0 mikef0x   (1000) mikef0x   (1000)        0 2023-07-04 11:49:42.000000 flask_validators-0.3/tests/__init__.py
+-rw-r--r--   0 mikef0x   (1000) mikef0x   (1000)      675 2023-07-05 13:19:02.000000 flask_validators-0.3/tests/test_flask.py
+-rw-r--r--   0 mikef0x   (1000) mikef0x   (1000)      107 2023-07-04 11:59:50.000000 flask_validators-0.3/tests/test_schemas.py
+-rw-r--r--   0 mikef0x   (1000) mikef0x   (1000)     3470 2023-07-05 09:52:23.000000 flask_validators-0.3/tests/test_validations.py
```

### Comparing `flask_validators-0.2/PKG-INFO` & `flask_validators-0.3/flask_validators.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: flask_validators
-Version: 0.2
+Name: flask-validators
+Version: 0.3
 Summary: Flask request validation
 Author: Dimitri Zhorzholiani
 Author-email: zhorzholiani.dimitri@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: License :: OSI Approved :: MIT License
 Requires-Python: >=3.6
@@ -16,17 +16,14 @@
 
 * **Simplified Data Validation:** Flask Validator streamlines the process of validating data in Flask applications, reducing the complexity and boilerplate code.
 * **Integration with Flask Routes:** The package seamlessly integrates with Flask routes through a custom decorator, making it easy to apply validation rules to specific endpoints.
 * **Flexible Validation Schema:** Flask Validator allows you to define validation rules using a schema structure, providing a clear and organized way to specify the expected data format.
 * **Custom Validators:** You can create custom validators to extend the validation capabilities of Flask Validator, enabling you to implement complex validation logic tailored to your application's needs.
 * **Error Handling:** Flask Validator automatically generates error messages based on the defined validation rules, simplifying the process of handling validation failures and providing 
 
-<p align="center">
-  <img src="./carbon.png" alt="Size Limit CLI" width="738">
-</p>
 
 With the help of Flask Validator, you can ensure the integrity and consistency of the data submitted to your Flask endpoints, enhancing the reliability and security of your application.
 
 ## How It Works
 
 1. Flask Validator provides a custom decorator, @validate_form, which can be applied to Flask routes.
 2. The decorator takes a validation schema as its argument, defined using the Schema class and Field class from Flask Validator.
```

### Comparing `flask_validators-0.2/README.md` & `flask_validators-0.3/README.md`

 * *Files identical despite different names*

### Comparing `flask_validators-0.2/flask_validators/controllers/validator.py` & `flask_validators-0.3/flask_validators/controllers/validator.py`

 * *Files identical despite different names*

### Comparing `flask_validators-0.2/flask_validators/decorators/validation_decorator.py` & `flask_validators-0.3/flask_validators/decorators/validation_decorator.py`

 * *Files identical despite different names*

### Comparing `flask_validators-0.2/flask_validators/models/fields.py` & `flask_validators-0.3/flask_validators/models/fields.py`

 * *Files identical despite different names*

### Comparing `flask_validators-0.2/flask_validators/models/schema.py` & `flask_validators-0.3/flask_validators/models/schema.py`

 * *Files identical despite different names*

### Comparing `flask_validators-0.2/flask_validators.egg-info/PKG-INFO` & `flask_validators-0.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: flask-validators
-Version: 0.2
+Name: flask_validators
+Version: 0.3
 Summary: Flask request validation
 Author: Dimitri Zhorzholiani
 Author-email: zhorzholiani.dimitri@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: License :: OSI Approved :: MIT License
 Requires-Python: >=3.6
@@ -16,17 +16,14 @@
 
 * **Simplified Data Validation:** Flask Validator streamlines the process of validating data in Flask applications, reducing the complexity and boilerplate code.
 * **Integration with Flask Routes:** The package seamlessly integrates with Flask routes through a custom decorator, making it easy to apply validation rules to specific endpoints.
 * **Flexible Validation Schema:** Flask Validator allows you to define validation rules using a schema structure, providing a clear and organized way to specify the expected data format.
 * **Custom Validators:** You can create custom validators to extend the validation capabilities of Flask Validator, enabling you to implement complex validation logic tailored to your application's needs.
 * **Error Handling:** Flask Validator automatically generates error messages based on the defined validation rules, simplifying the process of handling validation failures and providing 
 
-<p align="center">
-  <img src="./carbon.png" alt="Size Limit CLI" width="738">
-</p>
 
 With the help of Flask Validator, you can ensure the integrity and consistency of the data submitted to your Flask endpoints, enhancing the reliability and security of your application.
 
 ## How It Works
 
 1. Flask Validator provides a custom decorator, @validate_form, which can be applied to Flask routes.
 2. The decorator takes a validation schema as its argument, defined using the Schema class and Field class from Flask Validator.
```

### Comparing `flask_validators-0.2/flask_validators.egg-info/SOURCES.txt` & `flask_validators-0.3/flask_validators.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `flask_validators-0.2/setup.py` & `flask_validators-0.3/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup, find_packages
 
-with open('README.md', 'r', encoding='utf-8') as f:
+with open('READMEPypi.md', 'r', encoding='utf-8') as f:
     long_description = f.read()
 
 setup(
     name="flask_validators",
-    version="0.2",
+    version="0.3",
     packages=find_packages(),
     description="Flask request validation",
     long_description=long_description,
     long_description_content_type='text/markdown',
     author="Dimitri Zhorzholiani",
     author_email="zhorzholiani.dimitri@gmail.com",
     classifiers=[
```

### Comparing `flask_validators-0.2/tests/test_flask.py` & `flask_validators-0.3/tests/test_flask.py`

 * *Files identical despite different names*

### Comparing `flask_validators-0.2/tests/test_validations.py` & `flask_validators-0.3/tests/test_validations.py`

 * *Files identical despite different names*

