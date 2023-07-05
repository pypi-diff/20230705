# Comparing `tmp/tiny_vk-1.0.2.tar.gz` & `tmp/tiny_vk-1.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tiny_vk-1.0.2.tar", max compression
+gzip compressed data, was "tiny_vk-1.0.3.tar", max compression
```

## Comparing `tiny_vk-1.0.2.tar` & `tiny_vk-1.0.3.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0      736 2023-07-05 08:44:45.603767 tiny_vk-1.0.2/README.md
--rw-r--r--   0        0        0      356 2023-07-05 08:47:26.844364 tiny_vk-1.0.2/pyproject.toml
--rw-r--r--   0        0        0        0 2023-07-05 07:36:53.819676 tiny_vk-1.0.2/tiny_vk/__init__.py
--rw-r--r--   0        0        0     2739 2023-06-27 19:08:19.162081 tiny_vk-1.0.2/tiny_vk/_database.py
--rw-r--r--   0        0        0       77 2023-07-04 06:17:47.896813 tiny_vk-1.0.2/tiny_vk/_exceptions.py
--rw-r--r--   0        0        0     8530 2023-07-05 08:45:13.930224 tiny_vk-1.0.2/tiny_vk/bot.py
--rw-r--r--   0        0        0      402 2023-07-04 06:37:30.599601 tiny_vk-1.0.2/tiny_vk/ctx.py
--rw-r--r--   0        0        0     1151 1970-01-01 00:00:00.000000 tiny_vk-1.0.2/PKG-INFO
+-rw-r--r--   0        0        0      736 2023-07-05 08:59:55.174263 tiny_vk-1.0.3/README.md
+-rw-r--r--   0        0        0      356 2023-07-05 09:00:16.869606 tiny_vk-1.0.3/pyproject.toml
+-rw-r--r--   0        0        0       49 2023-07-05 08:55:38.878206 tiny_vk-1.0.3/tiny_vk/__init__.py
+-rw-r--r--   0        0        0     2739 2023-07-05 08:57:38.128095 tiny_vk-1.0.3/tiny_vk/_database.py
+-rw-r--r--   0        0        0       77 2023-07-04 06:17:47.896813 tiny_vk-1.0.3/tiny_vk/_exceptions.py
+-rw-r--r--   0        0        0     8530 2023-07-05 08:58:32.470955 tiny_vk-1.0.3/tiny_vk/bot.py
+-rw-r--r--   0        0        0      402 2023-07-04 06:37:30.599601 tiny_vk-1.0.3/tiny_vk/ctx.py
+-rw-r--r--   0        0        0     1151 1970-01-01 00:00:00.000000 tiny_vk-1.0.3/PKG-INFO
```

### Comparing `tiny_vk-1.0.2/README.md` & `tiny_vk-1.0.3/README.md`

 * *Files identical despite different names*

### Comparing `tiny_vk-1.0.2/tiny_vk/_database.py` & `tiny_vk-1.0.3/tiny_vk/_database.py`

 * *Files identical despite different names*

### Comparing `tiny_vk-1.0.2/tiny_vk/bot.py` & `tiny_vk-1.0.3/tiny_vk/bot.py`

 * *Files identical despite different names*

### Comparing `tiny_vk-1.0.2/PKG-INFO` & `tiny_vk-1.0.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tiny-vk
-Version: 1.0.2
+Version: 1.0.3
 Summary: Сreating simple vk bots
 Author: QuoNaro
 Author-email: QuoNaro@mail.ru
 Requires-Python: >=3.10
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
```

