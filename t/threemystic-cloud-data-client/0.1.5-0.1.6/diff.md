# Comparing `tmp/threemystic_cloud_data_client-0.1.5.tar.gz` & `tmp/threemystic_cloud_data_client-0.1.6.tar.gz`

## Comparing `threemystic_cloud_data_client-0.1.5.tar` & `threemystic_cloud_data_client-0.1.6.tar`

### file list

```diff
@@ -1,36 +1,40 @@
--rw-r--r--   0        0        0      212 2020-02-02 00:00:00.000000 threemystic_cloud_data_client-0.1.5/threemystic_cloud_data_client/__main__.py
--rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 threemystic_cloud_data_client-0.1.5/threemystic_cloud_data_client/__version__.py
--rw-r--r--   0        0        0     3895 2020-02-02 00:00:00.000000 threemystic_cloud_data_client-0.1.5/threemystic_cloud_data_client/cloud_data_client.py
--rw-r--r--   0        0        0     4150 2020-02-02 00:00:00.000000 threemystic_cloud_data_client-0.1.5/threemystic_cloud_data_client/cli/__init__.py
--rw-r--r--   0        0        0     2950 2020-02-02 00:00:00.000000 threemystic_cloud_data_client-0.1.5/threemystic_cloud_data_client/cli/actions/base_class/base.py
--rw-r--r--   0        0        0      702 2020-02-02 00:00:00.000000 threemystic_cloud_data_client-0.1.5/threemystic_cloud_data_client/cli/actions/config/__init__.py
--rw-r--r--   0        0        0      568 2020-02-02 00:00:00.000000 threemystic_cloud_data_client-0.1.5/threemystic_cloud_data_client/cloud_providers/aws/__init__.py
--rw-r--r--   0        0        0      260 2020-02-02 00:00:00.000000 threemystic_cloud_data_client-0.1.5/threemystic_cloud_data_client/cloud_providers/aws/base_class/base.py
--rw-r--r--   0        0        0      287 2020-02-02 00:00:00.000000 threemystic_cloud_data_client-0.1.5/threemystic_cloud_data_client/cloud_providers/aws/client/__init__.py
--rw-r--r--   0        0        0     3028 2020-02-02 00:00:00.000000 threemystic_cloud_data_client-0.1.5/threemystic_cloud_data_client/cloud_providers/aws/config/step_1.py
--rw-r--r--   0        0        0      400 2020-02-02 00:00:00.000000 threemystic_cloud_data_client-0.1.5/threemystic_cloud_data_client/cloud_providers/aws/config/base_class/base.py
--rw-r--r--   0        0        0      583 2020-02-02 00:00:00.000000 threemystic_cloud_data_client-0.1.5/threemystic_cloud_data_client/cloud_providers/azure/__init__.py
--rw-r--r--   0        0        0      264 2020-02-02 00:00:00.000000 threemystic_cloud_data_client-0.1.5/threemystic_cloud_data_client/cloud_providers/azure/base_class/base.py
--rw-r--r--   0        0        0      331 2020-02-02 00:00:00.000000 threemystic_cloud_data_client-0.1.5/threemystic_cloud_data_client/cloud_providers/azure/client/__init__.py
--rw-r--r--   0        0        0    13738 2020-02-02 00:00:00.000000 threemystic_cloud_data_client-0.1.5/threemystic_cloud_data_client/cloud_providers/azure/client/actions/budget.py
--rw-r--r--   0        0        0     4728 2020-02-02 00:00:00.000000 threemystic_cloud_data_client-0.1.5/threemystic_cloud_data_client/cloud_providers/azure/client/actions/certificates.py
--rw-r--r--   0        0        0     5548 2020-02-02 00:00:00.000000 threemystic_cloud_data_client-0.1.5/threemystic_cloud_data_client/cloud_providers/azure/client/actions/cloudstorage.py
--rw-r--r--   0        0        0     4718 2020-02-02 00:00:00.000000 threemystic_cloud_data_client-0.1.5/threemystic_cloud_data_client/cloud_providers/azure/client/actions/secrets.py
--rw-r--r--   0        0        0    13101 2020-02-02 00:00:00.000000 threemystic_cloud_data_client-0.1.5/threemystic_cloud_data_client/cloud_providers/azure/client/actions/storage.py
--rw-r--r--   0        0        0    11884 2020-02-02 00:00:00.000000 threemystic_cloud_data_client-0.1.5/threemystic_cloud_data_client/cloud_providers/azure/client/actions/vm.py
--rw-r--r--   0        0        0     3174 2020-02-02 00:00:00.000000 threemystic_cloud_data_client-0.1.5/threemystic_cloud_data_client/cloud_providers/azure/client/actions/vmss.py
--rw-r--r--   0        0        0      986 2020-02-02 00:00:00.000000 threemystic_cloud_data_client-0.1.5/threemystic_cloud_data_client/cloud_providers/azure/client/actions/base_class/base.py
--rw-r--r--   0        0        0     3046 2020-02-02 00:00:00.000000 threemystic_cloud_data_client-0.1.5/threemystic_cloud_data_client/cloud_providers/azure/config/step_1.py
--rw-r--r--   0        0        0      406 2020-02-02 00:00:00.000000 threemystic_cloud_data_client-0.1.5/threemystic_cloud_data_client/cloud_providers/azure/config/base_class/base.py
--rw-r--r--   0        0        0     4112 2020-02-02 00:00:00.000000 threemystic_cloud_data_client-0.1.5/threemystic_cloud_data_client/cloud_providers/base_class/base.py
--rw-r--r--   0        0        0    10662 2020-02-02 00:00:00.000000 threemystic_cloud_data_client-0.1.5/threemystic_cloud_data_client/cloud_providers/base_class/base_client.py
--rw-r--r--   0        0        0    20546 2020-02-02 00:00:00.000000 threemystic_cloud_data_client-0.1.5/threemystic_cloud_data_client/cloud_providers/base_class/base_data.py
--rw-r--r--   0        0        0      593 2020-02-02 00:00:00.000000 threemystic_cloud_data_client-0.1.5/threemystic_cloud_data_client/cloud_providers/general/__init__.py
--rw-r--r--   0        0        0     3547 2020-02-02 00:00:00.000000 threemystic_cloud_data_client-0.1.5/threemystic_cloud_data_client/cloud_providers/general/config/step_1.py
--rw-r--r--   0        0        0      396 2020-02-02 00:00:00.000000 threemystic_cloud_data_client-0.1.5/threemystic_cloud_data_client/cloud_providers/general/config/base_class/base.py
--rw-r--r--   0        0        0     1799 2020-02-02 00:00:00.000000 threemystic_cloud_data_client-0.1.5/.gitignore
--rw-r--r--   0        0        0     1068 2020-02-02 00:00:00.000000 threemystic_cloud_data_client-0.1.5/LICENSE
--rw-r--r--   0        0        0     1280 2020-02-02 00:00:00.000000 threemystic_cloud_data_client-0.1.5/README.md
--rw-r--r--   0        0        0      692 2020-02-02 00:00:00.000000 threemystic_cloud_data_client-0.1.5/hatch.toml
--rw-r--r--   0        0        0     3557 2020-02-02 00:00:00.000000 threemystic_cloud_data_client-0.1.5/pyproject.toml
--rw-r--r--   0        0        0     2943 2020-02-02 00:00:00.000000 threemystic_cloud_data_client-0.1.5/PKG-INFO
+-rw-r--r--   0        0        0      212 2020-02-02 00:00:00.000000 threemystic_cloud_data_client-0.1.6/threemystic_cloud_data_client/__main__.py
+-rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 threemystic_cloud_data_client-0.1.6/threemystic_cloud_data_client/__version__.py
+-rw-r--r--   0        0        0     3895 2020-02-02 00:00:00.000000 threemystic_cloud_data_client-0.1.6/threemystic_cloud_data_client/cloud_data_client.py
+-rw-r--r--   0        0        0     4150 2020-02-02 00:00:00.000000 threemystic_cloud_data_client-0.1.6/threemystic_cloud_data_client/cli/__init__.py
+-rw-r--r--   0        0        0     2950 2020-02-02 00:00:00.000000 threemystic_cloud_data_client-0.1.6/threemystic_cloud_data_client/cli/actions/base_class/base.py
+-rw-r--r--   0        0        0      702 2020-02-02 00:00:00.000000 threemystic_cloud_data_client-0.1.6/threemystic_cloud_data_client/cli/actions/config/__init__.py
+-rw-r--r--   0        0        0      568 2020-02-02 00:00:00.000000 threemystic_cloud_data_client-0.1.6/threemystic_cloud_data_client/cloud_providers/aws/__init__.py
+-rw-r--r--   0        0        0      260 2020-02-02 00:00:00.000000 threemystic_cloud_data_client-0.1.6/threemystic_cloud_data_client/cloud_providers/aws/base_class/base.py
+-rw-r--r--   0        0        0      287 2020-02-02 00:00:00.000000 threemystic_cloud_data_client-0.1.6/threemystic_cloud_data_client/cloud_providers/aws/client/__init__.py
+-rw-r--r--   0        0        0     3032 2020-02-02 00:00:00.000000 threemystic_cloud_data_client-0.1.6/threemystic_cloud_data_client/cloud_providers/aws/config/step_1.py
+-rw-r--r--   0        0        0      443 2020-02-02 00:00:00.000000 threemystic_cloud_data_client-0.1.6/threemystic_cloud_data_client/cloud_providers/aws/config/base_class/base.py
+-rw-r--r--   0        0        0      583 2020-02-02 00:00:00.000000 threemystic_cloud_data_client-0.1.6/threemystic_cloud_data_client/cloud_providers/azure/__init__.py
+-rw-r--r--   0        0        0      264 2020-02-02 00:00:00.000000 threemystic_cloud_data_client-0.1.6/threemystic_cloud_data_client/cloud_providers/azure/base_class/base.py
+-rw-r--r--   0        0        0      331 2020-02-02 00:00:00.000000 threemystic_cloud_data_client-0.1.6/threemystic_cloud_data_client/cloud_providers/azure/client/__init__.py
+-rw-r--r--   0        0        0    13738 2020-02-02 00:00:00.000000 threemystic_cloud_data_client-0.1.6/threemystic_cloud_data_client/cloud_providers/azure/client/actions/budget.py
+-rw-r--r--   0        0        0     4754 2020-02-02 00:00:00.000000 threemystic_cloud_data_client-0.1.6/threemystic_cloud_data_client/cloud_providers/azure/client/actions/certificates.py
+-rw-r--r--   0        0        0     5548 2020-02-02 00:00:00.000000 threemystic_cloud_data_client-0.1.6/threemystic_cloud_data_client/cloud_providers/azure/client/actions/cloudstorage.py
+-rw-r--r--   0        0        0     2539 2020-02-02 00:00:00.000000 threemystic_cloud_data_client-0.1.6/threemystic_cloud_data_client/cloud_providers/azure/client/actions/database.py
+-rw-r--r--   0        0        0     2498 2020-02-02 00:00:00.000000 threemystic_cloud_data_client-0.1.6/threemystic_cloud_data_client/cloud_providers/azure/client/actions/datawarehouse.py
+-rw-r--r--   0        0        0     2525 2020-02-02 00:00:00.000000 threemystic_cloud_data_client-0.1.6/threemystic_cloud_data_client/cloud_providers/azure/client/actions/dns.py
+-rw-r--r--   0        0        0     2550 2020-02-02 00:00:00.000000 threemystic_cloud_data_client-0.1.6/threemystic_cloud_data_client/cloud_providers/azure/client/actions/memorydb.py
+-rw-r--r--   0        0        0     5772 2020-02-02 00:00:00.000000 threemystic_cloud_data_client-0.1.6/threemystic_cloud_data_client/cloud_providers/azure/client/actions/secrets.py
+-rw-r--r--   0        0        0    13101 2020-02-02 00:00:00.000000 threemystic_cloud_data_client-0.1.6/threemystic_cloud_data_client/cloud_providers/azure/client/actions/storage.py
+-rw-r--r--   0        0        0    11884 2020-02-02 00:00:00.000000 threemystic_cloud_data_client-0.1.6/threemystic_cloud_data_client/cloud_providers/azure/client/actions/vm.py
+-rw-r--r--   0        0        0     3174 2020-02-02 00:00:00.000000 threemystic_cloud_data_client-0.1.6/threemystic_cloud_data_client/cloud_providers/azure/client/actions/vmss.py
+-rw-r--r--   0        0        0      986 2020-02-02 00:00:00.000000 threemystic_cloud_data_client-0.1.6/threemystic_cloud_data_client/cloud_providers/azure/client/actions/base_class/base.py
+-rw-r--r--   0        0        0     2917 2020-02-02 00:00:00.000000 threemystic_cloud_data_client-0.1.6/threemystic_cloud_data_client/cloud_providers/azure/config/step_1.py
+-rw-r--r--   0        0        0      445 2020-02-02 00:00:00.000000 threemystic_cloud_data_client-0.1.6/threemystic_cloud_data_client/cloud_providers/azure/config/base_class/base.py
+-rw-r--r--   0        0        0     7106 2020-02-02 00:00:00.000000 threemystic_cloud_data_client-0.1.6/threemystic_cloud_data_client/cloud_providers/base_class/base.py
+-rw-r--r--   0        0        0    10648 2020-02-02 00:00:00.000000 threemystic_cloud_data_client-0.1.6/threemystic_cloud_data_client/cloud_providers/base_class/base_client.py
+-rw-r--r--   0        0        0    20546 2020-02-02 00:00:00.000000 threemystic_cloud_data_client-0.1.6/threemystic_cloud_data_client/cloud_providers/base_class/base_data.py
+-rw-r--r--   0        0        0      593 2020-02-02 00:00:00.000000 threemystic_cloud_data_client-0.1.6/threemystic_cloud_data_client/cloud_providers/general/__init__.py
+-rw-r--r--   0        0        0     3604 2020-02-02 00:00:00.000000 threemystic_cloud_data_client-0.1.6/threemystic_cloud_data_client/cloud_providers/general/config/step_1.py
+-rw-r--r--   0        0        0      396 2020-02-02 00:00:00.000000 threemystic_cloud_data_client-0.1.6/threemystic_cloud_data_client/cloud_providers/general/config/base_class/base.py
+-rw-r--r--   0        0        0     1799 2020-02-02 00:00:00.000000 threemystic_cloud_data_client-0.1.6/.gitignore
+-rw-r--r--   0        0        0     1068 2020-02-02 00:00:00.000000 threemystic_cloud_data_client-0.1.6/LICENSE
+-rw-r--r--   0        0        0     1280 2020-02-02 00:00:00.000000 threemystic_cloud_data_client-0.1.6/README.md
+-rw-r--r--   0        0        0      692 2020-02-02 00:00:00.000000 threemystic_cloud_data_client-0.1.6/hatch.toml
+-rw-r--r--   0        0        0     3535 2020-02-02 00:00:00.000000 threemystic_cloud_data_client-0.1.6/pyproject.toml
+-rw-r--r--   0        0        0     2921 2020-02-02 00:00:00.000000 threemystic_cloud_data_client-0.1.6/PKG-INFO
```

### Comparing `threemystic_cloud_data_client-0.1.5/threemystic_cloud_data_client/cloud_data_client.py` & `threemystic_cloud_data_client-0.1.6/threemystic_cloud_data_client/cloud_data_client.py`

 * *Files identical despite different names*

### Comparing `threemystic_cloud_data_client-0.1.5/threemystic_cloud_data_client/cli/__init__.py` & `threemystic_cloud_data_client-0.1.6/threemystic_cloud_data_client/cli/__init__.py`

 * *Files identical despite different names*

### Comparing `threemystic_cloud_data_client-0.1.5/threemystic_cloud_data_client/cli/actions/base_class/base.py` & `threemystic_cloud_data_client-0.1.6/threemystic_cloud_data_client/cli/actions/base_class/base.py`

 * *Files identical despite different names*

### Comparing `threemystic_cloud_data_client-0.1.5/threemystic_cloud_data_client/cli/actions/config/__init__.py` & `threemystic_cloud_data_client-0.1.6/threemystic_cloud_data_client/cli/actions/config/__init__.py`

 * *Files identical despite different names*

### Comparing `threemystic_cloud_data_client-0.1.5/threemystic_cloud_data_client/cloud_providers/aws/__init__.py` & `threemystic_cloud_data_client-0.1.6/threemystic_cloud_data_client/cloud_providers/aws/__init__.py`

 * *Files identical despite different names*

### Comparing `threemystic_cloud_data_client-0.1.5/threemystic_cloud_data_client/cloud_providers/aws/config/step_1.py` & `threemystic_cloud_data_client-0.1.6/threemystic_cloud_data_client/cloud_providers/aws/config/step_1.py`

 * *Files 1% similar despite different names*

```diff
@@ -38,15 +38,15 @@
     if not super().step(run_base_config= True):
       return
     
     print()
     print()
     print()
     print(f"No additional config is required at this time for Data Client: {self.get_provider()}")
-
+    
     self.check_cloud_client(*args, **kwargs)
 
     response = self.get_common().generate_data().generate(
       generate_data_config = {
         "base_config": {
           "validation": lambda item: self.get_common().helper_type().bool().is_bool(check_value= item),
           "messages":{
```

### Comparing `threemystic_cloud_data_client-0.1.5/threemystic_cloud_data_client/cloud_providers/azure/__init__.py` & `threemystic_cloud_data_client-0.1.6/threemystic_cloud_data_client/cloud_providers/azure/__init__.py`

 * *Files identical despite different names*

### Comparing `threemystic_cloud_data_client-0.1.5/threemystic_cloud_data_client/cloud_providers/azure/client/actions/budget.py` & `threemystic_cloud_data_client-0.1.6/threemystic_cloud_data_client/cloud_providers/azure/client/actions/budget.py`

 * *Files identical despite different names*

### Comparing `threemystic_cloud_data_client-0.1.5/threemystic_cloud_data_client/cloud_providers/azure/client/actions/certificates.py` & `threemystic_cloud_data_client-0.1.6/threemystic_cloud_data_client/cloud_providers/azure/client/actions/certificates.py`

 * *Files 7% similar despite different names*

```diff
@@ -59,35 +59,34 @@
     
     keyvaults = await self.__process_get_resources_key_vaults(account= account)
 
     for kv in keyvaults.values():
       print(self.get_cloud_client().serialize_azresource(resource= kv))
       break
 
-    raise Exception("test")
-
     return {
         "account": account,
-        "data": [ self.get_common().helper_type().dictionary().merge_dictionary([
-            {},
-            self.get_base_return_data(
-              account= self.get_cloud_client().serialize_azresource(resource= account),
-              resource_id= self.get_cloud_client().get_resource_id_from_resource(resource= item),
-              resource= item,
-              region= self.get_cloud_client().get_azresource_location(resource= item),
-              resource_groups= [self.get_cloud_client().get_resource_group_from_resource(resource= item)],
-            ),
-            {
-              "extra_resource": self.get_cloud_client().serialize_azresource(tasks["resource"].result().get(self.get_cloud_client().get_resource_id_from_resource(resource= item))),
-              "extra_availability_set": tasks["availability_sets"].result().get(self.get_cloud_client().get_resource_id_from_resource(resource= item)),
-              "extra_nics": tasks["nics"].result().get(self.get_cloud_client().get_resource_id_from_resource(resource= item)),
-              "extra_load_balancers": await self._process_account_data_get_vm_load_balancers(
-                vm_nics= tasks["nics"].result().get(self.get_cloud_client().get_resource_id_from_resource(resource= item)),
-                load_balancers_by_nics = tasks["load_balancers"].result()
-              ),
-            },
-          ]) for item in self.get_cloud_client().sdk_request(
-           tenant= self.get_cloud_client().get_tenant_id(tenant= account, is_account= True), 
-           lambda_sdk_command=lambda: client.virtual_machines.list_all()
-          )
+        "data": [ 
+          # self.get_common().helper_type().dictionary().merge_dictionary([
+          #   {},
+          #   self.get_base_return_data(
+          #     account= self.get_cloud_client().serialize_azresource(resource= account),
+          #     resource_id= self.get_cloud_client().get_resource_id_from_resource(resource= item),
+          #     resource= item,
+          #     region= self.get_cloud_client().get_azresource_location(resource= item),
+          #     resource_groups= [self.get_cloud_client().get_resource_group_from_resource(resource= item)],
+          #   ),
+          #   {
+          #     "extra_resource": self.get_cloud_client().serialize_azresource(tasks["resource"].result().get(self.get_cloud_client().get_resource_id_from_resource(resource= item))),
+          #     "extra_availability_set": tasks["availability_sets"].result().get(self.get_cloud_client().get_resource_id_from_resource(resource= item)),
+          #     "extra_nics": tasks["nics"].result().get(self.get_cloud_client().get_resource_id_from_resource(resource= item)),
+          #     "extra_load_balancers": await self._process_account_data_get_vm_load_balancers(
+          #       vm_nics= tasks["nics"].result().get(self.get_cloud_client().get_resource_id_from_resource(resource= item)),
+          #       load_balancers_by_nics = tasks["load_balancers"].result()
+          #     ),
+          #   },
+          # ]) for item in self.get_cloud_client().sdk_request(
+          #  tenant= self.get_cloud_client().get_tenant_id(tenant= account, is_account= True), 
+          #  lambda_sdk_command=lambda: client.virtual_machines.list_all()
+          # )
         ]
     }
```

### Comparing `threemystic_cloud_data_client-0.1.5/threemystic_cloud_data_client/cloud_providers/azure/client/actions/cloudstorage.py` & `threemystic_cloud_data_client-0.1.6/threemystic_cloud_data_client/cloud_providers/azure/client/actions/cloudstorage.py`

 * *Files identical despite different names*

### Comparing `threemystic_cloud_data_client-0.1.5/threemystic_cloud_data_client/cloud_providers/azure/client/actions/secrets.py` & `threemystic_cloud_data_client-0.1.6/threemystic_cloud_data_client/cloud_providers/azure/client/actions/secrets.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,22 +1,39 @@
 from threemystic_cloud_data_client.cloud_providers.azure.client.actions.base_class.base import cloud_data_client_azure_client_action_base as base
 import asyncio
 from azure.mgmt.keyvault import KeyVaultManagementClient
 from azure.keyvault.secrets import SecretClient
 from azure.keyvault.keys import KeyClient
+from azure.keyvault.administration import KeyVaultAccessControlClient
 
 
 class cloud_data_client_azure_client_action(base):
   def __init__(self, *args, **kwargs):
     super().__init__(
       data_action="secrets", 
       logger_name= "cloud_data_client_azure_client_action_secrets", 
       uniqueid_lambda = lambda: True,
       *args, **kwargs)
   
+  async def __process_get_resources_key_vault_access_key(self, account, key_vault, *args, **kwargs):    
+    try:
+      client = KeyVaultAccessControlClient(vault_url= f'https://{key_vault}.vault.azure.net/', credential= self.get_cloud_client().get_tenant_credential(tenant= self.get_cloud_client().get_tenant_id(tenant= account, is_account= True)), subscription_id= self.get_cloud_client().get_account_id(account= account))
+      
+      # oid = print(self.get_cloud_client().get_tenant_credential_full(tenant= self.get_cloud_client().get_tenant_id(tenant= account, is_account= True)).get("jwt").get("oid"))
+
+
+      return [ key for key in self.get_cloud_client().sdk_request(
+          tenant= self.get_cloud_client().get_tenant_id(tenant= account, is_account= True), 
+          lambda_sdk_command=lambda: client.list_properties_of_keys()
+        )
+      ]
+           
+    except Exception as err:
+      return []
+    
   async def __process_get_resources_key_vault_keys(self, account, key_vault, *args, **kwargs):    
     try:
       client = KeyClient(vault_url= f'https://{key_vault}.vault.azure.net/', credential= self.get_cloud_client().get_tenant_credential(tenant= self.get_cloud_client().get_tenant_id(tenant= account, is_account= True)), subscription_id= self.get_cloud_client().get_account_id(account= account))
       
       return [ key for key in self.get_cloud_client().sdk_request(
           tenant= self.get_cloud_client().get_tenant_id(tenant= account, is_account= True), 
           lambda_sdk_command=lambda: client.list_properties_of_keys()
@@ -53,41 +70,42 @@
            
     except Exception as err:
       return {} 
 
   
   async def _process_account_data(self, account, loop, *args, **kwargs):
     
-    keyvaults = await self.__process_get_resources_key_vaults(account= account)
-
-    for kv in keyvaults.values():
-      print(self.get_cloud_client().serialize_azresource(resource= kv))
-      break
-
-    raise Exception("test")
+    # print(account)
+    
+    # keyvaults = await self.__process_get_resources_key_vaults(account= account)
 
+    # for kv in keyvaults.values():
+    #   print(self.get_cloud_client().serialize_azresource(resource= kv))
+    #   break
+    
     return {
         "account": account,
-        "data": [ self.get_common().helper_type().dictionary().merge_dictionary([
-            {},
-            self.get_base_return_data(
-              account= self.get_cloud_client().serialize_azresource(resource= account),
-              resource_id= self.get_cloud_client().get_resource_id_from_resource(resource= item),
-              resource= item,
-              region= self.get_cloud_client().get_azresource_location(resource= item),
-              resource_groups= [self.get_cloud_client().get_resource_group_from_resource(resource= item)],
-            ),
-            {
-              "extra_resource": self.get_cloud_client().serialize_azresource(tasks["resource"].result().get(self.get_cloud_client().get_resource_id_from_resource(resource= item))),
-              "extra_availability_set": tasks["availability_sets"].result().get(self.get_cloud_client().get_resource_id_from_resource(resource= item)),
-              "extra_nics": tasks["nics"].result().get(self.get_cloud_client().get_resource_id_from_resource(resource= item)),
-              "extra_load_balancers": await self._process_account_data_get_vm_load_balancers(
-                vm_nics= tasks["nics"].result().get(self.get_cloud_client().get_resource_id_from_resource(resource= item)),
-                load_balancers_by_nics = tasks["load_balancers"].result()
-              ),
-            },
-          ]) for item in self.get_cloud_client().sdk_request(
-           tenant= self.get_cloud_client().get_tenant_id(tenant= account, is_account= True), 
-           lambda_sdk_command=lambda: client.virtual_machines.list_all()
-          )
+        "data": [
+          #  self.get_common().helper_type().dictionary().merge_dictionary([
+          #   {},
+          #   self.get_base_return_data(
+          #     account= self.get_cloud_client().serialize_azresource(resource= account),
+          #     resource_id= self.get_cloud_client().get_resource_id_from_resource(resource= item),
+          #     resource= item,
+          #     region= self.get_cloud_client().get_azresource_location(resource= item),
+          #     resource_groups= [self.get_cloud_client().get_resource_group_from_resource(resource= item)],
+          #   ),
+          #   {
+          #     "extra_resource": self.get_cloud_client().serialize_azresource(tasks["resource"].result().get(self.get_cloud_client().get_resource_id_from_resource(resource= item))),
+          #     "extra_availability_set": tasks["availability_sets"].result().get(self.get_cloud_client().get_resource_id_from_resource(resource= item)),
+          #     "extra_nics": tasks["nics"].result().get(self.get_cloud_client().get_resource_id_from_resource(resource= item)),
+          #     "extra_load_balancers": await self._process_account_data_get_vm_load_balancers(
+          #       vm_nics= tasks["nics"].result().get(self.get_cloud_client().get_resource_id_from_resource(resource= item)),
+          #       load_balancers_by_nics = tasks["load_balancers"].result()
+          #     ),
+          #   },
+          # ]) for item in self.get_cloud_client().sdk_request(
+          #  tenant= self.get_cloud_client().get_tenant_id(tenant= account, is_account= True), 
+          #  lambda_sdk_command=lambda: client.virtual_machines.list_all()
+          # )
         ]
     }
```

### Comparing `threemystic_cloud_data_client-0.1.5/threemystic_cloud_data_client/cloud_providers/azure/client/actions/storage.py` & `threemystic_cloud_data_client-0.1.6/threemystic_cloud_data_client/cloud_providers/azure/client/actions/storage.py`

 * *Files identical despite different names*

### Comparing `threemystic_cloud_data_client-0.1.5/threemystic_cloud_data_client/cloud_providers/azure/client/actions/vm.py` & `threemystic_cloud_data_client-0.1.6/threemystic_cloud_data_client/cloud_providers/azure/client/actions/vm.py`

 * *Files identical despite different names*

### Comparing `threemystic_cloud_data_client-0.1.5/threemystic_cloud_data_client/cloud_providers/azure/client/actions/vmss.py` & `threemystic_cloud_data_client-0.1.6/threemystic_cloud_data_client/cloud_providers/azure/client/actions/vmss.py`

 * *Files identical despite different names*

### Comparing `threemystic_cloud_data_client-0.1.5/threemystic_cloud_data_client/cloud_providers/azure/client/actions/base_class/base.py` & `threemystic_cloud_data_client-0.1.6/threemystic_cloud_data_client/cloud_providers/azure/client/actions/base_class/base.py`

 * *Files identical despite different names*

### Comparing `threemystic_cloud_data_client-0.1.5/threemystic_cloud_data_client/cloud_providers/azure/config/step_1.py` & `threemystic_cloud_data_client-0.1.6/threemystic_cloud_data_client/cloud_providers/azure/config/step_1.py`

 * *Files 7% similar despite different names*

```diff
@@ -26,27 +26,26 @@
     )
 
     if response is None:
       return
     
     if not self.get_common().helper_type().bool().is_true(check_value= response.get("base_config").get("formated")):
       return
-    
-    from threemystic_cloud_client.cloud_providers.aws import cloud_client_aws as client
-    client( common= self.get_common(), logger= self.get_common().get_logger()).action_config()
+
 
   def step(self, *args, **kwargs):
     
     if not super().step(run_base_config= True):
       return
     
     print()
     print()
     print()
     print(f"No additional config is required at this time for Data Client: {self.get_provider()}")
+    # if steps are added will need to add a complete step
     
     self.check_cloud_client(*args, **kwargs)
     
 
     response = self.get_common().generate_data().generate(
       generate_data_config = {
         "base_config": {
```

### Comparing `threemystic_cloud_data_client-0.1.5/threemystic_cloud_data_client/cloud_providers/base_class/base_client.py` & `threemystic_cloud_data_client-0.1.6/threemystic_cloud_data_client/cloud_providers/base_class/base_client.py`

 * *Files 2% similar despite different names*

```diff
@@ -39,21 +39,21 @@
       "--budget": {
         "default": None, 
         "const": "budget",
         "dest": "data_action",
         "help": "Data Action: This pulls a general budget to provide you insights in your accounts/subscriptions",
         "action": 'store_const'
       },
-      # "--secrets": {
-      #   "default": None, 
-      #   "const": "secrets",
-      #   "dest": "data_action",
-      #   "help": "Data Action: Pulls Key Vaults Secrets and Keys / Paramater Store",
-      #   "action": 'store_const'
-      # },
+      "--secrets": {
+        "default": None, 
+        "const": "secrets",
+        "dest": "data_action",
+        "help": "Data Action: Pulls Key Vaults Secrets and Keys / Paramater Store",
+        "action": 'store_const'
+      },
       "--storage": {
         "default": None, 
         "const": "storage",
         "dest": "data_action",
         "help": "Data Action: This pulls either VM Disks or EC2 Storage depending on the provider",
         "action": 'store_const'
       },
```

### Comparing `threemystic_cloud_data_client-0.1.5/threemystic_cloud_data_client/cloud_providers/base_class/base_data.py` & `threemystic_cloud_data_client-0.1.6/threemystic_cloud_data_client/cloud_providers/base_class/base_data.py`

 * *Files identical despite different names*

### Comparing `threemystic_cloud_data_client-0.1.5/threemystic_cloud_data_client/cloud_providers/general/__init__.py` & `threemystic_cloud_data_client-0.1.6/threemystic_cloud_data_client/cloud_providers/general/__init__.py`

 * *Files identical despite different names*

### Comparing `threemystic_cloud_data_client-0.1.5/threemystic_cloud_data_client/cloud_providers/general/config/step_1.py` & `threemystic_cloud_data_client-0.1.6/threemystic_cloud_data_client/cloud_providers/general/config/step_1.py`

 * *Files 1% similar despite different names*

```diff
@@ -50,14 +50,15 @@
       }
     )
 
     if(response is not None):
       for key, item in response.items():
         self._update_config(config_key= key, config_value= item.get("formated"))
       self._save_config()
+      self.update_general_config_completed(status= True)
       print("-----------------------------")
       print()
       print()
       print("Base Configuration is updated")
       print()
       print()
       print("-----------------------------")
```

### Comparing `threemystic_cloud_data_client-0.1.5/.gitignore` & `threemystic_cloud_data_client-0.1.6/.gitignore`

 * *Files identical despite different names*

### Comparing `threemystic_cloud_data_client-0.1.5/LICENSE` & `threemystic_cloud_data_client-0.1.6/LICENSE`

 * *Files identical despite different names*

### Comparing `threemystic_cloud_data_client-0.1.5/README.md` & `threemystic_cloud_data_client-0.1.6/README.md`

 * *Files identical despite different names*

### Comparing `threemystic_cloud_data_client-0.1.5/hatch.toml` & `threemystic_cloud_data_client-0.1.6/hatch.toml`

 * *Files identical despite different names*

### Comparing `threemystic_cloud_data_client-0.1.5/pyproject.toml` & `threemystic_cloud_data_client-0.1.6/pyproject.toml`

 * *Files 14% similar despite different names*

```diff
@@ -28,25 +28,25 @@
 dependencies = [
   "colorama; platform_system == 'Windows'",
   "threemystic-common >= 0.1.3",
   "threemystic-cloud-client >= 0.1.5",
   "typing-extensions >= 4.4.0",
   "asyncio >= 3.4.3",
   "tqdm >= 4.65.0",
-  "azure-mgmt-subscription >= 3.1.1",
-  "azure-mgmt-managementgroups >= 1.0.0",
-  "azure-mgmt-resourcegraph >= 8.0.0",
-  "azure-mgmt-costmanagement >= 4.0.0",
-  "azure-mgmt-network >= 23.1.0",
-  "azure-mgmt-keyvault >= 10.2.2",
-  "azure-mgmt-monitor >= 6.0.1",
-  "azure-keyvault-administration >= 4.3.0",
-  "azure-keyvault-certificates >= 4.7.0",
-  "azure-keyvault-keys >= 4.8.0",
-  "azure-keyvault-secrets >= 4.7.0",
+  "azure-mgmt-subscription == 3.*",
+  "azure-mgmt-managementgroups == 1.*",
+  "azure-mgmt-resourcegraph == 8.*",
+  "azure-mgmt-costmanagement == 4.*",
+  "azure-mgmt-network == 23.*",
+  "azure-mgmt-monitor == 5.*",
+  "azure-mgmt-keyvault == 10.*",
+  "azure-keyvault-administration == 4.*",
+  "azure-keyvault-certificates == 4.*",
+  "azure-keyvault-keys == 4.*",
+  "azure-keyvault-secrets == 4.*",
 
 ]
 dynamic = ["version"]
 
 [project.urls]
 "Homepage" = "https://github.com/3MysticApes/3mystic_cloud_data_client"
 "Bug Tracker" = "https://github.com/3MysticApes/3mystic_cloud_data_client/issues"
```

### Comparing `threemystic_cloud_data_client-0.1.5/PKG-INFO` & `threemystic_cloud_data_client-0.1.6/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: threemystic-cloud-data-client
-Version: 0.1.5
+Version: 0.1.6
 Summary: A tool for collecting data from various cloud providers
 Project-URL: Homepage, https://github.com/3MysticApes/3mystic_cloud_data_client
 Project-URL: Bug Tracker, https://github.com/3MysticApes/3mystic_cloud_data_client/issues
 Author: Ron Truex
 License-Expression: MIT
 License-File: LICENSE
 Classifier: License :: OSI Approved :: MIT License
@@ -14,25 +14,25 @@
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Programming Language :: Python :: Implementation :: PyPy
 Requires-Python: >=3.8
 Requires-Dist: asyncio>=3.4.3
-Requires-Dist: azure-keyvault-administration>=4.3.0
-Requires-Dist: azure-keyvault-certificates>=4.7.0
-Requires-Dist: azure-keyvault-keys>=4.8.0
-Requires-Dist: azure-keyvault-secrets>=4.7.0
-Requires-Dist: azure-mgmt-costmanagement>=4.0.0
-Requires-Dist: azure-mgmt-keyvault>=10.2.2
-Requires-Dist: azure-mgmt-managementgroups>=1.0.0
-Requires-Dist: azure-mgmt-monitor>=6.0.1
-Requires-Dist: azure-mgmt-network>=23.1.0
-Requires-Dist: azure-mgmt-resourcegraph>=8.0.0
-Requires-Dist: azure-mgmt-subscription>=3.1.1
+Requires-Dist: azure-keyvault-administration==4.*
+Requires-Dist: azure-keyvault-certificates==4.*
+Requires-Dist: azure-keyvault-keys==4.*
+Requires-Dist: azure-keyvault-secrets==4.*
+Requires-Dist: azure-mgmt-costmanagement==4.*
+Requires-Dist: azure-mgmt-keyvault==10.*
+Requires-Dist: azure-mgmt-managementgroups==1.*
+Requires-Dist: azure-mgmt-monitor==5.*
+Requires-Dist: azure-mgmt-network==23.*
+Requires-Dist: azure-mgmt-resourcegraph==8.*
+Requires-Dist: azure-mgmt-subscription==3.*
 Requires-Dist: colorama; platform_system == 'Windows'
 Requires-Dist: threemystic-cloud-client>=0.1.5
 Requires-Dist: threemystic-common>=0.1.3
 Requires-Dist: tqdm>=4.65.0
 Requires-Dist: typing-extensions>=4.4.0
 Description-Content-Type: text/markdown
```

