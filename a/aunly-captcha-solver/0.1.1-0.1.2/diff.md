# Comparing `tmp/aunly_captcha_solver-0.1.1.tar.gz` & `tmp/aunly_captcha_solver-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aunly_captcha_solver-0.1.1.tar", last modified: Tue Jul  4 16:51:15 2023, max compression
+gzip compressed data, was "aunly_captcha_solver-0.1.2.tar", last modified: Tue Jul  4 17:01:12 2023, max compression
```

## Comparing `aunly_captcha_solver-0.1.1.tar` & `aunly_captcha_solver-0.1.2.tar`

### file list

```diff
@@ -1,4 +1,4 @@
--rw-r--r--   0        0        0        5 2023-07-04 16:50:58.992354 aunly_captcha_solver-0.1.1/README.md
--rw-r--r--   0        0        0     5191 2023-07-04 16:46:59.788049 aunly_captcha_solver-0.1.1/aunly_captcha_solver/__init__.py
--rw-r--r--   0        0        0      472 2023-07-04 16:51:15.927807 aunly_captcha_solver-0.1.1/pyproject.toml
--rw-r--r--   0        0        0      372 1970-01-01 00:00:00.000000 aunly_captcha_solver-0.1.1/PKG-INFO
+-rw-r--r--   0        0        0        5 2023-07-04 16:50:58.992354 aunly_captcha_solver-0.1.2/README.md
+-rw-r--r--   0        0        0     5191 2023-07-04 16:46:59.788049 aunly_captcha_solver-0.1.2/aunly_captcha_solver/__init__.py
+-rw-r--r--   0        0        0      480 2023-07-04 17:01:12.097547 aunly_captcha_solver-0.1.2/pyproject.toml
+-rw-r--r--   0        0        0      379 1970-01-01 00:00:00.000000 aunly_captcha_solver-0.1.2/PKG-INFO
```

### Comparing `aunly_captcha_solver-0.1.1/aunly_captcha_solver/__init__.py` & `aunly_captcha_solver-0.1.2/aunly_captcha_solver/__init__.py`

 * *Files identical despite different names*

