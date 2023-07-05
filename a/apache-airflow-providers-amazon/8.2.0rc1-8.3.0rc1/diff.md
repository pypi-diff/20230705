# Comparing `tmp/apache-airflow-providers-amazon-8.2.0rc1.tar.gz` & `tmp/apache-airflow-providers-amazon-8.3.0rc1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "apache-airflow-providers-amazon-8.2.0rc1.tar", last modified: Tue Jun 20 11:41:04 2023, max compression
+gzip compressed data, was "apache-airflow-providers-amazon-8.3.0rc1.tar", last modified: Wed Jul  5 07:29:33 2023, max compression
```

## Comparing `apache-airflow-providers-amazon-8.2.0rc1.tar` & `apache-airflow-providers-amazon-8.3.0rc1.tar`

### file list

```diff
@@ -1,184 +1,194 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 11:41:04.142130 apache-airflow-providers-amazon-8.2.0rc1/
--rw-r--r--   0 root         (0) root         (0)    10850 2023-06-01 06:14:29.000000 apache-airflow-providers-amazon-8.2.0rc1/LICENSE
--rw-r--r--   0 root         (0) root         (0)     1219 2023-06-20 11:41:01.000000 apache-airflow-providers-amazon-8.2.0rc1/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)      240 2023-06-01 06:14:29.000000 apache-airflow-providers-amazon-8.2.0rc1/NOTICE
--rw-r--r--   0 root         (0) root         (0)    62914 2023-06-20 11:41:04.143504 apache-airflow-providers-amazon-8.2.0rc1/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)    61092 2023-06-20 11:41:01.000000 apache-airflow-providers-amazon-8.2.0rc1/README.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 11:41:03.575815 apache-airflow-providers-amazon-8.2.0rc1/airflow/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 11:41:03.577052 apache-airflow-providers-amazon-8.2.0rc1/airflow/providers/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 11:41:03.626042 apache-airflow-providers-amazon-8.2.0rc1/airflow/providers/amazon/
--rw-r--r--   0 root         (0) root         (0)     1531 2023-06-20 11:01:09.000000 apache-airflow-providers-amazon-8.2.0rc1/airflow/providers/amazon/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 11:41:03.632965 apache-airflow-providers-amazon-8.2.0rc1/airflow/providers/amazon/aws/
--rw-r--r--   0 root         (0) root         (0)      785 2023-06-01 06:14:28.000000 apache-airflow-providers-amazon-8.2.0rc1/airflow/providers/amazon/aws/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1731 2023-06-01 06:14:28.000000 apache-airflow-providers-amazon-8.2.0rc1/airflow/providers/amazon/aws/exceptions.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 11:41:03.761400 apache-airflow-providers-amazon-8.2.0rc1/airflow/providers/amazon/aws/hooks/
--rw-r--r--   0 root         (0) root         (0)      785 2023-06-01 06:14:28.000000 apache-airflow-providers-amazon-8.2.0rc1/airflow/providers/amazon/aws/hooks/__init__.py
--rw-r--r--   0 root         (0) root         (0)     4842 2023-06-08 05:42:54.000000 apache-airflow-providers-amazon-8.2.0rc1/airflow/providers/amazon/aws/hooks/appflow.py
--rw-r--r--   0 root         (0) root         (0)    12311 2023-06-17 16:45:00.000000 apache-airflow-providers-amazon-8.2.0rc1/airflow/providers/amazon/aws/hooks/athena.py
--rw-r--r--   0 root         (0) root         (0)    46780 2023-06-17 16:45:00.000000 apache-airflow-providers-amazon-8.2.0rc1/airflow/providers/amazon/aws/hooks/base_aws.py
--rw-r--r--   0 root         (0) root         (0)    21315 2023-06-20 06:40:52.000000 apache-airflow-providers-amazon-8.2.0rc1/airflow/providers/amazon/aws/hooks/batch_client.py
--rw-r--r--   0 root         (0) root         (0)     2511 2023-06-01 06:14:28.000000 apache-airflow-providers-amazon-8.2.0rc1/airflow/providers/amazon/aws/hooks/batch_waiters.json
--rw-r--r--   0 root         (0) root         (0)    10532 2023-06-20 06:40:52.000000 apache-airflow-providers-amazon-8.2.0rc1/airflow/providers/amazon/aws/hooks/batch_waiters.py
--rw-r--r--   0 root         (0) root         (0)     3377 2023-06-08 05:42:54.000000 apache-airflow-providers-amazon-8.2.0rc1/airflow/providers/amazon/aws/hooks/cloud_formation.py
--rw-r--r--   0 root         (0) root         (0)    14134 2023-06-08 05:42:54.000000 apache-airflow-providers-amazon-8.2.0rc1/airflow/providers/amazon/aws/hooks/datasync.py
--rw-r--r--   0 root         (0) root         (0)     7914 2023-06-08 05:42:54.000000 apache-airflow-providers-amazon-8.2.0rc1/airflow/providers/amazon/aws/hooks/dms.py
--rw-r--r--   0 root         (0) root         (0)     2669 2023-06-08 05:42:54.000000 apache-airflow-providers-amazon-8.2.0rc1/airflow/providers/amazon/aws/hooks/dynamodb.py
--rw-r--r--   0 root         (0) root         (0)     7927 2023-06-08 05:42:54.000000 apache-airflow-providers-amazon-8.2.0rc1/airflow/providers/amazon/aws/hooks/ec2.py
--rw-r--r--   0 root         (0) root         (0)     3702 2023-06-01 06:14:28.000000 apache-airflow-providers-amazon-8.2.0rc1/airflow/providers/amazon/aws/hooks/ecr.py
--rw-r--r--   0 root         (0) root         (0)     6608 2023-06-20 06:40:52.000000 apache-airflow-providers-amazon-8.2.0rc1/airflow/providers/amazon/aws/hooks/ecs.py
--rw-r--r--   0 root         (0) root         (0)    23957 2023-06-01 06:14:28.000000 apache-airflow-providers-amazon-8.2.0rc1/airflow/providers/amazon/aws/hooks/eks.py
--rw-r--r--   0 root         (0) root         (0)    12118 2023-06-08 05:42:54.000000 apache-airflow-providers-amazon-8.2.0rc1/airflow/providers/amazon/aws/hooks/elasticache_replication_group.py
--rw-r--r--   0 root         (0) root         (0)    20466 2023-06-08 05:42:54.000000 apache-airflow-providers-amazon-8.2.0rc1/airflow/providers/amazon/aws/hooks/emr.py
--rw-r--r--   0 root         (0) root         (0)     3452 2023-06-17 16:45:00.000000 apache-airflow-providers-amazon-8.2.0rc1/airflow/providers/amazon/aws/hooks/glacier.py
--rw-r--r--   0 root         (0) root         (0)    16390 2023-06-08 05:42:54.000000 apache-airflow-providers-amazon-8.2.0rc1/airflow/providers/amazon/aws/hooks/glue.py
--rw-r--r--   0 root         (0) root         (0)     7615 2023-06-08 05:42:54.000000 apache-airflow-providers-amazon-8.2.0rc1/airflow/providers/amazon/aws/hooks/glue_catalog.py
--rw-r--r--   0 root         (0) root         (0)     7930 2023-06-01 07:44:14.000000 apache-airflow-providers-amazon-8.2.0rc1/airflow/providers/amazon/aws/hooks/glue_crawler.py
--rw-r--r--   0 root         (0) root         (0)     1995 2023-06-08 05:42:54.000000 apache-airflow-providers-amazon-8.2.0rc1/airflow/providers/amazon/aws/hooks/kinesis.py
--rw-r--r--   0 root         (0) root         (0)     8009 2023-06-08 05:42:54.000000 apache-airflow-providers-amazon-8.2.0rc1/airflow/providers/amazon/aws/hooks/lambda_function.py
--rw-r--r--   0 root         (0) root         (0)     5293 2023-06-17 16:45:00.000000 apache-airflow-providers-amazon-8.2.0rc1/airflow/providers/amazon/aws/hooks/logs.py
--rw-r--r--   0 root         (0) root         (0)     7093 2023-06-17 16:45:00.000000 apache-airflow-providers-amazon-8.2.0rc1/airflow/providers/amazon/aws/hooks/quicksight.py
--rw-r--r--   0 root         (0) root         (0)    15272 2023-06-01 06:14:28.000000 apache-airflow-providers-amazon-8.2.0rc1/airflow/providers/amazon/aws/hooks/rds.py
--rw-r--r--   0 root         (0) root         (0)    13169 2023-06-17 16:45:00.000000 apache-airflow-providers-amazon-8.2.0rc1/airflow/providers/amazon/aws/hooks/redshift_cluster.py
--rw-r--r--   0 root         (0) root         (0)     7721 2023-06-08 05:42:54.000000 apache-airflow-providers-amazon-8.2.0rc1/airflow/providers/amazon/aws/hooks/redshift_data.py
--rw-r--r--   0 root         (0) root         (0)     7160 2023-06-17 16:45:00.000000 apache-airflow-providers-amazon-8.2.0rc1/airflow/providers/amazon/aws/hooks/redshift_sql.py
--rw-r--r--   0 root         (0) root         (0)    52680 2023-06-17 16:45:00.000000 apache-airflow-providers-amazon-8.2.0rc1/airflow/providers/amazon/aws/hooks/s3.py
--rw-r--r--   0 root         (0) root         (0)    56365 2023-06-17 16:45:00.000000 apache-airflow-providers-amazon-8.2.0rc1/airflow/providers/amazon/aws/hooks/sagemaker.py
--rw-r--r--   0 root         (0) root         (0)     2667 2023-06-17 16:45:00.000000 apache-airflow-providers-amazon-8.2.0rc1/airflow/providers/amazon/aws/hooks/secrets_manager.py
--rw-r--r--   0 root         (0) root         (0)     4145 2023-06-08 05:42:54.000000 apache-airflow-providers-amazon-8.2.0rc1/airflow/providers/amazon/aws/hooks/ses.py
--rw-r--r--   0 root         (0) root         (0)     3462 2023-06-08 05:42:54.000000 apache-airflow-providers-amazon-8.2.0rc1/airflow/providers/amazon/aws/hooks/sns.py
--rw-r--r--   0 root         (0) root         (0)     3120 2023-06-08 05:42:54.000000 apache-airflow-providers-amazon-8.2.0rc1/airflow/providers/amazon/aws/hooks/sqs.py
--rw-r--r--   0 root         (0) root         (0)     2449 2023-06-01 06:14:28.000000 apache-airflow-providers-amazon-8.2.0rc1/airflow/providers/amazon/aws/hooks/ssm.py
--rw-r--r--   0 root         (0) root         (0)     3073 2023-06-08 05:42:54.000000 apache-airflow-providers-amazon-8.2.0rc1/airflow/providers/amazon/aws/hooks/step_function.py
--rw-r--r--   0 root         (0) root         (0)     1817 2023-06-01 06:14:28.000000 apache-airflow-providers-amazon-8.2.0rc1/airflow/providers/amazon/aws/hooks/sts.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 11:41:03.782119 apache-airflow-providers-amazon-8.2.0rc1/airflow/providers/amazon/aws/links/
--rw-r--r--   0 root         (0) root         (0)      785 2023-06-01 06:14:28.000000 apache-airflow-providers-amazon-8.2.0rc1/airflow/providers/amazon/aws/links/__init__.py
--rw-r--r--   0 root         (0) root         (0)     2946 2023-06-08 05:42:54.000000 apache-airflow-providers-amazon-8.2.0rc1/airflow/providers/amazon/aws/links/base_aws.py
--rw-r--r--   0 root         (0) root         (0)     1770 2023-06-08 05:42:54.000000 apache-airflow-providers-amazon-8.2.0rc1/airflow/providers/amazon/aws/links/batch.py
--rw-r--r--   0 root         (0) root         (0)     2532 2023-06-08 05:42:54.000000 apache-airflow-providers-amazon-8.2.0rc1/airflow/providers/amazon/aws/links/emr.py
--rw-r--r--   0 root         (0) root         (0)     1229 2023-06-08 05:42:54.000000 apache-airflow-providers-amazon-8.2.0rc1/airflow/providers/amazon/aws/links/glue.py
--rw-r--r--   0 root         (0) root         (0)     1608 2023-06-08 05:42:54.000000 apache-airflow-providers-amazon-8.2.0rc1/airflow/providers/amazon/aws/links/logs.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 11:41:03.792781 apache-airflow-providers-amazon-8.2.0rc1/airflow/providers/amazon/aws/log/
--rw-r--r--   0 root         (0) root         (0)      785 2023-06-01 06:14:28.000000 apache-airflow-providers-amazon-8.2.0rc1/airflow/providers/amazon/aws/log/__init__.py
--rw-r--r--   0 root         (0) root         (0)     5057 2023-06-01 07:44:14.000000 apache-airflow-providers-amazon-8.2.0rc1/airflow/providers/amazon/aws/log/cloudwatch_task_handler.py
--rw-r--r--   0 root         (0) root         (0)     9654 2023-06-08 05:42:54.000000 apache-airflow-providers-amazon-8.2.0rc1/airflow/providers/amazon/aws/log/s3_task_handler.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 11:41:03.873805 apache-airflow-providers-amazon-8.2.0rc1/airflow/providers/amazon/aws/operators/
--rw-r--r--   0 root         (0) root         (0)      785 2023-06-01 06:14:28.000000 apache-airflow-providers-amazon-8.2.0rc1/airflow/providers/amazon/aws/operators/__init__.py
--rw-r--r--   0 root         (0) root         (0)    19662 2023-06-01 07:44:14.000000 apache-airflow-providers-amazon-8.2.0rc1/airflow/providers/amazon/aws/operators/appflow.py
--rw-r--r--   0 root         (0) root         (0)     6154 2023-06-08 05:42:54.000000 apache-airflow-providers-amazon-8.2.0rc1/airflow/providers/amazon/aws/operators/athena.py
--rw-r--r--   0 root         (0) root         (0)    19036 2023-06-20 06:40:52.000000 apache-airflow-providers-amazon-8.2.0rc1/airflow/providers/amazon/aws/operators/batch.py
--rw-r--r--   0 root         (0) root         (0)     3633 2023-06-01 06:14:28.000000 apache-airflow-providers-amazon-8.2.0rc1/airflow/providers/amazon/aws/operators/cloud_formation.py
--rw-r--r--   0 root         (0) root         (0)    18421 2023-06-08 05:42:54.000000 apache-airflow-providers-amazon-8.2.0rc1/airflow/providers/amazon/aws/operators/datasync.py
--rw-r--r--   0 root         (0) root         (0)    10720 2023-06-08 05:42:54.000000 apache-airflow-providers-amazon-8.2.0rc1/airflow/providers/amazon/aws/operators/dms.py
--rw-r--r--   0 root         (0) root         (0)     9591 2023-06-08 05:42:54.000000 apache-airflow-providers-amazon-8.2.0rc1/airflow/providers/amazon/aws/operators/ec2.py
--rw-r--r--   0 root         (0) root         (0)    27808 2023-06-20 06:40:52.000000 apache-airflow-providers-amazon-8.2.0rc1/airflow/providers/amazon/aws/operators/ecs.py
--rw-r--r--   0 root         (0) root         (0)    35613 2023-06-17 16:45:00.000000 apache-airflow-providers-amazon-8.2.0rc1/airflow/providers/amazon/aws/operators/eks.py
--rw-r--r--   0 root         (0) root         (0)    57732 2023-06-17 16:45:00.000000 apache-airflow-providers-amazon-8.2.0rc1/airflow/providers/amazon/aws/operators/emr.py
--rw-r--r--   0 root         (0) root         (0)     3707 2023-06-08 05:42:54.000000 apache-airflow-providers-amazon-8.2.0rc1/airflow/providers/amazon/aws/operators/glacier.py
--rw-r--r--   0 root         (0) root         (0)     8417 2023-06-17 16:45:00.000000 apache-airflow-providers-amazon-8.2.0rc1/airflow/providers/amazon/aws/operators/glue.py
--rw-r--r--   0 root         (0) root         (0)     4244 2023-06-08 05:42:54.000000 apache-airflow-providers-amazon-8.2.0rc1/airflow/providers/amazon/aws/operators/glue_crawler.py
--rw-r--r--   0 root         (0) root         (0)     7740 2023-06-01 07:44:14.000000 apache-airflow-providers-amazon-8.2.0rc1/airflow/providers/amazon/aws/operators/lambda_function.py
--rw-r--r--   0 root         (0) root         (0)     3972 2023-06-01 06:14:28.000000 apache-airflow-providers-amazon-8.2.0rc1/airflow/providers/amazon/aws/operators/quicksight.py
--rw-r--r--   0 root         (0) root         (0)    29880 2023-06-08 05:42:54.000000 apache-airflow-providers-amazon-8.2.0rc1/airflow/providers/amazon/aws/operators/rds.py
--rw-r--r--   0 root         (0) root         (0)    31930 2023-06-08 05:42:54.000000 apache-airflow-providers-amazon-8.2.0rc1/airflow/providers/amazon/aws/operators/redshift_cluster.py
--rw-r--r--   0 root         (0) root         (0)     5547 2023-06-08 05:42:54.000000 apache-airflow-providers-amazon-8.2.0rc1/airflow/providers/amazon/aws/operators/redshift_data.py
--rw-r--r--   0 root         (0) root         (0)    30242 2023-06-08 05:42:54.000000 apache-airflow-providers-amazon-8.2.0rc1/airflow/providers/amazon/aws/operators/s3.py
--rw-r--r--   0 root         (0) root         (0)    55180 2023-06-01 07:44:14.000000 apache-airflow-providers-amazon-8.2.0rc1/airflow/providers/amazon/aws/operators/sagemaker.py
--rw-r--r--   0 root         (0) root         (0)     2960 2023-06-08 05:42:54.000000 apache-airflow-providers-amazon-8.2.0rc1/airflow/providers/amazon/aws/operators/sns.py
--rw-r--r--   0 root         (0) root         (0)     3565 2023-06-08 05:42:54.000000 apache-airflow-providers-amazon-8.2.0rc1/airflow/providers/amazon/aws/operators/sqs.py
--rw-r--r--   0 root         (0) root         (0)     4583 2023-06-01 06:14:28.000000 apache-airflow-providers-amazon-8.2.0rc1/airflow/providers/amazon/aws/operators/step_function.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 11:41:03.882777 apache-airflow-providers-amazon-8.2.0rc1/airflow/providers/amazon/aws/secrets/
--rw-r--r--   0 root         (0) root         (0)      785 2023-06-01 06:14:28.000000 apache-airflow-providers-amazon-8.2.0rc1/airflow/providers/amazon/aws/secrets/__init__.py
--rw-r--r--   0 root         (0) root         (0)    15625 2023-06-08 05:42:54.000000 apache-airflow-providers-amazon-8.2.0rc1/airflow/providers/amazon/aws/secrets/secrets_manager.py
--rw-r--r--   0 root         (0) root         (0)     8495 2023-06-08 05:42:54.000000 apache-airflow-providers-amazon-8.2.0rc1/airflow/providers/amazon/aws/secrets/systems_manager.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 11:41:03.949998 apache-airflow-providers-amazon-8.2.0rc1/airflow/providers/amazon/aws/sensors/
--rw-r--r--   0 root         (0) root         (0)      785 2023-06-01 06:14:28.000000 apache-airflow-providers-amazon-8.2.0rc1/airflow/providers/amazon/aws/sensors/__init__.py
--rw-r--r--   0 root         (0) root         (0)     3106 2023-06-08 05:42:54.000000 apache-airflow-providers-amazon-8.2.0rc1/airflow/providers/amazon/aws/sensors/athena.py
--rw-r--r--   0 root         (0) root         (0)     9098 2023-06-17 16:45:00.000000 apache-airflow-providers-amazon-8.2.0rc1/airflow/providers/amazon/aws/sensors/batch.py
--rw-r--r--   0 root         (0) root         (0)     4150 2023-06-08 05:42:54.000000 apache-airflow-providers-amazon-8.2.0rc1/airflow/providers/amazon/aws/sensors/cloud_formation.py
--rw-r--r--   0 root         (0) root         (0)     3984 2023-06-08 05:42:54.000000 apache-airflow-providers-amazon-8.2.0rc1/airflow/providers/amazon/aws/sensors/dms.py
--rw-r--r--   0 root         (0) root         (0)     4424 2023-06-08 05:42:54.000000 apache-airflow-providers-amazon-8.2.0rc1/airflow/providers/amazon/aws/sensors/dynamodb.py
--rw-r--r--   0 root         (0) root         (0)     3643 2023-06-01 07:44:14.000000 apache-airflow-providers-amazon-8.2.0rc1/airflow/providers/amazon/aws/sensors/ec2.py
--rw-r--r--   0 root         (0) root         (0)     7188 2023-06-01 07:44:14.000000 apache-airflow-providers-amazon-8.2.0rc1/airflow/providers/amazon/aws/sensors/ecs.py
--rw-r--r--   0 root         (0) root         (0)     9771 2023-06-01 07:44:14.000000 apache-airflow-providers-amazon-8.2.0rc1/airflow/providers/amazon/aws/sensors/eks.py
--rw-r--r--   0 root         (0) root         (0)    20515 2023-06-20 06:40:52.000000 apache-airflow-providers-amazon-8.2.0rc1/airflow/providers/amazon/aws/sensors/emr.py
--rw-r--r--   0 root         (0) root         (0)     4115 2023-06-08 05:42:54.000000 apache-airflow-providers-amazon-8.2.0rc1/airflow/providers/amazon/aws/sensors/glacier.py
--rw-r--r--   0 root         (0) root         (0)     3319 2023-06-08 05:42:54.000000 apache-airflow-providers-amazon-8.2.0rc1/airflow/providers/amazon/aws/sensors/glue.py
--rw-r--r--   0 root         (0) root         (0)     3719 2023-06-08 05:42:54.000000 apache-airflow-providers-amazon-8.2.0rc1/airflow/providers/amazon/aws/sensors/glue_catalog_partition.py
--rw-r--r--   0 root         (0) root         (0)     2951 2023-06-08 05:42:54.000000 apache-airflow-providers-amazon-8.2.0rc1/airflow/providers/amazon/aws/sensors/glue_crawler.py
--rw-r--r--   0 root         (0) root         (0)     3049 2023-06-01 07:44:14.000000 apache-airflow-providers-amazon-8.2.0rc1/airflow/providers/amazon/aws/sensors/lambda_function.py
--rw-r--r--   0 root         (0) root         (0)     3626 2023-06-01 07:44:14.000000 apache-airflow-providers-amazon-8.2.0rc1/airflow/providers/amazon/aws/sensors/quicksight.py
--rw-r--r--   0 root         (0) root         (0)     6434 2023-06-08 05:42:54.000000 apache-airflow-providers-amazon-8.2.0rc1/airflow/providers/amazon/aws/sensors/rds.py
--rw-r--r--   0 root         (0) root         (0)     2623 2023-06-08 05:42:54.000000 apache-airflow-providers-amazon-8.2.0rc1/airflow/providers/amazon/aws/sensors/redshift_cluster.py
--rw-r--r--   0 root         (0) root         (0)    13390 2023-06-17 16:45:00.000000 apache-airflow-providers-amazon-8.2.0rc1/airflow/providers/amazon/aws/sensors/s3.py
--rw-r--r--   0 root         (0) root         (0)    13042 2023-06-01 07:44:14.000000 apache-airflow-providers-amazon-8.2.0rc1/airflow/providers/amazon/aws/sensors/sagemaker.py
--rw-r--r--   0 root         (0) root         (0)     9542 2023-06-08 05:42:54.000000 apache-airflow-providers-amazon-8.2.0rc1/airflow/providers/amazon/aws/sensors/sqs.py
--rw-r--r--   0 root         (0) root         (0)     3386 2023-06-08 05:42:54.000000 apache-airflow-providers-amazon-8.2.0rc1/airflow/providers/amazon/aws/sensors/step_function.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 11:41:04.010271 apache-airflow-providers-amazon-8.2.0rc1/airflow/providers/amazon/aws/transfers/
--rw-r--r--   0 root         (0) root         (0)      785 2023-06-01 06:14:28.000000 apache-airflow-providers-amazon-8.2.0rc1/airflow/providers/amazon/aws/transfers/__init__.py
--rw-r--r--   0 root         (0) root         (0)     2850 2023-06-08 05:42:54.000000 apache-airflow-providers-amazon-8.2.0rc1/airflow/providers/amazon/aws/transfers/base.py
--rw-r--r--   0 root         (0) root         (0)     7832 2023-06-08 05:42:54.000000 apache-airflow-providers-amazon-8.2.0rc1/airflow/providers/amazon/aws/transfers/dynamodb_to_s3.py
--rw-r--r--   0 root         (0) root         (0)     4410 2023-06-01 06:14:28.000000 apache-airflow-providers-amazon-8.2.0rc1/airflow/providers/amazon/aws/transfers/exasol_to_s3.py
--rw-r--r--   0 root         (0) root         (0)     6435 2023-06-01 06:14:28.000000 apache-airflow-providers-amazon-8.2.0rc1/airflow/providers/amazon/aws/transfers/ftp_to_s3.py
--rw-r--r--   0 root         (0) root         (0)     7676 2023-06-01 06:14:28.000000 apache-airflow-providers-amazon-8.2.0rc1/airflow/providers/amazon/aws/transfers/gcs_to_s3.py
--rw-r--r--   0 root         (0) root         (0)     4702 2023-06-08 05:42:54.000000 apache-airflow-providers-amazon-8.2.0rc1/airflow/providers/amazon/aws/transfers/glacier_to_gcs.py
--rw-r--r--   0 root         (0) root         (0)     9042 2023-06-01 06:14:28.000000 apache-airflow-providers-amazon-8.2.0rc1/airflow/providers/amazon/aws/transfers/google_api_to_s3.py
--rw-r--r--   0 root         (0) root         (0)     4172 2023-06-01 06:14:28.000000 apache-airflow-providers-amazon-8.2.0rc1/airflow/providers/amazon/aws/transfers/hive_to_dynamodb.py
--rw-r--r--   0 root         (0) root         (0)     4248 2023-06-01 06:14:28.000000 apache-airflow-providers-amazon-8.2.0rc1/airflow/providers/amazon/aws/transfers/imap_attachment_to_s3.py
--rw-r--r--   0 root         (0) root         (0)     4158 2023-06-01 06:14:28.000000 apache-airflow-providers-amazon-8.2.0rc1/airflow/providers/amazon/aws/transfers/local_to_s3.py
--rw-r--r--   0 root         (0) root         (0)     5981 2023-06-17 16:45:00.000000 apache-airflow-providers-amazon-8.2.0rc1/airflow/providers/amazon/aws/transfers/mongo_to_s3.py
--rw-r--r--   0 root         (0) root         (0)     8108 2023-06-01 06:14:28.000000 apache-airflow-providers-amazon-8.2.0rc1/airflow/providers/amazon/aws/transfers/redshift_to_s3.py
--rw-r--r--   0 root         (0) root         (0)     2966 2023-06-01 06:14:28.000000 apache-airflow-providers-amazon-8.2.0rc1/airflow/providers/amazon/aws/transfers/s3_to_ftp.py
--rw-r--r--   0 root         (0) root         (0)     8287 2023-06-08 05:42:54.000000 apache-airflow-providers-amazon-8.2.0rc1/airflow/providers/amazon/aws/transfers/s3_to_redshift.py
--rw-r--r--   0 root         (0) root         (0)     3191 2023-06-01 06:14:28.000000 apache-airflow-providers-amazon-8.2.0rc1/airflow/providers/amazon/aws/transfers/s3_to_sftp.py
--rw-r--r--   0 root         (0) root         (0)     4634 2023-06-17 16:45:00.000000 apache-airflow-providers-amazon-8.2.0rc1/airflow/providers/amazon/aws/transfers/s3_to_sql.py
--rw-r--r--   0 root         (0) root         (0)     5679 2023-06-01 06:14:28.000000 apache-airflow-providers-amazon-8.2.0rc1/airflow/providers/amazon/aws/transfers/salesforce_to_s3.py
--rw-r--r--   0 root         (0) root         (0)     3679 2023-06-01 06:14:28.000000 apache-airflow-providers-amazon-8.2.0rc1/airflow/providers/amazon/aws/transfers/sftp_to_s3.py
--rw-r--r--   0 root         (0) root         (0)     8864 2023-06-08 05:42:54.000000 apache-airflow-providers-amazon-8.2.0rc1/airflow/providers/amazon/aws/transfers/sql_to_s3.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 11:41:04.042963 apache-airflow-providers-amazon-8.2.0rc1/airflow/providers/amazon/aws/triggers/
--rw-r--r--   0 root         (0) root         (0)      787 2023-06-01 06:14:28.000000 apache-airflow-providers-amazon-8.2.0rc1/airflow/providers/amazon/aws/triggers/__init__.py
--rw-r--r--   0 root         (0) root         (0)     7341 2023-06-17 16:45:00.000000 apache-airflow-providers-amazon-8.2.0rc1/airflow/providers/amazon/aws/triggers/batch.py
--rw-r--r--   0 root         (0) root         (0)     2991 2023-06-01 07:44:14.000000 apache-airflow-providers-amazon-8.2.0rc1/airflow/providers/amazon/aws/triggers/ec2.py
--rw-r--r--   0 root         (0) root         (0)     6587 2023-06-17 16:45:00.000000 apache-airflow-providers-amazon-8.2.0rc1/airflow/providers/amazon/aws/triggers/eks.py
--rw-r--r--   0 root         (0) root         (0)    12671 2023-06-20 06:40:52.000000 apache-airflow-providers-amazon-8.2.0rc1/airflow/providers/amazon/aws/triggers/emr.py
--rw-r--r--   0 root         (0) root         (0)     2346 2023-06-08 05:42:54.000000 apache-airflow-providers-amazon-8.2.0rc1/airflow/providers/amazon/aws/triggers/glue.py
--rw-r--r--   0 root         (0) root         (0)     3090 2023-06-08 05:42:54.000000 apache-airflow-providers-amazon-8.2.0rc1/airflow/providers/amazon/aws/triggers/glue_crawler.py
--rw-r--r--   0 root         (0) root         (0)    14450 2023-06-08 05:42:54.000000 apache-airflow-providers-amazon-8.2.0rc1/airflow/providers/amazon/aws/triggers/redshift_cluster.py
--rw-r--r--   0 root         (0) root         (0)     4119 2023-06-17 16:45:00.000000 apache-airflow-providers-amazon-8.2.0rc1/airflow/providers/amazon/aws/triggers/s3.py
--rw-r--r--   0 root         (0) root         (0)     3838 2023-06-01 07:44:14.000000 apache-airflow-providers-amazon-8.2.0rc1/airflow/providers/amazon/aws/triggers/sagemaker.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 11:41:04.072025 apache-airflow-providers-amazon-8.2.0rc1/airflow/providers/amazon/aws/utils/
--rw-r--r--   0 root         (0) root         (0)     2265 2023-06-01 06:14:28.000000 apache-airflow-providers-amazon-8.2.0rc1/airflow/providers/amazon/aws/utils/__init__.py
--rw-r--r--   0 root         (0) root         (0)    20649 2023-06-17 16:45:00.000000 apache-airflow-providers-amazon-8.2.0rc1/airflow/providers/amazon/aws/utils/connection_wrapper.py
--rw-r--r--   0 root         (0) root         (0)     2561 2023-06-01 06:14:28.000000 apache-airflow-providers-amazon-8.2.0rc1/airflow/providers/amazon/aws/utils/eks_get_token.py
--rw-r--r--   0 root         (0) root         (0)     1854 2023-06-08 05:42:54.000000 apache-airflow-providers-amazon-8.2.0rc1/airflow/providers/amazon/aws/utils/emailer.py
--rw-r--r--   0 root         (0) root         (0)      973 2023-06-08 05:42:54.000000 apache-airflow-providers-amazon-8.2.0rc1/airflow/providers/amazon/aws/utils/rds.py
--rw-r--r--   0 root         (0) root         (0)     1897 2023-06-17 16:45:00.000000 apache-airflow-providers-amazon-8.2.0rc1/airflow/providers/amazon/aws/utils/redshift.py
--rw-r--r--   0 root         (0) root         (0)     1040 2023-06-01 06:14:28.000000 apache-airflow-providers-amazon-8.2.0rc1/airflow/providers/amazon/aws/utils/sagemaker.py
--rw-r--r--   0 root         (0) root         (0)     1701 2023-06-01 06:14:28.000000 apache-airflow-providers-amazon-8.2.0rc1/airflow/providers/amazon/aws/utils/tags.py
--rw-r--r--   0 root         (0) root         (0)     4099 2023-06-20 06:40:52.000000 apache-airflow-providers-amazon-8.2.0rc1/airflow/providers/amazon/aws/utils/task_log_fetcher.py
--rw-r--r--   0 root         (0) root         (0)     3583 2023-06-01 06:14:28.000000 apache-airflow-providers-amazon-8.2.0rc1/airflow/providers/amazon/aws/utils/waiter.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 11:41:04.111489 apache-airflow-providers-amazon-8.2.0rc1/airflow/providers/amazon/aws/waiters/
--rw-r--r--   0 root         (0) root         (0)      785 2023-06-01 06:14:28.000000 apache-airflow-providers-amazon-8.2.0rc1/airflow/providers/amazon/aws/waiters/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1002 2023-06-01 06:14:28.000000 apache-airflow-providers-amazon-8.2.0rc1/airflow/providers/amazon/aws/waiters/appflow.json
--rw-r--r--   0 root         (0) root         (0)     1853 2023-06-01 06:14:28.000000 apache-airflow-providers-amazon-8.2.0rc1/airflow/providers/amazon/aws/waiters/base_waiter.py
--rw-r--r--   0 root         (0) root         (0)      542 2023-06-01 06:14:28.000000 apache-airflow-providers-amazon-8.2.0rc1/airflow/providers/amazon/aws/waiters/batch.json
--rw-r--r--   0 root         (0) root         (0)      895 2023-06-01 06:14:28.000000 apache-airflow-providers-amazon-8.2.0rc1/airflow/providers/amazon/aws/waiters/dynamodb.json
--rw-r--r--   0 root         (0) root         (0)     1674 2023-06-17 16:45:00.000000 apache-airflow-providers-amazon-8.2.0rc1/airflow/providers/amazon/aws/waiters/ecs.json
--rw-r--r--   0 root         (0) root         (0)      659 2023-06-01 06:14:28.000000 apache-airflow-providers-amazon-8.2.0rc1/airflow/providers/amazon/aws/waiters/eks.json
--rw-r--r--   0 root         (0) root         (0)      851 2023-06-20 06:40:52.000000 apache-airflow-providers-amazon-8.2.0rc1/airflow/providers/amazon/aws/waiters/emr-containers.json
--rw-r--r--   0 root         (0) root         (0)      430 2023-06-01 06:14:28.000000 apache-airflow-providers-amazon-8.2.0rc1/airflow/providers/amazon/aws/waiters/emr-serverless.json
--rw-r--r--   0 root         (0) root         (0)     3207 2023-06-17 16:45:00.000000 apache-airflow-providers-amazon-8.2.0rc1/airflow/providers/amazon/aws/waiters/emr.json
--rw-r--r--   0 root         (0) root         (0)      932 2023-06-01 07:44:14.000000 apache-airflow-providers-amazon-8.2.0rc1/airflow/providers/amazon/aws/waiters/glue.json
--rw-r--r--   0 root         (0) root         (0)     1742 2023-06-01 06:14:28.000000 apache-airflow-providers-amazon-8.2.0rc1/airflow/providers/amazon/aws/waiters/redshift.json
--rw-r--r--   0 root         (0) root         (0)     2699 2023-06-01 06:14:28.000000 apache-airflow-providers-amazon-8.2.0rc1/airflow/providers/amazon/aws/waiters/sagemaker.json
--rw-r--r--   0 root         (0) root         (0)    38443 2023-06-20 11:41:01.000000 apache-airflow-providers-amazon-8.2.0rc1/airflow/providers/amazon/get_provider_info.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 11:41:04.139176 apache-airflow-providers-amazon-8.2.0rc1/apache_airflow_providers_amazon.egg-info/
--rw-r--r--   0 root         (0) root         (0)    62914 2023-06-20 11:41:03.000000 apache-airflow-providers-amazon-8.2.0rc1/apache_airflow_providers_amazon.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     8002 2023-06-20 11:41:03.000000 apache-airflow-providers-amazon-8.2.0rc1/apache_airflow_providers_amazon.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-06-20 11:41:03.000000 apache-airflow-providers-amazon-8.2.0rc1/apache_airflow_providers_amazon.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      103 2023-06-20 11:41:03.000000 apache-airflow-providers-amazon-8.2.0rc1/apache_airflow_providers_amazon.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-06-20 11:41:03.000000 apache-airflow-providers-amazon-8.2.0rc1/apache_airflow_providers_amazon.egg-info/not-zip-safe
--rw-r--r--   0 root         (0) root         (0)      814 2023-06-20 11:41:03.000000 apache-airflow-providers-amazon-8.2.0rc1/apache_airflow_providers_amazon.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        8 2023-06-20 11:41:03.000000 apache-airflow-providers-amazon-8.2.0rc1/apache_airflow_providers_amazon.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)     5294 2023-06-08 05:42:54.000000 apache-airflow-providers-amazon-8.2.0rc1/pyproject.toml
--rw-r--r--   0 root         (0) root         (0)     2116 2023-06-20 11:41:04.145653 apache-airflow-providers-amazon-8.2.0rc1/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     2363 2023-06-20 11:41:01.000000 apache-airflow-providers-amazon-8.2.0rc1/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-05 07:29:33.219222 apache-airflow-providers-amazon-8.3.0rc1/
+-rw-r--r--   0 root         (0) root         (0)    10850 2023-06-01 06:14:29.000000 apache-airflow-providers-amazon-8.3.0rc1/LICENSE
+-rw-r--r--   0 root         (0) root         (0)     1219 2023-07-05 07:29:30.000000 apache-airflow-providers-amazon-8.3.0rc1/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)      240 2023-06-01 06:14:29.000000 apache-airflow-providers-amazon-8.3.0rc1/NOTICE
+-rw-r--r--   0 root         (0) root         (0)     8022 2023-07-05 07:29:33.219886 apache-airflow-providers-amazon-8.3.0rc1/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     6037 2023-07-05 07:29:30.000000 apache-airflow-providers-amazon-8.3.0rc1/README.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-05 07:29:32.607595 apache-airflow-providers-amazon-8.3.0rc1/airflow/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-05 07:29:32.608760 apache-airflow-providers-amazon-8.3.0rc1/airflow/providers/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-05 07:29:32.664412 apache-airflow-providers-amazon-8.3.0rc1/airflow/providers/amazon/
+-rw-r--r--   0 root         (0) root         (0)     1531 2023-07-05 07:19:39.000000 apache-airflow-providers-amazon-8.3.0rc1/airflow/providers/amazon/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-05 07:29:32.671860 apache-airflow-providers-amazon-8.3.0rc1/airflow/providers/amazon/aws/
+-rw-r--r--   0 root         (0) root         (0)      785 2023-06-01 06:14:28.000000 apache-airflow-providers-amazon-8.3.0rc1/airflow/providers/amazon/aws/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1731 2023-06-01 06:14:28.000000 apache-airflow-providers-amazon-8.3.0rc1/airflow/providers/amazon/aws/exceptions.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-05 07:29:32.800499 apache-airflow-providers-amazon-8.3.0rc1/airflow/providers/amazon/aws/hooks/
+-rw-r--r--   0 root         (0) root         (0)      785 2023-06-01 06:14:28.000000 apache-airflow-providers-amazon-8.3.0rc1/airflow/providers/amazon/aws/hooks/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     4835 2023-06-29 05:49:29.000000 apache-airflow-providers-amazon-8.3.0rc1/airflow/providers/amazon/aws/hooks/appflow.py
+-rw-r--r--   0 root         (0) root         (0)    12334 2023-06-28 06:26:40.000000 apache-airflow-providers-amazon-8.3.0rc1/airflow/providers/amazon/aws/hooks/athena.py
+-rw-r--r--   0 root         (0) root         (0)    46780 2023-06-17 16:45:00.000000 apache-airflow-providers-amazon-8.3.0rc1/airflow/providers/amazon/aws/hooks/base_aws.py
+-rw-r--r--   0 root         (0) root         (0)    21319 2023-06-29 05:49:29.000000 apache-airflow-providers-amazon-8.3.0rc1/airflow/providers/amazon/aws/hooks/batch_client.py
+-rw-r--r--   0 root         (0) root         (0)     2511 2023-06-01 06:14:28.000000 apache-airflow-providers-amazon-8.3.0rc1/airflow/providers/amazon/aws/hooks/batch_waiters.json
+-rw-r--r--   0 root         (0) root         (0)    10541 2023-06-29 05:49:29.000000 apache-airflow-providers-amazon-8.3.0rc1/airflow/providers/amazon/aws/hooks/batch_waiters.py
+-rw-r--r--   0 root         (0) root         (0)     4263 2023-06-28 06:26:40.000000 apache-airflow-providers-amazon-8.3.0rc1/airflow/providers/amazon/aws/hooks/chime.py
+-rw-r--r--   0 root         (0) root         (0)     3378 2023-06-29 05:49:29.000000 apache-airflow-providers-amazon-8.3.0rc1/airflow/providers/amazon/aws/hooks/cloud_formation.py
+-rw-r--r--   0 root         (0) root         (0)    14079 2023-06-29 05:49:29.000000 apache-airflow-providers-amazon-8.3.0rc1/airflow/providers/amazon/aws/hooks/datasync.py
+-rw-r--r--   0 root         (0) root         (0)     7907 2023-06-29 05:49:29.000000 apache-airflow-providers-amazon-8.3.0rc1/airflow/providers/amazon/aws/hooks/dms.py
+-rw-r--r--   0 root         (0) root         (0)     2670 2023-06-29 05:49:29.000000 apache-airflow-providers-amazon-8.3.0rc1/airflow/providers/amazon/aws/hooks/dynamodb.py
+-rw-r--r--   0 root         (0) root         (0)     7928 2023-06-29 05:49:29.000000 apache-airflow-providers-amazon-8.3.0rc1/airflow/providers/amazon/aws/hooks/ec2.py
+-rw-r--r--   0 root         (0) root         (0)     3703 2023-06-29 05:49:29.000000 apache-airflow-providers-amazon-8.3.0rc1/airflow/providers/amazon/aws/hooks/ecr.py
+-rw-r--r--   0 root         (0) root         (0)     6610 2023-06-29 05:49:29.000000 apache-airflow-providers-amazon-8.3.0rc1/airflow/providers/amazon/aws/hooks/ecs.py
+-rw-r--r--   0 root         (0) root         (0)    23958 2023-06-29 05:49:29.000000 apache-airflow-providers-amazon-8.3.0rc1/airflow/providers/amazon/aws/hooks/eks.py
+-rw-r--r--   0 root         (0) root         (0)    12119 2023-06-29 05:49:29.000000 apache-airflow-providers-amazon-8.3.0rc1/airflow/providers/amazon/aws/hooks/elasticache_replication_group.py
+-rw-r--r--   0 root         (0) root         (0)    20429 2023-06-29 05:49:29.000000 apache-airflow-providers-amazon-8.3.0rc1/airflow/providers/amazon/aws/hooks/emr.py
+-rw-r--r--   0 root         (0) root         (0)     3452 2023-06-17 16:45:00.000000 apache-airflow-providers-amazon-8.3.0rc1/airflow/providers/amazon/aws/hooks/glacier.py
+-rw-r--r--   0 root         (0) root         (0)    16313 2023-06-29 05:49:29.000000 apache-airflow-providers-amazon-8.3.0rc1/airflow/providers/amazon/aws/hooks/glue.py
+-rw-r--r--   0 root         (0) root         (0)     7616 2023-06-29 05:49:29.000000 apache-airflow-providers-amazon-8.3.0rc1/airflow/providers/amazon/aws/hooks/glue_catalog.py
+-rw-r--r--   0 root         (0) root         (0)     7872 2023-06-29 05:49:29.000000 apache-airflow-providers-amazon-8.3.0rc1/airflow/providers/amazon/aws/hooks/glue_crawler.py
+-rw-r--r--   0 root         (0) root         (0)     1996 2023-06-29 05:49:29.000000 apache-airflow-providers-amazon-8.3.0rc1/airflow/providers/amazon/aws/hooks/kinesis.py
+-rw-r--r--   0 root         (0) root         (0)     8095 2023-07-03 06:46:02.000000 apache-airflow-providers-amazon-8.3.0rc1/airflow/providers/amazon/aws/hooks/lambda_function.py
+-rw-r--r--   0 root         (0) root         (0)     5883 2023-06-29 05:49:29.000000 apache-airflow-providers-amazon-8.3.0rc1/airflow/providers/amazon/aws/hooks/logs.py
+-rw-r--r--   0 root         (0) root         (0)     7094 2023-06-29 05:49:29.000000 apache-airflow-providers-amazon-8.3.0rc1/airflow/providers/amazon/aws/hooks/quicksight.py
+-rw-r--r--   0 root         (0) root         (0)    15479 2023-06-29 05:49:29.000000 apache-airflow-providers-amazon-8.3.0rc1/airflow/providers/amazon/aws/hooks/rds.py
+-rw-r--r--   0 root         (0) root         (0)    13169 2023-06-17 16:45:00.000000 apache-airflow-providers-amazon-8.3.0rc1/airflow/providers/amazon/aws/hooks/redshift_cluster.py
+-rw-r--r--   0 root         (0) root         (0)     7722 2023-06-29 05:49:29.000000 apache-airflow-providers-amazon-8.3.0rc1/airflow/providers/amazon/aws/hooks/redshift_data.py
+-rw-r--r--   0 root         (0) root         (0)     7160 2023-06-17 16:45:00.000000 apache-airflow-providers-amazon-8.3.0rc1/airflow/providers/amazon/aws/hooks/redshift_sql.py
+-rw-r--r--   0 root         (0) root         (0)    58295 2023-06-30 08:49:17.000000 apache-airflow-providers-amazon-8.3.0rc1/airflow/providers/amazon/aws/hooks/s3.py
+-rw-r--r--   0 root         (0) root         (0)    56365 2023-06-17 16:45:00.000000 apache-airflow-providers-amazon-8.3.0rc1/airflow/providers/amazon/aws/hooks/sagemaker.py
+-rw-r--r--   0 root         (0) root         (0)     2667 2023-06-17 16:45:00.000000 apache-airflow-providers-amazon-8.3.0rc1/airflow/providers/amazon/aws/hooks/secrets_manager.py
+-rw-r--r--   0 root         (0) root         (0)     4146 2023-06-29 05:49:29.000000 apache-airflow-providers-amazon-8.3.0rc1/airflow/providers/amazon/aws/hooks/ses.py
+-rw-r--r--   0 root         (0) root         (0)     3463 2023-06-29 05:49:29.000000 apache-airflow-providers-amazon-8.3.0rc1/airflow/providers/amazon/aws/hooks/sns.py
+-rw-r--r--   0 root         (0) root         (0)     3121 2023-06-29 05:49:29.000000 apache-airflow-providers-amazon-8.3.0rc1/airflow/providers/amazon/aws/hooks/sqs.py
+-rw-r--r--   0 root         (0) root         (0)     2393 2023-06-29 05:49:29.000000 apache-airflow-providers-amazon-8.3.0rc1/airflow/providers/amazon/aws/hooks/ssm.py
+-rw-r--r--   0 root         (0) root         (0)     3074 2023-06-29 05:49:29.000000 apache-airflow-providers-amazon-8.3.0rc1/airflow/providers/amazon/aws/hooks/step_function.py
+-rw-r--r--   0 root         (0) root         (0)     1818 2023-06-29 05:49:29.000000 apache-airflow-providers-amazon-8.3.0rc1/airflow/providers/amazon/aws/hooks/sts.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-05 07:29:32.824555 apache-airflow-providers-amazon-8.3.0rc1/airflow/providers/amazon/aws/links/
+-rw-r--r--   0 root         (0) root         (0)      785 2023-06-01 06:14:28.000000 apache-airflow-providers-amazon-8.3.0rc1/airflow/providers/amazon/aws/links/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     2946 2023-06-08 05:42:54.000000 apache-airflow-providers-amazon-8.3.0rc1/airflow/providers/amazon/aws/links/base_aws.py
+-rw-r--r--   0 root         (0) root         (0)     1770 2023-06-08 05:42:54.000000 apache-airflow-providers-amazon-8.3.0rc1/airflow/providers/amazon/aws/links/batch.py
+-rw-r--r--   0 root         (0) root         (0)     2519 2023-06-29 05:49:29.000000 apache-airflow-providers-amazon-8.3.0rc1/airflow/providers/amazon/aws/links/emr.py
+-rw-r--r--   0 root         (0) root         (0)     1229 2023-06-08 05:42:54.000000 apache-airflow-providers-amazon-8.3.0rc1/airflow/providers/amazon/aws/links/glue.py
+-rw-r--r--   0 root         (0) root         (0)     1608 2023-06-08 05:42:54.000000 apache-airflow-providers-amazon-8.3.0rc1/airflow/providers/amazon/aws/links/logs.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-05 07:29:32.835000 apache-airflow-providers-amazon-8.3.0rc1/airflow/providers/amazon/aws/log/
+-rw-r--r--   0 root         (0) root         (0)      785 2023-06-01 06:14:28.000000 apache-airflow-providers-amazon-8.3.0rc1/airflow/providers/amazon/aws/log/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     5057 2023-06-01 07:44:14.000000 apache-airflow-providers-amazon-8.3.0rc1/airflow/providers/amazon/aws/log/cloudwatch_task_handler.py
+-rw-r--r--   0 root         (0) root         (0)     9600 2023-06-29 05:49:29.000000 apache-airflow-providers-amazon-8.3.0rc1/airflow/providers/amazon/aws/log/s3_task_handler.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-05 07:29:32.841548 apache-airflow-providers-amazon-8.3.0rc1/airflow/providers/amazon/aws/notifications/
+-rw-r--r--   0 root         (0) root         (0)      785 2023-06-29 05:49:29.000000 apache-airflow-providers-amazon-8.3.0rc1/airflow/providers/amazon/aws/notifications/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     2319 2023-06-29 05:49:29.000000 apache-airflow-providers-amazon-8.3.0rc1/airflow/providers/amazon/aws/notifications/chime.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-05 07:29:32.921658 apache-airflow-providers-amazon-8.3.0rc1/airflow/providers/amazon/aws/operators/
+-rw-r--r--   0 root         (0) root         (0)      785 2023-06-01 06:14:28.000000 apache-airflow-providers-amazon-8.3.0rc1/airflow/providers/amazon/aws/operators/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    19662 2023-06-01 07:44:14.000000 apache-airflow-providers-amazon-8.3.0rc1/airflow/providers/amazon/aws/operators/appflow.py
+-rw-r--r--   0 root         (0) root         (0)     7164 2023-07-05 07:19:39.000000 apache-airflow-providers-amazon-8.3.0rc1/airflow/providers/amazon/aws/operators/athena.py
+-rw-r--r--   0 root         (0) root         (0)    20439 2023-07-05 07:19:39.000000 apache-airflow-providers-amazon-8.3.0rc1/airflow/providers/amazon/aws/operators/batch.py
+-rw-r--r--   0 root         (0) root         (0)     3633 2023-06-01 06:14:28.000000 apache-airflow-providers-amazon-8.3.0rc1/airflow/providers/amazon/aws/operators/cloud_formation.py
+-rw-r--r--   0 root         (0) root         (0)    18421 2023-06-08 05:42:54.000000 apache-airflow-providers-amazon-8.3.0rc1/airflow/providers/amazon/aws/operators/datasync.py
+-rw-r--r--   0 root         (0) root         (0)    10720 2023-06-08 05:42:54.000000 apache-airflow-providers-amazon-8.3.0rc1/airflow/providers/amazon/aws/operators/dms.py
+-rw-r--r--   0 root         (0) root         (0)     9591 2023-06-08 05:42:54.000000 apache-airflow-providers-amazon-8.3.0rc1/airflow/providers/amazon/aws/operators/ec2.py
+-rw-r--r--   0 root         (0) root         (0)    33364 2023-07-05 07:19:39.000000 apache-airflow-providers-amazon-8.3.0rc1/airflow/providers/amazon/aws/operators/ecs.py
+-rw-r--r--   0 root         (0) root         (0)    43249 2023-07-05 07:19:39.000000 apache-airflow-providers-amazon-8.3.0rc1/airflow/providers/amazon/aws/operators/eks.py
+-rw-r--r--   0 root         (0) root         (0)    65005 2023-07-05 07:19:39.000000 apache-airflow-providers-amazon-8.3.0rc1/airflow/providers/amazon/aws/operators/emr.py
+-rw-r--r--   0 root         (0) root         (0)     3707 2023-06-08 05:42:54.000000 apache-airflow-providers-amazon-8.3.0rc1/airflow/providers/amazon/aws/operators/glacier.py
+-rw-r--r--   0 root         (0) root         (0)     9663 2023-07-05 07:19:39.000000 apache-airflow-providers-amazon-8.3.0rc1/airflow/providers/amazon/aws/operators/glue.py
+-rw-r--r--   0 root         (0) root         (0)     4349 2023-07-05 07:19:39.000000 apache-airflow-providers-amazon-8.3.0rc1/airflow/providers/amazon/aws/operators/glue_crawler.py
+-rw-r--r--   0 root         (0) root         (0)     7749 2023-07-03 06:46:02.000000 apache-airflow-providers-amazon-8.3.0rc1/airflow/providers/amazon/aws/operators/lambda_function.py
+-rw-r--r--   0 root         (0) root         (0)     3968 2023-06-29 05:49:29.000000 apache-airflow-providers-amazon-8.3.0rc1/airflow/providers/amazon/aws/operators/quicksight.py
+-rw-r--r--   0 root         (0) root         (0)    35167 2023-07-05 07:19:39.000000 apache-airflow-providers-amazon-8.3.0rc1/airflow/providers/amazon/aws/operators/rds.py
+-rw-r--r--   0 root         (0) root         (0)    32273 2023-07-05 07:19:39.000000 apache-airflow-providers-amazon-8.3.0rc1/airflow/providers/amazon/aws/operators/redshift_cluster.py
+-rw-r--r--   0 root         (0) root         (0)     5547 2023-06-08 05:42:54.000000 apache-airflow-providers-amazon-8.3.0rc1/airflow/providers/amazon/aws/operators/redshift_data.py
+-rw-r--r--   0 root         (0) root         (0)    30235 2023-06-29 05:49:29.000000 apache-airflow-providers-amazon-8.3.0rc1/airflow/providers/amazon/aws/operators/s3.py
+-rw-r--r--   0 root         (0) root         (0)    58086 2023-07-05 07:19:39.000000 apache-airflow-providers-amazon-8.3.0rc1/airflow/providers/amazon/aws/operators/sagemaker.py
+-rw-r--r--   0 root         (0) root         (0)     2960 2023-06-08 05:42:54.000000 apache-airflow-providers-amazon-8.3.0rc1/airflow/providers/amazon/aws/operators/sns.py
+-rw-r--r--   0 root         (0) root         (0)     3565 2023-06-08 05:42:54.000000 apache-airflow-providers-amazon-8.3.0rc1/airflow/providers/amazon/aws/operators/sqs.py
+-rw-r--r--   0 root         (0) root         (0)     4583 2023-06-01 06:14:28.000000 apache-airflow-providers-amazon-8.3.0rc1/airflow/providers/amazon/aws/operators/step_function.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-05 07:29:32.931314 apache-airflow-providers-amazon-8.3.0rc1/airflow/providers/amazon/aws/secrets/
+-rw-r--r--   0 root         (0) root         (0)      785 2023-06-01 06:14:28.000000 apache-airflow-providers-amazon-8.3.0rc1/airflow/providers/amazon/aws/secrets/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    15625 2023-06-08 05:42:54.000000 apache-airflow-providers-amazon-8.3.0rc1/airflow/providers/amazon/aws/secrets/secrets_manager.py
+-rw-r--r--   0 root         (0) root         (0)     8495 2023-06-08 05:42:54.000000 apache-airflow-providers-amazon-8.3.0rc1/airflow/providers/amazon/aws/secrets/systems_manager.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-05 07:29:32.999283 apache-airflow-providers-amazon-8.3.0rc1/airflow/providers/amazon/aws/sensors/
+-rw-r--r--   0 root         (0) root         (0)      785 2023-06-01 06:14:28.000000 apache-airflow-providers-amazon-8.3.0rc1/airflow/providers/amazon/aws/sensors/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     3057 2023-06-29 05:49:29.000000 apache-airflow-providers-amazon-8.3.0rc1/airflow/providers/amazon/aws/sensors/athena.py
+-rw-r--r--   0 root         (0) root         (0)     9059 2023-07-05 07:19:39.000000 apache-airflow-providers-amazon-8.3.0rc1/airflow/providers/amazon/aws/sensors/batch.py
+-rw-r--r--   0 root         (0) root         (0)     4150 2023-06-08 05:42:54.000000 apache-airflow-providers-amazon-8.3.0rc1/airflow/providers/amazon/aws/sensors/cloud_formation.py
+-rw-r--r--   0 root         (0) root         (0)     3984 2023-06-08 05:42:54.000000 apache-airflow-providers-amazon-8.3.0rc1/airflow/providers/amazon/aws/sensors/dms.py
+-rw-r--r--   0 root         (0) root         (0)     4424 2023-06-08 05:42:54.000000 apache-airflow-providers-amazon-8.3.0rc1/airflow/providers/amazon/aws/sensors/dynamodb.py
+-rw-r--r--   0 root         (0) root         (0)     3721 2023-07-05 07:19:39.000000 apache-airflow-providers-amazon-8.3.0rc1/airflow/providers/amazon/aws/sensors/ec2.py
+-rw-r--r--   0 root         (0) root         (0)     7063 2023-06-29 05:49:29.000000 apache-airflow-providers-amazon-8.3.0rc1/airflow/providers/amazon/aws/sensors/ecs.py
+-rw-r--r--   0 root         (0) root         (0)     9772 2023-06-29 05:49:29.000000 apache-airflow-providers-amazon-8.3.0rc1/airflow/providers/amazon/aws/sensors/eks.py
+-rw-r--r--   0 root         (0) root         (0)    22898 2023-07-05 07:19:39.000000 apache-airflow-providers-amazon-8.3.0rc1/airflow/providers/amazon/aws/sensors/emr.py
+-rw-r--r--   0 root         (0) root         (0)     4115 2023-06-08 05:42:54.000000 apache-airflow-providers-amazon-8.3.0rc1/airflow/providers/amazon/aws/sensors/glacier.py
+-rw-r--r--   0 root         (0) root         (0)     3319 2023-06-08 05:42:54.000000 apache-airflow-providers-amazon-8.3.0rc1/airflow/providers/amazon/aws/sensors/glue.py
+-rw-r--r--   0 root         (0) root         (0)     3719 2023-06-08 05:42:54.000000 apache-airflow-providers-amazon-8.3.0rc1/airflow/providers/amazon/aws/sensors/glue_catalog_partition.py
+-rw-r--r--   0 root         (0) root         (0)     2951 2023-06-08 05:42:54.000000 apache-airflow-providers-amazon-8.3.0rc1/airflow/providers/amazon/aws/sensors/glue_crawler.py
+-rw-r--r--   0 root         (0) root         (0)     3027 2023-06-29 05:49:29.000000 apache-airflow-providers-amazon-8.3.0rc1/airflow/providers/amazon/aws/sensors/lambda_function.py
+-rw-r--r--   0 root         (0) root         (0)     3626 2023-06-01 07:44:14.000000 apache-airflow-providers-amazon-8.3.0rc1/airflow/providers/amazon/aws/sensors/quicksight.py
+-rw-r--r--   0 root         (0) root         (0)     6434 2023-06-08 05:42:54.000000 apache-airflow-providers-amazon-8.3.0rc1/airflow/providers/amazon/aws/sensors/rds.py
+-rw-r--r--   0 root         (0) root         (0)     2623 2023-06-08 05:42:54.000000 apache-airflow-providers-amazon-8.3.0rc1/airflow/providers/amazon/aws/sensors/redshift_cluster.py
+-rw-r--r--   0 root         (0) root         (0)    15073 2023-07-05 07:19:39.000000 apache-airflow-providers-amazon-8.3.0rc1/airflow/providers/amazon/aws/sensors/s3.py
+-rw-r--r--   0 root         (0) root         (0)    12794 2023-06-29 05:49:29.000000 apache-airflow-providers-amazon-8.3.0rc1/airflow/providers/amazon/aws/sensors/sagemaker.py
+-rw-r--r--   0 root         (0) root         (0)     9543 2023-06-29 05:49:29.000000 apache-airflow-providers-amazon-8.3.0rc1/airflow/providers/amazon/aws/sensors/sqs.py
+-rw-r--r--   0 root         (0) root         (0)     3333 2023-06-29 05:49:29.000000 apache-airflow-providers-amazon-8.3.0rc1/airflow/providers/amazon/aws/sensors/step_function.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-05 07:29:33.062979 apache-airflow-providers-amazon-8.3.0rc1/airflow/providers/amazon/aws/transfers/
+-rw-r--r--   0 root         (0) root         (0)      785 2023-06-01 06:14:28.000000 apache-airflow-providers-amazon-8.3.0rc1/airflow/providers/amazon/aws/transfers/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     7019 2023-07-04 06:09:02.000000 apache-airflow-providers-amazon-8.3.0rc1/airflow/providers/amazon/aws/transfers/azure_blob_to_s3.py
+-rw-r--r--   0 root         (0) root         (0)     2850 2023-06-08 05:42:54.000000 apache-airflow-providers-amazon-8.3.0rc1/airflow/providers/amazon/aws/transfers/base.py
+-rw-r--r--   0 root         (0) root         (0)     7747 2023-06-29 05:49:29.000000 apache-airflow-providers-amazon-8.3.0rc1/airflow/providers/amazon/aws/transfers/dynamodb_to_s3.py
+-rw-r--r--   0 root         (0) root         (0)     4410 2023-06-01 06:14:28.000000 apache-airflow-providers-amazon-8.3.0rc1/airflow/providers/amazon/aws/transfers/exasol_to_s3.py
+-rw-r--r--   0 root         (0) root         (0)     6368 2023-06-29 05:49:29.000000 apache-airflow-providers-amazon-8.3.0rc1/airflow/providers/amazon/aws/transfers/ftp_to_s3.py
+-rw-r--r--   0 root         (0) root         (0)     8544 2023-07-05 07:19:39.000000 apache-airflow-providers-amazon-8.3.0rc1/airflow/providers/amazon/aws/transfers/gcs_to_s3.py
+-rw-r--r--   0 root         (0) root         (0)     4702 2023-06-08 05:42:54.000000 apache-airflow-providers-amazon-8.3.0rc1/airflow/providers/amazon/aws/transfers/glacier_to_gcs.py
+-rw-r--r--   0 root         (0) root         (0)     9042 2023-06-01 06:14:28.000000 apache-airflow-providers-amazon-8.3.0rc1/airflow/providers/amazon/aws/transfers/google_api_to_s3.py
+-rw-r--r--   0 root         (0) root         (0)     4173 2023-06-29 05:49:29.000000 apache-airflow-providers-amazon-8.3.0rc1/airflow/providers/amazon/aws/transfers/hive_to_dynamodb.py
+-rw-r--r--   0 root         (0) root         (0)     4248 2023-06-01 06:14:28.000000 apache-airflow-providers-amazon-8.3.0rc1/airflow/providers/amazon/aws/transfers/imap_attachment_to_s3.py
+-rw-r--r--   0 root         (0) root         (0)     4158 2023-06-01 06:14:28.000000 apache-airflow-providers-amazon-8.3.0rc1/airflow/providers/amazon/aws/transfers/local_to_s3.py
+-rw-r--r--   0 root         (0) root         (0)     5981 2023-06-17 16:45:00.000000 apache-airflow-providers-amazon-8.3.0rc1/airflow/providers/amazon/aws/transfers/mongo_to_s3.py
+-rw-r--r--   0 root         (0) root         (0)     8108 2023-06-01 06:14:28.000000 apache-airflow-providers-amazon-8.3.0rc1/airflow/providers/amazon/aws/transfers/redshift_to_s3.py
+-rw-r--r--   0 root         (0) root         (0)     2966 2023-06-01 06:14:28.000000 apache-airflow-providers-amazon-8.3.0rc1/airflow/providers/amazon/aws/transfers/s3_to_ftp.py
+-rw-r--r--   0 root         (0) root         (0)     8287 2023-06-08 05:42:54.000000 apache-airflow-providers-amazon-8.3.0rc1/airflow/providers/amazon/aws/transfers/s3_to_redshift.py
+-rw-r--r--   0 root         (0) root         (0)     3191 2023-06-01 06:14:28.000000 apache-airflow-providers-amazon-8.3.0rc1/airflow/providers/amazon/aws/transfers/s3_to_sftp.py
+-rw-r--r--   0 root         (0) root         (0)     4634 2023-06-17 16:45:00.000000 apache-airflow-providers-amazon-8.3.0rc1/airflow/providers/amazon/aws/transfers/s3_to_sql.py
+-rw-r--r--   0 root         (0) root         (0)     5679 2023-06-01 06:14:28.000000 apache-airflow-providers-amazon-8.3.0rc1/airflow/providers/amazon/aws/transfers/salesforce_to_s3.py
+-rw-r--r--   0 root         (0) root         (0)     3643 2023-06-29 05:49:29.000000 apache-airflow-providers-amazon-8.3.0rc1/airflow/providers/amazon/aws/transfers/sftp_to_s3.py
+-rw-r--r--   0 root         (0) root         (0)     8865 2023-06-29 05:49:29.000000 apache-airflow-providers-amazon-8.3.0rc1/airflow/providers/amazon/aws/transfers/sql_to_s3.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-05 07:29:33.103509 apache-airflow-providers-amazon-8.3.0rc1/airflow/providers/amazon/aws/triggers/
+-rw-r--r--   0 root         (0) root         (0)      787 2023-06-01 06:14:28.000000 apache-airflow-providers-amazon-8.3.0rc1/airflow/providers/amazon/aws/triggers/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     3154 2023-06-28 06:26:40.000000 apache-airflow-providers-amazon-8.3.0rc1/airflow/providers/amazon/aws/triggers/athena.py
+-rw-r--r--   0 root         (0) root         (0)     9670 2023-06-29 05:49:29.000000 apache-airflow-providers-amazon-8.3.0rc1/airflow/providers/amazon/aws/triggers/batch.py
+-rw-r--r--   0 root         (0) root         (0)     2942 2023-06-29 05:49:29.000000 apache-airflow-providers-amazon-8.3.0rc1/airflow/providers/amazon/aws/triggers/ec2.py
+-rw-r--r--   0 root         (0) root         (0)     8212 2023-06-29 05:49:29.000000 apache-airflow-providers-amazon-8.3.0rc1/airflow/providers/amazon/aws/triggers/ecs.py
+-rw-r--r--   0 root         (0) root         (0)     9760 2023-06-29 05:49:29.000000 apache-airflow-providers-amazon-8.3.0rc1/airflow/providers/amazon/aws/triggers/eks.py
+-rw-r--r--   0 root         (0) root         (0)    14727 2023-06-29 05:49:29.000000 apache-airflow-providers-amazon-8.3.0rc1/airflow/providers/amazon/aws/triggers/emr.py
+-rw-r--r--   0 root         (0) root         (0)     2567 2023-06-28 06:26:40.000000 apache-airflow-providers-amazon-8.3.0rc1/airflow/providers/amazon/aws/triggers/glue.py
+-rw-r--r--   0 root         (0) root         (0)     3090 2023-06-08 05:42:54.000000 apache-airflow-providers-amazon-8.3.0rc1/airflow/providers/amazon/aws/triggers/glue_crawler.py
+-rw-r--r--   0 root         (0) root         (0)     3874 2023-06-29 05:49:29.000000 apache-airflow-providers-amazon-8.3.0rc1/airflow/providers/amazon/aws/triggers/rds.py
+-rw-r--r--   0 root         (0) root         (0)    14450 2023-06-08 05:42:54.000000 apache-airflow-providers-amazon-8.3.0rc1/airflow/providers/amazon/aws/triggers/redshift_cluster.py
+-rw-r--r--   0 root         (0) root         (0)     9085 2023-06-30 08:49:17.000000 apache-airflow-providers-amazon-8.3.0rc1/airflow/providers/amazon/aws/triggers/s3.py
+-rw-r--r--   0 root         (0) root         (0)     4626 2023-06-28 06:26:40.000000 apache-airflow-providers-amazon-8.3.0rc1/airflow/providers/amazon/aws/triggers/sagemaker.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-05 07:29:33.138054 apache-airflow-providers-amazon-8.3.0rc1/airflow/providers/amazon/aws/utils/
+-rw-r--r--   0 root         (0) root         (0)     2265 2023-06-01 06:14:28.000000 apache-airflow-providers-amazon-8.3.0rc1/airflow/providers/amazon/aws/utils/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    20649 2023-06-17 16:45:00.000000 apache-airflow-providers-amazon-8.3.0rc1/airflow/providers/amazon/aws/utils/connection_wrapper.py
+-rw-r--r--   0 root         (0) root         (0)     2561 2023-06-01 06:14:28.000000 apache-airflow-providers-amazon-8.3.0rc1/airflow/providers/amazon/aws/utils/eks_get_token.py
+-rw-r--r--   0 root         (0) root         (0)     1854 2023-06-08 05:42:54.000000 apache-airflow-providers-amazon-8.3.0rc1/airflow/providers/amazon/aws/utils/emailer.py
+-rw-r--r--   0 root         (0) root         (0)      973 2023-06-08 05:42:54.000000 apache-airflow-providers-amazon-8.3.0rc1/airflow/providers/amazon/aws/utils/rds.py
+-rw-r--r--   0 root         (0) root         (0)     1897 2023-06-17 16:45:00.000000 apache-airflow-providers-amazon-8.3.0rc1/airflow/providers/amazon/aws/utils/redshift.py
+-rw-r--r--   0 root         (0) root         (0)     1040 2023-06-01 06:14:28.000000 apache-airflow-providers-amazon-8.3.0rc1/airflow/providers/amazon/aws/utils/sagemaker.py
+-rw-r--r--   0 root         (0) root         (0)     1762 2023-06-29 05:49:30.000000 apache-airflow-providers-amazon-8.3.0rc1/airflow/providers/amazon/aws/utils/tags.py
+-rw-r--r--   0 root         (0) root         (0)     4491 2023-06-29 05:49:30.000000 apache-airflow-providers-amazon-8.3.0rc1/airflow/providers/amazon/aws/utils/task_log_fetcher.py
+-rw-r--r--   0 root         (0) root         (0)     3509 2023-06-29 05:49:30.000000 apache-airflow-providers-amazon-8.3.0rc1/airflow/providers/amazon/aws/utils/waiter.py
+-rw-r--r--   0 root         (0) root         (0)     5890 2023-06-30 08:49:17.000000 apache-airflow-providers-amazon-8.3.0rc1/airflow/providers/amazon/aws/utils/waiter_with_logging.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-05 07:29:33.191341 apache-airflow-providers-amazon-8.3.0rc1/airflow/providers/amazon/aws/waiters/
+-rw-r--r--   0 root         (0) root         (0)      785 2023-06-01 06:14:28.000000 apache-airflow-providers-amazon-8.3.0rc1/airflow/providers/amazon/aws/waiters/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1002 2023-06-01 06:14:28.000000 apache-airflow-providers-amazon-8.3.0rc1/airflow/providers/amazon/aws/waiters/appflow.json
+-rw-r--r--   0 root         (0) root         (0)      892 2023-06-24 10:23:43.000000 apache-airflow-providers-amazon-8.3.0rc1/airflow/providers/amazon/aws/waiters/athena.json
+-rw-r--r--   0 root         (0) root         (0)     1853 2023-06-01 06:14:28.000000 apache-airflow-providers-amazon-8.3.0rc1/airflow/providers/amazon/aws/waiters/base_waiter.py
+-rw-r--r--   0 root         (0) root         (0)     1203 2023-06-28 06:26:40.000000 apache-airflow-providers-amazon-8.3.0rc1/airflow/providers/amazon/aws/waiters/batch.json
+-rw-r--r--   0 root         (0) root         (0)      895 2023-06-01 06:14:28.000000 apache-airflow-providers-amazon-8.3.0rc1/airflow/providers/amazon/aws/waiters/dynamodb.json
+-rw-r--r--   0 root         (0) root         (0)     1674 2023-06-17 16:45:00.000000 apache-airflow-providers-amazon-8.3.0rc1/airflow/providers/amazon/aws/waiters/ecs.json
+-rw-r--r--   0 root         (0) root         (0)      659 2023-06-01 06:14:28.000000 apache-airflow-providers-amazon-8.3.0rc1/airflow/providers/amazon/aws/waiters/eks.json
+-rw-r--r--   0 root         (0) root         (0)      851 2023-06-20 06:40:52.000000 apache-airflow-providers-amazon-8.3.0rc1/airflow/providers/amazon/aws/waiters/emr-containers.json
+-rw-r--r--   0 root         (0) root         (0)     4893 2023-06-24 10:23:12.000000 apache-airflow-providers-amazon-8.3.0rc1/airflow/providers/amazon/aws/waiters/emr-serverless.json
+-rw-r--r--   0 root         (0) root         (0)     4242 2023-06-28 06:26:40.000000 apache-airflow-providers-amazon-8.3.0rc1/airflow/providers/amazon/aws/waiters/emr.json
+-rw-r--r--   0 root         (0) root         (0)      932 2023-06-01 07:44:14.000000 apache-airflow-providers-amazon-8.3.0rc1/airflow/providers/amazon/aws/waiters/glue.json
+-rw-r--r--   0 root         (0) root         (0)     1742 2023-06-01 06:14:28.000000 apache-airflow-providers-amazon-8.3.0rc1/airflow/providers/amazon/aws/waiters/redshift.json
+-rw-r--r--   0 root         (0) root         (0)     3625 2023-06-28 06:26:40.000000 apache-airflow-providers-amazon-8.3.0rc1/airflow/providers/amazon/aws/waiters/sagemaker.json
+-rw-r--r--   0 root         (0) root         (0)    40167 2023-07-05 07:29:30.000000 apache-airflow-providers-amazon-8.3.0rc1/airflow/providers/amazon/get_provider_info.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-05 07:29:33.216689 apache-airflow-providers-amazon-8.3.0rc1/apache_airflow_providers_amazon.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     8022 2023-07-05 07:29:32.000000 apache-airflow-providers-amazon-8.3.0rc1/apache_airflow_providers_amazon.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     8457 2023-07-05 07:29:32.000000 apache-airflow-providers-amazon-8.3.0rc1/apache_airflow_providers_amazon.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-05 07:29:32.000000 apache-airflow-providers-amazon-8.3.0rc1/apache_airflow_providers_amazon.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      103 2023-07-05 07:29:32.000000 apache-airflow-providers-amazon-8.3.0rc1/apache_airflow_providers_amazon.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-05 07:29:32.000000 apache-airflow-providers-amazon-8.3.0rc1/apache_airflow_providers_amazon.egg-info/not-zip-safe
+-rw-r--r--   0 root         (0) root         (0)      949 2023-07-05 07:29:32.000000 apache-airflow-providers-amazon-8.3.0rc1/apache_airflow_providers_amazon.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        8 2023-07-05 07:29:32.000000 apache-airflow-providers-amazon-8.3.0rc1/apache_airflow_providers_amazon.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)     5424 2023-06-24 10:23:12.000000 apache-airflow-providers-amazon-8.3.0rc1/pyproject.toml
+-rw-r--r--   0 root         (0) root         (0)     2243 2023-07-05 07:29:33.221869 apache-airflow-providers-amazon-8.3.0rc1/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     2502 2023-07-05 07:29:30.000000 apache-airflow-providers-amazon-8.3.0rc1/setup.py
```

### Comparing `apache-airflow-providers-amazon-8.2.0rc1/LICENSE` & `apache-airflow-providers-amazon-8.3.0rc1/LICENSE`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-amazon-8.2.0rc1/MANIFEST.in` & `apache-airflow-providers-amazon-8.3.0rc1/MANIFEST.in`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-amazon-8.2.0rc1/airflow/providers/amazon/__init__.py` & `apache-airflow-providers-amazon-8.3.0rc1/airflow/providers/amazon/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -24,15 +24,15 @@
 #
 from __future__ import annotations
 
 import packaging.version
 
 __all__ = ["__version__"]
 
-__version__ = "8.2.0"
+__version__ = "8.3.0"
 
 try:
     from airflow import __version__ as airflow_version
 except ImportError:
     from airflow.version import version as airflow_version
 
 if packaging.version.parse(airflow_version) < packaging.version.parse("2.4.0"):
```

### Comparing `apache-airflow-providers-amazon-8.2.0rc1/airflow/providers/amazon/aws/__init__.py` & `apache-airflow-providers-amazon-8.3.0rc1/airflow/providers/amazon/aws/__init__.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-amazon-8.2.0rc1/airflow/providers/amazon/aws/exceptions.py` & `apache-airflow-providers-amazon-8.3.0rc1/airflow/providers/amazon/aws/exceptions.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-amazon-8.2.0rc1/airflow/providers/amazon/aws/hooks/__init__.py` & `apache-airflow-providers-amazon-8.3.0rc1/airflow/providers/amazon/aws/hooks/__init__.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-amazon-8.2.0rc1/airflow/providers/amazon/aws/hooks/appflow.py` & `apache-airflow-providers-amazon-8.3.0rc1/airflow/providers/amazon/aws/hooks/appflow.py`

 * *Files 0% similar despite different names*

```diff
@@ -25,14 +25,15 @@
     from mypy_boto3_appflow.client import AppflowClient
     from mypy_boto3_appflow.type_defs import TaskTypeDef
 
 
 class AppflowHook(AwsBaseHook):
     """
     Interact with Amazon Appflow.
+
     Provide thin wrapper around :external+boto3:py:class:`boto3.client("appflow") <Appflow.Client>`.
 
     Additional arguments (such as ``aws_conn_id``) may be specified and
     are passed down to the underlying AwsBaseHook.
 
     .. seealso::
         - :class:`airflow.providers.amazon.aws.hooks.base_aws.AwsBaseHook`
@@ -76,16 +77,15 @@
         exec_details = last_execs[execution_id]
         self.log.info("Run complete, execution details: %s", exec_details)
 
     def update_flow_filter(
         self, flow_name: str, filter_tasks: list[TaskTypeDef], set_trigger_ondemand: bool = False
     ) -> None:
         """
-        Update the flow task filter.
-        All filters will be removed if an empty array is passed to filter_tasks.
+        Update the flow task filter; all filters will be removed if an empty array is passed to filter_tasks.
 
         :param flow_name: The flow name
         :param filter_tasks: List flow tasks to be added
         :param set_trigger_ondemand: If True, set the trigger to on-demand; otherwise, keep the trigger as is
         :return: None
         """
         response = self.conn.describe_flow(flowName=flow_name)
```

### Comparing `apache-airflow-providers-amazon-8.2.0rc1/airflow/providers/amazon/aws/hooks/athena.py` & `apache-airflow-providers-amazon-8.3.0rc1/airflow/providers/amazon/aws/hooks/athena.py`

 * *Files 3% similar despite different names*

```diff
@@ -20,30 +20,31 @@
 
 .. spelling:word-list::
 
     PageIterator
 """
 from __future__ import annotations
 
-from time import sleep
+import warnings
 from typing import Any
 
 from botocore.paginate import PageIterator
 
+from airflow.exceptions import AirflowException, AirflowProviderDeprecationWarning
 from airflow.providers.amazon.aws.hooks.base_aws import AwsBaseHook
+from airflow.providers.amazon.aws.utils.waiter_with_logging import wait
 
 
 class AthenaHook(AwsBaseHook):
     """Interact with Amazon Athena.
 
     Provide thick wrapper around
     :external+boto3:py:class:`boto3.client("athena") <Athena.Client>`.
 
-    :param sleep_time: Time (in seconds) to wait between two consecutive calls
-        to check query status on Athena.
+    :param sleep_time: obsolete, please use the parameter of `poll_query_status` method instead
     :param log_query: Whether to log athena query and other execution params
         when it's executed. Defaults to *True*.
 
     Additional arguments (such as ``aws_conn_id``) may be specified and
     are passed down to the underlying AwsBaseHook.
 
     .. seealso::
@@ -61,17 +62,28 @@
     SUCCESS_STATES = ("SUCCEEDED",)
     TERMINAL_STATES = (
         "SUCCEEDED",
         "FAILED",
         "CANCELLED",
     )
 
-    def __init__(self, *args: Any, sleep_time: int = 30, log_query: bool = True, **kwargs: Any) -> None:
+    def __init__(
+        self, *args: Any, sleep_time: int | None = None, log_query: bool = True, **kwargs: Any
+    ) -> None:
         super().__init__(client_type="athena", *args, **kwargs)  # type: ignore
-        self.sleep_time = sleep_time
+        if sleep_time is not None:
+            self.sleep_time = sleep_time
+            warnings.warn(
+                "The `sleep_time` parameter of the Athena hook is deprecated, "
+                "please pass this parameter to the poll_query_status method instead.",
+                AirflowProviderDeprecationWarning,
+                stacklevel=2,
+            )
+        else:
+            self.sleep_time = 30  # previous default value
         self.log_query = log_query
 
     def run_query(
         self,
         query: str,
         query_context: dict[str, str],
         result_configuration: dict[str, Any],
@@ -225,59 +237,39 @@
                 "StartingToken": starting_token,
             },
         }
         paginator = self.get_conn().get_paginator("get_query_results")
         return paginator.paginate(**result_params)
 
     def poll_query_status(
-        self,
-        query_execution_id: str,
-        max_polling_attempts: int | None = None,
+        self, query_execution_id: str, max_polling_attempts: int | None = None, sleep_time: int | None = None
     ) -> str | None:
         """Poll the state of a submitted query until it reaches final state.
 
         :param query_execution_id: ID of submitted athena query
-        :param max_polling_attempts: Number of times to poll for query state
-            before function exits
+        :param max_polling_attempts: Number of times to poll for query state before function exits
+        :param sleep_time: Time (in seconds) to wait between two consecutive query status checks.
         :return: One of the final states
         """
-        try_number = 1
-        final_query_state = None  # Query state when query reaches final state or max_polling_attempts reached
-        while True:
-            query_state = self.check_query_status(query_execution_id)
-            if query_state is None:
-                self.log.info(
-                    "Query execution id: %s, trial %s: Invalid query state. Retrying again",
-                    query_execution_id,
-                    try_number,
-                )
-            elif query_state in self.TERMINAL_STATES:
-                self.log.info(
-                    "Query execution id: %s, trial %s: Query execution completed. Final state is %s",
-                    query_execution_id,
-                    try_number,
-                    query_state,
-                )
-                final_query_state = query_state
-                break
-            else:
-                self.log.info(
-                    "Query execution id: %s, trial %s: Query is still in non-terminal state - %s",
-                    query_execution_id,
-                    try_number,
-                    query_state,
-                )
-            if (
-                max_polling_attempts and try_number >= max_polling_attempts
-            ):  # Break loop if max_polling_attempts reached
-                final_query_state = query_state
-                break
-            try_number += 1
-            sleep(self.sleep_time)
-        return final_query_state
+        try:
+            wait(
+                waiter=self.get_waiter("query_complete"),
+                waiter_delay=sleep_time or self.sleep_time,
+                waiter_max_attempts=max_polling_attempts or 120,
+                args={"QueryExecutionId": query_execution_id},
+                failure_message=f"Error while waiting for query {query_execution_id} to complete",
+                status_message=f"Query execution id: {query_execution_id}, "
+                f"Query is still in non-terminal state",
+                status_args=["QueryExecution.Status.State"],
+            )
+        except AirflowException as error:
+            # this function does not raise errors to keep previous behavior.
+            self.log.warning(error)
+        finally:
+            return self.check_query_status(query_execution_id)
 
     def get_output_location(self, query_execution_id: str) -> str:
         """Get the output location of the query results in S3 URI format.
 
         .. seealso::
             - :external+boto3:py:meth:`Athena.Client.get_query_execution`
```

### Comparing `apache-airflow-providers-amazon-8.2.0rc1/airflow/providers/amazon/aws/hooks/base_aws.py` & `apache-airflow-providers-amazon-8.3.0rc1/airflow/providers/amazon/aws/hooks/base_aws.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-amazon-8.2.0rc1/airflow/providers/amazon/aws/hooks/batch_client.py` & `apache-airflow-providers-amazon-8.3.0rc1/airflow/providers/amazon/aws/hooks/batch_client.py`

 * *Files 1% similar despite different names*

```diff
@@ -40,14 +40,15 @@
 from airflow.typing_compat import Protocol, runtime_checkable
 
 
 @runtime_checkable
 class BatchProtocol(Protocol):
     """
     A structured Protocol for ``boto3.client('batch') -> botocore.client.Batch``.
+
     This is used for type hints on :py:meth:`.BatchClient.client`; it covers
     only the subset of client methods required.
 
     .. seealso::
 
         - https://mypy.readthedocs.io/en/latest/protocols.html
         - https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/batch.html
@@ -136,14 +137,15 @@
 # Note that the use of invalid-name parameters should be restricted to the boto3 mappings only;
 # all the Airflow wrappers of boto3 clients should not adopt invalid-names to match boto3.
 
 
 class BatchClientHook(AwsBaseHook):
     """
     Interact with AWS Batch.
+
     Provide thick wrapper around :external+boto3:py:class:`boto3.client("batch") <Batch.Client>`.
 
     :param max_retries: exponential back-off retries, 4200 = 48 hours;
         polling is only used when waiters is None
     :param status_retries: number of HTTP retries to get job status, 10;
         polling is only used when waiters is None
 
@@ -285,16 +287,17 @@
             if batch_log_fetcher:
                 batch_log_fetcher.stop()
                 batch_log_fetcher.join()
         self.log.info("AWS Batch job (%s) has completed", job_id)
 
     def poll_for_job_running(self, job_id: str, delay: int | float | None = None) -> None:
         """
-        Poll for job running. The status that indicates a job is running or
-        already complete are: 'RUNNING'|'SUCCEEDED'|'FAILED'.
+        Poll for job running.
+
+        The status that indicates a job is running or already complete are: 'RUNNING'|'SUCCEEDED'|'FAILED'.
 
         So the status options that this will wait for are the transitions from:
         'SUBMITTED'>'PENDING'>'RUNNABLE'>'STARTING'>'RUNNING'|'SUCCEEDED'|'FAILED'
 
         The completed status options are included for cases where the status
         changes too quickly for polling to detect a RUNNING status that moves
         quickly from STARTING to RUNNING to completed (often a failure).
@@ -307,16 +310,17 @@
         """
         self.delay(delay)
         running_status = [self.RUNNING_STATE, self.SUCCESS_STATE, self.FAILURE_STATE]
         self.poll_job_status(job_id, running_status)
 
     def poll_for_job_complete(self, job_id: str, delay: int | float | None = None) -> None:
         """
-        Poll for job completion. The status that indicates job completion
-        are: 'SUCCEEDED'|'FAILED'.
+        Poll for job completion.
+
+        The status that indicates job completion are: 'SUCCEEDED'|'FAILED'.
 
         So the status options that this will wait for are the transitions from:
         'SUBMITTED'>'PENDING'>'RUNNABLE'>'STARTING'>'RUNNING'>'SUCCEEDED'|'FAILED'
 
         :param job_id: a Batch job ID
 
         :param delay: a delay before polling for job status
@@ -551,16 +555,17 @@
         else:
             delay = BatchClientHook.add_jitter(delay)
         sleep(delay)
 
     @staticmethod
     def exponential_delay(tries: int) -> float:
         """
-        An exponential back-off delay, with random jitter.  There is a maximum
-        interval of 10 minutes (with random jitter between 3 and 10 minutes).
+        An exponential back-off delay, with random jitter.
+
+        There is a maximum interval of 10 minutes (with random jitter between 3 and 10 minutes).
         This is used in the :py:meth:`.poll_for_job_status` method.
 
         :param tries: Number of tries
 
 
         Examples of behavior:
```

### Comparing `apache-airflow-providers-amazon-8.2.0rc1/airflow/providers/amazon/aws/hooks/batch_waiters.json` & `apache-airflow-providers-amazon-8.3.0rc1/airflow/providers/amazon/aws/hooks/batch_waiters.json`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-amazon-8.2.0rc1/airflow/providers/amazon/aws/hooks/batch_waiters.py` & `apache-airflow-providers-amazon-8.3.0rc1/airflow/providers/amazon/aws/hooks/batch_waiters.py`

 * *Files 4% similar despite different names*

```diff
@@ -118,18 +118,19 @@
             with open(config_path) as config_file:
                 self._default_config = json.load(config_file)
         return deepcopy(self._default_config)  # avoid accidental mutation
 
     @property
     def waiter_config(self) -> dict:
         """
-        An immutable waiter configuration for this instance; a ``deepcopy`` is returned by this
-        property. During the init for BatchWaiters, the waiter_config is used to build a
-        waiter_model and this only occurs during the class init, to avoid any accidental
-        mutations of waiter_config leaking into the waiter_model.
+        An immutable waiter configuration for this instance; a ``deepcopy`` is returned by this property.
+
+        During the init for BatchWaiters, the waiter_config is used to build a
+        waiter_model and this only occurs during the class init, to avoid any
+        accidental mutations of waiter_config leaking into the waiter_model.
 
         :return: a waiter configuration for AWS Batch services
         """
         return deepcopy(self._waiter_config)  # avoid accidental mutation
 
     @property
     def waiter_model(self) -> botocore.waiter.WaiterModel:
@@ -189,17 +190,19 @@
     def wait_for_job(
         self,
         job_id: str,
         delay: int | float | None = None,
         get_batch_log_fetcher: Callable[[str], AwsTaskLogFetcher | None] | None = None,
     ) -> None:
         """
-        Wait for Batch job to complete.  This assumes that the ``.waiter_model`` is configured
-        using some variation of the ``.default_config`` so that it can generate waiters with the
-        following names: "JobExists", "JobRunning" and "JobComplete".
+        Wait for Batch job to complete.
+
+        This assumes that the ``.waiter_model`` is configured using some
+        variation of the ``.default_config`` so that it can generate waiters
+        with the following names: "JobExists", "JobRunning" and "JobComplete".
 
         :param job_id: a Batch job ID
 
         :param delay:  A delay before polling for job status
 
         :param get_batch_log_fetcher: A method that returns batch_log_fetcher of
             type AwsTaskLogFetcher or None when the CloudWatch log stream hasn't been created yet.
```

### Comparing `apache-airflow-providers-amazon-8.2.0rc1/airflow/providers/amazon/aws/hooks/cloud_formation.py` & `apache-airflow-providers-amazon-8.3.0rc1/airflow/providers/amazon/aws/hooks/cloud_formation.py`

 * *Files 1% similar despite different names*

```diff
@@ -23,14 +23,15 @@
 
 from airflow.providers.amazon.aws.hooks.base_aws import AwsBaseHook
 
 
 class CloudFormationHook(AwsBaseHook):
     """
     Interact with AWS CloudFormation.
+
     Provide thin wrapper around
     :external+boto3:py:class:`boto3.client("cloudformation") <CloudFormation.Client>`.
 
     Additional arguments (such as ``aws_conn_id``) may be specified and
     are passed down to the underlying AwsBaseHook.
 
     .. seealso::
```

### Comparing `apache-airflow-providers-amazon-8.2.0rc1/airflow/providers/amazon/aws/hooks/datasync.py` & `apache-airflow-providers-amazon-8.3.0rc1/airflow/providers/amazon/aws/hooks/datasync.py`

 * *Files 1% similar despite different names*

```diff
@@ -23,14 +23,15 @@
 from airflow.exceptions import AirflowBadRequest, AirflowException, AirflowTaskTimeout
 from airflow.providers.amazon.aws.hooks.base_aws import AwsBaseHook
 
 
 class DataSyncHook(AwsBaseHook):
     """
     Interact with AWS DataSync.
+
     Provide thick wrapper around :external+boto3:py:class:`boto3.client("datasync") <DataSync.Client>`.
 
     Additional arguments (such as ``aws_conn_id``) may be specified and
     are passed down to the underlying AwsBaseHook.
 
     :param wait_interval_seconds: Time to wait between two
         consecutive calls to check TaskExecution status. Defaults to 30 seconds.
@@ -194,16 +195,15 @@
 
     def get_task_arns_for_location_arns(
         self,
         source_location_arns: list,
         destination_location_arns: list,
     ) -> list:
         """
-        Return list of TaskArns for which use any one of the specified
-        source LocationArns and any one of the specified destination LocationArns.
+        Return list of TaskArns which use both a specified source and destination LocationArns.
 
         :param source_location_arns: List of source LocationArns.
         :param destination_location_arns: List of destination LocationArns.
         :raises AirflowBadRequest: if ``source_location_arns`` or ``destination_location_arns`` are empty.
         """
         if not source_location_arns:
             raise AirflowBadRequest("source_location_arns not specified")
@@ -220,14 +220,15 @@
                 if task_description["DestinationLocationArn"] in destination_location_arns:
                     result.append(task_arn)
         return result
 
     def start_task_execution(self, task_arn: str, **kwargs) -> str:
         """
         Start a TaskExecution for the specified task_arn.
+
         Each task can have at most one TaskExecution.
         Additional keyword arguments send to ``start_task_execution`` boto3 method.
 
         .. seealso::
             - :external+boto3:py:meth:`DataSync.Client.start_task_execution`
 
         :param task_arn: TaskArn
@@ -296,14 +297,15 @@
         if "CurrentTaskExecutionArn" in task_description:
             return task_description["CurrentTaskExecutionArn"]
         return None
 
     def wait_for_task_execution(self, task_execution_arn: str, max_iterations: int = 60) -> bool:
         """
         Wait for Task Execution status to be complete (SUCCESS/ERROR).
+
         The ``task_execution_arn`` must exist, or a boto3 ClientError will be raised.
 
         :param task_execution_arn: TaskExecutionArn
         :param max_iterations: Maximum number of iterations before timing out.
         :return: Result of task execution.
         :raises AirflowTaskTimeout: If maximum iterations is exceeded.
         :raises AirflowBadRequest: If ``task_execution_arn`` is empty.
```

### Comparing `apache-airflow-providers-amazon-8.2.0rc1/airflow/providers/amazon/aws/hooks/dms.py` & `apache-airflow-providers-amazon-8.3.0rc1/airflow/providers/amazon/aws/hooks/dms.py`

 * *Files 0% similar despite different names*

```diff
@@ -31,14 +31,15 @@
     RUNNING = "running"
     STOPPED = "stopped"
 
 
 class DmsHook(AwsBaseHook):
     """
     Interact with AWS Database Migration Service (DMS).
+
     Provide thin wrapper around
     :external+boto3:py:class:`boto3.client("dms") <DatabaseMigrationService.Client>`.
 
     Additional arguments (such as ``aws_conn_id``) may be specified and
     are passed down to the underlying AwsBaseHook.
 
     .. seealso::
@@ -193,16 +194,15 @@
         dms_client = self.get_conn()
         dms_client.delete_replication_task(ReplicationTaskArn=replication_task_arn)
 
         self.wait_for_task_status(replication_task_arn, DmsTaskWaiterStatus.DELETED)
 
     def wait_for_task_status(self, replication_task_arn: str, status: DmsTaskWaiterStatus):
         """
-        Waits for replication task to reach status.
-        Supported statuses: deleted, ready, running, stopped.
+        Waits for replication task to reach status; supported statuses: deleted, ready, running, stopped.
 
         :param status: Status to wait for
         :param replication_task_arn: Replication task ARN
         """
         if not isinstance(status, DmsTaskWaiterStatus):
             raise TypeError("Status must be an instance of DmsTaskWaiterStatus")
```

### Comparing `apache-airflow-providers-amazon-8.2.0rc1/airflow/providers/amazon/aws/hooks/dynamodb.py` & `apache-airflow-providers-amazon-8.3.0rc1/airflow/providers/amazon/aws/hooks/dynamodb.py`

 * *Files 1% similar despite different names*

```diff
@@ -23,14 +23,15 @@
 from airflow.exceptions import AirflowException
 from airflow.providers.amazon.aws.hooks.base_aws import AwsBaseHook
 
 
 class DynamoDBHook(AwsBaseHook):
     """
     Interact with Amazon DynamoDB.
+
     Provide thick wrapper around
     :external+boto3:py:class:`boto3.resource("dynamodb") <DynamoDB.ServiceResource>`.
 
     :param table_keys: partition key and sort key
     :param table_name: target DynamoDB table
 
     Additional arguments (such as ``aws_conn_id``) may be specified and
```

### Comparing `apache-airflow-providers-amazon-8.2.0rc1/airflow/providers/amazon/aws/hooks/ec2.py` & `apache-airflow-providers-amazon-8.3.0rc1/airflow/providers/amazon/aws/hooks/ec2.py`

 * *Files 0% similar despite different names*

```diff
@@ -46,14 +46,15 @@
 
     return checker
 
 
 class EC2Hook(AwsBaseHook):
     """
     Interact with Amazon Elastic Compute Cloud (EC2).
+
     Provide thick wrapper around :external+boto3:py:class:`boto3.client("ec2") <EC2.Client>`
     or :external+boto3:py:class:`boto3.resource("ec2") <EC2.ServiceResource>`.
 
     :param api_type: If set to ``client_type`` then hook use ``boto3.client("ec2")`` capabilities,
         If set to ``resource_type`` then hook use ``boto3.resource("ec2")`` capabilities.
 
     Additional arguments (such as ``aws_conn_id``) may be specified and
```

### Comparing `apache-airflow-providers-amazon-8.2.0rc1/airflow/providers/amazon/aws/hooks/ecr.py` & `apache-airflow-providers-amazon-8.3.0rc1/airflow/providers/amazon/aws/hooks/ecr.py`

 * *Files 1% similar despite different names*

```diff
@@ -47,14 +47,15 @@
         # https://github.com/docker/docker-py/issues/2256#issuecomment-824940506
         return self.proxy_endpoint.replace("https://", "")
 
 
 class EcrHook(AwsBaseHook):
     """
     Interact with Amazon Elastic Container Registry (ECR).
+
     Provide thin wrapper around :external+boto3:py:class:`boto3.client("ecr") <ECR.Client>`.
 
     Additional arguments (such as ``aws_conn_id``) may be specified and
     are passed down to the underlying AwsBaseHook.
 
     .. seealso::
         - :class:`airflow.providers.amazon.aws.hooks.base_aws.AwsBaseHook`
```

### Comparing `apache-airflow-providers-amazon-8.2.0rc1/airflow/providers/amazon/aws/hooks/ecs.py` & `apache-airflow-providers-amazon-8.3.0rc1/airflow/providers/amazon/aws/hooks/ecs.py`

 * *Files 1% similar despite different names*

```diff
@@ -77,14 +77,15 @@
     STOPPED = "STOPPED"
     NONE = "NONE"
 
 
 class EcsHook(AwsGenericHook):
     """
     Interact with Amazon Elastic Container Service (ECS).
+
     Provide thin wrapper around :external+boto3:py:class:`boto3.client("ecs") <ECS.Client>`.
 
     Additional arguments (such as ``aws_conn_id``) may be specified and
     are passed down to the underlying AwsBaseHook.
 
     .. seealso::
         - :class:`airflow.providers.amazon.aws.hooks.base_aws.AwsBaseHook`
@@ -133,16 +134,17 @@
         """
         return self.conn.describe_tasks(cluster=cluster, tasks=[task])["tasks"][0]["lastStatus"]
 
 
 @runtime_checkable
 class EcsProtocol(Protocol):
     """
-    A structured Protocol for ``boto3.client('ecs')``. This is used for type hints on
-    :py:meth:`.EcsOperator.client`.
+    A structured Protocol for ``boto3.client('ecs')``.
+
+    This is used for type hints on :py:meth:`.EcsOperator.client`.
 
     .. seealso::
 
         - https://mypy.readthedocs.io/en/latest/protocols.html
         - https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ecs.html
     """
```

### Comparing `apache-airflow-providers-amazon-8.2.0rc1/airflow/providers/amazon/aws/hooks/eks.py` & `apache-airflow-providers-amazon-8.3.0rc1/airflow/providers/amazon/aws/hooks/eks.py`

 * *Files 0% similar despite different names*

```diff
@@ -74,14 +74,15 @@
     DEGRADED = "DEGRADED"
     NONEXISTENT = "NONEXISTENT"
 
 
 class EksHook(AwsBaseHook):
     """
     Interact with Amazon Elastic Kubernetes Service (EKS).
+
     Provide thin wrapper around :external+boto3:py:class:`boto3.client("eks") <EKS.Client>`.
 
     Additional arguments (such as ``aws_conn_id``) may be specified and
     are passed down to the underlying AwsBaseHook.
 
     .. seealso::
         - :class:`airflow.providers.amazon.aws.hooks.base_aws.AwsBaseHook`
```

### Comparing `apache-airflow-providers-amazon-8.2.0rc1/airflow/providers/amazon/aws/hooks/elasticache_replication_group.py` & `apache-airflow-providers-amazon-8.3.0rc1/airflow/providers/amazon/aws/hooks/elasticache_replication_group.py`

 * *Files 0% similar despite different names*

```diff
@@ -22,14 +22,15 @@
 from airflow.exceptions import AirflowException
 from airflow.providers.amazon.aws.hooks.base_aws import AwsBaseHook
 
 
 class ElastiCacheReplicationGroupHook(AwsBaseHook):
     """
     Interact with Amazon ElastiCache.
+
     Provide thick wrapper around :external+boto3:py:class:`boto3.client("elasticache") <ElastiCache.Client>`.
 
     :param max_retries: Max retries for checking availability of and deleting replication group
             If this is not supplied then this is defaulted to 10
     :param exponential_back_off_factor: Multiplication factor for deciding next sleep time
             If this is not supplied then this is defaulted to 1
     :param initial_poke_interval: Initial sleep time in seconds
```

### Comparing `apache-airflow-providers-amazon-8.2.0rc1/airflow/providers/amazon/aws/hooks/emr.py` & `apache-airflow-providers-amazon-8.3.0rc1/airflow/providers/amazon/aws/hooks/emr.py`

 * *Files 1% similar despite different names*

```diff
@@ -28,14 +28,15 @@
 from airflow.providers.amazon.aws.hooks.base_aws import AwsBaseHook
 from airflow.utils.helpers import prune_dict
 
 
 class EmrHook(AwsBaseHook):
     """
     Interact with Amazon Elastic MapReduce Service (EMR).
+
     Provide thick wrapper around :external+boto3:py:class:`boto3.client("emr") <EMR.Client>`.
 
     :param emr_conn_id: :ref:`Amazon Elastic MapReduce Connection <howto/connection:emr>`.
         This attribute is only necessary when using
         the :meth:`airflow.providers.amazon.aws.hooks.emr.EmrHook.create_job_flow`.
 
     Additional arguments (such as ``aws_conn_id``) may be specified and
@@ -53,16 +54,15 @@
     def __init__(self, emr_conn_id: str | None = default_conn_name, *args, **kwargs) -> None:
         self.emr_conn_id = emr_conn_id
         kwargs["client_type"] = "emr"
         super().__init__(*args, **kwargs)
 
     def get_cluster_id_by_name(self, emr_cluster_name: str, cluster_states: list[str]) -> str | None:
         """
-        Fetch id of EMR cluster with given name and (optional) states.
-        Will return only if single id is found.
+        Fetch id of EMR cluster with given name and (optional) states; returns only if single id is found.
 
         .. seealso::
             - :external+boto3:py:meth:`EMR.Client.list_clusters`
 
         :param emr_cluster_name: Name of a cluster to find
         :param cluster_states: State(s) of cluster to find
         :return: id of the EMR cluster
@@ -181,15 +181,14 @@
                 )
         return response["StepIds"]
 
     def test_connection(self):
         """
         Return failed state for test Amazon Elastic MapReduce Connection (untestable).
 
-
         We need to overwrite this method because this hook is based on
         :class:`~airflow.providers.amazon.aws.hooks.base_aws.AwsGenericHook`,
         otherwise it will try to test connection to AWS STS by using the default boto3 credential strategy.
         """
         msg = (
             f"{self.hook_name!r} Airflow Connection cannot be tested, by design it stores "
             f"only key/value pairs and does not make a connection to an external resource."
@@ -230,14 +229,15 @@
             },
         }
 
 
 class EmrServerlessHook(AwsBaseHook):
     """
     Interact with Amazon EMR Serverless.
+
     Provide thin wrapper around :py:class:`boto3.client("emr-serverless") <EMRServerless.Client>`.
 
     Additional arguments (such as ``aws_conn_id``) may be specified and
     are passed down to the underlying AwsBaseHook.
 
     .. seealso::
         - :class:`airflow.providers.amazon.aws.hooks.base_aws.AwsBaseHook`
@@ -254,16 +254,16 @@
 
     def __init__(self, *args: Any, **kwargs: Any) -> None:
         kwargs["client_type"] = "emr-serverless"
         super().__init__(*args, **kwargs)
 
     def cancel_running_jobs(self, application_id: str, waiter_config: dict = {}):
         """
-        List all jobs in an intermediate state and cancel them.
-        Then wait for those jobs to reach a terminal state.
+        List all jobs in an intermediate state, cancel them, then wait for those jobs to reach terminal state.
+
         Note: if new jobs are triggered while this operation is ongoing,
         it's going to time out and return an error.
         """
         paginator = self.conn.get_paginator("list_job_runs")
         results_per_response = 50
         iterator = paginator.paginate(
             applicationId=application_id,
@@ -292,14 +292,15 @@
                 WaiterConfig=waiter_config,
             )
 
 
 class EmrContainerHook(AwsBaseHook):
     """
     Interact with Amazon EMR Containers (Amazon EMR on EKS).
+
     Provide thick wrapper around :py:class:`boto3.client("emr-containers") <EMRContainers.Client>`.
 
     :param virtual_cluster_id: Cluster ID of the EMR on EKS virtual cluster
 
     Additional arguments (such as ``aws_conn_id``) may be specified and
     are passed down to the underlying AwsBaseHook.
 
@@ -363,14 +364,15 @@
         job_driver: dict,
         configuration_overrides: dict | None = None,
         client_request_token: str | None = None,
         tags: dict | None = None,
     ) -> str:
         """
         Submit a job to the EMR Containers API and return the job ID.
+
         A job run is a unit of work, such as a Spark jar, PySpark script,
         or SparkSQL query, that you submit to Amazon EMR on EKS.
 
         .. seealso::
             - :external+boto3:py:meth:`EMRContainers.Client.start_job_run`
 
         :param name: The name of the job run.
@@ -460,16 +462,15 @@
     def poll_query_status(
         self,
         job_id: str,
         poll_interval: int = 30,
         max_polling_attempts: int | None = None,
     ) -> str | None:
         """
-        Poll the status of submitted job run until query state reaches final state.
-        Returns one of the final states.
+        Poll the status of submitted job run until query state reaches final state; returns the final state.
 
         :param job_id: The ID of the job run request.
         :param poll_interval: Time (in seconds) to wait between calls to check query status on EMR
         :param max_polling_attempts: Number of times to poll for query state before function exits
         """
         try_number = 1
         final_query_state = None  # Query state when query reaches final state or max_polling_attempts reached
```

### Comparing `apache-airflow-providers-amazon-8.2.0rc1/airflow/providers/amazon/aws/hooks/glacier.py` & `apache-airflow-providers-amazon-8.3.0rc1/airflow/providers/amazon/aws/hooks/glacier.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-amazon-8.2.0rc1/airflow/providers/amazon/aws/hooks/glue.py` & `apache-airflow-providers-amazon-8.3.0rc1/airflow/providers/amazon/aws/hooks/glue.py`

 * *Files 2% similar despite different names*

```diff
@@ -29,14 +29,15 @@
 DEFAULT_LOG_SUFFIX = "output"
 ERROR_LOG_SUFFIX = "error"
 
 
 class GlueJobHook(AwsBaseHook):
     """
     Interact with AWS Glue.
+
     Provide thick wrapper around :external+boto3:py:class:`boto3.client("glue") <Glue.Client>`.
 
     :param s3_bucket: S3 bucket where logs and local etl script will be uploaded
     :param job_name: unique job name per AWS account
     :param desc: job description
     :param concurrent_run_limit: The maximum number of concurrent runs allowed for a job
     :param script_location: path to etl script on s3
@@ -50,16 +51,14 @@
     Additional arguments (such as ``aws_conn_id``) may be specified and
     are passed down to the underlying AwsBaseHook.
 
     .. seealso::
         - :class:`airflow.providers.amazon.aws.hooks.base_aws.AwsBaseHook`
     """
 
-    JOB_POLL_INTERVAL = 6  # polls job status after every JOB_POLL_INTERVAL seconds
-
     class LogContinuationTokens:
         """Used to hold the continuation tokens when reading logs from both streams Glue Jobs write to."""
 
         def __init__(self):
             self.output_stream_continuation: str | None = None
             self.error_stream_continuation: str | None = None
 
@@ -71,27 +70,29 @@
         concurrent_run_limit: int = 1,
         script_location: str | None = None,
         retry_limit: int = 0,
         num_of_dpus: int | float | None = None,
         iam_role_name: str | None = None,
         create_job_kwargs: dict | None = None,
         update_config: bool = False,
+        job_poll_interval: int | float = 6,
         *args,
         **kwargs,
     ):
         self.job_name = job_name
         self.desc = desc
         self.concurrent_run_limit = concurrent_run_limit
         self.script_location = script_location
         self.retry_limit = retry_limit
         self.s3_bucket = s3_bucket
         self.role_name = iam_role_name
         self.s3_glue_logs = "logs/glue-logs/"
         self.create_job_kwargs = create_job_kwargs or {}
         self.update_config = update_config
+        self.job_poll_interval = job_poll_interval
 
         worker_type_exists = "WorkerType" in self.create_job_kwargs
         num_workers_exists = "NumberOfWorkers" in self.create_job_kwargs
 
         if worker_type_exists and num_workers_exists:
             if num_of_dpus is not None:
                 raise ValueError("Cannot specify num_of_dpus with custom WorkerType")
@@ -178,16 +179,15 @@
             return self.conn.start_job_run(JobName=job_name, Arguments=script_arguments, **run_kwargs)
         except Exception as general_error:
             self.log.error("Failed to run aws glue job, error: %s", general_error)
             raise
 
     def get_job_state(self, job_name: str, run_id: str) -> str:
         """
-        Get state of the Glue job.
-        The job state can be running, finished, failed, stopped or timeout.
+        Get state of the Glue job; the job state can be running, finished, failed, stopped or timeout.
 
         .. seealso::
             - :external+boto3:py:meth:`Glue.Client.get_job_run`
 
         :param job_name: unique job name per AWS account
         :param run_id: The job-run ID of the predecessor job run
         :return: State of the Glue job
@@ -259,49 +259,47 @@
         )
         continuation_tokens.error_stream_continuation = display_logs_from(
             log_group_error, continuation_tokens.error_stream_continuation
         )
 
     def job_completion(self, job_name: str, run_id: str, verbose: bool = False) -> dict[str, str]:
         """
-        Waits until Glue job with job_name completes or fails and return final state if finished.
-        Raises AirflowException when the job failed.
+        Wait until Glue job with job_name finishes; return final state if finished or raises AirflowException.
 
         :param job_name: unique job name per AWS account
         :param run_id: The job-run ID of the predecessor job run
         :param verbose: If True, more Glue Job Run logs show in the Airflow Task Logs.  (default: False)
         :return: Dict of JobRunState and JobRunId
         """
         next_log_tokens = self.LogContinuationTokens()
         while True:
             job_run_state = self.get_job_state(job_name, run_id)
             ret = self._handle_state(job_run_state, job_name, run_id, verbose, next_log_tokens)
             if ret:
                 return ret
             else:
-                time.sleep(self.JOB_POLL_INTERVAL)
+                time.sleep(self.job_poll_interval)
 
     async def async_job_completion(self, job_name: str, run_id: str, verbose: bool = False) -> dict[str, str]:
         """
-        Waits until Glue job with job_name completes or fails and return final state if finished.
-        Raises AirflowException when the job failed.
+        Wait until Glue job with job_name finishes; return final state if finished or raises AirflowException.
 
         :param job_name: unique job name per AWS account
         :param run_id: The job-run ID of the predecessor job run
         :param verbose: If True, more Glue Job Run logs show in the Airflow Task Logs.  (default: False)
         :return: Dict of JobRunState and JobRunId
         """
         next_log_tokens = self.LogContinuationTokens()
         while True:
             job_run_state = await self.async_get_job_state(job_name, run_id)
             ret = self._handle_state(job_run_state, job_name, run_id, verbose, next_log_tokens)
             if ret:
                 return ret
             else:
-                await asyncio.sleep(self.JOB_POLL_INTERVAL)
+                await asyncio.sleep(self.job_poll_interval)
 
     def _handle_state(
         self,
         state: str,
         job_name: str,
         run_id: str,
         verbose: bool,
```

### Comparing `apache-airflow-providers-amazon-8.2.0rc1/airflow/providers/amazon/aws/hooks/glue_catalog.py` & `apache-airflow-providers-amazon-8.3.0rc1/airflow/providers/amazon/aws/hooks/glue_catalog.py`

 * *Files 1% similar despite different names*

```diff
@@ -23,14 +23,15 @@
 from airflow.exceptions import AirflowException
 from airflow.providers.amazon.aws.hooks.base_aws import AwsBaseHook
 
 
 class GlueCatalogHook(AwsBaseHook):
     """
     Interact with AWS Glue Data Catalog.
+
     Provide thin wrapper around :external+boto3:py:class:`boto3.client("glue") <Glue.Client>`.
 
     Additional arguments (such as ``aws_conn_id``) may be specified and
     are passed down to the underlying AwsBaseHook.
 
     .. seealso::
         - :class:`airflow.providers.amazon.aws.hooks.base_aws.AwsBaseHook`
```

### Comparing `apache-airflow-providers-amazon-8.2.0rc1/airflow/providers/amazon/aws/hooks/glue_crawler.py` & `apache-airflow-providers-amazon-8.3.0rc1/airflow/providers/amazon/aws/hooks/glue_crawler.py`

 * *Files 2% similar despite different names*

```diff
@@ -22,14 +22,15 @@
 from airflow.providers.amazon.aws.hooks.base_aws import AwsBaseHook
 from airflow.providers.amazon.aws.hooks.sts import StsHook
 
 
 class GlueCrawlerHook(AwsBaseHook):
     """
     Interacts with AWS Glue Crawler.
+
     Provide thin wrapper around :external+boto3:py:class:`boto3.client("glue") <Glue.Client>`.
 
     Additional arguments (such as ``aws_conn_id``) may be specified and
     are passed down to the underlying AwsBaseHook.
 
     .. seealso::
         - :class:`airflow.providers.amazon.aws.hooks.base_aws.AwsBaseHook`
@@ -165,17 +166,15 @@
         :return: Empty dictionary
         """
         self.log.info("Starting crawler %s", crawler_name)
         return self.glue_client.start_crawler(Name=crawler_name)
 
     def wait_for_crawler_completion(self, crawler_name: str, poll_interval: int = 5) -> str:
         """
-        Waits until Glue crawler completes and
-        returns the status of the latest crawl run.
-        Raises AirflowException if the crawler fails or is cancelled.
+        Wait until Glue crawler completes; returns the status of the latest crawl or raises AirflowException.
 
         :param crawler_name: unique crawler name per AWS account
         :param poll_interval: Time (in seconds) to wait between two consecutive calls to check crawler status
         :return: Crawler's status
         """
         self.get_waiter("crawler_ready").wait(Name=crawler_name, WaiterConfig={"Delay": poll_interval})
```

### Comparing `apache-airflow-providers-amazon-8.2.0rc1/airflow/providers/amazon/aws/hooks/kinesis.py` & `apache-airflow-providers-amazon-8.3.0rc1/airflow/providers/amazon/aws/hooks/kinesis.py`

 * *Files 0% similar despite different names*

```diff
@@ -22,14 +22,15 @@
 
 from airflow.providers.amazon.aws.hooks.base_aws import AwsBaseHook
 
 
 class FirehoseHook(AwsBaseHook):
     """
     Interact with Amazon Kinesis Firehose.
+
     Provide thick wrapper around :external+boto3:py:class:`boto3.client("firehose") <Firehose.Client>`.
 
     :param delivery_stream: Name of the delivery stream
 
     Additional arguments (such as ``aws_conn_id``) may be specified and
     are passed down to the underlying AwsBaseHook.
```

### Comparing `apache-airflow-providers-amazon-8.2.0rc1/airflow/providers/amazon/aws/hooks/lambda_function.py` & `apache-airflow-providers-amazon-8.3.0rc1/airflow/providers/amazon/aws/hooks/lambda_function.py`

 * *Files 2% similar despite different names*

```diff
@@ -23,14 +23,15 @@
 from airflow.providers.amazon.aws.hooks.base_aws import AwsBaseHook
 from airflow.providers.amazon.aws.utils import trim_none_values
 
 
 class LambdaHook(AwsBaseHook):
     """
     Interact with AWS Lambda.
+
     Provide thin wrapper around :external+boto3:py:class:`boto3.client("lambda") <Lambda.Client>`.
 
     Additional arguments (such as ``aws_conn_id``) may be specified and
     are passed down to the underlying AwsBaseHook.
 
     .. seealso::
         - :class:`airflow.providers.amazon.aws.hooks.base_aws.AwsBaseHook`
@@ -43,15 +44,15 @@
     def invoke_lambda(
         self,
         *,
         function_name: str,
         invocation_type: str | None = None,
         log_type: str | None = None,
         client_context: str | None = None,
-        payload: str | None = None,
+        payload: bytes | str | None = None,
         qualifier: str | None = None,
     ):
         """
         Invoke Lambda Function.
 
         .. seealso::
             - :external+boto3:py:meth:`Lambda.Client.invoke`
@@ -60,14 +61,17 @@
         :param invocation_type: AWS Lambda Invocation Type (RequestResponse, Event etc)
         :param log_type: Tail Invocation Request
         :param client_context: Up to 3,583 bytes of base64-encoded data about the invoking client
             to pass to the function in the context object.
         :param payload: The JSON that you want to provide to your Lambda function as input.
         :param qualifier: AWS Lambda Function Version or Alias Name
         """
+        if isinstance(payload, str):
+            payload = payload.encode()
+
         invoke_args = {
             "FunctionName": function_name,
             "InvocationType": invocation_type,
             "LogType": log_type,
             "ClientContext": client_context,
             "Payload": payload,
             "Qualifier": qualifier,
```

### Comparing `apache-airflow-providers-amazon-8.2.0rc1/airflow/providers/amazon/aws/hooks/logs.py` & `apache-airflow-providers-amazon-8.3.0rc1/airflow/providers/amazon/aws/hooks/logs.py`

 * *Files 7% similar despite different names*

```diff
@@ -11,36 +11,35 @@
 #
 # Unless required by applicable law or agreed to in writing,
 # software distributed under the License is distributed on an
 # "AS IS" BASIS, WITHOUT WARRANTIES OR CONDITIONS OF ANY
 # KIND, either express or implied.  See the License for the
 # specific language governing permissions and limitations
 # under the License.
-"""
-This module contains a hook (AwsLogsHook) with some very basic
-functionality for interacting with AWS CloudWatch.
-"""
 from __future__ import annotations
 
+import warnings
 from typing import Generator
 
+from airflow.exceptions import AirflowProviderDeprecationWarning
 from airflow.providers.amazon.aws.hooks.base_aws import AwsBaseHook
 
 # Guidance received from the AWS team regarding the correct way to check for the end of a stream is that the
 # value of the nextForwardToken is the same in subsequent calls.
 # The issue with this approach is, it can take a huge amount of time (e.g. 20 seconds) to retrieve logs using
 # this approach. As an intermediate solution, we decided to stop fetching logs if 3 consecutive responses
 # are empty.
 # See PR https://github.com/apache/airflow/pull/20814
 NUM_CONSECUTIVE_EMPTY_RESPONSE_EXIT_THRESHOLD = 3
 
 
 class AwsLogsHook(AwsBaseHook):
     """
     Interact with Amazon CloudWatch Logs.
+
     Provide thin wrapper around :external+boto3:py:class:`boto3.client("logs") <CloudWatchLogs.Client>`.
 
     Additional arguments (such as ``aws_conn_id``) may be specified and
     are passed down to the underlying AwsBaseHook.
 
     .. seealso::
         - :class:`airflow.providers.amazon.aws.hooks.base_aws.AwsBaseHook`
@@ -58,38 +57,52 @@
 
     def get_log_events(
         self,
         log_group: str,
         log_stream_name: str,
         start_time: int = 0,
         skip: int = 0,
-        start_from_head: bool = True,
+        start_from_head: bool | None = None,
         continuation_token: ContinuationToken | None = None,
     ) -> Generator:
         """
-        A generator for log items in a single stream. This will yield all the
-        items that are available at the current moment.
+        A generator for log items in a single stream; yields all items available at the current moment.
 
         .. seealso::
             - :external+boto3:py:meth:`CloudWatchLogs.Client.get_log_events`
 
         :param log_group: The name of the log group.
         :param log_stream_name: The name of the specific stream.
         :param start_time: The time stamp value to start reading the logs from (default: 0).
         :param skip: The number of log entries to skip at the start (default: 0).
             This is for when there are multiple entries at the same timestamp.
-        :param start_from_head: whether to start from the beginning (True) of the log or
-            at the end of the log (False).
+        :param start_from_head: Deprecated. Do not use with False, logs would be retrieved out of order.
+            If possible, retrieve logs in one query, or implement pagination yourself.
         :param continuation_token: a token indicating where to read logs from.
             Will be updated as this method reads new logs, to be reused in subsequent calls.
         :return: | A CloudWatch log event with the following key-value pairs:
                  |   'timestamp' (int): The time in milliseconds of the event.
                  |   'message' (str): The log event data.
                  |   'ingestionTime' (int): The time in milliseconds the event was ingested.
         """
+        if start_from_head is not None:
+            message = (
+                "start_from_head is deprecated, please remove this parameter."
+                if start_from_head
+                else "Do not use this method with start_from_head=False, logs will be returned out of order. "
+                "If possible, retrieve logs in one query, or implement pagination yourself."
+            )
+            warnings.warn(
+                message,
+                AirflowProviderDeprecationWarning,
+                stacklevel=2,
+            )
+        else:
+            start_from_head = True
+
         if continuation_token is None:
             continuation_token = AwsLogsHook.ContinuationToken()
 
         num_consecutive_empty_response = 0
         while True:
             if continuation_token.value is not None:
                 token_arg: dict[str, str] = {"nextToken": continuation_token.value}
```

### Comparing `apache-airflow-providers-amazon-8.2.0rc1/airflow/providers/amazon/aws/hooks/quicksight.py` & `apache-airflow-providers-amazon-8.3.0rc1/airflow/providers/amazon/aws/hooks/quicksight.py`

 * *Files 0% similar despite different names*

```diff
@@ -26,14 +26,15 @@
 from airflow.providers.amazon.aws.hooks.base_aws import AwsBaseHook
 from airflow.providers.amazon.aws.hooks.sts import StsHook
 
 
 class QuickSightHook(AwsBaseHook):
     """
     Interact with Amazon QuickSight.
+
     Provide thin wrapper around :external+boto3:py:class:`boto3.client("quicksight") <QuickSight.Client>`.
 
     Additional arguments (such as ``aws_conn_id``) may be specified and
     are passed down to the underlying AwsBaseHook.
 
     .. seealso::
         - :class:`airflow.providers.amazon.aws.hooks.base_aws.AwsBaseHook`
```

### Comparing `apache-airflow-providers-amazon-8.2.0rc1/airflow/providers/amazon/aws/hooks/rds.py` & `apache-airflow-providers-amazon-8.3.0rc1/airflow/providers/amazon/aws/hooks/rds.py`

 * *Files 3% similar despite different names*

```diff
@@ -19,22 +19,24 @@
 from __future__ import annotations
 
 import time
 from typing import TYPE_CHECKING, Callable
 
 from airflow.exceptions import AirflowException, AirflowNotFoundException
 from airflow.providers.amazon.aws.hooks.base_aws import AwsGenericHook
+from airflow.providers.amazon.aws.utils.waiter_with_logging import wait
 
 if TYPE_CHECKING:
     from mypy_boto3_rds import RDSClient  # noqa
 
 
 class RdsHook(AwsGenericHook["RDSClient"]):
     """
     Interact with Amazon Relational Database Service (RDS).
+
     Provide thin wrapper around :external+boto3:py:class:`boto3.client("rds") <RDS.Client>`.
 
     Additional arguments (such as ``aws_conn_id``) may be specified and
     are passed down to the underlying AwsBaseHook.
 
     .. seealso::
         - :class:`airflow.providers.amazon.aws.hooks.base_aws.AwsBaseHook`
@@ -65,16 +67,15 @@
             raise e
         return response["DBSnapshots"][0]["Status"].lower()
 
     def wait_for_db_snapshot_state(
         self, snapshot_id: str, target_state: str, check_interval: int = 30, max_attempts: int = 40
     ) -> None:
         """
-        Polls DB Snapshots until the target state is reached.
-        An error is raised after a max number of attempts.
+        Poll DB Snapshots until target_state is reached; raise AirflowException after max_attempts.
 
         .. seealso::
             - :external+boto3:py:meth:`RDS.Client.describe_db_snapshots`
 
         :param snapshot_id: The ID of the target DB instance snapshot
         :param target_state: Wait until this state is reached
         :param check_interval: The amount of time in seconds to wait between attempts
@@ -114,16 +115,15 @@
             raise e
         return response["DBClusterSnapshots"][0]["Status"].lower()
 
     def wait_for_db_cluster_snapshot_state(
         self, snapshot_id: str, target_state: str, check_interval: int = 30, max_attempts: int = 40
     ) -> None:
         """
-        Polls DB Cluster Snapshots until the target state is reached.
-        An error is raised after a max number of attempts.
+        Poll DB Cluster Snapshots until target_state is reached; raise AirflowException after a max_attempts.
 
         .. seealso::
             - :external+boto3:py:meth:`RDS.Client.describe_db_cluster_snapshots`
 
         :param snapshot_id: The ID of the target DB cluster snapshot
         :param target_state: Wait until this state is reached
         :param check_interval: The amount of time in seconds to wait between attempts
@@ -163,16 +163,15 @@
             raise e
         return response["ExportTasks"][0]["Status"].lower()
 
     def wait_for_export_task_state(
         self, export_task_id: str, target_state: str, check_interval: int = 30, max_attempts: int = 40
     ) -> None:
         """
-        Polls export tasks until the target state is reached.
-        An error is raised after a max number of attempts.
+        Poll export tasks until target_state is reached; raise AirflowException after max_attempts.
 
         .. seealso::
             - :external+boto3:py:meth:`RDS.Client.describe_export_tasks`
 
         :param export_task_id: The identifier of the target snapshot export task.
         :param target_state: Wait until this state is reached
         :param check_interval: The amount of time in seconds to wait between attempts
@@ -205,16 +204,15 @@
             raise e
         return response["EventSubscriptionsList"][0]["Status"].lower()
 
     def wait_for_event_subscription_state(
         self, subscription_name: str, target_state: str, check_interval: int = 30, max_attempts: int = 40
     ) -> None:
         """
-        Polls Even Subscriptions until the target state is reached.
-        An error is raised after a max number of attempts.
+        Poll Event Subscriptions until target_state is reached; raise AirflowException after max_attempts.
 
         .. seealso::
             - :external+boto3:py:meth:`RDS.Client.describe_event_subscriptions`
 
         :param subscription_name: The name of the target RDS event notification subscription.
         :param target_state: Wait until this state is reached
         :param check_interval: The amount of time in seconds to wait between attempts
@@ -247,16 +245,15 @@
             raise e
         return response["DBInstances"][0]["DBInstanceStatus"].lower()
 
     def wait_for_db_instance_state(
         self, db_instance_id: str, target_state: str, check_interval: int = 30, max_attempts: int = 40
     ) -> None:
         """
-        Polls DB Instances until the target state is reached.
-        An error is raised after a max number of attempts.
+        Poll DB Instances until target_state is reached; raise AirflowException after max_attempts.
 
         .. seealso::
             - :external+boto3:py:meth:`RDS.Client.describe_db_instances`
 
         :param db_instance_id: The ID of the target DB instance.
         :param target_state: Wait until this state is reached
         :param check_interval: The amount of time in seconds to wait between attempts
@@ -265,17 +262,22 @@
 
         def poke():
             return self.get_db_instance_state(db_instance_id)
 
         target_state = target_state.lower()
         if target_state in ("available", "deleted"):
             waiter = self.conn.get_waiter(f"db_instance_{target_state}")  # type: ignore
-            waiter.wait(
-                DBInstanceIdentifier=db_instance_id,
-                WaiterConfig={"Delay": check_interval, "MaxAttempts": max_attempts},
+            wait(
+                waiter=waiter,
+                waiter_delay=check_interval,
+                waiter_max_attempts=max_attempts,
+                args={"DBInstanceIdentifier": db_instance_id},
+                failure_message=f"Rdb DB instance failed to reach state {target_state}",
+                status_message="Rds DB instance state is",
+                status_args=["DBInstances[0].DBInstanceStatus"],
             )
         else:
             self._wait_for_state(poke, target_state, check_interval, max_attempts)
             self.log.info("DB cluster snapshot '%s' reached the '%s' state", db_instance_id, target_state)
 
     def get_db_cluster_state(self, db_cluster_id: str) -> str:
         """
@@ -296,16 +298,15 @@
             raise e
         return response["DBClusters"][0]["Status"].lower()
 
     def wait_for_db_cluster_state(
         self, db_cluster_id: str, target_state: str, check_interval: int = 30, max_attempts: int = 40
     ) -> None:
         """
-        Polls DB Clusters until the target state is reached.
-        An error is raised after a max number of attempts.
+        Poll DB Clusters until target_state is reached; raise AirflowException after max_attempts.
 
         .. seealso::
             - :external+boto3:py:meth:`RDS.Client.describe_db_clusters`
 
         :param db_cluster_id: The ID of the target DB cluster.
         :param target_state: Wait until this state is reached
         :param check_interval: The amount of time in seconds to wait between attempts
```

### Comparing `apache-airflow-providers-amazon-8.2.0rc1/airflow/providers/amazon/aws/hooks/redshift_cluster.py` & `apache-airflow-providers-amazon-8.3.0rc1/airflow/providers/amazon/aws/hooks/redshift_cluster.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-amazon-8.2.0rc1/airflow/providers/amazon/aws/hooks/redshift_data.py` & `apache-airflow-providers-amazon-8.3.0rc1/airflow/providers/amazon/aws/hooks/redshift_data.py`

 * *Files 0% similar despite different names*

```diff
@@ -27,14 +27,15 @@
 if TYPE_CHECKING:
     from mypy_boto3_redshift_data import RedshiftDataAPIServiceClient  # noqa
 
 
 class RedshiftDataHook(AwsGenericHook["RedshiftDataAPIServiceClient"]):
     """
     Interact with Amazon Redshift Data API.
+
     Provide thin wrapper around
     :external+boto3:py:class:`boto3.client("redshift-data") <RedshiftDataAPIService.Client>`.
 
     Additional arguments (such as ``aws_conn_id``) may be specified and
     are passed down to the underlying AwsBaseHook.
 
     .. seealso::
```

### Comparing `apache-airflow-providers-amazon-8.2.0rc1/airflow/providers/amazon/aws/hooks/redshift_sql.py` & `apache-airflow-providers-amazon-8.3.0rc1/airflow/providers/amazon/aws/hooks/redshift_sql.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-amazon-8.2.0rc1/airflow/providers/amazon/aws/hooks/s3.py` & `apache-airflow-providers-amazon-8.3.0rc1/airflow/providers/amazon/aws/hooks/s3.py`

 * *Files 12% similar despite different names*

```diff
@@ -19,14 +19,15 @@
 from __future__ import annotations
 
 import asyncio
 import fnmatch
 import gzip as gz
 import io
 import logging
+import os
 import re
 import shutil
 import warnings
 from contextlib import suppress
 from copy import deepcopy
 from datetime import datetime
 from functools import wraps
@@ -60,18 +61,15 @@
 
 T = TypeVar("T", bound=Callable)
 
 logger = logging.getLogger(__name__)
 
 
 def provide_bucket_name(func: T) -> T:
-    """
-    Function decorator that provides a bucket name taken from the connection
-    in case no bucket name has been passed to the function.
-    """
+    """Provide a bucket name taken from the connection if no bucket name has been passed to the function."""
     if hasattr(func, "_unify_bucket_name_and_key_wrapped"):
         logger.warning("`unify_bucket_name_and_key` should wrap `provide_bucket_name`.")
     function_signature = signature(func)
 
     @wraps(func)
     def wrapper(*args, **kwargs) -> T:
         bound_args = function_signature.bind(*args, **kwargs)
@@ -79,32 +77,29 @@
         if "bucket_name" not in bound_args.arguments:
             self = args[0]
 
             if "bucket_name" in self.service_config:
                 bound_args.arguments["bucket_name"] = self.service_config["bucket_name"]
             elif self.conn_config and self.conn_config.schema:
                 warnings.warn(
-                    "s3 conn_type, and the associated schema field, is deprecated."
-                    " Please use aws conn_type instead, and specify `bucket_name`"
-                    " in `service_config.s3` within `extras`.",
+                    "s3 conn_type, and the associated schema field, is deprecated. "
+                    "Please use aws conn_type instead, and specify `bucket_name` "
+                    "in `service_config.s3` within `extras`.",
                     AirflowProviderDeprecationWarning,
                     stacklevel=2,
                 )
                 bound_args.arguments["bucket_name"] = self.conn_config.schema
 
         return func(*bound_args.args, **bound_args.kwargs)
 
     return cast(T, wrapper)
 
 
 def provide_bucket_name_async(func: T) -> T:
-    """
-    Function decorator that provides a bucket name taken from the connection
-    in case no bucket name has been passed to the function.
-    """
+    """Provide a bucket name taken from the connection if no bucket name has been passed to the function."""
     function_signature = signature(func)
 
     @wraps(func)
     async def wrapper(*args: Any, **kwargs: Any) -> Any:
         bound_args = function_signature.bind(*args, **kwargs)
 
         if "bucket_name" not in bound_args.arguments:
@@ -116,18 +111,15 @@
 
         return await func(*bound_args.args, **bound_args.kwargs)
 
     return cast(T, wrapper)
 
 
 def unify_bucket_name_and_key(func: T) -> T:
-    """
-    Function decorator that unifies bucket name and key taken from the key
-    in case no bucket name and at least a key has been passed to the function.
-    """
+    """Unify bucket name and key in case no bucket name and at least a key has been passed to the function."""
     function_signature = signature(func)
 
     @wraps(func)
     def wrapper(*args, **kwargs) -> T:
         bound_args = function_signature.bind(*args, **kwargs)
 
         if "wildcard_key" in bound_args.arguments:
@@ -152,14 +144,15 @@
     wrapper._unify_bucket_name_and_key_wrapped = True  # type: ignore[attr-defined]
     return cast(T, wrapper)
 
 
 class S3Hook(AwsBaseHook):
     """
     Interact with Amazon Simple Storage Service (S3).
+
     Provide thick wrapper around :external+boto3:py:class:`boto3.client("s3") <S3.Client>`
     and :external+boto3:py:class:`boto3.resource("s3") <S3.ServiceResource>`.
 
     :param transfer_config_args: Configuration object for managed S3 transfers.
     :param extra_args: Extra arguments that may be passed to the download/upload operations.
 
     .. seealso::
@@ -208,33 +201,46 @@
 
         See https://docs.aws.amazon.com/AmazonS3/latest/userguide/access-bucket-intro.html
         for valid url formats.
 
         :param s3url: The S3 Url to parse.
         :return: the parsed bucket name and key
         """
+        valid_s3_format = "S3://bucket-name/key-name"
+        valid_s3_virtual_hosted_format = "https://bucket-name.s3.region-code.amazonaws.com/key-name"
         format = s3url.split("//")
         if re.match(r"s3[na]?:", format[0], re.IGNORECASE):
             parsed_url = urlsplit(s3url)
             if not parsed_url.netloc:
-                raise S3HookUriParseFailure(f'Please provide a bucket name using a valid format: "{s3url}"')
+                raise S3HookUriParseFailure(
+                    "Please provide a bucket name using a valid format of the form: "
+                    f'{valid_s3_format} or {valid_s3_virtual_hosted_format} but provided: "{s3url}"'
+                )
 
             bucket_name = parsed_url.netloc
             key = parsed_url.path.lstrip("/")
         elif format[0] == "https:":
             temp_split = format[1].split(".")
             if temp_split[0] == "s3":
                 split_url = format[1].split("/")
                 bucket_name = split_url[1]
                 key = "/".join(split_url[2:])
             elif temp_split[1] == "s3":
                 bucket_name = temp_split[0]
                 key = "/".join(format[1].split("/")[1:])
+            else:
+                raise S3HookUriParseFailure(
+                    "Please provide a bucket name using a valid virtually hosted format which should "
+                    f'be of the form: {valid_s3_virtual_hosted_format} but provided: "{s3url}"'
+                )
         else:
-            raise S3HookUriParseFailure(f'Please provide a bucket name using a valid format: "{s3url}"')
+            raise S3HookUriParseFailure(
+                "Please provide a bucket name using a valid format of the form: "
+                f'{valid_s3_format} or {valid_s3_virtual_hosted_format} but provided: "{s3url}"'
+            )
         return bucket_name, key
 
     @staticmethod
     def get_s3_bucket_key(
         bucket: str | None, key: str, bucket_param_name: str, key_param_name: str
     ) -> tuple[str, str]:
         """
@@ -478,16 +484,18 @@
         self,
         client: AioBaseClient,
         bucket_val: str,
         wildcard_match: bool,
         key: str,
     ) -> bool:
         """
-        Function to check if wildcard_match is True get list of files that a key matching a wildcard
-        expression exists in a bucket asynchronously and return the boolean value. If  wildcard_match
+        Get a list of files that a key matching a wildcard expression or get the head object.
+
+        If wildcard_match is True get list of files that a key matching a wildcard
+        expression exists in a bucket asynchronously and return the boolean value. If wildcard_match
         is False get the head object from the bucket and return the boolean value.
 
         :param client: aiobotocore client
         :param bucket_val: the name of the bucket
         :param key: S3 keys that will point to the file
         :param wildcard_match: the path to the key
         """
@@ -621,14 +629,125 @@
                 return False
             if to_datetime is not None and input_date > to_datetime:
                 return False
             return True
 
         return [k["Key"] for k in keys if _is_in_period(k["LastModified"])]
 
+    async def is_keys_unchanged_async(
+        self,
+        client: AioBaseClient,
+        bucket_name: str,
+        prefix: str,
+        inactivity_period: float = 60 * 60,
+        min_objects: int = 1,
+        previous_objects: set[str] | None = None,
+        inactivity_seconds: int = 0,
+        allow_delete: bool = True,
+        last_activity_time: datetime | None = None,
+    ) -> dict[str, Any]:
+        """
+        Checks whether new objects have been uploaded and the inactivity_period
+        has passed and updates the state of the sensor accordingly.
+
+        :param client: aiobotocore client
+        :param bucket_name: the name of the bucket
+        :param prefix: a key prefix
+        :param inactivity_period:  the total seconds of inactivity to designate
+            keys unchanged. Note, this mechanism is not real time and
+            this operator may not return until a poke_interval after this period
+            has passed with no additional objects sensed.
+        :param min_objects: the minimum number of objects needed for keys unchanged
+            sensor to be considered valid.
+        :param previous_objects: the set of object ids found during the last poke.
+        :param inactivity_seconds: number of inactive seconds
+        :param allow_delete: Should this sensor consider objects being deleted
+            between pokes valid behavior. If true a warning message will be logged
+            when this happens. If false an error will be raised.
+        :param last_activity_time: last activity datetime.
+        """
+        if not previous_objects:
+            previous_objects = set()
+        list_keys = await self._list_keys_async(client=client, bucket_name=bucket_name, prefix=prefix)
+        current_objects = set(list_keys)
+        current_num_objects = len(current_objects)
+        if current_num_objects > len(previous_objects):
+            # When new objects arrived, reset the inactivity_seconds
+            # and update previous_objects for the next poke.
+            self.log.info(
+                "New objects found at %s, resetting last_activity_time.",
+                os.path.join(bucket_name, prefix),
+            )
+            self.log.debug("New objects: %s", current_objects - previous_objects)
+            last_activity_time = datetime.now()
+            inactivity_seconds = 0
+            previous_objects = current_objects
+            return {
+                "status": "pending",
+                "previous_objects": previous_objects,
+                "last_activity_time": last_activity_time,
+                "inactivity_seconds": inactivity_seconds,
+            }
+
+        if len(previous_objects) - len(current_objects):
+            # During the last poke interval objects were deleted.
+            if allow_delete:
+                deleted_objects = previous_objects - current_objects
+                previous_objects = current_objects
+                last_activity_time = datetime.now()
+                self.log.info(
+                    "Objects were deleted during the last poke interval. Updating the "
+                    "file counter and resetting last_activity_time:\n%s",
+                    deleted_objects,
+                )
+                return {
+                    "status": "pending",
+                    "previous_objects": previous_objects,
+                    "last_activity_time": last_activity_time,
+                    "inactivity_seconds": inactivity_seconds,
+                }
+
+            return {
+                "status": "error",
+                "message": f"{os.path.join(bucket_name, prefix)} between pokes.",
+            }
+
+        if last_activity_time:
+            inactivity_seconds = int((datetime.now() - last_activity_time).total_seconds())
+        else:
+            # Handles the first poke where last inactivity time is None.
+            last_activity_time = datetime.now()
+            inactivity_seconds = 0
+
+        if inactivity_seconds >= inactivity_period:
+            path = os.path.join(bucket_name, prefix)
+
+            if current_num_objects >= min_objects:
+                success_message = (
+                    f"SUCCESS: Sensor found {current_num_objects} objects at {path}. "
+                    "Waited at least {inactivity_period} seconds, with no new objects uploaded."
+                )
+                self.log.info(success_message)
+                return {
+                    "status": "success",
+                    "message": success_message,
+                }
+
+            self.log.error("FAILURE: Inactivity Period passed, not enough objects found in %s", path)
+            return {
+                "status": "error",
+                "message": f"FAILURE: Inactivity Period passed, not enough objects found in {path}",
+            }
+        return {
+            "status": "pending",
+            "previous_objects": previous_objects,
+            "last_activity_time": last_activity_time,
+            "inactivity_seconds": inactivity_seconds,
+        }
+
     @provide_bucket_name
     def list_keys(
         self,
         bucket_name: str | None = None,
         prefix: str | None = None,
         delimiter: str | None = None,
         page_size: int | None = None,
@@ -1342,16 +1461,15 @@
         self,
         tag_set: dict[str, str] | list[dict[str, str]] | None = None,
         key: str | None = None,
         value: str | None = None,
         bucket_name: str | None = None,
     ) -> None:
         """
-        Overwrites the existing TagSet with provided tags.
-        Must provide a TagSet, a key/value pair, or both.
+        Overwrites the existing TagSet with provided tags; must provide a TagSet, a key/value pair, or both.
 
         .. seealso::
             - :external+boto3:py:meth:`S3.Client.put_bucket_tagging`
 
         :param tag_set: A dictionary containing the key/value pairs for the tags,
             or a list already formatted for the API
         :param key: The Key for the new TagSet entry.
```

### Comparing `apache-airflow-providers-amazon-8.2.0rc1/airflow/providers/amazon/aws/hooks/sagemaker.py` & `apache-airflow-providers-amazon-8.3.0rc1/airflow/providers/amazon/aws/hooks/sagemaker.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-amazon-8.2.0rc1/airflow/providers/amazon/aws/hooks/secrets_manager.py` & `apache-airflow-providers-amazon-8.3.0rc1/airflow/providers/amazon/aws/hooks/secrets_manager.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-amazon-8.2.0rc1/airflow/providers/amazon/aws/hooks/ses.py` & `apache-airflow-providers-amazon-8.3.0rc1/airflow/providers/amazon/aws/hooks/ses.py`

 * *Files 0% similar despite different names*

```diff
@@ -22,14 +22,15 @@
 from airflow.providers.amazon.aws.hooks.base_aws import AwsBaseHook
 from airflow.utils.email import build_mime_message
 
 
 class SesHook(AwsBaseHook):
     """
     Interact with Amazon Simple Email Service.
+
     Provide thin wrapper around :external+boto3:py:class:`boto3.client("ses") <SES.Client>`.
 
     Additional arguments (such as ``aws_conn_id``) may be specified and
     are passed down to the underlying AwsBaseHook.
 
     .. seealso::
         - :class:`airflow.providers.amazon.aws.hooks.base_aws.AwsBaseHook`
```

### Comparing `apache-airflow-providers-amazon-8.2.0rc1/airflow/providers/amazon/aws/hooks/sns.py` & `apache-airflow-providers-amazon-8.3.0rc1/airflow/providers/amazon/aws/hooks/sns.py`

 * *Files 0% similar despite different names*

```diff
@@ -36,14 +36,15 @@
         f"Values in MessageAttributes must be one of bytes, str, int, float, or iterable; got {type(o)}"
     )
 
 
 class SnsHook(AwsBaseHook):
     """
     Interact with Amazon Simple Notification Service.
+
     Provide thin wrapper around :external+boto3:py:class:`boto3.client("sns") <SNS.Client>`.
 
     Additional arguments (such as ``aws_conn_id``) may be specified and
     are passed down to the underlying AwsBaseHook.
 
     .. seealso::
         - :class:`airflow.providers.amazon.aws.hooks.base_aws.AwsBaseHook`
```

### Comparing `apache-airflow-providers-amazon-8.2.0rc1/airflow/providers/amazon/aws/hooks/sqs.py` & `apache-airflow-providers-amazon-8.3.0rc1/airflow/providers/amazon/aws/hooks/sqs.py`

 * *Files 4% similar despite different names*

```diff
@@ -20,14 +20,15 @@
 
 from airflow.providers.amazon.aws.hooks.base_aws import AwsBaseHook
 
 
 class SqsHook(AwsBaseHook):
     """
     Interact with Amazon Simple Queue Service.
+
     Provide thin wrapper around :external+boto3:py:class:`boto3.client("sqs") <SQS.Client>`.
 
     Additional arguments (such as ``aws_conn_id``) may be specified and
     are passed down to the underlying AwsBaseHook.
 
     .. seealso::
         - :class:`airflow.providers.amazon.aws.hooks.base_aws.AwsBaseHook`
```

### Comparing `apache-airflow-providers-amazon-8.2.0rc1/airflow/providers/amazon/aws/hooks/ssm.py` & `apache-airflow-providers-amazon-8.3.0rc1/airflow/providers/amazon/aws/hooks/ssm.py`

 * *Files 7% similar despite different names*

```diff
@@ -21,14 +21,15 @@
 from airflow.utils.log.secrets_masker import mask_secret
 from airflow.utils.types import NOTSET, ArgNotSet
 
 
 class SsmHook(AwsBaseHook):
     """
     Interact with Amazon Systems Manager (SSM).
+
     Provide thin wrapper around :external+boto3:py:class:`boto3.client("ssm") <SSM.Client>`.
 
     Additional arguments (such as ``aws_conn_id``) may be specified and
     are passed down to the underlying AwsBaseHook.
 
     .. seealso::
         - :class:`airflow.providers.amazon.aws.hooks.base_aws.AwsBaseHook`
@@ -36,16 +37,15 @@
 
     def __init__(self, *args, **kwargs) -> None:
         kwargs["client_type"] = "ssm"
         super().__init__(*args, **kwargs)
 
     def get_parameter_value(self, parameter: str, default: str | ArgNotSet = NOTSET) -> str:
         """
-        Returns the value of the provided Parameter or an optional default.
-        If value exists, and it is encrypted, then decrypt and mask them for loggers.
+        Return the provided Parameter or an optional default; if it is encrypted, then decrypt and mask.
 
         .. seealso::
             - :external+boto3:py:meth:`SSM.Client.get_parameter`
 
         :param parameter: The SSM Parameter name to return the value for.
         :param default: Optional default value to return if none is found.
         """
```

### Comparing `apache-airflow-providers-amazon-8.2.0rc1/airflow/providers/amazon/aws/hooks/step_function.py` & `apache-airflow-providers-amazon-8.3.0rc1/airflow/providers/amazon/aws/hooks/step_function.py`

 * *Files 0% similar despite different names*

```diff
@@ -20,14 +20,15 @@
 
 from airflow.providers.amazon.aws.hooks.base_aws import AwsBaseHook
 
 
 class StepFunctionHook(AwsBaseHook):
     """
     Interact with an AWS Step Functions State Machine.
+
     Provide thin wrapper around :external+boto3:py:class:`boto3.client("stepfunctions") <SFN.Client>`.
 
     Additional arguments (such as ``aws_conn_id``) may be specified and
     are passed down to the underlying AwsBaseHook.
 
     .. seealso::
         - :class:`airflow.providers.amazon.aws.hooks.base_aws.AwsBaseHook`
```

### Comparing `apache-airflow-providers-amazon-8.2.0rc1/airflow/providers/amazon/aws/hooks/sts.py` & `apache-airflow-providers-amazon-8.3.0rc1/airflow/providers/amazon/aws/hooks/sts.py`

 * *Files 0% similar despite different names*

```diff
@@ -18,14 +18,15 @@
 
 from airflow.providers.amazon.aws.hooks.base_aws import AwsBaseHook
 
 
 class StsHook(AwsBaseHook):
     """
     Interact with AWS Security Token Service (STS).
+
     Provide thin wrapper around :external+boto3:py:class:`boto3.client("sts") <STS.Client>`.
 
     Additional arguments (such as ``aws_conn_id``) may be specified and
     are passed down to the underlying AwsBaseHook.
 
     .. seealso::
         - :class:`airflow.providers.amazon.aws.hooks.base_aws.AwsBaseHook`
```

### Comparing `apache-airflow-providers-amazon-8.2.0rc1/airflow/providers/amazon/aws/links/__init__.py` & `apache-airflow-providers-amazon-8.3.0rc1/airflow/providers/amazon/aws/links/__init__.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-amazon-8.2.0rc1/airflow/providers/amazon/aws/links/base_aws.py` & `apache-airflow-providers-amazon-8.3.0rc1/airflow/providers/amazon/aws/links/base_aws.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-amazon-8.2.0rc1/airflow/providers/amazon/aws/links/batch.py` & `apache-airflow-providers-amazon-8.3.0rc1/airflow/providers/amazon/aws/links/batch.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-amazon-8.2.0rc1/airflow/providers/amazon/aws/links/emr.py` & `apache-airflow-providers-amazon-8.3.0rc1/airflow/providers/amazon/aws/links/emr.py`

 * *Files 4% similar despite different names*

```diff
@@ -47,16 +47,17 @@
         return super().format_link(**kwargs)
 
 
 def get_log_uri(
     *, cluster: dict[str, Any] | None = None, emr_client: boto3.client = None, job_flow_id: str | None = None
 ) -> str | None:
     """
-    Retrieves the S3 URI to the EMR Job logs.  Requires either the output of a
-    describe_cluster call or both an EMR Client and a job_flow_id to look it up.
+    Retrieves the S3 URI to the EMR Job logs.
+
+    Requires either the output of a describe_cluster call or both an EMR Client and a job_flow_id..
     """
     if not exactly_one(bool(cluster), emr_client and job_flow_id):
         raise AirflowException(
             "Requires either the output of a describe_cluster call or both an EMR Client and a job_flow_id."
         )
 
     cluster_info = (cluster or emr_client.describe_cluster(ClusterId=job_flow_id))["Cluster"]
```

### Comparing `apache-airflow-providers-amazon-8.2.0rc1/airflow/providers/amazon/aws/links/glue.py` & `apache-airflow-providers-amazon-8.3.0rc1/airflow/providers/amazon/aws/links/glue.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-amazon-8.2.0rc1/airflow/providers/amazon/aws/links/logs.py` & `apache-airflow-providers-amazon-8.3.0rc1/airflow/providers/amazon/aws/links/logs.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-amazon-8.2.0rc1/airflow/providers/amazon/aws/log/__init__.py` & `apache-airflow-providers-amazon-8.3.0rc1/airflow/providers/amazon/aws/log/__init__.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-amazon-8.2.0rc1/airflow/providers/amazon/aws/log/cloudwatch_task_handler.py` & `apache-airflow-providers-amazon-8.3.0rc1/airflow/providers/amazon/aws/log/cloudwatch_task_handler.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-amazon-8.2.0rc1/airflow/providers/amazon/aws/log/s3_task_handler.py` & `apache-airflow-providers-amazon-8.3.0rc1/airflow/providers/amazon/aws/log/s3_task_handler.py`

 * *Files 2% similar despite different names*

```diff
@@ -40,17 +40,17 @@
     if Version(version) < Version("2.6"):
         return False
     return conf.getboolean("logging", "delete_local_logs")
 
 
 class S3TaskHandler(FileTaskHandler, LoggingMixin):
     """
-    S3TaskHandler is a python log handler that handles and reads
-    task instance logs. It extends airflow FileTaskHandler and
-    uploads to and reads from S3 remote storage.
+    S3TaskHandler is a python log handler that handles and reads task instance logs.
+
+    It extends airflow FileTaskHandler and uploads to and reads from S3 remote storage.
     """
 
     trigger_should_wrap = True
 
     def __init__(
         self, base_log_folder: str, s3_log_folder: str, filename_template: str | None = None, **kwargs
     ):
@@ -129,14 +129,15 @@
         else:
             messages.append(f"No logs found on s3 for ti={ti}")
         return messages, logs
 
     def _read(self, ti, try_number, metadata=None):
         """
         Read logs of given task instance and try_number from S3 remote storage.
+
         If failed, read the log from task instance host machine.
 
         todo: when min airflow version >= 2.6 then remove this method (``_read``)
 
         :param ti: task instance object
         :param try_number: task instance try_number to read logs from
         :param metadata: log metadata,
@@ -164,16 +165,15 @@
         :param remote_log_location: log's location in remote storage
         :return: True if location exists else False
         """
         return self.hook.check_for_key(remote_log_location)
 
     def s3_read(self, remote_log_location: str, return_error: bool = False) -> str:
         """
-        Returns the log found at the remote_log_location. Returns '' if no
-        logs are found or there is an error.
+        Returns the log found at the remote_log_location. Return '' if no logs are found or there is an error.
 
         :param remote_log_location: the log's location in remote storage
         :param return_error: if True, returns a string error message if an
             error occurs. Otherwise returns '' when an error occurs.
         :return: the log found at the remote_log_location
         """
         try:
@@ -184,16 +184,15 @@
             # return error if needed
             if return_error:
                 return msg
         return ""
 
     def s3_write(self, log: str, remote_log_location: str, append: bool = True, max_retry: int = 1) -> bool:
         """
-        Writes the log to the remote_log_location and return `True` when done. Fails silently
-         and return `False` if no log was created.
+        Write the log to the remote_log_location; return `True` or fails silently and return `False`.
 
         :param log: the log to write to the remote_log_location
         :param remote_log_location: the log's location in remote storage
         :param append: if False, any existing log file is overwritten. If True,
             the new log is appended to any existing logs.
         :param max_retry: Maximum number of times to retry on upload failure
         :return: whether the log is successfully written to remote location or not.
```

### Comparing `apache-airflow-providers-amazon-8.2.0rc1/airflow/providers/amazon/aws/operators/__init__.py` & `apache-airflow-providers-amazon-8.3.0rc1/airflow/providers/amazon/aws/notifications/__init__.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-amazon-8.2.0rc1/airflow/providers/amazon/aws/operators/appflow.py` & `apache-airflow-providers-amazon-8.3.0rc1/airflow/providers/amazon/aws/operators/appflow.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-amazon-8.2.0rc1/airflow/providers/amazon/aws/operators/athena.py` & `apache-airflow-providers-amazon-8.3.0rc1/airflow/providers/amazon/aws/operators/athena.py`

 * *Files 14% similar despite different names*

```diff
@@ -16,25 +16,31 @@
 # specific language governing permissions and limitations
 # under the License.
 from __future__ import annotations
 
 from functools import cached_property
 from typing import TYPE_CHECKING, Any, Sequence
 
+from airflow import AirflowException
+from airflow.configuration import conf
 from airflow.models import BaseOperator
 from airflow.providers.amazon.aws.hooks.athena import AthenaHook
+from airflow.providers.amazon.aws.triggers.athena import AthenaTrigger
 
 if TYPE_CHECKING:
     from airflow.utils.context import Context
 
 
 class AthenaOperator(BaseOperator):
     """
     An operator that submits a presto query to athena.
 
+    .. note:: if the task is killed while it runs, it'll cancel the athena query that was launched,
+        EXCEPT if running in deferrable mode.
+
     .. seealso::
         For more information on how to use this operator, take a look at the guide:
         :ref:`howto/operator:AthenaOperator`
 
     :param query: Presto to be run on athena. (templated)
     :param database: Database to select. (templated)
     :param output_location: s3 path to write the query results into. (templated)
@@ -65,49 +71,61 @@
         client_request_token: str | None = None,
         workgroup: str = "primary",
         query_execution_context: dict[str, str] | None = None,
         result_configuration: dict[str, Any] | None = None,
         sleep_time: int = 30,
         max_polling_attempts: int | None = None,
         log_query: bool = True,
+        deferrable: bool = conf.getboolean("operators", "default_deferrable", fallback=False),
         **kwargs: Any,
     ) -> None:
         super().__init__(**kwargs)
         self.query = query
         self.database = database
         self.output_location = output_location
         self.aws_conn_id = aws_conn_id
         self.client_request_token = client_request_token
         self.workgroup = workgroup
         self.query_execution_context = query_execution_context or {}
         self.result_configuration = result_configuration or {}
         self.sleep_time = sleep_time
-        self.max_polling_attempts = max_polling_attempts
+        self.max_polling_attempts = max_polling_attempts or 999999
         self.query_execution_id: str | None = None
         self.log_query: bool = log_query
+        self.deferrable = deferrable
 
     @cached_property
     def hook(self) -> AthenaHook:
         """Create and return an AthenaHook."""
-        return AthenaHook(self.aws_conn_id, sleep_time=self.sleep_time, log_query=self.log_query)
+        return AthenaHook(self.aws_conn_id, log_query=self.log_query)
 
     def execute(self, context: Context) -> str | None:
         """Run Presto Query on Athena."""
         self.query_execution_context["Database"] = self.database
         self.result_configuration["OutputLocation"] = self.output_location
         self.query_execution_id = self.hook.run_query(
             self.query,
             self.query_execution_context,
             self.result_configuration,
             self.client_request_token,
             self.workgroup,
         )
+
+        if self.deferrable:
+            self.defer(
+                trigger=AthenaTrigger(
+                    self.query_execution_id, self.sleep_time, self.max_polling_attempts, self.aws_conn_id
+                ),
+                method_name="execute_complete",
+            )
+        # implicit else:
         query_status = self.hook.poll_query_status(
             self.query_execution_id,
             max_polling_attempts=self.max_polling_attempts,
+            sleep_time=self.sleep_time,
         )
 
         if query_status in AthenaHook.FAILURE_STATES:
             error_message = self.hook.get_state_change_reason(self.query_execution_id)
             raise Exception(
                 f"Final state of Athena job is {query_status}, query_execution_id is "
                 f"{self.query_execution_id}. Error: {error_message}"
@@ -116,14 +134,19 @@
             raise Exception(
                 f"Final state of Athena job is {query_status}. Max tries of poll status exceeded, "
                 f"query_execution_id is {self.query_execution_id}."
             )
 
         return self.query_execution_id
 
+    def execute_complete(self, context, event=None):
+        if event["status"] != "success":
+            raise AirflowException(f"Error while waiting for operation on cluster to complete: {event}")
+        return event["value"]
+
     def on_kill(self) -> None:
         """Cancel the submitted athena query."""
         if self.query_execution_id:
             self.log.info("Received a kill signal.")
             response = self.hook.stop_query(self.query_execution_id)
             http_status_code = None
             try:
@@ -135,8 +158,8 @@
             finally:
                 if http_status_code is None or http_status_code != 200:
                     self.log.error("Unable to request query cancel on athena. Exiting")
                 else:
                     self.log.info(
                         "Polling Athena for query with id %s to reach final state", self.query_execution_id
                     )
-                    self.hook.poll_query_status(self.query_execution_id)
+                    self.hook.poll_query_status(self.query_execution_id, sleep_time=self.sleep_time)
```

### Comparing `apache-airflow-providers-amazon-8.2.0rc1/airflow/providers/amazon/aws/operators/batch.py` & `apache-airflow-providers-amazon-8.3.0rc1/airflow/providers/amazon/aws/operators/batch.py`

 * *Files 4% similar despite different names*

```diff
@@ -25,24 +25,28 @@
 from __future__ import annotations
 
 import warnings
 from datetime import timedelta
 from functools import cached_property
 from typing import TYPE_CHECKING, Any, Sequence
 
+from airflow.configuration import conf
 from airflow.exceptions import AirflowException, AirflowProviderDeprecationWarning
 from airflow.models import BaseOperator
 from airflow.providers.amazon.aws.hooks.batch_client import BatchClientHook
 from airflow.providers.amazon.aws.links.batch import (
     BatchJobDefinitionLink,
     BatchJobDetailsLink,
     BatchJobQueueLink,
 )
 from airflow.providers.amazon.aws.links.logs import CloudWatchEventsLink
-from airflow.providers.amazon.aws.triggers.batch import BatchOperatorTrigger
+from airflow.providers.amazon.aws.triggers.batch import (
+    BatchCreateComputeEnvironmentTrigger,
+    BatchOperatorTrigger,
+)
 from airflow.providers.amazon.aws.utils import trim_none_values
 from airflow.providers.amazon.aws.utils.task_log_fetcher import AwsTaskLogFetcher
 
 if TYPE_CHECKING:
     from airflow.utils.context import Context
 
 
@@ -147,15 +151,15 @@
         waiters: Any | None = None,
         max_retries: int | None = None,
         status_retries: int | None = None,
         aws_conn_id: str | None = None,
         region_name: str | None = None,
         tags: dict | None = None,
         wait_for_completion: bool = True,
-        deferrable: bool = False,
+        deferrable: bool = conf.getboolean("operators", "default_deferrable", fallback=False),
         poll_interval: int = 30,
         awslogs_enabled: bool = False,
         awslogs_fetch_interval: timedelta = timedelta(seconds=30),
         **kwargs,
     ) -> None:
         BaseOperator.__init__(self, **kwargs)
         self.job_id = job_id
@@ -398,22 +402,24 @@
     :param unmanaged_v_cpus: Maximum number of vCPU for an unmanaged compute
         environment. This parameter is only supported when the ``type``
         parameter is set to ``UNMANAGED``.
     :param service_role: IAM role that allows Batch to make calls to other AWS
         services on your behalf (templated).
     :param tags: Tags that you apply to the compute-environment to help you
         categorize and organize your resources.
-    :param max_retries: Exponential back-off retries, 4200 = 48 hours; polling
-        is only used when waiters is None.
-    :param status_retries: Number of HTTP retries to get job status, 10; polling
-        is only used when waiters is None.
+    :param poll_interval: How long to wait in seconds between 2 polls at the environment status.
+        Only useful when deferrable is True.
+    :param max_retries: How many times to poll for the environment status.
+        Only useful when deferrable is True.
     :param aws_conn_id: Connection ID of AWS credentials / region name. If None,
         credential boto3 strategy will be used.
     :param region_name: Region name to use in AWS Hook. Overrides the
         ``region_name`` in connection if provided.
+    :param deferrable: If True, the operator will wait asynchronously for the environment to be created.
+        This mode requires aiobotocore module to be installed. (default: False)
     """
 
     template_fields: Sequence[str] = (
         "compute_environment_name",
         "compute_resources",
         "service_role",
     )
@@ -424,39 +430,49 @@
         compute_environment_name: str,
         environment_type: str,
         state: str,
         compute_resources: dict,
         unmanaged_v_cpus: int | None = None,
         service_role: str | None = None,
         tags: dict | None = None,
+        poll_interval: int = 30,
         max_retries: int | None = None,
-        status_retries: int | None = None,
         aws_conn_id: str | None = None,
         region_name: str | None = None,
+        deferrable: bool = conf.getboolean("operators", "default_deferrable", fallback=False),
         **kwargs,
     ):
+        if "status_retries" in kwargs:
+            warnings.warn(
+                "The `status_retries` parameter is unused and should be removed. "
+                "It'll be deleted in a future version.",
+                AirflowProviderDeprecationWarning,
+                stacklevel=2,
+            )
+            kwargs.pop("status_retries")  # remove before calling super() to prevent unexpected arg error
+
         super().__init__(**kwargs)
+
         self.compute_environment_name = compute_environment_name
         self.environment_type = environment_type
         self.state = state
         self.unmanaged_v_cpus = unmanaged_v_cpus
         self.compute_resources = compute_resources
         self.service_role = service_role
         self.tags = tags or {}
-        self.max_retries = max_retries
-        self.status_retries = status_retries
+        self.poll_interval = poll_interval
+        self.max_retries = max_retries or 120
         self.aws_conn_id = aws_conn_id
         self.region_name = region_name
+        self.deferrable = deferrable
 
     @cached_property
     def hook(self):
         """Create and return a BatchClientHook."""
         return BatchClientHook(
-            max_retries=self.max_retries,
-            status_retries=self.status_retries,
             aws_conn_id=self.aws_conn_id,
             region_name=self.region_name,
         )
 
     def execute(self, context: Context):
         """Create an AWS batch compute environment."""
         kwargs: dict[str, Any] = {
@@ -464,10 +480,25 @@
             "type": self.environment_type,
             "state": self.state,
             "unmanagedvCpus": self.unmanaged_v_cpus,
             "computeResources": self.compute_resources,
             "serviceRole": self.service_role,
             "tags": self.tags,
         }
-        self.hook.client.create_compute_environment(**trim_none_values(kwargs))
+        response = self.hook.client.create_compute_environment(**trim_none_values(kwargs))
+        arn = response["computeEnvironmentArn"]
+
+        if self.deferrable:
+            self.defer(
+                trigger=BatchCreateComputeEnvironmentTrigger(
+                    arn, self.poll_interval, self.max_retries, self.aws_conn_id, self.region_name
+                ),
+                method_name="execute_complete",
+            )
 
         self.log.info("AWS Batch compute environment created successfully")
+        return arn
+
+    def execute_complete(self, context, event=None):
+        if event["status"] != "success":
+            raise AirflowException(f"Error while waiting for the compute environment to be ready: {event}")
+        return event["value"]
```

### Comparing `apache-airflow-providers-amazon-8.2.0rc1/airflow/providers/amazon/aws/operators/cloud_formation.py` & `apache-airflow-providers-amazon-8.3.0rc1/airflow/providers/amazon/aws/operators/cloud_formation.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-amazon-8.2.0rc1/airflow/providers/amazon/aws/operators/datasync.py` & `apache-airflow-providers-amazon-8.3.0rc1/airflow/providers/amazon/aws/operators/datasync.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-amazon-8.2.0rc1/airflow/providers/amazon/aws/operators/dms.py` & `apache-airflow-providers-amazon-8.3.0rc1/airflow/providers/amazon/aws/operators/dms.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-amazon-8.2.0rc1/airflow/providers/amazon/aws/operators/ec2.py` & `apache-airflow-providers-amazon-8.3.0rc1/airflow/providers/amazon/aws/operators/ec2.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-amazon-8.2.0rc1/airflow/providers/amazon/aws/operators/ecs.py` & `apache-airflow-providers-amazon-8.3.0rc1/airflow/providers/amazon/aws/operators/ecs.py`

 * *Files 10% similar despite different names*

```diff
@@ -22,23 +22,22 @@
 import warnings
 from datetime import timedelta
 from functools import cached_property
 from typing import TYPE_CHECKING, Sequence
 
 import boto3
 
+from airflow.configuration import conf
 from airflow.exceptions import AirflowException, AirflowProviderDeprecationWarning
 from airflow.models import BaseOperator, XCom
 from airflow.providers.amazon.aws.exceptions import EcsOperatorError, EcsTaskFailToStart
 from airflow.providers.amazon.aws.hooks.base_aws import AwsBaseHook
-from airflow.providers.amazon.aws.hooks.ecs import (
-    EcsClusterStates,
-    EcsHook,
-    should_retry_eni,
-)
+from airflow.providers.amazon.aws.hooks.ecs import EcsClusterStates, EcsHook, should_retry_eni
+from airflow.providers.amazon.aws.hooks.logs import AwsLogsHook
+from airflow.providers.amazon.aws.triggers.ecs import ClusterWaiterTrigger, TaskDoneTrigger
 from airflow.providers.amazon.aws.utils.task_log_fetcher import AwsTaskLogFetcher
 from airflow.utils.helpers import prune_dict
 from airflow.utils.session import provide_session
 
 if TYPE_CHECKING:
     from airflow.utils.context import Context
 
@@ -63,14 +62,23 @@
         """Create and return the EcsHook's client."""
         return self.hook.conn
 
     def execute(self, context: Context):
         """Must overwrite in child classes."""
         raise NotImplementedError("Please implement execute() in subclass")
 
+    def _complete_exec_with_cluster_desc(self, context, event=None):
+        """To be used as trigger callback for operators that return the cluster description."""
+        if event["status"] != "success":
+            raise AirflowException(f"Error while waiting for operation on cluster to complete: {event}")
+        cluster_arn = event.get("arn")
+        # We cannot get the cluster definition from the waiter on success, so we have to query it here.
+        details = self.hook.conn.describe_clusters(clusters=[cluster_arn])["clusters"][0]
+        return details
+
 
 class EcsCreateClusterOperator(EcsBaseOperator):
     """
     Creates an AWS ECS cluster.
 
     .. seealso::
         For more information on how to use this operator, take a look at the guide:
@@ -80,34 +88,44 @@
         cluster, you create a cluster that's named default.
     :param create_cluster_kwargs: Extra arguments for Cluster Creation.
     :param wait_for_completion: If True, waits for creation of the cluster to complete. (default: True)
     :param waiter_delay: The amount of time in seconds to wait between attempts,
         if not set then the default waiter value will be used.
     :param waiter_max_attempts: The maximum number of attempts to be made,
         if not set then the default waiter value will be used.
+    :param deferrable: If True, the operator will wait asynchronously for the job to complete.
+        This implies waiting for completion. This mode requires aiobotocore module to be installed.
+        (default: False)
     """
 
-    template_fields: Sequence[str] = ("cluster_name", "create_cluster_kwargs", "wait_for_completion")
+    template_fields: Sequence[str] = (
+        "cluster_name",
+        "create_cluster_kwargs",
+        "wait_for_completion",
+        "deferrable",
+    )
 
     def __init__(
         self,
         *,
         cluster_name: str,
         create_cluster_kwargs: dict | None = None,
         wait_for_completion: bool = True,
-        waiter_delay: int | None = None,
-        waiter_max_attempts: int | None = None,
+        waiter_delay: int = 15,
+        waiter_max_attempts: int = 60,
+        deferrable: bool = conf.getboolean("operators", "default_deferrable", fallback=False),
         **kwargs,
     ) -> None:
         super().__init__(**kwargs)
         self.cluster_name = cluster_name
         self.create_cluster_kwargs = create_cluster_kwargs or {}
         self.wait_for_completion = wait_for_completion
         self.waiter_delay = waiter_delay
         self.waiter_max_attempts = waiter_max_attempts
+        self.deferrable = deferrable
 
     def execute(self, context: Context):
         self.log.info(
             "Creating cluster %r using the following values: %s",
             self.cluster_name,
             self.create_cluster_kwargs,
         )
@@ -115,14 +133,29 @@
         cluster_details = result["cluster"]
         cluster_state = cluster_details.get("status")
 
         if cluster_state == EcsClusterStates.ACTIVE:
             # In some circumstances the ECS Cluster is created immediately,
             # and there is no reason to wait for completion.
             self.log.info("Cluster %r in state: %r.", self.cluster_name, cluster_state)
+        elif self.deferrable:
+            self.defer(
+                trigger=ClusterWaiterTrigger(
+                    waiter_name="cluster_active",
+                    cluster_arn=cluster_details["clusterArn"],
+                    waiter_delay=self.waiter_delay,
+                    waiter_max_attempts=self.waiter_max_attempts,
+                    aws_conn_id=self.aws_conn_id,
+                    region=self.region,
+                ),
+                method_name="_complete_exec_with_cluster_desc",
+                # timeout is set to ensure that if a trigger dies, the timeout does not restart
+                # 60 seconds is added to allow the trigger to exit gracefully (i.e. yield TriggerEvent)
+                timeout=timedelta(seconds=self.waiter_max_attempts * self.waiter_delay + 60),
+            )
         elif self.wait_for_completion:
             waiter = self.hook.get_waiter("cluster_active")
             waiter.wait(
                 clusters=[cluster_details["clusterArn"]],
                 WaiterConfig=prune_dict(
                     {
                         "Delay": self.waiter_delay,
@@ -144,43 +177,63 @@
 
     :param cluster_name: The short name or full Amazon Resource Name (ARN) of the cluster to delete.
     :param wait_for_completion: If True, waits for creation of the cluster to complete. (default: True)
     :param waiter_delay: The amount of time in seconds to wait between attempts,
         if not set then the default waiter value will be used.
     :param waiter_max_attempts: The maximum number of attempts to be made,
         if not set then the default waiter value will be used.
+    :param deferrable: If True, the operator will wait asynchronously for the job to complete.
+        This implies waiting for completion. This mode requires aiobotocore module to be installed.
+        (default: False)
     """
 
-    template_fields: Sequence[str] = ("cluster_name", "wait_for_completion")
+    template_fields: Sequence[str] = ("cluster_name", "wait_for_completion", "deferrable")
 
     def __init__(
         self,
         *,
         cluster_name: str,
         wait_for_completion: bool = True,
-        waiter_delay: int | None = None,
-        waiter_max_attempts: int | None = None,
+        waiter_delay: int = 15,
+        waiter_max_attempts: int = 60,
+        deferrable: bool = conf.getboolean("operators", "default_deferrable", fallback=False),
         **kwargs,
     ) -> None:
         super().__init__(**kwargs)
         self.cluster_name = cluster_name
         self.wait_for_completion = wait_for_completion
         self.waiter_delay = waiter_delay
         self.waiter_max_attempts = waiter_max_attempts
+        self.deferrable = deferrable
 
     def execute(self, context: Context):
         self.log.info("Deleting cluster %r.", self.cluster_name)
         result = self.client.delete_cluster(cluster=self.cluster_name)
         cluster_details = result["cluster"]
         cluster_state = cluster_details.get("status")
 
         if cluster_state == EcsClusterStates.INACTIVE:
-            # In some circumstances the ECS Cluster is deleted immediately,
-            # so there is no reason to wait for completion.
+            # if the cluster doesn't have capacity providers that are associated with it,
+            # the deletion is instantaneous, and we don't need to wait for it.
             self.log.info("Cluster %r in state: %r.", self.cluster_name, cluster_state)
+        elif self.deferrable:
+            self.defer(
+                trigger=ClusterWaiterTrigger(
+                    waiter_name="cluster_inactive",
+                    cluster_arn=cluster_details["clusterArn"],
+                    waiter_delay=self.waiter_delay,
+                    waiter_max_attempts=self.waiter_max_attempts,
+                    aws_conn_id=self.aws_conn_id,
+                    region=self.region,
+                ),
+                method_name="_complete_exec_with_cluster_desc",
+                # timeout is set to ensure that if a trigger dies, the timeout does not restart
+                # 60 seconds is added to allow the trigger to exit gracefully (i.e. yield TriggerEvent)
+                timeout=timedelta(seconds=self.waiter_max_attempts * self.waiter_delay + 60),
+            )
         elif self.wait_for_completion:
             waiter = self.hook.get_waiter("cluster_inactive")
             waiter.wait(
                 clusters=[cluster_details["clusterArn"]],
                 WaiterConfig=prune_dict(
                     {
                         "Delay": self.waiter_delay,
@@ -343,28 +396,32 @@
         this is the default AWS region based on your connection settings.
     :param awslogs_stream_prefix: the stream prefix that is used for the CloudWatch logs.
         This is usually based on some custom name combined with the name of the container.
         Only required if you want logs to be shown in the Airflow UI after your job has
         finished.
     :param awslogs_fetch_interval: the interval that the ECS task log fetcher should wait
         in between each Cloudwatch logs fetches.
+        If deferrable is set to True, that parameter is ignored and waiter_delay is used instead.
     :param quota_retry: Config if and how to retry the launch of a new ECS task, to handle
         transient errors.
     :param reattach: If set to True, will check if the task previously launched by the task_instance
         is already running. If so, the operator will attach to it instead of starting a new task.
         This is to avoid relaunching a new task when the connection drops between Airflow and ECS while
         the task is running (when the Airflow worker is restarted for example).
     :param number_logs_exception: Number of lines from the last Cloudwatch logs to return in the
         AirflowException if an ECS task is stopped (to receive Airflow alerts with the logs of what
         failed in the code running in ECS).
     :param wait_for_completion: If True, waits for creation of the cluster to complete. (default: True)
     :param waiter_delay: The amount of time in seconds to wait between attempts,
         if not set then the default waiter value will be used.
     :param waiter_max_attempts: The maximum number of attempts to be made,
         if not set then the default waiter value will be used.
+    :param deferrable: If True, the operator will wait asynchronously for the job to complete.
+        This implies waiting for completion. This mode requires aiobotocore module to be installed.
+        (default: False)
     """
 
     ui_color = "#f0ede4"
     template_fields: Sequence[str] = (
         "task_definition",
         "cluster",
         "overrides",
@@ -380,14 +437,15 @@
         "awslogs_region",
         "awslogs_stream_prefix",
         "awslogs_fetch_interval",
         "propagate_tags",
         "reattach",
         "number_logs_exception",
         "wait_for_completion",
+        "deferrable",
     )
     template_fields_renderers = {
         "overrides": "json",
         "network_configuration": "json",
         "tags": "json",
     }
     REATTACH_XCOM_KEY = "ecs_task_arn"
@@ -412,16 +470,17 @@
         awslogs_stream_prefix: str | None = None,
         awslogs_fetch_interval: timedelta = timedelta(seconds=30),
         propagate_tags: str | None = None,
         quota_retry: dict | None = None,
         reattach: bool = False,
         number_logs_exception: int = 10,
         wait_for_completion: bool = True,
-        waiter_delay: int | None = None,
-        waiter_max_attempts: int | None = None,
+        waiter_delay: int = 6,
+        waiter_max_attempts: int = 100,
+        deferrable: bool = conf.getboolean("operators", "default_deferrable", fallback=False),
         **kwargs,
     ):
         super().__init__(**kwargs)
 
         self.task_definition = task_definition
         self.cluster = cluster
         self.overrides = overrides
@@ -447,14 +506,15 @@
 
         self.arn: str | None = None
         self.retry_args = quota_retry
         self.task_log_fetcher: AwsTaskLogFetcher | None = None
         self.wait_for_completion = wait_for_completion
         self.waiter_delay = waiter_delay
         self.waiter_max_attempts = waiter_max_attempts
+        self.deferrable = deferrable
 
         if self._aws_logs_enabled() and not self.wait_for_completion:
             self.log.warning(
                 "Trying to get logs without waiting for the task to complete is undefined behavior."
             )
 
     @staticmethod
@@ -469,33 +529,37 @@
             "Running ECS Task - Task definition: %s - on cluster %s", self.task_definition, self.cluster
         )
         self.log.info("EcsOperator overrides: %s", self.overrides)
 
         if self.reattach:
             self._try_reattach_task(context)
 
-        self._start_wait_check_task(context)
-
-        self.log.info("ECS Task has been successfully executed")
-
-        if self.reattach:
-            # Clear the XCom value storing the ECS task ARN if the task has completed
-            # as we can't reattach it anymore
-            self._xcom_del(session, self.REATTACH_XCOM_TASK_ID_TEMPLATE.format(task_id=self.task_id))
-
-        if self.do_xcom_push and self.task_log_fetcher:
-            return self.task_log_fetcher.get_last_log_message()
-
-        return None
-
-    @AwsBaseHook.retry(should_retry_eni)
-    def _start_wait_check_task(self, context):
         if not self.arn:
+            # start the task except if we reattached to an existing one just before.
             self._start_task(context)
 
+        if self.deferrable:
+            self.defer(
+                trigger=TaskDoneTrigger(
+                    cluster=self.cluster,
+                    task_arn=self.arn,
+                    waiter_delay=self.waiter_delay,
+                    waiter_max_attempts=self.waiter_max_attempts,
+                    aws_conn_id=self.aws_conn_id,
+                    region=self.region,
+                    log_group=self.awslogs_group,
+                    log_stream=self._get_logs_stream_name(),
+                ),
+                method_name="execute_complete",
+                # timeout is set to ensure that if a trigger dies, the timeout does not restart
+                # 60 seconds is added to allow the trigger to exit gracefully (i.e. yield TriggerEvent)
+                timeout=timedelta(seconds=self.waiter_max_attempts * self.waiter_delay + 60),
+            )
+            # self.defer raises a special exception, so execution stops here in this case.
+
         if not self.wait_for_completion:
             return
 
         if self._aws_logs_enabled():
             self.log.info("Starting ECS Task Log Fetcher")
             self.task_log_fetcher = self._get_task_log_fetcher()
             self.task_log_fetcher.start()
@@ -504,19 +568,53 @@
                 self._wait_for_task_ended()
             finally:
                 self.task_log_fetcher.stop()
             self.task_log_fetcher.join()
         else:
             self._wait_for_task_ended()
 
+        self._after_execution(session)
+
+        if self.do_xcom_push and self.task_log_fetcher:
+            return self.task_log_fetcher.get_last_log_message()
+        else:
+            return None
+
+    def execute_complete(self, context, event=None):
+        if event["status"] != "success":
+            raise AirflowException(f"Error in task execution: {event}")
+        self.arn = event["task_arn"]  # restore arn to its updated value, needed for next steps
+        self._after_execution()
+        if self._aws_logs_enabled():
+            # same behavior as non-deferrable mode, return last line of logs of the task.
+            logs_client = AwsLogsHook(aws_conn_id=self.aws_conn_id, region_name=self.region).conn
+            one_log = logs_client.get_log_events(
+                logGroupName=self.awslogs_group,
+                logStreamName=self._get_logs_stream_name(),
+                startFromHead=False,
+                limit=1,
+            )
+            if len(one_log["events"]) > 0:
+                return one_log["events"][0]["message"]
+
+    @provide_session
+    def _after_execution(self, session=None):
         self._check_success_task()
 
+        self.log.info("ECS Task has been successfully executed")
+
+        if self.reattach:
+            # Clear the XCom value storing the ECS task ARN if the task has completed
+            # as we can't reattach it anymore
+            self._xcom_del(session, self.REATTACH_XCOM_TASK_ID_TEMPLATE.format(task_id=self.task_id))
+
     def _xcom_del(self, session, task_id):
         session.query(XCom).filter(XCom.dag_id == self.dag_id, XCom.task_id == task_id).delete()
 
+    @AwsBaseHook.retry(should_retry_eni)
     def _start_task(self, context):
         run_opts = {
             "cluster": self.cluster,
             "taskDefinition": self.task_definition,
             "overrides": self.overrides,
             "startedBy": self.owner,
         }
@@ -580,53 +678,53 @@
             return
 
         waiter = self.client.get_waiter("tasks_stopped")
         waiter.config.max_attempts = sys.maxsize  # timeout is managed by airflow
         waiter.wait(
             cluster=self.cluster,
             tasks=[self.arn],
-            WaiterConfig=prune_dict(
-                {
-                    "Delay": self.waiter_delay,
-                    "MaxAttempts": self.waiter_max_attempts,
-                }
-            ),
+            WaiterConfig={
+                "Delay": self.waiter_delay,
+                "MaxAttempts": self.waiter_max_attempts,
+            },
         )
 
         return
 
     def _aws_logs_enabled(self):
         return self.awslogs_group and self.awslogs_stream_prefix
 
+    def _get_logs_stream_name(self) -> str:
+        return f"{self.awslogs_stream_prefix}/{self._get_ecs_task_id(self.arn)}"
+
     def _get_task_log_fetcher(self) -> AwsTaskLogFetcher:
         if not self.awslogs_group:
             raise ValueError("must specify awslogs_group to fetch task logs")
-        log_stream_name = f"{self.awslogs_stream_prefix}/{self._get_ecs_task_id(self.arn)}"
 
         return AwsTaskLogFetcher(
             aws_conn_id=self.aws_conn_id,
             region_name=self.awslogs_region,
             log_group=self.awslogs_group,
-            log_stream_name=log_stream_name,
+            log_stream_name=self._get_logs_stream_name(),
             fetch_interval=self.awslogs_fetch_interval,
             logger=self.log,
         )
 
+    @AwsBaseHook.retry(should_retry_eni)
     def _check_success_task(self) -> None:
         if not self.client or not self.arn:
             return
 
         response = self.client.describe_tasks(cluster=self.cluster, tasks=[self.arn])
         self.log.info("ECS Task stopped, check status: %s", response)
 
         if len(response.get("failures", [])) > 0:
             raise AirflowException(response)
 
         for task in response["tasks"]:
-
             if task.get("stopCode", "") == "TaskFailedToStart":
                 # Reset task arn here otherwise the retry run will not start
                 # a new task but keep polling the old dead one
                 # I'm not resetting it for other exceptions here because
                 # EcsTaskFailToStart is the only exception that's being retried at the moment
                 self.arn = None
                 raise EcsTaskFailToStart(f"The task failed to start due to: {task.get('stoppedReason', '')}")
```

### Comparing `apache-airflow-providers-amazon-8.2.0rc1/airflow/providers/amazon/aws/operators/eks.py` & `apache-airflow-providers-amazon-8.3.0rc1/airflow/providers/amazon/aws/operators/eks.py`

 * *Files 21% similar despite different names*

```diff
@@ -13,28 +13,33 @@
 # "AS IS" BASIS, WITHOUT WARRANTIES OR CONDITIONS OF ANY
 # KIND, either express or implied.  See the License for the
 # specific language governing permissions and limitations
 # under the License.
 """This module contains Amazon EKS operators."""
 from __future__ import annotations
 
+import logging
 import warnings
 from ast import literal_eval
 from datetime import timedelta
-from typing import TYPE_CHECKING, Any, List, Sequence, cast
+from typing import TYPE_CHECKING, List, Sequence, cast
 
 from botocore.exceptions import ClientError, WaiterError
 
+from airflow.configuration import conf
 from airflow.exceptions import AirflowException, AirflowProviderDeprecationWarning
 from airflow.models import BaseOperator
 from airflow.providers.amazon.aws.hooks.eks import EksHook
 from airflow.providers.amazon.aws.triggers.eks import (
     EksCreateFargateProfileTrigger,
     EksDeleteFargateProfileTrigger,
+    EksNodegroupTrigger,
 )
+from airflow.providers.amazon.aws.utils.waiter_with_logging import wait
+from airflow.providers.cncf.kubernetes.utils.pod_manager import OnFinishAction
 
 try:
     from airflow.providers.cncf.kubernetes.operators.pod import KubernetesPodOperator
 except ImportError:
     # preserve backward compatibility for older versions of cncf.kubernetes provider
     from airflow.providers.cncf.kubernetes.operators.kubernetes_pod import KubernetesPodOperator
 
@@ -55,14 +60,81 @@
 SUCCESS_MSG = "No {compute} remain, deleting cluster."
 
 SUPPORTED_COMPUTE_VALUES = frozenset({"nodegroup", "fargate"})
 NODEGROUP_FULL_NAME = "Amazon EKS managed node groups"
 FARGATE_FULL_NAME = "AWS Fargate profiles"
 
 
+def _create_compute(
+    compute: str | None,
+    cluster_name: str,
+    aws_conn_id: str,
+    region: str | None,
+    waiter_delay: int,
+    waiter_max_attempts: int,
+    wait_for_completion: bool = False,
+    nodegroup_name: str | None = None,
+    nodegroup_role_arn: str | None = None,
+    create_nodegroup_kwargs: dict | None = None,
+    fargate_profile_name: str | None = None,
+    fargate_pod_execution_role_arn: str | None = None,
+    fargate_selectors: list | None = None,
+    create_fargate_profile_kwargs: dict | None = None,
+    subnets: list[str] | None = None,
+):
+    log = logging.getLogger(__name__)
+    eks_hook = EksHook(aws_conn_id=aws_conn_id, region_name=region)
+    if compute == "nodegroup" and nodegroup_name:
+        # this is to satisfy mypy
+        subnets = subnets or []
+        create_nodegroup_kwargs = create_nodegroup_kwargs or {}
+
+        eks_hook.create_nodegroup(
+            clusterName=cluster_name,
+            nodegroupName=nodegroup_name,
+            subnets=subnets,
+            nodeRole=nodegroup_role_arn,
+            **create_nodegroup_kwargs,
+        )
+        if wait_for_completion:
+            log.info("Waiting for nodegroup to provision.  This will take some time.")
+            wait(
+                waiter=eks_hook.conn.get_waiter("nodegroup_active"),
+                waiter_delay=waiter_delay,
+                waiter_max_attempts=waiter_max_attempts,
+                args={"clusterName": cluster_name, "nodegroupName": nodegroup_name},
+                failure_message="Nodegroup creation failed",
+                status_message="Nodegroup status is",
+                status_args=["nodegroup.status"],
+            )
+    elif compute == "fargate" and fargate_profile_name:
+        # this is to satisfy mypy
+        create_fargate_profile_kwargs = create_fargate_profile_kwargs or {}
+        fargate_selectors = fargate_selectors or []
+
+        eks_hook.create_fargate_profile(
+            clusterName=cluster_name,
+            fargateProfileName=fargate_profile_name,
+            podExecutionRoleArn=fargate_pod_execution_role_arn,
+            selectors=fargate_selectors,
+            **create_fargate_profile_kwargs,
+        )
+        if wait_for_completion:
+            log.info("Waiting for Fargate profile to provision.  This will take some time.")
+            wait(
+                waiter=eks_hook.conn.get_waiter("fargate_profile_active"),
+                waiter_delay=waiter_delay,
+                waiter_max_attempts=waiter_max_attempts,
+                args={"clusterName": cluster_name, "fargateProfileName": fargate_profile_name},
+                failure_message="Fargate profile creation failed",
+                status_message="Fargate profile status is",
+                status_args=["fargateProfile.status"],
+            )
+
+
 class EksCreateClusterOperator(BaseOperator):
     """
     Creates an Amazon EKS Cluster control plane.
 
     Optionally, can also create the supporting compute architecture:
 
      - If argument 'compute' is provided with a value of 'nodegroup', will also
@@ -108,14 +180,16 @@
 
     :param fargate_profile_name: *REQUIRED* The unique name to give your AWS Fargate profile. (templated)
     :param fargate_pod_execution_role_arn: *REQUIRED* The Amazon Resource Name (ARN) of the pod execution
          role to use for pods that match the selectors in the AWS Fargate profile. (templated)
     :param fargate_selectors: The selectors to match for pods to use this AWS Fargate profile. (templated)
     :param create_fargate_profile_kwargs: Optional parameters to pass to the CreateFargateProfile API
          (templated)
+    :param waiter_delay: Time (in seconds) to wait between two consecutive calls to check cluster state
+    :param waiter_max_attempts: The maximum number of attempts to check cluster state
 
     """
 
     template_fields: Sequence[str] = (
         "cluster_name",
         "cluster_role_arn",
         "resources_vpc_config",
@@ -133,45 +207,51 @@
         "region",
     )
 
     def __init__(
         self,
         cluster_name: str,
         cluster_role_arn: str,
-        resources_vpc_config: dict[str, Any],
+        resources_vpc_config: dict,
         compute: str | None = DEFAULT_COMPUTE_TYPE,
         create_cluster_kwargs: dict | None = None,
         nodegroup_name: str = DEFAULT_NODEGROUP_NAME,
         nodegroup_role_arn: str | None = None,
         create_nodegroup_kwargs: dict | None = None,
         fargate_profile_name: str = DEFAULT_FARGATE_PROFILE_NAME,
         fargate_pod_execution_role_arn: str | None = None,
         fargate_selectors: list | None = None,
         create_fargate_profile_kwargs: dict | None = None,
         wait_for_completion: bool = False,
         aws_conn_id: str = DEFAULT_CONN_ID,
         region: str | None = None,
+        waiter_delay: int = 30,
+        waiter_max_attempts: int = 40,
         **kwargs,
     ) -> None:
         self.compute = compute
         self.cluster_name = cluster_name
         self.cluster_role_arn = cluster_role_arn
         self.resources_vpc_config = resources_vpc_config
         self.create_cluster_kwargs = create_cluster_kwargs or {}
-        self.nodegroup_name = nodegroup_name
         self.nodegroup_role_arn = nodegroup_role_arn
-        self.create_nodegroup_kwargs = create_nodegroup_kwargs or {}
-        self.fargate_profile_name = fargate_profile_name
         self.fargate_pod_execution_role_arn = fargate_pod_execution_role_arn
-        self.fargate_selectors = fargate_selectors or [{"namespace": DEFAULT_NAMESPACE_NAME}]
         self.create_fargate_profile_kwargs = create_fargate_profile_kwargs or {}
         self.wait_for_completion = wait_for_completion
+        self.waiter_delay = waiter_delay
+        self.waiter_max_attempts = waiter_max_attempts
         self.aws_conn_id = aws_conn_id
         self.region = region
-        super().__init__(**kwargs)
+        self.nodegroup_name = nodegroup_name
+        self.create_nodegroup_kwargs = create_nodegroup_kwargs or {}
+        self.fargate_selectors = fargate_selectors or [{"namespace": DEFAULT_NAMESPACE_NAME}]
+        self.fargate_profile_name = fargate_profile_name
+        super().__init__(
+            **kwargs,
+        )
 
     def execute(self, context: Context):
         if self.compute:
             if self.compute not in SUPPORTED_COMPUTE_VALUES:
                 raise ValueError("Provided compute type is not supported.")
             elif (self.compute == "nodegroup") and not self.nodegroup_role_arn:
                 raise ValueError(
@@ -179,71 +259,60 @@
                 )
             elif (self.compute == "fargate") and not self.fargate_pod_execution_role_arn:
                 raise ValueError(
                     MISSING_ARN_MSG.format(
                         compute=FARGATE_FULL_NAME, requirement="fargate_pod_execution_role_arn"
                     )
                 )
-
-        eks_hook = EksHook(
-            aws_conn_id=self.aws_conn_id,
-            region_name=self.region,
-        )
-
-        eks_hook.create_cluster(
+        self.eks_hook = EksHook(aws_conn_id=self.aws_conn_id, region_name=self.region)
+        self.eks_hook.create_cluster(
             name=self.cluster_name,
             roleArn=self.cluster_role_arn,
             resourcesVpcConfig=self.resources_vpc_config,
             **self.create_cluster_kwargs,
         )
 
         # Short circuit early if we don't need to wait to attach compute
         # and the caller hasn't requested to wait for the cluster either.
         if not self.compute and not self.wait_for_completion:
             return None
 
         self.log.info("Waiting for EKS Cluster to provision.  This will take some time.")
-        client = eks_hook.conn
+        client = self.eks_hook.conn
 
         try:
-            client.get_waiter("cluster_active").wait(name=self.cluster_name)
+            client.get_waiter("cluster_active").wait(
+                name=self.cluster_name,
+                WaiterConfig={"Delay": self.waiter_delay, "MaxAttempts": self.waiter_max_attempts},
+            )
         except (ClientError, WaiterError) as e:
             self.log.error("Cluster failed to start and will be torn down.\n %s", e)
-            eks_hook.delete_cluster(name=self.cluster_name)
-            client.get_waiter("cluster_deleted").wait(name=self.cluster_name)
+            self.eks_hook.delete_cluster(name=self.cluster_name)
+            client.get_waiter("cluster_deleted").wait(
+                name=self.cluster_name,
+                WaiterConfig={"Delay": self.waiter_delay, "MaxAttempts": self.waiter_max_attempts},
+            )
             raise
-
-        if self.compute == "nodegroup":
-            eks_hook.create_nodegroup(
-                clusterName=self.cluster_name,
-                nodegroupName=self.nodegroup_name,
-                subnets=cast(List[str], self.resources_vpc_config.get("subnetIds")),
-                nodeRole=self.nodegroup_role_arn,
-                **self.create_nodegroup_kwargs,
-            )
-            if self.wait_for_completion:
-                self.log.info("Waiting for nodegroup to provision.  This will take some time.")
-                client.get_waiter("nodegroup_active").wait(
-                    clusterName=self.cluster_name,
-                    nodegroupName=self.nodegroup_name,
-                )
-        elif self.compute == "fargate":
-            eks_hook.create_fargate_profile(
-                clusterName=self.cluster_name,
-                fargateProfileName=self.fargate_profile_name,
-                podExecutionRoleArn=self.fargate_pod_execution_role_arn,
-                selectors=self.fargate_selectors,
-                **self.create_fargate_profile_kwargs,
-            )
-            if self.wait_for_completion:
-                self.log.info("Waiting for Fargate profile to provision.  This will take some time.")
-                client.get_waiter("fargate_profile_active").wait(
-                    clusterName=self.cluster_name,
-                    fargateProfileName=self.fargate_profile_name,
-                )
+        _create_compute(
+            compute=self.compute,
+            cluster_name=self.cluster_name,
+            aws_conn_id=self.aws_conn_id,
+            region=self.region,
+            wait_for_completion=self.wait_for_completion,
+            waiter_delay=self.waiter_delay,
+            waiter_max_attempts=self.waiter_max_attempts,
+            nodegroup_name=self.nodegroup_name,
+            nodegroup_role_arn=self.nodegroup_role_arn,
+            create_nodegroup_kwargs=self.create_nodegroup_kwargs,
+            fargate_profile_name=self.fargate_profile_name,
+            fargate_pod_execution_role_arn=self.fargate_pod_execution_role_arn,
+            fargate_selectors=self.fargate_selectors,
+            create_fargate_profile_kwargs=self.create_fargate_profile_kwargs,
+            subnets=cast(List[str], self.resources_vpc_config.get("subnetIds")),
+        )
 
 
 class EksCreateNodegroupOperator(BaseOperator):
     """
     Creates an Amazon EKS managed node group for an existing Amazon EKS Cluster.
 
     .. seealso::
@@ -261,14 +330,19 @@
     :param aws_conn_id: The Airflow connection used for AWS credentials. (templated)
          If this is None or empty then the default boto3 behaviour is used. If
          running Airflow in a distributed manner and aws_conn_id is None or
          empty, then the default boto3 configuration would be used (and must be
          maintained on each worker node).
     :param region: Which AWS region the connection should use. (templated)
         If this is None or empty then the default boto3 behaviour is used.
+    :param waiter_delay: Time (in seconds) to wait between two consecutive calls to check nodegroup state
+    :param waiter_max_attempts: The maximum number of attempts to check nodegroup state
+    :param deferrable: If True, the operator will wait asynchronously for the nodegroup to be created.
+        This implies waiting for completion. This mode requires aiobotocore module to be installed.
+        (default: False)
 
     """
 
     template_fields: Sequence[str] = (
         "cluster_name",
         "nodegroup_subnets",
         "nodegroup_role_arn",
@@ -285,58 +359,84 @@
         nodegroup_subnets: list[str] | str,
         nodegroup_role_arn: str,
         nodegroup_name: str = DEFAULT_NODEGROUP_NAME,
         create_nodegroup_kwargs: dict | None = None,
         wait_for_completion: bool = False,
         aws_conn_id: str = DEFAULT_CONN_ID,
         region: str | None = None,
+        waiter_delay: int = 30,
+        waiter_max_attempts: int = 80,
+        deferrable: bool = conf.getboolean("operators", "default_deferrable", fallback=False),
         **kwargs,
     ) -> None:
+        self.nodegroup_subnets = nodegroup_subnets
+        self.compute = "nodegroup"
         self.cluster_name = cluster_name
         self.nodegroup_role_arn = nodegroup_role_arn
         self.nodegroup_name = nodegroup_name
         self.create_nodegroup_kwargs = create_nodegroup_kwargs or {}
-        self.wait_for_completion = wait_for_completion
+        self.wait_for_completion = False if deferrable else wait_for_completion
         self.aws_conn_id = aws_conn_id
         self.region = region
-        self.nodegroup_subnets = nodegroup_subnets
+        self.waiter_delay = waiter_delay
+        self.waiter_max_attempts = waiter_max_attempts
+        self.deferrable = deferrable
         super().__init__(**kwargs)
 
     def execute(self, context: Context):
+        self.log.info(self.task_id)
         if isinstance(self.nodegroup_subnets, str):
             nodegroup_subnets_list: list[str] = []
             if self.nodegroup_subnets != "":
                 try:
-                    nodegroup_subnets_list = cast(List, literal_eval(self.nodegroup_subnets))
+                    nodegroup_subnets_list = cast(list, literal_eval(self.nodegroup_subnets))
                 except ValueError:
                     self.log.warning(
                         "The nodegroup_subnets should be List or string representing "
                         "Python list and is %s. Defaulting to []",
                         self.nodegroup_subnets,
                     )
             self.nodegroup_subnets = nodegroup_subnets_list
 
-        eks_hook = EksHook(
+        _create_compute(
+            compute=self.compute,
+            cluster_name=self.cluster_name,
             aws_conn_id=self.aws_conn_id,
-            region_name=self.region,
-        )
-        eks_hook.create_nodegroup(
-            clusterName=self.cluster_name,
-            nodegroupName=self.nodegroup_name,
+            region=self.region,
+            wait_for_completion=self.wait_for_completion,
+            waiter_delay=self.waiter_delay,
+            waiter_max_attempts=self.waiter_max_attempts,
+            nodegroup_name=self.nodegroup_name,
+            nodegroup_role_arn=self.nodegroup_role_arn,
+            create_nodegroup_kwargs=self.create_nodegroup_kwargs,
             subnets=self.nodegroup_subnets,
-            nodeRole=self.nodegroup_role_arn,
-            **self.create_nodegroup_kwargs,
         )
 
-        if self.wait_for_completion:
-            self.log.info("Waiting for nodegroup to provision.  This will take some time.")
-            eks_hook.conn.get_waiter("nodegroup_active").wait(
-                clusterName=self.cluster_name, nodegroupName=self.nodegroup_name
+        if self.deferrable:
+            self.defer(
+                trigger=EksNodegroupTrigger(
+                    waiter_name="nodegroup_active",
+                    cluster_name=self.cluster_name,
+                    nodegroup_name=self.nodegroup_name,
+                    aws_conn_id=self.aws_conn_id,
+                    region=self.region,
+                    waiter_delay=self.waiter_delay,
+                    waiter_max_attempts=self.waiter_max_attempts,
+                ),
+                method_name="execute_complete",
+                # timeout is set to ensure that if a trigger dies, the timeout does not restart
+                # 60 seconds is added to allow the trigger to exit gracefully (i.e. yield TriggerEvent)
+                timeout=timedelta(seconds=self.waiter_max_attempts * self.waiter_delay + 60),
             )
 
+    def execute_complete(self, context, event=None):
+        if event["status"] != "success":
+            raise AirflowException(f"Error creating nodegroup: {event}")
+        return
+
 
 class EksCreateFargateProfileOperator(BaseOperator):
     """
     Creates an AWS Fargate profile for an Amazon EKS cluster.
 
     .. seealso::
         For more information on how to use this operator, take a look at the guide:
@@ -384,64 +484,62 @@
         fargate_profile_name: str = DEFAULT_FARGATE_PROFILE_NAME,
         create_fargate_profile_kwargs: dict | None = None,
         wait_for_completion: bool = False,
         aws_conn_id: str = DEFAULT_CONN_ID,
         region: str | None = None,
         waiter_delay: int = 10,
         waiter_max_attempts: int = 60,
-        deferrable: bool = False,
+        deferrable: bool = conf.getboolean("operators", "default_deferrable", fallback=False),
         **kwargs,
     ) -> None:
         self.cluster_name = cluster_name
-        self.pod_execution_role_arn = pod_execution_role_arn
         self.selectors = selectors
+        self.pod_execution_role_arn = pod_execution_role_arn
         self.fargate_profile_name = fargate_profile_name
         self.create_fargate_profile_kwargs = create_fargate_profile_kwargs or {}
-        self.wait_for_completion = wait_for_completion
+        self.wait_for_completion = False if deferrable else wait_for_completion
         self.aws_conn_id = aws_conn_id
         self.region = region
         self.waiter_delay = waiter_delay
         self.waiter_max_attempts = waiter_max_attempts
         self.deferrable = deferrable
-        super().__init__(**kwargs)
+        self.compute = "fargate"
+        super().__init__(
+            **kwargs,
+        )
 
     def execute(self, context: Context):
-        eks_hook = EksHook(
+        _create_compute(
+            compute=self.compute,
+            cluster_name=self.cluster_name,
             aws_conn_id=self.aws_conn_id,
-            region_name=self.region,
-        )
-
-        eks_hook.create_fargate_profile(
-            clusterName=self.cluster_name,
-            fargateProfileName=self.fargate_profile_name,
-            podExecutionRoleArn=self.pod_execution_role_arn,
-            selectors=self.selectors,
-            **self.create_fargate_profile_kwargs,
+            region=self.region,
+            wait_for_completion=self.wait_for_completion,
+            waiter_delay=self.waiter_delay,
+            waiter_max_attempts=self.waiter_max_attempts,
+            fargate_profile_name=self.fargate_profile_name,
+            fargate_pod_execution_role_arn=self.pod_execution_role_arn,
+            fargate_selectors=self.selectors,
+            create_fargate_profile_kwargs=self.create_fargate_profile_kwargs,
         )
         if self.deferrable:
             self.defer(
                 trigger=EksCreateFargateProfileTrigger(
                     cluster_name=self.cluster_name,
                     fargate_profile_name=self.fargate_profile_name,
                     aws_conn_id=self.aws_conn_id,
-                    poll_interval=self.waiter_delay,
-                    max_attempts=self.waiter_max_attempts,
+                    waiter_delay=self.waiter_delay,
+                    waiter_max_attempts=self.waiter_max_attempts,
+                    region=self.region,
                 ),
                 method_name="execute_complete",
                 # timeout is set to ensure that if a trigger dies, the timeout does not restart
                 # 60 seconds is added to allow the trigger to exit gracefully (i.e. yield TriggerEvent)
                 timeout=timedelta(seconds=(self.waiter_max_attempts * self.waiter_delay + 60)),
             )
-        elif self.wait_for_completion:
-            self.log.info("Waiting for Fargate profile to provision.  This will take some time.")
-            eks_hook.conn.get_waiter("fargate_profile_active").wait(
-                clusterName=self.cluster_name,
-                fargateProfileName=self.fargate_profile_name,
-                WaiterConfig={"Delay": self.waiter_delay, "MaxAttempts": self.waiter_max_attempts},
-            )
 
     def execute_complete(self, context, event=None):
         if event["status"] != "success":
             raise AirflowException(f"Error creating Fargate profile: {event}")
         else:
             self.log.info("Fargate profile created successfully")
         return
@@ -562,14 +660,19 @@
     :param aws_conn_id: The Airflow connection used for AWS credentials. (templated)
          If this is None or empty then the default boto3 behaviour is used.  If
          running Airflow in a distributed manner and aws_conn_id is None or
          empty, then the default boto3 configuration would be used (and must be
          maintained on each worker node).
     :param region: Which AWS region the connection should use. (templated)
         If this is None or empty then the default boto3 behaviour is used.
+    :param waiter_delay: Time (in seconds) to wait between two consecutive calls to check nodegroup state
+    :param waiter_max_attempts: The maximum number of attempts to check nodegroup state
+    :param deferrable: If True, the operator will wait asynchronously for the nodegroup to be deleted.
+        This implies waiting for completion. This mode requires aiobotocore module to be installed.
+        (default: False)
 
     """
 
     template_fields: Sequence[str] = (
         "cluster_name",
         "nodegroup_name",
         "wait_for_completion",
@@ -580,36 +683,63 @@
     def __init__(
         self,
         cluster_name: str,
         nodegroup_name: str,
         wait_for_completion: bool = False,
         aws_conn_id: str = DEFAULT_CONN_ID,
         region: str | None = None,
+        waiter_delay: int = 30,
+        waiter_max_attempts: int = 40,
+        deferrable: bool = conf.getboolean("operators", "default_deferrable", fallback=False),
         **kwargs,
     ) -> None:
         self.cluster_name = cluster_name
         self.nodegroup_name = nodegroup_name
         self.wait_for_completion = wait_for_completion
         self.aws_conn_id = aws_conn_id
         self.region = region
+        self.waiter_delay = waiter_delay
+        self.waiter_max_attempts = waiter_max_attempts
+        self.deferrable = deferrable
         super().__init__(**kwargs)
 
     def execute(self, context: Context):
         eks_hook = EksHook(
             aws_conn_id=self.aws_conn_id,
             region_name=self.region,
         )
 
         eks_hook.delete_nodegroup(clusterName=self.cluster_name, nodegroupName=self.nodegroup_name)
-        if self.wait_for_completion:
+        if self.deferrable:
+            self.defer(
+                trigger=EksNodegroupTrigger(
+                    waiter_name="nodegroup_deleted",
+                    cluster_name=self.cluster_name,
+                    nodegroup_name=self.nodegroup_name,
+                    aws_conn_id=self.aws_conn_id,
+                    region=self.region,
+                    waiter_delay=self.waiter_delay,
+                    waiter_max_attempts=self.waiter_max_attempts,
+                ),
+                method_name="execute_complete",
+                # timeout is set to ensure that if a trigger dies, the timeout does not restart
+                # 60 seconds is added to allow the trigger to exit gracefully (i.e. yield TriggerEvent)
+                timeout=timedelta(seconds=self.waiter_max_attempts * self.waiter_delay + 60),
+            )
+        elif self.wait_for_completion:
             self.log.info("Waiting for nodegroup to delete.  This will take some time.")
             eks_hook.conn.get_waiter("nodegroup_deleted").wait(
                 clusterName=self.cluster_name, nodegroupName=self.nodegroup_name
             )
 
+    def execute_complete(self, context, event=None):
+        if event["status"] != "success":
+            raise AirflowException(f"Error deleting nodegroup: {event}")
+        return
+
 
 class EksDeleteFargateProfileOperator(BaseOperator):
     """
     Deletes an AWS Fargate profile from an Amazon EKS Cluster.
 
     .. seealso::
         For more information on how to use this operator, take a look at the guide:
@@ -645,15 +775,15 @@
         cluster_name: str,
         fargate_profile_name: str,
         wait_for_completion: bool = False,
         aws_conn_id: str = DEFAULT_CONN_ID,
         region: str | None = None,
         waiter_delay: int = 30,
         waiter_max_attempts: int = 60,
-        deferrable: bool = False,
+        deferrable: bool = conf.getboolean("operators", "default_deferrable", fallback=False),
         **kwargs,
     ) -> None:
         super().__init__(**kwargs)
         self.cluster_name = cluster_name
         self.fargate_profile_name = fargate_profile_name
         self.wait_for_completion = wait_for_completion
         self.aws_conn_id = aws_conn_id
@@ -673,16 +803,17 @@
         )
         if self.deferrable:
             self.defer(
                 trigger=EksDeleteFargateProfileTrigger(
                     cluster_name=self.cluster_name,
                     fargate_profile_name=self.fargate_profile_name,
                     aws_conn_id=self.aws_conn_id,
-                    poll_interval=self.waiter_delay,
-                    max_attempts=self.waiter_max_attempts,
+                    waiter_delay=self.waiter_delay,
+                    waiter_max_attempts=self.waiter_max_attempts,
+                    region=self.region,
                 ),
                 method_name="execute_complete",
                 # timeout is set to ensure that if a trigger dies, the timeout does not restart
                 # 60 seconds is added to allow the trigger to exit gracefully (i.e. yield TriggerEvent)
                 timeout=timedelta(seconds=(self.waiter_max_attempts * self.waiter_delay + 60)),
             )
         elif self.wait_for_completion:
@@ -719,18 +850,23 @@
     :param region: Which AWS region the connection should use. (templated)
          If this is None or empty then the default boto3 behaviour is used.
     :param aws_conn_id: The Airflow connection used for AWS credentials. (templated)
          If this is None or empty then the default boto3 behaviour is used. If
          running Airflow in a distributed manner and aws_conn_id is None or
          empty, then the default boto3 configuration would be used (and must be
          maintained on each worker node).
+    :param on_finish_action: What to do when the pod reaches its final state, or the execution is interrupted.
+        If "delete_pod", the pod will be deleted regardless it's state; if "delete_succeeded_pod",
+        only succeeded pod will be deleted. You can set to "keep_pod" to keep the pod.
+        Current default is `keep_pod`, but this will be changed in the next major release of this provider.
     :param is_delete_operator_pod: What to do when the pod reaches its final
         state, or the execution is interrupted. If True, delete the
-        pod; if False, leave the pod.  Current default is False, but this will be
+        pod; if False, leave the pod. Current default is False, but this will be
         changed in the next major release of this provider.
+        Deprecated - use `on_finish_action` instead.
 
     """
 
     template_fields: Sequence[str] = tuple(
         {
             "cluster_name",
             "in_cluster",
@@ -750,39 +886,51 @@
         in_cluster: bool = False,
         namespace: str = DEFAULT_NAMESPACE_NAME,
         pod_context: str | None = None,
         pod_name: str | None = None,
         pod_username: str | None = None,
         aws_conn_id: str = DEFAULT_CONN_ID,
         region: str | None = None,
+        on_finish_action: str | None = None,
         is_delete_operator_pod: bool | None = None,
         **kwargs,
     ) -> None:
-        if is_delete_operator_pod is None:
+        if is_delete_operator_pod is not None:
             warnings.warn(
-                f"You have not set parameter `is_delete_operator_pod` in class {self.__class__.__name__}. "
-                "Currently the default for this parameter is `False` but in a future release the default "
-                "will be changed to `True`. To ensure pods are not deleted in the future you will need to "
-                "set `is_delete_operator_pod=False` explicitly.",
+                "`is_delete_operator_pod` parameter is deprecated, please use `on_finish_action`",
                 AirflowProviderDeprecationWarning,
                 stacklevel=2,
             )
-            is_delete_operator_pod = False
+            kwargs["on_finish_action"] = (
+                OnFinishAction.DELETE_POD if is_delete_operator_pod else OnFinishAction.KEEP_POD
+            )
+        else:
+            if on_finish_action is not None:
+                kwargs["on_finish_action"] = OnFinishAction(on_finish_action)
+            else:
+                warnings.warn(
+                    f"You have not set parameter `on_finish_action` in class {self.__class__.__name__}. "
+                    "Currently the default for this parameter is `keep_pod` but in a future release"
+                    " the default will be changed to `delete_pod`. To ensure pods are not deleted in"
+                    " the future you will need to set `on_finish_action=keep_pod` explicitly.",
+                    AirflowProviderDeprecationWarning,
+                    stacklevel=2,
+                )
+                kwargs["on_finish_action"] = OnFinishAction.KEEP_POD
 
         self.cluster_name = cluster_name
         self.in_cluster = in_cluster
         self.namespace = namespace
         self.pod_name = pod_name
         self.aws_conn_id = aws_conn_id
         self.region = region
         super().__init__(
             in_cluster=self.in_cluster,
             namespace=self.namespace,
             name=self.pod_name,
-            is_delete_operator_pod=is_delete_operator_pod,
             **kwargs,
         )
         # There is no need to manage the kube_config file, as it will be generated automatically.
         # All Kubernetes parameters (except config_file) are also valid for the EksPodOperator.
         if self.config_file:
             raise AirflowException("The config_file is not an allowed parameter for the EksPodOperator.")
```

### Comparing `apache-airflow-providers-amazon-8.2.0rc1/airflow/providers/amazon/aws/operators/emr.py` & `apache-airflow-providers-amazon-8.3.0rc1/airflow/providers/amazon/aws/operators/emr.py`

 * *Files 12% similar despite different names*

```diff
@@ -20,24 +20,27 @@
 import ast
 import warnings
 from datetime import timedelta
 from functools import cached_property
 from typing import TYPE_CHECKING, Any, Sequence
 from uuid import uuid4
 
+from airflow.configuration import conf
 from airflow.exceptions import AirflowException, AirflowProviderDeprecationWarning
 from airflow.models import BaseOperator
 from airflow.providers.amazon.aws.hooks.emr import EmrContainerHook, EmrHook, EmrServerlessHook
 from airflow.providers.amazon.aws.links.emr import EmrClusterLink, EmrLogsLink, get_log_uri
 from airflow.providers.amazon.aws.triggers.emr import (
     EmrAddStepsTrigger,
+    EmrContainerTrigger,
     EmrCreateJobFlowTrigger,
     EmrTerminateJobFlowTrigger,
 )
 from airflow.providers.amazon.aws.utils.waiter import waiter
+from airflow.providers.amazon.aws.utils.waiter_with_logging import wait
 from airflow.utils.helpers import exactly_one, prune_dict
 from airflow.utils.types import NOTSET, ArgNotSet
 
 if TYPE_CHECKING:
     from airflow.utils.context import Context
 
 
@@ -90,15 +93,15 @@
         cluster_states: list[str] | None = None,
         aws_conn_id: str = "aws_default",
         steps: list[dict] | str | None = None,
         wait_for_completion: bool = False,
         waiter_delay: int | None = None,
         waiter_max_attempts: int | None = None,
         execution_role_arn: str | None = None,
-        deferrable: bool = False,
+        deferrable: bool = conf.getboolean("operators", "default_deferrable", fallback=False),
         **kwargs,
     ):
         if not exactly_one(job_flow_id is None, job_flow_name is None):
             raise AirflowException("Exactly one of job_flow_id or job_flow_name must be specified.")
         super().__init__(**kwargs)
         cluster_states = cluster_states or []
         steps = steps or []
@@ -475,14 +478,15 @@
     :param wait_for_completion: Whether or not to wait in the operator for the job to complete.
     :param poll_interval: Time (in seconds) to wait between two consecutive calls to check query status on EMR
     :param max_tries: Deprecated - use max_polling_attempts instead.
     :param max_polling_attempts: Maximum number of times to wait for the job run to finish.
         Defaults to None, which will poll until the job is *not* in a pending, submitted, or running state.
     :param tags: The tags assigned to job runs.
         Defaults to None
+    :param deferrable: Run operator in the deferrable mode.
     """
 
     template_fields: Sequence[str] = (
         "name",
         "virtual_cluster_id",
         "execution_role_arn",
         "release_label",
@@ -503,14 +507,15 @@
         client_request_token: str | None = None,
         aws_conn_id: str = "aws_default",
         wait_for_completion: bool = True,
         poll_interval: int = 30,
         max_tries: int | None = None,
         tags: dict | None = None,
         max_polling_attempts: int | None = None,
+        deferrable: bool = conf.getboolean("operators", "default_deferrable", fallback=False),
         **kwargs: Any,
     ) -> None:
         super().__init__(**kwargs)
         self.name = name
         self.virtual_cluster_id = virtual_cluster_id
         self.execution_role_arn = execution_role_arn
         self.release_label = release_label
@@ -519,14 +524,15 @@
         self.aws_conn_id = aws_conn_id
         self.client_request_token = client_request_token or str(uuid4())
         self.wait_for_completion = wait_for_completion
         self.poll_interval = poll_interval
         self.max_polling_attempts = max_polling_attempts
         self.tags = tags
         self.job_id: str | None = None
+        self.deferrable = deferrable
 
         if max_tries:
             warnings.warn(
                 f"Parameter `{self.__class__.__name__}.max_tries` is deprecated and will be removed "
                 "in a future release.  Please use method `max_polling_attempts` instead.",
                 AirflowProviderDeprecationWarning,
                 stacklevel=2,
@@ -551,35 +557,65 @@
             self.execution_role_arn,
             self.release_label,
             self.job_driver,
             self.configuration_overrides,
             self.client_request_token,
             self.tags,
         )
+        if self.deferrable:
+            query_status = self.hook.check_query_status(job_id=self.job_id)
+            self.check_failure(query_status)
+            if query_status in EmrContainerHook.SUCCESS_STATES:
+                return self.job_id
+            timeout = (
+                timedelta(seconds=self.max_polling_attempts * self.poll_interval)
+                if self.max_polling_attempts
+                else self.execution_timeout
+            )
+            self.defer(
+                timeout=timeout,
+                trigger=EmrContainerTrigger(
+                    virtual_cluster_id=self.virtual_cluster_id,
+                    job_id=self.job_id,
+                    aws_conn_id=self.aws_conn_id,
+                    poll_interval=self.poll_interval,
+                ),
+                method_name="execute_complete",
+            )
         if self.wait_for_completion:
             query_status = self.hook.poll_query_status(
                 self.job_id,
                 max_polling_attempts=self.max_polling_attempts,
                 poll_interval=self.poll_interval,
             )
 
-            if query_status in EmrContainerHook.FAILURE_STATES:
-                error_message = self.hook.get_job_failure_reason(self.job_id)
-                raise AirflowException(
-                    f"EMR Containers job failed. Final state is {query_status}. "
-                    f"query_execution_id is {self.job_id}. Error: {error_message}"
-                )
-            elif not query_status or query_status in EmrContainerHook.INTERMEDIATE_STATES:
+            self.check_failure(query_status)
+            if not query_status or query_status in EmrContainerHook.INTERMEDIATE_STATES:
                 raise AirflowException(
                     f"Final state of EMR Containers job is {query_status}. "
                     f"Max tries of poll status exceeded, query_execution_id is {self.job_id}."
                 )
 
         return self.job_id
 
+    def check_failure(self, query_status):
+        if query_status in EmrContainerHook.FAILURE_STATES:
+            error_message = self.hook.get_job_failure_reason(self.job_id)
+            raise AirflowException(
+                f"EMR Containers job failed. Final state is {query_status}. "
+                f"query_execution_id is {self.job_id}. Error: {error_message}"
+            )
+
+    def execute_complete(self, context, event=None):
+        if event["status"] != "success":
+            raise AirflowException(f"Error while running job: {event}")
+
+        self.log.info("%s", event["message"])
+        return event["job_id"]
+
     def on_kill(self) -> None:
         """Cancel the submitted job run."""
         if self.job_id:
             self.log.info("Stopping job run with jobId - %s", self.job_id)
             response = self.hook.stop_query(self.job_id)
             http_status_code = None
             try:
@@ -596,16 +632,16 @@
                     )
                     self.hook.poll_query_status(self.job_id)
 
 
 class EmrCreateJobFlowOperator(BaseOperator):
     """
     Creates an EMR JobFlow, reading the config from the EMR connection.
-    A dictionary of JobFlow overrides can be passed that override
-    the config from the connection.
+
+    A dictionary of JobFlow overrides can be passed that override the config from the connection.
 
     .. seealso::
         For more information on how to use this operator, take a look at the guide:
         :ref:`howto/operator:EmrCreateJobFlowOperator`
 
     :param aws_conn_id: The Airflow connection used for AWS credentials.
         If this is None or empty then the default boto3 behaviour is used. If
@@ -656,15 +692,15 @@
         region_name: str | None = None,
         wait_for_completion: bool = False,
         # TODO: waiter_max_attempts and waiter_delay should default to None when the other two are deprecated.
         waiter_max_attempts: int | None | ArgNotSet = NOTSET,
         waiter_delay: int | None | ArgNotSet = NOTSET,
         waiter_countdown: int | None = None,
         waiter_check_interval_seconds: int = 60,
-        deferrable: bool = False,
+        deferrable: bool = conf.getboolean("operators", "default_deferrable", fallback=False),
         **kwargs: Any,
     ):
         if waiter_max_attempts is NOTSET:
             warnings.warn(
                 "The parameter waiter_countdown has been deprecated to standardize "
                 "naming conventions.  Please use waiter_max_attempts instead.  In the "
                 "future this will default to None and defer to the waiter's default value."
@@ -758,18 +794,15 @@
         if event["status"] != "success":
             raise AirflowException(f"Error creating jobFlow: {event}")
         else:
             self.log.info("JobFlow created successfully")
         return event["job_flow_id"]
 
     def on_kill(self) -> None:
-        """
-        Terminate the EMR cluster (job flow). If TerminationProtected=True on the cluster,
-        termination will be unsuccessful.
-        """
+        """Terminate the EMR cluster (job flow) unless TerminationProtected is enabled on the cluster."""
         if self._job_flow_id:
             self.log.info("Terminating job flow %s", self._job_flow_id)
             self._emr_hook.conn.terminate_job_flows(JobFlowIds=[self._job_flow_id])
 
 
 class EmrModifyClusterOperator(BaseOperator):
     """
@@ -864,15 +897,15 @@
     def __init__(
         self,
         *,
         job_flow_id: str,
         aws_conn_id: str = "aws_default",
         waiter_delay: int = 60,
         waiter_max_attempts: int = 20,
-        deferrable: bool = False,
+        deferrable: bool = conf.getboolean("operators", "default_deferrable", fallback=False),
         **kwargs,
     ):
         super().__init__(**kwargs)
         self.job_flow_id = job_flow_id
         self.aws_conn_id = aws_conn_id
         self.waiter_delay = waiter_delay
         self.waiter_max_attempts = waiter_max_attempts
@@ -941,40 +974,66 @@
     :param wait_for_completion: If true, wait for the Application to start before returning. Default to True.
         If set to False, ``waiter_countdown`` and ``waiter_check_interval_seconds`` will only be applied when
         waiting for the application to be in the ``CREATED`` state.
     :param client_request_token: The client idempotency token of the application to create.
       Its value must be unique for each request.
     :param config: Optional dictionary for arbitrary parameters to the boto API create_application call.
     :param aws_conn_id: AWS connection to use
-    :param waiter_countdown: Total amount of time, in seconds, the operator will wait for
+    :param waiter_countdown: (deprecated) Total amount of time, in seconds, the operator will wait for
         the application to start. Defaults to 25 minutes.
-    :param waiter_check_interval_seconds: Number of seconds between polling the state of the application.
-        Defaults to 60 seconds.
+    :param waiter_check_interval_seconds: (deprecated) Number of seconds between polling the state
+        of the application. Defaults to 60 seconds.
+    :waiter_max_attempts: Number of times the waiter should poll the application to check the state.
+        If not set, the waiter will use its default value.
+    :param waiter_delay: Number of seconds between polling the state of the application.
     """
 
     def __init__(
         self,
         release_label: str,
         job_type: str,
         client_request_token: str = "",
         config: dict | None = None,
         wait_for_completion: bool = True,
         aws_conn_id: str = "aws_default",
-        waiter_countdown: int = 25 * 60,
-        waiter_check_interval_seconds: int = 60,
+        waiter_countdown: int | ArgNotSet = NOTSET,
+        waiter_check_interval_seconds: int | ArgNotSet = NOTSET,
+        waiter_max_attempts: int | ArgNotSet = NOTSET,
+        waiter_delay: int | ArgNotSet = NOTSET,
         **kwargs,
     ):
+        if waiter_check_interval_seconds is NOTSET:
+            waiter_delay = 60 if waiter_delay is NOTSET else waiter_delay
+        else:
+            waiter_delay = waiter_check_interval_seconds if waiter_delay is NOTSET else waiter_delay
+            warnings.warn(
+                "The parameter waiter_check_interval_seconds has been deprecated to standardize "
+                "naming conventions.  Please use waiter_delay instead.  In the "
+                "future this will default to None and defer to the waiter's default value."
+            )
+        if waiter_countdown is NOTSET:
+            waiter_max_attempts = 25 if waiter_max_attempts is NOTSET else waiter_max_attempts
+        else:
+            if waiter_max_attempts is NOTSET:
+                # ignoring mypy because it doesn't like ArgNotSet as an operand, but neither variables
+                # are of type ArgNotSet at this point.
+                waiter_max_attempts = waiter_countdown // waiter_delay  # type: ignore[operator]
+            warnings.warn(
+                "The parameter waiter_countdown has been deprecated to standardize "
+                "naming conventions.  Please use waiter_max_attempts instead. In the "
+                "future this will default to None and defer to the waiter's default value."
+            )
         self.aws_conn_id = aws_conn_id
         self.release_label = release_label
         self.job_type = job_type
         self.wait_for_completion = wait_for_completion
         self.kwargs = kwargs
         self.config = config or {}
-        self.waiter_countdown = waiter_countdown
-        self.waiter_check_interval_seconds = waiter_check_interval_seconds
+        self.waiter_max_attempts = int(waiter_max_attempts)  # type: ignore[arg-type]
+        self.waiter_delay = int(waiter_delay)  # type: ignore[arg-type]
         super().__init__(**kwargs)
 
         self.client_request_token = client_request_token or str(uuid4())
 
     @cached_property
     def hook(self) -> EmrServerlessHook:
         """Create and return an EmrServerlessHook."""
@@ -989,45 +1048,39 @@
         )
         application_id = response["applicationId"]
 
         if response["ResponseMetadata"]["HTTPStatusCode"] != 200:
             raise AirflowException(f"Application Creation failed: {response}")
 
         self.log.info("EMR serverless application created: %s", application_id)
+        waiter = self.hook.get_waiter("serverless_app_created")
 
-        # This should be replaced with a boto waiter when available.
-        waiter(
-            get_state_callable=self.hook.conn.get_application,
-            get_state_args={"applicationId": application_id},
-            parse_response=["application", "state"],
-            desired_state={"CREATED"},
-            failure_states=EmrServerlessHook.APPLICATION_FAILURE_STATES,
-            object_type="application",
-            action="created",
-            countdown=self.waiter_countdown,
-            check_interval_seconds=self.waiter_check_interval_seconds,
+        wait(
+            waiter=waiter,
+            waiter_delay=self.waiter_delay,
+            waiter_max_attempts=self.waiter_max_attempts,
+            args={"applicationId": application_id},
+            failure_message="Serverless Application creation failed",
+            status_message="Serverless Application status is",
+            status_args=["application.state", "application.stateDetails"],
         )
-
         self.log.info("Starting application %s", application_id)
         self.hook.conn.start_application(applicationId=application_id)
 
         if self.wait_for_completion:
-            # This should be replaced with a boto waiter when available.
-            waiter(
-                get_state_callable=self.hook.conn.get_application,
-                get_state_args={"applicationId": application_id},
-                parse_response=["application", "state"],
-                desired_state={"STARTED"},
-                failure_states=EmrServerlessHook.APPLICATION_FAILURE_STATES,
-                object_type="application",
-                action="started",
-                countdown=self.waiter_countdown,
-                check_interval_seconds=self.waiter_check_interval_seconds,
+            waiter = self.hook.get_waiter("serverless_app_started")
+            wait(
+                waiter=waiter,
+                waiter_max_attempts=self.waiter_max_attempts,
+                waiter_delay=self.waiter_delay,
+                args={"applicationId": application_id},
+                failure_message="Serverless Application failed to start",
+                status_message="Serverless Application status is",
+                status_args=["application.state", "application.stateDetails"],
             )
-
         return application_id
 
 
 class EmrServerlessStartJobOperator(BaseOperator):
     """
     Operator to start EMR Serverless job.
 
@@ -1043,18 +1096,21 @@
       Its value must be unique for each request.
     :param config: Optional dictionary for arbitrary parameters to the boto API start_job_run call.
     :param wait_for_completion: If true, waits for the job to start before returning. Defaults to True.
         If set to False, ``waiter_countdown`` and ``waiter_check_interval_seconds`` will only be applied
         when waiting for the application be to in the ``STARTED`` state.
     :param aws_conn_id: AWS connection to use.
     :param name: Name for the EMR Serverless job. If not provided, a default name will be assigned.
-    :param waiter_countdown: Total amount of time, in seconds, the operator will wait for
+    :param waiter_countdown: (deprecated) Total amount of time, in seconds, the operator will wait for
         the job finish. Defaults to 25 minutes.
-    :param waiter_check_interval_seconds: Number of seconds between polling the state of the job.
+    :param waiter_check_interval_seconds: (deprecated) Number of seconds between polling the state of the job.
         Defaults to 60 seconds.
+    :waiter_max_attempts: Number of times the waiter should poll the application to check the state.
+        If not set, the waiter will use its default value.
+    :param waiter_delay: Number of seconds between polling the state of the job run.
     """
 
     template_fields: Sequence[str] = (
         "application_id",
         "config",
         "execution_role_arn",
         "job_driver",
@@ -1073,28 +1129,51 @@
         job_driver: dict,
         configuration_overrides: dict | None,
         client_request_token: str = "",
         config: dict | None = None,
         wait_for_completion: bool = True,
         aws_conn_id: str = "aws_default",
         name: str | None = None,
-        waiter_countdown: int = 25 * 60,
-        waiter_check_interval_seconds: int = 60,
+        waiter_countdown: int | ArgNotSet = NOTSET,
+        waiter_check_interval_seconds: int | ArgNotSet = NOTSET,
+        waiter_max_attempts: int | ArgNotSet = NOTSET,
+        waiter_delay: int | ArgNotSet = NOTSET,
         **kwargs,
     ):
+        if waiter_check_interval_seconds is NOTSET:
+            waiter_delay = 60 if waiter_delay is NOTSET else waiter_delay
+        else:
+            waiter_delay = waiter_check_interval_seconds if waiter_delay is NOTSET else waiter_delay
+            warnings.warn(
+                "The parameter waiter_check_interval_seconds has been deprecated to standardize "
+                "naming conventions.  Please use waiter_delay instead.  In the "
+                "future this will default to None and defer to the waiter's default value."
+            )
+        if waiter_countdown is NOTSET:
+            waiter_max_attempts = 25 if waiter_max_attempts is NOTSET else waiter_max_attempts
+        else:
+            if waiter_max_attempts is NOTSET:
+                # ignoring mypy because it doesn't like ArgNotSet as an operand, but neither variables
+                # are of type ArgNotSet at this point.
+                waiter_max_attempts = waiter_countdown // waiter_delay  # type: ignore[operator]
+            warnings.warn(
+                "The parameter waiter_countdown has been deprecated to standardize "
+                "naming conventions.  Please use waiter_max_attempts instead.  In the "
+                "future this will default to None and defer to the waiter's default value."
+            )
         self.aws_conn_id = aws_conn_id
         self.application_id = application_id
         self.execution_role_arn = execution_role_arn
         self.job_driver = job_driver
         self.configuration_overrides = configuration_overrides
         self.wait_for_completion = wait_for_completion
         self.config = config or {}
         self.name = name or self.config.pop("name", f"emr_serverless_job_airflow_{uuid4()}")
-        self.waiter_countdown = waiter_countdown
-        self.waiter_check_interval_seconds = waiter_check_interval_seconds
+        self.waiter_max_attempts = int(waiter_max_attempts)  # type: ignore[arg-type]
+        self.waiter_delay = int(waiter_delay)  # type: ignore[arg-type]
         self.job_id: str | None = None
         super().__init__(**kwargs)
 
         self.client_request_token = client_request_token or str(uuid4())
 
     @cached_property
     def hook(self) -> EmrServerlessHook:
@@ -1103,25 +1182,24 @@
 
     def execute(self, context: Context) -> str | None:
         self.log.info("Starting job on Application: %s", self.application_id)
 
         app_state = self.hook.conn.get_application(applicationId=self.application_id)["application"]["state"]
         if app_state not in EmrServerlessHook.APPLICATION_SUCCESS_STATES:
             self.hook.conn.start_application(applicationId=self.application_id)
+            waiter = self.hook.get_waiter("serverless_app_started")
 
-            waiter(
-                get_state_callable=self.hook.conn.get_application,
-                get_state_args={"applicationId": self.application_id},
-                parse_response=["application", "state"],
-                desired_state={"STARTED"},
-                failure_states=EmrServerlessHook.APPLICATION_FAILURE_STATES,
-                object_type="application",
-                action="started",
-                countdown=self.waiter_countdown,
-                check_interval_seconds=self.waiter_check_interval_seconds,
+            wait(
+                waiter=waiter,
+                waiter_max_attempts=self.waiter_max_attempts,
+                waiter_delay=self.waiter_delay,
+                args={"applicationId": self.application_id},
+                failure_message="Serverless Application failed to start",
+                status_message="Serverless Application status is",
+                status_args=["application.state", "application.stateDetails"],
             )
 
         response = self.hook.conn.start_job_run(
             clientToken=self.client_request_token,
             applicationId=self.application_id,
             executionRoleArn=self.execution_role_arn,
             jobDriver=self.job_driver,
@@ -1132,29 +1210,25 @@
 
         if response["ResponseMetadata"]["HTTPStatusCode"] != 200:
             raise AirflowException(f"EMR serverless job failed to start: {response}")
 
         self.job_id = response["jobRunId"]
         self.log.info("EMR serverless job started: %s", self.job_id)
         if self.wait_for_completion:
-            # This should be replaced with a boto waiter when available.
-            waiter(
-                get_state_callable=self.hook.conn.get_job_run,
-                get_state_args={
-                    "applicationId": self.application_id,
-                    "jobRunId": self.job_id,
-                },
-                parse_response=["jobRun", "state"],
-                desired_state=EmrServerlessHook.JOB_SUCCESS_STATES,
-                failure_states=EmrServerlessHook.JOB_FAILURE_STATES,
-                object_type="job",
-                action="run",
-                countdown=self.waiter_countdown,
-                check_interval_seconds=self.waiter_check_interval_seconds,
+            waiter = self.hook.get_waiter("serverless_job_completed")
+            wait(
+                waiter=waiter,
+                waiter_max_attempts=self.waiter_max_attempts,
+                waiter_delay=self.waiter_delay,
+                args={"applicationId": self.application_id, "jobRunId": self.job_id},
+                failure_message="Serverless Job failed",
+                status_message="Serverless Job status is",
+                status_args=["jobRun.state", "jobRun.stateDetails"],
             )
+
         return self.job_id
 
     def on_kill(self) -> None:
         """Cancel the submitted job run."""
         if self.job_id:
             self.log.info("Stopping job run with jobId - %s", self.job_id)
             response = self.hook.conn.cancel_job_run(applicationId=self.application_id, jobRunId=self.job_id)
@@ -1176,16 +1250,16 @@
                     "jobRunId": self.job_id,
                 },
                 parse_response=["jobRun", "state"],
                 desired_state=EmrServerlessHook.JOB_TERMINAL_STATES,
                 failure_states=set(),
                 object_type="job",
                 action="cancelled",
-                countdown=self.waiter_countdown,
-                check_interval_seconds=self.waiter_check_interval_seconds,
+                countdown=self.waiter_delay * self.waiter_max_attempts,
+                check_interval_seconds=self.waiter_delay,
             )
 
 
 class EmrServerlessStopApplicationOperator(BaseOperator):
     """
     Operator to stop an EMR Serverless application.
 
@@ -1209,24 +1283,47 @@
     template_fields: Sequence[str] = ("application_id",)
 
     def __init__(
         self,
         application_id: str,
         wait_for_completion: bool = True,
         aws_conn_id: str = "aws_default",
-        waiter_countdown: int = 5 * 60,
-        waiter_check_interval_seconds: int = 30,
+        waiter_countdown: int | ArgNotSet = NOTSET,
+        waiter_check_interval_seconds: int | ArgNotSet = NOTSET,
+        waiter_max_attempts: int | ArgNotSet = NOTSET,
+        waiter_delay: int | ArgNotSet = NOTSET,
         force_stop: bool = False,
         **kwargs,
     ):
+        if waiter_check_interval_seconds is NOTSET:
+            waiter_delay = 60 if waiter_delay is NOTSET else waiter_delay
+        else:
+            waiter_delay = waiter_check_interval_seconds if waiter_delay is NOTSET else waiter_delay
+            warnings.warn(
+                "The parameter waiter_check_interval_seconds has been deprecated to standardize "
+                "naming conventions.  Please use waiter_delay instead.  In the "
+                "future this will default to None and defer to the waiter's default value."
+            )
+        if waiter_countdown is NOTSET:
+            waiter_max_attempts = 25 if waiter_max_attempts is NOTSET else waiter_max_attempts
+        else:
+            if waiter_max_attempts is NOTSET:
+                # ignoring mypy because it doesn't like ArgNotSet as an operand, but neither variables
+                # are of type ArgNotSet at this point.
+                waiter_max_attempts = waiter_countdown // waiter_delay  # type: ignore[operator]
+            warnings.warn(
+                "The parameter waiter_countdown has been deprecated to standardize "
+                "naming conventions.  Please use waiter_max_attempts instead.  In the "
+                "future this will default to None and defer to the waiter's default value."
+            )
         self.aws_conn_id = aws_conn_id
         self.application_id = application_id
         self.wait_for_completion = wait_for_completion
-        self.waiter_countdown = waiter_countdown
-        self.waiter_check_interval_seconds = waiter_check_interval_seconds
+        self.waiter_max_attempts = int(waiter_max_attempts)  # type: ignore[arg-type]
+        self.waiter_delay = int(waiter_delay)  # type: ignore[arg-type]
         self.force_stop = force_stop
         super().__init__(**kwargs)
 
     @cached_property
     def hook(self) -> EmrServerlessHook:
         """Create and return an EmrServerlessHook."""
         return EmrServerlessHook(aws_conn_id=self.aws_conn_id)
@@ -1234,35 +1331,31 @@
     def execute(self, context: Context) -> None:
         self.log.info("Stopping application: %s", self.application_id)
 
         if self.force_stop:
             self.hook.cancel_running_jobs(
                 self.application_id,
                 waiter_config={
-                    "Delay": self.waiter_check_interval_seconds,
-                    "MaxAttempts": self.waiter_countdown / self.waiter_check_interval_seconds,
+                    "Delay": self.waiter_delay,
+                    "MaxAttempts": self.waiter_max_attempts,
                 },
             )
 
         self.hook.conn.stop_application(applicationId=self.application_id)
 
         if self.wait_for_completion:
-            # This should be replaced with a boto waiter when available.
-            waiter(
-                get_state_callable=self.hook.conn.get_application,
-                get_state_args={
-                    "applicationId": self.application_id,
-                },
-                parse_response=["application", "state"],
-                desired_state=EmrServerlessHook.APPLICATION_FAILURE_STATES,
-                failure_states=set(),
-                object_type="application",
-                action="stopped",
-                countdown=self.waiter_countdown,
-                check_interval_seconds=self.waiter_check_interval_seconds,
+            waiter = self.hook.get_waiter("serverless_app_stopped")
+            wait(
+                waiter=waiter,
+                waiter_max_attempts=self.waiter_max_attempts,
+                waiter_delay=self.waiter_delay,
+                args={"applicationId": self.application_id},
+                failure_message="Error stopping application",
+                status_message="Serverless Application status is",
+                status_args=["application.state", "application.stateDetails"],
             )
             self.log.info("EMR serverless application %s stopped successfully", self.application_id)
 
 
 class EmrServerlessDeleteApplicationOperator(EmrServerlessStopApplicationOperator):
     """
     Operator to delete EMR Serverless application.
@@ -1288,28 +1381,51 @@
     template_fields: Sequence[str] = ("application_id",)
 
     def __init__(
         self,
         application_id: str,
         wait_for_completion: bool = True,
         aws_conn_id: str = "aws_default",
-        waiter_countdown: int = 25 * 60,
-        waiter_check_interval_seconds: int = 60,
+        waiter_countdown: int | ArgNotSet = NOTSET,
+        waiter_check_interval_seconds: int | ArgNotSet = NOTSET,
+        waiter_max_attempts: int | ArgNotSet = NOTSET,
+        waiter_delay: int | ArgNotSet = NOTSET,
         force_stop: bool = False,
         **kwargs,
     ):
+        if waiter_check_interval_seconds is NOTSET:
+            waiter_delay = 60 if waiter_delay is NOTSET else waiter_delay
+        else:
+            waiter_delay = waiter_check_interval_seconds if waiter_delay is NOTSET else waiter_delay
+            warnings.warn(
+                "The parameter waiter_check_interval_seconds has been deprecated to standardize "
+                "naming conventions.  Please use waiter_delay instead.  In the "
+                "future this will default to None and defer to the waiter's default value."
+            )
+        if waiter_countdown is NOTSET:
+            waiter_max_attempts = 25 if waiter_max_attempts is NOTSET else waiter_max_attempts
+        else:
+            if waiter_max_attempts is NOTSET:
+                # ignoring mypy because it doesn't like ArgNotSet as an operand, but neither variables
+                # are of type ArgNotSet at this point.
+                waiter_max_attempts = waiter_countdown // waiter_delay  # type: ignore[operator]
+            warnings.warn(
+                "The parameter waiter_countdown has been deprecated to standardize "
+                "naming conventions.  Please use waiter_max_attempts instead.  In the "
+                "future this will default to None and defer to the waiter's default value."
+            )
         self.wait_for_delete_completion = wait_for_completion
         # super stops the app
         super().__init__(
             application_id=application_id,
             # when deleting an app, we always need to wait for it to stop before we can call delete()
             wait_for_completion=True,
             aws_conn_id=aws_conn_id,
-            waiter_countdown=waiter_countdown,
-            waiter_check_interval_seconds=waiter_check_interval_seconds,
+            waiter_delay=waiter_delay,
+            waiter_max_attempts=waiter_max_attempts,
             force_stop=force_stop,
             **kwargs,
         )
 
     def execute(self, context: Context) -> None:
         # super stops the app (or makes sure it's already stopped)
         super().execute(context)
@@ -1317,21 +1433,20 @@
         self.log.info("Now deleting application: %s", self.application_id)
         response = self.hook.conn.delete_application(applicationId=self.application_id)
 
         if response["ResponseMetadata"]["HTTPStatusCode"] != 200:
             raise AirflowException(f"Application deletion failed: {response}")
 
         if self.wait_for_delete_completion:
-            # This should be replaced with a boto waiter when available.
-            waiter(
-                get_state_callable=self.hook.conn.get_application,
-                get_state_args={"applicationId": self.application_id},
-                parse_response=["application", "state"],
-                desired_state={"TERMINATED"},
-                failure_states=EmrServerlessHook.APPLICATION_FAILURE_STATES,
-                object_type="application",
-                action="deleted",
-                countdown=self.waiter_countdown,
-                check_interval_seconds=self.waiter_check_interval_seconds,
+            waiter = self.hook.get_waiter("serverless_app_terminated")
+
+            wait(
+                waiter=waiter,
+                waiter_max_attempts=self.waiter_max_attempts,
+                waiter_delay=self.waiter_delay,
+                args={"applicationId": self.application_id},
+                failure_message="Error terminating application",
+                status_message="Serverless Application status is",
+                status_args=["application.state", "application.stateDetails"],
             )
 
         self.log.info("EMR serverless application deleted")
```

### Comparing `apache-airflow-providers-amazon-8.2.0rc1/airflow/providers/amazon/aws/operators/glacier.py` & `apache-airflow-providers-amazon-8.3.0rc1/airflow/providers/amazon/aws/operators/glacier.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-amazon-8.2.0rc1/airflow/providers/amazon/aws/operators/glue.py` & `apache-airflow-providers-amazon-8.3.0rc1/airflow/providers/amazon/aws/operators/glue.py`

 * *Files 7% similar despite different names*

```diff
@@ -15,17 +15,19 @@
 # KIND, either express or implied.  See the License for the
 # specific language governing permissions and limitations
 # under the License.
 from __future__ import annotations
 
 import os.path
 import urllib.parse
+from functools import cached_property
 from typing import TYPE_CHECKING, Sequence
 
 from airflow import AirflowException
+from airflow.configuration import conf
 from airflow.models import BaseOperator
 from airflow.providers.amazon.aws.hooks.glue import GlueJobHook
 from airflow.providers.amazon.aws.hooks.s3 import S3Hook
 from airflow.providers.amazon.aws.links.glue import GlueJobRunDetailsLink
 from airflow.providers.amazon.aws.triggers.glue import GlueJobCompleteTrigger
 
 if TYPE_CHECKING:
@@ -56,14 +58,15 @@
     :param run_job_kwargs: Extra arguments for Glue Job Run
     :param wait_for_completion: Whether to wait for job run completion. (default: True)
     :param deferrable: If True, the operator will wait asynchronously for the job to complete.
         This implies waiting for completion. This mode requires aiobotocore module to be installed.
         (default: False)
     :param verbose: If True, Glue Job Run logs show in the Airflow Task Logs.  (default: False)
     :param update_config: If True, Operator will update job configuration.  (default: False)
+    :param stop_job_run_on_kill: If True, Operator will stop the job run when task is killed.
     """
 
     template_fields: Sequence[str] = (
         "job_name",
         "script_location",
         "script_args",
         "create_job_kwargs",
@@ -92,17 +95,19 @@
         aws_conn_id: str = "aws_default",
         region_name: str | None = None,
         s3_bucket: str | None = None,
         iam_role_name: str | None = None,
         create_job_kwargs: dict | None = None,
         run_job_kwargs: dict | None = None,
         wait_for_completion: bool = True,
-        deferrable: bool = False,
+        deferrable: bool = conf.getboolean("operators", "default_deferrable", fallback=False),
         verbose: bool = False,
         update_config: bool = False,
+        job_poll_interval: int | float = 6,
+        stop_job_run_on_kill: bool = False,
         **kwargs,
     ):
         super().__init__(**kwargs)
         self.job_name = job_name
         self.job_desc = job_desc
         self.script_location = script_location
         self.concurrent_run_limit = concurrent_run_limit or 1
@@ -117,86 +122,106 @@
         self.s3_artifacts_prefix = "artifacts/glue-scripts/"
         self.create_job_kwargs = create_job_kwargs
         self.run_job_kwargs = run_job_kwargs or {}
         self.wait_for_completion = wait_for_completion
         self.verbose = verbose
         self.update_config = update_config
         self.deferrable = deferrable
+        self.job_poll_interval = job_poll_interval
+        self.stop_job_run_on_kill = stop_job_run_on_kill
+        self._job_run_id: str | None = None
 
-    def execute(self, context: Context):
-        """Execute AWS Glue Job from Airflow.
-
-        :return: the current Glue job ID.
-        """
+    @cached_property
+    def glue_job_hook(self) -> GlueJobHook:
         if self.script_location is None:
             s3_script_location = None
         elif not self.script_location.startswith(self.s3_protocol):
             s3_hook = S3Hook(aws_conn_id=self.aws_conn_id)
             script_name = os.path.basename(self.script_location)
             s3_hook.load_file(
                 self.script_location, self.s3_artifacts_prefix + script_name, bucket_name=self.s3_bucket
             )
             s3_script_location = f"s3://{self.s3_bucket}/{self.s3_artifacts_prefix}{script_name}"
         else:
             s3_script_location = self.script_location
-        glue_job = GlueJobHook(
+        return GlueJobHook(
             job_name=self.job_name,
             desc=self.job_desc,
             concurrent_run_limit=self.concurrent_run_limit,
             script_location=s3_script_location,
             retry_limit=self.retry_limit,
             num_of_dpus=self.num_of_dpus,
             aws_conn_id=self.aws_conn_id,
             region_name=self.region_name,
             s3_bucket=self.s3_bucket,
             iam_role_name=self.iam_role_name,
             create_job_kwargs=self.create_job_kwargs,
             update_config=self.update_config,
+            job_poll_interval=self.job_poll_interval,
         )
+
+    def execute(self, context: Context):
+        """Execute AWS Glue Job from Airflow.
+
+        :return: the current Glue job ID.
+        """
         self.log.info(
             "Initializing AWS Glue Job: %s. Wait for completion: %s",
             self.job_name,
             self.wait_for_completion,
         )
-        glue_job_run = glue_job.initialize_job(self.script_args, self.run_job_kwargs)
+        glue_job_run = self.glue_job_hook.initialize_job(self.script_args, self.run_job_kwargs)
+        self._job_run_id = glue_job_run["JobRunId"]
         glue_job_run_url = GlueJobRunDetailsLink.format_str.format(
-            aws_domain=GlueJobRunDetailsLink.get_aws_domain(glue_job.conn_partition),
-            region_name=glue_job.conn_region_name,
+            aws_domain=GlueJobRunDetailsLink.get_aws_domain(self.glue_job_hook.conn_partition),
+            region_name=self.glue_job_hook.conn_region_name,
             job_name=urllib.parse.quote(self.job_name, safe=""),
-            job_run_id=glue_job_run["JobRunId"],
+            job_run_id=self._job_run_id,
         )
         GlueJobRunDetailsLink.persist(
             context=context,
             operator=self,
-            region_name=glue_job.conn_region_name,
-            aws_partition=glue_job.conn_partition,
+            region_name=self.glue_job_hook.conn_region_name,
+            aws_partition=self.glue_job_hook.conn_partition,
             job_name=urllib.parse.quote(self.job_name, safe=""),
-            job_run_id=glue_job_run["JobRunId"],
+            job_run_id=self._job_run_id,
         )
         self.log.info("You can monitor this Glue Job run at: %s", glue_job_run_url)
 
         if self.deferrable:
             self.defer(
                 trigger=GlueJobCompleteTrigger(
                     job_name=self.job_name,
-                    run_id=glue_job_run["JobRunId"],
+                    run_id=self._job_run_id,
                     verbose=self.verbose,
                     aws_conn_id=self.aws_conn_id,
+                    job_poll_interval=self.job_poll_interval,
                 ),
                 method_name="execute_complete",
             )
         elif self.wait_for_completion:
-            glue_job_run = glue_job.job_completion(self.job_name, glue_job_run["JobRunId"], self.verbose)
+            glue_job_run = self.glue_job_hook.job_completion(self.job_name, self._job_run_id, self.verbose)
             self.log.info(
                 "AWS Glue Job: %s status: %s. Run Id: %s",
                 self.job_name,
                 glue_job_run["JobRunState"],
-                glue_job_run["JobRunId"],
+                self._job_run_id,
             )
         else:
-            self.log.info("AWS Glue Job: %s. Run Id: %s", self.job_name, glue_job_run["JobRunId"])
-        return glue_job_run["JobRunId"]
+            self.log.info("AWS Glue Job: %s. Run Id: %s", self.job_name, self._job_run_id)
+        return self._job_run_id
 
     def execute_complete(self, context, event=None):
         if event["status"] != "success":
             raise AirflowException(f"Error in glue job: {event}")
         return event["value"]
+
+    def on_kill(self):
+        """Cancel the running AWS Glue Job."""
+        if self.stop_job_run_on_kill:
+            self.log.info("Stopping AWS Glue Job: %s. Run Id: %s", self.job_name, self._job_run_id)
+            response = self.glue_job_hook.conn.batch_stop_job_run(
+                JobName=self.job_name,
+                JobRunIds=[self._job_run_id],
+            )
+            if not response["SuccessfulSubmissions"]:
+                self.log.error("Failed to stop AWS Glue Job: %s. Run Id: %s", self.job_name, self._job_run_id)
```

### Comparing `apache-airflow-providers-amazon-8.2.0rc1/airflow/providers/amazon/aws/operators/glue_crawler.py` & `apache-airflow-providers-amazon-8.3.0rc1/airflow/providers/amazon/aws/operators/glue_crawler.py`

 * *Files 3% similar despite different names*

```diff
@@ -17,28 +17,31 @@
 # under the License.
 from __future__ import annotations
 
 from functools import cached_property
 from typing import TYPE_CHECKING, Sequence
 
 from airflow import AirflowException
+from airflow.configuration import conf
 from airflow.providers.amazon.aws.triggers.glue_crawler import GlueCrawlerCompleteTrigger
 
 if TYPE_CHECKING:
     from airflow.utils.context import Context
 
 from airflow.models import BaseOperator
 from airflow.providers.amazon.aws.hooks.glue_crawler import GlueCrawlerHook
 
 
 class GlueCrawlerOperator(BaseOperator):
     """
-    Creates, updates and triggers an AWS Glue Crawler. AWS Glue Crawler is a serverless
-    service that manages a catalog of metadata tables that contain the inferred
-    schema, format and data types of data stores within the AWS cloud.
+    Creates, updates and triggers an AWS Glue Crawler.
+
+    AWS Glue Crawler is a serverless service that manages a catalog of
+    metadata tables that contain the inferred schema, format and data
+    types of data stores within the AWS cloud.
 
     .. seealso::
         For more information on how to use this operator, take a look at the guide:
         :ref:`howto/operator:GlueCrawlerOperator`
 
     :param config: Configurations for the AWS Glue crawler
     :param aws_conn_id: aws connection to use
@@ -55,15 +58,15 @@
     def __init__(
         self,
         config,
         aws_conn_id="aws_default",
         region_name: str | None = None,
         poll_interval: int = 5,
         wait_for_completion: bool = True,
-        deferrable: bool = False,
+        deferrable: bool = conf.getboolean("operators", "default_deferrable", fallback=False),
         **kwargs,
     ):
         super().__init__(**kwargs)
         self.aws_conn_id = aws_conn_id
         self.poll_interval = poll_interval
         self.wait_for_completion = wait_for_completion
         self.deferrable = deferrable
```

### Comparing `apache-airflow-providers-amazon-8.2.0rc1/airflow/providers/amazon/aws/operators/lambda_function.py` & `apache-airflow-providers-amazon-8.3.0rc1/airflow/providers/amazon/aws/operators/lambda_function.py`

 * *Files 0% similar despite different names*

```diff
@@ -116,16 +116,17 @@
             )
 
         return response.get("FunctionArn")
 
 
 class LambdaInvokeFunctionOperator(BaseOperator):
     """
-    Invokes an AWS Lambda function. You can invoke a function synchronously (and wait for the response),
-    or asynchronously.
+    Invokes an AWS Lambda function.
+
+    You can invoke a function synchronously (and wait for the response), or asynchronously.
     To invoke a function asynchronously, set `invocation_type` to `Event`. For more details,
     review the boto3 Lambda invoke docs.
 
     .. seealso::
         For more information on how to use this operator, take a look at the guide:
         :ref:`howto/operator:LambdaInvokeFunctionOperator`
 
@@ -145,15 +146,15 @@
         self,
         *,
         function_name: str,
         log_type: str | None = None,
         qualifier: str | None = None,
         invocation_type: str | None = None,
         client_context: str | None = None,
-        payload: str | None = None,
+        payload: bytes | str | None = None,
         aws_conn_id: str = "aws_default",
         **kwargs,
     ):
         super().__init__(**kwargs)
         self.function_name = function_name
         self.payload = payload
         self.log_type = log_type
```

### Comparing `apache-airflow-providers-amazon-8.2.0rc1/airflow/providers/amazon/aws/operators/quicksight.py` & `apache-airflow-providers-amazon-8.3.0rc1/airflow/providers/amazon/aws/operators/quicksight.py`

 * *Files 2% similar despite different names*

```diff
@@ -25,16 +25,15 @@
     from airflow.utils.context import Context
 
 DEFAULT_CONN_ID = "aws_default"
 
 
 class QuickSightCreateIngestionOperator(BaseOperator):
     """
-    Creates and starts a new SPICE ingestion for a dataset.
-    Also, helps to Refresh existing SPICE datasets.
+    Creates and starts a new SPICE ingestion for a dataset;  also helps to Refresh existing SPICE datasets.
 
     .. seealso::
         For more information on how to use this operator, take a look at the guide:
         :ref:`howto/operator:QuickSightCreateIngestionOperator`
 
     :param data_set_id:  ID of the dataset used in the ingestion.
     :param ingestion_id: ID for the ingestion.
```

### Comparing `apache-airflow-providers-amazon-8.2.0rc1/airflow/providers/amazon/aws/operators/rds.py` & `apache-airflow-providers-amazon-8.3.0rc1/airflow/providers/amazon/aws/operators/rds.py`

 * *Files 17% similar despite different names*

```diff
@@ -14,36 +14,51 @@
 # "AS IS" BASIS, WITHOUT WARRANTIES OR CONDITIONS OF ANY
 # KIND, either express or implied.  See the License for the
 # specific language governing permissions and limitations
 # under the License.
 from __future__ import annotations
 
 import json
+import warnings
+from datetime import timedelta
 from typing import TYPE_CHECKING, Sequence
 
 from mypy_boto3_rds.type_defs import TagTypeDef
 
+from airflow.configuration import conf
+from airflow.exceptions import AirflowException, AirflowProviderDeprecationWarning
 from airflow.models import BaseOperator
 from airflow.providers.amazon.aws.hooks.rds import RdsHook
+from airflow.providers.amazon.aws.triggers.rds import RdsDbInstanceTrigger
 from airflow.providers.amazon.aws.utils.rds import RdsDbType
 from airflow.providers.amazon.aws.utils.tags import format_tags
+from airflow.providers.amazon.aws.utils.waiter_with_logging import wait
 
 if TYPE_CHECKING:
     from airflow.utils.context import Context
 
 
 class RdsBaseOperator(BaseOperator):
     """Base operator that implements common functions for all operators."""
 
     ui_color = "#eeaa88"
     ui_fgcolor = "#ffffff"
 
     def __init__(self, *args, aws_conn_id: str = "aws_conn_id", hook_params: dict | None = None, **kwargs):
-        hook_params = hook_params or {}
-        self.hook = RdsHook(aws_conn_id=aws_conn_id, **hook_params)
+        if hook_params is not None:
+            warnings.warn(
+                "The parameter hook_params is deprecated and will be removed. "
+                "If you were using it, please get in touch either on airflow slack, "
+                "or by opening a github issue on the project. "
+                "You can mention https://github.com/apache/airflow/pull/32352",
+                AirflowProviderDeprecationWarning,
+                stacklevel=3,  # 2 is in the operator's init, 3 is in the user code creating the operator
+            )
+        self.hook_params = hook_params or {}
+        self.hook = RdsHook(aws_conn_id=aws_conn_id, **self.hook_params)
         super().__init__(*args, **kwargs)
 
         self._await_interval = 60  # seconds
 
     def execute(self, context: Context) -> str:
         """Different implementations for snapshots, tasks and events."""
         raise NotImplementedError
@@ -52,14 +67,15 @@
         """Different implementations for snapshots, tasks and events."""
         raise NotImplementedError
 
 
 class RdsCreateDbSnapshotOperator(RdsBaseOperator):
     """
     Creates a snapshot of a DB instance or DB cluster.
+
     The source DB instance or cluster must be in the available or storage-optimization state.
 
     .. seealso::
         For more information on how to use this operator, take a look at the guide:
         :ref:`howto/operator:RdsCreateDbSnapshotOperator`
 
     :param db_type: Type of the DB - either "instance" or "cluster"
@@ -517,95 +533,179 @@
         contain from 1 to 63 letters, numbers, or hyphens
     :param db_instance_class: The compute and memory capacity of the DB instance, for example db.m5.large
     :param engine: The name of the database engine to be used for this instance
     :param rds_kwargs: Named arguments to pass to boto3 RDS client function ``create_db_instance``
         https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/rds.html#RDS.Client.create_db_instance
     :param aws_conn_id: The Airflow connection used for AWS credentials.
     :param wait_for_completion:  If True, waits for creation of the DB instance to complete. (default: True)
+    :param waiter_delay: Time (in seconds) to wait between two consecutive calls to check DB instance state
+    :param waiter_max_attempts: The maximum number of attempts to check DB instance state
+    :param deferrable: If True, the operator will wait asynchronously for the DB instance to be created.
+        This implies waiting for completion. This mode requires aiobotocore module to be installed.
+        (default: False)
     """
 
     template_fields = ("db_instance_identifier", "db_instance_class", "engine", "rds_kwargs")
 
     def __init__(
         self,
         *,
         db_instance_identifier: str,
         db_instance_class: str,
         engine: str,
         rds_kwargs: dict | None = None,
         aws_conn_id: str = "aws_default",
         wait_for_completion: bool = True,
+        deferrable: bool = conf.getboolean("operators", "default_deferrable", fallback=False),
+        waiter_delay: int = 30,
+        waiter_max_attempts: int = 60,
         **kwargs,
     ):
         super().__init__(aws_conn_id=aws_conn_id, **kwargs)
 
         self.db_instance_identifier = db_instance_identifier
         self.db_instance_class = db_instance_class
         self.engine = engine
         self.rds_kwargs = rds_kwargs or {}
-        self.wait_for_completion = wait_for_completion
+        self.wait_for_completion = False if deferrable else wait_for_completion
+        self.deferrable = deferrable
+        self.waiter_delay = waiter_delay
+        self.waiter_max_attempts = waiter_max_attempts
+        self.aws_conn_id = aws_conn_id
 
     def execute(self, context: Context) -> str:
         self.log.info("Creating new DB instance %s", self.db_instance_identifier)
 
         create_db_instance = self.hook.conn.create_db_instance(
             DBInstanceIdentifier=self.db_instance_identifier,
             DBInstanceClass=self.db_instance_class,
             Engine=self.engine,
             **self.rds_kwargs,
         )
+        if self.deferrable:
+            self.defer(
+                trigger=RdsDbInstanceTrigger(
+                    db_instance_identifier=self.db_instance_identifier,
+                    waiter_delay=self.waiter_delay,
+                    waiter_max_attempts=self.waiter_max_attempts,
+                    aws_conn_id=self.aws_conn_id,
+                    hook_params=self.hook_params,
+                    waiter_name="db_instance_available",
+                    # ignoring type because create_db_instance is a dict
+                    response=create_db_instance,  # type: ignore[arg-type]
+                ),
+                method_name="execute_complete",
+                timeout=timedelta(seconds=self.waiter_delay * self.waiter_max_attempts),
+            )
 
         if self.wait_for_completion:
-            self.hook.wait_for_db_instance_state(self.db_instance_identifier, target_state="available")
+            waiter = self.hook.conn.get_waiter("db_instance_available")
+            wait(
+                waiter=waiter,
+                waiter_delay=self.waiter_delay,
+                waiter_max_attempts=self.waiter_max_attempts,
+                args={"DBInstanceIdentifier": self.db_instance_identifier},
+                failure_message="DB instance creation failed",
+                status_message="DB Instance status is",
+                status_args=["DBInstances[0].DBInstanceStatus"],
+            )
         return json.dumps(create_db_instance, default=str)
 
+    def execute_complete(self, context, event=None) -> str:
+        if event["status"] != "success":
+            raise AirflowException(f"DB instance creation failed: {event}")
+        else:
+            return json.dumps(event["response"], default=str)
+
 
 class RdsDeleteDbInstanceOperator(RdsBaseOperator):
     """
     Deletes an RDS DB Instance.
 
     .. seealso::
         For more information on how to use this operator, take a look at the guide:
         :ref:`howto/operator:RdsDeleteDbInstanceOperator`
 
     :param db_instance_identifier: The DB instance identifier for the DB instance to be deleted
     :param rds_kwargs: Named arguments to pass to boto3 RDS client function ``delete_db_instance``
         https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/rds.html#RDS.Client.delete_db_instance
     :param aws_conn_id: The Airflow connection used for AWS credentials.
     :param wait_for_completion:  If True, waits for deletion of the DB instance to complete. (default: True)
+    :param waiter_delay: Time (in seconds) to wait between two consecutive calls to check DB instance state
+    :param waiter_max_attempts: The maximum number of attempts to check DB instance state
+    :param deferrable: If True, the operator will wait asynchronously for the DB instance to be created.
+        This implies waiting for completion. This mode requires aiobotocore module to be installed.
+        (default: False)
     """
 
     template_fields = ("db_instance_identifier", "rds_kwargs")
 
     def __init__(
         self,
         *,
         db_instance_identifier: str,
         rds_kwargs: dict | None = None,
         aws_conn_id: str = "aws_default",
         wait_for_completion: bool = True,
+        deferrable: bool = conf.getboolean("operators", "default_deferrable", fallback=False),
+        waiter_delay: int = 30,
+        waiter_max_attempts: int = 60,
         **kwargs,
     ):
         super().__init__(aws_conn_id=aws_conn_id, **kwargs)
         self.db_instance_identifier = db_instance_identifier
         self.rds_kwargs = rds_kwargs or {}
-        self.wait_for_completion = wait_for_completion
+        self.wait_for_completion = False if deferrable else wait_for_completion
+        self.deferrable = deferrable
+        self.waiter_delay = waiter_delay
+        self.waiter_max_attempts = waiter_max_attempts
+        self.aws_conn_id = aws_conn_id
 
     def execute(self, context: Context) -> str:
         self.log.info("Deleting DB instance %s", self.db_instance_identifier)
 
         delete_db_instance = self.hook.conn.delete_db_instance(
             DBInstanceIdentifier=self.db_instance_identifier,
             **self.rds_kwargs,
         )
+        if self.deferrable:
+            self.defer(
+                trigger=RdsDbInstanceTrigger(
+                    db_instance_identifier=self.db_instance_identifier,
+                    waiter_delay=self.waiter_delay,
+                    waiter_max_attempts=self.waiter_max_attempts,
+                    aws_conn_id=self.aws_conn_id,
+                    hook_params=self.hook_params,
+                    waiter_name="db_instance_deleted",
+                    # ignoring type because delete_db_instance is a dict
+                    response=delete_db_instance,  # type: ignore[arg-type]
+                ),
+                method_name="execute_complete",
+                timeout=timedelta(seconds=self.waiter_delay * self.waiter_max_attempts),
+            )
 
         if self.wait_for_completion:
-            self.hook.wait_for_db_instance_state(self.db_instance_identifier, target_state="deleted")
+            waiter = self.hook.conn.get_waiter("db_instance_deleted")
+            wait(
+                waiter=waiter,
+                waiter_delay=self.waiter_delay,
+                waiter_max_attempts=self.waiter_max_attempts,
+                args={"DBInstanceIdentifier": self.db_instance_identifier},
+                failure_message="DB instance deletion failed",
+                status_message="DB Instance status is",
+                status_args=["DBInstances[0].DBInstanceStatus"],
+            )
         return json.dumps(delete_db_instance, default=str)
 
+    def execute_complete(self, context, event=None) -> str:
+        if event["status"] != "success":
+            raise AirflowException(f"DB instance deletion failed: {event}")
+        else:
+            return json.dumps(event["response"], default=str)
+
 
 class RdsStartDbOperator(RdsBaseOperator):
     """
     Starts an RDS DB instance / cluster.
 
     .. seealso::
         For more information on how to use this operator, take a look at the guide:
```

### Comparing `apache-airflow-providers-amazon-8.2.0rc1/airflow/providers/amazon/aws/operators/redshift_cluster.py` & `apache-airflow-providers-amazon-8.3.0rc1/airflow/providers/amazon/aws/operators/redshift_cluster.py`

 * *Files 2% similar despite different names*

```diff
@@ -16,14 +16,15 @@
 # under the License.
 from __future__ import annotations
 
 import time
 from datetime import timedelta
 from typing import TYPE_CHECKING, Any, Sequence
 
+from airflow.configuration import conf
 from airflow.exceptions import AirflowException
 from airflow.models import BaseOperator
 from airflow.providers.amazon.aws.hooks.redshift_cluster import RedshiftHook
 from airflow.providers.amazon.aws.triggers.redshift_cluster import (
     RedshiftCreateClusterSnapshotTrigger,
     RedshiftCreateClusterTrigger,
     RedshiftDeleteClusterTrigger,
@@ -144,15 +145,15 @@
         availability_zone_relocation: bool | None = None,
         aqua_configuration_status: str | None = None,
         default_iam_role_arn: str | None = None,
         aws_conn_id: str = "aws_default",
         wait_for_completion: bool = False,
         max_attempt: int = 5,
         poll_interval: int = 60,
-        deferrable: bool = False,
+        deferrable: bool = conf.getboolean("operators", "default_deferrable", fallback=False),
         **kwargs,
     ):
         super().__init__(**kwargs)
         self.cluster_identifier = cluster_identifier
         self.node_type = node_type
         self.master_username = master_username
         self.master_user_password = master_user_password
@@ -323,15 +324,15 @@
         cluster_identifier: str,
         retention_period: int = -1,
         tags: list[Any] | None = None,
         wait_for_completion: bool = False,
         poll_interval: int = 15,
         max_attempt: int = 20,
         aws_conn_id: str = "aws_default",
-        deferrable: bool = False,
+        deferrable: bool = conf.getboolean("operators", "default_deferrable", fallback=False),
         **kwargs,
     ):
         super().__init__(**kwargs)
         self.snapshot_identifier = snapshot_identifier
         self.cluster_identifier = cluster_identifier
         self.retention_period = retention_period
         self.tags = tags
@@ -466,15 +467,15 @@
 
     def __init__(
         self,
         *,
         cluster_identifier: str,
         aws_conn_id: str = "aws_default",
         wait_for_completion: bool = False,
-        deferrable: bool = False,
+        deferrable: bool = conf.getboolean("operators", "default_deferrable", fallback=False),
         poll_interval: int = 10,
         max_attempts: int = 10,
         **kwargs,
     ):
         super().__init__(**kwargs)
         self.cluster_identifier = cluster_identifier
         self.aws_conn_id = aws_conn_id
@@ -556,15 +557,15 @@
     ui_fgcolor = "#ffffff"
 
     def __init__(
         self,
         *,
         cluster_identifier: str,
         aws_conn_id: str = "aws_default",
-        deferrable: bool = False,
+        deferrable: bool = conf.getboolean("operators", "default_deferrable", fallback=False),
         poll_interval: int = 10,
         max_attempts: int = 15,
         **kwargs,
     ):
         super().__init__(**kwargs)
         self.cluster_identifier = cluster_identifier
         self.aws_conn_id = aws_conn_id
@@ -643,15 +644,15 @@
         *,
         cluster_identifier: str,
         skip_final_cluster_snapshot: bool = True,
         final_cluster_snapshot_identifier: str | None = None,
         wait_for_completion: bool = True,
         aws_conn_id: str = "aws_default",
         poll_interval: int = 30,
-        deferrable: bool = False,
+        deferrable: bool = conf.getboolean("operators", "default_deferrable", fallback=False),
         max_attempts: int = 30,
         **kwargs,
     ):
         super().__init__(**kwargs)
         self.cluster_identifier = cluster_identifier
         self.skip_final_cluster_snapshot = skip_final_cluster_snapshot
         self.final_cluster_snapshot_identifier = final_cluster_snapshot_identifier
@@ -664,15 +665,14 @@
         self._attempt_interval = 15
         self.redshift_hook = RedshiftHook(aws_conn_id=aws_conn_id)
         self.aws_conn_id = aws_conn_id
         self.deferrable = deferrable
         self.max_attempts = max_attempts
 
     def execute(self, context: Context):
-
         while self._attempts >= 1:
             try:
                 self.redshift_hook.delete_cluster(
                     cluster_identifier=self.cluster_identifier,
                     skip_final_cluster_snapshot=self.skip_final_cluster_snapshot,
                     final_cluster_snapshot_identifier=self.final_cluster_snapshot_identifier,
                 )
```

### Comparing `apache-airflow-providers-amazon-8.2.0rc1/airflow/providers/amazon/aws/operators/redshift_data.py` & `apache-airflow-providers-amazon-8.3.0rc1/airflow/providers/amazon/aws/operators/redshift_data.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-amazon-8.2.0rc1/airflow/providers/amazon/aws/operators/s3.py` & `apache-airflow-providers-amazon-8.3.0rc1/airflow/providers/amazon/aws/operators/s3.py`

 * *Files 0% similar despite different names*

```diff
@@ -408,16 +408,15 @@
             )
         else:
             s3_hook.load_bytes(self.data, s3_key, s3_bucket, self.replace, self.encrypt, self.acl_policy)
 
 
 class S3DeleteObjectsOperator(BaseOperator):
     """
-    To enable users to delete single object or multiple objects from
-    a bucket using a single HTTP request.
+    To enable users to delete single object or multiple objects from a bucket using a single HTTP request.
 
     .. seealso::
         For more information on how to use this operator, take a look at the guide:
         :ref:`howto/operator:S3DeleteObjectsOperator`
 
     :param bucket: Name of the bucket in which you are going to delete object(s). (templated)
     :param keys: The key(s) to delete from S3 bucket. (templated)
@@ -478,18 +477,18 @@
         keys = self.keys or s3_hook.list_keys(bucket_name=self.bucket, prefix=self.prefix)
         if keys:
             s3_hook.delete_objects(bucket=self.bucket, keys=keys)
 
 
 class S3FileTransformOperator(BaseOperator):
     """
-    Copies data from a source S3 location to a temporary location on the
-    local filesystem. Runs a transformation on this file as specified by
-    the transformation script and uploads the output to a destination S3
-    location.
+    Copies data from a source S3 location to a temporary location on the local filesystem.
+
+    Runs a transformation on this file as specified by the transformation
+    script and uploads the output to a destination S3 location.
 
     The locations of the source and the destination files in the local
     filesystem is provided as a first and second arguments to the
     transformation script. The transformation script is expected to read the
     data from source, transform it and write the output to the local
     destination file. The operator then takes over control and uploads the
     local destination file to S3.
```

### Comparing `apache-airflow-providers-amazon-8.2.0rc1/airflow/providers/amazon/aws/operators/sagemaker.py` & `apache-airflow-providers-amazon-8.3.0rc1/airflow/providers/amazon/aws/operators/sagemaker.py`

 * *Files 2% similar despite different names*

```diff
@@ -12,22 +12,24 @@
 # software distributed under the License is distributed on an
 # "AS IS" BASIS, WITHOUT WARRANTIES OR CONDITIONS OF ANY
 # KIND, either express or implied.  See the License for the
 # specific language governing permissions and limitations
 # under the License.
 from __future__ import annotations
 
+import datetime
 import json
 import time
 import warnings
 from functools import cached_property
 from typing import TYPE_CHECKING, Any, Callable, Sequence
 
 from botocore.exceptions import ClientError
 
+from airflow.configuration import conf
 from airflow.exceptions import AirflowException, AirflowProviderDeprecationWarning
 from airflow.models import BaseOperator
 from airflow.providers.amazon.aws.hooks.base_aws import AwsBaseHook
 from airflow.providers.amazon.aws.hooks.sagemaker import SageMakerHook
 from airflow.providers.amazon.aws.triggers.sagemaker import SageMakerTrigger
 from airflow.providers.amazon.aws.utils import trim_none_values
 from airflow.providers.amazon.aws.utils.sagemaker import ApprovalStatus
@@ -101,14 +103,15 @@
             "After preprocessing the config is:\n %s",
             json.dumps(self.config, sort_keys=True, indent=4, separators=(",", ": ")),
         )
 
     def _create_integer_fields(self) -> None:
         """
         Set fields which should be cast to integers.
+
         Child classes should override this method if they need integer fields parsed.
         """
         self.integer_fields = []
 
     def _get_unique_job_name(
         self, proposed_name: str, fail_if_exists: bool, describe_func: Callable[[str], Any]
     ) -> str:
@@ -151,18 +154,19 @@
     def hook(self):
         """Return SageMakerHook."""
         return SageMakerHook(aws_conn_id=self.aws_conn_id)
 
 
 class SageMakerProcessingOperator(SageMakerBaseOperator):
     """
-    Use Amazon SageMaker Processing to analyze data and evaluate machine learning
-    models on Amazon SageMake. With Processing, you can use a simplified, managed
-    experience on SageMaker to run your data processing workloads, such as feature
-    engineering, data validation, model evaluation, and model interpretation.
+    Use Amazon SageMaker Processing to analyze data and evaluate machine learning models on Amazon SageMaker.
+
+    With Processing, you can use a simplified, managed experience on SageMaker
+    to run your data processing workloads, such as feature engineering, data
+    validation, model evaluation, and model interpretation.
 
      .. seealso::
         For more information on how to use this operator, take a look at the guide:
         :ref:`howto/operator:SageMakerProcessingOperator`
 
     :param config: The configuration necessary to start a processing job (templated).
         For details of the configuration parameter see :py:meth:`SageMaker.Client.create_processing_job`
@@ -191,15 +195,15 @@
         aws_conn_id: str = DEFAULT_CONN_ID,
         wait_for_completion: bool = True,
         print_log: bool = True,
         check_interval: int = CHECK_INTERVAL_SECOND,
         max_attempts: int | None = None,
         max_ingestion_time: int | None = None,
         action_if_job_exists: str = "timestamp",
-        deferrable: bool = False,
+        deferrable: bool = conf.getboolean("operators", "default_deferrable", fallback=False),
         **kwargs,
     ):
         super().__init__(config=config, aws_conn_id=aws_conn_id, **kwargs)
         if action_if_job_exists not in ("increment", "fail", "timestamp"):
             raise AirflowException(
                 f"Argument action_if_job_exists accepts only 'timestamp', 'increment' and 'fail'. \
                 Provided value: '{action_if_job_exists}'."
@@ -283,17 +287,17 @@
         else:
             self.log.info(event["message"])
         return {"Processing": serialize(self.hook.describe_processing_job(self.config["ProcessingJobName"]))}
 
 
 class SageMakerEndpointConfigOperator(SageMakerBaseOperator):
     """
-    Creates an endpoint configuration that Amazon SageMaker hosting
-    services uses to deploy models. In the configuration, you identify
-    one or more models, created using the CreateModel API, to deploy and
+    Creates an endpoint configuration that Amazon SageMaker hosting services uses to deploy models.
+
+    In the configuration, you identify one or more models, created using the CreateModel API, to deploy and
     the resources that you want Amazon SageMaker to provision.
 
     .. seealso::
         For more information on how to use this operator, take a look at the guide:
         :ref:`howto/operator:SageMakerEndpointConfigOperator`
 
     :param config: The configuration necessary to create an endpoint config.
@@ -328,18 +332,19 @@
                     self.hook.describe_endpoint_config(self.config["EndpointConfigName"])
                 )
             }
 
 
 class SageMakerEndpointOperator(SageMakerBaseOperator):
     """
-    When you create a serverless endpoint, SageMaker provisions and manages
-    the compute resources for you. Then, you can make inference requests to
-    the endpoint and receive model predictions in response. SageMaker scales
-    the compute resources up and down as needed to handle your request traffic.
+    When you create a serverless endpoint, SageMaker provisions and manages the compute resources for you.
+
+    Then, you can make inference requests to the endpoint and receive model predictions
+    in response. SageMaker scales the compute resources up and down as needed to handle
+    your request traffic.
 
     Requires an Endpoint Config.
 
     .. seealso::
         For more information on how to use this operator, take a look at the guide:
         :ref:`howto/operator:SageMakerEndpointOperator`
 
@@ -371,35 +376,38 @@
     :param wait_for_completion: Whether the operator should wait until the endpoint creation finishes.
     :param check_interval: If wait is set to True, this is the time interval, in seconds, that this operation
         waits before polling the status of the endpoint creation.
     :param max_ingestion_time: If wait is set to True, this operation fails if the endpoint creation doesn't
         finish within max_ingestion_time seconds. If you set this parameter to None it never times out.
     :param operation: Whether to create an endpoint or update an endpoint. Must be either 'create or 'update'.
     :param aws_conn_id: The AWS connection ID to use.
+    :param deferrable:  Will wait asynchronously for completion.
     :return Dict: Returns The ARN of the endpoint created in Amazon SageMaker.
     """
 
     def __init__(
         self,
         *,
         config: dict,
         aws_conn_id: str = DEFAULT_CONN_ID,
         wait_for_completion: bool = True,
         check_interval: int = CHECK_INTERVAL_SECOND,
         max_ingestion_time: int | None = None,
         operation: str = "create",
+        deferrable: bool = conf.getboolean("operators", "default_deferrable", fallback=False),
         **kwargs,
     ):
         super().__init__(config=config, aws_conn_id=aws_conn_id, **kwargs)
         self.wait_for_completion = wait_for_completion
         self.check_interval = check_interval
-        self.max_ingestion_time = max_ingestion_time
+        self.max_ingestion_time = max_ingestion_time or 3600 * 10
         self.operation = operation.lower()
         if self.operation not in ["create", "update"]:
             raise ValueError('Invalid value! Argument operation has to be one of "create" and "update"')
+        self.deferrable = deferrable
 
     def _create_integer_fields(self) -> None:
         """Set fields which should be cast to integers."""
         if "EndpointConfig" in self.config:
             self.integer_fields: list[list[str]] = [
                 ["EndpointConfig", "ProductionVariants", "InitialInstanceCount"]
             ]
@@ -432,43 +440,70 @@
             log_str = "Updating"
         else:
             raise ValueError('Invalid value! Argument operation has to be one of "create" and "update"')
         self.log.info("%s SageMaker endpoint %s.", log_str, endpoint_info["EndpointName"])
         try:
             response = sagemaker_operation(
                 endpoint_info,
-                wait_for_completion=self.wait_for_completion,
-                check_interval=self.check_interval,
-                max_ingestion_time=self.max_ingestion_time,
+                wait_for_completion=False,
             )
+            # waiting for completion is handled here in the operator
         except ClientError:
             self.operation = "update"
             sagemaker_operation = self.hook.update_endpoint
-            log_str = "Updating"
             response = sagemaker_operation(
                 endpoint_info,
-                wait_for_completion=self.wait_for_completion,
-                check_interval=self.check_interval,
-                max_ingestion_time=self.max_ingestion_time,
+                wait_for_completion=False,
             )
+
         if response["ResponseMetadata"]["HTTPStatusCode"] != 200:
             raise AirflowException(f"Sagemaker endpoint creation failed: {response}")
-        else:
-            return {
-                "EndpointConfig": serialize(
-                    self.hook.describe_endpoint_config(endpoint_info["EndpointConfigName"])
+
+        if self.deferrable:
+            self.defer(
+                trigger=SageMakerTrigger(
+                    job_name=endpoint_info["EndpointName"],
+                    job_type="endpoint",
+                    poke_interval=self.check_interval,
+                    aws_conn_id=self.aws_conn_id,
                 ),
-                "Endpoint": serialize(self.hook.describe_endpoint(endpoint_info["EndpointName"])),
-            }
+                method_name="execute_complete",
+                timeout=datetime.timedelta(seconds=self.max_ingestion_time),
+            )
+        elif self.wait_for_completion:
+            self.hook.get_waiter("endpoint_in_service").wait(
+                EndpointName=endpoint_info["EndpointName"],
+                WaiterConfig={"Delay": self.check_interval, "MaxAttempts": self.max_ingestion_time},
+            )
+
+        return {
+            "EndpointConfig": serialize(
+                self.hook.describe_endpoint_config(endpoint_info["EndpointConfigName"])
+            ),
+            "Endpoint": serialize(self.hook.describe_endpoint(endpoint_info["EndpointName"])),
+        }
+
+    def execute_complete(self, context, event=None):
+        if event["status"] != "success":
+            raise AirflowException(f"Error while running job: {event}")
+        endpoint_info = self.config.get("Endpoint", self.config)
+        return {
+            "EndpointConfig": serialize(
+                self.hook.describe_endpoint_config(endpoint_info["EndpointConfigName"])
+            ),
+            "Endpoint": serialize(self.hook.describe_endpoint(endpoint_info["EndpointName"])),
+        }
 
 
 class SageMakerTransformOperator(SageMakerBaseOperator):
     """
-    Starts a transform job. A transform job uses a trained model to get inferences
-    on a dataset and saves these results to an Amazon S3 location that you specify.
+    Starts a transform job.
+
+    A transform job uses a trained model to get inferences on a dataset
+    and saves these results to an Amazon S3 location that you specify.
 
     .. seealso::
         For more information on how to use this operator, take a look at the guide:
         :ref:`howto/operator:SageMakerTransformOperator`
 
     :param config: The configuration necessary to start a transform job (templated).
 
@@ -513,15 +548,15 @@
         aws_conn_id: str = DEFAULT_CONN_ID,
         wait_for_completion: bool = True,
         check_interval: int = CHECK_INTERVAL_SECOND,
         max_attempts: int | None = None,
         max_ingestion_time: int | None = None,
         check_if_job_exists: bool = True,
         action_if_job_exists: str = "timestamp",
-        deferrable: bool = False,
+        deferrable: bool = conf.getboolean("operators", "default_deferrable", fallback=False),
         **kwargs,
     ):
         super().__init__(config=config, aws_conn_id=aws_conn_id, **kwargs)
         self.wait_for_completion = wait_for_completion
         self.check_interval = check_interval
         self.max_attempts = max_attempts or 60
         self.max_ingestion_time = max_ingestion_time
@@ -627,19 +662,21 @@
             "Model": serialize(self.hook.describe_model(transform_config["ModelName"])),
             "Transform": serialize(self.hook.describe_transform_job(transform_config["TransformJobName"])),
         }
 
 
 class SageMakerTuningOperator(SageMakerBaseOperator):
     """
-    Starts a hyperparameter tuning job. A hyperparameter tuning job finds the
-    best version of a model by running many training jobs on your dataset using
-    the algorithm you choose and values for hyperparameters within ranges that
-    you specify. It then chooses the hyperparameter values that result in a model
-    that performs the best, as measured by an objective metric that you choose.
+    Starts a hyperparameter tuning job.
+
+    A hyperparameter tuning job finds the best version of a model by running
+    many training jobs on your dataset using the algorithm you choose and
+    values for hyperparameters within ranges that you specify. It then chooses
+    the hyperparameter values that result in a model that performs the best,
+    as measured by an objective metric that you choose.
 
     .. seealso::
         For more information on how to use this operator, take a look at the guide:
         :ref:`howto/operator:SageMakerTuningOperator`
 
     :param config: The configuration necessary to start a tuning job (templated).
 
@@ -648,31 +685,34 @@
     :param aws_conn_id: The AWS connection ID to use.
     :param wait_for_completion: Set to True to wait until the tuning job finishes.
     :param check_interval: If wait is set to True, the time interval, in seconds,
         that this operation waits to check the status of the tuning job.
     :param max_ingestion_time: If wait is set to True, the operation fails
         if the tuning job doesn't finish within max_ingestion_time seconds. If you
         set this parameter to None, the operation does not timeout.
+    :param deferrable: Will wait asynchronously for completion.
     :return Dict: Returns The ARN of the tuning job created in Amazon SageMaker.
     """
 
     def __init__(
         self,
         *,
         config: dict,
         aws_conn_id: str = DEFAULT_CONN_ID,
         wait_for_completion: bool = True,
         check_interval: int = CHECK_INTERVAL_SECOND,
         max_ingestion_time: int | None = None,
+        deferrable: bool = conf.getboolean("operators", "default_deferrable", fallback=False),
         **kwargs,
     ):
         super().__init__(config=config, aws_conn_id=aws_conn_id, **kwargs)
         self.wait_for_completion = wait_for_completion
         self.check_interval = check_interval
         self.max_ingestion_time = max_ingestion_time
+        self.deferrable = deferrable
 
     def expand_role(self) -> None:
         """Expands an IAM role name into an ARN."""
         if "TrainingJobDefinition" in self.config:
             config = self.config["TrainingJobDefinition"]
             if "RoleArn" in config:
                 hook = AwsBaseHook(self.aws_conn_id, client_type="iam")
@@ -691,32 +731,64 @@
     def execute(self, context: Context) -> dict:
         self.preprocess_config()
         self.log.info(
             "Creating SageMaker Hyper-Parameter Tuning Job %s", self.config["HyperParameterTuningJobName"]
         )
         response = self.hook.create_tuning_job(
             self.config,
-            wait_for_completion=self.wait_for_completion,
+            wait_for_completion=False,  # we handle this here
             check_interval=self.check_interval,
             max_ingestion_time=self.max_ingestion_time,
         )
         if response["ResponseMetadata"]["HTTPStatusCode"] != 200:
             raise AirflowException(f"Sagemaker Tuning Job creation failed: {response}")
+
+        if self.deferrable:
+            self.defer(
+                trigger=SageMakerTrigger(
+                    job_name=self.config["HyperParameterTuningJobName"],
+                    job_type="tuning",
+                    poke_interval=self.check_interval,
+                    aws_conn_id=self.aws_conn_id,
+                ),
+                method_name="execute_complete",
+                timeout=datetime.timedelta(seconds=self.max_ingestion_time)
+                if self.max_ingestion_time is not None
+                else None,
+            )
+            description = {}  # never executed but makes static checkers happy
+        elif self.wait_for_completion:
+            description = self.hook.check_status(
+                self.config["HyperParameterTuningJobName"],
+                "HyperParameterTuningJobStatus",
+                self.hook.describe_tuning_job,
+                self.check_interval,
+                self.max_ingestion_time,
+            )
         else:
-            return {
-                "Tuning": serialize(self.hook.describe_tuning_job(self.config["HyperParameterTuningJobName"]))
-            }
+            description = self.hook.describe_tuning_job(self.config["HyperParameterTuningJobName"])
+
+        return {"Tuning": serialize(description)}
+
+    def execute_complete(self, context, event=None):
+        if event["status"] != "success":
+            raise AirflowException(f"Error while running job: {event}")
+        return {
+            "Tuning": serialize(self.hook.describe_tuning_job(self.config["HyperParameterTuningJobName"]))
+        }
 
 
 class SageMakerModelOperator(SageMakerBaseOperator):
     """
-    Creates a model in Amazon SageMaker. In the request, you name the model and
-    describe a primary container. For the primary container, you specify the Docker
-    image that contains inference code, artifacts (from prior training), and a custom
-    environment map that the inference code uses when you deploy the model for predictions.
+    Creates a model in Amazon SageMaker.
+
+    In the request, you name the model and describe a primary container. For the
+    primary container, you specify the Docker image that contains inference code,
+    artifacts (from prior training), and a custom environment map that the inference
+    code uses when you deploy the model for predictions.
 
     .. seealso::
         For more information on how to use this operator, take a look at the guide:
         :ref:`howto/operator:SageMakerModelOperator`
 
     :param config: The configuration necessary to create a model.
 
@@ -742,16 +814,18 @@
             raise AirflowException(f"Sagemaker model creation failed: {response}")
         else:
             return {"Model": serialize(self.hook.describe_model(self.config["ModelName"]))}
 
 
 class SageMakerTrainingOperator(SageMakerBaseOperator):
     """
-    Starts a model training job. After training completes, Amazon SageMaker saves
-    the resulting model artifacts to an Amazon S3 location that you specify.
+    Starts a model training job.
+
+    After training completes, Amazon SageMaker saves the resulting
+    model artifacts to an Amazon S3 location that you specify.
 
     .. seealso::
         For more information on how to use this operator, take a look at the guide:
         :ref:`howto/operator:SageMakerTrainingOperator`
 
     :param config: The configuration necessary to start a training job (templated).
 
@@ -785,15 +859,15 @@
         wait_for_completion: bool = True,
         print_log: bool = True,
         check_interval: int = CHECK_INTERVAL_SECOND,
         max_attempts: int | None = None,
         max_ingestion_time: int | None = None,
         check_if_job_exists: bool = True,
         action_if_job_exists: str = "timestamp",
-        deferrable: bool = False,
+        deferrable: bool = conf.getboolean("operators", "default_deferrable", fallback=False),
         **kwargs,
     ):
         super().__init__(config=config, aws_conn_id=aws_conn_id, **kwargs)
         self.wait_for_completion = wait_for_completion
         self.print_log = print_log
         self.check_interval = check_interval
         self.max_attempts = max_attempts or 60
@@ -1024,16 +1098,17 @@
             status,
         )
         return status
 
 
 class SageMakerRegisterModelVersionOperator(SageMakerBaseOperator):
     """
-    Registers an Amazon SageMaker model by creating a model version that specifies the model group to which it
-    belongs. Will create the model group if it does not exist already.
+    Register a SageMaker model by creating a model version that specifies the model group to which it belongs.
+
+    Will create the model group if it does not exist already.
 
     .. seealso::
         For more information on how to use this operator, take a look at the guide:
         :ref:`howto/operator:SageMakerRegisterModelVersionOperator`
 
     :param image_uri: The Amazon EC2 Container Registry (Amazon ECR) path where inference code is stored.
     :param model_url: The Amazon S3 path where the model artifacts (the trained weights of the model), which
@@ -1114,14 +1189,15 @@
                 self.hook.conn.delete_model_package_group(ModelPackageGroupName=self.package_group_name)
             raise
 
 
 class SageMakerAutoMLOperator(SageMakerBaseOperator):
     """
     Creates an auto ML job, learning to predict the given column from the data provided through S3.
+
     The learning output is written to the specified S3 location.
 
     .. seealso::
         For more information on how to use this operator, take a look at the guide:
         :ref:`howto/operator:SageMakerAutoMLOperator`
 
     :param job_name: Name of the job to create, needs to be unique within the account.
```

### Comparing `apache-airflow-providers-amazon-8.2.0rc1/airflow/providers/amazon/aws/operators/sns.py` & `apache-airflow-providers-amazon-8.3.0rc1/airflow/providers/amazon/aws/operators/sns.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-amazon-8.2.0rc1/airflow/providers/amazon/aws/operators/sqs.py` & `apache-airflow-providers-amazon-8.3.0rc1/airflow/providers/amazon/aws/operators/sqs.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-amazon-8.2.0rc1/airflow/providers/amazon/aws/operators/step_function.py` & `apache-airflow-providers-amazon-8.3.0rc1/airflow/providers/amazon/aws/operators/step_function.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-amazon-8.2.0rc1/airflow/providers/amazon/aws/secrets/__init__.py` & `apache-airflow-providers-amazon-8.3.0rc1/airflow/providers/amazon/aws/operators/__init__.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-amazon-8.2.0rc1/airflow/providers/amazon/aws/secrets/secrets_manager.py` & `apache-airflow-providers-amazon-8.3.0rc1/airflow/providers/amazon/aws/secrets/secrets_manager.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-amazon-8.2.0rc1/airflow/providers/amazon/aws/secrets/systems_manager.py` & `apache-airflow-providers-amazon-8.3.0rc1/airflow/providers/amazon/aws/secrets/systems_manager.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-amazon-8.2.0rc1/airflow/providers/amazon/aws/sensors/__init__.py` & `apache-airflow-providers-amazon-8.3.0rc1/airflow/providers/amazon/aws/secrets/__init__.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-amazon-8.2.0rc1/airflow/providers/amazon/aws/sensors/athena.py` & `apache-airflow-providers-amazon-8.3.0rc1/airflow/providers/amazon/aws/sensors/athena.py`

 * *Files 9% similar despite different names*

```diff
@@ -26,16 +26,15 @@
 from airflow.exceptions import AirflowException
 from airflow.providers.amazon.aws.hooks.athena import AthenaHook
 from airflow.sensors.base import BaseSensorOperator
 
 
 class AthenaSensor(BaseSensorOperator):
     """
-    Asks for the state of the Query until it reaches a failure state or success state.
-    If the query fails, the task will fail.
+    Poll the state of the Query until it reaches a terminal state; fails if the query fails.
 
     .. seealso::
         For more information on how to use this sensor, take a look at the guide:
         :ref:`howto/sensor:AthenaSensor`
 
 
     :param query_execution_id: query_execution_id to check the state of
@@ -72,20 +71,20 @@
         super().__init__(**kwargs)
         self.aws_conn_id = aws_conn_id
         self.query_execution_id = query_execution_id
         self.sleep_time = sleep_time
         self.max_retries = max_retries
 
     def poke(self, context: Context) -> bool:
-        state = self.hook.poll_query_status(self.query_execution_id, self.max_retries)
+        state = self.hook.poll_query_status(self.query_execution_id, self.max_retries, self.sleep_time)
 
         if state in self.FAILURE_STATES:
             raise AirflowException("Athena sensor failed")
 
         if state in self.INTERMEDIATE_STATES:
             return False
         return True
 
     @cached_property
     def hook(self) -> AthenaHook:
         """Create and return an AthenaHook."""
-        return AthenaHook(self.aws_conn_id, sleep_time=self.sleep_time)
+        return AthenaHook(self.aws_conn_id)
```

### Comparing `apache-airflow-providers-amazon-8.2.0rc1/airflow/providers/amazon/aws/sensors/batch.py` & `apache-airflow-providers-amazon-8.3.0rc1/airflow/providers/amazon/aws/sensors/batch.py`

 * *Files 4% similar despite different names*

```diff
@@ -18,27 +18,27 @@
 
 from datetime import timedelta
 from functools import cached_property
 from typing import TYPE_CHECKING, Any, Sequence
 
 from deprecated import deprecated
 
+from airflow.configuration import conf
 from airflow.exceptions import AirflowException
 from airflow.providers.amazon.aws.hooks.batch_client import BatchClientHook
 from airflow.providers.amazon.aws.triggers.batch import BatchSensorTrigger
 from airflow.sensors.base import BaseSensorOperator
 
 if TYPE_CHECKING:
     from airflow.utils.context import Context
 
 
 class BatchSensor(BaseSensorOperator):
     """
-    Asks for the state of the Batch Job execution until it reaches a failure state or success state.
-    If the job fails, the task will fail.
+    Poll the state of the Batch Job until it reaches a terminal state; fails if the job fails.
 
     .. seealso::
         For more information on how to use this sensor, take a look at the guide:
         :ref:`howto/sensor:BatchSensor`
 
     :param job_id: Batch job_id to check the state for
     :param aws_conn_id: aws connection to use, defaults to 'aws_default'
@@ -55,15 +55,15 @@
 
     def __init__(
         self,
         *,
         job_id: str,
         aws_conn_id: str = "aws_default",
         region_name: str | None = None,
-        deferrable: bool = False,
+        deferrable: bool = conf.getboolean("operators", "default_deferrable", fallback=False),
         poke_interval: float = 5,
         max_retries: int = 5,
         **kwargs,
     ):
         super().__init__(**kwargs)
         self.job_id = job_id
         self.aws_conn_id = aws_conn_id
@@ -106,16 +106,16 @@
                 ),
                 method_name="execute_complete",
             )
 
     def execute_complete(self, context: Context, event: dict[str, Any]) -> None:
         """
         Callback for when the trigger fires - returns immediately.
-        Relies on trigger to throw an exception, otherwise it assumes execution was
-        successful.
+
+        Relies on trigger to throw an exception, otherwise it assumes execution was successful.
         """
         if "status" in event and event["status"] == "failure":
             raise AirflowException(event["message"])
         self.log.info(event["message"])
 
     @deprecated(reason="use `hook` property instead.")
     def get_hook(self) -> BatchClientHook:
@@ -128,16 +128,15 @@
             aws_conn_id=self.aws_conn_id,
             region_name=self.region_name,
         )
 
 
 class BatchComputeEnvironmentSensor(BaseSensorOperator):
     """
-    Asks for the state of the Batch compute environment until it reaches a failure state or success state.
-    If the environment fails, the task will fail.
+    Poll the state of the Batch environment until it reaches a terminal state; fails if the environment fails.
 
     .. seealso::
         For more information on how to use this sensor, take a look at the guide:
         :ref:`howto/sensor:BatchComputeEnvironmentSensor`
 
     :param compute_environment: Batch compute environment name
 
@@ -189,16 +188,15 @@
         raise AirflowException(
             f"AWS Batch compute environment failed. AWS Batch compute environment status: {status}"
         )
 
 
 class BatchJobQueueSensor(BaseSensorOperator):
     """
-    Asks for the state of the Batch job queue until it reaches a failure state or success state.
-    If the queue fails, the task will fail.
+    Poll the state of the Batch job queue until it reaches a terminal state; fails if the queue fails.
 
     .. seealso::
         For more information on how to use this sensor, take a look at the guide:
         :ref:`howto/sensor:BatchJobQueueSensor`
 
     :param job_queue: Batch job queue name
```

### Comparing `apache-airflow-providers-amazon-8.2.0rc1/airflow/providers/amazon/aws/sensors/cloud_formation.py` & `apache-airflow-providers-amazon-8.3.0rc1/airflow/providers/amazon/aws/sensors/cloud_formation.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-amazon-8.2.0rc1/airflow/providers/amazon/aws/sensors/dms.py` & `apache-airflow-providers-amazon-8.3.0rc1/airflow/providers/amazon/aws/sensors/dms.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-amazon-8.2.0rc1/airflow/providers/amazon/aws/sensors/dynamodb.py` & `apache-airflow-providers-amazon-8.3.0rc1/airflow/providers/amazon/aws/sensors/dynamodb.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-amazon-8.2.0rc1/airflow/providers/amazon/aws/sensors/ec2.py` & `apache-airflow-providers-amazon-8.3.0rc1/airflow/providers/amazon/aws/sensors/ec2.py`

 * *Files 16% similar despite different names*

```diff
@@ -16,27 +16,27 @@
 # specific language governing permissions and limitations
 # under the License.
 from __future__ import annotations
 
 from functools import cached_property
 from typing import TYPE_CHECKING, Any, Sequence
 
+from airflow.configuration import conf
 from airflow.exceptions import AirflowException
 from airflow.providers.amazon.aws.hooks.ec2 import EC2Hook
 from airflow.providers.amazon.aws.triggers.ec2 import EC2StateSensorTrigger
 from airflow.sensors.base import BaseSensorOperator
 
 if TYPE_CHECKING:
     from airflow.utils.context import Context
 
 
 class EC2InstanceStateSensor(BaseSensorOperator):
     """
-    Check the state of the AWS EC2 instance until
-    state of the instance become equal to the target state.
+    Poll the state of the AWS EC2 instance until the instance reaches the target state.
 
     .. seealso::
         For more information on how to use this sensor, take a look at the guide:
         :ref:`howto/sensor:EC2InstanceStateSensor`
 
     :param target_state: target state of instance
     :param instance_id: id of the AWS EC2 instance
@@ -52,15 +52,15 @@
     def __init__(
         self,
         *,
         target_state: str,
         instance_id: str,
         aws_conn_id: str = "aws_default",
         region_name: str | None = None,
-        deferrable: bool = False,
+        deferrable: bool = conf.getboolean("operators", "default_deferrable", fallback=False),
         **kwargs,
     ):
         if target_state not in self.valid_states:
             raise ValueError(f"Invalid target_state: {target_state}")
         super().__init__(**kwargs)
         self.target_state = target_state
         self.instance_id = instance_id
```

### Comparing `apache-airflow-providers-amazon-8.2.0rc1/airflow/providers/amazon/aws/sensors/ecs.py` & `apache-airflow-providers-amazon-8.3.0rc1/airflow/providers/amazon/aws/sensors/ecs.py`

 * *Files 2% similar despite different names*

```diff
@@ -60,16 +60,15 @@
     def client(self) -> boto3.client:
         """Create and return an EcsHook client."""
         return self.hook.conn
 
 
 class EcsClusterStateSensor(EcsBaseSensor):
     """
-    Polls the cluster state until it reaches a terminal state.  Raises an
-    AirflowException with the failure reason if a failed state is reached.
+    Poll the cluster state until it reaches a terminal state; raises AirflowException with the failure reason.
 
     .. seealso::
         For more information on how to use this operator, take a look at the guide:
         :ref:`howto/sensor:EcsClusterStateSensor`
 
     :param cluster_name: The name of your cluster.
     :param target_state: Success state to watch for. (Default: "ACTIVE")
@@ -99,16 +98,15 @@
         _check_failed(cluster_state, self.target_state, self.failure_states)
 
         return cluster_state == self.target_state
 
 
 class EcsTaskDefinitionStateSensor(EcsBaseSensor):
     """
-    Polls the task definition state until it reaches a terminal state.  Raises an
-    AirflowException with the failure reason if a failed state is reached.
+    Poll task definition until it reaches a terminal state; raise AirflowException with the failure reason.
 
     .. seealso::
         For more information on how to use this operator, take a look at the guide:
         :ref:`howto/sensor:EcsTaskDefinitionStateSensor`
 
     :param task_definition: The family for the latest ACTIVE revision, family and
          revision (family:revision ) for a specific revision in the family, or full
@@ -145,16 +143,15 @@
         self.log.info("Task Definition state: %s, waiting for: %s", task_definition_state, self.target_state)
         _check_failed(task_definition_state, self.target_state, [self.failure_states])
         return task_definition_state == self.target_state
 
 
 class EcsTaskStateSensor(EcsBaseSensor):
     """
-    Polls the task state until it reaches a terminal state.  Raises an
-    AirflowException with the failure reason if a failed state is reached.
+    Poll the task state until it reaches a terminal state; raises AirflowException with the failure reason.
 
     .. seealso::
         For more information on how to use this operator, take a look at the guide:
         :ref:`howto/sensor:EcsTaskStateSensor`
 
     :param cluster: The short name or full Amazon Resource Name (ARN) of the cluster that hosts the task.
     :param task: The task ID or full ARN of the task to poll.
```

### Comparing `apache-airflow-providers-amazon-8.2.0rc1/airflow/providers/amazon/aws/sensors/eks.py` & `apache-airflow-providers-amazon-8.3.0rc1/airflow/providers/amazon/aws/sensors/eks.py`

 * *Files 0% similar despite different names*

```diff
@@ -57,14 +57,15 @@
     "Terminal state reached. Current state: {current_state}, Expected state: {target_state}"
 )
 
 
 class EksBaseSensor(BaseSensorOperator):
     """
     Base class to check various EKS states.
+
     Subclasses need to implement get_state and get_terminal_states methods.
 
     :param cluster_name: The name of the Cluster
     :param target_state: Will return successfully when that state is reached.
     :param target_state_type: The enum containing the states,
         will be used to convert the target state if it has to be converted from a string
     :param aws_conn_id: The Airflow connection used for AWS credentials.
```

### Comparing `apache-airflow-providers-amazon-8.2.0rc1/airflow/providers/amazon/aws/sensors/emr.py` & `apache-airflow-providers-amazon-8.3.0rc1/airflow/providers/amazon/aws/sensors/emr.py`

 * *Files 6% similar despite different names*

```diff
@@ -19,18 +19,23 @@
 
 from datetime import timedelta
 from functools import cached_property
 from typing import TYPE_CHECKING, Any, Iterable, Sequence
 
 from deprecated import deprecated
 
+from airflow.configuration import conf
 from airflow.exceptions import AirflowException
 from airflow.providers.amazon.aws.hooks.emr import EmrContainerHook, EmrHook, EmrServerlessHook
 from airflow.providers.amazon.aws.links.emr import EmrClusterLink, EmrLogsLink, get_log_uri
-from airflow.providers.amazon.aws.triggers.emr import EmrContainerSensorTrigger
+from airflow.providers.amazon.aws.triggers.emr import (
+    EmrContainerTrigger,
+    EmrStepSensorTrigger,
+    EmrTerminateJobFlowTrigger,
+)
 from airflow.sensors.base import BaseSensorOperator
 
 if TYPE_CHECKING:
     from airflow.utils.context import Context
 
 
 class EmrBaseSensor(BaseSensorOperator):
@@ -108,16 +113,15 @@
         :return: failure message
         """
         raise NotImplementedError("Please implement failure_message_from_response() in subclass")
 
 
 class EmrServerlessJobSensor(BaseSensorOperator):
     """
-    Asks for the state of the job run until it reaches a failure state or success state.
-    If the job run fails, the task will fail.
+    Poll the state of the job run until it reaches a terminal state; fails if the job run fails.
 
     .. seealso::
         For more information on how to use this sensor, take a look at the guide:
         :ref:`howto/sensor:EmrServerlessJobSensor`
 
     :param application_id: application_id to check the state of
     :param job_run_id: job_run_id to check the state of
@@ -170,16 +174,15 @@
         :return: failure message
         """
         return response["jobRun"]["stateDetails"]
 
 
 class EmrServerlessApplicationSensor(BaseSensorOperator):
     """
-    Asks for the state of the application until it reaches a failure state or success state.
-    If the application fails, the task will fail.
+    Poll the state of the application until it reaches a terminal state; fails if the application fails.
 
     .. seealso::
         For more information on how to use this sensor, take a look at the guide:
         :ref:`howto/sensor:EmrServerlessApplicationSensor`
 
     :param application_id: application_id to check the state of
     :param target_states: a set of states to wait for, defaults to {'CREATED', 'STARTED'}
@@ -226,16 +229,15 @@
         :return: failure message
         """
         return response["application"]["stateDetails"]
 
 
 class EmrContainerSensor(BaseSensorOperator):
     """
-    Asks for the state of the job run until it reaches a failure state or success state.
-    If the job run fails, the task will fail.
+    Poll the state of the job run until it reaches a terminal state; fail if the job run fails.
 
     .. seealso::
         For more information on how to use this sensor, take a look at the guide:
         :ref:`howto/sensor:EmrContainerSensor`
 
     :param job_id: job_id to check the state of
     :param max_retries: Number of times to poll for query state before
@@ -266,15 +268,15 @@
         self,
         *,
         virtual_cluster_id: str,
         job_id: str,
         max_retries: int | None = None,
         aws_conn_id: str = "aws_default",
         poll_interval: int = 10,
-        deferrable: bool = False,
+        deferrable: bool = conf.getboolean("operators", "default_deferrable", fallback=False),
         **kwargs: Any,
     ) -> None:
         super().__init__(**kwargs)
         self.aws_conn_id = aws_conn_id
         self.virtual_cluster_id = virtual_cluster_id
         self.job_id = job_id
         self.poll_interval = poll_interval
@@ -306,15 +308,15 @@
             timeout = (
                 timedelta(seconds=self.max_retries * self.poll_interval + 60)
                 if self.max_retries
                 else self.execution_timeout
             )
             self.defer(
                 timeout=timeout,
-                trigger=EmrContainerSensorTrigger(
+                trigger=EmrContainerTrigger(
                     virtual_cluster_id=self.virtual_cluster_id,
                     job_id=self.job_id,
                     aws_conn_id=self.aws_conn_id,
                     poll_interval=self.poll_interval,
                 ),
                 method_name="execute_complete",
             )
@@ -324,17 +326,15 @@
             raise AirflowException(f"Error while running job: {event}")
         else:
             self.log.info(event["message"])
 
 
 class EmrNotebookExecutionSensor(EmrBaseSensor):
     """
-    Polls the state of the EMR notebook execution until it reaches
-    any of the target states.
-    If a failure state is reached, the sensor throws an error, and fails the task.
+    Poll the EMR notebook until it reaches any of the target states; raise AirflowException on failure.
 
     .. seealso::
         For more information on how to use this sensor, take a look at the guide:
         :ref:`howto/sensor:EmrNotebookExecutionSensor`
 
     :param notebook_execution_id: Unique id of the notebook execution to be poked.
     :target_states: the states the sensor will wait for the execution to reach.
@@ -388,31 +388,32 @@
         """
         cluster_status = response["NotebookExecution"]
         return cluster_status.get("LastStateChangeReason", None)
 
 
 class EmrJobFlowSensor(EmrBaseSensor):
     """
-    Asks for the state of the EMR JobFlow (Cluster) until it reaches
-    any of the target states.
-    If it fails the sensor errors, failing the task.
+    Poll the EMR JobFlow Cluster until it reaches any of the target states; raise AirflowException on failure.
 
     With the default target states, sensor waits cluster to be terminated.
     When target_states is set to ['RUNNING', 'WAITING'] sensor waits
     until job flow to be ready (after 'STARTING' and 'BOOTSTRAPPING' states)
 
     .. seealso::
         For more information on how to use this sensor, take a look at the guide:
         :ref:`howto/sensor:EmrJobFlowSensor`
 
     :param job_flow_id: job_flow_id to check the state of
     :param target_states: the target states, sensor waits until
-        job flow reaches any of these states
+        job flow reaches any of these states. In deferrable mode it would
+        run until reach the terminal state.
     :param failed_states: the failure states, sensor fails when
         job flow reaches any of these states
+    :param max_attempts: Maximum number of tries before failing
+    :param deferrable: Run sensor in the deferrable mode.
     """
 
     template_fields: Sequence[str] = ("job_flow_id", "target_states", "failed_states")
     template_ext: Sequence[str] = ()
     operator_extra_links = (
         EmrClusterLink(),
         EmrLogsLink(),
@@ -420,20 +421,24 @@
 
     def __init__(
         self,
         *,
         job_flow_id: str,
         target_states: Iterable[str] | None = None,
         failed_states: Iterable[str] | None = None,
+        max_attempts: int = 60,
+        deferrable: bool = conf.getboolean("operators", "default_deferrable", fallback=False),
         **kwargs,
     ):
         super().__init__(**kwargs)
         self.job_flow_id = job_flow_id
         self.target_states = target_states or ["TERMINATED"]
         self.failed_states = failed_states or ["TERMINATED_WITH_ERRORS"]
+        self.max_attempts = max_attempts
+        self.deferrable = deferrable
 
     def get_emr_response(self, context: Context) -> dict[str, Any]:
         """
         Make an API call with boto3 and get cluster-level details.
 
         .. seealso::
             https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/emr.html#EMR.Client.describe_cluster
@@ -484,32 +489,54 @@
         if state_change_reason:
             return (
                 f"for code: {state_change_reason.get('Code', 'No code')} "
                 f"with message {state_change_reason.get('Message', 'Unknown')}"
             )
         return None
 
+    def execute(self, context: Context) -> None:
+        if not self.deferrable:
+            super().execute(context=context)
+        elif not self.poke(context):
+            self.defer(
+                timeout=timedelta(seconds=self.poke_interval * self.max_attempts),
+                trigger=EmrTerminateJobFlowTrigger(
+                    job_flow_id=self.job_flow_id,
+                    max_attempts=self.max_attempts,
+                    aws_conn_id=self.aws_conn_id,
+                    poll_interval=int(self.poke_interval),
+                ),
+                method_name="execute_complete",
+            )
+
+    def execute_complete(self, context, event=None):
+        if event["status"] != "success":
+            raise AirflowException(f"Error while running job: {event}")
+        self.log.info("Job completed.")
+
 
 class EmrStepSensor(EmrBaseSensor):
     """
-    Asks for the state of the step until it reaches any of the target states.
-    If it fails the sensor errors, failing the task.
+    Poll the state of the step until it reaches any of the target states; raise AirflowException on failure.
 
     With the default target states, sensor waits step to be completed.
 
     .. seealso::
         For more information on how to use this sensor, take a look at the guide:
         :ref:`howto/sensor:EmrStepSensor`
 
     :param job_flow_id: job_flow_id which contains the step check the state of
     :param step_id: step to check the state of
     :param target_states: the target states, sensor waits until
-        step reaches any of these states
+        step reaches any of these states. In case of deferrable sensor it will
+        for reach to terminal state
     :param failed_states: the failure states, sensor fails when
         step reaches any of these states
+    :param max_attempts: Maximum number of tries before failing
+    :param deferrable: Run sensor in the deferrable mode.
     """
 
     template_fields: Sequence[str] = ("job_flow_id", "step_id", "target_states", "failed_states")
     template_ext: Sequence[str] = ()
     operator_extra_links = (
         EmrClusterLink(),
         EmrLogsLink(),
@@ -518,21 +545,25 @@
     def __init__(
         self,
         *,
         job_flow_id: str,
         step_id: str,
         target_states: Iterable[str] | None = None,
         failed_states: Iterable[str] | None = None,
+        max_attempts: int = 60,
+        deferrable: bool = conf.getboolean("operators", "default_deferrable", fallback=False),
         **kwargs,
     ):
         super().__init__(**kwargs)
         self.job_flow_id = job_flow_id
         self.step_id = step_id
         self.target_states = target_states or ["COMPLETED"]
         self.failed_states = failed_states or ["CANCELLED", "FAILED", "INTERRUPTED"]
+        self.max_attempts = max_attempts
+        self.deferrable = deferrable
 
     def get_emr_response(self, context: Context) -> dict[str, Any]:
         """
         Make an API call with boto3 and get details about the cluster step.
 
         .. seealso::
             https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/emr.html#EMR.Client.describe_step
@@ -583,7 +614,29 @@
         fail_details = response["Step"]["Status"].get("FailureDetails")
         if fail_details:
             return (
                 f"for reason {fail_details.get('Reason')} "
                 f"with message {fail_details.get('Message')} and log file {fail_details.get('LogFile')}"
             )
         return None
+
+    def execute(self, context: Context) -> None:
+        if not self.deferrable:
+            super().execute(context=context)
+        elif not self.poke(context):
+            self.defer(
+                timeout=timedelta(seconds=self.max_attempts * self.poke_interval),
+                trigger=EmrStepSensorTrigger(
+                    job_flow_id=self.job_flow_id,
+                    step_id=self.step_id,
+                    aws_conn_id=self.aws_conn_id,
+                    max_attempts=self.max_attempts,
+                    poke_interval=int(self.poke_interval),
+                ),
+                method_name="execute_complete",
+            )
+
+    def execute_complete(self, context, event=None):
+        if event["status"] != "success":
+            raise AirflowException(f"Error while running job: {event}")
+
+        self.log.info("Job completed.")
```

### Comparing `apache-airflow-providers-amazon-8.2.0rc1/airflow/providers/amazon/aws/sensors/glacier.py` & `apache-airflow-providers-amazon-8.3.0rc1/airflow/providers/amazon/aws/sensors/glacier.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-amazon-8.2.0rc1/airflow/providers/amazon/aws/sensors/glue.py` & `apache-airflow-providers-amazon-8.3.0rc1/airflow/providers/amazon/aws/sensors/glue.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-amazon-8.2.0rc1/airflow/providers/amazon/aws/sensors/glue_catalog_partition.py` & `apache-airflow-providers-amazon-8.3.0rc1/airflow/providers/amazon/aws/sensors/glue_catalog_partition.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-amazon-8.2.0rc1/airflow/providers/amazon/aws/sensors/glue_crawler.py` & `apache-airflow-providers-amazon-8.3.0rc1/airflow/providers/amazon/aws/sensors/glue_crawler.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-amazon-8.2.0rc1/airflow/providers/amazon/aws/sensors/lambda_function.py` & `apache-airflow-providers-amazon-8.3.0rc1/airflow/providers/amazon/aws/sensors/lambda_function.py`

 * *Files 5% similar despite different names*

```diff
@@ -28,16 +28,15 @@
 
 from airflow.exceptions import AirflowException
 from airflow.sensors.base import BaseSensorOperator
 
 
 class LambdaFunctionStateSensor(BaseSensorOperator):
     """
-    Asks for the state of the Lambda until it reaches a target state.
-    If the query fails, the task will fail.
+    Poll the state of the Lambda until it reaches a target state; fails if the query fails.
 
     .. seealso::
         For more information on how to use this sensor, take a look at the guide:
         :ref:`howto/sensor:LambdaFunctionStateSensor`
 
     :param function_name: The name of the AWS Lambda function, version, or alias.
     :param qualifier: Specify a version or alias to get details about a published version of the function.
```

### Comparing `apache-airflow-providers-amazon-8.2.0rc1/airflow/providers/amazon/aws/sensors/quicksight.py` & `apache-airflow-providers-amazon-8.3.0rc1/airflow/providers/amazon/aws/sensors/quicksight.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-amazon-8.2.0rc1/airflow/providers/amazon/aws/sensors/rds.py` & `apache-airflow-providers-amazon-8.3.0rc1/airflow/providers/amazon/aws/sensors/rds.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-amazon-8.2.0rc1/airflow/providers/amazon/aws/sensors/redshift_cluster.py` & `apache-airflow-providers-amazon-8.3.0rc1/airflow/providers/amazon/aws/sensors/redshift_cluster.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-amazon-8.2.0rc1/airflow/providers/amazon/aws/sensors/s3.py` & `apache-airflow-providers-amazon-8.3.0rc1/airflow/providers/amazon/aws/sensors/s3.py`

 * *Files 7% similar despite different names*

```diff
@@ -22,26 +22,29 @@
 import re
 from datetime import datetime, timedelta
 from functools import cached_property
 from typing import TYPE_CHECKING, Any, Callable, Sequence, cast
 
 from deprecated import deprecated
 
+from airflow.configuration import conf
+
 if TYPE_CHECKING:
     from airflow.utils.context import Context
 
 from airflow.exceptions import AirflowException
 from airflow.providers.amazon.aws.hooks.s3 import S3Hook
-from airflow.providers.amazon.aws.triggers.s3 import S3KeyTrigger
+from airflow.providers.amazon.aws.triggers.s3 import S3KeysUnchangedTrigger, S3KeyTrigger
 from airflow.sensors.base import BaseSensorOperator, poke_mode_only
 
 
 class S3KeySensor(BaseSensorOperator):
     """
     Waits for one or multiple keys (a file-like instance on S3) to be present in a S3 bucket.
+
     The path is just a key/value pointer to a resource for the given S3 path.
     Note: S3 does not support folders directly, and only provides key/value pairs.
 
     .. seealso::
         For more information on how to use this sensor, take a look at the guide:
         :ref:`howto/sensor:S3KeySensor`
 
@@ -82,15 +85,15 @@
         *,
         bucket_key: str | list[str],
         bucket_name: str | None = None,
         wildcard_match: bool = False,
         check_fn: Callable[..., bool] | None = None,
         aws_conn_id: str = "aws_default",
         verify: str | bool | None = None,
-        deferrable: bool = False,
+        deferrable: bool = conf.getboolean("operators", "default_deferrable", fallback=False),
         **kwargs,
     ):
         super().__init__(**kwargs)
         self.bucket_name = bucket_name
         self.bucket_key = bucket_key
         self.wildcard_match = wildcard_match
         self.check_fn = check_fn
@@ -158,16 +161,16 @@
             ),
             method_name="execute_complete",
         )
 
     def execute_complete(self, context: Context, event: dict[str, Any]) -> bool | None:
         """
         Callback for when the trigger fires - returns immediately.
-        Relies on trigger to throw an exception, otherwise it assumes execution was
-        successful.
+
+        Relies on trigger to throw an exception, otherwise it assumes execution was successful.
         """
         if event["status"] == "running":
             found_keys = self.check_fn(event["files"])  # type: ignore[misc]
             if found_keys:
                 return None
             else:
                 self._defer()
@@ -185,19 +188,18 @@
     def hook(self) -> S3Hook:
         return S3Hook(aws_conn_id=self.aws_conn_id, verify=self.verify)
 
 
 @poke_mode_only
 class S3KeysUnchangedSensor(BaseSensorOperator):
     """
-    Checks for changes in the number of objects at prefix in AWS S3
-    bucket and returns True if the inactivity period has passed with no
-    increase in the number of objects. Note, this sensor will not behave correctly
-    in reschedule mode, as the state of the listed objects in the S3 bucket will
-    be lost between rescheduled invocations.
+    Return True if inactivity_period has passed with no increase in the number of objects matching prefix.
+
+    Note, this sensor will not behave correctly in reschedule mode, as the state of the listed
+    objects in the S3 bucket will be lost between rescheduled invocations.
 
     .. seealso::
         For more information on how to use this sensor, take a look at the guide:
         :ref:`howto/sensor:S3KeysUnchangedSensor`
 
     :param bucket_name: Name of the S3 bucket
     :param prefix: The prefix being waited on. Relative path from bucket root level.
@@ -218,14 +220,15 @@
         has passed with no additional objects sensed.
     :param min_objects: The minimum number of objects needed for keys unchanged
         sensor to be considered valid.
     :param previous_objects: The set of object ids found during the last poke.
     :param allow_delete: Should this sensor consider objects being deleted
         between pokes valid behavior. If true a warning message will be logged
         when this happens. If false an error will be raised.
+    :param deferrable: Run sensor in the deferrable mode
     """
 
     template_fields: Sequence[str] = ("bucket_name", "prefix")
 
     def __init__(
         self,
         *,
@@ -233,41 +236,41 @@
         prefix: str,
         aws_conn_id: str = "aws_default",
         verify: bool | str | None = None,
         inactivity_period: float = 60 * 60,
         min_objects: int = 1,
         previous_objects: set[str] | None = None,
         allow_delete: bool = True,
+        deferrable: bool = conf.getboolean("operators", "default_deferrable", fallback=False),
         **kwargs,
     ) -> None:
-
         super().__init__(**kwargs)
 
         self.bucket_name = bucket_name
         self.prefix = prefix
         if inactivity_period < 0:
             raise ValueError("inactivity_period must be non-negative")
         self.inactivity_period = inactivity_period
         self.min_objects = min_objects
         self.previous_objects = previous_objects or set()
         self.inactivity_seconds = 0
         self.allow_delete = allow_delete
+        self.deferrable = deferrable
         self.aws_conn_id = aws_conn_id
         self.verify = verify
         self.last_activity_time: datetime | None = None
 
     @cached_property
     def hook(self):
         """Returns S3Hook."""
         return S3Hook(aws_conn_id=self.aws_conn_id, verify=self.verify)
 
     def is_keys_unchanged(self, current_objects: set[str]) -> bool:
         """
-        Checks whether new objects have been uploaded and the inactivity_period
-        has passed and updates the state of the sensor accordingly.
+        Check for new objects after the inactivity_period and update the sensor state accordingly.
 
         :param current_objects: set of object ids in bucket during last poke.
         """
         current_num_objects = len(current_objects)
         if current_objects > self.previous_objects:
             # When new objects arrived, reset the inactivity_seconds
             # and update previous_objects for the next poke.
@@ -322,7 +325,40 @@
             self.log.error("FAILURE: Inactivity Period passed, not enough objects found in %s", path)
 
             return False
         return False
 
     def poke(self, context: Context):
         return self.is_keys_unchanged(set(self.hook.list_keys(self.bucket_name, prefix=self.prefix)))
+
+    def execute(self, context: Context) -> None:
+        """Airflow runs this method on the worker and defers using the trigger if deferrable is True."""
+        if not self.deferrable:
+            super().execute(context)
+        else:
+            if not self.poke(context):
+                self.defer(
+                    timeout=timedelta(seconds=self.timeout),
+                    trigger=S3KeysUnchangedTrigger(
+                        bucket_name=self.bucket_name,
+                        prefix=self.prefix,
+                        inactivity_period=self.inactivity_period,
+                        min_objects=self.min_objects,
+                        previous_objects=self.previous_objects,
+                        inactivity_seconds=self.inactivity_seconds,
+                        allow_delete=self.allow_delete,
+                        aws_conn_id=self.aws_conn_id,
+                        verify=self.verify,
+                        last_activity_time=self.last_activity_time,
+                    ),
+                    method_name="execute_complete",
+                )
+
+    def execute_complete(self, context: Context, event: dict[str, Any] | None = None) -> None:
+        """
+        Callback for when the trigger fires - returns immediately.
+        Relies on trigger to throw an exception, otherwise it assumes execution was
+        successful.
+        """
+        if event and event["status"] == "error":
+            raise AirflowException(event["message"])
+        return None
```

### Comparing `apache-airflow-providers-amazon-8.2.0rc1/airflow/providers/amazon/aws/sensors/sagemaker.py` & `apache-airflow-providers-amazon-8.3.0rc1/airflow/providers/amazon/aws/sensors/sagemaker.py`

 * *Files 6% similar despite different names*

```diff
@@ -89,16 +89,15 @@
     def state_from_response(self, response: dict) -> str:
         """Placeholder for extracting the state from an AWS response."""
         raise NotImplementedError("Please implement state_from_response() in subclass")
 
 
 class SageMakerEndpointSensor(SageMakerBaseSensor):
     """
-    Polls the endpoint state until it reaches a terminal state.  Raises an
-    AirflowException with the failure reason if a failed state is reached.
+    Poll the endpoint state until it reaches a terminal state; raise AirflowException with the failure reason.
 
     .. seealso::
         For more information on how to use this sensor, take a look at the guide:
         :ref:`howto/sensor:SageMakerEndpointSensor`
 
     :param endpoint_name: Name of the endpoint instance to watch.
     """
@@ -125,16 +124,15 @@
 
     def state_from_response(self, response):
         return response["EndpointStatus"]
 
 
 class SageMakerTransformSensor(SageMakerBaseSensor):
     """
-    Polls the transform job until it reaches a terminal state.  Raises an
-    AirflowException with the failure reason if a failed state is reached.
+    Poll the transform job until it reaches a terminal state; raise AirflowException with the failure reason.
 
     .. seealso::
         For more information on how to use this sensor, take a look at the guide:
         :ref:`howto/sensor:SageMakerTransformSensor`
 
     :param job_name: Name of the transform job to watch.
     """
@@ -161,16 +159,15 @@
 
     def state_from_response(self, response):
         return response["TransformJobStatus"]
 
 
 class SageMakerTuningSensor(SageMakerBaseSensor):
     """
-    Asks for the state of the tuning state until it reaches a terminal state.
-    Raises an AirflowException with the failure reason if a failed state is reached.
+    Poll the tuning state until it reaches a terminal state; raise AirflowException with the failure reason.
 
     .. seealso::
         For more information on how to use this sensor, take a look at the guide:
         :ref:`howto/sensor:SageMakerTuningSensor`
 
     :param job_name: Name of the tuning instance to watch.
     """
@@ -197,16 +194,15 @@
 
     def state_from_response(self, response):
         return response["HyperParameterTuningJobStatus"]
 
 
 class SageMakerTrainingSensor(SageMakerBaseSensor):
     """
-    Polls the training job until it reaches a terminal state.  Raises an
-    AirflowException with the failure reason if a failed state is reached.
+    Poll the training job until it reaches a terminal state; raise AirflowException with the failure reason.
 
     .. seealso::
         For more information on how to use this sensor, take a look at the guide:
         :ref:`howto/sensor:SageMakerTrainingSensor`
 
     :param job_name: Name of the training job to watch.
     :param print_log: Prints the cloudwatch log if True; Defaults to True.
@@ -276,16 +272,15 @@
 
     def state_from_response(self, response):
         return response["TrainingJobStatus"]
 
 
 class SageMakerPipelineSensor(SageMakerBaseSensor):
     """
-    Polls the pipeline until it reaches a terminal state.  Raises an
-    AirflowException with the failure reason if a failed state is reached.
+    Poll the pipeline until it reaches a terminal state; raise AirflowException with the failure reason.
 
     .. seealso::
         For more information on how to use this sensor, take a look at the guide:
         :ref:`howto/sensor:SageMakerPipelineSensor`
 
     :param pipeline_exec_arn: ARN of the pipeline to watch.
     :param verbose: Whether to print steps details while waiting for completion.
@@ -311,16 +306,15 @@
 
     def state_from_response(self, response: dict) -> str:
         return response["PipelineExecutionStatus"]
 
 
 class SageMakerAutoMLSensor(SageMakerBaseSensor):
     """
-    Polls the auto ML job until it reaches a terminal state.
-    Raises an AirflowException with the failure reason if a failed state is reached.
+    Poll the auto ML job until it reaches a terminal state; raise AirflowException with the failure reason.
 
     .. seealso::
         For more information on how to use this sensor, take a look at the guide:
         :ref:`howto/sensor:SageMakerAutoMLSensor`
 
     :param job_name: unique name of the AutoML job to watch.
     """
```

### Comparing `apache-airflow-providers-amazon-8.2.0rc1/airflow/providers/amazon/aws/sensors/sqs.py` & `apache-airflow-providers-amazon-8.3.0rc1/airflow/providers/amazon/aws/sensors/sqs.py`

 * *Files 0% similar despite different names*

```diff
@@ -33,14 +33,15 @@
 if TYPE_CHECKING:
     from airflow.utils.context import Context
 
 
 class SqsSensor(BaseSensorOperator):
     """
     Get messages from an Amazon SQS queue and then delete the messages from the queue.
+
     If deletion of messages fails, an AirflowException is thrown. Otherwise, the messages
     are pushed through XCom with the key ``messages``.
 
     By default,the sensor performs one and only one SQS call per poke, which limits the result to
     a maximum of 10 messages. However, the total number of SQS API calls per poke can be controlled
     by num_batches param.
```

### Comparing `apache-airflow-providers-amazon-8.2.0rc1/airflow/providers/amazon/aws/sensors/step_function.py` & `apache-airflow-providers-amazon-8.3.0rc1/airflow/providers/amazon/aws/sensors/step_function.py`

 * *Files 2% similar despite different names*

```diff
@@ -28,17 +28,15 @@
 
 if TYPE_CHECKING:
     from airflow.utils.context import Context
 
 
 class StepFunctionExecutionSensor(BaseSensorOperator):
     """
-    Asks for the state of the AWS Step Function State Machine Execution until it
-    reaches a failure state or success state.
-    If it fails, then fail the task.
+    Poll the Step Function State Machine Execution until it reaches a terminal state; fails if the task fails.
 
     On successful completion of the Execution the Sensor will do an XCom Push
     of the State Machine's output to `output`
 
     .. seealso::
         For more information on how to use this sensor, take a look at the guide:
         :ref:`howto/sensor:StepFunctionExecutionSensor`
```

### Comparing `apache-airflow-providers-amazon-8.2.0rc1/airflow/providers/amazon/aws/transfers/__init__.py` & `apache-airflow-providers-amazon-8.3.0rc1/airflow/providers/amazon/aws/sensors/__init__.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-amazon-8.2.0rc1/airflow/providers/amazon/aws/transfers/base.py` & `apache-airflow-providers-amazon-8.3.0rc1/airflow/providers/amazon/aws/transfers/base.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-amazon-8.2.0rc1/airflow/providers/amazon/aws/transfers/dynamodb_to_s3.py` & `apache-airflow-providers-amazon-8.3.0rc1/airflow/providers/amazon/aws/transfers/dynamodb_to_s3.py`

 * *Files 2% similar despite different names*

```diff
@@ -11,18 +11,15 @@
 #
 # Unless required by applicable law or agreed to in writing,
 # software distributed under the License is distributed on an
 # "AS IS" BASIS, WITHOUT WARRANTIES OR CONDITIONS OF ANY
 # KIND, either express or implied.  See the License for the
 # specific language governing permissions and limitations
 # under the License.
-"""
-This module contains operators to replicate records from
-DynamoDB table to S3.
-"""
+
 from __future__ import annotations
 
 import json
 from copy import copy
 from datetime import datetime
 from decimal import Decimal
 from functools import cached_property
@@ -68,14 +65,15 @@
         Key=s3_key_prefix + str(uuid4()),
     )
 
 
 class DynamoDBToS3Operator(AwsToAwsBaseOperator):
     """
     Replicates records from a DynamoDB table to S3.
+
     It scans a DynamoDB table and writes the received records to a file
     on the local filesystem. It flushes the file to S3 once the file size
     exceeds the file size limit specified by the user.
 
     Users can also specify a filtering criteria using dynamodb_scan_kwargs
     to only replicate records that satisfy the criteria.
 
@@ -84,15 +82,15 @@
         :ref:`howto/transfer:DynamoDBToS3Operator`
 
     :param dynamodb_table_name: Dynamodb table to replicate data from
     :param s3_bucket_name: S3 bucket to replicate data to
     :param file_size: Flush file to s3 if file size >= file_size
     :param dynamodb_scan_kwargs: kwargs pass to <https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dynamodb.html#DynamoDB.Table.scan>
     :param s3_key_prefix: Prefix of s3 object key
-    :param process_func: How we transforms a dynamodb item to bytes. By default we dump the json
+    :param process_func: How we transform a dynamodb item to bytes. By default, we dump the json
     :param export_time: Time in the past from which to export table data, counted in seconds from the start of
      the Unix epoch. The table export will be a snapshot of the table's state at this point in time.
     :param export_format: The format for the exported data. Valid values for ExportFormat are DYNAMODB_JSON
      or ION.
     """
 
     template_fields: Sequence[str] = (
@@ -143,16 +141,17 @@
         if self.export_time:
             self._export_table_to_point_in_time()
         else:
             self._export_entire_data()
 
     def _export_table_to_point_in_time(self):
         """
-        Export data from start of epoc till `export_time`. Table export will be a snapshot of the table's
-         state at this point in time.
+        Export data from start of epoc till `export_time`.
+
+        Table export will be a snapshot of the table's state at this point in time.
         """
         if self.export_time and self.export_time > datetime.now(self.export_time.tzinfo):
             raise ValueError("The export_time parameter cannot be a future time.")
 
         client = self.hook.conn.meta.client
         table_description = client.describe_table(TableName=self.dynamodb_table_name)
         response = client.export_table_to_point_in_time(
```

### Comparing `apache-airflow-providers-amazon-8.2.0rc1/airflow/providers/amazon/aws/transfers/exasol_to_s3.py` & `apache-airflow-providers-amazon-8.3.0rc1/airflow/providers/amazon/aws/transfers/exasol_to_s3.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-amazon-8.2.0rc1/airflow/providers/amazon/aws/transfers/ftp_to_s3.py` & `apache-airflow-providers-amazon-8.3.0rc1/airflow/providers/amazon/aws/transfers/ftp_to_s3.py`

 * *Files 1% similar despite different names*

```diff
@@ -26,16 +26,15 @@
 
 if TYPE_CHECKING:
     from airflow.utils.context import Context
 
 
 class FTPToS3Operator(BaseOperator):
     """
-    This operator enables the transfer of files from a FTP server to S3. It can be used to
-    transfer one or multiple files.
+    Transfer of one or more files from an FTP server to S3.
 
     .. seealso::
         For more information on how to use this operator, take a look at the guide:
         :ref:`howto/operator:FTPToS3Operator`
 
     :param ftp_path: The ftp remote path. For one file it is mandatory to include the file as well.
         For multiple files, it is the route where the files will be found.
```

### Comparing `apache-airflow-providers-amazon-8.2.0rc1/airflow/providers/amazon/aws/transfers/gcs_to_s3.py` & `apache-airflow-providers-amazon-8.3.0rc1/airflow/providers/amazon/aws/transfers/gcs_to_s3.py`

 * *Files 6% similar despite different names*

```diff
@@ -15,16 +15,18 @@
 # KIND, either express or implied.  See the License for the
 # specific language governing permissions and limitations
 # under the License.
 """This module contains Google Cloud Storage to S3 operator."""
 from __future__ import annotations
 
 import os
+import warnings
 from typing import TYPE_CHECKING, Sequence
 
+from airflow.exceptions import AirflowProviderDeprecationWarning
 from airflow.models import BaseOperator
 from airflow.providers.amazon.aws.hooks.s3 import S3Hook
 from airflow.providers.google.cloud.hooks.gcs import GCSHook
 
 if TYPE_CHECKING:
     from airflow.utils.context import Context
 
@@ -36,15 +38,15 @@
     .. seealso::
         For more information on how to use this operator, take a look at the guide:
         :ref:`howto/operator:GCSToS3Operator`
 
     :param bucket: The Google Cloud Storage bucket to find the objects. (templated)
     :param prefix: Prefix string which filters objects whose name begin with
         this prefix. (templated)
-    :param delimiter: The delimiter by which you want to filter the objects. (templated)
+    :param delimiter: (Deprecated) The delimiter by which you want to filter the objects. (templated)
         For e.g to lists the CSV files from in a directory in GCS you would use
         delimiter='.csv'.
     :param gcp_conn_id: (Optional) The connection ID used to connect to Google Cloud.
     :param dest_aws_conn_id: The destination S3 connection
     :param dest_s3_key: The base S3 key to be used to store the files. (templated)
     :param dest_verify: Whether or not to verify SSL certificates for S3 connection.
         By default SSL certificates are verified.
@@ -72,14 +74,16 @@
         If set as a sequence, the identities from the list must grant
         Service Account Token Creator IAM role to the directly preceding identity, with first
         account from the list granting this role to the originating account (templated).
     :param s3_acl_policy: Optional The string to specify the canned ACL policy for the
         object to be uploaded in S3
     :param keep_directory_structure: (Optional) When set to False the path of the file
          on the bucket is recreated within path passed in dest_s3_key.
+    :param match_glob: (Optional) filters objects based on the glob pattern given by the string
+        (e.g, ``'**/*/.json'``)
     """
 
     template_fields: Sequence[str] = (
         "bucket",
         "prefix",
         "delimiter",
         "dest_s3_key",
@@ -98,30 +102,38 @@
         dest_s3_key: str,
         dest_verify: str | bool | None = None,
         replace: bool = False,
         google_impersonation_chain: str | Sequence[str] | None = None,
         dest_s3_extra_args: dict | None = None,
         s3_acl_policy: str | None = None,
         keep_directory_structure: bool = True,
+        match_glob: str | None = None,
         **kwargs,
     ) -> None:
         super().__init__(**kwargs)
 
         self.bucket = bucket
         self.prefix = prefix
+        if delimiter:
+            warnings.warn(
+                "Usage of 'delimiter' is deprecated, please use 'match_glob' instead",
+                AirflowProviderDeprecationWarning,
+                stacklevel=2,
+            )
         self.delimiter = delimiter
         self.gcp_conn_id = gcp_conn_id
         self.dest_aws_conn_id = dest_aws_conn_id
         self.dest_s3_key = dest_s3_key
         self.dest_verify = dest_verify
         self.replace = replace
         self.google_impersonation_chain = google_impersonation_chain
         self.dest_s3_extra_args = dest_s3_extra_args or {}
         self.s3_acl_policy = s3_acl_policy
         self.keep_directory_structure = keep_directory_structure
+        self.match_glob = match_glob
 
     def execute(self, context: Context) -> list[str]:
         # list all files in an Google Cloud Storage bucket
         hook = GCSHook(
             gcp_conn_id=self.gcp_conn_id,
             impersonation_chain=self.google_impersonation_chain,
         )
@@ -129,28 +141,35 @@
         self.log.info(
             "Getting list of the files. Bucket: %s; Delimiter: %s; Prefix: %s",
             self.bucket,
             self.delimiter,
             self.prefix,
         )
 
-        files = hook.list(bucket_name=self.bucket, prefix=self.prefix, delimiter=self.delimiter)
+        files = hook.list(
+            bucket_name=self.bucket, prefix=self.prefix, delimiter=self.delimiter, match_glob=self.match_glob
+        )
 
         s3_hook = S3Hook(
             aws_conn_id=self.dest_aws_conn_id, verify=self.dest_verify, extra_args=self.dest_s3_extra_args
         )
 
         if not self.keep_directory_structure and self.prefix:
             self.dest_s3_key = os.path.join(self.dest_s3_key, self.prefix)
 
         if not self.replace:
             # if we are not replacing -> list all files in the S3 bucket
             # and only keep those files which are present in
             # Google Cloud Storage and not in S3
             bucket_name, prefix = S3Hook.parse_s3_url(self.dest_s3_key)
+            # if prefix is empty, do not add "/" at end since it would
+            # filter all the objects (return empty list) instead of empty
+            # prefix returning all the objects
+            if prefix:
+                prefix = prefix if prefix.endswith("/") else f"{prefix}/"
             # look for the bucket and the prefix to avoid look into
             # parent directories/keys
             existing_files = s3_hook.list_keys(bucket_name, prefix=prefix)
             # in case that no files exists, return an empty array to avoid errors
             existing_files = existing_files if existing_files is not None else []
             # remove the prefix for the existing files to allow the match
             existing_files = [file.replace(prefix, "", 1) for file in existing_files]
```

### Comparing `apache-airflow-providers-amazon-8.2.0rc1/airflow/providers/amazon/aws/transfers/glacier_to_gcs.py` & `apache-airflow-providers-amazon-8.3.0rc1/airflow/providers/amazon/aws/transfers/glacier_to_gcs.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-amazon-8.2.0rc1/airflow/providers/amazon/aws/transfers/google_api_to_s3.py` & `apache-airflow-providers-amazon-8.3.0rc1/airflow/providers/amazon/aws/transfers/google_api_to_s3.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-amazon-8.2.0rc1/airflow/providers/amazon/aws/transfers/hive_to_dynamodb.py` & `apache-airflow-providers-amazon-8.3.0rc1/airflow/providers/amazon/aws/transfers/hive_to_dynamodb.py`

 * *Files 2% similar despite different names*

```diff
@@ -27,17 +27,18 @@
 
 if TYPE_CHECKING:
     from airflow.utils.context import Context
 
 
 class HiveToDynamoDBOperator(BaseOperator):
     """
-    Moves data from Hive to DynamoDB, note that for now the data is loaded
-    into memory before being pushed to DynamoDB, so this operator should
-    be used for smallish amount of data.
+    Moves data from Hive to DynamoDB.
+
+    Note that for now the data is loaded into memory before being pushed
+    to DynamoDB, so this operator should be used for smallish amount of data.
 
     .. seealso::
         For more information on how to use this operator, take a look at the guide:
         :ref:`howto/transfer:HiveToDynamoDBOperator`
 
     :param sql: SQL query to execute against the hive database. (templated)
     :param table_name: target DynamoDB table
```

### Comparing `apache-airflow-providers-amazon-8.2.0rc1/airflow/providers/amazon/aws/transfers/imap_attachment_to_s3.py` & `apache-airflow-providers-amazon-8.3.0rc1/airflow/providers/amazon/aws/transfers/imap_attachment_to_s3.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-amazon-8.2.0rc1/airflow/providers/amazon/aws/transfers/local_to_s3.py` & `apache-airflow-providers-amazon-8.3.0rc1/airflow/providers/amazon/aws/transfers/local_to_s3.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-amazon-8.2.0rc1/airflow/providers/amazon/aws/transfers/mongo_to_s3.py` & `apache-airflow-providers-amazon-8.3.0rc1/airflow/providers/amazon/aws/transfers/mongo_to_s3.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-amazon-8.2.0rc1/airflow/providers/amazon/aws/transfers/redshift_to_s3.py` & `apache-airflow-providers-amazon-8.3.0rc1/airflow/providers/amazon/aws/transfers/redshift_to_s3.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-amazon-8.2.0rc1/airflow/providers/amazon/aws/transfers/s3_to_ftp.py` & `apache-airflow-providers-amazon-8.3.0rc1/airflow/providers/amazon/aws/transfers/s3_to_ftp.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-amazon-8.2.0rc1/airflow/providers/amazon/aws/transfers/s3_to_redshift.py` & `apache-airflow-providers-amazon-8.3.0rc1/airflow/providers/amazon/aws/transfers/s3_to_redshift.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-amazon-8.2.0rc1/airflow/providers/amazon/aws/transfers/s3_to_sftp.py` & `apache-airflow-providers-amazon-8.3.0rc1/airflow/providers/amazon/aws/transfers/s3_to_sftp.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-amazon-8.2.0rc1/airflow/providers/amazon/aws/transfers/s3_to_sql.py` & `apache-airflow-providers-amazon-8.3.0rc1/airflow/providers/amazon/aws/transfers/s3_to_sql.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-amazon-8.2.0rc1/airflow/providers/amazon/aws/transfers/salesforce_to_s3.py` & `apache-airflow-providers-amazon-8.3.0rc1/airflow/providers/amazon/aws/transfers/salesforce_to_s3.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-amazon-8.2.0rc1/airflow/providers/amazon/aws/transfers/sftp_to_s3.py` & `apache-airflow-providers-amazon-8.3.0rc1/airflow/providers/amazon/aws/transfers/sftp_to_s3.py`

 * *Files 6% similar despite different names*

```diff
@@ -27,16 +27,15 @@
 
 if TYPE_CHECKING:
     from airflow.utils.context import Context
 
 
 class SFTPToS3Operator(BaseOperator):
     """
-    This operator enables the transferring of files from a SFTP server to
-    Amazon S3.
+    Transfer files from an SFTP server to Amazon S3.
 
     .. seealso::
         For more information on how to use this operator, take a look at the guide:
         :ref:`howto/operator:SFTPToS3Operator`
 
     :param sftp_conn_id: The sftp connection id. The name or identifier for
         establishing a connection to the SFTP server.
```

### Comparing `apache-airflow-providers-amazon-8.2.0rc1/airflow/providers/amazon/aws/transfers/sql_to_s3.py` & `apache-airflow-providers-amazon-8.3.0rc1/airflow/providers/amazon/aws/transfers/sql_to_s3.py`

 * *Files 0% similar despite different names*

```diff
@@ -129,14 +129,15 @@
         except KeyError:
             raise AirflowException(f"The argument file_format doesn't support {file_format} value.")
 
     @staticmethod
     def _fix_dtypes(df: DataFrame, file_format: FILE_FORMAT) -> None:
         """
         Mutate DataFrame to set dtypes for float columns containing NaN values.
+
         Set dtype of object to str to allow for downstream transformations.
         """
         try:
             import numpy as np
             from pandas import Float64Dtype, Int64Dtype
         except ImportError as e:
             from airflow.exceptions import AirflowOptionalProviderFeatureException
```

### Comparing `apache-airflow-providers-amazon-8.2.0rc1/airflow/providers/amazon/aws/triggers/__init__.py` & `apache-airflow-providers-amazon-8.3.0rc1/airflow/providers/amazon/aws/triggers/__init__.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-amazon-8.2.0rc1/airflow/providers/amazon/aws/triggers/batch.py` & `apache-airflow-providers-amazon-8.3.0rc1/airflow/providers/amazon/aws/triggers/batch.py`

 * *Files 18% similar despite different names*

```diff
@@ -19,22 +19,21 @@
 import asyncio
 from functools import cached_property
 from typing import Any
 
 from botocore.exceptions import WaiterError
 
 from airflow.providers.amazon.aws.hooks.batch_client import BatchClientHook
+from airflow.providers.amazon.aws.utils.waiter_with_logging import async_wait
 from airflow.triggers.base import BaseTrigger, TriggerEvent
 
 
 class BatchOperatorTrigger(BaseTrigger):
     """
-    Trigger for BatchOperator.
-    The trigger will asynchronously poll the boto3 API and wait for the
-    Batch job to be in the `SUCCEEDED` state.
+    Asynchronously poll the boto3 API and wait for the Batch job to be in the `SUCCEEDED` state.
 
     :param job_id:  A unique identifier for the cluster.
     :param max_retries: The maximum number of attempts to be made.
     :param aws_conn_id: The Airflow connection used for AWS credentials.
     :param region_name: region name to use in AWS Hook
     :param poll_interval: The amount of time in seconds to wait between attempts.
     """
@@ -106,14 +105,15 @@
         else:
             yield TriggerEvent({"status": "success", "job_id": self.job_id})
 
 
 class BatchSensorTrigger(BaseTrigger):
     """
     Checks for the status of a submitted job_id to AWS Batch until it reaches a failure or a success state.
+
     BatchSensorTrigger is fired as deferred class with params to poll the job state in Triggerer.
 
     :param job_id: the job ID, to poll for job completion or not
     :param region_name: AWS region name to use
         Override the region_name in connection (if provided)
     :param aws_conn_id: connection id of AWS credentials / region name. If None,
         credential boto3 strategy will be used
@@ -147,16 +147,15 @@
 
     @cached_property
     def hook(self) -> BatchClientHook:
         return BatchClientHook(aws_conn_id=self.aws_conn_id, region_name=self.region_name)
 
     async def run(self):
         """
-        Make async connection using aiobotocore library to AWS Batch,
-        periodically poll for the Batch job status.
+        Make async connection using aiobotocore library to AWS Batch, periodically poll for the job status.
 
         The status that indicates job completion are: 'SUCCEEDED'|'FAILED'.
         """
         async with self.hook.async_conn as client:
             waiter = self.hook.get_waiter("batch_job_complete", deferrable=True, client=client)
             attempt = 0
             while True:
@@ -184,7 +183,62 @@
             yield TriggerEvent(
                 {
                     "status": "success",
                     "job_id": self.job_id,
                     "message": f"Job {self.job_id} Succeeded",
                 }
             )
+
+
+class BatchCreateComputeEnvironmentTrigger(BaseTrigger):
+    """
+    Asynchronously poll the boto3 API and wait for the compute environment to be ready.
+
+    :param job_id:  A unique identifier for the cluster.
+    :param max_retries: The maximum number of attempts to be made.
+    :param aws_conn_id: The Airflow connection used for AWS credentials.
+    :param region_name: region name to use in AWS Hook
+    :param poll_interval: The amount of time in seconds to wait between attempts.
+    """
+
+    def __init__(
+        self,
+        compute_env_arn: str | None = None,
+        poll_interval: int = 30,
+        max_retries: int = 10,
+        aws_conn_id: str | None = "aws_default",
+        region_name: str | None = None,
+    ):
+        super().__init__()
+        self.compute_env_arn = compute_env_arn
+        self.max_retries = max_retries
+        self.aws_conn_id = aws_conn_id
+        self.region_name = region_name
+        self.poll_interval = poll_interval
+
+    def serialize(self) -> tuple[str, dict[str, Any]]:
+        """Serializes BatchOperatorTrigger arguments and classpath."""
+        return (
+            self.__class__.__module__ + "." + self.__class__.__qualname__,
+            {
+                "compute_env_arn": self.compute_env_arn,
+                "max_retries": self.max_retries,
+                "aws_conn_id": self.aws_conn_id,
+                "region_name": self.region_name,
+                "poll_interval": self.poll_interval,
+            },
+        )
+
+    async def run(self):
+        hook = BatchClientHook(aws_conn_id=self.aws_conn_id, region_name=self.region_name)
+        async with hook.async_conn as client:
+            waiter = hook.get_waiter("compute_env_ready", deferrable=True, client=client)
+            await async_wait(
+                waiter=waiter,
+                waiter_delay=self.poll_interval,
+                waiter_max_attempts=self.max_retries,
+                args={"computeEnvironments": [self.compute_env_arn]},
+                failure_message="Failure while creating Compute Environment",
+                status_message="Compute Environment not ready yet",
+                status_args=["computeEnvironments[].status", "computeEnvironments[].statusReason"],
+            )
+            yield TriggerEvent({"status": "success", "value": self.compute_env_arn})
```

### Comparing `apache-airflow-providers-amazon-8.2.0rc1/airflow/providers/amazon/aws/triggers/ec2.py` & `apache-airflow-providers-amazon-8.3.0rc1/airflow/providers/amazon/aws/triggers/ec2.py`

 * *Files 6% similar despite different names*

```diff
@@ -22,16 +22,15 @@
 
 from airflow.providers.amazon.aws.hooks.ec2 import EC2Hook
 from airflow.triggers.base import BaseTrigger, TriggerEvent
 
 
 class EC2StateSensorTrigger(BaseTrigger):
     """
-    Trigger for EC2StateSensor. The Trigger polls the EC2 instance, and yields a TriggerEvent once
-    the state of the instance matches the `target_state`.
+    Poll the EC2 instance and yield a TriggerEvent once the state of the instance matches the target_state.
 
     :param instance_id: id of the AWS EC2 instance
     :param target_state: target state of instance
     :param aws_conn_id: aws connection to use
     :param region_name: (optional) aws region name associated with the client
     :param poll_interval: number of seconds to wait before attempting the next poll
     """
```

### Comparing `apache-airflow-providers-amazon-8.2.0rc1/airflow/providers/amazon/aws/triggers/emr.py` & `apache-airflow-providers-amazon-8.3.0rc1/airflow/providers/amazon/aws/triggers/emr.py`

 * *Files 10% similar despite different names*

```diff
@@ -20,23 +20,23 @@
 from functools import cached_property
 from typing import Any, AsyncIterator
 
 from botocore.exceptions import WaiterError
 
 from airflow.exceptions import AirflowException
 from airflow.providers.amazon.aws.hooks.emr import EmrContainerHook, EmrHook
+from airflow.providers.amazon.aws.utils.waiter_with_logging import async_wait
 from airflow.triggers.base import BaseTrigger, TriggerEvent
 from airflow.utils.helpers import prune_dict
 
 
 class EmrAddStepsTrigger(BaseTrigger):
     """
-    AWS Emr Add Steps Trigger
-    The trigger will asynchronously poll the boto3 API and wait for the
-    steps to finish executing.
+    Asynchronously poll the boto3 API and wait for the steps to finish executing.
+
     :param job_flow_id: The id of the job flow.
     :param step_ids: The id of the steps being waited upon.
     :param poll_interval: The amount of time in seconds to wait between attempts.
     :param max_attempts: The maximum number of attempts to be made.
     :param aws_conn_id: The Airflow connection used for AWS credentials.
     """
 
@@ -100,17 +100,15 @@
             yield TriggerEvent({"status": "failure", "message": "Steps failed: max attempts reached"})
         else:
             yield TriggerEvent({"status": "success", "message": "Steps completed", "step_ids": self.step_ids})
 
 
 class EmrCreateJobFlowTrigger(BaseTrigger):
     """
-    Trigger for EmrCreateJobFlowOperator.
-    The trigger will asynchronously poll the boto3 API and wait for the
-    JobFlow to finish executing.
+    Asynchronously poll the boto3 API and wait for the JobFlow to finish executing.
 
     :param job_flow_id: The id of the job flow to wait for.
     :param poll_interval: The amount of time in seconds to wait between attempts.
     :param max_attempts: The maximum number of attempts to be made.
     :param aws_conn_id: The Airflow connection used for AWS credentials.
     """
 
@@ -174,17 +172,15 @@
                     "job_flow_id": self.job_flow_id,
                 }
             )
 
 
 class EmrTerminateJobFlowTrigger(BaseTrigger):
     """
-    Trigger that terminates a running EMR Job Flow.
-    The trigger will asynchronously poll the boto3 API and wait for the
-    JobFlow to finish terminating.
+    Asynchronously poll the boto3 API and wait for the JobFlow to finish terminating.
 
     :param job_flow_id: ID of the EMR Job Flow to terminate
     :param poll_interval: The amount of time in seconds to wait between attempts.
     :param max_attempts: The maximum number of attempts to be made.
     :param aws_conn_id: The Airflow connection used for AWS credentials.
     """
 
@@ -245,15 +241,15 @@
                 {
                     "status": "success",
                     "message": "JobFlow terminated successfully",
                 }
             )
 
 
-class EmrContainerSensorTrigger(BaseTrigger):
+class EmrContainerTrigger(BaseTrigger):
     """
     Poll for the status of EMR container until reaches terminal state.
 
     :param virtual_cluster_id: Reference Emr cluster id
     :param job_id:  job_id to check the state
     :param aws_conn_id: Reference to AWS connection id
     :param poll_interval: polling period in seconds to check for the status
@@ -274,17 +270,17 @@
         super().__init__(**kwargs)
 
     @cached_property
     def hook(self) -> EmrContainerHook:
         return EmrContainerHook(self.aws_conn_id, virtual_cluster_id=self.virtual_cluster_id)
 
     def serialize(self) -> tuple[str, dict[str, Any]]:
-        """Serializes EmrContainerSensorTrigger arguments and classpath."""
+        """Serializes EmrContainerTrigger arguments and classpath."""
         return (
-            "airflow.providers.amazon.aws.triggers.emr.EmrContainerSensorTrigger",
+            "airflow.providers.amazon.aws.triggers.emr.EmrContainerTrigger",
             {
                 "virtual_cluster_id": self.virtual_cluster_id,
                 "job_id": self.job_id,
                 "aws_conn_id": self.aws_conn_id,
                 "poll_interval": self.poll_interval,
             },
         )
@@ -313,7 +309,67 @@
                         "Job status is %s. Retrying attempt %s",
                         error.last_response["jobRun"]["state"],
                         attempt,
                     )
                     await asyncio.sleep(int(self.poll_interval))
 
             yield TriggerEvent({"status": "success", "job_id": self.job_id})
+
+
+class EmrStepSensorTrigger(BaseTrigger):
+    """
+    Poll for the status of EMR container until reaches terminal state.
+
+    :param job_flow_id: job_flow_id which contains the step check the state of
+    :param step_id:  step to check the state of
+    :param aws_conn_id: Reference to AWS connection id
+    :param max_attempts: The maximum number of attempts to be made
+    :param poke_interval: polling period in seconds to check for the status
+    """
+
+    def __init__(
+        self,
+        job_flow_id: str,
+        step_id: str,
+        aws_conn_id: str = "aws_default",
+        max_attempts: int = 60,
+        poke_interval: int = 30,
+        **kwargs: Any,
+    ):
+        self.job_flow_id = job_flow_id
+        self.step_id = step_id
+        self.aws_conn_id = aws_conn_id
+        self.max_attempts = max_attempts
+        self.poke_interval = poke_interval
+        super().__init__(**kwargs)
+
+    @cached_property
+    def hook(self) -> EmrHook:
+        return EmrHook(self.aws_conn_id)
+
+    def serialize(self) -> tuple[str, dict[str, Any]]:
+        return (
+            "airflow.providers.amazon.aws.triggers.emr.EmrStepSensorTrigger",
+            {
+                "job_flow_id": self.job_flow_id,
+                "step_id": self.step_id,
+                "aws_conn_id": self.aws_conn_id,
+                "max_attempts": self.max_attempts,
+                "poke_interval": self.poke_interval,
+            },
+        )
+
+    async def run(self) -> AsyncIterator[TriggerEvent]:
+
+        async with self.hook.async_conn as client:
+            waiter = client.get_waiter("step_wait_for_terminal", deferrable=True, client=client)
+            await async_wait(
+                waiter=waiter,
+                waiter_delay=self.poke_interval,
+                waiter_max_attempts=self.max_attempts,
+                args={"ClusterId": self.job_flow_id, "StepId": self.step_id},
+                failure_message=f"Error while waiting for step {self.step_id} to complete",
+                status_message=f"Step id: {self.step_id}, Step is still in non-terminal state",
+                status_args=["Step.Status.State"],
+            )
+
+        yield TriggerEvent({"status": "success"})
```

### Comparing `apache-airflow-providers-amazon-8.2.0rc1/airflow/providers/amazon/aws/triggers/glue.py` & `apache-airflow-providers-amazon-8.3.0rc1/airflow/providers/amazon/aws/triggers/glue.py`

 * *Files 11% similar despite different names*

```diff
@@ -35,29 +35,33 @@
 
     def __init__(
         self,
         job_name: str,
         run_id: str,
         verbose: bool,
         aws_conn_id: str,
+        job_poll_interval: int | float,
     ):
+        super().__init__()
         self.job_name = job_name
         self.run_id = run_id
         self.verbose = verbose
         self.aws_conn_id = aws_conn_id
+        self.job_poll_interval = job_poll_interval
 
     def serialize(self) -> tuple[str, dict[str, Any]]:
         return (
             # dynamically generate the fully qualified name of the class
             self.__class__.__module__ + "." + self.__class__.__qualname__,
             {
                 "job_name": self.job_name,
                 "run_id": self.run_id,
                 "verbose": str(self.verbose),
                 "aws_conn_id": self.aws_conn_id,
+                "job_poll_interval": self.job_poll_interval,
             },
         )
 
     async def run(self) -> AsyncIterator[TriggerEvent]:
-        hook = GlueJobHook(aws_conn_id=self.aws_conn_id)
+        hook = GlueJobHook(aws_conn_id=self.aws_conn_id, job_poll_interval=self.job_poll_interval)
         await hook.async_job_completion(self.job_name, self.run_id, self.verbose)
         yield TriggerEvent({"status": "success", "message": "Job done", "value": self.run_id})
```

### Comparing `apache-airflow-providers-amazon-8.2.0rc1/airflow/providers/amazon/aws/triggers/glue_crawler.py` & `apache-airflow-providers-amazon-8.3.0rc1/airflow/providers/amazon/aws/triggers/glue_crawler.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-amazon-8.2.0rc1/airflow/providers/amazon/aws/triggers/redshift_cluster.py` & `apache-airflow-providers-amazon-8.3.0rc1/airflow/providers/amazon/aws/triggers/redshift_cluster.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-amazon-8.2.0rc1/airflow/providers/amazon/aws/triggers/sagemaker.py` & `apache-airflow-providers-amazon-8.3.0rc1/airflow/providers/amazon/aws/triggers/sagemaker.py`

 * *Files 9% similar despite different names*

```diff
@@ -17,14 +17,15 @@
 
 from __future__ import annotations
 
 from functools import cached_property
 from typing import Any
 
 from airflow.providers.amazon.aws.hooks.sagemaker import SageMakerHook
+from airflow.providers.amazon.aws.utils.waiter_with_logging import async_wait
 from airflow.triggers.base import BaseTrigger, TriggerEvent
 
 
 class SageMakerTrigger(BaseTrigger):
     """
     SageMakerTrigger is fired as deferred class with params to run the task in triggerer.
 
@@ -37,15 +38,15 @@
     """
 
     def __init__(
         self,
         job_name: str,
         job_type: str,
         poke_interval: int = 30,
-        max_attempts: int | None = None,
+        max_attempts: int = 480,
         aws_conn_id: str = "aws_default",
     ):
         super().__init__()
         self.job_name = job_name
         self.job_type = job_type
         self.poke_interval = poke_interval
         self.max_attempts = max_attempts
@@ -70,32 +71,47 @@
 
     @staticmethod
     def _get_job_type_waiter(job_type: str) -> str:
         return {
             "training": "TrainingJobComplete",
             "transform": "TransformJobComplete",
             "processing": "ProcessingJobComplete",
+            "tuning": "TuningJobComplete",
+            "endpoint": "endpoint_in_service",  # this one is provided by boto
         }[job_type.lower()]
 
     @staticmethod
-    def _get_job_type_waiter_job_name_arg(job_type: str) -> str:
+    def _get_waiter_arg_name(job_type: str) -> str:
         return {
             "training": "TrainingJobName",
             "transform": "TransformJobName",
             "processing": "ProcessingJobName",
+            "tuning": "HyperParameterTuningJobName",
+            "endpoint": "EndpointName",
+        }[job_type.lower()]
+
+    @staticmethod
+    def _get_response_status_key(job_type: str) -> str:
+        return {
+            "training": "TrainingJobStatus",
+            "transform": "TransformJobStatus",
+            "processing": "ProcessingJobStatus",
+            "tuning": "HyperParameterTuningJobStatus",
+            "endpoint": "EndpointStatus",
         }[job_type.lower()]
 
     async def run(self):
         self.log.info("job name is %s and job type is %s", self.job_name, self.job_type)
         async with self.hook.async_conn as client:
             waiter = self.hook.get_waiter(
                 self._get_job_type_waiter(self.job_type), deferrable=True, client=client
             )
-            waiter_args = {
-                self._get_job_type_waiter_job_name_arg(self.job_type): self.job_name,
-                "WaiterConfig": {
-                    "Delay": self.poke_interval,
-                    "MaxAttempts": self.max_attempts,
-                },
-            }
-            await waiter.wait(**waiter_args)
-        yield TriggerEvent({"status": "success", "message": "Job completed."})
+            await async_wait(
+                waiter=waiter,
+                waiter_delay=self.poke_interval,
+                waiter_max_attempts=self.max_attempts,
+                args={self._get_waiter_arg_name(self.job_type): self.job_name},
+                failure_message=f"Error while waiting for {self.job_type} job",
+                status_message=f"{self.job_type} job not done yet",
+                status_args=[self._get_response_status_key(self.job_type)],
+            )
+            yield TriggerEvent({"status": "success", "message": "Job completed."})
```

### Comparing `apache-airflow-providers-amazon-8.2.0rc1/airflow/providers/amazon/aws/utils/__init__.py` & `apache-airflow-providers-amazon-8.3.0rc1/airflow/providers/amazon/aws/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-amazon-8.2.0rc1/airflow/providers/amazon/aws/utils/connection_wrapper.py` & `apache-airflow-providers-amazon-8.3.0rc1/airflow/providers/amazon/aws/utils/connection_wrapper.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-amazon-8.2.0rc1/airflow/providers/amazon/aws/utils/eks_get_token.py` & `apache-airflow-providers-amazon-8.3.0rc1/airflow/providers/amazon/aws/utils/eks_get_token.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-amazon-8.2.0rc1/airflow/providers/amazon/aws/utils/emailer.py` & `apache-airflow-providers-amazon-8.3.0rc1/airflow/providers/amazon/aws/utils/emailer.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-amazon-8.2.0rc1/airflow/providers/amazon/aws/utils/rds.py` & `apache-airflow-providers-amazon-8.3.0rc1/airflow/providers/amazon/aws/utils/rds.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-amazon-8.2.0rc1/airflow/providers/amazon/aws/utils/redshift.py` & `apache-airflow-providers-amazon-8.3.0rc1/airflow/providers/amazon/aws/utils/redshift.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-amazon-8.2.0rc1/airflow/providers/amazon/aws/utils/sagemaker.py` & `apache-airflow-providers-amazon-8.3.0rc1/airflow/providers/amazon/aws/utils/sagemaker.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-amazon-8.2.0rc1/airflow/providers/amazon/aws/utils/tags.py` & `apache-airflow-providers-amazon-8.3.0rc1/airflow/providers/amazon/aws/utils/tags.py`

 * *Files 4% similar despite different names*

```diff
@@ -17,16 +17,19 @@
 from __future__ import annotations
 
 from typing import Any
 
 
 def format_tags(source: Any, *, key_label: str = "Key", value_label: str = "Value"):
     """
+    Format tags for boto call which expect a given format.
+
     If given a dictionary, formats it as an array of objects with a key and a value field to be passed to boto
     calls that expect this format.
+
     Else, assumes that it's already in the right format and returns it as is. We do not validate
     the format here since it's done by boto anyway, and the error would not be clearer if thrown from here.
 
     :param source: a dict from which keys and values are read
     :param key_label: optional, the label to use for keys if not "Key"
     :param value_label: optional, the label to use for values if not "Value"
     """
```

### Comparing `apache-airflow-providers-amazon-8.2.0rc1/airflow/providers/amazon/aws/utils/task_log_fetcher.py` & `apache-airflow-providers-amazon-8.3.0rc1/airflow/providers/amazon/aws/utils/task_log_fetcher.py`

 * *Files 12% similar despite different names*

```diff
@@ -14,30 +14,26 @@
 # KIND, either express or implied.  See the License for the
 # specific language governing permissions and limitations
 # under the License.
 
 from __future__ import annotations
 
 import time
-from collections import deque
 from datetime import datetime, timedelta
 from logging import Logger
 from threading import Event, Thread
 from typing import Generator
 
 from botocore.exceptions import ClientError, ConnectionClosedError
 
 from airflow.providers.amazon.aws.hooks.logs import AwsLogsHook
 
 
 class AwsTaskLogFetcher(Thread):
-    """
-    Fetches Cloudwatch log events with specific interval as a thread
-    and sends the log events to the info channel of the provided logger.
-    """
+    """Fetch Cloudwatch log events with specific interval and send the log events to the logger.info."""
 
     def __init__(
         self,
         *,
         log_group: str,
         log_stream_name: str,
         fetch_interval: timedelta,
@@ -58,15 +54,15 @@
 
     def run(self) -> None:
         continuation_token = AwsLogsHook.ContinuationToken()
         while not self.is_stopped():
             time.sleep(self.fetch_interval.total_seconds())
             log_events = self._get_log_events(continuation_token)
             for log_event in log_events:
-                self.logger.info(self._event_to_str(log_event))
+                self.logger.info(self.event_to_str(log_event))
 
     def _get_log_events(self, skip_token: AwsLogsHook.ContinuationToken | None = None) -> Generator:
         if skip_token is None:
             skip_token = AwsLogsHook.ContinuationToken()
         try:
             yield from self.hook.get_log_events(
                 self.log_group, self.log_stream_name, continuation_token=skip_token
@@ -83,22 +79,36 @@
                     self.log_stream_name,
                 )
             yield from ()
         except ConnectionClosedError as error:
             self.logger.warning("ConnectionClosedError on retrieving Cloudwatch log events", error)
             yield from ()
 
-    def _event_to_str(self, event: dict) -> str:
+    @staticmethod
+    def event_to_str(event: dict) -> str:
         event_dt = datetime.utcfromtimestamp(event["timestamp"] / 1000.0)
         formatted_event_dt = event_dt.strftime("%Y-%m-%d %H:%M:%S,%f")[:-3]
         message = event["message"]
         return f"[{formatted_event_dt}] {message}"
 
     def get_last_log_messages(self, number_messages) -> list:
-        return [log["message"] for log in deque(self._get_log_events(), maxlen=number_messages)]
+        """
+        Gets the last logs messages in one single request.
+
+         NOTE: some restrictions apply:
+         - if logs are too old, the response will be empty
+         - the max number of messages we can retrieve is constrained by cloudwatch limits (10,000).
+        """
+        response = self.hook.conn.get_log_events(
+            logGroupName=self.log_group,
+            logStreamName=self.log_stream_name,
+            startFromHead=False,
+            limit=number_messages,
+        )
+        return [log["message"] for log in response["events"]]
 
     def get_last_log_message(self) -> str | None:
         try:
             return self.get_last_log_messages(1)[0]
         except IndexError:
             return None
```

### Comparing `apache-airflow-providers-amazon-8.2.0rc1/airflow/providers/amazon/aws/utils/waiter.py` & `apache-airflow-providers-amazon-8.3.0rc1/airflow/providers/amazon/aws/utils/waiter.py`

 * *Files 2% similar despite different names*

```diff
@@ -34,16 +34,15 @@
     failure_states: set,
     object_type: str,
     action: str,
     countdown: int | float | None = 25 * 60,
     check_interval_seconds: int = 60,
 ) -> None:
     """
-    Will call get_state_callable until it reaches the desired_state or the failure_states.
-    It will also time out if it waits longer than countdown seconds.
+    Call get_state_callable until it reaches the desired_state or the failure_states.
 
     PLEASE NOTE:  While not yet deprecated, we are moving away from this method
                   and encourage using the custom boto waiters as explained in
                   https://github.com/apache/airflow/tree/main/airflow/providers/amazon/aws/waiters
 
     :param get_state_callable: A callable to run until it returns True
     :param get_state_args: Arguments to pass to get_state_callable
```

### Comparing `apache-airflow-providers-amazon-8.2.0rc1/airflow/providers/amazon/aws/waiters/__init__.py` & `apache-airflow-providers-amazon-8.3.0rc1/airflow/providers/amazon/aws/transfers/__init__.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-amazon-8.2.0rc1/airflow/providers/amazon/aws/waiters/appflow.json` & `apache-airflow-providers-amazon-8.3.0rc1/airflow/providers/amazon/aws/waiters/appflow.json`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-amazon-8.2.0rc1/airflow/providers/amazon/aws/waiters/base_waiter.py` & `apache-airflow-providers-amazon-8.3.0rc1/airflow/providers/amazon/aws/waiters/base_waiter.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-amazon-8.2.0rc1/airflow/providers/amazon/aws/waiters/dynamodb.json` & `apache-airflow-providers-amazon-8.3.0rc1/airflow/providers/amazon/aws/waiters/dynamodb.json`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-amazon-8.2.0rc1/airflow/providers/amazon/aws/waiters/ecs.json` & `apache-airflow-providers-amazon-8.3.0rc1/airflow/providers/amazon/aws/waiters/ecs.json`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-amazon-8.2.0rc1/airflow/providers/amazon/aws/waiters/eks.json` & `apache-airflow-providers-amazon-8.3.0rc1/airflow/providers/amazon/aws/waiters/eks.json`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-amazon-8.2.0rc1/airflow/providers/amazon/aws/waiters/emr-containers.json` & `apache-airflow-providers-amazon-8.3.0rc1/airflow/providers/amazon/aws/waiters/emr-containers.json`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-amazon-8.2.0rc1/airflow/providers/amazon/aws/waiters/emr.json` & `apache-airflow-providers-amazon-8.3.0rc1/airflow/providers/amazon/aws/waiters/emr.json`

 * *Files 17% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.95%*

 * *Differences: {"'waiters'": "{'step_wait_for_terminal': OrderedDict([('operation', 'DescribeStep'), ('delay', "*

 * *              "30), ('maxAttempts', 60), ('acceptors', [OrderedDict([('matcher', 'path'), "*

 * *              "('argument', 'Step.Status.State'), ('expected', 'COMPLETED'), ('state', "*

 * *              "'success')]), OrderedDict([('matcher', 'path'), ('argument', 'Step.Status.State'), "*

 * *              "('expected', 'CANCELLED'), ('state', 'failure')]), OrderedDict([('matcher', "*

 * *              "'path'), ('argument', 'St […]*

```diff
@@ -90,10 +90,41 @@
                     "matcher": "path",
                     "state": "failure"
                 }
             ],
             "delay": 30,
             "maxAttempts": 60,
             "operation": "DescribeNotebookExecution"
+        },
+        "step_wait_for_terminal": {
+            "acceptors": [
+                {
+                    "argument": "Step.Status.State",
+                    "expected": "COMPLETED",
+                    "matcher": "path",
+                    "state": "success"
+                },
+                {
+                    "argument": "Step.Status.State",
+                    "expected": "CANCELLED",
+                    "matcher": "path",
+                    "state": "failure"
+                },
+                {
+                    "argument": "Step.Status.State",
+                    "expected": "FAILED",
+                    "matcher": "path",
+                    "state": "failure"
+                },
+                {
+                    "argument": "Step.Status.State",
+                    "expected": "INTERRUPTED",
+                    "matcher": "path",
+                    "state": "failure"
+                }
+            ],
+            "delay": 30,
+            "maxAttempts": 60,
+            "operation": "DescribeStep"
         }
     }
 }
```

### Comparing `apache-airflow-providers-amazon-8.2.0rc1/airflow/providers/amazon/aws/waiters/glue.json` & `apache-airflow-providers-amazon-8.3.0rc1/airflow/providers/amazon/aws/waiters/glue.json`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-amazon-8.2.0rc1/airflow/providers/amazon/aws/waiters/redshift.json` & `apache-airflow-providers-amazon-8.3.0rc1/airflow/providers/amazon/aws/waiters/redshift.json`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-amazon-8.2.0rc1/airflow/providers/amazon/aws/waiters/sagemaker.json` & `apache-airflow-providers-amazon-8.3.0rc1/airflow/providers/amazon/aws/waiters/sagemaker.json`

 * *Files 14% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9375%*

 * *Differences: {"'waiters'": "{'TuningJobComplete': OrderedDict([('delay', 30), ('operation', "*

 * *              "'DescribeHyperParameterTuningJob'), ('maxAttempts', 60), ('description', 'Wait "*

 * *              "until job is COMPLETED'), ('acceptors', [OrderedDict([('matcher', 'path'), "*

 * *              "('argument', 'HyperParameterTuningJobStatus'), ('expected', 'Completed'), ('state', "*

 * *              "'success')]), OrderedDict([('matcher', 'path'), ('argument', "*

 * *              "'HyperParameterTuningJobStatus'), ('expected', 'F […]*

```diff
@@ -74,10 +74,36 @@
                     "state": "failure"
                 }
             ],
             "delay": 30,
             "description": "Wait until job is COMPLETED",
             "maxAttempts": 60,
             "operation": "DescribeTransformJob"
+        },
+        "TuningJobComplete": {
+            "acceptors": [
+                {
+                    "argument": "HyperParameterTuningJobStatus",
+                    "expected": "Completed",
+                    "matcher": "path",
+                    "state": "success"
+                },
+                {
+                    "argument": "HyperParameterTuningJobStatus",
+                    "expected": "Failed",
+                    "matcher": "path",
+                    "state": "failure"
+                },
+                {
+                    "argument": "HyperParameterTuningJobStatus",
+                    "expected": "Stopped",
+                    "matcher": "path",
+                    "state": "failure"
+                }
+            ],
+            "delay": 30,
+            "description": "Wait until job is COMPLETED",
+            "maxAttempts": 60,
+            "operation": "DescribeHyperParameterTuningJob"
         }
     }
 }
```

### Comparing `apache-airflow-providers-amazon-8.2.0rc1/airflow/providers/amazon/get_provider_info.py` & `apache-airflow-providers-amazon-8.3.0rc1/airflow/providers/amazon/get_provider_info.py`

 * *Files 2% similar despite different names*

```diff
@@ -25,14 +25,15 @@
 def get_provider_info():
     return {
         "package-name": "apache-airflow-providers-amazon",
         "name": "Amazon",
         "description": "Amazon integration (including `Amazon Web Services (AWS) <https://aws.amazon.com/>`__).\n",
         "suspended": False,
         "versions": [
+            "8.3.0",
             "8.2.0",
             "8.1.0",
             "8.0.0",
             "7.4.1",
             "7.4.0",
             "7.3.0",
             "7.2.1",
@@ -63,14 +64,15 @@
             "1.2.0",
             "1.1.0",
             "1.0.0",
         ],
         "dependencies": [
             "apache-airflow>=2.4.0",
             "apache-airflow-providers-common-sql>=1.3.1",
+            "apache-airflow-providers-http",
             "boto3>=1.24.0",
             "asgiref",
             "watchtower~=2.0.1",
             "jsonpath_ng>=1.5.3",
             "redshift_connector>=2.0.888",
             "sqlalchemy_redshift>=0.8.6",
             "mypy-boto3-rds>=1.24.0",
@@ -84,14 +86,20 @@
                 "integration-name": "Amazon Athena",
                 "external-doc-url": "https://aws.amazon.com/athena/",
                 "logo": "/integration-logos/aws/Amazon-Athena_light-bg@4x.png",
                 "how-to-guide": ["/docs/apache-airflow-providers-amazon/operators/athena.rst"],
                 "tags": ["aws"],
             },
             {
+                "integration-name": "Amazon Chime",
+                "external-doc-url": "https://aws.amazon.com/chime/",
+                "logo": "/integration-logos/aws/Amazon-Chime-light-bg.png",
+                "tags": ["aws"],
+            },
+            {
                 "integration-name": "Amazon CloudFormation",
                 "external-doc-url": "https://aws.amazon.com/cloudformation/",
                 "logo": "/integration-logos/aws/AWS-CloudFormation_light-bg@4x.png",
                 "how-to-guide": ["/docs/apache-airflow-providers-amazon/operators/cloudformation.rst"],
                 "tags": ["aws"],
             },
             {
@@ -504,14 +512,18 @@
         ],
         "hooks": [
             {
                 "integration-name": "Amazon Athena",
                 "python-modules": ["airflow.providers.amazon.aws.hooks.athena"],
             },
             {
+                "integration-name": "Amazon Chime",
+                "python-modules": ["airflow.providers.amazon.aws.hooks.chime"],
+            },
+            {
                 "integration-name": "Amazon DynamoDB",
                 "python-modules": ["airflow.providers.amazon.aws.hooks.dynamodb"],
             },
             {
                 "integration-name": "Amazon Web Services",
                 "python-modules": ["airflow.providers.amazon.aws.hooks.base_aws"],
             },
@@ -629,14 +641,18 @@
             {
                 "integration-name": "Amazon Appflow",
                 "python-modules": ["airflow.providers.amazon.aws.hooks.appflow"],
             },
         ],
         "triggers": [
             {
+                "integration-name": "Amazon Athena",
+                "python-modules": ["airflow.providers.amazon.aws.triggers.athena"],
+            },
+            {
                 "integration-name": "AWS Batch",
                 "python-modules": ["airflow.providers.amazon.aws.triggers.batch"],
             },
             {
                 "integration-name": "Amazon EC2",
                 "python-modules": ["airflow.providers.amazon.aws.triggers.ec2"],
             },
@@ -663,14 +679,22 @@
                 "integration-name": "Amazon EMR",
                 "python-modules": ["airflow.providers.amazon.aws.triggers.emr"],
             },
             {
                 "integration-name": "Amazon Elastic Kubernetes Service (EKS)",
                 "python-modules": ["airflow.providers.amazon.aws.triggers.eks"],
             },
+            {
+                "integration-name": "Amazon ECS",
+                "python-modules": ["airflow.providers.amazon.aws.triggers.ecs"],
+            },
+            {
+                "integration-name": "Amazon RDS",
+                "python-modules": ["airflow.providers.amazon.aws.triggers.rds"],
+            },
         ],
         "transfers": [
             {
                 "source-integration-name": "Amazon DynamoDB",
                 "target-integration-name": "Amazon Simple Storage Service (S3)",
                 "how-to-guide": "/docs/apache-airflow-providers-amazon/transfer/dynamodb_to_s3.rst",
                 "python-module": "airflow.providers.amazon.aws.transfers.dynamodb_to_s3",
@@ -777,14 +801,20 @@
                 "python-module": "airflow.providers.amazon.aws.transfers.s3_to_sql",
             },
             {
                 "source-integration-name": "Amazon Web Services",
                 "target-integration-name": "Amazon Web Services",
                 "python-module": "airflow.providers.amazon.aws.transfers.base",
             },
+            {
+                "source-integration-name": "Microsoft Azure Blob Storage",
+                "target-integration-name": "Amazon Simple Storage Service (S3)",
+                "how-to-guide": "/docs/apache-airflow-providers-amazon/transfer/azure_blob_to_s3.rst",
+                "python-module": "airflow.providers.amazon.aws.transfers.azure_blob_to_s3",
+            },
         ],
         "extra-links": [
             "airflow.providers.amazon.aws.links.batch.BatchJobDefinitionLink",
             "airflow.providers.amazon.aws.links.batch.BatchJobDetailsLink",
             "airflow.providers.amazon.aws.links.batch.BatchJobQueueLink",
             "airflow.providers.amazon.aws.links.emr.EmrClusterLink",
             "airflow.providers.amazon.aws.links.emr.EmrLogsLink",
@@ -792,26 +822,32 @@
             "airflow.providers.amazon.aws.links.logs.CloudWatchEventsLink",
         ],
         "connection-types": [
             {
                 "hook-class-name": "airflow.providers.amazon.aws.hooks.base_aws.AwsGenericHook",
                 "connection-type": "aws",
             },
+            {
+                "hook-class-name": "airflow.providers.amazon.aws.hooks.chime.ChimeWebhookHook",
+                "connection-type": "chime",
+            },
             {"hook-class-name": "airflow.providers.amazon.aws.hooks.emr.EmrHook", "connection-type": "emr"},
             {
                 "hook-class-name": "airflow.providers.amazon.aws.hooks.redshift_sql.RedshiftSQLHook",
                 "connection-type": "redshift",
             },
         ],
+        "notifications": ["airflow.providers.amazon.aws.notifications.chime.ChimeNotifier"],
         "secrets-backends": [
             "airflow.providers.amazon.aws.secrets.secrets_manager.SecretsManagerBackend",
             "airflow.providers.amazon.aws.secrets.systems_manager.SystemsManagerParameterStoreBackend",
         ],
         "logging": [
             "airflow.providers.amazon.aws.log.s3_task_handler.S3TaskHandler",
             "airflow.providers.amazon.aws.log.cloudwatch_task_handler.CloudwatchTaskHandler",
         ],
         "additional-extras": [
             {"name": "pandas", "dependencies": ["pandas>=0.17.1"]},
             {"name": "aiobotocore", "dependencies": ["aiobotocore[boto3]>=2.2.0"]},
+            {"name": "cncf.kubernetes", "dependencies": ["apache-airflow-providers-cncf-kubernetes>=7.2.0"]},
         ],
     }
```

### Comparing `apache-airflow-providers-amazon-8.2.0rc1/apache_airflow_providers_amazon.egg-info/SOURCES.txt` & `apache-airflow-providers-amazon-8.3.0rc1/apache_airflow_providers_amazon.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -12,14 +12,15 @@
 airflow/providers/amazon/aws/hooks/__init__.py
 airflow/providers/amazon/aws/hooks/appflow.py
 airflow/providers/amazon/aws/hooks/athena.py
 airflow/providers/amazon/aws/hooks/base_aws.py
 airflow/providers/amazon/aws/hooks/batch_client.py
 airflow/providers/amazon/aws/hooks/batch_waiters.json
 airflow/providers/amazon/aws/hooks/batch_waiters.py
+airflow/providers/amazon/aws/hooks/chime.py
 airflow/providers/amazon/aws/hooks/cloud_formation.py
 airflow/providers/amazon/aws/hooks/datasync.py
 airflow/providers/amazon/aws/hooks/dms.py
 airflow/providers/amazon/aws/hooks/dynamodb.py
 airflow/providers/amazon/aws/hooks/ec2.py
 airflow/providers/amazon/aws/hooks/ecr.py
 airflow/providers/amazon/aws/hooks/ecs.py
@@ -52,14 +53,16 @@
 airflow/providers/amazon/aws/links/batch.py
 airflow/providers/amazon/aws/links/emr.py
 airflow/providers/amazon/aws/links/glue.py
 airflow/providers/amazon/aws/links/logs.py
 airflow/providers/amazon/aws/log/__init__.py
 airflow/providers/amazon/aws/log/cloudwatch_task_handler.py
 airflow/providers/amazon/aws/log/s3_task_handler.py
+airflow/providers/amazon/aws/notifications/__init__.py
+airflow/providers/amazon/aws/notifications/chime.py
 airflow/providers/amazon/aws/operators/__init__.py
 airflow/providers/amazon/aws/operators/appflow.py
 airflow/providers/amazon/aws/operators/athena.py
 airflow/providers/amazon/aws/operators/batch.py
 airflow/providers/amazon/aws/operators/cloud_formation.py
 airflow/providers/amazon/aws/operators/datasync.py
 airflow/providers/amazon/aws/operators/dms.py
@@ -102,14 +105,15 @@
 airflow/providers/amazon/aws/sensors/rds.py
 airflow/providers/amazon/aws/sensors/redshift_cluster.py
 airflow/providers/amazon/aws/sensors/s3.py
 airflow/providers/amazon/aws/sensors/sagemaker.py
 airflow/providers/amazon/aws/sensors/sqs.py
 airflow/providers/amazon/aws/sensors/step_function.py
 airflow/providers/amazon/aws/transfers/__init__.py
+airflow/providers/amazon/aws/transfers/azure_blob_to_s3.py
 airflow/providers/amazon/aws/transfers/base.py
 airflow/providers/amazon/aws/transfers/dynamodb_to_s3.py
 airflow/providers/amazon/aws/transfers/exasol_to_s3.py
 airflow/providers/amazon/aws/transfers/ftp_to_s3.py
 airflow/providers/amazon/aws/transfers/gcs_to_s3.py
 airflow/providers/amazon/aws/transfers/glacier_to_gcs.py
 airflow/providers/amazon/aws/transfers/google_api_to_s3.py
@@ -122,35 +126,40 @@
 airflow/providers/amazon/aws/transfers/s3_to_redshift.py
 airflow/providers/amazon/aws/transfers/s3_to_sftp.py
 airflow/providers/amazon/aws/transfers/s3_to_sql.py
 airflow/providers/amazon/aws/transfers/salesforce_to_s3.py
 airflow/providers/amazon/aws/transfers/sftp_to_s3.py
 airflow/providers/amazon/aws/transfers/sql_to_s3.py
 airflow/providers/amazon/aws/triggers/__init__.py
+airflow/providers/amazon/aws/triggers/athena.py
 airflow/providers/amazon/aws/triggers/batch.py
 airflow/providers/amazon/aws/triggers/ec2.py
+airflow/providers/amazon/aws/triggers/ecs.py
 airflow/providers/amazon/aws/triggers/eks.py
 airflow/providers/amazon/aws/triggers/emr.py
 airflow/providers/amazon/aws/triggers/glue.py
 airflow/providers/amazon/aws/triggers/glue_crawler.py
+airflow/providers/amazon/aws/triggers/rds.py
 airflow/providers/amazon/aws/triggers/redshift_cluster.py
 airflow/providers/amazon/aws/triggers/s3.py
 airflow/providers/amazon/aws/triggers/sagemaker.py
 airflow/providers/amazon/aws/utils/__init__.py
 airflow/providers/amazon/aws/utils/connection_wrapper.py
 airflow/providers/amazon/aws/utils/eks_get_token.py
 airflow/providers/amazon/aws/utils/emailer.py
 airflow/providers/amazon/aws/utils/rds.py
 airflow/providers/amazon/aws/utils/redshift.py
 airflow/providers/amazon/aws/utils/sagemaker.py
 airflow/providers/amazon/aws/utils/tags.py
 airflow/providers/amazon/aws/utils/task_log_fetcher.py
 airflow/providers/amazon/aws/utils/waiter.py
+airflow/providers/amazon/aws/utils/waiter_with_logging.py
 airflow/providers/amazon/aws/waiters/__init__.py
 airflow/providers/amazon/aws/waiters/appflow.json
+airflow/providers/amazon/aws/waiters/athena.json
 airflow/providers/amazon/aws/waiters/base_waiter.py
 airflow/providers/amazon/aws/waiters/batch.json
 airflow/providers/amazon/aws/waiters/dynamodb.json
 airflow/providers/amazon/aws/waiters/ecs.json
 airflow/providers/amazon/aws/waiters/eks.json
 airflow/providers/amazon/aws/waiters/emr-containers.json
 airflow/providers/amazon/aws/waiters/emr-serverless.json
```

### Comparing `apache-airflow-providers-amazon-8.2.0rc1/apache_airflow_providers_amazon.egg-info/requires.txt` & `apache-airflow-providers-amazon-8.3.0rc1/apache_airflow_providers_amazon.egg-info/requires.txt`

 * *Files 6% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 apache-airflow-providers-common-sql>=1.3.1.dev0
+apache-airflow-providers-http
 apache-airflow>=2.4.0.dev0
 asgiref
 asgiref
 boto3>=1.24.0
 jsonpath_ng>=1.5.3
 mypy-boto3-appflow>=1.24.0
 mypy-boto3-rds>=1.24.0
@@ -15,31 +16,37 @@
 [aiobotocore]
 aiobotocore[boto3]>=2.2.0
 
 [apache.hive]
 apache-airflow-providers-apache-hive
 
 [cncf.kubernetes]
-apache-airflow-providers-cncf-kubernetes
+apache-airflow-providers-cncf-kubernetes>=7.2.0
 
 [common.sql]
 apache-airflow-providers-common-sql
 
 [exasol]
 apache-airflow-providers-exasol
 
 [ftp]
 apache-airflow-providers-ftp
 
 [google]
 apache-airflow-providers-google
 
+[http]
+apache-airflow-providers-http
+
 [imap]
 apache-airflow-providers-imap
 
+[microsoft.azure]
+apache-airflow-providers-microsoft-azure
+
 [mongo]
 apache-airflow-providers-mongo
 
 [pandas]
 pandas>=0.17.1
 
 [salesforce]
```

### Comparing `apache-airflow-providers-amazon-8.2.0rc1/pyproject.toml` & `apache-airflow-providers-amazon-8.3.0rc1/pyproject.toml`

 * *Files 5% similar despite different names*

```diff
@@ -13,19 +13,21 @@
 # "AS IS" BASIS, WITHOUT WARRANTIES OR CONDITIONS OF ANY
 # KIND, either express or implied.  See the License for the
 # specific language governing permissions and limitations
 # under the License.
 [tool.black]
 line-length = 110
 target-version = ['py37', 'py38', 'py39', 'py310']
-# The build system section is needed in order to workaround the side-effect introduced by recent
-# setup tools version. The recent setuptools version update (64.0.0) broke paths of editable installations
-# and we have to pin it to 63.4.3 version
-# The problem is tracked (and this limitation might be removed if it is solved) in:
-# https://github.com/pypa/setuptools/issues/3548
+
+# Editable installs are currently broken using setuptools 64.0.0 and above. The problem is tracked in
+# https://github.com/pypa/setuptools/issues/3548. We're also discussing how we could potentially fix
+# this problem on our end in issue https://github.com/apache/airflow/issues/30764. Until then we need
+# to use one of the following workarounds locally for editable installs:
+# 1) Pin setuptools <= 63.4.3 below in the [build-system] section.
+# 2) Include your airflow source code directory in PYTHONPATH.
 [build-system]
 requires = ['setuptools==67.2.0']
 build-backend = "setuptools.build_meta"
 
 [project]
 requires-python = ">=3.8"
```

### Comparing `apache-airflow-providers-amazon-8.2.0rc1/setup.cfg` & `apache-airflow-providers-amazon-8.3.0rc1/setup.cfg`

 * *Files 19% similar despite different names*

```diff
@@ -23,15 +23,16 @@
 	License :: OSI Approved :: Apache Software License
 	Programming Language :: Python :: 3.8
 	Programming Language :: Python :: 3.9
 	Programming Language :: Python :: 3.10
 	Programming Language :: Python :: 3.11
 	Topic :: System :: Monitoring
 project_urls = 
-	Documentation=https://airflow.apache.org/docs/apache-airflow-providers-amazon/8.2.0/
+	Documentation=https://airflow.apache.org/docs/apache-airflow-providers-amazon/8.3.0/
+	Changelog=https://airflow.apache.org/docs/apache-airflow-providers-amazon/8.3.0/changelog.html
 	Bug Tracker=https://github.com/apache/airflow/issues
 	Source Code=https://github.com/apache/airflow
 	Slack Chat=https://s.apache.org/airflow-slack
 	Twitter=https://twitter.com/ApacheAirflow
 	YouTube=https://www.youtube.com/channel/UCSXwxpWZQ7XZ1WL3wqevChA/
 
 [bdist_wheel]
@@ -43,14 +44,15 @@
 python_requires = ~=3.8
 packages = find:
 setup_requires = 
 	setuptools
 	wheel
 install_requires = 
 	apache-airflow-providers-common-sql>=1.3.1.dev0
+	apache-airflow-providers-http
 	apache-airflow>=2.4.0.dev0
 	asgiref
 	asgiref
 	boto3>=1.24.0
 	jsonpath_ng>=1.5.3
 	mypy-boto3-appflow>=1.24.0
 	mypy-boto3-rds>=1.24.0
```

### Comparing `apache-airflow-providers-amazon-8.2.0rc1/setup.py` & `apache-airflow-providers-amazon-8.3.0rc1/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -22,29 +22,31 @@
 # IF YOU WANT TO MODIFY IT, YOU SHOULD MODIFY THE TEMPLATE
 # `SETUP_TEMPLATE.py.jinja2` IN the `dev/provider_packages` DIRECTORY
 
 """Setup.py for the apache-airflow-providers-amazon package."""
 
 from setuptools import find_namespace_packages, setup
 
-version = "8.2.0"
+version = "8.3.0"
 
 
 def do_setup():
     """Perform the package apache-airflow-providers-amazon setup."""
     setup(
         version=version,
         extras_require={
             "apache.hive": ["apache-airflow-providers-apache-hive"],
-            "cncf.kubernetes": ["apache-airflow-providers-cncf-kubernetes"],
+            "cncf.kubernetes": ["apache-airflow-providers-cncf-kubernetes>=7.2.0"],
             "common.sql": ["apache-airflow-providers-common-sql"],
             "exasol": ["apache-airflow-providers-exasol"],
             "ftp": ["apache-airflow-providers-ftp"],
             "google": ["apache-airflow-providers-google"],
+            "http": ["apache-airflow-providers-http"],
             "imap": ["apache-airflow-providers-imap"],
+            "microsoft.azure": ["apache-airflow-providers-microsoft-azure"],
             "mongo": ["apache-airflow-providers-mongo"],
             "salesforce": ["apache-airflow-providers-salesforce"],
             "ssh": ["apache-airflow-providers-ssh"],
             "pandas": ["pandas>=0.17.1"],
             "aiobotocore": ["aiobotocore[boto3]>=2.2.0"],
         },
         packages=find_namespace_packages(
```

