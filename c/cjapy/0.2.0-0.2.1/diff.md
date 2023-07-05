# Comparing `tmp/cjapy-0.2.0.tar.gz` & `tmp/cjapy-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cjapy-0.2.0.tar", last modified: Mon Jun 26 14:07:28 2023, max compression
+gzip compressed data, was "cjapy-0.2.1.tar", last modified: Wed Jul  5 20:21:31 2023, max compression
```

## Comparing `cjapy-0.2.0.tar` & `cjapy-0.2.1.tar`

### file list

```diff
@@ -1,35 +1,35 @@
-drwxrwxrwx   0        0        0        0 2023-06-26 14:07:28.419361 cjapy-0.2.0/
--rw-rw-rw-   0        0        0    10337 2021-10-20 19:50:41.000000 cjapy-0.2.0/LICENSE
--rw-rw-rw-   0        0        0     3565 2023-06-26 14:07:28.416364 cjapy-0.2.0/PKG-INFO
--rw-rw-rw-   0        0        0     2469 2021-11-08 18:46:39.000000 cjapy-0.2.0/README.md
-drwxrwxrwx   0        0        0        0 2023-06-26 14:07:28.148988 cjapy-0.2.0/cjapy/
--rw-rw-rw-   0        0        0      107 2021-10-20 19:50:41.000000 cjapy-0.2.0/cjapy/__init__.py
--rw-rw-rw-   0        0        0       23 2023-06-26 06:51:12.000000 cjapy-0.2.0/cjapy/__version__.py
--rw-rw-rw-   0        0        0   109066 2023-05-11 12:56:12.000000 cjapy-0.2.0/cjapy/cjapy.py
--rw-rw-rw-   0        0        0      566 2023-06-26 06:55:22.000000 cjapy-0.2.0/cjapy/config.py
--rw-rw-rw-   0        0        0     7666 2023-06-26 06:48:55.000000 cjapy-0.2.0/cjapy/configs.py
--rw-rw-rw-   0        0        0    12662 2023-06-26 09:12:19.000000 cjapy-0.2.0/cjapy/connector.py
--rw-rw-rw-   0        0        0    12007 2021-11-08 18:46:39.000000 cjapy-0.2.0/cjapy/projects.py
--rw-rw-rw-   0        0        0    16716 2023-05-11 12:56:12.000000 cjapy-0.2.0/cjapy/requestCreator.py
--rw-rw-rw-   0        0        0     3463 2023-06-26 09:22:08.000000 cjapy-0.2.0/cjapy/token_provider.py
--rw-rw-rw-   0        0        0     9362 2023-05-11 12:56:12.000000 cjapy-0.2.0/cjapy/workspace.py
-drwxrwxrwx   0        0        0        0 2023-06-26 14:07:28.213750 cjapy-0.2.0/cjapy.egg-info/
--rw-rw-rw-   0        0        0     3565 2023-06-26 14:07:27.000000 cjapy-0.2.0/cjapy.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      576 2023-06-26 14:07:27.000000 cjapy-0.2.0/cjapy.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-26 14:07:27.000000 cjapy-0.2.0/cjapy.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       79 2023-06-26 14:07:27.000000 cjapy-0.2.0/cjapy.egg-info/requires.txt
--rw-rw-rw-   0        0        0        6 2023-06-26 14:07:27.000000 cjapy-0.2.0/cjapy.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2023-06-26 14:07:28.410864 cjapy-0.2.0/docs/
--rw-rw-rw-   0        0        0     1805 2021-10-20 19:50:41.000000 cjapy-0.2.0/docs/authenticating_without_config_json.md
--rw-rw-rw-   0        0        0    27971 2023-05-11 12:56:12.000000 cjapy-0.2.0/docs/cja.md
--rw-rw-rw-   0        0        0     3664 2023-06-26 06:49:51.000000 cjapy-0.2.0/docs/getting_started.md
--rw-rw-rw-   0        0        0     3934 2021-10-20 19:50:41.000000 cjapy-0.2.0/docs/logging.md
--rw-rw-rw-   0        0        0     3335 2021-10-20 19:50:41.000000 cjapy-0.2.0/docs/main.md
--rw-rw-rw-   0        0        0     8595 2021-11-08 18:46:39.000000 cjapy-0.2.0/docs/projects.md
--rw-rw-rw-   0        0        0     1214 2023-06-26 14:06:41.000000 cjapy-0.2.0/docs/releases.md
--rw-rw-rw-   0        0        0     6126 2021-11-08 18:46:39.000000 cjapy-0.2.0/docs/requestCreator.md
--rw-rw-rw-   0        0        0     3348 2021-10-20 19:50:41.000000 cjapy-0.2.0/docs/workspace.md
--rw-rw-rw-   0        0        0     1364 2023-06-26 13:49:26.000000 cjapy-0.2.0/pyproject.toml
--rw-rw-rw-   0        0        0      100 2021-10-20 19:50:41.000000 cjapy-0.2.0/requirements.txt
--rw-rw-rw-   0        0        0       42 2023-06-26 14:07:28.427339 cjapy-0.2.0/setup.cfg
--rw-rw-rw-   0        0        0     1871 2021-10-20 19:50:41.000000 cjapy-0.2.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-05 20:21:31.350092 cjapy-0.2.1/
+-rw-rw-rw-   0        0        0    10337 2021-10-20 19:50:41.000000 cjapy-0.2.1/LICENSE
+-rw-rw-rw-   0        0        0     3565 2023-07-05 20:21:31.348097 cjapy-0.2.1/PKG-INFO
+-rw-rw-rw-   0        0        0     2469 2021-11-08 18:46:39.000000 cjapy-0.2.1/README.md
+drwxrwxrwx   0        0        0        0 2023-07-05 20:21:31.307878 cjapy-0.2.1/cjapy/
+-rw-rw-rw-   0        0        0      107 2021-10-20 19:50:41.000000 cjapy-0.2.1/cjapy/__init__.py
+-rw-rw-rw-   0        0        0       23 2023-07-05 06:14:05.000000 cjapy-0.2.1/cjapy/__version__.py
+-rw-rw-rw-   0        0        0   109187 2023-07-05 09:31:15.000000 cjapy-0.2.1/cjapy/cjapy.py
+-rw-rw-rw-   0        0        0      566 2023-06-26 06:55:22.000000 cjapy-0.2.1/cjapy/config.py
+-rw-rw-rw-   0        0        0     7666 2023-06-26 06:48:55.000000 cjapy-0.2.1/cjapy/configs.py
+-rw-rw-rw-   0        0        0    12821 2023-07-05 07:30:15.000000 cjapy-0.2.1/cjapy/connector.py
+-rw-rw-rw-   0        0        0    12007 2021-11-08 18:46:39.000000 cjapy-0.2.1/cjapy/projects.py
+-rw-rw-rw-   0        0        0    17279 2023-07-05 07:30:01.000000 cjapy-0.2.1/cjapy/requestCreator.py
+-rw-rw-rw-   0        0        0     3463 2023-06-26 09:22:08.000000 cjapy-0.2.1/cjapy/token_provider.py
+-rw-rw-rw-   0        0        0     9415 2023-07-05 06:15:53.000000 cjapy-0.2.1/cjapy/workspace.py
+drwxrwxrwx   0        0        0        0 2023-07-05 20:21:31.320064 cjapy-0.2.1/cjapy.egg-info/
+-rw-rw-rw-   0        0        0     3565 2023-07-05 20:21:31.000000 cjapy-0.2.1/cjapy.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      576 2023-07-05 20:21:31.000000 cjapy-0.2.1/cjapy.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-05 20:21:31.000000 cjapy-0.2.1/cjapy.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       79 2023-07-05 20:21:31.000000 cjapy-0.2.1/cjapy.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        6 2023-07-05 20:21:31.000000 cjapy-0.2.1/cjapy.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-07-05 20:21:31.346386 cjapy-0.2.1/docs/
+-rw-rw-rw-   0        0        0     1805 2021-10-20 19:50:41.000000 cjapy-0.2.1/docs/authenticating_without_config_json.md
+-rw-rw-rw-   0        0        0    27971 2023-05-11 12:56:12.000000 cjapy-0.2.1/docs/cja.md
+-rw-rw-rw-   0        0        0     3664 2023-06-26 06:49:51.000000 cjapy-0.2.1/docs/getting_started.md
+-rw-rw-rw-   0        0        0     3934 2021-10-20 19:50:41.000000 cjapy-0.2.1/docs/logging.md
+-rw-rw-rw-   0        0        0     3335 2021-10-20 19:50:41.000000 cjapy-0.2.1/docs/main.md
+-rw-rw-rw-   0        0        0     8595 2021-11-08 18:46:39.000000 cjapy-0.2.1/docs/projects.md
+-rw-rw-rw-   0        0        0     1477 2023-07-05 07:15:10.000000 cjapy-0.2.1/docs/releases.md
+-rw-rw-rw-   0        0        0     6126 2021-11-08 18:46:39.000000 cjapy-0.2.1/docs/requestCreator.md
+-rw-rw-rw-   0        0        0     3348 2021-10-20 19:50:41.000000 cjapy-0.2.1/docs/workspace.md
+-rw-rw-rw-   0        0        0     1364 2023-06-26 13:49:26.000000 cjapy-0.2.1/pyproject.toml
+-rw-rw-rw-   0        0        0      100 2021-10-20 19:50:41.000000 cjapy-0.2.1/requirements.txt
+-rw-rw-rw-   0        0        0       42 2023-07-05 20:21:31.350092 cjapy-0.2.1/setup.cfg
+-rw-rw-rw-   0        0        0     1871 2021-10-20 19:50:41.000000 cjapy-0.2.1/setup.py
```

### Comparing `cjapy-0.2.0/LICENSE` & `cjapy-0.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `cjapy-0.2.0/PKG-INFO` & `cjapy-0.2.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cjapy
-Version: 0.2.0
+Version: 0.2.1
 Summary: Adobe Customer Journey Analytics (CJA) wrapper
 Home-page: https://github.com/pitchmuc/cjapy
 Author: Julien Piccini
 Author-email: Julien Piccini <piccini.julien@gmail.com>
 License: Apache License 2.0
 Project-URL: homepage, https://github.com/pitchmuc/cjapy
 Project-URL: changelog, https://github.com/pitchmuc/cjapy/blob/master/docs/releases.md
```

### Comparing `cjapy-0.2.0/README.md` & `cjapy-0.2.1/README.md`

 * *Files identical despite different names*

### Comparing `cjapy-0.2.0/cjapy/cjapy.py` & `cjapy-0.2.1/cjapy/cjapy.py`

 * *Files 0% similar despite different names*

```diff
@@ -1962,19 +1962,19 @@
                     obj["id"]: obj["segmentId"]
                     for obj in dataRequest["metricContainer"]["metricFilters"]
                     if obj["id"].startswith("STATIC_ROW_COMPONENT")
                 }
         else:
             tableSegmentsRows = {
                 obj["id"]: obj["segmentId"]
-                for obj in dataRequest["metricContainer"]["metricFilters"]
+                for obj in dataRequest["metricContainer"].get("metricFilters",[])
             }
         ## retrieve place and segmentID
         segmentApplied = {}
-        for obj in dataRequest["metricContainer"]["metricFilters"]:
+        for obj in dataRequest["metricContainer"].get("metricFilters",[]):
             if obj["id"].startswith("STATIC_ROW") == False:
                 if obj["type"] == "breakdown":
                     segmentApplied[obj["id"]] = f"{obj['dimension']}:::{obj['itemId']}"
                 elif obj["type"] == "segment":
                     segmentApplied[obj["id"]] = obj["segmentId"]
                 elif obj["type"] == "dateRange":
                     segmentApplied[obj["id"]] = obj["dateRange"]
@@ -2063,15 +2063,15 @@
             "allowRemoteLoad": allowRemoteLoad,
             "useCache": useCache,
             "useResultsCache": useResultsCache,
             "includeOberonXml": includeOberonXml,
             "includePlatformPredictiveObjects": includePredictiveObjects,
         }
         if type(request) == dict:
-            dataRequest = request
+            dataRequest = deepcopy(request)
         elif type(request) == RequestCreator:
             dataRequest = request.to_dict()
         elif ".json" in request:
             with open(request, "r") as f:
                 dataRequest = json.load(f)
         else:
             raise ValueError("Require a JSON or Dictionary to request data")
@@ -2153,14 +2153,16 @@
                 metricFilterTranslation[filterId] = filterValue
             metricColumns = {}
             for colId in columnIdRelations.keys():
                 metricColumns[colId] = columnIdRelations[colId]
                 for element in filterRelations.get(colId, []):
                     metricColumns[colId] += f":::{metricFilterTranslation[element]}"
         else:
+            if 'error-504' in res.keys():
+                raise TimeoutError(res['error-504'])
             if returnClass == False:
                 return res
             reportType = "static"
             if self.loggingEnabled:
                 self.logger.debug(f"reportType: {reportType}")
             columns = None  ## no "columns" key in response
             summaryData = res.get("summaryData")
```

### Comparing `cjapy-0.2.0/cjapy/config.py` & `cjapy-0.2.1/cjapy/config.py`

 * *Files identical despite different names*

### Comparing `cjapy-0.2.0/cjapy/configs.py` & `cjapy-0.2.1/cjapy/configs.py`

 * *Files identical despite different names*

### Comparing `cjapy-0.2.0/cjapy/connector.py` & `cjapy-0.2.1/cjapy/connector.py`

 * *Files 1% similar despite different names*

```diff
@@ -206,15 +206,18 @@
                     return json.loads(res.text)
                 except:
                     if self.loggingEnabled:
                         self.logger.error(
                             f"POST method failed: {res.status}, {res.text}"
                         )
                     return res.text
-            res_json = {"error": "Request Error"}
+            if res.status_code == '504':
+                res_json = {"error-504": "504 Gateway Time-out"}
+            else:
+                res_json = {"error": f"Request Error, status: {res.status_code}"}
         return res_json
 
     def patchData(
         self,
         endpoint: str,
         params: dict = None,
         data=None,
```

### Comparing `cjapy-0.2.0/cjapy/projects.py` & `cjapy-0.2.1/cjapy/projects.py`

 * *Files identical despite different names*

### Comparing `cjapy-0.2.0/cjapy/requestCreator.py` & `cjapy-0.2.1/cjapy/requestCreator.py`

 * *Files 2% similar despite different names*

```diff
@@ -205,14 +205,31 @@
         """
         Specific the number of element to retrieve. Default is 10.
         Arguments:
             limit : OPTIONAL : number of elements to return
         """
         self.__request["settings"]["limit"] = limit
 
+    def setSearch(self,itemIds:list=None)-> None:
+        """
+        Set the items ID search in the specified dimension
+        Arguments :
+            itemIds : REQUIRED : The list of itemId to be searched in the dimension
+        """
+        if type(itemIds) != list:
+            raise TypeError("itemIds should be a list of values")
+        self.__request["search"]["itemIds"] = itemIds
+    
+    def removeSearch(self)->None:
+        """
+        Remove the search capability in the request.
+        """
+        del self.__request["search"]
+
+
     def setRepeatInstance(self, repeat: bool = True) -> None:
         """
         Specify if repeated instances should be counted.
         Arguments:
             repeat : OPTIONAL : True or False (True by default)
         """
         self.__request["settings"]["countRepeatInstances"] = repeat
```

### Comparing `cjapy-0.2.0/cjapy/token_provider.py` & `cjapy-0.2.1/cjapy/token_provider.py`

 * *Files identical despite different names*

### Comparing `cjapy-0.2.0/cjapy/workspace.py` & `cjapy-0.2.1/cjapy/workspace.py`

 * *Files 0% similar despite different names*

```diff
@@ -40,15 +40,16 @@
             metricFilters : OPTIONAL : Filter name for the id of the filter
             resolveColumns : OPTIONAL :
         """
         for filter in dataRequest["globalFilters"]:
             if filter["type"] == "dateRange":
                 self.startDate = filter["dateRange"].split("/")[0]
                 self.endDate = filter["dateRange"].split("/")[1]
-        self.dataRequest = RequestCreator(dataRequest)
+        dataRequestCopy = deepcopy(dataRequest)
+        self.dataRequest = RequestCreator(dataRequestCopy)
         self.requestSize = dataRequest["settings"]["limit"]
         self.settings = dataRequest["settings"]
         self.pageRequested = dataRequest["settings"]["page"] + 1
         self.summaryData = summaryData
         self.reportType = reportType
         self.cjaConnector = cjaConnector
         ## global filters resolution
```

### Comparing `cjapy-0.2.0/cjapy.egg-info/PKG-INFO` & `cjapy-0.2.1/cjapy.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cjapy
-Version: 0.2.0
+Version: 0.2.1
 Summary: Adobe Customer Journey Analytics (CJA) wrapper
 Home-page: https://github.com/pitchmuc/cjapy
 Author: Julien Piccini
 Author-email: Julien Piccini <piccini.julien@gmail.com>
 License: Apache License 2.0
 Project-URL: homepage, https://github.com/pitchmuc/cjapy
 Project-URL: changelog, https://github.com/pitchmuc/cjapy/blob/master/docs/releases.md
```

### Comparing `cjapy-0.2.0/cjapy.egg-info/SOURCES.txt` & `cjapy-0.2.1/cjapy.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `cjapy-0.2.0/docs/authenticating_without_config_json.md` & `cjapy-0.2.1/docs/authenticating_without_config_json.md`

 * *Files identical despite different names*

### Comparing `cjapy-0.2.0/docs/cja.md` & `cjapy-0.2.1/docs/cja.md`

 * *Files identical despite different names*

### Comparing `cjapy-0.2.0/docs/getting_started.md` & `cjapy-0.2.1/docs/getting_started.md`

 * *Files identical despite different names*

### Comparing `cjapy-0.2.0/docs/logging.md` & `cjapy-0.2.1/docs/logging.md`

 * *Files identical despite different names*

### Comparing `cjapy-0.2.0/docs/main.md` & `cjapy-0.2.1/docs/main.md`

 * *Files identical despite different names*

### Comparing `cjapy-0.2.0/docs/projects.md` & `cjapy-0.2.1/docs/projects.md`

 * *Files identical despite different names*

### Comparing `cjapy-0.2.0/docs/requestCreator.md` & `cjapy-0.2.1/docs/requestCreator.md`

 * *Files identical despite different names*

### Comparing `cjapy-0.2.0/docs/workspace.md` & `cjapy-0.2.1/docs/workspace.md`

 * *Files identical despite different names*

### Comparing `cjapy-0.2.0/pyproject.toml` & `cjapy-0.2.1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `cjapy-0.2.0/setup.py` & `cjapy-0.2.1/setup.py`

 * *Files identical despite different names*

