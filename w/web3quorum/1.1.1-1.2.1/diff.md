# Comparing `tmp/web3quorum-1.1.1.tar.gz` & `tmp/web3quorum-1.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "web3quorum-1.1.1.tar", last modified: Tue Dec 24 02:06:46 2019, max compression
+gzip compressed data, was "web3quorum-1.2.1.tar", max compression
```

## Comparing `web3quorum-1.1.1.tar` & `web3quorum-1.2.1.tar`

### file list

```diff
@@ -1,8 +1,7 @@
--rw-r--r--   0        0        0    11357 2019-12-20 10:09:54.370000 web3quorum-1.1.1/LICENSE
--rw-r--r--   0        0        0      339 2019-12-24 02:06:02.873666 web3quorum-1.1.1/pyproject.toml
--rw-r--r--   0        0        0      235 2019-12-20 10:09:54.370000 web3quorum-1.1.1/web3quorum/__init__.py
--rw-r--r--   0        0        0     3997 2019-12-24 01:53:39.633666 web3quorum-1.1.1/web3quorum/quorum.py
--rw-r--r--   0        0        0      703 2019-12-24 01:53:39.633666 web3quorum-1.1.1/web3quorum/test_utils.py
--rw-r--r--   0        0        0      594 2019-12-24 01:53:39.633666 web3quorum-1.1.1/web3quorum/utils.py
--rw-r--r--   0        0        0      617 2019-12-24 02:06:46.148151 web3quorum-1.1.1/setup.py
--rw-r--r--   0        0        0      426 2019-12-24 02:06:46.148381 web3quorum-1.1.1/PKG-INFO
+-rw-r--r--   0        0        0    11357 2023-03-04 08:34:00.042131 web3quorum-1.2.1/LICENSE
+-rw-r--r--   0        0        0      384 2023-07-05 05:44:39.745079 web3quorum-1.2.1/pyproject.toml
+-rw-r--r--   0        0        0      235 2023-03-04 08:34:00.042764 web3quorum-1.2.1/web3quorum/__init__.py
+-rw-r--r--   0        0        0     3997 2023-03-04 08:34:00.042860 web3quorum-1.2.1/web3quorum/quorum.py
+-rw-r--r--   0        0        0      703 2023-03-04 08:34:00.042938 web3quorum-1.2.1/web3quorum/test_utils.py
+-rw-r--r--   0        0        0      594 2023-03-04 08:34:00.043020 web3quorum-1.2.1/web3quorum/utils.py
+-rw-r--r--   0        0        0      538 1970-01-01 00:00:00.000000 web3quorum-1.2.1/PKG-INFO
```

### Comparing `web3quorum-1.1.1/LICENSE` & `web3quorum-1.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `web3quorum-1.1.1/web3quorum/quorum.py` & `web3quorum-1.2.1/web3quorum/quorum.py`

 * *Files identical despite different names*

### Comparing `web3quorum-1.1.1/web3quorum/test_utils.py` & `web3quorum-1.2.1/web3quorum/test_utils.py`

 * *Files identical despite different names*

### Comparing `web3quorum-1.1.1/web3quorum/utils.py` & `web3quorum-1.2.1/web3quorum/utils.py`

 * *Files identical despite different names*

