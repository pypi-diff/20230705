# Comparing `tmp/databricks-automl-runtime-0.2.9.tar.gz` & `tmp/databricks-automl-runtime-0.2.9.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "databricks-automl-runtime-0.2.9.tar", last modified: Fri Jun 24 00:23:56 2022, max compression
+gzip compressed data, was "databricks-automl-runtime-0.2.9.1.tar", last modified: Mon Jun 27 23:44:05 2022, max compression
```

## Comparing `databricks-automl-runtime-0.2.9.tar` & `databricks-automl-runtime-0.2.9.1.tar`

### file list

```diff
@@ -1,40 +1,40 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-24 00:23:56.040845 databricks-automl-runtime-0.2.9/
--rw-r--r--   0 runner    (1001) docker     (121)      456 2022-06-24 00:23:56.040845 databricks-automl-runtime-0.2.9/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)       36 2022-06-24 00:16:34.000000 databricks-automl-runtime-0.2.9/README.md
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-24 00:23:56.036845 databricks-automl-runtime-0.2.9/databricks/
--rw-r--r--   0 runner    (1001) docker     (121)      884 2022-06-24 00:16:34.000000 databricks-automl-runtime-0.2.9/databricks/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-24 00:23:56.036845 databricks-automl-runtime-0.2.9/databricks/automl_runtime/
--rw-r--r--   0 runner    (1001) docker     (121)      673 2022-06-24 00:16:34.000000 databricks-automl-runtime-0.2.9/databricks/automl_runtime/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-24 00:23:56.036845 databricks-automl-runtime-0.2.9/databricks/automl_runtime/forecast/
--rw-r--r--   0 runner    (1001) docker     (121)      926 2022-06-24 00:16:34.000000 databricks-automl-runtime-0.2.9/databricks/automl_runtime/forecast/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     2421 2022-06-24 00:16:34.000000 databricks-automl-runtime-0.2.9/databricks/automl_runtime/forecast/model.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-24 00:23:56.036845 databricks-automl-runtime-0.2.9/databricks/automl_runtime/forecast/pmdarima/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-06-24 00:16:34.000000 databricks-automl-runtime-0.2.9/databricks/automl_runtime/forecast/pmdarima/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     3321 2022-06-24 00:16:34.000000 databricks-automl-runtime-0.2.9/databricks/automl_runtime/forecast/pmdarima/diagnostics.py
--rw-r--r--   0 runner    (1001) docker     (121)    14173 2022-06-24 00:16:34.000000 databricks-automl-runtime-0.2.9/databricks/automl_runtime/forecast/pmdarima/model.py
--rw-r--r--   0 runner    (1001) docker     (121)     6565 2022-06-24 00:16:34.000000 databricks-automl-runtime-0.2.9/databricks/automl_runtime/forecast/pmdarima/training.py
--rw-r--r--   0 runner    (1001) docker     (121)     2496 2022-06-24 00:16:34.000000 databricks-automl-runtime-0.2.9/databricks/automl_runtime/forecast/pmdarima/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-24 00:23:56.036845 databricks-automl-runtime-0.2.9/databricks/automl_runtime/forecast/prophet/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-06-24 00:16:34.000000 databricks-automl-runtime-0.2.9/databricks/automl_runtime/forecast/prophet/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     7537 2022-06-24 00:16:34.000000 databricks-automl-runtime-0.2.9/databricks/automl_runtime/forecast/prophet/forecast.py
--rw-r--r--   0 runner    (1001) docker     (121)    12946 2022-06-24 00:16:34.000000 databricks-automl-runtime-0.2.9/databricks/automl_runtime/forecast/prophet/model.py
--rw-r--r--   0 runner    (1001) docker     (121)     4381 2022-06-24 00:16:34.000000 databricks-automl-runtime-0.2.9/databricks/automl_runtime/forecast/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-24 00:23:56.036845 databricks-automl-runtime-0.2.9/databricks/automl_runtime/hyperopt/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-06-24 00:16:34.000000 databricks-automl-runtime-0.2.9/databricks/automl_runtime/hyperopt/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     3467 2022-06-24 00:16:34.000000 databricks-automl-runtime-0.2.9/databricks/automl_runtime/hyperopt/early_stop.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-24 00:23:56.040845 databricks-automl-runtime-0.2.9/databricks/automl_runtime/sklearn/
--rw-r--r--   0 runner    (1001) docker     (121)      910 2022-06-24 00:16:34.000000 databricks-automl-runtime-0.2.9/databricks/automl_runtime/sklearn/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     4076 2022-06-24 00:16:34.000000 databricks-automl-runtime-0.2.9/databricks/automl_runtime/sklearn/base_datetime_transformer.py
--rw-r--r--   0 runner    (1001) docker     (121)     1791 2022-06-24 00:16:34.000000 databricks-automl-runtime-0.2.9/databricks/automl_runtime/sklearn/column_selector.py
--rw-r--r--   0 runner    (1001) docker     (121)     1400 2022-06-24 00:16:34.000000 databricks-automl-runtime-0.2.9/databricks/automl_runtime/sklearn/date_transformer.py
--rw-r--r--   0 runner    (1001) docker     (121)     2758 2022-06-24 00:16:34.000000 databricks-automl-runtime-0.2.9/databricks/automl_runtime/sklearn/datetime_imputer.py
--rw-r--r--   0 runner    (1001) docker     (121)     1669 2022-06-24 00:16:34.000000 databricks-automl-runtime-0.2.9/databricks/automl_runtime/sklearn/timestamp_transformer.py
--rw-r--r--   0 runner    (1001) docker     (121)      996 2022-06-24 00:16:34.000000 databricks-automl-runtime-0.2.9/databricks/automl_runtime/utils.py
--rw-r--r--   0 runner    (1001) docker     (121)      631 2022-06-24 00:16:34.000000 databricks-automl-runtime-0.2.9/databricks/automl_runtime/version.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-24 00:23:56.040845 databricks-automl-runtime-0.2.9/databricks_automl_runtime.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)      456 2022-06-24 00:23:55.000000 databricks-automl-runtime-0.2.9/databricks_automl_runtime.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     1346 2022-06-24 00:23:56.000000 databricks-automl-runtime-0.2.9/databricks_automl_runtime.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-06-24 00:23:55.000000 databricks-automl-runtime-0.2.9/databricks_automl_runtime.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)       11 2022-06-24 00:23:55.000000 databricks-automl-runtime-0.2.9/databricks_automl_runtime.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (121)       38 2022-06-24 00:23:56.040845 databricks-automl-runtime-0.2.9/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)     2204 2022-06-24 00:16:34.000000 databricks-automl-runtime-0.2.9/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-27 23:44:05.980531 databricks-automl-runtime-0.2.9.1/
+-rw-r--r--   0 runner    (1001) docker     (121)      458 2022-06-27 23:44:05.980531 databricks-automl-runtime-0.2.9.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (121)       36 2022-06-27 23:38:04.000000 databricks-automl-runtime-0.2.9.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-27 23:44:05.976531 databricks-automl-runtime-0.2.9.1/databricks/
+-rw-r--r--   0 runner    (1001) docker     (121)      884 2022-06-27 23:38:04.000000 databricks-automl-runtime-0.2.9.1/databricks/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-27 23:44:05.976531 databricks-automl-runtime-0.2.9.1/databricks/automl_runtime/
+-rw-r--r--   0 runner    (1001) docker     (121)      673 2022-06-27 23:38:04.000000 databricks-automl-runtime-0.2.9.1/databricks/automl_runtime/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-27 23:44:05.976531 databricks-automl-runtime-0.2.9.1/databricks/automl_runtime/forecast/
+-rw-r--r--   0 runner    (1001) docker     (121)      926 2022-06-27 23:38:04.000000 databricks-automl-runtime-0.2.9.1/databricks/automl_runtime/forecast/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2421 2022-06-27 23:38:04.000000 databricks-automl-runtime-0.2.9.1/databricks/automl_runtime/forecast/model.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-27 23:44:05.976531 databricks-automl-runtime-0.2.9.1/databricks/automl_runtime/forecast/pmdarima/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2022-06-27 23:38:04.000000 databricks-automl-runtime-0.2.9.1/databricks/automl_runtime/forecast/pmdarima/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3321 2022-06-27 23:38:04.000000 databricks-automl-runtime-0.2.9.1/databricks/automl_runtime/forecast/pmdarima/diagnostics.py
+-rw-r--r--   0 runner    (1001) docker     (121)    14173 2022-06-27 23:38:04.000000 databricks-automl-runtime-0.2.9.1/databricks/automl_runtime/forecast/pmdarima/model.py
+-rw-r--r--   0 runner    (1001) docker     (121)     6565 2022-06-27 23:38:04.000000 databricks-automl-runtime-0.2.9.1/databricks/automl_runtime/forecast/pmdarima/training.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2496 2022-06-27 23:38:04.000000 databricks-automl-runtime-0.2.9.1/databricks/automl_runtime/forecast/pmdarima/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-27 23:44:05.976531 databricks-automl-runtime-0.2.9.1/databricks/automl_runtime/forecast/prophet/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2022-06-27 23:38:04.000000 databricks-automl-runtime-0.2.9.1/databricks/automl_runtime/forecast/prophet/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     7537 2022-06-27 23:38:04.000000 databricks-automl-runtime-0.2.9.1/databricks/automl_runtime/forecast/prophet/forecast.py
+-rw-r--r--   0 runner    (1001) docker     (121)    12946 2022-06-27 23:38:04.000000 databricks-automl-runtime-0.2.9.1/databricks/automl_runtime/forecast/prophet/model.py
+-rw-r--r--   0 runner    (1001) docker     (121)     4381 2022-06-27 23:38:04.000000 databricks-automl-runtime-0.2.9.1/databricks/automl_runtime/forecast/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-27 23:44:05.976531 databricks-automl-runtime-0.2.9.1/databricks/automl_runtime/hyperopt/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2022-06-27 23:38:04.000000 databricks-automl-runtime-0.2.9.1/databricks/automl_runtime/hyperopt/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3467 2022-06-27 23:38:04.000000 databricks-automl-runtime-0.2.9.1/databricks/automl_runtime/hyperopt/early_stop.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-27 23:44:05.980531 databricks-automl-runtime-0.2.9.1/databricks/automl_runtime/sklearn/
+-rw-r--r--   0 runner    (1001) docker     (121)      910 2022-06-27 23:38:04.000000 databricks-automl-runtime-0.2.9.1/databricks/automl_runtime/sklearn/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     4076 2022-06-27 23:38:04.000000 databricks-automl-runtime-0.2.9.1/databricks/automl_runtime/sklearn/base_datetime_transformer.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1791 2022-06-27 23:38:04.000000 databricks-automl-runtime-0.2.9.1/databricks/automl_runtime/sklearn/column_selector.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1400 2022-06-27 23:38:04.000000 databricks-automl-runtime-0.2.9.1/databricks/automl_runtime/sklearn/date_transformer.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2775 2022-06-27 23:38:04.000000 databricks-automl-runtime-0.2.9.1/databricks/automl_runtime/sklearn/datetime_imputer.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1669 2022-06-27 23:38:04.000000 databricks-automl-runtime-0.2.9.1/databricks/automl_runtime/sklearn/timestamp_transformer.py
+-rw-r--r--   0 runner    (1001) docker     (121)      996 2022-06-27 23:38:04.000000 databricks-automl-runtime-0.2.9.1/databricks/automl_runtime/utils.py
+-rw-r--r--   0 runner    (1001) docker     (121)      633 2022-06-27 23:38:04.000000 databricks-automl-runtime-0.2.9.1/databricks/automl_runtime/version.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-27 23:44:05.980531 databricks-automl-runtime-0.2.9.1/databricks_automl_runtime.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (121)      458 2022-06-27 23:44:05.000000 databricks-automl-runtime-0.2.9.1/databricks_automl_runtime.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (121)     1346 2022-06-27 23:44:05.000000 databricks-automl-runtime-0.2.9.1/databricks_automl_runtime.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (121)        1 2022-06-27 23:44:05.000000 databricks-automl-runtime-0.2.9.1/databricks_automl_runtime.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (121)       11 2022-06-27 23:44:05.000000 databricks-automl-runtime-0.2.9.1/databricks_automl_runtime.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (121)       38 2022-06-27 23:44:05.980531 databricks-automl-runtime-0.2.9.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (121)     2204 2022-06-27 23:38:04.000000 databricks-automl-runtime-0.2.9.1/setup.py
```

### Comparing `databricks-automl-runtime-0.2.9/databricks/__init__.py` & `databricks-automl-runtime-0.2.9.1/databricks/__init__.py`

 * *Files identical despite different names*

### Comparing `databricks-automl-runtime-0.2.9/databricks/automl_runtime/__init__.py` & `databricks-automl-runtime-0.2.9.1/databricks/automl_runtime/__init__.py`

 * *Files identical despite different names*

### Comparing `databricks-automl-runtime-0.2.9/databricks/automl_runtime/forecast/__init__.py` & `databricks-automl-runtime-0.2.9.1/databricks/automl_runtime/forecast/__init__.py`

 * *Files identical despite different names*

### Comparing `databricks-automl-runtime-0.2.9/databricks/automl_runtime/forecast/model.py` & `databricks-automl-runtime-0.2.9.1/databricks/automl_runtime/forecast/model.py`

 * *Files identical despite different names*

### Comparing `databricks-automl-runtime-0.2.9/databricks/automl_runtime/forecast/pmdarima/diagnostics.py` & `databricks-automl-runtime-0.2.9.1/databricks/automl_runtime/forecast/pmdarima/diagnostics.py`

 * *Files identical despite different names*

### Comparing `databricks-automl-runtime-0.2.9/databricks/automl_runtime/forecast/pmdarima/model.py` & `databricks-automl-runtime-0.2.9.1/databricks/automl_runtime/forecast/pmdarima/model.py`

 * *Files identical despite different names*

### Comparing `databricks-automl-runtime-0.2.9/databricks/automl_runtime/forecast/pmdarima/training.py` & `databricks-automl-runtime-0.2.9.1/databricks/automl_runtime/forecast/pmdarima/training.py`

 * *Files identical despite different names*

### Comparing `databricks-automl-runtime-0.2.9/databricks/automl_runtime/forecast/pmdarima/utils.py` & `databricks-automl-runtime-0.2.9.1/databricks/automl_runtime/forecast/pmdarima/utils.py`

 * *Files identical despite different names*

### Comparing `databricks-automl-runtime-0.2.9/databricks/automl_runtime/forecast/prophet/forecast.py` & `databricks-automl-runtime-0.2.9.1/databricks/automl_runtime/forecast/prophet/forecast.py`

 * *Files identical despite different names*

### Comparing `databricks-automl-runtime-0.2.9/databricks/automl_runtime/forecast/prophet/model.py` & `databricks-automl-runtime-0.2.9.1/databricks/automl_runtime/forecast/prophet/model.py`

 * *Files identical despite different names*

### Comparing `databricks-automl-runtime-0.2.9/databricks/automl_runtime/forecast/utils.py` & `databricks-automl-runtime-0.2.9.1/databricks/automl_runtime/forecast/utils.py`

 * *Files identical despite different names*

### Comparing `databricks-automl-runtime-0.2.9/databricks/automl_runtime/hyperopt/early_stop.py` & `databricks-automl-runtime-0.2.9.1/databricks/automl_runtime/hyperopt/early_stop.py`

 * *Files identical despite different names*

### Comparing `databricks-automl-runtime-0.2.9/databricks/automl_runtime/sklearn/__init__.py` & `databricks-automl-runtime-0.2.9.1/databricks/automl_runtime/sklearn/__init__.py`

 * *Files identical despite different names*

### Comparing `databricks-automl-runtime-0.2.9/databricks/automl_runtime/sklearn/base_datetime_transformer.py` & `databricks-automl-runtime-0.2.9.1/databricks/automl_runtime/sklearn/base_datetime_transformer.py`

 * *Files identical despite different names*

### Comparing `databricks-automl-runtime-0.2.9/databricks/automl_runtime/sklearn/column_selector.py` & `databricks-automl-runtime-0.2.9.1/databricks/automl_runtime/sklearn/column_selector.py`

 * *Files identical despite different names*

### Comparing `databricks-automl-runtime-0.2.9/databricks/automl_runtime/sklearn/date_transformer.py` & `databricks-automl-runtime-0.2.9.1/databricks/automl_runtime/sklearn/date_transformer.py`

 * *Files identical despite different names*

### Comparing `databricks-automl-runtime-0.2.9/databricks/automl_runtime/sklearn/datetime_imputer.py` & `databricks-automl-runtime-0.2.9.1/databricks/automl_runtime/sklearn/datetime_imputer.py`

 * *Files 2% similar despite different names*

```diff
@@ -64,9 +64,9 @@
     def transform(self, X):
         """Convert the input to datetime object and then impute the missing values.
 
         Parameters
         ----------
         X: a pandas DataFrame whose values are date or timestamp.
         """
-        return X.apply(pd.to_datetime).fillna(self.fill_values)
+        return X.apply(pd.to_datetime, errors="coerce").fillna(self.fill_values)
```

### Comparing `databricks-automl-runtime-0.2.9/databricks/automl_runtime/sklearn/timestamp_transformer.py` & `databricks-automl-runtime-0.2.9.1/databricks/automl_runtime/sklearn/timestamp_transformer.py`

 * *Files identical despite different names*

### Comparing `databricks-automl-runtime-0.2.9/databricks/automl_runtime/utils.py` & `databricks-automl-runtime-0.2.9.1/databricks/automl_runtime/utils.py`

 * *Files identical despite different names*

### Comparing `databricks-automl-runtime-0.2.9/databricks/automl_runtime/version.py` & `databricks-automl-runtime-0.2.9.1/databricks/automl_runtime/version.py`

 * *Files 15% similar despite different names*

```diff
@@ -10,8 +10,8 @@
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 #
 
-__version__ = "0.2.9"  # pragma: no cover
+__version__ = "0.2.9.1"  # pragma: no cover
```

### Comparing `databricks-automl-runtime-0.2.9/databricks_automl_runtime.egg-info/SOURCES.txt` & `databricks-automl-runtime-0.2.9.1/databricks_automl_runtime.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `databricks-automl-runtime-0.2.9/setup.py` & `databricks-automl-runtime-0.2.9.1/setup.py`

 * *Files identical despite different names*

