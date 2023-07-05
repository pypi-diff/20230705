# Comparing `tmp/pubcontrol-3.4.0.tar.gz` & `tmp/pubcontrol-3.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pubcontrol-3.4.0.tar", last modified: Wed May 17 19:21:30 2023, max compression
+gzip compressed data, was "pubcontrol-3.5.0.tar", last modified: Wed Jul  5 19:11:04 2023, max compression
```

## Comparing `pubcontrol-3.4.0.tar` & `pubcontrol-3.5.0.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxr-xr-x   0 jkarneges   (501) staff       (20)        0 2023-05-17 19:21:30.728363 pubcontrol-3.4.0/
--rw-r--r--   0 jkarneges   (501) staff       (20)     1056 2022-04-22 01:30:17.000000 pubcontrol-3.4.0/COPYING
--rw-r--r--   0 jkarneges   (501) staff       (20)      326 2023-05-17 19:21:30.727973 pubcontrol-3.4.0/PKG-INFO
--rw-r--r--   0 jkarneges   (501) staff       (20)     4331 2022-04-22 01:30:17.000000 pubcontrol-3.4.0/README.md
-drwxr-xr-x   0 jkarneges   (501) staff       (20)        0 2023-05-17 19:21:30.720433 pubcontrol-3.4.0/pubcontrol.egg-info/
--rw-r--r--   0 jkarneges   (501) staff       (20)      326 2023-05-17 19:21:30.000000 pubcontrol-3.4.0/pubcontrol.egg-info/PKG-INFO
--rw-r--r--   0 jkarneges   (501) staff       (20)      388 2023-05-17 19:21:30.000000 pubcontrol-3.4.0/pubcontrol.egg-info/SOURCES.txt
--rw-r--r--   0 jkarneges   (501) staff       (20)        1 2023-05-17 19:21:30.000000 pubcontrol-3.4.0/pubcontrol.egg-info/dependency_links.txt
--rw-r--r--   0 jkarneges   (501) staff       (20)       96 2023-05-17 19:21:30.000000 pubcontrol-3.4.0/pubcontrol.egg-info/requires.txt
--rw-r--r--   0 jkarneges   (501) staff       (20)       11 2023-05-17 19:21:30.000000 pubcontrol-3.4.0/pubcontrol.egg-info/top_level.txt
--rw-r--r--   0 jkarneges   (501) staff       (20)       38 2023-05-17 19:21:30.728496 pubcontrol-3.4.0/setup.cfg
--rw-r--r--   0 jkarneges   (501) staff       (20)      522 2023-05-17 19:21:17.000000 pubcontrol-3.4.0/setup.py
-drwxr-xr-x   0 jkarneges   (501) staff       (20)        0 2023-05-17 19:21:30.726932 pubcontrol-3.4.0/src/
--rw-r--r--   0 jkarneges   (501) staff       (20)      569 2022-04-22 01:30:17.000000 pubcontrol-3.4.0/src/__init__.py
--rw-r--r--   0 jkarneges   (501) staff       (20)      716 2022-04-22 01:30:17.000000 pubcontrol-3.4.0/src/format.py
--rw-r--r--   0 jkarneges   (501) staff       (20)     2420 2022-04-22 01:30:17.000000 pubcontrol-3.4.0/src/item.py
--rw-r--r--   0 jkarneges   (501) staff       (20)     1846 2022-04-22 01:30:17.000000 pubcontrol-3.4.0/src/pcccbhandler.py
--rw-r--r--   0 jkarneges   (501) staff       (20)    11448 2022-04-22 01:30:17.000000 pubcontrol-3.4.0/src/pubcontrol.py
--rw-r--r--   0 jkarneges   (501) staff       (20)    10348 2023-05-17 19:21:17.000000 pubcontrol-3.4.0/src/pubcontrolclient.py
--rw-r--r--   0 jkarneges   (501) staff       (20)    10369 2022-04-22 01:30:17.000000 pubcontrol-3.4.0/src/pubsubmonitor.py
--rw-r--r--   0 jkarneges   (501) staff       (20)     2414 2022-04-22 01:30:17.000000 pubcontrol-3.4.0/src/utilities.py
--rw-r--r--   0 jkarneges   (501) staff       (20)    12981 2022-04-22 01:30:17.000000 pubcontrol-3.4.0/src/zmqpubcontrolclient.py
--rw-r--r--   0 jkarneges   (501) staff       (20)     6432 2022-04-22 01:30:17.000000 pubcontrol-3.4.0/src/zmqpubcontroller.py
+drwxr-xr-x   0 jkarneges   (501) staff       (20)        0 2023-07-05 19:11:04.405155 pubcontrol-3.5.0/
+-rw-r--r--   0 jkarneges   (501) staff       (20)     1056 2022-04-22 01:30:17.000000 pubcontrol-3.5.0/COPYING
+-rw-r--r--   0 jkarneges   (501) staff       (20)      298 2023-07-05 19:11:04.404604 pubcontrol-3.5.0/PKG-INFO
+-rw-r--r--   0 jkarneges   (501) staff       (20)     4331 2022-04-22 01:30:17.000000 pubcontrol-3.5.0/README.md
+drwxr-xr-x   0 jkarneges   (501) staff       (20)        0 2023-07-05 19:11:04.396735 pubcontrol-3.5.0/pubcontrol.egg-info/
+-rw-r--r--   0 jkarneges   (501) staff       (20)      298 2023-07-05 19:11:04.000000 pubcontrol-3.5.0/pubcontrol.egg-info/PKG-INFO
+-rw-r--r--   0 jkarneges   (501) staff       (20)      388 2023-07-05 19:11:04.000000 pubcontrol-3.5.0/pubcontrol.egg-info/SOURCES.txt
+-rw-r--r--   0 jkarneges   (501) staff       (20)        1 2023-07-05 19:11:04.000000 pubcontrol-3.5.0/pubcontrol.egg-info/dependency_links.txt
+-rw-r--r--   0 jkarneges   (501) staff       (20)       96 2023-07-05 19:11:04.000000 pubcontrol-3.5.0/pubcontrol.egg-info/requires.txt
+-rw-r--r--   0 jkarneges   (501) staff       (20)       11 2023-07-05 19:11:04.000000 pubcontrol-3.5.0/pubcontrol.egg-info/top_level.txt
+-rw-r--r--   0 jkarneges   (501) staff       (20)       38 2023-07-05 19:11:04.405324 pubcontrol-3.5.0/setup.cfg
+-rw-r--r--   0 jkarneges   (501) staff       (20)      522 2023-07-05 19:10:58.000000 pubcontrol-3.5.0/setup.py
+drwxr-xr-x   0 jkarneges   (501) staff       (20)        0 2023-07-05 19:11:04.403535 pubcontrol-3.5.0/src/
+-rw-r--r--   0 jkarneges   (501) staff       (20)      569 2022-04-22 01:30:17.000000 pubcontrol-3.5.0/src/__init__.py
+-rw-r--r--   0 jkarneges   (501) staff       (20)      716 2022-04-22 01:30:17.000000 pubcontrol-3.5.0/src/format.py
+-rw-r--r--   0 jkarneges   (501) staff       (20)     2420 2022-04-22 01:30:17.000000 pubcontrol-3.5.0/src/item.py
+-rw-r--r--   0 jkarneges   (501) staff       (20)     1846 2022-04-22 01:30:17.000000 pubcontrol-3.5.0/src/pcccbhandler.py
+-rw-r--r--   0 jkarneges   (501) staff       (20)    11555 2023-07-05 19:10:58.000000 pubcontrol-3.5.0/src/pubcontrol.py
+-rw-r--r--   0 jkarneges   (501) staff       (20)    10692 2023-07-05 19:10:58.000000 pubcontrol-3.5.0/src/pubcontrolclient.py
+-rw-r--r--   0 jkarneges   (501) staff       (20)    10651 2023-07-05 19:10:58.000000 pubcontrol-3.5.0/src/pubsubmonitor.py
+-rw-r--r--   0 jkarneges   (501) staff       (20)     2414 2022-04-22 01:30:17.000000 pubcontrol-3.5.0/src/utilities.py
+-rw-r--r--   0 jkarneges   (501) staff       (20)    12981 2022-04-22 01:30:17.000000 pubcontrol-3.5.0/src/zmqpubcontrolclient.py
+-rw-r--r--   0 jkarneges   (501) staff       (20)     6432 2022-04-22 01:30:17.000000 pubcontrol-3.5.0/src/zmqpubcontroller.py
```

### Comparing `pubcontrol-3.4.0/COPYING` & `pubcontrol-3.5.0/COPYING`

 * *Files identical despite different names*

### Comparing `pubcontrol-3.4.0/README.md` & `pubcontrol-3.5.0/README.md`

 * *Files identical despite different names*

### Comparing `pubcontrol-3.4.0/setup.py` & `pubcontrol-3.5.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 #!/usr/bin/env python
 
 from setuptools import setup
 
 setup(
 	name='pubcontrol',
-	version='3.4.0',
+	version='3.5.0',
 	description='EPCP library',
 	author='Justin Karneges',
 	author_email='justin@fanout.io',
 	url='https://github.com/fanout/pypubcontrol',
 	license='MIT',
 	package_dir={'pubcontrol': 'src'},
 	packages=['pubcontrol'],
```

### Comparing `pubcontrol-3.4.0/src/__init__.py` & `pubcontrol-3.5.0/src/__init__.py`

 * *Files identical despite different names*

### Comparing `pubcontrol-3.4.0/src/format.py` & `pubcontrol-3.5.0/src/format.py`

 * *Files identical despite different names*

### Comparing `pubcontrol-3.4.0/src/item.py` & `pubcontrol-3.5.0/src/item.py`

 * *Files identical despite different names*

### Comparing `pubcontrol-3.4.0/src/pcccbhandler.py` & `pubcontrol-3.5.0/src/pcccbhandler.py`

 * *Files identical despite different names*

### Comparing `pubcontrol-3.4.0/src/pubcontrol.py` & `pubcontrol-3.5.0/src/pubcontrol.py`

 * *Files 1% similar despite different names*

```diff
@@ -116,23 +116,27 @@
 		try:
 			for entry in config:
 				client = None
 				require_subscribers = entry.get('require_subscribers', False)
 				if 'uri' in entry:
 					claim = None
 					key = None
-					if 'iss' in entry:
-						claim = {'iss': entry['iss']}
-						key = entry['key']
+					bearer = None
+					if 'key' in entry:
+						if 'iss' in entry:
+							claim = {'iss': entry['iss']}
+							key = entry['key']
+						else:
+							bearer = entry['key']
 					handler = PubControl.SubCallbackHandler(self._client_sub_callback)
 					try:
 						handler.lock.acquire()
 						client = PubControlClient(entry['uri'],
 								claim, key, require_subscribers,
-								handler.handle)
+								handler.handle, auth_bearer=bearer)
 						handler.client = client
 					finally:
 						handler.lock.release()
 				if ('zmq_uri' in entry or 'zmq_push_uri' in entry or
 						'zmq_pub_uri' in entry):
 					_verify_zmq()
 					client = ZmqPubControlClient(entry.get('zmq_uri'),
```

### Comparing `pubcontrol-3.4.0/src/pubcontrolclient.py` & `pubcontrol-3.5.0/src/pubcontrolclient.py`

 * *Files 3% similar despite different names*

```diff
@@ -25,24 +25,25 @@
 # If require_subscribers is set to True then channel subscription monitoring
 # will be enabled and only channels that are subscribed to will be published
 # to.
 class PubControlClient(object):
 
 	# Initialize this class with a URL representing the publishing endpoint.
 	def __init__(self, uri, auth_jwt_claim=None,
-			auth_jwt_key=None, require_subscribers=False, sub_callback=None):
+			auth_jwt_key=None, require_subscribers=False, sub_callback=None, auth_bearer=None):
 		self.uri = uri
 		self.lock = threading.Lock()
 		self.thread = None
 		self.thread_cond = None
 		self.req_queue = deque()
 		self.auth_basic_user = None
 		self.auth_basic_pass = None
 		self.auth_jwt_claim = auth_jwt_claim
 		self.auth_jwt_key = auth_jwt_key
+		self.auth_bearer = auth_bearer
 		self.sub_monitor = None
 		self.closed = False
 
 		retry = Retry(
 			total=1,
 			backoff_factor=0.5,
 			status_forcelist=[500, 502, 503, 504],
@@ -52,25 +53,33 @@
 		adapter = HTTPAdapter(max_retries=retry)
 
 		self.requests_session = requests.session()
 		self.requests_session.mount('http://', adapter)
 		self.requests_session.mount('https://', adapter)
 
 		if require_subscribers:
-			self.sub_monitor = PubSubMonitor(uri, auth_jwt_claim, auth_jwt_key, sub_callback)
+			self.sub_monitor = PubSubMonitor(uri, auth_jwt_claim, auth_jwt_key, sub_callback, auth_bearer)
 
 	# Call this method and pass a username and password to use basic
 	# authentication with the configured endpoint.
 	def set_auth_basic(self, username, password):
 		self._verify_notclosed()
 		self.lock.acquire()
 		self.auth_basic_user = username
 		self.auth_basic_pass = password
 		self.lock.release()
 
+	# Call this method to use bearer authentication with the
+	# configured endpoint.
+	def set_auth_bearer(self, value):
+		self._verify_notclosed()
+		self.lock.acquire()
+		self.auth_bearer = value
+		self.lock.release()
+
 	# Call this method and pass a claim and key to use JWT authentication
 	# with the configured endpoint.
 	def set_auth_jwt(self, claim, key):
 		self._verify_notclosed()
 		self.lock.acquire()
 		self.auth_jwt_claim = claim
 		self.auth_jwt_key = key
@@ -166,14 +175,16 @@
 	# An internal method used to generate an authorization header. The
 	# authorization header is generated based on whether basic or JWT
 	# authorization information was provided via the publicly accessible
 	# 'set_*_auth' methods defined above.
 	def _gen_auth_header(self):
 		if self.auth_basic_user:
 			return 'Basic ' + str(b64encode(('%s:%s' % (self.auth_basic_user, self.auth_basic_pass)).encode('ascii')))
+		elif self.auth_bearer:
+			return 'Bearer ' + self.auth_bearer
 		elif self.auth_jwt_claim:
 			return _gen_auth_jwt_header(self.auth_jwt_claim, self.auth_jwt_key)
 		else:
 			return None
 
 	# An internal method that ensures that asynchronous publish calls are
 	# properly processed. This method initializes the required class fields,
```

### Comparing `pubcontrol-3.4.0/src/pubsubmonitor.py` & `pubcontrol-3.5.0/src/pubsubmonitor.py`

 * *Files 3% similar despite different names*

```diff
@@ -26,21 +26,23 @@
 	from httplib import IncompleteRead
 
 # The PubSubMonitor class monitors subscriptions to channels via an HTTP interface.
 class PubSubMonitor(object):
 
 	# Initialize with base stream URI, JWT auth info, and callback used for indicating
 	# when a subscription event occurs.
-	def __init__(self, base_stream_uri, auth_jwt_claim=None, auth_jwt_key=None, callback=None):
+	def __init__(self, base_stream_uri, auth_jwt_claim=None, auth_jwt_key=None, callback=None, auth_bearer=None):
 		if base_stream_uri[-1:] != '/':
 			base_stream_uri += '/'
 		self._stream_uri = base_stream_uri + 'subscriptions/stream/'
 		self._items_uri = base_stream_uri + 'subscriptions/items/'
 		self._auth_jwt_claim = None
-		if auth_jwt_claim:
+		if auth_bearer:
+			self._auth_bearer = auth_bearer
+		elif auth_jwt_claim:
 			self._auth_jwt_claim = copy.deepcopy(auth_jwt_claim)
 			self._auth_jwt_key = auth_jwt_key
 		self._callback = callback
 		self._lock = threading.Lock()
 		self._requests_session = requests.session()
 		self._stream_response = None
 		self._channels = set()
@@ -86,16 +88,19 @@
 			while retry_connection:
 				time.sleep(wait_interval)
 				wait_interval = PubSubMonitor._increase_wait_interval(wait_interval)
 				try:
 					logger.debug('stream get %s' % self._stream_uri)
 					timeout = (5,60)
 					headers = {}
-					headers['Authorization'] = _gen_auth_jwt_header(
-							self._auth_jwt_claim, self._auth_jwt_key)
+					if self._auth_bearer:
+						headers['Authorization'] = 'Bearer ' + self._auth_bearer
+					else:
+						headers['Authorization'] = _gen_auth_jwt_header(
+								self._auth_jwt_claim, self._auth_jwt_key)
 					self._stream_response = self._requests_session.get(
 							self._stream_uri, headers=headers, stream=True,
 							timeout=timeout)
 					# No concern about a race condition here since there's 5 full
 					# seconds between the .get() method above returning and the
 					# timeout exception being thrown. The lines below are guaranteed
 					# to execute within 5 seconds.
@@ -219,16 +224,19 @@
 						if self._last_cursor:
 							logger.debug('history get %s (%s)' % (
 									uri, PubSubMonitor._parse_cursor(
 									self._last_cursor)))
 						else:
 							logger.debug('history get %s' % uri)
 						headers = {}
-						headers['Authorization'] = _gen_auth_jwt_header(
-								self._auth_jwt_claim, self._auth_jwt_key)
+						if self._auth_bearer:
+							headers['Authorization'] = 'Bearer ' + self._auth_bearer
+						else:
+							headers['Authorization'] = _gen_auth_jwt_header(
+									self._auth_jwt_claim, self._auth_jwt_key)
 						res = self._requests_session.get(uri, headers=headers,
 								timeout=30)
 						if (res.status_code >= 200 and
 								res.status_code < 300):
 							retry_connection = False
 						elif res.status_code == 404:
 							self._unsub_and_clear_channels()
```

### Comparing `pubcontrol-3.4.0/src/utilities.py` & `pubcontrol-3.5.0/src/utilities.py`

 * *Files identical despite different names*

### Comparing `pubcontrol-3.4.0/src/zmqpubcontrolclient.py` & `pubcontrol-3.5.0/src/zmqpubcontrolclient.py`

 * *Files identical despite different names*

### Comparing `pubcontrol-3.4.0/src/zmqpubcontroller.py` & `pubcontrol-3.5.0/src/zmqpubcontroller.py`

 * *Files identical despite different names*

