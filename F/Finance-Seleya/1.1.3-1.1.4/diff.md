# Comparing `tmp/Finance-Seleya-1.1.3.tar.gz` & `tmp/Finance-Seleya-1.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/Finance-Seleya-1.1.3.tar", last modified: Tue Jul  4 06:39:59 2023, max compression
+gzip compressed data, was "dist/Finance-Seleya-1.1.4.tar", last modified: Wed Jul  5 08:01:19 2023, max compression
```

## Comparing `Finance-Seleya-1.1.3.tar` & `Finance-Seleya-1.1.4.tar`

### file list

```diff
@@ -1,116 +1,124 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-04 06:39:59.000000 Finance-Seleya-1.1.3/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-04 06:39:59.000000 Finance-Seleya-1.1.3/Finance_Seleya.egg-info/
--rw-r--r--   0 root         (0) root         (0)      211 2023-07-04 06:39:59.000000 Finance-Seleya-1.1.3/Finance_Seleya.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     3083 2023-07-04 06:39:59.000000 Finance-Seleya-1.1.3/Finance_Seleya.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-07-04 06:39:59.000000 Finance-Seleya-1.1.3/Finance_Seleya.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      213 2023-07-04 06:39:59.000000 Finance-Seleya-1.1.3/Finance_Seleya.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        7 2023-07-04 06:39:59.000000 Finance-Seleya-1.1.3/Finance_Seleya.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)      190 2023-06-24 10:22:53.000000 Finance-Seleya-1.1.3/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)      211 2023-07-04 06:39:59.000000 Finance-Seleya-1.1.3/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)        9 2022-11-07 11:29:19.000000 Finance-Seleya-1.1.3/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-04 06:39:59.000000 Finance-Seleya-1.1.3/requirements/
--rw-r--r--   0 root         (0) root         (0)        0 2022-11-07 11:29:19.000000 Finance-Seleya-1.1.3/requirements/py2.txt
--rw-r--r--   0 root         (0) root         (0)      212 2023-02-24 05:29:06.000000 Finance-Seleya-1.1.3/requirements/py3.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-04 06:39:59.000000 Finance-Seleya-1.1.3/seleya/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-04 06:39:59.000000 Finance-Seleya-1.1.3/seleya/Toolset/
--rw-r--r--   0 root         (0) root         (0)      107 2022-11-07 11:29:19.000000 Finance-Seleya-1.1.3/seleya/Toolset/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-04 06:39:59.000000 Finance-Seleya-1.1.3/seleya/Toolset/audit/
--rw-r--r--   0 root         (0) root         (0)        0 2022-11-07 11:29:19.000000 Finance-Seleya-1.1.3/seleya/Toolset/audit/__init__.py
--rw-r--r--   0 root         (0) root         (0)     2112 2023-02-20 15:07:28.000000 Finance-Seleya-1.1.3/seleya/Toolset/audit/esg_metrics.py
--rw-r--r--   0 root         (0) root         (0)     3486 2023-02-20 15:07:28.000000 Finance-Seleya-1.1.3/seleya/Toolset/blob_service.py
--rw-r--r--   0 root         (0) root         (0)     4827 2022-11-07 11:29:19.000000 Finance-Seleya-1.1.3/seleya/Toolset/calendar.py
--rw-r--r--   0 root         (0) root         (0)     7223 2023-02-23 08:27:43.000000 Finance-Seleya-1.1.3/seleya/Toolset/file_util.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-04 06:39:59.000000 Finance-Seleya-1.1.3/seleya/Toolset/portfolio/
--rw-r--r--   0 root         (0) root         (0)        0 2022-11-07 11:29:19.000000 Finance-Seleya-1.1.3/seleya/Toolset/portfolio/__init__.py
--rw-r--r--   0 root         (0) root         (0)     6676 2023-02-20 15:07:28.000000 Finance-Seleya-1.1.3/seleya/Toolset/portfolio/esg_metrics.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-04 06:39:59.000000 Finance-Seleya-1.1.3/seleya/Toolset/tests/
--rw-r--r--   0 root         (0) root         (0)       24 2022-11-07 11:29:19.000000 Finance-Seleya-1.1.3/seleya/Toolset/tests/__init__.py
--rw-r--r--   0 root         (0) root         (0)      632 2022-11-07 11:29:19.000000 Finance-Seleya-1.1.3/seleya/Toolset/tests/runner.py
--rw-r--r--   0 root         (0) root         (0)      244 2022-11-07 11:29:19.000000 Finance-Seleya-1.1.3/seleya/Toolset/tests/suite.py
--rw-r--r--   0 root         (0) root         (0)     5733 2022-11-07 11:29:19.000000 Finance-Seleya-1.1.3/seleya/Toolset/translator.py
--rw-r--r--   0 root         (0) root         (0)     2074 2023-02-20 15:07:28.000000 Finance-Seleya-1.1.3/seleya/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-04 06:39:59.000000 Finance-Seleya-1.1.3/seleya/config/
--rw-r--r--   0 root         (0) root         (0)        0 2022-11-07 11:29:19.000000 Finance-Seleya-1.1.3/seleya/config/__init__.py
--rw-r--r--   0 root         (0) root         (0)      489 2022-11-07 11:29:19.000000 Finance-Seleya-1.1.3/seleya/config/default_config.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-04 06:39:59.000000 Finance-Seleya-1.1.3/seleya/core/
--rw-r--r--   0 root         (0) root         (0)        0 2022-11-11 11:55:10.000000 Finance-Seleya-1.1.3/seleya/core/__init__.py
--rw-r--r--   0 root         (0) root         (0)     3121 2022-11-11 11:55:10.000000 Finance-Seleya-1.1.3/seleya/core/env.py
--rw-r--r--   0 root         (0) root         (0)     9714 2022-11-11 11:55:10.000000 Finance-Seleya-1.1.3/seleya/core/fixes.py
--rw-r--r--   0 root         (0) root         (0)     7809 2022-11-11 11:55:10.000000 Finance-Seleya-1.1.3/seleya/core/helper.py
--rw-r--r--   0 root         (0) root         (0)     1921 2022-11-11 11:55:10.000000 Finance-Seleya-1.1.3/seleya/core/parallel.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-04 06:39:59.000000 Finance-Seleya-1.1.3/seleya/data/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-04 06:39:59.000000 Finance-Seleya-1.1.3/seleya/data/DataAPI/
--rw-r--r--   0 root         (0) root         (0)       94 2023-02-20 15:07:28.000000 Finance-Seleya-1.1.3/seleya/data/DataAPI/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-04 06:39:59.000000 Finance-Seleya-1.1.3/seleya/data/DataAPI/http/
--rw-r--r--   0 root         (0) root         (0)     3533 2023-02-20 15:07:28.000000 Finance-Seleya-1.1.3/seleya/data/DataAPI/http/ESG.py
--rw-r--r--   0 root         (0) root         (0)     3211 2023-02-20 15:07:28.000000 Finance-Seleya-1.1.3/seleya/data/DataAPI/http/GD.py
--rw-r--r--   0 root         (0) root         (0)     4296 2023-02-20 15:07:28.000000 Finance-Seleya-1.1.3/seleya/data/DataAPI/http/SEARCH.py
--rw-r--r--   0 root         (0) root         (0)     2288 2023-02-20 15:07:28.000000 Finance-Seleya-1.1.3/seleya/data/DataAPI/http/USER.py
--rw-r--r--   0 root         (0) root         (0)      382 2023-02-20 15:07:28.000000 Finance-Seleya-1.1.3/seleya/data/DataAPI/http/__init__.py
--rw-r--r--   0 root         (0) root         (0)      599 2023-02-20 15:07:28.000000 Finance-Seleya-1.1.3/seleya/data/DataAPI/http/utils.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-04 06:39:59.000000 Finance-Seleya-1.1.3/seleya/data/DataAPI/mongo/
--rw-r--r--   0 root         (0) root         (0)       62 2023-02-20 15:07:28.000000 Finance-Seleya-1.1.3/seleya/data/DataAPI/mongo/__init__.py
--rw-r--r--   0 root         (0) root         (0)      348 2023-02-20 15:07:28.000000 Finance-Seleya-1.1.3/seleya/data/DataAPI/mongo/fetch_engine.py
--rw-r--r--   0 root         (0) root         (0)     2408 2023-02-20 15:07:28.000000 Finance-Seleya-1.1.3/seleya/data/DataAPI/mongo/mongodb.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-04 06:39:59.000000 Finance-Seleya-1.1.3/seleya/data/DataAPI/sqlatom/
--rw-r--r--   0 root         (0) root         (0)      117 2023-02-20 15:07:28.000000 Finance-Seleya-1.1.3/seleya/data/DataAPI/sqlatom/__init__.py
--rw-r--r--   0 root         (0) root         (0)    36127 2023-02-20 15:07:28.000000 Finance-Seleya-1.1.3/seleya/data/DataAPI/sqlatom/db_factory.py
--rw-r--r--   0 root         (0) root         (0)     7397 2023-04-17 00:03:09.000000 Finance-Seleya-1.1.3/seleya/data/DataAPI/sqlatom/fetch_engine.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-04 06:39:59.000000 Finance-Seleya-1.1.3/seleya/data/DataAPI/sqlatom/sly/
--rw-r--r--   0 root         (0) root         (0)        0 2023-02-20 15:07:28.000000 Finance-Seleya-1.1.3/seleya/data/DataAPI/sqlatom/sly/__init__.py
--rw-r--r--   0 root         (0) root         (0)    55584 2023-07-04 06:39:24.000000 Finance-Seleya-1.1.3/seleya/data/DataAPI/sqlatom/sly/sly_engine.py
--rw-r--r--   0 root         (0) root         (0)       21 2023-02-20 15:07:28.000000 Finance-Seleya-1.1.3/seleya/data/DataAPI/version.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-04 06:39:59.000000 Finance-Seleya-1.1.3/seleya/data/SurfaceAPI/
--rw-r--r--   0 root         (0) root         (0)       23 2023-02-20 15:07:28.000000 Finance-Seleya-1.1.3/seleya/data/SurfaceAPI/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-04 06:39:59.000000 Finance-Seleya-1.1.3/seleya/data/SurfaceAPI/mongo/
--rw-r--r--   0 root         (0) root         (0)      383 2023-02-28 01:50:45.000000 Finance-Seleya-1.1.3/seleya/data/SurfaceAPI/mongo/__init__.py
--rw-r--r--   0 root         (0) root         (0)      633 2023-02-28 12:53:15.000000 Finance-Seleya-1.1.3/seleya/data/SurfaceAPI/mongo/basic.py
--rw-r--r--   0 root         (0) root         (0)     2042 2023-03-03 01:31:51.000000 Finance-Seleya-1.1.3/seleya/data/SurfaceAPI/mongo/engine.py
--rw-r--r--   0 root         (0) root         (0)     1265 2023-02-28 10:24:23.000000 Finance-Seleya-1.1.3/seleya/data/SurfaceAPI/mongo/gd_qrank_dist.py
--rw-r--r--   0 root         (0) root         (0)     1168 2023-02-24 05:29:06.000000 Finance-Seleya-1.1.3/seleya/data/SurfaceAPI/mongo/gd_qrank_raw.py
--rw-r--r--   0 root         (0) root         (0)      866 2023-02-28 01:50:45.000000 Finance-Seleya-1.1.3/seleya/data/SurfaceAPI/mongo/gic_dist_level1.py
--rw-r--r--   0 root         (0) root         (0)      877 2023-02-28 12:26:53.000000 Finance-Seleya-1.1.3/seleya/data/SurfaceAPI/mongo/non_gic_dist_level1.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-04 06:39:59.000000 Finance-Seleya-1.1.3/seleya/data/SurfaceAPI/sqlatom/
--rw-r--r--   0 root         (0) root         (0)     1098 2023-03-28 11:57:26.000000 Finance-Seleya-1.1.3/seleya/data/SurfaceAPI/sqlatom/__init__.py
--rw-r--r--   0 root         (0) root         (0)      937 2023-03-02 23:18:44.000000 Finance-Seleya-1.1.3/seleya/data/SurfaceAPI/sqlatom/basic.py
--rw-r--r--   0 root         (0) root         (0)      626 2023-03-01 14:55:21.000000 Finance-Seleya-1.1.3/seleya/data/SurfaceAPI/sqlatom/co2_emission_target.py
--rw-r--r--   0 root         (0) root         (0)      537 2023-03-02 23:18:57.000000 Finance-Seleya-1.1.3/seleya/data/SurfaceAPI/sqlatom/company.py
--rw-r--r--   0 root         (0) root         (0)      527 2023-03-02 01:54:52.000000 Finance-Seleya-1.1.3/seleya/data/SurfaceAPI/sqlatom/company_emission_temperature.py
--rw-r--r--   0 root         (0) root         (0)      525 2023-03-02 02:20:33.000000 Finance-Seleya-1.1.3/seleya/data/SurfaceAPI/sqlatom/emission_score_average.py
--rw-r--r--   0 root         (0) root         (0)     1687 2023-03-30 06:02:56.000000 Finance-Seleya-1.1.3/seleya/data/SurfaceAPI/sqlatom/engine.py
--rw-r--r--   0 root         (0) root         (0)      836 2023-02-28 01:50:45.000000 Finance-Seleya-1.1.3/seleya/data/SurfaceAPI/sqlatom/feature_importance.py
--rw-r--r--   0 root         (0) root         (0)      497 2023-02-20 15:07:28.000000 Finance-Seleya-1.1.3/seleya/data/SurfaceAPI/sqlatom/gd_overview.py
--rw-r--r--   0 root         (0) root         (0)      611 2023-02-20 15:07:28.000000 Finance-Seleya-1.1.3/seleya/data/SurfaceAPI/sqlatom/gd_reviews.py
--rw-r--r--   0 root         (0) root         (0)      624 2023-03-28 12:22:57.000000 Finance-Seleya-1.1.3/seleya/data/SurfaceAPI/sqlatom/gd_reviews_base.py
--rw-r--r--   0 root         (0) root         (0)     2388 2023-03-28 12:11:51.000000 Finance-Seleya-1.1.3/seleya/data/SurfaceAPI/sqlatom/industry.py
--rw-r--r--   0 root         (0) root         (0)     2475 2023-03-16 08:51:54.000000 Finance-Seleya-1.1.3/seleya/data/SurfaceAPI/sqlatom/metrics.py
--rw-r--r--   0 root         (0) root         (0)      700 2023-02-24 05:29:06.000000 Finance-Seleya-1.1.3/seleya/data/SurfaceAPI/sqlatom/sasb_mapdom.py
--rw-r--r--   0 root         (0) root         (0)      836 2023-02-28 01:50:45.000000 Finance-Seleya-1.1.3/seleya/data/SurfaceAPI/sqlatom/sector.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-02-20 15:07:28.000000 Finance-Seleya-1.1.3/seleya/data/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-04 06:39:59.000000 Finance-Seleya-1.1.3/seleya/mfc/
--rw-r--r--   0 root         (0) root         (0)        0 2023-02-20 15:07:28.000000 Finance-Seleya-1.1.3/seleya/mfc/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-04 06:39:59.000000 Finance-Seleya-1.1.3/seleya/mfc/alchemy/
--rw-r--r--   0 root         (0) root         (0)      284 2023-03-16 07:14:16.000000 Finance-Seleya-1.1.3/seleya/mfc/alchemy/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-04 06:39:59.000000 Finance-Seleya-1.1.3/seleya/mfc/alchemy/qrank/
--rwxr-xr-x   0 root         (0) root         (0)   145856 2023-06-24 10:17:00.000000 Finance-Seleya-1.1.3/seleya/mfc/alchemy/qrank/glassdoo.cpython-37m-x86_64-linux-gnu.so
--rw-r--r--   0 root         (0) root         (0)   504608 2023-06-24 10:13:04.000000 Finance-Seleya-1.1.3/seleya/mfc/alchemy/qrank/glassdoor.c
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-04 06:39:59.000000 Finance-Seleya-1.1.3/seleya/mfc/alchemy/sbti/
--rw-r--r--   0 root         (0) root         (0)        0 2023-03-01 14:22:17.000000 Finance-Seleya-1.1.3/seleya/mfc/alchemy/sbti/__init__.py
--rw-r--r--   0 root         (0) root         (0)    22737 2023-04-02 13:21:46.000000 Finance-Seleya-1.1.3/seleya/mfc/alchemy/sbti/emission.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-04 06:39:59.000000 Finance-Seleya-1.1.3/seleya/mfc/alchemy/tsi/
--rw-r--r--   0 root         (0) root         (0)        0 2023-02-28 01:50:45.000000 Finance-Seleya-1.1.3/seleya/mfc/alchemy/tsi/__init__.py
--rw-r--r--   0 root         (0) root         (0)     7878 2023-03-17 00:13:38.000000 Finance-Seleya-1.1.3/seleya/mfc/alchemy/tsi/aerosol.py
--rw-r--r--   0 root         (0) root         (0)    11460 2023-03-10 06:20:30.000000 Finance-Seleya-1.1.3/seleya/mfc/alchemy/tsi/s2f.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-04 06:39:59.000000 Finance-Seleya-1.1.3/seleya/mfc/micro/
--rw-r--r--   0 root         (0) root         (0)        0 2023-02-06 13:27:54.000000 Finance-Seleya-1.1.3/seleya/mfc/micro/__init__.py
--rw-r--r--   0 root         (0) root         (0)      132 2022-11-07 11:29:19.000000 Finance-Seleya-1.1.3/seleya/seleya.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-04 06:39:59.000000 Finance-Seleya-1.1.3/seleya/utilities/
--rw-r--r--   0 root         (0) root         (0)        0 2022-11-07 11:29:19.000000 Finance-Seleya-1.1.3/seleya/utilities/__init__.py
--rw-r--r--   0 root         (0) root         (0)     3293 2022-11-07 11:29:19.000000 Finance-Seleya-1.1.3/seleya/utilities/api_base.py
--rw-r--r--   0 root         (0) root         (0)      418 2023-03-03 01:22:19.000000 Finance-Seleya-1.1.3/seleya/utilities/exceptions.py
--rw-r--r--   0 root         (0) root         (0)     5108 2023-02-20 15:07:28.000000 Finance-Seleya-1.1.3/seleya/utilities/kd_logger.py
--rw-r--r--   0 root         (0) root         (0)      490 2022-11-07 11:29:19.000000 Finance-Seleya-1.1.3/seleya/utilities/singleton.py
--rw-r--r--   0 root         (0) root         (0)      399 2022-11-07 11:29:19.000000 Finance-Seleya-1.1.3/seleya/utilities/warning.py
--rw-r--r--   0 root         (0) root         (0)       21 2023-07-04 06:28:45.000000 Finance-Seleya-1.1.3/seleya/version.py
--rw-r--r--   0 root         (0) root         (0)       38 2023-07-04 06:39:59.000000 Finance-Seleya-1.1.3/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     3338 2023-06-24 15:02:35.000000 Finance-Seleya-1.1.3/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-05 08:01:19.000000 Finance-Seleya-1.1.4/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-05 08:01:19.000000 Finance-Seleya-1.1.4/Finance_Seleya.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      211 2023-07-05 08:01:19.000000 Finance-Seleya-1.1.4/Finance_Seleya.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     3312 2023-07-05 08:01:19.000000 Finance-Seleya-1.1.4/Finance_Seleya.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-05 08:01:19.000000 Finance-Seleya-1.1.4/Finance_Seleya.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      213 2023-07-05 08:01:19.000000 Finance-Seleya-1.1.4/Finance_Seleya.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        7 2023-07-05 08:01:19.000000 Finance-Seleya-1.1.4/Finance_Seleya.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)      145 2023-07-05 06:31:30.000000 Finance-Seleya-1.1.4/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)      211 2023-07-05 08:01:19.000000 Finance-Seleya-1.1.4/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)        9 2022-11-07 11:29:19.000000 Finance-Seleya-1.1.4/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-05 08:01:19.000000 Finance-Seleya-1.1.4/requirements/
+-rw-r--r--   0 root         (0) root         (0)        0 2022-11-07 11:29:19.000000 Finance-Seleya-1.1.4/requirements/py2.txt
+-rw-r--r--   0 root         (0) root         (0)      212 2023-02-24 05:29:06.000000 Finance-Seleya-1.1.4/requirements/py3.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-05 08:01:19.000000 Finance-Seleya-1.1.4/seleya/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-05 08:01:19.000000 Finance-Seleya-1.1.4/seleya/Toolset/
+-rw-r--r--   0 root         (0) root         (0)      107 2022-11-07 11:29:19.000000 Finance-Seleya-1.1.4/seleya/Toolset/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-05 08:01:19.000000 Finance-Seleya-1.1.4/seleya/Toolset/audit/
+-rw-r--r--   0 root         (0) root         (0)        0 2022-11-07 11:29:19.000000 Finance-Seleya-1.1.4/seleya/Toolset/audit/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     2112 2023-02-20 15:07:28.000000 Finance-Seleya-1.1.4/seleya/Toolset/audit/esg_metrics.py
+-rw-r--r--   0 root         (0) root         (0)   306958 2023-07-05 03:10:53.000000 Finance-Seleya-1.1.4/seleya/Toolset/blob_service.c
+-rw-r--r--   0 root         (0) root         (0)     3486 2023-02-20 15:07:28.000000 Finance-Seleya-1.1.4/seleya/Toolset/blob_service.pyx
+-rw-r--r--   0 root         (0) root         (0)   425791 2023-07-05 03:10:53.000000 Finance-Seleya-1.1.4/seleya/Toolset/calendar.c
+-rw-r--r--   0 root         (0) root         (0)     4827 2022-11-07 11:29:19.000000 Finance-Seleya-1.1.4/seleya/Toolset/calendar.pyx
+-rw-r--r--   0 root         (0) root         (0)   538976 2023-07-05 03:10:53.000000 Finance-Seleya-1.1.4/seleya/Toolset/file_util.c
+-rw-r--r--   0 root         (0) root         (0)     7223 2023-07-05 03:01:47.000000 Finance-Seleya-1.1.4/seleya/Toolset/file_util.pyx
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-05 08:01:19.000000 Finance-Seleya-1.1.4/seleya/Toolset/portfolio/
+-rw-r--r--   0 root         (0) root         (0)        0 2022-11-07 11:29:19.000000 Finance-Seleya-1.1.4/seleya/Toolset/portfolio/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     6676 2023-02-20 15:07:28.000000 Finance-Seleya-1.1.4/seleya/Toolset/portfolio/esg_metrics.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-05 08:01:19.000000 Finance-Seleya-1.1.4/seleya/Toolset/tests/
+-rw-r--r--   0 root         (0) root         (0)       24 2022-11-07 11:29:19.000000 Finance-Seleya-1.1.4/seleya/Toolset/tests/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      632 2022-11-07 11:29:19.000000 Finance-Seleya-1.1.4/seleya/Toolset/tests/runner.py
+-rw-r--r--   0 root         (0) root         (0)      244 2022-11-07 11:29:19.000000 Finance-Seleya-1.1.4/seleya/Toolset/tests/suite.py
+-rw-r--r--   0 root         (0) root         (0)   331551 2023-07-05 03:10:53.000000 Finance-Seleya-1.1.4/seleya/Toolset/translator.c
+-rw-r--r--   0 root         (0) root         (0)     5733 2022-11-07 11:29:19.000000 Finance-Seleya-1.1.4/seleya/Toolset/translator.pyx
+-rw-r--r--   0 root         (0) root         (0)     2074 2023-07-05 03:10:06.000000 Finance-Seleya-1.1.4/seleya/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-05 08:01:19.000000 Finance-Seleya-1.1.4/seleya/config/
+-rw-r--r--   0 root         (0) root         (0)        0 2022-11-07 11:29:19.000000 Finance-Seleya-1.1.4/seleya/config/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      489 2022-11-07 11:29:19.000000 Finance-Seleya-1.1.4/seleya/config/default_config.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-05 08:01:19.000000 Finance-Seleya-1.1.4/seleya/core/
+-rw-r--r--   0 root         (0) root         (0)        0 2022-11-11 11:55:10.000000 Finance-Seleya-1.1.4/seleya/core/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     3121 2022-11-11 11:55:10.000000 Finance-Seleya-1.1.4/seleya/core/env.pyx
+-rw-r--r--   0 root         (0) root         (0)     9714 2022-11-11 11:55:10.000000 Finance-Seleya-1.1.4/seleya/core/fixes.pyx
+-rw-r--r--   0 root         (0) root         (0)     7809 2022-11-11 11:55:10.000000 Finance-Seleya-1.1.4/seleya/core/helper.pyx
+-rw-r--r--   0 root         (0) root         (0)     1921 2022-11-11 11:55:10.000000 Finance-Seleya-1.1.4/seleya/core/parallel.pyx
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-05 08:01:19.000000 Finance-Seleya-1.1.4/seleya/data/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-05 08:01:19.000000 Finance-Seleya-1.1.4/seleya/data/DataAPI/
+-rw-r--r--   0 root         (0) root         (0)       94 2023-02-20 15:07:28.000000 Finance-Seleya-1.1.4/seleya/data/DataAPI/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-05 08:01:19.000000 Finance-Seleya-1.1.4/seleya/data/DataAPI/http/
+-rw-r--r--   0 root         (0) root         (0)     3533 2023-02-20 15:07:28.000000 Finance-Seleya-1.1.4/seleya/data/DataAPI/http/ESG.py
+-rw-r--r--   0 root         (0) root         (0)     3211 2023-02-20 15:07:28.000000 Finance-Seleya-1.1.4/seleya/data/DataAPI/http/GD.py
+-rw-r--r--   0 root         (0) root         (0)     4296 2023-02-20 15:07:28.000000 Finance-Seleya-1.1.4/seleya/data/DataAPI/http/SEARCH.py
+-rw-r--r--   0 root         (0) root         (0)     2288 2023-02-20 15:07:28.000000 Finance-Seleya-1.1.4/seleya/data/DataAPI/http/USER.py
+-rw-r--r--   0 root         (0) root         (0)      382 2023-02-20 15:07:28.000000 Finance-Seleya-1.1.4/seleya/data/DataAPI/http/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      599 2023-02-20 15:07:28.000000 Finance-Seleya-1.1.4/seleya/data/DataAPI/http/utils.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-05 08:01:19.000000 Finance-Seleya-1.1.4/seleya/data/DataAPI/mongo/
+-rw-r--r--   0 root         (0) root         (0)       62 2023-02-20 15:07:28.000000 Finance-Seleya-1.1.4/seleya/data/DataAPI/mongo/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      348 2023-02-20 15:07:28.000000 Finance-Seleya-1.1.4/seleya/data/DataAPI/mongo/fetch_engine.py
+-rw-r--r--   0 root         (0) root         (0)     2408 2023-02-20 15:07:28.000000 Finance-Seleya-1.1.4/seleya/data/DataAPI/mongo/mongodb.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-05 08:01:19.000000 Finance-Seleya-1.1.4/seleya/data/DataAPI/sqlatom/
+-rw-r--r--   0 root         (0) root         (0)      117 2023-02-20 15:07:28.000000 Finance-Seleya-1.1.4/seleya/data/DataAPI/sqlatom/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    36127 2023-02-20 15:07:28.000000 Finance-Seleya-1.1.4/seleya/data/DataAPI/sqlatom/db_factory.py
+-rw-r--r--   0 root         (0) root         (0)     7397 2023-04-17 00:03:09.000000 Finance-Seleya-1.1.4/seleya/data/DataAPI/sqlatom/fetch_engine.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-05 08:01:19.000000 Finance-Seleya-1.1.4/seleya/data/DataAPI/sqlatom/sly/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-02-20 15:07:28.000000 Finance-Seleya-1.1.4/seleya/data/DataAPI/sqlatom/sly/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    55584 2023-07-04 06:39:24.000000 Finance-Seleya-1.1.4/seleya/data/DataAPI/sqlatom/sly/sly_engine.py
+-rw-r--r--   0 root         (0) root         (0)       21 2023-02-20 15:07:28.000000 Finance-Seleya-1.1.4/seleya/data/DataAPI/version.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-05 08:01:19.000000 Finance-Seleya-1.1.4/seleya/data/SurfaceAPI/
+-rw-r--r--   0 root         (0) root         (0)       23 2023-02-20 15:07:28.000000 Finance-Seleya-1.1.4/seleya/data/SurfaceAPI/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-05 08:01:19.000000 Finance-Seleya-1.1.4/seleya/data/SurfaceAPI/mongo/
+-rw-r--r--   0 root         (0) root         (0)      383 2023-02-28 01:50:45.000000 Finance-Seleya-1.1.4/seleya/data/SurfaceAPI/mongo/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      633 2023-02-28 12:53:15.000000 Finance-Seleya-1.1.4/seleya/data/SurfaceAPI/mongo/basic.py
+-rw-r--r--   0 root         (0) root         (0)     2042 2023-03-03 01:31:51.000000 Finance-Seleya-1.1.4/seleya/data/SurfaceAPI/mongo/engine.py
+-rw-r--r--   0 root         (0) root         (0)     1265 2023-02-28 10:24:23.000000 Finance-Seleya-1.1.4/seleya/data/SurfaceAPI/mongo/gd_qrank_dist.py
+-rw-r--r--   0 root         (0) root         (0)     1168 2023-02-24 05:29:06.000000 Finance-Seleya-1.1.4/seleya/data/SurfaceAPI/mongo/gd_qrank_raw.py
+-rw-r--r--   0 root         (0) root         (0)      866 2023-02-28 01:50:45.000000 Finance-Seleya-1.1.4/seleya/data/SurfaceAPI/mongo/gic_dist_level1.py
+-rw-r--r--   0 root         (0) root         (0)      877 2023-02-28 12:26:53.000000 Finance-Seleya-1.1.4/seleya/data/SurfaceAPI/mongo/non_gic_dist_level1.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-05 08:01:19.000000 Finance-Seleya-1.1.4/seleya/data/SurfaceAPI/sqlatom/
+-rw-r--r--   0 root         (0) root         (0)     1098 2023-03-28 11:57:26.000000 Finance-Seleya-1.1.4/seleya/data/SurfaceAPI/sqlatom/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      937 2023-03-02 23:18:44.000000 Finance-Seleya-1.1.4/seleya/data/SurfaceAPI/sqlatom/basic.py
+-rw-r--r--   0 root         (0) root         (0)      626 2023-03-01 14:55:21.000000 Finance-Seleya-1.1.4/seleya/data/SurfaceAPI/sqlatom/co2_emission_target.py
+-rw-r--r--   0 root         (0) root         (0)      537 2023-03-02 23:18:57.000000 Finance-Seleya-1.1.4/seleya/data/SurfaceAPI/sqlatom/company.py
+-rw-r--r--   0 root         (0) root         (0)      527 2023-03-02 01:54:52.000000 Finance-Seleya-1.1.4/seleya/data/SurfaceAPI/sqlatom/company_emission_temperature.py
+-rw-r--r--   0 root         (0) root         (0)      525 2023-03-02 02:20:33.000000 Finance-Seleya-1.1.4/seleya/data/SurfaceAPI/sqlatom/emission_score_average.py
+-rw-r--r--   0 root         (0) root         (0)     1687 2023-03-30 06:02:56.000000 Finance-Seleya-1.1.4/seleya/data/SurfaceAPI/sqlatom/engine.py
+-rw-r--r--   0 root         (0) root         (0)      836 2023-02-28 01:50:45.000000 Finance-Seleya-1.1.4/seleya/data/SurfaceAPI/sqlatom/feature_importance.py
+-rw-r--r--   0 root         (0) root         (0)      497 2023-02-20 15:07:28.000000 Finance-Seleya-1.1.4/seleya/data/SurfaceAPI/sqlatom/gd_overview.py
+-rw-r--r--   0 root         (0) root         (0)      611 2023-02-20 15:07:28.000000 Finance-Seleya-1.1.4/seleya/data/SurfaceAPI/sqlatom/gd_reviews.py
+-rw-r--r--   0 root         (0) root         (0)      624 2023-03-28 12:22:57.000000 Finance-Seleya-1.1.4/seleya/data/SurfaceAPI/sqlatom/gd_reviews_base.py
+-rw-r--r--   0 root         (0) root         (0)     2388 2023-03-28 12:11:51.000000 Finance-Seleya-1.1.4/seleya/data/SurfaceAPI/sqlatom/industry.py
+-rw-r--r--   0 root         (0) root         (0)     2475 2023-03-16 08:51:54.000000 Finance-Seleya-1.1.4/seleya/data/SurfaceAPI/sqlatom/metrics.py
+-rw-r--r--   0 root         (0) root         (0)      700 2023-02-24 05:29:06.000000 Finance-Seleya-1.1.4/seleya/data/SurfaceAPI/sqlatom/sasb_mapdom.py
+-rw-r--r--   0 root         (0) root         (0)      836 2023-02-28 01:50:45.000000 Finance-Seleya-1.1.4/seleya/data/SurfaceAPI/sqlatom/sector.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-02-20 15:07:28.000000 Finance-Seleya-1.1.4/seleya/data/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-05 08:01:19.000000 Finance-Seleya-1.1.4/seleya/mfc/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-02-20 15:07:28.000000 Finance-Seleya-1.1.4/seleya/mfc/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-05 08:01:19.000000 Finance-Seleya-1.1.4/seleya/mfc/alchemy/
+-rw-r--r--   0 root         (0) root         (0)      284 2023-03-16 07:14:16.000000 Finance-Seleya-1.1.4/seleya/mfc/alchemy/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-05 08:01:19.000000 Finance-Seleya-1.1.4/seleya/mfc/alchemy/qrank/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-02-20 15:07:28.000000 Finance-Seleya-1.1.4/seleya/mfc/alchemy/qrank/__init__.py
+-rw-r--r--   0 root         (0) root         (0)   505167 2023-07-05 03:10:53.000000 Finance-Seleya-1.1.4/seleya/mfc/alchemy/qrank/glassdoor.c
+-rw-r--r--   0 root         (0) root         (0)     7687 2023-06-24 10:01:03.000000 Finance-Seleya-1.1.4/seleya/mfc/alchemy/qrank/glassdoor.pyx
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-05 08:01:19.000000 Finance-Seleya-1.1.4/seleya/mfc/alchemy/sbti/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-03-01 14:22:17.000000 Finance-Seleya-1.1.4/seleya/mfc/alchemy/sbti/__init__.py
+-rw-r--r--   0 root         (0) root         (0)   886071 2023-07-05 03:10:53.000000 Finance-Seleya-1.1.4/seleya/mfc/alchemy/sbti/emission.c
+-rw-r--r--   0 root         (0) root         (0)    22737 2023-04-02 13:21:46.000000 Finance-Seleya-1.1.4/seleya/mfc/alchemy/sbti/emission.pyx
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-05 08:01:19.000000 Finance-Seleya-1.1.4/seleya/mfc/alchemy/tsi/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-02-28 01:50:45.000000 Finance-Seleya-1.1.4/seleya/mfc/alchemy/tsi/__init__.py
+-rw-r--r--   0 root         (0) root         (0)   469404 2023-07-05 03:10:53.000000 Finance-Seleya-1.1.4/seleya/mfc/alchemy/tsi/aerosol.c
+-rw-r--r--   0 root         (0) root         (0)     7878 2023-03-17 00:13:38.000000 Finance-Seleya-1.1.4/seleya/mfc/alchemy/tsi/aerosol.pyx
+-rw-r--r--   0 root         (0) root         (0)   501218 2023-07-05 03:10:53.000000 Finance-Seleya-1.1.4/seleya/mfc/alchemy/tsi/s2f.c
+-rw-r--r--   0 root         (0) root         (0)    11460 2023-03-10 06:20:30.000000 Finance-Seleya-1.1.4/seleya/mfc/alchemy/tsi/s2f.pyx
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-05 08:01:19.000000 Finance-Seleya-1.1.4/seleya/mfc/micro/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-02-06 13:27:54.000000 Finance-Seleya-1.1.4/seleya/mfc/micro/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      132 2022-11-07 11:29:19.000000 Finance-Seleya-1.1.4/seleya/seleya.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-05 08:01:19.000000 Finance-Seleya-1.1.4/seleya/utilities/
+-rw-r--r--   0 root         (0) root         (0)        0 2022-11-07 11:29:19.000000 Finance-Seleya-1.1.4/seleya/utilities/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     3293 2022-11-07 11:29:19.000000 Finance-Seleya-1.1.4/seleya/utilities/api_base.py
+-rw-r--r--   0 root         (0) root         (0)      418 2023-03-03 01:22:19.000000 Finance-Seleya-1.1.4/seleya/utilities/exceptions.py
+-rw-r--r--   0 root         (0) root         (0)     5108 2023-02-20 15:07:28.000000 Finance-Seleya-1.1.4/seleya/utilities/kd_logger.py
+-rw-r--r--   0 root         (0) root         (0)      490 2022-11-07 11:29:19.000000 Finance-Seleya-1.1.4/seleya/utilities/singleton.py
+-rw-r--r--   0 root         (0) root         (0)      399 2022-11-07 11:29:19.000000 Finance-Seleya-1.1.4/seleya/utilities/warning.py
+-rw-r--r--   0 root         (0) root         (0)       21 2023-07-05 08:00:55.000000 Finance-Seleya-1.1.4/seleya/version.py
+-rw-r--r--   0 root         (0) root         (0)       38 2023-07-05 08:01:19.000000 Finance-Seleya-1.1.4/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     3762 2023-07-05 06:18:11.000000 Finance-Seleya-1.1.4/setup.py
```

### Comparing `Finance-Seleya-1.1.3/Finance_Seleya.egg-info/SOURCES.txt` & `Finance-Seleya-1.1.4/Finance_Seleya.egg-info/SOURCES.txt`

 * *Files 10% similar despite different names*

```diff
@@ -9,32 +9,36 @@
 Finance_Seleya.egg-info/top_level.txt
 requirements/py2.txt
 requirements/py3.txt
 seleya/__init__.py
 seleya/seleya.py
 seleya/version.py
 seleya/Toolset/__init__.py
-seleya/Toolset/blob_service.py
-seleya/Toolset/calendar.py
-seleya/Toolset/file_util.py
-seleya/Toolset/translator.py
+seleya/Toolset/blob_service.c
+seleya/Toolset/blob_service.pyx
+seleya/Toolset/calendar.c
+seleya/Toolset/calendar.pyx
+seleya/Toolset/file_util.c
+seleya/Toolset/file_util.pyx
+seleya/Toolset/translator.c
+seleya/Toolset/translator.pyx
 seleya/Toolset/audit/__init__.py
 seleya/Toolset/audit/esg_metrics.py
 seleya/Toolset/portfolio/__init__.py
 seleya/Toolset/portfolio/esg_metrics.py
 seleya/Toolset/tests/__init__.py
 seleya/Toolset/tests/runner.py
 seleya/Toolset/tests/suite.py
 seleya/config/__init__.py
 seleya/config/default_config.py
 seleya/core/__init__.py
-seleya/core/env.py
-seleya/core/fixes.py
-seleya/core/helper.py
-seleya/core/parallel.py
+seleya/core/env.pyx
+seleya/core/fixes.pyx
+seleya/core/helper.pyx
+seleya/core/parallel.pyx
 seleya/data/__init__.py
 seleya/data/DataAPI/__init__.py
 seleya/data/DataAPI/version.py
 seleya/data/DataAPI/http/ESG.py
 seleya/data/DataAPI/http/GD.py
 seleya/data/DataAPI/http/SEARCH.py
 seleya/data/DataAPI/http/USER.py
@@ -69,21 +73,25 @@
 seleya/data/SurfaceAPI/sqlatom/gd_reviews_base.py
 seleya/data/SurfaceAPI/sqlatom/industry.py
 seleya/data/SurfaceAPI/sqlatom/metrics.py
 seleya/data/SurfaceAPI/sqlatom/sasb_mapdom.py
 seleya/data/SurfaceAPI/sqlatom/sector.py
 seleya/mfc/__init__.py
 seleya/mfc/alchemy/__init__.py
-seleya/mfc/alchemy/qrank/glassdoo.cpython-37m-x86_64-linux-gnu.so
+seleya/mfc/alchemy/qrank/__init__.py
 seleya/mfc/alchemy/qrank/glassdoor.c
+seleya/mfc/alchemy/qrank/glassdoor.pyx
 seleya/mfc/alchemy/sbti/__init__.py
-seleya/mfc/alchemy/sbti/emission.py
+seleya/mfc/alchemy/sbti/emission.c
+seleya/mfc/alchemy/sbti/emission.pyx
 seleya/mfc/alchemy/tsi/__init__.py
-seleya/mfc/alchemy/tsi/aerosol.py
-seleya/mfc/alchemy/tsi/s2f.py
+seleya/mfc/alchemy/tsi/aerosol.c
+seleya/mfc/alchemy/tsi/aerosol.pyx
+seleya/mfc/alchemy/tsi/s2f.c
+seleya/mfc/alchemy/tsi/s2f.pyx
 seleya/mfc/micro/__init__.py
 seleya/utilities/__init__.py
 seleya/utilities/api_base.py
 seleya/utilities/exceptions.py
 seleya/utilities/kd_logger.py
 seleya/utilities/singleton.py
 seleya/utilities/warning.py
```

### Comparing `Finance-Seleya-1.1.3/seleya/Toolset/audit/esg_metrics.py` & `Finance-Seleya-1.1.4/seleya/Toolset/audit/esg_metrics.py`

 * *Files identical despite different names*

### Comparing `Finance-Seleya-1.1.3/seleya/Toolset/blob_service.py` & `Finance-Seleya-1.1.4/seleya/Toolset/blob_service.pyx`

 * *Files identical despite different names*

### Comparing `Finance-Seleya-1.1.3/seleya/Toolset/calendar.py` & `Finance-Seleya-1.1.4/seleya/Toolset/calendar.pyx`

 * *Files identical despite different names*

### Comparing `Finance-Seleya-1.1.3/seleya/Toolset/file_util.py` & `Finance-Seleya-1.1.4/seleya/Toolset/file_util.pyx`

 * *Files identical despite different names*

### Comparing `Finance-Seleya-1.1.3/seleya/Toolset/portfolio/esg_metrics.py` & `Finance-Seleya-1.1.4/seleya/Toolset/portfolio/esg_metrics.py`

 * *Files identical despite different names*

### Comparing `Finance-Seleya-1.1.3/seleya/Toolset/tests/runner.py` & `Finance-Seleya-1.1.4/seleya/Toolset/tests/runner.py`

 * *Files identical despite different names*

### Comparing `Finance-Seleya-1.1.3/seleya/Toolset/translator.py` & `Finance-Seleya-1.1.4/seleya/Toolset/translator.pyx`

 * *Files identical despite different names*

### Comparing `Finance-Seleya-1.1.3/seleya/__init__.py` & `Finance-Seleya-1.1.4/seleya/__init__.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,16 @@
 # -*- coding: utf-8 -*-
 from __future__ import print_function
 from __future__ import absolute_import
 from __future__ import unicode_literals
 
 import warnings, requests, os, pdb
 
+from .version import __version__
+
 #defaul_url = 'https://ultronsandbox.oss-cn-hangzhou.aliyuncs.com/version/seleya.json'
 default_url = 'https://seleya.blob.core.windows.net/nsark'
 version_url = "{}/{}/{}".format(os.environ.get('jdw_version_url', default_url),
                                 'version', 'seleya.json')
 #try:
 from . import seleya
 from .data.DataAPI.sqlatom.fetch_engine import FetchEngine as DBFetchEngine
@@ -32,16 +34,14 @@
     from ultron.factor.data.processing import factor_processing
     from ultron import sentry
 except ImportError:
     warnings.warn(
         "If you need high-performance computing，please install Finance-Ultron.First make sure that the C++ compilation environment has been installed"
     )
 
-from .version import __version__
-
 session = requests.Session()
 
 
 def get_version():
     res = requests.get(version_url).json()
     if res.get('code') != 200:
         return '', ''
```

### Comparing `Finance-Seleya-1.1.3/seleya/core/env.py` & `Finance-Seleya-1.1.4/seleya/core/env.pyx`

 * *Files identical despite different names*

### Comparing `Finance-Seleya-1.1.3/seleya/core/fixes.py` & `Finance-Seleya-1.1.4/seleya/core/fixes.pyx`

 * *Files identical despite different names*

### Comparing `Finance-Seleya-1.1.3/seleya/core/helper.py` & `Finance-Seleya-1.1.4/seleya/core/helper.pyx`

 * *Files identical despite different names*

### Comparing `Finance-Seleya-1.1.3/seleya/core/parallel.py` & `Finance-Seleya-1.1.4/seleya/core/parallel.pyx`

 * *Files identical despite different names*

### Comparing `Finance-Seleya-1.1.3/seleya/data/DataAPI/http/ESG.py` & `Finance-Seleya-1.1.4/seleya/data/DataAPI/http/ESG.py`

 * *Files identical despite different names*

### Comparing `Finance-Seleya-1.1.3/seleya/data/DataAPI/http/GD.py` & `Finance-Seleya-1.1.4/seleya/data/DataAPI/http/GD.py`

 * *Files identical despite different names*

### Comparing `Finance-Seleya-1.1.3/seleya/data/DataAPI/http/SEARCH.py` & `Finance-Seleya-1.1.4/seleya/data/DataAPI/http/SEARCH.py`

 * *Files identical despite different names*

### Comparing `Finance-Seleya-1.1.3/seleya/data/DataAPI/http/USER.py` & `Finance-Seleya-1.1.4/seleya/data/DataAPI/http/USER.py`

 * *Files identical despite different names*

### Comparing `Finance-Seleya-1.1.3/seleya/data/DataAPI/http/utils.py` & `Finance-Seleya-1.1.4/seleya/data/DataAPI/http/utils.py`

 * *Files identical despite different names*

### Comparing `Finance-Seleya-1.1.3/seleya/data/DataAPI/mongo/mongodb.py` & `Finance-Seleya-1.1.4/seleya/data/DataAPI/mongo/mongodb.py`

 * *Files identical despite different names*

### Comparing `Finance-Seleya-1.1.3/seleya/data/DataAPI/sqlatom/db_factory.py` & `Finance-Seleya-1.1.4/seleya/data/DataAPI/sqlatom/db_factory.py`

 * *Files identical despite different names*

### Comparing `Finance-Seleya-1.1.3/seleya/data/DataAPI/sqlatom/fetch_engine.py` & `Finance-Seleya-1.1.4/seleya/data/DataAPI/sqlatom/fetch_engine.py`

 * *Files identical despite different names*

### Comparing `Finance-Seleya-1.1.3/seleya/data/DataAPI/sqlatom/sly/sly_engine.py` & `Finance-Seleya-1.1.4/seleya/data/DataAPI/sqlatom/sly/sly_engine.py`

 * *Files identical despite different names*

### Comparing `Finance-Seleya-1.1.3/seleya/data/SurfaceAPI/mongo/basic.py` & `Finance-Seleya-1.1.4/seleya/data/SurfaceAPI/mongo/basic.py`

 * *Files identical despite different names*

### Comparing `Finance-Seleya-1.1.3/seleya/data/SurfaceAPI/mongo/engine.py` & `Finance-Seleya-1.1.4/seleya/data/SurfaceAPI/mongo/engine.py`

 * *Files identical despite different names*

### Comparing `Finance-Seleya-1.1.3/seleya/data/SurfaceAPI/mongo/gd_qrank_dist.py` & `Finance-Seleya-1.1.4/seleya/data/SurfaceAPI/mongo/gd_qrank_dist.py`

 * *Files identical despite different names*

### Comparing `Finance-Seleya-1.1.3/seleya/data/SurfaceAPI/mongo/gd_qrank_raw.py` & `Finance-Seleya-1.1.4/seleya/data/SurfaceAPI/mongo/gd_qrank_raw.py`

 * *Files identical despite different names*

### Comparing `Finance-Seleya-1.1.3/seleya/data/SurfaceAPI/mongo/gic_dist_level1.py` & `Finance-Seleya-1.1.4/seleya/data/SurfaceAPI/mongo/gic_dist_level1.py`

 * *Files identical despite different names*

### Comparing `Finance-Seleya-1.1.3/seleya/data/SurfaceAPI/mongo/non_gic_dist_level1.py` & `Finance-Seleya-1.1.4/seleya/data/SurfaceAPI/mongo/non_gic_dist_level1.py`

 * *Files identical despite different names*

### Comparing `Finance-Seleya-1.1.3/seleya/data/SurfaceAPI/sqlatom/__init__.py` & `Finance-Seleya-1.1.4/seleya/data/SurfaceAPI/sqlatom/__init__.py`

 * *Files identical despite different names*

### Comparing `Finance-Seleya-1.1.3/seleya/data/SurfaceAPI/sqlatom/basic.py` & `Finance-Seleya-1.1.4/seleya/data/SurfaceAPI/sqlatom/basic.py`

 * *Files identical despite different names*

### Comparing `Finance-Seleya-1.1.3/seleya/data/SurfaceAPI/sqlatom/co2_emission_target.py` & `Finance-Seleya-1.1.4/seleya/data/SurfaceAPI/sqlatom/co2_emission_target.py`

 * *Files identical despite different names*

### Comparing `Finance-Seleya-1.1.3/seleya/data/SurfaceAPI/sqlatom/company.py` & `Finance-Seleya-1.1.4/seleya/data/SurfaceAPI/sqlatom/company.py`

 * *Files identical despite different names*

### Comparing `Finance-Seleya-1.1.3/seleya/data/SurfaceAPI/sqlatom/company_emission_temperature.py` & `Finance-Seleya-1.1.4/seleya/data/SurfaceAPI/sqlatom/company_emission_temperature.py`

 * *Files identical despite different names*

### Comparing `Finance-Seleya-1.1.3/seleya/data/SurfaceAPI/sqlatom/emission_score_average.py` & `Finance-Seleya-1.1.4/seleya/data/SurfaceAPI/sqlatom/emission_score_average.py`

 * *Files identical despite different names*

### Comparing `Finance-Seleya-1.1.3/seleya/data/SurfaceAPI/sqlatom/engine.py` & `Finance-Seleya-1.1.4/seleya/data/SurfaceAPI/sqlatom/engine.py`

 * *Files identical despite different names*

### Comparing `Finance-Seleya-1.1.3/seleya/data/SurfaceAPI/sqlatom/feature_importance.py` & `Finance-Seleya-1.1.4/seleya/data/SurfaceAPI/sqlatom/feature_importance.py`

 * *Files identical despite different names*

### Comparing `Finance-Seleya-1.1.3/seleya/data/SurfaceAPI/sqlatom/gd_reviews.py` & `Finance-Seleya-1.1.4/seleya/data/SurfaceAPI/sqlatom/gd_reviews.py`

 * *Files identical despite different names*

### Comparing `Finance-Seleya-1.1.3/seleya/data/SurfaceAPI/sqlatom/gd_reviews_base.py` & `Finance-Seleya-1.1.4/seleya/data/SurfaceAPI/sqlatom/gd_reviews_base.py`

 * *Files identical despite different names*

### Comparing `Finance-Seleya-1.1.3/seleya/data/SurfaceAPI/sqlatom/industry.py` & `Finance-Seleya-1.1.4/seleya/data/SurfaceAPI/sqlatom/industry.py`

 * *Files identical despite different names*

### Comparing `Finance-Seleya-1.1.3/seleya/data/SurfaceAPI/sqlatom/metrics.py` & `Finance-Seleya-1.1.4/seleya/data/SurfaceAPI/sqlatom/metrics.py`

 * *Files identical despite different names*

### Comparing `Finance-Seleya-1.1.3/seleya/data/SurfaceAPI/sqlatom/sasb_mapdom.py` & `Finance-Seleya-1.1.4/seleya/data/SurfaceAPI/sqlatom/sasb_mapdom.py`

 * *Files identical despite different names*

### Comparing `Finance-Seleya-1.1.3/seleya/data/SurfaceAPI/sqlatom/sector.py` & `Finance-Seleya-1.1.4/seleya/data/SurfaceAPI/sqlatom/sector.py`

 * *Files identical despite different names*

### Comparing `Finance-Seleya-1.1.3/seleya/mfc/alchemy/qrank/glassdoor.c` & `Finance-Seleya-1.1.4/seleya/mfc/alchemy/qrank/glassdoor.c`

 * *Files 1% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 /* Generated by Cython 0.29.21 */
 
 /* BEGIN: Cython Metadata
 {
     "distutils": {
-        "name": "seleya.mfc.alchemy.qrank.glassdoo",
+        "name": "seleya.mfc.alchemy.qrank.glassdoor",
         "sources": [
-            "seleya/mfc/alchemy/qrank/glassdoor.py"
+            "seleya/mfc/alchemy/qrank/glassdoor.pyx"
         ]
     },
-    "module_name": "seleya.mfc.alchemy.qrank.glassdoo"
+    "module_name": "seleya.mfc.alchemy.qrank.glassdoor"
 }
 END: Cython Metadata */
 
 #define PY_SSIZE_T_CLEAN
 #include "Python.h"
 #ifndef Py_PYTHON_H
     #error Python headers needed to compile C extensions, please install development version of Python.
@@ -610,16 +610,16 @@
   #ifdef __cplusplus
     #define __PYX_EXTERN_C extern "C"
   #else
     #define __PYX_EXTERN_C extern
   #endif
 #endif
 
-#define __PYX_HAVE__seleya__mfc__alchemy__qrank__glassdoo
-#define __PYX_HAVE_API__seleya__mfc__alchemy__qrank__glassdoo
+#define __PYX_HAVE__seleya__mfc__alchemy__qrank__glassdoor
+#define __PYX_HAVE_API__seleya__mfc__alchemy__qrank__glassdoor
 /* Early includes */
 #ifdef _OPENMP
 #include <omp.h>
 #endif /* _OPENMP */
 
 #if defined(PYREX_WITHOUT_ASSERTIONS) && !defined(CYTHON_WITHOUT_ASSERTIONS)
 #define CYTHON_WITHOUT_ASSERTIONS
@@ -821,57 +821,57 @@
 static int __pyx_lineno;
 static int __pyx_clineno = 0;
 static const char * __pyx_cfilenm= __FILE__;
 static const char *__pyx_filename;
 
 
 static const char *__pyx_f[] = {
-  "seleya/mfc/alchemy/qrank/glassdoor.py",
+  "seleya/mfc/alchemy/qrank/glassdoor.pyx",
 };
 
 /*--- Type declarations ---*/
-struct __pyx_obj_6seleya_3mfc_7alchemy_5qrank_8glassdoo___pyx_scope_struct___fetch_reviews;
-struct __pyx_obj_6seleya_3mfc_7alchemy_5qrank_8glassdoo___pyx_scope_struct_1__distribute;
-struct __pyx_obj_6seleya_3mfc_7alchemy_5qrank_8glassdoo___pyx_scope_struct_2_calculate_result;
+struct __pyx_obj_6seleya_3mfc_7alchemy_5qrank_9glassdoor___pyx_scope_struct___fetch_reviews;
+struct __pyx_obj_6seleya_3mfc_7alchemy_5qrank_9glassdoor___pyx_scope_struct_1__distribute;
+struct __pyx_obj_6seleya_3mfc_7alchemy_5qrank_9glassdoor___pyx_scope_struct_2_calculate_result;
 
-/* "seleya/mfc/alchemy/qrank/glassdoor.py":42
+/* "seleya/mfc/alchemy/qrank/glassdoor.pyx":42
  *         return gd_overview_data
  * 
  *     def _fetch_reviews(self, begin_date, end_date, cids):             # <<<<<<<<<<<<<<
  *         kd_logger.info('Fetching glassdoor reviews data...')
  *         columns = ['id', 'cid', 'reviewId', 'reviewDateTime'
  */
-struct __pyx_obj_6seleya_3mfc_7alchemy_5qrank_8glassdoo___pyx_scope_struct___fetch_reviews {
+struct __pyx_obj_6seleya_3mfc_7alchemy_5qrank_9glassdoor___pyx_scope_struct___fetch_reviews {
   PyObject_HEAD
   PyObject *__pyx_v_self;
 };
 
 
-/* "seleya/mfc/alchemy/qrank/glassdoor.py":119
+/* "seleya/mfc/alchemy/qrank/glassdoor.pyx":119
  *         return scores
  * 
  *     def _distribute(self, mean_data):             # <<<<<<<<<<<<<<
  *         dt = mean_data.set_index(['date', 'code', 'name'])['value']
  *         res = []
  */
-struct __pyx_obj_6seleya_3mfc_7alchemy_5qrank_8glassdoo___pyx_scope_struct_1__distribute {
+struct __pyx_obj_6seleya_3mfc_7alchemy_5qrank_9glassdoor___pyx_scope_struct_1__distribute {
   PyObject_HEAD
   PyObject *__pyx_v_res;
   PyObject *__pyx_v_self;
 };
 
 
-/* "seleya/mfc/alchemy/qrank/glassdoor.py":153
+/* "seleya/mfc/alchemy/qrank/glassdoor.pyx":153
  *         return mean_data
  * 
  *     def calculate_result(self, total_data, threshold=0.9):             # <<<<<<<<<<<<<<
  *         # aggregate means by year and cid
  *         mean_data = total_data.groupby(['date', 'code']).mean()
  */
-struct __pyx_obj_6seleya_3mfc_7alchemy_5qrank_8glassdoo___pyx_scope_struct_2_calculate_result {
+struct __pyx_obj_6seleya_3mfc_7alchemy_5qrank_9glassdoor___pyx_scope_struct_2_calculate_result {
   PyObject_HEAD
   PyObject *__pyx_v_col_name;
   PyObject *__pyx_v_self;
   PyObject *__pyx_v_threshold;
 };
 
 
@@ -1358,23 +1358,23 @@
 /* CheckBinaryVersion.proto */
 static int __Pyx_check_binary_version(void);
 
 /* InitStrings.proto */
 static int __Pyx_InitStrings(__Pyx_StringTabEntry *t);
 
 
-/* Module declarations from 'seleya.mfc.alchemy.qrank.glassdoo' */
-static PyTypeObject *__pyx_ptype_6seleya_3mfc_7alchemy_5qrank_8glassdoo___pyx_scope_struct___fetch_reviews = 0;
-static PyTypeObject *__pyx_ptype_6seleya_3mfc_7alchemy_5qrank_8glassdoo___pyx_scope_struct_1__distribute = 0;
-static PyTypeObject *__pyx_ptype_6seleya_3mfc_7alchemy_5qrank_8glassdoo___pyx_scope_struct_2_calculate_result = 0;
-#define __Pyx_MODULE_NAME "seleya.mfc.alchemy.qrank.glassdoo"
-extern int __pyx_module_is_main_seleya__mfc__alchemy__qrank__glassdoo;
-int __pyx_module_is_main_seleya__mfc__alchemy__qrank__glassdoo = 0;
+/* Module declarations from 'seleya.mfc.alchemy.qrank.glassdoor' */
+static PyTypeObject *__pyx_ptype_6seleya_3mfc_7alchemy_5qrank_9glassdoor___pyx_scope_struct___fetch_reviews = 0;
+static PyTypeObject *__pyx_ptype_6seleya_3mfc_7alchemy_5qrank_9glassdoor___pyx_scope_struct_1__distribute = 0;
+static PyTypeObject *__pyx_ptype_6seleya_3mfc_7alchemy_5qrank_9glassdoor___pyx_scope_struct_2_calculate_result = 0;
+#define __Pyx_MODULE_NAME "seleya.mfc.alchemy.qrank.glassdoor"
+extern int __pyx_module_is_main_seleya__mfc__alchemy__qrank__glassdoor;
+int __pyx_module_is_main_seleya__mfc__alchemy__qrank__glassdoor = 0;
 
-/* Implementation of 'seleya.mfc.alchemy.qrank.glassdoo' */
+/* Implementation of 'seleya.mfc.alchemy.qrank.glassdoor' */
 static PyObject *__pyx_builtin_object;
 static PyObject *__pyx_builtin_range;
 static const char __pyx_k_[] = "*";
 static const char __pyx_k_n[] = "n";
 static const char __pyx_k_x[] = "x";
 static const char __pyx_k_by[] = "by";
 static const char __pyx_k_dt[] = "dt";
@@ -1551,16 +1551,16 @@
 static const char __pyx_k_Glassdoor__calculate_distribute[] = "Glassdoor._calculate_distribute";
 static const char __pyx_k_Glassdoor__fetch_reviews_locals[] = "Glassdoor._fetch_reviews.<locals>.<lambda>";
 static const char __pyx_k_Glassdoor_reviews_data_is_empty[] = "Glassdoor reviews data is empty";
 static const char __pyx_k_Fetching_glassdoor_overview_data[] = "Fetching glassdoor overview data...";
 static const char __pyx_k_Glassdoor__distribute_locals_lam[] = "Glassdoor._distribute.<locals>.<lambda>";
 static const char __pyx_k_Glassdoor_calculate_result_local[] = "Glassdoor.calculate_result.<locals>.<lambda>";
 static const char __pyx_k_Glassdoor_overview_data_is_empty[] = "Glassdoor overview data is empty";
-static const char __pyx_k_seleya_mfc_alchemy_qrank_glassdo[] = "seleya.mfc.alchemy.qrank.glassdoo";
-static const char __pyx_k_seleya_mfc_alchemy_qrank_glassdo_2[] = "seleya/mfc/alchemy/qrank/glassdoor.py";
+static const char __pyx_k_seleya_mfc_alchemy_qrank_glassdo[] = "seleya.mfc.alchemy.qrank.glassdoor";
+static const char __pyx_k_seleya_mfc_alchemy_qrank_glassdo_2[] = "seleya/mfc/alchemy/qrank/glassdoor.pyx";
 static PyObject *__pyx_n_s_;
 static PyObject *__pyx_n_s_APPROVE;
 static PyObject *__pyx_n_s_CSQuantiles;
 static PyObject *__pyx_n_s_DISAPPROVE;
 static PyObject *__pyx_n_s_DataFrame;
 static PyObject *__pyx_kp_s_Fetching_glassdoor_overview_data;
 static PyObject *__pyx_kp_s_Fetching_glassdoor_reviews_data;
@@ -1737,32 +1737,32 @@
 static PyObject *__pyx_n_s_transform_raw;
 static PyObject *__pyx_n_s_ultron_sentry_api;
 static PyObject *__pyx_n_s_unique;
 static PyObject *__pyx_n_s_unstack;
 static PyObject *__pyx_n_s_value;
 static PyObject *__pyx_n_s_values_series;
 static PyObject *__pyx_n_s_x;
-static PyObject *__pyx_pf_6seleya_3mfc_7alchemy_5qrank_8glassdoo_9Glassdoor___init__(CYTHON_UNUSED PyObject *__pyx_self, PyObject *__pyx_v_self, PyObject *__pyx_v_industry_code); /* proto */
-static PyObject *__pyx_pf_6seleya_3mfc_7alchemy_5qrank_8glassdoo_9Glassdoor_2_fetch_overview(CYTHON_UNUSED PyObject *__pyx_self, CYTHON_UNUSED PyObject *__pyx_v_self, PyObject *__pyx_v_codes); /* proto */
+static PyObject *__pyx_pf_6seleya_3mfc_7alchemy_5qrank_9glassdoor_9Glassdoor___init__(CYTHON_UNUSED PyObject *__pyx_self, PyObject *__pyx_v_self, PyObject *__pyx_v_industry_code); /* proto */
+static PyObject *__pyx_pf_6seleya_3mfc_7alchemy_5qrank_9glassdoor_9Glassdoor_2_fetch_overview(CYTHON_UNUSED PyObject *__pyx_self, CYTHON_UNUSED PyObject *__pyx_v_self, PyObject *__pyx_v_codes); /* proto */
 static PyObject *__pyx_lambda_funcdef_lambda(PyObject *__pyx_self, PyObject *__pyx_v_x); /* proto */
-static PyObject *__pyx_pf_6seleya_3mfc_7alchemy_5qrank_8glassdoo_9Glassdoor_4_fetch_reviews(CYTHON_UNUSED PyObject *__pyx_self, PyObject *__pyx_v_self, PyObject *__pyx_v_begin_date, PyObject *__pyx_v_end_date, PyObject *__pyx_v_cids); /* proto */
-static PyObject *__pyx_pf_6seleya_3mfc_7alchemy_5qrank_8glassdoo_9Glassdoor_6prepare_data(CYTHON_UNUSED PyObject *__pyx_self, PyObject *__pyx_v_self, PyObject *__pyx_v_begin_date, PyObject *__pyx_v_end_date); /* proto */
-static PyObject *__pyx_pf_6seleya_3mfc_7alchemy_5qrank_8glassdoo_9Glassdoor_8_transform_raw(CYTHON_UNUSED PyObject *__pyx_self, PyObject *__pyx_v_self, PyObject *__pyx_v_mean_data); /* proto */
-static PyObject *__pyx_pf_6seleya_3mfc_7alchemy_5qrank_8glassdoo_9Glassdoor_10_blom_score(CYTHON_UNUSED PyObject *__pyx_self, CYTHON_UNUSED PyObject *__pyx_v_self, PyObject *__pyx_v_values_series, PyObject *__pyx_v_threshold); /* proto */
+static PyObject *__pyx_pf_6seleya_3mfc_7alchemy_5qrank_9glassdoor_9Glassdoor_4_fetch_reviews(CYTHON_UNUSED PyObject *__pyx_self, PyObject *__pyx_v_self, PyObject *__pyx_v_begin_date, PyObject *__pyx_v_end_date, PyObject *__pyx_v_cids); /* proto */
+static PyObject *__pyx_pf_6seleya_3mfc_7alchemy_5qrank_9glassdoor_9Glassdoor_6prepare_data(CYTHON_UNUSED PyObject *__pyx_self, PyObject *__pyx_v_self, PyObject *__pyx_v_begin_date, PyObject *__pyx_v_end_date); /* proto */
+static PyObject *__pyx_pf_6seleya_3mfc_7alchemy_5qrank_9glassdoor_9Glassdoor_8_transform_raw(CYTHON_UNUSED PyObject *__pyx_self, PyObject *__pyx_v_self, PyObject *__pyx_v_mean_data); /* proto */
+static PyObject *__pyx_pf_6seleya_3mfc_7alchemy_5qrank_9glassdoor_9Glassdoor_10_blom_score(CYTHON_UNUSED PyObject *__pyx_self, CYTHON_UNUSED PyObject *__pyx_v_self, PyObject *__pyx_v_values_series, PyObject *__pyx_v_threshold); /* proto */
 static PyObject *__pyx_lambda_funcdef_lambda1(PyObject *__pyx_self, PyObject *__pyx_v_x); /* proto */
-static PyObject *__pyx_pf_6seleya_3mfc_7alchemy_5qrank_8glassdoo_9Glassdoor_12_distribute(CYTHON_UNUSED PyObject *__pyx_self, PyObject *__pyx_v_self, PyObject *__pyx_v_mean_data); /* proto */
-static PyObject *__pyx_pf_6seleya_3mfc_7alchemy_5qrank_8glassdoo_9Glassdoor_14_percentile(CYTHON_UNUSED PyObject *__pyx_self, CYTHON_UNUSED PyObject *__pyx_v_self, PyObject *__pyx_v_x, PyObject *__pyx_v_res); /* proto */
-static PyObject *__pyx_pf_6seleya_3mfc_7alchemy_5qrank_8glassdoo_9Glassdoor_16_calculate_distribute(CYTHON_UNUSED PyObject *__pyx_self, PyObject *__pyx_v_self, PyObject *__pyx_v_mean_data); /* proto */
-static PyObject *__pyx_pf_6seleya_3mfc_7alchemy_5qrank_8glassdoo_9Glassdoor_18_format_mean(CYTHON_UNUSED PyObject *__pyx_self, PyObject *__pyx_v_self, PyObject *__pyx_v_mean_data); /* proto */
+static PyObject *__pyx_pf_6seleya_3mfc_7alchemy_5qrank_9glassdoor_9Glassdoor_12_distribute(CYTHON_UNUSED PyObject *__pyx_self, PyObject *__pyx_v_self, PyObject *__pyx_v_mean_data); /* proto */
+static PyObject *__pyx_pf_6seleya_3mfc_7alchemy_5qrank_9glassdoor_9Glassdoor_14_percentile(CYTHON_UNUSED PyObject *__pyx_self, CYTHON_UNUSED PyObject *__pyx_v_self, PyObject *__pyx_v_x, PyObject *__pyx_v_res); /* proto */
+static PyObject *__pyx_pf_6seleya_3mfc_7alchemy_5qrank_9glassdoor_9Glassdoor_16_calculate_distribute(CYTHON_UNUSED PyObject *__pyx_self, PyObject *__pyx_v_self, PyObject *__pyx_v_mean_data); /* proto */
+static PyObject *__pyx_pf_6seleya_3mfc_7alchemy_5qrank_9glassdoor_9Glassdoor_18_format_mean(CYTHON_UNUSED PyObject *__pyx_self, PyObject *__pyx_v_self, PyObject *__pyx_v_mean_data); /* proto */
 static PyObject *__pyx_lambda_funcdef_lambda2(PyObject *__pyx_self, PyObject *__pyx_v_x); /* proto */
-static PyObject *__pyx_pf_6seleya_3mfc_7alchemy_5qrank_8glassdoo_9Glassdoor_20calculate_result(CYTHON_UNUSED PyObject *__pyx_self, PyObject *__pyx_v_self, PyObject *__pyx_v_total_data, PyObject *__pyx_v_threshold); /* proto */
-static PyObject *__pyx_pf_6seleya_3mfc_7alchemy_5qrank_8glassdoo_9Glassdoor_22run(CYTHON_UNUSED PyObject *__pyx_self, PyObject *__pyx_v_self, PyObject *__pyx_v_begin_date, PyObject *__pyx_v_end_date, PyObject *__pyx_v_threshold); /* proto */
-static PyObject *__pyx_tp_new_6seleya_3mfc_7alchemy_5qrank_8glassdoo___pyx_scope_struct___fetch_reviews(PyTypeObject *t, PyObject *a, PyObject *k); /*proto*/
-static PyObject *__pyx_tp_new_6seleya_3mfc_7alchemy_5qrank_8glassdoo___pyx_scope_struct_1__distribute(PyTypeObject *t, PyObject *a, PyObject *k); /*proto*/
-static PyObject *__pyx_tp_new_6seleya_3mfc_7alchemy_5qrank_8glassdoo___pyx_scope_struct_2_calculate_result(PyTypeObject *t, PyObject *a, PyObject *k); /*proto*/
+static PyObject *__pyx_pf_6seleya_3mfc_7alchemy_5qrank_9glassdoor_9Glassdoor_20calculate_result(CYTHON_UNUSED PyObject *__pyx_self, PyObject *__pyx_v_self, PyObject *__pyx_v_total_data, PyObject *__pyx_v_threshold); /* proto */
+static PyObject *__pyx_pf_6seleya_3mfc_7alchemy_5qrank_9glassdoor_9Glassdoor_22run(CYTHON_UNUSED PyObject *__pyx_self, PyObject *__pyx_v_self, PyObject *__pyx_v_begin_date, PyObject *__pyx_v_end_date, PyObject *__pyx_v_threshold); /* proto */
+static PyObject *__pyx_tp_new_6seleya_3mfc_7alchemy_5qrank_9glassdoor___pyx_scope_struct___fetch_reviews(PyTypeObject *t, PyObject *a, PyObject *k); /*proto*/
+static PyObject *__pyx_tp_new_6seleya_3mfc_7alchemy_5qrank_9glassdoor___pyx_scope_struct_1__distribute(PyTypeObject *t, PyObject *a, PyObject *k); /*proto*/
+static PyObject *__pyx_tp_new_6seleya_3mfc_7alchemy_5qrank_9glassdoor___pyx_scope_struct_2_calculate_result(PyTypeObject *t, PyObject *a, PyObject *k); /*proto*/
 static PyObject *__pyx_float_0_9;
 static PyObject *__pyx_float_0_25;
 static PyObject *__pyx_int_0;
 static PyObject *__pyx_int_1;
 static PyObject *__pyx_int_neg_1;
 static PyObject *__pyx_tuple__2;
 static PyObject *__pyx_tuple__3;
@@ -1791,27 +1791,27 @@
 static PyObject *__pyx_codeobj__21;
 static PyObject *__pyx_codeobj__23;
 static PyObject *__pyx_codeobj__25;
 static PyObject *__pyx_codeobj__27;
 static PyObject *__pyx_codeobj__30;
 /* Late includes */
 
-/* "seleya/mfc/alchemy/qrank/glassdoor.py":13
+/* "seleya/mfc/alchemy/qrank/glassdoor.pyx":13
  * class Glassdoor(object):
  * 
  *     def __init__(self, industry_code):             # <<<<<<<<<<<<<<
  *         self._industry_code = industry_code
  *         self._mapping_dict = {
  */
 
 /* Python wrapper */
-static PyObject *__pyx_pw_6seleya_3mfc_7alchemy_5qrank_8glassdoo_9Glassdoor_1__init__(PyObject *__pyx_self, PyObject *__pyx_args, PyObject *__pyx_kwds); /*proto*/
-static char __pyx_doc_6seleya_3mfc_7alchemy_5qrank_8glassdoo_9Glassdoor___init__[] = "Glassdoor.__init__(self, industry_code)";
-static PyMethodDef __pyx_mdef_6seleya_3mfc_7alchemy_5qrank_8glassdoo_9Glassdoor_1__init__ = {"__init__", (PyCFunction)(void*)(PyCFunctionWithKeywords)__pyx_pw_6seleya_3mfc_7alchemy_5qrank_8glassdoo_9Glassdoor_1__init__, METH_VARARGS|METH_KEYWORDS, __pyx_doc_6seleya_3mfc_7alchemy_5qrank_8glassdoo_9Glassdoor___init__};
-static PyObject *__pyx_pw_6seleya_3mfc_7alchemy_5qrank_8glassdoo_9Glassdoor_1__init__(PyObject *__pyx_self, PyObject *__pyx_args, PyObject *__pyx_kwds) {
+static PyObject *__pyx_pw_6seleya_3mfc_7alchemy_5qrank_9glassdoor_9Glassdoor_1__init__(PyObject *__pyx_self, PyObject *__pyx_args, PyObject *__pyx_kwds); /*proto*/
+static char __pyx_doc_6seleya_3mfc_7alchemy_5qrank_9glassdoor_9Glassdoor___init__[] = "Glassdoor.__init__(self, industry_code)";
+static PyMethodDef __pyx_mdef_6seleya_3mfc_7alchemy_5qrank_9glassdoor_9Glassdoor_1__init__ = {"__init__", (PyCFunction)(void*)(PyCFunctionWithKeywords)__pyx_pw_6seleya_3mfc_7alchemy_5qrank_9glassdoor_9Glassdoor_1__init__, METH_VARARGS|METH_KEYWORDS, __pyx_doc_6seleya_3mfc_7alchemy_5qrank_9glassdoor_9Glassdoor___init__};
+static PyObject *__pyx_pw_6seleya_3mfc_7alchemy_5qrank_9glassdoor_9Glassdoor_1__init__(PyObject *__pyx_self, PyObject *__pyx_args, PyObject *__pyx_kwds) {
   PyObject *__pyx_v_self = 0;
   PyObject *__pyx_v_industry_code = 0;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   PyObject *__pyx_r = 0;
   __Pyx_RefNannyDeclarations
@@ -1854,46 +1854,46 @@
     __pyx_v_self = values[0];
     __pyx_v_industry_code = values[1];
   }
   goto __pyx_L4_argument_unpacking_done;
   __pyx_L5_argtuple_error:;
   __Pyx_RaiseArgtupleInvalid("__init__", 1, 2, 2, PyTuple_GET_SIZE(__pyx_args)); __PYX_ERR(0, 13, __pyx_L3_error)
   __pyx_L3_error:;
-  __Pyx_AddTraceback("seleya.mfc.alchemy.qrank.glassdoo.Glassdoor.__init__", __pyx_clineno, __pyx_lineno, __pyx_filename);
+  __Pyx_AddTraceback("seleya.mfc.alchemy.qrank.glassdoor.Glassdoor.__init__", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __Pyx_RefNannyFinishContext();
   return NULL;
   __pyx_L4_argument_unpacking_done:;
-  __pyx_r = __pyx_pf_6seleya_3mfc_7alchemy_5qrank_8glassdoo_9Glassdoor___init__(__pyx_self, __pyx_v_self, __pyx_v_industry_code);
+  __pyx_r = __pyx_pf_6seleya_3mfc_7alchemy_5qrank_9glassdoor_9Glassdoor___init__(__pyx_self, __pyx_v_self, __pyx_v_industry_code);
 
   /* function exit code */
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-static PyObject *__pyx_pf_6seleya_3mfc_7alchemy_5qrank_8glassdoo_9Glassdoor___init__(CYTHON_UNUSED PyObject *__pyx_self, PyObject *__pyx_v_self, PyObject *__pyx_v_industry_code) {
+static PyObject *__pyx_pf_6seleya_3mfc_7alchemy_5qrank_9glassdoor_9Glassdoor___init__(CYTHON_UNUSED PyObject *__pyx_self, PyObject *__pyx_v_self, PyObject *__pyx_v_industry_code) {
   PyObject *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   PyObject *__pyx_t_2 = NULL;
   PyObject *__pyx_t_3 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("__init__", 0);
 
-  /* "seleya/mfc/alchemy/qrank/glassdoor.py":14
+  /* "seleya/mfc/alchemy/qrank/glassdoor.pyx":14
  * 
  *     def __init__(self, industry_code):
  *         self._industry_code = industry_code             # <<<<<<<<<<<<<<
  *         self._mapping_dict = {
  *             'NO_OPINION': 0,
  */
   if (__Pyx_PyObject_SetAttrStr(__pyx_v_self, __pyx_n_s_industry_code_2, __pyx_v_industry_code) < 0) __PYX_ERR(0, 14, __pyx_L1_error)
 
-  /* "seleya/mfc/alchemy/qrank/glassdoor.py":16
+  /* "seleya/mfc/alchemy/qrank/glassdoor.pyx":16
  *         self._industry_code = industry_code
  *         self._mapping_dict = {
  *             'NO_OPINION': 0,             # <<<<<<<<<<<<<<
  *             'NEGATIVE': -1,
  *             'POSITIVE': 1,
  */
   __pyx_t_1 = __Pyx_PyDict_NewPresized(6); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 16, __pyx_L1_error)
@@ -1901,25 +1901,25 @@
   if (PyDict_SetItem(__pyx_t_1, __pyx_n_s_NO_OPINION, __pyx_int_0) < 0) __PYX_ERR(0, 16, __pyx_L1_error)
   if (PyDict_SetItem(__pyx_t_1, __pyx_n_s_NEGATIVE, __pyx_int_neg_1) < 0) __PYX_ERR(0, 16, __pyx_L1_error)
   if (PyDict_SetItem(__pyx_t_1, __pyx_n_s_POSITIVE, __pyx_int_1) < 0) __PYX_ERR(0, 16, __pyx_L1_error)
   if (PyDict_SetItem(__pyx_t_1, __pyx_n_s_NEUTRAL, __pyx_int_0) < 0) __PYX_ERR(0, 16, __pyx_L1_error)
   if (PyDict_SetItem(__pyx_t_1, __pyx_n_s_APPROVE, __pyx_int_1) < 0) __PYX_ERR(0, 16, __pyx_L1_error)
   if (PyDict_SetItem(__pyx_t_1, __pyx_n_s_DISAPPROVE, __pyx_int_neg_1) < 0) __PYX_ERR(0, 16, __pyx_L1_error)
 
-  /* "seleya/mfc/alchemy/qrank/glassdoor.py":15
+  /* "seleya/mfc/alchemy/qrank/glassdoor.pyx":15
  *     def __init__(self, industry_code):
  *         self._industry_code = industry_code
  *         self._mapping_dict = {             # <<<<<<<<<<<<<<
  *             'NO_OPINION': 0,
  *             'NEGATIVE': -1,
  */
   if (__Pyx_PyObject_SetAttrStr(__pyx_v_self, __pyx_n_s_mapping_dict, __pyx_t_1) < 0) __PYX_ERR(0, 15, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
 
-  /* "seleya/mfc/alchemy/qrank/glassdoor.py":23
+  /* "seleya/mfc/alchemy/qrank/glassdoor.pyx":23
  *             'DISAPPROVE': -1
  *         }
  *         self._probability_cols = [             # <<<<<<<<<<<<<<
  *             'ratingBusinessOutlook', 'ratingRecommendToFriend', 'ratingCeo'
  *         ]
  */
   __pyx_t_1 = PyList_New(3); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 23, __pyx_L1_error)
@@ -1932,15 +1932,15 @@
   PyList_SET_ITEM(__pyx_t_1, 1, __pyx_n_s_ratingRecommendToFriend);
   __Pyx_INCREF(__pyx_n_s_ratingCeo);
   __Pyx_GIVEREF(__pyx_n_s_ratingCeo);
   PyList_SET_ITEM(__pyx_t_1, 2, __pyx_n_s_ratingCeo);
   if (__Pyx_PyObject_SetAttrStr(__pyx_v_self, __pyx_n_s_probability_cols, __pyx_t_1) < 0) __PYX_ERR(0, 23, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
 
-  /* "seleya/mfc/alchemy/qrank/glassdoor.py":26
+  /* "seleya/mfc/alchemy/qrank/glassdoor.pyx":26
  *             'ratingBusinessOutlook', 'ratingRecommendToFriend', 'ratingCeo'
  *         ]
  *         self._mean_cols = [             # <<<<<<<<<<<<<<
  *             'ratingWorkLifeBalance', 'ratingCultureAndValues',
  *             'ratingSeniorLeadership', 'ratingCareerOpportunities',
  */
   __pyx_t_1 = PyList_New(7); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 26, __pyx_L1_error)
@@ -1965,15 +1965,15 @@
   PyList_SET_ITEM(__pyx_t_1, 5, __pyx_n_s_ratingCompensationAndBenefits);
   __Pyx_INCREF(__pyx_n_s_ratingDiversityAndInclusion);
   __Pyx_GIVEREF(__pyx_n_s_ratingDiversityAndInclusion);
   PyList_SET_ITEM(__pyx_t_1, 6, __pyx_n_s_ratingDiversityAndInclusion);
   if (__Pyx_PyObject_SetAttrStr(__pyx_v_self, __pyx_n_s_mean_cols, __pyx_t_1) < 0) __PYX_ERR(0, 26, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
 
-  /* "seleya/mfc/alchemy/qrank/glassdoor.py":32
+  /* "seleya/mfc/alchemy/qrank/glassdoor.pyx":32
  *             'ratingDiversityAndInclusion'
  *         ]
  *         self._factors_sets = self._probability_cols + self._mean_cols             # <<<<<<<<<<<<<<
  * 
  *     def _fetch_overview(self, codes):
  */
   __pyx_t_1 = __Pyx_PyObject_GetAttrStr(__pyx_v_self, __pyx_n_s_probability_cols); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 32, __pyx_L1_error)
@@ -1983,50 +1983,50 @@
   __pyx_t_3 = PyNumber_Add(__pyx_t_1, __pyx_t_2); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 32, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
   if (__Pyx_PyObject_SetAttrStr(__pyx_v_self, __pyx_n_s_factors_sets, __pyx_t_3) < 0) __PYX_ERR(0, 32, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
 
-  /* "seleya/mfc/alchemy/qrank/glassdoor.py":13
+  /* "seleya/mfc/alchemy/qrank/glassdoor.pyx":13
  * class Glassdoor(object):
  * 
  *     def __init__(self, industry_code):             # <<<<<<<<<<<<<<
  *         self._industry_code = industry_code
  *         self._mapping_dict = {
  */
 
   /* function exit code */
   __pyx_r = Py_None; __Pyx_INCREF(Py_None);
   goto __pyx_L0;
   __pyx_L1_error:;
   __Pyx_XDECREF(__pyx_t_1);
   __Pyx_XDECREF(__pyx_t_2);
   __Pyx_XDECREF(__pyx_t_3);
-  __Pyx_AddTraceback("seleya.mfc.alchemy.qrank.glassdoo.Glassdoor.__init__", __pyx_clineno, __pyx_lineno, __pyx_filename);
+  __Pyx_AddTraceback("seleya.mfc.alchemy.qrank.glassdoor.Glassdoor.__init__", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __pyx_r = NULL;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "seleya/mfc/alchemy/qrank/glassdoor.py":34
+/* "seleya/mfc/alchemy/qrank/glassdoor.pyx":34
  *         self._factors_sets = self._probability_cols + self._mean_cols
  * 
  *     def _fetch_overview(self, codes):             # <<<<<<<<<<<<<<
  *         kd_logger.info('Fetching glassdoor overview data...')
  *         gd_overview_data = SurfaceDBAPI.GDOveriew().fetch(
  */
 
 /* Python wrapper */
-static PyObject *__pyx_pw_6seleya_3mfc_7alchemy_5qrank_8glassdoo_9Glassdoor_3_fetch_overview(PyObject *__pyx_self, PyObject *__pyx_args, PyObject *__pyx_kwds); /*proto*/
-static char __pyx_doc_6seleya_3mfc_7alchemy_5qrank_8glassdoo_9Glassdoor_2_fetch_overview[] = "Glassdoor._fetch_overview(self, codes)";
-static PyMethodDef __pyx_mdef_6seleya_3mfc_7alchemy_5qrank_8glassdoo_9Glassdoor_3_fetch_overview = {"_fetch_overview", (PyCFunction)(void*)(PyCFunctionWithKeywords)__pyx_pw_6seleya_3mfc_7alchemy_5qrank_8glassdoo_9Glassdoor_3_fetch_overview, METH_VARARGS|METH_KEYWORDS, __pyx_doc_6seleya_3mfc_7alchemy_5qrank_8glassdoo_9Glassdoor_2_fetch_overview};
-static PyObject *__pyx_pw_6seleya_3mfc_7alchemy_5qrank_8glassdoo_9Glassdoor_3_fetch_overview(PyObject *__pyx_self, PyObject *__pyx_args, PyObject *__pyx_kwds) {
+static PyObject *__pyx_pw_6seleya_3mfc_7alchemy_5qrank_9glassdoor_9Glassdoor_3_fetch_overview(PyObject *__pyx_self, PyObject *__pyx_args, PyObject *__pyx_kwds); /*proto*/
+static char __pyx_doc_6seleya_3mfc_7alchemy_5qrank_9glassdoor_9Glassdoor_2_fetch_overview[] = "Glassdoor._fetch_overview(self, codes)";
+static PyMethodDef __pyx_mdef_6seleya_3mfc_7alchemy_5qrank_9glassdoor_9Glassdoor_3_fetch_overview = {"_fetch_overview", (PyCFunction)(void*)(PyCFunctionWithKeywords)__pyx_pw_6seleya_3mfc_7alchemy_5qrank_9glassdoor_9Glassdoor_3_fetch_overview, METH_VARARGS|METH_KEYWORDS, __pyx_doc_6seleya_3mfc_7alchemy_5qrank_9glassdoor_9Glassdoor_2_fetch_overview};
+static PyObject *__pyx_pw_6seleya_3mfc_7alchemy_5qrank_9glassdoor_9Glassdoor_3_fetch_overview(PyObject *__pyx_self, PyObject *__pyx_args, PyObject *__pyx_kwds) {
   CYTHON_UNUSED PyObject *__pyx_v_self = 0;
   PyObject *__pyx_v_codes = 0;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   PyObject *__pyx_r = 0;
   __Pyx_RefNannyDeclarations
@@ -2069,38 +2069,38 @@
     __pyx_v_self = values[0];
     __pyx_v_codes = values[1];
   }
   goto __pyx_L4_argument_unpacking_done;
   __pyx_L5_argtuple_error:;
   __Pyx_RaiseArgtupleInvalid("_fetch_overview", 1, 2, 2, PyTuple_GET_SIZE(__pyx_args)); __PYX_ERR(0, 34, __pyx_L3_error)
   __pyx_L3_error:;
-  __Pyx_AddTraceback("seleya.mfc.alchemy.qrank.glassdoo.Glassdoor._fetch_overview", __pyx_clineno, __pyx_lineno, __pyx_filename);
+  __Pyx_AddTraceback("seleya.mfc.alchemy.qrank.glassdoor.Glassdoor._fetch_overview", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __Pyx_RefNannyFinishContext();
   return NULL;
   __pyx_L4_argument_unpacking_done:;
-  __pyx_r = __pyx_pf_6seleya_3mfc_7alchemy_5qrank_8glassdoo_9Glassdoor_2_fetch_overview(__pyx_self, __pyx_v_self, __pyx_v_codes);
+  __pyx_r = __pyx_pf_6seleya_3mfc_7alchemy_5qrank_9glassdoor_9Glassdoor_2_fetch_overview(__pyx_self, __pyx_v_self, __pyx_v_codes);
 
   /* function exit code */
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-static PyObject *__pyx_pf_6seleya_3mfc_7alchemy_5qrank_8glassdoo_9Glassdoor_2_fetch_overview(CYTHON_UNUSED PyObject *__pyx_self, CYTHON_UNUSED PyObject *__pyx_v_self, PyObject *__pyx_v_codes) {
+static PyObject *__pyx_pf_6seleya_3mfc_7alchemy_5qrank_9glassdoor_9Glassdoor_2_fetch_overview(CYTHON_UNUSED PyObject *__pyx_self, CYTHON_UNUSED PyObject *__pyx_v_self, PyObject *__pyx_v_codes) {
   PyObject *__pyx_v_gd_overview_data = NULL;
   PyObject *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   PyObject *__pyx_t_2 = NULL;
   PyObject *__pyx_t_3 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("_fetch_overview", 0);
 
-  /* "seleya/mfc/alchemy/qrank/glassdoor.py":35
+  /* "seleya/mfc/alchemy/qrank/glassdoor.pyx":35
  * 
  *     def _fetch_overview(self, codes):
  *         kd_logger.info('Fetching glassdoor overview data...')             # <<<<<<<<<<<<<<
  *         gd_overview_data = SurfaceDBAPI.GDOveriew().fetch(
  *             codes=codes, columns=['code', 'cid'])
  */
   __Pyx_GetModuleGlobalName(__pyx_t_2, __pyx_n_s_kd_logger); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 35, __pyx_L1_error)
@@ -2121,15 +2121,15 @@
   __pyx_t_1 = (__pyx_t_2) ? __Pyx_PyObject_Call2Args(__pyx_t_3, __pyx_t_2, __pyx_kp_s_Fetching_glassdoor_overview_data) : __Pyx_PyObject_CallOneArg(__pyx_t_3, __pyx_kp_s_Fetching_glassdoor_overview_data);
   __Pyx_XDECREF(__pyx_t_2); __pyx_t_2 = 0;
   if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 35, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
 
-  /* "seleya/mfc/alchemy/qrank/glassdoor.py":36
+  /* "seleya/mfc/alchemy/qrank/glassdoor.pyx":36
  *     def _fetch_overview(self, codes):
  *         kd_logger.info('Fetching glassdoor overview data...')
  *         gd_overview_data = SurfaceDBAPI.GDOveriew().fetch(             # <<<<<<<<<<<<<<
  *             codes=codes, columns=['code', 'cid'])
  *         gd_overview_data = gd_overview_data[['cid', 'code'
  */
   __Pyx_GetModuleGlobalName(__pyx_t_3, __pyx_n_s_SurfaceDBAPI); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 36, __pyx_L1_error)
@@ -2152,15 +2152,15 @@
   if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 36, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
   __pyx_t_2 = __Pyx_PyObject_GetAttrStr(__pyx_t_1, __pyx_n_s_fetch); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 36, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
 
-  /* "seleya/mfc/alchemy/qrank/glassdoor.py":37
+  /* "seleya/mfc/alchemy/qrank/glassdoor.pyx":37
  *         kd_logger.info('Fetching glassdoor overview data...')
  *         gd_overview_data = SurfaceDBAPI.GDOveriew().fetch(
  *             codes=codes, columns=['code', 'cid'])             # <<<<<<<<<<<<<<
  *         gd_overview_data = gd_overview_data[['cid', 'code'
  *                                              ]].drop_duplicates(subset=['cid'])
  */
   __pyx_t_1 = __Pyx_PyDict_NewPresized(2); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 37, __pyx_L1_error)
@@ -2173,29 +2173,29 @@
   PyList_SET_ITEM(__pyx_t_3, 0, __pyx_n_s_code);
   __Pyx_INCREF(__pyx_n_s_cid);
   __Pyx_GIVEREF(__pyx_n_s_cid);
   PyList_SET_ITEM(__pyx_t_3, 1, __pyx_n_s_cid);
   if (PyDict_SetItem(__pyx_t_1, __pyx_n_s_columns, __pyx_t_3) < 0) __PYX_ERR(0, 37, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
 
-  /* "seleya/mfc/alchemy/qrank/glassdoor.py":36
+  /* "seleya/mfc/alchemy/qrank/glassdoor.pyx":36
  *     def _fetch_overview(self, codes):
  *         kd_logger.info('Fetching glassdoor overview data...')
  *         gd_overview_data = SurfaceDBAPI.GDOveriew().fetch(             # <<<<<<<<<<<<<<
  *             codes=codes, columns=['code', 'cid'])
  *         gd_overview_data = gd_overview_data[['cid', 'code'
  */
   __pyx_t_3 = __Pyx_PyObject_Call(__pyx_t_2, __pyx_empty_tuple, __pyx_t_1); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 36, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   __pyx_v_gd_overview_data = __pyx_t_3;
   __pyx_t_3 = 0;
 
-  /* "seleya/mfc/alchemy/qrank/glassdoor.py":38
+  /* "seleya/mfc/alchemy/qrank/glassdoor.pyx":38
  *         gd_overview_data = SurfaceDBAPI.GDOveriew().fetch(
  *             codes=codes, columns=['code', 'cid'])
  *         gd_overview_data = gd_overview_data[['cid', 'code'             # <<<<<<<<<<<<<<
  *                                              ]].drop_duplicates(subset=['cid'])
  *         return gd_overview_data
  */
   __pyx_t_3 = PyList_New(2); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 38, __pyx_L1_error)
@@ -2206,15 +2206,15 @@
   __Pyx_INCREF(__pyx_n_s_code);
   __Pyx_GIVEREF(__pyx_n_s_code);
   PyList_SET_ITEM(__pyx_t_3, 1, __pyx_n_s_code);
   __pyx_t_1 = __Pyx_PyObject_GetItem(__pyx_v_gd_overview_data, __pyx_t_3); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 38, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
 
-  /* "seleya/mfc/alchemy/qrank/glassdoor.py":39
+  /* "seleya/mfc/alchemy/qrank/glassdoor.pyx":39
  *             codes=codes, columns=['code', 'cid'])
  *         gd_overview_data = gd_overview_data[['cid', 'code'
  *                                              ]].drop_duplicates(subset=['cid'])             # <<<<<<<<<<<<<<
  *         return gd_overview_data
  * 
  */
   __pyx_t_3 = __Pyx_PyObject_GetAttrStr(__pyx_t_1, __pyx_n_s_drop_duplicates); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 39, __pyx_L1_error)
@@ -2232,61 +2232,61 @@
   __pyx_t_2 = __Pyx_PyObject_Call(__pyx_t_3, __pyx_empty_tuple, __pyx_t_1); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 39, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   __Pyx_DECREF_SET(__pyx_v_gd_overview_data, __pyx_t_2);
   __pyx_t_2 = 0;
 
-  /* "seleya/mfc/alchemy/qrank/glassdoor.py":40
+  /* "seleya/mfc/alchemy/qrank/glassdoor.pyx":40
  *         gd_overview_data = gd_overview_data[['cid', 'code'
  *                                              ]].drop_duplicates(subset=['cid'])
  *         return gd_overview_data             # <<<<<<<<<<<<<<
  * 
  *     def _fetch_reviews(self, begin_date, end_date, cids):
  */
   __Pyx_XDECREF(__pyx_r);
   __Pyx_INCREF(__pyx_v_gd_overview_data);
   __pyx_r = __pyx_v_gd_overview_data;
   goto __pyx_L0;
 
-  /* "seleya/mfc/alchemy/qrank/glassdoor.py":34
+  /* "seleya/mfc/alchemy/qrank/glassdoor.pyx":34
  *         self._factors_sets = self._probability_cols + self._mean_cols
  * 
  *     def _fetch_overview(self, codes):             # <<<<<<<<<<<<<<
  *         kd_logger.info('Fetching glassdoor overview data...')
  *         gd_overview_data = SurfaceDBAPI.GDOveriew().fetch(
  */
 
   /* function exit code */
   __pyx_L1_error:;
   __Pyx_XDECREF(__pyx_t_1);
   __Pyx_XDECREF(__pyx_t_2);
   __Pyx_XDECREF(__pyx_t_3);
-  __Pyx_AddTraceback("seleya.mfc.alchemy.qrank.glassdoo.Glassdoor._fetch_overview", __pyx_clineno, __pyx_lineno, __pyx_filename);
+  __Pyx_AddTraceback("seleya.mfc.alchemy.qrank.glassdoor.Glassdoor._fetch_overview", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __pyx_r = NULL;
   __pyx_L0:;
   __Pyx_XDECREF(__pyx_v_gd_overview_data);
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "seleya/mfc/alchemy/qrank/glassdoor.py":42
+/* "seleya/mfc/alchemy/qrank/glassdoor.pyx":42
  *         return gd_overview_data
  * 
  *     def _fetch_reviews(self, begin_date, end_date, cids):             # <<<<<<<<<<<<<<
  *         kd_logger.info('Fetching glassdoor reviews data...')
  *         columns = ['id', 'cid', 'reviewId', 'reviewDateTime'
  */
 
 /* Python wrapper */
-static PyObject *__pyx_pw_6seleya_3mfc_7alchemy_5qrank_8glassdoo_9Glassdoor_5_fetch_reviews(PyObject *__pyx_self, PyObject *__pyx_args, PyObject *__pyx_kwds); /*proto*/
-static char __pyx_doc_6seleya_3mfc_7alchemy_5qrank_8glassdoo_9Glassdoor_4_fetch_reviews[] = "Glassdoor._fetch_reviews(self, begin_date, end_date, cids)";
-static PyMethodDef __pyx_mdef_6seleya_3mfc_7alchemy_5qrank_8glassdoo_9Glassdoor_5_fetch_reviews = {"_fetch_reviews", (PyCFunction)(void*)(PyCFunctionWithKeywords)__pyx_pw_6seleya_3mfc_7alchemy_5qrank_8glassdoo_9Glassdoor_5_fetch_reviews, METH_VARARGS|METH_KEYWORDS, __pyx_doc_6seleya_3mfc_7alchemy_5qrank_8glassdoo_9Glassdoor_4_fetch_reviews};
-static PyObject *__pyx_pw_6seleya_3mfc_7alchemy_5qrank_8glassdoo_9Glassdoor_5_fetch_reviews(PyObject *__pyx_self, PyObject *__pyx_args, PyObject *__pyx_kwds) {
+static PyObject *__pyx_pw_6seleya_3mfc_7alchemy_5qrank_9glassdoor_9Glassdoor_5_fetch_reviews(PyObject *__pyx_self, PyObject *__pyx_args, PyObject *__pyx_kwds); /*proto*/
+static char __pyx_doc_6seleya_3mfc_7alchemy_5qrank_9glassdoor_9Glassdoor_4_fetch_reviews[] = "Glassdoor._fetch_reviews(self, begin_date, end_date, cids)";
+static PyMethodDef __pyx_mdef_6seleya_3mfc_7alchemy_5qrank_9glassdoor_9Glassdoor_5_fetch_reviews = {"_fetch_reviews", (PyCFunction)(void*)(PyCFunctionWithKeywords)__pyx_pw_6seleya_3mfc_7alchemy_5qrank_9glassdoor_9Glassdoor_5_fetch_reviews, METH_VARARGS|METH_KEYWORDS, __pyx_doc_6seleya_3mfc_7alchemy_5qrank_9glassdoor_9Glassdoor_4_fetch_reviews};
+static PyObject *__pyx_pw_6seleya_3mfc_7alchemy_5qrank_9glassdoor_9Glassdoor_5_fetch_reviews(PyObject *__pyx_self, PyObject *__pyx_args, PyObject *__pyx_kwds) {
   PyObject *__pyx_v_self = 0;
   PyObject *__pyx_v_begin_date = 0;
   PyObject *__pyx_v_end_date = 0;
   PyObject *__pyx_v_cids = 0;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
@@ -2351,61 +2351,61 @@
     __pyx_v_end_date = values[2];
     __pyx_v_cids = values[3];
   }
   goto __pyx_L4_argument_unpacking_done;
   __pyx_L5_argtuple_error:;
   __Pyx_RaiseArgtupleInvalid("_fetch_reviews", 1, 4, 4, PyTuple_GET_SIZE(__pyx_args)); __PYX_ERR(0, 42, __pyx_L3_error)
   __pyx_L3_error:;
-  __Pyx_AddTraceback("seleya.mfc.alchemy.qrank.glassdoo.Glassdoor._fetch_reviews", __pyx_clineno, __pyx_lineno, __pyx_filename);
+  __Pyx_AddTraceback("seleya.mfc.alchemy.qrank.glassdoor.Glassdoor._fetch_reviews", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __Pyx_RefNannyFinishContext();
   return NULL;
   __pyx_L4_argument_unpacking_done:;
-  __pyx_r = __pyx_pf_6seleya_3mfc_7alchemy_5qrank_8glassdoo_9Glassdoor_4_fetch_reviews(__pyx_self, __pyx_v_self, __pyx_v_begin_date, __pyx_v_end_date, __pyx_v_cids);
+  __pyx_r = __pyx_pf_6seleya_3mfc_7alchemy_5qrank_9glassdoor_9Glassdoor_4_fetch_reviews(__pyx_self, __pyx_v_self, __pyx_v_begin_date, __pyx_v_end_date, __pyx_v_cids);
 
   /* function exit code */
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "seleya/mfc/alchemy/qrank/glassdoor.py":56
+/* "seleya/mfc/alchemy/qrank/glassdoor.pyx":56
  *         for col in self._probability_cols:
  *             gd_reviews_data[col] = gd_reviews_data[col].apply(
  *                 lambda x: np.nan if x is None else self._mapping_dict[x])             # <<<<<<<<<<<<<<
  *         gd_reviews_data['reviewDateTime'] = pd.to_datetime(
  *             gd_reviews_data['reviewDateTime'])
  */
 
 /* Python wrapper */
-static PyObject *__pyx_pw_6seleya_3mfc_7alchemy_5qrank_8glassdoo_9Glassdoor_14_fetch_reviews_lambda(PyObject *__pyx_self, PyObject *__pyx_v_x); /*proto*/
-static PyMethodDef __pyx_mdef_6seleya_3mfc_7alchemy_5qrank_8glassdoo_9Glassdoor_14_fetch_reviews_lambda = {"lambda", (PyCFunction)__pyx_pw_6seleya_3mfc_7alchemy_5qrank_8glassdoo_9Glassdoor_14_fetch_reviews_lambda, METH_O, 0};
-static PyObject *__pyx_pw_6seleya_3mfc_7alchemy_5qrank_8glassdoo_9Glassdoor_14_fetch_reviews_lambda(PyObject *__pyx_self, PyObject *__pyx_v_x) {
+static PyObject *__pyx_pw_6seleya_3mfc_7alchemy_5qrank_9glassdoor_9Glassdoor_14_fetch_reviews_lambda(PyObject *__pyx_self, PyObject *__pyx_v_x); /*proto*/
+static PyMethodDef __pyx_mdef_6seleya_3mfc_7alchemy_5qrank_9glassdoor_9Glassdoor_14_fetch_reviews_lambda = {"lambda", (PyCFunction)__pyx_pw_6seleya_3mfc_7alchemy_5qrank_9glassdoor_9Glassdoor_14_fetch_reviews_lambda, METH_O, 0};
+static PyObject *__pyx_pw_6seleya_3mfc_7alchemy_5qrank_9glassdoor_9Glassdoor_14_fetch_reviews_lambda(PyObject *__pyx_self, PyObject *__pyx_v_x) {
   PyObject *__pyx_r = 0;
   __Pyx_RefNannyDeclarations
   __Pyx_RefNannySetupContext("lambda (wrapper)", 0);
   __pyx_r = __pyx_lambda_funcdef_lambda(__pyx_self, ((PyObject *)__pyx_v_x));
 
   /* function exit code */
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
 static PyObject *__pyx_lambda_funcdef_lambda(PyObject *__pyx_self, PyObject *__pyx_v_x) {
-  struct __pyx_obj_6seleya_3mfc_7alchemy_5qrank_8glassdoo___pyx_scope_struct___fetch_reviews *__pyx_cur_scope;
-  struct __pyx_obj_6seleya_3mfc_7alchemy_5qrank_8glassdoo___pyx_scope_struct___fetch_reviews *__pyx_outer_scope;
+  struct __pyx_obj_6seleya_3mfc_7alchemy_5qrank_9glassdoor___pyx_scope_struct___fetch_reviews *__pyx_cur_scope;
+  struct __pyx_obj_6seleya_3mfc_7alchemy_5qrank_9glassdoor___pyx_scope_struct___fetch_reviews *__pyx_outer_scope;
   PyObject *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_t_2;
   PyObject *__pyx_t_3 = NULL;
   PyObject *__pyx_t_4 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("lambda", 0);
-  __pyx_outer_scope = (struct __pyx_obj_6seleya_3mfc_7alchemy_5qrank_8glassdoo___pyx_scope_struct___fetch_reviews *) __Pyx_CyFunction_GetClosure(__pyx_self);
+  __pyx_outer_scope = (struct __pyx_obj_6seleya_3mfc_7alchemy_5qrank_9glassdoor___pyx_scope_struct___fetch_reviews *) __Pyx_CyFunction_GetClosure(__pyx_self);
   __pyx_cur_scope = __pyx_outer_scope;
   __Pyx_XDECREF(__pyx_r);
   __pyx_t_2 = (__pyx_v_x == Py_None);
   if ((__pyx_t_2 != 0)) {
     __Pyx_GetModuleGlobalName(__pyx_t_3, __pyx_n_s_np); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 56, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_3);
     __pyx_t_4 = __Pyx_PyObject_GetAttrStr(__pyx_t_3, __pyx_n_s_nan); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 56, __pyx_L1_error)
@@ -2428,32 +2428,32 @@
   goto __pyx_L0;
 
   /* function exit code */
   __pyx_L1_error:;
   __Pyx_XDECREF(__pyx_t_1);
   __Pyx_XDECREF(__pyx_t_3);
   __Pyx_XDECREF(__pyx_t_4);
-  __Pyx_AddTraceback("seleya.mfc.alchemy.qrank.glassdoo.Glassdoor._fetch_reviews.lambda", __pyx_clineno, __pyx_lineno, __pyx_filename);
+  __Pyx_AddTraceback("seleya.mfc.alchemy.qrank.glassdoor.Glassdoor._fetch_reviews.lambda", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __pyx_r = NULL;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "seleya/mfc/alchemy/qrank/glassdoor.py":42
+/* "seleya/mfc/alchemy/qrank/glassdoor.pyx":42
  *         return gd_overview_data
  * 
  *     def _fetch_reviews(self, begin_date, end_date, cids):             # <<<<<<<<<<<<<<
  *         kd_logger.info('Fetching glassdoor reviews data...')
  *         columns = ['id', 'cid', 'reviewId', 'reviewDateTime'
  */
 
-static PyObject *__pyx_pf_6seleya_3mfc_7alchemy_5qrank_8glassdoo_9Glassdoor_4_fetch_reviews(CYTHON_UNUSED PyObject *__pyx_self, PyObject *__pyx_v_self, PyObject *__pyx_v_begin_date, PyObject *__pyx_v_end_date, PyObject *__pyx_v_cids) {
-  struct __pyx_obj_6seleya_3mfc_7alchemy_5qrank_8glassdoo___pyx_scope_struct___fetch_reviews *__pyx_cur_scope;
+static PyObject *__pyx_pf_6seleya_3mfc_7alchemy_5qrank_9glassdoor_9Glassdoor_4_fetch_reviews(CYTHON_UNUSED PyObject *__pyx_self, PyObject *__pyx_v_self, PyObject *__pyx_v_begin_date, PyObject *__pyx_v_end_date, PyObject *__pyx_v_cids) {
+  struct __pyx_obj_6seleya_3mfc_7alchemy_5qrank_9glassdoor___pyx_scope_struct___fetch_reviews *__pyx_cur_scope;
   PyObject *__pyx_v_columns = NULL;
   PyObject *__pyx_v_gd_reviews_data = NULL;
   PyObject *__pyx_v_col = NULL;
   PyObject *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   PyObject *__pyx_t_2 = NULL;
@@ -2463,27 +2463,27 @@
   PyObject *(*__pyx_t_6)(PyObject *);
   PyObject *__pyx_t_7 = NULL;
   PyObject *__pyx_t_8 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("_fetch_reviews", 0);
-  __pyx_cur_scope = (struct __pyx_obj_6seleya_3mfc_7alchemy_5qrank_8glassdoo___pyx_scope_struct___fetch_reviews *)__pyx_tp_new_6seleya_3mfc_7alchemy_5qrank_8glassdoo___pyx_scope_struct___fetch_reviews(__pyx_ptype_6seleya_3mfc_7alchemy_5qrank_8glassdoo___pyx_scope_struct___fetch_reviews, __pyx_empty_tuple, NULL);
+  __pyx_cur_scope = (struct __pyx_obj_6seleya_3mfc_7alchemy_5qrank_9glassdoor___pyx_scope_struct___fetch_reviews *)__pyx_tp_new_6seleya_3mfc_7alchemy_5qrank_9glassdoor___pyx_scope_struct___fetch_reviews(__pyx_ptype_6seleya_3mfc_7alchemy_5qrank_9glassdoor___pyx_scope_struct___fetch_reviews, __pyx_empty_tuple, NULL);
   if (unlikely(!__pyx_cur_scope)) {
-    __pyx_cur_scope = ((struct __pyx_obj_6seleya_3mfc_7alchemy_5qrank_8glassdoo___pyx_scope_struct___fetch_reviews *)Py_None);
+    __pyx_cur_scope = ((struct __pyx_obj_6seleya_3mfc_7alchemy_5qrank_9glassdoor___pyx_scope_struct___fetch_reviews *)Py_None);
     __Pyx_INCREF(Py_None);
     __PYX_ERR(0, 42, __pyx_L1_error)
   } else {
     __Pyx_GOTREF(__pyx_cur_scope);
   }
   __pyx_cur_scope->__pyx_v_self = __pyx_v_self;
   __Pyx_INCREF(__pyx_cur_scope->__pyx_v_self);
   __Pyx_GIVEREF(__pyx_cur_scope->__pyx_v_self);
 
-  /* "seleya/mfc/alchemy/qrank/glassdoor.py":43
+  /* "seleya/mfc/alchemy/qrank/glassdoor.pyx":43
  * 
  *     def _fetch_reviews(self, begin_date, end_date, cids):
  *         kd_logger.info('Fetching glassdoor reviews data...')             # <<<<<<<<<<<<<<
  *         columns = ['id', 'cid', 'reviewId', 'reviewDateTime'
  *                    ] + self._factors_sets
  */
   __Pyx_GetModuleGlobalName(__pyx_t_2, __pyx_n_s_kd_logger); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 43, __pyx_L1_error)
@@ -2504,15 +2504,15 @@
   __pyx_t_1 = (__pyx_t_2) ? __Pyx_PyObject_Call2Args(__pyx_t_3, __pyx_t_2, __pyx_kp_s_Fetching_glassdoor_reviews_data) : __Pyx_PyObject_CallOneArg(__pyx_t_3, __pyx_kp_s_Fetching_glassdoor_reviews_data);
   __Pyx_XDECREF(__pyx_t_2); __pyx_t_2 = 0;
   if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 43, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
 
-  /* "seleya/mfc/alchemy/qrank/glassdoor.py":44
+  /* "seleya/mfc/alchemy/qrank/glassdoor.pyx":44
  *     def _fetch_reviews(self, begin_date, end_date, cids):
  *         kd_logger.info('Fetching glassdoor reviews data...')
  *         columns = ['id', 'cid', 'reviewId', 'reviewDateTime'             # <<<<<<<<<<<<<<
  *                    ] + self._factors_sets
  *         gd_reviews_data = SurfaceDBAPI.GDReviewsBase().fetch(
  */
   __pyx_t_1 = PyList_New(4); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 44, __pyx_L1_error)
@@ -2526,15 +2526,15 @@
   __Pyx_INCREF(__pyx_n_s_reviewId);
   __Pyx_GIVEREF(__pyx_n_s_reviewId);
   PyList_SET_ITEM(__pyx_t_1, 2, __pyx_n_s_reviewId);
   __Pyx_INCREF(__pyx_n_s_reviewDateTime);
   __Pyx_GIVEREF(__pyx_n_s_reviewDateTime);
   PyList_SET_ITEM(__pyx_t_1, 3, __pyx_n_s_reviewDateTime);
 
-  /* "seleya/mfc/alchemy/qrank/glassdoor.py":45
+  /* "seleya/mfc/alchemy/qrank/glassdoor.pyx":45
  *         kd_logger.info('Fetching glassdoor reviews data...')
  *         columns = ['id', 'cid', 'reviewId', 'reviewDateTime'
  *                    ] + self._factors_sets             # <<<<<<<<<<<<<<
  *         gd_reviews_data = SurfaceDBAPI.GDReviewsBase().fetch(
  *             begin_date=begin_date,
  */
   __pyx_t_3 = __Pyx_PyObject_GetAttrStr(__pyx_cur_scope->__pyx_v_self, __pyx_n_s_factors_sets); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 45, __pyx_L1_error)
@@ -2542,15 +2542,15 @@
   __pyx_t_2 = PyNumber_Add(__pyx_t_1, __pyx_t_3); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 45, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
   __pyx_v_columns = __pyx_t_2;
   __pyx_t_2 = 0;
 
-  /* "seleya/mfc/alchemy/qrank/glassdoor.py":46
+  /* "seleya/mfc/alchemy/qrank/glassdoor.pyx":46
  *         columns = ['id', 'cid', 'reviewId', 'reviewDateTime'
  *                    ] + self._factors_sets
  *         gd_reviews_data = SurfaceDBAPI.GDReviewsBase().fetch(             # <<<<<<<<<<<<<<
  *             begin_date=begin_date,
  *             end_date=end_date,
  */
   __Pyx_GetModuleGlobalName(__pyx_t_3, __pyx_n_s_SurfaceDBAPI); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 46, __pyx_L1_error)
@@ -2573,100 +2573,100 @@
   if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 46, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   __pyx_t_1 = __Pyx_PyObject_GetAttrStr(__pyx_t_2, __pyx_n_s_fetch); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 46, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
 
-  /* "seleya/mfc/alchemy/qrank/glassdoor.py":47
+  /* "seleya/mfc/alchemy/qrank/glassdoor.pyx":47
  *                    ] + self._factors_sets
  *         gd_reviews_data = SurfaceDBAPI.GDReviewsBase().fetch(
  *             begin_date=begin_date,             # <<<<<<<<<<<<<<
  *             end_date=end_date,
  *             cids=cids,
  */
   __pyx_t_2 = __Pyx_PyDict_NewPresized(4); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 47, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   if (PyDict_SetItem(__pyx_t_2, __pyx_n_s_begin_date, __pyx_v_begin_date) < 0) __PYX_ERR(0, 47, __pyx_L1_error)
 
-  /* "seleya/mfc/alchemy/qrank/glassdoor.py":48
+  /* "seleya/mfc/alchemy/qrank/glassdoor.pyx":48
  *         gd_reviews_data = SurfaceDBAPI.GDReviewsBase().fetch(
  *             begin_date=begin_date,
  *             end_date=end_date,             # <<<<<<<<<<<<<<
  *             cids=cids,
  *             columns=columns)
  */
   if (PyDict_SetItem(__pyx_t_2, __pyx_n_s_end_date, __pyx_v_end_date) < 0) __PYX_ERR(0, 47, __pyx_L1_error)
 
-  /* "seleya/mfc/alchemy/qrank/glassdoor.py":49
+  /* "seleya/mfc/alchemy/qrank/glassdoor.pyx":49
  *             begin_date=begin_date,
  *             end_date=end_date,
  *             cids=cids,             # <<<<<<<<<<<<<<
  *             columns=columns)
  *         if gd_reviews_data.empty:
  */
   if (PyDict_SetItem(__pyx_t_2, __pyx_n_s_cids, __pyx_v_cids) < 0) __PYX_ERR(0, 47, __pyx_L1_error)
 
-  /* "seleya/mfc/alchemy/qrank/glassdoor.py":50
+  /* "seleya/mfc/alchemy/qrank/glassdoor.pyx":50
  *             end_date=end_date,
  *             cids=cids,
  *             columns=columns)             # <<<<<<<<<<<<<<
  *         if gd_reviews_data.empty:
  *             return None
  */
   if (PyDict_SetItem(__pyx_t_2, __pyx_n_s_columns, __pyx_v_columns) < 0) __PYX_ERR(0, 47, __pyx_L1_error)
 
-  /* "seleya/mfc/alchemy/qrank/glassdoor.py":46
+  /* "seleya/mfc/alchemy/qrank/glassdoor.pyx":46
  *         columns = ['id', 'cid', 'reviewId', 'reviewDateTime'
  *                    ] + self._factors_sets
  *         gd_reviews_data = SurfaceDBAPI.GDReviewsBase().fetch(             # <<<<<<<<<<<<<<
  *             begin_date=begin_date,
  *             end_date=end_date,
  */
   __pyx_t_3 = __Pyx_PyObject_Call(__pyx_t_1, __pyx_empty_tuple, __pyx_t_2); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 46, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
   __pyx_v_gd_reviews_data = __pyx_t_3;
   __pyx_t_3 = 0;
 
-  /* "seleya/mfc/alchemy/qrank/glassdoor.py":51
+  /* "seleya/mfc/alchemy/qrank/glassdoor.pyx":51
  *             cids=cids,
  *             columns=columns)
  *         if gd_reviews_data.empty:             # <<<<<<<<<<<<<<
  *             return None
  * 
  */
   __pyx_t_3 = __Pyx_PyObject_GetAttrStr(__pyx_v_gd_reviews_data, __pyx_n_s_empty); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 51, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
   __pyx_t_4 = __Pyx_PyObject_IsTrue(__pyx_t_3); if (unlikely(__pyx_t_4 < 0)) __PYX_ERR(0, 51, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
   if (__pyx_t_4) {
 
-    /* "seleya/mfc/alchemy/qrank/glassdoor.py":52
+    /* "seleya/mfc/alchemy/qrank/glassdoor.pyx":52
  *             columns=columns)
  *         if gd_reviews_data.empty:
  *             return None             # <<<<<<<<<<<<<<
  * 
  *         for col in self._probability_cols:
  */
     __Pyx_XDECREF(__pyx_r);
     __pyx_r = Py_None; __Pyx_INCREF(Py_None);
     goto __pyx_L0;
 
-    /* "seleya/mfc/alchemy/qrank/glassdoor.py":51
+    /* "seleya/mfc/alchemy/qrank/glassdoor.pyx":51
  *             cids=cids,
  *             columns=columns)
  *         if gd_reviews_data.empty:             # <<<<<<<<<<<<<<
  *             return None
  * 
  */
   }
 
-  /* "seleya/mfc/alchemy/qrank/glassdoor.py":54
+  /* "seleya/mfc/alchemy/qrank/glassdoor.pyx":54
  *             return None
  * 
  *         for col in self._probability_cols:             # <<<<<<<<<<<<<<
  *             gd_reviews_data[col] = gd_reviews_data[col].apply(
  *                 lambda x: np.nan if x is None else self._mapping_dict[x])
  */
   __pyx_t_3 = __Pyx_PyObject_GetAttrStr(__pyx_cur_scope->__pyx_v_self, __pyx_n_s_probability_cols); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 54, __pyx_L1_error)
@@ -2710,35 +2710,35 @@
         break;
       }
       __Pyx_GOTREF(__pyx_t_3);
     }
     __Pyx_XDECREF_SET(__pyx_v_col, __pyx_t_3);
     __pyx_t_3 = 0;
 
-    /* "seleya/mfc/alchemy/qrank/glassdoor.py":55
+    /* "seleya/mfc/alchemy/qrank/glassdoor.pyx":55
  * 
  *         for col in self._probability_cols:
  *             gd_reviews_data[col] = gd_reviews_data[col].apply(             # <<<<<<<<<<<<<<
  *                 lambda x: np.nan if x is None else self._mapping_dict[x])
  *         gd_reviews_data['reviewDateTime'] = pd.to_datetime(
  */
     __pyx_t_1 = __Pyx_PyObject_GetItem(__pyx_v_gd_reviews_data, __pyx_v_col); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 55, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_1);
     __pyx_t_7 = __Pyx_PyObject_GetAttrStr(__pyx_t_1, __pyx_n_s_apply); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 55, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_7);
     __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
 
-    /* "seleya/mfc/alchemy/qrank/glassdoor.py":56
+    /* "seleya/mfc/alchemy/qrank/glassdoor.pyx":56
  *         for col in self._probability_cols:
  *             gd_reviews_data[col] = gd_reviews_data[col].apply(
  *                 lambda x: np.nan if x is None else self._mapping_dict[x])             # <<<<<<<<<<<<<<
  *         gd_reviews_data['reviewDateTime'] = pd.to_datetime(
  *             gd_reviews_data['reviewDateTime'])
  */
-    __pyx_t_1 = __Pyx_CyFunction_New(&__pyx_mdef_6seleya_3mfc_7alchemy_5qrank_8glassdoo_9Glassdoor_14_fetch_reviews_lambda, 0, __pyx_n_s_Glassdoor__fetch_reviews_locals, ((PyObject*)__pyx_cur_scope), __pyx_n_s_seleya_mfc_alchemy_qrank_glassdo, __pyx_d, NULL); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 56, __pyx_L1_error)
+    __pyx_t_1 = __Pyx_CyFunction_New(&__pyx_mdef_6seleya_3mfc_7alchemy_5qrank_9glassdoor_9Glassdoor_14_fetch_reviews_lambda, 0, __pyx_n_s_Glassdoor__fetch_reviews_locals, ((PyObject*)__pyx_cur_scope), __pyx_n_s_seleya_mfc_alchemy_qrank_glassdo, __pyx_d, NULL); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 56, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_1);
     __pyx_t_8 = NULL;
     if (CYTHON_UNPACK_METHODS && likely(PyMethod_Check(__pyx_t_7))) {
       __pyx_t_8 = PyMethod_GET_SELF(__pyx_t_7);
       if (likely(__pyx_t_8)) {
         PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_7);
         __Pyx_INCREF(__pyx_t_8);
@@ -2749,48 +2749,48 @@
     __pyx_t_3 = (__pyx_t_8) ? __Pyx_PyObject_Call2Args(__pyx_t_7, __pyx_t_8, __pyx_t_1) : __Pyx_PyObject_CallOneArg(__pyx_t_7, __pyx_t_1);
     __Pyx_XDECREF(__pyx_t_8); __pyx_t_8 = 0;
     __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
     if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 55, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_3);
     __Pyx_DECREF(__pyx_t_7); __pyx_t_7 = 0;
 
-    /* "seleya/mfc/alchemy/qrank/glassdoor.py":55
+    /* "seleya/mfc/alchemy/qrank/glassdoor.pyx":55
  * 
  *         for col in self._probability_cols:
  *             gd_reviews_data[col] = gd_reviews_data[col].apply(             # <<<<<<<<<<<<<<
  *                 lambda x: np.nan if x is None else self._mapping_dict[x])
  *         gd_reviews_data['reviewDateTime'] = pd.to_datetime(
  */
     if (unlikely(PyObject_SetItem(__pyx_v_gd_reviews_data, __pyx_v_col, __pyx_t_3) < 0)) __PYX_ERR(0, 55, __pyx_L1_error)
     __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
 
-    /* "seleya/mfc/alchemy/qrank/glassdoor.py":54
+    /* "seleya/mfc/alchemy/qrank/glassdoor.pyx":54
  *             return None
  * 
  *         for col in self._probability_cols:             # <<<<<<<<<<<<<<
  *             gd_reviews_data[col] = gd_reviews_data[col].apply(
  *                 lambda x: np.nan if x is None else self._mapping_dict[x])
  */
   }
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
 
-  /* "seleya/mfc/alchemy/qrank/glassdoor.py":57
+  /* "seleya/mfc/alchemy/qrank/glassdoor.pyx":57
  *             gd_reviews_data[col] = gd_reviews_data[col].apply(
  *                 lambda x: np.nan if x is None else self._mapping_dict[x])
  *         gd_reviews_data['reviewDateTime'] = pd.to_datetime(             # <<<<<<<<<<<<<<
  *             gd_reviews_data['reviewDateTime'])
  *         gd_reviews_data['date'] = pd.to_datetime(
  */
   __Pyx_GetModuleGlobalName(__pyx_t_3, __pyx_n_s_pd); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 57, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
   __pyx_t_7 = __Pyx_PyObject_GetAttrStr(__pyx_t_3, __pyx_n_s_to_datetime); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 57, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_7);
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
 
-  /* "seleya/mfc/alchemy/qrank/glassdoor.py":58
+  /* "seleya/mfc/alchemy/qrank/glassdoor.pyx":58
  *                 lambda x: np.nan if x is None else self._mapping_dict[x])
  *         gd_reviews_data['reviewDateTime'] = pd.to_datetime(
  *             gd_reviews_data['reviewDateTime'])             # <<<<<<<<<<<<<<
  *         gd_reviews_data['date'] = pd.to_datetime(
  *             gd_reviews_data['reviewDateTime']).dt.strftime('%Y-12-31')
  */
   __pyx_t_3 = __Pyx_PyObject_Dict_GetItem(__pyx_v_gd_reviews_data, __pyx_n_s_reviewDateTime); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 58, __pyx_L1_error)
@@ -2808,38 +2808,38 @@
   __pyx_t_2 = (__pyx_t_1) ? __Pyx_PyObject_Call2Args(__pyx_t_7, __pyx_t_1, __pyx_t_3) : __Pyx_PyObject_CallOneArg(__pyx_t_7, __pyx_t_3);
   __Pyx_XDECREF(__pyx_t_1); __pyx_t_1 = 0;
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
   if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 57, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   __Pyx_DECREF(__pyx_t_7); __pyx_t_7 = 0;
 
-  /* "seleya/mfc/alchemy/qrank/glassdoor.py":57
+  /* "seleya/mfc/alchemy/qrank/glassdoor.pyx":57
  *             gd_reviews_data[col] = gd_reviews_data[col].apply(
  *                 lambda x: np.nan if x is None else self._mapping_dict[x])
  *         gd_reviews_data['reviewDateTime'] = pd.to_datetime(             # <<<<<<<<<<<<<<
  *             gd_reviews_data['reviewDateTime'])
  *         gd_reviews_data['date'] = pd.to_datetime(
  */
   if (unlikely(PyObject_SetItem(__pyx_v_gd_reviews_data, __pyx_n_s_reviewDateTime, __pyx_t_2) < 0)) __PYX_ERR(0, 57, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
 
-  /* "seleya/mfc/alchemy/qrank/glassdoor.py":59
+  /* "seleya/mfc/alchemy/qrank/glassdoor.pyx":59
  *         gd_reviews_data['reviewDateTime'] = pd.to_datetime(
  *             gd_reviews_data['reviewDateTime'])
  *         gd_reviews_data['date'] = pd.to_datetime(             # <<<<<<<<<<<<<<
  *             gd_reviews_data['reviewDateTime']).dt.strftime('%Y-12-31')
  *         return gd_reviews_data
  */
   __Pyx_GetModuleGlobalName(__pyx_t_3, __pyx_n_s_pd); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 59, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
   __pyx_t_1 = __Pyx_PyObject_GetAttrStr(__pyx_t_3, __pyx_n_s_to_datetime); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 59, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
 
-  /* "seleya/mfc/alchemy/qrank/glassdoor.py":60
+  /* "seleya/mfc/alchemy/qrank/glassdoor.pyx":60
  *             gd_reviews_data['reviewDateTime'])
  *         gd_reviews_data['date'] = pd.to_datetime(
  *             gd_reviews_data['reviewDateTime']).dt.strftime('%Y-12-31')             # <<<<<<<<<<<<<<
  *         return gd_reviews_data
  * 
  */
   __pyx_t_3 = __Pyx_PyObject_Dict_GetItem(__pyx_v_gd_reviews_data, __pyx_n_s_reviewDateTime); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 60, __pyx_L1_error)
@@ -2878,76 +2878,76 @@
   }
   __pyx_t_2 = (__pyx_t_1) ? __Pyx_PyObject_Call2Args(__pyx_t_7, __pyx_t_1, __pyx_kp_s_Y_12_31) : __Pyx_PyObject_CallOneArg(__pyx_t_7, __pyx_kp_s_Y_12_31);
   __Pyx_XDECREF(__pyx_t_1); __pyx_t_1 = 0;
   if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 60, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   __Pyx_DECREF(__pyx_t_7); __pyx_t_7 = 0;
 
-  /* "seleya/mfc/alchemy/qrank/glassdoor.py":59
+  /* "seleya/mfc/alchemy/qrank/glassdoor.pyx":59
  *         gd_reviews_data['reviewDateTime'] = pd.to_datetime(
  *             gd_reviews_data['reviewDateTime'])
  *         gd_reviews_data['date'] = pd.to_datetime(             # <<<<<<<<<<<<<<
  *             gd_reviews_data['reviewDateTime']).dt.strftime('%Y-12-31')
  *         return gd_reviews_data
  */
   if (unlikely(PyObject_SetItem(__pyx_v_gd_reviews_data, __pyx_n_s_date, __pyx_t_2) < 0)) __PYX_ERR(0, 59, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
 
-  /* "seleya/mfc/alchemy/qrank/glassdoor.py":61
+  /* "seleya/mfc/alchemy/qrank/glassdoor.pyx":61
  *         gd_reviews_data['date'] = pd.to_datetime(
  *             gd_reviews_data['reviewDateTime']).dt.strftime('%Y-12-31')
  *         return gd_reviews_data             # <<<<<<<<<<<<<<
  * 
  *     def prepare_data(self, begin_date=None, end_date=None):
  */
   __Pyx_XDECREF(__pyx_r);
   __Pyx_INCREF(__pyx_v_gd_reviews_data);
   __pyx_r = __pyx_v_gd_reviews_data;
   goto __pyx_L0;
 
-  /* "seleya/mfc/alchemy/qrank/glassdoor.py":42
+  /* "seleya/mfc/alchemy/qrank/glassdoor.pyx":42
  *         return gd_overview_data
  * 
  *     def _fetch_reviews(self, begin_date, end_date, cids):             # <<<<<<<<<<<<<<
  *         kd_logger.info('Fetching glassdoor reviews data...')
  *         columns = ['id', 'cid', 'reviewId', 'reviewDateTime'
  */
 
   /* function exit code */
   __pyx_L1_error:;
   __Pyx_XDECREF(__pyx_t_1);
   __Pyx_XDECREF(__pyx_t_2);
   __Pyx_XDECREF(__pyx_t_3);
   __Pyx_XDECREF(__pyx_t_7);
   __Pyx_XDECREF(__pyx_t_8);
-  __Pyx_AddTraceback("seleya.mfc.alchemy.qrank.glassdoo.Glassdoor._fetch_reviews", __pyx_clineno, __pyx_lineno, __pyx_filename);
+  __Pyx_AddTraceback("seleya.mfc.alchemy.qrank.glassdoor.Glassdoor._fetch_reviews", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __pyx_r = NULL;
   __pyx_L0:;
   __Pyx_XDECREF(__pyx_v_columns);
   __Pyx_XDECREF(__pyx_v_gd_reviews_data);
   __Pyx_XDECREF(__pyx_v_col);
   __Pyx_DECREF(((PyObject *)__pyx_cur_scope));
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "seleya/mfc/alchemy/qrank/glassdoor.py":63
+/* "seleya/mfc/alchemy/qrank/glassdoor.pyx":63
  *         return gd_reviews_data
  * 
  *     def prepare_data(self, begin_date=None, end_date=None):             # <<<<<<<<<<<<<<
  *         kd_logger.info('Fetching industry data...')
  *         industry_data = SurfaceDBAPI.Industry().fetch(
  */
 
 /* Python wrapper */
-static PyObject *__pyx_pw_6seleya_3mfc_7alchemy_5qrank_8glassdoo_9Glassdoor_7prepare_data(PyObject *__pyx_self, PyObject *__pyx_args, PyObject *__pyx_kwds); /*proto*/
-static char __pyx_doc_6seleya_3mfc_7alchemy_5qrank_8glassdoo_9Glassdoor_6prepare_data[] = "Glassdoor.prepare_data(self, begin_date=None, end_date=None)";
-static PyMethodDef __pyx_mdef_6seleya_3mfc_7alchemy_5qrank_8glassdoo_9Glassdoor_7prepare_data = {"prepare_data", (PyCFunction)(void*)(PyCFunctionWithKeywords)__pyx_pw_6seleya_3mfc_7alchemy_5qrank_8glassdoo_9Glassdoor_7prepare_data, METH_VARARGS|METH_KEYWORDS, __pyx_doc_6seleya_3mfc_7alchemy_5qrank_8glassdoo_9Glassdoor_6prepare_data};
-static PyObject *__pyx_pw_6seleya_3mfc_7alchemy_5qrank_8glassdoo_9Glassdoor_7prepare_data(PyObject *__pyx_self, PyObject *__pyx_args, PyObject *__pyx_kwds) {
+static PyObject *__pyx_pw_6seleya_3mfc_7alchemy_5qrank_9glassdoor_9Glassdoor_7prepare_data(PyObject *__pyx_self, PyObject *__pyx_args, PyObject *__pyx_kwds); /*proto*/
+static char __pyx_doc_6seleya_3mfc_7alchemy_5qrank_9glassdoor_9Glassdoor_6prepare_data[] = "Glassdoor.prepare_data(self, begin_date=None, end_date=None)";
+static PyMethodDef __pyx_mdef_6seleya_3mfc_7alchemy_5qrank_9glassdoor_9Glassdoor_7prepare_data = {"prepare_data", (PyCFunction)(void*)(PyCFunctionWithKeywords)__pyx_pw_6seleya_3mfc_7alchemy_5qrank_9glassdoor_9Glassdoor_7prepare_data, METH_VARARGS|METH_KEYWORDS, __pyx_doc_6seleya_3mfc_7alchemy_5qrank_9glassdoor_9Glassdoor_6prepare_data};
+static PyObject *__pyx_pw_6seleya_3mfc_7alchemy_5qrank_9glassdoor_9Glassdoor_7prepare_data(PyObject *__pyx_self, PyObject *__pyx_args, PyObject *__pyx_kwds) {
   PyObject *__pyx_v_self = 0;
   PyObject *__pyx_v_begin_date = 0;
   PyObject *__pyx_v_end_date = 0;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   PyObject *__pyx_r = 0;
@@ -3007,26 +3007,26 @@
     __pyx_v_begin_date = values[1];
     __pyx_v_end_date = values[2];
   }
   goto __pyx_L4_argument_unpacking_done;
   __pyx_L5_argtuple_error:;
   __Pyx_RaiseArgtupleInvalid("prepare_data", 0, 1, 3, PyTuple_GET_SIZE(__pyx_args)); __PYX_ERR(0, 63, __pyx_L3_error)
   __pyx_L3_error:;
-  __Pyx_AddTraceback("seleya.mfc.alchemy.qrank.glassdoo.Glassdoor.prepare_data", __pyx_clineno, __pyx_lineno, __pyx_filename);
+  __Pyx_AddTraceback("seleya.mfc.alchemy.qrank.glassdoor.Glassdoor.prepare_data", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __Pyx_RefNannyFinishContext();
   return NULL;
   __pyx_L4_argument_unpacking_done:;
-  __pyx_r = __pyx_pf_6seleya_3mfc_7alchemy_5qrank_8glassdoo_9Glassdoor_6prepare_data(__pyx_self, __pyx_v_self, __pyx_v_begin_date, __pyx_v_end_date);
+  __pyx_r = __pyx_pf_6seleya_3mfc_7alchemy_5qrank_9glassdoor_9Glassdoor_6prepare_data(__pyx_self, __pyx_v_self, __pyx_v_begin_date, __pyx_v_end_date);
 
   /* function exit code */
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-static PyObject *__pyx_pf_6seleya_3mfc_7alchemy_5qrank_8glassdoo_9Glassdoor_6prepare_data(CYTHON_UNUSED PyObject *__pyx_self, PyObject *__pyx_v_self, PyObject *__pyx_v_begin_date, PyObject *__pyx_v_end_date) {
+static PyObject *__pyx_pf_6seleya_3mfc_7alchemy_5qrank_9glassdoor_9Glassdoor_6prepare_data(CYTHON_UNUSED PyObject *__pyx_self, PyObject *__pyx_v_self, PyObject *__pyx_v_begin_date, PyObject *__pyx_v_end_date) {
   PyObject *__pyx_v_industry_data = NULL;
   PyObject *__pyx_v_codes = NULL;
   PyObject *__pyx_v_gd_overview_data = NULL;
   PyObject *__pyx_v_cids = NULL;
   PyObject *__pyx_v_gd_reviews_data = NULL;
   PyObject *__pyx_v_total_data = NULL;
   PyObject *__pyx_r = NULL;
@@ -3037,15 +3037,15 @@
   int __pyx_t_4;
   PyObject *__pyx_t_5 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("prepare_data", 0);
 
-  /* "seleya/mfc/alchemy/qrank/glassdoor.py":64
+  /* "seleya/mfc/alchemy/qrank/glassdoor.pyx":64
  * 
  *     def prepare_data(self, begin_date=None, end_date=None):
  *         kd_logger.info('Fetching industry data...')             # <<<<<<<<<<<<<<
  *         industry_data = SurfaceDBAPI.Industry().fetch(
  *             industry_code=self._industry_code,
  */
   __Pyx_GetModuleGlobalName(__pyx_t_2, __pyx_n_s_kd_logger); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 64, __pyx_L1_error)
@@ -3066,15 +3066,15 @@
   __pyx_t_1 = (__pyx_t_2) ? __Pyx_PyObject_Call2Args(__pyx_t_3, __pyx_t_2, __pyx_kp_s_Fetching_industry_data) : __Pyx_PyObject_CallOneArg(__pyx_t_3, __pyx_kp_s_Fetching_industry_data);
   __Pyx_XDECREF(__pyx_t_2); __pyx_t_2 = 0;
   if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 64, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
 
-  /* "seleya/mfc/alchemy/qrank/glassdoor.py":65
+  /* "seleya/mfc/alchemy/qrank/glassdoor.pyx":65
  *     def prepare_data(self, begin_date=None, end_date=None):
  *         kd_logger.info('Fetching industry data...')
  *         industry_data = SurfaceDBAPI.Industry().fetch(             # <<<<<<<<<<<<<<
  *             industry_code=self._industry_code,
  *             columns=['code', 'industry_id1'])
  */
   __Pyx_GetModuleGlobalName(__pyx_t_3, __pyx_n_s_SurfaceDBAPI); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 65, __pyx_L1_error)
@@ -3097,29 +3097,29 @@
   if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 65, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
   __pyx_t_2 = __Pyx_PyObject_GetAttrStr(__pyx_t_1, __pyx_n_s_fetch); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 65, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
 
-  /* "seleya/mfc/alchemy/qrank/glassdoor.py":66
+  /* "seleya/mfc/alchemy/qrank/glassdoor.pyx":66
  *         kd_logger.info('Fetching industry data...')
  *         industry_data = SurfaceDBAPI.Industry().fetch(
  *             industry_code=self._industry_code,             # <<<<<<<<<<<<<<
  *             columns=['code', 'industry_id1'])
  *         if industry_data.empty:
  */
   __pyx_t_1 = __Pyx_PyDict_NewPresized(2); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 66, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_t_3 = __Pyx_PyObject_GetAttrStr(__pyx_v_self, __pyx_n_s_industry_code_2); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 66, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
   if (PyDict_SetItem(__pyx_t_1, __pyx_n_s_industry_code, __pyx_t_3) < 0) __PYX_ERR(0, 66, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
 
-  /* "seleya/mfc/alchemy/qrank/glassdoor.py":67
+  /* "seleya/mfc/alchemy/qrank/glassdoor.pyx":67
  *         industry_data = SurfaceDBAPI.Industry().fetch(
  *             industry_code=self._industry_code,
  *             columns=['code', 'industry_id1'])             # <<<<<<<<<<<<<<
  *         if industry_data.empty:
  *             kd_logger.error('Industry data is empty')
  */
   __pyx_t_3 = PyList_New(2); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 67, __pyx_L1_error)
@@ -3129,42 +3129,42 @@
   PyList_SET_ITEM(__pyx_t_3, 0, __pyx_n_s_code);
   __Pyx_INCREF(__pyx_n_s_industry_id1);
   __Pyx_GIVEREF(__pyx_n_s_industry_id1);
   PyList_SET_ITEM(__pyx_t_3, 1, __pyx_n_s_industry_id1);
   if (PyDict_SetItem(__pyx_t_1, __pyx_n_s_columns, __pyx_t_3) < 0) __PYX_ERR(0, 66, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
 
-  /* "seleya/mfc/alchemy/qrank/glassdoor.py":65
+  /* "seleya/mfc/alchemy/qrank/glassdoor.pyx":65
  *     def prepare_data(self, begin_date=None, end_date=None):
  *         kd_logger.info('Fetching industry data...')
  *         industry_data = SurfaceDBAPI.Industry().fetch(             # <<<<<<<<<<<<<<
  *             industry_code=self._industry_code,
  *             columns=['code', 'industry_id1'])
  */
   __pyx_t_3 = __Pyx_PyObject_Call(__pyx_t_2, __pyx_empty_tuple, __pyx_t_1); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 65, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   __pyx_v_industry_data = __pyx_t_3;
   __pyx_t_3 = 0;
 
-  /* "seleya/mfc/alchemy/qrank/glassdoor.py":68
+  /* "seleya/mfc/alchemy/qrank/glassdoor.pyx":68
  *             industry_code=self._industry_code,
  *             columns=['code', 'industry_id1'])
  *         if industry_data.empty:             # <<<<<<<<<<<<<<
  *             kd_logger.error('Industry data is empty')
  *             return None
  */
   __pyx_t_3 = __Pyx_PyObject_GetAttrStr(__pyx_v_industry_data, __pyx_n_s_empty); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 68, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
   __pyx_t_4 = __Pyx_PyObject_IsTrue(__pyx_t_3); if (unlikely(__pyx_t_4 < 0)) __PYX_ERR(0, 68, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
   if (__pyx_t_4) {
 
-    /* "seleya/mfc/alchemy/qrank/glassdoor.py":69
+    /* "seleya/mfc/alchemy/qrank/glassdoor.pyx":69
  *             columns=['code', 'industry_id1'])
  *         if industry_data.empty:
  *             kd_logger.error('Industry data is empty')             # <<<<<<<<<<<<<<
  *             return None
  * 
  */
     __Pyx_GetModuleGlobalName(__pyx_t_1, __pyx_n_s_kd_logger); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 69, __pyx_L1_error)
@@ -3185,35 +3185,35 @@
     __pyx_t_3 = (__pyx_t_1) ? __Pyx_PyObject_Call2Args(__pyx_t_2, __pyx_t_1, __pyx_kp_s_Industry_data_is_empty) : __Pyx_PyObject_CallOneArg(__pyx_t_2, __pyx_kp_s_Industry_data_is_empty);
     __Pyx_XDECREF(__pyx_t_1); __pyx_t_1 = 0;
     if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 69, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_3);
     __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
     __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
 
-    /* "seleya/mfc/alchemy/qrank/glassdoor.py":70
+    /* "seleya/mfc/alchemy/qrank/glassdoor.pyx":70
  *         if industry_data.empty:
  *             kd_logger.error('Industry data is empty')
  *             return None             # <<<<<<<<<<<<<<
  * 
  *         codes = industry_data['code'].unique().tolist()
  */
     __Pyx_XDECREF(__pyx_r);
     __pyx_r = Py_None; __Pyx_INCREF(Py_None);
     goto __pyx_L0;
 
-    /* "seleya/mfc/alchemy/qrank/glassdoor.py":68
+    /* "seleya/mfc/alchemy/qrank/glassdoor.pyx":68
  *             industry_code=self._industry_code,
  *             columns=['code', 'industry_id1'])
  *         if industry_data.empty:             # <<<<<<<<<<<<<<
  *             kd_logger.error('Industry data is empty')
  *             return None
  */
   }
 
-  /* "seleya/mfc/alchemy/qrank/glassdoor.py":72
+  /* "seleya/mfc/alchemy/qrank/glassdoor.pyx":72
  *             return None
  * 
  *         codes = industry_data['code'].unique().tolist()             # <<<<<<<<<<<<<<
  *         gd_overview_data = self._fetch_overview(codes)
  *         if gd_overview_data.empty:
  */
   __pyx_t_1 = __Pyx_PyObject_Dict_GetItem(__pyx_v_industry_data, __pyx_n_s_code); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 72, __pyx_L1_error)
@@ -3253,15 +3253,15 @@
   __Pyx_XDECREF(__pyx_t_2); __pyx_t_2 = 0;
   if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 72, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
   __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
   __pyx_v_codes = __pyx_t_3;
   __pyx_t_3 = 0;
 
-  /* "seleya/mfc/alchemy/qrank/glassdoor.py":73
+  /* "seleya/mfc/alchemy/qrank/glassdoor.pyx":73
  * 
  *         codes = industry_data['code'].unique().tolist()
  *         gd_overview_data = self._fetch_overview(codes)             # <<<<<<<<<<<<<<
  *         if gd_overview_data.empty:
  *             kd_logger.error('Glassdoor overview data is empty')
  */
   __pyx_t_5 = __Pyx_PyObject_GetAttrStr(__pyx_v_self, __pyx_n_s_fetch_overview); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 73, __pyx_L1_error)
@@ -3280,28 +3280,28 @@
   __Pyx_XDECREF(__pyx_t_2); __pyx_t_2 = 0;
   if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 73, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
   __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
   __pyx_v_gd_overview_data = __pyx_t_3;
   __pyx_t_3 = 0;
 
-  /* "seleya/mfc/alchemy/qrank/glassdoor.py":74
+  /* "seleya/mfc/alchemy/qrank/glassdoor.pyx":74
  *         codes = industry_data['code'].unique().tolist()
  *         gd_overview_data = self._fetch_overview(codes)
  *         if gd_overview_data.empty:             # <<<<<<<<<<<<<<
  *             kd_logger.error('Glassdoor overview data is empty')
  *             return None
  */
   __pyx_t_3 = __Pyx_PyObject_GetAttrStr(__pyx_v_gd_overview_data, __pyx_n_s_empty); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 74, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
   __pyx_t_4 = __Pyx_PyObject_IsTrue(__pyx_t_3); if (unlikely(__pyx_t_4 < 0)) __PYX_ERR(0, 74, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
   if (__pyx_t_4) {
 
-    /* "seleya/mfc/alchemy/qrank/glassdoor.py":75
+    /* "seleya/mfc/alchemy/qrank/glassdoor.pyx":75
  *         gd_overview_data = self._fetch_overview(codes)
  *         if gd_overview_data.empty:
  *             kd_logger.error('Glassdoor overview data is empty')             # <<<<<<<<<<<<<<
  *             return None
  * 
  */
     __Pyx_GetModuleGlobalName(__pyx_t_5, __pyx_n_s_kd_logger); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 75, __pyx_L1_error)
@@ -3322,35 +3322,35 @@
     __pyx_t_3 = (__pyx_t_5) ? __Pyx_PyObject_Call2Args(__pyx_t_2, __pyx_t_5, __pyx_kp_s_Glassdoor_overview_data_is_empty) : __Pyx_PyObject_CallOneArg(__pyx_t_2, __pyx_kp_s_Glassdoor_overview_data_is_empty);
     __Pyx_XDECREF(__pyx_t_5); __pyx_t_5 = 0;
     if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 75, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_3);
     __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
     __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
 
-    /* "seleya/mfc/alchemy/qrank/glassdoor.py":76
+    /* "seleya/mfc/alchemy/qrank/glassdoor.pyx":76
  *         if gd_overview_data.empty:
  *             kd_logger.error('Glassdoor overview data is empty')
  *             return None             # <<<<<<<<<<<<<<
  * 
  *         cids = gd_overview_data['cid'].unique().tolist()
  */
     __Pyx_XDECREF(__pyx_r);
     __pyx_r = Py_None; __Pyx_INCREF(Py_None);
     goto __pyx_L0;
 
-    /* "seleya/mfc/alchemy/qrank/glassdoor.py":74
+    /* "seleya/mfc/alchemy/qrank/glassdoor.pyx":74
  *         codes = industry_data['code'].unique().tolist()
  *         gd_overview_data = self._fetch_overview(codes)
  *         if gd_overview_data.empty:             # <<<<<<<<<<<<<<
  *             kd_logger.error('Glassdoor overview data is empty')
  *             return None
  */
   }
 
-  /* "seleya/mfc/alchemy/qrank/glassdoor.py":78
+  /* "seleya/mfc/alchemy/qrank/glassdoor.pyx":78
  *             return None
  * 
  *         cids = gd_overview_data['cid'].unique().tolist()             # <<<<<<<<<<<<<<
  *         gd_reviews_data = self._fetch_reviews(begin_date=begin_date,
  *                                               end_date=end_date,
  */
   __pyx_t_5 = __Pyx_PyObject_Dict_GetItem(__pyx_v_gd_overview_data, __pyx_n_s_cid); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 78, __pyx_L1_error)
@@ -3390,73 +3390,73 @@
   __Pyx_XDECREF(__pyx_t_2); __pyx_t_2 = 0;
   if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 78, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   __pyx_v_cids = __pyx_t_3;
   __pyx_t_3 = 0;
 
-  /* "seleya/mfc/alchemy/qrank/glassdoor.py":79
+  /* "seleya/mfc/alchemy/qrank/glassdoor.pyx":79
  * 
  *         cids = gd_overview_data['cid'].unique().tolist()
  *         gd_reviews_data = self._fetch_reviews(begin_date=begin_date,             # <<<<<<<<<<<<<<
  *                                               end_date=end_date,
  *                                               cids=cids)
  */
   __pyx_t_3 = __Pyx_PyObject_GetAttrStr(__pyx_v_self, __pyx_n_s_fetch_reviews); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 79, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
   __pyx_t_1 = __Pyx_PyDict_NewPresized(3); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 79, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   if (PyDict_SetItem(__pyx_t_1, __pyx_n_s_begin_date, __pyx_v_begin_date) < 0) __PYX_ERR(0, 79, __pyx_L1_error)
 
-  /* "seleya/mfc/alchemy/qrank/glassdoor.py":80
+  /* "seleya/mfc/alchemy/qrank/glassdoor.pyx":80
  *         cids = gd_overview_data['cid'].unique().tolist()
  *         gd_reviews_data = self._fetch_reviews(begin_date=begin_date,
  *                                               end_date=end_date,             # <<<<<<<<<<<<<<
  *                                               cids=cids)
  *         if gd_reviews_data.empty:
  */
   if (PyDict_SetItem(__pyx_t_1, __pyx_n_s_end_date, __pyx_v_end_date) < 0) __PYX_ERR(0, 79, __pyx_L1_error)
 
-  /* "seleya/mfc/alchemy/qrank/glassdoor.py":81
+  /* "seleya/mfc/alchemy/qrank/glassdoor.pyx":81
  *         gd_reviews_data = self._fetch_reviews(begin_date=begin_date,
  *                                               end_date=end_date,
  *                                               cids=cids)             # <<<<<<<<<<<<<<
  *         if gd_reviews_data.empty:
  *             kd_logger.error('Glassdoor reviews data is empty')
  */
   if (PyDict_SetItem(__pyx_t_1, __pyx_n_s_cids, __pyx_v_cids) < 0) __PYX_ERR(0, 79, __pyx_L1_error)
 
-  /* "seleya/mfc/alchemy/qrank/glassdoor.py":79
+  /* "seleya/mfc/alchemy/qrank/glassdoor.pyx":79
  * 
  *         cids = gd_overview_data['cid'].unique().tolist()
  *         gd_reviews_data = self._fetch_reviews(begin_date=begin_date,             # <<<<<<<<<<<<<<
  *                                               end_date=end_date,
  *                                               cids=cids)
  */
   __pyx_t_2 = __Pyx_PyObject_Call(__pyx_t_3, __pyx_empty_tuple, __pyx_t_1); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 79, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   __pyx_v_gd_reviews_data = __pyx_t_2;
   __pyx_t_2 = 0;
 
-  /* "seleya/mfc/alchemy/qrank/glassdoor.py":82
+  /* "seleya/mfc/alchemy/qrank/glassdoor.pyx":82
  *                                               end_date=end_date,
  *                                               cids=cids)
  *         if gd_reviews_data.empty:             # <<<<<<<<<<<<<<
  *             kd_logger.error('Glassdoor reviews data is empty')
  *             return None
  */
   __pyx_t_2 = __Pyx_PyObject_GetAttrStr(__pyx_v_gd_reviews_data, __pyx_n_s_empty); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 82, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   __pyx_t_4 = __Pyx_PyObject_IsTrue(__pyx_t_2); if (unlikely(__pyx_t_4 < 0)) __PYX_ERR(0, 82, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
   if (__pyx_t_4) {
 
-    /* "seleya/mfc/alchemy/qrank/glassdoor.py":83
+    /* "seleya/mfc/alchemy/qrank/glassdoor.pyx":83
  *                                               cids=cids)
  *         if gd_reviews_data.empty:
  *             kd_logger.error('Glassdoor reviews data is empty')             # <<<<<<<<<<<<<<
  *             return None
  * 
  */
     __Pyx_GetModuleGlobalName(__pyx_t_1, __pyx_n_s_kd_logger); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 83, __pyx_L1_error)
@@ -3477,35 +3477,35 @@
     __pyx_t_2 = (__pyx_t_1) ? __Pyx_PyObject_Call2Args(__pyx_t_3, __pyx_t_1, __pyx_kp_s_Glassdoor_reviews_data_is_empty) : __Pyx_PyObject_CallOneArg(__pyx_t_3, __pyx_kp_s_Glassdoor_reviews_data_is_empty);
     __Pyx_XDECREF(__pyx_t_1); __pyx_t_1 = 0;
     if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 83, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_2);
     __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
     __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
 
-    /* "seleya/mfc/alchemy/qrank/glassdoor.py":84
+    /* "seleya/mfc/alchemy/qrank/glassdoor.pyx":84
  *         if gd_reviews_data.empty:
  *             kd_logger.error('Glassdoor reviews data is empty')
  *             return None             # <<<<<<<<<<<<<<
  * 
  *         kd_logger.info('merging glassdoor data...')
  */
     __Pyx_XDECREF(__pyx_r);
     __pyx_r = Py_None; __Pyx_INCREF(Py_None);
     goto __pyx_L0;
 
-    /* "seleya/mfc/alchemy/qrank/glassdoor.py":82
+    /* "seleya/mfc/alchemy/qrank/glassdoor.pyx":82
  *                                               end_date=end_date,
  *                                               cids=cids)
  *         if gd_reviews_data.empty:             # <<<<<<<<<<<<<<
  *             kd_logger.error('Glassdoor reviews data is empty')
  *             return None
  */
   }
 
-  /* "seleya/mfc/alchemy/qrank/glassdoor.py":86
+  /* "seleya/mfc/alchemy/qrank/glassdoor.pyx":86
  *             return None
  * 
  *         kd_logger.info('merging glassdoor data...')             # <<<<<<<<<<<<<<
  *         total_data = gd_reviews_data.merge(gd_overview_data,
  *                                            on=['cid'],
  */
   __Pyx_GetModuleGlobalName(__pyx_t_3, __pyx_n_s_kd_logger); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 86, __pyx_L1_error)
@@ -3526,30 +3526,30 @@
   __pyx_t_2 = (__pyx_t_3) ? __Pyx_PyObject_Call2Args(__pyx_t_1, __pyx_t_3, __pyx_kp_s_merging_glassdoor_data) : __Pyx_PyObject_CallOneArg(__pyx_t_1, __pyx_kp_s_merging_glassdoor_data);
   __Pyx_XDECREF(__pyx_t_3); __pyx_t_3 = 0;
   if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 86, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
 
-  /* "seleya/mfc/alchemy/qrank/glassdoor.py":87
+  /* "seleya/mfc/alchemy/qrank/glassdoor.pyx":87
  * 
  *         kd_logger.info('merging glassdoor data...')
  *         total_data = gd_reviews_data.merge(gd_overview_data,             # <<<<<<<<<<<<<<
  *                                            on=['cid'],
  *                                            how='left')
  */
   __pyx_t_2 = __Pyx_PyObject_GetAttrStr(__pyx_v_gd_reviews_data, __pyx_n_s_merge); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 87, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   __pyx_t_1 = PyTuple_New(1); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 87, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __Pyx_INCREF(__pyx_v_gd_overview_data);
   __Pyx_GIVEREF(__pyx_v_gd_overview_data);
   PyTuple_SET_ITEM(__pyx_t_1, 0, __pyx_v_gd_overview_data);
 
-  /* "seleya/mfc/alchemy/qrank/glassdoor.py":88
+  /* "seleya/mfc/alchemy/qrank/glassdoor.pyx":88
  *         kd_logger.info('merging glassdoor data...')
  *         total_data = gd_reviews_data.merge(gd_overview_data,
  *                                            on=['cid'],             # <<<<<<<<<<<<<<
  *                                            how='left')
  *         return total_data
  */
   __pyx_t_3 = __Pyx_PyDict_NewPresized(2); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 88, __pyx_L1_error)
@@ -3559,82 +3559,82 @@
   __Pyx_INCREF(__pyx_n_s_cid);
   __Pyx_GIVEREF(__pyx_n_s_cid);
   PyList_SET_ITEM(__pyx_t_5, 0, __pyx_n_s_cid);
   if (PyDict_SetItem(__pyx_t_3, __pyx_n_s_on, __pyx_t_5) < 0) __PYX_ERR(0, 88, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
   if (PyDict_SetItem(__pyx_t_3, __pyx_n_s_how, __pyx_n_s_left) < 0) __PYX_ERR(0, 88, __pyx_L1_error)
 
-  /* "seleya/mfc/alchemy/qrank/glassdoor.py":87
+  /* "seleya/mfc/alchemy/qrank/glassdoor.pyx":87
  * 
  *         kd_logger.info('merging glassdoor data...')
  *         total_data = gd_reviews_data.merge(gd_overview_data,             # <<<<<<<<<<<<<<
  *                                            on=['cid'],
  *                                            how='left')
  */
   __pyx_t_5 = __Pyx_PyObject_Call(__pyx_t_2, __pyx_t_1, __pyx_t_3); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 87, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_5);
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
   __pyx_v_total_data = __pyx_t_5;
   __pyx_t_5 = 0;
 
-  /* "seleya/mfc/alchemy/qrank/glassdoor.py":90
+  /* "seleya/mfc/alchemy/qrank/glassdoor.pyx":90
  *                                            on=['cid'],
  *                                            how='left')
  *         return total_data             # <<<<<<<<<<<<<<
  * 
  *     def _transform_raw(self, mean_data):
  */
   __Pyx_XDECREF(__pyx_r);
   __Pyx_INCREF(__pyx_v_total_data);
   __pyx_r = __pyx_v_total_data;
   goto __pyx_L0;
 
-  /* "seleya/mfc/alchemy/qrank/glassdoor.py":63
+  /* "seleya/mfc/alchemy/qrank/glassdoor.pyx":63
  *         return gd_reviews_data
  * 
  *     def prepare_data(self, begin_date=None, end_date=None):             # <<<<<<<<<<<<<<
  *         kd_logger.info('Fetching industry data...')
  *         industry_data = SurfaceDBAPI.Industry().fetch(
  */
 
   /* function exit code */
   __pyx_L1_error:;
   __Pyx_XDECREF(__pyx_t_1);
   __Pyx_XDECREF(__pyx_t_2);
   __Pyx_XDECREF(__pyx_t_3);
   __Pyx_XDECREF(__pyx_t_5);
-  __Pyx_AddTraceback("seleya.mfc.alchemy.qrank.glassdoo.Glassdoor.prepare_data", __pyx_clineno, __pyx_lineno, __pyx_filename);
+  __Pyx_AddTraceback("seleya.mfc.alchemy.qrank.glassdoor.Glassdoor.prepare_data", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __pyx_r = NULL;
   __pyx_L0:;
   __Pyx_XDECREF(__pyx_v_industry_data);
   __Pyx_XDECREF(__pyx_v_codes);
   __Pyx_XDECREF(__pyx_v_gd_overview_data);
   __Pyx_XDECREF(__pyx_v_cids);
   __Pyx_XDECREF(__pyx_v_gd_reviews_data);
   __Pyx_XDECREF(__pyx_v_total_data);
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "seleya/mfc/alchemy/qrank/glassdoor.py":92
+/* "seleya/mfc/alchemy/qrank/glassdoor.pyx":92
  *         return total_data
  * 
  *     def _transform_raw(self, mean_data):             # <<<<<<<<<<<<<<
  *         # save the raw average scores for UI use
  *         raw_data = mean_data.reset_index().set_index([
  */
 
 /* Python wrapper */
-static PyObject *__pyx_pw_6seleya_3mfc_7alchemy_5qrank_8glassdoo_9Glassdoor_9_transform_raw(PyObject *__pyx_self, PyObject *__pyx_args, PyObject *__pyx_kwds); /*proto*/
-static char __pyx_doc_6seleya_3mfc_7alchemy_5qrank_8glassdoo_9Glassdoor_8_transform_raw[] = "Glassdoor._transform_raw(self, mean_data)";
-static PyMethodDef __pyx_mdef_6seleya_3mfc_7alchemy_5qrank_8glassdoo_9Glassdoor_9_transform_raw = {"_transform_raw", (PyCFunction)(void*)(PyCFunctionWithKeywords)__pyx_pw_6seleya_3mfc_7alchemy_5qrank_8glassdoo_9Glassdoor_9_transform_raw, METH_VARARGS|METH_KEYWORDS, __pyx_doc_6seleya_3mfc_7alchemy_5qrank_8glassdoo_9Glassdoor_8_transform_raw};
-static PyObject *__pyx_pw_6seleya_3mfc_7alchemy_5qrank_8glassdoo_9Glassdoor_9_transform_raw(PyObject *__pyx_self, PyObject *__pyx_args, PyObject *__pyx_kwds) {
+static PyObject *__pyx_pw_6seleya_3mfc_7alchemy_5qrank_9glassdoor_9Glassdoor_9_transform_raw(PyObject *__pyx_self, PyObject *__pyx_args, PyObject *__pyx_kwds); /*proto*/
+static char __pyx_doc_6seleya_3mfc_7alchemy_5qrank_9glassdoor_9Glassdoor_8_transform_raw[] = "Glassdoor._transform_raw(self, mean_data)";
+static PyMethodDef __pyx_mdef_6seleya_3mfc_7alchemy_5qrank_9glassdoor_9Glassdoor_9_transform_raw = {"_transform_raw", (PyCFunction)(void*)(PyCFunctionWithKeywords)__pyx_pw_6seleya_3mfc_7alchemy_5qrank_9glassdoor_9Glassdoor_9_transform_raw, METH_VARARGS|METH_KEYWORDS, __pyx_doc_6seleya_3mfc_7alchemy_5qrank_9glassdoor_9Glassdoor_8_transform_raw};
+static PyObject *__pyx_pw_6seleya_3mfc_7alchemy_5qrank_9glassdoor_9Glassdoor_9_transform_raw(PyObject *__pyx_self, PyObject *__pyx_args, PyObject *__pyx_kwds) {
   PyObject *__pyx_v_self = 0;
   PyObject *__pyx_v_mean_data = 0;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   PyObject *__pyx_r = 0;
   __Pyx_RefNannyDeclarations
@@ -3677,41 +3677,41 @@
     __pyx_v_self = values[0];
     __pyx_v_mean_data = values[1];
   }
   goto __pyx_L4_argument_unpacking_done;
   __pyx_L5_argtuple_error:;
   __Pyx_RaiseArgtupleInvalid("_transform_raw", 1, 2, 2, PyTuple_GET_SIZE(__pyx_args)); __PYX_ERR(0, 92, __pyx_L3_error)
   __pyx_L3_error:;
-  __Pyx_AddTraceback("seleya.mfc.alchemy.qrank.glassdoo.Glassdoor._transform_raw", __pyx_clineno, __pyx_lineno, __pyx_filename);
+  __Pyx_AddTraceback("seleya.mfc.alchemy.qrank.glassdoor.Glassdoor._transform_raw", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __Pyx_RefNannyFinishContext();
   return NULL;
   __pyx_L4_argument_unpacking_done:;
-  __pyx_r = __pyx_pf_6seleya_3mfc_7alchemy_5qrank_8glassdoo_9Glassdoor_8_transform_raw(__pyx_self, __pyx_v_self, __pyx_v_mean_data);
+  __pyx_r = __pyx_pf_6seleya_3mfc_7alchemy_5qrank_9glassdoor_9Glassdoor_8_transform_raw(__pyx_self, __pyx_v_self, __pyx_v_mean_data);
 
   /* function exit code */
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-static PyObject *__pyx_pf_6seleya_3mfc_7alchemy_5qrank_8glassdoo_9Glassdoor_8_transform_raw(CYTHON_UNUSED PyObject *__pyx_self, PyObject *__pyx_v_self, PyObject *__pyx_v_mean_data) {
+static PyObject *__pyx_pf_6seleya_3mfc_7alchemy_5qrank_9glassdoor_9Glassdoor_8_transform_raw(CYTHON_UNUSED PyObject *__pyx_self, PyObject *__pyx_v_self, PyObject *__pyx_v_mean_data) {
   PyObject *__pyx_v_raw_data = NULL;
   PyObject *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   PyObject *__pyx_t_2 = NULL;
   PyObject *__pyx_t_3 = NULL;
   PyObject *__pyx_t_4 = NULL;
   PyObject *__pyx_t_5 = NULL;
   PyObject *__pyx_t_6 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("_transform_raw", 0);
 
-  /* "seleya/mfc/alchemy/qrank/glassdoor.py":94
+  /* "seleya/mfc/alchemy/qrank/glassdoor.pyx":94
  *     def _transform_raw(self, mean_data):
  *         # save the raw average scores for UI use
  *         raw_data = mean_data.reset_index().set_index([             # <<<<<<<<<<<<<<
  *             'date',
  *             'code',
  */
   __pyx_t_5 = __Pyx_PyObject_GetAttrStr(__pyx_v_mean_data, __pyx_n_s_reset_index); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 94, __pyx_L1_error)
@@ -3755,15 +3755,15 @@
   __pyx_t_3 = (__pyx_t_6) ? __Pyx_PyObject_Call2Args(__pyx_t_5, __pyx_t_6, __pyx_t_4) : __Pyx_PyObject_CallOneArg(__pyx_t_5, __pyx_t_4);
   __Pyx_XDECREF(__pyx_t_6); __pyx_t_6 = 0;
   __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
   if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 94, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
   __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
 
-  /* "seleya/mfc/alchemy/qrank/glassdoor.py":97
+  /* "seleya/mfc/alchemy/qrank/glassdoor.pyx":97
  *             'date',
  *             'code',
  *         ]).stack().reset_index().rename(columns={             # <<<<<<<<<<<<<<
  *             'level_2': 'name',
  *             0: 'value'
  */
   __pyx_t_5 = __Pyx_PyObject_GetAttrStr(__pyx_t_3, __pyx_n_s_stack); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 97, __pyx_L1_error)
@@ -3804,56 +3804,56 @@
   __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
   __pyx_t_5 = __Pyx_PyObject_GetAttrStr(__pyx_t_1, __pyx_n_s_rename); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 97, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_5);
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   __pyx_t_1 = __Pyx_PyDict_NewPresized(1); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 97, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
 
-  /* "seleya/mfc/alchemy/qrank/glassdoor.py":98
+  /* "seleya/mfc/alchemy/qrank/glassdoor.pyx":98
  *             'code',
  *         ]).stack().reset_index().rename(columns={
  *             'level_2': 'name',             # <<<<<<<<<<<<<<
  *             0: 'value'
  *         })
  */
   __pyx_t_2 = __Pyx_PyDict_NewPresized(2); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 98, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   if (PyDict_SetItem(__pyx_t_2, __pyx_n_s_level_2, __pyx_n_s_name) < 0) __PYX_ERR(0, 98, __pyx_L1_error)
   if (PyDict_SetItem(__pyx_t_2, __pyx_int_0, __pyx_n_s_value) < 0) __PYX_ERR(0, 98, __pyx_L1_error)
   if (PyDict_SetItem(__pyx_t_1, __pyx_n_s_columns, __pyx_t_2) < 0) __PYX_ERR(0, 97, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
 
-  /* "seleya/mfc/alchemy/qrank/glassdoor.py":97
+  /* "seleya/mfc/alchemy/qrank/glassdoor.pyx":97
  *             'date',
  *             'code',
  *         ]).stack().reset_index().rename(columns={             # <<<<<<<<<<<<<<
  *             'level_2': 'name',
  *             0: 'value'
  */
   __pyx_t_2 = __Pyx_PyObject_Call(__pyx_t_5, __pyx_empty_tuple, __pyx_t_1); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 97, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   __pyx_v_raw_data = __pyx_t_2;
   __pyx_t_2 = 0;
 
-  /* "seleya/mfc/alchemy/qrank/glassdoor.py":101
+  /* "seleya/mfc/alchemy/qrank/glassdoor.pyx":101
  *             0: 'value'
  *         })
  *         raw_data['date'] = pd.to_datetime(             # <<<<<<<<<<<<<<
  *             raw_data['date']).dt.strftime('%Y-%m-%d')
  *         raw_data['industry'] = self._industry_code
  */
   __Pyx_GetModuleGlobalName(__pyx_t_5, __pyx_n_s_pd); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 101, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_5);
   __pyx_t_3 = __Pyx_PyObject_GetAttrStr(__pyx_t_5, __pyx_n_s_to_datetime); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 101, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
   __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
 
-  /* "seleya/mfc/alchemy/qrank/glassdoor.py":102
+  /* "seleya/mfc/alchemy/qrank/glassdoor.pyx":102
  *         })
  *         raw_data['date'] = pd.to_datetime(
  *             raw_data['date']).dt.strftime('%Y-%m-%d')             # <<<<<<<<<<<<<<
  *         raw_data['industry'] = self._industry_code
  *         return raw_data
  */
   __pyx_t_5 = __Pyx_PyObject_Dict_GetItem(__pyx_v_raw_data, __pyx_n_s_date); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 102, __pyx_L1_error)
@@ -3892,49 +3892,49 @@
   }
   __pyx_t_2 = (__pyx_t_3) ? __Pyx_PyObject_Call2Args(__pyx_t_1, __pyx_t_3, __pyx_kp_s_Y_m_d) : __Pyx_PyObject_CallOneArg(__pyx_t_1, __pyx_kp_s_Y_m_d);
   __Pyx_XDECREF(__pyx_t_3); __pyx_t_3 = 0;
   if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 102, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
 
-  /* "seleya/mfc/alchemy/qrank/glassdoor.py":101
+  /* "seleya/mfc/alchemy/qrank/glassdoor.pyx":101
  *             0: 'value'
  *         })
  *         raw_data['date'] = pd.to_datetime(             # <<<<<<<<<<<<<<
  *             raw_data['date']).dt.strftime('%Y-%m-%d')
  *         raw_data['industry'] = self._industry_code
  */
   if (unlikely(PyObject_SetItem(__pyx_v_raw_data, __pyx_n_s_date, __pyx_t_2) < 0)) __PYX_ERR(0, 101, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
 
-  /* "seleya/mfc/alchemy/qrank/glassdoor.py":103
+  /* "seleya/mfc/alchemy/qrank/glassdoor.pyx":103
  *         raw_data['date'] = pd.to_datetime(
  *             raw_data['date']).dt.strftime('%Y-%m-%d')
  *         raw_data['industry'] = self._industry_code             # <<<<<<<<<<<<<<
  *         return raw_data
  * 
  */
   __pyx_t_2 = __Pyx_PyObject_GetAttrStr(__pyx_v_self, __pyx_n_s_industry_code_2); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 103, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   if (unlikely(PyObject_SetItem(__pyx_v_raw_data, __pyx_n_s_industry, __pyx_t_2) < 0)) __PYX_ERR(0, 103, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
 
-  /* "seleya/mfc/alchemy/qrank/glassdoor.py":104
+  /* "seleya/mfc/alchemy/qrank/glassdoor.pyx":104
  *             raw_data['date']).dt.strftime('%Y-%m-%d')
  *         raw_data['industry'] = self._industry_code
  *         return raw_data             # <<<<<<<<<<<<<<
  * 
  *     def _blom_score(self, values_series, threshold=0.9):
  */
   __Pyx_XDECREF(__pyx_r);
   __Pyx_INCREF(__pyx_v_raw_data);
   __pyx_r = __pyx_v_raw_data;
   goto __pyx_L0;
 
-  /* "seleya/mfc/alchemy/qrank/glassdoor.py":92
+  /* "seleya/mfc/alchemy/qrank/glassdoor.pyx":92
  *         return total_data
  * 
  *     def _transform_raw(self, mean_data):             # <<<<<<<<<<<<<<
  *         # save the raw average scores for UI use
  *         raw_data = mean_data.reset_index().set_index([
  */
 
@@ -3942,36 +3942,36 @@
   __pyx_L1_error:;
   __Pyx_XDECREF(__pyx_t_1);
   __Pyx_XDECREF(__pyx_t_2);
   __Pyx_XDECREF(__pyx_t_3);
   __Pyx_XDECREF(__pyx_t_4);
   __Pyx_XDECREF(__pyx_t_5);
   __Pyx_XDECREF(__pyx_t_6);
-  __Pyx_AddTraceback("seleya.mfc.alchemy.qrank.glassdoo.Glassdoor._transform_raw", __pyx_clineno, __pyx_lineno, __pyx_filename);
+  __Pyx_AddTraceback("seleya.mfc.alchemy.qrank.glassdoor.Glassdoor._transform_raw", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __pyx_r = NULL;
   __pyx_L0:;
   __Pyx_XDECREF(__pyx_v_raw_data);
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "seleya/mfc/alchemy/qrank/glassdoor.py":106
+/* "seleya/mfc/alchemy/qrank/glassdoor.pyx":106
  *         return raw_data
  * 
  *     def _blom_score(self, values_series, threshold=0.9):             # <<<<<<<<<<<<<<
  *         idx = values_series.index.droplevel(level=0)
  *         coverage = values_series.isna().sum() / len(values_series)
  */
 
 /* Python wrapper */
-static PyObject *__pyx_pw_6seleya_3mfc_7alchemy_5qrank_8glassdoo_9Glassdoor_11_blom_score(PyObject *__pyx_self, PyObject *__pyx_args, PyObject *__pyx_kwds); /*proto*/
-static char __pyx_doc_6seleya_3mfc_7alchemy_5qrank_8glassdoo_9Glassdoor_10_blom_score[] = "Glassdoor._blom_score(self, values_series, threshold=0.9)";
-static PyMethodDef __pyx_mdef_6seleya_3mfc_7alchemy_5qrank_8glassdoo_9Glassdoor_11_blom_score = {"_blom_score", (PyCFunction)(void*)(PyCFunctionWithKeywords)__pyx_pw_6seleya_3mfc_7alchemy_5qrank_8glassdoo_9Glassdoor_11_blom_score, METH_VARARGS|METH_KEYWORDS, __pyx_doc_6seleya_3mfc_7alchemy_5qrank_8glassdoo_9Glassdoor_10_blom_score};
-static PyObject *__pyx_pw_6seleya_3mfc_7alchemy_5qrank_8glassdoo_9Glassdoor_11_blom_score(PyObject *__pyx_self, PyObject *__pyx_args, PyObject *__pyx_kwds) {
+static PyObject *__pyx_pw_6seleya_3mfc_7alchemy_5qrank_9glassdoor_9Glassdoor_11_blom_score(PyObject *__pyx_self, PyObject *__pyx_args, PyObject *__pyx_kwds); /*proto*/
+static char __pyx_doc_6seleya_3mfc_7alchemy_5qrank_9glassdoor_9Glassdoor_10_blom_score[] = "Glassdoor._blom_score(self, values_series, threshold=0.9)";
+static PyMethodDef __pyx_mdef_6seleya_3mfc_7alchemy_5qrank_9glassdoor_9Glassdoor_11_blom_score = {"_blom_score", (PyCFunction)(void*)(PyCFunctionWithKeywords)__pyx_pw_6seleya_3mfc_7alchemy_5qrank_9glassdoor_9Glassdoor_11_blom_score, METH_VARARGS|METH_KEYWORDS, __pyx_doc_6seleya_3mfc_7alchemy_5qrank_9glassdoor_9Glassdoor_10_blom_score};
+static PyObject *__pyx_pw_6seleya_3mfc_7alchemy_5qrank_9glassdoor_9Glassdoor_11_blom_score(PyObject *__pyx_self, PyObject *__pyx_args, PyObject *__pyx_kwds) {
   CYTHON_UNUSED PyObject *__pyx_v_self = 0;
   PyObject *__pyx_v_values_series = 0;
   PyObject *__pyx_v_threshold = 0;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   PyObject *__pyx_r = 0;
@@ -4029,26 +4029,26 @@
     __pyx_v_values_series = values[1];
     __pyx_v_threshold = values[2];
   }
   goto __pyx_L4_argument_unpacking_done;
   __pyx_L5_argtuple_error:;
   __Pyx_RaiseArgtupleInvalid("_blom_score", 0, 2, 3, PyTuple_GET_SIZE(__pyx_args)); __PYX_ERR(0, 106, __pyx_L3_error)
   __pyx_L3_error:;
-  __Pyx_AddTraceback("seleya.mfc.alchemy.qrank.glassdoo.Glassdoor._blom_score", __pyx_clineno, __pyx_lineno, __pyx_filename);
+  __Pyx_AddTraceback("seleya.mfc.alchemy.qrank.glassdoor.Glassdoor._blom_score", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __Pyx_RefNannyFinishContext();
   return NULL;
   __pyx_L4_argument_unpacking_done:;
-  __pyx_r = __pyx_pf_6seleya_3mfc_7alchemy_5qrank_8glassdoo_9Glassdoor_10_blom_score(__pyx_self, __pyx_v_self, __pyx_v_values_series, __pyx_v_threshold);
+  __pyx_r = __pyx_pf_6seleya_3mfc_7alchemy_5qrank_9glassdoor_9Glassdoor_10_blom_score(__pyx_self, __pyx_v_self, __pyx_v_values_series, __pyx_v_threshold);
 
   /* function exit code */
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-static PyObject *__pyx_pf_6seleya_3mfc_7alchemy_5qrank_8glassdoo_9Glassdoor_10_blom_score(CYTHON_UNUSED PyObject *__pyx_self, CYTHON_UNUSED PyObject *__pyx_v_self, PyObject *__pyx_v_values_series, PyObject *__pyx_v_threshold) {
+static PyObject *__pyx_pf_6seleya_3mfc_7alchemy_5qrank_9glassdoor_9Glassdoor_10_blom_score(CYTHON_UNUSED PyObject *__pyx_self, CYTHON_UNUSED PyObject *__pyx_v_self, PyObject *__pyx_v_values_series, PyObject *__pyx_v_threshold) {
   PyObject *__pyx_v_idx = NULL;
   PyObject *__pyx_v_coverage = NULL;
   PyObject *__pyx_v_scores = NULL;
   PyObject *__pyx_v_ranks = NULL;
   PyObject *__pyx_v_n = NULL;
   CYTHON_UNUSED Py_ssize_t __pyx_v__;
   PyObject *__pyx_r = NULL;
@@ -4064,15 +4064,15 @@
   PyObject *__pyx_t_9 = NULL;
   PyObject *__pyx_t_10 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("_blom_score", 0);
 
-  /* "seleya/mfc/alchemy/qrank/glassdoor.py":107
+  /* "seleya/mfc/alchemy/qrank/glassdoor.pyx":107
  * 
  *     def _blom_score(self, values_series, threshold=0.9):
  *         idx = values_series.index.droplevel(level=0)             # <<<<<<<<<<<<<<
  *         coverage = values_series.isna().sum() / len(values_series)
  *         if coverage > threshold:
  */
   __pyx_t_1 = __Pyx_PyObject_GetAttrStr(__pyx_v_values_series, __pyx_n_s_index); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 107, __pyx_L1_error)
@@ -4086,15 +4086,15 @@
   __pyx_t_3 = __Pyx_PyObject_Call(__pyx_t_2, __pyx_empty_tuple, __pyx_t_1); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 107, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   __pyx_v_idx = __pyx_t_3;
   __pyx_t_3 = 0;
 
-  /* "seleya/mfc/alchemy/qrank/glassdoor.py":108
+  /* "seleya/mfc/alchemy/qrank/glassdoor.pyx":108
  *     def _blom_score(self, values_series, threshold=0.9):
  *         idx = values_series.index.droplevel(level=0)
  *         coverage = values_series.isna().sum() / len(values_series)             # <<<<<<<<<<<<<<
  *         if coverage > threshold:
  *             scores = [np.nan for _ in range(len(values_series))]
  */
   __pyx_t_2 = __Pyx_PyObject_GetAttrStr(__pyx_v_values_series, __pyx_n_s_isna); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 108, __pyx_L1_error)
@@ -4138,27 +4138,27 @@
   __pyx_t_1 = __Pyx_PyNumber_Divide(__pyx_t_3, __pyx_t_2); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 108, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
   __pyx_v_coverage = __pyx_t_1;
   __pyx_t_1 = 0;
 
-  /* "seleya/mfc/alchemy/qrank/glassdoor.py":109
+  /* "seleya/mfc/alchemy/qrank/glassdoor.pyx":109
  *         idx = values_series.index.droplevel(level=0)
  *         coverage = values_series.isna().sum() / len(values_series)
  *         if coverage > threshold:             # <<<<<<<<<<<<<<
  *             scores = [np.nan for _ in range(len(values_series))]
  *         else:
  */
   __pyx_t_1 = PyObject_RichCompare(__pyx_v_coverage, __pyx_v_threshold, Py_GT); __Pyx_XGOTREF(__pyx_t_1); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 109, __pyx_L1_error)
   __pyx_t_6 = __Pyx_PyObject_IsTrue(__pyx_t_1); if (unlikely(__pyx_t_6 < 0)) __PYX_ERR(0, 109, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   if (__pyx_t_6) {
 
-    /* "seleya/mfc/alchemy/qrank/glassdoor.py":110
+    /* "seleya/mfc/alchemy/qrank/glassdoor.pyx":110
  *         coverage = values_series.isna().sum() / len(values_series)
  *         if coverage > threshold:
  *             scores = [np.nan for _ in range(len(values_series))]             # <<<<<<<<<<<<<<
  *         else:
  *             ranks = stats.mstats.rankdata(np.ma.masked_invalid(values_series))
  */
     __pyx_t_1 = PyList_New(0); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 110, __pyx_L1_error)
@@ -4174,25 +4174,25 @@
       __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
       if (unlikely(__Pyx_ListComp_Append(__pyx_t_1, (PyObject*)__pyx_t_3))) __PYX_ERR(0, 110, __pyx_L1_error)
       __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
     }
     __pyx_v_scores = __pyx_t_1;
     __pyx_t_1 = 0;
 
-    /* "seleya/mfc/alchemy/qrank/glassdoor.py":109
+    /* "seleya/mfc/alchemy/qrank/glassdoor.pyx":109
  *         idx = values_series.index.droplevel(level=0)
  *         coverage = values_series.isna().sum() / len(values_series)
  *         if coverage > threshold:             # <<<<<<<<<<<<<<
  *             scores = [np.nan for _ in range(len(values_series))]
  *         else:
  */
     goto __pyx_L3;
   }
 
-  /* "seleya/mfc/alchemy/qrank/glassdoor.py":112
+  /* "seleya/mfc/alchemy/qrank/glassdoor.pyx":112
  *             scores = [np.nan for _ in range(len(values_series))]
  *         else:
  *             ranks = stats.mstats.rankdata(np.ma.masked_invalid(values_series))             # <<<<<<<<<<<<<<
  *             ranks[ranks == 0] = np.nan
  *             n = ranks.size - np.count_nonzero(np.isnan(ranks))
  */
   /*else*/ {
@@ -4242,15 +4242,15 @@
     __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
     if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 112, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_1);
     __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
     __pyx_v_ranks = __pyx_t_1;
     __pyx_t_1 = 0;
 
-    /* "seleya/mfc/alchemy/qrank/glassdoor.py":113
+    /* "seleya/mfc/alchemy/qrank/glassdoor.pyx":113
  *         else:
  *             ranks = stats.mstats.rankdata(np.ma.masked_invalid(values_series))
  *             ranks[ranks == 0] = np.nan             # <<<<<<<<<<<<<<
  *             n = ranks.size - np.count_nonzero(np.isnan(ranks))
  *             scores = stats.norm.ppf((ranks - 3. / 8) / (n + 0.25))
  */
     __Pyx_GetModuleGlobalName(__pyx_t_1, __pyx_n_s_np); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 113, __pyx_L1_error)
@@ -4260,15 +4260,15 @@
     __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
     __pyx_t_1 = __Pyx_PyInt_EqObjC(__pyx_v_ranks, __pyx_int_0, 0, 0); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 113, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_1);
     if (unlikely(PyObject_SetItem(__pyx_v_ranks, __pyx_t_1, __pyx_t_3) < 0)) __PYX_ERR(0, 113, __pyx_L1_error)
     __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
     __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
 
-    /* "seleya/mfc/alchemy/qrank/glassdoor.py":114
+    /* "seleya/mfc/alchemy/qrank/glassdoor.pyx":114
  *             ranks = stats.mstats.rankdata(np.ma.masked_invalid(values_series))
  *             ranks[ranks == 0] = np.nan
  *             n = ranks.size - np.count_nonzero(np.isnan(ranks))             # <<<<<<<<<<<<<<
  *             scores = stats.norm.ppf((ranks - 3. / 8) / (n + 0.25))
  *         scores = pd.Series(data=scores, index=idx)
  */
     __pyx_t_3 = __Pyx_PyObject_GetAttrStr(__pyx_v_ranks, __pyx_n_s_size); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 114, __pyx_L1_error)
@@ -4317,15 +4317,15 @@
     __pyx_t_4 = PyNumber_Subtract(__pyx_t_3, __pyx_t_1); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 114, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_4);
     __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
     __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
     __pyx_v_n = __pyx_t_4;
     __pyx_t_4 = 0;
 
-    /* "seleya/mfc/alchemy/qrank/glassdoor.py":115
+    /* "seleya/mfc/alchemy/qrank/glassdoor.pyx":115
  *             ranks[ranks == 0] = np.nan
  *             n = ranks.size - np.count_nonzero(np.isnan(ranks))
  *             scores = stats.norm.ppf((ranks - 3. / 8) / (n + 0.25))             # <<<<<<<<<<<<<<
  *         scores = pd.Series(data=scores, index=idx)
  *         return scores
  */
     __Pyx_GetModuleGlobalName(__pyx_t_1, __pyx_n_s_stats); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 115, __pyx_L1_error)
@@ -4364,15 +4364,15 @@
     __Pyx_GOTREF(__pyx_t_4);
     __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
     __pyx_v_scores = __pyx_t_4;
     __pyx_t_4 = 0;
   }
   __pyx_L3:;
 
-  /* "seleya/mfc/alchemy/qrank/glassdoor.py":116
+  /* "seleya/mfc/alchemy/qrank/glassdoor.pyx":116
  *             n = ranks.size - np.count_nonzero(np.isnan(ranks))
  *             scores = stats.norm.ppf((ranks - 3. / 8) / (n + 0.25))
  *         scores = pd.Series(data=scores, index=idx)             # <<<<<<<<<<<<<<
  *         return scores
  * 
  */
   __Pyx_GetModuleGlobalName(__pyx_t_4, __pyx_n_s_pd); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 116, __pyx_L1_error)
@@ -4387,27 +4387,27 @@
   __pyx_t_10 = __Pyx_PyObject_Call(__pyx_t_1, __pyx_empty_tuple, __pyx_t_4); if (unlikely(!__pyx_t_10)) __PYX_ERR(0, 116, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_10);
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
   __Pyx_DECREF_SET(__pyx_v_scores, __pyx_t_10);
   __pyx_t_10 = 0;
 
-  /* "seleya/mfc/alchemy/qrank/glassdoor.py":117
+  /* "seleya/mfc/alchemy/qrank/glassdoor.pyx":117
  *             scores = stats.norm.ppf((ranks - 3. / 8) / (n + 0.25))
  *         scores = pd.Series(data=scores, index=idx)
  *         return scores             # <<<<<<<<<<<<<<
  * 
  *     def _distribute(self, mean_data):
  */
   __Pyx_XDECREF(__pyx_r);
   __Pyx_INCREF(__pyx_v_scores);
   __pyx_r = __pyx_v_scores;
   goto __pyx_L0;
 
-  /* "seleya/mfc/alchemy/qrank/glassdoor.py":106
+  /* "seleya/mfc/alchemy/qrank/glassdoor.pyx":106
  *         return raw_data
  * 
  *     def _blom_score(self, values_series, threshold=0.9):             # <<<<<<<<<<<<<<
  *         idx = values_series.index.droplevel(level=0)
  *         coverage = values_series.isna().sum() / len(values_series)
  */
 
@@ -4415,40 +4415,40 @@
   __pyx_L1_error:;
   __Pyx_XDECREF(__pyx_t_1);
   __Pyx_XDECREF(__pyx_t_2);
   __Pyx_XDECREF(__pyx_t_3);
   __Pyx_XDECREF(__pyx_t_4);
   __Pyx_XDECREF(__pyx_t_9);
   __Pyx_XDECREF(__pyx_t_10);
-  __Pyx_AddTraceback("seleya.mfc.alchemy.qrank.glassdoo.Glassdoor._blom_score", __pyx_clineno, __pyx_lineno, __pyx_filename);
+  __Pyx_AddTraceback("seleya.mfc.alchemy.qrank.glassdoor.Glassdoor._blom_score", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __pyx_r = NULL;
   __pyx_L0:;
   __Pyx_XDECREF(__pyx_v_idx);
   __Pyx_XDECREF(__pyx_v_coverage);
   __Pyx_XDECREF(__pyx_v_scores);
   __Pyx_XDECREF(__pyx_v_ranks);
   __Pyx_XDECREF(__pyx_v_n);
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "seleya/mfc/alchemy/qrank/glassdoor.py":119
+/* "seleya/mfc/alchemy/qrank/glassdoor.pyx":119
  *         return scores
  * 
  *     def _distribute(self, mean_data):             # <<<<<<<<<<<<<<
  *         dt = mean_data.set_index(['date', 'code', 'name'])['value']
  *         res = []
  */
 
 /* Python wrapper */
-static PyObject *__pyx_pw_6seleya_3mfc_7alchemy_5qrank_8glassdoo_9Glassdoor_13_distribute(PyObject *__pyx_self, PyObject *__pyx_args, PyObject *__pyx_kwds); /*proto*/
-static char __pyx_doc_6seleya_3mfc_7alchemy_5qrank_8glassdoo_9Glassdoor_12_distribute[] = "Glassdoor._distribute(self, mean_data)";
-static PyMethodDef __pyx_mdef_6seleya_3mfc_7alchemy_5qrank_8glassdoo_9Glassdoor_13_distribute = {"_distribute", (PyCFunction)(void*)(PyCFunctionWithKeywords)__pyx_pw_6seleya_3mfc_7alchemy_5qrank_8glassdoo_9Glassdoor_13_distribute, METH_VARARGS|METH_KEYWORDS, __pyx_doc_6seleya_3mfc_7alchemy_5qrank_8glassdoo_9Glassdoor_12_distribute};
-static PyObject *__pyx_pw_6seleya_3mfc_7alchemy_5qrank_8glassdoo_9Glassdoor_13_distribute(PyObject *__pyx_self, PyObject *__pyx_args, PyObject *__pyx_kwds) {
+static PyObject *__pyx_pw_6seleya_3mfc_7alchemy_5qrank_9glassdoor_9Glassdoor_13_distribute(PyObject *__pyx_self, PyObject *__pyx_args, PyObject *__pyx_kwds); /*proto*/
+static char __pyx_doc_6seleya_3mfc_7alchemy_5qrank_9glassdoor_9Glassdoor_12_distribute[] = "Glassdoor._distribute(self, mean_data)";
+static PyMethodDef __pyx_mdef_6seleya_3mfc_7alchemy_5qrank_9glassdoor_9Glassdoor_13_distribute = {"_distribute", (PyCFunction)(void*)(PyCFunctionWithKeywords)__pyx_pw_6seleya_3mfc_7alchemy_5qrank_9glassdoor_9Glassdoor_13_distribute, METH_VARARGS|METH_KEYWORDS, __pyx_doc_6seleya_3mfc_7alchemy_5qrank_9glassdoor_9Glassdoor_12_distribute};
+static PyObject *__pyx_pw_6seleya_3mfc_7alchemy_5qrank_9glassdoor_9Glassdoor_13_distribute(PyObject *__pyx_self, PyObject *__pyx_args, PyObject *__pyx_kwds) {
   PyObject *__pyx_v_self = 0;
   PyObject *__pyx_v_mean_data = 0;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   PyObject *__pyx_r = 0;
   __Pyx_RefNannyDeclarations
@@ -4491,62 +4491,62 @@
     __pyx_v_self = values[0];
     __pyx_v_mean_data = values[1];
   }
   goto __pyx_L4_argument_unpacking_done;
   __pyx_L5_argtuple_error:;
   __Pyx_RaiseArgtupleInvalid("_distribute", 1, 2, 2, PyTuple_GET_SIZE(__pyx_args)); __PYX_ERR(0, 119, __pyx_L3_error)
   __pyx_L3_error:;
-  __Pyx_AddTraceback("seleya.mfc.alchemy.qrank.glassdoo.Glassdoor._distribute", __pyx_clineno, __pyx_lineno, __pyx_filename);
+  __Pyx_AddTraceback("seleya.mfc.alchemy.qrank.glassdoor.Glassdoor._distribute", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __Pyx_RefNannyFinishContext();
   return NULL;
   __pyx_L4_argument_unpacking_done:;
-  __pyx_r = __pyx_pf_6seleya_3mfc_7alchemy_5qrank_8glassdoo_9Glassdoor_12_distribute(__pyx_self, __pyx_v_self, __pyx_v_mean_data);
+  __pyx_r = __pyx_pf_6seleya_3mfc_7alchemy_5qrank_9glassdoor_9Glassdoor_12_distribute(__pyx_self, __pyx_v_self, __pyx_v_mean_data);
 
   /* function exit code */
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "seleya/mfc/alchemy/qrank/glassdoor.py":122
+/* "seleya/mfc/alchemy/qrank/glassdoor.pyx":122
  *         dt = mean_data.set_index(['date', 'code', 'name'])['value']
  *         res = []
  *         _ = dt.unstack().apply(lambda x: self._percentile(x, res), axis=0)             # <<<<<<<<<<<<<<
  *         dt = pd.concat(res, axis=1)
  *         dt['industry'] = self._industry_code
  */
 
 /* Python wrapper */
-static PyObject *__pyx_pw_6seleya_3mfc_7alchemy_5qrank_8glassdoo_9Glassdoor_11_distribute_lambda1(PyObject *__pyx_self, PyObject *__pyx_v_x); /*proto*/
-static PyMethodDef __pyx_mdef_6seleya_3mfc_7alchemy_5qrank_8glassdoo_9Glassdoor_11_distribute_lambda1 = {"lambda1", (PyCFunction)__pyx_pw_6seleya_3mfc_7alchemy_5qrank_8glassdoo_9Glassdoor_11_distribute_lambda1, METH_O, 0};
-static PyObject *__pyx_pw_6seleya_3mfc_7alchemy_5qrank_8glassdoo_9Glassdoor_11_distribute_lambda1(PyObject *__pyx_self, PyObject *__pyx_v_x) {
+static PyObject *__pyx_pw_6seleya_3mfc_7alchemy_5qrank_9glassdoor_9Glassdoor_11_distribute_lambda1(PyObject *__pyx_self, PyObject *__pyx_v_x); /*proto*/
+static PyMethodDef __pyx_mdef_6seleya_3mfc_7alchemy_5qrank_9glassdoor_9Glassdoor_11_distribute_lambda1 = {"lambda1", (PyCFunction)__pyx_pw_6seleya_3mfc_7alchemy_5qrank_9glassdoor_9Glassdoor_11_distribute_lambda1, METH_O, 0};
+static PyObject *__pyx_pw_6seleya_3mfc_7alchemy_5qrank_9glassdoor_9Glassdoor_11_distribute_lambda1(PyObject *__pyx_self, PyObject *__pyx_v_x) {
   PyObject *__pyx_r = 0;
   __Pyx_RefNannyDeclarations
   __Pyx_RefNannySetupContext("lambda1 (wrapper)", 0);
   __pyx_r = __pyx_lambda_funcdef_lambda1(__pyx_self, ((PyObject *)__pyx_v_x));
 
   /* function exit code */
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
 static PyObject *__pyx_lambda_funcdef_lambda1(PyObject *__pyx_self, PyObject *__pyx_v_x) {
-  struct __pyx_obj_6seleya_3mfc_7alchemy_5qrank_8glassdoo___pyx_scope_struct_1__distribute *__pyx_cur_scope;
-  struct __pyx_obj_6seleya_3mfc_7alchemy_5qrank_8glassdoo___pyx_scope_struct_1__distribute *__pyx_outer_scope;
+  struct __pyx_obj_6seleya_3mfc_7alchemy_5qrank_9glassdoor___pyx_scope_struct_1__distribute *__pyx_cur_scope;
+  struct __pyx_obj_6seleya_3mfc_7alchemy_5qrank_9glassdoor___pyx_scope_struct_1__distribute *__pyx_outer_scope;
   PyObject *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   PyObject *__pyx_t_2 = NULL;
   PyObject *__pyx_t_3 = NULL;
   int __pyx_t_4;
   PyObject *__pyx_t_5 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("lambda1", 0);
-  __pyx_outer_scope = (struct __pyx_obj_6seleya_3mfc_7alchemy_5qrank_8glassdoo___pyx_scope_struct_1__distribute *) __Pyx_CyFunction_GetClosure(__pyx_self);
+  __pyx_outer_scope = (struct __pyx_obj_6seleya_3mfc_7alchemy_5qrank_9glassdoor___pyx_scope_struct_1__distribute *) __Pyx_CyFunction_GetClosure(__pyx_self);
   __pyx_cur_scope = __pyx_outer_scope;
   __Pyx_XDECREF(__pyx_r);
   if (unlikely(!__pyx_cur_scope->__pyx_v_self)) { __Pyx_RaiseClosureNameError("self"); __PYX_ERR(0, 122, __pyx_L1_error) }
   __pyx_t_2 = __Pyx_PyObject_GetAttrStr(__pyx_cur_scope->__pyx_v_self, __pyx_n_s_percentile); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 122, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   if (unlikely(!__pyx_cur_scope->__pyx_v_res)) { __Pyx_RaiseClosureNameError("res"); __PYX_ERR(0, 122, __pyx_L1_error) }
   __pyx_t_3 = NULL;
@@ -4600,57 +4600,57 @@
 
   /* function exit code */
   __pyx_L1_error:;
   __Pyx_XDECREF(__pyx_t_1);
   __Pyx_XDECREF(__pyx_t_2);
   __Pyx_XDECREF(__pyx_t_3);
   __Pyx_XDECREF(__pyx_t_5);
-  __Pyx_AddTraceback("seleya.mfc.alchemy.qrank.glassdoo.Glassdoor._distribute.lambda1", __pyx_clineno, __pyx_lineno, __pyx_filename);
+  __Pyx_AddTraceback("seleya.mfc.alchemy.qrank.glassdoor.Glassdoor._distribute.lambda1", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __pyx_r = NULL;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "seleya/mfc/alchemy/qrank/glassdoor.py":119
+/* "seleya/mfc/alchemy/qrank/glassdoor.pyx":119
  *         return scores
  * 
  *     def _distribute(self, mean_data):             # <<<<<<<<<<<<<<
  *         dt = mean_data.set_index(['date', 'code', 'name'])['value']
  *         res = []
  */
 
-static PyObject *__pyx_pf_6seleya_3mfc_7alchemy_5qrank_8glassdoo_9Glassdoor_12_distribute(CYTHON_UNUSED PyObject *__pyx_self, PyObject *__pyx_v_self, PyObject *__pyx_v_mean_data) {
-  struct __pyx_obj_6seleya_3mfc_7alchemy_5qrank_8glassdoo___pyx_scope_struct_1__distribute *__pyx_cur_scope;
+static PyObject *__pyx_pf_6seleya_3mfc_7alchemy_5qrank_9glassdoor_9Glassdoor_12_distribute(CYTHON_UNUSED PyObject *__pyx_self, PyObject *__pyx_v_self, PyObject *__pyx_v_mean_data) {
+  struct __pyx_obj_6seleya_3mfc_7alchemy_5qrank_9glassdoor___pyx_scope_struct_1__distribute *__pyx_cur_scope;
   PyObject *__pyx_v_dt = NULL;
   CYTHON_UNUSED PyObject *__pyx_v__ = NULL;
   PyObject *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   PyObject *__pyx_t_2 = NULL;
   PyObject *__pyx_t_3 = NULL;
   PyObject *__pyx_t_4 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("_distribute", 0);
-  __pyx_cur_scope = (struct __pyx_obj_6seleya_3mfc_7alchemy_5qrank_8glassdoo___pyx_scope_struct_1__distribute *)__pyx_tp_new_6seleya_3mfc_7alchemy_5qrank_8glassdoo___pyx_scope_struct_1__distribute(__pyx_ptype_6seleya_3mfc_7alchemy_5qrank_8glassdoo___pyx_scope_struct_1__distribute, __pyx_empty_tuple, NULL);
+  __pyx_cur_scope = (struct __pyx_obj_6seleya_3mfc_7alchemy_5qrank_9glassdoor___pyx_scope_struct_1__distribute *)__pyx_tp_new_6seleya_3mfc_7alchemy_5qrank_9glassdoor___pyx_scope_struct_1__distribute(__pyx_ptype_6seleya_3mfc_7alchemy_5qrank_9glassdoor___pyx_scope_struct_1__distribute, __pyx_empty_tuple, NULL);
   if (unlikely(!__pyx_cur_scope)) {
-    __pyx_cur_scope = ((struct __pyx_obj_6seleya_3mfc_7alchemy_5qrank_8glassdoo___pyx_scope_struct_1__distribute *)Py_None);
+    __pyx_cur_scope = ((struct __pyx_obj_6seleya_3mfc_7alchemy_5qrank_9glassdoor___pyx_scope_struct_1__distribute *)Py_None);
     __Pyx_INCREF(Py_None);
     __PYX_ERR(0, 119, __pyx_L1_error)
   } else {
     __Pyx_GOTREF(__pyx_cur_scope);
   }
   __pyx_cur_scope->__pyx_v_self = __pyx_v_self;
   __Pyx_INCREF(__pyx_cur_scope->__pyx_v_self);
   __Pyx_GIVEREF(__pyx_cur_scope->__pyx_v_self);
 
-  /* "seleya/mfc/alchemy/qrank/glassdoor.py":120
+  /* "seleya/mfc/alchemy/qrank/glassdoor.pyx":120
  * 
  *     def _distribute(self, mean_data):
  *         dt = mean_data.set_index(['date', 'code', 'name'])['value']             # <<<<<<<<<<<<<<
  *         res = []
  *         _ = dt.unstack().apply(lambda x: self._percentile(x, res), axis=0)
  */
   __pyx_t_2 = __Pyx_PyObject_GetAttrStr(__pyx_v_mean_data, __pyx_n_s_set_index); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 120, __pyx_L1_error)
@@ -4684,28 +4684,28 @@
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
   __pyx_t_2 = __Pyx_PyObject_Dict_GetItem(__pyx_t_1, __pyx_n_s_value); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 120, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   __pyx_v_dt = __pyx_t_2;
   __pyx_t_2 = 0;
 
-  /* "seleya/mfc/alchemy/qrank/glassdoor.py":121
+  /* "seleya/mfc/alchemy/qrank/glassdoor.pyx":121
  *     def _distribute(self, mean_data):
  *         dt = mean_data.set_index(['date', 'code', 'name'])['value']
  *         res = []             # <<<<<<<<<<<<<<
  *         _ = dt.unstack().apply(lambda x: self._percentile(x, res), axis=0)
  *         dt = pd.concat(res, axis=1)
  */
   __pyx_t_2 = PyList_New(0); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 121, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   __Pyx_GIVEREF(__pyx_t_2);
   __pyx_cur_scope->__pyx_v_res = ((PyObject*)__pyx_t_2);
   __pyx_t_2 = 0;
 
-  /* "seleya/mfc/alchemy/qrank/glassdoor.py":122
+  /* "seleya/mfc/alchemy/qrank/glassdoor.pyx":122
  *         dt = mean_data.set_index(['date', 'code', 'name'])['value']
  *         res = []
  *         _ = dt.unstack().apply(lambda x: self._percentile(x, res), axis=0)             # <<<<<<<<<<<<<<
  *         dt = pd.concat(res, axis=1)
  *         dt['industry'] = self._industry_code
  */
   __pyx_t_1 = __Pyx_PyObject_GetAttrStr(__pyx_v_dt, __pyx_n_s_unstack); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 122, __pyx_L1_error)
@@ -4724,15 +4724,15 @@
   __Pyx_XDECREF(__pyx_t_3); __pyx_t_3 = 0;
   if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 122, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   __pyx_t_1 = __Pyx_PyObject_GetAttrStr(__pyx_t_2, __pyx_n_s_apply); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 122, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
-  __pyx_t_2 = __Pyx_CyFunction_New(&__pyx_mdef_6seleya_3mfc_7alchemy_5qrank_8glassdoo_9Glassdoor_11_distribute_lambda1, 0, __pyx_n_s_Glassdoor__distribute_locals_lam, ((PyObject*)__pyx_cur_scope), __pyx_n_s_seleya_mfc_alchemy_qrank_glassdo, __pyx_d, NULL); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 122, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_CyFunction_New(&__pyx_mdef_6seleya_3mfc_7alchemy_5qrank_9glassdoor_9Glassdoor_11_distribute_lambda1, 0, __pyx_n_s_Glassdoor__distribute_locals_lam, ((PyObject*)__pyx_cur_scope), __pyx_n_s_seleya_mfc_alchemy_qrank_glassdo, __pyx_d, NULL); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 122, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   __pyx_t_3 = PyTuple_New(1); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 122, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
   __Pyx_GIVEREF(__pyx_t_2);
   PyTuple_SET_ITEM(__pyx_t_3, 0, __pyx_t_2);
   __pyx_t_2 = 0;
   __pyx_t_2 = __Pyx_PyDict_NewPresized(1); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 122, __pyx_L1_error)
@@ -4742,15 +4742,15 @@
   __Pyx_GOTREF(__pyx_t_4);
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
   __pyx_v__ = __pyx_t_4;
   __pyx_t_4 = 0;
 
-  /* "seleya/mfc/alchemy/qrank/glassdoor.py":123
+  /* "seleya/mfc/alchemy/qrank/glassdoor.pyx":123
  *         res = []
  *         _ = dt.unstack().apply(lambda x: self._percentile(x, res), axis=0)
  *         dt = pd.concat(res, axis=1)             # <<<<<<<<<<<<<<
  *         dt['industry'] = self._industry_code
  *         return dt
  */
   __Pyx_GetModuleGlobalName(__pyx_t_4, __pyx_n_s_pd); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 123, __pyx_L1_error)
@@ -4770,76 +4770,76 @@
   __Pyx_GOTREF(__pyx_t_1);
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
   __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
   __Pyx_DECREF_SET(__pyx_v_dt, __pyx_t_1);
   __pyx_t_1 = 0;
 
-  /* "seleya/mfc/alchemy/qrank/glassdoor.py":124
+  /* "seleya/mfc/alchemy/qrank/glassdoor.pyx":124
  *         _ = dt.unstack().apply(lambda x: self._percentile(x, res), axis=0)
  *         dt = pd.concat(res, axis=1)
  *         dt['industry'] = self._industry_code             # <<<<<<<<<<<<<<
  *         return dt
  * 
  */
   __pyx_t_1 = __Pyx_PyObject_GetAttrStr(__pyx_cur_scope->__pyx_v_self, __pyx_n_s_industry_code_2); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 124, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   if (unlikely(PyObject_SetItem(__pyx_v_dt, __pyx_n_s_industry, __pyx_t_1) < 0)) __PYX_ERR(0, 124, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
 
-  /* "seleya/mfc/alchemy/qrank/glassdoor.py":125
+  /* "seleya/mfc/alchemy/qrank/glassdoor.pyx":125
  *         dt = pd.concat(res, axis=1)
  *         dt['industry'] = self._industry_code
  *         return dt             # <<<<<<<<<<<<<<
  * 
  *     def _percentile(self, x, res):
  */
   __Pyx_XDECREF(__pyx_r);
   __Pyx_INCREF(__pyx_v_dt);
   __pyx_r = __pyx_v_dt;
   goto __pyx_L0;
 
-  /* "seleya/mfc/alchemy/qrank/glassdoor.py":119
+  /* "seleya/mfc/alchemy/qrank/glassdoor.pyx":119
  *         return scores
  * 
  *     def _distribute(self, mean_data):             # <<<<<<<<<<<<<<
  *         dt = mean_data.set_index(['date', 'code', 'name'])['value']
  *         res = []
  */
 
   /* function exit code */
   __pyx_L1_error:;
   __Pyx_XDECREF(__pyx_t_1);
   __Pyx_XDECREF(__pyx_t_2);
   __Pyx_XDECREF(__pyx_t_3);
   __Pyx_XDECREF(__pyx_t_4);
-  __Pyx_AddTraceback("seleya.mfc.alchemy.qrank.glassdoo.Glassdoor._distribute", __pyx_clineno, __pyx_lineno, __pyx_filename);
+  __Pyx_AddTraceback("seleya.mfc.alchemy.qrank.glassdoor.Glassdoor._distribute", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __pyx_r = NULL;
   __pyx_L0:;
   __Pyx_XDECREF(__pyx_v_dt);
   __Pyx_XDECREF(__pyx_v__);
   __Pyx_DECREF(((PyObject *)__pyx_cur_scope));
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "seleya/mfc/alchemy/qrank/glassdoor.py":127
+/* "seleya/mfc/alchemy/qrank/glassdoor.pyx":127
  *         return dt
  * 
  *     def _percentile(self, x, res):             # <<<<<<<<<<<<<<
  *         name = str(x.name)
  *         x = x.dropna()
  */
 
 /* Python wrapper */
-static PyObject *__pyx_pw_6seleya_3mfc_7alchemy_5qrank_8glassdoo_9Glassdoor_15_percentile(PyObject *__pyx_self, PyObject *__pyx_args, PyObject *__pyx_kwds); /*proto*/
-static char __pyx_doc_6seleya_3mfc_7alchemy_5qrank_8glassdoo_9Glassdoor_14_percentile[] = "Glassdoor._percentile(self, x, res)";
-static PyMethodDef __pyx_mdef_6seleya_3mfc_7alchemy_5qrank_8glassdoo_9Glassdoor_15_percentile = {"_percentile", (PyCFunction)(void*)(PyCFunctionWithKeywords)__pyx_pw_6seleya_3mfc_7alchemy_5qrank_8glassdoo_9Glassdoor_15_percentile, METH_VARARGS|METH_KEYWORDS, __pyx_doc_6seleya_3mfc_7alchemy_5qrank_8glassdoo_9Glassdoor_14_percentile};
-static PyObject *__pyx_pw_6seleya_3mfc_7alchemy_5qrank_8glassdoo_9Glassdoor_15_percentile(PyObject *__pyx_self, PyObject *__pyx_args, PyObject *__pyx_kwds) {
+static PyObject *__pyx_pw_6seleya_3mfc_7alchemy_5qrank_9glassdoor_9Glassdoor_15_percentile(PyObject *__pyx_self, PyObject *__pyx_args, PyObject *__pyx_kwds); /*proto*/
+static char __pyx_doc_6seleya_3mfc_7alchemy_5qrank_9glassdoor_9Glassdoor_14_percentile[] = "Glassdoor._percentile(self, x, res)";
+static PyMethodDef __pyx_mdef_6seleya_3mfc_7alchemy_5qrank_9glassdoor_9Glassdoor_15_percentile = {"_percentile", (PyCFunction)(void*)(PyCFunctionWithKeywords)__pyx_pw_6seleya_3mfc_7alchemy_5qrank_9glassdoor_9Glassdoor_15_percentile, METH_VARARGS|METH_KEYWORDS, __pyx_doc_6seleya_3mfc_7alchemy_5qrank_9glassdoor_9Glassdoor_14_percentile};
+static PyObject *__pyx_pw_6seleya_3mfc_7alchemy_5qrank_9glassdoor_9Glassdoor_15_percentile(PyObject *__pyx_self, PyObject *__pyx_args, PyObject *__pyx_kwds) {
   CYTHON_UNUSED PyObject *__pyx_v_self = 0;
   PyObject *__pyx_v_x = 0;
   PyObject *__pyx_v_res = 0;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   PyObject *__pyx_r = 0;
@@ -4893,26 +4893,26 @@
     __pyx_v_x = values[1];
     __pyx_v_res = values[2];
   }
   goto __pyx_L4_argument_unpacking_done;
   __pyx_L5_argtuple_error:;
   __Pyx_RaiseArgtupleInvalid("_percentile", 1, 3, 3, PyTuple_GET_SIZE(__pyx_args)); __PYX_ERR(0, 127, __pyx_L3_error)
   __pyx_L3_error:;
-  __Pyx_AddTraceback("seleya.mfc.alchemy.qrank.glassdoo.Glassdoor._percentile", __pyx_clineno, __pyx_lineno, __pyx_filename);
+  __Pyx_AddTraceback("seleya.mfc.alchemy.qrank.glassdoor.Glassdoor._percentile", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __Pyx_RefNannyFinishContext();
   return NULL;
   __pyx_L4_argument_unpacking_done:;
-  __pyx_r = __pyx_pf_6seleya_3mfc_7alchemy_5qrank_8glassdoo_9Glassdoor_14_percentile(__pyx_self, __pyx_v_self, __pyx_v_x, __pyx_v_res);
+  __pyx_r = __pyx_pf_6seleya_3mfc_7alchemy_5qrank_9glassdoor_9Glassdoor_14_percentile(__pyx_self, __pyx_v_self, __pyx_v_x, __pyx_v_res);
 
   /* function exit code */
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-static PyObject *__pyx_pf_6seleya_3mfc_7alchemy_5qrank_8glassdoo_9Glassdoor_14_percentile(CYTHON_UNUSED PyObject *__pyx_self, CYTHON_UNUSED PyObject *__pyx_v_self, PyObject *__pyx_v_x, PyObject *__pyx_v_res) {
+static PyObject *__pyx_pf_6seleya_3mfc_7alchemy_5qrank_9glassdoor_9Glassdoor_14_percentile(CYTHON_UNUSED PyObject *__pyx_self, CYTHON_UNUSED PyObject *__pyx_v_self, PyObject *__pyx_v_x, PyObject *__pyx_v_res) {
   PyObject *__pyx_v_name = NULL;
   PyObject *__pyx_v_rt = NULL;
   PyObject *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   PyObject *__pyx_t_2 = NULL;
   PyObject *__pyx_t_3 = NULL;
@@ -4921,30 +4921,30 @@
   int __pyx_t_6;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("_percentile", 0);
   __Pyx_INCREF(__pyx_v_x);
 
-  /* "seleya/mfc/alchemy/qrank/glassdoor.py":128
+  /* "seleya/mfc/alchemy/qrank/glassdoor.pyx":128
  * 
  *     def _percentile(self, x, res):
  *         name = str(x.name)             # <<<<<<<<<<<<<<
  *         x = x.dropna()
  *         rt = CSQuantiles(name).transform(x.reset_index().set_index('date'),
  */
   __pyx_t_1 = __Pyx_PyObject_GetAttrStr(__pyx_v_x, __pyx_n_s_name); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 128, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_t_2 = __Pyx_PyObject_CallOneArg(((PyObject *)(&PyString_Type)), __pyx_t_1); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 128, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   __pyx_v_name = __pyx_t_2;
   __pyx_t_2 = 0;
 
-  /* "seleya/mfc/alchemy/qrank/glassdoor.py":129
+  /* "seleya/mfc/alchemy/qrank/glassdoor.pyx":129
  *     def _percentile(self, x, res):
  *         name = str(x.name)
  *         x = x.dropna()             # <<<<<<<<<<<<<<
  *         rt = CSQuantiles(name).transform(x.reset_index().set_index('date'),
  *                                          name=name,
  */
   __pyx_t_1 = __Pyx_PyObject_GetAttrStr(__pyx_v_x, __pyx_n_s_dropna); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 129, __pyx_L1_error)
@@ -4963,15 +4963,15 @@
   __Pyx_XDECREF(__pyx_t_3); __pyx_t_3 = 0;
   if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 129, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   __Pyx_DECREF_SET(__pyx_v_x, __pyx_t_2);
   __pyx_t_2 = 0;
 
-  /* "seleya/mfc/alchemy/qrank/glassdoor.py":130
+  /* "seleya/mfc/alchemy/qrank/glassdoor.pyx":130
  *         name = str(x.name)
  *         x = x.dropna()
  *         rt = CSQuantiles(name).transform(x.reset_index().set_index('date'),             # <<<<<<<<<<<<<<
  *                                          name=name,
  *                                          category_field='code')
  */
   __Pyx_GetModuleGlobalName(__pyx_t_1, __pyx_n_s_CSQuantiles); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 130, __pyx_L1_error)
@@ -5031,42 +5031,42 @@
   __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
   __pyx_t_4 = PyTuple_New(1); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 130, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_4);
   __Pyx_GIVEREF(__pyx_t_2);
   PyTuple_SET_ITEM(__pyx_t_4, 0, __pyx_t_2);
   __pyx_t_2 = 0;
 
-  /* "seleya/mfc/alchemy/qrank/glassdoor.py":131
+  /* "seleya/mfc/alchemy/qrank/glassdoor.pyx":131
  *         x = x.dropna()
  *         rt = CSQuantiles(name).transform(x.reset_index().set_index('date'),
  *                                          name=name,             # <<<<<<<<<<<<<<
  *                                          category_field='code')
  *         res.append(rt.reset_index().set_index(['date', 'code']))
  */
   __pyx_t_2 = __Pyx_PyDict_NewPresized(2); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 131, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   if (PyDict_SetItem(__pyx_t_2, __pyx_n_s_name, __pyx_v_name) < 0) __PYX_ERR(0, 131, __pyx_L1_error)
   if (PyDict_SetItem(__pyx_t_2, __pyx_n_s_category_field, __pyx_n_s_code) < 0) __PYX_ERR(0, 131, __pyx_L1_error)
 
-  /* "seleya/mfc/alchemy/qrank/glassdoor.py":130
+  /* "seleya/mfc/alchemy/qrank/glassdoor.pyx":130
  *         name = str(x.name)
  *         x = x.dropna()
  *         rt = CSQuantiles(name).transform(x.reset_index().set_index('date'),             # <<<<<<<<<<<<<<
  *                                          name=name,
  *                                          category_field='code')
  */
   __pyx_t_3 = __Pyx_PyObject_Call(__pyx_t_1, __pyx_t_4, __pyx_t_2); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 130, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
   __pyx_v_rt = __pyx_t_3;
   __pyx_t_3 = 0;
 
-  /* "seleya/mfc/alchemy/qrank/glassdoor.py":133
+  /* "seleya/mfc/alchemy/qrank/glassdoor.pyx":133
  *                                          name=name,
  *                                          category_field='code')
  *         res.append(rt.reset_index().set_index(['date', 'code']))             # <<<<<<<<<<<<<<
  * 
  *     def _calculate_distribute(self, mean_data):
  */
   __pyx_t_4 = __Pyx_PyObject_GetAttrStr(__pyx_v_rt, __pyx_n_s_reset_index); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 133, __pyx_L1_error)
@@ -5112,15 +5112,15 @@
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
   if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 133, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
   __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
   __pyx_t_6 = __Pyx_PyObject_Append(__pyx_v_res, __pyx_t_3); if (unlikely(__pyx_t_6 == ((int)-1))) __PYX_ERR(0, 133, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
 
-  /* "seleya/mfc/alchemy/qrank/glassdoor.py":127
+  /* "seleya/mfc/alchemy/qrank/glassdoor.pyx":127
  *         return dt
  * 
  *     def _percentile(self, x, res):             # <<<<<<<<<<<<<<
  *         name = str(x.name)
  *         x = x.dropna()
  */
 
@@ -5129,38 +5129,38 @@
   goto __pyx_L0;
   __pyx_L1_error:;
   __Pyx_XDECREF(__pyx_t_1);
   __Pyx_XDECREF(__pyx_t_2);
   __Pyx_XDECREF(__pyx_t_3);
   __Pyx_XDECREF(__pyx_t_4);
   __Pyx_XDECREF(__pyx_t_5);
-  __Pyx_AddTraceback("seleya.mfc.alchemy.qrank.glassdoo.Glassdoor._percentile", __pyx_clineno, __pyx_lineno, __pyx_filename);
+  __Pyx_AddTraceback("seleya.mfc.alchemy.qrank.glassdoor.Glassdoor._percentile", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __pyx_r = NULL;
   __pyx_L0:;
   __Pyx_XDECREF(__pyx_v_name);
   __Pyx_XDECREF(__pyx_v_rt);
   __Pyx_XDECREF(__pyx_v_x);
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "seleya/mfc/alchemy/qrank/glassdoor.py":135
+/* "seleya/mfc/alchemy/qrank/glassdoor.pyx":135
  *         res.append(rt.reset_index().set_index(['date', 'code']))
  * 
  *     def _calculate_distribute(self, mean_data):             # <<<<<<<<<<<<<<
  *         kd_logger.info('calculating distribute...')
  *         mean_data['date'] = pd.to_datetime(mean_data['date'])
  */
 
 /* Python wrapper */
-static PyObject *__pyx_pw_6seleya_3mfc_7alchemy_5qrank_8glassdoo_9Glassdoor_17_calculate_distribute(PyObject *__pyx_self, PyObject *__pyx_args, PyObject *__pyx_kwds); /*proto*/
-static char __pyx_doc_6seleya_3mfc_7alchemy_5qrank_8glassdoo_9Glassdoor_16_calculate_distribute[] = "Glassdoor._calculate_distribute(self, mean_data)";
-static PyMethodDef __pyx_mdef_6seleya_3mfc_7alchemy_5qrank_8glassdoo_9Glassdoor_17_calculate_distribute = {"_calculate_distribute", (PyCFunction)(void*)(PyCFunctionWithKeywords)__pyx_pw_6seleya_3mfc_7alchemy_5qrank_8glassdoo_9Glassdoor_17_calculate_distribute, METH_VARARGS|METH_KEYWORDS, __pyx_doc_6seleya_3mfc_7alchemy_5qrank_8glassdoo_9Glassdoor_16_calculate_distribute};
-static PyObject *__pyx_pw_6seleya_3mfc_7alchemy_5qrank_8glassdoo_9Glassdoor_17_calculate_distribute(PyObject *__pyx_self, PyObject *__pyx_args, PyObject *__pyx_kwds) {
+static PyObject *__pyx_pw_6seleya_3mfc_7alchemy_5qrank_9glassdoor_9Glassdoor_17_calculate_distribute(PyObject *__pyx_self, PyObject *__pyx_args, PyObject *__pyx_kwds); /*proto*/
+static char __pyx_doc_6seleya_3mfc_7alchemy_5qrank_9glassdoor_9Glassdoor_16_calculate_distribute[] = "Glassdoor._calculate_distribute(self, mean_data)";
+static PyMethodDef __pyx_mdef_6seleya_3mfc_7alchemy_5qrank_9glassdoor_9Glassdoor_17_calculate_distribute = {"_calculate_distribute", (PyCFunction)(void*)(PyCFunctionWithKeywords)__pyx_pw_6seleya_3mfc_7alchemy_5qrank_9glassdoor_9Glassdoor_17_calculate_distribute, METH_VARARGS|METH_KEYWORDS, __pyx_doc_6seleya_3mfc_7alchemy_5qrank_9glassdoor_9Glassdoor_16_calculate_distribute};
+static PyObject *__pyx_pw_6seleya_3mfc_7alchemy_5qrank_9glassdoor_9Glassdoor_17_calculate_distribute(PyObject *__pyx_self, PyObject *__pyx_args, PyObject *__pyx_kwds) {
   PyObject *__pyx_v_self = 0;
   PyObject *__pyx_v_mean_data = 0;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   PyObject *__pyx_r = 0;
   __Pyx_RefNannyDeclarations
@@ -5203,26 +5203,26 @@
     __pyx_v_self = values[0];
     __pyx_v_mean_data = values[1];
   }
   goto __pyx_L4_argument_unpacking_done;
   __pyx_L5_argtuple_error:;
   __Pyx_RaiseArgtupleInvalid("_calculate_distribute", 1, 2, 2, PyTuple_GET_SIZE(__pyx_args)); __PYX_ERR(0, 135, __pyx_L3_error)
   __pyx_L3_error:;
-  __Pyx_AddTraceback("seleya.mfc.alchemy.qrank.glassdoo.Glassdoor._calculate_distribute", __pyx_clineno, __pyx_lineno, __pyx_filename);
+  __Pyx_AddTraceback("seleya.mfc.alchemy.qrank.glassdoor.Glassdoor._calculate_distribute", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __Pyx_RefNannyFinishContext();
   return NULL;
   __pyx_L4_argument_unpacking_done:;
-  __pyx_r = __pyx_pf_6seleya_3mfc_7alchemy_5qrank_8glassdoo_9Glassdoor_16_calculate_distribute(__pyx_self, __pyx_v_self, __pyx_v_mean_data);
+  __pyx_r = __pyx_pf_6seleya_3mfc_7alchemy_5qrank_9glassdoor_9Glassdoor_16_calculate_distribute(__pyx_self, __pyx_v_self, __pyx_v_mean_data);
 
   /* function exit code */
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-static PyObject *__pyx_pf_6seleya_3mfc_7alchemy_5qrank_8glassdoo_9Glassdoor_16_calculate_distribute(CYTHON_UNUSED PyObject *__pyx_self, PyObject *__pyx_v_self, PyObject *__pyx_v_mean_data) {
+static PyObject *__pyx_pf_6seleya_3mfc_7alchemy_5qrank_9glassdoor_9Glassdoor_16_calculate_distribute(CYTHON_UNUSED PyObject *__pyx_self, PyObject *__pyx_v_self, PyObject *__pyx_v_mean_data) {
   PyObject *__pyx_v_dist_data = NULL;
   PyObject *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   PyObject *__pyx_t_2 = NULL;
   PyObject *__pyx_t_3 = NULL;
   PyObject *__pyx_t_4 = NULL;
@@ -5232,15 +5232,15 @@
   PyObject *__pyx_t_8 = NULL;
   PyObject *__pyx_t_9 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("_calculate_distribute", 0);
 
-  /* "seleya/mfc/alchemy/qrank/glassdoor.py":136
+  /* "seleya/mfc/alchemy/qrank/glassdoor.pyx":136
  * 
  *     def _calculate_distribute(self, mean_data):
  *         kd_logger.info('calculating distribute...')             # <<<<<<<<<<<<<<
  *         mean_data['date'] = pd.to_datetime(mean_data['date'])
  *         dist_data = self._distribute(mean_data=mean_data)
  */
   __Pyx_GetModuleGlobalName(__pyx_t_2, __pyx_n_s_kd_logger); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 136, __pyx_L1_error)
@@ -5261,15 +5261,15 @@
   __pyx_t_1 = (__pyx_t_2) ? __Pyx_PyObject_Call2Args(__pyx_t_3, __pyx_t_2, __pyx_kp_s_calculating_distribute) : __Pyx_PyObject_CallOneArg(__pyx_t_3, __pyx_kp_s_calculating_distribute);
   __Pyx_XDECREF(__pyx_t_2); __pyx_t_2 = 0;
   if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 136, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
 
-  /* "seleya/mfc/alchemy/qrank/glassdoor.py":137
+  /* "seleya/mfc/alchemy/qrank/glassdoor.pyx":137
  *     def _calculate_distribute(self, mean_data):
  *         kd_logger.info('calculating distribute...')
  *         mean_data['date'] = pd.to_datetime(mean_data['date'])             # <<<<<<<<<<<<<<
  *         dist_data = self._distribute(mean_data=mean_data)
  *         if dist_data is None or dist_data.empty:
  */
   __Pyx_GetModuleGlobalName(__pyx_t_3, __pyx_n_s_pd); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 137, __pyx_L1_error)
@@ -5294,15 +5294,15 @@
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
   if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 137, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
   if (unlikely(PyObject_SetItem(__pyx_v_mean_data, __pyx_n_s_date, __pyx_t_1) < 0)) __PYX_ERR(0, 137, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
 
-  /* "seleya/mfc/alchemy/qrank/glassdoor.py":138
+  /* "seleya/mfc/alchemy/qrank/glassdoor.pyx":138
  *         kd_logger.info('calculating distribute...')
  *         mean_data['date'] = pd.to_datetime(mean_data['date'])
  *         dist_data = self._distribute(mean_data=mean_data)             # <<<<<<<<<<<<<<
  *         if dist_data is None or dist_data.empty:
  *             kd_logger.error('distribute data is empty')
  */
   __pyx_t_1 = __Pyx_PyObject_GetAttrStr(__pyx_v_self, __pyx_n_s_distribute); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 138, __pyx_L1_error)
@@ -5313,15 +5313,15 @@
   __pyx_t_3 = __Pyx_PyObject_Call(__pyx_t_1, __pyx_empty_tuple, __pyx_t_2); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 138, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
   __pyx_v_dist_data = __pyx_t_3;
   __pyx_t_3 = 0;
 
-  /* "seleya/mfc/alchemy/qrank/glassdoor.py":139
+  /* "seleya/mfc/alchemy/qrank/glassdoor.pyx":139
  *         mean_data['date'] = pd.to_datetime(mean_data['date'])
  *         dist_data = self._distribute(mean_data=mean_data)
  *         if dist_data is None or dist_data.empty:             # <<<<<<<<<<<<<<
  *             kd_logger.error('distribute data is empty')
  *             return None
  */
   __pyx_t_6 = (__pyx_v_dist_data == Py_None);
@@ -5335,15 +5335,15 @@
   __Pyx_GOTREF(__pyx_t_3);
   __pyx_t_7 = __Pyx_PyObject_IsTrue(__pyx_t_3); if (unlikely(__pyx_t_7 < 0)) __PYX_ERR(0, 139, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
   __pyx_t_5 = __pyx_t_7;
   __pyx_L4_bool_binop_done:;
   if (__pyx_t_5) {
 
-    /* "seleya/mfc/alchemy/qrank/glassdoor.py":140
+    /* "seleya/mfc/alchemy/qrank/glassdoor.pyx":140
  *         dist_data = self._distribute(mean_data=mean_data)
  *         if dist_data is None or dist_data.empty:
  *             kd_logger.error('distribute data is empty')             # <<<<<<<<<<<<<<
  *             return None
  *         dist_data = dist_data.reset_index().set_index(
  */
     __Pyx_GetModuleGlobalName(__pyx_t_2, __pyx_n_s_kd_logger); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 140, __pyx_L1_error)
@@ -5364,35 +5364,35 @@
     __pyx_t_3 = (__pyx_t_2) ? __Pyx_PyObject_Call2Args(__pyx_t_1, __pyx_t_2, __pyx_kp_s_distribute_data_is_empty) : __Pyx_PyObject_CallOneArg(__pyx_t_1, __pyx_kp_s_distribute_data_is_empty);
     __Pyx_XDECREF(__pyx_t_2); __pyx_t_2 = 0;
     if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 140, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_3);
     __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
     __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
 
-    /* "seleya/mfc/alchemy/qrank/glassdoor.py":141
+    /* "seleya/mfc/alchemy/qrank/glassdoor.pyx":141
  *         if dist_data is None or dist_data.empty:
  *             kd_logger.error('distribute data is empty')
  *             return None             # <<<<<<<<<<<<<<
  *         dist_data = dist_data.reset_index().set_index(
  *             ['date', 'code', 'industry']).stack().reset_index()
  */
     __Pyx_XDECREF(__pyx_r);
     __pyx_r = Py_None; __Pyx_INCREF(Py_None);
     goto __pyx_L0;
 
-    /* "seleya/mfc/alchemy/qrank/glassdoor.py":139
+    /* "seleya/mfc/alchemy/qrank/glassdoor.pyx":139
  *         mean_data['date'] = pd.to_datetime(mean_data['date'])
  *         dist_data = self._distribute(mean_data=mean_data)
  *         if dist_data is None or dist_data.empty:             # <<<<<<<<<<<<<<
  *             kd_logger.error('distribute data is empty')
  *             return None
  */
   }
 
-  /* "seleya/mfc/alchemy/qrank/glassdoor.py":142
+  /* "seleya/mfc/alchemy/qrank/glassdoor.pyx":142
  *             kd_logger.error('distribute data is empty')
  *             return None
  *         dist_data = dist_data.reset_index().set_index(             # <<<<<<<<<<<<<<
  *             ['date', 'code', 'industry']).stack().reset_index()
  *         dist_data = dist_data.rename(columns={'level_3': 'name', 0: 'value'})
  */
   __pyx_t_8 = __Pyx_PyObject_GetAttrStr(__pyx_v_dist_data, __pyx_n_s_reset_index); if (unlikely(!__pyx_t_8)) __PYX_ERR(0, 142, __pyx_L1_error)
@@ -5412,15 +5412,15 @@
   if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 142, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_4);
   __Pyx_DECREF(__pyx_t_8); __pyx_t_8 = 0;
   __pyx_t_8 = __Pyx_PyObject_GetAttrStr(__pyx_t_4, __pyx_n_s_set_index); if (unlikely(!__pyx_t_8)) __PYX_ERR(0, 142, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_8);
   __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
 
-  /* "seleya/mfc/alchemy/qrank/glassdoor.py":143
+  /* "seleya/mfc/alchemy/qrank/glassdoor.pyx":143
  *             return None
  *         dist_data = dist_data.reset_index().set_index(
  *             ['date', 'code', 'industry']).stack().reset_index()             # <<<<<<<<<<<<<<
  *         dist_data = dist_data.rename(columns={'level_3': 'name', 0: 'value'})
  *         dist_data['date'] = dist_data['date'].dt.strftime('%Y-%m-%d')
  */
   __pyx_t_4 = PyList_New(3); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 143, __pyx_L1_error)
@@ -5485,15 +5485,15 @@
   __Pyx_XDECREF(__pyx_t_1); __pyx_t_1 = 0;
   if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 143, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
   __Pyx_DECREF(__pyx_t_8); __pyx_t_8 = 0;
   __Pyx_DECREF_SET(__pyx_v_dist_data, __pyx_t_3);
   __pyx_t_3 = 0;
 
-  /* "seleya/mfc/alchemy/qrank/glassdoor.py":144
+  /* "seleya/mfc/alchemy/qrank/glassdoor.pyx":144
  *         dist_data = dist_data.reset_index().set_index(
  *             ['date', 'code', 'industry']).stack().reset_index()
  *         dist_data = dist_data.rename(columns={'level_3': 'name', 0: 'value'})             # <<<<<<<<<<<<<<
  *         dist_data['date'] = dist_data['date'].dt.strftime('%Y-%m-%d')
  *         return dist_data
  */
   __pyx_t_3 = __Pyx_PyObject_GetAttrStr(__pyx_v_dist_data, __pyx_n_s_rename); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 144, __pyx_L1_error)
@@ -5509,15 +5509,15 @@
   __pyx_t_1 = __Pyx_PyObject_Call(__pyx_t_3, __pyx_empty_tuple, __pyx_t_8); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 144, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
   __Pyx_DECREF(__pyx_t_8); __pyx_t_8 = 0;
   __Pyx_DECREF_SET(__pyx_v_dist_data, __pyx_t_1);
   __pyx_t_1 = 0;
 
-  /* "seleya/mfc/alchemy/qrank/glassdoor.py":145
+  /* "seleya/mfc/alchemy/qrank/glassdoor.pyx":145
  *             ['date', 'code', 'industry']).stack().reset_index()
  *         dist_data = dist_data.rename(columns={'level_3': 'name', 0: 'value'})
  *         dist_data['date'] = dist_data['date'].dt.strftime('%Y-%m-%d')             # <<<<<<<<<<<<<<
  *         return dist_data
  * 
  */
   __pyx_t_8 = __Pyx_PyObject_Dict_GetItem(__pyx_v_dist_data, __pyx_n_s_date); if (unlikely(!__pyx_t_8)) __PYX_ERR(0, 145, __pyx_L1_error)
@@ -5542,27 +5542,27 @@
   __Pyx_XDECREF(__pyx_t_3); __pyx_t_3 = 0;
   if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 145, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __Pyx_DECREF(__pyx_t_8); __pyx_t_8 = 0;
   if (unlikely(PyObject_SetItem(__pyx_v_dist_data, __pyx_n_s_date, __pyx_t_1) < 0)) __PYX_ERR(0, 145, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
 
-  /* "seleya/mfc/alchemy/qrank/glassdoor.py":146
+  /* "seleya/mfc/alchemy/qrank/glassdoor.pyx":146
  *         dist_data = dist_data.rename(columns={'level_3': 'name', 0: 'value'})
  *         dist_data['date'] = dist_data['date'].dt.strftime('%Y-%m-%d')
  *         return dist_data             # <<<<<<<<<<<<<<
  * 
  *     def _format_mean(self, mean_data):
  */
   __Pyx_XDECREF(__pyx_r);
   __Pyx_INCREF(__pyx_v_dist_data);
   __pyx_r = __pyx_v_dist_data;
   goto __pyx_L0;
 
-  /* "seleya/mfc/alchemy/qrank/glassdoor.py":135
+  /* "seleya/mfc/alchemy/qrank/glassdoor.pyx":135
  *         res.append(rt.reset_index().set_index(['date', 'code']))
  * 
  *     def _calculate_distribute(self, mean_data):             # <<<<<<<<<<<<<<
  *         kd_logger.info('calculating distribute...')
  *         mean_data['date'] = pd.to_datetime(mean_data['date'])
  */
 
@@ -5570,36 +5570,36 @@
   __pyx_L1_error:;
   __Pyx_XDECREF(__pyx_t_1);
   __Pyx_XDECREF(__pyx_t_2);
   __Pyx_XDECREF(__pyx_t_3);
   __Pyx_XDECREF(__pyx_t_4);
   __Pyx_XDECREF(__pyx_t_8);
   __Pyx_XDECREF(__pyx_t_9);
-  __Pyx_AddTraceback("seleya.mfc.alchemy.qrank.glassdoo.Glassdoor._calculate_distribute", __pyx_clineno, __pyx_lineno, __pyx_filename);
+  __Pyx_AddTraceback("seleya.mfc.alchemy.qrank.glassdoor.Glassdoor._calculate_distribute", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __pyx_r = NULL;
   __pyx_L0:;
   __Pyx_XDECREF(__pyx_v_dist_data);
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "seleya/mfc/alchemy/qrank/glassdoor.py":148
+/* "seleya/mfc/alchemy/qrank/glassdoor.pyx":148
  *         return dist_data
  * 
  *     def _format_mean(self, mean_data):             # <<<<<<<<<<<<<<
  *         mean_data['industry'] = self._industry_code
  *         mean_data['date'] = mean_data['date'].dt.strftime('%Y-%m-%d')
  */
 
 /* Python wrapper */
-static PyObject *__pyx_pw_6seleya_3mfc_7alchemy_5qrank_8glassdoo_9Glassdoor_19_format_mean(PyObject *__pyx_self, PyObject *__pyx_args, PyObject *__pyx_kwds); /*proto*/
-static char __pyx_doc_6seleya_3mfc_7alchemy_5qrank_8glassdoo_9Glassdoor_18_format_mean[] = "Glassdoor._format_mean(self, mean_data)";
-static PyMethodDef __pyx_mdef_6seleya_3mfc_7alchemy_5qrank_8glassdoo_9Glassdoor_19_format_mean = {"_format_mean", (PyCFunction)(void*)(PyCFunctionWithKeywords)__pyx_pw_6seleya_3mfc_7alchemy_5qrank_8glassdoo_9Glassdoor_19_format_mean, METH_VARARGS|METH_KEYWORDS, __pyx_doc_6seleya_3mfc_7alchemy_5qrank_8glassdoo_9Glassdoor_18_format_mean};
-static PyObject *__pyx_pw_6seleya_3mfc_7alchemy_5qrank_8glassdoo_9Glassdoor_19_format_mean(PyObject *__pyx_self, PyObject *__pyx_args, PyObject *__pyx_kwds) {
+static PyObject *__pyx_pw_6seleya_3mfc_7alchemy_5qrank_9glassdoor_9Glassdoor_19_format_mean(PyObject *__pyx_self, PyObject *__pyx_args, PyObject *__pyx_kwds); /*proto*/
+static char __pyx_doc_6seleya_3mfc_7alchemy_5qrank_9glassdoor_9Glassdoor_18_format_mean[] = "Glassdoor._format_mean(self, mean_data)";
+static PyMethodDef __pyx_mdef_6seleya_3mfc_7alchemy_5qrank_9glassdoor_9Glassdoor_19_format_mean = {"_format_mean", (PyCFunction)(void*)(PyCFunctionWithKeywords)__pyx_pw_6seleya_3mfc_7alchemy_5qrank_9glassdoor_9Glassdoor_19_format_mean, METH_VARARGS|METH_KEYWORDS, __pyx_doc_6seleya_3mfc_7alchemy_5qrank_9glassdoor_9Glassdoor_18_format_mean};
+static PyObject *__pyx_pw_6seleya_3mfc_7alchemy_5qrank_9glassdoor_9Glassdoor_19_format_mean(PyObject *__pyx_self, PyObject *__pyx_args, PyObject *__pyx_kwds) {
   PyObject *__pyx_v_self = 0;
   PyObject *__pyx_v_mean_data = 0;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   PyObject *__pyx_r = 0;
   __Pyx_RefNannyDeclarations
@@ -5642,49 +5642,49 @@
     __pyx_v_self = values[0];
     __pyx_v_mean_data = values[1];
   }
   goto __pyx_L4_argument_unpacking_done;
   __pyx_L5_argtuple_error:;
   __Pyx_RaiseArgtupleInvalid("_format_mean", 1, 2, 2, PyTuple_GET_SIZE(__pyx_args)); __PYX_ERR(0, 148, __pyx_L3_error)
   __pyx_L3_error:;
-  __Pyx_AddTraceback("seleya.mfc.alchemy.qrank.glassdoo.Glassdoor._format_mean", __pyx_clineno, __pyx_lineno, __pyx_filename);
+  __Pyx_AddTraceback("seleya.mfc.alchemy.qrank.glassdoor.Glassdoor._format_mean", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __Pyx_RefNannyFinishContext();
   return NULL;
   __pyx_L4_argument_unpacking_done:;
-  __pyx_r = __pyx_pf_6seleya_3mfc_7alchemy_5qrank_8glassdoo_9Glassdoor_18_format_mean(__pyx_self, __pyx_v_self, __pyx_v_mean_data);
+  __pyx_r = __pyx_pf_6seleya_3mfc_7alchemy_5qrank_9glassdoor_9Glassdoor_18_format_mean(__pyx_self, __pyx_v_self, __pyx_v_mean_data);
 
   /* function exit code */
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-static PyObject *__pyx_pf_6seleya_3mfc_7alchemy_5qrank_8glassdoo_9Glassdoor_18_format_mean(CYTHON_UNUSED PyObject *__pyx_self, PyObject *__pyx_v_self, PyObject *__pyx_v_mean_data) {
+static PyObject *__pyx_pf_6seleya_3mfc_7alchemy_5qrank_9glassdoor_9Glassdoor_18_format_mean(CYTHON_UNUSED PyObject *__pyx_self, PyObject *__pyx_v_self, PyObject *__pyx_v_mean_data) {
   PyObject *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   PyObject *__pyx_t_2 = NULL;
   PyObject *__pyx_t_3 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("_format_mean", 0);
 
-  /* "seleya/mfc/alchemy/qrank/glassdoor.py":149
+  /* "seleya/mfc/alchemy/qrank/glassdoor.pyx":149
  * 
  *     def _format_mean(self, mean_data):
  *         mean_data['industry'] = self._industry_code             # <<<<<<<<<<<<<<
  *         mean_data['date'] = mean_data['date'].dt.strftime('%Y-%m-%d')
  *         return mean_data
  */
   __pyx_t_1 = __Pyx_PyObject_GetAttrStr(__pyx_v_self, __pyx_n_s_industry_code_2); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 149, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   if (unlikely(PyObject_SetItem(__pyx_v_mean_data, __pyx_n_s_industry, __pyx_t_1) < 0)) __PYX_ERR(0, 149, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
 
-  /* "seleya/mfc/alchemy/qrank/glassdoor.py":150
+  /* "seleya/mfc/alchemy/qrank/glassdoor.pyx":150
  *     def _format_mean(self, mean_data):
  *         mean_data['industry'] = self._industry_code
  *         mean_data['date'] = mean_data['date'].dt.strftime('%Y-%m-%d')             # <<<<<<<<<<<<<<
  *         return mean_data
  * 
  */
   __pyx_t_2 = __Pyx_PyObject_Dict_GetItem(__pyx_v_mean_data, __pyx_n_s_date); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 150, __pyx_L1_error)
@@ -5709,60 +5709,60 @@
   __Pyx_XDECREF(__pyx_t_3); __pyx_t_3 = 0;
   if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 150, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
   if (unlikely(PyObject_SetItem(__pyx_v_mean_data, __pyx_n_s_date, __pyx_t_1) < 0)) __PYX_ERR(0, 150, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
 
-  /* "seleya/mfc/alchemy/qrank/glassdoor.py":151
+  /* "seleya/mfc/alchemy/qrank/glassdoor.pyx":151
  *         mean_data['industry'] = self._industry_code
  *         mean_data['date'] = mean_data['date'].dt.strftime('%Y-%m-%d')
  *         return mean_data             # <<<<<<<<<<<<<<
  * 
  *     def calculate_result(self, total_data, threshold=0.9):
  */
   __Pyx_XDECREF(__pyx_r);
   __Pyx_INCREF(__pyx_v_mean_data);
   __pyx_r = __pyx_v_mean_data;
   goto __pyx_L0;
 
-  /* "seleya/mfc/alchemy/qrank/glassdoor.py":148
+  /* "seleya/mfc/alchemy/qrank/glassdoor.pyx":148
  *         return dist_data
  * 
  *     def _format_mean(self, mean_data):             # <<<<<<<<<<<<<<
  *         mean_data['industry'] = self._industry_code
  *         mean_data['date'] = mean_data['date'].dt.strftime('%Y-%m-%d')
  */
 
   /* function exit code */
   __pyx_L1_error:;
   __Pyx_XDECREF(__pyx_t_1);
   __Pyx_XDECREF(__pyx_t_2);
   __Pyx_XDECREF(__pyx_t_3);
-  __Pyx_AddTraceback("seleya.mfc.alchemy.qrank.glassdoo.Glassdoor._format_mean", __pyx_clineno, __pyx_lineno, __pyx_filename);
+  __Pyx_AddTraceback("seleya.mfc.alchemy.qrank.glassdoor.Glassdoor._format_mean", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __pyx_r = NULL;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "seleya/mfc/alchemy/qrank/glassdoor.py":153
+/* "seleya/mfc/alchemy/qrank/glassdoor.pyx":153
  *         return mean_data
  * 
  *     def calculate_result(self, total_data, threshold=0.9):             # <<<<<<<<<<<<<<
  *         # aggregate means by year and cid
  *         mean_data = total_data.groupby(['date', 'code']).mean()
  */
 
 /* Python wrapper */
-static PyObject *__pyx_pw_6seleya_3mfc_7alchemy_5qrank_8glassdoo_9Glassdoor_21calculate_result(PyObject *__pyx_self, PyObject *__pyx_args, PyObject *__pyx_kwds); /*proto*/
-static char __pyx_doc_6seleya_3mfc_7alchemy_5qrank_8glassdoo_9Glassdoor_20calculate_result[] = "Glassdoor.calculate_result(self, total_data, threshold=0.9)";
-static PyMethodDef __pyx_mdef_6seleya_3mfc_7alchemy_5qrank_8glassdoo_9Glassdoor_21calculate_result = {"calculate_result", (PyCFunction)(void*)(PyCFunctionWithKeywords)__pyx_pw_6seleya_3mfc_7alchemy_5qrank_8glassdoo_9Glassdoor_21calculate_result, METH_VARARGS|METH_KEYWORDS, __pyx_doc_6seleya_3mfc_7alchemy_5qrank_8glassdoo_9Glassdoor_20calculate_result};
-static PyObject *__pyx_pw_6seleya_3mfc_7alchemy_5qrank_8glassdoo_9Glassdoor_21calculate_result(PyObject *__pyx_self, PyObject *__pyx_args, PyObject *__pyx_kwds) {
+static PyObject *__pyx_pw_6seleya_3mfc_7alchemy_5qrank_9glassdoor_9Glassdoor_21calculate_result(PyObject *__pyx_self, PyObject *__pyx_args, PyObject *__pyx_kwds); /*proto*/
+static char __pyx_doc_6seleya_3mfc_7alchemy_5qrank_9glassdoor_9Glassdoor_20calculate_result[] = "Glassdoor.calculate_result(self, total_data, threshold=0.9)";
+static PyMethodDef __pyx_mdef_6seleya_3mfc_7alchemy_5qrank_9glassdoor_9Glassdoor_21calculate_result = {"calculate_result", (PyCFunction)(void*)(PyCFunctionWithKeywords)__pyx_pw_6seleya_3mfc_7alchemy_5qrank_9glassdoor_9Glassdoor_21calculate_result, METH_VARARGS|METH_KEYWORDS, __pyx_doc_6seleya_3mfc_7alchemy_5qrank_9glassdoor_9Glassdoor_20calculate_result};
+static PyObject *__pyx_pw_6seleya_3mfc_7alchemy_5qrank_9glassdoor_9Glassdoor_21calculate_result(PyObject *__pyx_self, PyObject *__pyx_args, PyObject *__pyx_kwds) {
   PyObject *__pyx_v_self = 0;
   PyObject *__pyx_v_total_data = 0;
   PyObject *__pyx_v_threshold = 0;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   PyObject *__pyx_r = 0;
@@ -5820,104 +5820,104 @@
     __pyx_v_total_data = values[1];
     __pyx_v_threshold = values[2];
   }
   goto __pyx_L4_argument_unpacking_done;
   __pyx_L5_argtuple_error:;
   __Pyx_RaiseArgtupleInvalid("calculate_result", 0, 2, 3, PyTuple_GET_SIZE(__pyx_args)); __PYX_ERR(0, 153, __pyx_L3_error)
   __pyx_L3_error:;
-  __Pyx_AddTraceback("seleya.mfc.alchemy.qrank.glassdoo.Glassdoor.calculate_result", __pyx_clineno, __pyx_lineno, __pyx_filename);
+  __Pyx_AddTraceback("seleya.mfc.alchemy.qrank.glassdoor.Glassdoor.calculate_result", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __Pyx_RefNannyFinishContext();
   return NULL;
   __pyx_L4_argument_unpacking_done:;
-  __pyx_r = __pyx_pf_6seleya_3mfc_7alchemy_5qrank_8glassdoo_9Glassdoor_20calculate_result(__pyx_self, __pyx_v_self, __pyx_v_total_data, __pyx_v_threshold);
+  __pyx_r = __pyx_pf_6seleya_3mfc_7alchemy_5qrank_9glassdoor_9Glassdoor_20calculate_result(__pyx_self, __pyx_v_self, __pyx_v_total_data, __pyx_v_threshold);
 
   /* function exit code */
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "seleya/mfc/alchemy/qrank/glassdoor.py":164
+/* "seleya/mfc/alchemy/qrank/glassdoor.pyx":164
  *         for col_name in self._factors_sets:
  *             col_score = mean_data.sort_values(by=['date', 'code']).groupby(
  *                 by=['date']).apply(lambda x: self._blom_score(             # <<<<<<<<<<<<<<
  *                     x[col_name], threshold=threshold))
  *             if isinstance(col_score, pd.DataFrame):
  */
 
 /* Python wrapper */
-static PyObject *__pyx_pw_6seleya_3mfc_7alchemy_5qrank_8glassdoo_9Glassdoor_16calculate_result_lambda2(PyObject *__pyx_self, PyObject *__pyx_v_x); /*proto*/
-static PyMethodDef __pyx_mdef_6seleya_3mfc_7alchemy_5qrank_8glassdoo_9Glassdoor_16calculate_result_lambda2 = {"lambda2", (PyCFunction)__pyx_pw_6seleya_3mfc_7alchemy_5qrank_8glassdoo_9Glassdoor_16calculate_result_lambda2, METH_O, 0};
-static PyObject *__pyx_pw_6seleya_3mfc_7alchemy_5qrank_8glassdoo_9Glassdoor_16calculate_result_lambda2(PyObject *__pyx_self, PyObject *__pyx_v_x) {
+static PyObject *__pyx_pw_6seleya_3mfc_7alchemy_5qrank_9glassdoor_9Glassdoor_16calculate_result_lambda2(PyObject *__pyx_self, PyObject *__pyx_v_x); /*proto*/
+static PyMethodDef __pyx_mdef_6seleya_3mfc_7alchemy_5qrank_9glassdoor_9Glassdoor_16calculate_result_lambda2 = {"lambda2", (PyCFunction)__pyx_pw_6seleya_3mfc_7alchemy_5qrank_9glassdoor_9Glassdoor_16calculate_result_lambda2, METH_O, 0};
+static PyObject *__pyx_pw_6seleya_3mfc_7alchemy_5qrank_9glassdoor_9Glassdoor_16calculate_result_lambda2(PyObject *__pyx_self, PyObject *__pyx_v_x) {
   PyObject *__pyx_r = 0;
   __Pyx_RefNannyDeclarations
   __Pyx_RefNannySetupContext("lambda2 (wrapper)", 0);
   __pyx_r = __pyx_lambda_funcdef_lambda2(__pyx_self, ((PyObject *)__pyx_v_x));
 
   /* function exit code */
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
 static PyObject *__pyx_lambda_funcdef_lambda2(PyObject *__pyx_self, PyObject *__pyx_v_x) {
-  struct __pyx_obj_6seleya_3mfc_7alchemy_5qrank_8glassdoo___pyx_scope_struct_2_calculate_result *__pyx_cur_scope;
-  struct __pyx_obj_6seleya_3mfc_7alchemy_5qrank_8glassdoo___pyx_scope_struct_2_calculate_result *__pyx_outer_scope;
+  struct __pyx_obj_6seleya_3mfc_7alchemy_5qrank_9glassdoor___pyx_scope_struct_2_calculate_result *__pyx_cur_scope;
+  struct __pyx_obj_6seleya_3mfc_7alchemy_5qrank_9glassdoor___pyx_scope_struct_2_calculate_result *__pyx_outer_scope;
   PyObject *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   PyObject *__pyx_t_2 = NULL;
   PyObject *__pyx_t_3 = NULL;
   PyObject *__pyx_t_4 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("lambda2", 0);
-  __pyx_outer_scope = (struct __pyx_obj_6seleya_3mfc_7alchemy_5qrank_8glassdoo___pyx_scope_struct_2_calculate_result *) __Pyx_CyFunction_GetClosure(__pyx_self);
+  __pyx_outer_scope = (struct __pyx_obj_6seleya_3mfc_7alchemy_5qrank_9glassdoor___pyx_scope_struct_2_calculate_result *) __Pyx_CyFunction_GetClosure(__pyx_self);
   __pyx_cur_scope = __pyx_outer_scope;
   __Pyx_XDECREF(__pyx_r);
   if (unlikely(!__pyx_cur_scope->__pyx_v_self)) { __Pyx_RaiseClosureNameError("self"); __PYX_ERR(0, 164, __pyx_L1_error) }
   __pyx_t_1 = __Pyx_PyObject_GetAttrStr(__pyx_cur_scope->__pyx_v_self, __pyx_n_s_blom_score); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 164, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
 
-  /* "seleya/mfc/alchemy/qrank/glassdoor.py":165
+  /* "seleya/mfc/alchemy/qrank/glassdoor.pyx":165
  *             col_score = mean_data.sort_values(by=['date', 'code']).groupby(
  *                 by=['date']).apply(lambda x: self._blom_score(
  *                     x[col_name], threshold=threshold))             # <<<<<<<<<<<<<<
  *             if isinstance(col_score, pd.DataFrame):
  *                 col_score = col_score.stack()
  */
   if (unlikely(!__pyx_cur_scope->__pyx_v_col_name)) { __Pyx_RaiseClosureNameError("col_name"); __PYX_ERR(0, 165, __pyx_L1_error) }
   __pyx_t_2 = __Pyx_PyObject_GetItem(__pyx_v_x, __pyx_cur_scope->__pyx_v_col_name); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 165, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
 
-  /* "seleya/mfc/alchemy/qrank/glassdoor.py":164
+  /* "seleya/mfc/alchemy/qrank/glassdoor.pyx":164
  *         for col_name in self._factors_sets:
  *             col_score = mean_data.sort_values(by=['date', 'code']).groupby(
  *                 by=['date']).apply(lambda x: self._blom_score(             # <<<<<<<<<<<<<<
  *                     x[col_name], threshold=threshold))
  *             if isinstance(col_score, pd.DataFrame):
  */
   __pyx_t_3 = PyTuple_New(1); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 164, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
   __Pyx_GIVEREF(__pyx_t_2);
   PyTuple_SET_ITEM(__pyx_t_3, 0, __pyx_t_2);
   __pyx_t_2 = 0;
 
-  /* "seleya/mfc/alchemy/qrank/glassdoor.py":165
+  /* "seleya/mfc/alchemy/qrank/glassdoor.pyx":165
  *             col_score = mean_data.sort_values(by=['date', 'code']).groupby(
  *                 by=['date']).apply(lambda x: self._blom_score(
  *                     x[col_name], threshold=threshold))             # <<<<<<<<<<<<<<
  *             if isinstance(col_score, pd.DataFrame):
  *                 col_score = col_score.stack()
  */
   __pyx_t_2 = __Pyx_PyDict_NewPresized(1); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 165, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   if (unlikely(!__pyx_cur_scope->__pyx_v_threshold)) { __Pyx_RaiseClosureNameError("threshold"); __PYX_ERR(0, 165, __pyx_L1_error) }
   if (PyDict_SetItem(__pyx_t_2, __pyx_n_s_threshold, __pyx_cur_scope->__pyx_v_threshold) < 0) __PYX_ERR(0, 165, __pyx_L1_error)
 
-  /* "seleya/mfc/alchemy/qrank/glassdoor.py":164
+  /* "seleya/mfc/alchemy/qrank/glassdoor.pyx":164
  *         for col_name in self._factors_sets:
  *             col_score = mean_data.sort_values(by=['date', 'code']).groupby(
  *                 by=['date']).apply(lambda x: self._blom_score(             # <<<<<<<<<<<<<<
  *                     x[col_name], threshold=threshold))
  *             if isinstance(col_score, pd.DataFrame):
  */
   __pyx_t_4 = __Pyx_PyObject_Call(__pyx_t_1, __pyx_t_3, __pyx_t_2); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 164, __pyx_L1_error)
@@ -5931,32 +5931,32 @@
 
   /* function exit code */
   __pyx_L1_error:;
   __Pyx_XDECREF(__pyx_t_1);
   __Pyx_XDECREF(__pyx_t_2);
   __Pyx_XDECREF(__pyx_t_3);
   __Pyx_XDECREF(__pyx_t_4);
-  __Pyx_AddTraceback("seleya.mfc.alchemy.qrank.glassdoo.Glassdoor.calculate_result.lambda2", __pyx_clineno, __pyx_lineno, __pyx_filename);
+  __Pyx_AddTraceback("seleya.mfc.alchemy.qrank.glassdoor.Glassdoor.calculate_result.lambda2", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __pyx_r = NULL;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "seleya/mfc/alchemy/qrank/glassdoor.py":153
+/* "seleya/mfc/alchemy/qrank/glassdoor.pyx":153
  *         return mean_data
  * 
  *     def calculate_result(self, total_data, threshold=0.9):             # <<<<<<<<<<<<<<
  *         # aggregate means by year and cid
  *         mean_data = total_data.groupby(['date', 'code']).mean()
  */
 
-static PyObject *__pyx_pf_6seleya_3mfc_7alchemy_5qrank_8glassdoo_9Glassdoor_20calculate_result(CYTHON_UNUSED PyObject *__pyx_self, PyObject *__pyx_v_self, PyObject *__pyx_v_total_data, PyObject *__pyx_v_threshold) {
-  struct __pyx_obj_6seleya_3mfc_7alchemy_5qrank_8glassdoo___pyx_scope_struct_2_calculate_result *__pyx_cur_scope;
+static PyObject *__pyx_pf_6seleya_3mfc_7alchemy_5qrank_9glassdoor_9Glassdoor_20calculate_result(CYTHON_UNUSED PyObject *__pyx_self, PyObject *__pyx_v_self, PyObject *__pyx_v_total_data, PyObject *__pyx_v_threshold) {
+  struct __pyx_obj_6seleya_3mfc_7alchemy_5qrank_9glassdoor___pyx_scope_struct_2_calculate_result *__pyx_cur_scope;
   PyObject *__pyx_v_mean_data = NULL;
   PyObject *__pyx_v_raw_data = NULL;
   PyObject *__pyx_v_col_score = NULL;
   PyObject *__pyx_v_dist_data = NULL;
   PyObject *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
@@ -5969,30 +5969,30 @@
   int __pyx_t_8;
   Py_ssize_t __pyx_t_9;
   PyObject *(*__pyx_t_10)(PyObject *);
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("calculate_result", 0);
-  __pyx_cur_scope = (struct __pyx_obj_6seleya_3mfc_7alchemy_5qrank_8glassdoo___pyx_scope_struct_2_calculate_result *)__pyx_tp_new_6seleya_3mfc_7alchemy_5qrank_8glassdoo___pyx_scope_struct_2_calculate_result(__pyx_ptype_6seleya_3mfc_7alchemy_5qrank_8glassdoo___pyx_scope_struct_2_calculate_result, __pyx_empty_tuple, NULL);
+  __pyx_cur_scope = (struct __pyx_obj_6seleya_3mfc_7alchemy_5qrank_9glassdoor___pyx_scope_struct_2_calculate_result *)__pyx_tp_new_6seleya_3mfc_7alchemy_5qrank_9glassdoor___pyx_scope_struct_2_calculate_result(__pyx_ptype_6seleya_3mfc_7alchemy_5qrank_9glassdoor___pyx_scope_struct_2_calculate_result, __pyx_empty_tuple, NULL);
   if (unlikely(!__pyx_cur_scope)) {
-    __pyx_cur_scope = ((struct __pyx_obj_6seleya_3mfc_7alchemy_5qrank_8glassdoo___pyx_scope_struct_2_calculate_result *)Py_None);
+    __pyx_cur_scope = ((struct __pyx_obj_6seleya_3mfc_7alchemy_5qrank_9glassdoor___pyx_scope_struct_2_calculate_result *)Py_None);
     __Pyx_INCREF(Py_None);
     __PYX_ERR(0, 153, __pyx_L1_error)
   } else {
     __Pyx_GOTREF(__pyx_cur_scope);
   }
   __pyx_cur_scope->__pyx_v_self = __pyx_v_self;
   __Pyx_INCREF(__pyx_cur_scope->__pyx_v_self);
   __Pyx_GIVEREF(__pyx_cur_scope->__pyx_v_self);
   __pyx_cur_scope->__pyx_v_threshold = __pyx_v_threshold;
   __Pyx_INCREF(__pyx_cur_scope->__pyx_v_threshold);
   __Pyx_GIVEREF(__pyx_cur_scope->__pyx_v_threshold);
 
-  /* "seleya/mfc/alchemy/qrank/glassdoor.py":155
+  /* "seleya/mfc/alchemy/qrank/glassdoor.pyx":155
  *     def calculate_result(self, total_data, threshold=0.9):
  *         # aggregate means by year and cid
  *         mean_data = total_data.groupby(['date', 'code']).mean()             # <<<<<<<<<<<<<<
  *         raw_data = self._transform_raw(mean_data=mean_data)
  *         if raw_data is None or raw_data.empty:
  */
   __pyx_t_3 = __Pyx_PyObject_GetAttrStr(__pyx_v_total_data, __pyx_n_s_groupby); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 155, __pyx_L1_error)
@@ -6038,15 +6038,15 @@
   __Pyx_XDECREF(__pyx_t_2); __pyx_t_2 = 0;
   if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 155, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
   __pyx_v_mean_data = __pyx_t_1;
   __pyx_t_1 = 0;
 
-  /* "seleya/mfc/alchemy/qrank/glassdoor.py":156
+  /* "seleya/mfc/alchemy/qrank/glassdoor.pyx":156
  *         # aggregate means by year and cid
  *         mean_data = total_data.groupby(['date', 'code']).mean()
  *         raw_data = self._transform_raw(mean_data=mean_data)             # <<<<<<<<<<<<<<
  *         if raw_data is None or raw_data.empty:
  *             kd_logger.error('raw data is empty')
  */
   __pyx_t_1 = __Pyx_PyObject_GetAttrStr(__pyx_cur_scope->__pyx_v_self, __pyx_n_s_transform_raw); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 156, __pyx_L1_error)
@@ -6057,15 +6057,15 @@
   __pyx_t_2 = __Pyx_PyObject_Call(__pyx_t_1, __pyx_empty_tuple, __pyx_t_3); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 156, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
   __pyx_v_raw_data = __pyx_t_2;
   __pyx_t_2 = 0;
 
-  /* "seleya/mfc/alchemy/qrank/glassdoor.py":157
+  /* "seleya/mfc/alchemy/qrank/glassdoor.pyx":157
  *         mean_data = total_data.groupby(['date', 'code']).mean()
  *         raw_data = self._transform_raw(mean_data=mean_data)
  *         if raw_data is None or raw_data.empty:             # <<<<<<<<<<<<<<
  *             kd_logger.error('raw data is empty')
  *             return None
  */
   __pyx_t_7 = (__pyx_v_raw_data == Py_None);
@@ -6079,15 +6079,15 @@
   __Pyx_GOTREF(__pyx_t_2);
   __pyx_t_8 = __Pyx_PyObject_IsTrue(__pyx_t_2); if (unlikely(__pyx_t_8 < 0)) __PYX_ERR(0, 157, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
   __pyx_t_6 = __pyx_t_8;
   __pyx_L4_bool_binop_done:;
   if (__pyx_t_6) {
 
-    /* "seleya/mfc/alchemy/qrank/glassdoor.py":158
+    /* "seleya/mfc/alchemy/qrank/glassdoor.pyx":158
  *         raw_data = self._transform_raw(mean_data=mean_data)
  *         if raw_data is None or raw_data.empty:
  *             kd_logger.error('raw data is empty')             # <<<<<<<<<<<<<<
  *             return None
  * 
  */
     __Pyx_GetModuleGlobalName(__pyx_t_3, __pyx_n_s_kd_logger); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 158, __pyx_L1_error)
@@ -6108,35 +6108,35 @@
     __pyx_t_2 = (__pyx_t_3) ? __Pyx_PyObject_Call2Args(__pyx_t_1, __pyx_t_3, __pyx_kp_s_raw_data_is_empty) : __Pyx_PyObject_CallOneArg(__pyx_t_1, __pyx_kp_s_raw_data_is_empty);
     __Pyx_XDECREF(__pyx_t_3); __pyx_t_3 = 0;
     if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 158, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_2);
     __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
     __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
 
-    /* "seleya/mfc/alchemy/qrank/glassdoor.py":159
+    /* "seleya/mfc/alchemy/qrank/glassdoor.pyx":159
  *         if raw_data is None or raw_data.empty:
  *             kd_logger.error('raw data is empty')
  *             return None             # <<<<<<<<<<<<<<
  * 
  *         kd_logger.info('calculating blom score...')
  */
     __Pyx_XDECREF(__pyx_r);
     __pyx_r = Py_None; __Pyx_INCREF(Py_None);
     goto __pyx_L0;
 
-    /* "seleya/mfc/alchemy/qrank/glassdoor.py":157
+    /* "seleya/mfc/alchemy/qrank/glassdoor.pyx":157
  *         mean_data = total_data.groupby(['date', 'code']).mean()
  *         raw_data = self._transform_raw(mean_data=mean_data)
  *         if raw_data is None or raw_data.empty:             # <<<<<<<<<<<<<<
  *             kd_logger.error('raw data is empty')
  *             return None
  */
   }
 
-  /* "seleya/mfc/alchemy/qrank/glassdoor.py":161
+  /* "seleya/mfc/alchemy/qrank/glassdoor.pyx":161
  *             return None
  * 
  *         kd_logger.info('calculating blom score...')             # <<<<<<<<<<<<<<
  *         for col_name in self._factors_sets:
  *             col_score = mean_data.sort_values(by=['date', 'code']).groupby(
  */
   __Pyx_GetModuleGlobalName(__pyx_t_1, __pyx_n_s_kd_logger); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 161, __pyx_L1_error)
@@ -6157,15 +6157,15 @@
   __pyx_t_2 = (__pyx_t_1) ? __Pyx_PyObject_Call2Args(__pyx_t_3, __pyx_t_1, __pyx_kp_s_calculating_blom_score) : __Pyx_PyObject_CallOneArg(__pyx_t_3, __pyx_kp_s_calculating_blom_score);
   __Pyx_XDECREF(__pyx_t_1); __pyx_t_1 = 0;
   if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 161, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
 
-  /* "seleya/mfc/alchemy/qrank/glassdoor.py":162
+  /* "seleya/mfc/alchemy/qrank/glassdoor.pyx":162
  * 
  *         kd_logger.info('calculating blom score...')
  *         for col_name in self._factors_sets:             # <<<<<<<<<<<<<<
  *             col_score = mean_data.sort_values(by=['date', 'code']).groupby(
  *                 by=['date']).apply(lambda x: self._blom_score(
  */
   __pyx_t_2 = __Pyx_PyObject_GetAttrStr(__pyx_cur_scope->__pyx_v_self, __pyx_n_s_factors_sets); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 162, __pyx_L1_error)
@@ -6211,15 +6211,15 @@
       __Pyx_GOTREF(__pyx_t_2);
     }
     __Pyx_XGOTREF(__pyx_cur_scope->__pyx_v_col_name);
     __Pyx_XDECREF_SET(__pyx_cur_scope->__pyx_v_col_name, __pyx_t_2);
     __Pyx_GIVEREF(__pyx_t_2);
     __pyx_t_2 = 0;
 
-    /* "seleya/mfc/alchemy/qrank/glassdoor.py":163
+    /* "seleya/mfc/alchemy/qrank/glassdoor.pyx":163
  *         kd_logger.info('calculating blom score...')
  *         for col_name in self._factors_sets:
  *             col_score = mean_data.sort_values(by=['date', 'code']).groupby(             # <<<<<<<<<<<<<<
  *                 by=['date']).apply(lambda x: self._blom_score(
  *                     x[col_name], threshold=threshold))
  */
     __pyx_t_1 = __Pyx_PyObject_GetAttrStr(__pyx_v_mean_data, __pyx_n_s_sort_values); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 163, __pyx_L1_error)
@@ -6240,15 +6240,15 @@
     __Pyx_GOTREF(__pyx_t_5);
     __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
     __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
     __pyx_t_4 = __Pyx_PyObject_GetAttrStr(__pyx_t_5, __pyx_n_s_groupby); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 163, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_4);
     __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
 
-    /* "seleya/mfc/alchemy/qrank/glassdoor.py":164
+    /* "seleya/mfc/alchemy/qrank/glassdoor.pyx":164
  *         for col_name in self._factors_sets:
  *             col_score = mean_data.sort_values(by=['date', 'code']).groupby(
  *                 by=['date']).apply(lambda x: self._blom_score(             # <<<<<<<<<<<<<<
  *                     x[col_name], threshold=threshold))
  *             if isinstance(col_score, pd.DataFrame):
  */
     __pyx_t_5 = __Pyx_PyDict_NewPresized(1); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 164, __pyx_L1_error)
@@ -6257,37 +6257,37 @@
     __Pyx_GOTREF(__pyx_t_1);
     __Pyx_INCREF(__pyx_n_s_date);
     __Pyx_GIVEREF(__pyx_n_s_date);
     PyList_SET_ITEM(__pyx_t_1, 0, __pyx_n_s_date);
     if (PyDict_SetItem(__pyx_t_5, __pyx_n_s_by, __pyx_t_1) < 0) __PYX_ERR(0, 164, __pyx_L1_error)
     __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
 
-    /* "seleya/mfc/alchemy/qrank/glassdoor.py":163
+    /* "seleya/mfc/alchemy/qrank/glassdoor.pyx":163
  *         kd_logger.info('calculating blom score...')
  *         for col_name in self._factors_sets:
  *             col_score = mean_data.sort_values(by=['date', 'code']).groupby(             # <<<<<<<<<<<<<<
  *                 by=['date']).apply(lambda x: self._blom_score(
  *                     x[col_name], threshold=threshold))
  */
     __pyx_t_1 = __Pyx_PyObject_Call(__pyx_t_4, __pyx_empty_tuple, __pyx_t_5); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 163, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_1);
     __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
     __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
 
-    /* "seleya/mfc/alchemy/qrank/glassdoor.py":164
+    /* "seleya/mfc/alchemy/qrank/glassdoor.pyx":164
  *         for col_name in self._factors_sets:
  *             col_score = mean_data.sort_values(by=['date', 'code']).groupby(
  *                 by=['date']).apply(lambda x: self._blom_score(             # <<<<<<<<<<<<<<
  *                     x[col_name], threshold=threshold))
  *             if isinstance(col_score, pd.DataFrame):
  */
     __pyx_t_5 = __Pyx_PyObject_GetAttrStr(__pyx_t_1, __pyx_n_s_apply); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 164, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_5);
     __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
-    __pyx_t_1 = __Pyx_CyFunction_New(&__pyx_mdef_6seleya_3mfc_7alchemy_5qrank_8glassdoo_9Glassdoor_16calculate_result_lambda2, 0, __pyx_n_s_Glassdoor_calculate_result_local, ((PyObject*)__pyx_cur_scope), __pyx_n_s_seleya_mfc_alchemy_qrank_glassdo, __pyx_d, NULL); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 164, __pyx_L1_error)
+    __pyx_t_1 = __Pyx_CyFunction_New(&__pyx_mdef_6seleya_3mfc_7alchemy_5qrank_9glassdoor_9Glassdoor_16calculate_result_lambda2, 0, __pyx_n_s_Glassdoor_calculate_result_local, ((PyObject*)__pyx_cur_scope), __pyx_n_s_seleya_mfc_alchemy_qrank_glassdo, __pyx_d, NULL); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 164, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_1);
     __pyx_t_4 = NULL;
     if (CYTHON_UNPACK_METHODS && likely(PyMethod_Check(__pyx_t_5))) {
       __pyx_t_4 = PyMethod_GET_SELF(__pyx_t_5);
       if (likely(__pyx_t_4)) {
         PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_5);
         __Pyx_INCREF(__pyx_t_4);
@@ -6300,15 +6300,15 @@
     __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
     if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 164, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_2);
     __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
     __Pyx_XDECREF_SET(__pyx_v_col_score, __pyx_t_2);
     __pyx_t_2 = 0;
 
-    /* "seleya/mfc/alchemy/qrank/glassdoor.py":166
+    /* "seleya/mfc/alchemy/qrank/glassdoor.pyx":166
  *                 by=['date']).apply(lambda x: self._blom_score(
  *                     x[col_name], threshold=threshold))
  *             if isinstance(col_score, pd.DataFrame):             # <<<<<<<<<<<<<<
  *                 col_score = col_score.stack()
  *             col_score.name = col_name
  */
     __Pyx_GetModuleGlobalName(__pyx_t_2, __pyx_n_s_pd); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 166, __pyx_L1_error)
@@ -6317,15 +6317,15 @@
     __Pyx_GOTREF(__pyx_t_5);
     __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
     __pyx_t_6 = PyObject_IsInstance(__pyx_v_col_score, __pyx_t_5); if (unlikely(__pyx_t_6 == ((int)-1))) __PYX_ERR(0, 166, __pyx_L1_error)
     __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
     __pyx_t_8 = (__pyx_t_6 != 0);
     if (__pyx_t_8) {
 
-      /* "seleya/mfc/alchemy/qrank/glassdoor.py":167
+      /* "seleya/mfc/alchemy/qrank/glassdoor.pyx":167
  *                     x[col_name], threshold=threshold))
  *             if isinstance(col_score, pd.DataFrame):
  *                 col_score = col_score.stack()             # <<<<<<<<<<<<<<
  *             col_score.name = col_name
  *             mean_data[col_name] = col_score
  */
       __pyx_t_2 = __Pyx_PyObject_GetAttrStr(__pyx_v_col_score, __pyx_n_s_stack); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 167, __pyx_L1_error)
@@ -6344,52 +6344,52 @@
       __Pyx_XDECREF(__pyx_t_1); __pyx_t_1 = 0;
       if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 167, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_5);
       __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
       __Pyx_DECREF_SET(__pyx_v_col_score, __pyx_t_5);
       __pyx_t_5 = 0;
 
-      /* "seleya/mfc/alchemy/qrank/glassdoor.py":166
+      /* "seleya/mfc/alchemy/qrank/glassdoor.pyx":166
  *                 by=['date']).apply(lambda x: self._blom_score(
  *                     x[col_name], threshold=threshold))
  *             if isinstance(col_score, pd.DataFrame):             # <<<<<<<<<<<<<<
  *                 col_score = col_score.stack()
  *             col_score.name = col_name
  */
     }
 
-    /* "seleya/mfc/alchemy/qrank/glassdoor.py":168
+    /* "seleya/mfc/alchemy/qrank/glassdoor.pyx":168
  *             if isinstance(col_score, pd.DataFrame):
  *                 col_score = col_score.stack()
  *             col_score.name = col_name             # <<<<<<<<<<<<<<
  *             mean_data[col_name] = col_score
  *         mean_data = mean_data.stack().reset_index().rename(columns={
  */
     if (__Pyx_PyObject_SetAttrStr(__pyx_v_col_score, __pyx_n_s_name, __pyx_cur_scope->__pyx_v_col_name) < 0) __PYX_ERR(0, 168, __pyx_L1_error)
 
-    /* "seleya/mfc/alchemy/qrank/glassdoor.py":169
+    /* "seleya/mfc/alchemy/qrank/glassdoor.pyx":169
  *                 col_score = col_score.stack()
  *             col_score.name = col_name
  *             mean_data[col_name] = col_score             # <<<<<<<<<<<<<<
  *         mean_data = mean_data.stack().reset_index().rename(columns={
  *             'level_2': 'name',
  */
     if (unlikely(PyObject_SetItem(__pyx_v_mean_data, __pyx_cur_scope->__pyx_v_col_name, __pyx_v_col_score) < 0)) __PYX_ERR(0, 169, __pyx_L1_error)
 
-    /* "seleya/mfc/alchemy/qrank/glassdoor.py":162
+    /* "seleya/mfc/alchemy/qrank/glassdoor.pyx":162
  * 
  *         kd_logger.info('calculating blom score...')
  *         for col_name in self._factors_sets:             # <<<<<<<<<<<<<<
  *             col_score = mean_data.sort_values(by=['date', 'code']).groupby(
  *                 by=['date']).apply(lambda x: self._blom_score(
  */
   }
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
 
-  /* "seleya/mfc/alchemy/qrank/glassdoor.py":170
+  /* "seleya/mfc/alchemy/qrank/glassdoor.pyx":170
  *             col_score.name = col_name
  *             mean_data[col_name] = col_score
  *         mean_data = mean_data.stack().reset_index().rename(columns={             # <<<<<<<<<<<<<<
  *             'level_2': 'name',
  *             0: 'value'
  */
   __pyx_t_2 = __Pyx_PyObject_GetAttrStr(__pyx_v_mean_data, __pyx_n_s_stack); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 170, __pyx_L1_error)
@@ -6429,43 +6429,43 @@
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
   __pyx_t_2 = __Pyx_PyObject_GetAttrStr(__pyx_t_3, __pyx_n_s_rename); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 170, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
   __pyx_t_3 = __Pyx_PyDict_NewPresized(1); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 170, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
 
-  /* "seleya/mfc/alchemy/qrank/glassdoor.py":171
+  /* "seleya/mfc/alchemy/qrank/glassdoor.pyx":171
  *             mean_data[col_name] = col_score
  *         mean_data = mean_data.stack().reset_index().rename(columns={
  *             'level_2': 'name',             # <<<<<<<<<<<<<<
  *             0: 'value'
  *         })
  */
   __pyx_t_5 = __Pyx_PyDict_NewPresized(2); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 171, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_5);
   if (PyDict_SetItem(__pyx_t_5, __pyx_n_s_level_2, __pyx_n_s_name) < 0) __PYX_ERR(0, 171, __pyx_L1_error)
   if (PyDict_SetItem(__pyx_t_5, __pyx_int_0, __pyx_n_s_value) < 0) __PYX_ERR(0, 171, __pyx_L1_error)
   if (PyDict_SetItem(__pyx_t_3, __pyx_n_s_columns, __pyx_t_5) < 0) __PYX_ERR(0, 170, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
 
-  /* "seleya/mfc/alchemy/qrank/glassdoor.py":170
+  /* "seleya/mfc/alchemy/qrank/glassdoor.pyx":170
  *             col_score.name = col_name
  *             mean_data[col_name] = col_score
  *         mean_data = mean_data.stack().reset_index().rename(columns={             # <<<<<<<<<<<<<<
  *             'level_2': 'name',
  *             0: 'value'
  */
   __pyx_t_5 = __Pyx_PyObject_Call(__pyx_t_2, __pyx_empty_tuple, __pyx_t_3); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 170, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_5);
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
   __Pyx_DECREF_SET(__pyx_v_mean_data, __pyx_t_5);
   __pyx_t_5 = 0;
 
-  /* "seleya/mfc/alchemy/qrank/glassdoor.py":175
+  /* "seleya/mfc/alchemy/qrank/glassdoor.pyx":175
  *         })
  * 
  *         dist_data = self._calculate_distribute(mean_data=mean_data)             # <<<<<<<<<<<<<<
  *         if dist_data is None or dist_data.empty:
  *             kd_logger.error('distribute data is empty')
  */
   __pyx_t_5 = __Pyx_PyObject_GetAttrStr(__pyx_cur_scope->__pyx_v_self, __pyx_n_s_calculate_distribute); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 175, __pyx_L1_error)
@@ -6476,15 +6476,15 @@
   __pyx_t_2 = __Pyx_PyObject_Call(__pyx_t_5, __pyx_empty_tuple, __pyx_t_3); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 175, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
   __pyx_v_dist_data = __pyx_t_2;
   __pyx_t_2 = 0;
 
-  /* "seleya/mfc/alchemy/qrank/glassdoor.py":176
+  /* "seleya/mfc/alchemy/qrank/glassdoor.pyx":176
  * 
  *         dist_data = self._calculate_distribute(mean_data=mean_data)
  *         if dist_data is None or dist_data.empty:             # <<<<<<<<<<<<<<
  *             kd_logger.error('distribute data is empty')
  *             return None
  */
   __pyx_t_6 = (__pyx_v_dist_data == Py_None);
@@ -6498,15 +6498,15 @@
   __Pyx_GOTREF(__pyx_t_2);
   __pyx_t_7 = __Pyx_PyObject_IsTrue(__pyx_t_2); if (unlikely(__pyx_t_7 < 0)) __PYX_ERR(0, 176, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
   __pyx_t_8 = __pyx_t_7;
   __pyx_L10_bool_binop_done:;
   if (__pyx_t_8) {
 
-    /* "seleya/mfc/alchemy/qrank/glassdoor.py":177
+    /* "seleya/mfc/alchemy/qrank/glassdoor.pyx":177
  *         dist_data = self._calculate_distribute(mean_data=mean_data)
  *         if dist_data is None or dist_data.empty:
  *             kd_logger.error('distribute data is empty')             # <<<<<<<<<<<<<<
  *             return None
  * 
  */
     __Pyx_GetModuleGlobalName(__pyx_t_3, __pyx_n_s_kd_logger); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 177, __pyx_L1_error)
@@ -6527,35 +6527,35 @@
     __pyx_t_2 = (__pyx_t_3) ? __Pyx_PyObject_Call2Args(__pyx_t_5, __pyx_t_3, __pyx_kp_s_distribute_data_is_empty) : __Pyx_PyObject_CallOneArg(__pyx_t_5, __pyx_kp_s_distribute_data_is_empty);
     __Pyx_XDECREF(__pyx_t_3); __pyx_t_3 = 0;
     if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 177, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_2);
     __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
     __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
 
-    /* "seleya/mfc/alchemy/qrank/glassdoor.py":178
+    /* "seleya/mfc/alchemy/qrank/glassdoor.pyx":178
  *         if dist_data is None or dist_data.empty:
  *             kd_logger.error('distribute data is empty')
  *             return None             # <<<<<<<<<<<<<<
  * 
  *         kd_logger.info('calculating success...')
  */
     __Pyx_XDECREF(__pyx_r);
     __pyx_r = Py_None; __Pyx_INCREF(Py_None);
     goto __pyx_L0;
 
-    /* "seleya/mfc/alchemy/qrank/glassdoor.py":176
+    /* "seleya/mfc/alchemy/qrank/glassdoor.pyx":176
  * 
  *         dist_data = self._calculate_distribute(mean_data=mean_data)
  *         if dist_data is None or dist_data.empty:             # <<<<<<<<<<<<<<
  *             kd_logger.error('distribute data is empty')
  *             return None
  */
   }
 
-  /* "seleya/mfc/alchemy/qrank/glassdoor.py":180
+  /* "seleya/mfc/alchemy/qrank/glassdoor.pyx":180
  *             return None
  * 
  *         kd_logger.info('calculating success...')             # <<<<<<<<<<<<<<
  *         return raw_data, self._format_mean(mean_data), dist_data
  * 
  */
   __Pyx_GetModuleGlobalName(__pyx_t_5, __pyx_n_s_kd_logger); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 180, __pyx_L1_error)
@@ -6576,15 +6576,15 @@
   __pyx_t_2 = (__pyx_t_5) ? __Pyx_PyObject_Call2Args(__pyx_t_3, __pyx_t_5, __pyx_kp_s_calculating_success) : __Pyx_PyObject_CallOneArg(__pyx_t_3, __pyx_kp_s_calculating_success);
   __Pyx_XDECREF(__pyx_t_5); __pyx_t_5 = 0;
   if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 180, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
 
-  /* "seleya/mfc/alchemy/qrank/glassdoor.py":181
+  /* "seleya/mfc/alchemy/qrank/glassdoor.pyx":181
  * 
  *         kd_logger.info('calculating success...')
  *         return raw_data, self._format_mean(mean_data), dist_data             # <<<<<<<<<<<<<<
  * 
  *     def run(self, begin_date, end_date, threshold=0.9):
  */
   __Pyx_XDECREF(__pyx_r);
@@ -6616,55 +6616,55 @@
   __Pyx_GIVEREF(__pyx_v_dist_data);
   PyTuple_SET_ITEM(__pyx_t_3, 2, __pyx_v_dist_data);
   __pyx_t_2 = 0;
   __pyx_r = __pyx_t_3;
   __pyx_t_3 = 0;
   goto __pyx_L0;
 
-  /* "seleya/mfc/alchemy/qrank/glassdoor.py":153
+  /* "seleya/mfc/alchemy/qrank/glassdoor.pyx":153
  *         return mean_data
  * 
  *     def calculate_result(self, total_data, threshold=0.9):             # <<<<<<<<<<<<<<
  *         # aggregate means by year and cid
  *         mean_data = total_data.groupby(['date', 'code']).mean()
  */
 
   /* function exit code */
   __pyx_L1_error:;
   __Pyx_XDECREF(__pyx_t_1);
   __Pyx_XDECREF(__pyx_t_2);
   __Pyx_XDECREF(__pyx_t_3);
   __Pyx_XDECREF(__pyx_t_4);
   __Pyx_XDECREF(__pyx_t_5);
-  __Pyx_AddTraceback("seleya.mfc.alchemy.qrank.glassdoo.Glassdoor.calculate_result", __pyx_clineno, __pyx_lineno, __pyx_filename);
+  __Pyx_AddTraceback("seleya.mfc.alchemy.qrank.glassdoor.Glassdoor.calculate_result", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __pyx_r = NULL;
   __pyx_L0:;
   __Pyx_XDECREF(__pyx_v_mean_data);
   __Pyx_XDECREF(__pyx_v_raw_data);
   __Pyx_XDECREF(__pyx_v_col_score);
   __Pyx_XDECREF(__pyx_v_dist_data);
   __Pyx_DECREF(((PyObject *)__pyx_cur_scope));
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "seleya/mfc/alchemy/qrank/glassdoor.py":183
+/* "seleya/mfc/alchemy/qrank/glassdoor.pyx":183
  *         return raw_data, self._format_mean(mean_data), dist_data
  * 
  *     def run(self, begin_date, end_date, threshold=0.9):             # <<<<<<<<<<<<<<
  *         total_data = self.prepare_data(begin_date, end_date)
  *         if total_data is None or total_data.empty:
  */
 
 /* Python wrapper */
-static PyObject *__pyx_pw_6seleya_3mfc_7alchemy_5qrank_8glassdoo_9Glassdoor_23run(PyObject *__pyx_self, PyObject *__pyx_args, PyObject *__pyx_kwds); /*proto*/
-static char __pyx_doc_6seleya_3mfc_7alchemy_5qrank_8glassdoo_9Glassdoor_22run[] = "Glassdoor.run(self, begin_date, end_date, threshold=0.9)";
-static PyMethodDef __pyx_mdef_6seleya_3mfc_7alchemy_5qrank_8glassdoo_9Glassdoor_23run = {"run", (PyCFunction)(void*)(PyCFunctionWithKeywords)__pyx_pw_6seleya_3mfc_7alchemy_5qrank_8glassdoo_9Glassdoor_23run, METH_VARARGS|METH_KEYWORDS, __pyx_doc_6seleya_3mfc_7alchemy_5qrank_8glassdoo_9Glassdoor_22run};
-static PyObject *__pyx_pw_6seleya_3mfc_7alchemy_5qrank_8glassdoo_9Glassdoor_23run(PyObject *__pyx_self, PyObject *__pyx_args, PyObject *__pyx_kwds) {
+static PyObject *__pyx_pw_6seleya_3mfc_7alchemy_5qrank_9glassdoor_9Glassdoor_23run(PyObject *__pyx_self, PyObject *__pyx_args, PyObject *__pyx_kwds); /*proto*/
+static char __pyx_doc_6seleya_3mfc_7alchemy_5qrank_9glassdoor_9Glassdoor_22run[] = "Glassdoor.run(self, begin_date, end_date, threshold=0.9)";
+static PyMethodDef __pyx_mdef_6seleya_3mfc_7alchemy_5qrank_9glassdoor_9Glassdoor_23run = {"run", (PyCFunction)(void*)(PyCFunctionWithKeywords)__pyx_pw_6seleya_3mfc_7alchemy_5qrank_9glassdoor_9Glassdoor_23run, METH_VARARGS|METH_KEYWORDS, __pyx_doc_6seleya_3mfc_7alchemy_5qrank_9glassdoor_9Glassdoor_22run};
+static PyObject *__pyx_pw_6seleya_3mfc_7alchemy_5qrank_9glassdoor_9Glassdoor_23run(PyObject *__pyx_self, PyObject *__pyx_args, PyObject *__pyx_kwds) {
   PyObject *__pyx_v_self = 0;
   PyObject *__pyx_v_begin_date = 0;
   PyObject *__pyx_v_end_date = 0;
   PyObject *__pyx_v_threshold = 0;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
@@ -6733,26 +6733,26 @@
     __pyx_v_end_date = values[2];
     __pyx_v_threshold = values[3];
   }
   goto __pyx_L4_argument_unpacking_done;
   __pyx_L5_argtuple_error:;
   __Pyx_RaiseArgtupleInvalid("run", 0, 3, 4, PyTuple_GET_SIZE(__pyx_args)); __PYX_ERR(0, 183, __pyx_L3_error)
   __pyx_L3_error:;
-  __Pyx_AddTraceback("seleya.mfc.alchemy.qrank.glassdoo.Glassdoor.run", __pyx_clineno, __pyx_lineno, __pyx_filename);
+  __Pyx_AddTraceback("seleya.mfc.alchemy.qrank.glassdoor.Glassdoor.run", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __Pyx_RefNannyFinishContext();
   return NULL;
   __pyx_L4_argument_unpacking_done:;
-  __pyx_r = __pyx_pf_6seleya_3mfc_7alchemy_5qrank_8glassdoo_9Glassdoor_22run(__pyx_self, __pyx_v_self, __pyx_v_begin_date, __pyx_v_end_date, __pyx_v_threshold);
+  __pyx_r = __pyx_pf_6seleya_3mfc_7alchemy_5qrank_9glassdoor_9Glassdoor_22run(__pyx_self, __pyx_v_self, __pyx_v_begin_date, __pyx_v_end_date, __pyx_v_threshold);
 
   /* function exit code */
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-static PyObject *__pyx_pf_6seleya_3mfc_7alchemy_5qrank_8glassdoo_9Glassdoor_22run(CYTHON_UNUSED PyObject *__pyx_self, PyObject *__pyx_v_self, PyObject *__pyx_v_begin_date, PyObject *__pyx_v_end_date, PyObject *__pyx_v_threshold) {
+static PyObject *__pyx_pf_6seleya_3mfc_7alchemy_5qrank_9glassdoor_9Glassdoor_22run(CYTHON_UNUSED PyObject *__pyx_self, PyObject *__pyx_v_self, PyObject *__pyx_v_begin_date, PyObject *__pyx_v_end_date, PyObject *__pyx_v_threshold) {
   PyObject *__pyx_v_total_data = NULL;
   PyObject *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   PyObject *__pyx_t_2 = NULL;
   PyObject *__pyx_t_3 = NULL;
   int __pyx_t_4;
@@ -6761,15 +6761,15 @@
   int __pyx_t_7;
   int __pyx_t_8;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("run", 0);
 
-  /* "seleya/mfc/alchemy/qrank/glassdoor.py":184
+  /* "seleya/mfc/alchemy/qrank/glassdoor.pyx":184
  * 
  *     def run(self, begin_date, end_date, threshold=0.9):
  *         total_data = self.prepare_data(begin_date, end_date)             # <<<<<<<<<<<<<<
  *         if total_data is None or total_data.empty:
  *             kd_logger.error('Glassdoor data is empty')
  */
   __pyx_t_2 = __Pyx_PyObject_GetAttrStr(__pyx_v_self, __pyx_n_s_prepare_data); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 184, __pyx_L1_error)
@@ -6818,15 +6818,15 @@
     __Pyx_GOTREF(__pyx_t_1);
     __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
   }
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
   __pyx_v_total_data = __pyx_t_1;
   __pyx_t_1 = 0;
 
-  /* "seleya/mfc/alchemy/qrank/glassdoor.py":185
+  /* "seleya/mfc/alchemy/qrank/glassdoor.pyx":185
  *     def run(self, begin_date, end_date, threshold=0.9):
  *         total_data = self.prepare_data(begin_date, end_date)
  *         if total_data is None or total_data.empty:             # <<<<<<<<<<<<<<
  *             kd_logger.error('Glassdoor data is empty')
  *             return None
  */
   __pyx_t_7 = (__pyx_v_total_data == Py_None);
@@ -6840,15 +6840,15 @@
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_t_8 = __Pyx_PyObject_IsTrue(__pyx_t_1); if (unlikely(__pyx_t_8 < 0)) __PYX_ERR(0, 185, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   __pyx_t_6 = __pyx_t_8;
   __pyx_L4_bool_binop_done:;
   if (__pyx_t_6) {
 
-    /* "seleya/mfc/alchemy/qrank/glassdoor.py":186
+    /* "seleya/mfc/alchemy/qrank/glassdoor.pyx":186
  *         total_data = self.prepare_data(begin_date, end_date)
  *         if total_data is None or total_data.empty:
  *             kd_logger.error('Glassdoor data is empty')             # <<<<<<<<<<<<<<
  *             return None
  *         return self.calculate_result(total_data=total_data,
  */
     __Pyx_GetModuleGlobalName(__pyx_t_2, __pyx_n_s_kd_logger); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 186, __pyx_L1_error)
@@ -6869,143 +6869,143 @@
     __pyx_t_1 = (__pyx_t_2) ? __Pyx_PyObject_Call2Args(__pyx_t_5, __pyx_t_2, __pyx_kp_s_Glassdoor_data_is_empty) : __Pyx_PyObject_CallOneArg(__pyx_t_5, __pyx_kp_s_Glassdoor_data_is_empty);
     __Pyx_XDECREF(__pyx_t_2); __pyx_t_2 = 0;
     if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 186, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_1);
     __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
     __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
 
-    /* "seleya/mfc/alchemy/qrank/glassdoor.py":187
+    /* "seleya/mfc/alchemy/qrank/glassdoor.pyx":187
  *         if total_data is None or total_data.empty:
  *             kd_logger.error('Glassdoor data is empty')
  *             return None             # <<<<<<<<<<<<<<
  *         return self.calculate_result(total_data=total_data,
  *                                      threshold=threshold)
  */
     __Pyx_XDECREF(__pyx_r);
     __pyx_r = Py_None; __Pyx_INCREF(Py_None);
     goto __pyx_L0;
 
-    /* "seleya/mfc/alchemy/qrank/glassdoor.py":185
+    /* "seleya/mfc/alchemy/qrank/glassdoor.pyx":185
  *     def run(self, begin_date, end_date, threshold=0.9):
  *         total_data = self.prepare_data(begin_date, end_date)
  *         if total_data is None or total_data.empty:             # <<<<<<<<<<<<<<
  *             kd_logger.error('Glassdoor data is empty')
  *             return None
  */
   }
 
-  /* "seleya/mfc/alchemy/qrank/glassdoor.py":188
+  /* "seleya/mfc/alchemy/qrank/glassdoor.pyx":188
  *             kd_logger.error('Glassdoor data is empty')
  *             return None
  *         return self.calculate_result(total_data=total_data,             # <<<<<<<<<<<<<<
  *                                      threshold=threshold)
  */
   __Pyx_XDECREF(__pyx_r);
   __pyx_t_1 = __Pyx_PyObject_GetAttrStr(__pyx_v_self, __pyx_n_s_calculate_result); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 188, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_t_5 = __Pyx_PyDict_NewPresized(2); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 188, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_5);
   if (PyDict_SetItem(__pyx_t_5, __pyx_n_s_total_data, __pyx_v_total_data) < 0) __PYX_ERR(0, 188, __pyx_L1_error)
 
-  /* "seleya/mfc/alchemy/qrank/glassdoor.py":189
+  /* "seleya/mfc/alchemy/qrank/glassdoor.pyx":189
  *             return None
  *         return self.calculate_result(total_data=total_data,
  *                                      threshold=threshold)             # <<<<<<<<<<<<<<
  */
   if (PyDict_SetItem(__pyx_t_5, __pyx_n_s_threshold, __pyx_v_threshold) < 0) __PYX_ERR(0, 188, __pyx_L1_error)
 
-  /* "seleya/mfc/alchemy/qrank/glassdoor.py":188
+  /* "seleya/mfc/alchemy/qrank/glassdoor.pyx":188
  *             kd_logger.error('Glassdoor data is empty')
  *             return None
  *         return self.calculate_result(total_data=total_data,             # <<<<<<<<<<<<<<
  *                                      threshold=threshold)
  */
   __pyx_t_2 = __Pyx_PyObject_Call(__pyx_t_1, __pyx_empty_tuple, __pyx_t_5); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 188, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
   __pyx_r = __pyx_t_2;
   __pyx_t_2 = 0;
   goto __pyx_L0;
 
-  /* "seleya/mfc/alchemy/qrank/glassdoor.py":183
+  /* "seleya/mfc/alchemy/qrank/glassdoor.pyx":183
  *         return raw_data, self._format_mean(mean_data), dist_data
  * 
  *     def run(self, begin_date, end_date, threshold=0.9):             # <<<<<<<<<<<<<<
  *         total_data = self.prepare_data(begin_date, end_date)
  *         if total_data is None or total_data.empty:
  */
 
   /* function exit code */
   __pyx_L1_error:;
   __Pyx_XDECREF(__pyx_t_1);
   __Pyx_XDECREF(__pyx_t_2);
   __Pyx_XDECREF(__pyx_t_3);
   __Pyx_XDECREF(__pyx_t_5);
-  __Pyx_AddTraceback("seleya.mfc.alchemy.qrank.glassdoo.Glassdoor.run", __pyx_clineno, __pyx_lineno, __pyx_filename);
+  __Pyx_AddTraceback("seleya.mfc.alchemy.qrank.glassdoor.Glassdoor.run", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __pyx_r = NULL;
   __pyx_L0:;
   __Pyx_XDECREF(__pyx_v_total_data);
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-static struct __pyx_obj_6seleya_3mfc_7alchemy_5qrank_8glassdoo___pyx_scope_struct___fetch_reviews *__pyx_freelist_6seleya_3mfc_7alchemy_5qrank_8glassdoo___pyx_scope_struct___fetch_reviews[8];
-static int __pyx_freecount_6seleya_3mfc_7alchemy_5qrank_8glassdoo___pyx_scope_struct___fetch_reviews = 0;
+static struct __pyx_obj_6seleya_3mfc_7alchemy_5qrank_9glassdoor___pyx_scope_struct___fetch_reviews *__pyx_freelist_6seleya_3mfc_7alchemy_5qrank_9glassdoor___pyx_scope_struct___fetch_reviews[8];
+static int __pyx_freecount_6seleya_3mfc_7alchemy_5qrank_9glassdoor___pyx_scope_struct___fetch_reviews = 0;
 
-static PyObject *__pyx_tp_new_6seleya_3mfc_7alchemy_5qrank_8glassdoo___pyx_scope_struct___fetch_reviews(PyTypeObject *t, CYTHON_UNUSED PyObject *a, CYTHON_UNUSED PyObject *k) {
+static PyObject *__pyx_tp_new_6seleya_3mfc_7alchemy_5qrank_9glassdoor___pyx_scope_struct___fetch_reviews(PyTypeObject *t, CYTHON_UNUSED PyObject *a, CYTHON_UNUSED PyObject *k) {
   PyObject *o;
-  if (CYTHON_COMPILING_IN_CPYTHON && likely((__pyx_freecount_6seleya_3mfc_7alchemy_5qrank_8glassdoo___pyx_scope_struct___fetch_reviews > 0) & (t->tp_basicsize == sizeof(struct __pyx_obj_6seleya_3mfc_7alchemy_5qrank_8glassdoo___pyx_scope_struct___fetch_reviews)))) {
-    o = (PyObject*)__pyx_freelist_6seleya_3mfc_7alchemy_5qrank_8glassdoo___pyx_scope_struct___fetch_reviews[--__pyx_freecount_6seleya_3mfc_7alchemy_5qrank_8glassdoo___pyx_scope_struct___fetch_reviews];
-    memset(o, 0, sizeof(struct __pyx_obj_6seleya_3mfc_7alchemy_5qrank_8glassdoo___pyx_scope_struct___fetch_reviews));
+  if (CYTHON_COMPILING_IN_CPYTHON && likely((__pyx_freecount_6seleya_3mfc_7alchemy_5qrank_9glassdoor___pyx_scope_struct___fetch_reviews > 0) & (t->tp_basicsize == sizeof(struct __pyx_obj_6seleya_3mfc_7alchemy_5qrank_9glassdoor___pyx_scope_struct___fetch_reviews)))) {
+    o = (PyObject*)__pyx_freelist_6seleya_3mfc_7alchemy_5qrank_9glassdoor___pyx_scope_struct___fetch_reviews[--__pyx_freecount_6seleya_3mfc_7alchemy_5qrank_9glassdoor___pyx_scope_struct___fetch_reviews];
+    memset(o, 0, sizeof(struct __pyx_obj_6seleya_3mfc_7alchemy_5qrank_9glassdoor___pyx_scope_struct___fetch_reviews));
     (void) PyObject_INIT(o, t);
     PyObject_GC_Track(o);
   } else {
     o = (*t->tp_alloc)(t, 0);
     if (unlikely(!o)) return 0;
   }
   return o;
 }
 
-static void __pyx_tp_dealloc_6seleya_3mfc_7alchemy_5qrank_8glassdoo___pyx_scope_struct___fetch_reviews(PyObject *o) {
-  struct __pyx_obj_6seleya_3mfc_7alchemy_5qrank_8glassdoo___pyx_scope_struct___fetch_reviews *p = (struct __pyx_obj_6seleya_3mfc_7alchemy_5qrank_8glassdoo___pyx_scope_struct___fetch_reviews *)o;
+static void __pyx_tp_dealloc_6seleya_3mfc_7alchemy_5qrank_9glassdoor___pyx_scope_struct___fetch_reviews(PyObject *o) {
+  struct __pyx_obj_6seleya_3mfc_7alchemy_5qrank_9glassdoor___pyx_scope_struct___fetch_reviews *p = (struct __pyx_obj_6seleya_3mfc_7alchemy_5qrank_9glassdoor___pyx_scope_struct___fetch_reviews *)o;
   PyObject_GC_UnTrack(o);
   Py_CLEAR(p->__pyx_v_self);
-  if (CYTHON_COMPILING_IN_CPYTHON && ((__pyx_freecount_6seleya_3mfc_7alchemy_5qrank_8glassdoo___pyx_scope_struct___fetch_reviews < 8) & (Py_TYPE(o)->tp_basicsize == sizeof(struct __pyx_obj_6seleya_3mfc_7alchemy_5qrank_8glassdoo___pyx_scope_struct___fetch_reviews)))) {
-    __pyx_freelist_6seleya_3mfc_7alchemy_5qrank_8glassdoo___pyx_scope_struct___fetch_reviews[__pyx_freecount_6seleya_3mfc_7alchemy_5qrank_8glassdoo___pyx_scope_struct___fetch_reviews++] = ((struct __pyx_obj_6seleya_3mfc_7alchemy_5qrank_8glassdoo___pyx_scope_struct___fetch_reviews *)o);
+  if (CYTHON_COMPILING_IN_CPYTHON && ((__pyx_freecount_6seleya_3mfc_7alchemy_5qrank_9glassdoor___pyx_scope_struct___fetch_reviews < 8) & (Py_TYPE(o)->tp_basicsize == sizeof(struct __pyx_obj_6seleya_3mfc_7alchemy_5qrank_9glassdoor___pyx_scope_struct___fetch_reviews)))) {
+    __pyx_freelist_6seleya_3mfc_7alchemy_5qrank_9glassdoor___pyx_scope_struct___fetch_reviews[__pyx_freecount_6seleya_3mfc_7alchemy_5qrank_9glassdoor___pyx_scope_struct___fetch_reviews++] = ((struct __pyx_obj_6seleya_3mfc_7alchemy_5qrank_9glassdoor___pyx_scope_struct___fetch_reviews *)o);
   } else {
     (*Py_TYPE(o)->tp_free)(o);
   }
 }
 
-static int __pyx_tp_traverse_6seleya_3mfc_7alchemy_5qrank_8glassdoo___pyx_scope_struct___fetch_reviews(PyObject *o, visitproc v, void *a) {
+static int __pyx_tp_traverse_6seleya_3mfc_7alchemy_5qrank_9glassdoor___pyx_scope_struct___fetch_reviews(PyObject *o, visitproc v, void *a) {
   int e;
-  struct __pyx_obj_6seleya_3mfc_7alchemy_5qrank_8glassdoo___pyx_scope_struct___fetch_reviews *p = (struct __pyx_obj_6seleya_3mfc_7alchemy_5qrank_8glassdoo___pyx_scope_struct___fetch_reviews *)o;
+  struct __pyx_obj_6seleya_3mfc_7alchemy_5qrank_9glassdoor___pyx_scope_struct___fetch_reviews *p = (struct __pyx_obj_6seleya_3mfc_7alchemy_5qrank_9glassdoor___pyx_scope_struct___fetch_reviews *)o;
   if (p->__pyx_v_self) {
     e = (*v)(p->__pyx_v_self, a); if (e) return e;
   }
   return 0;
 }
 
-static int __pyx_tp_clear_6seleya_3mfc_7alchemy_5qrank_8glassdoo___pyx_scope_struct___fetch_reviews(PyObject *o) {
+static int __pyx_tp_clear_6seleya_3mfc_7alchemy_5qrank_9glassdoor___pyx_scope_struct___fetch_reviews(PyObject *o) {
   PyObject* tmp;
-  struct __pyx_obj_6seleya_3mfc_7alchemy_5qrank_8glassdoo___pyx_scope_struct___fetch_reviews *p = (struct __pyx_obj_6seleya_3mfc_7alchemy_5qrank_8glassdoo___pyx_scope_struct___fetch_reviews *)o;
+  struct __pyx_obj_6seleya_3mfc_7alchemy_5qrank_9glassdoor___pyx_scope_struct___fetch_reviews *p = (struct __pyx_obj_6seleya_3mfc_7alchemy_5qrank_9glassdoor___pyx_scope_struct___fetch_reviews *)o;
   tmp = ((PyObject*)p->__pyx_v_self);
   p->__pyx_v_self = Py_None; Py_INCREF(Py_None);
   Py_XDECREF(tmp);
   return 0;
 }
 
-static PyTypeObject __pyx_type_6seleya_3mfc_7alchemy_5qrank_8glassdoo___pyx_scope_struct___fetch_reviews = {
+static PyTypeObject __pyx_type_6seleya_3mfc_7alchemy_5qrank_9glassdoor___pyx_scope_struct___fetch_reviews = {
   PyVarObject_HEAD_INIT(0, 0)
-  "seleya.mfc.alchemy.qrank.glassdoo.__pyx_scope_struct___fetch_reviews", /*tp_name*/
-  sizeof(struct __pyx_obj_6seleya_3mfc_7alchemy_5qrank_8glassdoo___pyx_scope_struct___fetch_reviews), /*tp_basicsize*/
+  "seleya.mfc.alchemy.qrank.glassdoor.__pyx_scope_struct___fetch_reviews", /*tp_name*/
+  sizeof(struct __pyx_obj_6seleya_3mfc_7alchemy_5qrank_9glassdoor___pyx_scope_struct___fetch_reviews), /*tp_basicsize*/
   0, /*tp_itemsize*/
-  __pyx_tp_dealloc_6seleya_3mfc_7alchemy_5qrank_8glassdoo___pyx_scope_struct___fetch_reviews, /*tp_dealloc*/
+  __pyx_tp_dealloc_6seleya_3mfc_7alchemy_5qrank_9glassdoor___pyx_scope_struct___fetch_reviews, /*tp_dealloc*/
   #if PY_VERSION_HEX < 0x030800b4
   0, /*tp_print*/
   #endif
   #if PY_VERSION_HEX >= 0x030800b4
   0, /*tp_vectorcall_offset*/
   #endif
   0, /*tp_getattr*/
@@ -7024,31 +7024,31 @@
   0, /*tp_call*/
   0, /*tp_str*/
   0, /*tp_getattro*/
   0, /*tp_setattro*/
   0, /*tp_as_buffer*/
   Py_TPFLAGS_DEFAULT|Py_TPFLAGS_HAVE_VERSION_TAG|Py_TPFLAGS_CHECKTYPES|Py_TPFLAGS_HAVE_NEWBUFFER|Py_TPFLAGS_HAVE_GC, /*tp_flags*/
   0, /*tp_doc*/
-  __pyx_tp_traverse_6seleya_3mfc_7alchemy_5qrank_8glassdoo___pyx_scope_struct___fetch_reviews, /*tp_traverse*/
-  __pyx_tp_clear_6seleya_3mfc_7alchemy_5qrank_8glassdoo___pyx_scope_struct___fetch_reviews, /*tp_clear*/
+  __pyx_tp_traverse_6seleya_3mfc_7alchemy_5qrank_9glassdoor___pyx_scope_struct___fetch_reviews, /*tp_traverse*/
+  __pyx_tp_clear_6seleya_3mfc_7alchemy_5qrank_9glassdoor___pyx_scope_struct___fetch_reviews, /*tp_clear*/
   0, /*tp_richcompare*/
   0, /*tp_weaklistoffset*/
   0, /*tp_iter*/
   0, /*tp_iternext*/
   0, /*tp_methods*/
   0, /*tp_members*/
   0, /*tp_getset*/
   0, /*tp_base*/
   0, /*tp_dict*/
   0, /*tp_descr_get*/
   0, /*tp_descr_set*/
   0, /*tp_dictoffset*/
   0, /*tp_init*/
   0, /*tp_alloc*/
-  __pyx_tp_new_6seleya_3mfc_7alchemy_5qrank_8glassdoo___pyx_scope_struct___fetch_reviews, /*tp_new*/
+  __pyx_tp_new_6seleya_3mfc_7alchemy_5qrank_9glassdoor___pyx_scope_struct___fetch_reviews, /*tp_new*/
   0, /*tp_free*/
   0, /*tp_is_gc*/
   0, /*tp_bases*/
   0, /*tp_mro*/
   0, /*tp_cache*/
   0, /*tp_subclasses*/
   0, /*tp_weaklist*/
@@ -7061,73 +7061,73 @@
   0, /*tp_vectorcall*/
   #endif
   #if PY_VERSION_HEX >= 0x030800b4 && PY_VERSION_HEX < 0x03090000
   0, /*tp_print*/
   #endif
 };
 
-static struct __pyx_obj_6seleya_3mfc_7alchemy_5qrank_8glassdoo___pyx_scope_struct_1__distribute *__pyx_freelist_6seleya_3mfc_7alchemy_5qrank_8glassdoo___pyx_scope_struct_1__distribute[8];
-static int __pyx_freecount_6seleya_3mfc_7alchemy_5qrank_8glassdoo___pyx_scope_struct_1__distribute = 0;
+static struct __pyx_obj_6seleya_3mfc_7alchemy_5qrank_9glassdoor___pyx_scope_struct_1__distribute *__pyx_freelist_6seleya_3mfc_7alchemy_5qrank_9glassdoor___pyx_scope_struct_1__distribute[8];
+static int __pyx_freecount_6seleya_3mfc_7alchemy_5qrank_9glassdoor___pyx_scope_struct_1__distribute = 0;
 
-static PyObject *__pyx_tp_new_6seleya_3mfc_7alchemy_5qrank_8glassdoo___pyx_scope_struct_1__distribute(PyTypeObject *t, CYTHON_UNUSED PyObject *a, CYTHON_UNUSED PyObject *k) {
+static PyObject *__pyx_tp_new_6seleya_3mfc_7alchemy_5qrank_9glassdoor___pyx_scope_struct_1__distribute(PyTypeObject *t, CYTHON_UNUSED PyObject *a, CYTHON_UNUSED PyObject *k) {
   PyObject *o;
-  if (CYTHON_COMPILING_IN_CPYTHON && likely((__pyx_freecount_6seleya_3mfc_7alchemy_5qrank_8glassdoo___pyx_scope_struct_1__distribute > 0) & (t->tp_basicsize == sizeof(struct __pyx_obj_6seleya_3mfc_7alchemy_5qrank_8glassdoo___pyx_scope_struct_1__distribute)))) {
-    o = (PyObject*)__pyx_freelist_6seleya_3mfc_7alchemy_5qrank_8glassdoo___pyx_scope_struct_1__distribute[--__pyx_freecount_6seleya_3mfc_7alchemy_5qrank_8glassdoo___pyx_scope_struct_1__distribute];
-    memset(o, 0, sizeof(struct __pyx_obj_6seleya_3mfc_7alchemy_5qrank_8glassdoo___pyx_scope_struct_1__distribute));
+  if (CYTHON_COMPILING_IN_CPYTHON && likely((__pyx_freecount_6seleya_3mfc_7alchemy_5qrank_9glassdoor___pyx_scope_struct_1__distribute > 0) & (t->tp_basicsize == sizeof(struct __pyx_obj_6seleya_3mfc_7alchemy_5qrank_9glassdoor___pyx_scope_struct_1__distribute)))) {
+    o = (PyObject*)__pyx_freelist_6seleya_3mfc_7alchemy_5qrank_9glassdoor___pyx_scope_struct_1__distribute[--__pyx_freecount_6seleya_3mfc_7alchemy_5qrank_9glassdoor___pyx_scope_struct_1__distribute];
+    memset(o, 0, sizeof(struct __pyx_obj_6seleya_3mfc_7alchemy_5qrank_9glassdoor___pyx_scope_struct_1__distribute));
     (void) PyObject_INIT(o, t);
     PyObject_GC_Track(o);
   } else {
     o = (*t->tp_alloc)(t, 0);
     if (unlikely(!o)) return 0;
   }
   return o;
 }
 
-static void __pyx_tp_dealloc_6seleya_3mfc_7alchemy_5qrank_8glassdoo___pyx_scope_struct_1__distribute(PyObject *o) {
-  struct __pyx_obj_6seleya_3mfc_7alchemy_5qrank_8glassdoo___pyx_scope_struct_1__distribute *p = (struct __pyx_obj_6seleya_3mfc_7alchemy_5qrank_8glassdoo___pyx_scope_struct_1__distribute *)o;
+static void __pyx_tp_dealloc_6seleya_3mfc_7alchemy_5qrank_9glassdoor___pyx_scope_struct_1__distribute(PyObject *o) {
+  struct __pyx_obj_6seleya_3mfc_7alchemy_5qrank_9glassdoor___pyx_scope_struct_1__distribute *p = (struct __pyx_obj_6seleya_3mfc_7alchemy_5qrank_9glassdoor___pyx_scope_struct_1__distribute *)o;
   PyObject_GC_UnTrack(o);
   Py_CLEAR(p->__pyx_v_res);
   Py_CLEAR(p->__pyx_v_self);
-  if (CYTHON_COMPILING_IN_CPYTHON && ((__pyx_freecount_6seleya_3mfc_7alchemy_5qrank_8glassdoo___pyx_scope_struct_1__distribute < 8) & (Py_TYPE(o)->tp_basicsize == sizeof(struct __pyx_obj_6seleya_3mfc_7alchemy_5qrank_8glassdoo___pyx_scope_struct_1__distribute)))) {
-    __pyx_freelist_6seleya_3mfc_7alchemy_5qrank_8glassdoo___pyx_scope_struct_1__distribute[__pyx_freecount_6seleya_3mfc_7alchemy_5qrank_8glassdoo___pyx_scope_struct_1__distribute++] = ((struct __pyx_obj_6seleya_3mfc_7alchemy_5qrank_8glassdoo___pyx_scope_struct_1__distribute *)o);
+  if (CYTHON_COMPILING_IN_CPYTHON && ((__pyx_freecount_6seleya_3mfc_7alchemy_5qrank_9glassdoor___pyx_scope_struct_1__distribute < 8) & (Py_TYPE(o)->tp_basicsize == sizeof(struct __pyx_obj_6seleya_3mfc_7alchemy_5qrank_9glassdoor___pyx_scope_struct_1__distribute)))) {
+    __pyx_freelist_6seleya_3mfc_7alchemy_5qrank_9glassdoor___pyx_scope_struct_1__distribute[__pyx_freecount_6seleya_3mfc_7alchemy_5qrank_9glassdoor___pyx_scope_struct_1__distribute++] = ((struct __pyx_obj_6seleya_3mfc_7alchemy_5qrank_9glassdoor___pyx_scope_struct_1__distribute *)o);
   } else {
     (*Py_TYPE(o)->tp_free)(o);
   }
 }
 
-static int __pyx_tp_traverse_6seleya_3mfc_7alchemy_5qrank_8glassdoo___pyx_scope_struct_1__distribute(PyObject *o, visitproc v, void *a) {
+static int __pyx_tp_traverse_6seleya_3mfc_7alchemy_5qrank_9glassdoor___pyx_scope_struct_1__distribute(PyObject *o, visitproc v, void *a) {
   int e;
-  struct __pyx_obj_6seleya_3mfc_7alchemy_5qrank_8glassdoo___pyx_scope_struct_1__distribute *p = (struct __pyx_obj_6seleya_3mfc_7alchemy_5qrank_8glassdoo___pyx_scope_struct_1__distribute *)o;
+  struct __pyx_obj_6seleya_3mfc_7alchemy_5qrank_9glassdoor___pyx_scope_struct_1__distribute *p = (struct __pyx_obj_6seleya_3mfc_7alchemy_5qrank_9glassdoor___pyx_scope_struct_1__distribute *)o;
   if (p->__pyx_v_res) {
     e = (*v)(p->__pyx_v_res, a); if (e) return e;
   }
   if (p->__pyx_v_self) {
     e = (*v)(p->__pyx_v_self, a); if (e) return e;
   }
   return 0;
 }
 
-static int __pyx_tp_clear_6seleya_3mfc_7alchemy_5qrank_8glassdoo___pyx_scope_struct_1__distribute(PyObject *o) {
+static int __pyx_tp_clear_6seleya_3mfc_7alchemy_5qrank_9glassdoor___pyx_scope_struct_1__distribute(PyObject *o) {
   PyObject* tmp;
-  struct __pyx_obj_6seleya_3mfc_7alchemy_5qrank_8glassdoo___pyx_scope_struct_1__distribute *p = (struct __pyx_obj_6seleya_3mfc_7alchemy_5qrank_8glassdoo___pyx_scope_struct_1__distribute *)o;
+  struct __pyx_obj_6seleya_3mfc_7alchemy_5qrank_9glassdoor___pyx_scope_struct_1__distribute *p = (struct __pyx_obj_6seleya_3mfc_7alchemy_5qrank_9glassdoor___pyx_scope_struct_1__distribute *)o;
   tmp = ((PyObject*)p->__pyx_v_res);
   p->__pyx_v_res = ((PyObject*)Py_None); Py_INCREF(Py_None);
   Py_XDECREF(tmp);
   tmp = ((PyObject*)p->__pyx_v_self);
   p->__pyx_v_self = Py_None; Py_INCREF(Py_None);
   Py_XDECREF(tmp);
   return 0;
 }
 
-static PyTypeObject __pyx_type_6seleya_3mfc_7alchemy_5qrank_8glassdoo___pyx_scope_struct_1__distribute = {
+static PyTypeObject __pyx_type_6seleya_3mfc_7alchemy_5qrank_9glassdoor___pyx_scope_struct_1__distribute = {
   PyVarObject_HEAD_INIT(0, 0)
-  "seleya.mfc.alchemy.qrank.glassdoo.__pyx_scope_struct_1__distribute", /*tp_name*/
-  sizeof(struct __pyx_obj_6seleya_3mfc_7alchemy_5qrank_8glassdoo___pyx_scope_struct_1__distribute), /*tp_basicsize*/
+  "seleya.mfc.alchemy.qrank.glassdoor.__pyx_scope_struct_1__distribute", /*tp_name*/
+  sizeof(struct __pyx_obj_6seleya_3mfc_7alchemy_5qrank_9glassdoor___pyx_scope_struct_1__distribute), /*tp_basicsize*/
   0, /*tp_itemsize*/
-  __pyx_tp_dealloc_6seleya_3mfc_7alchemy_5qrank_8glassdoo___pyx_scope_struct_1__distribute, /*tp_dealloc*/
+  __pyx_tp_dealloc_6seleya_3mfc_7alchemy_5qrank_9glassdoor___pyx_scope_struct_1__distribute, /*tp_dealloc*/
   #if PY_VERSION_HEX < 0x030800b4
   0, /*tp_print*/
   #endif
   #if PY_VERSION_HEX >= 0x030800b4
   0, /*tp_vectorcall_offset*/
   #endif
   0, /*tp_getattr*/
@@ -7146,31 +7146,31 @@
   0, /*tp_call*/
   0, /*tp_str*/
   0, /*tp_getattro*/
   0, /*tp_setattro*/
   0, /*tp_as_buffer*/
   Py_TPFLAGS_DEFAULT|Py_TPFLAGS_HAVE_VERSION_TAG|Py_TPFLAGS_CHECKTYPES|Py_TPFLAGS_HAVE_NEWBUFFER|Py_TPFLAGS_HAVE_GC, /*tp_flags*/
   0, /*tp_doc*/
-  __pyx_tp_traverse_6seleya_3mfc_7alchemy_5qrank_8glassdoo___pyx_scope_struct_1__distribute, /*tp_traverse*/
-  __pyx_tp_clear_6seleya_3mfc_7alchemy_5qrank_8glassdoo___pyx_scope_struct_1__distribute, /*tp_clear*/
+  __pyx_tp_traverse_6seleya_3mfc_7alchemy_5qrank_9glassdoor___pyx_scope_struct_1__distribute, /*tp_traverse*/
+  __pyx_tp_clear_6seleya_3mfc_7alchemy_5qrank_9glassdoor___pyx_scope_struct_1__distribute, /*tp_clear*/
   0, /*tp_richcompare*/
   0, /*tp_weaklistoffset*/
   0, /*tp_iter*/
   0, /*tp_iternext*/
   0, /*tp_methods*/
   0, /*tp_members*/
   0, /*tp_getset*/
   0, /*tp_base*/
   0, /*tp_dict*/
   0, /*tp_descr_get*/
   0, /*tp_descr_set*/
   0, /*tp_dictoffset*/
   0, /*tp_init*/
   0, /*tp_alloc*/
-  __pyx_tp_new_6seleya_3mfc_7alchemy_5qrank_8glassdoo___pyx_scope_struct_1__distribute, /*tp_new*/
+  __pyx_tp_new_6seleya_3mfc_7alchemy_5qrank_9glassdoor___pyx_scope_struct_1__distribute, /*tp_new*/
   0, /*tp_free*/
   0, /*tp_is_gc*/
   0, /*tp_bases*/
   0, /*tp_mro*/
   0, /*tp_cache*/
   0, /*tp_subclasses*/
   0, /*tp_weaklist*/
@@ -7183,80 +7183,80 @@
   0, /*tp_vectorcall*/
   #endif
   #if PY_VERSION_HEX >= 0x030800b4 && PY_VERSION_HEX < 0x03090000
   0, /*tp_print*/
   #endif
 };
 
-static struct __pyx_obj_6seleya_3mfc_7alchemy_5qrank_8glassdoo___pyx_scope_struct_2_calculate_result *__pyx_freelist_6seleya_3mfc_7alchemy_5qrank_8glassdoo___pyx_scope_struct_2_calculate_result[8];
-static int __pyx_freecount_6seleya_3mfc_7alchemy_5qrank_8glassdoo___pyx_scope_struct_2_calculate_result = 0;
+static struct __pyx_obj_6seleya_3mfc_7alchemy_5qrank_9glassdoor___pyx_scope_struct_2_calculate_result *__pyx_freelist_6seleya_3mfc_7alchemy_5qrank_9glassdoor___pyx_scope_struct_2_calculate_result[8];
+static int __pyx_freecount_6seleya_3mfc_7alchemy_5qrank_9glassdoor___pyx_scope_struct_2_calculate_result = 0;
 
-static PyObject *__pyx_tp_new_6seleya_3mfc_7alchemy_5qrank_8glassdoo___pyx_scope_struct_2_calculate_result(PyTypeObject *t, CYTHON_UNUSED PyObject *a, CYTHON_UNUSED PyObject *k) {
+static PyObject *__pyx_tp_new_6seleya_3mfc_7alchemy_5qrank_9glassdoor___pyx_scope_struct_2_calculate_result(PyTypeObject *t, CYTHON_UNUSED PyObject *a, CYTHON_UNUSED PyObject *k) {
   PyObject *o;
-  if (CYTHON_COMPILING_IN_CPYTHON && likely((__pyx_freecount_6seleya_3mfc_7alchemy_5qrank_8glassdoo___pyx_scope_struct_2_calculate_result > 0) & (t->tp_basicsize == sizeof(struct __pyx_obj_6seleya_3mfc_7alchemy_5qrank_8glassdoo___pyx_scope_struct_2_calculate_result)))) {
-    o = (PyObject*)__pyx_freelist_6seleya_3mfc_7alchemy_5qrank_8glassdoo___pyx_scope_struct_2_calculate_result[--__pyx_freecount_6seleya_3mfc_7alchemy_5qrank_8glassdoo___pyx_scope_struct_2_calculate_result];
-    memset(o, 0, sizeof(struct __pyx_obj_6seleya_3mfc_7alchemy_5qrank_8glassdoo___pyx_scope_struct_2_calculate_result));
+  if (CYTHON_COMPILING_IN_CPYTHON && likely((__pyx_freecount_6seleya_3mfc_7alchemy_5qrank_9glassdoor___pyx_scope_struct_2_calculate_result > 0) & (t->tp_basicsize == sizeof(struct __pyx_obj_6seleya_3mfc_7alchemy_5qrank_9glassdoor___pyx_scope_struct_2_calculate_result)))) {
+    o = (PyObject*)__pyx_freelist_6seleya_3mfc_7alchemy_5qrank_9glassdoor___pyx_scope_struct_2_calculate_result[--__pyx_freecount_6seleya_3mfc_7alchemy_5qrank_9glassdoor___pyx_scope_struct_2_calculate_result];
+    memset(o, 0, sizeof(struct __pyx_obj_6seleya_3mfc_7alchemy_5qrank_9glassdoor___pyx_scope_struct_2_calculate_result));
     (void) PyObject_INIT(o, t);
     PyObject_GC_Track(o);
   } else {
     o = (*t->tp_alloc)(t, 0);
     if (unlikely(!o)) return 0;
   }
   return o;
 }
 
-static void __pyx_tp_dealloc_6seleya_3mfc_7alchemy_5qrank_8glassdoo___pyx_scope_struct_2_calculate_result(PyObject *o) {
-  struct __pyx_obj_6seleya_3mfc_7alchemy_5qrank_8glassdoo___pyx_scope_struct_2_calculate_result *p = (struct __pyx_obj_6seleya_3mfc_7alchemy_5qrank_8glassdoo___pyx_scope_struct_2_calculate_result *)o;
+static void __pyx_tp_dealloc_6seleya_3mfc_7alchemy_5qrank_9glassdoor___pyx_scope_struct_2_calculate_result(PyObject *o) {
+  struct __pyx_obj_6seleya_3mfc_7alchemy_5qrank_9glassdoor___pyx_scope_struct_2_calculate_result *p = (struct __pyx_obj_6seleya_3mfc_7alchemy_5qrank_9glassdoor___pyx_scope_struct_2_calculate_result *)o;
   PyObject_GC_UnTrack(o);
   Py_CLEAR(p->__pyx_v_col_name);
   Py_CLEAR(p->__pyx_v_self);
   Py_CLEAR(p->__pyx_v_threshold);
-  if (CYTHON_COMPILING_IN_CPYTHON && ((__pyx_freecount_6seleya_3mfc_7alchemy_5qrank_8glassdoo___pyx_scope_struct_2_calculate_result < 8) & (Py_TYPE(o)->tp_basicsize == sizeof(struct __pyx_obj_6seleya_3mfc_7alchemy_5qrank_8glassdoo___pyx_scope_struct_2_calculate_result)))) {
-    __pyx_freelist_6seleya_3mfc_7alchemy_5qrank_8glassdoo___pyx_scope_struct_2_calculate_result[__pyx_freecount_6seleya_3mfc_7alchemy_5qrank_8glassdoo___pyx_scope_struct_2_calculate_result++] = ((struct __pyx_obj_6seleya_3mfc_7alchemy_5qrank_8glassdoo___pyx_scope_struct_2_calculate_result *)o);
+  if (CYTHON_COMPILING_IN_CPYTHON && ((__pyx_freecount_6seleya_3mfc_7alchemy_5qrank_9glassdoor___pyx_scope_struct_2_calculate_result < 8) & (Py_TYPE(o)->tp_basicsize == sizeof(struct __pyx_obj_6seleya_3mfc_7alchemy_5qrank_9glassdoor___pyx_scope_struct_2_calculate_result)))) {
+    __pyx_freelist_6seleya_3mfc_7alchemy_5qrank_9glassdoor___pyx_scope_struct_2_calculate_result[__pyx_freecount_6seleya_3mfc_7alchemy_5qrank_9glassdoor___pyx_scope_struct_2_calculate_result++] = ((struct __pyx_obj_6seleya_3mfc_7alchemy_5qrank_9glassdoor___pyx_scope_struct_2_calculate_result *)o);
   } else {
     (*Py_TYPE(o)->tp_free)(o);
   }
 }
 
-static int __pyx_tp_traverse_6seleya_3mfc_7alchemy_5qrank_8glassdoo___pyx_scope_struct_2_calculate_result(PyObject *o, visitproc v, void *a) {
+static int __pyx_tp_traverse_6seleya_3mfc_7alchemy_5qrank_9glassdoor___pyx_scope_struct_2_calculate_result(PyObject *o, visitproc v, void *a) {
   int e;
-  struct __pyx_obj_6seleya_3mfc_7alchemy_5qrank_8glassdoo___pyx_scope_struct_2_calculate_result *p = (struct __pyx_obj_6seleya_3mfc_7alchemy_5qrank_8glassdoo___pyx_scope_struct_2_calculate_result *)o;
+  struct __pyx_obj_6seleya_3mfc_7alchemy_5qrank_9glassdoor___pyx_scope_struct_2_calculate_result *p = (struct __pyx_obj_6seleya_3mfc_7alchemy_5qrank_9glassdoor___pyx_scope_struct_2_calculate_result *)o;
   if (p->__pyx_v_col_name) {
     e = (*v)(p->__pyx_v_col_name, a); if (e) return e;
   }
   if (p->__pyx_v_self) {
     e = (*v)(p->__pyx_v_self, a); if (e) return e;
   }
   if (p->__pyx_v_threshold) {
     e = (*v)(p->__pyx_v_threshold, a); if (e) return e;
   }
   return 0;
 }
 
-static int __pyx_tp_clear_6seleya_3mfc_7alchemy_5qrank_8glassdoo___pyx_scope_struct_2_calculate_result(PyObject *o) {
+static int __pyx_tp_clear_6seleya_3mfc_7alchemy_5qrank_9glassdoor___pyx_scope_struct_2_calculate_result(PyObject *o) {
   PyObject* tmp;
-  struct __pyx_obj_6seleya_3mfc_7alchemy_5qrank_8glassdoo___pyx_scope_struct_2_calculate_result *p = (struct __pyx_obj_6seleya_3mfc_7alchemy_5qrank_8glassdoo___pyx_scope_struct_2_calculate_result *)o;
+  struct __pyx_obj_6seleya_3mfc_7alchemy_5qrank_9glassdoor___pyx_scope_struct_2_calculate_result *p = (struct __pyx_obj_6seleya_3mfc_7alchemy_5qrank_9glassdoor___pyx_scope_struct_2_calculate_result *)o;
   tmp = ((PyObject*)p->__pyx_v_col_name);
   p->__pyx_v_col_name = Py_None; Py_INCREF(Py_None);
   Py_XDECREF(tmp);
   tmp = ((PyObject*)p->__pyx_v_self);
   p->__pyx_v_self = Py_None; Py_INCREF(Py_None);
   Py_XDECREF(tmp);
   tmp = ((PyObject*)p->__pyx_v_threshold);
   p->__pyx_v_threshold = Py_None; Py_INCREF(Py_None);
   Py_XDECREF(tmp);
   return 0;
 }
 
-static PyTypeObject __pyx_type_6seleya_3mfc_7alchemy_5qrank_8glassdoo___pyx_scope_struct_2_calculate_result = {
+static PyTypeObject __pyx_type_6seleya_3mfc_7alchemy_5qrank_9glassdoor___pyx_scope_struct_2_calculate_result = {
   PyVarObject_HEAD_INIT(0, 0)
-  "seleya.mfc.alchemy.qrank.glassdoo.__pyx_scope_struct_2_calculate_result", /*tp_name*/
-  sizeof(struct __pyx_obj_6seleya_3mfc_7alchemy_5qrank_8glassdoo___pyx_scope_struct_2_calculate_result), /*tp_basicsize*/
+  "seleya.mfc.alchemy.qrank.glassdoor.__pyx_scope_struct_2_calculate_result", /*tp_name*/
+  sizeof(struct __pyx_obj_6seleya_3mfc_7alchemy_5qrank_9glassdoor___pyx_scope_struct_2_calculate_result), /*tp_basicsize*/
   0, /*tp_itemsize*/
-  __pyx_tp_dealloc_6seleya_3mfc_7alchemy_5qrank_8glassdoo___pyx_scope_struct_2_calculate_result, /*tp_dealloc*/
+  __pyx_tp_dealloc_6seleya_3mfc_7alchemy_5qrank_9glassdoor___pyx_scope_struct_2_calculate_result, /*tp_dealloc*/
   #if PY_VERSION_HEX < 0x030800b4
   0, /*tp_print*/
   #endif
   #if PY_VERSION_HEX >= 0x030800b4
   0, /*tp_vectorcall_offset*/
   #endif
   0, /*tp_getattr*/
@@ -7275,31 +7275,31 @@
   0, /*tp_call*/
   0, /*tp_str*/
   0, /*tp_getattro*/
   0, /*tp_setattro*/
   0, /*tp_as_buffer*/
   Py_TPFLAGS_DEFAULT|Py_TPFLAGS_HAVE_VERSION_TAG|Py_TPFLAGS_CHECKTYPES|Py_TPFLAGS_HAVE_NEWBUFFER|Py_TPFLAGS_HAVE_GC, /*tp_flags*/
   0, /*tp_doc*/
-  __pyx_tp_traverse_6seleya_3mfc_7alchemy_5qrank_8glassdoo___pyx_scope_struct_2_calculate_result, /*tp_traverse*/
-  __pyx_tp_clear_6seleya_3mfc_7alchemy_5qrank_8glassdoo___pyx_scope_struct_2_calculate_result, /*tp_clear*/
+  __pyx_tp_traverse_6seleya_3mfc_7alchemy_5qrank_9glassdoor___pyx_scope_struct_2_calculate_result, /*tp_traverse*/
+  __pyx_tp_clear_6seleya_3mfc_7alchemy_5qrank_9glassdoor___pyx_scope_struct_2_calculate_result, /*tp_clear*/
   0, /*tp_richcompare*/
   0, /*tp_weaklistoffset*/
   0, /*tp_iter*/
   0, /*tp_iternext*/
   0, /*tp_methods*/
   0, /*tp_members*/
   0, /*tp_getset*/
   0, /*tp_base*/
   0, /*tp_dict*/
   0, /*tp_descr_get*/
   0, /*tp_descr_set*/
   0, /*tp_dictoffset*/
   0, /*tp_init*/
   0, /*tp_alloc*/
-  __pyx_tp_new_6seleya_3mfc_7alchemy_5qrank_8glassdoo___pyx_scope_struct_2_calculate_result, /*tp_new*/
+  __pyx_tp_new_6seleya_3mfc_7alchemy_5qrank_9glassdoor___pyx_scope_struct_2_calculate_result, /*tp_new*/
   0, /*tp_free*/
   0, /*tp_is_gc*/
   0, /*tp_bases*/
   0, /*tp_mro*/
   0, /*tp_cache*/
   0, /*tp_subclasses*/
   0, /*tp_weaklist*/
@@ -7452,25 +7452,25 @@
 }
 
 
 
 #if PY_MAJOR_VERSION >= 3
 #if CYTHON_PEP489_MULTI_PHASE_INIT
 static PyObject* __pyx_pymod_create(PyObject *spec, PyModuleDef *def); /*proto*/
-static int __pyx_pymod_exec_glassdoo(PyObject* module); /*proto*/
+static int __pyx_pymod_exec_glassdoor(PyObject* module); /*proto*/
 static PyModuleDef_Slot __pyx_moduledef_slots[] = {
   {Py_mod_create, (void*)__pyx_pymod_create},
-  {Py_mod_exec, (void*)__pyx_pymod_exec_glassdoo},
+  {Py_mod_exec, (void*)__pyx_pymod_exec_glassdoor},
   {0, NULL}
 };
 #endif
 
 static struct PyModuleDef __pyx_moduledef = {
     PyModuleDef_HEAD_INIT,
-    "glassdoo",
+    "glassdoor",
     0, /* m_doc */
   #if CYTHON_PEP489_MULTI_PHASE_INIT
     0, /* m_size */
   #else
     -1, /* m_size */
   #endif
     __pyx_methods /* m_methods */,
@@ -7689,167 +7689,167 @@
   return -1;
 }
 
 static CYTHON_SMALL_CODE int __Pyx_InitCachedConstants(void) {
   __Pyx_RefNannyDeclarations
   __Pyx_RefNannySetupContext("__Pyx_InitCachedConstants", 0);
 
-  /* "seleya/mfc/alchemy/qrank/glassdoor.py":11
+  /* "seleya/mfc/alchemy/qrank/glassdoor.pyx":11
  * 
  * 
  * class Glassdoor(object):             # <<<<<<<<<<<<<<
  * 
  *     def __init__(self, industry_code):
  */
   __pyx_tuple__2 = PyTuple_Pack(1, __pyx_builtin_object); if (unlikely(!__pyx_tuple__2)) __PYX_ERR(0, 11, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_tuple__2);
   __Pyx_GIVEREF(__pyx_tuple__2);
 
-  /* "seleya/mfc/alchemy/qrank/glassdoor.py":13
+  /* "seleya/mfc/alchemy/qrank/glassdoor.pyx":13
  * class Glassdoor(object):
  * 
  *     def __init__(self, industry_code):             # <<<<<<<<<<<<<<
  *         self._industry_code = industry_code
  *         self._mapping_dict = {
  */
   __pyx_tuple__3 = PyTuple_Pack(2, __pyx_n_s_self, __pyx_n_s_industry_code); if (unlikely(!__pyx_tuple__3)) __PYX_ERR(0, 13, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_tuple__3);
   __Pyx_GIVEREF(__pyx_tuple__3);
   __pyx_codeobj__4 = (PyObject*)__Pyx_PyCode_New(2, 0, 2, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__3, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_seleya_mfc_alchemy_qrank_glassdo_2, __pyx_n_s_init, 13, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__4)) __PYX_ERR(0, 13, __pyx_L1_error)
 
-  /* "seleya/mfc/alchemy/qrank/glassdoor.py":34
+  /* "seleya/mfc/alchemy/qrank/glassdoor.pyx":34
  *         self._factors_sets = self._probability_cols + self._mean_cols
  * 
  *     def _fetch_overview(self, codes):             # <<<<<<<<<<<<<<
  *         kd_logger.info('Fetching glassdoor overview data...')
  *         gd_overview_data = SurfaceDBAPI.GDOveriew().fetch(
  */
   __pyx_tuple__5 = PyTuple_Pack(3, __pyx_n_s_self, __pyx_n_s_codes, __pyx_n_s_gd_overview_data); if (unlikely(!__pyx_tuple__5)) __PYX_ERR(0, 34, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_tuple__5);
   __Pyx_GIVEREF(__pyx_tuple__5);
   __pyx_codeobj__6 = (PyObject*)__Pyx_PyCode_New(2, 0, 3, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__5, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_seleya_mfc_alchemy_qrank_glassdo_2, __pyx_n_s_fetch_overview, 34, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__6)) __PYX_ERR(0, 34, __pyx_L1_error)
 
-  /* "seleya/mfc/alchemy/qrank/glassdoor.py":42
+  /* "seleya/mfc/alchemy/qrank/glassdoor.pyx":42
  *         return gd_overview_data
  * 
  *     def _fetch_reviews(self, begin_date, end_date, cids):             # <<<<<<<<<<<<<<
  *         kd_logger.info('Fetching glassdoor reviews data...')
  *         columns = ['id', 'cid', 'reviewId', 'reviewDateTime'
  */
   __pyx_tuple__7 = PyTuple_Pack(7, __pyx_n_s_self, __pyx_n_s_begin_date, __pyx_n_s_end_date, __pyx_n_s_cids, __pyx_n_s_columns, __pyx_n_s_gd_reviews_data, __pyx_n_s_col); if (unlikely(!__pyx_tuple__7)) __PYX_ERR(0, 42, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_tuple__7);
   __Pyx_GIVEREF(__pyx_tuple__7);
   __pyx_codeobj__8 = (PyObject*)__Pyx_PyCode_New(4, 0, 7, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__7, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_seleya_mfc_alchemy_qrank_glassdo_2, __pyx_n_s_fetch_reviews, 42, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__8)) __PYX_ERR(0, 42, __pyx_L1_error)
 
-  /* "seleya/mfc/alchemy/qrank/glassdoor.py":63
+  /* "seleya/mfc/alchemy/qrank/glassdoor.pyx":63
  *         return gd_reviews_data
  * 
  *     def prepare_data(self, begin_date=None, end_date=None):             # <<<<<<<<<<<<<<
  *         kd_logger.info('Fetching industry data...')
  *         industry_data = SurfaceDBAPI.Industry().fetch(
  */
   __pyx_tuple__9 = PyTuple_Pack(9, __pyx_n_s_self, __pyx_n_s_begin_date, __pyx_n_s_end_date, __pyx_n_s_industry_data, __pyx_n_s_codes, __pyx_n_s_gd_overview_data, __pyx_n_s_cids, __pyx_n_s_gd_reviews_data, __pyx_n_s_total_data); if (unlikely(!__pyx_tuple__9)) __PYX_ERR(0, 63, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_tuple__9);
   __Pyx_GIVEREF(__pyx_tuple__9);
   __pyx_codeobj__10 = (PyObject*)__Pyx_PyCode_New(3, 0, 9, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__9, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_seleya_mfc_alchemy_qrank_glassdo_2, __pyx_n_s_prepare_data, 63, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__10)) __PYX_ERR(0, 63, __pyx_L1_error)
   __pyx_tuple__11 = PyTuple_Pack(2, ((PyObject *)Py_None), ((PyObject *)Py_None)); if (unlikely(!__pyx_tuple__11)) __PYX_ERR(0, 63, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_tuple__11);
   __Pyx_GIVEREF(__pyx_tuple__11);
 
-  /* "seleya/mfc/alchemy/qrank/glassdoor.py":92
+  /* "seleya/mfc/alchemy/qrank/glassdoor.pyx":92
  *         return total_data
  * 
  *     def _transform_raw(self, mean_data):             # <<<<<<<<<<<<<<
  *         # save the raw average scores for UI use
  *         raw_data = mean_data.reset_index().set_index([
  */
   __pyx_tuple__12 = PyTuple_Pack(3, __pyx_n_s_self, __pyx_n_s_mean_data, __pyx_n_s_raw_data); if (unlikely(!__pyx_tuple__12)) __PYX_ERR(0, 92, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_tuple__12);
   __Pyx_GIVEREF(__pyx_tuple__12);
   __pyx_codeobj__13 = (PyObject*)__Pyx_PyCode_New(2, 0, 3, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__12, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_seleya_mfc_alchemy_qrank_glassdo_2, __pyx_n_s_transform_raw, 92, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__13)) __PYX_ERR(0, 92, __pyx_L1_error)
 
-  /* "seleya/mfc/alchemy/qrank/glassdoor.py":106
+  /* "seleya/mfc/alchemy/qrank/glassdoor.pyx":106
  *         return raw_data
  * 
  *     def _blom_score(self, values_series, threshold=0.9):             # <<<<<<<<<<<<<<
  *         idx = values_series.index.droplevel(level=0)
  *         coverage = values_series.isna().sum() / len(values_series)
  */
   __pyx_tuple__15 = PyTuple_Pack(9, __pyx_n_s_self, __pyx_n_s_values_series, __pyx_n_s_threshold, __pyx_n_s_idx, __pyx_n_s_coverage, __pyx_n_s_scores, __pyx_n_s_ranks, __pyx_n_s_n, __pyx_n_s__14); if (unlikely(!__pyx_tuple__15)) __PYX_ERR(0, 106, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_tuple__15);
   __Pyx_GIVEREF(__pyx_tuple__15);
   __pyx_codeobj__16 = (PyObject*)__Pyx_PyCode_New(3, 0, 9, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__15, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_seleya_mfc_alchemy_qrank_glassdo_2, __pyx_n_s_blom_score, 106, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__16)) __PYX_ERR(0, 106, __pyx_L1_error)
   __pyx_tuple__17 = PyTuple_Pack(1, ((PyObject*)__pyx_float_0_9)); if (unlikely(!__pyx_tuple__17)) __PYX_ERR(0, 106, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_tuple__17);
   __Pyx_GIVEREF(__pyx_tuple__17);
 
-  /* "seleya/mfc/alchemy/qrank/glassdoor.py":119
+  /* "seleya/mfc/alchemy/qrank/glassdoor.pyx":119
  *         return scores
  * 
  *     def _distribute(self, mean_data):             # <<<<<<<<<<<<<<
  *         dt = mean_data.set_index(['date', 'code', 'name'])['value']
  *         res = []
  */
   __pyx_tuple__18 = PyTuple_Pack(5, __pyx_n_s_self, __pyx_n_s_mean_data, __pyx_n_s_dt, __pyx_n_s_res, __pyx_n_s__14); if (unlikely(!__pyx_tuple__18)) __PYX_ERR(0, 119, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_tuple__18);
   __Pyx_GIVEREF(__pyx_tuple__18);
   __pyx_codeobj__19 = (PyObject*)__Pyx_PyCode_New(2, 0, 5, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__18, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_seleya_mfc_alchemy_qrank_glassdo_2, __pyx_n_s_distribute, 119, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__19)) __PYX_ERR(0, 119, __pyx_L1_error)
 
-  /* "seleya/mfc/alchemy/qrank/glassdoor.py":127
+  /* "seleya/mfc/alchemy/qrank/glassdoor.pyx":127
  *         return dt
  * 
  *     def _percentile(self, x, res):             # <<<<<<<<<<<<<<
  *         name = str(x.name)
  *         x = x.dropna()
  */
   __pyx_tuple__20 = PyTuple_Pack(5, __pyx_n_s_self, __pyx_n_s_x, __pyx_n_s_res, __pyx_n_s_name, __pyx_n_s_rt); if (unlikely(!__pyx_tuple__20)) __PYX_ERR(0, 127, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_tuple__20);
   __Pyx_GIVEREF(__pyx_tuple__20);
   __pyx_codeobj__21 = (PyObject*)__Pyx_PyCode_New(3, 0, 5, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__20, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_seleya_mfc_alchemy_qrank_glassdo_2, __pyx_n_s_percentile, 127, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__21)) __PYX_ERR(0, 127, __pyx_L1_error)
 
-  /* "seleya/mfc/alchemy/qrank/glassdoor.py":135
+  /* "seleya/mfc/alchemy/qrank/glassdoor.pyx":135
  *         res.append(rt.reset_index().set_index(['date', 'code']))
  * 
  *     def _calculate_distribute(self, mean_data):             # <<<<<<<<<<<<<<
  *         kd_logger.info('calculating distribute...')
  *         mean_data['date'] = pd.to_datetime(mean_data['date'])
  */
   __pyx_tuple__22 = PyTuple_Pack(3, __pyx_n_s_self, __pyx_n_s_mean_data, __pyx_n_s_dist_data); if (unlikely(!__pyx_tuple__22)) __PYX_ERR(0, 135, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_tuple__22);
   __Pyx_GIVEREF(__pyx_tuple__22);
   __pyx_codeobj__23 = (PyObject*)__Pyx_PyCode_New(2, 0, 3, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__22, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_seleya_mfc_alchemy_qrank_glassdo_2, __pyx_n_s_calculate_distribute, 135, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__23)) __PYX_ERR(0, 135, __pyx_L1_error)
 
-  /* "seleya/mfc/alchemy/qrank/glassdoor.py":148
+  /* "seleya/mfc/alchemy/qrank/glassdoor.pyx":148
  *         return dist_data
  * 
  *     def _format_mean(self, mean_data):             # <<<<<<<<<<<<<<
  *         mean_data['industry'] = self._industry_code
  *         mean_data['date'] = mean_data['date'].dt.strftime('%Y-%m-%d')
  */
   __pyx_tuple__24 = PyTuple_Pack(2, __pyx_n_s_self, __pyx_n_s_mean_data); if (unlikely(!__pyx_tuple__24)) __PYX_ERR(0, 148, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_tuple__24);
   __Pyx_GIVEREF(__pyx_tuple__24);
   __pyx_codeobj__25 = (PyObject*)__Pyx_PyCode_New(2, 0, 2, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__24, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_seleya_mfc_alchemy_qrank_glassdo_2, __pyx_n_s_format_mean, 148, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__25)) __PYX_ERR(0, 148, __pyx_L1_error)
 
-  /* "seleya/mfc/alchemy/qrank/glassdoor.py":153
+  /* "seleya/mfc/alchemy/qrank/glassdoor.pyx":153
  *         return mean_data
  * 
  *     def calculate_result(self, total_data, threshold=0.9):             # <<<<<<<<<<<<<<
  *         # aggregate means by year and cid
  *         mean_data = total_data.groupby(['date', 'code']).mean()
  */
   __pyx_tuple__26 = PyTuple_Pack(8, __pyx_n_s_self, __pyx_n_s_total_data, __pyx_n_s_threshold, __pyx_n_s_mean_data, __pyx_n_s_raw_data, __pyx_n_s_col_name, __pyx_n_s_col_score, __pyx_n_s_dist_data); if (unlikely(!__pyx_tuple__26)) __PYX_ERR(0, 153, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_tuple__26);
   __Pyx_GIVEREF(__pyx_tuple__26);
   __pyx_codeobj__27 = (PyObject*)__Pyx_PyCode_New(3, 0, 8, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__26, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_seleya_mfc_alchemy_qrank_glassdo_2, __pyx_n_s_calculate_result, 153, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__27)) __PYX_ERR(0, 153, __pyx_L1_error)
   __pyx_tuple__28 = PyTuple_Pack(1, ((PyObject*)__pyx_float_0_9)); if (unlikely(!__pyx_tuple__28)) __PYX_ERR(0, 153, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_tuple__28);
   __Pyx_GIVEREF(__pyx_tuple__28);
 
-  /* "seleya/mfc/alchemy/qrank/glassdoor.py":183
+  /* "seleya/mfc/alchemy/qrank/glassdoor.pyx":183
  *         return raw_data, self._format_mean(mean_data), dist_data
  * 
  *     def run(self, begin_date, end_date, threshold=0.9):             # <<<<<<<<<<<<<<
  *         total_data = self.prepare_data(begin_date, end_date)
  *         if total_data is None or total_data.empty:
  */
   __pyx_tuple__29 = PyTuple_Pack(5, __pyx_n_s_self, __pyx_n_s_begin_date, __pyx_n_s_end_date, __pyx_n_s_threshold, __pyx_n_s_total_data); if (unlikely(!__pyx_tuple__29)) __PYX_ERR(0, 183, __pyx_L1_error)
@@ -7913,38 +7913,38 @@
 static int __Pyx_modinit_type_init_code(void) {
   __Pyx_RefNannyDeclarations
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("__Pyx_modinit_type_init_code", 0);
   /*--- Type init code ---*/
-  if (PyType_Ready(&__pyx_type_6seleya_3mfc_7alchemy_5qrank_8glassdoo___pyx_scope_struct___fetch_reviews) < 0) __PYX_ERR(0, 42, __pyx_L1_error)
+  if (PyType_Ready(&__pyx_type_6seleya_3mfc_7alchemy_5qrank_9glassdoor___pyx_scope_struct___fetch_reviews) < 0) __PYX_ERR(0, 42, __pyx_L1_error)
   #if PY_VERSION_HEX < 0x030800B1
-  __pyx_type_6seleya_3mfc_7alchemy_5qrank_8glassdoo___pyx_scope_struct___fetch_reviews.tp_print = 0;
+  __pyx_type_6seleya_3mfc_7alchemy_5qrank_9glassdoor___pyx_scope_struct___fetch_reviews.tp_print = 0;
   #endif
-  if ((CYTHON_USE_TYPE_SLOTS && CYTHON_USE_PYTYPE_LOOKUP) && likely(!__pyx_type_6seleya_3mfc_7alchemy_5qrank_8glassdoo___pyx_scope_struct___fetch_reviews.tp_dictoffset && __pyx_type_6seleya_3mfc_7alchemy_5qrank_8glassdoo___pyx_scope_struct___fetch_reviews.tp_getattro == PyObject_GenericGetAttr)) {
-    __pyx_type_6seleya_3mfc_7alchemy_5qrank_8glassdoo___pyx_scope_struct___fetch_reviews.tp_getattro = __Pyx_PyObject_GenericGetAttrNoDict;
+  if ((CYTHON_USE_TYPE_SLOTS && CYTHON_USE_PYTYPE_LOOKUP) && likely(!__pyx_type_6seleya_3mfc_7alchemy_5qrank_9glassdoor___pyx_scope_struct___fetch_reviews.tp_dictoffset && __pyx_type_6seleya_3mfc_7alchemy_5qrank_9glassdoor___pyx_scope_struct___fetch_reviews.tp_getattro == PyObject_GenericGetAttr)) {
+    __pyx_type_6seleya_3mfc_7alchemy_5qrank_9glassdoor___pyx_scope_struct___fetch_reviews.tp_getattro = __Pyx_PyObject_GenericGetAttrNoDict;
   }
-  __pyx_ptype_6seleya_3mfc_7alchemy_5qrank_8glassdoo___pyx_scope_struct___fetch_reviews = &__pyx_type_6seleya_3mfc_7alchemy_5qrank_8glassdoo___pyx_scope_struct___fetch_reviews;
-  if (PyType_Ready(&__pyx_type_6seleya_3mfc_7alchemy_5qrank_8glassdoo___pyx_scope_struct_1__distribute) < 0) __PYX_ERR(0, 119, __pyx_L1_error)
+  __pyx_ptype_6seleya_3mfc_7alchemy_5qrank_9glassdoor___pyx_scope_struct___fetch_reviews = &__pyx_type_6seleya_3mfc_7alchemy_5qrank_9glassdoor___pyx_scope_struct___fetch_reviews;
+  if (PyType_Ready(&__pyx_type_6seleya_3mfc_7alchemy_5qrank_9glassdoor___pyx_scope_struct_1__distribute) < 0) __PYX_ERR(0, 119, __pyx_L1_error)
   #if PY_VERSION_HEX < 0x030800B1
-  __pyx_type_6seleya_3mfc_7alchemy_5qrank_8glassdoo___pyx_scope_struct_1__distribute.tp_print = 0;
+  __pyx_type_6seleya_3mfc_7alchemy_5qrank_9glassdoor___pyx_scope_struct_1__distribute.tp_print = 0;
   #endif
-  if ((CYTHON_USE_TYPE_SLOTS && CYTHON_USE_PYTYPE_LOOKUP) && likely(!__pyx_type_6seleya_3mfc_7alchemy_5qrank_8glassdoo___pyx_scope_struct_1__distribute.tp_dictoffset && __pyx_type_6seleya_3mfc_7alchemy_5qrank_8glassdoo___pyx_scope_struct_1__distribute.tp_getattro == PyObject_GenericGetAttr)) {
-    __pyx_type_6seleya_3mfc_7alchemy_5qrank_8glassdoo___pyx_scope_struct_1__distribute.tp_getattro = __Pyx_PyObject_GenericGetAttrNoDict;
+  if ((CYTHON_USE_TYPE_SLOTS && CYTHON_USE_PYTYPE_LOOKUP) && likely(!__pyx_type_6seleya_3mfc_7alchemy_5qrank_9glassdoor___pyx_scope_struct_1__distribute.tp_dictoffset && __pyx_type_6seleya_3mfc_7alchemy_5qrank_9glassdoor___pyx_scope_struct_1__distribute.tp_getattro == PyObject_GenericGetAttr)) {
+    __pyx_type_6seleya_3mfc_7alchemy_5qrank_9glassdoor___pyx_scope_struct_1__distribute.tp_getattro = __Pyx_PyObject_GenericGetAttrNoDict;
   }
-  __pyx_ptype_6seleya_3mfc_7alchemy_5qrank_8glassdoo___pyx_scope_struct_1__distribute = &__pyx_type_6seleya_3mfc_7alchemy_5qrank_8glassdoo___pyx_scope_struct_1__distribute;
-  if (PyType_Ready(&__pyx_type_6seleya_3mfc_7alchemy_5qrank_8glassdoo___pyx_scope_struct_2_calculate_result) < 0) __PYX_ERR(0, 153, __pyx_L1_error)
+  __pyx_ptype_6seleya_3mfc_7alchemy_5qrank_9glassdoor___pyx_scope_struct_1__distribute = &__pyx_type_6seleya_3mfc_7alchemy_5qrank_9glassdoor___pyx_scope_struct_1__distribute;
+  if (PyType_Ready(&__pyx_type_6seleya_3mfc_7alchemy_5qrank_9glassdoor___pyx_scope_struct_2_calculate_result) < 0) __PYX_ERR(0, 153, __pyx_L1_error)
   #if PY_VERSION_HEX < 0x030800B1
-  __pyx_type_6seleya_3mfc_7alchemy_5qrank_8glassdoo___pyx_scope_struct_2_calculate_result.tp_print = 0;
+  __pyx_type_6seleya_3mfc_7alchemy_5qrank_9glassdoor___pyx_scope_struct_2_calculate_result.tp_print = 0;
   #endif
-  if ((CYTHON_USE_TYPE_SLOTS && CYTHON_USE_PYTYPE_LOOKUP) && likely(!__pyx_type_6seleya_3mfc_7alchemy_5qrank_8glassdoo___pyx_scope_struct_2_calculate_result.tp_dictoffset && __pyx_type_6seleya_3mfc_7alchemy_5qrank_8glassdoo___pyx_scope_struct_2_calculate_result.tp_getattro == PyObject_GenericGetAttr)) {
-    __pyx_type_6seleya_3mfc_7alchemy_5qrank_8glassdoo___pyx_scope_struct_2_calculate_result.tp_getattro = __Pyx_PyObject_GenericGetAttrNoDict;
+  if ((CYTHON_USE_TYPE_SLOTS && CYTHON_USE_PYTYPE_LOOKUP) && likely(!__pyx_type_6seleya_3mfc_7alchemy_5qrank_9glassdoor___pyx_scope_struct_2_calculate_result.tp_dictoffset && __pyx_type_6seleya_3mfc_7alchemy_5qrank_9glassdoor___pyx_scope_struct_2_calculate_result.tp_getattro == PyObject_GenericGetAttr)) {
+    __pyx_type_6seleya_3mfc_7alchemy_5qrank_9glassdoor___pyx_scope_struct_2_calculate_result.tp_getattro = __Pyx_PyObject_GenericGetAttrNoDict;
   }
-  __pyx_ptype_6seleya_3mfc_7alchemy_5qrank_8glassdoo___pyx_scope_struct_2_calculate_result = &__pyx_type_6seleya_3mfc_7alchemy_5qrank_8glassdoo___pyx_scope_struct_2_calculate_result;
+  __pyx_ptype_6seleya_3mfc_7alchemy_5qrank_9glassdoor___pyx_scope_struct_2_calculate_result = &__pyx_type_6seleya_3mfc_7alchemy_5qrank_9glassdoor___pyx_scope_struct_2_calculate_result;
   __Pyx_RefNannyFinishContext();
   return 0;
   __pyx_L1_error:;
   __Pyx_RefNannyFinishContext();
   return -1;
 }
 
@@ -7987,19 +7987,19 @@
 #else
 #define __Pyx_PyMODINIT_FUNC PyObject *
 #endif
 #endif
 
 
 #if PY_MAJOR_VERSION < 3
-__Pyx_PyMODINIT_FUNC initglassdoo(void) CYTHON_SMALL_CODE; /*proto*/
-__Pyx_PyMODINIT_FUNC initglassdoo(void)
+__Pyx_PyMODINIT_FUNC initglassdoor(void) CYTHON_SMALL_CODE; /*proto*/
+__Pyx_PyMODINIT_FUNC initglassdoor(void)
 #else
-__Pyx_PyMODINIT_FUNC PyInit_glassdoo(void) CYTHON_SMALL_CODE; /*proto*/
-__Pyx_PyMODINIT_FUNC PyInit_glassdoo(void)
+__Pyx_PyMODINIT_FUNC PyInit_glassdoor(void) CYTHON_SMALL_CODE; /*proto*/
+__Pyx_PyMODINIT_FUNC PyInit_glassdoor(void)
 #if CYTHON_PEP489_MULTI_PHASE_INIT
 {
   return PyModuleDef_Init(&__pyx_moduledef);
 }
 static CYTHON_SMALL_CODE int __Pyx_check_single_interpreter(void) {
     #if PY_VERSION_HEX >= 0x030700A1
     static PY_INT64_T main_interpreter_id = -1;
@@ -8058,44 +8058,44 @@
     return module;
 bad:
     Py_XDECREF(module);
     return NULL;
 }
 
 
-static CYTHON_SMALL_CODE int __pyx_pymod_exec_glassdoo(PyObject *__pyx_pyinit_module)
+static CYTHON_SMALL_CODE int __pyx_pymod_exec_glassdoor(PyObject *__pyx_pyinit_module)
 #endif
 #endif
 {
   PyObject *__pyx_t_1 = NULL;
   PyObject *__pyx_t_2 = NULL;
   PyObject *__pyx_t_3 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannyDeclarations
   #if CYTHON_PEP489_MULTI_PHASE_INIT
   if (__pyx_m) {
     if (__pyx_m == __pyx_pyinit_module) return 0;
-    PyErr_SetString(PyExc_RuntimeError, "Module 'glassdoo' has already been imported. Re-initialisation is not supported.");
+    PyErr_SetString(PyExc_RuntimeError, "Module 'glassdoor' has already been imported. Re-initialisation is not supported.");
     return -1;
   }
   #elif PY_MAJOR_VERSION >= 3
   if (__pyx_m) return __Pyx_NewRef(__pyx_m);
   #endif
   #if CYTHON_REFNANNY
 __Pyx_RefNanny = __Pyx_RefNannyImportAPI("refnanny");
 if (!__Pyx_RefNanny) {
   PyErr_Clear();
   __Pyx_RefNanny = __Pyx_RefNannyImportAPI("Cython.Runtime.refnanny");
   if (!__Pyx_RefNanny)
       Py_FatalError("failed to import 'refnanny' module");
 }
 #endif
-  __Pyx_RefNannySetupContext("__Pyx_PyMODINIT_FUNC PyInit_glassdoo(void)", 0);
+  __Pyx_RefNannySetupContext("__Pyx_PyMODINIT_FUNC PyInit_glassdoor(void)", 0);
   if (__Pyx_check_binary_version() < 0) __PYX_ERR(0, 1, __pyx_L1_error)
   #ifdef __Pxy_PyFrame_Initialize_Offsets
   __Pxy_PyFrame_Initialize_Offsets();
   #endif
   __pyx_empty_tuple = PyTuple_New(0); if (unlikely(!__pyx_empty_tuple)) __PYX_ERR(0, 1, __pyx_L1_error)
   __pyx_empty_bytes = PyBytes_FromStringAndSize("", 0); if (unlikely(!__pyx_empty_bytes)) __PYX_ERR(0, 1, __pyx_L1_error)
   __pyx_empty_unicode = PyUnicode_FromStringAndSize("", 0); if (unlikely(!__pyx_empty_unicode)) __PYX_ERR(0, 1, __pyx_L1_error)
@@ -8126,15 +8126,15 @@
   #endif
   /*--- Module creation code ---*/
   #if CYTHON_PEP489_MULTI_PHASE_INIT
   __pyx_m = __pyx_pyinit_module;
   Py_INCREF(__pyx_m);
   #else
   #if PY_MAJOR_VERSION < 3
-  __pyx_m = Py_InitModule4("glassdoo", __pyx_methods, 0, 0, PYTHON_API_VERSION); Py_XINCREF(__pyx_m);
+  __pyx_m = Py_InitModule4("glassdoor", __pyx_methods, 0, 0, PYTHON_API_VERSION); Py_XINCREF(__pyx_m);
   #else
   __pyx_m = PyModule_Create(&__pyx_moduledef);
   #endif
   if (unlikely(!__pyx_m)) __PYX_ERR(0, 1, __pyx_L1_error)
   #endif
   __pyx_d = PyModule_GetDict(__pyx_m); if (unlikely(!__pyx_d)) __PYX_ERR(0, 1, __pyx_L1_error)
   Py_INCREF(__pyx_d);
@@ -8144,22 +8144,22 @@
   Py_INCREF(__pyx_cython_runtime);
   if (PyObject_SetAttrString(__pyx_m, "__builtins__", __pyx_b) < 0) __PYX_ERR(0, 1, __pyx_L1_error);
   /*--- Initialize various global constants etc. ---*/
   if (__Pyx_InitGlobals() < 0) __PYX_ERR(0, 1, __pyx_L1_error)
   #if PY_MAJOR_VERSION < 3 && (__PYX_DEFAULT_STRING_ENCODING_IS_ASCII || __PYX_DEFAULT_STRING_ENCODING_IS_DEFAULT)
   if (__Pyx_init_sys_getdefaultencoding_params() < 0) __PYX_ERR(0, 1, __pyx_L1_error)
   #endif
-  if (__pyx_module_is_main_seleya__mfc__alchemy__qrank__glassdoo) {
+  if (__pyx_module_is_main_seleya__mfc__alchemy__qrank__glassdoor) {
     if (PyObject_SetAttr(__pyx_m, __pyx_n_s_name_2, __pyx_n_s_main) < 0) __PYX_ERR(0, 1, __pyx_L1_error)
   }
   #if PY_MAJOR_VERSION >= 3
   {
     PyObject *modules = PyImport_GetModuleDict(); if (unlikely(!modules)) __PYX_ERR(0, 1, __pyx_L1_error)
-    if (!PyDict_GetItemString(modules, "seleya.mfc.alchemy.qrank.glassdoo")) {
-      if (unlikely(PyDict_SetItemString(modules, "seleya.mfc.alchemy.qrank.glassdoo", __pyx_m) < 0)) __PYX_ERR(0, 1, __pyx_L1_error)
+    if (!PyDict_GetItemString(modules, "seleya.mfc.alchemy.qrank.glassdoor")) {
+      if (unlikely(PyDict_SetItemString(modules, "seleya.mfc.alchemy.qrank.glassdoor", __pyx_m) < 0)) __PYX_ERR(0, 1, __pyx_L1_error)
     }
   }
   #endif
   /*--- Builtin init code ---*/
   if (__Pyx_InitCachedBuiltins() < 0) __PYX_ERR(0, 1, __pyx_L1_error)
   /*--- Constants init code ---*/
   if (__Pyx_InitCachedConstants() < 0) __PYX_ERR(0, 1, __pyx_L1_error)
@@ -8172,38 +8172,38 @@
   (void)__Pyx_modinit_variable_import_code();
   (void)__Pyx_modinit_function_import_code();
   /*--- Execution code ---*/
   #if defined(__Pyx_Generator_USED) || defined(__Pyx_Coroutine_USED)
   if (__Pyx_patch_abc() < 0) __PYX_ERR(0, 1, __pyx_L1_error)
   #endif
 
-  /* "seleya/mfc/alchemy/qrank/glassdoor.py":2
+  /* "seleya/mfc/alchemy/qrank/glassdoor.pyx":2
  * # -*- coding: utf-8 -*-
  * import numpy as np             # <<<<<<<<<<<<<<
  * import pandas as pd
  * import scipy.stats as stats
  */
   __pyx_t_1 = __Pyx_Import(__pyx_n_s_numpy, 0, -1); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 2, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   if (PyDict_SetItem(__pyx_d, __pyx_n_s_np, __pyx_t_1) < 0) __PYX_ERR(0, 2, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
 
-  /* "seleya/mfc/alchemy/qrank/glassdoor.py":3
+  /* "seleya/mfc/alchemy/qrank/glassdoor.pyx":3
  * # -*- coding: utf-8 -*-
  * import numpy as np
  * import pandas as pd             # <<<<<<<<<<<<<<
  * import scipy.stats as stats
  * from ultron.sentry.api import *
  */
   __pyx_t_1 = __Pyx_Import(__pyx_n_s_pandas, 0, -1); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 3, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   if (PyDict_SetItem(__pyx_d, __pyx_n_s_pd, __pyx_t_1) < 0) __PYX_ERR(0, 3, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
 
-  /* "seleya/mfc/alchemy/qrank/glassdoor.py":4
+  /* "seleya/mfc/alchemy/qrank/glassdoor.pyx":4
  * import numpy as np
  * import pandas as pd
  * import scipy.stats as stats             # <<<<<<<<<<<<<<
  * from ultron.sentry.api import *
  * from seleya import SurfaceDBAPI
  */
   __pyx_t_1 = PyList_New(1); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 4, __pyx_L1_error)
@@ -8213,15 +8213,15 @@
   PyList_SET_ITEM(__pyx_t_1, 0, __pyx_n_s_);
   __pyx_t_2 = __Pyx_Import(__pyx_n_s_scipy_stats, __pyx_t_1, -1); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 4, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   if (PyDict_SetItem(__pyx_d, __pyx_n_s_stats, __pyx_t_2) < 0) __PYX_ERR(0, 4, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
 
-  /* "seleya/mfc/alchemy/qrank/glassdoor.py":5
+  /* "seleya/mfc/alchemy/qrank/glassdoor.pyx":5
  * import pandas as pd
  * import scipy.stats as stats
  * from ultron.sentry.api import *             # <<<<<<<<<<<<<<
  * from seleya import SurfaceDBAPI
  * from seleya.utilities.kd_logger import kd_logger
  */
   __pyx_t_2 = PyList_New(1); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 5, __pyx_L1_error)
@@ -8231,15 +8231,15 @@
   PyList_SET_ITEM(__pyx_t_2, 0, __pyx_n_s_);
   __pyx_t_1 = __Pyx_Import(__pyx_n_s_ultron_sentry_api, __pyx_t_2, -1); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 5, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
   if (__pyx_import_star(__pyx_t_1) < 0) __PYX_ERR(0, 5, __pyx_L1_error);
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
 
-  /* "seleya/mfc/alchemy/qrank/glassdoor.py":6
+  /* "seleya/mfc/alchemy/qrank/glassdoor.pyx":6
  * import scipy.stats as stats
  * from ultron.sentry.api import *
  * from seleya import SurfaceDBAPI             # <<<<<<<<<<<<<<
  * from seleya.utilities.kd_logger import kd_logger
  * import pdb
  */
   __pyx_t_1 = PyList_New(1); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 6, __pyx_L1_error)
@@ -8252,15 +8252,15 @@
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   __pyx_t_1 = __Pyx_ImportFrom(__pyx_t_2, __pyx_n_s_SurfaceDBAPI); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 6, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   if (PyDict_SetItem(__pyx_d, __pyx_n_s_SurfaceDBAPI, __pyx_t_1) < 0) __PYX_ERR(0, 6, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
 
-  /* "seleya/mfc/alchemy/qrank/glassdoor.py":7
+  /* "seleya/mfc/alchemy/qrank/glassdoor.pyx":7
  * from ultron.sentry.api import *
  * from seleya import SurfaceDBAPI
  * from seleya.utilities.kd_logger import kd_logger             # <<<<<<<<<<<<<<
  * import pdb
  * 
  */
   __pyx_t_2 = PyList_New(1); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 7, __pyx_L1_error)
@@ -8273,201 +8273,201 @@
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
   __pyx_t_2 = __Pyx_ImportFrom(__pyx_t_1, __pyx_n_s_kd_logger); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 7, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   if (PyDict_SetItem(__pyx_d, __pyx_n_s_kd_logger, __pyx_t_2) < 0) __PYX_ERR(0, 7, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
 
-  /* "seleya/mfc/alchemy/qrank/glassdoor.py":8
+  /* "seleya/mfc/alchemy/qrank/glassdoor.pyx":8
  * from seleya import SurfaceDBAPI
  * from seleya.utilities.kd_logger import kd_logger
  * import pdb             # <<<<<<<<<<<<<<
  * 
  * 
  */
   __pyx_t_1 = __Pyx_Import(__pyx_n_s_pdb, 0, -1); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 8, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   if (PyDict_SetItem(__pyx_d, __pyx_n_s_pdb, __pyx_t_1) < 0) __PYX_ERR(0, 8, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
 
-  /* "seleya/mfc/alchemy/qrank/glassdoor.py":11
+  /* "seleya/mfc/alchemy/qrank/glassdoor.pyx":11
  * 
  * 
  * class Glassdoor(object):             # <<<<<<<<<<<<<<
  * 
  *     def __init__(self, industry_code):
  */
   __pyx_t_1 = __Pyx_CalculateMetaclass(NULL, __pyx_tuple__2); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 11, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_t_2 = __Pyx_Py3MetaclassPrepare(__pyx_t_1, __pyx_tuple__2, __pyx_n_s_Glassdoor, __pyx_n_s_Glassdoor, (PyObject *) NULL, __pyx_n_s_seleya_mfc_alchemy_qrank_glassdo, (PyObject *) NULL); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 11, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
 
-  /* "seleya/mfc/alchemy/qrank/glassdoor.py":13
+  /* "seleya/mfc/alchemy/qrank/glassdoor.pyx":13
  * class Glassdoor(object):
  * 
  *     def __init__(self, industry_code):             # <<<<<<<<<<<<<<
  *         self._industry_code = industry_code
  *         self._mapping_dict = {
  */
-  __pyx_t_3 = __Pyx_CyFunction_New(&__pyx_mdef_6seleya_3mfc_7alchemy_5qrank_8glassdoo_9Glassdoor_1__init__, 0, __pyx_n_s_Glassdoor___init, NULL, __pyx_n_s_seleya_mfc_alchemy_qrank_glassdo, __pyx_d, ((PyObject *)__pyx_codeobj__4)); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 13, __pyx_L1_error)
+  __pyx_t_3 = __Pyx_CyFunction_New(&__pyx_mdef_6seleya_3mfc_7alchemy_5qrank_9glassdoor_9Glassdoor_1__init__, 0, __pyx_n_s_Glassdoor___init, NULL, __pyx_n_s_seleya_mfc_alchemy_qrank_glassdo, __pyx_d, ((PyObject *)__pyx_codeobj__4)); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 13, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
   if (__Pyx_SetNameInClass(__pyx_t_2, __pyx_n_s_init, __pyx_t_3) < 0) __PYX_ERR(0, 13, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
 
-  /* "seleya/mfc/alchemy/qrank/glassdoor.py":34
+  /* "seleya/mfc/alchemy/qrank/glassdoor.pyx":34
  *         self._factors_sets = self._probability_cols + self._mean_cols
  * 
  *     def _fetch_overview(self, codes):             # <<<<<<<<<<<<<<
  *         kd_logger.info('Fetching glassdoor overview data...')
  *         gd_overview_data = SurfaceDBAPI.GDOveriew().fetch(
  */
-  __pyx_t_3 = __Pyx_CyFunction_New(&__pyx_mdef_6seleya_3mfc_7alchemy_5qrank_8glassdoo_9Glassdoor_3_fetch_overview, 0, __pyx_n_s_Glassdoor__fetch_overview, NULL, __pyx_n_s_seleya_mfc_alchemy_qrank_glassdo, __pyx_d, ((PyObject *)__pyx_codeobj__6)); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 34, __pyx_L1_error)
+  __pyx_t_3 = __Pyx_CyFunction_New(&__pyx_mdef_6seleya_3mfc_7alchemy_5qrank_9glassdoor_9Glassdoor_3_fetch_overview, 0, __pyx_n_s_Glassdoor__fetch_overview, NULL, __pyx_n_s_seleya_mfc_alchemy_qrank_glassdo, __pyx_d, ((PyObject *)__pyx_codeobj__6)); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 34, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
   if (__Pyx_SetNameInClass(__pyx_t_2, __pyx_n_s_fetch_overview, __pyx_t_3) < 0) __PYX_ERR(0, 34, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
 
-  /* "seleya/mfc/alchemy/qrank/glassdoor.py":42
+  /* "seleya/mfc/alchemy/qrank/glassdoor.pyx":42
  *         return gd_overview_data
  * 
  *     def _fetch_reviews(self, begin_date, end_date, cids):             # <<<<<<<<<<<<<<
  *         kd_logger.info('Fetching glassdoor reviews data...')
  *         columns = ['id', 'cid', 'reviewId', 'reviewDateTime'
  */
-  __pyx_t_3 = __Pyx_CyFunction_New(&__pyx_mdef_6seleya_3mfc_7alchemy_5qrank_8glassdoo_9Glassdoor_5_fetch_reviews, 0, __pyx_n_s_Glassdoor__fetch_reviews, NULL, __pyx_n_s_seleya_mfc_alchemy_qrank_glassdo, __pyx_d, ((PyObject *)__pyx_codeobj__8)); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 42, __pyx_L1_error)
+  __pyx_t_3 = __Pyx_CyFunction_New(&__pyx_mdef_6seleya_3mfc_7alchemy_5qrank_9glassdoor_9Glassdoor_5_fetch_reviews, 0, __pyx_n_s_Glassdoor__fetch_reviews, NULL, __pyx_n_s_seleya_mfc_alchemy_qrank_glassdo, __pyx_d, ((PyObject *)__pyx_codeobj__8)); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 42, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
   if (__Pyx_SetNameInClass(__pyx_t_2, __pyx_n_s_fetch_reviews, __pyx_t_3) < 0) __PYX_ERR(0, 42, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
 
-  /* "seleya/mfc/alchemy/qrank/glassdoor.py":63
+  /* "seleya/mfc/alchemy/qrank/glassdoor.pyx":63
  *         return gd_reviews_data
  * 
  *     def prepare_data(self, begin_date=None, end_date=None):             # <<<<<<<<<<<<<<
  *         kd_logger.info('Fetching industry data...')
  *         industry_data = SurfaceDBAPI.Industry().fetch(
  */
-  __pyx_t_3 = __Pyx_CyFunction_New(&__pyx_mdef_6seleya_3mfc_7alchemy_5qrank_8glassdoo_9Glassdoor_7prepare_data, 0, __pyx_n_s_Glassdoor_prepare_data, NULL, __pyx_n_s_seleya_mfc_alchemy_qrank_glassdo, __pyx_d, ((PyObject *)__pyx_codeobj__10)); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 63, __pyx_L1_error)
+  __pyx_t_3 = __Pyx_CyFunction_New(&__pyx_mdef_6seleya_3mfc_7alchemy_5qrank_9glassdoor_9Glassdoor_7prepare_data, 0, __pyx_n_s_Glassdoor_prepare_data, NULL, __pyx_n_s_seleya_mfc_alchemy_qrank_glassdo, __pyx_d, ((PyObject *)__pyx_codeobj__10)); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 63, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
   __Pyx_CyFunction_SetDefaultsTuple(__pyx_t_3, __pyx_tuple__11);
   if (__Pyx_SetNameInClass(__pyx_t_2, __pyx_n_s_prepare_data, __pyx_t_3) < 0) __PYX_ERR(0, 63, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
 
-  /* "seleya/mfc/alchemy/qrank/glassdoor.py":92
+  /* "seleya/mfc/alchemy/qrank/glassdoor.pyx":92
  *         return total_data
  * 
  *     def _transform_raw(self, mean_data):             # <<<<<<<<<<<<<<
  *         # save the raw average scores for UI use
  *         raw_data = mean_data.reset_index().set_index([
  */
-  __pyx_t_3 = __Pyx_CyFunction_New(&__pyx_mdef_6seleya_3mfc_7alchemy_5qrank_8glassdoo_9Glassdoor_9_transform_raw, 0, __pyx_n_s_Glassdoor__transform_raw, NULL, __pyx_n_s_seleya_mfc_alchemy_qrank_glassdo, __pyx_d, ((PyObject *)__pyx_codeobj__13)); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 92, __pyx_L1_error)
+  __pyx_t_3 = __Pyx_CyFunction_New(&__pyx_mdef_6seleya_3mfc_7alchemy_5qrank_9glassdoor_9Glassdoor_9_transform_raw, 0, __pyx_n_s_Glassdoor__transform_raw, NULL, __pyx_n_s_seleya_mfc_alchemy_qrank_glassdo, __pyx_d, ((PyObject *)__pyx_codeobj__13)); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 92, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
   if (__Pyx_SetNameInClass(__pyx_t_2, __pyx_n_s_transform_raw, __pyx_t_3) < 0) __PYX_ERR(0, 92, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
 
-  /* "seleya/mfc/alchemy/qrank/glassdoor.py":106
+  /* "seleya/mfc/alchemy/qrank/glassdoor.pyx":106
  *         return raw_data
  * 
  *     def _blom_score(self, values_series, threshold=0.9):             # <<<<<<<<<<<<<<
  *         idx = values_series.index.droplevel(level=0)
  *         coverage = values_series.isna().sum() / len(values_series)
  */
-  __pyx_t_3 = __Pyx_CyFunction_New(&__pyx_mdef_6seleya_3mfc_7alchemy_5qrank_8glassdoo_9Glassdoor_11_blom_score, 0, __pyx_n_s_Glassdoor__blom_score, NULL, __pyx_n_s_seleya_mfc_alchemy_qrank_glassdo, __pyx_d, ((PyObject *)__pyx_codeobj__16)); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 106, __pyx_L1_error)
+  __pyx_t_3 = __Pyx_CyFunction_New(&__pyx_mdef_6seleya_3mfc_7alchemy_5qrank_9glassdoor_9Glassdoor_11_blom_score, 0, __pyx_n_s_Glassdoor__blom_score, NULL, __pyx_n_s_seleya_mfc_alchemy_qrank_glassdo, __pyx_d, ((PyObject *)__pyx_codeobj__16)); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 106, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
   __Pyx_CyFunction_SetDefaultsTuple(__pyx_t_3, __pyx_tuple__17);
   if (__Pyx_SetNameInClass(__pyx_t_2, __pyx_n_s_blom_score, __pyx_t_3) < 0) __PYX_ERR(0, 106, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
 
-  /* "seleya/mfc/alchemy/qrank/glassdoor.py":119
+  /* "seleya/mfc/alchemy/qrank/glassdoor.pyx":119
  *         return scores
  * 
  *     def _distribute(self, mean_data):             # <<<<<<<<<<<<<<
  *         dt = mean_data.set_index(['date', 'code', 'name'])['value']
  *         res = []
  */
-  __pyx_t_3 = __Pyx_CyFunction_New(&__pyx_mdef_6seleya_3mfc_7alchemy_5qrank_8glassdoo_9Glassdoor_13_distribute, 0, __pyx_n_s_Glassdoor__distribute, NULL, __pyx_n_s_seleya_mfc_alchemy_qrank_glassdo, __pyx_d, ((PyObject *)__pyx_codeobj__19)); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 119, __pyx_L1_error)
+  __pyx_t_3 = __Pyx_CyFunction_New(&__pyx_mdef_6seleya_3mfc_7alchemy_5qrank_9glassdoor_9Glassdoor_13_distribute, 0, __pyx_n_s_Glassdoor__distribute, NULL, __pyx_n_s_seleya_mfc_alchemy_qrank_glassdo, __pyx_d, ((PyObject *)__pyx_codeobj__19)); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 119, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
   if (__Pyx_SetNameInClass(__pyx_t_2, __pyx_n_s_distribute, __pyx_t_3) < 0) __PYX_ERR(0, 119, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
 
-  /* "seleya/mfc/alchemy/qrank/glassdoor.py":127
+  /* "seleya/mfc/alchemy/qrank/glassdoor.pyx":127
  *         return dt
  * 
  *     def _percentile(self, x, res):             # <<<<<<<<<<<<<<
  *         name = str(x.name)
  *         x = x.dropna()
  */
-  __pyx_t_3 = __Pyx_CyFunction_New(&__pyx_mdef_6seleya_3mfc_7alchemy_5qrank_8glassdoo_9Glassdoor_15_percentile, 0, __pyx_n_s_Glassdoor__percentile, NULL, __pyx_n_s_seleya_mfc_alchemy_qrank_glassdo, __pyx_d, ((PyObject *)__pyx_codeobj__21)); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 127, __pyx_L1_error)
+  __pyx_t_3 = __Pyx_CyFunction_New(&__pyx_mdef_6seleya_3mfc_7alchemy_5qrank_9glassdoor_9Glassdoor_15_percentile, 0, __pyx_n_s_Glassdoor__percentile, NULL, __pyx_n_s_seleya_mfc_alchemy_qrank_glassdo, __pyx_d, ((PyObject *)__pyx_codeobj__21)); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 127, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
   if (__Pyx_SetNameInClass(__pyx_t_2, __pyx_n_s_percentile, __pyx_t_3) < 0) __PYX_ERR(0, 127, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
 
-  /* "seleya/mfc/alchemy/qrank/glassdoor.py":135
+  /* "seleya/mfc/alchemy/qrank/glassdoor.pyx":135
  *         res.append(rt.reset_index().set_index(['date', 'code']))
  * 
  *     def _calculate_distribute(self, mean_data):             # <<<<<<<<<<<<<<
  *         kd_logger.info('calculating distribute...')
  *         mean_data['date'] = pd.to_datetime(mean_data['date'])
  */
-  __pyx_t_3 = __Pyx_CyFunction_New(&__pyx_mdef_6seleya_3mfc_7alchemy_5qrank_8glassdoo_9Glassdoor_17_calculate_distribute, 0, __pyx_n_s_Glassdoor__calculate_distribute, NULL, __pyx_n_s_seleya_mfc_alchemy_qrank_glassdo, __pyx_d, ((PyObject *)__pyx_codeobj__23)); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 135, __pyx_L1_error)
+  __pyx_t_3 = __Pyx_CyFunction_New(&__pyx_mdef_6seleya_3mfc_7alchemy_5qrank_9glassdoor_9Glassdoor_17_calculate_distribute, 0, __pyx_n_s_Glassdoor__calculate_distribute, NULL, __pyx_n_s_seleya_mfc_alchemy_qrank_glassdo, __pyx_d, ((PyObject *)__pyx_codeobj__23)); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 135, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
   if (__Pyx_SetNameInClass(__pyx_t_2, __pyx_n_s_calculate_distribute, __pyx_t_3) < 0) __PYX_ERR(0, 135, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
 
-  /* "seleya/mfc/alchemy/qrank/glassdoor.py":148
+  /* "seleya/mfc/alchemy/qrank/glassdoor.pyx":148
  *         return dist_data
  * 
  *     def _format_mean(self, mean_data):             # <<<<<<<<<<<<<<
  *         mean_data['industry'] = self._industry_code
  *         mean_data['date'] = mean_data['date'].dt.strftime('%Y-%m-%d')
  */
-  __pyx_t_3 = __Pyx_CyFunction_New(&__pyx_mdef_6seleya_3mfc_7alchemy_5qrank_8glassdoo_9Glassdoor_19_format_mean, 0, __pyx_n_s_Glassdoor__format_mean, NULL, __pyx_n_s_seleya_mfc_alchemy_qrank_glassdo, __pyx_d, ((PyObject *)__pyx_codeobj__25)); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 148, __pyx_L1_error)
+  __pyx_t_3 = __Pyx_CyFunction_New(&__pyx_mdef_6seleya_3mfc_7alchemy_5qrank_9glassdoor_9Glassdoor_19_format_mean, 0, __pyx_n_s_Glassdoor__format_mean, NULL, __pyx_n_s_seleya_mfc_alchemy_qrank_glassdo, __pyx_d, ((PyObject *)__pyx_codeobj__25)); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 148, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
   if (__Pyx_SetNameInClass(__pyx_t_2, __pyx_n_s_format_mean, __pyx_t_3) < 0) __PYX_ERR(0, 148, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
 
-  /* "seleya/mfc/alchemy/qrank/glassdoor.py":153
+  /* "seleya/mfc/alchemy/qrank/glassdoor.pyx":153
  *         return mean_data
  * 
  *     def calculate_result(self, total_data, threshold=0.9):             # <<<<<<<<<<<<<<
  *         # aggregate means by year and cid
  *         mean_data = total_data.groupby(['date', 'code']).mean()
  */
-  __pyx_t_3 = __Pyx_CyFunction_New(&__pyx_mdef_6seleya_3mfc_7alchemy_5qrank_8glassdoo_9Glassdoor_21calculate_result, 0, __pyx_n_s_Glassdoor_calculate_result, NULL, __pyx_n_s_seleya_mfc_alchemy_qrank_glassdo, __pyx_d, ((PyObject *)__pyx_codeobj__27)); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 153, __pyx_L1_error)
+  __pyx_t_3 = __Pyx_CyFunction_New(&__pyx_mdef_6seleya_3mfc_7alchemy_5qrank_9glassdoor_9Glassdoor_21calculate_result, 0, __pyx_n_s_Glassdoor_calculate_result, NULL, __pyx_n_s_seleya_mfc_alchemy_qrank_glassdo, __pyx_d, ((PyObject *)__pyx_codeobj__27)); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 153, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
   __Pyx_CyFunction_SetDefaultsTuple(__pyx_t_3, __pyx_tuple__28);
   if (__Pyx_SetNameInClass(__pyx_t_2, __pyx_n_s_calculate_result, __pyx_t_3) < 0) __PYX_ERR(0, 153, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
 
-  /* "seleya/mfc/alchemy/qrank/glassdoor.py":183
+  /* "seleya/mfc/alchemy/qrank/glassdoor.pyx":183
  *         return raw_data, self._format_mean(mean_data), dist_data
  * 
  *     def run(self, begin_date, end_date, threshold=0.9):             # <<<<<<<<<<<<<<
  *         total_data = self.prepare_data(begin_date, end_date)
  *         if total_data is None or total_data.empty:
  */
-  __pyx_t_3 = __Pyx_CyFunction_New(&__pyx_mdef_6seleya_3mfc_7alchemy_5qrank_8glassdoo_9Glassdoor_23run, 0, __pyx_n_s_Glassdoor_run, NULL, __pyx_n_s_seleya_mfc_alchemy_qrank_glassdo, __pyx_d, ((PyObject *)__pyx_codeobj__30)); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 183, __pyx_L1_error)
+  __pyx_t_3 = __Pyx_CyFunction_New(&__pyx_mdef_6seleya_3mfc_7alchemy_5qrank_9glassdoor_9Glassdoor_23run, 0, __pyx_n_s_Glassdoor_run, NULL, __pyx_n_s_seleya_mfc_alchemy_qrank_glassdo, __pyx_d, ((PyObject *)__pyx_codeobj__30)); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 183, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
   __Pyx_CyFunction_SetDefaultsTuple(__pyx_t_3, __pyx_tuple__31);
   if (__Pyx_SetNameInClass(__pyx_t_2, __pyx_n_s_run, __pyx_t_3) < 0) __PYX_ERR(0, 183, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
 
-  /* "seleya/mfc/alchemy/qrank/glassdoor.py":11
+  /* "seleya/mfc/alchemy/qrank/glassdoor.pyx":11
  * 
  * 
  * class Glassdoor(object):             # <<<<<<<<<<<<<<
  * 
  *     def __init__(self, industry_code):
  */
   __pyx_t_3 = __Pyx_Py3ClassCreate(__pyx_t_1, __pyx_n_s_Glassdoor, __pyx_tuple__2, __pyx_t_2, NULL, 0, 1); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 11, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
   if (PyDict_SetItem(__pyx_d, __pyx_n_s_Glassdoor, __pyx_t_3) < 0) __PYX_ERR(0, 11, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
 
-  /* "seleya/mfc/alchemy/qrank/glassdoor.py":1
+  /* "seleya/mfc/alchemy/qrank/glassdoor.pyx":1
  * # -*- coding: utf-8 -*-             # <<<<<<<<<<<<<<
  * import numpy as np
  * import pandas as pd
  */
   __pyx_t_1 = __Pyx_PyDict_NewPresized(0); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 1, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   if (PyDict_SetItem(__pyx_d, __pyx_n_s_test, __pyx_t_1) < 0) __PYX_ERR(0, 1, __pyx_L1_error)
@@ -8478,19 +8478,19 @@
   goto __pyx_L0;
   __pyx_L1_error:;
   __Pyx_XDECREF(__pyx_t_1);
   __Pyx_XDECREF(__pyx_t_2);
   __Pyx_XDECREF(__pyx_t_3);
   if (__pyx_m) {
     if (__pyx_d) {
-      __Pyx_AddTraceback("init seleya.mfc.alchemy.qrank.glassdoo", __pyx_clineno, __pyx_lineno, __pyx_filename);
+      __Pyx_AddTraceback("init seleya.mfc.alchemy.qrank.glassdoor", __pyx_clineno, __pyx_lineno, __pyx_filename);
     }
     Py_CLEAR(__pyx_m);
   } else if (!PyErr_Occurred()) {
-    PyErr_SetString(PyExc_ImportError, "init seleya.mfc.alchemy.qrank.glassdoo");
+    PyErr_SetString(PyExc_ImportError, "init seleya.mfc.alchemy.qrank.glassdoor");
   }
   __pyx_L0:;
   __Pyx_RefNannyFinishContext();
   #if CYTHON_PEP489_MULTI_PHASE_INIT
   return (__pyx_m != NULL) ? 0 : -1;
   #elif PY_MAJOR_VERSION >= 3
   return __pyx_m;
```

### Comparing `Finance-Seleya-1.1.3/seleya/mfc/alchemy/sbti/emission.py` & `Finance-Seleya-1.1.4/seleya/mfc/alchemy/sbti/emission.pyx`

 * *Files identical despite different names*

### Comparing `Finance-Seleya-1.1.3/seleya/mfc/alchemy/tsi/aerosol.py` & `Finance-Seleya-1.1.4/seleya/mfc/alchemy/tsi/aerosol.pyx`

 * *Files identical despite different names*

### Comparing `Finance-Seleya-1.1.3/seleya/mfc/alchemy/tsi/s2f.py` & `Finance-Seleya-1.1.4/seleya/mfc/alchemy/tsi/s2f.pyx`

 * *Files identical despite different names*

### Comparing `Finance-Seleya-1.1.3/seleya/utilities/api_base.py` & `Finance-Seleya-1.1.4/seleya/utilities/api_base.py`

 * *Files identical despite different names*

### Comparing `Finance-Seleya-1.1.3/seleya/utilities/kd_logger.py` & `Finance-Seleya-1.1.4/seleya/utilities/kd_logger.py`

 * *Files identical despite different names*

