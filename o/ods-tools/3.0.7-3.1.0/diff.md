# Comparing `tmp/ods_tools-3.0.7.tar.gz` & `tmp/ods_tools-3.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ods_tools-3.0.7.tar", last modified: Fri Jun  9 09:03:21 2023, max compression
+gzip compressed data, was "ods_tools-3.1.0.tar", last modified: Wed Jul  5 10:49:32 2023, max compression
```

## Comparing `ods_tools-3.0.7.tar` & `ods_tools-3.1.0.tar`

### file list

```diff
@@ -1,24 +1,26 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 09:03:21.818235 ods_tools-3.0.7/
--rw-r--r--   0 runner    (1001) docker     (123)     8418 2023-06-09 09:03:21.814235 ods_tools-3.0.7/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     8119 2023-06-09 09:03:04.000000 ods_tools-3.0.7/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 09:03:21.810235 ods_tools-3.0.7/ods_tools/
--rw-r--r--   0 runner    (1001) docker     (123)       76 2023-06-09 09:03:04.000000 ods_tools-3.0.7/ods_tools/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5686 2023-06-09 09:03:04.000000 ods_tools-3.0.7/ods_tools/main.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 09:03:21.814235 ods_tools-3.0.7/ods_tools/oed/
--rw-r--r--   0 runner    (1001) docker     (123)      765 2023-06-09 09:03:04.000000 ods_tools-3.0.7/ods_tools/oed/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2406 2023-06-09 09:03:04.000000 ods_tools-3.0.7/ods_tools/oed/common.py
--rw-r--r--   0 runner    (1001) docker     (123)     8981 2023-06-09 09:03:04.000000 ods_tools-3.0.7/ods_tools/oed/exposure.py
--rw-r--r--   0 runner    (1001) docker     (123)    11177 2023-06-09 09:03:04.000000 ods_tools-3.0.7/ods_tools/oed/forex.py
--rw-r--r--   0 runner    (1001) docker     (123)     6592 2023-06-09 09:03:04.000000 ods_tools-3.0.7/ods_tools/oed/oed_schema.py
--rw-r--r--   0 runner    (1001) docker     (123)     9317 2023-06-09 09:03:04.000000 ods_tools-3.0.7/ods_tools/oed/setting_schema.py
--rw-r--r--   0 runner    (1001) docker     (123)    21203 2023-06-09 09:03:04.000000 ods_tools-3.0.7/ods_tools/oed/source.py
--rw-r--r--   0 runner    (1001) docker     (123)    14835 2023-06-09 09:03:04.000000 ods_tools-3.0.7/ods_tools/oed/validator.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 09:03:21.814235 ods_tools-3.0.7/ods_tools.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     8418 2023-06-09 09:03:21.000000 ods_tools-3.0.7/ods_tools.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      468 2023-06-09 09:03:21.000000 ods_tools-3.0.7/ods_tools.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-09 09:03:21.000000 ods_tools-3.0.7/ods_tools.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       51 2023-06-09 09:03:21.000000 ods_tools-3.0.7/ods_tools.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       44 2023-06-09 09:03:21.000000 ods_tools-3.0.7/ods_tools.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       10 2023-06-09 09:03:21.000000 ods_tools-3.0.7/ods_tools.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-09 09:03:21.818235 ods_tools-3.0.7/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     3798 2023-06-09 09:03:04.000000 ods_tools-3.0.7/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 10:49:32.887395 ods_tools-3.1.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     8418 2023-07-05 10:49:32.887395 ods_tools-3.1.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     8119 2023-07-05 10:49:14.000000 ods_tools-3.1.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 10:49:32.879395 ods_tools-3.1.0/ods_tools/
+-rw-r--r--   0 runner    (1001) docker     (123)       76 2023-07-05 10:49:14.000000 ods_tools-3.1.0/ods_tools/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 10:49:32.883395 ods_tools-3.1.0/ods_tools/data/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-05 10:49:14.000000 ods_tools-3.1.0/ods_tools/data/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5686 2023-07-05 10:49:14.000000 ods_tools-3.1.0/ods_tools/main.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 10:49:32.883395 ods_tools-3.1.0/ods_tools/oed/
+-rw-r--r--   0 runner    (1001) docker     (123)      850 2023-07-05 10:49:14.000000 ods_tools-3.1.0/ods_tools/oed/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2973 2023-07-05 10:49:14.000000 ods_tools-3.1.0/ods_tools/oed/common.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9136 2023-07-05 10:49:14.000000 ods_tools-3.1.0/ods_tools/oed/exposure.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11177 2023-07-05 10:49:14.000000 ods_tools-3.1.0/ods_tools/oed/forex.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6593 2023-07-05 10:49:14.000000 ods_tools-3.1.0/ods_tools/oed/oed_schema.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9317 2023-07-05 10:49:14.000000 ods_tools-3.1.0/ods_tools/oed/setting_schema.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23272 2023-07-05 10:49:14.000000 ods_tools-3.1.0/ods_tools/oed/source.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16994 2023-07-05 10:49:14.000000 ods_tools-3.1.0/ods_tools/oed/validator.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 10:49:32.883395 ods_tools-3.1.0/ods_tools.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     8418 2023-07-05 10:49:32.000000 ods_tools-3.1.0/ods_tools.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      495 2023-07-05 10:49:32.000000 ods_tools-3.1.0/ods_tools.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-05 10:49:32.000000 ods_tools-3.1.0/ods_tools.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       51 2023-07-05 10:49:32.000000 ods_tools-3.1.0/ods_tools.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       44 2023-07-05 10:49:32.000000 ods_tools-3.1.0/ods_tools.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-07-05 10:49:32.000000 ods_tools-3.1.0/ods_tools.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-05 10:49:32.887395 ods_tools-3.1.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     3817 2023-07-05 10:49:14.000000 ods_tools-3.1.0/setup.py
```

### Comparing `ods_tools-3.0.7/PKG-INFO` & `ods_tools-3.1.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ods_tools
-Version: 3.0.7
+Version: 3.1.0
 Summary: Tools to manage ODS files
 Home-page: https://github.com/OasisLMF/OpenDataStandards
 Author: Oasis LMF
 Author-email: support@oasislmf.org
 License: UNKNOWN
 Platform: UNKNOWN
 Requires-Python: >=3.7
```

### Comparing `ods_tools-3.0.7/README.md` & `ods_tools-3.1.0/README.md`

 * *Files identical despite different names*

### Comparing `ods_tools-3.0.7/ods_tools/main.py` & `ods_tools-3.1.0/ods_tools/main.py`

 * *Files identical despite different names*

### Comparing `ods_tools-3.0.7/ods_tools/oed/__init__.py` & `ods_tools-3.1.0/ods_tools/oed/__init__.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,15 +1,17 @@
 from .exposure import OedExposure
 from .oed_schema import OedSchema
 from .setting_schema import ModelSettingSchema, AnalysisSettingSchema
 from .source import OedSource
 from .common import (
     OdsException, PANDAS_COMPRESSION_MAP, PANDAS_DEFAULT_NULL_VALUES, USUAL_FILE_NAME, OED_TYPE_TO_NAME,
-    OED_NAME_TO_TYPE, OED_IDENTIFIER_FIELDS, VALIDATOR_ON_ERROR_ACTION, DEFAULT_VALIDATION_CONFIG, OED_PERIL_COLUMNS
+    OED_NAME_TO_TYPE, OED_IDENTIFIER_FIELDS, VALIDATOR_ON_ERROR_ACTION, DEFAULT_VALIDATION_CONFIG, OED_PERIL_COLUMNS, fill_empty,
+    UnknownColumnSaveOption
 )
 
 
 __all__ = [
     'OedExposure', 'OedSchema', 'OedSource', 'ModelSettingSchema', 'AnalysisSettingSchema',
     'OdsException', 'PANDAS_COMPRESSION_MAP', 'PANDAS_DEFAULT_NULL_VALUES', 'USUAL_FILE_NAME', 'OED_TYPE_TO_NAME',
-    'OED_NAME_TO_TYPE', 'OED_IDENTIFIER_FIELDS', 'VALIDATOR_ON_ERROR_ACTION', 'DEFAULT_VALIDATION_CONFIG', 'OED_PERIL_COLUMNS',
+    'OED_NAME_TO_TYPE', 'OED_IDENTIFIER_FIELDS', 'VALIDATOR_ON_ERROR_ACTION', 'DEFAULT_VALIDATION_CONFIG', 'OED_PERIL_COLUMNS', 'fill_empty',
+    'UnknownColumnSaveOption'
 ]
```

### Comparing `ods_tools-3.0.7/ods_tools/oed/common.py` & `ods_tools-3.1.0/ods_tools/oed/common.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,13 +1,15 @@
 """
 common static variable and ods_tools exceptions
 """
 from urllib.parse import urlparse
 from pathlib import Path
 import numpy as np
+import pandas as pd
+from enum import Enum
 
 
 class OdsException(Exception):
     pass
 
 
 def is_relative(filepath):
@@ -83,13 +85,29 @@
     {'name': 'required_fields', 'on_error': 'raise'},
     {'name': 'unknown_column', 'on_error': 'raise'},
     {'name': 'valid_values', 'on_error': 'raise'},
     {'name': 'perils', 'on_error': 'raise'},
     {'name': 'occupancy_code', 'on_error': 'raise'},
     {'name': 'construction_code', 'on_error': 'raise'},
     {'name': 'country_and_area_code', 'on_error': 'raise'},
+    {'name': 'conditional_requirement', 'on_error': 'raise'},
 ]
 
 OED_PERIL_COLUMNS = ['AccPeril', 'PolPerilsCovered', 'PolPeril', 'CondPeril', 'LocPerilsCovered', 'LocPeril',
                      'ReinsPeril']
 
-BLANK_VALUES = {np.nan, '', None}
+BLANK_VALUES = {np.nan, '', None, pd.NA, pd.NaT}
+
+
+def fill_empty(df, columns, value):
+    if isinstance(columns, str):
+        columns = [columns]
+    for column in columns:
+        if df[column].dtypes.name == 'category' and value not in {None, np.nan}.union(df[column].cat.categories):
+            df[column] = df[column].cat.add_categories(value)
+        df.loc[df[column].isin(BLANK_VALUES), column] = value
+
+
+class UnknownColumnSaveOption(Enum):
+    IGNORE = 1
+    RENAME = 2
+    DELETE = 3
```

### Comparing `ods_tools-3.0.7/ods_tools/oed/exposure.py` & `ods_tools-3.1.0/ods_tools/oed/exposure.py`

 * *Files 5% similar despite different names*

```diff
@@ -5,15 +5,16 @@
     support conversion of OED to other currencies
 """
 
 import json
 from pathlib import Path
 
 from .common import (PANDAS_COMPRESSION_MAP,
-                     USUAL_FILE_NAME, OED_TYPE_TO_NAME)
+                     USUAL_FILE_NAME, OED_TYPE_TO_NAME,
+                     UnknownColumnSaveOption)
 from .oed_schema import OedSchema
 from .source import OedSource
 from .validator import Validator
 from .forex import create_currency_rates
 
 
 class OedExposure:
@@ -161,15 +162,15 @@
         Args:
             filepath (str): path to save the config file
         """
         Path(filepath).parents[0].mkdir(parents=True, exist_ok=True)
         with open(filepath, 'w') as info_file:
             json.dump(self.info, info_file, indent='  ', default=str)
 
-    def save(self, path, version_name=None, compression=None, save_config=False):
+    def save(self, path, version_name=None, compression=None, save_config=False, unknown_columns=UnknownColumnSaveOption.IGNORE):
         """
         helper function to save all OED data to a location with specific compression
         Args:
             version_name (str): use as a prefix for the file names, if None name will be taken from the cur_version file name
                           if it's a filepath
             path (str): output folder
             compression (str): type of compression to use
@@ -201,15 +202,16 @@
                     compression = oed_source.sources[oed_source.cur_version_name].get('extension')
                 if compression is None:
                     compression = 'csv'
 
             filepath = filepath.with_suffix(PANDAS_COMPRESSION_MAP[compression])
 
             oed_source.save(saved_version_name + '_' + f'{compression}',
-                            {'source_type': 'filepath', 'filepath': filepath, 'extension': compression})
+                            {'source_type': 'filepath', 'filepath': filepath, 'extension': compression},
+                            unknown_columns=unknown_columns)
         if save_config:
             self.save_config(Path(path, self.DEFAULT_EXPOSURE_CONFIG_NAME))
 
     def check(self, validation_config=None):
         """
         check that all OED files respect rules related to an OedSchema
```

### Comparing `ods_tools-3.0.7/ods_tools/oed/forex.py` & `ods_tools-3.1.0/ods_tools/oed/forex.py`

 * *Files identical despite different names*

### Comparing `ods_tools-3.0.7/ods_tools/oed/oed_schema.py` & `ods_tools-3.1.0/ods_tools/oed/oed_schema.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,12 @@
 import json
 import os
 from pathlib import Path
-import pandas as pd
 
-from .common import OdsException
+from .common import OdsException, BLANK_VALUES
 
 
 class OedSchema:
     """
     Object managing information about a certain OED schema
 
     Attributes:
@@ -160,15 +159,15 @@
             valid_ranges (list): list of valid range
             allow_blanks (bool): if True blank value (ie pd.nan) will be considered valid
 
         Returns:
             True if value is in one of the range
         """
 
-        if pd.isna(value):
+        if value in BLANK_VALUES:
             return allow_blanks
         for valid_range in valid_ranges:
             if valid_range.get('min') is not None:
                 if value < valid_range.get('min'):
                     continue
             if valid_range.get('max') is not None:
                 if value > valid_range.get('max'):
```

### Comparing `ods_tools-3.0.7/ods_tools/oed/setting_schema.py` & `ods_tools-3.1.0/ods_tools/oed/setting_schema.py`

 * *Files identical despite different names*

### Comparing `ods_tools-3.0.7/ods_tools/oed/source.py` & `ods_tools-3.1.0/ods_tools/oed/source.py`

 * *Files 9% similar despite different names*

```diff
@@ -2,15 +2,16 @@
 import mimetypes
 
 import logging
 import pandas as pd
 import numpy as np
 from chardet.universaldetector import UniversalDetector
 
-from .common import OED_TYPE_TO_NAME, OdsException, PANDAS_COMPRESSION_MAP, PANDAS_DEFAULT_NULL_VALUES, is_relative, BLANK_VALUES
+from .common import (OED_TYPE_TO_NAME, OdsException, PANDAS_COMPRESSION_MAP, PANDAS_DEFAULT_NULL_VALUES, is_relative, BLANK_VALUES, fill_empty,
+                     UnknownColumnSaveOption)
 from .forex import convert_currency
 from .oed_schema import OedSchema
 
 logger = logging.getLogger(__file__)
 
 try:
     from functools import cached_property
@@ -54,31 +55,30 @@
             value = obj.__dict__.get(self.__name__, _missing)
             if value is _missing:
                 value = self.func(obj)
                 obj.__dict__[self.__name__] = value
             return value
 
 
-def detect_encoding(filepath):
+def detect_encoding(fileobj):
     """
     Given a path to a CSV of unknown encoding
     read lines to detect its encoding type
 
     :param filepath: Filepath to check
     :type  filepath: str
 
     :return: Example `{'encoding': 'ISO-8859-1', 'confidence': 0.73, 'language': ''}`
     :rtype: dict
     """
     detector = UniversalDetector()
-    with open(filepath, 'rb') as f:
-        for line in f:
-            detector.feed(line)
-            if detector.done:
-                break
+    for line in fileobj:
+        detector.feed(line)
+        if detector.done:
+            break
     detector.close()
     return detector.result
 
 
 def detect_stream_type(stream_obj):
     """
     Given a file object try to inferr if its holding
@@ -273,28 +273,29 @@
 
         if not format:
             format = detect_stream_type(stream_obj)
 
         try:
             if format == 'csv':
                 oed_df = pd.read_csv(stream_obj, **read_param)
-                ods_fields = exposure.get_input_fields(oed_type)
-                column_to_field = OedSchema.column_to_field(oed_df.columns, ods_fields)
-                oed_df = cls.as_oed_type(oed_df, column_to_field)
-                oed_df = cls.prepare_df(oed_df, column_to_field, ods_fields)
-
-                if exposure.use_field:
-                    oed_df = OedSchema.use_field(oed_df, ods_fields)
             elif format == 'parquet':
                 oed_df = pd.read_parquet(stream_obj, **read_param)
             else:
                 raise OdsException(f'Unsupported stream format {format}')
         except Exception as e:
             raise OdsException('Failed to read stream data') from e
 
+        ods_fields = exposure.get_input_fields(oed_type)
+        column_to_field = OedSchema.column_to_field(oed_df.columns, ods_fields)
+        oed_df = cls.as_oed_type(oed_df, column_to_field)
+        oed_df = cls.prepare_df(oed_df, column_to_field, ods_fields)
+
+        if exposure.use_field:
+            oed_df = OedSchema.use_field(oed_df, ods_fields)
+
         oed_source.dataframe = oed_df
         oed_source.loaded = True
         if oed_df.empty:
             logger.info(f'{oed_source.oed_name} {oed_source} is empty')
         return oed_source
 
     @classmethod
@@ -304,15 +305,15 @@
         for column in oed_df.columns:
             if column in column_to_field:
                 pd_dtype[column] = column_to_field[column]['pd_dtype']
             else:
                 pd_dtype[column] = 'category'
             if pd_dtype[column] == 'category':  # we need to convert to str first
                 to_tmp_dtype[column] = 'str'
-                if oed_df[column].dtype.name == 'category':
+                if oed_df[column].dtype.name == 'category' and '' not in oed_df[column].dtype.categories:
                     oed_df[column] = oed_df[column].cat.add_categories('')
                 oed_df.loc[oed_df[column].isin(BLANK_VALUES), column] = ''
             elif pd_dtype[column].startswith('Int'):
                 to_tmp_dtype[column] = 'float'
 
         return oed_df.astype(to_tmp_dtype).astype(pd_dtype)
 
@@ -326,22 +327,20 @@
             ods_fields: the ods_field info for this oed source type
 
         Returns:
             df
         """
         # set default values
         for col, field_info in column_to_field.items():
-            field_info = column_to_field.get(col)
             if (field_info
                     and field_info['Default'] != 'n/a'
                     and (df[col].isna().any() or (field_info['pd_dtype'] == 'category' and df[col].isnull().any()))):
-                if field_info['pd_dtype'] == 'category':
-                    df[col] = df[col].cat.add_categories(field_info['Default']).fillna(field_info['Default'])
-                else:
-                    df[col].fillna(df[col].dtype.type(field_info['Default']), inplace=True)
+                fill_empty(df, col, df[col].dtype.type(field_info['Default']))
+            elif df[col].dtype.name == 'category':
+                fill_empty(df, col, '')
 
         # add required columns that allow blank values if missing
         present_field = set(field_info['Input Field Name'] for field_info in column_to_field.values())
         for field_info in ods_fields.values():
             col = field_info['Input Field Name']
             if col not in present_field:
                 if field_info.get('Required Field') == 'R' and field_info.get("Allow blanks?").upper() == "YES":
@@ -408,14 +407,19 @@
         if source['source_type'] == 'filepath':
             filepath = source['filepath']
             if is_relative(filepath):
                 filepath = Path(self.exposure.working_dir, filepath)
             extension = PANDAS_COMPRESSION_MAP.get(source.get('extention')) or Path(filepath).suffix
             if extension == '.parquet':
                 oed_df = pd.read_parquet(filepath, **source.get('read_param', {}))
+                ods_fields = self.exposure.get_input_fields(self.oed_type)
+                column_to_field = OedSchema.column_to_field(oed_df.columns, ods_fields)
+                oed_df = self.as_oed_type(oed_df, column_to_field)
+                oed_df = self.prepare_df(oed_df, column_to_field, ods_fields)
+
             else:  # default we assume it is csv like
                 read_params = {'keep_default_na': False,
                                'na_values': PANDAS_DEFAULT_NULL_VALUES.difference({'NA'})}
                 read_params.update(source.get('read_param', {}))
                 oed_df = self.read_csv(filepath, self.exposure.get_input_fields(self.oed_type), **read_params)
         else:
             raise Exception(f"Source type {source['source_type']} is not supported")
@@ -435,102 +439,139 @@
         if self.loaded:
             convert_currency(self.dataframe,
                              self.oed_type,
                              self.exposure.reporting_currency,
                              self.exposure.currency_conversion,
                              self.exposure.oed_schema)
 
-    def save(self, version_name, source):
+    def manage_unknown_columns(self, unknown_columns):
+        if unknown_columns == UnknownColumnSaveOption.IGNORE:
+            return self.dataframe
+        if not isinstance(unknown_columns, dict):
+            option_map = {}
+            default = unknown_columns
+        else:
+            option_map = unknown_columns
+            default = unknown_columns.get('default', UnknownColumnSaveOption.IGNORE)
+        rename = {}
+        drop = set()
+        for column in set(self.dataframe.columns).difference(self.get_column_to_field()):
+            option = option_map.get(column, default)
+            if option == UnknownColumnSaveOption.IGNORE:
+                continue
+            elif option == UnknownColumnSaveOption.RENAME:
+                rename[column] = f'Flexi{self.oed_type}{column}'
+            elif option == UnknownColumnSaveOption.DELETE:
+                drop.add(column)
+
+        return self.dataframe.rename(columns=rename).drop(columns=drop)
+
+    def save(self, version_name, source, unknown_columns=UnknownColumnSaveOption.IGNORE):
         """
         save dataframe as version_name in source
         Args:
             version_name (str): name of the version
             source: str or dict with information to save the dataframe
                 str : output path
                 dict : {'source_type': 'filepath' # only support for the moment
                         'extension': 'parquet' or all pandas supported extension
                         'write_param' : all args you may want to pass to the pandas writer function (to_parquet, to_csv)
-
+            unknown_columns (UnknownColumnSaveOption or Dict):  action to take for non OED column
         """
         if isinstance(source, (str, Path)):
             source = {'source_type': 'filepath',
                       'filepath': source,
                       }
         if source['source_type'] == 'filepath':
             filepath = source['filepath']
             if is_relative(filepath):
                 filepath = Path(self.exposure.working_dir, filepath)
             Path(filepath).parents[0].mkdir(parents=True, exist_ok=True)
             extension = source.get('extension') or ''.join(Path(filepath).suffixes)
+            dataframe = self.manage_unknown_columns(unknown_columns)
             if extension == 'parquet':
-                self.dataframe.to_parquet(filepath, **source.get('write_param', {}))
+                dataframe.to_parquet(filepath, **source.get('write_param', {}))
             else:
                 write_param = {'index': False}
                 write_param.update(source.get('write_param', {}))
-                self.dataframe.to_csv(filepath, **write_param)
+                dataframe.to_csv(filepath, **write_param)
         else:
             raise Exception(f"Source type {source['source_type']} is not supported")
         self.cur_version_name = version_name
         self.sources[version_name] = source
 
     @classmethod
-    def read_csv(cls, filepath, ods_fields, df_engine=pd, **kwargs):
+    def read_csv(cls, filepath_or_buffer, ods_fields, df_engine=pd, **kwargs):
         """
         the function read_csv will load a csv file as a DataFrame
         with all the columns converted to the correct dtype and having the correct default.
         it will also try to save space by converting string dtype into categories
         By default, it uses pandas to create the DataFrame. In that case you will need to have pandas installed.
         You can use other options such as Dask or modin using the parameter df_engine.
         Args:
-            filepath (str): path to the csv file
+            filepath_or_buffer (str, stream): str, path object or file-like object with seek method
+            ods_fields (dict): OED schema input field definition
             df_engine: engine that will convert csv to a dataframe object (default to pandas if installed)
             kwargs: extra argument that will be passed to the df_engine
         Returns:
             df_engine dataframe of the file with correct dtype and default
         Raises:
         """
+        if is_readable(filepath_or_buffer):
+            stream_start = filepath_or_buffer.tell()
+        else:
+            stream_start = None
 
-        def read_or_try_encoding_read(df_engine, filepath, **read_kwargs):
-            #  try to read, if fail try to detect the encoding and update the top function kwargs for future read
+        def read_or_try_encoding_read(df_engine, filepath_or_buffer, **read_kwargs):
+            #  try to read, if it fails, try to detect the encoding and update the top function kwargs for future read
             try:
-                return df_engine.read_csv(filepath, **kwargs)
+                return df_engine.read_csv(filepath_or_buffer, **read_kwargs)
             except UnicodeDecodeError as e:
-                detected_encoding = detect_encoding(filepath)['encoding']
+                if stream_start is None:
+                    with open(filepath_or_buffer, 'rb') as buffer:
+                        detected_encoding = detect_encoding(buffer)['encoding']
+                else:
+                    detected_encoding = detect_encoding(filepath_or_buffer)['encoding']
+                    filepath_or_buffer.seek(stream_start)
                 if not read_kwargs.get('encoding') and detected_encoding:
                     kwargs['encoding'] = detected_encoding
-                    read_kwargs.pop('encoding')
-                    return df_engine.read_csv(filepath, encoding=detected_encoding, **read_kwargs)
+                    read_kwargs.pop('encoding', None)
+                    return df_engine.read_csv(filepath_or_buffer, encoding=detected_encoding, **read_kwargs)
                 else:
                     raise
+            finally:
+                if stream_start is not None:
+                    filepath_or_buffer.seek(stream_start)
 
         if df_engine is None:
             raise Exception("df_engine parameter not specified, you must install pandas"
                             " or pass your DataFrame engine (modin, dask,...)")
 
-        if Path(filepath).suffix == '.gzip' or kwargs.get('compression') == 'gzip':
-            # support for gzip  https://stackoverflow.com/questions/60460814/pandas-read-csv-failing-on-gzipped-file-with-unicodedecodeerror-utf-8-codec-c
-            with open(filepath, 'rb') as f:
-                header = df_engine.read(f, compression='gzip', nrows=0, index_col=False,
-                                        encoding=kwargs.get('encoding')).columns
-            kwargs['compression'] = 'gzip'
+        header_read_arg = {**kwargs, 'nrows': 0, 'index_col': False}
+        if (stream_start is None
+                and Path(filepath_or_buffer).suffix == '.gzip' or header_read_arg.get('compression') == 'gzip'):
+            # support for gzip https://stackoverflow.com/questions/60460814/pandas-read-csv-failing-on-gzipped-file-with-unicodedecodeerror-utf-8-codec-c
+            with open(filepath_or_buffer, 'rb') as f:
+                header_read_arg['compression'] = kwargs['compression'] = 'gzip'
+                header = df_engine.read(f, **header_read_arg).columns
+
         else:
-            header = read_or_try_encoding_read(df_engine, filepath, nrows=0, index_col=False,
-                                               encoding=kwargs.get('encoding')).columns
+            header = read_or_try_encoding_read(df_engine, filepath_or_buffer, **header_read_arg).columns
 
         # match header column name to oed field name and prepare pd_dtype used to read the data
         pd_dtype = {}
         column_to_field = OedSchema.column_to_field(header, ods_fields)
         for col in header:
             if col in column_to_field:
                 field_info = column_to_field[col]
                 pd_dtype[col] = field_info['pd_dtype']
             else:
                 pd_dtype[col] = 'category'
 
         # read the oed file
         if kwargs.get('compression') == 'gzip':
-            with open(filepath, 'rb') as f:
+            with open(filepath_or_buffer, 'rb') as f:
                 df = df_engine.read_csv(f, dtype=pd_dtype, **kwargs)
         else:
-            df = df_engine.read_csv(filepath, dtype=pd_dtype, **kwargs)
+            df = df_engine.read_csv(filepath_or_buffer, dtype=pd_dtype, **kwargs)
 
         return cls.prepare_df(df, column_to_field, ods_fields)
```

### Comparing `ods_tools-3.0.7/ods_tools/oed/validator.py` & `ods_tools-3.1.0/ods_tools/oed/validator.py`

 * *Files 6% similar despite different names*

```diff
@@ -276,7 +276,51 @@
             invalid_country = (country_only_df[~country_only_df[country_code_column]
                                                .isin(set(self.exposure.oed_schema.schema['country']) | BLANK_VALUES)])
             if not invalid_country.empty:
                 invalid_data.append({'name': oed_source.oed_name, 'source': oed_source.current_source,
                                      'msg': f"invalid CountryCode.\n"
                                             f"{invalid_country[identifier_field + [country_code_column]]}"})
         return invalid_data
+
+    def check_conditional_requirement(self):
+        invalid_data = []
+        for oed_source in self.exposure.get_oed_sources():
+            cr_field = self.exposure.oed_schema.schema['cr_field'].get(oed_source.oed_type)
+            if not cr_field:
+                continue
+            column_to_field = self.column_to_field_maps[oed_source]
+            identifier_field = self.identifier_field_maps[oed_source]
+
+            def check_cr(rec):
+                cr_fields = set()
+                for col in column_to_field:
+                    field_info = column_to_field[col]
+                    if field_info['Input Field Name'] not in cr_field:
+                        continue
+
+                    if field_info['Default'] != 'n/a':
+                        if oed_source.dataframe[col].dtype.name == 'category':
+                            default_set = {field_info['Default']}
+                        else:
+                            default_set = {oed_source.dataframe[col].dtype.type(field_info['Default'])}
+                    else:
+                        default_set = set()
+
+                    if rec[col] not in BLANK_VALUES | default_set and rec[col]:
+                        cr_fields |= set(cr_field[field_info['Input Field Name']])
+                msg = []
+                for field in cr_fields:
+                    col = self.field_to_column_maps[oed_source].get(field)
+                    if col is None or rec[col] in BLANK_VALUES:
+                        msg.append(f'{self.field_to_column_maps[oed_source].get(field) or field}')
+
+                return ', '.join(msg)
+
+            cr_msg = oed_source.dataframe.apply(check_cr, axis=1)
+            missing_data_df = oed_source.dataframe[cr_msg != ''].copy()
+            if not missing_data_df.empty:
+                missing_data_df['missing value'] = cr_msg
+                invalid_data.append({'name': oed_source.oed_name, 'source': oed_source.current_source,
+                                     'msg': f"Conditionally required column missing .\n"
+                                            f"{missing_data_df[identifier_field + ['missing value']]}"})
+
+        return invalid_data
```

### Comparing `ods_tools-3.0.7/ods_tools.egg-info/PKG-INFO` & `ods_tools-3.1.0/ods_tools.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ods-tools
-Version: 3.0.7
+Version: 3.1.0
 Summary: Tools to manage ODS files
 Home-page: https://github.com/OasisLMF/OpenDataStandards
 Author: Oasis LMF
 Author-email: support@oasislmf.org
 License: UNKNOWN
 Platform: UNKNOWN
 Requires-Python: >=3.7
```

### Comparing `ods_tools-3.0.7/setup.py` & `ods_tools-3.1.0/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 
 import urllib.request
 import json
 
 
 SCRIPT_DIR = os.path.abspath(os.path.dirname(__file__))
 
-OED_VERSION = '3.0.3'
+OED_VERSION = '3.0.4'
 # ORD_VERSION =
 
 
 def get_readme():
     with io.open(os.path.join(SCRIPT_DIR, 'README.md'), encoding='utf-8') as readme:
         return readme.read()
 
@@ -101,15 +101,15 @@
     entry_points={
         'console_scripts': [
             'ods_tools=ods_tools.main:main',
         ]
     },
     author='Oasis LMF',
     author_email="support@oasislmf.org",
-    packages=['ods_tools', 'ods_tools.oed', 'ods_tools.data'],
+    packages=setuptools.find_packages(exclude=('tests', 'tests.*', 'tests.*.*')),
     package_dir={'ods_tools': 'ods_tools'},
     python_requires='>=3.7',
     install_requires=reqs,
     description='Tools to manage ODS files',
     long_description=readme,
     long_description_content_type='text/markdown',
     url='https://github.com/OasisLMF/OpenDataStandards',
```

