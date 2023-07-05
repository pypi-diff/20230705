# Comparing `tmp/sanic-api-0.2.6.tar.gz` & `tmp/sanic-api-0.2.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sanic-api-0.2.6.tar", last modified: Wed Jul  5 08:13:47 2023, max compression
+gzip compressed data, was "sanic-api-0.2.7.tar", last modified: Wed Jul  5 08:43:02 2023, max compression
```

## Comparing `sanic-api-0.2.6.tar` & `sanic-api-0.2.7.tar`

### file list

```diff
@@ -1,39 +1,39 @@
--rw-r--r--   0        0        0        0 2023-07-01 02:01:18.676902 sanic-api-0.2.6/example/__init__.py
--rw-r--r--   0        0        0      605 2023-07-01 02:01:18.676902 sanic-api-0.2.6/example/__main__.py
--rw-r--r--   0        0        0       34 2023-07-01 02:01:18.676902 sanic-api-0.2.6/example/api/__init__.py
--rw-r--r--   0        0        0       66 2023-07-05 08:02:15.217469 sanic-api-0.2.6/example/api/t1/__init__.py
--rw-r--r--   0        0        0      634 2023-07-05 08:02:15.217469 sanic-api-0.2.6/example/api/t1/t1_1.py
--rw-r--r--   0        0        0      233 2023-07-05 08:02:15.217469 sanic-api-0.2.6/example/api/t1/t1_2.py
--rw-r--r--   0        0        0       29 2023-07-01 02:01:18.677902 sanic-api-0.2.6/example/api/t2/__init__.py
--rw-r--r--   0        0        0      248 2023-07-01 02:01:18.677902 sanic-api-0.2.6/example/api/t2/t2.py
--rw-r--r--   0        0        0       29 2023-07-01 02:01:18.677902 sanic-api-0.2.6/example/api/t2/t3/__init__.py
--rw-r--r--   0        0        0      248 2023-07-01 02:01:18.677902 sanic-api-0.2.6/example/api/t2/t3/t3.py
--rw-r--r--   0        0        0     1844 2023-07-01 02:01:18.677902 sanic-api-0.2.6/example/api/user.py
--rw-r--r--   0        0        0     1722 2023-07-01 02:01:18.677902 sanic-api-0.2.6/example/api/validator.py
--rw-r--r--   0        0        0     1202 2023-07-05 08:02:15.218469 sanic-api-0.2.6/example/app.py
--rw-r--r--   0        0        0      134 2023-07-01 02:01:18.677902 sanic-api-0.2.6/example/settings.py
--rw-r--r--   0        0        0     1090 2023-07-01 02:01:18.676902 sanic-api-0.2.6/LICENSE.txt
--rw-r--r--   0        0        0     1684 2023-07-05 08:02:41.957110 sanic-api-0.2.6/pyproject.toml
--rw-r--r--   0        0        0     1745 2023-07-01 02:01:18.676902 sanic-api-0.2.6/README.MD
--rw-r--r--   0        0        0      348 2023-07-01 02:01:18.679691 sanic-api-0.2.6/sanic_api/__init__.py
--rw-r--r--   0        0        0       51 2023-07-01 02:01:18.679691 sanic-api-0.2.6/sanic_api/api/__init__.py
--rw-r--r--   0        0        0     5486 2023-07-01 02:01:18.679691 sanic-api-0.2.6/sanic_api/api/api.py
--rw-r--r--   0        0        0     1216 2023-07-01 02:01:18.679691 sanic-api-0.2.6/sanic_api/api/exception.py
--rw-r--r--   0        0        0      706 2023-07-01 02:01:18.679691 sanic-api-0.2.6/sanic_api/api/extend.py
--rw-r--r--   0        0        0     1206 2023-07-01 02:01:18.679691 sanic-api-0.2.6/sanic_api/api/handle_exception.py
--rw-r--r--   0        0        0     1032 2023-07-01 02:01:18.679691 sanic-api-0.2.6/sanic_api/api/model.py
--rw-r--r--   0        0        0     2078 2023-07-01 02:01:18.680695 sanic-api-0.2.6/sanic_api/api/validators.py
--rw-r--r--   0        0        0       68 2023-07-01 02:01:18.680695 sanic-api-0.2.6/sanic_api/config/__init__.py
--rw-r--r--   0        0        0     3229 2023-07-01 02:01:18.680695 sanic-api-0.2.6/sanic_api/config/base.py
--rw-r--r--   0        0        0      636 2023-07-05 08:02:15.218469 sanic-api-0.2.6/sanic_api/config/sanic.py
--rw-r--r--   0        0        0      373 2023-07-05 08:02:15.219469 sanic-api-0.2.6/sanic_api/config/sanic_api.py
--rw-r--r--   0        0        0      735 2023-07-01 02:01:18.680695 sanic-api-0.2.6/sanic_api/config/setting.py
--rw-r--r--   0        0        0     2040 2023-07-01 02:01:18.680695 sanic-api-0.2.6/sanic_api/enum.py
--rw-r--r--   0        0        0       33 2023-07-01 02:01:18.680695 sanic-api-0.2.6/sanic_api/logger/__init__.py
--rw-r--r--   0        0        0     2511 2023-07-01 02:01:18.680695 sanic-api-0.2.6/sanic_api/logger/config.py
--rw-r--r--   0        0        0     1911 2023-07-01 02:01:18.680695 sanic-api-0.2.6/sanic_api/logger/extend.py
--rw-r--r--   0        0        0     2102 2023-07-01 02:01:18.681695 sanic-api-0.2.6/sanic_api/logger/sanic_http.py
--rw-r--r--   0        0        0      146 2023-07-01 02:01:18.681695 sanic-api-0.2.6/sanic_api/openapi/__init__.py
--rw-r--r--   0        0        0     4147 2023-07-01 02:01:18.681695 sanic-api-0.2.6/sanic_api/openapi/openapi.py
--rw-r--r--   0        0        0     3574 2023-07-05 08:02:15.219469 sanic-api-0.2.6/sanic_api/utils.py
--rw-r--r--   0        0        0     2088 1970-01-01 00:00:00.000000 sanic-api-0.2.6/PKG-INFO
+-rw-r--r--   0        0        0        0 2023-07-01 02:01:18.676902 sanic-api-0.2.7/example/__init__.py
+-rw-r--r--   0        0        0      605 2023-07-01 02:01:18.676902 sanic-api-0.2.7/example/__main__.py
+-rw-r--r--   0        0        0       34 2023-07-01 02:01:18.676902 sanic-api-0.2.7/example/api/__init__.py
+-rw-r--r--   0        0        0       66 2023-07-05 08:02:15.217469 sanic-api-0.2.7/example/api/t1/__init__.py
+-rw-r--r--   0        0        0      634 2023-07-05 08:02:15.217469 sanic-api-0.2.7/example/api/t1/t1_1.py
+-rw-r--r--   0        0        0      233 2023-07-05 08:02:15.217469 sanic-api-0.2.7/example/api/t1/t1_2.py
+-rw-r--r--   0        0        0       29 2023-07-01 02:01:18.677902 sanic-api-0.2.7/example/api/t2/__init__.py
+-rw-r--r--   0        0        0      248 2023-07-01 02:01:18.677902 sanic-api-0.2.7/example/api/t2/t2.py
+-rw-r--r--   0        0        0       29 2023-07-01 02:01:18.677902 sanic-api-0.2.7/example/api/t2/t3/__init__.py
+-rw-r--r--   0        0        0      248 2023-07-01 02:01:18.677902 sanic-api-0.2.7/example/api/t2/t3/t3.py
+-rw-r--r--   0        0        0     1844 2023-07-01 02:01:18.677902 sanic-api-0.2.7/example/api/user.py
+-rw-r--r--   0        0        0     1722 2023-07-01 02:01:18.677902 sanic-api-0.2.7/example/api/validator.py
+-rw-r--r--   0        0        0     1202 2023-07-05 08:02:15.218469 sanic-api-0.2.7/example/app.py
+-rw-r--r--   0        0        0      134 2023-07-01 02:01:18.677902 sanic-api-0.2.7/example/settings.py
+-rw-r--r--   0        0        0     1090 2023-07-01 02:01:18.676902 sanic-api-0.2.7/LICENSE.txt
+-rw-r--r--   0        0        0     1684 2023-07-05 08:41:38.580108 sanic-api-0.2.7/pyproject.toml
+-rw-r--r--   0        0        0     1745 2023-07-01 02:01:18.676902 sanic-api-0.2.7/README.MD
+-rw-r--r--   0        0        0      348 2023-07-01 02:01:18.679691 sanic-api-0.2.7/sanic_api/__init__.py
+-rw-r--r--   0        0        0       51 2023-07-01 02:01:18.679691 sanic-api-0.2.7/sanic_api/api/__init__.py
+-rw-r--r--   0        0        0     5486 2023-07-01 02:01:18.679691 sanic-api-0.2.7/sanic_api/api/api.py
+-rw-r--r--   0        0        0     1216 2023-07-01 02:01:18.679691 sanic-api-0.2.7/sanic_api/api/exception.py
+-rw-r--r--   0        0        0      706 2023-07-01 02:01:18.679691 sanic-api-0.2.7/sanic_api/api/extend.py
+-rw-r--r--   0        0        0     1206 2023-07-01 02:01:18.679691 sanic-api-0.2.7/sanic_api/api/handle_exception.py
+-rw-r--r--   0        0        0     1032 2023-07-01 02:01:18.679691 sanic-api-0.2.7/sanic_api/api/model.py
+-rw-r--r--   0        0        0     2078 2023-07-01 02:01:18.680695 sanic-api-0.2.7/sanic_api/api/validators.py
+-rw-r--r--   0        0        0       68 2023-07-01 02:01:18.680695 sanic-api-0.2.7/sanic_api/config/__init__.py
+-rw-r--r--   0        0        0     3228 2023-07-05 08:41:28.032788 sanic-api-0.2.7/sanic_api/config/base.py
+-rw-r--r--   0        0        0      636 2023-07-05 08:02:15.218469 sanic-api-0.2.7/sanic_api/config/sanic.py
+-rw-r--r--   0        0        0      373 2023-07-05 08:02:15.219469 sanic-api-0.2.7/sanic_api/config/sanic_api.py
+-rw-r--r--   0        0        0      735 2023-07-01 02:01:18.680695 sanic-api-0.2.7/sanic_api/config/setting.py
+-rw-r--r--   0        0        0     2040 2023-07-01 02:01:18.680695 sanic-api-0.2.7/sanic_api/enum.py
+-rw-r--r--   0        0        0       33 2023-07-01 02:01:18.680695 sanic-api-0.2.7/sanic_api/logger/__init__.py
+-rw-r--r--   0        0        0     2511 2023-07-01 02:01:18.680695 sanic-api-0.2.7/sanic_api/logger/config.py
+-rw-r--r--   0        0        0     1911 2023-07-01 02:01:18.680695 sanic-api-0.2.7/sanic_api/logger/extend.py
+-rw-r--r--   0        0        0     2102 2023-07-01 02:01:18.681695 sanic-api-0.2.7/sanic_api/logger/sanic_http.py
+-rw-r--r--   0        0        0      146 2023-07-01 02:01:18.681695 sanic-api-0.2.7/sanic_api/openapi/__init__.py
+-rw-r--r--   0        0        0     4147 2023-07-01 02:01:18.681695 sanic-api-0.2.7/sanic_api/openapi/openapi.py
+-rw-r--r--   0        0        0     3574 2023-07-05 08:02:15.219469 sanic-api-0.2.7/sanic_api/utils.py
+-rw-r--r--   0        0        0     2088 1970-01-01 00:00:00.000000 sanic-api-0.2.7/PKG-INFO
```

### Comparing `sanic-api-0.2.6/example/__main__.py` & `sanic-api-0.2.7/example/__main__.py`

 * *Files identical despite different names*

### Comparing `sanic-api-0.2.6/example/api/t1/t1_1.py` & `sanic-api-0.2.7/example/api/t1/t1_1.py`

 * *Files identical despite different names*

### Comparing `sanic-api-0.2.6/example/api/user.py` & `sanic-api-0.2.7/example/api/user.py`

 * *Files identical despite different names*

### Comparing `sanic-api-0.2.6/example/api/validator.py` & `sanic-api-0.2.7/example/api/validator.py`

 * *Files identical despite different names*

### Comparing `sanic-api-0.2.6/example/app.py` & `sanic-api-0.2.7/example/app.py`

 * *Files identical despite different names*

### Comparing `sanic-api-0.2.6/LICENSE.txt` & `sanic-api-0.2.7/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `sanic-api-0.2.6/pyproject.toml` & `sanic-api-0.2.7/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "sanic-api"
-version = "0.2.6"
+version = "0.2.7"
 description = "Sanic 框架实用API工具集，拥有自动生成文档、参数校验、配置的导入、日志功能的优化等功能，更好的助力接口的开发"
 authors = [
     { name = "昊色居士", email = "xhrtxh@gmail.com" },
 ]
 dependencies = [
     "sanic>=22.3",
     "pydantic[dotenv]>=1.10.2",
```

### Comparing `sanic-api-0.2.6/README.MD` & `sanic-api-0.2.7/README.MD`

 * *Files identical despite different names*

### Comparing `sanic-api-0.2.6/sanic_api/api/api.py` & `sanic-api-0.2.7/sanic_api/api/api.py`

 * *Files identical despite different names*

### Comparing `sanic-api-0.2.6/sanic_api/api/exception.py` & `sanic-api-0.2.7/sanic_api/api/exception.py`

 * *Files identical despite different names*

### Comparing `sanic-api-0.2.6/sanic_api/api/extend.py` & `sanic-api-0.2.7/sanic_api/api/extend.py`

 * *Files identical despite different names*

### Comparing `sanic-api-0.2.6/sanic_api/api/handle_exception.py` & `sanic-api-0.2.7/sanic_api/api/handle_exception.py`

 * *Files identical despite different names*

### Comparing `sanic-api-0.2.6/sanic_api/api/model.py` & `sanic-api-0.2.7/sanic_api/api/model.py`

 * *Files identical despite different names*

### Comparing `sanic-api-0.2.6/sanic_api/api/validators.py` & `sanic-api-0.2.7/sanic_api/api/validators.py`

 * *Files identical despite different names*

### Comparing `sanic-api-0.2.6/sanic_api/config/base.py` & `sanic-api-0.2.7/sanic_api/config/base.py`

 * *Files 0% similar despite different names*

```diff
@@ -56,15 +56,15 @@
 
 class SettingsBase(BaseSettings):
     """
     项目设置的基类
     """
 
     class Config:
-        root_config_dir = getpath_by_root("../configs")
+        root_config_dir = getpath_by_root("./configs")
         env_file = root_config_dir / ".env"
         env_file_encoding = "utf-8"
         env_nested_delimiter = "__"
 
         @classmethod
         def customise_sources(
             cls,
```

### Comparing `sanic-api-0.2.6/sanic_api/config/sanic.py` & `sanic-api-0.2.7/sanic_api/config/sanic.py`

 * *Files identical despite different names*

### Comparing `sanic-api-0.2.6/sanic_api/config/setting.py` & `sanic-api-0.2.7/sanic_api/config/setting.py`

 * *Files identical despite different names*

### Comparing `sanic-api-0.2.6/sanic_api/enum.py` & `sanic-api-0.2.7/sanic_api/enum.py`

 * *Files identical despite different names*

### Comparing `sanic-api-0.2.6/sanic_api/logger/config.py` & `sanic-api-0.2.7/sanic_api/logger/config.py`

 * *Files identical despite different names*

### Comparing `sanic-api-0.2.6/sanic_api/logger/extend.py` & `sanic-api-0.2.7/sanic_api/logger/extend.py`

 * *Files identical despite different names*

### Comparing `sanic-api-0.2.6/sanic_api/logger/sanic_http.py` & `sanic-api-0.2.7/sanic_api/logger/sanic_http.py`

 * *Files identical despite different names*

### Comparing `sanic-api-0.2.6/sanic_api/openapi/openapi.py` & `sanic-api-0.2.7/sanic_api/openapi/openapi.py`

 * *Files identical despite different names*

### Comparing `sanic-api-0.2.6/sanic_api/utils.py` & `sanic-api-0.2.7/sanic_api/utils.py`

 * *Files identical despite different names*

### Comparing `sanic-api-0.2.6/PKG-INFO` & `sanic-api-0.2.7/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sanic-api
-Version: 0.2.6
+Version: 0.2.7
 Summary: Sanic 框架实用API工具集，拥有自动生成文档、参数校验、配置的导入、日志功能的优化等功能，更好的助力接口的开发
 License: MIT
 Author-email: 昊色居士 <xhrtxh@gmail.com>
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 
 ![logo](https://images.haose.pro/2022/12/19/logo_17%3A34%3A07_qkt9yi4d7u.png)
```

