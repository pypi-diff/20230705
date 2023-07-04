# Comparing `tmp/population_trend-3.0.0.tar.gz` & `tmp/population_trend-3.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "population_trend-3.0.0.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
+gzip compressed data, was "population_trend-3.1.0.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `population_trend-3.0.0.tar` & `population_trend-3.1.0.tar`

### file list

```diff
@@ -1,7 +1,8 @@
--rw-r--r--   0        0        0     1037 2023-07-04 00:00:06.907205 population_trend-3.0.0/README.md
--rw-r--r--   0        0        0      163 2023-07-04 00:00:06.907205 population_trend-3.0.0/population_trend/__init__.py
--rw-r--r--   0        0        0     1894 2023-07-04 00:00:06.907205 population_trend-3.0.0/population_trend/cli.py
--rw-r--r--   0        0        0      403 2023-07-04 00:00:06.907205 population_trend-3.0.0/population_trend/filter_data.py
--rw-r--r--   0        0        0     4361 2023-07-04 00:00:06.907205 population_trend-3.0.0/population_trend/population_growth_model.py
--rw-r--r--   0        0        0      495 2023-07-04 00:00:06.907205 population_trend-3.0.0/pyproject.toml
--rw-r--r--   0        0        0     1504 1970-01-01 00:00:00.000000 population_trend-3.0.0/PKG-INFO
+-rw-r--r--   0        0        0     1037 2023-07-04 23:17:38.042354 population_trend-3.1.0/README.md
+-rw-r--r--   0        0        0      251 2023-07-04 23:17:38.042354 population_trend-3.1.0/population_trend/__init__.py
+-rw-r--r--   0        0        0     6901 2023-07-04 23:17:38.042354 population_trend-3.1.0/population_trend/calculate_growth_rates.py
+-rw-r--r--   0        0        0     1894 2023-07-04 23:17:38.042354 population_trend-3.1.0/population_trend/cli.py
+-rw-r--r--   0        0        0      403 2023-07-04 23:17:38.042354 population_trend-3.1.0/population_trend/filter_data.py
+-rw-r--r--   0        0        0     4361 2023-07-04 23:17:38.042354 population_trend-3.1.0/population_trend/population_growth_model.py
+-rw-r--r--   0        0        0      495 2023-07-04 23:17:38.042354 population_trend-3.1.0/pyproject.toml
+-rw-r--r--   0        0        0     1504 1970-01-01 00:00:00.000000 population_trend-3.1.0/PKG-INFO
```

### Comparing `population_trend-3.0.0/README.md` & `population_trend-3.1.0/README.md`

 * *Files identical despite different names*

### Comparing `population_trend-3.0.0/population_trend/cli.py` & `population_trend-3.1.0/population_trend/cli.py`

 * *Files identical despite different names*

### Comparing `population_trend-3.0.0/population_trend/population_growth_model.py` & `population_trend-3.1.0/population_trend/population_growth_model.py`

 * *Files identical despite different names*

### Comparing `population_trend-3.0.0/PKG-INFO` & `population_trend-3.1.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 Metadata-Version: 2.1
 Name: population_trend
-Version: 3.0.0
+Version: 3.1.0
 Summary: A template Python module
 Home-page: https://github.com/IslasGECI/population_trend
 Author: Ciencia de Datos • GECI
 Author-email: ciencia.datos@islas.org.mx
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
-Requires-Dist: bootstrapping-tools==1.1.1
+Requires-Dist: bootstrapping-tools==2.0.0
 Requires-Dist: geci-plots
 Requires-Dist: typer
 
 <a href="https://www.islas.org.mx/"><img src="https://www.islas.org.mx/img/logo.svg" align="right" width="256" /></a>
 # Dummy Transformations
 
 Para usar este repo como plantilla debemos hacer lo siguiente:
```

#### html2text {}

```diff
@@ -1,13 +1,13 @@
-Metadata-Version: 2.1 Name: population_trend Version: 3.0.0 Summary: A template
+Metadata-Version: 2.1 Name: population_trend Version: 3.1.0 Summary: A template
 Python module Home-page: https://github.com/IslasGECI/population_trend Author:
 Ciencia de Datos â¢ GECI Author-email: ciencia.datos@islas.org.mx Requires-
 Python: >=3.9 Description-Content-Type: text/markdown Classifier: License ::
 OSI Approved :: GNU General Public License v3 or later (GPLv3+) Requires-Dist:
-bootstrapping-tools==1.1.1 Requires-Dist: geci-plots Requires-Dist: typer
+bootstrapping-tools==2.0.0 Requires-Dist: geci-plots Requires-Dist: typer
 [https://www.islas.org.mx/img/logo.svg] # Dummy Transformations Para usar este
 repo como plantilla debemos hacer lo siguiente: 1. Presiona el botÃ³n verde que
 dice _Use this template_ 1. Selecciona como dueÃ±o a la organizaciÃ³n IslasGECI
 1. Agrega el nombre del nuevo mÃ³dulo de python 1. Presiona el botÃ³n _Create
 repository from template_ 1. Reemplaza `dummy_transformations` por el nombre
 del nuevo mÃ³dulo en: - `Makefile` - `pyproject.toml` -
 `tests\test_transformations.py` 1. Renombra el archivo
```

