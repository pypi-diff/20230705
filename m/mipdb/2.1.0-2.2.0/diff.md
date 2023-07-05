# Comparing `tmp/mipdb-2.1.0.tar.gz` & `tmp/mipdb-2.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mipdb-2.1.0.tar", max compression
+gzip compressed data, was "mipdb-2.2.0.tar", max compression
```

## Comparing `mipdb-2.1.0.tar` & `mipdb-2.2.0.tar`

### file list

```diff
@@ -1,14 +1,14 @@
--rw-r--r--   0        0        0      965 2023-04-24 10:54:41.260132 mipdb-2.1.0/mipdb/__init__.py
--rw-r--r--   0        0        0    13744 2023-04-24 10:54:41.260132 mipdb-2.1.0/mipdb/commands.py
--rw-r--r--   0        0        0      696 2023-04-24 10:54:41.260132 mipdb-2.1.0/mipdb/data_frame.py
--rw-r--r--   0        0        0     2345 2023-04-24 10:54:41.260132 mipdb-2.1.0/mipdb/data_frame_schema.py
--rw-r--r--   0        0        0    18348 2023-04-24 10:54:41.260132 mipdb-2.1.0/mipdb/database.py
--rw-r--r--   0        0        0     4140 2023-04-24 10:54:41.260132 mipdb-2.1.0/mipdb/dataelements.py
--rw-r--r--   0        0        0     2623 2023-04-24 10:54:41.260132 mipdb-2.1.0/mipdb/exceptions.py
--rw-r--r--   0        0        0     1697 2023-04-24 10:54:41.260132 mipdb-2.1.0/mipdb/properties.py
--rw-r--r--   0        0        0     1061 2023-04-24 10:54:41.260132 mipdb-2.1.0/mipdb/reader.py
--rw-r--r--   0        0        0      746 2023-04-24 10:54:41.260132 mipdb-2.1.0/mipdb/schema.py
--rw-r--r--   0        0        0    16219 2023-04-24 10:54:41.260132 mipdb-2.1.0/mipdb/tables.py
--rw-r--r--   0        0        0    41554 2023-04-24 10:54:41.260132 mipdb-2.1.0/mipdb/usecases.py
--rw-r--r--   0        0        0     1133 2023-04-24 10:54:41.260132 mipdb-2.1.0/pyproject.toml
--rw-r--r--   0        0        0      464 1970-01-01 00:00:00.000000 mipdb-2.1.0/PKG-INFO
+-rw-r--r--   0        0        0      965 2023-07-05 14:29:48.480403 mipdb-2.2.0/mipdb/__init__.py
+-rw-r--r--   0        0        0    14639 2023-07-05 14:29:48.480403 mipdb-2.2.0/mipdb/commands.py
+-rw-r--r--   0        0        0      696 2023-07-05 14:29:48.480403 mipdb-2.2.0/mipdb/data_frame.py
+-rw-r--r--   0        0        0     2385 2023-07-05 14:29:48.480403 mipdb-2.2.0/mipdb/data_frame_schema.py
+-rw-r--r--   0        0        0    18348 2023-07-05 14:29:48.480403 mipdb-2.2.0/mipdb/database.py
+-rw-r--r--   0        0        0     5188 2023-07-05 14:29:48.480403 mipdb-2.2.0/mipdb/dataelements.py
+-rw-r--r--   0        0        0     2623 2023-07-05 14:29:48.480403 mipdb-2.2.0/mipdb/exceptions.py
+-rw-r--r--   0        0        0     1697 2023-07-05 14:29:48.480403 mipdb-2.2.0/mipdb/properties.py
+-rw-r--r--   0        0        0     1061 2023-07-05 14:29:48.480403 mipdb-2.2.0/mipdb/reader.py
+-rw-r--r--   0        0        0      746 2023-07-05 14:29:48.480403 mipdb-2.2.0/mipdb/schema.py
+-rw-r--r--   0        0        0    15013 2023-07-05 14:29:48.480403 mipdb-2.2.0/mipdb/tables.py
+-rw-r--r--   0        0        0    44607 2023-07-05 14:29:48.480403 mipdb-2.2.0/mipdb/usecases.py
+-rw-r--r--   0        0        0     1133 2023-07-05 14:29:48.480403 mipdb-2.2.0/pyproject.toml
+-rw-r--r--   0        0        0      464 1970-01-01 00:00:00.000000 mipdb-2.2.0/PKG-INFO
```

### Comparing `mipdb-2.1.0/mipdb/__init__.py` & `mipdb-2.2.0/mipdb/__init__.py`

 * *Files identical despite different names*

### Comparing `mipdb-2.1.0/mipdb/commands.py` & `mipdb-2.2.0/mipdb/commands.py`

 * *Files 6% similar despite different names*

```diff
@@ -2,15 +2,20 @@
 
 import click as cl
 import os
 import glob
 
 from mipdb.database import MonetDB
 from mipdb.reader import JsonFileReader
-from mipdb.usecases import AddDataModel, Cleanup
+from mipdb.usecases import (
+    AddDataModel,
+    Cleanup,
+    ValidateDatasetNoDatabase,
+    ValidateDataModel,
+)
 from mipdb.usecases import AddPropertyToDataModel
 from mipdb.usecases import AddPropertyToDataset
 from mipdb.usecases import DeleteDataModel
 from mipdb.usecases import DeleteDataset
 from mipdb.usecases import ImportCSV
 from mipdb.usecases import InitDB
 from mipdb.exceptions import handle_errors, UserInputError
@@ -144,14 +149,35 @@
             print(f"CSV '{csv_path}' is being loaded...")
             ValidateDataset(db).execute(csv_path, copy_from_file, code, version)
             ImportCSV(db).execute(csv_path, copy_from_file, code, version)
             print(f"CSV '{csv_path}' was successfully added.")
 
 
 @entry.command()
+@cl.argument("file", required=True)
+@handle_errors
+def validate_folder(file):
+    for subdir, dirs, files in os.walk(file):
+        if dirs:
+            continue
+        print(f"Data model '{subdir}' is being validated...")
+        metadata_path = os.path.join(subdir, "CDEsMetadata.json")
+        reader = JsonFileReader(metadata_path)
+        data_model_metadata = reader.read()
+        code = data_model_metadata["code"]
+        ValidateDataModel().execute(data_model_metadata)
+        print(f"Data model '{code}' was successfully validated.")
+
+        for csv_path in glob.glob(subdir + "/*.csv"):
+            print(f"CSV '{csv_path}' is being validated...")
+            ValidateDatasetNoDatabase().execute(csv_path, data_model_metadata)
+            print(f"CSV '{csv_path}' was successfully validated.")
+
+
+@entry.command()
 @db_configs_options
 @handle_errors
 def init(ip, port, username, password, db_name):
     dbconfig = get_db_config(ip, port, username, password, db_name)
     db = MonetDB.from_config(dbconfig)
     InitDB(db).execute()
     print("Database initialized")
```

### Comparing `mipdb-2.1.0/mipdb/data_frame.py` & `mipdb-2.2.0/mipdb/data_frame.py`

 * *Files identical despite different names*

### Comparing `mipdb-2.1.0/mipdb/data_frame_schema.py` & `mipdb-2.2.0/mipdb/data_frame_schema.py`

 * *Files 6% similar despite different names*

```diff
@@ -11,20 +11,20 @@
         self, sql_type_per_column, cdes_with_min_max, cdes_with_enumerations, columns
     ) -> None:
         pa_columns = {}
         # Validating the dataset has proper values, according to the data model.
 
         # There is a need to construct a DataFrameSchema with all the constraints that the metadata is imposing
         # For each column a pandera Column is created that will contain the constraints for the specific column
-        for column in columns:
-            if column not in sql_type_per_column.keys():
-                raise InvalidDatasetError(
-                    f"The column: '{column}' does not exist in the metadata"
-                )
+        if not set(columns) <= set(sql_type_per_column.keys()):
+            raise InvalidDatasetError(
+                f"Columns:{set(columns) - set(sql_type_per_column.keys()) - {'row_id'} } are not present in the CDEs"
+            )
 
+        for column in columns:
             checks = self._get_pa_checks(
                 cdes_with_min_max, cdes_with_enumerations, column
             )
             cde_sql_type = sql_type_per_column[column]
             pa_type = self._pa_type_from_sql_type(cde_sql_type)
             pa_columns[column] = pa.Column(dtype=pa_type, checks=checks, nullable=True)
```

### Comparing `mipdb-2.1.0/mipdb/database.py` & `mipdb-2.2.0/mipdb/database.py`

 * *Files identical despite different names*

### Comparing `mipdb-2.1.0/mipdb/dataelements.py` & `mipdb-2.2.0/mipdb/dataelements.py`

 * *Files 18% similar despite different names*

```diff
@@ -40,14 +40,48 @@
             metadata
             for group_data in schema_data["groups"]
             for metadata in make_cdes(group_data)
         ]
     return cdes
 
 
+def get_sql_type_per_column(cdes):
+    return {code: json.loads(cde.metadata)["sql_type"] for code, cde in cdes.items()}
+
+
+def get_cdes_with_min_max(cdes, columns):
+    cdes_with_min_max = {}
+    for code, cde in cdes.items():
+        if code not in columns:
+            continue
+        metadata = json.loads(cde.metadata)
+        max_value = metadata["max"] if "max" in metadata else None
+        min_value = metadata["min"] if "min" in metadata else None
+        if code in columns and min_value or max_value:
+            cdes_with_min_max[code] = (min_value, max_value)
+    return cdes_with_min_max
+
+
+def get_cdes_with_enumerations(cdes, columns):
+    return {
+        code: [
+            enum_code
+            for enum_code, enum_label in json.loads(cde.metadata)[
+                "enumerations"
+            ].items()
+        ]
+        for code, cde in cdes.items()
+        if json.loads(cde.metadata)["is_categorical"] and code in columns
+    }
+
+
+def get_dataset_enums(cdes):
+    return json.loads(cdes["dataset"].metadata)["enumerations"]
+
+
 def validate_dataset_present_on_cdes_with_proper_format(cdes):
     dataset_cde = [cde for cde in cdes if cde.code == "dataset"]
     if not dataset_cde:
         raise InvalidDataModelError("There is no 'dataset' CDE in the data model.")
     dataset_metadata = json.loads(dataset_cde[0].metadata)
     if not dataset_metadata["is_categorical"]:
         raise InvalidDataModelError(
```

### Comparing `mipdb-2.1.0/mipdb/exceptions.py` & `mipdb-2.2.0/mipdb/exceptions.py`

 * *Files identical despite different names*

### Comparing `mipdb-2.1.0/mipdb/properties.py` & `mipdb-2.2.0/mipdb/properties.py`

 * *Files identical despite different names*

### Comparing `mipdb-2.1.0/mipdb/reader.py` & `mipdb-2.2.0/mipdb/reader.py`

 * *Files identical despite different names*

### Comparing `mipdb-2.1.0/mipdb/schema.py` & `mipdb-2.2.0/mipdb/schema.py`

 * *Files identical despite different names*

### Comparing `mipdb-2.1.0/mipdb/tables.py` & `mipdb-2.2.0/mipdb/tables.py`

 * *Files 5% similar despite different names*

```diff
@@ -339,47 +339,14 @@
         # Needs to be overridden because sqlalchemy and monetdb are not cooperating
         # well when inserting values to JSON columns
         query = sql.text(
             f'INSERT INTO "{self.schema}".{METADATA_TABLE} VALUES(:code, :metadata)'
         )
         db.execute(query, values)
 
-    def get_dataset_enums(self):
-        return json.loads(self.table["dataset"].metadata)["enumerations"]
-
-    def get_sql_type_per_column(self):
-        return {
-            code: json.loads(cde.metadata)["sql_type"]
-            for code, cde in self.table.items()
-        }
-
-    def get_cdes_with_min_max(self, columns):
-        cdes_with_min_max = {}
-        for code, cde in self.table.items():
-            if code not in columns:
-                continue
-            metadata = json.loads(cde.metadata)
-            max_value = metadata["max"] if "max" in metadata else None
-            min_value = metadata["min"] if "min" in metadata else None
-            if code in columns and min_value or max_value:
-                cdes_with_min_max[code] = (min_value, max_value)
-        return cdes_with_min_max
-
-    def get_cdes_with_enumerations(self, columns):
-        return {
-            code: [
-                enum_code
-                for enum_code, enum_label in json.loads(cde.metadata)[
-                    "enumerations"
-                ].items()
-            ]
-            for code, cde in self.table.items()
-            if json.loads(cde.metadata)["is_categorical"] and code in columns
-        }
-
 
 class TemporaryTable(Table):
     def __init__(self, dataframe_sql_type_per_column, db):
         columns = [
             sql.Column(name, STR2SQLTYPE[sql_type], quote=True)
             for name, sql_type in dataframe_sql_type_per_column.items()
         ]
```

### Comparing `mipdb-2.1.0/mipdb/usecases.py` & `mipdb-2.2.0/mipdb/usecases.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,26 +1,30 @@
 import copy
 import datetime
 import json
 from abc import ABC, abstractmethod
 
 import pandas as pd
 
-from mipdb.database import DataBase, Connection
+from mipdb.database import DataBase
 from mipdb.database import METADATA_SCHEMA
 from mipdb.data_frame_schema import DataFrameSchema
 from mipdb.exceptions import ForeignKeyError, InvalidDatasetError
 from mipdb.exceptions import UserInputError
 from mipdb.properties import Properties
 from mipdb.reader import CSVDataFrameReader
 from mipdb.schema import Schema
 from mipdb.dataelements import (
     make_cdes,
     validate_dataset_present_on_cdes_with_proper_format,
     validate_longitudinal_data_model,
+    get_sql_type_per_column,
+    get_cdes_with_min_max,
+    get_cdes_with_enumerations,
+    get_dataset_enums,
 )
 from mipdb.tables import (
     DataModelTable,
     DatasetsTable,
     ActionsTable,
     MetadataTable,
     PrimaryDataTable,
@@ -149,14 +153,22 @@
     def _create_metadata_table(self, schema, conn, cdes):
         metadata_table = MetadataTable(schema)
         metadata_table.create(conn)
         values = metadata_table.get_values_from_cdes(cdes)
         metadata_table.insert_values(values, conn)
 
 
+class ValidateDataModel(UseCase):
+    def execute(self, data_model_metadata) -> None:
+        cdes = make_cdes(copy.deepcopy(data_model_metadata))
+        validate_dataset_present_on_cdes_with_proper_format(cdes)
+        if LONGITUDINAL in data_model_metadata and data_model_metadata[LONGITUDINAL]:
+            validate_longitudinal_data_model(cdes)
+
+
 class DeleteDataModel(UseCase):
     def __init__(self, db: DataBase) -> None:
         self.db = db
         is_db_initialized(db)
 
     def execute(self, code, version, force) -> None:
         name = get_data_model_fullname(code, version)
@@ -222,16 +234,17 @@
         datasets_table = DatasetsTable(schema=metadata)
 
         with self.db.begin() as conn:
             data_model_id = data_model_table.get_data_model_id(
                 data_model_code, data_model_version, conn
             )
             metadata_table = MetadataTable.from_db(data_model, conn)
-            dataset_enumerations = metadata_table.get_dataset_enums()
-            sql_type_per_column = metadata_table.get_sql_type_per_column()
+            cdes = metadata_table.table
+            dataset_enumerations = get_dataset_enums(cdes)
+            sql_type_per_column = get_sql_type_per_column(cdes)
 
             if copy_from_file:
                 imported_datasets = self.import_csv_with_volume(
                     csv_path=csv_path,
                     sql_type_per_column=sql_type_per_column,
                     data_model=data_model,
                     conn=conn,
@@ -402,24 +415,22 @@
         with self.db.begin() as conn:
             csv_columns = pd.read_csv(csv_path, nrows=0).columns.tolist()
             if DATASET_COLUMN_NAME not in csv_columns:
                 raise InvalidDatasetError(
                     "The 'dataset' column is required to exist in the csv."
                 )
             metadata_table = MetadataTable.from_db(data_model, conn)
-            sql_type_per_column = metadata_table.get_sql_type_per_column()
-            cdes_with_min_max = metadata_table.get_cdes_with_min_max(csv_columns)
-            cdes_with_enumerations = metadata_table.get_cdes_with_enumerations(
-                csv_columns
-            )
-            dataset_enumerations = metadata_table.get_dataset_enums()
+            cdes = metadata_table.table
+            sql_type_per_column = get_sql_type_per_column(cdes)
+            cdes_with_min_max = get_cdes_with_min_max(cdes, csv_columns)
+            cdes_with_enumerations = get_cdes_with_enumerations(cdes, csv_columns)
+            dataset_enumerations = get_dataset_enums(cdes)
             if self.is_data_model_longitudinal(
                 data_model_code, data_model_version, conn
             ):
-                print("is_data_model_longitudinal")
                 are_data_valid_longitudinal(csv_path)
 
             if copy_from_file:
                 validated_datasets = self.validate_csv_with_volume(
                     csv_path,
                     sql_type_per_column,
                     cdes_with_min_max,
@@ -501,14 +512,73 @@
 
     def verify_datasets_exist_in_enumerations(self, datasets, dataset_enumerations):
         non_existing_datasets = [
             dataset for dataset in datasets if dataset not in dataset_enumerations
         ]
         if non_existing_datasets:
             raise InvalidDatasetError(
+                f"The values:'{non_existing_datasets}' are not present in the enumerations of the CDE 'dataset'."
+            )
+
+
+class ValidateDatasetNoDatabase(UseCase):
+    """
+    We separate the data validation from the importation to make sure that a csv is valid as a whole before committing it to the main table.
+    In the data validation we use chunking in order to reduce the memory footprint of the process.
+    Database constraints must NOT be used as part of the validation process since that could result in partially imported csvs.
+    """
+
+    def execute(self, csv_path, data_model_metadata) -> None:
+
+        csv_columns = pd.read_csv(csv_path, nrows=0).columns.tolist()
+        if DATASET_COLUMN_NAME not in csv_columns:
+            raise InvalidDatasetError(
+                "The 'dataset' column is required to exist in the csv."
+            )
+        cdes = make_cdes(copy.deepcopy(data_model_metadata))
+        cdes = {cde.code: cde for cde in cdes}
+        sql_type_per_column = get_sql_type_per_column(cdes)
+        cdes_with_min_max = get_cdes_with_min_max(cdes, csv_columns)
+        cdes_with_enumerations = get_cdes_with_enumerations(cdes, csv_columns)
+        dataset_enumerations = get_dataset_enums(cdes)
+        if "longitudinal" in data_model_metadata:
+            are_data_valid_longitudinal(csv_path)
+        validated_datasets = self.validate_csv(
+            csv_path,
+            sql_type_per_column,
+            cdes_with_min_max,
+            cdes_with_enumerations,
+        )
+        self.verify_datasets_exist_in_enumerations(
+            datasets=validated_datasets,
+            dataset_enumerations=dataset_enumerations,
+        )
+
+    def validate_csv(
+        self, csv_path, sql_type_per_column, cdes_with_min_max, cdes_with_enumerations
+    ):
+        imported_datasets = []
+
+        csv_columns = pd.read_csv(csv_path, nrows=0).columns.tolist()
+        dataframe_schema = DataFrameSchema(
+            sql_type_per_column, cdes_with_min_max, cdes_with_enumerations, csv_columns
+        )
+        with CSVDataFrameReader(csv_path).get_reader() as reader:
+            for dataset_data in reader:
+                dataframe = DataFrame(dataset_data)
+                dataframe_schema.validate_dataframe(dataframe.data)
+                imported_datasets = set(imported_datasets) | set(dataframe.datasets)
+        return imported_datasets
+
+    def verify_datasets_exist_in_enumerations(self, datasets, dataset_enumerations):
+        non_existing_datasets = [
+            dataset for dataset in datasets if dataset not in dataset_enumerations
+        ]
+        if non_existing_datasets:
+            raise InvalidDatasetError(
                 f"The values:'{non_existing_datasets}' are not present in the enumerations of the CDE 'dataset'."
             )
 
 
 class DeleteDataset(UseCase):
     def __init__(self, db: DataBase) -> None:
         self.db = db
```

### Comparing `mipdb-2.1.0/pyproject.toml` & `mipdb-2.2.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "mipdb"
-version = "2.1.0"
+version = "2.2.0"
 description = ""
 authors = ["Your Name <you@example.com>"]
 
 [tool.poetry.dependencies]
 python = "~3.8"
 SQLAlchemy = "~1.3"
 sqlalchemy_monetdb = "~1.0"
```

