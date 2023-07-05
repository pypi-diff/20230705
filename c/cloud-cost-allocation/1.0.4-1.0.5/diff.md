# Comparing `tmp/cloud-cost-allocation-1.0.4.tar.gz` & `tmp/cloud-cost-allocation-1.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cloud-cost-allocation-1.0.4.tar", last modified: Thu Jun  8 12:21:20 2023, max compression
+gzip compressed data, was "cloud-cost-allocation-1.0.5.tar", last modified: Wed Jul  5 06:46:11 2023, max compression
```

## Comparing `cloud-cost-allocation-1.0.4.tar` & `cloud-cost-allocation-1.0.5.tar`

### file list

```diff
@@ -1,41 +1,41 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 12:21:20.989045 cloud-cost-allocation-1.0.4/
--rw-r--r--   0 runner    (1001) docker     (123)     1078 2023-06-08 12:21:09.000000 cloud-cost-allocation-1.0.4/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       57 2023-06-08 12:21:09.000000 cloud-cost-allocation-1.0.4/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)    20967 2023-06-08 12:21:20.989045 cloud-cost-allocation-1.0.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    19754 2023-06-08 12:21:09.000000 cloud-cost-allocation-1.0.4/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 12:21:20.985045 cloud-cost-allocation-1.0.4/cloud_cost_allocation/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-08 12:21:09.000000 cloud-cost-allocation-1.0.4/cloud_cost_allocation/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    23784 2023-06-08 12:21:09.000000 cloud-cost-allocation-1.0.4/cloud_cost_allocation/cloud_cost_allocator.py
--rw-r--r--   0 runner    (1001) docker     (123)    10177 2023-06-08 12:21:09.000000 cloud-cost-allocation-1.0.4/cloud_cost_allocation/config.py
--rw-r--r--   0 runner    (1001) docker     (123)    41310 2023-06-08 12:21:09.000000 cloud-cost-allocation-1.0.4/cloud_cost_allocation/cost_items.py
--rw-r--r--   0 runner    (1001) docker     (123)      394 2023-06-08 12:21:09.000000 cloud-cost-allocation-1.0.4/cloud_cost_allocation/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)     3565 2023-06-08 12:21:09.000000 cloud-cost-allocation-1.0.4/cloud_cost_allocation/main.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 12:21:20.989045 cloud-cost-allocation-1.0.4/cloud_cost_allocation/reader/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-08 12:21:09.000000 cloud-cost-allocation-1.0.4/cloud_cost_allocation/reader/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4399 2023-06-08 12:21:09.000000 cloud-cost-allocation-1.0.4/cloud_cost_allocation/reader/azure_ea_amortized_cost_reader.py
--rw-r--r--   0 runner    (1001) docker     (123)     1659 2023-06-08 12:21:09.000000 cloud-cost-allocation-1.0.4/cloud_cost_allocation/reader/base_reader.py
--rw-r--r--   0 runner    (1001) docker     (123)     5564 2023-06-08 12:21:09.000000 cloud-cost-allocation-1.0.4/cloud_cost_allocation/reader/csv_allocated_cost_reader.py
--rw-r--r--   0 runner    (1001) docker     (123)    10325 2023-06-08 12:21:09.000000 cloud-cost-allocation-1.0.4/cloud_cost_allocation/reader/csv_cost_allocation_keys_reader.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 12:21:20.989045 cloud-cost-allocation-1.0.4/cloud_cost_allocation/utils/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-08 12:21:09.000000 cloud-cost-allocation-1.0.4/cloud_cost_allocation/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1191 2023-06-08 12:21:09.000000 cloud-cost-allocation-1.0.4/cloud_cost_allocation/utils/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 12:21:20.989045 cloud-cost-allocation-1.0.4/cloud_cost_allocation/writer/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-08 12:21:09.000000 cloud-cost-allocation-1.0.4/cloud_cost_allocation/writer/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2676 2023-06-08 12:21:09.000000 cloud-cost-allocation-1.0.4/cloud_cost_allocation/writer/base_writer.py
--rw-r--r--   0 runner    (1001) docker     (123)     6632 2023-06-08 12:21:09.000000 cloud-cost-allocation-1.0.4/cloud_cost_allocation/writer/csv_allocated_cost_writer.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 12:21:20.989045 cloud-cost-allocation-1.0.4/cloud_cost_allocation.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    20967 2023-06-08 12:21:20.000000 cloud-cost-allocation-1.0.4/cloud_cost_allocation.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1219 2023-06-08 12:21:20.000000 cloud-cost-allocation-1.0.4/cloud_cost_allocation.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-08 12:21:20.000000 cloud-cost-allocation-1.0.4/cloud_cost_allocation.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-06-08 12:21:20.000000 cloud-cost-allocation-1.0.4/cloud_cost_allocation.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 12:21:20.989045 cloud-cost-allocation-1.0.4/puml/
--rw-r--r--   0 runner    (1001) docker     (123)      968 2023-06-08 12:21:09.000000 cloud-cost-allocation-1.0.4/puml/cost-allocation-model.puml
--rw-r--r--   0 runner    (1001) docker     (123)    23813 2023-06-08 12:21:09.000000 cloud-cost-allocation-1.0.4/puml/cost-allocation-model.svg
--rw-r--r--   0 runner    (1001) docker     (123)     1073 2023-06-08 12:21:09.000000 cloud-cost-allocation-1.0.4/puml/hierarchical-service-consumption-example.puml
--rw-r--r--   0 runner    (1001) docker     (123)    16917 2023-06-08 12:21:09.000000 cloud-cost-allocation-1.0.4/puml/hierarchical-service-consumption-example.svg
--rw-r--r--   0 runner    (1001) docker     (123)     1160 2023-06-08 12:21:09.000000 cloud-cost-allocation-1.0.4/puml/hierarchical-service-cost-allocation-example.puml
--rw-r--r--   0 runner    (1001) docker     (123)    15996 2023-06-08 12:21:09.000000 cloud-cost-allocation-1.0.4/puml/hierarchical-service-cost-allocation-example.svg
--rw-r--r--   0 runner    (1001) docker     (123)     1140 2023-06-08 12:21:20.989045 cloud-cost-allocation-1.0.4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1446 2023-06-08 12:21:09.000000 cloud-cost-allocation-1.0.4/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 12:21:20.989045 cloud-cost-allocation-1.0.4/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     5812 2023-06-08 12:21:09.000000 cloud-cost-allocation-1.0.4/tests/test.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 06:46:11.897341 cloud-cost-allocation-1.0.5/
+-rw-r--r--   0 runner    (1001) docker     (123)     1078 2023-07-05 06:45:59.000000 cloud-cost-allocation-1.0.5/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       57 2023-07-05 06:45:59.000000 cloud-cost-allocation-1.0.5/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)    20967 2023-07-05 06:46:11.897341 cloud-cost-allocation-1.0.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    19754 2023-07-05 06:45:59.000000 cloud-cost-allocation-1.0.5/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 06:46:11.889341 cloud-cost-allocation-1.0.5/cloud_cost_allocation/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-05 06:45:59.000000 cloud-cost-allocation-1.0.5/cloud_cost_allocation/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23784 2023-07-05 06:45:59.000000 cloud-cost-allocation-1.0.5/cloud_cost_allocation/cloud_cost_allocator.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10177 2023-07-05 06:45:59.000000 cloud-cost-allocation-1.0.5/cloud_cost_allocation/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)    43878 2023-07-05 06:45:59.000000 cloud-cost-allocation-1.0.5/cloud_cost_allocation/cost_items.py
+-rw-r--r--   0 runner    (1001) docker     (123)      394 2023-07-05 06:45:59.000000 cloud-cost-allocation-1.0.5/cloud_cost_allocation/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3565 2023-07-05 06:45:59.000000 cloud-cost-allocation-1.0.5/cloud_cost_allocation/main.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 06:46:11.893341 cloud-cost-allocation-1.0.5/cloud_cost_allocation/reader/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-05 06:45:59.000000 cloud-cost-allocation-1.0.5/cloud_cost_allocation/reader/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4399 2023-07-05 06:45:59.000000 cloud-cost-allocation-1.0.5/cloud_cost_allocation/reader/azure_ea_amortized_cost_reader.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1659 2023-07-05 06:45:59.000000 cloud-cost-allocation-1.0.5/cloud_cost_allocation/reader/base_reader.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5564 2023-07-05 06:45:59.000000 cloud-cost-allocation-1.0.5/cloud_cost_allocation/reader/csv_allocated_cost_reader.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10325 2023-07-05 06:45:59.000000 cloud-cost-allocation-1.0.5/cloud_cost_allocation/reader/csv_cost_allocation_keys_reader.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 06:46:11.893341 cloud-cost-allocation-1.0.5/cloud_cost_allocation/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-05 06:45:59.000000 cloud-cost-allocation-1.0.5/cloud_cost_allocation/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1191 2023-07-05 06:45:59.000000 cloud-cost-allocation-1.0.5/cloud_cost_allocation/utils/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 06:46:11.893341 cloud-cost-allocation-1.0.5/cloud_cost_allocation/writer/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-05 06:45:59.000000 cloud-cost-allocation-1.0.5/cloud_cost_allocation/writer/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2676 2023-07-05 06:45:59.000000 cloud-cost-allocation-1.0.5/cloud_cost_allocation/writer/base_writer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6632 2023-07-05 06:45:59.000000 cloud-cost-allocation-1.0.5/cloud_cost_allocation/writer/csv_allocated_cost_writer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 06:46:11.893341 cloud-cost-allocation-1.0.5/cloud_cost_allocation.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    20967 2023-07-05 06:46:11.000000 cloud-cost-allocation-1.0.5/cloud_cost_allocation.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1219 2023-07-05 06:46:11.000000 cloud-cost-allocation-1.0.5/cloud_cost_allocation.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-05 06:46:11.000000 cloud-cost-allocation-1.0.5/cloud_cost_allocation.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-07-05 06:46:11.000000 cloud-cost-allocation-1.0.5/cloud_cost_allocation.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 06:46:11.893341 cloud-cost-allocation-1.0.5/puml/
+-rw-r--r--   0 runner    (1001) docker     (123)      968 2023-07-05 06:45:59.000000 cloud-cost-allocation-1.0.5/puml/cost-allocation-model.puml
+-rw-r--r--   0 runner    (1001) docker     (123)    23813 2023-07-05 06:45:59.000000 cloud-cost-allocation-1.0.5/puml/cost-allocation-model.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     1073 2023-07-05 06:45:59.000000 cloud-cost-allocation-1.0.5/puml/hierarchical-service-consumption-example.puml
+-rw-r--r--   0 runner    (1001) docker     (123)    16917 2023-07-05 06:45:59.000000 cloud-cost-allocation-1.0.5/puml/hierarchical-service-consumption-example.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     1160 2023-07-05 06:45:59.000000 cloud-cost-allocation-1.0.5/puml/hierarchical-service-cost-allocation-example.puml
+-rw-r--r--   0 runner    (1001) docker     (123)    15996 2023-07-05 06:45:59.000000 cloud-cost-allocation-1.0.5/puml/hierarchical-service-cost-allocation-example.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     1140 2023-07-05 06:46:11.897341 cloud-cost-allocation-1.0.5/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1446 2023-07-05 06:45:59.000000 cloud-cost-allocation-1.0.5/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 06:46:11.893341 cloud-cost-allocation-1.0.5/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     5812 2023-07-05 06:45:59.000000 cloud-cost-allocation-1.0.5/tests/test.py
```

### Comparing `cloud-cost-allocation-1.0.4/LICENSE` & `cloud-cost-allocation-1.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `cloud-cost-allocation-1.0.4/PKG-INFO` & `cloud-cost-allocation-1.0.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cloud-cost-allocation
-Version: 1.0.4
+Version: 1.0.5
 Summary: Python library for shared, hierarchical cost allocation based on user-defined usage metrics.
 Home-page: https://github.com/AmadeusITGroup/cloud-cost-allocation
 Author: Marc Perreaut
 Author-email: marc.perreaut@amadeus.com
 Maintainer: Amadeus IT Group
 Maintainer-email: opensource@amadeus.com
 License: MIT license
```

### Comparing `cloud-cost-allocation-1.0.4/README.md` & `cloud-cost-allocation-1.0.5/README.md`

 * *Files identical despite different names*

### Comparing `cloud-cost-allocation-1.0.4/cloud_cost_allocation/cloud_cost_allocator.py` & `cloud-cost-allocation-1.0.5/cloud_cost_allocation/cloud_cost_allocator.py`

 * *Files identical despite different names*

### Comparing `cloud-cost-allocation-1.0.4/cloud_cost_allocation/config.py` & `cloud-cost-allocation-1.0.5/cloud_cost_allocation/config.py`

 * *Files identical despite different names*

### Comparing `cloud-cost-allocation-1.0.4/cloud_cost_allocation/cost_items.py` & `cloud-cost-allocation-1.0.5/cloud_cost_allocation/cost_items.py`

 * *Files 2% similar despite different names*

```diff
@@ -556,92 +556,131 @@
             index = 0
             for amount_index in sorted(amount_to_allocation_key_indexes.keys()):
                 allocation_key_index = amount_to_allocation_key_indexes[amount_index]
                 amounts_by_product_info.total_keys[index] += consumer_item.allocation_keys[allocation_key_index]
                 amounts_by_product_info.nb_keys[index] += 1
                 index += 1
 
-        # Reset the number of matching provider tag selectors of every item
-        for item in self.cost_items:
-            item.nb_matching_provider_tag_selectors = 0
-
-        # Build evaluation error dict, used to avoid error streaming in case of incorrect provider tag
-        # selector expression
-        # Key = date, provider service, provider instance, provider tag selector, expression
-        # Value = count of errors
-        evaluation_error_dict = {}
+        # We will check whether provider tag selectors form a mathematical partition of the provider
+        # cost items, i.e. if every provider cost item is matched by a single provider tag selector
+        # We will also compute for every provider tag selector the (raw) amounts of the provider cost items
+        # that are matched by the provider tag selector
+        # If the provider tag selectors do not form a partition, the selected (raw) amounts of provider tag
+        # selectors will be adjusted proportionally so that the sum equals the sum of provider cost items
 
-        # Compute raw costs of non-default provider tag selectors, by checking matching items
+        # Process the simple common case of a single provider tag selector
+        is_partition = True
         total_provider_tag_selector_raw_amounts = [0.0] * nb_amounts
         total_provider_tag_selector_raw_product_amounts = [0.0] * nb_amounts
-        for provider_tag_selector_amount in self.provider_tag_selector_amounts.values():
+        if len(self.provider_tag_selector_amounts) == 1:
+
+            # For debug
+            provider_tag_selector_amount = list(self.provider_tag_selector_amounts.values())[0]
             if not provider_tag_selector_amount.is_default():
-                for cost_item in self.cost_items:
-                    if not cost_item.is_self_consumption():
+                debug("Provider service instance " + self.service + "." + self.instance +
+                      " has a single provider tag selector, which is not empty")
+
+            # Update raw amounts
+            for cost_item in self.cost_items:
+                if not cost_item.is_self_consumption():
+                    provider_tag_selector_amount\
+                        .update_raw_amounts(cost_item,
+                                            total_provider_tag_selector_raw_amounts,
+                                            total_provider_tag_selector_raw_product_amounts,
+                                            amount_to_allocation_key_indexes)
+
+        else:  # Case of multiple provider tag selectors
+
+            # Reset the number of matching provider tag selectors of every cost item, and build tag dict:
+            # - Key is cost item is tag string
+            # - Value is list of cost items
+            # Since multiple cost items may have the same tags, the goal is to minimize the number of tag evaluations
+            cost_item_tag_dict = {}
+            for cost_item in self.cost_items:
+                if not cost_item.is_self_consumption():
+                    cost_item.nb_matching_provider_tag_selectors = 0
+                    tag_string = str(cost_item.tags)
+                    if tag_string in cost_item_tag_dict:
+                        cost_item_list = cost_item_tag_dict[tag_string]
+                    else:
+                        cost_item_list = []
+                        cost_item_tag_dict[tag_string] = cost_item_list
+                    cost_item_list.append(cost_item)
+
+            # Build evaluation error dict, used to avoid error streaming in case of incorrect provider tag
+            # selector expression
+            # Key = date, provider service, provider instance, provider tag selector, expression
+            # Value = count of errors
+            evaluation_error_dict = {}
+
+            # Compute raw costs of non-default provider tag selectors, by checking matching items
+            for cost_item_tag, cost_item_list in cost_item_tag_dict.items():
+                for provider_tag_selector_amount in self.provider_tag_selector_amounts.values():
+                    if not provider_tag_selector_amount.is_default():
 
                         # Check if item matches provider tag selector
                         eval_globals_dict = {}
-                        for key, value in cost_item.tags.items():
+                        for key, value in cost_item_list[0].tags.items():
                             eval_globals_dict[re.sub(r'[^a-z0-9_]', '_', key)] = value
                         eval_true = False
                         try:
                             # Eval is dangerous. Considerations:
                             # - Audit cost allocation keys, which are provided by DevOps
                             # - Possibly forbid provider tag selectors
                             eval_true = eval(provider_tag_selector_amount.selector, eval_globals_dict, {})
                         except:
                             exception = sys.exc_info()[0]
                             error_key =\
-                                cost_item.date_str + chr(10) + self.service + chr(10) + self.instance + chr(10) +\
+                                cost_item_list[0].date_str + chr(10) + self.service + chr(10) + self.instance + chr(10) +\
                                 provider_tag_selector_amount.selector + chr(10) + str(exception)
                             if error_key in evaluation_error_dict:
                                 error_count = evaluation_error_dict[error_key]
                             else:
                                 error_count = 0
                             evaluation_error_dict[error_key] = error_count + 1
 
                         # If item matches provider tag selector, update raw amounts of the provider tag selector
                         if eval_true:
-                            cost_item.nb_matching_provider_tag_selectors += 1
-                            provider_tag_selector_amount\
-                                .update_raw_amounts(cost_item,
-                                                    total_provider_tag_selector_raw_amounts,
-                                                    total_provider_tag_selector_raw_product_amounts,
-                                                    amount_to_allocation_key_indexes)
-
-        # Log evaluation errors
-        for error_key, error_count in evaluation_error_dict.items():
-            error_fields = error_key.split(chr(10))
-            date_str = error_fields[0]
-            provider_service = error_fields[1]
-            provider_instance = error_fields[2]
-            provider_tag_selector = error_fields[3]
-            exception = error_fields[4]
-            error("Caught exception '" + exception + "' " + str(error_count) + " times " +
-                  "when evaluating ProviderTagSelector '" + provider_tag_selector +
-                  "' of ProviderService '" + provider_service +
-                  "' and of ProviderInstance '" + provider_instance + "'" +
-                  ", for date " + date_str)
-
-        # Compute the raw amounts of the default provider tag selector
-        if '' in self.provider_tag_selector_amounts:
-            default_provider_tag_selector = self.provider_tag_selector_amounts['']
-            for cost_item in self.cost_items:
-                if cost_item.nb_matching_provider_tag_selectors == 0 and not cost_item.is_self_consumption():
-                    cost_item.nb_matching_provider_tag_selectors = 1
-                    default_provider_tag_selector.update_raw_amounts(cost_item,
-                                                                     total_provider_tag_selector_raw_amounts,
-                                                                     total_provider_tag_selector_raw_product_amounts,
-                                                                     amount_to_allocation_key_indexes)
-
-        # Check if provider tag selectors form a partition
-        is_partition = True
-        for item in self.cost_items:
-            if not item.is_self_consumption() and item.nb_matching_provider_tag_selectors != 1:
-                is_partition = False
+                            for cost_item in cost_item_list:
+                                cost_item.nb_matching_provider_tag_selectors += 1
+                                provider_tag_selector_amount\
+                                    .update_raw_amounts(cost_item,
+                                                        total_provider_tag_selector_raw_amounts,
+                                                        total_provider_tag_selector_raw_product_amounts,
+                                                        amount_to_allocation_key_indexes)
+
+            # Log evaluation errors
+            for error_key, error_count in evaluation_error_dict.items():
+                error_fields = error_key.split(chr(10))
+                date_str = error_fields[0]
+                provider_service = error_fields[1]
+                provider_instance = error_fields[2]
+                provider_tag_selector = error_fields[3]
+                exception = error_fields[4]
+                error("Caught exception '" + exception + "' " + str(error_count) + " times " +
+                      "when evaluating ProviderTagSelector '" + provider_tag_selector +
+                      "' of ProviderService '" + provider_service +
+                      "' and of ProviderInstance '" + provider_instance + "'" +
+                      ", for date " + date_str)
+
+            # Compute the raw amounts of the default provider tag selector
+            if '' in self.provider_tag_selector_amounts:
+                default_provider_tag_selector = self.provider_tag_selector_amounts['']
+                for cost_item in self.cost_items:
+                    if cost_item.nb_matching_provider_tag_selectors == 0 and not cost_item.is_self_consumption():
+                        cost_item.nb_matching_provider_tag_selectors = 1
+                        default_provider_tag_selector.update_raw_amounts(cost_item,
+                                                                         total_provider_tag_selector_raw_amounts,
+                                                                         total_provider_tag_selector_raw_product_amounts,
+                                                                         amount_to_allocation_key_indexes)
+
+            # Check if provider tag selectors form a partition
+            for item in self.cost_items:
+                if not item.is_self_consumption() and item.nb_matching_provider_tag_selectors != 1:
+                    is_partition = False
 
         # For debug
         if not is_partition:
             debug("Provider tag selectors of provider service instance " + self.service + "." + self.instance +
                   " do not form a partition")
 
         # Adjust amounts
```

### Comparing `cloud-cost-allocation-1.0.4/cloud_cost_allocation/main.py` & `cloud-cost-allocation-1.0.5/cloud_cost_allocation/main.py`

 * *Files identical despite different names*

### Comparing `cloud-cost-allocation-1.0.4/cloud_cost_allocation/reader/azure_ea_amortized_cost_reader.py` & `cloud-cost-allocation-1.0.5/cloud_cost_allocation/reader/azure_ea_amortized_cost_reader.py`

 * *Files identical despite different names*

### Comparing `cloud-cost-allocation-1.0.4/cloud_cost_allocation/reader/base_reader.py` & `cloud-cost-allocation-1.0.5/cloud_cost_allocation/reader/base_reader.py`

 * *Files identical despite different names*

### Comparing `cloud-cost-allocation-1.0.4/cloud_cost_allocation/reader/csv_allocated_cost_reader.py` & `cloud-cost-allocation-1.0.5/cloud_cost_allocation/reader/csv_allocated_cost_reader.py`

 * *Files identical despite different names*

### Comparing `cloud-cost-allocation-1.0.4/cloud_cost_allocation/reader/csv_cost_allocation_keys_reader.py` & `cloud-cost-allocation-1.0.5/cloud_cost_allocation/reader/csv_cost_allocation_keys_reader.py`

 * *Files identical despite different names*

### Comparing `cloud-cost-allocation-1.0.4/cloud_cost_allocation/utils/utils.py` & `cloud-cost-allocation-1.0.5/cloud_cost_allocation/utils/utils.py`

 * *Files identical despite different names*

### Comparing `cloud-cost-allocation-1.0.4/cloud_cost_allocation/writer/base_writer.py` & `cloud-cost-allocation-1.0.5/cloud_cost_allocation/writer/base_writer.py`

 * *Files identical despite different names*

### Comparing `cloud-cost-allocation-1.0.4/cloud_cost_allocation/writer/csv_allocated_cost_writer.py` & `cloud-cost-allocation-1.0.5/cloud_cost_allocation/writer/csv_allocated_cost_writer.py`

 * *Files identical despite different names*

### Comparing `cloud-cost-allocation-1.0.4/cloud_cost_allocation.egg-info/PKG-INFO` & `cloud-cost-allocation-1.0.5/cloud_cost_allocation.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cloud-cost-allocation
-Version: 1.0.4
+Version: 1.0.5
 Summary: Python library for shared, hierarchical cost allocation based on user-defined usage metrics.
 Home-page: https://github.com/AmadeusITGroup/cloud-cost-allocation
 Author: Marc Perreaut
 Author-email: marc.perreaut@amadeus.com
 Maintainer: Amadeus IT Group
 Maintainer-email: opensource@amadeus.com
 License: MIT license
```

### Comparing `cloud-cost-allocation-1.0.4/cloud_cost_allocation.egg-info/SOURCES.txt` & `cloud-cost-allocation-1.0.5/cloud_cost_allocation.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `cloud-cost-allocation-1.0.4/puml/cost-allocation-model.puml` & `cloud-cost-allocation-1.0.5/puml/cost-allocation-model.puml`

 * *Files identical despite different names*

### Comparing `cloud-cost-allocation-1.0.4/puml/cost-allocation-model.svg` & `cloud-cost-allocation-1.0.5/puml/cost-allocation-model.svg`

 * *Files identical despite different names*

### Comparing `cloud-cost-allocation-1.0.4/puml/hierarchical-service-consumption-example.puml` & `cloud-cost-allocation-1.0.5/puml/hierarchical-service-consumption-example.puml`

 * *Files identical despite different names*

### Comparing `cloud-cost-allocation-1.0.4/puml/hierarchical-service-consumption-example.svg` & `cloud-cost-allocation-1.0.5/puml/hierarchical-service-consumption-example.svg`

 * *Files identical despite different names*

### Comparing `cloud-cost-allocation-1.0.4/puml/hierarchical-service-cost-allocation-example.puml` & `cloud-cost-allocation-1.0.5/puml/hierarchical-service-cost-allocation-example.puml`

 * *Files identical despite different names*

### Comparing `cloud-cost-allocation-1.0.4/puml/hierarchical-service-cost-allocation-example.svg` & `cloud-cost-allocation-1.0.5/puml/hierarchical-service-cost-allocation-example.svg`

 * *Files identical despite different names*

### Comparing `cloud-cost-allocation-1.0.4/setup.cfg` & `cloud-cost-allocation-1.0.5/setup.cfg`

 * *Files identical despite different names*

### Comparing `cloud-cost-allocation-1.0.4/setup.py` & `cloud-cost-allocation-1.0.5/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 # Import readme
 with open(os.path.join(os.path.dirname(__file__), 'README.md')) as readme_file:
     readme = readme_file.read()
 
 # Setup
 setup(
     name='cloud-cost-allocation',
-    version='1.0.4',
+    version='1.0.5',
     description='Python library for shared, hierarchical cost allocation based on user-defined usage metrics.',
     long_description=readme,
     long_description_content_type='text/markdown',
     packages=['cloud_cost_allocation',
               'cloud_cost_allocation.reader',
               'cloud_cost_allocation.utils',
               'cloud_cost_allocation.writer'],
```

### Comparing `cloud-cost-allocation-1.0.4/tests/test.py` & `cloud-cost-allocation-1.0.5/tests/test.py`

 * *Files identical despite different names*

