# Comparing `tmp/mlforecast-0.7.3.tar.gz` & `tmp/mlforecast-0.7.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mlforecast-0.7.3.tar", last modified: Tue May 23 01:55:50 2023, max compression
+gzip compressed data, was "mlforecast-0.7.4.tar", last modified: Wed Jul  5 02:25:09 2023, max compression
```

## Comparing `mlforecast-0.7.3.tar` & `mlforecast-0.7.4.tar`

### file list

```diff
@@ -1,42 +1,43 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 01:55:50.569450 mlforecast-0.7.3/
--rw-r--r--   0 runner    (1001) docker     (123)     4398 2023-05-23 01:55:41.000000 mlforecast-0.7.3/CONTRIBUTING.md
--rw-r--r--   0 runner    (1001) docker     (123)    11336 2023-05-23 01:55:41.000000 mlforecast-0.7.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      111 2023-05-23 01:55:41.000000 mlforecast-0.7.3/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)    12470 2023-05-23 01:55:50.569450 mlforecast-0.7.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    11575 2023-05-23 01:55:41.000000 mlforecast-0.7.3/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 01:55:50.565450 mlforecast-0.7.3/mlforecast/
--rw-r--r--   0 runner    (1001) docker     (123)       90 2023-05-23 01:55:41.000000 mlforecast-0.7.3/mlforecast/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    28756 2023-05-23 01:55:41.000000 mlforecast-0.7.3/mlforecast/_modidx.py
--rw-r--r--   0 runner    (1001) docker     (123)    22683 2023-05-23 01:55:41.000000 mlforecast-0.7.3/mlforecast/core.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 01:55:50.569450 mlforecast-0.7.3/mlforecast/distributed/
--rw-r--r--   0 runner    (1001) docker     (123)      102 2023-05-23 01:55:41.000000 mlforecast-0.7.3/mlforecast/distributed/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    25116 2023-05-23 01:55:41.000000 mlforecast-0.7.3/mlforecast/distributed/forecast.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 01:55:50.569450 mlforecast-0.7.3/mlforecast/distributed/models/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-23 01:55:41.000000 mlforecast-0.7.3/mlforecast/distributed/models/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 01:55:50.569450 mlforecast-0.7.3/mlforecast/distributed/models/dask/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-23 01:55:41.000000 mlforecast-0.7.3/mlforecast/distributed/models/dask/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      714 2023-05-23 01:55:41.000000 mlforecast-0.7.3/mlforecast/distributed/models/dask/lgb.py
--rw-r--r--   0 runner    (1001) docker     (123)      527 2023-05-23 01:55:41.000000 mlforecast-0.7.3/mlforecast/distributed/models/dask/xgb.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 01:55:50.569450 mlforecast-0.7.3/mlforecast/distributed/models/ray/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-23 01:55:41.000000 mlforecast-0.7.3/mlforecast/distributed/models/ray/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      450 2023-05-23 01:55:41.000000 mlforecast-0.7.3/mlforecast/distributed/models/ray/lgb.py
--rw-r--r--   0 runner    (1001) docker     (123)      552 2023-05-23 01:55:41.000000 mlforecast-0.7.3/mlforecast/distributed/models/ray/xgb.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 01:55:50.569450 mlforecast-0.7.3/mlforecast/distributed/models/spark/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-23 01:55:41.000000 mlforecast-0.7.3/mlforecast/distributed/models/spark/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      836 2023-05-23 01:55:41.000000 mlforecast-0.7.3/mlforecast/distributed/models/spark/lgb.py
--rw-r--r--   0 runner    (1001) docker     (123)      862 2023-05-23 01:55:41.000000 mlforecast-0.7.3/mlforecast/distributed/models/spark/xgb.py
--rw-r--r--   0 runner    (1001) docker     (123)    25865 2023-05-23 01:55:41.000000 mlforecast-0.7.3/mlforecast/forecast.py
--rw-r--r--   0 runner    (1001) docker     (123)     7357 2023-05-23 01:55:41.000000 mlforecast-0.7.3/mlforecast/grouped_array.py
--rw-r--r--   0 runner    (1001) docker     (123)    21409 2023-05-23 01:55:41.000000 mlforecast-0.7.3/mlforecast/lgb_cv.py
--rw-r--r--   0 runner    (1001) docker     (123)     2541 2023-05-23 01:55:41.000000 mlforecast-0.7.3/mlforecast/target_transforms.py
--rw-r--r--   0 runner    (1001) docker     (123)     6309 2023-05-23 01:55:41.000000 mlforecast-0.7.3/mlforecast/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 01:55:50.569450 mlforecast-0.7.3/mlforecast.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    12470 2023-05-23 01:55:50.000000 mlforecast-0.7.3/mlforecast.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      962 2023-05-23 01:55:50.000000 mlforecast-0.7.3/mlforecast.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-23 01:55:50.000000 mlforecast-0.7.3/mlforecast.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-23 01:55:50.000000 mlforecast-0.7.3/mlforecast.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)      304 2023-05-23 01:55:50.000000 mlforecast-0.7.3/mlforecast.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       11 2023-05-23 01:55:50.000000 mlforecast-0.7.3/mlforecast.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1043 2023-05-23 01:55:41.000000 mlforecast-0.7.3/settings.ini
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-23 01:55:50.569450 mlforecast-0.7.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2613 2023-05-23 01:55:41.000000 mlforecast-0.7.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 02:25:09.500041 mlforecast-0.7.4/
+-rw-r--r--   0 runner    (1001) docker     (123)     4398 2023-07-05 02:25:00.000000 mlforecast-0.7.4/CONTRIBUTING.md
+-rw-r--r--   0 runner    (1001) docker     (123)    11336 2023-07-05 02:25:00.000000 mlforecast-0.7.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      111 2023-07-05 02:25:00.000000 mlforecast-0.7.4/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)    12470 2023-07-05 02:25:09.500041 mlforecast-0.7.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    11575 2023-07-05 02:25:00.000000 mlforecast-0.7.4/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 02:25:09.496041 mlforecast-0.7.4/mlforecast/
+-rw-r--r--   0 runner    (1001) docker     (123)       90 2023-07-05 02:25:00.000000 mlforecast-0.7.4/mlforecast/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    29050 2023-07-05 02:25:00.000000 mlforecast-0.7.4/mlforecast/_modidx.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23281 2023-07-05 02:25:00.000000 mlforecast-0.7.4/mlforecast/core.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 02:25:09.496041 mlforecast-0.7.4/mlforecast/distributed/
+-rw-r--r--   0 runner    (1001) docker     (123)      102 2023-07-05 02:25:00.000000 mlforecast-0.7.4/mlforecast/distributed/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25116 2023-07-05 02:25:00.000000 mlforecast-0.7.4/mlforecast/distributed/forecast.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 02:25:09.496041 mlforecast-0.7.4/mlforecast/distributed/models/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-05 02:25:00.000000 mlforecast-0.7.4/mlforecast/distributed/models/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 02:25:09.500041 mlforecast-0.7.4/mlforecast/distributed/models/dask/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-05 02:25:00.000000 mlforecast-0.7.4/mlforecast/distributed/models/dask/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      714 2023-07-05 02:25:00.000000 mlforecast-0.7.4/mlforecast/distributed/models/dask/lgb.py
+-rw-r--r--   0 runner    (1001) docker     (123)      527 2023-07-05 02:25:00.000000 mlforecast-0.7.4/mlforecast/distributed/models/dask/xgb.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 02:25:09.500041 mlforecast-0.7.4/mlforecast/distributed/models/ray/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-05 02:25:00.000000 mlforecast-0.7.4/mlforecast/distributed/models/ray/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      450 2023-07-05 02:25:00.000000 mlforecast-0.7.4/mlforecast/distributed/models/ray/lgb.py
+-rw-r--r--   0 runner    (1001) docker     (123)      552 2023-07-05 02:25:00.000000 mlforecast-0.7.4/mlforecast/distributed/models/ray/xgb.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 02:25:09.500041 mlforecast-0.7.4/mlforecast/distributed/models/spark/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-05 02:25:00.000000 mlforecast-0.7.4/mlforecast/distributed/models/spark/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      836 2023-07-05 02:25:00.000000 mlforecast-0.7.4/mlforecast/distributed/models/spark/lgb.py
+-rw-r--r--   0 runner    (1001) docker     (123)      862 2023-07-05 02:25:00.000000 mlforecast-0.7.4/mlforecast/distributed/models/spark/xgb.py
+-rw-r--r--   0 runner    (1001) docker     (123)    27893 2023-07-05 02:25:00.000000 mlforecast-0.7.4/mlforecast/forecast.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7357 2023-07-05 02:25:00.000000 mlforecast-0.7.4/mlforecast/grouped_array.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21426 2023-07-05 02:25:00.000000 mlforecast-0.7.4/mlforecast/lgb_cv.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2541 2023-07-05 02:25:00.000000 mlforecast-0.7.4/mlforecast/target_transforms.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6309 2023-07-05 02:25:00.000000 mlforecast-0.7.4/mlforecast/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 02:25:09.496041 mlforecast-0.7.4/mlforecast.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    12470 2023-07-05 02:25:09.000000 mlforecast-0.7.4/mlforecast.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      977 2023-07-05 02:25:09.000000 mlforecast-0.7.4/mlforecast.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-05 02:25:09.000000 mlforecast-0.7.4/mlforecast.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-05 02:25:09.000000 mlforecast-0.7.4/mlforecast.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      295 2023-07-05 02:25:09.000000 mlforecast-0.7.4/mlforecast.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       11 2023-07-05 02:25:09.000000 mlforecast-0.7.4/mlforecast.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       59 2023-07-05 02:25:00.000000 mlforecast-0.7.4/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)     1033 2023-07-05 02:25:00.000000 mlforecast-0.7.4/settings.ini
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-05 02:25:09.500041 mlforecast-0.7.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2613 2023-07-05 02:25:00.000000 mlforecast-0.7.4/setup.py
```

### Comparing `mlforecast-0.7.3/CONTRIBUTING.md` & `mlforecast-0.7.4/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `mlforecast-0.7.3/LICENSE` & `mlforecast-0.7.4/LICENSE`

 * *Files identical despite different names*

### Comparing `mlforecast-0.7.3/PKG-INFO` & `mlforecast-0.7.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mlforecast
-Version: 0.7.3
+Version: 0.7.4
 Summary: Scalable machine learning based time series forecasting
 Home-page: https://github.com/Nixtla/mlforecast
 Author: José Morales
 Author-email: jmoralz92@gmail.com
 License: Apache Software License 2.0
 Keywords: python forecast forecasting machine-learning dask
 Classifier: Development Status :: 4 - Beta
```

### Comparing `mlforecast-0.7.3/README.md` & `mlforecast-0.7.4/README.md`

 * *Files identical despite different names*

### Comparing `mlforecast-0.7.3/mlforecast/_modidx.py` & `mlforecast-0.7.4/mlforecast/_modidx.py`

 * *Files 0% similar despite different names*

```diff
@@ -103,14 +103,16 @@
                                                                                   'mlforecast/forecast.py'),
                                      'mlforecast.forecast.MLForecast.__repr__': ( 'forecast.html#mlforecast.__repr__',
                                                                                   'mlforecast/forecast.py'),
                                      'mlforecast.forecast.MLForecast._conformity_scores': ( 'forecast.html#mlforecast._conformity_scores',
                                                                                             'mlforecast/forecast.py'),
                                      'mlforecast.forecast.MLForecast.cross_validation': ( 'forecast.html#mlforecast.cross_validation',
                                                                                           'mlforecast/forecast.py'),
+                                     'mlforecast.forecast.MLForecast.cross_validation_fitted_values': ( 'forecast.html#mlforecast.cross_validation_fitted_values',
+                                                                                                        'mlforecast/forecast.py'),
                                      'mlforecast.forecast.MLForecast.fit': ('forecast.html#mlforecast.fit', 'mlforecast/forecast.py'),
                                      'mlforecast.forecast.MLForecast.fit_models': ( 'forecast.html#mlforecast.fit_models',
                                                                                     'mlforecast/forecast.py'),
                                      'mlforecast.forecast.MLForecast.freq': ('forecast.html#mlforecast.freq', 'mlforecast/forecast.py'),
                                      'mlforecast.forecast.MLForecast.from_cv': ( 'forecast.html#mlforecast.from_cv',
                                                                                  'mlforecast/forecast.py'),
                                      'mlforecast.forecast.MLForecast.predict': ( 'forecast.html#mlforecast.predict',
```

### Comparing `mlforecast-0.7.3/mlforecast/core.py` & `mlforecast-0.7.4/mlforecast/core.py`

 * *Files 5% similar despite different names*

```diff
@@ -218,22 +218,27 @@
                 warnings.warn("Setting `freq=1` since time col is int.")
                 self.freq = 1
         else:
             raise ValueError(f"{time_col} must be either timestamp or integer.")
         self.id_col = id_col
         self.target_col = target_col
         self.time_col = time_col
+        to_drop = [id_col, time_col, target_col]
+        self.static_features = static_features
         if static_features is None:
-            static_features = df.columns.drop([id_col, time_col, target_col])
-        elif id_col in static_features:
-            raise ValueError(
-                "Cannot use the id_col as a static feature. Please create a separate column."
-            )
-        self.static_features = (
-            df.set_index(id_col)[static_features].groupby(id_col, observed=True).head(1)
+            static_features = df.columns.drop([time_col, target_col]).tolist()
+        elif id_col not in static_features:
+            static_features = [id_col] + static_features
+        else:  # static_features defined and contain id_col
+            to_drop = [time_col, target_col]
+        self.static_features_ = (
+            df[static_features]
+            .groupby(id_col, observed=True)
+            .head(1)
+            .reset_index(drop=True)
         )
         sort_idxs = pd.core.sorting.lexsort_indexer([df[id_col], df[time_col]])
         self.restore_idxs = np.empty(df.shape[0], dtype=np.int32)
         self.restore_idxs[sort_idxs] = np.arange(df.shape[0])
         sorted_df = df[[id_col, time_col, target_col]].iloc[sort_idxs]
         if self.target_transforms is not None:
             for tfm in self.target_transforms:
@@ -245,17 +250,15 @@
         self.features_ = self._compute_transforms()
         if keep_last_n is not None:
             self.ga = self.ga.take_from_groups(slice(-keep_last_n, None))
         self._ga = GroupedArray(self.ga.data, self.ga.indptr)
         self.last_dates = sorted_df.index.get_level_values(self.time_col)[
             self.ga.indptr[1:] - 1
         ]
-        self.features_order_ = (
-            df.columns.drop([id_col, time_col, target_col]).tolist() + self.features
-        )
+        self.features_order_ = df.columns.drop(to_drop).tolist() + self.features
         return self
 
     def _apply_transforms(self, updates_only: bool = False) -> Dict[str, np.ndarray]:
         """Apply the transformations using the main process.
 
         If `updates_only` then only the updates are returned.
         """
@@ -429,15 +432,15 @@
         for feature in self.date_features:
             feat_name, feat_vals = self._compute_date_feature(self.curr_dates, feature)
             features[feat_name] = feat_vals
 
         features_df = pd.DataFrame(features, columns=self.features)
         features_df[self.id_col] = self.uids
         features_df[self.time_col] = self.curr_dates
-        return self.static_features.merge(features_df, on=self.id_col)
+        return self.static_features_.merge(features_df, on=self.id_col)
 
     def _get_raw_predictions(self) -> np.ndarray:
         return np.array(self.y_pred).ravel("F")
 
     def _get_predictions(self) -> pd.DataFrame:
         """Get all the predicted values with their corresponding ids and datestamps."""
         n_preds = len(self.y_pred)
@@ -576,17 +579,26 @@
             df.groupby(self.id_col, observed=True)[self.time_col]
             .max()
             .reindex(sizes.index)
             .fillna(dict(zip(self.uids, self.last_dates)))
         ).astype(self.last_dates.dtype)
         self.uids = sizes.index
         new_statics = df.iloc[new_sizes.cumsum() - 1].set_index(self.id_col)
-        orig_dtypes = self.static_features.dtypes
-        self.static_features = self.static_features.reindex(self.uids)
-        self.static_features.update(new_statics)
-        self.static_features = self.static_features.astype(orig_dtypes)
+        orig_dtypes = self.static_features_.dtypes
+        if pd.api.types.is_categorical_dtype(orig_dtypes[self.id_col]):
+            orig_categories = orig_dtypes[self.id_col].categories.tolist()
+            missing_categories = set(self.uids) - set(orig_categories)
+            if missing_categories:
+                orig_dtypes[self.id_col] = pd.CategoricalDtype(
+                    categories=orig_categories + list(missing_categories)
+                )
+        self.static_features_ = self.static_features_.set_index(self.id_col).reindex(
+            self.uids
+        )
+        self.static_features_.update(new_statics)
+        self.static_features_ = self.static_features_.reset_index().astype(orig_dtypes)
         self.ga = self.ga.append_several(
             new_sizes=sizes.values.astype(np.int32),
             new_values=values,
             new_groups=new_groups,
         )
         self._ga = GroupedArray(self.ga.data, self.ga.indptr)
```

### Comparing `mlforecast-0.7.3/mlforecast/distributed/forecast.py` & `mlforecast-0.7.4/mlforecast/distributed/forecast.py`

 * *Files identical despite different names*

### Comparing `mlforecast-0.7.3/mlforecast/distributed/models/dask/lgb.py` & `mlforecast-0.7.4/mlforecast/distributed/models/dask/lgb.py`

 * *Files identical despite different names*

### Comparing `mlforecast-0.7.3/mlforecast/distributed/models/dask/xgb.py` & `mlforecast-0.7.4/mlforecast/distributed/models/dask/xgb.py`

 * *Files identical despite different names*

### Comparing `mlforecast-0.7.3/mlforecast/distributed/models/ray/xgb.py` & `mlforecast-0.7.4/mlforecast/distributed/models/ray/xgb.py`

 * *Files identical despite different names*

### Comparing `mlforecast-0.7.3/mlforecast/distributed/models/spark/lgb.py` & `mlforecast-0.7.4/mlforecast/distributed/models/spark/lgb.py`

 * *Files identical despite different names*

### Comparing `mlforecast-0.7.3/mlforecast/distributed/models/spark/xgb.py` & `mlforecast-0.7.4/mlforecast/distributed/models/spark/xgb.py`

 * *Files identical despite different names*

### Comparing `mlforecast-0.7.3/mlforecast/forecast.py` & `mlforecast-0.7.4/mlforecast/forecast.py`

 * *Files 4% similar despite different names*

```diff
@@ -440,15 +440,15 @@
                 target_transforms=self.ts.target_transforms,
             )
             new_ts._fit(
                 new_data,
                 id_col=self.ts.id_col,
                 time_col=self.ts.time_col,
                 target_col=self.ts.target_col,
-                static_features=self.ts.static_features.columns,
+                static_features=self.ts.static_features,
                 keep_last_n=self.ts.keep_last_n,
             )
             new_ts.max_horizon = self.ts.max_horizon
             ts = new_ts
         else:
             ts = self.ts
 
@@ -516,14 +516,15 @@
         refit: bool = True,
         max_horizon: Optional[int] = None,
         before_predict_callback: Optional[Callable] = None,
         after_predict_callback: Optional[Callable] = None,
         prediction_intervals: Optional[PredictionIntervals] = None,
         level: Optional[List[Union[int, float]]] = None,
         input_size: Optional[int] = None,
+        fitted: bool = False,
     ):
         """Perform time series cross validation.
         Creates `n_windows` splits where each window has `window_size` test periods,
         trains the models, computes the predictions and merges the actuals.
 
         Parameters
         ----------
@@ -562,14 +563,16 @@
                 The series identifier is on the index.
         prediction_intervals : PredictionIntervals, optional (default=None)
             Configuration to calibrate prediction intervals (Conformal Prediction).
         level : list of ints or floats, optional (default=None)
             Confidence levels between 0 and 100 for prediction intervals.
         input_size : int, optional (default=None)
             Maximum training samples per serie in each window. If None, will use an expanding window.
+        fitted : bool (default=False)
+            Store the in-sample predictions.
 
         Returns
         -------
         result : pandas DataFrame
             Predictions for each window with the series id, timestamp, last train date, target value and predictions from each model.
         """
         if hasattr(self, "models_"):
@@ -593,38 +596,74 @@
             step_size=step_size,
             input_size=input_size,
         )
         ex_cols_to_drop = [id_col, time_col, target_col]
         if static_features is not None:
             ex_cols_to_drop.extend(static_features)
         has_ex = not data.columns.drop(ex_cols_to_drop).empty
+        self.cv_fitted_values_ = []
         for i_window, (cutoffs, train, valid) in enumerate(splits):
             if refit or i_window == 0:
                 self.fit(
                     train,
                     id_col=id_col,
                     time_col=time_col,
                     target_col=target_col,
                     static_features=static_features,
                     dropna=dropna,
                     keep_last_n=keep_last_n,
                     max_horizon=max_horizon,
                     prediction_intervals=prediction_intervals,
                 )
             self.cv_models_.append(self.models_)
+            if fitted:
+                insample_results = train[[id_col, time_col]].copy()
+                trainX, _ = self.preprocess(
+                    train,
+                    id_col=id_col,
+                    time_col=time_col,
+                    target_col=target_col,
+                    static_features=static_features,
+                    dropna=False,
+                    keep_last_n=keep_last_n,
+                    max_horizon=max_horizon,
+                    return_X_y=True,
+                )
+                trainX = trainX[self.ts.features_order_]
+                for name, model in self.models_.items():
+                    insample_results[name] = model.predict(trainX)  # type: ignore[union-attr]
+                if self.ts.target_transforms is not None:
+                    for tfm in self.ts.target_transforms[::-1]:
+                        insample_results = tfm.inverse_transform(insample_results)
+                insample_results["fold"] = i_window
+                insample_results[target_col] = train[target_col].values
+                self.cv_fitted_values_.append(insample_results)
             dynamic_dfs = [valid.drop(columns=[target_col])] if has_ex else None
             y_pred = self.predict(
                 window_size,
                 dynamic_dfs,
                 before_predict_callback,
                 after_predict_callback,
                 new_data=train if not refit else None,
                 level=level,
             )
             y_pred = y_pred.merge(cutoffs, on=id_col, how="left")
             result = valid[[id_col, time_col, target_col]].merge(
                 y_pred, on=[id_col, time_col]
             )
+            if result.shape[0] < valid.shape[0]:
+                raise ValueError(
+                    "Cross validation result produced less results than expected. "
+                    "Please verify that the frequency set on the MLForecast constructor matches your series' "
+                    "and that there aren't any missing periods."
+                )
             results.append(result)
         out = pd.concat(results)
         cols_order = [id_col, time_col, "cutoff", target_col]
         return out[cols_order + out.columns.drop(cols_order).tolist()]
+
+    def cross_validation_fitted_values(self):
+        if not getattr(self, "cv_fitted_values_", []):
+            raise ValueError("Please run cross_validation with fitted=True first.")
+        cols_order = [self.ts.id_col, self.ts.time_col, "fold", self.ts.target_col]
+        out = pd.concat(self.cv_fitted_values_).reset_index(drop=True)
+        return out[cols_order + out.columns.drop(cols_order).tolist()]
```

### Comparing `mlforecast-0.7.3/mlforecast/grouped_array.py` & `mlforecast-0.7.4/mlforecast/grouped_array.py`

 * *Files identical despite different names*

### Comparing `mlforecast-0.7.3/mlforecast/lgb_cv.py` & `mlforecast-0.7.4/mlforecast/lgb_cv.py`

 * *Files 1% similar despite different names*

```diff
@@ -41,15 +41,15 @@
 def _update(bst, n):
     for _ in range(n):
         bst.update()
 
 
 def _predict(ts, bst, valid, h, before_predict_callback, after_predict_callback):
     ex_cols_to_drop = [ts.id_col, ts.time_col, ts.target_col]
-    static_features = ts.static_features.columns.tolist()
+    static_features = ts.static_features_.columns.drop(ts.id_col).tolist()
     ex_cols_to_drop.extend(static_features)
     has_ex = not valid.columns.drop(ex_cols_to_drop).empty
     dynamic_dfs = (
         [valid.drop(columns=static_features + [ts.target_col])] if has_ex else None
     )
     preds = ts.predict(
         {"Booster": bst},
```

### Comparing `mlforecast-0.7.3/mlforecast/target_transforms.py` & `mlforecast-0.7.4/mlforecast/target_transforms.py`

 * *Files identical despite different names*

### Comparing `mlforecast-0.7.3/mlforecast/utils.py` & `mlforecast-0.7.4/mlforecast/utils.py`

 * *Files identical despite different names*

### Comparing `mlforecast-0.7.3/mlforecast.egg-info/PKG-INFO` & `mlforecast-0.7.4/mlforecast.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mlforecast
-Version: 0.7.3
+Version: 0.7.4
 Summary: Scalable machine learning based time series forecasting
 Home-page: https://github.com/Nixtla/mlforecast
 Author: José Morales
 Author-email: jmoralz92@gmail.com
 License: Apache Software License 2.0
 Keywords: python forecast forecasting machine-learning dask
 Classifier: Development Status :: 4 - Beta
```

### Comparing `mlforecast-0.7.3/mlforecast.egg-info/SOURCES.txt` & `mlforecast-0.7.4/mlforecast.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 CONTRIBUTING.md
 LICENSE
 MANIFEST.in
 README.md
+pyproject.toml
 settings.ini
 setup.py
 mlforecast/__init__.py
 mlforecast/_modidx.py
 mlforecast/core.py
 mlforecast/forecast.py
 mlforecast/grouped_array.py
```

### Comparing `mlforecast-0.7.3/settings.ini` & `mlforecast-0.7.4/settings.ini`

 * *Files 3% similar despite different names*

```diff
@@ -4,24 +4,24 @@
 user = Nixtla
 description = Scalable machine learning based time series forecasting
 keywords = python forecast forecasting machine-learning dask
 author = José Morales
 author_email = jmoralz92@gmail.com
 copyright = Nixtla
 branch = main
-version = 0.7.3
+version = 0.7.4
 min_python = 3.6
 audience = Developers
 language = English
 custom_sidebar = True
 license = apache2
 status = 3
 requirements = numba pandas scikit-learn window-ops
-distributed_requirements = dask[complete] fugue[ray]  pyspark lightgbm_ray xgboost_ray
-dev_requirements = black datasetsforecast flake8 lightgbm matplotlib mypy nbdev pylint statsforecast xgboost
+distributed_requirements = dask[complete] fugue[ray] pyspark lightgbm_ray xgboost_ray
+dev_requirements = black datasetsforecast lightgbm matplotlib mypy nbdev ruff statsforecast xgboost
 nbs_path = nbs
 doc_path = _docs
 recursive = True
 doc_host = https://Nixtla.github.io
 doc_baseurl = /
 git_url = https://github.com/Nixtla/mlforecast
 lib_path = mlforecast
```

### Comparing `mlforecast-0.7.3/setup.py` & `mlforecast-0.7.4/setup.py`

 * *Files identical despite different names*

