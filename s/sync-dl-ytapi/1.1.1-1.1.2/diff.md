# Comparing `tmp/sync_dl_ytapi-1.1.1-py3-none-any.whl.zip` & `tmp/sync_dl_ytapi-1.1.2-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,12 +1,12 @@
-Zip file size: 9523 bytes, number of entries: 10
--rw-r--r--  2.0 unx       95 b- defN 23-Jul-04 17:23 sync_dl_ytapi/__init__.py
+Zip file size: 9526 bytes, number of entries: 10
+-rw-r--r--  2.0 unx       95 b- defN 23-Jul-04 22:24 sync_dl_ytapi/__init__.py
 -rw-r--r--  2.0 unx     2147 b- defN 22-Feb-03 02:14 sync_dl_ytapi/commands.py
 -rw-r--r--  2.0 unx     2970 b- defN 22-Feb-03 02:16 sync_dl_ytapi/credentials.py
--rw-r--r--  2.0 unx     6471 b- defN 23-Jul-04 17:22 sync_dl_ytapi/helpers.py
+-rw-r--r--  2.0 unx     6489 b- defN 23-Jul-04 22:23 sync_dl_ytapi/helpers.py
 -rw-r--r--  2.0 unx     6262 b- defN 22-Feb-03 02:26 sync_dl_ytapi/ytapiWrappers.py
--rw-r--r--  2.0 unx     1072 b- defN 23-Jul-04 17:47 sync_dl_ytapi-1.1.1.dist-info/LICENCE
--rw-r--r--  2.0 unx     2994 b- defN 23-Jul-04 17:47 sync_dl_ytapi-1.1.1.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 23-Jul-04 17:47 sync_dl_ytapi-1.1.1.dist-info/WHEEL
--rw-r--r--  2.0 unx       14 b- defN 23-Jul-04 17:47 sync_dl_ytapi-1.1.1.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx      831 b- defN 23-Jul-04 17:47 sync_dl_ytapi-1.1.1.dist-info/RECORD
-10 files, 22948 bytes uncompressed, 8099 bytes compressed:  64.7%
+-rw-r--r--  2.0 unx     1072 b- defN 23-Jul-04 22:26 sync_dl_ytapi-1.1.2.dist-info/LICENCE
+-rw-r--r--  2.0 unx     2994 b- defN 23-Jul-04 22:26 sync_dl_ytapi-1.1.2.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 23-Jul-04 22:26 sync_dl_ytapi-1.1.2.dist-info/WHEEL
+-rw-r--r--  2.0 unx       14 b- defN 23-Jul-04 22:26 sync_dl_ytapi-1.1.2.dist-info/top_level.txt
+?rw-rw-r--  2.0 unx      831 b- defN 23-Jul-04 22:26 sync_dl_ytapi-1.1.2.dist-info/RECORD
+10 files, 22966 bytes uncompressed, 8102 bytes compressed:  64.7%
```

## zipnote {}

```diff
@@ -9,23 +9,23 @@
 
 Filename: sync_dl_ytapi/helpers.py
 Comment: 
 
 Filename: sync_dl_ytapi/ytapiWrappers.py
 Comment: 
 
-Filename: sync_dl_ytapi-1.1.1.dist-info/LICENCE
+Filename: sync_dl_ytapi-1.1.2.dist-info/LICENCE
 Comment: 
 
-Filename: sync_dl_ytapi-1.1.1.dist-info/METADATA
+Filename: sync_dl_ytapi-1.1.2.dist-info/METADATA
 Comment: 
 
-Filename: sync_dl_ytapi-1.1.1.dist-info/WHEEL
+Filename: sync_dl_ytapi-1.1.2.dist-info/WHEEL
 Comment: 
 
-Filename: sync_dl_ytapi-1.1.1.dist-info/top_level.txt
+Filename: sync_dl_ytapi-1.1.2.dist-info/top_level.txt
 Comment: 
 
-Filename: sync_dl_ytapi-1.1.1.dist-info/RECORD
+Filename: sync_dl_ytapi-1.1.2.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## sync_dl_ytapi/__init__.py

```diff
@@ -1,2 +1,2 @@
 # This submodule extends sync_dl with tools for editing remote playlists
-__version__ = "1.1.1"
+__version__ = "1.1.2"
```

## sync_dl_ytapi/helpers.py

```diff
@@ -7,28 +7,25 @@
 
 def getPlId(plUrl):
     match = re.search(cfg.plIdRe,plUrl)
     assert match is not None
     return match.group()[5:]
     
 
+
+
 def oldToNewPushOrder(remoteIds, localIds):
     '''
     Used in pushLocalOrder
     '''
     
     blankingStr = ''
-    localIds = [localId for localId in localIds]
     remoteIds = [remoteId for remoteId in remoteIds]
-
-
     # Removes all localIds which arent in remoteIds (we arent going to upload songs)
-    for i in reversed(range(len(localIds))):
-        if localIds[i] not in remoteIds:
-            del localIds[i]
+    localIds = [id for id in localIds if id in remoteIds]
 
     lenRemote = len(remoteIds)
     oldToNew=[-1]*lenRemote
 
     prevOldIndex = -1
     newIndex = 0
 
@@ -42,15 +39,19 @@
             continue
 
         if newIndex == lenRemote:
             break
 
         localId = localIds.pop(0)
 
-        oldIndex = remoteIds.index(localId)
+        try:
+            oldIndex = remoteIds.index(localId)
+        except:
+            # duplicate local id that is not duplicated in remoteIds
+            continue
         remoteIds[oldIndex] = blankingStr
 
         oldToNew[oldIndex] = newIndex
 
         prevOldIndex = oldIndex
         newIndex+=1
     return oldToNew
```

## Comparing `sync_dl_ytapi-1.1.1.dist-info/LICENCE` & `sync_dl_ytapi-1.1.2.dist-info/LICENCE`

 * *Files identical despite different names*

## Comparing `sync_dl_ytapi-1.1.1.dist-info/METADATA` & `sync_dl_ytapi-1.1.2.dist-info/METADATA`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sync-dl-ytapi
-Version: 1.1.1
+Version: 1.1.2
 Summary: An addon for sync-dl, providing commands which utilize the youtube api
 Home-page: https://github.com/PrinceOfPuppers/sync-dl-ytapi
 Author: Joshua McPherson
 Author-email: joshuamcpherson5@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

## Comparing `sync_dl_ytapi-1.1.1.dist-info/RECORD` & `sync_dl_ytapi-1.1.2.dist-info/RECORD`

 * *Files 22% similar despite different names*

```diff
@@ -1,10 +1,10 @@
-sync_dl_ytapi/__init__.py,sha256=ww9U0IXDaKLPKuKoEH-ZkZN6bzItrcHy5WKfj-h9XnM,95
+sync_dl_ytapi/__init__.py,sha256=Aa__z1TwUKS3CvvPEYGDfRLOhQyadP-KOhYNg_zB3eI,95
 sync_dl_ytapi/commands.py,sha256=EV0ridtUYQ664J6RDM5UV0kA-IO9iPTrrdfBw0vZ9ok,2147
 sync_dl_ytapi/credentials.py,sha256=kXUdPOg22uz50yYcRFyim2Gbfm-TQz03tt8ll-6bo2Y,2970
-sync_dl_ytapi/helpers.py,sha256=xlrSJjDJLsPhWHJNzKEwI5vZVgBPChOOb6GcoqWCGUw,6471
+sync_dl_ytapi/helpers.py,sha256=ry4gfyDZ-fy6f7dgU71SUma4O6abuQ09iAT_nGgfLvI,6489
 sync_dl_ytapi/ytapiWrappers.py,sha256=gj9i9_xXyhWc8yFAjjPWKPvada6xsKCX_PpgY5FhX24,6262
-sync_dl_ytapi-1.1.1.dist-info/LICENCE,sha256=8va7PxKEglvuCq2Pnetv39LJ65l21CIS9Oh4vDyZVCY,1072
-sync_dl_ytapi-1.1.1.dist-info/METADATA,sha256=UXUX41OxxMW6DwxtqWFfyqdr5z_ZruTvq8QZ9gxM_88,2994
-sync_dl_ytapi-1.1.1.dist-info/WHEEL,sha256=G16H4A3IeoQmnOrYV4ueZGKSjhipXx8zc8nu9FGlvMA,92
-sync_dl_ytapi-1.1.1.dist-info/top_level.txt,sha256=R7_ogJWbgrOrWwpMIUAI7LLPCqnEgoLrWmp7wFoMYcY,14
-sync_dl_ytapi-1.1.1.dist-info/RECORD,,
+sync_dl_ytapi-1.1.2.dist-info/LICENCE,sha256=8va7PxKEglvuCq2Pnetv39LJ65l21CIS9Oh4vDyZVCY,1072
+sync_dl_ytapi-1.1.2.dist-info/METADATA,sha256=lKd3bZ0dPeanMRV_6jZJhaKOrfmFBuagURMo3M4IlkE,2994
+sync_dl_ytapi-1.1.2.dist-info/WHEEL,sha256=G16H4A3IeoQmnOrYV4ueZGKSjhipXx8zc8nu9FGlvMA,92
+sync_dl_ytapi-1.1.2.dist-info/top_level.txt,sha256=R7_ogJWbgrOrWwpMIUAI7LLPCqnEgoLrWmp7wFoMYcY,14
+sync_dl_ytapi-1.1.2.dist-info/RECORD,,
```

