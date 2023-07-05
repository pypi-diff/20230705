# Comparing `tmp/DigiCore-1.0.6.tar.gz` & `tmp/DigiCore-1.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\DigiCore-1.0.6.tar", last modified: Thu Jun 29 02:29:01 2023, max compression
+gzip compressed data, was "dist\DigiCore-1.0.7.tar", last modified: Wed Jul  5 06:41:51 2023, max compression
```

## Comparing `DigiCore-1.0.6.tar` & `DigiCore-1.0.7.tar`

### file list

```diff
@@ -1,48 +1,48 @@
-drwxrwxrwx   0        0        0        0 2023-06-29 02:29:01.172340 DigiCore-1.0.6/
-drwxrwxrwx   0        0        0        0 2023-06-29 02:29:01.129485 DigiCore-1.0.6/DigiCore.egg-info/
--rw-rw-rw-   0        0        0     4014 2023-06-29 02:29:01.000000 DigiCore-1.0.6/DigiCore.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1146 2023-06-29 02:29:01.000000 DigiCore-1.0.6/DigiCore.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-29 02:29:01.000000 DigiCore-1.0.6/DigiCore.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      585 2023-06-29 02:29:01.000000 DigiCore-1.0.6/DigiCore.egg-info/requires.txt
--rw-rw-rw-   0        0        0       28 2023-06-29 02:29:01.000000 DigiCore-1.0.6/DigiCore.egg-info/top_level.txt
--rw-rw-rw-   0        0        0        2 2023-06-29 02:29:01.000000 DigiCore-1.0.6/DigiCore.egg-info/zip-safe
--rw-rw-rw-   0        0        0     1104 2023-05-20 03:41:32.000000 DigiCore-1.0.6/LICENSE
--rw-rw-rw-   0        0        0     4014 2023-06-29 02:29:01.172340 DigiCore-1.0.6/PKG-INFO
--rw-rw-rw-   0        0        0     2670 2023-05-20 03:41:32.000000 DigiCore-1.0.6/README.md
-drwxrwxrwx   0        0        0        0 2023-06-29 02:29:01.143446 DigiCore-1.0.6/digiCore/
--rw-rw-rw-   0        0        0     1382 2023-05-20 06:50:26.000000 DigiCore-1.0.6/digiCore/__init__.py
--rw-rw-rw-   0        0        0     4901 2023-06-14 02:12:46.000000 DigiCore-1.0.6/digiCore/dsd_kafka.py
--rw-rw-rw-   0        0        0     3712 2023-06-15 03:25:11.000000 DigiCore-1.0.6/digiCore/dsd_mongodb.py
--rw-rw-rw-   0        0        0     6853 2023-06-14 02:12:46.000000 DigiCore-1.0.6/digiCore/dsd_mysql.py
--rw-rw-rw-   0        0        0     3919 2023-05-20 07:33:42.000000 DigiCore-1.0.6/digiCore/dsd_redis.py
--rw-rw-rw-   0        0        0     4161 2023-06-14 08:34:47.000000 DigiCore-1.0.6/digiCore/lingxing_api_scheduler.py
--rw-rw-rw-   0        0        0     1015 2023-05-23 01:25:52.000000 DigiCore-1.0.6/digiCore/model.py
--rw-rw-rw-   0        0        0     3739 2023-06-29 02:25:55.000000 DigiCore-1.0.6/digiCore/send_to_group.py
--rw-rw-rw-   0        0        0      786 2023-05-20 03:41:55.000000 DigiCore-1.0.6/digiCore/status_code.py
--rw-rw-rw-   0        0        0     5191 2023-06-15 03:25:11.000000 DigiCore-1.0.6/digiCore/utils.py
-drwxrwxrwx   0        0        0        0 2023-06-29 02:29:01.147803 DigiCore-1.0.6/k3cloud_webapi_sdk/
--rw-rw-rw-   0        0        0       29 2023-06-15 03:25:11.000000 DigiCore-1.0.6/k3cloud_webapi_sdk/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-29 02:29:01.150847 DigiCore-1.0.6/k3cloud_webapi_sdk/const/
--rw-rw-rw-   0        0        0       16 2023-06-15 03:25:11.000000 DigiCore-1.0.6/k3cloud_webapi_sdk/const/__init__.py
--rw-rw-rw-   0        0        0      418 2023-06-15 03:25:11.000000 DigiCore-1.0.6/k3cloud_webapi_sdk/const/const_define.py
--rw-rw-rw-   0        0        0      500 2023-06-15 03:25:11.000000 DigiCore-1.0.6/k3cloud_webapi_sdk/const/header_param.py
-drwxrwxrwx   0        0        0        0 2023-06-29 02:29:01.154707 DigiCore-1.0.6/k3cloud_webapi_sdk/core/
--rw-rw-rw-   0        0        0       15 2023-06-15 03:25:11.000000 DigiCore-1.0.6/k3cloud_webapi_sdk/core/__init__.py
--rw-rw-rw-   0        0        0     8162 2023-06-15 03:25:11.000000 DigiCore-1.0.6/k3cloud_webapi_sdk/core/webapi_client.py
--rw-rw-rw-   0        0        0     7910 2023-06-15 03:25:11.000000 DigiCore-1.0.6/k3cloud_webapi_sdk/main.py
-drwxrwxrwx   0        0        0        0 2023-06-29 02:29:01.163020 DigiCore-1.0.6/k3cloud_webapi_sdk/model/
--rw-rw-rw-   0        0        0       16 2023-06-15 03:25:11.000000 DigiCore-1.0.6/k3cloud_webapi_sdk/model/__init__.py
--rw-rw-rw-   0        0        0      433 2023-06-15 03:25:11.000000 DigiCore-1.0.6/k3cloud_webapi_sdk/model/api_config.py
--rw-rw-rw-   0        0        0     1109 2023-06-15 03:25:11.000000 DigiCore-1.0.6/k3cloud_webapi_sdk/model/cookie.py
--rw-rw-rw-   0        0        0      327 2023-06-15 03:25:11.000000 DigiCore-1.0.6/k3cloud_webapi_sdk/model/cookie_store.py
--rw-rw-rw-   0        0        0      411 2023-06-15 03:25:11.000000 DigiCore-1.0.6/k3cloud_webapi_sdk/model/identity.py
--rw-rw-rw-   0        0        0      197 2023-06-15 03:25:11.000000 DigiCore-1.0.6/k3cloud_webapi_sdk/model/query_param.py
--rw-rw-rw-   0        0        0     4385 2023-06-15 03:25:11.000000 DigiCore-1.0.6/k3cloud_webapi_sdk/sample.py
-drwxrwxrwx   0        0        0        0 2023-06-29 02:29:01.170836 DigiCore-1.0.6/k3cloud_webapi_sdk/util/
--rw-rw-rw-   0        0        0       15 2023-06-15 03:25:11.000000 DigiCore-1.0.6/k3cloud_webapi_sdk/util/__init__.py
--rw-rw-rw-   0        0        0     2001 2023-06-15 03:25:11.000000 DigiCore-1.0.6/k3cloud_webapi_sdk/util/base64_util.py
--rw-rw-rw-   0        0        0     2671 2023-06-15 03:25:11.000000 DigiCore-1.0.6/k3cloud_webapi_sdk/util/config_util.py
--rw-rw-rw-   0        0        0     1654 2023-06-15 03:25:11.000000 DigiCore-1.0.6/k3cloud_webapi_sdk/util/encode_util.py
--rw-rw-rw-   0        0        0      420 2023-06-15 03:25:11.000000 DigiCore-1.0.6/k3cloud_webapi_sdk/util/hmac_util.py
--rw-rw-rw-   0        0        0       42 2023-06-29 02:29:01.172340 DigiCore-1.0.6/setup.cfg
--rw-rw-rw-   0        0        0     3015 2023-06-29 02:28:52.000000 DigiCore-1.0.6/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-05 06:41:51.756384 DigiCore-1.0.7/
+drwxrwxrwx   0        0        0        0 2023-07-05 06:41:51.615870 DigiCore-1.0.7/DigiCore.egg-info/
+-rw-rw-rw-   0        0        0     4014 2023-07-05 06:41:51.000000 DigiCore-1.0.7/DigiCore.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1142 2023-07-05 06:41:51.000000 DigiCore-1.0.7/DigiCore.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-05 06:41:51.000000 DigiCore-1.0.7/DigiCore.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      585 2023-07-05 06:41:51.000000 DigiCore-1.0.7/DigiCore.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       28 2023-07-05 06:41:51.000000 DigiCore-1.0.7/DigiCore.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0        2 2023-07-05 06:41:51.000000 DigiCore-1.0.7/DigiCore.egg-info/zip-safe
+-rw-rw-rw-   0        0        0     1104 2023-05-20 03:41:32.000000 DigiCore-1.0.7/LICENSE
+-rw-rw-rw-   0        0        0     4014 2023-07-05 06:41:51.756384 DigiCore-1.0.7/PKG-INFO
+-rw-rw-rw-   0        0        0     2670 2023-05-20 03:41:32.000000 DigiCore-1.0.7/README.md
+drwxrwxrwx   0        0        0        0 2023-07-05 06:41:51.646140 DigiCore-1.0.7/digiCore/
+-rw-rw-rw-   0        0        0     1382 2023-07-05 06:14:20.000000 DigiCore-1.0.7/digiCore/__init__.py
+-rw-rw-rw-   0        0        0     3056 2023-07-05 06:35:37.000000 DigiCore-1.0.7/digiCore/db_init.py
+-rw-rw-rw-   0        0        0     4901 2023-06-14 02:12:46.000000 DigiCore-1.0.7/digiCore/dsd_kafka.py
+-rw-rw-rw-   0        0        0     3450 2023-07-05 06:40:33.000000 DigiCore-1.0.7/digiCore/dsd_mongodb.py
+-rw-rw-rw-   0        0        0     6853 2023-06-14 02:12:46.000000 DigiCore-1.0.7/digiCore/dsd_mysql.py
+-rw-rw-rw-   0        0        0     4457 2023-07-05 06:40:33.000000 DigiCore-1.0.7/digiCore/dsd_redis.py
+-rw-rw-rw-   0        0        0     4632 2023-07-04 08:04:47.000000 DigiCore-1.0.7/digiCore/lingxing_api_scheduler.py
+-rw-rw-rw-   0        0        0     3558 2023-07-05 06:40:33.000000 DigiCore-1.0.7/digiCore/model.py
+-rw-rw-rw-   0        0        0     3739 2023-06-29 02:25:55.000000 DigiCore-1.0.7/digiCore/send_to_group.py
+-rw-rw-rw-   0        0        0     5984 2023-07-04 09:09:42.000000 DigiCore-1.0.7/digiCore/utils.py
+drwxrwxrwx   0        0        0        0 2023-07-05 06:41:51.661785 DigiCore-1.0.7/k3cloud_webapi_sdk/
+-rw-rw-rw-   0        0        0       29 2023-06-15 03:25:11.000000 DigiCore-1.0.7/k3cloud_webapi_sdk/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-05 06:41:51.679110 DigiCore-1.0.7/k3cloud_webapi_sdk/const/
+-rw-rw-rw-   0        0        0       16 2023-06-15 03:25:11.000000 DigiCore-1.0.7/k3cloud_webapi_sdk/const/__init__.py
+-rw-rw-rw-   0        0        0      418 2023-06-15 03:25:11.000000 DigiCore-1.0.7/k3cloud_webapi_sdk/const/const_define.py
+-rw-rw-rw-   0        0        0      500 2023-06-15 03:25:11.000000 DigiCore-1.0.7/k3cloud_webapi_sdk/const/header_param.py
+drwxrwxrwx   0        0        0        0 2023-07-05 06:41:51.693136 DigiCore-1.0.7/k3cloud_webapi_sdk/core/
+-rw-rw-rw-   0        0        0       15 2023-06-15 03:25:11.000000 DigiCore-1.0.7/k3cloud_webapi_sdk/core/__init__.py
+-rw-rw-rw-   0        0        0     8162 2023-06-15 03:25:11.000000 DigiCore-1.0.7/k3cloud_webapi_sdk/core/webapi_client.py
+-rw-rw-rw-   0        0        0     7910 2023-06-15 03:25:11.000000 DigiCore-1.0.7/k3cloud_webapi_sdk/main.py
+drwxrwxrwx   0        0        0        0 2023-07-05 06:41:51.726665 DigiCore-1.0.7/k3cloud_webapi_sdk/model/
+-rw-rw-rw-   0        0        0       16 2023-06-15 03:25:11.000000 DigiCore-1.0.7/k3cloud_webapi_sdk/model/__init__.py
+-rw-rw-rw-   0        0        0      433 2023-06-15 03:25:11.000000 DigiCore-1.0.7/k3cloud_webapi_sdk/model/api_config.py
+-rw-rw-rw-   0        0        0     1109 2023-06-15 03:25:11.000000 DigiCore-1.0.7/k3cloud_webapi_sdk/model/cookie.py
+-rw-rw-rw-   0        0        0      327 2023-06-15 03:25:11.000000 DigiCore-1.0.7/k3cloud_webapi_sdk/model/cookie_store.py
+-rw-rw-rw-   0        0        0      411 2023-06-15 03:25:11.000000 DigiCore-1.0.7/k3cloud_webapi_sdk/model/identity.py
+-rw-rw-rw-   0        0        0      197 2023-06-15 03:25:11.000000 DigiCore-1.0.7/k3cloud_webapi_sdk/model/query_param.py
+-rw-rw-rw-   0        0        0     4385 2023-06-15 03:25:11.000000 DigiCore-1.0.7/k3cloud_webapi_sdk/sample.py
+drwxrwxrwx   0        0        0        0 2023-07-05 06:41:51.756384 DigiCore-1.0.7/k3cloud_webapi_sdk/util/
+-rw-rw-rw-   0        0        0       15 2023-06-15 03:25:11.000000 DigiCore-1.0.7/k3cloud_webapi_sdk/util/__init__.py
+-rw-rw-rw-   0        0        0     2001 2023-06-15 03:25:11.000000 DigiCore-1.0.7/k3cloud_webapi_sdk/util/base64_util.py
+-rw-rw-rw-   0        0        0     2671 2023-06-15 03:25:11.000000 DigiCore-1.0.7/k3cloud_webapi_sdk/util/config_util.py
+-rw-rw-rw-   0        0        0     1654 2023-06-15 03:25:11.000000 DigiCore-1.0.7/k3cloud_webapi_sdk/util/encode_util.py
+-rw-rw-rw-   0        0        0      420 2023-06-15 03:25:11.000000 DigiCore-1.0.7/k3cloud_webapi_sdk/util/hmac_util.py
+-rw-rw-rw-   0        0        0       42 2023-07-05 06:41:51.756384 DigiCore-1.0.7/setup.cfg
+-rw-rw-rw-   0        0        0     3015 2023-07-05 06:41:44.000000 DigiCore-1.0.7/setup.py
```

### Comparing `DigiCore-1.0.6/DigiCore.egg-info/PKG-INFO` & `DigiCore-1.0.7/DigiCore.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: DigiCore
-Version: 1.0.6
+Version: 1.0.7
 Summary: DigiCore是一个基于Python的数字化支持部第三方库，旨在为数据处理和开发提供完备的工具集和服务。
 Home-page: UNKNOWN
 Author: yarm
 Author-email: yangyang@doocn.com
 License: MIT License
 Keywords: digicore是服务于道诚集团数字化支持部的自建第三方库项目
 Platform: any
```

### Comparing `DigiCore-1.0.6/DigiCore.egg-info/SOURCES.txt` & `DigiCore-1.0.7/DigiCore.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -4,22 +4,22 @@
 DigiCore.egg-info/PKG-INFO
 DigiCore.egg-info/SOURCES.txt
 DigiCore.egg-info/dependency_links.txt
 DigiCore.egg-info/requires.txt
 DigiCore.egg-info/top_level.txt
 DigiCore.egg-info/zip-safe
 digiCore/__init__.py
+digiCore/db_init.py
 digiCore/dsd_kafka.py
 digiCore/dsd_mongodb.py
 digiCore/dsd_mysql.py
 digiCore/dsd_redis.py
 digiCore/lingxing_api_scheduler.py
 digiCore/model.py
 digiCore/send_to_group.py
-digiCore/status_code.py
 digiCore/utils.py
 k3cloud_webapi_sdk/__init__.py
 k3cloud_webapi_sdk/main.py
 k3cloud_webapi_sdk/sample.py
 k3cloud_webapi_sdk/const/__init__.py
 k3cloud_webapi_sdk/const/const_define.py
 k3cloud_webapi_sdk/const/header_param.py
```

### Comparing `DigiCore-1.0.6/DigiCore.egg-info/requires.txt` & `DigiCore-1.0.7/DigiCore.egg-info/requires.txt`

 * *Files identical despite different names*

### Comparing `DigiCore-1.0.6/LICENSE` & `DigiCore-1.0.7/LICENSE`

 * *Files identical despite different names*

### Comparing `DigiCore-1.0.6/PKG-INFO` & `DigiCore-1.0.7/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: DigiCore
-Version: 1.0.6
+Version: 1.0.7
 Summary: DigiCore是一个基于Python的数字化支持部第三方库，旨在为数据处理和开发提供完备的工具集和服务。
 Home-page: UNKNOWN
 Author: yarm
 Author-email: yangyang@doocn.com
 License: MIT License
 Keywords: digicore是服务于道诚集团数字化支持部的自建第三方库项目
 Platform: any
```

### Comparing `DigiCore-1.0.6/README.md` & `DigiCore-1.0.7/README.md`

 * *Files identical despite different names*

### Comparing `DigiCore-1.0.6/digiCore/__init__.py` & `DigiCore-1.0.7/digiCore/__init__.py`

 * *Files identical despite different names*

### Comparing `DigiCore-1.0.6/digiCore/dsd_kafka.py` & `DigiCore-1.0.7/digiCore/dsd_kafka.py`

 * *Files identical despite different names*

### Comparing `DigiCore-1.0.6/digiCore/dsd_mongodb.py` & `DigiCore-1.0.7/digiCore/dsd_mongodb.py`

 * *Files 6% similar despite different names*

```diff
@@ -59,57 +59,49 @@
 
 
 class MongoDao():
     """
     mongodb事务方法集合
     """
 
-    def __init__(self,
-                 mongodb_url: str,
-                 db_name: str,
-                 table_name: str):
+    def __init__(self, mongodb_url: str):
         self.client = pymongo.MongoClient(mongodb_url)
-        self.db_name = db_name
-        self.table_name = table_name
 
-    def load_table_ob(self):
+    def load_table_ob(self, db_name, table_name):
         """
         根据mongodb的数据库名称和表名称，创建表对象
         :param db_name: 数据库名称
         :param table_name: 表名称
         :return: object
         """
-        db_ob = self.client.get_database(self.db_name)
-        table_ob = db_ob.get_collection(self.table_name)
+        db_ob = self.client.get_database(db_name)
+        table_ob = db_ob.get_collection(table_name)
         return table_ob
 
     @Decorate.def_retry(msg="MongoDB: 创建联合索引主键失败！")
-    def create_index(self, field_list: list):
+    def create_index(self, field_list: list, table_ob):
         """
         自定义 表的联合索引主键
         :param field_list: 联合索引主键列表
         :return: bool
         """
         if not field_list:
             logger.info("无自定义主键！")
             return
-        table_ob = self.load_table_ob()
         index_data = [(one, 1) for one in field_list]
         name = '_1_'.join(field_list)
         table_ob.create_index(index_data, unique=True, name=name)
-        logger.info(f"创建联合索引主键成功！{name}")
 
     @Decorate.def_retry(msg="MongoDB: 数据批量插入失败！")
-    def bulk_save_data(self, data_list: list, field_list: list):
+    def bulk_save_data(self, data_list: list, field_list: list, table_ob):
         """
         批量保存数据到数据库
         如果数据存在则根据 自定义主键进行数据更新
         :param data_list: 数据列表
         :param field_list: 主键列表
-        :return: 
+        :return:
         """
-        table_ob = self.load_table_ob()
-        self.create_index(field_list)
+        self.create_index(field_list, table_ob)
         bulk_write_list = get_bulk_write_list(data_list, field_list)
         if not bulk_write_list:
             return
         table_ob.bulk_write(bulk_write_list, ordered=False)
```

### Comparing `DigiCore-1.0.6/digiCore/dsd_mysql.py` & `DigiCore-1.0.7/digiCore/dsd_mysql.py`

 * *Files identical despite different names*

### Comparing `DigiCore-1.0.6/digiCore/dsd_redis.py` & `DigiCore-1.0.7/digiCore/dsd_redis.py`

 * *Files 7% similar despite different names*

```diff
@@ -4,15 +4,14 @@
 实现增删改查功能
 
 """
 import json
 import time
 
 from redis import Redis, ConnectionPool
-from loguru import logger
 
 from digiCore import Decorate
 
 
 class RedisConnectionPool():
 
     def __init__(self,
@@ -69,26 +68,27 @@
         """
         删除分布式锁
         删除完成 或者 运行标识 不存在 返回 0
         :param run_sign: 运行标识
         :return: 0
         """
         with self.conn as redis_conn:
-            logger.info('运行标志删除成功！')
             return redis_conn.delete(run_sign)
 
     @Decorate.def_retry(msg="redis: 添加任务失败，正在重试连接！")
     def push_task(self, task_name: str, task_json: dict):
         """
         将任务添加到redis进行缓存
         :param task_name: 任务队列名称
         :param task_json: 任务实例
         :return: True
         """
         with self.conn as redis_conn:
+            if not task_json:
+                return None
             bson_data = json.dumps(task_json)
             return redis_conn.lpush(task_name, bson_data)
 
     @Decorate.def_retry(msg="redis: 弹出任务失败，正在重试连接！")
     def pop_task(self, task_name: str):
         """
         从任务队列中弹出一个任务实例
@@ -96,14 +96,16 @@
         队列存在数据的时候 返回 json格式数据
         队列不存在数据的时候，返回 None
         :param task_name: 任务队列名称
         :return: json/None
         """
         with self.conn as redis_conn:
             bson_data = redis_conn.rpop(task_name)
+            if not bson_data:
+                return None
             data_json = json.loads(bson_data)
             return data_json
 
     @Decorate.def_retry(msg="redis: hash添加数据失败，正在重试连接！")
     def hash_task(self, hash_name, hash_data):
         """
         将hash加密的数据缓存到redis。
@@ -111,7 +113,21 @@
         :param hash_name: hash队列的名称
         :param hash_data: hash加密之后的数据
         :return:
         """
         with self.conn as redis_conn:
             strTime = time.strftime("%Y-%m-%d %H:%M:%S", time.localtime())
             redis_conn.hset(hash_name, hash_data, strTime)
+
+    @Decorate.def_retry(msg="redis: outh_token获取失败，正在重试连接！")
+    def get_lingxing_auth_token(self, AUTH_TOKEN=None):
+        """
+        获取领星的token
+        """
+        if not AUTH_TOKEN:
+            AUTH_TOKEN = "common-lingxing-access-token:common:auth_token"
+        with self.conn as redis_conn:
+            token = redis_conn.get(AUTH_TOKEN)
+            if token:
+                return token.decode()
+            else:
+                return None
```

### Comparing `DigiCore-1.0.6/digiCore/lingxing_api_scheduler.py` & `DigiCore-1.0.7/digiCore/lingxing_api_scheduler.py`

 * *Files 12% similar despite different names*

```diff
@@ -4,17 +4,19 @@
 # @Email ： yangyang@doocn.com
 # @File : common-lingxing-sign-api
 # @Desc :
 import copy
 import time
 import urllib
 from typing import Union
+
+import requests
 from orjson import orjson
 from digiCore.utils import EncryptTool
-
+from .model import ErrorEnum,UrlEnum
 
 class SignBase(object):
 
     @classmethod
     def generate_sign(cls, encrypt_key: str, request_params: dict) -> str:
         """
         生成签名
@@ -118,9 +120,19 @@
         full_api = self.get_full_api_url(params)
         data = {
             'params': params,
             'lingxing_api': full_api
         }
         return data
 
-
+    def sync_lingxing_data(self, api, param_data, _code):
+        """
+        请求lingxing_api，获取response
+        :return:
+        """
+        headers = UrlEnum.headers
+        response = requests.post(url=api, headers=headers, json=param_data, timeout=20).json()
+        code = response.get("code")
+        if int(code) != _code:
+            return ErrorEnum.REQUESTS_ERROR
+        return response
```

### Comparing `DigiCore-1.0.6/digiCore/send_to_group.py` & `DigiCore-1.0.7/digiCore/send_to_group.py`

 * *Files identical despite different names*

### Comparing `DigiCore-1.0.6/digiCore/utils.py` & `DigiCore-1.0.7/digiCore/utils.py`

 * *Files 6% similar despite different names*

```diff
@@ -144,7 +144,34 @@
         return enc_text
 
     @classmethod
     def md5_encrypt(cls, text: str):
         md = hashlib.md5()
         md.update(text.encode('utf-8'))
         return md.hexdigest()
+
+
+class MsgTool:
+
+    @classmethod
+    def format_log_msg(cls, e):
+        """
+        格式化错误信息
+        :param e:
+        :return:
+        """
+        logger.error(f'error file:{e.__traceback__.tb_frame.f_globals["__file__"]}')
+        logger.error(f'error line:{e.__traceback__.tb_lineno}')
+        logger.error(f'error message:{e.args}')
+        error_msg = {'error_file': e.__traceback__.tb_frame.f_globals["__file__"],
+                     'error_line': e.__traceback__.tb_lineno,
+                     'error_message': e.args}
+        return error_msg
+
+    @classmethod
+    def format_api_msg(cls, enum):
+        """
+        格式化api返回信息
+        :param enum:
+        :return:
+        """
+        return {"code": enum[0], "msg": enum[1]}
```

### Comparing `DigiCore-1.0.6/k3cloud_webapi_sdk/core/webapi_client.py` & `DigiCore-1.0.7/k3cloud_webapi_sdk/core/webapi_client.py`

 * *Files identical despite different names*

### Comparing `DigiCore-1.0.6/k3cloud_webapi_sdk/main.py` & `DigiCore-1.0.7/k3cloud_webapi_sdk/main.py`

 * *Files identical despite different names*

### Comparing `DigiCore-1.0.6/k3cloud_webapi_sdk/model/cookie.py` & `DigiCore-1.0.7/k3cloud_webapi_sdk/model/cookie.py`

 * *Files identical despite different names*

### Comparing `DigiCore-1.0.6/k3cloud_webapi_sdk/sample.py` & `DigiCore-1.0.7/k3cloud_webapi_sdk/sample.py`

 * *Files identical despite different names*

### Comparing `DigiCore-1.0.6/k3cloud_webapi_sdk/util/base64_util.py` & `DigiCore-1.0.7/k3cloud_webapi_sdk/util/base64_util.py`

 * *Files identical despite different names*

### Comparing `DigiCore-1.0.6/k3cloud_webapi_sdk/util/config_util.py` & `DigiCore-1.0.7/k3cloud_webapi_sdk/util/config_util.py`

 * *Files identical despite different names*

### Comparing `DigiCore-1.0.6/k3cloud_webapi_sdk/util/encode_util.py` & `DigiCore-1.0.7/k3cloud_webapi_sdk/util/encode_util.py`

 * *Files identical despite different names*

### Comparing `DigiCore-1.0.6/setup.py` & `DigiCore-1.0.7/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -64,15 +64,15 @@
 "tzdata==2023.3",
 "urllib3==2.0.2",
 "win32-setctime==1.1.0"
 ]
 
 setup(
     name="DigiCore",
-    version="1.0.6",
+    version="1.0.7",
     description="DigiCore是一个基于Python的数字化支持部第三方库，旨在为数据处理和开发提供完备的工具集和服务。",
     long_description=README,
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "Environment :: Console",
         "Intended Audience :: Developers",
         "Programming Language :: Python",
```

