# Comparing `tmp/alanapy-0.10.tar.gz` & `tmp/alanapy-0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "alanapy-0.10.tar", last modified: Wed Jul  5 04:38:43 2023, max compression
+gzip compressed data, was "alanapy-0.9.tar", last modified: Thu Jun 22 00:10:02 2023, max compression
```

## Comparing `alanapy-0.10.tar` & `alanapy-0.9.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxrwxrwx   0        0        0        0 2023-07-05 04:38:43.255468 alanapy-0.10/
--rw-rw-rw-   0        0        0     1085 2023-06-15 19:50:23.000000 alanapy-0.10/LICENSE
--rw-rw-rw-   0        0        0      635 2023-07-05 04:38:43.254458 alanapy-0.10/PKG-INFO
--rw-rw-rw-   0        0        0        9 2023-06-15 19:50:23.000000 alanapy-0.10/README.md
-drwxrwxrwx   0        0        0        0 2023-07-05 04:38:43.252464 alanapy-0.10/alanapy.egg-info/
--rw-rw-rw-   0        0        0      635 2023-07-05 04:38:42.000000 alanapy-0.10/alanapy.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      191 2023-07-05 04:38:42.000000 alanapy-0.10/alanapy.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-05 04:38:42.000000 alanapy-0.10/alanapy.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       33 2023-07-05 04:38:42.000000 alanapy-0.10/alanapy.egg-info/requires.txt
--rw-rw-rw-   0        0        0        8 2023-07-05 04:38:42.000000 alanapy-0.10/alanapy.egg-info/top_level.txt
--rw-rw-rw-   0        0        0    76153 2023-07-05 04:36:48.000000 alanapy-0.10/alanapy.py
--rw-rw-rw-   0        0        0       42 2023-07-05 04:38:43.255468 alanapy-0.10/setup.cfg
--rw-rw-rw-   0        0        0      857 2023-07-05 04:38:23.000000 alanapy-0.10/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-22 00:10:02.134517 alanapy-0.9/
+-rw-rw-rw-   0        0        0     1085 2023-06-15 19:50:23.000000 alanapy-0.9/LICENSE
+-rw-rw-rw-   0        0        0      634 2023-06-22 00:10:02.133519 alanapy-0.9/PKG-INFO
+-rw-rw-rw-   0        0        0        9 2023-06-15 19:50:23.000000 alanapy-0.9/README.md
+drwxrwxrwx   0        0        0        0 2023-06-22 00:10:02.130537 alanapy-0.9/alanapy.egg-info/
+-rw-rw-rw-   0        0        0      634 2023-06-22 00:10:01.000000 alanapy-0.9/alanapy.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      191 2023-06-22 00:10:01.000000 alanapy-0.9/alanapy.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-22 00:10:01.000000 alanapy-0.9/alanapy.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       33 2023-06-22 00:10:01.000000 alanapy-0.9/alanapy.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        8 2023-06-22 00:10:01.000000 alanapy-0.9/alanapy.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0    71641 2023-06-21 23:47:13.000000 alanapy-0.9/alanapy.py
+-rw-rw-rw-   0        0        0       42 2023-06-22 00:10:02.134517 alanapy-0.9/setup.cfg
+-rw-rw-rw-   0        0        0      884 2023-06-22 00:09:51.000000 alanapy-0.9/setup.py
```

### Comparing `alanapy-0.10/LICENSE` & `alanapy-0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `alanapy-0.10/PKG-INFO` & `alanapy-0.9/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: alanapy
-Version: 0.10
+Version: 0.9
 Home-page: https://github.com/orkahub/alanapy
 Author: Orkahub Energy
 Author-email: orkahub@gmail.com
 License: MIT
 Keywords: RESERVOIR,ENERGY,OIL,GAS,PRODUCTION,PYTHON,ALANA
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
```

### Comparing `alanapy-0.10/alanapy.egg-info/PKG-INFO` & `alanapy-0.9/alanapy.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: alanapy
-Version: 0.10
+Version: 0.9
 Home-page: https://github.com/orkahub/alanapy
 Author: Orkahub Energy
 Author-email: orkahub@gmail.com
 License: MIT
 Keywords: RESERVOIR,ENERGY,OIL,GAS,PRODUCTION,PYTHON,ALANA
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
```

### Comparing `alanapy-0.10/alanapy.py` & `alanapy-0.9/alanapy.py`

 * *Files 9% similar despite different names*

```diff
@@ -463,43 +463,40 @@
 
 class Economics:
     def __init__(self):
         self.master = Singleton().master
 
     def runEconomics(self, params={}):
         """
-        {
-        "description":,
-        "returns":,
-        "example":,
-        }
+            args(self, master_fk)
         """
         if len(params) == 0:
             return "Please provide the params dictionary, refer to the documentation of this function"
 
         url = self.master.root_url + "/api/economics/runeconomics/"
         header = self.master.header
         mydata = requests.get(url, headers=header, params=params)  # .json()
         results = mydata.json()
         return results
 
     def createEconomicForecastMaster(self, _dict: dict):
         """
         {
-        "description":"Function that creates a Master for Economic Forecast",
-        "arguments":{
+        "description": "Function that creates a Master for Economic Forecast",
+        "arguments":
+            {
                 "name": "",
                 "description": ""
             },
-        "return":{
+        "return": {
                 "id": "",
                 "name": "",
                 "description": ""
             },
-        "example":,
+        "example": ""
         }
         """
         dict_response_api = self.master._createMaster("economics", "economicforecastmaster", _dict)
         return dict_response_api
 
     def editEconomicForecastMaster(self, master_fk: int, dict_edit_master: dict):
         """
@@ -1010,43 +1007,35 @@
                 "updated_at": "YYYY-MM-DD",
                 "description": "Empty",
                 "start_date": "YYYY-MM-DD",
                 "end_date": "YYYY-MM-DD",
                 "scope": "PUBLIC"
                 }
             },
-        "return":{
-            dict_response : {
-            }
-        },
         "example": ""
         }
         """
         dict_fdpmaster = self.master._createMaster("fdp", "fdpmaster", fdp_master_dict)
         return dict_fdpmaster
     
     def createFDPCase(self, case_app, case_table, list_of_dicts, str_fdp_name):
         """
         {
-            "description": "Create a Field Development Plan ",
-            "arguments" : {
-                dict_main : {
-                    "name": "str_fdp_name",
-                    "created_at": "YYYY-MM-DD",
-                    "updated_at": "YYYY-MM-DD",
-                    "description": "Empty",
-                    "start_date": "YYYY-MM-DD",
-                    "end_date": "YYYY-MM-DD",
-                    "scope": "PUBLIC"
-                    }
-                },
-            "return":{
-                "dict_response": {
+        "description": "Create a Field Development Plan ",
+        "arguments" : {
+            dict_main : {
+                "name": "str_fdp_name",
+                "created_at": "YYYY-MM-DD",
+                "updated_at": "YYYY-MM-DD",
+                "description": "Empty",
+                "start_date": "YYYY-MM-DD",
+                "end_date": "YYYY-MM-DD",
+                "scope": "PUBLIC"
                 }
-        },
+            },
         "example": ""
         }
         """
         df_temp = pd.DataFrame(list_of_dicts)
         df_temp["welltype_fk"] = ""
         df_temp["dcamaster_fk"] = ""       
         # fdpMaster
@@ -1155,24 +1144,20 @@
             bool_status = mygeneric.statusCodeCheck(mydata)
             if bool_status:
                 fdp_case = mydata.json()
                 
     def runFDP(self, str_fdp_name, preffix="FDP_"):
         """
         }
-            "description": "Run FDP given by a FDP master and its cases",
-            "arguments" : {
-                "FDP_master_name" : "str_fdp_master"
-                "Preffix" : "FDP_"
-                },
-            "return" : {
-            "dict_response":{
-            }
+        "description": "",
+        "arguments" : {
+            "FDP_master_name" : "str_fdp_master"
+            "Preffix" : "FDP_"
             },
-            "example": "",
+        "example": "",
         }
         """
         int_id_master = self.master.fdpmasterdict[str_fdp_name]
         url = self.master.root_url + "/api/" + "fdp/runfdp/"
         header = self.master.header
         params = {
             "fdpmaster_fk" : int_id_master ,
@@ -1188,25 +1173,18 @@
         """
         tuple_response_api = self.master._createMasterCases("fdp", "fdpmaster", _dict, list_of_dicts, "fdp", "fdpcase")
         print(tuple_response_api)
         return tuple_response_api
 
     def getFDPCases(self, master_fk: str):
         """
-        {
-            "description":"Function that return the cases that match with the master_fk",
-            "arguments":{
-                "master_fk" : int
-            },
-            "return":{
-                "dict_response":{
-                }
-            },
-            "example":,
-        }
+        Function that return the cases that match with the master_fk
+        args(master_fk)
+        master_fk = Integer
+        RETURN dict_get_cases
         """
         dict_get_cases = self.master._getMaster("fdp", "fdpcase", str(master_fk))
         print(dict_get_cases)
         return dict_get_cases
 
     def createFDPMasterAndCases(self, _dict: dict, list_of_dicts: list):
         """
@@ -1214,398 +1192,316 @@
         """
         tuple_response_api = self.master._createMasterCases("downtime", "downtimemaster", _dict, list_of_dicts, "downtime", "downtimecase")
         print(tuple_response_api)
         return tuple_response_api
 
     def getFDPDowtimeCases(self, master_fk: str):
         """
-        {
-            "description":"Function that return the cases that match with the master_fk",
-            "arguments":{
-                "master_fk" : int
-            },
-            "return":{
-                "dict_response":{
-                }
-            },
-            "example":,
-        }
+        Function that return the cases that match with the master_fk
+        args(master_fk)
+        master_fk = Integer
+        RETURN dict_get_cases
         """
         dict_get_cases = self.master._getMaster("fdp", "downtimecase", str(master_fk))
         print(dict_get_cases)
         return dict_get_cases
 
 class Datasource:
     def __init__(self):
         self.master = Singleton().master
 
     def createWellMaster(self, well_master_dict: dict):
         """
         {
-            "description": "Function that create Wells",
-            "arguments" : {
-                "dict_main" : {
-                    "well_name": "",
-                    "spud_date": "YYYY-MM-DD",
-                    "production_date": "YYYY-MM-DD",
-                    "api_code": int,
-                    "latitude": float,
-                    "longitude": float,
-                    "utm_x": float,
-                    "utm_y": float,
-                    "comment": "",
-                    "type": ""
-                    "field": "str_field"
-                    }
-                },
-            "return": {
-                dict_response : {
-                }
+        "description": "Function that create Wells",
+        "arguments" : {
+            "well_name": "",
+            "spud_date": "YYYY-MM-DD",
+            "production_date": "YYYY-MM-DD",
+            "api_code": int,
+            "latitude": float,
+            "longitude": float,
+            "utm_x": float,
+            "utm_y": float,
+            "comment": "",
+            "type": ""
+            "field": "str_field"
             },
-            "example": ""
+        "example": ""
         }
         """
         well_master_dict["field_fk"] = self.master.fieldmasterdict[well_master_dict["field"]]
         well_master_dict["formation_fk"] = self.master.formationmasterdict[well_master_dict["formation"]]
         dict_wellmaster = self.master._createMaster("datasource", "wellmaster", well_master_dict)
         return dict_wellmaster
 
     def getWellMaster(self, str_well_name=None):
         """
         {
             "description":"Function that fetch wellmaster information of a given name or whole table and return a dict.",
             "arguments":
-                {
-                    "str_well_name" : "str = None"
-                },
-            "return":{
-                "dict_response":{
-                }
+            {
+                "str_well_name" : "str = None"
             },
             "example" : "myapi.getWellMaster() or myapi.getWellMaster("well_name")"
         }
         """
         if str_well_name is None:
             dict_get_cases = self.master._getMaster("datasource", "wellmaster")
         else:
             int_well_id = self.master.wellmasterdict[str_well_name]
             dict_get_cases = self.master._getMaster("datasource", "wellmaster", str(int_well_id))
         return dict_get_cases
 
     def editWellMaster(self, master_fk: int, dict_edit_master: dict):
         """
-        {
-            "description":"Function that update a well master record",
-            "arguments":{
-                "dict_main" : {
-                    "well_name": "",
-                    "spud_date": "YYYY-MM-DD",
-                    "production_date": "YYYY-MM-DD",
-                    "api_code": int,
-                    "latitude": float,
-                    "longitude": float,
-                    "utm_x": float,
-                    "utm_y": float,
-                    "comment": "",
-                    "type": ""
-                    "field": "str_field"
-                    }
-                },
-            "return":{
-                "dict_response":{
-                }
-            },
-            "example":,
+        Function that update a Master
+
+        dict_edit_master = {
+            "well_name": "",
+            "spud_date": None,
+            "production_date": None,
+            "api_code": "",
+            "latitude": "",
+            "longitude": "",
+            "utm_x": None,
+            "utm_y": None,
+            "comment": "",
+            "type": None,
+            "field_fk": None,
+            "formation_fk": None
         }
+        RETURN dict_edit_master
         """
         dict_edit_master = self.master._editMaster("datasource", "wellmaster", dict_edit_master,  str(master_fk))
         return dict_edit_master
 
     def deleteWellMaster(self, master_fk):
+        
         """
-        {
-            "description":"Function that delete the master that match with the master_fk",
-            "arguments":{
-                "master_fk" : int
-            },
-            "return":{
-                "dict_response":{
-                }
-            },
-            "example":,
-        }
+        Function that delete the master that match with the master_fk
+        args(master_fk)
+        RETURN deleted_master
         """
         deleted_master = self.master._deleteMaster("datasource", "wellmaster", str(master_fk))
         return deleted_master
 
     def createFormationMaster(self, formation_master_dict: dict):
         """
         {
-            "description": "Function that create Formations"
-            "arguments" : {
-                "main_dict":{
-                    "formation_name": "",
-                    "comment": ""
-                    }
-                },
-            "return":{
-                "dict_response":{
-                }
+        "description": "Function that create Formations"
+        }
+        "arguments" : {
+            "formation_name": "",
+            "comment": ""
             },
         "example": ""
         }
+            
         """
 
         dict_wellmaster = self.master._createMaster("datasource", "formationmaster", formation_master_dict)
         return dict_wellmaster
 
     def getFormationMaster(self, str_formation_name=None):
         """
         {
             "description":"Function that fetch formation information of a given name or whole table and return a dict.",
             "arguments":
             {
                 "str_formation_name" : "str = None"
             },
-            "return": {
-                "dict_response":{
-                }
-            },
             "example" : "myapi.getFormationMaster() or myapi.getFormationMaster("formation_name")"
         }
         """
         if str_formation_name is None:
             dict_get_cases = self.master._getMaster("datasource", "formationmaster")
         else:
             int_formation_id = self.master.formationmasterdict[str_formation_name]
             dict_get_cases = self.master._getMaster("datasource", "formationmaster", str(int_formation_id))
         return dict_get_cases
 
     def editFormationMaster(self, master_fk: int, dict_formation_master: dict):
         """
-        {
-            "description":"Function that updates a formation master record",
-            "arguments":{
-                "dict_main":{
-                    "formation_name":"",
-                    "comment":""
-                }
-            },
-            "return":,
-            "example":,
+        Function that update a Master
+        well_master_dict = {
+            "formation_name":"",
+            "comment":"",
         }
+        RETURN dict_edit_master
         """
         dict_edit_master = self.master._editMaster("datasource", "formationmaster", dict_formation_master,  str(master_fk))
         return dict_edit_master
 
     def deleteFormationMaster(self, master_fk):
         """
-        {
-			"description":"Function that delete the master that match with the master_fk",
-			"arguments":{
-                "master_fk":int
-            },
-			"return":{
-                "dict_response":{
-                }
-            },
-			"example":,
-        }
+        Function that delete the master that match with the master_fk
+        args(master_fk)
+        RETURN deleted_master
         """
         deleted_master = self.master._deleteMaster("datasource", "formationmaster", str(master_fk))
         return deleted_master
 
     def createFieldMaster(self, field_master_dict: dict):
         """
         {
-            "description": "Function that create Fields"
-            "arguments" : {
-                "field_name": "",
-                "comment": "",
-                "Country": "",
-                "Basin":"",
-                "Block":""
-                },
-            "return":{
-                "dict_main":{
-                }
+        "description": "Function that create Fields"
+        }
+        "arguments" : {
+            "field_name": "",
+            "comment": "",
+            "Country": "",
+            "Basin":"",
+            "Block":""
             },
-            "example": ""
+        "example": ""
         }
         """
+
         response_api = self.master._createMaster("datasource", "fieldmaster", field_master_dict)
         return response_api
 
     def getFieldMaster(self, str_field_name=None):
         """
         {
             "description":"Function that fetch field information of a given name or whole table and return a dict.",
-            "arguments":{
-                    "str_field_name" : "str = None"
-                },
-            "return":{
-                "dict_response":{
-                }
+            "arguments":
+            {
+                "str_field_name" : "str = None"
             },
             "example" : "myapi.getFieldMaster() or myapi.getFieldMaster("field_name")"
         }
         """
         if str_field_name is None:
             dict_get_cases = self.master._getMaster("datasource", "fieldmaster")
         else:
             int_field_id = self.master.fieldmasterdict[str_field_name]
             dict_get_cases = self.master._getMaster("datasource", "fieldmaster", str(int_field_id))
         return dict_get_cases
 
-    def editFieldMaster(self, master_fk: int, dict_field_master: dict):
+    def editFieldMaster(self, master_fk: int, dict_formation_master: dict):
         """
-        {
-			"description":"Function that update a field master record",
-			"arguments":{
-                "dict_main": {
-                    "field_name": "Given_Name",
-                    "comment": "",
-                    "Country": "",
-                    "Basin":"",
-                    "Block":""
-                }
-            },
-			"return": {
-                "dict_response":{
-                }
-            },
-			"example":,
+        Function that update a Master
+        field_master_dict = {
+            "field_name": "Given_Name",
+            "comment": "",
+            "Country": "",
+            "Basin":"",
+            "Block":""
         }
+        RETURN dict_edit_master
         """
-        dict_edit_master = self.master._editMaster("datasource", "fieldmaster", dict_field_master,  str(master_fk))
+        dict_edit_master = self.master._editMaster("datasource", "fieldmaster", dict_formation_master,  str(master_fk))
         return dict_edit_master
 
     def deleteFieldMaster(self, master_fk):
         """
         {
-            "description": "Function that deletes a Field"
-            "arguments" : {
-                "master_fk": int,
-                },
-            "return":{
-                "dict_response":{
-                }
+        "description": "Function that deletes a Field"
+        }
+        "arguments" : {
+            "master_fk": int,
             },
-            "example": ""
+        "example": ""
         }
             
         """
+        """
+        Function that delete the master that match with the master_fk
+        args(master_fk)
+        RETURN deleted_master
+        """
         deleted_master = self.master._deleteMaster("datasource", "fieldmaster", str(master_fk))
         return deleted_master
 
     def getFieldWellsDict(self):
         """
         {
-            "description":"Preloaded dictionary of fields and its wells",
-            "arguments":{
-            },
-            "return":{
-                "dict_response":{
-                }
+            "description":"Preloaded dictionary of {field_name: [well_name]}",
+            "arguments":
+            {
             },
             "example" : ""
         }
         """
         field_wells_dict = {}
         for field in list(self.master.fieldmasterdict.keys()):
             field_wells_dict[field] = self.master._getKeysDictList(field, self.getWellFieldDict())
         return field_wells_dict
 
     def getWellFieldDict(self):
         """
         {
-            "description":"Preloaded dictionary of well names and its field",
-            "arguments":{
-            },
-            return:{
-                "dict_response":{
-                }
+            "description":"Preloaded dictionary of {well_name:field_name}",
+            "arguments":
+            {
             },
             "example" : ""
         }
         """
         results = {}
         for welldict in self.master.wellmasterdict_full:
             results[welldict['well_name']] = self.master.fieldmasterdict_inv[welldict['field_fk']]
         return results
 
     def getMonthlyProduction(self, str_well_name: str):
         """
         {
             "description":"Function that fetch monthly production profile of a given well name",
-            "arguments":{
-                    "str_well_name" : "str = None"
-                },
-            "return":{
-                "dict_response":{
-                }
+            "arguments":
+            {
+                "str_well_name" : "str = None"
             },
             "example" : "myapi.getMonthlyProduction("well_name")"
         }
         """
         int_well_id = self.master.wellmasterdict[str_well_name]
         monthly_volume = self.master._getCase("datasource", "wellmonthly", "well_fk", int_well_id)
         return monthly_volume
     
     def getDailyProduction(self,str_well_name: str):
         """
         {
             "description":"Function that fetch daily production profile of a given well name",
-            "arguments":{
+            "arguments":
+            {
                 "str_well_name" : "str = None"
             },
-            "return":{
-                "dict_response":{
-                }
-            },
             "example" : "myapi.getDailyProduction("well_name")"
         }
         """
         int_well_id = self.master.wellmasterdict[str_well_name]
         daily_volume = self.master._getCase("datasource", "welldaily", "well_fk", int_well_id)
         return daily_volume
     
     def getFieldMonthlyProduction(self,str_field_name: str):
         """
         {
             "description":"Function that fetch field monthly production profile of a given field name",
-            "arguments":{
+            "arguments":
+            {
                 "str_field_name" : "str = None"
             },
-            "return":{
-                "dict_response":{
-                }
-            },
             "example" : "myapi.getFieldMonthlyProduction("field_name")"
         }
         """
         monthly_volume = self.master._getCase("datasource","fieldmonthly","fields[]", str_field_name)
         return monthly_volume
         
     def importDataSource(self, tablename, df_table, is_new_data=False):
         """
         {
-            "description": "Function that uploads a csv with data",
-            "arguments" : {
-                dict_main : {
-                    "tablename": "",
-                    "df_table": df_table,
-                    "is_new_date": True
-                }
+        "description": "Function that uploads a csv with data"
+        }
+        "arguments" : {
+            "tablename": "",
+            "df_table": df_table,
+            "is_new_date": True,
             },
-            "return":{
-                "dict_response":{
-                }
-            }
-            "example": ""
+        "example": ""
         }
             
         """
         #test_file = open("/Users/alejandroprimeranavarro/Alana/jupyter_samples/DCA_Summary_sampledata.csv", "rb")
         df_table.to_csv("importDataSource_temp.csv", index=False)
         file = open("importDataSource_temp.csv", "rb")
         url = self.master.root_url +"/api/datasource/dataloader/import/"
@@ -1760,54 +1656,45 @@
 class DCA:
     def __init__(self):
         self.master = Singleton().master
         
     def createDCAMaster(self, dca_master_dict):
         """
         {
-            "description": "Function that creates master for DCA Data",
-            "arguments" : {
-                "dict_main":{
-                    "name": "",
-                    "dca_method": "ARPS",
-                    "forecast_type": "DET",
-                    "primary_fluid_phase": "OIL",
-                    "dca_defaults": "",
-                    "dca_scope": "PUBLIC"
-                }
-            },
-            "return":{
-                "dict_response":{
-                }
+        "description": "Function that creates master for DCA Data"
+        }
+        "arguments" : {
+            "name": "",
+            "dca_method": "ARPS",
+            "forecast_type": "DET",
+            "primary_fluid_phase": "OIL",
+            "dca_defaults": "",
+            "dca_scope": "PUBLIC"
             },
-            "example": ""
+        "example": ""
         }
+            
         """
         dca_master_dict["name"] = dca_master_dict["str_dca_name"]
         dict_dca_master = self.master._createMaster("dca", "dcamaster", dca_master_dict)
         return dict_dca_master
         
     def runDCA(self, dict_dca):
         """
         {
-            "description": "Function that creates a DCA master and then the cases for multiple wells",
-            "arguments":{
-                "dict_main":{
-                    "str_dca_name": "",
-                    "list_well_names": ["well 1", "well 2"],
-                    "date_primary_forecast": ["YYYY-MM-DD", "YYYY-MM-DD"],
-                    "str_arps": ["HYPE", "HYPE"],
-                    "str_date_prod": "monthly"
-                }
-            },
-            "return": {
-                "dict_response":{
-                }
+        "description": "Function that creates a DCA master and then the cases for multiple wells",
+        "arguments":
+            {
+                "str_dca_name": "",
+                "list_well_names": ["well 1", "well 2"],
+                "date_primary_forecast": ["YYYY-MM-DD", "YYYY-MM-DD"],
+                "str_arps": ["HYPE", "HYPE"],
+                "str_date_prod": "monthly"
             },
-            "example": ""
+        "example": ""
         }
         """
         mygeneric = Generic()
         list_check = mygeneric.lists_have_same_length(dict_dca["list_well_names"], dict_dca["date_primary_forecast"], dict_dca["str_arps"])
         if not list_check:
             return "All lists provided need to have the same size"
         url = self.master.root_url + "/api/dca/fit_forecast/"
@@ -1897,63 +1784,17 @@
         dict_response_api = self.master._createCases(list_of_dicts, "dca", "dcacase")
         return dict_response_api
 
     def createDCAMasterCases(self, _dict: dict, list_of_dicts: list):
         tuple_response_api = self.master._createMasterCases("dca", "dcamaster", _dict, list_of_dicts, "dca", "dcacase")
         return tuple_response_api
         
-class DatasourceEDA:
-    def __init__(self):
-        self.master = Singleton().master
-
-    def runNearByWells(self, dict_input):
-        """
-        {
-        "description": "Get Nearby wells given a well name and radius around it in metres"
-        }
-        "arguments" : {
-            well_name: "",
-            radius: float
-            },
-        "example": ""
-        }
-        """
-
-        url = self.master.root_url + "/api/datasource/eda/nearbywells/"
-        header = self.master.header
-        mydata = requests.get(url, headers=header, params=dict_input)  # .json()
-        results = mydata.json()
-        return results
-        
-
-
 class WellType:
-    def __init__(self):
+    def _init_(self):
         self.master = Singleton().master
-
-    def createWellType(self, dca_master_dict):
-        """
-        {
-        "description": "Function that creates master for DCA Data"
-        }
-        "arguments" : {
-            "name": "",
-            "dca_method": "ARPS",
-            "forecast_type": "DET",
-            "primary_fluid_phase": "OIL",
-            "dca_defaults": "",
-            "dca_scope": "PUBLIC"
-            },
-        "example": ""
-        }
-
-        """
-        welltype_master_dict["name"] = welltype_master_dict["str_dca_name"]
-        dict_welltype_master = self.master._createMaster("welltype", "welltypemaster", welltype_master_dict)
-        return dict_welltype_master
         
     def runWellType(self, dict_welltype):
         """
         {
         "description": "Function that runs a welltype for a list of wells",
         "arguments":
             {
```

### Comparing `alanapy-0.10/setup.py` & `alanapy-0.9/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 from setuptools import setup
 
 setup(
     name="alanapy",
-    version="0.10",
+    #packages=["alanapy"],
+    version="0.9",
     license="MIT",
     author = "Orkahub Energy",
 	author_email = "orkahub@gmail.com",
 	url = "https://github.com/orkahub/alanapy",
     long_description="Script for Alana API connection and functions https://alana.tech/open/accounts/login",
     long_description_content_type = "text/x-rst",
     classifiers=[
```

