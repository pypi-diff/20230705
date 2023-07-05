# Comparing `tmp/yplib-2.2.2.tar.gz` & `tmp/yplib-2.2.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\yplib-2.2.2.tar", last modified: Wed Jul  5 00:56:55 2023, max compression
+gzip compressed data, was "dist\yplib-2.2.3.tar", last modified: Wed Jul  5 01:20:53 2023, max compression
```

## Comparing `yplib-2.2.2.tar` & `yplib-2.2.3.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxrwxrwx   0        0        0        0 2023-07-05 00:56:55.795673 yplib-2.2.2/
--rw-rw-rw-   0        0        0     1091 2023-06-08 01:05:18.000000 yplib-2.2.2/LICENSE
--rw-rw-rw-   0        0        0      352 2023-07-05 00:56:55.795122 yplib-2.2.2/PKG-INFO
--rw-rw-rw-   0        0        0       13 2023-06-14 02:50:41.000000 yplib-2.2.2/README.md
--rw-rw-rw-   0        0        0       42 2023-07-05 00:56:55.796323 yplib-2.2.2/setup.cfg
--rw-rw-rw-   0        0        0      513 2023-07-05 00:56:11.000000 yplib-2.2.2/setup.py
-drwxrwxrwx   0        0        0        0 2023-07-05 00:56:55.792000 yplib-2.2.2/yplib/
--rw-rw-rw-   0        0        0      617 2023-07-03 01:30:34.000000 yplib-2.2.2/yplib/__init__.py
--rw-rw-rw-   0        0        0    12428 2023-07-04 00:52:40.000000 yplib-2.2.2/yplib/chart.py
--rw-rw-rw-   0        0        0     8406 2023-07-03 06:54:51.000000 yplib-2.2.2/yplib/chart_html.py
--rw-rw-rw-   0        0        0      838 2023-06-26 01:33:00.000000 yplib-2.2.2/yplib/db.py
--rw-rw-rw-   0        0        0     4002 2023-06-29 01:38:59.000000 yplib-2.2.2/yplib/file.py
--rw-rw-rw-   0        0        0     3471 2023-06-19 01:33:36.000000 yplib-2.2.2/yplib/http_util.py
--rw-rw-rw-   0        0        0    30121 2023-07-05 00:55:47.000000 yplib-2.2.2/yplib/index.py
--rw-rw-rw-   0        0        0     6196 2023-06-30 06:17:57.000000 yplib-2.2.2/yplib/mail.py
--rw-rw-rw-   0        0        0     3881 2023-06-30 02:49:14.000000 yplib-2.2.2/yplib/mail_html.py
--rw-rw-rw-   0        0        0     5417 2023-07-03 01:47:01.000000 yplib-2.2.2/yplib/markdown.py
--rw-rw-rw-   0        0        0      124 2023-06-25 07:57:19.000000 yplib-2.2.2/yplib/temp.py
-drwxrwxrwx   0        0        0        0 2023-07-05 00:56:55.794845 yplib-2.2.2/yplib.egg-info/
--rw-rw-rw-   0        0        0      352 2023-07-05 00:56:55.000000 yplib-2.2.2/yplib.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      320 2023-07-05 00:56:55.000000 yplib-2.2.2/yplib.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-05 00:56:55.000000 yplib-2.2.2/yplib.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        6 2023-07-05 00:56:55.000000 yplib-2.2.2/yplib.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-07-05 01:20:53.792203 yplib-2.2.3/
+-rw-rw-rw-   0        0        0     1091 2023-06-08 01:05:18.000000 yplib-2.2.3/LICENSE
+-rw-rw-rw-   0        0        0      352 2023-07-05 01:20:53.792203 yplib-2.2.3/PKG-INFO
+-rw-rw-rw-   0        0        0       13 2023-06-14 02:50:41.000000 yplib-2.2.3/README.md
+-rw-rw-rw-   0        0        0       42 2023-07-05 01:20:53.792795 yplib-2.2.3/setup.cfg
+-rw-rw-rw-   0        0        0      513 2023-07-05 01:20:39.000000 yplib-2.2.3/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-05 01:20:53.784249 yplib-2.2.3/yplib/
+-rw-rw-rw-   0        0        0      617 2023-07-03 01:30:34.000000 yplib-2.2.3/yplib/__init__.py
+-rw-rw-rw-   0        0        0    12428 2023-07-04 00:52:40.000000 yplib-2.2.3/yplib/chart.py
+-rw-rw-rw-   0        0        0     8406 2023-07-03 06:54:51.000000 yplib-2.2.3/yplib/chart_html.py
+-rw-rw-rw-   0        0        0      838 2023-06-26 01:33:00.000000 yplib-2.2.3/yplib/db.py
+-rw-rw-rw-   0        0        0     4002 2023-06-29 01:38:59.000000 yplib-2.2.3/yplib/file.py
+-rw-rw-rw-   0        0        0     3471 2023-06-19 01:33:36.000000 yplib-2.2.3/yplib/http_util.py
+-rw-rw-rw-   0        0        0    30220 2023-07-05 01:20:16.000000 yplib-2.2.3/yplib/index.py
+-rw-rw-rw-   0        0        0     6196 2023-06-30 06:17:57.000000 yplib-2.2.3/yplib/mail.py
+-rw-rw-rw-   0        0        0     3881 2023-06-30 02:49:14.000000 yplib-2.2.3/yplib/mail_html.py
+-rw-rw-rw-   0        0        0     5417 2023-07-03 01:47:01.000000 yplib-2.2.3/yplib/markdown.py
+-rw-rw-rw-   0        0        0      124 2023-06-25 07:57:19.000000 yplib-2.2.3/yplib/temp.py
+drwxrwxrwx   0        0        0        0 2023-07-05 01:20:53.791474 yplib-2.2.3/yplib.egg-info/
+-rw-rw-rw-   0        0        0      352 2023-07-05 01:20:53.000000 yplib-2.2.3/yplib.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      320 2023-07-05 01:20:53.000000 yplib-2.2.3/yplib.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-05 01:20:53.000000 yplib-2.2.3/yplib.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        6 2023-07-05 01:20:53.000000 yplib-2.2.3/yplib.egg-info/top_level.txt
```

### Comparing `yplib-2.2.2/LICENSE` & `yplib-2.2.3/LICENSE`

 * *Files identical despite different names*

### Comparing `yplib-2.2.2/setup.py` & `yplib-2.2.3/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r") as fh:
   long_description = fh.read()
 
 setuptools.setup(
   name="yplib",
-  version="2.2.2",
+  version="2.2.3",
   author="yangpu",
   author_email="wantwaterfish@gmail.com",
   description="util",
   long_description=long_description,
   long_description_content_type="text/markdown",
   packages=setuptools.find_packages(),
   classifiers=[
```

### Comparing `yplib-2.2.2/yplib/__init__.py` & `yplib-2.2.3/yplib/__init__.py`

 * *Files identical despite different names*

### Comparing `yplib-2.2.2/yplib/chart.py` & `yplib-2.2.3/yplib/chart.py`

 * *Files identical despite different names*

### Comparing `yplib-2.2.2/yplib/chart_html.py` & `yplib-2.2.3/yplib/chart_html.py`

 * *Files identical despite different names*

### Comparing `yplib-2.2.2/yplib/db.py` & `yplib-2.2.3/yplib/db.py`

 * *Files identical despite different names*

### Comparing `yplib-2.2.2/yplib/file.py` & `yplib-2.2.3/yplib/file.py`

 * *Files identical despite different names*

### Comparing `yplib-2.2.2/yplib/http_util.py` & `yplib-2.2.3/yplib/http_util.py`

 * *Files identical despite different names*

### Comparing `yplib-2.2.2/yplib/index.py` & `yplib-2.2.3/yplib/index.py`

 * *Files 0% similar despite different names*

```diff
@@ -549,20 +549,23 @@
         for d_o in data_list:
             n_l_f = False
             # 这一行, 等于 sep_line
             if sep_line is not None and d_o == sep_line:
                 n_l_f = True
             # 这一行, 包含 sep_line_contain
             elif sep_line_contain is not None and d_o.find(sep_line_contain) != -1:
+                t_l.append(d_o)
                 n_l_f = True
             # 这一行, 是否是以 sep_line_prefix 开头
             elif sep_line_prefix is not None and d_o.startswith(sep_line_prefix):
+                t_l.append(d_o)
                 n_l_f = True
             # 这一行, 是否是以 sep_line_suffix 结尾
             elif sep_line_suffix is not None and d_o.endswith(sep_line_suffix):
+                t_l.append(d_o)
                 n_l_f = True
             if n_l_f:
                 if len(t_l):
                     r_list.append(t_l)
                 t_l = []
             else:
                 t_l.append(d_o)
```

### Comparing `yplib-2.2.2/yplib/mail.py` & `yplib-2.2.3/yplib/mail.py`

 * *Files identical despite different names*

### Comparing `yplib-2.2.2/yplib/mail_html.py` & `yplib-2.2.3/yplib/mail_html.py`

 * *Files identical despite different names*

### Comparing `yplib-2.2.2/yplib/markdown.py` & `yplib-2.2.3/yplib/markdown.py`

 * *Files identical despite different names*

