# Comparing `tmp/tiny_vk-1.0.4.tar.gz` & `tmp/tiny_vk-1.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tiny_vk-1.0.4.tar", max compression
+gzip compressed data, was "tiny_vk-1.0.5.tar", max compression
```

## Comparing `tiny_vk-1.0.4.tar` & `tiny_vk-1.0.5.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0      732 2023-07-05 09:02:17.832517 tiny_vk-1.0.4/README.md
--rw-r--r--   0        0        0      356 2023-07-05 09:02:08.802374 tiny_vk-1.0.4/pyproject.toml
--rw-r--r--   0        0        0       49 2023-07-05 08:55:38.878206 tiny_vk-1.0.4/tiny_vk/__init__.py
--rw-r--r--   0        0        0     8530 2023-07-05 09:05:45.380792 tiny_vk-1.0.4/tiny_vk/bot.py
--rw-r--r--   0        0        0      402 2023-07-04 06:37:30.599601 tiny_vk-1.0.4/tiny_vk/ctx.py
--rw-r--r--   0        0        0     2739 2023-07-05 08:57:38.128095 tiny_vk-1.0.4/tiny_vk/database.py
--rw-r--r--   0        0        0       77 2023-07-04 06:17:47.896813 tiny_vk-1.0.4/tiny_vk/exceptions.py
--rw-r--r--   0        0        0     1147 1970-01-01 00:00:00.000000 tiny_vk-1.0.4/PKG-INFO
+-rw-r--r--   0        0        0      732 2023-07-05 18:40:46.146351 tiny_vk-1.0.5/README.md
+-rw-r--r--   0        0        0      356 2023-07-05 18:40:46.146351 tiny_vk-1.0.5/pyproject.toml
+-rw-r--r--   0        0        0       49 2023-07-05 18:40:46.146351 tiny_vk-1.0.5/tiny_vk/__init__.py
+-rw-r--r--   0        0        0     8530 2023-07-05 18:40:46.146351 tiny_vk-1.0.5/tiny_vk/bot.py
+-rw-r--r--   0        0        0      402 2023-07-05 18:40:46.146351 tiny_vk-1.0.5/tiny_vk/ctx.py
+-rw-r--r--   0        0        0     2739 2023-07-05 18:40:46.146351 tiny_vk-1.0.5/tiny_vk/database.py
+-rw-r--r--   0        0        0       77 2023-07-05 18:40:46.146351 tiny_vk-1.0.5/tiny_vk/exceptions.py
+-rw-r--r--   0        0        0     1147 1970-01-01 00:00:00.000000 tiny_vk-1.0.5/PKG-INFO
```

### Comparing `tiny_vk-1.0.4/README.md` & `tiny_vk-1.0.5/README.md`

 * *Files identical despite different names*

### Comparing `tiny_vk-1.0.4/tiny_vk/bot.py` & `tiny_vk-1.0.5/tiny_vk/bot.py`

 * *Files identical despite different names*

### Comparing `tiny_vk-1.0.4/tiny_vk/database.py` & `tiny_vk-1.0.5/tiny_vk/database.py`

 * *Files identical despite different names*

### Comparing `tiny_vk-1.0.4/PKG-INFO` & `tiny_vk-1.0.5/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tiny-vk
-Version: 1.0.4
+Version: 1.0.5
 Summary: Сreating simple vk bots
 Author: QuoNaro
 Author-email: QuoNaro@mail.ru
 Requires-Python: >=3.10
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
```

