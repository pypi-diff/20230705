# Comparing `tmp/pangolier-0.1.1-py3-none-any.whl.zip` & `tmp/pangolier-0.1.2-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,12 +1,12 @@
-Zip file size: 5170 bytes, number of entries: 10
+Zip file size: 5175 bytes, number of entries: 10
 -rw-rw-r--  2.0 unx        0 b- defN 22-Aug-07 02:48 pangolier/__init__.py
 -rw-rw-r--  2.0 unx      336 b- defN 23-Jun-12 03:36 pangolier/common.py
--rw-rw-r--  2.0 unx      593 b- defN 22-Aug-06 08:53 pangolier/filters.py
+-rw-rw-r--  2.0 unx      707 b- defN 23-Jul-05 09:20 pangolier/filters.py
 -rw-rw-r--  2.0 unx     2930 b- defN 23-Jan-16 03:51 pangolier/functions.py
 -rw-rw-r--  2.0 unx     3153 b- defN 23-Jun-12 03:36 pangolier/metrics.py
 -rw-rw-r--  2.0 unx     1121 b- defN 22-Aug-08 12:44 pangolier/prefixes.py
--rw-rw-r--  2.0 unx     3701 b- defN 23-Jun-12 03:36 pangolier-0.1.1.dist-info/METADATA
--rw-rw-r--  2.0 unx       92 b- defN 23-Jun-12 03:36 pangolier-0.1.1.dist-info/WHEEL
--rw-rw-r--  2.0 unx       10 b- defN 23-Jun-12 03:36 pangolier-0.1.1.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx      766 b- defN 23-Jun-12 03:36 pangolier-0.1.1.dist-info/RECORD
-10 files, 12702 bytes uncompressed, 3870 bytes compressed:  69.5%
+-rw-rw-r--  2.0 unx     3701 b- defN 23-Jul-05 09:21 pangolier-0.1.2.dist-info/METADATA
+-rw-rw-r--  2.0 unx       92 b- defN 23-Jul-05 09:21 pangolier-0.1.2.dist-info/WHEEL
+-rw-rw-r--  2.0 unx       10 b- defN 23-Jul-05 09:21 pangolier-0.1.2.dist-info/top_level.txt
+?rw-rw-r--  2.0 unx      766 b- defN 23-Jul-05 09:21 pangolier-0.1.2.dist-info/RECORD
+10 files, 12816 bytes uncompressed, 3875 bytes compressed:  69.8%
```

## zipnote {}

```diff
@@ -12,20 +12,20 @@
 
 Filename: pangolier/metrics.py
 Comment: 
 
 Filename: pangolier/prefixes.py
 Comment: 
 
-Filename: pangolier-0.1.1.dist-info/METADATA
+Filename: pangolier-0.1.2.dist-info/METADATA
 Comment: 
 
-Filename: pangolier-0.1.1.dist-info/WHEEL
+Filename: pangolier-0.1.2.dist-info/WHEEL
 Comment: 
 
-Filename: pangolier-0.1.1.dist-info/top_level.txt
+Filename: pangolier-0.1.2.dist-info/top_level.txt
 Comment: 
 
-Filename: pangolier-0.1.1.dist-info/RECORD
+Filename: pangolier-0.1.2.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## pangolier/filters.py

```diff
@@ -7,14 +7,19 @@
 
 
 class EqualFilter(FilterBase):
     def to_str(self, pretty=False):
         return '="%s"' % self.expression
 
 
+class NotEqualFilter(FilterBase):
+    def to_str(self, pretty=False):
+        return '!="%s"' % self.expression
+
+
 class RegexpFilter(FilterBase):
     def to_str(self, pretty=False):
         return '=~"%s"' % self.expression
 
 
 def _make_filter(value):
     if isinstance(value, str):
```

## Comparing `pangolier-0.1.1.dist-info/METADATA` & `pangolier-0.1.2.dist-info/METADATA`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pangolier
-Version: 0.1.1
+Version: 0.1.2
 Summary: prometheus query builder
 Home-page: https://github.com/lexdene/pangolier
 Requires-Python: >3.10.0
 Description-Content-Type: text/markdown
 
 # Pangolier
```

## Comparing `pangolier-0.1.1.dist-info/RECORD` & `pangolier-0.1.2.dist-info/RECORD`

 * *Files 13% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 pangolier/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 pangolier/common.py,sha256=6CiIILgtgsnSlYkreEOirY1Ox85e_iNBUqTnAmawxgM,336
-pangolier/filters.py,sha256=0rEzH9BsJ_Lka9JcnNLNK9-52V9G7NQ2DCKWXaKxvjM,593
+pangolier/filters.py,sha256=i5H3myifUoQWFHvnQhAb-dTLJf3AFbrsg5dtQR5uOCA,707
 pangolier/functions.py,sha256=wLnItRKEoCT5tnKX0ZgIbl6gPGB-_qosCz4v0qba8fI,2930
 pangolier/metrics.py,sha256=D47ly81aVF1jEKZPFtzhdP_Dyg7Ukh18QqvfCztwBzw,3153
 pangolier/prefixes.py,sha256=5lgLpoRUF2oP3eT5BEzWyOOxTb_dGdl6LR8YBvtWKtU,1121
-pangolier-0.1.1.dist-info/METADATA,sha256=VmNmmuHAaCvDcjRezF3mMxLIJ0k6DCqfBToTHYH0BQ4,3701
-pangolier-0.1.1.dist-info/WHEEL,sha256=2wepM1nk4DS4eFpYrW1TTqPcoGNfHhhO_i5m4cOimbo,92
-pangolier-0.1.1.dist-info/top_level.txt,sha256=oVjXI9K4K47ZzdvnhAwezlDWfgBGevyp1bX99_TSZlk,10
-pangolier-0.1.1.dist-info/RECORD,,
+pangolier-0.1.2.dist-info/METADATA,sha256=tu_KDa5D39W2fUi-4HD4dkwHY8Lt_DQ09S6Nr36SeSE,3701
+pangolier-0.1.2.dist-info/WHEEL,sha256=2wepM1nk4DS4eFpYrW1TTqPcoGNfHhhO_i5m4cOimbo,92
+pangolier-0.1.2.dist-info/top_level.txt,sha256=oVjXI9K4K47ZzdvnhAwezlDWfgBGevyp1bX99_TSZlk,10
+pangolier-0.1.2.dist-info/RECORD,,
```

