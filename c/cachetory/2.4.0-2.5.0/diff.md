# Comparing `tmp/cachetory-2.4.0.tar.gz` & `tmp/cachetory-2.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cachetory-2.4.0.tar", max compression
+gzip compressed data, was "cachetory-2.5.0.tar", max compression
```

## Comparing `cachetory-2.4.0.tar` & `cachetory-2.5.0.tar`

### file list

```diff
@@ -1,43 +1,43 @@
--rw-r--r--   0        0        0    11355 2023-07-04 13:44:57.849503 cachetory-2.4.0/LICENSE
--rw-r--r--   0        0        0    13582 2023-07-04 13:44:57.849503 cachetory-2.4.0/README.md
--rw-r--r--   0        0        0        0 2023-07-04 13:44:57.849503 cachetory-2.4.0/cachetory/__init__.py
--rw-r--r--   0        0        0       43 2023-07-04 13:44:57.849503 cachetory-2.4.0/cachetory/backends/__init__.py
--rw-r--r--   0        0        0      999 2023-07-04 13:44:57.849503 cachetory-2.4.0/cachetory/backends/async_/__init__.py
--rw-r--r--   0        0        0     1539 2023-07-04 13:44:57.849503 cachetory-2.4.0/cachetory/backends/async_/dummy.py
--rw-r--r--   0        0        0     1727 2023-07-04 13:44:57.849503 cachetory-2.4.0/cachetory/backends/async_/memory.py
--rw-r--r--   0        0        0     2502 2023-07-04 13:44:57.849503 cachetory-2.4.0/cachetory/backends/async_/redis.py
--rw-r--r--   0        0        0      993 2023-07-04 13:44:57.849503 cachetory-2.4.0/cachetory/backends/sync/__init__.py
--rw-r--r--   0        0        0     1427 2023-07-04 13:44:57.849503 cachetory-2.4.0/cachetory/backends/sync/dummy.py
--rw-r--r--   0        0        0     2361 2023-07-04 13:44:57.849503 cachetory-2.4.0/cachetory/backends/sync/memory.py
--rw-r--r--   0        0        0     2197 2023-07-04 13:44:57.849503 cachetory-2.4.0/cachetory/backends/sync/redis.py
--rw-r--r--   0        0        0       47 2023-07-04 13:44:57.849503 cachetory-2.4.0/cachetory/caches/__init__.py
--rw-r--r--   0        0        0     3631 2023-07-04 13:44:57.849503 cachetory-2.4.0/cachetory/caches/async_.py
--rw-r--r--   0        0        0      122 2023-07-04 13:44:57.849503 cachetory-2.4.0/cachetory/caches/private.py
--rw-r--r--   0        0        0     2978 2023-07-04 13:44:57.849503 cachetory-2.4.0/cachetory/caches/sync.py
--rw-r--r--   0        0        0        0 2023-07-04 13:44:57.849503 cachetory-2.4.0/cachetory/decorators/__init__.py
--rw-r--r--   0        0        0     2899 2023-07-04 13:44:57.849503 cachetory-2.4.0/cachetory/decorators/async_.py
--rw-r--r--   0        0        0      990 2023-07-04 13:44:57.849503 cachetory-2.4.0/cachetory/decorators/shared.py
--rw-r--r--   0        0        0     2539 2023-07-04 13:44:57.849503 cachetory-2.4.0/cachetory/decorators/sync.py
--rw-r--r--   0        0        0       41 2023-07-04 13:44:57.849503 cachetory-2.4.0/cachetory/interfaces/__init__.py
--rw-r--r--   0        0        0        0 2023-07-04 13:44:57.849503 cachetory-2.4.0/cachetory/interfaces/backends/__init__.py
--rw-r--r--   0        0        0     3644 2023-07-04 13:44:57.849503 cachetory-2.4.0/cachetory/interfaces/backends/async_.py
--rw-r--r--   0        0        0     1183 2023-07-04 13:44:57.849503 cachetory-2.4.0/cachetory/interfaces/backends/private.py
--rw-r--r--   0        0        0     3478 2023-07-04 13:44:57.849503 cachetory-2.4.0/cachetory/interfaces/backends/sync.py
--rw-r--r--   0        0        0     1598 2023-07-04 13:44:57.849503 cachetory-2.4.0/cachetory/interfaces/serializers.py
--rw-r--r--   0        0        0       67 2023-07-04 13:44:57.849503 cachetory-2.4.0/cachetory/private/__init__.py
--rw-r--r--   0        0        0      307 2023-07-04 13:44:57.849503 cachetory-2.4.0/cachetory/private/asyncio.py
--rw-r--r--   0        0        0      255 2023-07-04 13:44:57.849503 cachetory-2.4.0/cachetory/private/datetime.py
--rw-r--r--   0        0        0      618 2023-07-04 13:44:57.849503 cachetory-2.4.0/cachetory/private/functools.py
--rw-r--r--   0        0        0      205 2023-07-04 13:44:57.849503 cachetory-2.4.0/cachetory/private/typing.py
--rw-r--r--   0        0        0        0 2023-07-04 13:44:57.849503 cachetory-2.4.0/cachetory/py.typed
--rw-r--r--   0        0        0      402 2023-07-04 13:44:57.849503 cachetory-2.4.0/cachetory/serializers/__init__.py
--rw-r--r--   0        0        0     2718 2023-07-04 13:44:57.849503 cachetory-2.4.0/cachetory/serializers/chained.py
--rw-r--r--   0        0        0      326 2023-07-04 13:44:57.849503 cachetory-2.4.0/cachetory/serializers/compressors/__init__.py
--rw-r--r--   0        0        0     1026 2023-07-04 13:44:57.849503 cachetory-2.4.0/cachetory/serializers/compressors/zlib.py
--rw-r--r--   0        0        0     1248 2023-07-04 13:44:57.849503 cachetory-2.4.0/cachetory/serializers/compressors/zstd.py
--rw-r--r--   0        0        0      544 2023-07-04 13:44:57.849503 cachetory-2.4.0/cachetory/serializers/json.py
--rw-r--r--   0        0        0      608 2023-07-04 13:44:57.849503 cachetory-2.4.0/cachetory/serializers/msgpack.py
--rw-r--r--   0        0        0      538 2023-07-04 13:44:57.849503 cachetory-2.4.0/cachetory/serializers/noop.py
--rw-r--r--   0        0        0     1106 2023-07-04 13:44:57.849503 cachetory-2.4.0/cachetory/serializers/pickle.py
--rw-r--r--   0        0        0     3237 2023-07-04 13:45:11.665605 cachetory-2.4.0/pyproject.toml
--rw-r--r--   0        0        0    15097 1970-01-01 00:00:00.000000 cachetory-2.4.0/PKG-INFO
+-rw-r--r--   0        0        0    11355 2023-07-05 12:56:59.698513 cachetory-2.5.0/LICENSE
+-rw-r--r--   0        0        0    13890 2023-07-05 12:56:59.702513 cachetory-2.5.0/README.md
+-rw-r--r--   0        0        0        0 2023-07-05 12:56:59.702513 cachetory-2.5.0/cachetory/__init__.py
+-rw-r--r--   0        0        0       43 2023-07-05 12:56:59.702513 cachetory-2.5.0/cachetory/backends/__init__.py
+-rw-r--r--   0        0        0      999 2023-07-05 12:56:59.702513 cachetory-2.5.0/cachetory/backends/async_/__init__.py
+-rw-r--r--   0        0        0     1513 2023-07-05 12:56:59.702513 cachetory-2.5.0/cachetory/backends/async_/dummy.py
+-rw-r--r--   0        0        0     1711 2023-07-05 12:56:59.702513 cachetory-2.5.0/cachetory/backends/async_/memory.py
+-rw-r--r--   0        0        0     2476 2023-07-05 12:56:59.702513 cachetory-2.5.0/cachetory/backends/async_/redis.py
+-rw-r--r--   0        0        0      993 2023-07-05 12:56:59.702513 cachetory-2.5.0/cachetory/backends/sync/__init__.py
+-rw-r--r--   0        0        0     1401 2023-07-05 12:56:59.702513 cachetory-2.5.0/cachetory/backends/sync/dummy.py
+-rw-r--r--   0        0        0     2333 2023-07-05 12:56:59.702513 cachetory-2.5.0/cachetory/backends/sync/memory.py
+-rw-r--r--   0        0        0     2171 2023-07-05 12:56:59.702513 cachetory-2.5.0/cachetory/backends/sync/redis.py
+-rw-r--r--   0        0        0       47 2023-07-05 12:56:59.702513 cachetory-2.5.0/cachetory/caches/__init__.py
+-rw-r--r--   0        0        0     3631 2023-07-05 12:56:59.702513 cachetory-2.5.0/cachetory/caches/async_.py
+-rw-r--r--   0        0        0      122 2023-07-05 12:56:59.702513 cachetory-2.5.0/cachetory/caches/private.py
+-rw-r--r--   0        0        0     2978 2023-07-05 12:56:59.702513 cachetory-2.5.0/cachetory/caches/sync.py
+-rw-r--r--   0        0        0        0 2023-07-05 12:56:59.702513 cachetory-2.5.0/cachetory/decorators/__init__.py
+-rw-r--r--   0        0        0     3835 2023-07-05 12:56:59.702513 cachetory-2.5.0/cachetory/decorators/async_.py
+-rw-r--r--   0        0        0      990 2023-07-05 12:56:59.702513 cachetory-2.5.0/cachetory/decorators/shared.py
+-rw-r--r--   0        0        0     3318 2023-07-05 12:56:59.702513 cachetory-2.5.0/cachetory/decorators/sync.py
+-rw-r--r--   0        0        0       41 2023-07-05 12:56:59.702513 cachetory-2.5.0/cachetory/interfaces/__init__.py
+-rw-r--r--   0        0        0        0 2023-07-05 12:56:59.702513 cachetory-2.5.0/cachetory/interfaces/backends/__init__.py
+-rw-r--r--   0        0        0     3618 2023-07-05 12:56:59.702513 cachetory-2.5.0/cachetory/interfaces/backends/async_.py
+-rw-r--r--   0        0        0     1183 2023-07-05 12:56:59.702513 cachetory-2.5.0/cachetory/interfaces/backends/private.py
+-rw-r--r--   0        0        0     3452 2023-07-05 12:56:59.702513 cachetory-2.5.0/cachetory/interfaces/backends/sync.py
+-rw-r--r--   0        0        0     1598 2023-07-05 12:56:59.702513 cachetory-2.5.0/cachetory/interfaces/serializers.py
+-rw-r--r--   0        0        0       67 2023-07-05 12:56:59.702513 cachetory-2.5.0/cachetory/private/__init__.py
+-rw-r--r--   0        0        0      307 2023-07-05 12:56:59.702513 cachetory-2.5.0/cachetory/private/asyncio.py
+-rw-r--r--   0        0        0      255 2023-07-05 12:56:59.702513 cachetory-2.5.0/cachetory/private/datetime.py
+-rw-r--r--   0        0        0      909 2023-07-05 12:56:59.702513 cachetory-2.5.0/cachetory/private/functools.py
+-rw-r--r--   0        0        0      205 2023-07-05 12:56:59.702513 cachetory-2.5.0/cachetory/private/typing.py
+-rw-r--r--   0        0        0        0 2023-07-05 12:56:59.702513 cachetory-2.5.0/cachetory/py.typed
+-rw-r--r--   0        0        0      402 2023-07-05 12:56:59.702513 cachetory-2.5.0/cachetory/serializers/__init__.py
+-rw-r--r--   0        0        0     2718 2023-07-05 12:56:59.702513 cachetory-2.5.0/cachetory/serializers/chained.py
+-rw-r--r--   0        0        0      326 2023-07-05 12:56:59.702513 cachetory-2.5.0/cachetory/serializers/compressors/__init__.py
+-rw-r--r--   0        0        0     1026 2023-07-05 12:56:59.702513 cachetory-2.5.0/cachetory/serializers/compressors/zlib.py
+-rw-r--r--   0        0        0     1248 2023-07-05 12:56:59.702513 cachetory-2.5.0/cachetory/serializers/compressors/zstd.py
+-rw-r--r--   0        0        0      544 2023-07-05 12:56:59.702513 cachetory-2.5.0/cachetory/serializers/json.py
+-rw-r--r--   0        0        0      608 2023-07-05 12:56:59.702513 cachetory-2.5.0/cachetory/serializers/msgpack.py
+-rw-r--r--   0        0        0      538 2023-07-05 12:56:59.702513 cachetory-2.5.0/cachetory/serializers/noop.py
+-rw-r--r--   0        0        0     1106 2023-07-05 12:56:59.702513 cachetory-2.5.0/cachetory/serializers/pickle.py
+-rw-r--r--   0        0        0     3168 2023-07-05 12:57:12.926631 cachetory-2.5.0/pyproject.toml
+-rw-r--r--   0        0        0    15355 1970-01-01 00:00:00.000000 cachetory-2.5.0/PKG-INFO
```

### Comparing `cachetory-2.4.0/LICENSE` & `cachetory-2.5.0/LICENSE`

 * *Files identical despite different names*

### Comparing `cachetory-2.4.0/README.md` & `cachetory-2.5.0/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -137,23 +137,34 @@
     # `cache=lambda wrapped_callable, *args, **kwargs: cache if … else another_cache`
 
     # The following parameters are optional (shown the defaults):
     make_key=make_default_key,  # cache key generator
     time_to_live=None,  # forwarded to `Cache.set`
     if_not_exists=False,  # forwarded to `Cache.set`
 )
-def expensive_function() -> int:
-    return 42
+def expensive_function(x: int) -> int:
+    return 42 * x
 ```
 
-There's a few `make_key` functions provided by default:
+##### Key functions
+
+There are a few `make_key` functions provided by default:
 
 - `cachetory.decorators.shared.make_default_key` builds a human-readable cache key out of decorated function fully-qualified name and stringified arguments. The length of the key depends on the argument values.
 - `cachetory.decorators.shared.make_default_hashed_key` calls `make_default_key` under the hood but hashes the key and returns a hash hex digest – making it a fixed-length key and not human-readable.
 
+##### Purge cache
+
+Specific cached value can be deleted using the added `purge()` function, which accepts the same arguments as the original wrapped callable:
+
+```python
+expensive_function(100500)
+expensive_function.purge(100500)  # purge cached value for this argument
+```
+
 ## Supported backends
 
 The badges indicate which schemes are supported by a particular backend, and which package extras are required for it – if any:
 
 ### Redis
 
 ![scheme: redis](https://img.shields.io/badge/scheme-redis://-important)
```

### Comparing `cachetory-2.4.0/cachetory/backends/async_/__init__.py` & `cachetory-2.5.0/cachetory/backends/async_/__init__.py`

 * *Files identical despite different names*

### Comparing `cachetory-2.4.0/cachetory/backends/async_/dummy.py` & `cachetory-2.5.0/cachetory/backends/sync/dummy.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,47 +1,46 @@
 from __future__ import annotations
 
 from datetime import datetime, timedelta
-from typing import AsyncIterable, Generic, Iterable, Optional, Tuple
+from typing import Generic, Iterable
 
-from cachetory.interfaces.backends.async_ import AsyncBackend
 from cachetory.interfaces.backends.private import WireT
+from cachetory.interfaces.backends.sync import SyncBackend
 
 
-class DummyBackend(AsyncBackend[WireT], Generic[WireT]):
+class DummyBackend(SyncBackend[WireT], Generic[WireT]):
     """Dummy backend that stores nothing."""
 
     @classmethod
     def from_url(cls, url: str) -> DummyBackend:
         return DummyBackend()
 
-    async def get(self, key: str) -> WireT:  # pragma: no cover
+    def get(self, key: str) -> WireT:  # pragma: no cover
         raise KeyError(key)
 
-    async def get_many(self, *keys: str) -> AsyncIterable[Tuple[str, WireT]]:
-        for _ in ():  # pragma: no cover
-            yield ()  # type: ignore
+    def get_many(self, *keys: str) -> Iterable[tuple[str, WireT]]:  # pragma: no cover
+        return []
 
-    async def expire_in(self, key: str, time_to_live: Optional[timedelta] = None) -> None:  # pragma: no cover
+    def expire_in(self, key: str, time_to_live: timedelta | None = None) -> None:  # pragma: no cover
         return None
 
-    async def expire_at(self, key: str, deadline: Optional[datetime]) -> None:  # pragma: no cover
+    def expire_at(self, key: str, deadline: datetime | None) -> None:  # pragma: no cover
         return None
 
-    async def set(  # noqa: A003
+    def set(  # noqa: A003
         self,
         key: str,
         value: WireT,
         *,
-        time_to_live: Optional[timedelta] = None,
+        time_to_live: timedelta | None = None,
         if_not_exists: bool = False,
     ) -> bool:  # pragma: no cover
         return True
 
-    async def set_many(self, items: Iterable[Tuple[str, WireT]]) -> None:  # pragma: no cover
+    def set_many(self, items: Iterable[tuple[str, WireT]]) -> None:  # pragma: no cover
         return None
 
-    async def delete(self, key: str) -> bool:  # pragma: no cover
+    def delete(self, key: str) -> bool:  # pragma: no cover
         return False  # has never been there
 
-    async def clear(self) -> None:  # pragma: no cover
+    def clear(self) -> None:  # pragma: no cover
         return None  # already perfectly clean
```

### Comparing `cachetory-2.4.0/cachetory/backends/async_/memory.py` & `cachetory-2.5.0/cachetory/backends/async_/memory.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from __future__ import annotations
 
 from datetime import datetime, timedelta
-from typing import Any, Coroutine, Generic, Optional
+from typing import Any, Coroutine, Generic
 
 from cachetory.backends.sync.memory import MemoryBackend as SyncMemoryBackend
 from cachetory.interfaces.backends.async_ import AsyncBackend
 from cachetory.interfaces.backends.private import WireT
 from cachetory.private.asyncio import postpone
 
 
@@ -21,23 +21,23 @@
     def __init__(self) -> None:
         # We'll simply delegate call to the wrapped backend.
         self._inner: SyncMemoryBackend = SyncMemoryBackend()
 
     def get(self, key: str) -> Coroutine[Any, Any, WireT]:
         return postpone(self._inner.get, key)
 
-    def expire_at(self, key: str, deadline: Optional[datetime]) -> Coroutine[Any, Any, None]:
+    def expire_at(self, key: str, deadline: datetime | None) -> Coroutine[Any, Any, None]:
         return postpone(self._inner.expire_at, key, deadline)
 
     def set(  # noqa: A003
         self,
         key: str,
         value: WireT,
         *,
-        time_to_live: Optional[timedelta] = None,
+        time_to_live: timedelta | None = None,
         if_not_exists: bool = False,
     ) -> Coroutine[Any, Any, bool]:
         return postpone(
             self._inner.set,
             key,
             value,
             time_to_live=time_to_live,
```

### Comparing `cachetory-2.4.0/cachetory/backends/async_/redis.py` & `cachetory-2.5.0/cachetory/backends/async_/redis.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from __future__ import annotations
 
 import itertools
 from datetime import datetime, timedelta
-from typing import AsyncIterable, Iterable, Optional, Tuple
+from typing import AsyncIterable, Iterable
 
 from redis.asyncio import Redis
 
 from cachetory.interfaces.backends.async_ import AsyncBackend
 
 
 class RedisBackend(AsyncBackend[bytes]):
@@ -25,44 +25,44 @@
 
     async def get(self, key: str) -> bytes:
         data = await self._client.get(key)
         if data is not None:
             return data
         raise KeyError(key)
 
-    async def get_many(self, *keys: str) -> AsyncIterable[Tuple[str, bytes]]:
+    async def get_many(self, *keys: str) -> AsyncIterable[tuple[str, bytes]]:
         for key, value in zip(keys, await self._client.mget(*keys)):
             if value is not None:
                 yield key, value
 
-    async def expire_at(self, key: str, deadline: Optional[datetime]) -> None:
+    async def expire_at(self, key: str, deadline: datetime | None) -> None:
         if deadline:
             # One can pass `datetime` directly to `pexpireat`, but the latter
             # incorrectly converts datetime into timestamp.
             await self._client.pexpireat(key, int(deadline.timestamp() * 1000.0))
         else:
             await self._client.persist(key)
 
-    async def expire_in(self, key: str, time_to_live: Optional[timedelta] = None) -> None:
+    async def expire_in(self, key: str, time_to_live: timedelta | None = None) -> None:
         if time_to_live:
             await self._client.pexpire(key, time_to_live)
         else:
             await self._client.persist(key)
 
     async def set(  # noqa: A003
         self,
         key: str,
         value: bytes,
         *,
-        time_to_live: Optional[timedelta] = None,
+        time_to_live: timedelta | None = None,
         if_not_exists: bool = False,
     ) -> bool:
         return bool(await self._client.set(key, value, px=time_to_live, nx=if_not_exists))
 
-    async def set_many(self, items: Iterable[Tuple[str, bytes]]) -> None:
+    async def set_many(self, items: Iterable[tuple[str, bytes]]) -> None:
         await self._client.execute_command("MSET", *itertools.chain.from_iterable(items))
 
     async def delete(self, key: str) -> bool:
         return bool(await self._client.delete(key))
 
     async def clear(self) -> None:
         await self._client.flushdb()
```

### Comparing `cachetory-2.4.0/cachetory/backends/sync/__init__.py` & `cachetory-2.5.0/cachetory/backends/sync/__init__.py`

 * *Files identical despite different names*

### Comparing `cachetory-2.4.0/cachetory/backends/sync/dummy.py` & `cachetory-2.5.0/cachetory/backends/async_/dummy.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,46 +1,47 @@
 from __future__ import annotations
 
 from datetime import datetime, timedelta
-from typing import Generic, Iterable, Optional, Tuple
+from typing import AsyncIterable, Generic, Iterable
 
+from cachetory.interfaces.backends.async_ import AsyncBackend
 from cachetory.interfaces.backends.private import WireT
-from cachetory.interfaces.backends.sync import SyncBackend
 
 
-class DummyBackend(SyncBackend[WireT], Generic[WireT]):
+class DummyBackend(AsyncBackend[WireT], Generic[WireT]):
     """Dummy backend that stores nothing."""
 
     @classmethod
     def from_url(cls, url: str) -> DummyBackend:
         return DummyBackend()
 
-    def get(self, key: str) -> WireT:  # pragma: no cover
+    async def get(self, key: str) -> WireT:  # pragma: no cover
         raise KeyError(key)
 
-    def get_many(self, *keys: str) -> Iterable[Tuple[str, WireT]]:  # pragma: no cover
-        return []
+    async def get_many(self, *keys: str) -> AsyncIterable[tuple[str, WireT]]:
+        for _ in ():  # pragma: no cover
+            yield ()  # type: ignore
 
-    def expire_in(self, key: str, time_to_live: Optional[timedelta] = None) -> None:  # pragma: no cover
+    async def expire_in(self, key: str, time_to_live: timedelta | None = None) -> None:  # pragma: no cover
         return None
 
-    def expire_at(self, key: str, deadline: Optional[datetime]) -> None:  # pragma: no cover
+    async def expire_at(self, key: str, deadline: datetime | None) -> None:  # pragma: no cover
         return None
 
-    def set(  # noqa: A003
+    async def set(  # noqa: A003
         self,
         key: str,
         value: WireT,
         *,
-        time_to_live: Optional[timedelta] = None,
+        time_to_live: timedelta | None = None,
         if_not_exists: bool = False,
     ) -> bool:  # pragma: no cover
         return True
 
-    def set_many(self, items: Iterable[Tuple[str, WireT]]) -> None:  # pragma: no cover
+    async def set_many(self, items: Iterable[tuple[str, WireT]]) -> None:  # pragma: no cover
         return None
 
-    def delete(self, key: str) -> bool:  # pragma: no cover
+    async def delete(self, key: str) -> bool:  # pragma: no cover
         return False  # has never been there
 
-    def clear(self) -> None:  # pragma: no cover
+    async def clear(self) -> None:  # pragma: no cover
         return None  # already perfectly clean
```

### Comparing `cachetory-2.4.0/cachetory/backends/sync/memory.py` & `cachetory-2.5.0/cachetory/backends/sync/memory.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from __future__ import annotations
 
 from datetime import datetime, timedelta, timezone
-from typing import Dict, Generic, Optional
+from typing import Generic
 
 from cachetory.interfaces.backends.private import WireT
 from cachetory.interfaces.backends.sync import SyncBackend
 from cachetory.private.datetime import make_deadline
 
 
 class MemoryBackend(SyncBackend[WireT], Generic[WireT]):
@@ -14,33 +14,33 @@
     __slots__ = ("_entries",)
 
     @classmethod
     def from_url(cls, _url: str) -> MemoryBackend:
         return MemoryBackend()
 
     def __init__(self) -> None:
-        self._entries: Dict[str, _Entry[WireT]] = {}
+        self._entries: dict[str, _Entry[WireT]] = {}
 
     def get(self, key: str) -> WireT:
         return self._get_entry(key).value
 
-    def expire_at(self, key: str, deadline: Optional[datetime]) -> None:
+    def expire_at(self, key: str, deadline: datetime | None) -> None:
         try:
             entry = self._get_entry(key)
         except KeyError:
             pass
         else:
             entry.deadline = deadline
 
     def set(  # noqa: A003
         self,
         key: str,
         value: WireT,
         *,
-        time_to_live: Optional[timedelta] = None,
+        time_to_live: timedelta | None = None,
         if_not_exists: bool = False,
     ) -> bool:
         entry = _Entry[WireT](value, make_deadline(time_to_live))
         if if_not_exists:
             return self._entries.setdefault(key, entry) is entry
         else:
             self._entries[key] = _Entry[WireT](value, make_deadline(time_to_live))
@@ -64,17 +64,17 @@
         return len(self._entries)
 
 
 class _Entry(Generic[WireT]):
     """`mypy` doesn't support generic named tuples, thus defining this little one."""
 
     value: WireT
-    deadline: Optional[datetime]
+    deadline: datetime | None
 
     __slots__ = ("value", "deadline")
 
-    def __init__(self, value: WireT, deadline: Optional[datetime]) -> None:
+    def __init__(self, value: WireT, deadline: datetime | None) -> None:
         self.value = value
         self.deadline = deadline
 
 
 _SENTINEL = object()
```

### Comparing `cachetory-2.4.0/cachetory/backends/sync/redis.py` & `cachetory-2.5.0/cachetory/backends/sync/redis.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from __future__ import annotations
 
 import itertools
 from datetime import datetime, timedelta
-from typing import Iterable, Optional, Tuple
+from typing import Iterable
 
 from redis import Redis
 
 from cachetory.interfaces.backends.sync import SyncBackend
 
 
 class RedisBackend(SyncBackend[bytes]):
@@ -23,44 +23,44 @@
 
     def get(self, key: str) -> bytes:
         data = self._client.get(key)
         if data is not None:
             return data
         raise KeyError(key)
 
-    def get_many(self, *keys: str) -> Iterable[Tuple[str, bytes]]:
+    def get_many(self, *keys: str) -> Iterable[tuple[str, bytes]]:
         for key, value in zip(keys, self._client.mget(*keys)):
             if value is not None:
                 yield key, value
 
-    def expire_at(self, key: str, deadline: Optional[datetime]) -> None:
+    def expire_at(self, key: str, deadline: datetime | None) -> None:
         if deadline:
             # One can pass `datetime` directly to `pexpireat`, but the latter
             # incorrectly converts datetime into timestamp.
             self._client.pexpireat(key, int(deadline.timestamp() * 1000.0))
         else:
             self._client.persist(key)
 
-    def expire_in(self, key: str, time_to_live: Optional[timedelta] = None) -> None:
+    def expire_in(self, key: str, time_to_live: timedelta | None = None) -> None:
         if time_to_live:
             self._client.pexpire(key, time_to_live)
         else:
             self._client.persist(key)
 
     def set(  # noqa: A003
         self,
         key: str,
         value: bytes,
         *,
-        time_to_live: Optional[timedelta] = None,
+        time_to_live: timedelta | None = None,
         if_not_exists: bool = False,
     ) -> bool:
         return bool(self._client.set(key, value, px=time_to_live, nx=if_not_exists))
 
-    def set_many(self, items: Iterable[Tuple[str, bytes]]) -> None:
+    def set_many(self, items: Iterable[tuple[str, bytes]]) -> None:
         self._client.execute_command("MSET", *itertools.chain.from_iterable(items))
 
     def delete(self, key: str) -> bool:
         return bool(self._client.delete(key))
 
     def clear(self) -> None:
         self._client.flushdb()
```

### Comparing `cachetory-2.4.0/cachetory/caches/async_.py` & `cachetory-2.5.0/cachetory/caches/async_.py`

 * *Files identical despite different names*

### Comparing `cachetory-2.4.0/cachetory/caches/sync.py` & `cachetory-2.5.0/cachetory/caches/sync.py`

 * *Files identical despite different names*

### Comparing `cachetory-2.4.0/cachetory/decorators/async_.py` & `cachetory-2.5.0/cachetory/decorators/sync.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,66 +1,84 @@
 from __future__ import annotations
 
 from datetime import timedelta
 from functools import wraps
-from typing import Awaitable, Callable, Optional, Union
+from typing import Callable
 
-from typing_extensions import ParamSpec
+from typing_extensions import ParamSpec, Protocol
 
-from cachetory.caches.async_ import Cache
+from cachetory.caches.sync import Cache
 from cachetory.decorators import shared
 from cachetory.interfaces.backends.private import WireT
-from cachetory.interfaces.serializers import ValueT
-from cachetory.private.functools import maybe_awaitable, maybe_callable
+from cachetory.interfaces.serializers import ValueT, ValueT_co
+from cachetory.private.functools import into_callable
 
 P = ParamSpec("P")
-"""
-Original wrapped function parameter specification.
-"""
+"""Original wrapped function parameter specification."""
 
 
 def cached(
-    cache: Union[
-        Cache[ValueT, WireT],
-        Callable[..., Cache[ValueT, WireT]],
-        Callable[..., Awaitable[Cache[ValueT, WireT]]],
-    ],  # no way to use `P` here
+    cache: Cache[ValueT, WireT] | Callable[..., Cache[ValueT, WireT]],  # no way to use `P` here
     *,
     make_key: Callable[..., str] = shared.make_default_key,  # no way to use `P` here
-    time_to_live: Optional[timedelta | Callable[..., timedelta] | Callable[..., Awaitable[timedelta]]] = None,
+    time_to_live: timedelta | Callable[..., timedelta] | None = None,
     if_not_exists: bool = False,
-    exclude: None | Callable[[str, ValueT], bool] | Callable[[str, ValueT], Awaitable[bool]] = None,
-) -> Callable[[Callable[P, Awaitable[ValueT]]], Callable[P, Awaitable[ValueT]]]:
+    exclude: Callable[[str, ValueT], bool] | None = None,
+) -> Callable[[Callable[P, ValueT]], _CachedCallable[P, ValueT]]:
     """
     Apply memoization to the wrapped callable.
 
     Args:
         cache:
-            `Cache` instance or a callable (sync or async) that returns a `Cache` instance for each function call.
-            In the latter case the specific callable gets called with a wrapped function as the first argument,
+            `Cache` instance or a callable tha returns a `Cache` instance for each function call.
+            In the latter case the specified callable gets called with a wrapped function as the first argument,
             and the rest of the arguments next to it.
         make_key: callable to generate a custom cache key per each call.
         time_to_live:
-            cached value expiration time or a callable (sync or async) that returns the expiration time.
+            cached value expiration time or callable that returns the expiration time.
             The callable needs to accept keyword arguments, and it is given the cache key to
             compute the expiration time.
         if_not_exists: controls concurrent sets: if `True` – avoids overwriting a cached value.
         exclude: Optional callable to prevent a key-value pair from being cached if the callable returns true.
     """
 
-    def wrap(callable_: Callable[P, Awaitable[ValueT]]) -> Callable[P, Awaitable[ValueT]]:
+    def wrap(callable_: Callable[P, ValueT]) -> _CachedCallable[P, ValueT]:
+        get_cache = into_callable(cache)
+        get_time_to_live = into_callable(time_to_live)
+
         @wraps(callable_)
-        async def cached_callable(*args: P.args, **kwargs: P.kwargs) -> ValueT:
-            cache_ = await maybe_awaitable(maybe_callable(cache, callable_, *args, **kwargs))
+        def cached_callable(*args: P.args, **kwargs: P.kwargs) -> ValueT:
+            cache_ = get_cache(callable_, *args, **kwargs)
             key_ = make_key(callable_, *args, **kwargs)
-            time_to_live_ = await maybe_awaitable(maybe_callable(time_to_live, key=key_))
+            time_to_live_ = get_time_to_live(key=key_)
 
-            value = await cache_.get(key_)
-            if value is None:
-                value = await callable_(*args, **kwargs)
-                if exclude is None or not await maybe_awaitable(exclude(key_, value)):
-                    await cache_.set(key_, value, time_to_live=time_to_live_, if_not_exists=if_not_exists)
+            try:
+                value = cache_[key_]
+            except KeyError:
+                value = callable_(*args, **kwargs)
+                if exclude is None or not exclude(key_, value):
+                    cache_.set(key_, value, time_to_live=time_to_live_, if_not_exists=if_not_exists)
             return value
 
-        return cached_callable
+        def purge(*args: P.args, **kwargs: P.kwargs) -> bool:
+            key = make_key(callable_, *args, **kwargs)
+            return get_cache(callable_, *args, **kwargs).delete(key)
+
+        cached_callable.purge = purge  # type: ignore[attr-defined]
+        return cached_callable  # type: ignore[return-value]
 
     return wrap
+
+
+class _CachedCallable(Protocol[P, ValueT_co]):
+    """Protocol of the wrapped callable."""
+
+    def __call__(self, *args: P.args, **kwargs: P.kwargs) -> ValueT_co:
+        ...
+
+    def purge(self, *args: P.args, **kwargs: P.kwargs) -> bool:
+        """
+        Delete the value that was cached using the same call arguments.
+
+        Returns:
+            whether a cached value existed
+        """
```

### Comparing `cachetory-2.4.0/cachetory/decorators/shared.py` & `cachetory-2.5.0/cachetory/decorators/shared.py`

 * *Files identical despite different names*

### Comparing `cachetory-2.4.0/cachetory/interfaces/backends/async_.py` & `cachetory-2.5.0/cachetory/interfaces/backends/async_.py`

 * *Files 13% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 """
 
 from __future__ import annotations
 
 from abc import ABCMeta, abstractmethod
 from contextlib import AbstractAsyncContextManager
 from datetime import datetime, timedelta, timezone
-from typing import AsyncIterable, Generic, Iterable, Optional, Tuple
+from typing import AsyncIterable, Generic, Iterable
 
 from typing_extensions import Protocol
 
 from cachetory.interfaces.backends.private import WireT, WireT_co, WireT_contra
 
 
 class AsyncBackendRead(Protocol[WireT_co]):
@@ -28,15 +28,15 @@
             Cached value, if it exists.
 
         Raises:
             KeyError: the key doesn't exist in the cache.
         """
         raise NotImplementedError
 
-    async def get_many(self, *keys: str) -> AsyncIterable[Tuple[str, WireT_co]]:
+    async def get_many(self, *keys: str) -> AsyncIterable[tuple[str, WireT_co]]:
         """
         Get all the values corresponding to the specified keys.
 
         Returns:
             Existing key-value pairs.
         """
         for key in keys:
@@ -47,41 +47,41 @@
             else:
                 yield key, value
 
 
 class AsyncBackendWrite(Protocol[WireT_contra]):
     """Describes the write operations of an asynchronous cache."""
 
-    async def expire_in(self, key: str, time_to_live: Optional[timedelta] = None) -> None:
+    async def expire_in(self, key: str, time_to_live: timedelta | None = None) -> None:
         """Set the expiration time on the key."""
         deadline = datetime.now(timezone.utc) + time_to_live if time_to_live is not None else None
         await self.expire_at(key, deadline)
 
-    async def expire_at(self, key: str, deadline: Optional[datetime]) -> None:  # pragma: no cover
+    async def expire_at(self, key: str, deadline: datetime | None) -> None:  # pragma: no cover
         """Set the expiration deadline on the key."""
         raise NotImplementedError
 
     async def set(  # noqa: A003
         self,
         key: str,
         value: WireT_contra,
         *,
-        time_to_live: Optional[timedelta] = None,
+        time_to_live: timedelta | None = None,
         if_not_exists: bool = False,
     ) -> bool:  # pragma: no cover
         """
         Put the value into the cache.
 
         Returns:
             `True` if the value has been successfully set, `False` when `if_not_exists` is true
             and the key is already existing.
         """
         raise NotImplementedError
 
-    async def set_many(self, items: Iterable[Tuple[str, WireT_contra]]) -> None:
+    async def set_many(self, items: Iterable[tuple[str, WireT_contra]]) -> None:
         """Put all the specified values to the cache."""
         for key, value in items:
             await self.set(key, value)
 
     async def delete(self, key: str) -> bool:  # pragma: no cover
         """
         Delete the key from the cache.
```

### Comparing `cachetory-2.4.0/cachetory/interfaces/backends/private.py` & `cachetory-2.5.0/cachetory/interfaces/backends/private.py`

 * *Files identical despite different names*

### Comparing `cachetory-2.4.0/cachetory/interfaces/backends/sync.py` & `cachetory-2.5.0/cachetory/interfaces/backends/sync.py`

 * *Files 12% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 """
 
 from __future__ import annotations
 
 from abc import ABCMeta, abstractmethod
 from contextlib import AbstractContextManager
 from datetime import datetime, timedelta
-from typing import Generic, Iterable, Optional, Tuple
+from typing import Generic, Iterable
 
 from typing_extensions import Protocol
 
 from cachetory.interfaces.backends.private import WireT, WireT_co, WireT_contra
 from cachetory.private.datetime import make_deadline
 
 
@@ -29,15 +29,15 @@
             Cached value, if it exists.
 
         Raises:
             KeyError: the key does not exist.
         """
         raise NotImplementedError
 
-    def get_many(self, *keys: str) -> Iterable[Tuple[str, WireT_co]]:
+    def get_many(self, *keys: str) -> Iterable[tuple[str, WireT_co]]:
         """
         Get all the values corresponding to the specified keys.
 
         Returns:
             Existing key-value pairs.
         """
         for key in keys:
@@ -48,40 +48,40 @@
             else:
                 yield key, value
 
 
 class SyncBackendWrite(Protocol[WireT_contra]):
     """Describes the write operations of a synchronous cache."""
 
-    def expire_in(self, key: str, time_to_live: Optional[timedelta] = None) -> None:
+    def expire_in(self, key: str, time_to_live: timedelta | None = None) -> None:
         """Set the expiration time on the key."""
         self.expire_at(key, make_deadline(time_to_live))
 
-    def expire_at(self, key: str, deadline: Optional[datetime]) -> None:  # pragma: no cover
+    def expire_at(self, key: str, deadline: datetime | None) -> None:  # pragma: no cover
         """Set the expiration deadline on the key."""
         raise NotImplementedError
 
     def set(  # noqa: A003
         self,
         key: str,
         value: WireT_contra,
         *,
-        time_to_live: Optional[timedelta] = None,
+        time_to_live: timedelta | None = None,
         if_not_exists: bool = False,
     ) -> bool:  # pragma: no cover
         """
         Put the value into the cache.
 
         Returns:
             `True` if the value has been successfully set, `False` when `if_not_exists` is true
             and the key is already existing.
         """
         raise NotImplementedError
 
-    def set_many(self, items: Iterable[Tuple[str, WireT_contra]]) -> None:
+    def set_many(self, items: Iterable[tuple[str, WireT_contra]]) -> None:
         """Put all the specified values to the cache."""
         for key, value in items:
             self.set(key, value)
 
     def delete(self, key: str) -> bool:  # pragma: no cover
         """
         Delete the key from the cache.
```

### Comparing `cachetory-2.4.0/cachetory/interfaces/serializers.py` & `cachetory-2.5.0/cachetory/interfaces/serializers.py`

 * *Files identical despite different names*

### Comparing `cachetory-2.4.0/cachetory/serializers/chained.py` & `cachetory-2.5.0/cachetory/serializers/chained.py`

 * *Files identical despite different names*

### Comparing `cachetory-2.4.0/cachetory/serializers/compressors/zlib.py` & `cachetory-2.5.0/cachetory/serializers/compressors/zlib.py`

 * *Files identical despite different names*

### Comparing `cachetory-2.4.0/cachetory/serializers/compressors/zstd.py` & `cachetory-2.5.0/cachetory/serializers/compressors/zstd.py`

 * *Files identical despite different names*

### Comparing `cachetory-2.4.0/cachetory/serializers/json.py` & `cachetory-2.5.0/cachetory/serializers/json.py`

 * *Files identical despite different names*

### Comparing `cachetory-2.4.0/cachetory/serializers/msgpack.py` & `cachetory-2.5.0/cachetory/serializers/msgpack.py`

 * *Files identical despite different names*

### Comparing `cachetory-2.4.0/cachetory/serializers/noop.py` & `cachetory-2.5.0/cachetory/serializers/noop.py`

 * *Files identical despite different names*

### Comparing `cachetory-2.4.0/cachetory/serializers/pickle.py` & `cachetory-2.5.0/cachetory/serializers/pickle.py`

 * *Files identical despite different names*

### Comparing `cachetory-2.4.0/pyproject.toml` & `cachetory-2.5.0/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,41 +1,43 @@
+[project]
+requires-python = ">=3.8"
+
 [tool.poetry]
 authors = [
     "Pavel Perestoronin <pavel.perestoronin@kpn.com>",
 ]
 description = "Caching library with support for multiple cache backends"
 keywords = ["cache"]
 license = "Apache-2.0"
 name = "cachetory"
 readme = "README.md"
 repository = "https://github.com/kpn/cachetory"
-version = "2.4.0"
+version = "2.5.0"
 classifiers = [
     "Development Status :: 5 - Production/Stable",
     "Environment :: Web Environment",
     "Intended Audience :: Developers",
     "Operating System :: OS Independent",
     "Programming Language :: Python",
     "Programming Language :: Python :: 3",
     "Programming Language :: Python :: 3 :: Only",
-    "Programming Language :: Python :: 3.7",
     "Programming Language :: Python :: 3.8",
     "Programming Language :: Python :: 3.9",
     "Programming Language :: Python :: 3.10",
     "Programming Language :: Python :: 3.11",
     "Topic :: Internet :: WWW/HTTP",
     "Typing :: Typed",
 ]
 
 [build-system]
 requires = ["poetry-core", "poetry-dynamic-versioning"]
 build-backend = "poetry_dynamic_versioning.backend"
 
 [tool.poetry.dependencies]
-python = "^3.7.0"
+python = "^3.8.0"
 pydantic = "^1.10.4"
 typing-extensions = "^4.4.0"
 redis = {version = "^4.4.2", optional = true}
 zstd = {version = "^1.5.2.6", optional = true}
 ormsgpack = {version = "^1.2.6", optional = true, markers = "platform_python_implementation == 'CPython'"}
 
 [tool.poetry.extras]
@@ -104,17 +106,14 @@
     "D407",
     "D417",  # TODO: fix and enable
     "PT001",
     "PT011",
     "PT013",
     "RET505",
     "TRY003",
-    "UP006",  # 3.9
-    "UP007",  # 3.10
-    "UP033",  # 3.9
 ]
 unfixable = ["B"]
 
 [tool.ruff.per-file-ignores]
 "tests/*" = ["D101", "D102", "D106"]
 
 [tool.ruff.flake8-quotes]
```

### Comparing `cachetory-2.4.0/PKG-INFO` & `cachetory-2.5.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,25 +1,24 @@
 Metadata-Version: 2.1
 Name: cachetory
-Version: 2.4.0
+Version: 2.5.0
 Summary: Caching library with support for multiple cache backends
 Home-page: https://github.com/kpn/cachetory
 License: Apache-2.0
 Keywords: cache
 Author: Pavel Perestoronin
 Author-email: pavel.perestoronin@kpn.com
-Requires-Python: >=3.7.0,<4.0.0
+Requires-Python: >=3.8.0,<4.0.0
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Web Environment
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Topic :: Internet :: WWW/HTTP
 Classifier: Typing :: Typed
@@ -173,23 +172,34 @@
     # `cache=lambda wrapped_callable, *args, **kwargs: cache if … else another_cache`
 
     # The following parameters are optional (shown the defaults):
     make_key=make_default_key,  # cache key generator
     time_to_live=None,  # forwarded to `Cache.set`
     if_not_exists=False,  # forwarded to `Cache.set`
 )
-def expensive_function() -> int:
-    return 42
+def expensive_function(x: int) -> int:
+    return 42 * x
 ```
 
-There's a few `make_key` functions provided by default:
+##### Key functions
+
+There are a few `make_key` functions provided by default:
 
 - `cachetory.decorators.shared.make_default_key` builds a human-readable cache key out of decorated function fully-qualified name and stringified arguments. The length of the key depends on the argument values.
 - `cachetory.decorators.shared.make_default_hashed_key` calls `make_default_key` under the hood but hashes the key and returns a hash hex digest – making it a fixed-length key and not human-readable.
 
+##### Purge cache
+
+Specific cached value can be deleted using the added `purge()` function, which accepts the same arguments as the original wrapped callable:
+
+```python
+expensive_function(100500)
+expensive_function.purge(100500)  # purge cached value for this argument
+```
+
 ## Supported backends
 
 The badges indicate which schemes are supported by a particular backend, and which package extras are required for it – if any:
 
 ### Redis
 
 ![scheme: redis](https://img.shields.io/badge/scheme-redis://-important)
```

