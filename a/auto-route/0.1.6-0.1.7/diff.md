# Comparing `tmp/auto_route-0.1.6.tar.gz` & `tmp/auto_route-0.1.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "auto_route-0.1.6.tar", last modified: Wed Jun  7 00:45:01 2023, max compression
+gzip compressed data, was "auto_route-0.1.7.tar", last modified: Wed Jul  5 00:38:51 2023, max compression
```

## Comparing `auto_route-0.1.6.tar` & `auto_route-0.1.7.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxrwxr-x   0 ruben     (1000) ruben     (1000)        0 2023-06-07 00:45:01.110287 auto_route-0.1.6/
--rw-rw-r--   0 ruben     (1000) ruben     (1000)    35149 2023-06-07 00:39:57.000000 auto_route-0.1.6/LICENSE
--rw-rw-r--   0 ruben     (1000) ruben     (1000)     5005 2023-06-07 00:45:01.110287 auto_route-0.1.6/PKG-INFO
--rw-rw-r--   0 ruben     (1000) ruben     (1000)     4582 2023-06-07 00:39:57.000000 auto_route-0.1.6/README.rst
-drwxrwxr-x   0 ruben     (1000) ruben     (1000)        0 2023-06-07 00:45:01.110287 auto_route-0.1.6/auto_app/
--rw-rw-r--   0 ruben     (1000) ruben     (1000)        0 2023-06-07 00:39:57.000000 auto_route-0.1.6/auto_app/__init__.py
--rw-rw-r--   0 ruben     (1000) ruben     (1000)     3725 2023-06-07 00:39:57.000000 auto_route-0.1.6/auto_app/auto_app.py
--rw-rw-r--   0 ruben     (1000) ruben     (1000)     1608 2023-06-07 00:39:57.000000 auto_route-0.1.6/auto_app/cli_auto_app.py
--rw-rw-r--   0 ruben     (1000) ruben     (1000)      779 2023-06-07 00:39:57.000000 auto_route-0.1.6/auto_app/streamlit_demo.py
-drwxrwxr-x   0 ruben     (1000) ruben     (1000)        0 2023-06-07 00:45:01.110287 auto_route-0.1.6/auto_route/
--rw-rw-r--   0 ruben     (1000) ruben     (1000)        0 2023-06-07 00:39:57.000000 auto_route-0.1.6/auto_route/__init__.py
--rw-rw-r--   0 ruben     (1000) ruben     (1000)     7067 2023-06-07 00:39:57.000000 auto_route-0.1.6/auto_route/auto_route.py
--rw-rw-r--   0 ruben     (1000) ruben     (1000)     2657 2023-06-07 00:39:57.000000 auto_route-0.1.6/auto_route/create_composed_class.py
--rw-rw-r--   0 ruben     (1000) ruben     (1000)      349 2023-05-21 20:56:14.000000 auto_route-0.1.6/auto_route/generator.py
-drwxrwxr-x   0 ruben     (1000) ruben     (1000)        0 2023-06-07 00:45:01.110287 auto_route-0.1.6/auto_route.egg-info/
--rw-rw-r--   0 ruben     (1000) ruben     (1000)     5005 2023-06-07 00:45:01.000000 auto_route-0.1.6/auto_route.egg-info/PKG-INFO
--rw-rw-r--   0 ruben     (1000) ruben     (1000)      398 2023-06-07 00:45:01.000000 auto_route-0.1.6/auto_route.egg-info/SOURCES.txt
--rw-rw-r--   0 ruben     (1000) ruben     (1000)        1 2023-06-07 00:45:01.000000 auto_route-0.1.6/auto_route.egg-info/dependency_links.txt
--rw-rw-r--   0 ruben     (1000) ruben     (1000)       25 2023-06-07 00:45:01.000000 auto_route-0.1.6/auto_route.egg-info/requires.txt
--rw-rw-r--   0 ruben     (1000) ruben     (1000)       20 2023-06-07 00:45:01.000000 auto_route-0.1.6/auto_route.egg-info/top_level.txt
--rw-rw-r--   0 ruben     (1000) ruben     (1000)       38 2023-06-07 00:45:01.110287 auto_route-0.1.6/setup.cfg
--rw-rw-r--   0 ruben     (1000) ruben     (1000)      696 2023-06-07 00:44:58.000000 auto_route-0.1.6/setup.py
+drwxrwxr-x   0 ruben     (1000) ruben     (1000)        0 2023-07-05 00:38:51.775855 auto_route-0.1.7/
+-rw-rw-r--   0 ruben     (1000) ruben     (1000)    35149 2023-06-07 00:39:57.000000 auto_route-0.1.7/LICENSE
+-rw-rw-r--   0 ruben     (1000) ruben     (1000)     6460 2023-07-05 00:38:51.775855 auto_route-0.1.7/PKG-INFO
+-rw-rw-r--   0 ruben     (1000) ruben     (1000)     6037 2023-07-05 00:38:04.000000 auto_route-0.1.7/README.rst
+drwxrwxr-x   0 ruben     (1000) ruben     (1000)        0 2023-07-05 00:38:51.775855 auto_route-0.1.7/auto_app/
+-rw-rw-r--   0 ruben     (1000) ruben     (1000)        0 2023-06-07 00:39:57.000000 auto_route-0.1.7/auto_app/__init__.py
+-rw-rw-r--   0 ruben     (1000) ruben     (1000)     3725 2023-06-07 00:39:57.000000 auto_route-0.1.7/auto_app/auto_app.py
+-rw-rw-r--   0 ruben     (1000) ruben     (1000)     1608 2023-06-07 00:39:57.000000 auto_route-0.1.7/auto_app/cli_auto_app.py
+-rw-rw-r--   0 ruben     (1000) ruben     (1000)      779 2023-06-07 00:39:57.000000 auto_route-0.1.7/auto_app/streamlit_demo.py
+drwxrwxr-x   0 ruben     (1000) ruben     (1000)        0 2023-07-05 00:38:51.775855 auto_route-0.1.7/auto_route/
+-rw-rw-r--   0 ruben     (1000) ruben     (1000)        0 2023-06-07 00:39:57.000000 auto_route-0.1.7/auto_route/__init__.py
+-rw-rw-r--   0 ruben     (1000) ruben     (1000)     7067 2023-06-07 00:39:57.000000 auto_route-0.1.7/auto_route/auto_route.py
+-rw-rw-r--   0 ruben     (1000) ruben     (1000)     2657 2023-06-07 00:39:57.000000 auto_route-0.1.7/auto_route/create_composed_class.py
+-rw-rw-r--   0 ruben     (1000) ruben     (1000)      349 2023-05-21 20:56:14.000000 auto_route-0.1.7/auto_route/generator.py
+drwxrwxr-x   0 ruben     (1000) ruben     (1000)        0 2023-07-05 00:38:51.775855 auto_route-0.1.7/auto_route.egg-info/
+-rw-rw-r--   0 ruben     (1000) ruben     (1000)     6460 2023-07-05 00:38:51.000000 auto_route-0.1.7/auto_route.egg-info/PKG-INFO
+-rw-rw-r--   0 ruben     (1000) ruben     (1000)      398 2023-07-05 00:38:51.000000 auto_route-0.1.7/auto_route.egg-info/SOURCES.txt
+-rw-rw-r--   0 ruben     (1000) ruben     (1000)        1 2023-07-05 00:38:51.000000 auto_route-0.1.7/auto_route.egg-info/dependency_links.txt
+-rw-rw-r--   0 ruben     (1000) ruben     (1000)       25 2023-07-05 00:38:51.000000 auto_route-0.1.7/auto_route.egg-info/requires.txt
+-rw-rw-r--   0 ruben     (1000) ruben     (1000)       20 2023-07-05 00:38:51.000000 auto_route-0.1.7/auto_route.egg-info/top_level.txt
+-rw-rw-r--   0 ruben     (1000) ruben     (1000)       38 2023-07-05 00:38:51.775855 auto_route-0.1.7/setup.cfg
+-rw-rw-r--   0 ruben     (1000) ruben     (1000)      696 2023-07-05 00:38:37.000000 auto_route-0.1.7/setup.py
```

### Comparing `auto_route-0.1.6/LICENSE` & `auto_route-0.1.7/LICENSE`

 * *Files identical despite different names*

### Comparing `auto_route-0.1.6/PKG-INFO` & `auto_route-0.1.7/README.rst`

 * *Files 20% similar despite different names*

```diff
@@ -1,17 +1,7 @@
-Metadata-Version: 2.1
-Name: auto_route
-Version: 0.1.6
-Summary: Thank you for your interest in contributing to the AutoRoute project! Our goal is to simplify and automate the creation of SaaS/PaaS solutions. We're excited to welcome you to our community.
-Home-page: https://github.com/Bucanero06/auto_route
-Author: Ruben Fernandez
-Author-email: ruben@carbonyl.org
-Description-Content-Type: text/x-rst
-License-File: LICENSE
-
 Contributing to the AutoRoute Project
 =====================================
 
 Introduction
 ------------
 
 Thank you for your interest in contributing to the AutoRoute project!
@@ -40,35 +30,83 @@
    Configuration.md <3%20-%20Exploring%20the%20Generated%20Python%20Client%20Library%20and%20Customizing%20Its%20Configuration.md>`__
 -  `Part 4 - FastAPI Application and Generated Client Library: Complete
    Guide for
    Beginners.md <4%20-%20FastAPI%20Application%20and%20Generated%20Client%20Library%3A%20Complete%20Guide%20for%20Beginners.md>`__
 -  `Dockerfile_example.md <Dockerfile_example.md>`__
 -  `how_to_improve_microservice.md <how_to_improve_microservice.md>`__
 
-**Quick Guide:**
-
-::
-
-   @auto_route
-   def get_customer_id():
-       return "customer_id"
+**Quick and Incomplete Guide:**
 
 1.  *@auto_route:*
 
     1. The **naming conversion** for functions using this wrapper is
        ``http-method_tag_*detail`` :
 
        1. *where* http_method is in
           ``[get, post, put, delete, patch, options, head, trace]``
        2. the **tag** is the name of the class that the function is in,
           e.g. ``customer``
        3. the **detail** is the name of the function, in the example
           above, the detail would be ``id``
        4. e.g.  ## Areas of Contribution
 
+    ::
+
+       api = APIAutoRouter()
+
+        class User(BaseModel):
+            id: int
+            name: str
+
+        @api.register()
+        class User_Controller:
+            @api.route()
+            def get_user_by_id(id: int):
+                return {"id": id, "name": "User"}
+
+            @api.route()
+            def post_user_by_id(user: User):
+                return {"id": user.id, "name": user.name}
+
+            @api.route()
+            def delete_user_by_id(id: int):
+                return {"id_deleted": id}
+
+
+2.  *@auto_app:*
+
+    1. **Easy Integration**
+
+    ::
+
+        # Also includes AutoApp class for auto-generating FastAPI applications
+        from auto_app import APIAutoApp
+
+        APIAutoApp(routers_list=[api.router]).run(host='localhost', port=8000)
+
+    1. **Flexible**
+
+    ::
+
+        stripe_router_config = AutoLoadRouterConfigObject(
+            module_path='Stripe/stripe_class.py',
+            router_names=['stripe_router'],
+            init_classes=[
+                InitClassObject(class_name='Customer'),
+                InitClassObject(class_name='Payment_Intent'),
+                InitClassObject(class_name='Subscriptions'),
+            ]
+        )
+
+        api_auto_app = APIAutoApp(routers_list=[stripe_router_config])
+
+        # Can accept any FastAPI app including custom ones
+        app = api_auto_app.build_app() # This is done under the hood if app obj not passed, here done explicitly for clarity
+        api_auto_app.run(host='localhost', port=8000, app=app)
+
 2.  **Documentation:** Clear, comprehensive documentation is crucial for
     any successful open-source project. Help us improve our
     documentation by creating tutorials, adding usage examples, and
     improving descriptions of features and configurations.
 
 3.  **Continuous Integration/Continuous Deployment (CI/CD):** We’re
     always aiming to improve our automated testing and deployment
@@ -80,15 +118,15 @@
     commitment to code quality. Help us achieve this by writing unit
     tests and improving our code coverage.
 
 5.  **Code Quality Checks:** We’re committed to maintaining a clean and
     readable codebase. Contribute by improving our linting processes,
     static code analysis, and enforcing our code style guidelines.
 
-6.  **Debugging AI Models:** This is an exciting part of our project. If
+6.  **Debugging Pipelines:** This is an exciting part of our project. If
     you have ideas on how to include more common issues and security
     checks, or ways to extend our debugging with user-defined checks, we
     would love to hear from you.
 
 7.  **Payment Integrations:** We currently support Stripe, but we aim to
     provide more flexibility for our users. Help us integrate other
     payment providers like PayPal, Square, or even cryptocurrencies.
```

### Comparing `auto_route-0.1.6/auto_app/auto_app.py` & `auto_route-0.1.7/auto_app/auto_app.py`

 * *Files identical despite different names*

### Comparing `auto_route-0.1.6/auto_app/cli_auto_app.py` & `auto_route-0.1.7/auto_app/cli_auto_app.py`

 * *Files identical despite different names*

### Comparing `auto_route-0.1.6/auto_app/streamlit_demo.py` & `auto_route-0.1.7/auto_app/streamlit_demo.py`

 * *Files identical despite different names*

### Comparing `auto_route-0.1.6/auto_route/auto_route.py` & `auto_route-0.1.7/auto_route/auto_route.py`

 * *Files identical despite different names*

### Comparing `auto_route-0.1.6/auto_route/create_composed_class.py` & `auto_route-0.1.7/auto_route/create_composed_class.py`

 * *Files identical despite different names*

### Comparing `auto_route-0.1.6/auto_route.egg-info/PKG-INFO` & `auto_route-0.1.7/auto_route.egg-info/PKG-INFO`

 * *Files 26% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: auto-route
-Version: 0.1.6
+Version: 0.1.7
 Summary: Thank you for your interest in contributing to the AutoRoute project! Our goal is to simplify and automate the creation of SaaS/PaaS solutions. We're excited to welcome you to our community.
 Home-page: https://github.com/Bucanero06/auto_route
 Author: Ruben Fernandez
 Author-email: ruben@carbonyl.org
 Description-Content-Type: text/x-rst
 License-File: LICENSE
 
@@ -40,35 +40,83 @@
    Configuration.md <3%20-%20Exploring%20the%20Generated%20Python%20Client%20Library%20and%20Customizing%20Its%20Configuration.md>`__
 -  `Part 4 - FastAPI Application and Generated Client Library: Complete
    Guide for
    Beginners.md <4%20-%20FastAPI%20Application%20and%20Generated%20Client%20Library%3A%20Complete%20Guide%20for%20Beginners.md>`__
 -  `Dockerfile_example.md <Dockerfile_example.md>`__
 -  `how_to_improve_microservice.md <how_to_improve_microservice.md>`__
 
-**Quick Guide:**
-
-::
-
-   @auto_route
-   def get_customer_id():
-       return "customer_id"
+**Quick and Incomplete Guide:**
 
 1.  *@auto_route:*
 
     1. The **naming conversion** for functions using this wrapper is
        ``http-method_tag_*detail`` :
 
        1. *where* http_method is in
           ``[get, post, put, delete, patch, options, head, trace]``
        2. the **tag** is the name of the class that the function is in,
           e.g. ``customer``
        3. the **detail** is the name of the function, in the example
           above, the detail would be ``id``
        4. e.g.  ## Areas of Contribution
 
+    ::
+
+       api = APIAutoRouter()
+
+        class User(BaseModel):
+            id: int
+            name: str
+
+        @api.register()
+        class User_Controller:
+            @api.route()
+            def get_user_by_id(id: int):
+                return {"id": id, "name": "User"}
+
+            @api.route()
+            def post_user_by_id(user: User):
+                return {"id": user.id, "name": user.name}
+
+            @api.route()
+            def delete_user_by_id(id: int):
+                return {"id_deleted": id}
+
+
+2.  *@auto_app:*
+
+    1. **Easy Integration**
+
+    ::
+
+        # Also includes AutoApp class for auto-generating FastAPI applications
+        from auto_app import APIAutoApp
+
+        APIAutoApp(routers_list=[api.router]).run(host='localhost', port=8000)
+
+    1. **Flexible**
+
+    ::
+
+        stripe_router_config = AutoLoadRouterConfigObject(
+            module_path='Stripe/stripe_class.py',
+            router_names=['stripe_router'],
+            init_classes=[
+                InitClassObject(class_name='Customer'),
+                InitClassObject(class_name='Payment_Intent'),
+                InitClassObject(class_name='Subscriptions'),
+            ]
+        )
+
+        api_auto_app = APIAutoApp(routers_list=[stripe_router_config])
+
+        # Can accept any FastAPI app including custom ones
+        app = api_auto_app.build_app() # This is done under the hood if app obj not passed, here done explicitly for clarity
+        api_auto_app.run(host='localhost', port=8000, app=app)
+
 2.  **Documentation:** Clear, comprehensive documentation is crucial for
     any successful open-source project. Help us improve our
     documentation by creating tutorials, adding usage examples, and
     improving descriptions of features and configurations.
 
 3.  **Continuous Integration/Continuous Deployment (CI/CD):** We’re
     always aiming to improve our automated testing and deployment
@@ -80,15 +128,15 @@
     commitment to code quality. Help us achieve this by writing unit
     tests and improving our code coverage.
 
 5.  **Code Quality Checks:** We’re committed to maintaining a clean and
     readable codebase. Contribute by improving our linting processes,
     static code analysis, and enforcing our code style guidelines.
 
-6.  **Debugging AI Models:** This is an exciting part of our project. If
+6.  **Debugging Pipelines:** This is an exciting part of our project. If
     you have ideas on how to include more common issues and security
     checks, or ways to extend our debugging with user-defined checks, we
     would love to hear from you.
 
 7.  **Payment Integrations:** We currently support Stripe, but we aim to
     provide more flexibility for our users. Help us integrate other
     payment providers like PayPal, Square, or even cryptocurrencies.
```

### Comparing `auto_route-0.1.6/setup.py` & `auto_route-0.1.7/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='auto_route',
-    version='0.1.6',  # Semantic Versioning
+    version='0.1.7',  # Semantic Versioning
     packages=["auto_route", "auto_app"],
     author='Ruben Fernandez',
     author_email='ruben@carbonyl.org',
     description="Thank you for your interest in contributing to the AutoRoute project! Our goal is to simplify and "
                 "automate the creation of SaaS/PaaS solutions. We're excited to welcome you to our community.",
     long_description=open('README.rst').read(),
     long_description_content_type='text/x-rst',
```

