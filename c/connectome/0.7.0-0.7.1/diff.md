# Comparing `tmp/connectome-0.7.0.tar.gz` & `tmp/connectome-0.7.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "connectome-0.7.0.tar", last modified: Tue Jun 27 13:35:59 2023, max compression
+gzip compressed data, was "connectome-0.7.1.tar", last modified: Wed Jul  5 00:34:50 2023, max compression
```

## Comparing `connectome-0.7.0.tar` & `connectome-0.7.1.tar`

### file list

```diff
@@ -1,67 +1,67 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 13:35:59.509663 connectome-0.7.0/
--rw-r--r--   0 runner    (1001) docker     (123)    10763 2023-06-27 13:35:52.000000 connectome-0.7.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       93 2023-06-27 13:35:52.000000 connectome-0.7.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)    15337 2023-06-27 13:35:59.509663 connectome-0.7.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1900 2023-06-27 13:35:52.000000 connectome-0.7.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 13:35:59.497662 connectome-0.7.0/connectome/
--rw-r--r--   0 runner    (1001) docker     (123)       84 2023-06-27 13:35:52.000000 connectome-0.7.0/connectome/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-06-27 13:35:52.000000 connectome-0.7.0/connectome/__version__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 13:35:59.497662 connectome-0.7.0/connectome/cache/
--rw-r--r--   0 runner    (1001) docker     (123)      167 2023-06-27 13:35:52.000000 connectome-0.7.0/connectome/cache/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      836 2023-06-27 13:35:52.000000 connectome-0.7.0/connectome/cache/base.py
--rw-r--r--   0 runner    (1001) docker     (123)      676 2023-06-27 13:35:52.000000 connectome-0.7.0/connectome/cache/disk.py
--rw-r--r--   0 runner    (1001) docker     (123)      930 2023-06-27 13:35:52.000000 connectome-0.7.0/connectome/cache/memory.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 13:35:59.497662 connectome-0.7.0/connectome/containers/
--rw-r--r--   0 runner    (1001) docker     (123)       87 2023-06-27 13:35:52.000000 connectome-0.7.0/connectome/containers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10684 2023-06-27 13:35:52.000000 connectome-0.7.0/connectome/containers/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     3989 2023-06-27 13:35:52.000000 connectome-0.7.0/connectome/containers/context.py
--rw-r--r--   0 runner    (1001) docker     (123)     3883 2023-06-27 13:35:52.000000 connectome-0.7.0/connectome/containers/reversible.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 13:35:59.501663 connectome-0.7.0/connectome/engine/
--rw-r--r--   0 runner    (1001) docker     (123)      265 2023-06-27 13:35:52.000000 connectome-0.7.0/connectome/engine/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5557 2023-06-27 13:35:52.000000 connectome-0.7.0/connectome/engine/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     4968 2023-06-27 13:35:52.000000 connectome-0.7.0/connectome/engine/compiler.py
--rw-r--r--   0 runner    (1001) docker     (123)     6423 2023-06-27 13:35:52.000000 connectome-0.7.0/connectome/engine/edges.py
--rw-r--r--   0 runner    (1001) docker     (123)     1799 2023-06-27 13:35:52.000000 connectome-0.7.0/connectome/engine/executor.py
--rw-r--r--   0 runner    (1001) docker     (123)     3984 2023-06-27 13:35:52.000000 connectome-0.7.0/connectome/engine/graph.py
--rw-r--r--   0 runner    (1001) docker     (123)     3401 2023-06-27 13:35:52.000000 connectome-0.7.0/connectome/engine/node_hash.py
--rw-r--r--   0 runner    (1001) docker     (123)      620 2023-06-27 13:35:52.000000 connectome-0.7.0/connectome/engine/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     5012 2023-06-27 13:35:52.000000 connectome-0.7.0/connectome/engine/vm.py
--rw-r--r--   0 runner    (1001) docker     (123)      195 2023-06-27 13:35:52.000000 connectome-0.7.0/connectome/exceptions.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 13:35:59.505663 connectome-0.7.0/connectome/interface/
--rw-r--r--   0 runner    (1001) docker     (123)      195 2023-06-27 13:35:52.000000 connectome-0.7.0/connectome/interface/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       50 2023-06-27 13:35:52.000000 connectome-0.7.0/connectome/interface/blocks.py
--rw-r--r--   0 runner    (1001) docker     (123)     1762 2023-06-27 13:35:52.000000 connectome-0.7.0/connectome/interface/complex_edges.py
--rw-r--r--   0 runner    (1001) docker     (123)      338 2023-06-27 13:35:52.000000 connectome-0.7.0/connectome/interface/decorators.py
--rw-r--r--   0 runner    (1001) docker     (123)     6743 2023-06-27 13:35:52.000000 connectome-0.7.0/connectome/interface/edges.py
--rw-r--r--   0 runner    (1001) docker     (123)    17546 2023-06-27 13:35:52.000000 connectome-0.7.0/connectome/interface/factory.py
--rw-r--r--   0 runner    (1001) docker     (123)      369 2023-06-27 13:35:52.000000 connectome-0.7.0/connectome/interface/factory_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     4068 2023-06-27 13:35:52.000000 connectome-0.7.0/connectome/interface/metaclasses.py
--rw-r--r--   0 runner    (1001) docker     (123)     1679 2023-06-27 13:35:52.000000 connectome-0.7.0/connectome/interface/nodes.py
--rw-r--r--   0 runner    (1001) docker     (123)     1859 2023-06-27 13:35:52.000000 connectome-0.7.0/connectome/interface/split.py
--rw-r--r--   0 runner    (1001) docker     (123)      845 2023-06-27 13:35:52.000000 connectome-0.7.0/connectome/interface/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 13:35:59.509663 connectome-0.7.0/connectome/layers/
--rw-r--r--   0 runner    (1001) docker     (123)      322 2023-06-27 13:35:52.000000 connectome-0.7.0/connectome/layers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1309 2023-06-27 13:35:52.000000 connectome-0.7.0/connectome/layers/apply.py
--rw-r--r--   0 runner    (1001) docker     (123)     5929 2023-06-27 13:35:52.000000 connectome-0.7.0/connectome/layers/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     5846 2023-06-27 13:35:52.000000 connectome-0.7.0/connectome/layers/cache.py
--rw-r--r--   0 runner    (1001) docker     (123)      261 2023-06-27 13:35:52.000000 connectome-0.7.0/connectome/layers/chain.py
--rw-r--r--   0 runner    (1001) docker     (123)     6643 2023-06-27 13:35:52.000000 connectome-0.7.0/connectome/layers/columns.py
--rw-r--r--   0 runner    (1001) docker     (123)     2066 2023-06-27 13:35:52.000000 connectome-0.7.0/connectome/layers/debug.py
--rw-r--r--   0 runner    (1001) docker     (123)      463 2023-06-27 13:35:52.000000 connectome-0.7.0/connectome/layers/dynamic.py
--rw-r--r--   0 runner    (1001) docker     (123)     3533 2023-06-27 13:35:52.000000 connectome-0.7.0/connectome/layers/filter.py
--rw-r--r--   0 runner    (1001) docker     (123)     4611 2023-06-27 13:35:52.000000 connectome-0.7.0/connectome/layers/group.py
--rw-r--r--   0 runner    (1001) docker     (123)    11198 2023-06-27 13:35:52.000000 connectome-0.7.0/connectome/layers/join.py
--rw-r--r--   0 runner    (1001) docker     (123)     4367 2023-06-27 13:35:52.000000 connectome-0.7.0/connectome/layers/merge.py
--rw-r--r--   0 runner    (1001) docker     (123)     4307 2023-06-27 13:35:52.000000 connectome-0.7.0/connectome/layers/split.py
--rw-r--r--   0 runner    (1001) docker     (123)       54 2023-06-27 13:35:52.000000 connectome-0.7.0/connectome/serializers.py
--rw-r--r--   0 runner    (1001) docker     (123)     4193 2023-06-27 13:35:52.000000 connectome-0.7.0/connectome/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 13:35:59.497662 connectome-0.7.0/connectome.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    15337 2023-06-27 13:35:59.000000 connectome-0.7.0/connectome.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1570 2023-06-27 13:35:59.000000 connectome-0.7.0/connectome.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-27 13:35:59.000000 connectome-0.7.0/connectome.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       47 2023-06-27 13:35:59.000000 connectome-0.7.0/connectome.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       11 2023-06-27 13:35:59.000000 connectome-0.7.0/connectome.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1840 2023-06-27 13:35:52.000000 connectome-0.7.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       47 2023-06-27 13:35:52.000000 connectome-0.7.0/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-27 13:35:59.509663 connectome-0.7.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1478 2023-06-27 13:35:52.000000 connectome-0.7.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 00:34:50.977531 connectome-0.7.1/
+-rw-r--r--   0 runner    (1001) docker     (123)    10763 2023-07-05 00:34:47.000000 connectome-0.7.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       93 2023-07-05 00:34:47.000000 connectome-0.7.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)    15337 2023-07-05 00:34:50.977531 connectome-0.7.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1900 2023-07-05 00:34:47.000000 connectome-0.7.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 00:34:50.973531 connectome-0.7.1/connectome/
+-rw-r--r--   0 runner    (1001) docker     (123)       84 2023-07-05 00:34:47.000000 connectome-0.7.1/connectome/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-07-05 00:34:47.000000 connectome-0.7.1/connectome/__version__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 00:34:50.973531 connectome-0.7.1/connectome/cache/
+-rw-r--r--   0 runner    (1001) docker     (123)      167 2023-07-05 00:34:47.000000 connectome-0.7.1/connectome/cache/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      836 2023-07-05 00:34:47.000000 connectome-0.7.1/connectome/cache/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)      676 2023-07-05 00:34:47.000000 connectome-0.7.1/connectome/cache/disk.py
+-rw-r--r--   0 runner    (1001) docker     (123)      930 2023-07-05 00:34:47.000000 connectome-0.7.1/connectome/cache/memory.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 00:34:50.973531 connectome-0.7.1/connectome/containers/
+-rw-r--r--   0 runner    (1001) docker     (123)       87 2023-07-05 00:34:47.000000 connectome-0.7.1/connectome/containers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10684 2023-07-05 00:34:47.000000 connectome-0.7.1/connectome/containers/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3989 2023-07-05 00:34:47.000000 connectome-0.7.1/connectome/containers/context.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3883 2023-07-05 00:34:47.000000 connectome-0.7.1/connectome/containers/reversible.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 00:34:50.973531 connectome-0.7.1/connectome/engine/
+-rw-r--r--   0 runner    (1001) docker     (123)      265 2023-07-05 00:34:47.000000 connectome-0.7.1/connectome/engine/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5557 2023-07-05 00:34:47.000000 connectome-0.7.1/connectome/engine/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4968 2023-07-05 00:34:47.000000 connectome-0.7.1/connectome/engine/compiler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6423 2023-07-05 00:34:47.000000 connectome-0.7.1/connectome/engine/edges.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1799 2023-07-05 00:34:47.000000 connectome-0.7.1/connectome/engine/executor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3984 2023-07-05 00:34:47.000000 connectome-0.7.1/connectome/engine/graph.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3401 2023-07-05 00:34:47.000000 connectome-0.7.1/connectome/engine/node_hash.py
+-rw-r--r--   0 runner    (1001) docker     (123)      620 2023-07-05 00:34:47.000000 connectome-0.7.1/connectome/engine/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5012 2023-07-05 00:34:47.000000 connectome-0.7.1/connectome/engine/vm.py
+-rw-r--r--   0 runner    (1001) docker     (123)      195 2023-07-05 00:34:47.000000 connectome-0.7.1/connectome/exceptions.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 00:34:50.977531 connectome-0.7.1/connectome/interface/
+-rw-r--r--   0 runner    (1001) docker     (123)      195 2023-07-05 00:34:47.000000 connectome-0.7.1/connectome/interface/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       50 2023-07-05 00:34:47.000000 connectome-0.7.1/connectome/interface/blocks.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1762 2023-07-05 00:34:47.000000 connectome-0.7.1/connectome/interface/complex_edges.py
+-rw-r--r--   0 runner    (1001) docker     (123)      338 2023-07-05 00:34:47.000000 connectome-0.7.1/connectome/interface/decorators.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6743 2023-07-05 00:34:47.000000 connectome-0.7.1/connectome/interface/edges.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17982 2023-07-05 00:34:47.000000 connectome-0.7.1/connectome/interface/factory.py
+-rw-r--r--   0 runner    (1001) docker     (123)      369 2023-07-05 00:34:47.000000 connectome-0.7.1/connectome/interface/factory_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4068 2023-07-05 00:34:47.000000 connectome-0.7.1/connectome/interface/metaclasses.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1679 2023-07-05 00:34:47.000000 connectome-0.7.1/connectome/interface/nodes.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1859 2023-07-05 00:34:47.000000 connectome-0.7.1/connectome/interface/split.py
+-rw-r--r--   0 runner    (1001) docker     (123)      845 2023-07-05 00:34:47.000000 connectome-0.7.1/connectome/interface/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 00:34:50.977531 connectome-0.7.1/connectome/layers/
+-rw-r--r--   0 runner    (1001) docker     (123)      322 2023-07-05 00:34:47.000000 connectome-0.7.1/connectome/layers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1309 2023-07-05 00:34:47.000000 connectome-0.7.1/connectome/layers/apply.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5929 2023-07-05 00:34:47.000000 connectome-0.7.1/connectome/layers/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5846 2023-07-05 00:34:47.000000 connectome-0.7.1/connectome/layers/cache.py
+-rw-r--r--   0 runner    (1001) docker     (123)      261 2023-07-05 00:34:47.000000 connectome-0.7.1/connectome/layers/chain.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6643 2023-07-05 00:34:47.000000 connectome-0.7.1/connectome/layers/columns.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2066 2023-07-05 00:34:47.000000 connectome-0.7.1/connectome/layers/debug.py
+-rw-r--r--   0 runner    (1001) docker     (123)      463 2023-07-05 00:34:47.000000 connectome-0.7.1/connectome/layers/dynamic.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3533 2023-07-05 00:34:47.000000 connectome-0.7.1/connectome/layers/filter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4611 2023-07-05 00:34:47.000000 connectome-0.7.1/connectome/layers/group.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11198 2023-07-05 00:34:47.000000 connectome-0.7.1/connectome/layers/join.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4367 2023-07-05 00:34:47.000000 connectome-0.7.1/connectome/layers/merge.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4307 2023-07-05 00:34:47.000000 connectome-0.7.1/connectome/layers/split.py
+-rw-r--r--   0 runner    (1001) docker     (123)       54 2023-07-05 00:34:47.000000 connectome-0.7.1/connectome/serializers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4193 2023-07-05 00:34:47.000000 connectome-0.7.1/connectome/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 00:34:50.973531 connectome-0.7.1/connectome.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    15337 2023-07-05 00:34:50.000000 connectome-0.7.1/connectome.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1570 2023-07-05 00:34:50.000000 connectome-0.7.1/connectome.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-05 00:34:50.000000 connectome-0.7.1/connectome.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       47 2023-07-05 00:34:50.000000 connectome-0.7.1/connectome.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       11 2023-07-05 00:34:50.000000 connectome-0.7.1/connectome.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1840 2023-07-05 00:34:47.000000 connectome-0.7.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       47 2023-07-05 00:34:47.000000 connectome-0.7.1/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-05 00:34:50.977531 connectome-0.7.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1478 2023-07-05 00:34:47.000000 connectome-0.7.1/setup.py
```

### Comparing `connectome-0.7.0/LICENSE` & `connectome-0.7.1/LICENSE`

 * *Files identical despite different names*

### Comparing `connectome-0.7.0/PKG-INFO` & `connectome-0.7.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: connectome
-Version: 0.7.0
+Version: 0.7.1
 Summary: A library for datasets containing heterogeneous data
 Home-page: https://github.com/neuro-ml/connectome
-Download-URL: https://github.com/neuro-ml/connectome/archive/v0.7.0.tar.gz
+Download-URL: https://github.com/neuro-ml/connectome/archive/v0.7.1.tar.gz
 Author: NeuroML Group
 Author-email: NeuroML Group <max@ira-labs.com>
 License:                                  Apache License
                                    Version 2.0, January 2004
                                 http://www.apache.org/licenses/
         
            TERMS AND CONDITIONS FOR USE, REPRODUCTION, AND DISTRIBUTION
```

### Comparing `connectome-0.7.0/README.md` & `connectome-0.7.1/README.md`

 * *Files identical despite different names*

### Comparing `connectome-0.7.0/connectome/cache/base.py` & `connectome-0.7.1/connectome/cache/base.py`

 * *Files identical despite different names*

### Comparing `connectome-0.7.0/connectome/cache/disk.py` & `connectome-0.7.1/connectome/cache/disk.py`

 * *Files identical despite different names*

### Comparing `connectome-0.7.0/connectome/cache/memory.py` & `connectome-0.7.1/connectome/cache/memory.py`

 * *Files identical despite different names*

### Comparing `connectome-0.7.0/connectome/containers/base.py` & `connectome-0.7.1/connectome/containers/base.py`

 * *Files identical despite different names*

### Comparing `connectome-0.7.0/connectome/containers/context.py` & `connectome-0.7.1/connectome/containers/context.py`

 * *Files identical despite different names*

### Comparing `connectome-0.7.0/connectome/containers/reversible.py` & `connectome-0.7.1/connectome/containers/reversible.py`

 * *Files identical despite different names*

### Comparing `connectome-0.7.0/connectome/engine/base.py` & `connectome-0.7.1/connectome/engine/base.py`

 * *Files identical despite different names*

### Comparing `connectome-0.7.0/connectome/engine/compiler.py` & `connectome-0.7.1/connectome/engine/compiler.py`

 * *Files identical despite different names*

### Comparing `connectome-0.7.0/connectome/engine/edges.py` & `connectome-0.7.1/connectome/engine/edges.py`

 * *Files identical despite different names*

### Comparing `connectome-0.7.0/connectome/engine/executor.py` & `connectome-0.7.1/connectome/engine/executor.py`

 * *Files identical despite different names*

### Comparing `connectome-0.7.0/connectome/engine/graph.py` & `connectome-0.7.1/connectome/engine/graph.py`

 * *Files identical despite different names*

### Comparing `connectome-0.7.0/connectome/engine/node_hash.py` & `connectome-0.7.1/connectome/engine/node_hash.py`

 * *Files identical despite different names*

### Comparing `connectome-0.7.0/connectome/engine/utils.py` & `connectome-0.7.1/connectome/engine/utils.py`

 * *Files identical despite different names*

### Comparing `connectome-0.7.0/connectome/engine/vm.py` & `connectome-0.7.1/connectome/engine/vm.py`

 * *Files identical despite different names*

### Comparing `connectome-0.7.0/connectome/interface/complex_edges.py` & `connectome-0.7.1/connectome/interface/complex_edges.py`

 * *Files identical despite different names*

### Comparing `connectome-0.7.0/connectome/interface/edges.py` & `connectome-0.7.1/connectome/interface/edges.py`

 * *Files identical despite different names*

### Comparing `connectome-0.7.0/connectome/interface/factory.py` & `connectome-0.7.1/connectome/interface/factory.py`

 * *Files 0% similar despite different names*

```diff
@@ -204,26 +204,34 @@
                 raise FieldError(f"{type(value).__name__} objects can't be private ({name}).")
 
             self.parameters.add(name)
             # we have 2 edge cases here:
             is_argument = False
             if callable(value):
                 #  1. a callable argument without annotation: x = some_func
-                inside_body = getattr(value, '__qualname__', '').startswith(self.name)
+                qualname = getattr(value, '__qualname__', '')
+                # if we can't detect this better not to annoy the user
+                inside_body = None
+                if qualname.count('.') >= 1:
+                    scope, func_name = qualname.rsplit('.', 1)
+                    # lambdas are a special case. don't know what to do with them
+                    if func_name != '<lambda>':
+                        inside_body = scope.endswith(self.name)
+
                 if name not in annotations:
-                    if not inside_body:
+                    if inside_body is not None and not inside_body:
                         warnings.warn(
                             f'The parameter {name} is defined outside of the class body. Are you trying to pass '
                             f'a default value for an argument? If so, add a type annotation: "{name}: Callable = ..."',
                             UserWarning,
                         )
                 # a function defined inside the body, which also has a type annotation
                 else:
                     is_argument = True
-                    if not inside_body:
+                    if inside_body is not None and inside_body:
                         warnings.warn(
                             f'The default value for the argument {name} is a function, defined inside of the '
                             f'class body. Did you forget to remove the type annotation?',
                             UserWarning,
                         )
 
             if is_argument or not is_detectable(value) or value is inspect.Parameter.empty:
```

### Comparing `connectome-0.7.0/connectome/interface/metaclasses.py` & `connectome-0.7.1/connectome/interface/metaclasses.py`

 * *Files identical despite different names*

### Comparing `connectome-0.7.0/connectome/interface/nodes.py` & `connectome-0.7.1/connectome/interface/nodes.py`

 * *Files identical despite different names*

### Comparing `connectome-0.7.0/connectome/interface/split.py` & `connectome-0.7.1/connectome/interface/split.py`

 * *Files identical despite different names*

### Comparing `connectome-0.7.0/connectome/interface/utils.py` & `connectome-0.7.1/connectome/interface/utils.py`

 * *Files identical despite different names*

### Comparing `connectome-0.7.0/connectome/layers/apply.py` & `connectome-0.7.1/connectome/layers/apply.py`

 * *Files identical despite different names*

### Comparing `connectome-0.7.0/connectome/layers/base.py` & `connectome-0.7.1/connectome/layers/base.py`

 * *Files identical despite different names*

### Comparing `connectome-0.7.0/connectome/layers/cache.py` & `connectome-0.7.1/connectome/layers/cache.py`

 * *Files identical despite different names*

### Comparing `connectome-0.7.0/connectome/layers/columns.py` & `connectome-0.7.1/connectome/layers/columns.py`

 * *Files identical despite different names*

### Comparing `connectome-0.7.0/connectome/layers/debug.py` & `connectome-0.7.1/connectome/layers/debug.py`

 * *Files identical despite different names*

### Comparing `connectome-0.7.0/connectome/layers/filter.py` & `connectome-0.7.1/connectome/layers/filter.py`

 * *Files identical despite different names*

### Comparing `connectome-0.7.0/connectome/layers/group.py` & `connectome-0.7.1/connectome/layers/group.py`

 * *Files identical despite different names*

### Comparing `connectome-0.7.0/connectome/layers/join.py` & `connectome-0.7.1/connectome/layers/join.py`

 * *Files identical despite different names*

### Comparing `connectome-0.7.0/connectome/layers/merge.py` & `connectome-0.7.1/connectome/layers/merge.py`

 * *Files identical despite different names*

### Comparing `connectome-0.7.0/connectome/layers/split.py` & `connectome-0.7.1/connectome/layers/split.py`

 * *Files identical despite different names*

### Comparing `connectome-0.7.0/connectome/utils.py` & `connectome-0.7.1/connectome/utils.py`

 * *Files identical despite different names*

### Comparing `connectome-0.7.0/connectome.egg-info/PKG-INFO` & `connectome-0.7.1/connectome.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: connectome
-Version: 0.7.0
+Version: 0.7.1
 Summary: A library for datasets containing heterogeneous data
 Home-page: https://github.com/neuro-ml/connectome
-Download-URL: https://github.com/neuro-ml/connectome/archive/v0.7.0.tar.gz
+Download-URL: https://github.com/neuro-ml/connectome/archive/v0.7.1.tar.gz
 Author: NeuroML Group
 Author-email: NeuroML Group <max@ira-labs.com>
 License:                                  Apache License
                                    Version 2.0, January 2004
                                 http://www.apache.org/licenses/
         
            TERMS AND CONDITIONS FOR USE, REPRODUCTION, AND DISTRIBUTION
```

### Comparing `connectome-0.7.0/connectome.egg-info/SOURCES.txt` & `connectome-0.7.1/connectome.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `connectome-0.7.0/pyproject.toml` & `connectome-0.7.1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `connectome-0.7.0/setup.py` & `connectome-0.7.1/setup.py`

 * *Files identical despite different names*

