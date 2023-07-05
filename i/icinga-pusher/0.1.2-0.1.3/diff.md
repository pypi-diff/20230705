# Comparing `tmp/icinga_pusher-0.1.2.tar.gz` & `tmp/icinga_pusher-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "icinga_pusher-0.1.2.tar", max compression
+gzip compressed data, was "icinga_pusher-0.1.3.tar", max compression
```

## Comparing `icinga_pusher-0.1.2.tar` & `icinga_pusher-0.1.3.tar`

### file list

```diff
@@ -1,5 +1,5 @@
--rw-r--r--   0        0        0    35149 2023-07-04 15:40:12.723695 icinga_pusher-0.1.2/LICENSE
--rw-r--r--   0        0        0        0 2023-07-04 15:40:12.727028 icinga_pusher-0.1.2/README.md
--rw-r--r--   0        0        0     2910 2023-07-04 15:40:12.727028 icinga_pusher-0.1.2/icinga_pusher/__init__.py
--rw-r--r--   0        0        0      388 2023-07-04 15:40:26.110410 icinga_pusher-0.1.2/pyproject.toml
--rw-r--r--   0        0        0      331 1970-01-01 00:00:00.000000 icinga_pusher-0.1.2/PKG-INFO
+-rw-r--r--   0        0        0    35149 2023-07-04 15:40:12.723695 icinga_pusher-0.1.3/LICENSE
+-rw-r--r--   0        0        0        0 2023-07-04 15:40:12.727028 icinga_pusher-0.1.3/README.md
+-rw-r--r--   0        0        0     2910 2023-07-04 15:40:12.727028 icinga_pusher-0.1.3/icinga_pusher/__init__.py
+-rw-r--r--   0        0        0      388 2023-07-04 17:24:49.400246 icinga_pusher-0.1.3/pyproject.toml
+-rw-r--r--   0        0        0      382 1970-01-01 00:00:00.000000 icinga_pusher-0.1.3/PKG-INFO
```

### Comparing `icinga_pusher-0.1.2/LICENSE` & `icinga_pusher-0.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `icinga_pusher-0.1.2/icinga_pusher/__init__.py` & `icinga_pusher-0.1.3/icinga_pusher/__init__.py`

 * *Files identical despite different names*

