# Comparing `tmp/hkfdb-3.5.5.tar.gz` & `tmp/hkfdb-3.6.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hkfdb-3.5.5.tar", last modified: Fri Jun 23 00:20:31 2023, max compression
+gzip compressed data, was "hkfdb-3.6.1.tar", last modified: Wed Jul  5 09:03:40 2023, max compression
```

## Comparing `hkfdb-3.5.5.tar` & `hkfdb-3.6.1.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 cmw        (501) staff       (20)        0 2023-06-23 00:20:31.040716 hkfdb-3.5.5/
--rw-rw-rw-   0 cmw        (501) staff       (20)    35149 2021-07-30 00:33:11.000000 hkfdb-3.5.5/LICENSE
--rw-r--r--   0 cmw        (501) staff       (20)     1620 2023-06-23 00:20:31.040496 hkfdb-3.5.5/PKG-INFO
--rw-rw-rw-   0 cmw        (501) staff       (20)     1243 2023-03-30 03:29:25.000000 hkfdb-3.5.5/README.md
-drwxr-xr-x   0 cmw        (501) staff       (20)        0 2023-06-23 00:20:31.039079 hkfdb-3.5.5/hkfdb/
--rw-rw-rw-   0 cmw        (501) staff       (20)   108712 2023-06-23 00:19:39.000000 hkfdb-3.5.5/hkfdb/Database.py
--rw-rw-rw-   0 cmw        (501) staff       (20)       23 2021-09-12 13:30:45.000000 hkfdb-3.5.5/hkfdb/__init__.py
-drwxr-xr-x   0 cmw        (501) staff       (20)        0 2023-06-23 00:20:31.040186 hkfdb-3.5.5/hkfdb.egg-info/
--rw-rw-rw-   0 cmw        (501) staff       (20)     1620 2023-06-23 00:20:30.000000 hkfdb-3.5.5/hkfdb.egg-info/PKG-INFO
--rw-rw-rw-   0 cmw        (501) staff       (20)      206 2023-06-23 00:20:30.000000 hkfdb-3.5.5/hkfdb.egg-info/SOURCES.txt
--rw-rw-rw-   0 cmw        (501) staff       (20)        1 2023-06-23 00:20:30.000000 hkfdb-3.5.5/hkfdb.egg-info/dependency_links.txt
--rw-rw-rw-   0 cmw        (501) staff       (20)       51 2023-06-23 00:20:30.000000 hkfdb-3.5.5/hkfdb.egg-info/requires.txt
--rw-rw-rw-   0 cmw        (501) staff       (20)        6 2023-06-23 00:20:30.000000 hkfdb-3.5.5/hkfdb.egg-info/top_level.txt
--rw-r--r--   0 cmw        (501) staff       (20)       38 2023-06-23 00:20:31.040785 hkfdb-3.5.5/setup.cfg
--rw-rw-rw-   0 cmw        (501) staff       (20)      772 2023-06-23 00:20:18.000000 hkfdb-3.5.5/setup.py
+drwxr-xr-x   0 cmw        (501) staff       (20)        0 2023-07-05 09:03:40.199053 hkfdb-3.6.1/
+-rw-rw-rw-   0 cmw        (501) staff       (20)    35149 2021-07-30 00:33:11.000000 hkfdb-3.6.1/LICENSE
+-rw-r--r--   0 cmw        (501) staff       (20)     1620 2023-07-05 09:03:40.198657 hkfdb-3.6.1/PKG-INFO
+-rw-rw-rw-   0 cmw        (501) staff       (20)     1243 2023-03-30 03:29:25.000000 hkfdb-3.6.1/README.md
+drwxr-xr-x   0 cmw        (501) staff       (20)        0 2023-07-05 09:03:40.197147 hkfdb-3.6.1/hkfdb/
+-rw-rw-rw-   0 cmw        (501) staff       (20)   107552 2023-07-05 09:01:07.000000 hkfdb-3.6.1/hkfdb/Database.py
+-rw-rw-rw-   0 cmw        (501) staff       (20)       23 2021-09-12 13:30:45.000000 hkfdb-3.6.1/hkfdb/__init__.py
+drwxr-xr-x   0 cmw        (501) staff       (20)        0 2023-07-05 09:03:40.198377 hkfdb-3.6.1/hkfdb.egg-info/
+-rw-rw-rw-   0 cmw        (501) staff       (20)     1620 2023-07-05 09:03:39.000000 hkfdb-3.6.1/hkfdb.egg-info/PKG-INFO
+-rw-rw-rw-   0 cmw        (501) staff       (20)      206 2023-07-05 09:03:39.000000 hkfdb-3.6.1/hkfdb.egg-info/SOURCES.txt
+-rw-rw-rw-   0 cmw        (501) staff       (20)        1 2023-07-05 09:03:39.000000 hkfdb-3.6.1/hkfdb.egg-info/dependency_links.txt
+-rw-rw-rw-   0 cmw        (501) staff       (20)       51 2023-07-05 09:03:39.000000 hkfdb-3.6.1/hkfdb.egg-info/requires.txt
+-rw-rw-rw-   0 cmw        (501) staff       (20)        6 2023-07-05 09:03:39.000000 hkfdb-3.6.1/hkfdb.egg-info/top_level.txt
+-rw-r--r--   0 cmw        (501) staff       (20)       38 2023-07-05 09:03:40.199150 hkfdb-3.6.1/setup.cfg
+-rw-rw-rw-   0 cmw        (501) staff       (20)      772 2023-07-05 09:02:13.000000 hkfdb-3.6.1/setup.py
```

### Comparing `hkfdb-3.5.5/LICENSE` & `hkfdb-3.6.1/LICENSE`

 * *Files identical despite different names*

### Comparing `hkfdb-3.5.5/PKG-INFO` & `hkfdb-3.6.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hkfdb
-Version: 3.5.5
+Version: 3.6.1
 Summary: Hong Kong Finance Database.
 Home-page: https://www.hkfdb.net
 Author: Hong Kong Finance Database Team
 Author-email: info@hkfdb.net
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
```

### Comparing `hkfdb-3.5.5/README.md` & `hkfdb-3.6.1/README.md`

 * *Files identical despite different names*

### Comparing `hkfdb-3.5.5/hkfdb/Database.py` & `hkfdb-3.6.1/hkfdb/Database.py`

 * *Files 2% similar despite different names*

```diff
@@ -283,18 +283,14 @@
 
         if False not in list(check_bool_dict.values()):
 
             link_url = 'http://www.hkfdb.net/data_api?'
             token = str(self.authToken)
             start_date_str = str(start_date)
             end_date_str = str(end_date)
-            # end_date_str = str(end_date)[:4], str(end_date)[4:6]
-            # _, last_day = calendar.monthrange( int(str(end_date)[:4]), int(str(end_date)[4:6]))
-            # end_date_str = f'{str(end_date)[:4]}{str(end_date)[4:6]}{last_day}'
-            # print(start_date_str, end_date_str)
             link_str = f'{link_url}token={token}&database=hk_futures_ohlc&index={index}&freq={freq}&start_date={start_date_str}&end_date={end_date_str}'
             # print(link_str)
 
             response = requests.get(link_str)
             response_ok = response_check(response)
 
 
@@ -416,31 +412,17 @@
                     expiry_dates = list(df['expiry_date'].unique())
                     expiry_dates.sort()
                     # print(expiry_dates)
 
                     # Calculate roll diff
                     roll_diff_dict = {}
 
-                    df.to_csv('df.csv')
-
                     for expiry_date in expiry_dates:
 
                         try:
-
-
-                            # print(expiry_date)
-                            #
-                            # print(df[(df['expiry_date'] == expiry_date) &
-                            #                         (df['current_month_expiry_date_diff'] == rolling_day) &
-                            #                         (df['current_month'] == True)].sort_values(by=['datetime'], ascending=False))
-                            #
-                            # exact_rolling_date = df[(df['expiry_date'] == expiry_date) &
-                            #                         (df['current_month_expiry_date_diff'] == rolling_day) &
-                            #                         (df['current_month'] == True)].sort_values(by=['datetime'], ascending=False).reset_index(drop=True).reset_index(drop=True).at[0, 'date']
-
                             exact_rolling_date = df[(df['expiry_date'] == expiry_date) &
                                                     (df['current_month_expiry_date_diff'] == rolling_day) &
                                                     (df['current_month'] == True)].sort_values(by=['datetime'],
                                                                                                ascending=False).reset_index(
                                                                             drop=True).reset_index(drop=True).at[0, 'date']
                                 # Sorting Reverse because get later date to make sure it is RTH trading date
```

### Comparing `hkfdb-3.5.5/hkfdb.egg-info/PKG-INFO` & `hkfdb-3.6.1/hkfdb.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hkfdb
-Version: 3.5.5
+Version: 3.6.1
 Summary: Hong Kong Finance Database.
 Home-page: https://www.hkfdb.net
 Author: Hong Kong Finance Database Team
 Author-email: info@hkfdb.net
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
```

### Comparing `hkfdb-3.5.5/setup.py` & `hkfdb-3.6.1/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="hkfdb",
-    version="3.5.5",
+    version="3.6.1",
     author="Hong Kong Finance Database Team",
     author_email="info@hkfdb.net",
     description="Hong Kong Finance Database.",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://www.hkfdb.net",
     packages=setuptools.find_packages(),
```

