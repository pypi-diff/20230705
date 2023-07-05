# Comparing `tmp/isic-metadata-0.0.6.tar.gz` & `tmp/isic-metadata-0.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "isic-metadata-0.0.6.tar", last modified: Tue Jun 28 21:45:36 2022, max compression
+gzip compressed data, was "isic-metadata-0.0.7.tar", last modified: Wed Jul  5 15:56:44 2023, max compression
```

## Comparing `isic-metadata-0.0.6.tar` & `isic-metadata-0.0.7.tar`

### file list

```diff
@@ -1,29 +1,30 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-28 21:45:36.587044 isic-metadata-0.0.6/
--rw-r--r--   0 runner    (1001) docker     (121)      236 2022-06-28 21:45:12.000000 isic-metadata-0.0.6/.editorconfig
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-28 21:45:36.583044 isic-metadata-0.0.6/.github/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-28 21:45:36.587044 isic-metadata-0.0.6/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (121)      575 2022-06-28 21:45:12.000000 isic-metadata-0.0.6/.github/workflows/ci.yml
--rw-r--r--   0 runner    (1001) docker     (121)      674 2022-06-28 21:45:12.000000 isic-metadata-0.0.6/.github/workflows/release.yml
--rw-r--r--   0 runner    (1001) docker     (121)     1799 2022-06-28 21:45:12.000000 isic-metadata-0.0.6/.gitignore
--rw-r--r--   0 runner    (1001) docker     (121)    11357 2022-06-28 21:45:12.000000 isic-metadata-0.0.6/LICENSE
--rw-r--r--   0 runner    (1001) docker     (121)      939 2022-06-28 21:45:36.587044 isic-metadata-0.0.6/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      112 2022-06-28 21:45:12.000000 isic-metadata-0.0.6/README.md
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-28 21:45:36.587044 isic-metadata-0.0.6/isic_metadata/
--rw-r--r--   0 runner    (1001) docker     (121)     3994 2022-06-28 21:45:12.000000 isic-metadata-0.0.6/isic_metadata/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     9318 2022-06-28 21:45:12.000000 isic-metadata-0.0.6/isic_metadata/fields.py
--rw-r--r--   0 runner    (1001) docker     (121)     4999 2022-06-28 21:45:12.000000 isic-metadata-0.0.6/isic_metadata/metadata.py
--rw-r--r--   0 runner    (1001) docker     (121)      563 2022-06-28 21:45:12.000000 isic-metadata-0.0.6/isic_metadata/utils.py
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-06-28 21:45:12.000000 isic-metadata-0.0.6/isic_metadata/validators.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-28 21:45:36.587044 isic-metadata-0.0.6/isic_metadata.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)      939 2022-06-28 21:45:35.000000 isic-metadata-0.0.6/isic_metadata.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      481 2022-06-28 21:45:36.000000 isic-metadata-0.0.6/isic_metadata.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-06-28 21:45:36.000000 isic-metadata-0.0.6/isic_metadata.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)       16 2022-06-28 21:45:36.000000 isic-metadata-0.0.6/isic_metadata.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)       14 2022-06-28 21:45:36.000000 isic-metadata-0.0.6/isic_metadata.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (121)      582 2022-06-28 21:45:12.000000 isic-metadata-0.0.6/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (121)       38 2022-06-28 21:45:36.587044 isic-metadata-0.0.6/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)     1184 2022-06-28 21:45:12.000000 isic-metadata-0.0.6/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-28 21:45:36.587044 isic-metadata-0.0.6/tests/
--rw-r--r--   0 runner    (1001) docker     (121)     1401 2022-06-28 21:45:12.000000 isic-metadata-0.0.6/tests/test_fields.py
--rw-r--r--   0 runner    (1001) docker     (121)      540 2022-06-28 21:45:12.000000 isic-metadata-0.0.6/tests/test_utils.py
--rw-r--r--   0 runner    (1001) docker     (121)     1290 2022-06-28 21:45:12.000000 isic-metadata-0.0.6/tox.ini
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 15:56:44.250575 isic-metadata-0.0.7/
+-rw-r--r--   0 runner    (1001) docker     (123)      236 2023-07-05 15:56:19.000000 isic-metadata-0.0.7/.editorconfig
+-rw-r--r--   0 runner    (1001) docker     (123)       82 2023-07-05 15:56:19.000000 isic-metadata-0.0.7/.git-blame-ignore-revs
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 15:56:44.234575 isic-metadata-0.0.7/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 15:56:44.242575 isic-metadata-0.0.7/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)      575 2023-07-05 15:56:19.000000 isic-metadata-0.0.7/.github/workflows/ci.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      674 2023-07-05 15:56:19.000000 isic-metadata-0.0.7/.github/workflows/release.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1799 2023-07-05 15:56:19.000000 isic-metadata-0.0.7/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-07-05 15:56:19.000000 isic-metadata-0.0.7/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      939 2023-07-05 15:56:44.250575 isic-metadata-0.0.7/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      112 2023-07-05 15:56:19.000000 isic-metadata-0.0.7/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 15:56:44.246575 isic-metadata-0.0.7/isic_metadata/
+-rw-r--r--   0 runner    (1001) docker     (123)     3994 2023-07-05 15:56:19.000000 isic-metadata-0.0.7/isic_metadata/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9318 2023-07-05 15:56:19.000000 isic-metadata-0.0.7/isic_metadata/fields.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4997 2023-07-05 15:56:19.000000 isic-metadata-0.0.7/isic_metadata/metadata.py
+-rw-r--r--   0 runner    (1001) docker     (123)      563 2023-07-05 15:56:19.000000 isic-metadata-0.0.7/isic_metadata/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-05 15:56:19.000000 isic-metadata-0.0.7/isic_metadata/validators.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 15:56:44.246575 isic-metadata-0.0.7/isic_metadata.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      939 2023-07-05 15:56:44.000000 isic-metadata-0.0.7/isic_metadata.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      504 2023-07-05 15:56:44.000000 isic-metadata-0.0.7/isic_metadata.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-05 15:56:44.000000 isic-metadata-0.0.7/isic_metadata.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       18 2023-07-05 15:56:44.000000 isic-metadata-0.0.7/isic_metadata.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       14 2023-07-05 15:56:44.000000 isic-metadata-0.0.7/isic_metadata.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      549 2023-07-05 15:56:19.000000 isic-metadata-0.0.7/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-05 15:56:44.250575 isic-metadata-0.0.7/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1186 2023-07-05 15:56:19.000000 isic-metadata-0.0.7/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 15:56:44.246575 isic-metadata-0.0.7/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     1401 2023-07-05 15:56:19.000000 isic-metadata-0.0.7/tests/test_fields.py
+-rw-r--r--   0 runner    (1001) docker     (123)      540 2023-07-05 15:56:19.000000 isic-metadata-0.0.7/tests/test_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1272 2023-07-05 15:56:19.000000 isic-metadata-0.0.7/tox.ini
```

### Comparing `isic-metadata-0.0.6/.github/workflows/ci.yml` & `isic-metadata-0.0.7/.github/workflows/ci.yml`

 * *Files identical despite different names*

### Comparing `isic-metadata-0.0.6/.github/workflows/release.yml` & `isic-metadata-0.0.7/.github/workflows/release.yml`

 * *Files identical despite different names*

### Comparing `isic-metadata-0.0.6/.gitignore` & `isic-metadata-0.0.7/.gitignore`

 * *Files identical despite different names*

### Comparing `isic-metadata-0.0.6/LICENSE` & `isic-metadata-0.0.7/LICENSE`

 * *Files identical despite different names*

### Comparing `isic-metadata-0.0.6/PKG-INFO` & `isic-metadata-0.0.7/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: isic-metadata
-Version: 0.0.6
+Version: 0.0.7
 Home-page: https://github.com/ImageMarkup/isic-metadata
 Author: Kitware, Inc.
 Author-email: kitware@kitware.com
 License: Apache 2.0
 Project-URL: Bug Reports, https://github.com/ImageMarkup/isic-metadata/issues
 Project-URL: Source, https://github.com/ImageMarkup/isic-metadata
 Keywords: requests
```

### Comparing `isic-metadata-0.0.6/isic_metadata/__init__.py` & `isic-metadata-0.0.7/isic_metadata/__init__.py`

 * *Files 26% similar despite different names*

```diff
@@ -19,131 +19,131 @@
     MelType,
     NevusType,
     PatientId,
     Sex,
 )
 
 try:
-    __version__ = version('isic-metadata')
+    __version__ = version("isic-metadata")
 except PackageNotFoundError:
     # package is not installed
     pass
 
 
 FIELD_REGISTRY = {}
 
 for field in [
-    'blurry',
-    'hairy',
-    'marker_pen',
-    'personal_hx_mm',
-    'family_hx_mm',
-    'melanocytic',
-    'mel_ulcer',
+    "blurry",
+    "hairy",
+    "marker_pen",
+    "personal_hx_mm",
+    "family_hx_mm",
+    "melanocytic",
+    "mel_ulcer",
 ]:
     FIELD_REGISTRY[field] = {
-        'validator': bool,
-        'search': {
-            'key': field,
-            'es_property': {'type': 'boolean'},
-            'es_facet': {'terms': {'field': field}},
+        "validator": bool,
+        "search": {
+            "key": field,
+            "es_property": {"type": "boolean"},
+            "es_facet": {"terms": {"field": field}},
         },
     }
 
 
 for field, validator in [
-    ('sex', Sex),
-    ('benign_malignant', BenignMalignant),
-    ('diagnosis_confirm_type', DiagnosisConfirmType),
-    ('nevus_type', NevusType),
-    ('image_type', ImageType),
-    ('dermoscopic_type', DermoscopicType),
-    ('mel_type', MelType),
-    ('mel_class', MelClass),
-    ('mel_mitotic_index', MelMitoticIndex),
-    ('anatom_site_general', AnatomSiteGeneral),
-    ('color_tint', ColorTint),
-    ('patient_id', PatientId),
-    ('lesion_id', LesionId),
+    ("sex", Sex),
+    ("benign_malignant", BenignMalignant),
+    ("diagnosis_confirm_type", DiagnosisConfirmType),
+    ("nevus_type", NevusType),
+    ("image_type", ImageType),
+    ("dermoscopic_type", DermoscopicType),
+    ("mel_type", MelType),
+    ("mel_class", MelClass),
+    ("mel_mitotic_index", MelMitoticIndex),
+    ("anatom_site_general", AnatomSiteGeneral),
+    ("color_tint", ColorTint),
+    ("patient_id", PatientId),
+    ("lesion_id", LesionId),
 ]:
     FIELD_REGISTRY[field] = {
-        'validator': validator,
-        'search': {
-            'key': field,
-            'es_property': {'type': 'keyword'},
-            'es_facet': {'terms': {'field': field}},
+        "validator": validator,
+        "search": {
+            "key": field,
+            "es_property": {"type": "keyword"},
+            "es_facet": {"terms": {"field": field}},
         },
     }
 
 FIELD_REGISTRY.update(
     {
-        'clin_size_long_diam_mm': {
-            'validator': ClinSizeLongDiamMm,
-            'search': {
-                'key': 'clin_size_long_diam_mm',
-                'es_property': {'type': 'float'},
-                'es_facet': {
-                    'histogram': {
-                        'field': 'clin_size_long_diam_mm',
-                        'interval': 10,
-                        'extended_bounds': {'min': 0, 'max': 100},
+        "clin_size_long_diam_mm": {
+            "validator": ClinSizeLongDiamMm,
+            "search": {
+                "key": "clin_size_long_diam_mm",
+                "es_property": {"type": "float"},
+                "es_facet": {
+                    "histogram": {
+                        "field": "clin_size_long_diam_mm",
+                        "interval": 10,
+                        "extended_bounds": {"min": 0, "max": 100},
                     }
                 },
             },
         },
-        'acquisition_day': {
-            'validator': AcquisitionDay,
-            'search': False,
-        },
-        'diagnosis': {
-            'validator': Diagnosis,
-            'search': {
-                'key': 'diagnosis',
-                'es_property': {'type': 'keyword'},
-                'es_facet': {'terms': {'field': 'diagnosis', 'size': 100}},
+        "acquisition_day": {
+            "validator": AcquisitionDay,
+            "search": False,
+        },
+        "diagnosis": {
+            "validator": Diagnosis,
+            "search": {
+                "key": "diagnosis",
+                "es_property": {"type": "keyword"},
+                "es_facet": {"terms": {"field": "diagnosis", "size": 100}},
             },
         },
-        'mel_thick_mm': {
-            'validator': MelThickMm,
-            'search': {
-                'key': 'mel_thick_mm',
-                'es_property': {'type': 'float'},
-                'es_facet': {
-                    'range': {
-                        'field': 'mel_thick_mm',
-                        'ranges': [
-                            {'from': 0.0, 'to': 0.5},
-                            {'from': 0.5, 'to': 1.0},
-                            {'from': 1.0, 'to': 1.5},
-                            {'from': 1.5, 'to': 2.0},
-                            {'from': 2.0, 'to': 2.5},
-                            {'from': 2.5, 'to': 3.0},
-                            {'from': 3.0, 'to': 3.5},
-                            {'from': 3.5, 'to': 4.0},
-                            {'from': 4.0, 'to': 4.5},
-                            {'from': 4.5, 'to': 5.0},
-                            {'from': 5.0},
+        "mel_thick_mm": {
+            "validator": MelThickMm,
+            "search": {
+                "key": "mel_thick_mm",
+                "es_property": {"type": "float"},
+                "es_facet": {
+                    "range": {
+                        "field": "mel_thick_mm",
+                        "ranges": [
+                            {"from": 0.0, "to": 0.5},
+                            {"from": 0.5, "to": 1.0},
+                            {"from": 1.0, "to": 1.5},
+                            {"from": 1.5, "to": 2.0},
+                            {"from": 2.0, "to": 2.5},
+                            {"from": 2.5, "to": 3.0},
+                            {"from": 3.0, "to": 3.5},
+                            {"from": 3.5, "to": 4.0},
+                            {"from": 4.0, "to": 4.5},
+                            {"from": 4.5, "to": 5.0},
+                            {"from": 5.0},
                         ],
                     }
                 },
             },
         },
     }
 )
 
 for field in FIELD_REGISTRY.keys():
     if field in [
-        'blurry',
-        'color_tint',
-        'dermoscopic_type',
-        'hairy',
-        'image_type',
-        'marker_pen',
+        "blurry",
+        "color_tint",
+        "dermoscopic_type",
+        "hairy",
+        "image_type",
+        "marker_pen",
     ]:
-        FIELD_REGISTRY[field]['type'] = 'acquisition'
+        FIELD_REGISTRY[field]["type"] = "acquisition"
     else:
-        FIELD_REGISTRY[field]['type'] = 'clinical'
+        FIELD_REGISTRY[field]["type"] = "clinical"
 
 for field, label in [
-    ('anatom_site_general', 'Anatomic Site'),
+    ("anatom_site_general", "Anatomic Site"),
 ]:
-    FIELD_REGISTRY[field]['label'] = label
+    FIELD_REGISTRY[field]["label"] = label
```

### Comparing `isic-metadata-0.0.6/isic_metadata/fields.py` & `isic-metadata-0.0.7/isic_metadata/fields.py`

 * *Files 12% similar despite different names*

```diff
@@ -21,228 +21,228 @@
     def validate(cls, value) -> float | None:
         if not value:
             return None
 
         if isinstance(value, float):
             return value
 
-        match = re.match('(.+)(um|mm|cm)$', value)
+        match = re.match("(.+)(um|mm|cm)$", value)
 
         if not match:
-            raise ValueError(f'Invalid clinical size of {value}.')
+            raise ValueError(f"Invalid clinical size of {value}.")
 
         float_value, units = match.groups()
         float_value = float(float_value)
 
         if float_value <= 0:
-            raise ValueError(f'Invalid clinical size of {value}.')
+            raise ValueError(f"Invalid clinical size of {value}.")
 
         # Convert to mm
-        if units == 'um':
+        if units == "um":
             float_value *= 1e-3
-        elif units == 'cm':
+        elif units == "cm":
             float_value *= 1e1
 
         return round(float_value, ndigits=1)
 
 
 class Age(BaseStr):
     @classmethod
     def validate(cls, value: str | int) -> int | None:
         if not value:
             return None
-        elif value == '85+':
+        elif value == "85+":
             value = 85
         elif isinstance(value, str) and not value.isnumeric():
-            raise ValueError(f'Invalid age of {value}.')
+            raise ValueError(f"Invalid age of {value}.")
 
         value: int = int(value)
         # clip to 85
         value = min(value, 85)
         return value
 
 
 class Sex(BaseStr):
     @classmethod
     def validate(cls, value: str) -> str | None:
         if not value:
             return None
 
-        if value == 'm':
-            value = 'male'
-        elif value == 'f':
-            value = 'female'
+        if value == "m":
+            value = "male"
+        elif value == "f":
+            value = "female"
 
-        if value not in ['male', 'female']:
-            raise ValueError(f'Invalid sex of: {value}.')
+        if value not in ["male", "female"]:
+            raise ValueError(f"Invalid sex of: {value}.")
 
         return value
 
 
 class BenignMalignantEnum(str, Enum):
-    benign = 'benign'
-    malignant = 'malignant'
-    indeterminate = 'indeterminate'
-    indeterminate_benign = 'indeterminate/benign'
-    indeterminate_malignant = 'indeterminate/malignant'
+    benign = "benign"
+    malignant = "malignant"
+    indeterminate = "indeterminate"
+    indeterminate_benign = "indeterminate/benign"
+    indeterminate_malignant = "indeterminate/malignant"
 
 
 # todo indeterminable
 class BenignMalignant(BaseStr):
     @classmethod
     def validate(cls, value: str) -> str | None:
         if not value:
             return None
 
         if value not in BenignMalignantEnum._value2member_map_:
-            raise ValueError(f'Invalid benign/malignant value of {value}.')
+            raise ValueError(f"Invalid benign/malignant value of {value}.")
 
         return value
 
 
 class DiagnosisConfirmTypeEnum(str, Enum):
-    histopathology = 'histopathology'
-    serial_imaging_showing_no_change = 'serial imaging showing no change'
-    single_image_expert_consensus = 'single image expert consensus'
-    confocal_microscopy_with_consensus_dermoscopy = 'confocal microscopy with consensus dermoscopy'
+    histopathology = "histopathology"
+    serial_imaging_showing_no_change = "serial imaging showing no change"
+    single_image_expert_consensus = "single image expert consensus"
+    confocal_microscopy_with_consensus_dermoscopy = "confocal microscopy with consensus dermoscopy"
 
 
 class DiagnosisConfirmType(BaseStr):
     @classmethod
     def validate(cls, value: str) -> str | None:
         if value not in DiagnosisConfirmTypeEnum._value2member_map_:
-            raise ValueError(f'Invalid diagnosis confirm type of: {value}.')
+            raise ValueError(f"Invalid diagnosis confirm type of: {value}.")
         return value
 
 
 class DiagnosisEnum(str, Enum):
-    actinic_keratosis = 'actinic keratosis'
-    adnexal_tumor = 'adnexal tumor'
-    aimp = 'AIMP'
-    angiokeratoma = 'angiokeratoma'
-    angioma = 'angioma'
-    basal_cell_carcinoma = 'basal cell carcinoma'
-    cafe_au_lait_macule = 'cafe-au-lait macule'
-    dermatofibroma = 'dermatofibroma'
-    ephelis = 'ephelis'
-    lentigo_nos = 'lentigo NOS'
-    lentigo_simplex = 'lentigo simplex'
-    lichenoid_keratosis = 'lichenoid keratosis'
-    melanoma = 'melanoma'
-    melanoma_metastasis = 'melanoma metastasis'
-    merkel_cell_carcinoma = 'merkel cell carcinoma'
-    mucosal_melanosis = 'mucosal melanosis'
-    nevus = 'nevus'
-    nevus_spilus = 'nevus spilus'
-    seborrheic_keratosis = 'seborrheic keratosis'
-    solar_lentigo = 'solar lentigo'
-    squamous_cell_carcinoma = 'squamous cell carcinoma'
-    clear_cell_acanthoma = 'clear cell acanthoma'
-    atypical_spitz_tumor = 'atypical spitz tumor'
-    acrochordon = 'acrochordon'
-    angiofibroma_or_fibrous_papule = 'angiofibroma or fibrous papule'
-    neurofibroma = 'neurofibroma'
-    pyogenic_granuloma = 'pyogenic granuloma'
-    scar = 'scar'
-    sebaceous_adenoma = 'sebaceous adenoma'
-    sebaceous_hyperplasia = 'sebaceous hyperplasia'
-    verruca = 'verruca'
-    atypical_melanocytic_proliferation = 'atypical melanocytic proliferation'
-    epidermal_nevus = 'epidermal nevus'
-    pigmented_benign_keratosis = 'pigmented benign keratosis'
-    vascular_lesion = 'vascular lesion'
-    other = 'other'
+    actinic_keratosis = "actinic keratosis"
+    adnexal_tumor = "adnexal tumor"
+    aimp = "AIMP"
+    angiokeratoma = "angiokeratoma"
+    angioma = "angioma"
+    basal_cell_carcinoma = "basal cell carcinoma"
+    cafe_au_lait_macule = "cafe-au-lait macule"
+    dermatofibroma = "dermatofibroma"
+    ephelis = "ephelis"
+    lentigo_nos = "lentigo NOS"
+    lentigo_simplex = "lentigo simplex"
+    lichenoid_keratosis = "lichenoid keratosis"
+    melanoma = "melanoma"
+    melanoma_metastasis = "melanoma metastasis"
+    merkel_cell_carcinoma = "merkel cell carcinoma"
+    mucosal_melanosis = "mucosal melanosis"
+    nevus = "nevus"
+    nevus_spilus = "nevus spilus"
+    seborrheic_keratosis = "seborrheic keratosis"
+    solar_lentigo = "solar lentigo"
+    squamous_cell_carcinoma = "squamous cell carcinoma"
+    clear_cell_acanthoma = "clear cell acanthoma"
+    atypical_spitz_tumor = "atypical spitz tumor"
+    acrochordon = "acrochordon"
+    angiofibroma_or_fibrous_papule = "angiofibroma or fibrous papule"
+    neurofibroma = "neurofibroma"
+    pyogenic_granuloma = "pyogenic granuloma"
+    scar = "scar"
+    sebaceous_adenoma = "sebaceous adenoma"
+    sebaceous_hyperplasia = "sebaceous hyperplasia"
+    verruca = "verruca"
+    atypical_melanocytic_proliferation = "atypical melanocytic proliferation"
+    epidermal_nevus = "epidermal nevus"
+    pigmented_benign_keratosis = "pigmented benign keratosis"
+    vascular_lesion = "vascular lesion"
+    other = "other"
 
 
 class Diagnosis(BaseStr):
     @classmethod
     def validate(cls, value: str) -> str | None:
         if value not in DiagnosisEnum._value2member_map_:
-            raise ValueError(f'Invalid diagnosis of: {value}.')
+            raise ValueError(f"Invalid diagnosis of: {value}.")
         return value
 
 
 class NevusTypeEnum(str, Enum):
-    blue = 'blue'
-    combined = 'combined'
-    nevus_nos = 'nevus NOS'
-    deep_penetrating = 'deep penetrating'
-    halo = 'halo'
-    persistent_recurrent = 'persistent/recurrent'
-    pigmented_spindle_cell_of_reed = 'pigmented spindle cell of reed'
-    plexiform_spindle_cell = 'plexiform spindle cell'
-    special_site = 'special site'
-    spitz = 'spitz'
+    blue = "blue"
+    combined = "combined"
+    nevus_nos = "nevus NOS"
+    deep_penetrating = "deep penetrating"
+    halo = "halo"
+    persistent_recurrent = "persistent/recurrent"
+    pigmented_spindle_cell_of_reed = "pigmented spindle cell of reed"
+    plexiform_spindle_cell = "plexiform spindle cell"
+    special_site = "special site"
+    spitz = "spitz"
 
 
 class NevusType(BaseStr):
     @classmethod
     def validate(cls, value: str) -> str | None:
         if value not in NevusTypeEnum._value2member_map_:
-            raise ValueError(f'Invalid nevus type of: {value}.')
+            raise ValueError(f"Invalid nevus type of: {value}.")
         return value
 
 
 class ImageTypeEnum(str, Enum):
-    dermoscopic = 'dermoscopic'
-    clinical = 'clinical'
-    overview = 'overview'
+    dermoscopic = "dermoscopic"
+    clinical = "clinical"
+    overview = "overview"
 
 
 class ImageType(BaseStr):
     @classmethod
     def validate(cls, value: str) -> str | None:
         if value not in ImageTypeEnum._value2member_map_:
-            raise ValueError(f'Invalid image type of: {value}.')
+            raise ValueError(f"Invalid image type of: {value}.")
         return value
 
 
 class DermoscopicTypeEnum(str, Enum):
-    contact_polarized = 'contact polarized'
-    contact_non_polarized = 'contact non-polarized'
-    non_contact_polarized = 'non-contact polarized'
+    contact_polarized = "contact polarized"
+    contact_non_polarized = "contact non-polarized"
+    non_contact_polarized = "non-contact polarized"
 
 
 class DermoscopicType(BaseStr):
     @classmethod
     def validate(cls, value: str) -> str | None:
         if value not in DermoscopicTypeEnum._value2member_map_:
-            raise ValueError(f'Invalid dermoscopic type of: {value}.')
+            raise ValueError(f"Invalid dermoscopic type of: {value}.")
         return value
 
 
 class MelTypeEnum(str, Enum):
-    superficial_spreading_melanoma = 'superficial spreading melanoma'
-    nodular_melanoma = 'nodular melanoma'
-    lentigo_maligna_melanoma = 'lentigo maligna melanoma'
-    acral_lentiginous_melanoma = 'acral lentiginous melanoma'
-    melanoma_nos = 'melanoma NOS'
+    superficial_spreading_melanoma = "superficial spreading melanoma"
+    nodular_melanoma = "nodular melanoma"
+    lentigo_maligna_melanoma = "lentigo maligna melanoma"
+    acral_lentiginous_melanoma = "acral lentiginous melanoma"
+    melanoma_nos = "melanoma NOS"
 
 
 class MelType(BaseStr):
     @classmethod
     def validate(cls, value: str) -> str | None:
         if value not in MelTypeEnum._value2member_map_:
-            raise ValueError(f'Invalid mel type of: {value}.')
+            raise ValueError(f"Invalid mel type of: {value}.")
         return value
 
 
 class MelClassEnum(str, Enum):
-    melanoma_in_situ = 'melanoma in situ'
-    invasive_melanoma = 'invasive melanoma'
-    recurrent_persistent_melanoma_in_situ = 'recurrent/persistent melanoma, in situ'
-    recurrent_persistent_melanoma_invasive = 'recurrent/persistent melanoma, invasive'
-    melanoma_nos = 'melanoma NOS'
+    melanoma_in_situ = "melanoma in situ"
+    invasive_melanoma = "invasive melanoma"
+    recurrent_persistent_melanoma_in_situ = "recurrent/persistent melanoma, in situ"
+    recurrent_persistent_melanoma_invasive = "recurrent/persistent melanoma, invasive"
+    melanoma_nos = "melanoma NOS"
 
 
 class MelClass(BaseStr):
     @classmethod
     def validate(cls, value: str) -> str | None:
         if value not in MelClassEnum._value2member_map_:
-            raise ValueError(f'Invalid mel class of: {value}.')
+            raise ValueError(f"Invalid mel class of: {value}.")
         return value
 
 
 class MelThickMm(BaseStr):
     _regex = re.compile(
         r"""
         (.+?)    # Non-greedy
@@ -255,72 +255,72 @@
     @classmethod
     def validate(cls, value) -> float | None:
         if isinstance(value, float):
             return value
         # Parse value into floating point component and units
         result = re.match(cls._regex, value)
         if not result:
-            raise ValueError(f'Invalid melanoma thickness of: {value}.')
+            raise ValueError(f"Invalid melanoma thickness of: {value}.")
 
         value = result.group(1)
         int_value = float(value)
 
         return int_value
 
 
 class MelMitoticIndexEnum(str, Enum):
-    zero = '0/mm^2'
-    lt_one = '<1/mm^2'
-    one = '1/mm^2'
-    two = '2/mm^2'
-    three = '3/mm^2'
-    four = '4/mm^2'
-    gt_4 = '>4/mm^2'
+    zero = "0/mm^2"
+    lt_one = "<1/mm^2"
+    one = "1/mm^2"
+    two = "2/mm^2"
+    three = "3/mm^2"
+    four = "4/mm^2"
+    gt_4 = ">4/mm^2"
 
 
 class MelMitoticIndex(BaseStr):
     @classmethod
     def validate(cls, value: str) -> str | None:
         if value not in MelMitoticIndexEnum._value2member_map_:
-            raise ValueError(f'Invalid mel mitotic index of: {value}.')
+            raise ValueError(f"Invalid mel mitotic index of: {value}.")
         return value
 
 
 class AnatomSiteGeneralEnum(str, Enum):
-    head_neck = 'head/neck'
-    upper_extremity = 'upper extremity'
-    lower_extremity = 'lower extremity'
-    anterior_torso = 'anterior torso'
-    posterior_torso = 'posterior torso'
-    palms_soles = 'palms/soles'
-    lateral_torso = 'lateral torso'
-    oral_genital = 'oral/genital'
+    head_neck = "head/neck"
+    upper_extremity = "upper extremity"
+    lower_extremity = "lower extremity"
+    anterior_torso = "anterior torso"
+    posterior_torso = "posterior torso"
+    palms_soles = "palms/soles"
+    lateral_torso = "lateral torso"
+    oral_genital = "oral/genital"
 
 
 class AnatomSiteGeneral(BaseStr):
     @classmethod
     def validate(cls, value: str) -> str | None:
         if value not in AnatomSiteGeneralEnum._value2member_map_:
-            raise ValueError(f'Invalid general anatomical site of: {value}.')
+            raise ValueError(f"Invalid general anatomical site of: {value}.")
         return value
 
 
 class ColorTintEnum(str, Enum):
-    blue = 'blue'
-    pink = 'pink'
-    none = 'none'
+    blue = "blue"
+    pink = "pink"
+    none = "none"
 
 
 class ColorTint(BaseStr):
     @classmethod
     def validate(cls, value: str) -> str | None:
         if value not in ColorTintEnum._value2member_map_:
-            raise ValueError(f'Invalid color tint of: {value}.')
+            raise ValueError(f"Invalid color tint of: {value}.")
         return value
 
 
 class AcquisitionDay(int):
     pass
 
 
-PatientId = constr(regex=r'^IP_[0-9]{7}$')
-LesionId = constr(regex=r'^IL_[0-9]{7}$')
+PatientId = constr(regex=r"^IP_[0-9]{7}$")
+LesionId = constr(regex=r"^IL_[0-9]{7}$")
```

### Comparing `isic-metadata-0.0.6/isic_metadata/metadata.py` & `isic-metadata-0.0.7/isic_metadata/metadata.py`

 * *Files 6% similar despite different names*

```diff
@@ -57,100 +57,98 @@
 
     unstructured: Optional[dict]
 
     # See https://github.com/samuelcolvin/pydantic/issues/2285 for more detail
     @root_validator(pre=True)
     def build_extra(cls, values: dict[str, Any]) -> dict[str, Any]:  # noqa: N805
         all_required_field_names = {
-            field.alias for field in cls.__fields__.values() if field.alias != 'unstructured'
+            field.alias for field in cls.__fields__.values() if field.alias != "unstructured"
         }  # to support alias
 
         unstructured: dict[str, Any] = {}
         for field_name in list(values):
             if field_name not in all_required_field_names:
                 unstructured[field_name] = values.pop(field_name)
-        values['unstructured'] = unstructured
+        values["unstructured"] = unstructured
         return values
 
-    @validator('*', pre=True)
+    @validator("*", pre=True)
     @classmethod
     def strip(cls, v):
         if isinstance(v, str):
             v = v.strip()
         return v
 
     @validator(
-        'anatom_site_general',
-        'benign_malignant',
-        'clin_size_long_diam_mm',
-        'diagnosis_confirm_type',
-        'mel_mitotic_index',
-        'mel_thick_mm',
-        'sex',
+        "anatom_site_general",
+        "benign_malignant",
+        "clin_size_long_diam_mm",
+        "diagnosis_confirm_type",
+        "mel_mitotic_index",
+        "mel_thick_mm",
+        "sex",
         pre=True,
     )
     @classmethod
     def lower(cls, v):
         if isinstance(v, str):
             v = v.lower()
         return v
 
-    @validator('diagnosis')
+    @validator("diagnosis")
     @classmethod
     def validate_no_benign_melanoma(cls, v, values):
-        if 'benign_malignant' in values:
+        if "benign_malignant" in values:
+            if v == "melanoma" and values["benign_malignant"] == "benign":
+                raise ValueError("A benign melanoma cannot exist.")
 
-            if v == 'melanoma' and values['benign_malignant'] == 'benign':
-                raise ValueError('A benign melanoma cannot exist.')
-
-            if v == 'nevus' and values['benign_malignant'] not in [
+            if v == "nevus" and values["benign_malignant"] not in [
                 BenignMalignantEnum.benign,
                 BenignMalignantEnum.indeterminate_benign,
                 BenignMalignantEnum.indeterminate,
             ]:
                 raise ValueError(f'A {values["benign_malignant"]} nevus cannot exist.')
 
         return v
 
-    @validator('nevus_type')
+    @validator("nevus_type")
     @classmethod
     def validate_non_nevus_diagnoses(cls, v, values):
         if (
             v
-            and values.get('diagnosis')
-            and values['diagnosis'] not in [DiagnosisEnum.nevus, DiagnosisEnum.nevus_spilus]
+            and values.get("diagnosis")
+            and values["diagnosis"] not in [DiagnosisEnum.nevus, DiagnosisEnum.nevus_spilus]
         ):
             raise ValueError(f'Nevus type is inconsistent with {values["diagnosis"]}.')
         return v
 
-    @validator('mel_class', 'mel_mitotic_index', 'mel_thick_mm', 'mel_type', 'mel_ulcer')
+    @validator("mel_class", "mel_mitotic_index", "mel_thick_mm", "mel_type", "mel_ulcer")
     @classmethod
     def validate_melanoma_fields(cls, v, values, config, field):
-        if v and 'diagnosis' in values and values['diagnosis'] != 'melanoma':
-            raise ValueError(f'A non-melanoma {field} cannot exist.')
+        if v and "diagnosis" in values and values["diagnosis"] != "melanoma":
+            raise ValueError(f"A non-melanoma {field} cannot exist.")
         return v
 
-    @validator('diagnosis_confirm_type')
+    @validator("diagnosis_confirm_type")
     @classmethod
     def validate_non_histopathology_diagnoses(cls, v, values):
-        if 'diagnosis' not in values:
-            raise ValueError('Diagnosis confirm type requires a diagnosis.')
+        if "diagnosis" not in values:
+            raise ValueError("Diagnosis confirm type requires a diagnosis.")
 
-        if 'benign_malignant' in values:
-            if v != 'histopathology' and values['benign_malignant'] in [
+        if "benign_malignant" in values:
+            if v != "histopathology" and values["benign_malignant"] in [
                 BenignMalignantEnum.malignant,
                 BenignMalignantEnum.indeterminate_benign,
                 BenignMalignantEnum.indeterminate_malignant,
                 BenignMalignantEnum.indeterminate,
             ]:
-
                 raise ValueError(f'A {values["benign_malignant"]} ...')
 
         return v
 
-    @validator('dermoscopic_type')
+    @validator("dermoscopic_type")
     @classmethod
     def validate_dermoscopic_fields(cls, v, values):
-        if values.get('image_type') != ImageTypeEnum.dermoscopic and v:
-            image_type = values.get('image_type', 'none')
-            raise ValueError(f'Image type {image_type} inconsistent with dermoscopic type {v}.')
+        if values.get("image_type") != ImageTypeEnum.dermoscopic and v:
+            image_type = values.get("image_type", "none")
+            raise ValueError(f"Image type {image_type} inconsistent with dermoscopic type {v}.")
         return v
```

### Comparing `isic-metadata-0.0.6/isic_metadata/utils.py` & `isic-metadata-0.0.7/isic_metadata/utils.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from isic_metadata.metadata import MetadataRow
 
 
 def get_unstructured_columns(df):
     unstructured_columns = set()
-    structured_columns = set(MetadataRow.__fields__.keys()) - {'unstructured'}
+    structured_columns = set(MetadataRow.__fields__.keys()) - {"unstructured"}
 
     for _, (_, row) in enumerate(df.iterrows(), start=2):
         unstructured_columns |= set(row.keys()) - structured_columns
 
     # unstructured columns are any columns that aren't part of the core
     # columns (filename, isic_id) and aren't defined in MetadataRow
-    unstructured_columns -= {'filename', 'isic_id'}
+    unstructured_columns -= {"filename", "isic_id"}
 
     return sorted(list(unstructured_columns))
```

### Comparing `isic-metadata-0.0.6/isic_metadata.egg-info/PKG-INFO` & `isic-metadata-0.0.7/isic_metadata.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: isic-metadata
-Version: 0.0.6
+Version: 0.0.7
 Home-page: https://github.com/ImageMarkup/isic-metadata
 Author: Kitware, Inc.
 Author-email: kitware@kitware.com
 License: Apache 2.0
 Project-URL: Bug Reports, https://github.com/ImageMarkup/isic-metadata/issues
 Project-URL: Source, https://github.com/ImageMarkup/isic-metadata
 Keywords: requests
```

### Comparing `isic-metadata-0.0.6/pyproject.toml` & `isic-metadata-0.0.7/pyproject.toml`

 * *Files 7% similar despite different names*

```diff
@@ -2,15 +2,14 @@
 requires = ["setuptools >= 42", "wheel", "setuptools-scm[toml]>=3.4"]
 build-backend = "setuptools.build_meta"
 
 [tool.setuptools_scm]
 
 [tool.black]
 line-length = 100
-skip-string-normalization = true
 target-version = ["py38"]
 exclude='\.eggs|\.git|\.mypy_cache|\.tox|\.venv|_build|buck-out|build|dist'
 
 [tool.isort]
 profile = "black"
 line_length = 100
 # Sort by name, don't cluster "from" vs "import"
```

### Comparing `isic-metadata-0.0.6/tests/test_fields.py` & `isic-metadata-0.0.7/tests/test_fields.py`

 * *Files 7% similar despite different names*

```diff
@@ -3,42 +3,42 @@
 
 from isic_metadata.metadata import MetadataRow
 
 
 def test_melanoma_fields():
     try:
         # mel_class can only be set if diagnosis is melanoma
-        MetadataRow(diagnosis='angioma', mel_class='invasive melanoma')
+        MetadataRow(diagnosis="angioma", mel_class="invasive melanoma")
     except ValidationError as e:
         assert len(e.errors()) == 1
-        assert e.errors()[0]['loc'][0] == 'mel_class'
+        assert e.errors()[0]["loc"][0] == "mel_class"
 
     # mel_class can only be set if diagnosis is melanoma
-    MetadataRow(diagnosis='melanoma', mel_class='invasive melanoma')
+    MetadataRow(diagnosis="melanoma", mel_class="invasive melanoma")
 
 
 def test_no_benign_melanoma():
     try:
-        MetadataRow(diagnosis='melanoma', benign_malignant='benign')
+        MetadataRow(diagnosis="melanoma", benign_malignant="benign")
     except ValidationError as e:
         assert len(e.errors()) == 1
-        assert e.errors()[0]['loc'][0] == 'diagnosis'
+        assert e.errors()[0]["loc"][0] == "diagnosis"
 
 
 @given(age=st.integers(min_value=0).map(str))
 def test_age_ceiling(age):
     assert MetadataRow(age=age).age <= 85
 
 
 def test_age_special_case():
-    assert MetadataRow(age='85+').age == 85
+    assert MetadataRow(age="85+").age == 85
 
 
 @given(
     clin_size=st.one_of(st.floats(min_value=0, exclude_min=True), st.integers(min_value=1)).map(
-        lambda x: f'{x} mm'
+        lambda x: f"{x} mm"
     )
 )
 def test_clin_size_long_diam_mm_always_rounded(clin_size):
     metadata = MetadataRow(clin_size_long_diam_mm=clin_size)
     assert isinstance(metadata.clin_size_long_diam_mm, float)
     assert metadata.clin_size_long_diam_mm == round(metadata.clin_size_long_diam_mm, ndigits=1)
```

### Comparing `isic-metadata-0.0.6/tests/test_utils.py` & `isic-metadata-0.0.7/tests/test_utils.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 import pandas as pd
 
 from isic_metadata.utils import get_unstructured_columns
 
 
 def test_get_unstructured_columns():
-    data = [{'age': 25, 'foo': 'bar'}, {'age': 25}, {'age': 25, 'foo': 'bar'}]
+    data = [{"age": 25, "foo": "bar"}, {"age": 25}, {"age": 25, "foo": "bar"}]
 
     df = pd.DataFrame.from_records(data)
 
-    assert get_unstructured_columns(df) == ['foo']
+    assert get_unstructured_columns(df) == ["foo"]
 
 
 def test_get_unstructured_columns_ignore_filename():
-    data = [{'age': 25, 'foo': 'bar', 'filename': 'foobar'}, {'age': 25}, {'age': 25, 'foo': 'bar'}]
+    data = [{"age": 25, "foo": "bar", "filename": "foobar"}, {"age": 25}, {"age": 25, "foo": "bar"}]
 
     df = pd.DataFrame.from_records(data)
 
-    assert get_unstructured_columns(df) == ['foo']
+    assert get_unstructured_columns(df) == ["foo"]
```

### Comparing `isic-metadata-0.0.6/tox.ini` & `isic-metadata-0.0.7/tox.ini`

 * *Files 1% similar despite different names*

```diff
@@ -10,15 +10,14 @@
 skip_install = true
 deps =
     flake8
     flake8-black
     flake8-bugbear
     flake8-docstrings
     flake8-isort
-    flake8-quotes
     pep8-naming
 commands =
     flake8 {posargs:.}
 
 [testenv:test]
 deps =
     hypothesis
```

