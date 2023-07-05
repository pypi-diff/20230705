# Comparing `tmp/fgo_api_types-2023.7.5.15.28.38.tar.gz` & `tmp/fgo_api_types-2023.7.5.6.44.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fgo_api_types-2023.7.5.15.28.38.tar", max compression
+gzip compressed data, was "fgo_api_types-2023.7.5.6.44.7.tar", max compression
```

## Comparing `fgo_api_types-2023.7.5.15.28.38.tar` & `fgo_api_types-2023.7.5.6.44.7.tar`

### file list

```diff
@@ -1,14 +1,14 @@
--rw-r--r--   0        0        0    34523 2023-07-05 15:28:19.688435 fgo_api_types-2023.7.5.15.28.38/LICENSE
--rw-r--r--   0        0        0      449 2023-07-05 15:28:19.688435 fgo_api_types-2023.7.5.15.28.38/README.md
--rw-r--r--   0        0        0        0 2023-07-05 15:28:38.400507 fgo_api_types-2023.7.5.15.28.38/fgo_api_types/__init__.py
--rw-r--r--   0        0        0      434 2023-07-05 15:28:38.400507 fgo_api_types-2023.7.5.15.28.38/fgo_api_types/base.py
--rw-r--r--   0        0        0     4195 2023-07-05 15:28:38.400507 fgo_api_types-2023.7.5.15.28.38/fgo_api_types/basic.py
--rw-r--r--   0        0        0     3631 2023-07-05 15:28:38.400507 fgo_api_types-2023.7.5.15.28.38/fgo_api_types/common.py
--rw-r--r--   0        0        0    38038 2023-07-05 15:28:38.400507 fgo_api_types-2023.7.5.15.28.38/fgo_api_types/enums.py
--rw-r--r--   0        0        0   160313 2023-07-05 15:28:38.400507 fgo_api_types-2023.7.5.15.28.38/fgo_api_types/gameenums.py
--rw-r--r--   0        0        0    78537 2023-07-05 15:28:38.400507 fgo_api_types-2023.7.5.15.28.38/fgo_api_types/nice.py
--rw-r--r--   0        0        0    53238 2023-07-05 15:28:38.400507 fgo_api_types-2023.7.5.15.28.38/fgo_api_types/raw.py
--rw-r--r--   0        0        0     4176 2023-07-05 15:28:38.400507 fgo_api_types-2023.7.5.15.28.38/fgo_api_types/rayshift.py
--rw-r--r--   0        0        0    19183 2023-07-05 15:28:38.400507 fgo_api_types-2023.7.5.15.28.38/fgo_api_types/search.py
--rw-r--r--   0        0        0      520 2023-07-05 15:28:38.728508 fgo_api_types-2023.7.5.15.28.38/pyproject.toml
--rw-r--r--   0        0        0     1222 1970-01-01 00:00:00.000000 fgo_api_types-2023.7.5.15.28.38/PKG-INFO
+-rw-r--r--   0        0        0    34523 2023-07-05 06:43:48.212693 fgo_api_types-2023.7.5.6.44.7/LICENSE
+-rw-r--r--   0        0        0      449 2023-07-05 06:43:48.212693 fgo_api_types-2023.7.5.6.44.7/README.md
+-rw-r--r--   0        0        0        0 2023-07-05 06:44:07.492961 fgo_api_types-2023.7.5.6.44.7/fgo_api_types/__init__.py
+-rw-r--r--   0        0        0      434 2023-07-05 06:44:07.492961 fgo_api_types-2023.7.5.6.44.7/fgo_api_types/base.py
+-rw-r--r--   0        0        0     4195 2023-07-05 06:44:07.492961 fgo_api_types-2023.7.5.6.44.7/fgo_api_types/basic.py
+-rw-r--r--   0        0        0     3631 2023-07-05 06:44:07.496961 fgo_api_types-2023.7.5.6.44.7/fgo_api_types/common.py
+-rw-r--r--   0        0        0    38038 2023-07-05 06:44:07.496961 fgo_api_types-2023.7.5.6.44.7/fgo_api_types/enums.py
+-rw-r--r--   0        0        0   160313 2023-07-05 06:44:07.496961 fgo_api_types-2023.7.5.6.44.7/fgo_api_types/gameenums.py
+-rw-r--r--   0        0        0    78308 2023-07-05 06:44:07.496961 fgo_api_types-2023.7.5.6.44.7/fgo_api_types/nice.py
+-rw-r--r--   0        0        0    53003 2023-07-05 06:44:07.496961 fgo_api_types-2023.7.5.6.44.7/fgo_api_types/raw.py
+-rw-r--r--   0        0        0     4176 2023-07-05 06:44:07.496961 fgo_api_types-2023.7.5.6.44.7/fgo_api_types/rayshift.py
+-rw-r--r--   0        0        0    19183 2023-07-05 06:44:07.496961 fgo_api_types-2023.7.5.6.44.7/fgo_api_types/search.py
+-rw-r--r--   0        0        0      520 2023-07-05 06:44:07.836966 fgo_api_types-2023.7.5.6.44.7/pyproject.toml
+-rw-r--r--   0        0        0     1220 1970-01-01 00:00:00.000000 fgo_api_types-2023.7.5.6.44.7/PKG-INFO
```

### Comparing `fgo_api_types-2023.7.5.15.28.38/LICENSE` & `fgo_api_types-2023.7.5.6.44.7/LICENSE`

 * *Files identical despite different names*

### Comparing `fgo_api_types-2023.7.5.15.28.38/fgo_api_types/basic.py` & `fgo_api_types-2023.7.5.6.44.7/fgo_api_types/basic.py`

 * *Files identical despite different names*

### Comparing `fgo_api_types-2023.7.5.15.28.38/fgo_api_types/common.py` & `fgo_api_types-2023.7.5.6.44.7/fgo_api_types/common.py`

 * *Files identical despite different names*

### Comparing `fgo_api_types-2023.7.5.15.28.38/fgo_api_types/enums.py` & `fgo_api_types-2023.7.5.6.44.7/fgo_api_types/enums.py`

 * *Files identical despite different names*

### Comparing `fgo_api_types-2023.7.5.15.28.38/fgo_api_types/gameenums.py` & `fgo_api_types-2023.7.5.6.44.7/fgo_api_types/gameenums.py`

 * *Files identical despite different names*

### Comparing `fgo_api_types-2023.7.5.15.28.38/fgo_api_types/nice.py` & `fgo_api_types-2023.7.5.6.44.7/fgo_api_types/nice.py`

 * *Files 0% similar despite different names*

```diff
@@ -1936,24 +1936,14 @@
     assistCard: NiceCardType
     image: HttpUrl
     skill: NiceSkill
     skillLv: int
     releaseConditions: list[NiceCommonRelease]
 
 
-class NiceHeelPortrait(BaseModelORJson):
-    id: int
-    name: str
-    image: HttpUrl
-    dispCondType: NiceCondType
-    dispCondId: int
-    dispCondNum: int
-    script: dict[str, Any]
-
-
 class NiceEvent(BaseModelORJson):
     id: int
     type: NiceEventType
     name: str
     originalName: str
     shortName: str
     detail: str
@@ -1982,15 +1972,14 @@
     recipes: list[NiceEventRecipe]
     digging: NiceEventDigging | None
     cooltime: NiceEventCooltime | None
     fortifications: list[NiceEventFortification]
     campaigns: list[NiceEventCampaign]
     campaignQuests: list[NiceEventQuest]
     commandAssists: list[NiceEventCommandAssist]
-    heelPortraits: list[NiceHeelPortrait]
     voicePlays: list[NiceEventVoicePlay]
     voices: list[NiceVoiceGroup] = Field(
         ..., description="All voice lines related to this event"
     )
 
 
 class NiceMasterMission(BaseModelORJson):
```

### Comparing `fgo_api_types-2023.7.5.15.28.38/fgo_api_types/raw.py` & `fgo_api_types-2023.7.5.6.44.7/fgo_api_types/raw.py`

 * *Files 1% similar despite different names*

```diff
@@ -1370,25 +1370,14 @@
 
 class MstEventAlloutBattle(BaseModelORJson):
     eventId: int
     alloutBattleId: int
     warId: int
 
 
-class MstHeelPortrait(BaseModelORJson):
-    id: int
-    name: str
-    imageId: int
-    eventId: int
-    dispCondType: int
-    dispCondId: int
-    dispCondNum: int
-    script: dict[str, Any]
-
-
 class MstEvent(BaseModelORJson):
     script: list[dict[str, str]]  # []
     id: int  # 10083
     baseEventId: int  # 0
     type: int  # 20
     openType: int  # 1
     name: str  # "劇場版「Fate/stay night [Heaven's Feel]」公開記念キャンペーン"
@@ -2036,15 +2025,14 @@
     mstEventCampaign: list[MstEventCampaign]
     mstEventQuest: list[MstEventQuest]
     mstEventBulletinBoard: list[MstEventBulletinBoard]
     mstEventBulletinBoardRelease: list[MstEventBulletinBoardRelease]
     mstEventRecipe: list[MstEventRecipe]
     mstEventRecipeGift: list[MstEventRecipeGift]
     mstEventCommandAssist: list[MstEventCommandAssist]
-    mstHeelPortrait: list[MstHeelPortrait]
     mstItem: list[MstItem]
     mstCommonConsume: list[MstCommonConsume]
     mstCommonRelease: list[MstCommonRelease]
     mstSvtVoice: list[MstSvtVoice]
     mstVoice: list[MstVoice]
     mstSvtGroup: list[MstSvtGroup]
     mstSubtitle: list[GlobalNewMstSubtitle]
```

### Comparing `fgo_api_types-2023.7.5.15.28.38/fgo_api_types/rayshift.py` & `fgo_api_types-2023.7.5.6.44.7/fgo_api_types/rayshift.py`

 * *Files identical despite different names*

### Comparing `fgo_api_types-2023.7.5.15.28.38/fgo_api_types/search.py` & `fgo_api_types-2023.7.5.6.44.7/fgo_api_types/search.py`

 * *Files identical despite different names*

### Comparing `fgo_api_types-2023.7.5.15.28.38/pyproject.toml` & `fgo_api_types-2023.7.5.6.44.7/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "fgo-api-types"
-version = "2023.07.05.15.28.38"
+version = "2023.07.05.06.44.07"
 description = "Provide Pydantic types from FGO API"
 authors = ["squaresmile <squaresmile@protonmail.com>"]
 readme = "README.md"
 homepage = "https://api.atlasacademy.io"
 repository = "https://github.com/atlasacademy/fgo-game-data-api"
 
 [tool.poetry.dependencies]
```

### Comparing `fgo_api_types-2023.7.5.15.28.38/PKG-INFO` & `fgo_api_types-2023.7.5.6.44.7/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fgo-api-types
-Version: 2023.7.5.15.28.38
+Version: 2023.7.5.6.44.7
 Summary: Provide Pydantic types from FGO API
 Home-page: https://api.atlasacademy.io
 Author: squaresmile
 Author-email: squaresmile@protonmail.com
 Requires-Python: >=3.6,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.6
```

