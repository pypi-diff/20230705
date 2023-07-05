# Comparing `tmp/sanic-api-0.2.5.tar.gz` & `tmp/sanic-api-0.2.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sanic-api-0.2.5.tar", last modified: Sat Apr  8 16:27:09 2023, max compression
+gzip compressed data, was "sanic-api-0.2.6.tar", last modified: Wed Jul  5 08:13:47 2023, max compression
```

## Comparing `sanic-api-0.2.5.tar` & `sanic-api-0.2.6.tar`

### file list

```diff
@@ -1,38 +1,39 @@
--rw-r--r--   0        0        0        0 2022-12-19 09:31:30.146039 sanic-api-0.2.5/example/__init__.py
--rw-r--r--   0        0        0      624 2023-04-08 16:25:11.460645 sanic-api-0.2.5/example/__main__.py
--rw-r--r--   0        0        0       35 2023-04-08 16:25:11.461646 sanic-api-0.2.5/example/api/__init__.py
--rw-r--r--   0        0        0       30 2023-04-08 16:25:11.462645 sanic-api-0.2.5/example/api/t1/__init__.py
--rw-r--r--   0        0        0      640 2023-04-08 16:25:11.462645 sanic-api-0.2.5/example/api/t1/t1.py
--rw-r--r--   0        0        0       30 2023-04-08 16:25:11.463645 sanic-api-0.2.5/example/api/t2/__init__.py
--rw-r--r--   0        0        0      257 2023-04-08 16:25:11.463645 sanic-api-0.2.5/example/api/t2/t2.py
--rw-r--r--   0        0        0       30 2023-04-08 16:25:11.464645 sanic-api-0.2.5/example/api/t2/t3/__init__.py
--rw-r--r--   0        0        0      257 2023-04-08 16:25:11.464645 sanic-api-0.2.5/example/api/t2/t3/t3.py
--rw-r--r--   0        0        0     1933 2023-04-08 16:25:11.465646 sanic-api-0.2.5/example/api/user.py
--rw-r--r--   0        0        0     1819 2023-04-08 16:25:11.466645 sanic-api-0.2.5/example/api/validator.py
--rw-r--r--   0        0        0     1272 2023-04-08 16:25:11.467646 sanic-api-0.2.5/example/app.py
--rw-r--r--   0        0        0      144 2023-04-08 16:25:11.467646 sanic-api-0.2.5/example/settings.py
--rw-r--r--   0        0        0     1090 2022-12-19 09:31:30.145040 sanic-api-0.2.5/LICENSE.txt
--rw-r--r--   0        0        0     1651 2023-04-08 16:25:13.997538 sanic-api-0.2.5/pyproject.toml
--rw-r--r--   0        0        0     1824 2023-04-08 16:25:13.996538 sanic-api-0.2.5/README.MD
--rw-r--r--   0        0        0      369 2023-02-05 03:39:25.051397 sanic-api-0.2.5/sanic_api/__init__.py
--rw-r--r--   0        0        0       53 2023-02-05 03:39:25.052397 sanic-api-0.2.5/sanic_api/api/__init__.py
--rw-r--r--   0        0        0     5663 2023-04-08 16:25:11.470648 sanic-api-0.2.5/sanic_api/api/api.py
--rw-r--r--   0        0        0     1262 2023-04-08 16:25:11.471648 sanic-api-0.2.5/sanic_api/api/exception.py
--rw-r--r--   0        0        0      731 2023-02-05 03:57:56.988254 sanic-api-0.2.5/sanic_api/api/extend.py
--rw-r--r--   0        0        0     1267 2023-04-08 16:25:11.472646 sanic-api-0.2.5/sanic_api/api/handle_exception.py
--rw-r--r--   0        0        0     1077 2023-04-08 16:25:11.473648 sanic-api-0.2.5/sanic_api/api/model.py
--rw-r--r--   0        0        0     2154 2023-04-08 16:25:11.474646 sanic-api-0.2.5/sanic_api/api/validators.py
--rw-r--r--   0        0        0       70 2023-04-08 16:25:11.474646 sanic-api-0.2.5/sanic_api/config/__init__.py
--rw-r--r--   0        0        0     3339 2023-04-08 16:25:11.475649 sanic-api-0.2.5/sanic_api/config/base.py
--rw-r--r--   0        0        0      681 2023-04-08 16:25:11.476646 sanic-api-0.2.5/sanic_api/config/sanic.py
--rw-r--r--   0        0        0      410 2023-04-08 16:25:11.477647 sanic-api-0.2.5/sanic_api/config/sanic_api.py
--rw-r--r--   0        0        0      765 2023-04-08 16:25:11.477647 sanic-api-0.2.5/sanic_api/config/setting.py
--rw-r--r--   0        0        0     2128 2023-04-08 16:25:11.478649 sanic-api-0.2.5/sanic_api/enum.py
--rw-r--r--   0        0        0       34 2023-02-05 03:39:25.058399 sanic-api-0.2.5/sanic_api/logger/__init__.py
--rw-r--r--   0        0        0     2588 2023-04-08 16:25:11.479786 sanic-api-0.2.5/sanic_api/logger/config.py
--rw-r--r--   0        0        0     1982 2023-04-08 16:25:11.480646 sanic-api-0.2.5/sanic_api/logger/extend.py
--rw-r--r--   0        0        0     2170 2023-04-08 16:25:11.481646 sanic-api-0.2.5/sanic_api/logger/sanic_http.py
--rw-r--r--   0        0        0      153 2023-04-08 16:25:11.481646 sanic-api-0.2.5/sanic_api/openapi/__init__.py
--rw-r--r--   0        0        0     4249 2023-04-08 16:25:11.482646 sanic-api-0.2.5/sanic_api/openapi/openapi.py
--rw-r--r--   0        0        0     2882 2023-04-08 16:25:11.483646 sanic-api-0.2.5/sanic_api/utils.py
--rw-r--r--   0        0        0     2088 1970-01-01 00:00:00.000000 sanic-api-0.2.5/PKG-INFO
+-rw-r--r--   0        0        0        0 2023-07-01 02:01:18.676902 sanic-api-0.2.6/example/__init__.py
+-rw-r--r--   0        0        0      605 2023-07-01 02:01:18.676902 sanic-api-0.2.6/example/__main__.py
+-rw-r--r--   0        0        0       34 2023-07-01 02:01:18.676902 sanic-api-0.2.6/example/api/__init__.py
+-rw-r--r--   0        0        0       66 2023-07-05 08:02:15.217469 sanic-api-0.2.6/example/api/t1/__init__.py
+-rw-r--r--   0        0        0      634 2023-07-05 08:02:15.217469 sanic-api-0.2.6/example/api/t1/t1_1.py
+-rw-r--r--   0        0        0      233 2023-07-05 08:02:15.217469 sanic-api-0.2.6/example/api/t1/t1_2.py
+-rw-r--r--   0        0        0       29 2023-07-01 02:01:18.677902 sanic-api-0.2.6/example/api/t2/__init__.py
+-rw-r--r--   0        0        0      248 2023-07-01 02:01:18.677902 sanic-api-0.2.6/example/api/t2/t2.py
+-rw-r--r--   0        0        0       29 2023-07-01 02:01:18.677902 sanic-api-0.2.6/example/api/t2/t3/__init__.py
+-rw-r--r--   0        0        0      248 2023-07-01 02:01:18.677902 sanic-api-0.2.6/example/api/t2/t3/t3.py
+-rw-r--r--   0        0        0     1844 2023-07-01 02:01:18.677902 sanic-api-0.2.6/example/api/user.py
+-rw-r--r--   0        0        0     1722 2023-07-01 02:01:18.677902 sanic-api-0.2.6/example/api/validator.py
+-rw-r--r--   0        0        0     1202 2023-07-05 08:02:15.218469 sanic-api-0.2.6/example/app.py
+-rw-r--r--   0        0        0      134 2023-07-01 02:01:18.677902 sanic-api-0.2.6/example/settings.py
+-rw-r--r--   0        0        0     1090 2023-07-01 02:01:18.676902 sanic-api-0.2.6/LICENSE.txt
+-rw-r--r--   0        0        0     1684 2023-07-05 08:02:41.957110 sanic-api-0.2.6/pyproject.toml
+-rw-r--r--   0        0        0     1745 2023-07-01 02:01:18.676902 sanic-api-0.2.6/README.MD
+-rw-r--r--   0        0        0      348 2023-07-01 02:01:18.679691 sanic-api-0.2.6/sanic_api/__init__.py
+-rw-r--r--   0        0        0       51 2023-07-01 02:01:18.679691 sanic-api-0.2.6/sanic_api/api/__init__.py
+-rw-r--r--   0        0        0     5486 2023-07-01 02:01:18.679691 sanic-api-0.2.6/sanic_api/api/api.py
+-rw-r--r--   0        0        0     1216 2023-07-01 02:01:18.679691 sanic-api-0.2.6/sanic_api/api/exception.py
+-rw-r--r--   0        0        0      706 2023-07-01 02:01:18.679691 sanic-api-0.2.6/sanic_api/api/extend.py
+-rw-r--r--   0        0        0     1206 2023-07-01 02:01:18.679691 sanic-api-0.2.6/sanic_api/api/handle_exception.py
+-rw-r--r--   0        0        0     1032 2023-07-01 02:01:18.679691 sanic-api-0.2.6/sanic_api/api/model.py
+-rw-r--r--   0        0        0     2078 2023-07-01 02:01:18.680695 sanic-api-0.2.6/sanic_api/api/validators.py
+-rw-r--r--   0        0        0       68 2023-07-01 02:01:18.680695 sanic-api-0.2.6/sanic_api/config/__init__.py
+-rw-r--r--   0        0        0     3229 2023-07-01 02:01:18.680695 sanic-api-0.2.6/sanic_api/config/base.py
+-rw-r--r--   0        0        0      636 2023-07-05 08:02:15.218469 sanic-api-0.2.6/sanic_api/config/sanic.py
+-rw-r--r--   0        0        0      373 2023-07-05 08:02:15.219469 sanic-api-0.2.6/sanic_api/config/sanic_api.py
+-rw-r--r--   0        0        0      735 2023-07-01 02:01:18.680695 sanic-api-0.2.6/sanic_api/config/setting.py
+-rw-r--r--   0        0        0     2040 2023-07-01 02:01:18.680695 sanic-api-0.2.6/sanic_api/enum.py
+-rw-r--r--   0        0        0       33 2023-07-01 02:01:18.680695 sanic-api-0.2.6/sanic_api/logger/__init__.py
+-rw-r--r--   0        0        0     2511 2023-07-01 02:01:18.680695 sanic-api-0.2.6/sanic_api/logger/config.py
+-rw-r--r--   0        0        0     1911 2023-07-01 02:01:18.680695 sanic-api-0.2.6/sanic_api/logger/extend.py
+-rw-r--r--   0        0        0     2102 2023-07-01 02:01:18.681695 sanic-api-0.2.6/sanic_api/logger/sanic_http.py
+-rw-r--r--   0        0        0      146 2023-07-01 02:01:18.681695 sanic-api-0.2.6/sanic_api/openapi/__init__.py
+-rw-r--r--   0        0        0     4147 2023-07-01 02:01:18.681695 sanic-api-0.2.6/sanic_api/openapi/openapi.py
+-rw-r--r--   0        0        0     3574 2023-07-05 08:02:15.219469 sanic-api-0.2.6/sanic_api/utils.py
+-rw-r--r--   0        0        0     2088 1970-01-01 00:00:00.000000 sanic-api-0.2.6/PKG-INFO
```

### Comparing `sanic-api-0.2.5/example/__main__.py` & `sanic-api-0.2.6/example/__main__.py`

 * *Ordering differences only*

 * *Files 12% similar despite different names*

```diff
@@ -1,19 +1,19 @@
-from sanic import Sanic
-from sanic.worker.loader import AppLoader
-
-from example.app import app_factory
-from example.settings import settings
-from sanic_api.enum import RunModeEnum
-
-if __name__ == "__main__":
-    loader = AppLoader(factory=app_factory)
-    app = loader.load()
-    app.prepare(
-        host=settings.host,
-        port=settings.port,
-        debug=settings.mode == RunModeEnum.DEBUG,
-        dev=settings.mode == RunModeEnum.DEV,
-        workers=settings.workers,
-        fast=settings.mode == RunModeEnum.PRODUCTION and settings.workers == 1,
-    )
-    Sanic.serve(app, app_loader=loader)
+from sanic import Sanic
+from sanic.worker.loader import AppLoader
+
+from example.app import app_factory
+from example.settings import settings
+from sanic_api.enum import RunModeEnum
+
+if __name__ == "__main__":
+    loader = AppLoader(factory=app_factory)
+    app = loader.load()
+    app.prepare(
+        host=settings.host,
+        port=settings.port,
+        debug=settings.mode == RunModeEnum.DEBUG,
+        dev=settings.mode == RunModeEnum.DEV,
+        workers=settings.workers,
+        fast=settings.mode == RunModeEnum.PRODUCTION and settings.workers == 1,
+    )
+    Sanic.serve(app, app_loader=loader)
```

### Comparing `sanic-api-0.2.5/example/api/user.py` & `sanic-api-0.2.6/example/api/user.py`

 * *Ordering differences only*

 * *Files 15% similar despite different names*

```diff
@@ -1,89 +1,89 @@
-from typing import Any, Dict, List
-from uuid import uuid4
-
-from sanic import Blueprint, text
-from sanic.request import Request
-
-from .validator import (
-    UserAddApi,
-    UserDelApi,
-    UserFindOneApi,
-    UserListApi,
-    UserUpdateApi,
-)
-
-users_blueprint = Blueprint("users_blueprint", url_prefix="/users")
-users_blueprint.ctx.desc = "用户"
-
-
-@users_blueprint.route("/test", methods=["GET"])
-async def hello(request):
-    return text("Hello world!")
-
-
-@users_blueprint.route("/", methods=["POST"])
-async def user_add(request: Request, api: UserAddApi):
-    """
-    添加用户
-    """
-    api.resp.uid = 1
-    return api.json_resp()
-
-
-@users_blueprint.route("/<uid>", methods=["DELETE"])
-async def user_del(request: Request, uid: int, api: UserDelApi):
-    """
-    刪除一个用户
-    """
-
-    api.resp.uid = uid
-
-    return api.json_resp()
-
-
-@users_blueprint.route("/<uid>", methods=["PUT"])
-async def user_update(request: Request, uid: int, api: UserUpdateApi):
-    """
-    更新一个用户
-    """
-
-    api.resp.uid = uid
-
-    return api.json_resp()
-
-
-@users_blueprint.route("/<uid>", methods=["GET"])
-async def user_one(request: Request, uid: int, api: UserFindOneApi):
-    """
-    获取一个用户
-    """
-
-    api.resp.uid = 1
-    api.resp.username = "username"
-    api.resp.password = uuid4().hex
-
-    return api.json_resp()
-
-
-@users_blueprint.route("/", methods=["GET"])
-async def user_list(request: Request, api: UserListApi):
-    """
-    获取一些用户
-    """
-
-    users: List[Dict[str, Any]] = [
-        {
-            "uid": 1,
-            "username": "user1",
-        },
-        {
-            "uid": 2,
-            "username": "user2",
-        },
-    ]
-    for user in users:
-        api.resp.username = user["username"]
-        api.resp.uid = user["uid"]
-        api.resp.add_data()
-
-    return api.json_resp()
+from typing import Any, Dict, List
+from uuid import uuid4
+
+from sanic import Blueprint, text
+from sanic.request import Request
+
+from .validator import (
+    UserAddApi,
+    UserDelApi,
+    UserFindOneApi,
+    UserListApi,
+    UserUpdateApi,
+)
+
+users_blueprint = Blueprint("users_blueprint", url_prefix="/users")
+users_blueprint.ctx.desc = "用户"
+
+
+@users_blueprint.route("/test", methods=["GET"])
+async def hello(request):
+    return text("Hello world!")
+
+
+@users_blueprint.route("/", methods=["POST"])
+async def user_add(request: Request, api: UserAddApi):
+    """
+    添加用户
+    """
+    api.resp.uid = 1
+    return api.json_resp()
+
+
+@users_blueprint.route("/<uid>", methods=["DELETE"])
+async def user_del(request: Request, uid: int, api: UserDelApi):
+    """
+    刪除一个用户
+    """
+
+    api.resp.uid = uid
+
+    return api.json_resp()
+
+
+@users_blueprint.route("/<uid>", methods=["PUT"])
+async def user_update(request: Request, uid: int, api: UserUpdateApi):
+    """
+    更新一个用户
+    """
+
+    api.resp.uid = uid
+
+    return api.json_resp()
+
+
+@users_blueprint.route("/<uid>", methods=["GET"])
+async def user_one(request: Request, uid: int, api: UserFindOneApi):
+    """
+    获取一个用户
+    """
+
+    api.resp.uid = 1
+    api.resp.username = "username"
+    api.resp.password = uuid4().hex
+
+    return api.json_resp()
+
+
+@users_blueprint.route("/", methods=["GET"])
+async def user_list(request: Request, api: UserListApi):
+    """
+    获取一些用户
+    """
+
+    users: List[Dict[str, Any]] = [
+        {
+            "uid": 1,
+            "username": "user1",
+        },
+        {
+            "uid": 2,
+            "username": "user2",
+        },
+    ]
+    for user in users:
+        api.resp.username = user["username"]
+        api.resp.uid = user["uid"]
+        api.resp.add_data()
+
+    return api.json_resp()
```

### Comparing `sanic-api-0.2.5/example/api/validator.py` & `sanic-api-0.2.6/example/api/validator.py`

 * *Ordering differences only*

 * *Files 26% similar despite different names*

```diff
@@ -1,97 +1,97 @@
-from pydantic import BaseModel, Field
-
-from sanic_api.api import API
-from sanic_api.api.model import ListRespModel, ResponseModel
-
-
-class Pagination(BaseModel):
-    """
-    分页
-    """
-
-    page: int = Field(1, gt=0, title="页数")
-    per_page: int = Field(20, title="每页数量", gt=0, lt=100)
-
-
-class ListParam(Pagination):
-    """
-    列表
-    """
-
-    orderings: str = Field(None, title="排序字段", description='排序字段，多个字段 ”,“ 分割，倒序使用 "-", 如："id, -name"')
-
-
-class UserModel(BaseModel):
-    username: str = Field(title="用户名")
-    password: str = Field(title="密码", description="密码，经过md5加密的")
-
-
-class AddUserReqModel(BaseModel):
-    """
-    添加请求参数
-    """
-
-    user: UserModel = Field(title="用户信息")
-
-
-class AddUserRespModel(ResponseModel):
-    """
-    响应参数
-    """
-
-    uid: int = Field(default=None, title="用户ID", description="创建用户的用户ID")
-
-
-class FindOneUserRespModel(UserModel, AddUserRespModel):
-    """
-    响应参数
-    """
-
-
-class UserListRespModel(ListRespModel, FindOneUserRespModel):
-    """
-    用户列表响应参数
-    """
-
-
-class UserAddApi(API):
-    """
-    添加用户API
-    """
-
-    json_req: AddUserReqModel
-    resp: AddUserRespModel
-
-
-class UserDelApi(API):
-    """
-    删除用户API
-    """
-
-    resp: AddUserRespModel
-
-
-class UserUpdateApi(UserAddApi):
-    """
-    更新用户API
-    """
-
-    json_req: AddUserReqModel
-    resp: AddUserRespModel
-
-
-class UserFindOneApi(API):
-    """
-    查询单个用户API
-    """
-
-    resp: FindOneUserRespModel
-
-
-class UserListApi(API):
-    """
-    用户列表API
-    """
-
-    query_req: ListParam
-    resp: UserListRespModel
+from pydantic import BaseModel, Field
+
+from sanic_api.api import API
+from sanic_api.api.model import ListRespModel, ResponseModel
+
+
+class Pagination(BaseModel):
+    """
+    分页
+    """
+
+    page: int = Field(1, gt=0, title="页数")
+    per_page: int = Field(20, title="每页数量", gt=0, lt=100)
+
+
+class ListParam(Pagination):
+    """
+    列表
+    """
+
+    orderings: str = Field(None, title="排序字段", description='排序字段，多个字段 ”,“ 分割，倒序使用 "-", 如："id, -name"')
+
+
+class UserModel(BaseModel):
+    username: str = Field(title="用户名")
+    password: str = Field(title="密码", description="密码，经过md5加密的")
+
+
+class AddUserReqModel(BaseModel):
+    """
+    添加请求参数
+    """
+
+    user: UserModel = Field(title="用户信息")
+
+
+class AddUserRespModel(ResponseModel):
+    """
+    响应参数
+    """
+
+    uid: int = Field(default=None, title="用户ID", description="创建用户的用户ID")
+
+
+class FindOneUserRespModel(UserModel, AddUserRespModel):
+    """
+    响应参数
+    """
+
+
+class UserListRespModel(ListRespModel, FindOneUserRespModel):
+    """
+    用户列表响应参数
+    """
+
+
+class UserAddApi(API):
+    """
+    添加用户API
+    """
+
+    json_req: AddUserReqModel
+    resp: AddUserRespModel
+
+
+class UserDelApi(API):
+    """
+    删除用户API
+    """
+
+    resp: AddUserRespModel
+
+
+class UserUpdateApi(UserAddApi):
+    """
+    更新用户API
+    """
+
+    json_req: AddUserReqModel
+    resp: AddUserRespModel
+
+
+class UserFindOneApi(API):
+    """
+    查询单个用户API
+    """
+
+    resp: FindOneUserRespModel
+
+
+class UserListApi(API):
+    """
+    用户列表API
+    """
+
+    query_req: ListParam
+    resp: UserListRespModel
```

### Comparing `sanic-api-0.2.5/LICENSE.txt` & `sanic-api-0.2.6/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `sanic-api-0.2.5/pyproject.toml` & `sanic-api-0.2.6/pyproject.toml`

 * *Files 11% similar despite different names*

```diff
@@ -1,22 +1,23 @@
 [project]
 name = "sanic-api"
-version = "0.2.5"
+version = "0.2.6"
 description = "Sanic 框架实用API工具集，拥有自动生成文档、参数校验、配置的导入、日志功能的优化等功能，更好的助力接口的开发"
 authors = [
     { name = "昊色居士", email = "xhrtxh@gmail.com" },
 ]
 dependencies = [
-    "sanic>=22.12",
-    "pydantic>=1.10.2",
+    "sanic>=22.3",
+    "pydantic[dotenv]>=1.10.2",
     "sanic-ext>=22.12",
     "loguru>=0.6.0",
     "pygments>=2.13.0",
     "ujson>=5.7.0",
     "orjson>=3.8.6",
+    "setuptools>=68.0.0",
 ]
 requires-python = ">=3.8"
 readme = "README.MD"
 
 [project.license]
 text = "MIT"
```

### Comparing `sanic-api-0.2.5/README.MD` & `sanic-api-0.2.6/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,79 +1,89 @@
-![logo](https://images.haose.pro/2022/12/19/logo_17%3A34%3A07_qkt9yi4d7u.png)
-
-[![MIT License](https://img.shields.io/badge/License-MIT-green.svg)](https://choosealicense.com/licenses/mit/)
-[![Python](https://img.shields.io/badge/Python-3.8+-yellow.svg?logo=python)]()
-[![Sanic](https://img.shields.io/badge/framework-Sanic-Server.svg)](http://www.gnu.org/licenses/agpl-3.0)
-[![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)
-
-# Sanic-API
-
-让您的sanic服务程序更好的支持API文档、参数校验、日志打印、响应规范等
-
-## 特性
-
-- 无需任何多余改动，全自动生成openapi文档，使用更加方便
-
-- 基于`pydantic`的参数校验器，让接口的请求及响应更符合你的预期
-
-- 使用`loguru`库代替官方`logging`日志库，并对访问日志进行扩展，支持打印接口耗时、接口参数
-
-- 使用`{code: 0, data: null, msg: ""}`样式的接口返回
-
-- 对接口中的异常进行拦截，及自定义错误码
-
-- 接口返回样式可自定义配置
-
-## 截图
-
-## 路线图
-
-- 增加一键生成预设项目cli命令
-
-- 编写详细文档
-
-- API接口增加请求头、URL路径参数收集和校验:
-
-## 安装
-
-使用 pip 安装 sanic-api
-
-```bash
-  pip install sanic-api
-```
-
-## 使用方法/示例
-
-```python
-from sanic import Sanic, text
-from sanic_api import init_api
-
-app = Sanic("Sanic-API")
-
-
-@app.get('/')
-async def index(request):
-    return text("Sanic-API Example")
-
-
-def main():
-    init_api(app)
-    app.run(access_log=True)
-
-
-if __name__ == '__main__':
-    main()
-
-```
-
-## 开发
-
-要部署这个项目，请运行
-
-```bash
-  pip install pdm
-  pdm sync
-```
-
-## 文档
-
-[文档](https://linktodocumentation)
+Metadata-Version: 2.1
+Name: sanic-api
+Version: 0.2.6
+Summary: Sanic 框架实用API工具集，拥有自动生成文档、参数校验、配置的导入、日志功能的优化等功能，更好的助力接口的开发
+License: MIT
+Author-email: 昊色居士 <xhrtxh@gmail.com>
+Requires-Python: >=3.8
+Description-Content-Type: text/markdown
+
+![logo](https://images.haose.pro/2022/12/19/logo_17%3A34%3A07_qkt9yi4d7u.png)
+
+[![MIT License](https://img.shields.io/badge/License-MIT-green.svg)](https://choosealicense.com/licenses/mit/)
+[![Python](https://img.shields.io/badge/Python-3.8+-yellow.svg?logo=python)]()
+[![Sanic](https://img.shields.io/badge/framework-Sanic-Server.svg)](http://www.gnu.org/licenses/agpl-3.0)
+[![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)
+
+# Sanic-API
+
+让您的sanic服务程序更好的支持API文档、参数校验、日志打印、响应规范等
+
+## 特性
+
+- 无需任何多余改动，全自动生成openapi文档，使用更加方便
+
+- 基于`pydantic`的参数校验器，让接口的请求及响应更符合你的预期
+
+- 使用`loguru`库代替官方`logging`日志库，并对访问日志进行扩展，支持打印接口耗时、接口参数
+
+- 使用`{code: 0, data: null, msg: ""}`样式的接口返回
+
+- 对接口中的异常进行拦截，及自定义错误码
+
+- 接口返回样式可自定义配置
+
+## 截图
+
+## 路线图
+
+- 增加一键生成预设项目cli命令
+
+- 编写详细文档
+
+- API接口增加请求头、URL路径参数收集和校验:
+
+## 安装
+
+使用 pip 安装 sanic-api
+
+```bash
+  pip install sanic-api
+```
+
+## 使用方法/示例
+
+```python
+from sanic import Sanic, text
+from sanic_api import init_api
+
+app = Sanic("Sanic-API")
+
+
+@app.get('/')
+async def index(request):
+    return text("Sanic-API Example")
+
+
+def main():
+    init_api(app)
+    app.run(access_log=True)
+
+
+if __name__ == '__main__':
+    main()
+
+```
+
+## 开发
+
+要部署这个项目，请运行
+
+```bash
+  pip install pdm
+  pdm sync
+```
+
+## 文档
+
+[文档](https://linktodocumentation)
+
```

### Comparing `sanic-api-0.2.5/sanic_api/api/api.py` & `sanic-api-0.2.6/sanic_api/api/api.py`

 * *Ordering differences only*

 * *Files 22% similar despite different names*

```diff
@@ -1,177 +1,177 @@
-import functools
-from abc import ABCMeta
-from typing import Any, Callable, Dict, Optional
-
-from pydantic import BaseModel, Field
-from pydantic import ValidationError as PyDanticValidationError
-from sanic import HTTPResponse, Sanic
-from sanic.response import json
-
-from sanic_api.api.exception import ValidationError
-from sanic_api.api.model import ListRespModel, ResponseModel
-from sanic_api.enum import EnumBase, ParamEnum, RespCodeEnum
-from sanic_api.utils import json_dumps
-
-
-def get_resp_tmp(key: str, default):
-    """
-    获取响应字段模板
-    """
-    app = Sanic.get_app()
-    sanic_api: dict = app.config.get("sanic_api", {})
-    return sanic_api.get(key, default)
-
-
-class Response:
-    def __init__(
-        self,
-        http_code: int = 200,
-        headers: Optional[Dict[str, str]] = None,
-        server_code: EnumBase = RespCodeEnum.SUCCESS,
-        message: str = "Success",
-        data: Any = None,
-        response_type: Optional[type] = None,
-    ):
-        """
-        初始化函数
-        Args:
-            http_code: http响应码 默认是200
-            headers: 自定义的响应头
-            server_code: 自定义的服务码
-            message: 返回的消息
-            data: 返回的数据
-        """
-
-        self.http_code = http_code
-        self.headers = headers
-        self.message = message
-        response_type = response_type or Response.get_response_type(type(data))
-
-        if isinstance(data, ListRespModel):
-            data = data.to_list()
-        elif isinstance(data, BaseModel):
-            data = data.dict()
-
-        resp: ResponseModel = response_type()
-        code_tmp = get_resp_tmp("code_tmp", "code")
-        msg_tmp = get_resp_tmp("msg_tmp", "msg")
-        data_tmp = get_resp_tmp("data_tmp", "data")
-
-        setattr(resp, code_tmp, server_code)
-        setattr(resp, msg_tmp, message)
-        setattr(resp, data_tmp, data)
-
-        data = resp.dict()
-
-        self.data = data
-
-    def json_resp(self, default: Optional[Callable[[Any], Any]] = None) -> HTTPResponse:
-        """
-        返回json格式的响应
-        Args:
-
-        """
-        return json(
-            body=self.data,
-            status=self.http_code,
-            headers=self.headers,
-            dumps=functools.partial(json_dumps, default=default),
-        )
-
-    @classmethod
-    def get_response_type(cls, data_type: type):
-        """
-        获取响应的类型
-        Args:
-            data_type: 响应中data的类型
-
-        Returns:
-
-        """
-        code_tmp = get_resp_tmp("code_tmp", "code")
-        msg_tmp = get_resp_tmp("msg_tmp", "msg")
-        data_tmp = get_resp_tmp("data_tmp", "data")
-
-        attr_dict = {
-            code_tmp: Field(title="业务响应码"),
-            msg_tmp: Field(title="响应消息"),
-            data_tmp: Field(title="响应数据"),
-            "__annotations__": {code_tmp: int, msg_tmp: str, data_tmp: data_type},
-        }
-        resp_name = data_type.__name__ if data_type.__name__ != "NoneType" else "Response"
-        response_type = type(resp_name, (ResponseModel,), attr_dict)
-        return response_type
-
-    @staticmethod
-    def _get_tmp(key: str, default):
-        """
-        获取字段模板
-        """
-        app = Sanic.get_app()
-        sanic_api: dict = app.config.get("sanic_api", {})
-        return sanic_api.get(key, default)
-
-
-class API(metaclass=ABCMeta):
-    json_req: Optional[BaseModel] = None
-    form_req: Optional[BaseModel] = None
-    query_req: Optional[BaseModel] = None
-    resp: Optional[Any] = None
-    tags: list = []
-    description: str = ""
-
-    def __init__(self):
-        response_type = self.__class__.__annotations__.get("resp")
-        self.json_req_type = self.__class__.__annotations__.get("json_req")
-        self.form_req_type = self.__class__.__annotations__.get("form_req")
-        self.query_req_type = self.__class__.__annotations__.get("query_req")
-        self.response_type = Response.get_response_type(response_type)
-        self.resp = response_type()
-
-    def validate_params(self, req_data: dict, param_enum: ParamEnum):
-        """
-        验证参数，参数有问题抛出异常
-        Args:
-            req_data: 数据
-            param_enum: 参数类型
-
-        Returns:
-
-        """
-        try:
-            if param_enum == ParamEnum.JSON:
-                self.json_req = self.json_req_type(**req_data)
-            elif param_enum == ParamEnum.QUERY:
-                self.query_req = self.query_req_type(**req_data)
-            elif param_enum == ParamEnum.FORM:
-                self.form_req = self.form_req_type(**req_data)
-        except PyDanticValidationError as e:
-            raise ValidationError(e.errors()) from e
-
-    def json_resp(
-        self,
-        http_code: int = 200,
-        headers: Optional[Dict[str, str]] = None,
-        server_code: RespCodeEnum = RespCodeEnum.SUCCESS,
-        message: str = "Success",
-    ):
-        """
-        根据响应数据返回json格式的响应
-        Args:
-            http_code: http协议响应码
-            headers: 响应头
-            server_code: 应用协议响应码
-            message: 响应消息
-
-        Returns:
-            返回一个sanic的HTTPResponse
-        """
-
-        return Response(
-            data=self.resp,
-            http_code=http_code,
-            headers=headers,
-            server_code=server_code,
-            message=message,
-            response_type=self.response_type,
-        ).json_resp()
+import functools
+from abc import ABCMeta
+from typing import Any, Callable, Dict, Optional
+
+from pydantic import BaseModel, Field
+from pydantic import ValidationError as PyDanticValidationError
+from sanic import HTTPResponse, Sanic
+from sanic.response import json
+
+from sanic_api.api.exception import ValidationError
+from sanic_api.api.model import ListRespModel, ResponseModel
+from sanic_api.enum import EnumBase, ParamEnum, RespCodeEnum
+from sanic_api.utils import json_dumps
+
+
+def get_resp_tmp(key: str, default):
+    """
+    获取响应字段模板
+    """
+    app = Sanic.get_app()
+    sanic_api: dict = app.config.get("sanic_api", {})
+    return sanic_api.get(key, default)
+
+
+class Response:
+    def __init__(
+        self,
+        http_code: int = 200,
+        headers: Optional[Dict[str, str]] = None,
+        server_code: EnumBase = RespCodeEnum.SUCCESS,
+        message: str = "Success",
+        data: Any = None,
+        response_type: Optional[type] = None,
+    ):
+        """
+        初始化函数
+        Args:
+            http_code: http响应码 默认是200
+            headers: 自定义的响应头
+            server_code: 自定义的服务码
+            message: 返回的消息
+            data: 返回的数据
+        """
+
+        self.http_code = http_code
+        self.headers = headers
+        self.message = message
+        response_type = response_type or Response.get_response_type(type(data))
+
+        if isinstance(data, ListRespModel):
+            data = data.to_list()
+        elif isinstance(data, BaseModel):
+            data = data.dict()
+
+        resp: ResponseModel = response_type()
+        code_tmp = get_resp_tmp("code_tmp", "code")
+        msg_tmp = get_resp_tmp("msg_tmp", "msg")
+        data_tmp = get_resp_tmp("data_tmp", "data")
+
+        setattr(resp, code_tmp, server_code)
+        setattr(resp, msg_tmp, message)
+        setattr(resp, data_tmp, data)
+
+        data = resp.dict()
+
+        self.data = data
+
+    def json_resp(self, default: Optional[Callable[[Any], Any]] = None) -> HTTPResponse:
+        """
+        返回json格式的响应
+        Args:
+
+        """
+        return json(
+            body=self.data,
+            status=self.http_code,
+            headers=self.headers,
+            dumps=functools.partial(json_dumps, default=default),
+        )
+
+    @classmethod
+    def get_response_type(cls, data_type: type):
+        """
+        获取响应的类型
+        Args:
+            data_type: 响应中data的类型
+
+        Returns:
+
+        """
+        code_tmp = get_resp_tmp("code_tmp", "code")
+        msg_tmp = get_resp_tmp("msg_tmp", "msg")
+        data_tmp = get_resp_tmp("data_tmp", "data")
+
+        attr_dict = {
+            code_tmp: Field(title="业务响应码"),
+            msg_tmp: Field(title="响应消息"),
+            data_tmp: Field(title="响应数据"),
+            "__annotations__": {code_tmp: int, msg_tmp: str, data_tmp: data_type},
+        }
+        resp_name = data_type.__name__ if data_type.__name__ != "NoneType" else "Response"
+        response_type = type(resp_name, (ResponseModel,), attr_dict)
+        return response_type
+
+    @staticmethod
+    def _get_tmp(key: str, default):
+        """
+        获取字段模板
+        """
+        app = Sanic.get_app()
+        sanic_api: dict = app.config.get("sanic_api", {})
+        return sanic_api.get(key, default)
+
+
+class API(metaclass=ABCMeta):
+    json_req: Optional[BaseModel] = None
+    form_req: Optional[BaseModel] = None
+    query_req: Optional[BaseModel] = None
+    resp: Optional[Any] = None
+    tags: list = []
+    description: str = ""
+
+    def __init__(self):
+        response_type = self.__class__.__annotations__.get("resp")
+        self.json_req_type = self.__class__.__annotations__.get("json_req")
+        self.form_req_type = self.__class__.__annotations__.get("form_req")
+        self.query_req_type = self.__class__.__annotations__.get("query_req")
+        self.response_type = Response.get_response_type(response_type)
+        self.resp = response_type()
+
+    def validate_params(self, req_data: dict, param_enum: ParamEnum):
+        """
+        验证参数，参数有问题抛出异常
+        Args:
+            req_data: 数据
+            param_enum: 参数类型
+
+        Returns:
+
+        """
+        try:
+            if param_enum == ParamEnum.JSON:
+                self.json_req = self.json_req_type(**req_data)
+            elif param_enum == ParamEnum.QUERY:
+                self.query_req = self.query_req_type(**req_data)
+            elif param_enum == ParamEnum.FORM:
+                self.form_req = self.form_req_type(**req_data)
+        except PyDanticValidationError as e:
+            raise ValidationError(e.errors()) from e
+
+    def json_resp(
+        self,
+        http_code: int = 200,
+        headers: Optional[Dict[str, str]] = None,
+        server_code: RespCodeEnum = RespCodeEnum.SUCCESS,
+        message: str = "Success",
+    ):
+        """
+        根据响应数据返回json格式的响应
+        Args:
+            http_code: http协议响应码
+            headers: 响应头
+            server_code: 应用协议响应码
+            message: 响应消息
+
+        Returns:
+            返回一个sanic的HTTPResponse
+        """
+
+        return Response(
+            data=self.resp,
+            http_code=http_code,
+            headers=headers,
+            server_code=server_code,
+            message=message,
+            response_type=self.response_type,
+        ).json_resp()
```

### Comparing `sanic-api-0.2.5/sanic_api/api/extend.py` & `sanic-api-0.2.6/sanic_api/api/extend.py`

 * *Ordering differences only*

 * *Files 26% similar despite different names*

```diff
@@ -1,25 +1,25 @@
-from sanic.exceptions import NotFound
-from sanic_ext import Extension
-
-from sanic_api.api.exception import ServerException
-
-from .handle_exception import not_found, other_exception, server_exception
-from .validators import validators
-
-
-class ApiExtend(Extension):
-    """
-    接口处理扩展
-    参数校验、异常拦截等功能
-    """
-
-    name = "ApiExtend"
-
-    def startup(self, bootstrap) -> None:
-        if not self.included():
-            return
-
-        self.app.error_handler.add(ServerException, server_exception)
-        self.app.error_handler.add(Exception, other_exception)
-        self.app.error_handler.add(NotFound, not_found)
-        self.app.on_request(validators, priority=998)
+from sanic.exceptions import NotFound
+from sanic_ext import Extension
+
+from sanic_api.api.exception import ServerException
+
+from .handle_exception import not_found, other_exception, server_exception
+from .validators import validators
+
+
+class ApiExtend(Extension):
+    """
+    接口处理扩展
+    参数校验、异常拦截等功能
+    """
+
+    name = "ApiExtend"
+
+    def startup(self, bootstrap) -> None:
+        if not self.included():
+            return
+
+        self.app.error_handler.add(ServerException, server_exception)
+        self.app.error_handler.add(Exception, other_exception)
+        self.app.error_handler.add(NotFound, not_found)
+        self.app.on_request(validators, priority=998)
```

### Comparing `sanic-api-0.2.5/sanic_api/api/model.py` & `sanic-api-0.2.6/sanic_api/api/model.py`

 * *Ordering differences only*

 * *Files 21% similar despite different names*

```diff
@@ -1,45 +1,45 @@
-from typing import Optional, Union
-
-from pydantic.fields import ModelField, ModelPrivateAttr
-from pydantic.main import BaseModel
-
-
-class ResponseModel(BaseModel):
-    """
-    响应基础模型
-    """
-
-    def __new__(cls, *args, **kwargs):
-        for _field, value in cls.__fields__.items():
-            if not isinstance(value, ModelField):
-                continue
-            value.required = False
-
-        return super().__new__(cls, *args, **kwargs)
-
-
-class ListRespModel(ResponseModel):
-    """
-    列表格式的响应基础模型
-    """
-
-    _data_list: Optional[Union[ModelPrivateAttr, list]] = ModelPrivateAttr(default_factory=list)
-
-    def add_data(self):
-        """
-        当前模型下数据添加到列表中
-        Returns:
-
-        """
-        data = self.dict()
-        self._data_list.append(data)
-        for attr in data.keys():
-            self.__setattr__(attr, None)
-
-    def to_list(self):
-        """
-        返回列表响应数据
-        Returns:
-
-        """
-        return self._data_list
+from typing import Optional, Union
+
+from pydantic.fields import ModelField, ModelPrivateAttr
+from pydantic.main import BaseModel
+
+
+class ResponseModel(BaseModel):
+    """
+    响应基础模型
+    """
+
+    def __new__(cls, *args, **kwargs):
+        for _field, value in cls.__fields__.items():
+            if not isinstance(value, ModelField):
+                continue
+            value.required = False
+
+        return super().__new__(cls, *args, **kwargs)
+
+
+class ListRespModel(ResponseModel):
+    """
+    列表格式的响应基础模型
+    """
+
+    _data_list: Optional[Union[ModelPrivateAttr, list]] = ModelPrivateAttr(default_factory=list)
+
+    def add_data(self):
+        """
+        当前模型下数据添加到列表中
+        Returns:
+
+        """
+        data = self.dict()
+        self._data_list.append(data)
+        for attr in data.keys():
+            self.__setattr__(attr, None)
+
+    def to_list(self):
+        """
+        返回列表响应数据
+        Returns:
+
+        """
+        return self._data_list
```

### Comparing `sanic-api-0.2.5/sanic_api/api/validators.py` & `sanic-api-0.2.6/sanic_api/api/validators.py`

 * *Ordering differences only*

 * *Files 12% similar despite different names*

```diff
@@ -1,76 +1,76 @@
-import inspect
-
-from sanic import Request
-
-from sanic_api.api import API
-from sanic_api.api.exception import ValidationInitError
-from sanic_api.enum import ParamEnum
-
-
-def _do_validation(param_enum: ParamEnum, api: API, data: dict):
-    if param_enum == ParamEnum.JSON:
-        req_data = data
-    elif param_enum in [ParamEnum.QUERY, param_enum.FORM]:
-        req_data = {}
-        for k, v in data.items():
-            if type(v) == list and len(v) == 1:
-                req_data[k] = v[0]
-            else:
-                req_data[k] = v
-    else:
-        raise ValidationInitError("未知的验证器类型")
-
-    api.validate_params(req_data, param_enum)
-
-
-def get_handler_param(handler):
-    """
-    获取参数处理器的json、form、query参数
-    Args:
-        handler:
-
-    Returns:
-
-    """
-    sig = inspect.signature(handler)
-    api_parameter = sig.parameters.get("api")
-    api_cls = api_parameter.annotation if api_parameter else None
-    return api_cls
-
-
-async def validators(request: Request):
-    """
-    校验请求参数中间件
-    Args:
-        request: 请求
-
-    Returns:
-
-    """
-    # 如果执行中间价直接就发生了异常则直接抛出
-    if hasattr(request.ctx, "exception"):
-        raise request.ctx.exception
-
-    _, handler, _ = request.app.router.get(
-        request.path,
-        request.method,
-        request.headers.getone("host", None),
-    )
-
-    api_cls = get_handler_param(handler)
-    if not api_cls:
-        return
-
-    api: API = api_cls()
-    if api.json_req_type and api.query_req_type:
-        raise ValidationInitError("不能同时存在json参数和form参数")
-
-    if api.json_req_type and request.json:
-        _do_validation(param_enum=ParamEnum.JSON, api=api, data=request.json)
-    elif api.form_req_type and request.form:
-        _do_validation(param_enum=ParamEnum.FORM, api=api, data=request.form)
-    if api.query_req_type and request.query_args:
-        _do_validation(param_enum=ParamEnum.QUERY, api=api, data=request.args)
-
-    request.match_info.update({"api": api})
-    request.ctx.api = api
+import inspect
+
+from sanic import Request
+
+from sanic_api.api import API
+from sanic_api.api.exception import ValidationInitError
+from sanic_api.enum import ParamEnum
+
+
+def _do_validation(param_enum: ParamEnum, api: API, data: dict):
+    if param_enum == ParamEnum.JSON:
+        req_data = data
+    elif param_enum in [ParamEnum.QUERY, param_enum.FORM]:
+        req_data = {}
+        for k, v in data.items():
+            if type(v) == list and len(v) == 1:
+                req_data[k] = v[0]
+            else:
+                req_data[k] = v
+    else:
+        raise ValidationInitError("未知的验证器类型")
+
+    api.validate_params(req_data, param_enum)
+
+
+def get_handler_param(handler):
+    """
+    获取参数处理器的json、form、query参数
+    Args:
+        handler:
+
+    Returns:
+
+    """
+    sig = inspect.signature(handler)
+    api_parameter = sig.parameters.get("api")
+    api_cls = api_parameter.annotation if api_parameter else None
+    return api_cls
+
+
+async def validators(request: Request):
+    """
+    校验请求参数中间件
+    Args:
+        request: 请求
+
+    Returns:
+
+    """
+    # 如果执行中间价直接就发生了异常则直接抛出
+    if hasattr(request.ctx, "exception"):
+        raise request.ctx.exception
+
+    _, handler, _ = request.app.router.get(
+        request.path,
+        request.method,
+        request.headers.getone("host", None),
+    )
+
+    api_cls = get_handler_param(handler)
+    if not api_cls:
+        return
+
+    api: API = api_cls()
+    if api.json_req_type and api.query_req_type:
+        raise ValidationInitError("不能同时存在json参数和form参数")
+
+    if api.json_req_type and request.json:
+        _do_validation(param_enum=ParamEnum.JSON, api=api, data=request.json)
+    elif api.form_req_type and request.form:
+        _do_validation(param_enum=ParamEnum.FORM, api=api, data=request.form)
+    if api.query_req_type and request.query_args:
+        _do_validation(param_enum=ParamEnum.QUERY, api=api, data=request.args)
+
+    request.match_info.update({"api": api})
+    request.ctx.api = api
```

### Comparing `sanic-api-0.2.5/sanic_api/config/setting.py` & `sanic-api-0.2.6/sanic_api/config/setting.py`

 * *Ordering differences only*

 * *Files 10% similar despite different names*

```diff
@@ -1,30 +1,30 @@
-from pydantic import Field
-
-from sanic_api.config.base import SettingsBase
-from sanic_api.config.sanic import SanicConfig
-from sanic_api.config.sanic_api import SanicApiConfig
-from sanic_api.enum import RunModeEnum
-
-
-class DefaultSettings(SettingsBase):
-    """
-    配置类
-    """
-
-    # 主机
-    host: str = Field(default="127.0.0.1")
-
-    # 端口
-    port: int = Field(default=5798)
-
-    # 运行模式
-    mode: RunModeEnum = Field(default=RunModeEnum.DEV)
-
-    # 工作进程的数量
-    workers: int = Field(default=1)
-
-    # sanic 自身的配置
-    sanic: SanicConfig = Field(default_factory=SanicConfig)
-
-    # sanic_api 扩展自身需要的配置
-    sanic_api: SanicApiConfig = Field(default_factory=SanicApiConfig)
+from pydantic import Field
+
+from sanic_api.config.base import SettingsBase
+from sanic_api.config.sanic import SanicConfig
+from sanic_api.config.sanic_api import SanicApiConfig
+from sanic_api.enum import RunModeEnum
+
+
+class DefaultSettings(SettingsBase):
+    """
+    配置类
+    """
+
+    # 主机
+    host: str = Field(default="127.0.0.1")
+
+    # 端口
+    port: int = Field(default=5798)
+
+    # 运行模式
+    mode: RunModeEnum = Field(default=RunModeEnum.DEV)
+
+    # 工作进程的数量
+    workers: int = Field(default=1)
+
+    # sanic 自身的配置
+    sanic: SanicConfig = Field(default_factory=SanicConfig)
+
+    # sanic_api 扩展自身需要的配置
+    sanic_api: SanicApiConfig = Field(default_factory=SanicApiConfig)
```

### Comparing `sanic-api-0.2.5/sanic_api/enum.py` & `sanic-api-0.2.6/sanic_api/enum.py`

 * *Ordering differences only*

 * *Files 25% similar despite different names*

```diff
@@ -1,88 +1,88 @@
-import json
-from dataclasses import dataclass, field
-from enum import Enum, auto
-from types import DynamicClassAttribute
-from typing import Any
-
-
-@dataclass
-class EnumField:
-    """
-    枚举字段类
-    """
-
-    value: Any = field(default=auto())
-    desc: str = field(default_factory=str)
-
-
-class EnumBase(Enum):
-    """
-    枚举基类
-    """
-
-    @classmethod
-    def _missing_(cls, value: object) -> Any:
-        result = list(filter(lambda d: d.value == value, cls))  # type: ignore
-        return result[0] if result else None
-
-    @DynamicClassAttribute
-    def value(self) -> Any:
-        """
-        获取枚举的值
-        Returns:
-
-        """
-        if isinstance(self._value_, EnumField):
-            return self._value_.value
-        return self._value_
-
-    @DynamicClassAttribute
-    def desc(self) -> str:
-        """
-        获取枚举值的描述
-        Returns:
-
-        """
-        if isinstance(self._value_, EnumField):
-            return self._value_.desc
-        else:
-            return ""
-
-    @classmethod
-    def list(cls) -> list:
-        return [c.value for c in cls]
-
-    @classmethod
-    def to_desc(cls) -> str:
-        data = {d.value: d.desc for d in cls}
-        return json.dumps(data, ensure_ascii=False)
-
-
-class RespCodeEnum(EnumBase):
-    """
-    响应码枚举
-    """
-
-    SUCCESS = EnumField(10000, desc="成功")
-    FAILED = EnumField(40000, desc="失败")
-    PARAM_FAILED = EnumField(40001, desc="参数校验失败")
-
-
-class ParamEnum(EnumBase):
-    """
-    参数位置
-    """
-
-    JSON = EnumField("json")
-    FORM = EnumField("form")
-    QUERY = EnumField("query")
-
-
-class RunModeEnum(EnumBase):
-    """
-    运行模式
-    """
-
-    DEV = EnumField("dev", desc="开发模式。相当于debug模式加自动重载")
-    DEBUG = EnumField("debug", desc="调试模式。单workers启动。输出将更加详细，并将禁用多个运行时优化")
-    PRODUCTION = EnumField("production", desc="生产模式。如未指定workers数量，则自动使用fast模式启动。")
+import json
+from dataclasses import dataclass, field
+from enum import Enum, auto
+from types import DynamicClassAttribute
+from typing import Any
+
+
+@dataclass
+class EnumField:
+    """
+    枚举字段类
+    """
+
+    value: Any = field(default=auto())
+    desc: str = field(default_factory=str)
+
+
+class EnumBase(Enum):
+    """
+    枚举基类
+    """
+
+    @classmethod
+    def _missing_(cls, value: object) -> Any:
+        result = list(filter(lambda d: d.value == value, cls))  # type: ignore
+        return result[0] if result else None
+
+    @DynamicClassAttribute
+    def value(self) -> Any:
+        """
+        获取枚举的值
+        Returns:
+
+        """
+        if isinstance(self._value_, EnumField):
+            return self._value_.value
+        return self._value_
+
+    @DynamicClassAttribute
+    def desc(self) -> str:
+        """
+        获取枚举值的描述
+        Returns:
+
+        """
+        if isinstance(self._value_, EnumField):
+            return self._value_.desc
+        else:
+            return ""
+
+    @classmethod
+    def list(cls) -> list:
+        return [c.value for c in cls]
+
+    @classmethod
+    def to_desc(cls) -> str:
+        data = {d.value: d.desc for d in cls}
+        return json.dumps(data, ensure_ascii=False)
+
+
+class RespCodeEnum(EnumBase):
+    """
+    响应码枚举
+    """
+
+    SUCCESS = EnumField(10000, desc="成功")
+    FAILED = EnumField(40000, desc="失败")
+    PARAM_FAILED = EnumField(40001, desc="参数校验失败")
+
+
+class ParamEnum(EnumBase):
+    """
+    参数位置
+    """
+
+    JSON = EnumField("json")
+    FORM = EnumField("form")
+    QUERY = EnumField("query")
+
+
+class RunModeEnum(EnumBase):
+    """
+    运行模式
+    """
+
+    DEV = EnumField("dev", desc="开发模式。相当于debug模式加自动重载")
+    DEBUG = EnumField("debug", desc="调试模式。单workers启动。输出将更加详细，并将禁用多个运行时优化")
+    PRODUCTION = EnumField("production", desc="生产模式。如未指定workers数量，则自动使用fast模式启动。")
```

### Comparing `sanic-api-0.2.5/sanic_api/logger/config.py` & `sanic-api-0.2.6/sanic_api/logger/config.py`

 * *Ordering differences only*

 * *Files 25% similar despite different names*

```diff
@@ -1,77 +1,77 @@
-import logging
-import logging.config
-import sys
-from types import FrameType
-from typing import Optional, Union
-
-import sanic.exceptions
-from loguru import logger
-from pygments import highlight
-from pygments.formatters.terminal import TerminalFormatter
-from pygments.lexers.sql import PostgresLexer
-from sanic import Request
-
-
-class InterceptHandler(logging.StreamHandler):
-    def emit(self, record: logging.LogRecord):
-        # Get corresponding Loguru level if it exists
-        try:
-            level: Union[int, str] = logger.level(record.levelname).name
-        except ValueError:
-            level = record.levelno
-
-        # Find caller from where originated the logged message.
-        # noinspection PyProtectedMember,PyUnresolvedReferences
-        frame: Optional[FrameType] = sys._getframe(6)
-        depth: int = 6
-        while frame and frame.f_code.co_filename == logging.__file__:
-            frame = frame.f_back
-            depth += 1
-
-        fmt = "%(message)s"
-        sanic_access_fmt = "[%(host)s]: %(request)s %(message)s %(status)d %(byte)s %(time)s%(req_args)s"
-        fmt = fmt if record.name != "sanic.access" else sanic_access_fmt
-        formatter = logging.Formatter(fmt=fmt)
-        msg = formatter.format(record)
-        msg = self.highlight_sql(record, msg)
-        req_id = self.get_req_id()
-
-        if "Dispatching signal" not in msg:
-            etxra_data = {"type": record.name, "req_id": req_id}
-            logger.bind(**etxra_data).opt(depth=depth, exception=record.exc_info).log(level, msg)
-
-    @staticmethod
-    def get_req_id():
-        """
-        获取请求ID
-        """
-        try:
-            req = Request.get_current()
-            req_id = f" [{req.id}] "
-        except sanic.exceptions.ServerError:
-            req_id = " "
-        return req_id
-
-    def highlight_sql(self, record: logging.LogRecord, message: str):
-        """
-        打印日志时高亮SQl
-        Args:
-            record: 日志记录
-            message: 日志消息
-
-        Returns:
-
-        """
-        name = record.name
-        postgres = PostgresLexer()
-        terminal_formatter = TerminalFormatter()
-
-        if name == "tortoise.db_client":
-            if (
-                record.levelname == "DEBUG"
-                and not message.startswith("Created connection pool")
-                and not message.startswith("Closed connection pool")
-            ):
-                message = highlight(message, postgres, terminal_formatter).rstrip()
-
-        return message
+import logging
+import logging.config
+import sys
+from types import FrameType
+from typing import Optional, Union
+
+import sanic.exceptions
+from loguru import logger
+from pygments import highlight
+from pygments.formatters.terminal import TerminalFormatter
+from pygments.lexers.sql import PostgresLexer
+from sanic import Request
+
+
+class InterceptHandler(logging.StreamHandler):
+    def emit(self, record: logging.LogRecord):
+        # Get corresponding Loguru level if it exists
+        try:
+            level: Union[int, str] = logger.level(record.levelname).name
+        except ValueError:
+            level = record.levelno
+
+        # Find caller from where originated the logged message.
+        # noinspection PyProtectedMember,PyUnresolvedReferences
+        frame: Optional[FrameType] = sys._getframe(6)
+        depth: int = 6
+        while frame and frame.f_code.co_filename == logging.__file__:
+            frame = frame.f_back
+            depth += 1
+
+        fmt = "%(message)s"
+        sanic_access_fmt = "[%(host)s]: %(request)s %(message)s %(status)d %(byte)s %(time)s%(req_args)s"
+        fmt = fmt if record.name != "sanic.access" else sanic_access_fmt
+        formatter = logging.Formatter(fmt=fmt)
+        msg = formatter.format(record)
+        msg = self.highlight_sql(record, msg)
+        req_id = self.get_req_id()
+
+        if "Dispatching signal" not in msg:
+            etxra_data = {"type": record.name, "req_id": req_id}
+            logger.bind(**etxra_data).opt(depth=depth, exception=record.exc_info).log(level, msg)
+
+    @staticmethod
+    def get_req_id():
+        """
+        获取请求ID
+        """
+        try:
+            req = Request.get_current()
+            req_id = f" [{req.id}] "
+        except sanic.exceptions.ServerError:
+            req_id = " "
+        return req_id
+
+    def highlight_sql(self, record: logging.LogRecord, message: str):
+        """
+        打印日志时高亮SQl
+        Args:
+            record: 日志记录
+            message: 日志消息
+
+        Returns:
+
+        """
+        name = record.name
+        postgres = PostgresLexer()
+        terminal_formatter = TerminalFormatter()
+
+        if name == "tortoise.db_client":
+            if (
+                record.levelname == "DEBUG"
+                and not message.startswith("Created connection pool")
+                and not message.startswith("Closed connection pool")
+            ):
+                message = highlight(message, postgres, terminal_formatter).rstrip()
+
+        return message
```

### Comparing `sanic-api-0.2.5/sanic_api/logger/extend.py` & `sanic-api-0.2.6/sanic_api/logger/extend.py`

 * *Ordering differences only*

 * *Files 25% similar despite different names*

```diff
@@ -1,71 +1,71 @@
-import logging
-import logging.config
-import sys
-import time
-
-from loguru import logger
-
-# noinspection PyProtectedMember
-from loguru._defaults import env
-from sanic import HTTPResponse, Request
-from sanic.application.constants import Mode
-from sanic.server import HttpProtocol
-from sanic_ext import Extension
-
-from sanic_api.logger.config import InterceptHandler
-from sanic_api.logger.sanic_http import SanicHttp
-
-
-class LoggerExtend(Extension):
-    """
-    处理日志的扩展
-    """
-
-    name = "LoggerExtend"
-
-    def startup(self, bootstrap) -> None:
-        if not self.included():
-            return
-
-        log_level = logging.DEBUG if self.app.state.mode is Mode.DEBUG else logging.INFO
-        log_format = env(
-            "LOGURU_FORMAT",
-            str,
-            "<green>{time:YYYY-MM-DD HH:mm:ss.SSS}</green> | "
-            "<red>{extra[type]: <10}</red> | "
-            "<level>{level: <8}</level> | "
-            "<cyan>{name}</cyan>:<cyan>{function}</cyan>:<cyan>{line}</cyan> - {extra[req_id]}<level>{message}</level>",
-        )
-        logger.remove()
-        logger.add(sys.stdout, colorize=True, format=log_format)
-
-        logging.basicConfig(handlers=[InterceptHandler()], level=log_level, force=True)
-
-        HttpProtocol.HTTP_CLASS = SanicHttp
-        self.app.on_request(self.proc_request, priority=999)
-        self.app.on_response(self.proc_response, priority=0)
-
-    async def proc_request(self, request: Request):
-        """
-        处理请求的中间件
-        Args:
-            request:
-
-        Returns:
-
-        """
-        request.ctx.st = time.perf_counter()
-
-    async def proc_response(self, request: Request, response: HTTPResponse):
-        """
-        处理响应的中间件
-        Args:
-            request: 请求响应
-            response: 响应
-
-        Returns:
-
-        """
-        request.ctx.et = time.perf_counter()
-
-        return response
+import logging
+import logging.config
+import sys
+import time
+
+from loguru import logger
+
+# noinspection PyProtectedMember
+from loguru._defaults import env
+from sanic import HTTPResponse, Request
+from sanic.application.constants import Mode
+from sanic.server import HttpProtocol
+from sanic_ext import Extension
+
+from sanic_api.logger.config import InterceptHandler
+from sanic_api.logger.sanic_http import SanicHttp
+
+
+class LoggerExtend(Extension):
+    """
+    处理日志的扩展
+    """
+
+    name = "LoggerExtend"
+
+    def startup(self, bootstrap) -> None:
+        if not self.included():
+            return
+
+        log_level = logging.DEBUG if self.app.state.mode is Mode.DEBUG else logging.INFO
+        log_format = env(
+            "LOGURU_FORMAT",
+            str,
+            "<green>{time:YYYY-MM-DD HH:mm:ss.SSS}</green> | "
+            "<red>{extra[type]: <10}</red> | "
+            "<level>{level: <8}</level> | "
+            "<cyan>{name}</cyan>:<cyan>{function}</cyan>:<cyan>{line}</cyan> - {extra[req_id]}<level>{message}</level>",
+        )
+        logger.remove()
+        logger.add(sys.stdout, colorize=True, format=log_format)
+
+        logging.basicConfig(handlers=[InterceptHandler()], level=log_level, force=True)
+
+        HttpProtocol.HTTP_CLASS = SanicHttp
+        self.app.on_request(self.proc_request, priority=999)
+        self.app.on_response(self.proc_response, priority=0)
+
+    async def proc_request(self, request: Request):
+        """
+        处理请求的中间件
+        Args:
+            request:
+
+        Returns:
+
+        """
+        request.ctx.st = time.perf_counter()
+
+    async def proc_response(self, request: Request, response: HTTPResponse):
+        """
+        处理响应的中间件
+        Args:
+            request: 请求响应
+            response: 响应
+
+        Returns:
+
+        """
+        request.ctx.et = time.perf_counter()
+
+        return response
```

### Comparing `sanic-api-0.2.5/sanic_api/logger/sanic_http.py` & `sanic-api-0.2.6/sanic_api/logger/sanic_http.py`

 * *Ordering differences only*

 * *Files 25% similar despite different names*

```diff
@@ -1,68 +1,68 @@
-from sanic import Request
-from sanic.http import Http
-from sanic.log import access_logger
-
-from sanic_api.utils import json_dumps
-
-
-class SanicHttp(Http):
-    def log_response(self) -> None:
-        """
-        自定义输出访问日志
-        Returns:
-
-        """
-        req, res = self.request, self.response
-
-        dt = (req.ctx.et - req.ctx.st) * 1000
-        size = getattr(self, "response_bytes_left", getattr(self, "response_size", -1))
-        req_args = self.get_req_args(req)
-        extra = {
-            "status": getattr(res, "status", 0),
-            "byte": self.format_size(size),
-            "host": "UNKNOWN",
-            "request": "nil",
-            "time": f"{dt:.4f} ms",
-            "req_args": f" args: {req_args}" if req_args else "",
-        }
-        if req is not None:
-            if req.remote_addr or req.ip:
-                extra["host"] = f"{req.remote_addr or req.ip}:{req.port}"
-            extra["request"] = f"{req.method} {req.url}"
-        access_logger.info("", extra=extra)
-
-    def format_size(self, size: float):
-        """
-        格式化输出大小
-        :param size: 大小
-        :return: 返回格式化的字符串
-        """
-        for count in ["Bytes", "KB", "MB", "GB", "TB", "PB", "EB", "ZB"]:
-            if -1024.0 < size < 1024.0:
-                return f"{size:3.1f} {count}"
-            size /= 1024.0
-        return f"{size:3.1f} YB"
-
-    def get_req_args(self, request: Request) -> str:
-        """
-        获取请求参数
-        Args:
-            request: 请求
-
-        Returns:
-            返回具有 json、query、form参数的json
-        """
-        data = {}
-        for attr in ["args", "form"]:
-            attr_data = {}
-            for k, v in getattr(request, attr).items():
-                if type(v) == list and len(v) == 1:
-                    attr_data[k] = v[0]
-                else:
-                    attr_data[k] = v
-            if attr_data:
-                data[attr] = attr_data
-        if request.json:
-            data["json"] = request.json
-
-        return json_dumps(data) if data else ""
+from sanic import Request
+from sanic.http import Http
+from sanic.log import access_logger
+
+from sanic_api.utils import json_dumps
+
+
+class SanicHttp(Http):
+    def log_response(self) -> None:
+        """
+        自定义输出访问日志
+        Returns:
+
+        """
+        req, res = self.request, self.response
+
+        dt = (req.ctx.et - req.ctx.st) * 1000
+        size = getattr(self, "response_bytes_left", getattr(self, "response_size", -1))
+        req_args = self.get_req_args(req)
+        extra = {
+            "status": getattr(res, "status", 0),
+            "byte": self.format_size(size),
+            "host": "UNKNOWN",
+            "request": "nil",
+            "time": f"{dt:.4f} ms",
+            "req_args": f" args: {req_args}" if req_args else "",
+        }
+        if req is not None:
+            if req.remote_addr or req.ip:
+                extra["host"] = f"{req.remote_addr or req.ip}:{req.port}"
+            extra["request"] = f"{req.method} {req.url}"
+        access_logger.info("", extra=extra)
+
+    def format_size(self, size: float):
+        """
+        格式化输出大小
+        :param size: 大小
+        :return: 返回格式化的字符串
+        """
+        for count in ["Bytes", "KB", "MB", "GB", "TB", "PB", "EB", "ZB"]:
+            if -1024.0 < size < 1024.0:
+                return f"{size:3.1f} {count}"
+            size /= 1024.0
+        return f"{size:3.1f} YB"
+
+    def get_req_args(self, request: Request) -> str:
+        """
+        获取请求参数
+        Args:
+            request: 请求
+
+        Returns:
+            返回具有 json、query、form参数的json
+        """
+        data = {}
+        for attr in ["args", "form"]:
+            attr_data = {}
+            for k, v in getattr(request, attr).items():
+                if type(v) == list and len(v) == 1:
+                    attr_data[k] = v[0]
+                else:
+                    attr_data[k] = v
+            if attr_data:
+                data[attr] = attr_data
+        if request.json:
+            data["json"] = request.json
+
+        return json_dumps(data) if data else ""
```

### Comparing `sanic-api-0.2.5/sanic_api/openapi/openapi.py` & `sanic-api-0.2.6/sanic_api/openapi/openapi.py`

 * *Ordering differences only*

 * *Files 17% similar despite different names*

```diff
@@ -1,102 +1,102 @@
-from pydantic import BaseModel
-from sanic import Sanic
-from sanic_ext.extensions.openapi.builders import (
-    OperationBuilder,
-    OperationStore,
-    SpecificationBuilder,
-)
-from sanic_ext.extensions.openapi.definitions import Schema
-from sanic_ext.extensions.openapi.types import Array, Object
-from sanic_ext.utils.route import get_all_routes
-
-from sanic_api.api import API
-from sanic_api.api.model import ListRespModel
-from sanic_api.api.validators import get_handler_param
-
-
-# noinspection PyProtectedMember
-def auto_doc(app: Sanic):
-    config = app.config
-    specification = SpecificationBuilder()
-
-    for (
-        uri,
-        route_name,
-        _route_parameters,
-        method_handlers,
-        _host,
-    ) in get_all_routes(app, config.OAS_URL_PREFIX):
-        uri = uri if uri == "/" else uri.rstrip("/")
-
-        for method, _handler in method_handlers:
-            if (
-                (method == "OPTIONS" and app.config.OAS_IGNORE_OPTIONS)
-                or (method == "HEAD" and app.config.OAS_IGNORE_HEAD)
-                or method == "TRACE"
-            ):
-                continue
-
-            if hasattr(_handler, "view_class"):
-                _handler = getattr(_handler.view_class, method.lower())
-            operation: OperationBuilder = OperationStore()[_handler]
-
-            if operation._exclude or "openapi" in operation.tags:
-                continue
-
-            api_cls = get_handler_param(_handler)
-            if not api_cls:
-                continue
-
-            api: API = api_cls()
-
-            # 读取蓝图上面的 blueprint.ctx.desc 属性来代替name设置中文tag名
-            if len(route_name.split(".")) > 1:
-                blueprint = app.blueprints[route_name.split(".")[0]]
-                blueprint.ctx.desc = blueprint.ctx.desc or blueprint.name
-                api.tags.insert(0, blueprint.ctx.desc)
-
-            # 设置接口的标签和描述
-            tags = set(api.tags)
-            operation.tag(*tags)
-            tags_str = " ".join([f"[{tag}](/docs#tag/{tag})" for tag in tags])
-            operation.describe(description=f"### 标签: {tags_str}\n{api.description}")
-
-            if api.json_req_type:
-                body_type = api.json_req_type
-                mine_type = "application/json"
-            elif api.form_req_type:
-                body_type = api.form_req_type
-                mine_type = "application/x-www-form-urlencoded"
-            else:
-                body_type, mine_type, body_dict = ["", "", {}]
-
-            if body_type:
-                body_schema: dict = body_type.schema(ref_template="#/components/schemas/{model}")
-                body_dict = {
-                    mine_type: Object(body_schema["properties"]),
-                }
-                for model_name, schema_model in body_schema.get("definitions", {}).items():
-                    specification.add_component("schemas", model_name, schema_model)
-                body_dict[mine_type]._fields["required"] = body_schema.get("required", [])
-                operation.body(body_dict)
-
-            if api.query_req_type:
-                for k, v in api.query_req_type.schema()["properties"].items():  # type: (str, dict)
-                    operation.parameter(k, Schema(**v))
-
-            if api.response_type and issubclass(api.response_type, BaseModel):
-                resp_schema = api.response_type.schema(ref_template="#/components/schemas/{model}")
-                schema: Schema = Object(resp_schema["properties"])
-                if issubclass(api.response_type, ListRespModel):
-                    schema = Array(schema)
-                for model_name, schema_model in resp_schema.get("definitions", {}).items():
-                    specification.add_component("schemas", model_name, schema_model)
-                operation.response(
-                    status=200,
-                    content={"application/json": schema},
-                    description="成功",
-                )
-                specification.add_component("schemas", api.response_type.__name__, schema)
-
-            operation._app = app
-            specification.operation(uri, method, operation)
+from pydantic import BaseModel
+from sanic import Sanic
+from sanic_ext.extensions.openapi.builders import (
+    OperationBuilder,
+    OperationStore,
+    SpecificationBuilder,
+)
+from sanic_ext.extensions.openapi.definitions import Schema
+from sanic_ext.extensions.openapi.types import Array, Object
+from sanic_ext.utils.route import get_all_routes
+
+from sanic_api.api import API
+from sanic_api.api.model import ListRespModel
+from sanic_api.api.validators import get_handler_param
+
+
+# noinspection PyProtectedMember
+def auto_doc(app: Sanic):
+    config = app.config
+    specification = SpecificationBuilder()
+
+    for (
+        uri,
+        route_name,
+        _route_parameters,
+        method_handlers,
+        _host,
+    ) in get_all_routes(app, config.OAS_URL_PREFIX):
+        uri = uri if uri == "/" else uri.rstrip("/")
+
+        for method, _handler in method_handlers:
+            if (
+                (method == "OPTIONS" and app.config.OAS_IGNORE_OPTIONS)
+                or (method == "HEAD" and app.config.OAS_IGNORE_HEAD)
+                or method == "TRACE"
+            ):
+                continue
+
+            if hasattr(_handler, "view_class"):
+                _handler = getattr(_handler.view_class, method.lower())
+            operation: OperationBuilder = OperationStore()[_handler]
+
+            if operation._exclude or "openapi" in operation.tags:
+                continue
+
+            api_cls = get_handler_param(_handler)
+            if not api_cls:
+                continue
+
+            api: API = api_cls()
+
+            # 读取蓝图上面的 blueprint.ctx.desc 属性来代替name设置中文tag名
+            if len(route_name.split(".")) > 1:
+                blueprint = app.blueprints[route_name.split(".")[0]]
+                blueprint.ctx.desc = blueprint.ctx.desc or blueprint.name
+                api.tags.insert(0, blueprint.ctx.desc)
+
+            # 设置接口的标签和描述
+            tags = set(api.tags)
+            operation.tag(*tags)
+            tags_str = " ".join([f"[{tag}](/docs#tag/{tag})" for tag in tags])
+            operation.describe(description=f"### 标签: {tags_str}\n{api.description}")
+
+            if api.json_req_type:
+                body_type = api.json_req_type
+                mine_type = "application/json"
+            elif api.form_req_type:
+                body_type = api.form_req_type
+                mine_type = "application/x-www-form-urlencoded"
+            else:
+                body_type, mine_type, body_dict = ["", "", {}]
+
+            if body_type:
+                body_schema: dict = body_type.schema(ref_template="#/components/schemas/{model}")
+                body_dict = {
+                    mine_type: Object(body_schema["properties"]),
+                }
+                for model_name, schema_model in body_schema.get("definitions", {}).items():
+                    specification.add_component("schemas", model_name, schema_model)
+                body_dict[mine_type]._fields["required"] = body_schema.get("required", [])
+                operation.body(body_dict)
+
+            if api.query_req_type:
+                for k, v in api.query_req_type.schema()["properties"].items():  # type: (str, dict)
+                    operation.parameter(k, Schema(**v))
+
+            if api.response_type and issubclass(api.response_type, BaseModel):
+                resp_schema = api.response_type.schema(ref_template="#/components/schemas/{model}")
+                schema: Schema = Object(resp_schema["properties"])
+                if issubclass(api.response_type, ListRespModel):
+                    schema = Array(schema)
+                for model_name, schema_model in resp_schema.get("definitions", {}).items():
+                    specification.add_component("schemas", model_name, schema_model)
+                operation.response(
+                    status=200,
+                    content={"application/json": schema},
+                    description="成功",
+                )
+                specification.add_component("schemas", api.response_type.__name__, schema)
+
+            operation._app = app
+            specification.operation(uri, method, operation)
```

### Comparing `sanic-api-0.2.5/sanic_api/utils.py` & `sanic-api-0.2.6/sanic_api/utils.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,97 +1,112 @@
-from decimal import Decimal
-from importlib import import_module
-from inspect import getmembers
-from pathlib import Path
-from typing import Any, Dict, Optional
-
-import orjson
-from sanic import Blueprint, Request, Sanic
-from sanic.blueprint_group import BlueprintGroup
-from sanic.exceptions import ServerError as SanicServerError
-
-
-def getpath_by_root(path: str) -> Path:
-    """
-    根据根目录获取路径
-    基于 os.getcwd() 的同级路径、父目录来获取
-    Args:
-        path: 相对server的子路径
-
-    Returns:
-        完整路径
-    """
-    return (Path.cwd() / path).absolute()
-
-
-def json_dumps(data: dict, default=None) -> str:
-    """
-    调用orjson进行dumps
-    Args:
-        data: 数据
-        default: 数量处理方法
-
-    Returns:
-        返回json字符串
-    """
-
-    def _default(item):
-        if isinstance(item, Decimal):
-            return float(item.to_eng_string())
-
-    json_bytes = orjson.dumps(
-        data,
-        default=default or _default,
-        option=orjson.OPT_APPEND_NEWLINE | orjson.OPT_INDENT_2,
-    )
-    return json_bytes.decode("utf-8")
-
-
-def get_current_request() -> Optional[Request]:
-    """ "
-    获取当前请求
-    """
-    try:
-        return Request.get_current()
-    except SanicServerError:
-        return None
-
-
-def auto_blueprint(sanic_app: Sanic, base_api_module_name):
-    """
-    自动生成蓝图
-    Args:
-        sanic_app: app
-        base_api_module_name: api层模块名称
-
-    Returns:
-
-    """
-    # api层名称
-    base_api_name: str = base_api_module_name.split(".")[-1]
-    # api层模块
-    base_api_module = import_module(base_api_module_name, sanic_app.__module__)
-    # api层目录
-    base_api_dir = Path(str(base_api_module.__file__)).parent
-
-    # 所有路由组的字典
-    blueprint_group: Dict[str, BlueprintGroup] = {base_api_name: BlueprintGroup(base_api_name)}
-
-    # 遍历所有__init__文件找到所有蓝图
-    for path in base_api_dir.rglob("__init__.py"):
-        # 蓝图所在上层的模块
-        modules = [p.name for p in path.parents if str(base_api_dir.parent) in str(p)]
-        specmod = import_module(".".join(modules[::-1]), sanic_app.__module__)
-
-        # 获取该模块下的所有蓝图
-        blueprints = [m[1] for m in getmembers(specmod, lambda o: isinstance(o, Blueprint))]
-
-        blueprint_modules = modules[:-1]
-        for index, m in enumerate(blueprint_modules):
-            blueprint_group[m] = blueprint_group.get(m, Blueprint.group())
-            if index == 0:
-                blueprint_group[m].extend(blueprints)
-            else:
-                prev_bg: Any = blueprint_group.get(blueprint_modules[index - 1])
-                blueprint_group[m].append(prev_bg)
-
-    sanic_app.blueprint(blueprint_group[base_api_name])
+from decimal import Decimal
+from importlib import import_module
+from pathlib import Path
+from typing import Dict, List, Optional
+
+import orjson
+from sanic import Blueprint, Request, Sanic
+from sanic.blueprint_group import BlueprintGroup
+from sanic.exceptions import ServerError as SanicServerError
+
+
+def getpath_by_root(path: str) -> Path:
+    """
+    根据根目录获取路径
+    基于 os.getcwd() 的同级路径、父目录来获取
+    Args:
+        path: 相对server的子路径
+
+    Returns:
+        完整路径
+    """
+    return (Path.cwd() / path).absolute()
+
+
+def json_dumps(data: dict, default=None) -> str:
+    """
+    调用orjson进行dumps
+    Args:
+        data: 数据
+        default: 数量处理方法
+
+    Returns:
+        返回json字符串
+    """
+
+    def _default(item):
+        if isinstance(item, Decimal):
+            return float(item.to_eng_string())
+
+    json_bytes = orjson.dumps(
+        data,
+        default=default or _default,
+        option=orjson.OPT_APPEND_NEWLINE | orjson.OPT_INDENT_2,
+    )
+    return json_bytes.decode("utf-8")
+
+
+def get_current_request() -> Optional[Request]:
+    """ "
+    获取当前请求
+    """
+    try:
+        return Request.get_current()
+    except SanicServerError:
+        return None
+
+
+def auto_blueprint(sanic_app: Sanic, base_api_module_name: str) -> None:
+    """
+    自动生成蓝图
+    Args:
+        sanic_app: app
+        base_api_module_name: api层模块名称
+
+    Returns:
+
+    """
+    # 导入base_api_module_name模块并获取其文件夹路径
+    base_api_dir: Path = Path.cwd() / base_api_module_name
+
+    # 创建根API蓝图组
+    root_group: BlueprintGroup = BlueprintGroup(base_api_module_name)
+
+    blueprint_group_map: Dict[str, BlueprintGroup] = {}
+
+    # 遍历所有__init__.py文件，查找蓝图并创建对应的蓝图组
+    init_files: List[Path] = list(base_api_dir.glob("**/__init__.py"))
+    for init_file in reversed(init_files):
+        # 忽略__init__.py
+        init_file: Path = init_file.parent
+        # 获取该蓝图所在的模块路径和名称
+        module_path: str = init_file.relative_to(base_api_dir.parent).with_suffix("").as_posix()
+        module_name: str = module_path.replace("/", ".")
+
+        # 导入蓝图所在的模块，并获取该模块下的所有蓝图
+        module = import_module(module_name, base_api_module_name)
+        blueprints = [getattr(module, attr) for attr in dir(module) if isinstance(getattr(module, attr), Blueprint)]
+        # 拆分模块路径，创建对应的蓝图组并添加到父级蓝图组中
+        parts = [path for path in module_path.split("/") if path not in [base_api_module_name, init_file.name]]
+
+        if len(blueprints) == 1:
+            blueprint = blueprints[0]
+            if not parts:
+                blueprint_group = blueprint_group_map.get(init_file.name)
+                if blueprint_group:
+                    blueprint.url_prefix = ""
+                    blueprint_group.append(blueprint)
+                    root_group.append(blueprint_group)
+                else:
+                    root_group.append(blueprint)
+            else:
+                for part in parts:
+                    group = blueprint_group_map.get(part, BlueprintGroup(part))
+                    group.append(blueprint)
+                    blueprint_group_map[part] = group
+        else:
+            group = BlueprintGroup(init_file.name)
+            group.extend(blueprints)
+            root_group.append(group)
+
+    # 将根API蓝图组添加到应用中
+    sanic_app.blueprint(root_group)
```

### Comparing `sanic-api-0.2.5/PKG-INFO` & `sanic-api-0.2.6/README.MD`

 * *Files 11% similar despite different names*

```diff
@@ -1,16 +1,7 @@
-Metadata-Version: 2.1
-Name: sanic-api
-Version: 0.2.5
-Summary: Sanic 框架实用API工具集，拥有自动生成文档、参数校验、配置的导入、日志功能的优化等功能，更好的助力接口的开发
-License: MIT
-Author-email: 昊色居士 <xhrtxh@gmail.com>
-Requires-Python: >=3.8
-Description-Content-Type: text/markdown
-
 ![logo](https://images.haose.pro/2022/12/19/logo_17%3A34%3A07_qkt9yi4d7u.png)
 
 [![MIT License](https://img.shields.io/badge/License-MIT-green.svg)](https://choosealicense.com/licenses/mit/)
 [![Python](https://img.shields.io/badge/Python-3.8+-yellow.svg?logo=python)]()
 [![Sanic](https://img.shields.io/badge/framework-Sanic-Server.svg)](http://www.gnu.org/licenses/agpl-3.0)
 [![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)
 
@@ -82,8 +73,7 @@
   pip install pdm
   pdm sync
 ```
 
 ## 文档
 
 [文档](https://linktodocumentation)
-
```

