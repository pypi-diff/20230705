# Comparing `tmp/yyxx_game_pkg_dev-2023.6.9.1.dev8.tar.gz` & `tmp/yyxx_game_pkg_dev-2023.7.5.5.dev4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "yyxx_game_pkg_dev-2023.6.9.1.dev8.tar", max compression
+gzip compressed data, was "yyxx_game_pkg_dev-2023.7.5.5.dev4.tar", max compression
```

## Comparing `yyxx_game_pkg_dev-2023.6.9.1.dev8.tar` & `yyxx_game_pkg_dev-2023.7.5.5.dev4.tar`

### file list

```diff
@@ -1,116 +1,126 @@
--rw-r--r--   0        0        0     4895 2023-06-15 09:27:22.691723 yyxx_game_pkg_dev-2023.6.9.1.dev8/README.md
--rw-r--r--   0        0        0     1846 2023-06-15 09:27:35.619731 yyxx_game_pkg_dev-2023.6.9.1.dev8/pyproject.toml
--rw-r--r--   0        0        0       68 2023-06-15 09:27:22.691723 yyxx_game_pkg_dev-2023.6.9.1.dev8/tests/__init__.py
--rw-r--r--   0        0        0       83 2023-06-15 09:27:22.691723 yyxx_game_pkg_dev-2023.6.9.1.dev8/tests/dbops/__init__.py
--rw-r--r--   0        0        0     1341 2023-06-15 09:27:22.691723 yyxx_game_pkg_dev-2023.6.9.1.dev8/tests/dbops/mysql_op.py
--rw-r--r--   0        0        0       70 2023-06-15 09:27:22.691723 yyxx_game_pkg_dev-2023.6.9.1.dev8/tests/dispatch/__init__.py
--rw-r--r--   0        0        0       70 2023-06-15 09:27:22.691723 yyxx_game_pkg_dev-2023.6.9.1.dev8/tests/dispatch/config/__init__.py
--rw-r--r--   0        0        0     1228 2023-06-15 09:27:22.691723 yyxx_game_pkg_dev-2023.6.9.1.dev8/tests/dispatch/config/celery_local_config.py
--rw-r--r--   0        0        0      660 2023-06-15 09:27:22.691723 yyxx_game_pkg_dev-2023.6.9.1.dev8/tests/dispatch/rules/__init__.py
--rw-r--r--   0        0        0     1348 2023-06-15 09:27:22.691723 yyxx_game_pkg_dev-2023.6.9.1.dev8/tests/dispatch/rules/rule_temp.py
--rw-r--r--   0        0        0      580 2023-06-15 09:27:22.691723 yyxx_game_pkg_dev-2023.6.9.1.dev8/tests/dispatch/test_dispatch.py
--rw-r--r--   0        0        0       84 2023-06-15 09:27:22.691723 yyxx_game_pkg_dev-2023.6.9.1.dev8/tests/helpers/__init__.py
--rw-r--r--   0        0        0      522 2023-06-15 09:27:22.691723 yyxx_game_pkg_dev-2023.6.9.1.dev8/tests/helpers/test_mysql_helper.py
--rw-r--r--   0        0        0      455 2023-06-15 09:27:22.691723 yyxx_game_pkg_dev-2023.6.9.1.dev8/tests/helpers/test_pika_helper.py
--rw-r--r--   0        0        0      481 2023-06-15 09:27:22.691723 yyxx_game_pkg_dev-2023.6.9.1.dev8/tests/helpers/test_redis_helper.py
--rw-r--r--   0        0        0       70 2023-06-15 09:27:22.691723 yyxx_game_pkg_dev-2023.6.9.1.dev8/tests/submit/__init__.py
--rw-r--r--   0        0        0       70 2023-06-15 09:27:22.691723 yyxx_game_pkg_dev-2023.6.9.1.dev8/tests/submit/schedule_rule/__init__.py
--rw-r--r--   0        0        0       70 2023-06-15 09:27:22.691723 yyxx_game_pkg_dev-2023.6.9.1.dev8/tests/submit/schedule_rule/schedule/__init__.py
--rw-r--r--   0        0        0       70 2023-06-15 09:27:22.691723 yyxx_game_pkg_dev-2023.6.9.1.dev8/tests/submit/schedule_rule/schedule/statistic_task/__init__.py
--rw-r--r--   0        0        0      431 2023-06-15 09:27:22.691723 yyxx_game_pkg_dev-2023.6.9.1.dev8/tests/submit/schedule_rule/schedule/statistic_task/schedule_statistic_collect_test.py
--rw-r--r--   0        0        0      413 2023-06-15 09:27:22.691723 yyxx_game_pkg_dev-2023.6.9.1.dev8/tests/submit/schedule_rule/schedule/statistic_task/schedule_statistic_task_test.py
--rw-r--r--   0        0        0       70 2023-06-15 09:27:22.691723 yyxx_game_pkg_dev-2023.6.9.1.dev8/tests/submit/schedule_rule/schedule/work_flow/__init__.py
--rw-r--r--   0        0        0     1217 2023-06-15 09:27:22.691723 yyxx_game_pkg_dev-2023.6.9.1.dev8/tests/submit/schedule_rule/schedule/work_flow/schedule_work_flow_test.py
--rw-r--r--   0        0        0      305 2023-06-15 09:27:22.691723 yyxx_game_pkg_dev-2023.6.9.1.dev8/tests/submit/submit.json
--rw-r--r--   0        0        0     1250 2023-06-15 09:27:22.691723 yyxx_game_pkg_dev-2023.6.9.1.dev8/tests/submit/test_submit.py
--rw-r--r--   0        0        0      235 2023-06-15 09:27:22.691723 yyxx_game_pkg_dev-2023.6.9.1.dev8/tests/test_ip2region.py
--rw-r--r--   0        0        0      513 2023-06-15 09:27:22.691723 yyxx_game_pkg_dev-2023.6.9.1.dev8/tests/test_logger.py
--rw-r--r--   0        0        0      960 2023-06-15 09:27:22.691723 yyxx_game_pkg_dev-2023.6.9.1.dev8/tests/test_xtrace.py
--rw-r--r--   0        0        0       81 2023-06-15 09:27:22.691723 yyxx_game_pkg_dev-2023.6.9.1.dev8/tests/utils/__init__.py
--rw-r--r--   0        0        0       70 2023-06-15 09:27:22.691723 yyxx_game_pkg_dev-2023.6.9.1.dev8/tests/xcelery/__init__.py
--rw-r--r--   0        0        0       70 2023-06-15 09:27:22.691723 yyxx_game_pkg_dev-2023.6.9.1.dev8/tests/xcelery/config/__init__.py
--rw-r--r--   0        0        0     1226 2023-06-15 09:27:22.691723 yyxx_game_pkg_dev-2023.6.9.1.dev8/tests/xcelery/config/celery_local_config.py
--rw-r--r--   0        0        0      747 2023-06-15 09:27:22.691723 yyxx_game_pkg_dev-2023.6.9.1.dev8/tests/xcelery/task_register.py
--rw-r--r--   0        0        0      299 2023-06-15 09:27:22.691723 yyxx_game_pkg_dev-2023.6.9.1.dev8/tests/xcelery/test_celery.py
--rw-r--r--   0        0        0       69 2023-06-15 09:27:22.691723 yyxx_game_pkg_dev-2023.6.9.1.dev8/yyxx_game_pkg/__init__.py
--rw-r--r--   0        0        0      124 2023-06-15 09:27:22.691723 yyxx_game_pkg_dev-2023.6.9.1.dev8/yyxx_game_pkg/center_api/__init__.py
--rw-r--r--   0        0        0     5166 2023-06-15 09:27:22.695723 yyxx_game_pkg_dev-2023.6.9.1.dev8/yyxx_game_pkg/center_api/model/Operator.py
--rw-r--r--   0        0        0     1505 2023-06-15 09:27:22.695723 yyxx_game_pkg_dev-2023.6.9.1.dev8/yyxx_game_pkg/center_api/model/OperatorServer.py
--rw-r--r--   0        0        0     2572 2023-06-15 09:27:22.695723 yyxx_game_pkg_dev-2023.6.9.1.dev8/yyxx_game_pkg/center_api/model/RechargeConfig.py
--rw-r--r--   0        0        0     2600 2023-06-15 09:27:22.695723 yyxx_game_pkg_dev-2023.6.9.1.dev8/yyxx_game_pkg/center_api/model/TableFieldConf.py
--rw-r--r--   0        0        0      124 2023-06-15 09:27:22.695723 yyxx_game_pkg_dev-2023.6.9.1.dev8/yyxx_game_pkg/center_api/model/__init__.py
--rw-r--r--   0        0        0      124 2023-06-15 09:27:22.695723 yyxx_game_pkg_dev-2023.6.9.1.dev8/yyxx_game_pkg/center_api/sdk/__init__.py
--rw-r--r--   0        0        0     4353 2023-06-15 09:27:22.695723 yyxx_game_pkg_dev-2023.6.9.1.dev8/yyxx_game_pkg/center_api/sdk/check_token.py
--rw-r--r--   0        0        0     5805 2023-06-15 09:27:22.695723 yyxx_game_pkg_dev-2023.6.9.1.dev8/yyxx_game_pkg/center_api/sdk/map_core.py
--rw-r--r--   0        0        0     3506 2023-06-15 09:27:22.695723 yyxx_game_pkg_dev-2023.6.9.1.dev8/yyxx_game_pkg/center_api/sdk/recharge.py
--rw-r--r--   0        0        0     6894 2023-06-15 09:27:22.695723 yyxx_game_pkg_dev-2023.6.9.1.dev8/yyxx_game_pkg/conf/__init__.py
--rw-r--r--   0        0        0     2053 2023-06-15 09:27:22.695723 yyxx_game_pkg_dev-2023.6.9.1.dev8/yyxx_game_pkg/conf/global_settings.py
--rw-r--r--   0        0        0      128 2023-06-15 09:27:22.695723 yyxx_game_pkg_dev-2023.6.9.1.dev8/yyxx_game_pkg/crypto/__init__.py
--rw-r--r--   0        0        0     1164 2023-06-15 09:27:22.695723 yyxx_game_pkg_dev-2023.6.9.1.dev8/yyxx_game_pkg/crypto/aes.py
--rw-r--r--   0        0        0     1113 2023-06-15 09:27:22.695723 yyxx_game_pkg_dev-2023.6.9.1.dev8/yyxx_game_pkg/crypto/basic.py
--rw-r--r--   0        0        0     1351 2023-06-15 09:27:22.695723 yyxx_game_pkg_dev-2023.6.9.1.dev8/yyxx_game_pkg/crypto/make_sign.py
--rw-r--r--   0        0        0     2652 2023-06-15 09:27:22.695723 yyxx_game_pkg_dev-2023.6.9.1.dev8/yyxx_game_pkg/crypto/rsa.py
--rw-r--r--   0        0        0       83 2023-06-15 09:27:22.695723 yyxx_game_pkg_dev-2023.6.9.1.dev8/yyxx_game_pkg/dbops/__init__.py
--rw-r--r--   0        0        0     1331 2023-06-15 09:27:22.695723 yyxx_game_pkg_dev-2023.6.9.1.dev8/yyxx_game_pkg/dbops/base.py
--rw-r--r--   0        0        0     1304 2023-06-15 09:27:22.695723 yyxx_game_pkg_dev-2023.6.9.1.dev8/yyxx_game_pkg/dbops/ch_op.py
--rw-r--r--   0        0        0     5596 2023-06-15 09:27:22.695723 yyxx_game_pkg_dev-2023.6.9.1.dev8/yyxx_game_pkg/dbops/das_api.py
--rw-r--r--   0        0        0     1911 2023-06-15 09:27:22.695723 yyxx_game_pkg_dev-2023.6.9.1.dev8/yyxx_game_pkg/dbops/es_op.py
--rw-r--r--   0        0        0     1678 2023-06-15 09:27:22.695723 yyxx_game_pkg_dev-2023.6.9.1.dev8/yyxx_game_pkg/dbops/hdfs_op.py
--rw-r--r--   0        0        0      979 2023-06-15 09:27:22.695723 yyxx_game_pkg_dev-2023.6.9.1.dev8/yyxx_game_pkg/dbops/mongo_op.py
--rw-r--r--   0        0        0     3955 2023-06-15 09:27:22.695723 yyxx_game_pkg_dev-2023.6.9.1.dev8/yyxx_game_pkg/dbops/mysql_op.py
--rw-r--r--   0        0        0       81 2023-06-15 09:27:22.695723 yyxx_game_pkg_dev-2023.6.9.1.dev8/yyxx_game_pkg/helpers/__init__.py
--rw-r--r--   0        0        0     2686 2023-06-15 09:27:22.695723 yyxx_game_pkg_dev-2023.6.9.1.dev8/yyxx_game_pkg/helpers/mysql_helper.py
--rw-r--r--   0        0        0     3215 2023-06-15 09:27:22.695723 yyxx_game_pkg_dev-2023.6.9.1.dev8/yyxx_game_pkg/helpers/op_helper.py
--rw-r--r--   0        0        0     1266 2023-06-15 09:27:22.695723 yyxx_game_pkg_dev-2023.6.9.1.dev8/yyxx_game_pkg/helpers/pika_helper.py
--rw-r--r--   0        0        0     2966 2023-06-15 09:27:22.695723 yyxx_game_pkg_dev-2023.6.9.1.dev8/yyxx_game_pkg/helpers/redis_helper.py
--rw-r--r--   0        0        0       79 2023-06-15 09:27:22.695723 yyxx_game_pkg_dev-2023.6.9.1.dev8/yyxx_game_pkg/ip2region/__init__.py
--rw-r--r--   0        0        0 11070130 2023-06-15 09:27:22.755724 yyxx_game_pkg_dev-2023.6.9.1.dev8/yyxx_game_pkg/ip2region/ip2region.xdb
--rw-r--r--   0        0        0      604 2023-06-15 09:27:22.755724 yyxx_game_pkg_dev-2023.6.9.1.dev8/yyxx_game_pkg/ip2region/ip_x.py
--rw-r--r--   0        0        0     5735 2023-06-15 09:27:22.755724 yyxx_game_pkg_dev-2023.6.9.1.dev8/yyxx_game_pkg/ip2region/xdbSearcher.py
--rw-r--r--   0        0        0       81 2023-06-15 09:27:22.755724 yyxx_game_pkg_dev-2023.6.9.1.dev8/yyxx_game_pkg/logger/__init__.py
--rw-r--r--   0        0        0     2326 2023-06-15 09:27:22.755724 yyxx_game_pkg_dev-2023.6.9.1.dev8/yyxx_game_pkg/logger/config.py
--rw-r--r--   0        0        0     3467 2023-06-15 09:27:22.755724 yyxx_game_pkg_dev-2023.6.9.1.dev8/yyxx_game_pkg/logger/handlers.py
--rw-r--r--   0        0        0     2154 2023-06-15 09:27:22.755724 yyxx_game_pkg_dev-2023.6.9.1.dev8/yyxx_game_pkg/logger/log.py
--rw-r--r--   0        0        0       70 2023-06-15 09:27:22.755724 yyxx_game_pkg_dev-2023.6.9.1.dev8/yyxx_game_pkg/stat/__init__.py
--rw-r--r--   0        0        0       68 2023-06-15 09:27:22.755724 yyxx_game_pkg_dev-2023.6.9.1.dev8/yyxx_game_pkg/stat/dispatch/__init__.py
--rw-r--r--   0        0        0       70 2023-06-15 09:27:22.755724 yyxx_game_pkg_dev-2023.6.9.1.dev8/yyxx_game_pkg/stat/dispatch/common/__init__.py
--rw-r--r--   0        0        0     1514 2023-06-15 09:27:22.755724 yyxx_game_pkg_dev-2023.6.9.1.dev8/yyxx_game_pkg/stat/dispatch/common/common.py
--rw-r--r--   0        0        0       69 2023-06-15 09:27:22.755724 yyxx_game_pkg_dev-2023.6.9.1.dev8/yyxx_game_pkg/stat/dispatch/core/__init__.py
--rw-r--r--   0        0        0      805 2023-06-15 09:27:22.755724 yyxx_game_pkg_dev-2023.6.9.1.dev8/yyxx_game_pkg/stat/dispatch/core/manager.py
--rw-r--r--   0        0        0     1042 2023-06-15 09:27:22.755724 yyxx_game_pkg_dev-2023.6.9.1.dev8/yyxx_game_pkg/stat/dispatch/core/structs.py
--rw-r--r--   0        0        0     5533 2023-06-15 09:27:22.755724 yyxx_game_pkg_dev-2023.6.9.1.dev8/yyxx_game_pkg/stat/dispatch/core/workflows.py
--rw-r--r--   0        0        0      604 2023-06-15 09:27:22.755724 yyxx_game_pkg_dev-2023.6.9.1.dev8/yyxx_game_pkg/stat/dispatch/dispatch.py
--rw-r--r--   0        0        0       70 2023-06-15 09:27:22.755724 yyxx_game_pkg_dev-2023.6.9.1.dev8/yyxx_game_pkg/stat/dispatch/logic/__init__.py
--rw-r--r--   0        0        0     4402 2023-06-15 09:27:22.755724 yyxx_game_pkg_dev-2023.6.9.1.dev8/yyxx_game_pkg/stat/dispatch/logic/task_logic.py
--rw-r--r--   0        0        0      809 2023-06-15 09:27:22.755724 yyxx_game_pkg_dev-2023.6.9.1.dev8/yyxx_game_pkg/stat/dispatch/route.py
--rw-r--r--   0        0        0      677 2023-06-15 09:27:22.755724 yyxx_game_pkg_dev-2023.6.9.1.dev8/yyxx_game_pkg/stat/dispatch/rules/__init__.py
--rw-r--r--   0        0        0      689 2023-06-15 09:27:22.755724 yyxx_game_pkg_dev-2023.6.9.1.dev8/yyxx_game_pkg/stat/dispatch/rules/rule_base.py
--rw-r--r--   0        0        0     4270 2023-06-15 09:27:22.755724 yyxx_game_pkg_dev-2023.6.9.1.dev8/yyxx_game_pkg/stat/dispatch/rules/rule_workflow.py
--rw-r--r--   0        0        0      667 2023-06-15 09:27:22.755724 yyxx_game_pkg_dev-2023.6.9.1.dev8/yyxx_game_pkg/stat/log.py
--rw-r--r--   0        0        0       70 2023-06-15 09:27:22.755724 yyxx_game_pkg_dev-2023.6.9.1.dev8/yyxx_game_pkg/stat/submit/__init__.py
--rw-r--r--   0        0        0       70 2023-06-15 09:27:22.755724 yyxx_game_pkg_dev-2023.6.9.1.dev8/yyxx_game_pkg/stat/submit/logic/__init__.py
--rw-r--r--   0        0        0     5961 2023-06-15 09:27:22.755724 yyxx_game_pkg_dev-2023.6.9.1.dev8/yyxx_game_pkg/stat/submit/logic/submit_logic.py
--rw-r--r--   0        0        0      987 2023-06-15 09:27:22.759724 yyxx_game_pkg_dev-2023.6.9.1.dev8/yyxx_game_pkg/stat/submit/submit.py
--rw-r--r--   0        0        0       70 2023-06-15 09:27:22.759724 yyxx_game_pkg_dev-2023.6.9.1.dev8/yyxx_game_pkg/stat/xcelery/__init__.py
--rw-r--r--   0        0        0     2206 2023-06-15 09:27:22.759724 yyxx_game_pkg_dev-2023.6.9.1.dev8/yyxx_game_pkg/stat/xcelery/instance.py
--rw-r--r--   0        0        0     1183 2023-06-15 09:27:22.759724 yyxx_game_pkg_dev-2023.6.9.1.dev8/yyxx_game_pkg/stat/xcelery/task_base.py
--rw-r--r--   0        0        0      428 2023-06-15 09:27:22.759724 yyxx_game_pkg_dev-2023.6.9.1.dev8/yyxx_game_pkg/template/__init__.py
--rw-r--r--   0        0        0      132 2023-06-15 09:27:22.759724 yyxx_game_pkg_dev-2023.6.9.1.dev8/yyxx_game_pkg/template/sdk/cookiecutter.json
--rw-r--r--   0        0        0     4023 2023-06-15 09:27:22.759724 yyxx_game_pkg_dev-2023.6.9.1.dev8/yyxx_game_pkg/template/sdk/sdk_{{cookiecutter.sdk_name}}/check_token.py
--rw-r--r--   0        0        0      624 2023-06-15 09:27:22.759724 yyxx_game_pkg_dev-2023.6.9.1.dev8/yyxx_game_pkg/template/sdk/sdk_{{cookiecutter.sdk_name}}/map_factor.py
--rw-r--r--   0        0        0     4077 2023-06-15 09:27:22.759724 yyxx_game_pkg_dev-2023.6.9.1.dev8/yyxx_game_pkg/template/sdk/sdk_{{cookiecutter.sdk_name}}/recharge.py
--rw-r--r--   0        0        0       83 2023-06-15 09:27:22.759724 yyxx_game_pkg_dev-2023.6.9.1.dev8/yyxx_game_pkg/utils/__init__.py
--rw-r--r--   0        0        0     5652 2023-06-15 09:27:22.759724 yyxx_game_pkg_dev-2023.6.9.1.dev8/yyxx_game_pkg/utils/decorator.py
--rw-r--r--   0        0        0     3135 2023-06-15 09:27:22.759724 yyxx_game_pkg_dev-2023.6.9.1.dev8/yyxx_game_pkg/utils/error_code.py
--rw-r--r--   0        0        0     2845 2023-06-15 09:27:22.759724 yyxx_game_pkg_dev-2023.6.9.1.dev8/yyxx_game_pkg/utils/profiler.py
--rw-r--r--   0        0        0     3068 2023-06-15 09:27:22.759724 yyxx_game_pkg_dev-2023.6.9.1.dev8/yyxx_game_pkg/utils/xListStr.py
--rw-r--r--   0        0        0     8845 2023-06-15 09:27:22.759724 yyxx_game_pkg_dev-2023.6.9.1.dev8/yyxx_game_pkg/utils/xdataframe.py
--rw-r--r--   0        0        0     7441 2023-06-15 09:27:22.759724 yyxx_game_pkg_dev-2023.6.9.1.dev8/yyxx_game_pkg/utils/xdate.py
--rw-r--r--   0        0        0     2092 2023-06-15 09:27:22.759724 yyxx_game_pkg_dev-2023.6.9.1.dev8/yyxx_game_pkg/utils/xfutures.py
--rw-r--r--   0        0        0     3653 2023-06-15 09:27:22.759724 yyxx_game_pkg_dev-2023.6.9.1.dev8/yyxx_game_pkg/utils/xhttp.py
--rw-r--r--   0        0        0      971 2023-06-15 09:27:22.759724 yyxx_game_pkg_dev-2023.6.9.1.dev8/yyxx_game_pkg/utils/xmath.py
--rw-r--r--   0        0        0      573 2023-06-15 09:27:22.759724 yyxx_game_pkg_dev-2023.6.9.1.dev8/yyxx_game_pkg/utils/xstring.py
--rw-r--r--   0        0        0       69 2023-06-15 09:27:22.759724 yyxx_game_pkg_dev-2023.6.9.1.dev8/yyxx_game_pkg/xtrace/__init__.py
--rw-r--r--   0        0        0     1895 2023-06-15 09:27:22.759724 yyxx_game_pkg_dev-2023.6.9.1.dev8/yyxx_game_pkg/xtrace/flask/__init__.py
--rw-r--r--   0        0        0     2858 2023-06-15 09:27:22.759724 yyxx_game_pkg_dev-2023.6.9.1.dev8/yyxx_game_pkg/xtrace/helper.py
--rw-r--r--   0        0        0     6934 1970-01-01 00:00:00.000000 yyxx_game_pkg_dev-2023.6.9.1.dev8/PKG-INFO
+-rw-r--r--   0        0        0     4895 2023-07-05 08:07:26.186732 yyxx_game_pkg_dev-2023.7.5.5.dev4/README.md
+-rw-r--r--   0        0        0     1953 2023-07-05 08:07:36.706752 yyxx_game_pkg_dev-2023.7.5.5.dev4/pyproject.toml
+-rw-r--r--   0        0        0       68 2023-07-05 08:07:26.190732 yyxx_game_pkg_dev-2023.7.5.5.dev4/tests/__init__.py
+-rw-r--r--   0        0        0       83 2023-07-05 08:07:26.190732 yyxx_game_pkg_dev-2023.7.5.5.dev4/tests/dbops/__init__.py
+-rw-r--r--   0        0        0     1341 2023-07-05 08:07:26.190732 yyxx_game_pkg_dev-2023.7.5.5.dev4/tests/dbops/mysql_op.py
+-rw-r--r--   0        0        0       70 2023-07-05 08:07:26.190732 yyxx_game_pkg_dev-2023.7.5.5.dev4/tests/dispatch/__init__.py
+-rw-r--r--   0        0        0       70 2023-07-05 08:07:26.190732 yyxx_game_pkg_dev-2023.7.5.5.dev4/tests/dispatch/config/__init__.py
+-rw-r--r--   0        0        0     1228 2023-07-05 08:07:26.190732 yyxx_game_pkg_dev-2023.7.5.5.dev4/tests/dispatch/config/celery_local_config.py
+-rw-r--r--   0        0        0      660 2023-07-05 08:07:26.190732 yyxx_game_pkg_dev-2023.7.5.5.dev4/tests/dispatch/rules/__init__.py
+-rw-r--r--   0        0        0     1348 2023-07-05 08:07:26.190732 yyxx_game_pkg_dev-2023.7.5.5.dev4/tests/dispatch/rules/rule_temp.py
+-rw-r--r--   0        0        0      580 2023-07-05 08:07:26.190732 yyxx_game_pkg_dev-2023.7.5.5.dev4/tests/dispatch/test_dispatch.py
+-rw-r--r--   0        0        0       84 2023-07-05 08:07:26.190732 yyxx_game_pkg_dev-2023.7.5.5.dev4/tests/helpers/__init__.py
+-rw-r--r--   0        0        0      522 2023-07-05 08:07:26.190732 yyxx_game_pkg_dev-2023.7.5.5.dev4/tests/helpers/test_mysql_helper.py
+-rw-r--r--   0        0        0      455 2023-07-05 08:07:26.190732 yyxx_game_pkg_dev-2023.7.5.5.dev4/tests/helpers/test_pika_helper.py
+-rw-r--r--   0        0        0      481 2023-07-05 08:07:26.190732 yyxx_game_pkg_dev-2023.7.5.5.dev4/tests/helpers/test_redis_helper.py
+-rw-r--r--   0        0        0       70 2023-07-05 08:07:26.190732 yyxx_game_pkg_dev-2023.7.5.5.dev4/tests/submit/__init__.py
+-rw-r--r--   0        0        0       70 2023-07-05 08:07:26.190732 yyxx_game_pkg_dev-2023.7.5.5.dev4/tests/submit/schedule_rule/__init__.py
+-rw-r--r--   0        0        0       70 2023-07-05 08:07:26.190732 yyxx_game_pkg_dev-2023.7.5.5.dev4/tests/submit/schedule_rule/schedule/__init__.py
+-rw-r--r--   0        0        0       70 2023-07-05 08:07:26.190732 yyxx_game_pkg_dev-2023.7.5.5.dev4/tests/submit/schedule_rule/schedule/statistic_task/__init__.py
+-rw-r--r--   0        0        0      431 2023-07-05 08:07:26.190732 yyxx_game_pkg_dev-2023.7.5.5.dev4/tests/submit/schedule_rule/schedule/statistic_task/schedule_statistic_collect_test.py
+-rw-r--r--   0        0        0      413 2023-07-05 08:07:26.190732 yyxx_game_pkg_dev-2023.7.5.5.dev4/tests/submit/schedule_rule/schedule/statistic_task/schedule_statistic_task_test.py
+-rw-r--r--   0        0        0       70 2023-07-05 08:07:26.190732 yyxx_game_pkg_dev-2023.7.5.5.dev4/tests/submit/schedule_rule/schedule/work_flow/__init__.py
+-rw-r--r--   0        0        0     1217 2023-07-05 08:07:26.190732 yyxx_game_pkg_dev-2023.7.5.5.dev4/tests/submit/schedule_rule/schedule/work_flow/schedule_work_flow_test.py
+-rw-r--r--   0        0        0      305 2023-07-05 08:07:26.190732 yyxx_game_pkg_dev-2023.7.5.5.dev4/tests/submit/submit.json
+-rw-r--r--   0        0        0     1250 2023-07-05 08:07:26.190732 yyxx_game_pkg_dev-2023.7.5.5.dev4/tests/submit/test_submit.py
+-rw-r--r--   0        0        0      235 2023-07-05 08:07:26.190732 yyxx_game_pkg_dev-2023.7.5.5.dev4/tests/test_ip2region.py
+-rw-r--r--   0        0        0      513 2023-07-05 08:07:26.190732 yyxx_game_pkg_dev-2023.7.5.5.dev4/tests/test_logger.py
+-rw-r--r--   0        0        0      960 2023-07-05 08:07:26.190732 yyxx_game_pkg_dev-2023.7.5.5.dev4/tests/test_xtrace.py
+-rw-r--r--   0        0        0       81 2023-07-05 08:07:26.190732 yyxx_game_pkg_dev-2023.7.5.5.dev4/tests/utils/__init__.py
+-rw-r--r--   0        0        0       70 2023-07-05 08:07:26.190732 yyxx_game_pkg_dev-2023.7.5.5.dev4/tests/xcelery/__init__.py
+-rw-r--r--   0        0        0       70 2023-07-05 08:07:26.190732 yyxx_game_pkg_dev-2023.7.5.5.dev4/tests/xcelery/config/__init__.py
+-rw-r--r--   0        0        0     1226 2023-07-05 08:07:26.190732 yyxx_game_pkg_dev-2023.7.5.5.dev4/tests/xcelery/config/celery_local_config.py
+-rw-r--r--   0        0        0      747 2023-07-05 08:07:26.190732 yyxx_game_pkg_dev-2023.7.5.5.dev4/tests/xcelery/task_register.py
+-rw-r--r--   0        0        0      299 2023-07-05 08:07:26.190732 yyxx_game_pkg_dev-2023.7.5.5.dev4/tests/xcelery/test_celery.py
+-rw-r--r--   0        0        0       69 2023-07-05 08:07:26.190732 yyxx_game_pkg_dev-2023.7.5.5.dev4/yyxx_game_pkg/__init__.py
+-rw-r--r--   0        0        0      124 2023-07-05 08:07:26.190732 yyxx_game_pkg_dev-2023.7.5.5.dev4/yyxx_game_pkg/center_api/__init__.py
+-rw-r--r--   0        0        0     5166 2023-07-05 08:07:26.190732 yyxx_game_pkg_dev-2023.7.5.5.dev4/yyxx_game_pkg/center_api/model/Operator.py
+-rw-r--r--   0        0        0     1505 2023-07-05 08:07:26.190732 yyxx_game_pkg_dev-2023.7.5.5.dev4/yyxx_game_pkg/center_api/model/OperatorServer.py
+-rw-r--r--   0        0        0     2572 2023-07-05 08:07:26.190732 yyxx_game_pkg_dev-2023.7.5.5.dev4/yyxx_game_pkg/center_api/model/RechargeConfig.py
+-rw-r--r--   0        0        0     2600 2023-07-05 08:07:26.190732 yyxx_game_pkg_dev-2023.7.5.5.dev4/yyxx_game_pkg/center_api/model/TableFieldConf.py
+-rw-r--r--   0        0        0      124 2023-07-05 08:07:26.190732 yyxx_game_pkg_dev-2023.7.5.5.dev4/yyxx_game_pkg/center_api/model/__init__.py
+-rw-r--r--   0        0        0      124 2023-07-05 08:07:26.190732 yyxx_game_pkg_dev-2023.7.5.5.dev4/yyxx_game_pkg/center_api/sdk/__init__.py
+-rw-r--r--   0        0        0     4353 2023-07-05 08:07:26.190732 yyxx_game_pkg_dev-2023.7.5.5.dev4/yyxx_game_pkg/center_api/sdk/check_token.py
+-rw-r--r--   0        0        0     5805 2023-07-05 08:07:26.190732 yyxx_game_pkg_dev-2023.7.5.5.dev4/yyxx_game_pkg/center_api/sdk/map_core.py
+-rw-r--r--   0        0        0     3506 2023-07-05 08:07:26.190732 yyxx_game_pkg_dev-2023.7.5.5.dev4/yyxx_game_pkg/center_api/sdk/recharge.py
+-rw-r--r--   0        0        0     6894 2023-07-05 08:07:26.190732 yyxx_game_pkg_dev-2023.7.5.5.dev4/yyxx_game_pkg/conf/__init__.py
+-rw-r--r--   0        0        0     2053 2023-07-05 08:07:26.190732 yyxx_game_pkg_dev-2023.7.5.5.dev4/yyxx_game_pkg/conf/global_settings.py
+-rw-r--r--   0        0        0      128 2023-07-05 08:07:26.190732 yyxx_game_pkg_dev-2023.7.5.5.dev4/yyxx_game_pkg/crypto/__init__.py
+-rw-r--r--   0        0        0     1164 2023-07-05 08:07:26.190732 yyxx_game_pkg_dev-2023.7.5.5.dev4/yyxx_game_pkg/crypto/aes.py
+-rw-r--r--   0        0        0     1113 2023-07-05 08:07:26.190732 yyxx_game_pkg_dev-2023.7.5.5.dev4/yyxx_game_pkg/crypto/basic.py
+-rw-r--r--   0        0        0     1351 2023-07-05 08:07:26.190732 yyxx_game_pkg_dev-2023.7.5.5.dev4/yyxx_game_pkg/crypto/make_sign.py
+-rw-r--r--   0        0        0     2652 2023-07-05 08:07:26.190732 yyxx_game_pkg_dev-2023.7.5.5.dev4/yyxx_game_pkg/crypto/rsa.py
+-rw-r--r--   0        0        0       83 2023-07-05 08:07:26.190732 yyxx_game_pkg_dev-2023.7.5.5.dev4/yyxx_game_pkg/dbops/__init__.py
+-rw-r--r--   0        0        0     1331 2023-07-05 08:07:26.190732 yyxx_game_pkg_dev-2023.7.5.5.dev4/yyxx_game_pkg/dbops/base.py
+-rw-r--r--   0        0        0     1304 2023-07-05 08:07:26.190732 yyxx_game_pkg_dev-2023.7.5.5.dev4/yyxx_game_pkg/dbops/ch_op.py
+-rw-r--r--   0        0        0     5596 2023-07-05 08:07:26.190732 yyxx_game_pkg_dev-2023.7.5.5.dev4/yyxx_game_pkg/dbops/das_api.py
+-rw-r--r--   0        0        0     1911 2023-07-05 08:07:26.190732 yyxx_game_pkg_dev-2023.7.5.5.dev4/yyxx_game_pkg/dbops/es_op.py
+-rw-r--r--   0        0        0     1678 2023-07-05 08:07:26.190732 yyxx_game_pkg_dev-2023.7.5.5.dev4/yyxx_game_pkg/dbops/hdfs_op.py
+-rw-r--r--   0        0        0      149 2023-07-05 08:07:26.190732 yyxx_game_pkg_dev-2023.7.5.5.dev4/yyxx_game_pkg/dbops/mongo_op/__init__.py
+-rw-r--r--   0        0        0     3443 2023-07-05 08:07:26.190732 yyxx_game_pkg_dev-2023.7.5.5.dev4/yyxx_game_pkg/dbops/mongo_op/mongo_op.py
+-rw-r--r--   0        0        0      326 2023-07-05 08:07:26.190732 yyxx_game_pkg_dev-2023.7.5.5.dev4/yyxx_game_pkg/dbops/mongo_op/sql2mongo/__init__.py
+-rw-r--r--   0        0        0    10659 2023-07-05 08:07:26.190732 yyxx_game_pkg_dev-2023.7.5.5.dev4/yyxx_game_pkg/dbops/mongo_op/sql2mongo/sql2mongo.py
+-rw-r--r--   0        0        0     7993 2023-07-05 08:07:26.190732 yyxx_game_pkg_dev-2023.7.5.5.dev4/yyxx_game_pkg/dbops/mongo_op/sql2mongo/test.py
+-rw-r--r--   0        0        0     3955 2023-07-05 08:07:26.190732 yyxx_game_pkg_dev-2023.7.5.5.dev4/yyxx_game_pkg/dbops/mysql_op.py
+-rw-r--r--   0        0        0       81 2023-07-05 08:07:26.190732 yyxx_game_pkg_dev-2023.7.5.5.dev4/yyxx_game_pkg/helpers/__init__.py
+-rw-r--r--   0        0        0     2722 2023-07-05 08:07:26.190732 yyxx_game_pkg_dev-2023.7.5.5.dev4/yyxx_game_pkg/helpers/mysql_helper.py
+-rw-r--r--   0        0        0     3215 2023-07-05 08:07:26.190732 yyxx_game_pkg_dev-2023.7.5.5.dev4/yyxx_game_pkg/helpers/op_helper.py
+-rw-r--r--   0        0        0     1266 2023-07-05 08:07:26.190732 yyxx_game_pkg_dev-2023.7.5.5.dev4/yyxx_game_pkg/helpers/pika_helper.py
+-rw-r--r--   0        0        0     2966 2023-07-05 08:07:26.190732 yyxx_game_pkg_dev-2023.7.5.5.dev4/yyxx_game_pkg/helpers/redis_helper.py
+-rw-r--r--   0        0        0       79 2023-07-05 08:07:26.190732 yyxx_game_pkg_dev-2023.7.5.5.dev4/yyxx_game_pkg/ip2region/__init__.py
+-rw-r--r--   0        0        0 11070130 2023-07-05 08:07:26.258733 yyxx_game_pkg_dev-2023.7.5.5.dev4/yyxx_game_pkg/ip2region/ip2region.xdb
+-rw-r--r--   0        0        0      604 2023-07-05 08:07:26.258733 yyxx_game_pkg_dev-2023.7.5.5.dev4/yyxx_game_pkg/ip2region/ip_x.py
+-rw-r--r--   0        0        0     5735 2023-07-05 08:07:26.258733 yyxx_game_pkg_dev-2023.7.5.5.dev4/yyxx_game_pkg/ip2region/xdbSearcher.py
+-rw-r--r--   0        0        0       81 2023-07-05 08:07:26.258733 yyxx_game_pkg_dev-2023.7.5.5.dev4/yyxx_game_pkg/logger/__init__.py
+-rw-r--r--   0        0        0     2326 2023-07-05 08:07:26.258733 yyxx_game_pkg_dev-2023.7.5.5.dev4/yyxx_game_pkg/logger/config.py
+-rw-r--r--   0        0        0      666 2023-07-05 08:07:26.258733 yyxx_game_pkg_dev-2023.7.5.5.dev4/yyxx_game_pkg/logger/formatters.py
+-rw-r--r--   0        0        0     3467 2023-07-05 08:07:26.258733 yyxx_game_pkg_dev-2023.7.5.5.dev4/yyxx_game_pkg/logger/handlers.py
+-rw-r--r--   0        0        0     2154 2023-07-05 08:07:26.258733 yyxx_game_pkg_dev-2023.7.5.5.dev4/yyxx_game_pkg/logger/log.py
+-rw-r--r--   0        0        0       70 2023-07-05 08:07:26.258733 yyxx_game_pkg_dev-2023.7.5.5.dev4/yyxx_game_pkg/stat/__init__.py
+-rw-r--r--   0        0        0       68 2023-07-05 08:07:26.258733 yyxx_game_pkg_dev-2023.7.5.5.dev4/yyxx_game_pkg/stat/dispatch/__init__.py
+-rw-r--r--   0        0        0       70 2023-07-05 08:07:26.258733 yyxx_game_pkg_dev-2023.7.5.5.dev4/yyxx_game_pkg/stat/dispatch/common/__init__.py
+-rw-r--r--   0        0        0     1514 2023-07-05 08:07:26.258733 yyxx_game_pkg_dev-2023.7.5.5.dev4/yyxx_game_pkg/stat/dispatch/common/common.py
+-rw-r--r--   0        0        0       69 2023-07-05 08:07:26.258733 yyxx_game_pkg_dev-2023.7.5.5.dev4/yyxx_game_pkg/stat/dispatch/core/__init__.py
+-rw-r--r--   0        0        0      805 2023-07-05 08:07:26.258733 yyxx_game_pkg_dev-2023.7.5.5.dev4/yyxx_game_pkg/stat/dispatch/core/manager.py
+-rw-r--r--   0        0        0     1042 2023-07-05 08:07:26.258733 yyxx_game_pkg_dev-2023.7.5.5.dev4/yyxx_game_pkg/stat/dispatch/core/structs.py
+-rw-r--r--   0        0        0     5533 2023-07-05 08:07:26.258733 yyxx_game_pkg_dev-2023.7.5.5.dev4/yyxx_game_pkg/stat/dispatch/core/workflows.py
+-rw-r--r--   0        0        0      604 2023-07-05 08:07:26.258733 yyxx_game_pkg_dev-2023.7.5.5.dev4/yyxx_game_pkg/stat/dispatch/dispatch.py
+-rw-r--r--   0        0        0       70 2023-07-05 08:07:26.258733 yyxx_game_pkg_dev-2023.7.5.5.dev4/yyxx_game_pkg/stat/dispatch/logic/__init__.py
+-rw-r--r--   0        0        0     4402 2023-07-05 08:07:26.258733 yyxx_game_pkg_dev-2023.7.5.5.dev4/yyxx_game_pkg/stat/dispatch/logic/task_logic.py
+-rw-r--r--   0        0        0      809 2023-07-05 08:07:26.258733 yyxx_game_pkg_dev-2023.7.5.5.dev4/yyxx_game_pkg/stat/dispatch/route.py
+-rw-r--r--   0        0        0      677 2023-07-05 08:07:26.258733 yyxx_game_pkg_dev-2023.7.5.5.dev4/yyxx_game_pkg/stat/dispatch/rules/__init__.py
+-rw-r--r--   0        0        0      689 2023-07-05 08:07:26.258733 yyxx_game_pkg_dev-2023.7.5.5.dev4/yyxx_game_pkg/stat/dispatch/rules/rule_base.py
+-rw-r--r--   0        0        0     4270 2023-07-05 08:07:26.258733 yyxx_game_pkg_dev-2023.7.5.5.dev4/yyxx_game_pkg/stat/dispatch/rules/rule_workflow.py
+-rw-r--r--   0        0        0      667 2023-07-05 08:07:26.258733 yyxx_game_pkg_dev-2023.7.5.5.dev4/yyxx_game_pkg/stat/log.py
+-rw-r--r--   0        0        0       70 2023-07-05 08:07:26.258733 yyxx_game_pkg_dev-2023.7.5.5.dev4/yyxx_game_pkg/stat/submit/__init__.py
+-rw-r--r--   0        0        0       70 2023-07-05 08:07:26.258733 yyxx_game_pkg_dev-2023.7.5.5.dev4/yyxx_game_pkg/stat/submit/logic/__init__.py
+-rw-r--r--   0        0        0     5961 2023-07-05 08:07:26.258733 yyxx_game_pkg_dev-2023.7.5.5.dev4/yyxx_game_pkg/stat/submit/logic/submit_logic.py
+-rw-r--r--   0        0        0      987 2023-07-05 08:07:26.258733 yyxx_game_pkg_dev-2023.7.5.5.dev4/yyxx_game_pkg/stat/submit/submit.py
+-rw-r--r--   0        0        0       70 2023-07-05 08:07:26.258733 yyxx_game_pkg_dev-2023.7.5.5.dev4/yyxx_game_pkg/stat/xcelery/__init__.py
+-rw-r--r--   0        0        0     2206 2023-07-05 08:07:26.258733 yyxx_game_pkg_dev-2023.7.5.5.dev4/yyxx_game_pkg/stat/xcelery/instance.py
+-rw-r--r--   0        0        0     1183 2023-07-05 08:07:26.258733 yyxx_game_pkg_dev-2023.7.5.5.dev4/yyxx_game_pkg/stat/xcelery/task_base.py
+-rw-r--r--   0        0        0      428 2023-07-05 08:07:26.258733 yyxx_game_pkg_dev-2023.7.5.5.dev4/yyxx_game_pkg/template/__init__.py
+-rw-r--r--   0        0        0      132 2023-07-05 08:07:26.258733 yyxx_game_pkg_dev-2023.7.5.5.dev4/yyxx_game_pkg/template/sdk/cookiecutter.json
+-rw-r--r--   0        0        0     4023 2023-07-05 08:07:26.258733 yyxx_game_pkg_dev-2023.7.5.5.dev4/yyxx_game_pkg/template/sdk/sdk_{{cookiecutter.sdk_name}}/check_token.py
+-rw-r--r--   0        0        0      624 2023-07-05 08:07:26.258733 yyxx_game_pkg_dev-2023.7.5.5.dev4/yyxx_game_pkg/template/sdk/sdk_{{cookiecutter.sdk_name}}/map_factor.py
+-rw-r--r--   0        0        0     4077 2023-07-05 08:07:26.258733 yyxx_game_pkg_dev-2023.7.5.5.dev4/yyxx_game_pkg/template/sdk/sdk_{{cookiecutter.sdk_name}}/recharge.py
+-rw-r--r--   0        0        0       83 2023-07-05 08:07:26.258733 yyxx_game_pkg_dev-2023.7.5.5.dev4/yyxx_game_pkg/utils/__init__.py
+-rw-r--r--   0        0        0     5650 2023-07-05 08:07:26.258733 yyxx_game_pkg_dev-2023.7.5.5.dev4/yyxx_game_pkg/utils/decorator.py
+-rw-r--r--   0        0        0     3135 2023-07-05 08:07:26.258733 yyxx_game_pkg_dev-2023.7.5.5.dev4/yyxx_game_pkg/utils/error_code.py
+-rw-r--r--   0        0        0     2845 2023-07-05 08:07:26.258733 yyxx_game_pkg_dev-2023.7.5.5.dev4/yyxx_game_pkg/utils/profiler.py
+-rw-r--r--   0        0        0     3068 2023-07-05 08:07:26.262733 yyxx_game_pkg_dev-2023.7.5.5.dev4/yyxx_game_pkg/utils/xListStr.py
+-rw-r--r--   0        0        0     9461 2023-07-05 08:07:26.262733 yyxx_game_pkg_dev-2023.7.5.5.dev4/yyxx_game_pkg/utils/xdataframe.py
+-rw-r--r--   0        0        0     7441 2023-07-05 08:07:26.262733 yyxx_game_pkg_dev-2023.7.5.5.dev4/yyxx_game_pkg/utils/xdate.py
+-rw-r--r--   0        0        0     2092 2023-07-05 08:07:26.262733 yyxx_game_pkg_dev-2023.7.5.5.dev4/yyxx_game_pkg/utils/xfutures.py
+-rw-r--r--   0        0        0     3653 2023-07-05 08:07:26.262733 yyxx_game_pkg_dev-2023.7.5.5.dev4/yyxx_game_pkg/utils/xhttp.py
+-rw-r--r--   0        0        0      971 2023-07-05 08:07:26.262733 yyxx_game_pkg_dev-2023.7.5.5.dev4/yyxx_game_pkg/utils/xmath.py
+-rw-r--r--   0        0        0      573 2023-07-05 08:07:26.262733 yyxx_game_pkg_dev-2023.7.5.5.dev4/yyxx_game_pkg/utils/xstring.py
+-rw-r--r--   0        0        0       69 2023-07-05 08:07:26.262733 yyxx_game_pkg_dev-2023.7.5.5.dev4/yyxx_game_pkg/xtrace/__init__.py
+-rw-r--r--   0        0        0     1570 2023-07-05 08:07:26.262733 yyxx_game_pkg_dev-2023.7.5.5.dev4/yyxx_game_pkg/xtrace/django/__init__.py
+-rw-r--r--   0        0        0     2669 2023-07-05 08:07:26.262733 yyxx_game_pkg_dev-2023.7.5.5.dev4/yyxx_game_pkg/xtrace/django/middleware.py
+-rw-r--r--   0        0        0       71 2023-07-05 08:07:26.262733 yyxx_game_pkg_dev-2023.7.5.5.dev4/yyxx_game_pkg/xtrace/django/util/__init__.py
+-rw-r--r--   0        0        0      564 2023-07-05 08:07:26.262733 yyxx_game_pkg_dev-2023.7.5.5.dev4/yyxx_game_pkg/xtrace/django/util/common.py
+-rw-r--r--   0        0        0      663 2023-07-05 08:07:26.262733 yyxx_game_pkg_dev-2023.7.5.5.dev4/yyxx_game_pkg/xtrace/django/util/log_handlers.py
+-rw-r--r--   0        0        0     1994 2023-07-05 08:07:26.262733 yyxx_game_pkg_dev-2023.7.5.5.dev4/yyxx_game_pkg/xtrace/flask/__init__.py
+-rw-r--r--   0        0        0     2969 2023-07-05 08:07:26.262733 yyxx_game_pkg_dev-2023.7.5.5.dev4/yyxx_game_pkg/xtrace/helper.py
+-rw-r--r--   0        0        0     7125 1970-01-01 00:00:00.000000 yyxx_game_pkg_dev-2023.7.5.5.dev4/PKG-INFO
```

### Comparing `yyxx_game_pkg_dev-2023.6.9.1.dev8/README.md` & `yyxx_game_pkg_dev-2023.7.5.5.dev4/README.md`

 * *Files identical despite different names*

### Comparing `yyxx_game_pkg_dev-2023.6.9.1.dev8/pyproject.toml` & `yyxx_game_pkg_dev-2023.7.5.5.dev4/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = [ "poetry-core",]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry]
 name = "yyxx-game-pkg-dev"
-version = "v2023.06.09.001dev8"
+version = "v2023.07.05.005dev4"
 description = "yyxx game custom module"
 authors = [ "yyxx-game",]
 license = "MIT"
 homepage = "https://github.com/yyxxgame/yyxxgame-pkg"
 repository = "https://github.com/yyxxgame/yyxxgame-pkg"
 readme = "README.md"
 classifiers = [ "Programming Language :: Python :: 3", "License :: OSI Approved :: MIT License", "Operating System :: OS Independent",]
@@ -24,25 +24,29 @@
 opentelemetry-api = "^1.16.0"
 opentelemetry-sdk = "^1.16.0"
 opentelemetry-exporter-jaeger = "^1.16.0"
 opentelemetry-instrumentation-requests = "^0.37b0"
 opentelemetry-instrumentation-fastapi = "0.37b.0"
 opentelemetry-instrumentation-celery = "0.37b0"
 opentelemetry-instrumentation-flask = "^0.37b0"
+opentelemetry-instrumentation-django = "^0.37b0"
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
+pyparsing = "^3.1.0"
 
 [tool.poetry.extras]
 stat = [ "fastapi",]
 server_center = [ "django", "pillow", "filetype",]
 center_api = [ "flask", "cookiecutter",]
 
 [tool.poetry.dependencies.fastapi]
```

### Comparing `yyxx_game_pkg_dev-2023.6.9.1.dev8/tests/dbops/mysql_op.py` & `yyxx_game_pkg_dev-2023.7.5.5.dev4/tests/dbops/mysql_op.py`

 * *Files identical despite different names*

### Comparing `yyxx_game_pkg_dev-2023.6.9.1.dev8/tests/dispatch/config/celery_local_config.py` & `yyxx_game_pkg_dev-2023.7.5.5.dev4/tests/dispatch/config/celery_local_config.py`

 * *Files identical despite different names*

### Comparing `yyxx_game_pkg_dev-2023.6.9.1.dev8/tests/dispatch/rules/__init__.py` & `yyxx_game_pkg_dev-2023.7.5.5.dev4/tests/dispatch/rules/__init__.py`

 * *Files identical despite different names*

### Comparing `yyxx_game_pkg_dev-2023.6.9.1.dev8/tests/dispatch/rules/rule_temp.py` & `yyxx_game_pkg_dev-2023.7.5.5.dev4/tests/dispatch/rules/rule_temp.py`

 * *Files identical despite different names*

### Comparing `yyxx_game_pkg_dev-2023.6.9.1.dev8/tests/dispatch/test_dispatch.py` & `yyxx_game_pkg_dev-2023.7.5.5.dev4/tests/dispatch/test_dispatch.py`

 * *Files identical despite different names*

### Comparing `yyxx_game_pkg_dev-2023.6.9.1.dev8/tests/helpers/test_mysql_helper.py` & `yyxx_game_pkg_dev-2023.7.5.5.dev4/tests/helpers/test_mysql_helper.py`

 * *Files identical despite different names*

### Comparing `yyxx_game_pkg_dev-2023.6.9.1.dev8/tests/submit/schedule_rule/schedule/work_flow/schedule_work_flow_test.py` & `yyxx_game_pkg_dev-2023.7.5.5.dev4/tests/submit/schedule_rule/schedule/work_flow/schedule_work_flow_test.py`

 * *Files identical despite different names*

### Comparing `yyxx_game_pkg_dev-2023.6.9.1.dev8/tests/submit/test_submit.py` & `yyxx_game_pkg_dev-2023.7.5.5.dev4/tests/submit/test_submit.py`

 * *Files identical despite different names*

### Comparing `yyxx_game_pkg_dev-2023.6.9.1.dev8/tests/test_logger.py` & `yyxx_game_pkg_dev-2023.7.5.5.dev4/tests/test_logger.py`

 * *Files identical despite different names*

### Comparing `yyxx_game_pkg_dev-2023.6.9.1.dev8/tests/test_xtrace.py` & `yyxx_game_pkg_dev-2023.7.5.5.dev4/tests/test_xtrace.py`

 * *Files identical despite different names*

### Comparing `yyxx_game_pkg_dev-2023.6.9.1.dev8/tests/xcelery/config/celery_local_config.py` & `yyxx_game_pkg_dev-2023.7.5.5.dev4/tests/xcelery/config/celery_local_config.py`

 * *Files identical despite different names*

### Comparing `yyxx_game_pkg_dev-2023.6.9.1.dev8/tests/xcelery/task_register.py` & `yyxx_game_pkg_dev-2023.7.5.5.dev4/tests/xcelery/task_register.py`

 * *Files identical despite different names*

### Comparing `yyxx_game_pkg_dev-2023.6.9.1.dev8/yyxx_game_pkg/center_api/model/Operator.py` & `yyxx_game_pkg_dev-2023.7.5.5.dev4/yyxx_game_pkg/center_api/model/Operator.py`

 * *Files identical despite different names*

### Comparing `yyxx_game_pkg_dev-2023.6.9.1.dev8/yyxx_game_pkg/center_api/model/OperatorServer.py` & `yyxx_game_pkg_dev-2023.7.5.5.dev4/yyxx_game_pkg/center_api/model/OperatorServer.py`

 * *Files identical despite different names*

### Comparing `yyxx_game_pkg_dev-2023.6.9.1.dev8/yyxx_game_pkg/center_api/model/RechargeConfig.py` & `yyxx_game_pkg_dev-2023.7.5.5.dev4/yyxx_game_pkg/center_api/model/RechargeConfig.py`

 * *Files identical despite different names*

### Comparing `yyxx_game_pkg_dev-2023.6.9.1.dev8/yyxx_game_pkg/center_api/model/TableFieldConf.py` & `yyxx_game_pkg_dev-2023.7.5.5.dev4/yyxx_game_pkg/center_api/model/TableFieldConf.py`

 * *Files identical despite different names*

### Comparing `yyxx_game_pkg_dev-2023.6.9.1.dev8/yyxx_game_pkg/center_api/sdk/check_token.py` & `yyxx_game_pkg_dev-2023.7.5.5.dev4/yyxx_game_pkg/center_api/sdk/check_token.py`

 * *Files identical despite different names*

### Comparing `yyxx_game_pkg_dev-2023.6.9.1.dev8/yyxx_game_pkg/center_api/sdk/map_core.py` & `yyxx_game_pkg_dev-2023.7.5.5.dev4/yyxx_game_pkg/center_api/sdk/map_core.py`

 * *Files identical despite different names*

### Comparing `yyxx_game_pkg_dev-2023.6.9.1.dev8/yyxx_game_pkg/center_api/sdk/recharge.py` & `yyxx_game_pkg_dev-2023.7.5.5.dev4/yyxx_game_pkg/center_api/sdk/recharge.py`

 * *Files identical despite different names*

### Comparing `yyxx_game_pkg_dev-2023.6.9.1.dev8/yyxx_game_pkg/conf/__init__.py` & `yyxx_game_pkg_dev-2023.7.5.5.dev4/yyxx_game_pkg/conf/__init__.py`

 * *Files identical despite different names*

### Comparing `yyxx_game_pkg_dev-2023.6.9.1.dev8/yyxx_game_pkg/conf/global_settings.py` & `yyxx_game_pkg_dev-2023.7.5.5.dev4/yyxx_game_pkg/conf/global_settings.py`

 * *Files identical despite different names*

### Comparing `yyxx_game_pkg_dev-2023.6.9.1.dev8/yyxx_game_pkg/crypto/aes.py` & `yyxx_game_pkg_dev-2023.7.5.5.dev4/yyxx_game_pkg/crypto/aes.py`

 * *Files identical despite different names*

### Comparing `yyxx_game_pkg_dev-2023.6.9.1.dev8/yyxx_game_pkg/crypto/basic.py` & `yyxx_game_pkg_dev-2023.7.5.5.dev4/yyxx_game_pkg/crypto/basic.py`

 * *Files identical despite different names*

### Comparing `yyxx_game_pkg_dev-2023.6.9.1.dev8/yyxx_game_pkg/crypto/make_sign.py` & `yyxx_game_pkg_dev-2023.7.5.5.dev4/yyxx_game_pkg/crypto/make_sign.py`

 * *Files identical despite different names*

### Comparing `yyxx_game_pkg_dev-2023.6.9.1.dev8/yyxx_game_pkg/crypto/rsa.py` & `yyxx_game_pkg_dev-2023.7.5.5.dev4/yyxx_game_pkg/crypto/rsa.py`

 * *Files identical despite different names*

### Comparing `yyxx_game_pkg_dev-2023.6.9.1.dev8/yyxx_game_pkg/dbops/base.py` & `yyxx_game_pkg_dev-2023.7.5.5.dev4/yyxx_game_pkg/dbops/base.py`

 * *Files identical despite different names*

### Comparing `yyxx_game_pkg_dev-2023.6.9.1.dev8/yyxx_game_pkg/dbops/ch_op.py` & `yyxx_game_pkg_dev-2023.7.5.5.dev4/yyxx_game_pkg/dbops/ch_op.py`

 * *Files identical despite different names*

### Comparing `yyxx_game_pkg_dev-2023.6.9.1.dev8/yyxx_game_pkg/dbops/das_api.py` & `yyxx_game_pkg_dev-2023.7.5.5.dev4/yyxx_game_pkg/dbops/das_api.py`

 * *Files identical despite different names*

### Comparing `yyxx_game_pkg_dev-2023.6.9.1.dev8/yyxx_game_pkg/dbops/es_op.py` & `yyxx_game_pkg_dev-2023.7.5.5.dev4/yyxx_game_pkg/dbops/es_op.py`

 * *Files identical despite different names*

### Comparing `yyxx_game_pkg_dev-2023.6.9.1.dev8/yyxx_game_pkg/dbops/hdfs_op.py` & `yyxx_game_pkg_dev-2023.7.5.5.dev4/yyxx_game_pkg/dbops/hdfs_op.py`

 * *Files identical despite different names*

### Comparing `yyxx_game_pkg_dev-2023.6.9.1.dev8/yyxx_game_pkg/dbops/mysql_op.py` & `yyxx_game_pkg_dev-2023.7.5.5.dev4/yyxx_game_pkg/dbops/mysql_op.py`

 * *Files identical despite different names*

### Comparing `yyxx_game_pkg_dev-2023.6.9.1.dev8/yyxx_game_pkg/helpers/mysql_helper.py` & `yyxx_game_pkg_dev-2023.7.5.5.dev4/yyxx_game_pkg/helpers/mysql_helper.py`

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

### Comparing `yyxx_game_pkg_dev-2023.6.9.1.dev8/yyxx_game_pkg/helpers/op_helper.py` & `yyxx_game_pkg_dev-2023.7.5.5.dev4/yyxx_game_pkg/helpers/op_helper.py`

 * *Files identical despite different names*

### Comparing `yyxx_game_pkg_dev-2023.6.9.1.dev8/yyxx_game_pkg/helpers/pika_helper.py` & `yyxx_game_pkg_dev-2023.7.5.5.dev4/yyxx_game_pkg/helpers/pika_helper.py`

 * *Files identical despite different names*

### Comparing `yyxx_game_pkg_dev-2023.6.9.1.dev8/yyxx_game_pkg/helpers/redis_helper.py` & `yyxx_game_pkg_dev-2023.7.5.5.dev4/yyxx_game_pkg/helpers/redis_helper.py`

 * *Files identical despite different names*

### Comparing `yyxx_game_pkg_dev-2023.6.9.1.dev8/yyxx_game_pkg/ip2region/ip2region.xdb` & `yyxx_game_pkg_dev-2023.7.5.5.dev4/yyxx_game_pkg/ip2region/ip2region.xdb`

 * *Files identical despite different names*

### Comparing `yyxx_game_pkg_dev-2023.6.9.1.dev8/yyxx_game_pkg/ip2region/ip_x.py` & `yyxx_game_pkg_dev-2023.7.5.5.dev4/yyxx_game_pkg/ip2region/ip_x.py`

 * *Files identical despite different names*

### Comparing `yyxx_game_pkg_dev-2023.6.9.1.dev8/yyxx_game_pkg/ip2region/xdbSearcher.py` & `yyxx_game_pkg_dev-2023.7.5.5.dev4/yyxx_game_pkg/ip2region/xdbSearcher.py`

 * *Files identical despite different names*

### Comparing `yyxx_game_pkg_dev-2023.6.9.1.dev8/yyxx_game_pkg/logger/config.py` & `yyxx_game_pkg_dev-2023.7.5.5.dev4/yyxx_game_pkg/logger/config.py`

 * *Files identical despite different names*

### Comparing `yyxx_game_pkg_dev-2023.6.9.1.dev8/yyxx_game_pkg/logger/handlers.py` & `yyxx_game_pkg_dev-2023.7.5.5.dev4/yyxx_game_pkg/logger/handlers.py`

 * *Files identical despite different names*

### Comparing `yyxx_game_pkg_dev-2023.6.9.1.dev8/yyxx_game_pkg/logger/log.py` & `yyxx_game_pkg_dev-2023.7.5.5.dev4/yyxx_game_pkg/logger/log.py`

 * *Files identical despite different names*

### Comparing `yyxx_game_pkg_dev-2023.6.9.1.dev8/yyxx_game_pkg/stat/dispatch/common/common.py` & `yyxx_game_pkg_dev-2023.7.5.5.dev4/yyxx_game_pkg/stat/dispatch/common/common.py`

 * *Files identical despite different names*

### Comparing `yyxx_game_pkg_dev-2023.6.9.1.dev8/yyxx_game_pkg/stat/dispatch/core/manager.py` & `yyxx_game_pkg_dev-2023.7.5.5.dev4/yyxx_game_pkg/stat/dispatch/core/manager.py`

 * *Files identical despite different names*

### Comparing `yyxx_game_pkg_dev-2023.6.9.1.dev8/yyxx_game_pkg/stat/dispatch/core/structs.py` & `yyxx_game_pkg_dev-2023.7.5.5.dev4/yyxx_game_pkg/stat/dispatch/core/structs.py`

 * *Files identical despite different names*

### Comparing `yyxx_game_pkg_dev-2023.6.9.1.dev8/yyxx_game_pkg/stat/dispatch/core/workflows.py` & `yyxx_game_pkg_dev-2023.7.5.5.dev4/yyxx_game_pkg/stat/dispatch/core/workflows.py`

 * *Files identical despite different names*

### Comparing `yyxx_game_pkg_dev-2023.6.9.1.dev8/yyxx_game_pkg/stat/dispatch/dispatch.py` & `yyxx_game_pkg_dev-2023.7.5.5.dev4/yyxx_game_pkg/stat/dispatch/dispatch.py`

 * *Files identical despite different names*

### Comparing `yyxx_game_pkg_dev-2023.6.9.1.dev8/yyxx_game_pkg/stat/dispatch/logic/task_logic.py` & `yyxx_game_pkg_dev-2023.7.5.5.dev4/yyxx_game_pkg/stat/dispatch/logic/task_logic.py`

 * *Files identical despite different names*

### Comparing `yyxx_game_pkg_dev-2023.6.9.1.dev8/yyxx_game_pkg/stat/dispatch/route.py` & `yyxx_game_pkg_dev-2023.7.5.5.dev4/yyxx_game_pkg/stat/dispatch/route.py`

 * *Files identical despite different names*

### Comparing `yyxx_game_pkg_dev-2023.6.9.1.dev8/yyxx_game_pkg/stat/dispatch/rules/__init__.py` & `yyxx_game_pkg_dev-2023.7.5.5.dev4/yyxx_game_pkg/stat/dispatch/rules/__init__.py`

 * *Files identical despite different names*

### Comparing `yyxx_game_pkg_dev-2023.6.9.1.dev8/yyxx_game_pkg/stat/dispatch/rules/rule_base.py` & `yyxx_game_pkg_dev-2023.7.5.5.dev4/yyxx_game_pkg/stat/dispatch/rules/rule_base.py`

 * *Files identical despite different names*

### Comparing `yyxx_game_pkg_dev-2023.6.9.1.dev8/yyxx_game_pkg/stat/dispatch/rules/rule_workflow.py` & `yyxx_game_pkg_dev-2023.7.5.5.dev4/yyxx_game_pkg/stat/dispatch/rules/rule_workflow.py`

 * *Files identical despite different names*

### Comparing `yyxx_game_pkg_dev-2023.6.9.1.dev8/yyxx_game_pkg/stat/log.py` & `yyxx_game_pkg_dev-2023.7.5.5.dev4/yyxx_game_pkg/stat/log.py`

 * *Files identical despite different names*

### Comparing `yyxx_game_pkg_dev-2023.6.9.1.dev8/yyxx_game_pkg/stat/submit/logic/submit_logic.py` & `yyxx_game_pkg_dev-2023.7.5.5.dev4/yyxx_game_pkg/stat/submit/logic/submit_logic.py`

 * *Files identical despite different names*

### Comparing `yyxx_game_pkg_dev-2023.6.9.1.dev8/yyxx_game_pkg/stat/submit/submit.py` & `yyxx_game_pkg_dev-2023.7.5.5.dev4/yyxx_game_pkg/stat/submit/submit.py`

 * *Files identical despite different names*

### Comparing `yyxx_game_pkg_dev-2023.6.9.1.dev8/yyxx_game_pkg/stat/xcelery/instance.py` & `yyxx_game_pkg_dev-2023.7.5.5.dev4/yyxx_game_pkg/stat/xcelery/instance.py`

 * *Files identical despite different names*

### Comparing `yyxx_game_pkg_dev-2023.6.9.1.dev8/yyxx_game_pkg/stat/xcelery/task_base.py` & `yyxx_game_pkg_dev-2023.7.5.5.dev4/yyxx_game_pkg/stat/xcelery/task_base.py`

 * *Files identical despite different names*

### Comparing `yyxx_game_pkg_dev-2023.6.9.1.dev8/yyxx_game_pkg/template/sdk/sdk_{{cookiecutter.sdk_name}}/check_token.py` & `yyxx_game_pkg_dev-2023.7.5.5.dev4/yyxx_game_pkg/template/sdk/sdk_{{cookiecutter.sdk_name}}/check_token.py`

 * *Files identical despite different names*

### Comparing `yyxx_game_pkg_dev-2023.6.9.1.dev8/yyxx_game_pkg/template/sdk/sdk_{{cookiecutter.sdk_name}}/map_factor.py` & `yyxx_game_pkg_dev-2023.7.5.5.dev4/yyxx_game_pkg/template/sdk/sdk_{{cookiecutter.sdk_name}}/map_factor.py`

 * *Files identical despite different names*

### Comparing `yyxx_game_pkg_dev-2023.6.9.1.dev8/yyxx_game_pkg/template/sdk/sdk_{{cookiecutter.sdk_name}}/recharge.py` & `yyxx_game_pkg_dev-2023.7.5.5.dev4/yyxx_game_pkg/template/sdk/sdk_{{cookiecutter.sdk_name}}/recharge.py`

 * *Files identical despite different names*

### Comparing `yyxx_game_pkg_dev-2023.6.9.1.dev8/yyxx_game_pkg/utils/decorator.py` & `yyxx_game_pkg_dev-2023.7.5.5.dev4/yyxx_game_pkg/utils/decorator.py`

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

### Comparing `yyxx_game_pkg_dev-2023.6.9.1.dev8/yyxx_game_pkg/utils/error_code.py` & `yyxx_game_pkg_dev-2023.7.5.5.dev4/yyxx_game_pkg/utils/error_code.py`

 * *Files identical despite different names*

### Comparing `yyxx_game_pkg_dev-2023.6.9.1.dev8/yyxx_game_pkg/utils/profiler.py` & `yyxx_game_pkg_dev-2023.7.5.5.dev4/yyxx_game_pkg/utils/profiler.py`

 * *Files identical despite different names*

### Comparing `yyxx_game_pkg_dev-2023.6.9.1.dev8/yyxx_game_pkg/utils/xListStr.py` & `yyxx_game_pkg_dev-2023.7.5.5.dev4/yyxx_game_pkg/utils/xListStr.py`

 * *Files identical despite different names*

### Comparing `yyxx_game_pkg_dev-2023.6.9.1.dev8/yyxx_game_pkg/utils/xdataframe.py` & `yyxx_game_pkg_dev-2023.7.5.5.dev4/yyxx_game_pkg/utils/xdataframe.py`

 * *Files 4% similar despite different names*

```diff
@@ -315,7 +315,23 @@
             res = data_df[col].astype(str)
         else:
             res = res + data_df[col].astype(str)
         if col == cols[-1]:
             continue
         res = res + concat_by
     return res
+
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

### Comparing `yyxx_game_pkg_dev-2023.6.9.1.dev8/yyxx_game_pkg/utils/xdate.py` & `yyxx_game_pkg_dev-2023.7.5.5.dev4/yyxx_game_pkg/utils/xdate.py`

 * *Files identical despite different names*

### Comparing `yyxx_game_pkg_dev-2023.6.9.1.dev8/yyxx_game_pkg/utils/xfutures.py` & `yyxx_game_pkg_dev-2023.7.5.5.dev4/yyxx_game_pkg/utils/xfutures.py`

 * *Files identical despite different names*

### Comparing `yyxx_game_pkg_dev-2023.6.9.1.dev8/yyxx_game_pkg/utils/xhttp.py` & `yyxx_game_pkg_dev-2023.7.5.5.dev4/yyxx_game_pkg/utils/xhttp.py`

 * *Files identical despite different names*

### Comparing `yyxx_game_pkg_dev-2023.6.9.1.dev8/yyxx_game_pkg/utils/xmath.py` & `yyxx_game_pkg_dev-2023.7.5.5.dev4/yyxx_game_pkg/utils/xmath.py`

 * *Files identical despite different names*

### Comparing `yyxx_game_pkg_dev-2023.6.9.1.dev8/yyxx_game_pkg/utils/xstring.py` & `yyxx_game_pkg_dev-2023.7.5.5.dev4/yyxx_game_pkg/utils/xstring.py`

 * *Files identical despite different names*

### Comparing `yyxx_game_pkg_dev-2023.6.9.1.dev8/yyxx_game_pkg/xtrace/flask/__init__.py` & `yyxx_game_pkg_dev-2023.7.5.5.dev4/yyxx_game_pkg/xtrace/flask/__init__.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,40 +1,43 @@
 # -*- coding: utf-8 -*-
 # @Author   : LvWenQi
 # @Time     : 2023/06/12
 
 import json
 from flask import g, current_app
-from yyxx_game_pkg.xtrace import helper
+from opentelemetry.instrumentation.flask import FlaskInstrumentor
 from opentelemetry.trace import get_current_span
 from opentelemetry.trace.propagation.tracecontext import TraceContextTextMapPropagator
-from opentelemetry.instrumentation.flask import FlaskInstrumentor
+
+from yyxx_game_pkg.xtrace import helper
 
 
 class FlaskJaegerInstrumentor:
     def __init__(self):
         pass
 
     @staticmethod
     def _after_request(response):
         try:
-            log_max_size = current_app.config["JAEGER"].get("log_max_size", 2048)
+            jaeger_config = current_app.config["JAEGER"]
+            log_max_size = jaeger_config.get("log_max_size", 2048)
             span = get_current_span()
             # request event
             request_params = g.get("request_params")
             if request_params:
                 try:
                     request_params = json.dumps(request_params, ensure_ascii=False)
                 except Exception as e:
                     print(e)
                 span.add_event("request", {"params": str(request_params)[:log_max_size]})
             # response event
-            response_params = g.get("response_params")
-            if response_params:
-                span.add_event("response", {"params": str(response_params)[:log_max_size]})
+            if jaeger_config.get("is_log"):
+                response_params = g.get("response_params")
+                if response_params:
+                    span.add_event("response", {"params": str(response_params)[:log_max_size]})
             # inject trace parent to response header
             TraceContextTextMapPropagator().inject(response.headers)
         except Exception as e:
             print(e)
         return response
 
     def instrument(self, app):
```

### Comparing `yyxx_game_pkg_dev-2023.6.9.1.dev8/yyxx_game_pkg/xtrace/helper.py` & `yyxx_game_pkg_dev-2023.7.5.5.dev4/yyxx_game_pkg/xtrace/helper.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,21 +1,19 @@
 # -*- coding: utf-8 -*-
 # @Author   : KaiShin
 # @Time     : 2023/2/28
 
 from functools import wraps
-
 from opentelemetry import trace
 from opentelemetry.exporter.jaeger.thrift import JaegerExporter
 from opentelemetry.sdk.resources import SERVICE_NAME, Resource
 from opentelemetry.sdk.trace import TracerProvider
 from opentelemetry.sdk.trace.export import BatchSpanProcessor
-from opentelemetry.trace.status import Status, StatusCode
 from opentelemetry.trace import get_current_span
-
+from opentelemetry.trace.status import Status, StatusCode
 
 _tracer = trace.get_tracer(__name__)
 
 
 def get_tracer():
     """:cvar
     获取全局tracer实例
@@ -46,24 +44,26 @@
     # Create a BatchSpanProcessor and add the exporter to it
     span_processor = BatchSpanProcessor(jaeger_exporter)
 
     # add to the tracer
     trace.get_tracer_provider().add_span_processor(span_processor)
 
 
-def trace_span(ret_trace_id: bool = False, set_attributes: bool = False):
+def trace_span(ret_trace_id: bool = False, set_attributes: bool = False, operation_name: str = ""):
     """:cvar
     函数的span装饰器
     """
 
     def decorator(func):
         @wraps(func)
         def wrapper(*args, **kwargs):
-            operation_name = f"{func.__module__}.{func.__name__}"
-            with _tracer.start_as_current_span(operation_name) as span:
+            _operation_name = operation_name
+            if not _operation_name:
+                _operation_name = f"{func.__module__}.{func.__name__}"
+            with _tracer.start_as_current_span(_operation_name) as span:
                 try:
                     result = func(*args, **kwargs)
                     if ret_trace_id:
                         return result, hex(span.get_span_context().trace_id)
                     if set_attributes:
                         span.set_attributes({"kwargs": str(kwargs), "args": str(args)})
                     return result
```

### Comparing `yyxx_game_pkg_dev-2023.6.9.1.dev8/PKG-INFO` & `yyxx_game_pkg_dev-2023.7.5.5.dev4/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: yyxx-game-pkg-dev
-Version: 2023.6.9.1.dev8
+Version: 2023.7.5.5.dev4
 Summary: yyxx game custom module
 Home-page: https://github.com/yyxxgame/yyxxgame-pkg
 License: MIT
 Author: yyxx-game
 Requires-Python: >=3.8,<4
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -19,27 +19,31 @@
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
+Requires-Dist: opentelemetry-instrumentation-django (>=0.37b0,<0.38)
 Requires-Dist: opentelemetry-instrumentation-fastapi (==0.37b.0)
 Requires-Dist: opentelemetry-instrumentation-flask (>=0.37b0,<0.38)
 Requires-Dist: opentelemetry-instrumentation-requests (>=0.37b0,<0.38)
 Requires-Dist: opentelemetry-sdk (>=1.16.0,<2.0.0)
 Requires-Dist: pandas (>=1.5.3,<2.0.0)
 Requires-Dist: pika (>=1.3.1,<2.0.0)
 Requires-Dist: pillow (>=9.5.0,<10.0.0) ; extra == "server-center"
 Requires-Dist: pycryptodome (>=3.17,<4.0)
+Requires-Dist: pymongo (>=4.4.0,<5.0.0)
 Requires-Dist: pymysql (>=1.0.2,<2.0.0)
+Requires-Dist: pyparsing (>=3.1.0,<4.0.0)
 Requires-Dist: redis (>=4.5.1,<5.0.0)
 Requires-Dist: requests (==2.27.1)
 Requires-Dist: toml (>=0.10.2,<0.11.0)
 Requires-Dist: ujson (>=5.7.0,<6.0.0)
 Requires-Dist: uvicorn (>=0.21.0,<0.22.0)
 Project-URL: Repository, https://github.com/yyxxgame/yyxxgame-pkg
 Description-Content-Type: text/markdown
```

#### html2text {}

```diff
@@ -1,35 +1,37 @@
-Metadata-Version: 2.1 Name: yyxx-game-pkg-dev Version: 2023.6.9.1.dev8 Summary:
+Metadata-Version: 2.1 Name: yyxx-game-pkg-dev Version: 2023.7.5.5.dev4 Summary:
 yyxx game custom module Home-page: https://github.com/yyxxgame/yyxxgame-pkg
 License: MIT Author: yyxx-game Requires-Python: >=3.8,<4 Classifier: License ::
 OSI Approved :: MIT License Classifier: Operating System :: OS Independent
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
-instrumentation-flask (>=0.37b0,<0.38) Requires-Dist: opentelemetry-
-instrumentation-requests (>=0.37b0,<0.38) Requires-Dist: opentelemetry-sdk
-(>=1.16.0,<2.0.0) Requires-Dist: pandas (>=1.5.3,<2.0.0) Requires-Dist: pika
-(>=1.3.1,<2.0.0) Requires-Dist: pillow (>=9.5.0,<10.0.0) ; extra == "server-
-center" Requires-Dist: pycryptodome (>=3.17,<4.0) Requires-Dist: pymysql
-(>=1.0.2,<2.0.0) Requires-Dist: redis (>=4.5.1,<5.0.0) Requires-Dist: requests
-(==2.27.1) Requires-Dist: toml (>=0.10.2,<0.11.0) Requires-Dist: ujson
-(>=5.7.0,<6.0.0) Requires-Dist: uvicorn (>=0.21.0,<0.22.0) Project-URL:
-Repository, https://github.com/yyxxgame/yyxxgame-pkg Description-Content-Type:
-text/markdown # YYXXGAME-PKG `yyxx-game-pkg`
+(>=2.3.2,<3.0.0) ; extra == "center-api" Requires-Dist: httpx
+(>=0.24.1,<0.25.0) Requires-Dist: line-profiler (>=4.0.3,<5.0.0) Requires-Dist:
+opentelemetry-api (>=1.16.0,<2.0.0) Requires-Dist: opentelemetry-exporter-
+jaeger (>=1.16.0,<2.0.0) Requires-Dist: opentelemetry-instrumentation-celery
+(==0.37b0) Requires-Dist: opentelemetry-instrumentation-django (>=0.37b0,<0.38)
+Requires-Dist: opentelemetry-instrumentation-fastapi (==0.37b.0) Requires-Dist:
+opentelemetry-instrumentation-flask (>=0.37b0,<0.38) Requires-Dist:
+opentelemetry-instrumentation-requests (>=0.37b0,<0.38) Requires-Dist:
+opentelemetry-sdk (>=1.16.0,<2.0.0) Requires-Dist: pandas (>=1.5.3,<2.0.0)
+Requires-Dist: pika (>=1.3.1,<2.0.0) Requires-Dist: pillow (>=9.5.0,<10.0.0) ;
+extra == "server-center" Requires-Dist: pycryptodome (>=3.17,<4.0) Requires-
+Dist: pymongo (>=4.4.0,<5.0.0) Requires-Dist: pymysql (>=1.0.2,<2.0.0)
+Requires-Dist: pyparsing (>=3.1.0,<4.0.0) Requires-Dist: redis (>=4.5.1,<5.0.0)
+Requires-Dist: requests (==2.27.1) Requires-Dist: toml (>=0.10.2,<0.11.0)
+Requires-Dist: ujson (>=5.7.0,<6.0.0) Requires-Dist: uvicorn (>=0.21.0,<0.22.0)
+Project-URL: Repository, https://github.com/yyxxgame/yyxxgame-pkg Description-
+Content-Type: text/markdown # YYXXGAME-PKG `yyxx-game-pkg`
 æ¯ä¸ä¸ªä¸é¨ä¸ºåæ¸¸å¬å¸åå°å¼åç Python åé¨æ¥å£éåã  [!
 [Contributors][contributors-shield]][contributors-url] [![Forks][forks-shield]]
 [forks-url] [![Stargazers][stars-shield]][stars-url] [![Issues][issues-shield]]
 [issues-url] [![MIT License][license-shield]][license-url]
                                 [åæ¸¸ä¿¡æ¯]
                             **** åæ¸¸ä¿¡æ¯ ****
 ## ç®å½ - [ä¸ææå](#ä¸ææå) - [ç¯å¢éç½®](#ç¯å¢éç½®) -
```

