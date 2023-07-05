# Comparing `tmp/fabcohort-0.2.4.tar.gz` & `tmp/fabcohort-0.2.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fabcohort-0.2.4.tar", last modified: Wed Jul  5 13:17:58 2023, max compression
+gzip compressed data, was "fabcohort-0.2.5.tar", last modified: Wed Jul  5 13:22:50 2023, max compression
```

## Comparing `fabcohort-0.2.4.tar` & `fabcohort-0.2.5.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxr-xr-x   0 linliding   (501) staff       (20)        0 2023-07-05 13:17:58.929837 fabcohort-0.2.4/
--rw-r--r--   0 linliding   (501) staff       (20)     2527 2023-07-05 13:17:58.929673 fabcohort-0.2.4/PKG-INFO
--rw-r--r--   0 linliding   (501) staff       (20)     1836 2023-05-25 16:00:55.000000 fabcohort-0.2.4/README.md
-drwxr-xr-x   0 linliding   (501) staff       (20)        0 2023-07-05 13:17:58.928711 fabcohort-0.2.4/fab_cohort/
--rw-r--r--   0 linliding   (501) staff       (20)       36 2023-05-18 20:24:44.000000 fabcohort-0.2.4/fab_cohort/__init__.py
--rw-r--r--   0 linliding   (501) staff       (20)     4937 2023-07-05 13:16:58.000000 fabcohort-0.2.4/fab_cohort/cohort.py
-drwxr-xr-x   0 linliding   (501) staff       (20)        0 2023-07-05 13:17:58.929480 fabcohort-0.2.4/fabcohort.egg-info/
--rw-r--r--   0 linliding   (501) staff       (20)     2527 2023-07-05 13:17:58.000000 fabcohort-0.2.4/fabcohort.egg-info/PKG-INFO
--rw-r--r--   0 linliding   (501) staff       (20)      226 2023-07-05 13:17:58.000000 fabcohort-0.2.4/fabcohort.egg-info/SOURCES.txt
--rw-r--r--   0 linliding   (501) staff       (20)        1 2023-07-05 13:17:58.000000 fabcohort-0.2.4/fabcohort.egg-info/dependency_links.txt
--rw-r--r--   0 linliding   (501) staff       (20)       13 2023-07-05 13:17:58.000000 fabcohort-0.2.4/fabcohort.egg-info/requires.txt
--rw-r--r--   0 linliding   (501) staff       (20)       11 2023-07-05 13:17:58.000000 fabcohort-0.2.4/fabcohort.egg-info/top_level.txt
--rw-r--r--   0 linliding   (501) staff       (20)       38 2023-07-05 13:17:58.929888 fabcohort-0.2.4/setup.cfg
--rw-r--r--   0 linliding   (501) staff       (20)     1293 2023-07-05 13:16:52.000000 fabcohort-0.2.4/setup.py
+drwxr-xr-x   0 linliding   (501) staff       (20)        0 2023-07-05 13:22:50.043326 fabcohort-0.2.5/
+-rw-r--r--   0 linliding   (501) staff       (20)     2569 2023-07-05 13:22:50.043167 fabcohort-0.2.5/PKG-INFO
+-rw-r--r--   0 linliding   (501) staff       (20)     1878 2023-07-05 13:22:26.000000 fabcohort-0.2.5/README.md
+drwxr-xr-x   0 linliding   (501) staff       (20)        0 2023-07-05 13:22:50.042252 fabcohort-0.2.5/fab_cohort/
+-rw-r--r--   0 linliding   (501) staff       (20)       36 2023-05-18 20:24:44.000000 fabcohort-0.2.5/fab_cohort/__init__.py
+-rw-r--r--   0 linliding   (501) staff       (20)     4953 2023-07-05 13:21:02.000000 fabcohort-0.2.5/fab_cohort/cohort.py
+drwxr-xr-x   0 linliding   (501) staff       (20)        0 2023-07-05 13:22:50.042972 fabcohort-0.2.5/fabcohort.egg-info/
+-rw-r--r--   0 linliding   (501) staff       (20)     2569 2023-07-05 13:22:50.000000 fabcohort-0.2.5/fabcohort.egg-info/PKG-INFO
+-rw-r--r--   0 linliding   (501) staff       (20)      226 2023-07-05 13:22:50.000000 fabcohort-0.2.5/fabcohort.egg-info/SOURCES.txt
+-rw-r--r--   0 linliding   (501) staff       (20)        1 2023-07-05 13:22:50.000000 fabcohort-0.2.5/fabcohort.egg-info/dependency_links.txt
+-rw-r--r--   0 linliding   (501) staff       (20)       13 2023-07-05 13:22:50.000000 fabcohort-0.2.5/fabcohort.egg-info/requires.txt
+-rw-r--r--   0 linliding   (501) staff       (20)       11 2023-07-05 13:22:50.000000 fabcohort-0.2.5/fabcohort.egg-info/top_level.txt
+-rw-r--r--   0 linliding   (501) staff       (20)       38 2023-07-05 13:22:50.043379 fabcohort-0.2.5/setup.cfg
+-rw-r--r--   0 linliding   (501) staff       (20)     1293 2023-07-05 13:22:38.000000 fabcohort-0.2.5/setup.py
```

### Comparing `fabcohort-0.2.4/PKG-INFO` & `fabcohort-0.2.5/PKG-INFO`

 * *Files 19% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fabcohort
-Version: 0.2.4
+Version: 0.2.5
 Summary: for cohort analysis
 Home-page: https://github.com/linliD/fabcohort/
 Author: Linli Ding
 Author-email: linli@joinbonnet.com
 License: MIT
 Platform: UNKNOWN
 Classifier: Intended Audience :: Developers
@@ -15,82 +15,89 @@
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
 
 # fabcohort
+
 A small demo library for a fab_cohort about cohort analysis
 
 ### Installation
+
 ```
 pip install fabcohort
 ```
 
 ### Get started
+
 How to do cohort analysis with this lib:
 
-#### **FUNCTION1**: 
-Vanilla cohort analysis 
+#### **FUNCTION1**:
+
+Vanilla cohort analysis
 
-Pandas df.head(5) should look like - 
+Pandas df.head(5) should look like -
 | user_id | date | count |
 | -------- | -------- | -------- |
-| 5fb507360cd5c0   | 2023-04-01   | 1   |
-| weg507360cwfw3   | 2023-03-01   | 1   |
-| 6001ef966c13w3   | 2023-02-01   | 1   |
-| weg507360cwfw3   | 2023-04-01   | 1   |
-| 6001ef966c13w3   | 2023-03-01   | 1   |
+| 5fb507360cd5c0 | 2023-04-01 | 1 |
+| weg507360cwfw3 | 2023-03-01 | 1 |
+| 6001ef966c13w3 | 2023-02-01 | 1 |
+| weg507360cwfw3 | 2023-04-01 | 1 |
+| 6001ef966c13w3 | 2023-03-01 | 1 |
 
 ```Python
 from fab_cohort import Cohort
 
 # Instantiate a Cohort object
 cohort = Cohort()
 
-# Call the count_cohort method
-result = cohort.count_cohort(df)
+# Call the count_cohort method, e.g., MS for month start, WS for week start
+result = cohort.count_cohort(df, frequency)
 
 ```
 
-#### **FUNCTION2**: 
+#### **FUNCTION2**:
+
 Cohort analysis by segments
 
-Pandas df.head(5) should look like - 
+Pandas df.head(5) should look like -
 | user_id | date | segment | count |
 | -------- | -------- | -------- | -------- |
-| 5fb507360cd5c0   | 2023-04-01   | A,B   | 1   |
-| weg507360cwfw3   | 2023-03-01   | A,    | 1   |
-| 6001ef966c13w3   | 2023-02-01   | C,D   | 1   |
-| weg507360cwfw3   | 2023-04-01   | B,D   | 1   |
-| 6001ef966c13w3   | 2023-03-01   | A,B   | 1   |
+| 5fb507360cd5c0 | 2023-04-01 | A,B | 1 |
+| weg507360cwfw3 | 2023-03-01 | A, | 1 |
+| 6001ef966c13w3 | 2023-02-01 | C,D | 1 |
+| weg507360cwfw3 | 2023-04-01 | B,D | 1 |
+| 6001ef966c13w3 | 2023-03-01 | A,B | 1 |
 
 ```Python
 from fab_cohort import Cohort
 
 # Instantiate a Cohort object
 cohort = Cohort()
 
-# Call the count_cohort_segments method
-result = cohort.count_cohort_segments(df)
+# Call the count_cohort_segments method, e.g., MS for month start, WS for week start
+result = cohort.count_cohort_segments(df, frequency)
 
 # (Optional) if you have multiple segments just parse it
 result[['segment1', 'segment2']] = result['segment'].str.split(',', expand=True)
 result.drop('segment', axis=1, inplace=True)
 
 ```
 
-#### **FUNCTION3**: 
+#### **FUNCTION3**:
+
 Convert the count to percentage
 
 ```Python
 # once the above result is obtained
 
 # Call the count_cohort method
 result_pct = cohort.to_pct(result)
 
 # (Optional) if you have multiple segments just parse it
 result[['segment1', 'segment2']] = result['segment'].str.split(',', expand=True)
 result.drop('segment', axis=1, inplace=True)
 
 ```
 
+
```

### Comparing `fabcohort-0.2.4/README.md` & `fabcohort-0.2.5/README.md`

 * *Files 27% similar despite different names*

```diff
@@ -1,75 +1,81 @@
 # fabcohort
+
 A small demo library for a fab_cohort about cohort analysis
 
 ### Installation
+
 ```
 pip install fabcohort
 ```
 
 ### Get started
+
 How to do cohort analysis with this lib:
 
-#### **FUNCTION1**: 
-Vanilla cohort analysis 
+#### **FUNCTION1**:
+
+Vanilla cohort analysis
 
-Pandas df.head(5) should look like - 
+Pandas df.head(5) should look like -
 | user_id | date | count |
 | -------- | -------- | -------- |
-| 5fb507360cd5c0   | 2023-04-01   | 1   |
-| weg507360cwfw3   | 2023-03-01   | 1   |
-| 6001ef966c13w3   | 2023-02-01   | 1   |
-| weg507360cwfw3   | 2023-04-01   | 1   |
-| 6001ef966c13w3   | 2023-03-01   | 1   |
+| 5fb507360cd5c0 | 2023-04-01 | 1 |
+| weg507360cwfw3 | 2023-03-01 | 1 |
+| 6001ef966c13w3 | 2023-02-01 | 1 |
+| weg507360cwfw3 | 2023-04-01 | 1 |
+| 6001ef966c13w3 | 2023-03-01 | 1 |
 
 ```Python
 from fab_cohort import Cohort
 
 # Instantiate a Cohort object
 cohort = Cohort()
 
-# Call the count_cohort method
-result = cohort.count_cohort(df)
+# Call the count_cohort method, e.g., MS for month start, WS for week start
+result = cohort.count_cohort(df, frequency)
 
 ```
 
-#### **FUNCTION2**: 
+#### **FUNCTION2**:
+
 Cohort analysis by segments
 
-Pandas df.head(5) should look like - 
+Pandas df.head(5) should look like -
 | user_id | date | segment | count |
 | -------- | -------- | -------- | -------- |
-| 5fb507360cd5c0   | 2023-04-01   | A,B   | 1   |
-| weg507360cwfw3   | 2023-03-01   | A,    | 1   |
-| 6001ef966c13w3   | 2023-02-01   | C,D   | 1   |
-| weg507360cwfw3   | 2023-04-01   | B,D   | 1   |
-| 6001ef966c13w3   | 2023-03-01   | A,B   | 1   |
+| 5fb507360cd5c0 | 2023-04-01 | A,B | 1 |
+| weg507360cwfw3 | 2023-03-01 | A, | 1 |
+| 6001ef966c13w3 | 2023-02-01 | C,D | 1 |
+| weg507360cwfw3 | 2023-04-01 | B,D | 1 |
+| 6001ef966c13w3 | 2023-03-01 | A,B | 1 |
 
 ```Python
 from fab_cohort import Cohort
 
 # Instantiate a Cohort object
 cohort = Cohort()
 
-# Call the count_cohort_segments method
-result = cohort.count_cohort_segments(df)
+# Call the count_cohort_segments method, e.g., MS for month start, WS for week start
+result = cohort.count_cohort_segments(df, frequency)
 
 # (Optional) if you have multiple segments just parse it
 result[['segment1', 'segment2']] = result['segment'].str.split(',', expand=True)
 result.drop('segment', axis=1, inplace=True)
 
 ```
 
-#### **FUNCTION3**: 
+#### **FUNCTION3**:
+
 Convert the count to percentage
 
 ```Python
 # once the above result is obtained
 
 # Call the count_cohort method
 result_pct = cohort.to_pct(result)
 
 # (Optional) if you have multiple segments just parse it
 result[['segment1', 'segment2']] = result['segment'].str.split(',', expand=True)
 result.drop('segment', axis=1, inplace=True)
 
-```
+```
```

### Comparing `fabcohort-0.2.4/fab_cohort/cohort.py` & `fabcohort-0.2.5/fab_cohort/cohort.py`

 * *Files 2% similar despite different names*

```diff
@@ -36,17 +36,17 @@
 
         result = df_cont_created.groupby(['created', 'cohort']).size().reset_index(name='count')
 
         return result
     
     # for calculating the cohort filter by segments in the front-end
     @staticmethod
-    def count_cohort_segments(df):
+    def count_cohort_segments(df, frequency):
         # Generate continuous time series
-        time_series = pd.date_range(start=min(df['date']), end=max(df['date']), freq='MS')
+        time_series = pd.date_range(start=min(df['date']), end=max(df['date']), freq=frequency)
         time_series_df = pd.DataFrame({'date': time_series})
 
         # Get unique user_id values from df
         unique_user_ids = df['user_id'].unique()
         unique_user_ids_df = pd.DataFrame({'user_id': unique_user_ids})
 
         # Get unique segments
```

### Comparing `fabcohort-0.2.4/fabcohort.egg-info/PKG-INFO` & `fabcohort-0.2.5/fabcohort.egg-info/PKG-INFO`

 * *Files 19% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fabcohort
-Version: 0.2.4
+Version: 0.2.5
 Summary: for cohort analysis
 Home-page: https://github.com/linliD/fabcohort/
 Author: Linli Ding
 Author-email: linli@joinbonnet.com
 License: MIT
 Platform: UNKNOWN
 Classifier: Intended Audience :: Developers
@@ -15,82 +15,89 @@
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
 
 # fabcohort
+
 A small demo library for a fab_cohort about cohort analysis
 
 ### Installation
+
 ```
 pip install fabcohort
 ```
 
 ### Get started
+
 How to do cohort analysis with this lib:
 
-#### **FUNCTION1**: 
-Vanilla cohort analysis 
+#### **FUNCTION1**:
+
+Vanilla cohort analysis
 
-Pandas df.head(5) should look like - 
+Pandas df.head(5) should look like -
 | user_id | date | count |
 | -------- | -------- | -------- |
-| 5fb507360cd5c0   | 2023-04-01   | 1   |
-| weg507360cwfw3   | 2023-03-01   | 1   |
-| 6001ef966c13w3   | 2023-02-01   | 1   |
-| weg507360cwfw3   | 2023-04-01   | 1   |
-| 6001ef966c13w3   | 2023-03-01   | 1   |
+| 5fb507360cd5c0 | 2023-04-01 | 1 |
+| weg507360cwfw3 | 2023-03-01 | 1 |
+| 6001ef966c13w3 | 2023-02-01 | 1 |
+| weg507360cwfw3 | 2023-04-01 | 1 |
+| 6001ef966c13w3 | 2023-03-01 | 1 |
 
 ```Python
 from fab_cohort import Cohort
 
 # Instantiate a Cohort object
 cohort = Cohort()
 
-# Call the count_cohort method
-result = cohort.count_cohort(df)
+# Call the count_cohort method, e.g., MS for month start, WS for week start
+result = cohort.count_cohort(df, frequency)
 
 ```
 
-#### **FUNCTION2**: 
+#### **FUNCTION2**:
+
 Cohort analysis by segments
 
-Pandas df.head(5) should look like - 
+Pandas df.head(5) should look like -
 | user_id | date | segment | count |
 | -------- | -------- | -------- | -------- |
-| 5fb507360cd5c0   | 2023-04-01   | A,B   | 1   |
-| weg507360cwfw3   | 2023-03-01   | A,    | 1   |
-| 6001ef966c13w3   | 2023-02-01   | C,D   | 1   |
-| weg507360cwfw3   | 2023-04-01   | B,D   | 1   |
-| 6001ef966c13w3   | 2023-03-01   | A,B   | 1   |
+| 5fb507360cd5c0 | 2023-04-01 | A,B | 1 |
+| weg507360cwfw3 | 2023-03-01 | A, | 1 |
+| 6001ef966c13w3 | 2023-02-01 | C,D | 1 |
+| weg507360cwfw3 | 2023-04-01 | B,D | 1 |
+| 6001ef966c13w3 | 2023-03-01 | A,B | 1 |
 
 ```Python
 from fab_cohort import Cohort
 
 # Instantiate a Cohort object
 cohort = Cohort()
 
-# Call the count_cohort_segments method
-result = cohort.count_cohort_segments(df)
+# Call the count_cohort_segments method, e.g., MS for month start, WS for week start
+result = cohort.count_cohort_segments(df, frequency)
 
 # (Optional) if you have multiple segments just parse it
 result[['segment1', 'segment2']] = result['segment'].str.split(',', expand=True)
 result.drop('segment', axis=1, inplace=True)
 
 ```
 
-#### **FUNCTION3**: 
+#### **FUNCTION3**:
+
 Convert the count to percentage
 
 ```Python
 # once the above result is obtained
 
 # Call the count_cohort method
 result_pct = cohort.to_pct(result)
 
 # (Optional) if you have multiple segments just parse it
 result[['segment1', 'segment2']] = result['segment'].str.split(',', expand=True)
 result.drop('segment', axis=1, inplace=True)
 
 ```
 
+
```

### Comparing `fabcohort-0.2.4/setup.py` & `fabcohort-0.2.5/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 # Get the long description from the README file
 with open(path.join(HERE, 'README.md'), encoding='utf-8') as f:
     long_description = f.read()
 
 # This call to setup() does all the work
 setup(
     name="fabcohort",
-    version="0.2.4",
+    version="0.2.5",
     description="for cohort analysis",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/linliD/fabcohort/",
     author="Linli Ding",
     author_email="linli@joinbonnet.com",
     license="MIT",
```

