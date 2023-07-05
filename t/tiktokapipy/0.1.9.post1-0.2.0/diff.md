# Comparing `tmp/tiktokapipy-0.1.9.post1.tar.gz` & `tmp/tiktokapipy-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tiktokapipy-0.1.9.post1.tar", last modified: Thu Jan 12 02:35:52 2023, max compression
+gzip compressed data, was "tiktokapipy-0.2.0.tar", last modified: Wed Jul  5 16:47:46 2023, max compression
```

## Comparing `tiktokapipy-0.1.9.post1.tar` & `tiktokapipy-0.2.0.tar`

### file list

```diff
@@ -1,24 +1,35 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-12 02:35:52.334649 tiktokapipy-0.1.9.post1/
--rw-r--r--   0 runner    (1001) docker     (123)     1071 2023-01-12 02:35:40.000000 tiktokapipy-0.1.9.post1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     3676 2023-01-12 02:35:52.330649 tiktokapipy-0.1.9.post1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2460 2023-01-12 02:35:40.000000 tiktokapipy-0.1.9.post1/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     1558 2023-01-12 02:35:40.000000 tiktokapipy-0.1.9.post1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-01-12 02:35:52.334649 tiktokapipy-0.1.9.post1/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-12 02:35:52.330649 tiktokapipy-0.1.9.post1/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-12 02:35:52.330649 tiktokapipy-0.1.9.post1/src/tiktokapipy/
--rw-r--r--   0 runner    (1001) docker     (123)       93 2023-01-12 02:35:40.000000 tiktokapipy-0.1.9.post1/src/tiktokapipy/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    17476 2023-01-12 02:35:40.000000 tiktokapipy-0.1.9.post1/src/tiktokapipy/api.py
--rw-r--r--   0 runner    (1001) docker     (123)     7676 2023-01-12 02:35:40.000000 tiktokapipy-0.1.9.post1/src/tiktokapipy/async_api.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-12 02:35:52.330649 tiktokapipy-0.1.9.post1/src/tiktokapipy/models/
--rw-r--r--   0 runner    (1001) docker     (123)     4085 2023-01-12 02:35:40.000000 tiktokapipy-0.1.9.post1/src/tiktokapipy/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1297 2023-01-12 02:35:40.000000 tiktokapipy-0.1.9.post1/src/tiktokapipy/models/challenge.py
--rw-r--r--   0 runner    (1001) docker     (123)     2156 2023-01-12 02:35:40.000000 tiktokapipy-0.1.9.post1/src/tiktokapipy/models/comment.py
--rw-r--r--   0 runner    (1001) docker     (123)     4074 2023-01-12 02:35:40.000000 tiktokapipy-0.1.9.post1/src/tiktokapipy/models/raw_data.py
--rw-r--r--   0 runner    (1001) docker     (123)     2990 2023-01-12 02:35:40.000000 tiktokapipy-0.1.9.post1/src/tiktokapipy/models/user.py
--rw-r--r--   0 runner    (1001) docker     (123)     5891 2023-01-12 02:35:40.000000 tiktokapipy-0.1.9.post1/src/tiktokapipy/models/video.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-12 02:35:52.330649 tiktokapipy-0.1.9.post1/src/tiktokapipy.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3676 2023-01-12 02:35:52.000000 tiktokapipy-0.1.9.post1/src/tiktokapipy.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      509 2023-01-12 02:35:52.000000 tiktokapipy-0.1.9.post1/src/tiktokapipy.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-01-12 02:35:52.000000 tiktokapipy-0.1.9.post1/src/tiktokapipy.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      186 2023-01-12 02:35:52.000000 tiktokapipy-0.1.9.post1/src/tiktokapipy.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       12 2023-01-12 02:35:52.000000 tiktokapipy-0.1.9.post1/src/tiktokapipy.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 16:47:46.015465 tiktokapipy-0.2.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1071 2023-07-05 16:47:33.000000 tiktokapipy-0.2.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     4288 2023-07-05 16:47:46.015465 tiktokapipy-0.2.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3078 2023-07-05 16:47:33.000000 tiktokapipy-0.2.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1549 2023-07-05 16:47:33.000000 tiktokapipy-0.2.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-05 16:47:46.015465 tiktokapipy-0.2.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 16:47:46.011465 tiktokapipy-0.2.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 16:47:46.015465 tiktokapipy-0.2.0/src/tiktokapipy/
+-rw-r--r--   0 runner    (1001) docker     (123)     1385 2023-07-05 16:47:33.000000 tiktokapipy-0.2.0/src/tiktokapipy/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11278 2023-07-05 16:47:33.000000 tiktokapipy-0.2.0/src/tiktokapipy/api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5805 2023-07-05 16:47:33.000000 tiktokapipy-0.2.0/src/tiktokapipy/async_api.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 16:47:46.015465 tiktokapipy-0.2.0/src/tiktokapipy/models/
+-rw-r--r--   0 runner    (1001) docker     (123)     1631 2023-07-05 16:47:33.000000 tiktokapipy-0.2.0/src/tiktokapipy/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2050 2023-07-05 16:47:33.000000 tiktokapipy-0.2.0/src/tiktokapipy/models/challenge.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3278 2023-07-05 16:47:33.000000 tiktokapipy-0.2.0/src/tiktokapipy/models/comment.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2794 2023-07-05 16:47:33.000000 tiktokapipy-0.2.0/src/tiktokapipy/models/raw_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3790 2023-07-05 16:47:33.000000 tiktokapipy-0.2.0/src/tiktokapipy/models/user.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7727 2023-07-05 16:47:33.000000 tiktokapipy-0.2.0/src/tiktokapipy/models/video.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 16:47:46.015465 tiktokapipy-0.2.0/src/tiktokapipy/util/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-05 16:47:33.000000 tiktokapipy-0.2.0/src/tiktokapipy/util/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10422 2023-07-05 16:47:33.000000 tiktokapipy-0.2.0/src/tiktokapipy/util/deferred_collectors.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6148 2023-07-05 16:47:33.000000 tiktokapipy-0.2.0/src/tiktokapipy/util/queries.py
+-rw-r--r--   0 runner    (1001) docker     (123)    52530 2023-07-05 16:47:33.000000 tiktokapipy-0.2.0/src/tiktokapipy/util/signing.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 16:47:46.015465 tiktokapipy-0.2.0/src/tiktokapipy.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4288 2023-07-05 16:47:46.000000 tiktokapipy-0.2.0/src/tiktokapipy.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      758 2023-07-05 16:47:46.000000 tiktokapipy-0.2.0/src/tiktokapipy.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-05 16:47:46.000000 tiktokapipy-0.2.0/src/tiktokapipy.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      176 2023-07-05 16:47:46.000000 tiktokapipy-0.2.0/src/tiktokapipy.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-07-05 16:47:46.000000 tiktokapipy-0.2.0/src/tiktokapipy.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 16:47:46.015465 tiktokapipy-0.2.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     1249 2023-07-05 16:47:33.000000 tiktokapipy-0.2.0/tests/test_challenge.py
+-rw-r--r--   0 runner    (1001) docker     (123)      355 2023-07-05 16:47:33.000000 tiktokapipy-0.2.0/tests/test_errors.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1243 2023-07-05 16:47:33.000000 tiktokapipy-0.2.0/tests/test_slideshow.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1167 2023-07-05 16:47:33.000000 tiktokapipy-0.2.0/tests/test_user.py
+-rw-r--r--   0 runner    (1001) docker     (123)      611 2023-07-05 16:47:33.000000 tiktokapipy-0.2.0/tests/test_video.py
```

### Comparing `tiktokapipy-0.1.9.post1/LICENSE` & `tiktokapipy-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `tiktokapipy-0.1.9.post1/PKG-INFO` & `tiktokapipy-0.2.0/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tiktokapipy
-Version: 0.1.9.post1
+Version: 0.2.0
 Summary: Asyncio TikTok data scraping tool
 Author-email: Russell Newton <russell.newton01@gmail.com>
 Project-URL: Homepage, https://github.com/Russell-Newton/TikTokPy
 Project-URL: Documentation, https://tiktokpy.readthedocs.io/en/latest/
 Keywords: tiktok,python3,scraper,unofficial,tiktok-scraper,tiktok scraper,asyncio,playwright-python
 Classifier: Development Status :: 3 - Alpha
 Classifier: Framework :: AsyncIO
@@ -50,14 +50,15 @@
 
 ## Table of Contents
 
 * [Getting Started](#getting-started)
     * [Installation](#installation)
     * [Quick Start Guide](#quick-start-guide)
 * [Documentation](#documentation)
+* [Disclaimer](#disclaimer)
 
 ## Getting Started
 
 ### Installation
 
 Install the ``tiktokapipy`` package (or add it to your project requirements) and set up Playwright:
 
@@ -103,10 +104,26 @@
 </td>
 </tr>
 </table>
 
 More examples, including how to download videos and slideshows, can be found in the
 [documentation](https://tiktokpy.readthedocs.io/en/latest/users/usage.html#examples).
 
+Warnings can be ignored as follows:
+
+```py
+import warnings
+
+from tiktokapipy import TikTokAPIWarning
+
+warnings.filterwarnings("ignore", category=TikTokAPIWarning)
+```
+
 ## Documentation
 
 You can view the full documentation on [Read the Docs](https://tiktokpy.readthedocs.io/en/latest/).
+
+<hr>
+
+## Disclaimer
+
+TikTokPy is in no way affiliated with, authorized, maintained, sponsored or endorsed by TikTok or any of its affiliates or subsidiaries. Use of automated scripts to collect information from or otherwise interact with TikTok and its related services is against [TikTok's Terms of Service](https://www.tiktok.com/legal/page/us/terms-of-service/en). Use at your own risk. For educational purposes only.
```

#### html2text {}

```diff
@@ -1,9 +1,9 @@
-Metadata-Version: 2.1 Name: tiktokapipy Version: 0.1.9.post1 Summary: Asyncio
-TikTok data scraping tool Author-email: Russell Newton
+Metadata-Version: 2.1 Name: tiktokapipy Version: 0.2.0 Summary: Asyncio TikTok
+data scraping tool Author-email: Russell Newton
 newton01@gmail.com> Project-URL: Homepage, https://github.com/Russell-Newton/
 TikTokPy Project-URL: Documentation, https://tiktokpy.readthedocs.io/en/latest/
 Keywords: tiktok,python3,scraper,unofficial,tiktok-scraper,tiktok
 scraper,asyncio,playwright-python Classifier: Development Status :: 3 - Alpha
 Classifier: Framework :: AsyncIO Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Information Technology Classifier: Intended
 Audience :: Science/Research Classifier: License :: OSI Approved :: MIT License
@@ -16,23 +16,32 @@
 text/markdown Provides-Extra: test Provides-Extra: docs License-File: LICENSE
                             ****** TikTokPy ******
                     [PyPI] [Python_Version_3.8+] [License]
                   [Unit_Tests_Status] [Documentation_Status]
 **Extract data from TikTok without needing any login information or API keys.**
 ## Table of Contents * [Getting Started](#getting-started) * [Installation]
 (#installation) * [Quick Start Guide](#quick-start-guide) * [Documentation]
-(#documentation) ## Getting Started ### Installation Install the
-``tiktokapipy`` package (or add it to your project requirements) and set up
-Playwright: ```shell pip install tiktokapipy python -m playwright install ```
-### Quick Start Guide TikTokPy has both a synchronous and an asynchronous API.
-The interfaces are the same, but the asynchronous API requires awaiting of
-certain functions and iterators. Both APIs must be used as context managers. To
-get video information in both APIs:
+(#documentation) * [Disclaimer](#disclaimer) ## Getting Started ###
+Installation Install the ``tiktokapipy`` package (or add it to your project
+requirements) and set up Playwright: ```shell pip install tiktokapipy python -
+m playwright install ``` ### Quick Start Guide TikTokPy has both a synchronous
+and an asynchronous API. The interfaces are the same, but the asynchronous API
+requires awaiting of certain functions and iterators. Both APIs must be used as
+context managers. To get video information in both APIs:
 Synchronous                           Asynchronous
 ```py from tiktokapipy.api import     ```py from tiktokapipy.async_api import
 TikTokAPI with TikTokAPI() as api:    AsyncTikTokAPI async with AsyncTikTokAPI
 video = api.video(video_link) ... ``` () as api: video = await api.video
                                       (video_link) ... ```
 More examples, including how to download videos and slideshows, can be found in
 the [documentation](https://tiktokpy.readthedocs.io/en/latest/users/
-usage.html#examples). ## Documentation You can view the full documentation on
-[Read the Docs](https://tiktokpy.readthedocs.io/en/latest/).
+usage.html#examples). Warnings can be ignored as follows: ```py import warnings
+from tiktokapipy import TikTokAPIWarning warnings.filterwarnings("ignore",
+category=TikTokAPIWarning) ``` ## Documentation You can view the full
+documentation on [Read the Docs](https://tiktokpy.readthedocs.io/en/latest/).
+===============================================================================
+## Disclaimer TikTokPy is in no way affiliated with, authorized, maintained,
+sponsored or endorsed by TikTok or any of its affiliates or subsidiaries. Use
+of automated scripts to collect information from or otherwise interact with
+TikTok and its related services is against [TikTok's Terms of Service](https://
+www.tiktok.com/legal/page/us/terms-of-service/en). Use at your own risk. For
+educational purposes only.
```

### Comparing `tiktokapipy-0.1.9.post1/README.md` & `tiktokapipy-0.2.0/README.md`

 * *Files 9% similar despite different names*

```diff
@@ -22,14 +22,15 @@
 
 ## Table of Contents
 
 * [Getting Started](#getting-started)
     * [Installation](#installation)
     * [Quick Start Guide](#quick-start-guide)
 * [Documentation](#documentation)
+* [Disclaimer](#disclaimer)
 
 ## Getting Started
 
 ### Installation
 
 Install the ``tiktokapipy`` package (or add it to your project requirements) and set up Playwright:
 
@@ -75,10 +76,26 @@
 </td>
 </tr>
 </table>
 
 More examples, including how to download videos and slideshows, can be found in the
 [documentation](https://tiktokpy.readthedocs.io/en/latest/users/usage.html#examples).
 
+Warnings can be ignored as follows:
+
+```py
+import warnings
+
+from tiktokapipy import TikTokAPIWarning
+
+warnings.filterwarnings("ignore", category=TikTokAPIWarning)
+```
+
 ## Documentation
 
 You can view the full documentation on [Read the Docs](https://tiktokpy.readthedocs.io/en/latest/).
+
+<hr>
+
+## Disclaimer
+
+TikTokPy is in no way affiliated with, authorized, maintained, sponsored or endorsed by TikTok or any of its affiliates or subsidiaries. Use of automated scripts to collect information from or otherwise interact with TikTok and its related services is against [TikTok's Terms of Service](https://www.tiktok.com/legal/page/us/terms-of-service/en). Use at your own risk. For educational purposes only.
```

#### html2text {}

```diff
@@ -1,22 +1,31 @@
                             ****** TikTokPy ******
                     [PyPI] [Python_Version_3.8+] [License]
                   [Unit_Tests_Status] [Documentation_Status]
 **Extract data from TikTok without needing any login information or API keys.**
 ## Table of Contents * [Getting Started](#getting-started) * [Installation]
 (#installation) * [Quick Start Guide](#quick-start-guide) * [Documentation]
-(#documentation) ## Getting Started ### Installation Install the
-``tiktokapipy`` package (or add it to your project requirements) and set up
-Playwright: ```shell pip install tiktokapipy python -m playwright install ```
-### Quick Start Guide TikTokPy has both a synchronous and an asynchronous API.
-The interfaces are the same, but the asynchronous API requires awaiting of
-certain functions and iterators. Both APIs must be used as context managers. To
-get video information in both APIs:
+(#documentation) * [Disclaimer](#disclaimer) ## Getting Started ###
+Installation Install the ``tiktokapipy`` package (or add it to your project
+requirements) and set up Playwright: ```shell pip install tiktokapipy python -
+m playwright install ``` ### Quick Start Guide TikTokPy has both a synchronous
+and an asynchronous API. The interfaces are the same, but the asynchronous API
+requires awaiting of certain functions and iterators. Both APIs must be used as
+context managers. To get video information in both APIs:
 Synchronous                           Asynchronous
 ```py from tiktokapipy.api import     ```py from tiktokapipy.async_api import
 TikTokAPI with TikTokAPI() as api:    AsyncTikTokAPI async with AsyncTikTokAPI
 video = api.video(video_link) ... ``` () as api: video = await api.video
                                       (video_link) ... ```
 More examples, including how to download videos and slideshows, can be found in
 the [documentation](https://tiktokpy.readthedocs.io/en/latest/users/
-usage.html#examples). ## Documentation You can view the full documentation on
-[Read the Docs](https://tiktokpy.readthedocs.io/en/latest/).
+usage.html#examples). Warnings can be ignored as follows: ```py import warnings
+from tiktokapipy import TikTokAPIWarning warnings.filterwarnings("ignore",
+category=TikTokAPIWarning) ``` ## Documentation You can view the full
+documentation on [Read the Docs](https://tiktokpy.readthedocs.io/en/latest/).
+===============================================================================
+## Disclaimer TikTokPy is in no way affiliated with, authorized, maintained,
+sponsored or endorsed by TikTok or any of its affiliates or subsidiaries. Use
+of automated scripts to collect information from or otherwise interact with
+TikTok and its related services is against [TikTok's Terms of Service](https://
+www.tiktok.com/legal/page/us/terms-of-service/en). Use at your own risk. For
+educational purposes only.
```

### Comparing `tiktokapipy-0.1.9.post1/pyproject.toml` & `tiktokapipy-0.2.0/pyproject.toml`

 * *Files 7% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "tiktokapipy"
-version = "0.1.9.post1"
+version = "0.2.0"
 authors = [
     { name="Russell Newton", email="russell.newton01@gmail.com" },
 ]
 description = "Asyncio TikTok data scraping tool"
 readme = "README.md"
 requires-python = ">=3.8"
 
@@ -40,18 +40,19 @@
 test = [
     "pytest",
     "pytest-cov",
     "pytest-asyncio",
     "tox",
 ]
 docs = [
+    "toml",
     "docutils>=0.18",
-    "sphinx~=5.0",
+    "sphinx<7",
     "sphinx-rtd-theme",
     "sphinx-autodoc-typehints",
-    "autodoc_pydantic",
     "sphinx-tabs",
+    "mock",
 ]
 
 [project.urls]
 "Homepage" = "https://github.com/Russell-Newton/TikTokPy"
 "Documentation" = "https://tiktokpy.readthedocs.io/en/latest/"
```

### Comparing `tiktokapipy-0.1.9.post1/src/tiktokapipy/models/raw_data.py` & `tiktokapipy-0.2.0/src/tiktokapipy/models/raw_data.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 """
 Unprocessed data retrieved directly from TikTok
 :autodoc-skip:
 """
 
-import abc
-from typing import Dict, Generic, List, Optional, TypeVar, Union
+from typing import Any, Dict, List, Optional, TypeVar, Union
 
+from pydantic import AliasPath, Field
 from tiktokapipy.models import CamelCaseModel, TitleCaseModel
 from tiktokapipy.models.challenge import Challenge, ChallengeStats
 from tiktokapipy.models.comment import Comment
 from tiktokapipy.models.user import User, UserStats
 from tiktokapipy.models.video import LightVideo, Video
 
 
@@ -32,134 +32,88 @@
 
     status_code: int
 
 
 class ChallengePage(StatusPage):
     """:autodoc-skip:"""
 
-    challenge_info: Optional[ChallengeInfo]
+    challenge_info: Optional[ChallengeInfo] = None
 
 
-class APIResponse(CamelCaseModel):
+class VideoInfo(CamelCaseModel):
     """:autodoc-skip:"""
 
-    status_code: int = 0
-    cursor: Optional[int]
-    has_more: Union[bool, int]
+    video: Video = Field(alias="itemStruct")
 
-    total: Optional[int]
-    comments: Optional[List[Comment]]
-    item_list: Optional[List[LightVideo]]
 
-
-class PrimaryResponseType(TitleCaseModel):
+class VideoPage(StatusPage):
     """:autodoc-skip:"""
 
-    pass
+    item_info: VideoInfo
 
 
-class ChallengeResponse(PrimaryResponseType):
+class APIResponse(CamelCaseModel):
     """:autodoc-skip:"""
 
-    item_module: Optional[Dict[int, LightVideo]]
-    challenge_page: ChallengePage
-
+    status_code: int = 0
+    cursor: Optional[int] = None
+    has_more: Union[bool, int]
 
-DesktopResponseT = TypeVar("DesktopResponseT")
+    total: Optional[int] = None
+    comments: Optional[List[Comment]] = None
+    item_list: Optional[List[LightVideo]] = None
 
 
-class MobileResponseMixin(abc.ABC, Generic[DesktopResponseT]):
+class PrimaryResponseType(TitleCaseModel):
     """:autodoc-skip:"""
 
-    @abc.abstractmethod
-    def to_desktop(self) -> DesktopResponseT:
-        pass
+    pass
 
 
-class MobileChallengeResponse(
-    PrimaryResponseType, MobileResponseMixin[ChallengeResponse]
-):
+class ChallengeResponse(PrimaryResponseType):
     """:autodoc-skip:"""
 
-    mobile_item_module: Optional[Dict[int, LightVideo]]
-    mobile_challenge_page: ChallengePage
+    item_module: Optional[Dict[int, LightVideo]] = None
+    challenge_page: Optional[ChallengePage] = None
 
-    def to_desktop(self) -> ChallengeResponse:
-        return ChallengeResponse(
-            item_module=self.mobile_item_module,
-            challenge_page=self.mobile_challenge_page,
-        )
+
+DesktopResponseT = TypeVar("DesktopResponseT")
 
 
 class UserResponse(PrimaryResponseType):
     """:autodoc-skip:"""
 
-    item_module: Optional[Dict[int, LightVideo]]
-    user_module: Optional[UserModule]
+    item_module: Optional[Dict[int, LightVideo]] = None
+    user_module: Optional[UserModule] = None
     user_page: StatusPage
 
 
-class MobileUserResponse(PrimaryResponseType, MobileResponseMixin[UserResponse]):
-    """:autodoc-skip:"""
-
-    mobile_item_module: Optional[Dict[int, LightVideo]]
-    mobile_user_page: StatusPage
-    mobile_user_module: Optional[UserModule]
-
-    def to_desktop(self) -> UserResponse:
-        return UserResponse(
-            item_module=self.mobile_item_module,
-            user_page=self.mobile_user_page,
-            user_module=self.mobile_user_module,
-        )
-
-
 class VideoResponse(PrimaryResponseType):
     """:autodoc-skip:"""
 
-    item_module: Optional[Dict[int, Video]]
-    comment_item: Optional[Dict[int, Comment]]
+    item_module: Optional[Dict[int, Video]] = None
+    comment_item: Optional[Dict[int, Comment]] = None
     video_page: StatusPage
 
     # Preprocess to insert id if needed
     @classmethod
-    def parse_obj(cls, obj):
+    def model_validate(
+        cls,
+        obj,
+        *,
+        strict: Optional[bool] = None,
+        from_attributes: Optional[bool] = None,
+        context: Optional[Dict[str, Any]] = None,
+    ):
         if "ItemModule" in obj:
             for key in obj["ItemModule"]:
                 obj["ItemModule"][key]["id"] = key
                 obj["ItemModule"][key]["video"]["id"] = key
-        return super().parse_obj(obj)
-
-
-class MobileVideoData(StatusPage):
-    """:autodoc-skip:"""
-
-    item_info: Optional[Dict[str, Video]]
-
-
-class MobileVideoModule(CamelCaseModel):
-    """:autodoc-skip:"""
-
-    video_data: MobileVideoData
-
-
-class MobileVideoResponse(PrimaryResponseType, MobileResponseMixin[VideoResponse]):
-    """:autodoc-skip:"""
+        return super().model_validate(
+            obj, strict=strict, from_attributes=from_attributes, context=context
+        )
 
-    sharing_video_module: MobileVideoModule
-    mobile_sharing_comment: APIResponse
 
-    def to_desktop(self) -> VideoResponse:
-        return VideoResponse(
-            item_module={
-                i: v
-                for i, v in enumerate(
-                    self.sharing_video_module.video_data.item_info.values()
-                )
-            },
-            comment_item={
-                comment.id: comment for comment in self.mobile_sharing_comment.comments
-            },
-            video_page=StatusPage(
-                status_code=self.sharing_video_module.video_data.status_code
-            ),
-        )
+class SentToLoginResponse(TitleCaseModel):
+    redirect_url: str = Field(
+        validation_alias=AliasPath("LoginContextModule", "redirectUrl")
+    )
```

### Comparing `tiktokapipy-0.1.9.post1/src/tiktokapipy/models/video.py` & `tiktokapipy-0.2.0/src/tiktokapipy/models/video.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,22 +1,33 @@
 """Video data models"""
 
 from __future__ import annotations
 
 from datetime import datetime
-from typing import Awaitable, Callable, List, Optional, Union
+from functools import cached_property
+from typing import Any, ForwardRef, List, Optional, Union
 
-from pydantic import Field
-from tiktokapipy.models import (
-    AsyncDeferredIterator,
-    CamelCaseModel,
-    DeferredIterator,
-    TitleCaseModel,
+from playwright.async_api import BrowserContext as AsyncBrowserContext
+from pydantic import AliasChoices, Field, computed_field
+from tiktokapipy import TikTokAPIError
+from tiktokapipy.models import CamelCaseModel, TitleCaseModel
+from tiktokapipy.util.deferred_collectors import (
+    DeferredChallengeIterator,
+    DeferredCommentIterator,
+    DeferredUserGetterAsync,
+    DeferredUserGetterSync,
 )
 
+LightChallenge = ForwardRef("LightChallenge")
+Challenge = ForwardRef("Challenge")
+Comment = ForwardRef("Comment")
+LightUser = ForwardRef("LightUser")
+User = ForwardRef("User")
+UserStats = ForwardRef("UserStats")
+
 
 class VideoStats(CamelCaseModel):
     digg_count: int
     share_count: int
     comment_count: int
     play_count: int
 
@@ -32,54 +43,54 @@
     # video_subtitle_ID: int
     size: int
 
 
 class VideoData(CamelCaseModel):
     """Contains data about a downloadable video"""
 
-    id: int
+    # id: int
     height: int
     width: int
     duration: int
     ratio: str
-    format: Optional[str]
-    bitrate: Optional[int]
+    format: Optional[str] = None
+    bitrate: Optional[int] = None
     # encoded_type: str
     # video_quality: str
     # encode_user_tag: str
     # codec_type: str
     # definition: str
     # subtitle_infos: Optional[List[SubtitleData]]
 
     ################
     # Video stills #
     ################
     cover: str
     origin_cover: str
     dynamic_cover: str
-    share_cover: List[str]
-    reflow_cover: str
+    share_cover: Optional[List[str]] = None
+    reflow_cover: Optional[str] = None
 
     ###############
     # Video links #
     ###############
     play_addr: str
     download_addr: str
 
 
 class MusicData(CamelCaseModel):
     """Contains data about the music within a video"""
 
     id: int
     title: str
     play_url: str
-    author_name: str
+    author_name: Optional[str] = None
     duration: int
     original: bool
-    album: Optional[str]
+    album: Optional[str] = None
 
     cover_large: str
     cover_medium: str
     cover_thumb: str
 
     # schedule_search_time: int
 
@@ -108,43 +119,43 @@
     """Still image on the video before playing"""
     share_cover: ImageData
     """Still image embedded with a sharing link"""
     title: str
 
 
 class LightVideo(CamelCaseModel):
-    """:autodoc-skip:"""
+    """Bare minimum information for scraping"""
 
-    id: int
+    id: int = Field(validation_alias=AliasChoices("cid", "uid", "id"))
     """The unique video ID"""
     # Have this here to sort the iteration.
     stats: VideoStats
     """Stats about the video"""
     create_time: datetime
 
 
 class Video(LightVideo):
     #####################
     # Content and stats #
     #####################
     desc: str
     """Video description"""
-    diversification_labels: Optional[List[str]]
+    diversification_labels: Optional[List[str]] = None
     """Tags/Categories applied to the video"""
-    challenges: Optional[List[LightChallenge]]
+    challenges: Optional[List[LightChallenge]] = None
     """
     We don't want to grab anything more than the title so we can generate the lazy challenge getter.
     :autodoc-skip:
     """
     video: VideoData
     music: MusicData
     # digged: bool
     # item_comment_status: int
     # location_created: Optional[str]
-    image_post: Optional[ImagePost]
+    image_post: Optional[ImagePost] = None
     """The images in the video if the video is a slideshow"""
 
     ######################
     # Author information #
     ######################
     author: Union[LightUser, str]
     """
@@ -190,30 +201,70 @@
     # item_mute: bool
     # text_extra: Optional[list]
     # effect_stickers: Optional[list]
     # stickers_on_item: Optional[list]
     # for_friend: bool
     # vl1: bool
 
-    comments: Optional[List[Comment]]
-    """Set on return from API. Contains all :class:`.Comment`s gathered during scraping."""
-    creator: Optional[Callable[[], Union[User, Awaitable[User]]]]
-    """Set on return from API. Call to retrieve data on the :class:`.User` that created the video."""
-    tags: Optional[
-        Union[
-            DeferredIterator[LightChallenge, Challenge],
-            AsyncDeferredIterator[LightChallenge, Challenge],
-        ]
-    ]
-    """Set on return from API. Iterate over to retrieve data on the :class:`.Challenge`s applied to the video."""
+    @computed_field(repr=False)
+    @property
+    def _api(self) -> Any:
+        if not hasattr(self, "_api_internal"):
+            self._api_internal = None
+        return self._api_internal
+
+    @_api.setter
+    def _api(self, api):
+        self._api_internal = api
+
+    @computed_field(repr=False)
+    @cached_property
+    def comments(self) -> DeferredCommentIterator:
+        if self._api is None:
+            raise TikTokAPIError(
+                "A TikTokAPI must be attached to video._api before collecting comments"
+            )
+        return DeferredCommentIterator(self._api, self.id)
+
+    @computed_field(repr=False)
+    @cached_property
+    def tags(self) -> DeferredChallengeIterator:
+        if self._api is None:
+            raise TikTokAPIError(
+                "A TikTokAPI must be attached to video._api before collecting comments"
+            )
+        return DeferredChallengeIterator(
+            self._api,
+            [challenge.title for challenge in self.challenges]
+            if self.challenges
+            else [],
+        )
+
+    @computed_field(repr=False)
+    @cached_property
+    def creator(self) -> Union[DeferredUserGetterAsync, DeferredUserGetterSync]:
+        if self._api is None:
+            raise TikTokAPIError(
+                "A TikTokAPI must be attached to video._api before retrieving creator data"
+            )
+        unique_id = (
+            self.author if isinstance(self.author, str) else self.author.unique_id
+        )
+        if isinstance(self._api.context, AsyncBrowserContext):
+            return DeferredUserGetterAsync(self._api, unique_id)
+        else:
+            return DeferredUserGetterSync(self._api, unique_id)
+
+
+del Challenge, LightChallenge, Comment, LightUser, User, UserStats
 
 
 from tiktokapipy.models.challenge import Challenge, LightChallenge  # noqa E402
 from tiktokapipy.models.comment import Comment  # noqa E402
 from tiktokapipy.models.user import LightUser, User, UserStats  # noqa E402
 
-Video.update_forward_refs()
+Video.model_rebuild()
 
 
 def video_link(video_id: int) -> str:
     """Get a working link to a TikTok video from the video's unique id."""
     return f"https://m.tiktok.com/v/{video_id}"
```

### Comparing `tiktokapipy-0.1.9.post1/src/tiktokapipy.egg-info/PKG-INFO` & `tiktokapipy-0.2.0/src/tiktokapipy.egg-info/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tiktokapipy
-Version: 0.1.9.post1
+Version: 0.2.0
 Summary: Asyncio TikTok data scraping tool
 Author-email: Russell Newton <russell.newton01@gmail.com>
 Project-URL: Homepage, https://github.com/Russell-Newton/TikTokPy
 Project-URL: Documentation, https://tiktokpy.readthedocs.io/en/latest/
 Keywords: tiktok,python3,scraper,unofficial,tiktok-scraper,tiktok scraper,asyncio,playwright-python
 Classifier: Development Status :: 3 - Alpha
 Classifier: Framework :: AsyncIO
@@ -50,14 +50,15 @@
 
 ## Table of Contents
 
 * [Getting Started](#getting-started)
     * [Installation](#installation)
     * [Quick Start Guide](#quick-start-guide)
 * [Documentation](#documentation)
+* [Disclaimer](#disclaimer)
 
 ## Getting Started
 
 ### Installation
 
 Install the ``tiktokapipy`` package (or add it to your project requirements) and set up Playwright:
 
@@ -103,10 +104,26 @@
 </td>
 </tr>
 </table>
 
 More examples, including how to download videos and slideshows, can be found in the
 [documentation](https://tiktokpy.readthedocs.io/en/latest/users/usage.html#examples).
 
+Warnings can be ignored as follows:
+
+```py
+import warnings
+
+from tiktokapipy import TikTokAPIWarning
+
+warnings.filterwarnings("ignore", category=TikTokAPIWarning)
+```
+
 ## Documentation
 
 You can view the full documentation on [Read the Docs](https://tiktokpy.readthedocs.io/en/latest/).
+
+<hr>
+
+## Disclaimer
+
+TikTokPy is in no way affiliated with, authorized, maintained, sponsored or endorsed by TikTok or any of its affiliates or subsidiaries. Use of automated scripts to collect information from or otherwise interact with TikTok and its related services is against [TikTok's Terms of Service](https://www.tiktok.com/legal/page/us/terms-of-service/en). Use at your own risk. For educational purposes only.
```

#### html2text {}

```diff
@@ -1,9 +1,9 @@
-Metadata-Version: 2.1 Name: tiktokapipy Version: 0.1.9.post1 Summary: Asyncio
-TikTok data scraping tool Author-email: Russell Newton
+Metadata-Version: 2.1 Name: tiktokapipy Version: 0.2.0 Summary: Asyncio TikTok
+data scraping tool Author-email: Russell Newton
 newton01@gmail.com> Project-URL: Homepage, https://github.com/Russell-Newton/
 TikTokPy Project-URL: Documentation, https://tiktokpy.readthedocs.io/en/latest/
 Keywords: tiktok,python3,scraper,unofficial,tiktok-scraper,tiktok
 scraper,asyncio,playwright-python Classifier: Development Status :: 3 - Alpha
 Classifier: Framework :: AsyncIO Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Information Technology Classifier: Intended
 Audience :: Science/Research Classifier: License :: OSI Approved :: MIT License
@@ -16,23 +16,32 @@
 text/markdown Provides-Extra: test Provides-Extra: docs License-File: LICENSE
                             ****** TikTokPy ******
                     [PyPI] [Python_Version_3.8+] [License]
                   [Unit_Tests_Status] [Documentation_Status]
 **Extract data from TikTok without needing any login information or API keys.**
 ## Table of Contents * [Getting Started](#getting-started) * [Installation]
 (#installation) * [Quick Start Guide](#quick-start-guide) * [Documentation]
-(#documentation) ## Getting Started ### Installation Install the
-``tiktokapipy`` package (or add it to your project requirements) and set up
-Playwright: ```shell pip install tiktokapipy python -m playwright install ```
-### Quick Start Guide TikTokPy has both a synchronous and an asynchronous API.
-The interfaces are the same, but the asynchronous API requires awaiting of
-certain functions and iterators. Both APIs must be used as context managers. To
-get video information in both APIs:
+(#documentation) * [Disclaimer](#disclaimer) ## Getting Started ###
+Installation Install the ``tiktokapipy`` package (or add it to your project
+requirements) and set up Playwright: ```shell pip install tiktokapipy python -
+m playwright install ``` ### Quick Start Guide TikTokPy has both a synchronous
+and an asynchronous API. The interfaces are the same, but the asynchronous API
+requires awaiting of certain functions and iterators. Both APIs must be used as
+context managers. To get video information in both APIs:
 Synchronous                           Asynchronous
 ```py from tiktokapipy.api import     ```py from tiktokapipy.async_api import
 TikTokAPI with TikTokAPI() as api:    AsyncTikTokAPI async with AsyncTikTokAPI
 video = api.video(video_link) ... ``` () as api: video = await api.video
                                       (video_link) ... ```
 More examples, including how to download videos and slideshows, can be found in
 the [documentation](https://tiktokpy.readthedocs.io/en/latest/users/
-usage.html#examples). ## Documentation You can view the full documentation on
-[Read the Docs](https://tiktokpy.readthedocs.io/en/latest/).
+usage.html#examples). Warnings can be ignored as follows: ```py import warnings
+from tiktokapipy import TikTokAPIWarning warnings.filterwarnings("ignore",
+category=TikTokAPIWarning) ``` ## Documentation You can view the full
+documentation on [Read the Docs](https://tiktokpy.readthedocs.io/en/latest/).
+===============================================================================
+## Disclaimer TikTokPy is in no way affiliated with, authorized, maintained,
+sponsored or endorsed by TikTok or any of its affiliates or subsidiaries. Use
+of automated scripts to collect information from or otherwise interact with
+TikTok and its related services is against [TikTok's Terms of Service](https://
+www.tiktok.com/legal/page/us/terms-of-service/en). Use at your own risk. For
+educational purposes only.
```

