# Comparing `tmp/threemystic_cloud_client-0.1.5.tar.gz` & `tmp/threemystic_cloud_client-0.1.6.tar.gz`

## Comparing `threemystic_cloud_client-0.1.5.tar` & `threemystic_cloud_client-0.1.6.tar`

### file list

```diff
@@ -1,38 +1,38 @@
--rw-r--r--   0        0        0      197 2020-02-02 00:00:00.000000 threemystic_cloud_client-0.1.5/threemystic_cloud_client/__main__.py
--rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 threemystic_cloud_client-0.1.5/threemystic_cloud_client/__version__.py
--rw-r--r--   0        0        0     3168 2020-02-02 00:00:00.000000 threemystic_cloud_client-0.1.5/threemystic_cloud_client/cloud_client.py
--rw-r--r--   0        0        0     4011 2020-02-02 00:00:00.000000 threemystic_cloud_client-0.1.5/threemystic_cloud_client/cli/__init__.py
--rw-r--r--   0        0        0     2519 2020-02-02 00:00:00.000000 threemystic_cloud_client-0.1.5/threemystic_cloud_client/cli/actions/base_class/base.py
--rw-r--r--   0        0        0      631 2020-02-02 00:00:00.000000 threemystic_cloud_client-0.1.5/threemystic_cloud_client/cli/actions/config/__init__.py
--rw-r--r--   0        0        0      657 2020-02-02 00:00:00.000000 threemystic_cloud_client-0.1.5/threemystic_cloud_client/cli/actions/test/__init__.py
--rw-r--r--   0        0        0     4074 2020-02-02 00:00:00.000000 threemystic_cloud_client-0.1.5/threemystic_cloud_client/cli/actions/token/__init__.py
--rw-r--r--   0        0        0      911 2020-02-02 00:00:00.000000 threemystic_cloud_client-0.1.5/threemystic_cloud_client/cloud_providers/aws/__init__.py
--rw-r--r--   0        0        0     3591 2020-02-02 00:00:00.000000 threemystic_cloud_client-0.1.5/threemystic_cloud_client/cloud_providers/aws/base_class/base.py
--rw-r--r--   0        0        0     2045 2020-02-02 00:00:00.000000 threemystic_cloud_client-0.1.5/threemystic_cloud_client/cloud_providers/aws/client/auto_client.py
--rw-r--r--   0        0        0    12051 2020-02-02 00:00:00.000000 threemystic_cloud_client-0.1.5/threemystic_cloud_client/cloud_providers/aws/client/sso.py
--rw-r--r--   0        0        0    21260 2020-02-02 00:00:00.000000 threemystic_cloud_client-0.1.5/threemystic_cloud_client/cloud_providers/aws/client/base_class/base.py
--rw-r--r--   0        0        0     1528 2020-02-02 00:00:00.000000 threemystic_cloud_client-0.1.5/threemystic_cloud_client/cloud_providers/aws/config/step_1.py
--rw-r--r--   0        0        0    15698 2020-02-02 00:00:00.000000 threemystic_cloud_client-0.1.5/threemystic_cloud_client/cloud_providers/aws/config/step_2.py
--rw-r--r--   0        0        0     3451 2020-02-02 00:00:00.000000 threemystic_cloud_client-0.1.5/threemystic_cloud_client/cloud_providers/aws/config/base_class/base.py
--rw-r--r--   0        0        0     1671 2020-02-02 00:00:00.000000 threemystic_cloud_client-0.1.5/threemystic_cloud_client/cloud_providers/aws/test/step_1.py
--rw-r--r--   0        0        0     1095 2020-02-02 00:00:00.000000 threemystic_cloud_client-0.1.5/threemystic_cloud_client/cloud_providers/aws/test/step_2.py
--rw-r--r--   0        0        0      642 2020-02-02 00:00:00.000000 threemystic_cloud_client-0.1.5/threemystic_cloud_client/cloud_providers/aws/test/base_class/base.py
--rw-r--r--   0        0        0      874 2020-02-02 00:00:00.000000 threemystic_cloud_client-0.1.5/threemystic_cloud_client/cloud_providers/azure/__init__.py
--rw-r--r--   0        0        0    13856 2020-02-02 00:00:00.000000 threemystic_cloud_client-0.1.5/threemystic_cloud_client/cloud_providers/azure/base_class/base.py
--rw-r--r--   0        0        0      504 2020-02-02 00:00:00.000000 threemystic_cloud_client-0.1.5/threemystic_cloud_client/cloud_providers/azure/client/auto_client.py
--rw-r--r--   0        0        0     1478 2020-02-02 00:00:00.000000 threemystic_cloud_client-0.1.5/threemystic_cloud_client/cloud_providers/azure/client/cli.py
--rw-r--r--   0        0        0    13524 2020-02-02 00:00:00.000000 threemystic_cloud_client-0.1.5/threemystic_cloud_client/cloud_providers/azure/client/base_class/base.py
--rw-r--r--   0        0        0      569 2020-02-02 00:00:00.000000 threemystic_cloud_client-0.1.5/threemystic_cloud_client/cloud_providers/azure/config/step_1.py
--rw-r--r--   0        0        0     2788 2020-02-02 00:00:00.000000 threemystic_cloud_client-0.1.5/threemystic_cloud_client/cloud_providers/azure/config/base_class/base.py
--rw-r--r--   0        0        0     1054 2020-02-02 00:00:00.000000 threemystic_cloud_client-0.1.5/threemystic_cloud_client/cloud_providers/azure/test/step_1.py
--rw-r--r--   0        0        0      619 2020-02-02 00:00:00.000000 threemystic_cloud_client-0.1.5/threemystic_cloud_client/cloud_providers/azure/test/base_class/base.py
--rw-r--r--   0        0        0     4923 2020-02-02 00:00:00.000000 threemystic_cloud_client-0.1.5/threemystic_cloud_client/cloud_providers/base_class/base.py
--rw-r--r--   0        0        0      236 2020-02-02 00:00:00.000000 threemystic_cloud_client-0.1.5/threemystic_cloud_client/domain/aws/client_sso.py
--rw-r--r--   0        0        0      239 2020-02-02 00:00:00.000000 threemystic_cloud_client-0.1.5/threemystic_cloud_client/domain/aws/controller.py
--rw-r--r--   0        0        0      234 2020-02-02 00:00:00.000000 threemystic_cloud_client-0.1.5/threemystic_cloud_client/domain/azure/client.py
--rw-r--r--   0        0        0     1799 2020-02-02 00:00:00.000000 threemystic_cloud_client-0.1.5/.gitignore
--rw-r--r--   0        0        0     1068 2020-02-02 00:00:00.000000 threemystic_cloud_client-0.1.5/LICENSE
--rw-r--r--   0        0        0     1158 2020-02-02 00:00:00.000000 threemystic_cloud_client-0.1.5/README.md
--rw-r--r--   0        0        0      692 2020-02-02 00:00:00.000000 threemystic_cloud_client-0.1.5/hatch.toml
--rw-r--r--   0        0        0     3317 2020-02-02 00:00:00.000000 threemystic_cloud_client-0.1.5/pyproject.toml
--rw-r--r--   0        0        0     2595 2020-02-02 00:00:00.000000 threemystic_cloud_client-0.1.5/PKG-INFO
+-rw-r--r--   0        0        0      197 2020-02-02 00:00:00.000000 threemystic_cloud_client-0.1.6/threemystic_cloud_client/__main__.py
+-rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 threemystic_cloud_client-0.1.6/threemystic_cloud_client/__version__.py
+-rw-r--r--   0        0        0     3168 2020-02-02 00:00:00.000000 threemystic_cloud_client-0.1.6/threemystic_cloud_client/cloud_client.py
+-rw-r--r--   0        0        0     4101 2020-02-02 00:00:00.000000 threemystic_cloud_client-0.1.6/threemystic_cloud_client/cli/__init__.py
+-rw-r--r--   0        0        0     2519 2020-02-02 00:00:00.000000 threemystic_cloud_client-0.1.6/threemystic_cloud_client/cli/actions/base_class/base.py
+-rw-r--r--   0        0        0      631 2020-02-02 00:00:00.000000 threemystic_cloud_client-0.1.6/threemystic_cloud_client/cli/actions/config/__init__.py
+-rw-r--r--   0        0        0      649 2020-02-02 00:00:00.000000 threemystic_cloud_client-0.1.6/threemystic_cloud_client/cli/actions/test/__init__.py
+-rw-r--r--   0        0        0     4074 2020-02-02 00:00:00.000000 threemystic_cloud_client-0.1.6/threemystic_cloud_client/cli/actions/token/__init__.py
+-rw-r--r--   0        0        0     1200 2020-02-02 00:00:00.000000 threemystic_cloud_client-0.1.6/threemystic_cloud_client/cloud_providers/aws/__init__.py
+-rw-r--r--   0        0        0     3591 2020-02-02 00:00:00.000000 threemystic_cloud_client-0.1.6/threemystic_cloud_client/cloud_providers/aws/base_class/base.py
+-rw-r--r--   0        0        0     2045 2020-02-02 00:00:00.000000 threemystic_cloud_client-0.1.6/threemystic_cloud_client/cloud_providers/aws/client/auto_client.py
+-rw-r--r--   0        0        0    12051 2020-02-02 00:00:00.000000 threemystic_cloud_client-0.1.6/threemystic_cloud_client/cloud_providers/aws/client/sso.py
+-rw-r--r--   0        0        0    21260 2020-02-02 00:00:00.000000 threemystic_cloud_client-0.1.6/threemystic_cloud_client/cloud_providers/aws/client/base_class/base.py
+-rw-r--r--   0        0        0     1587 2020-02-02 00:00:00.000000 threemystic_cloud_client-0.1.6/threemystic_cloud_client/cloud_providers/aws/config/step_1.py
+-rw-r--r--   0        0        0    15986 2020-02-02 00:00:00.000000 threemystic_cloud_client-0.1.6/threemystic_cloud_client/cloud_providers/aws/config/step_2.py
+-rw-r--r--   0        0        0     3451 2020-02-02 00:00:00.000000 threemystic_cloud_client-0.1.6/threemystic_cloud_client/cloud_providers/aws/config/base_class/base.py
+-rw-r--r--   0        0        0     1671 2020-02-02 00:00:00.000000 threemystic_cloud_client-0.1.6/threemystic_cloud_client/cloud_providers/aws/test/step_1.py
+-rw-r--r--   0        0        0     1095 2020-02-02 00:00:00.000000 threemystic_cloud_client-0.1.6/threemystic_cloud_client/cloud_providers/aws/test/step_2.py
+-rw-r--r--   0        0        0      642 2020-02-02 00:00:00.000000 threemystic_cloud_client-0.1.6/threemystic_cloud_client/cloud_providers/aws/test/base_class/base.py
+-rw-r--r--   0        0        0     1177 2020-02-02 00:00:00.000000 threemystic_cloud_client-0.1.6/threemystic_cloud_client/cloud_providers/azure/__init__.py
+-rw-r--r--   0        0        0    13977 2020-02-02 00:00:00.000000 threemystic_cloud_client-0.1.6/threemystic_cloud_client/cloud_providers/azure/base_class/base.py
+-rw-r--r--   0        0        0      457 2020-02-02 00:00:00.000000 threemystic_cloud_client-0.1.6/threemystic_cloud_client/cloud_providers/azure/client/auto_client.py
+-rw-r--r--   0        0        0      806 2020-02-02 00:00:00.000000 threemystic_cloud_client-0.1.6/threemystic_cloud_client/cloud_providers/azure/client/cli.py
+-rw-r--r--   0        0        0    15316 2020-02-02 00:00:00.000000 threemystic_cloud_client-0.1.6/threemystic_cloud_client/cloud_providers/azure/client/base_class/base.py
+-rw-r--r--   0        0        0      816 2020-02-02 00:00:00.000000 threemystic_cloud_client-0.1.6/threemystic_cloud_client/cloud_providers/azure/config/step_1.py
+-rw-r--r--   0        0        0     2788 2020-02-02 00:00:00.000000 threemystic_cloud_client-0.1.6/threemystic_cloud_client/cloud_providers/azure/config/base_class/base.py
+-rw-r--r--   0        0        0     1054 2020-02-02 00:00:00.000000 threemystic_cloud_client-0.1.6/threemystic_cloud_client/cloud_providers/azure/test/step_1.py
+-rw-r--r--   0        0        0      619 2020-02-02 00:00:00.000000 threemystic_cloud_client-0.1.6/threemystic_cloud_client/cloud_providers/azure/test/base_class/base.py
+-rw-r--r--   0        0        0     6835 2020-02-02 00:00:00.000000 threemystic_cloud_client-0.1.6/threemystic_cloud_client/cloud_providers/base_class/base.py
+-rw-r--r--   0        0        0      236 2020-02-02 00:00:00.000000 threemystic_cloud_client-0.1.6/threemystic_cloud_client/domain/aws/client_sso.py
+-rw-r--r--   0        0        0      239 2020-02-02 00:00:00.000000 threemystic_cloud_client-0.1.6/threemystic_cloud_client/domain/aws/controller.py
+-rw-r--r--   0        0        0      234 2020-02-02 00:00:00.000000 threemystic_cloud_client-0.1.6/threemystic_cloud_client/domain/azure/client.py
+-rw-r--r--   0        0        0     1799 2020-02-02 00:00:00.000000 threemystic_cloud_client-0.1.6/.gitignore
+-rw-r--r--   0        0        0     1068 2020-02-02 00:00:00.000000 threemystic_cloud_client-0.1.6/LICENSE
+-rw-r--r--   0        0        0     1158 2020-02-02 00:00:00.000000 threemystic_cloud_client-0.1.6/README.md
+-rw-r--r--   0        0        0      692 2020-02-02 00:00:00.000000 threemystic_cloud_client-0.1.6/hatch.toml
+-rw-r--r--   0        0        0     3365 2020-02-02 00:00:00.000000 threemystic_cloud_client-0.1.6/pyproject.toml
+-rw-r--r--   0        0        0     2659 2020-02-02 00:00:00.000000 threemystic_cloud_client-0.1.6/PKG-INFO
```

### Comparing `threemystic_cloud_client-0.1.5/threemystic_cloud_client/cloud_client.py` & `threemystic_cloud_client-0.1.6/threemystic_cloud_client/cloud_client.py`

 * *Files identical despite different names*

### Comparing `threemystic_cloud_client-0.1.5/threemystic_cloud_client/cli/__init__.py` & `threemystic_cloud_client-0.1.6/threemystic_cloud_client/cli/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,14 @@
 import sys
 from threemystic_common.base_class.base_script_options import base_process_options
-
+from threemystic_cloud_client.cloud_client import cloud_client as threemystic_client
 
 class cloud_client_cli(base_process_options):
-  def __init__(self, *args, **kwargs):
-    from threemystic_cloud_client.cloud_client import cloud_client
-    self._cloud_client = cloud_client()
+  def __init__(self, cloud_client = None, *args, **kwargs):    
+    self._cloud_client = threemystic_client() if cloud_client is None else cloud_client
     
     super().__init__(common= self._cloud_client.get_common(), *args, **kwargs)
 
     self.parser = self.get_parser(
       parser_init_kwargs = {
         "description": "One Action is required"
       },
```

### Comparing `threemystic_cloud_client-0.1.5/threemystic_cloud_client/cli/actions/base_class/base.py` & `threemystic_cloud_client-0.1.6/threemystic_cloud_client/cli/actions/base_class/base.py`

 * *Files identical despite different names*

### Comparing `threemystic_cloud_client-0.1.5/threemystic_cloud_client/cli/actions/config/__init__.py` & `threemystic_cloud_client-0.1.6/threemystic_cloud_client/cli/actions/config/__init__.py`

 * *Files identical despite different names*

### Comparing `threemystic_cloud_client-0.1.5/threemystic_cloud_client/cli/actions/test/__init__.py` & `threemystic_cloud_client-0.1.6/threemystic_cloud_client/cli/actions/test/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,18 +3,18 @@
 
 class cloud_client_test(base):
   def __init__(self, *args, **kwargs):
     super().__init__(*args, **kwargs)
 
 
   def _process_provider_aws(self, *args, **kwargs):
-      from threemystic_cloud_client.cloud_providers.aws  import cloud_client_aws as client
-      client(common= self._cloud_client.get_common()).action_test()
+    from threemystic_cloud_client.cloud_providers.aws  import cloud_client_aws as client
+    client(common= self._cloud_client.get_common()).action_test()
 
 
   def _process_provider_azure(self, *args, **kwargs):
-      from threemystic_cloud_client.cloud_providers.azure import cloud_client_azure as client
-      client(common= self._cloud_client.get_common()).action_test()      
+    from threemystic_cloud_client.cloud_providers.azure import cloud_client_azure as client
+    client(common= self._cloud_client.get_common()).action_test()
```

### Comparing `threemystic_cloud_client-0.1.5/threemystic_cloud_client/cli/actions/token/__init__.py` & `threemystic_cloud_client-0.1.6/threemystic_cloud_client/cli/actions/token/__init__.py`

 * *Files identical despite different names*

### Comparing `threemystic_cloud_client-0.1.5/threemystic_cloud_client/cloud_providers/aws/__init__.py` & `threemystic_cloud_client-0.1.6/threemystic_cloud_client/cloud_providers/azure/__init__.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,29 +1,35 @@
-from threemystic_cloud_client.cloud_providers.aws.base_class.base import cloud_client_provider_aws_base as base
+from threemystic_cloud_client.cloud_providers.azure.base_class.base import cloud_client_provider_azure_base as base
 
-
-class cloud_client_aws(base):
+class cloud_client_azure(base):
   def __init__(self, *args, **kwargs):
-    super().__init__(logger_name= "cloud_client_aws", *args, **kwargs)
+    super().__init__(logger_name= "cloud_client_azure", *args, **kwargs)
   
-  # There is not post init when in Config Mode
-  def _post_init(self, *args, **kwargs):
+  def _login(self, *args, **kwargs):
     pass
   
-  def action_test(self, *args, **kwargs):
-    from threemystic_cloud_client.cloud_providers.aws.test.step_1 import cloud_client_aws_test_step_1 as test
+  def action_test(self, *args, **kwargs):    
+    if not self.is_provider_config_completed():
+      print("Provider must be configured first")
+      self._setup_another_config()
+      return
+    
+    from threemystic_cloud_client.cloud_providers.azure.test.step_1 import cloud_client_azure_test_step_1 as test
     next_step = test(common= self.get_common(), logger= self.get_logger(), *args, **kwargs)
     
     next_step.step()
-
-  def action_config(self, *args, **kwargs): 
+  
+  def action_config(self, *args, **kwargs):     
+    if not self.is_provider_config_completed():
+      print("Provider must be configured first")
+      self._setup_another_config()
+      return
     
-    from threemystic_cloud_client.cloud_providers.aws.config.step_1 import cloud_client_aws_config_step_1 as step
+    from threemystic_cloud_client.cloud_providers.azure.config.step_1 import cloud_client_azure_config_step_1 as step
     next_step = step(common= self.get_common(), logger= self.get_logger())
     
     next_step.step()
 
 
-
```

### Comparing `threemystic_cloud_client-0.1.5/threemystic_cloud_client/cloud_providers/aws/base_class/base.py` & `threemystic_cloud_client-0.1.6/threemystic_cloud_client/cloud_providers/aws/base_class/base.py`

 * *Files identical despite different names*

### Comparing `threemystic_cloud_client-0.1.5/threemystic_cloud_client/cloud_providers/aws/client/auto_client.py` & `threemystic_cloud_client-0.1.6/threemystic_cloud_client/cloud_providers/aws/client/auto_client.py`

 * *Files identical despite different names*

### Comparing `threemystic_cloud_client-0.1.5/threemystic_cloud_client/cloud_providers/aws/client/sso.py` & `threemystic_cloud_client-0.1.6/threemystic_cloud_client/cloud_providers/aws/client/sso.py`

 * *Files identical despite different names*

### Comparing `threemystic_cloud_client-0.1.5/threemystic_cloud_client/cloud_providers/aws/client/base_class/base.py` & `threemystic_cloud_client-0.1.6/threemystic_cloud_client/cloud_providers/aws/client/base_class/base.py`

 * *Files identical despite different names*

### Comparing `threemystic_cloud_client-0.1.5/threemystic_cloud_client/cloud_providers/aws/config/step_1.py` & `threemystic_cloud_client-0.1.6/threemystic_cloud_client/cloud_providers/aws/config/step_1.py`

 * *Files 7% similar despite different names*

```diff
@@ -28,10 +28,11 @@
         }
       }
     )
 
     if response is None:
       return
 
+    self.update_provider_config_completed(status= "step1")
     nextstep(init_object = self).step(is_new_config= response["type"].get("formated") == True)
```

### Comparing `threemystic_cloud_client-0.1.5/threemystic_cloud_client/cloud_providers/aws/config/step_2.py` & `threemystic_cloud_client-0.1.6/threemystic_cloud_client/cloud_providers/aws/config/step_2.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,14 +2,20 @@
 from threemystic_common.base_class.generate_data.generate_data_handlers import generate_data_handlers
 import configparser
 
 class cloud_client_aws_config_step_2(base):
   def __init__(self, *args, **kwargs):
     super().__init__(logger_name= "cloud_client_aws_config_step_2", *args, **kwargs)
 
+  def step_done(self, *args, **kwargs):
+    
+    self.update_provider_config_completed(status= True)
+    self._setup_another_config()
+
+
   def step(self, is_new_config, *args, **kwargs):
 
     if not super().step():
       return
 
     if is_new_config:
       self.__step_new()
@@ -200,38 +206,38 @@
           "desc": f"Use preconfigured aws cli sso profile (created with aws configure sso --profile <profile_name>)\nValid optiond for yes: {self.get_common().helper_type().bool().is_true_values()}{self.__get_existing_text(exiting_value= profile_data.get('use_cli_profile'))}",
           "handler": generate_data_handlers.get_handler(handler= "base"),
           "default": profile_data.get("use_cli_profile") == True,
           "optional": False
         },
         "sso_profile_name": {
           "validation": lambda item: self.__step_process_sso_valid_profile(profile_name= item, existing_profile= existing_sso_profile_name),
-          "allow_empty": True,
+          "allow_empty": False,
           "skip": lambda item: item.get("use_cli_profile").get("formatted") if item is not None and item.get("use_cli_profile") is not None else False,
           "messages":{
             "validation": f"Could not find profile.",
           },
           "conversion": lambda item: self.get_common().helper_type().string().trim(string_value= item),
           "desc": f"Enter the SSO Profile Name{self.__get_existing_text(exiting_value= existing_sso_profile_name)}",
           "handler": generate_data_handlers.get_handler(handler= "base"),
           "default": profile_data.get("sso_profile_name"),
-          "optional": False
+          "optional": not self.get_common().helper_type().string().is_null_or_whitespace(string_value= profile_data.get("sso_profile_name"))
         },
         "sso_start_url": {
           "validation": lambda item: item,
           "skip": lambda item: not item.get("use_cli_profile").get("formatted") if item is not None and item.get("use_cli_profile") is not None else True,
           "messages":{},
           "conversion": lambda item: self.get_common().helper_type().string().trim(item),
           "desc": f"Enter the SSO start url (ex: https://<aws_id>.awsapps.com/start",
           "handler": generate_data_handlers.get_handler(handler= "base"),
           "default": profile_data.get("sso_start_url"),
           "optional": not self.get_common().helper_type().string().is_null_or_whitespace(string_value= profile_data.get("sso_start_url"))
         },
         "sso_region": {
           "validation": lambda item: item,
-          "skip": lambda item: not item.get("use_cli_profile").get("formatted") if item is not None and item.get("use_cli_profile") is not None else True,
+          "skip": lambda item: not item.get("use_cli_profile").get("formatted") is not True if item is not None and item.get("use_cli_profile") is not None else True,
           "allow_empty": True,
           "messages":{},
           "conversion": lambda item: self.get_common().helper_type().string().trim(item),
           "desc": f"Enter the default region to use{self.__get_existing_text(exiting_value= profile_data.get('sso_region'))}",
           "handler": generate_data_handlers.get_handler(handler= "base"),
           "default": profile_data.get("sso_region") if not self.get_common().helper_type().string().is_null_or_whitespace(string_value= profile_data.get("sso_region")) else "us-east-1",
           "optional": False
@@ -293,10 +299,12 @@
       profile_data[key] = item.get("formated") if item is not None else ""
     
     if self.get_common().helper_type().string().is_null_or_whitespace(string_value=profile_data.get("sso_profile_name")):
       profile_data["sso_profile_name"] = existing_sso_profile_name
     
     self.update_config_profile(profile_name= profile_name, profile_data= profile_data)
     print(f"Profile ({profile_name} saved/updated)")
+    self.step_done()
+
```

### Comparing `threemystic_cloud_client-0.1.5/threemystic_cloud_client/cloud_providers/aws/config/base_class/base.py` & `threemystic_cloud_client-0.1.6/threemystic_cloud_client/cloud_providers/aws/config/base_class/base.py`

 * *Files identical despite different names*

### Comparing `threemystic_cloud_client-0.1.5/threemystic_cloud_client/cloud_providers/aws/test/step_1.py` & `threemystic_cloud_client-0.1.6/threemystic_cloud_client/cloud_providers/aws/test/step_1.py`

 * *Files identical despite different names*

### Comparing `threemystic_cloud_client-0.1.5/threemystic_cloud_client/cloud_providers/aws/test/step_2.py` & `threemystic_cloud_client-0.1.6/threemystic_cloud_client/cloud_providers/aws/test/step_2.py`

 * *Files identical despite different names*

### Comparing `threemystic_cloud_client-0.1.5/threemystic_cloud_client/cloud_providers/aws/test/base_class/base.py` & `threemystic_cloud_client-0.1.6/threemystic_cloud_client/cloud_providers/aws/test/base_class/base.py`

 * *Files identical despite different names*

### Comparing `threemystic_cloud_client-0.1.5/threemystic_cloud_client/cloud_providers/azure/__init__.py` & `threemystic_cloud_client-0.1.6/threemystic_cloud_client/cloud_providers/aws/__init__.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,26 +1,36 @@
-from threemystic_cloud_client.cloud_providers.azure.base_class.base import cloud_client_provider_azure_base as base
+from threemystic_cloud_client.cloud_providers.aws.base_class.base import cloud_client_provider_aws_base as base
 
-class cloud_client_azure(base):
+
+class cloud_client_aws(base):
   def __init__(self, *args, **kwargs):
-    super().__init__(logger_name= "cloud_client_azure", *args, **kwargs)
+    super().__init__(logger_name= "cloud_client_aws", *args, **kwargs)
   
-  def _login(self, *args, **kwargs):
+  # There is not post init when in Config Mode
+  def _post_init(self, *args, **kwargs):
     pass
   
   def action_test(self, *args, **kwargs):
-    from threemystic_cloud_client.cloud_providers.azure.test.step_1 import cloud_client_azure_test_step_1 as test
+    if not self.is_provider_config_completed():
+      print("Provider must be configured first")
+      self._setup_another_config()
+      return
+    from threemystic_cloud_client.cloud_providers.aws.test.step_1 import cloud_client_aws_test_step_1 as test
     next_step = test(common= self.get_common(), logger= self.get_logger(), *args, **kwargs)
     
     next_step.step()
-  
-  def action_config(self, *args, **kwargs): 
-    
-    from threemystic_cloud_client.cloud_providers.azure.config.step_1 import cloud_client_azure_config_step_1 as step
+
+  def action_config(self, *args, **kwargs):     
+    if not self.is_provider_config_completed():
+      print("Provider must be configured first")
+      self._setup_another_config()
+      return
+    from threemystic_cloud_client.cloud_providers.aws.config.step_1 import cloud_client_aws_config_step_1 as step
     next_step = step(common= self.get_common(), logger= self.get_logger())
     
     next_step.step()
 
 
+
```

### Comparing `threemystic_cloud_client-0.1.5/threemystic_cloud_client/cloud_providers/azure/base_class/base.py` & `threemystic_cloud_client-0.1.6/threemystic_cloud_client/cloud_providers/azure/base_class/base.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,63 +1,60 @@
 from threemystic_cloud_client.cloud_providers.base_class.base import cloud_client_provider_base as base
 from azure.mgmt.costmanagement.models import TimeframeType, OperatorType, QueryColumnType, QueryDefinition, QueryTimePeriod, QueryDataset, QueryAggregation, QueryGrouping, QueryFilter, QueryComparisonExpression
 from azure.core.exceptions import HttpResponseError, ClientAuthenticationError
 import time
 import math
 from abc import abstractmethod
-from polling2 import TimeoutException, poll as poll2
+import jwt
 
 
 class cloud_client_provider_azure_base(base):
   def __init__(self, *args, **kwargs):
     self._stop_process_login()
     super().__init__(provider= "azure", *args, **kwargs)
     
     self.links = {
       "cli_doc_link": "https://learn.microsoft.com/en-us/cli/azure/install-azure-cli"
     }
 
-  
-  @abstractmethod
-  def _login(self, *args, **kwargs):
-    pass
+
+  def decode_jwt_token(self, token, *args, **kwargs):
+    alg = jwt.get_unverified_header(jwt= token)
+    return jwt.decode(
+      jwt= token,
+      algorithms= [alg],
+      options= {"verify_signature": False}
+    )
 
   def is_login_processing(self, *args, **kwargs):
     return (self.__is_processing_login is True)
   
   def _start_process_login(self, *args, **kwargs):
     self.__is_processing_login = True
   
   def _stop_process_login(self, *args, **kwargs):
     self.__is_processing_login = False
 
   def _start_process_login(self, *args, **kwargs):
     self.__is_processing_login = True
-     
-  def login(self, *args, **kwargs):
-    if self.is_login_processing():
-      poll2(
-        lambda: self.is_login_processing(),
-        ignore_exceptions=(Exception,),
-        timeout=240,
-        step=0.1
-      )
-
-    self._start_process_login()
-    return_data = self._login(*args, **kwargs)
-    self._stop_process_login()
-
-    return return_data
 
-  def _get_credential(self, *args, **kwargs):
-    if hasattr(self, "_credentials"):
-      return self._credentials
+  
+  def _get_credential(self, account_id, unset = False, *args, **kwargs):
+    if unset is True:
+      if hasattr(self, f"_credentials_{account_id}"):
+        current_value = getattr(self, f"_credentials_{account_id}")
+        delattr(self, f"_credentials_{account_id}")
+        return current_value
+      return None
+      
+    if hasattr(self, f"_credentials_{account_id}"):
+      return getattr(self, f"_credentials_{account_id}")
     
-    self._credentials = {}
-    return self._get_credential()
+    setattr(self, f"_credentials_{account_id}", {})
+    return self._get_credential(account_id= account_id)
 
   def _clear_credential(self, *args, **kwargs):
     delattr(self, "_credentials")
   
   def check_request_too_many_requests(self, exception, *args, **kwargs):
     if not self.get_common().helper_type().general().is_type(obj= exception, type_check= HttpResponseError):
       return False
```

### Comparing `threemystic_cloud_client-0.1.5/threemystic_cloud_client/cloud_providers/azure/client/base_class/base.py` & `threemystic_cloud_client-0.1.6/threemystic_cloud_client/cloud_providers/azure/client/base_class/base.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,26 +1,71 @@
 from threemystic_cloud_client.cloud_providers.azure.base_class.base import cloud_client_provider_azure_base as base
 from abc import abstractmethod
 from io import StringIO
 from knack.log import CLI_LOGGER_NAME
 import logging
+from polling2 import TimeoutException, poll as poll2
 from azure.core.exceptions import HttpResponseError
 from azure.cli.core import get_default_cli
 from azure.mgmt.resource.subscriptions import SubscriptionClient as ResourceSubscriptionClient
 from azure.mgmt.resourcegraph import ResourceGraphClient
 from azure.mgmt.resourcegraph.models import QueryRequestOptions, QueryRequest
 
 class cloud_client_azure_client_base(base):
   def __init__(self, *args, **kwargs):
     super().__init__(*args, **kwargs)
 
   
   @abstractmethod
-  def get_tenant_credential(self, tenant = None, *args, **kwargs):
+  def _login(self, *args, **kwargs):
+    pass
+
+  @abstractmethod
+  def _get_tenant_credential(self, tenant = None, *args, **kwargs):
     pass
+
+  def login(self, *args, **kwargs):
+    if self.is_login_processing():
+      poll2(
+        lambda: self.is_login_processing(),
+        ignore_exceptions=(Exception,),
+        timeout=240,
+        step=0.1
+      )
+
+    self._start_process_login()
+    return_data = self._login(*args, **kwargs)
+    self._stop_process_login()
+
+    return return_data
+  
+  def get_tenant_credential_full(self, tenant = None, *args, **kwargs):
+    if self.get_common().helper_type().string().is_null_or_whitespace(string_value= self.get_tenant_id(tenant= tenant)):
+      raise self.get_common().exception().exception(
+        exception_type = "argument"
+      ).type_error(
+        logger = self.get_common().get_logger(),
+        name = "tenant_id",
+        message = f"tenant_id cannot be null or whitespace"
+      )
+    
+    if (self._get_credential(account_id= self.get_tenant_id(tenant= tenant)) is not None
+        and len(self._get_credential(account_id= self.get_tenant_id(tenant= tenant))) > 1):
+      return self._get_credential(account_id= self.get_tenant_id(tenant= tenant))
+    
+    credentials = self._get_tenant_credential(tenant= tenant)
+    self._get_credential(account_id= self.get_tenant_id(tenant= tenant) )["credentials"] = credentials
+    self._get_credential(account_id= self.get_tenant_id(tenant= tenant) )["jwt"] = self.decode_jwt_token(
+      token= credentials.get_token("https://graph.microsoft.com/.default").token
+    )
+
+    return self.get_tenant_credential_full(tenant= tenant, *args, **kwargs)
+  
+  def get_tenant_credential(self, tenant = None, *args, **kwargs):
+    return self.get_tenant_credential_full(tenant= tenant, *args, **kwargs).get("credentials")
          
   def get_tenants(self, refresh = False, tenant = None, *args, **kwargs):
     if tenant is None:
       return self.__get_tenants()
     
     if self.get_common().helper_type().general().is_type(obj= tenant, type_check= str) and not self.get_common().helper_type().string().is_null_or_whitespace(string_value= tenant):
       tenant = [ acct.strip() for acct in self.get_common().helper_type().string().split(string_value= tenant) if not self.get_common().helper_type().string().is_null_or_whitespace(string_value= acct) ]
```

### Comparing `threemystic_cloud_client-0.1.5/threemystic_cloud_client/cloud_providers/azure/config/base_class/base.py` & `threemystic_cloud_client-0.1.6/threemystic_cloud_client/cloud_providers/azure/config/base_class/base.py`

 * *Files identical despite different names*

### Comparing `threemystic_cloud_client-0.1.5/threemystic_cloud_client/cloud_providers/azure/test/step_1.py` & `threemystic_cloud_client-0.1.6/threemystic_cloud_client/cloud_providers/azure/test/step_1.py`

 * *Files identical despite different names*

### Comparing `threemystic_cloud_client-0.1.5/threemystic_cloud_client/cloud_providers/azure/test/base_class/base.py` & `threemystic_cloud_client-0.1.6/threemystic_cloud_client/cloud_providers/azure/test/base_class/base.py`

 * *Files identical despite different names*

### Comparing `threemystic_cloud_client-0.1.5/threemystic_cloud_client/cloud_providers/base_class/base.py` & `threemystic_cloud_client-0.1.6/threemystic_cloud_client/cloud_providers/base_class/base.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,19 +1,63 @@
 from threemystic_common.base_class.base_provider import base
 from abc import abstractmethod
+from threemystic_common.base_class.generate_data.generate_data_handlers import generate_data_handlers
+from threemystic_cloud_client.cli import cloud_client_cli
 
 class cloud_client_provider_base(base):
   def __init__(self, *args, **kwargs):
     super().__init__(*args, **kwargs)
     
     self._post_init(*args, **kwargs)
 
   
   def _post_init(self, *args, **kwargs):
     pass
+
+  def _setup_another_config(self, force_config = False, *args, **kwargs):
+    if not force_config:
+      response = self.get_common().generate_data().generate(
+        generate_data_config = {
+          "repeat_config": {
+              "validation": lambda item: self.get_common().helper_type().bool().is_bool(check_value= item),
+              "messages":{
+                "validation": f"Valid options for Yes are: {self.get_common().helper_type().bool().is_true_values()}",
+              },
+              "conversion": lambda item: self.get_common().helper_type().bool().is_true(check_value= item),
+              "desc": f"Do you want to setup another provider?: {self.get_common().helper_type().bool().is_true_values()}",
+              "default": None,
+              "handler": generate_data_handlers.get_handler(handler= "base"),
+              "optional": True
+          }
+        }
+      )
+
+      if response is None:
+        return
+      
+      if response.get("repeat_config") is None:
+        return
+      
+      if response.get("repeat_config").get("formated") is not True:
+        return
+    
+    print()
+    print()
+    print("-------------------------------------------------------------------------")
+    print()
+    print()
+
+    cloud_client_cli().process_client_action("config")
+  
+  def update_provider_config_completed(self, status, *args, **kwargs):
+    self.get_config()["_config_process"] = status
+    self._save_config()
+  
+  def is_provider_config_completed(self, *args, **kwargs):
+    return self.get_config().get("_config_process") is True and self.is_cli_installed()
   
   def get_main_directory_name(self, *args, **kwargs):
     return "client"
 
   @abstractmethod
   def get_account_name(self, account, *args, **kwargs):
     pass
@@ -86,14 +130,25 @@
     
     return None
 
   def config_profile_name_exists(self, *args, **kwargs):
     
     return self.get_config_profile_name(*args, **kwargs) != None
   
+  def _update_config(self,config_key, config_value, refresh= False,  *args, **kwargs):
+     self.get_config(refresh = True)[config_key] = config_value
+  
+  def _save_config(self, *args, **kwargs):
+     if not self.config_path().parent.exists():
+       self.config_path().parent.mkdir(parents= True)
+     self.config_path().write_text(
+      data= self.get_common().helper_yaml().dumps(data= self.get_config())
+     )
+     self.get_config(refresh = True)
+
   def get_config(self, refresh = False, *args, **kwargs):
     if hasattr(self, "_config_data") and not refresh:
       return self._config_data
     
     self._config_data = self.__load_config()    
     self._config_data["profiles"] = {self.get_common().helper_type().string().set_case(string_value= profile_name, case= "lower"):profile_data for profile_name,profile_data in self.get_config_profiles().items()}
 
@@ -101,22 +156,14 @@
   
   def get_config_value(self, config_key, default_if_none = None, refresh = False, *args, **kwargs):
     config_value = self.get_config(refresh= refresh).get(config_key)
     if config_value is not None:
       return config_value
     
     return default_if_none
-  
-  def _save_config(self, *args, **kwargs):
-     if not self.config_path().parent.exists():
-       self.config_path().mkdir(parents= True)
-     self.config_path().write_text(
-      data= self.get_common().helper_yaml().dumps(data= self.get_config())
-     )
-     self.get_config(refresh = True)
 
   def has_config_profiles(self, *args, **kwargs):
     
     if self.get_config().get("profiles") is None:
       return False
     
     return len(self.get_config().get("profiles")) > 0
```

### Comparing `threemystic_cloud_client-0.1.5/.gitignore` & `threemystic_cloud_client-0.1.6/.gitignore`

 * *Files identical despite different names*

### Comparing `threemystic_cloud_client-0.1.5/LICENSE` & `threemystic_cloud_client-0.1.6/LICENSE`

 * *Files identical despite different names*

### Comparing `threemystic_cloud_client-0.1.5/README.md` & `threemystic_cloud_client-0.1.6/README.md`

 * *Files identical despite different names*

### Comparing `threemystic_cloud_client-0.1.5/hatch.toml` & `threemystic_cloud_client-0.1.6/hatch.toml`

 * *Files identical despite different names*

### Comparing `threemystic_cloud_client-0.1.5/pyproject.toml` & `threemystic_cloud_client-0.1.6/pyproject.toml`

 * *Files 3% similar despite different names*

```diff
@@ -23,21 +23,23 @@
   "Programming Language :: Python :: 3.10",
   "Programming Language :: Python :: 3.11",
   "Programming Language :: Python :: Implementation :: CPython",
   "Programming Language :: Python :: Implementation :: PyPy",
 ]
 dependencies = [
   "colorama; platform_system == 'Windows'",
-  "threemystic-common >= 0.1.3",
+  "threemystic-common >= 0.1.4",
   "polling2 >= 0.5.0",
   "typing-extensions >= 4.4.0",
+  "PyJWT >= 2.7.0",
+  "cryptography >= 41.0.1",
   "boto3 >= 1.26.151",
   "botocore >= 1.29.151",
   "azure-common >= 1.1.28",
-  "azure-cli >= 2.49.0",
+  "azure-cli >= 2.50.0",
   "azure-identity >= 1.13.0",
   "azure-mgmt-subscription >= 3.1.1",
   "azure-mgmt-managementgroups >= 1.0.0",
   "azure-mgmt-resourcegraph >= 8.0.0",
   "azure-mgmt-sql >= 3.0.1",
 ]
 dynamic = ["version"]
```

### Comparing `threemystic_cloud_client-0.1.5/PKG-INFO` & `threemystic_cloud_client-0.1.6/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: threemystic-cloud-client
-Version: 0.1.5
+Version: 0.1.6
 Summary: A tool to help facilitate the communication with various cloud providers
 Project-URL: Homepage, https://github.com/3MysticApes/3mystic_cloud_client
 Project-URL: Bug Tracker, https://github.com/3MysticApes/3mystic_cloud_client/issues
 Author: Ron Truex
 License-Expression: MIT
 License-File: LICENSE
 Classifier: License :: OSI Approved :: MIT License
@@ -13,26 +13,28 @@
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Programming Language :: Python :: Implementation :: PyPy
 Requires-Python: >=3.8
-Requires-Dist: azure-cli>=2.49.0
+Requires-Dist: azure-cli>=2.50.0
 Requires-Dist: azure-common>=1.1.28
 Requires-Dist: azure-identity>=1.13.0
 Requires-Dist: azure-mgmt-managementgroups>=1.0.0
 Requires-Dist: azure-mgmt-resourcegraph>=8.0.0
 Requires-Dist: azure-mgmt-sql>=3.0.1
 Requires-Dist: azure-mgmt-subscription>=3.1.1
 Requires-Dist: boto3>=1.26.151
 Requires-Dist: botocore>=1.29.151
 Requires-Dist: colorama; platform_system == 'Windows'
+Requires-Dist: cryptography>=41.0.1
 Requires-Dist: polling2>=0.5.0
-Requires-Dist: threemystic-common>=0.1.3
+Requires-Dist: pyjwt>=2.7.0
+Requires-Dist: threemystic-common>=0.1.4
 Requires-Dist: typing-extensions>=4.4.0
 Description-Content-Type: text/markdown
 
 # 3mystic_cloud_client
 A tool to help uniform the connection to the cloud providers.
 Currently supports AWS/Azure
```

