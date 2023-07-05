# Comparing `tmp/odoo_addons_oca_server_ux-16.0.20230622.1-py3-none-any.whl.zip` & `tmp/odoo_addons_oca_server_ux-16.0.20230628.1-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,6 +1,6 @@
-Zip file size: 1518 bytes, number of entries: 4
--rw-r--r--  2.0 unx     1331 b- defN 23-Jun-23 05:12 odoo_addons_oca_server_ux-16.0.20230622.1.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 23-Jun-23 05:12 odoo_addons_oca_server_ux-16.0.20230622.1.dist-info/WHEEL
--rw-r--r--  2.0 unx        1 b- defN 23-Jun-23 05:12 odoo_addons_oca_server_ux-16.0.20230622.1.dist-info/top_level.txt
--rw-rw-r--  2.0 unx      409 b- defN 23-Jun-23 05:12 odoo_addons_oca_server_ux-16.0.20230622.1.dist-info/RECORD
-4 files, 1833 bytes uncompressed, 712 bytes compressed:  61.2%
+Zip file size: 1546 bytes, number of entries: 4
+-rw-r--r--  2.0 unx     1543 b- defN 23-Jun-29 06:34 odoo_addons_oca_server_ux-16.0.20230628.1.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 23-Jun-29 06:34 odoo_addons_oca_server_ux-16.0.20230628.1.dist-info/WHEEL
+-rw-r--r--  2.0 unx        1 b- defN 23-Jun-29 06:34 odoo_addons_oca_server_ux-16.0.20230628.1.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx      409 b- defN 23-Jun-29 06:34 odoo_addons_oca_server_ux-16.0.20230628.1.dist-info/RECORD
+4 files, 2045 bytes uncompressed, 740 bytes compressed:  63.8%
```

## zipnote {}

```diff
@@ -1,13 +1,13 @@
-Filename: odoo_addons_oca_server_ux-16.0.20230622.1.dist-info/METADATA
+Filename: odoo_addons_oca_server_ux-16.0.20230628.1.dist-info/METADATA
 Comment: 
 
-Filename: odoo_addons_oca_server_ux-16.0.20230622.1.dist-info/WHEEL
+Filename: odoo_addons_oca_server_ux-16.0.20230628.1.dist-info/WHEEL
 Comment: 
 
-Filename: odoo_addons_oca_server_ux-16.0.20230622.1.dist-info/top_level.txt
+Filename: odoo_addons_oca_server_ux-16.0.20230628.1.dist-info/top_level.txt
 Comment: 
 
-Filename: odoo_addons_oca_server_ux-16.0.20230622.1.dist-info/RECORD
+Filename: odoo_addons_oca_server_ux-16.0.20230628.1.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## Comparing `odoo_addons_oca_server_ux-16.0.20230622.1.dist-info/METADATA` & `odoo_addons_oca_server_ux-16.0.20230628.1.dist-info/METADATA`

 * *Files 18% similar despite different names*

```diff
@@ -1,28 +1,31 @@
 Metadata-Version: 2.1
 Name: odoo-addons-oca-server-ux
-Version: 16.0.20230622.1
+Version: 16.0.20230628.1
 Summary: Meta package for oca-server-ux Odoo addons
 Home-page: UNKNOWN
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python
 Classifier: Framework :: Odoo
 Classifier: Framework :: Odoo :: 16.0
+Requires-Dist: odoo-addon-base-binary-url-import (<16.1dev,>=16.0dev)
+Requires-Dist: odoo-addon-base-cancel-confirm (<16.1dev,>=16.0dev)
 Requires-Dist: odoo-addon-base-custom-filter (<16.1dev,>=16.0dev)
 Requires-Dist: odoo-addon-base-menu-visibility-restriction (<16.1dev,>=16.0dev)
 Requires-Dist: odoo-addon-base-optional-quick-create (<16.1dev,>=16.0dev)
 Requires-Dist: odoo-addon-base-revision (<16.1dev,>=16.0dev)
 Requires-Dist: odoo-addon-base-substate (<16.1dev,>=16.0dev)
 Requires-Dist: odoo-addon-base-technical-features (<16.1dev,>=16.0dev)
 Requires-Dist: odoo-addon-base-tier-validation (<16.1dev,>=16.0dev)
 Requires-Dist: odoo-addon-base-tier-validation-formula (<16.1dev,>=16.0dev)
 Requires-Dist: odoo-addon-base-tier-validation-forward (<16.1dev,>=16.0dev)
 Requires-Dist: odoo-addon-date-range (<16.1dev,>=16.0dev)
 Requires-Dist: odoo-addon-date-range-account (<16.1dev,>=16.0dev)
 Requires-Dist: odoo-addon-multi-step-wizard (<16.1dev,>=16.0dev)
 Requires-Dist: odoo-addon-sequence-reset-period (<16.1dev,>=16.0dev)
 Requires-Dist: odoo-addon-server-action-mass-edit (<16.1dev,>=16.0dev)
+Requires-Dist: odoo-addon-test-base-binary-url-import (<16.1dev,>=16.0dev)
 Requires-Dist: odoo-addon-user-all-groups (<16.1dev,>=16.0dev)
 
 UNKNOWN
```

