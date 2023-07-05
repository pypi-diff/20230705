# Comparing `tmp/type_dep-0.0.1.tar.gz` & `tmp/type_dep-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "type_dep-0.0.1.tar", last modified: Thu May 12 14:22:30 2022, max compression
+gzip compressed data, was "type_dep-0.0.2.tar", last modified: Wed Jul  5 14:57:26 2023, max compression
```

## Comparing `type_dep-0.0.1.tar` & `type_dep-0.0.2.tar`

### file list

```diff
@@ -1,15 +1,16 @@
-drwxr-xr-x   0 mac        (501) staff       (20)        0 2022-05-12 14:22:30.511999 type_dep-0.0.1/
--rw-r--r--   0 mac        (501) staff       (20)     1071 2022-04-25 18:59:01.000000 type_dep-0.0.1/LICENSE
--rw-r--r--   0 mac        (501) staff       (20)       24 2022-05-04 07:01:02.000000 type_dep-0.0.1/MANIFEST.in
--rw-r--r--   0 mac        (501) staff       (20)     2927 2022-05-12 14:22:30.511703 type_dep-0.0.1/PKG-INFO
--rw-r--r--   0 mac        (501) staff       (20)     2377 2022-05-12 14:18:11.000000 type_dep-0.0.1/README.md
--rw-r--r--   0 mac        (501) staff       (20)       38 2022-05-12 14:22:30.512155 type_dep-0.0.1/setup.cfg
--rw-r--r--   0 mac        (501) staff       (20)      974 2022-05-12 14:13:59.000000 type_dep-0.0.1/setup.py
-drwxr-xr-x   0 mac        (501) staff       (20)        0 2022-05-12 14:22:30.509580 type_dep-0.0.1/type_dep/
--rw-r--r--   0 mac        (501) staff       (20)      201 2022-05-12 14:16:19.000000 type_dep-0.0.1/type_dep/__init__.py
--rw-r--r--   0 mac        (501) staff       (20)     2213 2022-05-12 13:41:40.000000 type_dep-0.0.1/type_dep/_core.py
-drwxr-xr-x   0 mac        (501) staff       (20)        0 2022-05-12 14:22:30.511283 type_dep-0.0.1/type_dep.egg-info/
--rw-r--r--   0 mac        (501) staff       (20)     2927 2022-05-12 14:22:29.000000 type_dep-0.0.1/type_dep.egg-info/PKG-INFO
--rw-r--r--   0 mac        (501) staff       (20)      205 2022-05-12 14:22:30.000000 type_dep-0.0.1/type_dep.egg-info/SOURCES.txt
--rw-r--r--   0 mac        (501) staff       (20)        1 2022-05-12 14:22:29.000000 type_dep-0.0.1/type_dep.egg-info/dependency_links.txt
--rw-r--r--   0 mac        (501) staff       (20)        9 2022-05-12 14:22:30.000000 type_dep-0.0.1/type_dep.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-05 14:57:26.953490 type_dep-0.0.2/
+-rw-r--r--   0 runner    (1001) docker     (122)     1071 2023-07-05 14:57:15.000000 type_dep-0.0.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (122)     5139 2023-07-05 14:57:26.953490 type_dep-0.0.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)     4589 2023-07-05 14:57:15.000000 type_dep-0.0.2/README.md
+-rw-r--r--   0 runner    (1001) docker     (122)       38 2023-07-05 14:57:26.953490 type_dep-0.0.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (122)      974 2023-07-05 14:57:15.000000 type_dep-0.0.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-05 14:57:26.953490 type_dep-0.0.2/test/
+-rw-r--r--   0 runner    (1001) docker     (122)     4742 2023-07-05 14:57:15.000000 type_dep-0.0.2/test/test_core.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-05 14:57:26.953490 type_dep-0.0.2/type_dep/
+-rw-r--r--   0 runner    (1001) docker     (122)      224 2023-07-05 14:57:15.000000 type_dep-0.0.2/type_dep/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4387 2023-07-05 14:57:15.000000 type_dep-0.0.2/type_dep/_core.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-05 14:57:26.953490 type_dep-0.0.2/type_dep.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (122)     5139 2023-07-05 14:57:26.000000 type_dep-0.0.2/type_dep.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)      211 2023-07-05 14:57:26.000000 type_dep-0.0.2/type_dep.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        1 2023-07-05 14:57:26.000000 type_dep-0.0.2/type_dep.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        9 2023-07-05 14:57:26.000000 type_dep-0.0.2/type_dep.egg-info/top_level.txt
```

### Comparing `type_dep-0.0.1/LICENSE` & `type_dep-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `type_dep-0.0.1/setup.py` & `type_dep-0.0.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 
 # The text of the README file
 README = (HERE / "README.md").read_text()
 
 # This call to setup() does all the work
 setup(
     name="type_dep",
-    version="0.0.1",
+    version="0.0.2",
     description="type_dep is a dependency injection framework that uses type hints to inject dependencies (much like Angular, Dotnet and the like)",
     long_description=README,
     long_description_content_type="text/markdown",
     url="https://github.com/sopherapps/type_dep",
     author="Martin Ahindura",
     author_email="team.sopherapps@gmail.com",
     license="MIT",
```

