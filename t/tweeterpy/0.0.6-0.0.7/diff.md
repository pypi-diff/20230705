# Comparing `tmp/tweeterpy-0.0.6.tar.gz` & `tmp/tweeterpy-0.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tweeterpy-0.0.6.tar", last modified: Tue Jul  4 18:54:35 2023, max compression
+gzip compressed data, was "tweeterpy-0.0.7.tar", last modified: Wed Jul  5 07:03:51 2023, max compression
```

## Comparing `tweeterpy-0.0.6.tar` & `tweeterpy-0.0.7.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxrwxrwx   0        0        0        0 2023-07-04 18:54:35.091717 tweeterpy-0.0.6/
--rw-rw-rw-   0        0        0     1093 2023-05-19 18:11:22.000000 tweeterpy-0.0.6/LICENSE
--rw-rw-rw-   0        0        0       22 2023-06-20 15:06:14.000000 tweeterpy-0.0.6/MANIFEST.in
--rw-rw-rw-   0        0        0     3389 2023-07-04 18:54:35.076105 tweeterpy-0.0.6/PKG-INFO
--rw-rw-rw-   0        0        0     2336 2023-06-22 07:42:40.000000 tweeterpy-0.0.6/README.md
--rw-rw-rw-   0        0        0       42 2023-07-04 18:54:35.091717 tweeterpy-0.0.6/setup.cfg
--rw-rw-rw-   0        0        0     1499 2023-07-04 18:54:07.000000 tweeterpy-0.0.6/setup.py
-drwxrwxrwx   0        0        0        0 2023-07-04 18:54:35.076105 tweeterpy-0.0.6/tweeterpy/
--rw-rw-rw-   0        0        0       34 2023-06-20 15:09:15.000000 tweeterpy-0.0.6/tweeterpy/__init__.py
--rw-rw-rw-   0        0        0     4037 2023-06-28 13:39:17.000000 tweeterpy-0.0.6/tweeterpy/api_util.py
--rw-rw-rw-   0        0        0      671 2023-06-25 06:51:11.000000 tweeterpy-0.0.6/tweeterpy/config.py
--rw-rw-rw-   0        0        0     2635 2023-06-28 13:44:31.000000 tweeterpy-0.0.6/tweeterpy/constants.py
--rw-rw-rw-   0        0        0     6654 2023-06-24 14:06:58.000000 tweeterpy-0.0.6/tweeterpy/login_util.py
--rw-rw-rw-   0        0        0     1653 2023-06-20 07:35:05.000000 tweeterpy-0.0.6/tweeterpy/request_util.py
--rw-rw-rw-   0        0        0     2278 2023-06-25 06:51:11.000000 tweeterpy-0.0.6/tweeterpy/session_util.py
--rw-rw-rw-   0        0        0    23036 2023-06-28 13:57:16.000000 tweeterpy-0.0.6/tweeterpy/tweeterpy.py
--rw-rw-rw-   0        0        0     3593 2023-06-28 07:54:04.000000 tweeterpy-0.0.6/tweeterpy/util.py
-drwxrwxrwx   0        0        0        0 2023-07-04 18:54:35.076105 tweeterpy-0.0.6/tweeterpy.egg-info/
--rw-rw-rw-   0        0        0     3389 2023-07-04 18:54:34.000000 tweeterpy-0.0.6/tweeterpy.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      406 2023-07-04 18:54:34.000000 tweeterpy-0.0.6/tweeterpy.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-04 18:54:34.000000 tweeterpy-0.0.6/tweeterpy.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      221 2023-07-04 18:54:34.000000 tweeterpy-0.0.6/tweeterpy.egg-info/requires.txt
--rw-rw-rw-   0        0        0       10 2023-07-04 18:54:34.000000 tweeterpy-0.0.6/tweeterpy.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-07-05 07:03:51.627701 tweeterpy-0.0.7/
+-rw-rw-rw-   0        0        0     1093 2023-05-19 18:11:22.000000 tweeterpy-0.0.7/LICENSE
+-rw-rw-rw-   0        0        0       22 2023-06-20 15:06:14.000000 tweeterpy-0.0.7/MANIFEST.in
+-rw-rw-rw-   0        0        0     3389 2023-07-05 07:03:51.627701 tweeterpy-0.0.7/PKG-INFO
+-rw-rw-rw-   0        0        0     2336 2023-06-22 07:42:40.000000 tweeterpy-0.0.7/README.md
+-rw-rw-rw-   0        0        0       42 2023-07-05 07:03:51.627701 tweeterpy-0.0.7/setup.cfg
+-rw-rw-rw-   0        0        0     1499 2023-07-05 06:59:08.000000 tweeterpy-0.0.7/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-05 07:03:51.612062 tweeterpy-0.0.7/tweeterpy/
+-rw-rw-rw-   0        0        0       34 2023-06-20 15:09:15.000000 tweeterpy-0.0.7/tweeterpy/__init__.py
+-rw-rw-rw-   0        0        0     4037 2023-06-28 13:39:17.000000 tweeterpy-0.0.7/tweeterpy/api_util.py
+-rw-rw-rw-   0        0        0      671 2023-06-25 06:51:11.000000 tweeterpy-0.0.7/tweeterpy/config.py
+-rw-rw-rw-   0        0        0     2784 2023-07-05 06:41:31.000000 tweeterpy-0.0.7/tweeterpy/constants.py
+-rw-rw-rw-   0        0        0     6654 2023-06-24 14:06:58.000000 tweeterpy-0.0.7/tweeterpy/login_util.py
+-rw-rw-rw-   0        0        0     1653 2023-06-20 07:35:05.000000 tweeterpy-0.0.7/tweeterpy/request_util.py
+-rw-rw-rw-   0        0        0     2278 2023-06-25 06:51:11.000000 tweeterpy-0.0.7/tweeterpy/session_util.py
+-rw-rw-rw-   0        0        0    24985 2023-07-05 06:58:56.000000 tweeterpy-0.0.7/tweeterpy/tweeterpy.py
+-rw-rw-rw-   0        0        0     3593 2023-06-28 07:54:04.000000 tweeterpy-0.0.7/tweeterpy/util.py
+drwxrwxrwx   0        0        0        0 2023-07-05 07:03:51.627701 tweeterpy-0.0.7/tweeterpy.egg-info/
+-rw-rw-rw-   0        0        0     3389 2023-07-05 07:03:51.000000 tweeterpy-0.0.7/tweeterpy.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      406 2023-07-05 07:03:51.000000 tweeterpy-0.0.7/tweeterpy.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-05 07:03:51.000000 tweeterpy-0.0.7/tweeterpy.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      221 2023-07-05 07:03:51.000000 tweeterpy-0.0.7/tweeterpy.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       10 2023-07-05 07:03:51.000000 tweeterpy-0.0.7/tweeterpy.egg-info/top_level.txt
```

### Comparing `tweeterpy-0.0.6/LICENSE` & `tweeterpy-0.0.7/LICENSE`

 * *Files identical despite different names*

### Comparing `tweeterpy-0.0.6/PKG-INFO` & `tweeterpy-0.0.7/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tweeterpy
-Version: 0.0.6
+Version: 0.0.7
 Summary: TweeterPy is a python library to extract data from Twitter. TweeterPy API lets you scrape data from a user's profile like username, userid, bio, followers/followings list, profile media, tweets, etc.
 Home-page: https://github.com/iSarabjitDhiman/TweeterPy
 Author: Sarabjit Dhiman
 Author-email: hello@sarabjitdhiman.com
 License: MIT
 Keywords: tweeterpy,twitter scraper,tweet scraper,twitter data extraction,twitter api,twitter python,tweet api,tweetpy
 Classifier: Development Status :: 3 - Alpha
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: tweeterpy Version: 0.0.6 Summary: TweeterPy is a
+Metadata-Version: 2.1 Name: tweeterpy Version: 0.0.7 Summary: TweeterPy is a
 python library to extract data from Twitter. TweeterPy API lets you scrape data
 from a user's profile like username, userid, bio, followers/followings list,
 profile media, tweets, etc. Home-page: https://github.com/iSarabjitDhiman/
 TweeterPy Author: Sarabjit Dhiman Author-email: hello@sarabjitdhiman.com
 License: MIT Keywords: tweeterpy,twitter scraper,tweet scraper,twitter data
 extraction,twitter api,twitter python,tweet api,tweetpy Classifier: Development
 Status :: 3 - Alpha Classifier: Intended Audience :: End Users/Desktop
```

### Comparing `tweeterpy-0.0.6/README.md` & `tweeterpy-0.0.7/README.md`

 * *Files identical despite different names*

### Comparing `tweeterpy-0.0.6/setup.py` & `tweeterpy-0.0.7/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from setuptools import setup
 
-VERSION = "0.0.6"
+VERSION = "0.0.7"
 SHORT_DESCRIPTION = "TweeterPy is a python library to extract data from Twitter. TweeterPy API lets you scrape data from a user's profile like username, userid, bio, followers/followings list, profile media, tweets, etc."
 
 with open("requirements.txt") as file:
     dependencies = file.read().splitlines()
 with open("README.md", "r") as file:
     DESCRIPTION = file.read()
```

### Comparing `tweeterpy-0.0.6/tweeterpy/api_util.py` & `tweeterpy-0.0.7/tweeterpy/api_util.py`

 * *Files identical despite different names*

### Comparing `tweeterpy-0.0.6/tweeterpy/config.py` & `tweeterpy-0.0.7/tweeterpy/config.py`

 * *Files identical despite different names*

### Comparing `tweeterpy-0.0.6/tweeterpy/constants.py` & `tweeterpy-0.0.7/tweeterpy/constants.py`

 * *Files 12% similar despite different names*

```diff
@@ -18,14 +18,16 @@
     USER_ID_ENDPOINT = "9zwVLJ48lmVUk8u_Gh9DmA/ProfileSpotlightsQuery"
     USER_INFO_ENDPOINT = "8slyDObmnUzBOCu7kYZj_A/UserByRestId"
     USER_DATA_ENDPOINT = "qRednkZG-rn1P6b48NINmQ/UserByScreenName"
     MULTIPLE_USERS_DATA_ENDPOINT = "GD4q8bBE2i6cqWw2iT74Gg/UsersByRestIds"
     USER_MEDIA_ENDPOINT = "wlwQkva3Zii3b8CJjXSBCw/UserMedia"
     USER_TWEETS_ENDPOINT = "NPgNFbBEhFTul68weP-tYg/UserTweets"
     USER_TWEETS_AND_REPLIES_ENDPOINT = "2dNLofLWl-u8EQPURIAp9w/UserTweetsAndReplies"
+    TWEETS_LIST_ENDPOINT = "2Vjeyo_L0nizAUhHe3fKyA/ListLatestTweetsTimeline"
+    TOPIC_TWEETS_ENDPOINT = "KDCkc4PZY-sCy_L-scQImw/TopicLandingPage"
     TWEET_DETAILS_ENDPOINT = "Pn68XRZwyV9ClrAEmK8rrQ/TweetDetail"
     VIEWER_ENDPOINT = "k3027HdkVqbuDPpdoniLKA/Viewer"
     SEARCH_ENDPOINT = "IOJ89SDQ9IrZ2t7hSD4Fdg/SearchTimeline"
     FOLLOWERS_ENDPOINT = "WWFQL1d4gxtqm2mjZCRa-Q/Followers"
     FOLLOWINGS_ENDPOINT = "OLcddmNLPVXGDgSdSVj0ow/Following"
     MUTUAL_FOLLOWERS_ENDPOINT = "wYAUyD58y1AFol2g2bLqzw/FollowersYouKnow"
     LIKED_TWEETS_ENDPOINT = "QPKcH_nml6UIOxHLjmNsuw/Likes"
```

### Comparing `tweeterpy-0.0.6/tweeterpy/login_util.py` & `tweeterpy-0.0.7/tweeterpy/login_util.py`

 * *Files identical despite different names*

### Comparing `tweeterpy-0.0.6/tweeterpy/request_util.py` & `tweeterpy-0.0.7/tweeterpy/request_util.py`

 * *Files identical despite different names*

### Comparing `tweeterpy-0.0.6/tweeterpy/session_util.py` & `tweeterpy-0.0.7/tweeterpy/session_util.py`

 * *Files identical despite different names*

### Comparing `tweeterpy-0.0.6/tweeterpy/tweeterpy.py` & `tweeterpy-0.0.7/tweeterpy/tweeterpy.py`

 * *Files 5% similar despite different names*

```diff
@@ -225,14 +225,29 @@
         """
         variables = {"screen_name": username, "withSafetyModeUserFields": True}
         url, query_params = self._generate_request_data(
             Path.USER_DATA_ENDPOINT, variables, user_info_feautres=True)
         response = make_request(url, params=query_params)
         return response['data']['user']['result']
 
+    def get_multiple_users_data(self, user_ids):
+        """Get user information of multiple twitter users.
+
+        Args:
+            user_ids (list): List of twitter users' IDs.
+
+        Returns:
+            list: Multiple users data.
+        """
+        variables = {"userIds": user_ids}
+        url, query_params = self._generate_request_data(
+            Path.MULTIPLE_USERS_DATA_ENDPOINT, variables, default_features=True)
+        response = make_request(url, params=query_params)
+        return response['data']['users']
+
     def get_user_tweets(self, user_id, with_replies=False, end_cursor=None, total=None):
         """Get Tweets from a user's profile.
 
         Args:
             user_id (int): User ID.
             with_replies (bool, optional): Set to True if want to get the tweets user replied to, from user's profile page. Defaults to False.
             end_cursor (str, optional): Last endcursor point. (To start from where you left off last time). Defaults to None.
@@ -342,28 +357,49 @@
         variables = {"count": 40, "includePromotedContent": True,
                      "latestControlAvailable": True, "withCommunity": True}
         url, query_params = self._generate_request_data(
             Path.HOME_TIMELINE_ENDPOINT, variables, additional_features=True)
         data_path = ('data', 'home', 'home_timeline_urt', 'instructions')
         return self._handle_pagination(url, query_params, end_cursor=end_cursor, data_path=data_path, total=total)
 
-    def get_multiple_users_data(self, user_ids):
-        """Get user information of multiple twitter users.
+    def get_list_tweets(self, list_id, end_cursor=None, total=None):
+        """Get tweets from a Tweets List.
 
         Args:
-            user_ids (list): List of twitter users' IDs.
+            list_id (str/int): Tweets List ID. (Can be extracted from twitter mobile app.)
+            end_cursor (str, optional): Last endcursor point. (To start from where you left off last time). Defaults to None.
+            total (int, optional): Total(Max) number of results you want to get. If None, extracts all results. Defaults to None.
 
         Returns:
-            list: Multiple users data.
+            dict: Returns data, cursor_endpoint, has_next_page
         """
-        variables = {"userIds": user_ids}
+        variables = {"listId": list_id, "count": 100}
         url, query_params = self._generate_request_data(
-            Path.MULTIPLE_USERS_DATA_ENDPOINT, variables, default_features=True)
-        response = make_request(url, params=query_params)
-        return response['data']['users']
+            Path.TWEETS_LIST_ENDPOINT, variables, additional_features=True)
+        data_path = ('data', 'list', 'tweets_timeline',
+                     'timeline', 'instructions')
+        return self._handle_pagination(url, query_params, end_cursor=end_cursor, data_path=data_path, total=total)
+
+    def get_topic_tweets(self, topic_id, end_cursor=None, total=None):
+        """Get tweets from a Topic.
+
+        Args:
+            topic_id (str/int): Topic ID.
+            end_cursor (str, optional): Last endcursor point. (To start from where you left off last time). Defaults to None.
+            total (int, optional): Total(Max) number of results you want to get. If None, extracts all results. Defaults to None.
+
+        Returns:
+            dict: Returns data, cursor_endpoint, has_next_page
+        """
+        variables = {"rest_id": topic_id, "count": 100}
+        url, query_params = self._generate_request_data(
+            Path.TOPIC_TWEETS_ENDPOINT, variables, additional_features=True)
+        data_path = ('data', 'topic_by_rest_id', 'topic_page',
+                     'body', 'timeline', 'instructions')
+        return self._handle_pagination(url, query_params, end_cursor=end_cursor, data_path=data_path, total=total)
 
     def search(self, search_query, end_cursor=None, total=None, search_filter=None):
         """Get search results.
 
         Args:
             search_query (str): Search term.
             end_cursor (str, optional): Last endcursor point. (To start from where you left off last time). Defaults to None.
```

### Comparing `tweeterpy-0.0.6/tweeterpy/util.py` & `tweeterpy-0.0.7/tweeterpy/util.py`

 * *Files identical despite different names*

### Comparing `tweeterpy-0.0.6/tweeterpy.egg-info/PKG-INFO` & `tweeterpy-0.0.7/tweeterpy.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tweeterpy
-Version: 0.0.6
+Version: 0.0.7
 Summary: TweeterPy is a python library to extract data from Twitter. TweeterPy API lets you scrape data from a user's profile like username, userid, bio, followers/followings list, profile media, tweets, etc.
 Home-page: https://github.com/iSarabjitDhiman/TweeterPy
 Author: Sarabjit Dhiman
 Author-email: hello@sarabjitdhiman.com
 License: MIT
 Keywords: tweeterpy,twitter scraper,tweet scraper,twitter data extraction,twitter api,twitter python,tweet api,tweetpy
 Classifier: Development Status :: 3 - Alpha
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: tweeterpy Version: 0.0.6 Summary: TweeterPy is a
+Metadata-Version: 2.1 Name: tweeterpy Version: 0.0.7 Summary: TweeterPy is a
 python library to extract data from Twitter. TweeterPy API lets you scrape data
 from a user's profile like username, userid, bio, followers/followings list,
 profile media, tweets, etc. Home-page: https://github.com/iSarabjitDhiman/
 TweeterPy Author: Sarabjit Dhiman Author-email: hello@sarabjitdhiman.com
 License: MIT Keywords: tweeterpy,twitter scraper,tweet scraper,twitter data
 extraction,twitter api,twitter python,tweet api,tweetpy Classifier: Development
 Status :: 3 - Alpha Classifier: Intended Audience :: End Users/Desktop
```

