# Comparing `tmp/gripcontrol-4.0.0.tar.gz` & `tmp/gripcontrol-4.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/gripcontrol-4.0.0.tar", last modified: Sat Dec 21 17:31:47 2019, max compression
+gzip compressed data, was "dist/gripcontrol-4.1.0.tar", last modified: Fri Apr 23 18:37:57 2021, max compression
```

## Comparing `gripcontrol-4.0.0.tar` & `gripcontrol-4.1.0.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2019-12-21 17:31:47.000000 gripcontrol-4.0.0/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      317 2019-12-21 17:31:47.000000 gripcontrol-4.0.0/PKG-INFO
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       38 2019-12-21 17:31:47.000000 gripcontrol-4.0.0/setup.cfg
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      467 2019-12-21 17:31:41.000000 gripcontrol-4.0.0/setup.py
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2019-12-21 17:31:47.000000 gripcontrol-4.0.0/src/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      815 2017-12-02 22:47:15.000000 gripcontrol-4.0.0/src/__init__.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      535 2018-08-26 23:31:32.000000 gripcontrol-4.0.0/src/channel.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     3180 2017-12-02 22:47:15.000000 gripcontrol-4.0.0/src/websocketcontext.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     9688 2018-08-26 23:31:32.000000 gripcontrol-4.0.0/src/gripcontrol.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1507 2017-12-02 22:47:15.000000 gripcontrol-4.0.0/src/httpstreamformat.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1563 2019-04-19 02:41:02.000000 gripcontrol-4.0.0/src/httpresponseformat.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     5841 2017-12-02 22:47:15.000000 gripcontrol-4.0.0/src/grippubcontrol.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      644 2017-08-02 23:29:31.000000 gripcontrol-4.0.0/src/websocketevent.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      779 2017-08-02 23:29:31.000000 gripcontrol-4.0.0/src/response.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1231 2017-08-03 02:03:01.000000 gripcontrol-4.0.0/src/websocketmessageformat.py
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2019-12-21 17:31:47.000000 gripcontrol-4.0.0/gripcontrol.egg-info/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      317 2019-12-21 17:31:47.000000 gripcontrol-4.0.0/gripcontrol.egg-info/PKG-INFO
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       12 2019-12-21 17:31:47.000000 gripcontrol-4.0.0/gripcontrol.egg-info/top_level.txt
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        1 2019-12-21 17:31:47.000000 gripcontrol-4.0.0/gripcontrol.egg-info/dependency_links.txt
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      406 2019-12-21 17:31:47.000000 gripcontrol-4.0.0/gripcontrol.egg-info/SOURCES.txt
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       48 2019-12-21 17:31:47.000000 gripcontrol-4.0.0/gripcontrol.egg-info/requires.txt
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    11327 2017-08-02 23:29:31.000000 gripcontrol-4.0.0/README.md
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2021-04-23 18:37:57.000000 gripcontrol-4.1.0/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      317 2021-04-23 18:37:57.000000 gripcontrol-4.1.0/PKG-INFO
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       38 2021-04-23 18:37:57.000000 gripcontrol-4.1.0/setup.cfg
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      467 2021-04-23 18:37:54.000000 gripcontrol-4.1.0/setup.py
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2021-04-23 18:37:57.000000 gripcontrol-4.1.0/src/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      815 2017-12-02 22:47:15.000000 gripcontrol-4.1.0/src/__init__.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      535 2018-08-26 23:31:32.000000 gripcontrol-4.1.0/src/channel.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     3180 2017-12-02 22:47:15.000000 gripcontrol-4.1.0/src/websocketcontext.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     9720 2021-04-23 18:37:54.000000 gripcontrol-4.1.0/src/gripcontrol.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1507 2017-12-02 22:47:15.000000 gripcontrol-4.1.0/src/httpstreamformat.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1563 2019-04-19 02:41:02.000000 gripcontrol-4.1.0/src/httpresponseformat.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     5841 2017-12-02 22:47:15.000000 gripcontrol-4.1.0/src/grippubcontrol.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      644 2017-08-02 23:29:31.000000 gripcontrol-4.1.0/src/websocketevent.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      779 2017-08-02 23:29:31.000000 gripcontrol-4.1.0/src/response.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1231 2017-08-03 02:03:01.000000 gripcontrol-4.1.0/src/websocketmessageformat.py
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2021-04-23 18:37:57.000000 gripcontrol-4.1.0/gripcontrol.egg-info/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      317 2021-04-23 18:37:57.000000 gripcontrol-4.1.0/gripcontrol.egg-info/PKG-INFO
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       12 2021-04-23 18:37:57.000000 gripcontrol-4.1.0/gripcontrol.egg-info/top_level.txt
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        1 2021-04-23 18:37:57.000000 gripcontrol-4.1.0/gripcontrol.egg-info/dependency_links.txt
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      406 2021-04-23 18:37:57.000000 gripcontrol-4.1.0/gripcontrol.egg-info/SOURCES.txt
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       48 2021-04-23 18:37:57.000000 gripcontrol-4.1.0/gripcontrol.egg-info/requires.txt
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    11327 2017-08-02 23:29:31.000000 gripcontrol-4.1.0/README.md
```

### Comparing `gripcontrol-4.0.0/src/__init__.py` & `gripcontrol-4.1.0/src/__init__.py`

 * *Files identical despite different names*

### Comparing `gripcontrol-4.0.0/src/channel.py` & `gripcontrol-4.1.0/src/channel.py`

 * *Files identical despite different names*

### Comparing `gripcontrol-4.0.0/src/websocketcontext.py` & `gripcontrol-4.1.0/src/websocketcontext.py`

 * *Files identical despite different names*

### Comparing `gripcontrol-4.0.0/src/gripcontrol.py` & `gripcontrol-4.1.0/src/gripcontrol.py`

 * *Files 1% similar despite different names*

```diff
@@ -68,16 +68,16 @@
 # Note that the token expiration is also verified.
 def validate_sig(token, key):
 	# jwt expects the token in utf-8
 	if _is_unicode_instance(token):
 		token = token.encode('utf-8')	
 
 	try:
-		claim = jwt.decode(token, key)
-	except:
+		claim = jwt.decode(token, key, algorithms=['HS256'])
+	except Exception:
 		return False
 
 	exp = claim.get('exp')
 	if not exp:
 		return False
 
 	if _timestamp_utcnow() >= exp:
```

### Comparing `gripcontrol-4.0.0/src/httpstreamformat.py` & `gripcontrol-4.1.0/src/httpstreamformat.py`

 * *Files identical despite different names*

### Comparing `gripcontrol-4.0.0/src/httpresponseformat.py` & `gripcontrol-4.1.0/src/httpresponseformat.py`

 * *Files identical despite different names*

### Comparing `gripcontrol-4.0.0/src/grippubcontrol.py` & `gripcontrol-4.1.0/src/grippubcontrol.py`

 * *Files identical despite different names*

### Comparing `gripcontrol-4.0.0/src/websocketevent.py` & `gripcontrol-4.1.0/src/websocketevent.py`

 * *Files identical despite different names*

### Comparing `gripcontrol-4.0.0/src/response.py` & `gripcontrol-4.1.0/src/response.py`

 * *Files identical despite different names*

### Comparing `gripcontrol-4.0.0/src/websocketmessageformat.py` & `gripcontrol-4.1.0/src/websocketmessageformat.py`

 * *Files identical despite different names*

### Comparing `gripcontrol-4.0.0/README.md` & `gripcontrol-4.1.0/README.md`

 * *Files identical despite different names*

