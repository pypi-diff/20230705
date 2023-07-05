# Comparing `tmp/getdaft-0.1.7.tar.gz` & `tmp/getdaft-0.1.8.tar.gz`

## Comparing `getdaft-0.1.7.tar` & `getdaft-0.1.8.tar`

### file list

```diff
@@ -1,488 +1,499 @@
--rw-r--r--   0        0        0     1120 1970-01-01 00:00:00.000000 getdaft-0.1.7/local_dependencies/daft-io/Cargo.toml
--rw-r--r--   0      501       20     1028 2023-06-26 18:37:01.000000 getdaft-0.1.7/local_dependencies/daft-io/src/config.rs
--rw-r--r--   0      501       20     2594 2023-06-26 18:37:01.000000 getdaft-0.1.7/local_dependencies/daft-io/src/http.rs
--rw-r--r--   0      501       20     8588 2023-06-26 18:37:01.000000 getdaft-0.1.7/local_dependencies/daft-io/src/lib.rs
--rw-r--r--   0      501       20     2800 2023-06-26 18:37:01.000000 getdaft-0.1.7/local_dependencies/daft-io/src/local.rs
--rw-r--r--   0      501       20     1472 2023-06-26 18:37:01.000000 getdaft-0.1.7/local_dependencies/daft-io/src/object_io.rs
--rw-r--r--   0      501       20     1240 2023-06-26 18:37:01.000000 getdaft-0.1.7/local_dependencies/daft-io/src/python.rs
--rw-r--r--   0      501       20     4484 2023-06-26 18:37:01.000000 getdaft-0.1.7/local_dependencies/daft-io/src/s3_like.rs
--rw-r--r--   0        0        0      649 1970-01-01 00:00:00.000000 getdaft-0.1.7/local_dependencies/common-error/Cargo.toml
--rw-r--r--   0      501       20     2849 2023-06-26 18:37:01.000000 getdaft-0.1.7/local_dependencies/common-error/src/error.rs
--rw-r--r--   0      501       20       64 2023-06-26 18:37:01.000000 getdaft-0.1.7/local_dependencies/common-error/src/lib.rs
--rw-r--r--   0        0        0     1565 1970-01-01 00:00:00.000000 getdaft-0.1.7/local_dependencies/daft-core/Cargo.toml
--rw-r--r--   0      501       20     5844 2023-06-26 18:37:01.000000 getdaft-0.1.7/local_dependencies/daft-core/src/array/from.rs
--rw-r--r--   0      501       20      734 2023-06-26 18:37:01.000000 getdaft-0.1.7/local_dependencies/daft-core/src/array/iterator.rs
--rw-r--r--   0      501       20     3012 2023-06-26 18:37:01.000000 getdaft-0.1.7/local_dependencies/daft-core/src/array/mod.rs
--rw-r--r--   0      501       20      269 2023-06-26 18:37:01.000000 getdaft-0.1.7/local_dependencies/daft-core/src/array/ops/abs.rs
--rw-r--r--   0      501       20      738 2023-06-26 18:37:01.000000 getdaft-0.1.7/local_dependencies/daft-core/src/array/ops/apply.rs
--rw-r--r--   0      501       20      849 2023-06-26 18:37:01.000000 getdaft-0.1.7/local_dependencies/daft-core/src/array/ops/arange.rs
--rw-r--r--   0      501       20     6972 2023-06-26 18:37:01.000000 getdaft-0.1.7/local_dependencies/daft-core/src/array/ops/arithmetic.rs
--rw-r--r--   0      501       20     3055 2023-06-26 18:37:01.000000 getdaft-0.1.7/local_dependencies/daft-core/src/array/ops/arrow2/comparison.rs
--rw-r--r--   0      501       20       34 2023-06-26 18:37:01.000000 getdaft-0.1.7/local_dependencies/daft-core/src/array/ops/arrow2/mod.rs
--rw-r--r--   0      501       20       19 2023-06-26 18:37:01.000000 getdaft-0.1.7/local_dependencies/daft-core/src/array/ops/arrow2/sort/mod.rs
--rw-r--r--   0      501       20     3482 2023-06-26 18:37:01.000000 getdaft-0.1.7/local_dependencies/daft-core/src/array/ops/arrow2/sort/primitive/common.rs
--rw-r--r--   0      501       20      723 2023-06-26 18:37:01.000000 getdaft-0.1.7/local_dependencies/daft-core/src/array/ops/arrow2/sort/primitive/indices.rs
--rw-r--r--   0      501       20       47 2023-06-26 18:37:01.000000 getdaft-0.1.7/local_dependencies/daft-core/src/array/ops/arrow2/sort/primitive/mod.rs
--rw-r--r--   0      501       20     8075 2023-06-26 18:37:01.000000 getdaft-0.1.7/local_dependencies/daft-core/src/array/ops/arrow2/sort/primitive/sort.rs
--rw-r--r--   0      501       20     2409 2023-06-26 18:37:01.000000 getdaft-0.1.7/local_dependencies/daft-core/src/array/ops/as_arrow.rs
--rw-r--r--   0      501       20    11395 2023-06-26 18:37:01.000000 getdaft-0.1.7/local_dependencies/daft-core/src/array/ops/broadcast.rs
--rw-r--r--   0      501       20    40353 2023-06-26 18:37:01.000000 getdaft-0.1.7/local_dependencies/daft-core/src/array/ops/cast.rs
--rw-r--r--   0      501       20    11029 2023-06-26 18:37:01.000000 getdaft-0.1.7/local_dependencies/daft-core/src/array/ops/compare_agg.rs
--rw-r--r--   0      501       20    47241 2023-06-26 18:37:01.000000 getdaft-0.1.7/local_dependencies/daft-core/src/array/ops/comparison.rs
--rw-r--r--   0      501       20     1630 2023-06-26 18:37:01.000000 getdaft-0.1.7/local_dependencies/daft-core/src/array/ops/concat.rs
--rw-r--r--   0      501       20     5991 2023-06-26 18:37:01.000000 getdaft-0.1.7/local_dependencies/daft-core/src/array/ops/concat_agg.rs
--rw-r--r--   0      501       20     1444 2023-06-26 18:37:01.000000 getdaft-0.1.7/local_dependencies/daft-core/src/array/ops/count.rs
--rw-r--r--   0      501       20     1548 2023-06-26 18:37:01.000000 getdaft-0.1.7/local_dependencies/daft-core/src/array/ops/date.rs
--rw-r--r--   0      501       20     2430 2023-06-26 18:37:01.000000 getdaft-0.1.7/local_dependencies/daft-core/src/array/ops/filter.rs
--rw-r--r--   0      501       20     1271 2023-06-26 18:37:01.000000 getdaft-0.1.7/local_dependencies/daft-core/src/array/ops/float.rs
--rw-r--r--   0      501       20     1936 2023-06-26 18:37:01.000000 getdaft-0.1.7/local_dependencies/daft-core/src/array/ops/full.rs
--rw-r--r--   0      501       20     4823 2023-06-26 18:37:01.000000 getdaft-0.1.7/local_dependencies/daft-core/src/array/ops/get.rs
--rw-r--r--   0      501       20     4119 2023-06-26 18:37:01.000000 getdaft-0.1.7/local_dependencies/daft-core/src/array/ops/groups.rs
--rw-r--r--   0      501       20     1523 2023-06-26 18:37:01.000000 getdaft-0.1.7/local_dependencies/daft-core/src/array/ops/hash.rs
--rw-r--r--   0      501       20    12222 2023-06-26 18:37:01.000000 getdaft-0.1.7/local_dependencies/daft-core/src/array/ops/if_else.rs
--rw-r--r--   0      501       20    29241 2023-06-26 18:37:01.000000 getdaft-0.1.7/local_dependencies/daft-core/src/array/ops/image.rs
--rw-r--r--   0      501       20     1069 2023-06-26 18:37:01.000000 getdaft-0.1.7/local_dependencies/daft-core/src/array/ops/len.rs
--rw-r--r--   0      501       20     6625 2023-06-26 18:37:01.000000 getdaft-0.1.7/local_dependencies/daft-core/src/array/ops/list.rs
--rw-r--r--   0      501       20     3367 2023-06-26 18:37:01.000000 getdaft-0.1.7/local_dependencies/daft-core/src/array/ops/list_agg.rs
--rw-r--r--   0      501       20     1634 2023-06-26 18:37:01.000000 getdaft-0.1.7/local_dependencies/daft-core/src/array/ops/mean.rs
--rw-r--r--   0      501       20     2629 2023-06-26 18:37:01.000000 getdaft-0.1.7/local_dependencies/daft-core/src/array/ops/mod.rs
--rw-r--r--   0      501       20     1325 2023-06-26 18:37:01.000000 getdaft-0.1.7/local_dependencies/daft-core/src/array/ops/null.rs
--rw-r--r--   0      501       20     3826 2023-06-26 18:37:01.000000 getdaft-0.1.7/local_dependencies/daft-core/src/array/ops/pairwise.rs
--rw-r--r--   0      501       20     9877 2023-06-26 18:37:01.000000 getdaft-0.1.7/local_dependencies/daft-core/src/array/ops/repr.rs
--rw-r--r--   0      501       20      491 2023-06-26 18:37:01.000000 getdaft-0.1.7/local_dependencies/daft-core/src/array/ops/search_sorted.rs
--rw-r--r--   0      501       20    19867 2023-06-26 18:37:01.000000 getdaft-0.1.7/local_dependencies/daft-core/src/array/ops/sort.rs
--rw-r--r--   0      501       20     2396 2023-06-26 18:37:01.000000 getdaft-0.1.7/local_dependencies/daft-core/src/array/ops/sum.rs
--rw-r--r--   0      501       20     4604 2023-06-26 18:37:01.000000 getdaft-0.1.7/local_dependencies/daft-core/src/array/ops/take.rs
--rw-r--r--   0      501       20     5279 2023-06-26 18:37:01.000000 getdaft-0.1.7/local_dependencies/daft-core/src/array/ops/utf8.rs
--rw-r--r--   0      501       20      995 2023-06-26 18:37:01.000000 getdaft-0.1.7/local_dependencies/daft-core/src/array/pseudo_arrow/compute.rs
--rw-r--r--   0      501       20    13611 2023-06-26 18:37:01.000000 getdaft-0.1.7/local_dependencies/daft-core/src/array/pseudo_arrow/mod.rs
--rw-r--r--   0      501       20     2502 2023-06-26 18:37:01.000000 getdaft-0.1.7/local_dependencies/daft-core/src/array/pseudo_arrow/python.rs
--rw-r--r--   0      501       20    15026 2023-06-26 18:37:01.000000 getdaft-0.1.7/local_dependencies/daft-core/src/datatypes/dtype.rs
--rw-r--r--   0      501       20     2021 2023-06-26 18:37:01.000000 getdaft-0.1.7/local_dependencies/daft-core/src/datatypes/field.rs
--rw-r--r--   0      501       20     3187 2023-06-26 18:37:01.000000 getdaft-0.1.7/local_dependencies/daft-core/src/datatypes/image_format.rs
--rw-r--r--   0      501       20     6382 2023-06-26 18:37:01.000000 getdaft-0.1.7/local_dependencies/daft-core/src/datatypes/image_mode.rs
--rw-r--r--   0      501       20     3428 2023-06-26 18:37:01.000000 getdaft-0.1.7/local_dependencies/daft-core/src/datatypes/logical.rs
--rw-r--r--   0      501       20     9200 2023-06-26 18:37:01.000000 getdaft-0.1.7/local_dependencies/daft-core/src/datatypes/matching.rs
--rw-r--r--   0      501       20     6889 2023-06-26 18:37:01.000000 getdaft-0.1.7/local_dependencies/daft-core/src/datatypes/mod.rs
--rw-r--r--   0      501       20     1083 2023-06-26 18:37:01.000000 getdaft-0.1.7/local_dependencies/daft-core/src/datatypes/time_unit.rs
--rw-r--r--   0      501       20     5128 2023-06-26 18:37:01.000000 getdaft-0.1.7/local_dependencies/daft-core/src/ffi.rs
--rw-r--r--   0      501       20     6022 2023-06-26 18:37:01.000000 getdaft-0.1.7/local_dependencies/daft-core/src/kernels/hashing.rs
--rw-r--r--   0      501       20       54 2023-06-26 18:37:01.000000 getdaft-0.1.7/local_dependencies/daft-core/src/kernels/mod.rs
--rw-r--r--   0      501       20    12159 2023-06-26 18:37:01.000000 getdaft-0.1.7/local_dependencies/daft-core/src/kernels/search_sorted.rs
--rw-r--r--   0      501       20     3917 2023-06-26 18:37:01.000000 getdaft-0.1.7/local_dependencies/daft-core/src/kernels/utf8.rs
--rw-r--r--   0      501       20      553 2023-06-26 18:37:01.000000 getdaft-0.1.7/local_dependencies/daft-core/src/lib.rs
--rw-r--r--   0      501       20     8528 2023-06-26 18:37:01.000000 getdaft-0.1.7/local_dependencies/daft-core/src/python/datatype.rs
--rw-r--r--   0      501       20     1661 2023-06-26 18:37:01.000000 getdaft-0.1.7/local_dependencies/daft-core/src/python/field.rs
--rw-r--r--   0      501       20      610 2023-06-26 18:37:01.000000 getdaft-0.1.7/local_dependencies/daft-core/src/python/mod.rs
--rw-r--r--   0      501       20     2843 2023-06-26 18:37:01.000000 getdaft-0.1.7/local_dependencies/daft-core/src/python/schema.rs
--rw-r--r--   0      501       20    12308 2023-06-26 18:37:01.000000 getdaft-0.1.7/local_dependencies/daft-core/src/python/series.rs
--rw-r--r--   0      501       20     3669 2023-06-26 18:37:01.000000 getdaft-0.1.7/local_dependencies/daft-core/src/schema.rs
--rw-r--r--   0      501       20    10722 2023-06-26 18:37:01.000000 getdaft-0.1.7/local_dependencies/daft-core/src/series/array_impl/data_array.rs
--rw-r--r--   0      501       20     5704 2023-06-26 18:37:01.000000 getdaft-0.1.7/local_dependencies/daft-core/src/series/array_impl/logical_array.rs
--rw-r--r--   0      501       20      161 2023-06-26 18:37:01.000000 getdaft-0.1.7/local_dependencies/daft-core/src/series/array_impl/mod.rs
--rw-r--r--   0      501       20     2106 2023-06-26 18:37:01.000000 getdaft-0.1.7/local_dependencies/daft-core/src/series/from.rs
--rw-r--r--   0      501       20     2309 2023-06-26 18:37:01.000000 getdaft-0.1.7/local_dependencies/daft-core/src/series/mod.rs
--rw-r--r--   0      501       20      910 2023-06-26 18:37:01.000000 getdaft-0.1.7/local_dependencies/daft-core/src/series/ops/abs.rs
--rw-r--r--   0      501       20     5199 2023-06-26 18:37:01.000000 getdaft-0.1.7/local_dependencies/daft-core/src/series/ops/agg.rs
--rw-r--r--   0      501       20     6289 2023-06-26 18:37:01.000000 getdaft-0.1.7/local_dependencies/daft-core/src/series/ops/arithmetic.rs
--rw-r--r--   0      501       20     1924 2023-06-26 18:37:01.000000 getdaft-0.1.7/local_dependencies/daft-core/src/series/ops/broadcast.rs
--rw-r--r--   0      501       20      205 2023-06-26 18:37:01.000000 getdaft-0.1.7/local_dependencies/daft-core/src/series/ops/cast.rs
--rw-r--r--   0      501       20     2616 2023-06-26 18:37:01.000000 getdaft-0.1.7/local_dependencies/daft-core/src/series/ops/comparison.rs
--rw-r--r--   0      501       20     1565 2023-06-26 18:37:01.000000 getdaft-0.1.7/local_dependencies/daft-core/src/series/ops/concat.rs
--rw-r--r--   0      501       20     1820 2023-06-26 18:37:01.000000 getdaft-0.1.7/local_dependencies/daft-core/src/series/ops/date.rs
--rw-r--r--   0      501       20     3621 2023-06-26 18:37:01.000000 getdaft-0.1.7/local_dependencies/daft-core/src/series/ops/downcast.rs
--rw-r--r--   0      501       20      693 2023-06-26 18:37:01.000000 getdaft-0.1.7/local_dependencies/daft-core/src/series/ops/filter.rs
--rw-r--r--   0      501       20      411 2023-06-26 18:37:01.000000 getdaft-0.1.7/local_dependencies/daft-core/src/series/ops/float.rs
--rw-r--r--   0      501       20      439 2023-06-26 18:37:01.000000 getdaft-0.1.7/local_dependencies/daft-core/src/series/ops/groups.rs
--rw-r--r--   0      501       20      416 2023-06-26 18:37:01.000000 getdaft-0.1.7/local_dependencies/daft-core/src/series/ops/hash.rs
--rw-r--r--   0      501       20      324 2023-06-26 18:37:01.000000 getdaft-0.1.7/local_dependencies/daft-core/src/series/ops/if_else.rs
--rw-r--r--   0      501       20     2468 2023-06-26 18:37:01.000000 getdaft-0.1.7/local_dependencies/daft-core/src/series/ops/image.rs
--rw-r--r--   0      501       20      297 2023-06-26 18:37:01.000000 getdaft-0.1.7/local_dependencies/daft-core/src/series/ops/len.rs
--rw-r--r--   0      501       20     2351 2023-06-26 18:37:01.000000 getdaft-0.1.7/local_dependencies/daft-core/src/series/ops/list.rs
--rw-r--r--   0      501       20     2367 2023-06-26 18:37:01.000000 getdaft-0.1.7/local_dependencies/daft-core/src/series/ops/mod.rs
--rw-r--r--   0      501       20      475 2023-06-26 18:37:01.000000 getdaft-0.1.7/local_dependencies/daft-core/src/series/ops/not.rs
--rw-r--r--   0      501       20      160 2023-06-26 18:37:01.000000 getdaft-0.1.7/local_dependencies/daft-core/src/series/ops/null.rs
--rw-r--r--   0      501       20      645 2023-06-26 18:37:01.000000 getdaft-0.1.7/local_dependencies/daft-core/src/series/ops/search_sorted.rs
--rw-r--r--   0      501       20     1504 2023-06-26 18:37:01.000000 getdaft-0.1.7/local_dependencies/daft-core/src/series/ops/sort.rs
--rw-r--r--   0      501       20      662 2023-06-26 18:37:01.000000 getdaft-0.1.7/local_dependencies/daft-core/src/series/ops/take.rs
--rw-r--r--   0      501       20     1526 2023-06-26 18:37:01.000000 getdaft-0.1.7/local_dependencies/daft-core/src/series/ops/utf8.rs
--rw-r--r--   0      501       20     1406 2023-06-26 18:37:01.000000 getdaft-0.1.7/local_dependencies/daft-core/src/series/series_like.rs
--rw-r--r--   0      501       20     5401 2023-06-26 18:37:01.000000 getdaft-0.1.7/local_dependencies/daft-core/src/utils/arrow.rs
--rw-r--r--   0      501       20       34 2023-06-26 18:37:01.000000 getdaft-0.1.7/local_dependencies/daft-core/src/utils/mod.rs
--rw-r--r--   0      501       20    10065 2023-06-26 18:37:01.000000 getdaft-0.1.7/local_dependencies/daft-core/src/utils/supertype.rs
--rw-r--r--   0        0        0     1001 1970-01-01 00:00:00.000000 getdaft-0.1.7/local_dependencies/daft-table/Cargo.toml
--rw-r--r--   0      501       20     2853 2023-06-26 18:37:01.000000 getdaft-0.1.7/local_dependencies/daft-table/src/ffi.rs
--rw-r--r--   0      501       20    20533 2023-06-26 18:37:01.000000 getdaft-0.1.7/local_dependencies/daft-table/src/lib.rs
--rw-r--r--   0      501       20     2168 2023-06-26 18:37:01.000000 getdaft-0.1.7/local_dependencies/daft-table/src/ops/agg.rs
--rw-r--r--   0      501       20     3748 2023-06-26 18:37:01.000000 getdaft-0.1.7/local_dependencies/daft-table/src/ops/explode.rs
--rw-r--r--   0      501       20     4415 2023-06-26 18:37:01.000000 getdaft-0.1.7/local_dependencies/daft-table/src/ops/groups.rs
--rw-r--r--   0      501       20     2898 2023-06-26 18:37:01.000000 getdaft-0.1.7/local_dependencies/daft-table/src/ops/hash.rs
--rw-r--r--   0      501       20     2499 2023-06-26 18:37:01.000000 getdaft-0.1.7/local_dependencies/daft-table/src/ops/joins/hash_join.rs
--rw-r--r--   0      501       20     3727 2023-06-26 18:37:01.000000 getdaft-0.1.7/local_dependencies/daft-table/src/ops/joins/mod.rs
--rw-r--r--   0      501       20       99 2023-06-26 18:37:01.000000 getdaft-0.1.7/local_dependencies/daft-table/src/ops/mod.rs
--rw-r--r--   0      501       20     3478 2023-06-26 18:37:01.000000 getdaft-0.1.7/local_dependencies/daft-table/src/ops/partition.rs
--rw-r--r--   0      501       20     1808 2023-06-26 18:37:01.000000 getdaft-0.1.7/local_dependencies/daft-table/src/ops/search_sorted.rs
--rw-r--r--   0      501       20      998 2023-06-26 18:37:01.000000 getdaft-0.1.7/local_dependencies/daft-table/src/ops/sort.rs
--rw-r--r--   0      501       20    11179 2023-06-26 18:37:01.000000 getdaft-0.1.7/local_dependencies/daft-table/src/python.rs
--rw-r--r--   0        0        0      679 1970-01-01 00:00:00.000000 getdaft-0.1.7/local_dependencies/daft-dsl/Cargo.toml
--rw-r--r--   0      501       20      273 2023-06-26 18:37:01.000000 getdaft-0.1.7/local_dependencies/daft-dsl/src/README.md
--rw-r--r--   0      501       20     1454 2023-06-26 18:37:01.000000 getdaft-0.1.7/local_dependencies/daft-dsl/src/arithmetic.rs
--rw-r--r--   0      501       20    21833 2023-06-26 18:37:01.000000 getdaft-0.1.7/local_dependencies/daft-dsl/src/expr.rs
--rw-r--r--   0      501       20     1456 2023-06-26 18:37:01.000000 getdaft-0.1.7/local_dependencies/daft-dsl/src/functions/float/is_nan.rs
--rw-r--r--   0      501       20      582 2023-06-26 18:37:01.000000 getdaft-0.1.7/local_dependencies/daft-dsl/src/functions/float/mod.rs
--rw-r--r--   0      501       20     1353 2023-06-26 18:37:01.000000 getdaft-0.1.7/local_dependencies/daft-dsl/src/functions/image/decode.rs
--rw-r--r--   0      501       20     1790 2023-06-26 18:37:01.000000 getdaft-0.1.7/local_dependencies/daft-dsl/src/functions/image/encode.rs
--rw-r--r--   0      501       20     1292 2023-06-26 18:37:01.000000 getdaft-0.1.7/local_dependencies/daft-dsl/src/functions/image/mod.rs
--rw-r--r--   0      501       20     2524 2023-06-26 18:37:01.000000 getdaft-0.1.7/local_dependencies/daft-dsl/src/functions/image/resize.rs
--rw-r--r--   0      501       20     1130 2023-06-26 18:37:01.000000 getdaft-0.1.7/local_dependencies/daft-dsl/src/functions/list/explode.rs
--rw-r--r--   0      501       20     2329 2023-06-26 18:37:01.000000 getdaft-0.1.7/local_dependencies/daft-dsl/src/functions/list/join.rs
--rw-r--r--   0      501       20      873 2023-06-26 18:37:01.000000 getdaft-0.1.7/local_dependencies/daft-dsl/src/functions/list/mod.rs
--rw-r--r--   0      501       20     2085 2023-06-26 18:37:01.000000 getdaft-0.1.7/local_dependencies/daft-dsl/src/functions/mod.rs
--rw-r--r--   0      501       20     1197 2023-06-26 18:37:01.000000 getdaft-0.1.7/local_dependencies/daft-dsl/src/functions/numeric/abs.rs
--rw-r--r--   0      501       20      575 2023-06-26 18:37:01.000000 getdaft-0.1.7/local_dependencies/daft-dsl/src/functions/numeric/mod.rs
--rw-r--r--   0      501       20      684 2023-06-26 18:37:01.000000 getdaft-0.1.7/local_dependencies/daft-dsl/src/functions/python/mod.rs
--rw-r--r--   0      501       20     2050 2023-06-26 18:37:01.000000 getdaft-0.1.7/local_dependencies/daft-dsl/src/functions/python/partial_udf.rs
--rw-r--r--   0      501       20     2793 2023-06-26 18:37:01.000000 getdaft-0.1.7/local_dependencies/daft-dsl/src/functions/python/udf.rs
--rw-r--r--   0      501       20     1344 2023-06-26 18:37:01.000000 getdaft-0.1.7/local_dependencies/daft-dsl/src/functions/temporal/day.rs
--rw-r--r--   0      501       20     1373 2023-06-26 18:37:01.000000 getdaft-0.1.7/local_dependencies/daft-dsl/src/functions/temporal/day_of_week.rs
--rw-r--r--   0      501       20     1415 2023-06-26 18:37:01.000000 getdaft-0.1.7/local_dependencies/daft-dsl/src/functions/temporal/mod.rs
--rw-r--r--   0      501       20     1355 2023-06-26 18:37:01.000000 getdaft-0.1.7/local_dependencies/daft-dsl/src/functions/temporal/month.rs
--rw-r--r--   0      501       20     1349 2023-06-26 18:37:01.000000 getdaft-0.1.7/local_dependencies/daft-dsl/src/functions/temporal/year.rs
--rw-r--r--   0      501       20     2295 2023-06-26 18:37:01.000000 getdaft-0.1.7/local_dependencies/daft-dsl/src/functions/uri/download.rs
--rw-r--r--   0      501       20     1073 2023-06-26 18:37:01.000000 getdaft-0.1.7/local_dependencies/daft-dsl/src/functions/uri/mod.rs
--rw-r--r--   0      501       20     1652 2023-06-26 18:37:01.000000 getdaft-0.1.7/local_dependencies/daft-dsl/src/functions/utf8/contains.rs
--rw-r--r--   0      501       20     1651 2023-06-26 18:37:01.000000 getdaft-0.1.7/local_dependencies/daft-dsl/src/functions/utf8/endswith.rs
--rw-r--r--   0      501       20     1370 2023-06-26 18:37:01.000000 getdaft-0.1.7/local_dependencies/daft-dsl/src/functions/utf8/length.rs
--rw-r--r--   0      501       20     1519 2023-06-26 18:37:01.000000 getdaft-0.1.7/local_dependencies/daft-dsl/src/functions/utf8/mod.rs
--rw-r--r--   0      501       20     1661 2023-06-26 18:37:01.000000 getdaft-0.1.7/local_dependencies/daft-dsl/src/functions/utf8/startswith.rs
--rw-r--r--   0      501       20      707 2023-06-26 18:37:01.000000 getdaft-0.1.7/local_dependencies/daft-dsl/src/lib.rs
--rw-r--r--   0      501       20     4967 2023-06-26 18:37:01.000000 getdaft-0.1.7/local_dependencies/daft-dsl/src/lit.rs
--rw-r--r--   0      501       20     5298 2023-06-26 18:37:01.000000 getdaft-0.1.7/local_dependencies/daft-dsl/src/optimization.rs
--rw-r--r--   0      501       20     1982 2023-06-26 18:37:01.000000 getdaft-0.1.7/local_dependencies/daft-dsl/src/pyobject.rs
--rw-r--r--   0      501       20    11937 2023-06-26 18:37:01.000000 getdaft-0.1.7/local_dependencies/daft-dsl/src/python.rs
--rw-r--r--   0        0        0     2202 1970-01-01 00:00:00.000000 getdaft-0.1.7/Cargo.toml
--rw-r--r--   0      501       20      834 2023-06-26 18:37:01.000000 getdaft-0.1.7/.github/ISSUE_TEMPLATE/bug_report.md
--rw-r--r--   0      501       20      595 2023-06-26 18:37:01.000000 getdaft-0.1.7/.github/ISSUE_TEMPLATE/feature_request.md
--rw-r--r--   0      501       20      431 2023-06-26 18:37:01.000000 getdaft-0.1.7/.github/dependabot.yml
--rw-r--r--   0      501       20     1063 2023-06-26 18:37:01.000000 getdaft-0.1.7/.github/release-drafter.yml
--rw-r--r--   0      501       20     1333 2023-06-26 18:37:01.000000 getdaft-0.1.7/.github/workflows/broken-link-checker.yml
--rw-r--r--   0      501       20     3378 2023-06-26 18:37:01.000000 getdaft-0.1.7/.github/workflows/daft-profiling.yml
--rw-r--r--   0      501       20     1627 2023-06-26 18:37:01.000000 getdaft-0.1.7/.github/workflows/notebook-checker.yml
--rw-r--r--   0      501       20     2194 2023-06-26 18:37:01.000000 getdaft-0.1.7/.github/workflows/property-based-tests.yml
--rw-r--r--   0      501       20    13636 2023-06-26 18:37:01.000000 getdaft-0.1.7/.github/workflows/python-package.yml
--rw-r--r--   0      501       20     6185 2023-06-26 18:37:01.000000 getdaft-0.1.7/.github/workflows/python-publish.yml
--rw-r--r--   0      501       20     2638 2023-06-26 18:37:01.000000 getdaft-0.1.7/.github/workflows/ray-compatibility.yml
--rw-r--r--   0      501       20     2696 2023-06-26 18:37:01.000000 getdaft-0.1.7/.github/workflows/release-drafter.yml
--rw-r--r--   0      501       20      306 2023-06-26 18:37:01.000000 getdaft-0.1.7/.gitignore
--rw-r--r--   0      501       20     2226 2023-06-26 18:37:01.000000 getdaft-0.1.7/.pre-commit-config.yaml
--rw-r--r--   0      501       20      205 2023-06-26 18:37:01.000000 getdaft-0.1.7/.readthedocs.yaml
--rw-r--r--   0      501       20     1550 2023-06-26 18:37:01.000000 getdaft-0.1.7/CONTRIBUTING.md
--rw-r--r--   0      501       20    11357 2023-06-26 18:37:01.000000 getdaft-0.1.7/LICENSE
--rw-r--r--   0      501       20     1295 2023-06-26 18:37:01.000000 getdaft-0.1.7/Makefile
--rw-r--r--   0      501       20     9185 2023-06-26 18:37:01.000000 getdaft-0.1.7/README.rst
--rw-r--r--   0      501       20        0 2023-06-26 18:37:01.000000 getdaft-0.1.7/benchmarking/__init__.py
--rw-r--r--   0      501       20        0 2023-06-26 18:37:01.000000 getdaft-0.1.7/benchmarking/tpch/__init__.py
--rw-r--r--   0      501       20     9495 2023-06-26 18:37:01.000000 getdaft-0.1.7/benchmarking/tpch/__main__.py
--rw-r--r--   0      501       20    12428 2023-06-26 18:37:01.000000 getdaft-0.1.7/benchmarking/tpch/answers.py
--rw-r--r--   0      501       20    12336 2023-06-26 18:37:01.000000 getdaft-0.1.7/benchmarking/tpch/data_generation.py
--rw-r--r--   0      501       20     4573 2023-06-26 18:37:01.000000 getdaft-0.1.7/benchmarking/tpch/pipelined_data_generation.py
--rw-r--r--   0      501       20     2654 2023-06-26 18:37:01.000000 getdaft-0.1.7/benchmarking/tpch/subprefix_s3_files.py
--rw-r--r--   0      501       20     1436 2023-06-26 18:37:01.000000 getdaft-0.1.7/ci/upload_wheels.sh
--rw-r--r--   0      501       20      446 2023-06-26 18:37:01.000000 getdaft-0.1.7/codecov.yml
--rw-r--r--   0      501       20     2199 2023-06-26 18:37:01.000000 getdaft-0.1.7/daft/__init__.py
--rw-r--r--   0      501       20     6724 2023-06-26 18:37:01.000000 getdaft-0.1.7/daft/analytics.py
--rw-r--r--   0      501       20     3935 2023-06-26 18:37:01.000000 getdaft-0.1.7/daft/api_annotations.py
--rw-r--r--   0      501       20    10591 2023-06-26 18:37:01.000000 getdaft-0.1.7/daft/arrow_utils.py
--rw-r--r--   0      501       20     5511 2023-06-26 18:37:01.000000 getdaft-0.1.7/daft/context.py
--rw-r--r--   0      501       20     3412 2023-06-26 18:37:01.000000 getdaft-0.1.7/daft/convert.py
--rw-r--r--   0      501       20     1298 2023-06-26 18:37:01.000000 getdaft-0.1.7/daft/daft.pyi
--rw-r--r--   0      501       20       94 2023-06-26 18:37:01.000000 getdaft-0.1.7/daft/dataframe/__init__.py
--rw-r--r--   0      501       20    54827 2023-06-26 18:37:01.000000 getdaft-0.1.7/daft/dataframe/dataframe.py
--rw-r--r--   0      501       20      306 2023-06-26 18:37:01.000000 getdaft-0.1.7/daft/dataframe/preview.py
--rw-r--r--   0      501       20     1404 2023-06-26 18:37:01.000000 getdaft-0.1.7/daft/dataframe/to_torch.py
--rw-r--r--   0      501       20      850 2023-06-26 18:37:01.000000 getdaft-0.1.7/daft/datasources.py
--rw-r--r--   0      501       20    17515 2023-06-26 18:37:01.000000 getdaft-0.1.7/daft/datatype.py
--rw-r--r--   0      501       20       84 2023-06-26 18:37:01.000000 getdaft-0.1.7/daft/errors.py
--rw-r--r--   0      501       20        0 2023-06-26 18:37:01.000000 getdaft-0.1.7/daft/execution/__init__.py
--rw-r--r--   0      501       20    28993 2023-06-26 18:37:01.000000 getdaft-0.1.7/daft/execution/execution_step.py
--rw-r--r--   0      501       20    28946 2023-06-26 18:37:01.000000 getdaft-0.1.7/daft/execution/physical_plan.py
--rw-r--r--   0      501       20     6350 2023-06-26 18:37:01.000000 getdaft-0.1.7/daft/execution/physical_plan_factory.py
--rw-r--r--   0      501       20      170 2023-06-26 18:37:01.000000 getdaft-0.1.7/daft/expressions/__init__.py
--rw-r--r--   0      501       20    28908 2023-06-26 18:37:01.000000 getdaft-0.1.7/daft/expressions/expressions.py
--rw-r--r--   0      501       20      572 2023-06-26 18:37:01.000000 getdaft-0.1.7/daft/expressions/testing.py
--rw-r--r--   0      501       20    12728 2023-06-26 18:37:01.000000 getdaft-0.1.7/daft/filesystem.py
--rw-r--r--   0      501       20        0 2023-06-26 18:37:01.000000 getdaft-0.1.7/daft/internal/__init__.py
--rw-r--r--   0      501       20      509 2023-06-26 18:37:01.000000 getdaft-0.1.7/daft/internal/gpu.py
--rw-r--r--   0      501       20     1804 2023-06-26 18:37:01.000000 getdaft-0.1.7/daft/internal/rule.py
--rw-r--r--   0      501       20     2030 2023-06-26 18:37:01.000000 getdaft-0.1.7/daft/internal/rule_runner.py
--rw-r--r--   0      501       20     3490 2023-06-26 18:37:01.000000 getdaft-0.1.7/daft/internal/treenode.py
--rw-r--r--   0      501       20      377 2023-06-26 18:37:01.000000 getdaft-0.1.7/daft/io/__init__.py
--rw-r--r--   0      501       20     2292 2023-06-26 18:37:01.000000 getdaft-0.1.7/daft/io/_csv.py
--rw-r--r--   0      501       20     1470 2023-06-26 18:37:01.000000 getdaft-0.1.7/daft/io/_json.py
--rw-r--r--   0      501       20     2243 2023-06-26 18:37:01.000000 getdaft-0.1.7/daft/io/common.py
--rw-r--r--   0      501       20     2034 2023-06-26 18:37:01.000000 getdaft-0.1.7/daft/io/file_path.py
--rw-r--r--   0      501       20     1490 2023-06-26 18:37:01.000000 getdaft-0.1.7/daft/io/parquet.py
--rw-r--r--   0      501       20      264 2023-06-26 18:37:01.000000 getdaft-0.1.7/daft/logging.py
--rw-r--r--   0      501       20        0 2023-06-26 18:37:01.000000 getdaft-0.1.7/daft/logical/__init__.py
--rw-r--r--   0      501       20     8601 2023-06-26 18:37:01.000000 getdaft-0.1.7/daft/logical/aggregation_plan_builder.py
--rw-r--r--   0      501       20    38976 2023-06-26 18:37:01.000000 getdaft-0.1.7/daft/logical/logical_plan.py
--rw-r--r--   0      501       20     1492 2023-06-26 18:37:01.000000 getdaft-0.1.7/daft/logical/map_partition_ops.py
--rw-r--r--   0      501       20    19757 2023-06-26 18:37:01.000000 getdaft-0.1.7/daft/logical/optimizer.py
--rw-r--r--   0      501       20     3868 2023-06-26 18:37:01.000000 getdaft-0.1.7/daft/logical/schema.py
--rw-r--r--   0      501       20       99 2023-06-26 18:37:01.000000 getdaft-0.1.7/daft/pickle/__init__.py
--rw-r--r--   0      501       20    34760 2023-06-26 18:37:01.000000 getdaft-0.1.7/daft/pickle/cloudpickle.py
--rw-r--r--   0      501       20    34262 2023-06-26 18:37:01.000000 getdaft-0.1.7/daft/pickle/cloudpickle_fast.py
--rw-r--r--   0      501       20      639 2023-06-26 18:37:01.000000 getdaft-0.1.7/daft/pickle/compat.py
--rw-r--r--   0      501       20      312 2023-06-26 18:37:01.000000 getdaft-0.1.7/daft/pickle/pickle.py
--rw-r--r--   0      501       20        0 2023-06-26 18:37:01.000000 getdaft-0.1.7/daft/py.typed
--rw-r--r--   0      501       20     2036 2023-06-26 18:37:01.000000 getdaft-0.1.7/daft/resource_request.py
--rw-r--r--   0      501       20        0 2023-06-26 18:37:01.000000 getdaft-0.1.7/daft/runners/__init__.py
--rw-r--r--   0      501       20     4676 2023-06-26 18:37:01.000000 getdaft-0.1.7/daft/runners/partitioning.py
--rw-r--r--   0      501       20     1488 2023-06-26 18:37:01.000000 getdaft-0.1.7/daft/runners/profiler.py
--rw-r--r--   0      501       20    13637 2023-06-26 18:37:01.000000 getdaft-0.1.7/daft/runners/pyrunner.py
--rw-r--r--   0      501       20    27945 2023-06-26 18:37:01.000000 getdaft-0.1.7/daft/runners/ray_runner.py
--rw-r--r--   0      501       20     1428 2023-06-26 18:37:01.000000 getdaft-0.1.7/daft/runners/runner.py
--rw-r--r--   0      501       20     3338 2023-06-26 18:37:01.000000 getdaft-0.1.7/daft/runners/runner_io.py
--rw-r--r--   0      501       20    22246 2023-06-26 18:37:01.000000 getdaft-0.1.7/daft/series.py
--rw-r--r--   0      501       20       82 2023-06-26 18:37:01.000000 getdaft-0.1.7/daft/table/__init__.py
--rw-r--r--   0      501       20     2960 2023-06-26 18:37:01.000000 getdaft-0.1.7/daft/table/schema_inference.py
--rw-r--r--   0      501       20    14029 2023-06-26 18:37:01.000000 getdaft-0.1.7/daft/table/table.py
--rw-r--r--   0      501       20     9916 2023-06-26 18:37:01.000000 getdaft-0.1.7/daft/table/table_io.py
--rw-r--r--   0      501       20     7370 2023-06-26 18:37:01.000000 getdaft-0.1.7/daft/udf.py
--rw-r--r--   0      501       20        0 2023-06-26 18:37:01.000000 getdaft-0.1.7/daft/udf_library/__init__.py
--rw-r--r--   0      501       20     3486 2023-06-26 18:37:01.000000 getdaft-0.1.7/daft/udf_library/url_udfs.py
--rw-r--r--   0      501       20     2796 2023-06-26 18:37:01.000000 getdaft-0.1.7/daft/utils.py
--rw-r--r--   0      501       20      183 2023-06-26 18:37:01.000000 getdaft-0.1.7/daft/viz/__init__.py
--rw-r--r--   0      501       20     1929 2023-06-26 18:37:01.000000 getdaft-0.1.7/daft/viz/dataframe_display.py
--rw-r--r--   0      501       20     1522 2023-06-26 18:37:01.000000 getdaft-0.1.7/daft/viz/html_viz_hooks.py
--rw-r--r--   0      501       20      148 2023-06-26 18:37:01.000000 getdaft-0.1.7/docs/CONTRIBUTING.md
--rw-r--r--   0      501       20      638 2023-06-26 18:37:01.000000 getdaft-0.1.7/docs/Makefile
--rw-r--r--   0      501       20    73229 2023-06-26 18:37:01.000000 getdaft-0.1.7/docs/source/10-min.ipynb
--rw-r--r--   0      501       20      389 2023-06-26 18:37:01.000000 getdaft-0.1.7/docs/source/_static/custom-function-signatures.css
--rw-r--r--   0      501       20      565 2023-06-26 18:37:01.000000 getdaft-0.1.7/docs/source/_static/daft-favicon.png
--rw-r--r--   0      501       20     7804 2023-06-26 18:37:01.000000 getdaft-0.1.7/docs/source/_static/daft-logo.png
--rw-r--r--   0      501       20    42148 2023-06-26 18:37:01.000000 getdaft-0.1.7/docs/source/_static/daft_illustration.png
--rw-r--r--   0      501       20      583 2023-06-26 18:37:01.000000 getdaft-0.1.7/docs/source/_static/dataframe-comp-table.csv
--rw-r--r--   0      501       20    25200 2023-06-26 18:37:01.000000 getdaft-0.1.7/docs/source/_static/execution_model.png
--rw-r--r--   0      501       20     1901 2023-06-26 18:37:01.000000 getdaft-0.1.7/docs/source/_static/header.css
--rw-r--r--   0      501       20    32864 2023-06-26 18:37:01.000000 getdaft-0.1.7/docs/source/_static/high_level_architecture.png
--rw-r--r--   0      501       20      343 2023-06-26 18:37:01.000000 getdaft-0.1.7/docs/source/_static/icon-menu-close.svg
--rw-r--r--   0      501       20      333 2023-06-26 18:37:01.000000 getdaft-0.1.7/docs/source/_static/icon-menu-dots.svg
--rw-r--r--   0      501       20    18177 2023-06-26 18:37:01.000000 getdaft-0.1.7/docs/source/_static/in_memory_data_representation.png
--rw-r--r--   0      501       20      786 2023-06-26 18:37:01.000000 getdaft-0.1.7/docs/source/_static/mobile-menu.js
--rw-r--r--   0      501       20     9142 2023-06-26 18:37:01.000000 getdaft-0.1.7/docs/source/_static/tpch-1000sf.html
--rw-r--r--   0      501       20     9647 2023-06-26 18:37:01.000000 getdaft-0.1.7/docs/source/_static/tpch-100sf.html
--rw-r--r--   0      501       20     8757 2023-06-26 18:37:01.000000 getdaft-0.1.7/docs/source/_static/tpch-nodes-count-daft-1000-sf.html
--rw-r--r--   0      501       20      856 2023-06-26 18:37:01.000000 getdaft-0.1.7/docs/source/_templates/layout.html
--rw-r--r--   0      501       20     1179 2023-06-26 18:37:01.000000 getdaft-0.1.7/docs/source/_templates/sections/header.html
--rw-r--r--   0      501       20     1129 2023-06-26 18:37:01.000000 getdaft-0.1.7/docs/source/_templates/sections/mobile-menu.html
--rw-r--r--   0      501       20      333 2023-06-26 18:37:01.000000 getdaft-0.1.7/docs/source/api_docs/context.rst
--rw-r--r--   0      501       20     2759 2023-06-26 18:37:01.000000 getdaft-0.1.7/docs/source/api_docs/dataframe.rst
--rw-r--r--   0      501       20     2293 2023-06-26 18:37:01.000000 getdaft-0.1.7/docs/source/api_docs/datatype.rst
--rw-r--r--   0      501       20      139 2023-06-26 18:37:01.000000 getdaft-0.1.7/docs/source/api_docs/datatype_image_mode/daft.ImageMode.from_mode_string.rst
--rw-r--r--   0      501       20      430 2023-06-26 18:37:01.000000 getdaft-0.1.7/docs/source/api_docs/datatype_image_mode/daft.ImageMode.rst
--rw-r--r--   0      501       20      151 2023-06-26 18:37:01.000000 getdaft-0.1.7/docs/source/api_docs/datetype_image_format/daft.ImageFormat.from_format_string.rst
--rw-r--r--   0      501       20      333 2023-06-26 18:37:01.000000 getdaft-0.1.7/docs/source/api_docs/datetype_image_format/daft.ImageFormat.rst
--rw-r--r--   0      501       20     4727 2023-06-26 18:37:01.000000 getdaft-0.1.7/docs/source/api_docs/expressions.rst
--rw-r--r--   0      501       20      816 2023-06-26 18:37:01.000000 getdaft-0.1.7/docs/source/api_docs/groupby.rst
--rw-r--r--   0      501       20      146 2023-06-26 18:37:01.000000 getdaft-0.1.7/docs/source/api_docs/index.rst
--rw-r--r--   0      501       20     1537 2023-06-26 18:37:01.000000 getdaft-0.1.7/docs/source/api_docs/input_output.rst
--rw-r--r--   0      501       20      273 2023-06-26 18:37:01.000000 getdaft-0.1.7/docs/source/api_docs/series/daft.Series.rst
--rw-r--r--   0      501       20      492 2023-06-26 18:37:01.000000 getdaft-0.1.7/docs/source/api_docs/series.rst
--rw-r--r--   0      501       20       88 2023-06-26 18:37:01.000000 getdaft-0.1.7/docs/source/api_docs/udf.rst
--rw-r--r--   0      501       20    14528 2023-06-26 18:37:01.000000 getdaft-0.1.7/docs/source/benchmarks/index.rst
--rw-r--r--   0      501       20     4200 2023-06-26 18:37:01.000000 getdaft-0.1.7/docs/source/conf.py
--rw-r--r--   0      501       20     5114 2023-06-26 18:37:01.000000 getdaft-0.1.7/docs/source/dataframe_comparison.rst
--rw-r--r--   0      501       20     1723 2023-06-26 18:37:01.000000 getdaft-0.1.7/docs/source/index.rst
--rw-r--r--   0      501       20     1356 2023-06-26 18:37:01.000000 getdaft-0.1.7/docs/source/install.rst
--rw-r--r--   0      501       20      896 2023-06-26 18:37:01.000000 getdaft-0.1.7/docs/source/learn/index.rst
--rw-r--r--   0      501       20     7830 2023-06-26 18:37:01.000000 getdaft-0.1.7/docs/source/learn/key_concepts.rst
--rw-r--r--   0      501       20     1783 2023-06-26 18:37:01.000000 getdaft-0.1.7/docs/source/learn/tutorials.rst
--rw-r--r--   0      501       20     1388 2023-06-26 18:37:01.000000 getdaft-0.1.7/docs/source/learn/user_guides/aggregations.rst
--rw-r--r--   0      501       20     7009 2023-06-26 18:37:01.000000 getdaft-0.1.7/docs/source/learn/user_guides/dataframe-operations.rst
--rw-r--r--   0      501       20     5166 2023-06-26 18:37:01.000000 getdaft-0.1.7/docs/source/learn/user_guides/datatypes.rst
--rw-r--r--   0      501       20     9481 2023-06-26 18:37:01.000000 getdaft-0.1.7/docs/source/learn/user_guides/expressions.rst
--rw-r--r--   0      501       20     8241 2023-06-26 18:37:01.000000 getdaft-0.1.7/docs/source/learn/user_guides/intro-dataframes.rst
--rw-r--r--   0      501       20      206 2023-06-26 18:37:01.000000 getdaft-0.1.7/docs/source/learn/user_guides/partitioning.rst
--rw-r--r--   0      501       20     3251 2023-06-26 18:37:01.000000 getdaft-0.1.7/docs/source/learn/user_guides/read-write.rst
--rw-r--r--   0      501       20     1257 2023-06-26 18:37:01.000000 getdaft-0.1.7/docs/source/learn/user_guides/scaling-up.rst
--rw-r--r--   0      501       20     8853 2023-06-26 18:37:01.000000 getdaft-0.1.7/docs/source/learn/user_guides/udf.rst
--rw-r--r--   0      501       20     1577 2023-06-26 18:37:01.000000 getdaft-0.1.7/docs/source/learn/user_guides.rst
--rw-r--r--   0      501       20     6628 2023-06-26 18:37:01.000000 getdaft-0.1.7/docs/source/technical_architecture.rst
--rw-r--r--   0      501       20     1316 2023-06-26 18:37:01.000000 getdaft-0.1.7/docs/source/telemetry.rst
--rw-r--r--   0      501       20     1850 2023-06-26 18:37:01.000000 getdaft-0.1.7/pyproject.toml
--rw-r--r--   0      501       20      868 2023-06-26 18:37:01.000000 getdaft-0.1.7/requirements-dev.txt
--rw-r--r--   0      501       20       98 2023-06-26 18:37:01.000000 getdaft-0.1.7/rust-toolchain.toml
--rw-r--r--   0      501       20      687 2023-06-26 18:37:01.000000 getdaft-0.1.7/src/lib.rs
--rw-r--r--   0      501       20        0 2023-06-26 18:37:01.000000 getdaft-0.1.7/tests/__init__.py
--rw-r--r--   0      501       20      299 2023-06-26 18:37:01.000000 getdaft-0.1.7/tests/assets/__init__.py
--rw-r--r--   0      501       20      544 2023-06-26 18:37:01.000000 getdaft-0.1.7/tests/assets/tpch-sqlite-queries/1.sql
--rw-r--r--   0      501       20      542 2023-06-26 18:37:01.000000 getdaft-0.1.7/tests/assets/tpch-sqlite-queries/10.sql
--rw-r--r--   0      501       20      703 2023-06-26 18:37:01.000000 getdaft-0.1.7/tests/assets/tpch-sqlite-queries/2.sql
--rw-r--r--   0      501       20      444 2023-06-26 18:37:01.000000 getdaft-0.1.7/tests/assets/tpch-sqlite-queries/3.sql
--rw-r--r--   0      501       20      371 2023-06-26 18:37:01.000000 getdaft-0.1.7/tests/assets/tpch-sqlite-queries/4.sql
--rw-r--r--   0      501       20      504 2023-06-26 18:37:01.000000 getdaft-0.1.7/tests/assets/tpch-sqlite-queries/5.sql
--rw-r--r--   0      501       20      259 2023-06-26 18:37:01.000000 getdaft-0.1.7/tests/assets/tpch-sqlite-queries/6.sql
--rw-r--r--   0      501       20      834 2023-06-26 18:37:01.000000 getdaft-0.1.7/tests/assets/tpch-sqlite-queries/7.sql
--rw-r--r--   0      501       20      815 2023-06-26 18:37:01.000000 getdaft-0.1.7/tests/assets/tpch-sqlite-queries/8.sql
--rw-r--r--   0      501       20      627 2023-06-26 18:37:01.000000 getdaft-0.1.7/tests/assets/tpch-sqlite-queries/9.sql
--rw-r--r--   0      501       20       48 2023-06-26 18:37:01.000000 getdaft-0.1.7/tests/assets/tpch-sqlite-queries/README.md
--rw-r--r--   0      501       20      604 2023-06-26 18:37:01.000000 getdaft-0.1.7/tests/benchmarks/conftest.py
--rw-r--r--   0      501       20     1227 2023-06-26 18:37:01.000000 getdaft-0.1.7/tests/benchmarks/test_df_arithmetic.py
--rw-r--r--   0      501       20     2706 2023-06-26 18:37:01.000000 getdaft-0.1.7/tests/benchmarks/test_file_read.py
--rw-r--r--   0      501       20     5604 2023-06-26 18:37:01.000000 getdaft-0.1.7/tests/benchmarks/test_groups_and_aggs.py
--rw-r--r--   0      501       20     7292 2023-06-26 18:37:01.000000 getdaft-0.1.7/tests/benchmarks/test_join.py
--rw-r--r--   0      501       20     2603 2023-06-26 18:37:01.000000 getdaft-0.1.7/tests/benchmarks/test_repartition.py
--rw-r--r--   0      501       20     4005 2023-06-26 18:37:01.000000 getdaft-0.1.7/tests/benchmarks/test_sort.py
--rw-r--r--   0      501       20     2911 2023-06-26 18:37:01.000000 getdaft-0.1.7/tests/conftest.py
--rw-r--r--   0      501       20        0 2023-06-26 18:37:01.000000 getdaft-0.1.7/tests/cookbook/__init__.py
--rw-r--r--   0      501       20    13229 2023-06-26 18:37:01.000000 getdaft-0.1.7/tests/cookbook/assets/311-service-requests.24.csv
--rw-r--r--   0      501       20      255 2023-06-26 18:37:01.000000 getdaft-0.1.7/tests/cookbook/assets/__init__.py
--rw-r--r--   0      501       20      924 2023-06-26 18:37:01.000000 getdaft-0.1.7/tests/cookbook/assets/images/0000.jpg
--rw-r--r--   0      501       20      941 2023-06-26 18:37:01.000000 getdaft-0.1.7/tests/cookbook/assets/images/0007.jpg
--rw-r--r--   0      501       20     2740 2023-06-26 18:37:01.000000 getdaft-0.1.7/tests/cookbook/assets/images/0018.png
--rw-r--r--   0      501       20     7462 2023-06-26 18:37:01.000000 getdaft-0.1.7/tests/cookbook/assets/images/0025.tiff
--rw-r--r--   0      501       20      882 2023-06-26 18:37:01.000000 getdaft-0.1.7/tests/cookbook/conftest.py
--rw-r--r--   0      501       20     9268 2023-06-26 18:37:01.000000 getdaft-0.1.7/tests/cookbook/test_aggregations.py
--rw-r--r--   0      501       20     2979 2023-06-26 18:37:01.000000 getdaft-0.1.7/tests/cookbook/test_computations.py
--rw-r--r--   0      501       20     1798 2023-06-26 18:37:01.000000 getdaft-0.1.7/tests/cookbook/test_count_rows.py
--rw-r--r--   0      501       20     7099 2023-06-26 18:37:01.000000 getdaft-0.1.7/tests/cookbook/test_dataloading.py
--rw-r--r--   0      501       20      800 2023-06-26 18:37:01.000000 getdaft-0.1.7/tests/cookbook/test_distinct.py
--rw-r--r--   0      501       20     6049 2023-06-26 18:37:01.000000 getdaft-0.1.7/tests/cookbook/test_filter.py
--rw-r--r--   0      501       20     2930 2023-06-26 18:37:01.000000 getdaft-0.1.7/tests/cookbook/test_image.py
--rw-r--r--   0      501       20     3810 2023-06-26 18:37:01.000000 getdaft-0.1.7/tests/cookbook/test_joins.py
--rw-r--r--   0      501       20     2878 2023-06-26 18:37:01.000000 getdaft-0.1.7/tests/cookbook/test_literals.py
--rw-r--r--   0      501       20    10311 2023-06-26 18:37:01.000000 getdaft-0.1.7/tests/cookbook/test_pandas_cookbook.py
--rw-r--r--   0      501       20     4148 2023-06-26 18:37:01.000000 getdaft-0.1.7/tests/cookbook/test_sorting.py
--rw-r--r--   0      501       20     1497 2023-06-26 18:37:01.000000 getdaft-0.1.7/tests/cookbook/test_write.py
--rw-r--r--   0      501       20        0 2023-06-26 18:37:01.000000 getdaft-0.1.7/tests/dataframe/__init__.py
--rw-r--r--   0      501       20      751 2023-06-26 18:37:01.000000 getdaft-0.1.7/tests/dataframe/conftest.py
--rw-r--r--   0      501       20      805 2023-06-26 18:37:01.000000 getdaft-0.1.7/tests/dataframe/test_accessors.py
--rw-r--r--   0      501       20    10308 2023-06-26 18:37:01.000000 getdaft-0.1.7/tests/dataframe/test_aggregations.py
--rw-r--r--   0      501       20      472 2023-06-26 18:37:01.000000 getdaft-0.1.7/tests/dataframe/test_concat.py
--rw-r--r--   0      501       20    24585 2023-06-26 18:37:01.000000 getdaft-0.1.7/tests/dataframe/test_creation.py
--rw-r--r--   0      501       20     1824 2023-06-26 18:37:01.000000 getdaft-0.1.7/tests/dataframe/test_distinct.py
--rw-r--r--   0      501       20     1428 2023-06-26 18:37:01.000000 getdaft-0.1.7/tests/dataframe/test_explode.py
--rw-r--r--   0      501       20     1097 2023-06-26 18:37:01.000000 getdaft-0.1.7/tests/dataframe/test_filter.py
--rw-r--r--   0      501       20     2435 2023-06-26 18:37:01.000000 getdaft-0.1.7/tests/dataframe/test_getitem.py
--rw-r--r--   0      501       20     3205 2023-06-26 18:37:01.000000 getdaft-0.1.7/tests/dataframe/test_iter.py
--rw-r--r--   0      501       20     4091 2023-06-26 18:37:01.000000 getdaft-0.1.7/tests/dataframe/test_joins.py
--rw-r--r--   0      501       20     2253 2023-06-26 18:37:01.000000 getdaft-0.1.7/tests/dataframe/test_logical_type.py
--rw-r--r--   0      501       20      223 2023-06-26 18:37:01.000000 getdaft-0.1.7/tests/dataframe/test_repartition.py
--rw-r--r--   0      501       20     7880 2023-06-26 18:37:01.000000 getdaft-0.1.7/tests/dataframe/test_repr.py
--rw-r--r--   0      501       20      815 2023-06-26 18:37:01.000000 getdaft-0.1.7/tests/dataframe/test_select.py
--rw-r--r--   0      501       20      656 2023-06-26 18:37:01.000000 getdaft-0.1.7/tests/dataframe/test_show.py
--rw-r--r--   0      501       20     6364 2023-06-26 18:37:01.000000 getdaft-0.1.7/tests/dataframe/test_sort.py
--rw-r--r--   0      501       20     5210 2023-06-26 18:37:01.000000 getdaft-0.1.7/tests/dataframe/test_temporals.py
--rw-r--r--   0      501       20     2385 2023-06-26 18:37:01.000000 getdaft-0.1.7/tests/dataframe/test_to_integrations.py
--rw-r--r--   0      501       20      850 2023-06-26 18:37:01.000000 getdaft-0.1.7/tests/dataframe/test_with_column.py
--rw-r--r--   0      501       20        0 2023-06-26 18:37:01.000000 getdaft-0.1.7/tests/expressions/__init__.py
--rw-r--r--   0      501       20     1417 2023-06-26 18:37:01.000000 getdaft-0.1.7/tests/expressions/test_apply.py
--rw-r--r--   0      501       20     3533 2023-06-26 18:37:01.000000 getdaft-0.1.7/tests/expressions/test_expressions.py
--rw-r--r--   0      501       20     4259 2023-06-26 18:37:01.000000 getdaft-0.1.7/tests/expressions/test_expressions_projection.py
--rw-r--r--   0      501       20     5019 2023-06-26 18:37:01.000000 getdaft-0.1.7/tests/expressions/test_udf.py
--rw-r--r--   0      501       20        0 2023-06-26 18:37:01.000000 getdaft-0.1.7/tests/expressions/typing/__init__.py
--rw-r--r--   0      501       20     6290 2023-06-26 18:37:01.000000 getdaft-0.1.7/tests/expressions/typing/conftest.py
--rw-r--r--   0      501       20     1363 2023-06-26 18:37:01.000000 getdaft-0.1.7/tests/expressions/typing/test_aggs.py
--rw-r--r--   0      501       20     2335 2023-06-26 18:37:01.000000 getdaft-0.1.7/tests/expressions/typing/test_arithmetic.py
--rw-r--r--   0      501       20      853 2023-06-26 18:37:01.000000 getdaft-0.1.7/tests/expressions/typing/test_compare.py
--rw-r--r--   0      501       20      792 2023-06-26 18:37:01.000000 getdaft-0.1.7/tests/expressions/typing/test_dt.py
--rw-r--r--   0      501       20      531 2023-06-26 18:37:01.000000 getdaft-0.1.7/tests/expressions/typing/test_float.py
--rw-r--r--   0      501       20      684 2023-06-26 18:37:01.000000 getdaft-0.1.7/tests/expressions/typing/test_if_else.py
--rw-r--r--   0      501       20      422 2023-06-26 18:37:01.000000 getdaft-0.1.7/tests/expressions/typing/test_is_null.py
--rw-r--r--   0      501       20     1176 2023-06-26 18:37:01.000000 getdaft-0.1.7/tests/expressions/typing/test_logical.py
--rw-r--r--   0      501       20     1544 2023-06-26 18:37:01.000000 getdaft-0.1.7/tests/expressions/typing/test_str.py
--rw-r--r--   0      501       20        0 2023-06-26 18:37:01.000000 getdaft-0.1.7/tests/integration/__init__.py
--rw-r--r--   0      501       20     4343 2023-06-26 18:37:01.000000 getdaft-0.1.7/tests/integration/test_tpch.py
--rw-r--r--   0      501       20        0 2023-06-26 18:37:01.000000 getdaft-0.1.7/tests/optimizer/__init__.py
--rw-r--r--   0      501       20     1116 2023-06-26 18:37:01.000000 getdaft-0.1.7/tests/optimizer/conftest.py
--rw-r--r--   0      501       20     1666 2023-06-26 18:37:01.000000 getdaft-0.1.7/tests/optimizer/test_drop_projections.py
--rw-r--r--   0      501       20     1847 2023-06-26 18:37:01.000000 getdaft-0.1.7/tests/optimizer/test_drop_repartition.py
--rw-r--r--   0      501       20     2463 2023-06-26 18:37:01.000000 getdaft-0.1.7/tests/optimizer/test_fold_projections.py
--rw-r--r--   0      501       20     8050 2023-06-26 18:37:01.000000 getdaft-0.1.7/tests/optimizer/test_prune_columns.py
--rw-r--r--   0      501       20     3597 2023-06-26 18:37:01.000000 getdaft-0.1.7/tests/optimizer/test_pushdown_clauses_into_scan.py
--rw-r--r--   0      501       20     1170 2023-06-26 18:37:01.000000 getdaft-0.1.7/tests/optimizer/test_pushdown_limit.py
--rw-r--r--   0      501       20     8981 2023-06-26 18:37:01.000000 getdaft-0.1.7/tests/optimizer/test_pushdown_predicates.py
--rw-r--r--   0      501       20        0 2023-06-26 18:37:01.000000 getdaft-0.1.7/tests/property_based_testing/__init__.py
--rw-r--r--   0      501       20     4575 2023-06-26 18:37:01.000000 getdaft-0.1.7/tests/property_based_testing/strategies.py
--rw-r--r--   0      501       20     8895 2023-06-26 18:37:01.000000 getdaft-0.1.7/tests/property_based_testing/test_sort.py
--rw-r--r--   0      501       20        0 2023-06-26 18:37:01.000000 getdaft-0.1.7/tests/ray/__init__.py
--rw-r--r--   0      501       20     5375 2023-06-26 18:37:01.000000 getdaft-0.1.7/tests/ray/test_dask.py
--rw-r--r--   0      501       20     8864 2023-06-26 18:37:01.000000 getdaft-0.1.7/tests/ray/test_datasets.py
--rw-r--r--   0      501       20      278 2023-06-26 18:37:01.000000 getdaft-0.1.7/tests/series/__init__.py
--rw-r--r--   0      501       20     9299 2023-06-26 18:37:01.000000 getdaft-0.1.7/tests/series/test_arithmetic.py
--rw-r--r--   0      501       20    15034 2023-06-26 18:37:01.000000 getdaft-0.1.7/tests/series/test_cast.py
--rw-r--r--   0      501       20    17207 2023-06-26 18:37:01.000000 getdaft-0.1.7/tests/series/test_comparisons.py
--rw-r--r--   0      501       20     7188 2023-06-26 18:37:01.000000 getdaft-0.1.7/tests/series/test_concat.py
--rw-r--r--   0      501       20      896 2023-06-26 18:37:01.000000 getdaft-0.1.7/tests/series/test_embedding.py
--rw-r--r--   0      501       20     6151 2023-06-26 18:37:01.000000 getdaft-0.1.7/tests/series/test_filter.py
--rw-r--r--   0      501       20      874 2023-06-26 18:37:01.000000 getdaft-0.1.7/tests/series/test_float.py
--rw-r--r--   0      501       20     3344 2023-06-26 18:37:01.000000 getdaft-0.1.7/tests/series/test_hash.py
--rw-r--r--   0      501       20    21522 2023-06-26 18:37:01.000000 getdaft-0.1.7/tests/series/test_if_else.py
--rw-r--r--   0      501       20    22626 2023-06-26 18:37:01.000000 getdaft-0.1.7/tests/series/test_image.py
--rw-r--r--   0      501       20      889 2023-06-26 18:37:01.000000 getdaft-0.1.7/tests/series/test_numeric_ops.py
--rw-r--r--   0      501       20     3418 2023-06-26 18:37:01.000000 getdaft-0.1.7/tests/series/test_series.py
--rw-r--r--   0      501       20     9173 2023-06-26 18:37:01.000000 getdaft-0.1.7/tests/series/test_size_bytes.py
--rw-r--r--   0      501       20     2188 2023-06-26 18:37:01.000000 getdaft-0.1.7/tests/series/test_slice.py
--rw-r--r--   0      501       20     5495 2023-06-26 18:37:01.000000 getdaft-0.1.7/tests/series/test_sort.py
--rw-r--r--   0      501       20     6111 2023-06-26 18:37:01.000000 getdaft-0.1.7/tests/series/test_take.py
--rw-r--r--   0      501       20     1934 2023-06-26 18:37:01.000000 getdaft-0.1.7/tests/series/test_temporal_ops.py
--rw-r--r--   0      501       20     4413 2023-06-26 18:37:01.000000 getdaft-0.1.7/tests/series/test_utf8_ops.py
--rw-r--r--   0      501       20      694 2023-06-26 18:37:01.000000 getdaft-0.1.7/tests/table/__init__.py
--rw-r--r--   0      501       20        0 2023-06-26 18:37:01.000000 getdaft-0.1.7/tests/table/list/__init__.py
--rw-r--r--   0      501       20     1156 2023-06-26 18:37:01.000000 getdaft-0.1.7/tests/table/list/test_list_join.py
--rw-r--r--   0      501       20        0 2023-06-26 18:37:01.000000 getdaft-0.1.7/tests/table/table_io/__init__.py
--rw-r--r--   0      501       20     6289 2023-06-26 18:37:01.000000 getdaft-0.1.7/tests/table/table_io/test_csv.py
--rw-r--r--   0      501       20     4355 2023-06-26 18:37:01.000000 getdaft-0.1.7/tests/table/table_io/test_json.py
--rw-r--r--   0      501       20     4778 2023-06-26 18:37:01.000000 getdaft-0.1.7/tests/table/table_io/test_parquet.py
--rw-r--r--   0      501       20     2100 2023-06-26 18:37:01.000000 getdaft-0.1.7/tests/table/table_io/test_read_time_cast.py
--rw-r--r--   0      501       20     1070 2023-06-26 18:37:01.000000 getdaft-0.1.7/tests/table/test_blackbox_kernels.py
--rw-r--r--   0      501       20      426 2023-06-26 18:37:01.000000 getdaft-0.1.7/tests/table/test_broadcasts.py
--rw-r--r--   0      501       20     2123 2023-06-26 18:37:01.000000 getdaft-0.1.7/tests/table/test_concat.py
--rw-r--r--   0      501       20     4900 2023-06-26 18:37:01.000000 getdaft-0.1.7/tests/table/test_eval.py
--rw-r--r--   0      501       20     3930 2023-06-26 18:37:01.000000 getdaft-0.1.7/tests/table/test_explodes.py
--rw-r--r--   0      501       20     7413 2023-06-26 18:37:01.000000 getdaft-0.1.7/tests/table/test_filter.py
--rw-r--r--   0      501       20    23530 2023-06-26 18:37:01.000000 getdaft-0.1.7/tests/table/test_from_py.py
--rw-r--r--   0      501       20      842 2023-06-26 18:37:01.000000 getdaft-0.1.7/tests/table/test_head.py
--rw-r--r--   0      501       20    10974 2023-06-26 18:37:01.000000 getdaft-0.1.7/tests/table/test_joins.py
--rw-r--r--   0      501       20     7811 2023-06-26 18:37:01.000000 getdaft-0.1.7/tests/table/test_partitioning.py
--rw-r--r--   0      501       20      654 2023-06-26 18:37:01.000000 getdaft-0.1.7/tests/table/test_size_bytes.py
--rw-r--r--   0      501       20    10955 2023-06-26 18:37:01.000000 getdaft-0.1.7/tests/table/test_sorting.py
--rw-r--r--   0      501       20    20923 2023-06-26 18:37:01.000000 getdaft-0.1.7/tests/table/test_table_aggs.py
--rw-r--r--   0      501       20     5061 2023-06-26 18:37:01.000000 getdaft-0.1.7/tests/table/test_take.py
--rw-r--r--   0      501       20        0 2023-06-26 18:37:01.000000 getdaft-0.1.7/tests/table/utf8/__init__.py
--rw-r--r--   0      501       20     1165 2023-06-26 18:37:01.000000 getdaft-0.1.7/tests/table/utf8/test_compares.py
--rw-r--r--   0      501       20      321 2023-06-26 18:37:01.000000 getdaft-0.1.7/tests/table/utf8/test_length.py
--rw-r--r--   0      501       20     3533 2023-06-26 18:37:01.000000 getdaft-0.1.7/tests/test_analytics.py
--rw-r--r--   0      501       20      703 2023-06-26 18:37:01.000000 getdaft-0.1.7/tests/test_datatypes.py
--rw-r--r--   0      501       20     3653 2023-06-26 18:37:01.000000 getdaft-0.1.7/tests/test_schema.py
--rw-r--r--   0      501       20        0 2023-06-26 18:37:01.000000 getdaft-0.1.7/tests/udf_library/__init__.py
--rw-r--r--   0      501       20     4508 2023-06-26 18:37:01.000000 getdaft-0.1.7/tests/udf_library/test_url_udfs.py
--rw-r--r--   0      501       20      338 2023-06-26 18:37:01.000000 getdaft-0.1.7/tests/utils.py
--rw-r--r--   0      501       20        0 2023-06-26 18:37:01.000000 getdaft-0.1.7/tests_legacy/__init__.py
--rw-r--r--   0      501       20     6988 2023-06-26 18:37:01.000000 getdaft-0.1.7/tests_legacy/test_resource_requests.py
--rw-r--r--   0      501       20        0 2023-06-26 18:37:01.000000 getdaft-0.1.7/tools/__init__.py
--rw-r--r--   0      501       20     1633 2023-06-26 18:37:01.000000 getdaft-0.1.7/tools/patch_package_version.py
--rw-r--r--   0      501       20        0 2023-06-26 18:37:01.000000 getdaft-0.1.7/tools/wheels/__init__.py
--rw-r--r--   0      501       20        0 2023-06-26 18:37:01.000000 getdaft-0.1.7/tools/wheels/_vendor/__init__.py
--rw-r--r--   0      501       20     1125 2023-06-26 18:37:01.000000 getdaft-0.1.7/tools/wheels/_vendor/wheel/LICENSE.txt
--rw-r--r--   0      501       20       59 2023-06-26 18:37:01.000000 getdaft-0.1.7/tools/wheels/_vendor/wheel/__init__.py
--rw-r--r--   0      501       20     2499 2023-06-26 18:37:01.000000 getdaft-0.1.7/tools/wheels/_vendor/wheel/cli/__init__.py
--rw-r--r--   0      501       20     9514 2023-06-26 18:37:01.000000 getdaft-0.1.7/tools/wheels/_vendor/wheel/cli/convert.py
--rw-r--r--   0      501       20     3113 2023-06-26 18:37:01.000000 getdaft-0.1.7/tools/wheels/_vendor/wheel/cli/pack.py
--rw-r--r--   0      501       20      662 2023-06-26 18:37:01.000000 getdaft-0.1.7/tools/wheels/_vendor/wheel/cli/unpack.py
--rw-r--r--   0      501       20     1246 2023-06-26 18:37:01.000000 getdaft-0.1.7/tools/wheels/_vendor/wheel/pkginfo.py
--rw-r--r--   0      501       20      974 2023-06-26 18:37:01.000000 getdaft-0.1.7/tools/wheels/_vendor/wheel/util.py
--rw-r--r--   0      501       20     7125 2023-06-26 18:37:01.000000 getdaft-0.1.7/tools/wheels/_vendor/wheel/wheelfile.py
--rw-r--r--   0      501       20      878 2023-06-26 18:37:01.000000 getdaft-0.1.7/tools/wheels/fix-and-copy-wheel.py
--rw-r--r--   0      501       20     2981 2023-06-26 18:37:01.000000 getdaft-0.1.7/tools/wheels/tmpdirs.py
--rw-r--r--   0      501       20     4469 2023-06-26 18:37:01.000000 getdaft-0.1.7/tools/wheels/tools.py
--rw-r--r--   0      501       20     9484 2023-06-26 18:37:01.000000 getdaft-0.1.7/tools/wheels/wheeltools.py
--rw-r--r--   0      501       20       19 2023-06-26 18:37:01.000000 getdaft-0.1.7/tutorials/.gitignore
--rw-r--r--   0      501       20    19755 2023-06-26 18:37:01.000000 getdaft-0.1.7/tutorials/embeddings/daft_tutorial_embeddings_stackexchange.ipynb
--rw-r--r--   0      501       20    12068 2023-06-26 18:37:01.000000 getdaft-0.1.7/tutorials/image_querying/top_n_red_color.ipynb
--rw-r--r--   0      501       20    98730 2023-06-26 18:37:01.000000 getdaft-0.1.7/tutorials/mnist.ipynb
--rw-r--r--   0      501       20    11847 2023-06-26 18:37:01.000000 getdaft-0.1.7/tutorials/text_to_image/text_to_image_generation.ipynb
--rw-r--r--   0      501       20     9134 2023-06-26 18:37:01.000000 getdaft-0.1.7/tutorials/text_to_image/using_cloud_with_ray.ipynb
--rw-r--r--   0      501       20    73843 2023-06-26 18:38:06.000000 getdaft-0.1.7/Cargo.lock
--rw-r--r--   0        0        0    10351 1970-01-01 00:00:00.000000 getdaft-0.1.7/PKG-INFO
+-rw-r--r--   0        0        0     1001 1970-01-01 00:00:00.000000 getdaft-0.1.8/local_dependencies/daft-table/Cargo.toml
+-rw-r--r--   0      501       20     2853 2023-07-05 18:53:54.000000 getdaft-0.1.8/local_dependencies/daft-table/src/ffi.rs
+-rw-r--r--   0      501       20    20730 2023-07-05 18:53:54.000000 getdaft-0.1.8/local_dependencies/daft-table/src/lib.rs
+-rw-r--r--   0      501       20     2168 2023-07-05 18:53:54.000000 getdaft-0.1.8/local_dependencies/daft-table/src/ops/agg.rs
+-rw-r--r--   0      501       20     3748 2023-07-05 18:53:54.000000 getdaft-0.1.8/local_dependencies/daft-table/src/ops/explode.rs
+-rw-r--r--   0      501       20     4415 2023-07-05 18:53:54.000000 getdaft-0.1.8/local_dependencies/daft-table/src/ops/groups.rs
+-rw-r--r--   0      501       20     2898 2023-07-05 18:53:54.000000 getdaft-0.1.8/local_dependencies/daft-table/src/ops/hash.rs
+-rw-r--r--   0      501       20     2499 2023-07-05 18:53:54.000000 getdaft-0.1.8/local_dependencies/daft-table/src/ops/joins/hash_join.rs
+-rw-r--r--   0      501       20     3727 2023-07-05 18:53:54.000000 getdaft-0.1.8/local_dependencies/daft-table/src/ops/joins/mod.rs
+-rw-r--r--   0      501       20       99 2023-07-05 18:53:54.000000 getdaft-0.1.8/local_dependencies/daft-table/src/ops/mod.rs
+-rw-r--r--   0      501       20     3478 2023-07-05 18:53:54.000000 getdaft-0.1.8/local_dependencies/daft-table/src/ops/partition.rs
+-rw-r--r--   0      501       20     1808 2023-07-05 18:53:54.000000 getdaft-0.1.8/local_dependencies/daft-table/src/ops/search_sorted.rs
+-rw-r--r--   0      501       20      998 2023-07-05 18:53:54.000000 getdaft-0.1.8/local_dependencies/daft-table/src/ops/sort.rs
+-rw-r--r--   0      501       20    11179 2023-07-05 18:53:54.000000 getdaft-0.1.8/local_dependencies/daft-table/src/python.rs
+-rw-r--r--   0        0        0      649 1970-01-01 00:00:00.000000 getdaft-0.1.8/local_dependencies/common-error/Cargo.toml
+-rw-r--r--   0      501       20     2849 2023-07-05 18:53:54.000000 getdaft-0.1.8/local_dependencies/common-error/src/error.rs
+-rw-r--r--   0      501       20       64 2023-07-05 18:53:54.000000 getdaft-0.1.8/local_dependencies/common-error/src/lib.rs
+-rw-r--r--   0        0        0     1165 1970-01-01 00:00:00.000000 getdaft-0.1.8/local_dependencies/daft-io/Cargo.toml
+-rw-r--r--   0      501       20     1087 2023-07-05 18:53:54.000000 getdaft-0.1.8/local_dependencies/daft-io/src/config.rs
+-rw-r--r--   0      501       20     4730 2023-07-05 18:53:54.000000 getdaft-0.1.8/local_dependencies/daft-io/src/http.rs
+-rw-r--r--   0      501       20     8332 2023-07-05 18:53:54.000000 getdaft-0.1.8/local_dependencies/daft-io/src/lib.rs
+-rw-r--r--   0      501       20     6205 2023-07-05 18:53:54.000000 getdaft-0.1.8/local_dependencies/daft-io/src/local.rs
+-rw-r--r--   0      501       20     1652 2023-07-05 18:53:54.000000 getdaft-0.1.8/local_dependencies/daft-io/src/object_io.rs
+-rw-r--r--   0      501       20     1966 2023-07-05 18:53:54.000000 getdaft-0.1.8/local_dependencies/daft-io/src/python.rs
+-rw-r--r--   0      501       20    13490 2023-07-05 18:53:54.000000 getdaft-0.1.8/local_dependencies/daft-io/src/s3_like.rs
+-rw-r--r--   0        0        0      679 1970-01-01 00:00:00.000000 getdaft-0.1.8/local_dependencies/daft-dsl/Cargo.toml
+-rw-r--r--   0      501       20      273 2023-07-05 18:53:54.000000 getdaft-0.1.8/local_dependencies/daft-dsl/src/README.md
+-rw-r--r--   0      501       20     1454 2023-07-05 18:53:54.000000 getdaft-0.1.8/local_dependencies/daft-dsl/src/arithmetic.rs
+-rw-r--r--   0      501       20    19598 2023-07-05 18:53:54.000000 getdaft-0.1.8/local_dependencies/daft-dsl/src/expr.rs
+-rw-r--r--   0      501       20     1456 2023-07-05 18:53:54.000000 getdaft-0.1.8/local_dependencies/daft-dsl/src/functions/float/is_nan.rs
+-rw-r--r--   0      501       20      582 2023-07-05 18:53:54.000000 getdaft-0.1.8/local_dependencies/daft-dsl/src/functions/float/mod.rs
+-rw-r--r--   0      501       20     1353 2023-07-05 18:53:54.000000 getdaft-0.1.8/local_dependencies/daft-dsl/src/functions/image/decode.rs
+-rw-r--r--   0      501       20     1790 2023-07-05 18:53:54.000000 getdaft-0.1.8/local_dependencies/daft-dsl/src/functions/image/encode.rs
+-rw-r--r--   0      501       20     1292 2023-07-05 18:53:54.000000 getdaft-0.1.8/local_dependencies/daft-dsl/src/functions/image/mod.rs
+-rw-r--r--   0      501       20     2524 2023-07-05 18:53:54.000000 getdaft-0.1.8/local_dependencies/daft-dsl/src/functions/image/resize.rs
+-rw-r--r--   0      501       20     1130 2023-07-05 18:53:54.000000 getdaft-0.1.8/local_dependencies/daft-dsl/src/functions/list/explode.rs
+-rw-r--r--   0      501       20     2329 2023-07-05 18:53:54.000000 getdaft-0.1.8/local_dependencies/daft-dsl/src/functions/list/join.rs
+-rw-r--r--   0      501       20      873 2023-07-05 18:53:54.000000 getdaft-0.1.8/local_dependencies/daft-dsl/src/functions/list/mod.rs
+-rw-r--r--   0      501       20     2085 2023-07-05 18:53:54.000000 getdaft-0.1.8/local_dependencies/daft-dsl/src/functions/mod.rs
+-rw-r--r--   0      501       20     1197 2023-07-05 18:53:54.000000 getdaft-0.1.8/local_dependencies/daft-dsl/src/functions/numeric/abs.rs
+-rw-r--r--   0      501       20      575 2023-07-05 18:53:54.000000 getdaft-0.1.8/local_dependencies/daft-dsl/src/functions/numeric/mod.rs
+-rw-r--r--   0      501       20      684 2023-07-05 18:53:54.000000 getdaft-0.1.8/local_dependencies/daft-dsl/src/functions/python/mod.rs
+-rw-r--r--   0      501       20     2050 2023-07-05 18:53:54.000000 getdaft-0.1.8/local_dependencies/daft-dsl/src/functions/python/partial_udf.rs
+-rw-r--r--   0      501       20     2793 2023-07-05 18:53:54.000000 getdaft-0.1.8/local_dependencies/daft-dsl/src/functions/python/udf.rs
+-rw-r--r--   0      501       20     1344 2023-07-05 18:53:54.000000 getdaft-0.1.8/local_dependencies/daft-dsl/src/functions/temporal/day.rs
+-rw-r--r--   0      501       20     1373 2023-07-05 18:53:54.000000 getdaft-0.1.8/local_dependencies/daft-dsl/src/functions/temporal/day_of_week.rs
+-rw-r--r--   0      501       20     1415 2023-07-05 18:53:54.000000 getdaft-0.1.8/local_dependencies/daft-dsl/src/functions/temporal/mod.rs
+-rw-r--r--   0      501       20     1355 2023-07-05 18:53:54.000000 getdaft-0.1.8/local_dependencies/daft-dsl/src/functions/temporal/month.rs
+-rw-r--r--   0      501       20     1349 2023-07-05 18:53:54.000000 getdaft-0.1.8/local_dependencies/daft-dsl/src/functions/temporal/year.rs
+-rw-r--r--   0      501       20     2295 2023-07-05 18:53:54.000000 getdaft-0.1.8/local_dependencies/daft-dsl/src/functions/uri/download.rs
+-rw-r--r--   0      501       20     1073 2023-07-05 18:53:54.000000 getdaft-0.1.8/local_dependencies/daft-dsl/src/functions/uri/mod.rs
+-rw-r--r--   0      501       20     1652 2023-07-05 18:53:54.000000 getdaft-0.1.8/local_dependencies/daft-dsl/src/functions/utf8/contains.rs
+-rw-r--r--   0      501       20     1651 2023-07-05 18:53:54.000000 getdaft-0.1.8/local_dependencies/daft-dsl/src/functions/utf8/endswith.rs
+-rw-r--r--   0      501       20     1370 2023-07-05 18:53:54.000000 getdaft-0.1.8/local_dependencies/daft-dsl/src/functions/utf8/length.rs
+-rw-r--r--   0      501       20     1519 2023-07-05 18:53:54.000000 getdaft-0.1.8/local_dependencies/daft-dsl/src/functions/utf8/mod.rs
+-rw-r--r--   0      501       20     1661 2023-07-05 18:53:54.000000 getdaft-0.1.8/local_dependencies/daft-dsl/src/functions/utf8/startswith.rs
+-rw-r--r--   0      501       20      707 2023-07-05 18:53:54.000000 getdaft-0.1.8/local_dependencies/daft-dsl/src/lib.rs
+-rw-r--r--   0      501       20     4967 2023-07-05 18:53:54.000000 getdaft-0.1.8/local_dependencies/daft-dsl/src/lit.rs
+-rw-r--r--   0      501       20     5298 2023-07-05 18:53:54.000000 getdaft-0.1.8/local_dependencies/daft-dsl/src/optimization.rs
+-rw-r--r--   0      501       20     1982 2023-07-05 18:53:54.000000 getdaft-0.1.8/local_dependencies/daft-dsl/src/pyobject.rs
+-rw-r--r--   0      501       20    11937 2023-07-05 18:53:54.000000 getdaft-0.1.8/local_dependencies/daft-dsl/src/python.rs
+-rw-r--r--   0        0        0     1565 1970-01-01 00:00:00.000000 getdaft-0.1.8/local_dependencies/daft-core/Cargo.toml
+-rw-r--r--   0      501       20     5844 2023-07-05 18:53:54.000000 getdaft-0.1.8/local_dependencies/daft-core/src/array/from.rs
+-rw-r--r--   0      501       20      734 2023-07-05 18:53:54.000000 getdaft-0.1.8/local_dependencies/daft-core/src/array/iterator.rs
+-rw-r--r--   0      501       20     3012 2023-07-05 18:53:54.000000 getdaft-0.1.8/local_dependencies/daft-core/src/array/mod.rs
+-rw-r--r--   0      501       20      269 2023-07-05 18:53:54.000000 getdaft-0.1.8/local_dependencies/daft-core/src/array/ops/abs.rs
+-rw-r--r--   0      501       20      738 2023-07-05 18:53:54.000000 getdaft-0.1.8/local_dependencies/daft-core/src/array/ops/apply.rs
+-rw-r--r--   0      501       20      849 2023-07-05 18:53:54.000000 getdaft-0.1.8/local_dependencies/daft-core/src/array/ops/arange.rs
+-rw-r--r--   0      501       20     6972 2023-07-05 18:53:54.000000 getdaft-0.1.8/local_dependencies/daft-core/src/array/ops/arithmetic.rs
+-rw-r--r--   0      501       20     3055 2023-07-05 18:53:54.000000 getdaft-0.1.8/local_dependencies/daft-core/src/array/ops/arrow2/comparison.rs
+-rw-r--r--   0      501       20       34 2023-07-05 18:53:54.000000 getdaft-0.1.8/local_dependencies/daft-core/src/array/ops/arrow2/mod.rs
+-rw-r--r--   0      501       20       19 2023-07-05 18:53:54.000000 getdaft-0.1.8/local_dependencies/daft-core/src/array/ops/arrow2/sort/mod.rs
+-rw-r--r--   0      501       20     3482 2023-07-05 18:53:54.000000 getdaft-0.1.8/local_dependencies/daft-core/src/array/ops/arrow2/sort/primitive/common.rs
+-rw-r--r--   0      501       20      723 2023-07-05 18:53:54.000000 getdaft-0.1.8/local_dependencies/daft-core/src/array/ops/arrow2/sort/primitive/indices.rs
+-rw-r--r--   0      501       20       47 2023-07-05 18:53:54.000000 getdaft-0.1.8/local_dependencies/daft-core/src/array/ops/arrow2/sort/primitive/mod.rs
+-rw-r--r--   0      501       20     8075 2023-07-05 18:53:54.000000 getdaft-0.1.8/local_dependencies/daft-core/src/array/ops/arrow2/sort/primitive/sort.rs
+-rw-r--r--   0      501       20     2409 2023-07-05 18:53:54.000000 getdaft-0.1.8/local_dependencies/daft-core/src/array/ops/as_arrow.rs
+-rw-r--r--   0      501       20    11395 2023-07-05 18:53:54.000000 getdaft-0.1.8/local_dependencies/daft-core/src/array/ops/broadcast.rs
+-rw-r--r--   0      501       20    40353 2023-07-05 18:53:54.000000 getdaft-0.1.8/local_dependencies/daft-core/src/array/ops/cast.rs
+-rw-r--r--   0      501       20    11029 2023-07-05 18:53:54.000000 getdaft-0.1.8/local_dependencies/daft-core/src/array/ops/compare_agg.rs
+-rw-r--r--   0      501       20    47241 2023-07-05 18:53:54.000000 getdaft-0.1.8/local_dependencies/daft-core/src/array/ops/comparison.rs
+-rw-r--r--   0      501       20     1630 2023-07-05 18:53:54.000000 getdaft-0.1.8/local_dependencies/daft-core/src/array/ops/concat.rs
+-rw-r--r--   0      501       20     5991 2023-07-05 18:53:54.000000 getdaft-0.1.8/local_dependencies/daft-core/src/array/ops/concat_agg.rs
+-rw-r--r--   0      501       20     1444 2023-07-05 18:53:54.000000 getdaft-0.1.8/local_dependencies/daft-core/src/array/ops/count.rs
+-rw-r--r--   0      501       20     1548 2023-07-05 18:53:54.000000 getdaft-0.1.8/local_dependencies/daft-core/src/array/ops/date.rs
+-rw-r--r--   0      501       20     2430 2023-07-05 18:53:54.000000 getdaft-0.1.8/local_dependencies/daft-core/src/array/ops/filter.rs
+-rw-r--r--   0      501       20     1271 2023-07-05 18:53:54.000000 getdaft-0.1.8/local_dependencies/daft-core/src/array/ops/float.rs
+-rw-r--r--   0      501       20     1936 2023-07-05 18:53:54.000000 getdaft-0.1.8/local_dependencies/daft-core/src/array/ops/full.rs
+-rw-r--r--   0      501       20     4823 2023-07-05 18:53:54.000000 getdaft-0.1.8/local_dependencies/daft-core/src/array/ops/get.rs
+-rw-r--r--   0      501       20     4119 2023-07-05 18:53:54.000000 getdaft-0.1.8/local_dependencies/daft-core/src/array/ops/groups.rs
+-rw-r--r--   0      501       20     1523 2023-07-05 18:53:54.000000 getdaft-0.1.8/local_dependencies/daft-core/src/array/ops/hash.rs
+-rw-r--r--   0      501       20    12222 2023-07-05 18:53:54.000000 getdaft-0.1.8/local_dependencies/daft-core/src/array/ops/if_else.rs
+-rw-r--r--   0      501       20    29241 2023-07-05 18:53:54.000000 getdaft-0.1.8/local_dependencies/daft-core/src/array/ops/image.rs
+-rw-r--r--   0      501       20     1069 2023-07-05 18:53:54.000000 getdaft-0.1.8/local_dependencies/daft-core/src/array/ops/len.rs
+-rw-r--r--   0      501       20     6625 2023-07-05 18:53:54.000000 getdaft-0.1.8/local_dependencies/daft-core/src/array/ops/list.rs
+-rw-r--r--   0      501       20     3367 2023-07-05 18:53:54.000000 getdaft-0.1.8/local_dependencies/daft-core/src/array/ops/list_agg.rs
+-rw-r--r--   0      501       20     1634 2023-07-05 18:53:54.000000 getdaft-0.1.8/local_dependencies/daft-core/src/array/ops/mean.rs
+-rw-r--r--   0      501       20     2629 2023-07-05 18:53:54.000000 getdaft-0.1.8/local_dependencies/daft-core/src/array/ops/mod.rs
+-rw-r--r--   0      501       20     1325 2023-07-05 18:53:54.000000 getdaft-0.1.8/local_dependencies/daft-core/src/array/ops/null.rs
+-rw-r--r--   0      501       20     3826 2023-07-05 18:53:54.000000 getdaft-0.1.8/local_dependencies/daft-core/src/array/ops/pairwise.rs
+-rw-r--r--   0      501       20     9877 2023-07-05 18:53:54.000000 getdaft-0.1.8/local_dependencies/daft-core/src/array/ops/repr.rs
+-rw-r--r--   0      501       20      491 2023-07-05 18:53:54.000000 getdaft-0.1.8/local_dependencies/daft-core/src/array/ops/search_sorted.rs
+-rw-r--r--   0      501       20    19867 2023-07-05 18:53:54.000000 getdaft-0.1.8/local_dependencies/daft-core/src/array/ops/sort.rs
+-rw-r--r--   0      501       20     2396 2023-07-05 18:53:54.000000 getdaft-0.1.8/local_dependencies/daft-core/src/array/ops/sum.rs
+-rw-r--r--   0      501       20     4604 2023-07-05 18:53:54.000000 getdaft-0.1.8/local_dependencies/daft-core/src/array/ops/take.rs
+-rw-r--r--   0      501       20     5279 2023-07-05 18:53:54.000000 getdaft-0.1.8/local_dependencies/daft-core/src/array/ops/utf8.rs
+-rw-r--r--   0      501       20      995 2023-07-05 18:53:54.000000 getdaft-0.1.8/local_dependencies/daft-core/src/array/pseudo_arrow/compute.rs
+-rw-r--r--   0      501       20    13611 2023-07-05 18:53:54.000000 getdaft-0.1.8/local_dependencies/daft-core/src/array/pseudo_arrow/mod.rs
+-rw-r--r--   0      501       20     2502 2023-07-05 18:53:54.000000 getdaft-0.1.8/local_dependencies/daft-core/src/array/pseudo_arrow/python.rs
+-rw-r--r--   0      501       20     8228 2023-07-05 18:53:54.000000 getdaft-0.1.8/local_dependencies/daft-core/src/datatypes/binary_ops.rs
+-rw-r--r--   0      501       20    15026 2023-07-05 18:53:54.000000 getdaft-0.1.8/local_dependencies/daft-core/src/datatypes/dtype.rs
+-rw-r--r--   0      501       20     2021 2023-07-05 18:53:54.000000 getdaft-0.1.8/local_dependencies/daft-core/src/datatypes/field.rs
+-rw-r--r--   0      501       20     3187 2023-07-05 18:53:54.000000 getdaft-0.1.8/local_dependencies/daft-core/src/datatypes/image_format.rs
+-rw-r--r--   0      501       20     6382 2023-07-05 18:53:54.000000 getdaft-0.1.8/local_dependencies/daft-core/src/datatypes/image_mode.rs
+-rw-r--r--   0      501       20     3589 2023-07-05 18:53:54.000000 getdaft-0.1.8/local_dependencies/daft-core/src/datatypes/logical.rs
+-rw-r--r--   0      501       20     9200 2023-07-05 18:53:54.000000 getdaft-0.1.8/local_dependencies/daft-core/src/datatypes/matching.rs
+-rw-r--r--   0      501       20     6905 2023-07-05 18:53:54.000000 getdaft-0.1.8/local_dependencies/daft-core/src/datatypes/mod.rs
+-rw-r--r--   0      501       20     1100 2023-07-05 18:53:54.000000 getdaft-0.1.8/local_dependencies/daft-core/src/datatypes/time_unit.rs
+-rw-r--r--   0      501       20     5128 2023-07-05 18:53:54.000000 getdaft-0.1.8/local_dependencies/daft-core/src/ffi.rs
+-rw-r--r--   0      501       20     6022 2023-07-05 18:53:54.000000 getdaft-0.1.8/local_dependencies/daft-core/src/kernels/hashing.rs
+-rw-r--r--   0      501       20       54 2023-07-05 18:53:54.000000 getdaft-0.1.8/local_dependencies/daft-core/src/kernels/mod.rs
+-rw-r--r--   0      501       20    12159 2023-07-05 18:53:54.000000 getdaft-0.1.8/local_dependencies/daft-core/src/kernels/search_sorted.rs
+-rw-r--r--   0      501       20     3917 2023-07-05 18:53:54.000000 getdaft-0.1.8/local_dependencies/daft-core/src/kernels/utf8.rs
+-rw-r--r--   0      501       20      553 2023-07-05 18:53:54.000000 getdaft-0.1.8/local_dependencies/daft-core/src/lib.rs
+-rw-r--r--   0      501       20     8528 2023-07-05 18:53:54.000000 getdaft-0.1.8/local_dependencies/daft-core/src/python/datatype.rs
+-rw-r--r--   0      501       20     1661 2023-07-05 18:53:54.000000 getdaft-0.1.8/local_dependencies/daft-core/src/python/field.rs
+-rw-r--r--   0      501       20      610 2023-07-05 18:53:54.000000 getdaft-0.1.8/local_dependencies/daft-core/src/python/mod.rs
+-rw-r--r--   0      501       20     2843 2023-07-05 18:53:54.000000 getdaft-0.1.8/local_dependencies/daft-core/src/python/schema.rs
+-rw-r--r--   0      501       20    12308 2023-07-05 18:53:54.000000 getdaft-0.1.8/local_dependencies/daft-core/src/python/series.rs
+-rw-r--r--   0      501       20     3729 2023-07-05 18:53:54.000000 getdaft-0.1.8/local_dependencies/daft-core/src/schema.rs
+-rw-r--r--   0      501       20     7500 2023-07-05 18:53:54.000000 getdaft-0.1.8/local_dependencies/daft-core/src/series/array_impl/binary_ops.rs
+-rw-r--r--   0      501       20    11522 2023-07-05 18:53:54.000000 getdaft-0.1.8/local_dependencies/daft-core/src/series/array_impl/data_array.rs
+-rw-r--r--   0      501       20     6504 2023-07-05 18:53:54.000000 getdaft-0.1.8/local_dependencies/daft-core/src/series/array_impl/logical_array.rs
+-rw-r--r--   0      501       20      181 2023-07-05 18:53:54.000000 getdaft-0.1.8/local_dependencies/daft-core/src/series/array_impl/mod.rs
+-rw-r--r--   0      501       20     2106 2023-07-05 18:53:54.000000 getdaft-0.1.8/local_dependencies/daft-core/src/series/from.rs
+-rw-r--r--   0      501       20     2309 2023-07-05 18:53:54.000000 getdaft-0.1.8/local_dependencies/daft-core/src/series/mod.rs
+-rw-r--r--   0      501       20      910 2023-07-05 18:53:54.000000 getdaft-0.1.8/local_dependencies/daft-core/src/series/ops/abs.rs
+-rw-r--r--   0      501       20     5199 2023-07-05 18:53:54.000000 getdaft-0.1.8/local_dependencies/daft-core/src/series/ops/agg.rs
+-rw-r--r--   0      501       20     3419 2023-07-05 18:53:54.000000 getdaft-0.1.8/local_dependencies/daft-core/src/series/ops/arithmetic.rs
+-rw-r--r--   0      501       20     1924 2023-07-05 18:53:54.000000 getdaft-0.1.8/local_dependencies/daft-core/src/series/ops/broadcast.rs
+-rw-r--r--   0      501       20      205 2023-07-05 18:53:54.000000 getdaft-0.1.8/local_dependencies/daft-core/src/series/ops/cast.rs
+-rw-r--r--   0      501       20     2616 2023-07-05 18:53:54.000000 getdaft-0.1.8/local_dependencies/daft-core/src/series/ops/comparison.rs
+-rw-r--r--   0      501       20     1565 2023-07-05 18:53:54.000000 getdaft-0.1.8/local_dependencies/daft-core/src/series/ops/concat.rs
+-rw-r--r--   0      501       20     1820 2023-07-05 18:53:54.000000 getdaft-0.1.8/local_dependencies/daft-core/src/series/ops/date.rs
+-rw-r--r--   0      501       20     3621 2023-07-05 18:53:54.000000 getdaft-0.1.8/local_dependencies/daft-core/src/series/ops/downcast.rs
+-rw-r--r--   0      501       20      693 2023-07-05 18:53:54.000000 getdaft-0.1.8/local_dependencies/daft-core/src/series/ops/filter.rs
+-rw-r--r--   0      501       20      411 2023-07-05 18:53:54.000000 getdaft-0.1.8/local_dependencies/daft-core/src/series/ops/float.rs
+-rw-r--r--   0      501       20      439 2023-07-05 18:53:54.000000 getdaft-0.1.8/local_dependencies/daft-core/src/series/ops/groups.rs
+-rw-r--r--   0      501       20      416 2023-07-05 18:53:54.000000 getdaft-0.1.8/local_dependencies/daft-core/src/series/ops/hash.rs
+-rw-r--r--   0      501       20      324 2023-07-05 18:53:54.000000 getdaft-0.1.8/local_dependencies/daft-core/src/series/ops/if_else.rs
+-rw-r--r--   0      501       20     2468 2023-07-05 18:53:54.000000 getdaft-0.1.8/local_dependencies/daft-core/src/series/ops/image.rs
+-rw-r--r--   0      501       20      297 2023-07-05 18:53:54.000000 getdaft-0.1.8/local_dependencies/daft-core/src/series/ops/len.rs
+-rw-r--r--   0      501       20     2351 2023-07-05 18:53:54.000000 getdaft-0.1.8/local_dependencies/daft-core/src/series/ops/list.rs
+-rw-r--r--   0      501       20     2541 2023-07-05 18:53:54.000000 getdaft-0.1.8/local_dependencies/daft-core/src/series/ops/mod.rs
+-rw-r--r--   0      501       20      475 2023-07-05 18:53:54.000000 getdaft-0.1.8/local_dependencies/daft-core/src/series/ops/not.rs
+-rw-r--r--   0      501       20      160 2023-07-05 18:53:54.000000 getdaft-0.1.8/local_dependencies/daft-core/src/series/ops/null.rs
+-rw-r--r--   0      501       20      645 2023-07-05 18:53:54.000000 getdaft-0.1.8/local_dependencies/daft-core/src/series/ops/search_sorted.rs
+-rw-r--r--   0      501       20     1504 2023-07-05 18:53:54.000000 getdaft-0.1.8/local_dependencies/daft-core/src/series/ops/sort.rs
+-rw-r--r--   0      501       20      662 2023-07-05 18:53:54.000000 getdaft-0.1.8/local_dependencies/daft-core/src/series/ops/take.rs
+-rw-r--r--   0      501       20     1526 2023-07-05 18:53:54.000000 getdaft-0.1.8/local_dependencies/daft-core/src/series/ops/utf8.rs
+-rw-r--r--   0      501       20     1718 2023-07-05 18:53:54.000000 getdaft-0.1.8/local_dependencies/daft-core/src/series/series_like.rs
+-rw-r--r--   0      501       20     5401 2023-07-05 18:53:54.000000 getdaft-0.1.8/local_dependencies/daft-core/src/utils/arrow.rs
+-rw-r--r--   0      501       20      347 2023-07-05 18:53:54.000000 getdaft-0.1.8/local_dependencies/daft-core/src/utils/mod.rs
+-rw-r--r--   0      501       20    10066 2023-07-05 18:53:54.000000 getdaft-0.1.8/local_dependencies/daft-core/src/utils/supertype.rs
+-rw-r--r--   0        0        0     2202 1970-01-01 00:00:00.000000 getdaft-0.1.8/Cargo.toml
+-rw-r--r--   0      501       20      834 2023-07-05 18:53:54.000000 getdaft-0.1.8/.github/ISSUE_TEMPLATE/bug_report.md
+-rw-r--r--   0      501       20      595 2023-07-05 18:53:54.000000 getdaft-0.1.8/.github/ISSUE_TEMPLATE/feature_request.md
+-rw-r--r--   0      501       20      431 2023-07-05 18:53:54.000000 getdaft-0.1.8/.github/dependabot.yml
+-rw-r--r--   0      501       20     1063 2023-07-05 18:53:54.000000 getdaft-0.1.8/.github/release-drafter.yml
+-rw-r--r--   0      501       20     1333 2023-07-05 18:53:54.000000 getdaft-0.1.8/.github/workflows/broken-link-checker.yml
+-rw-r--r--   0      501       20     3395 2023-07-05 18:53:54.000000 getdaft-0.1.8/.github/workflows/daft-profiling.yml
+-rw-r--r--   0      501       20     1627 2023-07-05 18:53:54.000000 getdaft-0.1.8/.github/workflows/notebook-checker.yml
+-rw-r--r--   0      501       20     2211 2023-07-05 18:53:54.000000 getdaft-0.1.8/.github/workflows/property-based-tests.yml
+-rw-r--r--   0      501       20    16055 2023-07-05 18:53:54.000000 getdaft-0.1.8/.github/workflows/python-package.yml
+-rw-r--r--   0      501       20     6165 2023-07-05 18:53:54.000000 getdaft-0.1.8/.github/workflows/python-publish.yml
+-rw-r--r--   0      501       20     2655 2023-07-05 18:53:54.000000 getdaft-0.1.8/.github/workflows/ray-compatibility.yml
+-rw-r--r--   0      501       20     2696 2023-07-05 18:53:54.000000 getdaft-0.1.8/.github/workflows/release-drafter.yml
+-rw-r--r--   0      501       20      306 2023-07-05 18:53:54.000000 getdaft-0.1.8/.gitignore
+-rw-r--r--   0      501       20     2226 2023-07-05 18:53:54.000000 getdaft-0.1.8/.pre-commit-config.yaml
+-rw-r--r--   0      501       20      205 2023-07-05 18:53:54.000000 getdaft-0.1.8/.readthedocs.yaml
+-rw-r--r--   0      501       20     1550 2023-07-05 18:53:54.000000 getdaft-0.1.8/CONTRIBUTING.md
+-rw-r--r--   0      501       20    11357 2023-07-05 18:53:54.000000 getdaft-0.1.8/LICENSE
+-rw-r--r--   0      501       20     1295 2023-07-05 18:53:54.000000 getdaft-0.1.8/Makefile
+-rw-r--r--   0      501       20     8834 2023-07-05 18:53:54.000000 getdaft-0.1.8/README.rst
+-rw-r--r--   0      501       20        0 2023-07-05 18:53:54.000000 getdaft-0.1.8/benchmarking/__init__.py
+-rw-r--r--   0      501       20        0 2023-07-05 18:53:54.000000 getdaft-0.1.8/benchmarking/tpch/__init__.py
+-rw-r--r--   0      501       20     9495 2023-07-05 18:53:54.000000 getdaft-0.1.8/benchmarking/tpch/__main__.py
+-rw-r--r--   0      501       20    12428 2023-07-05 18:53:54.000000 getdaft-0.1.8/benchmarking/tpch/answers.py
+-rw-r--r--   0      501       20    12336 2023-07-05 18:53:54.000000 getdaft-0.1.8/benchmarking/tpch/data_generation.py
+-rw-r--r--   0      501       20     4573 2023-07-05 18:53:54.000000 getdaft-0.1.8/benchmarking/tpch/pipelined_data_generation.py
+-rw-r--r--   0      501       20     2654 2023-07-05 18:53:54.000000 getdaft-0.1.8/benchmarking/tpch/subprefix_s3_files.py
+-rw-r--r--   0      501       20     1436 2023-07-05 18:53:54.000000 getdaft-0.1.8/ci/upload_wheels.sh
+-rw-r--r--   0      501       20      446 2023-07-05 18:53:54.000000 getdaft-0.1.8/codecov.yml
+-rw-r--r--   0      501       20     2199 2023-07-05 18:53:54.000000 getdaft-0.1.8/daft/__init__.py
+-rw-r--r--   0      501       20     6724 2023-07-05 18:53:54.000000 getdaft-0.1.8/daft/analytics.py
+-rw-r--r--   0      501       20     3935 2023-07-05 18:53:54.000000 getdaft-0.1.8/daft/api_annotations.py
+-rw-r--r--   0      501       20    10591 2023-07-05 18:53:54.000000 getdaft-0.1.8/daft/arrow_utils.py
+-rw-r--r--   0      501       20     5511 2023-07-05 18:53:54.000000 getdaft-0.1.8/daft/context.py
+-rw-r--r--   0      501       20     3412 2023-07-05 18:53:54.000000 getdaft-0.1.8/daft/convert.py
+-rw-r--r--   0      501       20     1298 2023-07-05 18:53:54.000000 getdaft-0.1.8/daft/daft.pyi
+-rw-r--r--   0      501       20       94 2023-07-05 18:53:54.000000 getdaft-0.1.8/daft/dataframe/__init__.py
+-rw-r--r--   0      501       20    54827 2023-07-05 18:53:54.000000 getdaft-0.1.8/daft/dataframe/dataframe.py
+-rw-r--r--   0      501       20      306 2023-07-05 18:53:54.000000 getdaft-0.1.8/daft/dataframe/preview.py
+-rw-r--r--   0      501       20     1404 2023-07-05 18:53:54.000000 getdaft-0.1.8/daft/dataframe/to_torch.py
+-rw-r--r--   0      501       20      850 2023-07-05 18:53:54.000000 getdaft-0.1.8/daft/datasources.py
+-rw-r--r--   0      501       20    17515 2023-07-05 18:53:54.000000 getdaft-0.1.8/daft/datatype.py
+-rw-r--r--   0      501       20       84 2023-07-05 18:53:54.000000 getdaft-0.1.8/daft/errors.py
+-rw-r--r--   0      501       20        0 2023-07-05 18:53:54.000000 getdaft-0.1.8/daft/execution/__init__.py
+-rw-r--r--   0      501       20    28993 2023-07-05 18:53:54.000000 getdaft-0.1.8/daft/execution/execution_step.py
+-rw-r--r--   0      501       20    28946 2023-07-05 18:53:54.000000 getdaft-0.1.8/daft/execution/physical_plan.py
+-rw-r--r--   0      501       20     6350 2023-07-05 18:53:54.000000 getdaft-0.1.8/daft/execution/physical_plan_factory.py
+-rw-r--r--   0      501       20      170 2023-07-05 18:53:54.000000 getdaft-0.1.8/daft/expressions/__init__.py
+-rw-r--r--   0      501       20    28908 2023-07-05 18:53:54.000000 getdaft-0.1.8/daft/expressions/expressions.py
+-rw-r--r--   0      501       20      572 2023-07-05 18:53:54.000000 getdaft-0.1.8/daft/expressions/testing.py
+-rw-r--r--   0      501       20    12728 2023-07-05 18:53:54.000000 getdaft-0.1.8/daft/filesystem.py
+-rw-r--r--   0      501       20        0 2023-07-05 18:53:54.000000 getdaft-0.1.8/daft/internal/__init__.py
+-rw-r--r--   0      501       20      509 2023-07-05 18:53:54.000000 getdaft-0.1.8/daft/internal/gpu.py
+-rw-r--r--   0      501       20     1804 2023-07-05 18:53:54.000000 getdaft-0.1.8/daft/internal/rule.py
+-rw-r--r--   0      501       20     2030 2023-07-05 18:53:54.000000 getdaft-0.1.8/daft/internal/rule_runner.py
+-rw-r--r--   0      501       20     3490 2023-07-05 18:53:54.000000 getdaft-0.1.8/daft/internal/treenode.py
+-rw-r--r--   0      501       20      377 2023-07-05 18:53:54.000000 getdaft-0.1.8/daft/io/__init__.py
+-rw-r--r--   0      501       20     2456 2023-07-05 18:53:54.000000 getdaft-0.1.8/daft/io/_csv.py
+-rw-r--r--   0      501       20     1642 2023-07-05 18:53:54.000000 getdaft-0.1.8/daft/io/_json.py
+-rw-r--r--   0      501       20     2317 2023-07-05 18:53:54.000000 getdaft-0.1.8/daft/io/common.py
+-rw-r--r--   0      501       20     2036 2023-07-05 18:53:54.000000 getdaft-0.1.8/daft/io/file_path.py
+-rw-r--r--   0      501       20     1665 2023-07-05 18:53:54.000000 getdaft-0.1.8/daft/io/parquet.py
+-rw-r--r--   0      501       20      264 2023-07-05 18:53:54.000000 getdaft-0.1.8/daft/logging.py
+-rw-r--r--   0      501       20        0 2023-07-05 18:53:54.000000 getdaft-0.1.8/daft/logical/__init__.py
+-rw-r--r--   0      501       20     8601 2023-07-05 18:53:54.000000 getdaft-0.1.8/daft/logical/aggregation_plan_builder.py
+-rw-r--r--   0      501       20    38976 2023-07-05 18:53:54.000000 getdaft-0.1.8/daft/logical/logical_plan.py
+-rw-r--r--   0      501       20     1492 2023-07-05 18:53:54.000000 getdaft-0.1.8/daft/logical/map_partition_ops.py
+-rw-r--r--   0      501       20    19757 2023-07-05 18:53:54.000000 getdaft-0.1.8/daft/logical/optimizer.py
+-rw-r--r--   0      501       20     3868 2023-07-05 18:53:54.000000 getdaft-0.1.8/daft/logical/schema.py
+-rw-r--r--   0      501       20       99 2023-07-05 18:53:54.000000 getdaft-0.1.8/daft/pickle/__init__.py
+-rw-r--r--   0      501       20    34760 2023-07-05 18:53:54.000000 getdaft-0.1.8/daft/pickle/cloudpickle.py
+-rw-r--r--   0      501       20    34262 2023-07-05 18:53:54.000000 getdaft-0.1.8/daft/pickle/cloudpickle_fast.py
+-rw-r--r--   0      501       20      639 2023-07-05 18:53:54.000000 getdaft-0.1.8/daft/pickle/compat.py
+-rw-r--r--   0      501       20      312 2023-07-05 18:53:54.000000 getdaft-0.1.8/daft/pickle/pickle.py
+-rw-r--r--   0      501       20        0 2023-07-05 18:53:54.000000 getdaft-0.1.8/daft/py.typed
+-rw-r--r--   0      501       20     2036 2023-07-05 18:53:54.000000 getdaft-0.1.8/daft/resource_request.py
+-rw-r--r--   0      501       20        0 2023-07-05 18:53:54.000000 getdaft-0.1.8/daft/runners/__init__.py
+-rw-r--r--   0      501       20     4676 2023-07-05 18:53:54.000000 getdaft-0.1.8/daft/runners/partitioning.py
+-rw-r--r--   0      501       20     1488 2023-07-05 18:53:54.000000 getdaft-0.1.8/daft/runners/profiler.py
+-rw-r--r--   0      501       20    13802 2023-07-05 18:53:54.000000 getdaft-0.1.8/daft/runners/pyrunner.py
+-rw-r--r--   0      501       20    28094 2023-07-05 18:53:54.000000 getdaft-0.1.8/daft/runners/ray_runner.py
+-rw-r--r--   0      501       20     1428 2023-07-05 18:53:54.000000 getdaft-0.1.8/daft/runners/runner.py
+-rw-r--r--   0      501       20     3344 2023-07-05 18:53:54.000000 getdaft-0.1.8/daft/runners/runner_io.py
+-rw-r--r--   0      501       20    22246 2023-07-05 18:53:54.000000 getdaft-0.1.8/daft/series.py
+-rw-r--r--   0      501       20       82 2023-07-05 18:53:54.000000 getdaft-0.1.8/daft/table/__init__.py
+-rw-r--r--   0      501       20     2960 2023-07-05 18:53:54.000000 getdaft-0.1.8/daft/table/schema_inference.py
+-rw-r--r--   0      501       20    14029 2023-07-05 18:53:54.000000 getdaft-0.1.8/daft/table/table.py
+-rw-r--r--   0      501       20     9916 2023-07-05 18:53:54.000000 getdaft-0.1.8/daft/table/table_io.py
+-rw-r--r--   0      501       20     7370 2023-07-05 18:53:54.000000 getdaft-0.1.8/daft/udf.py
+-rw-r--r--   0      501       20        0 2023-07-05 18:53:54.000000 getdaft-0.1.8/daft/udf_library/__init__.py
+-rw-r--r--   0      501       20     3486 2023-07-05 18:53:54.000000 getdaft-0.1.8/daft/udf_library/url_udfs.py
+-rw-r--r--   0      501       20     2796 2023-07-05 18:53:54.000000 getdaft-0.1.8/daft/utils.py
+-rw-r--r--   0      501       20      183 2023-07-05 18:53:54.000000 getdaft-0.1.8/daft/viz/__init__.py
+-rw-r--r--   0      501       20     1929 2023-07-05 18:53:54.000000 getdaft-0.1.8/daft/viz/dataframe_display.py
+-rw-r--r--   0      501       20     1522 2023-07-05 18:53:54.000000 getdaft-0.1.8/daft/viz/html_viz_hooks.py
+-rw-r--r--   0      501       20      148 2023-07-05 18:53:54.000000 getdaft-0.1.8/docs/CONTRIBUTING.md
+-rw-r--r--   0      501       20      638 2023-07-05 18:53:54.000000 getdaft-0.1.8/docs/Makefile
+-rw-r--r--   0      501       20    73229 2023-07-05 18:53:54.000000 getdaft-0.1.8/docs/source/10-min.ipynb
+-rw-r--r--   0      501       20      389 2023-07-05 18:53:54.000000 getdaft-0.1.8/docs/source/_static/custom-function-signatures.css
+-rw-r--r--   0      501       20      565 2023-07-05 18:53:54.000000 getdaft-0.1.8/docs/source/_static/daft-favicon.png
+-rw-r--r--   0      501       20     7804 2023-07-05 18:53:54.000000 getdaft-0.1.8/docs/source/_static/daft-logo.png
+-rw-r--r--   0      501       20    42148 2023-07-05 18:53:54.000000 getdaft-0.1.8/docs/source/_static/daft_illustration.png
+-rw-r--r--   0      501       20      583 2023-07-05 18:53:54.000000 getdaft-0.1.8/docs/source/_static/dataframe-comp-table.csv
+-rw-r--r--   0      501       20    25200 2023-07-05 18:53:54.000000 getdaft-0.1.8/docs/source/_static/execution_model.png
+-rw-r--r--   0      501       20     1901 2023-07-05 18:53:54.000000 getdaft-0.1.8/docs/source/_static/header.css
+-rw-r--r--   0      501       20    32864 2023-07-05 18:53:54.000000 getdaft-0.1.8/docs/source/_static/high_level_architecture.png
+-rw-r--r--   0      501       20      343 2023-07-05 18:53:54.000000 getdaft-0.1.8/docs/source/_static/icon-menu-close.svg
+-rw-r--r--   0      501       20      333 2023-07-05 18:53:54.000000 getdaft-0.1.8/docs/source/_static/icon-menu-dots.svg
+-rw-r--r--   0      501       20    18177 2023-07-05 18:53:54.000000 getdaft-0.1.8/docs/source/_static/in_memory_data_representation.png
+-rw-r--r--   0      501       20      786 2023-07-05 18:53:54.000000 getdaft-0.1.8/docs/source/_static/mobile-menu.js
+-rw-r--r--   0      501       20     9142 2023-07-05 18:53:54.000000 getdaft-0.1.8/docs/source/_static/tpch-1000sf.html
+-rw-r--r--   0      501       20     9647 2023-07-05 18:53:54.000000 getdaft-0.1.8/docs/source/_static/tpch-100sf.html
+-rw-r--r--   0      501       20     8757 2023-07-05 18:53:54.000000 getdaft-0.1.8/docs/source/_static/tpch-nodes-count-daft-1000-sf.html
+-rw-r--r--   0      501       20      856 2023-07-05 18:53:54.000000 getdaft-0.1.8/docs/source/_templates/layout.html
+-rw-r--r--   0      501       20     1179 2023-07-05 18:53:54.000000 getdaft-0.1.8/docs/source/_templates/sections/header.html
+-rw-r--r--   0      501       20     1129 2023-07-05 18:53:54.000000 getdaft-0.1.8/docs/source/_templates/sections/mobile-menu.html
+-rw-r--r--   0      501       20      333 2023-07-05 18:53:54.000000 getdaft-0.1.8/docs/source/api_docs/context.rst
+-rw-r--r--   0      501       20     2759 2023-07-05 18:53:54.000000 getdaft-0.1.8/docs/source/api_docs/dataframe.rst
+-rw-r--r--   0      501       20     2293 2023-07-05 18:53:54.000000 getdaft-0.1.8/docs/source/api_docs/datatype.rst
+-rw-r--r--   0      501       20      139 2023-07-05 18:53:54.000000 getdaft-0.1.8/docs/source/api_docs/datatype_image_mode/daft.ImageMode.from_mode_string.rst
+-rw-r--r--   0      501       20      430 2023-07-05 18:53:54.000000 getdaft-0.1.8/docs/source/api_docs/datatype_image_mode/daft.ImageMode.rst
+-rw-r--r--   0      501       20      151 2023-07-05 18:53:54.000000 getdaft-0.1.8/docs/source/api_docs/datetype_image_format/daft.ImageFormat.from_format_string.rst
+-rw-r--r--   0      501       20      333 2023-07-05 18:53:54.000000 getdaft-0.1.8/docs/source/api_docs/datetype_image_format/daft.ImageFormat.rst
+-rw-r--r--   0      501       20     4727 2023-07-05 18:53:54.000000 getdaft-0.1.8/docs/source/api_docs/expressions.rst
+-rw-r--r--   0      501       20      816 2023-07-05 18:53:54.000000 getdaft-0.1.8/docs/source/api_docs/groupby.rst
+-rw-r--r--   0      501       20      146 2023-07-05 18:53:54.000000 getdaft-0.1.8/docs/source/api_docs/index.rst
+-rw-r--r--   0      501       20     1537 2023-07-05 18:53:54.000000 getdaft-0.1.8/docs/source/api_docs/input_output.rst
+-rw-r--r--   0      501       20      273 2023-07-05 18:53:54.000000 getdaft-0.1.8/docs/source/api_docs/series/daft.Series.rst
+-rw-r--r--   0      501       20      492 2023-07-05 18:53:54.000000 getdaft-0.1.8/docs/source/api_docs/series.rst
+-rw-r--r--   0      501       20       88 2023-07-05 18:53:54.000000 getdaft-0.1.8/docs/source/api_docs/udf.rst
+-rw-r--r--   0      501       20    14528 2023-07-05 18:53:54.000000 getdaft-0.1.8/docs/source/benchmarks/index.rst
+-rw-r--r--   0      501       20     4200 2023-07-05 18:53:54.000000 getdaft-0.1.8/docs/source/conf.py
+-rw-r--r--   0      501       20     5114 2023-07-05 18:53:54.000000 getdaft-0.1.8/docs/source/dataframe_comparison.rst
+-rw-r--r--   0      501       20     1723 2023-07-05 18:53:54.000000 getdaft-0.1.8/docs/source/index.rst
+-rw-r--r--   0      501       20     1356 2023-07-05 18:53:54.000000 getdaft-0.1.8/docs/source/install.rst
+-rw-r--r--   0      501       20      896 2023-07-05 18:53:54.000000 getdaft-0.1.8/docs/source/learn/index.rst
+-rw-r--r--   0      501       20     7830 2023-07-05 18:53:54.000000 getdaft-0.1.8/docs/source/learn/key_concepts.rst
+-rw-r--r--   0      501       20     1783 2023-07-05 18:53:54.000000 getdaft-0.1.8/docs/source/learn/tutorials.rst
+-rw-r--r--   0      501       20     1388 2023-07-05 18:53:54.000000 getdaft-0.1.8/docs/source/learn/user_guides/aggregations.rst
+-rw-r--r--   0      501       20     7009 2023-07-05 18:53:54.000000 getdaft-0.1.8/docs/source/learn/user_guides/dataframe-operations.rst
+-rw-r--r--   0      501       20     5166 2023-07-05 18:53:54.000000 getdaft-0.1.8/docs/source/learn/user_guides/datatypes.rst
+-rw-r--r--   0      501       20     9481 2023-07-05 18:53:54.000000 getdaft-0.1.8/docs/source/learn/user_guides/expressions.rst
+-rw-r--r--   0      501       20     8241 2023-07-05 18:53:54.000000 getdaft-0.1.8/docs/source/learn/user_guides/intro-dataframes.rst
+-rw-r--r--   0      501       20      206 2023-07-05 18:53:54.000000 getdaft-0.1.8/docs/source/learn/user_guides/partitioning.rst
+-rw-r--r--   0      501       20     3251 2023-07-05 18:53:54.000000 getdaft-0.1.8/docs/source/learn/user_guides/read-write.rst
+-rw-r--r--   0      501       20     1257 2023-07-05 18:53:54.000000 getdaft-0.1.8/docs/source/learn/user_guides/scaling-up.rst
+-rw-r--r--   0      501       20     8853 2023-07-05 18:53:54.000000 getdaft-0.1.8/docs/source/learn/user_guides/udf.rst
+-rw-r--r--   0      501       20     1577 2023-07-05 18:53:54.000000 getdaft-0.1.8/docs/source/learn/user_guides.rst
+-rw-r--r--   0      501       20     6628 2023-07-05 18:53:54.000000 getdaft-0.1.8/docs/source/technical_architecture.rst
+-rw-r--r--   0      501       20     1316 2023-07-05 18:53:54.000000 getdaft-0.1.8/docs/source/telemetry.rst
+-rw-r--r--   0      501       20     1871 2023-07-05 18:53:54.000000 getdaft-0.1.8/pyproject.toml
+-rw-r--r--   0      501       20     1137 2023-07-05 18:53:54.000000 getdaft-0.1.8/requirements-dev.txt
+-rw-r--r--   0      501       20       98 2023-07-05 18:53:54.000000 getdaft-0.1.8/rust-toolchain.toml
+-rw-r--r--   0      501       20      687 2023-07-05 18:53:54.000000 getdaft-0.1.8/src/lib.rs
+-rw-r--r--   0      501       20        0 2023-07-05 18:53:54.000000 getdaft-0.1.8/tests/__init__.py
+-rw-r--r--   0      501       20      299 2023-07-05 18:53:54.000000 getdaft-0.1.8/tests/assets/__init__.py
+-rw-r--r--   0      501       20      544 2023-07-05 18:53:54.000000 getdaft-0.1.8/tests/assets/tpch-sqlite-queries/1.sql
+-rw-r--r--   0      501       20      542 2023-07-05 18:53:54.000000 getdaft-0.1.8/tests/assets/tpch-sqlite-queries/10.sql
+-rw-r--r--   0      501       20      703 2023-07-05 18:53:54.000000 getdaft-0.1.8/tests/assets/tpch-sqlite-queries/2.sql
+-rw-r--r--   0      501       20      444 2023-07-05 18:53:54.000000 getdaft-0.1.8/tests/assets/tpch-sqlite-queries/3.sql
+-rw-r--r--   0      501       20      371 2023-07-05 18:53:54.000000 getdaft-0.1.8/tests/assets/tpch-sqlite-queries/4.sql
+-rw-r--r--   0      501       20      504 2023-07-05 18:53:54.000000 getdaft-0.1.8/tests/assets/tpch-sqlite-queries/5.sql
+-rw-r--r--   0      501       20      259 2023-07-05 18:53:54.000000 getdaft-0.1.8/tests/assets/tpch-sqlite-queries/6.sql
+-rw-r--r--   0      501       20      834 2023-07-05 18:53:54.000000 getdaft-0.1.8/tests/assets/tpch-sqlite-queries/7.sql
+-rw-r--r--   0      501       20      815 2023-07-05 18:53:54.000000 getdaft-0.1.8/tests/assets/tpch-sqlite-queries/8.sql
+-rw-r--r--   0      501       20      627 2023-07-05 18:53:54.000000 getdaft-0.1.8/tests/assets/tpch-sqlite-queries/9.sql
+-rw-r--r--   0      501       20       48 2023-07-05 18:53:54.000000 getdaft-0.1.8/tests/assets/tpch-sqlite-queries/README.md
+-rw-r--r--   0      501       20      604 2023-07-05 18:53:54.000000 getdaft-0.1.8/tests/benchmarks/conftest.py
+-rw-r--r--   0      501       20     1227 2023-07-05 18:53:54.000000 getdaft-0.1.8/tests/benchmarks/test_df_arithmetic.py
+-rw-r--r--   0      501       20     2706 2023-07-05 18:53:54.000000 getdaft-0.1.8/tests/benchmarks/test_file_read.py
+-rw-r--r--   0      501       20     5604 2023-07-05 18:53:54.000000 getdaft-0.1.8/tests/benchmarks/test_groups_and_aggs.py
+-rw-r--r--   0      501       20     7292 2023-07-05 18:53:54.000000 getdaft-0.1.8/tests/benchmarks/test_join.py
+-rw-r--r--   0      501       20     2603 2023-07-05 18:53:54.000000 getdaft-0.1.8/tests/benchmarks/test_repartition.py
+-rw-r--r--   0      501       20     4005 2023-07-05 18:53:54.000000 getdaft-0.1.8/tests/benchmarks/test_sort.py
+-rw-r--r--   0      501       20     2911 2023-07-05 18:53:54.000000 getdaft-0.1.8/tests/conftest.py
+-rw-r--r--   0      501       20        0 2023-07-05 18:53:54.000000 getdaft-0.1.8/tests/cookbook/__init__.py
+-rw-r--r--   0      501       20    13229 2023-07-05 18:53:54.000000 getdaft-0.1.8/tests/cookbook/assets/311-service-requests.24.csv
+-rw-r--r--   0      501       20      255 2023-07-05 18:53:54.000000 getdaft-0.1.8/tests/cookbook/assets/__init__.py
+-rw-r--r--   0      501       20      924 2023-07-05 18:53:54.000000 getdaft-0.1.8/tests/cookbook/assets/images/0000.jpg
+-rw-r--r--   0      501       20      941 2023-07-05 18:53:54.000000 getdaft-0.1.8/tests/cookbook/assets/images/0007.jpg
+-rw-r--r--   0      501       20     2740 2023-07-05 18:53:54.000000 getdaft-0.1.8/tests/cookbook/assets/images/0018.png
+-rw-r--r--   0      501       20     7462 2023-07-05 18:53:54.000000 getdaft-0.1.8/tests/cookbook/assets/images/0025.tiff
+-rw-r--r--   0      501       20      882 2023-07-05 18:53:54.000000 getdaft-0.1.8/tests/cookbook/conftest.py
+-rw-r--r--   0      501       20     9268 2023-07-05 18:53:54.000000 getdaft-0.1.8/tests/cookbook/test_aggregations.py
+-rw-r--r--   0      501       20     2979 2023-07-05 18:53:54.000000 getdaft-0.1.8/tests/cookbook/test_computations.py
+-rw-r--r--   0      501       20     1798 2023-07-05 18:53:54.000000 getdaft-0.1.8/tests/cookbook/test_count_rows.py
+-rw-r--r--   0      501       20     7099 2023-07-05 18:53:54.000000 getdaft-0.1.8/tests/cookbook/test_dataloading.py
+-rw-r--r--   0      501       20      800 2023-07-05 18:53:54.000000 getdaft-0.1.8/tests/cookbook/test_distinct.py
+-rw-r--r--   0      501       20     6049 2023-07-05 18:53:54.000000 getdaft-0.1.8/tests/cookbook/test_filter.py
+-rw-r--r--   0      501       20     2930 2023-07-05 18:53:54.000000 getdaft-0.1.8/tests/cookbook/test_image.py
+-rw-r--r--   0      501       20     3810 2023-07-05 18:53:54.000000 getdaft-0.1.8/tests/cookbook/test_joins.py
+-rw-r--r--   0      501       20     2878 2023-07-05 18:53:54.000000 getdaft-0.1.8/tests/cookbook/test_literals.py
+-rw-r--r--   0      501       20    10311 2023-07-05 18:53:54.000000 getdaft-0.1.8/tests/cookbook/test_pandas_cookbook.py
+-rw-r--r--   0      501       20     4148 2023-07-05 18:53:54.000000 getdaft-0.1.8/tests/cookbook/test_sorting.py
+-rw-r--r--   0      501       20     1497 2023-07-05 18:53:54.000000 getdaft-0.1.8/tests/cookbook/test_write.py
+-rw-r--r--   0      501       20        0 2023-07-05 18:53:54.000000 getdaft-0.1.8/tests/dataframe/__init__.py
+-rw-r--r--   0      501       20      751 2023-07-05 18:53:54.000000 getdaft-0.1.8/tests/dataframe/conftest.py
+-rw-r--r--   0      501       20      805 2023-07-05 18:53:54.000000 getdaft-0.1.8/tests/dataframe/test_accessors.py
+-rw-r--r--   0      501       20    10308 2023-07-05 18:53:54.000000 getdaft-0.1.8/tests/dataframe/test_aggregations.py
+-rw-r--r--   0      501       20      472 2023-07-05 18:53:54.000000 getdaft-0.1.8/tests/dataframe/test_concat.py
+-rw-r--r--   0      501       20    26635 2023-07-05 18:53:54.000000 getdaft-0.1.8/tests/dataframe/test_creation.py
+-rw-r--r--   0      501       20     1824 2023-07-05 18:53:54.000000 getdaft-0.1.8/tests/dataframe/test_distinct.py
+-rw-r--r--   0      501       20     1428 2023-07-05 18:53:54.000000 getdaft-0.1.8/tests/dataframe/test_explode.py
+-rw-r--r--   0      501       20     1097 2023-07-05 18:53:54.000000 getdaft-0.1.8/tests/dataframe/test_filter.py
+-rw-r--r--   0      501       20     2435 2023-07-05 18:53:54.000000 getdaft-0.1.8/tests/dataframe/test_getitem.py
+-rw-r--r--   0      501       20     3205 2023-07-05 18:53:54.000000 getdaft-0.1.8/tests/dataframe/test_iter.py
+-rw-r--r--   0      501       20     4091 2023-07-05 18:53:54.000000 getdaft-0.1.8/tests/dataframe/test_joins.py
+-rw-r--r--   0      501       20     2253 2023-07-05 18:53:54.000000 getdaft-0.1.8/tests/dataframe/test_logical_type.py
+-rw-r--r--   0      501       20      223 2023-07-05 18:53:54.000000 getdaft-0.1.8/tests/dataframe/test_repartition.py
+-rw-r--r--   0      501       20     8608 2023-07-05 18:53:54.000000 getdaft-0.1.8/tests/dataframe/test_repr.py
+-rw-r--r--   0      501       20      815 2023-07-05 18:53:54.000000 getdaft-0.1.8/tests/dataframe/test_select.py
+-rw-r--r--   0      501       20      656 2023-07-05 18:53:54.000000 getdaft-0.1.8/tests/dataframe/test_show.py
+-rw-r--r--   0      501       20     6364 2023-07-05 18:53:54.000000 getdaft-0.1.8/tests/dataframe/test_sort.py
+-rw-r--r--   0      501       20     7542 2023-07-05 18:53:54.000000 getdaft-0.1.8/tests/dataframe/test_temporals.py
+-rw-r--r--   0      501       20     2385 2023-07-05 18:53:54.000000 getdaft-0.1.8/tests/dataframe/test_to_integrations.py
+-rw-r--r--   0      501       20      850 2023-07-05 18:53:54.000000 getdaft-0.1.8/tests/dataframe/test_with_column.py
+-rw-r--r--   0      501       20        0 2023-07-05 18:53:54.000000 getdaft-0.1.8/tests/expressions/__init__.py
+-rw-r--r--   0      501       20     1417 2023-07-05 18:53:54.000000 getdaft-0.1.8/tests/expressions/test_apply.py
+-rw-r--r--   0      501       20     3533 2023-07-05 18:53:54.000000 getdaft-0.1.8/tests/expressions/test_expressions.py
+-rw-r--r--   0      501       20     4259 2023-07-05 18:53:54.000000 getdaft-0.1.8/tests/expressions/test_expressions_projection.py
+-rw-r--r--   0      501       20     5019 2023-07-05 18:53:54.000000 getdaft-0.1.8/tests/expressions/test_udf.py
+-rw-r--r--   0      501       20        0 2023-07-05 18:53:54.000000 getdaft-0.1.8/tests/expressions/typing/__init__.py
+-rw-r--r--   0      501       20     6290 2023-07-05 18:53:54.000000 getdaft-0.1.8/tests/expressions/typing/conftest.py
+-rw-r--r--   0      501       20     1363 2023-07-05 18:53:54.000000 getdaft-0.1.8/tests/expressions/typing/test_aggs.py
+-rw-r--r--   0      501       20     2335 2023-07-05 18:53:54.000000 getdaft-0.1.8/tests/expressions/typing/test_arithmetic.py
+-rw-r--r--   0      501       20      853 2023-07-05 18:53:54.000000 getdaft-0.1.8/tests/expressions/typing/test_compare.py
+-rw-r--r--   0      501       20      792 2023-07-05 18:53:54.000000 getdaft-0.1.8/tests/expressions/typing/test_dt.py
+-rw-r--r--   0      501       20      531 2023-07-05 18:53:54.000000 getdaft-0.1.8/tests/expressions/typing/test_float.py
+-rw-r--r--   0      501       20      684 2023-07-05 18:53:54.000000 getdaft-0.1.8/tests/expressions/typing/test_if_else.py
+-rw-r--r--   0      501       20      422 2023-07-05 18:53:54.000000 getdaft-0.1.8/tests/expressions/typing/test_is_null.py
+-rw-r--r--   0      501       20     1176 2023-07-05 18:53:54.000000 getdaft-0.1.8/tests/expressions/typing/test_logical.py
+-rw-r--r--   0      501       20     1544 2023-07-05 18:53:54.000000 getdaft-0.1.8/tests/expressions/typing/test_str.py
+-rw-r--r--   0      501       20        0 2023-07-05 18:53:54.000000 getdaft-0.1.8/tests/integration/__init__.py
+-rw-r--r--   0      501       20       91 2023-07-05 18:53:54.000000 getdaft-0.1.8/tests/integration/docker-compose/Dockerfile.nginx
+-rw-r--r--   0      501       20      699 2023-07-05 18:53:54.000000 getdaft-0.1.8/tests/integration/docker-compose/docker-compose.yml
+-rw-r--r--   0      501       20     1007 2023-07-05 18:53:54.000000 getdaft-0.1.8/tests/integration/docker-compose/nginx-serve-static-files.conf
+-rw-r--r--   0      501       20        0 2023-07-05 18:53:54.000000 getdaft-0.1.8/tests/integration/io/__init__.py
+-rw-r--r--   0      501       20     2902 2023-07-05 18:53:54.000000 getdaft-0.1.8/tests/integration/io/conftest.py
+-rw-r--r--   0      501       20     2242 2023-07-05 18:53:54.000000 getdaft-0.1.8/tests/integration/io/test_url_download_http.py
+-rw-r--r--   0      501       20     1829 2023-07-05 18:53:54.000000 getdaft-0.1.8/tests/integration/io/test_url_download_local.py
+-rw-r--r--   0      501       20     1780 2023-07-05 18:53:54.000000 getdaft-0.1.8/tests/integration/io/test_url_download_public_aws_s3.py
+-rw-r--r--   0      501       20     1062 2023-07-05 18:53:54.000000 getdaft-0.1.8/tests/integration/io/test_url_download_s3_minio.py
+-rw-r--r--   0      501       20     4343 2023-07-05 18:53:54.000000 getdaft-0.1.8/tests/integration/test_tpch.py
+-rw-r--r--   0      501       20        0 2023-07-05 18:53:54.000000 getdaft-0.1.8/tests/optimizer/__init__.py
+-rw-r--r--   0      501       20     1116 2023-07-05 18:53:54.000000 getdaft-0.1.8/tests/optimizer/conftest.py
+-rw-r--r--   0      501       20     1666 2023-07-05 18:53:54.000000 getdaft-0.1.8/tests/optimizer/test_drop_projections.py
+-rw-r--r--   0      501       20     1847 2023-07-05 18:53:54.000000 getdaft-0.1.8/tests/optimizer/test_drop_repartition.py
+-rw-r--r--   0      501       20     2463 2023-07-05 18:53:54.000000 getdaft-0.1.8/tests/optimizer/test_fold_projections.py
+-rw-r--r--   0      501       20     8050 2023-07-05 18:53:54.000000 getdaft-0.1.8/tests/optimizer/test_prune_columns.py
+-rw-r--r--   0      501       20     3597 2023-07-05 18:53:54.000000 getdaft-0.1.8/tests/optimizer/test_pushdown_clauses_into_scan.py
+-rw-r--r--   0      501       20     1170 2023-07-05 18:53:54.000000 getdaft-0.1.8/tests/optimizer/test_pushdown_limit.py
+-rw-r--r--   0      501       20     8981 2023-07-05 18:53:54.000000 getdaft-0.1.8/tests/optimizer/test_pushdown_predicates.py
+-rw-r--r--   0      501       20        0 2023-07-05 18:53:54.000000 getdaft-0.1.8/tests/property_based_testing/__init__.py
+-rw-r--r--   0      501       20     4575 2023-07-05 18:53:54.000000 getdaft-0.1.8/tests/property_based_testing/strategies.py
+-rw-r--r--   0      501       20     8895 2023-07-05 18:53:54.000000 getdaft-0.1.8/tests/property_based_testing/test_sort.py
+-rw-r--r--   0      501       20        0 2023-07-05 18:53:54.000000 getdaft-0.1.8/tests/ray/__init__.py
+-rw-r--r--   0      501       20     5375 2023-07-05 18:53:54.000000 getdaft-0.1.8/tests/ray/test_dask.py
+-rw-r--r--   0      501       20     8864 2023-07-05 18:53:54.000000 getdaft-0.1.8/tests/ray/test_datasets.py
+-rw-r--r--   0      501       20      278 2023-07-05 18:53:54.000000 getdaft-0.1.8/tests/series/__init__.py
+-rw-r--r--   0      501       20     9299 2023-07-05 18:53:54.000000 getdaft-0.1.8/tests/series/test_arithmetic.py
+-rw-r--r--   0      501       20    15034 2023-07-05 18:53:54.000000 getdaft-0.1.8/tests/series/test_cast.py
+-rw-r--r--   0      501       20    17207 2023-07-05 18:53:54.000000 getdaft-0.1.8/tests/series/test_comparisons.py
+-rw-r--r--   0      501       20     7188 2023-07-05 18:53:54.000000 getdaft-0.1.8/tests/series/test_concat.py
+-rw-r--r--   0      501       20      896 2023-07-05 18:53:54.000000 getdaft-0.1.8/tests/series/test_embedding.py
+-rw-r--r--   0      501       20     6151 2023-07-05 18:53:54.000000 getdaft-0.1.8/tests/series/test_filter.py
+-rw-r--r--   0      501       20      874 2023-07-05 18:53:54.000000 getdaft-0.1.8/tests/series/test_float.py
+-rw-r--r--   0      501       20     3344 2023-07-05 18:53:54.000000 getdaft-0.1.8/tests/series/test_hash.py
+-rw-r--r--   0      501       20    21522 2023-07-05 18:53:54.000000 getdaft-0.1.8/tests/series/test_if_else.py
+-rw-r--r--   0      501       20    22626 2023-07-05 18:53:54.000000 getdaft-0.1.8/tests/series/test_image.py
+-rw-r--r--   0      501       20      889 2023-07-05 18:53:54.000000 getdaft-0.1.8/tests/series/test_numeric_ops.py
+-rw-r--r--   0      501       20     3418 2023-07-05 18:53:54.000000 getdaft-0.1.8/tests/series/test_series.py
+-rw-r--r--   0      501       20     9173 2023-07-05 18:53:54.000000 getdaft-0.1.8/tests/series/test_size_bytes.py
+-rw-r--r--   0      501       20     2188 2023-07-05 18:53:54.000000 getdaft-0.1.8/tests/series/test_slice.py
+-rw-r--r--   0      501       20     5495 2023-07-05 18:53:54.000000 getdaft-0.1.8/tests/series/test_sort.py
+-rw-r--r--   0      501       20     6111 2023-07-05 18:53:54.000000 getdaft-0.1.8/tests/series/test_take.py
+-rw-r--r--   0      501       20     1934 2023-07-05 18:53:54.000000 getdaft-0.1.8/tests/series/test_temporal_ops.py
+-rw-r--r--   0      501       20     4413 2023-07-05 18:53:54.000000 getdaft-0.1.8/tests/series/test_utf8_ops.py
+-rw-r--r--   0      501       20      694 2023-07-05 18:53:54.000000 getdaft-0.1.8/tests/table/__init__.py
+-rw-r--r--   0      501       20        0 2023-07-05 18:53:54.000000 getdaft-0.1.8/tests/table/list/__init__.py
+-rw-r--r--   0      501       20     1156 2023-07-05 18:53:54.000000 getdaft-0.1.8/tests/table/list/test_list_join.py
+-rw-r--r--   0      501       20        0 2023-07-05 18:53:54.000000 getdaft-0.1.8/tests/table/table_io/__init__.py
+-rw-r--r--   0      501       20     6289 2023-07-05 18:53:54.000000 getdaft-0.1.8/tests/table/table_io/test_csv.py
+-rw-r--r--   0      501       20     4355 2023-07-05 18:53:54.000000 getdaft-0.1.8/tests/table/table_io/test_json.py
+-rw-r--r--   0      501       20     4778 2023-07-05 18:53:54.000000 getdaft-0.1.8/tests/table/table_io/test_parquet.py
+-rw-r--r--   0      501       20     2100 2023-07-05 18:53:54.000000 getdaft-0.1.8/tests/table/table_io/test_read_time_cast.py
+-rw-r--r--   0      501       20     1070 2023-07-05 18:53:54.000000 getdaft-0.1.8/tests/table/test_blackbox_kernels.py
+-rw-r--r--   0      501       20      426 2023-07-05 18:53:54.000000 getdaft-0.1.8/tests/table/test_broadcasts.py
+-rw-r--r--   0      501       20     2123 2023-07-05 18:53:54.000000 getdaft-0.1.8/tests/table/test_concat.py
+-rw-r--r--   0      501       20     4900 2023-07-05 18:53:54.000000 getdaft-0.1.8/tests/table/test_eval.py
+-rw-r--r--   0      501       20     3930 2023-07-05 18:53:54.000000 getdaft-0.1.8/tests/table/test_explodes.py
+-rw-r--r--   0      501       20     7413 2023-07-05 18:53:54.000000 getdaft-0.1.8/tests/table/test_filter.py
+-rw-r--r--   0      501       20    23530 2023-07-05 18:53:54.000000 getdaft-0.1.8/tests/table/test_from_py.py
+-rw-r--r--   0      501       20      842 2023-07-05 18:53:54.000000 getdaft-0.1.8/tests/table/test_head.py
+-rw-r--r--   0      501       20    10974 2023-07-05 18:53:54.000000 getdaft-0.1.8/tests/table/test_joins.py
+-rw-r--r--   0      501       20     7811 2023-07-05 18:53:54.000000 getdaft-0.1.8/tests/table/test_partitioning.py
+-rw-r--r--   0      501       20      654 2023-07-05 18:53:54.000000 getdaft-0.1.8/tests/table/test_size_bytes.py
+-rw-r--r--   0      501       20    10955 2023-07-05 18:53:54.000000 getdaft-0.1.8/tests/table/test_sorting.py
+-rw-r--r--   0      501       20    20923 2023-07-05 18:53:54.000000 getdaft-0.1.8/tests/table/test_table_aggs.py
+-rw-r--r--   0      501       20     5061 2023-07-05 18:53:54.000000 getdaft-0.1.8/tests/table/test_take.py
+-rw-r--r--   0      501       20        0 2023-07-05 18:53:54.000000 getdaft-0.1.8/tests/table/utf8/__init__.py
+-rw-r--r--   0      501       20     1165 2023-07-05 18:53:54.000000 getdaft-0.1.8/tests/table/utf8/test_compares.py
+-rw-r--r--   0      501       20      321 2023-07-05 18:53:54.000000 getdaft-0.1.8/tests/table/utf8/test_length.py
+-rw-r--r--   0      501       20     3533 2023-07-05 18:53:54.000000 getdaft-0.1.8/tests/test_analytics.py
+-rw-r--r--   0      501       20      703 2023-07-05 18:53:54.000000 getdaft-0.1.8/tests/test_datatypes.py
+-rw-r--r--   0      501       20     3653 2023-07-05 18:53:54.000000 getdaft-0.1.8/tests/test_schema.py
+-rw-r--r--   0      501       20        0 2023-07-05 18:53:54.000000 getdaft-0.1.8/tests/udf_library/__init__.py
+-rw-r--r--   0      501       20     4508 2023-07-05 18:53:54.000000 getdaft-0.1.8/tests/udf_library/test_url_udfs.py
+-rw-r--r--   0      501       20      338 2023-07-05 18:53:54.000000 getdaft-0.1.8/tests/utils.py
+-rw-r--r--   0      501       20        0 2023-07-05 18:53:54.000000 getdaft-0.1.8/tests_legacy/__init__.py
+-rw-r--r--   0      501       20     6988 2023-07-05 18:53:54.000000 getdaft-0.1.8/tests_legacy/test_resource_requests.py
+-rw-r--r--   0      501       20        0 2023-07-05 18:53:54.000000 getdaft-0.1.8/tools/__init__.py
+-rw-r--r--   0      501       20     1633 2023-07-05 18:53:54.000000 getdaft-0.1.8/tools/patch_package_version.py
+-rw-r--r--   0      501       20        0 2023-07-05 18:53:54.000000 getdaft-0.1.8/tools/wheels/__init__.py
+-rw-r--r--   0      501       20        0 2023-07-05 18:53:54.000000 getdaft-0.1.8/tools/wheels/_vendor/__init__.py
+-rw-r--r--   0      501       20     1125 2023-07-05 18:53:54.000000 getdaft-0.1.8/tools/wheels/_vendor/wheel/LICENSE.txt
+-rw-r--r--   0      501       20       59 2023-07-05 18:53:54.000000 getdaft-0.1.8/tools/wheels/_vendor/wheel/__init__.py
+-rw-r--r--   0      501       20     2499 2023-07-05 18:53:54.000000 getdaft-0.1.8/tools/wheels/_vendor/wheel/cli/__init__.py
+-rw-r--r--   0      501       20     9514 2023-07-05 18:53:54.000000 getdaft-0.1.8/tools/wheels/_vendor/wheel/cli/convert.py
+-rw-r--r--   0      501       20     3113 2023-07-05 18:53:54.000000 getdaft-0.1.8/tools/wheels/_vendor/wheel/cli/pack.py
+-rw-r--r--   0      501       20      662 2023-07-05 18:53:54.000000 getdaft-0.1.8/tools/wheels/_vendor/wheel/cli/unpack.py
+-rw-r--r--   0      501       20     1246 2023-07-05 18:53:54.000000 getdaft-0.1.8/tools/wheels/_vendor/wheel/pkginfo.py
+-rw-r--r--   0      501       20      974 2023-07-05 18:53:54.000000 getdaft-0.1.8/tools/wheels/_vendor/wheel/util.py
+-rw-r--r--   0      501       20     7125 2023-07-05 18:53:54.000000 getdaft-0.1.8/tools/wheels/_vendor/wheel/wheelfile.py
+-rw-r--r--   0      501       20      878 2023-07-05 18:53:54.000000 getdaft-0.1.8/tools/wheels/fix-and-copy-wheel.py
+-rw-r--r--   0      501       20     2981 2023-07-05 18:53:54.000000 getdaft-0.1.8/tools/wheels/tmpdirs.py
+-rw-r--r--   0      501       20     4469 2023-07-05 18:53:54.000000 getdaft-0.1.8/tools/wheels/tools.py
+-rw-r--r--   0      501       20     9484 2023-07-05 18:53:54.000000 getdaft-0.1.8/tools/wheels/wheeltools.py
+-rw-r--r--   0      501       20       19 2023-07-05 18:53:54.000000 getdaft-0.1.8/tutorials/.gitignore
+-rw-r--r--   0      501       20    19755 2023-07-05 18:53:54.000000 getdaft-0.1.8/tutorials/embeddings/daft_tutorial_embeddings_stackexchange.ipynb
+-rw-r--r--   0      501       20    12692 2023-07-05 18:53:54.000000 getdaft-0.1.8/tutorials/image_querying/top_n_red_color.ipynb
+-rw-r--r--   0      501       20    98730 2023-07-05 18:53:54.000000 getdaft-0.1.8/tutorials/mnist.ipynb
+-rw-r--r--   0      501       20    11690 2023-07-05 18:53:54.000000 getdaft-0.1.8/tutorials/text_to_image/text_to_image_generation.ipynb
+-rw-r--r--   0      501       20     9134 2023-07-05 18:53:54.000000 getdaft-0.1.8/tutorials/text_to_image/using_cloud_with_ray.ipynb
+-rw-r--r--   0      501       20    74387 2023-07-05 18:54:55.000000 getdaft-0.1.8/Cargo.lock
+-rw-r--r--   0        0        0    10000 1970-01-01 00:00:00.000000 getdaft-0.1.8/PKG-INFO
```

### Comparing `getdaft-0.1.7/local_dependencies/daft-io/Cargo.toml` & `getdaft-0.1.8/local_dependencies/daft-io/Cargo.toml`

 * *Files 7% similar despite different names*

```diff
@@ -1,12 +1,14 @@
 [dependencies]
 async-trait = "0.1.68"
 aws-config = {version = "0.55.3"}
 aws-credential-types = {version = "0.55.3", features = ["hardcoded-credentials"]}
 aws-sdk-s3 = "0.28.0"
+aws-sig-auth = "0.55.3"
+aws-sigv4 = "0.55.3"
 bytes = "1.4.0"
 common-error = {path = "../common-error", default-features = false}
 daft-core = {path = "../daft-core", default-features = false}
 futures = "0.3.28"
 snafu = "0.7.4"
 tokio = {version = "1.28.2", features = ["net", "time", "bytes", "process", "signal", "macros", "rt", "rt-multi-thread"]}
 url = "2.4.0"
```

### Comparing `getdaft-0.1.7/local_dependencies/daft-io/src/config.rs` & `getdaft-0.1.8/local_dependencies/daft-io/src/config.rs`

 * *Files 7% similar despite different names*

```diff
@@ -5,14 +5,15 @@
 use serde::Serialize;
 #[derive(Clone, Default, Debug, Serialize, Deserialize, PartialEq, Eq, Hash)]
 pub struct S3Config {
     pub region_name: Option<String>,
     pub endpoint_url: Option<String>,
     pub key_id: Option<String>,
     pub access_key: Option<String>,
+    pub anonymous: bool,
 }
 
 #[derive(Clone, Default, Debug, Serialize, Deserialize, PartialEq, Eq, Hash)]
 pub struct IOConfig {
     pub s3: S3Config,
 }
 
@@ -20,16 +21,17 @@
     fn fmt(&self, f: &mut Formatter<'_>) -> std::result::Result<(), std::fmt::Error> {
         write!(
             f,
             "S3Config
     region_name: {:?}
     endpoint_url: {:?}
     key_id: {:?}
-    access_key: {:?}",
-            self.region_name, self.endpoint_url, self.key_id, self.access_key
+    access_key: {:?}
+    anonymous: {}",
+            self.region_name, self.endpoint_url, self.key_id, self.access_key, self.anonymous
         )
     }
 }
 
 impl Display for IOConfig {
     fn fmt(&self, f: &mut Formatter<'_>) -> std::result::Result<(), std::fmt::Error> {
         write!(
```

### Comparing `getdaft-0.1.7/local_dependencies/daft-io/src/lib.rs` & `getdaft-0.1.8/local_dependencies/daft-io/src/lib.rs`

 * *Files 7% similar despite different names*

```diff
@@ -9,22 +9,15 @@
 #[cfg(feature = "python")]
 pub mod python;
 
 use config::IOConfig;
 #[cfg(feature = "python")]
 pub use python::register_modules;
 
-use lazy_static::lazy_static;
-
-use std::{
-    borrow::Cow,
-    collections::HashMap,
-    hash::Hash,
-    sync::{Arc, RwLock},
-};
+use std::{borrow::Cow, hash::Hash, ops::Range, sync::Arc};
 
 use futures::{StreamExt, TryStreamExt};
 
 use snafu::Snafu;
 use url::ParseError;
 
 use snafu::prelude::*;
@@ -65,18 +58,27 @@
     },
 
     #[snafu(display("Unable to convert URL \"{}\" to path", path))]
     InvalidUrl {
         path: String,
         source: url::ParseError,
     },
+
     #[snafu(display("Not a File: \"{}\"", path))]
     NotAFile { path: String },
+
+    #[snafu(display("Unable to load Credentials for store: {store} {source}"))]
+    UnableToLoadCredentials { store: SourceType, source: DynError },
+
+    #[snafu(display("Failed to load Credentials for store: {store} {source}"))]
+    UnableToCreateClient { store: SourceType, source: DynError },
+
     #[snafu(display("Source not yet implemented: {}", store))]
     NotImplementedSource { store: String },
+
     #[snafu(display("Error joining spawned task: {}", source), context(false))]
     JoinError { source: tokio::task::JoinError },
 }
 
 impl From<Error> for DaftError {
     fn from(err: Error) -> DaftError {
         use Error::*;
@@ -85,38 +87,20 @@
             _ => DaftError::External(err.into()),
         }
     }
 }
 
 type Result<T, E = Error> = std::result::Result<T, E>;
 
-lazy_static! {
-    static ref OBJ_SRC_MAP: RwLock<HashMap<(SourceType, IOConfig), Arc<dyn ObjectSource>>> =
-        RwLock::new(HashMap::new());
-}
-
 async fn get_source(source_type: SourceType, config: &IOConfig) -> Result<Arc<dyn ObjectSource>> {
-    let key = (source_type.clone(), config.clone());
-    {
-        if let Some(source) = OBJ_SRC_MAP.read().unwrap().get(&key) {
-            return Ok(source.clone());
-        }
-    }
-
-    let new_source: Arc<dyn ObjectSource> = match source_type {
-        SourceType::File => Arc::new(LocalSource::new().await) as Arc<dyn ObjectSource>,
-        SourceType::Http => Arc::new(HttpSource::new().await) as Arc<dyn ObjectSource>,
-        SourceType::S3 => Arc::new(S3LikeSource::new(&config.s3).await) as Arc<dyn ObjectSource>,
-    };
-
-    let mut w_handle = OBJ_SRC_MAP.write().unwrap();
-    if w_handle.get(&key).is_none() {
-        w_handle.insert(key, new_source.clone());
-    }
-    Ok(new_source)
+    Ok(match source_type {
+        SourceType::File => LocalSource::get_client().await? as Arc<dyn ObjectSource>,
+        SourceType::Http => HttpSource::get_client().await? as Arc<dyn ObjectSource>,
+        SourceType::S3 => S3LikeSource::get_client(&config.s3).await? as Arc<dyn ObjectSource>,
+    })
 }
 
 #[derive(Debug, Hash, PartialEq, std::cmp::Eq, Clone, Copy)]
 pub(crate) enum SourceType {
     File,
     Http,
     S3,
@@ -150,28 +134,32 @@
         "file" => Ok((SourceType::File, fixed_input)),
         "http" | "https" => Ok((SourceType::Http, fixed_input)),
         "s3" => Ok((SourceType::S3, fixed_input)),
         _ => Err(Error::NotImplementedSource { store: scheme }),
     }
 }
 
-async fn single_url_get(input: String, config: &IOConfig) -> Result<GetResult> {
+async fn single_url_get(
+    input: String,
+    range: Option<Range<usize>>,
+    config: &IOConfig,
+) -> Result<GetResult> {
     let (scheme, path) = parse_url(&input)?;
     let source = get_source(scheme, config).await?;
-    source.get(path.as_ref()).await
+    source.get(path.as_ref(), range).await
 }
 
 async fn single_url_download(
     index: usize,
     input: Option<String>,
     raise_error_on_failure: bool,
     config: Arc<IOConfig>,
 ) -> Result<Option<bytes::Bytes>> {
     let value = if let Some(input) = input {
-        let response = single_url_get(input, config.as_ref()).await;
+        let response = single_url_get(input, None, config.as_ref()).await;
         let res = match response {
             Ok(res) => res.bytes().await,
             Err(err) => Err(err),
         };
         Some(res)
     } else {
         None
```

### Comparing `getdaft-0.1.7/local_dependencies/daft-io/src/object_io.rs` & `getdaft-0.1.8/local_dependencies/daft-io/src/object_io.rs`

 * *Files 16% similar despite different names*

```diff
@@ -1,18 +1,19 @@
+use std::ops::Range;
 use std::path::PathBuf;
 
 use async_trait::async_trait;
 use bytes::Bytes;
 use futures::stream::{BoxStream, Stream};
 use futures::StreamExt;
 
-use crate::local::collect_file;
+use crate::local::{collect_file, LocalFile};
 
 pub(crate) enum GetResult {
-    File(PathBuf),
+    File(LocalFile),
     Stream(BoxStream<'static, super::Result<Bytes>>, Option<usize>),
 }
 
 async fn collect_bytes<S>(mut stream: S, size_hint: Option<usize>) -> super::Result<Bytes>
 where
     S: Stream<Item = super::Result<Bytes>> + Send + Unpin,
 {
@@ -35,17 +36,20 @@
     }
 }
 
 impl GetResult {
     pub async fn bytes(self) -> super::Result<Bytes> {
         use GetResult::*;
         match self {
-            File(path) => collect_file(path.to_str().unwrap()).await,
+            File(f) => collect_file(f).await,
             Stream(stream, size) => collect_bytes(stream, size).await,
         }
     }
 }
 
 #[async_trait]
 pub(crate) trait ObjectSource: Sync + Send {
-    async fn get(&self, uri: &str) -> super::Result<GetResult>;
+    async fn get(&self, uri: &str, range: Option<Range<usize>>) -> super::Result<GetResult>;
+    async fn get_range(&self, uri: &str, range: Range<usize>) -> super::Result<GetResult> {
+        self.get(uri, Some(range)).await
+    }
 }
```

### Comparing `getdaft-0.1.7/local_dependencies/daft-io/src/python.rs` & `getdaft-0.1.8/local_dependencies/daft-io/src/python.rs`

 * *Files 24% similar despite different names*

```diff
@@ -19,41 +19,71 @@
     pub fn new(s3: Option<PyS3Config>) -> Self {
         PyIOConfig {
             config: IOConfig {
                 s3: s3.unwrap_or_default().config,
             },
         }
     }
+
     pub fn __repr__(&self) -> PyResult<String> {
         Ok(format!("{}", self.config))
     }
+
+    #[getter]
+    pub fn s3(&self) -> PyResult<PyS3Config> {
+        Ok(PyS3Config {
+            config: self.config.s3.clone(),
+        })
+    }
 }
 
 #[pymethods]
 impl PyS3Config {
     #[new]
     pub fn new(
         region_name: Option<String>,
         endpoint_url: Option<String>,
         key_id: Option<String>,
         access_key: Option<String>,
+        anonymous: Option<bool>,
     ) -> Self {
         PyS3Config {
             config: S3Config {
                 region_name,
                 endpoint_url,
                 key_id,
                 access_key,
+                anonymous: anonymous.unwrap_or(false),
             },
         }
     }
 
     pub fn __repr__(&self) -> PyResult<String> {
         Ok(format!("{}", self.config))
     }
+
+    #[getter]
+    pub fn region_name(&self) -> PyResult<Option<String>> {
+        Ok(self.config.region_name.clone())
+    }
+
+    #[getter]
+    pub fn endpoint_url(&self) -> PyResult<Option<String>> {
+        Ok(self.config.endpoint_url.clone())
+    }
+
+    #[getter]
+    pub fn key_id(&self) -> PyResult<Option<String>> {
+        Ok(self.config.key_id.clone())
+    }
+
+    #[getter]
+    pub fn access_key(&self) -> PyResult<Option<String>> {
+        Ok(self.config.access_key.clone())
+    }
 }
 
 pub fn register_modules(_py: Python, parent: &PyModule) -> PyResult<()> {
     parent.add_class::<PyS3Config>()?;
     parent.add_class::<PyIOConfig>()?;
     Ok(())
 }
```

### Comparing `getdaft-0.1.7/local_dependencies/common-error/Cargo.toml` & `getdaft-0.1.8/local_dependencies/common-error/Cargo.toml`

 * *Files 18% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 [dependencies]
-serde_json = "1.0.96"
+serde_json = "1.0.99"
 
 [features]
 default = ["python"]
 python = ["dep:pyo3"]
 
 [package]
 edition = "2021"
```

### Comparing `getdaft-0.1.7/local_dependencies/common-error/src/error.rs` & `getdaft-0.1.8/local_dependencies/common-error/src/error.rs`

 * *Files identical despite different names*

### Comparing `getdaft-0.1.7/local_dependencies/daft-core/Cargo.toml` & `getdaft-0.1.8/local_dependencies/daft-core/Cargo.toml`

 * *Files 2% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 fnv = "1.0.7"
 html-escape = "0.2.13"
 ndarray = "0.15.6"
 num-derive = "0.3.3"
 num-traits = "0.2"
 prettytable-rs = "0.10"
 rand = "^0.8"
-serde_json = "1.0.96"
+serde_json = "1.0.99"
 
 [dependencies.image]
 default-features = false
 features = ["gif", "jpeg", "ico", "png", "tiff", "webp", "bmp", "hdr"]
 version = "0.24.6"
 
 [dependencies.indexmap]
```

### Comparing `getdaft-0.1.7/local_dependencies/daft-core/src/array/from.rs` & `getdaft-0.1.8/local_dependencies/daft-core/src/array/from.rs`

 * *Files identical despite different names*

### Comparing `getdaft-0.1.7/local_dependencies/daft-core/src/array/iterator.rs` & `getdaft-0.1.8/local_dependencies/daft-core/src/array/iterator.rs`

 * *Files identical despite different names*

### Comparing `getdaft-0.1.7/local_dependencies/daft-core/src/array/mod.rs` & `getdaft-0.1.8/local_dependencies/daft-core/src/array/mod.rs`

 * *Files identical despite different names*

### Comparing `getdaft-0.1.7/local_dependencies/daft-core/src/array/ops/apply.rs` & `getdaft-0.1.8/local_dependencies/daft-core/src/array/ops/apply.rs`

 * *Files identical despite different names*

### Comparing `getdaft-0.1.7/local_dependencies/daft-core/src/array/ops/arange.rs` & `getdaft-0.1.8/local_dependencies/daft-core/src/array/ops/arange.rs`

 * *Files identical despite different names*

### Comparing `getdaft-0.1.7/local_dependencies/daft-core/src/array/ops/arithmetic.rs` & `getdaft-0.1.8/local_dependencies/daft-core/src/array/ops/arithmetic.rs`

 * *Files identical despite different names*

### Comparing `getdaft-0.1.7/local_dependencies/daft-core/src/array/ops/arrow2/comparison.rs` & `getdaft-0.1.8/local_dependencies/daft-core/src/array/ops/arrow2/comparison.rs`

 * *Files identical despite different names*

### Comparing `getdaft-0.1.7/local_dependencies/daft-core/src/array/ops/arrow2/sort/primitive/common.rs` & `getdaft-0.1.8/local_dependencies/daft-core/src/array/ops/arrow2/sort/primitive/common.rs`

 * *Files identical despite different names*

### Comparing `getdaft-0.1.7/local_dependencies/daft-core/src/array/ops/arrow2/sort/primitive/indices.rs` & `getdaft-0.1.8/local_dependencies/daft-core/src/array/ops/arrow2/sort/primitive/indices.rs`

 * *Files identical despite different names*

### Comparing `getdaft-0.1.7/local_dependencies/daft-core/src/array/ops/arrow2/sort/primitive/sort.rs` & `getdaft-0.1.8/local_dependencies/daft-core/src/array/ops/arrow2/sort/primitive/sort.rs`

 * *Files identical despite different names*

### Comparing `getdaft-0.1.7/local_dependencies/daft-core/src/array/ops/as_arrow.rs` & `getdaft-0.1.8/local_dependencies/daft-core/src/array/ops/as_arrow.rs`

 * *Files identical despite different names*

### Comparing `getdaft-0.1.7/local_dependencies/daft-core/src/array/ops/broadcast.rs` & `getdaft-0.1.8/local_dependencies/daft-core/src/array/ops/broadcast.rs`

 * *Files identical despite different names*

### Comparing `getdaft-0.1.7/local_dependencies/daft-core/src/array/ops/cast.rs` & `getdaft-0.1.8/local_dependencies/daft-core/src/array/ops/cast.rs`

 * *Files identical despite different names*

### Comparing `getdaft-0.1.7/local_dependencies/daft-core/src/array/ops/compare_agg.rs` & `getdaft-0.1.8/local_dependencies/daft-core/src/array/ops/compare_agg.rs`

 * *Files identical despite different names*

### Comparing `getdaft-0.1.7/local_dependencies/daft-core/src/array/ops/comparison.rs` & `getdaft-0.1.8/local_dependencies/daft-core/src/array/ops/comparison.rs`

 * *Files identical despite different names*

### Comparing `getdaft-0.1.7/local_dependencies/daft-core/src/array/ops/concat.rs` & `getdaft-0.1.8/local_dependencies/daft-core/src/array/ops/concat.rs`

 * *Files identical despite different names*

### Comparing `getdaft-0.1.7/local_dependencies/daft-core/src/array/ops/concat_agg.rs` & `getdaft-0.1.8/local_dependencies/daft-core/src/array/ops/concat_agg.rs`

 * *Files identical despite different names*

### Comparing `getdaft-0.1.7/local_dependencies/daft-core/src/array/ops/count.rs` & `getdaft-0.1.8/local_dependencies/daft-core/src/array/ops/count.rs`

 * *Files identical despite different names*

### Comparing `getdaft-0.1.7/local_dependencies/daft-core/src/array/ops/date.rs` & `getdaft-0.1.8/local_dependencies/daft-core/src/array/ops/date.rs`

 * *Files identical despite different names*

### Comparing `getdaft-0.1.7/local_dependencies/daft-core/src/array/ops/filter.rs` & `getdaft-0.1.8/local_dependencies/daft-core/src/array/ops/filter.rs`

 * *Files identical despite different names*

### Comparing `getdaft-0.1.7/local_dependencies/daft-core/src/array/ops/float.rs` & `getdaft-0.1.8/local_dependencies/daft-core/src/array/ops/float.rs`

 * *Files identical despite different names*

### Comparing `getdaft-0.1.7/local_dependencies/daft-core/src/array/ops/full.rs` & `getdaft-0.1.8/local_dependencies/daft-core/src/array/ops/full.rs`

 * *Files identical despite different names*

### Comparing `getdaft-0.1.7/local_dependencies/daft-core/src/array/ops/get.rs` & `getdaft-0.1.8/local_dependencies/daft-core/src/array/ops/get.rs`

 * *Files identical despite different names*

### Comparing `getdaft-0.1.7/local_dependencies/daft-core/src/array/ops/groups.rs` & `getdaft-0.1.8/local_dependencies/daft-core/src/array/ops/groups.rs`

 * *Files identical despite different names*

### Comparing `getdaft-0.1.7/local_dependencies/daft-core/src/array/ops/hash.rs` & `getdaft-0.1.8/local_dependencies/daft-core/src/array/ops/hash.rs`

 * *Files identical despite different names*

### Comparing `getdaft-0.1.7/local_dependencies/daft-core/src/array/ops/if_else.rs` & `getdaft-0.1.8/local_dependencies/daft-core/src/array/ops/if_else.rs`

 * *Files identical despite different names*

### Comparing `getdaft-0.1.7/local_dependencies/daft-core/src/array/ops/image.rs` & `getdaft-0.1.8/local_dependencies/daft-core/src/array/ops/image.rs`

 * *Files identical despite different names*

### Comparing `getdaft-0.1.7/local_dependencies/daft-core/src/array/ops/len.rs` & `getdaft-0.1.8/local_dependencies/daft-core/src/array/ops/len.rs`

 * *Files identical despite different names*

### Comparing `getdaft-0.1.7/local_dependencies/daft-core/src/array/ops/list.rs` & `getdaft-0.1.8/local_dependencies/daft-core/src/array/ops/list.rs`

 * *Files identical despite different names*

### Comparing `getdaft-0.1.7/local_dependencies/daft-core/src/array/ops/list_agg.rs` & `getdaft-0.1.8/local_dependencies/daft-core/src/array/ops/list_agg.rs`

 * *Files identical despite different names*

### Comparing `getdaft-0.1.7/local_dependencies/daft-core/src/array/ops/mean.rs` & `getdaft-0.1.8/local_dependencies/daft-core/src/array/ops/mean.rs`

 * *Files identical despite different names*

### Comparing `getdaft-0.1.7/local_dependencies/daft-core/src/array/ops/mod.rs` & `getdaft-0.1.8/local_dependencies/daft-core/src/array/ops/mod.rs`

 * *Files identical despite different names*

### Comparing `getdaft-0.1.7/local_dependencies/daft-core/src/array/ops/null.rs` & `getdaft-0.1.8/local_dependencies/daft-core/src/array/ops/null.rs`

 * *Files identical despite different names*

### Comparing `getdaft-0.1.7/local_dependencies/daft-core/src/array/ops/pairwise.rs` & `getdaft-0.1.8/local_dependencies/daft-core/src/array/ops/pairwise.rs`

 * *Files identical despite different names*

### Comparing `getdaft-0.1.7/local_dependencies/daft-core/src/array/ops/repr.rs` & `getdaft-0.1.8/local_dependencies/daft-core/src/array/ops/repr.rs`

 * *Files identical despite different names*

### Comparing `getdaft-0.1.7/local_dependencies/daft-core/src/array/ops/sort.rs` & `getdaft-0.1.8/local_dependencies/daft-core/src/array/ops/sort.rs`

 * *Files identical despite different names*

### Comparing `getdaft-0.1.7/local_dependencies/daft-core/src/array/ops/sum.rs` & `getdaft-0.1.8/local_dependencies/daft-core/src/array/ops/sum.rs`

 * *Files identical despite different names*

### Comparing `getdaft-0.1.7/local_dependencies/daft-core/src/array/ops/take.rs` & `getdaft-0.1.8/local_dependencies/daft-core/src/array/ops/take.rs`

 * *Files identical despite different names*

### Comparing `getdaft-0.1.7/local_dependencies/daft-core/src/array/ops/utf8.rs` & `getdaft-0.1.8/local_dependencies/daft-core/src/array/ops/utf8.rs`

 * *Files identical despite different names*

### Comparing `getdaft-0.1.7/local_dependencies/daft-core/src/array/pseudo_arrow/compute.rs` & `getdaft-0.1.8/local_dependencies/daft-core/src/array/pseudo_arrow/compute.rs`

 * *Files identical despite different names*

### Comparing `getdaft-0.1.7/local_dependencies/daft-core/src/array/pseudo_arrow/mod.rs` & `getdaft-0.1.8/local_dependencies/daft-core/src/array/pseudo_arrow/mod.rs`

 * *Files identical despite different names*

### Comparing `getdaft-0.1.7/local_dependencies/daft-core/src/array/pseudo_arrow/python.rs` & `getdaft-0.1.8/local_dependencies/daft-core/src/array/pseudo_arrow/python.rs`

 * *Files identical despite different names*

### Comparing `getdaft-0.1.7/local_dependencies/daft-core/src/datatypes/dtype.rs` & `getdaft-0.1.8/local_dependencies/daft-core/src/datatypes/dtype.rs`

 * *Files identical despite different names*

### Comparing `getdaft-0.1.7/local_dependencies/daft-core/src/datatypes/field.rs` & `getdaft-0.1.8/local_dependencies/daft-core/src/datatypes/field.rs`

 * *Files identical despite different names*

### Comparing `getdaft-0.1.7/local_dependencies/daft-core/src/datatypes/image_format.rs` & `getdaft-0.1.8/local_dependencies/daft-core/src/datatypes/image_format.rs`

 * *Files identical despite different names*

### Comparing `getdaft-0.1.7/local_dependencies/daft-core/src/datatypes/image_mode.rs` & `getdaft-0.1.8/local_dependencies/daft-core/src/datatypes/image_mode.rs`

 * *Files identical despite different names*

### Comparing `getdaft-0.1.7/local_dependencies/daft-core/src/datatypes/logical.rs` & `getdaft-0.1.8/local_dependencies/daft-core/src/datatypes/logical.rs`

 * *Files 8% similar despite different names*

```diff
@@ -8,14 +8,20 @@
 };
 pub struct LogicalArray<L: DaftLogicalType> {
     pub field: Arc<Field>,
     pub physical: DataArray<L::PhysicalType>,
     marker_: PhantomData<L>,
 }
 
+impl<L: DaftLogicalType> Clone for LogicalArray<L> {
+    fn clone(&self) -> Self {
+        LogicalArray::new(self.field.clone(), self.physical.clone())
+    }
+}
+
 impl<L: DaftLogicalType + 'static> LogicalArray<L> {
     pub fn new<F: Into<Arc<Field>>>(field: F, physical: DataArray<L::PhysicalType>) -> Self {
         let field = field.into();
         assert!(
             field.dtype.is_logical(),
             "Can only construct Logical Arrays on Logical Types, got {}",
             field.dtype
```

### Comparing `getdaft-0.1.7/local_dependencies/daft-core/src/datatypes/matching.rs` & `getdaft-0.1.8/local_dependencies/daft-core/src/datatypes/matching.rs`

 * *Files identical despite different names*

### Comparing `getdaft-0.1.7/local_dependencies/daft-core/src/datatypes/mod.rs` & `getdaft-0.1.8/local_dependencies/daft-core/src/datatypes/mod.rs`

 * *Files 0% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+mod binary_ops;
 mod dtype;
 mod field;
 mod image_format;
 mod image_mode;
 mod matching;
 mod time_unit;
```

### Comparing `getdaft-0.1.7/local_dependencies/daft-core/src/datatypes/time_unit.rs` & `getdaft-0.1.8/local_dependencies/daft-core/src/datatypes/time_unit.rs`

 * *Files 12% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 use arrow2::datatypes::TimeUnit as ArrowTimeUnit;
 
 use common_error::DaftResult;
 
 use serde::{Deserialize, Serialize};
 
-#[derive(Copy, Clone, Debug, PartialEq, Eq, Hash, Deserialize, Serialize)]
+#[derive(Copy, Clone, Debug, PartialEq, Eq, PartialOrd, Ord, Hash, Deserialize, Serialize)]
 pub enum TimeUnit {
     Nanoseconds,
     Microseconds,
     Milliseconds,
     Seconds,
 }
```

### Comparing `getdaft-0.1.7/local_dependencies/daft-core/src/ffi.rs` & `getdaft-0.1.8/local_dependencies/daft-core/src/ffi.rs`

 * *Files identical despite different names*

### Comparing `getdaft-0.1.7/local_dependencies/daft-core/src/kernels/hashing.rs` & `getdaft-0.1.8/local_dependencies/daft-core/src/kernels/hashing.rs`

 * *Files identical despite different names*

### Comparing `getdaft-0.1.7/local_dependencies/daft-core/src/kernels/search_sorted.rs` & `getdaft-0.1.8/local_dependencies/daft-core/src/kernels/search_sorted.rs`

 * *Files identical despite different names*

### Comparing `getdaft-0.1.7/local_dependencies/daft-core/src/kernels/utf8.rs` & `getdaft-0.1.8/local_dependencies/daft-core/src/kernels/utf8.rs`

 * *Files identical despite different names*

### Comparing `getdaft-0.1.7/local_dependencies/daft-core/src/lib.rs` & `getdaft-0.1.8/local_dependencies/daft-core/src/lib.rs`

 * *Files identical despite different names*

### Comparing `getdaft-0.1.7/local_dependencies/daft-core/src/python/datatype.rs` & `getdaft-0.1.8/local_dependencies/daft-core/src/python/datatype.rs`

 * *Files identical despite different names*

### Comparing `getdaft-0.1.7/local_dependencies/daft-core/src/python/field.rs` & `getdaft-0.1.8/local_dependencies/daft-core/src/python/field.rs`

 * *Files identical despite different names*

### Comparing `getdaft-0.1.7/local_dependencies/daft-core/src/python/mod.rs` & `getdaft-0.1.8/local_dependencies/daft-core/src/python/mod.rs`

 * *Files identical despite different names*

### Comparing `getdaft-0.1.7/local_dependencies/daft-core/src/python/schema.rs` & `getdaft-0.1.8/local_dependencies/daft-core/src/python/schema.rs`

 * *Files identical despite different names*

### Comparing `getdaft-0.1.7/local_dependencies/daft-core/src/python/series.rs` & `getdaft-0.1.8/local_dependencies/daft-core/src/python/series.rs`

 * *Files identical despite different names*

### Comparing `getdaft-0.1.7/local_dependencies/daft-core/src/schema.rs` & `getdaft-0.1.8/local_dependencies/daft-core/src/schema.rs`

 * *Files 9% similar despite different names*

```diff
@@ -90,15 +90,15 @@
 
         let mut res = "<table class=\"dataframe\">\n".to_string();
 
         // Begin the header.
         res.push_str("<thead><tr>");
 
         for (name, field) in &self.fields {
-            res.push_str("<th>");
+            res.push_str("<th style=\"text-wrap: nowrap; max-width:192px; overflow:auto\">");
             res.push_str(&html_escape::encode_text(name));
             res.push_str("<br />");
             res.push_str(&html_escape::encode_text(&format!("{}", field.dtype)));
             res.push_str("</th>");
         }
 
         // End the header.
```

#### html2text {}

```diff
@@ -22,15 +22,12 @@
 (self.fields.keys()); let other_keys: HashSet<&String> = HashSet::from_iter
 (self.fields.keys()); match self_keys.difference(&other_keys).count() { 0 =>
 { let mut fields = IndexMap::new(); for (k, v) in self.fields.iter().chain
 (other.fields.iter()) { fields.insert(k.clone(), v.clone()); } Ok(Schema
 { fields }) } _ => Err(DaftError::ValueError( "Cannot union two schemas with
 overlapping keys".to_string(), )), } } pub fn repr_html(&self) -> String { /
 / Produces a
-"); res.push_str(&html_escape::encode_text(name)); res.push_str("
-"); res.push_str(&html_escape::encode_text(&format!("{}", field.dtype)));
-res.push_str("
 "); res } } impl Display for Schema { // `f` is a buffer, and this method must
 write the formatted string into it fn fmt(&self, f: &mut Formatter) -> Result
 { let mut table = prettytable::Table::new(); let header = self .fields .iter()
 .map(|(name, field)| format!("{}\n{:?}", name, field.dtype)) .collect();
 table.add_row(header); write!(f, "{table}") } }
```

### Comparing `getdaft-0.1.7/local_dependencies/daft-core/src/series/array_impl/data_array.rs` & `getdaft-0.1.8/local_dependencies/daft-core/src/series/array_impl/data_array.rs`

 * *Files 6% similar despite different names*

```diff
@@ -5,14 +5,15 @@
 use crate::array::ops::DaftListAggable;
 use crate::array::ops::GroupIndices;
 use crate::array::DataArray;
 use crate::datatypes::DaftArrowBackedType;
 
 #[cfg(feature = "python")]
 use crate::datatypes::PythonArray;
+use crate::series::array_impl::binary_ops::SeriesBinaryOps;
 use crate::series::Field;
 use crate::{
     datatypes::{
         BinaryArray, BooleanArray, ExtensionArray, FixedSizeListArray, Float32Array, Float64Array,
         Int16Array, Int32Array, Int64Array, Int8Array, ListArray, NullArray, StructArray,
         UInt16Array, UInt32Array, UInt64Array, UInt8Array, Utf8Array,
     },
@@ -165,14 +166,17 @@
         }
     }
 }
 
 macro_rules! impl_series_like_for_data_array {
     ($da:ident) => {
         impl SeriesLike for ArrayWrapper<$da> {
+            fn into_series(&self) -> Series {
+                self.0.clone().into_series()
+            }
             fn to_arrow(&self) -> Box<dyn arrow2::array::Array> {
                 logical_to_arrow(Cow::Borrowed(&self.0.data), self.field()).into_owned()
             }
 
             fn as_any(&self) -> &dyn std::any::Any {
                 self
             }
@@ -263,14 +267,34 @@
 
             fn agg_list(&self, groups: Option<&GroupIndices>) -> DaftResult<Series> {
                 match groups {
                     Some(groups) => Ok(self.0.grouped_list(groups)?.into_series()),
                     None => Ok(self.0.list()?.into_series()),
                 }
             }
+
+            fn add(&self, rhs: &Series) -> DaftResult<Series> {
+                SeriesBinaryOps::add(self, rhs)
+            }
+
+            fn sub(&self, rhs: &Series) -> DaftResult<Series> {
+                SeriesBinaryOps::sub(self, rhs)
+            }
+
+            fn mul(&self, rhs: &Series) -> DaftResult<Series> {
+                SeriesBinaryOps::mul(self, rhs)
+            }
+
+            fn div(&self, rhs: &Series) -> DaftResult<Series> {
+                SeriesBinaryOps::div(self, rhs)
+            }
+
+            fn rem(&self, rhs: &Series) -> DaftResult<Series> {
+                SeriesBinaryOps::rem(self, rhs)
+            }
         }
     };
 }
 
 impl_series_like_for_data_array!(NullArray);
 impl_series_like_for_data_array!(BooleanArray);
 impl_series_like_for_data_array!(BinaryArray);
```

### Comparing `getdaft-0.1.7/local_dependencies/daft-core/src/series/array_impl/logical_array.rs` & `getdaft-0.1.8/local_dependencies/daft-core/src/series/array_impl/logical_array.rs`

 * *Files 16% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 use crate::datatypes::logical::{
     DateArray, DurationArray, EmbeddingArray, FixedShapeImageArray, ImageArray, TimestampArray,
 };
 
 use super::{ArrayWrapper, IntoSeries, Series};
 use crate::array::ops::GroupIndices;
+use crate::series::array_impl::binary_ops::SeriesBinaryOps;
 use crate::series::DaftResult;
 use crate::series::SeriesLike;
 use crate::with_match_integer_daft_types;
 use std::sync::Arc;
 
 macro_rules! impl_series_like_for_logical_array {
     ($da:ident) => {
@@ -16,14 +17,17 @@
                 Series {
                     inner: Arc::new(ArrayWrapper(self)),
                 }
             }
         }
 
         impl SeriesLike for ArrayWrapper<$da> {
+            fn into_series(&self) -> Series {
+                self.0.clone().into_series()
+            }
             fn to_arrow(&self) -> Box<dyn arrow2::array::Array> {
                 let arrow_logical_type = self.0.logical_type().to_arrow().unwrap();
                 let physical_arrow_array = self.0.physical.data();
                 arrow2::compute::cast::cast(
                     physical_arrow_array,
                     &arrow_logical_type,
                     arrow2::compute::cast::CastOptions {
@@ -137,14 +141,34 @@
                 let data_array = match groups {
                     Some(groups) => self.0.physical.grouped_list(groups)?,
                     None => self.0.physical.list()?,
                 };
                 let new_field = self.field().to_list_field()?;
                 Ok(ListArray::new(Arc::new(new_field), data_array.data)?.into_series())
             }
+
+            fn add(&self, rhs: &Series) -> DaftResult<Series> {
+                SeriesBinaryOps::add(self, rhs)
+            }
+
+            fn sub(&self, rhs: &Series) -> DaftResult<Series> {
+                SeriesBinaryOps::sub(self, rhs)
+            }
+
+            fn mul(&self, rhs: &Series) -> DaftResult<Series> {
+                SeriesBinaryOps::mul(self, rhs)
+            }
+
+            fn div(&self, rhs: &Series) -> DaftResult<Series> {
+                SeriesBinaryOps::div(self, rhs)
+            }
+
+            fn rem(&self, rhs: &Series) -> DaftResult<Series> {
+                SeriesBinaryOps::rem(self, rhs)
+            }
         }
     };
 }
 
 impl_series_like_for_logical_array!(DateArray);
 impl_series_like_for_logical_array!(DurationArray);
 impl_series_like_for_logical_array!(EmbeddingArray);
```

### Comparing `getdaft-0.1.7/local_dependencies/daft-core/src/series/from.rs` & `getdaft-0.1.8/local_dependencies/daft-core/src/series/from.rs`

 * *Files identical despite different names*

### Comparing `getdaft-0.1.7/local_dependencies/daft-core/src/series/mod.rs` & `getdaft-0.1.8/local_dependencies/daft-core/src/series/mod.rs`

 * *Files identical despite different names*

### Comparing `getdaft-0.1.7/local_dependencies/daft-core/src/series/ops/abs.rs` & `getdaft-0.1.8/local_dependencies/daft-core/src/series/ops/abs.rs`

 * *Files identical despite different names*

### Comparing `getdaft-0.1.7/local_dependencies/daft-core/src/series/ops/agg.rs` & `getdaft-0.1.8/local_dependencies/daft-core/src/series/ops/agg.rs`

 * *Files identical despite different names*

### Comparing `getdaft-0.1.7/local_dependencies/daft-core/src/series/ops/broadcast.rs` & `getdaft-0.1.8/local_dependencies/daft-core/src/series/ops/broadcast.rs`

 * *Files identical despite different names*

### Comparing `getdaft-0.1.7/local_dependencies/daft-core/src/series/ops/comparison.rs` & `getdaft-0.1.8/local_dependencies/daft-core/src/series/ops/comparison.rs`

 * *Files identical despite different names*

### Comparing `getdaft-0.1.7/local_dependencies/daft-core/src/series/ops/concat.rs` & `getdaft-0.1.8/local_dependencies/daft-core/src/series/ops/concat.rs`

 * *Files identical despite different names*

### Comparing `getdaft-0.1.7/local_dependencies/daft-core/src/series/ops/date.rs` & `getdaft-0.1.8/local_dependencies/daft-core/src/series/ops/date.rs`

 * *Files identical despite different names*

### Comparing `getdaft-0.1.7/local_dependencies/daft-core/src/series/ops/downcast.rs` & `getdaft-0.1.8/local_dependencies/daft-core/src/series/ops/downcast.rs`

 * *Files identical despite different names*

### Comparing `getdaft-0.1.7/local_dependencies/daft-core/src/series/ops/filter.rs` & `getdaft-0.1.8/local_dependencies/daft-core/src/series/ops/filter.rs`

 * *Files identical despite different names*

### Comparing `getdaft-0.1.7/local_dependencies/daft-core/src/series/ops/image.rs` & `getdaft-0.1.8/local_dependencies/daft-core/src/series/ops/image.rs`

 * *Files identical despite different names*

### Comparing `getdaft-0.1.7/local_dependencies/daft-core/src/series/ops/list.rs` & `getdaft-0.1.8/local_dependencies/daft-core/src/series/ops/list.rs`

 * *Files identical despite different names*

### Comparing `getdaft-0.1.7/local_dependencies/daft-core/src/series/ops/mod.rs` & `getdaft-0.1.8/local_dependencies/daft-core/src/series/ops/mod.rs`

 * *Files 7% similar despite different names*

```diff
@@ -40,23 +40,28 @@
     if !rhs.data_type().eq(&supertype) {
         rhs = rhs.cast(&supertype)?;
     }
 
     Ok((lhs, rhs))
 }
 
+#[cfg(feature = "python")]
 macro_rules! py_binary_op_utilfn {
     ($lhs:expr, $rhs:expr, $pyoperator:expr, $utilfn:expr) => {{
         use crate::python::PySeries;
+        use crate::DataType;
         use pyo3::prelude::*;
 
-        let (lhs, rhs) = match ($lhs.len(), $rhs.len()) {
-            (a, b) if a == b => ($lhs, $rhs),
-            (a, 1) => ($lhs, $rhs.broadcast(a)?),
-            (1, b) => ($lhs.broadcast(b)?, $rhs),
+        let lhs = $lhs.cast(&DataType::Python)?;
+        let rhs = $rhs.cast(&DataType::Python)?;
+
+        let (lhs, rhs) = match (lhs.len(), rhs.len()) {
+            (a, b) if a == b => (lhs, rhs),
+            (a, 1) => (lhs, rhs.broadcast(a)?),
+            (1, b) => (lhs.broadcast(b)?, rhs),
             (a, b) => panic!("Cannot apply operation on arrays of different lengths: {a} vs {b}"),
         };
 
         let left_pylist = PySeries::from(lhs.clone()).to_pylist()?;
         let right_pylist = PySeries::from(rhs.clone()).to_pylist()?;
 
         let result_series: Series = Python::with_gil(|py| -> PyResult<PySeries> {
@@ -75,8 +80,9 @@
                 .extract()
         })?
         .into();
 
         result_series
     }};
 }
+#[cfg(feature = "python")]
 pub(super) use py_binary_op_utilfn;
```

### Comparing `getdaft-0.1.7/local_dependencies/daft-core/src/series/ops/search_sorted.rs` & `getdaft-0.1.8/local_dependencies/daft-core/src/series/ops/search_sorted.rs`

 * *Files identical despite different names*

### Comparing `getdaft-0.1.7/local_dependencies/daft-core/src/series/ops/sort.rs` & `getdaft-0.1.8/local_dependencies/daft-core/src/series/ops/sort.rs`

 * *Files identical despite different names*

### Comparing `getdaft-0.1.7/local_dependencies/daft-core/src/series/ops/take.rs` & `getdaft-0.1.8/local_dependencies/daft-core/src/series/ops/take.rs`

 * *Files identical despite different names*

### Comparing `getdaft-0.1.7/local_dependencies/daft-core/src/series/ops/utf8.rs` & `getdaft-0.1.8/local_dependencies/daft-core/src/series/ops/utf8.rs`

 * *Files identical despite different names*

### Comparing `getdaft-0.1.7/local_dependencies/daft-core/src/series/series_like.rs` & `getdaft-0.1.8/local_dependencies/daft-core/src/series/series_like.rs`

 * *Files 26% similar despite different names*

```diff
@@ -5,14 +5,15 @@
     datatypes::{BooleanArray, DataType, Field},
 };
 use common_error::DaftResult;
 
 use super::Series;
 
 pub trait SeriesLike: Send + Sync + Any {
+    fn into_series(&self) -> Series;
     fn to_arrow(&self) -> Box<dyn arrow2::array::Array>;
     fn as_any(&self) -> &dyn std::any::Any;
     fn min(&self, groups: Option<&GroupIndices>) -> DaftResult<Series>;
     fn max(&self, groups: Option<&GroupIndices>) -> DaftResult<Series>;
     fn agg_list(&self, groups: Option<&GroupIndices>) -> DaftResult<Series>;
     fn broadcast(&self, num: usize) -> DaftResult<Series>;
     fn cast(&self, datatype: &DataType) -> DaftResult<Series>;
@@ -27,8 +28,13 @@
     fn is_null(&self) -> DaftResult<Series>;
     fn sort(&self, descending: bool) -> DaftResult<Series>;
     fn head(&self, num: usize) -> DaftResult<Series>;
     fn slice(&self, start: usize, end: usize) -> DaftResult<Series>;
     fn take(&self, idx: &Series) -> DaftResult<Series>;
     fn str_value(&self, idx: usize) -> DaftResult<String>;
     fn html_value(&self, idx: usize) -> String;
+    fn add(&self, rhs: &Series) -> DaftResult<Series>;
+    fn sub(&self, rhs: &Series) -> DaftResult<Series>;
+    fn mul(&self, rhs: &Series) -> DaftResult<Series>;
+    fn div(&self, rhs: &Series) -> DaftResult<Series>;
+    fn rem(&self, rhs: &Series) -> DaftResult<Series>;
 }
```

### Comparing `getdaft-0.1.7/local_dependencies/daft-core/src/utils/arrow.rs` & `getdaft-0.1.8/local_dependencies/daft-core/src/utils/arrow.rs`

 * *Files identical despite different names*

### Comparing `getdaft-0.1.7/local_dependencies/daft-core/src/utils/supertype.rs` & `getdaft-0.1.8/local_dependencies/daft-core/src/utils/supertype.rs`

 * *Files 0% similar despite different names*

```diff
@@ -37,14 +37,15 @@
     match get_supertype(l, r) {
         Some(dt) => Ok(dt),
         None => Err(DaftError::TypeError(format!(
             "could not determine supertype of {l:?} and {r:?}"
         ))),
     }
 }
+
 pub fn get_supertype(l: &DataType, r: &DataType) -> Option<DataType> {
     fn inner(l: &DataType, r: &DataType) -> Option<DataType> {
         use DataType::*;
 
         if l == r {
             return Some(l.clone());
         }
```

### Comparing `getdaft-0.1.7/local_dependencies/daft-table/Cargo.toml` & `getdaft-0.1.8/local_dependencies/daft-table/Cargo.toml`

 * *Files identical despite different names*

### Comparing `getdaft-0.1.7/local_dependencies/daft-table/src/ffi.rs` & `getdaft-0.1.8/local_dependencies/daft-table/src/ffi.rs`

 * *Files identical despite different names*

### Comparing `getdaft-0.1.7/local_dependencies/daft-table/src/lib.rs` & `getdaft-0.1.8/local_dependencies/daft-table/src/lib.rs`

 * *Files 2% similar despite different names*

```diff
@@ -400,15 +400,15 @@
 
         let mut res = "<table class=\"dataframe\">\n".to_string();
 
         // Begin the header.
         res.push_str("<thead><tr>");
 
         for (name, field) in &self.schema.fields {
-            res.push_str("<th>");
+            res.push_str("<th style=\"text-wrap: nowrap; max-width:192px; overflow:auto\">");
             res.push_str(&html_escape::encode_text(name));
             res.push_str("<br />");
             res.push_str(&html_escape::encode_text(&format!("{}", field.dtype)));
             res.push_str("</th>");
         }
 
         // End the header.
@@ -424,22 +424,25 @@
             head_rows = 5;
             tail_rows = 5;
         } else {
             head_rows = self.len();
             tail_rows = 0;
         }
 
+        let styled_td =
+            "<td><div style=\"text-align:left; max-width:192px; max-height:64px; overflow:auto\">";
+
         for i in 0..head_rows {
             // Begin row.
             res.push_str("<tr>");
 
             for col in self.columns.iter() {
-                res.push_str("<td>");
+                res.push_str(styled_td);
                 res.push_str(&col.html_value(i));
-                res.push_str("</td>");
+                res.push_str("</div></td>");
             }
 
             // End row.
             res.push_str("</tr>\n");
         }
 
         if tail_rows != 0 {
@@ -451,15 +454,15 @@
         }
 
         for i in (self.len() - tail_rows)..(self.len()) {
             // Begin row.
             res.push_str("<tr>");
 
             for col in self.columns.iter() {
-                res.push_str("<td>");
+                res.push_str(styled_td);
                 res.push_str(&col.html_value(i));
                 res.push_str("</td>");
             }
 
             // End row.
             res.push_str("</tr>\n");
         }
```

### Comparing `getdaft-0.1.7/local_dependencies/daft-table/src/ops/agg.rs` & `getdaft-0.1.8/local_dependencies/daft-table/src/ops/agg.rs`

 * *Files identical despite different names*

### Comparing `getdaft-0.1.7/local_dependencies/daft-table/src/ops/explode.rs` & `getdaft-0.1.8/local_dependencies/daft-table/src/ops/explode.rs`

 * *Files identical despite different names*

### Comparing `getdaft-0.1.7/local_dependencies/daft-table/src/ops/groups.rs` & `getdaft-0.1.8/local_dependencies/daft-table/src/ops/groups.rs`

 * *Files identical despite different names*

### Comparing `getdaft-0.1.7/local_dependencies/daft-table/src/ops/hash.rs` & `getdaft-0.1.8/local_dependencies/daft-table/src/ops/hash.rs`

 * *Files identical despite different names*

### Comparing `getdaft-0.1.7/local_dependencies/daft-table/src/ops/joins/hash_join.rs` & `getdaft-0.1.8/local_dependencies/daft-table/src/ops/joins/hash_join.rs`

 * *Files identical despite different names*

### Comparing `getdaft-0.1.7/local_dependencies/daft-table/src/ops/joins/mod.rs` & `getdaft-0.1.8/local_dependencies/daft-table/src/ops/joins/mod.rs`

 * *Files identical despite different names*

### Comparing `getdaft-0.1.7/local_dependencies/daft-table/src/ops/partition.rs` & `getdaft-0.1.8/local_dependencies/daft-table/src/ops/partition.rs`

 * *Files identical despite different names*

### Comparing `getdaft-0.1.7/local_dependencies/daft-table/src/ops/search_sorted.rs` & `getdaft-0.1.8/local_dependencies/daft-table/src/ops/search_sorted.rs`

 * *Files identical despite different names*

### Comparing `getdaft-0.1.7/local_dependencies/daft-table/src/ops/sort.rs` & `getdaft-0.1.8/local_dependencies/daft-table/src/ops/sort.rs`

 * *Files identical despite different names*

### Comparing `getdaft-0.1.7/local_dependencies/daft-table/src/python.rs` & `getdaft-0.1.8/local_dependencies/daft-table/src/python.rs`

 * *Files identical despite different names*

### Comparing `getdaft-0.1.7/local_dependencies/daft-dsl/Cargo.toml` & `getdaft-0.1.8/local_dependencies/daft-dsl/Cargo.toml`

 * *Files identical despite different names*

### Comparing `getdaft-0.1.7/local_dependencies/daft-dsl/src/arithmetic.rs` & `getdaft-0.1.8/local_dependencies/daft-dsl/src/arithmetic.rs`

 * *Files identical despite different names*

### Comparing `getdaft-0.1.7/local_dependencies/daft-dsl/src/expr.rs` & `getdaft-0.1.8/local_dependencies/daft-dsl/src/expr.rs`

 * *Files 7% similar despite different names*

```diff
@@ -292,75 +292,36 @@
                             Ok(_) => Ok(Field::new(
                                 left.to_field(schema)?.name.as_str(),
                                 DataType::Boolean,
                             )),
                             Err(_) => Err(DaftError::TypeError(format!("Expected left and right arguments to be castable to the same supertype for comparison {op}, but received {left_field} and {right_field}"))),
                         }
                     }
-
-                    // Plus operation: special-cased as it has semantic meaning for some other types
                     Operator::Plus => {
-                        #[cfg(feature = "python")]
-                        {
-                            let supertype =
-                                try_get_supertype(&left_field.dtype, &right_field.dtype)?;
-                            if supertype.is_python() {
-                                return Ok(Field::new(left_field.name.as_str(), supertype));
-                            }
-                        }
-                        let (lhs, rhs) = (&left_field.dtype, &right_field.dtype);
-                        for dt in [lhs, rhs] {
-                            if !(dt.is_numeric()
-                                || dt.eq(&DataType::Utf8)
-                                || dt.eq(&DataType::Boolean)
-                                || dt.eq(&DataType::Null))
-                            {
-                                return Err(DaftError::TypeError(format!("Expected left and right arguments to both be numeric for {op}, but received {right_field} and {left_field}")));
-                            }
-                        }
-                        let supertype = try_get_supertype(lhs, rhs)?;
-                        Ok(Field::new(left.to_field(schema)?.name.as_str(), supertype))
+                        let result_type = (&left_field.dtype + &right_field.dtype)?;
+                        Ok(Field::new(left_field.name.as_str(), result_type))
+                    }
+                    Operator::Minus => {
+                        let result_type = (&left_field.dtype - &right_field.dtype)?;
+                        Ok(Field::new(left_field.name.as_str(), result_type))
+                    }
+                    Operator::Multiply => {
+                        let result_type = (&left_field.dtype * &right_field.dtype)?;
+                        Ok(Field::new(left_field.name.as_str(), result_type))
                     }
-
-                    // True divide operation
                     Operator::TrueDivide => {
-                        #[cfg(feature = "python")]
-                        {
-                            let supertype =
-                                try_get_supertype(&left_field.dtype, &right_field.dtype)?;
-                            if supertype.is_python() {
-                                return Ok(Field::new(left_field.name.as_str(), supertype));
-                            }
-                        }
-                        if !left_field.dtype.is_numeric() || !right_field.dtype.is_numeric() {
-                            return Err(DaftError::TypeError(format!("Expected left and right arguments for {op} to both be numeric and castable to {}, but received {left_field} and {right_field}", DataType::Float64)));
-                        }
-                        Ok(Field::new(left_field.name.as_str(), DataType::Float64))
+                        let result_type = (&left_field.dtype / &right_field.dtype)?;
+                        Ok(Field::new(left_field.name.as_str(), result_type))
                     }
-
-                    // Regular arithmetic operations
-                    Operator::Minus
-                    | Operator::Multiply
-                    | Operator::Modulus
-                    | Operator::FloorDivide => {
-                        #[cfg(feature = "python")]
-                        {
-                            let supertype =
-                                try_get_supertype(&left_field.dtype, &right_field.dtype)?;
-                            if supertype.is_python() {
-                                return Ok(Field::new(left_field.name.as_str(), supertype));
-                            }
-                        }
-                        if !&left_field.dtype.is_numeric() || !&right_field.dtype.is_numeric() {
-                            return Err(DaftError::TypeError(format!("Expected left and right arguments for {op} to both be numeric but received {left_field} and {right_field}")));
-                        }
-                        Ok(Field::new(
-                            left_field.name.as_str(),
-                            try_get_supertype(&left_field.dtype, &right_field.dtype)?,
-                        ))
+                    Operator::Modulus => {
+                        let result_type = (&left_field.dtype % &right_field.dtype)?;
+                        Ok(Field::new(left_field.name.as_str(), result_type))
+                    }
+                    Operator::FloorDivide => {
+                        unimplemented!()
                     }
                 }
             }
             IfElse {
                 if_true,
                 if_false,
                 predicate,
```

### Comparing `getdaft-0.1.7/local_dependencies/daft-dsl/src/functions/float/is_nan.rs` & `getdaft-0.1.8/local_dependencies/daft-dsl/src/functions/float/is_nan.rs`

 * *Files identical despite different names*

### Comparing `getdaft-0.1.7/local_dependencies/daft-dsl/src/functions/float/mod.rs` & `getdaft-0.1.8/local_dependencies/daft-dsl/src/functions/float/mod.rs`

 * *Files identical despite different names*

### Comparing `getdaft-0.1.7/local_dependencies/daft-dsl/src/functions/image/decode.rs` & `getdaft-0.1.8/local_dependencies/daft-dsl/src/functions/image/decode.rs`

 * *Files identical despite different names*

### Comparing `getdaft-0.1.7/local_dependencies/daft-dsl/src/functions/image/encode.rs` & `getdaft-0.1.8/local_dependencies/daft-dsl/src/functions/image/encode.rs`

 * *Files identical despite different names*

### Comparing `getdaft-0.1.7/local_dependencies/daft-dsl/src/functions/image/mod.rs` & `getdaft-0.1.8/local_dependencies/daft-dsl/src/functions/image/mod.rs`

 * *Files identical despite different names*

### Comparing `getdaft-0.1.7/local_dependencies/daft-dsl/src/functions/image/resize.rs` & `getdaft-0.1.8/local_dependencies/daft-dsl/src/functions/image/resize.rs`

 * *Files identical despite different names*

### Comparing `getdaft-0.1.7/local_dependencies/daft-dsl/src/functions/list/explode.rs` & `getdaft-0.1.8/local_dependencies/daft-dsl/src/functions/list/explode.rs`

 * *Files identical despite different names*

### Comparing `getdaft-0.1.7/local_dependencies/daft-dsl/src/functions/list/join.rs` & `getdaft-0.1.8/local_dependencies/daft-dsl/src/functions/list/join.rs`

 * *Files identical despite different names*

### Comparing `getdaft-0.1.7/local_dependencies/daft-dsl/src/functions/list/mod.rs` & `getdaft-0.1.8/local_dependencies/daft-dsl/src/functions/list/mod.rs`

 * *Files identical despite different names*

### Comparing `getdaft-0.1.7/local_dependencies/daft-dsl/src/functions/mod.rs` & `getdaft-0.1.8/local_dependencies/daft-dsl/src/functions/mod.rs`

 * *Files identical despite different names*

### Comparing `getdaft-0.1.7/local_dependencies/daft-dsl/src/functions/numeric/abs.rs` & `getdaft-0.1.8/local_dependencies/daft-dsl/src/functions/numeric/abs.rs`

 * *Files identical despite different names*

### Comparing `getdaft-0.1.7/local_dependencies/daft-dsl/src/functions/numeric/mod.rs` & `getdaft-0.1.8/local_dependencies/daft-dsl/src/functions/numeric/mod.rs`

 * *Files identical despite different names*

### Comparing `getdaft-0.1.7/local_dependencies/daft-dsl/src/functions/python/mod.rs` & `getdaft-0.1.8/local_dependencies/daft-dsl/src/functions/python/mod.rs`

 * *Files identical despite different names*

### Comparing `getdaft-0.1.7/local_dependencies/daft-dsl/src/functions/python/partial_udf.rs` & `getdaft-0.1.8/local_dependencies/daft-dsl/src/functions/python/partial_udf.rs`

 * *Files identical despite different names*

### Comparing `getdaft-0.1.7/local_dependencies/daft-dsl/src/functions/python/udf.rs` & `getdaft-0.1.8/local_dependencies/daft-dsl/src/functions/python/udf.rs`

 * *Files identical despite different names*

### Comparing `getdaft-0.1.7/local_dependencies/daft-dsl/src/functions/temporal/day.rs` & `getdaft-0.1.8/local_dependencies/daft-dsl/src/functions/temporal/day.rs`

 * *Files identical despite different names*

### Comparing `getdaft-0.1.7/local_dependencies/daft-dsl/src/functions/temporal/day_of_week.rs` & `getdaft-0.1.8/local_dependencies/daft-dsl/src/functions/temporal/day_of_week.rs`

 * *Files identical despite different names*

### Comparing `getdaft-0.1.7/local_dependencies/daft-dsl/src/functions/temporal/mod.rs` & `getdaft-0.1.8/local_dependencies/daft-dsl/src/functions/temporal/mod.rs`

 * *Files identical despite different names*

### Comparing `getdaft-0.1.7/local_dependencies/daft-dsl/src/functions/temporal/month.rs` & `getdaft-0.1.8/local_dependencies/daft-dsl/src/functions/temporal/month.rs`

 * *Files identical despite different names*

### Comparing `getdaft-0.1.7/local_dependencies/daft-dsl/src/functions/temporal/year.rs` & `getdaft-0.1.8/local_dependencies/daft-dsl/src/functions/temporal/year.rs`

 * *Files identical despite different names*

### Comparing `getdaft-0.1.7/local_dependencies/daft-dsl/src/functions/uri/download.rs` & `getdaft-0.1.8/local_dependencies/daft-dsl/src/functions/uri/download.rs`

 * *Files identical despite different names*

### Comparing `getdaft-0.1.7/local_dependencies/daft-dsl/src/functions/uri/mod.rs` & `getdaft-0.1.8/local_dependencies/daft-dsl/src/functions/uri/mod.rs`

 * *Files identical despite different names*

### Comparing `getdaft-0.1.7/local_dependencies/daft-dsl/src/functions/utf8/contains.rs` & `getdaft-0.1.8/local_dependencies/daft-dsl/src/functions/utf8/contains.rs`

 * *Files identical despite different names*

### Comparing `getdaft-0.1.7/local_dependencies/daft-dsl/src/functions/utf8/endswith.rs` & `getdaft-0.1.8/local_dependencies/daft-dsl/src/functions/utf8/endswith.rs`

 * *Files identical despite different names*

### Comparing `getdaft-0.1.7/local_dependencies/daft-dsl/src/functions/utf8/length.rs` & `getdaft-0.1.8/local_dependencies/daft-dsl/src/functions/utf8/length.rs`

 * *Files identical despite different names*

### Comparing `getdaft-0.1.7/local_dependencies/daft-dsl/src/functions/utf8/mod.rs` & `getdaft-0.1.8/local_dependencies/daft-dsl/src/functions/utf8/mod.rs`

 * *Files identical despite different names*

### Comparing `getdaft-0.1.7/local_dependencies/daft-dsl/src/functions/utf8/startswith.rs` & `getdaft-0.1.8/local_dependencies/daft-dsl/src/functions/utf8/startswith.rs`

 * *Files identical despite different names*

### Comparing `getdaft-0.1.7/local_dependencies/daft-dsl/src/lib.rs` & `getdaft-0.1.8/local_dependencies/daft-dsl/src/lib.rs`

 * *Files identical despite different names*

### Comparing `getdaft-0.1.7/local_dependencies/daft-dsl/src/lit.rs` & `getdaft-0.1.8/local_dependencies/daft-dsl/src/lit.rs`

 * *Files identical despite different names*

### Comparing `getdaft-0.1.7/local_dependencies/daft-dsl/src/optimization.rs` & `getdaft-0.1.8/local_dependencies/daft-dsl/src/optimization.rs`

 * *Files identical despite different names*

### Comparing `getdaft-0.1.7/local_dependencies/daft-dsl/src/pyobject.rs` & `getdaft-0.1.8/local_dependencies/daft-dsl/src/pyobject.rs`

 * *Files identical despite different names*

### Comparing `getdaft-0.1.7/local_dependencies/daft-dsl/src/python.rs` & `getdaft-0.1.8/local_dependencies/daft-dsl/src/python.rs`

 * *Files identical despite different names*

### Comparing `getdaft-0.1.7/Cargo.toml` & `getdaft-0.1.8/Cargo.toml`

 * *Files 1% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 crate-type = [ "cdylib",]
 name = "daft"
 
 [package]
 edition = "2021"
 name = "daft"
 publish = false
-version = "0.1.7"
+version = "0.1.8"
 
 [workspace]
 members = ["local_dependencies/daft-core", "local_dependencies/daft-io", "local_dependencies/daft-dsl", "local_dependencies/daft-table"]
 
 [dependencies.daft-core]
 path = "local_dependencies/daft-core"
 default-features = false
@@ -51,15 +51,15 @@
 
 [workspace.dependencies]
 html-escape = "0.2.13"
 num-derive = "0.3.3"
 num-traits = "0.2"
 prettytable-rs = "0.10"
 rand = "^0.8"
-serde_json = "1.0.96"
+serde_json = "1.0.99"
 
 [workspace.package]
 edition = "2021"
 version = "0.1.0"
 
 [workspace.dependencies.arrow2]
 branch = "clark/expand-casting-support"
```

### Comparing `getdaft-0.1.7/.github/ISSUE_TEMPLATE/bug_report.md` & `getdaft-0.1.8/.github/ISSUE_TEMPLATE/bug_report.md`

 * *Files identical despite different names*

### Comparing `getdaft-0.1.7/.github/ISSUE_TEMPLATE/feature_request.md` & `getdaft-0.1.8/.github/ISSUE_TEMPLATE/feature_request.md`

 * *Files identical despite different names*

### Comparing `getdaft-0.1.7/.github/release-drafter.yml` & `getdaft-0.1.8/.github/release-drafter.yml`

 * *Files identical despite different names*

### Comparing `getdaft-0.1.7/.github/workflows/broken-link-checker.yml` & `getdaft-0.1.8/.github/workflows/broken-link-checker.yml`

 * *Files identical despite different names*

### Comparing `getdaft-0.1.7/.github/workflows/daft-profiling.yml` & `getdaft-0.1.8/.github/workflows/daft-profiling.yml`

 * *Files 1% similar despite different names*

```diff
@@ -24,14 +24,15 @@
     - uses: actions/cache@v3
       env:
         cache-name: cache-cargo-profile
       with:
         path: |
           ~/.cargo/registry
           ~/.cargo/git
+          target
         key: ${{ runner.os }}-build-${{ env.cache-name }}-${{ hashFiles('**/Cargo.lock') }}
         restore-keys: |
           ${{ runner.os }}-build-${{ env.cache-name }}-
           ${{ runner.os }}-build-
           ${{ runner.os }}-
 
     - name: Set up Python ${{ env.PYTHON_VERSION }}
```

### Comparing `getdaft-0.1.7/.github/workflows/notebook-checker.yml` & `getdaft-0.1.8/.github/workflows/notebook-checker.yml`

 * *Files identical despite different names*

### Comparing `getdaft-0.1.7/.github/workflows/property-based-tests.yml` & `getdaft-0.1.8/.github/workflows/property-based-tests.yml`

 * *Files 4% similar despite different names*

```diff
@@ -23,14 +23,15 @@
     - uses: actions/cache@v3
       env:
         cache-name: cache-cargo
       with:
         path: |
           ~/.cargo/registry
           ~/.cargo/git
+          target
         key: ${{ runner.os }}-build-${{ env.cache-name }}-${{ hashFiles('**/Cargo.lock') }}
         restore-keys: |
           ${{ runner.os }}-build-${{ env.cache-name }}-
           ${{ runner.os }}-build-
           ${{ runner.os }}-
 
     - name: Set up Python ${{ matrix.python-version }}
```

### Comparing `getdaft-0.1.7/.github/workflows/python-package.yml` & `getdaft-0.1.8/.github/workflows/python-package.yml`

 * *Files 10% similar despite different names*

```diff
@@ -37,14 +37,15 @@
     - uses: actions/cache@v3
       env:
         cache-name: cache-cargo
       with:
         path: |
           ~/.cargo/registry
           ~/.cargo/git
+          target
         key: ${{ runner.os }}-build-${{ env.cache-name }}-${{ hashFiles('**/Cargo.lock') }}
         restore-keys: |
           ${{ runner.os }}-build-${{ env.cache-name }}-
           ${{ runner.os }}-build-
           ${{ runner.os }}-
     - name: Set up Python ${{ matrix.python-version }}
       uses: actions/setup-python@v4
@@ -119,37 +120,34 @@
       with:
         submodules: true
         fetch-depth: 0
     - uses: actions/setup-python@v4
       with:
         python-version: ${{ matrix.python-version }}
         architecture: x64
-    - run: pip install -U twine toml
+    - run: pip install -U twine toml maturin
     - run: python tools/patch_package_version.py
     - name: Install Rust toolchain
       uses: moonrepo/setup-rust@v0
     - uses: actions/cache@v3
       env:
         cache-name: cache-cargo
       with:
         path: |
           ~/.cargo/registry
           ~/.cargo/git
-        key: ${{ runner.os }}-build-${{ env.cache-name }}-${{ hashFiles('**/Cargo.lock') }}
+          target
+        key: ${{ runner.os }}-integration-build-${{ env.cache-name }}-${{ hashFiles('**/Cargo.lock') }}
         restore-keys: |
-          ${{ runner.os }}-build-${{ env.cache-name }}-
-          ${{ runner.os }}-build-
+          ${{ runner.os }}-integration-build-${{ env.cache-name }}-
+          ${{ runner.os }}-integration-build-
           ${{ runner.os }}-
-    - name: Build wheels - x86
-      uses: messense/maturin-action@v1
-      with:
-        target: x86_64
-        manylinux: auto
-        # NOTE: we don't build with all the actual release optimizations to avoid hellish CI times
-        args: --release --out dist --sdist
+    # NOTE: we don't build with all the actual release optimizations to avoid hellish CI times
+    - name: Build wheels
+      run: maturin build --release --compatibility linux --out dist
     - name: Upload wheels
       uses: actions/upload-artifact@v3
       with:
         name: wheels
         path: dist
 
   integration-test-tpch:
@@ -174,18 +172,22 @@
         python-version: ${{ matrix.python-version }}
         architecture: x64
     - name: Download built wheels
       uses: actions/download-artifact@v3
       with:
         name: wheels
         path: dist
+    - name: Setup Virtual Env
+      run: |
+        python -m venv venv
+        echo "$GITHUB_WORKSPACE/venv/bin" >> $GITHUB_PATH
     - name: Install Daft and dev dependencies
       run: |
-        pip install -r requirements-dev.txt
-        pip install dist/${{ env.package-name }}-*x86_64*.whl --force-reinstall
+        pip install --upgrade pip
+        pip install -r requirements-dev.txt dist/${{ env.package-name }}-*x86_64*.whl --force-reinstall
         rm -rf daft
     - uses: actions/cache@v3
       env:
         cache-name: cache-tpch-data
       with:
         path: data/tpch-dbgen
         key: ${{ runner.os }}-build-${{ env.cache-name }}-${{ hashFiles('tests/integration/test_tpch.py', 'benchmarking/tpch/**') }}
@@ -210,14 +212,83 @@
               }
             ]
           }
       env:
         SLACK_WEBHOOK_URL: ${{ secrets.SLACK_WEBHOOK_URL }}
         SLACK_WEBHOOK_TYPE: INCOMING_WEBHOOK
 
+  integration-test-io:
+    runs-on: ubuntu-latest
+    timeout-minutes: 30
+    needs:
+    - integration-test-build
+    env:
+      package-name: getdaft
+    strategy:
+      fail-fast: false
+      matrix:
+        python-version: ['3.7']
+        daft-runner: [py, ray]
+    steps:
+    - uses: actions/checkout@v3
+      with:
+        submodules: true
+        fetch-depth: 0
+    - uses: actions/setup-python@v4
+      with:
+        python-version: ${{ matrix.python-version }}
+        architecture: x64
+    - name: Download built wheels
+      uses: actions/download-artifact@v3
+      with:
+        name: wheels
+        path: dist
+    - name: Setup Virtual Env
+      run: |
+        python -m venv venv
+        echo "$GITHUB_WORKSPACE/venv/bin" >> $GITHUB_PATH
+    - name: Install Daft and dev dependencies
+      run: |
+        pip install --upgrade pip
+        pip install -r requirements-dev.txt dist/${{ env.package-name }}-*x86_64*.whl --force-reinstall
+        rm -rf daft
+    - name: Prepare tmpdirs for IO services
+      run: |
+        mkdir -p /tmp/daft-integration-testing/nginx
+        chmod +rw /tmp/daft-integration-testing/nginx
+    - name: Spin up IO services
+      uses: isbang/compose-action@v1.4.1
+      with:
+        compose-file: ./tests/integration/docker-compose/docker-compose.yml
+        down-flags: --volumes
+    - name: Run IO integration tests
+      run: |
+        pytest tests/integration/io -m 'integration' --durations=50
+      env:
+        DAFT_RUNNER: ${{ matrix.daft-runner }}
+    - name: Send Slack notification on failure
+      uses: slackapi/slack-github-action@v1.24.0
+      if: ${{ failure() && (github.ref == 'refs/heads/main') }}
+      with:
+        payload: |
+          {
+            "blocks": [
+              {
+                "type": "section",
+                "text": {
+                  "type": "mrkdwn",
+                  "text": ":rotating_light: [CI] IO Integration Tests <${{ github.server_url }}/${{ github.repository }}/actions/runs/${{ github.run_id }}|workflow> *FAILED on main* :rotating_light:"
+                }
+              }
+            ]
+          }
+      env:
+        SLACK_WEBHOOK_URL: ${{ secrets.SLACK_WEBHOOK_URL }}
+        SLACK_WEBHOOK_TYPE: INCOMING_WEBHOOK
+
   rust-tests:
     runs-on: ubuntu-latest
     timeout-minutes: 15
     strategy:
       fail-fast: false
     steps:
     - uses: actions/checkout@v3
@@ -225,18 +296,19 @@
     - uses: actions/cache@v3
       env:
         cache-name: cache-cargo
       with:
         path: |
           ~/.cargo/registry
           ~/.cargo/git
+          target
         key: ${{ runner.os }}-rust-package-${{ env.cache-name }}-${{ hashFiles('**/Cargo.lock') }}
         restore-keys: |
-          ${{ runner.os }}-build-${{ env.cache-name }}-
-          ${{ runner.os }}-build-
+          ${{ runner.os }}-rust-package-${{ env.cache-name }}-
+          ${{ runner.os }}-rust-package-
           ${{ runner.os }}-
     - name: Install cargo-llvm-cov
       uses: taiki-e/install-action@cargo-llvm-cov
     - name: Generate code coverage
       run: mkdir -p report-output && cargo llvm-cov --no-default-features --workspace --lcov --output-path ./report-output/lcov.info
     - name: Upload coverage report
       uses: actions/upload-artifact@v3
@@ -314,14 +386,15 @@
     - uses: actions/cache@v3
       env:
         cache-name: cache-cargo
       with:
         path: |
           ~/.cargo/registry
           ~/.cargo/git
+          target
         key: ${{ runner.os }}-build-${{ env.cache-name }}-${{ hashFiles('**/Cargo.lock') }}
         restore-keys: |
           ${{ runner.os }}-build-${{ env.cache-name }}-
           ${{ runner.os }}-build-
           ${{ runner.os }}-
 
     - name: Set up Python ${{ matrix.python-version }}
@@ -391,14 +464,15 @@
     - uses: actions/cache@v3
       env:
         cache-name: cache-cargo
       with:
         path: |
           ~/.cargo/registry
           ~/.cargo/git
+          target
         key: ${{ runner.os }}-build-${{ env.cache-name }}-${{ hashFiles('**/Cargo.lock') }}
         restore-keys: |
           ${{ runner.os }}-build-${{ env.cache-name }}-
           ${{ runner.os }}-build-
           ${{ runner.os }}-
 
     - uses: actions/cache@v3
```

### Comparing `getdaft-0.1.7/.github/workflows/python-publish.yml` & `getdaft-0.1.8/.github/workflows/python-publish.yml`

 * *Files 6% similar despite different names*

```diff
@@ -75,16 +75,15 @@
         args: --profile release-lto --out dist --sdist
       env:
         RUSTFLAGS: -Ctarget-cpu=apple-m1
 
     - name: Install and test built wheel - x86_64
       if: ${{ matrix.compile_arch == 'x86_64' }}
       run: |
-        pip install -r requirements-dev.txt
-        pip install dist/${{ env.PACKAGE_NAME }}-*x86_64*.whl --force-reinstall
+        pip install -r requirements-dev.txt dist/${{ env.PACKAGE_NAME }}-*x86_64*.whl --force-reinstall
         rm -rf daft
         pytest -v
 
     - name: Upload wheels
       uses: actions/upload-artifact@v3
       with:
         name: wheels
```

### Comparing `getdaft-0.1.7/.github/workflows/ray-compatibility.yml` & `getdaft-0.1.8/.github/workflows/ray-compatibility.yml`

 * *Files 4% similar despite different names*

```diff
@@ -26,14 +26,15 @@
     - uses: actions/cache@v3
       env:
         cache-name: cache-cargo
       with:
         path: |
           ~/.cargo/registry
           ~/.cargo/git
+          target
         key: ${{ runner.os }}-build-${{ env.cache-name }}-${{ hashFiles('**/Cargo.lock') }}
         restore-keys: |
           ${{ runner.os }}-build-${{ env.cache-name }}-
           ${{ runner.os }}-build-
           ${{ runner.os }}-
 
     - name: Set up Python ${{ matrix.python-version }}
```

### Comparing `getdaft-0.1.7/.github/workflows/release-drafter.yml` & `getdaft-0.1.8/.github/workflows/release-drafter.yml`

 * *Files identical despite different names*

### Comparing `getdaft-0.1.7/.pre-commit-config.yaml` & `getdaft-0.1.8/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `getdaft-0.1.7/CONTRIBUTING.md` & `getdaft-0.1.8/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `getdaft-0.1.7/LICENSE` & `getdaft-0.1.8/LICENSE`

 * *Files identical despite different names*

### Comparing `getdaft-0.1.7/Makefile` & `getdaft-0.1.8/Makefile`

 * *Files identical despite different names*

### Comparing `getdaft-0.1.7/README.rst` & `getdaft-0.1.8/README.rst`

 * *Files 6% similar despite different names*

```diff
@@ -22,15 +22,15 @@
 * `License`_
 
 About Daft
 ----------
 
 The Daft dataframe is a table of data with rows and columns. Columns can contain any Python objects, which allows Daft to support rich complex data types such as images, audio, video and more.
 
-1. **Any Data**: Columns can contain any Python objects, which means that the Python libraries you already use for running machine learning or custom data processing will work natively with Daft!
+1. **Any Data**: Beyond the usual strings/numbers/dates, Daft columns can also hold complex multimodal data such as Images, Embeddings and Python objects. Ingestion and basic transformations of complex data is extremely easy and performant in Daft.
 2. **Notebook Computing**: Daft is built for the interactive developer experience on a notebook - intelligent caching/query optimizations accelerates your experimentation and data exploration.
 3. **Distributed Computing**: Rich complex formats such as images can quickly outgrow your local laptop's computational resources - Daft integrates natively with `Ray <https://www.ray.io>`_ for running dataframes on large clusters of machines with thousands of CPUs/GPUs.
 
 Getting Started
 ---------------
 
 Installation
@@ -41,40 +41,29 @@
 For more advanced installations (e.g. installing from source or with extra dependencies such as Ray and AWS utilities), please see our `Installation Guide <https://www.getdaft.io/projects/docs/en/latest/install.html>`_
 
 Quickstart
 ^^^^^^^^^^
 
   Check out our `10-minute quickstart <https://www.getdaft.io/projects/docs/en/latest/learn/10-min.html>`_!
 
-In this example, we load images from an AWS S3 bucket and run a simple function to generate thumbnails for each image:
+In this example, we load images from an AWS S3 bucket's URLs and resize each image in the dataframe:
 
 .. code:: python
 
     import daft as daft
 
-    import io
-    from PIL import Image
-
-    def get_thumbnail(img: Image.Image) -> Image.Image:
-        """Simple function to make an image thumbnail"""
-        imgcopy = img.copy()
-        imgcopy.thumbnail((48, 48))
-        return imgcopy
-
-    # Load a dataframe from files in an S3 bucket
+    # Load a dataframe from filepaths in an S3 bucket
     df = daft.from_glob_path("s3://daft-public-data/laion-sample-images/*")
 
-    # Get the AWS S3 url of each image
-    df = df.select(df["path"].alias("s3_url"))
-
-    # Download images and load as a PIL Image object
-    df = df.with_column("image", df["s3_url"].url.download().apply(lambda data: Image.open(io.BytesIO(data)), return_dtype=daft.DataType.python()))
+    # 1. Download column of image URLs as a column of bytes
+    # 2. Decode the column of bytes into a column of images
+    df = df.with_column("image", df["path"].url.download().image.decode())
 
-    # Generate thumbnails from images
-    df = df.with_column("thumbnail", df["image"].apply(get_thumbnail, return_dtype=daft.DataType.python()))
+    # Resize each image into 32x32
+    df = df.with_column("resized", df["image"].image.resize(32, 32))
 
     df.show(3)
 
 |Quickstart Image|
 
 
 Benchmarks
@@ -133,15 +122,15 @@
 Check out our `dataframe comparison page <https://www.getdaft.io/projects/docs/en/latest/dataframe_comparison.html>`_ for more details!
 
 License
 -------
 
 Daft has an Apache 2.0 license - please see the LICENSE file.
 
-.. |Quickstart Image| image:: https://user-images.githubusercontent.com/17691182/200086119-fb73037b-8b4e-414a-9060-a44122f0c290.png
+.. |Quickstart Image| image:: https://github.com/Eventual-Inc/Daft/assets/17691182/dea2f515-9739-4f3e-ac58-cd96d51e44a8
    :alt: Dataframe code to load a folder of images from AWS S3 and create thumbnails
    :height: 256
 
 .. |Benchmark Image| image:: https://github-production-user-asset-6210df.s3.amazonaws.com/2550285/243524430-338e427d-f049-40b3-b555-4059d6be7bfd.png
    :alt: Benchmarks for SF100 TPCH
 
 .. |Banner| image:: https://user-images.githubusercontent.com/17691182/190476440-28f29e87-8e3b-41c4-9c28-e112e595f558.png
```

### Comparing `getdaft-0.1.7/benchmarking/tpch/__main__.py` & `getdaft-0.1.8/benchmarking/tpch/__main__.py`

 * *Files identical despite different names*

### Comparing `getdaft-0.1.7/benchmarking/tpch/answers.py` & `getdaft-0.1.8/benchmarking/tpch/answers.py`

 * *Files identical despite different names*

### Comparing `getdaft-0.1.7/benchmarking/tpch/data_generation.py` & `getdaft-0.1.8/benchmarking/tpch/data_generation.py`

 * *Files identical despite different names*

### Comparing `getdaft-0.1.7/benchmarking/tpch/pipelined_data_generation.py` & `getdaft-0.1.8/benchmarking/tpch/pipelined_data_generation.py`

 * *Files identical despite different names*

### Comparing `getdaft-0.1.7/benchmarking/tpch/subprefix_s3_files.py` & `getdaft-0.1.8/benchmarking/tpch/subprefix_s3_files.py`

 * *Files identical despite different names*

### Comparing `getdaft-0.1.7/ci/upload_wheels.sh` & `getdaft-0.1.8/ci/upload_wheels.sh`

 * *Files identical despite different names*

### Comparing `getdaft-0.1.7/daft/__init__.py` & `getdaft-0.1.8/daft/__init__.py`

 * *Files identical despite different names*

### Comparing `getdaft-0.1.7/daft/analytics.py` & `getdaft-0.1.8/daft/analytics.py`

 * *Files identical despite different names*

### Comparing `getdaft-0.1.7/daft/api_annotations.py` & `getdaft-0.1.8/daft/api_annotations.py`

 * *Files identical despite different names*

### Comparing `getdaft-0.1.7/daft/arrow_utils.py` & `getdaft-0.1.8/daft/arrow_utils.py`

 * *Files identical despite different names*

### Comparing `getdaft-0.1.7/daft/context.py` & `getdaft-0.1.8/daft/context.py`

 * *Files identical despite different names*

### Comparing `getdaft-0.1.7/daft/convert.py` & `getdaft-0.1.8/daft/convert.py`

 * *Files identical despite different names*

### Comparing `getdaft-0.1.7/daft/daft.pyi` & `getdaft-0.1.8/daft/daft.pyi`

 * *Files identical despite different names*

### Comparing `getdaft-0.1.7/daft/dataframe/dataframe.py` & `getdaft-0.1.8/daft/dataframe/dataframe.py`

 * *Files identical despite different names*

### Comparing `getdaft-0.1.7/daft/dataframe/to_torch.py` & `getdaft-0.1.8/daft/dataframe/to_torch.py`

 * *Files identical despite different names*

### Comparing `getdaft-0.1.7/daft/datasources.py` & `getdaft-0.1.8/daft/datasources.py`

 * *Files identical despite different names*

### Comparing `getdaft-0.1.7/daft/datatype.py` & `getdaft-0.1.8/daft/datatype.py`

 * *Files identical despite different names*

### Comparing `getdaft-0.1.7/daft/execution/execution_step.py` & `getdaft-0.1.8/daft/execution/execution_step.py`

 * *Files identical despite different names*

### Comparing `getdaft-0.1.7/daft/execution/physical_plan.py` & `getdaft-0.1.8/daft/execution/physical_plan.py`

 * *Files identical despite different names*

### Comparing `getdaft-0.1.7/daft/execution/physical_plan_factory.py` & `getdaft-0.1.8/daft/execution/physical_plan_factory.py`

 * *Files identical despite different names*

### Comparing `getdaft-0.1.7/daft/expressions/expressions.py` & `getdaft-0.1.8/daft/expressions/expressions.py`

 * *Files identical despite different names*

### Comparing `getdaft-0.1.7/daft/expressions/testing.py` & `getdaft-0.1.8/daft/expressions/testing.py`

 * *Files identical despite different names*

### Comparing `getdaft-0.1.7/daft/filesystem.py` & `getdaft-0.1.8/daft/filesystem.py`

 * *Files identical despite different names*

### Comparing `getdaft-0.1.7/daft/internal/rule.py` & `getdaft-0.1.8/daft/internal/rule.py`

 * *Files identical despite different names*

### Comparing `getdaft-0.1.7/daft/internal/rule_runner.py` & `getdaft-0.1.8/daft/internal/rule_runner.py`

 * *Files identical despite different names*

### Comparing `getdaft-0.1.7/daft/internal/treenode.py` & `getdaft-0.1.8/daft/internal/treenode.py`

 * *Files identical despite different names*

### Comparing `getdaft-0.1.7/daft/io/_csv.py` & `getdaft-0.1.8/daft/io/_csv.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 # isort: dont-add-import: from __future__ import annotations
 
-from typing import Dict, List, Optional
+from typing import Dict, List, Optional, Union
 
 import fsspec
 
 from daft.api_annotations import PublicAPI
 from daft.dataframe import DataFrame
 from daft.datasources import CSVSourceInfo
 from daft.datatype import DataType
 from daft.io.common import _get_tabular_files_scan
 
 
 @PublicAPI
 def read_csv(
-    path: str,
+    path: Union[str, List[str]],
     schema_hints: Optional[Dict[str, DataType]] = None,
     fs: Optional[fsspec.AbstractFileSystem] = None,
     has_headers: bool = True,
     column_names: Optional[List[str]] = None,
     delimiter: str = ",",
 ) -> DataFrame:
     """Creates a DataFrame from CSV file(s)
@@ -43,14 +43,16 @@
     if column_names is not None:
         raise NotImplementedError(
             "The `column_names` option has been deprecated. As an alternative, you may specify `has_headers=False` which will have Daft "
             "autogenerate your column names. Then, you can use `df.select` to alias each of the autogenerated columns: "
             "`df.select(*[col(old).alias(new) for old, new in zip(df.column_names, MY_COL_NAMES)])`. Please submit an issue if this is a "
             "blocker for your workflow!"
         )
+    if isinstance(path, list) and len(path) == 0:
+        raise ValueError(f"Cannot read DataFrame from from empty list of CSV filepaths")
 
     plan = _get_tabular_files_scan(
         path,
         schema_hints,
         CSVSourceInfo(
             delimiter=delimiter,
             has_headers=has_headers,
```

### Comparing `getdaft-0.1.7/daft/io/_json.py` & `getdaft-0.1.8/daft/io/_json.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 # isort: dont-add-import: from __future__ import annotations
 
-from typing import Dict, Optional
+from typing import Dict, List, Optional, Union
 
 import fsspec
 
 from daft.api_annotations import PublicAPI
 from daft.dataframe import DataFrame
 from daft.datasources import JSONSourceInfo
 from daft.datatype import DataType
 from daft.io.common import _get_tabular_files_scan
 
 
 @PublicAPI
 def read_json(
-    path: str,
+    path: Union[str, List[str]],
     schema_hints: Optional[Dict[str, DataType]] = None,
     fs: Optional[fsspec.AbstractFileSystem] = None,
 ) -> DataFrame:
     """Creates a DataFrame from line-delimited JSON file(s)
 
     Example:
         >>> df = daft.read_json("/path/to/file.json")
@@ -31,14 +31,17 @@
             disable all schema inference on data being read, and throw an error if data being read is incompatible.
         fs (fsspec.AbstractFileSystem): fsspec FileSystem to use for reading data.
             By default, Daft will automatically construct a FileSystem instance internally.
 
     returns:
         DataFrame: parsed DataFrame
     """
+    if isinstance(path, list) and len(path) == 0:
+        raise ValueError(f"Cannot read DataFrame from from empty list of JSON filepaths")
+
     plan = _get_tabular_files_scan(
         path,
         schema_hints,
         JSONSourceInfo(),
         fs,
     )
     return DataFrame(plan)
```

### Comparing `getdaft-0.1.7/daft/io/common.py` & `getdaft-0.1.8/daft/io/common.py`

 * *Files 9% similar despite different names*

```diff
@@ -13,23 +13,25 @@
     if isinstance(hints, dict):
         return Schema._from_field_name_and_types([(fname, dtype) for fname, dtype in hints.items()])
     else:
         raise NotImplementedError(f"Unsupported schema hints: {type(hints)}")
 
 
 def _get_tabular_files_scan(
-    path: str,
+    path: str | list[str],
     schema_hints: dict[str, DataType] | None,
     source_info: SourceInfo,
     fs: fsspec.AbstractFileSystem | None,
 ) -> logical_plan.TabularFilesScan:
     """Returns a TabularFilesScan LogicalPlan for a given glob filepath."""
     # Glob the path using the Runner
     runner_io = get_context().runner().runner_io()
-    listing_details_partition_set = runner_io.glob_paths_details(path, source_info, fs)
+
+    paths = path if isinstance(path, list) else [str(path)]
+    listing_details_partition_set = runner_io.glob_paths_details(paths, source_info, fs)
 
     # Infer schema if no hints provided
     inferred_or_provided_schema = (
         _get_schema_from_hints(schema_hints)
         if schema_hints is not None
         else runner_io.get_schema_from_first_filepath(listing_details_partition_set, source_info, fs)
     )
```

### Comparing `getdaft-0.1.7/daft/io/file_path.py` & `getdaft-0.1.8/daft/io/file_path.py`

 * *Files 1% similar despite different names*

```diff
@@ -38,15 +38,15 @@
             By default, Daft will automatically construct a FileSystem instance internally.
 
     Returns:
         DataFrame: DataFrame containing the path to each file as a row, along with other metadata
             parsed from the provided filesystem.
     """
     runner_io = get_context().runner().runner_io()
-    partition_set = runner_io.glob_paths_details(path, fs=fs)
+    partition_set = runner_io.glob_paths_details([path], fs=fs)
     cache_entry = get_context().runner().put_partition_set_into_cache(partition_set)
     filepath_plan = logical_plan.InMemoryScan(
         cache_entry=cache_entry,
         schema=runner_io.FS_LISTING_SCHEMA,
         partition_spec=logical_plan.PartitionSpec(logical_plan.PartitionScheme.UNKNOWN, partition_set.num_partitions()),
     )
     return DataFrame(filepath_plan)
```

### Comparing `getdaft-0.1.7/daft/io/parquet.py` & `getdaft-0.1.8/daft/io/parquet.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 # isort: dont-add-import: from __future__ import annotations
 
-from typing import Dict, Optional
+from typing import Dict, List, Optional, Union
 
 import fsspec
 
 from daft.api_annotations import PublicAPI
 from daft.dataframe import DataFrame
 from daft.datasources import ParquetSourceInfo
 from daft.datatype import DataType
 from daft.io.common import _get_tabular_files_scan
 
 
 @PublicAPI
 def read_parquet(
-    path: str,
+    path: Union[str, List[str]],
     schema_hints: Optional[Dict[str, DataType]] = None,
     fs: Optional[fsspec.AbstractFileSystem] = None,
 ) -> DataFrame:
     """Creates a DataFrame from Parquet file(s)
 
     Example:
         >>> df = daft.read_parquet("/path/to/file.parquet")
@@ -31,14 +31,17 @@
             disable all schema inference on data being read, and throw an error if data being read is incompatible.
         fs (fsspec.AbstractFileSystem): fsspec FileSystem to use for reading data.
             By default, Daft will automatically construct a FileSystem instance internally.
 
     returns:
         DataFrame: parsed DataFrame
     """
+    if isinstance(path, list) and len(path) == 0:
+        raise ValueError(f"Cannot read DataFrame from from empty list of Parquet filepaths")
+
     plan = _get_tabular_files_scan(
         path,
         schema_hints,
         ParquetSourceInfo(),
         fs,
     )
     return DataFrame(plan)
```

### Comparing `getdaft-0.1.7/daft/logical/aggregation_plan_builder.py` & `getdaft-0.1.8/daft/logical/aggregation_plan_builder.py`

 * *Files identical despite different names*

### Comparing `getdaft-0.1.7/daft/logical/logical_plan.py` & `getdaft-0.1.8/daft/logical/logical_plan.py`

 * *Files identical despite different names*

### Comparing `getdaft-0.1.7/daft/logical/map_partition_ops.py` & `getdaft-0.1.8/daft/logical/map_partition_ops.py`

 * *Files identical despite different names*

### Comparing `getdaft-0.1.7/daft/logical/optimizer.py` & `getdaft-0.1.8/daft/logical/optimizer.py`

 * *Files identical despite different names*

### Comparing `getdaft-0.1.7/daft/logical/schema.py` & `getdaft-0.1.8/daft/logical/schema.py`

 * *Files identical despite different names*

### Comparing `getdaft-0.1.7/daft/pickle/cloudpickle.py` & `getdaft-0.1.8/daft/pickle/cloudpickle.py`

 * *Files identical despite different names*

### Comparing `getdaft-0.1.7/daft/pickle/cloudpickle_fast.py` & `getdaft-0.1.8/daft/pickle/cloudpickle_fast.py`

 * *Files identical despite different names*

### Comparing `getdaft-0.1.7/daft/pickle/compat.py` & `getdaft-0.1.8/daft/pickle/compat.py`

 * *Files identical despite different names*

### Comparing `getdaft-0.1.7/daft/resource_request.py` & `getdaft-0.1.8/daft/resource_request.py`

 * *Files identical despite different names*

### Comparing `getdaft-0.1.7/daft/runners/partitioning.py` & `getdaft-0.1.8/daft/runners/partitioning.py`

 * *Files identical despite different names*

### Comparing `getdaft-0.1.7/daft/runners/profiler.py` & `getdaft-0.1.8/daft/runners/profiler.py`

 * *Files identical despite different names*

### Comparing `getdaft-0.1.7/daft/runners/pyrunner.py` & `getdaft-0.1.8/daft/runners/pyrunner.py`

 * *Files 2% similar despite different names*

```diff
@@ -78,32 +78,36 @@
     def wait(self) -> None:
         pass
 
 
 class PyRunnerIO(runner_io.RunnerIO[Table]):
     def glob_paths_details(
         self,
-        source_path: str,
+        source_paths: list[str],
         source_info: SourceInfo | None = None,
         fs: fsspec.AbstractFileSystem | None = None,
     ) -> LocalPartitionSet:
-        if fs is None:
-            fs = get_filesystem_from_path(source_path)
+        all_files_infos = []
+        for source_path in source_paths:
+            if fs is None:
+                fs = get_filesystem_from_path(source_path)
 
-        files_info = glob_path_with_stats(source_path, source_info, fs)
+            files_info = glob_path_with_stats(source_path, source_info, fs)
 
-        if len(files_info) == 0:
-            raise FileNotFoundError(f"No files found at {source_path}")
+            if len(files_info) == 0:
+                raise FileNotFoundError(f"No files found at {source_path}")
+
+            all_files_infos.extend(files_info)
 
         partition = Table.from_pydict(
             {
-                "path": pa.array([file_info.path for file_info in files_info], type=pa.string()),
-                "size": pa.array([file_info.size for file_info in files_info], type=pa.int64()),
-                "type": pa.array([file_info.type for file_info in files_info], type=pa.string()),
-                "rows": pa.array([file_info.rows for file_info in files_info], type=pa.int64()),
+                "path": pa.array([file_info.path for file_info in all_files_infos], type=pa.string()),
+                "size": pa.array([file_info.size for file_info in all_files_infos], type=pa.int64()),
+                "type": pa.array([file_info.type for file_info in all_files_infos], type=pa.string()),
+                "rows": pa.array([file_info.rows for file_info in all_files_infos], type=pa.int64()),
             },
         )
 
         # Make sure that the schema is consistent with what we expect
         assert (
             partition.schema() == PyRunnerIO.FS_LISTING_SCHEMA
         ), f"Schema should be expected: {PyRunnerIO.FS_LISTING_SCHEMA}, but received: {partition.schema()}"
```

### Comparing `getdaft-0.1.7/daft/runners/ray_runner.py` & `getdaft-0.1.8/daft/runners/ray_runner.py`

 * *Files 2% similar despite different names*

```diff
@@ -72,33 +72,36 @@
 from daft.logical.schema import Schema
 
 RAY_VERSION = tuple(int(s) for s in ray.__version__.split("."))
 
 
 @ray.remote
 def _glob_path_into_details_vpartitions(
-    path: str,
+    paths: list[str],
     schema: Schema,
     source_info: SourceInfo | None,
     fs: fsspec.AbstractFileSystem | None,
 ) -> list[tuple[PartID, Table]]:
-    if fs is None:
-        fs = get_filesystem_from_path(path)
-
-    listing_infos = glob_path_with_stats(path, source_info, fs)
-    if len(listing_infos) == 0:
-        raise FileNotFoundError(f"No files found at {path}")
+    all_listing_infos = []
+    for path in paths:
+        if fs is None:
+            fs = get_filesystem_from_path(path)
+
+        listing_infos = glob_path_with_stats(path, source_info, fs)
+        if len(listing_infos) == 0:
+            raise FileNotFoundError(f"No files found at {path}")
+        all_listing_infos.extend(listing_infos)
 
     # Hardcoded to 1 partition
     partition = Table.from_pydict(
         {
-            "path": pa.array([file_info.path for file_info in listing_infos], type=pa.string()),
-            "size": pa.array([file_info.size for file_info in listing_infos], type=pa.int64()),
-            "type": pa.array([file_info.type for file_info in listing_infos], type=pa.string()),
-            "rows": pa.array([file_info.rows for file_info in listing_infos], type=pa.int64()),
+            "path": pa.array([file_info.path for file_info in all_listing_infos], type=pa.string()),
+            "size": pa.array([file_info.size for file_info in all_listing_infos], type=pa.int64()),
+            "type": pa.array([file_info.type for file_info in all_listing_infos], type=pa.string()),
+            "rows": pa.array([file_info.rows for file_info in all_listing_infos], type=pa.int64()),
         },
     )
     assert partition.schema() == schema, f"Schema should be expected: {schema}, but received: {partition.schema()}"
 
     partition_ref = ray.put(partition)
     partition_refs = [(0, partition_ref)]
 
@@ -227,20 +230,20 @@
     def wait(self) -> None:
         ray.wait([o for o in self._partitions.values()])
 
 
 class RayRunnerIO(runner_io.RunnerIO[ray.ObjectRef]):
     def glob_paths_details(
         self,
-        source_path: str,
+        source_paths: list[str],
         source_info: SourceInfo | None = None,
         fs: fsspec.AbstractFileSystem | None = None,
     ) -> RayPartitionSet:
         partition_refs = ray.get(
-            _glob_path_into_details_vpartitions.remote(source_path, RayRunnerIO.FS_LISTING_SCHEMA, source_info, fs=fs)
+            _glob_path_into_details_vpartitions.remote(source_paths, RayRunnerIO.FS_LISTING_SCHEMA, source_info, fs=fs)
         )
         return RayPartitionSet({part_id: part for part_id, part in partition_refs})
 
     def get_schema_from_first_filepath(
         self,
         listing_details_partitions: PartitionSet[ray.ObjectRef],
         source_info: SourceInfo,
```

### Comparing `getdaft-0.1.7/daft/runners/runner.py` & `getdaft-0.1.8/daft/runners/runner.py`

 * *Files identical despite different names*

### Comparing `getdaft-0.1.7/daft/runners/runner_io.py` & `getdaft-0.1.8/daft/runners/runner_io.py`

 * *Files 2% similar despite different names*

```diff
@@ -42,15 +42,15 @@
             (FS_LISTING_ROWS_COLUMN_NAME, DataType.int64()),
         ]
     )
 
     @abstractmethod
     def glob_paths_details(
         self,
-        source_path: str,
+        source_path: list[str],
         source_info: SourceInfo | None = None,
         fs: fsspec.AbstractFileSystem | None = None,
     ) -> PartitionSet[PartitionT]:
         """Globs the specified filepath to construct Partitions containing file and dir metadata
 
         Args:
             source_path (str): path to glob
```

### Comparing `getdaft-0.1.7/daft/series.py` & `getdaft-0.1.8/daft/series.py`

 * *Files identical despite different names*

### Comparing `getdaft-0.1.7/daft/table/schema_inference.py` & `getdaft-0.1.8/daft/table/schema_inference.py`

 * *Files identical despite different names*

### Comparing `getdaft-0.1.7/daft/table/table.py` & `getdaft-0.1.8/daft/table/table.py`

 * *Files identical despite different names*

### Comparing `getdaft-0.1.7/daft/table/table_io.py` & `getdaft-0.1.8/daft/table/table_io.py`

 * *Files identical despite different names*

### Comparing `getdaft-0.1.7/daft/udf.py` & `getdaft-0.1.8/daft/udf.py`

 * *Files identical despite different names*

### Comparing `getdaft-0.1.7/daft/udf_library/url_udfs.py` & `getdaft-0.1.8/daft/udf_library/url_udfs.py`

 * *Files identical despite different names*

### Comparing `getdaft-0.1.7/daft/utils.py` & `getdaft-0.1.8/daft/utils.py`

 * *Files identical despite different names*

### Comparing `getdaft-0.1.7/daft/viz/dataframe_display.py` & `getdaft-0.1.8/daft/viz/dataframe_display.py`

 * *Files identical despite different names*

### Comparing `getdaft-0.1.7/daft/viz/html_viz_hooks.py` & `getdaft-0.1.8/daft/viz/html_viz_hooks.py`

 * *Files identical despite different names*

### Comparing `getdaft-0.1.7/docs/Makefile` & `getdaft-0.1.8/docs/Makefile`

 * *Files identical despite different names*

### Comparing `getdaft-0.1.7/docs/source/10-min.ipynb` & `getdaft-0.1.8/docs/source/10-min.ipynb`

 * *Files identical despite different names*

### Comparing `getdaft-0.1.7/docs/source/_static/daft-favicon.png` & `getdaft-0.1.8/docs/source/_static/daft-favicon.png`

 * *Files identical despite different names*

### Comparing `getdaft-0.1.7/docs/source/_static/daft-logo.png` & `getdaft-0.1.8/docs/source/_static/daft-logo.png`

 * *Files identical despite different names*

### Comparing `getdaft-0.1.7/docs/source/_static/daft_illustration.png` & `getdaft-0.1.8/docs/source/_static/daft_illustration.png`

 * *Files identical despite different names*

### Comparing `getdaft-0.1.7/docs/source/_static/dataframe-comp-table.csv` & `getdaft-0.1.8/docs/source/_static/dataframe-comp-table.csv`

 * *Files identical despite different names*

### Comparing `getdaft-0.1.7/docs/source/_static/execution_model.png` & `getdaft-0.1.8/docs/source/_static/execution_model.png`

 * *Files identical despite different names*

### Comparing `getdaft-0.1.7/docs/source/_static/header.css` & `getdaft-0.1.8/docs/source/_static/header.css`

 * *Files identical despite different names*

### Comparing `getdaft-0.1.7/docs/source/_static/high_level_architecture.png` & `getdaft-0.1.8/docs/source/_static/high_level_architecture.png`

 * *Files identical despite different names*

### Comparing `getdaft-0.1.7/docs/source/_static/in_memory_data_representation.png` & `getdaft-0.1.8/docs/source/_static/in_memory_data_representation.png`

 * *Files identical despite different names*

### Comparing `getdaft-0.1.7/docs/source/_static/mobile-menu.js` & `getdaft-0.1.8/docs/source/_static/mobile-menu.js`

 * *Files identical despite different names*

### Comparing `getdaft-0.1.7/docs/source/_static/tpch-1000sf.html` & `getdaft-0.1.8/docs/source/_static/tpch-1000sf.html`

 * *Files identical despite different names*

### Comparing `getdaft-0.1.7/docs/source/_static/tpch-100sf.html` & `getdaft-0.1.8/docs/source/_static/tpch-100sf.html`

 * *Files identical despite different names*

### Comparing `getdaft-0.1.7/docs/source/_static/tpch-nodes-count-daft-1000-sf.html` & `getdaft-0.1.8/docs/source/_static/tpch-nodes-count-daft-1000-sf.html`

 * *Files identical despite different names*

### Comparing `getdaft-0.1.7/docs/source/_templates/layout.html` & `getdaft-0.1.8/docs/source/_templates/layout.html`

 * *Files identical despite different names*

### Comparing `getdaft-0.1.7/docs/source/_templates/sections/header.html` & `getdaft-0.1.8/docs/source/_templates/sections/header.html`

 * *Files identical despite different names*

### Comparing `getdaft-0.1.7/docs/source/_templates/sections/mobile-menu.html` & `getdaft-0.1.8/docs/source/_templates/sections/mobile-menu.html`

 * *Files identical despite different names*

### Comparing `getdaft-0.1.7/docs/source/api_docs/dataframe.rst` & `getdaft-0.1.8/docs/source/api_docs/dataframe.rst`

 * *Files identical despite different names*

### Comparing `getdaft-0.1.7/docs/source/api_docs/datatype.rst` & `getdaft-0.1.8/docs/source/api_docs/datatype.rst`

 * *Files identical despite different names*

### Comparing `getdaft-0.1.7/docs/source/api_docs/expressions.rst` & `getdaft-0.1.8/docs/source/api_docs/expressions.rst`

 * *Files identical despite different names*

### Comparing `getdaft-0.1.7/docs/source/api_docs/groupby.rst` & `getdaft-0.1.8/docs/source/api_docs/groupby.rst`

 * *Files identical despite different names*

### Comparing `getdaft-0.1.7/docs/source/api_docs/input_output.rst` & `getdaft-0.1.8/docs/source/api_docs/input_output.rst`

 * *Files identical despite different names*

### Comparing `getdaft-0.1.7/docs/source/benchmarks/index.rst` & `getdaft-0.1.8/docs/source/benchmarks/index.rst`

 * *Files identical despite different names*

### Comparing `getdaft-0.1.7/docs/source/conf.py` & `getdaft-0.1.8/docs/source/conf.py`

 * *Files identical despite different names*

### Comparing `getdaft-0.1.7/docs/source/dataframe_comparison.rst` & `getdaft-0.1.8/docs/source/dataframe_comparison.rst`

 * *Files identical despite different names*

### Comparing `getdaft-0.1.7/docs/source/index.rst` & `getdaft-0.1.8/docs/source/index.rst`

 * *Files identical despite different names*

### Comparing `getdaft-0.1.7/docs/source/install.rst` & `getdaft-0.1.8/docs/source/install.rst`

 * *Files identical despite different names*

### Comparing `getdaft-0.1.7/docs/source/learn/index.rst` & `getdaft-0.1.8/docs/source/learn/index.rst`

 * *Files identical despite different names*

### Comparing `getdaft-0.1.7/docs/source/learn/key_concepts.rst` & `getdaft-0.1.8/docs/source/learn/key_concepts.rst`

 * *Files identical despite different names*

### Comparing `getdaft-0.1.7/docs/source/learn/tutorials.rst` & `getdaft-0.1.8/docs/source/learn/tutorials.rst`

 * *Files identical despite different names*

### Comparing `getdaft-0.1.7/docs/source/learn/user_guides/aggregations.rst` & `getdaft-0.1.8/docs/source/learn/user_guides/aggregations.rst`

 * *Files identical despite different names*

### Comparing `getdaft-0.1.7/docs/source/learn/user_guides/dataframe-operations.rst` & `getdaft-0.1.8/docs/source/learn/user_guides/dataframe-operations.rst`

 * *Files identical despite different names*

### Comparing `getdaft-0.1.7/docs/source/learn/user_guides/datatypes.rst` & `getdaft-0.1.8/docs/source/learn/user_guides/datatypes.rst`

 * *Files identical despite different names*

### Comparing `getdaft-0.1.7/docs/source/learn/user_guides/expressions.rst` & `getdaft-0.1.8/docs/source/learn/user_guides/expressions.rst`

 * *Files identical despite different names*

### Comparing `getdaft-0.1.7/docs/source/learn/user_guides/intro-dataframes.rst` & `getdaft-0.1.8/docs/source/learn/user_guides/intro-dataframes.rst`

 * *Files identical despite different names*

### Comparing `getdaft-0.1.7/docs/source/learn/user_guides/read-write.rst` & `getdaft-0.1.8/docs/source/learn/user_guides/read-write.rst`

 * *Files identical despite different names*

### Comparing `getdaft-0.1.7/docs/source/learn/user_guides/scaling-up.rst` & `getdaft-0.1.8/docs/source/learn/user_guides/scaling-up.rst`

 * *Files identical despite different names*

### Comparing `getdaft-0.1.7/docs/source/learn/user_guides/udf.rst` & `getdaft-0.1.8/docs/source/learn/user_guides/udf.rst`

 * *Files identical despite different names*

### Comparing `getdaft-0.1.7/docs/source/learn/user_guides.rst` & `getdaft-0.1.8/docs/source/learn/user_guides.rst`

 * *Files identical despite different names*

### Comparing `getdaft-0.1.7/docs/source/technical_architecture.rst` & `getdaft-0.1.8/docs/source/technical_architecture.rst`

 * *Files identical despite different names*

### Comparing `getdaft-0.1.7/docs/source/telemetry.rst` & `getdaft-0.1.8/docs/source/telemetry.rst`

 * *Files identical despite different names*

### Comparing `getdaft-0.1.7/pyproject.toml` & `getdaft-0.1.8/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -70,12 +70,12 @@
 
 [[tool.mypy.overrides]]
 enable_error_code = ["attr-defined"]
 module = 'daft.*'
 warn_return_any = false
 
 [tool.pytest.ini_options]
-addopts = "--benchmark-skip -m 'not hypothesis'"
+addopts = "--benchmark-skip -m 'not hypothesis' -m 'not integration'"
 minversion = "6.0"
 testpaths = [
   "tests"
 ]
```

### Comparing `getdaft-0.1.7/src/lib.rs` & `getdaft-0.1.8/src/lib.rs`

 * *Files identical despite different names*

### Comparing `getdaft-0.1.7/tests/assets/tpch-sqlite-queries/1.sql` & `getdaft-0.1.8/tests/assets/tpch-sqlite-queries/1.sql`

 * *Files identical despite different names*

### Comparing `getdaft-0.1.7/tests/assets/tpch-sqlite-queries/10.sql` & `getdaft-0.1.8/tests/assets/tpch-sqlite-queries/10.sql`

 * *Files identical despite different names*

### Comparing `getdaft-0.1.7/tests/assets/tpch-sqlite-queries/2.sql` & `getdaft-0.1.8/tests/assets/tpch-sqlite-queries/2.sql`

 * *Files identical despite different names*

### Comparing `getdaft-0.1.7/tests/assets/tpch-sqlite-queries/7.sql` & `getdaft-0.1.8/tests/assets/tpch-sqlite-queries/7.sql`

 * *Files identical despite different names*

### Comparing `getdaft-0.1.7/tests/assets/tpch-sqlite-queries/8.sql` & `getdaft-0.1.8/tests/assets/tpch-sqlite-queries/8.sql`

 * *Files identical despite different names*

### Comparing `getdaft-0.1.7/tests/assets/tpch-sqlite-queries/9.sql` & `getdaft-0.1.8/tests/assets/tpch-sqlite-queries/9.sql`

 * *Files identical despite different names*

### Comparing `getdaft-0.1.7/tests/benchmarks/conftest.py` & `getdaft-0.1.8/tests/benchmarks/conftest.py`

 * *Files identical despite different names*

### Comparing `getdaft-0.1.7/tests/benchmarks/test_df_arithmetic.py` & `getdaft-0.1.8/tests/benchmarks/test_df_arithmetic.py`

 * *Files identical despite different names*

### Comparing `getdaft-0.1.7/tests/benchmarks/test_file_read.py` & `getdaft-0.1.8/tests/benchmarks/test_file_read.py`

 * *Files identical despite different names*

### Comparing `getdaft-0.1.7/tests/benchmarks/test_groups_and_aggs.py` & `getdaft-0.1.8/tests/benchmarks/test_groups_and_aggs.py`

 * *Files identical despite different names*

### Comparing `getdaft-0.1.7/tests/benchmarks/test_join.py` & `getdaft-0.1.8/tests/benchmarks/test_join.py`

 * *Files identical despite different names*

### Comparing `getdaft-0.1.7/tests/benchmarks/test_repartition.py` & `getdaft-0.1.8/tests/benchmarks/test_repartition.py`

 * *Files identical despite different names*

### Comparing `getdaft-0.1.7/tests/benchmarks/test_sort.py` & `getdaft-0.1.8/tests/benchmarks/test_sort.py`

 * *Files identical despite different names*

### Comparing `getdaft-0.1.7/tests/conftest.py` & `getdaft-0.1.8/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `getdaft-0.1.7/tests/cookbook/assets/311-service-requests.24.csv` & `getdaft-0.1.8/tests/cookbook/assets/311-service-requests.24.csv`

 * *Files identical despite different names*

### Comparing `getdaft-0.1.7/tests/cookbook/assets/images/0000.jpg` & `getdaft-0.1.8/tests/cookbook/assets/images/0000.jpg`

 * *Files identical despite different names*

### Comparing `getdaft-0.1.7/tests/cookbook/assets/images/0007.jpg` & `getdaft-0.1.8/tests/cookbook/assets/images/0007.jpg`

 * *Files identical despite different names*

### Comparing `getdaft-0.1.7/tests/cookbook/assets/images/0018.png` & `getdaft-0.1.8/tests/cookbook/assets/images/0018.png`

 * *Files identical despite different names*

### Comparing `getdaft-0.1.7/tests/cookbook/assets/images/0025.tiff` & `getdaft-0.1.8/tests/cookbook/assets/images/0025.tiff`

 * *Files identical despite different names*

### Comparing `getdaft-0.1.7/tests/cookbook/conftest.py` & `getdaft-0.1.8/tests/cookbook/conftest.py`

 * *Files identical despite different names*

### Comparing `getdaft-0.1.7/tests/cookbook/test_aggregations.py` & `getdaft-0.1.8/tests/cookbook/test_aggregations.py`

 * *Files identical despite different names*

### Comparing `getdaft-0.1.7/tests/cookbook/test_computations.py` & `getdaft-0.1.8/tests/cookbook/test_computations.py`

 * *Files identical despite different names*

### Comparing `getdaft-0.1.7/tests/cookbook/test_count_rows.py` & `getdaft-0.1.8/tests/cookbook/test_count_rows.py`

 * *Files identical despite different names*

### Comparing `getdaft-0.1.7/tests/cookbook/test_dataloading.py` & `getdaft-0.1.8/tests/cookbook/test_dataloading.py`

 * *Files identical despite different names*

### Comparing `getdaft-0.1.7/tests/cookbook/test_distinct.py` & `getdaft-0.1.8/tests/cookbook/test_distinct.py`

 * *Files identical despite different names*

### Comparing `getdaft-0.1.7/tests/cookbook/test_filter.py` & `getdaft-0.1.8/tests/cookbook/test_filter.py`

 * *Files identical despite different names*

### Comparing `getdaft-0.1.7/tests/cookbook/test_image.py` & `getdaft-0.1.8/tests/cookbook/test_image.py`

 * *Files identical despite different names*

### Comparing `getdaft-0.1.7/tests/cookbook/test_joins.py` & `getdaft-0.1.8/tests/cookbook/test_joins.py`

 * *Files identical despite different names*

### Comparing `getdaft-0.1.7/tests/cookbook/test_literals.py` & `getdaft-0.1.8/tests/cookbook/test_literals.py`

 * *Files identical despite different names*

### Comparing `getdaft-0.1.7/tests/cookbook/test_pandas_cookbook.py` & `getdaft-0.1.8/tests/cookbook/test_pandas_cookbook.py`

 * *Files identical despite different names*

### Comparing `getdaft-0.1.7/tests/cookbook/test_sorting.py` & `getdaft-0.1.8/tests/cookbook/test_sorting.py`

 * *Files identical despite different names*

### Comparing `getdaft-0.1.7/tests/cookbook/test_write.py` & `getdaft-0.1.8/tests/cookbook/test_write.py`

 * *Files identical despite different names*

### Comparing `getdaft-0.1.7/tests/dataframe/conftest.py` & `getdaft-0.1.8/tests/dataframe/conftest.py`

 * *Files identical despite different names*

### Comparing `getdaft-0.1.7/tests/dataframe/test_accessors.py` & `getdaft-0.1.8/tests/dataframe/test_accessors.py`

 * *Files identical despite different names*

### Comparing `getdaft-0.1.7/tests/dataframe/test_aggregations.py` & `getdaft-0.1.8/tests/dataframe/test_aggregations.py`

 * *Files identical despite different names*

### Comparing `getdaft-0.1.7/tests/dataframe/test_creation.py` & `getdaft-0.1.8/tests/dataframe/test_creation.py`

 * *Files 2% similar despite different names*

```diff
@@ -64,14 +64,23 @@
 
 
 def test_wrong_input_type():
     with pytest.raises(APITypeError):
         daft.from_pydict("invalid input")
 
 
+def test_create_dataframe_empty_list() -> None:
+    with pytest.raises(ValueError):
+        daft.read_parquet([])
+    with pytest.raises(ValueError):
+        daft.read_csv([])
+    with pytest.raises(ValueError):
+        daft.read_json([])
+
+
 ###
 # List tests
 ###
 
 
 def test_create_dataframe_list(valid_data: list[dict[str, float]]) -> None:
     df = daft.from_pylist(valid_data)
@@ -350,14 +359,31 @@
         assert df.column_names == COL_NAMES
 
         pd_df = df.to_pandas()
         assert list(pd_df.columns) == COL_NAMES
         assert len(pd_df) == len(valid_data)
 
 
+def test_create_dataframe_multiple_csvs(valid_data: list[dict[str, float]]) -> None:
+    with tempfile.NamedTemporaryFile("w") as f1, tempfile.NamedTemporaryFile("w") as f2:
+        for f in (f1, f2):
+            header = list(valid_data[0].keys())
+            writer = csv.writer(f)
+            writer.writerow(header)
+            writer.writerows([[item[col] for col in header] for item in valid_data])
+            f.flush()
+
+        df = daft.read_csv([f1.name, f2.name])
+        assert df.column_names == COL_NAMES
+
+        pd_df = df.to_pandas()
+        assert list(pd_df.columns) == COL_NAMES
+        assert len(pd_df) == (len(valid_data) * 2)
+
+
 @pytest.mark.skipif(get_context().runner_config.name not in {"py"}, reason="requires PyRunner to be in use")
 def test_create_dataframe_csv_custom_fs(valid_data: list[dict[str, float]]) -> None:
     with tempfile.NamedTemporaryFile("w") as f:
         header = list(valid_data[0].keys())
         writer = csv.writer(f)
         writer.writerow(header)
         writer.writerows([[item[col] for col in header] for item in valid_data])
@@ -504,14 +530,30 @@
         assert df.column_names == COL_NAMES
 
         pd_df = df.to_pandas()
         assert list(pd_df.columns) == COL_NAMES
         assert len(pd_df) == len(valid_data)
 
 
+def test_create_dataframe_multiple_jsons(valid_data: list[dict[str, float]]) -> None:
+    with tempfile.NamedTemporaryFile("w") as f1, tempfile.NamedTemporaryFile("w") as f2:
+        for f in (f1, f2):
+            for data in valid_data:
+                f.write(json.dumps(data))
+                f.write("\n")
+            f.flush()
+
+        df = daft.read_json([f1.name, f2.name])
+        assert df.column_names == COL_NAMES
+
+        pd_df = df.to_pandas()
+        assert list(pd_df.columns) == COL_NAMES
+        assert len(pd_df) == (len(valid_data) * 2)
+
+
 @pytest.mark.skipif(get_context().runner_config.name not in {"py"}, reason="requires PyRunner to be in use")
 def test_create_dataframe_json_custom_fs(valid_data: list[dict[str, float]]) -> None:
     with tempfile.NamedTemporaryFile("w") as f:
         for data in valid_data:
             f.write(json.dumps(data))
             f.write("\n")
         f.flush()
@@ -603,14 +645,29 @@
         assert df.column_names == COL_NAMES
 
         pd_df = df.to_pandas()
         assert list(pd_df.columns) == COL_NAMES
         assert len(pd_df) == len(valid_data)
 
 
+def test_create_dataframe_multiple_parquets(valid_data: list[dict[str, float]]) -> None:
+    with tempfile.NamedTemporaryFile("w") as f1, tempfile.NamedTemporaryFile("w") as f2:
+        for f in (f1, f2):
+            table = pa.Table.from_pydict({col: [d[col] for d in valid_data] for col in COL_NAMES})
+            papq.write_table(table, f.name)
+            f.flush()
+
+        df = daft.read_parquet([f1.name, f2.name])
+        assert df.column_names == COL_NAMES
+
+        pd_df = df.to_pandas()
+        assert list(pd_df.columns) == COL_NAMES
+        assert len(pd_df) == (len(valid_data) * 2)
+
+
 @pytest.mark.skipif(get_context().runner_config.name not in {"py"}, reason="requires PyRunner to be in use")
 def test_create_dataframe_parquet_custom_fs(valid_data: list[dict[str, float]]) -> None:
     with tempfile.NamedTemporaryFile("w") as f:
         table = pa.Table.from_pydict({col: [d[col] for d in valid_data] for col in COL_NAMES})
         papq.write_table(table, f.name)
         f.flush()
```

### Comparing `getdaft-0.1.7/tests/dataframe/test_distinct.py` & `getdaft-0.1.8/tests/dataframe/test_distinct.py`

 * *Files identical despite different names*

### Comparing `getdaft-0.1.7/tests/dataframe/test_explode.py` & `getdaft-0.1.8/tests/dataframe/test_explode.py`

 * *Files identical despite different names*

### Comparing `getdaft-0.1.7/tests/dataframe/test_filter.py` & `getdaft-0.1.8/tests/dataframe/test_filter.py`

 * *Files identical despite different names*

### Comparing `getdaft-0.1.7/tests/dataframe/test_getitem.py` & `getdaft-0.1.8/tests/dataframe/test_getitem.py`

 * *Files identical despite different names*

### Comparing `getdaft-0.1.7/tests/dataframe/test_iter.py` & `getdaft-0.1.8/tests/dataframe/test_iter.py`

 * *Files identical despite different names*

### Comparing `getdaft-0.1.7/tests/dataframe/test_joins.py` & `getdaft-0.1.8/tests/dataframe/test_joins.py`

 * *Files identical despite different names*

### Comparing `getdaft-0.1.7/tests/dataframe/test_logical_type.py` & `getdaft-0.1.8/tests/dataframe/test_logical_type.py`

 * *Files identical despite different names*

### Comparing `getdaft-0.1.7/tests/dataframe/test_repr.py` & `getdaft-0.1.8/tests/dataframe/test_repr.py`

 * *Files 21% similar despite different names*

```diff
@@ -8,14 +8,15 @@
 
 import daft
 
 ROW_DIVIDER_REGEX = re.compile(r"\+-+\+")
 SHOWING_N_ROWS_REGEX = re.compile(r".*\(Showing first (\d+) of (\d+) rows\).*")
 UNMATERIALIZED_REGEX = re.compile(r".*\(No data to display: Dataframe not materialized\).*")
 MATERIALIZED_NO_ROWS_REGEX = re.compile(r".*\(No data to display: Materialized dataframe has no rows\).*")
+TD_STYLE = 'style="text-align:left; max-width:192px; max-height:64px; overflow:auto"'
 
 
 def parse_str_table(
     table: str, expected_user_msg_regex: re.Pattern = SHOWING_N_ROWS_REGEX
 ) -> dict[str, tuple[str, list[str]]]:
     def _split_table_row(row: str) -> list[str]:
         return [cell.strip() for cell in row.split("|")[1:-1]]
@@ -86,15 +87,15 @@
     expected_data = {"A": ("Int64", []), "B": ("Utf8", [])}
 
     assert parse_str_table(df.__repr__(), expected_user_msg_regex=UNMATERIALIZED_REGEX) == expected_data
     assert (
         df._repr_html_()
         == """<div>
 <table class="dataframe">
-<thead><tr><th>A<br />Int64</th><th>B<br />Utf8</th></tr></thead>
+<thead><tr><th style="text-wrap: nowrap; max-width:192px; overflow:auto">A<br />Int64</th><th style="text-wrap: nowrap; max-width:192px; overflow:auto">B<br />Utf8</th></tr></thead>
 </table>
 <small>(No data to display: Dataframe not materialized)</small>
 </div>"""
     )
 
     df.collect()
     expected_data = {
@@ -108,15 +109,15 @@
         ),
     }
     assert parse_str_table(df.__repr__(), expected_user_msg_regex=MATERIALIZED_NO_ROWS_REGEX) == expected_data
     assert (
         df._repr_html_()
         == """<div>
 <table class="dataframe">
-<thead><tr><th>A<br />Int64</th><th>B<br />Utf8</th></tr></thead>
+<thead><tr><th style="text-wrap: nowrap; max-width:192px; overflow:auto">A<br />Int64</th><th style="text-wrap: nowrap; max-width:192px; overflow:auto">B<br />Utf8</th></tr></thead>
 <tbody>
 </tbody>
 </table>
 <small>(No data to display: Materialized dataframe has no rows)</small>
 </div>"""
     )
 
@@ -127,15 +128,15 @@
 
     expected_data = {"A2": ("Int64", []), "B": ("Utf8", [])}
     assert parse_str_table(df.__repr__(), expected_user_msg_regex=UNMATERIALIZED_REGEX) == expected_data
     assert (
         df._repr_html_()
         == """<div>
 <table class="dataframe">
-<thead><tr><th>A2<br />Int64</th><th>B<br />Utf8</th></tr></thead>
+<thead><tr><th style="text-wrap: nowrap; max-width:192px; overflow:auto">A2<br />Int64</th><th style="text-wrap: nowrap; max-width:192px; overflow:auto">B<br />Utf8</th></tr></thead>
 </table>
 <small>(No data to display: Dataframe not materialized)</small>
 </div>"""
     )
 
     df.collect()
 
@@ -151,21 +152,21 @@
     }
     expected_data_html = {
         **expected_data,
     }
     assert parse_str_table(df.__repr__()) == expected_data
     assert (
         df._repr_html_()
-        == """<div>
+        == f"""<div>
 <table class="dataframe">
-<thead><tr><th>A2<br />Int64</th><th>B<br />Utf8</th></tr></thead>
+<thead><tr><th style="text-wrap: nowrap; max-width:192px; overflow:auto">A2<br />Int64</th><th style="text-wrap: nowrap; max-width:192px; overflow:auto">B<br />Utf8</th></tr></thead>
 <tbody>
-<tr><td>1</td><td>a</td></tr>
-<tr><td>2</td><td>b</td></tr>
-<tr><td>3</td><td>c</td></tr>
+<tr><td><div {TD_STYLE}>1</div></td><td><div {TD_STYLE}>a</div></td></tr>
+<tr><td><div {TD_STYLE}>2</div></td><td><div {TD_STYLE}>b</div></td></tr>
+<tr><td><div {TD_STYLE}>3</div></td><td><div {TD_STYLE}>c</div></td></tr>
 </tbody>
 </table>
 <small>(Showing first 3 of 3 rows)</small>
 </div>"""
     )
 
 
@@ -173,15 +174,15 @@
     df = daft.from_pydict({"A": [f"<div>body{i}</div>" for i in range(3)]})
     df.collect()
 
     non_html_table = df.__repr__()
     html_table = df._repr_html_()
     for i in range(3):
         assert f"<div>body{i}</div>" in non_html_table
-        assert f"<tr><td>&lt;div&gt;body{i}&lt;/div&gt;</td></tr>" in html_table
+        assert f"<tr><td><div {TD_STYLE}>&lt;div&gt;body{i}&lt;/div&gt;</div></td></tr>" in html_table
 
 
 class MyObj:
     def __repr__(self) -> str:
         return "myobj-custom-repr"
 
 
@@ -226,8 +227,8 @@
     assert "myobj-custom-repr" in html_repr
 
     # Assert that PIL viz hook correctly triggers in html repr
     assert 'alt="<PIL.Image.Image image mode=L size=3x3' in html_repr
     assert '<img style="max-height:128px;width:auto" src="data:image/png;base64,' in html_repr
 
     # Assert that numpy array viz hook correctly triggers in html repr
-    assert "<td>&ltnp.ndarray<br>shape=(3, 3)<br>dtype=float64&gt</td><td>" in html_repr
+    assert f"<td><div {TD_STYLE}>&ltnp.ndarray<br>shape=(3, 3)<br>dtype=float64&gt</div></td><td>" in html_repr
```

### Comparing `getdaft-0.1.7/tests/dataframe/test_select.py` & `getdaft-0.1.8/tests/dataframe/test_select.py`

 * *Files identical despite different names*

### Comparing `getdaft-0.1.7/tests/dataframe/test_show.py` & `getdaft-0.1.8/tests/dataframe/test_show.py`

 * *Files identical despite different names*

### Comparing `getdaft-0.1.7/tests/dataframe/test_sort.py` & `getdaft-0.1.8/tests/dataframe/test_sort.py`

 * *Files identical despite different names*

### Comparing `getdaft-0.1.7/tests/dataframe/test_to_integrations.py` & `getdaft-0.1.8/tests/dataframe/test_to_integrations.py`

 * *Files identical despite different names*

### Comparing `getdaft-0.1.7/tests/dataframe/test_with_column.py` & `getdaft-0.1.8/tests/dataframe/test_with_column.py`

 * *Files identical despite different names*

### Comparing `getdaft-0.1.7/tests/expressions/test_apply.py` & `getdaft-0.1.8/tests/expressions/test_apply.py`

 * *Files identical despite different names*

### Comparing `getdaft-0.1.7/tests/expressions/test_expressions.py` & `getdaft-0.1.8/tests/expressions/test_expressions.py`

 * *Files identical despite different names*

### Comparing `getdaft-0.1.7/tests/expressions/test_expressions_projection.py` & `getdaft-0.1.8/tests/expressions/test_expressions_projection.py`

 * *Files identical despite different names*

### Comparing `getdaft-0.1.7/tests/expressions/test_udf.py` & `getdaft-0.1.8/tests/expressions/test_udf.py`

 * *Files identical despite different names*

### Comparing `getdaft-0.1.7/tests/expressions/typing/conftest.py` & `getdaft-0.1.8/tests/expressions/typing/conftest.py`

 * *Files identical despite different names*

### Comparing `getdaft-0.1.7/tests/expressions/typing/test_aggs.py` & `getdaft-0.1.8/tests/expressions/typing/test_aggs.py`

 * *Files identical despite different names*

### Comparing `getdaft-0.1.7/tests/expressions/typing/test_arithmetic.py` & `getdaft-0.1.8/tests/expressions/typing/test_arithmetic.py`

 * *Files identical despite different names*

### Comparing `getdaft-0.1.7/tests/expressions/typing/test_compare.py` & `getdaft-0.1.8/tests/expressions/typing/test_compare.py`

 * *Files identical despite different names*

### Comparing `getdaft-0.1.7/tests/expressions/typing/test_dt.py` & `getdaft-0.1.8/tests/expressions/typing/test_dt.py`

 * *Files identical despite different names*

### Comparing `getdaft-0.1.7/tests/expressions/typing/test_float.py` & `getdaft-0.1.8/tests/expressions/typing/test_float.py`

 * *Files identical despite different names*

### Comparing `getdaft-0.1.7/tests/expressions/typing/test_if_else.py` & `getdaft-0.1.8/tests/expressions/typing/test_if_else.py`

 * *Files identical despite different names*

### Comparing `getdaft-0.1.7/tests/expressions/typing/test_logical.py` & `getdaft-0.1.8/tests/expressions/typing/test_logical.py`

 * *Files identical despite different names*

### Comparing `getdaft-0.1.7/tests/expressions/typing/test_str.py` & `getdaft-0.1.8/tests/expressions/typing/test_str.py`

 * *Files identical despite different names*

### Comparing `getdaft-0.1.7/tests/integration/test_tpch.py` & `getdaft-0.1.8/tests/integration/test_tpch.py`

 * *Files identical despite different names*

### Comparing `getdaft-0.1.7/tests/optimizer/conftest.py` & `getdaft-0.1.8/tests/optimizer/conftest.py`

 * *Files identical despite different names*

### Comparing `getdaft-0.1.7/tests/optimizer/test_drop_projections.py` & `getdaft-0.1.8/tests/optimizer/test_drop_projections.py`

 * *Files identical despite different names*

### Comparing `getdaft-0.1.7/tests/optimizer/test_drop_repartition.py` & `getdaft-0.1.8/tests/optimizer/test_drop_repartition.py`

 * *Files identical despite different names*

### Comparing `getdaft-0.1.7/tests/optimizer/test_fold_projections.py` & `getdaft-0.1.8/tests/optimizer/test_fold_projections.py`

 * *Files identical despite different names*

### Comparing `getdaft-0.1.7/tests/optimizer/test_prune_columns.py` & `getdaft-0.1.8/tests/optimizer/test_prune_columns.py`

 * *Files identical despite different names*

### Comparing `getdaft-0.1.7/tests/optimizer/test_pushdown_clauses_into_scan.py` & `getdaft-0.1.8/tests/optimizer/test_pushdown_clauses_into_scan.py`

 * *Files identical despite different names*

### Comparing `getdaft-0.1.7/tests/optimizer/test_pushdown_limit.py` & `getdaft-0.1.8/tests/optimizer/test_pushdown_limit.py`

 * *Files identical despite different names*

### Comparing `getdaft-0.1.7/tests/optimizer/test_pushdown_predicates.py` & `getdaft-0.1.8/tests/optimizer/test_pushdown_predicates.py`

 * *Files identical despite different names*

### Comparing `getdaft-0.1.7/tests/property_based_testing/strategies.py` & `getdaft-0.1.8/tests/property_based_testing/strategies.py`

 * *Files identical despite different names*

### Comparing `getdaft-0.1.7/tests/property_based_testing/test_sort.py` & `getdaft-0.1.8/tests/property_based_testing/test_sort.py`

 * *Files identical despite different names*

### Comparing `getdaft-0.1.7/tests/ray/test_dask.py` & `getdaft-0.1.8/tests/ray/test_dask.py`

 * *Files identical despite different names*

### Comparing `getdaft-0.1.7/tests/ray/test_datasets.py` & `getdaft-0.1.8/tests/ray/test_datasets.py`

 * *Files identical despite different names*

### Comparing `getdaft-0.1.7/tests/series/test_arithmetic.py` & `getdaft-0.1.8/tests/series/test_arithmetic.py`

 * *Files identical despite different names*

### Comparing `getdaft-0.1.7/tests/series/test_cast.py` & `getdaft-0.1.8/tests/series/test_cast.py`

 * *Files identical despite different names*

### Comparing `getdaft-0.1.7/tests/series/test_comparisons.py` & `getdaft-0.1.8/tests/series/test_comparisons.py`

 * *Files identical despite different names*

### Comparing `getdaft-0.1.7/tests/series/test_concat.py` & `getdaft-0.1.8/tests/series/test_concat.py`

 * *Files identical despite different names*

### Comparing `getdaft-0.1.7/tests/series/test_embedding.py` & `getdaft-0.1.8/tests/series/test_embedding.py`

 * *Files identical despite different names*

### Comparing `getdaft-0.1.7/tests/series/test_filter.py` & `getdaft-0.1.8/tests/series/test_filter.py`

 * *Files identical despite different names*

### Comparing `getdaft-0.1.7/tests/series/test_float.py` & `getdaft-0.1.8/tests/series/test_float.py`

 * *Files identical despite different names*

### Comparing `getdaft-0.1.7/tests/series/test_hash.py` & `getdaft-0.1.8/tests/series/test_hash.py`

 * *Files identical despite different names*

### Comparing `getdaft-0.1.7/tests/series/test_if_else.py` & `getdaft-0.1.8/tests/series/test_if_else.py`

 * *Files identical despite different names*

### Comparing `getdaft-0.1.7/tests/series/test_image.py` & `getdaft-0.1.8/tests/series/test_image.py`

 * *Files identical despite different names*

### Comparing `getdaft-0.1.7/tests/series/test_numeric_ops.py` & `getdaft-0.1.8/tests/series/test_numeric_ops.py`

 * *Files identical despite different names*

### Comparing `getdaft-0.1.7/tests/series/test_series.py` & `getdaft-0.1.8/tests/series/test_series.py`

 * *Files identical despite different names*

### Comparing `getdaft-0.1.7/tests/series/test_size_bytes.py` & `getdaft-0.1.8/tests/series/test_size_bytes.py`

 * *Files identical despite different names*

### Comparing `getdaft-0.1.7/tests/series/test_slice.py` & `getdaft-0.1.8/tests/series/test_slice.py`

 * *Files identical despite different names*

### Comparing `getdaft-0.1.7/tests/series/test_sort.py` & `getdaft-0.1.8/tests/series/test_sort.py`

 * *Files identical despite different names*

### Comparing `getdaft-0.1.7/tests/series/test_take.py` & `getdaft-0.1.8/tests/series/test_take.py`

 * *Files identical despite different names*

### Comparing `getdaft-0.1.7/tests/series/test_temporal_ops.py` & `getdaft-0.1.8/tests/series/test_temporal_ops.py`

 * *Files identical despite different names*

### Comparing `getdaft-0.1.7/tests/series/test_utf8_ops.py` & `getdaft-0.1.8/tests/series/test_utf8_ops.py`

 * *Files identical despite different names*

### Comparing `getdaft-0.1.7/tests/table/__init__.py` & `getdaft-0.1.8/tests/table/__init__.py`

 * *Files identical despite different names*

### Comparing `getdaft-0.1.7/tests/table/list/test_list_join.py` & `getdaft-0.1.8/tests/table/list/test_list_join.py`

 * *Files identical despite different names*

### Comparing `getdaft-0.1.7/tests/table/table_io/test_csv.py` & `getdaft-0.1.8/tests/table/table_io/test_csv.py`

 * *Files identical despite different names*

### Comparing `getdaft-0.1.7/tests/table/table_io/test_json.py` & `getdaft-0.1.8/tests/table/table_io/test_json.py`

 * *Files identical despite different names*

### Comparing `getdaft-0.1.7/tests/table/table_io/test_parquet.py` & `getdaft-0.1.8/tests/table/table_io/test_parquet.py`

 * *Files identical despite different names*

### Comparing `getdaft-0.1.7/tests/table/table_io/test_read_time_cast.py` & `getdaft-0.1.8/tests/table/table_io/test_read_time_cast.py`

 * *Files identical despite different names*

### Comparing `getdaft-0.1.7/tests/table/test_blackbox_kernels.py` & `getdaft-0.1.8/tests/table/test_blackbox_kernels.py`

 * *Files identical despite different names*

### Comparing `getdaft-0.1.7/tests/table/test_concat.py` & `getdaft-0.1.8/tests/table/test_concat.py`

 * *Files identical despite different names*

### Comparing `getdaft-0.1.7/tests/table/test_eval.py` & `getdaft-0.1.8/tests/table/test_eval.py`

 * *Files identical despite different names*

### Comparing `getdaft-0.1.7/tests/table/test_explodes.py` & `getdaft-0.1.8/tests/table/test_explodes.py`

 * *Files identical despite different names*

### Comparing `getdaft-0.1.7/tests/table/test_filter.py` & `getdaft-0.1.8/tests/table/test_filter.py`

 * *Files identical despite different names*

### Comparing `getdaft-0.1.7/tests/table/test_from_py.py` & `getdaft-0.1.8/tests/table/test_from_py.py`

 * *Files identical despite different names*

### Comparing `getdaft-0.1.7/tests/table/test_head.py` & `getdaft-0.1.8/tests/table/test_head.py`

 * *Files identical despite different names*

### Comparing `getdaft-0.1.7/tests/table/test_joins.py` & `getdaft-0.1.8/tests/table/test_joins.py`

 * *Files identical despite different names*

### Comparing `getdaft-0.1.7/tests/table/test_partitioning.py` & `getdaft-0.1.8/tests/table/test_partitioning.py`

 * *Files identical despite different names*

### Comparing `getdaft-0.1.7/tests/table/test_size_bytes.py` & `getdaft-0.1.8/tests/table/test_size_bytes.py`

 * *Files identical despite different names*

### Comparing `getdaft-0.1.7/tests/table/test_sorting.py` & `getdaft-0.1.8/tests/table/test_sorting.py`

 * *Files identical despite different names*

### Comparing `getdaft-0.1.7/tests/table/test_table_aggs.py` & `getdaft-0.1.8/tests/table/test_table_aggs.py`

 * *Files identical despite different names*

### Comparing `getdaft-0.1.7/tests/table/test_take.py` & `getdaft-0.1.8/tests/table/test_take.py`

 * *Files identical despite different names*

### Comparing `getdaft-0.1.7/tests/table/utf8/test_compares.py` & `getdaft-0.1.8/tests/table/utf8/test_compares.py`

 * *Files identical despite different names*

### Comparing `getdaft-0.1.7/tests/test_analytics.py` & `getdaft-0.1.8/tests/test_analytics.py`

 * *Files identical despite different names*

### Comparing `getdaft-0.1.7/tests/test_datatypes.py` & `getdaft-0.1.8/tests/test_datatypes.py`

 * *Files identical despite different names*

### Comparing `getdaft-0.1.7/tests/test_schema.py` & `getdaft-0.1.8/tests/test_schema.py`

 * *Files identical despite different names*

### Comparing `getdaft-0.1.7/tests/udf_library/test_url_udfs.py` & `getdaft-0.1.8/tests/udf_library/test_url_udfs.py`

 * *Files identical despite different names*

### Comparing `getdaft-0.1.7/tests_legacy/test_resource_requests.py` & `getdaft-0.1.8/tests_legacy/test_resource_requests.py`

 * *Files identical despite different names*

### Comparing `getdaft-0.1.7/tools/patch_package_version.py` & `getdaft-0.1.8/tools/patch_package_version.py`

 * *Files identical despite different names*

### Comparing `getdaft-0.1.7/tools/wheels/_vendor/wheel/LICENSE.txt` & `getdaft-0.1.8/tools/wheels/_vendor/wheel/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `getdaft-0.1.7/tools/wheels/_vendor/wheel/cli/__init__.py` & `getdaft-0.1.8/tools/wheels/_vendor/wheel/cli/__init__.py`

 * *Files identical despite different names*

### Comparing `getdaft-0.1.7/tools/wheels/_vendor/wheel/cli/convert.py` & `getdaft-0.1.8/tools/wheels/_vendor/wheel/cli/convert.py`

 * *Files identical despite different names*

### Comparing `getdaft-0.1.7/tools/wheels/_vendor/wheel/cli/pack.py` & `getdaft-0.1.8/tools/wheels/_vendor/wheel/cli/pack.py`

 * *Files identical despite different names*

### Comparing `getdaft-0.1.7/tools/wheels/_vendor/wheel/cli/unpack.py` & `getdaft-0.1.8/tools/wheels/_vendor/wheel/cli/unpack.py`

 * *Files identical despite different names*

### Comparing `getdaft-0.1.7/tools/wheels/_vendor/wheel/pkginfo.py` & `getdaft-0.1.8/tools/wheels/_vendor/wheel/pkginfo.py`

 * *Files identical despite different names*

### Comparing `getdaft-0.1.7/tools/wheels/_vendor/wheel/util.py` & `getdaft-0.1.8/tools/wheels/_vendor/wheel/util.py`

 * *Files identical despite different names*

### Comparing `getdaft-0.1.7/tools/wheels/_vendor/wheel/wheelfile.py` & `getdaft-0.1.8/tools/wheels/_vendor/wheel/wheelfile.py`

 * *Files identical despite different names*

### Comparing `getdaft-0.1.7/tools/wheels/fix-and-copy-wheel.py` & `getdaft-0.1.8/tools/wheels/fix-and-copy-wheel.py`

 * *Files identical despite different names*

### Comparing `getdaft-0.1.7/tools/wheels/tmpdirs.py` & `getdaft-0.1.8/tools/wheels/tmpdirs.py`

 * *Files identical despite different names*

### Comparing `getdaft-0.1.7/tools/wheels/tools.py` & `getdaft-0.1.8/tools/wheels/tools.py`

 * *Files identical despite different names*

### Comparing `getdaft-0.1.7/tools/wheels/wheeltools.py` & `getdaft-0.1.8/tools/wheels/wheeltools.py`

 * *Files identical despite different names*

### Comparing `getdaft-0.1.7/tutorials/embeddings/daft_tutorial_embeddings_stackexchange.ipynb` & `getdaft-0.1.8/tutorials/embeddings/daft_tutorial_embeddings_stackexchange.ipynb`

 * *Files identical despite different names*

### Comparing `getdaft-0.1.7/tutorials/image_querying/top_n_red_color.ipynb` & `getdaft-0.1.8/tutorials/image_querying/top_n_red_color.ipynb`

 * *Files 13% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9837239337239337%*

 * *Differences: {"'cells'": "{3: {'attachments': OrderedDict()}, 4: {'attachments': OrderedDict()}, 6: "*

 * *            "{'attachments': OrderedDict()}, 9: {'attachments': OrderedDict()}, 11: "*

 * *            "{'attachments': OrderedDict()}, 12: {'attachments': OrderedDict()}, 14: "*

 * *            "{'attachments': OrderedDict()}, 16: {'attachments': OrderedDict()}, 18: "*

 * *            "{'attachments': OrderedDict()}, 20: {'attachments': OrderedDict()}, 21: "*

 * *            "{'attachments': OrderedDict()}, 24: {'attachments': OrderedDict […]*

```diff
@@ -34,26 +34,28 @@
             },
             "outputs": [],
             "source": [
                 "USE_RAY = False"
             ]
         },
         {
+            "attachments": {},
             "cell_type": "markdown",
             "id": "0a521469",
             "metadata": {},
             "source": [
                 "```{hint}\n",
                 "\u2728\u2728\u2728 **Run this notebook on Google Colab** \u2728\u2728\u2728\n",
                 "\n",
                 "You can [run this notebook yourself with Google Colab](https://colab.research.google.com/github/Eventual-Inc/Daft/blob/main/tutorials/image_querying/top_n_red_color.ipynb)!\n",
                 "```"
             ]
         },
         {
+            "attachments": {},
             "cell_type": "markdown",
             "id": "1684139f-5b59-4e24-89d3-7cd67ba6c103",
             "metadata": {},
             "source": [
                 "# Top N Most Red Images\n",
                 "\n",
                 "In this demo we will go through a simple example of using Daft to find the top N most red images out of the OpenImages dataset."
@@ -87,14 +89,15 @@
                 "        runtime_env={\"pip\": [\"getdaft\", \"pillow\", \"s3fs\"]},\n",
                 "    )\n",
                 "\n",
                 "    daft.context.set_runner_ray(address=RAY_CLUSTER_ADDRESS)\n"
             ]
         },
         {
+            "attachments": {},
             "cell_type": "markdown",
             "id": "77aeeb92-e654-468b-b01e-430dd72fe9ea",
             "metadata": {},
             "source": [
                 "## Constructing our DataFrame"
             ]
         },
@@ -127,14 +130,15 @@
             },
             "outputs": [],
             "source": [
                 "df"
             ]
         },
         {
+            "attachments": {},
             "cell_type": "markdown",
             "id": "db95e6d8-6b41-4dc1-91c9-5304c16a69df",
             "metadata": {},
             "source": [
                 "### Filtering Data"
             ]
         },
@@ -147,22 +151,24 @@
             },
             "outputs": [],
             "source": [
                 "df = df.where(df[\"size\"] < 300000)"
             ]
         },
         {
+            "attachments": {},
             "cell_type": "markdown",
             "id": "bf871b1b-d106-4063-8009-d2debfb790a8",
             "metadata": {},
             "source": [
                 "**Daft is LAZY**: this filtering doesn't run immediately, but rather queues operations up in a query plan."
             ]
         },
         {
+            "attachments": {},
             "cell_type": "markdown",
             "id": "9a15f564-7da8-4d58-b29c-3cbc39259e8a",
             "metadata": {},
             "source": [
                 "Now, let's define another filter with a lower bound for the image size"
             ]
         },
@@ -175,14 +181,15 @@
             },
             "outputs": [],
             "source": [
                 "df = df.where(df[\"size\"] > 200000)"
             ]
         },
         {
+            "attachments": {},
             "cell_type": "markdown",
             "id": "2267d8c2-c33e-45f9-a03d-7f87acaf057d",
             "metadata": {},
             "source": [
                 "If we look at the plan, there are now two enqueued `Filter` operations!"
             ]
         },
@@ -195,14 +202,15 @@
             },
             "outputs": [],
             "source": [
                 "df.explain()"
             ]
         },
         {
+            "attachments": {},
             "cell_type": "markdown",
             "id": "633ecf9b-ea58-44a6-b761-66ebb0bc4060",
             "metadata": {},
             "source": [
                 "Doing these two `Filter`s one after another is really inefficient since we have to pass through the data twice!\n",
                 "\n",
                 "Don't worry though - Daft's query optimizer will actually optimize this at runtime and merge the two `Filter` operations into one. You can view the optimized plan with `show_optimized=True`:"
@@ -217,14 +225,15 @@
             },
             "outputs": [],
             "source": [
                 "df.explain(show_optimized=True)"
             ]
         },
         {
+            "attachments": {},
             "cell_type": "markdown",
             "id": "c7fb87fa-7387-4b11-aa28-58de658c272e",
             "metadata": {},
             "source": [
                 "This is just one example of query optimization, and Daft does many other really important ones such as Predicate Pushdowns and Column Pruning to keep your execution plans running efficiently.\n",
                 "\n",
                 "Now we can **materialize** the filtered dataframe like so:"
@@ -241,22 +250,24 @@
             "source": [
                 "# Materializes the dataframe and shows first 10 rows\n",
                 "\n",
                 "df.collect()"
             ]
         },
         {
+            "attachments": {},
             "cell_type": "markdown",
             "id": "2dd014ad-8d14-40eb-883c-89cee2d4f9e6",
             "metadata": {},
             "source": [
                 "Note that calling `.collect()` **materializes** the data. It will execute the above plan and all the computed data will be materialized in memory as long as the `df` variable is valid. This means that any subsequent operation on `df` will read from this materialized data instead of computing the entire plan again."
             ]
         },
         {
+            "attachments": {},
             "cell_type": "markdown",
             "id": "539db555-f70f-4d7d-8c1f-8af7d3ba0213",
             "metadata": {},
             "source": [
                 "Let's prune the columns to just the \"filepath\" column, which is the only one we need at the moment:"
             ]
         },
@@ -284,14 +295,15 @@
                 "# Show doesn't materialize the data, but lets us peek at the first N rows\n",
                 "# produced by the current query plan\n",
                 "\n",
                 "df.show(5)"
             ]
         },
         {
+            "attachments": {},
             "cell_type": "markdown",
             "id": "0a256a14-9cae-4262-807e-8d4cd2e6f0d3",
             "metadata": {},
             "source": [
                 "### Working with Complex Data\n",
                 "\n",
                 "Now let's do some data manipulation, starting with some simple ones (URLs) and finally images!"
@@ -320,42 +332,32 @@
             "outputs": [],
             "source": [
                 "# Materialize the dataframe, so that we don't have to hit S3 again for subsequent operations\n",
                 "df.collect()"
             ]
         },
         {
+            "attachments": {},
             "cell_type": "markdown",
             "id": "2c2f7980-0e8e-40ab-b02b-5f90d0fb3982",
             "metadata": {},
             "source": [
-                "To load the raw bytes we're downloading from the URL into a `PIL` image, we can define a simple function and run it on our column:"
+                "To decode the raw bytes we're downloading from the URL into an Image, we can simply use Daft's `.image.decode()` expression:"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
             "id": "6851bf9c-478b-4613-a9f2-edbb3cc81f48",
             "metadata": {
                 "tags": []
             },
             "outputs": [],
             "source": [
-                "from daft import udf, DataType\n",
-                "\n",
-                "import io\n",
-                "import PIL\n",
-                "\n",
-                "@udf(return_dtype=DataType.python())\n",
-                "def bytes_to_pil(bytes_column):\n",
-                "    return [\n",
-                "        PIL.Image.open(io.BytesIO(data)).resize((256, 256)) for data in bytes_column.to_pylist()\n",
-                "    ]\n",
-                "\n",
-                "df = df.with_column(\"image\", bytes_to_pil(df[\"image\"]))"
+                "df = df.with_column(\"image\", df[\"image\"].image.decode())"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
             "id": "ec2c009a-e1ba-429d-8632-9724cc51bb02",
             "metadata": {
@@ -363,43 +365,56 @@
             },
             "outputs": [],
             "source": [
                 "df.show(5)"
             ]
         },
         {
+            "attachments": {},
+            "cell_type": "markdown",
+            "id": "74dd028b",
+            "metadata": {},
+            "source": [
+                "Sometimes you may need to run your own custom Python function. We can do this with the `.apply` Daft expression.\n",
+                "\n",
+                "Let's run a custom `magic_red_detector` function, which will detect red pixels in our images and present us with a mask!"
+            ]
+        },
+        {
             "cell_type": "code",
             "execution_count": null,
             "id": "82afc506-cf6f-4e9a-b10e-7c7f1aed6b66",
             "metadata": {
                 "tags": []
             },
             "outputs": [],
             "source": [
+                "import PIL\n",
                 "from PIL import ImageFilter\n",
                 "import numpy as np\n",
                 "\n",
                 "\n",
-                "def magic_red_detector(img: PIL.Image.Image) -> PIL.Image.Image:\n",
+                "def magic_red_detector(img: np.ndarray) -> PIL.Image.Image:\n",
                 "    \"\"\"Gets a new image which is a mask covering all 'red' areas in the image\"\"\"\n",
+                "    img = PIL.Image.fromarray(img)\n",
                 "    lower = np.array([245, 100, 100])\n",
                 "    upper = np.array([10,255,255])\n",
                 "    lower_hue, upper_hue = lower[0, np.newaxis, np.newaxis], upper[0, np.newaxis, np.newaxis]\n",
                 "    lower_saturation_intensity, upper_saturation_intensity = lower[1:, np.newaxis, np.newaxis], upper[1:, np.newaxis, np.newaxis]    \n",
                 "    hsv = img.convert('HSV')\n",
                 "    hsv = np.asarray(hsv).T\n",
                 "    mask = np.all((hsv[1:, ...] >= lower_saturation_intensity) & (hsv[1:, ...] <= upper_saturation_intensity), axis=0) & ((hsv[0, ...] >= lower_hue) | (hsv[0, ...] <= upper_hue))\n",
                 "    img = PIL.Image.fromarray(mask.T)\n",
                 "    img = img.filter(ImageFilter.ModeFilter(size=5))\n",
                 "    return img\n",
                 "\n",
                 "\n",
                 "df = df.with_column(\n",
                 "    \"red_mask\",\n",
-                "    df[\"image\"].apply(magic_red_detector, return_dtype=DataType.python()),\n",
+                "    df[\"image\"].apply(magic_red_detector, return_dtype=daft.DataType.python()),\n",
                 ")"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
             "id": "27c8bd0a-2638-467d-80c2-a759033d18b6",
@@ -409,14 +424,23 @@
             },
             "outputs": [],
             "source": [
                 "df.collect()"
             ]
         },
         {
+            "attachments": {},
+            "cell_type": "markdown",
+            "id": "c39b8793",
+            "metadata": {},
+            "source": [
+                "Now to determine how \"red\" an image is, we can simply sum up the number of pixels in the `red_mask` column!"
+            ]
+        },
+        {
             "cell_type": "code",
             "execution_count": null,
             "id": "c9b940fd-6645-4034-9282-c46792c819ed",
             "metadata": {
                 "tags": []
             },
             "outputs": [],
@@ -425,15 +449,15 @@
                 "\n",
                 "def sum_mask(mask: PIL.Image.Image) -> int:\n",
                 "    val = np.asarray(mask).sum()\n",
                 "    return int(val)\n",
                 "\n",
                 "df = df.with_column(\n",
                 "    \"num_pixels_red\",\n",
-                "    df[\"red_mask\"].apply(sum_mask, return_dtype=DataType.int64()),\n",
+                "    df[\"red_mask\"].apply(sum_mask, return_dtype=daft.DataType.int64()),\n",
                 ")"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
             "id": "7bddede4-bd05-4611-ab9e-74e272397f29",
```

### Comparing `getdaft-0.1.7/tutorials/mnist.ipynb` & `getdaft-0.1.8/tutorials/mnist.ipynb`

 * *Files identical despite different names*

### Comparing `getdaft-0.1.7/tutorials/text_to_image/text_to_image_generation.ipynb` & `getdaft-0.1.8/tutorials/text_to_image/text_to_image_generation.ipynb`

 * *Files 6% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9888157894736842%*

 * *Differences: {"'cells'": "{3: {'attachments': OrderedDict()}, 4: {'attachments': OrderedDict()}, 5: "*

 * *            "{'attachments': OrderedDict()}, 6: {'source': {delete: [1]}}, 7: {'attachments': "*

 * *            "OrderedDict()}, 10: {'attachments': OrderedDict()}, 11: {'source': {insert: [(6, '    "*

 * *            'parquet_df["URL"].url.download().image.decode(),\\n\')], delete: [12, 11, 10, 9, 2, '*

 * *            "1, 0]}}, 12: {'source': {delete: [1, 0]}}, 13: {'attachments': OrderedDict()}, 14: "*

 * *            "{'attachments':  […]*

```diff
@@ -44,26 +44,28 @@
                 "# Flip this flag if you want to see the performance of running on CPU vs GPU\n",
                 "USE_GPU = False if CI else True\n",
                 "\n",
                 "PARQUET_PATH = \"https://huggingface.co/datasets/ChristophSchuhmann/improved_aesthetics_6.5plus/resolve/main/data/train-00000-of-00001-6f24a7497df494ae.parquet\""
             ]
         },
         {
+            "attachments": {},
             "cell_type": "markdown",
             "id": "d5a31f06",
             "metadata": {},
             "source": [
                 "```{hint}\n",
                 "\u2728\u2728\u2728 **Run this notebook on Google Colab** \u2728\u2728\u2728\n",
                 "\n",
                 "You can [run this notebook yourself with Google Colab](https://colab.research.google.com/github/Eventual-Inc/Daft/blob/main/tutorials/text_to_image/text_to_image_generation.ipynb)!\n",
                 "```"
             ]
         },
         {
+            "attachments": {},
             "cell_type": "markdown",
             "id": "78db424a-96b5-46f3-bd32-484f5c6b92a3",
             "metadata": {
                 "id": "78db424a-96b5-46f3-bd32-484f5c6b92a3"
             },
             "source": [
                 "# Generating Images from Text with DALL-E\n",
@@ -74,14 +76,15 @@
                 "\n",
                 "1. You will need access to a GPU. If you are on Google Colab, you may switch to a GPU runtime by going to the menu `Runtime -> Change runtime type -> Hardware accelerator -> GPU -> Save`.\n",
                 "\n",
                 "Let's get started!"
             ]
         },
         {
+            "attachments": {},
             "cell_type": "markdown",
             "id": "4da65a96-e4fe-4795-92d0-a5e631b58e33",
             "metadata": {
                 "id": "4da65a96-e4fe-4795-92d0-a5e631b58e33"
             },
             "source": [
                 "## Setting Up\n",
@@ -96,21 +99,21 @@
             "metadata": {
                 "id": "806451f8-68af-462a-af7b-ff5480425a3a",
                 "tags": []
             },
             "outputs": [],
             "source": [
                 "import daft\n",
-                "from daft import col, udf, DataType\n",
                 "daft.context.set_runner_py(use_thread_pool=False)\n",
                 "\n",
                 "parquet_df = daft.read_parquet(PARQUET_PATH)"
             ]
         },
         {
+            "attachments": {},
             "cell_type": "markdown",
             "id": "a1e20f90",
             "metadata": {},
             "source": [
                 "Let's go ahead and `.collect()` this DataFrame. This will download the Parquet file and materialize the data in memory so that all our subsequent operations will be cached!"
             ]
         },
@@ -142,14 +145,15 @@
             },
             "outputs": [],
             "source": [
                 "parquet_df = parquet_df.select(parquet_df[\"URL\"], parquet_df[\"TEXT\"], parquet_df[\"AESTHETIC_SCORE\"])"
             ]
         },
         {
+            "attachments": {},
             "cell_type": "markdown",
             "id": "f28047df-bf05-47df-b4d4-3507a8f7d2ac",
             "metadata": {
                 "id": "f28047df-bf05-47df-b4d4-3507a8f7d2ac"
             },
             "source": [
                 "## Downloading Images\n",
@@ -165,27 +169,21 @@
             "id": "f1e5cd84-4526-4a91-9fd5-f4e78f35965d",
             "metadata": {
                 "id": "f1e5cd84-4526-4a91-9fd5-f4e78f35965d",
                 "tags": []
             },
             "outputs": [],
             "source": [
-                "import io\n",
-                "import PIL.Image\n",
-                "\n",
                 "# Filter for images with longer descriptions\n",
                 "parquet_df_with_long_strings = parquet_df.where(parquet_df[\"TEXT\"].str.length() > 50)\n",
                 "\n",
                 "# Download images\n",
                 "images_df = parquet_df_with_long_strings.with_column(\n",
                 "    \"image\",\n",
-                "    parquet_df[\"URL\"].url.download().apply(\n",
-                "        lambda data: PIL.Image.open(io.BytesIO(data)) if data is not None else None,\n",
-                "        return_dtype=DataType.python(),\n",
-                "    ),\n",
+                "    parquet_df[\"URL\"].url.download().image.decode(),\n",
                 ")"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
             "id": "c1361728-8b1a-4e6e-9632-ddd17cad948b",
@@ -196,28 +194,28 @@
                 },
                 "id": "c1361728-8b1a-4e6e-9632-ddd17cad948b",
                 "outputId": "1c2ce3a4-63a1-4f77-ce2e-e3ecea2a3e1f",
                 "tags": []
             },
             "outputs": [],
             "source": [
-                "%%time\n",
-                "\n",
                 "images_df.show(5)"
             ]
         },
         {
+            "attachments": {},
             "cell_type": "markdown",
             "id": "6e6f59ee",
             "metadata": {},
             "source": [
                 "Great! Now we have a pretty good idea of what our dataset looks like."
             ]
         },
         {
+            "attachments": {},
             "cell_type": "markdown",
             "id": "gCTmONUl81Vw",
             "metadata": {
                 "id": "gCTmONUl81Vw"
             },
             "source": [
                 "# Running the Mini DALL-E model on a GPU using Daft UDFs\n",
@@ -238,15 +236,15 @@
             "source": [
                 "import torch\n",
                 "from min_dalle import MinDalle\n",
                 "\n",
                 "from daft.resource_request import ResourceRequest\n",
                 "\n",
                 "\n",
-                "@udf(return_dtype=DataType.python())\n",
+                "@daft.udf(return_dtype=daft.DataType.python())\n",
                 "class GenerateImageFromText:\n",
                 "    def __init__(self):\n",
                 "        self.model = MinDalle(\n",
                 "            models_root='./pretrained',\n",
                 "            dtype=torch.float32,\n",
                 "            # Tell the min-dalle library to load model on GPU or GPU\n",
                 "            device=\"cuda\" if USE_GPU else \"cpu\",\n",
```

### Comparing `getdaft-0.1.7/tutorials/text_to_image/using_cloud_with_ray.ipynb` & `getdaft-0.1.8/tutorials/text_to_image/using_cloud_with_ray.ipynb`

 * *Files identical despite different names*

### Comparing `getdaft-0.1.7/Cargo.lock` & `getdaft-0.1.8/Cargo.lock`

 * *Files 1% similar despite different names*

```diff
@@ -693,15 +693,15 @@
 checksum = "2b2466559f260f48ad25fe6317b3c8dac77b5bdb5763ac7d9d6103530663bc90"
 dependencies = [
  "memchr",
 ]
 
 [[package]]
 name = "daft"
-version = "0.1.7"
+version = "0.1.8"
 dependencies = [
  "daft-core",
  "daft-dsl",
  "daft-io",
  "daft-table",
  "pyo3",
  "pyo3-log",
@@ -754,25 +754,29 @@
 name = "daft-io"
 version = "0.1.0"
 dependencies = [
  "async-trait",
  "aws-config",
  "aws-credential-types",
  "aws-sdk-s3",
+ "aws-sig-auth",
+ "aws-sigv4",
  "bytes",
  "common-error",
  "daft-core",
  "futures",
  "lazy_static",
  "log",
+ "md5",
  "pyo3",
  "pyo3-log",
  "reqwest",
  "serde",
  "snafu",
+ "tempfile",
  "tokio",
  "url",
 ]
 
 [[package]]
 name = "daft-table"
 version = "0.1.0"
@@ -1460,14 +1464,20 @@
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "6365506850d44bff6e2fbcb5176cf63650e48bd45ef2fe2665ae1570e0f4b9ca"
 dependencies = [
  "digest",
 ]
 
 [[package]]
+name = "md5"
+version = "0.7.0"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "490cc448043f947bae3cbee9c203358d62dbee0db12107a74be5c30ccfd09771"
+
+[[package]]
 name = "memchr"
 version = "2.5.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "2dffe52ecf27772e601905b7522cb4ef790d2cc203488bbd0e2fe85fcb74566d"
 
 [[package]]
 name = "memoffset"
@@ -2178,17 +2188,17 @@
  "proc-macro2",
  "quote",
  "syn 2.0.18",
 ]
 
 [[package]]
 name = "serde_json"
-version = "1.0.97"
+version = "1.0.99"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "bdf3bf93142acad5821c99197022e170842cdbc1c30482b98750c688c640842a"
+checksum = "46266871c240a00b8f503b877622fe33430b3c7d963bdc0f2adc511e54a1eae3"
 dependencies = [
  "itoa",
  "ryu",
  "serde",
 ]
 
 [[package]]
@@ -2354,14 +2364,28 @@
 [[package]]
 name = "target-lexicon"
 version = "0.12.8"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "1b1c7f239eb94671427157bd93b3694320f3668d4e1eff08c7285366fd777fac"
 
 [[package]]
+name = "tempfile"
+version = "3.6.0"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "31c0432476357e58790aaa47a8efb0c5138f137343f3b5f23bd36a27e3b0a6d6"
+dependencies = [
+ "autocfg",
+ "cfg-if",
+ "fastrand",
+ "redox_syscall 0.3.5",
+ "rustix",
+ "windows-sys 0.48.0",
+]
+
+[[package]]
 name = "term"
 version = "0.7.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "c59df8ac95d96ff9bede18eb7300b0fda5e5d8d90960e76f8e14ae765eedbf1f"
 dependencies = [
  "dirs-next",
  "rustversion",
```

### Comparing `getdaft-0.1.7/PKG-INFO` & `getdaft-0.1.8/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,26 +1,26 @@
 Metadata-Version: 2.1
 Name: getdaft
-Version: 0.1.7
+Version: 0.1.8
 Requires-Dist: pyarrow >= 6.0.1
 Requires-Dist: fsspec[http]
 Requires-Dist: loguru
 Requires-Dist: psutil
 Requires-Dist: typing-extensions >= 4.0.0; python_version < '3.8'
 Requires-Dist: pickle5 >= 0.0.12; python_version < '3.8'
-Requires-Dist: pandas; extra == 'pandas'
 Requires-Dist: pydot; extra == 'viz'
 Requires-Dist: numpy; extra == 'numpy'
+Requires-Dist: pandas; extra == 'pandas'
 Requires-Dist: getdaft[aws, ray, pandas, numpy, viz]; extra == 'all'
 Requires-Dist: ray[data, default]>=2.0.0; extra == 'ray'
 Requires-Dist: packaging; extra == 'ray'
 Requires-Dist: s3fs; extra == 'aws'
-Provides-Extra: pandas
 Provides-Extra: viz
 Provides-Extra: numpy
+Provides-Extra: pandas
 Provides-Extra: all
 Provides-Extra: ray
 Provides-Extra: aws
 License-File: LICENSE
 Summary: A Distributed DataFrame library for large scale complex data processing.
 Author-email: Eventual Inc <daft@eventualcomputing.com>
 Maintainer-email: Sammy Sidhu <sammy@eventualcomputing.com>, Jay Chia <jay@eventualcomputing.com>
@@ -53,15 +53,15 @@
 * `License`_
 
 About Daft
 ----------
 
 The Daft dataframe is a table of data with rows and columns. Columns can contain any Python objects, which allows Daft to support rich complex data types such as images, audio, video and more.
 
-1. **Any Data**: Columns can contain any Python objects, which means that the Python libraries you already use for running machine learning or custom data processing will work natively with Daft!
+1. **Any Data**: Beyond the usual strings/numbers/dates, Daft columns can also hold complex multimodal data such as Images, Embeddings and Python objects. Ingestion and basic transformations of complex data is extremely easy and performant in Daft.
 2. **Notebook Computing**: Daft is built for the interactive developer experience on a notebook - intelligent caching/query optimizations accelerates your experimentation and data exploration.
 3. **Distributed Computing**: Rich complex formats such as images can quickly outgrow your local laptop's computational resources - Daft integrates natively with `Ray <https://www.ray.io>`_ for running dataframes on large clusters of machines with thousands of CPUs/GPUs.
 
 Getting Started
 ---------------
 
 Installation
@@ -72,40 +72,29 @@
 For more advanced installations (e.g. installing from source or with extra dependencies such as Ray and AWS utilities), please see our `Installation Guide <https://www.getdaft.io/projects/docs/en/latest/install.html>`_
 
 Quickstart
 ^^^^^^^^^^
 
   Check out our `10-minute quickstart <https://www.getdaft.io/projects/docs/en/latest/learn/10-min.html>`_!
 
-In this example, we load images from an AWS S3 bucket and run a simple function to generate thumbnails for each image:
+In this example, we load images from an AWS S3 bucket's URLs and resize each image in the dataframe:
 
 .. code:: python
 
     import daft as daft
 
-    import io
-    from PIL import Image
-
-    def get_thumbnail(img: Image.Image) -> Image.Image:
-        """Simple function to make an image thumbnail"""
-        imgcopy = img.copy()
-        imgcopy.thumbnail((48, 48))
-        return imgcopy
-
-    # Load a dataframe from files in an S3 bucket
+    # Load a dataframe from filepaths in an S3 bucket
     df = daft.from_glob_path("s3://daft-public-data/laion-sample-images/*")
 
-    # Get the AWS S3 url of each image
-    df = df.select(df["path"].alias("s3_url"))
-
-    # Download images and load as a PIL Image object
-    df = df.with_column("image", df["s3_url"].url.download().apply(lambda data: Image.open(io.BytesIO(data)), return_dtype=daft.DataType.python()))
+    # 1. Download column of image URLs as a column of bytes
+    # 2. Decode the column of bytes into a column of images
+    df = df.with_column("image", df["path"].url.download().image.decode())
 
-    # Generate thumbnails from images
-    df = df.with_column("thumbnail", df["image"].apply(get_thumbnail, return_dtype=daft.DataType.python()))
+    # Resize each image into 32x32
+    df = df.with_column("resized", df["image"].image.resize(32, 32))
 
     df.show(3)
 
 |Quickstart Image|
 
 
 Benchmarks
@@ -164,15 +153,15 @@
 Check out our `dataframe comparison page <https://www.getdaft.io/projects/docs/en/latest/dataframe_comparison.html>`_ for more details!
 
 License
 -------
 
 Daft has an Apache 2.0 license - please see the LICENSE file.
 
-.. |Quickstart Image| image:: https://user-images.githubusercontent.com/17691182/200086119-fb73037b-8b4e-414a-9060-a44122f0c290.png
+.. |Quickstart Image| image:: https://github.com/Eventual-Inc/Daft/assets/17691182/dea2f515-9739-4f3e-ac58-cd96d51e44a8
    :alt: Dataframe code to load a folder of images from AWS S3 and create thumbnails
    :height: 256
 
 .. |Benchmark Image| image:: https://github-production-user-asset-6210df.s3.amazonaws.com/2550285/243524430-338e427d-f049-40b3-b555-4059d6be7bfd.png
    :alt: Benchmarks for SF100 TPCH
 
 .. |Banner| image:: https://user-images.githubusercontent.com/17691182/190476440-28f29e87-8e3b-41c4-9c28-e112e595f558.png
```

