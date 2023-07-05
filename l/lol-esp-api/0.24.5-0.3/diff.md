# Comparing `tmp/lol-esp-api-0.24.5.tar.gz` & `tmp/lol-esp-api-0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lol-esp-api-0.24.5.tar", last modified: Sun Jun 25 18:29:38 2023, max compression
+gzip compressed data, was "lol-esp-api-0.3.tar", last modified: Wed Jul  5 05:18:24 2023, max compression
```

## Comparing `lol-esp-api-0.24.5.tar` & `lol-esp-api-0.3.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxr-xr-x   0 madking   (1000) madking   (1000)        0 2023-06-25 18:29:38.337074 lol-esp-api-0.24.5/
--rw-r--r--   0 madking   (1000) madking   (1000)     1071 2023-06-24 19:35:54.000000 lol-esp-api-0.24.5/LICENSE
--rw-r--r--   0 madking   (1000) madking   (1000)      252 2023-06-25 18:29:38.337074 lol-esp-api-0.24.5/PKG-INFO
--rw-r--r--   0 madking   (1000) madking   (1000)      103 2023-06-25 18:29:38.337074 lol-esp-api-0.24.5/setup.cfg
--rw-r--r--   0 madking   (1000) madking   (1000)      419 2023-06-25 18:29:15.000000 lol-esp-api-0.24.5/setup.py
-drwxr-xr-x   0 madking   (1000) madking   (1000)        0 2023-06-25 18:29:38.337074 lol-esp-api-0.24.5/src/
-drwxr-xr-x   0 madking   (1000) madking   (1000)        0 2023-06-25 18:29:38.337074 lol-esp-api-0.24.5/src/lol_esp_api/
--rw-r--r--   0 madking   (1000) madking   (1000)        0 2023-06-24 22:45:14.000000 lol-esp-api-0.24.5/src/lol_esp_api/__init__.py
-drwxr-xr-x   0 madking   (1000) madking   (1000)        0 2023-06-25 18:29:38.337074 lol-esp-api-0.24.5/src/lol_esp_api/apis/
--rw-r--r--   0 madking   (1000) madking   (1000)        0 2023-06-25 17:51:54.000000 lol-esp-api-0.24.5/src/lol_esp_api/apis/__init__.py
--rw-r--r--   0 madking   (1000) madking   (1000)      938 2023-06-25 18:20:39.000000 lol-esp-api-0.24.5/src/lol_esp_api/apis/eventsAPI.py
--rw-r--r--   0 madking   (1000) madking   (1000)     2072 2023-06-25 18:20:42.000000 lol-esp-api-0.24.5/src/lol_esp_api/apis/leaguesAPI.py
--rw-r--r--   0 madking   (1000) madking   (1000)      537 2023-06-25 18:20:44.000000 lol-esp-api-0.24.5/src/lol_esp_api/apis/matchAPI.py
--rw-r--r--   0 madking   (1000) madking   (1000)      265 2023-06-24 18:26:47.000000 lol-esp-api-0.24.5/src/lol_esp_api/apis/supfunc.py
--rw-r--r--   0 madking   (1000) madking   (1000)     1136 2023-06-25 18:20:48.000000 lol-esp-api-0.24.5/src/lol_esp_api/apis/teamsAPI.py
--rw-r--r--   0 madking   (1000) madking   (1000)      233 2023-06-25 18:19:43.000000 lol-esp-api-0.24.5/src/lol_esp_api/lol_esports_api.py
-drwxr-xr-x   0 madking   (1000) madking   (1000)        0 2023-06-25 18:29:38.337074 lol-esp-api-0.24.5/src/lol_esp_api.egg-info/
--rw-r--r--   0 madking   (1000) madking   (1000)      252 2023-06-25 18:29:38.000000 lol-esp-api-0.24.5/src/lol_esp_api.egg-info/PKG-INFO
--rw-r--r--   0 madking   (1000) madking   (1000)      483 2023-06-25 18:29:38.000000 lol-esp-api-0.24.5/src/lol_esp_api.egg-info/SOURCES.txt
--rw-r--r--   0 madking   (1000) madking   (1000)        1 2023-06-25 18:29:38.000000 lol-esp-api-0.24.5/src/lol_esp_api.egg-info/dependency_links.txt
--rw-r--r--   0 madking   (1000) madking   (1000)        9 2023-06-25 18:29:38.000000 lol-esp-api-0.24.5/src/lol_esp_api.egg-info/requires.txt
--rw-r--r--   0 madking   (1000) madking   (1000)       12 2023-06-25 18:29:38.000000 lol-esp-api-0.24.5/src/lol_esp_api.egg-info/top_level.txt
+drwxr-xr-x   0 madking   (1000) madking   (1000)        0 2023-07-05 05:18:24.249156 lol-esp-api-0.3/
+-rw-r--r--   0 madking   (1000) madking   (1000)     1071 2023-06-24 19:35:54.000000 lol-esp-api-0.3/LICENSE
+-rw-r--r--   0 madking   (1000) madking   (1000)      249 2023-07-05 05:18:24.249156 lol-esp-api-0.3/PKG-INFO
+-rw-r--r--   0 madking   (1000) madking   (1000)      103 2023-07-05 05:18:24.249156 lol-esp-api-0.3/setup.cfg
+-rw-r--r--   0 madking   (1000) madking   (1000)      416 2023-07-05 05:17:00.000000 lol-esp-api-0.3/setup.py
+drwxr-xr-x   0 madking   (1000) madking   (1000)        0 2023-07-05 05:18:24.239156 lol-esp-api-0.3/src/
+drwxr-xr-x   0 madking   (1000) madking   (1000)        0 2023-07-05 05:18:24.239156 lol-esp-api-0.3/src/lol_esp_api/
+-rw-r--r--   0 madking   (1000) madking   (1000)        0 2023-06-24 22:45:14.000000 lol-esp-api-0.3/src/lol_esp_api/__init__.py
+drwxr-xr-x   0 madking   (1000) madking   (1000)        0 2023-07-05 05:18:24.249156 lol-esp-api-0.3/src/lol_esp_api/apis/
+-rw-r--r--   0 madking   (1000) madking   (1000)        0 2023-06-25 17:51:54.000000 lol-esp-api-0.3/src/lol_esp_api/apis/__init__.py
+-rw-r--r--   0 madking   (1000) madking   (1000)      935 2023-07-05 04:58:24.000000 lol-esp-api-0.3/src/lol_esp_api/apis/eventsAPI.py
+-rw-r--r--   0 madking   (1000) madking   (1000)     2072 2023-07-02 20:09:11.000000 lol-esp-api-0.3/src/lol_esp_api/apis/leaguesAPI.py
+-rw-r--r--   0 madking   (1000) madking   (1000)      478 2023-07-05 05:05:28.000000 lol-esp-api-0.3/src/lol_esp_api/apis/matchAPI.py
+-rw-r--r--   0 madking   (1000) madking   (1000)      265 2023-07-05 04:53:58.000000 lol-esp-api-0.3/src/lol_esp_api/apis/supfunc.py
+-rw-r--r--   0 madking   (1000) madking   (1000)     1136 2023-06-25 18:20:48.000000 lol-esp-api-0.3/src/lol_esp_api/apis/teamsAPI.py
+-rw-r--r--   0 madking   (1000) madking   (1000)      233 2023-06-25 18:19:43.000000 lol-esp-api-0.3/src/lol_esp_api/lol_esports_api.py
+drwxr-xr-x   0 madking   (1000) madking   (1000)        0 2023-07-05 05:18:24.239156 lol-esp-api-0.3/src/lol_esp_api.egg-info/
+-rw-r--r--   0 madking   (1000) madking   (1000)      249 2023-07-05 05:18:24.000000 lol-esp-api-0.3/src/lol_esp_api.egg-info/PKG-INFO
+-rw-r--r--   0 madking   (1000) madking   (1000)      483 2023-07-05 05:18:24.000000 lol-esp-api-0.3/src/lol_esp_api.egg-info/SOURCES.txt
+-rw-r--r--   0 madking   (1000) madking   (1000)        1 2023-07-05 05:18:24.000000 lol-esp-api-0.3/src/lol_esp_api.egg-info/dependency_links.txt
+-rw-r--r--   0 madking   (1000) madking   (1000)        9 2023-07-05 05:18:24.000000 lol-esp-api-0.3/src/lol_esp_api.egg-info/requires.txt
+-rw-r--r--   0 madking   (1000) madking   (1000)       12 2023-07-05 05:18:24.000000 lol-esp-api-0.3/src/lol_esp_api.egg-info/top_level.txt
```

### Comparing `lol-esp-api-0.24.5/LICENSE` & `lol-esp-api-0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `lol-esp-api-0.24.5/src/lol_esp_api/apis/eventsAPI.py` & `lol-esp-api-0.3/src/lol_esp_api/apis/eventsAPI.py`

 * *Files 1% similar despite different names*

```diff
@@ -12,15 +12,15 @@
 
 def getLive():
     url = "https://esports-api.lolesports.com/persisted/gw/getLive?hl=en-US"
 
     return request(url)
 
 
-def getCompeletedEvents(eventID=""):
+def getCompeletedEvents(eventID):
     url = "https://esports-api.lolesports.com/persisted/gw/getCompletedEvents?tournamentId={0}&hl=en-US".format(
         eventID
     )
 
     return request(url)
```

### Comparing `lol-esp-api-0.24.5/src/lol_esp_api/apis/leaguesAPI.py` & `lol-esp-api-0.3/src/lol_esp_api/apis/leaguesAPI.py`

 * *Files 1% similar despite different names*

```diff
@@ -33,25 +33,25 @@
     return request(url)
 
 def getTournaments():
     url = "https://esports-api.lolesports.com/persisted/gw/getTournaments?hl=en-US"
 
     return request(url)
 
-def getTourmanentById(id):
+def getTournamentById(id):
     response = getTournaments()
     tournaments = response['data']['tournaments']
 
     for tournament in tournaments:
         if tournament['id'] == id:
             return tournament
         
     return "Tournament not found!"
 
-def getTourmanentBySlug(slug):
+def getTournamentBySlug(slug):
     response = getTournaments()
     tournaments = response['data']['tournaments']
 
     for tournament in tournaments:
         if tournament['slug'] == slug:
             return tournament
```

### Comparing `lol-esp-api-0.24.5/src/lol_esp_api/apis/teamsAPI.py` & `lol-esp-api-0.3/src/lol_esp_api/apis/teamsAPI.py`

 * *Files identical despite different names*

