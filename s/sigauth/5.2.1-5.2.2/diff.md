# Comparing `tmp/sigauth-5.2.1-py3-none-any.whl.zip` & `tmp/sigauth-5.2.2-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,11 +1,11 @@
-Zip file size: 6885 bytes, number of entries: 9
--rw-r--r--  2.0 unx        0 b- defN 23-Jun-09 12:50 sigauth/__init__.py
--rw-r--r--  2.0 unx     5854 b- defN 23-Jun-09 12:50 sigauth/helpers.py
--rw-r--r--  2.0 unx      915 b- defN 23-Jun-09 12:50 sigauth/middleware.py
--rw-r--r--  2.0 unx      487 b- defN 23-Jun-09 12:50 sigauth/permissions.py
--rw-r--r--  2.0 unx     1091 b- defN 23-Jun-09 12:50 sigauth-5.2.1.dist-info/LICENSE
--rw-r--r--  2.0 unx     6584 b- defN 23-Jun-09 12:50 sigauth-5.2.1.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 23-Jun-09 12:50 sigauth-5.2.1.dist-info/WHEEL
--rw-r--r--  2.0 unx        8 b- defN 23-Jun-09 12:50 sigauth-5.2.1.dist-info/top_level.txt
--rw-rw-r--  2.0 unx      688 b- defN 23-Jun-09 12:50 sigauth-5.2.1.dist-info/RECORD
-9 files, 15719 bytes uncompressed, 5701 bytes compressed:  63.7%
+Zip file size: 6889 bytes, number of entries: 9
+-rw-r--r--  2.0 unx        0 b- defN 23-Jul-05 15:42 sigauth/__init__.py
+-rw-r--r--  2.0 unx     5854 b- defN 23-Jul-05 15:42 sigauth/helpers.py
+-rw-r--r--  2.0 unx      915 b- defN 23-Jul-05 15:42 sigauth/middleware.py
+-rw-r--r--  2.0 unx      487 b- defN 23-Jul-05 15:42 sigauth/permissions.py
+-rw-r--r--  2.0 unx     1091 b- defN 23-Jul-05 15:42 sigauth-5.2.2.dist-info/LICENSE
+-rw-r--r--  2.0 unx     6625 b- defN 23-Jul-05 15:42 sigauth-5.2.2.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 23-Jul-05 15:42 sigauth-5.2.2.dist-info/WHEEL
+-rw-r--r--  2.0 unx        8 b- defN 23-Jul-05 15:42 sigauth-5.2.2.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx      688 b- defN 23-Jul-05 15:42 sigauth-5.2.2.dist-info/RECORD
+9 files, 15760 bytes uncompressed, 5705 bytes compressed:  63.8%
```

## zipnote {}

```diff
@@ -6,23 +6,23 @@
 
 Filename: sigauth/middleware.py
 Comment: 
 
 Filename: sigauth/permissions.py
 Comment: 
 
-Filename: sigauth-5.2.1.dist-info/LICENSE
+Filename: sigauth-5.2.2.dist-info/LICENSE
 Comment: 
 
-Filename: sigauth-5.2.1.dist-info/METADATA
+Filename: sigauth-5.2.2.dist-info/METADATA
 Comment: 
 
-Filename: sigauth-5.2.1.dist-info/WHEEL
+Filename: sigauth-5.2.2.dist-info/WHEEL
 Comment: 
 
-Filename: sigauth-5.2.1.dist-info/top_level.txt
+Filename: sigauth-5.2.2.dist-info/top_level.txt
 Comment: 
 
-Filename: sigauth-5.2.1.dist-info/RECORD
+Filename: sigauth-5.2.2.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## Comparing `sigauth-5.2.1.dist-info/LICENSE` & `sigauth-5.2.2.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `sigauth-5.2.1.dist-info/METADATA` & `sigauth-5.2.2.dist-info/METADATA`

 * *Files 2% similar despite different names*

```diff
@@ -1,36 +1,37 @@
 Metadata-Version: 2.1
 Name: sigauth
-Version: 5.2.1
+Version: 5.2.2
 Summary: Signature authentication library for Export Directory.
 Home-page: https://github.com/uktrade/directory-signature-auth
 Author: Department for International Trade
 License: MIT
 Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Web Environment
 Classifier: Framework :: Django
 Classifier: Framework :: Django :: 1.11
 Classifier: Framework :: Django :: 2.0
 Classifier: Framework :: Django :: 2.1
 Classifier: Framework :: Django :: 2.2
 Classifier: Framework :: Django :: 3.1
 Classifier: Framework :: Django :: 4.1
+Classifier: Framework :: Django :: 4.2
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Natural Language :: English
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3.5
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: Implementation :: PyPy
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Description-Content-Type: text/markdown
 License-File: LICENSE
-Requires-Dist: django (<=4.2,>=3.2.19)
+Requires-Dist: django (<=4.2.3,>=3.2.19)
 Requires-Dist: djangorestframework (<4.0.0,>=3.4.7)
 Requires-Dist: mohawk (<2.0.0,>=0.3.4)
 Provides-Extra: test
 Requires-Dist: pytest (==7.*) ; extra == 'test'
 Requires-Dist: pytest-cov (==4.*) ; extra == 'test'
 Requires-Dist: pytest-django (==4.*) ; extra == 'test'
 Requires-Dist: flake8 ; extra == 'test'
```

## Comparing `sigauth-5.2.1.dist-info/RECORD` & `sigauth-5.2.2.dist-info/RECORD`

 * *Files 8% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 sigauth/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 sigauth/helpers.py,sha256=rUwnTTfkuonFY-FXSZu4_V9QQcsRhWMBBL8_6u_K0u8,5854
 sigauth/middleware.py,sha256=FopB3wvZaGxR6kF8B7TKC_tY_35AG0asgmdGGft95LQ,915
 sigauth/permissions.py,sha256=c-fTj1sL2xeBeOqV1yQcBbfdton_PeFsM3CYgFdA9OE,487
-sigauth-5.2.1.dist-info/LICENSE,sha256=y-ArErAQz98OorLek2xntwEp9bo3ZcqfQMtAIcjBdvQ,1091
-sigauth-5.2.1.dist-info/METADATA,sha256=6wDnWe2tqvpLNs1HsX4dxNs0y6596Qn_CBgR3a6qC5w,6584
-sigauth-5.2.1.dist-info/WHEEL,sha256=pkctZYzUS4AYVn6dJ-7367OJZivF2e8RA9b_ZBjif18,92
-sigauth-5.2.1.dist-info/top_level.txt,sha256=mGlNBeKJK-HbIfvTKK_jrdMOtW4K3QcZNoGYTRSzhUc,8
-sigauth-5.2.1.dist-info/RECORD,,
+sigauth-5.2.2.dist-info/LICENSE,sha256=y-ArErAQz98OorLek2xntwEp9bo3ZcqfQMtAIcjBdvQ,1091
+sigauth-5.2.2.dist-info/METADATA,sha256=IySBFxfwC4kRnPvJQ0eIeil1PslWT4umsX4zo1a16LE,6625
+sigauth-5.2.2.dist-info/WHEEL,sha256=pkctZYzUS4AYVn6dJ-7367OJZivF2e8RA9b_ZBjif18,92
+sigauth-5.2.2.dist-info/top_level.txt,sha256=mGlNBeKJK-HbIfvTKK_jrdMOtW4K3QcZNoGYTRSzhUc,8
+sigauth-5.2.2.dist-info/RECORD,,
```

