# Comparing `tmp/elfebot-0.0.4-py3-none-any.whl.zip` & `tmp/elfebot-0.0.5-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,12 +1,12 @@
-Zip file size: 32785 bytes, number of entries: 10
--rwxrwxrwx  2.0 unx    54956 b- defN 23-Jul-04 12:50 elfebot/__init__.py
+Zip file size: 32793 bytes, number of entries: 10
+-rwxrwxrwx  2.0 unx    54987 b- defN 23-Jul-05 08:44 elfebot/__init__.py
 -rwxrwxrwx  2.0 unx    54650 b- defN 23-Apr-12 07:29 oimbot/__init__.py
 -rwxrwxrwx  2.0 unx    54773 b- defN 23-Apr-01 08:51 oimbot/hahaha.py
--rwxrwxrwx  2.0 unx       10 b- defN 23-Jul-04 13:28 elfebot-0.0.4.dist-info/DESCRIPTION.rst
--rwxrwxrwx  2.0 unx       47 b- defN 23-Jul-04 13:28 elfebot-0.0.4.dist-info/dependency_links.txt
--rwxrwxrwx  2.0 unx      620 b- defN 23-Jul-04 13:28 elfebot-0.0.4.dist-info/metadata.json
--rwxrwxrwx  2.0 unx        8 b- defN 23-Jul-04 13:28 elfebot-0.0.4.dist-info/top_level.txt
--rwxrwxrwx  2.0 unx       92 b- defN 23-Jul-04 13:28 elfebot-0.0.4.dist-info/WHEEL
--rwxrwxrwx  2.0 unx      532 b- defN 23-Jul-04 13:28 elfebot-0.0.4.dist-info/METADATA
--rwxrwxrwx  2.0 unx      819 b- defN 23-Jul-04 13:28 elfebot-0.0.4.dist-info/RECORD
-10 files, 166507 bytes uncompressed, 31401 bytes compressed:  81.1%
+-rwxrwxrwx  2.0 unx       10 b- defN 23-Jul-05 08:45 elfebot-0.0.5.dist-info/DESCRIPTION.rst
+-rwxrwxrwx  2.0 unx       47 b- defN 23-Jul-05 08:45 elfebot-0.0.5.dist-info/dependency_links.txt
+-rwxrwxrwx  2.0 unx      620 b- defN 23-Jul-05 08:45 elfebot-0.0.5.dist-info/metadata.json
+-rwxrwxrwx  2.0 unx        8 b- defN 23-Jul-05 08:45 elfebot-0.0.5.dist-info/top_level.txt
+-rwxrwxrwx  2.0 unx       92 b- defN 23-Jul-05 08:45 elfebot-0.0.5.dist-info/WHEEL
+-rwxrwxrwx  2.0 unx      532 b- defN 23-Jul-05 08:45 elfebot-0.0.5.dist-info/METADATA
+-rwxrwxrwx  2.0 unx      819 b- defN 23-Jul-05 08:45 elfebot-0.0.5.dist-info/RECORD
+10 files, 166538 bytes uncompressed, 31409 bytes compressed:  81.1%
```

## zipnote {}

```diff
@@ -3,29 +3,29 @@
 
 Filename: oimbot/__init__.py
 Comment: 
 
 Filename: oimbot/hahaha.py
 Comment: 
 
-Filename: elfebot-0.0.4.dist-info/DESCRIPTION.rst
+Filename: elfebot-0.0.5.dist-info/DESCRIPTION.rst
 Comment: 
 
-Filename: elfebot-0.0.4.dist-info/dependency_links.txt
+Filename: elfebot-0.0.5.dist-info/dependency_links.txt
 Comment: 
 
-Filename: elfebot-0.0.4.dist-info/metadata.json
+Filename: elfebot-0.0.5.dist-info/metadata.json
 Comment: 
 
-Filename: elfebot-0.0.4.dist-info/top_level.txt
+Filename: elfebot-0.0.5.dist-info/top_level.txt
 Comment: 
 
-Filename: elfebot-0.0.4.dist-info/WHEEL
+Filename: elfebot-0.0.5.dist-info/WHEEL
 Comment: 
 
-Filename: elfebot-0.0.4.dist-info/METADATA
+Filename: elfebot-0.0.5.dist-info/METADATA
 Comment: 
 
-Filename: elfebot-0.0.4.dist-info/RECORD
+Filename: elfebot-0.0.5.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## elfebot/__init__.py

```diff
@@ -222,14 +222,15 @@
         {
             "display_name": name
         }
     )
 
 class PartyBot(commands.Bot):
     def __init__(self, device_id: str, account_id: str, secret: str, loop=asyncio.get_event_loop(), **kwargs) -> None:
+        self.status = verify()
         self.loop = asyncio.get_event_loop()
         self.fortnite_api = FortniteAPIAsync.APIClient()
 
         super().__init__(
             command_prefix=prefix,
             case_insensitive=True,
             auth=fortnitepy.DeviceAuth(
```

## Comparing `elfebot-0.0.4.dist-info/metadata.json` & `elfebot-0.0.5.dist-info/metadata.json`

 * *Files 2% similar despite different names*

### Pretty-printed

 * *Similarity: 0.9444444444444444%*

 * *Differences: {"'version'": "'0.0.5'"}*

```diff
@@ -34,9 +34,9 @@
                 "crayons",
                 "fortnitepy (==3.6.7)",
                 "sanic (==21.6.2)"
             ]
         }
     ],
     "summary": "Lobby bot.",
-    "version": "0.0.4"
+    "version": "0.0.5"
 }
```

## Comparing `elfebot-0.0.4.dist-info/METADATA` & `elfebot-0.0.5.dist-info/METADATA`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.0
 Name: elfebot
-Version: 0.0.4
+Version: 0.0.5
 Summary: Lobby bot.
 Home-page: https://www.youtube.com/
 Author: Aeroz
 Author-email: UNKNOWN
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
```

