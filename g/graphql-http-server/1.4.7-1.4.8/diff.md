# Comparing `tmp/graphql_http_server-1.4.7.tar.gz` & `tmp/graphql_http_server-1.4.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "graphql_http_server-1.4.7.tar", last modified: Tue Jun  6 17:35:38 2023, max compression
+gzip compressed data, was "graphql_http_server-1.4.8.tar", last modified: Wed Jul  5 10:56:52 2023, max compression
```

## Comparing `graphql_http_server-1.4.7.tar` & `graphql_http_server-1.4.8.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-06 17:35:38.785602 graphql_http_server-1.4.7/
--rwxrwxrwx   0 root         (0) root         (0)     1069 2023-06-06 17:35:30.000000 graphql_http_server-1.4.7/LICENSE
--rwxrwxrwx   0 root         (0) root         (0)      149 2023-06-06 17:35:30.000000 graphql_http_server-1.4.7/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)      747 2023-06-06 17:35:38.785602 graphql_http_server-1.4.7/PKG-INFO
--rwxrwxrwx   0 root         (0) root         (0)       90 2023-06-06 17:35:30.000000 graphql_http_server-1.4.7/README.md
--rw-rw-rw-   0 root         (0) root         (0)        6 2023-06-06 17:35:38.000000 graphql_http_server-1.4.7/VERSION
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-06 17:35:38.783602 graphql_http_server-1.4.7/graphql_http_server/
--rwxrwxrwx   0 root         (0) root         (0)       71 2023-06-06 17:35:30.000000 graphql_http_server-1.4.7/graphql_http_server/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      745 2023-06-06 17:35:30.000000 graphql_http_server-1.4.7/graphql_http_server/error.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-06 17:35:38.784602 graphql_http_server-1.4.7/graphql_http_server/graphiql/
--rw-rw-rw-   0 root         (0) root         (0)     3100 2023-06-06 17:35:30.000000 graphql_http_server-1.4.7/graphql_http_server/graphiql/index.html
--rw-rw-rw-   0 root         (0) root         (0)     6574 2023-06-06 17:35:30.000000 graphql_http_server-1.4.7/graphql_http_server/helpers.py
--rwxrwxrwx   0 root         (0) root         (0)    10429 2023-06-06 17:35:30.000000 graphql_http_server-1.4.7/graphql_http_server/server.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-06 17:35:38.784602 graphql_http_server-1.4.7/graphql_http_server.egg-info/
--rw-r--r--   0 root         (0) root         (0)      747 2023-06-06 17:35:38.000000 graphql_http_server-1.4.7/graphql_http_server.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      525 2023-06-06 17:35:38.000000 graphql_http_server-1.4.7/graphql_http_server.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-06-06 17:35:38.000000 graphql_http_server-1.4.7/graphql_http_server.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      141 2023-06-06 17:35:38.000000 graphql_http_server-1.4.7/graphql_http_server.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       26 2023-06-06 17:35:38.000000 graphql_http_server-1.4.7/graphql_http_server.egg-info/top_level.txt
--rwxrwxrwx   0 root         (0) root         (0)       79 2023-06-06 17:35:38.786602 graphql_http_server-1.4.7/setup.cfg
--rwxrwxrwx   0 root         (0) root         (0)     1351 2023-06-06 17:35:30.000000 graphql_http_server-1.4.7/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-06 17:35:38.785602 graphql_http_server-1.4.7/tests/
--rwxrwxrwx   0 root         (0) root         (0)        0 2023-06-06 17:35:30.000000 graphql_http_server-1.4.7/tests/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      489 2023-06-06 17:35:30.000000 graphql_http_server-1.4.7/tests/app.py
--rwxrwxrwx   0 root         (0) root         (0)      399 2023-06-06 17:35:30.000000 graphql_http_server-1.4.7/tests/conftest.py
--rwxrwxrwx   0 root         (0) root         (0)     2211 2023-06-06 17:35:30.000000 graphql_http_server-1.4.7/tests/test_app.py
--rw-rw-rw-   0 root         (0) root         (0)     2664 2023-06-06 17:35:30.000000 graphql_http_server-1.4.7/tests/test_graphql_api.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-05 10:56:52.935595 graphql_http_server-1.4.8/
+-rwxrwxrwx   0 root         (0) root         (0)     1069 2023-07-05 10:56:45.000000 graphql_http_server-1.4.8/LICENSE
+-rwxrwxrwx   0 root         (0) root         (0)      149 2023-07-05 10:56:45.000000 graphql_http_server-1.4.8/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)      747 2023-07-05 10:56:52.935595 graphql_http_server-1.4.8/PKG-INFO
+-rwxrwxrwx   0 root         (0) root         (0)       90 2023-07-05 10:56:45.000000 graphql_http_server-1.4.8/README.md
+-rw-rw-rw-   0 root         (0) root         (0)        6 2023-07-05 10:56:52.000000 graphql_http_server-1.4.8/VERSION
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-05 10:56:52.933595 graphql_http_server-1.4.8/graphql_http_server/
+-rwxrwxrwx   0 root         (0) root         (0)       71 2023-07-05 10:56:45.000000 graphql_http_server-1.4.8/graphql_http_server/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      745 2023-07-05 10:56:45.000000 graphql_http_server-1.4.8/graphql_http_server/error.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-05 10:56:52.934595 graphql_http_server-1.4.8/graphql_http_server/graphiql/
+-rw-rw-rw-   0 root         (0) root         (0)     3100 2023-07-05 10:56:45.000000 graphql_http_server-1.4.8/graphql_http_server/graphiql/index.html
+-rw-rw-rw-   0 root         (0) root         (0)     6574 2023-07-05 10:56:45.000000 graphql_http_server-1.4.8/graphql_http_server/helpers.py
+-rwxrwxrwx   0 root         (0) root         (0)    10585 2023-07-05 10:56:45.000000 graphql_http_server-1.4.8/graphql_http_server/server.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-05 10:56:52.934595 graphql_http_server-1.4.8/graphql_http_server.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      747 2023-07-05 10:56:52.000000 graphql_http_server-1.4.8/graphql_http_server.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      525 2023-07-05 10:56:52.000000 graphql_http_server-1.4.8/graphql_http_server.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-05 10:56:52.000000 graphql_http_server-1.4.8/graphql_http_server.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      141 2023-07-05 10:56:52.000000 graphql_http_server-1.4.8/graphql_http_server.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       26 2023-07-05 10:56:52.000000 graphql_http_server-1.4.8/graphql_http_server.egg-info/top_level.txt
+-rwxrwxrwx   0 root         (0) root         (0)       79 2023-07-05 10:56:52.935595 graphql_http_server-1.4.8/setup.cfg
+-rwxrwxrwx   0 root         (0) root         (0)     1351 2023-07-05 10:56:45.000000 graphql_http_server-1.4.8/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-05 10:56:52.935595 graphql_http_server-1.4.8/tests/
+-rwxrwxrwx   0 root         (0) root         (0)        0 2023-07-05 10:56:45.000000 graphql_http_server-1.4.8/tests/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      489 2023-07-05 10:56:45.000000 graphql_http_server-1.4.8/tests/app.py
+-rwxrwxrwx   0 root         (0) root         (0)      399 2023-07-05 10:56:45.000000 graphql_http_server-1.4.8/tests/conftest.py
+-rwxrwxrwx   0 root         (0) root         (0)     2899 2023-07-05 10:56:45.000000 graphql_http_server-1.4.8/tests/test_app.py
+-rw-rw-rw-   0 root         (0) root         (0)     2664 2023-07-05 10:56:45.000000 graphql_http_server-1.4.8/tests/test_graphql_api.py
```

### Comparing `graphql_http_server-1.4.7/LICENSE` & `graphql_http_server-1.4.8/LICENSE`

 * *Files identical despite different names*

### Comparing `graphql_http_server-1.4.7/PKG-INFO` & `graphql_http_server-1.4.8/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: graphql_http_server
-Version: 1.4.7
+Version: 1.4.8
 Summary: HTTPServer for GraphQL.
 Home-page: https://gitlab.com/parob/graphql-http-server
-Download-URL: https://gitlab.com/parob/graphql-http-server/-/archive/master/graphql-http-server-v1.4.7.zip
+Download-URL: https://gitlab.com/parob/graphql-http-server/-/archive/master/graphql-http-server-v1.4.8.zip
 Author: Robert Parker
 Author-email: rob@parob.com
 License: MIT
 Keywords: GraphQL,HTTPServer,werkzeug
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
```

### Comparing `graphql_http_server-1.4.7/graphql_http_server/error.py` & `graphql_http_server-1.4.8/graphql_http_server/error.py`

 * *Files identical despite different names*

### Comparing `graphql_http_server-1.4.7/graphql_http_server/graphiql/index.html` & `graphql_http_server-1.4.8/graphql_http_server/graphiql/index.html`

 * *Files identical despite different names*

### Comparing `graphql_http_server-1.4.7/graphql_http_server/helpers.py` & `graphql_http_server-1.4.8/graphql_http_server/helpers.py`

 * *Files identical despite different names*

### Comparing `graphql_http_server-1.4.7/graphql_http_server/server.py` & `graphql_http_server-1.4.8/graphql_http_server/server.py`

 * *Files 1% similar despite different names*

```diff
@@ -196,17 +196,21 @@
                 html = open(graphiql_path, "r").read()
                 html = html.replace("DEFAULT_QUERY", default_query)
                 html = html.replace("DEFAULT_VARIABLES", default_variables)
 
                 return Response(html, content_type="text/html")
 
             if self.allow_cors:
+                allow_headers = ["Content-Type"]
+                if self.auth_enabled:
+                    allow_headers.append("Authorization")
+
                 headers = {
                     "Access-Control-Allow-Credentials": "true",
-                    "Access-Control-Allow-Headers": "Content-Type",
+                    "Access-Control-Allow-Headers": ", ".join(allow_headers),
                     "Access-Control-Allow-Methods": "GET, POST",
                 }
                 origin = request.headers.get("ORIGIN")
                 if origin:
                     headers["Access-Control-Allow-Origin"] = origin
 
                 if request_method == "options":
```

### Comparing `graphql_http_server-1.4.7/graphql_http_server.egg-info/PKG-INFO` & `graphql_http_server-1.4.8/graphql_http_server.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: graphql-http-server
-Version: 1.4.7
+Version: 1.4.8
 Summary: HTTPServer for GraphQL.
 Home-page: https://gitlab.com/parob/graphql-http-server
-Download-URL: https://gitlab.com/parob/graphql-http-server/-/archive/master/graphql-http-server-v1.4.7.zip
+Download-URL: https://gitlab.com/parob/graphql-http-server/-/archive/master/graphql-http-server-v1.4.8.zip
 Author: Robert Parker
 Author-email: rob@parob.com
 License: MIT
 Keywords: GraphQL,HTTPServer,werkzeug
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
```

### Comparing `graphql_http_server-1.4.7/graphql_http_server.egg-info/SOURCES.txt` & `graphql_http_server-1.4.8/graphql_http_server.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `graphql_http_server-1.4.7/setup.py` & `graphql_http_server-1.4.8/setup.py`

 * *Files identical despite different names*

### Comparing `graphql_http_server-1.4.7/tests/test_app.py` & `graphql_http_server-1.4.8/tests/test_app.py`

 * *Files 10% similar despite different names*

```diff
@@ -63,7 +63,29 @@
 
         time.sleep(0.5)
 
         req = request.Request("http://localhost:5000", headers={"Accept": "text/html"})
         response = request.urlopen(req).read()
 
         assert b"GraphiQL" in response
+
+    def test_dispatch_cors_allow_headers(self, schema):
+        server = GraphQLHTTPServer(schema=schema, allow_cors=True)
+
+        builder = EnvironBuilder(method="OPTIONS")
+
+        request = Request(builder.get_environ())
+        response = server.dispatch(request=request)
+
+        assert response.status_code == 200
+        assert response.headers["Access-Control-Allow-Headers"] == "Content-Type"
+
+        server.auth_enabled = True
+
+        response = server.dispatch(request=request)
+
+        assert response.status_code == 200
+        assert (
+            response.headers[
+                "Access-Control-Allow-Headers"
+            ] == "Content-Type, Authorization"
+        )
```

### Comparing `graphql_http_server-1.4.7/tests/test_graphql_api.py` & `graphql_http_server-1.4.8/tests/test_graphql_api.py`

 * *Files identical despite different names*

