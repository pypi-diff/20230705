# Comparing `tmp/pytest_async_generators-0.0.3.tar.gz` & `tmp/pytest_async_generators-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pytest_async_generators-0.0.3.tar", max compression
+gzip compressed data, was "pytest_async_generators-0.0.4.tar", max compression
```

## Comparing `pytest_async_generators-0.0.3.tar` & `pytest_async_generators-0.0.4.tar`

### file list

```diff
@@ -1,5 +1,5 @@
--rw-r--r--   0        0        0      876 2023-07-04 20:42:46.975820 pytest_async_generators-0.0.3/pyproject.toml
--rw-r--r--   0        0        0        0 2023-07-04 19:20:46.368349 pytest_async_generators-0.0.3/pytest_async_generators/__init__.py
--rw-r--r--   0        0        0     1919 2023-07-04 20:41:21.927064 pytest_async_generators-0.0.3/pytest_async_generators/subscribe_to_messages.py
--rw-r--r--   0        0        0     1036 2023-07-04 19:11:43.775589 pytest_async_generators-0.0.3/readme.md
--rw-r--r--   0        0        0     1583 1970-01-01 00:00:00.000000 pytest_async_generators-0.0.3/PKG-INFO
+-rw-r--r--   0        0        0      875 2023-07-05 00:31:01.282794 pytest_async_generators-0.0.4/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-07-04 19:20:46.368349 pytest_async_generators-0.0.4/pytest_async_generators/__init__.py
+-rw-r--r--   0        0        0     1606 2023-07-05 00:27:05.632520 pytest_async_generators-0.0.4/pytest_async_generators/subscribe_to_messages.py
+-rw-r--r--   0        0        0      783 2023-07-05 00:04:28.815690 pytest_async_generators-0.0.4/readme.md
+-rw-r--r--   0        0        0     1330 1970-01-01 00:00:00.000000 pytest_async_generators-0.0.4/PKG-INFO
```

### Comparing `pytest_async_generators-0.0.3/pyproject.toml` & `pytest_async_generators-0.0.4/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "pytest-async-generators"
-version = "0.0.3"
+version = "0.0.4"
 description = "Pytest fixtures for async generators"
 repository = "https://github.com/possibilities/pytest-async-generators"
 authors = ["Mike Bannister <notimpossiblemike@gmail.com>"]
 readme = "readme.md"
 packages = [{include = "pytest_async_generators"}]
 
 [tool.poetry.dependencies]
@@ -25,10 +25,9 @@
 
 [tool.pytest.ini_options]
 addopts = "--verbose --capture=no"
 
 [tool.poetry.plugins."pytest11"]
 "subscribe_to_messages" = "pytest_async_generators.subscribe_to_messages"
 
-
 [tool.mypy]
 disallow_untyped_defs = true
```

### Comparing `pytest_async_generators-0.0.3/pytest_async_generators/subscribe_to_messages.py` & `pytest_async_generators-0.0.4/pytest_async_generators/subscribe_to_messages.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,57 +1,51 @@
+import time
 import asyncio
+import typing
 import pytest_asyncio
 from dataclasses import dataclass
-from typing import List, Any, AsyncGenerator, Coroutine, Callable
 
 
 @dataclass
 class AsyncGeneratorSubscriber:
-    wait_for_messages: Callable[[], Coroutine[Any, Any, List[Any]]]
+    wait_for_messages: typing.Callable[
+        [], typing.Coroutine[typing.Any, typing.Any, typing.List[typing.Any]]
+    ]
 
 
 @pytest_asyncio.fixture
-async def subscribe_to_messages() -> Callable:
+async def subscribe_to_messages(timeout: float = 0.5) -> typing.Callable:
     async def _subscribe_to_messages(
-        generator: AsyncGenerator,
+        generator: typing.AsyncGenerator,
     ) -> AsyncGeneratorSubscriber:
         results = []
-        last_received_time = asyncio.get_event_loop().time()
 
         async def collector() -> None:
-            nonlocal last_received_time
-
-            value = await generator.asend(None)
-            results.append(value)
-            first_received_elapsed = (
-                asyncio.get_event_loop().time() - last_received_time
-            )
-            last_received_time = asyncio.get_event_loop().time()
-
+            start_time = time.time()
             while True:
                 try:
                     try:
+                        elapsed_time = time.time() - start_time
+                        remain_timeout = max(0, timeout - elapsed_time)
                         value = await asyncio.wait_for(
-                            generator.asend(None), first_received_elapsed * 1.25
+                            generator.asend(None), remain_timeout
                         )
                         results.append(value)
-                        last_received_time = asyncio.get_event_loop().time()
+                        start_time = time.time()
                     except asyncio.TimeoutError:
-                        if (
-                            asyncio.get_event_loop().time() - last_received_time
-                            > first_received_elapsed
-                        ):
-                            break
+                        break
                 except StopAsyncIteration:
                     break
                 except asyncio.CancelledError:
                     pass
 
         collector_task = asyncio.create_task(collector())
 
-        async def wait_for_messages() -> List[Any]:
+        async def wait_for_messages() -> typing.List[typing.Any]:
             await collector_task
             return results
 
+        print(999999)
+        await asyncio.sleep(timeout)
         return AsyncGeneratorSubscriber(wait_for_messages=wait_for_messages)
 
     return _subscribe_to_messages
```

### Comparing `pytest_async_generators-0.0.3/readme.md` & `pytest_async_generators-0.0.4/PKG-INFO`

 * *Files 26% similar despite different names*

```diff
@@ -1,27 +1,42 @@
+Metadata-Version: 2.1
+Name: pytest-async-generators
+Version: 0.0.4
+Summary: Pytest fixtures for async generators
+Home-page: https://github.com/possibilities/pytest-async-generators
+Author: Mike Bannister
+Author-email: notimpossiblemike@gmail.com
+Requires-Python: >=3.11,<4.0
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.11
+Requires-Dist: pytest-asyncio (>=0.21.0,<0.22.0)
+Project-URL: Repository, https://github.com/possibilities/pytest-async-generators
+Description-Content-Type: text/markdown
+
 # Pytest Async Generators
 
 Pytest fixtures for async generators
 
 ## Usage
 
-Invoke any async generator and call `wait_for_messages()` to retrieve the results.
+Invoke any async generator with `await subscribe_to_messages()` and then `await wait_for_messages()` to retrieve the results.
 
 ```
-async def count() -> AsyncGenerator[int, None]:
-    for n in range(10):
-        await asyncio.sleep(0.1)
-        yield n
+import asyncio
+import pytest
+from typing import AsyncGenerator, Callable
 
 
 @pytest.mark.asyncio
-async def test_counting(subscribe_to_messages) -> None:
+async def test_counting(subscribe_to_messages: Callable) -> None:
+    async def count() -> AsyncGenerator[int, None]:
+        for n in range(10):
+            await asyncio.sleep(0.1)
+            yield n
+
     subscription = await subscribe_to_messages(count())
     messages = await subscription.wait_for_messages()
     assert messages == [0, 1, 2, 3, 4, 5, 6, 7, 8, 9]
 ```
 
-Note that with real generators you might need to cause events to happen by adding more code after `subscribe_to_messages` and before calling `wait_for_messages`.
-
-## Caveats
+`subscribe_to_messages()` can be passed a `timeout` parameter to control how long to wait for new messages.
 
-The fixture assumes that each message takes approximately the same amount of time because the arrival time of the first message is used to determine the approximate timeout to wait before returning the collected messages. If your generators don't work this way this plugin will make yowon't work correctly and will make you sad.
```

