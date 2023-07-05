# Comparing `tmp/yyxx_game_pkg-2023.6.9.1.tar.gz` & `tmp/yyxx_game_pkg-2023.7.5.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "yyxx_game_pkg-2023.6.9.1.tar", max compression
+gzip compressed data, was "yyxx_game_pkg-2023.7.5.1.tar", max compression
```

## Comparing `yyxx_game_pkg-2023.6.9.1.tar` & `yyxx_game_pkg-2023.7.5.1.tar`

### file list

```diff
@@ -1,114 +1,121 @@
--rw-r--r--   0        0        0     4895 2023-06-09 02:30:09.482693 yyxx_game_pkg-2023.6.9.1/README.md
--rw-r--r--   0        0        0     1790 2023-06-09 02:30:25.342831 yyxx_game_pkg-2023.6.9.1/pyproject.toml
--rw-r--r--   0        0        0       68 2023-06-09 02:30:09.482693 yyxx_game_pkg-2023.6.9.1/tests/__init__.py
--rw-r--r--   0        0        0       83 2023-06-09 02:30:09.482693 yyxx_game_pkg-2023.6.9.1/tests/dbops/__init__.py
--rw-r--r--   0        0        0     1341 2023-06-09 02:30:09.482693 yyxx_game_pkg-2023.6.9.1/tests/dbops/mysql_op.py
--rw-r--r--   0        0        0       70 2023-06-09 02:30:09.482693 yyxx_game_pkg-2023.6.9.1/tests/dispatch/__init__.py
--rw-r--r--   0        0        0       70 2023-06-09 02:30:09.482693 yyxx_game_pkg-2023.6.9.1/tests/dispatch/config/__init__.py
--rw-r--r--   0        0        0     1228 2023-06-09 02:30:09.482693 yyxx_game_pkg-2023.6.9.1/tests/dispatch/config/celery_local_config.py
--rw-r--r--   0        0        0      660 2023-06-09 02:30:09.482693 yyxx_game_pkg-2023.6.9.1/tests/dispatch/rules/__init__.py
--rw-r--r--   0        0        0     1348 2023-06-09 02:30:09.482693 yyxx_game_pkg-2023.6.9.1/tests/dispatch/rules/rule_temp.py
--rw-r--r--   0        0        0      580 2023-06-09 02:30:09.482693 yyxx_game_pkg-2023.6.9.1/tests/dispatch/test_dispatch.py
--rw-r--r--   0        0        0       84 2023-06-09 02:30:09.482693 yyxx_game_pkg-2023.6.9.1/tests/helpers/__init__.py
--rw-r--r--   0        0        0      522 2023-06-09 02:30:09.482693 yyxx_game_pkg-2023.6.9.1/tests/helpers/test_mysql_helper.py
--rw-r--r--   0        0        0      455 2023-06-09 02:30:09.482693 yyxx_game_pkg-2023.6.9.1/tests/helpers/test_pika_helper.py
--rw-r--r--   0        0        0      481 2023-06-09 02:30:09.482693 yyxx_game_pkg-2023.6.9.1/tests/helpers/test_redis_helper.py
--rw-r--r--   0        0        0       70 2023-06-09 02:30:09.482693 yyxx_game_pkg-2023.6.9.1/tests/submit/__init__.py
--rw-r--r--   0        0        0       70 2023-06-09 02:30:09.482693 yyxx_game_pkg-2023.6.9.1/tests/submit/schedule_rule/__init__.py
--rw-r--r--   0        0        0       70 2023-06-09 02:30:09.482693 yyxx_game_pkg-2023.6.9.1/tests/submit/schedule_rule/schedule/__init__.py
--rw-r--r--   0        0        0       70 2023-06-09 02:30:09.482693 yyxx_game_pkg-2023.6.9.1/tests/submit/schedule_rule/schedule/statistic_task/__init__.py
--rw-r--r--   0        0        0      431 2023-06-09 02:30:09.482693 yyxx_game_pkg-2023.6.9.1/tests/submit/schedule_rule/schedule/statistic_task/schedule_statistic_collect_test.py
--rw-r--r--   0        0        0      413 2023-06-09 02:30:09.482693 yyxx_game_pkg-2023.6.9.1/tests/submit/schedule_rule/schedule/statistic_task/schedule_statistic_task_test.py
--rw-r--r--   0        0        0       70 2023-06-09 02:30:09.482693 yyxx_game_pkg-2023.6.9.1/tests/submit/schedule_rule/schedule/work_flow/__init__.py
--rw-r--r--   0        0        0     1217 2023-06-09 02:30:09.482693 yyxx_game_pkg-2023.6.9.1/tests/submit/schedule_rule/schedule/work_flow/schedule_work_flow_test.py
--rw-r--r--   0        0        0      305 2023-06-09 02:30:09.482693 yyxx_game_pkg-2023.6.9.1/tests/submit/submit.json
--rw-r--r--   0        0        0     1250 2023-06-09 02:30:09.482693 yyxx_game_pkg-2023.6.9.1/tests/submit/test_submit.py
--rw-r--r--   0        0        0      235 2023-06-09 02:30:09.482693 yyxx_game_pkg-2023.6.9.1/tests/test_ip2region.py
--rw-r--r--   0        0        0      513 2023-06-09 02:30:09.482693 yyxx_game_pkg-2023.6.9.1/tests/test_logger.py
--rw-r--r--   0        0        0      960 2023-06-09 02:30:09.482693 yyxx_game_pkg-2023.6.9.1/tests/test_xtrace.py
--rw-r--r--   0        0        0       81 2023-06-09 02:30:09.482693 yyxx_game_pkg-2023.6.9.1/tests/utils/__init__.py
--rw-r--r--   0        0        0       70 2023-06-09 02:30:09.482693 yyxx_game_pkg-2023.6.9.1/tests/xcelery/__init__.py
--rw-r--r--   0        0        0       70 2023-06-09 02:30:09.482693 yyxx_game_pkg-2023.6.9.1/tests/xcelery/config/__init__.py
--rw-r--r--   0        0        0     1226 2023-06-09 02:30:09.482693 yyxx_game_pkg-2023.6.9.1/tests/xcelery/config/celery_local_config.py
--rw-r--r--   0        0        0      747 2023-06-09 02:30:09.482693 yyxx_game_pkg-2023.6.9.1/tests/xcelery/task_register.py
--rw-r--r--   0        0        0      299 2023-06-09 02:30:09.482693 yyxx_game_pkg-2023.6.9.1/tests/xcelery/test_celery.py
--rw-r--r--   0        0        0       69 2023-06-09 02:30:09.482693 yyxx_game_pkg-2023.6.9.1/yyxx_game_pkg/__init__.py
--rw-r--r--   0        0        0      124 2023-06-09 02:30:09.486693 yyxx_game_pkg-2023.6.9.1/yyxx_game_pkg/center_api/__init__.py
--rw-r--r--   0        0        0     5166 2023-06-09 02:30:09.486693 yyxx_game_pkg-2023.6.9.1/yyxx_game_pkg/center_api/model/Operator.py
--rw-r--r--   0        0        0     1505 2023-06-09 02:30:09.486693 yyxx_game_pkg-2023.6.9.1/yyxx_game_pkg/center_api/model/OperatorServer.py
--rw-r--r--   0        0        0     2572 2023-06-09 02:30:09.486693 yyxx_game_pkg-2023.6.9.1/yyxx_game_pkg/center_api/model/RechargeConfig.py
--rw-r--r--   0        0        0     2600 2023-06-09 02:30:09.486693 yyxx_game_pkg-2023.6.9.1/yyxx_game_pkg/center_api/model/TableFieldConf.py
--rw-r--r--   0        0        0      124 2023-06-09 02:30:09.486693 yyxx_game_pkg-2023.6.9.1/yyxx_game_pkg/center_api/model/__init__.py
--rw-r--r--   0        0        0      124 2023-06-09 02:30:09.486693 yyxx_game_pkg-2023.6.9.1/yyxx_game_pkg/center_api/sdk/__init__.py
--rw-r--r--   0        0        0     4378 2023-06-09 02:30:09.486693 yyxx_game_pkg-2023.6.9.1/yyxx_game_pkg/center_api/sdk/check_token.py
--rw-r--r--   0        0        0     5897 2023-06-09 02:30:09.486693 yyxx_game_pkg-2023.6.9.1/yyxx_game_pkg/center_api/sdk/map_core.py
--rw-r--r--   0        0        0     3335 2023-06-09 02:30:09.486693 yyxx_game_pkg-2023.6.9.1/yyxx_game_pkg/center_api/sdk/recharge.py
--rw-r--r--   0        0        0     6894 2023-06-09 02:30:09.486693 yyxx_game_pkg-2023.6.9.1/yyxx_game_pkg/conf/__init__.py
--rw-r--r--   0        0        0     2053 2023-06-09 02:30:09.486693 yyxx_game_pkg-2023.6.9.1/yyxx_game_pkg/conf/global_settings.py
--rw-r--r--   0        0        0      128 2023-06-09 02:30:09.486693 yyxx_game_pkg-2023.6.9.1/yyxx_game_pkg/crypto/__init__.py
--rw-r--r--   0        0        0     1164 2023-06-09 02:30:09.486693 yyxx_game_pkg-2023.6.9.1/yyxx_game_pkg/crypto/aes.py
--rw-r--r--   0        0        0     1113 2023-06-09 02:30:09.486693 yyxx_game_pkg-2023.6.9.1/yyxx_game_pkg/crypto/basic.py
--rw-r--r--   0        0        0     1344 2023-06-09 02:30:09.486693 yyxx_game_pkg-2023.6.9.1/yyxx_game_pkg/crypto/make_sign.py
--rw-r--r--   0        0        0     2652 2023-06-09 02:30:09.486693 yyxx_game_pkg-2023.6.9.1/yyxx_game_pkg/crypto/rsa.py
--rw-r--r--   0        0        0       83 2023-06-09 02:30:09.486693 yyxx_game_pkg-2023.6.9.1/yyxx_game_pkg/dbops/__init__.py
--rw-r--r--   0        0        0     1331 2023-06-09 02:30:09.486693 yyxx_game_pkg-2023.6.9.1/yyxx_game_pkg/dbops/base.py
--rw-r--r--   0        0        0     1304 2023-06-09 02:30:09.486693 yyxx_game_pkg-2023.6.9.1/yyxx_game_pkg/dbops/ch_op.py
--rw-r--r--   0        0        0     5596 2023-06-09 02:30:09.486693 yyxx_game_pkg-2023.6.9.1/yyxx_game_pkg/dbops/das_api.py
--rw-r--r--   0        0        0     1911 2023-06-09 02:30:09.486693 yyxx_game_pkg-2023.6.9.1/yyxx_game_pkg/dbops/es_op.py
--rw-r--r--   0        0        0     1678 2023-06-09 02:30:09.486693 yyxx_game_pkg-2023.6.9.1/yyxx_game_pkg/dbops/hdfs_op.py
--rw-r--r--   0        0        0      979 2023-06-09 02:30:09.486693 yyxx_game_pkg-2023.6.9.1/yyxx_game_pkg/dbops/mongo_op.py
--rw-r--r--   0        0        0     3955 2023-06-09 02:30:09.486693 yyxx_game_pkg-2023.6.9.1/yyxx_game_pkg/dbops/mysql_op.py
--rw-r--r--   0        0        0       81 2023-06-09 02:30:09.486693 yyxx_game_pkg-2023.6.9.1/yyxx_game_pkg/helpers/__init__.py
--rw-r--r--   0        0        0     2686 2023-06-09 02:30:09.486693 yyxx_game_pkg-2023.6.9.1/yyxx_game_pkg/helpers/mysql_helper.py
--rw-r--r--   0        0        0     3215 2023-06-09 02:30:09.486693 yyxx_game_pkg-2023.6.9.1/yyxx_game_pkg/helpers/op_helper.py
--rw-r--r--   0        0        0     1266 2023-06-09 02:30:09.486693 yyxx_game_pkg-2023.6.9.1/yyxx_game_pkg/helpers/pika_helper.py
--rw-r--r--   0        0        0     2966 2023-06-09 02:30:09.486693 yyxx_game_pkg-2023.6.9.1/yyxx_game_pkg/helpers/redis_helper.py
--rw-r--r--   0        0        0       79 2023-06-09 02:30:09.486693 yyxx_game_pkg-2023.6.9.1/yyxx_game_pkg/ip2region/__init__.py
--rw-r--r--   0        0        0 11070130 2023-06-09 02:30:09.562694 yyxx_game_pkg-2023.6.9.1/yyxx_game_pkg/ip2region/ip2region.xdb
--rw-r--r--   0        0        0      604 2023-06-09 02:30:09.566694 yyxx_game_pkg-2023.6.9.1/yyxx_game_pkg/ip2region/ip_x.py
--rw-r--r--   0        0        0     5735 2023-06-09 02:30:09.566694 yyxx_game_pkg-2023.6.9.1/yyxx_game_pkg/ip2region/xdbSearcher.py
--rw-r--r--   0        0        0       81 2023-06-09 02:30:09.566694 yyxx_game_pkg-2023.6.9.1/yyxx_game_pkg/logger/__init__.py
--rw-r--r--   0        0        0     2326 2023-06-09 02:30:09.566694 yyxx_game_pkg-2023.6.9.1/yyxx_game_pkg/logger/config.py
--rw-r--r--   0        0        0     3467 2023-06-09 02:30:09.566694 yyxx_game_pkg-2023.6.9.1/yyxx_game_pkg/logger/handlers.py
--rw-r--r--   0        0        0     2154 2023-06-09 02:30:09.566694 yyxx_game_pkg-2023.6.9.1/yyxx_game_pkg/logger/log.py
--rw-r--r--   0        0        0       70 2023-06-09 02:30:09.566694 yyxx_game_pkg-2023.6.9.1/yyxx_game_pkg/stat/__init__.py
--rw-r--r--   0        0        0       68 2023-06-09 02:30:09.566694 yyxx_game_pkg-2023.6.9.1/yyxx_game_pkg/stat/dispatch/__init__.py
--rw-r--r--   0        0        0       70 2023-06-09 02:30:09.566694 yyxx_game_pkg-2023.6.9.1/yyxx_game_pkg/stat/dispatch/common/__init__.py
--rw-r--r--   0        0        0     1514 2023-06-09 02:30:09.566694 yyxx_game_pkg-2023.6.9.1/yyxx_game_pkg/stat/dispatch/common/common.py
--rw-r--r--   0        0        0       69 2023-06-09 02:30:09.566694 yyxx_game_pkg-2023.6.9.1/yyxx_game_pkg/stat/dispatch/core/__init__.py
--rw-r--r--   0        0        0      805 2023-06-09 02:30:09.566694 yyxx_game_pkg-2023.6.9.1/yyxx_game_pkg/stat/dispatch/core/manager.py
--rw-r--r--   0        0        0     1042 2023-06-09 02:30:09.566694 yyxx_game_pkg-2023.6.9.1/yyxx_game_pkg/stat/dispatch/core/structs.py
--rw-r--r--   0        0        0     5533 2023-06-09 02:30:09.566694 yyxx_game_pkg-2023.6.9.1/yyxx_game_pkg/stat/dispatch/core/workflows.py
--rw-r--r--   0        0        0      604 2023-06-09 02:30:09.566694 yyxx_game_pkg-2023.6.9.1/yyxx_game_pkg/stat/dispatch/dispatch.py
--rw-r--r--   0        0        0       70 2023-06-09 02:30:09.566694 yyxx_game_pkg-2023.6.9.1/yyxx_game_pkg/stat/dispatch/logic/__init__.py
--rw-r--r--   0        0        0     4402 2023-06-09 02:30:09.566694 yyxx_game_pkg-2023.6.9.1/yyxx_game_pkg/stat/dispatch/logic/task_logic.py
--rw-r--r--   0        0        0      809 2023-06-09 02:30:09.566694 yyxx_game_pkg-2023.6.9.1/yyxx_game_pkg/stat/dispatch/route.py
--rw-r--r--   0        0        0      677 2023-06-09 02:30:09.566694 yyxx_game_pkg-2023.6.9.1/yyxx_game_pkg/stat/dispatch/rules/__init__.py
--rw-r--r--   0        0        0      689 2023-06-09 02:30:09.566694 yyxx_game_pkg-2023.6.9.1/yyxx_game_pkg/stat/dispatch/rules/rule_base.py
--rw-r--r--   0        0        0     4270 2023-06-09 02:30:09.566694 yyxx_game_pkg-2023.6.9.1/yyxx_game_pkg/stat/dispatch/rules/rule_workflow.py
--rw-r--r--   0        0        0      667 2023-06-09 02:30:09.566694 yyxx_game_pkg-2023.6.9.1/yyxx_game_pkg/stat/log.py
--rw-r--r--   0        0        0       70 2023-06-09 02:30:09.566694 yyxx_game_pkg-2023.6.9.1/yyxx_game_pkg/stat/submit/__init__.py
--rw-r--r--   0        0        0       70 2023-06-09 02:30:09.566694 yyxx_game_pkg-2023.6.9.1/yyxx_game_pkg/stat/submit/logic/__init__.py
--rw-r--r--   0        0        0     5961 2023-06-09 02:30:09.566694 yyxx_game_pkg-2023.6.9.1/yyxx_game_pkg/stat/submit/logic/submit_logic.py
--rw-r--r--   0        0        0      987 2023-06-09 02:30:09.566694 yyxx_game_pkg-2023.6.9.1/yyxx_game_pkg/stat/submit/submit.py
--rw-r--r--   0        0        0       70 2023-06-09 02:30:09.566694 yyxx_game_pkg-2023.6.9.1/yyxx_game_pkg/stat/xcelery/__init__.py
--rw-r--r--   0        0        0     2206 2023-06-09 02:30:09.566694 yyxx_game_pkg-2023.6.9.1/yyxx_game_pkg/stat/xcelery/instance.py
--rw-r--r--   0        0        0     1183 2023-06-09 02:30:09.566694 yyxx_game_pkg-2023.6.9.1/yyxx_game_pkg/stat/xcelery/task_base.py
--rw-r--r--   0        0        0      428 2023-06-09 02:30:09.566694 yyxx_game_pkg-2023.6.9.1/yyxx_game_pkg/template/__init__.py
--rw-r--r--   0        0        0      132 2023-06-09 02:30:09.566694 yyxx_game_pkg-2023.6.9.1/yyxx_game_pkg/template/sdk/cookiecutter.json
--rw-r--r--   0        0        0     3930 2023-06-09 02:30:09.566694 yyxx_game_pkg-2023.6.9.1/yyxx_game_pkg/template/sdk/sdk_{{cookiecutter.sdk_name}}/check_token.py
--rw-r--r--   0        0        0      624 2023-06-09 02:30:09.566694 yyxx_game_pkg-2023.6.9.1/yyxx_game_pkg/template/sdk/sdk_{{cookiecutter.sdk_name}}/map_factor.py
--rw-r--r--   0        0        0     4027 2023-06-09 02:30:09.566694 yyxx_game_pkg-2023.6.9.1/yyxx_game_pkg/template/sdk/sdk_{{cookiecutter.sdk_name}}/recharge.py
--rw-r--r--   0        0        0       83 2023-06-09 02:30:09.566694 yyxx_game_pkg-2023.6.9.1/yyxx_game_pkg/utils/__init__.py
--rw-r--r--   0        0        0     5652 2023-06-09 02:30:09.566694 yyxx_game_pkg-2023.6.9.1/yyxx_game_pkg/utils/decorator.py
--rw-r--r--   0        0        0     3135 2023-06-09 02:30:09.566694 yyxx_game_pkg-2023.6.9.1/yyxx_game_pkg/utils/error_code.py
--rw-r--r--   0        0        0     2845 2023-06-09 02:30:09.566694 yyxx_game_pkg-2023.6.9.1/yyxx_game_pkg/utils/profiler.py
--rw-r--r--   0        0        0     3068 2023-06-09 02:30:09.566694 yyxx_game_pkg-2023.6.9.1/yyxx_game_pkg/utils/xListStr.py
--rw-r--r--   0        0        0     8580 2023-06-09 02:30:09.566694 yyxx_game_pkg-2023.6.9.1/yyxx_game_pkg/utils/xdataframe.py
--rw-r--r--   0        0        0     7441 2023-06-09 02:30:09.566694 yyxx_game_pkg-2023.6.9.1/yyxx_game_pkg/utils/xdate.py
--rw-r--r--   0        0        0     3653 2023-06-09 02:30:09.566694 yyxx_game_pkg-2023.6.9.1/yyxx_game_pkg/utils/xhttp.py
--rw-r--r--   0        0        0      971 2023-06-09 02:30:09.566694 yyxx_game_pkg-2023.6.9.1/yyxx_game_pkg/utils/xmath.py
--rw-r--r--   0        0        0      573 2023-06-09 02:30:09.566694 yyxx_game_pkg-2023.6.9.1/yyxx_game_pkg/utils/xstring.py
--rw-r--r--   0        0        0       69 2023-06-09 02:30:09.566694 yyxx_game_pkg-2023.6.9.1/yyxx_game_pkg/xtrace/__init__.py
--rw-r--r--   0        0        0     2858 2023-06-09 02:30:09.566694 yyxx_game_pkg-2023.6.9.1/yyxx_game_pkg/xtrace/helper.py
--rw-r--r--   0        0        0     6857 1970-01-01 00:00:00.000000 yyxx_game_pkg-2023.6.9.1/PKG-INFO
+-rw-r--r--   0        0        0     4895 2023-07-05 02:24:17.245787 yyxx_game_pkg-2023.7.5.1/README.md
+-rw-r--r--   0        0        0     1875 2023-07-05 02:24:30.225732 yyxx_game_pkg-2023.7.5.1/pyproject.toml
+-rw-r--r--   0        0        0       68 2023-07-05 02:24:17.249786 yyxx_game_pkg-2023.7.5.1/tests/__init__.py
+-rw-r--r--   0        0        0       83 2023-07-05 02:24:17.249786 yyxx_game_pkg-2023.7.5.1/tests/dbops/__init__.py
+-rw-r--r--   0        0        0     1341 2023-07-05 02:24:17.249786 yyxx_game_pkg-2023.7.5.1/tests/dbops/mysql_op.py
+-rw-r--r--   0        0        0       70 2023-07-05 02:24:17.249786 yyxx_game_pkg-2023.7.5.1/tests/dispatch/__init__.py
+-rw-r--r--   0        0        0       70 2023-07-05 02:24:17.249786 yyxx_game_pkg-2023.7.5.1/tests/dispatch/config/__init__.py
+-rw-r--r--   0        0        0     1228 2023-07-05 02:24:17.249786 yyxx_game_pkg-2023.7.5.1/tests/dispatch/config/celery_local_config.py
+-rw-r--r--   0        0        0      660 2023-07-05 02:24:17.249786 yyxx_game_pkg-2023.7.5.1/tests/dispatch/rules/__init__.py
+-rw-r--r--   0        0        0     1348 2023-07-05 02:24:17.249786 yyxx_game_pkg-2023.7.5.1/tests/dispatch/rules/rule_temp.py
+-rw-r--r--   0        0        0      580 2023-07-05 02:24:17.249786 yyxx_game_pkg-2023.7.5.1/tests/dispatch/test_dispatch.py
+-rw-r--r--   0        0        0       84 2023-07-05 02:24:17.249786 yyxx_game_pkg-2023.7.5.1/tests/helpers/__init__.py
+-rw-r--r--   0        0        0      522 2023-07-05 02:24:17.249786 yyxx_game_pkg-2023.7.5.1/tests/helpers/test_mysql_helper.py
+-rw-r--r--   0        0        0      455 2023-07-05 02:24:17.249786 yyxx_game_pkg-2023.7.5.1/tests/helpers/test_pika_helper.py
+-rw-r--r--   0        0        0      481 2023-07-05 02:24:17.249786 yyxx_game_pkg-2023.7.5.1/tests/helpers/test_redis_helper.py
+-rw-r--r--   0        0        0       70 2023-07-05 02:24:17.249786 yyxx_game_pkg-2023.7.5.1/tests/submit/__init__.py
+-rw-r--r--   0        0        0       70 2023-07-05 02:24:17.249786 yyxx_game_pkg-2023.7.5.1/tests/submit/schedule_rule/__init__.py
+-rw-r--r--   0        0        0       70 2023-07-05 02:24:17.249786 yyxx_game_pkg-2023.7.5.1/tests/submit/schedule_rule/schedule/__init__.py
+-rw-r--r--   0        0        0       70 2023-07-05 02:24:17.249786 yyxx_game_pkg-2023.7.5.1/tests/submit/schedule_rule/schedule/statistic_task/__init__.py
+-rw-r--r--   0        0        0      431 2023-07-05 02:24:17.249786 yyxx_game_pkg-2023.7.5.1/tests/submit/schedule_rule/schedule/statistic_task/schedule_statistic_collect_test.py
+-rw-r--r--   0        0        0      413 2023-07-05 02:24:17.249786 yyxx_game_pkg-2023.7.5.1/tests/submit/schedule_rule/schedule/statistic_task/schedule_statistic_task_test.py
+-rw-r--r--   0        0        0       70 2023-07-05 02:24:17.249786 yyxx_game_pkg-2023.7.5.1/tests/submit/schedule_rule/schedule/work_flow/__init__.py
+-rw-r--r--   0        0        0     1217 2023-07-05 02:24:17.249786 yyxx_game_pkg-2023.7.5.1/tests/submit/schedule_rule/schedule/work_flow/schedule_work_flow_test.py
+-rw-r--r--   0        0        0      305 2023-07-05 02:24:17.249786 yyxx_game_pkg-2023.7.5.1/tests/submit/submit.json
+-rw-r--r--   0        0        0     1250 2023-07-05 02:24:17.249786 yyxx_game_pkg-2023.7.5.1/tests/submit/test_submit.py
+-rw-r--r--   0        0        0      235 2023-07-05 02:24:17.249786 yyxx_game_pkg-2023.7.5.1/tests/test_ip2region.py
+-rw-r--r--   0        0        0      513 2023-07-05 02:24:17.249786 yyxx_game_pkg-2023.7.5.1/tests/test_logger.py
+-rw-r--r--   0        0        0      960 2023-07-05 02:24:17.249786 yyxx_game_pkg-2023.7.5.1/tests/test_xtrace.py
+-rw-r--r--   0        0        0       81 2023-07-05 02:24:17.249786 yyxx_game_pkg-2023.7.5.1/tests/utils/__init__.py
+-rw-r--r--   0        0        0       70 2023-07-05 02:24:17.249786 yyxx_game_pkg-2023.7.5.1/tests/xcelery/__init__.py
+-rw-r--r--   0        0        0       70 2023-07-05 02:24:17.249786 yyxx_game_pkg-2023.7.5.1/tests/xcelery/config/__init__.py
+-rw-r--r--   0        0        0     1226 2023-07-05 02:24:17.249786 yyxx_game_pkg-2023.7.5.1/tests/xcelery/config/celery_local_config.py
+-rw-r--r--   0        0        0      747 2023-07-05 02:24:17.249786 yyxx_game_pkg-2023.7.5.1/tests/xcelery/task_register.py
+-rw-r--r--   0        0        0      299 2023-07-05 02:24:17.249786 yyxx_game_pkg-2023.7.5.1/tests/xcelery/test_celery.py
+-rw-r--r--   0        0        0       69 2023-07-05 02:24:17.249786 yyxx_game_pkg-2023.7.5.1/yyxx_game_pkg/__init__.py
+-rw-r--r--   0        0        0      124 2023-07-05 02:24:17.249786 yyxx_game_pkg-2023.7.5.1/yyxx_game_pkg/center_api/__init__.py
+-rw-r--r--   0        0        0     5166 2023-07-05 02:24:17.249786 yyxx_game_pkg-2023.7.5.1/yyxx_game_pkg/center_api/model/Operator.py
+-rw-r--r--   0        0        0     1505 2023-07-05 02:24:17.249786 yyxx_game_pkg-2023.7.5.1/yyxx_game_pkg/center_api/model/OperatorServer.py
+-rw-r--r--   0        0        0     2572 2023-07-05 02:24:17.249786 yyxx_game_pkg-2023.7.5.1/yyxx_game_pkg/center_api/model/RechargeConfig.py
+-rw-r--r--   0        0        0     2600 2023-07-05 02:24:17.249786 yyxx_game_pkg-2023.7.5.1/yyxx_game_pkg/center_api/model/TableFieldConf.py
+-rw-r--r--   0        0        0      124 2023-07-05 02:24:17.249786 yyxx_game_pkg-2023.7.5.1/yyxx_game_pkg/center_api/model/__init__.py
+-rw-r--r--   0        0        0      124 2023-07-05 02:24:17.249786 yyxx_game_pkg-2023.7.5.1/yyxx_game_pkg/center_api/sdk/__init__.py
+-rw-r--r--   0        0        0     4353 2023-07-05 02:24:17.249786 yyxx_game_pkg-2023.7.5.1/yyxx_game_pkg/center_api/sdk/check_token.py
+-rw-r--r--   0        0        0     5805 2023-07-05 02:24:17.253786 yyxx_game_pkg-2023.7.5.1/yyxx_game_pkg/center_api/sdk/map_core.py
+-rw-r--r--   0        0        0     3506 2023-07-05 02:24:17.253786 yyxx_game_pkg-2023.7.5.1/yyxx_game_pkg/center_api/sdk/recharge.py
+-rw-r--r--   0        0        0     6894 2023-07-05 02:24:17.253786 yyxx_game_pkg-2023.7.5.1/yyxx_game_pkg/conf/__init__.py
+-rw-r--r--   0        0        0     2053 2023-07-05 02:24:17.253786 yyxx_game_pkg-2023.7.5.1/yyxx_game_pkg/conf/global_settings.py
+-rw-r--r--   0        0        0      128 2023-07-05 02:24:17.253786 yyxx_game_pkg-2023.7.5.1/yyxx_game_pkg/crypto/__init__.py
+-rw-r--r--   0        0        0     1164 2023-07-05 02:24:17.253786 yyxx_game_pkg-2023.7.5.1/yyxx_game_pkg/crypto/aes.py
+-rw-r--r--   0        0        0     1113 2023-07-05 02:24:17.253786 yyxx_game_pkg-2023.7.5.1/yyxx_game_pkg/crypto/basic.py
+-rw-r--r--   0        0        0     1351 2023-07-05 02:24:17.253786 yyxx_game_pkg-2023.7.5.1/yyxx_game_pkg/crypto/make_sign.py
+-rw-r--r--   0        0        0     2652 2023-07-05 02:24:17.253786 yyxx_game_pkg-2023.7.5.1/yyxx_game_pkg/crypto/rsa.py
+-rw-r--r--   0        0        0       83 2023-07-05 02:24:17.253786 yyxx_game_pkg-2023.7.5.1/yyxx_game_pkg/dbops/__init__.py
+-rw-r--r--   0        0        0     1331 2023-07-05 02:24:17.253786 yyxx_game_pkg-2023.7.5.1/yyxx_game_pkg/dbops/base.py
+-rw-r--r--   0        0        0     1304 2023-07-05 02:24:17.253786 yyxx_game_pkg-2023.7.5.1/yyxx_game_pkg/dbops/ch_op.py
+-rw-r--r--   0        0        0     5596 2023-07-05 02:24:17.253786 yyxx_game_pkg-2023.7.5.1/yyxx_game_pkg/dbops/das_api.py
+-rw-r--r--   0        0        0     1911 2023-07-05 02:24:17.253786 yyxx_game_pkg-2023.7.5.1/yyxx_game_pkg/dbops/es_op.py
+-rw-r--r--   0        0        0     1678 2023-07-05 02:24:17.253786 yyxx_game_pkg-2023.7.5.1/yyxx_game_pkg/dbops/hdfs_op.py
+-rw-r--r--   0        0        0       83 2023-07-05 02:24:17.253786 yyxx_game_pkg-2023.7.5.1/yyxx_game_pkg/dbops/mongo_op/__init__.py
+-rw-r--r--   0        0        0     3479 2023-07-05 02:24:17.253786 yyxx_game_pkg-2023.7.5.1/yyxx_game_pkg/dbops/mongo_op/mongo_op.py
+-rw-r--r--   0        0        0      326 2023-07-05 02:24:17.253786 yyxx_game_pkg-2023.7.5.1/yyxx_game_pkg/dbops/mongo_op/sql2mongo/__init__.py
+-rw-r--r--   0        0        0    10692 2023-07-05 02:24:17.253786 yyxx_game_pkg-2023.7.5.1/yyxx_game_pkg/dbops/mongo_op/sql2mongo/sql2mongo.py
+-rw-r--r--   0        0        0     7993 2023-07-05 02:24:17.253786 yyxx_game_pkg-2023.7.5.1/yyxx_game_pkg/dbops/mongo_op/sql2mongo/test.py
+-rw-r--r--   0        0        0     3955 2023-07-05 02:24:17.253786 yyxx_game_pkg-2023.7.5.1/yyxx_game_pkg/dbops/mysql_op.py
+-rw-r--r--   0        0        0       81 2023-07-05 02:24:17.253786 yyxx_game_pkg-2023.7.5.1/yyxx_game_pkg/helpers/__init__.py
+-rw-r--r--   0        0        0     2722 2023-07-05 02:24:17.253786 yyxx_game_pkg-2023.7.5.1/yyxx_game_pkg/helpers/mysql_helper.py
+-rw-r--r--   0        0        0     3215 2023-07-05 02:24:17.253786 yyxx_game_pkg-2023.7.5.1/yyxx_game_pkg/helpers/op_helper.py
+-rw-r--r--   0        0        0     1266 2023-07-05 02:24:17.253786 yyxx_game_pkg-2023.7.5.1/yyxx_game_pkg/helpers/pika_helper.py
+-rw-r--r--   0        0        0     2966 2023-07-05 02:24:17.253786 yyxx_game_pkg-2023.7.5.1/yyxx_game_pkg/helpers/redis_helper.py
+-rw-r--r--   0        0        0       79 2023-07-05 02:24:17.253786 yyxx_game_pkg-2023.7.5.1/yyxx_game_pkg/ip2region/__init__.py
+-rw-r--r--   0        0        0 11070130 2023-07-05 02:24:17.325786 yyxx_game_pkg-2023.7.5.1/yyxx_game_pkg/ip2region/ip2region.xdb
+-rw-r--r--   0        0        0      604 2023-07-05 02:24:17.325786 yyxx_game_pkg-2023.7.5.1/yyxx_game_pkg/ip2region/ip_x.py
+-rw-r--r--   0        0        0     5735 2023-07-05 02:24:17.325786 yyxx_game_pkg-2023.7.5.1/yyxx_game_pkg/ip2region/xdbSearcher.py
+-rw-r--r--   0        0        0       81 2023-07-05 02:24:17.325786 yyxx_game_pkg-2023.7.5.1/yyxx_game_pkg/logger/__init__.py
+-rw-r--r--   0        0        0     2326 2023-07-05 02:24:17.325786 yyxx_game_pkg-2023.7.5.1/yyxx_game_pkg/logger/config.py
+-rw-r--r--   0        0        0      666 2023-07-05 02:24:17.325786 yyxx_game_pkg-2023.7.5.1/yyxx_game_pkg/logger/formatters.py
+-rw-r--r--   0        0        0     3467 2023-07-05 02:24:17.325786 yyxx_game_pkg-2023.7.5.1/yyxx_game_pkg/logger/handlers.py
+-rw-r--r--   0        0        0     2154 2023-07-05 02:24:17.325786 yyxx_game_pkg-2023.7.5.1/yyxx_game_pkg/logger/log.py
+-rw-r--r--   0        0        0       70 2023-07-05 02:24:17.325786 yyxx_game_pkg-2023.7.5.1/yyxx_game_pkg/stat/__init__.py
+-rw-r--r--   0        0        0       68 2023-07-05 02:24:17.325786 yyxx_game_pkg-2023.7.5.1/yyxx_game_pkg/stat/dispatch/__init__.py
+-rw-r--r--   0        0        0       70 2023-07-05 02:24:17.325786 yyxx_game_pkg-2023.7.5.1/yyxx_game_pkg/stat/dispatch/common/__init__.py
+-rw-r--r--   0        0        0     1514 2023-07-05 02:24:17.325786 yyxx_game_pkg-2023.7.5.1/yyxx_game_pkg/stat/dispatch/common/common.py
+-rw-r--r--   0        0        0       69 2023-07-05 02:24:17.325786 yyxx_game_pkg-2023.7.5.1/yyxx_game_pkg/stat/dispatch/core/__init__.py
+-rw-r--r--   0        0        0      805 2023-07-05 02:24:17.325786 yyxx_game_pkg-2023.7.5.1/yyxx_game_pkg/stat/dispatch/core/manager.py
+-rw-r--r--   0        0        0     1042 2023-07-05 02:24:17.325786 yyxx_game_pkg-2023.7.5.1/yyxx_game_pkg/stat/dispatch/core/structs.py
+-rw-r--r--   0        0        0     5533 2023-07-05 02:24:17.325786 yyxx_game_pkg-2023.7.5.1/yyxx_game_pkg/stat/dispatch/core/workflows.py
+-rw-r--r--   0        0        0      604 2023-07-05 02:24:17.325786 yyxx_game_pkg-2023.7.5.1/yyxx_game_pkg/stat/dispatch/dispatch.py
+-rw-r--r--   0        0        0       70 2023-07-05 02:24:17.325786 yyxx_game_pkg-2023.7.5.1/yyxx_game_pkg/stat/dispatch/logic/__init__.py
+-rw-r--r--   0        0        0     4402 2023-07-05 02:24:17.325786 yyxx_game_pkg-2023.7.5.1/yyxx_game_pkg/stat/dispatch/logic/task_logic.py
+-rw-r--r--   0        0        0      809 2023-07-05 02:24:17.329786 yyxx_game_pkg-2023.7.5.1/yyxx_game_pkg/stat/dispatch/route.py
+-rw-r--r--   0        0        0      677 2023-07-05 02:24:17.329786 yyxx_game_pkg-2023.7.5.1/yyxx_game_pkg/stat/dispatch/rules/__init__.py
+-rw-r--r--   0        0        0      689 2023-07-05 02:24:17.329786 yyxx_game_pkg-2023.7.5.1/yyxx_game_pkg/stat/dispatch/rules/rule_base.py
+-rw-r--r--   0        0        0     4270 2023-07-05 02:24:17.329786 yyxx_game_pkg-2023.7.5.1/yyxx_game_pkg/stat/dispatch/rules/rule_workflow.py
+-rw-r--r--   0        0        0      667 2023-07-05 02:24:17.329786 yyxx_game_pkg-2023.7.5.1/yyxx_game_pkg/stat/log.py
+-rw-r--r--   0        0        0       70 2023-07-05 02:24:17.329786 yyxx_game_pkg-2023.7.5.1/yyxx_game_pkg/stat/submit/__init__.py
+-rw-r--r--   0        0        0       70 2023-07-05 02:24:17.329786 yyxx_game_pkg-2023.7.5.1/yyxx_game_pkg/stat/submit/logic/__init__.py
+-rw-r--r--   0        0        0     5961 2023-07-05 02:24:17.329786 yyxx_game_pkg-2023.7.5.1/yyxx_game_pkg/stat/submit/logic/submit_logic.py
+-rw-r--r--   0        0        0      987 2023-07-05 02:24:17.329786 yyxx_game_pkg-2023.7.5.1/yyxx_game_pkg/stat/submit/submit.py
+-rw-r--r--   0        0        0       70 2023-07-05 02:24:17.329786 yyxx_game_pkg-2023.7.5.1/yyxx_game_pkg/stat/xcelery/__init__.py
+-rw-r--r--   0        0        0     2206 2023-07-05 02:24:17.329786 yyxx_game_pkg-2023.7.5.1/yyxx_game_pkg/stat/xcelery/instance.py
+-rw-r--r--   0        0        0     1183 2023-07-05 02:24:17.329786 yyxx_game_pkg-2023.7.5.1/yyxx_game_pkg/stat/xcelery/task_base.py
+-rw-r--r--   0        0        0      428 2023-07-05 02:24:17.329786 yyxx_game_pkg-2023.7.5.1/yyxx_game_pkg/template/__init__.py
+-rw-r--r--   0        0        0      132 2023-07-05 02:24:17.329786 yyxx_game_pkg-2023.7.5.1/yyxx_game_pkg/template/sdk/cookiecutter.json
+-rw-r--r--   0        0        0     4023 2023-07-05 02:24:17.329786 yyxx_game_pkg-2023.7.5.1/yyxx_game_pkg/template/sdk/sdk_{{cookiecutter.sdk_name}}/check_token.py
+-rw-r--r--   0        0        0      624 2023-07-05 02:24:17.329786 yyxx_game_pkg-2023.7.5.1/yyxx_game_pkg/template/sdk/sdk_{{cookiecutter.sdk_name}}/map_factor.py
+-rw-r--r--   0        0        0     4077 2023-07-05 02:24:17.329786 yyxx_game_pkg-2023.7.5.1/yyxx_game_pkg/template/sdk/sdk_{{cookiecutter.sdk_name}}/recharge.py
+-rw-r--r--   0        0        0       83 2023-07-05 02:24:17.329786 yyxx_game_pkg-2023.7.5.1/yyxx_game_pkg/utils/__init__.py
+-rw-r--r--   0        0        0     5650 2023-07-05 02:24:17.329786 yyxx_game_pkg-2023.7.5.1/yyxx_game_pkg/utils/decorator.py
+-rw-r--r--   0        0        0     3135 2023-07-05 02:24:17.329786 yyxx_game_pkg-2023.7.5.1/yyxx_game_pkg/utils/error_code.py
+-rw-r--r--   0        0        0     2845 2023-07-05 02:24:17.329786 yyxx_game_pkg-2023.7.5.1/yyxx_game_pkg/utils/profiler.py
+-rw-r--r--   0        0        0     3068 2023-07-05 02:24:17.329786 yyxx_game_pkg-2023.7.5.1/yyxx_game_pkg/utils/xListStr.py
+-rw-r--r--   0        0        0     9461 2023-07-05 02:24:17.329786 yyxx_game_pkg-2023.7.5.1/yyxx_game_pkg/utils/xdataframe.py
+-rw-r--r--   0        0        0     7441 2023-07-05 02:24:17.329786 yyxx_game_pkg-2023.7.5.1/yyxx_game_pkg/utils/xdate.py
+-rw-r--r--   0        0        0     2092 2023-07-05 02:24:17.329786 yyxx_game_pkg-2023.7.5.1/yyxx_game_pkg/utils/xfutures.py
+-rw-r--r--   0        0        0     3653 2023-07-05 02:24:17.329786 yyxx_game_pkg-2023.7.5.1/yyxx_game_pkg/utils/xhttp.py
+-rw-r--r--   0        0        0      971 2023-07-05 02:24:17.329786 yyxx_game_pkg-2023.7.5.1/yyxx_game_pkg/utils/xmath.py
+-rw-r--r--   0        0        0      573 2023-07-05 02:24:17.329786 yyxx_game_pkg-2023.7.5.1/yyxx_game_pkg/utils/xstring.py
+-rw-r--r--   0        0        0       69 2023-07-05 02:24:17.329786 yyxx_game_pkg-2023.7.5.1/yyxx_game_pkg/xtrace/__init__.py
+-rw-r--r--   0        0        0     1895 2023-07-05 02:24:17.329786 yyxx_game_pkg-2023.7.5.1/yyxx_game_pkg/xtrace/flask/__init__.py
+-rw-r--r--   0        0        0     2858 2023-07-05 02:24:17.329786 yyxx_game_pkg-2023.7.5.1/yyxx_game_pkg/xtrace/helper.py
+-rw-r--r--   0        0        0     7005 1970-01-01 00:00:00.000000 yyxx_game_pkg-2023.7.5.1/PKG-INFO
```

### Comparing `yyxx_game_pkg-2023.6.9.1/README.md` & `yyxx_game_pkg-2023.7.5.1/README.md`

 * *Files identical despite different names*

### Comparing `yyxx_game_pkg-2023.6.9.1/pyproject.toml` & `yyxx_game_pkg-2023.7.5.1/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = [ "poetry-core",]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry]
 name = "yyxx-game-pkg"
-version = "v2023.06.09.001"
+version = "v2023.07.05.001"
 description = "yyxx game custom module"
 authors = [ "yyxx-game",]
 license = "MIT"
 homepage = "https://github.com/yyxxgame/yyxxgame-pkg"
 repository = "https://github.com/yyxxgame/yyxxgame-pkg"
 readme = "README.md"
 classifiers = [ "Programming Language :: Python :: 3", "License :: OSI Approved :: MIT License", "Operating System :: OS Independent",]
@@ -23,25 +23,28 @@
 toml = "^0.10.2"
 opentelemetry-api = "^1.16.0"
 opentelemetry-sdk = "^1.16.0"
 opentelemetry-exporter-jaeger = "^1.16.0"
 opentelemetry-instrumentation-requests = "^0.37b0"
 opentelemetry-instrumentation-fastapi = "0.37b.0"
 opentelemetry-instrumentation-celery = "0.37b0"
+opentelemetry-instrumentation-flask = "^0.37b0"
 line-profiler = "^4.0.3"
 redis = "^4.5.1"
 pymysql = "^1.0.2"
 pika = "^1.3.1"
 dbutils = "^3.0.2"
 ujson = "^5.7.0"
 requests = "2.27.1"
 celery = "5.2.7"
 uvicorn = "^0.21.0"
 pandas = "^1.5.3"
 pycryptodome = "^3.17"
+httpx = "^0.24.1"
+pymongo = "^4.4.0"
 
 [tool.poetry.extras]
 stat = [ "fastapi",]
 server_center = [ "django", "pillow", "filetype",]
 center_api = [ "flask", "cookiecutter",]
 
 [tool.poetry.dependencies.fastapi]
```

### Comparing `yyxx_game_pkg-2023.6.9.1/tests/dbops/mysql_op.py` & `yyxx_game_pkg-2023.7.5.1/tests/dbops/mysql_op.py`

 * *Files identical despite different names*

### Comparing `yyxx_game_pkg-2023.6.9.1/tests/dispatch/config/celery_local_config.py` & `yyxx_game_pkg-2023.7.5.1/tests/dispatch/config/celery_local_config.py`

 * *Files identical despite different names*

### Comparing `yyxx_game_pkg-2023.6.9.1/tests/dispatch/rules/__init__.py` & `yyxx_game_pkg-2023.7.5.1/tests/dispatch/rules/__init__.py`

 * *Files identical despite different names*

### Comparing `yyxx_game_pkg-2023.6.9.1/tests/dispatch/rules/rule_temp.py` & `yyxx_game_pkg-2023.7.5.1/tests/dispatch/rules/rule_temp.py`

 * *Files identical despite different names*

### Comparing `yyxx_game_pkg-2023.6.9.1/tests/dispatch/test_dispatch.py` & `yyxx_game_pkg-2023.7.5.1/tests/dispatch/test_dispatch.py`

 * *Files identical despite different names*

### Comparing `yyxx_game_pkg-2023.6.9.1/tests/helpers/test_mysql_helper.py` & `yyxx_game_pkg-2023.7.5.1/tests/helpers/test_mysql_helper.py`

 * *Files identical despite different names*

### Comparing `yyxx_game_pkg-2023.6.9.1/tests/submit/schedule_rule/schedule/work_flow/schedule_work_flow_test.py` & `yyxx_game_pkg-2023.7.5.1/tests/submit/schedule_rule/schedule/work_flow/schedule_work_flow_test.py`

 * *Files identical despite different names*

### Comparing `yyxx_game_pkg-2023.6.9.1/tests/submit/test_submit.py` & `yyxx_game_pkg-2023.7.5.1/tests/submit/test_submit.py`

 * *Files identical despite different names*

### Comparing `yyxx_game_pkg-2023.6.9.1/tests/test_logger.py` & `yyxx_game_pkg-2023.7.5.1/tests/test_logger.py`

 * *Files identical despite different names*

### Comparing `yyxx_game_pkg-2023.6.9.1/tests/test_xtrace.py` & `yyxx_game_pkg-2023.7.5.1/tests/test_xtrace.py`

 * *Files identical despite different names*

### Comparing `yyxx_game_pkg-2023.6.9.1/tests/xcelery/config/celery_local_config.py` & `yyxx_game_pkg-2023.7.5.1/tests/xcelery/config/celery_local_config.py`

 * *Files identical despite different names*

### Comparing `yyxx_game_pkg-2023.6.9.1/tests/xcelery/task_register.py` & `yyxx_game_pkg-2023.7.5.1/tests/xcelery/task_register.py`

 * *Files identical despite different names*

### Comparing `yyxx_game_pkg-2023.6.9.1/yyxx_game_pkg/center_api/model/Operator.py` & `yyxx_game_pkg-2023.7.5.1/yyxx_game_pkg/center_api/model/Operator.py`

 * *Files identical despite different names*

### Comparing `yyxx_game_pkg-2023.6.9.1/yyxx_game_pkg/center_api/model/OperatorServer.py` & `yyxx_game_pkg-2023.7.5.1/yyxx_game_pkg/center_api/model/OperatorServer.py`

 * *Files identical despite different names*

### Comparing `yyxx_game_pkg-2023.6.9.1/yyxx_game_pkg/center_api/model/RechargeConfig.py` & `yyxx_game_pkg-2023.7.5.1/yyxx_game_pkg/center_api/model/RechargeConfig.py`

 * *Files identical despite different names*

### Comparing `yyxx_game_pkg-2023.6.9.1/yyxx_game_pkg/center_api/model/TableFieldConf.py` & `yyxx_game_pkg-2023.7.5.1/yyxx_game_pkg/center_api/model/TableFieldConf.py`

 * *Files identical despite different names*

### Comparing `yyxx_game_pkg-2023.6.9.1/yyxx_game_pkg/center_api/sdk/check_token.py` & `yyxx_game_pkg-2023.7.5.1/yyxx_game_pkg/center_api/sdk/check_token.py`

 * *Files 5% similar despite different names*

```diff
@@ -25,73 +25,72 @@
     @func sdk_check_token: 验证token方法
     @func sdk_helper: sdk 参数处理
     @func channel_make_sign: 默认 sorted(params) md5
 
     根据渠道需求填写以下参数
     @param is_https: 请求是否为https；默认 True
     @param method: 请求方式 POST GET；默认 POST
-    @param params: 发送和收到 参数的字段名
-    @param time_param: 时间戳字段 time / timestamp，十位时间戳（秒） / 十三位时间戳（毫秒）
-    @param sign_param: 签名字段 sign / signature
+    @param params: (key)发送和(value)接收 参数的字段名
     """
 
     is_https = True  # True False
     method = "POST"
     # params = {}
-    time_param = None  # ("time", int(time.time()))
-    sign_param = "sign"
+    sdk_exclude = ()
 
     def run_check_token(self, *args, **kwargs) -> dict:
         """
         run check token
         """
         sdk_helper, response_helper = self.sdk_version_choice(**kwargs)
         if sdk_helper is None:
             return self.sdk_rechfeed(ErrorCode.ERROR_INVALID_PARAM)
 
-        channel_data, post_data = sdk_helper(**kwargs)
+        channel_data, post_data = sdk_helper(self.sdk_exclude, **kwargs)
         response = self.sdk_check_token(channel_data, post_data)
 
         return response_helper(response, **kwargs)
 
     @abstractmethod
     def response_helper(self, response: dict | None, **kwargs) -> dict:
         """
         根据需求 return 相应的数据
         :return: {"ret": 1, "user_id": "any_user_id"}
         """
-        return self.sdk_rechfeed(ErrorCode.ERROR_SERVER_API_URL_ERROR)
+        return self.sdk_rechfeed(ErrorCode.ERROR_INVALID_PARAM, "验证失败")
 
     @property
     def _params(self):
         """
         params = {
             "appId": "sdk_appId",
             "accountId": "sdk_accountId",
             "token": "sdk_token",
         }
         """
         if self.params is None:
-            raise ValueError("params must be specified")
+            raise ValueError("params must be specified as a dict")
 
         return self.params
 
-    def sdk_helper(self, **kwargs) -> (dict, dict):
+    def sdk_helper(self, sdk_exclude=(), **kwargs) -> (dict, dict):
         """
         处理 sdk 数据
+        :param sdk_exclude: sdk_helper 处理数据，要排除的key
+            可选值: time(self.Time) sign(self.Flag)
         """
         channel_data = kwargs.get("channel_data", {})
 
         post_data = {}
         for k, v in self._params.items():
             post_data[k] = kwargs.get(v)
-        if self.time_param:
-            post_data[self.time_param[0]] = self.time_param[1]
-        if self.sign_param:
-            post_data[self.sign_param] = self.channel_make_sign(
+        if self.Time not in sdk_exclude:
+            post_data[self.Time] = int(time.time())
+        if self.Flag not in sdk_exclude:
+            post_data[self.Flag] = self.channel_make_sign(
                 post_data, channel_data.get("app_key", "")
             )
 
         return channel_data, post_data
 
     def sdk_check_token(self, channel_data, post_data) -> dict | None:
         """
```

### Comparing `yyxx_game_pkg-2023.6.9.1/yyxx_game_pkg/center_api/sdk/map_core.py` & `yyxx_game_pkg-2023.7.5.1/yyxx_game_pkg/center_api/sdk/map_core.py`

 * *Files 4% similar despite different names*

```diff
@@ -54,21 +54,19 @@
             return False
         _sign = self.make_sign(values)
         if sign != _sign:
             return False
         return True
 
     def make_sign(self, values) -> str:
-        self.make_sign_exclude.add(self.Flag)
         return make_sign(
             values, self.api_key, exclude=self.make_sign_exclude, time_key=self.Time
         )
 
     def channel_make_sign(self, values, sign_key) -> str:
-        self.make_sign_exclude.add(self.Flag)
         return make_sign(
             values, sign_key, exclude=self.make_sign_exclude, time_key=None
         )
 
     def check_time_out(self, values):
         _time = int(values.get(self.Time, 0))
         t = time.time()
```

### Comparing `yyxx_game_pkg-2023.6.9.1/yyxx_game_pkg/center_api/sdk/recharge.py` & `yyxx_game_pkg-2023.7.5.1/yyxx_game_pkg/center_api/sdk/recharge.py`

 * *Files 11% similar despite different names*

```diff
@@ -21,16 +21,17 @@
     @param channel_username: 渠道帐号
     @param is_test: 是否测试订单
     """
     extra: str = "extra"
     cp_order_id: str = "billno"
     channel_order_id: str = "order_id"
     player_id: str = "role_id"
-    is_check_username: int = 1
     channel_username: str = "openid"
+    money: str = "amount"
+    is_check_username: int = 1
     is_test: int = 0
 
 
 class BaseRecharge(MapCore, ABC):
     """
     注意：
         方法 modify_params 用来修改 params 的参数值
@@ -78,14 +79,17 @@
         money  金额
         real_money  实付金额
         extra_gold  赠送元宝（渠道返利）
         extra_gold_bind  赠送绑元（渠道返利）
         pay_dt 充值时间（秒）
         --------------------------------
         """
+        amount = int(data.get(self.params.money, 0))
+        data_ary["real_money"] = int(amount / 100)
+        data_ary["money"] = amount / 100
 
     def make_sign_helper(self, values) -> (dict, str):
         ext_ary = values[self.params.extra].split(",")
         plat_code = ext_ary[0]
         game_channel_id = ext_ary[1]
         sdk_data = self.operator.get_key(plat_code, game_channel_id)
         pay_key = sdk_data.get("pay_key", "")
```

### Comparing `yyxx_game_pkg-2023.6.9.1/yyxx_game_pkg/conf/__init__.py` & `yyxx_game_pkg-2023.7.5.1/yyxx_game_pkg/conf/__init__.py`

 * *Files identical despite different names*

### Comparing `yyxx_game_pkg-2023.6.9.1/yyxx_game_pkg/conf/global_settings.py` & `yyxx_game_pkg-2023.7.5.1/yyxx_game_pkg/conf/global_settings.py`

 * *Files identical despite different names*

### Comparing `yyxx_game_pkg-2023.6.9.1/yyxx_game_pkg/crypto/aes.py` & `yyxx_game_pkg-2023.7.5.1/yyxx_game_pkg/crypto/aes.py`

 * *Files identical despite different names*

### Comparing `yyxx_game_pkg-2023.6.9.1/yyxx_game_pkg/crypto/basic.py` & `yyxx_game_pkg-2023.7.5.1/yyxx_game_pkg/crypto/basic.py`

 * *Files identical despite different names*

### Comparing `yyxx_game_pkg-2023.6.9.1/yyxx_game_pkg/crypto/make_sign.py` & `yyxx_game_pkg-2023.7.5.1/yyxx_game_pkg/crypto/make_sign.py`

 * *Files 1% similar despite different names*

```diff
@@ -13,15 +13,15 @@
     secret_key: str,
     *,
     exclude: Iterable = None,
     time_key="time",
     make_sign_func=md5,
     make_sign_key: str = None,
     digest_mod=None,
-):
+) -> str:
     """
     签名方法
     :param values: 需要加密的数据（字典）
     :param secret_key: 加密秘钥
     :param exclude: 字段名可选列表，如果提供，加密时会排除其中字段，然后进行加密
     :param time_key: 获取时间戳的字段名；默认为 time
     :param make_sign_func: 进行加密的方法
```

### Comparing `yyxx_game_pkg-2023.6.9.1/yyxx_game_pkg/crypto/rsa.py` & `yyxx_game_pkg-2023.7.5.1/yyxx_game_pkg/crypto/rsa.py`

 * *Files identical despite different names*

### Comparing `yyxx_game_pkg-2023.6.9.1/yyxx_game_pkg/dbops/base.py` & `yyxx_game_pkg-2023.7.5.1/yyxx_game_pkg/dbops/base.py`

 * *Files identical despite different names*

### Comparing `yyxx_game_pkg-2023.6.9.1/yyxx_game_pkg/dbops/ch_op.py` & `yyxx_game_pkg-2023.7.5.1/yyxx_game_pkg/dbops/ch_op.py`

 * *Files identical despite different names*

### Comparing `yyxx_game_pkg-2023.6.9.1/yyxx_game_pkg/dbops/das_api.py` & `yyxx_game_pkg-2023.7.5.1/yyxx_game_pkg/dbops/das_api.py`

 * *Files identical despite different names*

### Comparing `yyxx_game_pkg-2023.6.9.1/yyxx_game_pkg/dbops/es_op.py` & `yyxx_game_pkg-2023.7.5.1/yyxx_game_pkg/dbops/es_op.py`

 * *Files identical despite different names*

### Comparing `yyxx_game_pkg-2023.6.9.1/yyxx_game_pkg/dbops/hdfs_op.py` & `yyxx_game_pkg-2023.7.5.1/yyxx_game_pkg/dbops/hdfs_op.py`

 * *Files identical despite different names*

### Comparing `yyxx_game_pkg-2023.6.9.1/yyxx_game_pkg/dbops/mysql_op.py` & `yyxx_game_pkg-2023.7.5.1/yyxx_game_pkg/dbops/mysql_op.py`

 * *Files identical despite different names*

### Comparing `yyxx_game_pkg-2023.6.9.1/yyxx_game_pkg/helpers/mysql_helper.py` & `yyxx_game_pkg-2023.7.5.1/yyxx_game_pkg/helpers/mysql_helper.py`

 * *Files 4% similar despite different names*

```diff
@@ -26,23 +26,23 @@
     USE_UNICODE = None
     CHARSET = None
     MAX_CACHED = None
     MAX_CONNECTIONS = None
     CURSOR = None
 
     def __str__(self):
-        return "host:{},port:{},db:{},use_unicode:{},charset:{},max_cache:{},max_connections:{},cursor:{}".format(
+        # 不能返回无法序列化的数据， 否则单例会失效
+        return "host:{},port:{},db:{},use_unicode:{},charset:{},max_cache:{},max_connections:{}".format(
             self.HOST,
             self.PORT,
             self.DB,
             self.USE_UNICODE,
             self.CHARSET,
             self.MAX_CACHED,
-            self.MAX_CONNECTIONS,
-            self.CURSOR,
+            self.MAX_CONNECTIONS
         )
 
 
 @singleton_unique_obj_args
 class MysqlDbPool(object):
     def __init__(self, config: MysqlConfig):
         self.DB_POOL = PooledDB(
```

### Comparing `yyxx_game_pkg-2023.6.9.1/yyxx_game_pkg/helpers/op_helper.py` & `yyxx_game_pkg-2023.7.5.1/yyxx_game_pkg/helpers/op_helper.py`

 * *Files identical despite different names*

### Comparing `yyxx_game_pkg-2023.6.9.1/yyxx_game_pkg/helpers/pika_helper.py` & `yyxx_game_pkg-2023.7.5.1/yyxx_game_pkg/helpers/pika_helper.py`

 * *Files identical despite different names*

### Comparing `yyxx_game_pkg-2023.6.9.1/yyxx_game_pkg/helpers/redis_helper.py` & `yyxx_game_pkg-2023.7.5.1/yyxx_game_pkg/helpers/redis_helper.py`

 * *Files identical despite different names*

### Comparing `yyxx_game_pkg-2023.6.9.1/yyxx_game_pkg/ip2region/ip2region.xdb` & `yyxx_game_pkg-2023.7.5.1/yyxx_game_pkg/ip2region/ip2region.xdb`

 * *Files identical despite different names*

### Comparing `yyxx_game_pkg-2023.6.9.1/yyxx_game_pkg/ip2region/ip_x.py` & `yyxx_game_pkg-2023.7.5.1/yyxx_game_pkg/ip2region/ip_x.py`

 * *Files identical despite different names*

### Comparing `yyxx_game_pkg-2023.6.9.1/yyxx_game_pkg/ip2region/xdbSearcher.py` & `yyxx_game_pkg-2023.7.5.1/yyxx_game_pkg/ip2region/xdbSearcher.py`

 * *Files identical despite different names*

### Comparing `yyxx_game_pkg-2023.6.9.1/yyxx_game_pkg/logger/config.py` & `yyxx_game_pkg-2023.7.5.1/yyxx_game_pkg/logger/config.py`

 * *Files identical despite different names*

### Comparing `yyxx_game_pkg-2023.6.9.1/yyxx_game_pkg/logger/handlers.py` & `yyxx_game_pkg-2023.7.5.1/yyxx_game_pkg/logger/handlers.py`

 * *Files identical despite different names*

### Comparing `yyxx_game_pkg-2023.6.9.1/yyxx_game_pkg/logger/log.py` & `yyxx_game_pkg-2023.7.5.1/yyxx_game_pkg/logger/log.py`

 * *Files identical despite different names*

### Comparing `yyxx_game_pkg-2023.6.9.1/yyxx_game_pkg/stat/dispatch/common/common.py` & `yyxx_game_pkg-2023.7.5.1/yyxx_game_pkg/stat/dispatch/common/common.py`

 * *Files identical despite different names*

### Comparing `yyxx_game_pkg-2023.6.9.1/yyxx_game_pkg/stat/dispatch/core/manager.py` & `yyxx_game_pkg-2023.7.5.1/yyxx_game_pkg/stat/dispatch/core/manager.py`

 * *Files identical despite different names*

### Comparing `yyxx_game_pkg-2023.6.9.1/yyxx_game_pkg/stat/dispatch/core/structs.py` & `yyxx_game_pkg-2023.7.5.1/yyxx_game_pkg/stat/dispatch/core/structs.py`

 * *Files identical despite different names*

### Comparing `yyxx_game_pkg-2023.6.9.1/yyxx_game_pkg/stat/dispatch/core/workflows.py` & `yyxx_game_pkg-2023.7.5.1/yyxx_game_pkg/stat/dispatch/core/workflows.py`

 * *Files identical despite different names*

### Comparing `yyxx_game_pkg-2023.6.9.1/yyxx_game_pkg/stat/dispatch/dispatch.py` & `yyxx_game_pkg-2023.7.5.1/yyxx_game_pkg/stat/dispatch/dispatch.py`

 * *Files identical despite different names*

### Comparing `yyxx_game_pkg-2023.6.9.1/yyxx_game_pkg/stat/dispatch/logic/task_logic.py` & `yyxx_game_pkg-2023.7.5.1/yyxx_game_pkg/stat/dispatch/logic/task_logic.py`

 * *Files identical despite different names*

### Comparing `yyxx_game_pkg-2023.6.9.1/yyxx_game_pkg/stat/dispatch/route.py` & `yyxx_game_pkg-2023.7.5.1/yyxx_game_pkg/stat/dispatch/route.py`

 * *Files identical despite different names*

### Comparing `yyxx_game_pkg-2023.6.9.1/yyxx_game_pkg/stat/dispatch/rules/__init__.py` & `yyxx_game_pkg-2023.7.5.1/yyxx_game_pkg/stat/dispatch/rules/__init__.py`

 * *Files identical despite different names*

### Comparing `yyxx_game_pkg-2023.6.9.1/yyxx_game_pkg/stat/dispatch/rules/rule_base.py` & `yyxx_game_pkg-2023.7.5.1/yyxx_game_pkg/stat/dispatch/rules/rule_base.py`

 * *Files identical despite different names*

### Comparing `yyxx_game_pkg-2023.6.9.1/yyxx_game_pkg/stat/dispatch/rules/rule_workflow.py` & `yyxx_game_pkg-2023.7.5.1/yyxx_game_pkg/stat/dispatch/rules/rule_workflow.py`

 * *Files identical despite different names*

### Comparing `yyxx_game_pkg-2023.6.9.1/yyxx_game_pkg/stat/log.py` & `yyxx_game_pkg-2023.7.5.1/yyxx_game_pkg/stat/log.py`

 * *Files identical despite different names*

### Comparing `yyxx_game_pkg-2023.6.9.1/yyxx_game_pkg/stat/submit/logic/submit_logic.py` & `yyxx_game_pkg-2023.7.5.1/yyxx_game_pkg/stat/submit/logic/submit_logic.py`

 * *Files identical despite different names*

### Comparing `yyxx_game_pkg-2023.6.9.1/yyxx_game_pkg/stat/submit/submit.py` & `yyxx_game_pkg-2023.7.5.1/yyxx_game_pkg/stat/submit/submit.py`

 * *Files identical despite different names*

### Comparing `yyxx_game_pkg-2023.6.9.1/yyxx_game_pkg/stat/xcelery/instance.py` & `yyxx_game_pkg-2023.7.5.1/yyxx_game_pkg/stat/xcelery/instance.py`

 * *Files identical despite different names*

### Comparing `yyxx_game_pkg-2023.6.9.1/yyxx_game_pkg/stat/xcelery/task_base.py` & `yyxx_game_pkg-2023.7.5.1/yyxx_game_pkg/stat/xcelery/task_base.py`

 * *Files identical despite different names*

### Comparing `yyxx_game_pkg-2023.6.9.1/yyxx_game_pkg/template/sdk/sdk_{{cookiecutter.sdk_name}}/check_token.py` & `yyxx_game_pkg-2023.7.5.1/yyxx_game_pkg/template/sdk/sdk_{{cookiecutter.sdk_name}}/check_token.py`

 * *Files 5% similar despite different names*

```diff
@@ -17,14 +17,15 @@
     # time_param = ("time", int(time.time())
 
     # 根据接口文档填写 params 的键值
     # params key: post_data的键
     # params value: kwargs的键
     # --> post_data[key] = kwargs[value]
     params = {}
+    sdk_exclude = ()
 
     # 父类中核心代码，此处可删除
     # def run_check_token(self, *args, **kwargs) -> dict:
     #     """
     #     run check token
     #     """
     #     sdk_helper, response_helper = self.sdk_version_choice(**kwargs)
@@ -32,30 +33,31 @@
     #         return self.sdk_rechfeed(ErrorCode.ERROR_INVALID_PARAM)
     #
     #     channel_data, post_data = sdk_helper(**kwargs)
     #     response = self.sdk_check_token(channel_data, post_data)
     #
     #     return response_helper(response, **kwargs)
 
-    def sdk_helper(self, **kwargs) -> (dict, dict):
+    def sdk_helper(self, sdk_exclude=(), **kwargs) -> (dict, dict):
         """
         channel_data = kwargs.get("channel_data", {})
 
         post_data = {}
         for k, v in self._params.items():
             post_data[k] = kwargs.get(v)
-        if self.time_param:
-            post_data[self.time_param[0]] = self.time_param[1]
-        if self.sign_param:
-            post_data[self.sign_param] = self.channel_make_sign(
+        if self.Time not in sdk_exclude:
+            post_data[self.Time] = int(time.time())
+        if self.Flag not in sdk_exclude:
+            post_data[self.Flag] = self.channel_make_sign(
                 post_data, channel_data.get("app_key", "")
             )
 
         return channel_data, post_data
 
+        :param sdk_exclude: exclude parameters
         :param kwargs: 参数
         :return: channel_data, post_data
 
         --------------------------------
         如果 post_data 有修改或者补充，可以在此方法中添加
         channel_data, post_data = super().sdk_helper(**kwargs)
         post_data["需要修改或添加的键"] = "需要修改或添加的值"
```

### Comparing `yyxx_game_pkg-2023.6.9.1/yyxx_game_pkg/template/sdk/sdk_{{cookiecutter.sdk_name}}/map_factor.py` & `yyxx_game_pkg-2023.7.5.1/yyxx_game_pkg/template/sdk/sdk_{{cookiecutter.sdk_name}}/map_factor.py`

 * *Files identical despite different names*

### Comparing `yyxx_game_pkg-2023.6.9.1/yyxx_game_pkg/template/sdk/sdk_{{cookiecutter.sdk_name}}/recharge.py` & `yyxx_game_pkg-2023.7.5.1/yyxx_game_pkg/template/sdk/sdk_{{cookiecutter.sdk_name}}/recharge.py`

 * *Files 3% similar despite different names*

```diff
@@ -27,16 +27,16 @@
         """
         修改 self.params 属性
         默认值:
             extra: str = "extra"
             cp_order_id: str = "billno"
             channel_order_id: str = "order_id"
             player_id: str = "role_id"
-            is_check_username: int = 1
             channel_username: str = "openid"
+            is_check_username: int = 1
             is_test: int = 0
 
         self.params.cp_order_id = "xxx"
         """
         pass
 
     # 项目通用方法，一般不需要修改，直接使用父类方法，此处可删除
@@ -64,14 +64,15 @@
         money  金额
         real_money  实付金额
         extra_gold  赠送元宝（渠道返利）
         extra_gold_bind  赠送绑元（渠道返利）
         pay_dt 充值时间（秒）
         --------------------------------
         """
+        super().get_params_helper(data, data_ary)
 
     def make_sign_helper(self, values) -> (dict, str):
         """
         ext_ary = values[self.extra_key].split(",")
         plat_code = ext_ary[0]
         game_channel_id = ext_ary[1]
         sdk_data = self.operator.get_key(plat_code, game_channel_id)
```

### Comparing `yyxx_game_pkg-2023.6.9.1/yyxx_game_pkg/utils/decorator.py` & `yyxx_game_pkg-2023.7.5.1/yyxx_game_pkg/utils/decorator.py`

 * *Files 2% similar despite different names*

```diff
@@ -178,16 +178,16 @@
     """
 
     def decorator(func):
         @functools.wraps(func)
         def wrapper(*args, **kwargs):
             try:
                 _arg = pickle.dumps(args)
-            except Exception as e:
-                root_log(e)
+            except Exception:
+                # 静默处理
                 _arg = pickle.dumps(args[1:])
             _kwargs = pickle.dumps(kwargs)
             # 不指明redis_key默认用func.name
             cache_key = redis_key if redis_key else func.__name__
             # prefix 防止与其他模块的缓存key冲突
             cache_key = f"{prefix}_{cache_key}_{_arg}_{_kwargs}"
             cache_data = handle.get_data(cache_key)
```

### Comparing `yyxx_game_pkg-2023.6.9.1/yyxx_game_pkg/utils/error_code.py` & `yyxx_game_pkg-2023.7.5.1/yyxx_game_pkg/utils/error_code.py`

 * *Files identical despite different names*

### Comparing `yyxx_game_pkg-2023.6.9.1/yyxx_game_pkg/utils/profiler.py` & `yyxx_game_pkg-2023.7.5.1/yyxx_game_pkg/utils/profiler.py`

 * *Files identical despite different names*

### Comparing `yyxx_game_pkg-2023.6.9.1/yyxx_game_pkg/utils/xListStr.py` & `yyxx_game_pkg-2023.7.5.1/yyxx_game_pkg/utils/xListStr.py`

 * *Files identical despite different names*

### Comparing `yyxx_game_pkg-2023.6.9.1/yyxx_game_pkg/utils/xdataframe.py` & `yyxx_game_pkg-2023.7.5.1/yyxx_game_pkg/utils/xdataframe.py`

 * *Files 8% similar despite different names*

```diff
@@ -96,15 +96,17 @@
         return data.apply(cal_round_rate, args=(precision, suffix), axis=0)
     if isinstance(data, pd.Series):
         if str(invalid_value).isdigit():
             data = data.fillna(invalid_value)
         data = data.astype(float).round(precision)
         if precision == 0:
             data = data.astype(int)
-        return data.apply(lambda d: invalid_value if (d == np.inf or np.isnan(d)) else f"{d}{suffix}")
+        return data.apply(
+            lambda d: invalid_value if (d == np.inf or np.isnan(d)) else f"{d}{suffix}"
+        )
     if isinstance(data, (int, float)):
         if np.isnan(data) or data == np.inf:
             return invalid_value
         if precision == 0:
             return str(int(data)) + suffix
         return str(round(data, precision)) + suffix
     return invalid_value
@@ -267,39 +269,42 @@
         return labels, bins[position]
 
     return _df.apply(cut_bins, axis=1, result_type="expand")
 
 
 def div_rate(data_df: pd.DataFrame, top_key, bottom_key, precision=2) -> pd.Series:
     """
-    dataframe div函数计算百分比
+    dataframe div函数计算百分比 top_key / bottom_key
     example:
         data_df["pay_rate"] = div_rate(data_df, "pid_cnt", "act_player_cnt")
     :return:
     """
+    if isinstance(top_key, list):
+        return (
+            data_df[top_key]
+            .div(data_df[bottom_key], axis=0)
+            .round(precision + 2)
+            .applymap(lambda x: f"{round(x * 100, precision) }%")
+        )
     return (
         data_df[top_key]
         .div(data_df[bottom_key], axis=0)
         .round(precision + 2)
         .apply(lambda x: f"{round(x * 100, precision) }%")
     )
 
 
 def div_round(data_df: pd.DataFrame, top_key, bottom_key, precision=2) -> pd.Series:
     """
-    dataframe div函数
+    dataframe div函数 top_key / bottom_key
     example:
         data_df["pay_rate"] = div_round(data_df, "pid_cnt", "act_player_cnt")
     :return:
     """
-    return (
-        data_df[top_key]
-        .div(data_df[bottom_key], axis=0)
-        .round(precision)
-    )
+    return data_df[top_key].div(data_df[bottom_key], axis=0).round(precision)
 
 
 def concat_cols(data_df: pd.DataFrame, cols: list, concat_by="|") -> pd.Series:
     """
     合将列，汇总后的列为：recharge_cnt|recharge_type_id
     example:
         data_df["show_pid_cnt"] = concat_cols(data_df, ["pid_cnt", "pid_rate"]) -> 98|10.0%
@@ -311,7 +316,22 @@
         else:
             res = res + data_df[col].astype(str)
         if col == cols[-1]:
             continue
         res = res + concat_by
     return res
 
+
+def df_astype(_df: pd.DataFrame, columns=(), excludes=(), tpe=str):
+    """
+    dataframe转类型,可指定列进行转换,也可反向排除某些列,进行转换
+    主要用于某些数据列,仅少数列无需转,多数列需要转时,需要列举所有的列,此举可减少编写
+    columns:需转换的列
+    excludes:除了excludes外的列将进行转换(优先级更高)
+    tpe:需转换的类型
+    """
+    if excludes:
+        df_columns = _df.columns.tolist()
+        columns = list(set(df_columns) - set(excludes))
+    if columns:
+        _df[columns] = _df[columns].astype(tpe)
+    return _df
```

### Comparing `yyxx_game_pkg-2023.6.9.1/yyxx_game_pkg/utils/xdate.py` & `yyxx_game_pkg-2023.7.5.1/yyxx_game_pkg/utils/xdate.py`

 * *Files identical despite different names*

### Comparing `yyxx_game_pkg-2023.6.9.1/yyxx_game_pkg/utils/xhttp.py` & `yyxx_game_pkg-2023.7.5.1/yyxx_game_pkg/utils/xhttp.py`

 * *Files identical despite different names*

### Comparing `yyxx_game_pkg-2023.6.9.1/yyxx_game_pkg/utils/xmath.py` & `yyxx_game_pkg-2023.7.5.1/yyxx_game_pkg/utils/xmath.py`

 * *Files identical despite different names*

### Comparing `yyxx_game_pkg-2023.6.9.1/yyxx_game_pkg/utils/xstring.py` & `yyxx_game_pkg-2023.7.5.1/yyxx_game_pkg/utils/xstring.py`

 * *Files identical despite different names*

### Comparing `yyxx_game_pkg-2023.6.9.1/yyxx_game_pkg/xtrace/helper.py` & `yyxx_game_pkg-2023.7.5.1/yyxx_game_pkg/xtrace/helper.py`

 * *Files identical despite different names*

### Comparing `yyxx_game_pkg-2023.6.9.1/PKG-INFO` & `yyxx_game_pkg-2023.7.5.1/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: yyxx-game-pkg
-Version: 2023.6.9.1
+Version: 2023.7.5.1
 Summary: yyxx game custom module
 Home-page: https://github.com/yyxxgame/yyxxgame-pkg
 License: MIT
 Author: yyxx-game
 Requires-Python: >=3.8,<4
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -19,25 +19,28 @@
 Requires-Dist: celery (==5.2.7)
 Requires-Dist: cookiecutter (>=2.1.1,<3.0.0) ; extra == "center-api"
 Requires-Dist: dbutils (>=3.0.2,<4.0.0)
 Requires-Dist: django (>=4.2.1,<5.0.0) ; extra == "server-center"
 Requires-Dist: fastapi (>=0.94.0,<0.95.0) ; extra == "stat"
 Requires-Dist: filetype (>=1.2.0,<2.0.0) ; extra == "server-center"
 Requires-Dist: flask (>=2.3.2,<3.0.0) ; extra == "center-api"
+Requires-Dist: httpx (>=0.24.1,<0.25.0)
 Requires-Dist: line-profiler (>=4.0.3,<5.0.0)
 Requires-Dist: opentelemetry-api (>=1.16.0,<2.0.0)
 Requires-Dist: opentelemetry-exporter-jaeger (>=1.16.0,<2.0.0)
 Requires-Dist: opentelemetry-instrumentation-celery (==0.37b0)
 Requires-Dist: opentelemetry-instrumentation-fastapi (==0.37b.0)
+Requires-Dist: opentelemetry-instrumentation-flask (>=0.37b0,<0.38)
 Requires-Dist: opentelemetry-instrumentation-requests (>=0.37b0,<0.38)
 Requires-Dist: opentelemetry-sdk (>=1.16.0,<2.0.0)
 Requires-Dist: pandas (>=1.5.3,<2.0.0)
 Requires-Dist: pika (>=1.3.1,<2.0.0)
 Requires-Dist: pillow (>=9.5.0,<10.0.0) ; extra == "server-center"
 Requires-Dist: pycryptodome (>=3.17,<4.0)
+Requires-Dist: pymongo (>=4.4.0,<5.0.0)
 Requires-Dist: pymysql (>=1.0.2,<2.0.0)
 Requires-Dist: redis (>=4.5.1,<5.0.0)
 Requires-Dist: requests (==2.27.1)
 Requires-Dist: toml (>=0.10.2,<0.11.0)
 Requires-Dist: ujson (>=5.7.0,<6.0.0)
 Requires-Dist: uvicorn (>=0.21.0,<0.22.0)
 Project-URL: Repository, https://github.com/yyxxgame/yyxxgame-pkg
```

#### html2text {}

```diff
@@ -1,38 +1,40 @@
-Metadata-Version: 2.1 Name: yyxx-game-pkg Version: 2023.6.9.1 Summary: yyxx
+Metadata-Version: 2.1 Name: yyxx-game-pkg Version: 2023.7.5.1 Summary: yyxx
 game custom module Home-page: https://github.com/yyxxgame/yyxxgame-pkg License:
 MIT Author: yyxx-game Requires-Python: >=3.8,<4 Classifier: License :: OSI
 Approved :: MIT License Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3 Classifier: Programming
 Language :: Python :: 3.8 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10 Classifier: Programming
 Language :: Python :: 3.11 Provides-Extra: center-api Provides-Extra: server-
 center Provides-Extra: stat Requires-Dist: celery (==5.2.7) Requires-Dist:
 cookiecutter (>=2.1.1,<3.0.0) ; extra == "center-api" Requires-Dist: dbutils
 (>=3.0.2,<4.0.0) Requires-Dist: django (>=4.2.1,<5.0.0) ; extra == "server-
 center" Requires-Dist: fastapi (>=0.94.0,<0.95.0) ; extra == "stat" Requires-
 Dist: filetype (>=1.2.0,<2.0.0) ; extra == "server-center" Requires-Dist: flask
-(>=2.3.2,<3.0.0) ; extra == "center-api" Requires-Dist: line-profiler
-(>=4.0.3,<5.0.0) Requires-Dist: opentelemetry-api (>=1.16.0,<2.0.0) Requires-
-Dist: opentelemetry-exporter-jaeger (>=1.16.0,<2.0.0) Requires-Dist:
-opentelemetry-instrumentation-celery (==0.37b0) Requires-Dist: opentelemetry-
-instrumentation-fastapi (==0.37b.0) Requires-Dist: opentelemetry-
-instrumentation-requests (>=0.37b0,<0.38) Requires-Dist: opentelemetry-sdk
-(>=1.16.0,<2.0.0) Requires-Dist: pandas (>=1.5.3,<2.0.0) Requires-Dist: pika
-(>=1.3.1,<2.0.0) Requires-Dist: pillow (>=9.5.0,<10.0.0) ; extra == "server-
-center" Requires-Dist: pycryptodome (>=3.17,<4.0) Requires-Dist: pymysql
-(>=1.0.2,<2.0.0) Requires-Dist: redis (>=4.5.1,<5.0.0) Requires-Dist: requests
-(==2.27.1) Requires-Dist: toml (>=0.10.2,<0.11.0) Requires-Dist: ujson
-(>=5.7.0,<6.0.0) Requires-Dist: uvicorn (>=0.21.0,<0.22.0) Project-URL:
-Repository, https://github.com/yyxxgame/yyxxgame-pkg Description-Content-Type:
-text/markdown # YYXXGAME-PKG `yyxx-game-pkg`
-æ¯ä¸ä¸ªä¸é¨ä¸ºåæ¸¸å¬å¸åå°å¼åç Python åé¨æ¥å£éåã  [!
-[Contributors][contributors-shield]][contributors-url] [![Forks][forks-shield]]
-[forks-url] [![Stargazers][stars-shield]][stars-url] [![Issues][issues-shield]]
-[issues-url] [![MIT License][license-shield]][license-url]
+(>=2.3.2,<3.0.0) ; extra == "center-api" Requires-Dist: httpx
+(>=0.24.1,<0.25.0) Requires-Dist: line-profiler (>=4.0.3,<5.0.0) Requires-Dist:
+opentelemetry-api (>=1.16.0,<2.0.0) Requires-Dist: opentelemetry-exporter-
+jaeger (>=1.16.0,<2.0.0) Requires-Dist: opentelemetry-instrumentation-celery
+(==0.37b0) Requires-Dist: opentelemetry-instrumentation-fastapi (==0.37b.0)
+Requires-Dist: opentelemetry-instrumentation-flask (>=0.37b0,<0.38) Requires-
+Dist: opentelemetry-instrumentation-requests (>=0.37b0,<0.38) Requires-Dist:
+opentelemetry-sdk (>=1.16.0,<2.0.0) Requires-Dist: pandas (>=1.5.3,<2.0.0)
+Requires-Dist: pika (>=1.3.1,<2.0.0) Requires-Dist: pillow (>=9.5.0,<10.0.0) ;
+extra == "server-center" Requires-Dist: pycryptodome (>=3.17,<4.0) Requires-
+Dist: pymongo (>=4.4.0,<5.0.0) Requires-Dist: pymysql (>=1.0.2,<2.0.0)
+Requires-Dist: redis (>=4.5.1,<5.0.0) Requires-Dist: requests (==2.27.1)
+Requires-Dist: toml (>=0.10.2,<0.11.0) Requires-Dist: ujson (>=5.7.0,<6.0.0)
+Requires-Dist: uvicorn (>=0.21.0,<0.22.0) Project-URL: Repository, https://
+github.com/yyxxgame/yyxxgame-pkg Description-Content-Type: text/markdown #
+YYXXGAME-PKG `yyxx-game-pkg` æ¯ä¸ä¸ªä¸é¨ä¸ºåæ¸¸å¬å¸åå°å¼åç
+Python åé¨æ¥å£éåã  [![Contributors][contributors-shield]]
+[contributors-url] [![Forks][forks-shield]][forks-url] [![Stargazers][stars-
+shield]][stars-url] [![Issues][issues-shield]][issues-url] [![MIT License]
+[license-shield]][license-url]
                                 [åæ¸¸ä¿¡æ¯]
                             **** åæ¸¸ä¿¡æ¯ ****
 ## ç®å½ - [ä¸ææå](#ä¸ææå) - [ç¯å¢éç½®](#ç¯å¢éç½®) -
 [å®è£æ­¥éª¤](#å®è£æ­¥éª¤) - [æä»¶ç®å½è¯´æ](#æä»¶ç®å½è¯´æ) -
 [é¨ç½²](#é¨ç½²) - [develop](#develop) - [release](#release) - [æ¨¡åä»ç»]
 (#æ¨¡åä»ç») - [xtrace](#xtrace) - [stat](#stat) - [ä»£ç ç¤ºä¾]
 (#ä»£ç ç¤ºä¾) - [çæ¬æ§å¶](#çæ¬æ§å¶) ### ä¸ææå ######
```

