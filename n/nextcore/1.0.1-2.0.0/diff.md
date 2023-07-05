# Comparing `tmp/nextcore-1.0.1.tar.gz` & `tmp/nextcore-2.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nextcore-1.0.1.tar", max compression
+gzip compressed data, was "nextcore-2.0.0.tar", max compression
```

## Comparing `nextcore-1.0.1.tar` & `nextcore-2.0.0.tar`

### file list

```diff
@@ -1,8 +1,41 @@
--rw-r--r--   0        0        0     1066 2021-10-31 16:43:29.428149 nextcore-1.0.1/LICENSE
--rw-r--r--   0        0        0       59 2021-10-31 16:44:28.447707 nextcore-1.0.1/README.md
--rw-r--r--   0        0        0       97 2021-10-31 17:23:28.998271 nextcore-1.0.1/nextcore/__init__.py
--rw-r--r--   0        0        0      100 2021-10-31 16:46:20.766885 nextcore-1.0.1/nextcore/errors.py
--rw-r--r--   0        0        0      173 2021-10-31 17:23:07.988410 nextcore-1.0.1/nextcore/unset.py
--rw-r--r--   0        0        0      415 2021-10-31 17:23:35.978225 nextcore-1.0.1/pyproject.toml
--rw-r--r--   0        0        0      632 2021-10-31 17:24:14.440737 nextcore-1.0.1/setup.py
--rw-r--r--   0        0        0      661 2021-10-31 17:24:14.440960 nextcore-1.0.1/PKG-INFO
+-rw-r--r--   0        0        0     1076 2023-07-05 17:53:36.135146 nextcore-2.0.0/LICENSE
+-rw-r--r--   0        0        0     2873 2023-07-05 17:53:36.135146 nextcore-2.0.0/README.md
+-rw-r--r--   0        0        0     1334 2023-07-05 17:53:36.139146 nextcore-2.0.0/nextcore/__init__.py
+-rw-r--r--   0        0        0     1550 2023-07-05 17:53:36.139146 nextcore-2.0.0/nextcore/common/__init__.py
+-rw-r--r--   0        0        0    19861 2023-07-05 17:53:36.139146 nextcore-2.0.0/nextcore/common/dispatcher.py
+-rw-r--r--   0        0        0     1453 2023-07-05 17:53:36.139146 nextcore-2.0.0/nextcore/common/errors.py
+-rw-r--r--   0        0        0     2432 2023-07-05 17:53:36.139146 nextcore-2.0.0/nextcore/common/json.py
+-rw-r--r--   0        0        0     2444 2023-07-05 17:53:36.139146 nextcore-2.0.0/nextcore/common/maybe_coro.py
+-rw-r--r--   0        0        0     1371 2023-07-05 17:53:36.139146 nextcore-2.0.0/nextcore/common/times_per/__init__.py
+-rw-r--r--   0        0        0     2140 2023-07-05 17:53:36.139146 nextcore-2.0.0/nextcore/common/times_per/priority_queue_container.py
+-rw-r--r--   0        0        0     6559 2023-07-05 17:53:36.139146 nextcore-2.0.0/nextcore/common/times_per/times_per.py
+-rw-r--r--   0        0        0     1797 2023-07-05 17:53:36.139146 nextcore-2.0.0/nextcore/common/undefined.py
+-rw-r--r--   0        0        0     1855 2023-07-05 17:53:36.139146 nextcore-2.0.0/nextcore/gateway/__init__.py
+-rw-r--r--   0        0        0     2540 2023-07-05 17:53:36.139146 nextcore-2.0.0/nextcore/gateway/close_code.py
+-rw-r--r--   0        0        0     3227 2023-07-05 17:53:36.139146 nextcore-2.0.0/nextcore/gateway/decompressor.py
+-rw-r--r--   0        0        0     3571 2023-07-05 17:53:36.139146 nextcore-2.0.0/nextcore/gateway/errors.py
+-rw-r--r--   0        0        0     2854 2023-07-05 17:53:36.139146 nextcore-2.0.0/nextcore/gateway/exponential_backoff.py
+-rw-r--r--   0        0        0     1935 2023-07-05 17:53:36.139146 nextcore-2.0.0/nextcore/gateway/op_code.py
+-rw-r--r--   0        0        0    34036 2023-07-05 17:53:36.139146 nextcore-2.0.0/nextcore/gateway/shard.py
+-rw-r--r--   0        0        0    13422 2023-07-05 17:53:36.139146 nextcore-2.0.0/nextcore/gateway/shard_manager.py
+-rw-r--r--   0        0        0     1548 2023-07-05 17:53:36.139146 nextcore-2.0.0/nextcore/http/__init__.py
+-rw-r--r--   0        0        0     1465 2023-07-05 17:53:36.139146 nextcore-2.0.0/nextcore/http/authentication/__init__.py
+-rw-r--r--   0        0        0     2765 2023-07-05 17:53:36.139146 nextcore-2.0.0/nextcore/http/authentication/base.py
+-rw-r--r--   0        0        0     2633 2023-07-05 17:53:36.139146 nextcore-2.0.0/nextcore/http/authentication/bearer.py
+-rw-r--r--   0        0        0     2918 2023-07-05 17:53:36.139146 nextcore-2.0.0/nextcore/http/authentication/bot.py
+-rw-r--r--   0        0        0    10011 2023-07-05 17:53:36.139146 nextcore-2.0.0/nextcore/http/bucket.py
+-rw-r--r--   0        0        0     2558 2023-07-05 17:53:36.139146 nextcore-2.0.0/nextcore/http/bucket_metadata.py
+-rw-r--r--   0        0        0     1153 2023-07-05 17:53:36.139146 nextcore-2.0.0/nextcore/http/client/__init__.py
+-rw-r--r--   0        0        0     1978 2023-07-05 17:53:36.143146 nextcore-2.0.0/nextcore/http/client/base_client.py
+-rw-r--r--   0        0        0    19632 2023-07-05 17:53:36.143146 nextcore-2.0.0/nextcore/http/client/client.py
+-rw-r--r--   0        0        0     5627 2023-07-05 17:53:36.143146 nextcore-2.0.0/nextcore/http/errors.py
+-rw-r--r--   0        0        0     1504 2023-07-05 17:53:36.143146 nextcore-2.0.0/nextcore/http/global_rate_limiter/__init__.py
+-rw-r--r--   0        0        0     3183 2023-07-05 17:53:36.143146 nextcore-2.0.0/nextcore/http/global_rate_limiter/base.py
+-rw-r--r--   0        0        0     2044 2023-07-05 17:53:36.143146 nextcore-2.0.0/nextcore/http/global_rate_limiter/limited.py
+-rw-r--r--   0        0        0     5929 2023-07-05 17:53:36.143146 nextcore-2.0.0/nextcore/http/global_rate_limiter/unlimited.py
+-rw-r--r--   0        0        0     6274 2023-07-05 17:53:36.143146 nextcore-2.0.0/nextcore/http/rate_limit_storage.py
+-rw-r--r--   0        0        0     2481 2023-07-05 17:53:36.143146 nextcore-2.0.0/nextcore/http/request_session.py
+-rw-r--r--   0        0        0     4133 2023-07-05 17:53:36.143146 nextcore-2.0.0/nextcore/http/route.py
+-rw-r--r--   0        0        0       85 2023-07-05 17:53:36.143146 nextcore-2.0.0/nextcore/py.typed
+-rw-r--r--   0        0        0     2476 2023-07-05 17:53:36.143146 nextcore-2.0.0/pyproject.toml
+-rw-r--r--   0        0        0     4507 1970-01-01 00:00:00.000000 nextcore-2.0.0/PKG-INFO
```

### Comparing `nextcore-1.0.1/LICENSE` & `nextcore-2.0.0/nextcore/http/client/__init__.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,21 +1,22 @@
-MIT License
+# The MIT License (MIT)
+# Copyright (c) 2021-present nextcore developers
+#
+# Permission is hereby granted, free of charge, to any person obtaining a
+# copy of this software and associated documentation files (the "Software"),
+# to deal in the Software without restriction, including without limitation
+# the rights to use, copy, modify, merge, publish, distribute, sublicense,
+# and/or sell copies of the Software, and to permit persons to whom the
+# Software is furnished to do so, subject to the following conditions:
+#
+# The above copyright notice and this permission notice shall be included in
+# all copies or substantial portions of the Software.
+#
+# THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS
+# OR IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
+# FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
+# AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
+# LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING
+# FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER
+# DEALINGS IN THE SOFTWARE.
 
-Copyright (c) 2021 vcokltfre
-
-Permission is hereby granted, free of charge, to any person obtaining a copy
-of this software and associated documentation files (the "Software"), to deal
-in the Software without restriction, including without limitation the rights
-to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
-copies of the Software, and to permit persons to whom the Software is
-furnished to do so, subject to the following conditions:
-
-The above copyright notice and this permission notice shall be included in all
-copies or substantial portions of the Software.
-
-THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
-IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
-FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
-AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
-LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
-OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
-SOFTWARE.
+from .client import *
```

