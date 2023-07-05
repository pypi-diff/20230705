# Comparing `tmp/tdfs4ds-0.1.0.0-py3-none-any.whl.zip` & `tmp/tdfs4ds-0.1.0.1-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,14 +1,14 @@
-Zip file size: 73823 bytes, number of entries: 12
+Zip file size: 74991 bytes, number of entries: 12
 -rw-rw-rw-  2.0 fat       23 b- defN 23-Jul-05 10:56 tdfs/__init__.py
 -rw-rw-rw-  2.0 fat      985 b- defN 23-Jul-05 13:45 tdfs/datasets.py
 -rw-rw-rw-  2.0 fat    31354 b- defN 23-Jul-05 14:47 tdfs/feature_store.py
 -rw-rw-rw-  2.0 fat   112488 b- defN 23-Jul-05 13:43 tdfs/data/curves.csv
--rw-rw-rw-  2.0 fat       23 b- defN 23-Jul-05 10:56 tdfs4ds/__init__.py
+-rw-rw-rw-  2.0 fat       23 b- defN 23-Jul-05 15:31 tdfs4ds/__init__.py
 -rw-rw-rw-  2.0 fat      985 b- defN 23-Jul-05 13:45 tdfs4ds/datasets.py
 -rw-rw-rw-  2.0 fat    31279 b- defN 23-Jul-05 15:03 tdfs4ds/feature_store.py
 -rw-rw-rw-  2.0 fat   112488 b- defN 23-Jul-05 13:43 tdfs4ds/data/curves.csv
--rw-rw-rw-  2.0 fat     2658 b- defN 23-Jul-05 15:12 tdfs4ds-0.1.0.0.dist-info/METADATA
--rw-rw-rw-  2.0 fat       92 b- defN 23-Jul-05 15:12 tdfs4ds-0.1.0.0.dist-info/WHEEL
--rw-rw-rw-  2.0 fat        8 b- defN 23-Jul-05 15:12 tdfs4ds-0.1.0.0.dist-info/top_level.txt
-?rw-rw-r--  2.0 fat      919 b- defN 23-Jul-05 15:12 tdfs4ds-0.1.0.0.dist-info/RECORD
-12 files, 293302 bytes uncompressed, 72301 bytes compressed:  75.3%
+-rw-rw-rw-  2.0 fat     6123 b- defN 23-Jul-05 15:31 tdfs4ds-0.1.0.1.dist-info/METADATA
+-rw-rw-rw-  2.0 fat       92 b- defN 23-Jul-05 15:31 tdfs4ds-0.1.0.1.dist-info/WHEEL
+-rw-rw-rw-  2.0 fat        8 b- defN 23-Jul-05 15:31 tdfs4ds-0.1.0.1.dist-info/top_level.txt
+?rw-rw-r--  2.0 fat      919 b- defN 23-Jul-05 15:31 tdfs4ds-0.1.0.1.dist-info/RECORD
+12 files, 296767 bytes uncompressed, 73469 bytes compressed:  75.2%
```

## zipnote {}

```diff
@@ -18,20 +18,20 @@
 
 Filename: tdfs4ds/feature_store.py
 Comment: 
 
 Filename: tdfs4ds/data/curves.csv
 Comment: 
 
-Filename: tdfs4ds-0.1.0.0.dist-info/METADATA
+Filename: tdfs4ds-0.1.0.1.dist-info/METADATA
 Comment: 
 
-Filename: tdfs4ds-0.1.0.0.dist-info/WHEEL
+Filename: tdfs4ds-0.1.0.1.dist-info/WHEEL
 Comment: 
 
-Filename: tdfs4ds-0.1.0.0.dist-info/top_level.txt
+Filename: tdfs4ds-0.1.0.1.dist-info/top_level.txt
 Comment: 
 
-Filename: tdfs4ds-0.1.0.0.dist-info/RECORD
+Filename: tdfs4ds-0.1.0.1.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## tdfs4ds/__init__.py

```diff
@@ -1 +1 @@
-__version__ = '0.1.0.0'
+__version__ = '0.1.0.1'
```

## Comparing `tdfs4ds-0.1.0.0.dist-info/RECORD` & `tdfs4ds-0.1.0.1.dist-info/RECORD`

 * *Files 19% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 tdfs/__init__.py,sha256=7AcO7uB1opRCt7t2JOHworKimfAaDeO3boRW7u9Geo8,23
 tdfs/datasets.py,sha256=-b2MPEKGki2V1M8iUcoDR9uc2krIK7u1CK-EhChvihs,985
 tdfs/feature_store.py,sha256=Honu7eOAXxP4Ivz0mRlhuNkfTDzgZl5HB1WlQUwzcZ0,31354
 tdfs/data/curves.csv,sha256=q0Tm-0yu7VMK4lHvHpgi1LMeRq0lO5gJy2Q17brKbEM,112488
-tdfs4ds/__init__.py,sha256=7AcO7uB1opRCt7t2JOHworKimfAaDeO3boRW7u9Geo8,23
+tdfs4ds/__init__.py,sha256=GEfqHS5GHX-bao3eAwULQOT5hzwVghHcXNcGCwwAIdg,23
 tdfs4ds/datasets.py,sha256=-b2MPEKGki2V1M8iUcoDR9uc2krIK7u1CK-EhChvihs,985
 tdfs4ds/feature_store.py,sha256=EZLozx7UXOodzioukF1K1GxvSxe2BYvmxQwy8j3IP20,31279
 tdfs4ds/data/curves.csv,sha256=q0Tm-0yu7VMK4lHvHpgi1LMeRq0lO5gJy2Q17brKbEM,112488
-tdfs4ds-0.1.0.0.dist-info/METADATA,sha256=efOAEz5FSeGOu3uTH2-pcNZx7-eraoQlXAdHufoUzoo,2658
-tdfs4ds-0.1.0.0.dist-info/WHEEL,sha256=G16H4A3IeoQmnOrYV4ueZGKSjhipXx8zc8nu9FGlvMA,92
-tdfs4ds-0.1.0.0.dist-info/top_level.txt,sha256=wMyVkMvnBn8RRt1xBveGQxOpWFijPMPkMiE7G2mi8zo,8
-tdfs4ds-0.1.0.0.dist-info/RECORD,,
+tdfs4ds-0.1.0.1.dist-info/METADATA,sha256=yb7NEd8cLRRNKGjUgzYqBCIUPTNbJVrazUtgJkP-RKU,6123
+tdfs4ds-0.1.0.1.dist-info/WHEEL,sha256=G16H4A3IeoQmnOrYV4ueZGKSjhipXx8zc8nu9FGlvMA,92
+tdfs4ds-0.1.0.1.dist-info/top_level.txt,sha256=wMyVkMvnBn8RRt1xBveGQxOpWFijPMPkMiE7G2mi8zo,8
+tdfs4ds-0.1.0.1.dist-info/RECORD,,
```

