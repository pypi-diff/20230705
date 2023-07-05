# Comparing `tmp/diveplane_amalgam_api-2.3.7-py3-none-any.whl.zip` & `tmp/diveplane_amalgam_api-2.3.9-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,9 +1,9 @@
-Zip file size: 12611 bytes, number of entries: 7
--rw-r--r--  2.0 unx      224 b- defN 23-Jun-07 16:07 amalgam/__init__.py
--rw-r--r--  2.0 unx    26758 b- defN 23-Jun-07 16:06 amalgam/api.py
--rw-r--r--  2.0 unx    12104 b- defN 23-Jun-07 16:07 diveplane_amalgam_api-2.3.7.dist-info/LICENSE.txt
--rw-r--r--  2.0 unx      571 b- defN 23-Jun-07 16:07 diveplane_amalgam_api-2.3.7.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 23-Jun-07 16:07 diveplane_amalgam_api-2.3.7.dist-info/WHEEL
--rw-r--r--  2.0 unx        8 b- defN 23-Jun-07 16:07 diveplane_amalgam_api-2.3.7.dist-info/top_level.txt
--rw-rw-r--  2.0 unx      606 b- defN 23-Jun-07 16:07 diveplane_amalgam_api-2.3.7.dist-info/RECORD
-7 files, 40363 bytes uncompressed, 11525 bytes compressed:  71.4%
+Zip file size: 13573 bytes, number of entries: 7
+-rw-r--r--  2.0 unx      224 b- defN 23-Jul-04 18:19 amalgam/__init__.py
+-rw-r--r--  2.0 unx    26758 b- defN 23-Jul-04 18:19 amalgam/api.py
+-rw-r--r--  2.0 unx    12104 b- defN 23-Jul-04 18:19 diveplane_amalgam_api-2.3.9.dist-info/LICENSE.txt
+-rw-r--r--  2.0 unx     2885 b- defN 23-Jul-04 18:19 diveplane_amalgam_api-2.3.9.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 23-Jul-04 18:19 diveplane_amalgam_api-2.3.9.dist-info/WHEEL
+-rw-r--r--  2.0 unx        8 b- defN 23-Jul-04 18:19 diveplane_amalgam_api-2.3.9.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx      607 b- defN 23-Jul-04 18:19 diveplane_amalgam_api-2.3.9.dist-info/RECORD
+7 files, 42678 bytes uncompressed, 12487 bytes compressed:  70.7%
```

## zipnote {}

```diff
@@ -1,22 +1,22 @@
 Filename: amalgam/__init__.py
 Comment: 
 
 Filename: amalgam/api.py
 Comment: 
 
-Filename: diveplane_amalgam_api-2.3.7.dist-info/LICENSE.txt
+Filename: diveplane_amalgam_api-2.3.9.dist-info/LICENSE.txt
 Comment: 
 
-Filename: diveplane_amalgam_api-2.3.7.dist-info/METADATA
+Filename: diveplane_amalgam_api-2.3.9.dist-info/METADATA
 Comment: 
 
-Filename: diveplane_amalgam_api-2.3.7.dist-info/WHEEL
+Filename: diveplane_amalgam_api-2.3.9.dist-info/WHEEL
 Comment: 
 
-Filename: diveplane_amalgam_api-2.3.7.dist-info/top_level.txt
+Filename: diveplane_amalgam_api-2.3.9.dist-info/top_level.txt
 Comment: 
 
-Filename: diveplane_amalgam_api-2.3.7.dist-info/RECORD
+Filename: diveplane_amalgam_api-2.3.9.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## amalgam/__init__.py

```diff
@@ -3,8 +3,8 @@
 
 """
 The version number is automatically incremented by the pipeline
 It should not be manually changed.
 To change the major/minor number change the number in azure-pipelines.yml
 """
 
-__version__ = "2.3.7"
+__version__ = "2.3.9"
```

## Comparing `diveplane_amalgam_api-2.3.7.dist-info/LICENSE.txt` & `diveplane_amalgam_api-2.3.9.dist-info/LICENSE.txt`

 * *Files identical despite different names*

## Comparing `diveplane_amalgam_api-2.3.7.dist-info/RECORD` & `diveplane_amalgam_api-2.3.9.dist-info/RECORD`

 * *Files 26% similar despite different names*

```diff
@@ -1,7 +1,7 @@
-amalgam/__init__.py,sha256=VhQ7nnILExf38-sEN1dn5U_d0MhoKHe99EOdB9A_U0g,224
+amalgam/__init__.py,sha256=m6Qzzz9eRuUAOpbyVRe1F_oMZ-6Ysjku1KxnaHSkGi0,224
 amalgam/api.py,sha256=XL7tnGSbyDknjkGP2mslyhfNy-lM_PwyiZCpHNSnWTI,26758
-diveplane_amalgam_api-2.3.7.dist-info/LICENSE.txt,sha256=4UTGY81GVApDEB2E0QKXiQuyEUVTWXJvrR46vpD9oNM,12104
-diveplane_amalgam_api-2.3.7.dist-info/METADATA,sha256=zQY4fEBF7lT6LKlF-OiTG8F3g2gdA6kDrT2z937mcYY,571
-diveplane_amalgam_api-2.3.7.dist-info/WHEEL,sha256=pkctZYzUS4AYVn6dJ-7367OJZivF2e8RA9b_ZBjif18,92
-diveplane_amalgam_api-2.3.7.dist-info/top_level.txt,sha256=rmPHU144SyaB25u5-FAQyECAQnJ39NvuJEcKXMRcdBo,8
-diveplane_amalgam_api-2.3.7.dist-info/RECORD,,
+diveplane_amalgam_api-2.3.9.dist-info/LICENSE.txt,sha256=4UTGY81GVApDEB2E0QKXiQuyEUVTWXJvrR46vpD9oNM,12104
+diveplane_amalgam_api-2.3.9.dist-info/METADATA,sha256=Y8GhyzunWsJXT-TRJs-50CNSNXh_ooCuyD9PXf2j3EI,2885
+diveplane_amalgam_api-2.3.9.dist-info/WHEEL,sha256=pkctZYzUS4AYVn6dJ-7367OJZivF2e8RA9b_ZBjif18,92
+diveplane_amalgam_api-2.3.9.dist-info/top_level.txt,sha256=rmPHU144SyaB25u5-FAQyECAQnJ39NvuJEcKXMRcdBo,8
+diveplane_amalgam_api-2.3.9.dist-info/RECORD,,
```

