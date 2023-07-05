# Comparing `tmp/pvoutput-ocf-0.1.8.tar.gz` & `tmp/pvoutput-ocf-0.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pvoutput-ocf-0.1.8.tar", last modified: Tue Mar 15 12:47:27 2022, max compression
+gzip compressed data, was "pvoutput-ocf-0.1.9.tar", last modified: Tue Mar 15 13:17:09 2022, max compression
```

## Comparing `pvoutput-ocf-0.1.8.tar` & `pvoutput-ocf-0.1.9.tar`

### file list

```diff
@@ -1,36 +1,36 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-03-15 12:47:27.053066 pvoutput-ocf-0.1.8/
--rw-r--r--   0 runner    (1001) docker     (121)    11347 2022-03-15 12:47:12.000000 pvoutput-ocf-0.1.8/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (121)       14 2022-03-15 12:47:12.000000 pvoutput-ocf-0.1.8/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (121)     5988 2022-03-15 12:47:27.053066 pvoutput-ocf-0.1.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     5777 2022-03-15 12:47:12.000000 pvoutput-ocf-0.1.8/README.md
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-03-15 12:47:27.053066 pvoutput-ocf-0.1.8/pvoutput/
--rw-r--r--   0 runner    (1001) docker     (121)       43 2022-03-15 12:47:12.000000 pvoutput-ocf-0.1.8/pvoutput/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     6764 2022-03-15 12:47:12.000000 pvoutput-ocf-0.1.8/pvoutput/consts.py
--rw-r--r--   0 runner    (1001) docker     (121)     3718 2022-03-15 12:47:12.000000 pvoutput-ocf-0.1.8/pvoutput/daterange.py
--rw-r--r--   0 runner    (1001) docker     (121)      631 2022-03-15 12:47:12.000000 pvoutput-ocf-0.1.8/pvoutput/exceptions.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-03-15 12:47:27.053066 pvoutput-ocf-0.1.8/pvoutput/grid_search/
--rw-r--r--   0 runner    (1001) docker     (121)       36 2022-03-15 12:47:12.000000 pvoutput-ocf-0.1.8/pvoutput/grid_search/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     7785 2022-03-15 12:47:12.000000 pvoutput-ocf-0.1.8/pvoutput/grid_search/app.py
--rw-r--r--   0 runner    (1001) docker     (121)     8895 2022-03-15 12:47:12.000000 pvoutput-ocf-0.1.8/pvoutput/grid_search/clip.py
--rw-r--r--   0 runner    (1001) docker     (121)     9216 2022-03-15 12:47:12.000000 pvoutput-ocf-0.1.8/pvoutput/grid_search/grid_search.py
--rw-r--r--   0 runner    (1001) docker     (121)     5425 2022-03-15 12:47:12.000000 pvoutput-ocf-0.1.8/pvoutput/grid_search/natural_earth.py
--rw-r--r--   0 runner    (1001) docker     (121)    11253 2022-03-15 12:47:12.000000 pvoutput-ocf-0.1.8/pvoutput/mapscraper.py
--rw-r--r--   0 runner    (1001) docker     (121)    46581 2022-03-15 12:47:12.000000 pvoutput-ocf-0.1.8/pvoutput/pvoutput.py
--rw-r--r--   0 runner    (1001) docker     (121)     6499 2022-03-15 12:47:12.000000 pvoutput-ocf-0.1.8/pvoutput/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-03-15 12:47:27.053066 pvoutput-ocf-0.1.8/pvoutput_ocf.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)     5988 2022-03-15 12:47:26.000000 pvoutput-ocf-0.1.8/pvoutput_ocf.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      703 2022-03-15 12:47:27.000000 pvoutput-ocf-0.1.8/pvoutput_ocf.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-03-15 12:47:26.000000 pvoutput-ocf-0.1.8/pvoutput_ocf.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)      130 2022-03-15 12:47:26.000000 pvoutput-ocf-0.1.8/pvoutput_ocf.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)       15 2022-03-15 12:47:27.000000 pvoutput-ocf-0.1.8/pvoutput_ocf.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (121)      130 2022-03-15 12:47:12.000000 pvoutput-ocf-0.1.8/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (121)       38 2022-03-15 12:47:27.053066 pvoutput-ocf-0.1.8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)      568 2022-03-15 12:47:13.000000 pvoutput-ocf-0.1.8/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-03-15 12:47:27.053066 pvoutput-ocf-0.1.8/tests/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-03-15 12:47:12.000000 pvoutput-ocf-0.1.8/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     1751 2022-03-15 12:47:12.000000 pvoutput-ocf-0.1.8/tests/conftest.py
--rw-r--r--   0 runner    (1001) docker     (121)     3699 2022-03-15 12:47:12.000000 pvoutput-ocf-0.1.8/tests/test_daterange.py
--rw-r--r--   0 runner    (1001) docker     (121)     2709 2022-03-15 12:47:12.000000 pvoutput-ocf-0.1.8/tests/test_grid_search.py
--rw-r--r--   0 runner    (1001) docker     (121)     2720 2022-03-15 12:47:12.000000 pvoutput-ocf-0.1.8/tests/test_mapscraper.py
--rw-r--r--   0 runner    (1001) docker     (121)     4133 2022-03-15 12:47:12.000000 pvoutput-ocf-0.1.8/tests/test_pvoutput.py
--rw-r--r--   0 runner    (1001) docker     (121)     1516 2022-03-15 12:47:12.000000 pvoutput-ocf-0.1.8/tests/test_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-03-15 13:17:09.446850 pvoutput-ocf-0.1.9/
+-rw-r--r--   0 runner    (1001) docker     (121)    11347 2022-03-15 13:16:49.000000 pvoutput-ocf-0.1.9/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (121)       14 2022-03-15 13:16:49.000000 pvoutput-ocf-0.1.9/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (121)     5988 2022-03-15 13:17:09.442850 pvoutput-ocf-0.1.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (121)     5777 2022-03-15 13:16:49.000000 pvoutput-ocf-0.1.9/README.md
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-03-15 13:17:09.442850 pvoutput-ocf-0.1.9/pvoutput/
+-rw-r--r--   0 runner    (1001) docker     (121)       43 2022-03-15 13:16:49.000000 pvoutput-ocf-0.1.9/pvoutput/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     6764 2022-03-15 13:16:49.000000 pvoutput-ocf-0.1.9/pvoutput/consts.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3718 2022-03-15 13:16:49.000000 pvoutput-ocf-0.1.9/pvoutput/daterange.py
+-rw-r--r--   0 runner    (1001) docker     (121)      631 2022-03-15 13:16:49.000000 pvoutput-ocf-0.1.9/pvoutput/exceptions.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-03-15 13:17:09.442850 pvoutput-ocf-0.1.9/pvoutput/grid_search/
+-rw-r--r--   0 runner    (1001) docker     (121)       36 2022-03-15 13:16:49.000000 pvoutput-ocf-0.1.9/pvoutput/grid_search/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     7785 2022-03-15 13:16:49.000000 pvoutput-ocf-0.1.9/pvoutput/grid_search/app.py
+-rw-r--r--   0 runner    (1001) docker     (121)     8895 2022-03-15 13:16:49.000000 pvoutput-ocf-0.1.9/pvoutput/grid_search/clip.py
+-rw-r--r--   0 runner    (1001) docker     (121)     9216 2022-03-15 13:16:49.000000 pvoutput-ocf-0.1.9/pvoutput/grid_search/grid_search.py
+-rw-r--r--   0 runner    (1001) docker     (121)     5425 2022-03-15 13:16:49.000000 pvoutput-ocf-0.1.9/pvoutput/grid_search/natural_earth.py
+-rw-r--r--   0 runner    (1001) docker     (121)    11253 2022-03-15 13:16:49.000000 pvoutput-ocf-0.1.9/pvoutput/mapscraper.py
+-rw-r--r--   0 runner    (1001) docker     (121)    46585 2022-03-15 13:16:49.000000 pvoutput-ocf-0.1.9/pvoutput/pvoutput.py
+-rw-r--r--   0 runner    (1001) docker     (121)     6499 2022-03-15 13:16:49.000000 pvoutput-ocf-0.1.9/pvoutput/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-03-15 13:17:09.442850 pvoutput-ocf-0.1.9/pvoutput_ocf.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (121)     5988 2022-03-15 13:17:09.000000 pvoutput-ocf-0.1.9/pvoutput_ocf.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (121)      703 2022-03-15 13:17:09.000000 pvoutput-ocf-0.1.9/pvoutput_ocf.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (121)        1 2022-03-15 13:17:09.000000 pvoutput-ocf-0.1.9/pvoutput_ocf.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (121)      130 2022-03-15 13:17:09.000000 pvoutput-ocf-0.1.9/pvoutput_ocf.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (121)       15 2022-03-15 13:17:09.000000 pvoutput-ocf-0.1.9/pvoutput_ocf.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (121)      130 2022-03-15 13:16:49.000000 pvoutput-ocf-0.1.9/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (121)       38 2022-03-15 13:17:09.446850 pvoutput-ocf-0.1.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (121)      568 2022-03-15 13:16:51.000000 pvoutput-ocf-0.1.9/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-03-15 13:17:09.442850 pvoutput-ocf-0.1.9/tests/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2022-03-15 13:16:49.000000 pvoutput-ocf-0.1.9/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1751 2022-03-15 13:16:49.000000 pvoutput-ocf-0.1.9/tests/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3699 2022-03-15 13:16:49.000000 pvoutput-ocf-0.1.9/tests/test_daterange.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2709 2022-03-15 13:16:49.000000 pvoutput-ocf-0.1.9/tests/test_grid_search.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2720 2022-03-15 13:16:49.000000 pvoutput-ocf-0.1.9/tests/test_mapscraper.py
+-rw-r--r--   0 runner    (1001) docker     (121)     4133 2022-03-15 13:16:49.000000 pvoutput-ocf-0.1.9/tests/test_pvoutput.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1516 2022-03-15 13:16:49.000000 pvoutput-ocf-0.1.9/tests/test_utils.py
```

### Comparing `pvoutput-ocf-0.1.8/LICENSE.txt` & `pvoutput-ocf-0.1.9/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `pvoutput-ocf-0.1.8/PKG-INFO` & `pvoutput-ocf-0.1.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pvoutput-ocf
-Version: 0.1.8
+Version: 0.1.9
 Summary: UNKNOWN
 Author-email: info@openclimatefix.org
 License: MIT
 Platform: UNKNOWN
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: pvoutput-ocf Version: 0.1.8 Summary: UNKNOWN
+Metadata-Version: 2.1 Name: pvoutput-ocf Version: 0.1.9 Summary: UNKNOWN
 Author-email: info@openclimatefix.org License: MIT Platform: UNKNOWN
 Description-Content-Type: text/markdown License-File: LICENSE.txt  [![All
 Contributors](https://img.shields.io/badge/all_contributors-7-
 orange.svg?style=flat-square)](#contributors-)  [![codecov](https://codecov.io/
 gh/openclimatefix/pvoutput/branch/main/graph/badge.svg?token=GTQDR2ZZ2S)]
 (https://codecov.io/gh/openclimatefix/pvoutput) Download historical solar
 photovoltaic data from [PVOutput.org](https://pvoutput.org). This code is a
```

### Comparing `pvoutput-ocf-0.1.8/README.md` & `pvoutput-ocf-0.1.9/README.md`

 * *Files identical despite different names*

### Comparing `pvoutput-ocf-0.1.8/pvoutput/consts.py` & `pvoutput-ocf-0.1.9/pvoutput/consts.py`

 * *Files identical despite different names*

### Comparing `pvoutput-ocf-0.1.8/pvoutput/daterange.py` & `pvoutput-ocf-0.1.9/pvoutput/daterange.py`

 * *Files identical despite different names*

### Comparing `pvoutput-ocf-0.1.8/pvoutput/exceptions.py` & `pvoutput-ocf-0.1.9/pvoutput/exceptions.py`

 * *Files identical despite different names*

### Comparing `pvoutput-ocf-0.1.8/pvoutput/grid_search/app.py` & `pvoutput-ocf-0.1.9/pvoutput/grid_search/app.py`

 * *Files identical despite different names*

### Comparing `pvoutput-ocf-0.1.8/pvoutput/grid_search/clip.py` & `pvoutput-ocf-0.1.9/pvoutput/grid_search/clip.py`

 * *Files identical despite different names*

### Comparing `pvoutput-ocf-0.1.8/pvoutput/grid_search/grid_search.py` & `pvoutput-ocf-0.1.9/pvoutput/grid_search/grid_search.py`

 * *Files identical despite different names*

### Comparing `pvoutput-ocf-0.1.8/pvoutput/grid_search/natural_earth.py` & `pvoutput-ocf-0.1.9/pvoutput/grid_search/natural_earth.py`

 * *Files identical despite different names*

### Comparing `pvoutput-ocf-0.1.8/pvoutput/mapscraper.py` & `pvoutput-ocf-0.1.9/pvoutput/mapscraper.py`

 * *Files identical despite different names*

### Comparing `pvoutput-ocf-0.1.8/pvoutput/pvoutput.py` & `pvoutput-ocf-0.1.9/pvoutput/pvoutput.py`

 * *Files 1% similar despite different names*

```diff
@@ -267,25 +267,25 @@
             dtype={col: np.float64 for col in columns},
         ).sort_index()
 
         return pv_system_status
 
     def get_system_status(
         self,
-        pv_system_id: List[int],
+        pv_system_ids: List[int],
         date: Union[str, datetime],
         **kwargs,
     ) -> pd.DataFrame:
         """Get Batch of PV system status (e.g. power generation) for one day, for multiple systems
 
         The returned DataFrame will be empty if the PVOutput API
         returns 'status 400: No status found'.
 
         Args:
-            pv_system_id: list of ints.
+            pv_system_ids: list of ints.
                 If you have a subscription service then multiple (up to 50)
                 pv systems status can be queries at once
             date: str in format YYYYMMDD; or datetime
                 (localtime of the PV system)
 
         Returns:
             pd.DataFrame:
@@ -295,20 +295,20 @@
                     instantaneous_power_gen_W,
                     cumulative_energy_gen_Wh,
                     instantaneous_power_gen_W,
                     energy_consumption_Wh",
                     temperature_C,
                     voltage,
         """
-        _LOG.info("system_id %d: Requesting batch system status for %s", pv_system_id, date)
+        _LOG.info(f"system_ids {pv_system_ids}: Requesting batch system status for %s", date)
         date = date_to_pvoutput_str(date)
         _check_date(date)
 
         # join the system ids with a column
-        all_pv_system_id = ",".join([str(idx) for idx in pv_system_id])
+        all_pv_system_id = ",".join([str(idx) for idx in pv_system_ids])
 
         api_params = {
             "dt": date,  # date, YYYYMMDD, localtime of the PV system
             "sid1": all_pv_system_id,  # SystemID.
         }
 
         try:
```

### Comparing `pvoutput-ocf-0.1.8/pvoutput/utils.py` & `pvoutput-ocf-0.1.9/pvoutput/utils.py`

 * *Files identical despite different names*

### Comparing `pvoutput-ocf-0.1.8/pvoutput_ocf.egg-info/PKG-INFO` & `pvoutput-ocf-0.1.9/pvoutput_ocf.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pvoutput-ocf
-Version: 0.1.8
+Version: 0.1.9
 Summary: UNKNOWN
 Author-email: info@openclimatefix.org
 License: MIT
 Platform: UNKNOWN
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: pvoutput-ocf Version: 0.1.8 Summary: UNKNOWN
+Metadata-Version: 2.1 Name: pvoutput-ocf Version: 0.1.9 Summary: UNKNOWN
 Author-email: info@openclimatefix.org License: MIT Platform: UNKNOWN
 Description-Content-Type: text/markdown License-File: LICENSE.txt  [![All
 Contributors](https://img.shields.io/badge/all_contributors-7-
 orange.svg?style=flat-square)](#contributors-)  [![codecov](https://codecov.io/
 gh/openclimatefix/pvoutput/branch/main/graph/badge.svg?token=GTQDR2ZZ2S)]
 (https://codecov.io/gh/openclimatefix/pvoutput) Download historical solar
 photovoltaic data from [PVOutput.org](https://pvoutput.org). This code is a
```

### Comparing `pvoutput-ocf-0.1.8/pvoutput_ocf.egg-info/SOURCES.txt` & `pvoutput-ocf-0.1.9/pvoutput_ocf.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pvoutput-ocf-0.1.8/setup.py` & `pvoutput-ocf-0.1.9/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 
 this_directory = Path(__file__).parent
 install_requires = (this_directory / "requirements.txt").read_text().splitlines()
 long_description = (this_directory / "README.md").read_text()
 
 setup(
     name="pvoutput-ocf",
-    version="0.1.8",
+    version="0.1.9",
     license="MIT",
     packages=find_packages(),
     install_requires=install_requires,
     long_description=long_description,
     long_description_content_type="text/markdown",
     company="Open Climate Fix Ltd",
     author_email="info@openclimatefix.org",
```

### Comparing `pvoutput-ocf-0.1.8/tests/conftest.py` & `pvoutput-ocf-0.1.9/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `pvoutput-ocf-0.1.8/tests/test_daterange.py` & `pvoutput-ocf-0.1.9/tests/test_daterange.py`

 * *Files identical despite different names*

### Comparing `pvoutput-ocf-0.1.8/tests/test_grid_search.py` & `pvoutput-ocf-0.1.9/tests/test_grid_search.py`

 * *Files identical despite different names*

### Comparing `pvoutput-ocf-0.1.8/tests/test_mapscraper.py` & `pvoutput-ocf-0.1.9/tests/test_mapscraper.py`

 * *Files identical despite different names*

### Comparing `pvoutput-ocf-0.1.8/tests/test_pvoutput.py` & `pvoutput-ocf-0.1.9/tests/test_pvoutput.py`

 * *Files identical despite different names*

### Comparing `pvoutput-ocf-0.1.8/tests/test_utils.py` & `pvoutput-ocf-0.1.9/tests/test_utils.py`

 * *Files identical despite different names*

