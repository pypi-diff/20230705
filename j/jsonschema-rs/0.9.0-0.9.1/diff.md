# Comparing `tmp/jsonschema_rs-0.9.0.tar.gz` & `tmp/jsonschema_rs-0.9.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/jsonschema_rs-0.9.0.tar", last modified: Fri May  7 07:08:19 2021, max compression
+gzip compressed data, was "dist/jsonschema_rs-0.9.1.tar", last modified: Thu Jun 17 11:38:18 2021, max compression
```

## Comparing `jsonschema_rs-0.9.0.tar` & `jsonschema_rs-0.9.1.tar`

### file list

```diff
@@ -1,86 +1,86 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-05-07 07:08:19.000000 jsonschema_rs-0.9.0/
--rw-r--r--   0 runner    (1001) docker     (121)     1399 2021-05-07 07:08:18.000000 jsonschema_rs-0.9.0/Cargo.toml
--rw-r--r--   0 runner    (1001) docker     (121)      316 2021-05-07 07:07:47.000000 jsonschema_rs-0.9.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (121)    12368 2021-05-07 07:08:19.000000 jsonschema_rs-0.9.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)    10032 2021-05-07 07:07:47.000000 jsonschema_rs-0.9.0/README.rst
--rw-r--r--   0 runner    (1001) docker     (121)      415 2021-05-07 07:07:47.000000 jsonschema_rs-0.9.0/build.rs
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-05-07 07:08:18.000000 jsonschema_rs-0.9.0/jsonschema-lib/
--rw-r--r--   0 runner    (1001) docker     (121)     1348 2021-05-07 07:07:47.000000 jsonschema_rs-0.9.0/jsonschema-lib/Cargo.toml
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-05-07 07:08:18.000000 jsonschema_rs-0.9.0/jsonschema-lib/benches/
--rw-r--r--   0 runner    (1001) docker     (121)    18926 2021-05-07 07:07:47.000000 jsonschema_rs-0.9.0/jsonschema-lib/benches/jsonschema.rs
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-05-07 07:08:18.000000 jsonschema_rs-0.9.0/jsonschema-lib/meta_schemas/
--rw-r--r--   0 runner    (1001) docker     (121)     4357 2021-05-07 07:07:47.000000 jsonschema_rs-0.9.0/jsonschema-lib/meta_schemas/draft4.json
--rw-r--r--   0 runner    (1001) docker     (121)     4497 2021-05-07 07:07:47.000000 jsonschema_rs-0.9.0/jsonschema-lib/meta_schemas/draft6.json
--rw-r--r--   0 runner    (1001) docker     (121)     4979 2021-05-07 07:07:47.000000 jsonschema_rs-0.9.0/jsonschema-lib/meta_schemas/draft7.json
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-05-07 07:08:18.000000 jsonschema_rs-0.9.0/jsonschema-lib/src/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-05-07 07:08:18.000000 jsonschema_rs-0.9.0/jsonschema-lib/src/compilation/
--rw-r--r--   0 runner    (1001) docker     (121)     1944 2021-05-07 07:07:47.000000 jsonschema_rs-0.9.0/jsonschema-lib/src/compilation/context.rs
--rw-r--r--   0 runner    (1001) docker     (121)     7115 2021-05-07 07:07:47.000000 jsonschema_rs-0.9.0/jsonschema-lib/src/compilation/mod.rs
--rw-r--r--   0 runner    (1001) docker     (121)    13691 2021-05-07 07:07:47.000000 jsonschema_rs-0.9.0/jsonschema-lib/src/compilation/options.rs
--rw-r--r--   0 runner    (1001) docker     (121)      981 2021-05-07 07:07:47.000000 jsonschema_rs-0.9.0/jsonschema-lib/src/content_encoding.rs
--rw-r--r--   0 runner    (1001) docker     (121)      539 2021-05-07 07:07:47.000000 jsonschema_rs-0.9.0/jsonschema-lib/src/content_media_type.rs
--rw-r--r--   0 runner    (1001) docker     (121)    37022 2021-05-07 07:07:47.000000 jsonschema_rs-0.9.0/jsonschema-lib/src/error.rs
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-05-07 07:08:19.000000 jsonschema_rs-0.9.0/jsonschema-lib/src/keywords/
--rw-r--r--   0 runner    (1001) docker     (121)     4461 2021-05-07 07:07:47.000000 jsonschema_rs-0.9.0/jsonschema-lib/src/keywords/additional_items.rs
--rw-r--r--   0 runner    (1001) docker     (121)    50864 2021-05-07 07:07:47.000000 jsonschema_rs-0.9.0/jsonschema-lib/src/keywords/additional_properties.rs
--rw-r--r--   0 runner    (1001) docker     (121)     3438 2021-05-07 07:07:47.000000 jsonschema_rs-0.9.0/jsonschema-lib/src/keywords/all_of.rs
--rw-r--r--   0 runner    (1001) docker     (121)     1983 2021-05-07 07:07:47.000000 jsonschema_rs-0.9.0/jsonschema-lib/src/keywords/any_of.rs
--rw-r--r--   0 runner    (1001) docker     (121)      886 2021-05-07 07:07:47.000000 jsonschema_rs-0.9.0/jsonschema-lib/src/keywords/boolean.rs
--rw-r--r--   0 runner    (1001) docker     (121)     7898 2021-05-07 07:07:47.000000 jsonschema_rs-0.9.0/jsonschema-lib/src/keywords/const_.rs
--rw-r--r--   0 runner    (1001) docker     (121)     2108 2021-05-07 07:07:47.000000 jsonschema_rs-0.9.0/jsonschema-lib/src/keywords/contains.rs
--rw-r--r--   0 runner    (1001) docker     (121)     7882 2021-05-07 07:07:47.000000 jsonschema_rs-0.9.0/jsonschema-lib/src/keywords/content.rs
--rw-r--r--   0 runner    (1001) docker     (121)     3037 2021-05-07 07:07:47.000000 jsonschema_rs-0.9.0/jsonschema-lib/src/keywords/dependencies.rs
--rw-r--r--   0 runner    (1001) docker     (121)     3741 2021-05-07 07:07:47.000000 jsonschema_rs-0.9.0/jsonschema-lib/src/keywords/enum_.rs
--rw-r--r--   0 runner    (1001) docker     (121)     4399 2021-05-07 07:07:47.000000 jsonschema_rs-0.9.0/jsonschema-lib/src/keywords/exclusive_maximum.rs
--rw-r--r--   0 runner    (1001) docker     (121)     4365 2021-05-07 07:07:47.000000 jsonschema_rs-0.9.0/jsonschema-lib/src/keywords/exclusive_minimum.rs
--rw-r--r--   0 runner    (1001) docker     (121)    12945 2021-05-07 07:07:47.000000 jsonschema_rs-0.9.0/jsonschema-lib/src/keywords/format.rs
--rw-r--r--   0 runner    (1001) docker     (121)     2347 2021-05-07 07:07:47.000000 jsonschema_rs-0.9.0/jsonschema-lib/src/keywords/helpers.rs
--rw-r--r--   0 runner    (1001) docker     (121)     6702 2021-05-07 07:07:47.000000 jsonschema_rs-0.9.0/jsonschema-lib/src/keywords/if_.rs
--rw-r--r--   0 runner    (1001) docker     (121)     4278 2021-05-07 07:07:47.000000 jsonschema_rs-0.9.0/jsonschema-lib/src/keywords/items.rs
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-05-07 07:08:19.000000 jsonschema_rs-0.9.0/jsonschema-lib/src/keywords/legacy/
--rw-r--r--   0 runner    (1001) docker     (121)      510 2021-05-07 07:07:47.000000 jsonschema_rs-0.9.0/jsonschema-lib/src/keywords/legacy/maximum_draft_4.rs
--rw-r--r--   0 runner    (1001) docker     (121)      510 2021-05-07 07:07:47.000000 jsonschema_rs-0.9.0/jsonschema-lib/src/keywords/legacy/minimum_draft_4.rs
--rw-r--r--   0 runner    (1001) docker     (121)       93 2021-05-07 07:07:47.000000 jsonschema_rs-0.9.0/jsonschema-lib/src/keywords/legacy/mod.rs
--rw-r--r--   0 runner    (1001) docker     (121)     5139 2021-05-07 07:07:47.000000 jsonschema_rs-0.9.0/jsonschema-lib/src/keywords/legacy/type_draft_4.rs
--rw-r--r--   0 runner    (1001) docker     (121)     1700 2021-05-07 07:07:47.000000 jsonschema_rs-0.9.0/jsonschema-lib/src/keywords/max_items.rs
--rw-r--r--   0 runner    (1001) docker     (121)     1732 2021-05-07 07:07:47.000000 jsonschema_rs-0.9.0/jsonschema-lib/src/keywords/max_length.rs
--rw-r--r--   0 runner    (1001) docker     (121)     1738 2021-05-07 07:07:47.000000 jsonschema_rs-0.9.0/jsonschema-lib/src/keywords/max_properties.rs
--rw-r--r--   0 runner    (1001) docker     (121)     4082 2021-05-07 07:07:47.000000 jsonschema_rs-0.9.0/jsonschema-lib/src/keywords/maximum.rs
--rw-r--r--   0 runner    (1001) docker     (121)     1700 2021-05-07 07:07:47.000000 jsonschema_rs-0.9.0/jsonschema-lib/src/keywords/min_items.rs
--rw-r--r--   0 runner    (1001) docker     (121)     1726 2021-05-07 07:07:47.000000 jsonschema_rs-0.9.0/jsonschema-lib/src/keywords/min_length.rs
--rw-r--r--   0 runner    (1001) docker     (121)     1738 2021-05-07 07:07:47.000000 jsonschema_rs-0.9.0/jsonschema-lib/src/keywords/min_properties.rs
--rw-r--r--   0 runner    (1001) docker     (121)     4082 2021-05-07 07:07:47.000000 jsonschema_rs-0.9.0/jsonschema-lib/src/keywords/minimum.rs
--rw-r--r--   0 runner    (1001) docker     (121)    17626 2021-05-07 07:07:47.000000 jsonschema_rs-0.9.0/jsonschema-lib/src/keywords/mod.rs
--rw-r--r--   0 runner    (1001) docker     (121)     3864 2021-05-07 07:07:47.000000 jsonschema_rs-0.9.0/jsonschema-lib/src/keywords/multiple_of.rs
--rw-r--r--   0 runner    (1001) docker     (121)     1723 2021-05-07 07:07:47.000000 jsonschema_rs-0.9.0/jsonschema-lib/src/keywords/not.rs
--rw-r--r--   0 runner    (1001) docker     (121)     3368 2021-05-07 07:07:47.000000 jsonschema_rs-0.9.0/jsonschema-lib/src/keywords/one_of.rs
--rw-r--r--   0 runner    (1001) docker     (121)     6021 2021-05-07 07:07:47.000000 jsonschema_rs-0.9.0/jsonschema-lib/src/keywords/pattern.rs
--rw-r--r--   0 runner    (1001) docker     (121)     5932 2021-05-07 07:07:47.000000 jsonschema_rs-0.9.0/jsonschema-lib/src/keywords/pattern_properties.rs
--rw-r--r--   0 runner    (1001) docker     (121)     3040 2021-05-07 07:07:47.000000 jsonschema_rs-0.9.0/jsonschema-lib/src/keywords/properties.rs
--rw-r--r--   0 runner    (1001) docker     (121)     3926 2021-05-07 07:07:47.000000 jsonschema_rs-0.9.0/jsonschema-lib/src/keywords/property_names.rs
--rw-r--r--   0 runner    (1001) docker     (121)     3919 2021-05-07 07:07:47.000000 jsonschema_rs-0.9.0/jsonschema-lib/src/keywords/ref_.rs
--rw-r--r--   0 runner    (1001) docker     (121)     4005 2021-05-07 07:07:47.000000 jsonschema_rs-0.9.0/jsonschema-lib/src/keywords/required.rs
--rw-r--r--   0 runner    (1001) docker     (121)    10471 2021-05-07 07:07:47.000000 jsonschema_rs-0.9.0/jsonschema-lib/src/keywords/type_.rs
--rw-r--r--   0 runner    (1001) docker     (121)     4496 2021-05-07 07:07:47.000000 jsonschema_rs-0.9.0/jsonschema-lib/src/keywords/unique_items.rs
--rw-r--r--   0 runner    (1001) docker     (121)     5447 2021-05-07 07:07:47.000000 jsonschema_rs-0.9.0/jsonschema-lib/src/lib.rs
--rw-r--r--   0 runner    (1001) docker     (121)     2108 2021-05-07 07:07:47.000000 jsonschema_rs-0.9.0/jsonschema-lib/src/main.rs
--rw-r--r--   0 runner    (1001) docker     (121)     4400 2021-05-07 07:07:47.000000 jsonschema_rs-0.9.0/jsonschema-lib/src/paths.rs
--rw-r--r--   0 runner    (1001) docker     (121)     5517 2021-05-07 07:07:47.000000 jsonschema_rs-0.9.0/jsonschema-lib/src/primitive_type.rs
--rw-r--r--   0 runner    (1001) docker     (121)    16219 2021-05-07 07:07:47.000000 jsonschema_rs-0.9.0/jsonschema-lib/src/resolver.rs
--rw-r--r--   0 runner    (1001) docker     (121)     5845 2021-05-07 07:07:47.000000 jsonschema_rs-0.9.0/jsonschema-lib/src/schemas.rs
--rw-r--r--   0 runner    (1001) docker     (121)      745 2021-05-07 07:07:47.000000 jsonschema_rs-0.9.0/jsonschema-lib/src/validator.rs
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-05-07 07:08:19.000000 jsonschema_rs-0.9.0/jsonschema_rs.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)    12368 2021-05-07 07:08:18.000000 jsonschema_rs-0.9.0/jsonschema_rs.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     2621 2021-05-07 07:08:18.000000 jsonschema_rs-0.9.0/jsonschema_rs.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2021-05-07 07:08:18.000000 jsonschema_rs-0.9.0/jsonschema_rs.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2021-05-07 07:08:18.000000 jsonschema_rs-0.9.0/jsonschema_rs.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (121)        1 2021-05-07 07:08:18.000000 jsonschema_rs-0.9.0/jsonschema_rs.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (121)      340 2021-05-07 07:07:47.000000 jsonschema_rs-0.9.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (121)        7 2021-05-07 07:07:47.000000 jsonschema_rs-0.9.0/rust-toolchain
--rw-r--r--   0 runner    (1001) docker     (121)       38 2021-05-07 07:08:19.000000 jsonschema_rs-0.9.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)     1910 2021-05-07 07:07:47.000000 jsonschema_rs-0.9.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-05-07 07:08:19.000000 jsonschema_rs-0.9.0/src/
--rw-r--r--   0 runner    (1001) docker     (121)     8678 2021-05-07 07:07:47.000000 jsonschema_rs-0.9.0/src/lib.rs
--rw-r--r--   0 runner    (1001) docker     (121)     6653 2021-05-07 07:07:47.000000 jsonschema_rs-0.9.0/src/ser.rs
--rw-r--r--   0 runner    (1001) docker     (121)     1629 2021-05-07 07:07:47.000000 jsonschema_rs-0.9.0/src/string.rs
--rw-r--r--   0 runner    (1001) docker     (121)     1284 2021-05-07 07:07:47.000000 jsonschema_rs-0.9.0/src/types.rs
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-06-17 11:38:18.000000 jsonschema_rs-0.9.1/
+-rw-r--r--   0 runner    (1001) docker     (121)     1399 2021-06-17 11:38:18.000000 jsonschema_rs-0.9.1/Cargo.toml
+-rw-r--r--   0 runner    (1001) docker     (121)      316 2021-06-17 11:37:54.000000 jsonschema_rs-0.9.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (121)    11029 2021-06-17 11:38:18.000000 jsonschema_rs-0.9.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (121)    10032 2021-06-17 11:37:54.000000 jsonschema_rs-0.9.1/README.rst
+-rw-r--r--   0 runner    (1001) docker     (121)      415 2021-06-17 11:37:54.000000 jsonschema_rs-0.9.1/build.rs
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-06-17 11:38:18.000000 jsonschema_rs-0.9.1/jsonschema-lib/
+-rw-r--r--   0 runner    (1001) docker     (121)     1348 2021-06-17 11:37:54.000000 jsonschema_rs-0.9.1/jsonschema-lib/Cargo.toml
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-06-17 11:38:18.000000 jsonschema_rs-0.9.1/jsonschema-lib/benches/
+-rw-r--r--   0 runner    (1001) docker     (121)    18926 2021-06-17 11:37:54.000000 jsonschema_rs-0.9.1/jsonschema-lib/benches/jsonschema.rs
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-06-17 11:38:18.000000 jsonschema_rs-0.9.1/jsonschema-lib/meta_schemas/
+-rw-r--r--   0 runner    (1001) docker     (121)     4357 2021-06-17 11:37:54.000000 jsonschema_rs-0.9.1/jsonschema-lib/meta_schemas/draft4.json
+-rw-r--r--   0 runner    (1001) docker     (121)     4497 2021-06-17 11:37:54.000000 jsonschema_rs-0.9.1/jsonschema-lib/meta_schemas/draft6.json
+-rw-r--r--   0 runner    (1001) docker     (121)     4979 2021-06-17 11:37:54.000000 jsonschema_rs-0.9.1/jsonschema-lib/meta_schemas/draft7.json
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-06-17 11:38:18.000000 jsonschema_rs-0.9.1/jsonschema-lib/src/
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-06-17 11:38:18.000000 jsonschema_rs-0.9.1/jsonschema-lib/src/compilation/
+-rw-r--r--   0 runner    (1001) docker     (121)     1944 2021-06-17 11:37:54.000000 jsonschema_rs-0.9.1/jsonschema-lib/src/compilation/context.rs
+-rw-r--r--   0 runner    (1001) docker     (121)     7115 2021-06-17 11:37:54.000000 jsonschema_rs-0.9.1/jsonschema-lib/src/compilation/mod.rs
+-rw-r--r--   0 runner    (1001) docker     (121)    13691 2021-06-17 11:37:54.000000 jsonschema_rs-0.9.1/jsonschema-lib/src/compilation/options.rs
+-rw-r--r--   0 runner    (1001) docker     (121)      981 2021-06-17 11:37:54.000000 jsonschema_rs-0.9.1/jsonschema-lib/src/content_encoding.rs
+-rw-r--r--   0 runner    (1001) docker     (121)      539 2021-06-17 11:37:54.000000 jsonschema_rs-0.9.1/jsonschema-lib/src/content_media_type.rs
+-rw-r--r--   0 runner    (1001) docker     (121)    37022 2021-06-17 11:37:54.000000 jsonschema_rs-0.9.1/jsonschema-lib/src/error.rs
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-06-17 11:38:18.000000 jsonschema_rs-0.9.1/jsonschema-lib/src/keywords/
+-rw-r--r--   0 runner    (1001) docker     (121)     4461 2021-06-17 11:37:54.000000 jsonschema_rs-0.9.1/jsonschema-lib/src/keywords/additional_items.rs
+-rw-r--r--   0 runner    (1001) docker     (121)    50864 2021-06-17 11:37:54.000000 jsonschema_rs-0.9.1/jsonschema-lib/src/keywords/additional_properties.rs
+-rw-r--r--   0 runner    (1001) docker     (121)     3417 2021-06-17 11:37:54.000000 jsonschema_rs-0.9.1/jsonschema-lib/src/keywords/all_of.rs
+-rw-r--r--   0 runner    (1001) docker     (121)     1983 2021-06-17 11:37:54.000000 jsonschema_rs-0.9.1/jsonschema-lib/src/keywords/any_of.rs
+-rw-r--r--   0 runner    (1001) docker     (121)      886 2021-06-17 11:37:54.000000 jsonschema_rs-0.9.1/jsonschema-lib/src/keywords/boolean.rs
+-rw-r--r--   0 runner    (1001) docker     (121)     7898 2021-06-17 11:37:54.000000 jsonschema_rs-0.9.1/jsonschema-lib/src/keywords/const_.rs
+-rw-r--r--   0 runner    (1001) docker     (121)     2108 2021-06-17 11:37:54.000000 jsonschema_rs-0.9.1/jsonschema-lib/src/keywords/contains.rs
+-rw-r--r--   0 runner    (1001) docker     (121)     7882 2021-06-17 11:37:54.000000 jsonschema_rs-0.9.1/jsonschema-lib/src/keywords/content.rs
+-rw-r--r--   0 runner    (1001) docker     (121)     3037 2021-06-17 11:37:54.000000 jsonschema_rs-0.9.1/jsonschema-lib/src/keywords/dependencies.rs
+-rw-r--r--   0 runner    (1001) docker     (121)     3741 2021-06-17 11:37:54.000000 jsonschema_rs-0.9.1/jsonschema-lib/src/keywords/enum_.rs
+-rw-r--r--   0 runner    (1001) docker     (121)     4399 2021-06-17 11:37:54.000000 jsonschema_rs-0.9.1/jsonschema-lib/src/keywords/exclusive_maximum.rs
+-rw-r--r--   0 runner    (1001) docker     (121)     4365 2021-06-17 11:37:54.000000 jsonschema_rs-0.9.1/jsonschema-lib/src/keywords/exclusive_minimum.rs
+-rw-r--r--   0 runner    (1001) docker     (121)    13246 2021-06-17 11:37:54.000000 jsonschema_rs-0.9.1/jsonschema-lib/src/keywords/format.rs
+-rw-r--r--   0 runner    (1001) docker     (121)     2347 2021-06-17 11:37:54.000000 jsonschema_rs-0.9.1/jsonschema-lib/src/keywords/helpers.rs
+-rw-r--r--   0 runner    (1001) docker     (121)     6702 2021-06-17 11:37:54.000000 jsonschema_rs-0.9.1/jsonschema-lib/src/keywords/if_.rs
+-rw-r--r--   0 runner    (1001) docker     (121)     4278 2021-06-17 11:37:54.000000 jsonschema_rs-0.9.1/jsonschema-lib/src/keywords/items.rs
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-06-17 11:38:18.000000 jsonschema_rs-0.9.1/jsonschema-lib/src/keywords/legacy/
+-rw-r--r--   0 runner    (1001) docker     (121)      510 2021-06-17 11:37:54.000000 jsonschema_rs-0.9.1/jsonschema-lib/src/keywords/legacy/maximum_draft_4.rs
+-rw-r--r--   0 runner    (1001) docker     (121)      510 2021-06-17 11:37:54.000000 jsonschema_rs-0.9.1/jsonschema-lib/src/keywords/legacy/minimum_draft_4.rs
+-rw-r--r--   0 runner    (1001) docker     (121)       93 2021-06-17 11:37:54.000000 jsonschema_rs-0.9.1/jsonschema-lib/src/keywords/legacy/mod.rs
+-rw-r--r--   0 runner    (1001) docker     (121)     5139 2021-06-17 11:37:54.000000 jsonschema_rs-0.9.1/jsonschema-lib/src/keywords/legacy/type_draft_4.rs
+-rw-r--r--   0 runner    (1001) docker     (121)     1700 2021-06-17 11:37:54.000000 jsonschema_rs-0.9.1/jsonschema-lib/src/keywords/max_items.rs
+-rw-r--r--   0 runner    (1001) docker     (121)     1732 2021-06-17 11:37:54.000000 jsonschema_rs-0.9.1/jsonschema-lib/src/keywords/max_length.rs
+-rw-r--r--   0 runner    (1001) docker     (121)     1738 2021-06-17 11:37:54.000000 jsonschema_rs-0.9.1/jsonschema-lib/src/keywords/max_properties.rs
+-rw-r--r--   0 runner    (1001) docker     (121)     4082 2021-06-17 11:37:54.000000 jsonschema_rs-0.9.1/jsonschema-lib/src/keywords/maximum.rs
+-rw-r--r--   0 runner    (1001) docker     (121)     1700 2021-06-17 11:37:54.000000 jsonschema_rs-0.9.1/jsonschema-lib/src/keywords/min_items.rs
+-rw-r--r--   0 runner    (1001) docker     (121)     1726 2021-06-17 11:37:54.000000 jsonschema_rs-0.9.1/jsonschema-lib/src/keywords/min_length.rs
+-rw-r--r--   0 runner    (1001) docker     (121)     1738 2021-06-17 11:37:54.000000 jsonschema_rs-0.9.1/jsonschema-lib/src/keywords/min_properties.rs
+-rw-r--r--   0 runner    (1001) docker     (121)     4082 2021-06-17 11:37:54.000000 jsonschema_rs-0.9.1/jsonschema-lib/src/keywords/minimum.rs
+-rw-r--r--   0 runner    (1001) docker     (121)    17626 2021-06-17 11:37:54.000000 jsonschema_rs-0.9.1/jsonschema-lib/src/keywords/mod.rs
+-rw-r--r--   0 runner    (1001) docker     (121)     3864 2021-06-17 11:37:54.000000 jsonschema_rs-0.9.1/jsonschema-lib/src/keywords/multiple_of.rs
+-rw-r--r--   0 runner    (1001) docker     (121)     1723 2021-06-17 11:37:54.000000 jsonschema_rs-0.9.1/jsonschema-lib/src/keywords/not.rs
+-rw-r--r--   0 runner    (1001) docker     (121)     3368 2021-06-17 11:37:54.000000 jsonschema_rs-0.9.1/jsonschema-lib/src/keywords/one_of.rs
+-rw-r--r--   0 runner    (1001) docker     (121)     6030 2021-06-17 11:37:54.000000 jsonschema_rs-0.9.1/jsonschema-lib/src/keywords/pattern.rs
+-rw-r--r--   0 runner    (1001) docker     (121)     5892 2021-06-17 11:37:54.000000 jsonschema_rs-0.9.1/jsonschema-lib/src/keywords/pattern_properties.rs
+-rw-r--r--   0 runner    (1001) docker     (121)     3040 2021-06-17 11:37:54.000000 jsonschema_rs-0.9.1/jsonschema-lib/src/keywords/properties.rs
+-rw-r--r--   0 runner    (1001) docker     (121)     3926 2021-06-17 11:37:54.000000 jsonschema_rs-0.9.1/jsonschema-lib/src/keywords/property_names.rs
+-rw-r--r--   0 runner    (1001) docker     (121)     3919 2021-06-17 11:37:54.000000 jsonschema_rs-0.9.1/jsonschema-lib/src/keywords/ref_.rs
+-rw-r--r--   0 runner    (1001) docker     (121)     3987 2021-06-17 11:37:54.000000 jsonschema_rs-0.9.1/jsonschema-lib/src/keywords/required.rs
+-rw-r--r--   0 runner    (1001) docker     (121)    10471 2021-06-17 11:37:54.000000 jsonschema_rs-0.9.1/jsonschema-lib/src/keywords/type_.rs
+-rw-r--r--   0 runner    (1001) docker     (121)     4496 2021-06-17 11:37:54.000000 jsonschema_rs-0.9.1/jsonschema-lib/src/keywords/unique_items.rs
+-rw-r--r--   0 runner    (1001) docker     (121)     5447 2021-06-17 11:37:54.000000 jsonschema_rs-0.9.1/jsonschema-lib/src/lib.rs
+-rw-r--r--   0 runner    (1001) docker     (121)     2108 2021-06-17 11:37:54.000000 jsonschema_rs-0.9.1/jsonschema-lib/src/main.rs
+-rw-r--r--   0 runner    (1001) docker     (121)     4391 2021-06-17 11:37:54.000000 jsonschema_rs-0.9.1/jsonschema-lib/src/paths.rs
+-rw-r--r--   0 runner    (1001) docker     (121)     5517 2021-06-17 11:37:54.000000 jsonschema_rs-0.9.1/jsonschema-lib/src/primitive_type.rs
+-rw-r--r--   0 runner    (1001) docker     (121)    16219 2021-06-17 11:37:54.000000 jsonschema_rs-0.9.1/jsonschema-lib/src/resolver.rs
+-rw-r--r--   0 runner    (1001) docker     (121)     5845 2021-06-17 11:37:54.000000 jsonschema_rs-0.9.1/jsonschema-lib/src/schemas.rs
+-rw-r--r--   0 runner    (1001) docker     (121)      745 2021-06-17 11:37:54.000000 jsonschema_rs-0.9.1/jsonschema-lib/src/validator.rs
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-06-17 11:38:18.000000 jsonschema_rs-0.9.1/jsonschema_rs.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (121)    11029 2021-06-17 11:38:18.000000 jsonschema_rs-0.9.1/jsonschema_rs.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (121)     2621 2021-06-17 11:38:18.000000 jsonschema_rs-0.9.1/jsonschema_rs.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (121)        1 2021-06-17 11:38:18.000000 jsonschema_rs-0.9.1/jsonschema_rs.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (121)        1 2021-06-17 11:38:18.000000 jsonschema_rs-0.9.1/jsonschema_rs.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (121)        1 2021-06-17 11:38:18.000000 jsonschema_rs-0.9.1/jsonschema_rs.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (121)      340 2021-06-17 11:37:54.000000 jsonschema_rs-0.9.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (121)        7 2021-06-17 11:37:54.000000 jsonschema_rs-0.9.1/rust-toolchain
+-rw-r--r--   0 runner    (1001) docker     (121)       38 2021-06-17 11:38:18.000000 jsonschema_rs-0.9.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (121)     1910 2021-06-17 11:37:54.000000 jsonschema_rs-0.9.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-06-17 11:38:18.000000 jsonschema_rs-0.9.1/src/
+-rw-r--r--   0 runner    (1001) docker     (121)     8678 2021-06-17 11:37:54.000000 jsonschema_rs-0.9.1/src/lib.rs
+-rw-r--r--   0 runner    (1001) docker     (121)     6653 2021-06-17 11:37:54.000000 jsonschema_rs-0.9.1/src/ser.rs
+-rw-r--r--   0 runner    (1001) docker     (121)     1629 2021-06-17 11:37:54.000000 jsonschema_rs-0.9.1/src/string.rs
+-rw-r--r--   0 runner    (1001) docker     (121)     1284 2021-06-17 11:37:54.000000 jsonschema_rs-0.9.1/src/types.rs
```

### Comparing `jsonschema_rs-0.9.0/Cargo.toml` & `jsonschema_rs-0.9.1/Cargo.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [package]
 name = "jsonschema-python"
-version = "0.9.0"
+version = "0.9.1"
 authors = ["Dmitry Dygalo <dadygalo@gmail.com>"]
 edition = "2018"
 
 # See more keys and their definitions at https://doc.rust-lang.org/cargo/reference/manifest.html
 [lib]
 name = "jsonschema_rs"
 crate-type = ["cdylib"]
```

### Comparing `jsonschema_rs-0.9.0/PKG-INFO` & `jsonschema_rs-0.9.1/jsonschema_rs.egg-info/PKG-INFO`

 * *Files 19% similar despite different names*

```diff
@@ -1,184 +1,17 @@
 Metadata-Version: 2.1
-Name: jsonschema_rs
-Version: 0.9.0
+Name: jsonschema-rs
+Version: 0.9.1
 Summary: Fast JSON Schema validation for Python implemented in Rust
 Home-page: https://github.com/Stranger6667/jsonschema-rs/tree/master/python
 Author: Dmitry Dygalo
 Author-email: dadygalo@gmail.com
 Maintainer: Dmitry Dygalo
 Maintainer-email: dadygalo@gmail.com
 License: MIT
-Description: jsonschema-rs
-        =============
-        
-        |Build| |Version| |Python versions| |License|
-        
-        Fast JSON Schema validation for Python implemented in Rust.
-        
-        Supported drafts:
-        
-        - Draft 7
-        - Draft 6
-        - Draft 4
-        
-        There are some notable restrictions at the moment:
-        
-        - The underlying crate doesn't support arbitrary precision integers yet, which may lead to ``SystemError`` when such value is used;
-        - ``multipleOf`` keyword validation may produce false-negative results on some input. See `#84 <https://github.com/Stranger6667/jsonschema-rs/issues/84>`_ for more details
-        
-        Installation
-        ------------
-        
-        To install ``jsonschema-rs`` via ``pip`` run the following command:
-        
-        .. code:: bash
-        
-            pip install jsonschema-rs
-        
-        Usage
-        -----
-        
-        To check if the input document is valid:
-        
-        .. code:: python
-        
-            import jsonschema_rs
-        
-            validator = jsonschema_rs.JSONSchema({"minimum": 42})
-            validator.is_valid(45)  # True
-        
-        or:
-        
-        .. code:: python
-        
-            import jsonschema_rs
-        
-            validator = jsonschema_rs.JSONSchema({"minimum": 42})
-            validator.validate(41)  # raises ValidationError
-        
-        **NOTE**. This library is in early development.
-        
-        Performance
-        -----------
-        
-        According to our benchmarks, ``jsonschema-rs`` is usually faster than existing alternatives in real-life scenarios.
-        
-        However, for small schemas & inputs it might be slower than ``fastjsonschema`` or ``jsonschema`` on PyPy.
-        
-        Input values and schemas
-        ~~~~~~~~~~~~~~~~~~~~~~~~
-        
-        - `Zuora <https://github.com/APIs-guru/openapi-directory/blob/master/APIs/zuora.com/2021-04-23/openapi.yaml>`_ OpenAPI schema (``zuora.json``). Validated against `OpenAPI 3.0 JSON Schema <https://github.com/OAI/OpenAPI-Specification/blob/main/schemas/v3.0/schema.json>`_ (``openapi.json``).
-        - `Kubernetes <https://raw.githubusercontent.com/APIs-guru/openapi-directory/master/APIs/kubernetes.io/v1.10.0/swagger.yaml>`_ Swagger schema (``kubernetes.json``). Validated against `Swagger JSON Schema <https://github.com/OAI/OpenAPI-Specification/blob/main/schemas/v2.0/schema.json>`_ (``swagger.json``).
-        - Canadian border in GeoJSON format (``canada.json``). Schema is taken from the `GeoJSON website <https://geojson.org/schema/FeatureCollection.json>`_ (``geojson.json``).
-        - Concert data catalog (``citm_catalog.json``). Schema is inferred via `infers-jsonschema <https://github.com/Stranger6667/infers-jsonschema>`_ & manually adjusted (``citm_catalog_schema.json``).
-        - ``Fast`` is taken from `fastjsonschema benchmarks <https://github.com/horejsek/python-fastjsonschema/blob/master/performance.py#L15>`_ (``fast_schema.json``, `f`ast_valid.json`` and ``fast_invalid.json``).
-        
-        +----------------+-------------+---------------+
-        | Case           | Schema size | Instance size |
-        +================+=============+===============+
-        | OpenAPI        | 18 KB       | 4.5 MB        |
-        +----------------+-------------+---------------+
-        | Swagger        | 25 KB       | 3.0 MB        |
-        +----------------+-------------+---------------+
-        | Canada         | 4.8 KB      | 2.1 MB        |
-        +----------------+-------------+---------------+
-        | CITM catalog   | 2.3 KB      | 501 KB        |
-        +----------------+-------------+---------------+
-        | Fast (valid)   | 595 B       | 55 B          |
-        +----------------+-------------+---------------+
-        | Fast (invalid) | 595 B       | 60 B          |
-        +----------------+-------------+---------------+
-        
-        Compiled validators (when the input schema is compiled once and reused later). ``jsonschema-rs`` comes in three variants in the tables below:
-        
-        - ``validate``. This method raises ``ValidationError`` on errors or returns ``None`` on their absence.
-        - ``is_valid``. A faster method that returns a boolean result whether the instance is valid.
-        - ``overhead``. Only transforms data to underlying Rust types and do not perform any validation. Shows the Python -> Rust data conversion cost.
-        
-        Ratios are given against the ``validate`` variant.
-        
-        Small schemas:
-        
-        +-------------------------+------------------------+-----------------------+----------------------------+----------------------------+
-        | library                 | ``true``               | ``{"minimum": 10}``   | ``Fast (valid)``           | ``Fast (invalid)``         |
-        +=========================+========================+=======================+============================+============================+
-        | jsonschema-rs[validate] |              200.82 ns |             203.10 ns |                    1.22 us |                    1.51 us |
-        +-------------------------+------------------------+-----------------------+----------------------------+----------------------------+
-        | jsonschema-rs[is_valid] |  187.60 ns (**x0.93**) | 185.24 ns (**x0.91**) |      850.25 ns (**x0.69**) |        1.18 us (**x0.78**) |
-        +-------------------------+------------------------+-----------------------+----------------------------+----------------------------+
-        | jsonschema-rs[overhead] |  180.83 ns (**x0.90**) | 181.68 ns (**x0.89**) |      638.40 ns (**x0.52**) |        1.06 us (**x0.70**) |
-        +-------------------------+------------------------+-----------------------+----------------------------+----------------------------+
-        | fastjsonschema[CPython] |   58.57 ns (**x0.29**) | 109.10 ns (**x0.53**) |        4.16 us (**x3.40**) |        4.75 us (**x3.14**) |
-        +-------------------------+------------------------+-----------------------+----------------------------+----------------------------+
-        | fastjsonschema[PyPy]    |   1.32 ns (**x0.006**) |  33.39 ns (**x0.16**) |        890 ns  (**x0.72**) |         875 ns (**x0.58**) |
-        +-------------------------+------------------------+-----------------------+----------------------------+----------------------------+
-        | jsonschema[CPython]     |  226.48 ns (**x1.12**) |   1.88 us (**x9.25**) |      56.58 us (**x46.37**) |      57.31 us (**x37.95**) |
-        +-------------------------+------------------------+-----------------------+----------------------------+----------------------------+
-        | jsonschema[PyPy]        |   41.18 ns (**x0.20**) | 224.94 ns (**x1.10**) |      23.40 us (**x19.18**) |      22.78 us (**x15.08**) |
-        +-------------------------+------------------------+-----------------------+----------------------------+----------------------------+
-        
-        Large schemas:
-        
-        +-------------------------+-------------------------+--------------------------+----------------------------+---------------------------+
-        | library                 | ``Zuora (OpenAPI)``     | ``Kubernetes (Swagger)`` | ``Canada (GeoJSON)``       | ``CITM catalog``          |
-        +=========================+=========================+==========================+============================+===========================+
-        | jsonschema-rs[validate] |               13.970 ms |                13.076 ms |                   4.428 ms |                  4.715 ms |
-        +-------------------------+-------------------------+--------------------------+----------------------------+---------------------------+
-        | jsonschema-rs[is_valid] |   13.664 ms (**x0.97**) |    11.506 ms (**x0.87**) |       4.422 ms (**x0.99**) |      3.134 ms (**x0.66**) |
-        +-------------------------+-------------------------+--------------------------+----------------------------+---------------------------+
-        | jsonschema-rs[overhead] |   12.206 ms (**x0.87**) |     8.116 ms (**x0.62**) |       3.666 ms (**x0.82**) |      2.648 ms (**x0.56**) |
-        +-------------------------+-------------------------+--------------------------+----------------------------+---------------------------+
-        | fastjsonschema[CPython] |                  -- (1) |    87.020 ms (**x6.65**) |      31.705 ms (**x7.16**) |     11.715 ms (**x2.48**) |
-        +-------------------------+-------------------------+--------------------------+----------------------------+---------------------------+
-        | fastjsonschema[PyPy]    |                  -- (1) |    38.586 ms (**x2.95**) |       8.417 ms (**x1.90**) |      4.789 ms (**x1.01**) |
-        +-------------------------+-------------------------+--------------------------+----------------------------+---------------------------+
-        | jsonschema[CPython]     | 749.615 ms (**x53.65**) |     1.032 s (**x78.92**) |      1.286 s (**x290.42**) |   112.510 ms (**x23.86**) |
-        +-------------------------+-------------------------+--------------------------+----------------------------+---------------------------+
-        | jsonschema[PyPy]        | 611.056 ms (**x43.74**) |  592.584 ms (**x45.31**) |   530.567 ms (**x119.82**) |     28.619 ms (**x6.06**) |
-        +-------------------------+-------------------------+--------------------------+----------------------------+---------------------------+
-        
-        Notes:
-        
-        1. ``fastjsonschema`` fails to compile the Open API spec due to the presence of the ``uri-reference`` format (that is not defined in Draft 4). However, unknown formats are `explicitly supported <https://tools.ietf.org/html/draft-fge-json-schema-validation-00#section-7.1>`_ by the spec.
-        
-        The bigger the input is the bigger is performance win. You can take a look at benchmarks in ``benches/bench.py``.
-        
-        Package versions:
-        
-        - ``jsonschema-rs`` - latest version from the repository
-        - ``jsonschema`` - ``3.2.0``
-        - ``fastjsonschema`` - ``2.15.0``
-        
-        Measured with stable Rust 1.51, CPython 3.9.4 / PyPy3 7.3.4 on i8700K (12 cores), 32GB RAM, Arch Linux.
-        
-        Python support
-        --------------
-        
-        ``jsonschema-rs`` supports CPython 3.6, 3.7, 3.8 and 3.9.
-        
-        License
-        -------
-        
-        The code in this project is licensed under `MIT license`_.
-        By contributing to ``jsonschema-rs``, you agree that your contributions
-        will be licensed under its MIT license.
-         
-        .. |Build| image:: https://github.com/Stranger6667/jsonschema-rs/workflows/ci/badge.svg
-           :target: https://github.com/Stranger6667/jsonschema-rs/actions
-        .. |Version| image:: https://img.shields.io/pypi/v/jsonschema-rs.svg
-           :target: https://pypi.org/project/jsonschema-rs/
-        .. |Python versions| image:: https://img.shields.io/pypi/pyversions/jsonschema-rs.svg
-           :target: https://pypi.org/project/jsonschema-rs/
-        .. |License| image:: https://img.shields.io/pypi/l/jsonschema-rs.svg
-           :target: https://opensource.org/licenses/MIT
-        
-        .. _MIT license: https://opensource.org/licenses/MIT
-        
 Keywords: jsonschema validation rust
 Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
@@ -186,7 +19,176 @@
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Programming Language :: Rust
 Requires-Python: >=3.6
 Description-Content-Type: text/x-rst
+
+jsonschema-rs
+=============
+
+|Build| |Version| |Python versions| |License|
+
+Fast JSON Schema validation for Python implemented in Rust.
+
+Supported drafts:
+
+- Draft 7
+- Draft 6
+- Draft 4
+
+There are some notable restrictions at the moment:
+
+- The underlying crate doesn't support arbitrary precision integers yet, which may lead to ``SystemError`` when such value is used;
+- ``multipleOf`` keyword validation may produce false-negative results on some input. See `#84 <https://github.com/Stranger6667/jsonschema-rs/issues/84>`_ for more details
+
+Installation
+------------
+
+To install ``jsonschema-rs`` via ``pip`` run the following command:
+
+.. code:: bash
+
+    pip install jsonschema-rs
+
+Usage
+-----
+
+To check if the input document is valid:
+
+.. code:: python
+
+    import jsonschema_rs
+
+    validator = jsonschema_rs.JSONSchema({"minimum": 42})
+    validator.is_valid(45)  # True
+
+or:
+
+.. code:: python
+
+    import jsonschema_rs
+
+    validator = jsonschema_rs.JSONSchema({"minimum": 42})
+    validator.validate(41)  # raises ValidationError
+
+**NOTE**. This library is in early development.
+
+Performance
+-----------
+
+According to our benchmarks, ``jsonschema-rs`` is usually faster than existing alternatives in real-life scenarios.
+
+However, for small schemas & inputs it might be slower than ``fastjsonschema`` or ``jsonschema`` on PyPy.
+
+Input values and schemas
+~~~~~~~~~~~~~~~~~~~~~~~~
+
+- `Zuora <https://github.com/APIs-guru/openapi-directory/blob/master/APIs/zuora.com/2021-04-23/openapi.yaml>`_ OpenAPI schema (``zuora.json``). Validated against `OpenAPI 3.0 JSON Schema <https://github.com/OAI/OpenAPI-Specification/blob/main/schemas/v3.0/schema.json>`_ (``openapi.json``).
+- `Kubernetes <https://raw.githubusercontent.com/APIs-guru/openapi-directory/master/APIs/kubernetes.io/v1.10.0/swagger.yaml>`_ Swagger schema (``kubernetes.json``). Validated against `Swagger JSON Schema <https://github.com/OAI/OpenAPI-Specification/blob/main/schemas/v2.0/schema.json>`_ (``swagger.json``).
+- Canadian border in GeoJSON format (``canada.json``). Schema is taken from the `GeoJSON website <https://geojson.org/schema/FeatureCollection.json>`_ (``geojson.json``).
+- Concert data catalog (``citm_catalog.json``). Schema is inferred via `infers-jsonschema <https://github.com/Stranger6667/infers-jsonschema>`_ & manually adjusted (``citm_catalog_schema.json``).
+- ``Fast`` is taken from `fastjsonschema benchmarks <https://github.com/horejsek/python-fastjsonschema/blob/master/performance.py#L15>`_ (``fast_schema.json``, `f`ast_valid.json`` and ``fast_invalid.json``).
+
++----------------+-------------+---------------+
+| Case           | Schema size | Instance size |
++================+=============+===============+
+| OpenAPI        | 18 KB       | 4.5 MB        |
++----------------+-------------+---------------+
+| Swagger        | 25 KB       | 3.0 MB        |
++----------------+-------------+---------------+
+| Canada         | 4.8 KB      | 2.1 MB        |
++----------------+-------------+---------------+
+| CITM catalog   | 2.3 KB      | 501 KB        |
++----------------+-------------+---------------+
+| Fast (valid)   | 595 B       | 55 B          |
++----------------+-------------+---------------+
+| Fast (invalid) | 595 B       | 60 B          |
++----------------+-------------+---------------+
+
+Compiled validators (when the input schema is compiled once and reused later). ``jsonschema-rs`` comes in three variants in the tables below:
+
+- ``validate``. This method raises ``ValidationError`` on errors or returns ``None`` on their absence.
+- ``is_valid``. A faster method that returns a boolean result whether the instance is valid.
+- ``overhead``. Only transforms data to underlying Rust types and do not perform any validation. Shows the Python -> Rust data conversion cost.
+
+Ratios are given against the ``validate`` variant.
+
+Small schemas:
+
++-------------------------+------------------------+-----------------------+----------------------------+----------------------------+
+| library                 | ``true``               | ``{"minimum": 10}``   | ``Fast (valid)``           | ``Fast (invalid)``         |
++=========================+========================+=======================+============================+============================+
+| jsonschema-rs[validate] |              200.82 ns |             203.10 ns |                    1.22 us |                    1.51 us |
++-------------------------+------------------------+-----------------------+----------------------------+----------------------------+
+| jsonschema-rs[is_valid] |  187.60 ns (**x0.93**) | 185.24 ns (**x0.91**) |      850.25 ns (**x0.69**) |        1.18 us (**x0.78**) |
++-------------------------+------------------------+-----------------------+----------------------------+----------------------------+
+| jsonschema-rs[overhead] |  180.83 ns (**x0.90**) | 181.68 ns (**x0.89**) |      638.40 ns (**x0.52**) |        1.06 us (**x0.70**) |
++-------------------------+------------------------+-----------------------+----------------------------+----------------------------+
+| fastjsonschema[CPython] |   58.57 ns (**x0.29**) | 109.10 ns (**x0.53**) |        4.16 us (**x3.40**) |        4.75 us (**x3.14**) |
++-------------------------+------------------------+-----------------------+----------------------------+----------------------------+
+| fastjsonschema[PyPy]    |   1.32 ns (**x0.006**) |  33.39 ns (**x0.16**) |        890 ns  (**x0.72**) |         875 ns (**x0.58**) |
++-------------------------+------------------------+-----------------------+----------------------------+----------------------------+
+| jsonschema[CPython]     |  226.48 ns (**x1.12**) |   1.88 us (**x9.25**) |      56.58 us (**x46.37**) |      57.31 us (**x37.95**) |
++-------------------------+------------------------+-----------------------+----------------------------+----------------------------+
+| jsonschema[PyPy]        |   41.18 ns (**x0.20**) | 224.94 ns (**x1.10**) |      23.40 us (**x19.18**) |      22.78 us (**x15.08**) |
++-------------------------+------------------------+-----------------------+----------------------------+----------------------------+
+
+Large schemas:
+
++-------------------------+-------------------------+--------------------------+----------------------------+---------------------------+
+| library                 | ``Zuora (OpenAPI)``     | ``Kubernetes (Swagger)`` | ``Canada (GeoJSON)``       | ``CITM catalog``          |
++=========================+=========================+==========================+============================+===========================+
+| jsonschema-rs[validate] |               13.970 ms |                13.076 ms |                   4.428 ms |                  4.715 ms |
++-------------------------+-------------------------+--------------------------+----------------------------+---------------------------+
+| jsonschema-rs[is_valid] |   13.664 ms (**x0.97**) |    11.506 ms (**x0.87**) |       4.422 ms (**x0.99**) |      3.134 ms (**x0.66**) |
++-------------------------+-------------------------+--------------------------+----------------------------+---------------------------+
+| jsonschema-rs[overhead] |   12.206 ms (**x0.87**) |     8.116 ms (**x0.62**) |       3.666 ms (**x0.82**) |      2.648 ms (**x0.56**) |
++-------------------------+-------------------------+--------------------------+----------------------------+---------------------------+
+| fastjsonschema[CPython] |                  -- (1) |    87.020 ms (**x6.65**) |      31.705 ms (**x7.16**) |     11.715 ms (**x2.48**) |
++-------------------------+-------------------------+--------------------------+----------------------------+---------------------------+
+| fastjsonschema[PyPy]    |                  -- (1) |    38.586 ms (**x2.95**) |       8.417 ms (**x1.90**) |      4.789 ms (**x1.01**) |
++-------------------------+-------------------------+--------------------------+----------------------------+---------------------------+
+| jsonschema[CPython]     | 749.615 ms (**x53.65**) |     1.032 s (**x78.92**) |      1.286 s (**x290.42**) |   112.510 ms (**x23.86**) |
++-------------------------+-------------------------+--------------------------+----------------------------+---------------------------+
+| jsonschema[PyPy]        | 611.056 ms (**x43.74**) |  592.584 ms (**x45.31**) |   530.567 ms (**x119.82**) |     28.619 ms (**x6.06**) |
++-------------------------+-------------------------+--------------------------+----------------------------+---------------------------+
+
+Notes:
+
+1. ``fastjsonschema`` fails to compile the Open API spec due to the presence of the ``uri-reference`` format (that is not defined in Draft 4). However, unknown formats are `explicitly supported <https://tools.ietf.org/html/draft-fge-json-schema-validation-00#section-7.1>`_ by the spec.
+
+The bigger the input is the bigger is performance win. You can take a look at benchmarks in ``benches/bench.py``.
+
+Package versions:
+
+- ``jsonschema-rs`` - latest version from the repository
+- ``jsonschema`` - ``3.2.0``
+- ``fastjsonschema`` - ``2.15.0``
+
+Measured with stable Rust 1.51, CPython 3.9.4 / PyPy3 7.3.4 on i8700K (12 cores), 32GB RAM, Arch Linux.
+
+Python support
+--------------
+
+``jsonschema-rs`` supports CPython 3.6, 3.7, 3.8 and 3.9.
+
+License
+-------
+
+The code in this project is licensed under `MIT license`_.
+By contributing to ``jsonschema-rs``, you agree that your contributions
+will be licensed under its MIT license.
+ 
+.. |Build| image:: https://github.com/Stranger6667/jsonschema-rs/workflows/ci/badge.svg
+   :target: https://github.com/Stranger6667/jsonschema-rs/actions
+.. |Version| image:: https://img.shields.io/pypi/v/jsonschema-rs.svg
+   :target: https://pypi.org/project/jsonschema-rs/
+.. |Python versions| image:: https://img.shields.io/pypi/pyversions/jsonschema-rs.svg
+   :target: https://pypi.org/project/jsonschema-rs/
+.. |License| image:: https://img.shields.io/pypi/l/jsonschema-rs.svg
+   :target: https://opensource.org/licenses/MIT
+
+.. _MIT license: https://opensource.org/licenses/MIT
+
+
```

### Comparing `jsonschema_rs-0.9.0/README.rst` & `jsonschema_rs-0.9.1/README.rst`

 * *Files identical despite different names*

### Comparing `jsonschema_rs-0.9.0/jsonschema-lib/Cargo.toml` & `jsonschema_rs-0.9.1/jsonschema-lib/Cargo.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [package]
 name = "jsonschema"
-version = "0.9.0"
+version = "0.9.1"
 authors = ["dmitry.dygalo <dadygalo@gmail.com>"]
 edition = "2018"
 license = "MIT"
 readme = "../README.md"
 description = "A crate for performing JSON schema validation"
 repository = "https://github.com/Stranger6667/jsonschema-rs"
 keywords = ["jsonschema", "validation"]
@@ -20,15 +20,15 @@
 
 [dependencies]
 serde_json = "1"
 url = "2"
 lazy_static = "1"
 percent-encoding = "2"
 regex = "1"
-fancy-regex = "0.5"
+fancy-regex = "0.6"
 base64 = ">= 0.2"
 chrono = ">= 0.2"
 reqwest = { version = ">= 0.10", features = ["blocking", "json"], optional = true}
 parking_lot = ">= 0.1"
 num-cmp = ">= 0.1"
 ahash = "0.7"
 structopt = { version = ">= 0.3", optional = true }
```

### Comparing `jsonschema_rs-0.9.0/jsonschema-lib/benches/jsonschema.rs` & `jsonschema_rs-0.9.1/jsonschema-lib/benches/jsonschema.rs`

 * *Files identical despite different names*

### Comparing `jsonschema_rs-0.9.0/jsonschema-lib/meta_schemas/draft4.json` & `jsonschema_rs-0.9.1/jsonschema-lib/meta_schemas/draft4.json`

 * *Files identical despite different names*

### Comparing `jsonschema_rs-0.9.0/jsonschema-lib/meta_schemas/draft6.json` & `jsonschema_rs-0.9.1/jsonschema-lib/meta_schemas/draft6.json`

 * *Files identical despite different names*

### Comparing `jsonschema_rs-0.9.0/jsonschema-lib/meta_schemas/draft7.json` & `jsonschema_rs-0.9.1/jsonschema-lib/meta_schemas/draft7.json`

 * *Files identical despite different names*

### Comparing `jsonschema_rs-0.9.0/jsonschema-lib/src/compilation/context.rs` & `jsonschema_rs-0.9.1/jsonschema-lib/src/compilation/context.rs`

 * *Files identical despite different names*

### Comparing `jsonschema_rs-0.9.0/jsonschema-lib/src/compilation/mod.rs` & `jsonschema_rs-0.9.1/jsonschema-lib/src/compilation/mod.rs`

 * *Files identical despite different names*

### Comparing `jsonschema_rs-0.9.0/jsonschema-lib/src/compilation/options.rs` & `jsonschema_rs-0.9.1/jsonschema-lib/src/compilation/options.rs`

 * *Files identical despite different names*

### Comparing `jsonschema_rs-0.9.0/jsonschema-lib/src/content_encoding.rs` & `jsonschema_rs-0.9.1/jsonschema-lib/src/content_encoding.rs`

 * *Files identical despite different names*

### Comparing `jsonschema_rs-0.9.0/jsonschema-lib/src/content_media_type.rs` & `jsonschema_rs-0.9.1/jsonschema-lib/src/content_media_type.rs`

 * *Files identical despite different names*

### Comparing `jsonschema_rs-0.9.0/jsonschema-lib/src/error.rs` & `jsonschema_rs-0.9.1/jsonschema-lib/src/error.rs`

 * *Files identical despite different names*

### Comparing `jsonschema_rs-0.9.0/jsonschema-lib/src/keywords/additional_items.rs` & `jsonschema_rs-0.9.1/jsonschema-lib/src/keywords/additional_items.rs`

 * *Files identical despite different names*

### Comparing `jsonschema_rs-0.9.0/jsonschema-lib/src/keywords/additional_properties.rs` & `jsonschema_rs-0.9.1/jsonschema-lib/src/keywords/additional_properties.rs`

 * *Files identical despite different names*

### Comparing `jsonschema_rs-0.9.0/jsonschema-lib/src/keywords/all_of.rs` & `jsonschema_rs-0.9.1/jsonschema-lib/src/keywords/all_of.rs`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,11 @@
-use crate::keywords::format_validators;
 use crate::{
     compilation::{compile_validators, context::CompilationContext, JSONSchema},
     error::{CompilationError, ErrorIterator},
-    keywords::{format_vec_of_validators, CompilationResult, Validators},
+    keywords::{format_validators, format_vec_of_validators, CompilationResult, Validators},
     paths::InstancePath,
     validator::Validate,
 };
 use serde_json::{Map, Value};
 
 pub(crate) struct AllOfValidator {
     schemas: Vec<Validators>,
```

### Comparing `jsonschema_rs-0.9.0/jsonschema-lib/src/keywords/any_of.rs` & `jsonschema_rs-0.9.1/jsonschema-lib/src/keywords/any_of.rs`

 * *Files identical despite different names*

### Comparing `jsonschema_rs-0.9.0/jsonschema-lib/src/keywords/boolean.rs` & `jsonschema_rs-0.9.1/jsonschema-lib/src/keywords/boolean.rs`

 * *Files identical despite different names*

### Comparing `jsonschema_rs-0.9.0/jsonschema-lib/src/keywords/const_.rs` & `jsonschema_rs-0.9.1/jsonschema-lib/src/keywords/const_.rs`

 * *Files identical despite different names*

### Comparing `jsonschema_rs-0.9.0/jsonschema-lib/src/keywords/contains.rs` & `jsonschema_rs-0.9.1/jsonschema-lib/src/keywords/contains.rs`

 * *Files identical despite different names*

### Comparing `jsonschema_rs-0.9.0/jsonschema-lib/src/keywords/content.rs` & `jsonschema_rs-0.9.1/jsonschema-lib/src/keywords/content.rs`

 * *Files identical despite different names*

### Comparing `jsonschema_rs-0.9.0/jsonschema-lib/src/keywords/dependencies.rs` & `jsonschema_rs-0.9.1/jsonschema-lib/src/keywords/dependencies.rs`

 * *Files identical despite different names*

### Comparing `jsonschema_rs-0.9.0/jsonschema-lib/src/keywords/enum_.rs` & `jsonschema_rs-0.9.1/jsonschema-lib/src/keywords/enum_.rs`

 * *Files identical despite different names*

### Comparing `jsonschema_rs-0.9.0/jsonschema-lib/src/keywords/exclusive_maximum.rs` & `jsonschema_rs-0.9.1/jsonschema-lib/src/keywords/exclusive_maximum.rs`

 * *Files identical despite different names*

### Comparing `jsonschema_rs-0.9.0/jsonschema-lib/src/keywords/exclusive_minimum.rs` & `jsonschema_rs-0.9.1/jsonschema-lib/src/keywords/exclusive_minimum.rs`

 * *Files identical despite different names*

### Comparing `jsonschema_rs-0.9.0/jsonschema-lib/src/keywords/format.rs` & `jsonschema_rs-0.9.1/jsonschema-lib/src/keywords/format.rs`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 //! Validator for `format` keyword.
 use crate::{
     compilation::{context::CompilationContext, JSONSchema},
     error::{error, no_error, CompilationError, ErrorIterator, ValidationError},
-    keywords::CompilationResult,
+    keywords::{pattern, CompilationResult},
     paths::InstancePath,
     validator::Validate,
     Draft,
 };
 use chrono::{DateTime, NaiveDate};
 use fancy_regex::Regex;
 use serde_json::{Map, Value};
@@ -263,15 +263,15 @@
     }
 }
 format_validator!(RegexValidator, "regex");
 impl Validate for RegexValidator {
     validate!("regex");
     fn is_valid(&self, _: &JSONSchema, instance: &Value) -> bool {
         if let Value::String(item) = instance {
-            Regex::new(item).is_ok()
+            pattern::convert_regex(item).is_ok()
         } else {
             true
         }
     }
 }
 format_validator!(RelativeJSONPointerValidator, "relative-json-pointer");
 impl Validate for RelativeJSONPointerValidator {
@@ -377,8 +377,17 @@
     #[test]
     fn ignored_format() {
         let schema = json!({"format": "custom", "type": "string"});
         let instance = json!("foo");
         let compiled = JSONSchema::compile(&schema).unwrap();
         assert!(compiled.is_valid(&instance))
     }
+
+    #[test]
+    fn ecma_regex() {
+        // See GH-230
+        let schema = json!({"format": "regex", "type": "string"});
+        let instance = json!("^\\cc$");
+        let compiled = JSONSchema::compile(&schema).unwrap();
+        assert!(compiled.is_valid(&instance))
+    }
 }
```

### Comparing `jsonschema_rs-0.9.0/jsonschema-lib/src/keywords/helpers.rs` & `jsonschema_rs-0.9.1/jsonschema-lib/src/keywords/helpers.rs`

 * *Files identical despite different names*

### Comparing `jsonschema_rs-0.9.0/jsonschema-lib/src/keywords/if_.rs` & `jsonschema_rs-0.9.1/jsonschema-lib/src/keywords/if_.rs`

 * *Files identical despite different names*

### Comparing `jsonschema_rs-0.9.0/jsonschema-lib/src/keywords/items.rs` & `jsonschema_rs-0.9.1/jsonschema-lib/src/keywords/items.rs`

 * *Files identical despite different names*

### Comparing `jsonschema_rs-0.9.0/jsonschema-lib/src/keywords/legacy/type_draft_4.rs` & `jsonschema_rs-0.9.1/jsonschema-lib/src/keywords/legacy/type_draft_4.rs`

 * *Files identical despite different names*

### Comparing `jsonschema_rs-0.9.0/jsonschema-lib/src/keywords/max_items.rs` & `jsonschema_rs-0.9.1/jsonschema-lib/src/keywords/max_items.rs`

 * *Files identical despite different names*

### Comparing `jsonschema_rs-0.9.0/jsonschema-lib/src/keywords/max_length.rs` & `jsonschema_rs-0.9.1/jsonschema-lib/src/keywords/max_length.rs`

 * *Files identical despite different names*

### Comparing `jsonschema_rs-0.9.0/jsonschema-lib/src/keywords/max_properties.rs` & `jsonschema_rs-0.9.1/jsonschema-lib/src/keywords/max_properties.rs`

 * *Files identical despite different names*

### Comparing `jsonschema_rs-0.9.0/jsonschema-lib/src/keywords/maximum.rs` & `jsonschema_rs-0.9.1/jsonschema-lib/src/keywords/maximum.rs`

 * *Files identical despite different names*

### Comparing `jsonschema_rs-0.9.0/jsonschema-lib/src/keywords/min_items.rs` & `jsonschema_rs-0.9.1/jsonschema-lib/src/keywords/min_items.rs`

 * *Files identical despite different names*

### Comparing `jsonschema_rs-0.9.0/jsonschema-lib/src/keywords/min_length.rs` & `jsonschema_rs-0.9.1/jsonschema-lib/src/keywords/min_length.rs`

 * *Files identical despite different names*

### Comparing `jsonschema_rs-0.9.0/jsonschema-lib/src/keywords/min_properties.rs` & `jsonschema_rs-0.9.1/jsonschema-lib/src/keywords/min_properties.rs`

 * *Files identical despite different names*

### Comparing `jsonschema_rs-0.9.0/jsonschema-lib/src/keywords/minimum.rs` & `jsonschema_rs-0.9.1/jsonschema-lib/src/keywords/minimum.rs`

 * *Files identical despite different names*

### Comparing `jsonschema_rs-0.9.0/jsonschema-lib/src/keywords/mod.rs` & `jsonschema_rs-0.9.1/jsonschema-lib/src/keywords/mod.rs`

 * *Files identical despite different names*

### Comparing `jsonschema_rs-0.9.0/jsonschema-lib/src/keywords/multiple_of.rs` & `jsonschema_rs-0.9.1/jsonschema-lib/src/keywords/multiple_of.rs`

 * *Files identical despite different names*

### Comparing `jsonschema_rs-0.9.0/jsonschema-lib/src/keywords/not.rs` & `jsonschema_rs-0.9.1/jsonschema-lib/src/keywords/not.rs`

 * *Files identical despite different names*

### Comparing `jsonschema_rs-0.9.0/jsonschema-lib/src/keywords/one_of.rs` & `jsonschema_rs-0.9.1/jsonschema-lib/src/keywords/one_of.rs`

 * *Files identical despite different names*

### Comparing `jsonschema_rs-0.9.0/jsonschema-lib/src/keywords/pattern.rs` & `jsonschema_rs-0.9.1/jsonschema-lib/src/keywords/pattern.rs`

 * *Files 2% similar despite different names*

```diff
@@ -71,20 +71,20 @@
         }
         true
     }
 }
 
 impl ToString for PatternValidator {
     fn to_string(&self) -> String {
-        format!("pattern: {:?}", self.pattern)
+        format!("pattern: {}", self.pattern)
     }
 }
 
 // ECMA 262 has differences
-fn convert_regex(pattern: &str) -> Result<fancy_regex::Regex, fancy_regex::Error> {
+pub(crate) fn convert_regex(pattern: &str) -> Result<fancy_regex::Regex, fancy_regex::Error> {
     // replace control chars
     let new_pattern = CONTROL_GROUPS_RE.replace_all(pattern, replace_control_group);
     let mut out = String::with_capacity(new_pattern.len());
     let mut chars = new_pattern.chars().peekable();
     // To convert character group we need to iterate over chars and in case of `\` take a look
     // at the next char to detect whether this group should be converted
     while let Some(current) = chars.next() {
```

### Comparing `jsonschema_rs-0.9.0/jsonschema-lib/src/keywords/pattern_properties.rs` & `jsonschema_rs-0.9.1/jsonschema-lib/src/keywords/pattern_properties.rs`

 * *Files 1% similar despite different names*

```diff
@@ -76,17 +76,15 @@
 
 impl ToString for PatternPropertiesValidator {
     fn to_string(&self) -> String {
         format!(
             "patternProperties: {{{}}}",
             self.patterns
                 .iter()
-                .map(|(key, validators)| {
-                    format!("{:?}: {}", key, format_validators(validators))
-                })
+                .map(|(key, validators)| { format!("{}: {}", key, format_validators(validators)) })
                 .collect::<Vec<String>>()
                 .join(", ")
         )
     }
 }
 
 pub(crate) struct SingleValuePatternPropertiesValidator {
@@ -146,15 +144,15 @@
         }
     }
 }
 
 impl ToString for SingleValuePatternPropertiesValidator {
     fn to_string(&self) -> String {
         format!(
-            "patternProperties: {{{:?}: {}}}",
+            "patternProperties: {{{}: {}}}",
             self.pattern,
             format_validators(&self.validators)
         )
     }
 }
 
 #[inline]
```

### Comparing `jsonschema_rs-0.9.0/jsonschema-lib/src/keywords/properties.rs` & `jsonschema_rs-0.9.1/jsonschema-lib/src/keywords/properties.rs`

 * *Files identical despite different names*

### Comparing `jsonschema_rs-0.9.0/jsonschema-lib/src/keywords/property_names.rs` & `jsonschema_rs-0.9.1/jsonschema-lib/src/keywords/property_names.rs`

 * *Files identical despite different names*

### Comparing `jsonschema_rs-0.9.0/jsonschema-lib/src/keywords/ref_.rs` & `jsonschema_rs-0.9.1/jsonschema-lib/src/keywords/ref_.rs`

 * *Files identical despite different names*

### Comparing `jsonschema_rs-0.9.0/jsonschema-lib/src/keywords/required.rs` & `jsonschema_rs-0.9.1/jsonschema-lib/src/keywords/required.rs`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,10 @@
-use crate::error::error;
 use crate::{
     compilation::{context::CompilationContext, JSONSchema},
-    error::{no_error, CompilationError, ErrorIterator, ValidationError},
+    error::{error, no_error, CompilationError, ErrorIterator, ValidationError},
     keywords::CompilationResult,
     paths::InstancePath,
     validator::Validate,
 };
 use serde_json::{Map, Value};
 
 pub(crate) struct RequiredValidator {
```

### Comparing `jsonschema_rs-0.9.0/jsonschema-lib/src/keywords/type_.rs` & `jsonschema_rs-0.9.1/jsonschema-lib/src/keywords/type_.rs`

 * *Files identical despite different names*

### Comparing `jsonschema_rs-0.9.0/jsonschema-lib/src/keywords/unique_items.rs` & `jsonschema_rs-0.9.1/jsonschema-lib/src/keywords/unique_items.rs`

 * *Files identical despite different names*

### Comparing `jsonschema_rs-0.9.0/jsonschema-lib/src/lib.rs` & `jsonschema_rs-0.9.1/jsonschema-lib/src/lib.rs`

 * *Files identical despite different names*

### Comparing `jsonschema_rs-0.9.0/jsonschema-lib/src/main.rs` & `jsonschema_rs-0.9.1/jsonschema-lib/src/main.rs`

 * *Files identical despite different names*

### Comparing `jsonschema_rs-0.9.0/jsonschema-lib/src/paths.rs` & `jsonschema_rs-0.9.1/jsonschema-lib/src/paths.rs`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,9 @@
 //! Facilities for working with paths within schemas or validated instances.
-use std::slice::Iter;
-use std::{fmt, fmt::Write};
+use std::{fmt, fmt::Write, slice::Iter};
 
 #[derive(Clone, Debug, Eq, PartialEq)]
 /// JSON Pointer as a wrapper around individual path components.
 pub struct JSONPointer(Vec<PathChunk>);
 
 impl JSONPointer {
     #[must_use]
```

### Comparing `jsonschema_rs-0.9.0/jsonschema-lib/src/primitive_type.rs` & `jsonschema_rs-0.9.1/jsonschema-lib/src/primitive_type.rs`

 * *Files identical despite different names*

### Comparing `jsonschema_rs-0.9.0/jsonschema-lib/src/resolver.rs` & `jsonschema_rs-0.9.1/jsonschema-lib/src/resolver.rs`

 * *Files identical despite different names*

### Comparing `jsonschema_rs-0.9.0/jsonschema-lib/src/schemas.rs` & `jsonschema_rs-0.9.1/jsonschema-lib/src/schemas.rs`

 * *Files identical despite different names*

### Comparing `jsonschema_rs-0.9.0/jsonschema-lib/src/validator.rs` & `jsonschema_rs-0.9.1/jsonschema-lib/src/validator.rs`

 * *Files identical despite different names*

### Comparing `jsonschema_rs-0.9.0/jsonschema_rs.egg-info/PKG-INFO` & `jsonschema_rs-0.9.1/PKG-INFO`

 * *Files 19% similar despite different names*

```diff
@@ -1,184 +1,17 @@
 Metadata-Version: 2.1
-Name: jsonschema-rs
-Version: 0.9.0
+Name: jsonschema_rs
+Version: 0.9.1
 Summary: Fast JSON Schema validation for Python implemented in Rust
 Home-page: https://github.com/Stranger6667/jsonschema-rs/tree/master/python
 Author: Dmitry Dygalo
 Author-email: dadygalo@gmail.com
 Maintainer: Dmitry Dygalo
 Maintainer-email: dadygalo@gmail.com
 License: MIT
-Description: jsonschema-rs
-        =============
-        
-        |Build| |Version| |Python versions| |License|
-        
-        Fast JSON Schema validation for Python implemented in Rust.
-        
-        Supported drafts:
-        
-        - Draft 7
-        - Draft 6
-        - Draft 4
-        
-        There are some notable restrictions at the moment:
-        
-        - The underlying crate doesn't support arbitrary precision integers yet, which may lead to ``SystemError`` when such value is used;
-        - ``multipleOf`` keyword validation may produce false-negative results on some input. See `#84 <https://github.com/Stranger6667/jsonschema-rs/issues/84>`_ for more details
-        
-        Installation
-        ------------
-        
-        To install ``jsonschema-rs`` via ``pip`` run the following command:
-        
-        .. code:: bash
-        
-            pip install jsonschema-rs
-        
-        Usage
-        -----
-        
-        To check if the input document is valid:
-        
-        .. code:: python
-        
-            import jsonschema_rs
-        
-            validator = jsonschema_rs.JSONSchema({"minimum": 42})
-            validator.is_valid(45)  # True
-        
-        or:
-        
-        .. code:: python
-        
-            import jsonschema_rs
-        
-            validator = jsonschema_rs.JSONSchema({"minimum": 42})
-            validator.validate(41)  # raises ValidationError
-        
-        **NOTE**. This library is in early development.
-        
-        Performance
-        -----------
-        
-        According to our benchmarks, ``jsonschema-rs`` is usually faster than existing alternatives in real-life scenarios.
-        
-        However, for small schemas & inputs it might be slower than ``fastjsonschema`` or ``jsonschema`` on PyPy.
-        
-        Input values and schemas
-        ~~~~~~~~~~~~~~~~~~~~~~~~
-        
-        - `Zuora <https://github.com/APIs-guru/openapi-directory/blob/master/APIs/zuora.com/2021-04-23/openapi.yaml>`_ OpenAPI schema (``zuora.json``). Validated against `OpenAPI 3.0 JSON Schema <https://github.com/OAI/OpenAPI-Specification/blob/main/schemas/v3.0/schema.json>`_ (``openapi.json``).
-        - `Kubernetes <https://raw.githubusercontent.com/APIs-guru/openapi-directory/master/APIs/kubernetes.io/v1.10.0/swagger.yaml>`_ Swagger schema (``kubernetes.json``). Validated against `Swagger JSON Schema <https://github.com/OAI/OpenAPI-Specification/blob/main/schemas/v2.0/schema.json>`_ (``swagger.json``).
-        - Canadian border in GeoJSON format (``canada.json``). Schema is taken from the `GeoJSON website <https://geojson.org/schema/FeatureCollection.json>`_ (``geojson.json``).
-        - Concert data catalog (``citm_catalog.json``). Schema is inferred via `infers-jsonschema <https://github.com/Stranger6667/infers-jsonschema>`_ & manually adjusted (``citm_catalog_schema.json``).
-        - ``Fast`` is taken from `fastjsonschema benchmarks <https://github.com/horejsek/python-fastjsonschema/blob/master/performance.py#L15>`_ (``fast_schema.json``, `f`ast_valid.json`` and ``fast_invalid.json``).
-        
-        +----------------+-------------+---------------+
-        | Case           | Schema size | Instance size |
-        +================+=============+===============+
-        | OpenAPI        | 18 KB       | 4.5 MB        |
-        +----------------+-------------+---------------+
-        | Swagger        | 25 KB       | 3.0 MB        |
-        +----------------+-------------+---------------+
-        | Canada         | 4.8 KB      | 2.1 MB        |
-        +----------------+-------------+---------------+
-        | CITM catalog   | 2.3 KB      | 501 KB        |
-        +----------------+-------------+---------------+
-        | Fast (valid)   | 595 B       | 55 B          |
-        +----------------+-------------+---------------+
-        | Fast (invalid) | 595 B       | 60 B          |
-        +----------------+-------------+---------------+
-        
-        Compiled validators (when the input schema is compiled once and reused later). ``jsonschema-rs`` comes in three variants in the tables below:
-        
-        - ``validate``. This method raises ``ValidationError`` on errors or returns ``None`` on their absence.
-        - ``is_valid``. A faster method that returns a boolean result whether the instance is valid.
-        - ``overhead``. Only transforms data to underlying Rust types and do not perform any validation. Shows the Python -> Rust data conversion cost.
-        
-        Ratios are given against the ``validate`` variant.
-        
-        Small schemas:
-        
-        +-------------------------+------------------------+-----------------------+----------------------------+----------------------------+
-        | library                 | ``true``               | ``{"minimum": 10}``   | ``Fast (valid)``           | ``Fast (invalid)``         |
-        +=========================+========================+=======================+============================+============================+
-        | jsonschema-rs[validate] |              200.82 ns |             203.10 ns |                    1.22 us |                    1.51 us |
-        +-------------------------+------------------------+-----------------------+----------------------------+----------------------------+
-        | jsonschema-rs[is_valid] |  187.60 ns (**x0.93**) | 185.24 ns (**x0.91**) |      850.25 ns (**x0.69**) |        1.18 us (**x0.78**) |
-        +-------------------------+------------------------+-----------------------+----------------------------+----------------------------+
-        | jsonschema-rs[overhead] |  180.83 ns (**x0.90**) | 181.68 ns (**x0.89**) |      638.40 ns (**x0.52**) |        1.06 us (**x0.70**) |
-        +-------------------------+------------------------+-----------------------+----------------------------+----------------------------+
-        | fastjsonschema[CPython] |   58.57 ns (**x0.29**) | 109.10 ns (**x0.53**) |        4.16 us (**x3.40**) |        4.75 us (**x3.14**) |
-        +-------------------------+------------------------+-----------------------+----------------------------+----------------------------+
-        | fastjsonschema[PyPy]    |   1.32 ns (**x0.006**) |  33.39 ns (**x0.16**) |        890 ns  (**x0.72**) |         875 ns (**x0.58**) |
-        +-------------------------+------------------------+-----------------------+----------------------------+----------------------------+
-        | jsonschema[CPython]     |  226.48 ns (**x1.12**) |   1.88 us (**x9.25**) |      56.58 us (**x46.37**) |      57.31 us (**x37.95**) |
-        +-------------------------+------------------------+-----------------------+----------------------------+----------------------------+
-        | jsonschema[PyPy]        |   41.18 ns (**x0.20**) | 224.94 ns (**x1.10**) |      23.40 us (**x19.18**) |      22.78 us (**x15.08**) |
-        +-------------------------+------------------------+-----------------------+----------------------------+----------------------------+
-        
-        Large schemas:
-        
-        +-------------------------+-------------------------+--------------------------+----------------------------+---------------------------+
-        | library                 | ``Zuora (OpenAPI)``     | ``Kubernetes (Swagger)`` | ``Canada (GeoJSON)``       | ``CITM catalog``          |
-        +=========================+=========================+==========================+============================+===========================+
-        | jsonschema-rs[validate] |               13.970 ms |                13.076 ms |                   4.428 ms |                  4.715 ms |
-        +-------------------------+-------------------------+--------------------------+----------------------------+---------------------------+
-        | jsonschema-rs[is_valid] |   13.664 ms (**x0.97**) |    11.506 ms (**x0.87**) |       4.422 ms (**x0.99**) |      3.134 ms (**x0.66**) |
-        +-------------------------+-------------------------+--------------------------+----------------------------+---------------------------+
-        | jsonschema-rs[overhead] |   12.206 ms (**x0.87**) |     8.116 ms (**x0.62**) |       3.666 ms (**x0.82**) |      2.648 ms (**x0.56**) |
-        +-------------------------+-------------------------+--------------------------+----------------------------+---------------------------+
-        | fastjsonschema[CPython] |                  -- (1) |    87.020 ms (**x6.65**) |      31.705 ms (**x7.16**) |     11.715 ms (**x2.48**) |
-        +-------------------------+-------------------------+--------------------------+----------------------------+---------------------------+
-        | fastjsonschema[PyPy]    |                  -- (1) |    38.586 ms (**x2.95**) |       8.417 ms (**x1.90**) |      4.789 ms (**x1.01**) |
-        +-------------------------+-------------------------+--------------------------+----------------------------+---------------------------+
-        | jsonschema[CPython]     | 749.615 ms (**x53.65**) |     1.032 s (**x78.92**) |      1.286 s (**x290.42**) |   112.510 ms (**x23.86**) |
-        +-------------------------+-------------------------+--------------------------+----------------------------+---------------------------+
-        | jsonschema[PyPy]        | 611.056 ms (**x43.74**) |  592.584 ms (**x45.31**) |   530.567 ms (**x119.82**) |     28.619 ms (**x6.06**) |
-        +-------------------------+-------------------------+--------------------------+----------------------------+---------------------------+
-        
-        Notes:
-        
-        1. ``fastjsonschema`` fails to compile the Open API spec due to the presence of the ``uri-reference`` format (that is not defined in Draft 4). However, unknown formats are `explicitly supported <https://tools.ietf.org/html/draft-fge-json-schema-validation-00#section-7.1>`_ by the spec.
-        
-        The bigger the input is the bigger is performance win. You can take a look at benchmarks in ``benches/bench.py``.
-        
-        Package versions:
-        
-        - ``jsonschema-rs`` - latest version from the repository
-        - ``jsonschema`` - ``3.2.0``
-        - ``fastjsonschema`` - ``2.15.0``
-        
-        Measured with stable Rust 1.51, CPython 3.9.4 / PyPy3 7.3.4 on i8700K (12 cores), 32GB RAM, Arch Linux.
-        
-        Python support
-        --------------
-        
-        ``jsonschema-rs`` supports CPython 3.6, 3.7, 3.8 and 3.9.
-        
-        License
-        -------
-        
-        The code in this project is licensed under `MIT license`_.
-        By contributing to ``jsonschema-rs``, you agree that your contributions
-        will be licensed under its MIT license.
-         
-        .. |Build| image:: https://github.com/Stranger6667/jsonschema-rs/workflows/ci/badge.svg
-           :target: https://github.com/Stranger6667/jsonschema-rs/actions
-        .. |Version| image:: https://img.shields.io/pypi/v/jsonschema-rs.svg
-           :target: https://pypi.org/project/jsonschema-rs/
-        .. |Python versions| image:: https://img.shields.io/pypi/pyversions/jsonschema-rs.svg
-           :target: https://pypi.org/project/jsonschema-rs/
-        .. |License| image:: https://img.shields.io/pypi/l/jsonschema-rs.svg
-           :target: https://opensource.org/licenses/MIT
-        
-        .. _MIT license: https://opensource.org/licenses/MIT
-        
 Keywords: jsonschema validation rust
 Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
@@ -186,7 +19,176 @@
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Programming Language :: Rust
 Requires-Python: >=3.6
 Description-Content-Type: text/x-rst
+
+jsonschema-rs
+=============
+
+|Build| |Version| |Python versions| |License|
+
+Fast JSON Schema validation for Python implemented in Rust.
+
+Supported drafts:
+
+- Draft 7
+- Draft 6
+- Draft 4
+
+There are some notable restrictions at the moment:
+
+- The underlying crate doesn't support arbitrary precision integers yet, which may lead to ``SystemError`` when such value is used;
+- ``multipleOf`` keyword validation may produce false-negative results on some input. See `#84 <https://github.com/Stranger6667/jsonschema-rs/issues/84>`_ for more details
+
+Installation
+------------
+
+To install ``jsonschema-rs`` via ``pip`` run the following command:
+
+.. code:: bash
+
+    pip install jsonschema-rs
+
+Usage
+-----
+
+To check if the input document is valid:
+
+.. code:: python
+
+    import jsonschema_rs
+
+    validator = jsonschema_rs.JSONSchema({"minimum": 42})
+    validator.is_valid(45)  # True
+
+or:
+
+.. code:: python
+
+    import jsonschema_rs
+
+    validator = jsonschema_rs.JSONSchema({"minimum": 42})
+    validator.validate(41)  # raises ValidationError
+
+**NOTE**. This library is in early development.
+
+Performance
+-----------
+
+According to our benchmarks, ``jsonschema-rs`` is usually faster than existing alternatives in real-life scenarios.
+
+However, for small schemas & inputs it might be slower than ``fastjsonschema`` or ``jsonschema`` on PyPy.
+
+Input values and schemas
+~~~~~~~~~~~~~~~~~~~~~~~~
+
+- `Zuora <https://github.com/APIs-guru/openapi-directory/blob/master/APIs/zuora.com/2021-04-23/openapi.yaml>`_ OpenAPI schema (``zuora.json``). Validated against `OpenAPI 3.0 JSON Schema <https://github.com/OAI/OpenAPI-Specification/blob/main/schemas/v3.0/schema.json>`_ (``openapi.json``).
+- `Kubernetes <https://raw.githubusercontent.com/APIs-guru/openapi-directory/master/APIs/kubernetes.io/v1.10.0/swagger.yaml>`_ Swagger schema (``kubernetes.json``). Validated against `Swagger JSON Schema <https://github.com/OAI/OpenAPI-Specification/blob/main/schemas/v2.0/schema.json>`_ (``swagger.json``).
+- Canadian border in GeoJSON format (``canada.json``). Schema is taken from the `GeoJSON website <https://geojson.org/schema/FeatureCollection.json>`_ (``geojson.json``).
+- Concert data catalog (``citm_catalog.json``). Schema is inferred via `infers-jsonschema <https://github.com/Stranger6667/infers-jsonschema>`_ & manually adjusted (``citm_catalog_schema.json``).
+- ``Fast`` is taken from `fastjsonschema benchmarks <https://github.com/horejsek/python-fastjsonschema/blob/master/performance.py#L15>`_ (``fast_schema.json``, `f`ast_valid.json`` and ``fast_invalid.json``).
+
++----------------+-------------+---------------+
+| Case           | Schema size | Instance size |
++================+=============+===============+
+| OpenAPI        | 18 KB       | 4.5 MB        |
++----------------+-------------+---------------+
+| Swagger        | 25 KB       | 3.0 MB        |
++----------------+-------------+---------------+
+| Canada         | 4.8 KB      | 2.1 MB        |
++----------------+-------------+---------------+
+| CITM catalog   | 2.3 KB      | 501 KB        |
++----------------+-------------+---------------+
+| Fast (valid)   | 595 B       | 55 B          |
++----------------+-------------+---------------+
+| Fast (invalid) | 595 B       | 60 B          |
++----------------+-------------+---------------+
+
+Compiled validators (when the input schema is compiled once and reused later). ``jsonschema-rs`` comes in three variants in the tables below:
+
+- ``validate``. This method raises ``ValidationError`` on errors or returns ``None`` on their absence.
+- ``is_valid``. A faster method that returns a boolean result whether the instance is valid.
+- ``overhead``. Only transforms data to underlying Rust types and do not perform any validation. Shows the Python -> Rust data conversion cost.
+
+Ratios are given against the ``validate`` variant.
+
+Small schemas:
+
++-------------------------+------------------------+-----------------------+----------------------------+----------------------------+
+| library                 | ``true``               | ``{"minimum": 10}``   | ``Fast (valid)``           | ``Fast (invalid)``         |
++=========================+========================+=======================+============================+============================+
+| jsonschema-rs[validate] |              200.82 ns |             203.10 ns |                    1.22 us |                    1.51 us |
++-------------------------+------------------------+-----------------------+----------------------------+----------------------------+
+| jsonschema-rs[is_valid] |  187.60 ns (**x0.93**) | 185.24 ns (**x0.91**) |      850.25 ns (**x0.69**) |        1.18 us (**x0.78**) |
++-------------------------+------------------------+-----------------------+----------------------------+----------------------------+
+| jsonschema-rs[overhead] |  180.83 ns (**x0.90**) | 181.68 ns (**x0.89**) |      638.40 ns (**x0.52**) |        1.06 us (**x0.70**) |
++-------------------------+------------------------+-----------------------+----------------------------+----------------------------+
+| fastjsonschema[CPython] |   58.57 ns (**x0.29**) | 109.10 ns (**x0.53**) |        4.16 us (**x3.40**) |        4.75 us (**x3.14**) |
++-------------------------+------------------------+-----------------------+----------------------------+----------------------------+
+| fastjsonschema[PyPy]    |   1.32 ns (**x0.006**) |  33.39 ns (**x0.16**) |        890 ns  (**x0.72**) |         875 ns (**x0.58**) |
++-------------------------+------------------------+-----------------------+----------------------------+----------------------------+
+| jsonschema[CPython]     |  226.48 ns (**x1.12**) |   1.88 us (**x9.25**) |      56.58 us (**x46.37**) |      57.31 us (**x37.95**) |
++-------------------------+------------------------+-----------------------+----------------------------+----------------------------+
+| jsonschema[PyPy]        |   41.18 ns (**x0.20**) | 224.94 ns (**x1.10**) |      23.40 us (**x19.18**) |      22.78 us (**x15.08**) |
++-------------------------+------------------------+-----------------------+----------------------------+----------------------------+
+
+Large schemas:
+
++-------------------------+-------------------------+--------------------------+----------------------------+---------------------------+
+| library                 | ``Zuora (OpenAPI)``     | ``Kubernetes (Swagger)`` | ``Canada (GeoJSON)``       | ``CITM catalog``          |
++=========================+=========================+==========================+============================+===========================+
+| jsonschema-rs[validate] |               13.970 ms |                13.076 ms |                   4.428 ms |                  4.715 ms |
++-------------------------+-------------------------+--------------------------+----------------------------+---------------------------+
+| jsonschema-rs[is_valid] |   13.664 ms (**x0.97**) |    11.506 ms (**x0.87**) |       4.422 ms (**x0.99**) |      3.134 ms (**x0.66**) |
++-------------------------+-------------------------+--------------------------+----------------------------+---------------------------+
+| jsonschema-rs[overhead] |   12.206 ms (**x0.87**) |     8.116 ms (**x0.62**) |       3.666 ms (**x0.82**) |      2.648 ms (**x0.56**) |
++-------------------------+-------------------------+--------------------------+----------------------------+---------------------------+
+| fastjsonschema[CPython] |                  -- (1) |    87.020 ms (**x6.65**) |      31.705 ms (**x7.16**) |     11.715 ms (**x2.48**) |
++-------------------------+-------------------------+--------------------------+----------------------------+---------------------------+
+| fastjsonschema[PyPy]    |                  -- (1) |    38.586 ms (**x2.95**) |       8.417 ms (**x1.90**) |      4.789 ms (**x1.01**) |
++-------------------------+-------------------------+--------------------------+----------------------------+---------------------------+
+| jsonschema[CPython]     | 749.615 ms (**x53.65**) |     1.032 s (**x78.92**) |      1.286 s (**x290.42**) |   112.510 ms (**x23.86**) |
++-------------------------+-------------------------+--------------------------+----------------------------+---------------------------+
+| jsonschema[PyPy]        | 611.056 ms (**x43.74**) |  592.584 ms (**x45.31**) |   530.567 ms (**x119.82**) |     28.619 ms (**x6.06**) |
++-------------------------+-------------------------+--------------------------+----------------------------+---------------------------+
+
+Notes:
+
+1. ``fastjsonschema`` fails to compile the Open API spec due to the presence of the ``uri-reference`` format (that is not defined in Draft 4). However, unknown formats are `explicitly supported <https://tools.ietf.org/html/draft-fge-json-schema-validation-00#section-7.1>`_ by the spec.
+
+The bigger the input is the bigger is performance win. You can take a look at benchmarks in ``benches/bench.py``.
+
+Package versions:
+
+- ``jsonschema-rs`` - latest version from the repository
+- ``jsonschema`` - ``3.2.0``
+- ``fastjsonschema`` - ``2.15.0``
+
+Measured with stable Rust 1.51, CPython 3.9.4 / PyPy3 7.3.4 on i8700K (12 cores), 32GB RAM, Arch Linux.
+
+Python support
+--------------
+
+``jsonschema-rs`` supports CPython 3.6, 3.7, 3.8 and 3.9.
+
+License
+-------
+
+The code in this project is licensed under `MIT license`_.
+By contributing to ``jsonschema-rs``, you agree that your contributions
+will be licensed under its MIT license.
+ 
+.. |Build| image:: https://github.com/Stranger6667/jsonschema-rs/workflows/ci/badge.svg
+   :target: https://github.com/Stranger6667/jsonschema-rs/actions
+.. |Version| image:: https://img.shields.io/pypi/v/jsonschema-rs.svg
+   :target: https://pypi.org/project/jsonschema-rs/
+.. |Python versions| image:: https://img.shields.io/pypi/pyversions/jsonschema-rs.svg
+   :target: https://pypi.org/project/jsonschema-rs/
+.. |License| image:: https://img.shields.io/pypi/l/jsonschema-rs.svg
+   :target: https://opensource.org/licenses/MIT
+
+.. _MIT license: https://opensource.org/licenses/MIT
+
+
```

### Comparing `jsonschema_rs-0.9.0/jsonschema_rs.egg-info/SOURCES.txt` & `jsonschema_rs-0.9.1/jsonschema_rs.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `jsonschema_rs-0.9.0/setup.py` & `jsonschema_rs-0.9.1/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -16,15 +16,15 @@
         )
     )
 
 
 def call_setup():
     setup(
         name="jsonschema_rs",
-        version="0.9.0",
+        version="0.9.1",
         description="Fast JSON Schema validation for Python implemented in Rust",
         long_description=open("README.rst", encoding="utf-8").read(),
         long_description_content_type="text/x-rst",
         keywords="jsonschema validation rust",
         author="Dmitry Dygalo",
         author_email="dadygalo@gmail.com",
         maintainer="Dmitry Dygalo",
```

### Comparing `jsonschema_rs-0.9.0/src/lib.rs` & `jsonschema_rs-0.9.1/src/lib.rs`

 * *Files identical despite different names*

### Comparing `jsonschema_rs-0.9.0/src/ser.rs` & `jsonschema_rs-0.9.1/src/ser.rs`

 * *Files identical despite different names*

### Comparing `jsonschema_rs-0.9.0/src/string.rs` & `jsonschema_rs-0.9.1/src/string.rs`

 * *Files identical despite different names*

### Comparing `jsonschema_rs-0.9.0/src/types.rs` & `jsonschema_rs-0.9.1/src/types.rs`

 * *Files identical despite different names*

