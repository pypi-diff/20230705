# Comparing `tmp/bondzai.bootstrap-framework-0.0.7.tar.gz` & `tmp/bondzai.bootstrap-framework-0.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bondzai.bootstrap-framework-0.0.7.tar", last modified: Tue Jul  4 14:20:38 2023, max compression
+gzip compressed data, was "bondzai.bootstrap-framework-0.0.8.tar", last modified: Wed Jul  5 12:40:50 2023, max compression
```

## Comparing `bondzai.bootstrap-framework-0.0.7.tar` & `bondzai.bootstrap-framework-0.0.8.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxr-xr-x   0 theo       (501) staff       (20)        0 2023-07-04 14:20:38.286749 bondzai.bootstrap-framework-0.0.7/
--rw-r--r--   0 theo       (501) staff       (20)      547 2023-07-04 14:19:57.000000 bondzai.bootstrap-framework-0.0.7/NOTICE
--rw-r--r--   0 theo       (501) staff       (20)      578 2023-07-04 14:20:38.286858 bondzai.bootstrap-framework-0.0.7/PKG-INFO
--rw-r--r--   0 theo       (501) staff       (20)      141 2023-07-04 14:19:57.000000 bondzai.bootstrap-framework-0.0.7/README.md
-drwxr-xr-x   0 theo       (501) staff       (20)        0 2023-07-04 14:20:38.281118 bondzai.bootstrap-framework-0.0.7/bondzai/
-drwxr-xr-x   0 theo       (501) staff       (20)        0 2023-07-04 14:20:38.284081 bondzai.bootstrap-framework-0.0.7/bondzai/bootstrap_framework/
--rw-r--r--   0 theo       (501) staff       (20)      212 2023-07-04 14:20:27.000000 bondzai.bootstrap-framework-0.0.7/bondzai/bootstrap_framework/__init__.py
--rw-r--r--   0 theo       (501) staff       (20)     2696 2023-07-04 14:19:57.000000 bondzai.bootstrap-framework-0.0.7/bondzai/bootstrap_framework/bootstrap.py
--rw-r--r--   0 theo       (501) staff       (20)    10143 2023-07-04 14:19:57.000000 bondzai.bootstrap-framework-0.0.7/bondzai/bootstrap_framework/dvs_agent.py
--rw-r--r--   0 theo       (501) staff       (20)    14052 2023-07-04 14:19:57.000000 bondzai.bootstrap-framework-0.0.7/bondzai/bootstrap_framework/dvs_com.py
--rw-r--r--   0 theo       (501) staff       (20)     7338 2023-07-04 14:20:27.000000 bondzai.bootstrap-framework-0.0.7/bondzai/bootstrap_framework/dvs_config.py
--rw-r--r--   0 theo       (501) staff       (20)     3008 2023-07-04 14:20:27.000000 bondzai.bootstrap-framework-0.0.7/bondzai/bootstrap_framework/file_handler.py
--rw-r--r--   0 theo       (501) staff       (20)      333 2023-07-04 14:19:57.000000 bondzai.bootstrap-framework-0.0.7/bondzai/bootstrap_framework/logger.py
-drwxr-xr-x   0 theo       (501) staff       (20)        0 2023-07-04 14:20:38.286441 bondzai.bootstrap-framework-0.0.7/bondzai.bootstrap_framework.egg-info/
--rw-r--r--   0 theo       (501) staff       (20)      578 2023-07-04 14:20:38.000000 bondzai.bootstrap-framework-0.0.7/bondzai.bootstrap_framework.egg-info/PKG-INFO
--rw-r--r--   0 theo       (501) staff       (20)      700 2023-07-04 14:20:38.000000 bondzai.bootstrap-framework-0.0.7/bondzai.bootstrap_framework.egg-info/SOURCES.txt
--rw-r--r--   0 theo       (501) staff       (20)        1 2023-07-04 14:20:38.000000 bondzai.bootstrap-framework-0.0.7/bondzai.bootstrap_framework.egg-info/dependency_links.txt
--rw-r--r--   0 theo       (501) staff       (20)        8 2023-07-04 14:20:38.000000 bondzai.bootstrap-framework-0.0.7/bondzai.bootstrap_framework.egg-info/namespace_packages.txt
--rw-r--r--   0 theo       (501) staff       (20)       52 2023-07-04 14:20:38.000000 bondzai.bootstrap-framework-0.0.7/bondzai.bootstrap_framework.egg-info/requires.txt
--rw-r--r--   0 theo       (501) staff       (20)       13 2023-07-04 14:20:38.000000 bondzai.bootstrap-framework-0.0.7/bondzai.bootstrap_framework.egg-info/top_level.txt
--rw-r--r--   0 theo       (501) staff       (20)        1 2023-07-04 14:20:38.000000 bondzai.bootstrap-framework-0.0.7/bondzai.bootstrap_framework.egg-info/zip-safe
--rw-r--r--   0 theo       (501) staff       (20)       71 2023-07-04 14:19:57.000000 bondzai.bootstrap-framework-0.0.7/pyproject.toml
--rw-r--r--   0 theo       (501) staff       (20)      755 2023-07-04 14:20:38.287533 bondzai.bootstrap-framework-0.0.7/setup.cfg
+drwxr-xr-x   0 theo       (501) staff       (20)        0 2023-07-05 12:40:50.981659 bondzai.bootstrap-framework-0.0.8/
+-rw-r--r--   0 theo       (501) staff       (20)      547 2023-07-05 12:40:15.000000 bondzai.bootstrap-framework-0.0.8/NOTICE
+-rw-r--r--   0 theo       (501) staff       (20)      578 2023-07-05 12:40:50.981807 bondzai.bootstrap-framework-0.0.8/PKG-INFO
+-rw-r--r--   0 theo       (501) staff       (20)      141 2023-07-05 12:40:15.000000 bondzai.bootstrap-framework-0.0.8/README.md
+drwxr-xr-x   0 theo       (501) staff       (20)        0 2023-07-05 12:40:50.976828 bondzai.bootstrap-framework-0.0.8/bondzai/
+drwxr-xr-x   0 theo       (501) staff       (20)        0 2023-07-05 12:40:50.979543 bondzai.bootstrap-framework-0.0.8/bondzai/bootstrap_framework/
+-rw-r--r--   0 theo       (501) staff       (20)      212 2023-07-05 12:40:42.000000 bondzai.bootstrap-framework-0.0.8/bondzai/bootstrap_framework/__init__.py
+-rw-r--r--   0 theo       (501) staff       (20)     2696 2023-07-05 12:40:15.000000 bondzai.bootstrap-framework-0.0.8/bondzai/bootstrap_framework/bootstrap.py
+-rw-r--r--   0 theo       (501) staff       (20)    11284 2023-07-05 12:40:42.000000 bondzai.bootstrap-framework-0.0.8/bondzai/bootstrap_framework/dvs_agent.py
+-rw-r--r--   0 theo       (501) staff       (20)    14052 2023-07-05 12:40:15.000000 bondzai.bootstrap-framework-0.0.8/bondzai/bootstrap_framework/dvs_com.py
+-rw-r--r--   0 theo       (501) staff       (20)     8285 2023-07-05 12:40:42.000000 bondzai.bootstrap-framework-0.0.8/bondzai/bootstrap_framework/dvs_config.py
+-rw-r--r--   0 theo       (501) staff       (20)     3008 2023-07-05 12:40:15.000000 bondzai.bootstrap-framework-0.0.8/bondzai/bootstrap_framework/file_handler.py
+-rw-r--r--   0 theo       (501) staff       (20)      333 2023-07-05 12:40:15.000000 bondzai.bootstrap-framework-0.0.8/bondzai/bootstrap_framework/logger.py
+drwxr-xr-x   0 theo       (501) staff       (20)        0 2023-07-05 12:40:50.981445 bondzai.bootstrap-framework-0.0.8/bondzai.bootstrap_framework.egg-info/
+-rw-r--r--   0 theo       (501) staff       (20)      578 2023-07-05 12:40:50.000000 bondzai.bootstrap-framework-0.0.8/bondzai.bootstrap_framework.egg-info/PKG-INFO
+-rw-r--r--   0 theo       (501) staff       (20)      700 2023-07-05 12:40:50.000000 bondzai.bootstrap-framework-0.0.8/bondzai.bootstrap_framework.egg-info/SOURCES.txt
+-rw-r--r--   0 theo       (501) staff       (20)        1 2023-07-05 12:40:50.000000 bondzai.bootstrap-framework-0.0.8/bondzai.bootstrap_framework.egg-info/dependency_links.txt
+-rw-r--r--   0 theo       (501) staff       (20)        8 2023-07-05 12:40:50.000000 bondzai.bootstrap-framework-0.0.8/bondzai.bootstrap_framework.egg-info/namespace_packages.txt
+-rw-r--r--   0 theo       (501) staff       (20)       52 2023-07-05 12:40:50.000000 bondzai.bootstrap-framework-0.0.8/bondzai.bootstrap_framework.egg-info/requires.txt
+-rw-r--r--   0 theo       (501) staff       (20)       13 2023-07-05 12:40:50.000000 bondzai.bootstrap-framework-0.0.8/bondzai.bootstrap_framework.egg-info/top_level.txt
+-rw-r--r--   0 theo       (501) staff       (20)        1 2023-07-05 12:40:50.000000 bondzai.bootstrap-framework-0.0.8/bondzai.bootstrap_framework.egg-info/zip-safe
+-rw-r--r--   0 theo       (501) staff       (20)       71 2023-07-05 12:40:15.000000 bondzai.bootstrap-framework-0.0.8/pyproject.toml
+-rw-r--r--   0 theo       (501) staff       (20)      755 2023-07-05 12:40:50.982367 bondzai.bootstrap-framework-0.0.8/setup.cfg
```

### Comparing `bondzai.bootstrap-framework-0.0.7/NOTICE` & `bondzai.bootstrap-framework-0.0.8/NOTICE`

 * *Files identical despite different names*

### Comparing `bondzai.bootstrap-framework-0.0.7/PKG-INFO` & `bondzai.bootstrap-framework-0.0.8/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bondzai.bootstrap-framework
-Version: 0.0.7
+Version: 0.0.8
 Summary: Bondzai Bootstrap Framework
 Home-page: UNKNOWN
 Author: Bondzai
 License: Apache License 2.0
 Keywords: davinsy,bondzai
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
```

### Comparing `bondzai.bootstrap-framework-0.0.7/bondzai/bootstrap_framework/bootstrap.py` & `bondzai.bootstrap-framework-0.0.8/bondzai/bootstrap_framework/bootstrap.py`

 * *Files identical despite different names*

### Comparing `bondzai.bootstrap-framework-0.0.7/bondzai/bootstrap_framework/dvs_agent.py` & `bondzai.bootstrap-framework-0.0.8/bondzai/bootstrap_framework/dvs_agent.py`

 * *Files 7% similar despite different names*

```diff
@@ -86,16 +86,14 @@
             for vm in vms:
                 rowsize = max(rowsize, vm.get_vm_row_size())
 
             # create the VM table here 
             logger.debug(f"create_vm_table {rowsize}, {len(vms)} vms")
             self.vmTable = self.link.create_vm_table(rowsize,len(vms))
             
-            print(f" VM TABLE {type(self.vmTable)} value {self.vmTable}")
-
             uids = self.link.get_uids()
             print(uids)
             # add to config ?
             logger.debug("import_virtual_model")
             for vm in vms:
                 vm.set_uid2id(uids)
                 row,preproc = self.link.import_virtual_model(vm,self.vmTable)
@@ -107,19 +105,35 @@
                     vm_name = vm.get_name() 
                     if vm_name in bootstrap_info_list :
                         info = bootstrap_info_list[vm_name]
                         if "source" in info:
                             # keep this preprocess for the initial dataset (data-conditionning)
                             self.signalConditionning[info["source"]["id"]] = self.config.get_bootstrap_dataconditionning(self.preproc[vm_name])
 
-            logger.debug("create_dbm_table")
-            self.datTable = self.link.create_dbm_table(self.config.get_max_raw_data(),
-                                                       self.config.get_max_labels(),
-                                                       self.config.get_max_reg_len(),
-                                                       self.config.get_max_nb_raw_data()
+            max_raw_data = self.config.get_max_raw_data()
+            if (max_raw_data<1):
+                raise Exception("Max Raw Data Length (for DavinSy internal storage) not defined")
+            max_label = self.config.get_max_labels()
+            max_reg_len = self.config.get_max_reg_len()
+            if (max_label<1 and max_reg_len < 1):
+                raise Exception("Labels and regression size not defined")
+            max_nb_raw_data = self.config.get_max_nb_raw_data()
+            if (max_nb_raw_data < 1):
+                raise Exception("Max Raw Data Length (for DavinSy internal storage) not defined")
+
+            if (max_nb_raw_data*max_raw_data >  self.config.get_max_dbm_raw_data()):
+                max_nb_raw_data = int(self.config.get_max_dbm_raw_data()/max_raw_data)
+                self.config.set_max_nb_raw_data(max_nb_raw_data)
+                logger.warning(f"create_dbm_table limiting : {max_nb_raw_data} elements in DavinSy internal storage")
+
+            logger.debug(f"create_dbm_table max rawdata len: {max_raw_data}, {max_nb_raw_data} elements, with {max_label} label(s) or {max_reg_len} regression vector length")
+            self.datTable = self.link.create_dbm_table(max_raw_data,
+                                                       max_label,
+                                                       max_reg_len,
+                                                       max_nb_raw_data
                                                        )
             logger.debug("create_ctx_table")
 
             self.ctxTable = self.link.create_ctx_table(self.config.get_max_models())
 
             # create special row for correction
             # Row(self.datTable, -1, "lastin")
@@ -163,16 +177,16 @@
                         for labeltype in output:
                             label_type_id = self.config.get_item_id("labels", labeltype)
                             if not label_type_id:
                                 label_type_id = outputs_definition[labeltype].get("id", None)
                             label_value = output[labeltype]
 
                             # manage regression here
-                            if "labels" in outputs_definition[labeltype]:
-                                label_value_id = outputs_definition[labeltype]["labels"].get(label_value, None)
+                            if label_value in outputs_definition[labeltype]:
+                                label_value_id = outputs_definition[labeltype].get(label_value, None)
 
                                 if label_value_id is None:
                                     raise Exception(f"Unable to find label value id for {label_value}")
                                 
                                 groundthruth_for_davinsy.append(label_type_id)
                                 groundthruth_for_davinsy.append(label_value_id)
                             else:
@@ -188,15 +202,19 @@
 
                         logger.debug(f"loading file {filename}, GT {groundthruth_for_davinsy}")
                         sigVect = self.compute_raw_data(sourceid,data=raw_input)
                         if len(sigVect) < 1:
                             raise Exception(f"Unable to process data len  {str(len(raw_input))}")
 
                         isLoaded = self.load_one_raw_data(is_classification,inputVect=sigVect, expectedOutput=groundthruth_for_davinsy)
-                        ack += int(isLoaded)                
+                        ack += int(isLoaded)
+
+                        if ack >= (self.config.get_max_nb_raw_data()-1):
+                            logger.warn("DavinSy Internal Storage for raw data might be full")
+                            break
                 else:
                     logger.debug("INITIAL DATASET HAVE NO DEFINITION")
 
                 self.config.close_targz(my_tar)
         return ack
```

### Comparing `bondzai.bootstrap-framework-0.0.7/bondzai/bootstrap_framework/dvs_com.py` & `bondzai.bootstrap-framework-0.0.8/bondzai/bootstrap_framework/dvs_com.py`

 * *Files identical despite different names*

### Comparing `bondzai.bootstrap-framework-0.0.7/bondzai/bootstrap_framework/dvs_config.py` & `bondzai.bootstrap-framework-0.0.8/bondzai/bootstrap_framework/dvs_config.py`

 * *Files 24% similar despite different names*

```diff
@@ -41,14 +41,15 @@
         self.max_input_data = 0
         self.bootstrap_info = {}
         self.max_models = 0
         self.max_labels = 0
         self.max_reg_len = 0
         self.max_nb_raw_data = 3000
 
+        self.max_dbm_raw_data = int (0.8*(32 * 1024 * 1024)/4) # set DBM_TOTAL_ALLOCATED_PERSISTENT in platform_overload.h. limite to 80%
 
     def set_data_path(self,data_path):
         self.rootPath = data_path
 
     def preload_vms(self,vmFiles = None):
 
         if vmFiles is None:
@@ -98,22 +99,33 @@
                     self.max_models +=1    
                 else:
                     self.max_models += model["description"]["maxsplit"]
 
             bootstrap_info = vm.get_bootstrap_info()
             if bootstrap_info is not None :
                 self.bootstrap_info[vm.get_name()] =  bootstrap_info
-                if "source" in bootstrap_info:
-                    if self.max_raw_data < bootstrap_info["source"]["preproc_out_len"] :
-                        self.max_raw_data = bootstrap_info["source"]["preproc_out_len"]
-                    
-                    input_len = bootstrap_info["source"]["frame_len"] * bootstrap_info["source"]["max_frames_number"]
-                    if self.max_input_data < input_len :
-                        self.max_input_data = input_len
-                # max_nb_raw_data
+
+                if bootstrap_info["isDataconditionning"] == 1 : # in this case, take the ouput
+                    if "source" in bootstrap_info:
+                        if self.max_raw_data < bootstrap_info["source"]["preproc_out_len"] :
+                            self.max_raw_data = bootstrap_info["source"]["preproc_out_len"]
+                        
+                        input_len = bootstrap_info["source"]["frame_len"] * bootstrap_info["source"]["max_frames_number"]
+                        if self.max_input_data < input_len :
+                            self.max_input_data = input_len
+                else: # in this case without data conditionning, take the input (directly stored)
+                    if "source" in bootstrap_info:
+                        
+                        input_len = bootstrap_info["source"]["frame_len"] * bootstrap_info["source"]["max_frames_number"]
+                        if self.max_raw_data < input_len :
+                            self.max_raw_data = input_len
+
+                        if self.max_input_data < input_len :
+                            self.max_input_data = input_len
+
         return self.vm
     
     def load_initial_dataset_definition(self,path : Path = None):
         if path is None:
             path = self.rootPath / "dataset" /"myDataset.yml"
 
         if not Path.exists(path):
@@ -217,14 +229,20 @@
     
     def get_max_nb_raw_data(self):
         return self.max_nb_raw_data
 
     def get_nb_vm(self):
         return self.nb_vm
     
+    def set_max_dbm_raw_data (self,max_dbm_raw_data:int):
+        self.max_dbm_raw_data = max_dbm_raw_data
+
+    def get_max_dbm_raw_data (self):
+        return self.max_dbm_raw_data
+
     def get_bootstrap_info_list(self):
         return self.bootstrap_info
 
     def get_bootstrap_dataconditionning(self,preproc):
         return preproc[PreprocPhase.INFERENCE]
 
     def register_external_ops(self,opId: str,operation: callable):
```

### Comparing `bondzai.bootstrap-framework-0.0.7/bondzai/bootstrap_framework/file_handler.py` & `bondzai.bootstrap-framework-0.0.8/bondzai/bootstrap_framework/file_handler.py`

 * *Files identical despite different names*

### Comparing `bondzai.bootstrap-framework-0.0.7/bondzai.bootstrap_framework.egg-info/PKG-INFO` & `bondzai.bootstrap-framework-0.0.8/bondzai.bootstrap_framework.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bondzai.bootstrap-framework
-Version: 0.0.7
+Version: 0.0.8
 Summary: Bondzai Bootstrap Framework
 Home-page: UNKNOWN
 Author: Bondzai
 License: Apache License 2.0
 Keywords: davinsy,bondzai
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
```

### Comparing `bondzai.bootstrap-framework-0.0.7/bondzai.bootstrap_framework.egg-info/SOURCES.txt` & `bondzai.bootstrap-framework-0.0.8/bondzai.bootstrap_framework.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `bondzai.bootstrap-framework-0.0.7/setup.cfg` & `bondzai.bootstrap-framework-0.0.8/setup.cfg`

 * *Files identical despite different names*

