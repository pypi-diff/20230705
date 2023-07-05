# Comparing `tmp/bi_etl-1.4.2.tar.gz` & `tmp/bi_etl-1.4.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bi_etl-1.4.2.tar", max compression
+gzip compressed data, was "bi_etl-1.4.3.tar", max compression
```

## Comparing `bi_etl-1.4.2.tar` & `bi_etl-1.4.3.tar`

### file list

```diff
@@ -1,131 +1,131 @@
--rw-r--r--   0        0        0      628 2021-09-27 17:13:33.000000 bi_etl-1.4.2/bi_etl/.coveragerc
--rw-r--r--   0        0        0      360 2021-09-27 17:13:33.000000 bi_etl-1.4.2/bi_etl/.project
--rw-r--r--   0        0        0      423 2021-09-27 17:13:33.000000 bi_etl-1.4.2/bi_etl/.pydevproject
--rw-r--r--   0        0        0     3529 2021-09-27 17:13:33.000000 bi_etl-1.4.2/bi_etl/.pylintrc
--rw-r--r--   0        0        0      104 2022-07-21 13:01:16.000000 bi_etl-1.4.2/bi_etl/__init__.py
--rw-r--r--   0        0        0     2612 2022-07-21 13:01:16.000000 bi_etl-1.4.2/bi_etl/__main__.py
--rw-r--r--   0        0        0       61 2022-07-21 13:01:16.000000 bi_etl-1.4.2/bi_etl/boto3_helper/__init__.py
--rw-r--r--   0        0        0     1664 2022-07-21 13:01:16.000000 bi_etl-1.4.2/bi_etl/boto3_helper/dynamodb.py
--rw-r--r--   0        0        0      148 2022-07-21 13:01:16.000000 bi_etl-1.4.2/bi_etl/boto3_helper/lambdas.py
--rw-r--r--   0        0        0    12181 2022-08-11 15:34:45.000000 bi_etl-1.4.2/bi_etl/boto3_helper/s3.py
--rw-r--r--   0        0        0     1905 2022-07-21 13:01:16.000000 bi_etl-1.4.2/bi_etl/boto3_helper/session.py
--rw-r--r--   0        0        0      142 2022-07-21 13:01:16.000000 bi_etl-1.4.2/bi_etl/boto3_helper/ssm.py
--rw-r--r--   0        0        0        0 2021-09-27 17:13:33.000000 bi_etl-1.4.2/bi_etl/bulk_loaders/__init__.py
--rw-r--r--   0        0        0     6756 2023-03-15 15:53:33.483857 bi_etl-1.4.2/bi_etl/bulk_loaders/bulk_loader.py
--rw-r--r--   0        0        0      982 2021-09-27 17:13:33.000000 bi_etl-1.4.2/bi_etl/bulk_loaders/bulk_loader_exception.py
--rw-r--r--   0        0        0      323 2022-10-06 20:54:25.000000 bi_etl-1.4.2/bi_etl/bulk_loaders/postgresql_bulk_load_config.py
--rw-r--r--   0        0        0     3759 2023-01-18 17:48:19.693841 bi_etl-1.4.2/bi_etl/bulk_loaders/postgresql_copy.py
--rw-r--r--   0        0        0     6299 2023-01-18 17:48:19.786858 bi_etl-1.4.2/bi_etl/bulk_loaders/redshift_s3_avro_loader.py
--rw-r--r--   0        0        0    14049 2023-03-23 20:50:09.146143 bi_etl-1.4.2/bi_etl/bulk_loaders/redshift_s3_base.py
--rw-r--r--   0        0        0    11775 2023-01-18 17:48:19.808886 bi_etl-1.4.2/bi_etl/bulk_loaders/redshift_s3_csv_loader.py
--rw-r--r--   0        0        0     4081 2023-01-18 17:48:19.827968 bi_etl-1.4.2/bi_etl/bulk_loaders/redshift_s3_json_loader.py
--rw-r--r--   0        0        0     6335 2023-01-18 17:48:19.714844 bi_etl-1.4.2/bi_etl/bulk_loaders/redshift_s3_parquet_loader.py
--rw-r--r--   0        0        0     1063 2023-01-10 02:14:59.086394 bi_etl-1.4.2/bi_etl/bulk_loaders/s3_bulk_load_config.py
--rw-r--r--   0        0        0     4821 2023-01-18 17:48:19.735841 bi_etl-1.4.2/bi_etl/bulk_loaders/sql_server_bcp.py
--rw-r--r--   0        0        0        0 2021-09-27 17:13:33.000000 bi_etl-1.4.2/bi_etl/components/__init__.py
--rw-r--r--   0        0        0    16109 2022-10-06 21:12:48.000000 bi_etl-1.4.2/bi_etl/components/csv_writer.py
--rw-r--r--   0        0        0    17630 2022-08-24 15:21:41.000000 bi_etl-1.4.2/bi_etl/components/csvreader.py
--rw-r--r--   0        0        0    19384 2022-07-21 13:01:16.000000 bi_etl-1.4.2/bi_etl/components/data_analyzer.py
--rw-r--r--   0        0        0    52067 2022-10-31 19:45:21.367328 bi_etl-1.4.2/bi_etl/components/etlcomponent.py
--rw-r--r--   0        0        0       61 2021-09-27 17:13:33.000000 bi_etl-1.4.2/bi_etl/components/get_next_key/__init__.py
--rw-r--r--   0        0        0      873 2022-05-04 02:21:27.000000 bi_etl-1.4.2/bi_etl/components/get_next_key/base_table_memory.py
--rw-r--r--   0        0        0      644 2021-09-27 17:13:33.000000 bi_etl-1.4.2/bi_etl/components/get_next_key/local_table_memory.py
--rw-r--r--   0        0        0     2047 2022-06-06 16:22:38.000000 bi_etl-1.4.2/bi_etl/components/get_next_key/shared_table_memory.py
--rw-r--r--   0        0        0      708 2021-09-27 17:13:33.000000 bi_etl-1.4.2/bi_etl/components/get_next_key/shared_table_memory_manager.py
--rw-r--r--   0        0        0   107458 2023-03-15 15:33:34.268035 bi_etl-1.4.2/bi_etl/components/hst_table.py
--rw-r--r--   0        0        0    42645 2023-03-15 15:53:33.397385 bi_etl-1.4.2/bi_etl/components/hst_table_source_based.py
--rw-r--r--   0        0        0    57029 2023-03-15 15:33:34.192481 bi_etl-1.4.2/bi_etl/components/readonlytable.py
--rw-r--r--   0        0        0       54 2021-09-27 17:13:33.000000 bi_etl-1.4.2/bi_etl/components/row/__init__.py
--rw-r--r--   0        0        0      456 2022-07-21 13:01:16.000000 bi_etl-1.4.2/bi_etl/components/row/cached_frozenset.py
--rw-r--r--   0        0        0      564 2022-07-21 13:01:16.000000 bi_etl-1.4.2/bi_etl/components/row/column_difference.py
--rw-r--r--   0        0        0    32775 2022-10-06 21:20:46.000000 bi_etl-1.4.2/bi_etl/components/row/row.py
--rw-r--r--   0        0        0     1661 2022-07-21 13:01:16.000000 bi_etl-1.4.2/bi_etl/components/row/row_case_insensitive.py
--rw-r--r--   0        0        0    25341 2023-03-15 15:32:32.540669 bi_etl-1.4.2/bi_etl/components/row/row_iteration_header.py
--rw-r--r--   0        0        0     4220 2022-07-21 13:01:16.000000 bi_etl-1.4.2/bi_etl/components/row/row_iteration_header_case_insensitive.py
--rw-r--r--   0        0        0      293 2022-07-21 13:01:16.000000 bi_etl-1.4.2/bi_etl/components/row/row_status.py
--rw-r--r--   0        0        0     3165 2022-07-21 13:01:16.000000 bi_etl-1.4.2/bi_etl/components/sqlquery.py
--rw-r--r--   0        0        0   164231 2023-03-15 15:33:43.015659 bi_etl-1.4.2/bi_etl/components/table.py
--rw-r--r--   0        0        0     8365 2022-07-21 13:01:16.000000 bi_etl-1.4.2/bi_etl/components/w3c_reader.py
--rw-r--r--   0        0        0     9820 2023-01-25 16:23:05.105369 bi_etl-1.4.2/bi_etl/components/xlsx_reader.py
--rw-r--r--   0        0        0    12007 2022-08-30 16:22:27.000000 bi_etl-1.4.2/bi_etl/components/xlsx_writer.py
--rw-r--r--   0        0        0        0 2022-07-21 13:01:16.000000 bi_etl-1.4.2/bi_etl/config/__init__.py
--rw-r--r--   0        0        0     1780 2022-07-21 13:01:16.000000 bi_etl-1.4.2/bi_etl/config/bi_etl_config_base.py
--rw-r--r--   0        0        0     3025 2023-03-15 15:33:34.244760 bi_etl-1.4.2/bi_etl/config/notifiers_config.py
--rw-r--r--   0        0        0      328 2022-07-21 13:01:16.000000 bi_etl-1.4.2/bi_etl/config/scheduler_config.py
--rw-r--r--   0        0        0    14301 2022-09-06 16:31:27.000000 bi_etl-1.4.2/bi_etl/conversions.py
--rw-r--r--   0        0        0      133 2021-09-27 17:13:34.000000 bi_etl-1.4.2/bi_etl/database/__init__.py
--rw-r--r--   0        0        0    17838 2023-03-21 14:17:46.169530 bi_etl-1.4.2/bi_etl/database/database_metadata.py
--rw-r--r--   0        0        0     1045 2022-07-21 13:01:16.000000 bi_etl-1.4.2/bi_etl/database/mock_database_metadata.py
--rw-r--r--   0        0        0     5699 2022-08-30 16:22:27.000000 bi_etl-1.4.2/bi_etl/example_config.ini
--rw-r--r--   0        0        0     5490 2022-08-30 16:22:27.000000 bi_etl-1.4.2/bi_etl/example_config_shared.ini
--rw-r--r--   0        0        0      923 2021-09-27 17:13:34.000000 bi_etl-1.4.2/bi_etl/exceptions/__init__.py
--rw-r--r--   0        0        0        0 2021-09-27 17:13:34.000000 bi_etl-1.4.2/bi_etl/informatica/__init__.py
--rw-r--r--   0        0        0       89 2022-07-21 13:01:17.000000 bi_etl-1.4.2/bi_etl/informatica/exceptions.py
--rw-r--r--   0        0        0      493 2022-07-21 13:01:17.000000 bi_etl-1.4.2/bi_etl/informatica/pm_config.py
--rw-r--r--   0        0        0     7540 2022-07-21 13:01:17.000000 bi_etl-1.4.2/bi_etl/informatica/pmcmd.py
--rw-r--r--   0        0        0     1219 2022-07-21 13:01:17.000000 bi_etl-1.4.2/bi_etl/informatica/pmcmd_task.py
--rw-r--r--   0        0        0    18054 2022-07-21 13:01:17.000000 bi_etl-1.4.2/bi_etl/informatica/pmrep.py
--rw-r--r--   0        0        0        0 2021-09-27 17:13:34.000000 bi_etl-1.4.2/bi_etl/lookups/__init__.py
--rw-r--r--   0        0        0    14159 2022-10-28 13:41:10.698113 bi_etl-1.4.2/bi_etl/lookups/autodisk_lookup.py
--rw-r--r--   0        0        0     3965 2022-07-21 13:01:17.000000 bi_etl-1.4.2/bi_etl/lookups/autodisk_range_lookup.py
--rw-r--r--   0        0        0     4699 2023-01-18 17:48:19.675169 bi_etl-1.4.2/bi_etl/lookups/disk_lookup.py
--rw-r--r--   0        0        0     1934 2022-07-21 13:01:17.000000 bi_etl-1.4.2/bi_etl/lookups/disk_range_lookup.py
--rw-r--r--   0        0        0    28901 2022-07-21 13:01:17.000000 bi_etl-1.4.2/bi_etl/lookups/lookup.py
--rw-r--r--   0        0        0     9926 2022-07-21 13:01:17.000000 bi_etl-1.4.2/bi_etl/lookups/non_unique_lookup.py
--rw-r--r--   0        0        0    12839 2022-07-21 13:01:17.000000 bi_etl-1.4.2/bi_etl/lookups/range_lookup.py
--rw-r--r--   0        0        0     3358 2022-07-21 13:01:17.000000 bi_etl-1.4.2/bi_etl/memory_size.py
--rw-r--r--   0        0        0      308 2022-07-21 13:01:17.000000 bi_etl-1.4.2/bi_etl/notifiers/__init__.py
--rw-r--r--   0        0        0     4323 2022-07-21 13:01:17.000000 bi_etl-1.4.2/bi_etl/notifiers/email.py
--rw-r--r--   0        0        0     8451 2022-07-21 20:01:17.000000 bi_etl-1.4.2/bi_etl/notifiers/jira.py
--rw-r--r--   0        0        0      379 2022-07-21 13:01:17.000000 bi_etl-1.4.2/bi_etl/notifiers/log_notifier.py
--rw-r--r--   0        0        0      706 2023-03-15 16:37:38.935207 bi_etl-1.4.2/bi_etl/notifiers/notifier_base.py
--rw-r--r--   0        0        0     6398 2023-03-15 16:37:38.986969 bi_etl-1.4.2/bi_etl/notifiers/slack.py
--rw-r--r--   0        0        0       61 2021-09-27 17:13:34.000000 bi_etl-1.4.2/bi_etl/parallel/__init__.py
--rw-r--r--   0        0        0        1 2022-07-21 13:01:17.000000 bi_etl-1.4.2/bi_etl/parallel/mp.py
--rw-r--r--   0        0        0        0 2021-09-27 17:13:34.000000 bi_etl-1.4.2/bi_etl/parameters/__init__.py
--rw-r--r--   0        0        0      956 2021-09-27 17:13:34.000000 bi_etl-1.4.2/bi_etl/parameters/file_parameter.py
--rw-r--r--   0        0        0       61 2021-09-27 17:13:34.000000 bi_etl-1.4.2/bi_etl/performance_test/__init__.py
--rw-r--r--   0        0        0     1071 2022-07-21 13:01:17.000000 bi_etl-1.4.2/bi_etl/performance_test/perftest_static_reader.py
--rw-r--r--   0        0        0        0 2021-09-27 17:13:34.000000 bi_etl-1.4.2/bi_etl/scheduler/__init__.py
--rw-r--r--   0        0        0     1737 2022-10-06 21:20:46.000000 bi_etl-1.4.2/bi_etl/scheduler/dependent_reasons.py
--rw-r--r--   0        0        0      706 2021-09-27 17:13:34.000000 bi_etl-1.4.2/bi_etl/scheduler/exceptions.py
--rw-r--r--   0        0        0     1853 2021-09-27 17:13:34.000000 bi_etl-1.4.2/bi_etl/scheduler/messages.py
--rw-r--r--   0        0        0    10430 2022-07-21 13:01:17.000000 bi_etl-1.4.2/bi_etl/scheduler/models.py
--rw-r--r--   0        0        0      672 2022-07-21 13:01:17.000000 bi_etl-1.4.2/bi_etl/scheduler/queue_io.py
--rw-r--r--   0        0        0      116 2021-09-27 17:13:34.000000 bi_etl-1.4.2/bi_etl/scheduler/run_scheduler.sh
--rw-r--r--   0        0        0      391 2021-09-27 17:13:34.000000 bi_etl-1.4.2/bi_etl/scheduler/run_scheduler_screen.sh
--rw-r--r--   0        0        0    65309 2022-10-06 21:20:46.000000 bi_etl-1.4.2/bi_etl/scheduler/scheduler.py
--rw-r--r--   0        0        0        0 2021-09-27 17:13:34.000000 bi_etl-1.4.2/bi_etl/scheduler/scheduler_etl_jobs/__init__.py
--rw-r--r--   0        0        0     2659 2022-07-21 13:01:17.000000 bi_etl-1.4.2/bi_etl/scheduler/scheduler_etl_jobs/etl_task_status_cd.py
--rw-r--r--   0        0        0    28623 2022-07-21 13:01:17.000000 bi_etl-1.4.2/bi_etl/scheduler/scheduler_interface.py
--rw-r--r--   0        0        0      444 2021-09-27 17:13:34.000000 bi_etl-1.4.2/bi_etl/scheduler/sdtout_queue.py
--rw-r--r--   0        0        0      688 2022-07-21 13:01:17.000000 bi_etl-1.4.2/bi_etl/scheduler/special_tasks.py
--rw-r--r--   0        0        0     2801 2022-07-21 13:01:17.000000 bi_etl-1.4.2/bi_etl/scheduler/status.py
--rw-r--r--   0        0        0    57835 2023-06-27 14:21:39.760133 bi_etl-1.4.2/bi_etl/scheduler/task.py
--rw-r--r--   0        0        0     7377 2022-10-31 20:23:08.644384 bi_etl-1.4.2/bi_etl/statement_queue.py
--rw-r--r--   0        0        0     6742 2022-07-21 13:01:17.000000 bi_etl-1.4.2/bi_etl/statistics.py
--rw-r--r--   0        0        0       61 2021-09-27 17:13:34.000000 bi_etl-1.4.2/bi_etl/test_notebooks/__init__.py
--rw-r--r--   0        0        0     1073 2022-06-09 14:18:34.000000 bi_etl-1.4.2/bi_etl/test_notebooks/perftest_static_reader.py
--rw-r--r--   0        0        0    17122 2022-05-12 15:44:59.000000 bi_etl-1.4.2/bi_etl/test_notebooks/Row performance.ipynb
--rw-r--r--   0        0        0     3509 2022-05-12 15:44:59.000000 bi_etl-1.4.2/bi_etl/test_notebooks/Utility Test.ipynb
--rw-r--r--   0        0        0     4343 2021-09-27 17:13:34.000000 bi_etl-1.4.2/bi_etl/timer.py
--rw-r--r--   0        0        0    11366 2022-07-21 13:01:17.000000 bi_etl-1.4.2/bi_etl/utility/__init__.py
--rw-r--r--   0        0        0     2118 2022-07-21 13:01:17.000000 bi_etl-1.4.2/bi_etl/utility/ask.py
--rw-r--r--   0        0        0     8976 2023-01-18 17:48:19.758841 bi_etl-1.4.2/bi_etl/utility/bcp_helpers.py
--rw-r--r--   0        0        0      925 2021-09-27 17:13:34.000000 bi_etl-1.4.2/bi_etl/utility/case_insentive_set.py
--rw-r--r--   0        0        0     1869 2022-07-21 13:01:17.000000 bi_etl-1.4.2/bi_etl/utility/copy_table_data.py
--rw-r--r--   0        0        0     5000 2022-07-21 13:01:17.000000 bi_etl-1.4.2/bi_etl/utility/line_counter.py
--rw-r--r--   0        0        0      472 2021-09-27 17:13:34.000000 bi_etl-1.4.2/bi_etl/utility/logging_helpers.py
--rw-r--r--   0        0        0      947 2022-07-21 13:01:17.000000 bi_etl-1.4.2/bi_etl/utility/package_root.py
--rw-r--r--   0        0        0       61 2021-09-27 17:13:34.000000 bi_etl-1.4.2/bi_etl/utility/postgresql/__init__.py
--rw-r--r--   0        0        0     3686 2023-01-18 17:48:19.844889 bi_etl-1.4.2/bi_etl/utility/postgresql/psql_command.py
--rw-r--r--   0        0        0     4777 2022-10-06 20:52:27.000000 bi_etl-1.4.2/bi_etl/utility/postgresql/psycopg2_helpers.py
--rw-r--r--   0        0        0    11998 2023-03-15 15:33:34.410960 bi_etl-1.4.2/bi_etl/utility/run_sql_script.py
--rw-r--r--   0        0        0       61 2021-09-27 17:13:34.000000 bi_etl-1.4.2/bi_etl/utility/sql_server/__init__.py
--rw-r--r--   0        0        0     2776 2023-06-27 14:01:47.122835 bi_etl-1.4.2/bi_etl/utility/sql_server/defrag_indexes.py
--rw-r--r--   0        0        0     4674 2022-07-21 13:01:17.000000 bi_etl-1.4.2/bi_etl/utility/ssh_forward.py
--rw-r--r--   0        0        0      341 2022-07-21 13:01:17.000000 bi_etl-1.4.2/bi_etl/version.py
--rw-r--r--   0        0        0     1086 2020-06-29 20:22:28.000000 bi_etl-1.4.2/license.txt
--rw-r--r--   0        0        0     2009 2023-07-05 15:24:56.841691 bi_etl-1.4.2/pyproject.toml
--rw-r--r--   0        0        0     1251 2022-10-06 21:20:46.000000 bi_etl-1.4.2/README.md
--rw-r--r--   0        0        0     2975 1970-01-01 00:00:00.000000 bi_etl-1.4.2/PKG-INFO
+-rw-r--r--   0        0        0      628 2021-09-27 17:13:33.000000 bi_etl-1.4.3/bi_etl/.coveragerc
+-rw-r--r--   0        0        0      360 2021-09-27 17:13:33.000000 bi_etl-1.4.3/bi_etl/.project
+-rw-r--r--   0        0        0      423 2021-09-27 17:13:33.000000 bi_etl-1.4.3/bi_etl/.pydevproject
+-rw-r--r--   0        0        0     3529 2021-09-27 17:13:33.000000 bi_etl-1.4.3/bi_etl/.pylintrc
+-rw-r--r--   0        0        0      104 2022-07-21 13:01:16.000000 bi_etl-1.4.3/bi_etl/__init__.py
+-rw-r--r--   0        0        0     2612 2022-07-21 13:01:16.000000 bi_etl-1.4.3/bi_etl/__main__.py
+-rw-r--r--   0        0        0       61 2022-07-21 13:01:16.000000 bi_etl-1.4.3/bi_etl/boto3_helper/__init__.py
+-rw-r--r--   0        0        0     1664 2022-07-21 13:01:16.000000 bi_etl-1.4.3/bi_etl/boto3_helper/dynamodb.py
+-rw-r--r--   0        0        0      148 2022-07-21 13:01:16.000000 bi_etl-1.4.3/bi_etl/boto3_helper/lambdas.py
+-rw-r--r--   0        0        0    12181 2022-08-11 15:34:45.000000 bi_etl-1.4.3/bi_etl/boto3_helper/s3.py
+-rw-r--r--   0        0        0     1905 2022-07-21 13:01:16.000000 bi_etl-1.4.3/bi_etl/boto3_helper/session.py
+-rw-r--r--   0        0        0      142 2022-07-21 13:01:16.000000 bi_etl-1.4.3/bi_etl/boto3_helper/ssm.py
+-rw-r--r--   0        0        0        0 2021-09-27 17:13:33.000000 bi_etl-1.4.3/bi_etl/bulk_loaders/__init__.py
+-rw-r--r--   0        0        0     6756 2023-03-15 15:53:33.483857 bi_etl-1.4.3/bi_etl/bulk_loaders/bulk_loader.py
+-rw-r--r--   0        0        0      982 2021-09-27 17:13:33.000000 bi_etl-1.4.3/bi_etl/bulk_loaders/bulk_loader_exception.py
+-rw-r--r--   0        0        0      323 2022-10-06 20:54:25.000000 bi_etl-1.4.3/bi_etl/bulk_loaders/postgresql_bulk_load_config.py
+-rw-r--r--   0        0        0     3759 2023-01-18 17:48:19.693841 bi_etl-1.4.3/bi_etl/bulk_loaders/postgresql_copy.py
+-rw-r--r--   0        0        0     6299 2023-07-05 15:52:48.202294 bi_etl-1.4.3/bi_etl/bulk_loaders/redshift_s3_avro_loader.py
+-rw-r--r--   0        0        0    14675 2023-07-05 16:48:36.150907 bi_etl-1.4.3/bi_etl/bulk_loaders/redshift_s3_base.py
+-rw-r--r--   0        0        0    11775 2023-07-05 15:52:56.457815 bi_etl-1.4.3/bi_etl/bulk_loaders/redshift_s3_csv_loader.py
+-rw-r--r--   0        0        0     4081 2023-07-05 15:53:00.027111 bi_etl-1.4.3/bi_etl/bulk_loaders/redshift_s3_json_loader.py
+-rw-r--r--   0        0        0     6335 2023-07-05 15:53:04.881027 bi_etl-1.4.3/bi_etl/bulk_loaders/redshift_s3_parquet_loader.py
+-rw-r--r--   0        0        0     1063 2023-01-10 02:14:59.086394 bi_etl-1.4.3/bi_etl/bulk_loaders/s3_bulk_load_config.py
+-rw-r--r--   0        0        0     4821 2023-01-18 17:48:19.735841 bi_etl-1.4.3/bi_etl/bulk_loaders/sql_server_bcp.py
+-rw-r--r--   0        0        0        0 2021-09-27 17:13:33.000000 bi_etl-1.4.3/bi_etl/components/__init__.py
+-rw-r--r--   0        0        0    16109 2022-10-06 21:12:48.000000 bi_etl-1.4.3/bi_etl/components/csv_writer.py
+-rw-r--r--   0        0        0    17630 2022-08-24 15:21:41.000000 bi_etl-1.4.3/bi_etl/components/csvreader.py
+-rw-r--r--   0        0        0    19384 2022-07-21 13:01:16.000000 bi_etl-1.4.3/bi_etl/components/data_analyzer.py
+-rw-r--r--   0        0        0    52067 2022-10-31 19:45:21.367328 bi_etl-1.4.3/bi_etl/components/etlcomponent.py
+-rw-r--r--   0        0        0       61 2021-09-27 17:13:33.000000 bi_etl-1.4.3/bi_etl/components/get_next_key/__init__.py
+-rw-r--r--   0        0        0      873 2022-05-04 02:21:27.000000 bi_etl-1.4.3/bi_etl/components/get_next_key/base_table_memory.py
+-rw-r--r--   0        0        0      644 2021-09-27 17:13:33.000000 bi_etl-1.4.3/bi_etl/components/get_next_key/local_table_memory.py
+-rw-r--r--   0        0        0     2047 2022-06-06 16:22:38.000000 bi_etl-1.4.3/bi_etl/components/get_next_key/shared_table_memory.py
+-rw-r--r--   0        0        0      708 2021-09-27 17:13:33.000000 bi_etl-1.4.3/bi_etl/components/get_next_key/shared_table_memory_manager.py
+-rw-r--r--   0        0        0   107458 2023-03-15 15:33:34.268035 bi_etl-1.4.3/bi_etl/components/hst_table.py
+-rw-r--r--   0        0        0    42645 2023-03-15 15:53:33.397385 bi_etl-1.4.3/bi_etl/components/hst_table_source_based.py
+-rw-r--r--   0        0        0    57029 2023-03-15 15:33:34.192481 bi_etl-1.4.3/bi_etl/components/readonlytable.py
+-rw-r--r--   0        0        0       54 2021-09-27 17:13:33.000000 bi_etl-1.4.3/bi_etl/components/row/__init__.py
+-rw-r--r--   0        0        0      456 2022-07-21 13:01:16.000000 bi_etl-1.4.3/bi_etl/components/row/cached_frozenset.py
+-rw-r--r--   0        0        0      564 2022-07-21 13:01:16.000000 bi_etl-1.4.3/bi_etl/components/row/column_difference.py
+-rw-r--r--   0        0        0    32775 2022-10-06 21:20:46.000000 bi_etl-1.4.3/bi_etl/components/row/row.py
+-rw-r--r--   0        0        0     1661 2022-07-21 13:01:16.000000 bi_etl-1.4.3/bi_etl/components/row/row_case_insensitive.py
+-rw-r--r--   0        0        0    25341 2023-03-15 15:32:32.540669 bi_etl-1.4.3/bi_etl/components/row/row_iteration_header.py
+-rw-r--r--   0        0        0     4220 2022-07-21 13:01:16.000000 bi_etl-1.4.3/bi_etl/components/row/row_iteration_header_case_insensitive.py
+-rw-r--r--   0        0        0      293 2022-07-21 13:01:16.000000 bi_etl-1.4.3/bi_etl/components/row/row_status.py
+-rw-r--r--   0        0        0     3165 2022-07-21 13:01:16.000000 bi_etl-1.4.3/bi_etl/components/sqlquery.py
+-rw-r--r--   0        0        0   164231 2023-03-15 15:33:43.015659 bi_etl-1.4.3/bi_etl/components/table.py
+-rw-r--r--   0        0        0     8365 2022-07-21 13:01:16.000000 bi_etl-1.4.3/bi_etl/components/w3c_reader.py
+-rw-r--r--   0        0        0     9820 2023-01-25 16:23:05.105369 bi_etl-1.4.3/bi_etl/components/xlsx_reader.py
+-rw-r--r--   0        0        0    12007 2022-08-30 16:22:27.000000 bi_etl-1.4.3/bi_etl/components/xlsx_writer.py
+-rw-r--r--   0        0        0        0 2022-07-21 13:01:16.000000 bi_etl-1.4.3/bi_etl/config/__init__.py
+-rw-r--r--   0        0        0     1780 2022-07-21 13:01:16.000000 bi_etl-1.4.3/bi_etl/config/bi_etl_config_base.py
+-rw-r--r--   0        0        0     3025 2023-03-15 15:33:34.244760 bi_etl-1.4.3/bi_etl/config/notifiers_config.py
+-rw-r--r--   0        0        0      328 2022-07-21 13:01:16.000000 bi_etl-1.4.3/bi_etl/config/scheduler_config.py
+-rw-r--r--   0        0        0    14301 2022-09-06 16:31:27.000000 bi_etl-1.4.3/bi_etl/conversions.py
+-rw-r--r--   0        0        0      133 2021-09-27 17:13:34.000000 bi_etl-1.4.3/bi_etl/database/__init__.py
+-rw-r--r--   0        0        0    17838 2023-07-05 15:26:38.339350 bi_etl-1.4.3/bi_etl/database/database_metadata.py
+-rw-r--r--   0        0        0     1045 2022-07-21 13:01:16.000000 bi_etl-1.4.3/bi_etl/database/mock_database_metadata.py
+-rw-r--r--   0        0        0     5699 2022-08-30 16:22:27.000000 bi_etl-1.4.3/bi_etl/example_config.ini
+-rw-r--r--   0        0        0     5490 2022-08-30 16:22:27.000000 bi_etl-1.4.3/bi_etl/example_config_shared.ini
+-rw-r--r--   0        0        0      923 2021-09-27 17:13:34.000000 bi_etl-1.4.3/bi_etl/exceptions/__init__.py
+-rw-r--r--   0        0        0        0 2021-09-27 17:13:34.000000 bi_etl-1.4.3/bi_etl/informatica/__init__.py
+-rw-r--r--   0        0        0       89 2022-07-21 13:01:17.000000 bi_etl-1.4.3/bi_etl/informatica/exceptions.py
+-rw-r--r--   0        0        0      493 2022-07-21 13:01:17.000000 bi_etl-1.4.3/bi_etl/informatica/pm_config.py
+-rw-r--r--   0        0        0     7540 2022-07-21 13:01:17.000000 bi_etl-1.4.3/bi_etl/informatica/pmcmd.py
+-rw-r--r--   0        0        0     1219 2022-07-21 13:01:17.000000 bi_etl-1.4.3/bi_etl/informatica/pmcmd_task.py
+-rw-r--r--   0        0        0    18054 2022-07-21 13:01:17.000000 bi_etl-1.4.3/bi_etl/informatica/pmrep.py
+-rw-r--r--   0        0        0        0 2021-09-27 17:13:34.000000 bi_etl-1.4.3/bi_etl/lookups/__init__.py
+-rw-r--r--   0        0        0    14159 2022-10-28 13:41:10.698113 bi_etl-1.4.3/bi_etl/lookups/autodisk_lookup.py
+-rw-r--r--   0        0        0     3965 2022-07-21 13:01:17.000000 bi_etl-1.4.3/bi_etl/lookups/autodisk_range_lookup.py
+-rw-r--r--   0        0        0     4699 2023-01-18 17:48:19.675169 bi_etl-1.4.3/bi_etl/lookups/disk_lookup.py
+-rw-r--r--   0        0        0     1934 2022-07-21 13:01:17.000000 bi_etl-1.4.3/bi_etl/lookups/disk_range_lookup.py
+-rw-r--r--   0        0        0    28901 2022-07-21 13:01:17.000000 bi_etl-1.4.3/bi_etl/lookups/lookup.py
+-rw-r--r--   0        0        0     9926 2022-07-21 13:01:17.000000 bi_etl-1.4.3/bi_etl/lookups/non_unique_lookup.py
+-rw-r--r--   0        0        0    12839 2022-07-21 13:01:17.000000 bi_etl-1.4.3/bi_etl/lookups/range_lookup.py
+-rw-r--r--   0        0        0     3358 2022-07-21 13:01:17.000000 bi_etl-1.4.3/bi_etl/memory_size.py
+-rw-r--r--   0        0        0      308 2022-07-21 13:01:17.000000 bi_etl-1.4.3/bi_etl/notifiers/__init__.py
+-rw-r--r--   0        0        0     4323 2022-07-21 13:01:17.000000 bi_etl-1.4.3/bi_etl/notifiers/email.py
+-rw-r--r--   0        0        0     8451 2022-07-21 20:01:17.000000 bi_etl-1.4.3/bi_etl/notifiers/jira.py
+-rw-r--r--   0        0        0      379 2022-07-21 13:01:17.000000 bi_etl-1.4.3/bi_etl/notifiers/log_notifier.py
+-rw-r--r--   0        0        0      706 2023-03-15 16:37:38.935207 bi_etl-1.4.3/bi_etl/notifiers/notifier_base.py
+-rw-r--r--   0        0        0     6398 2023-03-15 16:37:38.986969 bi_etl-1.4.3/bi_etl/notifiers/slack.py
+-rw-r--r--   0        0        0       61 2021-09-27 17:13:34.000000 bi_etl-1.4.3/bi_etl/parallel/__init__.py
+-rw-r--r--   0        0        0        1 2022-07-21 13:01:17.000000 bi_etl-1.4.3/bi_etl/parallel/mp.py
+-rw-r--r--   0        0        0        0 2021-09-27 17:13:34.000000 bi_etl-1.4.3/bi_etl/parameters/__init__.py
+-rw-r--r--   0        0        0      956 2021-09-27 17:13:34.000000 bi_etl-1.4.3/bi_etl/parameters/file_parameter.py
+-rw-r--r--   0        0        0       61 2021-09-27 17:13:34.000000 bi_etl-1.4.3/bi_etl/performance_test/__init__.py
+-rw-r--r--   0        0        0     1071 2022-07-21 13:01:17.000000 bi_etl-1.4.3/bi_etl/performance_test/perftest_static_reader.py
+-rw-r--r--   0        0        0        0 2021-09-27 17:13:34.000000 bi_etl-1.4.3/bi_etl/scheduler/__init__.py
+-rw-r--r--   0        0        0     1737 2022-10-06 21:20:46.000000 bi_etl-1.4.3/bi_etl/scheduler/dependent_reasons.py
+-rw-r--r--   0        0        0      706 2021-09-27 17:13:34.000000 bi_etl-1.4.3/bi_etl/scheduler/exceptions.py
+-rw-r--r--   0        0        0     1853 2021-09-27 17:13:34.000000 bi_etl-1.4.3/bi_etl/scheduler/messages.py
+-rw-r--r--   0        0        0    10430 2022-07-21 13:01:17.000000 bi_etl-1.4.3/bi_etl/scheduler/models.py
+-rw-r--r--   0        0        0      672 2022-07-21 13:01:17.000000 bi_etl-1.4.3/bi_etl/scheduler/queue_io.py
+-rw-r--r--   0        0        0      116 2021-09-27 17:13:34.000000 bi_etl-1.4.3/bi_etl/scheduler/run_scheduler.sh
+-rw-r--r--   0        0        0      391 2021-09-27 17:13:34.000000 bi_etl-1.4.3/bi_etl/scheduler/run_scheduler_screen.sh
+-rw-r--r--   0        0        0    65309 2022-10-06 21:20:46.000000 bi_etl-1.4.3/bi_etl/scheduler/scheduler.py
+-rw-r--r--   0        0        0        0 2021-09-27 17:13:34.000000 bi_etl-1.4.3/bi_etl/scheduler/scheduler_etl_jobs/__init__.py
+-rw-r--r--   0        0        0     2659 2022-07-21 13:01:17.000000 bi_etl-1.4.3/bi_etl/scheduler/scheduler_etl_jobs/etl_task_status_cd.py
+-rw-r--r--   0        0        0    28623 2022-07-21 13:01:17.000000 bi_etl-1.4.3/bi_etl/scheduler/scheduler_interface.py
+-rw-r--r--   0        0        0      444 2021-09-27 17:13:34.000000 bi_etl-1.4.3/bi_etl/scheduler/sdtout_queue.py
+-rw-r--r--   0        0        0      688 2022-07-21 13:01:17.000000 bi_etl-1.4.3/bi_etl/scheduler/special_tasks.py
+-rw-r--r--   0        0        0     2801 2022-07-21 13:01:17.000000 bi_etl-1.4.3/bi_etl/scheduler/status.py
+-rw-r--r--   0        0        0    57835 2023-06-27 14:21:39.760133 bi_etl-1.4.3/bi_etl/scheduler/task.py
+-rw-r--r--   0        0        0     7377 2022-10-31 20:23:08.644384 bi_etl-1.4.3/bi_etl/statement_queue.py
+-rw-r--r--   0        0        0     6742 2022-07-21 13:01:17.000000 bi_etl-1.4.3/bi_etl/statistics.py
+-rw-r--r--   0        0        0       61 2021-09-27 17:13:34.000000 bi_etl-1.4.3/bi_etl/test_notebooks/__init__.py
+-rw-r--r--   0        0        0     1073 2022-06-09 14:18:34.000000 bi_etl-1.4.3/bi_etl/test_notebooks/perftest_static_reader.py
+-rw-r--r--   0        0        0    17122 2022-05-12 15:44:59.000000 bi_etl-1.4.3/bi_etl/test_notebooks/Row performance.ipynb
+-rw-r--r--   0        0        0     3509 2022-05-12 15:44:59.000000 bi_etl-1.4.3/bi_etl/test_notebooks/Utility Test.ipynb
+-rw-r--r--   0        0        0     4343 2021-09-27 17:13:34.000000 bi_etl-1.4.3/bi_etl/timer.py
+-rw-r--r--   0        0        0    11366 2022-07-21 13:01:17.000000 bi_etl-1.4.3/bi_etl/utility/__init__.py
+-rw-r--r--   0        0        0     2118 2022-07-21 13:01:17.000000 bi_etl-1.4.3/bi_etl/utility/ask.py
+-rw-r--r--   0        0        0     8976 2023-01-18 17:48:19.758841 bi_etl-1.4.3/bi_etl/utility/bcp_helpers.py
+-rw-r--r--   0        0        0      925 2021-09-27 17:13:34.000000 bi_etl-1.4.3/bi_etl/utility/case_insentive_set.py
+-rw-r--r--   0        0        0     1869 2022-07-21 13:01:17.000000 bi_etl-1.4.3/bi_etl/utility/copy_table_data.py
+-rw-r--r--   0        0        0     5000 2022-07-21 13:01:17.000000 bi_etl-1.4.3/bi_etl/utility/line_counter.py
+-rw-r--r--   0        0        0      472 2021-09-27 17:13:34.000000 bi_etl-1.4.3/bi_etl/utility/logging_helpers.py
+-rw-r--r--   0        0        0      947 2022-07-21 13:01:17.000000 bi_etl-1.4.3/bi_etl/utility/package_root.py
+-rw-r--r--   0        0        0       61 2021-09-27 17:13:34.000000 bi_etl-1.4.3/bi_etl/utility/postgresql/__init__.py
+-rw-r--r--   0        0        0     3686 2023-01-18 17:48:19.844889 bi_etl-1.4.3/bi_etl/utility/postgresql/psql_command.py
+-rw-r--r--   0        0        0     4777 2022-10-06 20:52:27.000000 bi_etl-1.4.3/bi_etl/utility/postgresql/psycopg2_helpers.py
+-rw-r--r--   0        0        0    11998 2023-03-15 15:33:34.410960 bi_etl-1.4.3/bi_etl/utility/run_sql_script.py
+-rw-r--r--   0        0        0       61 2021-09-27 17:13:34.000000 bi_etl-1.4.3/bi_etl/utility/sql_server/__init__.py
+-rw-r--r--   0        0        0     2776 2023-06-27 14:01:47.122835 bi_etl-1.4.3/bi_etl/utility/sql_server/defrag_indexes.py
+-rw-r--r--   0        0        0     4674 2022-07-21 13:01:17.000000 bi_etl-1.4.3/bi_etl/utility/ssh_forward.py
+-rw-r--r--   0        0        0      341 2022-07-21 13:01:17.000000 bi_etl-1.4.3/bi_etl/version.py
+-rw-r--r--   0        0        0     1086 2020-06-29 20:22:28.000000 bi_etl-1.4.3/license.txt
+-rw-r--r--   0        0        0     2009 2023-07-05 16:46:27.214059 bi_etl-1.4.3/pyproject.toml
+-rw-r--r--   0        0        0     1251 2022-10-06 21:20:46.000000 bi_etl-1.4.3/README.md
+-rw-r--r--   0        0        0     2975 1970-01-01 00:00:00.000000 bi_etl-1.4.3/PKG-INFO
```

### Comparing `bi_etl-1.4.2/bi_etl/.coveragerc` & `bi_etl-1.4.3/bi_etl/.coveragerc`

 * *Files identical despite different names*

### Comparing `bi_etl-1.4.2/bi_etl/.pylintrc` & `bi_etl-1.4.3/bi_etl/.pylintrc`

 * *Files identical despite different names*

### Comparing `bi_etl-1.4.2/bi_etl/__main__.py` & `bi_etl-1.4.3/bi_etl/__main__.py`

 * *Files identical despite different names*

### Comparing `bi_etl-1.4.2/bi_etl/boto3_helper/dynamodb.py` & `bi_etl-1.4.3/bi_etl/boto3_helper/dynamodb.py`

 * *Files identical despite different names*

### Comparing `bi_etl-1.4.2/bi_etl/boto3_helper/s3.py` & `bi_etl-1.4.3/bi_etl/boto3_helper/s3.py`

 * *Files identical despite different names*

### Comparing `bi_etl-1.4.2/bi_etl/boto3_helper/session.py` & `bi_etl-1.4.3/bi_etl/boto3_helper/session.py`

 * *Files identical despite different names*

### Comparing `bi_etl-1.4.2/bi_etl/bulk_loaders/bulk_loader.py` & `bi_etl-1.4.3/bi_etl/bulk_loaders/bulk_loader.py`

 * *Files identical despite different names*

### Comparing `bi_etl-1.4.2/bi_etl/bulk_loaders/bulk_loader_exception.py` & `bi_etl-1.4.3/bi_etl/bulk_loaders/bulk_loader_exception.py`

 * *Files identical despite different names*

### Comparing `bi_etl-1.4.2/bi_etl/bulk_loaders/postgresql_copy.py` & `bi_etl-1.4.3/bi_etl/bulk_loaders/postgresql_copy.py`

 * *Files identical despite different names*

### Comparing `bi_etl-1.4.2/bi_etl/bulk_loaders/redshift_s3_avro_loader.py` & `bi_etl-1.4.3/bi_etl/bulk_loaders/redshift_s3_avro_loader.py`

 * *Files identical despite different names*

### Comparing `bi_etl-1.4.2/bi_etl/bulk_loaders/redshift_s3_base.py` & `bi_etl-1.4.3/bi_etl/bulk_loaders/redshift_s3_base.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 # https://www.python.org/dev/peps/pep-0563/
 from __future__ import annotations
 
 import os.path
 import textwrap
 import time
+import uuid
 from pathlib import Path
 from typing import *
 
 import boto3
 import sqlalchemy
 from sqlalchemy import text
 
@@ -120,19 +121,23 @@
 
         self.log.info(f"Uploaded {total_size:,} bytes in total to {s3_full_folder}")
         return s3_files
 
     def _get_error_details(
             self,
             connection: sqlalchemy.engine.base.Connection,
-            table_object: Table,
-            exception: sqlalchemy.exc.SQLAlchemyError
+            exception: sqlalchemy.exc.SQLAlchemyError,
+            s3_source_path: str,
     ) -> BulkLoaderException:
         bulk_loader_exception = BulkLoaderException(exception, password=self.s3_password)
 
+        # early exit for cases where we failed while making a connection
+        if connection is None:
+            return bulk_loader_exception
+
         self.log.debug(f'Getting pg_last_copy_id')
 
         pg_last_copy_id_res = connection.execute("select pg_last_copy_id() as id")
         pg_last_copy_id_row = next(pg_last_copy_id_res)
         pg_last_copy_id = pg_last_copy_id_row.id
 
         self.log.error(f'pg_last_copy_id = {pg_last_copy_id}')
@@ -141,19 +146,19 @@
             sql = """
                     SELECT *
                     FROM stl_load_errors
                     WHERE query = pg_last_copy_id()
                     ORDER BY starttime DESC
                   """
         else:
-            self.log.error(f"Unable to use pg_last_copy_id()")
+            self.log.error(f"Unable to use pg_last_copy_id().  Seems to only work on successful COPY.")
             sql = f"""
                     SELECT TOP 1 *
                     FROM stl_load_errors
-                    WHERE filename like '%{table_object.table_name}%'
+                    WHERE filename like '%{s3_source_path}%'
                     ORDER BY starttime DESC
                    """
 
         self.log.error(f'Checking stl_load_errors with\n{sql}')
         try:
             results = connection.execute(text(sql))
         except Exception as e2:
@@ -184,78 +189,87 @@
 
         return bulk_loader_exception
 
     def _run_copy_sql(
             self,
             copy_sql: str,
             table_object: Table,
+            s3_source_path: str,
     ) -> int:
         copy_sql = textwrap.dedent(copy_sql)
         sql_safe_pw = copy_sql.replace(self.s3_password, '*' * 8)
         self.log.debug(sql_safe_pw)
 
         keep_trying = True
         wait_seconds = 15
         t_end = time.time() + wait_seconds
+        connection = None
+        rows_loaded = None
 
         while keep_trying:
+
             try:
                 connection = table_object.connection()
                 connection.execute(copy_sql)
                 # Load worked we can stop looping
                 keep_trying = False
                 connection.execute(f"COMMIT;")
             except sqlalchemy.exc.SQLAlchemyError as e:
                 safe_e = str(e).replace(self.s3_password, '*' * 8)
 
                 # Check if the error is non-recoverable
-                if any(error in str(e) for error in self.non_recoverable_error_matches):
-                    self.log.error(f"Cannot recover from this error - {safe_e}")
-                    raise
 
                 self.log.error('!' * 80)
                 self.log.error(f'!! Details for {safe_e} below:')
                 self.log.error('!' * 80)
 
                 bulk_loader_exception = self._get_error_details(
                     connection=connection,
-                    table_object=table_object,
                     exception=e,
+                    s3_source_path=s3_source_path,
                 )
 
                 if 'S3ServiceException' in str(e):
-                    if time.time() > t_end:
-                        self.log.info(f'{wait_seconds} seconds wait is over. File cannot be loaded. {t_end}')
+                    if any(error in str(e) for error in self.non_recoverable_error_matches):
+                        self.log.error(f"Cannot recover from this error - {safe_e}")
+                        keep_trying = False
+                    elif time.time() > t_end:
+                        self.log.info(f'{wait_seconds} seconds recovery wait time exceeded. File cannot be loaded. {t_end}')
                         keep_trying = False
-                    self.log.info(f'Will retry in 5 seconds file copy after S3ServiceException failure - {safe_e}')
-                    time.sleep(5)
-                else:
-                    raise bulk_loader_exception
 
-        sql = f"""
-        SELECT SUM(lines_scanned) as lines_scanned, count(DISTINCT filename) as file_cnt
-        FROM stl_load_commits
-        WHERE query = pg_last_copy_id()
-        """
-        # Default to -1 rows to indicate error
-        rows_loaded = -1
-        try:
-            results = connection.execute(sql)
-            for row in results:
-                lines_scanned = row.lines_scanned
-                file_cnt = row.file_cnt
-                if self.lines_scanned_modifier == 0:
-                    rows_loaded = lines_scanned
+                    if keep_trying:
+                        self.log.info(f'Will retry in 5 seconds file copy after S3ServiceException failure - {safe_e}')
+                        time.sleep(5)
+                    else:
+                        raise bulk_loader_exception from None
                 else:
-                    rows_loaded = lines_scanned + (self.lines_scanned_modifier * file_cnt)
-        except Exception as e:
-            e = str(e).replace(self.s3_password, '*' * 8)
-            self.log.warning(f"Error getting row count: {e}")
+                    raise bulk_loader_exception from None
+
+        if connection is not None:
+            sql = f"""
+            SELECT SUM(lines_scanned) as lines_scanned, count(DISTINCT filename) as file_cnt
+            FROM stl_load_commits
+            WHERE query = pg_last_copy_id()
+            """
+            # Default to -1 rows to indicate error
+            rows_loaded = -1
+            try:
+                results = connection.execute(sql)
+                for row in results:
+                    lines_scanned = row.lines_scanned
+                    file_cnt = row.file_cnt
+                    if self.lines_scanned_modifier == 0:
+                        rows_loaded = lines_scanned
+                    else:
+                        rows_loaded = lines_scanned + (self.lines_scanned_modifier * file_cnt)
+            except Exception as e:
+                e = str(e).replace(self.s3_password, '*' * 8)
+                self.log.warning(f"Error getting row count: {e}")
 
-        connection.close()
+            connection.close()
 
         return rows_loaded
 
     def get_copy_sql(
             self,
             s3_source_path: str,
             table_to_load: str,
@@ -288,14 +302,15 @@
             file_compression=file_compression,
             analyze_compression=analyze_compression,
             options=options,
         )
         rows_loaded = self._run_copy_sql(
             copy_sql=copy_sql,
             table_object=table_object,
+            s3_source_path=s3_source_path,
         )
         if perform_rename:
             self.rename_table(table_to_load, table_object)
         return rows_loaded
 
     def load_from_files(
             self,
```

### Comparing `bi_etl-1.4.2/bi_etl/bulk_loaders/redshift_s3_csv_loader.py` & `bi_etl-1.4.3/bi_etl/bulk_loaders/redshift_s3_csv_loader.py`

 * *Files identical despite different names*

### Comparing `bi_etl-1.4.2/bi_etl/bulk_loaders/redshift_s3_json_loader.py` & `bi_etl-1.4.3/bi_etl/bulk_loaders/redshift_s3_json_loader.py`

 * *Files identical despite different names*

### Comparing `bi_etl-1.4.2/bi_etl/bulk_loaders/redshift_s3_parquet_loader.py` & `bi_etl-1.4.3/bi_etl/bulk_loaders/redshift_s3_parquet_loader.py`

 * *Files identical despite different names*

### Comparing `bi_etl-1.4.2/bi_etl/bulk_loaders/s3_bulk_load_config.py` & `bi_etl-1.4.3/bi_etl/bulk_loaders/s3_bulk_load_config.py`

 * *Files identical despite different names*

### Comparing `bi_etl-1.4.2/bi_etl/bulk_loaders/sql_server_bcp.py` & `bi_etl-1.4.3/bi_etl/bulk_loaders/sql_server_bcp.py`

 * *Files identical despite different names*

### Comparing `bi_etl-1.4.2/bi_etl/components/csv_writer.py` & `bi_etl-1.4.3/bi_etl/components/csv_writer.py`

 * *Files identical despite different names*

### Comparing `bi_etl-1.4.2/bi_etl/components/csvreader.py` & `bi_etl-1.4.3/bi_etl/components/csvreader.py`

 * *Files identical despite different names*

### Comparing `bi_etl-1.4.2/bi_etl/components/data_analyzer.py` & `bi_etl-1.4.3/bi_etl/components/data_analyzer.py`

 * *Files identical despite different names*

### Comparing `bi_etl-1.4.2/bi_etl/components/etlcomponent.py` & `bi_etl-1.4.3/bi_etl/components/etlcomponent.py`

 * *Files identical despite different names*

### Comparing `bi_etl-1.4.2/bi_etl/components/get_next_key/base_table_memory.py` & `bi_etl-1.4.3/bi_etl/components/get_next_key/base_table_memory.py`

 * *Files identical despite different names*

### Comparing `bi_etl-1.4.2/bi_etl/components/get_next_key/local_table_memory.py` & `bi_etl-1.4.3/bi_etl/components/get_next_key/local_table_memory.py`

 * *Files identical despite different names*

### Comparing `bi_etl-1.4.2/bi_etl/components/get_next_key/shared_table_memory.py` & `bi_etl-1.4.3/bi_etl/components/get_next_key/shared_table_memory.py`

 * *Files identical despite different names*

### Comparing `bi_etl-1.4.2/bi_etl/components/get_next_key/shared_table_memory_manager.py` & `bi_etl-1.4.3/bi_etl/components/get_next_key/shared_table_memory_manager.py`

 * *Files identical despite different names*

### Comparing `bi_etl-1.4.2/bi_etl/components/hst_table.py` & `bi_etl-1.4.3/bi_etl/components/hst_table.py`

 * *Files identical despite different names*

### Comparing `bi_etl-1.4.2/bi_etl/components/hst_table_source_based.py` & `bi_etl-1.4.3/bi_etl/components/hst_table_source_based.py`

 * *Files identical despite different names*

### Comparing `bi_etl-1.4.2/bi_etl/components/readonlytable.py` & `bi_etl-1.4.3/bi_etl/components/readonlytable.py`

 * *Files identical despite different names*

### Comparing `bi_etl-1.4.2/bi_etl/components/row/column_difference.py` & `bi_etl-1.4.3/bi_etl/components/row/column_difference.py`

 * *Files identical despite different names*

### Comparing `bi_etl-1.4.2/bi_etl/components/row/row.py` & `bi_etl-1.4.3/bi_etl/components/row/row.py`

 * *Files identical despite different names*

### Comparing `bi_etl-1.4.2/bi_etl/components/row/row_case_insensitive.py` & `bi_etl-1.4.3/bi_etl/components/row/row_case_insensitive.py`

 * *Files identical despite different names*

### Comparing `bi_etl-1.4.2/bi_etl/components/row/row_iteration_header.py` & `bi_etl-1.4.3/bi_etl/components/row/row_iteration_header.py`

 * *Files identical despite different names*

### Comparing `bi_etl-1.4.2/bi_etl/components/row/row_iteration_header_case_insensitive.py` & `bi_etl-1.4.3/bi_etl/components/row/row_iteration_header_case_insensitive.py`

 * *Files identical despite different names*

### Comparing `bi_etl-1.4.2/bi_etl/components/sqlquery.py` & `bi_etl-1.4.3/bi_etl/components/sqlquery.py`

 * *Files identical despite different names*

### Comparing `bi_etl-1.4.2/bi_etl/components/table.py` & `bi_etl-1.4.3/bi_etl/components/table.py`

 * *Files identical despite different names*

### Comparing `bi_etl-1.4.2/bi_etl/components/w3c_reader.py` & `bi_etl-1.4.3/bi_etl/components/w3c_reader.py`

 * *Files identical despite different names*

### Comparing `bi_etl-1.4.2/bi_etl/components/xlsx_reader.py` & `bi_etl-1.4.3/bi_etl/components/xlsx_reader.py`

 * *Files identical despite different names*

### Comparing `bi_etl-1.4.2/bi_etl/components/xlsx_writer.py` & `bi_etl-1.4.3/bi_etl/components/xlsx_writer.py`

 * *Files identical despite different names*

### Comparing `bi_etl-1.4.2/bi_etl/config/bi_etl_config_base.py` & `bi_etl-1.4.3/bi_etl/config/bi_etl_config_base.py`

 * *Files identical despite different names*

### Comparing `bi_etl-1.4.2/bi_etl/config/notifiers_config.py` & `bi_etl-1.4.3/bi_etl/config/notifiers_config.py`

 * *Files identical despite different names*

### Comparing `bi_etl-1.4.2/bi_etl/conversions.py` & `bi_etl-1.4.3/bi_etl/conversions.py`

 * *Files identical despite different names*

### Comparing `bi_etl-1.4.2/bi_etl/database/database_metadata.py` & `bi_etl-1.4.3/bi_etl/database/database_metadata.py`

 * *Files 0% similar despite different names*

```diff
@@ -240,25 +240,23 @@
                 auto_commit=auto_commit,
             )
             if transaction:
                 transaction_ctl = connection.begin()
             else:
                 transaction_ctl = None
             result = connection.execute(sql, *list_params, **params)
-
+            return result
         finally:
             if transaction:
                 if transaction_ctl is not None:
                     transaction_ctl.commit()
             if auto_close:
                 if connection is not None:
                     connection.close()
 
-        return result
-
     def execute_procedure(
             self,
             procedure_name,
             *args,
             return_results=False,
             dpapi_connection=None
     ):
```

### Comparing `bi_etl-1.4.2/bi_etl/database/mock_database_metadata.py` & `bi_etl-1.4.3/bi_etl/database/mock_database_metadata.py`

 * *Files identical despite different names*

### Comparing `bi_etl-1.4.2/bi_etl/example_config.ini` & `bi_etl-1.4.3/bi_etl/example_config.ini`

 * *Files identical despite different names*

### Comparing `bi_etl-1.4.2/bi_etl/example_config_shared.ini` & `bi_etl-1.4.3/bi_etl/example_config_shared.ini`

 * *Files identical despite different names*

### Comparing `bi_etl-1.4.2/bi_etl/exceptions/__init__.py` & `bi_etl-1.4.3/bi_etl/exceptions/__init__.py`

 * *Files identical despite different names*

### Comparing `bi_etl-1.4.2/bi_etl/informatica/pmcmd.py` & `bi_etl-1.4.3/bi_etl/informatica/pmcmd.py`

 * *Files identical despite different names*

### Comparing `bi_etl-1.4.2/bi_etl/informatica/pmcmd_task.py` & `bi_etl-1.4.3/bi_etl/informatica/pmcmd_task.py`

 * *Files identical despite different names*

### Comparing `bi_etl-1.4.2/bi_etl/informatica/pmrep.py` & `bi_etl-1.4.3/bi_etl/informatica/pmrep.py`

 * *Files identical despite different names*

### Comparing `bi_etl-1.4.2/bi_etl/lookups/autodisk_lookup.py` & `bi_etl-1.4.3/bi_etl/lookups/autodisk_lookup.py`

 * *Files identical despite different names*

### Comparing `bi_etl-1.4.2/bi_etl/lookups/autodisk_range_lookup.py` & `bi_etl-1.4.3/bi_etl/lookups/autodisk_range_lookup.py`

 * *Files identical despite different names*

### Comparing `bi_etl-1.4.2/bi_etl/lookups/disk_lookup.py` & `bi_etl-1.4.3/bi_etl/lookups/disk_lookup.py`

 * *Files identical despite different names*

### Comparing `bi_etl-1.4.2/bi_etl/lookups/disk_range_lookup.py` & `bi_etl-1.4.3/bi_etl/lookups/disk_range_lookup.py`

 * *Files identical despite different names*

### Comparing `bi_etl-1.4.2/bi_etl/lookups/lookup.py` & `bi_etl-1.4.3/bi_etl/lookups/lookup.py`

 * *Files identical despite different names*

### Comparing `bi_etl-1.4.2/bi_etl/lookups/non_unique_lookup.py` & `bi_etl-1.4.3/bi_etl/lookups/non_unique_lookup.py`

 * *Files identical despite different names*

### Comparing `bi_etl-1.4.2/bi_etl/lookups/range_lookup.py` & `bi_etl-1.4.3/bi_etl/lookups/range_lookup.py`

 * *Files identical despite different names*

### Comparing `bi_etl-1.4.2/bi_etl/memory_size.py` & `bi_etl-1.4.3/bi_etl/memory_size.py`

 * *Files identical despite different names*

### Comparing `bi_etl-1.4.2/bi_etl/notifiers/email.py` & `bi_etl-1.4.3/bi_etl/notifiers/email.py`

 * *Files identical despite different names*

### Comparing `bi_etl-1.4.2/bi_etl/notifiers/jira.py` & `bi_etl-1.4.3/bi_etl/notifiers/jira.py`

 * *Files identical despite different names*

### Comparing `bi_etl-1.4.2/bi_etl/notifiers/notifier_base.py` & `bi_etl-1.4.3/bi_etl/notifiers/notifier_base.py`

 * *Files identical despite different names*

### Comparing `bi_etl-1.4.2/bi_etl/notifiers/slack.py` & `bi_etl-1.4.3/bi_etl/notifiers/slack.py`

 * *Files identical despite different names*

### Comparing `bi_etl-1.4.2/bi_etl/parameters/file_parameter.py` & `bi_etl-1.4.3/bi_etl/parameters/file_parameter.py`

 * *Files identical despite different names*

### Comparing `bi_etl-1.4.2/bi_etl/performance_test/perftest_static_reader.py` & `bi_etl-1.4.3/bi_etl/performance_test/perftest_static_reader.py`

 * *Files identical despite different names*

### Comparing `bi_etl-1.4.2/bi_etl/scheduler/dependent_reasons.py` & `bi_etl-1.4.3/bi_etl/scheduler/dependent_reasons.py`

 * *Files identical despite different names*

### Comparing `bi_etl-1.4.2/bi_etl/scheduler/exceptions.py` & `bi_etl-1.4.3/bi_etl/scheduler/exceptions.py`

 * *Files identical despite different names*

### Comparing `bi_etl-1.4.2/bi_etl/scheduler/messages.py` & `bi_etl-1.4.3/bi_etl/scheduler/messages.py`

 * *Files identical despite different names*

### Comparing `bi_etl-1.4.2/bi_etl/scheduler/models.py` & `bi_etl-1.4.3/bi_etl/scheduler/models.py`

 * *Files identical despite different names*

### Comparing `bi_etl-1.4.2/bi_etl/scheduler/queue_io.py` & `bi_etl-1.4.3/bi_etl/scheduler/queue_io.py`

 * *Files identical despite different names*

### Comparing `bi_etl-1.4.2/bi_etl/scheduler/scheduler.py` & `bi_etl-1.4.3/bi_etl/scheduler/scheduler.py`

 * *Files identical despite different names*

### Comparing `bi_etl-1.4.2/bi_etl/scheduler/scheduler_etl_jobs/etl_task_status_cd.py` & `bi_etl-1.4.3/bi_etl/scheduler/scheduler_etl_jobs/etl_task_status_cd.py`

 * *Files identical despite different names*

### Comparing `bi_etl-1.4.2/bi_etl/scheduler/scheduler_interface.py` & `bi_etl-1.4.3/bi_etl/scheduler/scheduler_interface.py`

 * *Files identical despite different names*

### Comparing `bi_etl-1.4.2/bi_etl/scheduler/special_tasks.py` & `bi_etl-1.4.3/bi_etl/scheduler/special_tasks.py`

 * *Files identical despite different names*

### Comparing `bi_etl-1.4.2/bi_etl/scheduler/status.py` & `bi_etl-1.4.3/bi_etl/scheduler/status.py`

 * *Files identical despite different names*

### Comparing `bi_etl-1.4.2/bi_etl/scheduler/task.py` & `bi_etl-1.4.3/bi_etl/scheduler/task.py`

 * *Files identical despite different names*

### Comparing `bi_etl-1.4.2/bi_etl/statement_queue.py` & `bi_etl-1.4.3/bi_etl/statement_queue.py`

 * *Files identical despite different names*

### Comparing `bi_etl-1.4.2/bi_etl/statistics.py` & `bi_etl-1.4.3/bi_etl/statistics.py`

 * *Files identical despite different names*

### Comparing `bi_etl-1.4.2/bi_etl/test_notebooks/perftest_static_reader.py` & `bi_etl-1.4.3/bi_etl/test_notebooks/perftest_static_reader.py`

 * *Files identical despite different names*

### Comparing `bi_etl-1.4.2/bi_etl/test_notebooks/Row performance.ipynb` & `bi_etl-1.4.3/bi_etl/test_notebooks/Row performance.ipynb`

 * *Files identical despite different names*

### Comparing `bi_etl-1.4.2/bi_etl/test_notebooks/Utility Test.ipynb` & `bi_etl-1.4.3/bi_etl/test_notebooks/Utility Test.ipynb`

 * *Files identical despite different names*

### Comparing `bi_etl-1.4.2/bi_etl/timer.py` & `bi_etl-1.4.3/bi_etl/timer.py`

 * *Files identical despite different names*

### Comparing `bi_etl-1.4.2/bi_etl/utility/__init__.py` & `bi_etl-1.4.3/bi_etl/utility/__init__.py`

 * *Files identical despite different names*

### Comparing `bi_etl-1.4.2/bi_etl/utility/ask.py` & `bi_etl-1.4.3/bi_etl/utility/ask.py`

 * *Files identical despite different names*

### Comparing `bi_etl-1.4.2/bi_etl/utility/bcp_helpers.py` & `bi_etl-1.4.3/bi_etl/utility/bcp_helpers.py`

 * *Files identical despite different names*

### Comparing `bi_etl-1.4.2/bi_etl/utility/case_insentive_set.py` & `bi_etl-1.4.3/bi_etl/utility/case_insentive_set.py`

 * *Files identical despite different names*

### Comparing `bi_etl-1.4.2/bi_etl/utility/copy_table_data.py` & `bi_etl-1.4.3/bi_etl/utility/copy_table_data.py`

 * *Files identical despite different names*

### Comparing `bi_etl-1.4.2/bi_etl/utility/line_counter.py` & `bi_etl-1.4.3/bi_etl/utility/line_counter.py`

 * *Files identical despite different names*

### Comparing `bi_etl-1.4.2/bi_etl/utility/package_root.py` & `bi_etl-1.4.3/bi_etl/utility/package_root.py`

 * *Files identical despite different names*

### Comparing `bi_etl-1.4.2/bi_etl/utility/postgresql/psql_command.py` & `bi_etl-1.4.3/bi_etl/utility/postgresql/psql_command.py`

 * *Files identical despite different names*

### Comparing `bi_etl-1.4.2/bi_etl/utility/postgresql/psycopg2_helpers.py` & `bi_etl-1.4.3/bi_etl/utility/postgresql/psycopg2_helpers.py`

 * *Files identical despite different names*

### Comparing `bi_etl-1.4.2/bi_etl/utility/run_sql_script.py` & `bi_etl-1.4.3/bi_etl/utility/run_sql_script.py`

 * *Files identical despite different names*

### Comparing `bi_etl-1.4.2/bi_etl/utility/sql_server/defrag_indexes.py` & `bi_etl-1.4.3/bi_etl/utility/sql_server/defrag_indexes.py`

 * *Files identical despite different names*

### Comparing `bi_etl-1.4.2/bi_etl/utility/ssh_forward.py` & `bi_etl-1.4.3/bi_etl/utility/ssh_forward.py`

 * *Files identical despite different names*

### Comparing `bi_etl-1.4.2/license.txt` & `bi_etl-1.4.3/license.txt`

 * *Files identical despite different names*

### Comparing `bi_etl-1.4.2/pyproject.toml` & `bi_etl-1.4.3/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "bi_etl"
-version = "1.4.2"
+version = "1.4.3"
 description = "Python ETL Framework"
 keywords=["etl"]
 classifiers = [
     "Topic :: Software Development :: Libraries :: Python Modules",
     "Development Status :: 5 - Production/Stable",
     "Topic :: Database",
 ]
```

### Comparing `bi_etl-1.4.2/README.md` & `bi_etl-1.4.3/README.md`

 * *Files identical despite different names*

### Comparing `bi_etl-1.4.2/PKG-INFO` & `bi_etl-1.4.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bi-etl
-Version: 1.4.2
+Version: 1.4.3
 Summary: Python ETL Framework
 Home-page: https://github.com/arcann/bi_etl
 License: MIT
 Keywords: etl
 Author: Derek Wood
 Author-email: bietl_info@bietl.dev
 Requires-Python: >=3.7,<4.0
```

