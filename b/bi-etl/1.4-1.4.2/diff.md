# Comparing `tmp/bi_etl-1.4.tar.gz` & `tmp/bi_etl-1.4.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bi_etl-1.4.tar", max compression
+gzip compressed data, was "bi_etl-1.4.2.tar", max compression
```

## Comparing `bi_etl-1.4.tar` & `bi_etl-1.4.2.tar`

### file list

```diff
@@ -1,132 +1,131 @@
--rw-r--r--   0        0        0      628 2021-09-27 17:13:33.000000 bi_etl-1.4/bi_etl/.coveragerc
--rw-r--r--   0        0        0      360 2021-09-27 17:13:33.000000 bi_etl-1.4/bi_etl/.project
--rw-r--r--   0        0        0      423 2021-09-27 17:13:33.000000 bi_etl-1.4/bi_etl/.pydevproject
--rw-r--r--   0        0        0     3529 2021-09-27 17:13:33.000000 bi_etl-1.4/bi_etl/.pylintrc
--rw-r--r--   0        0        0      104 2022-07-21 13:01:16.000000 bi_etl-1.4/bi_etl/__init__.py
--rw-r--r--   0        0        0     2612 2022-07-21 13:01:16.000000 bi_etl-1.4/bi_etl/__main__.py
--rw-r--r--   0        0        0       61 2022-07-21 13:01:16.000000 bi_etl-1.4/bi_etl/boto3_helper/__init__.py
--rw-r--r--   0        0        0     1664 2022-07-21 13:01:16.000000 bi_etl-1.4/bi_etl/boto3_helper/dynamodb.py
--rw-r--r--   0        0        0      148 2022-07-21 13:01:16.000000 bi_etl-1.4/bi_etl/boto3_helper/lambdas.py
--rw-r--r--   0        0        0    12181 2022-08-11 15:34:45.000000 bi_etl-1.4/bi_etl/boto3_helper/s3.py
--rw-r--r--   0        0        0     1905 2022-07-21 13:01:16.000000 bi_etl-1.4/bi_etl/boto3_helper/session.py
--rw-r--r--   0        0        0      142 2022-07-21 13:01:16.000000 bi_etl-1.4/bi_etl/boto3_helper/ssm.py
--rw-r--r--   0        0        0        0 2021-09-27 17:13:33.000000 bi_etl-1.4/bi_etl/bulk_loaders/__init__.py
--rw-r--r--   0        0        0     6756 2023-03-15 15:53:33.483857 bi_etl-1.4/bi_etl/bulk_loaders/bulk_loader.py
--rw-r--r--   0        0        0      982 2021-09-27 17:13:33.000000 bi_etl-1.4/bi_etl/bulk_loaders/bulk_loader_exception.py
--rw-r--r--   0        0        0      323 2022-10-06 20:54:25.000000 bi_etl-1.4/bi_etl/bulk_loaders/postgresql_bulk_load_config.py
--rw-r--r--   0        0        0     3759 2023-01-18 17:48:19.693841 bi_etl-1.4/bi_etl/bulk_loaders/postgresql_copy.py
--rw-r--r--   0        0        0     6299 2023-01-18 17:48:19.786858 bi_etl-1.4/bi_etl/bulk_loaders/redshift_s3_avro_loader.py
--rw-r--r--   0        0        0    13303 2023-01-18 15:00:40.203491 bi_etl-1.4/bi_etl/bulk_loaders/redshift_s3_base.py
--rw-r--r--   0        0        0    11775 2023-01-18 17:48:19.808886 bi_etl-1.4/bi_etl/bulk_loaders/redshift_s3_csv_loader.py
--rw-r--r--   0        0        0     4081 2023-01-18 17:48:19.827968 bi_etl-1.4/bi_etl/bulk_loaders/redshift_s3_json_loader.py
--rw-r--r--   0        0        0     6335 2023-01-18 17:48:19.714844 bi_etl-1.4/bi_etl/bulk_loaders/redshift_s3_parquet_loader.py
--rw-r--r--   0        0        0     1063 2023-01-10 02:14:59.086394 bi_etl-1.4/bi_etl/bulk_loaders/s3_bulk_load_config.py
--rw-r--r--   0        0        0     4821 2023-01-18 17:48:19.735841 bi_etl-1.4/bi_etl/bulk_loaders/sql_server_bcp.py
--rw-r--r--   0        0        0        0 2021-09-27 17:13:33.000000 bi_etl-1.4/bi_etl/components/__init__.py
--rw-r--r--   0        0        0    16109 2022-10-06 21:12:48.000000 bi_etl-1.4/bi_etl/components/csv_writer.py
--rw-r--r--   0        0        0    17630 2022-08-24 15:21:41.000000 bi_etl-1.4/bi_etl/components/csvreader.py
--rw-r--r--   0        0        0    19384 2022-07-21 13:01:16.000000 bi_etl-1.4/bi_etl/components/data_analyzer.py
--rw-r--r--   0        0        0    52067 2022-10-31 19:45:21.367328 bi_etl-1.4/bi_etl/components/etlcomponent.py
--rw-r--r--   0        0        0       61 2021-09-27 17:13:33.000000 bi_etl-1.4/bi_etl/components/get_next_key/__init__.py
--rw-r--r--   0        0        0      873 2022-05-04 02:21:27.000000 bi_etl-1.4/bi_etl/components/get_next_key/base_table_memory.py
--rw-r--r--   0        0        0      644 2021-09-27 17:13:33.000000 bi_etl-1.4/bi_etl/components/get_next_key/local_table_memory.py
--rw-r--r--   0        0        0     2047 2022-06-06 16:22:38.000000 bi_etl-1.4/bi_etl/components/get_next_key/shared_table_memory.py
--rw-r--r--   0        0        0      708 2021-09-27 17:13:33.000000 bi_etl-1.4/bi_etl/components/get_next_key/shared_table_memory_manager.py
--rw-r--r--   0        0        0   107458 2023-03-15 15:33:34.268035 bi_etl-1.4/bi_etl/components/hst_table.py
--rw-r--r--   0        0        0    42645 2023-03-15 15:53:33.397385 bi_etl-1.4/bi_etl/components/hst_table_source_based.py
--rw-r--r--   0        0        0    57029 2023-03-15 15:33:34.192481 bi_etl-1.4/bi_etl/components/readonlytable.py
--rw-r--r--   0        0        0       54 2021-09-27 17:13:33.000000 bi_etl-1.4/bi_etl/components/row/__init__.py
--rw-r--r--   0        0        0      456 2022-07-21 13:01:16.000000 bi_etl-1.4/bi_etl/components/row/cached_frozenset.py
--rw-r--r--   0        0        0      564 2022-07-21 13:01:16.000000 bi_etl-1.4/bi_etl/components/row/column_difference.py
--rw-r--r--   0        0        0    32775 2022-10-06 21:20:46.000000 bi_etl-1.4/bi_etl/components/row/row.py
--rw-r--r--   0        0        0     1661 2022-07-21 13:01:16.000000 bi_etl-1.4/bi_etl/components/row/row_case_insensitive.py
--rw-r--r--   0        0        0    25341 2023-03-15 15:32:32.540669 bi_etl-1.4/bi_etl/components/row/row_iteration_header.py
--rw-r--r--   0        0        0     4220 2022-07-21 13:01:16.000000 bi_etl-1.4/bi_etl/components/row/row_iteration_header_case_insensitive.py
--rw-r--r--   0        0        0      293 2022-07-21 13:01:16.000000 bi_etl-1.4/bi_etl/components/row/row_status.py
--rw-r--r--   0        0        0     3165 2022-07-21 13:01:16.000000 bi_etl-1.4/bi_etl/components/sqlquery.py
--rw-r--r--   0        0        0   164231 2023-03-15 15:33:43.015659 bi_etl-1.4/bi_etl/components/table.py
--rw-r--r--   0        0        0     8365 2022-07-21 13:01:16.000000 bi_etl-1.4/bi_etl/components/w3c_reader.py
--rw-r--r--   0        0        0     9820 2023-01-25 16:23:05.105369 bi_etl-1.4/bi_etl/components/xlsx_reader.py
--rw-r--r--   0        0        0    12007 2022-08-30 16:22:27.000000 bi_etl-1.4/bi_etl/components/xlsx_writer.py
--rw-r--r--   0        0        0        0 2022-07-21 13:01:16.000000 bi_etl-1.4/bi_etl/config/__init__.py
--rw-r--r--   0        0        0     1780 2022-07-21 13:01:16.000000 bi_etl-1.4/bi_etl/config/bi_etl_config_base.py
--rw-r--r--   0        0        0     3025 2023-03-15 15:33:34.244760 bi_etl-1.4/bi_etl/config/notifiers_config.py
--rw-r--r--   0        0        0      328 2022-07-21 13:01:16.000000 bi_etl-1.4/bi_etl/config/scheduler_config.py
--rw-r--r--   0        0        0    14301 2022-09-06 16:31:27.000000 bi_etl-1.4/bi_etl/conversions.py
--rw-r--r--   0        0        0      133 2021-09-27 17:13:34.000000 bi_etl-1.4/bi_etl/database/__init__.py
--rw-r--r--   0        0        0    17838 2023-03-15 15:29:36.687488 bi_etl-1.4/bi_etl/database/database_metadata.py
--rw-r--r--   0        0        0     1045 2022-07-21 13:01:16.000000 bi_etl-1.4/bi_etl/database/mock_database_metadata.py
--rw-r--r--   0        0        0     5699 2022-08-30 16:22:27.000000 bi_etl-1.4/bi_etl/example_config.ini
--rw-r--r--   0        0        0     5490 2022-08-30 16:22:27.000000 bi_etl-1.4/bi_etl/example_config_shared.ini
--rw-r--r--   0        0        0      923 2021-09-27 17:13:34.000000 bi_etl-1.4/bi_etl/exceptions/__init__.py
--rw-r--r--   0        0        0        0 2021-09-27 17:13:34.000000 bi_etl-1.4/bi_etl/informatica/__init__.py
--rw-r--r--   0        0        0       89 2022-07-21 13:01:17.000000 bi_etl-1.4/bi_etl/informatica/exceptions.py
--rw-r--r--   0        0        0      493 2022-07-21 13:01:17.000000 bi_etl-1.4/bi_etl/informatica/pm_config.py
--rw-r--r--   0        0        0     7540 2022-07-21 13:01:17.000000 bi_etl-1.4/bi_etl/informatica/pmcmd.py
--rw-r--r--   0        0        0     1219 2022-07-21 13:01:17.000000 bi_etl-1.4/bi_etl/informatica/pmcmd_task.py
--rw-r--r--   0        0        0    18054 2022-07-21 13:01:17.000000 bi_etl-1.4/bi_etl/informatica/pmrep.py
--rw-r--r--   0        0        0        0 2021-09-27 17:13:34.000000 bi_etl-1.4/bi_etl/lookups/__init__.py
--rw-r--r--   0        0        0    14159 2022-10-28 13:41:10.698113 bi_etl-1.4/bi_etl/lookups/autodisk_lookup.py
--rw-r--r--   0        0        0     3965 2022-07-21 13:01:17.000000 bi_etl-1.4/bi_etl/lookups/autodisk_range_lookup.py
--rw-r--r--   0        0        0     4699 2023-01-18 17:48:19.675169 bi_etl-1.4/bi_etl/lookups/disk_lookup.py
--rw-r--r--   0        0        0     1934 2022-07-21 13:01:17.000000 bi_etl-1.4/bi_etl/lookups/disk_range_lookup.py
--rw-r--r--   0        0        0    28901 2022-07-21 13:01:17.000000 bi_etl-1.4/bi_etl/lookups/lookup.py
--rw-r--r--   0        0        0     9926 2022-07-21 13:01:17.000000 bi_etl-1.4/bi_etl/lookups/non_unique_lookup.py
--rw-r--r--   0        0        0    12839 2022-07-21 13:01:17.000000 bi_etl-1.4/bi_etl/lookups/range_lookup.py
--rw-r--r--   0        0        0     3358 2022-07-21 13:01:17.000000 bi_etl-1.4/bi_etl/memory_size.py
--rw-r--r--   0        0        0      308 2022-07-21 13:01:17.000000 bi_etl-1.4/bi_etl/notifiers/__init__.py
--rw-r--r--   0        0        0     4323 2022-07-21 13:01:17.000000 bi_etl-1.4/bi_etl/notifiers/email.py
--rw-r--r--   0        0        0     8451 2022-07-21 20:01:17.000000 bi_etl-1.4/bi_etl/notifiers/jira.py
--rw-r--r--   0        0        0      379 2022-07-21 13:01:17.000000 bi_etl-1.4/bi_etl/notifiers/log_notifier.py
--rw-r--r--   0        0        0      706 2023-03-15 16:37:38.935207 bi_etl-1.4/bi_etl/notifiers/notifier_base.py
--rw-r--r--   0        0        0     6398 2023-03-15 16:37:38.986969 bi_etl-1.4/bi_etl/notifiers/slack.py
--rw-r--r--   0        0        0       61 2021-09-27 17:13:34.000000 bi_etl-1.4/bi_etl/parallel/__init__.py
--rw-r--r--   0        0        0        1 2022-07-21 13:01:17.000000 bi_etl-1.4/bi_etl/parallel/mp.py
--rw-r--r--   0        0        0        0 2021-09-27 17:13:34.000000 bi_etl-1.4/bi_etl/parameters/__init__.py
--rw-r--r--   0        0        0      956 2021-09-27 17:13:34.000000 bi_etl-1.4/bi_etl/parameters/file_parameter.py
--rw-r--r--   0        0        0       61 2021-09-27 17:13:34.000000 bi_etl-1.4/bi_etl/performance_test/__init__.py
--rw-r--r--   0        0        0     1071 2022-07-21 13:01:17.000000 bi_etl-1.4/bi_etl/performance_test/perftest_static_reader.py
--rw-r--r--   0        0        0        0 2021-09-27 17:13:34.000000 bi_etl-1.4/bi_etl/scheduler/__init__.py
--rw-r--r--   0        0        0     1737 2022-10-06 21:20:46.000000 bi_etl-1.4/bi_etl/scheduler/dependent_reasons.py
--rw-r--r--   0        0        0      706 2021-09-27 17:13:34.000000 bi_etl-1.4/bi_etl/scheduler/exceptions.py
--rw-r--r--   0        0        0     1853 2021-09-27 17:13:34.000000 bi_etl-1.4/bi_etl/scheduler/messages.py
--rw-r--r--   0        0        0    10430 2022-07-21 13:01:17.000000 bi_etl-1.4/bi_etl/scheduler/models.py
--rw-r--r--   0        0        0      672 2022-07-21 13:01:17.000000 bi_etl-1.4/bi_etl/scheduler/queue_io.py
--rw-r--r--   0        0        0      116 2021-09-27 17:13:34.000000 bi_etl-1.4/bi_etl/scheduler/run_scheduler.sh
--rw-r--r--   0        0        0      391 2021-09-27 17:13:34.000000 bi_etl-1.4/bi_etl/scheduler/run_scheduler_screen.sh
--rw-r--r--   0        0        0    65309 2022-10-06 21:20:46.000000 bi_etl-1.4/bi_etl/scheduler/scheduler.py
--rw-r--r--   0        0        0        0 2021-09-27 17:13:34.000000 bi_etl-1.4/bi_etl/scheduler/scheduler_etl_jobs/__init__.py
--rw-r--r--   0        0        0     2659 2022-07-21 13:01:17.000000 bi_etl-1.4/bi_etl/scheduler/scheduler_etl_jobs/etl_task_status_cd.py
--rw-r--r--   0        0        0    28623 2022-07-21 13:01:17.000000 bi_etl-1.4/bi_etl/scheduler/scheduler_interface.py
--rw-r--r--   0        0        0      444 2021-09-27 17:13:34.000000 bi_etl-1.4/bi_etl/scheduler/sdtout_queue.py
--rw-r--r--   0        0        0      688 2022-07-21 13:01:17.000000 bi_etl-1.4/bi_etl/scheduler/special_tasks.py
--rw-r--r--   0        0        0     2801 2022-07-21 13:01:17.000000 bi_etl-1.4/bi_etl/scheduler/status.py
--rw-r--r--   0        0        0    58023 2023-03-15 16:37:38.884897 bi_etl-1.4/bi_etl/scheduler/task.py
--rw-r--r--   0        0        0     7377 2022-10-31 20:23:08.644384 bi_etl-1.4/bi_etl/statement_queue.py
--rw-r--r--   0        0        0     6742 2022-07-21 13:01:17.000000 bi_etl-1.4/bi_etl/statistics.py
--rw-r--r--   0        0        0       61 2021-09-27 17:13:34.000000 bi_etl-1.4/bi_etl/test_notebooks/__init__.py
--rw-r--r--   0        0        0     1073 2022-06-09 14:18:34.000000 bi_etl-1.4/bi_etl/test_notebooks/perftest_static_reader.py
--rw-r--r--   0        0        0    17122 2022-05-12 15:44:59.000000 bi_etl-1.4/bi_etl/test_notebooks/Row performance.ipynb
--rw-r--r--   0        0        0     3509 2022-05-12 15:44:59.000000 bi_etl-1.4/bi_etl/test_notebooks/Utility Test.ipynb
--rw-r--r--   0        0        0     4343 2021-09-27 17:13:34.000000 bi_etl-1.4/bi_etl/timer.py
--rw-r--r--   0        0        0    11366 2022-07-21 13:01:17.000000 bi_etl-1.4/bi_etl/utility/__init__.py
--rw-r--r--   0        0        0     2118 2022-07-21 13:01:17.000000 bi_etl-1.4/bi_etl/utility/ask.py
--rw-r--r--   0        0        0     8976 2023-01-18 17:48:19.758841 bi_etl-1.4/bi_etl/utility/bcp_helpers.py
--rw-r--r--   0        0        0      925 2021-09-27 17:13:34.000000 bi_etl-1.4/bi_etl/utility/case_insentive_set.py
--rw-r--r--   0        0        0     1869 2022-07-21 13:01:17.000000 bi_etl-1.4/bi_etl/utility/copy_table_data.py
--rw-r--r--   0        0        0     5000 2022-07-21 13:01:17.000000 bi_etl-1.4/bi_etl/utility/line_counter.py
--rw-r--r--   0        0        0      472 2021-09-27 17:13:34.000000 bi_etl-1.4/bi_etl/utility/logging_helpers.py
--rw-r--r--   0        0        0      947 2022-07-21 13:01:17.000000 bi_etl-1.4/bi_etl/utility/package_root.py
--rw-r--r--   0        0        0       61 2021-09-27 17:13:34.000000 bi_etl-1.4/bi_etl/utility/postgresql/__init__.py
--rw-r--r--   0        0        0     3686 2023-01-18 17:48:19.844889 bi_etl-1.4/bi_etl/utility/postgresql/psql_command.py
--rw-r--r--   0        0        0     4777 2022-10-06 20:52:27.000000 bi_etl-1.4/bi_etl/utility/postgresql/psycopg2_helpers.py
--rw-r--r--   0        0        0    11998 2023-03-15 15:33:34.410960 bi_etl-1.4/bi_etl/utility/run_sql_script.py
--rw-r--r--   0        0        0       61 2021-09-27 17:13:34.000000 bi_etl-1.4/bi_etl/utility/sql_server/__init__.py
--rw-r--r--   0        0        0     2778 2022-10-06 21:17:15.000000 bi_etl-1.4/bi_etl/utility/sql_server/defrag_indexes.py
--rw-r--r--   0        0        0     4674 2022-07-21 13:01:17.000000 bi_etl-1.4/bi_etl/utility/ssh_forward.py
--rw-r--r--   0        0        0      341 2022-07-21 13:01:17.000000 bi_etl-1.4/bi_etl/version.py
--rw-r--r--   0        0        0     1086 2020-06-29 20:22:28.000000 bi_etl-1.4/license.txt
--rw-r--r--   0        0        0     2099 2023-03-15 15:32:32.432042 bi_etl-1.4/pyproject.toml
--rw-r--r--   0        0        0     1251 2022-10-06 21:20:46.000000 bi_etl-1.4/README.md
--rw-r--r--   0        0        0     2823 1970-01-01 00:00:00.000000 bi_etl-1.4/setup.py
--rw-r--r--   0        0        0     3029 1970-01-01 00:00:00.000000 bi_etl-1.4/PKG-INFO
+-rw-r--r--   0        0        0      628 2021-09-27 17:13:33.000000 bi_etl-1.4.2/bi_etl/.coveragerc
+-rw-r--r--   0        0        0      360 2021-09-27 17:13:33.000000 bi_etl-1.4.2/bi_etl/.project
+-rw-r--r--   0        0        0      423 2021-09-27 17:13:33.000000 bi_etl-1.4.2/bi_etl/.pydevproject
+-rw-r--r--   0        0        0     3529 2021-09-27 17:13:33.000000 bi_etl-1.4.2/bi_etl/.pylintrc
+-rw-r--r--   0        0        0      104 2022-07-21 13:01:16.000000 bi_etl-1.4.2/bi_etl/__init__.py
+-rw-r--r--   0        0        0     2612 2022-07-21 13:01:16.000000 bi_etl-1.4.2/bi_etl/__main__.py
+-rw-r--r--   0        0        0       61 2022-07-21 13:01:16.000000 bi_etl-1.4.2/bi_etl/boto3_helper/__init__.py
+-rw-r--r--   0        0        0     1664 2022-07-21 13:01:16.000000 bi_etl-1.4.2/bi_etl/boto3_helper/dynamodb.py
+-rw-r--r--   0        0        0      148 2022-07-21 13:01:16.000000 bi_etl-1.4.2/bi_etl/boto3_helper/lambdas.py
+-rw-r--r--   0        0        0    12181 2022-08-11 15:34:45.000000 bi_etl-1.4.2/bi_etl/boto3_helper/s3.py
+-rw-r--r--   0        0        0     1905 2022-07-21 13:01:16.000000 bi_etl-1.4.2/bi_etl/boto3_helper/session.py
+-rw-r--r--   0        0        0      142 2022-07-21 13:01:16.000000 bi_etl-1.4.2/bi_etl/boto3_helper/ssm.py
+-rw-r--r--   0        0        0        0 2021-09-27 17:13:33.000000 bi_etl-1.4.2/bi_etl/bulk_loaders/__init__.py
+-rw-r--r--   0        0        0     6756 2023-03-15 15:53:33.483857 bi_etl-1.4.2/bi_etl/bulk_loaders/bulk_loader.py
+-rw-r--r--   0        0        0      982 2021-09-27 17:13:33.000000 bi_etl-1.4.2/bi_etl/bulk_loaders/bulk_loader_exception.py
+-rw-r--r--   0        0        0      323 2022-10-06 20:54:25.000000 bi_etl-1.4.2/bi_etl/bulk_loaders/postgresql_bulk_load_config.py
+-rw-r--r--   0        0        0     3759 2023-01-18 17:48:19.693841 bi_etl-1.4.2/bi_etl/bulk_loaders/postgresql_copy.py
+-rw-r--r--   0        0        0     6299 2023-01-18 17:48:19.786858 bi_etl-1.4.2/bi_etl/bulk_loaders/redshift_s3_avro_loader.py
+-rw-r--r--   0        0        0    14049 2023-03-23 20:50:09.146143 bi_etl-1.4.2/bi_etl/bulk_loaders/redshift_s3_base.py
+-rw-r--r--   0        0        0    11775 2023-01-18 17:48:19.808886 bi_etl-1.4.2/bi_etl/bulk_loaders/redshift_s3_csv_loader.py
+-rw-r--r--   0        0        0     4081 2023-01-18 17:48:19.827968 bi_etl-1.4.2/bi_etl/bulk_loaders/redshift_s3_json_loader.py
+-rw-r--r--   0        0        0     6335 2023-01-18 17:48:19.714844 bi_etl-1.4.2/bi_etl/bulk_loaders/redshift_s3_parquet_loader.py
+-rw-r--r--   0        0        0     1063 2023-01-10 02:14:59.086394 bi_etl-1.4.2/bi_etl/bulk_loaders/s3_bulk_load_config.py
+-rw-r--r--   0        0        0     4821 2023-01-18 17:48:19.735841 bi_etl-1.4.2/bi_etl/bulk_loaders/sql_server_bcp.py
+-rw-r--r--   0        0        0        0 2021-09-27 17:13:33.000000 bi_etl-1.4.2/bi_etl/components/__init__.py
+-rw-r--r--   0        0        0    16109 2022-10-06 21:12:48.000000 bi_etl-1.4.2/bi_etl/components/csv_writer.py
+-rw-r--r--   0        0        0    17630 2022-08-24 15:21:41.000000 bi_etl-1.4.2/bi_etl/components/csvreader.py
+-rw-r--r--   0        0        0    19384 2022-07-21 13:01:16.000000 bi_etl-1.4.2/bi_etl/components/data_analyzer.py
+-rw-r--r--   0        0        0    52067 2022-10-31 19:45:21.367328 bi_etl-1.4.2/bi_etl/components/etlcomponent.py
+-rw-r--r--   0        0        0       61 2021-09-27 17:13:33.000000 bi_etl-1.4.2/bi_etl/components/get_next_key/__init__.py
+-rw-r--r--   0        0        0      873 2022-05-04 02:21:27.000000 bi_etl-1.4.2/bi_etl/components/get_next_key/base_table_memory.py
+-rw-r--r--   0        0        0      644 2021-09-27 17:13:33.000000 bi_etl-1.4.2/bi_etl/components/get_next_key/local_table_memory.py
+-rw-r--r--   0        0        0     2047 2022-06-06 16:22:38.000000 bi_etl-1.4.2/bi_etl/components/get_next_key/shared_table_memory.py
+-rw-r--r--   0        0        0      708 2021-09-27 17:13:33.000000 bi_etl-1.4.2/bi_etl/components/get_next_key/shared_table_memory_manager.py
+-rw-r--r--   0        0        0   107458 2023-03-15 15:33:34.268035 bi_etl-1.4.2/bi_etl/components/hst_table.py
+-rw-r--r--   0        0        0    42645 2023-03-15 15:53:33.397385 bi_etl-1.4.2/bi_etl/components/hst_table_source_based.py
+-rw-r--r--   0        0        0    57029 2023-03-15 15:33:34.192481 bi_etl-1.4.2/bi_etl/components/readonlytable.py
+-rw-r--r--   0        0        0       54 2021-09-27 17:13:33.000000 bi_etl-1.4.2/bi_etl/components/row/__init__.py
+-rw-r--r--   0        0        0      456 2022-07-21 13:01:16.000000 bi_etl-1.4.2/bi_etl/components/row/cached_frozenset.py
+-rw-r--r--   0        0        0      564 2022-07-21 13:01:16.000000 bi_etl-1.4.2/bi_etl/components/row/column_difference.py
+-rw-r--r--   0        0        0    32775 2022-10-06 21:20:46.000000 bi_etl-1.4.2/bi_etl/components/row/row.py
+-rw-r--r--   0        0        0     1661 2022-07-21 13:01:16.000000 bi_etl-1.4.2/bi_etl/components/row/row_case_insensitive.py
+-rw-r--r--   0        0        0    25341 2023-03-15 15:32:32.540669 bi_etl-1.4.2/bi_etl/components/row/row_iteration_header.py
+-rw-r--r--   0        0        0     4220 2022-07-21 13:01:16.000000 bi_etl-1.4.2/bi_etl/components/row/row_iteration_header_case_insensitive.py
+-rw-r--r--   0        0        0      293 2022-07-21 13:01:16.000000 bi_etl-1.4.2/bi_etl/components/row/row_status.py
+-rw-r--r--   0        0        0     3165 2022-07-21 13:01:16.000000 bi_etl-1.4.2/bi_etl/components/sqlquery.py
+-rw-r--r--   0        0        0   164231 2023-03-15 15:33:43.015659 bi_etl-1.4.2/bi_etl/components/table.py
+-rw-r--r--   0        0        0     8365 2022-07-21 13:01:16.000000 bi_etl-1.4.2/bi_etl/components/w3c_reader.py
+-rw-r--r--   0        0        0     9820 2023-01-25 16:23:05.105369 bi_etl-1.4.2/bi_etl/components/xlsx_reader.py
+-rw-r--r--   0        0        0    12007 2022-08-30 16:22:27.000000 bi_etl-1.4.2/bi_etl/components/xlsx_writer.py
+-rw-r--r--   0        0        0        0 2022-07-21 13:01:16.000000 bi_etl-1.4.2/bi_etl/config/__init__.py
+-rw-r--r--   0        0        0     1780 2022-07-21 13:01:16.000000 bi_etl-1.4.2/bi_etl/config/bi_etl_config_base.py
+-rw-r--r--   0        0        0     3025 2023-03-15 15:33:34.244760 bi_etl-1.4.2/bi_etl/config/notifiers_config.py
+-rw-r--r--   0        0        0      328 2022-07-21 13:01:16.000000 bi_etl-1.4.2/bi_etl/config/scheduler_config.py
+-rw-r--r--   0        0        0    14301 2022-09-06 16:31:27.000000 bi_etl-1.4.2/bi_etl/conversions.py
+-rw-r--r--   0        0        0      133 2021-09-27 17:13:34.000000 bi_etl-1.4.2/bi_etl/database/__init__.py
+-rw-r--r--   0        0        0    17838 2023-03-21 14:17:46.169530 bi_etl-1.4.2/bi_etl/database/database_metadata.py
+-rw-r--r--   0        0        0     1045 2022-07-21 13:01:16.000000 bi_etl-1.4.2/bi_etl/database/mock_database_metadata.py
+-rw-r--r--   0        0        0     5699 2022-08-30 16:22:27.000000 bi_etl-1.4.2/bi_etl/example_config.ini
+-rw-r--r--   0        0        0     5490 2022-08-30 16:22:27.000000 bi_etl-1.4.2/bi_etl/example_config_shared.ini
+-rw-r--r--   0        0        0      923 2021-09-27 17:13:34.000000 bi_etl-1.4.2/bi_etl/exceptions/__init__.py
+-rw-r--r--   0        0        0        0 2021-09-27 17:13:34.000000 bi_etl-1.4.2/bi_etl/informatica/__init__.py
+-rw-r--r--   0        0        0       89 2022-07-21 13:01:17.000000 bi_etl-1.4.2/bi_etl/informatica/exceptions.py
+-rw-r--r--   0        0        0      493 2022-07-21 13:01:17.000000 bi_etl-1.4.2/bi_etl/informatica/pm_config.py
+-rw-r--r--   0        0        0     7540 2022-07-21 13:01:17.000000 bi_etl-1.4.2/bi_etl/informatica/pmcmd.py
+-rw-r--r--   0        0        0     1219 2022-07-21 13:01:17.000000 bi_etl-1.4.2/bi_etl/informatica/pmcmd_task.py
+-rw-r--r--   0        0        0    18054 2022-07-21 13:01:17.000000 bi_etl-1.4.2/bi_etl/informatica/pmrep.py
+-rw-r--r--   0        0        0        0 2021-09-27 17:13:34.000000 bi_etl-1.4.2/bi_etl/lookups/__init__.py
+-rw-r--r--   0        0        0    14159 2022-10-28 13:41:10.698113 bi_etl-1.4.2/bi_etl/lookups/autodisk_lookup.py
+-rw-r--r--   0        0        0     3965 2022-07-21 13:01:17.000000 bi_etl-1.4.2/bi_etl/lookups/autodisk_range_lookup.py
+-rw-r--r--   0        0        0     4699 2023-01-18 17:48:19.675169 bi_etl-1.4.2/bi_etl/lookups/disk_lookup.py
+-rw-r--r--   0        0        0     1934 2022-07-21 13:01:17.000000 bi_etl-1.4.2/bi_etl/lookups/disk_range_lookup.py
+-rw-r--r--   0        0        0    28901 2022-07-21 13:01:17.000000 bi_etl-1.4.2/bi_etl/lookups/lookup.py
+-rw-r--r--   0        0        0     9926 2022-07-21 13:01:17.000000 bi_etl-1.4.2/bi_etl/lookups/non_unique_lookup.py
+-rw-r--r--   0        0        0    12839 2022-07-21 13:01:17.000000 bi_etl-1.4.2/bi_etl/lookups/range_lookup.py
+-rw-r--r--   0        0        0     3358 2022-07-21 13:01:17.000000 bi_etl-1.4.2/bi_etl/memory_size.py
+-rw-r--r--   0        0        0      308 2022-07-21 13:01:17.000000 bi_etl-1.4.2/bi_etl/notifiers/__init__.py
+-rw-r--r--   0        0        0     4323 2022-07-21 13:01:17.000000 bi_etl-1.4.2/bi_etl/notifiers/email.py
+-rw-r--r--   0        0        0     8451 2022-07-21 20:01:17.000000 bi_etl-1.4.2/bi_etl/notifiers/jira.py
+-rw-r--r--   0        0        0      379 2022-07-21 13:01:17.000000 bi_etl-1.4.2/bi_etl/notifiers/log_notifier.py
+-rw-r--r--   0        0        0      706 2023-03-15 16:37:38.935207 bi_etl-1.4.2/bi_etl/notifiers/notifier_base.py
+-rw-r--r--   0        0        0     6398 2023-03-15 16:37:38.986969 bi_etl-1.4.2/bi_etl/notifiers/slack.py
+-rw-r--r--   0        0        0       61 2021-09-27 17:13:34.000000 bi_etl-1.4.2/bi_etl/parallel/__init__.py
+-rw-r--r--   0        0        0        1 2022-07-21 13:01:17.000000 bi_etl-1.4.2/bi_etl/parallel/mp.py
+-rw-r--r--   0        0        0        0 2021-09-27 17:13:34.000000 bi_etl-1.4.2/bi_etl/parameters/__init__.py
+-rw-r--r--   0        0        0      956 2021-09-27 17:13:34.000000 bi_etl-1.4.2/bi_etl/parameters/file_parameter.py
+-rw-r--r--   0        0        0       61 2021-09-27 17:13:34.000000 bi_etl-1.4.2/bi_etl/performance_test/__init__.py
+-rw-r--r--   0        0        0     1071 2022-07-21 13:01:17.000000 bi_etl-1.4.2/bi_etl/performance_test/perftest_static_reader.py
+-rw-r--r--   0        0        0        0 2021-09-27 17:13:34.000000 bi_etl-1.4.2/bi_etl/scheduler/__init__.py
+-rw-r--r--   0        0        0     1737 2022-10-06 21:20:46.000000 bi_etl-1.4.2/bi_etl/scheduler/dependent_reasons.py
+-rw-r--r--   0        0        0      706 2021-09-27 17:13:34.000000 bi_etl-1.4.2/bi_etl/scheduler/exceptions.py
+-rw-r--r--   0        0        0     1853 2021-09-27 17:13:34.000000 bi_etl-1.4.2/bi_etl/scheduler/messages.py
+-rw-r--r--   0        0        0    10430 2022-07-21 13:01:17.000000 bi_etl-1.4.2/bi_etl/scheduler/models.py
+-rw-r--r--   0        0        0      672 2022-07-21 13:01:17.000000 bi_etl-1.4.2/bi_etl/scheduler/queue_io.py
+-rw-r--r--   0        0        0      116 2021-09-27 17:13:34.000000 bi_etl-1.4.2/bi_etl/scheduler/run_scheduler.sh
+-rw-r--r--   0        0        0      391 2021-09-27 17:13:34.000000 bi_etl-1.4.2/bi_etl/scheduler/run_scheduler_screen.sh
+-rw-r--r--   0        0        0    65309 2022-10-06 21:20:46.000000 bi_etl-1.4.2/bi_etl/scheduler/scheduler.py
+-rw-r--r--   0        0        0        0 2021-09-27 17:13:34.000000 bi_etl-1.4.2/bi_etl/scheduler/scheduler_etl_jobs/__init__.py
+-rw-r--r--   0        0        0     2659 2022-07-21 13:01:17.000000 bi_etl-1.4.2/bi_etl/scheduler/scheduler_etl_jobs/etl_task_status_cd.py
+-rw-r--r--   0        0        0    28623 2022-07-21 13:01:17.000000 bi_etl-1.4.2/bi_etl/scheduler/scheduler_interface.py
+-rw-r--r--   0        0        0      444 2021-09-27 17:13:34.000000 bi_etl-1.4.2/bi_etl/scheduler/sdtout_queue.py
+-rw-r--r--   0        0        0      688 2022-07-21 13:01:17.000000 bi_etl-1.4.2/bi_etl/scheduler/special_tasks.py
+-rw-r--r--   0        0        0     2801 2022-07-21 13:01:17.000000 bi_etl-1.4.2/bi_etl/scheduler/status.py
+-rw-r--r--   0        0        0    57835 2023-06-27 14:21:39.760133 bi_etl-1.4.2/bi_etl/scheduler/task.py
+-rw-r--r--   0        0        0     7377 2022-10-31 20:23:08.644384 bi_etl-1.4.2/bi_etl/statement_queue.py
+-rw-r--r--   0        0        0     6742 2022-07-21 13:01:17.000000 bi_etl-1.4.2/bi_etl/statistics.py
+-rw-r--r--   0        0        0       61 2021-09-27 17:13:34.000000 bi_etl-1.4.2/bi_etl/test_notebooks/__init__.py
+-rw-r--r--   0        0        0     1073 2022-06-09 14:18:34.000000 bi_etl-1.4.2/bi_etl/test_notebooks/perftest_static_reader.py
+-rw-r--r--   0        0        0    17122 2022-05-12 15:44:59.000000 bi_etl-1.4.2/bi_etl/test_notebooks/Row performance.ipynb
+-rw-r--r--   0        0        0     3509 2022-05-12 15:44:59.000000 bi_etl-1.4.2/bi_etl/test_notebooks/Utility Test.ipynb
+-rw-r--r--   0        0        0     4343 2021-09-27 17:13:34.000000 bi_etl-1.4.2/bi_etl/timer.py
+-rw-r--r--   0        0        0    11366 2022-07-21 13:01:17.000000 bi_etl-1.4.2/bi_etl/utility/__init__.py
+-rw-r--r--   0        0        0     2118 2022-07-21 13:01:17.000000 bi_etl-1.4.2/bi_etl/utility/ask.py
+-rw-r--r--   0        0        0     8976 2023-01-18 17:48:19.758841 bi_etl-1.4.2/bi_etl/utility/bcp_helpers.py
+-rw-r--r--   0        0        0      925 2021-09-27 17:13:34.000000 bi_etl-1.4.2/bi_etl/utility/case_insentive_set.py
+-rw-r--r--   0        0        0     1869 2022-07-21 13:01:17.000000 bi_etl-1.4.2/bi_etl/utility/copy_table_data.py
+-rw-r--r--   0        0        0     5000 2022-07-21 13:01:17.000000 bi_etl-1.4.2/bi_etl/utility/line_counter.py
+-rw-r--r--   0        0        0      472 2021-09-27 17:13:34.000000 bi_etl-1.4.2/bi_etl/utility/logging_helpers.py
+-rw-r--r--   0        0        0      947 2022-07-21 13:01:17.000000 bi_etl-1.4.2/bi_etl/utility/package_root.py
+-rw-r--r--   0        0        0       61 2021-09-27 17:13:34.000000 bi_etl-1.4.2/bi_etl/utility/postgresql/__init__.py
+-rw-r--r--   0        0        0     3686 2023-01-18 17:48:19.844889 bi_etl-1.4.2/bi_etl/utility/postgresql/psql_command.py
+-rw-r--r--   0        0        0     4777 2022-10-06 20:52:27.000000 bi_etl-1.4.2/bi_etl/utility/postgresql/psycopg2_helpers.py
+-rw-r--r--   0        0        0    11998 2023-03-15 15:33:34.410960 bi_etl-1.4.2/bi_etl/utility/run_sql_script.py
+-rw-r--r--   0        0        0       61 2021-09-27 17:13:34.000000 bi_etl-1.4.2/bi_etl/utility/sql_server/__init__.py
+-rw-r--r--   0        0        0     2776 2023-06-27 14:01:47.122835 bi_etl-1.4.2/bi_etl/utility/sql_server/defrag_indexes.py
+-rw-r--r--   0        0        0     4674 2022-07-21 13:01:17.000000 bi_etl-1.4.2/bi_etl/utility/ssh_forward.py
+-rw-r--r--   0        0        0      341 2022-07-21 13:01:17.000000 bi_etl-1.4.2/bi_etl/version.py
+-rw-r--r--   0        0        0     1086 2020-06-29 20:22:28.000000 bi_etl-1.4.2/license.txt
+-rw-r--r--   0        0        0     2009 2023-07-05 15:24:56.841691 bi_etl-1.4.2/pyproject.toml
+-rw-r--r--   0        0        0     1251 2022-10-06 21:20:46.000000 bi_etl-1.4.2/README.md
+-rw-r--r--   0        0        0     2975 1970-01-01 00:00:00.000000 bi_etl-1.4.2/PKG-INFO
```

### Comparing `bi_etl-1.4/bi_etl/.coveragerc` & `bi_etl-1.4.2/bi_etl/.coveragerc`

 * *Files identical despite different names*

### Comparing `bi_etl-1.4/bi_etl/.pylintrc` & `bi_etl-1.4.2/bi_etl/.pylintrc`

 * *Files identical despite different names*

### Comparing `bi_etl-1.4/bi_etl/__main__.py` & `bi_etl-1.4.2/bi_etl/__main__.py`

 * *Files identical despite different names*

### Comparing `bi_etl-1.4/bi_etl/boto3_helper/dynamodb.py` & `bi_etl-1.4.2/bi_etl/boto3_helper/dynamodb.py`

 * *Files identical despite different names*

### Comparing `bi_etl-1.4/bi_etl/boto3_helper/s3.py` & `bi_etl-1.4.2/bi_etl/boto3_helper/s3.py`

 * *Files identical despite different names*

### Comparing `bi_etl-1.4/bi_etl/boto3_helper/session.py` & `bi_etl-1.4.2/bi_etl/boto3_helper/session.py`

 * *Files identical despite different names*

### Comparing `bi_etl-1.4/bi_etl/bulk_loaders/bulk_loader.py` & `bi_etl-1.4.2/bi_etl/bulk_loaders/bulk_loader.py`

 * *Files identical despite different names*

### Comparing `bi_etl-1.4/bi_etl/bulk_loaders/bulk_loader_exception.py` & `bi_etl-1.4.2/bi_etl/bulk_loaders/bulk_loader_exception.py`

 * *Files identical despite different names*

### Comparing `bi_etl-1.4/bi_etl/bulk_loaders/postgresql_copy.py` & `bi_etl-1.4.2/bi_etl/bulk_loaders/postgresql_copy.py`

 * *Files identical despite different names*

### Comparing `bi_etl-1.4/bi_etl/bulk_loaders/redshift_s3_avro_loader.py` & `bi_etl-1.4.2/bi_etl/bulk_loaders/redshift_s3_avro_loader.py`

 * *Files identical despite different names*

### Comparing `bi_etl-1.4/bi_etl/bulk_loaders/redshift_s3_base.py` & `bi_etl-1.4.2/bi_etl/bulk_loaders/redshift_s3_base.py`

 * *Files 4% similar despite different names*

```diff
@@ -5,14 +5,15 @@
 import textwrap
 import time
 from pathlib import Path
 from typing import *
 
 import boto3
 import sqlalchemy
+from sqlalchemy import text
 
 from bi_etl.bulk_loaders.bulk_loader import BulkLoader
 from bi_etl.bulk_loaders.bulk_loader_exception import BulkLoaderException
 from bi_etl.bulk_loaders.s3_bulk_load_config import S3_Bulk_Loader_Config
 from bi_etl.conversions import strip
 
 if TYPE_CHECKING:
@@ -118,29 +119,47 @@
                         response = self.bucket.Object(s3_path).get()
 
         self.log.info(f"Uploaded {total_size:,} bytes in total to {s3_full_folder}")
         return s3_files
 
     def _get_error_details(
             self,
+            connection: sqlalchemy.engine.base.Connection,
             table_object: Table,
             exception: sqlalchemy.exc.SQLAlchemyError
     ) -> BulkLoaderException:
         bulk_loader_exception = BulkLoaderException(exception, password=self.s3_password)
 
-        sql = f"""
+        self.log.debug(f'Getting pg_last_copy_id')
+
+        pg_last_copy_id_res = connection.execute("select pg_last_copy_id() as id")
+        pg_last_copy_id_row = next(pg_last_copy_id_res)
+        pg_last_copy_id = pg_last_copy_id_row.id
+
+        self.log.error(f'pg_last_copy_id = {pg_last_copy_id}')
+
+        if pg_last_copy_id != -1:
+            sql = """
                     SELECT *
                     FROM stl_load_errors
                     WHERE query = pg_last_copy_id()
                     ORDER BY starttime DESC
-                    """
+                  """
+        else:
+            self.log.error(f"Unable to use pg_last_copy_id()")
+            sql = f"""
+                    SELECT TOP 1 *
+                    FROM stl_load_errors
+                    WHERE filename like '%{table_object.table_name}%'
+                    ORDER BY starttime DESC
+                   """
 
         self.log.error(f'Checking stl_load_errors with\n{sql}')
         try:
-            results = table_object.execute(sql)
+            results = connection.execute(text(sql))
         except Exception as e2:
             bulk_loader_exception.add_error(f'Error {e2} when getting stl_load_errors contents')
             results = []
         rows_found = 0
         for row in results:
             rows_found += 1
             filename = strip(row.filename)
@@ -176,67 +195,68 @@
 
         keep_trying = True
         wait_seconds = 15
         t_end = time.time() + wait_seconds
 
         while keep_trying:
             try:
-                table_object.execute(copy_sql)
+                connection = table_object.connection()
+                connection.execute(copy_sql)
                 # Load worked we can stop looping
                 keep_trying = False
+                connection.execute(f"COMMIT;")
             except sqlalchemy.exc.SQLAlchemyError as e:
                 safe_e = str(e).replace(self.s3_password, '*' * 8)
 
                 # Check if the error is non-recoverable
                 if any(error in str(e) for error in self.non_recoverable_error_matches):
                     self.log.error(f"Cannot recover from this error - {safe_e}")
                     raise
 
                 self.log.error('!' * 80)
                 self.log.error(f'!! Details for {safe_e} below:')
                 self.log.error('!' * 80)
 
                 bulk_loader_exception = self._get_error_details(
+                    connection=connection,
                     table_object=table_object,
                     exception=e,
                 )
 
                 if 'S3ServiceException' in str(e):
                     if time.time() > t_end:
                         self.log.info(f'{wait_seconds} seconds wait is over. File cannot be loaded. {t_end}')
                         keep_trying = False
                     self.log.info(f'Will retry in 5 seconds file copy after S3ServiceException failure - {safe_e}')
                     time.sleep(5)
                 else:
                     raise bulk_loader_exception
 
-        # TODO: Consider removing this commit the called should do that.
-        #       However, requires extensive testing
-        table_object.execute(f"COMMIT;")
-
         sql = f"""
         SELECT SUM(lines_scanned) as lines_scanned, count(DISTINCT filename) as file_cnt
         FROM stl_load_commits
         WHERE query = pg_last_copy_id()
         """
         # Default to -1 rows to indicate error
         rows_loaded = -1
         try:
-            results = table_object.execute(sql)
+            results = connection.execute(sql)
             for row in results:
                 lines_scanned = row.lines_scanned
                 file_cnt = row.file_cnt
                 if self.lines_scanned_modifier == 0:
                     rows_loaded = lines_scanned
                 else:
                     rows_loaded = lines_scanned + (self.lines_scanned_modifier * file_cnt)
         except Exception as e:
             e = str(e).replace(self.s3_password, '*' * 8)
             self.log.warning(f"Error getting row count: {e}")
 
+        connection.close()
+
         return rows_loaded
 
     def get_copy_sql(
             self,
             s3_source_path: str,
             table_to_load: str,
             file_compression: str = '',
```

### Comparing `bi_etl-1.4/bi_etl/bulk_loaders/redshift_s3_csv_loader.py` & `bi_etl-1.4.2/bi_etl/bulk_loaders/redshift_s3_csv_loader.py`

 * *Files identical despite different names*

### Comparing `bi_etl-1.4/bi_etl/bulk_loaders/redshift_s3_json_loader.py` & `bi_etl-1.4.2/bi_etl/bulk_loaders/redshift_s3_json_loader.py`

 * *Files identical despite different names*

### Comparing `bi_etl-1.4/bi_etl/bulk_loaders/redshift_s3_parquet_loader.py` & `bi_etl-1.4.2/bi_etl/bulk_loaders/redshift_s3_parquet_loader.py`

 * *Files identical despite different names*

### Comparing `bi_etl-1.4/bi_etl/bulk_loaders/s3_bulk_load_config.py` & `bi_etl-1.4.2/bi_etl/bulk_loaders/s3_bulk_load_config.py`

 * *Files identical despite different names*

### Comparing `bi_etl-1.4/bi_etl/bulk_loaders/sql_server_bcp.py` & `bi_etl-1.4.2/bi_etl/bulk_loaders/sql_server_bcp.py`

 * *Files identical despite different names*

### Comparing `bi_etl-1.4/bi_etl/components/csv_writer.py` & `bi_etl-1.4.2/bi_etl/components/csv_writer.py`

 * *Files identical despite different names*

### Comparing `bi_etl-1.4/bi_etl/components/csvreader.py` & `bi_etl-1.4.2/bi_etl/components/csvreader.py`

 * *Files identical despite different names*

### Comparing `bi_etl-1.4/bi_etl/components/data_analyzer.py` & `bi_etl-1.4.2/bi_etl/components/data_analyzer.py`

 * *Files identical despite different names*

### Comparing `bi_etl-1.4/bi_etl/components/etlcomponent.py` & `bi_etl-1.4.2/bi_etl/components/etlcomponent.py`

 * *Files identical despite different names*

### Comparing `bi_etl-1.4/bi_etl/components/get_next_key/base_table_memory.py` & `bi_etl-1.4.2/bi_etl/components/get_next_key/base_table_memory.py`

 * *Files identical despite different names*

### Comparing `bi_etl-1.4/bi_etl/components/get_next_key/local_table_memory.py` & `bi_etl-1.4.2/bi_etl/components/get_next_key/local_table_memory.py`

 * *Files identical despite different names*

### Comparing `bi_etl-1.4/bi_etl/components/get_next_key/shared_table_memory.py` & `bi_etl-1.4.2/bi_etl/components/get_next_key/shared_table_memory.py`

 * *Files identical despite different names*

### Comparing `bi_etl-1.4/bi_etl/components/get_next_key/shared_table_memory_manager.py` & `bi_etl-1.4.2/bi_etl/components/get_next_key/shared_table_memory_manager.py`

 * *Files identical despite different names*

### Comparing `bi_etl-1.4/bi_etl/components/hst_table.py` & `bi_etl-1.4.2/bi_etl/components/hst_table.py`

 * *Files identical despite different names*

### Comparing `bi_etl-1.4/bi_etl/components/hst_table_source_based.py` & `bi_etl-1.4.2/bi_etl/components/hst_table_source_based.py`

 * *Files identical despite different names*

### Comparing `bi_etl-1.4/bi_etl/components/readonlytable.py` & `bi_etl-1.4.2/bi_etl/components/readonlytable.py`

 * *Files identical despite different names*

### Comparing `bi_etl-1.4/bi_etl/components/row/column_difference.py` & `bi_etl-1.4.2/bi_etl/components/row/column_difference.py`

 * *Files identical despite different names*

### Comparing `bi_etl-1.4/bi_etl/components/row/row.py` & `bi_etl-1.4.2/bi_etl/components/row/row.py`

 * *Files identical despite different names*

### Comparing `bi_etl-1.4/bi_etl/components/row/row_case_insensitive.py` & `bi_etl-1.4.2/bi_etl/components/row/row_case_insensitive.py`

 * *Files identical despite different names*

### Comparing `bi_etl-1.4/bi_etl/components/row/row_iteration_header.py` & `bi_etl-1.4.2/bi_etl/components/row/row_iteration_header.py`

 * *Files identical despite different names*

### Comparing `bi_etl-1.4/bi_etl/components/row/row_iteration_header_case_insensitive.py` & `bi_etl-1.4.2/bi_etl/components/row/row_iteration_header_case_insensitive.py`

 * *Files identical despite different names*

### Comparing `bi_etl-1.4/bi_etl/components/sqlquery.py` & `bi_etl-1.4.2/bi_etl/components/sqlquery.py`

 * *Files identical despite different names*

### Comparing `bi_etl-1.4/bi_etl/components/table.py` & `bi_etl-1.4.2/bi_etl/components/table.py`

 * *Files identical despite different names*

### Comparing `bi_etl-1.4/bi_etl/components/w3c_reader.py` & `bi_etl-1.4.2/bi_etl/components/w3c_reader.py`

 * *Files identical despite different names*

### Comparing `bi_etl-1.4/bi_etl/components/xlsx_reader.py` & `bi_etl-1.4.2/bi_etl/components/xlsx_reader.py`

 * *Files identical despite different names*

### Comparing `bi_etl-1.4/bi_etl/components/xlsx_writer.py` & `bi_etl-1.4.2/bi_etl/components/xlsx_writer.py`

 * *Files identical despite different names*

### Comparing `bi_etl-1.4/bi_etl/config/bi_etl_config_base.py` & `bi_etl-1.4.2/bi_etl/config/bi_etl_config_base.py`

 * *Files identical despite different names*

### Comparing `bi_etl-1.4/bi_etl/config/notifiers_config.py` & `bi_etl-1.4.2/bi_etl/config/notifiers_config.py`

 * *Files identical despite different names*

### Comparing `bi_etl-1.4/bi_etl/conversions.py` & `bi_etl-1.4.2/bi_etl/conversions.py`

 * *Files identical despite different names*

### Comparing `bi_etl-1.4/bi_etl/database/database_metadata.py` & `bi_etl-1.4.2/bi_etl/database/database_metadata.py`

 * *Files 0% similar despite different names*

```diff
@@ -240,23 +240,25 @@
                 auto_commit=auto_commit,
             )
             if transaction:
                 transaction_ctl = connection.begin()
             else:
                 transaction_ctl = None
             result = connection.execute(sql, *list_params, **params)
-            return result
+
         finally:
             if transaction:
                 if transaction_ctl is not None:
                     transaction_ctl.commit()
             if auto_close:
                 if connection is not None:
                     connection.close()
 
+        return result
+
     def execute_procedure(
             self,
             procedure_name,
             *args,
             return_results=False,
             dpapi_connection=None
     ):
```

### Comparing `bi_etl-1.4/bi_etl/database/mock_database_metadata.py` & `bi_etl-1.4.2/bi_etl/database/mock_database_metadata.py`

 * *Files identical despite different names*

### Comparing `bi_etl-1.4/bi_etl/example_config.ini` & `bi_etl-1.4.2/bi_etl/example_config.ini`

 * *Files identical despite different names*

### Comparing `bi_etl-1.4/bi_etl/example_config_shared.ini` & `bi_etl-1.4.2/bi_etl/example_config_shared.ini`

 * *Files identical despite different names*

### Comparing `bi_etl-1.4/bi_etl/exceptions/__init__.py` & `bi_etl-1.4.2/bi_etl/exceptions/__init__.py`

 * *Files identical despite different names*

### Comparing `bi_etl-1.4/bi_etl/informatica/pmcmd.py` & `bi_etl-1.4.2/bi_etl/informatica/pmcmd.py`

 * *Files identical despite different names*

### Comparing `bi_etl-1.4/bi_etl/informatica/pmcmd_task.py` & `bi_etl-1.4.2/bi_etl/informatica/pmcmd_task.py`

 * *Files identical despite different names*

### Comparing `bi_etl-1.4/bi_etl/informatica/pmrep.py` & `bi_etl-1.4.2/bi_etl/informatica/pmrep.py`

 * *Files identical despite different names*

### Comparing `bi_etl-1.4/bi_etl/lookups/autodisk_lookup.py` & `bi_etl-1.4.2/bi_etl/lookups/autodisk_lookup.py`

 * *Files identical despite different names*

### Comparing `bi_etl-1.4/bi_etl/lookups/autodisk_range_lookup.py` & `bi_etl-1.4.2/bi_etl/lookups/autodisk_range_lookup.py`

 * *Files identical despite different names*

### Comparing `bi_etl-1.4/bi_etl/lookups/disk_lookup.py` & `bi_etl-1.4.2/bi_etl/lookups/disk_lookup.py`

 * *Files identical despite different names*

### Comparing `bi_etl-1.4/bi_etl/lookups/disk_range_lookup.py` & `bi_etl-1.4.2/bi_etl/lookups/disk_range_lookup.py`

 * *Files identical despite different names*

### Comparing `bi_etl-1.4/bi_etl/lookups/lookup.py` & `bi_etl-1.4.2/bi_etl/lookups/lookup.py`

 * *Files identical despite different names*

### Comparing `bi_etl-1.4/bi_etl/lookups/non_unique_lookup.py` & `bi_etl-1.4.2/bi_etl/lookups/non_unique_lookup.py`

 * *Files identical despite different names*

### Comparing `bi_etl-1.4/bi_etl/lookups/range_lookup.py` & `bi_etl-1.4.2/bi_etl/lookups/range_lookup.py`

 * *Files identical despite different names*

### Comparing `bi_etl-1.4/bi_etl/memory_size.py` & `bi_etl-1.4.2/bi_etl/memory_size.py`

 * *Files identical despite different names*

### Comparing `bi_etl-1.4/bi_etl/notifiers/email.py` & `bi_etl-1.4.2/bi_etl/notifiers/email.py`

 * *Files identical despite different names*

### Comparing `bi_etl-1.4/bi_etl/notifiers/jira.py` & `bi_etl-1.4.2/bi_etl/notifiers/jira.py`

 * *Files identical despite different names*

### Comparing `bi_etl-1.4/bi_etl/notifiers/notifier_base.py` & `bi_etl-1.4.2/bi_etl/notifiers/notifier_base.py`

 * *Files identical despite different names*

### Comparing `bi_etl-1.4/bi_etl/notifiers/slack.py` & `bi_etl-1.4.2/bi_etl/notifiers/slack.py`

 * *Files identical despite different names*

### Comparing `bi_etl-1.4/bi_etl/parameters/file_parameter.py` & `bi_etl-1.4.2/bi_etl/parameters/file_parameter.py`

 * *Files identical despite different names*

### Comparing `bi_etl-1.4/bi_etl/performance_test/perftest_static_reader.py` & `bi_etl-1.4.2/bi_etl/performance_test/perftest_static_reader.py`

 * *Files identical despite different names*

### Comparing `bi_etl-1.4/bi_etl/scheduler/dependent_reasons.py` & `bi_etl-1.4.2/bi_etl/scheduler/dependent_reasons.py`

 * *Files identical despite different names*

### Comparing `bi_etl-1.4/bi_etl/scheduler/exceptions.py` & `bi_etl-1.4.2/bi_etl/scheduler/exceptions.py`

 * *Files identical despite different names*

### Comparing `bi_etl-1.4/bi_etl/scheduler/messages.py` & `bi_etl-1.4.2/bi_etl/scheduler/messages.py`

 * *Files identical despite different names*

### Comparing `bi_etl-1.4/bi_etl/scheduler/models.py` & `bi_etl-1.4.2/bi_etl/scheduler/models.py`

 * *Files identical despite different names*

### Comparing `bi_etl-1.4/bi_etl/scheduler/queue_io.py` & `bi_etl-1.4.2/bi_etl/scheduler/queue_io.py`

 * *Files identical despite different names*

### Comparing `bi_etl-1.4/bi_etl/scheduler/scheduler.py` & `bi_etl-1.4.2/bi_etl/scheduler/scheduler.py`

 * *Files identical despite different names*

### Comparing `bi_etl-1.4/bi_etl/scheduler/scheduler_etl_jobs/etl_task_status_cd.py` & `bi_etl-1.4.2/bi_etl/scheduler/scheduler_etl_jobs/etl_task_status_cd.py`

 * *Files identical despite different names*

### Comparing `bi_etl-1.4/bi_etl/scheduler/scheduler_interface.py` & `bi_etl-1.4.2/bi_etl/scheduler/scheduler_interface.py`

 * *Files identical despite different names*

### Comparing `bi_etl-1.4/bi_etl/scheduler/special_tasks.py` & `bi_etl-1.4.2/bi_etl/scheduler/special_tasks.py`

 * *Files identical despite different names*

### Comparing `bi_etl-1.4/bi_etl/scheduler/status.py` & `bi_etl-1.4.2/bi_etl/scheduler/status.py`

 * *Files identical despite different names*

### Comparing `bi_etl-1.4/bi_etl/scheduler/task.py` & `bi_etl-1.4.2/bi_etl/scheduler/task.py`

 * *Files 1% similar despite different names*

```diff
@@ -9,14 +9,15 @@
 import logging
 import socket
 import traceback
 import warnings
 from pathlib import Path
 from queue import Empty
 from typing import *
+from inspect import signature
 
 from config_wrangler.config_templates.sqlalchemy_database import SQLAlchemyDatabase, SQLAlchemyMetadata
 from config_wrangler.config_types.dynamically_referenced import DynamicallyReferenced
 from pydicti import dicti, Dicti
 
 import bi_etl
 import bi_etl.config.notifiers_config as notifiers_config
@@ -60,14 +61,15 @@
     def __init__(self,
                  config: BI_ETL_Config_Base,
                  task_id=None,
                  parent_task_id=None,
                  root_task_id=None,
                  scheduler=None,
                  task_rec=None,
+                 **kwargs
                  ):
         """
         Constructor. This code will run on the scheduler thread and the execution thread.
         It should do as little as possible.
 
         Parameters
         ----------
@@ -127,14 +129,15 @@
 
         self._externally_provided_scheduler = (scheduler is not None)
         self._scheduler = scheduler
         if self.status is None:
             self.status = Status.new
         self._parameters_loaded = False
         self._parameter_dict = dicti()
+        self.set_parameters(**kwargs)
         self.parent_to_child = None
         self.child_to_parent = None
         self.object_registry = list()
         self.thread_running = None
         self.summary_message_from_client = False
         self.last_log_msg_time = None
         self.pending_log_msgs = list()
@@ -643,94 +646,66 @@
         param_value: object
             The value of the parameter
         commit: bool
         local_only: bool
         """
         if not self._parameters_loaded:
             self.load_parameters()
+        self.log.info(f'add_parameter to task {param_name} = {param_value}')
         self._parameter_dict[param_name] = param_value
 
-        if not local_only:
-            if self.task_id is not None:
-                self.log.info(f'add_parameter to scheduler {param_name} = {param_value}')
-                self.scheduler.add_task_paramter(self.task_id, param_name, param_value, commit=commit)
-        else:
-            print(f"add_parameter local {param_name}={param_value}")
-
-    # Deprecated name
-    def add_parameter(
-            self,
-            param_name: str,
-            param_value: object,
-            local_only: bool = False,
-            commit: bool = True,
-    ):
-        warnings.warn("add_parameter is deprecated, please use set_parameter instead")
-        self.set_parameter(param_name=param_name,
-                           param_value=param_value,
-                           local_only=local_only,
-                           commit=commit)
-
     def set_parameters(
             self,
             local_only=False,
             commit=True,
             *args,
             **kwargs
     ):
         """
         Add multiple parameters to this task.
         Parameters can be passed in as any combination of:
-        * dict instance. Example ``add_parameters( {'param1':'example', 'param2':100} )``
-        * list of lists. Example: ``add_parameters( [ ['param1','example'], ['param2',100] ] )``
-        * list of tuples. Example: ``add_parameters( [ ('param1','example'), ('param2',100) ] )``
-        * keyword arguments. Example: ``add_parameters(foo=1, bar='apple')``
+        * dict instance. Example ``set_parameters( {'param1':'example', 'param2':100} )``
+        * list of lists. Example: ``set_parameters( [ ['param1','example'], ['param2',100] ] )``
+        * list of tuples. Example: ``set_parameters( [ ('param1','example'), ('param2',100) ] )``
+        * keyword arguments. Example: ``set_parameters(foo=1, bar='apple')``
         
         Parameters
         ----------
         local_only: boolean
             Optional. Default= False. Add parameters to local task only. Do not record in the scheduler.
         commit: boolean 
             Optional. Default= True. Commit changes to the task database.
         args: list
             list of lists. or list of tuples. See above.
         kwargs: dict
             keyword arguments send to parameters. See above.
         """
-        # Support add_parameters(param1='example', param2=100)
+        # Support set_parameters(param1='example', param2=100)
         self._parameter_dict.update(kwargs)
         for param_name, param_value in kwargs.items():
             self.set_parameter(param_name, param_value, local_only=local_only, commit=commit)
 
         # Also accept a list of dicts, tuples, or lists
-        # eg. add_parameters( [ ('param1','example'), ('param2',100) ] )
-        #  or add_parameters( [ ['param1','example'], ['param2',100] ] )
-        #  or add_parameters( [ ('param1','example'), ['param2',100] ] )
+        # eg. set_parameters( [ ('param1','example'), ('param2',100) ] )
+        #  or set_parameters( [ ['param1','example'], ['param2',100] ] )
+        #  or set_parameters( [ ('param1','example'), ['param2',100] ] )
         #  or parms = {'param1':'example', 'param2':100}
-        #     add_parameters(parms)
+        #     set_parameters(parms)
         #
         # which is equivalent to
         #     add_parameters(**parms)
         for arg in args:
             if isinstance(arg, Mapping):
                 for param_name, param_value in arg.items():
                     self.set_parameter(param_name, param_value, local_only=local_only, commit=commit)
             elif hasattr(arg, '__getitem__'):
                 if len(arg) == 2:
                     self.set_parameter(arg[0], arg[1], local_only=local_only, commit=commit)
                 else:
-                    raise ValueError(f"add_parameters sequence {arg} had unexpected length {len(arg)}")
-
-    # Deprecated name
-    def add_parameters(self, local_only=False, commit=True, *args, **kwargs):
-        warnings.warn("add_parameters is deprecated, please use set_parameters instead")
-        self.set_parameters(local_only=local_only,
-                            commit=commit,
-                            *args,
-                            **kwargs)
+                    raise ValueError(f"set_parameters sequence {arg} had unexpected length {len(arg)}")
 
     def parameters(self):
         """
         Returns a generator yielding tuples of parameter (name,value)
         """
         if not self._parameters_loaded:
             self.load_parameters()
@@ -1071,15 +1046,31 @@
             self.init_timer.start()
             self.init()
             self.init_timer.stop()
 
             self.process_messages()
 
             self.load_timer.start()
-            self.load()
+
+            # Check for paramters to pass to the load function
+            load_sig = signature(self.load)
+            load_params = load_sig.parameters
+            load_kwargs = dict()
+            valid_parameter_names = set(self.parameter_names())
+            for param in sig.parameters.values():
+                if param.kind in {param.POSITIONAL_ONLY, param.VAR_POSITIONAL}:
+                    raise ValueError(f"bi_etl.ETLTask only supports keyword parameters.")
+                else:
+                    if param.name in valid_parameter_names:
+                        load_kwargs[param.name] = self.get_parameter(param.name)
+                    else:
+                        if param.default == param.empty:
+                            raise ValueError(f"{self} needs parameter {param.name}. Load takes {load_sig}")
+
+            self.load(**load_args)
             self.load_timer.stop()
 
             self.process_messages()
 
             # finish would be the place to cleanup anything done in the init method 
             self.finish_timer.start()
             self.finish()
@@ -1352,15 +1343,15 @@
     Used to find an ETL task module and start it.
 
     Parameters
     ----------
     task_name: str
         The task name to run. Must match the name or at least *ending* of the name of a module under **etl_jobs**.
     parameters: list or dict
-        Parameters for the task. Passed to method :meth:`bi_etl.scheduler.task.ETLTask.add_parameters`.
+        Parameters for the task. Passed to method :meth:`bi_etl.scheduler.task.ETLTask.set_parameters`.
     config: Union[str, bi_etl.config.bi_etl_config_base.BI_ETL_Config_Base]
         The configuration to use (defaults to reading it from :doc:`config_ini`).
         If passed it should be an string reference to an ini file
         or an instance of :class:`bi_etl.config.bi_etl_config_base.BI_ETL_Config_Base`.
     suppress_notifications: boolean
         Skip sending email on failure? See suppress_notifications in :meth:`bi_etl.scheduler.task.ETLTask.run`.
     scheduler: bi_etl.scheduler.scheduler.Scheduler
```

### Comparing `bi_etl-1.4/bi_etl/statement_queue.py` & `bi_etl-1.4.2/bi_etl/statement_queue.py`

 * *Files identical despite different names*

### Comparing `bi_etl-1.4/bi_etl/statistics.py` & `bi_etl-1.4.2/bi_etl/statistics.py`

 * *Files identical despite different names*

### Comparing `bi_etl-1.4/bi_etl/test_notebooks/perftest_static_reader.py` & `bi_etl-1.4.2/bi_etl/test_notebooks/perftest_static_reader.py`

 * *Files identical despite different names*

### Comparing `bi_etl-1.4/bi_etl/test_notebooks/Row performance.ipynb` & `bi_etl-1.4.2/bi_etl/test_notebooks/Row performance.ipynb`

 * *Files identical despite different names*

### Comparing `bi_etl-1.4/bi_etl/test_notebooks/Utility Test.ipynb` & `bi_etl-1.4.2/bi_etl/test_notebooks/Utility Test.ipynb`

 * *Files identical despite different names*

### Comparing `bi_etl-1.4/bi_etl/timer.py` & `bi_etl-1.4.2/bi_etl/timer.py`

 * *Files identical despite different names*

### Comparing `bi_etl-1.4/bi_etl/utility/__init__.py` & `bi_etl-1.4.2/bi_etl/utility/__init__.py`

 * *Files identical despite different names*

### Comparing `bi_etl-1.4/bi_etl/utility/ask.py` & `bi_etl-1.4.2/bi_etl/utility/ask.py`

 * *Files identical despite different names*

### Comparing `bi_etl-1.4/bi_etl/utility/bcp_helpers.py` & `bi_etl-1.4.2/bi_etl/utility/bcp_helpers.py`

 * *Files identical despite different names*

### Comparing `bi_etl-1.4/bi_etl/utility/case_insentive_set.py` & `bi_etl-1.4.2/bi_etl/utility/case_insentive_set.py`

 * *Files identical despite different names*

### Comparing `bi_etl-1.4/bi_etl/utility/copy_table_data.py` & `bi_etl-1.4.2/bi_etl/utility/copy_table_data.py`

 * *Files identical despite different names*

### Comparing `bi_etl-1.4/bi_etl/utility/line_counter.py` & `bi_etl-1.4.2/bi_etl/utility/line_counter.py`

 * *Files identical despite different names*

### Comparing `bi_etl-1.4/bi_etl/utility/package_root.py` & `bi_etl-1.4.2/bi_etl/utility/package_root.py`

 * *Files identical despite different names*

### Comparing `bi_etl-1.4/bi_etl/utility/postgresql/psql_command.py` & `bi_etl-1.4.2/bi_etl/utility/postgresql/psql_command.py`

 * *Files identical despite different names*

### Comparing `bi_etl-1.4/bi_etl/utility/postgresql/psycopg2_helpers.py` & `bi_etl-1.4.2/bi_etl/utility/postgresql/psycopg2_helpers.py`

 * *Files identical despite different names*

### Comparing `bi_etl-1.4/bi_etl/utility/run_sql_script.py` & `bi_etl-1.4.2/bi_etl/utility/run_sql_script.py`

 * *Files identical despite different names*

### Comparing `bi_etl-1.4/bi_etl/utility/sql_server/defrag_indexes.py` & `bi_etl-1.4.2/bi_etl/utility/sql_server/defrag_indexes.py`

 * *Files 2% similar despite different names*

```diff
@@ -63,9 +63,9 @@
 if __name__ == '__main__':
     parser = ArgumentParser(description="Run ETL")
     parser.add_argument('--database', type=str, help='Database entry in config.ini to use')
     args = parser.parse_args()
     config = BI_ETL_Config_Base_From_Ini_Env()
     config.logging.setup_logging()
     df = DefragIndexes(config=config)
-    df.add_parameter("database", args.database)
+    df.set_parameters(database=args.database)
     df.run()
```

### Comparing `bi_etl-1.4/bi_etl/utility/ssh_forward.py` & `bi_etl-1.4.2/bi_etl/utility/ssh_forward.py`

 * *Files identical despite different names*

### Comparing `bi_etl-1.4/license.txt` & `bi_etl-1.4.2/license.txt`

 * *Files identical despite different names*

### Comparing `bi_etl-1.4/pyproject.toml` & `bi_etl-1.4.2/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "bi_etl"
-version = "1.4"
+version = "1.4.2"
 description = "Python ETL Framework"
 keywords=["etl"]
 classifiers = [
     "Topic :: Software Development :: Libraries :: Python Modules",
     "Development Status :: 5 - Production/Stable",
     "Topic :: Database",
 ]
@@ -13,66 +13,64 @@
 documentation = "https://bietl.dev/docs/"
 readme="README.md"
 license = "MIT"
 repository = "https://github.com/arcann/bi_etl"
 
 [tool.poetry.dependencies]
 python = "^3.7,<4.0"
-config-wrangler = ">= 0.5.0"
+config-wrangler = ">= 0.5.5"
 SQLAlchemy = ">=1.4.35"
 semidbm = ">=0.5.1"
 psutil = ">=5.7.2"
 openpyxl = ">=3.0.5"
 btrees = ">=4.7.2"
 gevent = ">=21.8.0"
 sqlparse = ">=0.4.2"
 keyring = ">=21.1.0"
 pydicti = ">=1.1.6"
 more-itertools = ">=9.0.0"
 
 # Optional
-pyramid = { version = ">=1.10.4", optional = true }
-pyjtable = {version = ">=0.1.1", optional = true}
 fastavro = {version = ">=1.0.0", optional = true}
 pyarrow = {version = ">=10.0.1", optional = true}
 boto3 = {version = ">=1.21", optional = true}
 psycopg2 = {version = ">=2.8.6", optional = true}
 jira = {version = ">=3.1.1", optional = true}
 slack-sdk = {version = ">=3.19.5", optional = true}
+pykeepass = {version = ">=4.0.5", optional = true}
 
 [tool.poetry.extras]
 # Install with:
 # poetry install -E keyring
 keyring = ["keyring"]
 
-jira = ["jira"]
+pykeepass = ["pykeepass"]
 
-# poetry install -E scheduler
-scheduler = ["pyramid", "pyjtable"]
+jira = ["jira"]
 
 slack = ["slack-sdk"]
 
 # poetry install -E test
 test = ["psycopg2", "testcontainers"]
 
 [tool.poetry.dev-dependencies]
 toml = "^0.10.1"
 testcontainers = {version = ">=3.5.4", extras = ["mysql oracle postgresql mssqlserver"]}
 tox = "^3.25.0"
 Jinja2 = ">=3.1.2"
-boto3 = ">=1.24"
-fastavro = "^1.5.3"
+boto3 = ">=1.26"
+fastavro = ">=1.5.3"
 Sphinx = ">=4.5,<5.0"
 sphinx-paramlinks = ">=0.5.4"
 sphinx-pydantic = ">=0.1.1"
 autodoc-pydantic = ">=1.7.2"
 # sphinx-autodoc-annotation = "^1.0-1"
 psycopg2 = ">=2.9.3"
 sphinx-sizzle-theme = ">=0.1.1"
 sphinx-autobuild = "^2021.3.14"
-cx-Oracle = "^8.3.0"
+oracledb = ">=1.2.0"
 pip = ">=22.1.2"
 slack-sdk = ">=3.19.5"
 
 [build-system]
 requires = ["poetry-core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
```

### Comparing `bi_etl-1.4/README.md` & `bi_etl-1.4.2/README.md`

 * *Files identical despite different names*

### Comparing `bi_etl-1.4/PKG-INFO` & `bi_etl-1.4.2/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bi-etl
-Version: 1.4
+Version: 1.4.2
 Summary: Python ETL Framework
 Home-page: https://github.com/arcann/bi_etl
 License: MIT
 Keywords: etl
 Author: Derek Wood
 Author-email: bietl_info@bietl.dev
 Requires-Python: >=3.7,<4.0
@@ -16,33 +16,32 @@
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Database
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Provides-Extra: jira
 Provides-Extra: keyring
-Provides-Extra: scheduler
+Provides-Extra: pykeepass
 Provides-Extra: slack
 Provides-Extra: test
 Requires-Dist: SQLAlchemy (>=1.4.35)
 Requires-Dist: boto3 (>=1.21)
 Requires-Dist: btrees (>=4.7.2)
-Requires-Dist: config-wrangler (>=0.5.0)
+Requires-Dist: config-wrangler (>=0.5.5)
 Requires-Dist: fastavro (>=1.0.0)
 Requires-Dist: gevent (>=21.8.0)
 Requires-Dist: jira (>=3.1.1) ; extra == "jira"
 Requires-Dist: keyring (>=21.1.0) ; extra == "keyring"
 Requires-Dist: more-itertools (>=9.0.0)
 Requires-Dist: openpyxl (>=3.0.5)
 Requires-Dist: psutil (>=5.7.2)
 Requires-Dist: psycopg2 (>=2.8.6) ; extra == "test"
 Requires-Dist: pyarrow (>=10.0.1)
 Requires-Dist: pydicti (>=1.1.6)
-Requires-Dist: pyjtable (>=0.1.1) ; extra == "scheduler"
-Requires-Dist: pyramid (>=1.10.4) ; extra == "scheduler"
+Requires-Dist: pykeepass (>=4.0.5) ; extra == "pykeepass"
 Requires-Dist: semidbm (>=0.5.1)
 Requires-Dist: slack-sdk (>=3.19.5) ; extra == "slack"
 Requires-Dist: sqlparse (>=0.4.2)
 Project-URL: Documentation, https://bietl.dev/docs/
 Project-URL: Repository, https://github.com/arcann/bi_etl
 Description-Content-Type: text/markdown
```

