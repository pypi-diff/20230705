# Comparing `tmp/config_wrangler-0.5.4a0.tar.gz` & `tmp/config_wrangler-0.5.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "config_wrangler-0.5.4a0.tar", max compression
+gzip compressed data, was "config_wrangler-0.5.5.tar", max compression
```

## Comparing `config_wrangler-0.5.4a0.tar` & `config_wrangler-0.5.5.tar`

### file list

```diff
@@ -1,74 +1,74 @@
--rw-r--r--   0        0        0        0 2022-04-04 16:58:45.000000 config_wrangler-0.5.4a0/config_wrangler/__init__.py
--rw-r--r--   0        0        0       61 2021-10-15 15:29:20.000000 config_wrangler-0.5.4a0/config_wrangler/config_data_loaders/__init__.py
--rw-r--r--   0        0        0      302 2023-01-19 18:10:28.528146 config_wrangler-0.5.4a0/config_wrangler/config_data_loaders/__pycache__/__init__.cpython-310.pyc
--rw-r--r--   0        0        0      372 2023-01-19 18:40:29.151992 config_wrangler-0.5.4a0/config_wrangler/config_data_loaders/__pycache__/__init__.cpython-311.pyc
--rw-r--r--   0        0        0     1481 2023-01-19 18:10:28.709147 config_wrangler-0.5.4a0/config_wrangler/config_data_loaders/__pycache__/base_config_data_loader.cpython-310.pyc
--rw-r--r--   0        0        0     2279 2023-01-19 18:40:29.302749 config_wrangler-0.5.4a0/config_wrangler/config_data_loaders/__pycache__/base_config_data_loader.cpython-311.pyc
--rw-r--r--   0        0        0     2610 2023-01-19 18:10:28.537147 config_wrangler-0.5.4a0/config_wrangler/config_data_loaders/__pycache__/env_config_data_loader.cpython-310.pyc
--rw-r--r--   0        0        0     4364 2023-01-19 18:40:29.157963 config_wrangler-0.5.4a0/config_wrangler/config_data_loaders/__pycache__/env_config_data_loader.cpython-311.pyc
--rw-r--r--   0        0        0     3154 2023-01-19 18:10:28.767146 config_wrangler-0.5.4a0/config_wrangler/config_data_loaders/__pycache__/file_config_data_loader.cpython-310.pyc
--rw-r--r--   0        0        0     5475 2023-01-19 18:40:29.370771 config_wrangler-0.5.4a0/config_wrangler/config_data_loaders/__pycache__/file_config_data_loader.cpython-311.pyc
--rw-r--r--   0        0        0     5224 2023-01-19 18:10:28.758164 config_wrangler-0.5.4a0/config_wrangler/config_data_loaders/__pycache__/ini_config_data_loader.cpython-310.pyc
--rw-r--r--   0        0        0    10394 2023-01-19 18:40:29.358749 config_wrangler-0.5.4a0/config_wrangler/config_data_loaders/__pycache__/ini_config_data_loader.cpython-311.pyc
--rw-r--r--   0        0        0     1058 2022-10-04 13:22:12.000000 config_wrangler-0.5.4a0/config_wrangler/config_data_loaders/base_config_data_loader.py
--rw-r--r--   0        0        0     3546 2022-10-04 13:22:12.000000 config_wrangler-0.5.4a0/config_wrangler/config_data_loaders/env_config_data_loader.py
--rw-r--r--   0        0        0     3894 2022-10-04 13:22:12.000000 config_wrangler-0.5.4a0/config_wrangler/config_data_loaders/file_config_data_loader.py
--rw-r--r--   0        0        0     7018 2022-10-04 13:22:12.000000 config_wrangler-0.5.4a0/config_wrangler/config_data_loaders/ini_config_data_loader.py
--rw-r--r--   0        0        0     5064 2022-10-04 13:22:12.000000 config_wrangler-0.5.4a0/config_wrangler/config_data_loaders/toml_config_data_loader.py
--rw-r--r--   0        0        0       40 2021-10-15 15:29:20.000000 config_wrangler-0.5.4a0/config_wrangler/config_exception.py
--rw-r--r--   0        0        0      763 2022-10-04 13:22:12.000000 config_wrangler-0.5.4a0/config_wrangler/config_from_ini.py
--rw-r--r--   0        0        0      952 2022-10-04 13:22:12.000000 config_wrangler-0.5.4a0/config_wrangler/config_from_ini_env.py
--rw-r--r--   0        0        0     2119 2022-06-17 21:01:06.000000 config_wrangler-0.5.4a0/config_wrangler/config_from_loaders.py
--rw-r--r--   0        0        0     4324 2023-01-19 18:17:35.428775 config_wrangler-0.5.4a0/config_wrangler/config_root.py
--rw-r--r--   0        0        0        0 2022-08-11 15:33:26.000000 config_wrangler-0.5.4a0/config_wrangler/config_templates/__init__.py
--rw-r--r--   0        0        0      161 2023-01-19 18:10:28.741146 config_wrangler-0.5.4a0/config_wrangler/config_templates/__pycache__/__init__.cpython-310.pyc
--rw-r--r--   0        0        0      177 2023-01-19 18:40:29.340750 config_wrangler-0.5.4a0/config_wrangler/config_templates/__pycache__/__init__.cpython-311.pyc
--rw-r--r--   0        0        0     8028 2023-01-19 18:10:28.749146 config_wrangler-0.5.4a0/config_wrangler/config_templates/__pycache__/config_hierarchy.cpython-310.pyc
--rw-r--r--   0        0        0    11768 2023-01-19 18:40:29.347749 config_wrangler-0.5.4a0/config_wrangler/config_templates/__pycache__/config_hierarchy.cpython-311.pyc
--rw-r--r--   0        0        0     7151 2023-01-20 17:31:46.043198 config_wrangler-0.5.4a0/config_wrangler/config_templates/__pycache__/credentials.cpython-310.pyc
--rw-r--r--   0        0        0    12121 2023-01-20 17:25:24.935289 config_wrangler-0.5.4a0/config_wrangler/config_templates/__pycache__/credentials.cpython-311.pyc
--rw-r--r--   0        0        0     3685 2023-01-20 17:31:46.055202 config_wrangler-0.5.4a0/config_wrangler/config_templates/__pycache__/keepass_config.cpython-310.pyc
--rw-r--r--   0        0        0     6724 2023-01-19 22:24:32.125487 config_wrangler-0.5.4a0/config_wrangler/config_templates/__pycache__/keepass_config.cpython-311.pyc
--rw-r--r--   0        0        0     6988 2023-01-20 17:31:46.662180 config_wrangler-0.5.4a0/config_wrangler/config_templates/__pycache__/logging_config.cpython-310.pyc
--rw-r--r--   0        0        0    14658 2023-03-16 14:56:27.659745 config_wrangler-0.5.4a0/config_wrangler/config_templates/__pycache__/logging_config.cpython-311.pyc
--rw-r--r--   0        0        0      993 2023-01-20 17:31:46.506204 config_wrangler-0.5.4a0/config_wrangler/config_templates/__pycache__/password_defaults.cpython-310.pyc
--rw-r--r--   0        0        0     1336 2023-01-20 17:21:34.973531 config_wrangler-0.5.4a0/config_wrangler/config_templates/__pycache__/password_defaults.cpython-311.pyc
--rw-r--r--   0        0        0      463 2023-01-20 17:31:46.066200 config_wrangler-0.5.4a0/config_wrangler/config_templates/__pycache__/password_source.cpython-310.pyc
--rw-r--r--   0        0        0      649 2023-01-19 22:24:32.131486 config_wrangler-0.5.4a0/config_wrangler/config_templates/__pycache__/password_source.cpython-311.pyc
--rw-r--r--   0        0        0     7082 2023-01-19 18:10:29.377731 config_wrangler-0.5.4a0/config_wrangler/config_templates/__pycache__/sqlalchemy_database.cpython-310.pyc
--rw-r--r--   0        0        0    12245 2023-01-19 18:40:29.833455 config_wrangler-0.5.4a0/config_wrangler/config_templates/__pycache__/sqlalchemy_database.cpython-311.pyc
--rw-r--r--   0        0        0        0 2022-08-11 13:26:46.000000 config_wrangler-0.5.4a0/config_wrangler/config_templates/aws/__init__.py
--rw-r--r--   0        0        0      165 2023-01-19 18:12:31.247280 config_wrangler-0.5.4a0/config_wrangler/config_templates/aws/__pycache__/__init__.cpython-310.pyc
--rw-r--r--   0        0        0      181 2023-01-19 18:40:30.694299 config_wrangler-0.5.4a0/config_wrangler/config_templates/aws/__pycache__/__init__.cpython-311.pyc
--rw-r--r--   0        0        0     3596 2023-03-02 17:17:56.052265 config_wrangler-0.5.4a0/config_wrangler/config_templates/aws/__pycache__/aws_session.cpython-310.pyc
--rw-r--r--   0        0        0     5908 2023-03-15 17:13:27.230489 config_wrangler-0.5.4a0/config_wrangler/config_templates/aws/__pycache__/aws_session.cpython-311.pyc
--rw-r--r--   0        0        0    14179 2023-01-19 18:12:31.260286 config_wrangler-0.5.4a0/config_wrangler/config_templates/aws/__pycache__/s3_bucket.cpython-310.pyc
--rw-r--r--   0        0        0    24274 2023-01-19 18:40:30.705300 config_wrangler-0.5.4a0/config_wrangler/config_templates/aws/__pycache__/s3_bucket.cpython-311.pyc
--rw-r--r--   0        0        0     3568 2023-02-16 16:55:47.006011 config_wrangler-0.5.4a0/config_wrangler/config_templates/aws/aws_session.py
--rw-r--r--   0        0        0     5311 2023-02-16 17:45:03.096268 config_wrangler-0.5.4a0/config_wrangler/config_templates/aws/dynamodb.py
--rw-r--r--   0        0        0    14856 2023-05-22 18:55:50.987295 config_wrangler-0.5.4a0/config_wrangler/config_templates/aws/s3_bucket.py
--rw-r--r--   0        0        0     8553 2022-10-04 13:22:12.000000 config_wrangler-0.5.4a0/config_wrangler/config_templates/config_hierarchy.py
--rw-r--r--   0        0        0    11433 2023-01-20 17:25:24.488708 config_wrangler-0.5.4a0/config_wrangler/config_templates/credentials.py
--rw-r--r--   0        0        0     5027 2023-01-19 22:24:31.736478 config_wrangler-0.5.4a0/config_wrangler/config_templates/keepass_config.py
--rw-r--r--   0        0        0    14413 2023-05-03 21:30:39.090898 config_wrangler-0.5.4a0/config_wrangler/config_templates/logging_config.py
--rw-r--r--   0        0        0     1110 2023-01-20 17:09:25.490777 config_wrangler-0.5.4a0/config_wrangler/config_templates/password_defaults.py
--rw-r--r--   0        0        0      158 2023-01-19 22:23:52.308314 config_wrangler-0.5.4a0/config_wrangler/config_templates/password_source.py
--rw-r--r--   0        0        0    10163 2022-06-07 18:18:22.000000 config_wrangler-0.5.4a0/config_wrangler/config_templates/sqlalchemy_database.py
--rw-r--r--   0        0        0        0 2022-02-14 17:48:00.000000 config_wrangler-0.5.4a0/config_wrangler/config_types/__init__.py
--rw-r--r--   0        0        0      157 2023-01-19 18:10:28.731147 config_wrangler-0.5.4a0/config_wrangler/config_types/__pycache__/__init__.cpython-310.pyc
--rw-r--r--   0        0        0      173 2023-01-19 18:40:29.328750 config_wrangler-0.5.4a0/config_wrangler/config_types/__pycache__/__init__.cpython-311.pyc
--rw-r--r--   0        0        0     2020 2023-01-20 17:31:46.519194 config_wrangler-0.5.4a0/config_wrangler/config_types/__pycache__/dynamically_referenced.cpython-310.pyc
--rw-r--r--   0        0        0     2966 2023-01-19 22:18:20.497962 config_wrangler-0.5.4a0/config_wrangler/config_types/__pycache__/dynamically_referenced.cpython-311.pyc
--rw-r--r--   0        0        0      354 2023-01-20 17:31:46.672182 config_wrangler-0.5.4a0/config_wrangler/config_types/__pycache__/enum.cpython-310.pyc
--rw-r--r--   0        0        0      453 2023-03-16 13:23:06.383418 config_wrangler-0.5.4a0/config_wrangler/config_types/__pycache__/enum.cpython-311.pyc
--rw-r--r--   0        0        0     4217 2023-01-19 18:10:28.913147 config_wrangler-0.5.4a0/config_wrangler/config_types/__pycache__/path_types.cpython-310.pyc
--rw-r--r--   0        0        0     7374 2023-01-19 18:40:29.441803 config_wrangler-0.5.4a0/config_wrangler/config_types/__pycache__/path_types.cpython-311.pyc
--rw-r--r--   0        0        0     1600 2023-01-19 22:18:19.854961 config_wrangler-0.5.4a0/config_wrangler/config_types/dynamically_referenced.py
--rw-r--r--   0        0        0      255 2022-04-27 17:59:32.000000 config_wrangler-0.5.4a0/config_wrangler/config_types/enum.py
--rw-r--r--   0        0        0     3045 2022-06-02 20:11:39.000000 config_wrangler-0.5.4a0/config_wrangler/config_types/path_types.py
--rw-r--r--   0        0        0    17593 2023-03-02 17:43:02.517669 config_wrangler-0.5.4a0/config_wrangler/utils.py
--rw-r--r--   0        0        0     1067 2021-10-15 15:29:20.000000 config_wrangler-0.5.4a0/LICENSE
--rw-r--r--   0        0        0     1066 2021-10-15 15:29:20.000000 config_wrangler-0.5.4a0/LICENSE.txt
--rw-r--r--   0        0        0     1284 2023-05-22 19:01:32.782536 config_wrangler-0.5.4a0/pyproject.toml
--rw-r--r--   0        0        0     6157 2022-10-04 13:22:12.000000 config_wrangler-0.5.4a0/README.md
--rw-r--r--   0        0        0     7369 1970-01-01 00:00:00.000000 config_wrangler-0.5.4a0/PKG-INFO
+-rw-r--r--   0        0        0        0 2022-04-04 16:58:45.000000 config_wrangler-0.5.5/config_wrangler/__init__.py
+-rw-r--r--   0        0        0       61 2021-10-15 15:29:20.000000 config_wrangler-0.5.5/config_wrangler/config_data_loaders/__init__.py
+-rw-r--r--   0        0        0      302 2023-01-19 18:10:28.528146 config_wrangler-0.5.5/config_wrangler/config_data_loaders/__pycache__/__init__.cpython-310.pyc
+-rw-r--r--   0        0        0      372 2023-01-19 18:40:29.151992 config_wrangler-0.5.5/config_wrangler/config_data_loaders/__pycache__/__init__.cpython-311.pyc
+-rw-r--r--   0        0        0     1481 2023-01-19 18:10:28.709147 config_wrangler-0.5.5/config_wrangler/config_data_loaders/__pycache__/base_config_data_loader.cpython-310.pyc
+-rw-r--r--   0        0        0     2279 2023-01-19 18:40:29.302749 config_wrangler-0.5.5/config_wrangler/config_data_loaders/__pycache__/base_config_data_loader.cpython-311.pyc
+-rw-r--r--   0        0        0     2610 2023-01-19 18:10:28.537147 config_wrangler-0.5.5/config_wrangler/config_data_loaders/__pycache__/env_config_data_loader.cpython-310.pyc
+-rw-r--r--   0        0        0     4364 2023-01-19 18:40:29.157963 config_wrangler-0.5.5/config_wrangler/config_data_loaders/__pycache__/env_config_data_loader.cpython-311.pyc
+-rw-r--r--   0        0        0     3154 2023-01-19 18:10:28.767146 config_wrangler-0.5.5/config_wrangler/config_data_loaders/__pycache__/file_config_data_loader.cpython-310.pyc
+-rw-r--r--   0        0        0     5475 2023-01-19 18:40:29.370771 config_wrangler-0.5.5/config_wrangler/config_data_loaders/__pycache__/file_config_data_loader.cpython-311.pyc
+-rw-r--r--   0        0        0     5224 2023-01-19 18:10:28.758164 config_wrangler-0.5.5/config_wrangler/config_data_loaders/__pycache__/ini_config_data_loader.cpython-310.pyc
+-rw-r--r--   0        0        0    10394 2023-01-19 18:40:29.358749 config_wrangler-0.5.5/config_wrangler/config_data_loaders/__pycache__/ini_config_data_loader.cpython-311.pyc
+-rw-r--r--   0        0        0     1058 2022-10-04 13:22:12.000000 config_wrangler-0.5.5/config_wrangler/config_data_loaders/base_config_data_loader.py
+-rw-r--r--   0        0        0     3546 2022-10-04 13:22:12.000000 config_wrangler-0.5.5/config_wrangler/config_data_loaders/env_config_data_loader.py
+-rw-r--r--   0        0        0     3894 2022-10-04 13:22:12.000000 config_wrangler-0.5.5/config_wrangler/config_data_loaders/file_config_data_loader.py
+-rw-r--r--   0        0        0     7018 2022-10-04 13:22:12.000000 config_wrangler-0.5.5/config_wrangler/config_data_loaders/ini_config_data_loader.py
+-rw-r--r--   0        0        0     5064 2022-10-04 13:22:12.000000 config_wrangler-0.5.5/config_wrangler/config_data_loaders/toml_config_data_loader.py
+-rw-r--r--   0        0        0       40 2021-10-15 15:29:20.000000 config_wrangler-0.5.5/config_wrangler/config_exception.py
+-rw-r--r--   0        0        0      763 2022-10-04 13:22:12.000000 config_wrangler-0.5.5/config_wrangler/config_from_ini.py
+-rw-r--r--   0        0        0      952 2022-10-04 13:22:12.000000 config_wrangler-0.5.5/config_wrangler/config_from_ini_env.py
+-rw-r--r--   0        0        0     2119 2022-06-17 21:01:06.000000 config_wrangler-0.5.5/config_wrangler/config_from_loaders.py
+-rw-r--r--   0        0        0     4324 2023-01-19 18:17:35.428775 config_wrangler-0.5.5/config_wrangler/config_root.py
+-rw-r--r--   0        0        0        0 2022-08-11 15:33:26.000000 config_wrangler-0.5.5/config_wrangler/config_templates/__init__.py
+-rw-r--r--   0        0        0      161 2023-01-19 18:10:28.741146 config_wrangler-0.5.5/config_wrangler/config_templates/__pycache__/__init__.cpython-310.pyc
+-rw-r--r--   0        0        0      177 2023-01-19 18:40:29.340750 config_wrangler-0.5.5/config_wrangler/config_templates/__pycache__/__init__.cpython-311.pyc
+-rw-r--r--   0        0        0     8028 2023-01-19 18:10:28.749146 config_wrangler-0.5.5/config_wrangler/config_templates/__pycache__/config_hierarchy.cpython-310.pyc
+-rw-r--r--   0        0        0    11768 2023-01-19 18:40:29.347749 config_wrangler-0.5.5/config_wrangler/config_templates/__pycache__/config_hierarchy.cpython-311.pyc
+-rw-r--r--   0        0        0     7151 2023-01-20 17:31:46.043198 config_wrangler-0.5.5/config_wrangler/config_templates/__pycache__/credentials.cpython-310.pyc
+-rw-r--r--   0        0        0    12121 2023-01-20 17:25:24.935289 config_wrangler-0.5.5/config_wrangler/config_templates/__pycache__/credentials.cpython-311.pyc
+-rw-r--r--   0        0        0     3685 2023-01-20 17:31:46.055202 config_wrangler-0.5.5/config_wrangler/config_templates/__pycache__/keepass_config.cpython-310.pyc
+-rw-r--r--   0        0        0     6724 2023-01-19 22:24:32.125487 config_wrangler-0.5.5/config_wrangler/config_templates/__pycache__/keepass_config.cpython-311.pyc
+-rw-r--r--   0        0        0     8241 2023-07-05 14:31:35.771143 config_wrangler-0.5.5/config_wrangler/config_templates/__pycache__/logging_config.cpython-310.pyc
+-rw-r--r--   0        0        0    14658 2023-03-16 14:56:27.659745 config_wrangler-0.5.5/config_wrangler/config_templates/__pycache__/logging_config.cpython-311.pyc
+-rw-r--r--   0        0        0      993 2023-01-20 17:31:46.506204 config_wrangler-0.5.5/config_wrangler/config_templates/__pycache__/password_defaults.cpython-310.pyc
+-rw-r--r--   0        0        0     1336 2023-01-20 17:21:34.973531 config_wrangler-0.5.5/config_wrangler/config_templates/__pycache__/password_defaults.cpython-311.pyc
+-rw-r--r--   0        0        0      463 2023-01-20 17:31:46.066200 config_wrangler-0.5.5/config_wrangler/config_templates/__pycache__/password_source.cpython-310.pyc
+-rw-r--r--   0        0        0      649 2023-01-19 22:24:32.131486 config_wrangler-0.5.5/config_wrangler/config_templates/__pycache__/password_source.cpython-311.pyc
+-rw-r--r--   0        0        0     7082 2023-01-19 18:10:29.377731 config_wrangler-0.5.5/config_wrangler/config_templates/__pycache__/sqlalchemy_database.cpython-310.pyc
+-rw-r--r--   0        0        0    12245 2023-01-19 18:40:29.833455 config_wrangler-0.5.5/config_wrangler/config_templates/__pycache__/sqlalchemy_database.cpython-311.pyc
+-rw-r--r--   0        0        0        0 2022-08-11 13:26:46.000000 config_wrangler-0.5.5/config_wrangler/config_templates/aws/__init__.py
+-rw-r--r--   0        0        0      165 2023-01-19 18:12:31.247280 config_wrangler-0.5.5/config_wrangler/config_templates/aws/__pycache__/__init__.cpython-310.pyc
+-rw-r--r--   0        0        0      181 2023-01-19 18:40:30.694299 config_wrangler-0.5.5/config_wrangler/config_templates/aws/__pycache__/__init__.cpython-311.pyc
+-rw-r--r--   0        0        0     3596 2023-03-02 17:17:56.052265 config_wrangler-0.5.5/config_wrangler/config_templates/aws/__pycache__/aws_session.cpython-310.pyc
+-rw-r--r--   0        0        0     5908 2023-03-15 17:13:27.230489 config_wrangler-0.5.5/config_wrangler/config_templates/aws/__pycache__/aws_session.cpython-311.pyc
+-rw-r--r--   0        0        0    14240 2023-07-05 14:31:40.272232 config_wrangler-0.5.5/config_wrangler/config_templates/aws/__pycache__/s3_bucket.cpython-310.pyc
+-rw-r--r--   0        0        0    24274 2023-01-19 18:40:30.705300 config_wrangler-0.5.5/config_wrangler/config_templates/aws/__pycache__/s3_bucket.cpython-311.pyc
+-rw-r--r--   0        0        0     3568 2023-02-16 16:55:47.006011 config_wrangler-0.5.5/config_wrangler/config_templates/aws/aws_session.py
+-rw-r--r--   0        0        0     5311 2023-02-16 17:45:03.096268 config_wrangler-0.5.5/config_wrangler/config_templates/aws/dynamodb.py
+-rw-r--r--   0        0        0    14857 2023-05-22 19:04:06.163859 config_wrangler-0.5.5/config_wrangler/config_templates/aws/s3_bucket.py
+-rw-r--r--   0        0        0     8553 2022-10-04 13:22:12.000000 config_wrangler-0.5.5/config_wrangler/config_templates/config_hierarchy.py
+-rw-r--r--   0        0        0    11433 2023-01-20 17:25:24.488708 config_wrangler-0.5.5/config_wrangler/config_templates/credentials.py
+-rw-r--r--   0        0        0     5027 2023-01-19 22:24:31.736478 config_wrangler-0.5.5/config_wrangler/config_templates/keepass_config.py
+-rw-r--r--   0        0        0    14413 2023-05-03 21:30:39.090898 config_wrangler-0.5.5/config_wrangler/config_templates/logging_config.py
+-rw-r--r--   0        0        0     1110 2023-01-20 17:09:25.490777 config_wrangler-0.5.5/config_wrangler/config_templates/password_defaults.py
+-rw-r--r--   0        0        0      158 2023-01-19 22:23:52.308314 config_wrangler-0.5.5/config_wrangler/config_templates/password_source.py
+-rw-r--r--   0        0        0    10163 2022-06-07 18:18:22.000000 config_wrangler-0.5.5/config_wrangler/config_templates/sqlalchemy_database.py
+-rw-r--r--   0        0        0        0 2022-02-14 17:48:00.000000 config_wrangler-0.5.5/config_wrangler/config_types/__init__.py
+-rw-r--r--   0        0        0      157 2023-01-19 18:10:28.731147 config_wrangler-0.5.5/config_wrangler/config_types/__pycache__/__init__.cpython-310.pyc
+-rw-r--r--   0        0        0      173 2023-01-19 18:40:29.328750 config_wrangler-0.5.5/config_wrangler/config_types/__pycache__/__init__.cpython-311.pyc
+-rw-r--r--   0        0        0     2020 2023-01-20 17:31:46.519194 config_wrangler-0.5.5/config_wrangler/config_types/__pycache__/dynamically_referenced.cpython-310.pyc
+-rw-r--r--   0        0        0     2966 2023-01-19 22:18:20.497962 config_wrangler-0.5.5/config_wrangler/config_types/__pycache__/dynamically_referenced.cpython-311.pyc
+-rw-r--r--   0        0        0      354 2023-01-20 17:31:46.672182 config_wrangler-0.5.5/config_wrangler/config_types/__pycache__/enum.cpython-310.pyc
+-rw-r--r--   0        0        0      453 2023-03-16 13:23:06.383418 config_wrangler-0.5.5/config_wrangler/config_types/__pycache__/enum.cpython-311.pyc
+-rw-r--r--   0        0        0     4217 2023-01-19 18:10:28.913147 config_wrangler-0.5.5/config_wrangler/config_types/__pycache__/path_types.cpython-310.pyc
+-rw-r--r--   0        0        0     7374 2023-01-19 18:40:29.441803 config_wrangler-0.5.5/config_wrangler/config_types/__pycache__/path_types.cpython-311.pyc
+-rw-r--r--   0        0        0     1600 2023-01-19 22:18:19.854961 config_wrangler-0.5.5/config_wrangler/config_types/dynamically_referenced.py
+-rw-r--r--   0        0        0      255 2022-04-27 17:59:32.000000 config_wrangler-0.5.5/config_wrangler/config_types/enum.py
+-rw-r--r--   0        0        0     3045 2022-06-02 20:11:39.000000 config_wrangler-0.5.5/config_wrangler/config_types/path_types.py
+-rw-r--r--   0        0        0    17593 2023-03-02 17:43:02.517669 config_wrangler-0.5.5/config_wrangler/utils.py
+-rw-r--r--   0        0        0     1067 2021-10-15 15:29:20.000000 config_wrangler-0.5.5/LICENSE
+-rw-r--r--   0        0        0     1066 2021-10-15 15:29:20.000000 config_wrangler-0.5.5/LICENSE.txt
+-rw-r--r--   0        0        0     1284 2023-07-05 14:23:46.329449 config_wrangler-0.5.5/pyproject.toml
+-rw-r--r--   0        0        0     6157 2022-10-04 13:22:12.000000 config_wrangler-0.5.5/README.md
+-rw-r--r--   0        0        0     7376 1970-01-01 00:00:00.000000 config_wrangler-0.5.5/PKG-INFO
```

### Comparing `config_wrangler-0.5.4a0/config_wrangler/config_data_loaders/__pycache__/base_config_data_loader.cpython-310.pyc` & `config_wrangler-0.5.5/config_wrangler/config_data_loaders/__pycache__/base_config_data_loader.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `config_wrangler-0.5.4a0/config_wrangler/config_data_loaders/__pycache__/base_config_data_loader.cpython-311.pyc` & `config_wrangler-0.5.5/config_wrangler/config_data_loaders/__pycache__/base_config_data_loader.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `config_wrangler-0.5.4a0/config_wrangler/config_data_loaders/__pycache__/env_config_data_loader.cpython-310.pyc` & `config_wrangler-0.5.5/config_wrangler/config_data_loaders/__pycache__/env_config_data_loader.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `config_wrangler-0.5.4a0/config_wrangler/config_data_loaders/__pycache__/env_config_data_loader.cpython-311.pyc` & `config_wrangler-0.5.5/config_wrangler/config_data_loaders/__pycache__/env_config_data_loader.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `config_wrangler-0.5.4a0/config_wrangler/config_data_loaders/__pycache__/file_config_data_loader.cpython-310.pyc` & `config_wrangler-0.5.5/config_wrangler/config_data_loaders/__pycache__/file_config_data_loader.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `config_wrangler-0.5.4a0/config_wrangler/config_data_loaders/__pycache__/file_config_data_loader.cpython-311.pyc` & `config_wrangler-0.5.5/config_wrangler/config_data_loaders/__pycache__/file_config_data_loader.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `config_wrangler-0.5.4a0/config_wrangler/config_data_loaders/__pycache__/ini_config_data_loader.cpython-310.pyc` & `config_wrangler-0.5.5/config_wrangler/config_data_loaders/__pycache__/ini_config_data_loader.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `config_wrangler-0.5.4a0/config_wrangler/config_data_loaders/__pycache__/ini_config_data_loader.cpython-311.pyc` & `config_wrangler-0.5.5/config_wrangler/config_data_loaders/__pycache__/ini_config_data_loader.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `config_wrangler-0.5.4a0/config_wrangler/config_data_loaders/base_config_data_loader.py` & `config_wrangler-0.5.5/config_wrangler/config_data_loaders/base_config_data_loader.py`

 * *Files identical despite different names*

### Comparing `config_wrangler-0.5.4a0/config_wrangler/config_data_loaders/env_config_data_loader.py` & `config_wrangler-0.5.5/config_wrangler/config_data_loaders/env_config_data_loader.py`

 * *Files identical despite different names*

### Comparing `config_wrangler-0.5.4a0/config_wrangler/config_data_loaders/file_config_data_loader.py` & `config_wrangler-0.5.5/config_wrangler/config_data_loaders/file_config_data_loader.py`

 * *Files identical despite different names*

### Comparing `config_wrangler-0.5.4a0/config_wrangler/config_data_loaders/ini_config_data_loader.py` & `config_wrangler-0.5.5/config_wrangler/config_data_loaders/ini_config_data_loader.py`

 * *Files identical despite different names*

### Comparing `config_wrangler-0.5.4a0/config_wrangler/config_data_loaders/toml_config_data_loader.py` & `config_wrangler-0.5.5/config_wrangler/config_data_loaders/toml_config_data_loader.py`

 * *Files identical despite different names*

### Comparing `config_wrangler-0.5.4a0/config_wrangler/config_from_ini.py` & `config_wrangler-0.5.5/config_wrangler/config_from_ini.py`

 * *Files identical despite different names*

### Comparing `config_wrangler-0.5.4a0/config_wrangler/config_from_ini_env.py` & `config_wrangler-0.5.5/config_wrangler/config_from_ini_env.py`

 * *Files identical despite different names*

### Comparing `config_wrangler-0.5.4a0/config_wrangler/config_from_loaders.py` & `config_wrangler-0.5.5/config_wrangler/config_from_loaders.py`

 * *Files identical despite different names*

### Comparing `config_wrangler-0.5.4a0/config_wrangler/config_root.py` & `config_wrangler-0.5.5/config_wrangler/config_root.py`

 * *Files identical despite different names*

### Comparing `config_wrangler-0.5.4a0/config_wrangler/config_templates/__pycache__/config_hierarchy.cpython-310.pyc` & `config_wrangler-0.5.5/config_wrangler/config_templates/__pycache__/config_hierarchy.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `config_wrangler-0.5.4a0/config_wrangler/config_templates/__pycache__/config_hierarchy.cpython-311.pyc` & `config_wrangler-0.5.5/config_wrangler/config_templates/__pycache__/config_hierarchy.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `config_wrangler-0.5.4a0/config_wrangler/config_templates/__pycache__/credentials.cpython-310.pyc` & `config_wrangler-0.5.5/config_wrangler/config_templates/__pycache__/credentials.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `config_wrangler-0.5.4a0/config_wrangler/config_templates/__pycache__/credentials.cpython-311.pyc` & `config_wrangler-0.5.5/config_wrangler/config_templates/__pycache__/credentials.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `config_wrangler-0.5.4a0/config_wrangler/config_templates/__pycache__/keepass_config.cpython-310.pyc` & `config_wrangler-0.5.5/config_wrangler/config_templates/__pycache__/keepass_config.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `config_wrangler-0.5.4a0/config_wrangler/config_templates/__pycache__/keepass_config.cpython-311.pyc` & `config_wrangler-0.5.5/config_wrangler/config_templates/__pycache__/keepass_config.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `config_wrangler-0.5.4a0/config_wrangler/config_templates/__pycache__/logging_config.cpython-310.pyc` & `config_wrangler-0.5.5/config_wrangler/config_templates/__pycache__/logging_config.cpython-310.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.10, timestamp-based, .py timestamp: Tue Oct  4 13:22:12 2022 UTC, .py size: 11796 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 24% similar despite different names*

```diff
@@ -1,437 +1,516 @@
-00000000: 6f0d 0d0a 0000 0000 8433 3c63 142e 0000  o........3<c....
+00000000: 6f0d 0d0a 0000 0000 7fd2 5264 4d38 0000  o.........RdM8..
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
-00000020: 0004 0000 0040 0000 0073 b800 0000 6400  .....@...s....d.
+00000020: 0004 0000 0040 0000 0073 d000 0000 6400  .....@...s....d.
 00000030: 6401 6c00 5a00 6400 6401 6c01 5a01 6400  d.l.Z.d.d.l.Z.d.
 00000040: 6402 6c02 5400 6400 6403 6c03 6d04 5a04  d.l.T.d.d.l.m.Z.
-00000050: 0100 6400 6404 6c05 6d05 5a05 0100 6400  ..d.d.l.m.Z...d.
-00000060: 6405 6c06 6d07 5a07 0100 6400 6406 6c08  d.l.m.Z...d.d.l.
-00000070: 6d09 5a09 0100 6400 6407 6c0a 6d0b 5a0b  m.Z...d.d.l.m.Z.
-00000080: 0100 6400 6408 6c0c 6d0d 5a0d 0100 6400  ..d.d.l.m.Z...d.
-00000090: 6409 6c0e 6d0f 5a0f 0100 6400 640a 6c10  d.l.m.Z...d.d.l.
-000000a0: 6d11 5a11 6d12 5a12 0100 6400 640b 6c13  m.Z.m.Z...d.d.l.
-000000b0: 6d14 5a14 0100 6400 640c 6c15 6d16 5a16  m.Z...d.d.l.m.Z.
-000000c0: 0100 4700 640d 640e 8400 640e 6511 8303  ..G.d.d...d.e...
-000000d0: 5a17 4700 640f 6410 8400 6410 650f 8303  Z.G.d.d...d.e...
-000000e0: 5a18 6401 5300 2911 e900 0000 004e 2901  Z.d.S.)......N).
-000000f0: da01 2a29 01da 0e63 6f6e 7465 7874 6d61  ..*)...contextma
-00000100: 6e61 6765 7229 01da 0864 6174 6574 696d  nager)...datetim
-00000110: 6529 01da 1352 6f74 6174 696e 6746 696c  e)...RotatingFil
-00000120: 6548 616e 646c 6572 2901 da04 5061 7468  eHandler)...Path
-00000130: 2901 da08 4279 7465 5369 7a65 2901 da05  )...ByteSize)...
-00000140: 4469 6374 6929 01da 0f43 6f6e 6669 6748  Dicti)...ConfigH
-00000150: 6965 7261 7263 6879 2902 da07 5374 7245  ierarchy)...StrE
-00000160: 6e75 6dda 0861 7574 6f5f 7374 7229 01da  num..auto_str)..
-00000170: 1741 7574 6f43 7265 6174 6544 6972 6563  .AutoCreateDirec
-00000180: 746f 7279 5061 7468 2901 da0b 545a 466f  toryPath)...TZFo
-00000190: 726d 6174 7465 7263 0000 0000 0000 0000  rmatterc........
-000001a0: 0000 0000 0000 0000 0100 0000 4000 0000  ............@...
-000001b0: 7336 0000 0065 005a 0164 005a 0265 0383  s6...e.Z.d.Z.e..
-000001c0: 005a 0465 0383 005a 0565 0383 005a 0665  .Z.e...Z.e...Z.e
-000001d0: 0383 005a 0765 0383 005a 0865 0383 005a  ...Z.e...Z.e...Z
-000001e0: 0965 0383 005a 0a64 0153 0029 02da 084c  .e...Z.d.S.)...L
-000001f0: 6f67 4c65 7665 6c4e 290b da08 5f5f 6e61  ogLevelN)...__na
-00000200: 6d65 5f5f da0a 5f5f 6d6f 6475 6c65 5f5f  me__..__module__
-00000210: da0c 5f5f 7175 616c 6e61 6d65 5f5f 720b  ..__qualname__r.
-00000220: 0000 00da 0843 5249 5449 4341 4cda 0546  .....CRITICAL..F
-00000230: 4154 414c da05 4552 524f 52da 0757 4152  ATAL..ERROR..WAR
-00000240: 4e49 4e47 da04 494e 464f da05 4445 4255  NING..INFO..DEBU
-00000250: 47da 064e 4f54 5345 54a9 0072 1900 0000  G..NOTSET..r....
-00000260: 7219 0000 00fa 4a43 3a5c 436f 6465 5c63  r.....JC:\Code\c
-00000270: 6f6e 6669 675f 7772 616e 676c 6572 5c63  onfig_wrangler\c
-00000280: 6f6e 6669 675f 7772 616e 676c 6572 5c63  onfig_wrangler\c
-00000290: 6f6e 6669 675f 7465 6d70 6c61 7465 735c  onfig_templates\
-000002a0: 6c6f 6767 696e 675f 636f 6e66 6967 2e70  logging_config.p
-000002b0: 7972 0e00 0000 1200 0000 7310 0000 0008  yr........s.....
-000002c0: 0006 0106 0106 0106 0106 0106 010a 0172  ...............r
-000002d0: 0e00 0000 6300 0000 0000 0000 0000 0000  ....c...........
-000002e0: 0000 0000 0009 0000 0040 0000 0073 5801  .........@...sX.
-000002f0: 0000 6500 5a01 6400 5a02 5500 6503 6a04  ..e.Z.d.Z.U.e.j.
-00000300: 5a05 6503 6506 6401 3c00 6402 5a07 6508  Z.e.e.d.<.d.Z.e.
-00000310: 6506 6403 3c00 6509 6506 6404 3c00 6405  e.d.<.e.e.d.<.d.
-00000320: 5a0a 6508 6506 6406 3c00 6407 5a0b 650c  Z.e.e.d.<.d.Z.e.
-00000330: 6506 6408 3c00 6409 5a0d 6508 6506 640a  e.d.<.d.Z.e.e.d.
-00000340: 3c00 6503 6a0e 5a0f 6503 6506 640b 3c00  <.e.j.Z.e.e.d.<.
-00000350: 6402 5a10 6508 6506 640c 3c00 6511 a012  d.Z.e.e.d.<.e...
-00000360: 640d a101 a013 640e a101 5a14 6511 6506  d.....d...Z.e.e.
-00000370: 640f 3c00 6410 5a15 6516 6506 6411 3c00  d.<.d.Z.e.e.d.<.
-00000380: 6412 5a17 6508 6506 6413 3c00 6414 5a18  d.Z.e.e.d.<.d.Z.
-00000390: 650c 6506 6415 3c00 6519 6508 6503 6602  e.e.d.<.e.e.e.f.
-000003a0: 1900 6506 6416 3c00 651a 0917 6429 6418  ..e.d.<.e...d)d.
-000003b0: 6508 6419 6508 641a 6508 6606 641b 641c  e.d.e.d.e.f.d.d.
-000003c0: 8405 8301 5a1b 0905 0905 0917 642a 6418  ....Z.......d*d.
-000003d0: 6508 6408 650c 641a 6508 641d 651c 6a1d  e.d.e.d.e.d.e.j.
-000003e0: 6608 641e 641f 8405 5a1e 6420 651c 6a1d  f.d.d...Z.d e.j.
-000003f0: 6602 6421 6422 8404 5a1f 6520 0905 0914  f.d!d"..Z.e ....
-00000400: 0917 642b 6418 6508 6408 650c 641a 6508  ..d+d.e.d.e.d.e.
-00000410: 6606 6423 6424 8405 8301 5a21 6425 6426  f.d#d$....Z!d%d&
-00000420: 8400 5a22 0905 0905 0917 0905 0907 642c  ..Z"..........d,
-00000430: 6418 6508 6408 650c 641a 6508 6606 6427  d.e.d.e.d.e.f.d'
-00000440: 6428 8405 5a23 6405 5300 292d da0d 4c6f  d(..Z#d.S.)-..Lo
-00000450: 6767 696e 6743 6f6e 6669 67da 1163 6f6e  ggingConfig..con
-00000460: 736f 6c65 5f6c 6f67 5f6c 6576 656c 7a35  sole_log_levelz5
-00000470: 2528 6173 6374 696d 6529 7320 2d20 2528  %(asctime)s - %(
-00000480: 6c65 7665 6c6e 616d 6529 2d38 7320 2d20  levelname)-8s - 
-00000490: 2528 6e61 6d65 2973 3a20 2528 6d65 7373  %(name)s: %(mess
-000004a0: 6167 6529 73da 1463 6f6e 736f 6c65 5f65  age)s..console_e
-000004b0: 6e74 7279 5f66 6f72 6d61 74da 0a6c 6f67  ntry_format..log
-000004c0: 5f66 6f6c 6465 724e da0d 6c6f 675f 6669  _folderN..log_fi
-000004d0: 6c65 5f6e 616d 6554 da19 6164 645f 6461  le_nameT..add_da
-000004e0: 7465 5f74 6f5f 6c6f 675f 6669 6c65 5f6e  te_to_log_file_n
-000004f0: 616d 657a 155f 2559 5f25 6d5f 2564 5f61  amez._%Y_%m_%d_a
-00000500: 745f 2548 5f25 4d5f 2553 da1e 6c6f 675f  t_%H_%M_%S..log_
-00000510: 6669 6c65 5f6e 616d 655f 6461 7465 5f74  file_name_date_t
-00000520: 696d 655f 666f 726d 6174 da0e 6669 6c65  ime_format..file
-00000530: 5f6c 6f67 5f6c 6576 656c da15 6c6f 675f  _log_level..log_
-00000540: 6669 6c65 5f65 6e74 7279 5f66 6f72 6d61  file_entry_forma
-00000550: 747a 0531 3020 4d42 da01 62da 116c 6f67  tz.10 MB..b..log
-00000560: 5f66 696c 655f 6d61 785f 7369 7a65 e90a  _file_max_size..
-00000570: 0000 00da 116c 6f67 5f66 696c 6573 5f74  .....log_files_t
-00000580: 6f5f 6b65 6570 7a13 2559 2d25 6d2d 2564  o_keepz.%Y-%m-%d
-00000590: 2025 483a 254d 3a25 5325 7ada 136c 6f67   %H:%M:%S%z..log
-000005a0: 6769 6e67 5f64 6174 655f 666f 726d 6174  ging_date_format
-000005b0: 46da 1374 7261 6365 5f6c 6f67 6769 6e67  F..trace_logging
-000005c0: 5f73 6574 7570 da0a 6c6f 675f 6c65 7665  _setup..log_leve
-000005d0: 6c73 fa04 2e6c 6f67 da0f 6c6f 675f 6669  ls...log..log_fi
-000005e0: 6c65 5f70 7265 6669 78da 1064 6174 655f  le_prefix..date_
-000005f0: 7469 6d65 5f66 6f72 6d61 74da 0f6c 6f67  time_format..log
-00000600: 5f66 696c 655f 7375 6666 6978 6303 0000  _file_suffixc...
-00000610: 0000 0000 0000 0000 0003 0000 0004 0000  ................
-00000620: 0043 0000 0073 1a00 0000 7c00 9b00 7400  .C...s....|...t.
-00000630: a001 a100 a002 7c01 a101 9b00 7c02 9b00  ......|.....|...
-00000640: 9d03 5300 2901 61a6 0100 000a 2020 2020  ..S.).a.....    
-00000650: 2020 2020 4765 6e65 7261 7465 7320 6120      Generates a 
-00000660: 6c6f 6720 6669 6c65 206e 616d 6520 7769  log file name wi
-00000670: 7468 2061 2067 6976 656e 2070 7265 6669  th a given prefi
-00000680: 782c 2073 7566 6669 7820 616e 6420 6461  x, suffix and da
-00000690: 7465 2074 696d 6520 666f 726d 6174 2e0a  te time format..
-000006a0: 0a20 2020 2020 2020 2050 6172 616d 6574  .        Paramet
-000006b0: 6572 730a 2020 2020 2020 2020 2d2d 2d2d  ers.        ----
-000006c0: 2d2d 2d2d 2d2d 0a20 2020 2020 2020 206c  ------.        l
-000006d0: 6f67 5f66 696c 655f 7072 6566 6978 3a20  og_file_prefix: 
-000006e0: 7374 720a 2020 2020 2020 2020 2020 2020  str.            
-000006f0: 5468 6520 7061 7274 206f 6620 7468 6520  The part of the 
-00000700: 6c6f 6720 6669 6c65 206e 616d 6520 6265  log file name be
-00000710: 666f 7265 2074 6865 2064 6174 650a 2020  fore the date.  
-00000720: 2020 2020 2020 6c6f 675f 6669 6c65 5f73        log_file_s
-00000730: 7566 6669 783a 2073 7472 0a20 2020 2020  uffix: str.     
-00000740: 2020 2020 2020 2054 6865 2070 6172 7420         The part 
-00000750: 6f66 2074 6865 206c 6f67 2066 696c 6520  of the log file 
-00000760: 6e61 6d65 2061 6674 6572 2074 6865 2064  name after the d
-00000770: 6174 650a 2020 2020 2020 2020 6461 7465  ate.        date
-00000780: 5f74 696d 655f 666f 726d 6174 3a20 7374  _time_format: st
-00000790: 720a 2020 2020 2020 2020 2020 2020 4f70  r.            Op
-000007a0: 7469 6f6e 616c 2e20 5468 6520 6461 7465  tional. The date
-000007b0: 2074 696d 6520 666f 726d 6174 2074 6f20   time format to 
-000007c0: 7573 652e 2044 6566 6175 6c74 7320 746f  use. Defaults to
-000007d0: 2027 5f25 595f 256d 5f25 645f 6174 5f25   '_%Y_%m_%d_at_%
-000007e0: 485f 254d 5f25 5327 0a20 2020 2020 2020  H_%M_%S'.       
-000007f0: 2029 0372 0400 0000 da03 6e6f 77da 0873   ).r......now..s
-00000800: 7472 6674 696d 65a9 0372 2c00 0000 722d  trftime..r,...r-
-00000810: 0000 0072 2e00 0000 7219 0000 0072 1900  ...r....r....r..
-00000820: 0000 721a 0000 00da 1767 6574 5f64 6174  ..r......get_dat
-00000830: 6564 5f6c 6f67 5f66 696c 655f 6e61 6d65  ed_log_file_name
-00000840: 2b00 0000 7302 0000 001a 127a 254c 6f67  +...s......z%Log
-00000850: 6769 6e67 436f 6e66 6967 2e67 6574 5f64  gingConfig.get_d
-00000860: 6174 6564 5f6c 6f67 5f66 696c 655f 6e61  ated_log_file_na
-00000870: 6d65 da06 7265 7475 726e 6304 0000 0000  me..returnc.....
-00000880: 0000 0000 0000 000b 0000 0006 0000 0043  ...............C
-00000890: 0000 0073 3c01 0000 7400 a001 7402 a101  ...s<...t...t...
-000008a0: 7d04 7400 a001 a100 7d05 7c02 6400 7500  }.t.....}.|.d.u.
-000008b0: 7210 7c00 6a03 7d02 7c01 6400 7500 7220  r.|.j.}.|.d.u.r 
-000008c0: 7c00 6a04 6400 7501 721d 7c00 6a04 7d06  |.j.d.u.r.|.j.}.
-000008d0: 6e16 6400 7d06 6e13 7c02 722c 7405 6a06  n.d.}.n.|.r,t.j.
-000008e0: 7c01 7c00 6a07 7c03 6401 8d03 7d06 6e07  |.|.j.|.d...}.n.
-000008f0: 7c01 9b00 6402 7c03 9b00 9d03 7d06 6400  |...d.|.....}.d.
-00000900: 7d07 7c06 6400 7501 7294 7c00 6a08 6400  }.|.d.u.r.|.j.d.
-00000910: 7501 724b 7409 7c06 8301 a00a a100 734b  u.rKt.|.......sK
-00000920: 7409 7c00 6a08 7c06 8302 7d08 6e04 7409  t.|.j.|...}.n.t.
-00000930: 7c06 8301 7d08 7c00 6a0b 725a 7c04 a00c  |...}.|.j.rZ|...
-00000940: 6403 a00d 7c08 a101 a101 0100 7c08 6a0e  d...|.......|.j.
-00000950: 7d09 7c09 a00a a100 7268 7c09 6a0f 6404  }.|.....rh|.j.d.
-00000960: 6404 6405 8d02 0100 7410 7c08 7c00 6a11  d.d.....t.|.|.j.
-00000970: 7c00 6a12 6406 6407 8d04 7d07 7413 7c00  |.j.d.d...}.t.|.
-00000980: 6a14 7c00 6a15 8302 7d0a 7c07 a016 7c0a  j.|.j...}.|...|.
-00000990: a101 0100 7c07 a017 7c00 6a18 a101 0100  ....|...|.j.....
-000009a0: 7c05 a019 7c07 a101 0100 7c04 a00c 6408  |...|.....|...d.
-000009b0: a00d 7c00 6a18 a101 a101 0100 7c07 5300  ..|.j.......|.S.
-000009c0: 7c00 6a0b 729c 7c04 a00c 6409 a101 0100  |.j.r.|...d.....
-000009d0: 7c07 5300 290a 4e72 3100 0000 da01 2e7a  |.S.).Nr1......z
-000009e0: 114c 6f67 6769 6e67 2070 6174 6820 3d20  .Logging path = 
-000009f0: 7b7d 5429 02da 0770 6172 656e 7473 da08  {}T)...parents..
-00000a00: 6578 6973 745f 6f6b da04 7574 6638 2904  exist_ok..utf8).
-00000a10: da08 6669 6c65 6e61 6d65 5a08 6d61 7842  ..filenameZ.maxB
-00000a20: 7974 6573 5a0b 6261 636b 7570 436f 756e  ytesZ.backupCoun
-00000a30: 74da 0865 6e63 6f64 696e 677a 1346 696c  t..encodingz.Fil
-00000a40: 6520 6c6f 6720 6c65 7665 6c20 3d20 7b7d  e log level = {}
-00000a50: 7a2e 4e6f 206c 6f67 2066 696c 656e 616d  z.No log filenam
-00000a60: 6520 6465 6669 6e65 642e 2046 696c 6520  e defined. File 
-00000a70: 6c6f 6767 696e 6720 736b 6970 7065 642e  logging skipped.
-00000a80: 291a da07 6c6f 6767 696e 67da 0967 6574  )...logging..get
-00000a90: 4c6f 6767 6572 720f 0000 0072 2000 0000  Loggerr....r ...
-00000aa0: 721f 0000 0072 1b00 0000 7232 0000 0072  r....r....r2...r
-00000ab0: 2100 0000 721e 0000 0072 0600 0000 da0b  !...r....r......
-00000ac0: 6973 5f61 6273 6f6c 7574 6572 2900 0000  is_absoluter)...
-00000ad0: da04 696e 666f da06 666f 726d 6174 da06  ..info..format..
-00000ae0: 7061 7265 6e74 da05 6d6b 6469 7272 0500  parent..mkdirr..
-00000af0: 0000 7225 0000 0072 2700 0000 720d 0000  ..r%...r'...r...
-00000b00: 0072 2300 0000 7228 0000 00da 0c73 6574  .r#...r(.....set
-00000b10: 466f 726d 6174 7465 72da 0873 6574 4c65  Formatter..setLe
-00000b20: 7665 6c72 2200 0000 da0a 6164 6448 616e  velr".....addHan
-00000b30: 646c 6572 290b da04 7365 6c66 722c 0000  dler)...selfr,..
-00000b40: 0072 2000 0000 722e 0000 00da 036c 6f67  .r ...r......log
-00000b50: da0b 726f 6f74 5f6c 6f67 6765 7272 1f00  ..root_loggerr..
-00000b60: 0000 5a0c 6669 6c65 5f68 616e 646c 6572  ..Z.file_handler
-00000b70: 5a0d 6c6f 675f 6669 6c65 5f70 6174 685a  Z.log_file_pathZ
-00000b80: 0864 6972 5f6e 616d 655a 186c 6f67 5f66  .dir_nameZ.log_f
-00000b90: 696c 655f 656e 7472 795f 666f 726d 6174  ile_entry_format
-00000ba0: 7465 7272 1900 0000 7219 0000 0072 1a00  terr....r....r..
-00000bb0: 0000 da14 6164 645f 6c6f 675f 6669 6c65  ....add_log_file
-00000bc0: 5f68 616e 646c 6572 3f00 0000 734e 0000  _handler?...sN..
-00000bd0: 000a 0608 0108 0106 0108 010a 0108 0106  ................
-00000be0: 0204 0204 0102 0104 0102 0108 fd0e 0604  ................
-00000bf0: 0208 0116 010e 0108 0206 0210 0106 0508  ................
-00000c00: 010e 0104 0204 0104 0102 0106 fd0e 050a  ................
-00000c10: 010c 010a 0112 0104 0406 fe0a 0104 017a  ...............z
-00000c20: 224c 6f67 6769 6e67 436f 6e66 6967 2e61  "LoggingConfig.a
-00000c30: 6464 5f6c 6f67 5f66 696c 655f 6861 6e64  dd_log_file_hand
-00000c40: 6c65 72da 0768 616e 646c 6572 6302 0000  ler..handlerc...
-00000c50: 0000 0000 0000 0000 0004 0000 0004 0000  ................
-00000c60: 0043 0000 0073 5e00 0000 7400 a001 7402  .C...s^...t...t.
-00000c70: a101 7d02 7c01 6400 7501 7223 7c00 6a03  ..}.|.d.u.r#|.j.
-00000c80: 7214 7c02 a004 6401 7c01 9b00 9d02 a101  r.|...d.|.......
-00000c90: 0100 7400 a001 a100 7d03 7c03 a005 7c01  ..t.....}.|...|.
-00000ca0: a101 0100 7c01 a006 a100 0100 6400 5300  ....|.......d.S.
-00000cb0: 7c00 6a03 722d 7c02 a004 6402 a101 0100  |.j.r-|...d.....
-00000cc0: 6400 5300 6400 5300 2903 4e7a 1443 6c6f  d.S.d.S.).Nz.Clo
-00000cd0: 7369 6e67 206c 6f67 2068 616e 646c 6572  sing log handler
-00000ce0: 207a 294e 6f20 6861 6e64 6c65 7220 7072   z)No handler pr
-00000cf0: 6f76 6964 6564 2074 6f20 7265 6d6f 7665  ovided to remove
-00000d00: 5f6c 6f67 5f68 616e 646c 6572 2907 723a  _log_handler).r:
-00000d10: 0000 0072 3b00 0000 720f 0000 0072 2900  ...r;...r....r).
-00000d20: 0000 723d 0000 00da 0d72 656d 6f76 6548  ..r=.....removeH
-00000d30: 616e 646c 6572 da05 636c 6f73 6529 0472  andler..close).r
-00000d40: 4400 0000 7248 0000 0072 4500 0000 7246  D...rH...rE...rF
-00000d50: 0000 0072 1900 0000 7219 0000 0072 1a00  ...r....r....r..
-00000d60: 0000 da12 7265 6d6f 7665 5f6c 6f67 5f68  ....remove_log_h
-00000d70: 616e 646c 6572 7800 0000 7314 0000 000a  andlerx...s.....
-00000d80: 0108 0106 0110 0108 010a 010c 0106 020e  ................
-00000d90: 0104 ff7a 204c 6f67 6769 6e67 436f 6e66  ...z LoggingConf
-00000da0: 6967 2e72 656d 6f76 655f 6c6f 675f 6861  ig.remove_log_ha
-00000db0: 6e64 6c65 7263 0400 0000 0000 0000 0000  ndlerc..........
-00000dc0: 0000 0500 0000 0900 0000 6300 0000 7336  ..........c...s6
-00000dd0: 0000 0081 007c 006a 007c 017c 027c 0364  .....|.j.|.|.|.d
-00000de0: 018d 037d 047a 0b7c 0456 0001 0057 007c  ...}.z.|.V...W.|
-00000df0: 00a0 017c 04a1 0101 0064 0053 007c 00a0  ...|.....d.S.|..
-00000e00: 017c 04a1 0101 0077 0029 024e a903 722c  .|.....w.).N..r,
-00000e10: 0000 0072 2000 0000 722e 0000 0029 0272  ...r ...r....).r
-00000e20: 4700 0000 724b 0000 0029 0572 4400 0000  G...rK...).rD...
-00000e30: 722c 0000 0072 2000 0000 722e 0000 005a  r,...r ...r....Z
-00000e40: 106c 6f67 5f66 696c 655f 6861 6e64 6c65  .log_file_handle
-00000e50: 7272 1900 0000 7219 0000 0072 1a00 0000  rr....r....r....
-00000e60: da10 6c6f 675f 6669 6c65 5f6d 616e 6167  ..log_file_manag
-00000e70: 6572 8400 0000 7312 0000 0002 8004 0702  er....s.........
-00000e80: 0102 0102 0106 fd02 0508 011a 037a 1e4c  .............z.L
-00000e90: 6f67 6769 6e67 436f 6e66 6967 2e6c 6f67  oggingConfig.log
-00000ea0: 5f66 696c 655f 6d61 6e61 6765 7263 0100  _file_managerc..
-00000eb0: 0000 0000 0000 0000 0000 0a00 0000 0b00  ................
-00000ec0: 0000 4300 0000 739c 0100 0074 0083 007d  ..C...s....t...}
-00000ed0: 0174 01a0 02a1 007d 0274 0374 016a 046a  .t.....}.t.t.j.j
-00000ee0: 056a 0683 017d 037c 0374 016a 046a 055f  .j...}.|.t.j.j._
-00000ef0: 067c 006a 07a0 08a1 0044 005d 375c 027d  .|.j.....D.]7\.}
-00000f00: 047d 057c 04a0 09a1 0064 016b 0272 257c  .}.|.....d.k.r%|
-00000f10: 027d 066e 0574 01a0 027c 04a1 017d 067c  .}.n.t...|...}.|
-00000f20: 067c 017c 043c 0064 027c 065f 0a7c 0564  .|.|.<.d.|._.|.d
-00000f30: 0075 0072 3864 037d 056e 047c 05a0 0ba1  .u.r8d.}.n.|....
-00000f40: 007d 057c 006a 0c72 4a74 0d64 047c 066a  .}.|.j.rJt.d.|.j
-00000f50: 0e9b 0064 057c 059b 009d 0483 0101 007c  ...d.|.........|
-00000f60: 06a0 0f7c 05a1 0101 0071 1874 1074 016a  ...|.....q.t.t.j
-00000f70: 046a 056a 0683 0144 005d 5b7d 0474 01a0  .j.j...D.][}.t..
-00000f80: 027c 04a1 017d 067c 006a 0c72 6c74 0d64  .|...}.|.j.rlt.d
-00000f90: 067c 049b 0064 077c 066a 119b 009d 0483  .|...d.|.j......
-00000fa0: 0101 007c 047c 0176 0172 b27c 006a 0c72  ...|.|.v.r.|.j.r
-00000fb0: 8274 0d64 087c 049b 0064 0974 01a0 127c  .t.d.|...d.t...|
-00000fc0: 06a0 13a1 00a1 019b 009d 0483 0101 0074  ...............t
-00000fd0: 107c 0183 0144 005d 2b7d 077c 04a0 147c  .|...D.]+}.|...|
-00000fe0: 07a1 0172 b17c 017c 0719 007d 087c 08a0  ...r.|.|...}.|..
-00000ff0: 13a1 007d 097c 06a0 0f7c 09a1 0101 007c  ...}.|...|.....|
-00001000: 006a 0c72 ae74 0d64 0a7c 049b 0064 0b7c  .j.r.t.d.|...d.|
-00001010: 086a 0e9b 0064 0c74 01a0 127c 09a1 019b  .j...d.t...|....
-00001020: 009d 0683 0101 0064 027c 065f 0a71 8671  .......d.|._.q.q
-00001030: 577c 006a 0c72 cc74 0d64 0d74 01a0 127c  W|.j.r.t.d.t...|
-00001040: 02a0 13a1 00a1 019b 009d 0283 0101 0074  ...............t
-00001050: 0d64 0e7c 026a 119b 009d 0283 0101 0064  .d.|.j.........d
-00001060: 0053 0064 0053 0029 0f4e da04 726f 6f74  .S.d.S.).N..root
-00001070: 5472 1600 0000 7a0f 5365 7474 696e 6720  Tr....z.Setting 
-00001080: 6c6f 6767 6572 207a 0420 746f 207a 074c  logger z. to z.L
-00001090: 6f67 6765 7220 7a0a 2068 616e 646c 6572  ogger z. handler
-000010a0: 7320 7a19 4368 6563 6b69 6e67 2065 7869  s z.Checking exi
-000010b0: 7374 696e 6720 6c6f 6767 6572 207a 0720  sting logger z. 
-000010c0: 6c65 7665 6c20 7a10 4578 6973 7469 6e67  level z.Existing
-000010d0: 206c 6f67 6765 7220 7a0f 2072 652d 7365   logger z. re-se
-000010e0: 7475 7020 7769 7468 207a 0a20 7365 7474  tup with z. sett
-000010f0: 696e 6773 207a 1652 6f6f 7420 6c6f 6767  ings z.Root logg
-00001100: 696e 6720 6c65 7665 6c20 6973 207a 1a52  ing level is z.R
-00001110: 6f6f 7420 6c6f 6767 696e 6720 6861 6e64  oot logging hand
-00001120: 6c65 7273 2061 7265 2029 15da 0464 6963  lers are )...dic
-00001130: 7472 3a00 0000 723b 0000 0072 0800 0000  tr:...r;...r....
-00001140: da06 4c6f 6767 6572 da07 6d61 6e61 6765  ..Logger..manage
-00001150: 72da 0a6c 6f67 6765 7244 6963 7472 2a00  r..loggerDictr*.
-00001160: 0000 da05 6974 656d 73da 056c 6f77 6572  ....items..lower
-00001170: da09 7072 6f70 6167 6174 65da 0575 7070  ..propagate..upp
-00001180: 6572 7229 0000 00da 0570 7269 6e74 da04  err).....print..
-00001190: 6e61 6d65 7242 0000 00da 0673 6f72 7465  namerB.....sorte
-000011a0: 64da 0868 616e 646c 6572 73da 0c67 6574  d..handlers..get
-000011b0: 4c65 7665 6c4e 616d 65da 1167 6574 4566  LevelName..getEf
-000011c0: 6665 6374 6976 654c 6576 656c da0a 7374  fectiveLevel..st
-000011d0: 6172 7473 7769 7468 290a 7244 0000 005a  artswith).rD...Z
-000011e0: 1263 6f6e 6669 6775 7265 645f 6c6f 6767  .configured_logg
-000011f0: 6572 7372 4600 0000 5a0b 6c6f 6767 6572  ersrF...Z.logger
-00001200: 5f64 6963 745a 0c6c 6f67 6765 725f 636c  _dictZ.logger_cl
-00001210: 6173 735a 1264 6573 6972 6564 5f6c 6576  assZ.desired_lev
-00001220: 656c 5f6e 616d 65da 066c 6f67 6765 725a  el_name..loggerZ
-00001230: 0e63 6f6d 7061 7265 5f6c 6f67 6765 725a  .compare_loggerZ
-00001240: 0d70 6172 656e 745f 6c6f 6767 6572 da05  .parent_logger..
-00001250: 6c65 7665 6c72 1900 0000 7219 0000 0072  levelr....r....r
-00001260: 1a00 0000 da10 7365 7475 705f 6c6f 675f  ......setup_log_
-00001270: 6c65 7665 6c73 9600 0000 7358 0000 0006  levels....sX....
-00001280: 0108 010e 030a 0112 020c 0106 010a 0208  ................
-00001290: 0106 0108 0106 0108 0206 0116 020c 0112  ................
-000012a0: 030a 0106 0116 0108 0106 0102 0208 010c  ................
-000012b0: 0104 ff04 ff0c 040a 0108 0108 010a 0106  ................
-000012c0: 0102 0210 0108 0104 ff04 ff06 0404 8006  ................
-000012d0: 0218 0214 0104 fd7a 1e4c 6f67 6769 6e67  .......z.Logging
-000012e0: 436f 6e66 6967 2e73 6574 7570 5f6c 6f67  Config.setup_log
-000012f0: 5f6c 6576 656c 7363 0600 0000 0000 0000  _levelsc........
-00001300: 0000 0000 1100 0000 0500 0000 4300 0000  ............C...
-00001310: 7376 0100 0074 00a0 01a1 007d 0674 027c  sv...t.....}.t.|
-00001320: 0664 0183 0273 b964 027c 065f 037c 066a  .d...s.d.|._.|.j
-00001330: 0444 005d 0a7d 077c 07a0 05a1 0001 007c  .D.].}.|.......|
-00001340: 07a0 06a1 0001 0071 0f7c 066a 04a0 07a1  .......q.|.j....
-00001350: 0001 007c 006a 0872 2e74 0964 0383 0101  ...|.j.r.t.d....
-00001360: 0074 0964 047c 066a 049b 009d 0283 0101  .t.d.|.j........
-00001370: 007c 06a0 0a74 006a 0ba1 0101 007c 0464  .|...t.j.....|.d
-00001380: 0575 0072 3f74 0c6a 0d7d 0874 0c6a 0e7d  .u.r?t.j.}.t.j.}
-00001390: 096e 047c 047d 087c 047d 0974 00a0 0f7c  .n.|.}.|.}.t...|
-000013a0: 08a1 017d 0a7c 0aa0 0a74 006a 10a1 0101  ...}.|...t.j....
-000013b0: 007c 06a0 117c 0aa1 0101 0074 00a0 0f7c  .|...|.....t...|
-000013c0: 09a1 017d 0b7c 0ba0 0a7c 006a 12a1 0101  ...}.|...|.j....
-000013d0: 0064 0664 0784 007d 0c7c 0ba0 137c 0ca1  .d.d...}.|...|..
-000013e0: 0101 007c 06a0 117c 0ba1 0101 007c 006a  ...|...|.....|.j
-000013f0: 147d 0d7c 0d72 8174 157c 0d7c 006a 1683  .}.|.r.t.|.|.j..
-00001400: 027d 0e7c 0ba0 177c 0ea1 0101 007c 0aa0  .}.|...|.....|..
-00001410: 177c 0ea1 0101 007c 00a0 18a1 0001 0074  .|.....|.......t
-00001420: 00a0 0174 19a1 017d 0f74 00a0 1a64 02a1  ...t...}.t...d..
-00001430: 0101 0074 00a0 1b7c 0fa0 1ca1 00a1 017d  ...t...|.......}
-00001440: 107c 006a 0872 a17c 0fa0 1d64 08a0 1e7c  .|.j.r.|...d...|
-00001450: 10a1 01a1 0101 007c 0573 a77c 0164 0575  .......|.s.|.d.u
-00001460: 0172 af7c 006a 1f7c 017c 027c 0364 098d  .r.|.j.|.|.|.d..
-00001470: 0353 007c 006a 0872 b77c 0fa0 1d64 0aa1  .S.|.j.r.|...d..
-00001480: 0101 0064 0553 0064 0553 0029 0b7a 370a  ...d.S.d.S.).z7.
-00001490: 2020 2020 2020 2020 5365 7475 7020 6c6f          Setup lo
-000014a0: 6767 696e 6720 6261 7365 6420 6f6e 2063  gging based on c
-000014b0: 6f6e 6669 6775 7261 7469 6f6e 2e0a 2020  onfiguration..  
-000014c0: 2020 2020 2020 da1a 636f 6e66 6967 5f77        ..config_w
-000014d0: 7261 6e67 6c65 725f 7365 7475 705f 646f  rangler_setup_do
-000014e0: 6e65 547a 1c6c 6f67 6769 6e67 2e74 7261  neTz.logging.tra
-000014f0: 6365 5f73 6574 7570 2069 7320 5472 7565  ce_setup is True
-00001500: 7d7a 1e53 7461 7274 696e 6720 726f 6f74  }z.Starting root
-00001510: 206c 6f67 6765 7220 6861 6e64 6c65 7273   logger handlers
-00001520: 204e 6301 0000 0000 0000 0000 0000 0001   Nc.............
-00001530: 0000 0002 0000 0053 0000 0073 0c00 0000  .......S...s....
-00001540: 7c00 6a00 7401 6a02 6b03 5300 2901 4e29  |.j.t.j.k.S.).N)
-00001550: 03da 076c 6576 656c 6e6f 723a 0000 0072  ...levelnor:...r
-00001560: 1400 0000 2901 da06 7265 636f 7264 7219  ....)...recordr.
-00001570: 0000 0072 1900 0000 721a 0000 00da 096e  ...r....r......n
-00001580: 6f6e 5f65 7272 6f72 ff00 0000 7302 0000  on_error....s...
-00001590: 000c 017a 2e4c 6f67 6769 6e67 436f 6e66  ...z.LoggingConf
-000015a0: 6967 2e73 6574 7570 5f6c 6f67 6769 6e67  ig.setup_logging
-000015b0: 2e3c 6c6f 6361 6c73 3e2e 6e6f 6e5f 6572  .<locals>.non_er
-000015c0: 726f 727a 2054 6869 7320 6d6f 6475 6c65  rorz This module
-000015d0: 7320 6c6f 6767 696e 6720 6c65 7665 6c20  s logging level 
-000015e0: 6973 207b 7d72 4c00 0000 7a38 7573 655f  is {}rL...z8use_
-000015f0: 6c6f 675f 6669 6c65 5f73 6574 7469 6e67  log_file_setting
-00001600: 203d 2046 616c 7365 2e20 7365 7475 705f   = False. setup_
-00001610: 6c6f 675f 6669 6c65 206e 6f74 2063 616c  log_file not cal
-00001620: 6c65 642e 2920 723a 0000 0072 3b00 0000  led.) r:...r;...
-00001630: da07 6861 7361 7474 7272 6100 0000 725a  ..hasattrra...rZ
-00001640: 0000 00da 0566 6c75 7368 724a 0000 00da  .....flushrJ....
-00001650: 0563 6c65 6172 7229 0000 0072 5700 0000  .clearr)...rW...
-00001660: 7242 0000 0072 1600 0000 da03 7379 73da  rB...r......sys.
-00001670: 0673 7464 6572 72da 0673 7464 6f75 74da  .stderr..stdout.
-00001680: 0d53 7472 6561 6d48 616e 646c 6572 7214  .StreamHandlerr.
-00001690: 0000 0072 4300 0000 721c 0000 00da 0961  ...rC...r......a
-000016a0: 6464 4669 6c74 6572 721d 0000 0072 0d00  ddFilterr....r..
-000016b0: 0000 7228 0000 0072 4100 0000 7260 0000  ..r(...rA...r`..
-000016c0: 0072 0f00 0000 da0f 6361 7074 7572 6557  .r......captureW
-000016d0: 6172 6e69 6e67 7372 5b00 0000 725c 0000  arningsr[...r\..
-000016e0: 0072 3d00 0000 723e 0000 0072 4700 0000  .r=...r>...rG...
-000016f0: 2911 7244 0000 0072 2c00 0000 7220 0000  ).rD...r,...r ..
-00001700: 0072 2e00 0000 5a0e 636f 6e73 6f6c 655f  .r....Z.console_
-00001710: 6f75 7470 7574 5a14 7573 655f 6c6f 675f  outputZ.use_log_
-00001720: 6669 6c65 5f73 6574 7469 6e67 7246 0000  file_settingrF..
-00001730: 0072 4800 0000 5a0c 6572 726f 725f 6f75  .rH...Z.error_ou
-00001740: 7470 7574 5a0e 7265 6775 6c61 725f 6f75  tputZ.regular_ou
-00001750: 7470 7574 5a11 636f 6e73 6f6c 655f 6572  tputZ.console_er
-00001760: 726f 725f 6c6f 675a 0b63 6f6e 736f 6c65  ror_logZ.console
-00001770: 5f6c 6f67 7264 0000 0072 1d00 0000 5a17  _logrd...r....Z.
-00001780: 636f 6e73 6f6c 655f 656e 7472 795f 666f  console_entry_fo
-00001790: 726d 6174 7465 7272 4500 0000 5a0e 6c6f  rmatterrE...Z.lo
-000017a0: 675f 6c65 7665 6c5f 6e61 6d65 7219 0000  g_level_namer...
-000017b0: 0072 1900 0000 721a 0000 00da 0d73 6574  .r....r......set
-000017c0: 7570 5f6c 6f67 6769 6e67 cc00 0000 735a  up_logging....sZ
-000017d0: 0000 0008 0c0a 0206 040a 0308 010a 010a  ................
-000017e0: 0306 0208 0210 010c 0308 0206 0108 0104  ................
-000017f0: 0204 010a 020c 010a 010a 020c 0108 030a  ................
-00001800: 040a 0206 0204 010c 010a 010a 0108 020a  ................
-00001810: 030a 020e 0206 0110 010c 0204 0102 0102  ................
-00001820: 0102 0106 fd06 060a 0104 0104 b97a 1b4c  .............z.L
-00001830: 6f67 6769 6e67 436f 6e66 6967 2e73 6574  oggingConfig.set
-00001840: 7570 5f6c 6f67 6769 6e67 2901 722b 0000  up_logging).r+..
-00001850: 0029 034e 4e72 2b00 0000 2903 4e46 722b  .).NNr+...).NFr+
-00001860: 0000 0029 054e 4e72 2b00 0000 4e54 2924  ...).NNr+...NT)$
-00001870: 720f 0000 0072 1000 0000 7211 0000 0072  r....r....r....r
-00001880: 0e00 0000 7216 0000 0072 1c00 0000 da0f  ....r....r......
-00001890: 5f5f 616e 6e6f 7461 7469 6f6e 735f 5f72  __annotations__r
-000018a0: 1d00 0000 da03 7374 7272 0c00 0000 721f  ......strr....r.
-000018b0: 0000 0072 2000 0000 da04 626f 6f6c 7221  ...r .....boolr!
-000018c0: 0000 0072 1700 0000 7222 0000 0072 2300  ...r....r"...r#.
-000018d0: 0000 7207 0000 00da 0876 616c 6964 6174  ..r......validat
-000018e0: 65da 0274 6f72 2500 0000 7227 0000 00da  e..tor%...r'....
-000018f0: 0369 6e74 7228 0000 0072 2900 0000 da04  .intr(...r).....
-00001900: 4469 6374 da0c 7374 6174 6963 6d65 7468  Dict..staticmeth
-00001910: 6f64 7232 0000 0072 3a00 0000 da07 4861  odr2...r:.....Ha
-00001920: 6e64 6c65 7272 4700 0000 724b 0000 0072  ndlerrG...rK...r
-00001930: 0300 0000 724d 0000 0072 6000 0000 726e  ....rM...r`...rn
-00001940: 0000 0072 1900 0000 7219 0000 0072 1900  ...r....r....r..
-00001950: 0000 721a 0000 0072 1b00 0000 1c00 0000  ..r....r........
-00001960: 7378 0000 000a 000e 010c 0108 010c 010c  sx..............
-00001970: 010c 010e 010c 0118 010c 010c 010c 0110  ................
-00001980: 0102 0202 0404 fd02 0102 ff02 0202 fe02  ................
-00001990: 030c fd02 1502 0102 0104 fc02 0202 fe02  ................
-000019a0: 0302 fd02 0402 fc04 050a fb10 3902 0c02  ............9...
-000019b0: 0302 0102 0104 fc02 0202 fe02 0302 fd02  ................
-000019c0: 040c fc08 1102 3802 0102 0102 0102 0104  ......8.........
-000019d0: fa02 0202 fe02 0302 fd02 040e fc72 1b00  .............r..
-000019e0: 0000 2919 723a 0000 0072 6800 0000 da06  ..).r:...rh.....
-000019f0: 7479 7069 6e67 da0a 636f 6e74 6578 746c  typing..contextl
-00001a00: 6962 7203 0000 0072 0400 0000 5a10 6c6f  ibr....r....Z.lo
-00001a10: 6767 696e 672e 6861 6e64 6c65 7273 7205  gging.handlersr.
-00001a20: 0000 00da 0770 6174 686c 6962 7206 0000  .....pathlibr...
-00001a30: 00da 0870 7964 616e 7469 6372 0700 0000  ...pydanticr....
-00001a40: da07 7079 6469 6374 6972 0800 0000 da31  ..pydictir.....1
-00001a50: 636f 6e66 6967 5f77 7261 6e67 6c65 722e  config_wrangler.
-00001a60: 636f 6e66 6967 5f74 656d 706c 6174 6573  config_templates
-00001a70: 2e63 6f6e 6669 675f 6869 6572 6172 6368  .config_hierarch
-00001a80: 7972 0900 0000 5a21 636f 6e66 6967 5f77  yr....Z!config_w
-00001a90: 7261 6e67 6c65 722e 636f 6e66 6967 5f74  rangler.config_t
-00001aa0: 7970 6573 2e65 6e75 6d72 0a00 0000 720b  ypes.enumr....r.
-00001ab0: 0000 00da 2763 6f6e 6669 675f 7772 616e  ....'config_wran
-00001ac0: 676c 6572 2e63 6f6e 6669 675f 7479 7065  gler.config_type
-00001ad0: 732e 7061 7468 5f74 7970 6573 720c 0000  s.path_typesr...
-00001ae0: 00da 1563 6f6e 6669 675f 7772 616e 676c  ...config_wrangl
-00001af0: 6572 2e75 7469 6c73 720d 0000 0072 0e00  er.utilsr....r..
-00001b00: 0000 721b 0000 0072 1900 0000 7219 0000  ..r....r....r...
-00001b10: 0072 1900 0000 721a 0000 00da 083c 6d6f  .r....r......<mo
-00001b20: 6475 6c65 3e01 0000 0073 1e00 0000 0800  dule>....s......
-00001b30: 0801 0801 0c01 0c01 0c01 0c01 0c02 0c01  ................
-00001b40: 0c02 1001 0c01 0c01 1003 140a            ............
+00000050: 0100 6400 6404 6c05 6d05 5a05 6d06 5a06  ..d.d.l.m.Z.m.Z.
+00000060: 0100 6400 6405 6c07 6d08 5a08 6d09 5a09  ..d.d.l.m.Z.m.Z.
+00000070: 0100 6400 6406 6c0a 6d0b 5a0b 0100 6400  ..d.d.l.m.Z...d.
+00000080: 6407 6c0c 6d0d 5a0d 0100 6400 6408 6c0e  d.l.m.Z...d.d.l.
+00000090: 6d0f 5a0f 0100 6400 6409 6c10 6d11 5a11  m.Z...d.d.l.m.Z.
+000000a0: 0100 6400 640a 6c12 6d13 5a13 6d14 5a14  ..d.d.l.m.Z.m.Z.
+000000b0: 0100 6400 640b 6c15 6d16 5a16 0100 6400  ..d.d.l.m.Z...d.
+000000c0: 640c 6c17 6d18 5a18 0100 4700 640d 640e  d.l.m.Z...G.d.d.
+000000d0: 8400 640e 6513 8303 5a19 4700 640f 6410  ..d.e...Z.G.d.d.
+000000e0: 8400 6410 6513 8303 5a1a 4700 6411 6412  ..d.e...Z.G.d.d.
+000000f0: 8400 6412 6511 8303 5a1b 6401 5300 2913  ..d.e...Z.d.S.).
+00000100: e900 0000 004e 2901 da01 2a29 01da 0e63  .....N)...*)...c
+00000110: 6f6e 7465 7874 6d61 6e61 6765 7229 02da  ontextmanager)..
+00000120: 0864 6174 6574 696d 65da 0474 696d 6529  .datetime..time)
+00000130: 02da 1352 6f74 6174 696e 6746 696c 6548  ...RotatingFileH
+00000140: 616e 646c 6572 da18 5469 6d65 6452 6f74  andler..TimedRot
+00000150: 6174 696e 6746 696c 6548 616e 646c 6572  atingFileHandler
+00000160: 2901 da04 5061 7468 2901 da08 4279 7465  )...Path)...Byte
+00000170: 5369 7a65 2901 da05 4469 6374 6929 01da  Size)...Dicti)..
+00000180: 0f43 6f6e 6669 6748 6965 7261 7263 6879  .ConfigHierarchy
+00000190: 2902 da07 5374 7245 6e75 6dda 0861 7574  )...StrEnum..aut
+000001a0: 6f5f 7374 7229 01da 1741 7574 6f43 7265  o_str)...AutoCre
+000001b0: 6174 6544 6972 6563 746f 7279 5061 7468  ateDirectoryPath
+000001c0: 2901 da0b 545a 466f 726d 6174 7465 7263  )...TZFormatterc
+000001d0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+000001e0: 0100 0000 4000 0000 7336 0000 0065 005a  ....@...s6...e.Z
+000001f0: 0164 005a 0265 0383 005a 0465 0383 005a  .d.Z.e...Z.e...Z
+00000200: 0565 0383 005a 0665 0383 005a 0765 0383  .e...Z.e...Z.e..
+00000210: 005a 0865 0383 005a 0965 0383 005a 0a64  .Z.e...Z.e...Z.d
+00000220: 0153 0029 02da 084c 6f67 4c65 7665 6c4e  .S.)...LogLevelN
+00000230: 290b da08 5f5f 6e61 6d65 5f5f da0a 5f5f  )...__name__..__
+00000240: 6d6f 6475 6c65 5f5f da0c 5f5f 7175 616c  module__..__qual
+00000250: 6e61 6d65 5f5f 720d 0000 00da 0843 5249  name__r......CRI
+00000260: 5449 4341 4cda 0546 4154 414c da05 4552  TICAL..FATAL..ER
+00000270: 524f 52da 0757 4152 4e49 4e47 da04 494e  ROR..WARNING..IN
+00000280: 464f da05 4445 4255 47da 064e 4f54 5345  FO..DEBUG..NOTSE
+00000290: 54a9 0072 1b00 0000 721b 0000 00fa 4a43  T..r....r.....JC
+000002a0: 3a5c 436f 6465 5c63 6f6e 6669 675f 7772  :\Code\config_wr
+000002b0: 616e 676c 6572 5c63 6f6e 6669 675f 7772  angler\config_wr
+000002c0: 616e 676c 6572 5c63 6f6e 6669 675f 7465  angler\config_te
+000002d0: 6d70 6c61 7465 735c 6c6f 6767 696e 675f  mplates\logging_
+000002e0: 636f 6e66 6967 2e70 7972 1000 0000 1200  config.pyr......
+000002f0: 0000 7310 0000 0008 0006 0106 0106 0106  ..s.............
+00000300: 0106 0106 010a 0172 1000 0000 6300 0000  .......r....c...
+00000310: 0000 0000 0000 0000 0000 0000 0001 0000  ................
+00000320: 0040 0000 0073 1800 0000 6500 5a01 6400  .@...s....e.Z.d.
+00000330: 5a02 6503 8300 5a04 6503 8300 5a05 6401  Z.e...Z.e...Z.d.
+00000340: 5300 2902 da10 4669 6c65 4861 6e64 6c65  S.)...FileHandle
+00000350: 7243 6c61 7373 4e29 0672 1100 0000 7212  rClassN).r....r.
+00000360: 0000 0072 1300 0000 720d 0000 0072 0600  ...r....r....r..
+00000370: 0000 7207 0000 0072 1b00 0000 721b 0000  ..r....r....r...
+00000380: 0072 1b00 0000 721c 0000 0072 1d00 0000  .r....r....r....
+00000390: 1c00 0000 7306 0000 0008 0006 020a 0372  ....s..........r
+000003a0: 1d00 0000 6300 0000 0000 0000 0000 0000  ....c...........
+000003b0: 0000 0000 0009 0000 0040 0000 0073 a401  .........@...s..
+000003c0: 0000 6500 5a01 6400 5a02 5500 6503 6a04  ..e.Z.d.Z.U.e.j.
+000003d0: 5a05 6503 6506 6401 3c00 6402 5a07 6508  Z.e.e.d.<.d.Z.e.
+000003e0: 6506 6403 3c00 6404 5a09 650a 6506 6405  e.d.<.d.Z.e.e.d.
+000003f0: 3c00 6404 5a0b 6508 6506 6406 3c00 6404  <.d.Z.e.e.d.<.d.
+00000400: 5a0c 650d 6506 6407 3c00 6408 5a0e 6508  Z.e.e.d.<.d.Z.e.
+00000410: 6506 6409 3c00 6503 6a0f 5a10 6503 6506  e.d.<.e.j.Z.e.e.
+00000420: 640a 3c00 6402 5a11 6508 6506 640b 3c00  d.<.d.Z.e.e.d.<.
+00000430: 6512 6a13 5a14 6512 6506 640c 3c00 6515  e.j.Z.e.e.d.<.e.
+00000440: a016 640d a101 a017 640e a101 5a18 6515  ..d.....d...Z.e.
+00000450: 6506 640f 3c00 6410 5a19 6508 6506 6411  e.d.<.d.Z.e.e.d.
+00000460: 3c00 6412 5a1a 651b 6506 6413 3c00 6404  <.d.Z.e.e.d.<.d.
+00000470: 5a1c 651d 6506 6414 3c00 0900 6415 5a1e  Z.e.e.d.<...d.Z.
+00000480: 650d 6506 6416 3c00 6417 5a1f 651b 6506  e.e.d.<.d.Z.e.e.
+00000490: 6418 3c00 6419 5a20 6508 6506 641a 3c00  d.<.d.Z e.e.d.<.
+000004a0: 6415 5a21 650d 6506 641b 3c00 6522 6508  d.Z!e.e.d.<.e"e.
+000004b0: 6503 6602 1900 6506 641c 3c00 641d 641e  e.f...e.d.<.d.d.
+000004c0: 8400 5a23 6524 091f 6432 6420 6508 6421  ..Z#e$..d2d e.d!
+000004d0: 6508 6422 6508 6606 6423 6424 8405 8301  e.d"e.f.d#d$....
+000004e0: 5a25 0904 0904 091f 6433 6420 6508 6407  Z%......d3d e.d.
+000004f0: 650d 6422 6508 6425 6526 6a27 6608 6426  e.d"e.d%e&j'f.d&
+00000500: 6427 8405 5a28 6428 6526 6a27 6602 6429  d'..Z(d(e&j'f.d)
+00000510: 642a 8404 5a29 652a 0904 0915 091f 6434  d*..Z)e*......d4
+00000520: 6420 6508 6407 650d 6422 6508 6606 642b  d e.d.e.d"e.f.d+
+00000530: 642c 8405 8301 5a2b 642d 642e 8400 5a2c  d,....Z+d-d...Z,
+00000540: 0904 0904 091f 0904 092f 6435 6420 6508  ........./d5d e.
+00000550: 6407 650d 6422 6508 6606 6430 6431 8405  d.e.d"e.f.d0d1..
+00000560: 5a2d 6404 5300 2936 da0d 4c6f 6767 696e  Z-d.S.)6..Loggin
+00000570: 6743 6f6e 6669 67da 1163 6f6e 736f 6c65  gConfig..console
+00000580: 5f6c 6f67 5f6c 6576 656c 7a35 2528 6173  _log_levelz5%(as
+00000590: 6374 696d 6529 7320 2d20 2528 6c65 7665  ctime)s - %(leve
+000005a0: 6c6e 616d 6529 2d38 7320 2d20 2528 6e61  lname)-8s - %(na
+000005b0: 6d65 2973 3a20 2528 6d65 7373 6167 6529  me)s: %(message)
+000005c0: 73da 1463 6f6e 736f 6c65 5f65 6e74 7279  s..console_entry
+000005d0: 5f66 6f72 6d61 744e da0a 6c6f 675f 666f  _formatN..log_fo
+000005e0: 6c64 6572 da0d 6c6f 675f 6669 6c65 5f6e  lder..log_file_n
+000005f0: 616d 65da 1961 6464 5f64 6174 655f 746f  ame..add_date_to
+00000600: 5f6c 6f67 5f66 696c 655f 6e61 6d65 7a15  _log_file_namez.
+00000610: 5f25 595f 256d 5f25 645f 6174 5f25 485f  _%Y_%m_%d_at_%H_
+00000620: 254d 5f25 53da 1e6c 6f67 5f66 696c 655f  %M_%S..log_file_
+00000630: 6e61 6d65 5f64 6174 655f 7469 6d65 5f66  name_date_time_f
+00000640: 6f72 6d61 74da 0e66 696c 655f 6c6f 675f  ormat..file_log_
+00000650: 6c65 7665 6cda 156c 6f67 5f66 696c 655f  level..log_file_
+00000660: 656e 7472 795f 666f 726d 6174 da17 6c6f  entry_format..lo
+00000670: 675f 6669 6c65 5f72 6f74 6174 696f 6e5f  g_file_rotation_
+00000680: 636c 6173 737a 0531 3020 4d42 da01 62da  classz.10 MB..b.
+00000690: 116c 6f67 5f66 696c 655f 6d61 785f 7369  .log_file_max_si
+000006a0: 7a65 da08 6d69 646e 6967 6874 da1c 6c6f  ze..midnight..lo
+000006b0: 675f 6669 6c65 5f74 696d 6564 5f72 6f74  g_file_timed_rot
+000006c0: 6174 696f 6e5f 7768 656e e901 0000 00da  ation_when......
+000006d0: 206c 6f67 5f66 696c 655f 7469 6d65 645f   log_file_timed_
+000006e0: 726f 7461 7469 6f6e 5f69 6e74 6572 7661  rotation_interva
+000006f0: 6cda 1e6c 6f67 5f66 696c 655f 7469 6d65  l..log_file_time
+00000700: 645f 726f 7461 7469 6f6e 5f61 7474 696d  d_rotation_attim
+00000710: 6546 da1b 6c6f 675f 6669 6c65 5f74 696d  eF..log_file_tim
+00000720: 6564 5f72 6f74 6174 696f 6e5f 7574 63e9  ed_rotation_utc.
+00000730: 0a00 0000 da11 6c6f 675f 6669 6c65 735f  ......log_files_
+00000740: 746f 5f6b 6565 707a 1325 592d 256d 2d25  to_keepz.%Y-%m-%
+00000750: 6420 2548 3a25 4d3a 2553 257a da13 6c6f  d %H:%M:%S%z..lo
+00000760: 6767 696e 675f 6461 7465 5f66 6f72 6d61  gging_date_forma
+00000770: 74da 1374 7261 6365 5f6c 6f67 6769 6e67  t..trace_logging
+00000780: 5f73 6574 7570 da0a 6c6f 675f 6c65 7665  _setup..log_leve
+00000790: 6c73 6301 0000 0000 0000 0000 0000 0001  lsc.............
+000007a0: 0000 0003 0000 0043 0000 0073 2e00 0000  .......C...s....
+000007b0: 7c00 6a00 6400 7501 7213 7c00 6a01 6400  |.j.d.u.r.|.j.d.
+000007c0: 7500 7215 7402 7c00 a003 a100 9b00 6401  u.r.t.|.......d.
+000007d0: 9d02 8301 8201 6400 5300 6400 5300 2902  ......d.S.d.S.).
+000007e0: 4e7a 2d20 6c6f 675f 6669 6c65 5f6e 616d  Nz- log_file_nam
+000007f0: 6520 7365 7420 6275 7420 6e6f 206c 6f67  e set but no log
+00000800: 5f66 6f6c 6465 7220 7072 6f76 6964 6564  _folder provided
+00000810: 2904 7222 0000 0072 2100 0000 da0a 5661  ).r"...r!.....Va
+00000820: 6c75 6545 7272 6f72 da0e 6675 6c6c 5f69  lueError..full_i
+00000830: 7465 6d5f 6e61 6d65 2901 da04 7365 6c66  tem_name)...self
+00000840: 721b 0000 0072 1b00 0000 721c 0000 00da  r....r....r.....
+00000850: 105f 7661 6c69 6461 7465 5f6d 6f64 656c  ._validate_model
+00000860: 5f49 0000 0073 0a00 0000 0a01 0a01 1201  _I...s..........
+00000870: 04fe 0401 7a1e 4c6f 6767 696e 6743 6f6e  ....z.LoggingCon
+00000880: 6669 672e 5f76 616c 6964 6174 655f 6d6f  fig._validate_mo
+00000890: 6465 6c5f fa04 2e6c 6f67 da0f 6c6f 675f  del_...log..log_
+000008a0: 6669 6c65 5f70 7265 6669 78da 1064 6174  file_prefix..dat
+000008b0: 655f 7469 6d65 5f66 6f72 6d61 74da 0f6c  e_time_format..l
+000008c0: 6f67 5f66 696c 655f 7375 6666 6978 6303  og_file_suffixc.
+000008d0: 0000 0000 0000 0000 0000 0003 0000 0004  ................
+000008e0: 0000 0043 0000 0073 1a00 0000 7c00 9b00  ...C...s....|...
+000008f0: 7400 a001 a100 a002 7c01 a101 9b00 7c02  t.......|.....|.
+00000900: 9b00 9d03 5300 2901 61a6 0100 000a 2020  ....S.).a.....  
+00000910: 2020 2020 2020 4765 6e65 7261 7465 7320        Generates 
+00000920: 6120 6c6f 6720 6669 6c65 206e 616d 6520  a log file name 
+00000930: 7769 7468 2061 2067 6976 656e 2070 7265  with a given pre
+00000940: 6669 782c 2073 7566 6669 7820 616e 6420  fix, suffix and 
+00000950: 6461 7465 2074 696d 6520 666f 726d 6174  date time format
+00000960: 2e0a 0a20 2020 2020 2020 2050 6172 616d  ...        Param
+00000970: 6574 6572 730a 2020 2020 2020 2020 2d2d  eters.        --
+00000980: 2d2d 2d2d 2d2d 2d2d 0a20 2020 2020 2020  --------.       
+00000990: 206c 6f67 5f66 696c 655f 7072 6566 6978   log_file_prefix
+000009a0: 3a20 7374 720a 2020 2020 2020 2020 2020  : str.          
+000009b0: 2020 5468 6520 7061 7274 206f 6620 7468    The part of th
+000009c0: 6520 6c6f 6720 6669 6c65 206e 616d 6520  e log file name 
+000009d0: 6265 666f 7265 2074 6865 2064 6174 650a  before the date.
+000009e0: 2020 2020 2020 2020 6c6f 675f 6669 6c65          log_file
+000009f0: 5f73 7566 6669 783a 2073 7472 0a20 2020  _suffix: str.   
+00000a00: 2020 2020 2020 2020 2054 6865 2070 6172           The par
+00000a10: 7420 6f66 2074 6865 206c 6f67 2066 696c  t of the log fil
+00000a20: 6520 6e61 6d65 2061 6674 6572 2074 6865  e name after the
+00000a30: 2064 6174 650a 2020 2020 2020 2020 6461   date.        da
+00000a40: 7465 5f74 696d 655f 666f 726d 6174 3a20  te_time_format: 
+00000a50: 7374 720a 2020 2020 2020 2020 2020 2020  str.            
+00000a60: 4f70 7469 6f6e 616c 2e20 5468 6520 6461  Optional. The da
+00000a70: 7465 2074 696d 6520 666f 726d 6174 2074  te time format t
+00000a80: 6f20 7573 652e 2044 6566 6175 6c74 7320  o use. Defaults 
+00000a90: 746f 2027 5f25 595f 256d 5f25 645f 6174  to '_%Y_%m_%d_at
+00000aa0: 5f25 485f 254d 5f25 5327 0a20 2020 2020  _%H_%M_%S'.     
+00000ab0: 2020 2029 0372 0400 0000 da03 6e6f 77da     ).r......now.
+00000ac0: 0873 7472 6674 696d 65a9 0372 3a00 0000  .strftime..r:...
+00000ad0: 723b 0000 0072 3c00 0000 721b 0000 0072  r;...r<...r....r
+00000ae0: 1b00 0000 721c 0000 00da 1767 6574 5f64  ....r......get_d
+00000af0: 6174 6564 5f6c 6f67 5f66 696c 655f 6e61  ated_log_file_na
+00000b00: 6d65 4e00 0000 7302 0000 001a 127a 254c  meN...s......z%L
+00000b10: 6f67 6769 6e67 436f 6e66 6967 2e67 6574  oggingConfig.get
+00000b20: 5f64 6174 6564 5f6c 6f67 5f66 696c 655f  _dated_log_file_
+00000b30: 6e61 6d65 da06 7265 7475 726e 6304 0000  name..returnc...
+00000b40: 0000 0000 0000 0000 000b 0000 0009 0000  ................
+00000b50: 0043 0000 0073 be01 0000 7400 a001 7402  .C...s....t...t.
+00000b60: a101 7d04 7400 a001 a100 7d05 7c02 6400  ..}.t.....}.|.d.
+00000b70: 7500 7210 7c00 6a03 7d02 7c01 6400 7500  u.r.|.j.}.|.d.u.
+00000b80: 7220 7c00 6a04 6400 7501 721d 7c00 6a04  r |.j.d.u.r.|.j.
+00000b90: 7d06 6e2c 6400 7d06 6e29 7c04 a005 6401  }.n,d.}.n)|...d.
+00000ba0: 7c01 9b00 9d02 a101 0100 7c02 6400 7500  |.........|.d.u.
+00000bb0: 7237 7c00 6a06 7407 6a08 6b02 7235 6402  r7|.j.t.j.k.r5d.
+00000bc0: 7d02 6e02 6403 7d02 7c02 7243 7409 6a0a  }.n.d.}.|.rCt.j.
+00000bd0: 7c01 7c00 6a0b 7c03 6404 8d03 7d06 6e06  |.|.j.|.d...}.n.
+00000be0: 7c01 9b00 7c03 9b00 9d02 7d06 6400 7d07  |...|.....}.d.}.
+00000bf0: 7c06 6400 7501 72d5 7c00 6a0c 6400 7501  |.d.u.r.|.j.d.u.
+00000c00: 7261 740d 7c06 8301 a00e a100 7361 740d  rat.|.......sat.
+00000c10: 7c00 6a0c 7c06 8302 7d08 6e04 740d 7c06  |.j.|...}.n.t.|.
+00000c20: 8301 7d08 7c00 6a0f 7270 7c04 a005 6405  ..}.|.j.rp|...d.
+00000c30: 7c08 9b00 9d02 a101 0100 7c08 6a10 7d09  |.........|.j.}.
+00000c40: 7c09 a00e a100 727e 7c09 6a11 6403 6403  |.....r~|.j.d.d.
+00000c50: 6406 8d02 0100 7c00 6a06 7407 6a12 6b02  d.....|.j.t.j.k.
+00000c60: 728f 7412 7c08 7c00 6a13 7c00 6a14 6407  r.t.|.|.j.|.j.d.
+00000c70: 6408 8d04 7d07 6e24 7c00 6a06 7407 6a08  d...}.n$|.j.t.j.
+00000c80: 6b02 72ab 7408 7c08 7c00 6a15 7c00 6a16  k.r.t.|.|.j.|.j.
+00000c90: 7c00 6a17 7c00 6a18 7c00 6a14 6407 6409  |.j.|.j.|.j.d.d.
+00000ca0: 8d07 7d07 640a 640b 8400 7c07 5f19 6e08  ..}.d.d...|._.n.
+00000cb0: 741a 640c 7c00 6a06 9b00 9d02 8301 8201  t.d.|.j.........
+00000cc0: 741b 7c00 6a1c 7c00 6a1d 8302 7d0a 7c07  t.|.j.|.j...}.|.
+00000cd0: a01e 7c0a a101 0100 7c07 a01f 7c00 6a20  ..|.....|...|.j 
+00000ce0: a101 0100 7c05 a021 7c07 a101 0100 7c04  ....|..!|.....|.
+00000cf0: a005 640d 7c00 6a20 9b00 9d02 a101 0100  ..d.|.j ........
+00000d00: 7c07 5300 7c00 6a0f 72dd 7c04 a005 640e  |.S.|.j.r.|...d.
+00000d10: a101 0100 7c07 5300 290f 4e7a 1b55 7369  ....|.S.).Nz.Usi
+00000d20: 6e67 2063 6f64 6520 7072 6f76 6964 6564  ng code provided
+00000d30: 2070 7265 6669 7820 4654 723f 0000 007a   prefix FTr?...z
+00000d40: 0f4c 6f67 6769 6e67 2070 6174 6820 3d20  .Logging path = 
+00000d50: 2902 da07 7061 7265 6e74 73da 0865 7869  )...parents..exi
+00000d60: 7374 5f6f 6bda 0475 7466 3829 04da 0866  st_ok..utf8)...f
+00000d70: 696c 656e 616d 65da 086d 6178 4279 7465  ilename..maxByte
+00000d80: 73da 0b62 6163 6b75 7043 6f75 6e74 da08  s..backupCount..
+00000d90: 656e 636f 6469 6e67 2907 7245 0000 00da  encoding).rE....
+00000da0: 0477 6865 6eda 0869 6e74 6572 7661 6cda  .when..interval.
+00000db0: 0661 7454 696d 65da 0375 7463 7247 0000  .atTime..utcrG..
+00000dc0: 0072 4800 0000 6301 0000 0000 0000 0000  .rH...c.........
+00000dd0: 0000 0001 0000 0004 0000 0053 0000 0073  ...........S...s
+00000de0: 1000 0000 7c00 a000 6401 6402 a102 6401  ....|...d.d...d.
+00000df0: 1700 5300 2903 4e72 3900 0000 da00 2901  ..S.).Nr9.....).
+00000e00: da07 7265 706c 6163 6529 01da 046e 616d  ..replace)...nam
+00000e10: 6572 1b00 0000 721b 0000 0072 1c00 0000  er....r....r....
+00000e20: da08 3c6c 616d 6264 613e a600 0000 7302  ..<lambda>....s.
+00000e30: 0000 0010 007a 344c 6f67 6769 6e67 436f  .....z4LoggingCo
+00000e40: 6e66 6967 2e61 6464 5f6c 6f67 5f66 696c  nfig.add_log_fil
+00000e50: 655f 6861 6e64 6c65 722e 3c6c 6f63 616c  e_handler.<local
+00000e60: 733e 2e3c 6c61 6d62 6461 3e7a 1f42 6164  s>.<lambda>z.Bad
+00000e70: 206c 6f67 5f66 696c 655f 726f 7461 7469   log_file_rotati
+00000e80: 6f6e 5f63 6c61 7373 206f 6620 7a11 4669  on_class of z.Fi
+00000e90: 6c65 206c 6f67 206c 6576 656c 203d 207a  le log level = z
+00000ea0: 2e4e 6f20 6c6f 6720 6669 6c65 6e61 6d65  .No log filename
+00000eb0: 2064 6566 696e 6564 2e20 4669 6c65 206c   defined. File l
+00000ec0: 6f67 6769 6e67 2073 6b69 7070 6564 2e29  ogging skipped.)
+00000ed0: 22da 076c 6f67 6769 6e67 da09 6765 744c  "..logging..getL
+00000ee0: 6f67 6765 7272 1100 0000 7223 0000 0072  oggerr....r#...r
+00000ef0: 2200 0000 da04 696e 666f 7227 0000 0072  ".....infor'...r
+00000f00: 1d00 0000 7207 0000 0072 1e00 0000 7240  ....r....r....r@
+00000f10: 0000 0072 2400 0000 7221 0000 0072 0800  ...r$...r!...r..
+00000f20: 0000 da0b 6973 5f61 6273 6f6c 7574 6572  ....is_absoluter
+00000f30: 3300 0000 da06 7061 7265 6e74 da05 6d6b  3.....parent..mk
+00000f40: 6469 7272 0600 0000 7229 0000 0072 3100  dirr....r)...r1.
+00000f50: 0000 722b 0000 0072 2d00 0000 722e 0000  ..r+...r-...r...
+00000f60: 0072 2f00 0000 da05 6e61 6d65 7272 3500  .r/.....namerr5.
+00000f70: 0000 720f 0000 0072 2600 0000 7232 0000  ..r....r&...r2..
+00000f80: 00da 0c73 6574 466f 726d 6174 7465 72da  ...setFormatter.
+00000f90: 0873 6574 4c65 7665 6c72 2500 0000 da0a  .setLevelr%.....
+00000fa0: 6164 6448 616e 646c 6572 290b 7237 0000  addHandler).r7..
+00000fb0: 0072 3a00 0000 7223 0000 0072 3c00 0000  .r:...r#...r<...
+00000fc0: da03 6c6f 67da 0b72 6f6f 745f 6c6f 6767  ..log..root_logg
+00000fd0: 6572 7222 0000 005a 0c66 696c 655f 6861  err"...Z.file_ha
+00000fe0: 6e64 6c65 725a 0d6c 6f67 5f66 696c 655f  ndlerZ.log_file_
+00000ff0: 7061 7468 5a08 6469 725f 6e61 6d65 5a18  pathZ.dir_nameZ.
+00001000: 6c6f 675f 6669 6c65 5f65 6e74 7279 5f66  log_file_entry_f
+00001010: 6f72 6d61 7474 6572 721b 0000 0072 1b00  ormatterr....r..
+00001020: 0000 721c 0000 00da 1461 6464 5f6c 6f67  ..r......add_log
+00001030: 5f66 696c 655f 6861 6e64 6c65 7262 0000  _file_handlerb..
+00001040: 0073 7400 0000 0a06 0801 0801 0601 0801  .st.............
+00001050: 0a01 0801 0602 1002 0801 0c01 0601 0402  ................
+00001060: 0402 0401 0201 0401 0201 08fd 0c06 0402  ................
+00001070: 0801 1601 0e01 0802 0602 1001 0605 0803  ................
+00001080: 0e01 0c02 0201 0201 0401 0401 0201 08fc  ................
+00001090: 0c06 0201 0201 0401 0401 0401 0401 0401  ................
+000010a0: 0201 06f9 0c09 1002 0e02 0a01 0c01 0a01  ................
+000010b0: 1201 0404 06fe 0a01 0401 7a22 4c6f 6767  ..........z"Logg
+000010c0: 696e 6743 6f6e 6669 672e 6164 645f 6c6f  ingConfig.add_lo
+000010d0: 675f 6669 6c65 5f68 616e 646c 6572 da07  g_file_handler..
+000010e0: 6861 6e64 6c65 7263 0200 0000 0000 0000  handlerc........
+000010f0: 0000 0000 0400 0000 0400 0000 4300 0000  ............C...
+00001100: 735e 0000 0074 00a0 0174 02a1 017d 027c  s^...t...t...}.|
+00001110: 0164 0075 0172 237c 006a 0372 147c 02a0  .d.u.r#|.j.r.|..
+00001120: 0464 017c 019b 009d 02a1 0101 0074 00a0  .d.|.........t..
+00001130: 01a1 007d 037c 03a0 057c 01a1 0101 007c  ...}.|...|.....|
+00001140: 01a0 06a1 0001 0064 0053 007c 006a 0372  .......d.S.|.j.r
+00001150: 2d7c 02a0 0464 02a1 0101 0064 0053 0064  -|...d.....d.S.d
+00001160: 0053 0029 034e 7a14 436c 6f73 696e 6720  .S.).Nz.Closing 
+00001170: 6c6f 6720 6861 6e64 6c65 7220 7a29 4e6f  log handler z)No
+00001180: 2068 616e 646c 6572 2070 726f 7669 6465   handler provide
+00001190: 6420 746f 2072 656d 6f76 655f 6c6f 675f  d to remove_log_
+000011a0: 6861 6e64 6c65 7229 0772 5100 0000 7252  handler).rQ...rR
+000011b0: 0000 0072 1100 0000 7233 0000 0072 5300  ...r....r3...rS.
+000011c0: 0000 da0d 7265 6d6f 7665 4861 6e64 6c65  ....removeHandle
+000011d0: 72da 0563 6c6f 7365 2904 7237 0000 0072  r..close).r7...r
+000011e0: 5e00 0000 725b 0000 0072 5c00 0000 721b  ^...r[...r\...r.
+000011f0: 0000 0072 1b00 0000 721c 0000 00da 1272  ...r....r......r
+00001200: 656d 6f76 655f 6c6f 675f 6861 6e64 6c65  emove_log_handle
+00001210: 72b4 0000 0073 1400 0000 0a01 0801 0601  r....s..........
+00001220: 1001 0801 0a01 0c01 0602 0e01 04ff 7a20  ..............z 
+00001230: 4c6f 6767 696e 6743 6f6e 6669 672e 7265  LoggingConfig.re
+00001240: 6d6f 7665 5f6c 6f67 5f68 616e 646c 6572  move_log_handler
+00001250: 6304 0000 0000 0000 0000 0000 0005 0000  c...............
+00001260: 0009 0000 0063 0000 0073 3600 0000 8100  .....c...s6.....
+00001270: 7c00 6a00 7c01 7c02 7c03 6401 8d03 7d04  |.j.|.|.|.d...}.
+00001280: 7a0b 7c04 5600 0100 5700 7c00 a001 7c04  z.|.V...W.|...|.
+00001290: a101 0100 6400 5300 7c00 a001 7c04 a101  ....d.S.|...|...
+000012a0: 0100 7700 2902 4ea9 0372 3a00 0000 7223  ..w.).N..r:...r#
+000012b0: 0000 0072 3c00 0000 2902 725d 0000 0072  ...r<...).r]...r
+000012c0: 6100 0000 2905 7237 0000 0072 3a00 0000  a...).r7...r:...
+000012d0: 7223 0000 0072 3c00 0000 5a10 6c6f 675f  r#...r<...Z.log_
+000012e0: 6669 6c65 5f68 616e 646c 6572 721b 0000  file_handlerr...
+000012f0: 0072 1b00 0000 721c 0000 00da 106c 6f67  .r....r......log
+00001300: 5f66 696c 655f 6d61 6e61 6765 72c0 0000  _file_manager...
+00001310: 0073 1200 0000 0280 0407 0201 0201 0201  .s..............
+00001320: 06fd 0205 0801 1a03 7a1e 4c6f 6767 696e  ........z.Loggin
+00001330: 6743 6f6e 6669 672e 6c6f 675f 6669 6c65  gConfig.log_file
+00001340: 5f6d 616e 6167 6572 6301 0000 0000 0000  _managerc.......
+00001350: 0000 0000 000a 0000 000b 0000 0043 0000  .............C..
+00001360: 0073 9c01 0000 7400 8300 7d01 7401 a002  .s....t...}.t...
+00001370: a100 7d02 7403 7401 6a04 6a05 6a06 8301  ..}.t.t.j.j.j...
+00001380: 7d03 7c03 7401 6a04 6a05 5f06 7c00 6a07  }.|.t.j.j._.|.j.
+00001390: a008 a100 4400 5d37 5c02 7d04 7d05 7c04  ....D.]7\.}.}.|.
+000013a0: a009 a100 6401 6b02 7225 7c02 7d06 6e05  ....d.k.r%|.}.n.
+000013b0: 7401 a002 7c04 a101 7d06 7c06 7c01 7c04  t...|...}.|.|.|.
+000013c0: 3c00 6402 7c06 5f0a 7c05 6400 7500 7238  <.d.|._.|.d.u.r8
+000013d0: 6403 7d05 6e04 7c05 a00b a100 7d05 7c00  d.}.n.|.....}.|.
+000013e0: 6a0c 724a 740d 6404 7c06 6a0e 9b00 6405  j.rJt.d.|.j...d.
+000013f0: 7c05 9b00 9d04 8301 0100 7c06 a00f 7c05  |.........|...|.
+00001400: a101 0100 7118 7410 7401 6a04 6a05 6a06  ....q.t.t.j.j.j.
+00001410: 8301 4400 5d5b 7d04 7401 a002 7c04 a101  ..D.][}.t...|...
+00001420: 7d06 7c00 6a0c 726c 740d 6406 7c04 9b00  }.|.j.rlt.d.|...
+00001430: 6407 7c06 6a11 9b00 9d04 8301 0100 7c04  d.|.j.........|.
+00001440: 7c01 7601 72b2 7c00 6a0c 7282 740d 6408  |.v.r.|.j.r.t.d.
+00001450: 7c04 9b00 6409 7401 a012 7c06 a013 a100  |...d.t...|.....
+00001460: a101 9b00 9d04 8301 0100 7410 7c01 8301  ..........t.|...
+00001470: 4400 5d2b 7d07 7c04 a014 7c07 a101 72b1  D.]+}.|...|...r.
+00001480: 7c01 7c07 1900 7d08 7c08 a013 a100 7d09  |.|...}.|.....}.
+00001490: 7c06 a00f 7c09 a101 0100 7c00 6a0c 72ae  |...|.....|.j.r.
+000014a0: 740d 640a 7c04 9b00 640b 7c08 6a0e 9b00  t.d.|...d.|.j...
+000014b0: 640c 7401 a012 7c09 a101 9b00 9d06 8301  d.t...|.........
+000014c0: 0100 6402 7c06 5f0a 7186 7157 7c00 6a0c  ..d.|._.q.qW|.j.
+000014d0: 72cc 740d 640d 7401 a012 7c02 a013 a100  r.t.d.t...|.....
+000014e0: a101 9b00 9d02 8301 0100 740d 640e 7c02  ..........t.d.|.
+000014f0: 6a11 9b00 9d02 8301 0100 6400 5300 6400  j.........d.S.d.
+00001500: 5300 290f 4eda 0472 6f6f 7454 7218 0000  S.).N..rootTr...
+00001510: 007a 0f53 6574 7469 6e67 206c 6f67 6765  .z.Setting logge
+00001520: 7220 7a04 2074 6f20 7a07 4c6f 6767 6572  r z. to z.Logger
+00001530: 207a 0a20 6861 6e64 6c65 7273 207a 1943   z. handlers z.C
+00001540: 6865 636b 696e 6720 6578 6973 7469 6e67  hecking existing
+00001550: 206c 6f67 6765 7220 7a07 206c 6576 656c   logger z. level
+00001560: 207a 1045 7869 7374 696e 6720 6c6f 6767   z.Existing logg
+00001570: 6572 207a 0f20 7265 2d73 6574 7570 2077  er z. re-setup w
+00001580: 6974 6820 7a0a 2073 6574 7469 6e67 7320  ith z. settings 
+00001590: 7a16 526f 6f74 206c 6f67 6769 6e67 206c  z.Root logging l
+000015a0: 6576 656c 2069 7320 7a1a 526f 6f74 206c  evel is z.Root l
+000015b0: 6f67 6769 6e67 2068 616e 646c 6572 7320  ogging handlers 
+000015c0: 6172 6520 2915 da04 6469 6374 7251 0000  are )...dictrQ..
+000015d0: 0072 5200 0000 720a 0000 00da 064c 6f67  .rR...r......Log
+000015e0: 6765 72da 076d 616e 6167 6572 da0a 6c6f  ger..manager..lo
+000015f0: 6767 6572 4469 6374 7234 0000 00da 0569  ggerDictr4.....i
+00001600: 7465 6d73 da05 6c6f 7765 72da 0970 726f  tems..lower..pro
+00001610: 7061 6761 7465 da05 7570 7065 7272 3300  pagate..upperr3.
+00001620: 0000 da05 7072 696e 7472 4f00 0000 7259  ....printrO...rY
+00001630: 0000 00da 0673 6f72 7465 64da 0868 616e  .....sorted..han
+00001640: 646c 6572 73da 0c67 6574 4c65 7665 6c4e  dlers..getLevelN
+00001650: 616d 65da 1167 6574 4566 6665 6374 6976  ame..getEffectiv
+00001660: 654c 6576 656c da0a 7374 6172 7473 7769  eLevel..startswi
+00001670: 7468 290a 7237 0000 005a 1263 6f6e 6669  th).r7...Z.confi
+00001680: 6775 7265 645f 6c6f 6767 6572 7372 5c00  gured_loggersr\.
+00001690: 0000 5a0b 6c6f 6767 6572 5f64 6963 745a  ..Z.logger_dictZ
+000016a0: 0c6c 6f67 6765 725f 636c 6173 735a 1264  .logger_classZ.d
+000016b0: 6573 6972 6564 5f6c 6576 656c 5f6e 616d  esired_level_nam
+000016c0: 65da 066c 6f67 6765 725a 0e63 6f6d 7061  e..loggerZ.compa
+000016d0: 7265 5f6c 6f67 6765 725a 0d70 6172 656e  re_loggerZ.paren
+000016e0: 745f 6c6f 6767 6572 da05 6c65 7665 6c72  t_logger..levelr
+000016f0: 1b00 0000 721b 0000 0072 1c00 0000 da10  ....r....r......
+00001700: 7365 7475 705f 6c6f 675f 6c65 7665 6c73  setup_log_levels
+00001710: d200 0000 7358 0000 0006 0108 010e 030a  ....sX..........
+00001720: 0112 020c 0106 010a 0208 0106 0108 0106  ................
+00001730: 0108 0206 0116 020c 0112 030a 0106 0116  ................
+00001740: 0108 0106 0102 0208 010c 0104 ff04 ff0c  ................
+00001750: 040a 0108 0108 010a 0106 0102 0210 0108  ................
+00001760: 0104 ff04 ff06 0404 8006 0218 0214 0104  ................
+00001770: fd7a 1e4c 6f67 6769 6e67 436f 6e66 6967  .z.LoggingConfig
+00001780: 2e73 6574 7570 5f6c 6f67 5f6c 6576 656c  .setup_log_level
+00001790: 7354 6306 0000 0000 0000 0000 0000 0011  sTc.............
+000017a0: 0000 0005 0000 0043 0000 0073 7601 0000  .......C...sv...
+000017b0: 7400 a001 a100 7d06 7402 7c06 6401 8302  t.....}.t.|.d...
+000017c0: 73b9 6402 7c06 5f03 7c06 6a04 4400 5d0a  s.d.|._.|.j.D.].
+000017d0: 7d07 7c07 a005 a100 0100 7c07 a006 a100  }.|.......|.....
+000017e0: 0100 710f 7c06 6a04 a007 a100 0100 7c00  ..q.|.j.......|.
+000017f0: 6a08 722e 7409 6403 8301 0100 7409 6404  j.r.t.d.....t.d.
+00001800: 7c06 6a04 9b00 9d02 8301 0100 7c06 a00a  |.j.........|...
+00001810: 7400 6a0b a101 0100 7c04 6405 7500 723f  t.j.....|.d.u.r?
+00001820: 740c 6a0d 7d08 740c 6a0e 7d09 6e04 7c04  t.j.}.t.j.}.n.|.
+00001830: 7d08 7c04 7d09 7400 a00f 7c08 a101 7d0a  }.|.}.t...|...}.
+00001840: 7c0a a00a 7400 6a10 a101 0100 7c06 a011  |...t.j.....|...
+00001850: 7c0a a101 0100 7400 a00f 7c09 a101 7d0b  |.....t...|...}.
+00001860: 7c0b a00a 7c00 6a12 a101 0100 6406 6407  |...|.j.....d.d.
+00001870: 8400 7d0c 7c0b a013 7c0c a101 0100 7c06  ..}.|...|.....|.
+00001880: a011 7c0b a101 0100 7c00 6a14 7d0d 7c0d  ..|.....|.j.}.|.
+00001890: 7281 7415 7c0d 7c00 6a16 8302 7d0e 7c0b  r.t.|.|.j...}.|.
+000018a0: a017 7c0e a101 0100 7c0a a017 7c0e a101  ..|.....|...|...
+000018b0: 0100 7c00 a018 a100 0100 7400 a001 7419  ..|.......t...t.
+000018c0: a101 7d0f 7400 a01a 6402 a101 0100 7400  ..}.t...d.....t.
+000018d0: a01b 7c0f a01c a100 a101 7d10 7c00 6a08  ..|.......}.|.j.
+000018e0: 72a1 7c0f a01d 6408 7c10 9b00 9d02 a101  r.|...d.|.......
+000018f0: 0100 7c05 73a7 7c01 6405 7501 72af 7c00  ..|.s.|.d.u.r.|.
+00001900: 6a1e 7c01 7c02 7c03 6409 8d03 5300 7c00  j.|.|.|.d...S.|.
+00001910: 6a08 72b7 7c0f a01d 640a a101 0100 6405  j.r.|...d.....d.
+00001920: 5300 6405 5300 290b 7a37 0a20 2020 2020  S.d.S.).z7.     
+00001930: 2020 2053 6574 7570 206c 6f67 6769 6e67     Setup logging
+00001940: 2062 6173 6564 206f 6e20 636f 6e66 6967   based on config
+00001950: 7572 6174 696f 6e2e 0a20 2020 2020 2020  uration..       
+00001960: 20da 1a63 6f6e 6669 675f 7772 616e 676c   ..config_wrangl
+00001970: 6572 5f73 6574 7570 5f64 6f6e 6554 7a1c  er_setup_doneTz.
+00001980: 6c6f 6767 696e 672e 7472 6163 655f 7365  logging.trace_se
+00001990: 7475 7020 6973 2054 7275 657d 7a1e 5374  tup is True}z.St
+000019a0: 6172 7469 6e67 2072 6f6f 7420 6c6f 6767  arting root logg
+000019b0: 6572 2068 616e 646c 6572 7320 4e63 0100  er handlers Nc..
+000019c0: 0000 0000 0000 0000 0000 0100 0000 0200  ................
+000019d0: 0000 5300 0000 730c 0000 007c 006a 0074  ..S...s....|.j.t
+000019e0: 016a 026b 0353 0029 014e 2903 da07 6c65  .j.k.S.).N)...le
+000019f0: 7665 6c6e 6f72 5100 0000 7216 0000 0029  velnorQ...r....)
+00001a00: 01da 0672 6563 6f72 6472 1b00 0000 721b  ...recordr....r.
+00001a10: 0000 0072 1c00 0000 da09 6e6f 6e5f 6572  ...r......non_er
+00001a20: 726f 723b 0100 0073 0200 0000 0c01 7a2e  ror;...s......z.
+00001a30: 4c6f 6767 696e 6743 6f6e 6669 672e 7365  LoggingConfig.se
+00001a40: 7475 705f 6c6f 6767 696e 672e 3c6c 6f63  tup_logging.<loc
+00001a50: 616c 733e 2e6e 6f6e 5f65 7272 6f72 7a1e  als>.non_errorz.
+00001a60: 5468 6973 206d 6f64 756c 6573 206c 6f67  This modules log
+00001a70: 6769 6e67 206c 6576 656c 2069 7320 7262  ging level is rb
+00001a80: 0000 007a 3875 7365 5f6c 6f67 5f66 696c  ...z8use_log_fil
+00001a90: 655f 7365 7474 696e 6720 3d20 4661 6c73  e_setting = Fals
+00001aa0: 652e 2073 6574 7570 5f6c 6f67 5f66 696c  e. setup_log_fil
+00001ab0: 6520 6e6f 7420 6361 6c6c 6564 2e29 1f72  e not called.).r
+00001ac0: 5100 0000 7252 0000 00da 0768 6173 6174  Q...rR.....hasat
+00001ad0: 7472 7276 0000 0072 6f00 0000 da05 666c  trrv...ro.....fl
+00001ae0: 7573 6872 6000 0000 da05 636c 6561 7272  ushr`.....clearr
+00001af0: 3300 0000 726d 0000 0072 5900 0000 7218  3...rm...rY...r.
+00001b00: 0000 00da 0373 7973 da06 7374 6465 7272  .....sys..stderr
+00001b10: da06 7374 646f 7574 da0d 5374 7265 616d  ..stdout..Stream
+00001b20: 4861 6e64 6c65 7272 1600 0000 725a 0000  Handlerr....rZ..
+00001b30: 0072 1f00 0000 da09 6164 6446 696c 7465  .r......addFilte
+00001b40: 7272 2000 0000 720f 0000 0072 3200 0000  rr ...r....r2...
+00001b50: 7258 0000 0072 7500 0000 7211 0000 00da  rX...ru...r.....
+00001b60: 0f63 6170 7475 7265 5761 726e 696e 6773  .captureWarnings
+00001b70: 7270 0000 0072 7100 0000 7253 0000 0072  rp...rq...rS...r
+00001b80: 5d00 0000 2911 7237 0000 0072 3a00 0000  ]...).r7...r:...
+00001b90: 7223 0000 0072 3c00 0000 5a0e 636f 6e73  r#...r<...Z.cons
+00001ba0: 6f6c 655f 6f75 7470 7574 5a14 7573 655f  ole_outputZ.use_
+00001bb0: 6c6f 675f 6669 6c65 5f73 6574 7469 6e67  log_file_setting
+00001bc0: 725c 0000 0072 5e00 0000 5a0c 6572 726f  r\...r^...Z.erro
+00001bd0: 725f 6f75 7470 7574 5a0e 7265 6775 6c61  r_outputZ.regula
+00001be0: 725f 6f75 7470 7574 5a11 636f 6e73 6f6c  r_outputZ.consol
+00001bf0: 655f 6572 726f 725f 6c6f 675a 0b63 6f6e  e_error_logZ.con
+00001c00: 736f 6c65 5f6c 6f67 7279 0000 0072 2000  sole_logry...r .
+00001c10: 0000 5a17 636f 6e73 6f6c 655f 656e 7472  ..Z.console_entr
+00001c20: 795f 666f 726d 6174 7465 7272 5b00 0000  y_formatterr[...
+00001c30: 5a0e 6c6f 675f 6c65 7665 6c5f 6e61 6d65  Z.log_level_name
+00001c40: 721b 0000 0072 1b00 0000 721c 0000 00da  r....r....r.....
+00001c50: 0d73 6574 7570 5f6c 6f67 6769 6e67 0801  .setup_logging..
+00001c60: 0000 735a 0000 0008 0c0a 0206 040a 0308  ..sZ............
+00001c70: 010a 010a 0306 0208 0210 010c 0308 0206  ................
+00001c80: 0108 0104 0204 010a 020c 010a 010a 020c  ................
+00001c90: 0108 030a 040a 0206 0204 010c 010a 010a  ................
+00001ca0: 0108 020a 030a 020e 0206 0110 010c 0204  ................
+00001cb0: 0102 0102 0102 0106 fd06 060a 0104 0104  ................
+00001cc0: b97a 1b4c 6f67 6769 6e67 436f 6e66 6967  .z.LoggingConfig
+00001cd0: 2e73 6574 7570 5f6c 6f67 6769 6e67 2901  .setup_logging).
+00001ce0: 7239 0000 0029 034e 4e72 3900 0000 2903  r9...).NNr9...).
+00001cf0: 4e46 7239 0000 0029 054e 4e72 3900 0000  NFr9...).NNr9...
+00001d00: 4e54 292e 7211 0000 0072 1200 0000 7213  NT).r....r....r.
+00001d10: 0000 0072 1000 0000 7218 0000 0072 1f00  ...r....r....r..
+00001d20: 0000 da0f 5f5f 616e 6e6f 7461 7469 6f6e  ....__annotation
+00001d30: 735f 5f72 2000 0000 da03 7374 7272 2100  s__r .....strr!.
+00001d40: 0000 720e 0000 0072 2200 0000 7223 0000  ..r....r"...r#..
+00001d50: 00da 0462 6f6f 6c72 2400 0000 7219 0000  ...boolr$...r...
+00001d60: 0072 2500 0000 7226 0000 0072 1d00 0000  .r%...r&...r....
+00001d70: 7206 0000 0072 2700 0000 7209 0000 00da  r....r'...r.....
+00001d80: 0876 616c 6964 6174 65da 0274 6f72 2900  .validate..tor).
+00001d90: 0000 722b 0000 0072 2d00 0000 da03 696e  ..r+...r-.....in
+00001da0: 7472 2e00 0000 7205 0000 0072 2f00 0000  tr....r....r/...
+00001db0: 7231 0000 0072 3200 0000 7233 0000 00da  r1...r2...r3....
+00001dc0: 0444 6963 7472 3800 0000 da0c 7374 6174  .Dictr8.....stat
+00001dd0: 6963 6d65 7468 6f64 7240 0000 0072 5100  icmethodr@...rQ.
+00001de0: 0000 da07 4861 6e64 6c65 7272 5d00 0000  ....Handlerr]...
+00001df0: 7261 0000 0072 0300 0000 7263 0000 0072  ra...r....rc...r
+00001e00: 7500 0000 7283 0000 0072 1b00 0000 721b  u...r....r....r.
+00001e10: 0000 0072 1b00 0000 721c 0000 0072 1e00  ...r....r....r..
+00001e20: 0000 2400 0000 7386 0000 000a 000e 010c  ..$...s.........
+00001e30: 010c 010c 010c 010c 010e 010c 010e 0118  ................
+00001e40: 040c 040c 010c 0102 010c 0a0c 020c 010c  ................
+00001e50: 0110 0108 0202 0502 0404 fd02 0102 ff02  ................
+00001e60: 0202 fe02 030c fd02 1502 0102 0104 fc02  ................
+00001e70: 0202 fe02 0302 fd02 0402 fc04 050a fb10  ................
+00001e80: 5202 0c02 0302 0102 0104 fc02 0202 fe02  R...............
+00001e90: 0302 fd02 040c fc08 1102 3802 0102 0102  ..........8.....
+00001ea0: 0102 0104 fa02 0202 fe02 0302 fd02 040e  ................
+00001eb0: fc72 1e00 0000 291c 7251 0000 0072 7d00  .r....).rQ...r}.
+00001ec0: 0000 da06 7479 7069 6e67 da0a 636f 6e74  ....typing..cont
+00001ed0: 6578 746c 6962 7203 0000 0072 0400 0000  extlibr....r....
+00001ee0: 7205 0000 00da 106c 6f67 6769 6e67 2e68  r......logging.h
+00001ef0: 616e 646c 6572 7372 0600 0000 7207 0000  andlersr....r...
+00001f00: 00da 0770 6174 686c 6962 7208 0000 00da  ...pathlibr.....
+00001f10: 0870 7964 616e 7469 6372 0900 0000 da07  .pydanticr......
+00001f20: 7079 6469 6374 6972 0a00 0000 da31 636f  pydictir.....1co
+00001f30: 6e66 6967 5f77 7261 6e67 6c65 722e 636f  nfig_wrangler.co
+00001f40: 6e66 6967 5f74 656d 706c 6174 6573 2e63  nfig_templates.c
+00001f50: 6f6e 6669 675f 6869 6572 6172 6368 7972  onfig_hierarchyr
+00001f60: 0b00 0000 5a21 636f 6e66 6967 5f77 7261  ....Z!config_wra
+00001f70: 6e67 6c65 722e 636f 6e66 6967 5f74 7970  ngler.config_typ
+00001f80: 6573 2e65 6e75 6d72 0c00 0000 720d 0000  es.enumr....r...
+00001f90: 00da 2763 6f6e 6669 675f 7772 616e 676c  ..'config_wrangl
+00001fa0: 6572 2e63 6f6e 6669 675f 7479 7065 732e  er.config_types.
+00001fb0: 7061 7468 5f74 7970 6573 720e 0000 00da  path_typesr.....
+00001fc0: 1563 6f6e 6669 675f 7772 616e 676c 6572  .config_wrangler
+00001fd0: 2e75 7469 6c73 720f 0000 0072 1000 0000  .utilsr....r....
+00001fe0: 721d 0000 0072 1e00 0000 721b 0000 0072  r....r....r....r
+00001ff0: 1b00 0000 721b 0000 0072 1c00 0000 da08  ....r....r......
+00002000: 3c6d 6f64 756c 653e 0100 0000 7320 0000  <module>....s ..
+00002010: 0008 0008 0108 010c 0110 0110 010c 010c  ................
+00002020: 020c 010c 0210 010c 010c 0110 0310 0a14  ................
+00002030: 08                                       .
```

### Comparing `config_wrangler-0.5.4a0/config_wrangler/config_templates/__pycache__/logging_config.cpython-311.pyc` & `config_wrangler-0.5.5/config_wrangler/config_templates/__pycache__/logging_config.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `config_wrangler-0.5.4a0/config_wrangler/config_templates/__pycache__/password_defaults.cpython-310.pyc` & `config_wrangler-0.5.5/config_wrangler/config_templates/__pycache__/password_defaults.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `config_wrangler-0.5.4a0/config_wrangler/config_templates/__pycache__/password_defaults.cpython-311.pyc` & `config_wrangler-0.5.5/config_wrangler/config_templates/__pycache__/password_defaults.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `config_wrangler-0.5.4a0/config_wrangler/config_templates/__pycache__/password_source.cpython-311.pyc` & `config_wrangler-0.5.5/config_wrangler/config_templates/__pycache__/password_source.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `config_wrangler-0.5.4a0/config_wrangler/config_templates/__pycache__/sqlalchemy_database.cpython-310.pyc` & `config_wrangler-0.5.5/config_wrangler/config_templates/__pycache__/sqlalchemy_database.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `config_wrangler-0.5.4a0/config_wrangler/config_templates/__pycache__/sqlalchemy_database.cpython-311.pyc` & `config_wrangler-0.5.5/config_wrangler/config_templates/__pycache__/sqlalchemy_database.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `config_wrangler-0.5.4a0/config_wrangler/config_templates/aws/__pycache__/aws_session.cpython-310.pyc` & `config_wrangler-0.5.5/config_wrangler/config_templates/aws/__pycache__/aws_session.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `config_wrangler-0.5.4a0/config_wrangler/config_templates/aws/__pycache__/aws_session.cpython-311.pyc` & `config_wrangler-0.5.5/config_wrangler/config_templates/aws/__pycache__/aws_session.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `config_wrangler-0.5.4a0/config_wrangler/config_templates/aws/__pycache__/s3_bucket.cpython-310.pyc` & `config_wrangler-0.5.5/config_wrangler/config_templates/aws/__pycache__/s3_bucket.cpython-310.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.10, timestamp-based, .py timestamp: Tue Oct  4 13:22:13 2022 UTC, .py size: 14733 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 6f0d 0d0a 0000 0000 8533 3c63 8d39 0000  o........3<c.9..
+00000000: 6f0d 0d0a 0000 0000 a6bc 6b64 093a 0000  o.........kd.:..
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0008 0000 0040 0000 0073 dc00 0000 6400  .....@...s....d.
 00000030: 6401 6c00 6d01 5a01 0100 6400 6402 6c02  d.l.m.Z...d.d.l.
 00000040: 6d03 5a03 6d04 5a04 0100 6400 6403 6c05  m.Z.m.Z...d.d.l.
 00000050: 5400 6400 6404 6c06 6d07 5a07 0100 6400  T.d.d.l.m.Z...d.
 00000060: 6405 6c08 6d09 5a09 6d0a 5a0a 0100 6400  d.l.m.Z.m.Z...d.
 00000070: 6406 6c0b 6d0c 5a0c 0100 7a06 6400 6407  d.l.m.Z...z.d.d.
@@ -141,747 +141,750 @@
 000008c0: 7302 0000 0010 087a 1b53 335f 4275 636b  s......z.S3_Buck
 000008d0: 6574 2e67 6574 5f62 7563 6b65 745f 7265  et.get_bucket_re
 000008e0: 6769 6f6e 4eda 0e6c 6f63 616c 5f66 696c  gionN..local_fil
 000008f0: 656e 616d 65da 036b 6579 da0a 6578 7472  ename..key..extr
 00000900: 615f 6172 6773 da0f 7472 616e 7366 6572  a_args..transfer
 00000910: 5f63 6f6e 6669 6763 0500 0000 0000 0000  _configc........
 00000920: 0000 0000 0500 0000 0700 0000 4300 0000  ............C...
-00000930: 7324 0000 007c 006a 006a 0174 027c 0183  s$...|.j.j.t.|..
-00000940: 017c 006a 0374 027c 0283 017c 037c 0464  .|.j.t.|...|.|.d
-00000950: 018d 0501 0064 0053 0029 024e 2905 da08  .....d.S.).N)...
-00000960: 4669 6c65 6e61 6d65 7213 0000 00da 034b  Filenamer......K
-00000970: 6579 da09 4578 7472 6141 7267 73da 0643  ey..ExtraArgs..C
-00000980: 6f6e 6669 6729 0472 1e00 0000 da0b 7570  onfig).r......up
-00000990: 6c6f 6164 5f66 696c 65da 0373 7472 720b  load_file..strr.
-000009a0: 0000 0029 0572 1500 0000 7222 0000 0072  ...).r....r"...r
-000009b0: 2300 0000 7224 0000 0072 2500 0000 7216  #...r$...r%...r.
-000009c0: 0000 0072 1600 0000 7217 0000 0072 2a00  ...r....r....r*.
-000009d0: 0000 3d00 0000 730e 0000 0006 0706 0104  ..=...s.........
-000009e0: 0106 0102 0102 010a fb7a 1553 335f 4275  .........z.S3_Bu
-000009f0: 636b 6574 2e75 706c 6f61 645f 6669 6c65  cket.upload_file
-00000a00: 54da 0e63 7265 6174 655f 7061 7265 6e74  T..create_parent
-00000a10: 7363 0600 0000 0000 0000 0000 0000 0700  sc..............
-00000a20: 0000 0600 0000 4300 0000 7344 0000 007c  ......C...sD...|
-00000a30: 0572 0e74 007c 0283 017d 067c 066a 016a  .r.t.|...}.|.j.j
-00000a40: 0264 0164 0164 028d 0201 007c 006a 03a0  .d.d.d.....|.j..
-00000a50: 047c 006a 05a1 016a 0674 077c 0183 0174  .|.j...j.t.|...t
-00000a60: 077c 0283 017c 037c 0464 038d 0401 0064  .|...|.|.d.....d
-00000a70: 0053 0029 044e 5429 02da 0770 6172 656e  .S.).NT)...paren
-00000a80: 7473 da08 6578 6973 745f 6f6b 2904 7227  ts..exist_ok).r'
-00000a90: 0000 0072 2600 0000 7228 0000 0072 2900  ...r&...r(...r).
-00000aa0: 0000 2908 7204 0000 00da 0670 6172 656e  ..).r......paren
-00000ab0: 74da 056d 6b64 6972 7212 0000 0072 1300  t..mkdirr....r..
-00000ac0: 0000 720b 0000 00da 0d64 6f77 6e6c 6f61  ..r......downloa
-00000ad0: 645f 6669 6c65 722b 0000 0029 0772 1500  d_filer+...).r..
-00000ae0: 0000 7223 0000 0072 2200 0000 7224 0000  ..r#...r"...r$..
-00000af0: 0072 2500 0000 722c 0000 005a 0a6c 6f63  .r%...r,...Z.loc
-00000b00: 616c 5f70 6174 6872 1600 0000 7216 0000  al_pathr....r...
-00000b10: 0072 1700 0000 7231 0000 004c 0000 0073  .r....r1...L...s
-00000b20: 1200 0000 0408 0801 1001 0e01 0601 0601  ................
-00000b30: 0201 0201 0afc 7a17 5333 5f42 7563 6b65  ......z.S3_Bucke
-00000b40: 742e 646f 776e 6c6f 6164 5f66 696c 6563  t.download_filec
-00000b50: 0200 0000 0000 0000 0000 0000 0200 0000  ................
-00000b60: 0800 0000 4300 0000 7332 0000 007a 0e7c  ....C...s2...z.|
-00000b70: 006a 006a 017c 006a 0274 037c 0183 0164  .j.j.|.j.t.|...d
-00000b80: 018d 0201 0057 0064 0253 0004 0074 0479  .....W.d.S...t.y
-00000b90: 1801 0001 0001 0059 0064 0353 0077 0029  .......Y.d.S.w.)
-00000ba0: 044e a902 7213 0000 0072 2700 0000 5446  .N..r....r'...TF
-00000bb0: 2905 721e 0000 005a 0b68 6561 645f 6f62  ).r....Z.head_ob
-00000bc0: 6a65 6374 720b 0000 0072 2b00 0000 da09  jectr....r+.....
-00000bd0: 4578 6365 7074 696f 6ea9 0272 1500 0000  Exception..r....
-00000be0: 7223 0000 0072 1600 0000 7216 0000 0072  r#...r....r....r
-00000bf0: 1700 0000 da0a 6b65 795f 6578 6973 7473  ......key_exists
-00000c00: 5e00 0000 730c 0000 0002 0116 0106 010c  ^...s...........
-00000c10: 0106 0102 ff7a 1453 335f 4275 636b 6574  .....z.S3_Bucket
-00000c20: 2e6b 6579 5f65 7869 7374 7363 0200 0000  .key_existsc....
-00000c30: 0000 0000 0000 0000 0200 0000 0500 0000  ................
-00000c40: 4300 0000 7314 0000 007c 006a 00a0 017c  C...s....|.j...|
-00000c50: 006a 0274 037c 0183 01a1 0253 0072 1100  .j.t.|.....S.r..
-00000c60: 0000 2904 7212 0000 005a 064f 626a 6563  ..).r....Z.Objec
-00000c70: 7472 0b00 0000 722b 0000 0072 3400 0000  tr....r+...r4...
-00000c80: 7216 0000 0072 1600 0000 7217 0000 00da  r....r....r.....
-00000c90: 0a67 6574 5f6f 626a 6563 7465 0000 00f3  .get_objecte....
-00000ca0: 0200 0000 1401 7a14 5333 5f42 7563 6b65  ......z.S3_Bucke
-00000cb0: 742e 6765 745f 6f62 6a65 6374 da0a 7665  t.get_object..ve
-00000cc0: 7273 696f 6e5f 6964 6303 0000 0000 0000  rsion_idc.......
-00000cd0: 0000 0000 0004 0000 0004 0000 0043 0000  .............C..
-00000ce0: 0073 3600 0000 7c00 6a00 7401 7c01 8301  .s6...|.j.t.|...
-00000cf0: 6401 9c02 7d03 7c02 6400 7501 7210 7c02  d...}.|.d.u.r.|.
-00000d00: 7c03 6402 3c00 7c00 6a02 6a03 6403 6900  |.d.<.|.j.j.d.i.
-00000d10: 7c03 a401 8e01 0100 6400 5300 2904 4e72  |.......d.S.).Nr
-00000d20: 3200 0000 da09 5665 7273 696f 6e49 6472  2.....VersionIdr
-00000d30: 1600 0000 2904 720b 0000 0072 2b00 0000  ....).r....r+...
-00000d40: 721e 0000 005a 0d64 656c 6574 655f 6f62  r....Z.delete_ob
-00000d50: 6a65 6374 2904 7215 0000 0072 2300 0000  ject).r....r#...
-00000d60: 7238 0000 00da 066b 7761 7267 7372 1600  r8.....kwargsr..
-00000d70: 0000 7216 0000 0072 1700 0000 da0d 6465  ..r....r......de
-00000d80: 6c65 7465 5f62 795f 6b65 7968 0000 0073  lete_by_keyh...s
-00000d90: 0c00 0000 0402 0601 06fe 0804 0801 1601  ................
-00000da0: 7a17 5333 5f42 7563 6b65 742e 6465 6c65  z.S3_Bucket.dele
-00000db0: 7465 5f62 795f 6b65 79fa 2562 6f74 6f73  te_by_key.%botos
-00000dc0: 7475 6273 2e53 332e 5333 5265 736f 7572  tubs.S3.S3Resour
-00000dd0: 6365 2e4f 626a 6563 7453 756d 6d61 7279  ce.ObjectSummary
-00000de0: 6302 0000 0000 0000 0000 0000 0003 0000  c...............
-00000df0: 0003 0000 0043 0000 0073 2c00 0000 7c01  .....C...s,...|.
-00000e00: 6400 7500 7206 6401 7d01 7c00 6a00 a001  d.u.r.d.}.|.j...
-00000e10: 7c00 6a02 a101 6a03 6a04 7405 7c01 8301  |.j...j.j.t.|...
-00000e20: 6402 8d01 7d02 7c02 5300 2903 4eda 0029  d...}.|.S.).N..)
-00000e30: 01da 0650 7265 6669 7829 0672 1200 0000  ...Prefix).r....
-00000e40: 7213 0000 0072 0b00 0000 da07 6f62 6a65  r....r......obje
-00000e50: 6374 73da 0666 696c 7465 7272 2b00 0000  cts..filterr+...
-00000e60: 2903 7215 0000 0072 2300 0000 da0a 636f  ).r....r#.....co
-00000e70: 6c6c 6563 7469 6f6e 7216 0000 0072 1600  llectionr....r..
-00000e80: 0000 7217 0000 00da 0c66 696e 645f 6f62  ..r......find_ob
-00000e90: 6a65 6374 7371 0000 0073 0800 0000 0801  jectsq...s......
-00000ea0: 0401 1c01 0401 7a16 5333 5f42 7563 6b65  ......z.S3_Bucke
-00000eb0: 742e 6669 6e64 5f6f 626a 6563 7473 6302  t.find_objectsc.
-00000ec0: 0000 0000 0000 0000 0000 0003 0000 0003  ................
-00000ed0: 0000 0043 0000 0073 1800 0000 7c00 a000  ...C...s....|...
-00000ee0: 7c01 a101 7d02 6401 6402 8400 7c02 4400  |...}.d.d...|.D.
-00000ef0: 8301 5300 2903 4e63 0100 0000 0000 0000  ..S.).Nc........
-00000f00: 0000 0000 0200 0000 0300 0000 5300 0000  ............S...
-00000f10: 7312 0000 0067 007c 005d 057d 017c 016a  s....g.|.].}.|.j
-00000f20: 0091 0271 0253 0072 1600 0000 a901 7223  ...q.S.r......r#
-00000f30: 0000 0029 02da 022e 30da 036f 626a 7216  ...)....0..objr.
-00000f40: 0000 0072 1600 0000 7217 0000 00da 0a3c  ...r....r......<
-00000f50: 6c69 7374 636f 6d70 3e79 0000 0073 0200  listcomp>y...s..
-00000f60: 0000 1200 7a2e 5333 5f42 7563 6b65 742e  ....z.S3_Bucket.
-00000f70: 6c69 7374 5f6f 626a 6563 745f 6b65 7973  list_object_keys
-00000f80: 2e3c 6c6f 6361 6c73 3e2e 3c6c 6973 7463  .<locals>.<listc
-00000f90: 6f6d 703e 2901 7242 0000 0029 0372 1500  omp>).rB...).r..
-00000fa0: 0000 7223 0000 005a 0e6f 626a 5f63 6f6c  ..r#...Z.obj_col
-00000fb0: 6c65 6374 696f 6e72 1600 0000 7216 0000  lectionr....r...
-00000fc0: 0072 1700 0000 da10 6c69 7374 5f6f 626a  .r......list_obj
-00000fd0: 6563 745f 6b65 7973 7700 0000 7304 0000  ect_keysw...s...
-00000fe0: 000a 010e 017a 1a53 335f 4275 636b 6574  .....z.S3_Bucket
-00000ff0: 2e6c 6973 745f 6f62 6a65 6374 5f6b 6579  .list_object_key
-00001000: 7363 0200 0000 0000 0000 0000 0000 0200  sc..............
-00001010: 0000 0400 0000 4300 0000 7314 0000 0064  ......C...s....d
-00001020: 0164 0284 007c 00a0 007c 01a1 0144 0083  .d...|...|...D..
-00001030: 0153 0029 034e 6301 0000 0000 0000 0000  .S.).Nc.........
-00001040: 0000 0002 0000 0004 0000 0053 0000 0073  ...........S...s
-00001050: 1400 0000 6700 7c00 5d06 7d01 7400 7c01  ....g.|.].}.t.|.
-00001060: 8301 9102 7102 5300 7216 0000 0029 0172  ....q.S.r....).r
-00001070: 0300 0000 2902 7244 0000 0072 2300 0000  ....).rD...r#...
-00001080: 7216 0000 0072 1600 0000 7217 0000 0072  r....r....r....r
-00001090: 4600 0000 7c00 0000 7302 0000 0014 007a  F...|...s......z
-000010a0: 2f53 335f 4275 636b 6574 2e6c 6973 745f  /S3_Bucket.list_
-000010b0: 6f62 6a65 6374 5f70 6174 6873 2e3c 6c6f  object_paths.<lo
-000010c0: 6361 6c73 3e2e 3c6c 6973 7463 6f6d 703e  cals>.<listcomp>
-000010d0: 2901 7247 0000 0072 3400 0000 7216 0000  ).rG...r4...r...
-000010e0: 0072 1600 0000 7217 0000 00da 116c 6973  .r....r......lis
-000010f0: 745f 6f62 6a65 6374 5f70 6174 6873 7b00  t_object_paths{.
-00001100: 0000 7237 0000 007a 1b53 335f 4275 636b  ..r7...z.S3_Buck
-00001110: 6574 2e6c 6973 745f 6f62 6a65 6374 5f70  et.list_object_p
-00001120: 6174 6873 da08 6765 745f 636f 7079 da09  aths..get_copy..
-00001130: 636f 7069 6564 5f62 7963 0200 0000 0000  copied_byc......
-00001140: 0000 0000 0000 0200 0000 0500 0000 0300  ................
-00001150: 0000 f312 0000 0074 0064 0174 0183 00a0  .......t.d.t....
-00001160: 027c 01a1 0183 0253 0029 024e 720a 0000  .|.....S.).Nr...
-00001170: 00a9 03da 0463 6173 74da 0573 7570 6572  .....cast..super
-00001180: 7249 0000 00a9 0272 1500 0000 724a 0000  rI.....r....rJ..
-00001190: 00a9 01da 095f 5f63 6c61 7373 5f5f 7216  .....__class__r.
-000011a0: 0000 0072 1700 0000 7249 0000 007e 0000  ...r....rI...~..
-000011b0: 00f3 0200 0000 1201 7a12 5333 5f42 7563  ........z.S3_Buc
-000011c0: 6b65 742e 6765 745f 636f 7079 da0d 5333  ket.get_copy..S3
-000011d0: 5f42 7563 6b65 745f 4b65 7963 0200 0000  _Bucket_Keyc....
-000011e0: 0000 0000 0000 0000 0200 0000 0300 0000  ................
-000011f0: 4300 0000 f30a 0000 007c 00a0 007c 01a1  C........|...|..
-00001200: 0153 0072 1100 0000 a901 da14 5f62 7569  .S.r........_bui
-00001210: 6c64 5f73 335f 6275 636b 6574 5f6b 6579  ld_s3_bucket_key
-00001220: 7234 0000 0072 1600 0000 7216 0000 0072  r4...r....r....r
-00001230: 1700 0000 da0a 6e61 765f 746f 5f6b 6579  ......nav_to_key
-00001240: 8100 0000 f302 0000 000a 017a 1453 335f  ...........z.S3_
-00001250: 4275 636b 6574 2e6e 6176 5f74 6f5f 6b65  Bucket.nav_to_ke
-00001260: 79da 0666 6f6c 6465 72da 1053 335f 4275  y..folder..S3_Bu
-00001270: 636b 6574 5f46 6f6c 6465 7263 0200 0000  cket_Folderc....
-00001280: 0000 0000 0000 0000 0200 0000 0300 0000  ................
-00001290: 4300 0000 7254 0000 0072 1100 0000 a901  C...rT...r......
-000012a0: da17 5f62 7569 6c64 5f73 335f 6275 636b  .._build_s3_buck
-000012b0: 6574 5f66 6f6c 6465 72a9 0272 1500 0000  et_folder..r....
-000012c0: 7259 0000 0072 1600 0000 7216 0000 0072  rY...r....r....r
-000012d0: 1700 0000 da0d 6e61 765f 746f 5f66 6f6c  ......nav_to_fol
-000012e0: 6465 7284 0000 00f3 0200 0000 0a04 7a17  der...........z.
-000012f0: 5333 5f42 7563 6b65 742e 6e61 765f 746f  S3_Bucket.nav_to
-00001300: 5f66 6f6c 6465 7263 0200 0000 0000 0000  _folderc........
-00001310: 0000 0000 0200 0000 0300 0000 4300 0000  ............C...
-00001320: 7254 0000 0072 1100 0000 725b 0000 0072  rT...r....r[...r
-00001330: 5d00 0000 7216 0000 0072 1600 0000 7217  ]...r....r....r.
-00001340: 0000 00da 166e 6176 5f74 6f5f 7265 6c61  .....nav_to_rela
-00001350: 7469 7665 5f66 6f6c 6465 728a 0000 0072  tive_folder....r
-00001360: 5f00 0000 7a20 5333 5f42 7563 6b65 742e  _...z S3_Bucket.
-00001370: 6e61 765f 746f 5f72 656c 6174 6976 655f  nav_to_relative_
-00001380: 666f 6c64 6572 da05 6f74 6865 7263 0200  folder..otherc..
-00001390: 0000 0000 0000 0000 0000 0200 0000 0300  ................
-000013a0: 0000 4300 0000 7254 0000 0072 1100 0000  ..C...rT...r....
-000013b0: 2901 7257 0000 0029 0272 1500 0000 7261  ).rW...).r....ra
-000013c0: 0000 0072 1600 0000 7216 0000 0072 1700  ...r....r....r..
-000013d0: 0000 da0b 5f5f 7472 7565 6469 765f 5f90  ....__truediv__.
-000013e0: 0000 0073 0200 0000 0a03 7a15 5333 5f42  ...s......z.S3_B
-000013f0: 7563 6b65 742e 5f5f 7472 7565 6469 765f  ucket.__truediv_
-00001400: 5f29 0272 5300 0000 725a 0000 0063 0100  _).rS...rZ...c..
-00001410: 0000 0000 0000 0000 0000 0400 0000 0300  ................
-00001420: 0000 4700 0000 731a 0000 007c 007d 027c  ..G...s....|.}.|
-00001430: 0144 005d 067d 037c 027c 031b 007d 0271  .D.].}.|.|...}.q
-00001440: 047c 0253 0072 1100 0000 7216 0000 0029  .|.S.r....r....)
-00001450: 0472 1500 0000 da06 6f74 6865 7273 da08  .r......others..
-00001460: 6e65 775f 7061 7468 7261 0000 0072 1600  new_pathra...r..
-00001470: 0000 7216 0000 0072 1700 0000 da08 6a6f  ..r....r......jo
-00001480: 696e 7061 7468 9600 0000 7308 0000 0004  inpath....s.....
-00001490: 0708 010a 0104 017a 1253 335f 4275 636b  .......z.S3_Buck
-000014a0: 6574 2e6a 6f69 6e70 6174 6863 0200 0000  et.joinpathc....
-000014b0: 0000 0000 0000 0000 0200 0000 0500 0000  ................
-000014c0: 4300 0000 7316 0000 007c 006a 0074 0164  C...s....|.j.t.d
-000014d0: 0168 0174 027c 0183 0164 028d 0353 0029  .h.t.|...d...S.)
-000014e0: 034e da09 6669 6c65 5f6e 616d 6529 02da  .N..file_name)..
-000014f0: 0765 7863 6c75 6465 7259 0000 0029 03da  .excluderY...)..
-00001500: 085f 6661 6374 6f72 7972 5a00 0000 722b  ._factoryrZ...r+
-00001510: 0000 0072 5d00 0000 7216 0000 0072 1600  ...r]...r....r..
-00001520: 0000 7217 0000 0072 5c00 0000 a200 0000  ..r....r\.......
-00001530: 730a 0000 0004 0102 0104 0106 0106 fd7a  s..............z
-00001540: 2153 335f 4275 636b 6574 2e5f 6275 696c  !S3_Bucket._buil
-00001550: 645f 7333 5f62 7563 6b65 745f 666f 6c64  d_s3_bucket_fold
-00001560: 6572 7266 0000 0063 0300 0000 0000 0000  errf...c........
-00001570: 0000 0000 0300 0000 0600 0000 4300 0000  ............C...
-00001580: 733a 0000 007c 0264 0075 0072 0f7c 006a  s:...|.d.u.r.|.j
-00001590: 0074 0164 0168 0174 027c 0183 0164 028d  .t.d.h.t.|...d..
-000015a0: 0353 007c 006a 0074 0164 0168 0174 027c  .S.|.j.t.d.h.t.|
-000015b0: 0283 0174 027c 0183 0164 038d 0453 0029  ...t.|...d...S.)
-000015c0: 044e 7223 0000 0029 0272 6700 0000 7266  .Nr#...).rg...rf
-000015d0: 0000 0029 0372 6700 0000 7259 0000 0072  ...).rg...rY...r
-000015e0: 6600 0000 2903 7268 0000 00da 1553 335f  f...).rh.....S3_
-000015f0: 4275 636b 6574 5f46 6f6c 6465 725f 4669  Bucket_Folder_Fi
-00001600: 6c65 722b 0000 0029 0372 1500 0000 7266  ler+...).r....rf
-00001610: 0000 0072 5900 0000 7216 0000 0072 1600  ...rY...r....r..
-00001620: 0000 7217 0000 00da 1c5f 6275 696c 645f  ..r......_build_
-00001630: 7333 5f62 7563 6b65 745f 666f 6c64 6572  s3_bucket_folder
-00001640: 5f66 696c 65a9 0000 0073 1800 0000 0801  _file....s......
-00001650: 0401 0201 0401 0601 06fd 0406 0201 0401  ................
-00001660: 0601 0601 06fc 7a26 5333 5f42 7563 6b65  ......z&S3_Bucke
-00001670: 742e 5f62 7569 6c64 5f73 335f 6275 636b  t._build_s3_buck
-00001680: 6574 5f66 6f6c 6465 725f 6669 6c65 6302  et_folder_filec.
-00001690: 0000 0000 0000 0000 0000 0002 0000 0005  ................
-000016a0: 0000 0043 0000 0073 1800 0000 7c00 6a00  ...C...s....|.j.
-000016b0: 7401 7402 7c01 8301 6401 6402 6802 6403  t.t.|...d.d.h.d.
-000016c0: 8d03 5300 2904 4e72 5900 0000 7266 0000  ..S.).NrY...rf..
-000016d0: 0029 0272 2300 0000 7267 0000 0029 0372  .).r#...rg...).r
-000016e0: 6800 0000 7253 0000 0072 2b00 0000 7234  h...rS...r+...r4
-000016f0: 0000 0072 1600 0000 7216 0000 0072 1700  ...r....r....r..
-00001700: 0000 7256 0000 00b8 0000 0073 0200 0000  ..rV.......s....
-00001710: 1801 7a1e 5333 5f42 7563 6b65 742e 5f62  ..z.S3_Bucket._b
-00001720: 7569 6c64 5f73 335f 6275 636b 6574 5f6b  uild_s3_bucket_k
-00001730: 6579 2902 720f 0000 0072 1000 0000 a902  ey).r....r......
-00001740: 4e4e a903 4e4e 5472 1100 0000 a901 7249  NN..NNTr......rI
-00001750: 0000 00a9 0272 0f00 0000 7253 0000 0029  .....r....rS...)
-00001760: 28da 085f 5f6e 616d 655f 5fda 0a5f 5f6d  (..__name__..__m
-00001770: 6f64 756c 655f 5fda 0c5f 5f71 7561 6c6e  odule__..__qualn
-00001780: 616d 655f 5f72 2b00 0000 da0f 5f5f 616e  ame__r+.....__an
-00001790: 6e6f 7461 7469 6f6e 735f 5f72 0700 0000  notations__r....
-000017a0: 720e 0000 0072 1800 0000 721a 0000 00da  r....r....r.....
-000017b0: 0c73 7461 7469 636d 6574 686f 6472 0200  .staticmethodr..
-000017c0: 0000 7220 0000 0072 2100 0000 da05 556e  ..r ...r!.....Un
-000017d0: 696f 6e72 0400 0000 7203 0000 00da 084f  ionr....r......O
-000017e0: 7074 696f 6e61 6cda 0464 6963 7472 0600  ptional..dictr..
-000017f0: 0000 722a 0000 00da 0462 6f6f 6c72 3100  ..r*.....boolr1.
-00001800: 0000 7235 0000 0072 3600 0000 723b 0000  ..r5...r6...r;..
-00001810: 00da 0849 7465 7261 626c 6572 4200 0000  ...IterablerB...
-00001820: da04 4c69 7374 7247 0000 0072 4800 0000  ..ListrG...rH...
-00001830: 7249 0000 0072 5700 0000 725e 0000 0072  rI...rW...r^...r
-00001840: 6000 0000 7262 0000 0072 6500 0000 725c  `...rb...re...r\
-00001850: 0000 0072 6a00 0000 7256 0000 00da 0d5f  ...rj...rV....._
-00001860: 5f63 6c61 7373 6365 6c6c 5f5f 7216 0000  _classcell__r...
-00001870: 0072 1600 0000 7250 0000 0072 1700 0000  .r....rP...r....
-00001880: 720a 0000 001d 0000 0073 8200 0000 0a00  r........s......
-00001890: 0801 1202 0a02 0803 0203 0801 1201 0e09  ................
-000018a0: 020e 0201 04fb 0a02 02fe 0a03 02fd 0604  ................
-000018b0: 02fc 0605 0afb 0213 0201 0201 04fa 0a02  ................
-000018c0: 02fe 0a03 02fd 0604 02fc 0605 02fb 0206  ................
-000018d0: 0afa 1a12 1607 1c03 2009 2006 1e04 1803  ........ . .....
-000018e0: 0a03 0203 0a02 02fe 0203 0afd 0206 0a02  ................
-000018f0: 02fe 0203 0afd 0206 0a01 02ff 0202 0afe  ................
-00001900: 0206 0203 0201 02ff 0afd 160c 2407 1e0f  ............$...
-00001910: 720a 0000 0063 0000 0000 0000 0000 0000  r....c..........
-00001920: 0000 0000 0000 0b00 0000 0000 0000 739c  ..............s.
-00001930: 0100 0065 005a 0164 005a 0255 0064 015a  ...e.Z.d.Z.U.d.Z
-00001940: 0365 0465 0564 023c 0065 0664 0283 0164  .e.e.d.<.e.d...d
-00001950: 0364 0484 0083 015a 0764 0564 0684 005a  .d.....Z.d.d...Z
-00001960: 0864 2b64 0865 0464 0964 0066 0487 0066  .d+d.e.d.d.f...f
-00001970: 0164 0a64 0b84 0d5a 0909 0c09 0c64 2c64  .d.d...Z.....d,d
-00001980: 0d65 0a65 0465 0b66 0219 0064 0e65 0a65  .e.e.e.f...d.e.e
-00001990: 0465 0c66 0219 0064 0f65 0d65 0e19 0064  .e.f...d.e.e...d
-000019a0: 1065 0d65 0f19 0066 0887 0066 0164 1164  .e.e...f...f.d.d
-000019b0: 1284 0d5a 1009 0c09 0c09 1364 2d64 0e65  ...Z.......d-d.e
-000019c0: 0a65 0465 0c66 0219 0064 0d65 0a65 0465  .e.e.f...d.e.e.e
-000019d0: 0b66 0219 0064 0f65 0d65 0e19 0064 1065  .f...d.e.e...d.e
-000019e0: 0d65 0f19 0064 1465 1166 0a87 0066 0164  .e...d.e.f...f.d
-000019f0: 1564 1684 0d5a 1264 1765 0a65 0465 0b66  .d...Z.d.e.e.e.f
-00001a00: 0219 0064 0964 0066 0464 1864 1984 045a  ...d.d.f.d.d...Z
-00001a10: 1364 0265 0a65 0465 0b66 0219 0064 0964  .d.e.e.e.f...d.d
-00001a20: 0066 0464 1a64 1b84 045a 1464 1c65 0a65  .f.d.d...Z.d.e.e
-00001a30: 0465 0b66 0219 0064 0964 1d66 0464 1e64  .e.f...d.d.f.d.d
-00001a40: 1f84 045a 1564 2065 0a65 0465 0b66 0219  ...Z.d e.e.e.f..
-00001a50: 0064 0964 2166 0464 2264 2384 045a 1664  .d.d!f.d"d#..Z.d
-00001a60: 2e64 2465 0a65 0465 0c66 0219 0064 0965  .d$e.e.e.f...d.e
-00001a70: 1765 0419 0066 0487 0066 0164 2564 2684  .e...f...f.d%d&.
-00001a80: 0d5a 1864 2e64 2465 0a65 0465 0c66 0219  .Z.d.d$e.e.e.f..
-00001a90: 0064 0965 1765 0c19 0066 0487 0066 0164  .d.e.e...f...f.d
-00001aa0: 2764 2884 0d5a 1964 2e64 2465 0a65 0465  'd(..Z.d.d$e.e.e
-00001ab0: 0c66 0219 0064 0965 1166 0487 0066 0164  .f...d.e.f...f.d
-00001ac0: 2964 2a84 0d5a 1a87 0004 005a 1b53 0029  )d*..Z.....Z.S.)
-00001ad0: 2f72 5a00 0000 7a36 0a20 2020 2020 2020  /rZ...z6.       
-00001ae0: 2052 6570 7265 7365 6e74 7320 6120 666f   Represents a fo
-00001af0: 6c64 6572 2077 6974 6869 6e20 616e 2053  lder within an S
-00001b00: 3320 6275 636b 6574 2e0a 2020 2020 7259  3 bucket..    rY
-00001b10: 0000 0063 0200 0000 0000 0000 0000 0000  ...c............
-00001b20: 0200 0000 0300 0000 4300 0000 f32a 0000  ........C....*..
-00001b30: 0074 007c 0174 0183 0273 0974 017c 0183  .t.|.t...s.t.|..
-00001b40: 017d 0174 027c 0183 0164 016b 0272 1374  .}.t.|...d.k.r.t
-00001b50: 0364 0283 0182 017c 0153 0029 034e 7201  .d.....|.S.).Nr.
-00001b60: 0000 007a 255a 6572 6f20 6c65 6e67 7468  ...z%Zero length
-00001b70: 2073 7472 696e 6720 6e6f 7420 6120 7661   string not a va
-00001b80: 6c69 6420 666f 6c64 6572 a904 da0a 6973  lid folder....is
-00001b90: 696e 7374 616e 6365 722b 0000 00da 036c  instancer+.....l
-00001ba0: 656e da0a 5661 6c75 6545 7272 6f72 a902  en..ValueError..
-00001bb0: da03 636c 73da 0176 7216 0000 0072 1600  ..cls..vr....r..
-00001bc0: 0000 7217 0000 00da 0f76 616c 6964 6174  ..r......validat
-00001bd0: 655f 666f 6c64 6572 c300 0000 f30a 0000  e_folder........
-00001be0: 000a 0308 010c 0108 0104 017a 2053 335f  ...........z S3_
-00001bf0: 4275 636b 6574 5f46 6f6c 6465 722e 7661  Bucket_Folder.va
-00001c00: 6c69 6461 7465 5f66 6f6c 6465 7263 0100  lidate_folderc..
-00001c10: 0000 0000 0000 0000 0000 0100 0000 0400  ................
-00001c20: 0000 4300 0000 f314 0000 0064 017c 006a  ..C........d.|.j
-00001c30: 009b 0064 027c 006a 019b 009d 0453 00a9  ...d.|.j.....S..
-00001c40: 034e 7219 0000 00fa 012f 2902 720b 0000  .Nr....../).r...
-00001c50: 0072 5900 0000 7214 0000 0072 1600 0000  .rY...r....r....
-00001c60: 7216 0000 0072 1700 0000 721a 0000 00cc  r....r....r.....
-00001c70: 0000 0072 3700 0000 7a18 5333 5f42 7563  ...r7...z.S3_Buc
-00001c80: 6b65 745f 466f 6c64 6572 2e5f 5f73 7472  ket_Folder.__str
-00001c90: 5f5f 7249 0000 0072 4a00 0000 720f 0000  __rI...rJ...r...
-00001ca0: 0063 0200 0000 0000 0000 0000 0000 0200  .c..............
-00001cb0: 0000 0500 0000 0300 0000 724b 0000 0029  ..........rK...)
-00001cc0: 024e 725a 0000 0072 4c00 0000 724f 0000  .NrZ...rL...rO..
-00001cd0: 0072 5000 0000 7216 0000 0072 1700 0000  .rP...r....r....
-00001ce0: 7249 0000 00cf 0000 0072 5200 0000 7a19  rI.......rR...z.
-00001cf0: 5333 5f42 7563 6b65 745f 466f 6c64 6572  S3_Bucket_Folder
-00001d00: 2e67 6574 5f63 6f70 794e 7222 0000 00da  .get_copyNr"....
-00001d10: 0a6b 6579 5f73 7566 6669 7872 2400 0000  .key_suffixr$...
-00001d20: 7225 0000 0063 0500 0000 0000 0000 0000  r%...c..........
-00001d30: 0000 0600 0000 0600 0000 0300 0000 7324  ..............s$
-00001d40: 0000 0074 007c 006a 017c 0283 027d 0574  ...t.|.j.|...}.t
-00001d50: 0283 006a 037c 017c 057c 037c 0464 018d  ...j.|.|.|.|.d..
-00001d60: 0401 0064 0053 00a9 024e 2904 7222 0000  ...d.S...N).r"..
-00001d70: 0072 2300 0000 7224 0000 0072 2500 0000  .r#...r$...r%...
-00001d80: 2904 7203 0000 0072 5900 0000 724e 0000  ).r....rY...rN..
-00001d90: 0072 2a00 0000 2906 7215 0000 0072 2200  .r*...).r....r".
-00001da0: 0000 7288 0000 0072 2400 0000 7225 0000  ..r....r$...r%..
-00001db0: 00da 0866 756c 6c5f 6b65 7972 5000 0000  ...full_keyrP...
-00001dc0: 7216 0000 0072 1700 0000 da12 7570 6c6f  r....r......uplo
-00001dd0: 6164 5f66 6f6c 6465 725f 6669 6c65 d200  ad_folder_file..
-00001de0: 0000 730e 0000 000c 0706 0102 0102 0102  ..s.............
-00001df0: 0102 010a fc7a 2353 335f 4275 636b 6574  .....z#S3_Bucket
-00001e00: 5f46 6f6c 6465 722e 7570 6c6f 6164 5f66  _Folder.upload_f
-00001e10: 6f6c 6465 725f 6669 6c65 5472 2c00 0000  older_fileTr,...
-00001e20: 6306 0000 0000 0000 0000 0000 0007 0000  c...............
-00001e30: 0007 0000 0003 0000 0073 2600 0000 7400  .........s&...t.
-00001e40: 7c00 6a01 7c01 8302 7d06 7402 8300 6a03  |.j.|...}.t...j.
-00001e50: 7c06 7c02 7c03 7c04 7c05 6401 8d05 0100  |.|.|.|.|.d.....
-00001e60: 6400 5300 2902 4e29 0572 2300 0000 7222  d.S.).N).r#...r"
-00001e70: 0000 0072 2400 0000 7225 0000 0072 2c00  ...r$...r%...r,.
-00001e80: 0000 2904 7203 0000 0072 5900 0000 724e  ..).r....rY...rN
-00001e90: 0000 0072 3100 0000 2907 7215 0000 0072  ...r1...).r....r
-00001ea0: 8800 0000 7222 0000 0072 2400 0000 7225  ....r"...r$...r%
-00001eb0: 0000 0072 2c00 0000 728a 0000 0072 5000  ...r,...r....rP.
-00001ec0: 0000 7216 0000 0072 1700 0000 da14 646f  ..r....r......do
-00001ed0: 776e 6c6f 6164 5f66 6f6c 6465 725f 6669  wnload_folder_fi
-00001ee0: 6c65 e100 0000 7310 0000 000c 0806 0102  le....s.........
-00001ef0: 0102 0102 0102 0102 010a fb7a 2553 335f  ...........z%S3_
-00001f00: 4275 636b 6574 5f46 6f6c 6465 722e 646f  Bucket_Folder.do
-00001f10: 776e 6c6f 6164 5f66 6f6c 6465 725f 6669  wnload_folder_fi
-00001f20: 6c65 da0a 666f 6c64 6572 5f6b 6579 6302  le..folder_keyc.
-00001f30: 0000 0000 0000 0000 0000 0002 0000 0003  ................
-00001f40: 0000 0043 0000 0072 5400 0000 7211 0000  ...C...rT...r...
-00001f50: 0072 5b00 0000 2902 7215 0000 0072 8d00  .r[...).r....r..
-00001f60: 0000 7216 0000 0072 1600 0000 7217 0000  ..r....r....r...
-00001f70: 0072 5e00 0000 f200 0000 7258 0000 007a  .r^.......rX...z
-00001f80: 1e53 335f 4275 636b 6574 5f46 6f6c 6465  .S3_Bucket_Folde
-00001f90: 722e 6e61 765f 746f 5f66 6f6c 6465 7263  r.nav_to_folderc
-00001fa0: 0200 0000 0000 0000 0000 0000 0300 0000  ................
-00001fb0: 0300 0000 4300 0000 f318 0000 0074 007c  ....C........t.|
-00001fc0: 006a 0183 017c 011b 007d 027c 00a0 027c  .j...|...}.|...|
-00001fd0: 02a1 0153 0072 1100 0000 2903 7203 0000  ...S.r....).r...
-00001fe0: 0072 5900 0000 725e 0000 00a9 0372 1500  .rY...r^.....r..
-00001ff0: 0000 7259 0000 0072 6400 0000 7216 0000  ..rY...rd...r...
-00002000: 0072 1600 0000 7217 0000 0072 6000 0000  .r....r....r`...
-00002010: f500 0000 7304 0000 000e 010a 017a 2753  ....s........z'S
-00002020: 335f 4275 636b 6574 5f46 6f6c 6465 722e  3_Bucket_Folder.
-00002030: 6e61 765f 746f 5f72 656c 6174 6976 655f  nav_to_relative_
-00002040: 666f 6c64 6572 7266 0000 0072 6900 0000  folderrf...ri...
-00002050: 6302 0000 0000 0000 0000 0000 0002 0000  c...............
-00002060: 0003 0000 0043 0000 0072 5400 0000 7211  .....C...rT...r.
-00002070: 0000 0029 0172 6a00 0000 a902 7215 0000  ...).rj.....r...
-00002080: 0072 6600 0000 7216 0000 0072 1600 0000  .rf...r....r....
-00002090: 7217 0000 00da 0b6e 6176 5f74 6f5f 6669  r......nav_to_fi
-000020a0: 6c65 f900 0000 7306 0000 0004 0402 0104  le....s.........
-000020b0: ff7a 1c53 335f 4275 636b 6574 5f46 6f6c  .z.S3_Bucket_Fol
-000020c0: 6465 722e 6e61 765f 746f 5f66 696c 6572  der.nav_to_filer
-000020d0: 6100 0000 7253 0000 0063 0200 0000 0000  a...rS...c......
-000020e0: 0000 0000 0000 0300 0000 0300 0000 4300  ..............C.
-000020f0: 0000 728e 0000 0072 1100 0000 2903 7203  ..r....r....).r.
-00002100: 0000 0072 5900 0000 7257 0000 00a9 0372  ...rY...rW.....r
-00002110: 1500 0000 7261 0000 0072 6400 0000 7216  ....ra...rd...r.
-00002120: 0000 0072 1600 0000 7217 0000 0072 6200  ...r....r....rb.
-00002130: 0000 0101 0000 f304 0000 000e 030a 017a  ...............z
-00002140: 1c53 335f 4275 636b 6574 5f46 6f6c 6465  .S3_Bucket_Folde
-00002150: 722e 5f5f 7472 7565 6469 765f 5f72 2300  r.__truediv__r#.
-00002160: 0000 6302 0000 0000 0000 0000 0000 0002  ..c.............
-00002170: 0000 0003 0000 0003 0000 00f3 1c00 0000  ................
-00002180: 7c01 6400 7500 7207 7c00 6a00 7d01 7401  |.d.u.r.|.j.}.t.
-00002190: 8300 6a02 7c01 6401 8d01 5300 a902 4e72  ..j.|.d...S...Nr
-000021a0: 4300 0000 2903 7259 0000 0072 4e00 0000  C...).rY...rN...
-000021b0: 7247 0000 0072 3400 0000 7250 0000 0072  rG...r4...rP...r
-000021c0: 1600 0000 7217 0000 0072 4700 0000 0701  ....r....rG.....
-000021d0: 0000 f306 0000 0008 0106 010e 017a 2153  .............z!S
-000021e0: 335f 4275 636b 6574 5f46 6f6c 6465 722e  3_Bucket_Folder.
-000021f0: 6c69 7374 5f6f 626a 6563 745f 6b65 7973  list_object_keys
-00002200: 6302 0000 0000 0000 0000 0000 0002 0000  c...............
-00002210: 0003 0000 0003 0000 0072 9400 0000 7295  .........r....r.
-00002220: 0000 0029 0372 5900 0000 724e 0000 0072  ...).rY...rN...r
-00002230: 4800 0000 7234 0000 0072 5000 0000 7216  H...r4...rP...r.
-00002240: 0000 0072 1700 0000 7248 0000 000c 0100  ...r....rH......
-00002250: 0072 9600 0000 7a22 5333 5f42 7563 6b65  .r....z"S3_Bucke
-00002260: 745f 466f 6c64 6572 2e6c 6973 745f 6f62  t_Folder.list_ob
-00002270: 6a65 6374 5f70 6174 6873 6302 0000 0000  ject_pathsc.....
-00002280: 0000 0000 0000 0002 0000 0003 0000 0003  ................
-00002290: 0000 00f3 1a00 0000 7c01 6400 7500 7207  ........|.d.u.r.
-000022a0: 7c00 6a00 7d01 7401 8300 a002 7c01 a101  |.j.}.t.....|...
-000022b0: 5300 7211 0000 0029 0372 5900 0000 724e  S.r....).rY...rN
-000022c0: 0000 0072 3500 0000 7234 0000 0072 5000  ...r5...r4...rP.
-000022d0: 0000 7216 0000 0072 1700 0000 7235 0000  ..r....r....r5..
-000022e0: 0011 0100 00f3 0600 0000 0801 0601 0c01  ................
-000022f0: 7a1b 5333 5f42 7563 6b65 745f 466f 6c64  z.S3_Bucket_Fold
-00002300: 6572 2e6b 6579 5f65 7869 7374 7372 6d00  er.key_existsrm.
-00002310: 0000 726b 0000 0072 6c00 0000 7211 0000  ..rk...rl...r...
-00002320: 0029 1c72 6f00 0000 7270 0000 0072 7100  .).ro...rp...rq.
-00002330: 0000 da07 5f5f 646f 635f 5f72 2b00 0000  ....__doc__r+...
-00002340: 7272 0000 0072 0800 0000 7283 0000 0072  rr...r....r....r
-00002350: 1a00 0000 7249 0000 0072 7400 0000 7204  ....rI...rt...r.
-00002360: 0000 0072 0300 0000 7275 0000 0072 7600  ...r....ru...rv.
-00002370: 0000 7206 0000 0072 8b00 0000 7277 0000  ..r....r....rw..
-00002380: 0072 8c00 0000 725e 0000 0072 6000 0000  .r....r^...r`...
-00002390: 7291 0000 0072 6200 0000 7279 0000 0072  r....rb...ry...r
-000023a0: 4700 0000 7248 0000 0072 3500 0000 727a  G...rH...r5...rz
-000023b0: 0000 0072 1600 0000 7216 0000 0072 5000  ...r....r....rP.
-000023c0: 0000 7217 0000 0072 5a00 0000 bc00 0000  ..r....rZ.......
-000023d0: 735e 0000 000a 0004 0108 0306 030a 0108  s^..............
-000023e0: 0818 0302 0702 0104 fb0a 0202 fe0a 0302  ................
-000023f0: fd06 0402 fc06 050e fb02 1302 0102 0104  ................
-00002400: fa0a 0202 fe0a 0302 fd06 0402 fc06 0502  ................
-00002410: fb02 060e fa1a 111a 0302 040a 0202 fe02  ................
-00002420: 030a fd02 080a 0102 ff02 020a fe24 0624  .............$.$
-00002430: 0528 0572 5a00 0000 6300 0000 0000 0000  .(.rZ...c.......
-00002440: 0000 0000 0000 0000 0008 0000 0000 0000  ................
-00002450: 0073 e400 0000 6500 5a01 6400 5a02 5500  .s....e.Z.d.Z.U.
-00002460: 6401 5a03 6504 6505 6402 3c00 6506 6402  d.Z.e.e.d.<.e.d.
-00002470: 8301 6403 6404 8400 8301 5a07 6405 6406  ..d.d.....Z.d.d.
-00002480: 8400 5a08 641b 6408 6504 6409 6400 6604  ..Z.d.d.e.d.d.f.
-00002490: 8700 6601 640a 640b 840d 5a09 090c 090c  ..f.d.d...Z.....
-000024a0: 641c 640d 650a 6504 650b 6602 1900 640e  d.d.e.e.e.f...d.
-000024b0: 650c 650d 1900 640f 650c 650e 1900 6606  e.e...d.e.e...f.
-000024c0: 8700 6601 6410 6411 840d 5a0f 090c 090c  ..f.d.d...Z.....
-000024d0: 641c 640d 650a 6504 650b 6602 1900 640e  d.d.e.e.e.f...d.
-000024e0: 650c 650d 1900 640f 650c 650e 1900 6606  e.e...d.e.e...f.
-000024f0: 8700 6601 6412 6413 840d 5a10 641d 6414  ..f.d.d...Z.d.d.
-00002500: 650a 6504 650b 6602 1900 6602 8700 6601  e.e.e.f...f...f.
-00002510: 6415 6416 840d 5a11 6417 650a 6504 6512  d.d...Z.d.e.e.e.
-00002520: 6602 1900 6409 6418 6604 6419 641a 8404  f...d.d.f.d.d...
-00002530: 5a13 8700 0400 5a14 5300 291e 7269 0000  Z.....Z.S.).ri..
-00002540: 007a 9a0a 2020 2020 2020 2020 5265 7072  .z..        Repr
-00002550: 6573 656e 7473 2061 2075 6e69 7175 6520  esents a unique 
-00002560: 666f 6c64 6572 2026 2066 696c 6520 7769  folder & file wi
-00002570: 7468 696e 2061 6e20 5333 2062 7563 6b65  thin an S3 bucke
-00002580: 742e 0a20 2020 2020 2020 2053 696d 696c  t..        Simil
-00002590: 6172 2074 6f20 5333 5f42 7563 6b65 745f  ar to S3_Bucket_
-000025a0: 4b65 7920 6275 7420 7573 6573 2066 6f6c  Key but uses fol
-000025b0: 6465 7220 2b20 6669 6c65 5f6e 616d 6520  der + file_name 
-000025c0: 696e 7374 6561 6420 6f66 2061 2073 696e  instead of a sin
-000025d0: 676c 6520 6b65 792e 0a20 2020 2072 6600  gle key..    rf.
-000025e0: 0000 6302 0000 0000 0000 0000 0000 0002  ..c.............
-000025f0: 0000 0003 0000 0043 0000 0072 7b00 0000  .......C...r{...
-00002600: 2903 4e72 0100 0000 7a28 5a65 726f 206c  ).Nr....z(Zero l
-00002610: 656e 6774 6820 7374 7269 6e67 206e 6f74  ength string not
-00002620: 2061 2076 616c 6964 2066 696c 655f 6e61   a valid file_na
-00002630: 6d65 727c 0000 0072 8000 0000 7216 0000  mer|...r....r...
-00002640: 0072 1600 0000 7217 0000 00da 1276 616c  .r....r......val
-00002650: 6964 6174 655f 6669 6c65 5f6e 616d 651f  idate_file_name.
-00002660: 0100 0072 8400 0000 7a28 5333 5f42 7563  ...r....z(S3_Buc
-00002670: 6b65 745f 466f 6c64 6572 5f46 696c 652e  ket_Folder_File.
-00002680: 7661 6c69 6461 7465 5f66 696c 655f 6e61  validate_file_na
-00002690: 6d65 6301 0000 0000 0000 0000 0000 0001  mec.............
-000026a0: 0000 0006 0000 0043 0000 0073 1c00 0000  .......C...s....
-000026b0: 6401 7c00 6a00 9b00 6402 7c00 6a01 9b00  d.|.j...d.|.j...
-000026c0: 6402 7c00 6a02 9b00 9d06 5300 7286 0000  d.|.j.....S.r...
-000026d0: 0029 0372 0b00 0000 7259 0000 0072 6600  .).r....rY...rf.
-000026e0: 0000 7214 0000 0072 1600 0000 7216 0000  ..r....r....r...
-000026f0: 0072 1700 0000 721a 0000 0028 0100 0073  .r....r....(...s
-00002700: 0200 0000 1c01 7a1d 5333 5f42 7563 6b65  ......z.S3_Bucke
-00002710: 745f 466f 6c64 6572 5f46 696c 652e 5f5f  t_Folder_File.__
-00002720: 7374 725f 5f72 4900 0000 724a 0000 0072  str__rI...rJ...r
-00002730: 0f00 0000 6302 0000 0000 0000 0000 0000  ....c...........
-00002740: 0002 0000 0005 0000 0003 0000 0072 4b00  .............rK.
-00002750: 0000 2902 4e72 6900 0000 724c 0000 0072  ..).Nri...rL...r
-00002760: 4f00 0000 7250 0000 0072 1600 0000 7217  O...rP...r....r.
-00002770: 0000 0072 4900 0000 2b01 0000 7252 0000  ...rI...+...rR..
-00002780: 007a 1e53 335f 4275 636b 6574 5f46 6f6c  .z.S3_Bucket_Fol
-00002790: 6465 725f 4669 6c65 2e67 6574 5f63 6f70  der_File.get_cop
-000027a0: 794e 7222 0000 0072 2400 0000 7225 0000  yNr"...r$...r%..
-000027b0: 0063 0400 0000 0000 0000 0000 0000 0400  .c..............
-000027c0: 0000 0600 0000 0300 0000 f31a 0000 0074  ...............t
-000027d0: 0083 006a 017c 017c 006a 027c 027c 0364  ...j.|.|.j.|.|.d
-000027e0: 018d 0401 0064 0053 00a9 024e 2904 7222  .....d.S...N).r"
-000027f0: 0000 0072 8800 0000 7224 0000 0072 2500  ...r....r$...r%.
-00002800: 0000 2903 724e 0000 0072 8b00 0000 7266  ..).rN...r....rf
-00002810: 0000 00a9 0472 1500 0000 7222 0000 0072  .....r....r"...r
-00002820: 2400 0000 7225 0000 0072 5000 0000 7216  $...r%...rP...r.
-00002830: 0000 0072 1700 0000 da15 7570 6c6f 6164  ...r......upload
-00002840: 5f73 7065 6369 6669 6564 5f66 696c 652e  _specified_file.
-00002850: 0100 00f3 0c00 0000 0606 0201 0401 0201  ................
-00002860: 0201 0afc 7a2b 5333 5f42 7563 6b65 745f  ....z+S3_Bucket_
-00002870: 466f 6c64 6572 5f46 696c 652e 7570 6c6f  Folder_File.uplo
-00002880: 6164 5f73 7065 6369 6669 6564 5f66 696c  ad_specified_fil
-00002890: 6563 0400 0000 0000 0000 0000 0000 0400  ec..............
-000028a0: 0000 0600 0000 0300 0000 729b 0000 0072  ..........r....r
-000028b0: 9c00 0000 2903 724e 0000 0072 8c00 0000  ....).rN...r....
-000028c0: 7266 0000 0072 9d00 0000 7250 0000 0072  rf...r....rP...r
-000028d0: 1600 0000 7217 0000 00da 1764 6f77 6e6c  ....r......downl
-000028e0: 6f61 645f 7370 6563 6966 6965 645f 6669  oad_specified_fi
-000028f0: 6c65 3b01 0000 729f 0000 007a 2d53 335f  le;...r....z-S3_
-00002900: 4275 636b 6574 5f46 6f6c 6465 725f 4669  Bucket_Folder_Fi
-00002910: 6c65 2e64 6f77 6e6c 6f61 645f 7370 6563  le.download_spec
-00002920: 6966 6965 645f 6669 6c65 7223 0000 0063  ified_filer#...c
-00002930: 0200 0000 0000 0000 0000 0000 0200 0000  ................
-00002940: 0300 0000 0300 0000 7328 0000 007c 0164  ........s(...|.d
-00002950: 0075 0072 0d7c 006a 009b 0064 017c 006a  .u.r.|.j...d.|.j
-00002960: 019b 009d 037d 0174 0283 006a 037c 0164  .....}.t...j.|.d
-00002970: 028d 0153 0029 034e 7287 0000 0072 4300  ...S.).Nr....rC.
-00002980: 0000 2904 7259 0000 0072 6600 0000 724e  ..).rY...rf...rN
-00002990: 0000 0072 3600 0000 7234 0000 0072 5000  ...r6...r4...rP.
-000029a0: 0000 7216 0000 0072 1700 0000 7236 0000  ..r....r....r6..
-000029b0: 0048 0100 0073 0600 0000 0801 1201 0e01  .H...s..........
-000029c0: 7a20 5333 5f42 7563 6b65 745f 466f 6c64  z S3_Bucket_Fold
-000029d0: 6572 5f46 696c 652e 6765 745f 6f62 6a65  er_File.get_obje
-000029e0: 6374 7261 0000 0072 5300 0000 6302 0000  ctra...rS...c...
-000029f0: 0000 0000 0000 0000 0003 0000 0003 0000  ................
-00002a00: 0043 0000 0073 1e00 0000 7400 7c00 6a01  .C...s....t.|.j.
-00002a10: 8301 7c00 6a02 1b00 7c01 1b00 7d02 7c00  ..|.j...|...}.|.
-00002a20: a003 7c02 a101 5300 7211 0000 0029 0472  ..|...S.r....).r
-00002a30: 0300 0000 7259 0000 0072 6600 0000 7257  ....rY...rf...rW
-00002a40: 0000 0072 9200 0000 7216 0000 0072 1600  ...r....r....r..
-00002a50: 0000 7217 0000 0072 6200 0000 4d01 0000  ..r....rb...M...
-00002a60: 7304 0000 0014 040a 017a 2153 335f 4275  s........z!S3_Bu
-00002a70: 636b 6574 5f46 6f6c 6465 725f 4669 6c65  cket_Folder_File
-00002a80: 2e5f 5f74 7275 6564 6976 5f5f 726d 0000  .__truediv__rm..
-00002a90: 0072 6b00 0000 7211 0000 0029 1572 6f00  .rk...r....).ro.
-00002aa0: 0000 7270 0000 0072 7100 0000 7299 0000  ..rp...rq...r...
-00002ab0: 0072 2b00 0000 7272 0000 0072 0800 0000  .r+...rr...r....
-00002ac0: 729a 0000 0072 1a00 0000 7249 0000 0072  r....r....rI...r
-00002ad0: 7400 0000 7203 0000 0072 7500 0000 7276  t...r....ru...rv
-00002ae0: 0000 0072 0600 0000 729e 0000 0072 a000  ...r....r....r..
-00002af0: 0000 7236 0000 0072 0400 0000 7262 0000  ..r6...r....rb..
-00002b00: 0072 7a00 0000 7216 0000 0072 1600 0000  .rz...r....r....
-00002b10: 7250 0000 0072 1700 0000 7269 0000 0017  rP...r....ri....
-00002b20: 0100 0073 3e00 0000 0a00 0401 0804 0603  ...s>...........
-00002b30: 0a01 0808 1803 0206 0201 04fc 0a02 02fe  ................
-00002b40: 0603 02fd 0604 0efc 0210 0201 04fc 0a02  ................
-00002b50: 02fe 0603 02fd 0604 0efc 1c0d 0205 0a01  ................
-00002b60: 02ff 0202 12fe 7269 0000 0063 0000 0000  ......ri...c....
-00002b70: 0000 0000 0000 0000 0000 0000 0900 0000  ................
-00002b80: 0000 0000 73ae 0100 0065 005a 0164 005a  ....s....e.Z.d.Z
-00002b90: 0255 0064 015a 0365 0465 0564 023c 0065  .U.d.Z.e.e.d.<.e
-00002ba0: 0664 0283 0164 0364 0484 0083 015a 0764  .d...d.d.....Z.d
-00002bb0: 0564 0684 005a 0864 2e64 0865 0464 0964  .d...Z.d.d.e.d.d
-00002bc0: 0066 0487 0066 0164 0a64 0b84 0d5a 0964  .f...f.d.d...Z.d
-00002bd0: 2f64 0c64 0d84 045a 0a09 0e09 0e64 3064  /d.d...Z.....d0d
-00002be0: 0f65 0b65 0465 0c66 0219 0064 1065 0d65  .e.e.e.f...d.e.e
-00002bf0: 0e19 0064 1165 0d65 0f19 0066 0687 0066  ...d.e.e...f...f
-00002c00: 0164 1264 1384 0d5a 1009 0e09 0e09 1464  .d.d...Z.......d
-00002c10: 3164 0f65 0b65 0465 0c66 0219 0064 1065  1d.e.e.e.f...d.e
-00002c20: 0d65 0e19 0064 1165 0d65 0f19 0064 1565  .e...d.e.e...d.e
-00002c30: 1166 0887 0066 0164 1664 1784 0d5a 1264  .f...f.d.d...Z.d
-00002c40: 3064 0265 0b65 0465 0c66 0219 0066 0287  0d.e.e.e.f...f..
-00002c50: 0066 0164 1864 1984 0d5a 1364 3264 0265  .f.d.d...Z.d2d.e
-00002c60: 0b65 0465 0c66 0219 0064 0965 1465 0419  .e.e.f...d.e.e..
-00002c70: 0066 0487 0066 0164 1a64 1b84 0d5a 1564  .f...f.d.d...Z.d
-00002c80: 3264 0265 0b65 0465 0c66 0219 0064 0965  2d.e.e.e.f...d.e
-00002c90: 1465 0c19 0066 0487 0066 0164 1c64 1d84  .e...f...f.d.d..
-00002ca0: 0d5a 1664 3264 0265 0b65 0465 0c66 0219  .Z.d2d.e.e.e.f..
-00002cb0: 0064 0965 1764 1e19 0066 0487 0066 0164  .d.e.d...f...f.d
-00002cc0: 1f64 2084 0d5a 1864 2165 0b65 0465 1966  .d ..Z.d!e.e.e.f
-00002cd0: 0219 0064 0964 2266 0464 2364 2484 045a  ...d.d"f.d#d$..Z
-00002ce0: 1a64 2165 0b65 0465 1966 0219 0064 0964  .d!e.e.e.f...d.d
-00002cf0: 2266 0464 2564 2684 045a 1b64 2765 0b65  "f.d%d&..Z.d'e.e
-00002d00: 0465 1966 0219 0064 0964 2866 0464 2964  .e.f...d.d(f.d)d
-00002d10: 2a84 045a 1c64 2b65 0b65 0465 1966 0219  *..Z.d+e.e.e.f..
-00002d20: 0064 0964 0066 0464 2c64 2d84 045a 1d87  .d.d.f.d,d-..Z..
-00002d30: 0004 005a 1e53 0029 3372 5300 0000 7a96  ...Z.S.)3rS...z.
-00002d40: 0a20 2020 2052 6570 7265 7365 6e74 7320  .    Represents 
-00002d50: 6120 756e 6971 7565 2066 696c 6520 286b  a unique file (k
-00002d60: 6579 2920 7769 7468 696e 2061 6e20 5333  ey) within an S3
-00002d70: 2062 7563 6b65 742e 0a20 2020 2053 696d   bucket..    Sim
-00002d80: 696c 6172 2074 6f20 5333 5f42 7563 6b65  ilar to S3_Bucke
-00002d90: 745f 466f 6c64 6572 5f46 696c 6520 6275  t_Folder_File bu
-00002da0: 7420 7573 6573 2061 2073 696e 676c 6520  t uses a single 
-00002db0: 6b65 7920 696e 7374 6561 6420 6f66 2066  key instead of f
-00002dc0: 6f6c 6465 7220 2b20 6669 6c65 5f6e 616d  older + file_nam
-00002dd0: 650a 2020 2020 7223 0000 0063 0200 0000  e.    r#...c....
-00002de0: 0000 0000 0000 0000 0200 0000 0300 0000  ................
-00002df0: 4300 0000 727b 0000 0029 034e 7201 0000  C...r{...).Nr...
-00002e00: 007a 225a 6572 6f20 6c65 6e67 7468 2073  .z"Zero length s
-00002e10: 7472 696e 6720 6e6f 7420 6120 7661 6c69  tring not a vali
-00002e20: 6420 6b65 7972 7c00 0000 7280 0000 0072  d keyr|...r....r
-00002e30: 1600 0000 7216 0000 0072 1700 0000 da0c  ....r....r......
-00002e40: 7661 6c69 6461 7465 5f6b 6579 5d01 0000  validate_key]...
-00002e50: 7284 0000 007a 1a53 335f 4275 636b 6574  r....z.S3_Bucket
-00002e60: 5f4b 6579 2e76 616c 6964 6174 655f 6b65  _Key.validate_ke
-00002e70: 7963 0100 0000 0000 0000 0000 0000 0100  yc..............
-00002e80: 0000 0400 0000 4300 0000 7285 0000 0072  ......C...r....r
-00002e90: 8600 0000 2902 720b 0000 0072 2300 0000  ....).r....r#...
-00002ea0: 7214 0000 0072 1600 0000 7216 0000 0072  r....r....r....r
-00002eb0: 1700 0000 721a 0000 0066 0100 0072 3700  ....r....f...r7.
-00002ec0: 0000 7a15 5333 5f42 7563 6b65 745f 4b65  ..z.S3_Bucket_Ke
-00002ed0: 792e 5f5f 7374 725f 5f72 4900 0000 724a  y.__str__rI...rJ
-00002ee0: 0000 0072 0f00 0000 6302 0000 0000 0000  ...r....c.......
-00002ef0: 0000 0000 0002 0000 0005 0000 0003 0000  ................
-00002f00: 0072 4b00 0000 2902 4e72 5300 0000 724c  .rK...).NrS...rL
-00002f10: 0000 0072 4f00 0000 7250 0000 0072 1600  ...rO...rP...r..
-00002f20: 0000 7217 0000 0072 4900 0000 6901 0000  ..r....rI...i...
-00002f30: 7252 0000 007a 1653 335f 4275 636b 6574  rR...z.S3_Bucket
-00002f40: 5f4b 6579 2e67 6574 5f63 6f70 7963 0200  _Key.get_copyc..
-00002f50: 0000 0000 0000 0000 0000 0200 0000 0300  ................
-00002f60: 0000 4300 0000 7254 0000 0072 1100 0000  ..C...rT...r....
-00002f70: 7255 0000 0072 3400 0000 7216 0000 0072  rU...r4...r....r
-00002f80: 1600 0000 7217 0000 0072 5700 0000 6c01  ....r....rW...l.
-00002f90: 0000 7258 0000 007a 1853 335f 4275 636b  ..rX...z.S3_Buck
-00002fa0: 6574 5f4b 6579 2e6e 6176 5f74 6f5f 6b65  et_Key.nav_to_ke
-00002fb0: 794e 7222 0000 0072 2400 0000 7225 0000  yNr"...r$...r%..
-00002fc0: 0063 0400 0000 0000 0000 0000 0000 0400  .c..............
-00002fd0: 0000 0600 0000 0300 0000 729b 0000 0072  ..........r....r
-00002fe0: 8900 0000 2903 724e 0000 0072 2a00 0000  ....).rN...r*...
-00002ff0: 7223 0000 0072 9d00 0000 7250 0000 0072  r#...r....rP...r
-00003000: 1600 0000 7217 0000 0072 9e00 0000 6f01  ....r....r....o.
-00003010: 0000 729f 0000 007a 2353 335f 4275 636b  ..r....z#S3_Buck
-00003020: 6574 5f4b 6579 2e75 706c 6f61 645f 7370  et_Key.upload_sp
-00003030: 6563 6966 6965 645f 6669 6c65 5472 2c00  ecified_fileTr,.
-00003040: 0000 6305 0000 0000 0000 0000 0000 0005  ..c.............
-00003050: 0000 0007 0000 0003 0000 0073 1c00 0000  ...........s....
-00003060: 7400 8300 6a01 7c01 7c00 6a02 7c02 7c03  t...j.|.|.j.|.|.
-00003070: 7c04 6401 8d05 0100 6400 5300 2902 4e29  |.d.....d.S.).N)
-00003080: 0572 2200 0000 7223 0000 0072 2400 0000  .r"...r#...r$...
-00003090: 7225 0000 0072 2c00 0000 2903 724e 0000  r%...r,...).rN..
-000030a0: 0072 3100 0000 7223 0000 0029 0572 1500  .r1...r#...).r..
-000030b0: 0000 7222 0000 0072 2400 0000 7225 0000  ..r"...r$...r%..
-000030c0: 0072 2c00 0000 7250 0000 0072 1600 0000  .r,...rP...r....
-000030d0: 7217 0000 0072 a000 0000 7c01 0000 730e  r....r....|...s.
-000030e0: 0000 0006 0702 0104 0102 0102 0102 010a  ................
-000030f0: fb7a 2553 335f 4275 636b 6574 5f4b 6579  .z%S3_Bucket_Key
-00003100: 2e64 6f77 6e6c 6f61 645f 7370 6563 6966  .download_specif
-00003110: 6965 645f 6669 6c65 6303 0000 0000 0000  ied_filec.......
-00003120: 0000 0000 0003 0000 0003 0000 0003 0000  ................
-00003130: 0072 9400 0000 7295 0000 0029 0372 2300  .r....r....).r#.
-00003140: 0000 724e 0000 0072 3600 0000 2903 7215  ..rN...r6...).r.
-00003150: 0000 0072 2300 0000 7238 0000 0072 5000  ...r#...r8...rP.
-00003160: 0000 7216 0000 0072 1700 0000 7236 0000  ..r....r....r6..
-00003170: 008b 0100 0072 9600 0000 7a18 5333 5f42  .....r....z.S3_B
-00003180: 7563 6b65 745f 4b65 792e 6765 745f 6f62  ucket_Key.get_ob
-00003190: 6a65 6374 6302 0000 0000 0000 0000 0000  jectc...........
-000031a0: 0002 0000 0003 0000 0003 0000 0072 9400  .............r..
-000031b0: 0000 7295 0000 0029 0372 2300 0000 724e  ..r....).r#...rN
-000031c0: 0000 0072 4700 0000 7234 0000 0072 5000  ...rG...r4...rP.
-000031d0: 0000 7216 0000 0072 1700 0000 7247 0000  ..r....r....rG..
-000031e0: 0090 0100 0072 9600 0000 7a1e 5333 5f42  .....r....z.S3_B
-000031f0: 7563 6b65 745f 4b65 792e 6c69 7374 5f6f  ucket_Key.list_o
-00003200: 626a 6563 745f 6b65 7973 6302 0000 0000  bject_keysc.....
-00003210: 0000 0000 0000 0002 0000 0003 0000 0003  ................
-00003220: 0000 0072 9400 0000 7295 0000 0029 0372  ...r....r....).r
-00003230: 2300 0000 724e 0000 0072 4800 0000 7234  #...rN...rH...r4
-00003240: 0000 0072 5000 0000 7216 0000 0072 1700  ...rP...r....r..
-00003250: 0000 7248 0000 0095 0100 0072 9600 0000  ..rH.......r....
-00003260: 7a1f 5333 5f42 7563 6b65 745f 4b65 792e  z.S3_Bucket_Key.
-00003270: 6c69 7374 5f6f 626a 6563 745f 7061 7468  list_object_path
-00003280: 7372 3c00 0000 6302 0000 0000 0000 0000  sr<...c.........
-00003290: 0000 0002 0000 0003 0000 0003 0000 0072  ...............r
-000032a0: 9700 0000 7211 0000 0029 0372 2300 0000  ....r....).r#...
-000032b0: 724e 0000 0072 4200 0000 7234 0000 0072  rN...rB...r4...r
-000032c0: 5000 0000 7216 0000 0072 1700 0000 7242  P...r....r....rB
-000032d0: 0000 009a 0100 0072 9800 0000 7a1a 5333  .......r....z.S3
-000032e0: 5f42 7563 6b65 745f 4b65 792e 6669 6e64  _Bucket_Key.find
-000032f0: 5f6f 626a 6563 7473 7259 0000 0072 5a00  _objectsrY...rZ.
-00003300: 0000 6302 0000 0000 0000 0000 0000 0002  ..c.............
-00003310: 0000 0003 0000 0043 0000 0072 5400 0000  .......C...rT...
-00003320: 7211 0000 0072 5b00 0000 725d 0000 0072  r....r[...r]...r
-00003330: 1600 0000 7216 0000 0072 1700 0000 725e  ....r....r....r^
-00003340: 0000 009f 0100 0072 5f00 0000 7a1b 5333  .......r_...z.S3
-00003350: 5f42 7563 6b65 745f 4b65 792e 6e61 765f  _Bucket_Key.nav_
-00003360: 746f 5f66 6f6c 6465 7263 0200 0000 0000  to_folderc......
-00003370: 0000 0000 0000 0300 0000 0300 0000 4300  ..............C.
-00003380: 0000 728e 0000 0072 1100 0000 2903 7203  ..r....r....).r.
-00003390: 0000 0072 2300 0000 725e 0000 0072 8f00  ...r#...r^...r..
-000033a0: 0000 7216 0000 0072 1600 0000 7217 0000  ..r....r....r...
-000033b0: 0072 6000 0000 a501 0000 7304 0000 000e  .r`.......s.....
-000033c0: 040a 017a 2453 335f 4275 636b 6574 5f4b  ...z$S3_Bucket_K
-000033d0: 6579 2e6e 6176 5f74 6f5f 7265 6c61 7469  ey.nav_to_relati
-000033e0: 7665 5f66 6f6c 6465 7272 6600 0000 7269  ve_folderrf...ri
-000033f0: 0000 0063 0200 0000 0000 0000 0000 0000  ...c............
-00003400: 0200 0000 0400 0000 4300 0000 7310 0000  ........C...s...
-00003410: 007c 006a 007c 006a 017c 0164 018d 0253  .|.j.|.j.|.d...S
-00003420: 0029 024e 2902 7259 0000 0072 6600 0000  .).N).rY...rf...
-00003430: 2902 726a 0000 0072 2300 0000 7290 0000  ).rj...r#...r...
-00003440: 0072 1600 0000 7216 0000 0072 1700 0000  .r....r....r....
-00003450: 7291 0000 00ac 0100 0073 0800 0000 0404  r........s......
-00003460: 0401 0201 06fe 7a19 5333 5f42 7563 6b65  ......z.S3_Bucke
-00003470: 745f 4b65 792e 6e61 765f 746f 5f66 696c  t_Key.nav_to_fil
-00003480: 6572 6100 0000 6302 0000 0000 0000 0000  era...c.........
-00003490: 0000 0003 0000 0003 0000 0043 0000 0072  ...........C...r
-000034a0: 8e00 0000 7211 0000 0029 0372 0300 0000  ....r....).r....
-000034b0: 7223 0000 0072 5700 0000 7292 0000 0072  r#...rW...r....r
-000034c0: 1600 0000 7216 0000 0072 1700 0000 7262  ....r....r....rb
-000034d0: 0000 00b5 0100 0072 9300 0000 7a19 5333  .......r....z.S3
-000034e0: 5f42 7563 6b65 745f 4b65 792e 5f5f 7472  _Bucket_Key.__tr
-000034f0: 7565 6469 765f 5f72 6d00 0000 726e 0000  uediv__rm...rn..
-00003500: 0072 6b00 0000 726c 0000 0072 1100 0000  .rk...rl...r....
-00003510: 291f 726f 0000 0072 7000 0000 7271 0000  ).ro...rp...rq..
-00003520: 0072 9900 0000 722b 0000 0072 7200 0000  .r....r+...rr...
-00003530: 7208 0000 0072 a100 0000 721a 0000 0072  r....r....r....r
-00003540: 4900 0000 7257 0000 0072 7400 0000 7203  I...rW...rt...r.
-00003550: 0000 0072 7500 0000 7276 0000 0072 0600  ...ru...rv...r..
-00003560: 0000 729e 0000 0072 7700 0000 72a0 0000  ..r....rw...r...
-00003570: 0072 3600 0000 7279 0000 0072 4700 0000  .r6...ry...rG...
-00003580: 7248 0000 0072 7800 0000 7242 0000 0072  rH...rx...rB...r
-00003590: 0400 0000 725e 0000 0072 6000 0000 7291  ....r^...r`...r.
-000035a0: 0000 0072 6200 0000 727a 0000 0072 1600  ...rb...rz...r..
-000035b0: 0000 7216 0000 0072 5000 0000 7217 0000  ..r....rP...r...
-000035c0: 0072 5300 0000 5501 0000 736a 0000 000a  .rS...U...sj....
-000035d0: 0004 0108 0406 030a 0108 0818 030a 0302  ................
-000035e0: 0602 0104 fc0a 0202 fe06 0302 fd06 040e  ................
-000035f0: fc02 1002 0102 0104 fb0a 0202 fe06 0302  ................
-00003600: fd06 0402 fc02 050e fb1c 0f24 0524 0524  ...........$.$.$
-00003610: 0502 050a 0202 fe02 030a fd02 060a 0202  ................
-00003620: fe02 030a fd02 070a 0202 fe02 030a fd02  ................
-00003630: 090a 0102 ff02 0212 fe72 5300 0000 2915  .........rS...).
-00003640: da09 6675 6e63 746f 6f6c 7372 0200 0000  ..functoolsr....
-00003650: da07 7061 7468 6c69 6272 0300 0000 7204  ..pathlibr....r.
-00003660: 0000 00da 0674 7970 696e 675a 1162 6f74  .....typingZ.bot
-00003670: 6f33 2e73 332e 7472 616e 7366 6572 7206  o3.s3.transferr.
-00003680: 0000 00da 0870 7964 616e 7469 6372 0700  .....pydanticr..
-00003690: 0000 7208 0000 005a 3063 6f6e 6669 675f  ..r....Z0config_
-000036a0: 7772 616e 676c 6572 2e63 6f6e 6669 675f  wrangler.config_
-000036b0: 7465 6d70 6c61 7465 732e 6177 732e 6177  templates.aws.aw
-000036c0: 735f 7365 7373 696f 6e72 0900 0000 da05  s_sessionr......
-000036d0: 626f 746f 33da 0b49 6d70 6f72 7445 7272  boto3..ImportErr
-000036e0: 6f72 da0d 5459 5045 5f43 4845 434b 494e  or..TYPE_CHECKIN
-000036f0: 475a 0962 6f74 6f73 7475 6273 720a 0000  GZ.botostubsr...
-00003700: 0072 5a00 0000 7269 0000 0072 5300 0000  .rZ...ri...rS...
-00003710: 7216 0000 0072 1600 0000 7216 0000 0072  r....r....r....r
-00003720: 1700 0000 da08 3c6d 6f64 756c 653e 0100  ......<module>..
-00003730: 0000 732c 0000 000c 0010 0108 010c 0210  ..s,............
-00003740: 010c 0202 020c 010c 0108 0102 ff04 0302  ................
-00003750: 010c 010c 0108 0102 ff10 0b00 7f10 2010  .............. .
-00003760: 5b14 3e                                  [.>
+00000930: 7336 0000 007c 0464 0075 0072 0974 0064  s6...|.d.u.r.t.d
+00000940: 0164 028d 017d 047c 006a 016a 0274 037c  .d...}.|.j.j.t.|
+00000950: 0183 017c 006a 0474 037c 0283 017c 037c  ...|.j.t.|...|.|
+00000960: 0464 038d 0501 0064 0053 0029 044e 6c03  .d.....d.S.).Nl.
+00000970: 0000 0000 0000 0005 0029 015a 136d 756c  .........).Z.mul
+00000980: 7469 7061 7274 5f74 6872 6573 686f 6c64  tipart_threshold
+00000990: 2905 da08 4669 6c65 6e61 6d65 7213 0000  )...Filenamer...
+000009a0: 00da 034b 6579 da09 4578 7472 6141 7267  ...Key..ExtraArg
+000009b0: 73da 0643 6f6e 6669 6729 0572 0600 0000  s..Config).r....
+000009c0: 721e 0000 00da 0b75 706c 6f61 645f 6669  r......upload_fi
+000009d0: 6c65 da03 7374 7272 0b00 0000 2905 7215  le..strr....).r.
+000009e0: 0000 0072 2200 0000 7223 0000 0072 2400  ...r"...r#...r$.
+000009f0: 0000 7225 0000 0072 1600 0000 7216 0000  ..r%...r....r...
+00000a00: 0072 1700 0000 722a 0000 003d 0000 0073  .r....r*...=...s
+00000a10: 1200 0000 0807 0a01 0602 0601 0401 0601  ................
+00000a20: 0201 0201 0afb 7a15 5333 5f42 7563 6b65  ......z.S3_Bucke
+00000a30: 742e 7570 6c6f 6164 5f66 696c 6554 da0e  t.upload_fileT..
+00000a40: 6372 6561 7465 5f70 6172 656e 7473 6306  create_parentsc.
+00000a50: 0000 0000 0000 0000 0000 0007 0000 0006  ................
+00000a60: 0000 0043 0000 0073 4400 0000 7c05 720e  ...C...sD...|.r.
+00000a70: 7400 7c02 8301 7d06 7c06 6a01 6a02 6401  t.|...}.|.j.j.d.
+00000a80: 6401 6402 8d02 0100 7c00 6a03 a004 7c00  d.d.....|.j...|.
+00000a90: 6a05 a101 6a06 7407 7c01 8301 7407 7c02  j...j.t.|...t.|.
+00000aa0: 8301 7c03 7c04 6403 8d04 0100 6400 5300  ..|.|.d.....d.S.
+00000ab0: 2904 4e54 2902 da07 7061 7265 6e74 73da  ).NT)...parents.
+00000ac0: 0865 7869 7374 5f6f 6b29 0472 2700 0000  .exist_ok).r'...
+00000ad0: 7226 0000 0072 2800 0000 7229 0000 0029  r&...r(...r)...)
+00000ae0: 0872 0400 0000 da06 7061 7265 6e74 da05  .r......parent..
+00000af0: 6d6b 6469 7272 1200 0000 7213 0000 0072  mkdirr....r....r
+00000b00: 0b00 0000 da0d 646f 776e 6c6f 6164 5f66  ......download_f
+00000b10: 696c 6572 2b00 0000 2907 7215 0000 0072  iler+...).r....r
+00000b20: 2300 0000 7222 0000 0072 2400 0000 7225  #...r"...r$...r%
+00000b30: 0000 0072 2c00 0000 5a0a 6c6f 6361 6c5f  ...r,...Z.local_
+00000b40: 7061 7468 7216 0000 0072 1600 0000 7217  pathr....r....r.
+00000b50: 0000 0072 3100 0000 4f00 0000 7312 0000  ...r1...O...s...
+00000b60: 0004 0808 0110 010e 0106 0106 0102 0102  ................
+00000b70: 010a fc7a 1753 335f 4275 636b 6574 2e64  ...z.S3_Bucket.d
+00000b80: 6f77 6e6c 6f61 645f 6669 6c65 6302 0000  ownload_filec...
+00000b90: 0000 0000 0000 0000 0002 0000 0008 0000  ................
+00000ba0: 0043 0000 0073 3200 0000 7a0e 7c00 6a00  .C...s2...z.|.j.
+00000bb0: 6a01 7c00 6a02 7403 7c01 8301 6401 8d02  j.|.j.t.|...d...
+00000bc0: 0100 5700 6402 5300 0400 7404 7918 0100  ..W.d.S...t.y...
+00000bd0: 0100 0100 5900 6403 5300 7700 2904 4ea9  ....Y.d.S.w.).N.
+00000be0: 0272 1300 0000 7227 0000 0054 4629 0572  .r....r'...TF).r
+00000bf0: 1e00 0000 5a0b 6865 6164 5f6f 626a 6563  ....Z.head_objec
+00000c00: 7472 0b00 0000 722b 0000 00da 0945 7863  tr....r+.....Exc
+00000c10: 6570 7469 6f6e a902 7215 0000 0072 2300  eption..r....r#.
+00000c20: 0000 7216 0000 0072 1600 0000 7217 0000  ..r....r....r...
+00000c30: 00da 0a6b 6579 5f65 7869 7374 7361 0000  ...key_existsa..
+00000c40: 0073 0c00 0000 0201 1601 0601 0c01 0601  .s..............
+00000c50: 02ff 7a14 5333 5f42 7563 6b65 742e 6b65  ..z.S3_Bucket.ke
+00000c60: 795f 6578 6973 7473 6302 0000 0000 0000  y_existsc.......
+00000c70: 0000 0000 0002 0000 0005 0000 0043 0000  .............C..
+00000c80: 0073 1400 0000 7c00 6a00 a001 7c00 6a02  .s....|.j...|.j.
+00000c90: 7403 7c01 8301 a102 5300 7211 0000 0029  t.|.....S.r....)
+00000ca0: 0472 1200 0000 5a06 4f62 6a65 6374 720b  .r....Z.Objectr.
+00000cb0: 0000 0072 2b00 0000 7234 0000 0072 1600  ...r+...r4...r..
+00000cc0: 0000 7216 0000 0072 1700 0000 da0a 6765  ..r....r......ge
+00000cd0: 745f 6f62 6a65 6374 6800 0000 f302 0000  t_objecth.......
+00000ce0: 0014 017a 1453 335f 4275 636b 6574 2e67  ...z.S3_Bucket.g
+00000cf0: 6574 5f6f 626a 6563 74da 0a76 6572 7369  et_object..versi
+00000d00: 6f6e 5f69 6463 0300 0000 0000 0000 0000  on_idc..........
+00000d10: 0000 0400 0000 0400 0000 4300 0000 7336  ..........C...s6
+00000d20: 0000 007c 006a 0074 017c 0183 0164 019c  ...|.j.t.|...d..
+00000d30: 027d 037c 0264 0075 0172 107c 027c 0364  .}.|.d.u.r.|.|.d
+00000d40: 023c 007c 006a 026a 0364 0369 007c 03a4  .<.|.j.j.d.i.|..
+00000d50: 018e 0101 0064 0053 0029 044e 7232 0000  .....d.S.).Nr2..
+00000d60: 00da 0956 6572 7369 6f6e 4964 7216 0000  ...VersionIdr...
+00000d70: 0029 0472 0b00 0000 722b 0000 0072 1e00  .).r....r+...r..
+00000d80: 0000 5a0d 6465 6c65 7465 5f6f 626a 6563  ..Z.delete_objec
+00000d90: 7429 0472 1500 0000 7223 0000 0072 3800  t).r....r#...r8.
+00000da0: 0000 da06 6b77 6172 6773 7216 0000 0072  ....kwargsr....r
+00000db0: 1600 0000 7217 0000 00da 0d64 656c 6574  ....r......delet
+00000dc0: 655f 6279 5f6b 6579 6b00 0000 730c 0000  e_by_keyk...s...
+00000dd0: 0004 0206 0106 fe08 0408 0116 017a 1753  .............z.S
+00000de0: 335f 4275 636b 6574 2e64 656c 6574 655f  3_Bucket.delete_
+00000df0: 6279 5f6b 6579 fa25 626f 746f 7374 7562  by_key.%botostub
+00000e00: 732e 5333 2e53 3352 6573 6f75 7263 652e  s.S3.S3Resource.
+00000e10: 4f62 6a65 6374 5375 6d6d 6172 7963 0200  ObjectSummaryc..
+00000e20: 0000 0000 0000 0000 0000 0300 0000 0300  ................
+00000e30: 0000 4300 0000 732c 0000 007c 0164 0075  ..C...s,...|.d.u
+00000e40: 0072 0664 017d 017c 006a 00a0 017c 006a  .r.d.}.|.j...|.j
+00000e50: 02a1 016a 036a 0474 057c 0183 0164 028d  ...j.j.t.|...d..
+00000e60: 017d 027c 0253 0029 034e da00 2901 da06  .}.|.S.).N..)...
+00000e70: 5072 6566 6978 2906 7212 0000 0072 1300  Prefix).r....r..
+00000e80: 0000 720b 0000 00da 076f 626a 6563 7473  ..r......objects
+00000e90: da06 6669 6c74 6572 722b 0000 0029 0372  ..filterr+...).r
+00000ea0: 1500 0000 7223 0000 00da 0a63 6f6c 6c65  ....r#.....colle
+00000eb0: 6374 696f 6e72 1600 0000 7216 0000 0072  ctionr....r....r
+00000ec0: 1700 0000 da0c 6669 6e64 5f6f 626a 6563  ......find_objec
+00000ed0: 7473 7400 0000 7308 0000 0008 0104 011c  tst...s.........
+00000ee0: 0104 017a 1653 335f 4275 636b 6574 2e66  ...z.S3_Bucket.f
+00000ef0: 696e 645f 6f62 6a65 6374 7363 0200 0000  ind_objectsc....
+00000f00: 0000 0000 0000 0000 0300 0000 0300 0000  ................
+00000f10: 4300 0000 7318 0000 007c 00a0 007c 01a1  C...s....|...|..
+00000f20: 017d 0264 0164 0284 007c 0244 0083 0153  .}.d.d...|.D...S
+00000f30: 0029 034e 6301 0000 0000 0000 0000 0000  .).Nc...........
+00000f40: 0002 0000 0003 0000 0053 0000 0073 1200  .........S...s..
+00000f50: 0000 6700 7c00 5d05 7d01 7c01 6a00 9102  ..g.|.].}.|.j...
+00000f60: 7102 5300 7216 0000 00a9 0172 2300 0000  q.S.r......r#...
+00000f70: 2902 da02 2e30 da03 6f62 6a72 1600 0000  )....0..objr....
+00000f80: 7216 0000 0072 1700 0000 da0a 3c6c 6973  r....r......<lis
+00000f90: 7463 6f6d 703e 7c00 0000 7302 0000 0012  tcomp>|...s.....
+00000fa0: 007a 2e53 335f 4275 636b 6574 2e6c 6973  .z.S3_Bucket.lis
+00000fb0: 745f 6f62 6a65 6374 5f6b 6579 732e 3c6c  t_object_keys.<l
+00000fc0: 6f63 616c 733e 2e3c 6c69 7374 636f 6d70  ocals>.<listcomp
+00000fd0: 3e29 0172 4200 0000 2903 7215 0000 0072  >).rB...).r....r
+00000fe0: 2300 0000 5a0e 6f62 6a5f 636f 6c6c 6563  #...Z.obj_collec
+00000ff0: 7469 6f6e 7216 0000 0072 1600 0000 7217  tionr....r....r.
+00001000: 0000 00da 106c 6973 745f 6f62 6a65 6374  .....list_object
+00001010: 5f6b 6579 737a 0000 0073 0400 0000 0a01  _keysz...s......
+00001020: 0e01 7a1a 5333 5f42 7563 6b65 742e 6c69  ..z.S3_Bucket.li
+00001030: 7374 5f6f 626a 6563 745f 6b65 7973 6302  st_object_keysc.
+00001040: 0000 0000 0000 0000 0000 0002 0000 0004  ................
+00001050: 0000 0043 0000 0073 1400 0000 6401 6402  ...C...s....d.d.
+00001060: 8400 7c00 a000 7c01 a101 4400 8301 5300  ..|...|...D...S.
+00001070: 2903 4e63 0100 0000 0000 0000 0000 0000  ).Nc............
+00001080: 0200 0000 0400 0000 5300 0000 7314 0000  ........S...s...
+00001090: 0067 007c 005d 067d 0174 007c 0183 0191  .g.|.].}.t.|....
+000010a0: 0271 0253 0072 1600 0000 2901 7203 0000  .q.S.r....).r...
+000010b0: 0029 0272 4400 0000 7223 0000 0072 1600  .).rD...r#...r..
+000010c0: 0000 7216 0000 0072 1700 0000 7246 0000  ..r....r....rF..
+000010d0: 007f 0000 0073 0200 0000 1400 7a2f 5333  .....s......z/S3
+000010e0: 5f42 7563 6b65 742e 6c69 7374 5f6f 626a  _Bucket.list_obj
+000010f0: 6563 745f 7061 7468 732e 3c6c 6f63 616c  ect_paths.<local
+00001100: 733e 2e3c 6c69 7374 636f 6d70 3e29 0172  s>.<listcomp>).r
+00001110: 4700 0000 7234 0000 0072 1600 0000 7216  G...r4...r....r.
+00001120: 0000 0072 1700 0000 da11 6c69 7374 5f6f  ...r......list_o
+00001130: 626a 6563 745f 7061 7468 737e 0000 0072  bject_paths~...r
+00001140: 3700 0000 7a1b 5333 5f42 7563 6b65 742e  7...z.S3_Bucket.
+00001150: 6c69 7374 5f6f 626a 6563 745f 7061 7468  list_object_path
+00001160: 73da 0867 6574 5f63 6f70 79da 0963 6f70  s..get_copy..cop
+00001170: 6965 645f 6279 6302 0000 0000 0000 0000  ied_byc.........
+00001180: 0000 0002 0000 0005 0000 0003 0000 00f3  ................
+00001190: 1200 0000 7400 6401 7401 8300 a002 7c01  ....t.d.t.....|.
+000011a0: a101 8302 5300 2902 4e72 0a00 0000 a903  ....S.).Nr......
+000011b0: da04 6361 7374 da05 7375 7065 7272 4900  ..cast..superrI.
+000011c0: 0000 a902 7215 0000 0072 4a00 0000 a901  ....r....rJ.....
+000011d0: da09 5f5f 636c 6173 735f 5f72 1600 0000  ..__class__r....
+000011e0: 7217 0000 0072 4900 0000 8100 0000 f302  r....rI.........
+000011f0: 0000 0012 017a 1253 335f 4275 636b 6574  .....z.S3_Bucket
+00001200: 2e67 6574 5f63 6f70 79da 0d53 335f 4275  .get_copy..S3_Bu
+00001210: 636b 6574 5f4b 6579 6302 0000 0000 0000  cket_Keyc.......
+00001220: 0000 0000 0002 0000 0003 0000 0043 0000  .............C..
+00001230: 00f3 0a00 0000 7c00 a000 7c01 a101 5300  ......|...|...S.
+00001240: 7211 0000 00a9 01da 145f 6275 696c 645f  r........_build_
+00001250: 7333 5f62 7563 6b65 745f 6b65 7972 3400  s3_bucket_keyr4.
+00001260: 0000 7216 0000 0072 1600 0000 7217 0000  ..r....r....r...
+00001270: 00da 0a6e 6176 5f74 6f5f 6b65 7984 0000  ...nav_to_key...
+00001280: 00f3 0200 0000 0a01 7a14 5333 5f42 7563  ........z.S3_Buc
+00001290: 6b65 742e 6e61 765f 746f 5f6b 6579 da06  ket.nav_to_key..
+000012a0: 666f 6c64 6572 da10 5333 5f42 7563 6b65  folder..S3_Bucke
+000012b0: 745f 466f 6c64 6572 6302 0000 0000 0000  t_Folderc.......
+000012c0: 0000 0000 0002 0000 0003 0000 0043 0000  .............C..
+000012d0: 0072 5400 0000 7211 0000 00a9 01da 175f  .rT...r........_
+000012e0: 6275 696c 645f 7333 5f62 7563 6b65 745f  build_s3_bucket_
+000012f0: 666f 6c64 6572 a902 7215 0000 0072 5900  folder..r....rY.
+00001300: 0000 7216 0000 0072 1600 0000 7217 0000  ..r....r....r...
+00001310: 00da 0d6e 6176 5f74 6f5f 666f 6c64 6572  ...nav_to_folder
+00001320: 8700 0000 f302 0000 000a 047a 1753 335f  ...........z.S3_
+00001330: 4275 636b 6574 2e6e 6176 5f74 6f5f 666f  Bucket.nav_to_fo
+00001340: 6c64 6572 6302 0000 0000 0000 0000 0000  lderc...........
+00001350: 0002 0000 0003 0000 0043 0000 0072 5400  .........C...rT.
+00001360: 0000 7211 0000 0072 5b00 0000 725d 0000  ..r....r[...r]..
+00001370: 0072 1600 0000 7216 0000 0072 1700 0000  .r....r....r....
+00001380: da16 6e61 765f 746f 5f72 656c 6174 6976  ..nav_to_relativ
+00001390: 655f 666f 6c64 6572 8d00 0000 725f 0000  e_folder....r_..
+000013a0: 007a 2053 335f 4275 636b 6574 2e6e 6176  .z S3_Bucket.nav
+000013b0: 5f74 6f5f 7265 6c61 7469 7665 5f66 6f6c  _to_relative_fol
+000013c0: 6465 72da 056f 7468 6572 6302 0000 0000  der..otherc.....
+000013d0: 0000 0000 0000 0002 0000 0003 0000 0043  ...............C
+000013e0: 0000 0072 5400 0000 7211 0000 0029 0172  ...rT...r....).r
+000013f0: 5700 0000 2902 7215 0000 0072 6100 0000  W...).r....ra...
+00001400: 7216 0000 0072 1600 0000 7217 0000 00da  r....r....r.....
+00001410: 0b5f 5f74 7275 6564 6976 5f5f 9300 0000  .__truediv__....
+00001420: 7302 0000 000a 037a 1553 335f 4275 636b  s......z.S3_Buck
+00001430: 6574 2e5f 5f74 7275 6564 6976 5f5f 2902  et.__truediv__).
+00001440: 7253 0000 0072 5a00 0000 6301 0000 0000  rS...rZ...c.....
+00001450: 0000 0000 0000 0004 0000 0003 0000 0047  ...............G
+00001460: 0000 0073 1a00 0000 7c00 7d02 7c01 4400  ...s....|.}.|.D.
+00001470: 5d06 7d03 7c02 7c03 1b00 7d02 7104 7c02  ].}.|.|...}.q.|.
+00001480: 5300 7211 0000 0072 1600 0000 2904 7215  S.r....r....).r.
+00001490: 0000 00da 066f 7468 6572 73da 086e 6577  .....others..new
+000014a0: 5f70 6174 6872 6100 0000 7216 0000 0072  _pathra...r....r
+000014b0: 1600 0000 7217 0000 00da 086a 6f69 6e70  ....r......joinp
+000014c0: 6174 6899 0000 0073 0800 0000 0407 0801  ath....s........
+000014d0: 0a01 0401 7a12 5333 5f42 7563 6b65 742e  ....z.S3_Bucket.
+000014e0: 6a6f 696e 7061 7468 6302 0000 0000 0000  joinpathc.......
+000014f0: 0000 0000 0002 0000 0005 0000 0043 0000  .............C..
+00001500: 0073 1600 0000 7c00 6a00 7401 6401 6801  .s....|.j.t.d.h.
+00001510: 7402 7c01 8301 6402 8d03 5300 2903 4eda  t.|...d...S.).N.
+00001520: 0966 696c 655f 6e61 6d65 2902 da07 6578  .file_name)...ex
+00001530: 636c 7564 6572 5900 0000 2903 da08 5f66  cluderY...)..._f
+00001540: 6163 746f 7279 725a 0000 0072 2b00 0000  actoryrZ...r+...
+00001550: 725d 0000 0072 1600 0000 7216 0000 0072  r]...r....r....r
+00001560: 1700 0000 725c 0000 00a5 0000 0073 0a00  ....r\.......s..
+00001570: 0000 0401 0201 0401 0601 06fd 7a21 5333  ............z!S3
+00001580: 5f42 7563 6b65 742e 5f62 7569 6c64 5f73  _Bucket._build_s
+00001590: 335f 6275 636b 6574 5f66 6f6c 6465 7272  3_bucket_folderr
+000015a0: 6600 0000 6303 0000 0000 0000 0000 0000  f...c...........
+000015b0: 0003 0000 0006 0000 0043 0000 0073 3a00  .........C...s:.
+000015c0: 0000 7c02 6400 7500 720f 7c00 6a00 7401  ..|.d.u.r.|.j.t.
+000015d0: 6401 6801 7402 7c01 8301 6402 8d03 5300  d.h.t.|...d...S.
+000015e0: 7c00 6a00 7401 6401 6801 7402 7c02 8301  |.j.t.d.h.t.|...
+000015f0: 7402 7c01 8301 6403 8d04 5300 2904 4e72  t.|...d...S.).Nr
+00001600: 2300 0000 2902 7267 0000 0072 6600 0000  #...).rg...rf...
+00001610: 2903 7267 0000 0072 5900 0000 7266 0000  ).rg...rY...rf..
+00001620: 0029 0372 6800 0000 da15 5333 5f42 7563  .).rh.....S3_Buc
+00001630: 6b65 745f 466f 6c64 6572 5f46 696c 6572  ket_Folder_Filer
+00001640: 2b00 0000 2903 7215 0000 0072 6600 0000  +...).r....rf...
+00001650: 7259 0000 0072 1600 0000 7216 0000 0072  rY...r....r....r
+00001660: 1700 0000 da1c 5f62 7569 6c64 5f73 335f  ......_build_s3_
+00001670: 6275 636b 6574 5f66 6f6c 6465 725f 6669  bucket_folder_fi
+00001680: 6c65 ac00 0000 7318 0000 0008 0104 0102  le....s.........
+00001690: 0104 0106 0106 fd04 0602 0104 0106 0106  ................
+000016a0: 0106 fc7a 2653 335f 4275 636b 6574 2e5f  ...z&S3_Bucket._
+000016b0: 6275 696c 645f 7333 5f62 7563 6b65 745f  build_s3_bucket_
+000016c0: 666f 6c64 6572 5f66 696c 6563 0200 0000  folder_filec....
+000016d0: 0000 0000 0000 0000 0200 0000 0500 0000  ................
+000016e0: 4300 0000 7318 0000 007c 006a 0074 0174  C...s....|.j.t.t
+000016f0: 027c 0183 0164 0164 0268 0264 038d 0353  .|...d.d.h.d...S
+00001700: 0029 044e 7259 0000 0072 6600 0000 2902  .).NrY...rf...).
+00001710: 7223 0000 0072 6700 0000 2903 7268 0000  r#...rg...).rh..
+00001720: 0072 5300 0000 722b 0000 0072 3400 0000  .rS...r+...r4...
+00001730: 7216 0000 0072 1600 0000 7217 0000 0072  r....r....r....r
+00001740: 5600 0000 bb00 0000 7302 0000 0018 017a  V.......s......z
+00001750: 1e53 335f 4275 636b 6574 2e5f 6275 696c  .S3_Bucket._buil
+00001760: 645f 7333 5f62 7563 6b65 745f 6b65 7929  d_s3_bucket_key)
+00001770: 0272 0f00 0000 7210 0000 00a9 024e 4ea9  .r....r......NN.
+00001780: 034e 4e54 7211 0000 00a9 0172 4900 0000  .NNTr......rI...
+00001790: a902 720f 0000 0072 5300 0000 2928 da08  ..r....rS...)(..
+000017a0: 5f5f 6e61 6d65 5f5f da0a 5f5f 6d6f 6475  __name__..__modu
+000017b0: 6c65 5f5f da0c 5f5f 7175 616c 6e61 6d65  le__..__qualname
+000017c0: 5f5f 722b 0000 00da 0f5f 5f61 6e6e 6f74  __r+.....__annot
+000017d0: 6174 696f 6e73 5f5f 7207 0000 0072 0e00  ations__r....r..
+000017e0: 0000 7218 0000 0072 1a00 0000 da0c 7374  ..r....r......st
+000017f0: 6174 6963 6d65 7468 6f64 7202 0000 0072  aticmethodr....r
+00001800: 2000 0000 7221 0000 00da 0555 6e69 6f6e   ...r!.....Union
+00001810: 7204 0000 0072 0300 0000 da08 4f70 7469  r....r......Opti
+00001820: 6f6e 616c da04 6469 6374 7206 0000 0072  onal..dictr....r
+00001830: 2a00 0000 da04 626f 6f6c 7231 0000 0072  *.....boolr1...r
+00001840: 3500 0000 7236 0000 0072 3b00 0000 da08  5...r6...r;.....
+00001850: 4974 6572 6162 6c65 7242 0000 00da 044c  IterablerB.....L
+00001860: 6973 7472 4700 0000 7248 0000 0072 4900  istrG...rH...rI.
+00001870: 0000 7257 0000 0072 5e00 0000 7260 0000  ..rW...r^...r`..
+00001880: 0072 6200 0000 7265 0000 0072 5c00 0000  .rb...re...r\...
+00001890: 726a 0000 0072 5600 0000 da0d 5f5f 636c  rj...rV.....__cl
+000018a0: 6173 7363 656c 6c5f 5f72 1600 0000 7216  asscell__r....r.
+000018b0: 0000 0072 5000 0000 7217 0000 0072 0a00  ...rP...r....r..
+000018c0: 0000 1d00 0000 7382 0000 000a 0008 0112  ......s.........
+000018d0: 020a 0208 0302 0308 0112 010e 0902 0e02  ................
+000018e0: 0104 fb0a 0202 fe0a 0302 fd06 0402 fc06  ................
+000018f0: 050a fb02 1602 0102 0104 fa0a 0202 fe0a  ................
+00001900: 0302 fd06 0402 fc06 0502 fb02 060a fa1a  ................
+00001910: 1216 071c 0320 0920 061e 0418 030a 0302  ..... . ........
+00001920: 030a 0202 fe02 030a fd02 060a 0202 fe02  ................
+00001930: 030a fd02 060a 0102 ff02 020a fe02 0602  ................
+00001940: 0302 0102 ff0a fd16 0c24 071e 0f72 0a00  .........$...r..
+00001950: 0000 6300 0000 0000 0000 0000 0000 0000  ..c.............
+00001960: 0000 000b 0000 0000 0000 0073 9c01 0000  ...........s....
+00001970: 6500 5a01 6400 5a02 5500 6401 5a03 6504  e.Z.d.Z.U.d.Z.e.
+00001980: 6505 6402 3c00 6506 6402 8301 6403 6404  e.d.<.e.d...d.d.
+00001990: 8400 8301 5a07 6405 6406 8400 5a08 642b  ....Z.d.d...Z.d+
+000019a0: 6408 6504 6409 6400 6604 8700 6601 640a  d.e.d.d.f...f.d.
+000019b0: 640b 840d 5a09 090c 090c 642c 640d 650a  d...Z.....d,d.e.
+000019c0: 6504 650b 6602 1900 640e 650a 6504 650c  e.e.f...d.e.e.e.
+000019d0: 6602 1900 640f 650d 650e 1900 6410 650d  f...d.e.e...d.e.
+000019e0: 650f 1900 6608 8700 6601 6411 6412 840d  e...f...f.d.d...
+000019f0: 5a10 090c 090c 0913 642d 640e 650a 6504  Z.......d-d.e.e.
+00001a00: 650c 6602 1900 640d 650a 6504 650b 6602  e.f...d.e.e.e.f.
+00001a10: 1900 640f 650d 650e 1900 6410 650d 650f  ..d.e.e...d.e.e.
+00001a20: 1900 6414 6511 660a 8700 6601 6415 6416  ..d.e.f...f.d.d.
+00001a30: 840d 5a12 6417 650a 6504 650b 6602 1900  ..Z.d.e.e.e.f...
+00001a40: 6409 6400 6604 6418 6419 8404 5a13 6402  d.d.f.d.d...Z.d.
+00001a50: 650a 6504 650b 6602 1900 6409 6400 6604  e.e.e.f...d.d.f.
+00001a60: 641a 641b 8404 5a14 641c 650a 6504 650b  d.d...Z.d.e.e.e.
+00001a70: 6602 1900 6409 641d 6604 641e 641f 8404  f...d.d.f.d.d...
+00001a80: 5a15 6420 650a 6504 650b 6602 1900 6409  Z.d e.e.e.f...d.
+00001a90: 6421 6604 6422 6423 8404 5a16 642e 6424  d!f.d"d#..Z.d.d$
+00001aa0: 650a 6504 650c 6602 1900 6409 6517 6504  e.e.e.f...d.e.e.
+00001ab0: 1900 6604 8700 6601 6425 6426 840d 5a18  ..f...f.d%d&..Z.
+00001ac0: 642e 6424 650a 6504 650c 6602 1900 6409  d.d$e.e.e.f...d.
+00001ad0: 6517 650c 1900 6604 8700 6601 6427 6428  e.e...f...f.d'd(
+00001ae0: 840d 5a19 642e 6424 650a 6504 650c 6602  ..Z.d.d$e.e.e.f.
+00001af0: 1900 6409 6511 6604 8700 6601 6429 642a  ..d.e.f...f.d)d*
+00001b00: 840d 5a1a 8700 0400 5a1b 5300 292f 725a  ..Z.....Z.S.)/rZ
+00001b10: 0000 007a 360a 2020 2020 2020 2020 5265  ...z6.        Re
+00001b20: 7072 6573 656e 7473 2061 2066 6f6c 6465  presents a folde
+00001b30: 7220 7769 7468 696e 2061 6e20 5333 2062  r within an S3 b
+00001b40: 7563 6b65 742e 0a20 2020 2072 5900 0000  ucket..    rY...
+00001b50: 6302 0000 0000 0000 0000 0000 0002 0000  c...............
+00001b60: 0003 0000 0043 0000 00f3 2a00 0000 7400  .....C....*...t.
+00001b70: 7c01 7401 8302 7309 7401 7c01 8301 7d01  |.t...s.t.|...}.
+00001b80: 7402 7c01 8301 6401 6b02 7213 7403 6402  t.|...d.k.r.t.d.
+00001b90: 8301 8201 7c01 5300 2903 4e72 0100 0000  ....|.S.).Nr....
+00001ba0: 7a25 5a65 726f 206c 656e 6774 6820 7374  z%Zero length st
+00001bb0: 7269 6e67 206e 6f74 2061 2076 616c 6964  ring not a valid
+00001bc0: 2066 6f6c 6465 72a9 04da 0a69 7369 6e73   folder....isins
+00001bd0: 7461 6e63 6572 2b00 0000 da03 6c65 6eda  tancer+.....len.
+00001be0: 0a56 616c 7565 4572 726f 72a9 02da 0363  .ValueError....c
+00001bf0: 6c73 da01 7672 1600 0000 7216 0000 0072  ls..vr....r....r
+00001c00: 1700 0000 da0f 7661 6c69 6461 7465 5f66  ......validate_f
+00001c10: 6f6c 6465 72c6 0000 00f3 0a00 0000 0a03  older...........
+00001c20: 0801 0c01 0801 0401 7a20 5333 5f42 7563  ........z S3_Buc
+00001c30: 6b65 745f 466f 6c64 6572 2e76 616c 6964  ket_Folder.valid
+00001c40: 6174 655f 666f 6c64 6572 6301 0000 0000  ate_folderc.....
+00001c50: 0000 0000 0000 0001 0000 0004 0000 0043  ...............C
+00001c60: 0000 00f3 1400 0000 6401 7c00 6a00 9b00  ........d.|.j...
+00001c70: 6402 7c00 6a01 9b00 9d04 5300 a903 4e72  d.|.j.....S...Nr
+00001c80: 1900 0000 fa01 2f29 0272 0b00 0000 7259  ....../).r....rY
+00001c90: 0000 0072 1400 0000 7216 0000 0072 1600  ...r....r....r..
+00001ca0: 0000 7217 0000 0072 1a00 0000 cf00 0000  ..r....r........
+00001cb0: 7237 0000 007a 1853 335f 4275 636b 6574  r7...z.S3_Bucket
+00001cc0: 5f46 6f6c 6465 722e 5f5f 7374 725f 5f72  _Folder.__str__r
+00001cd0: 4900 0000 724a 0000 0072 0f00 0000 6302  I...rJ...r....c.
+00001ce0: 0000 0000 0000 0000 0000 0002 0000 0005  ................
+00001cf0: 0000 0003 0000 0072 4b00 0000 2902 4e72  .......rK...).Nr
+00001d00: 5a00 0000 724c 0000 0072 4f00 0000 7250  Z...rL...rO...rP
+00001d10: 0000 0072 1600 0000 7217 0000 0072 4900  ...r....r....rI.
+00001d20: 0000 d200 0000 7252 0000 007a 1953 335f  ......rR...z.S3_
+00001d30: 4275 636b 6574 5f46 6f6c 6465 722e 6765  Bucket_Folder.ge
+00001d40: 745f 636f 7079 4e72 2200 0000 da0a 6b65  t_copyNr".....ke
+00001d50: 795f 7375 6666 6978 7224 0000 0072 2500  y_suffixr$...r%.
+00001d60: 0000 6305 0000 0000 0000 0000 0000 0006  ..c.............
+00001d70: 0000 0006 0000 0003 0000 0073 2400 0000  ...........s$...
+00001d80: 7400 7c00 6a01 7c02 8302 7d05 7402 8300  t.|.j.|...}.t...
+00001d90: 6a03 7c01 7c05 7c03 7c04 6401 8d04 0100  j.|.|.|.|.d.....
+00001da0: 6400 5300 a902 4e29 0472 2200 0000 7223  d.S...N).r"...r#
+00001db0: 0000 0072 2400 0000 7225 0000 0029 0472  ...r$...r%...).r
+00001dc0: 0300 0000 7259 0000 0072 4e00 0000 722a  ....rY...rN...r*
+00001dd0: 0000 0029 0672 1500 0000 7222 0000 0072  ...).r....r"...r
+00001de0: 8800 0000 7224 0000 0072 2500 0000 da08  ....r$...r%.....
+00001df0: 6675 6c6c 5f6b 6579 7250 0000 0072 1600  full_keyrP...r..
+00001e00: 0000 7217 0000 00da 1275 706c 6f61 645f  ..r......upload_
+00001e10: 666f 6c64 6572 5f66 696c 65d5 0000 0073  folder_file....s
+00001e20: 0e00 0000 0c07 0601 0201 0201 0201 0201  ................
+00001e30: 0afc 7a23 5333 5f42 7563 6b65 745f 466f  ..z#S3_Bucket_Fo
+00001e40: 6c64 6572 2e75 706c 6f61 645f 666f 6c64  lder.upload_fold
+00001e50: 6572 5f66 696c 6554 722c 0000 0063 0600  er_fileTr,...c..
+00001e60: 0000 0000 0000 0000 0000 0700 0000 0700  ................
+00001e70: 0000 0300 0000 7326 0000 0074 007c 006a  ......s&...t.|.j
+00001e80: 017c 0183 027d 0674 0283 006a 037c 067c  .|...}.t...j.|.|
+00001e90: 027c 037c 047c 0564 018d 0501 0064 0053  .|.|.|.d.....d.S
+00001ea0: 0029 024e 2905 7223 0000 0072 2200 0000  .).N).r#...r"...
+00001eb0: 7224 0000 0072 2500 0000 722c 0000 0029  r$...r%...r,...)
+00001ec0: 0472 0300 0000 7259 0000 0072 4e00 0000  .r....rY...rN...
+00001ed0: 7231 0000 0029 0772 1500 0000 7288 0000  r1...).r....r...
+00001ee0: 0072 2200 0000 7224 0000 0072 2500 0000  .r"...r$...r%...
+00001ef0: 722c 0000 0072 8a00 0000 7250 0000 0072  r,...r....rP...r
+00001f00: 1600 0000 7217 0000 00da 1464 6f77 6e6c  ....r......downl
+00001f10: 6f61 645f 666f 6c64 6572 5f66 696c 65e4  oad_folder_file.
+00001f20: 0000 0073 1000 0000 0c08 0601 0201 0201  ...s............
+00001f30: 0201 0201 0201 0afb 7a25 5333 5f42 7563  ........z%S3_Buc
+00001f40: 6b65 745f 466f 6c64 6572 2e64 6f77 6e6c  ket_Folder.downl
+00001f50: 6f61 645f 666f 6c64 6572 5f66 696c 65da  oad_folder_file.
+00001f60: 0a66 6f6c 6465 725f 6b65 7963 0200 0000  .folder_keyc....
+00001f70: 0000 0000 0000 0000 0200 0000 0300 0000  ................
+00001f80: 4300 0000 7254 0000 0072 1100 0000 725b  C...rT...r....r[
+00001f90: 0000 0029 0272 1500 0000 728d 0000 0072  ...).r....r....r
+00001fa0: 1600 0000 7216 0000 0072 1700 0000 725e  ....r....r....r^
+00001fb0: 0000 00f5 0000 0072 5800 0000 7a1e 5333  .......rX...z.S3
+00001fc0: 5f42 7563 6b65 745f 466f 6c64 6572 2e6e  _Bucket_Folder.n
+00001fd0: 6176 5f74 6f5f 666f 6c64 6572 6302 0000  av_to_folderc...
+00001fe0: 0000 0000 0000 0000 0003 0000 0003 0000  ................
+00001ff0: 0043 0000 00f3 1800 0000 7400 7c00 6a01  .C........t.|.j.
+00002000: 8301 7c01 1b00 7d02 7c00 a002 7c02 a101  ..|...}.|...|...
+00002010: 5300 7211 0000 0029 0372 0300 0000 7259  S.r....).r....rY
+00002020: 0000 0072 5e00 0000 a903 7215 0000 0072  ...r^.....r....r
+00002030: 5900 0000 7264 0000 0072 1600 0000 7216  Y...rd...r....r.
+00002040: 0000 0072 1700 0000 7260 0000 00f8 0000  ...r....r`......
+00002050: 0073 0400 0000 0e01 0a01 7a27 5333 5f42  .s........z'S3_B
+00002060: 7563 6b65 745f 466f 6c64 6572 2e6e 6176  ucket_Folder.nav
+00002070: 5f74 6f5f 7265 6c61 7469 7665 5f66 6f6c  _to_relative_fol
+00002080: 6465 7272 6600 0000 7269 0000 0063 0200  derrf...ri...c..
+00002090: 0000 0000 0000 0000 0000 0200 0000 0300  ................
+000020a0: 0000 4300 0000 7254 0000 0072 1100 0000  ..C...rT...r....
+000020b0: 2901 726a 0000 00a9 0272 1500 0000 7266  ).rj.....r....rf
+000020c0: 0000 0072 1600 0000 7216 0000 0072 1700  ...r....r....r..
+000020d0: 0000 da0b 6e61 765f 746f 5f66 696c 65fc  ....nav_to_file.
+000020e0: 0000 0073 0600 0000 0404 0201 04ff 7a1c  ...s..........z.
+000020f0: 5333 5f42 7563 6b65 745f 466f 6c64 6572  S3_Bucket_Folder
+00002100: 2e6e 6176 5f74 6f5f 6669 6c65 7261 0000  .nav_to_filera..
+00002110: 0072 5300 0000 6302 0000 0000 0000 0000  .rS...c.........
+00002120: 0000 0003 0000 0003 0000 0043 0000 0072  ...........C...r
+00002130: 8e00 0000 7211 0000 0029 0372 0300 0000  ....r....).r....
+00002140: 7259 0000 0072 5700 0000 a903 7215 0000  rY...rW.....r...
+00002150: 0072 6100 0000 7264 0000 0072 1600 0000  .ra...rd...r....
+00002160: 7216 0000 0072 1700 0000 7262 0000 0004  r....r....rb....
+00002170: 0100 00f3 0400 0000 0e03 0a01 7a1c 5333  ............z.S3
+00002180: 5f42 7563 6b65 745f 466f 6c64 6572 2e5f  _Bucket_Folder._
+00002190: 5f74 7275 6564 6976 5f5f 7223 0000 0063  _truediv__r#...c
+000021a0: 0200 0000 0000 0000 0000 0000 0200 0000  ................
+000021b0: 0300 0000 0300 0000 f31c 0000 007c 0164  .............|.d
+000021c0: 0075 0072 077c 006a 007d 0174 0183 006a  .u.r.|.j.}.t...j
+000021d0: 027c 0164 018d 0153 00a9 024e 7243 0000  .|.d...S...NrC..
+000021e0: 0029 0372 5900 0000 724e 0000 0072 4700  .).rY...rN...rG.
+000021f0: 0000 7234 0000 0072 5000 0000 7216 0000  ..r4...rP...r...
+00002200: 0072 1700 0000 7247 0000 000a 0100 00f3  .r....rG........
+00002210: 0600 0000 0801 0601 0e01 7a21 5333 5f42  ..........z!S3_B
+00002220: 7563 6b65 745f 466f 6c64 6572 2e6c 6973  ucket_Folder.lis
+00002230: 745f 6f62 6a65 6374 5f6b 6579 7363 0200  t_object_keysc..
+00002240: 0000 0000 0000 0000 0000 0200 0000 0300  ................
+00002250: 0000 0300 0000 7294 0000 0072 9500 0000  ......r....r....
+00002260: 2903 7259 0000 0072 4e00 0000 7248 0000  ).rY...rN...rH..
+00002270: 0072 3400 0000 7250 0000 0072 1600 0000  .r4...rP...r....
+00002280: 7217 0000 0072 4800 0000 0f01 0000 7296  r....rH.......r.
+00002290: 0000 007a 2253 335f 4275 636b 6574 5f46  ...z"S3_Bucket_F
+000022a0: 6f6c 6465 722e 6c69 7374 5f6f 626a 6563  older.list_objec
+000022b0: 745f 7061 7468 7363 0200 0000 0000 0000  t_pathsc........
+000022c0: 0000 0000 0200 0000 0300 0000 0300 0000  ................
+000022d0: f31a 0000 007c 0164 0075 0072 077c 006a  .....|.d.u.r.|.j
+000022e0: 007d 0174 0183 00a0 027c 01a1 0153 0072  .}.t.....|...S.r
+000022f0: 1100 0000 2903 7259 0000 0072 4e00 0000  ....).rY...rN...
+00002300: 7235 0000 0072 3400 0000 7250 0000 0072  r5...r4...rP...r
+00002310: 1600 0000 7217 0000 0072 3500 0000 1401  ....r....r5.....
+00002320: 0000 f306 0000 0008 0106 010c 017a 1b53  .............z.S
+00002330: 335f 4275 636b 6574 5f46 6f6c 6465 722e  3_Bucket_Folder.
+00002340: 6b65 795f 6578 6973 7473 726d 0000 0072  key_existsrm...r
+00002350: 6b00 0000 726c 0000 0072 1100 0000 291c  k...rl...r....).
+00002360: 726f 0000 0072 7000 0000 7271 0000 00da  ro...rp...rq....
+00002370: 075f 5f64 6f63 5f5f 722b 0000 0072 7200  .__doc__r+...rr.
+00002380: 0000 7208 0000 0072 8300 0000 721a 0000  ..r....r....r...
+00002390: 0072 4900 0000 7274 0000 0072 0400 0000  .rI...rt...r....
+000023a0: 7203 0000 0072 7500 0000 7276 0000 0072  r....ru...rv...r
+000023b0: 0600 0000 728b 0000 0072 7700 0000 728c  ....r....rw...r.
+000023c0: 0000 0072 5e00 0000 7260 0000 0072 9100  ...r^...r`...r..
+000023d0: 0000 7262 0000 0072 7900 0000 7247 0000  ..rb...ry...rG..
+000023e0: 0072 4800 0000 7235 0000 0072 7a00 0000  .rH...r5...rz...
+000023f0: 7216 0000 0072 1600 0000 7250 0000 0072  r....r....rP...r
+00002400: 1700 0000 725a 0000 00bf 0000 0073 5e00  ....rZ.......s^.
+00002410: 0000 0a00 0401 0803 0603 0a01 0808 1803  ................
+00002420: 0207 0201 04fb 0a02 02fe 0a03 02fd 0604  ................
+00002430: 02fc 0605 0efb 0213 0201 0201 04fa 0a02  ................
+00002440: 02fe 0a03 02fd 0604 02fc 0605 02fb 0206  ................
+00002450: 0efa 1a11 1a03 0204 0a02 02fe 0203 0afd  ................
+00002460: 0208 0a01 02ff 0202 0afe 2406 2405 2805  ..........$.$.(.
+00002470: 725a 0000 0063 0000 0000 0000 0000 0000  rZ...c..........
+00002480: 0000 0000 0000 0800 0000 0000 0000 73e4  ..............s.
+00002490: 0000 0065 005a 0164 005a 0255 0064 015a  ...e.Z.d.Z.U.d.Z
+000024a0: 0365 0465 0564 023c 0065 0664 0283 0164  .e.e.d.<.e.d...d
+000024b0: 0364 0484 0083 015a 0764 0564 0684 005a  .d.....Z.d.d...Z
+000024c0: 0864 1b64 0865 0464 0964 0066 0487 0066  .d.d.e.d.d.f...f
+000024d0: 0164 0a64 0b84 0d5a 0909 0c09 0c64 1c64  .d.d...Z.....d.d
+000024e0: 0d65 0a65 0465 0b66 0219 0064 0e65 0c65  .e.e.e.f...d.e.e
+000024f0: 0d19 0064 0f65 0c65 0e19 0066 0687 0066  ...d.e.e...f...f
+00002500: 0164 1064 1184 0d5a 0f09 0c09 0c64 1c64  .d.d...Z.....d.d
+00002510: 0d65 0a65 0465 0b66 0219 0064 0e65 0c65  .e.e.e.f...d.e.e
+00002520: 0d19 0064 0f65 0c65 0e19 0066 0687 0066  ...d.e.e...f...f
+00002530: 0164 1264 1384 0d5a 1064 1d64 1465 0a65  .d.d...Z.d.d.e.e
+00002540: 0465 0b66 0219 0066 0287 0066 0164 1564  .e.f...f...f.d.d
+00002550: 1684 0d5a 1164 1765 0a65 0465 1266 0219  ...Z.d.e.e.e.f..
+00002560: 0064 0964 1866 0464 1964 1a84 045a 1387  .d.d.f.d.d...Z..
+00002570: 0004 005a 1453 0029 1e72 6900 0000 7a9a  ...Z.S.).ri...z.
+00002580: 0a20 2020 2020 2020 2052 6570 7265 7365  .        Represe
+00002590: 6e74 7320 6120 756e 6971 7565 2066 6f6c  nts a unique fol
+000025a0: 6465 7220 2620 6669 6c65 2077 6974 6869  der & file withi
+000025b0: 6e20 616e 2053 3320 6275 636b 6574 2e0a  n an S3 bucket..
+000025c0: 2020 2020 2020 2020 5369 6d69 6c61 7220          Similar 
+000025d0: 746f 2053 335f 4275 636b 6574 5f4b 6579  to S3_Bucket_Key
+000025e0: 2062 7574 2075 7365 7320 666f 6c64 6572   but uses folder
+000025f0: 202b 2066 696c 655f 6e61 6d65 2069 6e73   + file_name ins
+00002600: 7465 6164 206f 6620 6120 7369 6e67 6c65  tead of a single
+00002610: 206b 6579 2e0a 2020 2020 7266 0000 0063   key..    rf...c
+00002620: 0200 0000 0000 0000 0000 0000 0200 0000  ................
+00002630: 0300 0000 4300 0000 727b 0000 0029 034e  ....C...r{...).N
+00002640: 7201 0000 007a 285a 6572 6f20 6c65 6e67  r....z(Zero leng
+00002650: 7468 2073 7472 696e 6720 6e6f 7420 6120  th string not a 
+00002660: 7661 6c69 6420 6669 6c65 5f6e 616d 6572  valid file_namer
+00002670: 7c00 0000 7280 0000 0072 1600 0000 7216  |...r....r....r.
+00002680: 0000 0072 1700 0000 da12 7661 6c69 6461  ...r......valida
+00002690: 7465 5f66 696c 655f 6e61 6d65 2201 0000  te_file_name"...
+000026a0: 7284 0000 007a 2853 335f 4275 636b 6574  r....z(S3_Bucket
+000026b0: 5f46 6f6c 6465 725f 4669 6c65 2e76 616c  _Folder_File.val
+000026c0: 6964 6174 655f 6669 6c65 5f6e 616d 6563  idate_file_namec
+000026d0: 0100 0000 0000 0000 0000 0000 0100 0000  ................
+000026e0: 0600 0000 4300 0000 731c 0000 0064 017c  ....C...s....d.|
+000026f0: 006a 009b 0064 027c 006a 019b 0064 027c  .j...d.|.j...d.|
+00002700: 006a 029b 009d 0653 0072 8600 0000 2903  .j.....S.r....).
+00002710: 720b 0000 0072 5900 0000 7266 0000 0072  r....rY...rf...r
+00002720: 1400 0000 7216 0000 0072 1600 0000 7217  ....r....r....r.
+00002730: 0000 0072 1a00 0000 2b01 0000 7302 0000  ...r....+...s...
+00002740: 001c 017a 1d53 335f 4275 636b 6574 5f46  ...z.S3_Bucket_F
+00002750: 6f6c 6465 725f 4669 6c65 2e5f 5f73 7472  older_File.__str
+00002760: 5f5f 7249 0000 0072 4a00 0000 720f 0000  __rI...rJ...r...
+00002770: 0063 0200 0000 0000 0000 0000 0000 0200  .c..............
+00002780: 0000 0500 0000 0300 0000 724b 0000 0029  ..........rK...)
+00002790: 024e 7269 0000 0072 4c00 0000 724f 0000  .Nri...rL...rO..
+000027a0: 0072 5000 0000 7216 0000 0072 1700 0000  .rP...r....r....
+000027b0: 7249 0000 002e 0100 0072 5200 0000 7a1e  rI.......rR...z.
+000027c0: 5333 5f42 7563 6b65 745f 466f 6c64 6572  S3_Bucket_Folder
+000027d0: 5f46 696c 652e 6765 745f 636f 7079 4e72  _File.get_copyNr
+000027e0: 2200 0000 7224 0000 0072 2500 0000 6304  "...r$...r%...c.
+000027f0: 0000 0000 0000 0000 0000 0004 0000 0006  ................
+00002800: 0000 0003 0000 00f3 1a00 0000 7400 8300  ............t...
+00002810: 6a01 7c01 7c00 6a02 7c02 7c03 6401 8d04  j.|.|.j.|.|.d...
+00002820: 0100 6400 5300 a902 4e29 0472 2200 0000  ..d.S...N).r"...
+00002830: 7288 0000 0072 2400 0000 7225 0000 0029  r....r$...r%...)
+00002840: 0372 4e00 0000 728b 0000 0072 6600 0000  .rN...r....rf...
+00002850: a904 7215 0000 0072 2200 0000 7224 0000  ..r....r"...r$..
+00002860: 0072 2500 0000 7250 0000 0072 1600 0000  .r%...rP...r....
+00002870: 7217 0000 00da 1575 706c 6f61 645f 7370  r......upload_sp
+00002880: 6563 6966 6965 645f 6669 6c65 3101 0000  ecified_file1...
+00002890: f30c 0000 0006 0602 0104 0102 0102 010a  ................
+000028a0: fc7a 2b53 335f 4275 636b 6574 5f46 6f6c  .z+S3_Bucket_Fol
+000028b0: 6465 725f 4669 6c65 2e75 706c 6f61 645f  der_File.upload_
+000028c0: 7370 6563 6966 6965 645f 6669 6c65 6304  specified_filec.
+000028d0: 0000 0000 0000 0000 0000 0004 0000 0006  ................
+000028e0: 0000 0003 0000 0072 9b00 0000 729c 0000  .......r....r...
+000028f0: 0029 0372 4e00 0000 728c 0000 0072 6600  .).rN...r....rf.
+00002900: 0000 729d 0000 0072 5000 0000 7216 0000  ..r....rP...r...
+00002910: 0072 1700 0000 da17 646f 776e 6c6f 6164  .r......download
+00002920: 5f73 7065 6369 6669 6564 5f66 696c 653e  _specified_file>
+00002930: 0100 0072 9f00 0000 7a2d 5333 5f42 7563  ...r....z-S3_Buc
+00002940: 6b65 745f 466f 6c64 6572 5f46 696c 652e  ket_Folder_File.
+00002950: 646f 776e 6c6f 6164 5f73 7065 6369 6669  download_specifi
+00002960: 6564 5f66 696c 6572 2300 0000 6302 0000  ed_filer#...c...
+00002970: 0000 0000 0000 0000 0002 0000 0003 0000  ................
+00002980: 0003 0000 0073 2800 0000 7c01 6400 7500  .....s(...|.d.u.
+00002990: 720d 7c00 6a00 9b00 6401 7c00 6a01 9b00  r.|.j...d.|.j...
+000029a0: 9d03 7d01 7402 8300 6a03 7c01 6402 8d01  ..}.t...j.|.d...
+000029b0: 5300 2903 4e72 8700 0000 7243 0000 0029  S.).Nr....rC...)
+000029c0: 0472 5900 0000 7266 0000 0072 4e00 0000  .rY...rf...rN...
+000029d0: 7236 0000 0072 3400 0000 7250 0000 0072  r6...r4...rP...r
+000029e0: 1600 0000 7217 0000 0072 3600 0000 4b01  ....r....r6...K.
+000029f0: 0000 7306 0000 0008 0112 010e 017a 2053  ..s..........z S
+00002a00: 335f 4275 636b 6574 5f46 6f6c 6465 725f  3_Bucket_Folder_
+00002a10: 4669 6c65 2e67 6574 5f6f 626a 6563 7472  File.get_objectr
+00002a20: 6100 0000 7253 0000 0063 0200 0000 0000  a...rS...c......
+00002a30: 0000 0000 0000 0300 0000 0300 0000 4300  ..............C.
+00002a40: 0000 731e 0000 0074 007c 006a 0183 017c  ..s....t.|.j...|
+00002a50: 006a 021b 007c 011b 007d 027c 00a0 037c  .j...|...}.|...|
+00002a60: 02a1 0153 0072 1100 0000 2904 7203 0000  ...S.r....).r...
+00002a70: 0072 5900 0000 7266 0000 0072 5700 0000  .rY...rf...rW...
+00002a80: 7292 0000 0072 1600 0000 7216 0000 0072  r....r....r....r
+00002a90: 1700 0000 7262 0000 0050 0100 0073 0400  ....rb...P...s..
+00002aa0: 0000 1404 0a01 7a21 5333 5f42 7563 6b65  ......z!S3_Bucke
+00002ab0: 745f 466f 6c64 6572 5f46 696c 652e 5f5f  t_Folder_File.__
+00002ac0: 7472 7565 6469 765f 5f72 6d00 0000 726b  truediv__rm...rk
+00002ad0: 0000 0072 1100 0000 2915 726f 0000 0072  ...r....).ro...r
+00002ae0: 7000 0000 7271 0000 0072 9900 0000 722b  p...rq...r....r+
+00002af0: 0000 0072 7200 0000 7208 0000 0072 9a00  ...rr...r....r..
+00002b00: 0000 721a 0000 0072 4900 0000 7274 0000  ..r....rI...rt..
+00002b10: 0072 0300 0000 7275 0000 0072 7600 0000  .r....ru...rv...
+00002b20: 7206 0000 0072 9e00 0000 72a0 0000 0072  r....r....r....r
+00002b30: 3600 0000 7204 0000 0072 6200 0000 727a  6...r....rb...rz
+00002b40: 0000 0072 1600 0000 7216 0000 0072 5000  ...r....r....rP.
+00002b50: 0000 7217 0000 0072 6900 0000 1a01 0000  ..r....ri.......
+00002b60: 733e 0000 000a 0004 0108 0406 030a 0108  s>..............
+00002b70: 0818 0302 0602 0104 fc0a 0202 fe06 0302  ................
+00002b80: fd06 040e fc02 1002 0104 fc0a 0202 fe06  ................
+00002b90: 0302 fd06 040e fc1c 0d02 050a 0102 ff02  ................
+00002ba0: 0212 fe72 6900 0000 6300 0000 0000 0000  ...ri...c.......
+00002bb0: 0000 0000 0000 0000 0009 0000 0000 0000  ................
+00002bc0: 0073 ae01 0000 6500 5a01 6400 5a02 5500  .s....e.Z.d.Z.U.
+00002bd0: 6401 5a03 6504 6505 6402 3c00 6506 6402  d.Z.e.e.d.<.e.d.
+00002be0: 8301 6403 6404 8400 8301 5a07 6405 6406  ..d.d.....Z.d.d.
+00002bf0: 8400 5a08 642e 6408 6504 6409 6400 6604  ..Z.d.d.e.d.d.f.
+00002c00: 8700 6601 640a 640b 840d 5a09 642f 640c  ..f.d.d...Z.d/d.
+00002c10: 640d 8404 5a0a 090e 090e 6430 640f 650b  d...Z.....d0d.e.
+00002c20: 6504 650c 6602 1900 6410 650d 650e 1900  e.e.f...d.e.e...
+00002c30: 6411 650d 650f 1900 6606 8700 6601 6412  d.e.e...f...f.d.
+00002c40: 6413 840d 5a10 090e 090e 0914 6431 640f  d...Z.......d1d.
+00002c50: 650b 6504 650c 6602 1900 6410 650d 650e  e.e.e.f...d.e.e.
+00002c60: 1900 6411 650d 650f 1900 6415 6511 6608  ..d.e.e...d.e.f.
+00002c70: 8700 6601 6416 6417 840d 5a12 6430 6402  ..f.d.d...Z.d0d.
+00002c80: 650b 6504 650c 6602 1900 6602 8700 6601  e.e.e.f...f...f.
+00002c90: 6418 6419 840d 5a13 6432 6402 650b 6504  d.d...Z.d2d.e.e.
+00002ca0: 650c 6602 1900 6409 6514 6504 1900 6604  e.f...d.e.e...f.
+00002cb0: 8700 6601 641a 641b 840d 5a15 6432 6402  ..f.d.d...Z.d2d.
+00002cc0: 650b 6504 650c 6602 1900 6409 6514 650c  e.e.e.f...d.e.e.
+00002cd0: 1900 6604 8700 6601 641c 641d 840d 5a16  ..f...f.d.d...Z.
+00002ce0: 6432 6402 650b 6504 650c 6602 1900 6409  d2d.e.e.e.f...d.
+00002cf0: 6517 641e 1900 6604 8700 6601 641f 6420  e.d...f...f.d.d 
+00002d00: 840d 5a18 6421 650b 6504 6519 6602 1900  ..Z.d!e.e.e.f...
+00002d10: 6409 6422 6604 6423 6424 8404 5a1a 6421  d.d"f.d#d$..Z.d!
+00002d20: 650b 6504 6519 6602 1900 6409 6422 6604  e.e.e.f...d.d"f.
+00002d30: 6425 6426 8404 5a1b 6427 650b 6504 6519  d%d&..Z.d'e.e.e.
+00002d40: 6602 1900 6409 6428 6604 6429 642a 8404  f...d.d(f.d)d*..
+00002d50: 5a1c 642b 650b 6504 6519 6602 1900 6409  Z.d+e.e.e.f...d.
+00002d60: 6400 6604 642c 642d 8404 5a1d 8700 0400  d.f.d,d-..Z.....
+00002d70: 5a1e 5300 2933 7253 0000 007a 960a 2020  Z.S.)3rS...z..  
+00002d80: 2020 5265 7072 6573 656e 7473 2061 2075    Represents a u
+00002d90: 6e69 7175 6520 6669 6c65 2028 6b65 7929  nique file (key)
+00002da0: 2077 6974 6869 6e20 616e 2053 3320 6275   within an S3 bu
+00002db0: 636b 6574 2e0a 2020 2020 5369 6d69 6c61  cket..    Simila
+00002dc0: 7220 746f 2053 335f 4275 636b 6574 5f46  r to S3_Bucket_F
+00002dd0: 6f6c 6465 725f 4669 6c65 2062 7574 2075  older_File but u
+00002de0: 7365 7320 6120 7369 6e67 6c65 206b 6579  ses a single key
+00002df0: 2069 6e73 7465 6164 206f 6620 666f 6c64   instead of fold
+00002e00: 6572 202b 2066 696c 655f 6e61 6d65 0a20  er + file_name. 
+00002e10: 2020 2072 2300 0000 6302 0000 0000 0000     r#...c.......
+00002e20: 0000 0000 0002 0000 0003 0000 0043 0000  .............C..
+00002e30: 0072 7b00 0000 2903 4e72 0100 0000 7a22  .r{...).Nr....z"
+00002e40: 5a65 726f 206c 656e 6774 6820 7374 7269  Zero length stri
+00002e50: 6e67 206e 6f74 2061 2076 616c 6964 206b  ng not a valid k
+00002e60: 6579 727c 0000 0072 8000 0000 7216 0000  eyr|...r....r...
+00002e70: 0072 1600 0000 7217 0000 00da 0c76 616c  .r....r......val
+00002e80: 6964 6174 655f 6b65 7960 0100 0072 8400  idate_key`...r..
+00002e90: 0000 7a1a 5333 5f42 7563 6b65 745f 4b65  ..z.S3_Bucket_Ke
+00002ea0: 792e 7661 6c69 6461 7465 5f6b 6579 6301  y.validate_keyc.
+00002eb0: 0000 0000 0000 0000 0000 0001 0000 0004  ................
+00002ec0: 0000 0043 0000 0072 8500 0000 7286 0000  ...C...r....r...
+00002ed0: 0029 0272 0b00 0000 7223 0000 0072 1400  .).r....r#...r..
+00002ee0: 0000 7216 0000 0072 1600 0000 7217 0000  ..r....r....r...
+00002ef0: 0072 1a00 0000 6901 0000 7237 0000 007a  .r....i...r7...z
+00002f00: 1553 335f 4275 636b 6574 5f4b 6579 2e5f  .S3_Bucket_Key._
+00002f10: 5f73 7472 5f5f 7249 0000 0072 4a00 0000  _str__rI...rJ...
+00002f20: 720f 0000 0063 0200 0000 0000 0000 0000  r....c..........
+00002f30: 0000 0200 0000 0500 0000 0300 0000 724b  ..............rK
+00002f40: 0000 0029 024e 7253 0000 0072 4c00 0000  ...).NrS...rL...
+00002f50: 724f 0000 0072 5000 0000 7216 0000 0072  rO...rP...r....r
+00002f60: 1700 0000 7249 0000 006c 0100 0072 5200  ....rI...l...rR.
+00002f70: 0000 7a16 5333 5f42 7563 6b65 745f 4b65  ..z.S3_Bucket_Ke
+00002f80: 792e 6765 745f 636f 7079 6302 0000 0000  y.get_copyc.....
+00002f90: 0000 0000 0000 0002 0000 0003 0000 0043  ...............C
+00002fa0: 0000 0072 5400 0000 7211 0000 0072 5500  ...rT...r....rU.
+00002fb0: 0000 7234 0000 0072 1600 0000 7216 0000  ..r4...r....r...
+00002fc0: 0072 1700 0000 7257 0000 006f 0100 0072  .r....rW...o...r
+00002fd0: 5800 0000 7a18 5333 5f42 7563 6b65 745f  X...z.S3_Bucket_
+00002fe0: 4b65 792e 6e61 765f 746f 5f6b 6579 4e72  Key.nav_to_keyNr
+00002ff0: 2200 0000 7224 0000 0072 2500 0000 6304  "...r$...r%...c.
+00003000: 0000 0000 0000 0000 0000 0004 0000 0006  ................
+00003010: 0000 0003 0000 0072 9b00 0000 7289 0000  .......r....r...
+00003020: 0029 0372 4e00 0000 722a 0000 0072 2300  .).rN...r*...r#.
+00003030: 0000 729d 0000 0072 5000 0000 7216 0000  ..r....rP...r...
+00003040: 0072 1700 0000 729e 0000 0072 0100 0072  .r....r....r...r
+00003050: 9f00 0000 7a23 5333 5f42 7563 6b65 745f  ....z#S3_Bucket_
+00003060: 4b65 792e 7570 6c6f 6164 5f73 7065 6369  Key.upload_speci
+00003070: 6669 6564 5f66 696c 6554 722c 0000 0063  fied_fileTr,...c
+00003080: 0500 0000 0000 0000 0000 0000 0500 0000  ................
+00003090: 0700 0000 0300 0000 731c 0000 0074 0083  ........s....t..
+000030a0: 006a 017c 017c 006a 027c 027c 037c 0464  .j.|.|.j.|.|.|.d
+000030b0: 018d 0501 0064 0053 0029 024e 2905 7222  .....d.S.).N).r"
+000030c0: 0000 0072 2300 0000 7224 0000 0072 2500  ...r#...r$...r%.
+000030d0: 0000 722c 0000 0029 0372 4e00 0000 7231  ..r,...).rN...r1
+000030e0: 0000 0072 2300 0000 2905 7215 0000 0072  ...r#...).r....r
+000030f0: 2200 0000 7224 0000 0072 2500 0000 722c  "...r$...r%...r,
+00003100: 0000 0072 5000 0000 7216 0000 0072 1700  ...rP...r....r..
+00003110: 0000 72a0 0000 007f 0100 0073 0e00 0000  ..r........s....
+00003120: 0607 0201 0401 0201 0201 0201 0afb 7a25  ..............z%
+00003130: 5333 5f42 7563 6b65 745f 4b65 792e 646f  S3_Bucket_Key.do
+00003140: 776e 6c6f 6164 5f73 7065 6369 6669 6564  wnload_specified
+00003150: 5f66 696c 6563 0300 0000 0000 0000 0000  _filec..........
+00003160: 0000 0300 0000 0300 0000 0300 0000 7294  ..............r.
+00003170: 0000 0072 9500 0000 2903 7223 0000 0072  ...r....).r#...r
+00003180: 4e00 0000 7236 0000 0029 0372 1500 0000  N...r6...).r....
+00003190: 7223 0000 0072 3800 0000 7250 0000 0072  r#...r8...rP...r
+000031a0: 1600 0000 7217 0000 0072 3600 0000 8e01  ....r....r6.....
+000031b0: 0000 7296 0000 007a 1853 335f 4275 636b  ..r....z.S3_Buck
+000031c0: 6574 5f4b 6579 2e67 6574 5f6f 626a 6563  et_Key.get_objec
+000031d0: 7463 0200 0000 0000 0000 0000 0000 0200  tc..............
+000031e0: 0000 0300 0000 0300 0000 7294 0000 0072  ..........r....r
+000031f0: 9500 0000 2903 7223 0000 0072 4e00 0000  ....).r#...rN...
+00003200: 7247 0000 0072 3400 0000 7250 0000 0072  rG...r4...rP...r
+00003210: 1600 0000 7217 0000 0072 4700 0000 9301  ....r....rG.....
+00003220: 0000 7296 0000 007a 1e53 335f 4275 636b  ..r....z.S3_Buck
+00003230: 6574 5f4b 6579 2e6c 6973 745f 6f62 6a65  et_Key.list_obje
+00003240: 6374 5f6b 6579 7363 0200 0000 0000 0000  ct_keysc........
+00003250: 0000 0000 0200 0000 0300 0000 0300 0000  ................
+00003260: 7294 0000 0072 9500 0000 2903 7223 0000  r....r....).r#..
+00003270: 0072 4e00 0000 7248 0000 0072 3400 0000  .rN...rH...r4...
+00003280: 7250 0000 0072 1600 0000 7217 0000 0072  rP...r....r....r
+00003290: 4800 0000 9801 0000 7296 0000 007a 1f53  H.......r....z.S
+000032a0: 335f 4275 636b 6574 5f4b 6579 2e6c 6973  3_Bucket_Key.lis
+000032b0: 745f 6f62 6a65 6374 5f70 6174 6873 723c  t_object_pathsr<
+000032c0: 0000 0063 0200 0000 0000 0000 0000 0000  ...c............
+000032d0: 0200 0000 0300 0000 0300 0000 7297 0000  ............r...
+000032e0: 0072 1100 0000 2903 7223 0000 0072 4e00  .r....).r#...rN.
+000032f0: 0000 7242 0000 0072 3400 0000 7250 0000  ..rB...r4...rP..
+00003300: 0072 1600 0000 7217 0000 0072 4200 0000  .r....r....rB...
+00003310: 9d01 0000 7298 0000 007a 1a53 335f 4275  ....r....z.S3_Bu
+00003320: 636b 6574 5f4b 6579 2e66 696e 645f 6f62  cket_Key.find_ob
+00003330: 6a65 6374 7372 5900 0000 725a 0000 0063  jectsrY...rZ...c
+00003340: 0200 0000 0000 0000 0000 0000 0200 0000  ................
+00003350: 0300 0000 4300 0000 7254 0000 0072 1100  ....C...rT...r..
+00003360: 0000 725b 0000 0072 5d00 0000 7216 0000  ..r[...r]...r...
+00003370: 0072 1600 0000 7217 0000 0072 5e00 0000  .r....r....r^...
+00003380: a201 0000 725f 0000 007a 1b53 335f 4275  ....r_...z.S3_Bu
+00003390: 636b 6574 5f4b 6579 2e6e 6176 5f74 6f5f  cket_Key.nav_to_
+000033a0: 666f 6c64 6572 6302 0000 0000 0000 0000  folderc.........
+000033b0: 0000 0003 0000 0003 0000 0043 0000 0072  ...........C...r
+000033c0: 8e00 0000 7211 0000 0029 0372 0300 0000  ....r....).r....
+000033d0: 7223 0000 0072 5e00 0000 728f 0000 0072  r#...r^...r....r
+000033e0: 1600 0000 7216 0000 0072 1700 0000 7260  ....r....r....r`
+000033f0: 0000 00a8 0100 0073 0400 0000 0e04 0a01  .......s........
+00003400: 7a24 5333 5f42 7563 6b65 745f 4b65 792e  z$S3_Bucket_Key.
+00003410: 6e61 765f 746f 5f72 656c 6174 6976 655f  nav_to_relative_
+00003420: 666f 6c64 6572 7266 0000 0072 6900 0000  folderrf...ri...
+00003430: 6302 0000 0000 0000 0000 0000 0002 0000  c...............
+00003440: 0004 0000 0043 0000 0073 1000 0000 7c00  .....C...s....|.
+00003450: 6a00 7c00 6a01 7c01 6401 8d02 5300 2902  j.|.j.|.d...S.).
+00003460: 4e29 0272 5900 0000 7266 0000 0029 0272  N).rY...rf...).r
+00003470: 6a00 0000 7223 0000 0072 9000 0000 7216  j...r#...r....r.
+00003480: 0000 0072 1600 0000 7217 0000 0072 9100  ...r....r....r..
+00003490: 0000 af01 0000 7308 0000 0004 0404 0102  ......s.........
+000034a0: 0106 fe7a 1953 335f 4275 636b 6574 5f4b  ...z.S3_Bucket_K
+000034b0: 6579 2e6e 6176 5f74 6f5f 6669 6c65 7261  ey.nav_to_filera
+000034c0: 0000 0063 0200 0000 0000 0000 0000 0000  ...c............
+000034d0: 0300 0000 0300 0000 4300 0000 728e 0000  ........C...r...
+000034e0: 0072 1100 0000 2903 7203 0000 0072 2300  .r....).r....r#.
+000034f0: 0000 7257 0000 0072 9200 0000 7216 0000  ..rW...r....r...
+00003500: 0072 1600 0000 7217 0000 0072 6200 0000  .r....r....rb...
+00003510: b801 0000 7293 0000 007a 1953 335f 4275  ....r....z.S3_Bu
+00003520: 636b 6574 5f4b 6579 2e5f 5f74 7275 6564  cket_Key.__trued
+00003530: 6976 5f5f 726d 0000 0072 6e00 0000 726b  iv__rm...rn...rk
+00003540: 0000 0072 6c00 0000 7211 0000 0029 1f72  ...rl...r....).r
+00003550: 6f00 0000 7270 0000 0072 7100 0000 7299  o...rp...rq...r.
+00003560: 0000 0072 2b00 0000 7272 0000 0072 0800  ...r+...rr...r..
+00003570: 0000 72a1 0000 0072 1a00 0000 7249 0000  ..r....r....rI..
+00003580: 0072 5700 0000 7274 0000 0072 0300 0000  .rW...rt...r....
+00003590: 7275 0000 0072 7600 0000 7206 0000 0072  ru...rv...r....r
+000035a0: 9e00 0000 7277 0000 0072 a000 0000 7236  ....rw...r....r6
+000035b0: 0000 0072 7900 0000 7247 0000 0072 4800  ...ry...rG...rH.
+000035c0: 0000 7278 0000 0072 4200 0000 7204 0000  ..rx...rB...r...
+000035d0: 0072 5e00 0000 7260 0000 0072 9100 0000  .r^...r`...r....
+000035e0: 7262 0000 0072 7a00 0000 7216 0000 0072  rb...rz...r....r
+000035f0: 1600 0000 7250 0000 0072 1700 0000 7253  ....rP...r....rS
+00003600: 0000 0058 0100 0073 6a00 0000 0a00 0401  ...X...sj.......
+00003610: 0804 0603 0a01 0808 1803 0a03 0206 0201  ................
+00003620: 04fc 0a02 02fe 0603 02fd 0604 0efc 0210  ................
+00003630: 0201 0201 04fb 0a02 02fe 0603 02fd 0604  ................
+00003640: 02fc 0205 0efb 1c0f 2405 2405 2405 0205  ........$.$.$...
+00003650: 0a02 02fe 0203 0afd 0206 0a02 02fe 0203  ................
+00003660: 0afd 0207 0a02 02fe 0203 0afd 0209 0a01  ................
+00003670: 02ff 0202 12fe 7253 0000 0029 15da 0966  ......rS...)...f
+00003680: 756e 6374 6f6f 6c73 7202 0000 00da 0770  unctoolsr......p
+00003690: 6174 686c 6962 7203 0000 0072 0400 0000  athlibr....r....
+000036a0: da06 7479 7069 6e67 5a11 626f 746f 332e  ..typingZ.boto3.
+000036b0: 7333 2e74 7261 6e73 6665 7272 0600 0000  s3.transferr....
+000036c0: da08 7079 6461 6e74 6963 7207 0000 0072  ..pydanticr....r
+000036d0: 0800 0000 5a30 636f 6e66 6967 5f77 7261  ....Z0config_wra
+000036e0: 6e67 6c65 722e 636f 6e66 6967 5f74 656d  ngler.config_tem
+000036f0: 706c 6174 6573 2e61 7773 2e61 7773 5f73  plates.aws.aws_s
+00003700: 6573 7369 6f6e 7209 0000 00da 0562 6f74  essionr......bot
+00003710: 6f33 da0b 496d 706f 7274 4572 726f 72da  o3..ImportError.
+00003720: 0d54 5950 455f 4348 4543 4b49 4e47 5a09  .TYPE_CHECKINGZ.
+00003730: 626f 746f 7374 7562 7372 0a00 0000 725a  botostubsr....rZ
+00003740: 0000 0072 6900 0000 7253 0000 0072 1600  ...ri...rS...r..
+00003750: 0000 7216 0000 0072 1600 0000 7217 0000  ..r....r....r...
+00003760: 00da 083c 6d6f 6475 6c65 3e01 0000 0073  ...<module>....s
+00003770: 2c00 0000 0c00 1001 0801 0c02 1001 0c02  ,...............
+00003780: 0202 0c01 0c01 0801 02ff 0403 0201 0c01  ................
+00003790: 0c01 0801 02ff 100b 007f 1023 105b 143e  ...........#.[.>
```

### Comparing `config_wrangler-0.5.4a0/config_wrangler/config_templates/aws/__pycache__/s3_bucket.cpython-311.pyc` & `config_wrangler-0.5.5/config_wrangler/config_templates/aws/__pycache__/s3_bucket.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `config_wrangler-0.5.4a0/config_wrangler/config_templates/aws/aws_session.py` & `config_wrangler-0.5.5/config_wrangler/config_templates/aws/aws_session.py`

 * *Files identical despite different names*

### Comparing `config_wrangler-0.5.4a0/config_wrangler/config_templates/aws/dynamodb.py` & `config_wrangler-0.5.5/config_wrangler/config_templates/aws/dynamodb.py`

 * *Files identical despite different names*

### Comparing `config_wrangler-0.5.4a0/config_wrangler/config_templates/aws/s3_bucket.py` & `config_wrangler-0.5.5/config_wrangler/config_templates/aws/s3_bucket.py`

 * *Files 0% similar despite different names*

```diff
@@ -62,15 +62,15 @@
             self,
             local_filename: Union[str, Path],
             key: Union[str, PurePosixPath],
             extra_args: Optional[dict] = None,
             transfer_config: Optional[TransferConfig] = None,
     ):
         if transfer_config is None:
-            transfer_config = TransferConfig(multipart_threshold=5* (1024**3)) # 5 GB
+            transfer_config = TransferConfig(multipart_threshold=5* (1024**3))  # 5 GB
 
         self.client.upload_file(
             Filename=str(local_filename),
             Bucket=self.bucket_name,
             Key=str(key),
             ExtraArgs=extra_args,
             Config=transfer_config,
```

### Comparing `config_wrangler-0.5.4a0/config_wrangler/config_templates/config_hierarchy.py` & `config_wrangler-0.5.5/config_wrangler/config_templates/config_hierarchy.py`

 * *Files identical despite different names*

### Comparing `config_wrangler-0.5.4a0/config_wrangler/config_templates/credentials.py` & `config_wrangler-0.5.5/config_wrangler/config_templates/credentials.py`

 * *Files identical despite different names*

### Comparing `config_wrangler-0.5.4a0/config_wrangler/config_templates/keepass_config.py` & `config_wrangler-0.5.5/config_wrangler/config_templates/keepass_config.py`

 * *Files identical despite different names*

### Comparing `config_wrangler-0.5.4a0/config_wrangler/config_templates/logging_config.py` & `config_wrangler-0.5.5/config_wrangler/config_templates/logging_config.py`

 * *Files identical despite different names*

### Comparing `config_wrangler-0.5.4a0/config_wrangler/config_templates/password_defaults.py` & `config_wrangler-0.5.5/config_wrangler/config_templates/password_defaults.py`

 * *Files identical despite different names*

### Comparing `config_wrangler-0.5.4a0/config_wrangler/config_templates/sqlalchemy_database.py` & `config_wrangler-0.5.5/config_wrangler/config_templates/sqlalchemy_database.py`

 * *Files identical despite different names*

### Comparing `config_wrangler-0.5.4a0/config_wrangler/config_types/__pycache__/dynamically_referenced.cpython-310.pyc` & `config_wrangler-0.5.5/config_wrangler/config_types/__pycache__/dynamically_referenced.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `config_wrangler-0.5.4a0/config_wrangler/config_types/__pycache__/dynamically_referenced.cpython-311.pyc` & `config_wrangler-0.5.5/config_wrangler/config_types/__pycache__/dynamically_referenced.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `config_wrangler-0.5.4a0/config_wrangler/config_types/__pycache__/path_types.cpython-310.pyc` & `config_wrangler-0.5.5/config_wrangler/config_types/__pycache__/path_types.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `config_wrangler-0.5.4a0/config_wrangler/config_types/__pycache__/path_types.cpython-311.pyc` & `config_wrangler-0.5.5/config_wrangler/config_types/__pycache__/path_types.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `config_wrangler-0.5.4a0/config_wrangler/config_types/dynamically_referenced.py` & `config_wrangler-0.5.5/config_wrangler/config_types/dynamically_referenced.py`

 * *Files identical despite different names*

### Comparing `config_wrangler-0.5.4a0/config_wrangler/config_types/path_types.py` & `config_wrangler-0.5.5/config_wrangler/config_types/path_types.py`

 * *Files identical despite different names*

### Comparing `config_wrangler-0.5.4a0/config_wrangler/utils.py` & `config_wrangler-0.5.5/config_wrangler/utils.py`

 * *Files identical despite different names*

### Comparing `config_wrangler-0.5.4a0/LICENSE` & `config_wrangler-0.5.5/LICENSE`

 * *Files identical despite different names*

### Comparing `config_wrangler-0.5.4a0/LICENSE.txt` & `config_wrangler-0.5.5/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `config_wrangler-0.5.4a0/pyproject.toml` & `config_wrangler-0.5.5/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 [tool.poetry]
 name = "config_wrangler"
-version = "0.5.4a"
+version = "0.5.5"
 license = "MIT"
 authors = ["Derek Wood"]
 description = "pydantic based configuration wrangler. Handles reading multiple ini or toml files with inheritance rules and variable expansions."
 readme = "README.md"
 repository = "https://github.com/arcann/config_wrangler"
 
 
 [tool.poetry.dependencies]
 python = ">=3.7, <4.0.0"
-pydantic = ">=1.8.2"
+pydantic = "^1.10.11"
 StrEnum = "^0.4.7"
 SQLAlchemy = {version = ">=1.4", optional = true}
 boto3 = {version = ">=1.21", optional = true}
 pykeepass = {version = ">=4.0.0", optional = true}
 auto-all = "^1.4.1"
 pydicti = "^1.1.6"
```

### Comparing `config_wrangler-0.5.4a0/README.md` & `config_wrangler-0.5.5/README.md`

 * *Files identical despite different names*

### Comparing `config_wrangler-0.5.4a0/PKG-INFO` & `config_wrangler-0.5.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: config-wrangler
-Version: 0.5.4a0
+Version: 0.5.5
 Summary: pydantic based configuration wrangler. Handles reading multiple ini or toml files with inheritance rules and variable expansions.
 Home-page: https://github.com/arcann/config_wrangler
 License: MIT
 Author: Derek Wood
 Requires-Python: >=3.7,<4.0.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
@@ -17,15 +17,15 @@
 Provides-Extra: redshift
 Provides-Extra: s3
 Provides-Extra: sqlalchemy
 Requires-Dist: SQLAlchemy (>=1.4) ; extra == "sqlalchemy"
 Requires-Dist: StrEnum (>=0.4.7,<0.5.0)
 Requires-Dist: auto-all (>=1.4.1,<2.0.0)
 Requires-Dist: boto3 (>=1.21) ; extra == "redshift" or extra == "s3"
-Requires-Dist: pydantic (>=1.8.2)
+Requires-Dist: pydantic (>=1.10.11,<2.0.0)
 Requires-Dist: pydicti (>=1.1.6,<2.0.0)
 Requires-Dist: pykeepass (>=4.0.0) ; extra == "pykeepass"
 Project-URL: Repository, https://github.com/arcann/config_wrangler
 Description-Content-Type: text/markdown
 
 # Config Wrangler
```

