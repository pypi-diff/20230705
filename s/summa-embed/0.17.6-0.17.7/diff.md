# Comparing `tmp/summa_embed-0.17.6.tar.gz` & `tmp/summa_embed-0.17.7.tar.gz`

## Comparing `summa_embed-0.17.6.tar` & `summa_embed-0.17.7.tar`

### file list

```diff
@@ -1,125 +1,125 @@
--rw-r--r--   0        0        0     2767 1970-01-01 00:00:00.000000 summa_embed-0.17.6/local_dependencies/summa-server/Cargo.toml
--rw-r--r--   0      501       20       43 2023-07-03 15:18:18.000000 summa_embed-0.17.6/local_dependencies/summa-server/.cargo/config.toml
--rw-r--r--   0      501       20     1050 2023-07-03 15:18:18.000000 summa_embed-0.17.6/local_dependencies/summa-server/LICENSE
--rw-r--r--   0      501       20     2832 2023-07-03 15:18:18.000000 summa_embed-0.17.6/local_dependencies/summa-server/src/apis/consumer.rs
--rw-r--r--   0      501       20    13268 2023-07-03 15:18:18.000000 summa_embed-0.17.6/local_dependencies/summa-server/src/apis/index.rs
--rw-r--r--   0      501       20      105 2023-07-03 15:18:18.000000 summa_embed-0.17.6/local_dependencies/summa-server/src/apis/mod.rs
--rw-r--r--   0      501       20     2909 2023-07-03 15:18:18.000000 summa_embed-0.17.6/local_dependencies/summa-server/src/apis/reflection.rs
--rw-r--r--   0      501       20     1278 2023-07-03 15:18:18.000000 summa_embed-0.17.6/local_dependencies/summa-server/src/apis/search.rs
--rw-r--r--   0      501       20      783 2023-07-03 15:18:18.000000 summa_embed-0.17.6/local_dependencies/summa-server/src/bin/main.rs
--rw-r--r--   0      501       20     5305 2023-07-03 15:18:18.000000 summa_embed-0.17.6/local_dependencies/summa-server/src/components/consumer_manager.rs
--rw-r--r--   0      501       20      813 2023-07-03 15:18:18.000000 summa_embed-0.17.6/local_dependencies/summa-server/src/components/consumers/consumer_thread.rs
--rw-r--r--   0      501       20     1082 2023-07-03 15:18:18.000000 summa_embed-0.17.6/local_dependencies/summa-server/src/components/consumers/dummy.rs
--rw-r--r--   0      501       20    11633 2023-07-03 15:18:18.000000 summa_embed-0.17.6/local_dependencies/summa-server/src/components/consumers/kafka/consumer.rs
--rw-r--r--   0      501       20      270 2023-07-03 15:18:18.000000 summa_embed-0.17.6/local_dependencies/summa-server/src/components/consumers/kafka/mod.rs
--rw-r--r--   0      501       20      532 2023-07-03 15:18:18.000000 summa_embed-0.17.6/local_dependencies/summa-server/src/components/consumers/kafka/status.rs
--rw-r--r--   0      501       20      155 2023-07-03 15:18:18.000000 summa_embed-0.17.6/local_dependencies/summa-server/src/components/consumers/mod.rs
--rw-r--r--   0      501       20     3811 2023-07-03 15:18:18.000000 summa_embed-0.17.6/local_dependencies/summa-server/src/components/index_meter.rs
--rw-r--r--   0      501       20      258 2023-07-03 15:18:18.000000 summa_embed-0.17.6/local_dependencies/summa-server/src/components/mod.rs
--rw-r--r--   0      501       20      943 2023-07-03 15:18:18.000000 summa_embed-0.17.6/local_dependencies/summa-server/src/configs/api.rs
--rw-r--r--   0      501       20      919 2023-07-03 15:18:18.000000 summa_embed-0.17.6/local_dependencies/summa-server/src/configs/consumer.rs
--rw-r--r--   0      501       20      434 2023-07-03 15:18:18.000000 summa_embed-0.17.6/local_dependencies/summa-server/src/configs/metrics.rs
--rw-r--r--   0      501       20      116 2023-07-03 15:18:18.000000 summa_embed-0.17.6/local_dependencies/summa-server/src/configs/mod.rs
--rw-r--r--   0      501       20     4268 2023-07-03 15:18:18.000000 summa_embed-0.17.6/local_dependencies/summa-server/src/configs/server.rs
--rw-r--r--   0      501       20      991 2023-07-03 15:18:18.000000 summa_embed-0.17.6/local_dependencies/summa-server/src/configs/store.rs
--rw-r--r--   0      501       20     3459 2023-07-03 15:18:18.000000 summa_embed-0.17.6/local_dependencies/summa-server/src/errors.rs
--rw-r--r--   0      501       20     1427 2023-07-03 15:18:18.000000 summa_embed-0.17.6/local_dependencies/summa-server/src/lib.rs
--rw-r--r--   0      501       20     3681 2023-07-03 15:18:18.000000 summa_embed-0.17.6/local_dependencies/summa-server/src/logging.rs
--rw-r--r--   0      501       20    15704 2023-07-03 15:18:18.000000 summa_embed-0.17.6/local_dependencies/summa-server/src/server.rs
--rw-r--r--   0      501       20     8110 2023-07-03 15:18:18.000000 summa_embed-0.17.6/local_dependencies/summa-server/src/services/api.rs
--rw-r--r--   0      501       20    40154 2023-07-03 15:18:18.000000 summa_embed-0.17.6/local_dependencies/summa-server/src/services/index.rs
--rw-r--r--   0      501       20     5174 2023-07-03 15:18:18.000000 summa_embed-0.17.6/local_dependencies/summa-server/src/services/metrics.rs
--rw-r--r--   0      501       20      287 2023-07-03 15:18:18.000000 summa_embed-0.17.6/local_dependencies/summa-server/src/services/mod.rs
--rw-r--r--   0      501       20     2108 2023-07-03 15:18:18.000000 summa_embed-0.17.6/local_dependencies/summa-server/src/utils/mod.rs
--rw-r--r--   0      501       20      923 2023-07-03 15:18:18.000000 summa_embed-0.17.6/local_dependencies/summa-server/src/utils/thread_handler.rs
--rw-r--r--   0        0        0     2113 1970-01-01 00:00:00.000000 summa_embed-0.17.6/local_dependencies/summa-core/Cargo.toml
--rw-r--r--   0      501       20     1050 2023-07-03 15:18:18.000000 summa_embed-0.17.6/local_dependencies/summa-core/LICENSE
--rw-r--r--   0      501       20   370551 2023-07-03 15:18:18.000000 summa_embed-0.17.6/local_dependencies/summa-core/dictionaries/drugs.csv
--rw-r--r--   0      501       20       92 2023-07-03 15:18:18.000000 summa_embed-0.17.6/local_dependencies/summa-core/src/collectors/mod.rs
--rw-r--r--   0      501       20     7233 2023-07-03 15:18:18.000000 summa_embed-0.17.6/local_dependencies/summa-core/src/collectors/reservoir_sampling_collector.rs
--rw-r--r--   0      501       20     2107 2023-07-03 15:18:18.000000 summa_embed-0.17.6/local_dependencies/summa-core/src/components/custom_serializer.rs
--rw-r--r--   0      501       20     5492 2023-07-03 15:18:18.000000 summa_embed-0.17.6/local_dependencies/summa-core/src/components/default_tokenizers.rs
--rw-r--r--   0      501       20    13820 2023-07-03 15:18:18.000000 summa_embed-0.17.6/local_dependencies/summa-core/src/components/fruit_extractors.rs
--rw-r--r--   0      501       20    31266 2023-07-03 15:18:18.000000 summa_embed-0.17.6/local_dependencies/summa-core/src/components/index_holder.rs
--rw-r--r--   0      501       20    13903 2023-07-03 15:18:18.000000 summa_embed-0.17.6/local_dependencies/summa-core/src/components/index_registry.rs
--rw-r--r--   0      501       20    20309 2023-07-03 15:18:18.000000 summa_embed-0.17.6/local_dependencies/summa-core/src/components/index_writer_holder.rs
--rw-r--r--   0      501       20     1694 2023-07-03 15:18:18.000000 summa_embed-0.17.6/local_dependencies/summa-core/src/components/merge_policies/log_merge_policy.rs
--rw-r--r--   0      501       20      144 2023-07-03 15:18:18.000000 summa_embed-0.17.6/local_dependencies/summa-core/src/components/merge_policies/mod.rs
--rw-r--r--   0      501       20     2045 2023-07-03 15:18:18.000000 summa_embed-0.17.6/local_dependencies/summa-core/src/components/merge_policies/temporal_merge_policy.rs
--rw-r--r--   0      501       20     5962 2023-07-03 15:18:18.000000 summa_embed-0.17.6/local_dependencies/summa-core/src/components/mod.rs
--rw-r--r--   0      501       20     6539 2023-07-03 15:18:18.000000 summa_embed-0.17.6/local_dependencies/summa-core/src/components/queries/exists_query.rs
--rw-r--r--   0      501       20       54 2023-07-03 15:18:18.000000 summa_embed-0.17.6/local_dependencies/summa-core/src/components/queries/mod.rs
--rw-r--r--   0      501       20      250 2023-07-03 15:18:18.000000 summa_embed-0.17.6/local_dependencies/summa-core/src/components/query_parser/mod.rs
--rw-r--r--   0      501       20     1193 2023-07-03 15:18:18.000000 summa_embed-0.17.6/local_dependencies/summa-core/src/components/query_parser/morphology/english.rs
--rw-r--r--   0      501       20      693 2023-07-03 15:18:18.000000 summa_embed-0.17.6/local_dependencies/summa-core/src/components/query_parser/morphology/manager.rs
--rw-r--r--   0      501       20     2092 2023-07-03 15:18:18.000000 summa_embed-0.17.6/local_dependencies/summa-core/src/components/query_parser/morphology/mod.rs
--rw-r--r--   0      501       20    13740 2023-07-03 15:18:18.000000 summa_embed-0.17.6/local_dependencies/summa-core/src/components/query_parser/proto_query_parser.rs
--rw-r--r--   0      501       20     1899 2023-07-03 15:18:18.000000 summa_embed-0.17.6/local_dependencies/summa-core/src/components/query_parser/summa_ql.pest
--rw-r--r--   0      501       20    63781 2023-07-03 15:18:18.000000 summa_embed-0.17.6/local_dependencies/summa-core/src/components/query_parser/summa_ql.rs
--rw-r--r--   0      501       20     5812 2023-07-03 15:18:18.000000 summa_embed-0.17.6/local_dependencies/summa-core/src/components/query_parser/term_field_mappers.rs
--rw-r--r--   0      501       20     2498 2023-07-03 15:18:18.000000 summa_embed-0.17.6/local_dependencies/summa-core/src/components/query_parser/utils.rs
--rw-r--r--   0      501       20     2216 2023-07-03 15:18:18.000000 summa_embed-0.17.6/local_dependencies/summa-core/src/components/segment_attributes.rs
--rw-r--r--   0      501       20     1901 2023-07-03 15:18:18.000000 summa_embed-0.17.6/local_dependencies/summa-core/src/components/snippet_generator.rs
--rw-r--r--   0      501       20    11998 2023-07-03 15:18:18.000000 summa_embed-0.17.6/local_dependencies/summa-core/src/components/summa_document.rs
--rw-r--r--   0      501       20     7462 2023-07-03 15:18:18.000000 summa_embed-0.17.6/local_dependencies/summa-core/src/components/summa_tokenizer.rs
--rw-r--r--   0      501       20     2162 2023-07-03 15:18:18.000000 summa_embed-0.17.6/local_dependencies/summa-core/src/configs/config_proxy.rs
--rw-r--r--   0      501       20     4526 2023-07-03 15:18:18.000000 summa_embed-0.17.6/local_dependencies/summa-core/src/configs/core.rs
--rw-r--r--   0      501       20     3512 2023-07-03 15:18:18.000000 summa_embed-0.17.6/local_dependencies/summa-core/src/configs/file_proxy.rs
--rw-r--r--   0      501       20      383 2023-07-03 15:18:18.000000 summa_embed-0.17.6/local_dependencies/summa-core/src/configs/mod.rs
--rw-r--r--   0      501       20     3335 2023-07-03 15:18:18.000000 summa_embed-0.17.6/local_dependencies/summa-core/src/configs/partial_proxy.rs
--rw-r--r--   0      501       20     8009 2023-07-03 15:18:18.000000 summa_embed-0.17.6/local_dependencies/summa-core/src/directories/byte_range_cache.rs
--rw-r--r--   0      501       20     8015 2023-07-03 15:18:18.000000 summa_embed-0.17.6/local_dependencies/summa-core/src/directories/caching_directory.rs
--rw-r--r--   0      501       20     7015 2023-07-03 15:18:18.000000 summa_embed-0.17.6/local_dependencies/summa-core/src/directories/debug_proxy_directory.rs
--rw-r--r--   0      501       20     5258 2023-07-03 15:18:18.000000 summa_embed-0.17.6/local_dependencies/summa-core/src/directories/external_requests.rs
--rw-r--r--   0      501       20    17667 2023-07-03 15:18:18.000000 summa_embed-0.17.6/local_dependencies/summa-core/src/directories/hot_cache_directory.rs
--rw-r--r--   0      501       20     2255 2023-07-03 15:18:18.000000 summa_embed-0.17.6/local_dependencies/summa-core/src/directories/mod.rs
--rw-r--r--   0      501       20     6756 2023-07-03 15:18:18.000000 summa_embed-0.17.6/local_dependencies/summa-core/src/directories/network_directory.rs
--rw-r--r--   0      501       20     5192 2023-07-03 15:18:18.000000 summa_embed-0.17.6/local_dependencies/summa-core/src/errors.rs
--rw-r--r--   0      501       20     2421 2023-07-03 15:18:18.000000 summa_embed-0.17.6/local_dependencies/summa-core/src/hyper_external_request.rs
--rw-r--r--   0      501       20      742 2023-07-03 15:18:18.000000 summa_embed-0.17.6/local_dependencies/summa-core/src/lib.rs
--rw-r--r--   0      501       20     1471 2023-07-03 15:18:18.000000 summa_embed-0.17.6/local_dependencies/summa-core/src/metrics/cache_metrics.rs
--rw-r--r--   0      501       20      960 2023-07-03 15:18:18.000000 summa_embed-0.17.6/local_dependencies/summa-core/src/metrics/label.rs
--rw-r--r--   0      501       20       92 2023-07-03 15:18:18.000000 summa_embed-0.17.6/local_dependencies/summa-core/src/metrics/mod.rs
--rw-r--r--   0      501       20      583 2023-07-03 15:18:18.000000 summa_embed-0.17.6/local_dependencies/summa-core/src/page_rank.rs
--rw-r--r--   0      501       20     5474 2023-07-03 15:18:18.000000 summa_embed-0.17.6/local_dependencies/summa-core/src/proto_traits/aggregation.rs
--rw-r--r--   0      501       20     2294 2023-07-03 15:18:18.000000 summa_embed-0.17.6/local_dependencies/summa-core/src/proto_traits/compression.rs
--rw-r--r--   0      501       20     1068 2023-07-03 15:18:18.000000 summa_embed-0.17.6/local_dependencies/summa-core/src/proto_traits/merge_policy.rs
--rw-r--r--   0      501       20      323 2023-07-03 15:18:18.000000 summa_embed-0.17.6/local_dependencies/summa-core/src/proto_traits/mod.rs
--rw-r--r--   0      501       20      662 2023-07-03 15:18:18.000000 summa_embed-0.17.6/local_dependencies/summa-core/src/proto_traits/order.rs
--rw-r--r--   0      501       20      582 2023-07-03 15:18:18.000000 summa_embed-0.17.6/local_dependencies/summa-core/src/proto_traits/snippet.rs
--rw-r--r--   0      501       20      411 2023-07-03 15:18:18.000000 summa_embed-0.17.6/local_dependencies/summa-core/src/proto_traits/sort_by_field.rs
--rw-r--r--   0      501       20     2048 2023-07-03 15:18:18.000000 summa_embed-0.17.6/local_dependencies/summa-core/src/scorers/eval_scorer.rs
--rw-r--r--   0      501       20     1538 2023-07-03 15:18:18.000000 summa_embed-0.17.6/local_dependencies/summa-core/src/scorers/eval_scorer_tweaker.rs
--rw-r--r--   0      501       20      826 2023-07-03 15:18:18.000000 summa_embed-0.17.6/local_dependencies/summa-core/src/scorers/fast_field_iterator.rs
--rw-r--r--   0      501       20      218 2023-07-03 15:18:18.000000 summa_embed-0.17.6/local_dependencies/summa-core/src/scorers/mod.rs
--rw-r--r--   0      501       20      480 2023-07-03 15:18:18.000000 summa_embed-0.17.6/local_dependencies/summa-core/src/scorers/safe_into_f64.rs
--rw-r--r--   0      501       20     7908 2023-07-03 15:18:18.000000 summa_embed-0.17.6/local_dependencies/summa-core/src/scorers/segment_eval_scorer.rs
--rw-r--r--   0      501       20      415 2023-07-03 15:18:18.000000 summa_embed-0.17.6/local_dependencies/summa-core/src/utils/mod.rs
--rw-r--r--   0      501       20      309 2023-07-03 15:18:18.000000 summa_embed-0.17.6/local_dependencies/summa-core/src/utils/random.rs
--rw-r--r--   0      501       20     3165 2023-07-03 15:18:18.000000 summa_embed-0.17.6/local_dependencies/summa-core/src/utils/sync.rs
--rw-r--r--   0      501       20      559 2023-07-03 15:18:18.000000 summa_embed-0.17.6/local_dependencies/summa-core/src/validators.rs
--rw-r--r--   0        0        0      905 1970-01-01 00:00:00.000000 summa_embed-0.17.6/local_dependencies/summa-proto/Cargo.toml
--rw-r--r--   0      501       20     1050 2023-07-03 15:18:18.000000 summa_embed-0.17.6/local_dependencies/summa-proto/LICENSE
--rw-r--r--   0      501       20     2381 2023-07-03 15:18:18.000000 summa_embed-0.17.6/local_dependencies/summa-proto/build.rs
--rwxr-xr-x   0      501       20      244 2023-07-03 15:18:18.000000 summa_embed-0.17.6/local_dependencies/summa-proto/gen-docs.sh
--rw-r--r--   0      501       20     2561 2023-07-03 15:18:18.000000 summa_embed-0.17.6/local_dependencies/summa-proto/markdown.tmpl
--rw-r--r--   0      501       20        0 2023-07-03 15:18:18.000000 summa_embed-0.17.6/local_dependencies/summa-proto/proto/__init__.py
--rw-r--r--   0      501       20     1556 2023-07-03 15:18:18.000000 summa_embed-0.17.6/local_dependencies/summa-proto/proto/consumer_service.proto
--rw-r--r--   0      501       20      393 2023-07-03 15:18:18.000000 summa_embed-0.17.6/local_dependencies/summa-proto/proto/dag_pb.proto
--rw-r--r--   0      501       20    10598 2023-07-03 15:18:18.000000 summa_embed-0.17.6/local_dependencies/summa-proto/proto/index_service.proto
--rw-r--r--   0      501       20     7741 2023-07-03 15:18:18.000000 summa_embed-0.17.6/local_dependencies/summa-proto/proto/query.proto
--rw-r--r--   0      501       20      499 2023-07-03 15:18:18.000000 summa_embed-0.17.6/local_dependencies/summa-proto/proto/reflection_service.proto
--rw-r--r--   0      501       20      867 2023-07-03 15:18:18.000000 summa_embed-0.17.6/local_dependencies/summa-proto/proto/search_service.proto
--rw-r--r--   0      501       20      407 2023-07-03 15:18:18.000000 summa_embed-0.17.6/local_dependencies/summa-proto/proto/unixfs.proto
--rw-r--r--   0      501       20       96 2023-07-03 15:18:18.000000 summa_embed-0.17.6/local_dependencies/summa-proto/proto/utils.proto
--rw-r--r--   0      501       20     2523 2023-07-03 15:18:18.000000 summa_embed-0.17.6/local_dependencies/summa-proto/src/lib.rs
--rw-r--r--   0      501       20     2683 2023-07-03 15:18:18.000000 summa_embed-0.17.6/local_dependencies/summa-proto/src/proto_traits/collector.rs
--rw-r--r--   0      501       20      212 2023-07-03 15:18:18.000000 summa_embed-0.17.6/local_dependencies/summa-proto/src/proto_traits/mod.rs
--rw-r--r--   0      501       20      394 2023-07-03 15:18:18.000000 summa_embed-0.17.6/local_dependencies/summa-proto/src/proto_traits/query.rs
--rw-r--r--   0      501       20      613 2023-07-03 15:18:18.000000 summa_embed-0.17.6/local_dependencies/summa-proto/src/proto_traits/score.rs
--rw-r--r--   0        0        0     1008 1970-01-01 00:00:00.000000 summa_embed-0.17.6/Cargo.toml
--rw-r--r--   0      501       20      685 2023-07-03 15:18:18.000000 summa_embed-0.17.6/.gitignore
--rw-r--r--   0      501       20      400 2023-07-03 15:18:18.000000 summa_embed-0.17.6/pyproject.toml
--rw-r--r--   0      501       20     2199 2023-07-03 15:18:18.000000 summa_embed-0.17.6/src/lib.rs
--rw-r--r--   0      501       20   101640 2023-07-03 15:18:31.000000 summa_embed-0.17.6/Cargo.lock
--rw-r--r--   0        0        0      261 1970-01-01 00:00:00.000000 summa_embed-0.17.6/PKG-INFO
+-rw-r--r--   0        0        0      905 1970-01-01 00:00:00.000000 summa_embed-0.17.7/local_dependencies/summa-proto/Cargo.toml
+-rw-r--r--   0      501       20     1050 2023-07-05 08:54:48.000000 summa_embed-0.17.7/local_dependencies/summa-proto/LICENSE
+-rw-r--r--   0      501       20     2381 2023-07-05 08:54:48.000000 summa_embed-0.17.7/local_dependencies/summa-proto/build.rs
+-rwxr-xr-x   0      501       20      244 2023-07-05 08:54:48.000000 summa_embed-0.17.7/local_dependencies/summa-proto/gen-docs.sh
+-rw-r--r--   0      501       20     2561 2023-07-05 08:54:48.000000 summa_embed-0.17.7/local_dependencies/summa-proto/markdown.tmpl
+-rw-r--r--   0      501       20        0 2023-07-05 08:54:49.000000 summa_embed-0.17.7/local_dependencies/summa-proto/proto/__init__.py
+-rw-r--r--   0      501       20     1556 2023-07-05 08:54:49.000000 summa_embed-0.17.7/local_dependencies/summa-proto/proto/consumer_service.proto
+-rw-r--r--   0      501       20      393 2023-07-05 08:54:49.000000 summa_embed-0.17.7/local_dependencies/summa-proto/proto/dag_pb.proto
+-rw-r--r--   0      501       20    10598 2023-07-05 08:54:49.000000 summa_embed-0.17.7/local_dependencies/summa-proto/proto/index_service.proto
+-rw-r--r--   0      501       20     7741 2023-07-05 08:54:49.000000 summa_embed-0.17.7/local_dependencies/summa-proto/proto/query.proto
+-rw-r--r--   0      501       20      499 2023-07-05 08:54:49.000000 summa_embed-0.17.7/local_dependencies/summa-proto/proto/reflection_service.proto
+-rw-r--r--   0      501       20      867 2023-07-05 08:54:49.000000 summa_embed-0.17.7/local_dependencies/summa-proto/proto/search_service.proto
+-rw-r--r--   0      501       20      407 2023-07-05 08:54:49.000000 summa_embed-0.17.7/local_dependencies/summa-proto/proto/unixfs.proto
+-rw-r--r--   0      501       20       96 2023-07-05 08:54:49.000000 summa_embed-0.17.7/local_dependencies/summa-proto/proto/utils.proto
+-rw-r--r--   0      501       20     2523 2023-07-05 08:54:49.000000 summa_embed-0.17.7/local_dependencies/summa-proto/src/lib.rs
+-rw-r--r--   0      501       20     2683 2023-07-05 08:54:49.000000 summa_embed-0.17.7/local_dependencies/summa-proto/src/proto_traits/collector.rs
+-rw-r--r--   0      501       20      212 2023-07-05 08:54:49.000000 summa_embed-0.17.7/local_dependencies/summa-proto/src/proto_traits/mod.rs
+-rw-r--r--   0      501       20      394 2023-07-05 08:54:49.000000 summa_embed-0.17.7/local_dependencies/summa-proto/src/proto_traits/query.rs
+-rw-r--r--   0      501       20      613 2023-07-05 08:54:49.000000 summa_embed-0.17.7/local_dependencies/summa-proto/src/proto_traits/score.rs
+-rw-r--r--   0        0        0     2113 1970-01-01 00:00:00.000000 summa_embed-0.17.7/local_dependencies/summa-core/Cargo.toml
+-rw-r--r--   0      501       20     1050 2023-07-05 08:54:45.000000 summa_embed-0.17.7/local_dependencies/summa-core/LICENSE
+-rw-r--r--   0      501       20   370551 2023-07-05 08:54:45.000000 summa_embed-0.17.7/local_dependencies/summa-core/dictionaries/drugs.csv
+-rw-r--r--   0      501       20       92 2023-07-05 08:54:45.000000 summa_embed-0.17.7/local_dependencies/summa-core/src/collectors/mod.rs
+-rw-r--r--   0      501       20     7233 2023-07-05 08:54:45.000000 summa_embed-0.17.7/local_dependencies/summa-core/src/collectors/reservoir_sampling_collector.rs
+-rw-r--r--   0      501       20     2107 2023-07-05 08:54:45.000000 summa_embed-0.17.7/local_dependencies/summa-core/src/components/custom_serializer.rs
+-rw-r--r--   0      501       20     5492 2023-07-05 08:54:45.000000 summa_embed-0.17.7/local_dependencies/summa-core/src/components/default_tokenizers.rs
+-rw-r--r--   0      501       20    13820 2023-07-05 08:54:45.000000 summa_embed-0.17.7/local_dependencies/summa-core/src/components/fruit_extractors.rs
+-rw-r--r--   0      501       20    31266 2023-07-05 08:54:45.000000 summa_embed-0.17.7/local_dependencies/summa-core/src/components/index_holder.rs
+-rw-r--r--   0      501       20    13903 2023-07-05 08:54:46.000000 summa_embed-0.17.7/local_dependencies/summa-core/src/components/index_registry.rs
+-rw-r--r--   0      501       20    20309 2023-07-05 08:54:46.000000 summa_embed-0.17.7/local_dependencies/summa-core/src/components/index_writer_holder.rs
+-rw-r--r--   0      501       20     1694 2023-07-05 08:54:46.000000 summa_embed-0.17.7/local_dependencies/summa-core/src/components/merge_policies/log_merge_policy.rs
+-rw-r--r--   0      501       20      144 2023-07-05 08:54:46.000000 summa_embed-0.17.7/local_dependencies/summa-core/src/components/merge_policies/mod.rs
+-rw-r--r--   0      501       20     2045 2023-07-05 08:54:46.000000 summa_embed-0.17.7/local_dependencies/summa-core/src/components/merge_policies/temporal_merge_policy.rs
+-rw-r--r--   0      501       20     5962 2023-07-05 08:54:46.000000 summa_embed-0.17.7/local_dependencies/summa-core/src/components/mod.rs
+-rw-r--r--   0      501       20     6539 2023-07-05 08:54:46.000000 summa_embed-0.17.7/local_dependencies/summa-core/src/components/queries/exists_query.rs
+-rw-r--r--   0      501       20       54 2023-07-05 08:54:46.000000 summa_embed-0.17.7/local_dependencies/summa-core/src/components/queries/mod.rs
+-rw-r--r--   0      501       20      250 2023-07-05 08:54:46.000000 summa_embed-0.17.7/local_dependencies/summa-core/src/components/query_parser/mod.rs
+-rw-r--r--   0      501       20     1193 2023-07-05 08:54:46.000000 summa_embed-0.17.7/local_dependencies/summa-core/src/components/query_parser/morphology/english.rs
+-rw-r--r--   0      501       20      693 2023-07-05 08:54:46.000000 summa_embed-0.17.7/local_dependencies/summa-core/src/components/query_parser/morphology/manager.rs
+-rw-r--r--   0      501       20     2092 2023-07-05 08:54:46.000000 summa_embed-0.17.7/local_dependencies/summa-core/src/components/query_parser/morphology/mod.rs
+-rw-r--r--   0      501       20    13740 2023-07-05 08:54:46.000000 summa_embed-0.17.7/local_dependencies/summa-core/src/components/query_parser/proto_query_parser.rs
+-rw-r--r--   0      501       20     1899 2023-07-05 08:54:46.000000 summa_embed-0.17.7/local_dependencies/summa-core/src/components/query_parser/summa_ql.pest
+-rw-r--r--   0      501       20    63781 2023-07-05 08:54:46.000000 summa_embed-0.17.7/local_dependencies/summa-core/src/components/query_parser/summa_ql.rs
+-rw-r--r--   0      501       20     5812 2023-07-05 08:54:46.000000 summa_embed-0.17.7/local_dependencies/summa-core/src/components/query_parser/term_field_mappers.rs
+-rw-r--r--   0      501       20     2498 2023-07-05 08:54:46.000000 summa_embed-0.17.7/local_dependencies/summa-core/src/components/query_parser/utils.rs
+-rw-r--r--   0      501       20     2216 2023-07-05 08:54:47.000000 summa_embed-0.17.7/local_dependencies/summa-core/src/components/segment_attributes.rs
+-rw-r--r--   0      501       20     1901 2023-07-05 08:54:47.000000 summa_embed-0.17.7/local_dependencies/summa-core/src/components/snippet_generator.rs
+-rw-r--r--   0      501       20    11998 2023-07-05 08:54:47.000000 summa_embed-0.17.7/local_dependencies/summa-core/src/components/summa_document.rs
+-rw-r--r--   0      501       20     7462 2023-07-05 08:54:47.000000 summa_embed-0.17.7/local_dependencies/summa-core/src/components/summa_tokenizer.rs
+-rw-r--r--   0      501       20     2162 2023-07-05 08:54:47.000000 summa_embed-0.17.7/local_dependencies/summa-core/src/configs/config_proxy.rs
+-rw-r--r--   0      501       20     4526 2023-07-05 08:54:47.000000 summa_embed-0.17.7/local_dependencies/summa-core/src/configs/core.rs
+-rw-r--r--   0      501       20     3512 2023-07-05 08:54:47.000000 summa_embed-0.17.7/local_dependencies/summa-core/src/configs/file_proxy.rs
+-rw-r--r--   0      501       20      383 2023-07-05 08:54:47.000000 summa_embed-0.17.7/local_dependencies/summa-core/src/configs/mod.rs
+-rw-r--r--   0      501       20     3335 2023-07-05 08:54:47.000000 summa_embed-0.17.7/local_dependencies/summa-core/src/configs/partial_proxy.rs
+-rw-r--r--   0      501       20     8009 2023-07-05 08:54:47.000000 summa_embed-0.17.7/local_dependencies/summa-core/src/directories/byte_range_cache.rs
+-rw-r--r--   0      501       20     8015 2023-07-05 08:54:47.000000 summa_embed-0.17.7/local_dependencies/summa-core/src/directories/caching_directory.rs
+-rw-r--r--   0      501       20     7015 2023-07-05 08:54:47.000000 summa_embed-0.17.7/local_dependencies/summa-core/src/directories/debug_proxy_directory.rs
+-rw-r--r--   0      501       20     5258 2023-07-05 08:54:47.000000 summa_embed-0.17.7/local_dependencies/summa-core/src/directories/external_requests.rs
+-rw-r--r--   0      501       20    17667 2023-07-05 08:54:47.000000 summa_embed-0.17.7/local_dependencies/summa-core/src/directories/hot_cache_directory.rs
+-rw-r--r--   0      501       20     2255 2023-07-05 08:54:47.000000 summa_embed-0.17.7/local_dependencies/summa-core/src/directories/mod.rs
+-rw-r--r--   0      501       20     6756 2023-07-05 08:54:47.000000 summa_embed-0.17.7/local_dependencies/summa-core/src/directories/network_directory.rs
+-rw-r--r--   0      501       20     5192 2023-07-05 08:54:47.000000 summa_embed-0.17.7/local_dependencies/summa-core/src/errors.rs
+-rw-r--r--   0      501       20     2421 2023-07-05 08:54:47.000000 summa_embed-0.17.7/local_dependencies/summa-core/src/hyper_external_request.rs
+-rw-r--r--   0      501       20      742 2023-07-05 08:54:47.000000 summa_embed-0.17.7/local_dependencies/summa-core/src/lib.rs
+-rw-r--r--   0      501       20     1471 2023-07-05 08:54:47.000000 summa_embed-0.17.7/local_dependencies/summa-core/src/metrics/cache_metrics.rs
+-rw-r--r--   0      501       20      960 2023-07-05 08:54:47.000000 summa_embed-0.17.7/local_dependencies/summa-core/src/metrics/label.rs
+-rw-r--r--   0      501       20       92 2023-07-05 08:54:47.000000 summa_embed-0.17.7/local_dependencies/summa-core/src/metrics/mod.rs
+-rw-r--r--   0      501       20      583 2023-07-05 08:54:47.000000 summa_embed-0.17.7/local_dependencies/summa-core/src/page_rank.rs
+-rw-r--r--   0      501       20     5474 2023-07-05 08:54:47.000000 summa_embed-0.17.7/local_dependencies/summa-core/src/proto_traits/aggregation.rs
+-rw-r--r--   0      501       20     2294 2023-07-05 08:54:47.000000 summa_embed-0.17.7/local_dependencies/summa-core/src/proto_traits/compression.rs
+-rw-r--r--   0      501       20     1068 2023-07-05 08:54:47.000000 summa_embed-0.17.7/local_dependencies/summa-core/src/proto_traits/merge_policy.rs
+-rw-r--r--   0      501       20      323 2023-07-05 08:54:47.000000 summa_embed-0.17.7/local_dependencies/summa-core/src/proto_traits/mod.rs
+-rw-r--r--   0      501       20      662 2023-07-05 08:54:47.000000 summa_embed-0.17.7/local_dependencies/summa-core/src/proto_traits/order.rs
+-rw-r--r--   0      501       20      582 2023-07-05 08:54:47.000000 summa_embed-0.17.7/local_dependencies/summa-core/src/proto_traits/snippet.rs
+-rw-r--r--   0      501       20      411 2023-07-05 08:54:47.000000 summa_embed-0.17.7/local_dependencies/summa-core/src/proto_traits/sort_by_field.rs
+-rw-r--r--   0      501       20     2048 2023-07-05 08:54:47.000000 summa_embed-0.17.7/local_dependencies/summa-core/src/scorers/eval_scorer.rs
+-rw-r--r--   0      501       20     1538 2023-07-05 08:54:47.000000 summa_embed-0.17.7/local_dependencies/summa-core/src/scorers/eval_scorer_tweaker.rs
+-rw-r--r--   0      501       20      826 2023-07-05 08:54:48.000000 summa_embed-0.17.7/local_dependencies/summa-core/src/scorers/fast_field_iterator.rs
+-rw-r--r--   0      501       20      218 2023-07-05 08:54:48.000000 summa_embed-0.17.7/local_dependencies/summa-core/src/scorers/mod.rs
+-rw-r--r--   0      501       20      480 2023-07-05 08:54:48.000000 summa_embed-0.17.7/local_dependencies/summa-core/src/scorers/safe_into_f64.rs
+-rw-r--r--   0      501       20     7908 2023-07-05 08:54:48.000000 summa_embed-0.17.7/local_dependencies/summa-core/src/scorers/segment_eval_scorer.rs
+-rw-r--r--   0      501       20      415 2023-07-05 08:54:48.000000 summa_embed-0.17.7/local_dependencies/summa-core/src/utils/mod.rs
+-rw-r--r--   0      501       20      309 2023-07-05 08:54:48.000000 summa_embed-0.17.7/local_dependencies/summa-core/src/utils/random.rs
+-rw-r--r--   0      501       20     3165 2023-07-05 08:54:48.000000 summa_embed-0.17.7/local_dependencies/summa-core/src/utils/sync.rs
+-rw-r--r--   0      501       20      559 2023-07-05 08:54:48.000000 summa_embed-0.17.7/local_dependencies/summa-core/src/validators.rs
+-rw-r--r--   0        0        0     2767 1970-01-01 00:00:00.000000 summa_embed-0.17.7/local_dependencies/summa-server/Cargo.toml
+-rw-r--r--   0      501       20       43 2023-07-05 08:54:49.000000 summa_embed-0.17.7/local_dependencies/summa-server/.cargo/config.toml
+-rw-r--r--   0      501       20     1050 2023-07-05 08:54:49.000000 summa_embed-0.17.7/local_dependencies/summa-server/LICENSE
+-rw-r--r--   0      501       20     2832 2023-07-05 08:54:50.000000 summa_embed-0.17.7/local_dependencies/summa-server/src/apis/consumer.rs
+-rw-r--r--   0      501       20    13268 2023-07-05 08:54:50.000000 summa_embed-0.17.7/local_dependencies/summa-server/src/apis/index.rs
+-rw-r--r--   0      501       20      105 2023-07-05 08:54:50.000000 summa_embed-0.17.7/local_dependencies/summa-server/src/apis/mod.rs
+-rw-r--r--   0      501       20     2909 2023-07-05 08:54:50.000000 summa_embed-0.17.7/local_dependencies/summa-server/src/apis/reflection.rs
+-rw-r--r--   0      501       20     1278 2023-07-05 08:54:50.000000 summa_embed-0.17.7/local_dependencies/summa-server/src/apis/search.rs
+-rw-r--r--   0      501       20      783 2023-07-05 08:54:50.000000 summa_embed-0.17.7/local_dependencies/summa-server/src/bin/main.rs
+-rw-r--r--   0      501       20     5305 2023-07-05 08:54:50.000000 summa_embed-0.17.7/local_dependencies/summa-server/src/components/consumer_manager.rs
+-rw-r--r--   0      501       20      813 2023-07-05 08:54:50.000000 summa_embed-0.17.7/local_dependencies/summa-server/src/components/consumers/consumer_thread.rs
+-rw-r--r--   0      501       20     1082 2023-07-05 08:54:50.000000 summa_embed-0.17.7/local_dependencies/summa-server/src/components/consumers/dummy.rs
+-rw-r--r--   0      501       20    11633 2023-07-05 08:54:50.000000 summa_embed-0.17.7/local_dependencies/summa-server/src/components/consumers/kafka/consumer.rs
+-rw-r--r--   0      501       20      270 2023-07-05 08:54:50.000000 summa_embed-0.17.7/local_dependencies/summa-server/src/components/consumers/kafka/mod.rs
+-rw-r--r--   0      501       20      532 2023-07-05 08:54:50.000000 summa_embed-0.17.7/local_dependencies/summa-server/src/components/consumers/kafka/status.rs
+-rw-r--r--   0      501       20      155 2023-07-05 08:54:50.000000 summa_embed-0.17.7/local_dependencies/summa-server/src/components/consumers/mod.rs
+-rw-r--r--   0      501       20     3811 2023-07-05 08:54:50.000000 summa_embed-0.17.7/local_dependencies/summa-server/src/components/index_meter.rs
+-rw-r--r--   0      501       20      258 2023-07-05 08:54:50.000000 summa_embed-0.17.7/local_dependencies/summa-server/src/components/mod.rs
+-rw-r--r--   0      501       20      943 2023-07-05 08:54:50.000000 summa_embed-0.17.7/local_dependencies/summa-server/src/configs/api.rs
+-rw-r--r--   0      501       20      919 2023-07-05 08:54:50.000000 summa_embed-0.17.7/local_dependencies/summa-server/src/configs/consumer.rs
+-rw-r--r--   0      501       20      434 2023-07-05 08:54:51.000000 summa_embed-0.17.7/local_dependencies/summa-server/src/configs/metrics.rs
+-rw-r--r--   0      501       20      116 2023-07-05 08:54:51.000000 summa_embed-0.17.7/local_dependencies/summa-server/src/configs/mod.rs
+-rw-r--r--   0      501       20     4268 2023-07-05 08:54:51.000000 summa_embed-0.17.7/local_dependencies/summa-server/src/configs/server.rs
+-rw-r--r--   0      501       20      991 2023-07-05 08:54:51.000000 summa_embed-0.17.7/local_dependencies/summa-server/src/configs/store.rs
+-rw-r--r--   0      501       20     3459 2023-07-05 08:54:51.000000 summa_embed-0.17.7/local_dependencies/summa-server/src/errors.rs
+-rw-r--r--   0      501       20     1427 2023-07-05 08:54:51.000000 summa_embed-0.17.7/local_dependencies/summa-server/src/lib.rs
+-rw-r--r--   0      501       20     3681 2023-07-05 08:54:51.000000 summa_embed-0.17.7/local_dependencies/summa-server/src/logging.rs
+-rw-r--r--   0      501       20    15704 2023-07-05 08:54:51.000000 summa_embed-0.17.7/local_dependencies/summa-server/src/server.rs
+-rw-r--r--   0      501       20     8110 2023-07-05 08:54:51.000000 summa_embed-0.17.7/local_dependencies/summa-server/src/services/api.rs
+-rw-r--r--   0      501       20    40154 2023-07-05 08:54:51.000000 summa_embed-0.17.7/local_dependencies/summa-server/src/services/index.rs
+-rw-r--r--   0      501       20     5174 2023-07-05 08:54:51.000000 summa_embed-0.17.7/local_dependencies/summa-server/src/services/metrics.rs
+-rw-r--r--   0      501       20      287 2023-07-05 08:54:51.000000 summa_embed-0.17.7/local_dependencies/summa-server/src/services/mod.rs
+-rw-r--r--   0      501       20     2108 2023-07-05 08:54:51.000000 summa_embed-0.17.7/local_dependencies/summa-server/src/utils/mod.rs
+-rw-r--r--   0      501       20      923 2023-07-05 08:54:51.000000 summa_embed-0.17.7/local_dependencies/summa-server/src/utils/thread_handler.rs
+-rw-r--r--   0        0        0     1008 1970-01-01 00:00:00.000000 summa_embed-0.17.7/Cargo.toml
+-rw-r--r--   0      501       20      685 2023-07-05 08:54:48.000000 summa_embed-0.17.7/.gitignore
+-rw-r--r--   0      501       20      400 2023-07-05 08:54:48.000000 summa_embed-0.17.7/pyproject.toml
+-rw-r--r--   0      501       20     2199 2023-07-05 08:54:48.000000 summa_embed-0.17.7/src/lib.rs
+-rw-r--r--   0      501       20   101390 2023-07-05 08:55:23.000000 summa_embed-0.17.7/Cargo.lock
+-rw-r--r--   0        0        0      261 1970-01-01 00:00:00.000000 summa_embed-0.17.7/PKG-INFO
```

### Comparing `summa_embed-0.17.6/local_dependencies/summa-server/Cargo.toml` & `summa_embed-0.17.7/local_dependencies/summa-server/Cargo.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 [package]
 edition = "2021"
 name = "summa-server"
-version = "0.17.6"
+version = "0.17.7"
 license-file = "LICENSE"
 description = "Fast full-text search server"
 homepage = "https://github.com/izihawa/summa"
 repository = "https://github.com/izihawa/summa"
 keywords = ["async", "search", "server", "grpc"]
 
 [lib]
@@ -51,15 +51,15 @@
 rand = { version = "0.8", features = ["small_rng"] }
 rdkafka = { version = "0.29", optional = true }
 rlimit = "0.9"
 serde = { version = "1.0", default_features = false, features = ["derive", "std"] }
 serde_derive = "1.0"
 serde_json = { version = "1.0" }
 serde_yaml = { version = "0.8" }
-summa-core = { version = "0.17.6", path = "../summa-core", features = ["fs", "hyper-external-request", "tokio-rt"] }
+summa-core = { version = "0.17.7", path = "../summa-core", features = ["fs", "hyper-external-request", "tokio-rt"] }
 summa-proto = { features = ["grpc"] , path = "../summa-proto" }
 take_mut = "0.2"
 tantivy = { git = "https://github.com/izihawa/tantivy", branch = "feature/summa", default_features = false, features = ["quickwit", "zstd-compression"] }
 tantivy-fst = "0.4.0"
 time = { version = "0.3", features = ["serde-well-known", "wasm-bindgen"] }
 thiserror = "1.0"
 tokio = { version = "1.25", default_features = false , features = ["full", "time"] }
```

### Comparing `summa_embed-0.17.6/local_dependencies/summa-server/LICENSE` & `summa_embed-0.17.7/local_dependencies/summa-proto/LICENSE`

 * *Files identical despite different names*

### Comparing `summa_embed-0.17.6/local_dependencies/summa-server/src/apis/consumer.rs` & `summa_embed-0.17.7/local_dependencies/summa-server/src/apis/consumer.rs`

 * *Files identical despite different names*

### Comparing `summa_embed-0.17.6/local_dependencies/summa-server/src/apis/index.rs` & `summa_embed-0.17.7/local_dependencies/summa-server/src/apis/index.rs`

 * *Files identical despite different names*

### Comparing `summa_embed-0.17.6/local_dependencies/summa-server/src/apis/reflection.rs` & `summa_embed-0.17.7/local_dependencies/summa-server/src/apis/reflection.rs`

 * *Files identical despite different names*

### Comparing `summa_embed-0.17.6/local_dependencies/summa-server/src/apis/search.rs` & `summa_embed-0.17.7/local_dependencies/summa-server/src/apis/search.rs`

 * *Files identical despite different names*

### Comparing `summa_embed-0.17.6/local_dependencies/summa-server/src/bin/main.rs` & `summa_embed-0.17.7/local_dependencies/summa-server/src/bin/main.rs`

 * *Files identical despite different names*

### Comparing `summa_embed-0.17.6/local_dependencies/summa-server/src/components/consumer_manager.rs` & `summa_embed-0.17.7/local_dependencies/summa-server/src/components/consumer_manager.rs`

 * *Files identical despite different names*

### Comparing `summa_embed-0.17.6/local_dependencies/summa-server/src/components/consumers/consumer_thread.rs` & `summa_embed-0.17.7/local_dependencies/summa-server/src/components/consumers/consumer_thread.rs`

 * *Files identical despite different names*

### Comparing `summa_embed-0.17.6/local_dependencies/summa-server/src/components/consumers/dummy.rs` & `summa_embed-0.17.7/local_dependencies/summa-server/src/components/consumers/dummy.rs`

 * *Files identical despite different names*

### Comparing `summa_embed-0.17.6/local_dependencies/summa-server/src/components/consumers/kafka/consumer.rs` & `summa_embed-0.17.7/local_dependencies/summa-server/src/components/consumers/kafka/consumer.rs`

 * *Files identical despite different names*

### Comparing `summa_embed-0.17.6/local_dependencies/summa-server/src/components/consumers/kafka/status.rs` & `summa_embed-0.17.7/local_dependencies/summa-server/src/components/consumers/kafka/status.rs`

 * *Files identical despite different names*

### Comparing `summa_embed-0.17.6/local_dependencies/summa-server/src/components/index_meter.rs` & `summa_embed-0.17.7/local_dependencies/summa-server/src/components/index_meter.rs`

 * *Files identical despite different names*

### Comparing `summa_embed-0.17.6/local_dependencies/summa-server/src/configs/api.rs` & `summa_embed-0.17.7/local_dependencies/summa-server/src/configs/api.rs`

 * *Files identical despite different names*

### Comparing `summa_embed-0.17.6/local_dependencies/summa-server/src/configs/consumer.rs` & `summa_embed-0.17.7/local_dependencies/summa-server/src/configs/consumer.rs`

 * *Files identical despite different names*

### Comparing `summa_embed-0.17.6/local_dependencies/summa-server/src/configs/server.rs` & `summa_embed-0.17.7/local_dependencies/summa-server/src/configs/server.rs`

 * *Files identical despite different names*

### Comparing `summa_embed-0.17.6/local_dependencies/summa-server/src/configs/store.rs` & `summa_embed-0.17.7/local_dependencies/summa-server/src/configs/store.rs`

 * *Files identical despite different names*

### Comparing `summa_embed-0.17.6/local_dependencies/summa-server/src/errors.rs` & `summa_embed-0.17.7/local_dependencies/summa-server/src/errors.rs`

 * *Files identical despite different names*

### Comparing `summa_embed-0.17.6/local_dependencies/summa-server/src/lib.rs` & `summa_embed-0.17.7/local_dependencies/summa-server/src/lib.rs`

 * *Files identical despite different names*

### Comparing `summa_embed-0.17.6/local_dependencies/summa-server/src/logging.rs` & `summa_embed-0.17.7/local_dependencies/summa-server/src/logging.rs`

 * *Files identical despite different names*

### Comparing `summa_embed-0.17.6/local_dependencies/summa-server/src/server.rs` & `summa_embed-0.17.7/local_dependencies/summa-server/src/server.rs`

 * *Files identical despite different names*

### Comparing `summa_embed-0.17.6/local_dependencies/summa-server/src/services/api.rs` & `summa_embed-0.17.7/local_dependencies/summa-server/src/services/api.rs`

 * *Files identical despite different names*

### Comparing `summa_embed-0.17.6/local_dependencies/summa-server/src/services/index.rs` & `summa_embed-0.17.7/local_dependencies/summa-server/src/services/index.rs`

 * *Files identical despite different names*

### Comparing `summa_embed-0.17.6/local_dependencies/summa-server/src/services/metrics.rs` & `summa_embed-0.17.7/local_dependencies/summa-server/src/services/metrics.rs`

 * *Files identical despite different names*

### Comparing `summa_embed-0.17.6/local_dependencies/summa-server/src/utils/mod.rs` & `summa_embed-0.17.7/local_dependencies/summa-server/src/utils/mod.rs`

 * *Files identical despite different names*

### Comparing `summa_embed-0.17.6/local_dependencies/summa-server/src/utils/thread_handler.rs` & `summa_embed-0.17.7/local_dependencies/summa-server/src/utils/thread_handler.rs`

 * *Files identical despite different names*

### Comparing `summa_embed-0.17.6/local_dependencies/summa-core/Cargo.toml` & `summa_embed-0.17.7/local_dependencies/summa-core/Cargo.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [package]
 name = "summa-core"
-version = "0.17.6"
+version = "0.17.7"
 authors = ["Pasha Podolsky <ppodolsky@me.com>"]
 edition = "2021"
 license-file = "LICENSE"
 description = "Summa Core library"
 
 [lib]
 name = "summa_core"
```

### Comparing `summa_embed-0.17.6/local_dependencies/summa-core/LICENSE` & `summa_embed-0.17.7/local_dependencies/summa-core/LICENSE`

 * *Files identical despite different names*

### Comparing `summa_embed-0.17.6/local_dependencies/summa-core/dictionaries/drugs.csv` & `summa_embed-0.17.7/local_dependencies/summa-core/dictionaries/drugs.csv`

 * *Files identical despite different names*

### Comparing `summa_embed-0.17.6/local_dependencies/summa-core/src/collectors/reservoir_sampling_collector.rs` & `summa_embed-0.17.7/local_dependencies/summa-core/src/collectors/reservoir_sampling_collector.rs`

 * *Files identical despite different names*

### Comparing `summa_embed-0.17.6/local_dependencies/summa-core/src/components/custom_serializer.rs` & `summa_embed-0.17.7/local_dependencies/summa-core/src/components/custom_serializer.rs`

 * *Files identical despite different names*

### Comparing `summa_embed-0.17.6/local_dependencies/summa-core/src/components/default_tokenizers.rs` & `summa_embed-0.17.7/local_dependencies/summa-core/src/components/default_tokenizers.rs`

 * *Files identical despite different names*

### Comparing `summa_embed-0.17.6/local_dependencies/summa-core/src/components/fruit_extractors.rs` & `summa_embed-0.17.7/local_dependencies/summa-core/src/components/fruit_extractors.rs`

 * *Files identical despite different names*

### Comparing `summa_embed-0.17.6/local_dependencies/summa-core/src/components/index_holder.rs` & `summa_embed-0.17.7/local_dependencies/summa-core/src/components/index_holder.rs`

 * *Files identical despite different names*

### Comparing `summa_embed-0.17.6/local_dependencies/summa-core/src/components/index_registry.rs` & `summa_embed-0.17.7/local_dependencies/summa-core/src/components/index_registry.rs`

 * *Files identical despite different names*

### Comparing `summa_embed-0.17.6/local_dependencies/summa-core/src/components/index_writer_holder.rs` & `summa_embed-0.17.7/local_dependencies/summa-core/src/components/index_writer_holder.rs`

 * *Files identical despite different names*

### Comparing `summa_embed-0.17.6/local_dependencies/summa-core/src/components/merge_policies/log_merge_policy.rs` & `summa_embed-0.17.7/local_dependencies/summa-core/src/components/merge_policies/log_merge_policy.rs`

 * *Files identical despite different names*

### Comparing `summa_embed-0.17.6/local_dependencies/summa-core/src/components/merge_policies/temporal_merge_policy.rs` & `summa_embed-0.17.7/local_dependencies/summa-core/src/components/merge_policies/temporal_merge_policy.rs`

 * *Files identical despite different names*

### Comparing `summa_embed-0.17.6/local_dependencies/summa-core/src/components/mod.rs` & `summa_embed-0.17.7/local_dependencies/summa-core/src/components/mod.rs`

 * *Files identical despite different names*

### Comparing `summa_embed-0.17.6/local_dependencies/summa-core/src/components/queries/exists_query.rs` & `summa_embed-0.17.7/local_dependencies/summa-core/src/components/queries/exists_query.rs`

 * *Files identical despite different names*

### Comparing `summa_embed-0.17.6/local_dependencies/summa-core/src/components/query_parser/morphology/english.rs` & `summa_embed-0.17.7/local_dependencies/summa-core/src/components/query_parser/morphology/english.rs`

 * *Files identical despite different names*

### Comparing `summa_embed-0.17.6/local_dependencies/summa-core/src/components/query_parser/morphology/manager.rs` & `summa_embed-0.17.7/local_dependencies/summa-core/src/components/query_parser/morphology/manager.rs`

 * *Files identical despite different names*

### Comparing `summa_embed-0.17.6/local_dependencies/summa-core/src/components/query_parser/morphology/mod.rs` & `summa_embed-0.17.7/local_dependencies/summa-core/src/components/query_parser/morphology/mod.rs`

 * *Files identical despite different names*

### Comparing `summa_embed-0.17.6/local_dependencies/summa-core/src/components/query_parser/proto_query_parser.rs` & `summa_embed-0.17.7/local_dependencies/summa-core/src/components/query_parser/proto_query_parser.rs`

 * *Files identical despite different names*

### Comparing `summa_embed-0.17.6/local_dependencies/summa-core/src/components/query_parser/summa_ql.pest` & `summa_embed-0.17.7/local_dependencies/summa-core/src/components/query_parser/summa_ql.pest`

 * *Files identical despite different names*

### Comparing `summa_embed-0.17.6/local_dependencies/summa-core/src/components/query_parser/summa_ql.rs` & `summa_embed-0.17.7/local_dependencies/summa-core/src/components/query_parser/summa_ql.rs`

 * *Files identical despite different names*

### Comparing `summa_embed-0.17.6/local_dependencies/summa-core/src/components/query_parser/term_field_mappers.rs` & `summa_embed-0.17.7/local_dependencies/summa-core/src/components/query_parser/term_field_mappers.rs`

 * *Files identical despite different names*

### Comparing `summa_embed-0.17.6/local_dependencies/summa-core/src/components/query_parser/utils.rs` & `summa_embed-0.17.7/local_dependencies/summa-core/src/components/query_parser/utils.rs`

 * *Files identical despite different names*

### Comparing `summa_embed-0.17.6/local_dependencies/summa-core/src/components/segment_attributes.rs` & `summa_embed-0.17.7/local_dependencies/summa-core/src/components/segment_attributes.rs`

 * *Files identical despite different names*

### Comparing `summa_embed-0.17.6/local_dependencies/summa-core/src/components/snippet_generator.rs` & `summa_embed-0.17.7/local_dependencies/summa-core/src/components/snippet_generator.rs`

 * *Files identical despite different names*

### Comparing `summa_embed-0.17.6/local_dependencies/summa-core/src/components/summa_document.rs` & `summa_embed-0.17.7/local_dependencies/summa-core/src/components/summa_document.rs`

 * *Files identical despite different names*

### Comparing `summa_embed-0.17.6/local_dependencies/summa-core/src/components/summa_tokenizer.rs` & `summa_embed-0.17.7/local_dependencies/summa-core/src/components/summa_tokenizer.rs`

 * *Files identical despite different names*

### Comparing `summa_embed-0.17.6/local_dependencies/summa-core/src/configs/config_proxy.rs` & `summa_embed-0.17.7/local_dependencies/summa-core/src/configs/config_proxy.rs`

 * *Files identical despite different names*

### Comparing `summa_embed-0.17.6/local_dependencies/summa-core/src/configs/core.rs` & `summa_embed-0.17.7/local_dependencies/summa-core/src/configs/core.rs`

 * *Files identical despite different names*

### Comparing `summa_embed-0.17.6/local_dependencies/summa-core/src/configs/file_proxy.rs` & `summa_embed-0.17.7/local_dependencies/summa-core/src/configs/file_proxy.rs`

 * *Files identical despite different names*

### Comparing `summa_embed-0.17.6/local_dependencies/summa-core/src/configs/partial_proxy.rs` & `summa_embed-0.17.7/local_dependencies/summa-core/src/configs/partial_proxy.rs`

 * *Files identical despite different names*

### Comparing `summa_embed-0.17.6/local_dependencies/summa-core/src/directories/byte_range_cache.rs` & `summa_embed-0.17.7/local_dependencies/summa-core/src/directories/byte_range_cache.rs`

 * *Files identical despite different names*

### Comparing `summa_embed-0.17.6/local_dependencies/summa-core/src/directories/caching_directory.rs` & `summa_embed-0.17.7/local_dependencies/summa-core/src/directories/caching_directory.rs`

 * *Files identical despite different names*

### Comparing `summa_embed-0.17.6/local_dependencies/summa-core/src/directories/debug_proxy_directory.rs` & `summa_embed-0.17.7/local_dependencies/summa-core/src/directories/debug_proxy_directory.rs`

 * *Files identical despite different names*

### Comparing `summa_embed-0.17.6/local_dependencies/summa-core/src/directories/external_requests.rs` & `summa_embed-0.17.7/local_dependencies/summa-core/src/directories/external_requests.rs`

 * *Files identical despite different names*

### Comparing `summa_embed-0.17.6/local_dependencies/summa-core/src/directories/hot_cache_directory.rs` & `summa_embed-0.17.7/local_dependencies/summa-core/src/directories/hot_cache_directory.rs`

 * *Files identical despite different names*

### Comparing `summa_embed-0.17.6/local_dependencies/summa-core/src/directories/mod.rs` & `summa_embed-0.17.7/local_dependencies/summa-core/src/directories/mod.rs`

 * *Files identical despite different names*

### Comparing `summa_embed-0.17.6/local_dependencies/summa-core/src/directories/network_directory.rs` & `summa_embed-0.17.7/local_dependencies/summa-core/src/directories/network_directory.rs`

 * *Files identical despite different names*

### Comparing `summa_embed-0.17.6/local_dependencies/summa-core/src/errors.rs` & `summa_embed-0.17.7/local_dependencies/summa-core/src/errors.rs`

 * *Files identical despite different names*

### Comparing `summa_embed-0.17.6/local_dependencies/summa-core/src/hyper_external_request.rs` & `summa_embed-0.17.7/local_dependencies/summa-core/src/hyper_external_request.rs`

 * *Files identical despite different names*

### Comparing `summa_embed-0.17.6/local_dependencies/summa-core/src/lib.rs` & `summa_embed-0.17.7/local_dependencies/summa-core/src/lib.rs`

 * *Files identical despite different names*

### Comparing `summa_embed-0.17.6/local_dependencies/summa-core/src/metrics/cache_metrics.rs` & `summa_embed-0.17.7/local_dependencies/summa-core/src/metrics/cache_metrics.rs`

 * *Files identical despite different names*

### Comparing `summa_embed-0.17.6/local_dependencies/summa-core/src/metrics/label.rs` & `summa_embed-0.17.7/local_dependencies/summa-core/src/metrics/label.rs`

 * *Files identical despite different names*

### Comparing `summa_embed-0.17.6/local_dependencies/summa-core/src/page_rank.rs` & `summa_embed-0.17.7/local_dependencies/summa-core/src/page_rank.rs`

 * *Files identical despite different names*

### Comparing `summa_embed-0.17.6/local_dependencies/summa-core/src/proto_traits/aggregation.rs` & `summa_embed-0.17.7/local_dependencies/summa-core/src/proto_traits/aggregation.rs`

 * *Files identical despite different names*

### Comparing `summa_embed-0.17.6/local_dependencies/summa-core/src/proto_traits/compression.rs` & `summa_embed-0.17.7/local_dependencies/summa-core/src/proto_traits/compression.rs`

 * *Files identical despite different names*

### Comparing `summa_embed-0.17.6/local_dependencies/summa-core/src/proto_traits/merge_policy.rs` & `summa_embed-0.17.7/local_dependencies/summa-core/src/proto_traits/merge_policy.rs`

 * *Files identical despite different names*

### Comparing `summa_embed-0.17.6/local_dependencies/summa-core/src/proto_traits/order.rs` & `summa_embed-0.17.7/local_dependencies/summa-core/src/proto_traits/order.rs`

 * *Files identical despite different names*

### Comparing `summa_embed-0.17.6/local_dependencies/summa-core/src/proto_traits/snippet.rs` & `summa_embed-0.17.7/local_dependencies/summa-core/src/proto_traits/snippet.rs`

 * *Files identical despite different names*

### Comparing `summa_embed-0.17.6/local_dependencies/summa-core/src/scorers/eval_scorer.rs` & `summa_embed-0.17.7/local_dependencies/summa-core/src/scorers/eval_scorer.rs`

 * *Files identical despite different names*

### Comparing `summa_embed-0.17.6/local_dependencies/summa-core/src/scorers/eval_scorer_tweaker.rs` & `summa_embed-0.17.7/local_dependencies/summa-core/src/scorers/eval_scorer_tweaker.rs`

 * *Files identical despite different names*

### Comparing `summa_embed-0.17.6/local_dependencies/summa-core/src/scorers/fast_field_iterator.rs` & `summa_embed-0.17.7/local_dependencies/summa-core/src/scorers/fast_field_iterator.rs`

 * *Files identical despite different names*

### Comparing `summa_embed-0.17.6/local_dependencies/summa-core/src/scorers/segment_eval_scorer.rs` & `summa_embed-0.17.7/local_dependencies/summa-core/src/scorers/segment_eval_scorer.rs`

 * *Files identical despite different names*

### Comparing `summa_embed-0.17.6/local_dependencies/summa-core/src/utils/sync.rs` & `summa_embed-0.17.7/local_dependencies/summa-core/src/utils/sync.rs`

 * *Files identical despite different names*

### Comparing `summa_embed-0.17.6/local_dependencies/summa-core/src/validators.rs` & `summa_embed-0.17.7/local_dependencies/summa-core/src/validators.rs`

 * *Files identical despite different names*

### Comparing `summa_embed-0.17.6/local_dependencies/summa-proto/Cargo.toml` & `summa_embed-0.17.7/local_dependencies/summa-proto/Cargo.toml`

 * *Files identical despite different names*

### Comparing `summa_embed-0.17.6/local_dependencies/summa-proto/LICENSE` & `summa_embed-0.17.7/local_dependencies/summa-server/LICENSE`

 * *Files identical despite different names*

### Comparing `summa_embed-0.17.6/local_dependencies/summa-proto/build.rs` & `summa_embed-0.17.7/local_dependencies/summa-proto/build.rs`

 * *Files identical despite different names*

### Comparing `summa_embed-0.17.6/local_dependencies/summa-proto/markdown.tmpl` & `summa_embed-0.17.7/local_dependencies/summa-proto/markdown.tmpl`

 * *Files identical despite different names*

### Comparing `summa_embed-0.17.6/local_dependencies/summa-proto/proto/consumer_service.proto` & `summa_embed-0.17.7/local_dependencies/summa-proto/proto/consumer_service.proto`

 * *Files identical despite different names*

### Comparing `summa_embed-0.17.6/local_dependencies/summa-proto/proto/index_service.proto` & `summa_embed-0.17.7/local_dependencies/summa-proto/proto/index_service.proto`

 * *Files identical despite different names*

### Comparing `summa_embed-0.17.6/local_dependencies/summa-proto/proto/query.proto` & `summa_embed-0.17.7/local_dependencies/summa-proto/proto/query.proto`

 * *Files identical despite different names*

### Comparing `summa_embed-0.17.6/local_dependencies/summa-proto/proto/search_service.proto` & `summa_embed-0.17.7/local_dependencies/summa-proto/proto/search_service.proto`

 * *Files identical despite different names*

### Comparing `summa_embed-0.17.6/local_dependencies/summa-proto/src/lib.rs` & `summa_embed-0.17.7/local_dependencies/summa-proto/src/lib.rs`

 * *Files identical despite different names*

### Comparing `summa_embed-0.17.6/local_dependencies/summa-proto/src/proto_traits/collector.rs` & `summa_embed-0.17.7/local_dependencies/summa-proto/src/proto_traits/collector.rs`

 * *Files identical despite different names*

### Comparing `summa_embed-0.17.6/local_dependencies/summa-proto/src/proto_traits/score.rs` & `summa_embed-0.17.7/local_dependencies/summa-proto/src/proto_traits/score.rs`

 * *Files identical despite different names*

### Comparing `summa_embed-0.17.6/Cargo.toml` & `summa_embed-0.17.7/Cargo.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [package]
 name = "summa-embed-py"
-version = "0.17.6"
+version = "0.17.7"
 edition = "2021"
 
 # See more keys and their definitions at https://doc.rust-lang.org/cargo/reference/manifest.html
 [lib]
 name = "summa_embed"
 crate-type = ["cdylib"]
 
@@ -13,12 +13,12 @@
 futures = "0.3"
 prost = "0.11"
 pyo3 = { version = "0.18", features = ["serde"] }
 pyo3-asyncio = { version =  "0.18", features = ["attributes", "tokio-runtime"] }
 pyo3-log = "0.8"
 pythonize = "0.18"
 serde_json = "1.0"
-summa-core = { version = "0.17.6", path = "local_dependencies/summa-core", default_features = false, features = ["fs", "hyper-external-request", "tokio-rt"] }
-summa-server = { version = "0.17.6", path = "local_dependencies/summa-server", default_features = false }
+summa-core = { version = "0.17.7", path = "local_dependencies/summa-core", default_features = false, features = ["fs", "hyper-external-request", "tokio-rt"] }
+summa-server = { version = "0.17.7", path = "local_dependencies/summa-server", default_features = false }
 summa-proto = { path = "local_dependencies/summa-proto" }
 tantivy = { git = "https://github.com/izihawa/tantivy", branch = "feature/summa", default_features = false, features = ["quickwit", "zstd-compression"] }
 tokio = { version = "1.25", default_features = false }
```

### Comparing `summa_embed-0.17.6/.gitignore` & `summa_embed-0.17.7/.gitignore`

 * *Files identical despite different names*

### Comparing `summa_embed-0.17.6/src/lib.rs` & `summa_embed-0.17.7/src/lib.rs`

 * *Files identical despite different names*

### Comparing `summa_embed-0.17.6/Cargo.lock` & `summa_embed-0.17.7/Cargo.lock`

 * *Files 1% similar despite different names*

```diff
@@ -144,17 +144,17 @@
 dependencies = [
  "event-listener",
  "futures-core",
 ]
 
 [[package]]
 name = "async-trait"
-version = "0.1.69"
+version = "0.1.70"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "7b2d0f03b3640e3a630367e40c468cb7f309529c708ed1d88597047b0e7c6ef7"
+checksum = "79fa67157abdfd688a259b6648808757db9347af834624f27ec646da976aee5d"
 dependencies = [
  "proc-macro2",
  "quote",
  "syn 2.0.23",
 ]
 
 [[package]]
@@ -754,25 +754,14 @@
  "serde_json",
  "summa-proto",
  "tokio",
  "tonic",
 ]
 
 [[package]]
-name = "fail"
-version = "0.5.1"
-source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "fe5e43d0f78a42ad591453aedb1d7ae631ce7ee445c7643691055a9ed8d3b01c"
-dependencies = [
- "log",
- "once_cell",
- "rand 0.8.5",
-]
-
-[[package]]
 name = "fastdivide"
 version = "0.4.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "25c7df09945d65ea8d70b3321547ed414bbc540aad5bac6883d021b970f35b04"
 
 [[package]]
 name = "fasteval2"
@@ -1108,17 +1097,17 @@
 name = "heck"
 version = "0.4.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "95505c38b4572b2d910cecb0281560f54b440a19336cbbcb27bf6ce6adc6f5a8"
 
 [[package]]
 name = "hermit-abi"
-version = "0.3.1"
+version = "0.3.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "fed44880c466736ef9a5c5b5facefb5ed0785676d0c02d612db14e54f0d84286"
+checksum = "443144c8cdadd93ebf52ddb4056d257f5b52c04d3c804e657d19eb73fc33668b"
 
 [[package]]
 name = "htmlescape"
 version = "0.3.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "e9025058dae765dee5070ec375f591e2ba14638c63feff74f13805a72e523163"
 
@@ -1328,17 +1317,17 @@
 checksum = "b0fd2260e829bddf4cb6ea802289de2f86d6a7a690192fbe91b3f46e0f2c8473"
 dependencies = [
  "either",
 ]
 
 [[package]]
 name = "itoa"
-version = "1.0.7"
+version = "1.0.8"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "c0aa48fab2893d8a49caa94082ae8488f4e1050d73b367881dcd2198f4199fd8"
+checksum = "62b02a5381cc465bd3041d84623d0fa3b66738b52b8e2fc3bab8ad63ab032f4a"
 
 [[package]]
 name = "izihawa-fst"
 version = "0.4.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "12ab646c8dd0c6ea3f36c02d4bd61773536509d822445aecf9c88362558c2244"
 dependencies = [
@@ -1601,17 +1590,17 @@
 name = "memchr"
 version = "2.5.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "2dffe52ecf27772e601905b7522cb4ef790d2cc203488bbd0e2fe85fcb74566d"
 
 [[package]]
 name = "memmap2"
-version = "0.6.2"
+version = "0.7.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "6d28bba84adfe6646737845bc5ebbfa2c08424eb1c37e94a1fd2a82adb56a872"
+checksum = "f49388d20533534cd19360ad3d6a7dadc885944aa802ba3995040c5ec11288c6"
 dependencies = [
  "libc",
 ]
 
 [[package]]
 name = "memoffset"
 version = "0.8.0"
@@ -1983,15 +1972,15 @@
 version = "0.1.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "b15813163c1d831bf4a13c3610c05c0d03b39feb07f7e09fa234dac9b15aaf39"
 
 [[package]]
 name = "ownedbytes"
 version = "0.5.0"
-source = "git+https://github.com/izihawa/tantivy?branch=feature/summa#af277119d67e178c2095640256be681dd47e0ad8"
+source = "git+https://github.com/izihawa/tantivy?branch=feature/summa#4d4561067efc6cb42ec29e7e8ede621a06f5a41f"
 dependencies = [
  "stable_deref_trait",
 ]
 
 [[package]]
 name = "parking_lot"
 version = "0.11.2"
@@ -2756,23 +2745,23 @@
  "libc",
  "linux-raw-sys 0.4.3",
  "windows-sys",
 ]
 
 [[package]]
 name = "rustversion"
-version = "1.0.12"
+version = "1.0.13"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "4f3208ce4d8448b3f3e7d168a73f5e0c43a61e32930de3bceeccedb388b6bf06"
+checksum = "dc31bd9b61a32c31f9650d18add92aa83a49ba979c143eefd27fe7177b05bd5f"
 
 [[package]]
 name = "ryu"
-version = "1.0.13"
+version = "1.0.14"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "f91339c0467de62360649f8d3e185ca8de4224ff281f66000de5eb2a77a79041"
+checksum = "fe232bdf6be8c8de797b22184ee71118d63780ea42ac85b61d1baa6d3b782ae9"
 
 [[package]]
 name = "schannel"
 version = "0.1.22"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "0c3733bf4cf7ea0880754e19cb5a462007c4a8c1914bff372ccc95b464f1df88"
 dependencies = [
@@ -2812,17 +2801,17 @@
 dependencies = [
  "core-foundation-sys",
  "libc",
 ]
 
 [[package]]
 name = "serde"
-version = "1.0.165"
+version = "1.0.166"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "c939f902bb7d0ccc5bce4f03297e161543c2dcb30914faf032c2bd0b7a0d48fc"
+checksum = "d01b7404f9d441d3ad40e6a636a7782c377d2abdbe4fa2440e2edcc2f4f10db8"
 dependencies = [
  "serde_derive",
 ]
 
 [[package]]
 name = "serde-wasm-bindgen"
 version = "0.5.0"
@@ -2832,17 +2821,17 @@
  "js-sys",
  "serde",
  "wasm-bindgen",
 ]
 
 [[package]]
 name = "serde_bytes"
-version = "0.11.9"
+version = "0.11.10"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "416bda436f9aab92e02c8e10d49a15ddd339cea90b6e340fe51ed97abb548294"
+checksum = "f3c5113243e4a3a1c96587342d067f3e6b0f50790b6cf40d2868eb647a3eef0e"
 dependencies = [
  "serde",
 ]
 
 [[package]]
 name = "serde_cbor"
 version = "0.11.2"
@@ -2851,28 +2840,28 @@
 dependencies = [
  "half",
  "serde",
 ]
 
 [[package]]
 name = "serde_derive"
-version = "1.0.165"
+version = "1.0.166"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "6eaae920e25fffe4019b75ff65e7660e72091e59dd204cb5849bbd6a3fd343d7"
+checksum = "5dd83d6dde2b6b2d466e14d9d1acce8816dedee94f735eac6395808b3483c6d6"
 dependencies = [
  "proc-macro2",
  "quote",
  "syn 2.0.23",
 ]
 
 [[package]]
 name = "serde_json"
-version = "1.0.99"
+version = "1.0.100"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "46266871c240a00b8f503b877622fe33430b3c7d963bdc0f2adc511e54a1eae3"
+checksum = "0f1e14e89be7aa4c4b78bdbdc9eb5bf8517829a600ae8eaa39a6e1d960b5185c"
 dependencies = [
  "itoa",
  "ryu",
  "serde",
 ]
 
 [[package]]
@@ -3013,15 +3002,15 @@
 name = "strsim"
 version = "0.10.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "73473c0e59e6d5812c5dfe2a064a6444949f089e20eec9a2e5506596494e4623"
 
 [[package]]
 name = "summa-core"
-version = "0.17.6"
+version = "0.17.7"
 dependencies = [
  "anyhow",
  "async-trait",
  "base64 0.21.2",
  "bytes",
  "chrono",
  "config",
@@ -3061,15 +3050,15 @@
  "time 0.3.22",
  "tokio",
  "tracing",
 ]
 
 [[package]]
 name = "summa-embed-py"
-version = "0.17.6"
+version = "0.17.7"
 dependencies = [
  "async-broadcast",
  "futures",
  "prost",
  "pyo3",
  "pyo3-asyncio",
  "pyo3-log",
@@ -3095,15 +3084,15 @@
  "tonic",
  "tonic-build",
  "tonic-reflection",
 ]
 
 [[package]]
 name = "summa-server"
-version = "0.17.6"
+version = "0.17.7"
 dependencies = [
  "anyhow",
  "async-broadcast",
  "async-trait",
  "clap",
  "config",
  "derive_builder",
@@ -3222,27 +3211,26 @@
 version = "0.2.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "f764005d11ee5f36500a149ace24e00e3da98b0158b3e2d53a7495660d3f4d60"
 
 [[package]]
 name = "tantivy"
 version = "0.20.2"
-source = "git+https://github.com/izihawa/tantivy?branch=feature/summa#af277119d67e178c2095640256be681dd47e0ad8"
+source = "git+https://github.com/izihawa/tantivy?branch=feature/summa#4d4561067efc6cb42ec29e7e8ede621a06f5a41f"
 dependencies = [
  "aho-corasick",
  "arc-swap",
  "async-trait",
  "base64 0.21.2",
  "bitpacking",
  "byteorder",
  "census",
  "crc32fast",
  "crossbeam-channel",
  "downcast-rs",
- "fail",
  "fastdivide",
  "fs4",
  "futures",
  "futures-util",
  "htmlescape",
  "itertools",
  "izihawa-fst",
@@ -3279,38 +3267,38 @@
  "winapi",
  "zstd",
 ]
 
 [[package]]
 name = "tantivy-bitpacker"
 version = "0.4.0"
-source = "git+https://github.com/izihawa/tantivy?branch=feature/summa#af277119d67e178c2095640256be681dd47e0ad8"
+source = "git+https://github.com/izihawa/tantivy?branch=feature/summa#4d4561067efc6cb42ec29e7e8ede621a06f5a41f"
 dependencies = [
  "bitpacking",
 ]
 
 [[package]]
 name = "tantivy-columnar"
 version = "0.1.0"
-source = "git+https://github.com/izihawa/tantivy?branch=feature/summa#af277119d67e178c2095640256be681dd47e0ad8"
+source = "git+https://github.com/izihawa/tantivy?branch=feature/summa#4d4561067efc6cb42ec29e7e8ede621a06f5a41f"
 dependencies = [
  "fastdivide",
  "fnv",
  "itertools",
  "serde",
  "tantivy-bitpacker",
  "tantivy-common",
  "tantivy-sstable",
  "tantivy-stacker",
 ]
 
 [[package]]
 name = "tantivy-common"
 version = "0.5.0"
-source = "git+https://github.com/izihawa/tantivy?branch=feature/summa#af277119d67e178c2095640256be681dd47e0ad8"
+source = "git+https://github.com/izihawa/tantivy?branch=feature/summa#4d4561067efc6cb42ec29e7e8ede621a06f5a41f"
 dependencies = [
  "async-trait",
  "byteorder",
  "ownedbytes",
  "serde",
  "time 0.3.22",
 ]
@@ -3325,44 +3313,44 @@
  "regex-syntax 0.6.29",
  "utf8-ranges",
 ]
 
 [[package]]
 name = "tantivy-query-grammar"
 version = "0.20.0"
-source = "git+https://github.com/izihawa/tantivy?branch=feature/summa#af277119d67e178c2095640256be681dd47e0ad8"
+source = "git+https://github.com/izihawa/tantivy?branch=feature/summa#4d4561067efc6cb42ec29e7e8ede621a06f5a41f"
 dependencies = [
  "combine",
  "once_cell",
  "regex",
 ]
 
 [[package]]
 name = "tantivy-sstable"
 version = "0.1.0"
-source = "git+https://github.com/izihawa/tantivy?branch=feature/summa#af277119d67e178c2095640256be681dd47e0ad8"
+source = "git+https://github.com/izihawa/tantivy?branch=feature/summa#4d4561067efc6cb42ec29e7e8ede621a06f5a41f"
 dependencies = [
  "izihawa-fst",
  "tantivy-common",
  "zstd",
 ]
 
 [[package]]
 name = "tantivy-stacker"
 version = "0.1.0"
-source = "git+https://github.com/izihawa/tantivy?branch=feature/summa#af277119d67e178c2095640256be681dd47e0ad8"
+source = "git+https://github.com/izihawa/tantivy?branch=feature/summa#4d4561067efc6cb42ec29e7e8ede621a06f5a41f"
 dependencies = [
  "murmurhash32",
  "tantivy-common",
 ]
 
 [[package]]
 name = "tantivy-tokenizer-api"
 version = "0.1.0"
-source = "git+https://github.com/izihawa/tantivy?branch=feature/summa#af277119d67e178c2095640256be681dd47e0ad8"
+source = "git+https://github.com/izihawa/tantivy?branch=feature/summa#4d4561067efc6cb42ec29e7e8ede621a06f5a41f"
 dependencies = [
  "serde",
 ]
 
 [[package]]
 name = "tap"
 version = "1.0.1"
@@ -3397,26 +3385,26 @@
  "redox_syscall 0.3.5",
  "rustix 0.37.22",
  "windows-sys",
 ]
 
 [[package]]
 name = "thiserror"
-version = "1.0.40"
+version = "1.0.41"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "978c9a314bd8dc99be594bc3c175faaa9794be04a5a5e153caba6915336cebac"
+checksum = "c16a64ba9387ef3fdae4f9c1a7f07a0997fce91985c0336f1ddc1822b3b37802"
 dependencies = [
  "thiserror-impl",
 ]
 
 [[package]]
 name = "thiserror-impl"
-version = "1.0.40"
+version = "1.0.41"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "f9456a42c5b0d803c8cd86e73dd7cc9edd429499f37a3550d286d5e86720569f"
+checksum = "d14928354b01c4d6a4f0e549069adef399a284e7995c7ccca94e8a07a5346c59"
 dependencies = [
  "proc-macro2",
  "quote",
  "syn 2.0.23",
 ]
 
 [[package]]
@@ -3824,17 +3812,17 @@
 name = "ucd-trie"
 version = "0.1.5"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "9e79c4d996edb816c91e4308506774452e55e95c3c9de07b6729e17e15a5ef81"
 
 [[package]]
 name = "unicode-ident"
-version = "1.0.9"
+version = "1.0.10"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "b15811caf2415fb889178633e7724bad2509101cde276048e013b9def5e51fa0"
+checksum = "22049a19f4a68748a168c0fc439f9516686aa045927ff767eca0a85101fb6e73"
 
 [[package]]
 name = "unicode-segmentation"
 version = "1.10.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "1dd624098567895118886609431a7c3b8f516e41d30e0643f03d94592a147e36"
```

