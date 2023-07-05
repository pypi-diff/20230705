# Comparing `tmp/wibuapi-0.1.2.tar.gz` & `tmp/wibuapi-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "wibuapi-0.1.2.tar", last modified: Sat Apr 15 20:18:31 2023, max compression
+gzip compressed data, was "wibuapi-0.1.3.tar", last modified: Wed Jul  5 03:17:10 2023, max compression
```

## Comparing `wibuapi-0.1.2.tar` & `wibuapi-0.1.3.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 20:18:31.534878 wibuapi-0.1.2/
--rw-r--r--   0 runner    (1001) docker     (123)    35145 2023-04-15 20:18:18.000000 wibuapi-0.1.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     9476 2023-04-15 20:18:31.534878 wibuapi-0.1.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     8810 2023-04-15 20:18:18.000000 wibuapi-0.1.2/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       85 2023-04-15 20:18:18.000000 wibuapi-0.1.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-15 20:18:31.534878 wibuapi-0.1.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      923 2023-04-15 20:18:18.000000 wibuapi-0.1.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 20:18:31.530878 wibuapi-0.1.2/wibuapi/
--rw-r--r--   0 runner    (1001) docker     (123)      118 2023-04-15 20:18:18.000000 wibuapi-0.1.2/wibuapi/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    16424 2023-04-15 20:18:18.000000 wibuapi-0.1.2/wibuapi/wibuapi.py
--rw-r--r--   0 runner    (1001) docker     (123)     1142 2023-04-15 20:18:18.000000 wibuapi-0.1.2/wibuapi/zyxdevs.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 20:18:31.534878 wibuapi-0.1.2/wibuapi.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     9476 2023-04-15 20:18:31.000000 wibuapi-0.1.2/wibuapi.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      253 2023-04-15 20:18:31.000000 wibuapi-0.1.2/wibuapi.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-15 20:18:31.000000 wibuapi-0.1.2/wibuapi.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-04-15 20:18:31.000000 wibuapi-0.1.2/wibuapi.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-04-15 20:18:31.000000 wibuapi-0.1.2/wibuapi.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 03:17:10.223983 wibuapi-0.1.3/
+-rw-r--r--   0 runner    (1001) docker     (123)    35145 2023-07-05 03:16:56.000000 wibuapi-0.1.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    10500 2023-07-05 03:17:10.223983 wibuapi-0.1.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     9228 2023-07-05 03:16:56.000000 wibuapi-0.1.3/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       85 2023-07-05 03:16:56.000000 wibuapi-0.1.3/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-05 03:17:10.223983 wibuapi-0.1.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1763 2023-07-05 03:16:56.000000 wibuapi-0.1.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 03:17:10.223983 wibuapi-0.1.3/wibuapi/
+-rw-r--r--   0 runner    (1001) docker     (123)      118 2023-07-05 03:16:56.000000 wibuapi-0.1.3/wibuapi/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16915 2023-07-05 03:16:56.000000 wibuapi-0.1.3/wibuapi/wibuapi.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1142 2023-07-05 03:16:56.000000 wibuapi-0.1.3/wibuapi/zyxdevs.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 03:17:10.223983 wibuapi-0.1.3/wibuapi.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    10500 2023-07-05 03:17:10.000000 wibuapi-0.1.3/wibuapi.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      253 2023-07-05 03:17:10.000000 wibuapi-0.1.3/wibuapi.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-05 03:17:10.000000 wibuapi-0.1.3/wibuapi.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-07-05 03:17:10.000000 wibuapi-0.1.3/wibuapi.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-07-05 03:17:10.000000 wibuapi-0.1.3/wibuapi.egg-info/top_level.txt
```

### Comparing `wibuapi-0.1.2/LICENSE` & `wibuapi-0.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `wibuapi-0.1.2/PKG-INFO` & `wibuapi-0.1.3/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,21 +1,31 @@
 Metadata-Version: 2.1
 Name: wibuapi
-Version: 0.1.2
+Version: 0.1.3
 Summary: Official Python Wrapper for Wibu API.
 Home-page: https://github.com/zYxDevs/wibu-api-py
 Author: Yoga Pranata
 Author-email: yoga@zyxdevs.eu.org
-License: License :: OSI Approved :: GNU Lesser General Public License v3 (LGPLv3)
+License: GNU Lesser General Public License v3 (LGPLv3)
+Keywords: wibu,weebs,otaku,anime,hentai,donghua,manga,doujin,manhwa,manhua,jdrama,jav,music,booru,api,nsfw,scraper,bypasser,genshin,facebook,youtube
+Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: Operating System :: OS Independent
+Classifier: Development Status :: 5 - Production/Stable
+Classifier: Natural Language :: English
+Classifier: Topic :: Internet
+Classifier: Topic :: Software Development :: Libraries
+Classifier: Topic :: Software Development :: Libraries :: Python Modules
+Classifier: License :: OSI Approved :: GNU Lesser General Public License v3 (LGPLv3)
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # Wibu-API-Py
 [![Downloads](https://static.pepy.tech/personalized-badge/wibuapi?units=none&left_color=gray&right_color=blue&left_text=downloads)](https://pepy.tech/project/wibuapi)  [![Repo Size](https://img.shields.io/github/repo-size/zYxDevs/wibu-api-py?style=flat-square)](https://github.com/zYxDevs/wibu-api-py)  [![Languages](https://img.shields.io/github/languages/top/zYxDevs/wibu-api-py?style=flat-square)](https://github.com/zYxDevs/wibu-api-py)  [![CodeFactor](https://www.codefactor.io/repository/github/zYxDevs/wibu-api-py/badge)](https://www.codefactor.io/repository/github/zYxDevs/wibu-api-py)  [![Codacy Badge](https://app.codacy.com/project/badge/Grade/8b87ea2387574f54849805430a9bc9ea)](https://www.codacy.com/gh/zYxDevs/wibu-api-py/dashboard?utm_source=github.com&amp;utm_medium=referral&amp;utm_content=zYxDevs/wibu-api-py&amp;utm_campaign=Badge_Grade)
 
@@ -54,20 +64,24 @@
 - [x] Worldmanhwas zipper
 - [x] Maid Manga zipper
 - [x] Mangayaro zipper
 - [x] Cosmicscans zipper
 - [x] nHentai zipper
 - [x] Sheakomik, Sheamanga zipper
 - [x] Komikindo.info zipper
+- [x] Mikoroku zipper
+- [x] Onlylama
+  - [x] Download link sraper
+  - [x] Photo album zipper
 - [x] Otomi Games
   - [x] Search parser
-  - [x] Download link scrapper
+  - [x] Download link scraper
 - [x] Javhd
   - [x] Search parser
-  - [x] Download link scrapper
+  - [x] Download link scraper
 - [x] Other incoming features
 
 [![WibuAPI Bot](https://img.shields.io/badge/WibuAPI-Bot-blue?&logo=telegram)](https://wibuapibot.t.me)
 [![Yoga Pranata](https://img.shields.io/badge/Yoga-Pranata-blue?&logo=telegram)](https://t.me/Yoga_CIC)
 [![Supoort Chat](https://img.shields.io/badge/Support-Chat-blue?&logo=telegram)](https://ybotssupport.t.me)
 [![Update Channel](https://img.shields.io/badge/Update-Channel-blue?&logo=telegram)](https://spreadnetworks.t.me)
 
@@ -85,14 +99,15 @@
 | :-: | :-: |
 | [Lendrive](https://github.com/zYxDevs/wibu-api-py#lendrive)| link |
 | [Anichin](https://github.com/zYxDevs/wibu-api-py#anichin) | link |
 | [Donghua](https://github.com/zYxDevs/wibu-api-py#donghua) | link |
 | [Kusonime](https://github.com/zYxDevs/wibu-api-py#kusonime) | link |
 | [Doronime](https://github.com/zYxDevs/wibu-api-py#doronime) | link |
 | [Samehadaku](https://github.com/zYxDevs/wibu-api-py#samehadaku) | link |
+| [Kuramanime](https://github.com/zYxDevs/wibu-api-py#kuramanime) | link |
 | [Nekopoi](https://github.com/zYxDevs/wibu-api-py#nekopoi) | link |
 
 #### [Lendrive](https://lendrive.web.id)
 ```python
 # works with batch, bd, and single eps link
 url = "https://lendrive.web.id/tondemo-skill-de-isekai-hourou-meshi-ep-04-dual-subs-x265-hevc-subtitle-indonesia-english/"
 res = api.lendrive(url)
@@ -135,14 +150,22 @@
 ```python
 # works with batch, bd, and single eps link
 url = "https://samehadaku.run/nierautomata-ver1-1a-episode-8/"
 res = api.samehadaku(url)
 print(res)
 ```
 
+#### [Kuramanime](https://kuramalink.my.id)
+```python
+# works with batch, bd, and single eps link
+url = "https://kuramanime.art/anime/2004/mushoku-tensei-isekai-ittara-honki-dasu-shugo-jutsushi-fitz/episode/1"
+res = api.kuramanime(url)
+print(res)
+```
+
 #### [Nekopoi](https://nekopoi.care)
 ```python
 # works with single eps link (hentai, jav)
 url = "https://nekopoi.care/koumi-jima-shuu-7-de-umeru-mesu-tachi-episode-1-subtitle-indonesia/"
 res = api.nekopoi(url)
 print(res)
 ```
```

### Comparing `wibuapi-0.1.2/README.md` & `wibuapi-0.1.3/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -36,20 +36,24 @@
 - [x] Worldmanhwas zipper
 - [x] Maid Manga zipper
 - [x] Mangayaro zipper
 - [x] Cosmicscans zipper
 - [x] nHentai zipper
 - [x] Sheakomik, Sheamanga zipper
 - [x] Komikindo.info zipper
+- [x] Mikoroku zipper
+- [x] Onlylama
+  - [x] Download link sraper
+  - [x] Photo album zipper
 - [x] Otomi Games
   - [x] Search parser
-  - [x] Download link scrapper
+  - [x] Download link scraper
 - [x] Javhd
   - [x] Search parser
-  - [x] Download link scrapper
+  - [x] Download link scraper
 - [x] Other incoming features
 
 [![WibuAPI Bot](https://img.shields.io/badge/WibuAPI-Bot-blue?&logo=telegram)](https://wibuapibot.t.me)
 [![Yoga Pranata](https://img.shields.io/badge/Yoga-Pranata-blue?&logo=telegram)](https://t.me/Yoga_CIC)
 [![Supoort Chat](https://img.shields.io/badge/Support-Chat-blue?&logo=telegram)](https://ybotssupport.t.me)
 [![Update Channel](https://img.shields.io/badge/Update-Channel-blue?&logo=telegram)](https://spreadnetworks.t.me)
 
@@ -67,14 +71,15 @@
 | :-: | :-: |
 | [Lendrive](https://github.com/zYxDevs/wibu-api-py#lendrive)| link |
 | [Anichin](https://github.com/zYxDevs/wibu-api-py#anichin) | link |
 | [Donghua](https://github.com/zYxDevs/wibu-api-py#donghua) | link |
 | [Kusonime](https://github.com/zYxDevs/wibu-api-py#kusonime) | link |
 | [Doronime](https://github.com/zYxDevs/wibu-api-py#doronime) | link |
 | [Samehadaku](https://github.com/zYxDevs/wibu-api-py#samehadaku) | link |
+| [Kuramanime](https://github.com/zYxDevs/wibu-api-py#kuramanime) | link |
 | [Nekopoi](https://github.com/zYxDevs/wibu-api-py#nekopoi) | link |
 
 #### [Lendrive](https://lendrive.web.id)
 ```python
 # works with batch, bd, and single eps link
 url = "https://lendrive.web.id/tondemo-skill-de-isekai-hourou-meshi-ep-04-dual-subs-x265-hevc-subtitle-indonesia-english/"
 res = api.lendrive(url)
@@ -117,14 +122,22 @@
 ```python
 # works with batch, bd, and single eps link
 url = "https://samehadaku.run/nierautomata-ver1-1a-episode-8/"
 res = api.samehadaku(url)
 print(res)
 ```
 
+#### [Kuramanime](https://kuramalink.my.id)
+```python
+# works with batch, bd, and single eps link
+url = "https://kuramanime.art/anime/2004/mushoku-tensei-isekai-ittara-honki-dasu-shugo-jutsushi-fitz/episode/1"
+res = api.kuramanime(url)
+print(res)
+```
+
 #### [Nekopoi](https://nekopoi.care)
 ```python
 # works with single eps link (hentai, jav)
 url = "https://nekopoi.care/koumi-jima-shuu-7-de-umeru-mesu-tachi-episode-1-subtitle-indonesia/"
 res = api.nekopoi(url)
 print(res)
 ```
```

### Comparing `wibuapi-0.1.2/wibuapi/wibuapi.py` & `wibuapi-0.1.3/wibuapi/wibuapi.py`

 * *Files 1% similar despite different names*

```diff
@@ -83,14 +83,25 @@
         try:
             url = f"{self.base_url}/anime/samehadaku?link={link}"
             response = get(url, timeout=15).json()
             return dumps(response, indent=2)
         except Exception as e:
             return f"An error occured report on @YBotsSupport\n\n{e}"
 
+    def kuramanime(self, link: str):
+        """works with batch, bd, and single eps link
+        https://kuramanime.art/anime/2004/mushoku-tensei-isekai-ittara-honki-dasu-shugo-jutsushi-fitz/episode/1
+        """
+        try:
+            url = f"{self.base_url}/anime/kuramanime?link={link}"
+            response = get(url, timeout=15).json()
+            return dumps(response, indent=2)
+        except Exception as e:
+            return f"An error occured report on @YBotsSupport\n\n{e}"
+
     def rawkuma(self, link: str):
         """works with list and single chapter
         list: https://rawkuma.com/manga/guilty-circle/
         single: https://rawkuma.com/guilty-circle-chapter-83/
         """
         try:
             url = f"{self.base_url}/manga/rawkuma?link={link}"
```

### Comparing `wibuapi-0.1.2/wibuapi/zyxdevs.py` & `wibuapi-0.1.3/wibuapi/zyxdevs.py`

 * *Files identical despite different names*

### Comparing `wibuapi-0.1.2/wibuapi.egg-info/PKG-INFO` & `wibuapi-0.1.3/wibuapi.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,21 +1,31 @@
 Metadata-Version: 2.1
 Name: wibuapi
-Version: 0.1.2
+Version: 0.1.3
 Summary: Official Python Wrapper for Wibu API.
 Home-page: https://github.com/zYxDevs/wibu-api-py
 Author: Yoga Pranata
 Author-email: yoga@zyxdevs.eu.org
-License: License :: OSI Approved :: GNU Lesser General Public License v3 (LGPLv3)
+License: GNU Lesser General Public License v3 (LGPLv3)
+Keywords: wibu,weebs,otaku,anime,hentai,donghua,manga,doujin,manhwa,manhua,jdrama,jav,music,booru,api,nsfw,scraper,bypasser,genshin,facebook,youtube
+Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: Operating System :: OS Independent
+Classifier: Development Status :: 5 - Production/Stable
+Classifier: Natural Language :: English
+Classifier: Topic :: Internet
+Classifier: Topic :: Software Development :: Libraries
+Classifier: Topic :: Software Development :: Libraries :: Python Modules
+Classifier: License :: OSI Approved :: GNU Lesser General Public License v3 (LGPLv3)
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # Wibu-API-Py
 [![Downloads](https://static.pepy.tech/personalized-badge/wibuapi?units=none&left_color=gray&right_color=blue&left_text=downloads)](https://pepy.tech/project/wibuapi)  [![Repo Size](https://img.shields.io/github/repo-size/zYxDevs/wibu-api-py?style=flat-square)](https://github.com/zYxDevs/wibu-api-py)  [![Languages](https://img.shields.io/github/languages/top/zYxDevs/wibu-api-py?style=flat-square)](https://github.com/zYxDevs/wibu-api-py)  [![CodeFactor](https://www.codefactor.io/repository/github/zYxDevs/wibu-api-py/badge)](https://www.codefactor.io/repository/github/zYxDevs/wibu-api-py)  [![Codacy Badge](https://app.codacy.com/project/badge/Grade/8b87ea2387574f54849805430a9bc9ea)](https://www.codacy.com/gh/zYxDevs/wibu-api-py/dashboard?utm_source=github.com&amp;utm_medium=referral&amp;utm_content=zYxDevs/wibu-api-py&amp;utm_campaign=Badge_Grade)
 
@@ -54,20 +64,24 @@
 - [x] Worldmanhwas zipper
 - [x] Maid Manga zipper
 - [x] Mangayaro zipper
 - [x] Cosmicscans zipper
 - [x] nHentai zipper
 - [x] Sheakomik, Sheamanga zipper
 - [x] Komikindo.info zipper
+- [x] Mikoroku zipper
+- [x] Onlylama
+  - [x] Download link sraper
+  - [x] Photo album zipper
 - [x] Otomi Games
   - [x] Search parser
-  - [x] Download link scrapper
+  - [x] Download link scraper
 - [x] Javhd
   - [x] Search parser
-  - [x] Download link scrapper
+  - [x] Download link scraper
 - [x] Other incoming features
 
 [![WibuAPI Bot](https://img.shields.io/badge/WibuAPI-Bot-blue?&logo=telegram)](https://wibuapibot.t.me)
 [![Yoga Pranata](https://img.shields.io/badge/Yoga-Pranata-blue?&logo=telegram)](https://t.me/Yoga_CIC)
 [![Supoort Chat](https://img.shields.io/badge/Support-Chat-blue?&logo=telegram)](https://ybotssupport.t.me)
 [![Update Channel](https://img.shields.io/badge/Update-Channel-blue?&logo=telegram)](https://spreadnetworks.t.me)
 
@@ -85,14 +99,15 @@
 | :-: | :-: |
 | [Lendrive](https://github.com/zYxDevs/wibu-api-py#lendrive)| link |
 | [Anichin](https://github.com/zYxDevs/wibu-api-py#anichin) | link |
 | [Donghua](https://github.com/zYxDevs/wibu-api-py#donghua) | link |
 | [Kusonime](https://github.com/zYxDevs/wibu-api-py#kusonime) | link |
 | [Doronime](https://github.com/zYxDevs/wibu-api-py#doronime) | link |
 | [Samehadaku](https://github.com/zYxDevs/wibu-api-py#samehadaku) | link |
+| [Kuramanime](https://github.com/zYxDevs/wibu-api-py#kuramanime) | link |
 | [Nekopoi](https://github.com/zYxDevs/wibu-api-py#nekopoi) | link |
 
 #### [Lendrive](https://lendrive.web.id)
 ```python
 # works with batch, bd, and single eps link
 url = "https://lendrive.web.id/tondemo-skill-de-isekai-hourou-meshi-ep-04-dual-subs-x265-hevc-subtitle-indonesia-english/"
 res = api.lendrive(url)
@@ -135,14 +150,22 @@
 ```python
 # works with batch, bd, and single eps link
 url = "https://samehadaku.run/nierautomata-ver1-1a-episode-8/"
 res = api.samehadaku(url)
 print(res)
 ```
 
+#### [Kuramanime](https://kuramalink.my.id)
+```python
+# works with batch, bd, and single eps link
+url = "https://kuramanime.art/anime/2004/mushoku-tensei-isekai-ittara-honki-dasu-shugo-jutsushi-fitz/episode/1"
+res = api.kuramanime(url)
+print(res)
+```
+
 #### [Nekopoi](https://nekopoi.care)
 ```python
 # works with single eps link (hentai, jav)
 url = "https://nekopoi.care/koumi-jima-shuu-7-de-umeru-mesu-tachi-episode-1-subtitle-indonesia/"
 res = api.nekopoi(url)
 print(res)
 ```
```

