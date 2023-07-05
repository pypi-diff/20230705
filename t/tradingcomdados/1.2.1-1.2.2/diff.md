# Comparing `tmp/tradingcomdados-1.2.1.tar.gz` & `tmp/tradingcomdados-1.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tradingcomdados-1.2.1.tar", last modified: Sun Jul  2 18:18:24 2023, max compression
+gzip compressed data, was "tradingcomdados-1.2.2.tar", last modified: Wed Jul  5 01:16:39 2023, max compression
```

## Comparing `tradingcomdados-1.2.1.tar` & `tradingcomdados-1.2.2.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxrwxrwx   0        0        0        0 2023-07-02 18:18:23.974869 tradingcomdados-1.2.1/
--rw-rw-rw-   0        0        0     1702 2023-07-02 18:18:23.973869 tradingcomdados-1.2.1/PKG-INFO
--rw-rw-rw-   0        0        0     1500 2023-06-26 00:40:07.000000 tradingcomdados-1.2.1/README.md
--rw-rw-rw-   0        0        0      452 2023-07-02 18:17:22.000000 tradingcomdados-1.2.1/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-07-02 18:18:23.974869 tradingcomdados-1.2.1/setup.cfg
--rw-rw-rw-   0        0        0      627 2023-05-23 23:49:47.000000 tradingcomdados-1.2.1/setup.py
-drwxrwxrwx   0        0        0        0 2023-07-02 18:18:15.580250 tradingcomdados-1.2.1/tradingcomdados/
--rw-rw-rw-   0        0        0        0 2023-05-05 15:34:18.000000 tradingcomdados-1.2.1/tradingcomdados/__init__.py
--rw-rw-rw-   0        0        0     2080 2023-07-02 18:17:22.000000 tradingcomdados-1.2.1/tradingcomdados/alternative_data.py
--rw-rw-rw-   0        0        0    12204 2023-07-02 18:17:22.000000 tradingcomdados-1.2.1/tradingcomdados/data_provider.py
--rw-rw-rw-   0        0        0    37098 2023-07-02 18:17:22.000000 tradingcomdados-1.2.1/tradingcomdados/ta_indicators.py
--rw-rw-rw-   0        0        0     6347 2023-06-20 01:15:28.000000 tradingcomdados-1.2.1/tradingcomdados/unsupervised_learning.py
-drwxrwxrwx   0        0        0        0 2023-07-02 18:18:23.972869 tradingcomdados-1.2.1/tradingcomdados.egg-info/
--rw-rw-rw-   0        0        0     1702 2023-07-02 18:18:13.000000 tradingcomdados-1.2.1/tradingcomdados.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      398 2023-07-02 18:18:14.000000 tradingcomdados-1.2.1/tradingcomdados.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-02 18:18:13.000000 tradingcomdados-1.2.1/tradingcomdados.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      131 2023-07-02 18:18:13.000000 tradingcomdados-1.2.1/tradingcomdados.egg-info/requires.txt
--rw-rw-rw-   0        0        0       16 2023-07-02 18:18:13.000000 tradingcomdados-1.2.1/tradingcomdados.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-07-05 01:16:39.700714 tradingcomdados-1.2.2/
+-rw-rw-rw-   0        0        0     1702 2023-07-05 01:16:39.700714 tradingcomdados-1.2.2/PKG-INFO
+-rw-rw-rw-   0        0        0     1500 2023-06-26 00:40:07.000000 tradingcomdados-1.2.2/README.md
+-rw-rw-rw-   0        0        0      452 2023-07-05 01:14:34.000000 tradingcomdados-1.2.2/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-07-05 01:16:39.701711 tradingcomdados-1.2.2/setup.cfg
+-rw-rw-rw-   0        0        0      627 2023-05-23 23:49:47.000000 tradingcomdados-1.2.2/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-05 01:16:39.687712 tradingcomdados-1.2.2/tradingcomdados/
+-rw-rw-rw-   0        0        0        0 2023-05-05 15:34:18.000000 tradingcomdados-1.2.2/tradingcomdados/__init__.py
+-rw-rw-rw-   0        0        0     2080 2023-07-02 18:17:22.000000 tradingcomdados-1.2.2/tradingcomdados/alternative_data.py
+-rw-rw-rw-   0        0        0    11915 2023-07-05 01:13:25.000000 tradingcomdados-1.2.2/tradingcomdados/data_provider.py
+-rw-rw-rw-   0        0        0    37098 2023-07-02 18:17:22.000000 tradingcomdados-1.2.2/tradingcomdados/ta_indicators.py
+-rw-rw-rw-   0        0        0     6347 2023-06-20 01:15:28.000000 tradingcomdados-1.2.2/tradingcomdados/unsupervised_learning.py
+drwxrwxrwx   0        0        0        0 2023-07-05 01:16:39.699714 tradingcomdados-1.2.2/tradingcomdados.egg-info/
+-rw-rw-rw-   0        0        0     1702 2023-07-05 01:16:38.000000 tradingcomdados-1.2.2/tradingcomdados.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      398 2023-07-05 01:16:38.000000 tradingcomdados-1.2.2/tradingcomdados.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-05 01:16:38.000000 tradingcomdados-1.2.2/tradingcomdados.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      131 2023-07-05 01:16:38.000000 tradingcomdados-1.2.2/tradingcomdados.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       16 2023-07-05 01:16:38.000000 tradingcomdados-1.2.2/tradingcomdados.egg-info/top_level.txt
```

### Comparing `tradingcomdados-1.2.1/PKG-INFO` & `tradingcomdados-1.2.2/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tradingcomdados
-Version: 1.2.1
+Version: 1.2.2
 Summary: tradingcomdados
 Author: Lucas Roberto Correa
 License: UNKNOWN
 Platform: UNKNOWN
 Description-Content-Type: text/markdown
 
 # tradingcomdados
```

### Comparing `tradingcomdados-1.2.1/README.md` & `tradingcomdados-1.2.2/README.md`

 * *Files identical despite different names*

### Comparing `tradingcomdados-1.2.1/setup.py` & `tradingcomdados-1.2.2/setup.py`

 * *Files identical despite different names*

### Comparing `tradingcomdados-1.2.1/tradingcomdados/alternative_data.py` & `tradingcomdados-1.2.2/tradingcomdados/alternative_data.py`

 * *Files identical despite different names*

### Comparing `tradingcomdados-1.2.1/tradingcomdados/data_provider.py` & `tradingcomdados-1.2.2/tradingcomdados/data_provider.py`

 * *Files 4% similar despite different names*

```diff
@@ -47,33 +47,30 @@
                 "historical_data_bpa",
                 "historical_data_bpp",
                 "historical_data_dre",
                 "historical_data_dfc",
             ]
 
             if data_type == "stock" and request_type not in report_list:
-                params = {"ticker": ticker, "dataInicio": date_begin}
+                params = {
+                    "ticker": ticker,
+                    "dataInicio": date_begin,
+                    "dataFim": date_end,
+                }
 
             elif data_type == "treasury":
                 params = {"tamanho": "1000"}
 
             elif data_type == "treasury_historical":
                 params = {
                     "tamanho": "1000",
                     "dataInicio": date_begin,
                     "dataFim": date_end,
                 }
 
-            elif data_type == "stock" and request_type in report_list:
-                params = {
-                    "ticker": ticker,
-                    "ano": date_begin[0:4],
-                    "trimestre": "1",
-                }
-
             return params
 
         params = _ckeck_data_type(data_type)
         res = req.get(endpoint, headers=header, params=params).json()
 
         return res
 
@@ -102,18 +99,15 @@
             report_list = [
                 "historical_data_bpa",
                 "historical_data_bpp",
                 "historical_data_dre",
                 "historical_data_dfc",
             ]
 
-            if data_type == "stock" and request_type not in report_list:
-                params = {"ticker": ticker, "dataInicio": date_begin}
-
-            elif data_type == "stock" and request_type in report_list:
+            if data_type == "stock" and request_type in report_list:
                 params = {
                     "ticker": ticker,
                     "ano": date_begin[0:4],
                     "trimestre": trimester,
                 }
 
             return params
```

### Comparing `tradingcomdados-1.2.1/tradingcomdados/ta_indicators.py` & `tradingcomdados-1.2.2/tradingcomdados/ta_indicators.py`

 * *Files identical despite different names*

### Comparing `tradingcomdados-1.2.1/tradingcomdados/unsupervised_learning.py` & `tradingcomdados-1.2.2/tradingcomdados/unsupervised_learning.py`

 * *Files identical despite different names*

### Comparing `tradingcomdados-1.2.1/tradingcomdados.egg-info/PKG-INFO` & `tradingcomdados-1.2.2/tradingcomdados.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tradingcomdados
-Version: 1.2.1
+Version: 1.2.2
 Summary: tradingcomdados
 Author: Lucas Roberto Correa
 License: UNKNOWN
 Platform: UNKNOWN
 Description-Content-Type: text/markdown
 
 # tradingcomdados
```

