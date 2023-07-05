# Comparing `tmp/geoinsight-0.5.3.tar.gz` & `tmp/geoinsight-0.5.4.tar.gz`

## Comparing `geoinsight-0.5.3.tar` & `geoinsight-0.5.4.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rw-r--r--   0        0        0       43 2020-02-02 00:00:00.000000 geoinsight-0.5.3/geoinsight/src/__init__.py
--rw-r--r--   0        0        0    75207 2020-02-02 00:00:00.000000 geoinsight-0.5.3/geoinsight/src/api.py
--rw-r--r--   0        0        0     2176 2020-02-02 00:00:00.000000 geoinsight-0.5.3/geoinsight/src/geoinsight.py
--rw-r--r--   0        0        0     4999 2020-02-02 00:00:00.000000 geoinsight-0.5.3/geoinsight/src/util.py
--rw-r--r--   0        0        0      584 2020-02-02 00:00:00.000000 geoinsight-0.5.3/.gitignore
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 geoinsight-0.5.3/LICENSE
--rw-r--r--   0        0        0      771 2020-02-02 00:00:00.000000 geoinsight-0.5.3/README.md
--rw-r--r--   0        0        0      453 2020-02-02 00:00:00.000000 geoinsight-0.5.3/pyproject.toml
--rw-r--r--   0        0        0     1138 2020-02-02 00:00:00.000000 geoinsight-0.5.3/PKG-INFO
+-rw-r--r--   0        0        0       43 2020-02-02 00:00:00.000000 geoinsight-0.5.4/geoinsight/src/__init__.py
+-rw-r--r--   0        0        0    75207 2020-02-02 00:00:00.000000 geoinsight-0.5.4/geoinsight/src/api.py
+-rw-r--r--   0        0        0     2176 2020-02-02 00:00:00.000000 geoinsight-0.5.4/geoinsight/src/geoinsight.py
+-rw-r--r--   0        0        0     4999 2020-02-02 00:00:00.000000 geoinsight-0.5.4/geoinsight/src/util.py
+-rw-r--r--   0        0        0      593 2020-02-02 00:00:00.000000 geoinsight-0.5.4/.gitignore
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 geoinsight-0.5.4/LICENSE
+-rw-r--r--   0        0        0      771 2020-02-02 00:00:00.000000 geoinsight-0.5.4/README.md
+-rw-r--r--   0        0        0      453 2020-02-02 00:00:00.000000 geoinsight-0.5.4/pyproject.toml
+-rw-r--r--   0        0        0     1138 2020-02-02 00:00:00.000000 geoinsight-0.5.4/PKG-INFO
```

### Comparing `geoinsight-0.5.3/geoinsight/src/api.py` & `geoinsight-0.5.4/geoinsight/src/api.py`

 * *Files identical despite different names*

### Comparing `geoinsight-0.5.3/geoinsight/src/geoinsight.py` & `geoinsight-0.5.4/geoinsight/src/geoinsight.py`

 * *Files identical despite different names*

### Comparing `geoinsight-0.5.3/geoinsight/src/util.py` & `geoinsight-0.5.4/geoinsight/src/util.py`

 * *Files identical despite different names*

### Comparing `geoinsight-0.5.3/.gitignore` & `geoinsight-0.5.4/.gitignore`

 * *Files 2% similar despite different names*

```diff
@@ -29,7 +29,8 @@
 scratch.sql
 /public/python/dist
 /public/python/build
 /public/python/geoinsight/src/geoinsight.egg-info
 /core/notebooks/jupyterlab/.[a-zA-Z_]*
 run.sql
 /certs/
+/backup/
```

### Comparing `geoinsight-0.5.3/README.md` & `geoinsight-0.5.4/README.md`

 * *Files identical despite different names*

### Comparing `geoinsight-0.5.3/PKG-INFO` & `geoinsight-0.5.4/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: geoinsight
-Version: 0.5.3
+Version: 0.5.4
 Summary: GeoInsight python package
 Author-email: GeoInsight <info@geoinsight.ai>
 License-File: LICENSE
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.6
```

