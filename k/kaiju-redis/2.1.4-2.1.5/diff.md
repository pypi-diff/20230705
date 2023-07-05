# Comparing `tmp/kaiju_redis-2.1.4-py3-none-any.whl.zip` & `tmp/kaiju_redis-2.1.5-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,12 +1,12 @@
-Zip file size: 8999 bytes, number of entries: 10
--rw-r--r--  2.0 unx      110 b- defN 23-Jul-02 12:45 kaiju_redis/__init__.py
--rw-r--r--  2.0 unx    14894 b- defN 23-Jul-02 12:45 kaiju_redis/services.py
--rw-r--r--  2.0 unx        0 b- defN 23-Jul-02 12:45 kaiju_redis/tests/__init__.py
--rw-r--r--  2.0 unx     2956 b- defN 23-Jul-02 12:45 kaiju_redis/tests/fixtures.py
--rw-r--r--  2.0 unx     4086 b- defN 23-Jul-02 12:45 kaiju_redis/tests/test_redis.py
--rw-rw-rw-  2.0 unx      610 b- defN 23-Jul-02 12:45 kaiju_redis-2.1.4.dist-info/LICENSE
--rw-r--r--  2.0 unx     3002 b- defN 23-Jul-02 12:45 kaiju_redis-2.1.4.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 23-Jul-02 12:45 kaiju_redis-2.1.4.dist-info/WHEEL
--rw-r--r--  2.0 unx       12 b- defN 23-Jul-02 12:45 kaiju_redis-2.1.4.dist-info/top_level.txt
--rw-rw-r--  2.0 unx      822 b- defN 23-Jul-02 12:45 kaiju_redis-2.1.4.dist-info/RECORD
-10 files, 26584 bytes uncompressed, 7589 bytes compressed:  71.5%
+Zip file size: 9109 bytes, number of entries: 10
+-rw-r--r--  2.0 unx      110 b- defN 23-Jul-05 18:36 kaiju_redis/__init__.py
+-rw-r--r--  2.0 unx    14911 b- defN 23-Jul-05 18:36 kaiju_redis/services.py
+-rw-r--r--  2.0 unx        0 b- defN 23-Jul-05 18:36 kaiju_redis/tests/__init__.py
+-rw-r--r--  2.0 unx     2980 b- defN 23-Jul-05 18:36 kaiju_redis/tests/fixtures.py
+-rw-r--r--  2.0 unx     4433 b- defN 23-Jul-05 18:36 kaiju_redis/tests/test_redis.py
+-rw-rw-rw-  2.0 unx      610 b- defN 23-Jul-05 18:36 kaiju_redis-2.1.5.dist-info/LICENSE
+-rw-r--r--  2.0 unx     3116 b- defN 23-Jul-05 18:36 kaiju_redis-2.1.5.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 23-Jul-05 18:36 kaiju_redis-2.1.5.dist-info/WHEEL
+-rw-r--r--  2.0 unx       12 b- defN 23-Jul-05 18:36 kaiju_redis-2.1.5.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx      822 b- defN 23-Jul-05 18:36 kaiju_redis-2.1.5.dist-info/RECORD
+10 files, 27086 bytes uncompressed, 7699 bytes compressed:  71.6%
```

## zipnote {}

```diff
@@ -9,23 +9,23 @@
 
 Filename: kaiju_redis/tests/fixtures.py
 Comment: 
 
 Filename: kaiju_redis/tests/test_redis.py
 Comment: 
 
-Filename: kaiju_redis-2.1.4.dist-info/LICENSE
+Filename: kaiju_redis-2.1.5.dist-info/LICENSE
 Comment: 
 
-Filename: kaiju_redis-2.1.4.dist-info/METADATA
+Filename: kaiju_redis-2.1.5.dist-info/METADATA
 Comment: 
 
-Filename: kaiju_redis-2.1.4.dist-info/WHEEL
+Filename: kaiju_redis-2.1.5.dist-info/WHEEL
 Comment: 
 
-Filename: kaiju_redis-2.1.4.dist-info/top_level.txt
+Filename: kaiju_redis-2.1.5.dist-info/top_level.txt
 Comment: 
 
-Filename: kaiju_redis-2.1.4.dist-info/RECORD
+Filename: kaiju_redis-2.1.5.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## kaiju_redis/__init__.py

```diff
@@ -1,5 +1,5 @@
 from .services import *
 
-__version__ = '2.1.4'
+__version__ = '2.1.5'
 __python_version__ = '3.8'
 __author__ = 'antonnidhoggr@me.com'
```

## kaiju_redis/services.py

```diff
@@ -41,15 +41,15 @@
         :param cluster: use cluster connector class
         :param connect_timeout: connection timeout
         :param max_idle_time: max connection idle time
         :param retry_on_timeout: retry connection on timeout
         :param logger:
         :param kws: additional transport cls args
         """
-        ContextableService.__init__(self, app, logger=logger)
+        super().__init__(app, logger=logger)
         if cluster:
             cls = self.cluster_transport_class
         else:
             cls = self.transport_class
         self._transport = cls(
             *args,
             connect_timeout=connect_timeout,
@@ -293,15 +293,15 @@
         self,
         *args,
         group_id: str = None,
         consumer_id: str = None,
         max_batch_size: int = 10,
         max_wait_time_ms: int = 500,
         pending_messages_time_ms: int = None,
-        trim_size: int = None,
+        trim_size: int = 100000,
         **kws,
     ):
         """Initialize.
 
         :param group_id: consumer group, `app.name` by default
         :param consumer_id: unique instance id, `app.id` by default
         :param max_batch_size: max single acquired batch size
@@ -352,17 +352,16 @@
             groups, mk_stream = frozenset(), True
         else:
             groups, mk_stream = frozenset(group[b'name'].decode() for group in groups), False
         if self.group_id not in groups:
             result = await self._transport.xgroup_create(self._key, self.group_id, identifier='$', mkstream=mk_stream)
             self.logger.debug('group create: %s', result)
 
-    @classmethod
-    def get_transport_cls(cls) -> Type:
-        return RedisTransportService
+    def get_transport(self):
+        return self.discover_service(self._transport, cls=RedisTransportService)
 
     async def _read_batch(self) -> list:
         try:
             batch = await self._transport.xreadgroup(
                 self.group_id,
                 self.consumer_id,
                 count=self.max_batch_size,
@@ -411,17 +410,16 @@
 
 class RedisStreamRPCClient(StreamRPCClient):
     """Redis stream client."""
 
     _transport: RedisTransportService
     _dumps = msgpack_dumps
 
-    @classmethod
-    def get_transport_cls(cls) -> Type:
-        return RedisTransportService
+    def get_transport(self):
+        return self.discover_service(self._transport, cls=RedisTransportService)
 
     async def write(self, topic: NSKey, body, headers: dict = None, key=None) -> None:
         """Write data to the stream.
 
         :param topic: topic key
         :param body: rpc request body
         :param headers: request headers
```

## kaiju_redis/tests/fixtures.py

```diff
@@ -87,14 +87,15 @@
         rpc_service=rpc,
         scheduler=scheduler,
         session_service=mock_sessions,
         authentication_service=mock_auth,
         locks_service=mock_locks,
         max_batch_size=1,
         max_wait_time_ms=50,
+        scope='SYSTEM',
     )
     app.services.add_service(service)
     return service
 
 
 @pytest.fixture
 def redis_client(app, redis_transport, mock_users) -> RedisStreamRPCClient:
```

## kaiju_redis/tests/test_redis.py

```diff
@@ -1,8 +1,9 @@
 import asyncio
+import uuid
 
 import pytest  # noqa: pycharm
 import pytest_asyncio
 
 from kaiju_tools.tests.test_cache import TestCache as TestCacheBase
 from kaiju_tools.tests.test_locks import TestLocks as TestLocksBase
 from kaiju_tools.tests.test_streams import TestStreamServer as TestStreamServerBase
@@ -100,14 +101,22 @@
             await _queue.join()
         value = await _listener._transport.xlen(_listener._key)
         assert value == 10, 'before trim'
         await _listener._trim_records()
         value = await _listener._transport.xlen(_listener._key)
         assert value == 1, 'after trim'
 
+    async def test_connection_issues(self, redis_glob, rpc, _listener, _queue, mock_service):
+        redis_glob.pause()
+        await asyncio.sleep(3)
+        redis_glob.unpause()
+        await _listener._transport.flushdb()
+        await asyncio.sleep(1)
+        await self.test_valid_requests(rpc, _listener, _queue, mock_service)
+
 
 @pytest.mark.docker
 class TestStreamClient(TestStreamClientBase):
     """Test redis stream client."""
 
     @pytest_asyncio.fixture
     async def _client(self, app, redis_listener, mock_service, mock_sessions, mock_session, redis_client):
```

## Comparing `kaiju_redis-2.1.4.dist-info/LICENSE` & `kaiju_redis-2.1.5.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `kaiju_redis-2.1.4.dist-info/METADATA` & `kaiju_redis-2.1.5.dist-info/METADATA`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: kaiju-redis
-Version: 2.1.4
+Version: 2.1.5
 Summary: Redis and keydb services
 Home-page: https://gitlab.com/kaiju-python/kaiju-redis
 Author: antonnidhoggr@me.com
 Author-email: antonnidhoggr@me.com
 License: Apache Software License 2.0
 Classifier: Development Status :: 3 - Alpha
 Classifier: License :: OSI Approved :: Apache Software License
@@ -37,18 +37,20 @@
 Requires-Dist: pip-tools (>=6.13) ; extra == 'dev'
 Requires-Dist: pyupgrade (>=3.4) ; extra == 'dev'
 Requires-Dist: towncrier (>=23.6) ; extra == 'dev'
 Provides-Extra: docs
 Requires-Dist: sphinx ; extra == 'docs'
 Requires-Dist: python-docs-theme ; extra == 'docs'
 Provides-Extra: test
-Requires-Dist: pytest (>=7.2) ; extra == 'test'
-Requires-Dist: pytest-asyncio (>=0.20) ; extra == 'test'
-Requires-Dist: docker (>=6.0) ; extra == 'test'
+Requires-Dist: pytest (>=7.4) ; extra == 'test'
+Requires-Dist: pytest-asyncio (>=0.21) ; extra == 'test'
+Requires-Dist: docker (>=6.1.3) ; extra == 'test'
 Requires-Dist: pytest-timeout (>=2.1) ; extra == 'test'
+Requires-Dist: pytest-aiohttp (>=1.0.4) ; extra == 'test'
+Requires-Dist: pytest-cov (>=4.1.0) ; extra == 'test'
 
 
 .. image:: https://badge.fury.io/py/kaiju-redis.svg
     :target: https://pypi.org/project/kaiju-redis
     :alt: Latest package version
 
 .. image:: https://readthedocs.org/projects/kaiju-redis/badge/?version=latest
```

## Comparing `kaiju_redis-2.1.4.dist-info/RECORD` & `kaiju_redis-2.1.5.dist-info/RECORD`

 * *Files 24% similar despite different names*

```diff
@@ -1,10 +1,10 @@
-kaiju_redis/__init__.py,sha256=GbveAxfFie7WR4l0-ZEZQX5pX1f98fV-MIQ_VL_1304,110
-kaiju_redis/services.py,sha256=Xu-sQXiilGnHTUqnfPF2pnn6VG5fRuTFrMrqqXcJePg,14894
+kaiju_redis/__init__.py,sha256=4IGYmMC8wr41NpeN3cSHCmvlYdc78esO8e8KwMtQUWs,110
+kaiju_redis/services.py,sha256=xbB2dv-iLRwm-Sn2zPLtIYvMMSJne96qyRUQ6E8M_A0,14911
 kaiju_redis/tests/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
-kaiju_redis/tests/fixtures.py,sha256=YDaJxKaEmbPQyi64x0o-dxDwK9JE90hdzUxbEc6QkEk,2956
-kaiju_redis/tests/test_redis.py,sha256=Mu5hl5EYY5mEkXxU7TeXVYBsxh6ZiV59X1ovYqP68BE,4086
-kaiju_redis-2.1.4.dist-info/LICENSE,sha256=XIlN2qA8UqpBDA-PteoYP4hTU0qBW0G9PRB__khO2zc,610
-kaiju_redis-2.1.4.dist-info/METADATA,sha256=Lrakp3Z-xqAQ7si4mV6y-X_5OaEV4hwiu4NM1vYNq5U,3002
-kaiju_redis-2.1.4.dist-info/WHEEL,sha256=pkctZYzUS4AYVn6dJ-7367OJZivF2e8RA9b_ZBjif18,92
-kaiju_redis-2.1.4.dist-info/top_level.txt,sha256=-4Sc1VXkNcLW_b2uQWx-BICdwMu_NTUwDmt_q_SxB1Q,12
-kaiju_redis-2.1.4.dist-info/RECORD,,
+kaiju_redis/tests/fixtures.py,sha256=RGjqP_tMBC09WCtvJkFWufH-ZXWdVPll_P9SyEkjRYI,2980
+kaiju_redis/tests/test_redis.py,sha256=7Ka4G6XhMcoM571EciIf8_pB-An93kzj9TqzXoYqJQo,4433
+kaiju_redis-2.1.5.dist-info/LICENSE,sha256=XIlN2qA8UqpBDA-PteoYP4hTU0qBW0G9PRB__khO2zc,610
+kaiju_redis-2.1.5.dist-info/METADATA,sha256=CKuDsZqdnNSJkoZ6bteeHhhuC-_-jfflsS_onPyalcg,3116
+kaiju_redis-2.1.5.dist-info/WHEEL,sha256=pkctZYzUS4AYVn6dJ-7367OJZivF2e8RA9b_ZBjif18,92
+kaiju_redis-2.1.5.dist-info/top_level.txt,sha256=-4Sc1VXkNcLW_b2uQWx-BICdwMu_NTUwDmt_q_SxB1Q,12
+kaiju_redis-2.1.5.dist-info/RECORD,,
```

