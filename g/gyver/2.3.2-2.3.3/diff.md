# Comparing `tmp/gyver-2.3.2.tar.gz` & `tmp/gyver-2.3.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gyver-2.3.2.tar", max compression
+gzip compressed data, was "gyver-2.3.3.tar", max compression
```

## Comparing `gyver-2.3.2.tar` & `gyver-2.3.3.tar`

### file list

```diff
@@ -1,97 +1,97 @@
--rw-r--r--   0        0        0     1079 2023-06-20 21:41:14.557536 gyver-2.3.2/LICENSE
--rw-r--r--   0        0        0     1005 2023-06-20 21:41:14.557536 gyver-2.3.2/README.md
--rw-r--r--   0        0        0      158 2023-06-29 13:49:38.481507 gyver-2.3.2/gyver/__init__.py
--rw-r--r--   0        0        0      359 2023-06-20 21:41:14.559536 gyver-2.3.2/gyver/cache/__init__.py
--rw-r--r--   0        0        0     1201 2023-06-20 21:41:14.559536 gyver-2.3.2/gyver/cache/asyncio.py
--rw-r--r--   0        0        0      237 2023-06-20 21:41:14.559536 gyver-2.3.2/gyver/cache/config.py
--rw-r--r--   0        0        0     1776 2023-06-20 21:41:14.559536 gyver-2.3.2/gyver/cache/interface.py
--rw-r--r--   0        0        0     1395 2023-06-20 21:41:14.559536 gyver-2.3.2/gyver/cache/mapper.py
--rw-r--r--   0        0        0     5993 2023-06-20 21:41:14.559536 gyver-2.3.2/gyver/cache/mock.py
--rw-r--r--   0        0        0     4283 2023-06-20 21:41:14.559536 gyver-2.3.2/gyver/cache/redis.py
--rw-r--r--   0        0        0     1128 2023-06-20 21:41:14.559536 gyver-2.3.2/gyver/cache/sync.py
--rw-r--r--   0        0        0      558 2023-06-20 21:41:14.559536 gyver-2.3.2/gyver/cache/utils.py
--rw-r--r--   0        0        0      597 2023-06-27 06:41:36.152386 gyver-2.3.2/gyver/config/__init__.py
--rw-r--r--   0        0        0       78 2023-06-20 21:41:14.559536 gyver-2.3.2/gyver/config/adapter/__init__.py
--rw-r--r--   0        0        0     1320 2023-06-20 21:41:14.559536 gyver-2.3.2/gyver/config/adapter/attrs.py
--rw-r--r--   0        0        0     1078 2023-06-20 21:41:14.560536 gyver-2.3.2/gyver/config/adapter/dataclass.py
--rw-r--r--   0        0        0     5940 2023-06-27 06:41:36.152386 gyver-2.3.2/gyver/config/adapter/factory.py
--rw-r--r--   0        0        0     1056 2023-06-20 21:41:14.560536 gyver-2.3.2/gyver/config/adapter/gattrs.py
--rw-r--r--   0        0        0     2107 2023-06-20 21:41:14.560536 gyver-2.3.2/gyver/config/adapter/interface.py
--rw-r--r--   0        0        0     1701 2023-06-20 21:41:14.560536 gyver-2.3.2/gyver/config/adapter/mark.py
--rw-r--r--   0        0        0     1091 2023-06-20 21:41:14.560536 gyver-2.3.2/gyver/config/adapter/pydantic.py
--rw-r--r--   0        0        0     3459 2023-06-27 06:41:36.152386 gyver-2.3.2/gyver/config/config.py
--rw-r--r--   0        0        0     2690 2023-06-27 06:41:36.152386 gyver-2.3.2/gyver/config/envconfig.py
--rw-r--r--   0        0        0     1016 2023-06-27 06:41:36.152386 gyver-2.3.2/gyver/config/interface.py
--rw-r--r--   0        0        0     5534 2023-06-27 06:41:36.152386 gyver-2.3.2/gyver/config/lazy.py
--rw-r--r--   0        0        0      627 2023-06-27 06:41:36.152386 gyver-2.3.2/gyver/config/typedef.py
--rw-r--r--   0        0        0      473 2023-06-20 21:41:14.560536 gyver-2.3.2/gyver/config/utils.py
--rw-r--r--   0        0        0      419 2023-06-20 21:41:14.560536 gyver-2.3.2/gyver/context/__init__.py
--rw-r--r--   0        0        0      288 2023-06-20 21:41:14.560536 gyver-2.3.2/gyver/context/atomic_/__init__.py
--rw-r--r--   0        0        0     2317 2023-06-20 21:41:14.561536 gyver-2.3.2/gyver/context/atomic_/bound.py
--rw-r--r--   0        0        0     2493 2023-06-20 21:41:14.561536 gyver-2.3.2/gyver/context/atomic_/core.py
--rw-r--r--   0        0        0     1332 2023-06-20 21:41:14.561536 gyver-2.3.2/gyver/context/atomic_/resolver.py
--rw-r--r--   0        0        0     5659 2023-06-20 21:41:14.561536 gyver-2.3.2/gyver/context/context.py
--rw-r--r--   0        0        0      102 2023-06-20 21:41:14.561536 gyver-2.3.2/gyver/context/interfaces/__init__.py
--rw-r--r--   0        0        0     1525 2023-06-20 21:41:14.561536 gyver-2.3.2/gyver/context/interfaces/adapter.py
--rw-r--r--   0        0        0       39 2023-06-20 21:41:14.561536 gyver-2.3.2/gyver/context/typedef.py
--rw-r--r--   0        0        0      253 2023-06-20 21:41:14.561536 gyver-2.3.2/gyver/crypto/__init__.py
--rw-r--r--   0        0        0      133 2023-06-20 21:41:14.561536 gyver-2.3.2/gyver/crypto/config.py
--rw-r--r--   0        0        0      909 2023-06-20 21:41:14.561536 gyver-2.3.2/gyver/crypto/fernet.py
--rw-r--r--   0        0        0     1856 2023-06-20 21:41:14.561536 gyver-2.3.2/gyver/crypto/rsa.py
--rw-r--r--   0        0        0      749 2023-06-20 21:41:14.561536 gyver-2.3.2/gyver/database/__init__.py
--rw-r--r--   0        0        0     2136 2023-06-20 21:41:14.561536 gyver-2.3.2/gyver/database/adapter.py
--rw-r--r--   0        0        0     1233 2023-06-20 21:41:14.562536 gyver-2.3.2/gyver/database/config.py
--rw-r--r--   0        0        0      360 2023-06-20 21:41:14.562536 gyver-2.3.2/gyver/database/context/__init__.py
--rw-r--r--   0        0        0     3542 2023-06-20 21:41:14.562536 gyver-2.3.2/gyver/database/context/asyncio.py
--rw-r--r--   0        0        0     3349 2023-06-20 21:41:14.562536 gyver-2.3.2/gyver/database/context/sync.py
--rw-r--r--   0        0        0      170 2023-06-20 21:41:14.562536 gyver-2.3.2/gyver/database/drivers/__init__.py
--rw-r--r--   0        0        0      229 2023-06-20 21:41:14.562536 gyver-2.3.2/gyver/database/drivers/dialect.py
--rw-r--r--   0        0        0      224 2023-06-20 21:41:14.562536 gyver-2.3.2/gyver/database/drivers/interface.py
--rw-r--r--   0        0        0     1493 2023-06-20 21:41:14.562536 gyver-2.3.2/gyver/database/drivers/utils.py
--rw-r--r--   0        0        0     1076 2023-06-20 21:41:14.562536 gyver-2.3.2/gyver/database/entity.py
--rw-r--r--   0        0        0      498 2023-06-20 21:41:14.562536 gyver-2.3.2/gyver/database/entity.pyi
--rw-r--r--   0        0        0       50 2023-06-20 21:41:14.562536 gyver-2.3.2/gyver/database/metadata.py
--rw-r--r--   0        0        0     1012 2023-06-20 21:41:14.562536 gyver-2.3.2/gyver/database/query/__init__.py
--rw-r--r--   0        0        0     1692 2023-06-20 21:41:14.562536 gyver-2.3.2/gyver/database/query/_helpers.py
--rw-r--r--   0        0        0     2935 2023-06-20 21:41:14.563536 gyver-2.3.2/gyver/database/query/comp.py
--rw-r--r--   0        0        0      294 2023-06-20 21:41:14.563536 gyver-2.3.2/gyver/database/query/exc.py
--rw-r--r--   0        0        0     1220 2023-06-29 13:49:12.116121 gyver-2.3.2/gyver/database/query/interface.py
--rw-r--r--   0        0        0      279 2023-06-20 21:41:14.563536 gyver-2.3.2/gyver/database/query/null.py
--rw-r--r--   0        0        0     1270 2023-06-20 21:41:14.563536 gyver-2.3.2/gyver/database/query/order_by.py
--rw-r--r--   0        0        0     1239 2023-06-20 21:41:14.563536 gyver-2.3.2/gyver/database/query/paginate.py
--rw-r--r--   0        0        0      697 2023-06-20 21:41:14.563536 gyver-2.3.2/gyver/database/query/utils.py
--rw-r--r--   0        0        0     4613 2023-06-20 21:41:14.563536 gyver-2.3.2/gyver/database/query/where.py
--rw-r--r--   0        0        0      327 2023-06-20 21:41:14.563536 gyver-2.3.2/gyver/database/typedef.py
--rw-r--r--   0        0        0     4243 2023-06-20 21:41:14.563536 gyver-2.3.2/gyver/database/utils.py
--rw-r--r--   0        0        0     2272 2023-06-27 06:41:36.152386 gyver-2.3.2/gyver/exc.py
--rw-r--r--   0        0        0      225 2023-06-20 21:52:51.019089 gyver-2.3.2/gyver/filetree/__init__.py
--rw-r--r--   0        0        0     1749 2023-06-20 21:41:14.563536 gyver-2.3.2/gyver/filetree/filetree.py
--rw-r--r--   0        0        0      348 2023-06-20 21:41:14.563536 gyver-2.3.2/gyver/filetree/helpers.py
--rw-r--r--   0        0        0     3107 2023-06-27 06:41:36.153386 gyver-2.3.2/gyver/filetree/interface.py
--rw-r--r--   0        0        0     2503 2023-06-27 06:41:36.153386 gyver-2.3.2/gyver/filetree/typedef.py
--rw-r--r--   0        0        0     2808 2023-06-27 06:41:36.153386 gyver-2.3.2/gyver/filetree/virtual.py
--rw-r--r--   0        0        0      857 2023-06-20 21:41:14.563536 gyver-2.3.2/gyver/model.py
--rw-r--r--   0        0        0      101 2023-06-20 21:41:14.564536 gyver-2.3.2/gyver/pools/__init__.py
--rw-r--r--   0        0        0     5764 2023-06-20 21:41:14.564536 gyver-2.3.2/gyver/pools/asyncio.py
--rw-r--r--   0        0        0     2225 2023-06-20 21:41:14.564536 gyver-2.3.2/gyver/pools/resource.py
--rw-r--r--   0        0        0     3855 2023-06-20 21:41:14.564536 gyver-2.3.2/gyver/pools/thread.py
--rw-r--r--   0        0        0        0 2023-06-20 21:41:14.564536 gyver-2.3.2/gyver/py.typed
--rw-r--r--   0        0        0      186 2023-06-20 21:41:14.564536 gyver-2.3.2/gyver/url/__init__.py
--rw-r--r--   0        0        0     4663 2023-06-27 06:41:36.153386 gyver-2.3.2/gyver/url/core.py
--rw-r--r--   0        0        0      423 2023-06-20 21:41:14.564536 gyver-2.3.2/gyver/url/encode.py
--rw-r--r--   0        0        0     1285 2023-06-27 06:41:36.153386 gyver-2.3.2/gyver/url/fragment.py
--rw-r--r--   0        0        0     5566 2023-06-27 06:41:36.153386 gyver-2.3.2/gyver/url/netloc.py
--rw-r--r--   0        0        0     4307 2023-06-27 06:41:36.153386 gyver-2.3.2/gyver/url/path.py
--rw-r--r--   0        0        0     3592 2023-06-27 06:41:36.153386 gyver-2.3.2/gyver/url/query.py
--rw-r--r--   0        0        0     1186 2023-06-27 06:41:36.153386 gyver-2.3.2/gyver/url/utils.py
--rw-r--r--   0        0        0      726 2023-06-20 21:41:14.565536 gyver-2.3.2/gyver/utils/__init__.py
--rw-r--r--   0        0        0      156 2023-06-20 21:41:14.565536 gyver-2.3.2/gyver/utils/exc.py
--rw-r--r--   0        0        0     7836 2023-06-20 21:41:14.565536 gyver-2.3.2/gyver/utils/finder.py
--rw-r--r--   0        0        0     4262 2023-06-27 06:41:36.153386 gyver-2.3.2/gyver/utils/helpers.py
--rw-r--r--   0        0        0      174 2023-06-20 21:41:14.565536 gyver-2.3.2/gyver/utils/json.py
--rw-r--r--   0        0        0     2574 2023-06-27 06:41:36.154386 gyver-2.3.2/gyver/utils/lazy.py
--rw-r--r--   0        0        0     1319 2023-06-20 21:41:14.565536 gyver-2.3.2/gyver/utils/singleton.py
--rw-r--r--   0        0        0     2224 2023-06-27 06:41:36.154386 gyver-2.3.2/gyver/utils/strings.py
--rw-r--r--   0        0        0      134 2023-06-27 06:41:36.154386 gyver-2.3.2/gyver/utils/timezone.py
--rw-r--r--   0        0        0     2456 2023-06-29 13:49:38.480507 gyver-2.3.2/pyproject.toml
--rw-r--r--   0        0        0     2553 1970-01-01 00:00:00.000000 gyver-2.3.2/PKG-INFO
+-rw-r--r--   0        0        0     1079 2023-06-20 21:41:14.557536 gyver-2.3.3/LICENSE
+-rw-r--r--   0        0        0     1005 2023-06-20 21:41:14.557536 gyver-2.3.3/README.md
+-rw-r--r--   0        0        0      158 2023-07-05 16:04:22.222621 gyver-2.3.3/gyver/__init__.py
+-rw-r--r--   0        0        0      359 2023-06-20 21:41:14.559536 gyver-2.3.3/gyver/cache/__init__.py
+-rw-r--r--   0        0        0     1201 2023-06-20 21:41:14.559536 gyver-2.3.3/gyver/cache/asyncio.py
+-rw-r--r--   0        0        0      237 2023-06-20 21:41:14.559536 gyver-2.3.3/gyver/cache/config.py
+-rw-r--r--   0        0        0     1776 2023-06-20 21:41:14.559536 gyver-2.3.3/gyver/cache/interface.py
+-rw-r--r--   0        0        0     1395 2023-06-20 21:41:14.559536 gyver-2.3.3/gyver/cache/mapper.py
+-rw-r--r--   0        0        0     5993 2023-06-20 21:41:14.559536 gyver-2.3.3/gyver/cache/mock.py
+-rw-r--r--   0        0        0     4283 2023-06-20 21:41:14.559536 gyver-2.3.3/gyver/cache/redis.py
+-rw-r--r--   0        0        0     1128 2023-06-20 21:41:14.559536 gyver-2.3.3/gyver/cache/sync.py
+-rw-r--r--   0        0        0      558 2023-06-20 21:41:14.559536 gyver-2.3.3/gyver/cache/utils.py
+-rw-r--r--   0        0        0      597 2023-06-27 06:41:36.152386 gyver-2.3.3/gyver/config/__init__.py
+-rw-r--r--   0        0        0       78 2023-06-20 21:41:14.559536 gyver-2.3.3/gyver/config/adapter/__init__.py
+-rw-r--r--   0        0        0     1320 2023-06-20 21:41:14.559536 gyver-2.3.3/gyver/config/adapter/attrs.py
+-rw-r--r--   0        0        0     1078 2023-06-20 21:41:14.560536 gyver-2.3.3/gyver/config/adapter/dataclass.py
+-rw-r--r--   0        0        0     5940 2023-06-27 06:41:36.152386 gyver-2.3.3/gyver/config/adapter/factory.py
+-rw-r--r--   0        0        0     1056 2023-06-20 21:41:14.560536 gyver-2.3.3/gyver/config/adapter/gattrs.py
+-rw-r--r--   0        0        0     2107 2023-06-20 21:41:14.560536 gyver-2.3.3/gyver/config/adapter/interface.py
+-rw-r--r--   0        0        0     1701 2023-06-20 21:41:14.560536 gyver-2.3.3/gyver/config/adapter/mark.py
+-rw-r--r--   0        0        0     1091 2023-06-20 21:41:14.560536 gyver-2.3.3/gyver/config/adapter/pydantic.py
+-rw-r--r--   0        0        0     3459 2023-06-27 06:41:36.152386 gyver-2.3.3/gyver/config/config.py
+-rw-r--r--   0        0        0     2690 2023-06-27 06:41:36.152386 gyver-2.3.3/gyver/config/envconfig.py
+-rw-r--r--   0        0        0     1016 2023-06-27 06:41:36.152386 gyver-2.3.3/gyver/config/interface.py
+-rw-r--r--   0        0        0     5534 2023-06-27 06:41:36.152386 gyver-2.3.3/gyver/config/lazy.py
+-rw-r--r--   0        0        0      627 2023-06-27 06:41:36.152386 gyver-2.3.3/gyver/config/typedef.py
+-rw-r--r--   0        0        0      473 2023-06-20 21:41:14.560536 gyver-2.3.3/gyver/config/utils.py
+-rw-r--r--   0        0        0      419 2023-06-20 21:41:14.560536 gyver-2.3.3/gyver/context/__init__.py
+-rw-r--r--   0        0        0      288 2023-06-20 21:41:14.560536 gyver-2.3.3/gyver/context/atomic_/__init__.py
+-rw-r--r--   0        0        0     2317 2023-06-20 21:41:14.561536 gyver-2.3.3/gyver/context/atomic_/bound.py
+-rw-r--r--   0        0        0     2493 2023-06-20 21:41:14.561536 gyver-2.3.3/gyver/context/atomic_/core.py
+-rw-r--r--   0        0        0     1332 2023-06-20 21:41:14.561536 gyver-2.3.3/gyver/context/atomic_/resolver.py
+-rw-r--r--   0        0        0     5659 2023-06-20 21:41:14.561536 gyver-2.3.3/gyver/context/context.py
+-rw-r--r--   0        0        0      102 2023-06-20 21:41:14.561536 gyver-2.3.3/gyver/context/interfaces/__init__.py
+-rw-r--r--   0        0        0     1525 2023-06-20 21:41:14.561536 gyver-2.3.3/gyver/context/interfaces/adapter.py
+-rw-r--r--   0        0        0       39 2023-06-20 21:41:14.561536 gyver-2.3.3/gyver/context/typedef.py
+-rw-r--r--   0        0        0      253 2023-06-20 21:41:14.561536 gyver-2.3.3/gyver/crypto/__init__.py
+-rw-r--r--   0        0        0      133 2023-06-20 21:41:14.561536 gyver-2.3.3/gyver/crypto/config.py
+-rw-r--r--   0        0        0      909 2023-06-20 21:41:14.561536 gyver-2.3.3/gyver/crypto/fernet.py
+-rw-r--r--   0        0        0     1856 2023-06-20 21:41:14.561536 gyver-2.3.3/gyver/crypto/rsa.py
+-rw-r--r--   0        0        0      749 2023-06-20 21:41:14.561536 gyver-2.3.3/gyver/database/__init__.py
+-rw-r--r--   0        0        0     2136 2023-06-20 21:41:14.561536 gyver-2.3.3/gyver/database/adapter.py
+-rw-r--r--   0        0        0     1233 2023-06-20 21:41:14.562536 gyver-2.3.3/gyver/database/config.py
+-rw-r--r--   0        0        0      360 2023-06-20 21:41:14.562536 gyver-2.3.3/gyver/database/context/__init__.py
+-rw-r--r--   0        0        0     3542 2023-06-20 21:41:14.562536 gyver-2.3.3/gyver/database/context/asyncio.py
+-rw-r--r--   0        0        0     3349 2023-06-20 21:41:14.562536 gyver-2.3.3/gyver/database/context/sync.py
+-rw-r--r--   0        0        0      170 2023-06-20 21:41:14.562536 gyver-2.3.3/gyver/database/drivers/__init__.py
+-rw-r--r--   0        0        0      229 2023-06-20 21:41:14.562536 gyver-2.3.3/gyver/database/drivers/dialect.py
+-rw-r--r--   0        0        0      224 2023-06-20 21:41:14.562536 gyver-2.3.3/gyver/database/drivers/interface.py
+-rw-r--r--   0        0        0     1493 2023-06-20 21:41:14.562536 gyver-2.3.3/gyver/database/drivers/utils.py
+-rw-r--r--   0        0        0     1076 2023-06-20 21:41:14.562536 gyver-2.3.3/gyver/database/entity.py
+-rw-r--r--   0        0        0      498 2023-06-20 21:41:14.562536 gyver-2.3.3/gyver/database/entity.pyi
+-rw-r--r--   0        0        0       50 2023-06-20 21:41:14.562536 gyver-2.3.3/gyver/database/metadata.py
+-rw-r--r--   0        0        0     1012 2023-06-20 21:41:14.562536 gyver-2.3.3/gyver/database/query/__init__.py
+-rw-r--r--   0        0        0     1692 2023-06-20 21:41:14.562536 gyver-2.3.3/gyver/database/query/_helpers.py
+-rw-r--r--   0        0        0     2935 2023-06-20 21:41:14.563536 gyver-2.3.3/gyver/database/query/comp.py
+-rw-r--r--   0        0        0      294 2023-06-20 21:41:14.563536 gyver-2.3.3/gyver/database/query/exc.py
+-rw-r--r--   0        0        0     1220 2023-06-29 13:49:12.116121 gyver-2.3.3/gyver/database/query/interface.py
+-rw-r--r--   0        0        0      279 2023-06-20 21:41:14.563536 gyver-2.3.3/gyver/database/query/null.py
+-rw-r--r--   0        0        0     1270 2023-06-20 21:41:14.563536 gyver-2.3.3/gyver/database/query/order_by.py
+-rw-r--r--   0        0        0     1239 2023-06-20 21:41:14.563536 gyver-2.3.3/gyver/database/query/paginate.py
+-rw-r--r--   0        0        0      697 2023-06-20 21:41:14.563536 gyver-2.3.3/gyver/database/query/utils.py
+-rw-r--r--   0        0        0     4613 2023-06-20 21:41:14.563536 gyver-2.3.3/gyver/database/query/where.py
+-rw-r--r--   0        0        0      327 2023-06-20 21:41:14.563536 gyver-2.3.3/gyver/database/typedef.py
+-rw-r--r--   0        0        0     4243 2023-06-20 21:41:14.563536 gyver-2.3.3/gyver/database/utils.py
+-rw-r--r--   0        0        0     2272 2023-06-27 06:41:36.152386 gyver-2.3.3/gyver/exc.py
+-rw-r--r--   0        0        0      225 2023-06-20 21:52:51.019089 gyver-2.3.3/gyver/filetree/__init__.py
+-rw-r--r--   0        0        0     1749 2023-06-20 21:41:14.563536 gyver-2.3.3/gyver/filetree/filetree.py
+-rw-r--r--   0        0        0      348 2023-06-20 21:41:14.563536 gyver-2.3.3/gyver/filetree/helpers.py
+-rw-r--r--   0        0        0     3248 2023-07-05 16:03:52.217431 gyver-2.3.3/gyver/filetree/interface.py
+-rw-r--r--   0        0        0     2503 2023-06-27 06:41:36.153386 gyver-2.3.3/gyver/filetree/typedef.py
+-rw-r--r--   0        0        0     2808 2023-06-27 06:41:36.153386 gyver-2.3.3/gyver/filetree/virtual.py
+-rw-r--r--   0        0        0      857 2023-06-20 21:41:14.563536 gyver-2.3.3/gyver/model.py
+-rw-r--r--   0        0        0      101 2023-06-20 21:41:14.564536 gyver-2.3.3/gyver/pools/__init__.py
+-rw-r--r--   0        0        0     5764 2023-06-20 21:41:14.564536 gyver-2.3.3/gyver/pools/asyncio.py
+-rw-r--r--   0        0        0     2225 2023-06-20 21:41:14.564536 gyver-2.3.3/gyver/pools/resource.py
+-rw-r--r--   0        0        0     3855 2023-06-20 21:41:14.564536 gyver-2.3.3/gyver/pools/thread.py
+-rw-r--r--   0        0        0        0 2023-06-20 21:41:14.564536 gyver-2.3.3/gyver/py.typed
+-rw-r--r--   0        0        0      186 2023-06-20 21:41:14.564536 gyver-2.3.3/gyver/url/__init__.py
+-rw-r--r--   0        0        0     4663 2023-06-27 06:41:36.153386 gyver-2.3.3/gyver/url/core.py
+-rw-r--r--   0        0        0      423 2023-06-20 21:41:14.564536 gyver-2.3.3/gyver/url/encode.py
+-rw-r--r--   0        0        0     1285 2023-06-27 06:41:36.153386 gyver-2.3.3/gyver/url/fragment.py
+-rw-r--r--   0        0        0     5566 2023-06-27 06:41:36.153386 gyver-2.3.3/gyver/url/netloc.py
+-rw-r--r--   0        0        0     4307 2023-06-27 06:41:36.153386 gyver-2.3.3/gyver/url/path.py
+-rw-r--r--   0        0        0     3592 2023-06-27 06:41:36.153386 gyver-2.3.3/gyver/url/query.py
+-rw-r--r--   0        0        0     1186 2023-06-27 06:41:36.153386 gyver-2.3.3/gyver/url/utils.py
+-rw-r--r--   0        0        0      726 2023-06-20 21:41:14.565536 gyver-2.3.3/gyver/utils/__init__.py
+-rw-r--r--   0        0        0      156 2023-06-20 21:41:14.565536 gyver-2.3.3/gyver/utils/exc.py
+-rw-r--r--   0        0        0     7836 2023-06-20 21:41:14.565536 gyver-2.3.3/gyver/utils/finder.py
+-rw-r--r--   0        0        0     4262 2023-06-27 06:41:36.153386 gyver-2.3.3/gyver/utils/helpers.py
+-rw-r--r--   0        0        0      174 2023-06-20 21:41:14.565536 gyver-2.3.3/gyver/utils/json.py
+-rw-r--r--   0        0        0     2574 2023-06-27 06:41:36.154386 gyver-2.3.3/gyver/utils/lazy.py
+-rw-r--r--   0        0        0     1319 2023-06-20 21:41:14.565536 gyver-2.3.3/gyver/utils/singleton.py
+-rw-r--r--   0        0        0     2224 2023-06-27 06:41:36.154386 gyver-2.3.3/gyver/utils/strings.py
+-rw-r--r--   0        0        0      134 2023-06-27 06:41:36.154386 gyver-2.3.3/gyver/utils/timezone.py
+-rw-r--r--   0        0        0     2456 2023-07-05 16:04:22.220621 gyver-2.3.3/pyproject.toml
+-rw-r--r--   0        0        0     2553 1970-01-01 00:00:00.000000 gyver-2.3.3/PKG-INFO
```

### Comparing `gyver-2.3.2/LICENSE` & `gyver-2.3.3/LICENSE`

 * *Files identical despite different names*

### Comparing `gyver-2.3.2/README.md` & `gyver-2.3.3/README.md`

 * *Files identical despite different names*

### Comparing `gyver-2.3.2/gyver/cache/asyncio.py` & `gyver-2.3.3/gyver/cache/asyncio.py`

 * *Files identical despite different names*

### Comparing `gyver-2.3.2/gyver/cache/interface.py` & `gyver-2.3.3/gyver/cache/interface.py`

 * *Files identical despite different names*

### Comparing `gyver-2.3.2/gyver/cache/mapper.py` & `gyver-2.3.3/gyver/cache/mapper.py`

 * *Files identical despite different names*

### Comparing `gyver-2.3.2/gyver/cache/mock.py` & `gyver-2.3.3/gyver/cache/mock.py`

 * *Files identical despite different names*

### Comparing `gyver-2.3.2/gyver/cache/redis.py` & `gyver-2.3.3/gyver/cache/redis.py`

 * *Files identical despite different names*

### Comparing `gyver-2.3.2/gyver/cache/sync.py` & `gyver-2.3.3/gyver/cache/sync.py`

 * *Files identical despite different names*

### Comparing `gyver-2.3.2/gyver/cache/utils.py` & `gyver-2.3.3/gyver/cache/utils.py`

 * *Files identical despite different names*

### Comparing `gyver-2.3.2/gyver/config/__init__.py` & `gyver-2.3.3/gyver/config/__init__.py`

 * *Files identical despite different names*

### Comparing `gyver-2.3.2/gyver/config/adapter/attrs.py` & `gyver-2.3.3/gyver/config/adapter/attrs.py`

 * *Files identical despite different names*

### Comparing `gyver-2.3.2/gyver/config/adapter/dataclass.py` & `gyver-2.3.3/gyver/config/adapter/dataclass.py`

 * *Files identical despite different names*

### Comparing `gyver-2.3.2/gyver/config/adapter/factory.py` & `gyver-2.3.3/gyver/config/adapter/factory.py`

 * *Files identical despite different names*

### Comparing `gyver-2.3.2/gyver/config/adapter/gattrs.py` & `gyver-2.3.3/gyver/config/adapter/gattrs.py`

 * *Files identical despite different names*

### Comparing `gyver-2.3.2/gyver/config/adapter/interface.py` & `gyver-2.3.3/gyver/config/adapter/interface.py`

 * *Files identical despite different names*

### Comparing `gyver-2.3.2/gyver/config/adapter/mark.py` & `gyver-2.3.3/gyver/config/adapter/mark.py`

 * *Files identical despite different names*

### Comparing `gyver-2.3.2/gyver/config/adapter/pydantic.py` & `gyver-2.3.3/gyver/config/adapter/pydantic.py`

 * *Files identical despite different names*

### Comparing `gyver-2.3.2/gyver/config/config.py` & `gyver-2.3.3/gyver/config/config.py`

 * *Files identical despite different names*

### Comparing `gyver-2.3.2/gyver/config/envconfig.py` & `gyver-2.3.3/gyver/config/envconfig.py`

 * *Files identical despite different names*

### Comparing `gyver-2.3.2/gyver/config/interface.py` & `gyver-2.3.3/gyver/config/interface.py`

 * *Files identical despite different names*

### Comparing `gyver-2.3.2/gyver/config/lazy.py` & `gyver-2.3.3/gyver/config/lazy.py`

 * *Files identical despite different names*

### Comparing `gyver-2.3.2/gyver/config/typedef.py` & `gyver-2.3.3/gyver/config/typedef.py`

 * *Files identical despite different names*

### Comparing `gyver-2.3.2/gyver/context/atomic_/bound.py` & `gyver-2.3.3/gyver/context/atomic_/bound.py`

 * *Files identical despite different names*

### Comparing `gyver-2.3.2/gyver/context/atomic_/core.py` & `gyver-2.3.3/gyver/context/atomic_/core.py`

 * *Files identical despite different names*

### Comparing `gyver-2.3.2/gyver/context/atomic_/resolver.py` & `gyver-2.3.3/gyver/context/atomic_/resolver.py`

 * *Files identical despite different names*

### Comparing `gyver-2.3.2/gyver/context/context.py` & `gyver-2.3.3/gyver/context/context.py`

 * *Files identical despite different names*

### Comparing `gyver-2.3.2/gyver/context/interfaces/adapter.py` & `gyver-2.3.3/gyver/context/interfaces/adapter.py`

 * *Files identical despite different names*

### Comparing `gyver-2.3.2/gyver/crypto/fernet.py` & `gyver-2.3.3/gyver/crypto/fernet.py`

 * *Files identical despite different names*

### Comparing `gyver-2.3.2/gyver/crypto/rsa.py` & `gyver-2.3.3/gyver/crypto/rsa.py`

 * *Files identical despite different names*

### Comparing `gyver-2.3.2/gyver/database/__init__.py` & `gyver-2.3.3/gyver/database/__init__.py`

 * *Files identical despite different names*

### Comparing `gyver-2.3.2/gyver/database/adapter.py` & `gyver-2.3.3/gyver/database/adapter.py`

 * *Files identical despite different names*

### Comparing `gyver-2.3.2/gyver/database/config.py` & `gyver-2.3.3/gyver/database/config.py`

 * *Files identical despite different names*

### Comparing `gyver-2.3.2/gyver/database/context/asyncio.py` & `gyver-2.3.3/gyver/database/context/asyncio.py`

 * *Files identical despite different names*

### Comparing `gyver-2.3.2/gyver/database/context/sync.py` & `gyver-2.3.3/gyver/database/context/sync.py`

 * *Files identical despite different names*

### Comparing `gyver-2.3.2/gyver/database/drivers/utils.py` & `gyver-2.3.3/gyver/database/drivers/utils.py`

 * *Files identical despite different names*

### Comparing `gyver-2.3.2/gyver/database/entity.py` & `gyver-2.3.3/gyver/database/entity.py`

 * *Files identical despite different names*

### Comparing `gyver-2.3.2/gyver/database/query/__init__.py` & `gyver-2.3.3/gyver/database/query/__init__.py`

 * *Files identical despite different names*

### Comparing `gyver-2.3.2/gyver/database/query/_helpers.py` & `gyver-2.3.3/gyver/database/query/_helpers.py`

 * *Files identical despite different names*

### Comparing `gyver-2.3.2/gyver/database/query/comp.py` & `gyver-2.3.3/gyver/database/query/comp.py`

 * *Files identical despite different names*

### Comparing `gyver-2.3.2/gyver/database/query/interface.py` & `gyver-2.3.3/gyver/database/query/interface.py`

 * *Files identical despite different names*

### Comparing `gyver-2.3.2/gyver/database/query/order_by.py` & `gyver-2.3.3/gyver/database/query/order_by.py`

 * *Files identical despite different names*

### Comparing `gyver-2.3.2/gyver/database/query/paginate.py` & `gyver-2.3.3/gyver/database/query/paginate.py`

 * *Files identical despite different names*

### Comparing `gyver-2.3.2/gyver/database/query/utils.py` & `gyver-2.3.3/gyver/database/query/utils.py`

 * *Files identical despite different names*

### Comparing `gyver-2.3.2/gyver/database/query/where.py` & `gyver-2.3.3/gyver/database/query/where.py`

 * *Files identical despite different names*

### Comparing `gyver-2.3.2/gyver/database/utils.py` & `gyver-2.3.3/gyver/database/utils.py`

 * *Files identical despite different names*

### Comparing `gyver-2.3.2/gyver/exc.py` & `gyver-2.3.3/gyver/exc.py`

 * *Files identical despite different names*

### Comparing `gyver-2.3.2/gyver/filetree/filetree.py` & `gyver-2.3.3/gyver/filetree/filetree.py`

 * *Files identical despite different names*

### Comparing `gyver-2.3.2/gyver/filetree/interface.py` & `gyver-2.3.3/gyver/filetree/interface.py`

 * *Files 6% similar despite different names*

```diff
@@ -48,14 +48,17 @@
         if not isinstance(target, fileclass):
             raise InvalidPath(
                 "filename conflicts with other folder, or different fileclass"
             )
         directory.contents[filename] = target
         return target
 
+    def create_text_file(self, filename: str, *path: str) -> TextFile:
+        return self.create_file(filename, *path, fileclass=TextFile)
+
     def get_file(self, filename: str, *path: str) -> File:
         if path:
             dirname, *restpath = path
             directory = self.get_dir(dirname, *restpath)
         else:
             directory = self.root
         if not directory:
```

### Comparing `gyver-2.3.2/gyver/filetree/typedef.py` & `gyver-2.3.3/gyver/filetree/typedef.py`

 * *Files identical despite different names*

### Comparing `gyver-2.3.2/gyver/filetree/virtual.py` & `gyver-2.3.3/gyver/filetree/virtual.py`

 * *Files identical despite different names*

### Comparing `gyver-2.3.2/gyver/model.py` & `gyver-2.3.3/gyver/model.py`

 * *Files identical despite different names*

### Comparing `gyver-2.3.2/gyver/pools/asyncio.py` & `gyver-2.3.3/gyver/pools/asyncio.py`

 * *Files identical despite different names*

### Comparing `gyver-2.3.2/gyver/pools/resource.py` & `gyver-2.3.3/gyver/pools/resource.py`

 * *Files identical despite different names*

### Comparing `gyver-2.3.2/gyver/pools/thread.py` & `gyver-2.3.3/gyver/pools/thread.py`

 * *Files identical despite different names*

### Comparing `gyver-2.3.2/gyver/url/core.py` & `gyver-2.3.3/gyver/url/core.py`

 * *Files identical despite different names*

### Comparing `gyver-2.3.2/gyver/url/fragment.py` & `gyver-2.3.3/gyver/url/fragment.py`

 * *Files identical despite different names*

### Comparing `gyver-2.3.2/gyver/url/netloc.py` & `gyver-2.3.3/gyver/url/netloc.py`

 * *Files identical despite different names*

### Comparing `gyver-2.3.2/gyver/url/path.py` & `gyver-2.3.3/gyver/url/path.py`

 * *Files identical despite different names*

### Comparing `gyver-2.3.2/gyver/url/query.py` & `gyver-2.3.3/gyver/url/query.py`

 * *Files identical despite different names*

### Comparing `gyver-2.3.2/gyver/url/utils.py` & `gyver-2.3.3/gyver/url/utils.py`

 * *Files identical despite different names*

### Comparing `gyver-2.3.2/gyver/utils/__init__.py` & `gyver-2.3.3/gyver/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `gyver-2.3.2/gyver/utils/finder.py` & `gyver-2.3.3/gyver/utils/finder.py`

 * *Files identical despite different names*

### Comparing `gyver-2.3.2/gyver/utils/helpers.py` & `gyver-2.3.3/gyver/utils/helpers.py`

 * *Files identical despite different names*

### Comparing `gyver-2.3.2/gyver/utils/lazy.py` & `gyver-2.3.3/gyver/utils/lazy.py`

 * *Files identical despite different names*

### Comparing `gyver-2.3.2/gyver/utils/singleton.py` & `gyver-2.3.3/gyver/utils/singleton.py`

 * *Files identical despite different names*

### Comparing `gyver-2.3.2/gyver/utils/strings.py` & `gyver-2.3.3/gyver/utils/strings.py`

 * *Files identical despite different names*

### Comparing `gyver-2.3.2/pyproject.toml` & `gyver-2.3.3/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "gyver"
-version = "2.3.2"
+version = "2.3.3"
 description = "Toolbox for web development"
 authors = ["Gustavo Correa <self.gustavocorrea@gmail.com>"]
 readme = "README.md"
 repository = "https://github.com/guscardvs/gyver"
 
 [tool.poetry.dependencies]
 python = "^3.9"
```

### Comparing `gyver-2.3.2/PKG-INFO` & `gyver-2.3.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gyver
-Version: 2.3.2
+Version: 2.3.3
 Summary: Toolbox for web development
 Home-page: https://github.com/guscardvs/gyver
 Author: Gustavo Correa
 Author-email: self.gustavocorrea@gmail.com
 Requires-Python: >=3.9,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
```

