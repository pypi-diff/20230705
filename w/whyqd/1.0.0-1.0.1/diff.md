# Comparing `tmp/whyqd-1.0.0.tar.gz` & `tmp/whyqd-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "whyqd-1.0.0.tar", max compression
+gzip compressed data, was "whyqd-1.0.1.tar", max compression
```

## Comparing `whyqd-1.0.0.tar` & `whyqd-1.0.1.tar`

### file list

```diff
@@ -1,95 +1,95 @@
--rwxr-xr-x   0        0        0     1543 2020-02-03 11:45:00.076853 whyqd-1.0.0/LICENSE
--rwxr-xr-x   0        0        0     7711 2023-05-10 14:13:08.437398 whyqd-1.0.0/README.md
--rwxr-xr-x   0        0        0     1737 2023-05-10 14:13:08.488398 whyqd-1.0.0/pyproject.toml
--rwxr-xr-x   0        0        0    23800 2023-05-10 14:13:08.619398 whyqd-1.0.0/tests/data/2023-05-09-human-development-report-interim.PARQUET
--rwxr-xr-x   0        0        0    40526 2021-08-23 16:43:27.488340 whyqd-1.0.0/tests/data/HDR-2007-2008-Table-03.xlsx
--rwxr-xr-x   0        0        0   242453 2020-02-12 10:37:10.119769 whyqd-1.0.0/tests/data/raw_E06000044_014_0.XLSX
--rwxr-xr-x   0        0        0     1422 2023-05-10 14:13:08.621402 whyqd-1.0.0/tests/data/raw_E06000044_014_0.data
--rwxr-xr-x   0        0        0    38885 2020-02-12 10:37:08.070860 whyqd-1.0.0/tests/data/raw_E06000044_014_1.XLSX
--rwxr-xr-x   0        0        0   306675 2020-02-12 10:37:12.460459 whyqd-1.0.0/tests/data/raw_E06000044_014_2.XLSX
--rwxr-xr-x   0        0        0   330970 2023-05-10 14:13:08.625396 whyqd-1.0.0/tests/data/raw_duplicated_E06000044_014.xlsx
--rwxr-xr-x   0        0        0   508171 2023-05-10 14:13:08.631399 whyqd-1.0.0/tests/data/raw_multi_E06000044_014.xlsx
--rwxr-xr-x   0        0        0   246405 2023-02-14 09:10:52.024386 whyqd-1.0.0/tests/data/restructured_test_data.xlsx
--rwxr-xr-x   0        0        0     4229 2023-05-10 14:13:08.631399 whyqd-1.0.0/tests/data/test_crosswalk.crosswalk
--rwxr-xr-x   0        0        0     1435 2023-05-10 14:13:08.632398 whyqd-1.0.0/tests/data/test_cthulu_destination.schema
--rwxr-xr-x   0        0        0     3144 2023-05-10 14:13:08.633398 whyqd-1.0.0/tests/data/test_cthulu_interim.data
--rwxr-xr-x   0        0        0     3022 2023-05-10 14:13:08.633398 whyqd-1.0.0/tests/data/test_cthulu_interim.schema
--rwxr-xr-x   0        0        0     2538 2023-05-10 14:13:08.634397 whyqd-1.0.0/tests/data/test_cthulu_source.data
--rwxr-xr-x   0        0        0     2606 2023-05-10 14:13:08.635398 whyqd-1.0.0/tests/data/test_cthulu_source.schema
--rwxr-xr-x   0        0        0   582612 2023-05-10 14:13:08.640397 whyqd-1.0.0/tests/data/test_data.csv
--rwxr-xr-x   0        0        0     1159 2023-05-10 14:13:08.641397 whyqd-1.0.0/tests/data/test_derived_schema.schema
--rwxr-xr-x   0        0        0     2529 2023-05-10 14:13:08.642398 whyqd-1.0.0/tests/data/test_portsmouth_destination.schema
--rwxr-xr-x   0        0        0     1234 2023-05-10 14:13:08.643397 whyqd-1.0.0/tests/data/test_portsmouth_source.data
--rwxr-xr-x   0        0        0     1978 2023-05-10 14:13:08.643397 whyqd-1.0.0/tests/data/test_portsmouth_source.schema
--rwxr-xr-x   0        0        0     1943 2021-08-23 16:43:27.501347 whyqd-1.0.0/tests/data/test_schema.json
--rwxr-xr-x   0        0        0     2529 2023-05-10 14:13:08.644397 whyqd-1.0.0/tests/data/test_schema.schema
--rwxr-xr-x   0        0        0     1986 2023-05-10 14:13:08.645397 whyqd-1.0.0/tests/data/test_source_schema.schema
--rwxr-xr-x   0        0        0     1728 2021-08-23 16:43:27.501347 whyqd-1.0.0/tests/data/urban_population.json
--rwxr-xr-x   0        0        0   505134 2023-02-14 09:10:52.029354 whyqd-1.0.0/tests/data/working_test_data.xlsx
--rwxr-xr-x   0        0        0   153076 2020-05-03 21:13:05.504203 whyqd-1.0.0/tests/data/working_test_world_bank_data.xlsx
--rwxr-xr-x   0        0        0      165 2023-05-10 14:13:08.646397 whyqd-1.0.0/tests/data/~$HDR-2007-2008-Table-03.xlsx
--rwxr-xr-x   0        0        0        5 2023-05-10 14:13:08.654397 whyqd-1.0.0/whyqd/VERSION
--rwxr-xr-x   0        0        0      315 2023-05-10 14:13:08.655398 whyqd-1.0.0/whyqd/__init__.py
--rwxr-xr-x   0        0        0      214 2021-08-23 16:43:27.509335 whyqd-1.0.0/whyqd/__main__.py
--rwxr-xr-x   0        0        0        0 2023-02-14 09:10:52.048356 whyqd-1.0.0/whyqd/config/__init__.py
--rwxr-xr-x   0        0        0     2607 2023-05-10 14:13:08.656397 whyqd-1.0.0/whyqd/config/ray_init.py
--rwxr-xr-x   0        0        0      520 2023-05-10 14:13:08.657397 whyqd-1.0.0/whyqd/config/settings.py
--rwxr-xr-x   0        0        0      172 2023-05-10 14:13:08.657397 whyqd-1.0.0/whyqd/core/__init__.py
--rwxr-xr-x   0        0        0     8358 2023-05-10 14:13:08.658398 whyqd-1.0.0/whyqd/core/base.py
--rwxr-xr-x   0        0        0     6065 2023-05-10 14:13:08.659397 whyqd-1.0.0/whyqd/core/crosswalk.py
--rwxr-xr-x   0        0        0    11122 2023-05-10 14:13:08.660397 whyqd-1.0.0/whyqd/core/datasource.py
--rwxr-xr-x   0        0        0     3859 2023-05-10 14:13:08.660397 whyqd-1.0.0/whyqd/core/schema.py
--rwxr-xr-x   0        0        0    12113 2023-05-10 14:13:08.661397 whyqd-1.0.0/whyqd/core/transform.py
--rwxr-xr-x   0        0        0        0 2023-05-10 14:13:08.662396 whyqd-1.0.0/whyqd/crosswalk/__init__.py
--rwxr-xr-x   0        0        0     1537 2023-05-10 14:13:08.662396 whyqd-1.0.0/whyqd/crosswalk/actions/__init__.py
--rwxr-xr-x   0        0        0     2934 2023-05-10 14:13:08.663396 whyqd-1.0.0/whyqd/crosswalk/actions/calculate.py
--rwxr-xr-x   0        0        0     1507 2023-05-10 14:13:08.664396 whyqd-1.0.0/whyqd/crosswalk/actions/categorise.py
--rwxr-xr-x   0        0        0     1090 2023-05-10 14:13:08.664396 whyqd-1.0.0/whyqd/crosswalk/actions/deblank.py
--rwxr-xr-x   0        0        0      975 2023-05-10 14:13:08.665396 whyqd-1.0.0/whyqd/crosswalk/actions/dedupe.py
--rwxr-xr-x   0        0        0     1249 2023-05-10 14:13:08.665396 whyqd-1.0.0/whyqd/crosswalk/actions/delete_rows.py
--rwxr-xr-x   0        0        0     1538 2023-05-10 14:13:08.666397 whyqd-1.0.0/whyqd/crosswalk/actions/new.py
--rwxr-xr-x   0        0        0     4021 2023-05-10 14:13:08.667401 whyqd-1.0.0/whyqd/crosswalk/actions/pivot_categories.py
--rwxr-xr-x   0        0        0     1893 2023-05-10 14:13:08.667401 whyqd-1.0.0/whyqd/crosswalk/actions/pivot_longer.py
--rwxr-xr-x   0        0        0     1535 2023-05-10 14:13:08.668401 whyqd-1.0.0/whyqd/crosswalk/actions/rename.py
--rwxr-xr-x   0        0        0     2200 2023-05-10 14:13:08.669397 whyqd-1.0.0/whyqd/crosswalk/actions/select.py
--rwxr-xr-x   0        0        0     3832 2023-05-10 14:13:08.669397 whyqd-1.0.0/whyqd/crosswalk/actions/select_newest.py
--rwxr-xr-x   0        0        0     3826 2023-05-10 14:13:08.670396 whyqd-1.0.0/whyqd/crosswalk/actions/select_oldest.py
--rwxr-xr-x   0        0        0     3418 2023-05-10 14:13:08.671399 whyqd-1.0.0/whyqd/crosswalk/actions/separate.py
--rwxr-xr-x   0        0        0     2105 2023-05-10 14:13:08.672397 whyqd-1.0.0/whyqd/crosswalk/actions/unite.py
--rwxr-xr-x   0        0        0      131 2023-05-10 14:13:08.673398 whyqd-1.0.0/whyqd/crosswalk/base/__init__.py
--rwxr-xr-x   0        0        0     6247 2023-05-10 14:13:08.674398 whyqd-1.0.0/whyqd/crosswalk/base/action_base.py
--rwxr-xr-x   0        0        0     8242 2023-05-10 14:13:08.675397 whyqd-1.0.0/whyqd/crosswalk/base/category_base.py
--rwxr-xr-x   0        0        0     3940 2023-05-10 14:13:08.675397 whyqd-1.0.0/whyqd/crosswalk/base/morph_base.py
--rwxr-xr-x   0        0        0      258 2023-05-10 14:13:08.676397 whyqd-1.0.0/whyqd/crud/__init__.py
--rwxr-xr-x   0        0        0    12397 2023-05-10 14:13:08.677395 whyqd-1.0.0/whyqd/crud/action.py
--rwxr-xr-x   0        0        0     4873 2023-05-10 14:13:08.677395 whyqd-1.0.0/whyqd/crud/base.py
--rwxr-xr-x   0        0        0     7877 2023-05-10 14:13:08.678409 whyqd-1.0.0/whyqd/crud/field.py
--rwxr-xr-x   0        0        0       88 2023-05-10 14:13:08.679396 whyqd-1.0.0/whyqd/dtypes/__init__.py
--rwxr-xr-x   0        0        0     1928 2023-05-10 14:13:08.679396 whyqd-1.0.0/whyqd/dtypes/field.py
--rwxr-xr-x   0        0        0      900 2023-05-10 14:13:08.680396 whyqd-1.0.0/whyqd/dtypes/mime.py
--rwxr-xr-x   0        0        0     1294 2023-05-10 14:13:08.680396 whyqd-1.0.0/whyqd/dtypes/status.py
--rwxr-xr-x   0        0        0      617 2023-05-10 14:13:08.681397 whyqd-1.0.0/whyqd/models/__init__.py
--rwxr-xr-x   0        0        0     1077 2023-05-10 14:13:08.681397 whyqd-1.0.0/whyqd/models/action_category.py
--rwxr-xr-x   0        0        0     1086 2023-05-10 14:13:08.682397 whyqd-1.0.0/whyqd/models/action_morph.py
--rwxr-xr-x   0        0        0     1665 2023-05-10 14:13:08.682397 whyqd-1.0.0/whyqd/models/action_schema.py
--rwxr-xr-x   0        0        0      530 2023-05-10 14:13:08.683396 whyqd-1.0.0/whyqd/models/actionscript.py
--rwxr-xr-x   0        0        0      584 2023-05-10 14:13:08.683396 whyqd-1.0.0/whyqd/models/category.py
--rwxr-xr-x   0        0        0     2569 2023-05-10 14:13:08.684399 whyqd-1.0.0/whyqd/models/citation.py
--rwxr-xr-x   0        0        0     1366 2023-05-10 14:13:08.684399 whyqd-1.0.0/whyqd/models/column.py
--rwxr-xr-x   0        0        0     2162 2023-05-10 14:13:08.685395 whyqd-1.0.0/whyqd/models/constraints.py
--rwxr-xr-x   0        0        0     1977 2023-05-10 14:13:08.685395 whyqd-1.0.0/whyqd/models/crosswalk.py
--rwxr-xr-x   0        0        0     4358 2023-05-10 14:13:08.686398 whyqd-1.0.0/whyqd/models/datasource.py
--rwxr-xr-x   0        0        0     1367 2023-05-10 14:13:08.687398 whyqd-1.0.0/whyqd/models/fields.py
--rwxr-xr-x   0        0        0      608 2023-05-10 14:13:08.688398 whyqd-1.0.0/whyqd/models/modifier.py
--rwxr-xr-x   0        0        0     2650 2023-05-10 14:13:08.688398 whyqd-1.0.0/whyqd/models/schema.py
--rwxr-xr-x   0        0        0     2046 2023-05-10 14:13:08.690396 whyqd-1.0.0/whyqd/models/transform.py
--rwxr-xr-x   0        0        0      527 2023-05-10 14:13:08.690396 whyqd-1.0.0/whyqd/models/version.py
--rwxr-xr-x   0        0        0      210 2023-05-10 14:13:08.691396 whyqd-1.0.0/whyqd/parsers/__init__.py
--rwxr-xr-x   0        0        0    14750 2023-05-10 14:13:08.692394 whyqd-1.0.0/whyqd/parsers/action.py
--rwxr-xr-x   0        0        0    10614 2023-05-10 14:13:08.692394 whyqd-1.0.0/whyqd/parsers/category.py
--rwxr-xr-x   0        0        0     9192 2023-05-10 14:13:08.693398 whyqd-1.0.0/whyqd/parsers/core.py
--rwxr-xr-x   0        0        0    30850 2023-05-10 14:13:08.694397 whyqd-1.0.0/whyqd/parsers/datasource.py
--rwxr-xr-x   0        0        0     9021 2023-05-10 14:13:08.694397 whyqd-1.0.0/whyqd/parsers/morph.py
--rwxr-xr-x   0        0        0     6789 2023-05-10 14:13:08.695395 whyqd-1.0.0/whyqd/parsers/script.py
--rw-r--r--   0        0        0     8892 1970-01-01 00:00:00.000000 whyqd-1.0.0/setup.py
--rw-r--r--   0        0        0     9200 1970-01-01 00:00:00.000000 whyqd-1.0.0/PKG-INFO
+-rwxr-xr-x   0        0        0     1543 2020-02-03 11:45:00.076853 whyqd-1.0.1/LICENSE
+-rwxr-xr-x   0        0        0     7853 2023-05-12 07:06:44.670906 whyqd-1.0.1/README.md
+-rwxr-xr-x   0        0        0     1737 2023-07-05 15:25:45.044584 whyqd-1.0.1/pyproject.toml
+-rwxr-xr-x   0        0        0    23800 2023-05-10 14:13:08.619398 whyqd-1.0.1/tests/data/2023-05-09-human-development-report-interim.PARQUET
+-rwxr-xr-x   0        0        0    40526 2021-08-23 16:43:27.488340 whyqd-1.0.1/tests/data/HDR-2007-2008-Table-03.xlsx
+-rwxr-xr-x   0        0        0   242453 2020-02-12 10:37:10.119769 whyqd-1.0.1/tests/data/raw_E06000044_014_0.XLSX
+-rwxr-xr-x   0        0        0     1422 2023-05-10 14:13:08.621402 whyqd-1.0.1/tests/data/raw_E06000044_014_0.data
+-rwxr-xr-x   0        0        0    38885 2020-02-12 10:37:08.070860 whyqd-1.0.1/tests/data/raw_E06000044_014_1.XLSX
+-rwxr-xr-x   0        0        0   306675 2020-02-12 10:37:12.460459 whyqd-1.0.1/tests/data/raw_E06000044_014_2.XLSX
+-rwxr-xr-x   0        0        0   330970 2023-05-10 14:13:08.625396 whyqd-1.0.1/tests/data/raw_duplicated_E06000044_014.xlsx
+-rwxr-xr-x   0        0        0   508171 2023-05-10 14:13:08.631399 whyqd-1.0.1/tests/data/raw_multi_E06000044_014.xlsx
+-rwxr-xr-x   0        0        0   246405 2023-02-14 09:10:52.024386 whyqd-1.0.1/tests/data/restructured_test_data.xlsx
+-rwxr-xr-x   0        0        0     4229 2023-05-10 14:13:08.631399 whyqd-1.0.1/tests/data/test_crosswalk.crosswalk
+-rwxr-xr-x   0        0        0     1435 2023-05-19 09:38:36.782172 whyqd-1.0.1/tests/data/test_cthulu_destination.schema
+-rwxr-xr-x   0        0        0     3144 2023-05-19 09:38:38.269033 whyqd-1.0.1/tests/data/test_cthulu_interim.data
+-rwxr-xr-x   0        0        0     3022 2023-05-19 09:38:39.967455 whyqd-1.0.1/tests/data/test_cthulu_interim.schema
+-rwxr-xr-x   0        0        0     2538 2023-05-19 09:38:41.929747 whyqd-1.0.1/tests/data/test_cthulu_source.data
+-rwxr-xr-x   0        0        0     2606 2023-05-19 09:38:44.186689 whyqd-1.0.1/tests/data/test_cthulu_source.schema
+-rwxr-xr-x   0        0        0   582612 2023-05-10 14:13:08.640397 whyqd-1.0.1/tests/data/test_data.csv
+-rwxr-xr-x   0        0        0     1159 2023-05-10 14:13:08.641397 whyqd-1.0.1/tests/data/test_derived_schema.schema
+-rwxr-xr-x   0        0        0     2529 2023-05-10 14:13:08.642398 whyqd-1.0.1/tests/data/test_portsmouth_destination.schema
+-rwxr-xr-x   0        0        0     1234 2023-05-10 14:13:08.643397 whyqd-1.0.1/tests/data/test_portsmouth_source.data
+-rwxr-xr-x   0        0        0     1978 2023-05-10 14:13:08.643397 whyqd-1.0.1/tests/data/test_portsmouth_source.schema
+-rwxr-xr-x   0        0        0     1943 2021-08-23 16:43:27.501347 whyqd-1.0.1/tests/data/test_schema.json
+-rwxr-xr-x   0        0        0     2529 2023-05-10 14:13:08.644397 whyqd-1.0.1/tests/data/test_schema.schema
+-rwxr-xr-x   0        0        0     1986 2023-05-10 14:13:08.645397 whyqd-1.0.1/tests/data/test_source_schema.schema
+-rwxr-xr-x   0        0        0     1728 2021-08-23 16:43:27.501347 whyqd-1.0.1/tests/data/urban_population.json
+-rwxr-xr-x   0        0        0   505134 2023-02-14 09:10:52.029354 whyqd-1.0.1/tests/data/working_test_data.xlsx
+-rwxr-xr-x   0        0        0   153076 2020-05-03 21:13:05.504203 whyqd-1.0.1/tests/data/working_test_world_bank_data.xlsx
+-rwxr-xr-x   0        0        0      165 2023-06-06 14:19:33.611783 whyqd-1.0.1/tests/data/~$HDR-2007-2008-Table-03.xlsx
+-rwxr-xr-x   0        0        0        5 2023-07-05 15:25:04.796251 whyqd-1.0.1/whyqd/VERSION
+-rwxr-xr-x   0        0        0      315 2023-05-10 14:13:08.655398 whyqd-1.0.1/whyqd/__init__.py
+-rwxr-xr-x   0        0        0      214 2021-08-23 16:43:27.509335 whyqd-1.0.1/whyqd/__main__.py
+-rwxr-xr-x   0        0        0        0 2023-02-14 09:10:52.048356 whyqd-1.0.1/whyqd/config/__init__.py
+-rwxr-xr-x   0        0        0     2607 2023-05-10 14:13:08.656397 whyqd-1.0.1/whyqd/config/ray_init.py
+-rwxr-xr-x   0        0        0      520 2023-05-10 14:13:08.657397 whyqd-1.0.1/whyqd/config/settings.py
+-rwxr-xr-x   0        0        0      172 2023-05-10 14:13:08.657397 whyqd-1.0.1/whyqd/core/__init__.py
+-rwxr-xr-x   0        0        0     8358 2023-05-10 14:13:08.658398 whyqd-1.0.1/whyqd/core/base.py
+-rwxr-xr-x   0        0        0     6068 2023-05-12 06:36:03.714646 whyqd-1.0.1/whyqd/core/crosswalk.py
+-rwxr-xr-x   0        0        0    10547 2023-05-12 06:36:33.964292 whyqd-1.0.1/whyqd/core/datasource.py
+-rwxr-xr-x   0        0        0     3862 2023-05-12 06:37:05.626333 whyqd-1.0.1/whyqd/core/schema.py
+-rwxr-xr-x   0        0        0    11580 2023-05-11 08:09:37.227431 whyqd-1.0.1/whyqd/core/transform.py
+-rwxr-xr-x   0        0        0        0 2023-05-10 14:13:08.662396 whyqd-1.0.1/whyqd/crosswalk/__init__.py
+-rwxr-xr-x   0        0        0     1537 2023-05-10 14:13:08.662396 whyqd-1.0.1/whyqd/crosswalk/actions/__init__.py
+-rwxr-xr-x   0        0        0     2934 2023-05-10 14:13:08.663396 whyqd-1.0.1/whyqd/crosswalk/actions/calculate.py
+-rwxr-xr-x   0        0        0     1507 2023-05-10 14:13:08.664396 whyqd-1.0.1/whyqd/crosswalk/actions/categorise.py
+-rwxr-xr-x   0        0        0     1090 2023-05-10 14:13:08.664396 whyqd-1.0.1/whyqd/crosswalk/actions/deblank.py
+-rwxr-xr-x   0        0        0      975 2023-05-10 14:13:08.665396 whyqd-1.0.1/whyqd/crosswalk/actions/dedupe.py
+-rwxr-xr-x   0        0        0     1249 2023-05-10 14:13:08.665396 whyqd-1.0.1/whyqd/crosswalk/actions/delete_rows.py
+-rwxr-xr-x   0        0        0     1538 2023-05-10 14:13:08.666397 whyqd-1.0.1/whyqd/crosswalk/actions/new.py
+-rwxr-xr-x   0        0        0     4021 2023-05-10 14:13:08.667401 whyqd-1.0.1/whyqd/crosswalk/actions/pivot_categories.py
+-rwxr-xr-x   0        0        0     1893 2023-05-10 14:13:08.667401 whyqd-1.0.1/whyqd/crosswalk/actions/pivot_longer.py
+-rwxr-xr-x   0        0        0     1535 2023-05-10 14:13:08.668401 whyqd-1.0.1/whyqd/crosswalk/actions/rename.py
+-rwxr-xr-x   0        0        0     2200 2023-05-10 14:13:08.669397 whyqd-1.0.1/whyqd/crosswalk/actions/select.py
+-rwxr-xr-x   0        0        0     3832 2023-05-10 14:13:08.669397 whyqd-1.0.1/whyqd/crosswalk/actions/select_newest.py
+-rwxr-xr-x   0        0        0     3826 2023-05-10 14:13:08.670396 whyqd-1.0.1/whyqd/crosswalk/actions/select_oldest.py
+-rwxr-xr-x   0        0        0     3418 2023-05-10 14:13:08.671399 whyqd-1.0.1/whyqd/crosswalk/actions/separate.py
+-rwxr-xr-x   0        0        0     2105 2023-05-10 14:13:08.672397 whyqd-1.0.1/whyqd/crosswalk/actions/unite.py
+-rwxr-xr-x   0        0        0      131 2023-05-10 14:13:08.673398 whyqd-1.0.1/whyqd/crosswalk/base/__init__.py
+-rwxr-xr-x   0        0        0     6247 2023-05-10 14:13:08.674398 whyqd-1.0.1/whyqd/crosswalk/base/action_base.py
+-rwxr-xr-x   0        0        0     8242 2023-05-10 14:13:08.675397 whyqd-1.0.1/whyqd/crosswalk/base/category_base.py
+-rwxr-xr-x   0        0        0     3940 2023-05-10 14:13:08.675397 whyqd-1.0.1/whyqd/crosswalk/base/morph_base.py
+-rwxr-xr-x   0        0        0      258 2023-05-10 14:13:08.676397 whyqd-1.0.1/whyqd/crud/__init__.py
+-rwxr-xr-x   0        0        0    12381 2023-05-12 06:38:16.658348 whyqd-1.0.1/whyqd/crud/action.py
+-rwxr-xr-x   0        0        0     4873 2023-05-10 14:13:08.677395 whyqd-1.0.1/whyqd/crud/base.py
+-rwxr-xr-x   0        0        0     7873 2023-05-12 06:38:36.849050 whyqd-1.0.1/whyqd/crud/field.py
+-rwxr-xr-x   0        0        0       88 2023-05-10 14:13:08.679396 whyqd-1.0.1/whyqd/dtypes/__init__.py
+-rwxr-xr-x   0        0        0     1928 2023-05-10 14:13:08.679396 whyqd-1.0.1/whyqd/dtypes/field.py
+-rwxr-xr-x   0        0        0      900 2023-05-10 14:13:08.680396 whyqd-1.0.1/whyqd/dtypes/mime.py
+-rwxr-xr-x   0        0        0     1294 2023-05-10 14:13:08.680396 whyqd-1.0.1/whyqd/dtypes/status.py
+-rwxr-xr-x   0        0        0      617 2023-05-10 14:13:08.681397 whyqd-1.0.1/whyqd/models/__init__.py
+-rwxr-xr-x   0        0        0     1077 2023-05-10 14:13:08.681397 whyqd-1.0.1/whyqd/models/action_category.py
+-rwxr-xr-x   0        0        0     1086 2023-05-10 14:13:08.682397 whyqd-1.0.1/whyqd/models/action_morph.py
+-rwxr-xr-x   0        0        0     1665 2023-05-10 14:13:08.682397 whyqd-1.0.1/whyqd/models/action_schema.py
+-rwxr-xr-x   0        0        0      530 2023-05-10 14:13:08.683396 whyqd-1.0.1/whyqd/models/actionscript.py
+-rwxr-xr-x   0        0        0      584 2023-05-10 14:13:08.683396 whyqd-1.0.1/whyqd/models/category.py
+-rwxr-xr-x   0        0        0     2569 2023-05-10 14:13:08.684399 whyqd-1.0.1/whyqd/models/citation.py
+-rwxr-xr-x   0        0        0     1366 2023-05-10 14:13:08.684399 whyqd-1.0.1/whyqd/models/column.py
+-rwxr-xr-x   0        0        0     2162 2023-05-10 14:13:08.685395 whyqd-1.0.1/whyqd/models/constraints.py
+-rwxr-xr-x   0        0        0     1977 2023-05-10 14:13:08.685395 whyqd-1.0.1/whyqd/models/crosswalk.py
+-rwxr-xr-x   0        0        0     4358 2023-05-10 14:13:08.686398 whyqd-1.0.1/whyqd/models/datasource.py
+-rwxr-xr-x   0        0        0     1367 2023-05-10 14:13:08.687398 whyqd-1.0.1/whyqd/models/fields.py
+-rwxr-xr-x   0        0        0      608 2023-05-10 14:13:08.688398 whyqd-1.0.1/whyqd/models/modifier.py
+-rwxr-xr-x   0        0        0     2650 2023-05-10 14:13:08.688398 whyqd-1.0.1/whyqd/models/schema.py
+-rwxr-xr-x   0        0        0     2046 2023-05-10 14:13:08.690396 whyqd-1.0.1/whyqd/models/transform.py
+-rwxr-xr-x   0        0        0      527 2023-05-10 14:13:08.690396 whyqd-1.0.1/whyqd/models/version.py
+-rwxr-xr-x   0        0        0      210 2023-05-10 14:13:08.691396 whyqd-1.0.1/whyqd/parsers/__init__.py
+-rwxr-xr-x   0        0        0    14750 2023-05-10 14:13:08.692394 whyqd-1.0.1/whyqd/parsers/action.py
+-rwxr-xr-x   0        0        0    10614 2023-05-10 14:13:08.692394 whyqd-1.0.1/whyqd/parsers/category.py
+-rwxr-xr-x   0        0        0     9550 2023-06-06 14:17:55.467244 whyqd-1.0.1/whyqd/parsers/core.py
+-rwxr-xr-x   0        0        0    31304 2023-06-06 14:29:01.427298 whyqd-1.0.1/whyqd/parsers/datasource.py
+-rwxr-xr-x   0        0        0     9021 2023-05-10 14:13:08.694397 whyqd-1.0.1/whyqd/parsers/morph.py
+-rwxr-xr-x   0        0        0     6789 2023-05-10 14:13:08.695395 whyqd-1.0.1/whyqd/parsers/script.py
+-rw-r--r--   0        0        0     9036 1970-01-01 00:00:00.000000 whyqd-1.0.1/setup.py
+-rw-r--r--   0        0        0     9339 1970-01-01 00:00:00.000000 whyqd-1.0.1/PKG-INFO
```

### Comparing `whyqd-1.0.0/LICENSE` & `whyqd-1.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `whyqd-1.0.0/README.md` & `whyqd-1.0.1/README.md`

 * *Files 11% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 # whyqd: simplicity, transparency, speed
 
-[![Documentation Status](https://readthedocs.org/projects/whyqd/badge/?version=latest)](https://whyqd.readthedocs.io/en/latest/?badge=latest)
+[![Documentation Status](https://readthedocs.org/projects/whyqd/badge/?version=latest)](docs/en/latest/?badge=latest)
 [![Build Status](https://travis-ci.com/whythawk/whyqd.svg?branch=master)](https://travis-ci.com/whythawk/whyqd.svg?branch=master)
 [![DOI](https://zenodo.org/badge/239159569.svg)](https://zenodo.org/badge/latestdoi/239159569)
 
 ## What is it?
 
 > More research, less wrangling
 
 [**whyqd**](https://whyqd.com) (/wɪkɪd/) is a curatorial toolkit intended to produce well-structured and predictable 
 data for research analysis.
 
-It provides an intuitive method creating schema-to-schema crosswalks for restructuring messy data to conform to a 
+It provides an intuitive method for creating schema-to-schema crosswalks for restructuring messy data to conform to a 
 standardised metadata schema. It supports rapid and continuous transformation of messy data using a simple series of 
 steps. Once complete, you can import wrangled data into more complex analytical or database systems.
 
 **whyqd** plays well with your existing Python-based data-analytical tools. It uses [Ray](https://www.ray.io/) and 
 [Modin](https://modin.readthedocs.io/) as a drop-in replacement for [Pandas](https://pandas.pydata.org/) to support 
 processing of large datasets, and [Pydantic](https://pydantic-docs.helpmanual.io/) for data models. 
 
@@ -24,22 +24,23 @@
 production.
 
 Once complete, a transform file can be shared, along with your input data, and anyone can import and validate your 
 crosswalk to verify that your output data is the product of these inputs.
 
 ## Why use it?
 
-If all you want to do is test whether your source data are even useful, spending days or weeks slogging through data 
-restructuring could kill a project. If you already have a workflow and established software which includes Python and 
-pandas, having to change your code every time your source data changes is really, really frustrating.
+**whyqd** allows you to get to work without requiring you to achieve buy-in from anyone or change your existing code.
 
-If you want to go from a [Cthulhu dataset](https://whyqd.readthedocs.io/tutorials/tutorial3) like this:
+If you don't want to spend days or weeks slogging through data when all you want to do is test whether your source 
+data are even useful. If you already have a workflow and established software which includes Python and pandas, and 
+don't want to change your code every time your source data changes.
 
-![UNDP Human Development Index 2007-2008: a beautiful example of messy data.](https://raw.githubusercontent.com/whythawk/whyqd/master/docs/images/undp-hdi-2007-8.jpg)
+If you want to go from a [Cthulhu dataset](https://whyqd.readthedocs.io/en/latest/tutorials/tutorial3) like this:
 
+![UNDP Human Development Index 2007-2008: a beautiful example of messy data.](docs/images/undp-hdi-2007-8.jpg)
 *UNDP Human Development Index 2007-2008: a beautiful example of messy data.*
 
 To this:
 
 |    | country_name           | indicator_name   | reference   |   year |   values |
 |:---|:-----------------------|:-----------------|:------------|:-------|:---------|
 |  0 | Hong Kong, China (SAR) | HDI rank         | e           |   2008 |       21 |
@@ -58,18 +59,20 @@
     "PIVOT_LONGER > ['indicator_name', 'values'] < ['HDI rank', 'HDI Category', 'Human poverty index (HPI-1) - Rank;;2008', 'Human poverty index (HPI-1) - Value (%);;2008', 'Probability at birth of not surviving to age 40 (% of cohort);;2000-05', 'Adult illiteracy rate (% aged 15 and older);;1995-2005', 'Population not using an improved water source (%);;2004', 'Children under weight for age (% under age 5);;1996-2005', 'Population below income poverty line (%) - $1 a day;;1990-2005', 'Population below income poverty line (%) - $2 a day;;1990-2005', 'Population below income poverty line (%) - National poverty line;;1990-2004', 'HPI-1 rank minus income poverty rank;;2008']",
     "SEPARATE > ['indicator_name', 'year'] < ';;'::['indicator_name']",
     "DEBLANK",
     "DEDUPE",
 ]
 ```
 
+Then **whyqd** may be for you.
+
 ## How does it work?
 
 > Crosswalks are mappings of the relationships between fields defined in different metadata 
-> [schemas](https://whyqd.readthedocs.io/strategies/schema). Ideally, these are one-to-one, where a field in 
+> [schemas](https://whyqd.readthedocs.io/en/latest/strategies/schema). Ideally, these are one-to-one, where a field in 
 > one has an exact match in the other. In practice, it's more complicated than that.
 
 Your workflow is:
 
 1. Define a single destination schema,
 2. Derive a source schema from a data source,
 3. Review your source data structure,
@@ -79,21 +82,21 @@
 
 It starts like this:
 
 ```python
 import whyqd as qd
 ```
 
-[Install](https://whyqd.readthedocs.io/installation) and [get started](https://whyqd.readthedocs.io/quickstart).
+[Install](https://whyqd.readthedocs.io/en/latest/installation) and then read the [quickstart](https://whyqd.readthedocs.io/en/latest/quickstart).
 
 There are three worked tutorials to guide you through three typical scenarios:
 
-- [Aligning multiple data disparate sources to a single schema](https://whyqd.readthedocs.io/tutorials/tutorial1)
-- [Pivoting wide-format data into archival long-format](https://whyqd.readthedocs.io/tutorials/tutorial2)
-- [Wrangling Cthulhu data without losing your mind](https://whyqd.readthedocs.io/tutorials/tutorial3)
+- [Aligning multiple disparate data sources to a single schema](https://whyqd.readthedocs.io/en/latest/tutorials/tutorial1)
+- [Pivoting wide-format data into archival long-format](https://whyqd.readthedocs.io/en/latest/tutorials/tutorial2)
+- [Wrangling Cthulhu data without losing your mind](https://whyqd.readthedocs.io/en/latest/tutorials/tutorial3)
 
 ## Installation
 
 You'll need at least Python 3.8, then install with your favourite package manager:
 
 ```bash
 pip install whyqd
@@ -109,19 +112,19 @@
 schema_source = qd.SchemaDefinition()
 schema_source.derive_model(data=datasource.get)
 schema_source.fields.set_categories(name=CATEGORY_FIELD, 
                                     terms=datasource.get_data())
 schema_source.save()
 ```
 
-[Get started...](https://whyqd.readthedocs.io/quickstart)
+[Get started...](https://whyqd.readthedocs.io/en/latest/quickstart)
 
 ## Changelog
 
-The version history can be found in the [changelog](https://whyqd.readthedocs.io/changelog).
+The version history can be found in the [changelog](https://whyqd.readthedocs.io/en/latest/changelog).
 
 ## Background and funding
 
 **whyqd** was created to serve a continuous data wrangling process, including collaboration on more complex messy 
 sources, ensuring the integrity of the source data, and producing a complete audit trail from data imported to our 
 database, back to source. You can see the product of that at [openLocal.uk](https://openlocal.uk).
```

### Comparing `whyqd-1.0.0/pyproject.toml` & `whyqd-1.0.1/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "whyqd"
-version = "1.0.0"
+version = "1.0.1"
 description = "data wrangling simplicity, complete audit transparency, and at speed"
 authors = ["Gavin Chait <gchait@whythawk.com>"]
 license = "BSD-3-Clause"
 readme = "README.md"
 homepage = "https://whyqd.com"
 repository = "https://github.com/whythawk/whyqd/"
 documentation = "https://whyqd.readthedocs.io/"
@@ -58,8 +58,8 @@
 build-backend = "poetry.core.masonry.api"
 
 [tool.black]
 line-length = 120
 target-version = ["py38"]
 
 [tool.poetry.extras]
-docs = ["Sphinx"]
+docs = ["MKDocs"]
```

### Comparing `whyqd-1.0.0/tests/data/2023-05-09-human-development-report-interim.PARQUET` & `whyqd-1.0.1/tests/data/2023-05-09-human-development-report-interim.PARQUET`

 * *Files identical despite different names*

### Comparing `whyqd-1.0.0/tests/data/HDR-2007-2008-Table-03.xlsx` & `whyqd-1.0.1/tests/data/HDR-2007-2008-Table-03.xlsx`

 * *Files identical despite different names*

### Comparing `whyqd-1.0.0/tests/data/raw_E06000044_014_0.XLSX` & `whyqd-1.0.1/tests/data/raw_E06000044_014_0.XLSX`

 * *Files identical despite different names*

### Comparing `whyqd-1.0.0/tests/data/raw_E06000044_014_0.data` & `whyqd-1.0.1/tests/data/raw_E06000044_014_0.data`

 * *Files identical despite different names*

### Comparing `whyqd-1.0.0/tests/data/raw_E06000044_014_1.XLSX` & `whyqd-1.0.1/tests/data/raw_E06000044_014_1.XLSX`

 * *Files identical despite different names*

### Comparing `whyqd-1.0.0/tests/data/raw_E06000044_014_2.XLSX` & `whyqd-1.0.1/tests/data/raw_E06000044_014_2.XLSX`

 * *Files identical despite different names*

### Comparing `whyqd-1.0.0/tests/data/raw_duplicated_E06000044_014.xlsx` & `whyqd-1.0.1/tests/data/raw_duplicated_E06000044_014.xlsx`

 * *Files identical despite different names*

### Comparing `whyqd-1.0.0/tests/data/raw_multi_E06000044_014.xlsx` & `whyqd-1.0.1/tests/data/raw_multi_E06000044_014.xlsx`

 * *Files identical despite different names*

### Comparing `whyqd-1.0.0/tests/data/restructured_test_data.xlsx` & `whyqd-1.0.1/tests/data/restructured_test_data.xlsx`

 * *Files identical despite different names*

### Comparing `whyqd-1.0.0/tests/data/test_crosswalk.crosswalk` & `whyqd-1.0.1/tests/data/test_crosswalk.crosswalk`

 * *Files identical despite different names*

### Comparing `whyqd-1.0.0/tests/data/test_cthulu_destination.schema` & `whyqd-1.0.1/tests/data/test_cthulu_destination.schema`

 * *Files identical despite different names*

### Comparing `whyqd-1.0.0/tests/data/test_cthulu_interim.data` & `whyqd-1.0.1/tests/data/test_cthulu_interim.data`

 * *Files identical despite different names*

### Comparing `whyqd-1.0.0/tests/data/test_cthulu_interim.schema` & `whyqd-1.0.1/tests/data/test_cthulu_interim.schema`

 * *Files identical despite different names*

### Comparing `whyqd-1.0.0/tests/data/test_cthulu_source.data` & `whyqd-1.0.1/tests/data/test_cthulu_source.data`

 * *Files identical despite different names*

### Comparing `whyqd-1.0.0/tests/data/test_cthulu_source.schema` & `whyqd-1.0.1/tests/data/test_cthulu_source.schema`

 * *Files identical despite different names*

### Comparing `whyqd-1.0.0/tests/data/test_data.csv` & `whyqd-1.0.1/tests/data/test_data.csv`

 * *Files identical despite different names*

### Comparing `whyqd-1.0.0/tests/data/test_derived_schema.schema` & `whyqd-1.0.1/tests/data/test_derived_schema.schema`

 * *Files identical despite different names*

### Comparing `whyqd-1.0.0/tests/data/test_portsmouth_destination.schema` & `whyqd-1.0.1/tests/data/test_portsmouth_destination.schema`

 * *Files identical despite different names*

### Comparing `whyqd-1.0.0/tests/data/test_portsmouth_source.data` & `whyqd-1.0.1/tests/data/test_portsmouth_source.data`

 * *Files identical despite different names*

### Comparing `whyqd-1.0.0/tests/data/test_portsmouth_source.schema` & `whyqd-1.0.1/tests/data/test_portsmouth_source.schema`

 * *Files identical despite different names*

### Comparing `whyqd-1.0.0/tests/data/test_schema.json` & `whyqd-1.0.1/tests/data/test_schema.json`

 * *Files identical despite different names*

### Comparing `whyqd-1.0.0/tests/data/test_schema.schema` & `whyqd-1.0.1/tests/data/test_schema.schema`

 * *Files identical despite different names*

### Comparing `whyqd-1.0.0/tests/data/test_source_schema.schema` & `whyqd-1.0.1/tests/data/test_source_schema.schema`

 * *Files identical despite different names*

### Comparing `whyqd-1.0.0/tests/data/urban_population.json` & `whyqd-1.0.1/tests/data/urban_population.json`

 * *Files identical despite different names*

### Comparing `whyqd-1.0.0/tests/data/working_test_data.xlsx` & `whyqd-1.0.1/tests/data/working_test_data.xlsx`

 * *Files identical despite different names*

### Comparing `whyqd-1.0.0/tests/data/working_test_world_bank_data.xlsx` & `whyqd-1.0.1/tests/data/working_test_world_bank_data.xlsx`

 * *Files identical despite different names*

### Comparing `whyqd-1.0.0/whyqd/config/ray_init.py` & `whyqd-1.0.1/whyqd/config/ray_init.py`

 * *Files identical despite different names*

### Comparing `whyqd-1.0.0/whyqd/config/settings.py` & `whyqd-1.0.1/whyqd/config/settings.py`

 * *Files identical despite different names*

### Comparing `whyqd-1.0.0/whyqd/core/base.py` & `whyqd-1.0.1/whyqd/core/base.py`

 * *Files identical despite different names*

### Comparing `whyqd-1.0.0/whyqd/core/crosswalk.py` & `whyqd-1.0.1/whyqd/core/crosswalk.py`

 * *Files 1% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 
 
 class CrosswalkDefinition(BaseDefinition):
     """Create and manage a method to perform a schema to schema crosswalk.
 
     !!! tip "Strategy"
         Guidance on how to use this definition is in the strategies section on
-        [Crosswalk Strategies](/strategies/crosswalk).
+        [Crosswalk Strategies](../strategies/crosswalk.md).
 
     Parameters:
       crosswalk: A dictionary conforming to the CrosswalkModel, or a path to a saved definition.
       schema_source: Path to a json file containing a saved schema, or a dictionary conforming to one, or a definition.
       schema_destination: Path to a json file containing a saved schema, or a dictionary conforming to one, or a definition.
 
     Example:
@@ -104,15 +104,15 @@
 
     #########################################################################################
     # MANAGE ACTION SCRIPTS
     #########################################################################################
 
     @property
     def actions(self) -> CRUDAction:
-        """Returns the active crud model for all Action operations. See [Action CRUD](/api/action) for API.
+        """Returns the active crud model for all Action operations. See [Action CRUD](action.md) for API.
 
         Returns:
           For all Action CRUD behaviours.
         """
         if not self.model.schemaSource or not self.model.schemaDestination:
             raise ValueError("First set source and destination schemas before performing defining a crosswalk.")
         return self.crud
```

### Comparing `whyqd-1.0.0/whyqd/core/datasource.py` & `whyqd-1.0.1/whyqd/core/datasource.py`

 * *Files 4% similar despite different names*

```diff
@@ -14,25 +14,31 @@
 
 
 class DataSourceDefinition(BaseDefinition):
     """Create and manage a data source schema.
 
     !!! tip "Strategy"
         Guidance on how to use this definition is in the strategies section on
-        [DataSource Strategies](/strategies/datasource).
+        [DataSource Strategies](../strategies/datasource.md).
 
     !!! info
         **whyqd** supports any of the following file mime types:
 
         - `CSV`: "text/csv"
         - `XLS`: "application/vnd.ms-excel"
         - `XLSX`: "application/vnd.openxmlformats-officedocument.spreadsheetml.sheet"
         - `PARQUET` (or `PRQ`): "application/vnd.apache.parquet"
         - `FEATHER` (or `FTR`): "application/vnd.apache.feather"
 
+        Declare it like so:
+
+        ```python
+        MIMETYPE = "xlsx" # upper- or lower-case is fine
+        ```
+
         Specify the mime type as a text string, uppper- or lower-case. Neither of
         [Parquet](https://parquet.apache.org/docs/overview/) or [Feather](https://arrow.apache.org/docs/python/feather.html)
         yet have official mimetypes, so this is what we're using for now.
 
     Parameters:
       source: A path to a json file containing a saved schema, or a dictionary conforming to the DataSourceModel.
 
@@ -105,27 +111,14 @@
         mimetype: str | MimeType,
         header: int | list[int | None] | None = 0,
         **attributes,
     ) -> DataSourceModel | list[DataSourceModel]:
         """Derive a data model schema (or list) from a data source. All columns will be coerced to `string` type to
         preserve data quality even though this is far less efficient.
 
-        !!! info
-            **whyqd** supports any of the following file mime types:
-
-            - `CSV`: "text/csv"
-            - `XLS`: "application/vnd.ms-excel"
-            - `XLSX`: "application/vnd.openxmlformats-officedocument.spreadsheetml.sheet"
-            - `PARQUET` (or `PRQ`): "application/vnd.apache.parquet"
-            - `FEATHER` (or `FTR`): "application/vnd.apache.feather"
-
-            Specify the mime type as a text string, uppper- or lower-case. Neither of
-            [Parquet](https://parquet.apache.org/docs/overview/) or [Feather](https://arrow.apache.org/docs/python/feather.html)
-            yet have official mimetypes, so this is what we're using for now.
-
         Parameters:
           source:  Source filename.
           mimetype:  Pandas can read a diversity of mimetypes. **whyqd** supports `xls`, `xlsx`, `csv`, `parquet` and `feather`.
           header:  Row (0-indexed) to use for the column labels of the parsed DataFrame. If there are multiple sheets, then
                     a list of integers should be provided. If `header` is `None`, row 0 will be treated as values and a
                     set of field names will be generated indexed to the number of data columns.
           attributes: dict of specific `mimetype` related Pandas attributes. Use sparingly.
```

### Comparing `whyqd-1.0.0/whyqd/core/schema.py` & `whyqd-1.0.1/whyqd/core/schema.py`

 * *Files 4% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 
 
 class SchemaDefinition(BaseDefinition):
     """Create and manage a metadata schema.
 
     !!! tip "Strategy"
         Guidance on how to use this definition is in the strategies section on
-        [Schema Strategies](/strategies/schema).
+        [Schema Strategies](../strategies/schema.md).
 
     Parameters:
       source: A path to a json file containing a saved schema, or a dictionary conforming to the SchemaModel.
 
     Example:
       Create a new `SchemaDefinition` as follows:
 
@@ -72,15 +72,15 @@
           schema: A dictionary, or path to a dictionary or json file, conforming to the SchemaModel.
         """
         self.model = self.core.create_or_update_model(modelType=SchemaModel, source=schema, model=self.model)
         self._refresh_model_fields()
 
     @property
     def fields(self) -> CRUDField:
-        """Returns the active crud model for all Field operations. See [Field CRUD](/api/field) for API.
+        """Returns the active crud model for all Field operations. See [Field CRUD](field.md) for API.
 
         Returns:
           For all Field CRUD behaviours.
         """
         return self.crud
 
     #########################################################################################
```

### Comparing `whyqd-1.0.0/whyqd/core/transform.py` & `whyqd-1.0.1/whyqd/core/transform.py`

 * *Files 3% similar despite different names*

```diff
@@ -197,27 +197,22 @@
         directory: str | Path | None = None,
         created_by: str | None = None,
         hide_uuid: bool = False,
     ) -> bool:
         """Save model as a json file, and save crosswalked destination dataframe as a chosen mimetype.
 
         !!! info
-            **whyqd** supports any of the following file mime types:
+            **NOTE:** by default, transformed data are saved as `PARQUET` as this is the most efficient.
 
-            - `CSV`: "text/csv"
-            - `XLS`: "application/vnd.ms-excel"
-            - `XLSX`: "application/vnd.openxmlformats-officedocument.spreadsheetml.sheet"
-            - `PARQUET` (or `PRQ`): "application/vnd.apache.parquet"
-            - `FEATHER` (or `FTR`): "application/vnd.apache.feather"
+            Declare your mime type like so:
 
-            Specify the mime type as a text string, uppper- or lower-case. Neither of
-            [Parquet](https://parquet.apache.org/docs/overview/) or [Feather](https://arrow.apache.org/docs/python/feather.html)
-            yet have official mimetypes, so this is what we're using for now.
+            ```python
+            MIMETYPE = "csv" # upper- or lower-case is fine
+            ```
 
-            **NOTE:** by default, transformed data are saved as `PARQUET` as this is the most efficient.
 
         Parameters:
           directory:  Defaults to working directory
           filename:  Defaults to model name
           mimetype: **whyqd** supports saving to CSV, XLS, XLSX, Feather and Parquet files. Defaults to Parquet.
           created_by:  Declare the model creator/updater
           hide_uuid:  Hide all UUIDs in the nested JSON output.
```

### Comparing `whyqd-1.0.0/whyqd/crosswalk/actions/__init__.py` & `whyqd-1.0.1/whyqd/crosswalk/actions/__init__.py`

 * *Files identical despite different names*

### Comparing `whyqd-1.0.0/whyqd/crosswalk/actions/calculate.py` & `whyqd-1.0.1/whyqd/crosswalk/actions/calculate.py`

 * *Files identical despite different names*

### Comparing `whyqd-1.0.0/whyqd/crosswalk/actions/categorise.py` & `whyqd-1.0.1/whyqd/crosswalk/actions/categorise.py`

 * *Files identical despite different names*

### Comparing `whyqd-1.0.0/whyqd/crosswalk/actions/deblank.py` & `whyqd-1.0.1/whyqd/crosswalk/actions/deblank.py`

 * *Files identical despite different names*

### Comparing `whyqd-1.0.0/whyqd/crosswalk/actions/dedupe.py` & `whyqd-1.0.1/whyqd/crosswalk/actions/dedupe.py`

 * *Files identical despite different names*

### Comparing `whyqd-1.0.0/whyqd/crosswalk/actions/delete_rows.py` & `whyqd-1.0.1/whyqd/crosswalk/actions/delete_rows.py`

 * *Files identical despite different names*

### Comparing `whyqd-1.0.0/whyqd/crosswalk/actions/new.py` & `whyqd-1.0.1/whyqd/crosswalk/actions/new.py`

 * *Files identical despite different names*

### Comparing `whyqd-1.0.0/whyqd/crosswalk/actions/pivot_categories.py` & `whyqd-1.0.1/whyqd/crosswalk/actions/pivot_categories.py`

 * *Files identical despite different names*

### Comparing `whyqd-1.0.0/whyqd/crosswalk/actions/pivot_longer.py` & `whyqd-1.0.1/whyqd/crosswalk/actions/pivot_longer.py`

 * *Files identical despite different names*

### Comparing `whyqd-1.0.0/whyqd/crosswalk/actions/rename.py` & `whyqd-1.0.1/whyqd/crosswalk/actions/rename.py`

 * *Files identical despite different names*

### Comparing `whyqd-1.0.0/whyqd/crosswalk/actions/select.py` & `whyqd-1.0.1/whyqd/crosswalk/actions/select.py`

 * *Files identical despite different names*

### Comparing `whyqd-1.0.0/whyqd/crosswalk/actions/select_newest.py` & `whyqd-1.0.1/whyqd/crosswalk/actions/select_newest.py`

 * *Files identical despite different names*

### Comparing `whyqd-1.0.0/whyqd/crosswalk/actions/select_oldest.py` & `whyqd-1.0.1/whyqd/crosswalk/actions/select_oldest.py`

 * *Files identical despite different names*

### Comparing `whyqd-1.0.0/whyqd/crosswalk/actions/separate.py` & `whyqd-1.0.1/whyqd/crosswalk/actions/separate.py`

 * *Files identical despite different names*

### Comparing `whyqd-1.0.0/whyqd/crosswalk/actions/unite.py` & `whyqd-1.0.1/whyqd/crosswalk/actions/unite.py`

 * *Files identical despite different names*

### Comparing `whyqd-1.0.0/whyqd/crosswalk/base/action_base.py` & `whyqd-1.0.1/whyqd/crosswalk/base/action_base.py`

 * *Files identical despite different names*

### Comparing `whyqd-1.0.0/whyqd/crosswalk/base/category_base.py` & `whyqd-1.0.1/whyqd/crosswalk/base/category_base.py`

 * *Files identical despite different names*

### Comparing `whyqd-1.0.0/whyqd/crosswalk/base/morph_base.py` & `whyqd-1.0.1/whyqd/crosswalk/base/morph_base.py`

 * *Files identical despite different names*

### Comparing `whyqd-1.0.0/whyqd/crud/action.py` & `whyqd-1.0.1/whyqd/crud/action.py`

 * *Files 2% similar despite different names*

```diff
@@ -11,17 +11,17 @@
 if TYPE_CHECKING:
     from whyqd.core import SchemaDefinition
     from whyqd.models import FieldModel
 
 
 class CRUDAction(CRUDBase[ActionScriptModel]):
     """Create, Read, Update and Delete Field Models. Usually instantiated as part of a
-    [CrosswalkDefinition](/api/crosswalk) and accessed as `.actions`.
+    [CrosswalkDefinition](crosswalk.md) and accessed as `.actions`.
 
-    [Base CRUD operations](/api/basecrud) are common for both `CRUDField` and `CRUDAction`.
+    [Base CRUD operations](basecrud.md) are common for both `CRUDField` and `CRUDAction`.
 
     Example:
       ```python
       import whyqd as qd
 
       crosswalk = qd.CrosswalkDefinition()
       crosswalk.set(schema_source=SCHEMA_SOURCE, schema_destination=SCHEMA_DESTINATION)
@@ -36,16 +36,16 @@
           "RENAME > 'country_code' < ['Country Code']",
           "RENAME > 'country_name' < ['Country Name']",
       ]
       crosswalk.actions.add_multi(terms=schema_scripts)
       ```
 
     Parameters:
-      schema_source: A [SchemaDefinition](/api/schema) for access to source schema definitions and operations.
-      schema_destination: A [SchemaDefinition](/api/schema) for access to destination schema definitions and operations.
+      schema_source: A [SchemaDefinition](schema.md) for access to source schema definitions and operations.
+      schema_destination: A [SchemaDefinition](schema.md) for access to destination schema definitions and operations.
     """
 
     def __init__(self, *, schema_source: SchemaDefinition = None, schema_destination: SchemaDefinition = None):
         super().__init__(ActionScriptModel)
         self.parser = ScriptParser()
         self.schema_source = None
         self.schema_destination = None
@@ -226,16 +226,16 @@
 
     def set_schema(
         self, *, schema_source: SchemaDefinition = None, schema_destination: SchemaDefinition = None
     ) -> None:
         """Set SchemaDefinitions.
 
         Parameters:
-          schema_source: A [SchemaDefinition](/api/schema) for access to source schema definitions and operations.
-          schema_destination: A [SchemaDefinition](/api/schema) for access to destination schema definitions and operations.
+          schema_source: A [SchemaDefinition](schema.md) for access to source schema definitions and operations.
+          schema_destination: A [SchemaDefinition](schema.md) for access to destination schema definitions and operations.
         """
         if not schema_source or not schema_destination:
             raise ValueError("Schema for both source and destination has not been provided.")
         self.schema_source = schema_source
         self.schema_destination = schema_destination
         self.uncrossed = {field.uuid for field in self.schema_destination.get.fields}
 
@@ -263,15 +263,15 @@
           script: A string term conforming to the script structure for a specific action.
           action: The action model type conforming to the requirements for a script.
 
         Raises:
           ValueError: If the script can't be parsed.
 
         Returns:
-          Parser for Action type, and used in [TransformDefinition](/api/transform) and [CrosswalkDefinition](/api/crosswalk).
+          Parser for Action type, and used in [TransformDefinition](transform.md) and [CrosswalkDefinition](crosswalk.md).
         """
         if not action:
             action = self.get_action(script=script)
         # Test for each of BaseSchemaAction | BaseMorphAction | BaseCategoryAction
         if isinstance(action, BaseSchemaAction):
             return ActionParser
         if isinstance(action, BaseMorphAction):
```

### Comparing `whyqd-1.0.0/whyqd/crud/base.py` & `whyqd-1.0.1/whyqd/crud/base.py`

 * *Files identical despite different names*

### Comparing `whyqd-1.0.0/whyqd/crud/field.py` & `whyqd-1.0.1/whyqd/crud/field.py`

 * *Files 1% similar despite different names*

```diff
@@ -5,17 +5,17 @@
 from whyqd.crud.base import CRUDBase
 from whyqd.models import FieldModel, ConstraintsModel, CategoryModel
 from whyqd.dtypes import FieldType
 
 
 class CRUDField(CRUDBase[FieldModel]):
     """Create, Read, Update and Delete Field Models. Usually instantiated as part of a
-    [SchemaDefinition](/api/schema) and accessed as `.fields`.
+    [SchemaDefinition](schema.md) and accessed as `.fields`.
 
-    [Base CRUD operations](/api/basecrud) are common for both `CRUDField` and `CRUDAction`.
+    [Base CRUD operations](basecrud.md) are common for both `CRUDField` and `CRUDAction`.
 
     Example:
       ```python
       import whyqd as qd
 
       schema: qd.models.SchemaModel = {
           "name": "urban_population",
```

### Comparing `whyqd-1.0.0/whyqd/dtypes/field.py` & `whyqd-1.0.1/whyqd/dtypes/field.py`

 * *Files identical despite different names*

### Comparing `whyqd-1.0.0/whyqd/dtypes/mime.py` & `whyqd-1.0.1/whyqd/dtypes/mime.py`

 * *Files identical despite different names*

### Comparing `whyqd-1.0.0/whyqd/dtypes/status.py` & `whyqd-1.0.1/whyqd/dtypes/status.py`

 * *Files identical despite different names*

### Comparing `whyqd-1.0.0/whyqd/models/__init__.py` & `whyqd-1.0.1/whyqd/models/__init__.py`

 * *Files identical despite different names*

### Comparing `whyqd-1.0.0/whyqd/models/action_category.py` & `whyqd-1.0.1/whyqd/models/action_category.py`

 * *Files identical despite different names*

### Comparing `whyqd-1.0.0/whyqd/models/action_morph.py` & `whyqd-1.0.1/whyqd/models/action_morph.py`

 * *Files identical despite different names*

### Comparing `whyqd-1.0.0/whyqd/models/action_schema.py` & `whyqd-1.0.1/whyqd/models/action_schema.py`

 * *Files identical despite different names*

### Comparing `whyqd-1.0.0/whyqd/models/actionscript.py` & `whyqd-1.0.1/whyqd/models/actionscript.py`

 * *Files identical despite different names*

### Comparing `whyqd-1.0.0/whyqd/models/category.py` & `whyqd-1.0.1/whyqd/models/category.py`

 * *Files identical despite different names*

### Comparing `whyqd-1.0.0/whyqd/models/citation.py` & `whyqd-1.0.1/whyqd/models/citation.py`

 * *Files identical despite different names*

### Comparing `whyqd-1.0.0/whyqd/models/column.py` & `whyqd-1.0.1/whyqd/models/column.py`

 * *Files identical despite different names*

### Comparing `whyqd-1.0.0/whyqd/models/constraints.py` & `whyqd-1.0.1/whyqd/models/constraints.py`

 * *Files identical despite different names*

### Comparing `whyqd-1.0.0/whyqd/models/crosswalk.py` & `whyqd-1.0.1/whyqd/models/crosswalk.py`

 * *Files identical despite different names*

### Comparing `whyqd-1.0.0/whyqd/models/datasource.py` & `whyqd-1.0.1/whyqd/models/datasource.py`

 * *Files identical despite different names*

### Comparing `whyqd-1.0.0/whyqd/models/fields.py` & `whyqd-1.0.1/whyqd/models/fields.py`

 * *Files identical despite different names*

### Comparing `whyqd-1.0.0/whyqd/models/modifier.py` & `whyqd-1.0.1/whyqd/models/modifier.py`

 * *Files identical despite different names*

### Comparing `whyqd-1.0.0/whyqd/models/schema.py` & `whyqd-1.0.1/whyqd/models/schema.py`

 * *Files identical despite different names*

### Comparing `whyqd-1.0.0/whyqd/models/transform.py` & `whyqd-1.0.1/whyqd/models/transform.py`

 * *Files identical despite different names*

### Comparing `whyqd-1.0.0/whyqd/models/version.py` & `whyqd-1.0.1/whyqd/models/version.py`

 * *Files identical despite different names*

### Comparing `whyqd-1.0.0/whyqd/parsers/action.py` & `whyqd-1.0.1/whyqd/parsers/action.py`

 * *Files identical despite different names*

### Comparing `whyqd-1.0.0/whyqd/parsers/category.py` & `whyqd-1.0.1/whyqd/parsers/category.py`

 * *Files identical despite different names*

### Comparing `whyqd-1.0.0/whyqd/parsers/core.py` & `whyqd-1.0.1/whyqd/parsers/core.py`

 * *Files 3% similar despite different names*

```diff
@@ -2,14 +2,16 @@
 from typing import TYPE_CHECKING
 from pydantic import Json
 import json
 import sys
 import hashlib
 from urllib.parse import urlparse
 import urllib
+import posixpath
+from uuid import uuid4
 from datetime import date, datetime
 from pathlib import Path, PurePath
 import modin.pandas as pd
 
 # from pandas.util import hash_pandas_object
 import locale
 import randomname
@@ -157,14 +159,21 @@
         Returns
         -------
         Path to local source.
         """
         request = urllib.request.Request(source, method="HEAD")
         request = urllib.request.urlopen(request).info()
         filename = request.get_filename()
+        if not filename:
+            #  https://stackoverflow.com/a/11783319/295606
+            source_path = urllib.request.urlsplit(source).path
+            filename = posixpath.basename(source_path)
+        if not filename:
+            # Make something up ...
+            filename = f"temporary-{uuid4()}"
         if not directory:
             directory = self.default_directory
         local_source = Path(directory) / filename
         if not self.check_source(source=local_source):
             urllib.request.urlretrieve(source, local_source)
         return local_source
```

### Comparing `whyqd-1.0.0/whyqd/parsers/datasource.py` & `whyqd-1.0.1/whyqd/parsers/datasource.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,16 @@
 from __future__ import annotations
 from typing import List, Union, Type, TYPE_CHECKING
 from pathlib import Path
 from datetime import date, datetime
 import pandas as _pd
 import modin.pandas as pd
 import numpy as np
+from pyarrow.parquet import ParquetFile
+import pyarrow as pa
 import re
 import locale
 import ast
 
 from whyqd.parsers.core import CoreParser
 from whyqd.models import ColumnModel, DataSourceModel, DataSourceAttributeModel
 from whyqd.dtypes import MimeType, FieldType
@@ -71,16 +73,22 @@
         else:
             kwargs["iterator"] = True
             kwargs["chunksize"] = 10000
             df_iterator = pd.read_csv(source, **kwargs)
             df = pd.concat(df_iterator, ignore_index=True)
         return df
 
-    def read_parquet(self, *, source: str | Path, **kwargs) -> pd.DataFrame:
+    def read_parquet(self, *, source: str | Path, nrows: int | None = None, **kwargs) -> pd.DataFrame:
         # https://pandas.pydata.org/docs/reference/api/pandas.read_parquet.html
+        if nrows:
+            # https://stackoverflow.com/a/69888274/295606
+            pf = ParquetFile(str(source))
+            pf = next(pf.iter_batches(batch_size=nrows))
+            # https://arrow.apache.org/docs/python/generated/pyarrow.Table.html#pyarrow.Table.to_pandas
+            return pa.Table.from_batches([pf]).to_pandas(**kwargs)
         ray_start()
         if "engine" not in kwargs:
             kwargs["engine"] = "pyarrow"
         return pd.read_parquet(source, **kwargs)
 
     def read_feather(self, *, source: str | Path, **kwargs) -> pd.DataFrame:
         # https://pandas.pydata.org/docs/reference/api/pandas.read_feather.html
@@ -157,15 +165,15 @@
             source = self.core.download_uri_source(source=source, directory=directory)
         if not self.core.check_source(source=source):
             e = f"Source at `{source}` not found."
             raise FileNotFoundError(e)
         # These, currently, don't accept any additional parameters.
         mimetype = self.get_mimetype(mimetype=mimetype)
         if mimetype in [MimeType.PRQ, MimeType.PARQUET]:
-            return self.read_parquet(source=source, **kwargs)
+            return self.read_parquet(source=source, nrows=nrows, **kwargs)
         if mimetype in [MimeType.FTR, MimeType.FEATHER]:
             return self.read_feather(source=source, **kwargs)
         # If the dtypes have not been set, then ensure that any provided preserved columns remain untouched
         # i.e. no forcing of text to numbers
         # defaulting to `dtype = object` ...
         if preserve:
             if isinstance(preserve, bool):
```

### Comparing `whyqd-1.0.0/whyqd/parsers/morph.py` & `whyqd-1.0.1/whyqd/parsers/morph.py`

 * *Files identical despite different names*

### Comparing `whyqd-1.0.0/whyqd/parsers/script.py` & `whyqd-1.0.1/whyqd/parsers/script.py`

 * *Files identical despite different names*

### Comparing `whyqd-1.0.0/setup.py` & `whyqd-1.0.1/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -28,17 +28,17 @@
  'ray>=2.2.0,<3.0.0',
  'setuptools>=67.7.2,<68.0.0',
  'tabulate>=0.8.9,<0.9.0',
  'xlrd>=2.0.1,<3.0.0']
 
 setup_kwargs = {
     'name': 'whyqd',
-    'version': '1.0.0',
+    'version': '1.0.1',
     'description': 'data wrangling simplicity, complete audit transparency, and at speed',
-    'long_description': '# whyqd: simplicity, transparency, speed\n\n[![Documentation Status](https://readthedocs.org/projects/whyqd/badge/?version=latest)](https://whyqd.readthedocs.io/en/latest/?badge=latest)\n[![Build Status](https://travis-ci.com/whythawk/whyqd.svg?branch=master)](https://travis-ci.com/whythawk/whyqd.svg?branch=master)\n[![DOI](https://zenodo.org/badge/239159569.svg)](https://zenodo.org/badge/latestdoi/239159569)\n\n## What is it?\n\n> More research, less wrangling\n\n[**whyqd**](https://whyqd.com) (/wɪkɪd/) is a curatorial toolkit intended to produce well-structured and predictable \ndata for research analysis.\n\nIt provides an intuitive method creating schema-to-schema crosswalks for restructuring messy data to conform to a \nstandardised metadata schema. It supports rapid and continuous transformation of messy data using a simple series of \nsteps. Once complete, you can import wrangled data into more complex analytical or database systems.\n\n**whyqd** plays well with your existing Python-based data-analytical tools. It uses [Ray](https://www.ray.io/) and \n[Modin](https://modin.readthedocs.io/) as a drop-in replacement for [Pandas](https://pandas.pydata.org/) to support \nprocessing of large datasets, and [Pydantic](https://pydantic-docs.helpmanual.io/) for data models. \n\nEach definition is saved as [JSON Schema-compliant](https://json-schema.org/) file. This permits others to read and \nscrutinise your approach, validate your methodology, or even use your crosswalks to import and transform data in \nproduction.\n\nOnce complete, a transform file can be shared, along with your input data, and anyone can import and validate your \ncrosswalk to verify that your output data is the product of these inputs.\n\n## Why use it?\n\nIf all you want to do is test whether your source data are even useful, spending days or weeks slogging through data \nrestructuring could kill a project. If you already have a workflow and established software which includes Python and \npandas, having to change your code every time your source data changes is really, really frustrating.\n\nIf you want to go from a [Cthulhu dataset](https://whyqd.readthedocs.io/tutorials/tutorial3) like this:\n\n![UNDP Human Development Index 2007-2008: a beautiful example of messy data.](https://raw.githubusercontent.com/whythawk/whyqd/master/docs/images/undp-hdi-2007-8.jpg)\n\n*UNDP Human Development Index 2007-2008: a beautiful example of messy data.*\n\nTo this:\n\n|    | country_name           | indicator_name   | reference   |   year |   values |\n|:---|:-----------------------|:-----------------|:------------|:-------|:---------|\n|  0 | Hong Kong, China (SAR) | HDI rank         | e           |   2008 |       21 |\n|  1 | Singapore              | HDI rank         | nan         |   2008 |       25 |\n|  2 | Korea (Republic of)    | HDI rank         | nan         |   2008 |       26 |\n|  3 | Cyprus                 | HDI rank         | nan         |   2008 |       28 |\n|  4 | Brunei Darussalam      | HDI rank         | nan         |   2008 |       30 |\n|  5 | Barbados               | HDI rank         | e,g,f       |   2008 |       31 |\n\nWith a readable set of scripts to ensure that your process can be audited and repeated:\n\n```python\nschema_scripts = [\n    f"UNITE > \'reference\' < {REFERENCE_COLUMNS}",\n    "RENAME > \'country_name\' < [\'Country\']",\n    "PIVOT_LONGER > [\'indicator_name\', \'values\'] < [\'HDI rank\', \'HDI Category\', \'Human poverty index (HPI-1) - Rank;;2008\', \'Human poverty index (HPI-1) - Value (%);;2008\', \'Probability at birth of not surviving to age 40 (% of cohort);;2000-05\', \'Adult illiteracy rate (% aged 15 and older);;1995-2005\', \'Population not using an improved water source (%);;2004\', \'Children under weight for age (% under age 5);;1996-2005\', \'Population below income poverty line (%) - $1 a day;;1990-2005\', \'Population below income poverty line (%) - $2 a day;;1990-2005\', \'Population below income poverty line (%) - National poverty line;;1990-2004\', \'HPI-1 rank minus income poverty rank;;2008\']",\n    "SEPARATE > [\'indicator_name\', \'year\'] < \';;\'::[\'indicator_name\']",\n    "DEBLANK",\n    "DEDUPE",\n]\n```\n\n## How does it work?\n\n> Crosswalks are mappings of the relationships between fields defined in different metadata \n> [schemas](https://whyqd.readthedocs.io/strategies/schema). Ideally, these are one-to-one, where a field in \n> one has an exact match in the other. In practice, it\'s more complicated than that.\n\nYour workflow is:\n\n1. Define a single destination schema,\n2. Derive a source schema from a data source,\n3. Review your source data structure,\n4. Develop a crosswalk to define the relationship between source and destination,\n5. Transform and validate your outputs,\n6. Share your output data, transform definitions, and a citation.\n\nIt starts like this:\n\n```python\nimport whyqd as qd\n```\n\n[Install](https://whyqd.readthedocs.io/installation) and [get started](https://whyqd.readthedocs.io/quickstart).\n\nThere are three worked tutorials to guide you through three typical scenarios:\n\n- [Aligning multiple data disparate sources to a single schema](https://whyqd.readthedocs.io/tutorials/tutorial1)\n- [Pivoting wide-format data into archival long-format](https://whyqd.readthedocs.io/tutorials/tutorial2)\n- [Wrangling Cthulhu data without losing your mind](https://whyqd.readthedocs.io/tutorials/tutorial3)\n\n## Installation\n\nYou\'ll need at least Python 3.8, then install with your favourite package manager:\n\n```bash\npip install whyqd\n```\n\nTo derive a source schema from tabular data, import from `DATASOURCE_PATH`, define its `MIMETYPE`, and derive a schema:\n\n```python\nimport whyqd as qd\n\ndatasource = qd.DataSourceDefinition()\ndatasource.derive_model(source=DATASOURCE_PATH, mimetype=MIMETYPE)\nschema_source = qd.SchemaDefinition()\nschema_source.derive_model(data=datasource.get)\nschema_source.fields.set_categories(name=CATEGORY_FIELD, \n                                    terms=datasource.get_data())\nschema_source.save()\n```\n\n[Get started...](https://whyqd.readthedocs.io/quickstart)\n\n## Changelog\n\nThe version history can be found in the [changelog](https://whyqd.readthedocs.io/changelog).\n\n## Background and funding\n\n**whyqd** was created to serve a continuous data wrangling process, including collaboration on more complex messy \nsources, ensuring the integrity of the source data, and producing a complete audit trail from data imported to our \ndatabase, back to source. You can see the product of that at [openLocal.uk](https://openlocal.uk).\n\n**whyqd** [received initial funding](https://eoscfuture-grants.eu/meet-the-grantees/implementation-no-code-method-schema-schema-data-transformations-interoperability)\nfrom the European Union\'s Horizon 2020 research and innovation programme under grant agreement No 101017536. Technical \ndevelopment support is from [EOSC Future](https://eoscfuture.eu/) through the \n[RDA Open Call mechanism](https://eoscfuture-grants.eu/provider/research-data-alliance), based on evaluations of \nexternal, independent experts.\n\nThe \'backronym\' for **whyqd** /wɪkɪd/ is *Whythawk Quantitative Data*, [Whythawk](https://whythawk.com)\nis an open data science and open research technical consultancy.\n\n## Licence\n\nThe [**whyqd** Python distribution](https://github.com/whythawk/whyqd) is licensed under the terms of the \n[BSD 3-Clause license](https://github.com/whythawk/whyqd/blob/master/LICENSE). All documentation is released under \n[Attribution 4.0 International (CC BY 4.0)](https://creativecommons.org/licenses/by/4.0/). **whyqd** tradenames and \nmarks are copyright [Whythawk](https://whythawk.com).\n',
+    'long_description': '# whyqd: simplicity, transparency, speed\n\n[![Documentation Status](https://readthedocs.org/projects/whyqd/badge/?version=latest)](docs/en/latest/?badge=latest)\n[![Build Status](https://travis-ci.com/whythawk/whyqd.svg?branch=master)](https://travis-ci.com/whythawk/whyqd.svg?branch=master)\n[![DOI](https://zenodo.org/badge/239159569.svg)](https://zenodo.org/badge/latestdoi/239159569)\n\n## What is it?\n\n> More research, less wrangling\n\n[**whyqd**](https://whyqd.com) (/wɪkɪd/) is a curatorial toolkit intended to produce well-structured and predictable \ndata for research analysis.\n\nIt provides an intuitive method for creating schema-to-schema crosswalks for restructuring messy data to conform to a \nstandardised metadata schema. It supports rapid and continuous transformation of messy data using a simple series of \nsteps. Once complete, you can import wrangled data into more complex analytical or database systems.\n\n**whyqd** plays well with your existing Python-based data-analytical tools. It uses [Ray](https://www.ray.io/) and \n[Modin](https://modin.readthedocs.io/) as a drop-in replacement for [Pandas](https://pandas.pydata.org/) to support \nprocessing of large datasets, and [Pydantic](https://pydantic-docs.helpmanual.io/) for data models. \n\nEach definition is saved as [JSON Schema-compliant](https://json-schema.org/) file. This permits others to read and \nscrutinise your approach, validate your methodology, or even use your crosswalks to import and transform data in \nproduction.\n\nOnce complete, a transform file can be shared, along with your input data, and anyone can import and validate your \ncrosswalk to verify that your output data is the product of these inputs.\n\n## Why use it?\n\n**whyqd** allows you to get to work without requiring you to achieve buy-in from anyone or change your existing code.\n\nIf you don\'t want to spend days or weeks slogging through data when all you want to do is test whether your source \ndata are even useful. If you already have a workflow and established software which includes Python and pandas, and \ndon\'t want to change your code every time your source data changes.\n\nIf you want to go from a [Cthulhu dataset](https://whyqd.readthedocs.io/en/latest/tutorials/tutorial3) like this:\n\n![UNDP Human Development Index 2007-2008: a beautiful example of messy data.](docs/images/undp-hdi-2007-8.jpg)\n*UNDP Human Development Index 2007-2008: a beautiful example of messy data.*\n\nTo this:\n\n|    | country_name           | indicator_name   | reference   |   year |   values |\n|:---|:-----------------------|:-----------------|:------------|:-------|:---------|\n|  0 | Hong Kong, China (SAR) | HDI rank         | e           |   2008 |       21 |\n|  1 | Singapore              | HDI rank         | nan         |   2008 |       25 |\n|  2 | Korea (Republic of)    | HDI rank         | nan         |   2008 |       26 |\n|  3 | Cyprus                 | HDI rank         | nan         |   2008 |       28 |\n|  4 | Brunei Darussalam      | HDI rank         | nan         |   2008 |       30 |\n|  5 | Barbados               | HDI rank         | e,g,f       |   2008 |       31 |\n\nWith a readable set of scripts to ensure that your process can be audited and repeated:\n\n```python\nschema_scripts = [\n    f"UNITE > \'reference\' < {REFERENCE_COLUMNS}",\n    "RENAME > \'country_name\' < [\'Country\']",\n    "PIVOT_LONGER > [\'indicator_name\', \'values\'] < [\'HDI rank\', \'HDI Category\', \'Human poverty index (HPI-1) - Rank;;2008\', \'Human poverty index (HPI-1) - Value (%);;2008\', \'Probability at birth of not surviving to age 40 (% of cohort);;2000-05\', \'Adult illiteracy rate (% aged 15 and older);;1995-2005\', \'Population not using an improved water source (%);;2004\', \'Children under weight for age (% under age 5);;1996-2005\', \'Population below income poverty line (%) - $1 a day;;1990-2005\', \'Population below income poverty line (%) - $2 a day;;1990-2005\', \'Population below income poverty line (%) - National poverty line;;1990-2004\', \'HPI-1 rank minus income poverty rank;;2008\']",\n    "SEPARATE > [\'indicator_name\', \'year\'] < \';;\'::[\'indicator_name\']",\n    "DEBLANK",\n    "DEDUPE",\n]\n```\n\nThen **whyqd** may be for you.\n\n## How does it work?\n\n> Crosswalks are mappings of the relationships between fields defined in different metadata \n> [schemas](https://whyqd.readthedocs.io/en/latest/strategies/schema). Ideally, these are one-to-one, where a field in \n> one has an exact match in the other. In practice, it\'s more complicated than that.\n\nYour workflow is:\n\n1. Define a single destination schema,\n2. Derive a source schema from a data source,\n3. Review your source data structure,\n4. Develop a crosswalk to define the relationship between source and destination,\n5. Transform and validate your outputs,\n6. Share your output data, transform definitions, and a citation.\n\nIt starts like this:\n\n```python\nimport whyqd as qd\n```\n\n[Install](https://whyqd.readthedocs.io/en/latest/installation) and then read the [quickstart](https://whyqd.readthedocs.io/en/latest/quickstart).\n\nThere are three worked tutorials to guide you through three typical scenarios:\n\n- [Aligning multiple disparate data sources to a single schema](https://whyqd.readthedocs.io/en/latest/tutorials/tutorial1)\n- [Pivoting wide-format data into archival long-format](https://whyqd.readthedocs.io/en/latest/tutorials/tutorial2)\n- [Wrangling Cthulhu data without losing your mind](https://whyqd.readthedocs.io/en/latest/tutorials/tutorial3)\n\n## Installation\n\nYou\'ll need at least Python 3.8, then install with your favourite package manager:\n\n```bash\npip install whyqd\n```\n\nTo derive a source schema from tabular data, import from `DATASOURCE_PATH`, define its `MIMETYPE`, and derive a schema:\n\n```python\nimport whyqd as qd\n\ndatasource = qd.DataSourceDefinition()\ndatasource.derive_model(source=DATASOURCE_PATH, mimetype=MIMETYPE)\nschema_source = qd.SchemaDefinition()\nschema_source.derive_model(data=datasource.get)\nschema_source.fields.set_categories(name=CATEGORY_FIELD, \n                                    terms=datasource.get_data())\nschema_source.save()\n```\n\n[Get started...](https://whyqd.readthedocs.io/en/latest/quickstart)\n\n## Changelog\n\nThe version history can be found in the [changelog](https://whyqd.readthedocs.io/en/latest/changelog).\n\n## Background and funding\n\n**whyqd** was created to serve a continuous data wrangling process, including collaboration on more complex messy \nsources, ensuring the integrity of the source data, and producing a complete audit trail from data imported to our \ndatabase, back to source. You can see the product of that at [openLocal.uk](https://openlocal.uk).\n\n**whyqd** [received initial funding](https://eoscfuture-grants.eu/meet-the-grantees/implementation-no-code-method-schema-schema-data-transformations-interoperability)\nfrom the European Union\'s Horizon 2020 research and innovation programme under grant agreement No 101017536. Technical \ndevelopment support is from [EOSC Future](https://eoscfuture.eu/) through the \n[RDA Open Call mechanism](https://eoscfuture-grants.eu/provider/research-data-alliance), based on evaluations of \nexternal, independent experts.\n\nThe \'backronym\' for **whyqd** /wɪkɪd/ is *Whythawk Quantitative Data*, [Whythawk](https://whythawk.com)\nis an open data science and open research technical consultancy.\n\n## Licence\n\nThe [**whyqd** Python distribution](https://github.com/whythawk/whyqd) is licensed under the terms of the \n[BSD 3-Clause license](https://github.com/whythawk/whyqd/blob/master/LICENSE). All documentation is released under \n[Attribution 4.0 International (CC BY 4.0)](https://creativecommons.org/licenses/by/4.0/). **whyqd** tradenames and \nmarks are copyright [Whythawk](https://whythawk.com).\n',
     'author': 'Gavin Chait',
     'author_email': 'gchait@whythawk.com',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'https://whyqd.com',
     'packages': packages,
     'package_data': package_data,
```

### Comparing `whyqd-1.0.0/PKG-INFO` & `whyqd-1.0.1/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: whyqd
-Version: 1.0.0
+Version: 1.0.1
 Summary: data wrangling simplicity, complete audit transparency, and at speed
 Home-page: https://whyqd.com
 License: BSD-3-Clause
 Keywords: python,data-science,pandas,open-data,open-science,data-analysis,data-wrangling,data-management,munging,crosswalks
 Author: Gavin Chait
 Author-email: gchait@whythawk.com
 Requires-Python: >=3.8.1,<4.0
@@ -35,26 +35,26 @@
 Requires-Dist: xlrd (>=2.0.1,<3.0.0)
 Project-URL: Documentation, https://whyqd.readthedocs.io/
 Project-URL: Repository, https://github.com/whythawk/whyqd/
 Description-Content-Type: text/markdown
 
 # whyqd: simplicity, transparency, speed
 
-[![Documentation Status](https://readthedocs.org/projects/whyqd/badge/?version=latest)](https://whyqd.readthedocs.io/en/latest/?badge=latest)
+[![Documentation Status](https://readthedocs.org/projects/whyqd/badge/?version=latest)](docs/en/latest/?badge=latest)
 [![Build Status](https://travis-ci.com/whythawk/whyqd.svg?branch=master)](https://travis-ci.com/whythawk/whyqd.svg?branch=master)
 [![DOI](https://zenodo.org/badge/239159569.svg)](https://zenodo.org/badge/latestdoi/239159569)
 
 ## What is it?
 
 > More research, less wrangling
 
 [**whyqd**](https://whyqd.com) (/wɪkɪd/) is a curatorial toolkit intended to produce well-structured and predictable 
 data for research analysis.
 
-It provides an intuitive method creating schema-to-schema crosswalks for restructuring messy data to conform to a 
+It provides an intuitive method for creating schema-to-schema crosswalks for restructuring messy data to conform to a 
 standardised metadata schema. It supports rapid and continuous transformation of messy data using a simple series of 
 steps. Once complete, you can import wrangled data into more complex analytical or database systems.
 
 **whyqd** plays well with your existing Python-based data-analytical tools. It uses [Ray](https://www.ray.io/) and 
 [Modin](https://modin.readthedocs.io/) as a drop-in replacement for [Pandas](https://pandas.pydata.org/) to support 
 processing of large datasets, and [Pydantic](https://pydantic-docs.helpmanual.io/) for data models. 
 
@@ -63,22 +63,23 @@
 production.
 
 Once complete, a transform file can be shared, along with your input data, and anyone can import and validate your 
 crosswalk to verify that your output data is the product of these inputs.
 
 ## Why use it?
 
-If all you want to do is test whether your source data are even useful, spending days or weeks slogging through data 
-restructuring could kill a project. If you already have a workflow and established software which includes Python and 
-pandas, having to change your code every time your source data changes is really, really frustrating.
+**whyqd** allows you to get to work without requiring you to achieve buy-in from anyone or change your existing code.
 
-If you want to go from a [Cthulhu dataset](https://whyqd.readthedocs.io/tutorials/tutorial3) like this:
+If you don't want to spend days or weeks slogging through data when all you want to do is test whether your source 
+data are even useful. If you already have a workflow and established software which includes Python and pandas, and 
+don't want to change your code every time your source data changes.
 
-![UNDP Human Development Index 2007-2008: a beautiful example of messy data.](https://raw.githubusercontent.com/whythawk/whyqd/master/docs/images/undp-hdi-2007-8.jpg)
+If you want to go from a [Cthulhu dataset](https://whyqd.readthedocs.io/en/latest/tutorials/tutorial3) like this:
 
+![UNDP Human Development Index 2007-2008: a beautiful example of messy data.](docs/images/undp-hdi-2007-8.jpg)
 *UNDP Human Development Index 2007-2008: a beautiful example of messy data.*
 
 To this:
 
 |    | country_name           | indicator_name   | reference   |   year |   values |
 |:---|:-----------------------|:-----------------|:------------|:-------|:---------|
 |  0 | Hong Kong, China (SAR) | HDI rank         | e           |   2008 |       21 |
@@ -97,18 +98,20 @@
     "PIVOT_LONGER > ['indicator_name', 'values'] < ['HDI rank', 'HDI Category', 'Human poverty index (HPI-1) - Rank;;2008', 'Human poverty index (HPI-1) - Value (%);;2008', 'Probability at birth of not surviving to age 40 (% of cohort);;2000-05', 'Adult illiteracy rate (% aged 15 and older);;1995-2005', 'Population not using an improved water source (%);;2004', 'Children under weight for age (% under age 5);;1996-2005', 'Population below income poverty line (%) - $1 a day;;1990-2005', 'Population below income poverty line (%) - $2 a day;;1990-2005', 'Population below income poverty line (%) - National poverty line;;1990-2004', 'HPI-1 rank minus income poverty rank;;2008']",
     "SEPARATE > ['indicator_name', 'year'] < ';;'::['indicator_name']",
     "DEBLANK",
     "DEDUPE",
 ]
 ```
 
+Then **whyqd** may be for you.
+
 ## How does it work?
 
 > Crosswalks are mappings of the relationships between fields defined in different metadata 
-> [schemas](https://whyqd.readthedocs.io/strategies/schema). Ideally, these are one-to-one, where a field in 
+> [schemas](https://whyqd.readthedocs.io/en/latest/strategies/schema). Ideally, these are one-to-one, where a field in 
 > one has an exact match in the other. In practice, it's more complicated than that.
 
 Your workflow is:
 
 1. Define a single destination schema,
 2. Derive a source schema from a data source,
 3. Review your source data structure,
@@ -118,21 +121,21 @@
 
 It starts like this:
 
 ```python
 import whyqd as qd
 ```
 
-[Install](https://whyqd.readthedocs.io/installation) and [get started](https://whyqd.readthedocs.io/quickstart).
+[Install](https://whyqd.readthedocs.io/en/latest/installation) and then read the [quickstart](https://whyqd.readthedocs.io/en/latest/quickstart).
 
 There are three worked tutorials to guide you through three typical scenarios:
 
-- [Aligning multiple data disparate sources to a single schema](https://whyqd.readthedocs.io/tutorials/tutorial1)
-- [Pivoting wide-format data into archival long-format](https://whyqd.readthedocs.io/tutorials/tutorial2)
-- [Wrangling Cthulhu data without losing your mind](https://whyqd.readthedocs.io/tutorials/tutorial3)
+- [Aligning multiple disparate data sources to a single schema](https://whyqd.readthedocs.io/en/latest/tutorials/tutorial1)
+- [Pivoting wide-format data into archival long-format](https://whyqd.readthedocs.io/en/latest/tutorials/tutorial2)
+- [Wrangling Cthulhu data without losing your mind](https://whyqd.readthedocs.io/en/latest/tutorials/tutorial3)
 
 ## Installation
 
 You'll need at least Python 3.8, then install with your favourite package manager:
 
 ```bash
 pip install whyqd
@@ -148,19 +151,19 @@
 schema_source = qd.SchemaDefinition()
 schema_source.derive_model(data=datasource.get)
 schema_source.fields.set_categories(name=CATEGORY_FIELD, 
                                     terms=datasource.get_data())
 schema_source.save()
 ```
 
-[Get started...](https://whyqd.readthedocs.io/quickstart)
+[Get started...](https://whyqd.readthedocs.io/en/latest/quickstart)
 
 ## Changelog
 
-The version history can be found in the [changelog](https://whyqd.readthedocs.io/changelog).
+The version history can be found in the [changelog](https://whyqd.readthedocs.io/en/latest/changelog).
 
 ## Background and funding
 
 **whyqd** was created to serve a continuous data wrangling process, including collaboration on more complex messy 
 sources, ensuring the integrity of the source data, and producing a complete audit trail from data imported to our 
 database, back to source. You can see the product of that at [openLocal.uk](https://openlocal.uk).
```

