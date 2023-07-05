# Comparing `tmp/total-perspective-vortex-2.2.4.tar.gz` & `tmp/total-perspective-vortex-2.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "total-perspective-vortex-2.2.4.tar", last modified: Fri May 26 07:54:11 2023, max compression
+gzip compressed data, was "total-perspective-vortex-2.3.0.tar", last modified: Wed Jul  5 06:17:07 2023, max compression
```

## Comparing `total-perspective-vortex-2.2.4.tar` & `total-perspective-vortex-2.3.0.tar`

### file list

```diff
@@ -1,51 +1,51 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 07:54:11.380432 total-perspective-vortex-2.2.4/
--rw-r--r--   0 runner    (1001) docker     (123)     1071 2023-05-26 07:54:01.000000 total-perspective-vortex-2.2.4/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     2238 2023-05-26 07:54:11.380432 total-perspective-vortex-2.2.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1337 2023-05-26 07:54:01.000000 total-perspective-vortex-2.2.4/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      374 2023-05-26 07:54:11.380432 total-perspective-vortex-2.2.4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2046 2023-05-26 07:54:01.000000 total-perspective-vortex-2.2.4/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 07:54:11.380432 total-perspective-vortex-2.2.4/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-26 07:54:01.000000 total-perspective-vortex-2.2.4/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2162 2023-05-26 07:54:01.000000 total-perspective-vortex-2.2.4/tests/test_entity.py
--rw-r--r--   0 runner    (1001) docker     (123)     2883 2023-05-26 07:54:01.000000 total-perspective-vortex-2.2.4/tests/test_mapper_basic.py
--rw-r--r--   0 runner    (1001) docker     (123)     3065 2023-05-26 07:54:01.000000 total-perspective-vortex-2.2.4/tests/test_mapper_context.py
--rw-r--r--   0 runner    (1001) docker     (123)    12535 2023-05-26 07:54:01.000000 total-perspective-vortex-2.2.4/tests/test_mapper_destinations.py
--rw-r--r--   0 runner    (1001) docker     (123)     5779 2023-05-26 07:54:01.000000 total-perspective-vortex-2.2.4/tests/test_mapper_inheritance.py
--rw-r--r--   0 runner    (1001) docker     (123)     6920 2023-05-26 07:54:01.000000 total-perspective-vortex-2.2.4/tests/test_mapper_merge_multiple.py
--rw-r--r--   0 runner    (1001) docker     (123)     2325 2023-05-26 07:54:01.000000 total-perspective-vortex-2.2.4/tests/test_mapper_params_specific.py
--rw-r--r--   0 runner    (1001) docker     (123)     1140 2023-05-26 07:54:01.000000 total-perspective-vortex-2.2.4/tests/test_mapper_rank.py
--rw-r--r--   0 runner    (1001) docker     (123)     2028 2023-05-26 07:54:01.000000 total-perspective-vortex-2.2.4/tests/test_mapper_resubmit.py
--rw-r--r--   0 runner    (1001) docker     (123)     3198 2023-05-26 07:54:01.000000 total-perspective-vortex-2.2.4/tests/test_mapper_role.py
--rw-r--r--   0 runner    (1001) docker     (123)    13750 2023-05-26 07:54:01.000000 total-perspective-vortex-2.2.4/tests/test_mapper_rules.py
--rw-r--r--   0 runner    (1001) docker     (123)      908 2023-05-26 07:54:01.000000 total-perspective-vortex-2.2.4/tests/test_mapper_sample.py
--rw-r--r--   0 runner    (1001) docker     (123)     4079 2023-05-26 07:54:01.000000 total-perspective-vortex-2.2.4/tests/test_mapper_user.py
--rw-r--r--   0 runner    (1001) docker     (123)    14778 2023-05-26 07:54:01.000000 total-perspective-vortex-2.2.4/tests/test_scenarios.py
--rw-r--r--   0 runner    (1001) docker     (123)    16894 2023-05-26 07:54:01.000000 total-perspective-vortex-2.2.4/tests/test_shell.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 07:54:11.380432 total-perspective-vortex-2.2.4/total_perspective_vortex.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2238 2023-05-26 07:54:11.000000 total-perspective-vortex-2.2.4/total_perspective_vortex.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1129 2023-05-26 07:54:11.000000 total-perspective-vortex-2.2.4/total_perspective_vortex.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-26 07:54:11.000000 total-perspective-vortex-2.2.4/total_perspective_vortex.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       48 2023-05-26 07:54:11.000000 total-perspective-vortex-2.2.4/total_perspective_vortex.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      439 2023-05-26 07:54:11.000000 total-perspective-vortex-2.2.4/total_perspective_vortex.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       10 2023-05-26 07:54:11.000000 total-perspective-vortex-2.2.4/total_perspective_vortex.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 07:54:11.380432 total-perspective-vortex-2.2.4/tpv/
--rw-r--r--   0 runner    (1001) docker     (123)      294 2023-05-26 07:54:01.000000 total-perspective-vortex-2.2.4/tpv/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 07:54:11.380432 total-perspective-vortex-2.2.4/tpv/commands/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-26 07:54:01.000000 total-perspective-vortex-2.2.4/tpv/commands/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1603 2023-05-26 07:54:01.000000 total-perspective-vortex-2.2.4/tpv/commands/dryrunner.py
--rw-r--r--   0 runner    (1001) docker     (123)     4084 2023-05-26 07:54:01.000000 total-perspective-vortex-2.2.4/tpv/commands/formatter.py
--rw-r--r--   0 runner    (1001) docker     (123)     3082 2023-05-26 07:54:01.000000 total-perspective-vortex-2.2.4/tpv/commands/linter.py
--rw-r--r--   0 runner    (1001) docker     (123)     4939 2023-05-26 07:54:01.000000 total-perspective-vortex-2.2.4/tpv/commands/shell.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 07:54:11.380432 total-perspective-vortex-2.2.4/tpv/commands/test/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-26 07:54:01.000000 total-perspective-vortex-2.2.4/tpv/commands/test/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2795 2023-05-26 07:54:01.000000 total-perspective-vortex-2.2.4/tpv/commands/test/mock_galaxy.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 07:54:11.380432 total-perspective-vortex-2.2.4/tpv/core/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-26 07:54:01.000000 total-perspective-vortex-2.2.4/tpv/core/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    35031 2023-05-26 07:54:01.000000 total-perspective-vortex-2.2.4/tpv/core/entities.py
--rw-r--r--   0 runner    (1001) docker     (123)     3865 2023-05-26 07:54:01.000000 total-perspective-vortex-2.2.4/tpv/core/helpers.py
--rw-r--r--   0 runner    (1001) docker     (123)     5660 2023-05-26 07:54:01.000000 total-perspective-vortex-2.2.4/tpv/core/loader.py
--rw-r--r--   0 runner    (1001) docker     (123)     7033 2023-05-26 07:54:01.000000 total-perspective-vortex-2.2.4/tpv/core/mapper.py
--rw-r--r--   0 runner    (1001) docker     (123)      343 2023-05-26 07:54:01.000000 total-perspective-vortex-2.2.4/tpv/core/util.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 07:54:11.380432 total-perspective-vortex-2.2.4/tpv/rules/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-26 07:54:01.000000 total-perspective-vortex-2.2.4/tpv/rules/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2155 2023-05-26 07:54:01.000000 total-perspective-vortex-2.2.4/tpv/rules/gateway.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 06:17:07.614799 total-perspective-vortex-2.3.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1071 2023-07-05 06:16:48.000000 total-perspective-vortex-2.3.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     2238 2023-07-05 06:17:07.614799 total-perspective-vortex-2.3.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1337 2023-07-05 06:16:48.000000 total-perspective-vortex-2.3.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      374 2023-07-05 06:17:07.614799 total-perspective-vortex-2.3.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2046 2023-07-05 06:16:48.000000 total-perspective-vortex-2.3.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 06:17:07.610799 total-perspective-vortex-2.3.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-05 06:16:48.000000 total-perspective-vortex-2.3.0/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2162 2023-07-05 06:16:48.000000 total-perspective-vortex-2.3.0/tests/test_entity.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2883 2023-07-05 06:16:48.000000 total-perspective-vortex-2.3.0/tests/test_mapper_basic.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3065 2023-07-05 06:16:48.000000 total-perspective-vortex-2.3.0/tests/test_mapper_context.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13522 2023-07-05 06:16:48.000000 total-perspective-vortex-2.3.0/tests/test_mapper_destinations.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5779 2023-07-05 06:16:48.000000 total-perspective-vortex-2.3.0/tests/test_mapper_inheritance.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8257 2023-07-05 06:16:48.000000 total-perspective-vortex-2.3.0/tests/test_mapper_merge_multiple.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2325 2023-07-05 06:16:48.000000 total-perspective-vortex-2.3.0/tests/test_mapper_params_specific.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1140 2023-07-05 06:16:48.000000 total-perspective-vortex-2.3.0/tests/test_mapper_rank.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2028 2023-07-05 06:16:48.000000 total-perspective-vortex-2.3.0/tests/test_mapper_resubmit.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3198 2023-07-05 06:16:48.000000 total-perspective-vortex-2.3.0/tests/test_mapper_role.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13750 2023-07-05 06:16:48.000000 total-perspective-vortex-2.3.0/tests/test_mapper_rules.py
+-rw-r--r--   0 runner    (1001) docker     (123)      908 2023-07-05 06:16:48.000000 total-perspective-vortex-2.3.0/tests/test_mapper_sample.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4079 2023-07-05 06:16:48.000000 total-perspective-vortex-2.3.0/tests/test_mapper_user.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14778 2023-07-05 06:16:48.000000 total-perspective-vortex-2.3.0/tests/test_scenarios.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16894 2023-07-05 06:16:48.000000 total-perspective-vortex-2.3.0/tests/test_shell.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 06:17:07.610799 total-perspective-vortex-2.3.0/total_perspective_vortex.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2238 2023-07-05 06:17:07.000000 total-perspective-vortex-2.3.0/total_perspective_vortex.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1129 2023-07-05 06:17:07.000000 total-perspective-vortex-2.3.0/total_perspective_vortex.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-05 06:17:07.000000 total-perspective-vortex-2.3.0/total_perspective_vortex.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       48 2023-07-05 06:17:07.000000 total-perspective-vortex-2.3.0/total_perspective_vortex.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      439 2023-07-05 06:17:07.000000 total-perspective-vortex-2.3.0/total_perspective_vortex.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-07-05 06:17:07.000000 total-perspective-vortex-2.3.0/total_perspective_vortex.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 06:17:07.610799 total-perspective-vortex-2.3.0/tpv/
+-rw-r--r--   0 runner    (1001) docker     (123)      294 2023-07-05 06:16:48.000000 total-perspective-vortex-2.3.0/tpv/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 06:17:07.610799 total-perspective-vortex-2.3.0/tpv/commands/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-05 06:16:48.000000 total-perspective-vortex-2.3.0/tpv/commands/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1603 2023-07-05 06:16:48.000000 total-perspective-vortex-2.3.0/tpv/commands/dryrunner.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4084 2023-07-05 06:16:48.000000 total-perspective-vortex-2.3.0/tpv/commands/formatter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3082 2023-07-05 06:16:48.000000 total-perspective-vortex-2.3.0/tpv/commands/linter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4939 2023-07-05 06:16:48.000000 total-perspective-vortex-2.3.0/tpv/commands/shell.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 06:17:07.610799 total-perspective-vortex-2.3.0/tpv/commands/test/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-05 06:16:48.000000 total-perspective-vortex-2.3.0/tpv/commands/test/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2795 2023-07-05 06:16:48.000000 total-perspective-vortex-2.3.0/tpv/commands/test/mock_galaxy.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 06:17:07.614799 total-perspective-vortex-2.3.0/tpv/core/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-05 06:16:48.000000 total-perspective-vortex-2.3.0/tpv/core/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    35270 2023-07-05 06:16:48.000000 total-perspective-vortex-2.3.0/tpv/core/entities.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3865 2023-07-05 06:16:48.000000 total-perspective-vortex-2.3.0/tpv/core/helpers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5499 2023-07-05 06:16:48.000000 total-perspective-vortex-2.3.0/tpv/core/loader.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7383 2023-07-05 06:16:48.000000 total-perspective-vortex-2.3.0/tpv/core/mapper.py
+-rw-r--r--   0 runner    (1001) docker     (123)      343 2023-07-05 06:16:48.000000 total-perspective-vortex-2.3.0/tpv/core/util.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 06:17:07.614799 total-perspective-vortex-2.3.0/tpv/rules/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-05 06:16:48.000000 total-perspective-vortex-2.3.0/tpv/rules/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2155 2023-07-05 06:16:48.000000 total-perspective-vortex-2.3.0/tpv/rules/gateway.py
```

### Comparing `total-perspective-vortex-2.2.4/LICENSE` & `total-perspective-vortex-2.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `total-perspective-vortex-2.2.4/PKG-INFO` & `total-perspective-vortex-2.3.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: total-perspective-vortex
-Version: 2.2.4
+Version: 2.3.0
 Summary: A library for routing entities (jobs, users or groups) to destinations in Galaxy
 Home-page: https://github.com/galaxyproject/total-perspective-vortex
 Author: Galaxy and GVL projects
 Author-email: help@genome.edu.au
 License: MIT
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Programming Language :: Python :: 3
```

### Comparing `total-perspective-vortex-2.2.4/README.md` & `total-perspective-vortex-2.3.0/README.md`

 * *Files identical despite different names*

### Comparing `total-perspective-vortex-2.2.4/setup.py` & `total-perspective-vortex-2.3.0/setup.py`

 * *Files identical despite different names*

### Comparing `total-perspective-vortex-2.2.4/tests/test_entity.py` & `total-perspective-vortex-2.3.0/tests/test_entity.py`

 * *Files identical despite different names*

### Comparing `total-perspective-vortex-2.2.4/tests/test_mapper_basic.py` & `total-perspective-vortex-2.3.0/tests/test_mapper_basic.py`

 * *Files identical despite different names*

### Comparing `total-perspective-vortex-2.2.4/tests/test_mapper_context.py` & `total-perspective-vortex-2.3.0/tests/test_mapper_context.py`

 * *Files identical despite different names*

### Comparing `total-perspective-vortex-2.2.4/tests/test_mapper_destinations.py` & `total-perspective-vortex-2.3.0/tests/test_mapper_destinations.py`

 * *Files 6% similar despite different names*

```diff
@@ -203,7 +203,22 @@
 
         config = os.path.join(os.path.dirname(__file__), 'fixtures/mapping-destinations.yml')
 
         tool = mock_galaxy.Tool('toolshed_hifiasm')
         datasets = [mock_galaxy.DatasetAssociation("test", mock_galaxy.Dataset("test.txt", file_size=12 * 1024 ** 3))]
         destination = self._map_to_destination(tool, user, datasets, tpv_config_paths=[config])
         self.assertEqual(destination.id, "pulsar-canberra")
+
+    def test_destination_clamping(self):
+        """_summary_ Any variables defined in a tool should be evaluated as late as possible, so that destination level
+                     clamping works.
+        """
+        user = mock_galaxy.User('albo', 'pulsar_canberra_user@act.au')
+
+        config = os.path.join(os.path.dirname(__file__), 'fixtures/mapping-destinations.yml')
+
+        tool = mock_galaxy.Tool('tool_for_testing_resource_clamping')
+        datasets = [mock_galaxy.DatasetAssociation("test", mock_galaxy.Dataset("test.txt", file_size=12 * 1024 ** 3))]
+        destination = self._map_to_destination(tool, user, datasets, tpv_config_paths=[config])
+        self.assertEqual(destination.id, "clamped_destination")
+        self.assertEqual([env['value'] for env in destination.env if env['name'] == 'MY_DEST_ENV'], ['cores: 8 mem: 24 gpus: 1'])
+        self.assertEqual([env['value'] for env in destination.env if env['name'] == 'MY_TOOL_ENV'], ['cores: 8 mem: 24 gpus: 1'])
```

### Comparing `total-perspective-vortex-2.2.4/tests/test_mapper_inheritance.py` & `total-perspective-vortex-2.3.0/tests/test_mapper_inheritance.py`

 * *Files identical despite different names*

### Comparing `total-perspective-vortex-2.2.4/tests/test_mapper_merge_multiple.py` & `total-perspective-vortex-2.3.0/tests/test_mapper_merge_multiple.py`

 * *Files 15% similar despite different names*

```diff
@@ -34,15 +34,15 @@
         with self.assertRaisesRegex(JobMappingException, "Too much data, shouldn't run"):
             self._map_to_destination(tool, user, datasets, tpv_config_paths=[config_first, config_second])
 
         # an intermediate file size should compute correct values
         datasets = [mock_galaxy.DatasetAssociation("test", mock_galaxy.Dataset("test.txt", file_size=7*1024**3))]
         destination = self._map_to_destination(tool, user, datasets, tpv_config_paths=[config_first, config_second])
         self.assertEqual(destination.id, "k8s_environment")
-        self.assertEqual([env['value'] for env in destination.env if env['name'] == 'TEST_JOB_SLOTS'], ['2'])
+        self.assertEqual([env['value'] for env in destination.env if env['name'] == 'TEST_JOB_SLOTS'], ['4'])
         self.assertEqual(destination.params['native_spec'], '--mem 8 --cores 2')
         self.assertEqual(destination.params['custom_context_remote'], 'remote var')
         self.assertEqual(destination.params['custom_context_local'], 'local var')
         self.assertEqual(destination.params['custom_context_override'], 'local override')
 
     def test_merge_local_with_local(self):
         tool = mock_galaxy.Tool('bwa')
@@ -61,15 +61,15 @@
         with self.assertRaisesRegex(JobMappingException, "Too much data, shouldn't run"):
             self._map_to_destination(tool, user, datasets, tpv_config_paths=[config_first, config_second])
 
         # an intermediate file size should compute correct values
         datasets = [mock_galaxy.DatasetAssociation("test", mock_galaxy.Dataset("test.txt", file_size=7*1024**3))]
         destination = self._map_to_destination(tool, user, datasets, tpv_config_paths=[config_first, config_second])
         self.assertEqual(destination.id, "k8s_environment")
-        self.assertEqual([env['value'] for env in destination.env if env['name'] == 'TEST_JOB_SLOTS'], ['2'])
+        self.assertEqual([env['value'] for env in destination.env if env['name'] == 'TEST_JOB_SLOTS'], ['4'])
         self.assertEqual(destination.params['native_spec'], '--mem 8 --cores 2')
         self.assertEqual(destination.params['custom_context_remote'], 'remote var')
         self.assertEqual(destination.params['custom_context_local'], 'local var')
         self.assertEqual(destination.params['custom_context_override'], 'local override')
 
     def test_merge_rules(self):
         tool = mock_galaxy.Tool('bwa')
@@ -100,7 +100,24 @@
         destination = self._map_to_destination(tool, user, datasets, tpv_config_paths=[config_first, config_second])
         self.assertEqual(destination.id, "another_k8s_environment")
         # since the last defined hisat2 contains overridden defaults, those defaults will apply
         self.assertEqual([env['value'] for env in destination.env if env['name'] == 'TEST_JOB_SLOTS'], ['6'])
         # this var is not overridden by the last defined defaults, and therefore, the remote value of cores*2 applies
         self.assertEqual([env['value'] for env in destination.env if env['name'] == 'MORE_JOB_SLOTS'], ['12'])
         self.assertEqual(destination.params['native_spec'], '--mem 18 --cores 6')
+
+    def test_merge_rules_local_defaults_do_not_override_remote_tool(self):
+        tool = mock_galaxy.Tool('toolshed.g2.bx.psu.edu/repos/iuc/disco/disco/v1.0')
+        user = mock_galaxy.User('ford', 'prefect@vortex.org')
+
+        config_first = os.path.join(os.path.dirname(__file__), 'fixtures/mapping-merge-multiple-remote.yml')
+        config_second = os.path.join(os.path.dirname(__file__), 'fixtures/mapping-merge-multiple-local.yml')
+
+        # the disco rules should take effect, with local override winning
+        datasets = [mock_galaxy.DatasetAssociation("test", mock_galaxy.Dataset("test.txt", file_size=42*1024**3))]
+        destination = self._map_to_destination(tool, user, datasets, tpv_config_paths=[config_first, config_second])
+        self.assertEqual(destination.id, "k8s_environment")
+        # since the last defined hisat2 contains overridden defaults, those defaults will apply
+        self.assertEqual([env['value'] for env in destination.env if env['name'] == 'DISCO_MAX_MEMORY'], ['24'])
+        self.assertEqual([env['value'] for env in destination.env if env['name'] == 'DISCO_MORE_PARAMS'], ['just another param'])
+        # this var is not overridden by the last defined defaults, and therefore, the remote value applies
+        self.assertEqual(destination.params['native_spec'], '--mem 24 --cores 8')
```

### Comparing `total-perspective-vortex-2.2.4/tests/test_mapper_params_specific.py` & `total-perspective-vortex-2.3.0/tests/test_mapper_params_specific.py`

 * *Files identical despite different names*

### Comparing `total-perspective-vortex-2.2.4/tests/test_mapper_rank.py` & `total-perspective-vortex-2.3.0/tests/test_mapper_rank.py`

 * *Files identical despite different names*

### Comparing `total-perspective-vortex-2.2.4/tests/test_mapper_resubmit.py` & `total-perspective-vortex-2.3.0/tests/test_mapper_resubmit.py`

 * *Files identical despite different names*

### Comparing `total-perspective-vortex-2.2.4/tests/test_mapper_role.py` & `total-perspective-vortex-2.3.0/tests/test_mapper_role.py`

 * *Files identical despite different names*

### Comparing `total-perspective-vortex-2.2.4/tests/test_mapper_rules.py` & `total-perspective-vortex-2.3.0/tests/test_mapper_rules.py`

 * *Files identical despite different names*

### Comparing `total-perspective-vortex-2.2.4/tests/test_mapper_sample.py` & `total-perspective-vortex-2.3.0/tests/test_mapper_sample.py`

 * *Files identical despite different names*

### Comparing `total-perspective-vortex-2.2.4/tests/test_mapper_user.py` & `total-perspective-vortex-2.3.0/tests/test_mapper_user.py`

 * *Files identical despite different names*

### Comparing `total-perspective-vortex-2.2.4/tests/test_scenarios.py` & `total-perspective-vortex-2.3.0/tests/test_scenarios.py`

 * *Files identical despite different names*

### Comparing `total-perspective-vortex-2.2.4/tests/test_shell.py` & `total-perspective-vortex-2.3.0/tests/test_shell.py`

 * *Files identical despite different names*

### Comparing `total-perspective-vortex-2.2.4/total_perspective_vortex.egg-info/PKG-INFO` & `total-perspective-vortex-2.3.0/total_perspective_vortex.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: total-perspective-vortex
-Version: 2.2.4
+Version: 2.3.0
 Summary: A library for routing entities (jobs, users or groups) to destinations in Galaxy
 Home-page: https://github.com/galaxyproject/total-perspective-vortex
 Author: Galaxy and GVL projects
 Author-email: help@genome.edu.au
 License: MIT
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Programming Language :: Python :: 3
```

### Comparing `total-perspective-vortex-2.2.4/total_perspective_vortex.egg-info/SOURCES.txt` & `total-perspective-vortex-2.3.0/total_perspective_vortex.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `total-perspective-vortex-2.2.4/tpv/commands/dryrunner.py` & `total-perspective-vortex-2.3.0/tpv/commands/dryrunner.py`

 * *Files identical despite different names*

### Comparing `total-perspective-vortex-2.2.4/tpv/commands/formatter.py` & `total-perspective-vortex-2.3.0/tpv/commands/formatter.py`

 * *Files identical despite different names*

### Comparing `total-perspective-vortex-2.2.4/tpv/commands/linter.py` & `total-perspective-vortex-2.3.0/tpv/commands/linter.py`

 * *Files identical despite different names*

### Comparing `total-perspective-vortex-2.2.4/tpv/commands/shell.py` & `total-perspective-vortex-2.3.0/tpv/commands/shell.py`

 * *Files identical despite different names*

### Comparing `total-perspective-vortex-2.2.4/tpv/commands/test/mock_galaxy.py` & `total-perspective-vortex-2.3.0/tpv/commands/test/mock_galaxy.py`

 * *Files identical despite different names*

### Comparing `total-perspective-vortex-2.2.4/tpv/core/entities.py` & `total-perspective-vortex-2.3.0/tpv/core/entities.py`

 * *Files 2% similar despite different names*

```diff
@@ -347,22 +347,15 @@
         :return:
         """
         new_entity = self.override(entity)
         new_entity.id = f"{type(self).__name__}: {self.id}, {type(entity).__name__}: {entity.id}"
         new_entity.tpv_tags = entity.tpv_tags.combine(self.tpv_tags)
         return new_entity
 
-    def evaluate(self, context):
-        """
-        Evaluate expressions in entity properties that must be evaluated as late as possible, which is
-        to say, after combining entity requirements. This includes env, params and resubmit, that rely on
-        properties such as cores, mem and gpus after they are combined.
-        :param context:
-        :return:
-        """
+    def evaluate_resources(self, context):
         new_entity = copy.deepcopy(self)
         context.update(self.context or {})
         if self.min_gpus is not None:
             new_entity.min_gpus = self.loader.eval_code_block(self.min_gpus, context)
             context['min_gpus'] = new_entity.min_gpus
         if self.min_cores is not None:
             new_entity.min_cores = self.loader.eval_code_block(self.min_cores, context)
@@ -393,24 +386,34 @@
             context['cores'] = new_entity.cores
         if self.mem is not None:
             new_entity.mem = self.loader.eval_code_block(self.mem, context)
             # clamp mem
             new_entity.mem = max(new_entity.min_mem or 0, new_entity.mem or 0)
             new_entity.mem = min(new_entity.max_mem, new_entity.mem or 0) if new_entity.max_mem else new_entity.mem
             context['mem'] = new_entity.mem
+        return new_entity
+
+    def evaluate(self, context):
+        """
+        Evaluate expressions in entity properties that must be evaluated as late as possible, which is
+        to say, after combining entity requirements. This includes env, params and resubmit, that rely on
+        properties such as cores, mem and gpus after they are combined.
+        :param context:
+        :return:
+        """
+        new_entity = self.evaluate_resources(context)
         if self.env:
             new_entity.env = self.evaluate_complex_property(self.env, context, stringify=True)
             context['env'] = new_entity.env
         if self.params:
             new_entity.params = self.evaluate_complex_property(self.params, context)
             context['params'] = new_entity.params
         if self.resubmit:
             new_entity.resubmit = self.evaluate_complex_property(self.resubmit, context)
             context['resubmit'] = new_entity.resubmit
-
         return new_entity
 
     def rank_destinations(self, destinations, context):
         if self.rank:
             log.debug(f"Ranking destinations: {destinations} for entity: {self} using custom function")
             context['candidate_destinations'] = destinations
             return self.loader.eval_code_block(self.rank, context)
@@ -474,28 +477,32 @@
         new_entity.rules = copy.deepcopy(entity.rules)
         new_entity.rules.update(self.rules or {})
         for rule in self.rules.values():
             if entity.rules.get(rule.id):
                 new_entity.rules[rule.id] = rule.inherit(entity.rules[rule.id])
         return new_entity
 
-    def evaluate(self, context):
+    def evaluate_rules(self, context):
         new_entity = copy.deepcopy(self)
         context.update(new_entity.context or {})
         for rule in self.rules.values():
             if rule.is_matching(context):
                 rule = rule.evaluate(context)
                 new_entity = rule.inherit(new_entity)
                 new_entity.gpus = rule.gpus or new_entity.gpus
                 new_entity.cores = rule.cores or new_entity.cores
                 new_entity.mem = rule.mem or new_entity.mem
                 new_entity.id = f"{new_entity.id}, Rule: {rule.id}"
                 context.update({
                     'entity': new_entity
                 })
+        return new_entity
+
+    def evaluate(self, context):
+        new_entity = self.evaluate_rules(context)
         return super(EntityWithRules, new_entity).evaluate(context)
 
     def __repr__(self):
         return super().__repr__() + f", rules={self.rules}"
 
 
 class Tool(EntityWithRules):
```

### Comparing `total-perspective-vortex-2.2.4/tpv/core/helpers.py` & `total-perspective-vortex-2.3.0/tpv/core/helpers.py`

 * *Files identical despite different names*

### Comparing `total-perspective-vortex-2.2.4/tpv/core/loader.py` & `total-perspective-vortex-2.3.0/tpv/core/loader.py`

 * *Files 9% similar despite different names*

```diff
@@ -57,21 +57,17 @@
     def process_inheritance(self, entity_list: dict[str, Entity], entity: Entity):
         if entity.inherits:
             parent_entity = entity_list.get(entity.inherits)
             if not parent_entity:
                 raise InvalidParentException(f"The specified parent: {entity.inherits} for"
                                              f" entity: {entity} does not exist")
             return entity.inherit(self.process_inheritance(entity_list, parent_entity))
-        else:
-            default_inherits = self.global_settings.get('default_inherits')
-            if default_inherits and not entity.id == default_inherits:
-                default_parent = entity_list.get(default_inherits)
-                return entity.inherit(default_parent)
-            else:
-                return entity
+        # do not process default inheritance here, only at runtime, as multiple can cause default inheritance
+        # to override later matches.
+        return entity
 
     def recompute_inheritance(self, entities: dict[str, Entity]):
         for key, entity in entities.items():
             entities[key] = self.process_inheritance(entities, entity)
 
     def validate_entities(self, entity_class: type, entity_list: dict) -> dict:
         # This code relies on dict ordering guarantees provided since python 3.6
```

### Comparing `total-perspective-vortex-2.2.4/tpv/core/mapper.py` & `total-perspective-vortex-2.3.0/tpv/core/mapper.py`

 * *Files 8% similar despite different names*

```diff
@@ -31,26 +31,26 @@
             return re.compile(key)
         except re.error:
             log.error(f"Failed to compile regex: {key}")
             raise
 
     def _find_entities_matching_id(self, entity_list, entity_name):
         matches = []
+        if self.default_inherits:
+            default_match = entity_list.get(self.default_inherits)
+            if default_match:
+                matches.append(default_match)
         for key in entity_list.keys():
             if self.lookup_tool_regex(key).match(entity_name):
                 match = entity_list[key]
                 if match.abstract:
                     from galaxy.jobs.mapper import JobMappingException
                     raise JobMappingException(f"This entity is abstract and cannot be mapped : {match}")
                 else:
                     matches.append(match)
-        if not matches and self.default_inherits:
-            default_match = entity_list.get(self.default_inherits)
-            if default_match:
-                matches.append(default_match)
         return matches
 
     def __inherit_matching_entities(self, entity_type, entity_name):
         entity_list = self.entities.get(entity_type)
         matches = self._find_entities_matching_id(entity_list, entity_name)
         return self.inherit_entities(matches)
 
@@ -66,15 +66,17 @@
         else:
             return None
 
     def rank(self, entity, destinations, context):
         return entity.rank_destinations(destinations, context)
 
     def match_and_rank_destinations(self, entity, destinations, context):
-        matches = [dest for dest in destinations.values() if dest.matches(entity, context)]
+        # At this point, the resource requirements (cores, mem, gpus) are unevaluated.
+        # So temporarily evaluate them so we can match up with a destination.
+        matches = [dest for dest in destinations.values() if dest.matches(entity.evaluate_resources(context), context)]
         return self.rank(entity, matches, context)
 
     def to_galaxy_destination(self, destination):
         return JobDestination(
             id=destination.dest_name,
             tags=destination.handler_tags,
             runner=destination.runner,
@@ -112,16 +114,17 @@
         # 2. Combine entity requirements
         combined_entity = self.combine_entities(entity_list)
         context.update({
             'entity': combined_entity,
             'self': combined_entity
         })
 
-        # 3. Evaluate expressions
-        evaluated_entity = combined_entity.evaluate(context)
+        # 3. Evaluate rules only, so that all expressions are collapsed into a flat entity. The final
+        #    values for expressions should be evaluated only after combining with the destination.
+        evaluated_entity = combined_entity.evaluate_rules(context)
         context.update({
             'entity': evaluated_entity,
             'self': evaluated_entity
         })
 
         # Remove the rules as they've already been evaluated, and should not be re-evaluated when combining
         # with destinations
```

### Comparing `total-perspective-vortex-2.2.4/tpv/rules/gateway.py` & `total-perspective-vortex-2.3.0/tpv/rules/gateway.py`

 * *Files identical despite different names*

