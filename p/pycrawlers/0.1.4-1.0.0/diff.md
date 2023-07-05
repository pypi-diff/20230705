# Comparing `tmp/pycrawlers-0.1.4.tar.gz` & `tmp/pycrawlers-1.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pycrawlers-0.1.4.tar", last modified: Fri Jun 30 09:58:25 2023, max compression
+gzip compressed data, was "pycrawlers-1.0.0.tar", last modified: Wed Jul  5 05:39:39 2023, max compression
```

## Comparing `pycrawlers-0.1.4.tar` & `pycrawlers-1.0.0.tar`

### file list

```diff
@@ -1,30 +1,30 @@
-drwxr-xr-x   0 bo         (501) staff       (20)        0 2023-06-30 09:58:25.053035 pycrawlers-0.1.4/
--rw-r--r--   0 bo         (501) staff       (20)    11357 2022-08-16 07:24:33.000000 pycrawlers-0.1.4/LICENSE
--rw-r--r--   0 bo         (501) staff       (20)     2948 2023-06-30 09:58:25.052900 pycrawlers-0.1.4/PKG-INFO
--rw-r--r--   0 bo         (501) staff       (20)     2491 2023-06-30 09:56:53.000000 pycrawlers-0.1.4/README.md
-drwxr-xr-x   0 bo         (501) staff       (20)        0 2023-06-30 09:58:25.049671 pycrawlers-0.1.4/other/
--rw-r--r--   0 bo         (501) staff       (20)       73 2022-08-17 07:58:18.000000 pycrawlers-0.1.4/other/__init__.py
--rw-r--r--   0 bo         (501) staff       (20)      745 2022-08-17 09:04:51.000000 pycrawlers-0.1.4/other/dw_hg.py
-drwxr-xr-x   0 bo         (501) staff       (20)        0 2023-06-30 09:58:25.049879 pycrawlers-0.1.4/pycrawlers/
--rw-r--r--   0 bo         (501) staff       (20)      232 2023-06-30 09:44:44.000000 pycrawlers-0.1.4/pycrawlers/__init__.py
-drwxr-xr-x   0 bo         (501) staff       (20)        0 2023-06-30 09:58:25.051048 pycrawlers-0.1.4/pycrawlers/common/
--rw-r--r--   0 bo         (501) staff       (20)       73 2022-08-17 07:44:00.000000 pycrawlers-0.1.4/pycrawlers/common/__init__.py
--rw-r--r--   0 bo         (501) staff       (20)     2644 2023-06-21 08:33:43.000000 pycrawlers-0.1.4/pycrawlers/common/default_data.py
--rw-r--r--   0 bo         (501) staff       (20)     4962 2023-06-21 09:14:16.000000 pycrawlers-0.1.4/pycrawlers/common/tools.py
-drwxr-xr-x   0 bo         (501) staff       (20)        0 2023-06-30 09:58:25.051455 pycrawlers-0.1.4/pycrawlers/huggingfaces/
--rw-r--r--   0 bo         (501) staff       (20)       73 2022-08-17 08:04:35.000000 pycrawlers-0.1.4/pycrawlers/huggingfaces/__init__.py
--rw-r--r--   0 bo         (501) staff       (20)     4657 2023-02-16 06:57:07.000000 pycrawlers-0.1.4/pycrawlers/huggingfaces/download.py
-drwxr-xr-x   0 bo         (501) staff       (20)        0 2023-06-30 09:58:25.052593 pycrawlers-0.1.4/pycrawlers/websites/
--rw-r--r--   0 bo         (501) staff       (20)       75 2023-06-25 03:29:06.000000 pycrawlers-0.1.4/pycrawlers/websites/__init__.py
--rw-r--r--   0 bo         (501) staff       (20)     2239 2023-06-25 05:57:32.000000 pycrawlers-0.1.4/pycrawlers/websites/get_web_page.py
--rw-r--r--   0 bo         (501) staff       (20)     3607 2023-06-30 07:03:43.000000 pycrawlers-0.1.4/pycrawlers/websites/get_web_page_id.py
--rw-r--r--   0 bo         (501) staff       (20)      882 2023-06-30 09:44:44.000000 pycrawlers-0.1.4/pycrawlers/websites/get_websites.py
--rw-r--r--   0 bo         (501) staff       (20)      568 2023-06-30 07:15:34.000000 pycrawlers-0.1.4/pycrawlers/websites/url_filters.py
-drwxr-xr-x   0 bo         (501) staff       (20)        0 2023-06-30 09:58:25.050560 pycrawlers-0.1.4/pycrawlers.egg-info/
--rw-r--r--   0 bo         (501) staff       (20)     2948 2023-06-30 09:58:24.000000 pycrawlers-0.1.4/pycrawlers.egg-info/PKG-INFO
--rw-r--r--   0 bo         (501) staff       (20)      592 2023-06-30 09:58:25.000000 pycrawlers-0.1.4/pycrawlers.egg-info/SOURCES.txt
--rw-r--r--   0 bo         (501) staff       (20)        1 2023-06-30 09:58:24.000000 pycrawlers-0.1.4/pycrawlers.egg-info/dependency_links.txt
--rw-r--r--   0 bo         (501) staff       (20)       71 2023-06-30 09:58:24.000000 pycrawlers-0.1.4/pycrawlers.egg-info/requires.txt
--rw-r--r--   0 bo         (501) staff       (20)       17 2023-06-30 09:58:24.000000 pycrawlers-0.1.4/pycrawlers.egg-info/top_level.txt
--rw-r--r--   0 bo         (501) staff       (20)       38 2023-06-30 09:58:25.053081 pycrawlers-0.1.4/setup.cfg
--rw-r--r--   0 bo         (501) staff       (20)      907 2023-06-30 09:57:42.000000 pycrawlers-0.1.4/setup.py
+drwxr-xr-x   0 bo         (501) staff       (20)        0 2023-07-05 05:39:39.899920 pycrawlers-1.0.0/
+-rw-r--r--   0 bo         (501) staff       (20)    11357 2022-08-16 07:24:33.000000 pycrawlers-1.0.0/LICENSE
+-rw-r--r--   0 bo         (501) staff       (20)     2948 2023-07-05 05:39:39.899780 pycrawlers-1.0.0/PKG-INFO
+-rw-r--r--   0 bo         (501) staff       (20)     2491 2023-06-30 09:56:53.000000 pycrawlers-1.0.0/README.md
+drwxr-xr-x   0 bo         (501) staff       (20)        0 2023-07-05 05:39:39.896185 pycrawlers-1.0.0/other/
+-rw-r--r--   0 bo         (501) staff       (20)       73 2022-08-17 07:58:18.000000 pycrawlers-1.0.0/other/__init__.py
+-rw-r--r--   0 bo         (501) staff       (20)      745 2022-08-17 09:04:51.000000 pycrawlers-1.0.0/other/dw_hg.py
+drwxr-xr-x   0 bo         (501) staff       (20)        0 2023-07-05 05:39:39.896375 pycrawlers-1.0.0/pycrawlers/
+-rw-r--r--   0 bo         (501) staff       (20)      232 2023-06-30 09:44:44.000000 pycrawlers-1.0.0/pycrawlers/__init__.py
+drwxr-xr-x   0 bo         (501) staff       (20)        0 2023-07-05 05:39:39.897535 pycrawlers-1.0.0/pycrawlers/common/
+-rw-r--r--   0 bo         (501) staff       (20)       73 2022-08-17 07:44:00.000000 pycrawlers-1.0.0/pycrawlers/common/__init__.py
+-rw-r--r--   0 bo         (501) staff       (20)     2644 2023-06-21 08:33:43.000000 pycrawlers-1.0.0/pycrawlers/common/default_data.py
+-rw-r--r--   0 bo         (501) staff       (20)     5356 2023-07-05 03:46:40.000000 pycrawlers-1.0.0/pycrawlers/common/tools.py
+drwxr-xr-x   0 bo         (501) staff       (20)        0 2023-07-05 05:39:39.898027 pycrawlers-1.0.0/pycrawlers/huggingfaces/
+-rw-r--r--   0 bo         (501) staff       (20)       73 2022-08-17 08:04:35.000000 pycrawlers-1.0.0/pycrawlers/huggingfaces/__init__.py
+-rw-r--r--   0 bo         (501) staff       (20)     5106 2023-07-05 03:33:48.000000 pycrawlers-1.0.0/pycrawlers/huggingfaces/download.py
+drwxr-xr-x   0 bo         (501) staff       (20)        0 2023-07-05 05:39:39.899258 pycrawlers-1.0.0/pycrawlers/websites/
+-rw-r--r--   0 bo         (501) staff       (20)       75 2023-06-25 03:29:06.000000 pycrawlers-1.0.0/pycrawlers/websites/__init__.py
+-rw-r--r--   0 bo         (501) staff       (20)     2239 2023-06-25 05:57:32.000000 pycrawlers-1.0.0/pycrawlers/websites/get_web_page.py
+-rw-r--r--   0 bo         (501) staff       (20)     3607 2023-06-30 07:03:43.000000 pycrawlers-1.0.0/pycrawlers/websites/get_web_page_id.py
+-rw-r--r--   0 bo         (501) staff       (20)      882 2023-06-30 09:44:44.000000 pycrawlers-1.0.0/pycrawlers/websites/get_websites.py
+-rw-r--r--   0 bo         (501) staff       (20)      568 2023-06-30 07:15:34.000000 pycrawlers-1.0.0/pycrawlers/websites/url_filters.py
+drwxr-xr-x   0 bo         (501) staff       (20)        0 2023-07-05 05:39:39.896964 pycrawlers-1.0.0/pycrawlers.egg-info/
+-rw-r--r--   0 bo         (501) staff       (20)     2948 2023-07-05 05:39:39.000000 pycrawlers-1.0.0/pycrawlers.egg-info/PKG-INFO
+-rw-r--r--   0 bo         (501) staff       (20)      592 2023-07-05 05:39:39.000000 pycrawlers-1.0.0/pycrawlers.egg-info/SOURCES.txt
+-rw-r--r--   0 bo         (501) staff       (20)        1 2023-07-05 05:39:39.000000 pycrawlers-1.0.0/pycrawlers.egg-info/dependency_links.txt
+-rw-r--r--   0 bo         (501) staff       (20)       71 2023-07-05 05:39:39.000000 pycrawlers-1.0.0/pycrawlers.egg-info/requires.txt
+-rw-r--r--   0 bo         (501) staff       (20)       17 2023-07-05 05:39:39.000000 pycrawlers-1.0.0/pycrawlers.egg-info/top_level.txt
+-rw-r--r--   0 bo         (501) staff       (20)       38 2023-07-05 05:39:39.899961 pycrawlers-1.0.0/setup.cfg
+-rw-r--r--   0 bo         (501) staff       (20)      907 2023-07-05 03:49:19.000000 pycrawlers-1.0.0/setup.py
```

### Comparing `pycrawlers-0.1.4/LICENSE` & `pycrawlers-1.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `pycrawlers-0.1.4/PKG-INFO` & `pycrawlers-1.0.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pycrawlers
-Version: 0.1.4
+Version: 1.0.0
 Summary: A collection of Crawlers
 Home-page: https://gitee.com/maxbanana
 Author: hongbo liu
 Author-email: 782027465@qq.com
 License: Apache
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
```

### Comparing `pycrawlers-0.1.4/README.md` & `pycrawlers-1.0.0/README.md`

 * *Files identical despite different names*

### Comparing `pycrawlers-0.1.4/other/dw_hg.py` & `pycrawlers-1.0.0/other/dw_hg.py`

 * *Files identical despite different names*

### Comparing `pycrawlers-0.1.4/pycrawlers/common/default_data.py` & `pycrawlers-1.0.0/pycrawlers/common/default_data.py`

 * *Files identical despite different names*

### Comparing `pycrawlers-0.1.4/pycrawlers/common/tools.py` & `pycrawlers-1.0.0/pycrawlers/common/tools.py`

 * *Files 7% similar despite different names*

```diff
@@ -37,31 +37,42 @@
                 return response
             except requests.RequestException as e:
                 print(e)
         return wrapped_function
 
 
 # 下载数据
-def download(url: str, fname: str, headers: dict, read_timeout: int = 15):
+def download(url: str, fname: str, headers: dict, read_timeout: int = 15, file_size=None):
+    if 'Range' in headers:
+        del headers['Range']
+
     @DealException()
     def get_data():
         return requests_session.get(url, headers=headers, stream=True, timeout=(read_timeout, 5))
-
-    resp = get_data()
-    total = int(resp.headers.get('content-length', 0))
-    with open(fname, 'wb') as file, tqdm(
-        desc=fname,
-        total=total,
-        unit='iB',
-        unit_scale=True,
-        unit_divisor=1024,
-    ) as bar:
-        for data in resp.iter_content(chunk_size=1024):
-            size = file.write(data)
-            bar.update(size)
+    resp_ = get_data()
+    total_ = int(resp_.headers.get('content-length', 0))
+    if file_size < total_:
+        file_op = 'wb'
+        if file_size:
+            headers['Range'] = f'bytes={file_size}-'
+            file_op = 'ab'
+        resp = get_data()
+        total = int(resp.headers.get('content-length', 0))
+        with open(fname, file_op) as file, tqdm(
+            desc=fname,
+            total=total,
+            unit='iB',
+            unit_scale=True,
+            unit_divisor=1024,
+        ) as bar:
+            for data in resp.iter_content(chunk_size=1024):
+                size = file.write(data)
+                bar.update(size)
+    else:
+        print(fname, ' ✅')
 
 
 def juedge_path(file_path: str):
     """判断路径是否存在，不存在就创建"""
     if not os.path.exists(file_path):
         os.makedirs(file_path)
     if file_path[-1] != '/':
```

### Comparing `pycrawlers-0.1.4/pycrawlers/huggingfaces/download.py` & `pycrawlers-1.0.0/pycrawlers/huggingfaces/download.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 # -*- coding: UTF-8 -*-
 # @Time : 2022/8/17 15:38 
 # @Author : 刘洪波
 
 """
 获取hugging face 模型
 """
+import os
 import time
 from lxml import etree
 from pycrawlers.common.default_data import headers
 from pycrawlers.common.tools import requests_session
 from pycrawlers.common.tools import DealException
 from pycrawlers.common.tools import download
 from pycrawlers.common.tools import juedge_path
@@ -37,17 +38,17 @@
             self.html_data = etree.HTML(response.content)
             # print(self.html_data)
             file_names = self.get_file_names()
             file_urls = self.get_file_urls()
             # print(file_urls)
             # print(file_names)
             files_path = juedge_path(file_save_path) if file_save_path else juedge_path('./' + _url[-3] + '/')
-            print(f"{'$' * 30}{' ' * 5}开始下载：{_url[-3]}{' ' * 5}{'$' * 30}")
+            print(f"{'🔴' * 10}{' ' * 5}Start downloading: {_url[-3]}{' ' * 5}{'🔴' * 10}")
             self.get_files(file_names, file_urls, files_path)
-            print(f"{'$' * 30}{' ' * 5}完成下载{' ' * 5}{'$' * 30}")
+            print(f"{'🟢' * 10}{' ' * 5}Download completed{' ' * 5}{'🟢' * 10}")
 
     def get_batch_data(self, urls: list, file_save_paths: list = None, count_info=True):
         """
         批量获取数据
         :param urls: ['https://huggingface.co/albert-base-v2/tree/main',
                       'https://huggingface.co/dmis-lab/biosyn-sapbert-bc5cdr-disease/tree/main']
         :param file_save_paths:['./model_1/albert-base-v2', './model_2/']
@@ -106,17 +107,30 @@
         """生成路径"""
         return juedge_path('./' + _url[-3] + '/')
 
     def get_files(self, file_names, file_urls, files_path):
         for name, part_url in zip(file_names, file_urls):
             if name in part_url:
                 url = self.base_url + part_url
-                download(url, files_path + name, headers, read_timeout=60)
+                save_file_path = files_path + name
+                download(url, save_file_path, headers, read_timeout=60, file_size=self.get_file_size(save_file_path))
                 time.sleep(0.5)
 
     @staticmethod
     def count_info(success_urls, fail_urls):
         print(f'程序执行统计：')
         print(f'a. 成功{str(len(success_urls))}个')
         print(f'b. 失败{str(len(fail_urls))}个')
         print(f'c. 成功的URL：{"，".join(success_urls)}')
         print(f'd. 失败的URL：{"，".join(fail_urls)}')
+
+    @staticmethod
+    def get_file_size(file_path):
+        """
+        获取文件大小
+        :param:  file_path:文件路径（带文件名）
+        :return: file_size：文件大小
+        """
+        if os.path.exists(file_path):
+            return os.path.getsize(file_path)
+        else:
+            return 0
```

### Comparing `pycrawlers-0.1.4/pycrawlers/websites/get_web_page.py` & `pycrawlers-1.0.0/pycrawlers/websites/get_web_page.py`

 * *Files identical despite different names*

### Comparing `pycrawlers-0.1.4/pycrawlers/websites/get_web_page_id.py` & `pycrawlers-1.0.0/pycrawlers/websites/get_web_page_id.py`

 * *Files identical despite different names*

### Comparing `pycrawlers-0.1.4/pycrawlers/websites/get_websites.py` & `pycrawlers-1.0.0/pycrawlers/websites/get_websites.py`

 * *Files identical despite different names*

### Comparing `pycrawlers-0.1.4/pycrawlers/websites/url_filters.py` & `pycrawlers-1.0.0/pycrawlers/websites/url_filters.py`

 * *Files identical despite different names*

### Comparing `pycrawlers-0.1.4/pycrawlers.egg-info/PKG-INFO` & `pycrawlers-1.0.0/pycrawlers.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pycrawlers
-Version: 0.1.4
+Version: 1.0.0
 Summary: A collection of Crawlers
 Home-page: https://gitee.com/maxbanana
 Author: hongbo liu
 Author-email: 782027465@qq.com
 License: Apache
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
```

### Comparing `pycrawlers-0.1.4/pycrawlers.egg-info/SOURCES.txt` & `pycrawlers-1.0.0/pycrawlers.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pycrawlers-0.1.4/setup.py` & `pycrawlers-1.0.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 from setuptools import setup
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setup(
     name='pycrawlers',
-    version='0.1.4',
+    version='1.0.0',
     packages=setuptools.find_packages(),
     url='https://gitee.com/maxbanana',
     license='Apache',
     author='hongbo liu',
     author_email='782027465@qq.com',
     description='A collection of Crawlers',
     long_description=long_description,
```

