# Comparing `tmp/dbl_discoverx-0.0.2.tar.gz` & `tmp/dbl_discoverx-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dbl_discoverx-0.0.2.tar", last modified: Tue Jun 27 18:07:10 2023, max compression
+gzip compressed data, was "dbl_discoverx-0.0.3.tar", last modified: Wed Jul  5 14:35:20 2023, max compression
```

## Comparing `dbl_discoverx-0.0.2.tar` & `dbl_discoverx-0.0.3.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 18:07:10.914896 dbl_discoverx-0.0.2/
--rw-r--r--   0 runner    (1001) docker     (123)     3597 2023-06-27 18:06:58.000000 dbl_discoverx-0.0.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     5598 2023-06-27 18:07:10.914896 dbl_discoverx-0.0.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     5121 2023-06-27 18:06:58.000000 dbl_discoverx-0.0.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 18:07:10.910896 dbl_discoverx-0.0.2/dbl_discoverx.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     5598 2023-06-27 18:07:10.000000 dbl_discoverx-0.0.2/dbl_discoverx.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      419 2023-06-27 18:07:10.000000 dbl_discoverx-0.0.2/dbl_discoverx.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-27 18:07:10.000000 dbl_discoverx-0.0.2/dbl_discoverx.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      151 2023-06-27 18:07:10.000000 dbl_discoverx-0.0.2/dbl_discoverx.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       10 2023-06-27 18:07:10.000000 dbl_discoverx-0.0.2/dbl_discoverx.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 18:07:10.914896 dbl_discoverx-0.0.2/discoverx/
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-06-27 18:06:58.000000 dbl_discoverx-0.0.2/discoverx/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 18:07:10.914896 dbl_discoverx-0.0.2/discoverx/common/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-27 18:06:58.000000 dbl_discoverx-0.0.2/discoverx/common/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1164 2023-06-27 18:06:58.000000 dbl_discoverx-0.0.2/discoverx/common/helper.py
--rw-r--r--   0 runner    (1001) docker     (123)    16235 2023-06-27 18:06:58.000000 dbl_discoverx-0.0.2/discoverx/dx.py
--rw-r--r--   0 runner    (1001) docker     (123)      683 2023-06-27 18:06:58.000000 dbl_discoverx-0.0.2/discoverx/logging.py
--rw-r--r--   0 runner    (1001) docker     (123)     7676 2023-06-27 18:06:58.000000 dbl_discoverx-0.0.2/discoverx/msql.py
--rw-r--r--   0 runner    (1001) docker     (123)    19554 2023-06-27 18:06:58.000000 dbl_discoverx-0.0.2/discoverx/rules.py
--rw-r--r--   0 runner    (1001) docker     (123)    13615 2023-06-27 18:06:58.000000 dbl_discoverx-0.0.2/discoverx/scanner.py
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-06-27 18:06:58.000000 dbl_discoverx-0.0.2/discoverx/version.py
--rw-r--r--   0 runner    (1001) docker     (123)      720 2023-06-27 18:06:58.000000 dbl_discoverx-0.0.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-27 18:07:10.914896 dbl_discoverx-0.0.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2305 2023-06-27 18:06:58.000000 dbl_discoverx-0.0.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 14:35:20.392141 dbl_discoverx-0.0.3/
+-rw-r--r--   0 runner    (1001) docker     (123)     3597 2023-07-05 14:35:07.000000 dbl_discoverx-0.0.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     5693 2023-07-05 14:35:20.392141 dbl_discoverx-0.0.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     5216 2023-07-05 14:35:07.000000 dbl_discoverx-0.0.3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 14:35:20.388141 dbl_discoverx-0.0.3/dbl_discoverx.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     5693 2023-07-05 14:35:20.000000 dbl_discoverx-0.0.3/dbl_discoverx.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      419 2023-07-05 14:35:20.000000 dbl_discoverx-0.0.3/dbl_discoverx.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-05 14:35:20.000000 dbl_discoverx-0.0.3/dbl_discoverx.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      156 2023-07-05 14:35:20.000000 dbl_discoverx-0.0.3/dbl_discoverx.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-07-05 14:35:20.000000 dbl_discoverx-0.0.3/dbl_discoverx.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 14:35:20.392141 dbl_discoverx-0.0.3/discoverx/
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-05 14:35:07.000000 dbl_discoverx-0.0.3/discoverx/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 14:35:20.392141 dbl_discoverx-0.0.3/discoverx/common/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-05 14:35:07.000000 dbl_discoverx-0.0.3/discoverx/common/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1164 2023-07-05 14:35:07.000000 dbl_discoverx-0.0.3/discoverx/common/helper.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16241 2023-07-05 14:35:07.000000 dbl_discoverx-0.0.3/discoverx/dx.py
+-rw-r--r--   0 runner    (1001) docker     (123)      683 2023-07-05 14:35:07.000000 dbl_discoverx-0.0.3/discoverx/logging.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7676 2023-07-05 14:35:07.000000 dbl_discoverx-0.0.3/discoverx/msql.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20876 2023-07-05 14:35:07.000000 dbl_discoverx-0.0.3/discoverx/rules.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13615 2023-07-05 14:35:07.000000 dbl_discoverx-0.0.3/discoverx/scanner.py
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-07-05 14:35:07.000000 dbl_discoverx-0.0.3/discoverx/version.py
+-rw-r--r--   0 runner    (1001) docker     (123)      720 2023-07-05 14:35:07.000000 dbl_discoverx-0.0.3/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-05 14:35:20.392141 dbl_discoverx-0.0.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2340 2023-07-05 14:35:07.000000 dbl_discoverx-0.0.3/setup.py
```

### Comparing `dbl_discoverx-0.0.2/LICENSE` & `dbl_discoverx-0.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `dbl_discoverx-0.0.2/PKG-INFO` & `dbl_discoverx-0.0.3/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,30 +1,25 @@
 Metadata-Version: 2.1
 Name: dbl_discoverx
-Version: 0.0.2
+Version: 0.0.3
 Summary: DiscoverX - Map and Search your Lakehouse
 Home-page: https://databricks.com/learn/labs
 Author: Erni Durdevic, David Tempelmann
 Author-email: labs@databricks.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: Other/Proprietary License
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
 Provides-Extra: local
 Provides-Extra: test
 License-File: LICENSE
 
 # DiscoverX
 
-Scan, Classify, and Discover the content of your Lakehouse
-
-## Requirements
-
-* A [Databricks workspace](https://www.databricks.com/try-databricks#account)
-* [Unity Catalog](https://www.databricks.com/product/unity-catalog)
+Scan, Classify, and Discover the content of your Lakehouse.
 
 ## Getting started
 
 Install DiscoverX, in Databricks notebook type
 
 ```
 %pip install dbl-discoverx
@@ -35,47 +30,54 @@
 ```
 from discoverx import DX
 dx = DX(locale="US")
 ```
 
 ## Scan & classify
 
-You can now scan the content of any set of tables for
-- IP addresses (v4 and v6)
-- Email addresses
-- URLs
-- ... and many more
-
-See the full list of rules with 
+You can scan a sample of 10k rows from each table with
 
 ```
-dx.display_rules()
+dx.scan(from_tables="*.*.*")
 ```
 
-You can also provide your [custom matching rules](#custom-rules).
+Check out the [scan parameters](#scan-parameters) for more details.
 
-The scan will automatically classify columns.
+The scan result is a dataset with a `score` column, which defines the fraction of matched records against the total records scanned for each rule.
 
+### Available classes
 
-### Example
+The supported classes are:
+- IP v4 addresses
+- IP v6 addresses
+- Email addresses
+- URLs
+- fqdn (Fully qualified domain names)
+- Credit card number
+- Credit card expiration date
+- Iso date
+- Iso date time
+- Mac address
+
+US locale specific classes
+- us_mailing_address
+- us_phone_number
+- us_social_security_number
+- us_state
+- us_state_abbreviation
+- us_zip_code
 
-Scan all (samples 10k rows from each table)
+See the list of available classification rules with 
 
 ```
-dx.scan(from_tables="*.*.*")
+dx.display_rules()
 ```
 
-Check out the [scan parameters](#scan-parameters).
-
-The result is a dataset with a `score` column, which defines the fraction of matched records against the total records scanned for each rule.
-The full scan result can be displayed using
+You can also provide your [custom matching rules](#custom-rules).
 
-```
-dx.scan_result
-```
 
 ## Save & Load the Scan Results
 
 After a `scan` you can save the scan results in a delta table of your choice.
 
 ```
 dx.save(full_table_name=<your-table-name>)
@@ -157,20 +159,18 @@
 
 ### Scan parameters
 
 You can define 
 
 ```
 dx.scan(
-    catalogs="*",      # Catalog filter ('*' is a wildcard)
-    schemas="*",       # Database filter ('*' is a wildcard)
-    tables="*",        # Table filter ('*' is a wildcard)
-    rules="*",         # Rule filter ('*' is a wildcard) or list[string]
-    sample_size=10000, # Number of rows to sample, use None for a full table scan
-    what_if=False      # If `True` it prints the SQL that would be executed
+    from_tables="*.*.*", # Table pattern in form of <catalog>.<schema>.<table> ('*' is a wildcard)
+    rules="*",           # Rule filter ('*' is a wildcard)
+    sample_size=10000,   # Number of rows to sample, use None for a full table scan
+    what_if=False        # If `True` it prints the SQL that would be executed
 )
 ```
 
 ### Custom rules
 
 You can provide your custom scanning rules based on regex expressions.
 
@@ -190,12 +190,17 @@
 
 You should now see your rules added to the default ones with
 
 ```
 dx.display_rules()
 ```
 
+## Requirements
+
+* A [Databricks workspace](https://www.databricks.com/try-databricks#account)
+* [Unity Catalog](https://www.databricks.com/product/unity-catalog)
+
 ## Project Support
 Please note that all projects in the /databrickslabs github account are provided for your exploration only, and are not formally supported by Databricks with Service Level Agreements (SLAs).  They are provided AS-IS and we do not make any guarantees of any kind.  Please do not submit a support ticket relating to any issues arising from the use of these projects.
 
 Any issues discovered through the use of this project should be filed as GitHub Issues on the Repo.  They will be reviewed as time permits, but there are no formal SLAs for support.
```

### Comparing `dbl_discoverx-0.0.2/README.md` & `dbl_discoverx-0.0.3/README.md`

 * *Files 5% similar despite different names*

```diff
@@ -1,15 +1,10 @@
 # DiscoverX
 
-Scan, Classify, and Discover the content of your Lakehouse
-
-## Requirements
-
-* A [Databricks workspace](https://www.databricks.com/try-databricks#account)
-* [Unity Catalog](https://www.databricks.com/product/unity-catalog)
+Scan, Classify, and Discover the content of your Lakehouse.
 
 ## Getting started
 
 Install DiscoverX, in Databricks notebook type
 
 ```
 %pip install dbl-discoverx
@@ -20,47 +15,54 @@
 ```
 from discoverx import DX
 dx = DX(locale="US")
 ```
 
 ## Scan & classify
 
-You can now scan the content of any set of tables for
-- IP addresses (v4 and v6)
-- Email addresses
-- URLs
-- ... and many more
-
-See the full list of rules with 
+You can scan a sample of 10k rows from each table with
 
 ```
-dx.display_rules()
+dx.scan(from_tables="*.*.*")
 ```
 
-You can also provide your [custom matching rules](#custom-rules).
+Check out the [scan parameters](#scan-parameters) for more details.
 
-The scan will automatically classify columns.
+The scan result is a dataset with a `score` column, which defines the fraction of matched records against the total records scanned for each rule.
 
+### Available classes
 
-### Example
+The supported classes are:
+- IP v4 addresses
+- IP v6 addresses
+- Email addresses
+- URLs
+- fqdn (Fully qualified domain names)
+- Credit card number
+- Credit card expiration date
+- Iso date
+- Iso date time
+- Mac address
+
+US locale specific classes
+- us_mailing_address
+- us_phone_number
+- us_social_security_number
+- us_state
+- us_state_abbreviation
+- us_zip_code
 
-Scan all (samples 10k rows from each table)
+See the list of available classification rules with 
 
 ```
-dx.scan(from_tables="*.*.*")
+dx.display_rules()
 ```
 
-Check out the [scan parameters](#scan-parameters).
-
-The result is a dataset with a `score` column, which defines the fraction of matched records against the total records scanned for each rule.
-The full scan result can be displayed using
+You can also provide your [custom matching rules](#custom-rules).
 
-```
-dx.scan_result
-```
 
 ## Save & Load the Scan Results
 
 After a `scan` you can save the scan results in a delta table of your choice.
 
 ```
 dx.save(full_table_name=<your-table-name>)
@@ -142,20 +144,18 @@
 
 ### Scan parameters
 
 You can define 
 
 ```
 dx.scan(
-    catalogs="*",      # Catalog filter ('*' is a wildcard)
-    schemas="*",       # Database filter ('*' is a wildcard)
-    tables="*",        # Table filter ('*' is a wildcard)
-    rules="*",         # Rule filter ('*' is a wildcard) or list[string]
-    sample_size=10000, # Number of rows to sample, use None for a full table scan
-    what_if=False      # If `True` it prints the SQL that would be executed
+    from_tables="*.*.*", # Table pattern in form of <catalog>.<schema>.<table> ('*' is a wildcard)
+    rules="*",           # Rule filter ('*' is a wildcard)
+    sample_size=10000,   # Number of rows to sample, use None for a full table scan
+    what_if=False        # If `True` it prints the SQL that would be executed
 )
 ```
 
 ### Custom rules
 
 You can provide your custom scanning rules based on regex expressions.
 
@@ -175,12 +175,17 @@
 
 You should now see your rules added to the default ones with
 
 ```
 dx.display_rules()
 ```
 
+## Requirements
+
+* A [Databricks workspace](https://www.databricks.com/try-databricks#account)
+* [Unity Catalog](https://www.databricks.com/product/unity-catalog)
+
 ## Project Support
 Please note that all projects in the /databrickslabs github account are provided for your exploration only, and are not formally supported by Databricks with Service Level Agreements (SLAs).  They are provided AS-IS and we do not make any guarantees of any kind.  Please do not submit a support ticket relating to any issues arising from the use of these projects.
 
 Any issues discovered through the use of this project should be filed as GitHub Issues on the Repo.  They will be reviewed as time permits, but there are no formal SLAs for support.
```

### Comparing `dbl_discoverx-0.0.2/dbl_discoverx.egg-info/PKG-INFO` & `dbl_discoverx-0.0.3/dbl_discoverx.egg-info/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,30 +1,25 @@
 Metadata-Version: 2.1
 Name: dbl-discoverx
-Version: 0.0.2
+Version: 0.0.3
 Summary: DiscoverX - Map and Search your Lakehouse
 Home-page: https://databricks.com/learn/labs
 Author: Erni Durdevic, David Tempelmann
 Author-email: labs@databricks.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: Other/Proprietary License
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
 Provides-Extra: local
 Provides-Extra: test
 License-File: LICENSE
 
 # DiscoverX
 
-Scan, Classify, and Discover the content of your Lakehouse
-
-## Requirements
-
-* A [Databricks workspace](https://www.databricks.com/try-databricks#account)
-* [Unity Catalog](https://www.databricks.com/product/unity-catalog)
+Scan, Classify, and Discover the content of your Lakehouse.
 
 ## Getting started
 
 Install DiscoverX, in Databricks notebook type
 
 ```
 %pip install dbl-discoverx
@@ -35,47 +30,54 @@
 ```
 from discoverx import DX
 dx = DX(locale="US")
 ```
 
 ## Scan & classify
 
-You can now scan the content of any set of tables for
-- IP addresses (v4 and v6)
-- Email addresses
-- URLs
-- ... and many more
-
-See the full list of rules with 
+You can scan a sample of 10k rows from each table with
 
 ```
-dx.display_rules()
+dx.scan(from_tables="*.*.*")
 ```
 
-You can also provide your [custom matching rules](#custom-rules).
+Check out the [scan parameters](#scan-parameters) for more details.
 
-The scan will automatically classify columns.
+The scan result is a dataset with a `score` column, which defines the fraction of matched records against the total records scanned for each rule.
 
+### Available classes
 
-### Example
+The supported classes are:
+- IP v4 addresses
+- IP v6 addresses
+- Email addresses
+- URLs
+- fqdn (Fully qualified domain names)
+- Credit card number
+- Credit card expiration date
+- Iso date
+- Iso date time
+- Mac address
+
+US locale specific classes
+- us_mailing_address
+- us_phone_number
+- us_social_security_number
+- us_state
+- us_state_abbreviation
+- us_zip_code
 
-Scan all (samples 10k rows from each table)
+See the list of available classification rules with 
 
 ```
-dx.scan(from_tables="*.*.*")
+dx.display_rules()
 ```
 
-Check out the [scan parameters](#scan-parameters).
-
-The result is a dataset with a `score` column, which defines the fraction of matched records against the total records scanned for each rule.
-The full scan result can be displayed using
+You can also provide your [custom matching rules](#custom-rules).
 
-```
-dx.scan_result
-```
 
 ## Save & Load the Scan Results
 
 After a `scan` you can save the scan results in a delta table of your choice.
 
 ```
 dx.save(full_table_name=<your-table-name>)
@@ -157,20 +159,18 @@
 
 ### Scan parameters
 
 You can define 
 
 ```
 dx.scan(
-    catalogs="*",      # Catalog filter ('*' is a wildcard)
-    schemas="*",       # Database filter ('*' is a wildcard)
-    tables="*",        # Table filter ('*' is a wildcard)
-    rules="*",         # Rule filter ('*' is a wildcard) or list[string]
-    sample_size=10000, # Number of rows to sample, use None for a full table scan
-    what_if=False      # If `True` it prints the SQL that would be executed
+    from_tables="*.*.*", # Table pattern in form of <catalog>.<schema>.<table> ('*' is a wildcard)
+    rules="*",           # Rule filter ('*' is a wildcard)
+    sample_size=10000,   # Number of rows to sample, use None for a full table scan
+    what_if=False        # If `True` it prints the SQL that would be executed
 )
 ```
 
 ### Custom rules
 
 You can provide your custom scanning rules based on regex expressions.
 
@@ -190,12 +190,17 @@
 
 You should now see your rules added to the default ones with
 
 ```
 dx.display_rules()
 ```
 
+## Requirements
+
+* A [Databricks workspace](https://www.databricks.com/try-databricks#account)
+* [Unity Catalog](https://www.databricks.com/product/unity-catalog)
+
 ## Project Support
 Please note that all projects in the /databrickslabs github account are provided for your exploration only, and are not formally supported by Databricks with Service Level Agreements (SLAs).  They are provided AS-IS and we do not make any guarantees of any kind.  Please do not submit a support ticket relating to any issues arising from the use of these projects.
 
 Any issues discovered through the use of this project should be filed as GitHub Issues on the Repo.  They will be reviewed as time permits, but there are no formal SLAs for support.
```

### Comparing `dbl_discoverx-0.0.2/discoverx/common/helper.py` & `dbl_discoverx-0.0.3/discoverx/common/helper.py`

 * *Files identical despite different names*

### Comparing `dbl_discoverx-0.0.2/discoverx/dx.py` & `dbl_discoverx-0.0.3/discoverx/dx.py`

 * *Files 1% similar despite different names*

```diff
@@ -240,15 +240,15 @@
             raise ValueError(f"The provided by_class {by_class} must be of string type.")
 
         sql_filter = f"[{search_matching_rules[0]}] = '{search_term}'"
         select_statement = (
             "named_struct("
             + ", ".join(
                 [
-                    f"'{rule_name}', named_struct('column_name', '[{rule_name}]', 'value', [{rule_name}])"
+                    f"'{rule_name}', named_struct('column_name', '[{rule_name}]', 'value', `[{rule_name}]`)"
                     for rule_name in search_matching_rules
                 ]
             )
             + ") AS search_result"
         )
 
         if search_term is None:
@@ -298,15 +298,15 @@
                 f" either a str or List[str]."
             )
 
         from_statement = (
             "named_struct("
             + ", ".join(
                 [
-                    f"'{class_name}', named_struct('column_name', '[{class_name}]', 'value', [{class_name}])"
+                    f"'{class_name}', named_struct('column_name', '[{class_name}]', 'value', `[{class_name}]`)"
                     for class_name in by_classes
                 ]
             )
             + ") AS classified_columns"
         )
 
         return self._msql(
@@ -367,15 +367,15 @@
                 f"Please confirm that you want to delete the following values from the table {from_tables} using the class {by_class}: {values}"
             )
             self.logger.friendly(
                 f"If you are sure, please run the same command again but set the parameter yes_i_am_sure to True."
             )
 
         delete_result = self._msql(
-            f"DELETE FROM {from_tables} WHERE [{by_class}] IN ({value_string})",
+            f"DELETE FROM {from_tables} WHERE `[{by_class}]` IN ({value_string})",
             what_if=(not yes_i_am_sure),
             min_score=min_score,
         )
 
         if delete_result is not None:
             delete_result = delete_result.toPandas()
             self.logger.friendlyHTML(f"<p>The affcted tables are</p>{delete_result.to_html()}")
```

### Comparing `dbl_discoverx-0.0.2/discoverx/logging.py` & `dbl_discoverx-0.0.3/discoverx/logging.py`

 * *Files identical despite different names*

### Comparing `dbl_discoverx-0.0.2/discoverx/msql.py` & `dbl_discoverx-0.0.3/discoverx/msql.py`

 * *Files identical despite different names*

### Comparing `dbl_discoverx-0.0.2/discoverx/rules.py` & `dbl_discoverx-0.0.3/discoverx/rules.py`

 * *Files 4% similar despite different names*

```diff
@@ -4,24 +4,29 @@
 """
 
 from dataclasses import dataclass
 from enum import Enum
 from fnmatch import fnmatch
 import re
 from typing import Union, Optional, List
-from pydantic import BaseModel, validator
+from pydantic import BaseModel, field_validator
 
 
 class RuleTypes(str, Enum):
     """Allowed types/choices for Rules"""
 
     REGEX = "regex"
 
 
 class Rule(BaseModel):
+    """Parent class for rules
+    Attributes:
+        type (RuleTypes): Defines the type of Rule, e.g. Regex
+    """
+
     type: RuleTypes
 
 
 class RegexRule(Rule):
     """Definition of Regex Rule that applies to a column content
     Attributes:
         name (str): Name of rule
@@ -32,45 +37,69 @@
         match_example (str, optional): It is possible to provide an example of
             a string/expression to be matched by the Rule. This example
             is used to validate the Rule upon instantiation.
         class_name (str, optional): Name of the class used to select columns in unity
             catalog
     """
 
-    type = RuleTypes.REGEX
+    type: RuleTypes = RuleTypes.REGEX
 
     name: str
     description: str
     definition: str
     match_example: Optional[Union[str, List[str]]] = None
     nomatch_example: Optional[Union[str, List[str]]] = None
     class_name: Optional[str] = None
 
     # pylint: disable=no-self-argument
-    @validator("match_example")
+    @field_validator("match_example")
     def validate_match_example(cls, match_example, values):
+        """Validate regular expression
+        This validator checks that the regular expression matches
+        the provided match_example.
+
+        Args:
+            match_example (List): A list of strings supposed to match the
+                defined regular expression
+            values (ValidationInfo): values.data provides dictionary of
+            remaining fields
+
+        Returns: List of specified examples
+        """
         return cls.validate_rule(match_example, values, False)
 
     # pylint: disable=no-self-argument
-    @validator("nomatch_example")
+    @field_validator("nomatch_example")
     def validate_nomatch_example(cls, nomatch_example, values):
+        """Validate regular expression
+        This validator checks that the regular expression does not match
+        the provided nomatch_example.
+
+        Args:
+            nomatch_example (List): A list of strings supposed to not
+                match the defined regular expression
+            values (ValidationInfo): values.data provides dictionary of
+                remaining fields
+
+        Returns: List of specified examples
+        """
         return cls.validate_rule(nomatch_example, values, True)
 
     @staticmethod
     def validate_rule(example, values, fail_match: bool):
         """Validates that given example is matched by defined pattern"""
         if not isinstance(example, list):
             validation_example = [example]
         else:
             validation_example = example
 
         for ex in validation_example:
-            if (not re.match(values["definition"], ex)) != fail_match:
+            if (not re.match(values.data["definition"], ex)) != fail_match:
                 raise ValueError(
-                    f"The definition of the rule {values['name']} does not match the provided example {ex}"
+                    f"The definition of the rule {values.data['name']} does not match the provided example {ex}"
                 )
         return example
 
 
 @dataclass
 class RulesList:
     """A list of rules with added properties
@@ -95,18 +124,19 @@
     def number_of_rules(self) -> int:
         """Return the number of rules in the list."""
         if self.rules:
             return len(self.rules)
         return 0
 
     def test_match(self, input_string: str):
+        """Return a list of rules which match the given input string"""
         if self.rules is not None:
             return [rule.name for rule in self.rules if re.match(rule.definition, input_string)]
-        else:
-            return []
+
+        return []
 
 
 # define builtin rules
 global_rules = [
     RegexRule(
         name="credit_card_expiration_date",
         description="Credit Card Expiration Date",
@@ -498,15 +528,15 @@
         Args:
             locale (str, optional): The locale to use. Defaults to None.
             custom_rules (List[Rule], optional): A list of
                 custom-defined rules. Defaults to None.
         """
         rules = global_rules.copy()
         if locale is not None:
-            if locale.lower() not in localized_rules.keys():
+            if locale.lower() not in localized_rules:
                 raise ValueError(f"Unsupported locale: {locale}. Use one of {localized_rules.keys()}")
             rules += localized_rules[locale.lower()]
         self.builtin_rules: RulesList = RulesList(rules)
         self.custom_rules = RulesList(custom_rules)
 
     def get_rules_info(self):
         """Returns info about the available rules
@@ -565,8 +595,16 @@
         Returns:
             A list of rules from the specified rule set matching the
             wildcard.
         """
         return [rule for rule in (rule_set if rule_set is not None else []) if fnmatch(rule.name, rule_filter)]
 
     def match_search_term(self, search_term: str):
+        """Return list of rules matching the search term
+
+        Args:
+            search_term: A string to be matched by the available rules
+
+        Returns:
+            A list of matching rules, both custom and built-in
+        """
         return self.builtin_rules.test_match(search_term) + self.custom_rules.test_match(search_term)
```

### Comparing `dbl_discoverx-0.0.2/discoverx/scanner.py` & `dbl_discoverx-0.0.3/discoverx/scanner.py`

 * *Files identical despite different names*

### Comparing `dbl_discoverx-0.0.2/pyproject.toml` & `dbl_discoverx-0.0.3/pyproject.toml`

 * *Files identical despite different names*

### Comparing `dbl_discoverx-0.0.2/setup.py` & `dbl_discoverx-0.0.3/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -12,24 +12,24 @@
 DESCRIPTION = "DiscoverX - Map and Search your Lakehouse"
 
 this_directory = path.abspath(path.dirname(__file__))
 with open(path.join(this_directory, "README.md"), encoding="utf-8") as f:
     LONG_DESCRIPTION = f.read()
 
 # import version
-VERSIONFILE = "discoverx/version.py"
-version_line = open(VERSIONFILE, "rt").read()
+with open(path.join(this_directory, "discoverx/version.py"), encoding="utf-8") as f:
+    version_line = f.read()
 VERSION_PATTERN = r"^__version__ = ['\"]([^'\"]*)['\"]"
 parsed_version = re.search(VERSION_PATTERN, version_line, re.M)
 if parsed_version:
     version_string = parsed_version.group(1)
 else:
-    raise RuntimeError("Unable to find version string in %s." % (VERSIONFILE,))
+    raise RuntimeError("Unable to find version string in discoverx/version.py")
 
-PACKAGE_REQUIREMENTS = ["pyyaml", "pydantic"]
+PACKAGE_REQUIREMENTS = ["pyyaml", "pydantic>=2.0"]
 
 # packages for local development and unit testing
 # please note that these packages are already available in DBR, there is no need to install them on DBR.
 LOCAL_REQUIREMENTS = [
     "pyspark>=3.3.0",
     "delta-spark>=2.2.0",
     "pandas<2.0.0",  # From 2.0.0 onwards, pandas does not support iteritems() anymore, spark.createDataFrame will fail
```

