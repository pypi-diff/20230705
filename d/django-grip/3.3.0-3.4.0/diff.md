# Comparing `tmp/django-grip-3.3.0.tar.gz` & `tmp/django-grip-3.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django-grip-3.3.0.tar", last modified: Sat May 27 00:49:53 2023, max compression
+gzip compressed data, was "django-grip-3.4.0.tar", last modified: Wed Jul  5 19:38:12 2023, max compression
```

## Comparing `django-grip-3.3.0.tar` & `django-grip-3.4.0.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxr-xr-x   0 jkarneges   (501) staff       (20)        0 2023-05-27 00:49:53.182755 django-grip-3.3.0/
--rw-r--r--   0 jkarneges   (501) staff       (20)     1056 2022-06-17 18:20:45.000000 django-grip-3.3.0/COPYING
--rw-r--r--   0 jkarneges   (501) staff       (20)      333 2023-05-27 00:49:53.182944 django-grip-3.3.0/PKG-INFO
--rw-r--r--   0 jkarneges   (501) staff       (20)     5974 2022-06-17 18:20:45.000000 django-grip-3.3.0/README.md
-drwxr-xr-x   0 jkarneges   (501) staff       (20)        0 2023-05-27 00:49:53.182368 django-grip-3.3.0/django_grip.egg-info/
--rw-r--r--   0 jkarneges   (501) staff       (20)      333 2023-05-27 00:49:52.000000 django-grip-3.3.0/django_grip.egg-info/PKG-INFO
--rw-r--r--   0 jkarneges   (501) staff       (20)      225 2023-05-27 00:49:53.000000 django-grip-3.3.0/django_grip.egg-info/SOURCES.txt
--rw-r--r--   0 jkarneges   (501) staff       (20)        1 2023-05-27 00:49:52.000000 django-grip-3.3.0/django_grip.egg-info/dependency_links.txt
--rw-r--r--   0 jkarneges   (501) staff       (20)       81 2023-05-27 00:49:53.000000 django-grip-3.3.0/django_grip.egg-info/requires.txt
--rw-r--r--   0 jkarneges   (501) staff       (20)       12 2023-05-27 00:49:53.000000 django-grip-3.3.0/django_grip.egg-info/top_level.txt
--rw-r--r--   0 jkarneges   (501) staff       (20)    10731 2022-08-17 01:15:17.000000 django-grip-3.3.0/django_grip.py
--rw-r--r--   0 jkarneges   (501) staff       (20)       79 2023-05-27 00:49:53.183564 django-grip-3.3.0/setup.cfg
--rw-r--r--   0 jkarneges   (501) staff       (20)      477 2023-05-27 00:49:47.000000 django-grip-3.3.0/setup.py
+drwxr-xr-x   0 jkarneges   (501) staff       (20)        0 2023-07-05 19:38:12.592558 django-grip-3.4.0/
+-rw-r--r--   0 jkarneges   (501) staff       (20)     1056 2022-06-17 18:20:45.000000 django-grip-3.4.0/COPYING
+-rw-r--r--   0 jkarneges   (501) staff       (20)      305 2023-07-05 19:38:12.592710 django-grip-3.4.0/PKG-INFO
+-rw-r--r--   0 jkarneges   (501) staff       (20)     6044 2023-07-05 19:38:09.000000 django-grip-3.4.0/README.md
+drwxr-xr-x   0 jkarneges   (501) staff       (20)        0 2023-07-05 19:38:12.592178 django-grip-3.4.0/django_grip.egg-info/
+-rw-r--r--   0 jkarneges   (501) staff       (20)      305 2023-07-05 19:38:12.000000 django-grip-3.4.0/django_grip.egg-info/PKG-INFO
+-rw-r--r--   0 jkarneges   (501) staff       (20)      225 2023-07-05 19:38:12.000000 django-grip-3.4.0/django_grip.egg-info/SOURCES.txt
+-rw-r--r--   0 jkarneges   (501) staff       (20)        1 2023-07-05 19:38:12.000000 django-grip-3.4.0/django_grip.egg-info/dependency_links.txt
+-rw-r--r--   0 jkarneges   (501) staff       (20)       81 2023-07-05 19:38:12.000000 django-grip-3.4.0/django_grip.egg-info/requires.txt
+-rw-r--r--   0 jkarneges   (501) staff       (20)       12 2023-07-05 19:38:12.000000 django-grip-3.4.0/django_grip.egg-info/top_level.txt
+-rw-r--r--   0 jkarneges   (501) staff       (20)    10987 2023-07-05 19:38:09.000000 django-grip-3.4.0/django_grip.py
+-rw-r--r--   0 jkarneges   (501) staff       (20)       79 2023-07-05 19:38:12.593163 django-grip-3.4.0/setup.cfg
+-rw-r--r--   0 jkarneges   (501) staff       (20)      477 2023-07-05 19:38:09.000000 django-grip-3.4.0/setup.py
```

### Comparing `django-grip-3.3.0/COPYING` & `django-grip-3.4.0/COPYING`

 * *Files identical despite different names*

### Comparing `django-grip-3.3.0/README.md` & `django-grip-3.4.0/README.md`

 * *Files 15% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 # Django GRIP
 
 Author: Justin Karneges <justin@fanout.io>
 
-This library helps your Django application delegate long-lived HTTP/WebSocket connection management to a GRIP-compatible proxy such as [Fanout Cloud](https://fanout.io/) or [Pushpin](https://pushpin.org/).
+This library helps your Django application delegate long-lived HTTP/WebSocket connection management to a GRIP-compatible proxy such as [Pushpin](https://pushpin.org/) or [Fastly Fanout](https://fanout.io/).
 
 ## Setup
 
 First, install this module:
 
 ```sh
 pip install django-grip
@@ -22,21 +22,25 @@
 ```
 
 The middleware handles parsing/generating GRIP headers and WebSocket-Over-HTTP events. It should be placed early in the stack.
 
 Additionally, set `GRIP_URL` with your proxy settings, e.g.:
 
 ```python
-# fanout cloud
-GRIP_URL = 'http://api.fanout.io/realm/your-realm?iss=your-realm&key=base64:your-realm-key'
+# pushpin
+GRIP_URL = 'http://localhost:5561'
 ```
 
 ```python
-# pushpin
-GRIP_URL = 'http://localhost:5561'
+# fastly
+GRIP_VERIFY_KEY = """
+[ ... public key ... ]
+"""
+
+GRIP_URL = 'https://api.fastly.com/service/your-service-id?verify-iss=fastly:your-service-id&key=your-api-token'
 ```
 
 ## Usage
 
 ### HTTP streaming
 
 ```python
@@ -148,27 +152,27 @@
 
 The `while` loop is deceptive. It looks like it's looping for the lifetime of the WebSocket connection, but what it's really doing is looping through a batch of WebSocket messages that was just received via HTTP. Often this will be one message, and so the loop performs one iteration and then exits. Similarly, the `ws` object only exists for the duration of the handler invocation, rather than for the lifetime of the connection as you might expect. It may look like socket code, but it's all an illusion. :tophat:
 
 For details on the underlying protocol conversion, see the [WebSocket-Over-HTTP Protocol spec](http://pushpin.org/docs/protocols/websocket-over-http/).
 
 ## Advanced settings
 
-If you need to communicate with more than one GRIP proxy (e.g. multiple Pushpin instances, or Fanout Cloud + Pushpin), you can use `GRIP_PROXIES` instead of `GRIP_URL`. For example:
+If you need to communicate with more than one GRIP proxy (e.g. multiple Pushpin instances, or Fastly Fanout + Pushpin), you can use `GRIP_PROXIES` instead of `GRIP_URL`. For example:
 
 ```python
 GRIP_PROXIES = [
     # pushpin
     {
         'control_uri': 'http://localhost:5561'
     },
-    # fanout cloud
+    # fastly
     {
-        'key': b64decode('your-realm-key'),
-        'control_uri': 'http://api.fanout.io/realm/your-realm',
-        'control_iss': 'your-realm'
+        'control_uri': 'https://api.fastly.com/service/your-service-id',
+        'key': 'your-api-token',
+        'verify_iss': 'fastly:your-service-id'
     }
 ]
 ```
 
 If it's possible for clients to access the Django app directly, without necessarily going through a GRIP proxy, then you may want to avoid sending GRIP instructions to those clients. An easy way to achieve this is with the `GRIP_PROXY_REQUIRED` setting. If set, then any direct requests that trigger a GRIP instruction response will be given a 501 Not Implemented error instead.
 
 ```python
```

### Comparing `django-grip-3.3.0/django_grip.py` & `django-grip-3.4.0/django_grip.py`

 * *Files 4% similar despite different names*

```diff
@@ -89,14 +89,21 @@
 		return self.instruct
 
 def _get_proxies():
 	proxies = getattr(settings, 'GRIP_PROXIES', [])
 	grip_url = getattr(settings, 'GRIP_URL', None)
 	if grip_url:
 		proxies.append(parse_grip_uri(grip_url))
+
+	verify_key = getattr(settings, 'GRIP_VERIFY_KEY', None)
+	if verify_key:
+		for p in proxies:
+			if 'verify_key' not in p:
+				p['verify_key'] = verify_key
+
 	return proxies
 
 def _get_pubcontrol():
 	global _pubcontrol
 	_lock.acquire()
 	if _pubcontrol is None:
 		_pubcontrol = GripPubControl()
@@ -216,24 +223,25 @@
 
 		grip_sig_header = request.META.get('HTTP_GRIP_SIG')
 		if grip_sig_header:
 			proxies = _get_proxies()
 
 			all_proxies_have_keys = True
 			for entry in proxies:
-				if 'key' not in entry:
+				if 'verify_key' not in entry and 'key' not in entry:
 					all_proxies_have_keys = False
 					break
 
 			if all_proxies_have_keys:
 				# if all proxies have keys, then don't
 				#   consider the request to be proxied unless
 				#   one of them signed it
 				for entry in proxies:
-					if validate_sig(grip_sig_header, entry['key']):
+					key = entry.get('verify_key', entry['key'])
+					if validate_sig(grip_sig_header, key, iss=entry.get('verify_iss')):
 						proxied = True
 						signed = True
 						break
 			else:
 				# if even one proxy doesn't have a key, then
 				#   don't require verification in order to
 				#   consider the request to have been proxied
```

