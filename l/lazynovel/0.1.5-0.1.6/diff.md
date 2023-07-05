# Comparing `tmp/lazynovel-0.1.5.tar.gz` & `tmp/lazynovel-0.1.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lazynovel-0.1.5.tar", last modified: Wed Jun 28 07:20:07 2023, max compression
+gzip compressed data, was "lazynovel-0.1.6.tar", last modified: Wed Jul  5 07:10:21 2023, max compression
```

## Comparing `lazynovel-0.1.5.tar` & `lazynovel-0.1.6.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxr-xr-x   0 zeroseeker   (501) staff       (20)        0 2023-06-28 07:20:07.651406 lazynovel-0.1.5/
--rw-r--r--   0 zeroseeker   (501) staff       (20)    35181 2023-02-28 06:27:15.000000 lazynovel-0.1.5/LICENSE
--rw-r--r--   0 zeroseeker   (501) staff       (20)     1305 2023-06-28 07:20:07.651290 lazynovel-0.1.5/PKG-INFO
--rw-r--r--   0 zeroseeker   (501) staff       (20)      954 2023-02-28 06:27:15.000000 lazynovel-0.1.5/README.md
-drwxr-xr-x   0 zeroseeker   (501) staff       (20)        0 2023-06-28 07:20:07.650371 lazynovel-0.1.5/lazynovel/
--rw-r--r--   0 zeroseeker   (501) staff       (20)      415 2023-05-25 10:17:10.000000 lazynovel-0.1.5/lazynovel/__init__.py
--rw-r--r--   0 zeroseeker   (501) staff       (20)     6989 2023-05-25 08:04:09.000000 lazynovel-0.1.5/lazynovel/crawler_changdu.py
--rw-r--r--   0 zeroseeker   (501) staff       (20)    10870 2023-06-28 07:17:21.000000 lazynovel-0.1.5/lazynovel/crawler_mbookcn.py
--rw-r--r--   0 zeroseeker   (501) staff       (20)     5902 2023-06-27 08:25:54.000000 lazynovel-0.1.5/lazynovel/crawler_reading163.py
--rw-r--r--   0 zeroseeker   (501) staff       (20)    10568 2023-02-28 06:27:15.000000 lazynovel-0.1.5/lazynovel/open_changdu.py
--rw-r--r--   0 zeroseeker   (501) staff       (20)     9853 2023-02-28 06:27:15.000000 lazynovel-0.1.5/lazynovel/open_dianzhong.py
--rw-r--r--   0 zeroseeker   (501) staff       (20)     9680 2023-02-28 06:27:15.000000 lazynovel-0.1.5/lazynovel/open_mbookcn.py
--rw-r--r--   0 zeroseeker   (501) staff       (20)    21587 2023-05-29 10:32:37.000000 lazynovel-0.1.5/lazynovel/open_reading163.py
--rw-r--r--   0 zeroseeker   (501) staff       (20)      830 2023-02-28 06:27:15.000000 lazynovel-0.1.5/lazynovel/open_yangguang.py
--rw-r--r--   0 zeroseeker   (501) staff       (20)     2694 2023-02-28 06:27:15.000000 lazynovel-0.1.5/lazynovel/open_yiqbook.py
--rw-r--r--   0 zeroseeker   (501) staff       (20)    57844 2023-02-28 06:27:15.000000 lazynovel-0.1.5/lazynovel/open_yuewen.py
-drwxr-xr-x   0 zeroseeker   (501) staff       (20)        0 2023-06-28 07:20:07.651120 lazynovel-0.1.5/lazynovel.egg-info/
--rw-r--r--   0 zeroseeker   (501) staff       (20)     1305 2023-06-28 07:20:07.000000 lazynovel-0.1.5/lazynovel.egg-info/PKG-INFO
--rw-r--r--   0 zeroseeker   (501) staff       (20)      490 2023-06-28 07:20:07.000000 lazynovel-0.1.5/lazynovel.egg-info/SOURCES.txt
--rw-r--r--   0 zeroseeker   (501) staff       (20)        1 2023-06-28 07:20:07.000000 lazynovel-0.1.5/lazynovel.egg-info/dependency_links.txt
--rw-r--r--   0 zeroseeker   (501) staff       (20)       15 2023-06-28 07:20:07.000000 lazynovel-0.1.5/lazynovel.egg-info/requires.txt
--rw-r--r--   0 zeroseeker   (501) staff       (20)       10 2023-06-28 07:20:07.000000 lazynovel-0.1.5/lazynovel.egg-info/top_level.txt
--rw-r--r--   0 zeroseeker   (501) staff       (20)       38 2023-06-28 07:20:07.651450 lazynovel-0.1.5/setup.cfg
--rw-r--r--   0 zeroseeker   (501) staff       (20)      869 2023-06-28 07:17:21.000000 lazynovel-0.1.5/setup.py
+drwxr-xr-x   0 zeroseeker   (501) staff       (20)        0 2023-07-05 07:10:21.238778 lazynovel-0.1.6/
+-rw-r--r--   0 zeroseeker   (501) staff       (20)    35181 2023-02-28 06:27:15.000000 lazynovel-0.1.6/LICENSE
+-rw-r--r--   0 zeroseeker   (501) staff       (20)     1305 2023-07-05 07:10:21.238650 lazynovel-0.1.6/PKG-INFO
+-rw-r--r--   0 zeroseeker   (501) staff       (20)      954 2023-02-28 06:27:15.000000 lazynovel-0.1.6/README.md
+drwxr-xr-x   0 zeroseeker   (501) staff       (20)        0 2023-07-05 07:10:21.237645 lazynovel-0.1.6/lazynovel/
+-rw-r--r--   0 zeroseeker   (501) staff       (20)      415 2023-05-25 10:17:10.000000 lazynovel-0.1.6/lazynovel/__init__.py
+-rw-r--r--   0 zeroseeker   (501) staff       (20)     6989 2023-05-25 08:04:09.000000 lazynovel-0.1.6/lazynovel/crawler_changdu.py
+-rw-r--r--   0 zeroseeker   (501) staff       (20)    10870 2023-06-28 07:17:21.000000 lazynovel-0.1.6/lazynovel/crawler_mbookcn.py
+-rw-r--r--   0 zeroseeker   (501) staff       (20)     5914 2023-07-05 07:09:26.000000 lazynovel-0.1.6/lazynovel/crawler_reading163.py
+-rw-r--r--   0 zeroseeker   (501) staff       (20)    10568 2023-02-28 06:27:15.000000 lazynovel-0.1.6/lazynovel/open_changdu.py
+-rw-r--r--   0 zeroseeker   (501) staff       (20)     9853 2023-02-28 06:27:15.000000 lazynovel-0.1.6/lazynovel/open_dianzhong.py
+-rw-r--r--   0 zeroseeker   (501) staff       (20)     9680 2023-02-28 06:27:15.000000 lazynovel-0.1.6/lazynovel/open_mbookcn.py
+-rw-r--r--   0 zeroseeker   (501) staff       (20)    21587 2023-05-29 10:32:37.000000 lazynovel-0.1.6/lazynovel/open_reading163.py
+-rw-r--r--   0 zeroseeker   (501) staff       (20)      830 2023-02-28 06:27:15.000000 lazynovel-0.1.6/lazynovel/open_yangguang.py
+-rw-r--r--   0 zeroseeker   (501) staff       (20)     2694 2023-02-28 06:27:15.000000 lazynovel-0.1.6/lazynovel/open_yiqbook.py
+-rw-r--r--   0 zeroseeker   (501) staff       (20)    57844 2023-02-28 06:27:15.000000 lazynovel-0.1.6/lazynovel/open_yuewen.py
+drwxr-xr-x   0 zeroseeker   (501) staff       (20)        0 2023-07-05 07:10:21.238435 lazynovel-0.1.6/lazynovel.egg-info/
+-rw-r--r--   0 zeroseeker   (501) staff       (20)     1305 2023-07-05 07:10:21.000000 lazynovel-0.1.6/lazynovel.egg-info/PKG-INFO
+-rw-r--r--   0 zeroseeker   (501) staff       (20)      490 2023-07-05 07:10:21.000000 lazynovel-0.1.6/lazynovel.egg-info/SOURCES.txt
+-rw-r--r--   0 zeroseeker   (501) staff       (20)        1 2023-07-05 07:10:21.000000 lazynovel-0.1.6/lazynovel.egg-info/dependency_links.txt
+-rw-r--r--   0 zeroseeker   (501) staff       (20)       15 2023-07-05 07:10:21.000000 lazynovel-0.1.6/lazynovel.egg-info/requires.txt
+-rw-r--r--   0 zeroseeker   (501) staff       (20)       10 2023-07-05 07:10:21.000000 lazynovel-0.1.6/lazynovel.egg-info/top_level.txt
+-rw-r--r--   0 zeroseeker   (501) staff       (20)       38 2023-07-05 07:10:21.238825 lazynovel-0.1.6/setup.cfg
+-rw-r--r--   0 zeroseeker   (501) staff       (20)      869 2023-07-05 07:09:51.000000 lazynovel-0.1.6/setup.py
```

### Comparing `lazynovel-0.1.5/LICENSE` & `lazynovel-0.1.6/LICENSE`

 * *Files identical despite different names*

### Comparing `lazynovel-0.1.5/PKG-INFO` & `lazynovel-0.1.6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lazynovel
-Version: 0.1.5
+Version: 0.1.6
 Summary: 小说平台接口封包
 Home-page: https://gitee.com/ZeroSeeker/lazynovel
 Author: ZeroSeeker
 Author-email: zeroseeker@foxmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
```

### Comparing `lazynovel-0.1.5/README.md` & `lazynovel-0.1.6/README.md`

 * *Files identical despite different names*

### Comparing `lazynovel-0.1.5/lazynovel/crawler_changdu.py` & `lazynovel-0.1.6/lazynovel/crawler_changdu.py`

 * *Files identical despite different names*

### Comparing `lazynovel-0.1.5/lazynovel/crawler_mbookcn.py` & `lazynovel-0.1.6/lazynovel/crawler_mbookcn.py`

 * *Files identical despite different names*

### Comparing `lazynovel-0.1.5/lazynovel/crawler_reading163.py` & `lazynovel-0.1.6/lazynovel/crawler_reading163.py`

 * *Files 1% similar despite different names*

```diff
@@ -118,15 +118,15 @@
         "title": title,  # 消息名称
         "sendTime": send_time,  # 发送时间（13位时间戳）
         "content": content,  # 消息内容
         "type": msg_type,  # 消息类型，图文消息：0，文字消息：4，图片消息：2
         "siteId": site_id,  # 公众号id
         "sendType": send_type  # 触达人群，全部用户：0，按标签选择：1
     }
-    if recharge_type:
+    if recharge_type is not None:
         json_data['tagInfo'] = json.dumps(
             {
                 'rechargeType': recharge_type,
                 'siteId': site_id
             }
         )
     # print('json_data:', json_data)
```

### Comparing `lazynovel-0.1.5/lazynovel/open_changdu.py` & `lazynovel-0.1.6/lazynovel/open_changdu.py`

 * *Files identical despite different names*

### Comparing `lazynovel-0.1.5/lazynovel/open_dianzhong.py` & `lazynovel-0.1.6/lazynovel/open_dianzhong.py`

 * *Files identical despite different names*

### Comparing `lazynovel-0.1.5/lazynovel/open_mbookcn.py` & `lazynovel-0.1.6/lazynovel/open_mbookcn.py`

 * *Files identical despite different names*

### Comparing `lazynovel-0.1.5/lazynovel/open_reading163.py` & `lazynovel-0.1.6/lazynovel/open_reading163.py`

 * *Files identical despite different names*

### Comparing `lazynovel-0.1.5/lazynovel/open_yangguang.py` & `lazynovel-0.1.6/lazynovel/open_yangguang.py`

 * *Files identical despite different names*

### Comparing `lazynovel-0.1.5/lazynovel/open_yiqbook.py` & `lazynovel-0.1.6/lazynovel/open_yiqbook.py`

 * *Files identical despite different names*

### Comparing `lazynovel-0.1.5/lazynovel/open_yuewen.py` & `lazynovel-0.1.6/lazynovel/open_yuewen.py`

 * *Files identical despite different names*

### Comparing `lazynovel-0.1.5/lazynovel.egg-info/PKG-INFO` & `lazynovel-0.1.6/lazynovel.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lazynovel
-Version: 0.1.5
+Version: 0.1.6
 Summary: 小说平台接口封包
 Home-page: https://gitee.com/ZeroSeeker/lazynovel
 Author: ZeroSeeker
 Author-email: zeroseeker@foxmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
```

### Comparing `lazynovel-0.1.5/setup.py` & `lazynovel-0.1.6/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 import setuptools
 
 with open("README.md", "r", encoding='utf-8') as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="lazynovel",
-    version="0.1.5",
+    version="0.1.6",
     description="小说平台接口封包",
     long_description=long_description,
     long_description_content_type="text/markdown",
     author="ZeroSeeker",
     author_email="zeroseeker@foxmail.com",
     url="https://gitee.com/ZeroSeeker/lazynovel",
     packages=setuptools.find_packages(),
```

