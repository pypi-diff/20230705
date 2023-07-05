# Comparing `tmp/yplib-2.2.1.tar.gz` & `tmp/yplib-2.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\yplib-2.2.1.tar", last modified: Wed Jul  5 00:39:06 2023, max compression
+gzip compressed data, was "dist\yplib-2.2.2.tar", last modified: Wed Jul  5 00:56:55 2023, max compression
```

## Comparing `yplib-2.2.1.tar` & `yplib-2.2.2.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxrwxrwx   0        0        0        0 2023-07-05 00:39:06.345252 yplib-2.2.1/
--rw-rw-rw-   0        0        0     1091 2023-06-08 01:05:18.000000 yplib-2.2.1/LICENSE
--rw-rw-rw-   0        0        0      352 2023-07-05 00:39:06.344352 yplib-2.2.1/PKG-INFO
--rw-rw-rw-   0        0        0       13 2023-06-14 02:50:41.000000 yplib-2.2.1/README.md
--rw-rw-rw-   0        0        0       42 2023-07-05 00:39:06.345542 yplib-2.2.1/setup.cfg
--rw-rw-rw-   0        0        0      513 2023-07-05 00:38:39.000000 yplib-2.2.1/setup.py
-drwxrwxrwx   0        0        0        0 2023-07-05 00:39:06.342107 yplib-2.2.1/yplib/
--rw-rw-rw-   0        0        0      617 2023-07-03 01:30:34.000000 yplib-2.2.1/yplib/__init__.py
--rw-rw-rw-   0        0        0    12428 2023-07-04 00:52:40.000000 yplib-2.2.1/yplib/chart.py
--rw-rw-rw-   0        0        0     8406 2023-07-03 06:54:51.000000 yplib-2.2.1/yplib/chart_html.py
--rw-rw-rw-   0        0        0      838 2023-06-26 01:33:00.000000 yplib-2.2.1/yplib/db.py
--rw-rw-rw-   0        0        0     4002 2023-06-29 01:38:59.000000 yplib-2.2.1/yplib/file.py
--rw-rw-rw-   0        0        0     3471 2023-06-19 01:33:36.000000 yplib-2.2.1/yplib/http_util.py
--rw-rw-rw-   0        0        0    28973 2023-07-05 00:38:24.000000 yplib-2.2.1/yplib/index.py
--rw-rw-rw-   0        0        0     6196 2023-06-30 06:17:57.000000 yplib-2.2.1/yplib/mail.py
--rw-rw-rw-   0        0        0     3881 2023-06-30 02:49:14.000000 yplib-2.2.1/yplib/mail_html.py
--rw-rw-rw-   0        0        0     5417 2023-07-03 01:47:01.000000 yplib-2.2.1/yplib/markdown.py
--rw-rw-rw-   0        0        0      124 2023-06-25 07:57:19.000000 yplib-2.2.1/yplib/temp.py
-drwxrwxrwx   0        0        0        0 2023-07-05 00:39:06.344352 yplib-2.2.1/yplib.egg-info/
--rw-rw-rw-   0        0        0      352 2023-07-05 00:39:06.000000 yplib-2.2.1/yplib.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      320 2023-07-05 00:39:06.000000 yplib-2.2.1/yplib.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-05 00:39:06.000000 yplib-2.2.1/yplib.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        6 2023-07-05 00:39:06.000000 yplib-2.2.1/yplib.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-07-05 00:56:55.795673 yplib-2.2.2/
+-rw-rw-rw-   0        0        0     1091 2023-06-08 01:05:18.000000 yplib-2.2.2/LICENSE
+-rw-rw-rw-   0        0        0      352 2023-07-05 00:56:55.795122 yplib-2.2.2/PKG-INFO
+-rw-rw-rw-   0        0        0       13 2023-06-14 02:50:41.000000 yplib-2.2.2/README.md
+-rw-rw-rw-   0        0        0       42 2023-07-05 00:56:55.796323 yplib-2.2.2/setup.cfg
+-rw-rw-rw-   0        0        0      513 2023-07-05 00:56:11.000000 yplib-2.2.2/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-05 00:56:55.792000 yplib-2.2.2/yplib/
+-rw-rw-rw-   0        0        0      617 2023-07-03 01:30:34.000000 yplib-2.2.2/yplib/__init__.py
+-rw-rw-rw-   0        0        0    12428 2023-07-04 00:52:40.000000 yplib-2.2.2/yplib/chart.py
+-rw-rw-rw-   0        0        0     8406 2023-07-03 06:54:51.000000 yplib-2.2.2/yplib/chart_html.py
+-rw-rw-rw-   0        0        0      838 2023-06-26 01:33:00.000000 yplib-2.2.2/yplib/db.py
+-rw-rw-rw-   0        0        0     4002 2023-06-29 01:38:59.000000 yplib-2.2.2/yplib/file.py
+-rw-rw-rw-   0        0        0     3471 2023-06-19 01:33:36.000000 yplib-2.2.2/yplib/http_util.py
+-rw-rw-rw-   0        0        0    30121 2023-07-05 00:55:47.000000 yplib-2.2.2/yplib/index.py
+-rw-rw-rw-   0        0        0     6196 2023-06-30 06:17:57.000000 yplib-2.2.2/yplib/mail.py
+-rw-rw-rw-   0        0        0     3881 2023-06-30 02:49:14.000000 yplib-2.2.2/yplib/mail_html.py
+-rw-rw-rw-   0        0        0     5417 2023-07-03 01:47:01.000000 yplib-2.2.2/yplib/markdown.py
+-rw-rw-rw-   0        0        0      124 2023-06-25 07:57:19.000000 yplib-2.2.2/yplib/temp.py
+drwxrwxrwx   0        0        0        0 2023-07-05 00:56:55.794845 yplib-2.2.2/yplib.egg-info/
+-rw-rw-rw-   0        0        0      352 2023-07-05 00:56:55.000000 yplib-2.2.2/yplib.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      320 2023-07-05 00:56:55.000000 yplib-2.2.2/yplib.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-05 00:56:55.000000 yplib-2.2.2/yplib.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        6 2023-07-05 00:56:55.000000 yplib-2.2.2/yplib.egg-info/top_level.txt
```

### Comparing `yplib-2.2.1/LICENSE` & `yplib-2.2.2/LICENSE`

 * *Files identical despite different names*

### Comparing `yplib-2.2.1/setup.py` & `yplib-2.2.2/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r") as fh:
   long_description = fh.read()
 
 setuptools.setup(
   name="yplib",
-  version="2.2.1",
+  version="2.2.2",
   author="yangpu",
   author_email="wantwaterfish@gmail.com",
   description="util",
   long_description=long_description,
   long_description_content_type="text/markdown",
   packages=setuptools.find_packages(),
   classifiers=[
```

### Comparing `yplib-2.2.1/yplib/__init__.py` & `yplib-2.2.2/yplib/__init__.py`

 * *Files identical despite different names*

### Comparing `yplib-2.2.1/yplib/chart.py` & `yplib-2.2.2/yplib/chart.py`

 * *Files identical despite different names*

### Comparing `yplib-2.2.1/yplib/chart_html.py` & `yplib-2.2.2/yplib/chart_html.py`

 * *Files identical despite different names*

### Comparing `yplib-2.2.1/yplib/db.py` & `yplib-2.2.2/yplib/db.py`

 * *Files identical despite different names*

### Comparing `yplib-2.2.1/yplib/file.py` & `yplib-2.2.2/yplib/file.py`

 * *Files identical despite different names*

### Comparing `yplib-2.2.1/yplib/http_util.py` & `yplib-2.2.2/yplib/http_util.py`

 * *Files identical despite different names*

### Comparing `yplib-2.2.1/yplib/index.py` & `yplib-2.2.2/yplib/index.py`

 * *Files 1% similar despite different names*

```diff
@@ -14,14 +14,21 @@
 
 # 记录日志, 如果是对象会转化为 json
 def to_print(a1='tag', a2='', a3='', a4='', a5='', a6='', a7='', a8='', a9='', a10='', a11='', a12='',
              a13='', a14='', a15='', a16='', a17='', a18='', a19='', a20=''):
     return to_log(a1, a2, a3, a4, a5, a6, a7, a8, a9, a10, a11, a12, a13, a14, a15, a16, a17, a18, a19, a20, time_prefix=False)
 
 
+# 将 log 数据, 写入到文件
+def to_print_file(a1='tag', a2='', a3='', a4='', a5='', a6='', a7='', a8='', a9='', a10='', a11='', a12='',
+                  a13='', a14='', a15='', a16='', a17='', a18='', a19='', a20=''):
+    lo = to_print(a1, a2, a3, a4, a5, a6, a7, a8, a9, a10, a11, a12, a13, a14, a15, a16, a17, a18, a19, a20)
+    to_txt([lo], datetime.today().strftime('%Y-%m-%d'), 'print', True, '.txt')
+
+
 # 记录日志, 如果是对象会转化为 json
 def to_log(a1='tag', a2='', a3='', a4='', a5='', a6='', a7='', a8='', a9='', a10='', a11='', a12='',
            a13='', a14='', a15='', a16='', a17='', a18='', a19='', a20='', time_prefix=True):
     l = [a1, a2, a3, a4, a5, a6, a7, a8, a9, a10,
          a11, a12, a13, a14, a15, a16, a17, a18, a19, a20]
     d = ''
     for one in l:
@@ -471,24 +478,28 @@
 
 # 将 txt 文件转化成 list 的方法
 # 当读取 txt 之类的文件的时候
 # 将 txt 文件读取到 list 中, 每一行自动过滤掉行前行后的特殊字符
 # sep : 是否对每一行进行分割,如果存在这个字段,就分割
 # sep_line : 这一行是一个分隔符, 返回的是一个 list(list)
 # sep_line_contain : 这一行是一个分隔符,包含这个行分隔符的做分割, 返回的是一个 list(list)
+# sep_line_prefix : 这一行是一个分隔符,以这个分隔符作为前缀的, 返回的是一个 list(list)
+# sep_line_suffix : 这一行是一个分隔符,以这个分隔符作为后缀的, 返回的是一个 list(list)
 # sep_all : 将文件转化成一个字符串,然后对这个字符串,再次总体分割
 # start_index : 从这个地方开始读取,从1开始标号 , 包含这一行
 # start_line :  从这个地方开始读取,从第一行开始找到这个字符串开始标记 , 包含这一行
 # end_index :   读取到这个地方结束,从1开始标号 , 不包含这一行
 # end_line :    读取到这个地方结束,从第一行开始找到这个字符串开始标记 , 不包含这一行
 # count :       读取指定的行数
 def to_list_from_txt(file_name='a.txt',
                      sep=None,
                      sep_line=None,
                      sep_line_contain=None,
+                     sep_line_prefix=None,
+                     sep_line_suffix=None,
                      sep_all=None,
                      start_index=None,
                      start_line=None,
                      end_index=None,
                      end_line=None,
                      count=None):
     if file_is_empty(file_name=file_name):
@@ -528,25 +539,31 @@
         if sep is not None:
             data_list.append(line.split(str(sep)))
         else:
             data_list.append(line)
     if sep_all is not None:
         data_list = ''.join(data_list).split(str(sep_all))
     # 有行分隔符
-    if sep_line is not None or sep_line_contain is not None:
+    if sep_line is not None or sep_line_contain is not None or sep_line_prefix is not None or sep_line_suffix is not None:
         r_list = []
         t_l = []
         for d_o in data_list:
             n_l_f = False
             # 这一行, 等于 sep_line
             if sep_line is not None and d_o == sep_line:
                 n_l_f = True
             # 这一行, 包含 sep_line_contain
             elif sep_line_contain is not None and d_o.find(sep_line_contain) != -1:
                 n_l_f = True
+            # 这一行, 是否是以 sep_line_prefix 开头
+            elif sep_line_prefix is not None and d_o.startswith(sep_line_prefix):
+                n_l_f = True
+            # 这一行, 是否是以 sep_line_suffix 结尾
+            elif sep_line_suffix is not None and d_o.endswith(sep_line_suffix):
+                n_l_f = True
             if n_l_f:
                 if len(t_l):
                     r_list.append(t_l)
                 t_l = []
             else:
                 t_l.append(d_o)
         if len(t_l):
```

### Comparing `yplib-2.2.1/yplib/mail.py` & `yplib-2.2.2/yplib/mail.py`

 * *Files identical despite different names*

### Comparing `yplib-2.2.1/yplib/mail_html.py` & `yplib-2.2.2/yplib/mail_html.py`

 * *Files identical despite different names*

### Comparing `yplib-2.2.1/yplib/markdown.py` & `yplib-2.2.2/yplib/markdown.py`

 * *Files identical despite different names*

