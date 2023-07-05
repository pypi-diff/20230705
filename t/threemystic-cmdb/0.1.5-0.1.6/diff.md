# Comparing `tmp/threemystic_cmdb-0.1.5.tar.gz` & `tmp/threemystic_cmdb-0.1.6.tar.gz`

## Comparing `threemystic_cmdb-0.1.5.tar` & `threemystic_cmdb-0.1.6.tar`

### file list

```diff
@@ -1,38 +1,38 @@
--rw-r--r--   0        0        0      191 2020-02-02 00:00:00.000000 threemystic_cmdb-0.1.5/threemystic_cloud_cmdb/__main__.py
--rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 threemystic_cmdb-0.1.5/threemystic_cloud_cmdb/__version__.py
--rw-r--r--   0        0        0     3560 2020-02-02 00:00:00.000000 threemystic_cmdb-0.1.5/threemystic_cloud_cmdb/cloud_cmdb_client.py
--rw-r--r--   0        0        0     4484 2020-02-02 00:00:00.000000 threemystic_cmdb-0.1.5/threemystic_cloud_cmdb/cli/__init__.py
--rw-r--r--   0        0        0     2910 2020-02-02 00:00:00.000000 threemystic_cmdb-0.1.5/threemystic_cloud_cmdb/cli/actions/base_class/base.py
--rw-r--r--   0        0        0      653 2020-02-02 00:00:00.000000 threemystic_cmdb-0.1.5/threemystic_cloud_cmdb/cli/actions/config/__init__.py
--rw-r--r--   0        0        0      526 2020-02-02 00:00:00.000000 threemystic_cmdb-0.1.5/threemystic_cloud_cmdb/cloud_providers/aws/__init__.py
--rw-r--r--   0        0        0      239 2020-02-02 00:00:00.000000 threemystic_cmdb-0.1.5/threemystic_cloud_cmdb/cloud_providers/aws/base_class/base.py
--rw-r--r--   0        0        0      287 2020-02-02 00:00:00.000000 threemystic_cmdb-0.1.5/threemystic_cloud_cmdb/cloud_providers/aws/client/__init__.py
--rw-r--r--   0        0        0     3018 2020-02-02 00:00:00.000000 threemystic_cmdb-0.1.5/threemystic_cloud_cmdb/cloud_providers/aws/config/step_1.py
--rw-r--r--   0        0        0      379 2020-02-02 00:00:00.000000 threemystic_cmdb-0.1.5/threemystic_cloud_cmdb/cloud_providers/aws/config/base_class/base.py
--rw-r--r--   0        0        0      541 2020-02-02 00:00:00.000000 threemystic_cmdb-0.1.5/threemystic_cloud_cmdb/cloud_providers/azure/__init__.py
--rw-r--r--   0        0        0      243 2020-02-02 00:00:00.000000 threemystic_cmdb-0.1.5/threemystic_cloud_cmdb/cloud_providers/azure/base_class/base.py
--rw-r--r--   0        0        0      294 2020-02-02 00:00:00.000000 threemystic_cmdb-0.1.5/threemystic_cloud_cmdb/cloud_providers/azure/client/__init__.py
--rw-r--r--   0        0        0     2663 2020-02-02 00:00:00.000000 threemystic_cmdb-0.1.5/threemystic_cloud_cmdb/cloud_providers/azure/client/actions/budget.py
--rw-r--r--   0        0        0     2804 2020-02-02 00:00:00.000000 threemystic_cmdb-0.1.5/threemystic_cloud_cmdb/cloud_providers/azure/client/actions/cloudstorage.py
--rw-r--r--   0        0        0     3309 2020-02-02 00:00:00.000000 threemystic_cmdb-0.1.5/threemystic_cloud_cmdb/cloud_providers/azure/client/actions/storage.py
--rw-r--r--   0        0        0    21346 2020-02-02 00:00:00.000000 threemystic_cmdb-0.1.5/threemystic_cloud_cmdb/cloud_providers/azure/client/actions/vm.py
--rw-r--r--   0        0        0     5201 2020-02-02 00:00:00.000000 threemystic_cmdb-0.1.5/threemystic_cloud_cmdb/cloud_providers/azure/client/actions/base_class/base.py
--rw-r--r--   0        0        0     3023 2020-02-02 00:00:00.000000 threemystic_cmdb-0.1.5/threemystic_cloud_cmdb/cloud_providers/azure/config/step_1.py
--rw-r--r--   0        0        0      385 2020-02-02 00:00:00.000000 threemystic_cmdb-0.1.5/threemystic_cloud_cmdb/cloud_providers/azure/config/base_class/base.py
--rw-r--r--   0        0        0     4597 2020-02-02 00:00:00.000000 threemystic_cmdb-0.1.5/threemystic_cloud_cmdb/cloud_providers/base_class/base.py
--rw-r--r--   0        0        0     7789 2020-02-02 00:00:00.000000 threemystic_cmdb-0.1.5/threemystic_cloud_cmdb/cloud_providers/base_class/base_client.py
--rw-r--r--   0        0        0    21382 2020-02-02 00:00:00.000000 threemystic_cmdb-0.1.5/threemystic_cloud_cmdb/cloud_providers/base_class/base_cmdb.py
--rw-r--r--   0        0        0      537 2020-02-02 00:00:00.000000 threemystic_cmdb-0.1.5/threemystic_cloud_cmdb/cloud_providers/general/__init__.py
--rw-r--r--   0        0        0     1006 2020-02-02 00:00:00.000000 threemystic_cmdb-0.1.5/threemystic_cloud_cmdb/cloud_providers/general/cmdb_connector/auto_cmdb_connector.py
--rw-r--r--   0        0        0    31108 2020-02-02 00:00:00.000000 threemystic_cmdb-0.1.5/threemystic_cloud_cmdb/cloud_providers/general/cmdb_connector/ms365.py
--rw-r--r--   0        0        0    13381 2020-02-02 00:00:00.000000 threemystic_cmdb-0.1.5/threemystic_cloud_cmdb/cloud_providers/general/cmdb_connector/base_class/base.py
--rw-r--r--   0        0        0     2888 2020-02-02 00:00:00.000000 threemystic_cmdb-0.1.5/threemystic_cloud_cmdb/cloud_providers/general/config/step_1.py
--rw-r--r--   0        0        0     5774 2020-02-02 00:00:00.000000 threemystic_cmdb-0.1.5/threemystic_cloud_cmdb/cloud_providers/general/config/step_2.py
--rw-r--r--   0        0        0    18353 2020-02-02 00:00:00.000000 threemystic_cmdb-0.1.5/threemystic_cloud_cmdb/cloud_providers/general/config/step_2_cloud_share.py
--rw-r--r--   0        0        0     5751 2020-02-02 00:00:00.000000 threemystic_cmdb-0.1.5/threemystic_cloud_cmdb/cloud_providers/general/config/step_3.py
--rw-r--r--   0        0        0      375 2020-02-02 00:00:00.000000 threemystic_cmdb-0.1.5/threemystic_cloud_cmdb/cloud_providers/general/config/base_class/base.py
--rw-r--r--   0        0        0     3078 2020-02-02 00:00:00.000000 threemystic_cmdb-0.1.5/.gitignore
--rw-r--r--   0        0        0     1068 2020-02-02 00:00:00.000000 threemystic_cmdb-0.1.5/LICENSE
--rw-r--r--   0        0        0     1300 2020-02-02 00:00:00.000000 threemystic_cmdb-0.1.5/README.md
--rw-r--r--   0        0        0     3163 2020-02-02 00:00:00.000000 threemystic_cmdb-0.1.5/pyproject.toml
--rw-r--r--   0        0        0     2586 2020-02-02 00:00:00.000000 threemystic_cmdb-0.1.5/PKG-INFO
+-rw-r--r--   0        0        0      191 2020-02-02 00:00:00.000000 threemystic_cmdb-0.1.6/threemystic_cloud_cmdb/__main__.py
+-rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 threemystic_cmdb-0.1.6/threemystic_cloud_cmdb/__version__.py
+-rw-r--r--   0        0        0     3560 2020-02-02 00:00:00.000000 threemystic_cmdb-0.1.6/threemystic_cloud_cmdb/cloud_cmdb_client.py
+-rw-r--r--   0        0        0     4484 2020-02-02 00:00:00.000000 threemystic_cmdb-0.1.6/threemystic_cloud_cmdb/cli/__init__.py
+-rw-r--r--   0        0        0     2910 2020-02-02 00:00:00.000000 threemystic_cmdb-0.1.6/threemystic_cloud_cmdb/cli/actions/base_class/base.py
+-rw-r--r--   0        0        0      653 2020-02-02 00:00:00.000000 threemystic_cmdb-0.1.6/threemystic_cloud_cmdb/cli/actions/config/__init__.py
+-rw-r--r--   0        0        0      526 2020-02-02 00:00:00.000000 threemystic_cmdb-0.1.6/threemystic_cloud_cmdb/cloud_providers/aws/__init__.py
+-rw-r--r--   0        0        0      239 2020-02-02 00:00:00.000000 threemystic_cmdb-0.1.6/threemystic_cloud_cmdb/cloud_providers/aws/base_class/base.py
+-rw-r--r--   0        0        0      287 2020-02-02 00:00:00.000000 threemystic_cmdb-0.1.6/threemystic_cloud_cmdb/cloud_providers/aws/client/__init__.py
+-rw-r--r--   0        0        0     3018 2020-02-02 00:00:00.000000 threemystic_cmdb-0.1.6/threemystic_cloud_cmdb/cloud_providers/aws/config/step_1.py
+-rw-r--r--   0        0        0      417 2020-02-02 00:00:00.000000 threemystic_cmdb-0.1.6/threemystic_cloud_cmdb/cloud_providers/aws/config/base_class/base.py
+-rw-r--r--   0        0        0      541 2020-02-02 00:00:00.000000 threemystic_cmdb-0.1.6/threemystic_cloud_cmdb/cloud_providers/azure/__init__.py
+-rw-r--r--   0        0        0      243 2020-02-02 00:00:00.000000 threemystic_cmdb-0.1.6/threemystic_cloud_cmdb/cloud_providers/azure/base_class/base.py
+-rw-r--r--   0        0        0      294 2020-02-02 00:00:00.000000 threemystic_cmdb-0.1.6/threemystic_cloud_cmdb/cloud_providers/azure/client/__init__.py
+-rw-r--r--   0        0        0     2663 2020-02-02 00:00:00.000000 threemystic_cmdb-0.1.6/threemystic_cloud_cmdb/cloud_providers/azure/client/actions/budget.py
+-rw-r--r--   0        0        0     2804 2020-02-02 00:00:00.000000 threemystic_cmdb-0.1.6/threemystic_cloud_cmdb/cloud_providers/azure/client/actions/cloudstorage.py
+-rw-r--r--   0        0        0     3309 2020-02-02 00:00:00.000000 threemystic_cmdb-0.1.6/threemystic_cloud_cmdb/cloud_providers/azure/client/actions/storage.py
+-rw-r--r--   0        0        0    21346 2020-02-02 00:00:00.000000 threemystic_cmdb-0.1.6/threemystic_cloud_cmdb/cloud_providers/azure/client/actions/vm.py
+-rw-r--r--   0        0        0     5201 2020-02-02 00:00:00.000000 threemystic_cmdb-0.1.6/threemystic_cloud_cmdb/cloud_providers/azure/client/actions/base_class/base.py
+-rw-r--r--   0        0        0     3023 2020-02-02 00:00:00.000000 threemystic_cmdb-0.1.6/threemystic_cloud_cmdb/cloud_providers/azure/config/step_1.py
+-rw-r--r--   0        0        0      423 2020-02-02 00:00:00.000000 threemystic_cmdb-0.1.6/threemystic_cloud_cmdb/cloud_providers/azure/config/base_class/base.py
+-rw-r--r--   0        0        0     7190 2020-02-02 00:00:00.000000 threemystic_cmdb-0.1.6/threemystic_cloud_cmdb/cloud_providers/base_class/base.py
+-rw-r--r--   0        0        0     7789 2020-02-02 00:00:00.000000 threemystic_cmdb-0.1.6/threemystic_cloud_cmdb/cloud_providers/base_class/base_client.py
+-rw-r--r--   0        0        0    21382 2020-02-02 00:00:00.000000 threemystic_cmdb-0.1.6/threemystic_cloud_cmdb/cloud_providers/base_class/base_cmdb.py
+-rw-r--r--   0        0        0      537 2020-02-02 00:00:00.000000 threemystic_cmdb-0.1.6/threemystic_cloud_cmdb/cloud_providers/general/__init__.py
+-rw-r--r--   0        0        0     1006 2020-02-02 00:00:00.000000 threemystic_cmdb-0.1.6/threemystic_cloud_cmdb/cloud_providers/general/cmdb_connector/auto_cmdb_connector.py
+-rw-r--r--   0        0        0    31108 2020-02-02 00:00:00.000000 threemystic_cmdb-0.1.6/threemystic_cloud_cmdb/cloud_providers/general/cmdb_connector/ms365.py
+-rw-r--r--   0        0        0    13381 2020-02-02 00:00:00.000000 threemystic_cmdb-0.1.6/threemystic_cloud_cmdb/cloud_providers/general/cmdb_connector/base_class/base.py
+-rw-r--r--   0        0        0     3018 2020-02-02 00:00:00.000000 threemystic_cmdb-0.1.6/threemystic_cloud_cmdb/cloud_providers/general/config/step_1.py
+-rw-r--r--   0        0        0     6484 2020-02-02 00:00:00.000000 threemystic_cmdb-0.1.6/threemystic_cloud_cmdb/cloud_providers/general/config/step_2.py
+-rw-r--r--   0        0        0    18763 2020-02-02 00:00:00.000000 threemystic_cmdb-0.1.6/threemystic_cloud_cmdb/cloud_providers/general/config/step_2_cloud_share.py
+-rw-r--r--   0        0        0     5893 2020-02-02 00:00:00.000000 threemystic_cmdb-0.1.6/threemystic_cloud_cmdb/cloud_providers/general/config/step_3.py
+-rw-r--r--   0        0        0      413 2020-02-02 00:00:00.000000 threemystic_cmdb-0.1.6/threemystic_cloud_cmdb/cloud_providers/general/config/base_class/base.py
+-rw-r--r--   0        0        0     3078 2020-02-02 00:00:00.000000 threemystic_cmdb-0.1.6/.gitignore
+-rw-r--r--   0        0        0     1068 2020-02-02 00:00:00.000000 threemystic_cmdb-0.1.6/LICENSE
+-rw-r--r--   0        0        0     1300 2020-02-02 00:00:00.000000 threemystic_cmdb-0.1.6/README.md
+-rw-r--r--   0        0        0     3163 2020-02-02 00:00:00.000000 threemystic_cmdb-0.1.6/pyproject.toml
+-rw-r--r--   0        0        0     2586 2020-02-02 00:00:00.000000 threemystic_cmdb-0.1.6/PKG-INFO
```

### Comparing `threemystic_cmdb-0.1.5/threemystic_cloud_cmdb/cloud_cmdb_client.py` & `threemystic_cmdb-0.1.6/threemystic_cloud_cmdb/cloud_cmdb_client.py`

 * *Files identical despite different names*

### Comparing `threemystic_cmdb-0.1.5/threemystic_cloud_cmdb/cli/__init__.py` & `threemystic_cmdb-0.1.6/threemystic_cloud_cmdb/cli/__init__.py`

 * *Files identical despite different names*

### Comparing `threemystic_cmdb-0.1.5/threemystic_cloud_cmdb/cli/actions/base_class/base.py` & `threemystic_cmdb-0.1.6/threemystic_cloud_cmdb/cli/actions/base_class/base.py`

 * *Files identical despite different names*

### Comparing `threemystic_cmdb-0.1.5/threemystic_cloud_cmdb/cli/actions/config/__init__.py` & `threemystic_cmdb-0.1.6/threemystic_cloud_cmdb/cli/actions/config/__init__.py`

 * *Files identical despite different names*

### Comparing `threemystic_cmdb-0.1.5/threemystic_cloud_cmdb/cloud_providers/aws/__init__.py` & `threemystic_cmdb-0.1.6/threemystic_cloud_cmdb/cloud_providers/aws/__init__.py`

 * *Files identical despite different names*

### Comparing `threemystic_cmdb-0.1.5/threemystic_cloud_cmdb/cloud_providers/aws/config/step_1.py` & `threemystic_cmdb-0.1.6/threemystic_cloud_cmdb/cloud_providers/aws/config/step_1.py`

 * *Files identical despite different names*

### Comparing `threemystic_cmdb-0.1.5/threemystic_cloud_cmdb/cloud_providers/azure/__init__.py` & `threemystic_cmdb-0.1.6/threemystic_cloud_cmdb/cloud_providers/azure/__init__.py`

 * *Files identical despite different names*

### Comparing `threemystic_cmdb-0.1.5/threemystic_cloud_cmdb/cloud_providers/azure/client/actions/budget.py` & `threemystic_cmdb-0.1.6/threemystic_cloud_cmdb/cloud_providers/azure/client/actions/budget.py`

 * *Files identical despite different names*

### Comparing `threemystic_cmdb-0.1.5/threemystic_cloud_cmdb/cloud_providers/azure/client/actions/cloudstorage.py` & `threemystic_cmdb-0.1.6/threemystic_cloud_cmdb/cloud_providers/azure/client/actions/cloudstorage.py`

 * *Files identical despite different names*

### Comparing `threemystic_cmdb-0.1.5/threemystic_cloud_cmdb/cloud_providers/azure/client/actions/storage.py` & `threemystic_cmdb-0.1.6/threemystic_cloud_cmdb/cloud_providers/azure/client/actions/storage.py`

 * *Files identical despite different names*

### Comparing `threemystic_cmdb-0.1.5/threemystic_cloud_cmdb/cloud_providers/azure/client/actions/vm.py` & `threemystic_cmdb-0.1.6/threemystic_cloud_cmdb/cloud_providers/azure/client/actions/vm.py`

 * *Files identical despite different names*

### Comparing `threemystic_cmdb-0.1.5/threemystic_cloud_cmdb/cloud_providers/azure/client/actions/base_class/base.py` & `threemystic_cmdb-0.1.6/threemystic_cloud_cmdb/cloud_providers/azure/client/actions/base_class/base.py`

 * *Files identical despite different names*

### Comparing `threemystic_cmdb-0.1.5/threemystic_cloud_cmdb/cloud_providers/azure/config/step_1.py` & `threemystic_cmdb-0.1.6/threemystic_cloud_cmdb/cloud_providers/azure/config/step_1.py`

 * *Files identical despite different names*

### Comparing `threemystic_cmdb-0.1.5/threemystic_cloud_cmdb/cloud_providers/base_class/base.py` & `threemystic_cmdb-0.1.6/threemystic_cloud_cmdb/cloud_providers/base_class/base.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,15 +1,79 @@
 from threemystic_common.base_class.base_provider import base
+from threemystic_cloud_cmdb.cli import cloud_cmdb_cli
+from threemystic_common.base_class.generate_data.generate_data_handlers import generate_data_handlers
+from threemystic_cloud_data_client.cloud_providers.base_class.base import cloud_data_client_provider_base as main_cloud_data_client
 
 class cloud_cmdb_provider_base(base):
   def __init__(self, *args, **kwargs):
     if "provider" not in kwargs:
       kwargs["provider"] = self.get_default_provider()
     super().__init__(*args, **kwargs)
     
+  def _setup_another_config(self):
+    response = self.get_common().generate_data().generate(
+      generate_data_config = {
+        "repeat_config": {
+            "validation": lambda item: self.get_common().helper_type().bool().is_bool(check_value= item),
+            "messages":{
+              "validation": f"Valid options for Yes are: {self.get_common().helper_type().bool().is_true_values()}",
+            },
+            "conversion": lambda item: self.get_common().helper_type().bool().is_true(check_value= item),
+            "desc": f"Do you want to setup another provider?: {self.get_common().helper_type().bool().is_true_values()}",
+            "default": None,
+            "handler": generate_data_handlers.get_handler(handler= "base"),
+            "optional": True
+        }
+      }
+    )
+
+    if response is None:
+      return
+    
+    if response.get("repeat_config") is None:
+      return
+    
+    if response.get("repeat_config").get("formated") is not True:
+      return
+    
+    print()
+    print()
+    print("-------------------------------------------------------------------------")
+    print()
+    print()
+
+    cloud_cmdb_cli().process_client_action("config")
+  
+  def update_general_config_completed(self, status, *args, **kwargs):
+    self.get_config()["_config_process"] = status
+    self._save_config()
+  
+  def is_data_client_config_completed(self, *args, **kwargs):
+    cloud_client = main_cloud_data_client( common= self.get_common(), logger_name= "cmdb_init", logger= self.get_common().get_logger())
+    
+    return cloud_client.is_provider_config_completed()
+
+  
+  def ensure_data_client_config_completed(self, *args, **kwargs):
+    if self.is_data_client_config_completed():
+      return True
+    
+    print("Data Client needs to be configured")
+    cloud_client = main_cloud_data_client( common= self.get_common(), logger_name= "cmdb_init", logger= self.get_common().get_logger())
+    cloud_client._setup_another_config(force_config= True)
+    
+    return False
+
+    
+  def is_provider_config_completed_only(self, *args, **kwargs):
+    return self.get_config().get("_config_process") is True 
+
+  def is_provider_config_completed(self, *args, **kwargs):
+    return self.is_provider_config_completed_only() and self.is_data_client_config_completed()
+    
   
   def get_main_directory_name(self, *args, **kwargs):
     return "cmdb"  
   
   def get_supported_cloud_share(self, *args, **kwargs):
     return ["ms365"]
 
@@ -83,16 +147,16 @@
   def get_config(self, refresh = False, *args, **kwargs):
     if hasattr(self, "_config_data") and not refresh:
       return self._config_data
     
     self._config_data = self.__load_config()    
     return self.get_config(*args, **kwargs)
 
-  def _update_config(self,config_key, config_value,  *args, **kwargs):
-     self.get_config(refresh = True)[config_key] = config_value
+  def _update_config(self,config_key, config_value, refresh= False,  *args, **kwargs):
+     self.get_config(refresh = refresh)[config_key] = config_value
      
   def _save_config(self, *args, **kwargs):
      if not self.config_path().parent.exists():
        self.config_path().parent.mkdir(parents= True)
      self.config_path().write_text(
       data= self.get_common().helper_yaml().dumps(data= self.get_config())
      )
```

### Comparing `threemystic_cmdb-0.1.5/threemystic_cloud_cmdb/cloud_providers/base_class/base_client.py` & `threemystic_cmdb-0.1.6/threemystic_cloud_cmdb/cloud_providers/base_class/base_client.py`

 * *Files identical despite different names*

### Comparing `threemystic_cmdb-0.1.5/threemystic_cloud_cmdb/cloud_providers/base_class/base_cmdb.py` & `threemystic_cmdb-0.1.6/threemystic_cloud_cmdb/cloud_providers/base_class/base_cmdb.py`

 * *Files identical despite different names*

### Comparing `threemystic_cmdb-0.1.5/threemystic_cloud_cmdb/cloud_providers/general/__init__.py` & `threemystic_cmdb-0.1.6/threemystic_cloud_cmdb/cloud_providers/general/__init__.py`

 * *Files identical despite different names*

### Comparing `threemystic_cmdb-0.1.5/threemystic_cloud_cmdb/cloud_providers/general/cmdb_connector/auto_cmdb_connector.py` & `threemystic_cmdb-0.1.6/threemystic_cloud_cmdb/cloud_providers/general/cmdb_connector/auto_cmdb_connector.py`

 * *Files identical despite different names*

### Comparing `threemystic_cmdb-0.1.5/threemystic_cloud_cmdb/cloud_providers/general/cmdb_connector/ms365.py` & `threemystic_cmdb-0.1.6/threemystic_cloud_cmdb/cloud_providers/general/cmdb_connector/ms365.py`

 * *Files identical despite different names*

### Comparing `threemystic_cmdb-0.1.5/threemystic_cloud_cmdb/cloud_providers/general/cmdb_connector/base_class/base.py` & `threemystic_cmdb-0.1.6/threemystic_cloud_cmdb/cloud_providers/general/cmdb_connector/base_class/base.py`

 * *Files identical despite different names*

### Comparing `threemystic_cmdb-0.1.5/threemystic_cloud_cmdb/cloud_providers/general/config/step_1.py` & `threemystic_cmdb-0.1.6/threemystic_cloud_cmdb/cloud_providers/general/config/step_1.py`

 * *Files 6% similar despite different names*

```diff
@@ -46,25 +46,28 @@
       print("-----------------------------")
       print()
       print()
       print("Base Configuration is updated")
       print()
       print()
       print("-----------------------------")
+      from threemystic_cloud_cmdb.cloud_providers.general.config.step_2 import cloud_cmdb_general_config_step_2 as step
+      next_step = step(common= self.get_common(), logger= self.get_logger())
+      
+      if not self.is_provider_config_completed_only():
+        self.update_general_config_completed(status= "step1")
+      next_step.step()
     else:
       print("-----------------------------")
       print()
       print()
       print("Base Configuration NOT updated")
       print()
       print()
       print("-----------------------------")    
     
     
-    from threemystic_cloud_cmdb.cloud_providers.general.config.step_2 import cloud_cmdb_general_config_step_2 as step
-    next_step = step(common= self.get_common(), logger= self.get_logger())
     
-    next_step.step()
```

### Comparing `threemystic_cmdb-0.1.5/threemystic_cloud_cmdb/cloud_providers/general/config/step_2.py` & `threemystic_cmdb-0.1.6/threemystic_cloud_cmdb/cloud_providers/general/config/step_2.py`

 * *Files 6% similar despite different names*

```diff
@@ -36,15 +36,22 @@
       }
     )
     
     if response is None:
       return
 
     if not self.get_common().helper_type().bool().is_true(check_value= response.get("cmdb_cloud_share").get("formated")):
+      from threemystic_cloud_cmdb.cloud_providers.general.config.step_3 import cloud_cmdb_general_config_step_3 as step
+      next_step = step(common= self.get_common(), logger= self.get_logger())
+      
+      if not self.is_provider_config_completed_only():
+        self.update_general_config_completed(status= "step2")
+
       if len(self.get_config_cloud_share()) < 1:
+        next_step.step(cloud_share= self.get_cloud_share_config_value(config_key= "type"))
         return
       
       response = self.get_common().generate_data().generate(
         generate_data_config = {
           "reset_cloud_share": {
             "validation": lambda item: self.get_common().helper_type().bool().is_bool(check_value= item),
             "messages":{
@@ -55,19 +62,20 @@
             "default": None,
             "handler": generate_data_handlers.get_handler(handler= "base"),
             "optional": True
           }
         }
       )
       if response is None:
-        return
+        next_step.step(cloud_share= self.get_cloud_share_config_value(config_key= "type"))
 
       if self.get_common().helper_type().bool().is_true(check_value= response.get("reset_cloud_share").get("formated")):
         self.reset_config_cloud_share()
       
+      next_step.step(cloud_share= self.get_cloud_share_config_value(config_key= "type"))
       return
 
     response = self.get_common().generate_data().generate(
       generate_data_config = {
         "type": {
           "validation": lambda item: self.get_common().helper_type().string().set_case(string_value= item, case= "lower") in self.get_supported_cloud_share(),
           "messages":{
@@ -102,18 +110,21 @@
     if(response is not None):
       for key, item in response.items():
         self._update_config_cloud_share(config_key= key, config_value= item.get("formated"))    
       if self.get_cloud_share_config_value(config_key= response.get("type").get("formated")) is None:
         self._update_config_cloud_share(config_key= response.get("type").get("formated"), config_value= {})
       self._save_config_cloud_share()
       
-
+      
       from threemystic_cloud_cmdb.cloud_providers.general.config.step_2_cloud_share import cloud_cmdb_general_config_step_2_cloud_share as step
       next_step = step(common= self.get_common(), logger= self.get_logger())
       
+      if not self.is_provider_config_completed_only():
+        self.update_general_config_completed(status= "step2")
+        
       next_step.step(cloud_share= self.get_cloud_share_config_value(config_key= "type"))
 
       print("-----------------------------")
       print()
       print()
       print("CMDB Cloud Share is updated")
       print()
```

### Comparing `threemystic_cmdb-0.1.5/threemystic_cloud_cmdb/cloud_providers/general/config/step_2_cloud_share.py` & `threemystic_cmdb-0.1.6/threemystic_cloud_cmdb/cloud_providers/general/config/step_2_cloud_share.py`

 * *Files 1% similar despite different names*

```diff
@@ -430,17 +430,26 @@
       
       
       
     self.get_cloud_share_config_value(
       config_key= cloud_share
     )["drive_id"] = drive_item_ids
     self._save_config_cloud_share()
+    
     print("-----------------------------")
     print()
     print(f"Drive ID Updated: {drive_item_ids[-1]}")
     print()
     print("-----------------------------")
 
+    from threemystic_cloud_cmdb.cloud_providers.general.config.step_3 import cloud_cmdb_general_config_step_3 as step
+    next_step = step(common= self.get_common(), logger= self.get_logger())
+    
+    if not self.is_provider_config_completed_only():
+      self.update_general_config_completed(status= "CloudShare")
+
+    next_step.step(cloud_share= self.get_cloud_share_config_value(config_key= "type"))
+
```

### Comparing `threemystic_cmdb-0.1.5/threemystic_cloud_cmdb/cloud_providers/general/config/step_3.py` & `threemystic_cmdb-0.1.6/threemystic_cloud_cmdb/cloud_providers/general/config/step_3.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from threemystic_cloud_cmdb.cloud_providers.general.config.base_class.base import cloud_cmdb_general_config_base as base
 from threemystic_common.base_class.generate_data.generate_data_handlers import generate_data_handlers
 
 
 
-class cloud_cmdb_general_config_step_2(base):
+class cloud_cmdb_general_config_step_3(base):
   def __init__(self, *args, **kwargs):
     super().__init__(logger_name= "cloud_cmdb_general_config_step_1", *args, **kwargs)
     
   def step_tag_question(self, *args, **kwargs):
     response = self.get_common().generate_data().generate(
       generate_data_config = {
         "name": {
@@ -34,15 +34,17 @@
       }
     )
 
   def step(self, *args, **kwargs):
     if not super().step(run_base_config= True):
       return
     
-    
+    #Not Implemented
+    self.update_general_config_completed(status= True)
+    return
     print("-----------------------------")
     print()
     print()
     print("CMDB Cloud Share")
     print()
     print()
     print("-----------------------------")
@@ -112,14 +114,15 @@
       for key, item in response.items():
         self._update_config_cloud_share(config_key= key, config_value= item.get("formated"))
       self._save_config_cloud_share()
 
       from threemystic_cloud_cmdb.cloud_providers.general.config.step_2_cloud_share import cloud_cmdb_general_config_step_2_cloud_share as step
       next_step = step(common= self.get_common(), logger= self.get_logger())
       
+      self.update_general_config_completed(status= "step3")
       next_step.step(cloud_share= self.get_cloud_share_config_value(config_key= "cloud_share_location"))
 
       print("-----------------------------")
       print()
       print()
       print("CMDB Cloud Share is updated")
       print()
```

### Comparing `threemystic_cmdb-0.1.5/.gitignore` & `threemystic_cmdb-0.1.6/.gitignore`

 * *Files identical despite different names*

### Comparing `threemystic_cmdb-0.1.5/LICENSE` & `threemystic_cmdb-0.1.6/LICENSE`

 * *Files identical despite different names*

### Comparing `threemystic_cmdb-0.1.5/README.md` & `threemystic_cmdb-0.1.6/README.md`

 * *Files identical despite different names*

### Comparing `threemystic_cmdb-0.1.5/pyproject.toml` & `threemystic_cmdb-0.1.6/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -23,16 +23,16 @@
   "Programming Language :: Python :: 3.10",
   "Programming Language :: Python :: 3.11",
   "Programming Language :: Python :: Implementation :: CPython",
   "Programming Language :: Python :: Implementation :: PyPy",
 ]
 dependencies = [
   "colorama; platform_system == 'Windows'",
-  "threemystic-common >= 0.1.3",
-  "threemystic-cloud-data-client >= 0.1.5",
+  "threemystic-common >= 0.1.4",
+  "threemystic-cloud-data-client >= 0.1.6",
   "typing-extensions >= 4.4.0",
   "asyncio >= 3.4.3",
   "tqdm >= 4.65.0",
   "openpyxl >= 3.1.2",
   "lxml >= 4.9.2",
   "msgraph-sdk >= 1.0.0a12",  
   "polling2 >= 0.5.0",
```

### Comparing `threemystic_cmdb-0.1.5/PKG-INFO` & `threemystic_cmdb-0.1.6/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: threemystic-cmdb
-Version: 0.1.5
+Version: 0.1.6
 Summary: A lightweight CMDB to help you track your cloud resources from various providers
 Project-URL: Homepage, https://github.com/3MysticApes/3mystic_cloud_cmdb
 Project-URL: Bug Tracker, https://github.com/3MysticApes/3mystic_cloud_cmdb/issues
 Author: Ron Truex
 License-Expression: MIT
 License-File: LICENSE
 Classifier: License :: OSI Approved :: MIT License
@@ -19,16 +19,16 @@
 Requires-Python: >=3.8
 Requires-Dist: asyncio>=3.4.3
 Requires-Dist: colorama; platform_system == 'Windows'
 Requires-Dist: lxml>=4.9.2
 Requires-Dist: msgraph-sdk>=1.0.0a12
 Requires-Dist: openpyxl>=3.1.2
 Requires-Dist: polling2>=0.5.0
-Requires-Dist: threemystic-cloud-data-client>=0.1.5
-Requires-Dist: threemystic-common>=0.1.3
+Requires-Dist: threemystic-cloud-data-client>=0.1.6
+Requires-Dist: threemystic-common>=0.1.4
 Requires-Dist: tqdm>=4.65.0
 Requires-Dist: typing-extensions>=4.4.0
 Description-Content-Type: text/markdown
 
 # 3mystic_cmdb
 A Lightweight Multi Cloud CMDB (Configuration management database)
 Currently supports AWS/Azure
```

