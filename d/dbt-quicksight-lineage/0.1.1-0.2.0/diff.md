# Comparing `tmp/dbt_quicksight_lineage-0.1.1.tar.gz` & `tmp/dbt_quicksight_lineage-0.2.0.tar.gz`

## Comparing `dbt_quicksight_lineage-0.1.1.tar` & `dbt_quicksight_lineage-0.2.0.tar`

### file list

```diff
@@ -1,52 +1,69 @@
--rw-r--r--   0        0        0    21487 2020-02-02 00:00:00.000000 dbt_quicksight_lineage-0.1.1/.pylintrc
--rw-r--r--   0        0        0       15 2020-02-02 00:00:00.000000 dbt_quicksight_lineage-0.1.1/.python-version
--rw-r--r--   0        0        0     1471 2020-02-02 00:00:00.000000 dbt_quicksight_lineage-0.1.1/.tagpr
--rw-r--r--   0        0        0      519 2020-02-02 00:00:00.000000 dbt_quicksight_lineage-0.1.1/CHANGELOG.md
--rw-r--r--   0        0        0     2164 2020-02-02 00:00:00.000000 dbt_quicksight_lineage-0.1.1/requirements-dev.lock
--rw-r--r--   0        0        0     1009 2020-02-02 00:00:00.000000 dbt_quicksight_lineage-0.1.1/requirements.lock
--rw-r--r--   0        0        0      356 2020-02-02 00:00:00.000000 dbt_quicksight_lineage-0.1.1/.github/dependabot.yaml
--rw-r--r--   0        0        0       48 2020-02-02 00:00:00.000000 dbt_quicksight_lineage-0.1.1/.github/release.yml
--rw-r--r--   0        0        0      988 2020-02-02 00:00:00.000000 dbt_quicksight_lineage-0.1.1/.github/workflows/reviewdog.yaml
--rw-r--r--   0        0        0     1302 2020-02-02 00:00:00.000000 dbt_quicksight_lineage-0.1.1/.github/workflows/tagpr.yaml
--rw-r--r--   0        0        0      437 2020-02-02 00:00:00.000000 dbt_quicksight_lineage-0.1.1/.github/workflows/test.yaml
--rw-r--r--   0        0        0   208760 2020-02-02 00:00:00.000000 dbt_quicksight_lineage-0.1.1/docs/images/dataset.png
--rw-r--r--   0        0        0      206 2020-02-02 00:00:00.000000 dbt_quicksight_lineage-0.1.1/src/dbt_quicksight_lineage/__about__.py
--rw-r--r--   0        0        0      107 2020-02-02 00:00:00.000000 dbt_quicksight_lineage-0.1.1/src/dbt_quicksight_lineage/__init__.py
--rw-r--r--   0        0        0      329 2020-02-02 00:00:00.000000 dbt_quicksight_lineage-0.1.1/src/dbt_quicksight_lineage/__main__.py
--rw-r--r--   0        0        0      188 2020-02-02 00:00:00.000000 dbt_quicksight_lineage-0.1.1/src/dbt_quicksight_lineage/cli/__init__.py
--rw-r--r--   0        0        0     3354 2020-02-02 00:00:00.000000 dbt_quicksight_lineage-0.1.1/src/dbt_quicksight_lineage/cli/main.py
--rw-r--r--   0        0        0     2172 2020-02-02 00:00:00.000000 dbt_quicksight_lineage-0.1.1/src/dbt_quicksight_lineage/cli/requires.py
--rw-r--r--   0        0        0      246 2020-02-02 00:00:00.000000 dbt_quicksight_lineage-0.1.1/src/dbt_quicksight_lineage/core/__init__.py
--rw-r--r--   0        0        0    23636 2020-02-02 00:00:00.000000 dbt_quicksight_lineage-0.1.1/src/dbt_quicksight_lineage/core/app.py
--rw-r--r--   0        0        0     2763 2020-02-02 00:00:00.000000 dbt_quicksight_lineage-0.1.1/src/dbt_quicksight_lineage/core/dbt.py
--rw-r--r--   0        0        0      107 2020-02-02 00:00:00.000000 dbt_quicksight_lineage-0.1.1/tests/__init__.py
--rw-r--r--   0        0        0     7574 2020-02-02 00:00:00.000000 dbt_quicksight_lineage-0.1.1/tests/core/test_app.py
--rw-r--r--   0        0        0     5937 2020-02-02 00:00:00.000000 dbt_quicksight_lineage-0.1.1/tests/core/test_dbt.py
--rw-r--r--   0        0        0     1972 2020-02-02 00:00:00.000000 dbt_quicksight_lineage-0.1.1/tests/data/describe_data_set_output.json
--rw-r--r--   0        0        0      794 2020-02-02 00:00:00.000000 dbt_quicksight_lineage-0.1.1/tests/data/expected_schema.yml
--rw-r--r--   0        0        0   302180 2020-02-02 00:00:00.000000 dbt_quicksight_lineage-0.1.1/tests/data/manifest.json
--rw-r--r--   0        0        0     1925 2020-02-02 00:00:00.000000 dbt_quicksight_lineage-0.1.1/tests/data/modified_data_set.json
--rw-r--r--   0        0        0   305700 2020-02-02 00:00:00.000000 dbt_quicksight_lineage-0.1.1/tests/data/partial_parse.msgpack
--rw-r--r--   0        0        0      437 2020-02-02 00:00:00.000000 dbt_quicksight_lineage-0.1.1/tests/data/schema.yml
--rw-r--r--   0        0        0       11 2020-02-02 00:00:00.000000 dbt_quicksight_lineage-0.1.1/tests/data/models/example/.gitignore
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 dbt_quicksight_lineage-0.1.1/tests/data/models/example/.gitkeep
--rw-r--r--   0        0        0       28 2020-02-02 00:00:00.000000 dbt_quicksight_lineage-0.1.1/tests/data/test_project/.gitignore
--rw-r--r--   0        0        0       41 2020-02-02 00:00:00.000000 dbt_quicksight_lineage-0.1.1/tests/data/test_project/.user.yml
--rw-r--r--   0        0        0      149 2020-02-02 00:00:00.000000 dbt_quicksight_lineage-0.1.1/tests/data/test_project/Makefile
--rw-r--r--   0        0        0      571 2020-02-02 00:00:00.000000 dbt_quicksight_lineage-0.1.1/tests/data/test_project/README.md
--rw-r--r--   0        0        0     1268 2020-02-02 00:00:00.000000 dbt_quicksight_lineage-0.1.1/tests/data/test_project/dbt_project.yml
--rw-r--r--   0        0        0      300 2020-02-02 00:00:00.000000 dbt_quicksight_lineage-0.1.1/tests/data/test_project/docker-compose.yaml
--rw-r--r--   0        0        0      211 2020-02-02 00:00:00.000000 dbt_quicksight_lineage-0.1.1/tests/data/test_project/profiles.yml
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 dbt_quicksight_lineage-0.1.1/tests/data/test_project/analyses/.gitkeep
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 dbt_quicksight_lineage-0.1.1/tests/data/test_project/macros/.gitkeep
--rw-r--r--   0        0        0      472 2020-02-02 00:00:00.000000 dbt_quicksight_lineage-0.1.1/tests/data/test_project/models/example/my_first_dbt_model.sql
--rw-r--r--   0        0        0      115 2020-02-02 00:00:00.000000 dbt_quicksight_lineage-0.1.1/tests/data/test_project/models/example/my_second_dbt_model.sql
--rw-r--r--   0        0        0     1318 2020-02-02 00:00:00.000000 dbt_quicksight_lineage-0.1.1/tests/data/test_project/models/example/schema.yml
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 dbt_quicksight_lineage-0.1.1/tests/data/test_project/seeds/.gitkeep
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 dbt_quicksight_lineage-0.1.1/tests/data/test_project/snapshots/.gitkeep
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 dbt_quicksight_lineage-0.1.1/tests/data/test_project/tests/.gitkeep
--rw-r--r--   0        0        0     3078 2020-02-02 00:00:00.000000 dbt_quicksight_lineage-0.1.1/.gitignore
--rw-r--r--   0        0        0     1070 2020-02-02 00:00:00.000000 dbt_quicksight_lineage-0.1.1/LICENSE
--rw-r--r--   0        0        0     2436 2020-02-02 00:00:00.000000 dbt_quicksight_lineage-0.1.1/README.md
--rw-r--r--   0        0        0     3758 2020-02-02 00:00:00.000000 dbt_quicksight_lineage-0.1.1/pyproject.toml
--rw-r--r--   0        0        0     3385 2020-02-02 00:00:00.000000 dbt_quicksight_lineage-0.1.1/PKG-INFO
+-rw-r--r--   0        0        0    21501 2020-02-02 00:00:00.000000 dbt_quicksight_lineage-0.2.0/.pylintrc
+-rw-r--r--   0        0        0       15 2020-02-02 00:00:00.000000 dbt_quicksight_lineage-0.2.0/.python-version
+-rw-r--r--   0        0        0     1471 2020-02-02 00:00:00.000000 dbt_quicksight_lineage-0.2.0/.tagpr
+-rw-r--r--   0        0        0     1076 2020-02-02 00:00:00.000000 dbt_quicksight_lineage-0.2.0/CHANGELOG.md
+-rw-r--r--   0        0        0     2164 2020-02-02 00:00:00.000000 dbt_quicksight_lineage-0.2.0/requirements-dev.lock
+-rw-r--r--   0        0        0     1009 2020-02-02 00:00:00.000000 dbt_quicksight_lineage-0.2.0/requirements.lock
+-rw-r--r--   0        0        0      356 2020-02-02 00:00:00.000000 dbt_quicksight_lineage-0.2.0/.github/dependabot.yaml
+-rw-r--r--   0        0        0       48 2020-02-02 00:00:00.000000 dbt_quicksight_lineage-0.2.0/.github/release.yml
+-rw-r--r--   0        0        0      988 2020-02-02 00:00:00.000000 dbt_quicksight_lineage-0.2.0/.github/workflows/reviewdog.yaml
+-rw-r--r--   0        0        0     1302 2020-02-02 00:00:00.000000 dbt_quicksight_lineage-0.2.0/.github/workflows/tagpr.yaml
+-rw-r--r--   0        0        0      437 2020-02-02 00:00:00.000000 dbt_quicksight_lineage-0.2.0/.github/workflows/test.yaml
+-rw-r--r--   0        0        0   208760 2020-02-02 00:00:00.000000 dbt_quicksight_lineage-0.2.0/docs/images/dataset.png
+-rw-r--r--   0        0        0      206 2020-02-02 00:00:00.000000 dbt_quicksight_lineage-0.2.0/src/dbt_quicksight_lineage/__about__.py
+-rw-r--r--   0        0        0      107 2020-02-02 00:00:00.000000 dbt_quicksight_lineage-0.2.0/src/dbt_quicksight_lineage/__init__.py
+-rw-r--r--   0        0        0      329 2020-02-02 00:00:00.000000 dbt_quicksight_lineage-0.2.0/src/dbt_quicksight_lineage/__main__.py
+-rw-r--r--   0        0        0      188 2020-02-02 00:00:00.000000 dbt_quicksight_lineage-0.2.0/src/dbt_quicksight_lineage/cli/__init__.py
+-rw-r--r--   0        0        0     3354 2020-02-02 00:00:00.000000 dbt_quicksight_lineage-0.2.0/src/dbt_quicksight_lineage/cli/main.py
+-rw-r--r--   0        0        0     2172 2020-02-02 00:00:00.000000 dbt_quicksight_lineage-0.2.0/src/dbt_quicksight_lineage/cli/requires.py
+-rw-r--r--   0        0        0      246 2020-02-02 00:00:00.000000 dbt_quicksight_lineage-0.2.0/src/dbt_quicksight_lineage/core/__init__.py
+-rw-r--r--   0        0        0    17669 2020-02-02 00:00:00.000000 dbt_quicksight_lineage-0.2.0/src/dbt_quicksight_lineage/core/app.py
+-rw-r--r--   0        0        0     5556 2020-02-02 00:00:00.000000 dbt_quicksight_lineage-0.2.0/src/dbt_quicksight_lineage/core/dbt.py
+-rw-r--r--   0        0        0    29104 2020-02-02 00:00:00.000000 dbt_quicksight_lineage-0.2.0/src/dbt_quicksight_lineage/core/quicksight.py
+-rw-r--r--   0        0        0      107 2020-02-02 00:00:00.000000 dbt_quicksight_lineage-0.2.0/tests/__init__.py
+-rw-r--r--   0        0        0    11639 2020-02-02 00:00:00.000000 dbt_quicksight_lineage-0.2.0/tests/core/test_app.py
+-rw-r--r--   0        0        0     5937 2020-02-02 00:00:00.000000 dbt_quicksight_lineage-0.2.0/tests/core/test_dbt.py
+-rw-r--r--   0        0        0     7638 2020-02-02 00:00:00.000000 dbt_quicksight_lineage-0.2.0/tests/core/test_quicksight.py
+-rw-r--r--   0        0        0     1972 2020-02-02 00:00:00.000000 dbt_quicksight_lineage-0.2.0/tests/data/describe_data_set_output.json
+-rw-r--r--   0        0        0      794 2020-02-02 00:00:00.000000 dbt_quicksight_lineage-0.2.0/tests/data/expected_schema.yml
+-rw-r--r--   0        0        0   302180 2020-02-02 00:00:00.000000 dbt_quicksight_lineage-0.2.0/tests/data/manifest.json
+-rw-r--r--   0        0        0     1925 2020-02-02 00:00:00.000000 dbt_quicksight_lineage-0.2.0/tests/data/modified_data_set.json
+-rw-r--r--   0        0        0   305700 2020-02-02 00:00:00.000000 dbt_quicksight_lineage-0.2.0/tests/data/partial_parse.msgpack
+-rw-r--r--   0        0        0      437 2020-02-02 00:00:00.000000 dbt_quicksight_lineage-0.2.0/tests/data/schema.yml
+-rw-r--r--   0        0        0     2951 2020-02-02 00:00:00.000000 dbt_quicksight_lineage-0.2.0/tests/data/fixture/data_set.json
+-rw-r--r--   0        0        0     2720 2020-02-02 00:00:00.000000 dbt_quicksight_lineage-0.2.0/tests/data/fixture/test_add_to_field_folder_move.golden.json
+-rw-r--r--   0        0        0     2824 2020-02-02 00:00:00.000000 dbt_quicksight_lineage-0.2.0/tests/data/fixture/test_add_to_field_folder_not_exits.golden.json
+-rw-r--r--   0        0        0     2771 2020-02-02 00:00:00.000000 dbt_quicksight_lineage-0.2.0/tests/data/fixture/test_add_to_field_folder_same_folder.golden.json
+-rw-r--r--   0        0        0     2756 2020-02-02 00:00:00.000000 dbt_quicksight_lineage-0.2.0/tests/data/fixture/test_add_to_projected_columns_exists.golden.json
+-rw-r--r--   0        0        0     2778 2020-02-02 00:00:00.000000 dbt_quicksight_lineage-0.2.0/tests/data/fixture/test_add_to_projected_columns_not_exists.golden.json
+-rw-r--r--   0        0        0     2713 2020-02-02 00:00:00.000000 dbt_quicksight_lineage-0.2.0/tests/data/fixture/test_set_cast_column_type_operation_exists_replace.golden.json
+-rw-r--r--   0        0        0     2863 2020-02-02 00:00:00.000000 dbt_quicksight_lineage-0.2.0/tests/data/fixture/test_set_cast_column_type_operation_not_exists.golden.json
+-rw-r--r--   0        0        0     2568 2020-02-02 00:00:00.000000 dbt_quicksight_lineage-0.2.0/tests/data/fixture/test_set_cast_column_type_operation_same_type.golden.json
+-rw-r--r--   0        0        0     2909 2020-02-02 00:00:00.000000 dbt_quicksight_lineage-0.2.0/tests/data/fixture/test_set_rename_column_oeration_not_exists.golden.json
+-rw-r--r--   0        0        0     2765 2020-02-02 00:00:00.000000 dbt_quicksight_lineage-0.2.0/tests/data/fixture/test_set_rename_operation_exits_replace.golden.json
+-rw-r--r--   0        0        0     2712 2020-02-02 00:00:00.000000 dbt_quicksight_lineage-0.2.0/tests/data/fixture/test_set_tag_column_geographic_role_operation_exists_replace.golden.json
+-rw-r--r--   0        0        0     2937 2020-02-02 00:00:00.000000 dbt_quicksight_lineage-0.2.0/tests/data/fixture/test_set_tag_column_geographic_role_operation_not_exists.golden.json
+-rw-r--r--   0        0        0     2767 2020-02-02 00:00:00.000000 dbt_quicksight_lineage-0.2.0/tests/data/fixture/test_set_tag_column_operation_description_exists_replace.golden.json
+-rw-r--r--   0        0        0     3027 2020-02-02 00:00:00.000000 dbt_quicksight_lineage-0.2.0/tests/data/fixture/test_set_tag_column_operation_description_not_exists.golden.json
+-rw-r--r--   0        0        0       11 2020-02-02 00:00:00.000000 dbt_quicksight_lineage-0.2.0/tests/data/models/example/.gitignore
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 dbt_quicksight_lineage-0.2.0/tests/data/models/example/.gitkeep
+-rw-r--r--   0        0        0       28 2020-02-02 00:00:00.000000 dbt_quicksight_lineage-0.2.0/tests/data/test_project/.gitignore
+-rw-r--r--   0        0        0       41 2020-02-02 00:00:00.000000 dbt_quicksight_lineage-0.2.0/tests/data/test_project/.user.yml
+-rw-r--r--   0        0        0      149 2020-02-02 00:00:00.000000 dbt_quicksight_lineage-0.2.0/tests/data/test_project/Makefile
+-rw-r--r--   0        0        0      571 2020-02-02 00:00:00.000000 dbt_quicksight_lineage-0.2.0/tests/data/test_project/README.md
+-rw-r--r--   0        0        0     1268 2020-02-02 00:00:00.000000 dbt_quicksight_lineage-0.2.0/tests/data/test_project/dbt_project.yml
+-rw-r--r--   0        0        0      300 2020-02-02 00:00:00.000000 dbt_quicksight_lineage-0.2.0/tests/data/test_project/docker-compose.yaml
+-rw-r--r--   0        0        0      211 2020-02-02 00:00:00.000000 dbt_quicksight_lineage-0.2.0/tests/data/test_project/profiles.yml
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 dbt_quicksight_lineage-0.2.0/tests/data/test_project/analyses/.gitkeep
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 dbt_quicksight_lineage-0.2.0/tests/data/test_project/macros/.gitkeep
+-rw-r--r--   0        0        0      472 2020-02-02 00:00:00.000000 dbt_quicksight_lineage-0.2.0/tests/data/test_project/models/example/my_first_dbt_model.sql
+-rw-r--r--   0        0        0      115 2020-02-02 00:00:00.000000 dbt_quicksight_lineage-0.2.0/tests/data/test_project/models/example/my_second_dbt_model.sql
+-rw-r--r--   0        0        0     1318 2020-02-02 00:00:00.000000 dbt_quicksight_lineage-0.2.0/tests/data/test_project/models/example/schema.yml
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 dbt_quicksight_lineage-0.2.0/tests/data/test_project/seeds/.gitkeep
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 dbt_quicksight_lineage-0.2.0/tests/data/test_project/snapshots/.gitkeep
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 dbt_quicksight_lineage-0.2.0/tests/data/test_project/tests/.gitkeep
+-rw-r--r--   0        0        0     3078 2020-02-02 00:00:00.000000 dbt_quicksight_lineage-0.2.0/.gitignore
+-rw-r--r--   0        0        0     1070 2020-02-02 00:00:00.000000 dbt_quicksight_lineage-0.2.0/LICENSE
+-rw-r--r--   0        0        0     2863 2020-02-02 00:00:00.000000 dbt_quicksight_lineage-0.2.0/README.md
+-rw-r--r--   0        0        0     3758 2020-02-02 00:00:00.000000 dbt_quicksight_lineage-0.2.0/pyproject.toml
+-rw-r--r--   0        0        0     3812 2020-02-02 00:00:00.000000 dbt_quicksight_lineage-0.2.0/PKG-INFO
```

### Comparing `dbt_quicksight_lineage-0.1.1/.pylintrc` & `dbt_quicksight_lineage-0.2.0/.pylintrc`

 * *Files 0% similar despite different names*

```diff
@@ -184,14 +184,15 @@
 # naming style.
 #function-rgx=
 
 # Good variable names which should always be accepted, separated by a comma.
 good-names=i,
            j,
            k,
+           v,
            ex,
            Run,
            f,
            _
 
 # Good variable names regexes, separated by a comma. If names match any regex,
 # they will always be accepted
@@ -300,15 +301,15 @@
 # Maximum number of locals for function / method body.
 max-locals=15
 
 # Maximum number of parents for a class (see R0901).
 max-parents=7
 
 # Maximum number of public methods for a class (see R0904).
-max-public-methods=20
+max-public-methods=30
 
 # Maximum number of return / yield for function / method body.
 max-returns=6
 
 # Maximum number of statements in function / method body.
 max-statements=50
```

### Comparing `dbt_quicksight_lineage-0.1.1/.tagpr` & `dbt_quicksight_lineage-0.2.0/.tagpr`

 * *Files identical despite different names*

### Comparing `dbt_quicksight_lineage-0.1.1/CHANGELOG.md` & `dbt_quicksight_lineage-0.2.0/CHANGELOG.md`

 * *Files 20% similar despite different names*

```diff
@@ -1,9 +1,15 @@
 # Changelog
 
+## [v0.2.0](https://github.com/mashiike/dbt-quicksight-lineage/compare/v0.1.1...v0.2.0) - 2023-07-05
+- できる限り、元のDataSetの定義を維持したい by @mashiike in https://github.com/mashiike/dbt-quicksight-lineage/pull/7
+- add hidden on init command by @mashiike in https://github.com/mashiike/dbt-quicksight-lineage/pull/9
+- add geographic role by @mashiike in https://github.com/mashiike/dbt-quicksight-lineage/pull/10
+- data_type meta for CastColumnTypeOperation by @mashiike in https://github.com/mashiike/dbt-quicksight-lineage/pull/11
+
 ## [v0.1.1](https://github.com/mashiike/dbt-quicksight-lineage/compare/v0.1.0...v0.1.1) - 2023-07-04
 - fix pipeline and fix dependency by @mashiike in https://github.com/mashiike/dbt-quicksight-lineage/pull/5
 
 ## [v0.1.0](https://github.com/mashiike/dbt-quicksight-lineage/compare/v0.0.2...v0.1.0) - 2023-07-04
 
 ## [v0.0.2](https://github.com/mashiike/dbt-quicksight-lineage/compare/v0.0.1...v0.0.2) - 2023-07-04
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `dbt_quicksight_lineage-0.1.1/requirements-dev.lock` & `dbt_quicksight_lineage-0.2.0/requirements-dev.lock`

 * *Files identical despite different names*

### Comparing `dbt_quicksight_lineage-0.1.1/requirements.lock` & `dbt_quicksight_lineage-0.2.0/requirements.lock`

 * *Files identical despite different names*

### Comparing `dbt_quicksight_lineage-0.1.1/.github/workflows/reviewdog.yaml` & `dbt_quicksight_lineage-0.2.0/.github/workflows/reviewdog.yaml`

 * *Files identical despite different names*

### Comparing `dbt_quicksight_lineage-0.1.1/.github/workflows/tagpr.yaml` & `dbt_quicksight_lineage-0.2.0/.github/workflows/tagpr.yaml`

 * *Files identical despite different names*

### Comparing `dbt_quicksight_lineage-0.1.1/docs/images/dataset.png` & `dbt_quicksight_lineage-0.2.0/docs/images/dataset.png`

 * *Files identical despite different names*

### Comparing `dbt_quicksight_lineage-0.1.1/src/dbt_quicksight_lineage/cli/main.py` & `dbt_quicksight_lineage-0.2.0/src/dbt_quicksight_lineage/cli/main.py`

 * *Files identical despite different names*

### Comparing `dbt_quicksight_lineage-0.1.1/src/dbt_quicksight_lineage/cli/requires.py` & `dbt_quicksight_lineage-0.2.0/src/dbt_quicksight_lineage/cli/requires.py`

 * *Files identical despite different names*

### Comparing `dbt_quicksight_lineage-0.1.1/tests/core/test_app.py` & `dbt_quicksight_lineage-0.2.0/tests/core/test_app.py`

 * *Files 24% similar despite different names*

```diff
@@ -3,18 +3,18 @@
 import boto3
 import botocore
 import json
 import shutil
 import filecmp
 from moto import mock_quicksight, mock_sts
 from mock import patch
+from dbt_quicksight_lineage.core.quicksight import DataSet
 from dbt_quicksight_lineage.core import (
     ManifestLoader,
     App,
-    DataSet,
 )
 import logging
 logging.basicConfig(level=logging.DEBUG)
 logger = logging.getLogger()
 
 
 @pytest.fixture(scope='class')
@@ -76,44 +76,41 @@
         app = App(
             quicksight_client=mock_quicksight_client,
             manifest=example_manifest
         )
         with open('tests/data/describe_data_set_output.json', 'r') as f:
             describe_data_set_output = json.load(f)
         actual = set([
-            (physical_table_id, node.unique_id)
-            for physical_table_id, node in app._detect_modify_target(DataSet(describe_data_set_output.get('DataSet')))
+            (physical_table.physical_table_id, node.unique_id)
+            for physical_table, node in app._detect_modify_target(DataSet(describe_data_set_output.get('DataSet')))
         ])
         expected = set([
             ('12345678-9abc-def0-1234-56789abcdef0',
              'model.test_project.my_first_dbt_model'),
         ])
         assert actual == expected
 
-    def test_generate_logical_table(self, example_manifest, mock_quicksight_client):
+    def test_modify_logical_table(self, example_manifest, mock_quicksight_client):
         app = App(
             quicksight_client=mock_quicksight_client,
             manifest=example_manifest
         )
         with open('tests/data/describe_data_set_output.json', 'r') as f:
             describe_data_set_output = json.load(f)
         data_set = DataSet(describe_data_set_output.get('DataSet'))
         physical_table_id = '12345678-9abc-def0-1234-56789abcdef0'
-        logical_table, filed_folders = app._generate_logical_table(
-            physical_table_id,
-            data_set.physical_relational_table(physical_table_id),
+        app._modify_logical_table(
+            data_set,
+            data_set.physical_table_map[physical_table_id],
             example_manifest.nodes['model.test_project.my_first_dbt_model'],
         )
 
         with open('tests/data/modified_data_set.json') as f:
             modified_data_set = DataSet(json.load(f))
-        _, expected = modified_data_set.find_logical_table_by_physical_table_id(
-            physical_table_id)
-        assert expected == logical_table
-        assert modified_data_set.filed_folders() == filed_folders
+        assert data_set.to_dict() == modified_data_set.to_dict()
 
     @patch('botocore.client.BaseClient._make_api_call', new=mock_make_api_call)
     def test_update_data_set_dry_run(
         self,
         example_manifest,
         mock_quicksight_client,
     ):
@@ -124,27 +121,28 @@
         _, input = app.update_data_set(
             '00000000-0000-0000-0000-000000000000',
             dry_run=True,
         )
         with open('tests/data/modified_data_set.json') as f:
             modified_data_set = DataSet(json.load(f))
         assert input == modified_data_set.generate_update_data_set_input(
-            '123456789012')
+            '123456789012'
+        )
 
     def test_detect_related_nodes(self, example_manifest, mock_quicksight_client):
         app = App(
             quicksight_client=mock_quicksight_client,
             manifest=example_manifest
         )
         with open('tests/data/modified_data_set.json', 'r') as f:
             data_set = DataSet(json.load(f))
 
         actual = set([
-            (physical_table_id, node.unique_id)
-            for physical_table_id, node in app._detect_related_nodes(
+            (physical_table.physical_table_id, node.unique_id)
+            for physical_table, node in app._detect_related_nodes(
                 data_set,
             )
         ])
         expected = set([
             ('12345678-9abc-def0-1234-56789abcdef0',
              'model.test_project.my_first_dbt_model'),
         ])
@@ -188,14 +186,121 @@
                                 },
                             },
                         },
                     ],
                 },
             ],
         }
+        assert actual == expected
+
+    def test_generate_schema_dict_fixture_data_set(self, example_manifest, mock_quicksight_client):
+        app = App(
+            quicksight_client=mock_quicksight_client,
+            manifest=example_manifest
+        )
+        with open('tests/data/fixture/data_set.json', 'r') as f:
+            data_set = DataSet(json.load(f))
+        actual = app._generate_schema_dict(
+            'test_model',
+            data_set,
+            '12345678-9abc-def0-1234-56789abcdef0',
+        )
+        expected = {
+            'models': [
+                {
+                    'name': 'test_model',
+                    'meta': {
+                        'quicksight': {
+                            'logical_table_name': 'My First DBT Model',
+                            'data_sets': [
+                                {
+                                    'id': '00000000-0000-0000-0000-000000000000',
+                                    'data_source_arn': 'arn:aws:quicksight:ap-northeast-1:123456789012:datasource/00000000-0000-0000-0000-000000000000',
+                                },
+                            ],
+                            'folders': [
+                                {
+                                    'description': 'this is key folder',
+                                    'name': 'Key',
+                                }
+                            ],
+                        },
+                    },
+                    'columns': [
+                        {
+                            'name': 'id',
+                            'description': 'The primary key for this table',
+                            'meta': {
+                                'quicksight': {
+                                    'field_name': 'ID',
+                                    'folder': 'Key',
+                                },
+                            },
+                        },
+                        {
+                            'name': 'name',
+                            'meta': {
+                                'quicksight': {
+                                    'hidden': True,
+                                },
+                            },
+                        },
+                        {
+                            'name': 'geo',
+                            'meta': {
+                                'quicksight': {
+                                    'geographic_role': 'state',
+                                },
+                            },
+                        },
+                        {
+                            'name': 'latitude',
+                            'meta': {
+                                'quicksight': {
+                                    'hidden': True,
+                                },
+                            },
+                        },
+                        {
+                            'name': 'longitude',
+                            'meta': {
+                                'quicksight': {
+                                    'hidden': True,
+                                },
+                            },
+                        },
+                        {
+                            'name': 'rate',
+                            'meta': {
+                                'quicksight': {
+                                    'data_type': 'boolean',
+                                    'hidden': True,
+                                },
+                            },
+                        },
+                        {
+                            'name': 'created_at',
+                            'meta': {
+                                'quicksight': {
+                                    'hidden': True,
+                                },
+                            },
+                        },
+                        {
+                            'name': 'updated_at',
+                            'meta': {
+                                'quicksight': {
+                                    'hidden': True,
+                                },
+                            },
+                        },
+                    ],
+                },
+            ],
+        }
         assert actual == expected
 
     def test_update_schema_yaml(self, example_manifest, mock_quicksight_client):
         app = App(
             quicksight_client=mock_quicksight_client,
             manifest=example_manifest
         )
```

### Comparing `dbt_quicksight_lineage-0.1.1/tests/core/test_dbt.py` & `dbt_quicksight_lineage-0.2.0/tests/core/test_dbt.py`

 * *Files identical despite different names*

### Comparing `dbt_quicksight_lineage-0.1.1/tests/data/describe_data_set_output.json` & `dbt_quicksight_lineage-0.2.0/tests/data/describe_data_set_output.json`

 * *Files identical despite different names*

### Comparing `dbt_quicksight_lineage-0.1.1/tests/data/expected_schema.yml` & `dbt_quicksight_lineage-0.2.0/tests/data/expected_schema.yml`

 * *Files identical despite different names*

### Comparing `dbt_quicksight_lineage-0.1.1/tests/data/manifest.json` & `dbt_quicksight_lineage-0.2.0/tests/data/manifest.json`

 * *Files identical despite different names*

### Comparing `dbt_quicksight_lineage-0.1.1/tests/data/modified_data_set.json` & `dbt_quicksight_lineage-0.2.0/tests/data/modified_data_set.json`

 * *Files identical despite different names*

### Comparing `dbt_quicksight_lineage-0.1.1/tests/data/partial_parse.msgpack` & `dbt_quicksight_lineage-0.2.0/tests/data/partial_parse.msgpack`

 * *Files identical despite different names*

### Comparing `dbt_quicksight_lineage-0.1.1/tests/data/test_project/README.md` & `dbt_quicksight_lineage-0.2.0/tests/data/test_project/README.md`

 * *Files identical despite different names*

### Comparing `dbt_quicksight_lineage-0.1.1/tests/data/test_project/dbt_project.yml` & `dbt_quicksight_lineage-0.2.0/tests/data/test_project/dbt_project.yml`

 * *Files identical despite different names*

### Comparing `dbt_quicksight_lineage-0.1.1/tests/data/test_project/models/example/schema.yml` & `dbt_quicksight_lineage-0.2.0/tests/data/test_project/models/example/schema.yml`

 * *Files identical despite different names*

### Comparing `dbt_quicksight_lineage-0.1.1/.gitignore` & `dbt_quicksight_lineage-0.2.0/.gitignore`

 * *Files identical despite different names*

### Comparing `dbt_quicksight_lineage-0.1.1/LICENSE` & `dbt_quicksight_lineage-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `dbt_quicksight_lineage-0.1.1/README.md` & `dbt_quicksight_lineage-0.2.0/README.md`

 * *Files 10% similar despite different names*

```diff
@@ -54,24 +54,40 @@
     description: "A starter dbt model"
     meta:
       quicksight:
         logical_table_name: My First DBT Model
         data_sets:
           - id: 00000000-0000-0000-0000-000000000000
             data_source_arn: arn:aws:quicksight:ap-northeast-1:123456789012:datasource/00000000-0000-0000-0000-000000000000
+        folders:
+          - name: Key
+            description: "this is Key folder, must distinct counts"
+          
     columns:
       - name: id
         description: "The primary key for this table"
         meta:
           quicksight:
             field_name: ID
             folder: Key
+            data_type: string
         tests:
           - unique
           - not_null
+      - name: geo
+        description: "City name of geometry"
+        meta:
+          quicksight:
+            geographic_role: city 
+            field_name: Geometry
+            folder: Key
+      - name: hidden_value
+        meta:
+          quicksight:
+            hidden: true
 
   - name: my_second_dbt_model
     description: "A starter dbt model"
     columns:
       - name: id
         description: "The primary key for this table"
         tests:
```

### Comparing `dbt_quicksight_lineage-0.1.1/pyproject.toml` & `dbt_quicksight_lineage-0.2.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `dbt_quicksight_lineage-0.1.1/PKG-INFO` & `dbt_quicksight_lineage-0.2.0/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dbt-quicksight-lineage
-Version: 0.1.1
+Version: 0.2.0
 Project-URL: Documentation, https://github.com/mashiike/dbt-quicksight-lineage#readme
 Project-URL: Issues, https://github.com/mashiike/dbt-quicksight-lineage/issues
 Project-URL: Source, https://github.com/mashiike/dbt-quicksight-lineage
 Author-email: mashiike <ikeda-masashi@kayac.com>
 License-Expression: MIT
 License-File: LICENSE
 Classifier: Development Status :: 4 - Beta
@@ -77,24 +77,40 @@
     description: "A starter dbt model"
     meta:
       quicksight:
         logical_table_name: My First DBT Model
         data_sets:
           - id: 00000000-0000-0000-0000-000000000000
             data_source_arn: arn:aws:quicksight:ap-northeast-1:123456789012:datasource/00000000-0000-0000-0000-000000000000
+        folders:
+          - name: Key
+            description: "this is Key folder, must distinct counts"
+          
     columns:
       - name: id
         description: "The primary key for this table"
         meta:
           quicksight:
             field_name: ID
             folder: Key
+            data_type: string
         tests:
           - unique
           - not_null
+      - name: geo
+        description: "City name of geometry"
+        meta:
+          quicksight:
+            geographic_role: city 
+            field_name: Geometry
+            folder: Key
+      - name: hidden_value
+        meta:
+          quicksight:
+            hidden: true
 
   - name: my_second_dbt_model
     description: "A starter dbt model"
     columns:
       - name: id
         description: "The primary key for this table"
         tests:
```

