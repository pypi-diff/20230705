# Comparing `tmp/asset_tracking_pepsico-1.0.0.tar.gz` & `tmp/asset_tracking_pepsico-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "asset_tracking_pepsico-1.0.0.tar", last modified: Mon Jul  3 06:37:46 2023, max compression
+gzip compressed data, was "asset_tracking_pepsico-1.0.1.tar", last modified: Wed Jul  5 13:01:09 2023, max compression
```

## Comparing `asset_tracking_pepsico-1.0.0.tar` & `asset_tracking_pepsico-1.0.1.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 jatintalati   (501) staff       (20)        0 2023-07-03 06:37:46.386428 asset_tracking_pepsico-1.0.0/
--rw-r--r--   0 jatintalati   (501) staff       (20)     1070 2023-01-19 18:18:48.000000 asset_tracking_pepsico-1.0.0/LICENSE
--rw-r--r--   0 jatintalati   (501) staff       (20)     1593 2023-07-03 06:37:46.385979 asset_tracking_pepsico-1.0.0/PKG-INFO
--rw-r--r--   0 jatintalati   (501) staff       (20)     1015 2023-05-31 14:48:14.000000 asset_tracking_pepsico-1.0.0/README.md
-drwxr-xr-x   0 jatintalati   (501) staff       (20)        0 2023-07-03 06:37:46.380626 asset_tracking_pepsico-1.0.0/asset_tracking_pepsico/
--rw-r--r--   0 jatintalati   (501) staff       (20)     6746 2023-05-31 12:41:32.000000 asset_tracking_pepsico-1.0.0/asset_tracking_pepsico/asset_tracking_devicelogs.py
--rw-r--r--   0 jatintalati   (501) staff       (20)     4851 2023-06-07 10:03:22.000000 asset_tracking_pepsico-1.0.0/asset_tracking_pepsico/asset_tracking_ingest.py
-drwxr-xr-x   0 jatintalati   (501) staff       (20)        0 2023-07-03 06:37:46.384656 asset_tracking_pepsico-1.0.0/asset_tracking_pepsico/dto/
--rw-r--r--   0 jatintalati   (501) staff       (20)     6539 2023-05-31 15:54:17.000000 asset_tracking_pepsico-1.0.0/asset_tracking_pepsico/dto/PostgresSchema.py
--rw-r--r--   0 jatintalati   (501) staff       (20)     1332 2023-07-03 06:34:17.000000 asset_tracking_pepsico-1.0.0/asset_tracking_pepsico/utilities.py
-drwxr-xr-x   0 jatintalati   (501) staff       (20)        0 2023-07-03 06:37:46.383538 asset_tracking_pepsico-1.0.0/asset_tracking_pepsico.egg-info/
--rw-r--r--   0 jatintalati   (501) staff       (20)     1593 2023-07-03 06:37:46.000000 asset_tracking_pepsico-1.0.0/asset_tracking_pepsico.egg-info/PKG-INFO
--rw-r--r--   0 jatintalati   (501) staff       (20)      442 2023-07-03 06:37:46.000000 asset_tracking_pepsico-1.0.0/asset_tracking_pepsico.egg-info/SOURCES.txt
--rw-r--r--   0 jatintalati   (501) staff       (20)        1 2023-07-03 06:37:46.000000 asset_tracking_pepsico-1.0.0/asset_tracking_pepsico.egg-info/dependency_links.txt
--rw-r--r--   0 jatintalati   (501) staff       (20)       35 2023-07-03 06:37:46.000000 asset_tracking_pepsico-1.0.0/asset_tracking_pepsico.egg-info/requires.txt
--rw-r--r--   0 jatintalati   (501) staff       (20)       23 2023-07-03 06:37:46.000000 asset_tracking_pepsico-1.0.0/asset_tracking_pepsico.egg-info/top_level.txt
--rw-r--r--   0 jatintalati   (501) staff       (20)      748 2023-07-03 06:37:03.000000 asset_tracking_pepsico-1.0.0/pyproject.toml
--rw-r--r--   0 jatintalati   (501) staff       (20)       38 2023-07-03 06:37:46.386603 asset_tracking_pepsico-1.0.0/setup.cfg
+drwxr-xr-x   0 jatintalati   (501) staff       (20)        0 2023-07-05 13:01:09.093556 asset_tracking_pepsico-1.0.1/
+-rw-r--r--   0 jatintalati   (501) staff       (20)     1070 2023-01-19 18:18:48.000000 asset_tracking_pepsico-1.0.1/LICENSE
+-rw-r--r--   0 jatintalati   (501) staff       (20)     1593 2023-07-05 13:01:09.092982 asset_tracking_pepsico-1.0.1/PKG-INFO
+-rw-r--r--   0 jatintalati   (501) staff       (20)     1015 2023-05-31 14:48:14.000000 asset_tracking_pepsico-1.0.1/README.md
+drwxr-xr-x   0 jatintalati   (501) staff       (20)        0 2023-07-05 13:01:09.087053 asset_tracking_pepsico-1.0.1/asset_tracking_pepsico/
+-rw-r--r--   0 jatintalati   (501) staff       (20)     6746 2023-05-31 12:41:32.000000 asset_tracking_pepsico-1.0.1/asset_tracking_pepsico/asset_tracking_devicelogs.py
+-rw-r--r--   0 jatintalati   (501) staff       (20)     4855 2023-07-05 12:58:56.000000 asset_tracking_pepsico-1.0.1/asset_tracking_pepsico/asset_tracking_ingest.py
+drwxr-xr-x   0 jatintalati   (501) staff       (20)        0 2023-07-05 13:01:09.091971 asset_tracking_pepsico-1.0.1/asset_tracking_pepsico/dto/
+-rw-r--r--   0 jatintalati   (501) staff       (20)     6503 2023-07-05 12:58:56.000000 asset_tracking_pepsico-1.0.1/asset_tracking_pepsico/dto/PostgresSchema.py
+-rw-r--r--   0 jatintalati   (501) staff       (20)     1332 2023-07-03 06:34:17.000000 asset_tracking_pepsico-1.0.1/asset_tracking_pepsico/utilities.py
+drwxr-xr-x   0 jatintalati   (501) staff       (20)        0 2023-07-05 13:01:09.091198 asset_tracking_pepsico-1.0.1/asset_tracking_pepsico.egg-info/
+-rw-r--r--   0 jatintalati   (501) staff       (20)     1593 2023-07-05 13:01:09.000000 asset_tracking_pepsico-1.0.1/asset_tracking_pepsico.egg-info/PKG-INFO
+-rw-r--r--   0 jatintalati   (501) staff       (20)      442 2023-07-05 13:01:09.000000 asset_tracking_pepsico-1.0.1/asset_tracking_pepsico.egg-info/SOURCES.txt
+-rw-r--r--   0 jatintalati   (501) staff       (20)        1 2023-07-05 13:01:09.000000 asset_tracking_pepsico-1.0.1/asset_tracking_pepsico.egg-info/dependency_links.txt
+-rw-r--r--   0 jatintalati   (501) staff       (20)       35 2023-07-05 13:01:09.000000 asset_tracking_pepsico-1.0.1/asset_tracking_pepsico.egg-info/requires.txt
+-rw-r--r--   0 jatintalati   (501) staff       (20)       23 2023-07-05 13:01:09.000000 asset_tracking_pepsico-1.0.1/asset_tracking_pepsico.egg-info/top_level.txt
+-rw-r--r--   0 jatintalati   (501) staff       (20)      748 2023-07-05 12:59:49.000000 asset_tracking_pepsico-1.0.1/pyproject.toml
+-rw-r--r--   0 jatintalati   (501) staff       (20)       38 2023-07-05 13:01:09.093729 asset_tracking_pepsico-1.0.1/setup.cfg
```

### Comparing `asset_tracking_pepsico-1.0.0/LICENSE` & `asset_tracking_pepsico-1.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `asset_tracking_pepsico-1.0.0/PKG-INFO` & `asset_tracking_pepsico-1.0.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: asset_tracking_pepsico
-Version: 1.0.0
+Version: 1.0.1
 Summary: An asset tracking package where the device logs can be read and the location information can be extracted from the log file provided in the parameters.
 Author-email: Jatin Talati <jatalati@in.ibm.com>
 Keywords: asset,tracking,pepsico,location,latitude,longitude,store,events
 Classifier: Programming Language :: Python :: 3
 Classifier: Development Status :: 1 - Planning
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.7
```

### Comparing `asset_tracking_pepsico-1.0.0/README.md` & `asset_tracking_pepsico-1.0.1/README.md`

 * *Files identical despite different names*

### Comparing `asset_tracking_pepsico-1.0.0/asset_tracking_pepsico/asset_tracking_devicelogs.py` & `asset_tracking_pepsico-1.0.1/asset_tracking_pepsico/asset_tracking_devicelogs.py`

 * *Files identical despite different names*

### Comparing `asset_tracking_pepsico-1.0.0/asset_tracking_pepsico/asset_tracking_ingest.py` & `asset_tracking_pepsico-1.0.1/asset_tracking_pepsico/asset_tracking_ingest.py`

 * *Files 5% similar despite different names*

```diff
@@ -51,15 +51,15 @@
             traceback.print_exc()
 
     def extract_properties(self, properties):
         try:
             # print("properties === ", properties)
             emp_det = properties['Employee']
             loc_info = properties['UserLocationCoordinates']
-            asset_id, emp_name = emp_det[:emp_det.find(',')], emp_det[emp_det.find(',')+1:]
+            object_id, emp_name = emp_det[:emp_det.find(',')], emp_det[emp_det.find(',')+1:]
             lat, long, acc, _ = loc_info.split(',')
             lat, long, acc = float(lat.strip()), float(long.strip()), float(acc.strip())
             event_desc = properties['Description']
             try:
                 loc_desc = properties['LocationDescription'].replace("'", "")
             except KeyError:
                 loc_desc = None
@@ -72,28 +72,28 @@
             except KeyError:
                 transition = None
             try:
                 route = properties['Route']
             except KeyError:
                 route = None
             version = properties['Version']
-            return asset_id, emp_name, lat, long, acc, event_desc, transition, route, version, loc_desc, loc_id
+            return object_id, emp_name, lat, long, acc, event_desc, transition, route, version, loc_desc, loc_id
         except KeyError:
             traceback.print_exc()
 
-    def create_schema_list(self, df, asset_type, data_source, schema_version):
+    def create_schema_list(self, df, object_type, data_source, schema_version):
         try:
             schema_list = []
             for idx, item in df.iterrows():
                 if item['EventName'] == 'CrashDiagnostics' or item['EventName'] == '':
                     continue
-                asset_id, emp_name, lat, long, acc, event_desc, transition, route, version, loc_desc, loc_id = \
+                object_id, emp_name, lat, long, acc, event_desc, transition, route, version, loc_desc, loc_id = \
                     None, None, None, None, None, None, None, None, None, None, None
                 if len(item['Properties']) != 0:
-                    asset_id, emp_name, lat, long, acc, event_desc, transition, route, version, loc_desc, loc_id = \
+                    object_id, emp_name, lat, long, acc, event_desc, transition, route, version, loc_desc, loc_id = \
                         self.extract_properties(item['Properties'])
 
                 times = item['Timestamp']
                 event = item['EventName']
 
                 properties_dict = {
                     'Employee_Name': emp_name,
@@ -103,14 +103,14 @@
                     'Transition': transition,
                     'Route': route,
                     'Version': version,
                     'EventId': item['EventId'],
                     'Description': event_desc
                 }
 
-                schema = PostgresSchemaDto(schema_version=schema_version, asset_id=asset_id, asset_type=asset_type, event_type=event,
-                                           location_description=loc_desc, location_id=loc_id, asset_latitude=lat, asset_longitude=long,
+                schema = PostgresSchemaDto(schema_version=schema_version, object_id=object_id, object_type=object_type, event_type=event,
+                                           location_hint=loc_desc, location_id=loc_id, object_latitude=lat, object_longitude=long,
                                            created_ts=times, lat_long_acc=acc, datasource=data_source, properties_dict=str(properties_dict))
                 schema_list.append(schema)
             return schema_list
         except:
             traceback.print_exc()
```

### Comparing `asset_tracking_pepsico-1.0.0/asset_tracking_pepsico/dto/PostgresSchema.py` & `asset_tracking_pepsico-1.0.1/asset_tracking_pepsico/dto/PostgresSchema.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,64 +1,64 @@
 from typing import Optional
 from pydantic import BaseModel
 
 
 class Item(BaseModel):
     schema_version: Optional[float] = None
-    asset_type: Optional[str] = None
-    asset_id: Optional[str] = None
+    object_type: Optional[str] = None
+    object_id: Optional[str] = None
     event_type: Optional[str] = None
-    location_description: Optional[str] = None
+    location_hint: Optional[str] = None
     location_id: Optional[str] = None
-    asset_latitude: Optional[float] = None
-    asset_longitude: Optional[float] = None
+    object_latitude: Optional[float] = None
+    object_longitude: Optional[float] = None
     lat_long_acc: Optional[float] = None
     created_ts: Optional[str] = None
     altitude: Optional[float] = None
     heading: Optional[float] = None
     speed: Optional[float] = None
     speed_accuracy: Optional[float] = None
     course: Optional[float] = None
     course_accuracy: Optional[float] = None
     datasource: Optional[str] = None
     properties_dict: Optional[str] = None
 
 
 class PostgresSchemaDto:
     schema_version: Optional[float] = None
-    asset_type: Optional[str] = None
-    asset_id: Optional[str] = None
+    object_type: Optional[str] = None
+    object_id: Optional[str] = None
     event_type: Optional[str] = None
-    location_description: Optional[str] = None
+    location_hint: Optional[str] = None
     location_id: Optional[str] = None
-    asset_latitude: Optional[float] = None
-    asset_longitude: Optional[float] = None
+    object_latitude: Optional[float] = None
+    object_longitude: Optional[float] = None
     lat_long_acc: Optional[float] = None
     created_ts: Optional[str] = None
     altitude: Optional[float] = None
     heading: Optional[float] = None
     speed: Optional[float] = None
     speed_accuracy: Optional[float] = None
     course: Optional[float] = None
     course_accuracy: Optional[float] = None
     datasource: Optional[str] = None
     properties_dict: Optional[str] = None
 
-    def __init__(self, schema_version=None, asset_type=None, asset_id=None, event_type=None, location_description=None, location_id=None,
-                 asset_latitude=None, asset_longitude=None, lat_long_acc=None, created_ts=None, altitude=None, heading=None,
+    def __init__(self, schema_version=None, object_type=None, object_id=None, event_type=None, location_hint=None, location_id=None,
+                 object_latitude=None, object_longitude=None, lat_long_acc=None, created_ts=None, altitude=None, heading=None,
                  speed=None, speed_accuracy=None, course=None, course_accuracy=None,
                  datasource=None, properties_dict=None):
         self.schema_version = schema_version
-        self.asset_type = asset_type
-        self.asset_id = asset_id
+        self.object_type = object_type
+        self.object_id = object_id
         self.event_type = event_type
-        self.location_description = location_description
+        self.location_hint = location_hint
         self.location_id = location_id
-        self.asset_latitude = asset_latitude
-        self.asset_longitude = asset_longitude
+        self.object_latitude = object_latitude
+        self.object_longitude = object_longitude
         self.lat_long_acc = lat_long_acc
         self.created_ts = created_ts
         self.altitude = altitude
         self.heading = heading
         self.speed = speed
         self.speed_accuracy = speed_accuracy
         self.course = course
@@ -66,34 +66,34 @@
         self.datasource = datasource
         self.properties_dict = properties_dict
 
     # Getter methods
     def get_schema_version(self):
         return self.schema_version
 
-    def get_asset_type(self):
-        return self.asset_type
+    def get_object_type(self):
+        return self.object_type
 
-    def get_asset_id(self):
-        return self.asset_id
+    def get_object_id(self):
+        return self.object_id
 
     def get_event_type(self):
         return self.event_type
 
-    def get_location_description(self):
-        return self.location_description
+    def get_location_hint(self):
+        return self.location_hint
 
     def get_location_id(self):
         return self.location_id
 
-    def get_asset_latitude(self):
-        return self.asset_latitude
+    def get_object_latitude(self):
+        return self.object_latitude
 
-    def get_asset_longitude(self):
-        return self.asset_longitude
+    def get_object_longitude(self):
+        return self.object_longitude
 
     def get_lat_long_acc(self):
         return self.lat_long_acc
 
     def get_created_ts(self):
         return self.created_ts
 
@@ -121,34 +121,34 @@
     def get_properties_dict(self):
         return self.properties_dict
 
     # Setter methods
     def set_schema_version(self, value):
         self.schema_version = value
 
-    def set_asset_type(self, value):
-        self.asset_type = value
+    def set_object_type(self, value):
+        self.object_type = value
 
-    def set_asset_id(self, value):
-        self.asset_id = value
+    def set_object_id(self, value):
+        self.object_id = value
 
     def set_event_type(self, value):
         self.event_type = value
 
-    def set_location_description(self, value):
-        self.location_description = value
+    def set_location_hint(self, value):
+        self.location_hint = value
 
     def set_location_id(self, value):
         self.location_id = value
 
-    def set_asset_latitude(self, value):
-        self.asset_latitude = value
+    def set_object_latitude(self, value):
+        self.object_latitude = value
 
-    def set_asset_longitude(self, value):
-        self.asset_longitude = value
+    def set_object_longitude(self, value):
+        self.object_longitude = value
 
     def set_lat_long_acc(self, value):
         self.lat_long_acc = value
 
     def set_created_ts(self, value):
         self.created_ts = value
 
@@ -175,31 +175,31 @@
 
     def set_properties_dict(self, value):
         self.properties_dict = value
 
     def __dict__(self):
         return {
             'schema_version': self.schema_version,
-            'asset_type': self.asset_type,
-            'asset_id': self.asset_id,
+            'object_type': self.object_type,
+            'object_id': self.object_id,
             'event_type': self.event_type,
-            'location_description': self.location_description,
+            'location_hint': self.location_hint,
             'location_id': self.location_id,
-            'asset_latitude': self.asset_latitude,
-            'asset_longitude': self.asset_longitude,
+            'object_latitude': self.object_latitude,
+            'object_longitude': self.object_longitude,
             'lat_long_acc': self.lat_long_acc,
             'created_ts': self.created_ts,
             'altitude': self.altitude,
             'heading': self.heading,
             'speed': self.speed,
             'speed_accuracy': self.speed_accuracy,
             'course': self.course,
             'course_accuracy': self.course_accuracy,
             'datasource': self.datasource,
             'properties_dict': self.properties_dict
         }
 
     def __str__(self):
-        return f"{self.schema_version}, \'{self.asset_type}\', \'{self.asset_id}\', \'{self.event_type}\', \'{self.location_description}\', " \
-               f"\'{self.location_id}\', {self.asset_latitude}, {self.asset_longitude}, {self.lat_long_acc}, \'{self.created_ts}\', " \
+        return f"{self.schema_version}, \'{self.object_type}\', \'{self.object_id}\', \'{self.event_type}\', \'{self.location_hint}\', " \
+               f"\'{self.location_id}\', {self.object_latitude}, {self.object_longitude}, {self.lat_long_acc}, \'{self.created_ts}\', " \
                f"{self.altitude}, {self.heading}, {self.speed}, {self.speed_accuracy}, {self.course}, {self.course_accuracy}, " \
                f"\'{self.datasource}\', \'{self.properties_dict}\'"
```

### Comparing `asset_tracking_pepsico-1.0.0/asset_tracking_pepsico/utilities.py` & `asset_tracking_pepsico-1.0.1/asset_tracking_pepsico/utilities.py`

 * *Files identical despite different names*

### Comparing `asset_tracking_pepsico-1.0.0/asset_tracking_pepsico.egg-info/PKG-INFO` & `asset_tracking_pepsico-1.0.1/asset_tracking_pepsico.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: asset-tracking-pepsico
-Version: 1.0.0
+Version: 1.0.1
 Summary: An asset tracking package where the device logs can be read and the location information can be extracted from the log file provided in the parameters.
 Author-email: Jatin Talati <jatalati@in.ibm.com>
 Keywords: asset,tracking,pepsico,location,latitude,longitude,store,events
 Classifier: Programming Language :: Python :: 3
 Classifier: Development Status :: 1 - Planning
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.7
```

### Comparing `asset_tracking_pepsico-1.0.0/pyproject.toml` & `asset_tracking_pepsico-1.0.1/pyproject.toml`

 * *Files 11% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "asset_tracking_pepsico"
-version = "1.0.0"
+version = "1.0.1"
 authors = [
   { name="Jatin Talati", email="jatalati@in.ibm.com" },
 ]
 description = "An asset tracking package where the device logs can be read and the location information can be extracted from the log file provided in the parameters."
 readme = "README.md"
 requires-python = ">=3.7"
 keywords = ["asset", "tracking", "pepsico", "location", "latitude", "longitude", "store", "events"]
```

