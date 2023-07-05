# Comparing `tmp/sopel-twitter-1.1.0.tar.gz` & `tmp/sopel-twitter-1.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sopel-twitter-1.1.0.tar", last modified: Fri May 26 05:20:25 2023, max compression
+gzip compressed data, was "sopel-twitter-1.2.0.tar", last modified: Wed Jul  5 15:51:47 2023, max compression
```

## Comparing `sopel-twitter-1.1.0.tar` & `sopel-twitter-1.2.0.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxr-xr-x   0 dgw       (1000) dgw       (1000)        0 2023-05-26 05:20:25.428260 sopel-twitter-1.1.0/
--rw-r--r--   0 dgw       (1000) dgw       (1000)     1022 2022-03-02 18:17:04.000000 sopel-twitter-1.1.0/COPYING
--rw-r--r--   0 dgw       (1000) dgw       (1000)      161 2023-04-29 21:04:00.000000 sopel-twitter-1.1.0/MANIFEST.in
--rw-r--r--   0 dgw       (1000) dgw       (1000)     2634 2023-05-18 04:45:03.000000 sopel-twitter-1.1.0/NEWS
--rw-r--r--   0 dgw       (1000) dgw       (1000)     4506 2023-05-26 05:20:25.428760 sopel-twitter-1.1.0/PKG-INFO
--rw-r--r--   0 dgw       (1000) dgw       (1000)     1298 2023-04-29 21:04:00.000000 sopel-twitter-1.1.0/README.md
--rw-r--r--   0 dgw       (1000) dgw       (1000)        0 2023-04-29 21:04:00.000000 sopel-twitter-1.1.0/dev-requirements.txt
--rw-r--r--   0 dgw       (1000) dgw       (1000)      694 2023-05-26 05:20:25.431258 sopel-twitter-1.1.0/setup.cfg
--rwxr-xr-x   0 dgw       (1000) dgw       (1000)      889 2023-04-29 21:04:00.000000 sopel-twitter-1.1.0/setup.py
-drwxr-xr-x   0 dgw       (1000) dgw       (1000)        0 2023-05-26 05:20:25.376254 sopel-twitter-1.1.0/sopel_twitter/
--rw-r--r--   0 dgw       (1000) dgw       (1000)     8920 2023-05-26 05:18:02.000000 sopel-twitter-1.1.0/sopel_twitter/__init__.py
-drwxr-xr-x   0 dgw       (1000) dgw       (1000)        0 2023-05-26 05:20:25.411759 sopel-twitter-1.1.0/sopel_twitter.egg-info/
--rw-r--r--   0 dgw       (1000) dgw       (1000)     4506 2023-05-26 05:20:24.000000 sopel-twitter-1.1.0/sopel_twitter.egg-info/PKG-INFO
--rw-r--r--   0 dgw       (1000) dgw       (1000)      400 2023-05-26 05:20:24.000000 sopel-twitter-1.1.0/sopel_twitter.egg-info/SOURCES.txt
--rw-r--r--   0 dgw       (1000) dgw       (1000)        1 2023-05-26 05:20:24.000000 sopel-twitter-1.1.0/sopel_twitter.egg-info/dependency_links.txt
--rw-r--r--   0 dgw       (1000) dgw       (1000)       40 2023-05-26 05:20:24.000000 sopel-twitter-1.1.0/sopel_twitter.egg-info/entry_points.txt
--rw-r--r--   0 dgw       (1000) dgw       (1000)        1 2023-04-15 21:13:31.000000 sopel-twitter-1.1.0/sopel_twitter.egg-info/not-zip-safe
--rw-r--r--   0 dgw       (1000) dgw       (1000)       31 2023-05-26 05:20:24.000000 sopel-twitter-1.1.0/sopel_twitter.egg-info/requires.txt
--rw-r--r--   0 dgw       (1000) dgw       (1000)       20 2023-05-26 05:20:24.000000 sopel-twitter-1.1.0/sopel_twitter.egg-info/top_level.txt
-drwxr-xr-x   0 dgw       (1000) dgw       (1000)        0 2023-05-26 05:20:25.427262 sopel-twitter-1.1.0/tests/
--rw-r--r--   0 dgw       (1000) dgw       (1000)       15 2023-04-29 21:04:00.000000 sopel-twitter-1.1.0/tests/__init__.py
--rw-r--r--   0 dgw       (1000) dgw       (1000)      296 2023-04-29 21:04:00.000000 sopel-twitter-1.1.0/tests/test_twitter.py
+drwxr-xr-x   0 dgw       (1000) dgw       (1000)        0 2023-07-05 15:51:47.229837 sopel-twitter-1.2.0/
+-rw-r--r--   0 dgw       (1000) dgw       (1000)     1022 2022-03-02 18:17:04.000000 sopel-twitter-1.2.0/COPYING
+-rw-r--r--   0 dgw       (1000) dgw       (1000)      161 2023-04-29 21:04:00.000000 sopel-twitter-1.2.0/MANIFEST.in
+-rw-r--r--   0 dgw       (1000) dgw       (1000)     2795 2023-07-05 15:50:39.000000 sopel-twitter-1.2.0/NEWS
+-rw-r--r--   0 dgw       (1000) dgw       (1000)     5403 2023-07-05 15:51:47.229837 sopel-twitter-1.2.0/PKG-INFO
+-rw-r--r--   0 dgw       (1000) dgw       (1000)     2034 2023-07-05 15:50:27.000000 sopel-twitter-1.2.0/README.md
+-rw-r--r--   0 dgw       (1000) dgw       (1000)        0 2023-04-29 21:04:00.000000 sopel-twitter-1.2.0/dev-requirements.txt
+-rw-r--r--   0 dgw       (1000) dgw       (1000)      694 2023-07-05 15:51:47.236836 sopel-twitter-1.2.0/setup.cfg
+-rwxr-xr-x   0 dgw       (1000) dgw       (1000)      889 2023-04-29 21:04:00.000000 sopel-twitter-1.2.0/setup.py
+drwxr-xr-x   0 dgw       (1000) dgw       (1000)        0 2023-07-05 15:51:47.169837 sopel-twitter-1.2.0/sopel_twitter/
+-rw-r--r--   0 dgw       (1000) dgw       (1000)     9836 2023-07-05 15:50:27.000000 sopel-twitter-1.2.0/sopel_twitter/__init__.py
+drwxr-xr-x   0 dgw       (1000) dgw       (1000)        0 2023-07-05 15:51:47.208845 sopel-twitter-1.2.0/sopel_twitter.egg-info/
+-rw-r--r--   0 dgw       (1000) dgw       (1000)     5403 2023-07-05 15:51:46.000000 sopel-twitter-1.2.0/sopel_twitter.egg-info/PKG-INFO
+-rw-r--r--   0 dgw       (1000) dgw       (1000)      400 2023-07-05 15:51:46.000000 sopel-twitter-1.2.0/sopel_twitter.egg-info/SOURCES.txt
+-rw-r--r--   0 dgw       (1000) dgw       (1000)        1 2023-07-05 15:51:46.000000 sopel-twitter-1.2.0/sopel_twitter.egg-info/dependency_links.txt
+-rw-r--r--   0 dgw       (1000) dgw       (1000)       40 2023-07-05 15:51:46.000000 sopel-twitter-1.2.0/sopel_twitter.egg-info/entry_points.txt
+-rw-r--r--   0 dgw       (1000) dgw       (1000)        1 2023-04-15 21:13:31.000000 sopel-twitter-1.2.0/sopel_twitter.egg-info/not-zip-safe
+-rw-r--r--   0 dgw       (1000) dgw       (1000)       31 2023-07-05 15:51:46.000000 sopel-twitter-1.2.0/sopel_twitter.egg-info/requires.txt
+-rw-r--r--   0 dgw       (1000) dgw       (1000)       20 2023-07-05 15:51:46.000000 sopel-twitter-1.2.0/sopel_twitter.egg-info/top_level.txt
+drwxr-xr-x   0 dgw       (1000) dgw       (1000)        0 2023-07-05 15:51:47.226845 sopel-twitter-1.2.0/tests/
+-rw-r--r--   0 dgw       (1000) dgw       (1000)       15 2023-04-29 21:04:00.000000 sopel-twitter-1.2.0/tests/__init__.py
+-rw-r--r--   0 dgw       (1000) dgw       (1000)      296 2023-04-29 21:04:00.000000 sopel-twitter-1.2.0/tests/test_twitter.py
```

### Comparing `sopel-twitter-1.1.0/COPYING` & `sopel-twitter-1.2.0/COPYING`

 * *Files identical despite different names*

### Comparing `sopel-twitter-1.1.0/NEWS` & `sopel-twitter-1.2.0/NEWS`

 * *Files 9% similar despite different names*

```diff
@@ -1,7 +1,17 @@
+Changes between 1.1.0 and 1.2.0
+===============================
+
+Breaking:
+* **Twitter cookies are now required**
+
+Changed:
+* Updated to `tweety-ns` 0.8 (#48)
+
+
 Changes between 1.0.1 and 1.1.0
 ===============================
 
 Changed:
 * Updated to `tweety-ns` 0.7, including revamped exceptions (#46)
```

### Comparing `sopel-twitter-1.1.0/PKG-INFO` & `sopel-twitter-1.2.0/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sopel-twitter
-Version: 1.1.0
+Version: 1.2.0
 Summary: A Twitter plugin for Sopel
 Home-page: https://github.com/sopel-irc/sopel-twitter
 Author: dgw
 Author-email: dgw@technobabbl.es
 License: Eiffel Forum License, version 2
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: System Administrators
@@ -27,32 +27,45 @@
 ```
 
 If you want to use the development version, simply clone the repository and use
 `pip install path/to/sopel-twitter`
 
 ## Configuring
 
-The easiest way to configure `sopel-twitter` is using Sopel's configuration
-wizard – simply run `sopel-plugins configure twitter` and enter the
-credentials for the Twitter application you created.
+**Twitter cookies are required to use this plugin** as of 1 July 2023. You may
+want to minimize the risk of adverse action by using a throwaway login instead
+of your real profile; however, note that doing so will affect the rate limit
+available to this plugin.
+
+The easiest way to configure `sopel-twitter` is via Sopel's configuration
+wizard – simply run `sopel-plugins configure twitter` and enter the cookie
+values for which it prompts you.
 
 Otherwise, you can edit your bot's configuration file:
 
 ```ini
 [twitter]
+cookies =
+    auth_token=df4c7364f4fac2b3843904ecc566b0e1accdf98b;
+    ct0=23f96509cba936b732cd39e171dce0fa5da9ecd1d7f3551258fe3e1a21da79a797e80496e8190613ba8a8ebc07ef6d8004b17518e84f9b6f8100738c5243a3da3139c87a5a55e46d70ed99cf0f068a23
+# Required: Cookies from Twitter
+# Newlines are not required, but the semicolon (;) very much is!
+# You will have to pull this from your own logged-in account; rate limits will
+# vary depending on the account's verification/Blue status.
+
 show_quoted_tweets = True
 # Optional: For quote-tweets, send a second message showing the quoted tweet?
 # Default: True
 
 alternate_domains =
     fxtwitter.com
     vxtwitter.com
     nitter.net
 # Optional: What other domains should we treat like twitter domains?
-# Default: vxtwitter.com, nitter.net
+# Default: fxtwitter.com, vxtwitter.com, nitter.net
 ```
 
 ## Usage
 
 Just send a link to a tweet or profile!
 
 You can also retrieve a user's info with the `.twitinfo` command:
@@ -61,14 +74,24 @@
 < Wiz> .twitinfo NASA
 < Sopel> [Twitter] NASA (@NASA) ✔️ | Pale Blue Dot | http://www.nasa.gov/
          | 204 friends, 46,602,251 followers | 65,377 tweets, 13,040 ♥s
          | Joined: 2007-12-19 - 20:20:32UTC | There's space for everybody. ✨
 ```
 
 
+Changes between 1.1.0 and 1.2.0
+===============================
+
+Breaking:
+* **Twitter cookies are now required**
+
+Changed:
+* Updated to `tweety-ns` 0.8 (#48)
+
+
 Changes between 1.0.1 and 1.1.0
 ===============================
 
 Changed:
 * Updated to `tweety-ns` 0.7, including revamped exceptions (#46)
```

### Comparing `sopel-twitter-1.1.0/setup.cfg` & `sopel-twitter-1.2.0/setup.cfg`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = sopel-twitter
-version = 1.1.0
+version = 1.2.0
 description = A Twitter plugin for Sopel
 author = dgw
 author_email = dgw@technobabbl.es
 url = https://github.com/sopel-irc/sopel-twitter
 license = Eiffel Forum License, version 2
 classifiers = 
 	Intended Audience :: Developers
@@ -15,15 +15,15 @@
 
 [options]
 packages = find:
 zip_safe = false
 include_package_data = true
 install_requires = 
 	sopel>=7.1,<9
-	tweety-ns~=0.7.1
+	tweety-ns~=0.8.0
 
 [options.entry_points]
 sopel.plugins = 
 	twitter = sopel_twitter
 
 [egg_info]
 tag_build =
```

### Comparing `sopel-twitter-1.1.0/setup.py` & `sopel-twitter-1.2.0/setup.py`

 * *Files identical despite different names*

### Comparing `sopel-twitter-1.1.0/sopel_twitter/__init__.py` & `sopel-twitter-1.2.0/sopel_twitter/__init__.py`

 * *Files 6% similar despite different names*

```diff
@@ -12,35 +12,41 @@
 from tweety.bot import Twitter
 from tweety import exceptions_ as tweety_errors
 
 from sopel import plugin, tools
 from sopel.config.types import (
     BooleanAttribute,
     ListAttribute,
+    NO_DEFAULT,
     StaticSection,
+    ValidatedAttribute,
 )
 
 logger = tools.get_logger('twitter')
 
 DOMAIN_REGEX = r"https?://(?:m(?:obile)?\.)?twitter\.com/"
 STATUS_REGEX = r"(?:\w+|i/web)/status/(?P<status>\d+)"
 USER_REGEX = r"(?P<user>\w+)/?(?:\?.*)?$"
 NEWLINE_RUN_REGEX = re.compile(r"\s*\n[\n\s]*")
 
 
 class TwitterSection(StaticSection):
+    cookies = ValidatedAttribute('cookies', default=NO_DEFAULT)
     show_quoted_tweets = BooleanAttribute('show_quoted_tweets', default=True)
     alternate_domains = ListAttribute(
         "alternate_domains",
         default=["vxtwitter.com", "nitter.net"],
     )
 
 
 def configure(config):
     config.define_section('twitter', TwitterSection, validate=False)
+    tok = input('REQUIRED: Twitter auth_token cookie value: ')
+    ct0 = input('REQUIRED: Twitter ct0 cookie value: ')
+    config.twitter.cookies = 'auth_token={};ct0={}'.format(tok, ct0)
     config.twitter.configure_setting(
         'show_quoted_tweets', 'When a tweet quotes another status, '
         'show the quoted tweet on a second IRC line?')
 
 
 def setup(bot):
     bot.config.define_section('twitter', TwitterSection)
@@ -175,18 +181,24 @@
         return plugin.NOLIMIT
 
     output_user(bot, trigger, trigger.group(3))
 
 
 def output_status(bot, trigger, id_):
     try:
-        tweet = Twitter().tweet_detail(id_)
+        tweet = Twitter(cookies=bot.settings.twitter.cookies).tweet_detail(id_)
+    except tweety_errors.InvalidCredentials:
+        bot.say("Incorrect plugin configuration. Please ask my owner to set correct cookies.")
+        return
     except tweety_errors.AuthenticationRequired:
         bot.say("That content requires authentication; sorry!")
         return
+    except tweety_errors.RateLimitReached:
+        bot.say("Rate limit reached. Please try again later.")
+        return
     except tweety_errors.InvalidTweetIdentifier:
         bot.say("Couldn't fetch that tweet. It's probably private, 18+ flagged, or deleted.")
         return
     except (
         tweety_errors.GuestTokenNotFound,
         tweety_errors.InvalidCredentials,
         tweety_errors.ProxyParseError,
@@ -212,24 +224,30 @@
                                 RTs=tweet.retweet_counts,
                                 hearts=tweet.likes,
                                 posted=format_time(bot, trigger, tweet.created_on)))
 
 
 def output_user(bot, trigger, sn):
     try:
-        user = Twitter().get_user_info(sn)
+        user = Twitter(cookies=bot.settings.twitter.cookies).get_user_info(sn)
+    except tweety_errors.InvalidCredentials:
+        bot.say("Incorrect plugin configuration. Please ask my owner to set correct cookies.")
+        return
     except tweety_errors.UserNotFound:
         bot.say("User not found.")
         return
     except tweety_errors.UserProtected:
         bot.say("User profile is protected.")
         return
     except tweety_errors.AuthenticationRequired:
         bot.say("That content requires authentication; sorry!")
         return
+    except tweety_errors.RateLimitReached:
+        bot.say("Rate limit reached. Please try again later.")
+        return
     except (
         tweety_errors.GuestTokenNotFound,
         tweety_errors.InvalidCredentials,
         tweety_errors.ProxyParseError,
         tweety_errors.UnknownError,
     ):
         bot.say("Can't access Twitter data. Please try again later.")
```

### Comparing `sopel-twitter-1.1.0/sopel_twitter.egg-info/PKG-INFO` & `sopel-twitter-1.2.0/sopel_twitter.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sopel-twitter
-Version: 1.1.0
+Version: 1.2.0
 Summary: A Twitter plugin for Sopel
 Home-page: https://github.com/sopel-irc/sopel-twitter
 Author: dgw
 Author-email: dgw@technobabbl.es
 License: Eiffel Forum License, version 2
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: System Administrators
@@ -27,32 +27,45 @@
 ```
 
 If you want to use the development version, simply clone the repository and use
 `pip install path/to/sopel-twitter`
 
 ## Configuring
 
-The easiest way to configure `sopel-twitter` is using Sopel's configuration
-wizard – simply run `sopel-plugins configure twitter` and enter the
-credentials for the Twitter application you created.
+**Twitter cookies are required to use this plugin** as of 1 July 2023. You may
+want to minimize the risk of adverse action by using a throwaway login instead
+of your real profile; however, note that doing so will affect the rate limit
+available to this plugin.
+
+The easiest way to configure `sopel-twitter` is via Sopel's configuration
+wizard – simply run `sopel-plugins configure twitter` and enter the cookie
+values for which it prompts you.
 
 Otherwise, you can edit your bot's configuration file:
 
 ```ini
 [twitter]
+cookies =
+    auth_token=df4c7364f4fac2b3843904ecc566b0e1accdf98b;
+    ct0=23f96509cba936b732cd39e171dce0fa5da9ecd1d7f3551258fe3e1a21da79a797e80496e8190613ba8a8ebc07ef6d8004b17518e84f9b6f8100738c5243a3da3139c87a5a55e46d70ed99cf0f068a23
+# Required: Cookies from Twitter
+# Newlines are not required, but the semicolon (;) very much is!
+# You will have to pull this from your own logged-in account; rate limits will
+# vary depending on the account's verification/Blue status.
+
 show_quoted_tweets = True
 # Optional: For quote-tweets, send a second message showing the quoted tweet?
 # Default: True
 
 alternate_domains =
     fxtwitter.com
     vxtwitter.com
     nitter.net
 # Optional: What other domains should we treat like twitter domains?
-# Default: vxtwitter.com, nitter.net
+# Default: fxtwitter.com, vxtwitter.com, nitter.net
 ```
 
 ## Usage
 
 Just send a link to a tweet or profile!
 
 You can also retrieve a user's info with the `.twitinfo` command:
@@ -61,14 +74,24 @@
 < Wiz> .twitinfo NASA
 < Sopel> [Twitter] NASA (@NASA) ✔️ | Pale Blue Dot | http://www.nasa.gov/
          | 204 friends, 46,602,251 followers | 65,377 tweets, 13,040 ♥s
          | Joined: 2007-12-19 - 20:20:32UTC | There's space for everybody. ✨
 ```
 
 
+Changes between 1.1.0 and 1.2.0
+===============================
+
+Breaking:
+* **Twitter cookies are now required**
+
+Changed:
+* Updated to `tweety-ns` 0.8 (#48)
+
+
 Changes between 1.0.1 and 1.1.0
 ===============================
 
 Changed:
 * Updated to `tweety-ns` 0.7, including revamped exceptions (#46)
```

