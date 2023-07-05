# Comparing `tmp/tweety-ns-0.7.1.tar.gz` & `tmp/tweety-ns-0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tweety-ns-0.7.1.tar", last modified: Thu May 11 11:43:23 2023, max compression
+gzip compressed data, was "tweety-ns-0.8.tar", last modified: Wed Jul  5 11:20:58 2023, max compression
```

## Comparing `tweety-ns-0.7.1.tar` & `tweety-ns-0.8.tar`

### file list

```diff
@@ -1,27 +1,33 @@
-drwxrwxrwx   0        0        0        0 2023-05-11 11:43:23.921986 tweety-ns-0.7.1/
--rw-rw-rw-   0        0        0     1019 2023-05-11 11:43:23.921986 tweety-ns-0.7.1/PKG-INFO
--rw-rw-rw-   0        0        0      302 2022-10-22 17:49:03.000000 tweety-ns-0.7.1/README.md
--rw-rw-rw-   0        0        0      108 2021-11-15 09:32:36.000000 tweety-ns-0.7.1/pyproject.toml
--rw-rw-rw-   0        0        0      701 2023-05-11 11:43:23.922982 tweety-ns-0.7.1/setup.cfg
--rw-rw-rw-   0        0        0      784 2023-05-11 11:42:58.000000 tweety-ns-0.7.1/setup.py
-drwxrwxrwx   0        0        0        0 2023-05-11 11:43:23.895746 tweety-ns-0.7.1/src/
-drwxrwxrwx   0        0        0        0 2023-05-11 11:43:23.908818 tweety-ns-0.7.1/src/tweety/
--rw-rw-rw-   0        0        0       54 2023-05-11 11:42:45.000000 tweety-ns-0.7.1/src/tweety/__init__.py
--rw-rw-rw-   0        0        0     9142 2023-05-11 10:52:50.000000 tweety-ns-0.7.1/src/tweety/bot.py
--rw-rw-rw-   0        0        0    12483 2023-05-10 20:10:35.000000 tweety-ns-0.7.1/src/tweety/builder.py
--rw-rw-rw-   0        0        0    18251 2023-04-24 18:05:20.000000 tweety-ns-0.7.1/src/tweety/exceptions_.py
--rw-rw-rw-   0        0        0      282 2022-03-04 06:53:48.000000 tweety-ns-0.7.1/src/tweety/filters.py
--rw-rw-rw-   0        0        0     5521 2023-05-11 04:58:39.000000 tweety-ns-0.7.1/src/tweety/http.py
-drwxrwxrwx   0        0        0        0 2023-05-11 11:43:23.915121 tweety-ns-0.7.1/src/tweety/types/
--rw-rw-rw-   0        0        0       58 2023-03-12 12:43:32.000000 tweety-ns-0.7.1/src/tweety/types/__init__.py
--rw-rw-rw-   0        0        0     2110 2023-05-10 06:18:15.000000 tweety-ns-0.7.1/src/tweety/types/n_types.py
--rw-rw-rw-   0        0        0     4932 2023-05-11 07:38:05.000000 tweety-ns-0.7.1/src/tweety/types/search.py
--rw-rw-rw-   0        0        0    27617 2023-05-10 19:53:22.000000 tweety-ns-0.7.1/src/tweety/types/twDataTypes.py
--rw-rw-rw-   0        0        0     3690 2023-05-11 07:18:05.000000 tweety-ns-0.7.1/src/tweety/types/usertweet.py
--rw-rw-rw-   0        0        0       96 2023-03-13 06:35:02.000000 tweety-ns-0.7.1/src/tweety/utils.py
-drwxrwxrwx   0        0        0        0 2023-05-11 11:43:23.921002 tweety-ns-0.7.1/src/tweety_ns.egg-info/
--rw-rw-rw-   0        0        0     1019 2023-05-11 11:43:23.000000 tweety-ns-0.7.1/src/tweety_ns.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      523 2023-05-11 11:43:23.000000 tweety-ns-0.7.1/src/tweety_ns.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-11 11:43:23.000000 tweety-ns-0.7.1/src/tweety_ns.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       45 2023-05-11 11:43:23.000000 tweety-ns-0.7.1/src/tweety_ns.egg-info/requires.txt
--rw-rw-rw-   0        0        0        7 2023-05-11 11:43:23.000000 tweety-ns-0.7.1/src/tweety_ns.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-07-05 11:20:58.807665 tweety-ns-0.8/
+-rw-rw-rw-   0        0        0     1846 2023-07-05 11:20:58.807665 tweety-ns-0.8/PKG-INFO
+-rw-rw-rw-   0        0        0     1137 2023-05-17 13:43:00.000000 tweety-ns-0.8/README.md
+-rw-rw-rw-   0        0        0      108 2021-11-15 09:32:36.000000 tweety-ns-0.8/pyproject.toml
+-rw-rw-rw-   0        0        0      699 2023-07-05 11:20:58.808663 tweety-ns-0.8/setup.cfg
+-rw-rw-rw-   0        0        0      800 2023-07-05 11:17:13.000000 tweety-ns-0.8/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-05 11:20:58.791461 tweety-ns-0.8/src/
+drwxrwxrwx   0        0        0        0 2023-07-05 11:20:58.798298 tweety-ns-0.8/src/tweety/
+-rw-rw-rw-   0        0        0       52 2023-07-05 11:18:41.000000 tweety-ns-0.8/src/tweety/__init__.py
+-rw-rw-rw-   0        0        0    10992 2023-07-05 07:31:27.000000 tweety-ns-0.8/src/tweety/bot.py
+-rw-rw-rw-   0        0        0    22429 2023-07-04 18:35:58.000000 tweety-ns-0.8/src/tweety/builder.py
+drwxrwxrwx   0        0        0        0 2023-07-05 11:20:58.799309 tweety-ns-0.8/src/tweety/events/
+-rw-rw-rw-   0        0        0       42 2023-07-04 06:05:54.000000 tweety-ns-0.8/src/tweety/events/__init__.py
+-rw-rw-rw-   0        0        0     1768 2023-07-04 10:00:32.000000 tweety-ns-0.8/src/tweety/events/newmessage.py
+-rw-rw-rw-   0        0        0    18739 2023-07-05 09:21:32.000000 tweety-ns-0.8/src/tweety/exceptions_.py
+-rw-rw-rw-   0        0        0      282 2022-03-04 06:53:48.000000 tweety-ns-0.8/src/tweety/filters.py
+-rw-rw-rw-   0        0        0     7465 2023-07-04 18:35:04.000000 tweety-ns-0.8/src/tweety/http.py
+drwxrwxrwx   0        0        0        0 2023-07-05 11:20:58.803664 tweety-ns-0.8/src/tweety/types/
+-rw-rw-rw-   0        0        0       58 2023-03-12 12:43:32.000000 tweety-ns-0.8/src/tweety/types/__init__.py
+-rw-rw-rw-   0        0        0     9218 2023-07-05 09:26:20.000000 tweety-ns-0.8/src/tweety/types/inbox.py
+-rw-rw-rw-   0        0        0     2631 2023-07-03 12:56:12.000000 tweety-ns-0.8/src/tweety/types/mentions.py
+-rw-rw-rw-   0        0        0     2141 2023-07-03 11:20:02.000000 tweety-ns-0.8/src/tweety/types/n_types.py
+-rw-rw-rw-   0        0        0     4325 2023-07-01 13:33:55.000000 tweety-ns-0.8/src/tweety/types/search.py
+-rw-rw-rw-   0        0        0    30124 2023-07-05 10:13:51.000000 tweety-ns-0.8/src/tweety/types/twDataTypes.py
+-rw-rw-rw-   0        0        0     3873 2023-07-05 07:09:50.000000 tweety-ns-0.8/src/tweety/types/usertweet.py
+-rw-rw-rw-   0        0        0      584 2023-07-04 06:06:52.000000 tweety-ns-0.8/src/tweety/updates.py
+-rw-rw-rw-   0        0        0      677 2023-07-04 06:34:07.000000 tweety-ns-0.8/src/tweety/utils.py
+drwxrwxrwx   0        0        0        0 2023-07-05 11:20:58.806663 tweety-ns-0.8/src/tweety_ns.egg-info/
+-rw-rw-rw-   0        0        0     1846 2023-07-05 11:20:58.000000 tweety-ns-0.8/src/tweety_ns.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      662 2023-07-05 11:20:58.000000 tweety-ns-0.8/src/tweety_ns.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-05 11:20:58.000000 tweety-ns-0.8/src/tweety_ns.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       45 2023-07-05 11:20:58.000000 tweety-ns-0.8/src/tweety_ns.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        7 2023-07-05 11:20:58.000000 tweety-ns-0.8/src/tweety_ns.egg-info/top_level.txt
```

### Comparing `tweety-ns-0.7.1/setup.cfg` & `tweety-ns-0.8/setup.cfg`

 * *Files 16% similar despite different names*

```diff
@@ -1,44 +1,44 @@
 00000000: 5b6d 6574 6164 6174 615d 0d0a 6e61 6d65  [metadata]..name
 00000010: 203d 2074 7765 6574 792d 6e73 0d0a 7665   = tweety-ns..ve
-00000020: 7273 696f 6e20 3d20 302e 372e 310d 0a61  rsion = 0.7.1..a
-00000030: 7574 686f 7220 3d20 5461 7979 6162 204b  uthor = Tayyab K
-00000040: 6861 726c 0d0a 6175 7468 6f72 5f65 6d61  harl..author_ema
-00000050: 696c 203d 2074 6179 7961 626d 6168 7240  il = tayyabmahr@
-00000060: 676d 6169 6c2e 636f 6d0d 0a64 6573 6372  gmail.com..descr
-00000070: 6970 7469 6f6e 203d 2041 6e20 6561 7379  iption = An easy
-00000080: 2054 7769 7474 6572 2053 6372 6170 6572   Twitter Scraper
-00000090: 0d0a 6c6f 6e67 5f64 6573 6372 6970 7469  ..long_descripti
-000000a0: 6f6e 203d 2066 696c 653a 2052 4541 444d  on = file: READM
-000000b0: 452e 6d64 0d0a 6c6f 6e67 5f64 6573 6372  E.md..long_descr
-000000c0: 6970 7469 6f6e 5f63 6f6e 7465 6e74 5f74  iption_content_t
-000000d0: 7970 6520 3d20 7465 7874 2f6d 6172 6b64  ype = text/markd
-000000e0: 6f77 6e0d 0a75 726c 203d 2068 7474 7073  own..url = https
-000000f0: 3a2f 2f67 6974 6875 622e 636f 6d2f 6d61  ://github.com/ma
-00000100: 6872 7461 7979 6162 2f74 7765 6574 790d  hrtayyab/tweety.
-00000110: 0a70 726f 6a65 6374 5f75 726c 7320 3d20  .project_urls = 
-00000120: 0d0a 0942 7567 2054 7261 636b 6572 203d  ...Bug Tracker =
-00000130: 2068 7474 7073 3a2f 2f67 6974 6875 622e   https://github.
-00000140: 636f 6d2f 6d61 6872 7461 7979 6162 2f74  com/mahrtayyab/t
-00000150: 7765 6574 792f 6973 7375 6573 0d0a 0944  weety/issues...D
-00000160: 6f63 756d 656e 7461 7469 6f6e 203d 2068  ocumentation = h
-00000170: 7474 7073 3a2f 2f67 6974 6875 622e 636f  ttps://github.co
-00000180: 6d2f 6d61 6872 7461 7979 6162 2f74 7765  m/mahrtayyab/twe
-00000190: 6574 790d 0a63 6c61 7373 6966 6965 7273  ety..classifiers
-000001a0: 203d 200d 0a09 5072 6f67 7261 6d6d 696e   = ...Programmin
-000001b0: 6720 4c61 6e67 7561 6765 203a 3a20 5079  g Language :: Py
-000001c0: 7468 6f6e 203a 3a20 330d 0a09 4c69 6365  thon :: 3...Lice
-000001d0: 6e73 6520 3a3a 204f 5349 2041 7070 726f  nse :: OSI Appro
-000001e0: 7665 6420 3a3a 204d 4954 204c 6963 656e  ved :: MIT Licen
-000001f0: 7365 0d0a 094f 7065 7261 7469 6e67 2053  se...Operating S
-00000200: 7973 7465 6d20 3a3a 204f 5320 496e 6465  ystem :: OS Inde
-00000210: 7065 6e64 656e 740d 0a0d 0a5b 6f70 7469  pendent....[opti
-00000220: 6f6e 735d 0d0a 7061 636b 6167 655f 6469  ons]..package_di
-00000230: 7220 3d20 0d0a 093d 2073 7263 0d0a 7061  r = ...= src..pa
-00000240: 636b 6167 6573 203d 2066 696e 643a 0d0a  ckages = find:..
-00000250: 7079 7468 6f6e 5f72 6571 7569 7265 7320  python_requires 
-00000260: 3d20 3e3d 332e 360d 0a0d 0a5b 6f70 7469  = >=3.6....[opti
-00000270: 6f6e 732e 7061 636b 6167 6573 2e66 696e  ons.packages.fin
-00000280: 645d 0d0a 7768 6572 6520 3d20 7372 630d  d]..where = src.
-00000290: 0a0d 0a5b 6567 675f 696e 666f 5d0d 0a74  ...[egg_info]..t
-000002a0: 6167 5f62 7569 6c64 203d 200d 0a74 6167  ag_build = ..tag
-000002b0: 5f64 6174 6520 3d20 300d 0a0d 0a         _date = 0....
+00000020: 7273 696f 6e20 3d20 302e 380d 0a61 7574  rsion = 0.8..aut
+00000030: 686f 7220 3d20 5461 7979 6162 204b 6861  hor = Tayyab Kha
+00000040: 726c 0d0a 6175 7468 6f72 5f65 6d61 696c  rl..author_email
+00000050: 203d 2074 6179 7961 626d 6168 7240 676d   = tayyabmahr@gm
+00000060: 6169 6c2e 636f 6d0d 0a64 6573 6372 6970  ail.com..descrip
+00000070: 7469 6f6e 203d 2041 6e20 6561 7379 2054  tion = An easy T
+00000080: 7769 7474 6572 2053 6372 6170 6572 0d0a  witter Scraper..
+00000090: 6c6f 6e67 5f64 6573 6372 6970 7469 6f6e  long_description
+000000a0: 203d 2066 696c 653a 2052 4541 444d 452e   = file: README.
+000000b0: 6d64 0d0a 6c6f 6e67 5f64 6573 6372 6970  md..long_descrip
+000000c0: 7469 6f6e 5f63 6f6e 7465 6e74 5f74 7970  tion_content_typ
+000000d0: 6520 3d20 7465 7874 2f6d 6172 6b64 6f77  e = text/markdow
+000000e0: 6e0d 0a75 726c 203d 2068 7474 7073 3a2f  n..url = https:/
+000000f0: 2f67 6974 6875 622e 636f 6d2f 6d61 6872  /github.com/mahr
+00000100: 7461 7979 6162 2f74 7765 6574 790d 0a70  tayyab/tweety..p
+00000110: 726f 6a65 6374 5f75 726c 7320 3d20 0d0a  roject_urls = ..
+00000120: 0942 7567 2054 7261 636b 6572 203d 2068  .Bug Tracker = h
+00000130: 7474 7073 3a2f 2f67 6974 6875 622e 636f  ttps://github.co
+00000140: 6d2f 6d61 6872 7461 7979 6162 2f74 7765  m/mahrtayyab/twe
+00000150: 6574 792f 6973 7375 6573 0d0a 0944 6f63  ety/issues...Doc
+00000160: 756d 656e 7461 7469 6f6e 203d 2068 7474  umentation = htt
+00000170: 7073 3a2f 2f67 6974 6875 622e 636f 6d2f  ps://github.com/
+00000180: 6d61 6872 7461 7979 6162 2f74 7765 6574  mahrtayyab/tweet
+00000190: 790d 0a63 6c61 7373 6966 6965 7273 203d  y..classifiers =
+000001a0: 200d 0a09 5072 6f67 7261 6d6d 696e 6720   ...Programming 
+000001b0: 4c61 6e67 7561 6765 203a 3a20 5079 7468  Language :: Pyth
+000001c0: 6f6e 203a 3a20 330d 0a09 4c69 6365 6e73  on :: 3...Licens
+000001d0: 6520 3a3a 204f 5349 2041 7070 726f 7665  e :: OSI Approve
+000001e0: 6420 3a3a 204d 4954 204c 6963 656e 7365  d :: MIT License
+000001f0: 0d0a 094f 7065 7261 7469 6e67 2053 7973  ...Operating Sys
+00000200: 7465 6d20 3a3a 204f 5320 496e 6465 7065  tem :: OS Indepe
+00000210: 6e64 656e 740d 0a0d 0a5b 6f70 7469 6f6e  ndent....[option
+00000220: 735d 0d0a 7061 636b 6167 655f 6469 7220  s]..package_dir 
+00000230: 3d20 0d0a 093d 2073 7263 0d0a 7061 636b  = ...= src..pack
+00000240: 6167 6573 203d 2066 696e 643a 0d0a 7079  ages = find:..py
+00000250: 7468 6f6e 5f72 6571 7569 7265 7320 3d20  thon_requires = 
+00000260: 3e3d 332e 360d 0a0d 0a5b 6f70 7469 6f6e  >=3.6....[option
+00000270: 732e 7061 636b 6167 6573 2e66 696e 645d  s.packages.find]
+00000280: 0d0a 7768 6572 6520 3d20 7372 630d 0a0d  ..where = src...
+00000290: 0a5b 6567 675f 696e 666f 5d0d 0a74 6167  .[egg_info]..tag
+000002a0: 5f62 7569 6c64 203d 200d 0a74 6167 5f64  _build = ..tag_d
+000002b0: 6174 6520 3d20 300d 0a0d 0a              ate = 0....
```

### Comparing `tweety-ns-0.7.1/setup.py` & `tweety-ns-0.8/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 from distutils.core import setup
 
 setup(
     name='tweety-ns',
-    packages=['tweety', 'tweety.types'],
-    version='0.7.1',
+    packages=['tweety', 'tweety.types', 'tweety.events'],
+    version='0.8',
     license='MIT',
     description='An easy Twitter Scraper',
     author='Tayyab Kharl',
     author_email='tayyabmahr@gmail.com',
     url='https://github.com/mahrtayyab/tweety',
     keywords=['TWITTER', 'TWITTER SCRAPE', 'SCRAPE TWEETS'],
     install_requires=[
         'beautifulsoup4',
         'openpyxl',
         'httpx',
         'dateutils',
-        'tqdm'
+        'tqdm',
     ],
     classifiers=[
         'Development Status :: 4 - Beta',
         'Intended Audience :: Developers',
         'Topic :: Software Development :: Build Tools',
         'License :: OSI Approved :: MIT License',
         'Programming Language :: Python :: 3'
```

### Comparing `tweety-ns-0.7.1/src/tweety/bot.py` & `tweety-ns-0.8/src/tweety/bot.py`

 * *Files 20% similar despite different names*

```diff
@@ -3,40 +3,49 @@
 from typing import Union
 
 from .types.n_types import Proxy
 from .exceptions_ import *
 from .http import Request
 from .types.usertweet import UserTweets
 from .types.search import Search
+from .types.mentions import Mention
+from .types.inbox import Inbox, SendMessage, Conversation
+from .updates import UpdateMethods
 from .types.twDataTypes import User, Trends, Tweet
+from .utils import create_conversation_id
 
 
 def AuthRequired(f):
     @functools.wraps(f)
     def wrapper(self, *args, **kwargs):
         if self.user is None:
             raise AuthenticationRequired(200, "GenericForbidden", None)
 
         return f(self, *args, **kwargs)
 
     return wrapper
 
 
-class Twitter:
+class Twitter(UpdateMethods):
     def __init__(self, max_retires: int = 10, proxy: Union[dict, Proxy] = None, cookies: Union[str, dict] = None):
         """
         Constructor of the Twitter Public class
 
         :param max_retires: (`int`) Number of retries the script would make , if the guest token wasn't found
         :param proxy: (`dict` or `Proxy`) Provide the proxy you want to use while making a request
         :param cookies: (`str` or `dict`) Cookies which will be used for user authentication
         """
 
+        if not cookies:
+            raise AuthenticationRequired(200, "GenericForbidden", None)
+
         self.request = Request(max_retries=max_retires, proxy=proxy, cookies=cookies)
-        self.user = self.get_user_info() if cookies is not None else None
+        self.user = self.get_user_info()
+        super().__init__(self.request)
+        self.request.set_user(self.user)
 
     def get_user_info(self, username: str = None, banner_extensions: bool = False, image_extensions: bool = False):
         """
         Get the User Info of the specified username
 
         :param username: (`str`) username to get information of
         :param banner_extensions: (`boolean`) Get the Banner extension on the user page
@@ -64,16 +73,15 @@
     @property
     def user_id(self):
         """
         Get the user unique twitter id
 
         :return: int
         """
-
-        return self.user.rest_id if self.user else None
+        return self.user.id if self.user else None
 
     def _get_user_id(self, username):
         if isinstance(username, User):
             user_id = username.rest_id
         elif isinstance(username, int):
             user_id = username
         elif isinstance(username, str) and str(username).isdigit():
@@ -132,15 +140,15 @@
         """
         Get the Trends from you locale
 
         :return:list of .types.twDataTypes.Trends
         """
         trends = []
         response = self.request.get_trends()
-        for i in response.json()['timeline']['instructions'][1]['addEntries']['entries'][1]['content']['timelineModule']['items']:
+        for i in response['timeline']['instructions'][1]['addEntries']['entries'][1]['content']['timelineModule']['items']:
             data = {
                 "name": i['item']['content']['trend']['name'],
                 "url": str(i['item']['content']['trend']['url']['url']).replace("twitter://",
                                                                                 "https://twitter.com/").replace("query",
                                                                                                                 "q"),
             }
             try:
@@ -196,14 +204,51 @@
         if wait_time is None:
             wait_time = 0
 
         search = Search(keyword, self.request, pages, filter_, wait_time, cursor)
 
         return search.generator()
 
+    def get_mentions(self, pages: int = 1, wait_time: int = 2, cursor: str = None):
+        """
+
+        :param pages: (`int`) The number of pages to get
+        :param wait_time: (`int`) seconds to wait between multiple requests
+        :param cursor: (`str`) Pagination cursor if you want to get the pages from that cursor up-to (This cursor is different from actual API cursor)
+        :return:
+        """
+
+        if wait_time is None:
+            wait_time = 0
+
+        mentions = Mention(self.user.id, self.request, pages, wait_time, cursor)
+        results = [i for i in mentions.generator()]
+
+        return mentions
+
+    def get_inbox(self, user_id: Union[int, str, User] = None, cursor: str = None):
+        """
+        :param user_id : (`str`, `int`, `User`) User id or username of the user whom to get the messages of. Default is ALL
+        :param cursor: (`str`) Pagination cursor if you want to get the pages from that cursor up-to (This cursor is different from actual API cursor)
+                                It is used to get the messages updates
+        :return:
+        """
+
+        if user_id:
+            user_id = self._get_user_id(user_id)
+
+        inbox = Inbox(user_id, self.request, cursor)
+
+        return inbox
+
+    def send_message(self, username: Union[str, int, User], text: str):
+        user_id = self._get_user_id(username)
+        conversation_id = create_conversation_id(self.user.id, user_id)
+        return SendMessage(self.request, conversation_id, text).send()
+
     def tweet_detail(self, identifier: str):
         """
         Get Detail of a single tweet
 
         :param identifier: (`str`) The unique identifier of the tweet , either the `Tweet id` or `Tweet Link`
 
         :return: .types.twDataTypes.Tweet
@@ -215,11 +260,11 @@
 
         try:
             for entry in r['data']['threaded_conversation_with_injections_v2']['instructions'][0]['entries']:
                 if str(entry['entryId']).split("-")[0] == "tweet":
                     raw_tweet = entry['content']['itemContent']['tweet_results']['result']
 
                     if raw_tweet['rest_id'] == str(tweetId):
-                        return Tweet(r, raw_tweet, self.request, True, False, True)
+                        return Tweet(raw_tweet, self.request, r)
 
         except KeyError:
             raise InvalidTweetIdentifier(144, "StatusNotFound", r)
```

### Comparing `tweety-ns-0.7.1/src/tweety/exceptions_.py` & `tweety-ns-0.8/src/tweety/exceptions_.py`

 * *Files 2% similar despite different names*

```diff
@@ -46,14 +46,30 @@
         self.message = message
         self.error_code = error_code
         self.error_name = error_name
         self.response = response
         super().__init__(self.message)
 
 
+class RateLimitReached(Exception):
+    """
+        Exception Raised when the tweet identifier is invalid
+
+        Attributes:
+            message -- explanation of the error
+    """
+
+    def __init__(self, error_code, error_name, response, message="You have exceeded the Twitter Rate Limit"):
+        self.message = message
+        self.error_code = error_code
+        self.error_name = error_name
+        self.response = response
+        super().__init__(self.message)
+
+
 class ProxyParseError(Exception):
     """
     Exception Raised when an error occurs while parsing the provided proxy
 
     Attributes:
         message -- explanation of the error
     """
```

### Comparing `tweety-ns-0.7.1/src/tweety/http.py` & `tweety-ns-0.8/src/tweety/http.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,42 +1,45 @@
 import os
 import httpx as s
 from tqdm import tqdm
-
 from .exceptions_ import GuestTokenNotFound, UnknownError, UserNotFound, InvalidCredentials
 from .types.n_types import GenericError
-from .utils import custom_json
+from .utils import custom_json, create_request_id
 from .builder import UrlBuilder
 
+
 s.Response.json_ = custom_json
 
 
 class Request:
     def __init__(self, max_retries=10, proxy=None, cookies=None):
+        self.user = None
         self.username = None
         self.__is_client = True if cookies else False
         self.__session = s.Client(proxies=proxy, cookies=self._parse_cookies(cookies), timeout=60)
         self.__builder = UrlBuilder(self.__session.cookies)
         self.__guest_token = self._get_guest_token(max_retries)
-        self._init_api()
         self._verify_cookies()
-
+    
+    def set_user(self, user):
+        self.user = user
+    
     def __get_response__(self, **request_data):
         response = self.__session.request(**request_data)
         response_json = response.json_() # noqa
 
         if not response_json:
             raise UnknownError(
                 error_code=500,
                 error_name="Server Error",
                 response=response,
                 message="Unknown Error Occurs on Twitter"
             )
 
-        if response_json.get("errors"):
+        if response_json.get("errors") and not response_json.get("data"):
             error = response_json['errors'][0]
             return GenericError(
                 response, error.get("code"), error.get("message")
             )
 
         return response_json
 
@@ -125,29 +128,73 @@
         request_data = self.__builder.search(keyword, cursor, filter_)
         # del request_data['headers']['content-type']
         request_data['headers']['referer'] = f"https://twitter.com/search?q={keyword}"
 
         response = self.__get_response__(**request_data)
         return response
 
-    def get_tweet_detail(self, tweetId):
-        response = self.__get_response__(**self.__builder.tweet_detail(tweetId))
+    def get_tweet_detail(self, tweetId, cursor=None):
+        response = self.__get_response__(**self.__builder.tweet_detail(tweetId, cursor))
+        return response
+
+    def get_mentions(self, user_id, cursor=None):
+        response = self.__get_response__(**self.__builder.get_mentions(cursor))
+        return response
+
+    def get_inbox(self, user_id, cursor=None):
+        response = self.__get_response__(**self.__builder.get_inbox(cursor))
+        return response
+
+    def get_trusted_inbox(self, max_id):
+        response = self.__get_response__(**self.__builder.get_trusted_inbox(max_id))
+        return response
+
+    def get_untrusted_inbox(self, max_id, low_quality=False):
+        response = self.__get_response__(**self.__builder.get_untrusted_inbox(max_id, low_quality))
+        return response
+
+    def get_conversation(self, conversation_id, max_id=None):
+        response = self.__get_response__(**self.__builder.get_conversation_with_messages(conversation_id, max_id))
+        return response
+
+    def send_message(self, conversation_id, text):
+        request_id = create_request_id()
+        json_data = {
+            'conversation_id': conversation_id,
+            'recipient_ids': False,
+            'request_id': request_id,
+            'text': text,
+            'cards_platform': 'Web-12',
+            'include_cards': 1,
+            'include_quote_count': True,
+            'dm_users': False,
+        }
+        request_data = self.__builder.send_message()
+        request_data['json'] = json_data
+        response = self.__get_response__(**request_data)
         return response
 
     def download_media(self, media_url, filename=None, show_progress=True):
         filename = os.path.basename(media_url).split("?")[0] if not filename else filename
+        headers = self.__session.headers
+        oldReferer = headers.get('Referer')
+
+        if media_url.startswith("https://ton.twitter.com"):
+            headers['Referer'] = "https://twitter.com/"
+            self.__session.header = headers
 
-        with self.__session.stream('GET', media_url) as response:
+        with self.__session.stream('GET', media_url, follow_redirects=True) as response:
             response.raise_for_status()
             content_length = int(response.headers['Content-Length'])
             f = open(filename, 'wb')
             if show_progress:
                 with tqdm(total=content_length, unit='B', unit_scale=True, desc=f"[{filename}]") as pbar:
                     for chunk in response.iter_bytes(chunk_size=8192):
                         f.write(chunk)
                         pbar.update(len(chunk))
             else:
                 for chunk in response.iter_bytes(chunk_size=8192):
                     f.write(chunk)
             f.close()
 
+        self.__session.header['Referer'] = oldReferer
         return filename
```

### Comparing `tweety-ns-0.7.1/src/tweety/types/n_types.py` & `tweety-ns-0.8/src/tweety/types/n_types.py`

 * *Files 3% similar despite different names*

```diff
@@ -35,15 +35,16 @@
 
         raise ProxyParseError()
 
 
 class GenericError:
     EXCEPTIONS = {
         32: InvalidCredentials,
-        144: InvalidTweetIdentifier
+        144: InvalidTweetIdentifier,
+        88: RateLimitReached
     }
 
     def __init__(self, response, error_code, message=None):
         self.response = response
         self.error_code = error_code
         self.message = message
         self._raise_exception()
```

### Comparing `tweety-ns-0.7.1/src/tweety/types/search.py` & `tweety-ns-0.8/src/tweety/types/search.py`

 * *Files 14% similar despite different names*

```diff
@@ -31,76 +31,78 @@
 
             self['is_next_page'] = self.is_next_page
             self['cursor'] = self.cursor
 
             return thisTweets
 
         return []
+
+    @staticmethod
+    def _get_entries(response):
+        instructions = response['data']['search_by_raw_query']['search_timeline']['timeline']['instructions']
+        for instruction in instructions:
+            if instruction.get("type") == "TimelineAddEntries":
+                return instruction['entries']
+
+        return []
+
+    @staticmethod
+    def _get_tweet_content_key(response):
+        if str(response['entryId']).split("-")[0] == "tweet":
+            return [response['content']['itemContent']['tweet_results']['result']]
+
+        if str(response['entryId']).split("-")[0] == "user":
+            return [response['content']['itemContent']['user_results']['result']]
+
+        if str(response['entryId']).split("-")[0] == "homeConversation":
+            return [item['item']['itemContent']['tweet_results']['result'] for item in response["content"]["items"]]
+
+        return []
+
     def _parse_response(self, response):
         thisObjects = []
-        if self.filter == "users":
-            for raw_user in response['globalObjects']['users'].values():
-                try:
-                    user = User(raw_user)
-                    self.users.append(user)
-                    thisObjects.append(user)
-                except:
-                    pass
-            self['users'] = self.users
-        else:
-            users = response['globalObjects']['users']
-            for tweet_id, raw_tweet in response['globalObjects']['tweets'].items():
-                try:
-                    raw_tweet['rest_id'], raw_tweet['author'] = tweet_id, users.get(str(raw_tweet['user_id']))
-                    tweet = Tweet(response, raw_tweet, self.http, False, True)
-                    self.tweets.append(tweet)
-                    thisObjects.append(tweet)
-                except:
-                    traceback.print_exc()
-                    pass
+        entries = self._get_entries(response)
+        for entry in entries:
+            if self.filter == "users":
+                users = self._get_tweet_content_key(entry)
+                for user in users:
+                    try:
+                        user = User(user)
+                        self.users.append(user)
+                        thisObjects.append(user)
+                    except:
+                        pass
+                self['users'] = self.users
+            else:
+                tweets = self._get_tweet_content_key(entry)
+                for tweet in tweets:
+                    try:
+                        parsed = Tweet(response, tweet, self.http)
+                        self.tweets.append(parsed)
+                        thisObjects.append(parsed)
+                    except:
+                        pass
 
-            self['tweets'] = self.tweets
+                self['tweets'] = self.tweets
 
-        self.is_next_page = self._get_cursor(response)
+        self.is_next_page = self._get_cursor(entries)
         return thisObjects
 
-    def _get_cursor(self, response):
-        if self.filter == "users":
-            for i in response['timeline']['instructions'][-1]['addEntries']['entries']:
-                if str(i['entryId']).split("-")[0] == "cursor":
-                    if i['content']['operation']['cursor']['cursorType'] == "Bottom":
-                        newCursor = i['content']['operation']['cursor']['value']
-                        if newCursor == self.cursor:
-                            return False
-                        self.cursor = newCursor
-                        return True
-        else:
-            for i in response['timeline']['instructions'][0]['addEntries']['entries']:
-                try:
-                    if i['content']['operation']:
-                        if i['content']['operation']['cursor']['cursorType'] == "Bottom":
-                            newCursor = i['content']['operation']['cursor']['value']
-                            if newCursor == self.cursor:
-                                return False
-                            self.cursor = newCursor
-                            return True
-                except:
-                    pass
-                try:
-                    for j in response['timeline']['instructions']:
-                        for key in j.keys():
-                            if key == "replaceEntry":
-                                if j['replaceEntry']['entry']['content']['operation']['cursor']['cursorType'] == "Bottom":
-                                    newCursor = j['replaceEntry']['entry']['content']['operation']['cursor']['value']
-                                    if newCursor == self.cursor:
-                                        return False
-                                    self.cursor = newCursor
-                                    return True
-                except:
-                    pass
+    def _get_cursor(self, entries):
+        for entry in entries:
+            if str(entry['entryId']).split("-")[0] == "cursor":
+                if entry['content']['cursorType'] == "Bottom":
+                    newCursor = entry['content']['value']
+
+                    if newCursor == self.cursor:
+                        return False
+
+                    self.cursor = newCursor
+                    return True
+
         return False
 
     def generator(self):
         for page in range(1, int(self.pages) + 1):
             this_tweets = self.get_next_page()
 
             yield self, this_tweets
```

### Comparing `tweety-ns-0.7.1/src/tweety/types/twDataTypes.py` & `tweety-ns-0.8/src/tweety/types/twDataTypes.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,17 +1,18 @@
 import base64
 import os.path
 import re
 import sys
+import time
 import warnings
 from dateutil import parser
 import openpyxl
 import dateutil
 
-WORKBOOK_HEADERS = ['Created on', 'author', 'is_retweet', 'is_reply', 'tweet_id', 'tweet_body', 'language', 'likes',
+WORKBOOK_HEADERS = ['Date', 'Author', 'id', 'text', 'is_retweet', 'is_reply', 'language', 'likes',
                     'retweet_count', 'source', 'medias', 'user_mentioned', 'urls', 'hashtags', 'symbols']
 
 
 def decodeBase64(encoded_string):
     return str(base64.b64decode(bytes(encoded_string, "utf-8")))[2:-1]
 
 
@@ -36,217 +37,303 @@
 def bar_progress(current, total, width=80):
     progress_message = "Downloading: %d%% [%d / %d] bytes" % (current / total * 100, current, total)
     sys.stdout.write("\r" + progress_message)
     sys.stdout.flush()
 
 
 class Excel:
-    def __init__(self, tweets, user, filename=None):
+    def __init__(self, tweets, filename=None, append=False):
         self.tweets = tweets
-        self.user = user
         self.filename = filename
-        self.workbook = openpyxl.Workbook()
-        self.worksheet = self.workbook.create_sheet("tweets")
-        self._set_headers()
-        self.max_row = 1
+        self.author = self._get_author()
+        self._append = append
+        self._get_sheet()
+        self.max_row = self._get_max_row()
         self._write_data()
 
+    def _get_sheet(self):
+        if self._append and self.filename:
+            self.workbook = openpyxl.load_workbook(self.filename)
+            self.worksheet = self.workbook.active
+        else:
+            self._append = False
+            self.workbook = openpyxl.Workbook()
+            self.worksheet = self.workbook.create_sheet("tweets")
+
+    def _get_author(self):
+        for tweet in self.tweets:
+            if hasattr(tweet, "author"):
+                return tweet.author.username
+
+        return ""
+
+    def _get_max_row(self):
+        if self._append:
+            for row in reversed(self.worksheet.iter_rows(values_only=True)):
+                if any(cell for cell in row):
+                    return row[0].row
+
+        self._set_headers()
+        return 1
+
     def _set_headers(self):
         for index, value in enumerate(WORKBOOK_HEADERS, start=1):
             self.worksheet.cell(row=1, column=index).value = value
 
+    def _write_tweet(self, tweet):
+        self.worksheet[f'A{self.max_row + 1}'] = tweet.date
+        self.worksheet[f'B{self.max_row + 1}'] = tweet.author.name
+        self.worksheet[f'C{self.max_row + 1}'] = tweet.id
+        self.worksheet[f'D{self.max_row + 1}'] = tweet.text
+        self.worksheet[f'E{self.max_row + 1}'] = tweet.is_retweet
+        self.worksheet[f'F{self.max_row + 1}'] = tweet.is_reply
+        self.worksheet[f'G{self.max_row + 1}'] = tweet.language
+        self.worksheet[f'H{self.max_row + 1}'] = tweet.likes
+        self.worksheet[f'I{self.max_row + 1}'] = tweet.retweet_counts
+        self.worksheet[f'J{self.max_row + 1}'] = tweet.source
+        self.worksheet[f'K{self.max_row + 1}'] = ",".join(
+            [media.expanded_url for media in tweet.media]) if tweet.media else ""
+        self.worksheet[f'L{self.max_row + 1}'] = ",".join(
+            [user_mention.screen_name for user_mention in tweet.user_mentions]) if tweet.user_mentions else ""
+        self.worksheet[f'M{self.max_row + 1}'] = ",".join(
+            [url['expanded_url'] for url in tweet.urls]) if tweet.urls else ""
+        self.worksheet[f'N{self.max_row + 1}'] = ",".join(
+            [hashtag['text'] for hashtag in tweet.hashtags]) if tweet.hashtags else ""
+        self.worksheet[f'O{self.max_row + 1}'] = ",".join([symbol for symbol in tweet.symbols]) if tweet.symbols else ""
+        self.max_row += 1
+
     def _write_data(self):
         for tweet in self.tweets:
-            self.worksheet[f'A{self.max_row  + 1}'] = tweet.date
-            self.worksheet[f'B{self.max_row  + 1}'] = tweet.author.name
-            self.worksheet[f'C{self.max_row  + 1}'] = tweet.is_retweet
-            self.worksheet[f'D{self.max_row  + 1}'] = tweet.is_reply
-            self.worksheet[f'E{self.max_row  + 1}'] = tweet.id
-            self.worksheet[f'F{self.max_row  + 1}'] = tweet.text
-            self.worksheet[f'G{self.max_row  + 1}'] = tweet.language
-            self.worksheet[f'H{self.max_row  + 1}'] = tweet.likes
-            self.worksheet[f'I{self.max_row  + 1}'] = tweet.retweet_counts
-            self.worksheet[f'J{self.max_row  + 1}'] = tweet.source
-            self.worksheet[f'K{self.max_row  + 1}'] = ",".join([media.expanded_url for media in tweet.media]) if tweet.media else ""
-            self.worksheet[f'L{self.max_row  + 1}'] = ",".join([user_mention.screen_name for user_mention in tweet.user_mentions]) if tweet.user_mentions else ""
-            self.worksheet[f'M{self.max_row  + 1}'] = ",".join([url['expanded_url'] for url in tweet.urls]) if tweet.urls else ""
-            self.worksheet[f'N{self.max_row  + 1}'] = ",".join([hashtag['text'] for hashtag in tweet.hashtags]) if tweet.hashtags else ""
-            self.worksheet[f'O{self.max_row  + 1}'] = ",".join([symbol for symbol in tweet.symbols]) if tweet.symbols else ""
-            self.max_row += 1
+            if isinstance(tweet, Tweet):
+                self._write_tweet(tweet)
+            elif isinstance(tweet, TweetThread):
+                for _threadedTweet in tweet:
+                    self._write_tweet(_threadedTweet)
 
         if not self.filename:
-            self.filename = f"tweets-{self.user.screen_name}.xlsx"
+            self.filename = f"tweets-{self.author}.xlsx"
 
         try:
             self.workbook.remove("sheet")
         except ValueError:
             pass
 
         self.workbook.save(self.filename)
 
 
+class TweetThread(dict):
+    def __init__(self, response, http, _full_response=None):
+        super().__init__()
+        self._raw = response
+        self._http = http
+        self._full_response = _full_response
+        self.tweets = self['tweets'] = self.parse_tweets()
+
+    def parse_tweets(self):
+        _tweets = []
+        for tweet in self._raw:
+            try:
+                _tweets.append(Tweet(tweet, self._http, self._full_response))
+            except:
+                pass
+
+        return _tweets
+
+    def __getitem__(self, index):
+        return self.tweets[index]
+
+    def __iter__(self):
+        for __tweet in self.tweets:
+            yield __tweet
+
+    def __len__(self):
+        return len(self.tweets)
+
+    def __repr__(self):
+        return "TweetThread(tweets={})".format(
+            len(self.tweets)
+        )
+
+
 class Tweet(dict):
-    def __init__(self, raw_response, raw_tweet, http, get_threads=False, is_legacy_user=False, get_reply=False):  # noqa
+    def __init__(self, tweet, http, full_response=None):  # noqa
         super().__init__()
         self.http = http
-        self.__raw_response = raw_response
-        self.__raw_tweet = raw_tweet
-        self.__is_legacy_user = is_legacy_user
+        self.__tweet = tweet
+        self.__full_response = full_response
         self.__replied_to = None
-        self._get_reply = get_reply
         self._format_tweet()
 
-        if get_threads:
-            self._get_threads()
-
         for key, value in vars(self).items():
             if not str(key).startswith("_"):
                 self[key] = value
 
     def __repr__(self):
-        return f"Tweet(id={self.id}, author={self.author}, created_on={self.created_on}, threads={len(self.threads) if self.threads else None})"  # noqa
+        return f"Tweet(id={self.id}, author={self.author}, created_on={self.created_on})"  # noqa
 
     def __iter__(self):
         if self.threads:  # noqa
             for thread_ in self.threads:  # noqa
                 yield thread_
 
     def _format_tweet(self):
-        original_tweet = self._get_original_tweet()
+        original_tweet = self.__tweet['legacy'] if self.__tweet.get('legacy') else self.__tweet
         self.id = self._get_id()
-        self.created_on = self.date = dateutil.parser.parse(original_tweet["created_at"])
+        self.created_on = self.date = self._get_date(original_tweet)
         self.author = self._get_author()
         self.is_retweet = self._is_retweet(original_tweet)
         self.retweeted_tweet = self._get_retweeted_tweet(self.is_retweet, original_tweet)
         self.text = self.tweet_body = self._get_tweet_text(original_tweet, self.is_retweet)
         self.is_quoted = self._is_quoted(original_tweet)
         self.quoted_tweet = self._get_quoted_tweet(self.is_quoted)
         self.is_reply = self._is_reply(original_tweet)
         self.is_sensitive = self._is_sensitive(original_tweet)
         self.reply_counts = self._get_reply_counts(original_tweet)
         self.quote_counts = self._get_quote_counts(original_tweet)
-        self.replied_to = self.__replied_to = self._get_reply_to(self.is_reply, original_tweet)
+        self.replied_to = self._get_reply_to(self.is_reply)
         self.bookmark_count = self._get_bookmark_count(original_tweet)
         self.vibe = self._get_vibe()
         self.views = self._get_views()
         self.language = self._get_language(original_tweet)
         self.likes = self._get_likes(original_tweet)
-        self.card = self._get_card()
         self.place = self._get_place(original_tweet)
         self.retweet_counts = self._get_retweet_counts(original_tweet)
-        self.source = self._get_source(self.__raw_tweet)
+        self.source = self._get_source(self.__tweet)
         self.voice_info = None  # TODO
         self.media = self._get_tweet_media(original_tweet)
         self.user_mentions = self._get_tweet_mentions(original_tweet)
         self.urls = self._get_tweet_urls(original_tweet)
         self.hashtags = self._get_tweet_hashtags(original_tweet)
         self.symbols = self._get_tweet_symbols(original_tweet)
-        self.threads = []
         self.comments = []
 
-    def _get_id(self):
-        if self.__raw_tweet.get("rest_id"):
-            return self.__raw_tweet['rest_id']
+    def get_comments(self, pages=1, wait_time=2, cursor=None):
+        if not wait_time:
+            wait_time = 0
+
+        results = [i for i in self.iter_comments(pages, wait_time, cursor)]
+        return self.comments
+
+    def iter_comments(self, pages=1, wait_time=2, cursor=None):
+        if not wait_time:
+            wait_time = 0
+
+        cursor = cursor
+        _comments = []
+        pages = pages
+        for page in range(1, int(pages) + 1):
+            _, comments, new_cursor = self._get_comments(cursor, self.__full_response)
+
+            yield self, comments
+
+            if cursor != new_cursor and page != pages:
+                time.sleep(wait_time)
+            else:
+                break
+
+    def _get_comments(self, cursor=None, response=None):
+        _comments = []
+        _cursor = cursor
+
+        if not response:
+            response = self.http.get_tweet_detail(self.id, cursor)
+        else:
+            self.__full_response = None
+
+        for instruction in response['data']['threaded_conversation_with_injections_v2']['instructions']:
+            if instruction['type'] == "TimelineAddEntries":
+                for entry in instruction['entries']:
+                    if str(entry['entryId'].split("-")[0]) == "conversationthread":
+                        for item in entry['content']['items']:
+                            tweet = item['item']['itemContent']['tweet_results']['result']
+                            try:
+                                parsed = Tweet(tweet, self.http)
+                                _comments.append(parsed)
+                                self.comments.append(parsed)
+                            except:
+                                pass
+                    elif "cursor-bottom" in str(entry['entryId']):
+                        _cursor = entry['content']['itemContent']['value']
+
+        return self, _comments, _cursor
 
-        if self.__raw_tweet.get("tweet"):
-            return self.__raw_tweet['tweet']['rest_id']
+    @staticmethod
+    def _get_date(original_tweet):
+        date = original_tweet.get("created_at")
+
+        if date:
+            return dateutil.parser.parse(date)
 
-    def _get_original_tweet(self):
-        if self.__raw_tweet.get("tweet"):
-            self.__raw_tweet = self.__raw_tweet['tweet']
+        return None
 
-        if self.__raw_tweet.get("legacy"):
-            return self.__raw_tweet['legacy']
+    def _get_id(self):
+        if self.__tweet.get("rest_id"):
+            return self.__tweet['rest_id']
 
-        return self.__raw_tweet
+        if self.__tweet.get("tweet"):
+            return self.__tweet['tweet']['rest_id']
 
     def _get_author(self):
-        if self.__raw_tweet.get("core"):
-            return User(self.__raw_tweet['core']['user_results']['result'])
+        if self.__tweet.get("core"):
+            return User(self.__tweet['core']['user_results']['result'])
+
+        if self.__tweet.get("author"):
+            return User(self.__tweet['author'])
 
-        if self.__raw_tweet.get("author"):
-            return User(self.__raw_tweet['author'])
         return None
 
     def _get_retweeted_tweet(self, is_retweet, original_tweet):
         if is_retweet and original_tweet.get("retweeted_status_result"):
             retweet = original_tweet['retweeted_status_result']['result']
-            return Tweet(None, retweet, self.http)
+            return Tweet(retweet, self.http)
 
         return None
 
-    def _get_threads(self):
-        if not self.__raw_response:
-            self.__raw_response = self.http.get_tweet_detail(self.id)  # noqa
-
-        for entry in self.__raw_response['data']['threaded_conversation_with_injections_v2']['instructions'][0]['entries']:
-            if str(entry['entryId']).split("-")[0] == "conversationthread":
-                for item in entry['content']['items']:
-                    try:
-                        tweetType = item["item"]["itemContent"]["tweetDisplayType"]
-                        tweet = item['item']['itemContent']['tweet_results']['result']
-
-                        if not self.__replied_to or self.__replied_to.id != tweet['rest_id']:
-                            if tweetType == "SelfThread":
-                                self.threads.append(Tweet(None, tweet, self.http))
-                            else:
-                                self.comments.append(Tweet(None, tweet, self.http))
-                    except KeyError as e:
-                        pass
-
     def _get_quoted_tweet(self, is_quoted):
-        raw_tweet = None
         if is_quoted:
-            raw_response = self.__raw_response
             try:
-                if self.__raw_tweet.get("quoted_status_result"):
-                    raw_tweet = self.__raw_tweet['quoted_status_result']['result']
-                    return Tweet(raw_response, raw_tweet, self.http)
-
-                if not raw_tweet and self.__raw_tweet.get("legacy"):
-                    raw_tweet = self.__raw_tweet['legacy']['retweeted_status_result']['result']['quoted_status_result']['result']
-                    return Tweet(raw_response, raw_tweet, self.http)
+                if self.__tweet.get("quoted_status_result"):
+                    raw_tweet = self.__tweet['quoted_status_result']['result']
+                    return Tweet(raw_tweet, self.http)
+
+                if self.__tweet.get("legacy"):
+                    raw_tweet = self.__tweet['legacy']['retweeted_status_result']['result']['quoted_status_result']['result']
+                    return Tweet(raw_tweet, self.http)
+
+                return None
             except:
                 return None
 
         return None
 
-    def _get_card(self):
-        if self.__raw_tweet.get("card"):
-            try:
-                return Card(self.__raw_tweet['card'])
-            except KeyError:
-                pass
-        return None
-
     def _get_vibe(self):
-        if self.__raw_tweet.get("vibe"):
-            vibeImage = self.__raw_tweet['vibe']['imgDescription']
-            vibeText = self.__raw_tweet['vibe']['text']
+        if self.__tweet.get("vibe"):
+            vibeImage = self.__tweet['vibe']['imgDescription']
+            vibeText = self.__tweet['vibe']['text']
             return f"{vibeImage} {vibeText}"
 
         return ""
 
     def _get_views(self):
-        if self.__raw_tweet.get("views"):
-            return self.__raw_tweet['views'].get('count', 'Unavailable')
+        if self.__tweet.get("views"):
+            return self.__tweet['views'].get('count', 'Unavailable')
 
         return 0
 
-    def _get_reply_to(self, is_reply, tweet):
-        if is_reply and self._get_reply:
-            tweet_id = tweet['in_reply_to_status_id_str']
-            response = self.http.get_tweet_detail(tweet_id)
-            for entry in response.json()['data']['threaded_conversation_with_injections_v2']['instructions'][0]['entries']:
-                if str(entry['entryId']).split("-")[0] == "tweet":
+    def _get_reply_to(self, is_reply):
+        if is_reply:
+            tweet_id = self.__tweet['legacy']['in_reply_to_status_id_str']
+            if not self.__full_response:
+                response = self.http.get_tweet_detail(tweet_id)
+            else:
+                response = self.__full_response
+            for entry in response['data']['threaded_conversation_with_injections_v2']['instructions'][0]['entries']:
+                if str(entry['entryId']).split("-")[0] == "tweet" and str(entry['content']['itemContent']['tweet_results']['result']['rest_id']) == str(tweet_id):
                     raw_tweet = entry['content']['itemContent']['tweet_results']['result']
-                    return Tweet(response, raw_tweet, self.http)
-
-        elif is_reply and not self._get_reply:
-            return tweet['in_reply_to_screen_name']
+                    return Tweet(raw_tweet, self.http)
         return None
 
     @staticmethod
     def _is_sensitive(original_tweet):
         return original_tweet.get("possibly_sensitive", False)
 
     @staticmethod
@@ -369,25 +456,31 @@
             return []
 
         if not original_tweet['entities'].get("symbols"):
             return []
 
         return [symbol for symbol in original_tweet['entities']['symbols']]
 
+    def __eq__(self, other):
+        if isinstance(other, Tweet):
+            return str(self.id) == str(other.id) and str(self.author.id) == str(other.author.id)
+
+        return str(self.id) == str(other)
+
 
 class Media(dict):
     def __init__(self, media_dict, http):
         super().__init__()
         self.__dictionary = media_dict
         self.__http = http
         self.display_url = self.__dictionary.get("display_url")
         self.expanded_url = self.__dictionary.get("expanded_url")
         self.id = self.__dictionary.get("id_str")
         self.indices = self.__dictionary.get("indices")
-        self.media_url_https = self.direct_url = self.__dictionary.get("media_url_https")
+        self.media_url_https = self.direct_url = self._get_direct_url()
         self.type = self.__dictionary.get("type")
         self.url = self.__dictionary.get("url")
         self.features = self.__dictionary.get("features")
         self.media_key = self.__dictionary.get("media_key")
         self.mediaStats = self.__dictionary.get("mediaStats")
         self.sizes = [MediaSize(k, v) for k, v in self.__dictionary.get("sizes").items() if self.__dictionary.get('sizes')]
         self.original_info = self.__dictionary.get("original_info")
@@ -397,14 +490,21 @@
         if self.type == "video" or self.type == "animated_gif":
             self.__parse_video_streams()
 
         for k, v in vars(self).items():
             if not k.startswith("_"):
                 self[k] = v
 
+    def _get_direct_url(self):
+        url = self.__dictionary.get("media_url_https")
+        if url.startswith("https://ton.twitter.com"):
+            url = f"{url}:small"
+
+        return url
+
     def _get_file_format(self):
         filename = os.path.basename(self.media_url_https).split("?")[0]
         return filename.split(".")[-1] if self.type == "photo" else "mp4"
 
     def __parse_video_streams(self):
         videoDict = self.__dictionary.get("video_info")
         if not videoDict:
@@ -649,14 +749,15 @@
         self.profile_image_url_https = self._get_key("profile_image_url_https")
         self.profile_interstitial_type = self._get_key("profile_interstitial_type")
         self.protected = self._get_key("protected")
         self.screen_name = self.username = self._get_key("screen_name")
         self.statuses_count = self._get_key("statuses_count")
         self.translator_type = self._get_key("translator_type")
         self.verified = self._get_verified()
+        self.can_dm = self._get_key("can_dm")
         # self.verified_type = self._get_key("verified_type")
         self.possibly_sensitive = self._get_key("possibly_sensitive")
         self.pinned_tweets = self._get_key("pinned_tweet_ids_str")
         self.profile_url = "https://twitter.com/{}".format(self.screen_name)
 
     def __repr__(self):
         return "User(id={}, username={}, name={}, verified={})".format(
```

### Comparing `tweety-ns-0.7.1/src/tweety/types/usertweet.py` & `tweety-ns-0.8/src/tweety/types/usertweet.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,9 +1,11 @@
 import time
 import traceback
+
+from .twDataTypes import TweetThread
 from ..exceptions_ import UserProtected, UserNotFound
 from . import Tweet, Excel, deprecated
 
 
 class UserTweets(dict):
     def __init__(self, user_id, http, pages=1, get_replies: bool = True, wait_time=2, cursor=None):
         super().__init__()
@@ -11,15 +13,14 @@
         self.get_replies = get_replies
         self.cursor = cursor
         self.is_next_page = True
         self.http = http
         self.user_id = user_id
         self.pages = pages
         self.wait_time = wait_time
-        # self._get_tweets(pages, wait_time)
 
     @staticmethod
     def _get_entries(response):
         instructions = response['data']['user']['result']['timeline_v2']['timeline']['instructions']
         for instruction in instructions:
             if instruction.get("type") == "TimelineAddEntries":
                 return instruction['entries']
@@ -30,14 +31,17 @@
     def _get_tweet_content_key(tweet):
         if str(tweet['entryId']).split("-")[0] == "tweet":
             return [tweet['content']['itemContent']['tweet_results']['result']]
 
         if str(tweet['entryId']).split("-")[0] == "homeConversation":
             return [item['item']['itemContent']['tweet_results']['result'] for item in tweet["content"]["items"]]
 
+        if str(tweet['entryId']).split("-")[0] == "profile" and str(tweet['entryId']).split("-")[1] == "conversation":
+            return [item['item']['itemContent']['tweet_results']['result'] for item in tweet["content"]["items"]]
+
         return []
 
     def get_next_page(self):
         _tweets = []
         if self.is_next_page:
             response = self.http.get_tweets(self.user_id, replies=self.get_replies, cursor=self.cursor)
 
@@ -47,21 +51,22 @@
             if response['data']['user']['result']['__typename'] == "UserUnavailable":
                 raise UserProtected(403, "UserUnavailable", None)
 
             entries = self._get_entries(response)
 
             for entry in entries:
                 tweets = self._get_tweet_content_key(entry)
-                for tweet in tweets:
-                    try:
-                        parsed = Tweet(response, tweet, self.http)
-                        _tweets.append(parsed)
-                        # yield parsed
-                    except:
-                        pass
+                try:
+                    if len(tweets) > 1:
+                        parsed = TweetThread(tweets, self.http, response)
+                    else:
+                        parsed = Tweet(tweets[0], self.http, response)
+                    _tweets.append(parsed)
+                except:
+                    pass
 
             self.is_next_page = self._get_cursor(entries)
 
             for tweet in _tweets:
                 self.tweets.append(tweet)
 
             self['tweets'] = self.tweets
@@ -90,27 +95,24 @@
 
                     self.cursor = newCursor
                     return True
 
         return False
 
     def to_xlsx(self, filename=None):
-        return Excel(self.tweets, self.tweets[0].author, filename)
+        return Excel(self, filename)
 
     def __getitem__(self, index):
         return self.tweets[index]
 
     def __iter__(self):
         for __tweet in self.tweets:
             yield __tweet
 
     def __len__(self):
         return len(self.tweets)
 
     def __repr__(self):
         return f"UserTweets(user_id={self.user_id}, count={self.__len__()})"
 
-    @deprecated
-    def to_dict(self):
-        return self.tweets
```

### Comparing `tweety-ns-0.7.1/src/tweety_ns.egg-info/SOURCES.txt` & `tweety-ns-0.8/src/tweety_ns.egg-info/SOURCES.txt`

 * *Files 12% similar despite different names*

```diff
@@ -4,16 +4,21 @@
 setup.py
 src/tweety/__init__.py
 src/tweety/bot.py
 src/tweety/builder.py
 src/tweety/exceptions_.py
 src/tweety/filters.py
 src/tweety/http.py
+src/tweety/updates.py
 src/tweety/utils.py
+src/tweety/events/__init__.py
+src/tweety/events/newmessage.py
 src/tweety/types/__init__.py
+src/tweety/types/inbox.py
+src/tweety/types/mentions.py
 src/tweety/types/n_types.py
 src/tweety/types/search.py
 src/tweety/types/twDataTypes.py
 src/tweety/types/usertweet.py
 src/tweety_ns.egg-info/PKG-INFO
 src/tweety_ns.egg-info/SOURCES.txt
 src/tweety_ns.egg-info/dependency_links.txt
```

