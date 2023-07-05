# Comparing `tmp/mui_data_grid-0.8.4.tar.gz` & `tmp/mui_data_grid-0.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mui_data_grid-0.8.4.tar", max compression
+gzip compressed data, was "mui_data_grid-0.9.0.tar", max compression
```

## Comparing `mui_data_grid-0.8.4.tar` & `mui_data_grid-0.9.0.tar`

### file list

```diff
@@ -1,60 +1,113 @@
--rw-r--r--   0        0        0     1070 2022-12-16 13:41:12.116958 mui_data_grid-0.8.4/LICENSE
--rw-r--r--   0        0        0     3216 2022-12-16 13:41:12.117211 mui_data_grid-0.8.4/README.md
--rw-r--r--   0        0        0     2671 2023-03-10 20:18:46.559541 mui_data_grid-0.8.4/pyproject.toml
--rw-r--r--   0        0        0       58 2022-12-16 13:41:12.119860 mui_data_grid-0.8.4/src/mui/__init__.py
--rw-r--r--   0        0        0     1430 2022-12-16 13:41:12.120182 mui_data_grid-0.8.4/src/mui/compat.py
--rw-r--r--   0        0        0        0 2022-12-16 13:41:12.120319 mui_data_grid-0.8.4/src/mui/py.typed
--rw-r--r--   0        0        0     1554 2022-12-16 13:41:12.120737 mui_data_grid-0.8.4/src/mui/v5/__init__.py
--rw-r--r--   0        0        0     1526 2022-12-16 13:41:12.121179 mui_data_grid-0.8.4/src/mui/v5/grid/__init__.py
--rw-r--r--   0        0        0     2359 2022-12-16 13:41:12.121488 mui_data_grid-0.8.4/src/mui/v5/grid/base.py
--rw-r--r--   0        0        0     1134 2022-12-16 13:41:12.122018 mui_data_grid-0.8.4/src/mui/v5/grid/filter/__init__.py
--rw-r--r--   0        0        0     4474 2022-12-16 13:41:12.122325 mui_data_grid-0.8.4/src/mui/v5/grid/filter/item.py
--rw-r--r--   0        0        0     6267 2022-12-16 13:41:12.122600 mui_data_grid-0.8.4/src/mui/v5/grid/filter/model.py
--rw-r--r--   0        0        0      162 2022-12-16 13:41:12.123028 mui_data_grid-0.8.4/src/mui/v5/grid/link/__init__.py
--rw-r--r--   0        0        0      661 2022-12-16 13:41:12.123324 mui_data_grid-0.8.4/src/mui/v5/grid/link/operator.py
--rw-r--r--   0        0        0      117 2022-12-16 13:41:12.123739 mui_data_grid-0.8.4/src/mui/v5/grid/pagination/__init__.py
--rw-r--r--   0        0        0     1231 2022-12-16 13:41:12.124037 mui_data_grid-0.8.4/src/mui/v5/grid/pagination/model.py
--rw-r--r--   0        0        0     3499 2023-03-10 20:16:36.216380 mui_data_grid-0.8.4/src/mui/v5/grid/request.py
--rw-r--r--   0        0        0      387 2022-12-16 13:41:12.124855 mui_data_grid-0.8.4/src/mui/v5/grid/sort/__init__.py
--rw-r--r--   0        0        0      453 2022-12-16 13:41:12.125197 mui_data_grid-0.8.4/src/mui/v5/grid/sort/direction.py
--rw-r--r--   0        0        0     1212 2022-12-16 13:41:12.125571 mui_data_grid-0.8.4/src/mui/v5/grid/sort/item.py
--rw-r--r--   0        0        0      444 2022-12-16 13:41:12.125882 mui_data_grid-0.8.4/src/mui/v5/grid/sort/model.py
--rw-r--r--   0        0        0      218 2022-12-16 13:41:12.126568 mui_data_grid-0.8.4/src/mui/v5/integrations/__init__.py
--rw-r--r--   0        0        0      658 2022-12-16 13:41:12.127271 mui_data_grid-0.8.4/src/mui/v5/integrations/flask/__init__.py
--rw-r--r--   0        0        0      230 2022-12-16 13:41:12.128102 mui_data_grid-0.8.4/src/mui/v5/integrations/flask/filter/__init__.py
--rw-r--r--   0        0        0     1611 2022-12-16 13:41:12.128507 mui_data_grid-0.8.4/src/mui/v5/integrations/flask/filter/model.py
--rw-r--r--   0        0        0      259 2022-12-16 13:41:12.129079 mui_data_grid-0.8.4/src/mui/v5/integrations/flask/pagination/__init__.py
--rw-r--r--   0        0        0     1958 2022-12-16 13:41:12.129532 mui_data_grid-0.8.4/src/mui/v5/integrations/flask/pagination/model.py
--rw-r--r--   0        0        0     2661 2023-03-10 20:16:36.217171 mui_data_grid-0.8.4/src/mui/v5/integrations/flask/request.py
--rw-r--r--   0        0        0      220 2022-12-16 13:41:12.130650 mui_data_grid-0.8.4/src/mui/v5/integrations/flask/sort/__init__.py
--rw-r--r--   0        0        0     1370 2022-12-16 13:41:12.131021 mui_data_grid-0.8.4/src/mui/v5/integrations/flask/sort/model.py
--rw-r--r--   0        0        0      988 2022-12-16 13:41:12.131975 mui_data_grid-0.8.4/src/mui/v5/integrations/sqlalchemy/__init__.py
--rw-r--r--   0        0        0     3428 2022-12-16 13:41:12.132431 mui_data_grid-0.8.4/src/mui/v5/integrations/sqlalchemy/apply_models.py
--rw-r--r--   0        0        0      325 2022-12-16 13:41:12.133123 mui_data_grid-0.8.4/src/mui/v5/integrations/sqlalchemy/filter/__init__.py
--rw-r--r--   0        0        0     2029 2022-12-16 13:41:12.133929 mui_data_grid-0.8.4/src/mui/v5/integrations/sqlalchemy/filter/applicators/__init__.py
--rw-r--r--   0        0        0      753 2022-12-16 14:16:39.831140 mui_data_grid-0.8.4/src/mui/v5/integrations/sqlalchemy/filter/applicators/after.py
--rw-r--r--   0        0        0     2446 2022-12-16 13:41:12.134812 mui_data_grid-0.8.4/src/mui/v5/integrations/sqlalchemy/filter/applicators/basic.py
--rw-r--r--   0        0        0      756 2022-12-16 14:16:39.832139 mui_data_grid-0.8.4/src/mui/v5/integrations/sqlalchemy/filter/applicators/before.py
--rw-r--r--   0        0        0      969 2022-12-16 13:41:12.135652 mui_data_grid-0.8.4/src/mui/v5/integrations/sqlalchemy/filter/applicators/contains.py
--rw-r--r--   0        0        0      999 2022-12-16 13:41:12.136052 mui_data_grid-0.8.4/src/mui/v5/integrations/sqlalchemy/filter/applicators/endswith.py
--rw-r--r--   0        0        0     1273 2023-03-10 20:18:46.560787 mui_data_grid-0.8.4/src/mui/v5/integrations/sqlalchemy/filter/applicators/is_.py
--rw-r--r--   0        0        0     1118 2022-12-16 13:41:12.136923 mui_data_grid-0.8.4/src/mui/v5/integrations/sqlalchemy/filter/applicators/is_any_of.py
--rw-r--r--   0        0        0      603 2022-12-16 13:41:12.137363 mui_data_grid-0.8.4/src/mui/v5/integrations/sqlalchemy/filter/applicators/is_empty.py
--rw-r--r--   0        0        0      627 2022-12-16 13:41:12.137870 mui_data_grid-0.8.4/src/mui/v5/integrations/sqlalchemy/filter/applicators/is_not_empty.py
--rw-r--r--   0        0        0      848 2023-03-10 20:18:46.562123 mui_data_grid-0.8.4/src/mui/v5/integrations/sqlalchemy/filter/applicators/not_.py
--rw-r--r--   0        0        0      801 2022-12-16 14:16:39.834164 mui_data_grid-0.8.4/src/mui/v5/integrations/sqlalchemy/filter/applicators/on_or_after.py
--rw-r--r--   0        0        0      793 2022-12-16 14:16:39.835013 mui_data_grid-0.8.4/src/mui/v5/integrations/sqlalchemy/filter/applicators/on_or_before.py
--rw-r--r--   0        0        0     1015 2022-12-16 13:41:12.139884 mui_data_grid-0.8.4/src/mui/v5/integrations/sqlalchemy/filter/applicators/startswith.py
--rw-r--r--   0        0        0     5917 2023-03-09 14:32:27.748800 mui_data_grid-0.8.4/src/mui/v5/integrations/sqlalchemy/filter/apply_items.py
--rw-r--r--   0        0        0     1098 2023-03-09 14:32:27.749964 mui_data_grid-0.8.4/src/mui/v5/integrations/sqlalchemy/filter/apply_model.py
--rw-r--r--   0        0        0      189 2022-12-16 13:41:12.141613 mui_data_grid-0.8.4/src/mui/v5/integrations/sqlalchemy/pagination/__init__.py
--rw-r--r--   0        0        0      733 2023-03-09 14:32:27.750630 mui_data_grid-0.8.4/src/mui/v5/integrations/sqlalchemy/pagination/apply_model.py
--rw-r--r--   0        0        0      299 2022-12-16 13:41:12.143027 mui_data_grid-0.8.4/src/mui/v5/integrations/sqlalchemy/resolver/__init__.py
--rw-r--r--   0        0        0      305 2022-12-16 13:41:12.143414 mui_data_grid-0.8.4/src/mui/v5/integrations/sqlalchemy/resolver/types.py
--rw-r--r--   0        0        0      289 2022-12-16 13:41:12.144320 mui_data_grid-0.8.4/src/mui/v5/integrations/sqlalchemy/sort/__init__.py
--rw-r--r--   0        0        0     3007 2022-12-21 14:34:26.459733 mui_data_grid-0.8.4/src/mui/v5/integrations/sqlalchemy/sort/apply_item.py
--rw-r--r--   0        0        0     1792 2023-03-09 14:32:27.751840 mui_data_grid-0.8.4/src/mui/v5/integrations/sqlalchemy/sort/apply_model.py
--rw-r--r--   0        0        0      124 2022-12-16 13:41:12.146599 mui_data_grid-0.8.4/src/mui/v5/integrations/sqlalchemy/structures/__init__.py
--rw-r--r--   0        0        0      444 2022-12-16 13:41:12.147306 mui_data_grid-0.8.4/src/mui/v5/integrations/sqlalchemy/structures/factory.py
--rw-r--r--   0        0        0     7010 2022-12-16 13:41:12.147943 mui_data_grid-0.8.4/src/mui/v5/integrations/sqlalchemy/structures/query.py
--rw-r--r--   0        0        0     4051 1970-01-01 00:00:00.000000 mui_data_grid-0.8.4/PKG-INFO
+-rw-r--r--   0        0        0     1070 2023-07-05 13:16:29.903135 mui_data_grid-0.9.0/LICENSE
+-rw-r--r--   0        0        0     3216 2023-07-05 18:05:48.395835 mui_data_grid-0.9.0/README.md
+-rw-r--r--   0        0        0     2675 2023-07-05 18:31:58.275810 mui_data_grid-0.9.0/pyproject.toml
+-rw-r--r--   0        0        0       68 2023-07-05 18:31:58.277363 mui_data_grid-0.9.0/src/mui/__init__.py
+-rw-r--r--   0        0        0     1430 2023-07-05 13:16:29.906834 mui_data_grid-0.9.0/src/mui/compat.py
+-rw-r--r--   0        0        0        0 2023-07-05 13:16:29.906993 mui_data_grid-0.9.0/src/mui/py.typed
+-rw-r--r--   0        0        0     1554 2023-07-05 13:16:29.907512 mui_data_grid-0.9.0/src/mui/v5/__init__.py
+-rw-r--r--   0        0        0     1526 2023-07-05 13:16:29.908207 mui_data_grid-0.9.0/src/mui/v5/grid/__init__.py
+-rw-r--r--   0        0        0     2359 2023-07-05 18:05:48.401211 mui_data_grid-0.9.0/src/mui/v5/grid/base.py
+-rw-r--r--   0        0        0     1134 2023-07-05 13:16:29.909930 mui_data_grid-0.9.0/src/mui/v5/grid/filter/__init__.py
+-rw-r--r--   0        0        0     4474 2023-07-05 13:16:29.910360 mui_data_grid-0.9.0/src/mui/v5/grid/filter/item.py
+-rw-r--r--   0        0        0     6267 2023-07-05 13:16:29.910782 mui_data_grid-0.9.0/src/mui/v5/grid/filter/model.py
+-rw-r--r--   0        0        0      162 2023-07-05 13:16:29.911536 mui_data_grid-0.9.0/src/mui/v5/grid/link/__init__.py
+-rw-r--r--   0        0        0      661 2023-07-05 15:10:27.942870 mui_data_grid-0.9.0/src/mui/v5/grid/link/operator.py
+-rw-r--r--   0        0        0      117 2023-07-05 13:16:29.912614 mui_data_grid-0.9.0/src/mui/v5/grid/pagination/__init__.py
+-rw-r--r--   0        0        0     1231 2023-07-05 18:05:48.401651 mui_data_grid-0.9.0/src/mui/v5/grid/pagination/model.py
+-rw-r--r--   0        0        0     3499 2023-07-05 18:05:48.402057 mui_data_grid-0.9.0/src/mui/v5/grid/request.py
+-rw-r--r--   0        0        0      387 2023-07-05 13:16:29.913626 mui_data_grid-0.9.0/src/mui/v5/grid/sort/__init__.py
+-rw-r--r--   0        0        0      453 2023-07-05 13:16:29.913926 mui_data_grid-0.9.0/src/mui/v5/grid/sort/direction.py
+-rw-r--r--   0        0        0     1212 2023-07-05 13:16:29.914186 mui_data_grid-0.9.0/src/mui/v5/grid/sort/item.py
+-rw-r--r--   0        0        0      444 2023-07-05 13:16:29.914487 mui_data_grid-0.9.0/src/mui/v5/grid/sort/model.py
+-rw-r--r--   0        0        0      218 2023-07-05 13:16:29.915006 mui_data_grid-0.9.0/src/mui/v5/integrations/__init__.py
+-rw-r--r--   0        0        0      658 2023-07-05 13:16:29.915468 mui_data_grid-0.9.0/src/mui/v5/integrations/flask/__init__.py
+-rw-r--r--   0        0        0      230 2023-07-05 13:16:29.915811 mui_data_grid-0.9.0/src/mui/v5/integrations/flask/filter/__init__.py
+-rw-r--r--   0        0        0     1611 2023-07-05 18:05:48.403355 mui_data_grid-0.9.0/src/mui/v5/integrations/flask/filter/model.py
+-rw-r--r--   0        0        0      259 2023-07-05 13:16:29.916458 mui_data_grid-0.9.0/src/mui/v5/integrations/flask/pagination/__init__.py
+-rw-r--r--   0        0        0     1958 2023-07-05 18:05:48.404565 mui_data_grid-0.9.0/src/mui/v5/integrations/flask/pagination/model.py
+-rw-r--r--   0        0        0     2661 2023-07-05 13:16:29.917015 mui_data_grid-0.9.0/src/mui/v5/integrations/flask/request.py
+-rw-r--r--   0        0        0      220 2023-07-05 13:16:29.917494 mui_data_grid-0.9.0/src/mui/v5/integrations/flask/sort/__init__.py
+-rw-r--r--   0        0        0     1370 2023-07-05 18:05:48.406203 mui_data_grid-0.9.0/src/mui/v5/integrations/flask/sort/model.py
+-rw-r--r--   0        0        0      988 2023-07-05 13:16:29.918281 mui_data_grid-0.9.0/src/mui/v5/integrations/sqlalchemy/__init__.py
+-rw-r--r--   0        0        0     3428 2023-07-05 13:16:29.918655 mui_data_grid-0.9.0/src/mui/v5/integrations/sqlalchemy/apply_models.py
+-rw-r--r--   0        0        0      325 2023-07-05 13:16:29.919076 mui_data_grid-0.9.0/src/mui/v5/integrations/sqlalchemy/filter/__init__.py
+-rw-r--r--   0        0        0     2029 2023-07-05 13:16:29.919739 mui_data_grid-0.9.0/src/mui/v5/integrations/sqlalchemy/filter/applicators/__init__.py
+-rw-r--r--   0        0        0      753 2023-07-05 13:16:29.919971 mui_data_grid-0.9.0/src/mui/v5/integrations/sqlalchemy/filter/applicators/after.py
+-rw-r--r--   0        0        0     2446 2023-07-05 13:16:29.920191 mui_data_grid-0.9.0/src/mui/v5/integrations/sqlalchemy/filter/applicators/basic.py
+-rw-r--r--   0        0        0      756 2023-07-05 13:16:29.920414 mui_data_grid-0.9.0/src/mui/v5/integrations/sqlalchemy/filter/applicators/before.py
+-rw-r--r--   0        0        0      969 2023-07-05 13:16:29.920634 mui_data_grid-0.9.0/src/mui/v5/integrations/sqlalchemy/filter/applicators/contains.py
+-rw-r--r--   0        0        0      999 2023-07-05 13:16:29.920960 mui_data_grid-0.9.0/src/mui/v5/integrations/sqlalchemy/filter/applicators/endswith.py
+-rw-r--r--   0        0        0     1273 2023-07-05 13:16:29.921345 mui_data_grid-0.9.0/src/mui/v5/integrations/sqlalchemy/filter/applicators/is_.py
+-rw-r--r--   0        0        0     1118 2023-07-05 13:16:29.921570 mui_data_grid-0.9.0/src/mui/v5/integrations/sqlalchemy/filter/applicators/is_any_of.py
+-rw-r--r--   0        0        0      603 2023-07-05 13:16:29.921805 mui_data_grid-0.9.0/src/mui/v5/integrations/sqlalchemy/filter/applicators/is_empty.py
+-rw-r--r--   0        0        0      627 2023-07-05 13:16:29.921988 mui_data_grid-0.9.0/src/mui/v5/integrations/sqlalchemy/filter/applicators/is_not_empty.py
+-rw-r--r--   0        0        0      848 2023-07-05 13:16:29.922183 mui_data_grid-0.9.0/src/mui/v5/integrations/sqlalchemy/filter/applicators/not_.py
+-rw-r--r--   0        0        0      801 2023-07-05 13:16:29.922478 mui_data_grid-0.9.0/src/mui/v5/integrations/sqlalchemy/filter/applicators/on_or_after.py
+-rw-r--r--   0        0        0      793 2023-07-05 13:16:29.922699 mui_data_grid-0.9.0/src/mui/v5/integrations/sqlalchemy/filter/applicators/on_or_before.py
+-rw-r--r--   0        0        0     1015 2023-07-05 13:16:29.923010 mui_data_grid-0.9.0/src/mui/v5/integrations/sqlalchemy/filter/applicators/startswith.py
+-rw-r--r--   0        0        0     5917 2023-07-05 13:16:29.923287 mui_data_grid-0.9.0/src/mui/v5/integrations/sqlalchemy/filter/apply_items.py
+-rw-r--r--   0        0        0     1098 2023-07-05 13:16:29.923623 mui_data_grid-0.9.0/src/mui/v5/integrations/sqlalchemy/filter/apply_model.py
+-rw-r--r--   0        0        0      189 2023-07-05 13:16:29.924090 mui_data_grid-0.9.0/src/mui/v5/integrations/sqlalchemy/pagination/__init__.py
+-rw-r--r--   0        0        0      733 2023-07-05 13:16:29.924303 mui_data_grid-0.9.0/src/mui/v5/integrations/sqlalchemy/pagination/apply_model.py
+-rw-r--r--   0        0        0      299 2023-07-05 13:16:29.924766 mui_data_grid-0.9.0/src/mui/v5/integrations/sqlalchemy/resolver/__init__.py
+-rw-r--r--   0        0        0      305 2023-07-05 13:16:29.924973 mui_data_grid-0.9.0/src/mui/v5/integrations/sqlalchemy/resolver/types.py
+-rw-r--r--   0        0        0      289 2023-07-05 13:16:29.925443 mui_data_grid-0.9.0/src/mui/v5/integrations/sqlalchemy/sort/__init__.py
+-rw-r--r--   0        0        0     3007 2023-07-05 13:16:29.925667 mui_data_grid-0.9.0/src/mui/v5/integrations/sqlalchemy/sort/apply_item.py
+-rw-r--r--   0        0        0     1792 2023-07-05 13:16:29.925877 mui_data_grid-0.9.0/src/mui/v5/integrations/sqlalchemy/sort/apply_model.py
+-rw-r--r--   0        0        0      124 2023-07-05 13:16:29.926493 mui_data_grid-0.9.0/src/mui/v5/integrations/sqlalchemy/structures/__init__.py
+-rw-r--r--   0        0        0      444 2023-07-05 13:16:29.926655 mui_data_grid-0.9.0/src/mui/v5/integrations/sqlalchemy/structures/factory.py
+-rw-r--r--   0        0        0     7010 2023-07-05 13:16:29.926829 mui_data_grid-0.9.0/src/mui/v5/integrations/sqlalchemy/structures/query.py
+-rw-r--r--   0        0        0     1424 2023-07-05 18:31:58.278488 mui_data_grid-0.9.0/src/mui/v6/__init__.py
+-rw-r--r--   0        0        0     1495 2023-07-05 18:31:58.279247 mui_data_grid-0.9.0/src/mui/v6/grid/__init__.py
+-rw-r--r--   0        0        0     2359 2023-07-05 18:31:58.279517 mui_data_grid-0.9.0/src/mui/v6/grid/base.py
+-rw-r--r--   0        0        0      980 2023-07-05 18:31:58.280554 mui_data_grid-0.9.0/src/mui/v6/grid/filter/__init__.py
+-rw-r--r--   0        0        0     2955 2023-07-05 18:31:58.281810 mui_data_grid-0.9.0/src/mui/v6/grid/filter/item.py
+-rw-r--r--   0        0        0     6302 2023-07-05 18:31:58.282727 mui_data_grid-0.9.0/src/mui/v6/grid/filter/model.py
+-rw-r--r--   0        0        0      167 2023-07-05 18:31:58.284159 mui_data_grid-0.9.0/src/mui/v6/grid/logic/__init__.py
+-rw-r--r--   0        0        0      663 2023-07-05 18:31:58.284624 mui_data_grid-0.9.0/src/mui/v6/grid/logic/operator.py
+-rw-r--r--   0        0        0      117 2023-07-05 18:31:58.285274 mui_data_grid-0.9.0/src/mui/v6/grid/pagination/__init__.py
+-rw-r--r--   0        0        0     1231 2023-07-05 18:31:58.286454 mui_data_grid-0.9.0/src/mui/v6/grid/pagination/model.py
+-rw-r--r--   0        0        0     3490 2023-07-05 18:31:58.287454 mui_data_grid-0.9.0/src/mui/v6/grid/request.py
+-rw-r--r--   0        0        0      387 2023-07-05 18:31:58.288351 mui_data_grid-0.9.0/src/mui/v6/grid/sort/__init__.py
+-rw-r--r--   0        0        0      453 2023-07-05 18:31:58.288561 mui_data_grid-0.9.0/src/mui/v6/grid/sort/direction.py
+-rw-r--r--   0        0        0     1310 2023-07-05 18:31:58.288987 mui_data_grid-0.9.0/src/mui/v6/grid/sort/item.py
+-rw-r--r--   0        0        0      444 2023-07-05 18:31:58.289418 mui_data_grid-0.9.0/src/mui/v6/grid/sort/model.py
+-rw-r--r--   0        0        0      218 2023-07-05 18:31:58.289741 mui_data_grid-0.9.0/src/mui/v6/integrations/__init__.py
+-rw-r--r--   0        0        0      658 2023-07-05 18:31:58.290276 mui_data_grid-0.9.0/src/mui/v6/integrations/flask/__init__.py
+-rw-r--r--   0        0        0      230 2023-07-05 18:31:58.291760 mui_data_grid-0.9.0/src/mui/v6/integrations/flask/filter/__init__.py
+-rw-r--r--   0        0        0     1611 2023-07-05 18:31:58.292173 mui_data_grid-0.9.0/src/mui/v6/integrations/flask/filter/model.py
+-rw-r--r--   0        0        0      259 2023-07-05 18:31:58.292729 mui_data_grid-0.9.0/src/mui/v6/integrations/flask/pagination/__init__.py
+-rw-r--r--   0        0        0     1958 2023-07-05 18:31:58.293152 mui_data_grid-0.9.0/src/mui/v6/integrations/flask/pagination/model.py
+-rw-r--r--   0        0        0     2661 2023-07-05 18:31:58.293529 mui_data_grid-0.9.0/src/mui/v6/integrations/flask/request.py
+-rw-r--r--   0        0        0      220 2023-07-05 18:31:58.293920 mui_data_grid-0.9.0/src/mui/v6/integrations/flask/sort/__init__.py
+-rw-r--r--   0        0        0     1370 2023-07-05 18:31:58.294359 mui_data_grid-0.9.0/src/mui/v6/integrations/flask/sort/model.py
+-rw-r--r--   0        0        0      988 2023-07-05 18:31:58.294762 mui_data_grid-0.9.0/src/mui/v6/integrations/sqlalchemy/__init__.py
+-rw-r--r--   0        0        0     3428 2023-07-05 18:31:58.295110 mui_data_grid-0.9.0/src/mui/v6/integrations/sqlalchemy/apply_models.py
+-rw-r--r--   0        0        0      325 2023-07-05 18:31:58.295590 mui_data_grid-0.9.0/src/mui/v6/integrations/sqlalchemy/filter/__init__.py
+-rw-r--r--   0        0        0     2029 2023-07-05 18:31:58.296168 mui_data_grid-0.9.0/src/mui/v6/integrations/sqlalchemy/filter/applicators/__init__.py
+-rw-r--r--   0        0        0      753 2023-07-05 18:31:58.296428 mui_data_grid-0.9.0/src/mui/v6/integrations/sqlalchemy/filter/applicators/after.py
+-rw-r--r--   0        0        0     2404 2023-07-05 18:31:58.296793 mui_data_grid-0.9.0/src/mui/v6/integrations/sqlalchemy/filter/applicators/basic.py
+-rw-r--r--   0        0        0      756 2023-07-05 18:31:58.296999 mui_data_grid-0.9.0/src/mui/v6/integrations/sqlalchemy/filter/applicators/before.py
+-rw-r--r--   0        0        0      969 2023-07-05 18:31:58.297194 mui_data_grid-0.9.0/src/mui/v6/integrations/sqlalchemy/filter/applicators/contains.py
+-rw-r--r--   0        0        0      999 2023-07-05 18:31:58.297413 mui_data_grid-0.9.0/src/mui/v6/integrations/sqlalchemy/filter/applicators/endswith.py
+-rw-r--r--   0        0        0     1273 2023-07-05 18:31:58.297678 mui_data_grid-0.9.0/src/mui/v6/integrations/sqlalchemy/filter/applicators/is_.py
+-rw-r--r--   0        0        0     1118 2023-07-05 18:31:58.297902 mui_data_grid-0.9.0/src/mui/v6/integrations/sqlalchemy/filter/applicators/is_any_of.py
+-rw-r--r--   0        0        0      603 2023-07-05 18:31:58.298113 mui_data_grid-0.9.0/src/mui/v6/integrations/sqlalchemy/filter/applicators/is_empty.py
+-rw-r--r--   0        0        0      627 2023-07-05 18:31:58.298318 mui_data_grid-0.9.0/src/mui/v6/integrations/sqlalchemy/filter/applicators/is_not_empty.py
+-rw-r--r--   0        0        0      848 2023-07-05 18:31:58.298542 mui_data_grid-0.9.0/src/mui/v6/integrations/sqlalchemy/filter/applicators/not_.py
+-rw-r--r--   0        0        0      801 2023-07-05 18:31:58.298762 mui_data_grid-0.9.0/src/mui/v6/integrations/sqlalchemy/filter/applicators/on_or_after.py
+-rw-r--r--   0        0        0      793 2023-07-05 18:31:58.298972 mui_data_grid-0.9.0/src/mui/v6/integrations/sqlalchemy/filter/applicators/on_or_before.py
+-rw-r--r--   0        0        0     1015 2023-07-05 18:31:58.299217 mui_data_grid-0.9.0/src/mui/v6/integrations/sqlalchemy/filter/applicators/startswith.py
+-rw-r--r--   0        0        0     5830 2023-07-05 18:31:58.299666 mui_data_grid-0.9.0/src/mui/v6/integrations/sqlalchemy/filter/apply_items.py
+-rw-r--r--   0        0        0     1098 2023-07-05 18:31:58.300095 mui_data_grid-0.9.0/src/mui/v6/integrations/sqlalchemy/filter/apply_model.py
+-rw-r--r--   0        0        0      189 2023-07-05 18:31:58.300572 mui_data_grid-0.9.0/src/mui/v6/integrations/sqlalchemy/pagination/__init__.py
+-rw-r--r--   0        0        0      733 2023-07-05 18:31:58.300965 mui_data_grid-0.9.0/src/mui/v6/integrations/sqlalchemy/pagination/apply_model.py
+-rw-r--r--   0        0        0      299 2023-07-05 18:31:58.301480 mui_data_grid-0.9.0/src/mui/v6/integrations/sqlalchemy/resolver/__init__.py
+-rw-r--r--   0        0        0      305 2023-07-05 18:31:58.301701 mui_data_grid-0.9.0/src/mui/v6/integrations/sqlalchemy/resolver/types.py
+-rw-r--r--   0        0        0      289 2023-07-05 18:31:58.302243 mui_data_grid-0.9.0/src/mui/v6/integrations/sqlalchemy/sort/__init__.py
+-rw-r--r--   0        0        0     3007 2023-07-05 18:31:58.302641 mui_data_grid-0.9.0/src/mui/v6/integrations/sqlalchemy/sort/apply_item.py
+-rw-r--r--   0        0        0     1792 2023-07-05 18:31:58.303038 mui_data_grid-0.9.0/src/mui/v6/integrations/sqlalchemy/sort/apply_model.py
+-rw-r--r--   0        0        0      124 2023-07-05 18:31:58.303562 mui_data_grid-0.9.0/src/mui/v6/integrations/sqlalchemy/structures/__init__.py
+-rw-r--r--   0        0        0      444 2023-07-05 18:31:58.303811 mui_data_grid-0.9.0/src/mui/v6/integrations/sqlalchemy/structures/factory.py
+-rw-r--r--   0        0        0     7010 2023-07-05 18:31:58.304742 mui_data_grid-0.9.0/src/mui/v6/integrations/sqlalchemy/structures/query.py
+-rw-r--r--   0        0        0     3953 1970-01-01 00:00:00.000000 mui_data_grid-0.9.0/PKG-INFO
```

### Comparing `mui_data_grid-0.8.4/LICENSE` & `mui_data_grid-0.9.0/LICENSE`

 * *Files identical despite different names*

### Comparing `mui_data_grid-0.8.4/README.md` & `mui_data_grid-0.9.0/README.md`

 * *Files identical despite different names*

### Comparing `mui_data_grid-0.8.4/pyproject.toml` & `mui_data_grid-0.9.0/pyproject.toml`

 * *Files 5% similar despite different names*

```diff
@@ -5,68 +5,68 @@
 # documentation = "https://mui-data-grid.readthedocs.io/en/latest/"
 include = ["src/mui/py.typed", "LICENSE"]
 license = "MIT"
 name = "mui-data-grid"
 packages = [{ include = "mui", from = "src" }]
 readme = "README.md"
 repository = "https://github.com/kkirsche/mui-data-grid"
-version = "0.8.4"
+version = "0.9.0"
 
 [tool.poetry.dependencies]
-python = ">=3.7,<4"
+python = ">=3.8.1,<4"
 pydantic = ">=1.10.2,<2"
-typing-extensions = ">=4.4.0,<5"
+typing-extensions = ">=4.7.1,<5"
 
 # [tool.poetry.extras]
 # flask = ["flask@>=2,<3"]
 # sqlalchemy = ["sqlalchemy@>=1.4,<2"]
 
 [tool.poetry.group.github-actions.dependencies]
-bandit = "^1.7.4"
-black = "^22.12.0"
-codespell = "^2.2.2"
+bandit = "^1.7.5"
+black = "^23.3.0"
+codespell = "^2.2.5"
 example-isort-formatting-plugin = "^0.1.1"
 example-isort-sorting-plugin = "^0.1.0"
-flake8 = "<6"
-flake8-bugbear = "^23.1.20"
-flake8-pyi = "^23.1.0"
-hypothesis = "^6.65.0"
+flake8 = "^6.0.0"
+flake8-bugbear = "^23.6.5"
+flake8-pyi = "^23.6.0"
+hypothesis = "^6.80.0"
 interrogate = "^1.5.0"
-isort = "^5.11.4"
-mypy = "^0.991"
-pytest = "^7.2.1"
-pyupgrade = "^3.3.1"
+isort = "^5.12.0"
+mypy = "<1"
+pytest = "^7.4.0"
+pyupgrade = "^3.8.0"
 
 [tool.poetry.group.flask.dependencies]
-flask = ">=2,<3"
+flask = ">=2.2.5,<3"
 
 [tool.poetry.group.sqlalchemy.dependencies]
 sqlalchemy = ">=1.4,<2"
-sqlalchemy2-stubs = ">=0.0.2a29"
+sqlalchemy2-stubs = ">=0.0.2a34"
 
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.isort]
 formatter = "example"
 profile = "black"
 remove_redundant_aliases = true
 sort_order = "natural_plus"
 
 [tool.black]
 include = '\.pyi?$'
 line-length = 88
-target-version = ['py37']
+target-version = ['py38']
 
 [tool.mypy]
 exclude = ['^compat\.py$']
 follow_imports = "normal"
 plugins = ["pydantic.mypy", "sqlalchemy.ext.mypy.plugin"]
-python_version = "3.7"
+python_version = "3.8"
 strict = true
 warn_return_any = true
 warn_unused_configs = true
 
 [[tool.mypy.overrides]]
 ignore_missing_imports = true
 module = [
@@ -103,9 +103,9 @@
 quiet = false
 verbose = 1
 
 [tool.pyright]
 exclude = ["**/__pycache__", "**/.git"]
 include = ["src"]
 pythonPlatform = "All"
-pythonVersion = "3.7"
+pythonVersion = "3.8"
 typeCheckingMode = "strict"
```

### Comparing `mui_data_grid-0.8.4/src/mui/compat.py` & `mui_data_grid-0.9.0/src/mui/compat.py`

 * *Files identical despite different names*

### Comparing `mui_data_grid-0.8.4/src/mui/v5/__init__.py` & `mui_data_grid-0.9.0/src/mui/v5/__init__.py`

 * *Files identical despite different names*

### Comparing `mui_data_grid-0.8.4/src/mui/v5/grid/__init__.py` & `mui_data_grid-0.9.0/src/mui/v5/grid/__init__.py`

 * *Files identical despite different names*

### Comparing `mui_data_grid-0.8.4/src/mui/v5/grid/base.py` & `mui_data_grid-0.9.0/src/mui/v5/grid/base.py`

 * *Files identical despite different names*

### Comparing `mui_data_grid-0.8.4/src/mui/v5/grid/filter/__init__.py` & `mui_data_grid-0.9.0/src/mui/v5/grid/filter/__init__.py`

 * *Files identical despite different names*

### Comparing `mui_data_grid-0.8.4/src/mui/v5/grid/filter/item.py` & `mui_data_grid-0.9.0/src/mui/v5/grid/filter/item.py`

 * *Files identical despite different names*

### Comparing `mui_data_grid-0.8.4/src/mui/v5/grid/filter/model.py` & `mui_data_grid-0.9.0/src/mui/v5/grid/filter/model.py`

 * *Files identical despite different names*

### Comparing `mui_data_grid-0.8.4/src/mui/v5/grid/link/operator.py` & `mui_data_grid-0.9.0/src/mui/v5/grid/link/operator.py`

 * *Files identical despite different names*

### Comparing `mui_data_grid-0.8.4/src/mui/v5/grid/pagination/model.py` & `mui_data_grid-0.9.0/src/mui/v5/grid/pagination/model.py`

 * *Files identical despite different names*

### Comparing `mui_data_grid-0.8.4/src/mui/v5/grid/request.py` & `mui_data_grid-0.9.0/src/mui/v5/grid/request.py`

 * *Files identical despite different names*

### Comparing `mui_data_grid-0.8.4/src/mui/v5/grid/sort/item.py` & `mui_data_grid-0.9.0/src/mui/v5/grid/sort/item.py`

 * *Files identical despite different names*

### Comparing `mui_data_grid-0.8.4/src/mui/v5/integrations/flask/__init__.py` & `mui_data_grid-0.9.0/src/mui/v5/integrations/flask/__init__.py`

 * *Files identical despite different names*

### Comparing `mui_data_grid-0.8.4/src/mui/v5/integrations/flask/filter/model.py` & `mui_data_grid-0.9.0/src/mui/v5/integrations/flask/filter/model.py`

 * *Files identical despite different names*

### Comparing `mui_data_grid-0.8.4/src/mui/v5/integrations/flask/pagination/model.py` & `mui_data_grid-0.9.0/src/mui/v5/integrations/flask/pagination/model.py`

 * *Files identical despite different names*

### Comparing `mui_data_grid-0.8.4/src/mui/v5/integrations/flask/request.py` & `mui_data_grid-0.9.0/src/mui/v5/integrations/flask/request.py`

 * *Files identical despite different names*

### Comparing `mui_data_grid-0.8.4/src/mui/v5/integrations/flask/sort/model.py` & `mui_data_grid-0.9.0/src/mui/v5/integrations/flask/sort/model.py`

 * *Files identical despite different names*

### Comparing `mui_data_grid-0.8.4/src/mui/v5/integrations/sqlalchemy/__init__.py` & `mui_data_grid-0.9.0/src/mui/v5/integrations/sqlalchemy/__init__.py`

 * *Files identical despite different names*

### Comparing `mui_data_grid-0.8.4/src/mui/v5/integrations/sqlalchemy/apply_models.py` & `mui_data_grid-0.9.0/src/mui/v5/integrations/sqlalchemy/apply_models.py`

 * *Files identical despite different names*

### Comparing `mui_data_grid-0.8.4/src/mui/v5/integrations/sqlalchemy/filter/applicators/__init__.py` & `mui_data_grid-0.9.0/src/mui/v5/integrations/sqlalchemy/filter/applicators/__init__.py`

 * *Files identical despite different names*

### Comparing `mui_data_grid-0.8.4/src/mui/v5/integrations/sqlalchemy/filter/applicators/after.py` & `mui_data_grid-0.9.0/src/mui/v5/integrations/sqlalchemy/filter/applicators/after.py`

 * *Files identical despite different names*

### Comparing `mui_data_grid-0.8.4/src/mui/v5/integrations/sqlalchemy/filter/applicators/basic.py` & `mui_data_grid-0.9.0/src/mui/v5/integrations/sqlalchemy/filter/applicators/basic.py`

 * *Files identical despite different names*

### Comparing `mui_data_grid-0.8.4/src/mui/v5/integrations/sqlalchemy/filter/applicators/before.py` & `mui_data_grid-0.9.0/src/mui/v5/integrations/sqlalchemy/filter/applicators/before.py`

 * *Files identical despite different names*

### Comparing `mui_data_grid-0.8.4/src/mui/v5/integrations/sqlalchemy/filter/applicators/contains.py` & `mui_data_grid-0.9.0/src/mui/v5/integrations/sqlalchemy/filter/applicators/contains.py`

 * *Files identical despite different names*

### Comparing `mui_data_grid-0.8.4/src/mui/v5/integrations/sqlalchemy/filter/applicators/endswith.py` & `mui_data_grid-0.9.0/src/mui/v5/integrations/sqlalchemy/filter/applicators/endswith.py`

 * *Files identical despite different names*

### Comparing `mui_data_grid-0.8.4/src/mui/v5/integrations/sqlalchemy/filter/applicators/is_.py` & `mui_data_grid-0.9.0/src/mui/v5/integrations/sqlalchemy/filter/applicators/is_.py`

 * *Files identical despite different names*

### Comparing `mui_data_grid-0.8.4/src/mui/v5/integrations/sqlalchemy/filter/applicators/is_any_of.py` & `mui_data_grid-0.9.0/src/mui/v5/integrations/sqlalchemy/filter/applicators/is_any_of.py`

 * *Files identical despite different names*

### Comparing `mui_data_grid-0.8.4/src/mui/v5/integrations/sqlalchemy/filter/applicators/is_empty.py` & `mui_data_grid-0.9.0/src/mui/v5/integrations/sqlalchemy/filter/applicators/is_empty.py`

 * *Files identical despite different names*

### Comparing `mui_data_grid-0.8.4/src/mui/v5/integrations/sqlalchemy/filter/applicators/is_not_empty.py` & `mui_data_grid-0.9.0/src/mui/v5/integrations/sqlalchemy/filter/applicators/is_not_empty.py`

 * *Files identical despite different names*

### Comparing `mui_data_grid-0.8.4/src/mui/v5/integrations/sqlalchemy/filter/applicators/not_.py` & `mui_data_grid-0.9.0/src/mui/v5/integrations/sqlalchemy/filter/applicators/not_.py`

 * *Files identical despite different names*

### Comparing `mui_data_grid-0.8.4/src/mui/v5/integrations/sqlalchemy/filter/applicators/on_or_after.py` & `mui_data_grid-0.9.0/src/mui/v5/integrations/sqlalchemy/filter/applicators/on_or_after.py`

 * *Files identical despite different names*

### Comparing `mui_data_grid-0.8.4/src/mui/v5/integrations/sqlalchemy/filter/applicators/on_or_before.py` & `mui_data_grid-0.9.0/src/mui/v5/integrations/sqlalchemy/filter/applicators/on_or_before.py`

 * *Files identical despite different names*

### Comparing `mui_data_grid-0.8.4/src/mui/v5/integrations/sqlalchemy/filter/applicators/startswith.py` & `mui_data_grid-0.9.0/src/mui/v5/integrations/sqlalchemy/filter/applicators/startswith.py`

 * *Files identical despite different names*

### Comparing `mui_data_grid-0.8.4/src/mui/v5/integrations/sqlalchemy/filter/apply_items.py` & `mui_data_grid-0.9.0/src/mui/v5/integrations/sqlalchemy/filter/apply_items.py`

 * *Files identical despite different names*

### Comparing `mui_data_grid-0.8.4/src/mui/v5/integrations/sqlalchemy/filter/apply_model.py` & `mui_data_grid-0.9.0/src/mui/v5/integrations/sqlalchemy/filter/apply_model.py`

 * *Files identical despite different names*

### Comparing `mui_data_grid-0.8.4/src/mui/v5/integrations/sqlalchemy/pagination/apply_model.py` & `mui_data_grid-0.9.0/src/mui/v5/integrations/sqlalchemy/pagination/apply_model.py`

 * *Files identical despite different names*

### Comparing `mui_data_grid-0.8.4/src/mui/v5/integrations/sqlalchemy/sort/apply_item.py` & `mui_data_grid-0.9.0/src/mui/v5/integrations/sqlalchemy/sort/apply_item.py`

 * *Files identical despite different names*

### Comparing `mui_data_grid-0.8.4/src/mui/v5/integrations/sqlalchemy/sort/apply_model.py` & `mui_data_grid-0.9.0/src/mui/v5/integrations/sqlalchemy/sort/apply_model.py`

 * *Files identical despite different names*

### Comparing `mui_data_grid-0.8.4/src/mui/v5/integrations/sqlalchemy/structures/query.py` & `mui_data_grid-0.9.0/src/mui/v5/integrations/sqlalchemy/structures/query.py`

 * *Files identical despite different names*

### Comparing `mui_data_grid-0.8.4/PKG-INFO` & `mui_data_grid-0.9.0/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,25 +1,23 @@
 Metadata-Version: 2.1
 Name: mui-data-grid
-Version: 0.8.4
+Version: 0.9.0
 Summary: Unofficial backend utilities for using Material-UI's X-Data-Grid component
 Home-page: https://github.com/kkirsche/mui-data-grid
 License: MIT
 Author: Kevin Kirsche
 Author-email: kev.kirsche@gmail.com
-Requires-Python: >=3.7,<4
+Requires-Python: >=3.8.1,<4
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.7
-Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: pydantic (>=1.10.2,<2)
-Requires-Dist: typing-extensions (>=4.4.0,<5)
+Requires-Dist: typing-extensions (>=4.7.1,<5)
 Project-URL: Repository, https://github.com/kkirsche/mui-data-grid
 Description-Content-Type: text/markdown
 
 # MUI Data Grid
 
 This is an unofficial toolbox to make integrating a Python web application with Material UI's data grid simpler.
```

