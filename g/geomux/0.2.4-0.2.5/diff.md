# Comparing `tmp/geomux-0.2.4.tar.gz` & `tmp/geomux-0.2.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "geomux-0.2.4.tar", last modified: Fri Jun 30 23:52:46 2023, max compression
+gzip compressed data, was "geomux-0.2.5.tar", last modified: Wed Jul  5 20:26:47 2023, max compression
```

## Comparing `geomux-0.2.4.tar` & `geomux-0.2.5.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 noam      (1000) noam      (1000)        0 2023-06-30 23:52:46.827882 geomux-0.2.4/
--rw-r--r--   0 noam      (1000) noam      (1000)     3548 2023-06-30 23:52:46.827882 geomux-0.2.4/PKG-INFO
--rw-r--r--   0 noam      (1000) noam      (1000)     3282 2023-06-30 23:52:39.000000 geomux-0.2.4/README.md
-drwxr-xr-x   0 noam      (1000) noam      (1000)        0 2023-06-30 23:52:46.824548 geomux-0.2.4/geomux/
--rw-r--r--   0 noam      (1000) noam      (1000)       71 2023-06-23 19:19:47.000000 geomux-0.2.4/geomux/__init__.py
--rw-r--r--   0 noam      (1000) noam      (1000)     2482 2023-06-30 23:52:39.000000 geomux-0.2.4/geomux/__main__.py
--rw-r--r--   0 noam      (1000) noam      (1000)     9419 2023-06-30 23:52:39.000000 geomux-0.2.4/geomux/geomux.py
--rw-r--r--   0 noam      (1000) noam      (1000)     1005 2023-06-28 20:47:48.000000 geomux-0.2.4/geomux/utils.py
-drwxr-xr-x   0 noam      (1000) noam      (1000)        0 2023-06-30 23:52:46.827882 geomux-0.2.4/geomux.egg-info/
--rw-r--r--   0 noam      (1000) noam      (1000)     3548 2023-06-30 23:52:46.000000 geomux-0.2.4/geomux.egg-info/PKG-INFO
--rw-r--r--   0 noam      (1000) noam      (1000)      309 2023-06-30 23:52:46.000000 geomux-0.2.4/geomux.egg-info/SOURCES.txt
--rw-r--r--   0 noam      (1000) noam      (1000)        1 2023-06-30 23:52:46.000000 geomux-0.2.4/geomux.egg-info/dependency_links.txt
--rw-r--r--   0 noam      (1000) noam      (1000)       52 2023-06-30 23:52:46.000000 geomux-0.2.4/geomux.egg-info/entry_points.txt
--rw-r--r--   0 noam      (1000) noam      (1000)       36 2023-06-30 23:52:46.000000 geomux-0.2.4/geomux.egg-info/requires.txt
--rw-r--r--   0 noam      (1000) noam      (1000)        7 2023-06-30 23:52:46.000000 geomux-0.2.4/geomux.egg-info/top_level.txt
--rw-r--r--   0 noam      (1000) noam      (1000)       38 2023-06-30 23:52:46.827882 geomux-0.2.4/setup.cfg
--rw-r--r--   0 noam      (1000) noam      (1000)      658 2023-06-30 23:52:39.000000 geomux-0.2.4/setup.py
-drwxr-xr-x   0 noam      (1000) noam      (1000)        0 2023-06-30 23:52:46.827882 geomux-0.2.4/tests/
--rw-r--r--   0 noam      (1000) noam      (1000)     3160 2023-06-30 23:52:39.000000 geomux-0.2.4/tests/test_geomux.py
--rw-r--r--   0 noam      (1000) noam      (1000)     1110 2023-06-28 20:47:48.000000 geomux-0.2.4/tests/test_io.py
+drwxr-xr-x   0 noam      (1000) noam      (1000)        0 2023-07-05 20:26:47.535847 geomux-0.2.5/
+-rw-r--r--   0 noam      (1000) noam      (1000)     3548 2023-07-05 20:26:47.535847 geomux-0.2.5/PKG-INFO
+-rw-r--r--   0 noam      (1000) noam      (1000)     3282 2023-06-30 23:52:39.000000 geomux-0.2.5/README.md
+drwxr-xr-x   0 noam      (1000) noam      (1000)        0 2023-07-05 20:26:47.535847 geomux-0.2.5/geomux/
+-rw-r--r--   0 noam      (1000) noam      (1000)       71 2023-06-23 19:19:47.000000 geomux-0.2.5/geomux/__init__.py
+-rw-r--r--   0 noam      (1000) noam      (1000)     2482 2023-06-30 23:52:39.000000 geomux-0.2.5/geomux/__main__.py
+-rw-r--r--   0 noam      (1000) noam      (1000)    10177 2023-07-05 20:26:30.000000 geomux-0.2.5/geomux/geomux.py
+-rw-r--r--   0 noam      (1000) noam      (1000)     1005 2023-06-28 20:47:48.000000 geomux-0.2.5/geomux/utils.py
+drwxr-xr-x   0 noam      (1000) noam      (1000)        0 2023-07-05 20:26:47.535847 geomux-0.2.5/geomux.egg-info/
+-rw-r--r--   0 noam      (1000) noam      (1000)     3548 2023-07-05 20:26:47.000000 geomux-0.2.5/geomux.egg-info/PKG-INFO
+-rw-r--r--   0 noam      (1000) noam      (1000)      309 2023-07-05 20:26:47.000000 geomux-0.2.5/geomux.egg-info/SOURCES.txt
+-rw-r--r--   0 noam      (1000) noam      (1000)        1 2023-07-05 20:26:47.000000 geomux-0.2.5/geomux.egg-info/dependency_links.txt
+-rw-r--r--   0 noam      (1000) noam      (1000)       52 2023-07-05 20:26:47.000000 geomux-0.2.5/geomux.egg-info/entry_points.txt
+-rw-r--r--   0 noam      (1000) noam      (1000)       36 2023-07-05 20:26:47.000000 geomux-0.2.5/geomux.egg-info/requires.txt
+-rw-r--r--   0 noam      (1000) noam      (1000)        7 2023-07-05 20:26:47.000000 geomux-0.2.5/geomux.egg-info/top_level.txt
+-rw-r--r--   0 noam      (1000) noam      (1000)       38 2023-07-05 20:26:47.535847 geomux-0.2.5/setup.cfg
+-rw-r--r--   0 noam      (1000) noam      (1000)      658 2023-07-05 20:26:30.000000 geomux-0.2.5/setup.py
+drwxr-xr-x   0 noam      (1000) noam      (1000)        0 2023-07-05 20:26:47.535847 geomux-0.2.5/tests/
+-rw-r--r--   0 noam      (1000) noam      (1000)     3160 2023-06-30 23:52:39.000000 geomux-0.2.5/tests/test_geomux.py
+-rw-r--r--   0 noam      (1000) noam      (1000)     1110 2023-06-28 20:47:48.000000 geomux-0.2.5/tests/test_io.py
```

### Comparing `geomux-0.2.4/PKG-INFO` & `geomux-0.2.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: geomux
-Version: 0.2.4
+Version: 0.2.5
 Summary: a tool to assign an identity to a table of barcode guides
 Home-page: https://github.com/noamteyssier/geomux
 Author: Noam Teysser
 Author-email: Noam.Teyssier@ucsf.edu
 Description-Content-Type: text/markdown
 
 # geomux
```

### Comparing `geomux-0.2.4/README.md` & `geomux-0.2.5/README.md`

 * *Files identical despite different names*

### Comparing `geomux-0.2.4/geomux/__main__.py` & `geomux-0.2.5/geomux/__main__.py`

 * *Files identical despite different names*

### Comparing `geomux-0.2.4/geomux/geomux.py` & `geomux-0.2.5/geomux/geomux.py`

 * *Files 6% similar despite different names*

```diff
@@ -217,14 +217,22 @@
             AttributeError("Please run `.test()` method first")
         guide_indices = np.arange(self._m_total)
         guide_mask = guide_indices[self.passing_guides]
         self.labels = [
             self.guide_names[guide_mask[np.flatnonzero(self.pv_mat[i] < threshold)]]
             for i in np.arange(self._n_cells)
         ]
+        self.counts = [
+            self.matrix[i][np.flatnonzero(self.pv_mat[i] < threshold)]
+            for i in np.arange(self._n_cells)
+        ]
+        self.pvalues = [
+            self.pv_mat[i][np.flatnonzero(self.pv_mat[i] < threshold)]
+            for i in np.arange(self._n_cells)
+        ]
         return self.labels
 
     def _calc_moi(self, threshold=0.05):
         """
         Classify each cell between single, double, or null assignments
         """
         if not self.is_fit:
@@ -238,34 +246,46 @@
         """
         cell_id_in = np.arange(self._n_total)[self.passing_cells]
         cell_id_out = np.arange(self._n_total)[~self.passing_cells]
 
         cell_name_in = self.cell_names[self.passing_cells]
         cell_name_out = self.cell_names[~self.passing_cells]
 
+        self._calc_assignments(threshold)
+
         frame = pd.DataFrame(
             {
                 "cell_id": cell_name_in,
-                "assignment": self._calc_assignments(threshold),
+                "assignment": self.labels,
+                "counts": self.counts,
+                "pvalues": self.pvalues,
                 "moi": self._calc_moi(threshold),
                 "n_umi": self.draws,
-                "p_value": self.pv_mat.min(axis=1),
+                "min_pvalue": self.pv_mat.min(axis=1),
+                "max_count": self.matrix.max(axis=1),
                 "log_odds": self.log_odds,
                 "tested": True,
             },
             index=cell_id_in,
         )
         null = pd.DataFrame(
             {
                 "cell_id": cell_name_out,
                 "assignment": [
                     np.array([]) for _ in np.arange(np.sum(~self.passing_cells))
                 ],
+                "counts": [
+                    np.array([]) for _ in np.arange(np.sum(~self.passing_cells))
+                ],
+                "pvalues": [
+                    np.array([]) for _ in np.arange(np.sum(~self.passing_cells))
+                ],
                 "moi": np.nan,
                 "n_umi": np.nan,
-                "p_value": np.nan,
+                "min_pvalue": np.nan,
+                "max_count": np.nan,
                 "log_odds": np.nan,
                 "tested": False,
             },
             index=cell_id_out,
         )
         return pd.concat([frame, null]).sort_index()
```

### Comparing `geomux-0.2.4/geomux/utils.py` & `geomux-0.2.5/geomux/utils.py`

 * *Files identical despite different names*

### Comparing `geomux-0.2.4/geomux.egg-info/PKG-INFO` & `geomux-0.2.5/geomux.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: geomux
-Version: 0.2.4
+Version: 0.2.5
 Summary: a tool to assign an identity to a table of barcode guides
 Home-page: https://github.com/noamteyssier/geomux
 Author: Noam Teysser
 Author-email: Noam.Teyssier@ucsf.edu
 Description-Content-Type: text/markdown
 
 # geomux
```

### Comparing `geomux-0.2.4/setup.py` & `geomux-0.2.5/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setup(
     name="geomux",
-    version="0.2.4",
+    version="0.2.5",
     author="Noam Teysser",
     author_email="Noam.Teyssier@ucsf.edu",
     packages=["geomux"],
     description="a tool to assign an identity to a table of barcode guides",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/noamteyssier/geomux",
```

### Comparing `geomux-0.2.4/tests/test_geomux.py` & `geomux-0.2.5/tests/test_geomux.py`

 * *Files identical despite different names*

### Comparing `geomux-0.2.4/tests/test_io.py` & `geomux-0.2.5/tests/test_io.py`

 * *Files identical despite different names*

