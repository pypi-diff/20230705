# Comparing `tmp/cumulus_library_covid-0.1.2.tar.gz` & `tmp/cumulus_library_covid-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cumulus_library_covid-0.1.2.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
+gzip compressed data, was "cumulus_library_covid-0.1.3.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `cumulus_library_covid-0.1.2.tar` & `cumulus_library_covid-0.1.3.tar`

### file list

```diff
@@ -1,17 +1,33 @@
--rw-r--r--   0        0        0     1062 2023-05-31 15:42:19.793235 cumulus_library_covid-0.1.2/README.md
--rw-r--r--   0        0        0        0 2023-05-31 15:42:19.793235 cumulus_library_covid-0.1.2/cumulus_library_covid/__init__.py
--rw-r--r--   0        0        0        0 2023-05-31 15:42:19.793235 cumulus_library_covid-0.1.2/cumulus_library_covid/covid_symptom/__init__.py
--rw-r--r--   0        0        0      551 2023-05-31 15:42:19.797235 cumulus_library_covid-0.1.2/cumulus_library_covid/covid_symptom/count_covid.py
--rw-r--r--   0        0        0     1237 2023-05-31 15:42:19.797235 cumulus_library_covid-0.1.2/cumulus_library_covid/covid_symptom/count_covid_dx.sql
--rw-r--r--   0        0        0     2387 2023-05-31 15:42:19.797235 cumulus_library_covid-0.1.2/cumulus_library_covid/covid_symptom/count_covid_pcr.sql
--rw-r--r--   0        0        0     2443 2023-05-31 15:42:19.797235 cumulus_library_covid-0.1.2/cumulus_library_covid/covid_symptom/count_covid_prevalence_ed.sql
--rw-r--r--   0        0        0     2329 2023-05-31 15:42:19.797235 cumulus_library_covid-0.1.2/cumulus_library_covid/covid_symptom/count_covid_study_period.sql
--rw-r--r--   0        0        0     3348 2023-05-31 15:42:19.797235 cumulus_library_covid-0.1.2/cumulus_library_covid/covid_symptom/count_covid_symptom.sql
--rw-r--r--   0        0        0     2522 2023-05-31 15:42:19.797235 cumulus_library_covid-0.1.2/cumulus_library_covid/covid_symptom/covid_define.py
--rw-r--r--   0        0        0     5029 2023-05-31 15:42:19.797235 cumulus_library_covid-0.1.2/cumulus_library_covid/covid_symptom/covid_define.sql
--rw-r--r--   0        0        0      737 2023-05-31 15:42:19.797235 cumulus_library_covid-0.1.2/cumulus_library_covid/covid_symptom/covid_define_symptom.py
--rw-r--r--   0        0        0    16063 2023-05-31 15:42:19.797235 cumulus_library_covid-0.1.2/cumulus_library_covid/covid_symptom/covid_define_symptom.sql
--rw-r--r--   0        0        0      617 2023-05-31 15:42:19.797235 cumulus_library_covid-0.1.2/cumulus_library_covid/covid_symptom/manifest.toml
--rw-r--r--   0        0        0     4917 2023-05-31 15:42:19.797235 cumulus_library_covid-0.1.2/cumulus_library_covid/covid_symptom/site_define.sql
--rw-r--r--   0        0        0     1099 2023-05-31 15:42:19.797235 cumulus_library_covid-0.1.2/pyproject.toml
--rw-r--r--   0        0        0     1917 1970-01-01 00:00:00.000000 cumulus_library_covid-0.1.2/PKG-INFO
+-rw-r--r--   0        0        0     1062 2023-05-30 20:14:21.539236 cumulus_library_covid-0.1.3/README.md
+-rw-r--r--   0        0        0        0 2023-05-30 20:14:21.539306 cumulus_library_covid-0.1.3/cumulus_library_covid/__init__.py
+-rw-r--r--   0        0        0        0 2023-05-30 20:14:21.539386 cumulus_library_covid-0.1.3/cumulus_library_covid/covid_symptom/__init__.py
+-rw-r--r--   0        0        0     3473 2023-07-05 20:21:01.776802 cumulus_library_covid-0.1.3/cumulus_library_covid/covid_symptom/count.py
+-rw-r--r--   0        0        0     4429 2023-07-05 20:21:01.777002 cumulus_library_covid-0.1.3/cumulus_library_covid/covid_symptom/count.sql
+-rw-r--r--   0        0        0     2678 2023-07-05 20:21:01.777174 cumulus_library_covid-0.1.3/cumulus_library_covid/covid_symptom/define_age_general.sql
+-rw-r--r--   0        0        0      600 2023-07-05 20:21:01.777331 cumulus_library_covid-0.1.3/cumulus_library_covid/covid_symptom/define_age_pediatric.sql
+-rw-r--r--   0        0        0      192 2023-07-05 20:21:01.777487 cumulus_library_covid-0.1.3/cumulus_library_covid/covid_symptom/define_dx_icd10.sql
+-rw-r--r--   0        0        0     4154 2023-07-05 20:21:01.777645 cumulus_library_covid-0.1.3/cumulus_library_covid/covid_symptom/define_dx_snomed.sql
+-rw-r--r--   0        0        0     1586 2023-07-05 20:21:01.777801 cumulus_library_covid-0.1.3/cumulus_library_covid/covid_symptom/define_ed_note.sql
+-rw-r--r--   0        0        0     8576 2023-07-05 20:21:01.777962 cumulus_library_covid-0.1.3/cumulus_library_covid/covid_symptom/define_pcr.sql
+-rw-r--r--   0        0        0     1522 2023-07-05 20:21:01.778121 cumulus_library_covid-0.1.3/cumulus_library_covid/covid_symptom/define_pcr_custom.sql
+-rw-r--r--   0        0        0     2022 2023-07-05 20:21:01.778280 cumulus_library_covid-0.1.3/cumulus_library_covid/covid_symptom/define_pcr_negative.sql
+-rw-r--r--   0        0        0     2747 2023-07-05 20:21:01.778440 cumulus_library_covid-0.1.3/cumulus_library_covid/covid_symptom/define_pcr_positive.sql
+-rw-r--r--   0        0        0      794 2023-07-05 19:43:06.938136 cumulus_library_covid-0.1.3/cumulus_library_covid/covid_symptom/define_study_period.sql
+-rw-r--r--   0        0        0      731 2023-07-05 19:43:06.938214 cumulus_library_covid-0.1.3/cumulus_library_covid/covid_symptom/define_symptom.py
+-rw-r--r--   0        0        0    16063 2023-07-05 19:43:06.938352 cumulus_library_covid-0.1.3/cumulus_library_covid/covid_symptom/define_symptom.sql
+-rw-r--r--   0        0        0     1115 2023-07-05 19:43:06.938524 cumulus_library_covid-0.1.3/cumulus_library_covid/covid_symptom/manifest.toml
+-rw-r--r--   0        0        0      864 2023-07-05 20:21:01.778747 cumulus_library_covid-0.1.3/cumulus_library_covid/covid_symptom/table_dx.sql
+-rw-r--r--   0        0        0     1569 2023-07-05 20:21:01.778943 cumulus_library_covid-0.1.3/cumulus_library_covid/covid_symptom/table_pcr.sql
+-rw-r--r--   0        0        0     1540 2023-07-05 19:43:06.939079 cumulus_library_covid-0.1.3/cumulus_library_covid/covid_symptom/table_prevalence_ed.sql
+-rw-r--r--   0        0        0     1031 2023-07-05 20:21:01.779138 cumulus_library_covid-0.1.3/cumulus_library_covid/covid_symptom/table_study_period.sql
+-rw-r--r--   0        0        0     2277 2023-07-05 20:21:01.779326 cumulus_library_covid-0.1.3/cumulus_library_covid/covid_symptom/table_symptom.sql
+-rw-r--r--   0        0        0     2522 2023-07-05 19:43:06.939445 cumulus_library_covid-0.1.3/cumulus_library_covid/covid_symptom/typesystem.py
+-rw-r--r--   0        0        0     1905 2023-07-05 19:43:06.939507 cumulus_library_covid-0.1.3/cumulus_library_covid/covid_symptom/valueset_dx_icd10.json
+-rw-r--r--   0        0        0     5415 2023-07-05 19:43:06.939562 cumulus_library_covid-0.1.3/cumulus_library_covid/covid_symptom/valueset_dx_snomed.json
+-rw-r--r--   0        0        0     3376 2023-07-05 19:43:06.939664 cumulus_library_covid-0.1.3/cumulus_library_covid/covid_symptom/valueset_pcr_interpretation.json
+-rw-r--r--   0        0        0     4037 2023-07-05 19:43:06.939753 cumulus_library_covid-0.1.3/cumulus_library_covid/covid_symptom/valueset_pcr_negative.json
+-rw-r--r--   0        0        0     4602 2023-07-05 19:43:06.939807 cumulus_library_covid-0.1.3/cumulus_library_covid/covid_symptom/valueset_pcr_positive.json
+-rw-r--r--   0        0        0     3369 2023-07-05 19:43:06.939974 cumulus_library_covid-0.1.3/cumulus_library_covid/covid_symptom/valueset_pcr_qualitative.json
+-rw-r--r--   0        0        0     8196 2023-07-05 19:43:06.940040 cumulus_library_covid-0.1.3/cumulus_library_covid/covid_symptom/valueset_pcr_qualitative_quantitative.json
+-rw-r--r--   0        0        0     1099 2023-07-05 20:27:29.283253 cumulus_library_covid-0.1.3/pyproject.toml
+-rw-r--r--   0        0        0     1917 1970-01-01 00:00:00.000000 cumulus_library_covid-0.1.3/PKG-INFO
```

### Comparing `cumulus_library_covid-0.1.2/README.md` & `cumulus_library_covid-0.1.3/README.md`

 * *Files identical despite different names*

### Comparing `cumulus_library_covid-0.1.2/cumulus_library_covid/covid_symptom/count_covid_dx.sql` & `cumulus_library_covid-0.1.3/cumulus_library_covid/covid_symptom/table_dx.sql`

 * *Files 18% similar despite different names*

```diff
@@ -1,50 +1,35 @@
 -- ############################################################################
 -- Table COVID19 Diagnosis
 
 CREATE TABLE covid_symptom__dx AS
+WITH define_dx AS (
+    SELECT
+        code,
+        system,
+        display
+    FROM covid_symptom__define_dx_icd10
+    UNION
+    SELECT
+        code,
+        system,
+        display
+    FROM covid_symptom__define_dx_snomed
+)
+
 SELECT DISTINCT
     c.subject_ref,
     c.encounter_ref,
     c.cond_code.coding[1].code AS cond_code, -- noqa: LT01,RF02
     c.recorded_week AS cond_week,
+    c.recorded_month AS cond_month,
+    c.recorded_year AS cond_year,
     s.enc_class_code,
     s.age_at_visit,
     s.ed_note,
     s.variant_era
 FROM core__condition AS c,
     covid_symptom__study_period AS s,
-    covid_symptom__define_dx AS dx
+    define_dx
 WHERE
-    c.cond_code.coding[1].code = dx.code -- noqa: LT01,RF02
+    c.cond_code.coding[1].code = define_dx.code -- noqa: LT01,RF02
     AND c.encounter_ref = s.encounter_ref;
-
-CREATE OR REPLACE VIEW covid_symptom__count_dx_week AS
-WITH powerset AS (
-    SELECT
-        count(DISTINCT subject_ref) AS cnt_subject,
-        count(DISTINCT encounter_ref) AS cnt_encounter,
-        cond_week,
-        enc_class_code,
-        age_at_visit,
-        ed_note,
-        variant_era
-    FROM covid_symptom__dx
-    GROUP BY
-        cube(
-            cond_week,
-            enc_class_code,
-            age_at_visit,
-            ed_note,
-            variant_era
-        )
-)
-
-SELECT
-    cnt_encounter AS cnt,
-    cond_week,
-    enc_class_code,
-    age_at_visit,
-    ed_note,
-    variant_era
-FROM powerset
-WHERE cnt_subject >= 10 ORDER BY cnt DESC;
```

### Comparing `cumulus_library_covid-0.1.2/cumulus_library_covid/covid_symptom/count_covid_pcr.sql` & `cumulus_library_covid-0.1.3/cumulus_library_covid/covid_symptom/table_pcr.sql`

 * *Files 27% similar despite different names*

```diff
@@ -1,18 +1,33 @@
 -- ############################################################################
 -- Table COVID19 PCR tests for COVID performed at the local hospital
--- **Likely does not include PCR tests from other healthcare settings**
---
--- Study Period: @core_study_period_covid
--- PCR Test Codes: @covid_define_pcr, @map_lab_code
 
 CREATE TABLE covid_symptom__pcr AS
+WITH obs_interpret AS (
+    SELECT
+        system,
+        code,
+        'Negative' AS display
+    FROM covid_symptom__define_pcr_negative
+    UNION
+    SELECT
+        system,
+        code,
+        'Positive' AS display
+    FROM covid_symptom__define_pcr_positive
+    UNION
+    SELECT
+        from_system,
+        from_code AS code,
+        display
+    FROM covid_symptom__define_pcr_custom
+)
+
 SELECT DISTINCT
-    upper(o.lab_result.display) AS covid_pcr_result_display,
-    o.lab_result AS covid_pcr_result,
+    obs_interpret.display AS covid_pcr_result_display,
     o.lab_code AS covid_pcr_code,
     o.lab_date AS covid_pcr_date,
     o.lab_week AS covid_pcr_week,
     o.lab_month AS covid_pcr_month,
     s.variant_era,
     s.author_date,
     s.author_week,
@@ -24,61 +39,20 @@
     s.age_at_visit,
     s.gender,
     s.race_display,
     o.subject_ref,
     o.encounter_ref,
     o.observation_ref
 FROM core__observation_lab AS o,
-    covid_symptom__define_pcr AS pcr,
     covid_symptom__define_period AS p,
-    covid_symptom__site_pcr,
-    covid_symptom__study_period AS s
+    covid_symptom__study_period AS s,
+    covid_symptom__define_pcr AS pcr,
+    obs_interpret
 WHERE
     (s.encounter_ref = o.encounter_ref)
     AND (s.variant_era = p.variant_era)
     AND (o.lab_week BETWEEN p.variant_start AND p.variant_end)
     AND (o.lab_code.code = pcr.code)
-    AND (o.lab_result.code IN (
-        '260385009', 'Negative', 'NEGATIVE',
-        '10828004', 'Positive', 'POSITIVE'
-    ));
+    AND (o.lab_result.code = obs_interpret.code);
 
--- ############################################################################
-
-
-CREATE OR REPLACE VIEW covid_symptom__count_pcr_week AS
-WITH powerset AS (
-    SELECT
-        count(DISTINCT cp.subject_ref) AS cnt_subject,
-        count(DISTINCT cp.encounter_ref) AS cnt_encounter,
-        upper(covid_pcr_result.display) AS covid_pcr_result_display,
-        cp.covid_pcr_week,
-        cp.variant_era,
-        cp.ed_note,
-        cp.age_at_visit,
-        cp.gender,
-        cp.race_display
-    FROM covid_symptom__pcr AS cp
-    GROUP BY
-        cube(
-            cp.covid_pcr_result,
-            cp.covid_pcr_week,
-            cp.variant_era,
-            cp.ed_note,
-            cp.age_at_visit,
-            cp.gender,
-            cp.race_display
-        )
-)
-
-SELECT DISTINCT
-    cnt_encounter AS cnt,
-    covid_pcr_result_display,
-    covid_pcr_week,
-    variant_era,
-    ed_note,
-    age_at_visit,
-    gender,
-    race_display
-FROM powerset
-WHERE cnt_subject >= 10
-ORDER BY covid_pcr_week ASC, covid_pcr_result_display ASC;
+-- TODO Cerner specific handling of lab RESULT
+-- https://github.com/smart-on-fhir/cumulus-library-covid/issues/13
```

### Comparing `cumulus_library_covid-0.1.2/cumulus_library_covid/covid_symptom/covid_define.py` & `cumulus_library_covid-0.1.3/cumulus_library_covid/covid_symptom/typesystem.py`

 * *Files identical despite different names*

### Comparing `cumulus_library_covid-0.1.2/cumulus_library_covid/covid_symptom/covid_define_symptom.py` & `cumulus_library_covid-0.1.3/cumulus_library_covid/covid_symptom/define_symptom.py`

 * *Files 2% similar despite different names*

```diff
@@ -14,13 +14,13 @@
 
     table_cols = "AS t (cui, tui, code, system, text, pref);"
     create_view = (
         "create or replace view covid_symptom__define_symptom as "
         f"select * from (VALUES \n {values_sql}) \n {table_cols}"
     )
 
-    with open("covid_define_symptom.sql", "w", encoding="UTF-8") as f:
+    with open("define_symptom.sql", "w", encoding="UTF-8") as f:
         f.write(create_view)
 
 
 if __name__ == "__main__":
     main()
```

### Comparing `cumulus_library_covid-0.1.2/cumulus_library_covid/covid_symptom/covid_define_symptom.sql` & `cumulus_library_covid-0.1.3/cumulus_library_covid/covid_symptom/define_symptom.sql`

 * *Files identical despite different names*

### Comparing `cumulus_library_covid-0.1.2/pyproject.toml` & `cumulus_library_covid-0.1.3/pyproject.toml`

 * *Files 10% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 [project]
 name = "cumulus-library-covid"
-version = "0.1.2"
+version = "0.1.3"
 # In order to support 3.12, we wil need to refactor out load_module, which is
 # targeted for deprecation in that version.
 requires-python = ">= 3.9, <3.12"
 dependencies = [
-    "cumulus-library >= 0.1.2",
+    "cumulus-library >= 0.3.0",
     "sqlfluff == 2.0.2"
 ]
 description = "SQL generation for cumulus covid symptom analysis"
 readme = "README.md"
 license = { text="Apache License 2.0" }
 classifiers = [
     "License :: OSI Approved :: Apache Software License",
```

### Comparing `cumulus_library_covid-0.1.2/PKG-INFO` & `cumulus_library_covid-0.1.3/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 Metadata-Version: 2.1
 Name: cumulus-library-covid
-Version: 0.1.2
+Version: 0.1.3
 Summary: SQL generation for cumulus covid symptom analysis
 Requires-Python: >= 3.9, <3.12
 Description-Content-Type: text/markdown
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
-Requires-Dist: cumulus-library >= 0.1.2
+Requires-Dist: cumulus-library >= 0.3.0
 Requires-Dist: sqlfluff == 2.0.2
 Requires-Dist: black ; extra == "dev"
 Requires-Dist: pylint ; extra == "dev"
 Project-URL: Documentation, https://docs.smarthealthit.org/cumulus/
 Project-URL: Home, https://smarthealthit.org/cumulus-a-universal-sidecar-for-a-smart-learning-healthcare-system/
 Project-URL: Source, https://github.com/smart-on-fhir/cumulus-library-covid
 Provides-Extra: dev
```

