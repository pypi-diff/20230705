# Comparing `tmp/scrapy-proxycrawl-middleware-1.1.0.tar.gz` & `tmp/scrapy-proxycrawl-middleware-1.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/scrapy-proxycrawl-middleware-1.1.0.tar", last modified: Tue Jan 28 02:58:03 2020, max compression
+gzip compressed data, was "dist/scrapy-proxycrawl-middleware-1.2.0.tar", last modified: Wed Jul  5 05:21:02 2023, max compression
```

## Comparing `scrapy-proxycrawl-middleware-1.1.0.tar` & `scrapy-proxycrawl-middleware-1.2.0.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxr-xr-x   0 adria      (501) staff       (20)        0 2020-01-28 02:58:03.000000 scrapy-proxycrawl-middleware-1.1.0/
--rw-r--r--   0 adria      (501) staff       (20)     2881 2020-01-28 02:58:03.000000 scrapy-proxycrawl-middleware-1.1.0/PKG-INFO
--rw-r--r--   0 adria      (501) staff       (20)     1542 2020-01-28 02:56:08.000000 scrapy-proxycrawl-middleware-1.1.0/README.md
-drwxr-xr-x   0 adria      (501) staff       (20)        0 2020-01-28 02:58:03.000000 scrapy-proxycrawl-middleware-1.1.0/scrapy_proxycrawl/
--rw-r--r--   0 adria      (501) staff       (20)      305 2020-01-28 02:56:08.000000 scrapy-proxycrawl-middleware-1.1.0/scrapy_proxycrawl/__init__.py
--rw-r--r--   0 adria      (501) staff       (20)     2275 2020-01-28 02:56:08.000000 scrapy-proxycrawl-middleware-1.1.0/scrapy_proxycrawl/proxycrawl.py
--rw-r--r--   0 adria      (501) staff       (20)     7018 2020-01-28 02:56:08.000000 scrapy-proxycrawl-middleware-1.1.0/scrapy_proxycrawl/request.py
-drwxr-xr-x   0 adria      (501) staff       (20)        0 2020-01-28 02:58:03.000000 scrapy-proxycrawl-middleware-1.1.0/scrapy_proxycrawl_middleware.egg-info/
--rw-r--r--   0 adria      (501) staff       (20)     2881 2020-01-28 02:58:03.000000 scrapy-proxycrawl-middleware-1.1.0/scrapy_proxycrawl_middleware.egg-info/PKG-INFO
--rw-r--r--   0 adria      (501) staff       (20)      317 2020-01-28 02:58:03.000000 scrapy-proxycrawl-middleware-1.1.0/scrapy_proxycrawl_middleware.egg-info/SOURCES.txt
--rw-r--r--   0 adria      (501) staff       (20)        1 2020-01-28 02:58:03.000000 scrapy-proxycrawl-middleware-1.1.0/scrapy_proxycrawl_middleware.egg-info/dependency_links.txt
--rw-r--r--   0 adria      (501) staff       (20)       18 2020-01-28 02:58:03.000000 scrapy-proxycrawl-middleware-1.1.0/scrapy_proxycrawl_middleware.egg-info/top_level.txt
--rw-r--r--   0 adria      (501) staff       (20)       38 2020-01-28 02:58:03.000000 scrapy-proxycrawl-middleware-1.1.0/setup.cfg
--rw-r--r--   0 adria      (501) staff       (20)     1243 2020-01-28 02:56:08.000000 scrapy-proxycrawl-middleware-1.1.0/setup.py
+drwxr-xr-x   0 jamal      (501) staff       (20)        0 2023-07-05 05:21:02.000000 scrapy-proxycrawl-middleware-1.2.0/
+-rw-r--r--   0 jamal      (501) staff       (20)     3351 2023-07-05 05:21:02.000000 scrapy-proxycrawl-middleware-1.2.0/PKG-INFO
+drwxr-xr-x   0 jamal      (501) staff       (20)        0 2023-07-05 05:21:02.000000 scrapy-proxycrawl-middleware-1.2.0/scrapy_proxycrawl/
+-rw-r--r--   0 jamal      (501) staff       (20)     2275 2020-01-26 20:52:32.000000 scrapy-proxycrawl-middleware-1.2.0/scrapy_proxycrawl/proxycrawl.py
+-rw-r--r--   0 jamal      (501) staff       (20)     7018 2020-01-26 20:52:32.000000 scrapy-proxycrawl-middleware-1.2.0/scrapy_proxycrawl/request.py
+-rw-r--r--   0 jamal      (501) staff       (20)      964 2023-07-05 05:18:00.000000 scrapy-proxycrawl-middleware-1.2.0/scrapy_proxycrawl/__init__.py
+-rw-r--r--   0 jamal      (501) staff       (20)     1932 2023-07-05 05:16:52.000000 scrapy-proxycrawl-middleware-1.2.0/README.md
+-rw-r--r--   0 jamal      (501) staff       (20)     1243 2023-07-05 05:19:25.000000 scrapy-proxycrawl-middleware-1.2.0/setup.py
+-rw-r--r--   0 jamal      (501) staff       (20)       38 2023-07-05 05:21:02.000000 scrapy-proxycrawl-middleware-1.2.0/setup.cfg
+drwxr-xr-x   0 jamal      (501) staff       (20)        0 2023-07-05 05:21:02.000000 scrapy-proxycrawl-middleware-1.2.0/scrapy_proxycrawl_middleware.egg-info/
+-rw-r--r--   0 jamal      (501) staff       (20)     3351 2023-07-05 05:21:02.000000 scrapy-proxycrawl-middleware-1.2.0/scrapy_proxycrawl_middleware.egg-info/PKG-INFO
+-rw-r--r--   0 jamal      (501) staff       (20)      317 2023-07-05 05:21:02.000000 scrapy-proxycrawl-middleware-1.2.0/scrapy_proxycrawl_middleware.egg-info/SOURCES.txt
+-rw-r--r--   0 jamal      (501) staff       (20)       18 2023-07-05 05:21:02.000000 scrapy-proxycrawl-middleware-1.2.0/scrapy_proxycrawl_middleware.egg-info/top_level.txt
+-rw-r--r--   0 jamal      (501) staff       (20)        1 2023-07-05 05:21:02.000000 scrapy-proxycrawl-middleware-1.2.0/scrapy_proxycrawl_middleware.egg-info/dependency_links.txt
```

### Comparing `scrapy-proxycrawl-middleware-1.1.0/PKG-INFO` & `scrapy-proxycrawl-middleware-1.2.0/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,28 +1,35 @@
 Metadata-Version: 2.1
 Name: scrapy-proxycrawl-middleware
-Version: 1.1.0
+Version: 1.2.0
 Summary: Scrapy ProxyCrawl Proxy Middleware: ProxyCrawl interfacing middleware for Scrapy
 Home-page: https://github.com/proxycrawl/scrapy-proxycrawl-middleware
 Author: ProxyCrawl
 Author-email: info@proxycrawl.com
 License: Apache-2.0
-Description: # ProxyCrawl API middleware for Scrapy
+Description: # DEPRECATION NOTICE
         
-        Processes [Scrapy](http://scrapy.org/) requests using [ProxyCrawl](https://proxycrawl.com) services either with Normal or Javascript tokens
+        > :warning: **IMPORTANT:** This package is no longer maintained or supported. For the latest updates, please use our new package at [scrapy-crawlbase-middleware](https://github.com/crawlbase-source/scrapy-crawlbase-middleware).
+        
+        ---
         
+        # ProxyCrawl API middleware for Scrapy
+        
+        Processes [Scrapy](http://scrapy.org/) requests using [ProxyCrawl](https://proxycrawl.com) services either with Normal or Javascript tokens
         
         ## Installing
         
         Choose a way of installing:
         
         - Clone the repository inside your Scrapy project and run the following:
+        
         ```bash
         python setup.py install
         ```
+        
         - Or use [PyPi](https://pypi.org/project/scrapy-proxycrawl-middleware/) Python package manager. `pip install scrapy-proxycrawl-middleware`
         
         Then in your Scrapy `settings.py` add the following lines:
         
         ```python
         # Activate the middleware
         PROXYCRAWL_ENABLED = True
@@ -31,41 +38,44 @@
         PROXYCRAWL_TOKEN = 'your token'
         
         # Enable the middleware
         DOWNLOADER_MIDDLEWARES = {
             'scrapy_proxycrawl.ProxyCrawlMiddleware': 610
         }
         ```
+        
         ## Usage
         
         Use the scrapy_proxycrawl.ProxyCrawlRequest instead of the scrapy built-in Request.
         The scrapy_proxycrawl.ProxyCrawlRequest accepts additional arguments, used in Proxy Crawl API:
         
         ```python
         from scrapy_proxycrawl import ProxyCrawlRequest
         
-        yield ProxyCrawlRequest(
-            "http://target-url",
-            callback=self.parse_result
-            device='desktop',
-            country='US',
-            page_wait=1000,
-            ajax_wait=True,
-            dont_filter=True
-        )
+        class ExampleScraper(Spider):
+        
+            def start_requests(self):
+                yield ProxyCrawlRequest(
+                    "http://target-url",
+                    callback=self.parse_result
+                    device='desktop',
+                    country='US',
+                    page_wait=1000,
+                    ajax_wait=True,
+                    dont_filter=True
+                )
         ```
         
         The target url will be replaced with proxy crawl url and parameters will be encoded into the url by the middleware automatically.
         
-        
         If you have questions or need help using the library, please open an issue or [contact us](https://proxycrawl.com/contact).
         
         ---
         
-        Copyright 2020 ProxyCrawl
+        Copyright 2023 ProxyCrawl
         
 Keywords: scrapy middleware scraping scraper crawler crawling proxycrawl api
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 2
 Classifier: Programming Language :: Python :: 2.7
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.5
```

### Comparing `scrapy-proxycrawl-middleware-1.1.0/scrapy_proxycrawl/proxycrawl.py` & `scrapy-proxycrawl-middleware-1.2.0/scrapy_proxycrawl/proxycrawl.py`

 * *Files identical despite different names*

### Comparing `scrapy-proxycrawl-middleware-1.1.0/scrapy_proxycrawl/request.py` & `scrapy-proxycrawl-middleware-1.2.0/scrapy_proxycrawl/request.py`

 * *Files identical despite different names*

### Comparing `scrapy-proxycrawl-middleware-1.1.0/scrapy_proxycrawl_middleware.egg-info/PKG-INFO` & `scrapy-proxycrawl-middleware-1.2.0/scrapy_proxycrawl_middleware.egg-info/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,28 +1,35 @@
 Metadata-Version: 2.1
 Name: scrapy-proxycrawl-middleware
-Version: 1.1.0
+Version: 1.2.0
 Summary: Scrapy ProxyCrawl Proxy Middleware: ProxyCrawl interfacing middleware for Scrapy
 Home-page: https://github.com/proxycrawl/scrapy-proxycrawl-middleware
 Author: ProxyCrawl
 Author-email: info@proxycrawl.com
 License: Apache-2.0
-Description: # ProxyCrawl API middleware for Scrapy
+Description: # DEPRECATION NOTICE
         
-        Processes [Scrapy](http://scrapy.org/) requests using [ProxyCrawl](https://proxycrawl.com) services either with Normal or Javascript tokens
+        > :warning: **IMPORTANT:** This package is no longer maintained or supported. For the latest updates, please use our new package at [scrapy-crawlbase-middleware](https://github.com/crawlbase-source/scrapy-crawlbase-middleware).
+        
+        ---
         
+        # ProxyCrawl API middleware for Scrapy
+        
+        Processes [Scrapy](http://scrapy.org/) requests using [ProxyCrawl](https://proxycrawl.com) services either with Normal or Javascript tokens
         
         ## Installing
         
         Choose a way of installing:
         
         - Clone the repository inside your Scrapy project and run the following:
+        
         ```bash
         python setup.py install
         ```
+        
         - Or use [PyPi](https://pypi.org/project/scrapy-proxycrawl-middleware/) Python package manager. `pip install scrapy-proxycrawl-middleware`
         
         Then in your Scrapy `settings.py` add the following lines:
         
         ```python
         # Activate the middleware
         PROXYCRAWL_ENABLED = True
@@ -31,41 +38,44 @@
         PROXYCRAWL_TOKEN = 'your token'
         
         # Enable the middleware
         DOWNLOADER_MIDDLEWARES = {
             'scrapy_proxycrawl.ProxyCrawlMiddleware': 610
         }
         ```
+        
         ## Usage
         
         Use the scrapy_proxycrawl.ProxyCrawlRequest instead of the scrapy built-in Request.
         The scrapy_proxycrawl.ProxyCrawlRequest accepts additional arguments, used in Proxy Crawl API:
         
         ```python
         from scrapy_proxycrawl import ProxyCrawlRequest
         
-        yield ProxyCrawlRequest(
-            "http://target-url",
-            callback=self.parse_result
-            device='desktop',
-            country='US',
-            page_wait=1000,
-            ajax_wait=True,
-            dont_filter=True
-        )
+        class ExampleScraper(Spider):
+        
+            def start_requests(self):
+                yield ProxyCrawlRequest(
+                    "http://target-url",
+                    callback=self.parse_result
+                    device='desktop',
+                    country='US',
+                    page_wait=1000,
+                    ajax_wait=True,
+                    dont_filter=True
+                )
         ```
         
         The target url will be replaced with proxy crawl url and parameters will be encoded into the url by the middleware automatically.
         
-        
         If you have questions or need help using the library, please open an issue or [contact us](https://proxycrawl.com/contact).
         
         ---
         
-        Copyright 2020 ProxyCrawl
+        Copyright 2023 ProxyCrawl
         
 Keywords: scrapy middleware scraping scraper crawler crawling proxycrawl api
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 2
 Classifier: Programming Language :: Python :: 2.7
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.5
```

### Comparing `scrapy-proxycrawl-middleware-1.1.0/setup.py` & `scrapy-proxycrawl-middleware-1.2.0/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -8,15 +8,15 @@
     from distutils.core import setup, find_packages
 
 readme = open('README.md').read()
 
 setup(
     name = 'scrapy-proxycrawl-middleware',
     license = 'Apache-2.0',
-    version = '1.1.0',
+    version = '1.2.0',
     description = 'Scrapy ProxyCrawl Proxy Middleware: ProxyCrawl interfacing middleware for Scrapy',
     long_description = readme,
     long_description_content_type = 'text/markdown',
     author = 'ProxyCrawl',
     author_email = 'info@proxycrawl.com',
     url = 'https://github.com/proxycrawl/scrapy-proxycrawl-middleware',
     keywords = 'scrapy middleware scraping scraper crawler crawling proxycrawl api',
```

