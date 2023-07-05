# Comparing `tmp/sneakpeek-0.8.1.tar.gz` & `tmp/sneakpeek-0.8.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sneakpeek-0.8.1.tar", max compression
+gzip compressed data, was "sneakpeek-0.8.2.tar", max compression
```

## Comparing `sneakpeek-0.8.1.tar` & `sneakpeek-0.8.2.tar`

### file list

```diff
@@ -1,9 +1,8 @@
--rw-r--r--   0        0        0     1096 2022-08-06 08:02:16.394602 sneakpeek-0.8.1/LICENSE
--rw-r--r--   0        0        0     8017 2022-08-09 07:58:52.451653 sneakpeek-0.8.1/README.md
--rw-r--r--   0        0        0     1564 2022-08-13 21:00:44.674666 sneakpeek-0.8.1/pyproject.toml
--rw-r--r--   0        0        0       56 2022-08-13 21:00:35.397950 sneakpeek-0.8.1/sneakpeek/__init__.py
--rw-r--r--   0        0        0     1213 2022-08-07 08:16:42.784012 sneakpeek-0.8.1/sneakpeek/console.py
--rw-r--r--   0        0        0      458 2022-08-06 20:19:19.735265 sneakpeek-0.8.1/sneakpeek/server.py
--rw-r--r--   0        0        0     5840 2022-08-13 20:56:33.996694 sneakpeek-0.8.1/sneakpeek/sneakpeek.py
--rw-r--r--   0        0        0     9405 2022-08-13 21:01:08.967166 sneakpeek-0.8.1/setup.py
--rw-r--r--   0        0        0     9638 2022-08-13 21:01:08.967610 sneakpeek-0.8.1/PKG-INFO
+-rw-r--r--   0        0        0     1096 2023-06-22 08:34:03.000000 sneakpeek-0.8.2/LICENSE
+-rw-r--r--   0        0        0     9150 2023-07-05 11:03:50.000000 sneakpeek-0.8.2/README.md
+-rw-r--r--   0        0        0     1582 2023-07-05 13:23:45.000000 sneakpeek-0.8.2/pyproject.toml
+-rw-r--r--   0        0        0       56 2023-07-05 13:23:51.000000 sneakpeek-0.8.2/sneakpeek/__init__.py
+-rw-r--r--   0        0        0     1245 2023-06-23 02:05:57.000000 sneakpeek-0.8.2/sneakpeek/console.py
+-rw-r--r--   0        0        0      458 2023-06-23 01:43:18.000000 sneakpeek-0.8.2/sneakpeek/server.py
+-rw-r--r--   0        0        0     4978 2023-07-05 11:34:49.000000 sneakpeek-0.8.2/sneakpeek/sneakpeek.py
+-rw-r--r--   0        0        0    10861 1970-01-01 00:00:00.000000 sneakpeek-0.8.2/PKG-INFO
```

### Comparing `sneakpeek-0.8.1/LICENSE` & `sneakpeek-0.8.2/LICENSE`

 * *Files identical despite different names*

### Comparing `sneakpeek-0.8.1/README.md` & `sneakpeek-0.8.2/README.md`

 * *Files 13% similar despite different names*

```diff
@@ -30,15 +30,15 @@
 ```
 
 
 ## Usage as a Python Module
 
 ### From a URL
 
-```sh
+```py
 >>> import sneakpeek
 >>> from pprint import pprint
 
 >>> link = sneakpeek.SneakPeek("https://www.youtube.com/watch?v=dQw4w9WgXcQ")
 >>> link.fetch()
 >>> link.is_valid()
 True
@@ -204,26 +204,43 @@
 poetry run pytest
 ```
 
 - Tested Websites
   - [x] [YouTube](https://youtube.com)
   - [x] [GitHub](https://github.com)
   - [x] [LinkedIN](https://linkedin.com)
-  - [x] [Reddit](https://reddit.com)
   - [x] [StackOverflow](https://stackoverflow.com)
   - [x] [Business Insider](https://www.businessinsider.in)
   - [x] [HackerNews](https://news.ycombinator.com/)
-  - [x] [Twitter](https://twitter.com)
 
 
 ## TODO
 
+- [ ] handle images ending in jpg / png etc
+  - [ ] the image could be this itself or a snap of the top part of the image
+  - [ ] the text can be AI generated or text detected in image
+  - [ ] https://i.ibb.co/ZLp46Kx/Screenshot-20230623-133028-Gmail.jpg
+- [ ] [Twitter](https://twitter.com) use v@ API with tweepy and have fallback as what is current
+- [ ] write a custom parser for [Reddit](https://reddit.com)
+- [ ] switch CLI to [typer](https://github.com/tiangolo/typer)
 - [ ] [Instagram](https://instagram.com) (using [instagram-scraper](https://github.com/arc298/instagram-scraper))
+- [ ] [Techcrunch](https://techcrunch.com/2023/06/23/pillow-discontinue/)
 - [ ] [Facebook](https://facebook.com)
 - [ ] CI/CD for publishing to PyPi
+- [ ] [Google](https://google.com) should show Google's image atleast
+- [ ] [LinkedIn](https://linkedin.com)
+- [ ] [HackerNews](https://news.ycombinator.com/) via API
+- [ ] safe image handling for sites like - https://techpays.eu/countries/germany
+- [ ] test cases
+  - [ ] test website without image
+  - [ ] test website without description
+  - [ ] test google should return custom Google image
+  - [ ] https://www.cnn.com/2022/07/07/tech/tech-layoffs-workers-silicon-valley/index.html
+  - [ ] https://edition.cnn.com/2022/07/07/tech/tech-layoffs-workers-silicon-valley/index.html
+  - [ ] https://www.levels.fyi/comp.html?track=Software+Engineer&showAll=true
 
 
 ## Contribution
 
 Have better suggestions to optimize the server image? Found some typos? Need special handling for a new website? Found a bug? Go ahead and create an [Issue](https://github.com/codingcoffee/sneakpeek/issues)! Contributions of any kind welcome!
 
 Want to work on a TODO? Its always a good idea to talk about what are going to do before you actually start it, so frustration can be avoided.
```

#### html2text {}

```diff
@@ -11,15 +11,15 @@
 sneakpeek)](https://hub.docker.com/r/codingcoffee/sneakpeek) [![Docker Image
 Size (tag)](https://img.shields.io/docker/image-size/codingcoffee/sneakpeek/
 latest)](https://hub.docker.com/r/codingcoffee/sneakpeek) ## What is supported
 - Any page which supports [Open Graph Protocol](https://ogp.me) (which most
 sane websites do) - Special handling for sites like - [Twitter](https://
 twitter.com) (requires a twitter [API key](https://developer.twitter.com/)) ##
 Installation Run the following to install ```sh pip install sneakpeek ``` ##
-Usage as a Python Module ### From a URL ```sh >>> import sneakpeek >>> from
+Usage as a Python Module ### From a URL ```py >>> import sneakpeek >>> from
 pprint import pprint >>> link = sneakpeek.SneakPeek("https://www.youtube.com/
 watch?v=dQw4w9WgXcQ") >>> link.fetch() >>> link.is_valid() True >>> pprint
 (link) {'description': 'The official video for âNever Gonna Give You Upâ by
 Rick ' 'AstleyTaken from the album âWhenever You Need Somebodyâ â '
 'deluxe 2CD and digital deluxe out 6th May ...', 'domain': 'www.youtube.com',
 'image': 'https://i.ytimg.com/vi/dQw4w9WgXcQ/maxresdefault.jpg', 'image:
 height': '720', 'image:width': '1280', 'scrape': False, 'site_name': 'YouTube',
@@ -79,23 +79,38 @@
 [here](https://developer.twitter.com/) - Create an app - Add the following
 variables as ENV vars ``` TWITTER_CONSUMER_KEY="sample"
 TWITTER_CONSUMER_SECRET="sample" TWITTER_ACCESS_TOKEN="sample"
 TWITTER_ACCESS_TOKEN_SECRET="sample" ``` ## Development ``` pip install -
 U poetry git clone https://github.com/codingcoffee/sneakpeek cd sneakpeek
 poetry install ``` ## Running Tests ```sh poetry run pytest ``` - Tested
 Websites - [x] [YouTube](https://youtube.com) - [x] [GitHub](https://
-github.com) - [x] [LinkedIN](https://linkedin.com) - [x] [Reddit](https://
-reddit.com) - [x] [StackOverflow](https://stackoverflow.com) - [x] [Business
-Insider](https://www.businessinsider.in) - [x] [HackerNews](https://
-news.ycombinator.com/) - [x] [Twitter](https://twitter.com) ## TODO - [ ]
-[Instagram](https://instagram.com) (using [instagram-scraper](https://
-github.com/arc298/instagram-scraper)) - [ ] [Facebook](https://facebook.com) -
-[ ] CI/CD for publishing to PyPi ## Contribution Have better suggestions to
-optimize the server image? Found some typos? Need special handling for a new
-website? Found a bug? Go ahead and create an [Issue](https://github.com/
-codingcoffee/sneakpeek/issues)! Contributions of any kind welcome! Want to work
-on a TODO? Its always a good idea to talk about what are going to do before you
-actually start it, so frustration can be avoided. Some rules for coding: - Use
-the code style the project uses - For each feature, make a seperate branch, so
-it can be reviewed separately - Use commits with a good description, so
-everyone can see what you did ## License The code in this repository has been
-released under the [MIT License](https://opensource.org/licenses/MIT)
+github.com) - [x] [LinkedIN](https://linkedin.com) - [x] [StackOverflow](https:
+//stackoverflow.com) - [x] [Business Insider](https://www.businessinsider.in) -
+[x] [HackerNews](https://news.ycombinator.com/) ## TODO - [ ] handle images
+ending in jpg / png etc - [ ] the image could be this itself or a snap of the
+top part of the image - [ ] the text can be AI generated or text detected in
+image - [ ] https://i.ibb.co/ZLp46Kx/Screenshot-20230623-133028-Gmail.jpg - [ ]
+[Twitter](https://twitter.com) use v@ API with tweepy and have fallback as what
+is current - [ ] write a custom parser for [Reddit](https://reddit.com) - [ ]
+switch CLI to [typer](https://github.com/tiangolo/typer) - [ ] [Instagram]
+(https://instagram.com) (using [instagram-scraper](https://github.com/arc298/
+instagram-scraper)) - [ ] [Techcrunch](https://techcrunch.com/2023/06/23/
+pillow-discontinue/) - [ ] [Facebook](https://facebook.com) - [ ] CI/CD for
+publishing to PyPi - [ ] [Google](https://google.com) should show Google's
+image atleast - [ ] [LinkedIn](https://linkedin.com) - [ ] [HackerNews](https:/
+/news.ycombinator.com/) via API - [ ] safe image handling for sites like -
+https://techpays.eu/countries/germany - [ ] test cases - [ ] test website
+without image - [ ] test website without description - [ ] test google should
+return custom Google image - [ ] https://www.cnn.com/2022/07/07/tech/tech-
+layoffs-workers-silicon-valley/index.html - [ ] https://edition.cnn.com/2022/
+07/07/tech/tech-layoffs-workers-silicon-valley/index.html - [ ] https://
+www.levels.fyi/comp.html?track=Software+Engineer&showAll=true ## Contribution
+Have better suggestions to optimize the server image? Found some typos? Need
+special handling for a new website? Found a bug? Go ahead and create an [Issue]
+(https://github.com/codingcoffee/sneakpeek/issues)! Contributions of any kind
+welcome! Want to work on a TODO? Its always a good idea to talk about what are
+going to do before you actually start it, so frustration can be avoided. Some
+rules for coding: - Use the code style the project uses - For each feature,
+make a seperate branch, so it can be reviewed separately - Use commits with a
+good description, so everyone can see what you did ## License The code in this
+repository has been released under the [MIT License](https://opensource.org/
+licenses/MIT)
```

### Comparing `sneakpeek-0.8.1/pyproject.toml` & `sneakpeek-0.8.2/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "sneakpeek"
-version = "0.8.1"
+version = "0.8.2"
 description = "A python module to generate link previews."
 license = "MIT"
 authors = ["Ameya Shenoy <shenoy.ameya@gmail.com>"]
 maintainers = ["Ameya Shenoy <shenoy.ameya@gmail.com>"]
 readme = "README.md"
 homepage = "https://github.com/codingcoffee/sneakpeek"
 repository = "https://github.com/codingcoffee/sneakpeek"
@@ -32,14 +32,15 @@
 validators = "^0.20.0"
 beautifulsoup4 = "^4.11.1"
 fastapi = "^0.79.0"
 click = "^8.1.3"
 uvicorn = "^0.18.2"
 rich = "^12.5.1"
 tweepy = "^4.10.0"
+loguru = "^0.7.0"
 
 [tool.poetry.dev-dependencies]
 pytest = "^7.1.2"
 
 [build-system]
 requires = ["poetry-core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
```

### Comparing `sneakpeek-0.8.1/sneakpeek/console.py` & `sneakpeek-0.8.2/sneakpeek/console.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 # third-party imprts
 import json
 
 import click
 import uvicorn
+from loguru import logger
 from rich import print
 
 # app imports
 from sneakpeek.server import get_link_preview
 
 
 @click.group()
@@ -17,15 +18,15 @@
 @click.command()
 @click.option("--host", default="localhost", help="Sever Host.")
 @click.option("--port", default=9000, help="Server Port.")
 @click.option("--reload", is_flag=True, help="Enable auto-reload on code change.")
 @click.option("--workers", default=2, help="No. of worker threads.")
 def serve(host, port, reload, workers):
     """Spin up a simple server using FastAPI."""
-    print(
+    logger.info(
         f"Starting a server on {host}:{port} "
         f"with auto reload {reload} and {workers} workers"
     )
     uvicorn.run(
         "sneakpeek.server:app", host=host, port=port, reload=reload, workers=workers
     )
```

### Comparing `sneakpeek-0.8.1/sneakpeek/sneakpeek.py` & `sneakpeek-0.8.2/sneakpeek/sneakpeek.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,35 +1,21 @@
 # encoding: utf-8
 
 """Module for SneakPeek."""
 
 # standard imports
 import json
-import os
 import re
 import urllib.request
 from urllib.parse import urlparse
 
 # third-party imports
-import tweepy
 import validators
 from bs4 import BeautifulSoup
-
-consumer_key = os.environ.get("TWITTER_CONSUMER_KEY", "")
-consumer_secret = os.environ.get("TWITTER_CONSUMER_SECRET", "")
-access_token = os.environ.get("TWITTER_ACCESS_TOKEN", "")
-access_token_secret = os.environ.get("TWITTER_ACCESS_TOKEN_SECRET", "")
-auth = tweepy.OAuth1UserHandler(consumer_key, consumer_secret)
-auth.set_access_token(access_token, access_token_secret)
-api = tweepy.API(auth)
-try:
-    api.verify_credentials()
-    TWITTER_SETUP = True
-except:
-    TWITTER_SETUP = False
+from loguru import logger
 
 
 class SneakPeek(dict):
     """ """
 
     required_attrs = ["title", "type", "image", "url", "description"]
 
@@ -62,53 +48,49 @@
 
     def __getattr__(self, name):
         return self[name]
 
     def is_valid_url(self, url=None):
         return validators.url(url)
 
-    def is_twitter_setup(self):
-        global TWITTER_SETUP
-        return TWITTER_SETUP
-
     def fetch_and_parse_twitter(self):
-        if not self.is_twitter_setup():
+        if not isinstance(self.url, str):
             return
         if "status" in self.url:
-            tweet_id = int(self.url.split("status/")[-1].split("?")[0])
-            status = api.get_status(tweet_id, tweet_mode="extended")
-            self.title = f"{status.user.name} on Twitter"
-            self.description = status.full_text
-            if status._json["entities"].get("media"):
-                self.image = status._json["entities"]["media"][0]["media_url_https"]
-            else:
-                self.image = status._json["user"]["profile_image_url_https"].replace(
-                    "_normal", ""
-                )
+            # tweet_id = int(self.url.split("status/")[-1].split("?")[0])
+            username = self.url.split("/")[3]
+            self.title = f"{username} on Twitter"
             self.type = "article"
-            self.created_at = status._json["created_at"]
+            self.description = ""
             return
+        elif self.url.strip("/").endswith(".com"):
+            self.title = "Twitter"
+            self.type = "website"
+            self.description = "Social Network Company"
         else:
             username = self.url.strip("/").split("/")[-1]
-            user = api.get_user(screen_name=username)
-            self.title = f"{user.name} (@{user.screen_name}) / Twitter"
+            self.title = f"{username} on Twitter"
             self.type = "profile"
-            self.description = user.description
-            self.image = user.profile_image_url_https.replace("_normal", "")
+            self.description = ""
+
+        self.image = "https://upload.wikimedia.org/wikipedia/commons/6/6f/Logo_of_Twitter.svg"
 
     def fetch(self):
         """ """
         if self.domain in ["twitter.com", "mobile.twitter.com", "www.twitter.com"]:
             return self.fetch_and_parse_twitter()
+        if not isinstance(self.url, str):
+            return
         # TODO: use random user agent for every request - https://github.com/Luqman-Ud-Din/random_user_agent
         req = urllib.request.Request(self.url, headers={"User-Agent": "Mozilla/5.0"})
         try:
             with urllib.request.urlopen(req) as raw:
                 html = raw.read()
         except Exception as err:
+            logger.debug("Unable to fetch data for URL")
             html = ""
             self.error = str(err)
             return
         return self.parse(html)
 
     def parse(self, html):
         """ """
@@ -169,25 +151,19 @@
 
     def scrape_title(self, doc):
         try:
             return doc.html.head.title.text
         except:
             return ""
 
-    def scrape_type(self, doc):
-        try:
-            return "other"
-        except:
-            return ""
+    def scrape_type(self, _):
+        return "other"
 
-    def scrape_url(self, doc):
-        try:
-            return self.url
-        except:
-            return ""
+    def scrape_url(self, _):
+        return self.url
 
     def scrape_description(self, doc):
         try:
             tag = doc.html.head.findAll("meta", attrs={"name": "description"})
             result = "".join([t["content"] for t in tag])
             return result
         except:
```

### Comparing `sneakpeek-0.8.1/setup.py` & `sneakpeek-0.8.2/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,40 +1,299 @@
-# -*- coding: utf-8 -*-
-from setuptools import setup
+Metadata-Version: 2.1
+Name: sneakpeek
+Version: 0.8.2
+Summary: A python module to generate link previews.
+Home-page: https://github.com/codingcoffee/sneakpeek
+License: MIT
+Keywords: open-graph-protocol,ogp,twitter,twitter-cards,python,schema,link-preview
+Author: Ameya Shenoy
+Author-email: shenoy.ameya@gmail.com
+Maintainer: Ameya Shenoy
+Maintainer-email: shenoy.ameya@gmail.com
+Requires-Python: >=3.7,<4.0
+Classifier: Development Status :: 4 - Beta
+Classifier: Intended Audience :: Developers
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Operating System :: POSIX :: Linux
+Classifier: Operating System :: Unix
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.7
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Topic :: Software Development :: Build Tools
+Classifier: Topic :: Software Development :: Libraries
+Classifier: Topic :: Software Development :: Libraries :: Python Modules
+Classifier: Topic :: Text Processing :: Markup :: HTML
+Classifier: Topic :: Utilities
+Requires-Dist: beautifulsoup4 (>=4.11.1,<5.0.0)
+Requires-Dist: click (>=8.1.3,<9.0.0)
+Requires-Dist: fastapi (>=0.79.0,<0.80.0)
+Requires-Dist: loguru (>=0.7.0,<0.8.0)
+Requires-Dist: rich (>=12.5.1,<13.0.0)
+Requires-Dist: tweepy (>=4.10.0,<5.0.0)
+Requires-Dist: uvicorn (>=0.18.2,<0.19.0)
+Requires-Dist: validators (>=0.20.0,<0.21.0)
+Project-URL: Documentation, https://github.com/codingcoffee/sneakpeek
+Project-URL: Repository, https://github.com/codingcoffee/sneakpeek
+Description-Content-Type: text/markdown
 
-packages = \
-['sneakpeek']
 
-package_data = \
-{'': ['*']}
+<div align="center">
+  <h1>
+    SneakPeek
+  </h1>
+  <h4>A python module and a minimalistic server to generate link previews.</h4>
+</div>
 
-install_requires = \
-['beautifulsoup4>=4.11.1,<5.0.0',
- 'click>=8.1.3,<9.0.0',
- 'fastapi>=0.79.0,<0.80.0',
- 'rich>=12.5.1,<13.0.0',
- 'tweepy>=4.10.0,<5.0.0',
- 'uvicorn>=0.18.2,<0.19.0',
- 'validators>=0.20.0,<0.21.0']
-
-entry_points = \
-{'console_scripts': ['sneakpeek = sneakpeek.console:cli']}
-
-setup_kwargs = {
-    'name': 'sneakpeek',
-    'version': '0.8.1',
-    'description': 'A python module to generate link previews.',
-    'long_description': '\n<div align="center">\n  <h1>\n    SneakPeek\n  </h1>\n  <h4>A python module and a minimalistic server to generate link previews.</h4>\n</div>\n\n[![License: MIT](https://img.shields.io/badge/License-MIT-green.svg)](https://opensource.org/licenses/MIT)\n[![Downloads](https://pepy.tech/badge/sneakpeek)](https://pepy.tech/project/sneakpeek)\n[![PyPI](https://img.shields.io/pypi/v/sneakpeek)](https://pypi.org/project/sneakpeek)\n[![PyPI - Python Version](https://img.shields.io/pypi/pyversions/sneakpeek)](https://pypi.org/project/sneakpeek)\n[![test-ci](https://img.shields.io/github/workflow/status/codingcoffee/sneakpeek/test-ci)](https://github.com/codingCoffee/sneakpeek/actions)\n[![Docker Pulls](https://img.shields.io/docker/pulls/codingcoffee/sneakpeek)](https://hub.docker.com/r/codingcoffee/sneakpeek)\n[![Docker Image Size (tag)](https://img.shields.io/docker/image-size/codingcoffee/sneakpeek/latest)](https://hub.docker.com/r/codingcoffee/sneakpeek)\n\n## What is supported\n\n- Any page which supports [Open Graph Protocol](https://ogp.me) (which most sane websites do)\n- Special handling for sites like\n  - [Twitter](https://twitter.com) (requires a twitter [API key](https://developer.twitter.com/))\n\n\n## Installation\n\nRun the following to install\n\n```sh\npip install sneakpeek\n```\n\n\n## Usage as a Python Module\n\n### From a URL\n\n```sh\n>>> import sneakpeek\n>>> from pprint import pprint\n\n>>> link = sneakpeek.SneakPeek("https://www.youtube.com/watch?v=dQw4w9WgXcQ")\n>>> link.fetch()\n>>> link.is_valid()\nTrue\n>>> pprint(link)\n{\'description\': \'The official video for “Never Gonna Give You Up” by Rick \'\n                \'AstleyTaken from the album ‘Whenever You Need Somebody’ – \'\n                \'deluxe 2CD and digital deluxe out 6th May ...\',\n \'domain\': \'www.youtube.com\',\n \'image\': \'https://i.ytimg.com/vi/dQw4w9WgXcQ/maxresdefault.jpg\',\n \'image:height\': \'720\',\n \'image:width\': \'1280\',\n \'scrape\': False,\n \'site_name\': \'YouTube\',\n \'title\': \'Rick Astley - Never Gonna Give You Up (Official Music Video)\',\n \'type\': \'video.other\',\n \'url\': \'https://www.youtube.com/watch?v=dQw4w9WgXcQ\',\n \'video:height\': \'720\',\n \'video:secure_url\': \'https://www.youtube.com/embed/dQw4w9WgXcQ\',\n \'video:tag\': \'never gonna give you up karaoke\',\n \'video:type\': \'text/html\',\n \'video:url\': \'https://www.youtube.com/embed/dQw4w9WgXcQ\',\n \'video:width\': \'1280\'}\n\n>>> link = sneakpeek.SneakPeek(url="https://codingcoffee.dev")\n>>> link.fetch()\n>>> pprint(link)\n{\'description\': \'A generalist with multi faceted interests and extensive \'\n                \'experience with DevOps, System Design and Full Stack \'\n                \'Development. I like blogging about things which interest me, \'\n                \'have a niche for optimizing and customizing things to the \'\n                \'very last detail, this includes my text editor and operating \'\n                \'system alike.\',\n \'domain\': \'codingcoffee.dev\',\n \'image\': \'https://www.gravatar.com/avatar/7ecdc5e1441ecd501faaf42a6ab9d6c0?s=200\',\n \'scrape\': False,\n \'title\': \'Ameya Shenoy\',\n \'type\': \'website\',\n \'url\': \'https://codingcoffee.dev\'}\n```\n\nUse `scrape=True` to fetch data using scraping instead of relying on open graph tags\n\n```sh\n>>> link = sneakpeek.SneakPeek(url="https://news.ycombinator.com/item?id=23812063", scrape=True)\n>>> link.fetch()\n>>> pprint(link)\n{\'description\': \'\',\n \'domain\': \'news.ycombinator.com\',\n \'image\': \'y18.gif\',\n \'scrape\': True,\n \'title\': \'WireGuard as VPN Server on Kubernetes with AdBlocking | Hacker News\',\n \'type\': \'other\',\n \'url\': \'https://news.ycombinator.com/item?id=23812063\'}\n ```\n\n### From HTML\n\n```\n>>> HTML = """\n... <html xmlns:og="http://ogp.me/ns">\n... <head>\n... <title>The Rock (1996)</title>\n... <meta property="og:title" content="The Rock" />\n... <meta property="og:description" content="The Rock: Directed by Michael Bay. With Sean Connery, Nicolas Cage, Ed Harris, John Spencer. A mild-mannered chemist and an ex-con must lead the counterstrike when a rogue group of military men, led by a renegade general, threaten a nerve gas attack from Alcatraz against San Francisco.">\n... <meta property="og:type" content="movie" />\n... <meta property="og:url" content="http://www.imdb.com/title/tt0117500/" />\n... <meta property="og:image" content="https://m.media-amazon.com/images/M/MV5BZDJjOTE0N2EtMmRlZS00NzU0LWE0ZWQtM2Q3MWMxNjcwZjBhXkEyXkFqcGdeQXVyNDk3NzU2MTQ@._V1_FMjpg_UX1000_.jpg">\n... </head>\n... </html>\n... """\n>>> movie = sneakpeek.SneakPeek(html=HTML)\n>>> movie.is_valid()\nTrue\n>>> pprint(movie)\n{\'description\': \'The Rock: Directed by Michael Bay. With Sean Connery, Nicolas \'\n                \'Cage, Ed Harris, John Spencer. A mild-mannered chemist and an \'\n                \'ex-con must lead the counterstrike when a rogue group of \'\n                \'military men, led by a renegade general, threaten a nerve gas \'\n                \'attack from Alcatraz against San Francisco.\',\n \'domain\': None,\n \'image\': \'https://m.media-amazon.com/images/M/MV5BZDJjOTE0N2EtMmRlZS00NzU0LWE0ZWQtM2Q3MWMxNjcwZjBhXkEyXkFqcGdeQXVyNDk3NzU2MTQ@._V1_FMjpg_UX1000_.jpg\',\n \'scrape\': False,\n \'title\': \'The Rock\',\n \'type\': \'movie\',\n \'url\': \'http://www.imdb.com/title/tt0117500/\'}\n```\n\n\n## Usage as a Server\n\nA simple server using FastAPI and uvicorn is used to serve the requests.\n\n```sh\nsneekpeek serve\n```\n\nYou can view the docs at http://localhost:9000/docs\n\n\n## Usage as a CLI\n\n```\nsneakpeek preview --url "https://github.com/codingcoffee/" | jq\n{\n  "domain": "github.com",\n  "scrape": false,\n  "url": "https://github.com/codingCoffee",\n  "title": "codingCoffee - Overview",\n  "type": "profile",\n  "image": "https://avatars.githubusercontent.com/u/13611153?v=4?s=400",\n  "description": "Automate anything and everything 🙋\u200d♂️. codingCoffee has 68 repositories available. Follow their code on GitHub.",\n  "error": null,\n  "image:alt": "Automate anything and everything 🙋\u200d♂️. codingCoffee has 68 repositories available. Follow their code on GitHub.",\n  "site_name": "GitHub"\n}\n```\n\n## Docker\n\n### As a Server\n\n```sh\ndocker run -it --rm -p 9000:9000 codingcoffee/sneakpeek -- serve --host 0.0.0.0\n```\n\n### As a CLI\n\n```sh\ndocker run -it --rm -p 9000:9000 codingcoffee/sneakpeek -- preview --url "https://github.com/codingcoffee"\n```\n\n\n## Configuration\n\n### Twitter\n\n- Sign up for a developer account on twitter [here](https://developer.twitter.com/)\n- Create an app\n- Add the following variables as ENV vars\n\n\n```\nTWITTER_CONSUMER_KEY="sample"\nTWITTER_CONSUMER_SECRET="sample"\nTWITTER_ACCESS_TOKEN="sample"\nTWITTER_ACCESS_TOKEN_SECRET="sample"\n```\n\n\n## Development\n\n```\npip install -U poetry\ngit clone https://github.com/codingcoffee/sneakpeek\ncd sneakpeek\npoetry install\n```\n\n\n## Running Tests\n\n```sh\npoetry run pytest\n```\n\n- Tested Websites\n  - [x] [YouTube](https://youtube.com)\n  - [x] [GitHub](https://github.com)\n  - [x] [LinkedIN](https://linkedin.com)\n  - [x] [Reddit](https://reddit.com)\n  - [x] [StackOverflow](https://stackoverflow.com)\n  - [x] [Business Insider](https://www.businessinsider.in)\n  - [x] [HackerNews](https://news.ycombinator.com/)\n  - [x] [Twitter](https://twitter.com)\n\n\n## TODO\n\n- [ ] [Instagram](https://instagram.com) (using [instagram-scraper](https://github.com/arc298/instagram-scraper))\n- [ ] [Facebook](https://facebook.com)\n- [ ] CI/CD for publishing to PyPi\n\n\n## Contribution\n\nHave better suggestions to optimize the server image? Found some typos? Need special handling for a new website? Found a bug? Go ahead and create an [Issue](https://github.com/codingcoffee/sneakpeek/issues)! Contributions of any kind welcome!\n\nWant to work on a TODO? Its always a good idea to talk about what are going to do before you actually start it, so frustration can be avoided.\n\nSome rules for coding:\n\n- Use the code style the project uses\n- For each feature, make a seperate branch, so it can be reviewed separately\n- Use commits with a good description, so everyone can see what you did\n\n\n## License\n\nThe code in this repository has been released under the [MIT License](https://opensource.org/licenses/MIT)\n\n',
-    'author': 'Ameya Shenoy',
-    'author_email': 'shenoy.ameya@gmail.com',
-    'maintainer': 'Ameya Shenoy',
-    'maintainer_email': 'shenoy.ameya@gmail.com',
-    'url': 'https://github.com/codingcoffee/sneakpeek',
-    'packages': packages,
-    'package_data': package_data,
-    'install_requires': install_requires,
-    'entry_points': entry_points,
-    'python_requires': '>=3.7,<4.0',
+[![License: MIT](https://img.shields.io/badge/License-MIT-green.svg)](https://opensource.org/licenses/MIT)
+[![Downloads](https://pepy.tech/badge/sneakpeek)](https://pepy.tech/project/sneakpeek)
+[![PyPI](https://img.shields.io/pypi/v/sneakpeek)](https://pypi.org/project/sneakpeek)
+[![PyPI - Python Version](https://img.shields.io/pypi/pyversions/sneakpeek)](https://pypi.org/project/sneakpeek)
+[![test-ci](https://img.shields.io/github/workflow/status/codingcoffee/sneakpeek/test-ci)](https://github.com/codingCoffee/sneakpeek/actions)
+[![Docker Pulls](https://img.shields.io/docker/pulls/codingcoffee/sneakpeek)](https://hub.docker.com/r/codingcoffee/sneakpeek)
+[![Docker Image Size (tag)](https://img.shields.io/docker/image-size/codingcoffee/sneakpeek/latest)](https://hub.docker.com/r/codingcoffee/sneakpeek)
+
+## What is supported
+
+- Any page which supports [Open Graph Protocol](https://ogp.me) (which most sane websites do)
+- Special handling for sites like
+  - [Twitter](https://twitter.com) (requires a twitter [API key](https://developer.twitter.com/))
+
+
+## Installation
+
+Run the following to install
+
+```sh
+pip install sneakpeek
+```
+
+
+## Usage as a Python Module
+
+### From a URL
+
+```py
+>>> import sneakpeek
+>>> from pprint import pprint
+
+>>> link = sneakpeek.SneakPeek("https://www.youtube.com/watch?v=dQw4w9WgXcQ")
+>>> link.fetch()
+>>> link.is_valid()
+True
+>>> pprint(link)
+{'description': 'The official video for “Never Gonna Give You Up” by Rick '
+                'AstleyTaken from the album ‘Whenever You Need Somebody’ – '
+                'deluxe 2CD and digital deluxe out 6th May ...',
+ 'domain': 'www.youtube.com',
+ 'image': 'https://i.ytimg.com/vi/dQw4w9WgXcQ/maxresdefault.jpg',
+ 'image:height': '720',
+ 'image:width': '1280',
+ 'scrape': False,
+ 'site_name': 'YouTube',
+ 'title': 'Rick Astley - Never Gonna Give You Up (Official Music Video)',
+ 'type': 'video.other',
+ 'url': 'https://www.youtube.com/watch?v=dQw4w9WgXcQ',
+ 'video:height': '720',
+ 'video:secure_url': 'https://www.youtube.com/embed/dQw4w9WgXcQ',
+ 'video:tag': 'never gonna give you up karaoke',
+ 'video:type': 'text/html',
+ 'video:url': 'https://www.youtube.com/embed/dQw4w9WgXcQ',
+ 'video:width': '1280'}
+
+>>> link = sneakpeek.SneakPeek(url="https://codingcoffee.dev")
+>>> link.fetch()
+>>> pprint(link)
+{'description': 'A generalist with multi faceted interests and extensive '
+                'experience with DevOps, System Design and Full Stack '
+                'Development. I like blogging about things which interest me, '
+                'have a niche for optimizing and customizing things to the '
+                'very last detail, this includes my text editor and operating '
+                'system alike.',
+ 'domain': 'codingcoffee.dev',
+ 'image': 'https://www.gravatar.com/avatar/7ecdc5e1441ecd501faaf42a6ab9d6c0?s=200',
+ 'scrape': False,
+ 'title': 'Ameya Shenoy',
+ 'type': 'website',
+ 'url': 'https://codingcoffee.dev'}
+```
+
+Use `scrape=True` to fetch data using scraping instead of relying on open graph tags
+
+```sh
+>>> link = sneakpeek.SneakPeek(url="https://news.ycombinator.com/item?id=23812063", scrape=True)
+>>> link.fetch()
+>>> pprint(link)
+{'description': '',
+ 'domain': 'news.ycombinator.com',
+ 'image': 'y18.gif',
+ 'scrape': True,
+ 'title': 'WireGuard as VPN Server on Kubernetes with AdBlocking | Hacker News',
+ 'type': 'other',
+ 'url': 'https://news.ycombinator.com/item?id=23812063'}
+ ```
+
+### From HTML
+
+```
+>>> HTML = """
+... <html xmlns:og="http://ogp.me/ns">
+... <head>
+... <title>The Rock (1996)</title>
+... <meta property="og:title" content="The Rock" />
+... <meta property="og:description" content="The Rock: Directed by Michael Bay. With Sean Connery, Nicolas Cage, Ed Harris, John Spencer. A mild-mannered chemist and an ex-con must lead the counterstrike when a rogue group of military men, led by a renegade general, threaten a nerve gas attack from Alcatraz against San Francisco.">
+... <meta property="og:type" content="movie" />
+... <meta property="og:url" content="http://www.imdb.com/title/tt0117500/" />
+... <meta property="og:image" content="https://m.media-amazon.com/images/M/MV5BZDJjOTE0N2EtMmRlZS00NzU0LWE0ZWQtM2Q3MWMxNjcwZjBhXkEyXkFqcGdeQXVyNDk3NzU2MTQ@._V1_FMjpg_UX1000_.jpg">
+... </head>
+... </html>
+... """
+>>> movie = sneakpeek.SneakPeek(html=HTML)
+>>> movie.is_valid()
+True
+>>> pprint(movie)
+{'description': 'The Rock: Directed by Michael Bay. With Sean Connery, Nicolas '
+                'Cage, Ed Harris, John Spencer. A mild-mannered chemist and an '
+                'ex-con must lead the counterstrike when a rogue group of '
+                'military men, led by a renegade general, threaten a nerve gas '
+                'attack from Alcatraz against San Francisco.',
+ 'domain': None,
+ 'image': 'https://m.media-amazon.com/images/M/MV5BZDJjOTE0N2EtMmRlZS00NzU0LWE0ZWQtM2Q3MWMxNjcwZjBhXkEyXkFqcGdeQXVyNDk3NzU2MTQ@._V1_FMjpg_UX1000_.jpg',
+ 'scrape': False,
+ 'title': 'The Rock',
+ 'type': 'movie',
+ 'url': 'http://www.imdb.com/title/tt0117500/'}
+```
+
+
+## Usage as a Server
+
+A simple server using FastAPI and uvicorn is used to serve the requests.
+
+```sh
+sneekpeek serve
+```
+
+You can view the docs at http://localhost:9000/docs
+
+
+## Usage as a CLI
+
+```
+sneakpeek preview --url "https://github.com/codingcoffee/" | jq
+{
+  "domain": "github.com",
+  "scrape": false,
+  "url": "https://github.com/codingCoffee",
+  "title": "codingCoffee - Overview",
+  "type": "profile",
+  "image": "https://avatars.githubusercontent.com/u/13611153?v=4?s=400",
+  "description": "Automate anything and everything 🙋‍♂️. codingCoffee has 68 repositories available. Follow their code on GitHub.",
+  "error": null,
+  "image:alt": "Automate anything and everything 🙋‍♂️. codingCoffee has 68 repositories available. Follow their code on GitHub.",
+  "site_name": "GitHub"
 }
+```
+
+## Docker
+
+### As a Server
+
+```sh
+docker run -it --rm -p 9000:9000 codingcoffee/sneakpeek -- serve --host 0.0.0.0
+```
+
+### As a CLI
+
+```sh
+docker run -it --rm -p 9000:9000 codingcoffee/sneakpeek -- preview --url "https://github.com/codingcoffee"
+```
+
+
+## Configuration
+
+### Twitter
+
+- Sign up for a developer account on twitter [here](https://developer.twitter.com/)
+- Create an app
+- Add the following variables as ENV vars
+
+
+```
+TWITTER_CONSUMER_KEY="sample"
+TWITTER_CONSUMER_SECRET="sample"
+TWITTER_ACCESS_TOKEN="sample"
+TWITTER_ACCESS_TOKEN_SECRET="sample"
+```
+
+
+## Development
+
+```
+pip install -U poetry
+git clone https://github.com/codingcoffee/sneakpeek
+cd sneakpeek
+poetry install
+```
+
+
+## Running Tests
+
+```sh
+poetry run pytest
+```
+
+- Tested Websites
+  - [x] [YouTube](https://youtube.com)
+  - [x] [GitHub](https://github.com)
+  - [x] [LinkedIN](https://linkedin.com)
+  - [x] [StackOverflow](https://stackoverflow.com)
+  - [x] [Business Insider](https://www.businessinsider.in)
+  - [x] [HackerNews](https://news.ycombinator.com/)
+
+
+## TODO
+
+- [ ] handle images ending in jpg / png etc
+  - [ ] the image could be this itself or a snap of the top part of the image
+  - [ ] the text can be AI generated or text detected in image
+  - [ ] https://i.ibb.co/ZLp46Kx/Screenshot-20230623-133028-Gmail.jpg
+- [ ] [Twitter](https://twitter.com) use v@ API with tweepy and have fallback as what is current
+- [ ] write a custom parser for [Reddit](https://reddit.com)
+- [ ] switch CLI to [typer](https://github.com/tiangolo/typer)
+- [ ] [Instagram](https://instagram.com) (using [instagram-scraper](https://github.com/arc298/instagram-scraper))
+- [ ] [Techcrunch](https://techcrunch.com/2023/06/23/pillow-discontinue/)
+- [ ] [Facebook](https://facebook.com)
+- [ ] CI/CD for publishing to PyPi
+- [ ] [Google](https://google.com) should show Google's image atleast
+- [ ] [LinkedIn](https://linkedin.com)
+- [ ] [HackerNews](https://news.ycombinator.com/) via API
+- [ ] safe image handling for sites like - https://techpays.eu/countries/germany
+- [ ] test cases
+  - [ ] test website without image
+  - [ ] test website without description
+  - [ ] test google should return custom Google image
+  - [ ] https://www.cnn.com/2022/07/07/tech/tech-layoffs-workers-silicon-valley/index.html
+  - [ ] https://edition.cnn.com/2022/07/07/tech/tech-layoffs-workers-silicon-valley/index.html
+  - [ ] https://www.levels.fyi/comp.html?track=Software+Engineer&showAll=true
+
+
+## Contribution
+
+Have better suggestions to optimize the server image? Found some typos? Need special handling for a new website? Found a bug? Go ahead and create an [Issue](https://github.com/codingcoffee/sneakpeek/issues)! Contributions of any kind welcome!
+
+Want to work on a TODO? Its always a good idea to talk about what are going to do before you actually start it, so frustration can be avoided.
+
+Some rules for coding:
+
+- Use the code style the project uses
+- For each feature, make a seperate branch, so it can be reviewed separately
+- Use commits with a good description, so everyone can see what you did
+
+
+## License
+
+The code in this repository has been released under the [MIT License](https://opensource.org/licenses/MIT)
 
 
-setup(**setup_kwargs)
```

