# Comparing `tmp/twscrape-0.3.0.tar.gz` & `tmp/twscrape-0.4.0.tar.gz`

## Comparing `twscrape-0.3.0.tar` & `twscrape-0.4.0.tar`

### file list

```diff
@@ -1,44 +1,44 @@
--rw-r--r--   0        0        0       34 2020-02-02 00:00:00.000000 twscrape-0.3.0/.gitattributes
--rw-r--r--   0        0        0      724 2020-02-02 00:00:00.000000 twscrape-0.3.0/Dockerfile-test
--rw-r--r--   0        0        0      633 2020-02-02 00:00:00.000000 twscrape-0.3.0/Makefile
--rw-r--r--   0        0        0       11 2020-02-02 00:00:00.000000 twscrape-0.3.0/.github/CODEOWNERS
--rw-r--r--   0        0        0       16 2020-02-02 00:00:00.000000 twscrape-0.3.0/.github/FUNDING.yml
--rw-r--r--   0        0        0      512 2020-02-02 00:00:00.000000 twscrape-0.3.0/.github/workflows/publish.yml
--rw-r--r--   0        0        0      493 2020-02-02 00:00:00.000000 twscrape-0.3.0/.github/workflows/test.yml
--rw-r--r--   0        0        0      301 2020-02-02 00:00:00.000000 twscrape-0.3.0/.vscode/settings.json
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 twscrape-0.3.0/tests/__init__.py
--rw-r--r--   0        0        0      890 2020-02-02 00:00:00.000000 twscrape-0.3.0/tests/conftest.py
--rw-r--r--   0        0        0      939 2020-02-02 00:00:00.000000 twscrape-0.3.0/tests/test_api.py
--rw-r--r--   0        0        0     7899 2020-02-02 00:00:00.000000 twscrape-0.3.0/tests/test_parser.py
--rw-r--r--   0        0        0     4460 2020-02-02 00:00:00.000000 twscrape-0.3.0/tests/test_pool.py
--rw-r--r--   0        0        0     2520 2020-02-02 00:00:00.000000 twscrape-0.3.0/tests/test_queue_client.py
--rw-r--r--   0        0        0    67646 2020-02-02 00:00:00.000000 twscrape-0.3.0/tests/mocked-data/favoriters_raw.json
--rw-r--r--   0        0        0   152580 2020-02-02 00:00:00.000000 twscrape-0.3.0/tests/mocked-data/followers_raw.json
--rw-r--r--   0        0        0   142243 2020-02-02 00:00:00.000000 twscrape-0.3.0/tests/mocked-data/following_raw.json
--rw-r--r--   0        0        0    76607 2020-02-02 00:00:00.000000 twscrape-0.3.0/tests/mocked-data/manual_tweet_with_video_1.json
--rw-r--r--   0        0        0    84696 2020-02-02 00:00:00.000000 twscrape-0.3.0/tests/mocked-data/manual_tweet_with_video_2.json
--rw-r--r--   0        0        0    69669 2020-02-02 00:00:00.000000 twscrape-0.3.0/tests/mocked-data/retweeters_raw.json
--rw-r--r--   0        0        0   177570 2020-02-02 00:00:00.000000 twscrape-0.3.0/tests/mocked-data/search_raw.json
--rw-r--r--   0        0        0    95327 2020-02-02 00:00:00.000000 twscrape-0.3.0/tests/mocked-data/tweet_details_raw.json
--rw-r--r--   0        0        0     3107 2020-02-02 00:00:00.000000 twscrape-0.3.0/tests/mocked-data/user_by_id_raw.json
--rw-r--r--   0        0        0     4178 2020-02-02 00:00:00.000000 twscrape-0.3.0/tests/mocked-data/user_by_login_raw.json
--rw-r--r--   0        0        0   497799 2020-02-02 00:00:00.000000 twscrape-0.3.0/tests/mocked-data/user_tweets_and_replies_raw.json
--rw-r--r--   0        0        0   496101 2020-02-02 00:00:00.000000 twscrape-0.3.0/tests/mocked-data/user_tweets_raw.json
--rw-r--r--   0        0        0      205 2020-02-02 00:00:00.000000 twscrape-0.3.0/twscrape/__init__.py
--rw-r--r--   0        0        0     2337 2020-02-02 00:00:00.000000 twscrape-0.3.0/twscrape/account.py
--rw-r--r--   0        0        0     8379 2020-02-02 00:00:00.000000 twscrape-0.3.0/twscrape/accounts_pool.py
--rw-r--r--   0        0        0     9515 2020-02-02 00:00:00.000000 twscrape-0.3.0/twscrape/api.py
--rw-r--r--   0        0        0     4786 2020-02-02 00:00:00.000000 twscrape-0.3.0/twscrape/cli.py
--rw-r--r--   0        0        0     2771 2020-02-02 00:00:00.000000 twscrape-0.3.0/twscrape/constants.py
--rw-r--r--   0        0        0     4294 2020-02-02 00:00:00.000000 twscrape-0.3.0/twscrape/db.py
--rw-r--r--   0        0        0     2968 2020-02-02 00:00:00.000000 twscrape-0.3.0/twscrape/imap.py
--rw-r--r--   0        0        0      348 2020-02-02 00:00:00.000000 twscrape-0.3.0/twscrape/logger.py
--rw-r--r--   0        0        0     6992 2020-02-02 00:00:00.000000 twscrape-0.3.0/twscrape/login.py
--rw-r--r--   0        0        0     9630 2020-02-02 00:00:00.000000 twscrape-0.3.0/twscrape/models.py
--rw-r--r--   0        0        0     4707 2020-02-02 00:00:00.000000 twscrape-0.3.0/twscrape/queue_client.py
--rw-r--r--   0        0        0     4305 2020-02-02 00:00:00.000000 twscrape-0.3.0/twscrape/utils.py
--rw-r--r--   0        0        0     3153 2020-02-02 00:00:00.000000 twscrape-0.3.0/.gitignore
--rw-r--r--   0        0        0     1064 2020-02-02 00:00:00.000000 twscrape-0.3.0/LICENSE
--rw-r--r--   0        0        0     1514 2020-02-02 00:00:00.000000 twscrape-0.3.0/pyproject.toml
--rw-r--r--   0        0        0     6846 2020-02-02 00:00:00.000000 twscrape-0.3.0/readme.md
--rw-r--r--   0        0        0     7868 2020-02-02 00:00:00.000000 twscrape-0.3.0/PKG-INFO
+-rw-r--r--   0        0        0       34 2020-02-02 00:00:00.000000 twscrape-0.4.0/.gitattributes
+-rw-r--r--   0        0        0      724 2020-02-02 00:00:00.000000 twscrape-0.4.0/Dockerfile-test
+-rw-r--r--   0        0        0      633 2020-02-02 00:00:00.000000 twscrape-0.4.0/Makefile
+-rw-r--r--   0        0        0       11 2020-02-02 00:00:00.000000 twscrape-0.4.0/.github/CODEOWNERS
+-rw-r--r--   0        0        0       16 2020-02-02 00:00:00.000000 twscrape-0.4.0/.github/FUNDING.yml
+-rw-r--r--   0        0        0      512 2020-02-02 00:00:00.000000 twscrape-0.4.0/.github/workflows/publish.yml
+-rw-r--r--   0        0        0      493 2020-02-02 00:00:00.000000 twscrape-0.4.0/.github/workflows/test.yml
+-rw-r--r--   0        0        0      301 2020-02-02 00:00:00.000000 twscrape-0.4.0/.vscode/settings.json
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 twscrape-0.4.0/tests/__init__.py
+-rw-r--r--   0        0        0      890 2020-02-02 00:00:00.000000 twscrape-0.4.0/tests/conftest.py
+-rw-r--r--   0        0        0      939 2020-02-02 00:00:00.000000 twscrape-0.4.0/tests/test_api.py
+-rw-r--r--   0        0        0     8136 2020-02-02 00:00:00.000000 twscrape-0.4.0/tests/test_parser.py
+-rw-r--r--   0        0        0     4460 2020-02-02 00:00:00.000000 twscrape-0.4.0/tests/test_pool.py
+-rw-r--r--   0        0        0     2520 2020-02-02 00:00:00.000000 twscrape-0.4.0/tests/test_queue_client.py
+-rw-r--r--   0        0        0    67646 2020-02-02 00:00:00.000000 twscrape-0.4.0/tests/mocked-data/favoriters_raw.json
+-rw-r--r--   0        0        0   152580 2020-02-02 00:00:00.000000 twscrape-0.4.0/tests/mocked-data/followers_raw.json
+-rw-r--r--   0        0        0   142243 2020-02-02 00:00:00.000000 twscrape-0.4.0/tests/mocked-data/following_raw.json
+-rw-r--r--   0        0        0    76607 2020-02-02 00:00:00.000000 twscrape-0.4.0/tests/mocked-data/manual_tweet_with_video_1.json
+-rw-r--r--   0        0        0    84696 2020-02-02 00:00:00.000000 twscrape-0.4.0/tests/mocked-data/manual_tweet_with_video_2.json
+-rw-r--r--   0        0        0    69669 2020-02-02 00:00:00.000000 twscrape-0.4.0/tests/mocked-data/retweeters_raw.json
+-rw-r--r--   0        0        0   110556 2020-02-02 00:00:00.000000 twscrape-0.4.0/tests/mocked-data/search_raw.json
+-rw-r--r--   0        0        0    95327 2020-02-02 00:00:00.000000 twscrape-0.4.0/tests/mocked-data/tweet_details_raw.json
+-rw-r--r--   0        0        0     3107 2020-02-02 00:00:00.000000 twscrape-0.4.0/tests/mocked-data/user_by_id_raw.json
+-rw-r--r--   0        0        0     4178 2020-02-02 00:00:00.000000 twscrape-0.4.0/tests/mocked-data/user_by_login_raw.json
+-rw-r--r--   0        0        0   497799 2020-02-02 00:00:00.000000 twscrape-0.4.0/tests/mocked-data/user_tweets_and_replies_raw.json
+-rw-r--r--   0        0        0   496101 2020-02-02 00:00:00.000000 twscrape-0.4.0/tests/mocked-data/user_tweets_raw.json
+-rw-r--r--   0        0        0      205 2020-02-02 00:00:00.000000 twscrape-0.4.0/twscrape/__init__.py
+-rw-r--r--   0        0        0     2337 2020-02-02 00:00:00.000000 twscrape-0.4.0/twscrape/account.py
+-rw-r--r--   0        0        0     8379 2020-02-02 00:00:00.000000 twscrape-0.4.0/twscrape/accounts_pool.py
+-rw-r--r--   0        0        0     9734 2020-02-02 00:00:00.000000 twscrape-0.4.0/twscrape/api.py
+-rw-r--r--   0        0        0     4775 2020-02-02 00:00:00.000000 twscrape-0.4.0/twscrape/cli.py
+-rw-r--r--   0        0        0     1308 2020-02-02 00:00:00.000000 twscrape-0.4.0/twscrape/constants.py
+-rw-r--r--   0        0        0     4294 2020-02-02 00:00:00.000000 twscrape-0.4.0/twscrape/db.py
+-rw-r--r--   0        0        0     2968 2020-02-02 00:00:00.000000 twscrape-0.4.0/twscrape/imap.py
+-rw-r--r--   0        0        0      348 2020-02-02 00:00:00.000000 twscrape-0.4.0/twscrape/logger.py
+-rw-r--r--   0        0        0     6992 2020-02-02 00:00:00.000000 twscrape-0.4.0/twscrape/login.py
+-rw-r--r--   0        0        0     9992 2020-02-02 00:00:00.000000 twscrape-0.4.0/twscrape/models.py
+-rw-r--r--   0        0        0     4751 2020-02-02 00:00:00.000000 twscrape-0.4.0/twscrape/queue_client.py
+-rw-r--r--   0        0        0     4305 2020-02-02 00:00:00.000000 twscrape-0.4.0/twscrape/utils.py
+-rw-r--r--   0        0        0     3153 2020-02-02 00:00:00.000000 twscrape-0.4.0/.gitignore
+-rw-r--r--   0        0        0     1064 2020-02-02 00:00:00.000000 twscrape-0.4.0/LICENSE
+-rw-r--r--   0        0        0     1514 2020-02-02 00:00:00.000000 twscrape-0.4.0/pyproject.toml
+-rw-r--r--   0        0        0     6846 2020-02-02 00:00:00.000000 twscrape-0.4.0/readme.md
+-rw-r--r--   0        0        0     7868 2020-02-02 00:00:00.000000 twscrape-0.4.0/PKG-INFO
```

### Comparing `twscrape-0.3.0/Dockerfile-test` & `twscrape-0.4.0/Dockerfile-test`

 * *Files identical despite different names*

### Comparing `twscrape-0.3.0/Makefile` & `twscrape-0.4.0/Makefile`

 * *Files identical despite different names*

### Comparing `twscrape-0.3.0/.github/workflows/publish.yml` & `twscrape-0.4.0/.github/workflows/publish.yml`

 * *Files identical despite different names*

### Comparing `twscrape-0.3.0/tests/conftest.py` & `twscrape-0.4.0/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `twscrape-0.3.0/tests/test_api.py` & `twscrape-0.4.0/tests/test_api.py`

 * *Files identical despite different names*

### Comparing `twscrape-0.3.0/tests/test_parser.py` & `twscrape-0.4.0/tests/test_parser.py`

 * *Files 2% similar despite different names*

```diff
@@ -100,14 +100,21 @@
     assert doc.id is not None
     assert doc.id_str is not None
     assert isinstance(doc.id, int)
     assert isinstance(doc.id_str, str)
     assert doc.id == int(doc.id_str)
 
     assert doc.username is not None
+    assert doc.descriptionLinks is not None
+
+    if len(doc.descriptionLinks) > 0:
+        for x in doc.descriptionLinks:
+            assert x.url is not None
+            assert x.text is not None
+            assert x.tcourl is not None
 
     obj = doc.dict()
     assert doc.id == obj["id"]
     assert doc.username == obj["username"]
 
     txt = doc.json()
     assert isinstance(txt, str)
```

### Comparing `twscrape-0.3.0/tests/test_pool.py` & `twscrape-0.4.0/tests/test_pool.py`

 * *Files identical despite different names*

### Comparing `twscrape-0.3.0/tests/test_queue_client.py` & `twscrape-0.4.0/tests/test_queue_client.py`

 * *Files identical despite different names*

### Comparing `twscrape-0.3.0/tests/mocked-data/favoriters_raw.json` & `twscrape-0.4.0/tests/mocked-data/favoriters_raw.json`

 * *Files identical despite different names*

### Comparing `twscrape-0.3.0/tests/mocked-data/followers_raw.json` & `twscrape-0.4.0/tests/mocked-data/followers_raw.json`

 * *Files identical despite different names*

### Comparing `twscrape-0.3.0/tests/mocked-data/following_raw.json` & `twscrape-0.4.0/tests/mocked-data/following_raw.json`

 * *Files identical despite different names*

### Comparing `twscrape-0.3.0/tests/mocked-data/manual_tweet_with_video_1.json` & `twscrape-0.4.0/tests/mocked-data/manual_tweet_with_video_1.json`

 * *Files identical despite different names*

### Comparing `twscrape-0.3.0/tests/mocked-data/manual_tweet_with_video_2.json` & `twscrape-0.4.0/tests/mocked-data/manual_tweet_with_video_2.json`

 * *Files identical despite different names*

### Comparing `twscrape-0.3.0/tests/mocked-data/retweeters_raw.json` & `twscrape-0.4.0/tests/mocked-data/retweeters_raw.json`

 * *Files identical despite different names*

### Comparing `twscrape-0.3.0/tests/mocked-data/tweet_details_raw.json` & `twscrape-0.4.0/tests/mocked-data/tweet_details_raw.json`

 * *Files identical despite different names*

### Comparing `twscrape-0.3.0/tests/mocked-data/user_by_id_raw.json` & `twscrape-0.4.0/tests/mocked-data/user_by_id_raw.json`

 * *Files identical despite different names*

### Comparing `twscrape-0.3.0/tests/mocked-data/user_by_login_raw.json` & `twscrape-0.4.0/tests/mocked-data/user_by_login_raw.json`

 * *Files identical despite different names*

### Comparing `twscrape-0.3.0/tests/mocked-data/user_tweets_and_replies_raw.json` & `twscrape-0.4.0/tests/mocked-data/user_tweets_and_replies_raw.json`

 * *Files identical despite different names*

### Comparing `twscrape-0.3.0/tests/mocked-data/user_tweets_raw.json` & `twscrape-0.4.0/tests/mocked-data/user_tweets_raw.json`

 * *Files identical despite different names*

### Comparing `twscrape-0.3.0/twscrape/account.py` & `twscrape-0.4.0/twscrape/account.py`

 * *Files identical despite different names*

### Comparing `twscrape-0.3.0/twscrape/accounts_pool.py` & `twscrape-0.4.0/twscrape/accounts_pool.py`

 * *Files identical despite different names*

### Comparing `twscrape-0.3.0/twscrape/api.py` & `twscrape-0.4.0/twscrape/api.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from httpx import Response
 
 from .accounts_pool import AccountsPool
-from .constants import GQL_FEATURES, GQL_URL, SEARCH_PARAMS, SEARCH_URL
+from .constants import GQL_FEATURES, GQL_URL
 from .logger import logger
 from .models import Tweet, User
 from .queue_client import QueueClient, req_id
 from .utils import encode_params, find_obj, get_by_path, to_old_obj, to_old_rep
 
 
 class API:
@@ -32,20 +32,23 @@
     def _get_cursor(self, obj: dict):
         if cur := find_obj(obj, lambda x: x.get("cursorType") == "Bottom"):
             return cur.get("value")
         return None
 
     # gql helpers
 
-    async def _gql_items(self, op: str, kv: dict, limit=-1):
+    async def _gql_items(self, op: str, kv: dict, ft: dict | None = None, limit=-1):
         queue, cursor, count, active = op.split("/")[-1], None, 0, True
+        kv, ft = {**kv}, {**GQL_FEATURES, **(ft or {})}
 
         async with QueueClient(self.pool, queue, self.debug) as client:
             while active:
-                params = {"variables": {**kv, "cursor": cursor}, "features": GQL_FEATURES}
+                params = {"variables": {**kv, "cursor": cursor}, "features": ft}
+                if op.endswith("/SearchTimeline"):
+                    params["fieldToggles"] = {"withArticleRichContentState": False}
 
                 rep = await client.get(f"{GQL_URL}/{op}", params=encode_params(params))
                 obj = rep.json()
 
                 entries = get_by_path(obj, "entries") or []
                 entries = [x for x in entries if not x["entryId"].startswith("cursor-")]
                 cursor = self._get_cursor(obj)
@@ -61,43 +64,43 @@
         queue = op.split("/")[-1]
         async with QueueClient(self.pool, queue, self.debug) as client:
             params = {"variables": {**kv}, "features": {**GQL_FEATURES, **ft}}
             return await client.get(f"{GQL_URL}/{op}", params=encode_params(params))
 
     # search
 
-    async def search_raw(self, q: str, limit=-1):
-        queue, cursor, count, active = "search", None, 0, True
+    async def search_raw(self, q: str, limit=-1, kv=None):
+        op = "nK1dw4oV3k4w5TdtcAdSww/SearchTimeline"
+        kv = {
+            "rawQuery": q,
+            "count": 20,
+            "product": "Latest",
+            "querySource": "typed_query",
+            **(kv or {}),
+        }
+        ft = {
+            "rweb_lists_timeline_redesign_enabled": True,
+            "creator_subscriptions_tweet_preview_api_enabled": True,
+            "responsive_web_twitter_article_tweet_consumption_enabled": False,
+            "tweet_with_visibility_results_prefer_gql_limited_actions_policy_enabled": True,
+            "responsive_web_media_download_video_enabled": False,
+            "longform_notetweets_inline_media_enabled": True,
+        }
+        async for x in self._gql_items(op, kv, ft, limit=limit):
+            yield x
 
-        async with QueueClient(self.pool, queue, self.debug) as client:
-            while active:
-                params = {**SEARCH_PARAMS, "q": q, "count": 20}
-                params["cursor" if cursor else "requestContext"] = cursor if cursor else "launch"
-
-                rep = await client.get(SEARCH_URL, params=params)
-                obj = rep.json()
-
-                tweets = obj.get("globalObjects", {}).get("tweets", [])
-                cursor = self._get_cursor(obj)
-
-                rep, count, active = self._is_end(rep, q, tweets, cursor, count, limit)
-                if rep is None:
-                    return
-
-                yield rep
-
-    async def search(self, q: str, limit=-1):
+    async def search(self, q: str, limit=-1, kv=None):
         twids = set()
-        async for rep in self.search_raw(q, limit=limit):
-            res = rep.json()
-            obj = res.get("globalObjects", {})
-            for x in list(obj.get("tweets", {}).values()):
-                if x["id_str"] not in twids:
-                    twids.add(x["id_str"])
-                    yield Tweet.parse(x, obj)
+        async for rep in self.search_raw(q, limit=limit, kv=kv):
+            obj = to_old_rep(rep.json())
+            for x in obj["tweets"].values():
+                tmp = Tweet.parse(x, obj)
+                if tmp.id not in twids:
+                    twids.add(tmp.id)
+                    yield tmp
 
     # user_by_id
 
     async def user_by_id_raw(self, uid: int, kv=None):
         op = "GazOglcBvgLigl3ywt6b3Q/UserByRestId"
         kv = {"userId": str(uid), "withSafetyModeUserFields": True, **(kv or {})}
         return await self._gql_item(op, kv)
```

### Comparing `twscrape-0.3.0/twscrape/cli.py` & `twscrape-0.4.0/twscrape/cli.py`

 * *Files 14% similar despite different names*

```diff
@@ -3,17 +3,20 @@
 import argparse
 import asyncio
 import io
 import json
 import sqlite3
 from importlib.metadata import version
 
+import httpx
+
 from .api import API, AccountsPool
 from .db import get_sqlite_version
 from .logger import logger, set_log_level
+from .models import Tweet, User
 from .utils import print_table
 
 
 class CustomHelpFormatter(argparse.HelpFormatter):
     def __init__(self, prog):
         super().__init__(prog, max_help_position=30, width=120)
 
@@ -24,18 +27,17 @@
         if name in args:
             return name, getattr(args, name)
 
     logger.error(f"Missing argument: {names}")
     exit(1)
 
 
-def to_str(doc):
-    # doc is httpx.Response or twscrape.User / twscrape.Tweet
-    # both have .json method but with different return type
-    return doc if isinstance(doc, str) else json.dumps(doc.json(), default=str)
+def to_str(doc: httpx.Response | Tweet | User) -> str:
+    tmp = doc.json()
+    return tmp if isinstance(tmp, str) else json.dumps(tmp, default=str)
 
 
 async def main(args):
     if args.debug:
         set_log_level("DEBUG")
 
     if args.command == "version":
@@ -103,42 +105,42 @@
 
 def run():
     p = argparse.ArgumentParser(add_help=False, formatter_class=CustomHelpFormatter)
     p.add_argument("--db", default="accounts.db", help="Accounts database file")
     p.add_argument("--debug", action="store_true", help="Enable debug mode")
     subparsers = p.add_subparsers(dest="command")
 
-    def cone(name: str, msg: str, a_name: str, a_msg: str, a_type: type = str):
+    def c_one(name: str, msg: str, a_name: str, a_msg: str, a_type: type = str):
         p = subparsers.add_parser(name, help=msg)
         p.add_argument(a_name, help=a_msg, type=a_type)
         p.add_argument("--raw", action="store_true", help="Print raw response")
         return p
 
-    def clim(name: str, msg: str, a_name: str, a_msg: str, a_type: type = str):
-        p = cone(name, msg, a_name, a_msg, a_type)
+    def c_lim(name: str, msg: str, a_name: str, a_msg: str, a_type: type = str):
+        p = c_one(name, msg, a_name, a_msg, a_type)
         p.add_argument("--limit", type=int, default=-1, help="Max tweets to retrieve")
         return p
 
     subparsers.add_parser("version", help="Show version")
 
     subparsers.add_parser("accounts", help="List all accounts")
     add_accounts = subparsers.add_parser("add_accounts", help="Add accounts")
     add_accounts.add_argument("file_path", help="File with accounts")
     add_accounts.add_argument("line_format", help="args of Pool.add_account splited by same delim")
     subparsers.add_parser("login_accounts", help="Login accounts")
 
-    clim("search", "Search for tweets", "query", "Search query")
-    cone("tweet_details", "Get tweet details", "tweet_id", "Tweet ID", int)
-    clim("retweeters", "Get retweeters of a tweet", "tweet_id", "Tweet ID", int)
-    clim("favoriters", "Get favoriters of a tweet", "tweet_id", "Tweet ID", int)
-    cone("user_by_id", "Get user data by ID", "user_id", "User ID", int)
-    clim("user_by_login", "Get user data by username", "username", "Username")
-    clim("followers", "Get user followers", "user_id", "User ID", int)
-    clim("following", "Get user following", "user_id", "User ID", int)
-    clim("user_tweets", "Get user tweets", "user_id", "User ID", int)
-    clim("user_tweets_and_replies", "Get user tweets and replies", "user_id", "User ID", int)
+    c_lim("search", "Search for tweets", "query", "Search query")
+    c_one("tweet_details", "Get tweet details", "tweet_id", "Tweet ID", int)
+    c_lim("retweeters", "Get retweeters of a tweet", "tweet_id", "Tweet ID", int)
+    c_lim("favoriters", "Get favoriters of a tweet", "tweet_id", "Tweet ID", int)
+    c_one("user_by_id", "Get user data by ID", "user_id", "User ID", int)
+    c_one("user_by_login", "Get user data by username", "username", "Username")
+    c_lim("followers", "Get user followers", "user_id", "User ID", int)
+    c_lim("following", "Get user following", "user_id", "User ID", int)
+    c_lim("user_tweets", "Get user tweets", "user_id", "User ID", int)
+    c_lim("user_tweets_and_replies", "Get user tweets and replies", "user_id", "User ID", int)
 
     args = p.parse_args()
     if args.command is None:
         return custom_help(p)
 
     asyncio.run(main(args))
```

### Comparing `twscrape-0.3.0/twscrape/db.py` & `twscrape-0.4.0/twscrape/db.py`

 * *Files identical despite different names*

### Comparing `twscrape-0.3.0/twscrape/imap.py` & `twscrape-0.4.0/twscrape/imap.py`

 * *Files identical despite different names*

### Comparing `twscrape-0.3.0/twscrape/login.py` & `twscrape-0.4.0/twscrape/login.py`

 * *Files identical despite different names*

### Comparing `twscrape-0.3.0/twscrape/models.py` & `twscrape-0.4.0/twscrape/models.py`

 * *Files 8% similar despite different names*

```diff
@@ -56,25 +56,28 @@
 
 
 @dataclass
 class TextLink(JSONTrait):
     url: str
     text: str | None
     tcourl: str | None
-    indices: tuple[int, int]
 
     @staticmethod
     def parse(obj: dict):
-        return TextLink(
-            url=obj["expanded_url"],
-            text=obj["display_url"],
-            tcourl=obj["url"],
-            indices=tuple(obj["indices"]),
+        tmp = TextLink(
+            url=obj.get("expanded_url", None),
+            text=obj.get("display_url", None),
+            tcourl=obj.get("url", None),
         )
 
+        if tmp.url is None or tmp.tcourl is None:
+            return None
+
+        return tmp
+
 
 @dataclass
 class UserRef(JSONTrait):
     id: int
     username: str
     displayname: str
     _type: str = "snscrape.modules.twitter.UserRef"
@@ -100,18 +103,18 @@
     listedCount: int
     mediaCount: int
     location: str
     profileImageUrl: str
     profileBannerUrl: str | None = None
     protected: bool | None = None
     verified: bool | None = None
+    descriptionLinks: list[TextLink] = field(default_factory=list)
     _type: str = "snscrape.modules.twitter.User"
 
     # todo:
-    # descriptionLinks: typing.Optional[typing.List[TextLink]] = None
     # link: typing.Optional[TextLink] = None
     # label: typing.Optional["UserLabel"] = None
 
     @staticmethod
     def parse(obj: dict):
         return User(
             id=int(obj["id_str"]),
@@ -128,14 +131,15 @@
             listedCount=obj["listed_count"],
             mediaCount=obj["media_count"],
             location=obj["location"],
             profileImageUrl=obj["profile_image_url_https"],
             profileBannerUrl=obj.get("profile_banner_url"),
             verified=obj.get("verified"),
             protected=obj.get("protected"),
+            descriptionLinks=_parse_links(obj, ["entities.description.urls", "entities.url.urls"]),
         )
 
 
 @dataclass
 class Tweet(JSONTrait):
     id: int
     id_str: str
@@ -189,15 +193,15 @@
             retweetCount=obj["retweet_count"],
             likeCount=obj["favorite_count"],
             quoteCount=obj["quote_count"],
             conversationId=int(obj["conversation_id_str"]),
             hashtags=[x["text"] for x in get_or(obj, "entities.hashtags", [])],
             cashtags=[x["text"] for x in get_or(obj, "entities.symbols", [])],
             mentionedUsers=[UserRef.parse(x) for x in get_or(obj, "entities.user_mentions", [])],
-            links=[TextLink.parse(x) for x in get_or(obj, "entities.urls", [])],
+            links=_parse_links(obj, ["entities.urls"]),
             viewCount=int_or_none(obj, "ext_views.count"),
             retweetedTweet=Tweet.parse(rt_obj, res) if rt_obj else None,
             quotedTweet=Tweet.parse(qt_obj, res) if qt_obj else None,
             place=Place.parse(obj["place"]) if obj.get("place") else None,
             coordinates=Coordinates.parse(obj),
             inReplyToTweetId=int_or_none(obj, "in_reply_to_status_id_str"),
             inReplyToUser=_get_reply_user(obj, res),
@@ -327,7 +331,17 @@
 
 
 def _get_source_label(tw_obj: dict):
     source = tw_obj.get("source", None)
     if source and (match := re.search(r">([^<]*)<", source)):
         return str(match.group(1))
     return None
+
+
+def _parse_links(obj: dict, paths: list[str]):
+    links = []
+    for x in paths:
+        links.extend(get_or(obj, x, []))
+
+    links = [TextLink.parse(x) for x in links]
+    links = [x for x in links if x is not None]
+    return links
```

### Comparing `twscrape-0.3.0/twscrape/queue_client.py` & `twscrape-0.4.0/twscrape/queue_client.py`

 * *Files 5% similar despite different names*

```diff
@@ -107,17 +107,17 @@
                 if rep.status_code == 429:
                     logger.debug(f"Rate limit for {log_id}")
                     reset_ts = int(rep.headers.get("x-rate-limit-reset", 0))
                     await self.pool.lock_until(ctx.acc.username, self.queue, reset_ts)
                     continue
 
                 # possible account banned
-                if rep.status_code == 403:
-                    logger.warning(f"403 for {log_id}")
+                if rep.status_code in (401, 403):
                     reset_ts = utc_ts() + 60 * 60  # + 1 hour
+                    logger.warning(f"Code {rep.status_code} for {log_id} – frozen for 1h")
                     await self.pool.lock_until(ctx.acc.username, self.queue, reset_ts)
                     continue
 
                 # twitter can return different types of cursors that not transfers between accounts
                 # just take the next account, the current cursor can work in it
                 if rep.status_code == 400:
                     logger.debug(f"Cursor not valid for {log_id}")
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `twscrape-0.3.0/twscrape/utils.py` & `twscrape-0.4.0/twscrape/utils.py`

 * *Files identical despite different names*

### Comparing `twscrape-0.3.0/.gitignore` & `twscrape-0.4.0/.gitignore`

 * *Files identical despite different names*

### Comparing `twscrape-0.3.0/LICENSE` & `twscrape-0.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `twscrape-0.3.0/pyproject.toml` & `twscrape-0.4.0/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "twscrape"
-version = "0.3.0"
+version = "0.4.0"
 authors = [{name = "vladkens", email = "v.pronsky@gmail.com"}]
 description = "Twitter GraphQL and Search API implementation with SNScrape data models"
 readme = "readme.md"
 requires-python = ">=3.10"
 keywords = ["twitter", "scrape", "scrapper", "api", "snscrape"]
 license = {text = "MIT"}
 classifiers = [
```

### Comparing `twscrape-0.3.0/readme.md` & `twscrape-0.4.0/readme.md`

 * *Files identical despite different names*

### Comparing `twscrape-0.3.0/PKG-INFO` & `twscrape-0.4.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: twscrape
-Version: 0.3.0
+Version: 0.4.0
 Summary: Twitter GraphQL and Search API implementation with SNScrape data models
 Project-URL: repository, https://github.com/vladkens/twscrape
 Author-email: vladkens <v.pronsky@gmail.com>
 License: MIT
 License-File: LICENSE
 Keywords: api,scrape,scrapper,snscrape,twitter
 Classifier: Development Status :: 4 - Beta
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: twscrape Version: 0.3.0 Summary: Twitter GraphQL
+Metadata-Version: 2.1 Name: twscrape Version: 0.4.0 Summary: Twitter GraphQL
 and Search API implementation with SNScrape data models Project-URL:
 repository, https://github.com/vladkens/twscrape Author-email: vladkens
 pronsky@gmail.com> License: MIT License-File: LICENSE Keywords:
 api,scrape,scrapper,snscrape,twitter Classifier: Development Status :: 4 - Beta
 Classifier: License :: OSI Approved :: MIT License Classifier: Programming
 Language :: Python :: 3.10 Classifier: Programming Language :: Python :: 3.11
 Requires-Python: >=3.10 Requires-Dist: aiosqlite==0.17.0 Requires-Dist: fake-
```

