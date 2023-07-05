# Comparing `tmp/xata-1.0.0a1.tar.gz` & `tmp/xata-1.0.0a2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "xata-1.0.0a1.tar", max compression
+gzip compressed data, was "xata-1.0.0a2.tar", max compression
```

## Comparing `xata-1.0.0a1.tar` & `xata-1.0.0a2.tar`

### file list

```diff
@@ -1,22 +1,22 @@
--rw-r--r--   0        0        0    11357 2023-07-04 18:58:29.629796 xata-1.0.0a1/LICENSE
--rw-r--r--   0        0        0     1156 2023-07-04 18:58:29.633796 xata-1.0.0a1/README.md
--rw-r--r--   0        0        0      818 2023-07-04 18:58:29.657796 xata-1.0.0a1/pyproject.toml
--rw-r--r--   0        0        0      873 2023-07-04 18:58:29.689796 xata-1.0.0a1/xata/__init__.py
--rw-r--r--   0        0        0      769 2023-07-04 18:58:29.689796 xata-1.0.0a1/xata/api/__init__.py
--rw-r--r--   0        0        0     2681 2023-07-04 18:58:29.689796 xata-1.0.0a1/xata/api/authentication.py
--rw-r--r--   0        0        0    12341 2023-07-04 18:58:29.689796 xata-1.0.0a1/xata/api/branch.py
--rw-r--r--   0        0        0     7553 2023-07-04 18:58:29.689796 xata-1.0.0a1/xata/api/databases.py
--rw-r--r--   0        0        0     8958 2023-07-04 18:58:29.689796 xata-1.0.0a1/xata/api/files.py
--rw-r--r--   0        0        0     6083 2023-07-04 18:58:29.689796 xata-1.0.0a1/xata/api/invites.py
--rw-r--r--   0        0        0    11676 2023-07-04 18:58:29.689796 xata-1.0.0a1/xata/api/migrations.py
--rw-r--r--   0        0        0    12501 2023-07-04 18:58:29.689796 xata-1.0.0a1/xata/api/records.py
--rw-r--r--   0        0        0    31539 2023-07-04 18:58:29.689796 xata-1.0.0a1/xata/api/search_and_filter.py
--rw-r--r--   0        0        0    12238 2023-07-04 18:58:29.689796 xata-1.0.0a1/xata/api/table.py
--rw-r--r--   0        0        0     2532 2023-07-04 18:58:29.689796 xata-1.0.0a1/xata/api/users.py
--rw-r--r--   0        0        0     7314 2023-07-04 18:58:29.689796 xata-1.0.0a1/xata/api/workspaces.py
--rw-r--r--   0        0        0     2294 2023-07-04 18:58:29.689796 xata-1.0.0a1/xata/api_response.py
--rw-r--r--   0        0        0    13623 2023-07-04 18:58:29.689796 xata-1.0.0a1/xata/client.py
--rw-r--r--   0        0        0     1188 2023-07-04 18:58:29.689796 xata-1.0.0a1/xata/errors.py
--rw-r--r--   0        0        0    15888 2023-07-04 18:58:29.689796 xata-1.0.0a1/xata/helpers.py
--rw-r--r--   0        0        0     3076 2023-07-04 18:58:29.689796 xata-1.0.0a1/xata/namespace.py
--rw-r--r--   0        0        0     1869 1970-01-01 00:00:00.000000 xata-1.0.0a1/PKG-INFO
+-rw-r--r--   0        0        0    11357 2023-07-05 15:15:08.613422 xata-1.0.0a2/LICENSE
+-rw-r--r--   0        0        0     1156 2023-07-05 15:15:08.613422 xata-1.0.0a2/README.md
+-rw-r--r--   0        0        0      818 2023-07-05 15:15:08.637422 xata-1.0.0a2/pyproject.toml
+-rw-r--r--   0        0        0      873 2023-07-05 15:15:08.669422 xata-1.0.0a2/xata/__init__.py
+-rw-r--r--   0        0        0      769 2023-07-05 15:15:08.669422 xata-1.0.0a2/xata/api/__init__.py
+-rw-r--r--   0        0        0     2694 2023-07-05 15:15:08.673422 xata-1.0.0a2/xata/api/authentication.py
+-rw-r--r--   0        0        0    12385 2023-07-05 15:15:08.673422 xata-1.0.0a2/xata/api/branch.py
+-rw-r--r--   0        0        0     7577 2023-07-05 15:15:08.673422 xata-1.0.0a2/xata/api/databases.py
+-rw-r--r--   0        0        0     8958 2023-07-05 15:15:08.673422 xata-1.0.0a2/xata/api/files.py
+-rw-r--r--   0        0        0     6103 2023-07-05 15:15:08.673422 xata-1.0.0a2/xata/api/invites.py
+-rw-r--r--   0        0        0    11716 2023-07-05 15:15:08.673422 xata-1.0.0a2/xata/api/migrations.py
+-rw-r--r--   0        0        0    12533 2023-07-05 15:15:08.673422 xata-1.0.0a2/xata/api/records.py
+-rw-r--r--   0        0        0    31571 2023-07-05 15:15:08.673422 xata-1.0.0a2/xata/api/search_and_filter.py
+-rw-r--r--   0        0        0    12278 2023-07-05 15:15:08.673422 xata-1.0.0a2/xata/api/table.py
+-rw-r--r--   0        0        0     2544 2023-07-05 15:15:08.673422 xata-1.0.0a2/xata/api/users.py
+-rw-r--r--   0        0        0     7346 2023-07-05 15:15:08.673422 xata-1.0.0a2/xata/api/workspaces.py
+-rw-r--r--   0        0        0     2637 2023-07-05 15:15:08.673422 xata-1.0.0a2/xata/api_response.py
+-rw-r--r--   0        0        0    13637 2023-07-05 15:15:08.673422 xata-1.0.0a2/xata/client.py
+-rw-r--r--   0        0        0     1188 2023-07-05 15:15:08.673422 xata-1.0.0a2/xata/errors.py
+-rw-r--r--   0        0        0    15894 2023-07-05 15:15:08.673422 xata-1.0.0a2/xata/helpers.py
+-rw-r--r--   0        0        0     3077 2023-07-05 15:15:08.673422 xata-1.0.0a2/xata/namespace.py
+-rw-r--r--   0        0        0     1869 1970-01-01 00:00:00.000000 xata-1.0.0a2/PKG-INFO
```

### Comparing `xata-1.0.0a1/LICENSE` & `xata-1.0.0a2/LICENSE`

 * *Files identical despite different names*

### Comparing `xata-1.0.0a1/README.md` & `xata-1.0.0a2/README.md`

 * *Files identical despite different names*

### Comparing `xata-1.0.0a1/pyproject.toml` & `xata-1.0.0a2/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "xata"
-version = "1.0.0a1"
+version = "1.0.0a2"
 description = "Python client for Xata.io"
 authors = ["Xata <support@xata.io>"]
 license = "Apache-2.0"
 readme = "README.md"
 documentation = "https://xata-py.readthedocs.io"
 
 [tool.poetry.dependencies]
```

### Comparing `xata-1.0.0a1/xata/__init__.py` & `xata-1.0.0a2/xata/__init__.py`

 * *Files identical despite different names*

### Comparing `xata-1.0.0a1/xata/api/__init__.py` & `xata-1.0.0a2/xata/api/__init__.py`

 * *Files identical despite different names*

### Comparing `xata-1.0.0a1/xata/api/authentication.py` & `xata-1.0.0a2/xata/api/authentication.py`

 * *Files 6% similar despite different names*

```diff
@@ -41,15 +41,16 @@
         - 200: OK
         - 400: Bad Request
         - 401: Authentication Error
         - 404: Example response
         - 5XX: Unexpected Error
         Response: application/json
 
-        :return Response
+
+        :returns ApiResponse
         """
         url_path = "/user/keys"
         return self.request("GET", url_path)
 
     def create_user_api_keys(self, key_name: str) -> ApiResponse:
         """
         Create and return new API key
@@ -62,15 +63,15 @@
         - 401: Authentication Error
         - 404: Example response
         - 5XX: Unexpected Error
         Response: application/json
 
         :param key_name: str API Key name
 
-        :return Response
+        :returns ApiResponse
         """
         url_path = f"/user/keys/{key_name}"
         return self.request("POST", url_path)
 
     def delete_user_api_keys(self, key_name: str) -> ApiResponse:
         """
         Delete an existing API key
@@ -82,11 +83,11 @@
         - 400: Bad Request
         - 401: Authentication Error
         - 404: Example response
         - 5XX: Unexpected Error
 
         :param key_name: str API Key name
 
-        :return Response
+        :returns ApiResponse
         """
         url_path = f"/user/keys/{key_name}"
         return self.request("DELETE", url_path)
```

### Comparing `xata-1.0.0a1/xata/api/branch.py` & `xata-1.0.0a2/xata/api/branch.py`

 * *Files 4% similar despite different names*

```diff
@@ -43,15 +43,15 @@
         - 401: Authentication Error
         - 404: Example response
         - 5XX: Unexpected Error
         Response: application/json
 
         :param db_name: str The Database Name
 
-        :return Response
+        :returns ApiResponse
         """
         url_path = f"/dbs/{db_name}"
         return self.request("GET", url_path)
 
     def get_details(self, db_name: str = None, branch_name: str = None) -> ApiResponse:
         """
         Get branch schema and metadata
@@ -65,21 +65,21 @@
         - 404: Example response
         - 5XX: Unexpected Error
         Response: application/json
 
         :param db_name: str = None The name of the database to query. Default: database name from the client.
         :param branch_name: str = None The name of the branch to query. Default: branch name from the client.
 
-        :return Response
+        :returns ApiResponse
         """
         db_branch_name = self.client.get_db_branch_name(db_name, branch_name)
         url_path = f"/db/{db_branch_name}"
         return self.request("GET", url_path)
 
-    def create(self, payload: dict, db_name: str = None, branch_name: str = None, _from: str = None) -> ApiResponse:
+    def create(self, payload: dict, db_name: str = None, branch_name: str = None, from_: str = None) -> ApiResponse:
         """
         Create Database branch
 
         Path: /db/{db_branch_name}
         Method: PUT
         Response status codes:
         - 201: Created
@@ -89,22 +89,22 @@
         - 423: Example response
         - 5XX: Unexpected Error
         Response: application/json
 
         :param payload: dict content
         :param db_name: str = None The name of the database to query. Default: database name from the client.
         :param branch_name: str = None The name of the branch to query. Default: branch name from the client.
-        :param _from: str = None Name of source branch to branch the new schema from
+        :param from_: str = None Name of source branch to branch the new schema from
 
-        :return Response
+        :returns ApiResponse
         """
         db_branch_name = self.client.get_db_branch_name(db_name, branch_name)
         url_path = f"/db/{db_branch_name}"
-        if _from is not None:
-            url_path += "?from={_from}"
+        if from_ is not None:
+            url_path += "?from={from_}"
         headers = {"content-type": "application/json"}
         return self.request("PUT", url_path, headers, payload)
 
     def delete(self, db_name: str = None, branch_name: str = None) -> ApiResponse:
         """
         Delete the branch in the database and all its resources
 
@@ -118,15 +118,15 @@
         - 409: Example response
         - 5XX: Unexpected Error
         Response: application/json
 
         :param db_name: str = None The name of the database to query. Default: database name from the client.
         :param branch_name: str = None The name of the branch to query. Default: branch name from the client.
 
-        :return Response
+        :returns ApiResponse
         """
         db_branch_name = self.client.get_db_branch_name(db_name, branch_name)
         url_path = f"/db/{db_branch_name}"
         return self.request("DELETE", url_path)
 
     def get_metadata(self, db_name: str = None, branch_name: str = None) -> ApiResponse:
         """
@@ -141,15 +141,15 @@
         - 404: Example response
         - 5XX: Unexpected Error
         Response: application/json
 
         :param db_name: str = None The name of the database to query. Default: database name from the client.
         :param branch_name: str = None The name of the branch to query. Default: branch name from the client.
 
-        :return Response
+        :returns ApiResponse
         """
         db_branch_name = self.client.get_db_branch_name(db_name, branch_name)
         url_path = f"/db/{db_branch_name}/metadata"
         return self.request("GET", url_path)
 
     def update_metadata(self, payload: dict, db_name: str = None, branch_name: str = None) -> ApiResponse:
         """
@@ -164,15 +164,15 @@
         - 404: Example response
         - 5XX: Unexpected Error
 
         :param payload: dict content
         :param db_name: str = None The name of the database to query. Default: database name from the client.
         :param branch_name: str = None The name of the branch to query. Default: branch name from the client.
 
-        :return Response
+        :returns ApiResponse
         """
         db_branch_name = self.client.get_db_branch_name(db_name, branch_name)
         url_path = f"/db/{db_branch_name}/metadata"
         headers = {"content-type": "application/json"}
         return self.request("PUT", url_path, headers, payload)
 
     def get_stats(self, db_name: str = None, branch_name: str = None) -> ApiResponse:
@@ -188,15 +188,15 @@
         - 404: Example response
         - 5XX: Unexpected Error
         Response: application/json
 
         :param db_name: str = None The name of the database to query. Default: database name from the client.
         :param branch_name: str = None The name of the branch to query. Default: branch name from the client.
 
-        :return Response
+        :returns ApiResponse
         """
         db_branch_name = self.client.get_db_branch_name(db_name, branch_name)
         url_path = f"/db/{db_branch_name}/stats"
         return self.request("GET", url_path)
 
     def get_git_branches_mapping(self, db_name: str) -> ApiResponse:
         """
@@ -213,15 +213,15 @@
         - 400: Bad Request
         - 401: Authentication Error
         - 5XX: Unexpected Error
         Response: application/json
 
         :param db_name: str The Database Name
 
-        :return Response
+        :returns ApiResponse
         """
         url_path = f"/dbs/{db_name}/gitBranches"
         return self.request("GET", url_path)
 
     def add_git_branches_entry(self, db_name: str, payload: dict) -> ApiResponse:
         """
         Adds an entry to the mapping of git branches to Xata branches.  The git branch and the
@@ -242,15 +242,15 @@
         - 401: Authentication Error
         - 5XX: Unexpected Error
         Response: application/json
 
         :param db_name: str The Database Name
         :param payload: dict content
 
-        :return Response
+        :returns ApiResponse
         """
         url_path = f"/dbs/{db_name}/gitBranches"
         headers = {"content-type": "application/json"}
         return self.request("POST", url_path, headers, payload)
 
     def remove_git_branches_entry(self, db_name: str, git_branch: str) -> ApiResponse:
         """
@@ -267,15 +267,15 @@
         - 401: Authentication Error
         - 404: The git branch was not found in the mapping
         - 5XX: Unexpected Error
 
         :param db_name: str The Database Name
         :param git_branch: str The Git Branch to remove from the mapping
 
-        :return Response
+        :returns ApiResponse
         """
         url_path = f"/dbs/{db_name}/gitBranches"
         if git_branch is not None:
             url_path += "?gitBranch={git_branch}"
         return self.request("DELETE", url_path)
 
     def resolve(self, db_name: str, git_branch: str = None, fallback_branch: str = None) -> ApiResponse:
@@ -300,15 +300,15 @@
         - 5XX: Unexpected Error
         Response: application/json
 
         :param db_name: str The Database Name
         :param git_branch: str = None The Git Branch
         :param fallback_branch: str = None Default branch to fallback to
 
-        :return Response
+        :returns ApiResponse
         """
         url_path = f"/dbs/{db_name}/resolveBranch"
         query_params = []
         if git_branch is not None:
             query_params.append(f"gitBranch={git_branch}")
         if fallback_branch is not None:
             query_params.append(f"fallbackBranch={fallback_branch}")
```

### Comparing `xata-1.0.0a1/xata/api/databases.py` & `xata-1.0.0a2/xata/api/databases.py`

 * *Files 8% similar despite different names*

```diff
@@ -42,15 +42,15 @@
         - 400: Bad Request
         - 401: Authentication Error
         - 5XX: Unexpected Error
         Response: application/json
 
         :param workspace_id: str = None The workspace identifier. Default: workspace Id from the client.
 
-        :return Response
+        :returns ApiResponse
         """
         if workspace_id is None:
             workspace_id = self.client.get_workspace_id()
         url_path = f"/workspaces/{workspace_id}/dbs"
         return self.request("GET", url_path)
 
     def get_metadata(self, db_name: str, workspace_id: str = None) -> ApiResponse:
@@ -66,15 +66,15 @@
         - 404: Example response
         - 5XX: Unexpected Error
         Response: application/json
 
         :param db_name: str The Database Name
         :param workspace_id: str = None The workspace identifier. Default: workspace Id from the client.
 
-        :return Response
+        :returns ApiResponse
         """
         if workspace_id is None:
             workspace_id = self.client.get_workspace_id()
         url_path = f"/workspaces/{workspace_id}/dbs/{db_name}"
         return self.request("GET", url_path)
 
     def create(
@@ -124,15 +124,15 @@
         - 404: Example response
         - 5XX: Unexpected Error
         Response: application/json
 
         :param db_name: str The Database Name
         :param workspace_id: str = None The workspace identifier. Default: workspace Id from the client.
 
-        :return Response
+        :returns ApiResponse
         """
         if workspace_id is None:
             workspace_id = self.client.get_workspace_id()
         url_path = f"/workspaces/{workspace_id}/dbs/{db_name}"
         return self.request("DELETE", url_path)
 
     def update_metadata(self, db_name: str, payload: dict, workspace_id: str = None) -> ApiResponse:
@@ -149,15 +149,15 @@
         - 5XX: Unexpected Error
         Response: application/json
 
         :param db_name: str The Database Name
         :param payload: dict content
         :param workspace_id: str = None The workspace identifier. Default: workspace Id from the client.
 
-        :return Response
+        :returns ApiResponse
         """
         if workspace_id is None:
             workspace_id = self.client.get_workspace_id()
         url_path = f"/workspaces/{workspace_id}/dbs/{db_name}"
         headers = {"content-type": "application/json"}
         return self.request("PATCH", url_path, headers, payload)
 
@@ -176,15 +176,15 @@
         - 5XX: Unexpected Error
         Response: application/json
 
         :param db_name: str The Database Name
         :param payload: dict content
         :param workspace_id: str = None The workspace identifier. Default: workspace Id from the client.
 
-        :return Response
+        :returns ApiResponse
         """
         if workspace_id is None:
             workspace_id = self.client.get_workspace_id()
         url_path = f"/workspaces/{workspace_id}/dbs/{db_name}/rename"
         headers = {"content-type": "application/json"}
         return self.request("POST", url_path, headers, payload)
 
@@ -199,13 +199,13 @@
         - 400: Bad Request
         - 401: Authentication Error
         - 5XX: Unexpected Error
         Response: application/json
 
         :param workspace_id: str = None The workspace identifier. Default: workspace Id from the client.
 
-        :return Response
+        :returns ApiResponse
         """
         if workspace_id is None:
             workspace_id = self.client.get_workspace_id()
         url_path = f"/workspaces/{workspace_id}/regions"
         return self.request("GET", url_path)
```

### Comparing `xata-1.0.0a1/xata/api/files.py` & `xata-1.0.0a2/xata/api/files.py`

 * *Files identical despite different names*

### Comparing `xata-1.0.0a1/xata/api/invites.py` & `xata-1.0.0a2/xata/api/invites.py`

 * *Files 5% similar despite different names*

```diff
@@ -46,15 +46,15 @@
         - 409: Example response
         - 5XX: Unexpected Error
         Response: application/json
 
         :param payload: dict content
         :param workspace_id: str = None The workspace identifier. Default: workspace Id from the client.
 
-        :return Response
+        :returns ApiResponse
         """
         if workspace_id is None:
             workspace_id = self.client.get_workspace_id()
         url_path = f"/workspaces/{workspace_id}/invites"
         headers = {"content-type": "application/json"}
         return self.request("POST", url_path, headers, payload)
 
@@ -72,15 +72,15 @@
         - 403: Authentication Error
         - 404: Example response
         - 5XX: Unexpected Error
 
         :param invite_id: str Invite identifier
         :param workspace_id: str = None The workspace identifier. Default: workspace Id from the client.
 
-        :return Response
+        :returns ApiResponse
         """
         if workspace_id is None:
             workspace_id = self.client.get_workspace_id()
         url_path = f"/workspaces/{workspace_id}/invites/{invite_id}"
         return self.request("DELETE", url_path)
 
     def update(self, invite_id: str, payload: dict, workspace_id: str = None) -> ApiResponse:
@@ -101,15 +101,15 @@
         - 5XX: Unexpected Error
         Response: application/json
 
         :param invite_id: str Invite identifier
         :param payload: dict content
         :param workspace_id: str = None The workspace identifier. Default: workspace Id from the client.
 
-        :return Response
+        :returns ApiResponse
         """
         if workspace_id is None:
             workspace_id = self.client.get_workspace_id()
         url_path = f"/workspaces/{workspace_id}/invites/{invite_id}"
         headers = {"content-type": "application/json"}
         return self.request("PATCH", url_path, headers, payload)
 
@@ -127,15 +127,15 @@
         - 403: Authentication Error
         - 404: Example response
         - 5XX: Unexpected Error
 
         :param invite_key: str Invite Key (secret) for the invited user
         :param workspace_id: str = None The workspace identifier. Default: workspace Id from the client.
 
-        :return Response
+        :returns ApiResponse
         """
         if workspace_id is None:
             workspace_id = self.client.get_workspace_id()
         url_path = f"/workspaces/{workspace_id}/invites/{invite_key}/accept"
         return self.request("POST", url_path)
 
     def resend(self, invite_id: str, workspace_id: str = None) -> ApiResponse:
@@ -152,13 +152,13 @@
         - 403: Authentication Error
         - 404: Example response
         - 5XX: Unexpected Error
 
         :param invite_id: str Invite identifier
         :param workspace_id: str = None The workspace identifier. Default: workspace Id from the client.
 
-        :return Response
+        :returns ApiResponse
         """
         if workspace_id is None:
             workspace_id = self.client.get_workspace_id()
         url_path = f"/workspaces/{workspace_id}/invites/{invite_id}/resend"
         return self.request("POST", url_path)
```

### Comparing `xata-1.0.0a1/xata/api/migrations.py` & `xata-1.0.0a2/xata/api/migrations.py`

 * *Files 2% similar despite different names*

```diff
@@ -45,15 +45,15 @@
         - 5XX: Unexpected Error
         Response: application/json
 
         :param payload: dict content
         :param db_name: str = None The name of the database to query. Default: database name from the client.
         :param branch_name: str = None The name of the branch to query. Default: branch name from the client.
 
-        :return Response
+        :returns ApiResponse
         """
         db_branch_name = self.client.get_db_branch_name(db_name, branch_name)
         url_path = f"/db/{db_branch_name}/migrations"
         headers = {"content-type": "application/json"}
         return self.request("GET", url_path, headers, payload)
 
     def get_plan(self, payload: dict, db_name: str = None, branch_name: str = None) -> ApiResponse:
@@ -69,15 +69,15 @@
         - 404: Example response
         - 5XX: Unexpected Error
 
         :param payload: dict content
         :param db_name: str = None The name of the database to query. Default: database name from the client.
         :param branch_name: str = None The name of the branch to query. Default: branch name from the client.
 
-        :return Response
+        :returns ApiResponse
         """
         db_branch_name = self.client.get_db_branch_name(db_name, branch_name)
         url_path = f"/db/{db_branch_name}/migrations/plan"
         headers = {"content-type": "application/json"}
         return self.request("POST", url_path, headers, payload)
 
     def execute_plan(self, payload: dict, db_name: str = None, branch_name: str = None) -> ApiResponse:
@@ -93,15 +93,15 @@
         - 404: Example response
         - 5XX: Unexpected Error
 
         :param payload: dict content
         :param db_name: str = None The name of the database to query. Default: database name from the client.
         :param branch_name: str = None The name of the branch to query. Default: branch name from the client.
 
-        :return Response
+        :returns ApiResponse
         """
         db_branch_name = self.client.get_db_branch_name(db_name, branch_name)
         url_path = f"/db/{db_branch_name}/migrations/execute"
         headers = {"content-type": "application/json"}
         return self.request("POST", url_path, headers, payload)
 
     def get_schema_history(self, payload: dict, db_name: str = None, branch_name: str = None) -> ApiResponse:
@@ -118,15 +118,15 @@
         - 5XX: Unexpected Error
         Response: application/json
 
         :param payload: dict content
         :param db_name: str = None The name of the database to query. Default: database name from the client.
         :param branch_name: str = None The name of the branch to query. Default: branch name from the client.
 
-        :return Response
+        :returns ApiResponse
         """
         db_branch_name = self.client.get_db_branch_name(db_name, branch_name)
         url_path = f"/db/{db_branch_name}/schema/history"
         headers = {"content-type": "application/json"}
         return self.request("POST", url_path, headers, payload)
 
     def compare_branch_with_user_schema(
@@ -144,15 +144,15 @@
         - 404: Example response
         - 5XX: Unexpected Error
 
         :param payload: dict content
         :param db_name: str = None The name of the database to query. Default: database name from the client.
         :param branch_name: str = None The name of the branch to query. Default: branch name from the client.
 
-        :return Response
+        :returns ApiResponse
         """
         db_branch_name = self.client.get_db_branch_name(db_name, branch_name)
         url_path = f"/db/{db_branch_name}/schema/compare"
         headers = {"content-type": "application/json"}
         return self.request("POST", url_path, headers, payload)
 
     def compare_schemas(self, payload: dict, db_name: str = None, branch_name: str = None) -> ApiResponse:
@@ -168,15 +168,15 @@
         - 404: Example response
         - 5XX: Unexpected Error
 
         :param payload: dict content
         :param db_name: str = None The name of the database to query. Default: database name from the client.
         :param branch_name: str = None The name of the branch to query. Default: branch name from the client.
 
-        :return Response
+        :returns ApiResponse
         """
         db_branch_name = self.client.get_db_branch_name(db_name, branch_name)
         url_path = f"/db/{db_branch_name}/schema/compare/{branch_name}"
         headers = {"content-type": "application/json"}
         return self.request("POST", url_path, headers, payload)
 
     def upadte_schema(self, payload: dict, db_name: str = None, branch_name: str = None) -> ApiResponse:
@@ -192,15 +192,15 @@
         - 404: Example response
         - 5XX: Unexpected Error
 
         :param payload: dict content
         :param db_name: str = None The name of the database to query. Default: database name from the client.
         :param branch_name: str = None The name of the branch to query. Default: branch name from the client.
 
-        :return Response
+        :returns ApiResponse
         """
         db_branch_name = self.client.get_db_branch_name(db_name, branch_name)
         url_path = f"/db/{db_branch_name}/schema/update"
         headers = {"content-type": "application/json"}
         return self.request("POST", url_path, headers, payload)
 
     def preview(self, payload: dict, db_name: str = None, branch_name: str = None) -> ApiResponse:
@@ -217,15 +217,15 @@
         - 5XX: Unexpected Error
         Response: application/json
 
         :param payload: dict content
         :param db_name: str = None The name of the database to query. Default: database name from the client.
         :param branch_name: str = None The name of the branch to query. Default: branch name from the client.
 
-        :return Response
+        :returns ApiResponse
         """
         db_branch_name = self.client.get_db_branch_name(db_name, branch_name)
         url_path = f"/db/{db_branch_name}/schema/preview"
         headers = {"content-type": "application/json"}
         return self.request("POST", url_path, headers, payload)
 
     def apply(self, payload: dict, db_name: str = None, branch_name: str = None) -> ApiResponse:
@@ -241,15 +241,15 @@
         - 404: Example response
         - 5XX: Unexpected Error
 
         :param payload: dict content
         :param db_name: str = None The name of the database to query. Default: database name from the client.
         :param branch_name: str = None The name of the branch to query. Default: branch name from the client.
 
-        :return Response
+        :returns ApiResponse
         """
         db_branch_name = self.client.get_db_branch_name(db_name, branch_name)
         url_path = f"/db/{db_branch_name}/schema/apply"
         headers = {"content-type": "application/json"}
         return self.request("POST", url_path, headers, payload)
 
     def push(self, payload: dict, db_name: str = None, branch_name: str = None) -> ApiResponse:
@@ -271,13 +271,13 @@
         - 404: Example response
         - 5XX: Unexpected Error
 
         :param payload: dict content
         :param db_name: str = None The name of the database to query. Default: database name from the client.
         :param branch_name: str = None The name of the branch to query. Default: branch name from the client.
 
-        :return Response
+        :returns ApiResponse
         """
         db_branch_name = self.client.get_db_branch_name(db_name, branch_name)
         url_path = f"/db/{db_branch_name}/schema/push"
         headers = {"content-type": "application/json"}
         return self.request("POST", url_path, headers, payload)
```

### Comparing `xata-1.0.0a1/xata/api/records.py` & `xata-1.0.0a2/xata/api/records.py`

 * *Files 1% similar despite different names*

```diff
@@ -45,15 +45,15 @@
         - 5XX: Unexpected Error
         Response: application/json
 
         :param payload: dict content
         :param db_name: str = None The name of the database to query. Default: database name from the client.
         :param branch_name: str = None The name of the branch to query. Default: branch name from the client.
 
-        :return Response
+        :returns ApiResponse
         """
         db_branch_name = self.client.get_db_branch_name(db_name, branch_name)
         url_path = f"/db/{db_branch_name}/transaction"
         headers = {"content-type": "application/json"}
         return self.request("POST", url_path, headers, payload)
 
     def insert(
@@ -73,15 +73,15 @@
 
         :param table_name: str The Table name
         :param payload: dict content
         :param db_name: str = None The name of the database to query. Default: database name from the client.
         :param branch_name: str = None The name of the branch to query. Default: branch name from the client.
         :param columns: list = None Column filters
 
-        :return Response
+        :returns ApiResponse
         """
         db_branch_name = self.client.get_db_branch_name(db_name, branch_name)
         url_path = f"/db/{db_branch_name}/tables/{table_name}/data"
         if columns is not None:
             url_path += "?columns=%s" % ",".join(columns)
         headers = {"content-type": "application/json"}
         return self.request("POST", url_path, headers, payload)
@@ -103,15 +103,15 @@
 
         :param table_name: str The Table name
         :param record_id: str The Record name
         :param db_name: str = None The name of the database to query. Default: database name from the client.
         :param branch_name: str = None The name of the branch to query. Default: branch name from the client.
         :param columns: list = None Column filters
 
-        :return Response
+        :returns ApiResponse
         """
         db_branch_name = self.client.get_db_branch_name(db_name, branch_name)
         url_path = f"/db/{db_branch_name}/tables/{table_name}/data/{record_id}"
         if columns is not None:
             url_path += "?columns=%s" % ",".join(columns)
         return self.request("GET", url_path)
 
@@ -147,15 +147,15 @@
         :param payload: dict content
         :param db_name: str = None The name of the database to query. Default: database name from the client.
         :param branch_name: str = None The name of the branch to query. Default: branch name from the client.
         :param columns: list = None Column filters
         :param create_only: bool = None
         :param if_version: int = None
 
-        :return Response
+        :returns ApiResponse
         """
         db_branch_name = self.client.get_db_branch_name(db_name, branch_name)
         url_path = f"/db/{db_branch_name}/tables/{table_name}/data/{record_id}"
         query_params = []
         if columns is not None:
             query_params.append("columns=%s" % ",".join(columns))
         if create_only is not None:
@@ -195,15 +195,15 @@
         :param record_id: str The Record name
         :param payload: dict content
         :param db_name: str = None The name of the database to query. Default: database name from the client.
         :param branch_name: str = None The name of the branch to query. Default: branch name from the client.
         :param columns: list = None Column filters
         :param if_version: int = None
 
-        :return Response
+        :returns ApiResponse
         """
         db_branch_name = self.client.get_db_branch_name(db_name, branch_name)
         url_path = f"/db/{db_branch_name}/tables/{table_name}/data/{record_id}"
         query_params = []
         if columns is not None:
             query_params.append("columns=%s" % ",".join(columns))
         if if_version is not None:
@@ -231,15 +231,15 @@
 
         :param table_name: str The Table name
         :param record_id: str The Record name
         :param db_name: str = None The name of the database to query. Default: database name from the client.
         :param branch_name: str = None The name of the branch to query. Default: branch name from the client.
         :param columns: list = None Column filters
 
-        :return Response
+        :returns ApiResponse
         """
         db_branch_name = self.client.get_db_branch_name(db_name, branch_name)
         url_path = f"/db/{db_branch_name}/tables/{table_name}/data/{record_id}"
         if columns is not None:
             url_path += "?columns=%s" % ",".join(columns)
         return self.request("DELETE", url_path)
 
@@ -270,15 +270,15 @@
         :param record_id: str The Record name
         :param payload: dict content
         :param db_name: str = None The name of the database to query. Default: database name from the client.
         :param branch_name: str = None The name of the branch to query. Default: branch name from the client.
         :param columns: list = None Column filters
         :param if_version: int = None
 
-        :return Response
+        :returns ApiResponse
         """
         db_branch_name = self.client.get_db_branch_name(db_name, branch_name)
         url_path = f"/db/{db_branch_name}/tables/{table_name}/data/{record_id}"
         query_params = []
         if columns is not None:
             query_params.append("columns=%s" % ",".join(columns))
         if if_version is not None:
@@ -306,15 +306,15 @@
 
         :param table_name: str The Table name
         :param payload: dict content
         :param db_name: str = None The name of the database to query. Default: database name from the client.
         :param branch_name: str = None The name of the branch to query. Default: branch name from the client.
         :param columns: list = None Column filters
 
-        :return Response
+        :returns ApiResponse
         """
         db_branch_name = self.client.get_db_branch_name(db_name, branch_name)
         url_path = f"/db/{db_branch_name}/tables/{table_name}/bulk"
         if columns is not None:
             url_path += "?columns=%s" % ",".join(columns)
         headers = {"content-type": "application/json"}
         return self.request("POST", url_path, headers, payload)
```

### Comparing `xata-1.0.0a1/xata/api/search_and_filter.py` & `xata-1.0.0a2/xata/api/search_and_filter.py`

 * *Files 2% similar despite different names*

```diff
@@ -223,15 +223,15 @@
         - 5XX: Unexpected Error
 
         :param table_name: str The Table name
         :param payload: dict content
         :param db_name: str = None The name of the database to query. Default: database name from the client.
         :param branch_name: str = None The name of the branch to query. Default: branch name from the client.
 
-        :return Response
+        :returns ApiResponse
         """
         db_branch_name = self.client.get_db_branch_name(db_name, branch_name)
         url_path = f"/db/{db_branch_name}/tables/{table_name}/query"
         headers = {"content-type": "application/json"}
         return self.request("POST", url_path, headers, payload)
 
     def search_branch(self, payload: dict, db_name: str = None, branch_name: str = None) -> ApiResponse:
@@ -248,15 +248,15 @@
         - 503: ServiceUnavailable
         - 5XX: Unexpected Error
 
         :param payload: dict content
         :param db_name: str = None The name of the database to query. Default: database name from the client.
         :param branch_name: str = None The name of the branch to query. Default: branch name from the client.
 
-        :return Response
+        :returns ApiResponse
         """
         db_branch_name = self.client.get_db_branch_name(db_name, branch_name)
         url_path = f"/db/{db_branch_name}/search"
         headers = {"content-type": "application/json"}
         return self.request("POST", url_path, headers, payload)
 
     def search_table(self, table_name: str, payload: dict, db_name: str = None, branch_name: str = None) -> ApiResponse:
@@ -279,15 +279,15 @@
         - 5XX: Unexpected Error
 
         :param table_name: str The Table name
         :param payload: dict content
         :param db_name: str = None The name of the database to query. Default: database name from the client.
         :param branch_name: str = None The name of the branch to query. Default: branch name from the client.
 
-        :return Response
+        :returns ApiResponse
         """
         db_branch_name = self.client.get_db_branch_name(db_name, branch_name)
         url_path = f"/db/{db_branch_name}/tables/{table_name}/search"
         headers = {"content-type": "application/json"}
         return self.request("POST", url_path, headers, payload)
 
     def vector_search(
@@ -309,15 +309,15 @@
         - 5XX: Unexpected Error
 
         :param table_name: str The Table name
         :param payload: dict content
         :param db_name: str = None The name of the database to query. Default: database name from the client.
         :param branch_name: str = None The name of the branch to query. Default: branch name from the client.
 
-        :return Response
+        :returns ApiResponse
         """
         db_branch_name = self.client.get_db_branch_name(db_name, branch_name)
         url_path = f"/db/{db_branch_name}/tables/{table_name}/vectorSearch"
         headers = {"content-type": "application/json"}
         return self.request("POST", url_path, headers, payload)
 
     def ask(
@@ -348,15 +348,15 @@
 
         :param table_name: str The Table name
         :param payload: dict content
         :param db_name: str = None The name of the database to query. Default: database name from the client.
         :param branch_name: str = None The name of the branch to query. Default: branch name from the client.
         :param response_content_type: str = "application/json" Content type of the response. Default: application/json
 
-        :return Response
+        :returns ApiResponse
         """
         db_branch_name = self.client.get_db_branch_name(db_name, branch_name)
         url_path = f"/db/{db_branch_name}/tables/{table_name}/ask"
         headers = {
             "content-type": "application/json",
             "accept": response_content_type,
         }
@@ -383,15 +383,15 @@
 
         :param table_name: str The Table name
         :param session_id: str
         :param payload: dict content
         :param db_name: str = None The name of the database to query. Default: database name from the client.
         :param branch_name: str = None The name of the branch to query. Default: branch name from the client.
 
-        :return Response
+        :returns ApiResponse
         """
         db_branch_name = self.client.get_db_branch_name(db_name, branch_name)
         url_path = f"/db/{db_branch_name}/tables/{table_name}/ask/{session_id}"
         headers = {"content-type": "application/json"}
         return self.request("POST", url_path, headers, payload)
 
     def summarize(self, table_name: str, payload: dict, db_name: str = None, branch_name: str = None) -> ApiResponse:
@@ -440,15 +440,15 @@
         - 5XX: Unexpected Error
 
         :param table_name: str The Table name
         :param payload: dict content
         :param db_name: str = None The name of the database to query. Default: database name from the client.
         :param branch_name: str = None The name of the branch to query. Default: branch name from the client.
 
-        :return Response
+        :returns ApiResponse
         """
         db_branch_name = self.client.get_db_branch_name(db_name, branch_name)
         url_path = f"/db/{db_branch_name}/tables/{table_name}/summarize"
         headers = {"content-type": "application/json"}
         return self.request("POST", url_path, headers, payload)
 
     def aggregate(self, table_name: str, payload: dict, db_name: str = None, branch_name: str = None) -> ApiResponse:
@@ -471,13 +471,13 @@
         - 5XX: Unexpected Error
 
         :param table_name: str The Table name
         :param payload: dict content
         :param db_name: str = None The name of the database to query. Default: database name from the client.
         :param branch_name: str = None The name of the branch to query. Default: branch name from the client.
 
-        :return Response
+        :returns ApiResponse
         """
         db_branch_name = self.client.get_db_branch_name(db_name, branch_name)
         url_path = f"/db/{db_branch_name}/tables/{table_name}/aggregate"
         headers = {"content-type": "application/json"}
         return self.request("POST", url_path, headers, payload)
```

### Comparing `xata-1.0.0a1/xata/api/table.py` & `xata-1.0.0a2/xata/api/table.py`

 * *Files 2% similar despite different names*

```diff
@@ -48,15 +48,15 @@
         - 5XX: Unexpected Error
         Response: application/json
 
         :param table_name: str The Table name
         :param db_name: str = None The name of the database to query. Default: database name from the client.
         :param branch_name: str = None The name of the branch to query. Default: branch name from the client.
 
-        :return Response
+        :returns ApiResponse
         """
         db_branch_name = self.client.get_db_branch_name(db_name, branch_name)
         url_path = f"/db/{db_branch_name}/tables/{table_name}"
         return self.request("PUT", url_path)
 
     def delete(self, table_name: str, db_name: str = None, branch_name: str = None) -> ApiResponse:
         """
@@ -72,15 +72,15 @@
         - 5XX: Unexpected Error
         Response: application/json
 
         :param table_name: str The Table name
         :param db_name: str = None The name of the database to query. Default: database name from the client.
         :param branch_name: str = None The name of the branch to query. Default: branch name from the client.
 
-        :return Response
+        :returns ApiResponse
         """
         db_branch_name = self.client.get_db_branch_name(db_name, branch_name)
         url_path = f"/db/{db_branch_name}/tables/{table_name}"
         return self.request("DELETE", url_path)
 
     def update(self, table_name: str, payload: dict, db_name: str = None, branch_name: str = None) -> ApiResponse:
         """
@@ -99,15 +99,15 @@
         - 5XX: Unexpected Error
 
         :param table_name: str The Table name
         :param payload: dict content
         :param db_name: str = None The name of the database to query. Default: database name from the client.
         :param branch_name: str = None The name of the branch to query. Default: branch name from the client.
 
-        :return Response
+        :returns ApiResponse
         """
         db_branch_name = self.client.get_db_branch_name(db_name, branch_name)
         url_path = f"/db/{db_branch_name}/tables/{table_name}"
         headers = {"content-type": "application/json"}
         return self.request("PATCH", url_path, headers, payload)
 
     def get_schema(self, table_name: str, db_name: str = None, branch_name: str = None) -> ApiResponse:
@@ -124,15 +124,15 @@
         - 5XX: Unexpected Error
         Response: application/json
 
         :param table_name: str The Table name
         :param db_name: str = None The name of the database to query. Default: database name from the client.
         :param branch_name: str = None The name of the branch to query. Default: branch name from the client.
 
-        :return Response
+        :returns ApiResponse
         """
         db_branch_name = self.client.get_db_branch_name(db_name, branch_name)
         url_path = f"/db/{db_branch_name}/tables/{table_name}/schema"
         return self.request("GET", url_path)
 
     def set_schema(self, table_name: str, payload: dict, db_name: str = None, branch_name: str = None) -> ApiResponse:
         """
@@ -150,15 +150,15 @@
         - 5XX: Unexpected Error
 
         :param table_name: str The Table name
         :param payload: dict content
         :param db_name: str = None The name of the database to query. Default: database name from the client.
         :param branch_name: str = None The name of the branch to query. Default: branch name from the client.
 
-        :return Response
+        :returns ApiResponse
         """
         db_branch_name = self.client.get_db_branch_name(db_name, branch_name)
         url_path = f"/db/{db_branch_name}/tables/{table_name}/schema"
         headers = {"content-type": "application/json"}
         return self.request("PUT", url_path, headers, payload)
 
     def get_columns(self, table_name: str, db_name: str = None, branch_name: str = None) -> ApiResponse:
@@ -177,15 +177,15 @@
         - 5XX: Unexpected Error
         Response: application/json
 
         :param table_name: str The Table name
         :param db_name: str = None The name of the database to query. Default: database name from the client.
         :param branch_name: str = None The name of the branch to query. Default: branch name from the client.
 
-        :return Response
+        :returns ApiResponse
         """
         db_branch_name = self.client.get_db_branch_name(db_name, branch_name)
         url_path = f"/db/{db_branch_name}/tables/{table_name}/columns"
         return self.request("GET", url_path)
 
     def add_column(self, table_name: str, payload: dict, db_name: str = None, branch_name: str = None) -> ApiResponse:
         """
@@ -202,15 +202,15 @@
         - 5XX: Unexpected Error
 
         :param table_name: str The Table name
         :param payload: dict content
         :param db_name: str = None The name of the database to query. Default: database name from the client.
         :param branch_name: str = None The name of the branch to query. Default: branch name from the client.
 
-        :return Response
+        :returns ApiResponse
         """
         db_branch_name = self.client.get_db_branch_name(db_name, branch_name)
         url_path = f"/db/{db_branch_name}/tables/{table_name}/columns"
         headers = {"content-type": "application/json"}
         return self.request("POST", url_path, headers, payload)
 
     def get_column(
@@ -230,15 +230,15 @@
         Response: application/json
 
         :param table_name: str The Table name
         :param column_name: str The Column name
         :param db_name: str = None The name of the database to query. Default: database name from the client.
         :param branch_name: str = None The name of the branch to query. Default: branch name from the client.
 
-        :return Response
+        :returns ApiResponse
         """
         db_branch_name = self.client.get_db_branch_name(db_name, branch_name)
         url_path = f"/db/{db_branch_name}/tables/{table_name}/columns/{column_name}"
         return self.request("GET", url_path)
 
     def delete_column(
         self, table_name: str, column_name: str, db_name: str = None, branch_name: str = None
@@ -256,15 +256,15 @@
         - 5XX: Unexpected Error
 
         :param table_name: str The Table name
         :param column_name: str The Column name
         :param db_name: str = None The name of the database to query. Default: database name from the client.
         :param branch_name: str = None The name of the branch to query. Default: branch name from the client.
 
-        :return Response
+        :returns ApiResponse
         """
         db_branch_name = self.client.get_db_branch_name(db_name, branch_name)
         url_path = f"/db/{db_branch_name}/tables/{table_name}/columns/{column_name}"
         return self.request("DELETE", url_path)
 
     def update_column(
         self, table_name: str, column_name: str, payload: dict, db_name: str = None, branch_name: str = None
@@ -284,13 +284,13 @@
 
         :param table_name: str The Table name
         :param column_name: str The Column name
         :param payload: dict content
         :param db_name: str = None The name of the database to query. Default: database name from the client.
         :param branch_name: str = None The name of the branch to query. Default: branch name from the client.
 
-        :return Response
+        :returns ApiResponse
         """
         db_branch_name = self.client.get_db_branch_name(db_name, branch_name)
         url_path = f"/db/{db_branch_name}/tables/{table_name}/columns/{column_name}"
         headers = {"content-type": "application/json"}
         return self.request("PATCH", url_path, headers, payload)
```

### Comparing `xata-1.0.0a1/xata/api/users.py` & `xata-1.0.0a2/xata/api/users.py`

 * *Files 5% similar despite different names*

```diff
@@ -42,15 +42,15 @@
         - 400: Bad Request
         - 401: Authentication Error
         - 404: Example response
         - 5XX: Unexpected Error
         Response: application/json
 
 
-        :return Response
+        :returns ApiResponse
         """
         url_path = "/user"
         return self.request("GET", url_path)
 
     def update(self, payload: dict) -> ApiResponse:
         """
         Update user info
@@ -63,15 +63,15 @@
         - 401: Authentication Error
         - 404: Example response
         - 5XX: Unexpected Error
         Response: application/json
 
         :param payload: dict content
 
-        :return Response
+        :returns ApiResponse
         """
         url_path = "/user"
         headers = {"content-type": "application/json"}
         return self.request("PUT", url_path, headers, payload)
 
     def delete(self) -> ApiResponse:
         """
@@ -83,11 +83,11 @@
         - 204: No Content
         - 400: Bad Request
         - 401: Authentication Error
         - 404: Example response
         - 5XX: Unexpected Error
 
 
-        :return Response
+        :returns ApiResponse
         """
         url_path = "/user"
         return self.request("DELETE", url_path)
```

### Comparing `xata-1.0.0a1/xata/api/workspaces.py` & `xata-1.0.0a2/xata/api/workspaces.py`

 * *Files 2% similar despite different names*

```diff
@@ -42,15 +42,15 @@
         - 400: Bad Request
         - 401: Authentication Error
         - 404: Example response
         - 5XX: Unexpected Error
         Response: application/json
 
 
-        :return Response
+        :returns ApiResponse
         """
         url_path = "/workspaces"
         return self.request("GET", url_path)
 
     def create(self, payload: dict) -> ApiResponse:
         """
         Creates a new workspace with the user requesting it as its single owner.
@@ -63,15 +63,15 @@
         - 401: Authentication Error
         - 404: Example response
         - 5XX: Unexpected Error
         Response: application/json
 
         :param payload: dict content
 
-        :return Response
+        :returns ApiResponse
         """
         url_path = "/workspaces"
         headers = {"content-type": "application/json"}
         return self.request("POST", url_path, headers, payload)
 
     def get(self, workspace_id: str = None) -> ApiResponse:
         """
@@ -86,15 +86,15 @@
         - 403: Authentication Error
         - 404: Example response
         - 5XX: Unexpected Error
         Response: application/json
 
         :param workspace_id: str = None The workspace identifier. Default: workspace Id from the client.
 
-        :return Response
+        :returns ApiResponse
         """
         if workspace_id is None:
             workspace_id = self.client.get_workspace_id()
         url_path = f"/workspaces/{workspace_id}"
         return self.request("GET", url_path)
 
     def update(self, payload: dict, workspace_id: str = None) -> ApiResponse:
@@ -111,15 +111,15 @@
         - 404: Example response
         - 5XX: Unexpected Error
         Response: application/json
 
         :param payload: dict content
         :param workspace_id: str = None The workspace identifier. Default: workspace Id from the client.
 
-        :return Response
+        :returns ApiResponse
         """
         if workspace_id is None:
             workspace_id = self.client.get_workspace_id()
         url_path = f"/workspaces/{workspace_id}"
         headers = {"content-type": "application/json"}
         return self.request("PUT", url_path, headers, payload)
 
@@ -135,15 +135,15 @@
         - 401: Authentication Error
         - 403: Authentication Error
         - 404: Example response
         - 5XX: Unexpected Error
 
         :param workspace_id: str = None The workspace identifier. Default: workspace Id from the client.
 
-        :return Response
+        :returns ApiResponse
         """
         if workspace_id is None:
             workspace_id = self.client.get_workspace_id()
         url_path = f"/workspaces/{workspace_id}"
         return self.request("DELETE", url_path)
 
     def get_members(self, workspace_id: str = None) -> ApiResponse:
@@ -159,15 +159,15 @@
         - 403: Authentication Error
         - 404: Example response
         - 5XX: Unexpected Error
         Response: application/json
 
         :param workspace_id: str = None The workspace identifier. Default: workspace Id from the client.
 
-        :return Response
+        :returns ApiResponse
         """
         if workspace_id is None:
             workspace_id = self.client.get_workspace_id()
         url_path = f"/workspaces/{workspace_id}/members"
         return self.request("GET", url_path)
 
     def update_member(self, user_id: str, payload: dict, workspace_id: str = None) -> ApiResponse:
@@ -185,15 +185,15 @@
         - 404: Example response
         - 5XX: Unexpected Error
 
         :param user_id: str UserID
         :param payload: dict content
         :param workspace_id: str = None The workspace identifier. Default: workspace Id from the client.
 
-        :return Response
+        :returns ApiResponse
         """
         if workspace_id is None:
             workspace_id = self.client.get_workspace_id()
         url_path = f"/workspaces/{workspace_id}/members/{user_id}"
         headers = {"content-type": "application/json"}
         return self.request("PUT", url_path, headers, payload)
 
@@ -210,13 +210,13 @@
         - 403: Authentication Error
         - 404: Example response
         - 5XX: Unexpected Error
 
         :param user_id: str UserID
         :param workspace_id: str = None The workspace identifier. Default: workspace Id from the client.
 
-        :return Response
+        :returns ApiResponse
         """
         if workspace_id is None:
             workspace_id = self.client.get_workspace_id()
         url_path = f"/workspaces/{workspace_id}/members/{user_id}"
         return self.request("DELETE", url_path)
```

### Comparing `xata-1.0.0a1/xata/api_response.py` & `xata-1.0.0a2/xata/api_response.py`

 * *Files 6% similar despite different names*

```diff
@@ -16,14 +16,15 @@
 # specific language governing permissions and limitations
 # under the License.
 #
 
 import logging
 from typing import Union
 
+import deprecation
 from requests import Response
 from requests.exceptions import JSONDecodeError
 
 
 class ApiResponse(dict):
     def __init__(self, response: Response):
         self.response = response
@@ -38,43 +39,53 @@
         # log server message
         if "x-xata-message" in self.headers:
             self.logger.warn(self.headers["x-xata-message"])
 
     def server_message(self) -> Union[str, None]:
         """
         Get the server message from the response
-        :return str | None
+        :returns str | None
         """
-        if "x-xata-message" in self.headers:
-            return self.headers["x-xata-message"]
-        return None
+        return self.headers["x-xata-message"] if "x-xata-message" in self.headers else None
 
     def is_success(self) -> bool:
         """
         Was the request successful?
-        :return bool
+        :returns bool
         """
         return 200 <= self.status_code < 300
 
+    @deprecation.deprecated(
+        deprecated_in="1.0.0a2",
+        removed_in="2.0.0",
+        details="This method is obsolete as this class directly returns a dict",
+    )
+    def json(self) -> dict:
+        """
+        Legacy support for requests.Response from 0.x
+        :returns dict
+        """
+        return self.response.json()
+
     @property
     def status_code(self) -> int:
         """
         Get the status code of the response
-        :return int
+        :returns int
         """
         return self.response.status_code
 
     @property
     def headers(self) -> dict:
         """
         Get the response headers
-        :return dict
+        :returns dict
         """
         return self.response.headers
 
     @property
     def content(self) -> bytes:
         """
         For files support, to get the file content
-        :return bytes
+        :returns bytes
         """
         return self.response.content
```

### Comparing `xata-1.0.0a1/xata/client.py` & `xata-1.0.0a2/xata/client.py`

 * *Files 2% similar despite different names*

```diff
@@ -34,15 +34,15 @@
 from .api.search_and_filter import SearchAndFilter
 from .api.table import Table
 from .api.users import Users
 from .api.workspaces import Workspaces
 
 # TODO this is a manual task, to keep in sync with pyproject.toml
 # could/should be automated to keep in sync
-__version__ = "1.0.0a1"
+__version__ = "1.0.0a2"
 
 PERSONAL_API_KEY_LOCATION = "~/.config/xata/key"
 DEFAULT_DATA_PLANE_DOMAIN = "xata.sh"
 DEFAULT_CONTROL_PLANE_DOMAIN = "api.xata.io"
 DEFAULT_REGION = "us-east-1"
 DEFAULT_BRANCH_NAME = "main"
 CONFIG_LOCATION = ".xatarc"
@@ -185,15 +185,15 @@
         """
         self.headers[name.lower().strip()] = value
 
     def delete_header(self, name: str) -> bool:
         """
         Delete a header from the scope. A header name will be lowercased.
         :param name: str
-        :return bool
+        :returns bool
         """
         name = name.lower().strip()
         if name not in self.headers:
             return False
         del self.headers[name]
         return True
 
@@ -254,15 +254,15 @@
         """
         Get Database with branch name, format: {db_name}:{branch_name}
         The name can be build with passed params or from config or a combination of both
 
         :param db_name: str
         :branch_name: str
 
-        :return str
+        :returns str
         """
         if db_name is None:
             db_name = self.db_name
         if branch_name is None:
             branch_name = self.branch_name
         return f"{db_name}:{branch_name}"
 
@@ -288,15 +288,15 @@
         return True
 
     def _parse_database_url(self, database_url: str) -> tuple[str, str, str, str, str]:
         """
         Parse Database URL
         Branch name is optional.
         Format: https://{workspace_id}.{region}.xata.sh/db/{db_name}:{branch_name}
-        :return workspace_id, region, db_name, branch_name, domain
+        :returns workspace_id, region, db_name, branch_name, domain
         """
         (_, _, host, _, db_branch_name) = database_url.split("/")
         if host == "" or db_branch_name == "":
             raise Exception(
                 "Invalid database URL: '%s', expected the format: "
                 + "'https://{workspace_id}.{region}.xata.sh/db/{db_name}:{branch_name}'" % database_url
             )
@@ -316,83 +316,83 @@
             return host_parts[0], host_parts[1], db_branch_parts[0], db_branch_parts[1], domain
         # does not have a branch defined
         return host_parts[0], host_parts[1], db_branch_parts[0], DEFAULT_BRANCH_NAME, domain
 
     def authentication(self) -> Authentication:
         """
         Authentication Namespace
-        :return Authentication
+        :returns Authentication
         """
         return self._authentication
 
     def databases(self) -> Databases:
         """
         Databases Namespace
-        :return Databases
+        :returns Databases
         """
         return self._databases
 
     def invites(self) -> Invites:
         """
         Invites Namespace
-        :return Invites
+        :returns Invites
         """
         return self._invites
 
     def users(self) -> Users:
         """
         Users Namespace
-        :return Users
+        :returns Users
         """
         return self._users
 
     def workspaces(self) -> Workspaces:
         """
         Workspaces Namespace
-        :return Workspaces
+        :returns Workspaces
         """
         return self._workspaces
 
     def branch(self) -> Branch:
         """
         Branch Namespace
-        :return Branch
+        :returns Branch
         """
         return self._branch
 
     def migrations(self) -> Migrations:
         """
         Migrations Namespace
-        :return Migrations
+        :returns Migrations
         """
         return self._migrations
 
     def records(self) -> Records:
         """
         Records Namespace
-        :return Records
+        :returns Records
         """
         return self._records
 
     def search_and_filter(self) -> SearchAndFilter:
         """
         Search_and_Filter Namespace
-        :return Search_and_filter
+        :returns Search_and_filter
         """
         return self._search_and_filter
 
     def data(self) -> SearchAndFilter:
         """
         Shorter alias for Search_and_Filter
-        :return Search_and_filter
+        :returns Search_and_filter
         """
         return self._search_and_filter
 
     def table(self) -> Table:
         """
         Table Namespace
-        :return Table
+        :returns Table
         """
         return self._table
 
     def files(self) -> Files:
         return self._files
```

### Comparing `xata-1.0.0a1/xata/errors.py` & `xata-1.0.0a2/xata/errors.py`

 * *Files identical despite different names*

### Comparing `xata-1.0.0a1/xata/helpers.py` & `xata-1.0.0a2/xata/helpers.py`

 * *Files 1% similar despite different names*

```diff
@@ -158,23 +158,23 @@
         :param records: list[dict]
         """
         self.records.put(table_name, records)
 
     def get_failed_batches(self) -> list[dict]:
         """
         Get the batched records that could not be processed with the error
-        :return list[dict]
+        :returns list[dict]
         """
         return self.failed_batches_queue
 
     def get_stats(self):
         """
         Get processing statistics
 
-        :return dict
+        :returns dict
         """
         return self.stats
 
     def flush_queue(self):
         """
         Flush all records from the queue.
         """
@@ -227,15 +227,15 @@
             with self.store[table_name]["lock"]:
                 self.store[table_name]["records"] += records
 
         def next_batch(self) -> dict:
             """
             Get the next batch of records to persist
 
-            :return dict
+            :returns dict
             """
             table_name = ""
             with self.lock:
                 names = list(self.store.keys())
                 if len(names) == 0:
                     return {}
 
@@ -287,15 +287,15 @@
     """
     Format a datetime object to an RFC3339 compliant string
     :link https://xata.io/docs/concepts/data-model#datetime
     :link https://datatracker.ietf.org/doc/html/rfc3339
 
     :param dt: datetime instance to convert
     :param tz: timezone to convert in, default: UTC
-    :return str
+    :returns str
     """
     return dt.replace(tzinfo=tz).isoformat()
 
 
 class Transaction(object):
     """
     Additional abstraction for bulk requests that process'
@@ -388,25 +388,25 @@
         """
         self._add_operation({"get": {"table": table, "id": record_id, "columns": columns}})
 
     def run(self) -> dict:
         """
         Commit the transactions. Flushes the operations queue
 
-        :return dict
+        :returns dict
         """
         r = self.client.records().transaction(self.operations)
         result = {
             "status_code": r.status_code,
             "results": r["results"] if "results" in r else [],
             "has_errors": True if "errors" in r else False,
             "errors": r["errors"] if "errors" in r else [],
         }
         self.operations["operations"] = []  # free memory
         return result
 
     def size(self) -> int:
         """
         Get amount of operations in queue
-        :return int
+        :returns int
         """
         return len(self.operations["operations"])
```

### Comparing `xata-1.0.0a1/xata/namespace.py` & `xata-1.0.0a2/xata/namespace.py`

 * *Files 0% similar despite different names*

```diff
@@ -54,15 +54,15 @@
         """
         :param http_method: str
         :param url_path: str
         :headers: dict = {}
         :param payload: dict = None
         :param data: bytes = None
 
-        :return ApiResponse
+        :returns ApiResponse
 
         :raises RateLimitError
         :raises UnauthorizedError
         :raises ServerError
         """
         # TODO use "|" when client py min version >= 3.9
         headers = {**headers, **self.client.get_headers()}
```

### Comparing `xata-1.0.0a1/PKG-INFO` & `xata-1.0.0a2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: xata
-Version: 1.0.0a1
+Version: 1.0.0a2
 Summary: Python client for Xata.io
 License: Apache-2.0
 Author: Xata
 Author-email: support@xata.io
 Requires-Python: >=3.9,<4.0
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3
```

