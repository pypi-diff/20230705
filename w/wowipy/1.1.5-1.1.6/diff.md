# Comparing `tmp/wowipy-1.1.5.tar.gz` & `tmp/wowipy-1.1.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "wowipy-1.1.5.tar", last modified: Wed Jul  5 08:07:24 2023, max compression
+gzip compressed data, was "wowipy-1.1.6.tar", last modified: Wed Jul  5 08:29:36 2023, max compression
```

## Comparing `wowipy-1.1.5.tar` & `wowipy-1.1.6.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxrwxrwx   0        0        0        0 2023-07-05 08:07:24.483780 wowipy-1.1.5/
--rw-rw-rw-   0        0        0    35817 2023-06-05 13:12:07.000000 wowipy-1.1.5/COPYING
--rw-rw-rw-   0        0        0    35817 2023-06-09 09:15:36.000000 wowipy-1.1.5/LICENSE
--rw-rw-rw-   0        0        0     1120 2023-07-05 08:07:24.482816 wowipy-1.1.5/PKG-INFO
--rw-rw-rw-   0        0        0       42 2023-07-05 08:07:24.483780 wowipy-1.1.5/setup.cfg
--rw-rw-rw-   0        0        0     1317 2023-07-05 08:07:22.000000 wowipy-1.1.5/setup.py
-drwxrwxrwx   0        0        0        0 2023-07-05 08:07:24.465828 wowipy-1.1.5/wowipy/
--rw-rw-rw-   0        0        0      153 2023-06-09 09:33:03.000000 wowipy-1.1.5/wowipy/__init__.py
--rw-rw-rw-   0        0        0       45 2023-06-05 13:24:50.000000 wowipy-1.1.5/wowipy/exceptions.py
--rw-rw-rw-   0        0        0    49213 2023-06-30 09:34:21.000000 wowipy-1.1.5/wowipy/models.py
--rw-rw-rw-   0        0        0     4550 2023-06-27 13:11:28.000000 wowipy-1.1.5/wowipy/rest_adapter.py
--rw-rw-rw-   0        0        0    43536 2023-07-05 08:07:06.000000 wowipy-1.1.5/wowipy/wowipy.py
-drwxrwxrwx   0        0        0        0 2023-07-05 08:07:24.481785 wowipy-1.1.5/wowipy.egg-info/
--rw-rw-rw-   0        0        0     1120 2023-07-05 08:07:24.000000 wowipy-1.1.5/wowipy.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      270 2023-07-05 08:07:24.000000 wowipy-1.1.5/wowipy.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-05 08:07:24.000000 wowipy-1.1.5/wowipy.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       42 2023-07-05 08:07:24.000000 wowipy-1.1.5/wowipy.egg-info/requires.txt
--rw-rw-rw-   0        0        0        7 2023-07-05 08:07:24.000000 wowipy-1.1.5/wowipy.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-07-05 08:29:36.580701 wowipy-1.1.6/
+-rw-rw-rw-   0        0        0    35817 2023-06-05 13:12:07.000000 wowipy-1.1.6/COPYING
+-rw-rw-rw-   0        0        0    35817 2023-06-09 09:15:36.000000 wowipy-1.1.6/LICENSE
+-rw-rw-rw-   0        0        0     1120 2023-07-05 08:29:36.579707 wowipy-1.1.6/PKG-INFO
+-rw-rw-rw-   0        0        0       42 2023-07-05 08:29:36.580701 wowipy-1.1.6/setup.cfg
+-rw-rw-rw-   0        0        0     1317 2023-07-05 08:29:34.000000 wowipy-1.1.6/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-05 08:29:36.563746 wowipy-1.1.6/wowipy/
+-rw-rw-rw-   0        0        0      153 2023-06-09 09:33:03.000000 wowipy-1.1.6/wowipy/__init__.py
+-rw-rw-rw-   0        0        0       45 2023-06-05 13:24:50.000000 wowipy-1.1.6/wowipy/exceptions.py
+-rw-rw-rw-   0        0        0    50382 2023-07-05 08:28:56.000000 wowipy-1.1.6/wowipy/models.py
+-rw-rw-rw-   0        0        0     4550 2023-06-27 13:11:28.000000 wowipy-1.1.6/wowipy/rest_adapter.py
+-rw-rw-rw-   0        0        0    43536 2023-07-05 08:07:06.000000 wowipy-1.1.6/wowipy/wowipy.py
+drwxrwxrwx   0        0        0        0 2023-07-05 08:29:36.578709 wowipy-1.1.6/wowipy.egg-info/
+-rw-rw-rw-   0        0        0     1120 2023-07-05 08:29:36.000000 wowipy-1.1.6/wowipy.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      270 2023-07-05 08:29:36.000000 wowipy-1.1.6/wowipy.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-05 08:29:36.000000 wowipy-1.1.6/wowipy.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       42 2023-07-05 08:29:36.000000 wowipy-1.1.6/wowipy.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        7 2023-07-05 08:29:36.000000 wowipy-1.1.6/wowipy.egg-info/top_level.txt
```

### Comparing `wowipy-1.1.5/COPYING` & `wowipy-1.1.6/COPYING`

 * *Files identical despite different names*

### Comparing `wowipy-1.1.5/LICENSE` & `wowipy-1.1.6/LICENSE`

 * *Files identical despite different names*

### Comparing `wowipy-1.1.5/PKG-INFO` & `wowipy-1.1.6/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: wowipy
-Version: 1.1.5
+Version: 1.1.6
 Summary: OPENWOWI Wowiport API wrapper for python
 Home-page: https://github.com/seb-bau/WowiPy
 Author: Sebastian Bauhaus
 Author-email: sebastian@bytewish.de
 License: GPL-3.0
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
```

### Comparing `wowipy-1.1.5/setup.py` & `wowipy-1.1.6/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup
 
 setup(
     name='wowipy',
-    version='1.1.5',
+    version='1.1.6',
     description='OPENWOWI Wowiport API wrapper for python',
     url='https://github.com/seb-bau/WowiPy',
     author='Sebastian Bauhaus',
     author_email='sebastian@bytewish.de',
     license='GPL-3.0',
     packages=['wowipy'],
     install_requires=['requests>=2.0',
```

### Comparing `wowipy-1.1.5/wowipy/models.py` & `wowipy-1.1.6/wowipy/models.py`

 * *Files 2% similar despite different names*

```diff
@@ -306,14 +306,48 @@
     code: str
 
     def __init__(self, id_: int, code: str) -> None:
         self.id_ = id_
         self.code = code
 
 
+class Budget:
+    id_: int
+    code: str
+
+    def __init__(self, id_: int, code: str) -> None:
+        self.id_ = id_
+        self.code = code
+
+
+class BudgetDetail:
+    id_: int
+    budget_id: int
+    hierarchy1_value: str
+    hierarchy2_value: str
+    hierarchy3_value: str
+
+    def __init__(self, id_: int, budget_id: int, hierarchy1_value: str,
+                 hierarchy2_value: str, hierarchy3_value: str) -> None:
+        self.id_ = id_
+        self.budget_id = budget_id
+        self.hierarchy1_value = hierarchy1_value
+        self.hierarchy2_value = hierarchy2_value
+        self.hierarchy3_value = hierarchy3_value
+
+
+class BudgetData:
+    budget: Budget
+    budget_detail: BudgetDetail
+
+    def __init__(self, budget: Dict, budget_detail: Dict):
+        self.budget = Budget(**budget)
+        self.budget_detail = BudgetDetail(**budget_detail)
+
+
 class DunningData:
     dunningblock: bool
     dunning_level: Optional[DunningLevel]
 
     def __init__(self, dunningblock: bool, dunning_level: Dict = None) -> None:
         self.dunningblock = dunningblock
         if dunning_level is not None:
@@ -471,14 +505,15 @@
     unit_price: int
     gross_amount: int
     net_amount: int
     units: int
     commission_text: str
     internal_description: str
     position_number: int
+    budget_data: Optional[BudgetData]
     sales_tax: SalesTax
     service_catalogue: ServiceCatalogue
     craft_activity: CraftActivity
     quantity_type: Optional[QuantityType]
     component: Optional[Component]
     facility: Optional[Facility]
     approved_net_amount: int
@@ -489,14 +524,15 @@
                  unit_price: int,
                  gross_amount: int,
                  net_amount: int,
                  units: int,
                  commission_text: str,
                  internal_description: str,
                  position_number: int,
+                 budget_data: Dict,
                  sales_tax: Dict,
                  service_catalogue: Dict,
                  craft_activity: Dict,
                  quantity_type: Dict,
                  component: Dict,
                  facility: Dict,
                  approved_net_amount: int,
@@ -506,14 +542,19 @@
         self.unit_price = unit_price
         self.gross_amount = gross_amount
         self.net_amount = net_amount
         self.units = units
         self.commission_text = commission_text
         self.internal_description = internal_description
         self.position_number = position_number
+        if budget_data is not None:
+            budget_data["id_"] = budget_data.pop("id")
+            self.budget_data = BudgetData(**budget_data)
+        else:
+            self.budget_data = None
         sales_tax["id_"] = sales_tax.pop("id")
         self.sales_tax = SalesTax(**sales_tax)
         service_catalogue["id_"] = service_catalogue.pop("id")
         self.service_catalogue = ServiceCatalogue(**service_catalogue)
         craft_activity["id_"] = craft_activity.pop("id")
         self.craft_activity = CraftActivity(**craft_activity)
         if quantity_type is not None:
```

### Comparing `wowipy-1.1.5/wowipy/rest_adapter.py` & `wowipy-1.1.6/wowipy/rest_adapter.py`

 * *Files identical despite different names*

### Comparing `wowipy-1.1.5/wowipy/wowipy.py` & `wowipy-1.1.6/wowipy/wowipy.py`

 * *Files identical despite different names*

### Comparing `wowipy-1.1.5/wowipy.egg-info/PKG-INFO` & `wowipy-1.1.6/wowipy.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: wowipy
-Version: 1.1.5
+Version: 1.1.6
 Summary: OPENWOWI Wowiport API wrapper for python
 Home-page: https://github.com/seb-bau/WowiPy
 Author: Sebastian Bauhaus
 Author-email: sebastian@bytewish.de
 License: GPL-3.0
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
```

