# Comparing `tmp/wagtail-external-link-richtext-1.1.1.tar.gz` & `tmp/wagtail-external-link-richtext-1.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "wagtail-external-link-richtext-1.1.1.tar", last modified: Tue Jul  4 13:56:50 2023, max compression
+gzip compressed data, was "wagtail-external-link-richtext-1.1.2.tar", last modified: Wed Jul  5 12:23:09 2023, max compression
```

## Comparing `wagtail-external-link-richtext-1.1.1.tar` & `wagtail-external-link-richtext-1.1.2.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxr-xr-x   0 rubenhesselink   (501) staff       (20)        0 2023-07-04 13:56:50.090724 wagtail-external-link-richtext-1.1.1/
--rw-r--r--   0 rubenhesselink   (501) staff       (20)     1058 2023-07-04 11:49:42.000000 wagtail-external-link-richtext-1.1.1/LICENSE
--rw-r--r--   0 rubenhesselink   (501) staff       (20)       59 2023-07-03 13:55:40.000000 wagtail-external-link-richtext-1.1.1/MANIFEST.in
--rw-r--r--   0 rubenhesselink   (501) staff       (20)     2554 2023-07-04 13:56:50.090183 wagtail-external-link-richtext-1.1.1/PKG-INFO
--rw-r--r--   0 rubenhesselink   (501) staff       (20)      587 2023-07-04 13:56:37.000000 wagtail-external-link-richtext-1.1.1/README.rst
-drwxr-xr-x   0 rubenhesselink   (501) staff       (20)        0 2023-07-04 13:56:50.082483 wagtail-external-link-richtext-1.1.1/external_link/
--rw-r--r--   0 rubenhesselink   (501) staff       (20)        0 2023-07-03 11:48:23.000000 wagtail-external-link-richtext-1.1.1/external_link/__init__.py
--rw-r--r--   0 rubenhesselink   (501) staff       (20)      894 2023-07-03 11:51:09.000000 wagtail-external-link-richtext-1.1.1/external_link/handlers.py
-drwxr-xr-x   0 rubenhesselink   (501) staff       (20)        0 2023-07-04 13:56:50.083050 wagtail-external-link-richtext-1.1.1/external_link/migrations/
--rw-r--r--   0 rubenhesselink   (501) staff       (20)        0 2023-07-03 11:48:23.000000 wagtail-external-link-richtext-1.1.1/external_link/migrations/__init__.py
-drwxr-xr-x   0 rubenhesselink   (501) staff       (20)        0 2023-07-04 13:56:50.078301 wagtail-external-link-richtext-1.1.1/external_link/static/
-drwxr-xr-x   0 rubenhesselink   (501) staff       (20)        0 2023-07-04 13:56:50.083547 wagtail-external-link-richtext-1.1.1/external_link/static/css/
--rw-r--r--   0 rubenhesselink   (501) staff       (20)      617 2023-07-03 11:51:09.000000 wagtail-external-link-richtext-1.1.1/external_link/static/css/newtab_form.css
-drwxr-xr-x   0 rubenhesselink   (501) staff       (20)        0 2023-07-04 13:56:50.084167 wagtail-external-link-richtext-1.1.1/external_link/static/js/
--rw-r--r--   0 rubenhesselink   (501) staff       (20)     6401 2023-07-03 11:51:09.000000 wagtail-external-link-richtext-1.1.1/external_link/static/js/newtab.js
--rw-r--r--   0 rubenhesselink   (501) staff       (20)     1310 2023-07-03 12:07:09.000000 wagtail-external-link-richtext-1.1.1/external_link/wagtail_hooks.py
--rw-r--r--   0 rubenhesselink   (501) staff       (20)     1017 2023-07-04 13:54:54.000000 wagtail-external-link-richtext-1.1.1/pyproject.toml
--rw-r--r--   0 rubenhesselink   (501) staff       (20)       38 2023-07-04 13:56:50.090878 wagtail-external-link-richtext-1.1.1/setup.cfg
-drwxr-xr-x   0 rubenhesselink   (501) staff       (20)        0 2023-07-04 13:56:50.089424 wagtail-external-link-richtext-1.1.1/wagtail_external_link_richtext.egg-info/
--rw-r--r--   0 rubenhesselink   (501) staff       (20)     2554 2023-07-04 13:56:50.000000 wagtail-external-link-richtext-1.1.1/wagtail_external_link_richtext.egg-info/PKG-INFO
--rw-r--r--   0 rubenhesselink   (501) staff       (20)      509 2023-07-04 13:56:50.000000 wagtail-external-link-richtext-1.1.1/wagtail_external_link_richtext.egg-info/SOURCES.txt
--rw-r--r--   0 rubenhesselink   (501) staff       (20)        1 2023-07-04 13:56:50.000000 wagtail-external-link-richtext-1.1.1/wagtail_external_link_richtext.egg-info/dependency_links.txt
--rw-r--r--   0 rubenhesselink   (501) staff       (20)       35 2023-07-04 13:56:50.000000 wagtail-external-link-richtext-1.1.1/wagtail_external_link_richtext.egg-info/requires.txt
--rw-r--r--   0 rubenhesselink   (501) staff       (20)       14 2023-07-04 13:56:50.000000 wagtail-external-link-richtext-1.1.1/wagtail_external_link_richtext.egg-info/top_level.txt
+drwxr-xr-x   0 rubenhesselink   (501) staff       (20)        0 2023-07-05 12:23:09.312514 wagtail-external-link-richtext-1.1.2/
+-rw-r--r--   0 rubenhesselink   (501) staff       (20)     1058 2023-07-04 11:49:42.000000 wagtail-external-link-richtext-1.1.2/LICENSE
+-rw-r--r--   0 rubenhesselink   (501) staff       (20)       77 2023-07-05 12:06:28.000000 wagtail-external-link-richtext-1.1.2/MANIFEST.in
+-rw-r--r--   0 rubenhesselink   (501) staff       (20)     3690 2023-07-05 12:23:09.312039 wagtail-external-link-richtext-1.1.2/PKG-INFO
+-rw-r--r--   0 rubenhesselink   (501) staff       (20)     1721 2023-07-05 12:19:42.000000 wagtail-external-link-richtext-1.1.2/README.md
+drwxr-xr-x   0 rubenhesselink   (501) staff       (20)        0 2023-07-05 12:23:09.302396 wagtail-external-link-richtext-1.1.2/external_link/
+-rw-r--r--   0 rubenhesselink   (501) staff       (20)        0 2023-07-03 11:48:23.000000 wagtail-external-link-richtext-1.1.2/external_link/__init__.py
+-rw-r--r--   0 rubenhesselink   (501) staff       (20)      894 2023-07-03 11:51:09.000000 wagtail-external-link-richtext-1.1.2/external_link/handlers.py
+drwxr-xr-x   0 rubenhesselink   (501) staff       (20)        0 2023-07-05 12:23:09.303435 wagtail-external-link-richtext-1.1.2/external_link/migrations/
+-rw-r--r--   0 rubenhesselink   (501) staff       (20)        0 2023-07-03 11:48:23.000000 wagtail-external-link-richtext-1.1.2/external_link/migrations/__init__.py
+drwxr-xr-x   0 rubenhesselink   (501) staff       (20)        0 2023-07-05 12:23:09.298012 wagtail-external-link-richtext-1.1.2/external_link/static/
+drwxr-xr-x   0 rubenhesselink   (501) staff       (20)        0 2023-07-05 12:23:09.304023 wagtail-external-link-richtext-1.1.2/external_link/static/css/
+-rw-r--r--   0 rubenhesselink   (501) staff       (20)      617 2023-07-03 11:51:09.000000 wagtail-external-link-richtext-1.1.2/external_link/static/css/newtab_form.css
+drwxr-xr-x   0 rubenhesselink   (501) staff       (20)        0 2023-07-05 12:23:09.305016 wagtail-external-link-richtext-1.1.2/external_link/static/js/
+-rw-r--r--   0 rubenhesselink   (501) staff       (20)     6401 2023-07-03 11:51:09.000000 wagtail-external-link-richtext-1.1.2/external_link/static/js/newtab.js
+-rw-r--r--   0 rubenhesselink   (501) staff       (20)     1310 2023-07-03 12:07:09.000000 wagtail-external-link-richtext-1.1.2/external_link/wagtail_hooks.py
+-rw-r--r--   0 rubenhesselink   (501) staff       (20)     1158 2023-07-05 12:22:52.000000 wagtail-external-link-richtext-1.1.2/pyproject.toml
+-rw-r--r--   0 rubenhesselink   (501) staff       (20)       38 2023-07-05 12:23:09.312657 wagtail-external-link-richtext-1.1.2/setup.cfg
+drwxr-xr-x   0 rubenhesselink   (501) staff       (20)        0 2023-07-05 12:23:09.311246 wagtail-external-link-richtext-1.1.2/wagtail_external_link_richtext.egg-info/
+-rw-r--r--   0 rubenhesselink   (501) staff       (20)     3690 2023-07-05 12:23:09.000000 wagtail-external-link-richtext-1.1.2/wagtail_external_link_richtext.egg-info/PKG-INFO
+-rw-r--r--   0 rubenhesselink   (501) staff       (20)      508 2023-07-05 12:23:09.000000 wagtail-external-link-richtext-1.1.2/wagtail_external_link_richtext.egg-info/SOURCES.txt
+-rw-r--r--   0 rubenhesselink   (501) staff       (20)        1 2023-07-05 12:23:09.000000 wagtail-external-link-richtext-1.1.2/wagtail_external_link_richtext.egg-info/dependency_links.txt
+-rw-r--r--   0 rubenhesselink   (501) staff       (20)       35 2023-07-05 12:23:09.000000 wagtail-external-link-richtext-1.1.2/wagtail_external_link_richtext.egg-info/requires.txt
+-rw-r--r--   0 rubenhesselink   (501) staff       (20)       14 2023-07-05 12:23:09.000000 wagtail-external-link-richtext-1.1.2/wagtail_external_link_richtext.egg-info/top_level.txt
```

### Comparing `wagtail-external-link-richtext-1.1.1/LICENSE` & `wagtail-external-link-richtext-1.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `wagtail-external-link-richtext-1.1.1/external_link/handlers.py` & `wagtail-external-link-richtext-1.1.2/external_link/handlers.py`

 * *Files identical despite different names*

### Comparing `wagtail-external-link-richtext-1.1.1/external_link/static/css/newtab_form.css` & `wagtail-external-link-richtext-1.1.2/external_link/static/css/newtab_form.css`

 * *Files identical despite different names*

### Comparing `wagtail-external-link-richtext-1.1.1/external_link/static/js/newtab.js` & `wagtail-external-link-richtext-1.1.2/external_link/static/js/newtab.js`

 * *Files identical despite different names*

### Comparing `wagtail-external-link-richtext-1.1.1/external_link/wagtail_hooks.py` & `wagtail-external-link-richtext-1.1.2/external_link/wagtail_hooks.py`

 * *Files identical despite different names*

### Comparing `wagtail-external-link-richtext-1.1.1/pyproject.toml` & `wagtail-external-link-richtext-1.1.2/pyproject.toml`

 * *Files 7% similar despite different names*

```diff
@@ -1,16 +1,23 @@
 [build-system]
 requires = ["setuptools", "wheel"]
 build-backend = "setuptools.build_meta"
 
+[tool.setuptools]
+include-package-data = false
+
+[tool.setuptools.packages.find]
+include = ["external_link*"]
+exclude = ["sandbox*", "docs*"]
+
 [project]
 name = "wagtail-external-link-richtext"
-version = "1.1.1"
+version = "1.1.2"
 description = "A feature for the richtext fields in Wagtail"
-readme = "README.rst"
+readme = "README.md"
 authors = [{name = "Ruben Hesselink", email = "ruben@fourdigits.nl" }]
 license = { file = "LICENSE" }
 classifiers = [
     "Environment :: Web Environment",
     "Framework :: Wagtail",
     "Framework :: Django",
     "Intended Audience :: Developers",
```

