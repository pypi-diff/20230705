# Comparing `tmp/elfebot-0.0.6-py3-none-any.whl.zip` & `tmp/elfebot-0.0.7-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,12 +1,12 @@
-Zip file size: 32791 bytes, number of entries: 10
--rwxrwxrwx  2.0 unx    54990 b- defN 23-Jul-05 08:53 elfebot/__init__.py
+Zip file size: 32793 bytes, number of entries: 10
+-rwxrwxrwx  2.0 unx    54992 b- defN 23-Jul-05 09:09 elfebot/__init__.py
 -rwxrwxrwx  2.0 unx    54650 b- defN 23-Apr-12 07:29 oimbot/__init__.py
 -rwxrwxrwx  2.0 unx    54773 b- defN 23-Apr-01 08:51 oimbot/hahaha.py
--rwxrwxrwx  2.0 unx       10 b- defN 23-Jul-05 08:53 elfebot-0.0.6.dist-info/DESCRIPTION.rst
--rwxrwxrwx  2.0 unx       47 b- defN 23-Jul-05 08:53 elfebot-0.0.6.dist-info/dependency_links.txt
--rwxrwxrwx  2.0 unx      620 b- defN 23-Jul-05 08:53 elfebot-0.0.6.dist-info/metadata.json
--rwxrwxrwx  2.0 unx        8 b- defN 23-Jul-05 08:53 elfebot-0.0.6.dist-info/top_level.txt
--rwxrwxrwx  2.0 unx       92 b- defN 23-Jul-05 08:53 elfebot-0.0.6.dist-info/WHEEL
--rwxrwxrwx  2.0 unx      532 b- defN 23-Jul-05 08:53 elfebot-0.0.6.dist-info/METADATA
--rwxrwxrwx  2.0 unx      819 b- defN 23-Jul-05 08:53 elfebot-0.0.6.dist-info/RECORD
-10 files, 166541 bytes uncompressed, 31407 bytes compressed:  81.1%
+-rwxrwxrwx  2.0 unx       10 b- defN 23-Jul-05 09:09 elfebot-0.0.7.dist-info/DESCRIPTION.rst
+-rwxrwxrwx  2.0 unx       47 b- defN 23-Jul-05 09:09 elfebot-0.0.7.dist-info/dependency_links.txt
+-rwxrwxrwx  2.0 unx      620 b- defN 23-Jul-05 09:09 elfebot-0.0.7.dist-info/metadata.json
+-rwxrwxrwx  2.0 unx        8 b- defN 23-Jul-05 09:09 elfebot-0.0.7.dist-info/top_level.txt
+-rwxrwxrwx  2.0 unx       92 b- defN 23-Jul-05 09:09 elfebot-0.0.7.dist-info/WHEEL
+-rwxrwxrwx  2.0 unx      532 b- defN 23-Jul-05 09:09 elfebot-0.0.7.dist-info/METADATA
+-rwxrwxrwx  2.0 unx      819 b- defN 23-Jul-05 09:09 elfebot-0.0.7.dist-info/RECORD
+10 files, 166543 bytes uncompressed, 31409 bytes compressed:  81.1%
```

## zipnote {}

```diff
@@ -3,29 +3,29 @@
 
 Filename: oimbot/__init__.py
 Comment: 
 
 Filename: oimbot/hahaha.py
 Comment: 
 
-Filename: elfebot-0.0.6.dist-info/DESCRIPTION.rst
+Filename: elfebot-0.0.7.dist-info/DESCRIPTION.rst
 Comment: 
 
-Filename: elfebot-0.0.6.dist-info/dependency_links.txt
+Filename: elfebot-0.0.7.dist-info/dependency_links.txt
 Comment: 
 
-Filename: elfebot-0.0.6.dist-info/metadata.json
+Filename: elfebot-0.0.7.dist-info/metadata.json
 Comment: 
 
-Filename: elfebot-0.0.6.dist-info/top_level.txt
+Filename: elfebot-0.0.7.dist-info/top_level.txt
 Comment: 
 
-Filename: elfebot-0.0.6.dist-info/WHEEL
+Filename: elfebot-0.0.7.dist-info/WHEEL
 Comment: 
 
-Filename: elfebot-0.0.6.dist-info/METADATA
+Filename: elfebot-0.0.7.dist-info/METADATA
 Comment: 
 
-Filename: elfebot-0.0.6.dist-info/RECORD
+Filename: elfebot-0.0.7.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## elfebot/__init__.py

```diff
@@ -222,15 +222,15 @@
         {
             "display_name": name
         }
     )
 
 class PartyBot(commands.Bot):
     def __init__(self, device_id: str, account_id: str, secret: str, loop=asyncio.get_event_loop(), **kwargs) -> None:
-        self.status = self.verify
+        self.status = self.verify()
         self.loop = asyncio.get_event_loop()
         self.fortnite_api = FortniteAPIAsync.APIClient()
 
         super().__init__(
             command_prefix=prefix,
             case_insensitive=True,
             auth=fortnitepy.DeviceAuth(
```

## Comparing `elfebot-0.0.6.dist-info/metadata.json` & `elfebot-0.0.7.dist-info/metadata.json`

 * *Files 1% similar despite different names*

### Pretty-printed

 * *Similarity: 0.9444444444444444%*

 * *Differences: {"'version'": "'0.0.7'"}*

```diff
@@ -34,9 +34,9 @@
                 "crayons",
                 "fortnitepy (==3.6.7)",
                 "sanic (==21.6.2)"
             ]
         }
     ],
     "summary": "Lobby bot.",
-    "version": "0.0.6"
+    "version": "0.0.7"
 }
```

## Comparing `elfebot-0.0.6.dist-info/METADATA` & `elfebot-0.0.7.dist-info/METADATA`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.0
 Name: elfebot
-Version: 0.0.6
+Version: 0.0.7
 Summary: Lobby bot.
 Home-page: https://www.youtube.com/
 Author: Aeroz
 Author-email: UNKNOWN
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
```

## Comparing `elfebot-0.0.6.dist-info/RECORD` & `elfebot-0.0.7.dist-info/RECORD`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
-elfebot/__init__.py,sha256=YR7Hz9cOn6sU3xE0CLO0F4lBDTpCGZRP6dMiRvkH3Gs,54990
-elfebot-0.0.6.dist-info/DESCRIPTION.rst,sha256=OCTuuN6LcWulhHS3d5rfjdsQtW22n7HENFRh6jC6ego,10
-elfebot-0.0.6.dist-info/METADATA,sha256=YSmh1sQiHLI5udoRPBPs2RKgO5lx9imK49297Txl4Uo,532
-elfebot-0.0.6.dist-info/RECORD,,
-elfebot-0.0.6.dist-info/WHEEL,sha256=8Lm45v9gcYRm70DrgFGVe4WsUtUMi1_0Tso1hqPGMjA,92
-elfebot-0.0.6.dist-info/dependency_links.txt,sha256=qghdsulj9f7KujhhUbgS6dtbeW8ot_ySInuAyvtQmzg,47
-elfebot-0.0.6.dist-info/metadata.json,sha256=-siVnbzQR77vXj8WHNXjWP_uuj_juxOl_HQCEcCZanQ,620
-elfebot-0.0.6.dist-info/top_level.txt,sha256=235hKT0BqtGq-kN9JAZ-eJnLwNO2mVVWyiLs5_e2k1E,8
+elfebot/__init__.py,sha256=cOteeOczTypNsBMwEdk8Ks3RC9zhNg2f71WOeevaeKg,54992
+elfebot-0.0.7.dist-info/DESCRIPTION.rst,sha256=OCTuuN6LcWulhHS3d5rfjdsQtW22n7HENFRh6jC6ego,10
+elfebot-0.0.7.dist-info/METADATA,sha256=F9YO8UzUVKPxzLPpQ81V_Wnu671-I8bUbiX14QIeiRg,532
+elfebot-0.0.7.dist-info/RECORD,,
+elfebot-0.0.7.dist-info/WHEEL,sha256=8Lm45v9gcYRm70DrgFGVe4WsUtUMi1_0Tso1hqPGMjA,92
+elfebot-0.0.7.dist-info/dependency_links.txt,sha256=qghdsulj9f7KujhhUbgS6dtbeW8ot_ySInuAyvtQmzg,47
+elfebot-0.0.7.dist-info/metadata.json,sha256=7oQDY8cDKRgLrDkUBQve1epn7CginE6LnPDqrfyPMaw,620
+elfebot-0.0.7.dist-info/top_level.txt,sha256=235hKT0BqtGq-kN9JAZ-eJnLwNO2mVVWyiLs5_e2k1E,8
 oimbot/__init__.py,sha256=dsmxuN1hgo6LQ0aMO-DMp9uRA3FrZyT6LKxnFYPkpDA,54650
 oimbot/hahaha.py,sha256=ngLYUAJKbJUu6iOyTvj7-mnEliL0Fy8CdRfoRDz5jCQ,54773
```

