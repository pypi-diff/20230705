# Comparing `tmp/cannlytics-0.0.8.tar.gz` & `tmp/cannlytics-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\cannlytics-0.0.8.tar", last modified: Sat Aug 21 17:04:39 2021, max compression
+gzip compressed data, was "dist\cannlytics-0.0.9.tar", last modified: Mon Jan 10 16:31:05 2022, max compression
```

## Comparing `cannlytics-0.0.8.tar` & `cannlytics-0.0.9.tar`

### file list

```diff
@@ -1,53 +1,95 @@
-drwxrwxrwx   0        0        0        0 2021-08-21 17:04:39.356179 cannlytics-0.0.8/
--rw-rw-rw-   0        0        0    35821 2021-04-28 15:00:05.000000 cannlytics-0.0.8/LICENSE
--rw-rw-rw-   0        0        0      775 2021-08-21 17:04:39.356067 cannlytics-0.0.8/PKG-INFO
--rw-rw-rw-   0        0        0     2973 2021-08-21 17:03:18.000000 cannlytics-0.0.8/README.md
-drwxrwxrwx   0        0        0        0 2021-08-21 17:04:39.010861 cannlytics-0.0.8/cannlytics/
--rw-rw-rw-   0        0        0        0 2021-05-31 15:31:07.000000 cannlytics-0.0.8/cannlytics/__init__.py
--rw-rw-rw-   0        0        0    28924 2021-08-05 15:16:14.000000 cannlytics-0.0.8/cannlytics/firebase.py
-drwxrwxrwx   0        0        0        0 2021-08-21 17:04:39.162685 cannlytics-0.0.8/cannlytics/lims/
--rw-rw-rw-   0        0        0      747 2021-07-19 22:56:58.000000 cannlytics-0.0.8/cannlytics/lims/__init__.py
--rw-rw-rw-   0        0        0     7001 2021-07-26 00:06:33.000000 cannlytics-0.0.8/cannlytics/lims/calculations.py
--rw-rw-rw-   0        0        0    17026 2021-08-21 00:00:56.000000 cannlytics-0.0.8/cannlytics/lims/certificates.py
--rw-rw-rw-   0        0        0     7540 2021-08-12 01:50:28.000000 cannlytics-0.0.8/cannlytics/lims/data.py
--rw-rw-rw-   0        0        0    13843 2021-08-21 16:35:15.000000 cannlytics-0.0.8/cannlytics/lims/instruments.py
--rw-rw-rw-   0        0        0     1198 2021-07-25 23:48:30.000000 cannlytics-0.0.8/cannlytics/lims/qc.py
--rw-rw-rw-   0        0        0     7693 2021-08-12 01:48:10.000000 cannlytics-0.0.8/cannlytics/lims/results.py
--rw-rw-rw-   0        0        0      482 2021-08-10 18:00:45.000000 cannlytics-0.0.8/cannlytics/lims/samples.py
--rw-rw-rw-   0        0        0     1064 2021-07-25 23:48:56.000000 cannlytics-0.0.8/cannlytics/lims/stats.py
--rw-rw-rw-   0        0        0     1097 2021-08-10 18:05:21.000000 cannlytics-0.0.8/cannlytics/lims/transfers.py
--rw-rw-rw-   0        0        0     8744 2021-08-10 17:42:44.000000 cannlytics-0.0.8/cannlytics/lims/worksheets.py
--rw-rw-rw-   0        0        0    14436 2021-07-25 23:25:29.000000 cannlytics-0.0.8/cannlytics/models.py
-drwxrwxrwx   0        0        0        0 2021-08-21 17:04:39.162685 cannlytics-0.0.8/cannlytics/traceability/
--rw-rw-rw-   0        0        0        0 2021-05-31 15:31:07.000000 cannlytics-0.0.8/cannlytics/traceability/__init__.py
-drwxrwxrwx   0        0        0        0 2021-08-21 17:04:39.224030 cannlytics-0.0.8/cannlytics/traceability/leaf/
--rw-rw-rw-   0        0        0      647 2021-05-31 15:31:07.000000 cannlytics-0.0.8/cannlytics/traceability/leaf/__init__.py
--rw-rw-rw-   0        0        0    43186 2021-06-15 12:44:41.000000 cannlytics-0.0.8/cannlytics/traceability/leaf/client.py
--rw-rw-rw-   0        0        0      946 2021-05-31 15:31:07.000000 cannlytics-0.0.8/cannlytics/traceability/leaf/exceptions.py
--rw-rw-rw-   0        0        0    16724 2021-05-31 15:31:07.000000 cannlytics-0.0.8/cannlytics/traceability/leaf/models.py
--rw-rw-rw-   0        0        0     3300 2021-05-31 15:31:07.000000 cannlytics-0.0.8/cannlytics/traceability/leaf/urls.py
--rw-rw-rw-   0        0        0     5879 2021-06-15 12:44:41.000000 cannlytics-0.0.8/cannlytics/traceability/leaf/utils.py
-drwxrwxrwx   0        0        0        0 2021-08-21 17:04:39.279744 cannlytics-0.0.8/cannlytics/traceability/metrc/
--rw-rw-rw-   0        0        0      981 2021-05-31 15:31:07.000000 cannlytics-0.0.8/cannlytics/traceability/metrc/__init__.py
--rw-rw-rw-   0        0        0    43460 2021-07-25 22:35:58.000000 cannlytics-0.0.8/cannlytics/traceability/metrc/client.py
--rw-rw-rw-   0        0        0     1240 2021-07-25 23:27:00.000000 cannlytics-0.0.8/cannlytics/traceability/metrc/exceptions.py
--rw-rw-rw-   0        0        0    43064 2021-07-29 13:04:01.000000 cannlytics-0.0.8/cannlytics/traceability/metrc/models.py
--rw-rw-rw-   0        0        0     1376 2021-07-25 23:27:20.000000 cannlytics-0.0.8/cannlytics/traceability/metrc/urls.py
--rw-rw-rw-   0        0        0    18800 2021-07-25 23:27:34.000000 cannlytics-0.0.8/cannlytics/traceability/metrc/utils.py
-drwxrwxrwx   0        0        0        0 2021-08-21 17:04:39.339362 cannlytics-0.0.8/cannlytics/utils/
--rw-rw-rw-   0        0        0        0 2021-05-31 15:31:07.000000 cannlytics-0.0.8/cannlytics/utils/__init__.py
--rw-rw-rw-   0        0        0      489 2021-06-23 22:04:53.000000 cannlytics-0.0.8/cannlytics/utils/emails.py
--rw-rw-rw-   0        0        0     5509 2021-05-31 15:31:07.000000 cannlytics-0.0.8/cannlytics/utils/find_labs.py
--rw-rw-rw-   0        0        0     2688 2021-05-31 15:31:07.000000 cannlytics-0.0.8/cannlytics/utils/firebase_metrc_sync.py
--rw-rw-rw-   0        0        0     2977 2021-07-26 00:48:33.000000 cannlytics-0.0.8/cannlytics/utils/logistics.py
--rw-rw-rw-   0        0        0     5609 2021-05-31 15:31:07.000000 cannlytics-0.0.8/cannlytics/utils/scraper.py
--rw-rw-rw-   0        0        0     1563 2021-05-31 15:31:07.000000 cannlytics-0.0.8/cannlytics/utils/upload_labs.py
--rw-rw-rw-   0        0        0     2300 2021-07-25 19:54:16.000000 cannlytics-0.0.8/cannlytics/utils/utils.py
-drwxrwxrwx   0        0        0        0 2021-08-21 17:04:39.045707 cannlytics-0.0.8/cannlytics.egg-info/
--rw-rw-rw-   0        0        0      775 2021-08-21 17:04:38.000000 cannlytics-0.0.8/cannlytics.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1327 2021-08-21 17:04:38.000000 cannlytics-0.0.8/cannlytics.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2021-08-21 17:04:38.000000 cannlytics-0.0.8/cannlytics.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       55 2021-08-21 17:04:38.000000 cannlytics-0.0.8/cannlytics.egg-info/requires.txt
--rw-rw-rw-   0        0        0       11 2021-08-21 17:04:38.000000 cannlytics-0.0.8/cannlytics.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2021-08-21 17:04:39.356179 cannlytics-0.0.8/setup.cfg
--rw-rw-rw-   0        0        0     1361 2021-08-21 17:01:20.000000 cannlytics-0.0.8/setup.py
+drwxrwxrwx   0        0        0        0 2022-01-10 16:31:05.794274 cannlytics-0.0.9/
+-rw-rw-rw-   0        0        0     1079 2022-01-10 15:20:46.000000 cannlytics-0.0.9/LICENSE
+-rw-rw-rw-   0        0        0     6720 2022-01-10 16:31:05.794274 cannlytics-0.0.9/PKG-INFO
+-rw-rw-rw-   0        0        0     6024 2022-01-10 16:04:09.000000 cannlytics-0.0.9/README.md
+drwxrwxrwx   0        0        0        0 2022-01-10 16:31:05.610142 cannlytics-0.0.9/cannlytics/
+-rw-rw-rw-   0        0        0      493 2022-01-10 14:54:34.000000 cannlytics-0.0.9/cannlytics/__init__.py
+drwxrwxrwx   0        0        0        0 2022-01-10 16:31:05.645131 cannlytics-0.0.9/cannlytics/auth/
+-rw-rw-rw-   0        0        0        0 2021-05-31 15:31:07.000000 cannlytics-0.0.9/cannlytics/auth/__init__.py
+-rw-rw-rw-   0        0        0    14175 2022-01-10 14:54:34.000000 cannlytics-0.0.9/cannlytics/auth/auth.py
+-rw-rw-rw-   0        0        0     3898 2022-01-10 14:54:34.000000 cannlytics-0.0.9/cannlytics/cannlytics.py
+drwxrwxrwx   0        0        0        0 2022-01-10 16:31:05.649642 cannlytics-0.0.9/cannlytics/charts/
+-rw-rw-rw-   0        0        0        0 2021-05-31 15:31:07.000000 cannlytics-0.0.9/cannlytics/charts/__init__.py
+-rw-rw-rw-   0        0        0     7576 2022-01-10 14:54:34.000000 cannlytics-0.0.9/cannlytics/charts/charts.py
+drwxrwxrwx   0        0        0        0 2022-01-10 16:31:05.652129 cannlytics-0.0.9/cannlytics/crm/
+-rw-rw-rw-   0        0        0        0 2021-05-31 15:31:07.000000 cannlytics-0.0.9/cannlytics/crm/__init__.py
+-rw-rw-rw-   0        0        0      874 2022-01-10 14:54:34.000000 cannlytics-0.0.9/cannlytics/crm/crm.py
+drwxrwxrwx   0        0        0        0 2022-01-10 16:31:05.652129 cannlytics-0.0.9/cannlytics/data/
+-rw-rw-rw-   0        0        0        0 2021-05-31 15:31:07.000000 cannlytics-0.0.9/cannlytics/data/__init__.py
+-rw-rw-rw-   0        0        0     7905 2022-01-10 14:54:34.000000 cannlytics-0.0.9/cannlytics/data/market.py
+-rw-rw-rw-   0        0        0     1489 2022-01-10 14:54:34.000000 cannlytics-0.0.9/cannlytics/exceptions.py
+-rw-rw-rw-   0        0        0    32549 2022-01-10 14:54:34.000000 cannlytics-0.0.9/cannlytics/firebase.py
+drwxrwxrwx   0        0        0        0 2022-01-10 16:31:05.684315 cannlytics-0.0.9/cannlytics/lims/
+-rw-rw-rw-   0        0        0      808 2022-01-10 14:54:34.000000 cannlytics-0.0.9/cannlytics/lims/__init__.py
+-rw-rw-rw-   0        0        0     7091 2022-01-10 14:54:34.000000 cannlytics-0.0.9/cannlytics/lims/calculations.py
+-rw-rw-rw-   0        0        0    17105 2022-01-10 14:54:34.000000 cannlytics-0.0.9/cannlytics/lims/certificates.py
+-rw-rw-rw-   0        0        0    13703 2022-01-10 14:54:34.000000 cannlytics-0.0.9/cannlytics/lims/instruments.py
+-rw-rw-rw-   0        0        0     4856 2022-01-10 14:54:34.000000 cannlytics-0.0.9/cannlytics/lims/lims.py
+-rw-rw-rw-   0        0        0      511 2021-12-21 14:09:48.000000 cannlytics-0.0.9/cannlytics/lims/measurements.py
+-rw-rw-rw-   0        0        0      285 2021-12-23 12:59:06.000000 cannlytics-0.0.9/cannlytics/lims/projects.py
+-rw-rw-rw-   0        0        0     1199 2021-12-21 14:09:47.000000 cannlytics-0.0.9/cannlytics/lims/qc.py
+-rw-rw-rw-   0        0        0     7682 2022-01-10 14:28:55.000000 cannlytics-0.0.9/cannlytics/lims/results.py
+-rw-rw-rw-   0        0        0      483 2021-12-21 14:09:47.000000 cannlytics-0.0.9/cannlytics/lims/samples.py
+-rw-rw-rw-   0        0        0     1065 2021-12-21 14:09:47.000000 cannlytics-0.0.9/cannlytics/lims/stats.py
+-rw-rw-rw-   0        0        0     1136 2021-12-23 00:54:17.000000 cannlytics-0.0.9/cannlytics/lims/transfers.py
+-rw-rw-rw-   0        0        0    10618 2022-01-10 14:54:34.000000 cannlytics-0.0.9/cannlytics/lims/worksheets.py
+drwxrwxrwx   0        0        0        0 2022-01-10 16:31:05.700327 cannlytics-0.0.9/cannlytics/metrc/
+-rw-rw-rw-   0        0        0     1182 2022-01-10 14:54:34.000000 cannlytics-0.0.9/cannlytics/metrc/__init__.py
+-rw-rw-rw-   0        0        0    78692 2022-01-10 14:54:34.000000 cannlytics-0.0.9/cannlytics/metrc/client.py
+-rw-rw-rw-   0        0        0    11558 2022-01-10 14:54:34.000000 cannlytics-0.0.9/cannlytics/metrc/constants.py
+-rw-rw-rw-   0        0        0     1542 2022-01-10 14:54:34.000000 cannlytics-0.0.9/cannlytics/metrc/exceptions.py
+-rw-rw-rw-   0        0        0    61066 2022-01-10 14:54:34.000000 cannlytics-0.0.9/cannlytics/metrc/models.py
+-rw-rw-rw-   0        0        0     1172 2022-01-10 14:54:34.000000 cannlytics-0.0.9/cannlytics/metrc/urls.py
+-rw-rw-rw-   0        0        0     6826 2022-01-10 14:54:34.000000 cannlytics-0.0.9/cannlytics/metrc/utils.py
+drwxrwxrwx   0        0        0        0 2022-01-10 16:31:05.762821 cannlytics-0.0.9/cannlytics/models/
+-rw-rw-rw-   0        0        0     1596 2022-01-10 14:54:34.000000 cannlytics-0.0.9/cannlytics/models/__init__.py
+-rw-rw-rw-   0        0        0      855 2022-01-10 14:54:34.000000 cannlytics-0.0.9/cannlytics/models/analysis.py
+-rw-rw-rw-   0        0        0     1035 2022-01-10 14:54:34.000000 cannlytics-0.0.9/cannlytics/models/analyte.py
+-rw-rw-rw-   0        0        0      764 2022-01-10 14:54:34.000000 cannlytics-0.0.9/cannlytics/models/api_key.py
+-rw-rw-rw-   0        0        0     1058 2022-01-10 14:54:34.000000 cannlytics-0.0.9/cannlytics/models/area.py
+-rw-rw-rw-   0        0        0     1510 2022-01-10 14:54:34.000000 cannlytics-0.0.9/cannlytics/models/base.py
+-rw-rw-rw-   0        0        0      617 2022-01-10 14:54:34.000000 cannlytics-0.0.9/cannlytics/models/batch.py
+-rw-rw-rw-   0        0        0      635 2022-01-10 14:54:34.000000 cannlytics-0.0.9/cannlytics/models/calculation.py
+-rw-rw-rw-   0        0        0      656 2022-01-10 14:54:34.000000 cannlytics-0.0.9/cannlytics/models/cannabis_license.py
+-rw-rw-rw-   0        0        0     1326 2022-01-10 14:54:34.000000 cannlytics-0.0.9/cannlytics/models/certificate.py
+-rw-rw-rw-   0        0        0     1149 2022-01-10 14:54:34.000000 cannlytics-0.0.9/cannlytics/models/contact.py
+-rw-rw-rw-   0        0        0      528 2022-01-10 14:54:34.000000 cannlytics-0.0.9/cannlytics/models/dataset.py
+-rw-rw-rw-   0        0        0      987 2022-01-10 14:54:34.000000 cannlytics-0.0.9/cannlytics/models/instrument.py
+-rw-rw-rw-   0        0        0     1616 2022-01-10 14:54:34.000000 cannlytics-0.0.9/cannlytics/models/inventory_type.py
+-rw-rw-rw-   0        0        0      661 2022-01-10 14:54:34.000000 cannlytics-0.0.9/cannlytics/models/invoice.py
+-rw-rw-rw-   0        0        0     1428 2022-01-10 14:54:34.000000 cannlytics-0.0.9/cannlytics/models/item.py
+-rw-rw-rw-   0        0        0      681 2022-01-10 14:54:34.000000 cannlytics-0.0.9/cannlytics/models/measurement.py
+-rw-rw-rw-   0        0        0      778 2022-01-10 14:54:34.000000 cannlytics-0.0.9/cannlytics/models/organization.py
+-rw-rw-rw-   0        0        0      625 2022-01-10 14:54:34.000000 cannlytics-0.0.9/cannlytics/models/price.py
+-rw-rw-rw-   0        0        0      604 2022-01-10 14:54:34.000000 cannlytics-0.0.9/cannlytics/models/project.py
+-rw-rw-rw-   0        0        0      481 2022-01-10 14:54:34.000000 cannlytics-0.0.9/cannlytics/models/regulation.py
+-rw-rw-rw-   0        0        0      512 2022-01-10 14:54:34.000000 cannlytics-0.0.9/cannlytics/models/report.py
+-rw-rw-rw-   0        0        0     1071 2022-01-10 14:54:34.000000 cannlytics-0.0.9/cannlytics/models/results.py
+-rw-rw-rw-   0        0        0     1245 2022-01-10 14:54:34.000000 cannlytics-0.0.9/cannlytics/models/sample.py
+-rw-rw-rw-   0        0        0     1296 2022-01-10 14:54:34.000000 cannlytics-0.0.9/cannlytics/models/settings.py
+-rw-rw-rw-   0        0        0      663 2022-01-10 14:54:34.000000 cannlytics-0.0.9/cannlytics/models/template.py
+-rw-rw-rw-   0        0        0      888 2022-01-10 14:54:34.000000 cannlytics-0.0.9/cannlytics/models/transfer.py
+-rw-rw-rw-   0        0        0      779 2022-01-10 14:54:34.000000 cannlytics-0.0.9/cannlytics/models/user.py
+-rw-rw-rw-   0        0        0      546 2022-01-10 14:54:34.000000 cannlytics-0.0.9/cannlytics/models/workflow.py
+-rw-rw-rw-   0        0        0     3407 2022-01-10 14:53:02.000000 cannlytics-0.0.9/cannlytics/paypal.py
+drwxrwxrwx   0        0        0        0 2022-01-10 16:31:05.762821 cannlytics-0.0.9/cannlytics/stats/
+-rw-rw-rw-   0        0        0        0 2021-05-31 15:31:07.000000 cannlytics-0.0.9/cannlytics/stats/__init__.py
+-rw-rw-rw-   0        0        0     4737 2022-01-10 14:54:34.000000 cannlytics-0.0.9/cannlytics/stats/arima.py
+-rw-rw-rw-   0        0        0     3359 2022-01-10 14:54:34.000000 cannlytics-0.0.9/cannlytics/stats/var.py
+drwxrwxrwx   0        0        0        0 2022-01-10 16:31:05.778650 cannlytics-0.0.9/cannlytics/utils/
+-rw-rw-rw-   0        0        0      408 2022-01-10 14:54:34.000000 cannlytics-0.0.9/cannlytics/utils/__init__.py
+-rw-rw-rw-   0        0        0     1954 2022-01-10 14:54:34.000000 cannlytics-0.0.9/cannlytics/utils/constants.py
+-rw-rw-rw-   0        0        0      845 2021-12-21 17:51:49.000000 cannlytics-0.0.9/cannlytics/utils/emails.py
+-rw-rw-rw-   0        0        0      980 2022-01-10 14:54:34.000000 cannlytics-0.0.9/cannlytics/utils/files.py
+-rw-rw-rw-   0        0        0     4170 2022-01-10 14:54:34.000000 cannlytics-0.0.9/cannlytics/utils/logistics.py
+-rw-rw-rw-   0        0        0     9946 2022-01-10 14:54:34.000000 cannlytics-0.0.9/cannlytics/utils/utils.py
+-rw-rw-rw-   0        0        0     6824 2022-01-10 14:54:34.000000 cannlytics-0.0.9/cannlytics/utils/web.py
+drwxrwxrwx   0        0        0        0 2022-01-10 16:31:05.639679 cannlytics-0.0.9/cannlytics.egg-info/
+-rw-rw-rw-   0        0        0     6720 2022-01-10 16:31:05.000000 cannlytics-0.0.9/cannlytics.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     2259 2022-01-10 16:31:05.000000 cannlytics-0.0.9/cannlytics.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2022-01-10 16:31:05.000000 cannlytics-0.0.9/cannlytics.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        2 2022-01-10 16:24:50.000000 cannlytics-0.0.9/cannlytics.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0      192 2022-01-10 16:31:05.000000 cannlytics-0.0.9/cannlytics.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       11 2022-01-10 16:31:05.000000 cannlytics-0.0.9/cannlytics.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2022-01-10 16:31:05.794274 cannlytics-0.0.9/setup.cfg
+-rw-rw-rw-   0        0        0     2095 2022-01-10 16:31:02.000000 cannlytics-0.0.9/setup.py
```

### Comparing `cannlytics-0.0.8/cannlytics/firebase.py` & `cannlytics-0.0.9/cannlytics/firebase.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,286 +1,322 @@
 """
 Firebase Module | Cannlytics
+Copyright (c) 2021-2022 Cannlytics
 
-Author: Keegan Skeate <contact@cannlytics.com>  
-Created: 2/7/2021  
-Updated: 7/30/2021  
-
-Resources:
-
-- https://firebase.google.com/docs/
-
-Description:
-
-A wrapper of firebase_admin to make interacting with the Firestore database
-and Firebase Storage buckets even easier.
+Authors: Keegan Skeate <contact@cannlytics.com>
+Created: 2/7/2021
+Updated: 1/10/2022
+License: <https://github.com/cannlytics/cannlytics-engine/blob/main/LICENSE>
+
+Description: A wrapper of `firebase_admin` to make interacting with a Firestore
+database and Firebase Storage buckets even easier. For more information, see
+<https://firebase.google.com/docs/>.
 
 Example:
 
 ```py
-import os
-import environ
+# Get the path to your service account.
+from dotenv import dotenv_values
+config = dotenv_values('./env')
+key_path = config['GOOGLE_APPLICATION_CREDENTIALS']
 
-# Get and set all credentials.
-env = environ.Env()
-env.read_env('.env')
-credentials = env('GOOGLE_APPLICATION_CREDENTIALS')
-os.environ['GOOGLE_APPLICATION_CREDENTIALS'] = credentials
-bucket_name = environ.get('FIREBASE_STORAGE_BUCKET')
-
-# Initialize Firebase
-db = initialize_firebase()
+# Initialize Firebase.
+database = initialize_firebase(key_path)
 ```
 """
-try:
-    # Standard imports
-    from datetime import datetime, timedelta
-    from os import listdir
-    from os.path import isfile, join
-
-    # External imports
-    import requests
-    import ulid
-    from django.utils.crypto import get_random_string
-    from firebase_admin import auth, firestore, initialize_app, storage
-    from google.cloud import secretmanager
-    try:
-        from google.cloud.firestore import ArrayUnion, ArrayRemove, Increment
-        from google.cloud.firestore_v1.collection import CollectionReference
-        from google.cloud.firestore_v1.transforms import DELETE_FIELD
-    except:
-        pass
-    try:
-        from pandas import notnull, read_csv, read_excel, DataFrame, Series
-    except:
-        # FIXME: pandas has problems with Django on Cloud Run
-        pass
-
-    # Internal imports.
-    from cannlytics.utils.utils import snake_case
-except:
-    pass # FIXME: Ignore import in Docs
+# Standard imports
+from datetime import datetime, timedelta
+from os import listdir
+from os.path import isfile, join
+from typing import Any, List, Optional, Tuple
+
+# External imports
+import requests
+import ulid
+from firebase_admin import (
+    auth,
+    credentials,
+    firestore,
+    initialize_app,
+    storage,
+)
+from google.cloud import secretmanager
+from google.cloud.firestore import ArrayUnion, ArrayRemove, Increment
+from google.cloud.firestore_v1.collection import CollectionReference
+from google.cloud.firestore_v1.transforms import DELETE_FIELD
+from pandas import notnull, read_csv, read_excel, DataFrame, Series
+
+# Internal imports.
+from .utils.utils import get_random_string, snake_case
+
+# The maximum number of documents to include in batch updates.
+# The official limit is 500, but pushing too close to the limit
+# increses the likelihood of failure to commit.
+MAX_BATCH_SIZE = 420
 
-# ------------------------------------------------------------#
+#------------------------------------------------------------------------------
 # Firestore
-# FIXME: Pass existing database reference to functions instead
-# of creating a new `firestore.client()` each time.
-# ------------------------------------------------------------#
+#------------------------------------------------------------------------------
 
-def add_to_array(ref, field, value):
+def add_to_array(ref, field, value, database=None):
     """Add an element to a given field for a given reference.
     Args:
         ref (str): A document reference.
         field (str): A list field to create or update.
         value (dynamic): The value to be added to the list.
+        database (Client): An optional existing Firestore database client.
     """
-    database = firestore.client()
+    if database is None:
+        database = firestore.client()
     doc = create_reference(database, ref)
     doc.set({field: ArrayUnion([value])}, merge=True)
 
 
-def create_document(ref, values):
+def create_document(ref, values, database=None):
     """Create a given document with given values, this leverages the
     same functionality as `update_document` thanks to `set` with `merge=True`.
     Args:
         ref (str): A document reference.
         values (str): A dictionary of values to update.
+        database (Client): An optional existing Firestore database client.
     """
-    update_document(ref, values)
+    update_document(ref, values, database)
 
 
 def create_reference(database, path):
     """Create a database reference for a given path.
     Args:
         database (Firestore Client): The Firestore Client.
         path (str): The path to the document or collection.
     Returns:
         (ref): Either a document or collection reference.
     """
     ref = database
     parts = path.split('/')
-    for i in range(len(parts)):
-        part = parts[i]
-        if i % 2:
+    for index, part in enumerate(parts):
+        if index % 2:
             ref = ref.document(part)
         else:
             ref = ref.collection(part)
     return ref
 
 
-def delete_collection(ref, batch_size=420):
+def delete_collection(ref, batch_size=420, database=None):
     """Delete a given collection, a batch at a time.
     Args:
         ref (str): A document reference.
         batch_size (int): The number of documents to delete at a time.
             The default is 420 and the maximum is 500.
+        database (Client): An optional existing Firestore database client.
     """
-    database = firestore.client()
+    if database is None:
+        database = firestore.client()
     col = create_reference(database, ref)
     docs = col.limit(batch_size).stream()
     deleted = 0
     for doc in docs:
         doc.reference.delete()
         deleted = deleted + 1
         if deleted >= batch_size:
             return delete_collection(col, batch_size)
 
 
-def delete_document(ref):
+def delete_document(ref: str, database=None):
     """Delete a given document.
     Args:
         ref (str): A document reference.
+        database (Client): An optional existing Firestore database client.
     """
-    database = firestore.client()
+    if database is None:
+        database = firestore.client()
     doc = create_reference(database, ref)
     doc.delete()
 
 
-def delete_field(ref, field):
+def delete_field(ref: str, field: str, database=None):
     """Delete a given field from a document.
     Args:
         ref (str): A document reference.
         field (str): The field to remove from the document.
+        database (Client): An optional existing Firestore database client.
     """
-    database = firestore.client()
+    if database is None:
+        database = firestore.client()
     doc = create_reference(database, ref)
     doc.set({field: DELETE_FIELD}, merge=True)
 
 
-def remove_from_array(ref, field, value):
+def remove_from_array(ref: str, field: str, value: Any, database=None):
     """Remove an element from a given field for a given reference.
     Args:
         ref (str): A document reference.
         field (str): A list field to update.
         value (dynamic): The value to be removed from the list.
+        database (Client): An optional existing Firestore database client.
     """
-    database = firestore.client()
+    if database is None:
+        database = firestore.client()
     doc = create_reference(database, ref)
     doc.set({field: ArrayRemove([value])}, merge=True)
 
 
-def increment_value(ref, field, amount=1):
+def increment_value(ref: str, field: str, amount: int = 1, database=None):
     """Increment a given field for a given reference.
     Args:
         ref (str): A document reference.
         field (str): A numeric field to create or update.
         amount (int): The amount to increment, default 1.
+        database (Client): An optional existing Firestore database client.
     """
-    database = firestore.client()
+    if database is None:
+        database = firestore.client()
     doc = create_reference(database, ref)
     doc.set({field: Increment(amount)}, merge=True)
 
 
-def initialize_firebase():
-    """Initialize Firebase, unless already initialized.
+def initialize_firebase(
+        key_path: Optional[str] = None,
+        bucket_name: Optional[str] = None,
+        project_id: Optional[str] = None,
+):
+    """Initialize Firebase, unless already initialized. Searches for environment
+    credentials if `key_path` is not specified.
+    Args:
+        key_path (str): A path to your service account credentials (optional).
+        project_id (str): A Firebase project ID (optional).
+        bucket_name (str): A Cloud Storage bucket name (optional).
     Returns:
         (Firestore client): A Firestore database instance.
     """
+    cred = None
+    options = {}
+    if key_path:
+        cred = credentials.Certificate(key_path)
+    if bucket_name:
+        options['storageBucket'] = bucket_name.replace('gs://', '')
+    if project_id:
+        options['projectId'] = project_id
     try:
-        initialize_app()
+        initialize_app(cred, options)
     except ValueError:
         pass
     return firestore.client()
 
 
-def update_document(ref, values):
+def update_document(ref: str, values: dict, database=None):
     """Update a given document with given values.
     Args:
         ref (str): A document reference.
         values (str): A dictionary of values to update.
+        database (Client): An optional existing Firestore database client.
     """
-    database = firestore.client()
+    if database is None:
+        database = firestore.client()
     doc = create_reference(database, ref)
     doc.set(values, merge=True)
 
 
-def update_documents(refs, data):
-    """Batch update documents, up to 420 at a time (to give the 500
-    limit set by Firebase a cushion).
+def update_documents(refs: List[str], data: List[dict], database=None):
+    """Batch update documents, up to the `MAX_BATCH_SIZE`, 420 by default.
     Args:
         refs (list): A list of document paths (str).
         data (list): A list of document data (dict).
+        database (Client): An optional existing Firestore database client.
     """
-    n = 420
-    database = firestore.client()
-    ref_shards = [refs[i:i+n] for i in range(0, len(refs), n)]
-    data_shards = [data[i:i+n] for i in range(0, len(data), n)]
-    for s in range(len(ref_shards)):
-        ref_shard = ref_shards[s]
-        data_shard = data_shards[s]
+    if database is None:
+        database = firestore.client()
+    ref_shards = [refs[i:i + MAX_BATCH_SIZE] for i in range(0, len(refs), MAX_BATCH_SIZE)]
+    data_shards = [data[i:i + MAX_BATCH_SIZE] for i in range(0, len(data), MAX_BATCH_SIZE)]
+    for shard_index, ref_shard in enumerate(ref_shards):
+        data_shard = data_shards[shard_index]
         batch = database.batch()
-        for i in range(len(ref_shard)):
-            ref = ref_shard[i]
-            values = data_shard[i]
+        for index, ref in enumerate(ref_shard):
+            values = data_shard[index]
             doc = create_reference(database, ref)
             batch.set(doc, values, merge=True)
         batch.commit()
 
 
-def get_document(ref):
+def get_document(ref: str, database=None) -> dict:
     """Get a given document.
     Args:
         ref (str): A document reference.
+        database (Client): A Firestore database client.
     Returns:
         (dict): Returns the document as a dictionary.
             Returns an empty dictionary if no data is found.
     """
-    database = firestore.client()
+    if database is None:
+        database = firestore.client()
     doc = create_reference(database, ref)
     data = doc.get()
-    if data is None:
-        return {}
-    else:
+    try:
         values = data.to_dict()
         if values is None:
             return {}
         return {**{'id': data.id}, **values}
+    except AttributeError:
+        return {}
 
 
-def get_collection(ref, limit=None, order_by=None, desc=False, filters=[]):
+def get_collection( #pylint: disable=too-many-arguments
+        ref: str,
+        limit: int = None,
+        order_by: str = None,
+        desc: bool = False,
+        filters: List[dict] = None,
+        database=None,
+        start_at: dict = None,
+) -> List[dict]:
     """Get documents from a collection.
     Args:
         ref (str): A document reference.
         limit (int): The maximum number of documents to return. The default is no limit.
         order_by (str): A field to order the documents by, with the default being none.
         desc (bool): The direction to order the documents by the order_by field.
         filters (list): Filters are dictionaries of the form
             `{'key': '', 'operation': '', 'value': ''}`.
             Filters apply [Firebase queries](https://firebase.google.com/docs/firestore/query-data/queries)
             to the given `key` for the given `value`.
             Operators include: `==`, `>=`, `<=`, `>`, `<`, `!=`,
             `in`, `not_in`, `array_contains`, `array_contains_any`.
+        start_at (dict): Optional starting at value for pagination. Expect a dict
+            of with `key` and `value` fields. For example: `{'key': 'number', 'value': 4 }`.
+        database (Client): A Firestore database client.
     Returns:
         (list): A list of documents.
     """
     docs = []
-    database = firestore.client()
+    if database is None:
+        database = firestore.client()
     collection = create_reference(database, ref)
-    if filters:
-        for filter in filters:
+    if filters is not None:
+        for query_filter in filters:
             collection = collection.where(
-                filter['key'], filter['operation'], filter['value']
+                query_filter['key'], query_filter['operation'], query_filter['value']
             )
     if order_by and desc:
         collection = collection.order_by(order_by, direction='DESCENDING')
     elif order_by:
         collection = collection.order_by(order_by)
+    if start_at:
+        collection = collection.start_after({start_at['key']: start_at['value']})
     if limit:
         collection = collection.limit(limit)
     query = collection.stream()  # Only handles streams less than 2 mins.
     for doc in query:
         data = doc.to_dict()
         docs.append({**{'id': doc.id}, **data})
     return docs
 
 
-def import_data(db, ref, data_file):
+def import_data(database, ref: str, data_file: str):
     """Import data into Firestore.
     Args:
-        db (Firestore Client):
+        database (Firestore Client):
         ref (str): A collection or document reference.
         data_file (str): The path to the local data file to upload.
     !!! info "Wishlist"
         It would be desirable for the following functionality to be implemented:
         - Batch upload
         - Handle types <https://hackersandslackers.com/importing-excel-dates-times-into-pandas/>
     """
@@ -303,29 +339,29 @@
                     encoding='utf-16',
                     sep='\t',
                 )
             except:
                 data = read_excel(data_file, header=0)
     data.columns = map(snake_case, data.columns)
     data = data.where(notnull(data), None)
-    data_ref = create_reference(db, ref)
+    data_ref = create_reference(database, ref)
     if isinstance(data_ref, CollectionReference):
         for index, values in data.iterrows():
             doc_id = str(index)
             doc_data = values.to_dict()
             data_ref.document(doc_id).set(doc_data, merge=True)
     else:
         doc_data = data.to_dict(orient='index')
         data_ref.set(doc_data, merge=True)
 
 
-def export_data(db, ref, data_file):
+def export_data(database, ref: str, data_file: str):
     """Export data from Firestore.    
     Args:
-        db (Firestore Client):
+        database (Firestore Client):
         ref (str): A collection or document reference.
         data_file (str): The path to the local data file to upload.
     !!! info "Wishlist"
         Parse fields that are objects into fields, similar to below.
         ```py
         from pandas.io.json import json_normalize
         artist_and_track = json_normalize(
@@ -334,15 +370,15 @@
             meta=['id'],
             record_prefix='sp_artist_',
             meta_prefix='sp_track_',
             sep='_'
         )
         ```
     """
-    data_ref = create_reference(db, ref)
+    data_ref = create_reference(database, ref)
     if isinstance(data_ref, CollectionReference):
         data = []
         docs = data_ref.stream()
         for doc in docs:
             doc_data = doc.to_dict()
             doc_data['id'] = doc.id
             data.append(doc_data)
@@ -353,55 +389,55 @@
         output.name = doc.id
     if data_file.endswith('.csv'):
         output.to_csv(data_file)
     else:
         output.to_excel(data_file)
 
 
-def create_id():
+def create_id() -> str:
     """Generate a universal ID.
     Returns:
-        (str): A unique, lexicographic ID, a ULID.
+        (str): A unique lexicographic ID.
     """
     return ulid.new().str.lower()
 
 
-def create_id_from_datetime(dt):
+def create_id_from_datetime(timestamp: datetime) -> str:
     """Create an ID from an existing datetime.
     Args:
-        dt (datetime): The time to timestamp the ID.
+        timestamp (datetime): The time to timestamp the ID.
     Returns:
         (str): A unique lexicographic ID.
     """
-    return ulid.from_timestamp(dt)
+    return ulid.from_timestamp(timestamp).str.lower()
 
 
-def get_id_timestamp(uid):
+def get_id_timestamp(uid: str) -> datetime:
     """Get the datetime that an ID was created.
     Args:
         uid (str): A unique ID string.
     Returns:
         (datetime): The date when a unique lexicographic ID was generated.
     """
     return ulid.from_str(uid).timestamp().datetime
 
 
-# ------------------------------------------------------------#
+#------------------------------------------------------------------------------
 # Authentication
-# ------------------------------------------------------------#
+#------------------------------------------------------------------------------
 
-def create_user(name, email):
+def create_user(name: str, email: str) -> Tuple[str]:
     """
     Given user name and email, create an account.
     If the email is already being used, then nothing is returned.
     Args:
         name (str): A name for the user.
         email (str): The user's email.
     Returns:
-        (tuple): User object, random password
+        (tuple): Returns the User instance and a random password.
     """
     chars = 'abcdefghijklmnopqrstuvwxyz0123456789!@#$-_'
     password = get_random_string(42, chars)
     photo_url = f'https://robohash.org/{email}?set=set5'
     try:
         user = auth.create_user(
             uid=create_id(),
@@ -413,122 +449,131 @@
             disabled=False,
         )
         return user, password
     except:
         return None, None
 
 
-def create_custom_claims(uid, email=None, claims=None):
+def create_custom_claims(uid: str , email: str = None, claims: dict = None):
     """Create custom claims for a user to grant granular permission.
     The new custom claims will propagate to the user's ID token the
     next time a new one is issued.
     Args:
         uid (str): A user's ID.
         email (str): A user's email.
         claims (dict): A dictionary of the user's custom claims.
     """
     if email:
         user = auth.get_user_by_email(email)
         uid = user.uid
     auth.set_custom_user_claims(uid, claims)
 
 
-def update_custom_claims(uid, email=None, claims=None):
+def update_custom_claims(uid: str, email: str = None, claims: dict = None):
     """Update custom claims for a user.
     The new custom claims will propagate to the user's ID token the
     next time a new one is issued.
     Args:
         uid (str): A user's ID.
         email (str): A user's email.
         claims (dict): A dictionary of the user's custom claims.
     """
     if email:
         user = auth.get_user_by_email(email)
         uid = user.uid
     existing_claims = get_custom_claims(uid)
-    if existing_claims:
-        existing_owner = existing_claims.get('owner', [])
-    else:
+    if not existing_claims:
         existing_claims = {}
-        existing_owner = []
-    current_owner = claims.get('owner', [])
-    claims['owner'] = list(set(existing_owner + current_owner))
+    # if existing_claims:
+    #     existing_owner = existing_claims.get('owner', [])
+    # else:
+    #     existing_claims = {}
+    #     existing_owner = []
+    # current_owner = claims.get('owner', [])
+    # FIXME: For now, only 1 organization per user.
+    # claims['owner'] = list(set(existing_owner + current_owner))
     auth.set_custom_user_claims(uid, {**existing_claims, **claims})
 
 
-def get_custom_claims(name):
+def get_custom_claims(name: str) -> dict:
     """Get custom claims for a user.
     Args:
         name (str): A user ID or user email.
     """
     user = get_user(name)
     return user.custom_claims
 
 
-def create_custom_token(uid='', email=None, claims=None):
+def create_custom_token(
+        uid: Optional[str] = '',
+        email: Optional[str] = None,
+        claims: Optional[dict] = None
+) -> bytes:
     """Create a custom token for a given user, expires after one hour.
     Args:
         uid (str): A user's ID.
         email (str): A user's email.
         claims (dict):  A dictionary of the user's claims.
     Returns:
-        (dict): A dictionary of custom claims.
+        (bytes): A token minted from the input parameters.
     """
     if email:
         user = auth.get_user_by_email(email)
         uid = user.uid
     return auth.create_custom_token(uid, claims)
 
 
-def create_session_cookie(id_token, expires_in=None):
+def create_session_cookie(id_token: str, expires_in: timedelta = None) -> bytes:
     """Create a session cookie.
     Args:
         id_token (str): A user ID token passed from the client.
         expires_in (timedelta): The time until the session will expire.
     Returns:
         (bytes): A session cookie in bytes.
     """
     if expires_in is None:
         expires_in = timedelta(days=7)
     return auth.create_session_cookie(id_token, expires_in=expires_in)
 
 
-def revoke_refresh_tokens(token):
+def revoke_refresh_tokens(token: str):
     """Revoke a user's refresh token.
     Args:
         token (str): The refresh token to authenticate a user.
     """
-    return auth.revoke_refresh_tokens(token)
+    auth.revoke_refresh_tokens(token)
 
 
-def verify_token(token):
+def verify_token(token: str) -> dict:
     """Verify a user's custom token.
     Args:
         token (str): The custom token to authenticate a user.
     Returns:
         (dict): A dictionary of key-value pairs parsed from the decoded JWT.
     """
     return auth.verify_id_token(token)
 
 
-def verify_session_cookie(session_cookie, check_revoked=True, app=None): # FIXME: Don't hardcode
+def verify_session_cookie(session_cookie: str, check_revoked: bool = True, app=None) -> dict:
     """Verify a user's session cookie.
     Args:
         session_cookie (str): A session cookie to authenticate a user.
+        check_revoked (bool): Checks if the cookie has been revoked or not (optional).
+        app (App): A Firebase App instance.
     Returns:
         (dict): A dictionary of key-value pairs parsed from the decoded JWT.
     """
     return auth.verify_session_cookie(
         session_cookie,
         check_revoked=check_revoked,
         app=app,
     )
 
 
-def get_user(name):
+def get_user(name: str) -> Any:
     """Get a user by user ID or by email.
     Args:
         name (str): A user ID, email, or phone number.
     Returns:
         (UserRecord): A Firebase user object.
     """
     user = None
@@ -545,42 +590,36 @@
         try:
             user = auth.get_user_by_phone_number(name)
         except:
             pass
     return user
 
 
-def get_users():
+def get_users() -> list:
     """Get all Firebase users.
     Returns:
         (list): A list of Firebase users.
     """
     users = []
     for user in auth.list_users().iterate_all():
         users.append(user)
     return users
 
 
-def update_user(existing_user, data):
+def update_user(existing_user: Any, data: dict):
     """Update a user.
     Args:
-        existing_user (Firebase user):
+        existing_user (Firebase user): A Firebase user object.
         data (dict): The values of the user to update, which can include
             email, phone_number, email_verified, diplay_name, photo_url,
             and disabled.
     """
     values = {}
-    fields = [
-        'email',
-        'phone_number',
-        'email_verified',
-        'display_name',
-        'photo_url',
-        'disabled',
-    ]
+    fields = ['email', 'phone_number', 'email_verified', 'display_name',
+              'photo_url', 'disabled']
     for field in fields:
         new_value = data.get(field)
         if new_value:
             values[field] = new_value
         else:
             values[field] = getattr(existing_user, field)
     return auth.update_user(
@@ -590,103 +629,110 @@
         email_verified=values['email_verified'],
         display_name=values['display_name'],
         photo_url=values['photo_url'],
         disabled=values['disabled'],
     )
 
 
-def delete_user(uid):
+def delete_user(uid: str):
     """Delete a user from Firebase.
     Args:
         uid (str): A user's ID.
     """
     auth.delete_user(uid)
 
 
-# Optional: Implement custom password-reset email.
-# def send_password_reset(email):
-#     """Send a password reset to a user given an email."""
-#     link = auth.generate_password_reset_link(email)
-#     send_custom_email(email, link)
+def generate_password_reset_link(email: str) -> str:
+    """Get a password reset link for a user given their email.
+    Args:
+        email (str): A user's email.
+    Returns:
+        (str): A password reset link for the user.
+    """
+    return auth.generate_password_reset_link(email)
 
 
-# ------------------------------------------------------------#
+#------------------------------------------------------------------------------
 # Secret Management
-# 'Secret Manager Admin' permissions needed for service account.
-# https://cloud.google.com/secret-manager/docs/creating-and-accessing-secrets
-# ------------------------------------------------------------#
+#------------------------------------------------------------------------------
 
-def create_secret(project_id, secret_id, secret):
+def create_secret(project_id: str, secret_id: str, secret: Any) -> str:
     """Create a new secret with the given name. A secret is a logical wrapper
     around a collection of secret versions. Secret versions hold the actual
-    secret material.
+    secret material. 'Secret Manager Admin' permissions needed for service account.
+    See <https://cloud.google.com/secret-manager/docs/creating-and-accessing-secrets>.
     Args:
         project_id (str): The project associated with the secret.
         secret_id (str): An ID for the secret.
-        secret (str): The secret data.
+        secret (dynamic): The secret data, a string or a dict can both be used.
+    Returns:
+        (str): The name of the created secret.
     """
     client = secretmanager.SecretManagerServiceClient()
     parent = f'projects/{project_id}'
-    response = client.create_secret(parent, secret_id, {"replication": {"automatic": {}}})
+    response = client.create_secret(parent, secret_id, secret)
     return response.name
 
 
-def add_secret_version(project_id, secret_id, payload):
+def add_secret_version(project_id: str, secret_id: str, payload: Any) -> str:
     """
     Add a new secret version to the given secret with the provided payload.
     A secret version contains the actual contents of a secret.
     A secret version can be enabled, disabled, or destroyed.
     To change the contents of a secret, you create a new version.
     Adding a secret version requires the Secret Manager Admin role
     (roles/secretmanager.admin) on the secret, project, folder, or organization.
     Roles can't be granted on a secret version.
+    'Secret Manager Admin' permissions needed for service account.
+    See <https://cloud.google.com/secret-manager/docs/creating-and-accessing-secrets>.
     Args:
         project_id (str): A Firestore project ID.
         secret_id (str): An ID for the secret.
-        payload (str): The secret.
+        payload (dynamic): The secret.
     Returns:
         (str): The secret version's name.
     """
     client = secretmanager.SecretManagerServiceClient()
     parent = f'projects/{project_id}/secrets/{secret_id}'
     payload = payload.encode('UTF-8')
     response = client.add_secret_version(parent, {'data': payload})
     return response.name
 
 
-def access_secret_version(project_id, secret_id, version_id):
+def access_secret_version(project_id: str, secret_id: str, version_id: str) -> str:
     """
     Access the payload for a given secret version if one exists. The version
     can be a version number as a string (e.g. "5") or an alias (e.g. "latest").
+    'Secret Manager Admin' permissions needed for service account.
+    See <https://cloud.google.com/secret-manager/docs/creating-and-accessing-secrets>.
     !!! Warning
         Do not print the secret in a production environment.
     Args:
         project_id (str): A Firestore project ID.
         secret_id (str): An ID for the secret.
         version_id (str): A version for the secret.
     Returns:
-        (str): The secret version's name.
+        (str): The secret value.
     """
     client = secretmanager.SecretManagerServiceClient()
     name = f'projects/{project_id}/secrets/{secret_id}/versions/{version_id}'
-    response = client.access_secret_version(name)
+    response = client.access_secret_version({'name': name})
     return response.payload.data.decode('UTF-8')
 
 
-# ------------------------------------------------------------#
+#------------------------------------------------------------------------------
 # Storage
-# FIXME: Allow user to not have to pass bucket_name.
-# ------------------------------------------------------------#
+#------------------------------------------------------------------------------
 
-def create_short_url(api_key, long_url, project_name='cannlytics'):
+def create_short_url(api_key: str, long_url: str, project_name: str) -> str:
     """Create a short URL to a specified file.
     Args:
         api_key (str): An API key for Firebase dynamic links.
         long_url (str): A URL to create a short, dynamic link.
-        project_name (str): The name of the Firebase project, `cannlytics` by default.
+        project_name (str): The name of the Firebase project.
     Returns:
         (str): A short link to the given URL.
     """
     try:
         url = f'https://firebasedynamiclinks.googleapis.com/v1/shortLinks?key={api_key}'
         data= {
             'dynamicLinkInfo': {
@@ -697,50 +743,46 @@
         }
         response = requests.post(url, json=data)
         return response.json()['shortLink']
     except ConnectionError:
         raise ConnectionError # Optional: Handle connection errors more elegantly?
 
 
-def download_file(bucket_name, source_blob_name, destination_file_name, verbose=False):
+def download_file(
+        source_blob_name: str,
+        destination_file_name: str,
+        bucket_name: Optional[str] = None
+):
     """Downloads a file from Firebase Storage.
     Args:
-        bucket_name (str): The name of the storage bucket.
         source_blob_name (str): The file name to upload.
         destination_file_name (str): The destination file name.
-        verbose (bool): Whether or not to print status.
+        bucket_name (str): The name of the storage bucket (optional).
     """
     bucket = storage.bucket(name=bucket_name)
     blob = bucket.blob(source_blob_name)
     blob.download_to_filename(destination_file_name)
-    if verbose:
-        print(
-            'Blob {} downloaded to {}.'.format(source_blob_name, destination_file_name)
-        )
 
 
-def download_files(bucket_name, bucket_folder, local_folder, verbose=False):
+def download_files(bucket_folder: str, local_folder: str, bucket_name: Optional[str] = None):
     """Download all files in a given Firebase Storage folder.
     Args:
-        bucket_name (str): The name of the storage bucket.
         bucket_folder (str): A folder in the storage bucket.
         local_folder (str): The local folder to download files.
-        verbose (bool): Whether or not to print status.
+        bucket_name (str): The name of the storage bucket (optional).
     """
     bucket = storage.bucket(name=bucket_name)
     file_list = list_files(bucket_name, bucket_folder)
     for file in file_list:
         blob = bucket.blob(file)
         file_name = blob.name.split('/')[-1]
         blob.download_to_filename(local_folder + '/' + file_name)
-        if verbose:
-            print(f'{file_name} downloaded from bucket.')
 
 
-def get_file_url(ref, bucket_name=None, expiration=None):
+def get_file_url(ref: str, bucket_name: Optional[str] = None, expiration=None) -> str:
     """Return the storage URL of a given file reference.
     Args:
         ref (str): The storage location of the file.
         bucket_name (str): The name of the storage bucket.
         expiration (datetime): The date for when the file link should expire.
     Returns:
         (str): The storage URL of the file.
@@ -748,92 +790,104 @@
     if expiration is None:
         expiration = datetime.now() + timedelta(days=100 * 365)
     bucket = storage.bucket(name=bucket_name)
     blob = bucket.blob(ref)
     return blob.generate_signed_url(expiration)
 
 
-def upload_file(bucket_name, destination_blob_name, source_file_name=None, data_url=None, content_type='image/jpg'):
+def upload_file(
+        destination_blob_name: str,
+        source_file_name: Optional[str] = None,
+        data_url: Optional[str] = None,
+        content_type: Optional[str] = 'image/jpg',
+        bucket_name: Optional[str] = None,
+):
     """Upload file to Firebase Storage.
     Args:
-        bucket_name (str): The name of the storage bucket.
         destination_blob_name (str): The name to save the file as.
         source_file_name (str): The local file name.
         data_url (str): The data URL to upload from a string.
         content_type (str): The content type of the file, when uploading from a string.
+        bucket_name (str): The name of the storage bucket (optional).
     """
     bucket = storage.bucket(name=bucket_name)
     blob = bucket.blob(destination_blob_name)
     if source_file_name:
         blob.upload_from_filename(source_file_name)
     else:
         blob.upload_from_string(data_url, content_type=content_type)
 
-def upload_files(bucket_name, bucket_folder, local_folder, verbose=True):
+def upload_files(bucket_folder: str, local_folder: str, bucket_name: Optional[str] = None):
     """Upload multiple files to Firebase Storage.
     Args:
-        bucket_name (str): The name of the storage bucket.
         bucket_folder (str): A folder in the storage bucket to upload files.
         local_folder (str): The local folder of files to upload.
-        verbose (bool): Whether or not to print status.
+        bucket_name (str): The name of the storage bucket (optional).
     """
     bucket = storage.bucket(name=bucket_name)
     files = [f for f in listdir(local_folder) if isfile(join(local_folder, f))]
     for file in files:
         local_file = join(local_folder, file)
         blob = bucket.blob(bucket_folder + '/' + file)
         blob.upload_from_filename(local_file)
-    if verbose:
-        print(f'Uploaded {len(files)} to "{bucket_folder}" bucket.')
 
 
-def list_files(bucket_name, bucket_folder):
+def list_files(bucket_folder: str, bucket_name: Optional[str] = None) -> List[str]:
     """List all files in GCP bucket folder.
     Args:
-        bucket_name (str): The name of the storage bucket.
         bucket_folder (str): A folder in the storage bucket to list files.
+        bucket_name (str): The name of the storage bucket (optional).
     Returns:
         (list): A list of file names in the given bucket.
     """
     bucket = storage.bucket(name=bucket_name)
     files = bucket.list_blobs(prefix=bucket_folder)
     return [file.name for file in files if '.' in file.name]
 
 
-def delete_file(bucket_name, blob_name):
+def delete_file(blob_name: str, bucket_name: Optional[str] = None):
     """Delete file from GCP bucket.
     Args:
-        bucket_name (str): The name of the storage bucket.
         blob_name (str): The name of the file to delete.
+        bucket_name (str): The name of the storage bucket (optional).
     """
     bucket = storage.bucket(name=bucket_name)
     bucket.delete_blob(blob_name)
 
 
-def rename_file(bucket_name, bucket_folder, file_name, newfile_name, verbose=True):
+def rename_file(
+        bucket_folder: str,
+        file_name: str,
+        newfile_name: str,
+        bucket_name: Optional[str] = None,
+):
     """Rename file in GCP bucket.
     Args:
-        bucket_name (str): The name of the storage bucket.
         bucket_folder (str): A folder in the storage bucket.
         file_name (str): The name of the file to rename.
         newfile_name (str): The new name for the file.
-        verbose (bool): Whether or not to print status.
+        bucket_name (str): The name of the storage bucket (optional).
     """
     bucket = storage.bucket(name=bucket_name)
     blob = bucket.blob(bucket_folder + '/' + file_name)
     bucket.rename_blob(blob, new_name=newfile_name)
-    if verbose:
-        print(f'{file_name} renamed to {newfile_name}.')
 
 
-# ------------------------------------------------------------#
+#------------------------------------------------------------------------------
 # Misc
-# ------------------------------------------------------------#
+#------------------------------------------------------------------------------
 
-def create_log(ref, claims, action, log_type, key, changes=None):
+def create_log( #pylint: disable=too-many-arguments
+        ref: str,
+        claims: dict,
+        action: str,
+        log_type: str,
+        key: str,
+        changes: Any = None,
+):
     """Create an activity log.
     Args:
         ref (str): Path to a collection of logs.
         claims (dict): A dict with user fields or a Firestore user object.
         action (str): The activity that took place.
         log_type (str): The log type.
         key (str): A key to recognize the action.
```

### Comparing `cannlytics-0.0.8/cannlytics/lims/__init__.py` & `cannlytics-0.0.9/cannlytics/lims/__init__.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,20 +1,17 @@
-# -*- coding: utf-8 -*-
 """
-LIMS Module | Cannlytics
-Author: Keegan Skeate <keegan@cannlytics.com>
-Created: 2/6/2021
-Updated: 6/17/2021
-"""
-
-
-__version__ = '0.0.7'
-__author__ = 'Keegan Skeate'
+Cannlytics LIMS Initialization | Cannlytics
+Copyright (c) 2021-2022 Cannlytics and Cannlytics Contributors
 
+Authors: Keegan Skeate <keegan@cannlytics.com>
+Created: 11/6/2021
+Updated: 11/6/2021
+"""
 
+# TODO: Decide which packages to make readily available.
 # from .calculations import calculate_results
 # from .certificates import (
 #     create_coa,
 #     delete_coa,
 #     email_coas,
 #     text_coas,
 #     send_coas,
```

### Comparing `cannlytics-0.0.8/cannlytics/lims/calculations.py` & `cannlytics-0.0.9/cannlytics/lims/calculations.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 """
 Calculation Parser | Cannlytics
+Copyright (c) 2021-2022 Cannlytics
 
-Author: Keegan Skeate  
-Contact: <keegan@cannlytics.com>  
-Created: 6/8/2021  
-Updated: 6/8/2021  
-License: MIT License <https://opensource.org/licenses/MIT>
+Authors: Keegan Skeate <keegan@cannlytics.com>
+Created: 6/8/2021
+Updated: 6/8/2021
+License: <https://github.com/cannlytics/cannlytics-engine/blob/main/LICENSE>
 """
 # Standard imports
 import re
 
 # External imports
 try:
     import pandas as pd
@@ -19,20 +19,17 @@
 
 
 def calculate_results():
     """Calculate results by using analyte formula and
     instrument / analyst measurements.
     Calculate results by using analyte formula and
     instrument / analyst measurements.
-    Args:
-
-    Returns:
     """
-
-    print('Calculating results..')
+    # TODO: Implement a function that calculates results given a formula and results.
+    raise NotImplementedError
 
 
 # # Prepare testing dataset
 # tags = np.array(['tag'+str(i) for i in np.random.randint(10, size=200)])  # randomly generate tag list
 # vals = np.random.randint(20, size=200)  # generate a list of random integers
 
 # raw_df = pd.DataFrame({
```

### Comparing `cannlytics-0.0.8/cannlytics/lims/certificates.py` & `cannlytics-0.0.9/cannlytics/lims/certificates.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,44 +1,45 @@
 """
 Certificate of Analysis (CoA) Generation | Cannlytics
+Copyright (c) 2021-2022 Cannlytics
 
-Author: Keegan Skeate <keegan@cannlytics.com>  
-Created: 2/6/2021  
-Updated: 8/9/2021  
+Authors: Keegan Skeate <keegan@cannlytics.com>
+Created: 2/6/2021
+Updated: 1/10/2022
 License: MIT LIcense <https://opensource.org/licenses/MIT>
 
 TODO:
     - Allow users to create CoA's with a myriad of templates! (.docx, .xlsx, etc.)
-    - Import any docx template styed with jinga-style formatting and let'r'rip.
-    - Use your own templates or download the started templates and customize them to your heart's galore.
+    - Import any docx template styed with Jinga-style formatting and let'r'rip.
+    - Use your own templates or download the started templates and customize
+    them to your heart's galore.
 """
-# Standard imports
+# Standard imports.
 import os
-import environ
 from pathlib import Path
 from shutil import copyfile
 
-try:
+# External packages.
+from dotenv import dotenv_values
+import openpyxl
+# from openpyxl.drawing.image import Image
+import pandas as pd
+# import qrcode
+
+# Internal imports.
+from ..firebase import (
+    get_document,
+    # update_document,
+    download_file,
+)
+from ..utils.utils import snake_case
 
-    # External packages
-    import openpyxl
-    from openpyxl.drawing.image import Image
-    import pandas as pd
-    # import qrcode
-
-    # Internal imports
-    from cannlytics.firebase import (
-        get_document,
-        update_document,
-        download_file,
-    )
-    from cannlytics.utils.utils import snake_case
 
-except:
-    pass
+# TODO: This file needs a MAJOR refactor.
+
 
 def create_coa():
     """
     Creates a certificate of analysis.
     """
 
     # TODO: Get sample details.
@@ -168,19 +169,18 @@
     """
     Creates a certificate of analysis.
     """
     # TODO: Validate the user's pin to get their UID.
     uid = ''
 
     # Get the user's signature (if not already downloaded?).
-    env = environ.Env()
-    env.read_env(env_file)
-    bucket_name = env('FIREBASE_STORAGE_BUCKET')
+    env_variables = dotenv_values(env_file)
+    bucket_name = env_variables['FIREBASE_STORAGE_BUCKET']
     signature_data = get_document(f'users/{uid}/user_settings/signature')
-    download_file(bucket_name, signature_data['signature_ref'], signature_dest)
+    download_file(signature_data['signature_ref'], signature_dest, bucket_name)
 
     # Insert the signature into the CoA template.
 
     # Create the PDF.
 
     # Upload the PDF to storage.
 
@@ -357,15 +357,15 @@
 
     # Ensure Excel is visible.
     excel.ScreenUpdating = True
     excel.DisplayAlerts = True
     excel.EnableEvents = True
 
 
-# FIXME: Do it without Excel :(
+# FIXME: This requires that Excel is installed on Windows. Try to do this without Excel :(
 def create_coa_pdfs(render_file, ws_index_list, output_file, tight=False):
     """Generate PDFs for rendred CoAs.
     Args:
         render_file (str): The path of the rendred workbook.
         ws_index_list (list): A list of the worksheet indexes to include in the PDF.
         output_file (str): The name of the output PDF (expected .pdf extension).
         tight (bool): Optional, default False, choice to scale all pages.
@@ -554,8 +554,8 @@
 
     # Test CoA generation.
     generate_coas(
         files,
         output_pages=pages,
         # coa_template=args.template,
         limits=limits
-    )
+    )
```

### Comparing `cannlytics-0.0.8/cannlytics/lims/instruments.py` & `cannlytics-0.0.9/cannlytics/lims/instruments.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,105 +1,110 @@
 """
 Instruments | Cannlytics
+Copyright (c) 2021-2022 Cannlytics
 
-Author: Keegan Skeate <keegan@cannlytics.com>  
-Created: 8/3/2021  
-Updated: 8/21/2021  
-License: MIT License <https://opensource.org/licenses/MIT>  
+Authors: Keegan Skeate <keegan@cannlytics.com>
+Created: 8/3/2021
+Updated: 12/21/2021
+License: MIT License <https://opensource.org/licenses/MIT>
 
-Manage scientific instruments and measurements from the instruments.
+Description: Manage scientific instruments and measurements from the instruments.
 """
 # Standard imports
 import os
-import environ
 from datetime import datetime, timedelta
+from typing import Any, List, Optional
 
-try:
+# External imports
+from dotenv import dotenv_values
+import pandas as pd
+import requests
+
+# Internal imports
+from ..firebase import (
+    get_collection,
+    initialize_firebase,
+    update_document
+)
+from ..utils.utils import clean_column_names, snake_case
 
-    # External imports
-    import pandas as pd
-    import requests
-
-    # Internal imports
-    from cannlytics.firebase import (
-        get_collection,
-        initialize_firebase,
-        update_document
-    )
-    from cannlytics.utils.utils import snake_case
-
-except:
-    pass
 
 API_BASE = 'https://console.cannlytics.com'
 
 
-def automatic_collection(org_id=None, env_file='.env', minutes_ago=None):
+# TODO: Refactor, big time.
+def automatic_collection(
+        org_id: Optional[str] = None,
+        env_file: Optional[str] = '.env',
+        minutes_ago: Optional[int] = None,
+) -> List[dict]:
     """Automatically collect results from scientific instruments.
     Args:
         org_id (str): The organization ID to associate with instrument results.
         env_file (str): The environment variable file, `.env` by default.
             Either a `GOOGLE_APPLICATION_CREDENTIALS` or a
             `CANNLYTICS_API_KEY` is needed to run the routine.
         minutes_ago (int): The number of minutes in the past to restrict
             recently modified files.
     Returns:
         (list): A list of measurements (dict) that were collected.
     """
 
-    # Try to initialize Firebase, otherwise an API key will be used.
+    # Try to set credentials and initialize Firebase, otherwise an API key will be used.
     try:
-        env = environ.Env()
-        env.read_env(env_file)
-        credentials = env('GOOGLE_APPLICATION_CREDENTIALS')
-        os.environ['GOOGLE_APPLICATION_CREDENTIALS'] = credentials
-        initialize_firebase()
+        config = dotenv_values(env_file)
+        credentials = config.get('GOOGLE_APPLICATION_CREDENTIALS')
+        initialize_firebase(credentials)
     except:
         pass
 
     # Get the organization ID from the .env file if not specified.
     if not org_id:
-        org_id = env('CANNLYTICS_ORGANIZATION_ID')
+        org_id = config['CANNLYTICS_ORGANIZATION_ID']
 
     # Format the last modified time cut-off as a datetime.
     last_modified_at = None
     if minutes_ago:
         last_modified_at = datetime.now() - timedelta(minutes=minutes_ago)
 
     # Get the instruments, trying Firestore, then the API.
     try:
         ref = f'organizations/{org_id}/instruments'
         instrument_data = get_collection(ref)
     except:
-        api_key = env('CANNLYTICS_API_KEY')
+        api_key = config['CANNLYTICS_API_KEY']
         headers = {
             'Authorization': 'Bearer %s' % api_key,
             'Content-type': 'application/json',
         }
         url = f'{API_BASE}/instruments?organization_id={org_id}'
         response = requests.get(url, headers=headers)
         instrument_data = response.json()['data']
 
+    # TODO: Split this functionality into separate functions.
     # Iterate over instruments, collecting measurements.
     measurements = []
     for instrument in instrument_data:
 
         # Iterate over analyses that the instrument may be running.
-        analyses = instrument.get('analyses', '').split(',')
+        try:
+            analyses = instrument.get('analyses', '').split(',')
+        except AttributeError:
+            continue # FIXME: Handle missing analyses more elegantly.
         analyses = [x.strip() for x in analyses]
-        for n in range(len(analyses)):
+        for index, analysis in enumerate(analyses):
 
             # Optional: Handle multiple data paths more elegantly.
-            analysis = analyses[n]
+            analysis = analyses[index]
             try:
                 data_paths = instrument['data_path'].split(',')
             except AttributeError:
                 continue # No data path.
             data_paths = [x.strip() for x in data_paths]
-            data_path = data_paths[n]
+            data_path = data_paths[index]
             if not data_path:
                 continue
 
             # Identify the analysis being run and identify the import routine.
             # Optional: Identify more elegantly.
             if 'micro' in analysis or 'MICR' in analysis:
                 import_method = globals()['import_micro']
@@ -111,15 +116,15 @@
             # Search for recently modified files in the instrument directory
             # and parse any recently modified file.
             for root, _, filenames in os.walk(data_path):
                 for filename in filenames:
                     if filename.endswith('.xlsx') or filename.endswith('.xls'):
                         data_file = os.path.join(root, filename)
                         modifed_at = os.stat(data_file).st_mtime
-                        # FIXME: Ensure date restriction works.
+                        # TODO: Ensure that date restriction works.
                         if last_modified_at:
                             if modifed_at < last_modified_at:
                                 continue
                         samples = import_method(data_file)
                         if isinstance(samples, dict):
                             sample_data = {**instrument, **samples}
                             measurements.append(sample_data)
@@ -136,15 +141,14 @@
             measurement['sample_id'] = measurement['sample_name']
         except:
             continue # Already has `sample_id`.
 
         # TODO: Format a better measurement ID.
         measurement_id = measurement.get('acq_inj_time') # E.g. 12-Jun-21, 15:21:07
         if not measurement_id:
-            # measurement_id = now.strftime('%d-%b-%y-%H-%M-%S') + '_' + str(measurement['sample_id'])
             measurement_id = measurement['sample_id']
         else:
             try:
                 measurement_id = measurement_id.replace(',', '').replace(' ', '-').replace(':', '-')
             except AttributeError:
                 pass
             measurement_id = str(measurement_id) + '_' + str(measurement['sample_id'])
@@ -174,40 +178,15 @@
                 response = requests.post(url, json=result, headers=headers)
             print('Uploaded result:', ref)
 
     # Return the measurements
     return measurements
 
 
-def clean_column_names(df, column):
-    """
-    Args:
-        df (DataFrame): A DataFrame with any column names.
-        column (str): The column of the DataFrame to clean.
-    Returns:
-        (DataFrame): A DataFrame with snake_case column names.
-    """
-    df[column] = df[column].str.strip()
-    df[column] = df[column].str.rstrip('.)]')
-    df[column] = df[column].str.replace('%', 'percent', regex=True)
-    df[column] = df[column].str.replace('#', 'number', regex=True)
-    df[column] = df[column].str.replace('[/,]', '_', regex=True)
-    df[column] = df[column].str.replace('[.,(,)]', '', regex=True)
-    df[column] = df[column].str.replace("\'", '', regex=True)
-    df[column] = df[column].str.replace("[[]", '_', regex=True)
-    df[column] = df[column].str.replace(r"[]]", '', regex=True)
-    df[column] = df[column].str.replace('β', 'beta', regex=True)
-    df[column] = df[column].str.replace('Δ', 'delta', regex=True)
-    df[column] = df[column].str.replace('δ', 'delta', regex=True)
-    df[column] = df[column].str.replace('α', 'alpha', regex=True)
-    df[column] = df[column].str.replace('__', '', regex=True)
-    return df
-
-
-def get_compound_dataframe(workbook_data, sheetname='Compound'):
+def get_compound_dataframe(workbook_data: dict, sheetname: Optional[str] = 'Compound') -> Any:
     """ Rename the columns in the `Compound` sheet to match the required
     names. For simplicity, make a copy of the `Compound` sheet to
     handle NaN values.
     Args:
         workbook_data (dict): A dictionary of worksheet DataFrames.
         sheetname (str): The worksheet that contains the compound data.
     Returns:
@@ -222,36 +201,55 @@
     compounds = workbook_data[sheetname].copy()
     criterion = (compounds.analyte.isnull()) & (compounds.measurement > 0)
     compounds.loc[criterion, 'analyte'] = 'wildcard'
     compounds.dropna(subset=['analyte'], inplace=True)
     return compounds
 
 
-def get_sample_data(workbook_data, sheet_name='Sheet1'):
+def get_sample_data(workbook_data: dict, sheet_name: Optional[str] = 'Sheet1') -> dict:
     """Return the sample name from a dictionary.
     Converts the first column of the first sheet to snake_case.
     Args:
-        df (DataFrame): A DataFrame.
+        data (DataFrame): A DataFrame.
         sheet_name (str): The name of the worksheet containing the sample data.
     Returns:
         (dict): The sample data as a key and value pairs.
     """
     data = workbook_data[sheet_name]
     data['ObjClass'] = data['ObjClass'].apply(snake_case)
     return dict(data.values)
 
 
-def import_heavy_metals(file_name):
+def import_analyses(directory: str):
+    """Import analyses to Firestore from a .csv or .xlsx file.
+    Args:
+        directory (str): The full filename of a data file.
+    """
+    analyses = pd.read_excel(directory + 'analyses.xlsx')
+    analytes = pd.read_excel(directory + 'analytes.xlsx')
+    for index, analysis in analyses.iterrows():
+        analyte_data = []
+        analyte_names = analysis.analyte_keys.split(', ')
+        for analyte_key in analyte_names:
+            analyte_item = analytes.loc[analytes.key == analyte_key]
+            analyte_data.append(analyte_item.to_dict(orient='records'))
+        analyses.at[index, 'analytes'] = analyte_data 
+    analyses_data = analyses.to_dict(orient='records')
+    # TODO: Implement.
+    raise NotImplementedError
+
+
+def import_heavy_metals(file_name: str) -> List[dict]:
     """Import heavy metal results from ICP-MS screening.
     First, reads in the log sheet and summary sheets seperately to
     make parsing easier. Drops the rows that do not contain sample ids.
     Renames columns to make parsing clearer. Get list of samples and
     then parses measurements.
     Args:
-        df (DataFrame): A DataFrame.
+        data (DataFrame): A DataFrame.
     Returns:
         (list): A list of measurements (dict).
     """
     results_data = pd.read_excel(file_name, sheet_name='Log')
     samples_data = pd.read_excel(file_name, sheet_name='Quant Summary')
     results_data.dropna(subset = ['Sample Mass (g)'], inplace=True)
     samples_data.rename(columns = {'Analysis':'analyte', '-': 'mass'}, inplace=True)
@@ -261,32 +259,32 @@
         sample = {}
         result_data = results_data[results_data['Sample ID'] == sample_id]
         sample['sample_id'] = sample_id
         sample['sample_mass'] = result_data['Sample Mass (g)'].values[0]
         sample['sample_dilution'] = result_data['Sample Dilution'].values[0]
         analytes = []
         criterion = (samples_data['analyte'] == 'ID:') & (samples_data['mass'] == sample_id)
-        index  = samples_data.index[criterion].tolist()
+        index = samples_data.index[criterion].tolist()
         for offset in range(index[0] + 20, index[0] + 27): # Magic numbers
             analyte = {}
             analyte['analyte'] = samples_data.iloc[offset].analyte
             analyte['measurement'] = samples_data.iloc[offset + 9].mass # Magic number
             analytes.append(analyte)
         sample['results'] = analytes
         samples.append(sample)
     return samples
 
 
-def import_micro(file_name):
+def import_micro(file_name: str) -> List[dict]:
     """Import microbiological screening results, grouping sample results
     by well name.
     Args:
         file_name (str): The path to a qPCR data file.
     Returns:
-        (list): A list of sample measurements (dictionary).
+        (list): A list of sample measurements (dict).
     """
     workbook_data = pd.read_excel(file_name, sheet_name=None)
     results = workbook_data['Tabular Results']
     sample_names = results['Well Name'].unique()
     columns = {
         'Dye': 'method',
         'Target': 'analyte',
@@ -301,49 +299,48 @@
         sample_data = results.loc[results['well_name'] == sample_name]
         fields = list(columns.values())
         sample['results'] = sample_data[fields].to_dict('records')
         samples.append(sample)
     return samples
 
 
-def import_results(file_name):
+def import_results(file_name: str) -> dict:
     """Import scientific instrument data. The routine is as follows:
         1. Read in all the excel sheets at one time.
         2. Get the sample name.
         3. Get and tidy the compound data from the compound sheet.
         4. Add the analyte names and measurements to a list of result dictionaries.
         5. Collect the data into a running list.
     Args:
-        df (DataFrame): A DataFrame.
+        data (DataFrame): A DataFrame.
     Returns:
         (dict): A dictionary of sample results.
     """
     workbook_data = pd.read_excel(file_name, sheet_name=None)
     sample = get_sample_data(workbook_data)
     compounds = get_compound_dataframe(workbook_data)
     compounds = clean_column_names(compounds, 'analyte')
     columns = ['analyte', 'measurement', 'amount_per_response']
     sample['results'] = compounds[columns].to_dict('records')
     return sample
 
 
 if __name__ == '__main__':
 
+    # Standard imports.
     import argparse
-    import os, sys
-    # sys.path.append(os.path.join(os.path.dirname(__file__)))
-    sys.path.append('../cannlytics')
+    import os
 
-    # Internal imports
-    from cannlytics.firebase import (
+    # Internal imports.
+    from ..firebase import (
         get_collection,
         initialize_firebase,
         update_document
     )
-    from cannlytics.utils.utils import snake_case
+    from ..utils.utils import snake_case
 
     # Declare command line arguments.
     parser = argparse.ArgumentParser(description='Scientific instrument data collection routine.')
     parser.add_argument('--env', action='store', dest='env_file', default='.env')
     parser.add_argument('--modified', action='store', dest='last_modified', default=None)
     parser.add_argument('--org', action='store', dest='org_id', default='')
     args = parser.parse_args()
```

### Comparing `cannlytics-0.0.8/cannlytics/lims/qc.py` & `cannlytics-0.0.9/cannlytics/lims/qc.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 """
 Quality Control Tools | Cannlytics
 
-Author: Keegan Skeate <keegan@cannlytics.com>  
+Authors: Keegan Skeate <keegan@cannlytics.com>  
 Created: 2/6/2021  
 Updated: 6/23/2021  
 License: MIT License <https://opensource.org/licenses/MIT>  
 
 Perform various quality control checks and analyses to ensure
 that your laboratory is operating as desired.
```

### Comparing `cannlytics-0.0.8/cannlytics/lims/results.py` & `cannlytics-0.0.9/cannlytics/lims/results.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,33 +1,26 @@
 """
 Result Calculation | Cannlytics
 
-Author: Keegan Skeate <keegan@cannlytics.com>  
+Authors: Keegan Skeate <keegan@cannlytics.com>  
 Created: 6/23/2021  
 Updated: 7/19/2021  
 License: MIT License <https://opensource.org/licenses/MIT>  
 
 Use analyte limits and formulas and instrument measurements to calculate
 final results for analyses.
 """
-try:
-
-    # Standard imports
-    from datetime import datetime
-
-    # External imports
-    from smtplib import SMTP
-    from email.mime.multipart import MIMEMultipart
-
-    # Internal imports
-    from cannlytics.firebase import get_collection, update_documents
-    from cannlytics.traceability.metrc.utils import encode_pdf
-
-except:
-    pass # FIXME: Docs can't import.
+# Standard imports.
+from datetime import datetime
+from email.mime.multipart import MIMEMultipart
+from smtplib import SMTP
+
+# Internal imports.
+from ..firebase import get_collection, update_documents
+from ..metrc.utils import encode_pdf
 
 
 def calculate_results(sample_data, analysis, mass, dilution_factor=10, correction_factor=10000):
     """Calculate percentage results given raw results,
     dilution factor, and analysis type.
     Args:
         sample_data (dict): A dictionary of sample data.
@@ -46,14 +39,20 @@
             raw_value = float(sample_data[analyte])
             sample_data[analyte] = ((raw_value * dilution_factor) / mass) / correction_factor
         except ValueError:
             continue
     return sample_data
 
 
+# TODO: Implement.
+def convert_results_units():
+    """Convert results between units."""
+    raise NotImplementedError
+
+
 def post_results():
     """
     Post results to your state traceability system.
     """
     # # Initialize Firebase.
     # config = dotenv_values('../../../.env')
     # os.environ['GOOGLE_APPLICATION_CREDENTIALS'] = config['GOOGLE_APPLICATION_CREDENTIALS']
```

### Comparing `cannlytics-0.0.8/cannlytics/lims/stats.py` & `cannlytics-0.0.9/cannlytics/lims/stats.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 """
 Statistics | Cannlytics
 
-Author: Keegan Skeate <keegan@cannlytics.com>  
+Authors: Keegan Skeate <keegan@cannlytics.com>  
 Created: 6/23/2021  
 Updated: 6/23/2021  
 License: MIT License <https://opensource.org/licenses/MIT>  
 
 Calculate statistics on your laboratory performance.
 """
```

### Comparing `cannlytics-0.0.8/cannlytics/lims/transfers.py` & `cannlytics-0.0.9/cannlytics/lims/transfers.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,31 +1,32 @@
 """
 Transfer Management | Cannlytics
 
-Author: Keegan Skeate <keegan@cannlytics.com>  
+Authors: Keegan Skeate <keegan@cannlytics.com>  
 Created: 6/23/2021  
 Updated: 6/23/2021  
 License: MIT License <https://opensource.org/licenses/MIT>  
 
 Tools to help manage transfers of laboratory samples.
 """
+# TODO: Does this belong in crm?
 
 def create_transfer():
     """Create a transfer of samples to a lab for analysis. The sending
     organization specifies the sample details and the analyses requested.
     The receiving organization, the lab, can create projects from the
     sample details and analyses requested. The lab can edit sample details
     stored in a project, but only the sender can edit sample details in
     the transfer. By default, the sending organization will receive
     results when they are released."""
 
     return NotImplementedError
 
 
-def receive_transfer(transfer_id):
+def receive_transfer(transfer_id: str):
     """
     Receive a transfer of laboratory samples.
     """
     packages = track.get_packages(license_number=cultivator.license_number)
     return NotImplementedError
```

### Comparing `cannlytics-0.0.8/cannlytics/lims/worksheets.py` & `cannlytics-0.0.9/cannlytics/lims/worksheets.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,37 +1,59 @@
 """
 Worksheets | Cannlytics
+Copyright (c) 2021-2022 Cannlytics
 
-Author: Keegan Skeate <keegan@cannlytics.com>
+Authors: Keegan Skeate <keegan@cannlytics.com>
 Created: 7/18/2021
-Updated: 7/20/2021
+Updated: 1/10/2022
 License: MIT License <https://opensource.org/licenses/MIT>
 """
-
+# Standard packages
+from ast import literal_eval
+from typing import Any, List, Optional, Tuple, Union
+
+# External packages.
+from dotenv import dotenv_values
+from pandas import DataFrame, to_datetime
+import requests
 try:
-
-    # Standard packages
-    from ast import literal_eval
-    import os
-
-    # External packages.
-    from dotenv import load_dotenv
-    from pandas import DataFrame, to_datetime
-    import requests
     import xlwings
     from xlwings.utils import rgb_to_int
+except ImportError:
+    # FIXME: Work on alternatives as xlwings doesn't work in App Engine.
+    pass
+
+# Internal packages.
+from ..utils.utils import snake_case
 
-    # Internal packages.
-    from cannlytics.utils.utils import snake_case
 
-except:
-    pass # FIXME: Docs can't import.
+def format_values(data: Union[list, dict], columns: List[str]) -> List[dict]:
+    """Format response data by given columns. Handles a list or dictionary of data.
+    Args:
+        data (list,dict): A list of values or a dictionary of values.
+        columns (list): A list of column names used to get values from the data.
+    Returns:
+        (list): Returns a list of items.
+    """
+    items = []
+    try:
+        for item in data:
+            values = []
+            for column in columns:
+                values.append(item.get(column))
+            items.append(values)
+    except AttributeError:
+        values = []
+        for column in columns:
+            values.append(data.get(column))
+        items = [values]
+    return items
 
 
-def get_data_block(sheet, coords, expand=None):
+def get_data_block(sheet: Any, coords: str, expand: Optional[str] = None) -> dict:
     """Get a data block.
     Args:
         sheet (Sheet): The worksheet containing the data block.
         coords (str): The inclusive coordinates of the data block.
         expand (str): Optionally expand the range of values.
     Returns
         (dict): A dictionary of the data in the data block.
@@ -41,31 +63,62 @@
     for item in values:
         key = snake_case(item[0])
         value = item[1]
         data[key] = value
     return data
 
 
-def increment_row(coords):
+def get_data_model(worksheet: Any, config: dict, model_type: str, ids: List[str]) -> Any:
+    """Get a specific data model from the Cannlytics API.
+    Args:
+        worksheet (Worksheet): An xlwings Excel worksheet instance.
+        config (dict): A dictionary of user configuration.
+        model_type (str): The data model name.
+        ids (list): Specific IDs to retrieve from the API.
+    Returns:
+        (HTTPResponse): An HTTP response from the Cannlytics API.
+    """
+    base = config['api_url']
+    org_id = worksheet.range(config['org_id_cell']).value
+    env_variables = dotenv_values(config['env_path'])
+    api_key = env_variables['CANNLYTICS_API_KEY']
+    headers = {
+        'Authorization': 'Bearer %s' % api_key,
+        'Content-type': 'application/json',
+    }
+    if len(ids) == 1:
+        url = f'{base}/{model_type}/{ids[0]}?organization_id={org_id}'
+    else:
+        url = f'{base}/{model_type}?organization_id={org_id}&items={str(ids)}'
+    response = requests.get(url, headers=headers)
+    return response
+
+
+def increment_row(coords: str) -> str:
     """Increment a row given its starting coordinates.
     Args:
         coords (str):
     Returns:
         (str): The incremented row coordinates.
     """
     column = ''.join([i for i in coords if not i.isdigit()])
     seq_type = type(coords)
     row = int(seq_type().join(filter(seq_type.isdigit, coords))) + 1
     return column + str(row)
 
 
-def import_worksheet(filename, sheetname, range_start='A1'):
+def import_worksheet(
+        filename: str,
+        sheetname: str,
+        range_start: Optional[str] = 'A1',
+) -> List[dict]:
     """Read the data from a given worksheet using xlwings.
     Args:
-        filename (str): The name of the Excel file to read.
+        filename (str): The name of the Excel workbook to read.
+        sheetname (str): The name of the worksheet to import.
         range_start (str): Optional starting cell.
     Returns:
         list(dict): A list of dictionaries.
     """
     app = xlwings.App(visible=False)
     book = xlwings.Book(filename)
     sheet = book.sheets(sheetname)
@@ -74,148 +127,142 @@
     data = [dict(zip(keys, values)) for values in excel_data[1:]]
     book.close()
     app.quit()
     return data
 
 
 @xlwings.sub
-def import_worksheet_data(model_type):
-    """A function called from Excel to import data by ID
+def import_worksheet_data(model_type: str):
+    """A function called from Excel to import data by IDs in the worksheet
     from Firestore into the Excel workbook.
     Args:
         model_type (str): The data model at hand.
     """
 
     # Initialize the workbook.
-    book = xlwings.Book.caller()
-    worksheet = book.sheets.active
-    config_sheet = book.sheets['cannlytics.conf']
-    config = get_data_block(config_sheet, 'A1', expand='table')
+    worksheet, config = initialize_workbook()
+    status_cell = config['status_cell']
     show_status_message(
         worksheet,
-        coords=config['status_cell'],
+        coords=status_cell,
         message='Importing %s data...' % model_type,
         background=config['success_color'],
     )
 
     # Read the IDs.
     id_cell = increment_row(config['table_cell'])
     ids = worksheet.range(id_cell).options(expand='down', ndim=1).value
 
-    # Get your Cannlytics API key from your .env file, location specified
-    # by env_path on the cannlytics.config sheet.
-    load_dotenv(config['env_path'])
-    api_key = os.getenv('CANNLYTICS_API_KEY')
-
     # Get the worksheet columns.
     columns = worksheet.range(config['table_cell']).options(expand='right', ndim=1).value
     columns = [snake_case(x) for x in columns]
 
     # Get data using model type and ID through the API.
-    base = config['api_url']
-    org_id = worksheet.range(config['org_id_cell']).value
-    headers = {
-        'Authorization': 'Bearer %s' % api_key,
-        'Content-type': 'application/json',
-    }
-    if len(ids) == 1:
-        url = f'{base}/{model_type}/{ids[0]}?organization_id={org_id}'
-    else:
-        url = f'{base}/{model_type}?organization_id={org_id}&items={str(ids)}'
-    response = requests.get(url, headers=headers)
+    response = get_data_model(worksheet, config, model_type, ids)
     if response.status_code != 200:
         show_status_message(
             worksheet,
-            coords=config['status_cell'],
+            coords=status_cell,
             message='Error importing data.',
             background=config['error_color']
         )
         return
 
     # Format the values.
-    items = []
-    data = response.json()['data']
-    if not data:
+    try:
+        data = response.json()['data']
+        items = format_values(data, columns)
+    except TypeError:
         show_status_message(
             worksheet,
-            coords=config['status_cell'],
+            coords=status_cell,
             message='No data found.',
             background=config['error_color']
         )
         return
-    try:
-        for item in data:
-            values = []
-            for column in columns:
-                values.append(item.get(column))
-            items.append(values)
-    except AttributeError:
-        values = []
-        for column in columns:
-            values.append(data.get(column))
-        items = [values]
 
     # Insert all rows at the same time.
     worksheet.range(id_cell).value = items
 
     # Show success status message.
     show_status_message(
         worksheet,
-        coords=config['status_cell'],
+        coords=status_cell,
         message='Imported %i %s.' % (len(ids), model_type),
     )
 
 
-@xlwings.sub
-def upload_worksheet_data(model_type):
-    """A function called from Excel to import data by ID
-    from Firestore into the Excel workbook."""
-
-    # Initialize the workbook.
+def initialize_workbook() -> Tuple:
+    """Initialize an xlwings workbook and return the config worksheet data.
+    Returns:
+        (Worksheet): Returns the active worksheet.
+        (dict): Returns a dictionary of user configuration.
+    """
     book = xlwings.Book.caller()
     worksheet = book.sheets.active
     config_sheet = book.sheets['cannlytics.conf']
     config = get_data_block(config_sheet, 'A1', expand='table')
-    show_status_message(
-        worksheet,
-        coords=config['status_cell'],
-        message='Uploading %s data...' % model_type,
-        background=config['success_color'],
-    )
+    return worksheet, config
 
-    # Read the table data, cleaning the column names.
-    table = worksheet.range(config['table_cell'])
+
+def read_table_data(worksheet: Any, cell: str) -> dict:
+    """Read table data from a worksheet and clean the columns and data.
+    Args:
+        worksheet (Worksheet): A worksheet containing the table data.
+        cell (str): The cell range of the table.
+    Returns:
+        (dict): Returns the data in the worksheet table as a dictionary.
+    """
+    table = worksheet.range(cell)
     data = table.options(DataFrame, index=False, expand='table').value
     data.columns = list(map(snake_case, data.columns))
-
-    # Clean columns. (Optional: Clean more efficiently.)
     for column in data.columns:
         if column.endswith('_at'):
             try:
                 data[column] = to_datetime(data[column]).dt.strftime('%Y-%m-%dT%H:%M%:%SZ')
             except:
                 pass
-    data = data.fillna('')
+    return data.fillna('')
+
+
+@xlwings.sub
+def upload_worksheet_data(model_type):
+    """A function called from Excel to import data by IDs in the worksheet
+    from Firestore into the Excel workbook."""
+
+    # Initialize the workbook.
+    worksheet, config = initialize_workbook()
+    status_cell = config['status_cell']
+    show_status_message(
+        worksheet,
+        coords=status_cell,
+        message='Uploading %s data...' % model_type,
+        background=config['success_color'],
+    )
+
+    # Read the table data, cleaning the column names.
+    data = read_table_data(worksheet, config['table_cell'])
 
     # Determine the model type and the organization.
     org_id = worksheet.range(config['org_id_cell']).value
     model_singular = data.columns[0].replace('_id', '')
     if not org_id:
         show_status_message(
             worksheet,
-            coords=config['status_cell'],
+            coords=status_cell,
             message='Organization ID required.',
             background=config['error_color']
         )
         return
 
     # Get Cannlytics API key from .env using env_path in config.
-    load_dotenv(config['env_path'])
-    api_key = os.getenv('CANNLYTICS_API_KEY')
+    env_variables = dotenv_values(config['env_path'])
+    api_key = env_variables['CANNLYTICS_API_KEY']
 
+    # TODO: Split this into a separate function.
     # Upload data using model type, ID, and data through the API.
     headers = {
         'Authorization': 'Bearer %s' % api_key,
         'Content-type': 'application/json',
     }
     base = config['api_url']
     for _, row in data.iterrows():
@@ -225,30 +272,30 @@
         if not doc_id:
             continue
         url = f'{base}/{model_type}?organization_id={org_id}'
         response = requests.post(url, json=json, headers=headers)
         if response.status_code == 200:
             show_status_message(
                 worksheet,
-                coords=config['status_cell'],
+                coords=status_cell,
                 message='Uploaded %s' % doc_id,
             )
         else:
             show_status_message(
                 worksheet,
-                coords=config['status_cell'],
+                coords=status_cell,
                 message='Error uploading %s. Check your organization, internet connection and API key.' % doc_id, # pylint:disable=line-too-long
                 background=config['error_color']
             )
             return
 
     # Show success status message.
     show_status_message(
         worksheet,
-        coords=config['status_cell'],
+        coords=status_cell,
         message='Uploaded %i %s.' % (len(data), model_type),
     )
 
 
 def show_status_message(sheet, coords, message, background=None, color=None):
     """Show a status message in an Excel spreadsheet.
     Args:
```

### Comparing `cannlytics-0.0.8/cannlytics/traceability/metrc/exceptions.py` & `cannlytics-0.0.9/cannlytics/metrc/exceptions.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,37 +1,45 @@
-# -*- coding: utf-8 -*-
 """
 Metrc Exceptions | Cannlytics
+Copyright (c) 2021-2022 Cannlytics and Cannlytics Contributors
+
+Authors: Keegan Skeate <keegan@cannlytics.com>
+Created: 11/5/2021
+Updated: 11/8/2021
+License: <https://github.com/cannlytics/cannlytics-engine/blob/main/LICENSE>
 
 Exceptions used when interfacing with the Metrc API.
 """
 
 
-class TraceabilityException(Exception):
-    """A base class for traceability system exceptions."""
-
-
-class MetrcAPIError(TraceabilityException):
-    """A primary error raised by the API.
+class MetrcAPIError(Exception):
+    """A primary error raised by the Metrc API.
     Insufficient permissions for a request typically
     result in a 401 unauthorized error.
     """
 
     def __init__(self, response):
-        super(MetrcAPIError, self).__init__(self._extract_text(response))
+        message = self.get_response_messages(response)
+        super().__init__(message)
         self.response = response
 
-    def _extract_text(self, response):
-        return self._text_from_detail(response) or response.text
-
-    def _text_from_detail(self, response):
+    def get_response_messages(self, response):
+        """Extract error messages from a Metrc API response.
+        Args:
+            response (Response): A request response from the Metrc API.
+        Returns:
+            (str): Returns any error messages.
+        """
         try:
             errors = response.json()
             if isinstance(errors, list):
-                message = '\n'.join(errors)
-                return f'\n---------------\n{message}\n---------------'
+                try:
+                    message = '\n'.join(errors)
+                except TypeError:
+                    message = '\n'.join([x.get('message') for x in errors])
+            elif isinstance(errors, dict):
+                message = errors.get('Message', errors.get('message'))
             else:
-                message = errors['Message']
-                return f'\n---------------\n{message}\n---------------'
+                message = response.text
         except (AttributeError, KeyError, ValueError):
-            message = 'Unknown API error'
-            return f'\n---------------\n{message}\n---------------'
+            message = 'Unknown Metrc API error'
+        return message
```

### Comparing `cannlytics-0.0.8/cannlytics/traceability/metrc/models.py` & `cannlytics-0.0.9/cannlytics/metrc/models.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,30 +1,30 @@
-# -*- coding: utf-8 -*-
 """
 Metrc Models | Cannlytics
+Copyright (c) 2021-2022 Cannlytics and Cannlytics Contributors
+
+Authors: Keegan Skeate <keegan@cannlytics.com>
+Created: 11/5/2021
+Updated: 11/12/2021
+License: <https://github.com/cannlytics/cannlytics-engine/blob/main/LICENSE>
 
 This module contains common Metrc models.
 """
 
-# External imports
-from datetime import datetime
-
-# Internal imports
-from cannlytics.firebase import get_document, update_document
-
-# Local imports
-from .utils import (
+# Internal imports.
+from ..firebase import get_document, update_document
+from ..utils.utils import (
+    camel_to_snake,
     clean_dictionary,
     clean_nested_dictionary,
-    camel_to_snake,
-    snake_to_camel,
-    update_context,
+    get_timestamp,
     remove_dict_fields,
     remove_dict_nulls,
-    get_timestamp,
+    snake_to_camel,
+    update_dict,
 )
 
 
 class Model(object):
     """Base class for all Metrc models."""
 
     def __init__(
@@ -43,34 +43,46 @@
 
     def __getattr__(self, key):
         return self.__dict__[key]
 
     def __setattr__(self, key, value):
         self.__dict__[key] = value
 
+    @property
+    def uid(self):
+        """The model's unique ID."""
+        return self.__dict__.get('id')
+
+    @classmethod
+    def from_dict(cls, client, json):
+        """Initiate a class instance from a dictionary."""
+        obj = cls(client, json)
+        try:
+            obj.create()
+        except KeyError:
+            pass
+        return obj
+
     @classmethod
     def from_fb(cls, client, ref):
         """Initialize a class from Firebase data.
         Args:
             client (Client): A Metrc client instance.
             ref (str): The reference to the document in Firestore.
+        Returns:
+            (Model): A Metrc model.
         """
         data = get_document(ref)
         obj = cls(client, data)
         return obj
 
-    @property
-    def uid(self):
-        """The model's unique ID."""
-        return self.__dict__.get('id')
-
     def to_dict(self):
         """Returns the model's properties as a dictionary."""
         data = vars(self).copy()
-        [data.pop(x, None) for x in ['_license', 'client']]
+        [data.pop(x, None) for x in ['_license', 'client', '__class__']]
         return data
 
     def to_fb(self, ref='', col=''):
         """Upload the model's properties as a dictionary to Firestore.
         Args:
             ref (str): The Firestore document reference.
             col (str): A Firestore collection, with the UID as document ID.
@@ -78,15 +90,112 @@
         data = vars(self).copy()
         [data.pop(x, None) for x in ['_license', 'client']]
         if col:
             update_document(f'{col}/{self.uid}', data)
         else:
             update_document(ref, data)
 
-    # TODO: Add create_from_json to all models.
+
+class Delivery(Model):
+    """A class that represents a cannabis home delivery. Sales are reported to
+    record the transfer of cannabis products to a consumer, patient or
+    caregiver.
+
+    When you request receipts you receive the following object.
+    ```js
+    {
+        "Id": 1,
+        "ReceiptNumber": null,
+        "SalesDateTime": "2016-01-01T17:35:45.000",
+        "SalesCustomerType": "Consumer",
+        "PatientLicenseNumber": null,
+        "CaregiverLicenseNumber": null,
+        "IdentificationMethod": null,
+        "TotalPackages": 0,
+        "TotalPrice": 0.0,
+        "Transactions": [],
+        "IsFinal": false,
+        "ArchivedDate": null,
+        "RecordedDateTime": "0001-01-01T00:00:00+00:00",
+        "RecordedByUserName": null,
+        "LastModified": "0001-01-01T00:00:00+00:00"
+    }
+    ```
+
+    When you create a receipt, you pass the following object.
+    ```js
+    {
+        "SalesDateTime": "2016-10-04T16:44:53.000",
+        "SalesCustomerType": "Consumer",
+        "PatientLicenseNumber": null,
+        "CaregiverLicenseNumber": null,
+        "IdentificationMethod": null,
+        "Transactions": [
+            {
+                "PackageLabel": "ABCDEF012345670000010331",
+                "Quantity": 1.0,
+                "UnitOfMeasure": "Ounces",
+                "TotalAmount": 9.99
+            }
+        ]
+    }
+    ```
+    """
+
+    def create(self):
+        """Create a receipt record in Metrc."""
+        context = self.to_dict()
+        data = clean_nested_dictionary(context, snake_to_camel)
+        self.client.create_receipts([data], license_number=self._license)
+
+    def update(self, **kwargs):
+        """Update the receipt given parameters as keyword arguments."""
+        context = self.to_dict().copy()
+        data = update_dict(context, **kwargs)
+        data = remove_dict_nulls(data)
+        self.client.update_receipts([data], self._license)
+
+    def delete(self):
+        """Delete the receipt."""
+        self.client.delete_receipt(self.id, self._license)
+
+
+class Category(Model):
+    """A class representing an item category.
+    ```js
+        {
+            "Name": "Buds",
+            "ProductCategoryType": "Buds",
+            "QuantityType": "WeightBased",
+            "RequiresStrain": true,
+            "RequiresItemBrand": false,
+            "RequiresAdministrationMethod": false,
+            "RequiresUnitCbdPercent": false,
+            "RequiresUnitCbdContent": false,
+            "RequiresUnitCbdContentDose": false,
+            "RequiresUnitThcPercent": false,
+            "RequiresUnitThcContent": false,
+            "RequiresUnitThcContentDose": false,
+            "RequiresUnitVolume": false,
+            "RequiresUnitWeight": false,
+            "RequiresServingSize": false,
+            "RequiresSupplyDurationDays": false,
+            "RequiresNumberOfDoses": false,
+            "RequiresPublicIngredients": false,
+            "RequiresDescription": false,
+            "RequiresProductPhotos": 0,
+            "RequiresLabelPhotos": 0,
+            "RequiresPackagingPhotos": 0,
+            "CanContainSeeds": true,
+            "CanBeRemediated": true,
+            "CanBeDestroyed": false
+        }
+    ```
+    """
+    pass
 
 
 class Employee(Model):
     """An organization's employee or team member.
     ```js
         {
             "FullName": "Keegan Skeate",
@@ -94,17 +203,17 @@
         }
     ```
     """
     pass
 
 
 class Facility(Model):
-    """A Facility represents a building licensed for the growing,
-    processing, and/or selling of product. Facilities are created
-    and have their permissions determined by a state.
+    """A Facility represents a building licensed for the growing, processing,
+    and/or selling of product. Facilities are created and have their
+    permissions determined by a state.
     ```js
     {
         "HireDate": "0001-01-01",
         "IsOwner": false,
         "IsManager": true,
         "Occupations": [],
         "Name": "Cultivation LLC",
@@ -130,176 +239,98 @@
         """The facilities license number."""
         return self.license['number']
 
     def get_locations(self, uid='', action=''):
         """Get locations at the facility.
         Args:
             uid (str): The UID of a location, takes precedent over action.
-            action (str): A specific filter to apply, with options: `active`, `types`.
+            action (str): A specific filter to apply: `active` or `types`.
         """
-        response = self.client.get_locations(uid=uid, action=action, license_number=self.license_number)
+        response = self.client.get_locations(
+            uid=uid,
+            action=action,
+            license_number=self.license_number
+        )
         return response
 
-    def create_locations(self, names, types):
+    def create_location(self, name, location_type='default'):
         """Create locations at the facility.
         Args:
-            names (list): A list of location names.
-            types (list): A list of location types:
+            name (str): A location name.
+            location_type (str): An optional location type:
                 `default`, `planting`, or `packing`.
+                `default` is assigned by default.
         """
-        data = []
-        for i in range(len(names)):
-            try:
-                location_type = types[i]
-            except IndexError:
-                location_type = 'Default Location Type'
-            data.append({
-                'Name': names[i],
-                'LocationTypeName': location_type
-            })
-        response = self.client.create_locations(
-            data,
-            license_number=self.license_number
+        return self.client.create_locations(
+            [name],
+            [location_type],
+            self.license_number
         )
-        return response
+        # TODO: Implement return_obs
+
+    def create_locations(self, names, types=[]):
+        """Create locations at the facility.
+        Args:
+            names (list): A list of location names.
+            types (list): An optional list of location types:
+                `default`, `planting`, or `packing`.
+                `default` is assigned by default.
+        """
+        return self.client.create_locations(names, types, self.license_number)
+        # TODO: Implement return_obs
 
     def update_locations(self, ids, names, types=[]):
         """Update locations at the facility.
         Args:
             ids (list): A list of location IDs.
             names (list): A list of location names.
             types (list): A list of location types:
                 `default`, `planting`, or `packing`.
         """
         data = []
-        for i in range(len(ids)):
+        for index, location_id in enumerate(ids):
             try:
-                location_type = types[i]
+                location_type = types[index]
             except IndexError:
                 location_type = 'Default Location Type'
             data.append({
-                'Id': ids[i],
-                'Name': names[i],
+                'Id': location_id,
+                'Name': names[index],
                 'LocationTypeName': location_type
             })
         response = self.client.update_locations(
             data,
             license_number=self.license_number
         )
         return response
+        # TODO: Implement return_obs
 
     def delete_location(self, uid):
         """Delete a location at the facility.
         Args:
             uid (str): The UID of a location to delete.
         """
         response = self.client.delete_location(
             uid,
             license_number=self.license_number
         )
         return response
 
-    # TODO:
-    # Get / Create / Update / Delete strains from facility
-    # Get / Create / Update / Delete items from facility
-
-    # TODO: Create transfers from the facility
-
-
-class Location(Model):
-    """A class that represents a cannabis-production location.
-    ```js
-        {
-            "Id": 1,
-            "Name": "Harvest Location",
-            "LocationTypeId": 1,
-            "LocationTypeName": "Default",
-            "ForPlantBatches": True,
-            "ForPlants": True,
-            "ForHarvests": True,
-            "ForPackages": True
-        }
-    ```
-    """
-
-    def __init__(self, client, properties, license_number=''):
-        super().__init__(client, properties, license_number)
-        self._parameters = {
-            'name': 'Name',
-            'location_type': 'LocationTypeName',
-            'batches': 'ForPlantBatches',
-            'plants': 'ForPlants',
-            'harvests': 'ForHarvests',
-            'packages': 'ForPackages'
-        }
-
-    def update(self, **kwargs):
-        """Update location."""
-        data = self.to_dict()
-        update = clean_dictionary(data, snake_to_camel)
-        for param in kwargs:
-            key = self._parameters.get(param, param)
-            update[key] = kwargs[param]
-        self.client.update_locations([update])
-
-    def delete(self):
-        """Delete location."""
-        self.client.delete_location(self.id)
-
-
-class Strain(Model):
-    """A class that represents a cannabis strain.
-    ```js
-        {
-            "Id": 1,
-            "Name": "Old-time Moonshine",
-            "TestingStatus": "InHouse",
-            "ThcLevel": 0.1865,
-            "CbdLevel": 0.1075,
-            "IndicaPercentage": 25.0,
-            "SativaPercentage": 75.0
-        }
-    ```
-    """
-
-    @classmethod
-    def create_from_json(cls, client, json):
-        """Initiate a class instance from a dictionary."""
-        obj = cls(client, json)
-        obj.create()
-        return obj
-
-    def create(self):
-        """Create a strain record in Metrc."""
-        context = self.to_dict()
-        data = clean_dictionary(context, snake_to_camel)
-        self.client.create_strains([data])
-
-    def update(self, **kwargs):
-        """Update the strain given parameters as keyword arguments."""
-        context = self.to_dict()
-        data = update_context(context, **kwargs)
-        self.client.update_strains([data], license_number=self._license)
-
-    def delete(self):
-        """Delete the strain."""
-        self.client.delete_strain(self.id, license_number=self._license)
-
 
 class Item(Model):
     """Items are used to track a licensee's inventory at a given facility.
-    Items belong to a single facility
-    Each item has a unique item name, category, and strain.
-    Item Names are used for identification, so an item name
-    should not simply be a category name. Item names are
-    specific to the item in that package or production batch.
-    Categories are pre-defined. The item name
-    identifies what is in the package and categories
-    are used for grouping similar items for reporting purposes.    
-    An item will retain its name unless it is re-packaged.
+    Metrc documentation states:
+
+    Items belong to a single facility. Each item has a unique item name,
+    category, and strain. Item Names are used for identification, so an item
+    name should not simply be a category name. Item names are specific to the
+    item in that package or production batch. Categories are pre-defined. The
+    item name identifies what is in the package and categories are used for
+    grouping similar items for reporting purposes. An item will retain its name
+    unless it is re-packaged.
     ```js
         {
             "Id": 1,
             "Name": "Buds",
             "ProductCategoryName": "Buds",
             "ProductCategoryType": "Buds",
             "QuantityType": "WeightBased",
@@ -354,357 +385,399 @@
         super().__init__(client, properties, license_number)
         for k, v in self.RETURNED_VALUES.items():
             try:
                 self.__dict__[v] = properties[k]
             except KeyError:
                 pass
 
-    @classmethod
-    def create_from_json(cls, client, license_number, json):
-        """Initiate a class instance from a dictionary."""
-        new_obj = cls(client, json, license_number)
-        new_obj.create(license_number)
-        return new_obj
-
-    def create(self, license_number):
+    def create(self, license_number='', return_obs=False):
         """Create an item record in Metrc."""
         context = self.to_dict()
         data = clean_dictionary(context, snake_to_camel)
-        self.client.create_items([data], license_number)
+        self.client.create_items([data], license_number, return_obs=return_obs)
 
     def update(self, **kwargs):
         """Update the item given parameters as keyword arguments."""
         context = self.to_dict().copy()
-        data = update_context(context, **kwargs)
+        data = update_dict(context, **kwargs)
         data = remove_dict_fields(data, self.RETURNED_VALUES.keys())
         data = remove_dict_nulls(data)
         self.client.update_items([data], self._license)
 
     def delete(self):
         """Delete the item."""
         self.client.delete_item(self.id, self._license)
 
 
-class Plant(Model):
-    """A class that represents a cannabis plant.
-    
-    Plants are tagged at the immature lot growth phase and at the mature / flowering growth
-    phase.
-    A UID number is assigned to an immature plant lot of
-    up to 100 seeds or immature plants. Required corresponding UID
-    number labels will need to be produced by the licensee
-    . Once the immature lot has been
-    established in Metrc, the death of an immature plant(s) must be recorded in Metrc by
-    recording the associated waste amount and reducing the total number of the immature
-    plants in the lot for each immature plant that was destroyed.
-
-    Plant tags are assigned to individual plants when they are moved to a designated
-    canopy area, or when the plant begins flowering.
-
-    A plant can be destroyed anytime during the growth phases.
-    Any waste produced by the plant should be recorded prior to the destruction.
-    2. Any waste created during the immature growth phase must be recorded as waste
-    using the Plant Waste function and destroyed.
-    3. When immature plants begin to flower, select the Change Growth Phase button
-    to record the change and associate the new Plant Tag ID to the plant(s).
-    4. In Metrc, anytime something is trimmed from a flowering plant during growing
-    with the intent to sell it, process it, or perform a partial harvest, a Manicure batch
-    must be created.
+class Location(Model):
+    """A class that represents a cannabis-production location.
+    ```js
+        {
+            "Id": 1,
+            "Name": "Harvest Location",
+            "LocationTypeId": 1,
+            "LocationTypeName": "Default",
+            "ForPlantBatches": True,
+            "ForPlants": True,
+            "ForHarvests": True,
+            "ForPackages": True
+        }
+    ```
     """
 
-    # TODO: `create/plantings`,
-    # TODO: `create/plantbatch/packages`,
-
-    def flower(self, tag, location_name=None):
-        """Change the growth phase of the plant to flowering.
-        Args:
-            tag (str): A tag to assign to the flowering plant.
-            location_name (str): An optional new location for the plant.
-        """
-        if location_name is None:
-            location_name = self.location_name
-        data = {
-            'Label': self.label,
-            'NewTag': tag,
-            'GrowthPhase': 'Flowering',
-            'NewLocation': location_name,
-            'GrowthDate': get_timestamp()
+    def __init__(self, client, properties, license_number=''):
+        super().__init__(client, properties, license_number)
+        self._parameters = {
+            'name': 'Name',
+            'location_type': 'LocationTypeName',
+            'batches': 'ForPlantBatches',
+            'plants': 'ForPlants',
+            'harvests': 'ForHarvests',
+            'packages': 'ForPackages'
         }
-        self.client.manage_plants(
-            [data],
-            action='changegrowthphases',
-            license_number=self._license
-        )
 
-    def move(self, location_name):
-        """Move the plant to a new location.
-        Args:
-            location_name (str): The destination's name.
-        """
-        data = {
-            'Id': self.id,
-            'Location': location_name,
-            'ActualDate': get_timestamp()
-        }
-        self.client.manage_plants(
-            [data],
-            action='moveplants',
-            license_number=self._license
-        )
+    def update(self, **kwargs):
+        """Update location."""
+        data = self.to_dict()
+        update = clean_dictionary(data, snake_to_camel)
+        for param in kwargs:
+            key = self._parameters.get(param, param)
+            update[key] = kwargs[param]
+        self.client.update_locations([update])
 
-    def destroy(
-        self,
-        weight,
-        method='Compost',
-        material='Soil',
-        note='n/a',
-        reason='Contamination',
-        uom='grams',
-        ):
-        """Destroy the plant.
-        Args:
-            weight (float): Required weight of the waste.
-            material (str): The waste material, e.g soil.
-            method (str): The mechanism of destruction:
-                `Grinder` or `Compost`.
-            reason (str): The reason for destruction:
-                `Contamination` or `Male Plants`.
-        """
-        data = {
-            'Id': self.id,
-            'WasteMethodName': method,
-            'WasteMaterialMixed': material,
-            'WasteWeight': weight,
-            'WasteUnitOfMeasureName': uom,
-            'WasteReasonName': reason,
-            'ReasonNote': note,
-            'ActualDate': get_timestamp()
-        }
-        self.client.manage_plants(
-            [data],
-            action='destroyplants',
-            license_number=self._license
-        )
+    def delete(self):
+        """Delete location."""
+        self.client.delete_location(self.id)
 
-    def manicure(
-        self,
-        weight,
-        harvest_name=None,
-        location_name=None,
-        patient_license=None,
-        uom='Grams',
-    ):
-        """Manicure the plant.
-        Args:
-            weight (float): Required harvest weight.
-            harvest_name (str): Optional harvest name.
-            location_name (str): The drying location's name.
-            patient_license (str): A patient's license number.
-            uom (str): The unit of measure
-        """
-        if location_name is None:
-            location_name = self.location_name
-        data = {
-            'Plant': self.label,
-            'Weight': weight,
-            'UnitOfWeight': uom,
-            'DryingLocation': location_name,
-            'HarvestName': harvest_name,
-            'PatientLicenseNumber': patient_license,
-            'ActualDate': get_timestamp()
-        }
-        self.client.manage_plants(
-            [data],
-            action='manicureplants',
-            license_number=self._license
-        )
 
-    def harvest(
-        self,
-        harvest_name,
-        weight,
-        location_name=None,
-        patient_license=None,
-        uom='Grams',
-    ):
-        """Harvest the plant.
-        Args:
-            harvest_name (str): Required harvest name.
-            weight (float): Required harvest weight.
-            location_name (str): The harvest location's name.
-            patient_license (str): A patient's license number.
-            uom (str): The unit of measure.
-        """
-        if location_name is None:
-            location_name = self.location_name
-        data = {
-            'Plant': self.label,
-            'Weight': weight,
-            'UnitOfWeight': uom,
-            'DryingLocation': location_name,
-            'HarvestName': harvest_name,
-            'PatientLicenseNumber': patient_license,
-            'ActualDate': get_timestamp()
-        }
-        self.client.manage_plants(
-            [data],
-            action='harvestplants',
-            license_number=self._license
-        )
+class Harvest(Model):
+    """A class that represents a cannabis harvest. Metrc documentation states:
 
+    A harvest batch is created and given a unique Harvest Name when plants
+    or plant material are harvested. [The following 7 conditions must be met.]
 
-class Harvest(Model):
-    """A class that represents a cannabis harvest.
-    
-    A harvest batch is created and given a
-    unique Harvest Name when plants
-    or plant material are harvested.
-
-    A. Harvest Name – Harvests must be strain specific. The Harvest Name must be
-    unique. It is a best practice for the harvest name to include the Strain Name
-    and Harvest Date, but it is not required by the State.
+    1. Harvest Name – Harvests must be strain specific. The Harvest Name must
+    be unique. It is a best practice for the harvest name to include the Strain
+    Name and Harvest Date, but it is not required by the State.
 
-    B. Weight – The plant is weighed individually in its entirety after being cut from
-    root ball (stem, stalk, bud/flower, leaves, trim leaves, etc.).
+    2. Weight – The plant is weighed individually in its entirety after being
+    cut from root ball (stem, stalk, bud/flower, leaves, trim leaves, etc.).
 
-    C. Waste – This can be recorded using multiple entries but must be reported
+    3. Waste – This can be recorded using multiple entries but must be reported
     within three days of destruction.
 
-    D. Package – Package and tag the product from the Harvest Batch (Fresh
+    4. Package – Package and tag the product from the Harvest Batch (Fresh
     Cannabis Plant, Flower, Leaf or Kief). These packages must be strain
     specific.
 
-    E. Transfer – Licensee must create transfer manifest to move product to a
+    5. Transfer – Licensee must create transfer manifest to move product to a
     Processor, Distributor, or Manufacturer.
 
-    F. Finish – When the Harvest Batch (HB) has been fully packaged, there should
-    be remaining wet weight to account for moisture loss. Selecting Finish
-    Harvest will attribute any remaining weight to moisture loss.
-
-    6. A Harvest Batch package of Flower, Leaf, Kief or Fresh Cannabis Plant can only
-    be created from the Harvested Tab using a single strain from plants harvested at
-    the same time.
+    6. Finish – When the Harvest Batch (HB) has been fully packaged, there
+    should be remaining wet weight to account for moisture loss. Selecting
+    Finish Harvest will attribute any remaining weight to moisture loss.
+
+    7. A Harvest Batch package of Flower, Leaf, Kief or Fresh Cannabis Plant
+    can only be created from the Harvested Tab using a single strain from
+    plants harvested at the same time.
     """
 
-    def create_packages(self, data):
+    def create_package(
+            self,
+            name,
+            tag,
+            weight,
+            location=None,
+            note='',
+            uom=None
+    ):
+        """Create a package from a harvest.
+        Args:
+            name (str): The name of the packaged item.
+            tag (str): A tag for the package.
+            weight (float): The weight of the package.
+            location (str): An optional location for the package, the location
+                of the harvest is used by default.
+            note (str): A note for the package.
+            uom (str): The unit of measure, the unit of measure from the
+                harvest is used by default.
+        """
+        data = {
+            'Tag': tag,
+            'Location': location or self.drying_location_name,
+            'Item': name,
+            'UnitOfWeight': uom or self.unit_of_weight_name,
+            'Note': note,
+            'ActualDate': get_timestamp(zone=self.client.state),
+            'Ingredients': [
+                {
+                    'HarvestId': self.id,
+                    'Weight': weight,
+                    'UnitOfWeight': uom or self.unit_of_weight_name,
+                },
+            ]
+        }
+        self.client.create_harvest_packages(
+            [data],
+            license_number=self._license,
+        )
+        # TODO: Implement return_obs
+
+    def create_packages(
+            self,
+            name,
+            tag,
+            weights,
+            location=None,
+            note='',
+            uom=None
+    ):
         """Create packages from a harvest.
         Args:
-            data (list): The package data.
+            name (str): The name of the packaged item.
+            tag (str): A tag for the package.
+            weights (list): A list of package weights (float).
+            location (str): An optional location for the package, the location
+                of the harvest is used by default.
+            note (str): A note for the package.
+            uom (str): The unit of measure, the unit of measure from the
+                harvest is used by default.
         """
+        if uom is None:
+            uom = self.unit_of_weight_name
+        data = {
+            'Tag': tag,
+            'Location': location or self.drying_location_name,
+            'Item': name,
+            'UnitOfWeight': uom,
+            'Note': note,
+            'ActualDate': get_timestamp(zone=self.client.state),
+            'Ingredients': []
+        }
+        for weight in weights:
+            data['Ingredients'].append({
+                'HarvestId': self.id,
+                'Weight': weight,
+                'UnitOfWeight': uom,
+            })
         self.client.create_harvest_packages(data, license_number=self._license)
+        # TODO: Implement return_obs
 
-    # FIXME: create testing package
     def create_testing_packages(self, data):
         """Create testing packages from a harvest.
         Args:
             data (list): The package data.
         """
-        self.client.create_harvest_packages(data, license_number=self._license)
+        self.client.create_harvest_testing_packages(data, license_number=self._license)
+        # TODO: Implement return_obs
 
     def remove_waste(self, weight, waste_type='Waste', uom='Grams'):
         """Remove waste from the harvest.
         Args:
             weight (float): Required harvest weight.
             waste_type (str): The type of waste.
             uom (str): The unit of measure.
         """
         data = {
             'Id': self.uid,
             'WasteType': waste_type,
             'UnitOfWeight': uom,
             'WasteWeight': weight,
-            'ActualDate': get_timestamp()
+            'ActualDate': get_timestamp(zone=self.client.state)
         }
         self.client.remove_waste([data], license_number=self._license)
 
     def finish(self):
         """Finish a harvest."""
-        data = {'Id': self.uid, 'ActualDate': get_timestamp()}
+        data = {
+            'Id': self.uid,
+            'ActualDate': get_timestamp(zone=self.client.state),
+        }
         self.client.finish_harvests([data], license_number=self._license)
 
     def unfinish(self):
-        """Unfinish a harvest."""
-        self.client.unfinish_harvests([{'Id': self.uid}], license_number=self._license)
+        """Un-finish a harvest."""
+        self.client.unfinish_harvests(
+            [{'Id': self.uid}],
+            license_number=self._license,
+        )
 
     def move(self, destination, harvest_name=None):
         """Move a harvest.
         Args:
             destination (str): THe name of the destination location.
             harvest_name (str): An optional harvest name.
         """
         data = {
             "Id": self.uid,
             "HarvestName": harvest_name,
             "DryingLocation": destination,
-            "ActualDate": get_timestamp()
+            "ActualDate": get_timestamp(zone=self.client.state)
         }
         self.client.move_harvest([data], license_number=self._license)
 
 
 class Package(Model):
-    """A class that represents a cannabis package.
+    """A class that represents a cannabis package. Metrc documentation states:
 
-    Immature plants and seeds can be packaged by a nursery and
-    transported by a distributor to a cultivator,
-    distributor or retailer for sale.
-
-    2. When a manufacturer is creating a concentrate that will then be used in multiple
-    infused production batches, the concentrate must be created as a new package.
-    The infused production batches will then be created from the concentrate
-    package.
+    Immature plants and seeds can be packaged by a nursery and transported by a
+    distributor to a cultivator, distributor or retailer for sale.
+
+    2. When a manufacturer is creating a concentrate that will then be used i
+    multiple infused production batches, the concentrate must be created as a
+    new package. The infused production batches will then be created from the
+    concentrate package.
 
     A. The new package of concentrate is a production batch and will then be
     partially used in an infused product or sold to a customer.
 
     B. This makes it more easily recorded as connected to the finished infused
     product package.
 
-    3. Packages made at a manufacturer facility that creates concentrates must be
-    created by pulling from other packages.
+    3. Packages made at a manufacturer facility that creates concentrates must
+    be created by pulling from other packages.
 
     4. A package must exist in order for it to be selected for transfer.
     Transfers are realtime inventory dependent.
 
-    5. There must be a contents section for each new package created from an existing
-    package.
+    5. There must be a contents section for each new package created from an
+    existing package.
 
     6. When adjusting a package, use the appropriate adjustment reason.
 
-    7. In order for a distributor to send a sample for testing,
-    a test sample package must be created. A new test sample must
-    have a new RFID package tag and be pulled
-    from an existing package.
+    7. In order for a distributor to send a sample for testing, a test sample
+    package must be created. A new test sample must have a new RFID package tag
+    and be pulled from an existing package.
 
     8. Package tags may only be used once and may not be reused.
     """
 
-    # @classmethod
-    # def create_from_json(cls, client, license_number, json):
-    #     new_obj = cls(client, json, license_number)
-    #     new_obj.create_package(new_obj.to_dict(), license_number)
-    #     return new_obj
-
-    def create_package(self, data):
-        """Create a package record in Metrc."""
-        data = clean_nested_dictionary(data, snake_to_camel)
-        self.client.create_packages([data], self._license)
+    def create_package(
+            self,
+            name,
+            tag='',
+            label='',
+            labels=[],
+            weight=0,
+            weights=[],
+            location=None,
+            note='',
+            patient_license=None,
+            uom=None,
+            uoms=[],
+            production_batch=False,
+            donation=False,
+            remediation=False,
+            same_item=False,
+
+    ):
+        """Create a package from a harvest.
+        Args:
+            name (str): The name of the packaged item.
+            tag (str): A tag for the package.
+            label (str): A package label for the item.
+            labels (list): A list of package labels (str) that supersede the
+                label.
+            weight (float): A weight for the package.
+            weights (list): A list of weights (float) for the packages that
+                supersede the weight.
+            location (str): An optional location for the package, the location
+                of the harvest is used by default.
+            patient_license (str): A patient license number.
+            note (str): A note for the package.
+            uom (str): The unit of measure for the package and items.
+            uoms (list): A list of unit of measures for the items.
+            production_batch (bool): Whether the package is for production.
+            donation (bool): Whether the package is for donation.
+            remediation (bool): Whether the package is for remediation.
+            same_item (bool): Whether the package has the same items as its
+                parent.
+        """
+        if weights:
+            total_weight = sum(weights)
+        else:
+            total_weight = weight
+        data = {
+            'Tag': tag,
+            'Location': location or self.location_name,
+            'Item': name,
+            'Quantity': total_weight,
+            'UnitOfMeasure': uom or self.unit_of_measure_name,
+            'PatientLicenseNumber': patient_license,
+            'Note': note,
+            'IsProductionBatch': bool(production_batch),
+            'ProductionBatchNumber': production_batch,
+            'IsDonation': donation,
+            'ProductRequiresRemediation': remediation,
+            'UseSameItem': same_item,
+            'ActualDate': get_timestamp(zone=self.client.state),
+            'Ingredients': []
+        }
+
+        if labels:
+            for index, item_label in enumerate(labels):
+                try:
+                    item_uom = uoms[index]
+                except IndexError:
+                    item_uom = uom or self.unit_of_measure_name
+                try:
+                    item_weight = weights[index]
+                except IndexError:
+                    item_weight = weight
+                data['Ingredients'].append({
+                    'Package': item_label,
+                    'Quantity': item_weight,
+                    'UnitOfMeasure': item_uom,
+                })
+        else:
+            data['Ingredients'].append({
+                'Package': label,
+                'Quantity': weight,
+                'UnitOfMeasure': uom or self.unit_of_measure_name,
+            })
+        self.client.create_packages(
+            [data],
+            license_number=self._license,
+        )
+        # TODO: Implement return_obs
+
+    # TODO: Implement (with return_obs)
+    def create_packages(
+            self,
+    ):
+        """Create multiple packages from a harvest."""
+        raise NotImplementedError
 
     def change_item(self, item_name):
         """Change the item of the package."""
-        data = {'Label': self.label, 'Item': item_name}
+        data = {
+            'Label': self.label,
+            'Item': item_name,
+        }
         self.client.change_package_items([data], self._license)
 
     def finish(self):
         """Finish a package."""
-        data = {'Label': self.label, 'ActualDate': get_timestamp()}
-        self.client.manage_packages([data], action='finish', license_number=self._license)
+        data = {
+            'Label': self.label,
+            'ActualDate': get_timestamp(zone=self.client.state)
+        }
+        self.client.manage_packages(
+            [data],
+            action='finish',
+            license_number=self._license
+        )
 
     def unfinish(self):
-        """Unfinish a package."""
-        self.client.manage_packages([{'Label': self.label}], action='unfinish', license_number=self._license)
+        """Un-finish a package."""
+        self.client.manage_packages(
+            [{'Label': self.label}],
+            action='unfinish',
+            license_number=self._license
+        )
 
     def adjust(
             self,
             weight,
             note='',
             reason='Mandatory State Destruction',
             uom='Grams'
@@ -717,22 +790,94 @@
             uom (str): The unit of measure.
         """
         data = {
             'Label': self.label,
             'Quantity': weight,
             'UnitOfMeasure': uom,
             'AdjustmentReason': reason,
-            'AdjustmentDate': get_timestamp(),
+            'AdjustmentDate': get_timestamp(zone=self.client.state),
             'ReasonNote': note
         }
-        self.client.manage_packages([data], action='adjust', license_number=self._license)
+        self.client.manage_packages(
+            [data],
+            action='adjust',
+            license_number=self._license,
+        )
 
+    def remediate(self, method, steps):
+        """Remediate the package.
+        Args:
+            method (str): The method used for remediation.
+            steps (str): A description of the steps followed to remediate
+                the package.
+        """
+        data = [{
+            'PackageLabel': self.label,
+            'RemediationMethodName': method,
+            'RemediationDate': get_timestamp(zone=self.client.state),
+            'RemediationSteps': steps,
+        }]
+        self.client.manage_packages(
+            data,
+            action='remediate',
+            license_number=self._license,
+        )
+
+    def update_note(self, note):
+        """Update the package's note.
+        Args:
+            note (str): The new package note.
+        """
+        data = [{
+            'PackageLabel': self.label,
+            'Note': note,
+        }]
+        self.client.update_package_notes(data)
+
+
+    def change_location(self, location):
+        """Change the package's location.
+        Args:
+            location (str): The new location for the package.
+        """
+        data = [{
+            'Label': self.label,
+            'Location': location,
+            'MoveDate': get_timestamp(zone=self.client.state)
+        }]
+        self.client.update_package_item_locations(data)
+
+
+    def update_items(self, name='', names=[]):
+        """Update the package's item.
+        Args:
+            name (str): The name of the package item.
+            names (list): A list of item names to update.
+        """
+        data = []
+        if not names:
+            data.append({
+                'PackageLabel': self.label,
+                'Item': name,
+            })
+        else:
+            # Warning: untested
+            for index, item_name in enumerate(names):
+                item_name = names[index]
+                item_label = self.ingredients[index]['PackageLabel']
+                data.append({
+                    'PackageLabel': item_label,
+                    'Item': item_name,
+                })
+        self.client.change_package_items(data)
+
+    def delete(self):
+        """Delete the package."""
+        self.client.delete_package(self.id)
 
-    # TODO:  remediate, update_note, change_location
-    # update_items, update, delete
 
 
 class Patient(Model):
     """A class that represents a cannabis patient.
     ```js
     {
         'PatientId': 1,
@@ -744,40 +889,274 @@
         'RecommendedSmokableQuantity': 2.0,
         'HasSalesLimitExemption': false,
         'OtherFacilitiesCount': 1
     }
     ```
     """
 
-    @classmethod
-    def create_from_json(cls, client, json):
-        """Initiate a class instance from a dictionary."""
-        obj = cls(client, json)
-        obj.create()
-        return obj
-
     def create(self):
         """Create a patient record in Metrc."""
         context = self.to_dict()
-        context['actual_date'] = get_timestamp()
+        context['actual_date'] = get_timestamp(zone=self.client.state)
         data = clean_nested_dictionary(context, snake_to_camel)
         self.client.create_patients([data], license_number=self._license)
 
     def update(self, **kwargs):
         """Update the patient given parameters as keyword arguments."""
         context = self.to_dict().copy()
-        data = update_context(context, **kwargs)
+        data = update_dict(context, **kwargs)
         data = remove_dict_nulls(data)
         self.client.update_patients([data], self._license)
 
     def delete(self):
         """Delete the patient."""
         self.client.delete_patient(self.id, self._license)
 
 
+class Plant(Model):
+    """A class that represents a cannabis plant. Metrc documentation states:
+
+    Plants are tagged at the immature lot growth phase and at the mature /
+    flowering growth phase. A UID number is assigned to an immature plant lot
+    of up to 100 seeds or immature plants. Required corresponding UID
+    number labels will need to be produced by the licensee.
+    
+    Once the immature lot has been established in Metrc, the death of an
+    immature plant(s) must be recorded in Metrc by
+    recording the associated waste amount and reducing the total number of the
+    immature plants in the lot for each immature plant that was destroyed.
+
+    Plant tags are assigned to individual plants when they are moved to a
+    designated canopy area, or when the plant begins flowering.
+
+    A plant can be destroyed anytime during the growth phases.
+    Any waste produced by the plant should be recorded prior to the
+    destruction.
+    2. Any waste created during the immature growth phase must be recorded as
+    waste using the Plant Waste function and destroyed.
+    3. When immature plants begin to flower, select the Change Growth Phase
+    button to record the change and associate the new Plant Tag ID to the
+    plant(s).
+    4. In Metrc, anytime something is trimmed from a flowering plant during
+    growing with the intent to sell it, process it, or perform a partial
+    harvest, a Manicure batch must be created.
+    """
+
+    def create_planting(self, name, count, location=None, batch_type='Clone'):
+        """Create an immature plant batch from the plant.
+        Args:
+            name (str): The name of the new plant batch.
+            count (int): The number of clones being planted.
+            location (str): An optional new location for the plant batch.
+            batch_type (str): The type of planting, Seed of Clone, with Clone
+                as the default.
+        """
+        data = {
+            'PlantLabel': self.label,
+            'PlantBatchName': name,
+            'PlantBatchType': batch_type,
+            'PlantCount': count,
+            'LocationName': location or self.location_name,
+            'StrainName': self.strain_name,
+            'PatientLicenseNumber': None,
+            'ActualDate': get_timestamp(zone=self.client.state),
+        }
+        self.client.manage_plants(
+            [data],
+            action='create/plantings',
+            license_number=self._license
+        )
+        # TODO: Implement return_obs
+
+    def create_plant_package(
+            self,
+            name,
+            tag,
+            count=1,
+            batch_type='Clone',
+            trade_sample=False,
+            donation=False,
+            location=None,
+            note='',
+            patient_license=None,
+    ):
+        """Create a package of immature plants from the plant.
+        Args:
+            name (str): The name of the item to create.
+            tag (str): The tag for the package.
+            count (int): The number of immature plants to package, 1 by
+                default.
+            batch_type (str): The batch type, Seed or Clone,
+                with Clone as the default.
+            trade_sample (bool): Whether or not the package is for sale.
+            donation (bool): Whether or not the package is for donation.
+            location (str): An optional new location for the package.
+            note (str): An optional note for the package.
+            patient_license (str): An optional patient license.
+        """
+        data = {
+            'PlantLabel': self.label,
+            'PackageTag': tag,
+            'PlantBatchType': batch_type,
+            'Item': name,
+            'Location': location or self.location_name,
+            'Note': note,
+            'IsTradeSample': trade_sample,
+            'PatientLicenseNumber': patient_license,
+            'IsDonation': donation,
+            'Count': count,
+            'ActualDate': get_timestamp(zone=self.client.state)
+        }
+        self.client.manage_plants(
+            [data],
+            action='create/plantbatch/packages',
+            license_number=self._license
+        )
+        # TODO: Implement return_obs
+
+    def flower(self, tag, location_name=None):
+        """Change the growth phase of the plant to flowering.
+        Args:
+            tag (str): A tag to assign to the flowering plant.
+            location_name (str): An optional new location for the plant.
+        """
+        if location_name is None:
+            location_name = self.location_name
+        data = {
+            'Label': self.label,
+            'NewTag': tag,
+            'GrowthPhase': 'Flowering',
+            'NewLocation': location_name,
+            'GrowthDate': get_timestamp(zone=self.client.state)
+        }
+        self.client.manage_plants(
+            [data],
+            action='changegrowthphases',
+            license_number=self._license
+        )
+
+    def move(self, location_name):
+        """Move the plant to a new location.
+        Args:
+            location_name (str): The destination's name.
+        """
+        data = {
+            'Id': self.id,
+            'Location': location_name,
+            'ActualDate': get_timestamp(zone=self.client.state)
+        }
+        self.client.manage_plants(
+            [data],
+            action='moveplants',
+            license_number=self._license
+        )
+
+    def destroy(
+            self,
+            weight,
+            method='Compost',
+            material='Soil',
+            note='n/a',
+            reason='Contamination',
+            uom='grams',
+    ):
+        """Destroy the plant.
+        Args:
+            weight (float): Required weight of the waste.
+            material (str): The waste material, e.g soil.
+            method (str): The mechanism of destruction:
+                `Grinder` or `Compost`.
+            reason (str): The reason for destruction:
+                `Contamination` or `Male Plants`.
+        """
+        data = {
+            'Id': self.id,
+            'WasteMethodName': method,
+            'WasteMaterialMixed': material,
+            'WasteWeight': weight,
+            'WasteUnitOfMeasureName': uom,
+            'WasteReasonName': reason,
+            'ReasonNote': note,
+            'ActualDate': get_timestamp(zone=self.client.state)
+        }
+        self.client.manage_plants(
+            [data],
+            action='destroyplants',
+            license_number=self._license
+        )
+
+    def manicure(
+            self,
+            weight,
+            harvest_name=None,
+            location_name=None,
+            patient_license=None,
+            uom='Grams',
+    ):
+        """Manicure the plant.
+        Args:
+            weight (float): Required harvest weight.
+            harvest_name (str): Optional harvest name.
+            location_name (str): The drying location's name.
+            patient_license (str): A patient's license number.
+            uom (str): The unit of measure
+        """
+        if location_name is None:
+            location_name = self.location_name
+        data = {
+            'Plant': self.label,
+            'Weight': weight,
+            'UnitOfWeight': uom,
+            'DryingLocation': location_name,
+            'HarvestName': harvest_name,
+            'PatientLicenseNumber': patient_license,
+            'ActualDate': get_timestamp(zone=self.client.state)
+        }
+        self.client.manage_plants(
+            [data],
+            action='manicureplants',
+            license_number=self._license
+        )
+        # TODO: Implement return_obs
+
+    def harvest(
+            self,
+            harvest_name,
+            weight,
+            location_name=None,
+            patient_license=None,
+            uom='Grams',
+    ):
+        """Harvest the plant.
+        Args:
+            harvest_name (str): Required harvest name.
+            weight (float): Required harvest weight.
+            location_name (str): The harvest location's name.
+            patient_license (str): A patient's license number.
+            uom (str): The unit of measure.
+        """
+        if location_name is None:
+            location_name = self.location_name
+        data = {
+            'Plant': self.label,
+            'Weight': weight,
+            'UnitOfWeight': uom,
+            'DryingLocation': location_name,
+            'HarvestName': harvest_name,
+            'PatientLicenseNumber': patient_license,
+            'ActualDate': get_timestamp(zone=self.client.state)
+        }
+        self.client.manage_plants(
+            [data],
+            action='harvestplants',
+            license_number=self._license
+        )
+        # TODO: Implement return_obs
+
+
 class PlantBatch(Model):
     """A class that represents a cannabis plant batch.
     ```js
         {
             "Id": 5,
             "Name": "Demo Plant Batch 1",
             "Type": "Seed",
@@ -831,217 +1210,404 @@
         super().__init__(client, properties, license_number)
         for k, v in self.RETURNED_VALUES.items():
             try:
                 self.__dict__[v] = properties[k]
             except KeyError:
                 pass
 
-    @classmethod
-    def create_from_json(cls, client, license_number, json):
-        """Initiate a class instance from a dictionary."""
-        new_obj = cls(client, json, license_number)
-        new_obj.create(license_number)
-        return new_obj
+    # TODO: Implement add_additive, add_additives
 
-    def create(self, license_number):
+    def create(self, license_number=''):
         """Create a plant batch record in Metrc."""
         context = self.to_dict()
         data = clean_dictionary(context, snake_to_camel)
         self.client.manage_batches([data], 'createplantings', license_number)
 
-    def create_package(self, data):
+    def create_package(
+            self,
+            item_name,
+            tag,
+            count,
+            location='',
+            note='',
+            trade_sample=False,
+            donation=False,
+    ):
         """Create a package from the plant batch."""
+        data = {
+            'id': self.uid,
+            'count': count,
+            'location': location or self.location_name,
+            'item': item_name,
+            'tag': tag,
+            'note': note,
+            'is_trade_sample': trade_sample,
+            'is_donation': donation,
+            'actual_date': get_timestamp(zone=self.client.state)
+        }
         data = clean_dictionary(data, snake_to_camel)
-        self.client.manage_batches([data], 'createpackages', self._license) # , from_mother=True
+        self.client.manage_batches([data], 'createpackages', self._license)
+        # TODO: Implement return_obs
 
-    def create_package_from_plants(self, data):
-        """Create a package from the plant batch."""
-        data = clean_dictionary(data, snake_to_camel)
-        self.client.manage_batches([data], '/create/packages/frommotherplant', self._license)
+    # TODO: Implement create_packages
 
-    def change_growth_phase(self, data):
-        """Change the growth phase of the batch."""
+    def create_package_from_mother(
+            self,
+            tag,
+            item,
+            count,
+            location=None,
+            note='',
+            trade_sample=False,
+            donation=False,
+    ):
+        """Create a package from the plant batch mother plant."""
+        data = {
+            'PlantBatch': self.name,
+            'Count': count,
+            'Location': location or self.location_name,
+            'Item': item,
+            'Tag': tag,
+            'Note': note,
+            'IsTradeSample': trade_sample,
+            'IsDonation': donation,
+            'ActualDate': get_timestamp(zone=self.client.state),
+        }
         data = clean_dictionary(data, snake_to_camel)
+        self.client.manage_batches(
+            [data],
+            '/create/packages/frommotherplant',
+            self._license,
+        )
+        # TODO: Implement return_obs
+
+    def change_growth_phase(
+            self,
+            tag,
+            count=1,
+            growth_phase='Vegetative',
+            location=None,
+            patient_license=None,
+    ):
+        """Change the growth phase of the batch.
+        Args:
+            tag (str): A plant tag for the new growth phase for the plants.
+                Subsequent tags will be used for plants beyond the first.
+            count (int): The number of plants to change growth phase, 1 by
+                default.
+            growth_phase (str): The growth phase for the plant(s), Flowering
+                or Vegetative. Vegetative is used by default.
+            location (str): A location for the plants, the current location of
+                the plant batch is used by default.
+            patient_license (str): An optional patient license number.
+        """
+        data = {
+            'Name': self.name,
+            'Count': count,
+            'StartingTag': tag,
+            'GrowthPhase': growth_phase,
+            'NewLocation': location or self.location_name,
+            'GrowthDate': get_timestamp(zone=self.client.state),
+            'PatientLicenseNumber': patient_license,
+        }
         self.client.manage_batches([data], 'changegrowthphase', self._license)
 
     def destroy_plants(self, count, reason):
         """Destroy a number of plants for a given reason.
         Args:
             count (int): The number of plants to destroy.
             reason (str): The reason for the destruction.
         """
-        date = datetime.now().strftime('%Y-%m-%d')
         data = {
             'PlantBatch': self.name,
             'Count': count,
             'ReasonNote': reason,
-            'ActualDate': date
+            'ActualDate': get_timestamp(zone=self.client.state),
         }
         self.client.manage_batches([data], 'destroy', self._license)
 
+    def split(self, name, count, location=None):
+        """Split the batch.
+        Args:
+            name (dict): The name of the new batch.
+            count (int): The number of plants to include in the new batch.
+            location (str): An optional location for the plant.
+        """
+        data = {
+            'PlantBatch': self.name,
+            'GroupName': name,
+            'Count': count,
+            'Location': location or self.location_name,
+            'Strain': self.strain_name,
+            'PatientLicenseNumber': None,
+            'ActualDate': get_timestamp(zone=self.client.state),
+        }
+        self.client.manage_batches([data], 'split', self._license)
+        # TODO: Implement return_obs
+
 
 class LabResult(Model):
-    """A class that represents a cannabis lab result.
+    """A class that represents a cannabis lab result. Metrc documentation
+    states:
 
-    The Lab Results tab displays the details of each individual lab test performed on
-    the package. A Document Download button is available on each row on the Lab
-    Results tab to view the associated certificate of analysis (COA), which the
-    laboratory staff uploads when test results are recorded. The test results and
-    COA are available on the source package and any related packages only after
-    the laboratory staff releases the results
+    The Lab Results tab displays the details of each individual lab test
+    performed on the package. A Document Download button is available on each
+    row on the Lab Results tab to view the associated certificate of analysis
+    (COA), which the laboratory staff uploads when test results are recorded.
+    The test results and COA are available on the source package and any
+    related packages only after the laboratory staff releases the results.
     """
 
-    @classmethod
-    def create_from_json(cls, client, license_number, json):
-        """Initiate a class instance from a dictionary."""
-        new_obj = cls(client, json, license_number)
-        new_obj.post(license_number)
-        return new_obj
-
-    def post(self, data={}):
+    def create(self, data={}):
         """Post lab result data."""
         context = self.to_dict()
         result = clean_dictionary(data, snake_to_camel)
         self.client.post_lab_results([{**context, **result}], self._license)
 
+    def post(self, data={}):
+        """Post lab result data. Equivalent alternative of `create`."""
+        self.create(data)
+
     def upload_coa(self, data={}):
         """Upload lab result CoA."""
         context = self.to_dict()
         result = clean_dictionary(data, snake_to_camel)
         self.client.upload_coas([{**context, **result}], self._license)
 
     def release(self, data={}):
         """Release lab results."""
         context = self.to_dict()
         result = clean_dictionary(data, snake_to_camel)
         self.client.release_lab_results([{**context, **result}], self._license)
 
 
+class Receipt(Model):
+    """A class that represents a cannabis sale receipt. Sales are reported to
+    record the transfer of cannabis products to a consumer, patient or
+    caregiver.
+
+    When you request receipts you receive the following object.
+    ```js
+    {
+        "Id": 1,
+        "ReceiptNumber": null,
+        "SalesDateTime": "2016-01-01T17:35:45.000",
+        "SalesCustomerType": "Consumer",
+        "PatientLicenseNumber": null,
+        "CaregiverLicenseNumber": null,
+        "IdentificationMethod": null,
+        "TotalPackages": 0,
+        "TotalPrice": 0.0,
+        "Transactions": [],
+        "IsFinal": false,
+        "ArchivedDate": null,
+        "RecordedDateTime": "0001-01-01T00:00:00+00:00",
+        "RecordedByUserName": null,
+        "LastModified": "0001-01-01T00:00:00+00:00"
+    }
+    ```
+
+    When you create a receipt, you pass the following object.
+    ```js
+    {
+        "SalesDateTime": "2016-10-04T16:44:53.000",
+        "SalesCustomerType": "Consumer",
+        "PatientLicenseNumber": null,
+        "CaregiverLicenseNumber": null,
+        "IdentificationMethod": null,
+        "Transactions": [
+            {
+                "PackageLabel": "ABCDEF012345670000010331",
+                "Quantity": 1.0,
+                "UnitOfMeasure": "Ounces",
+                "TotalAmount": 9.99
+            }
+        ]
+    }
+    ```
+    """
+
+    RETURNED_VALUES = {
+        'ReceiptNumber': 'receipt_number',
+        'TotalPackages': 'total_packages',
+        'TotalPrice': 'total_price',
+        'IsFinal': 'is_final',
+        'RecordedDateTime': 'recorded_date_time',
+        'RecordedByUserName': 'recorded_by_user_name',
+        'LastModified': 'last_modified',
+    }
+
+    def create(self):
+        """Create a receipt record in Metrc."""
+        context = self.to_dict()
+        data = clean_nested_dictionary(context, snake_to_camel)
+        self.client.create_receipts([data], license_number=self._license)
+
+    def update(self, **kwargs):
+        """Update the receipt given parameters as keyword arguments."""
+        context = self.to_dict().copy()
+        data = update_dict(context, **kwargs)
+        data = remove_dict_fields(data, self.RETURNED_VALUES.keys())
+        data = remove_dict_nulls(data)
+        self.client.update_receipts([data], self._license)
+
+    def delete(self):
+        """Delete the receipt."""
+        self.client.delete_receipt(self.id, self._license)
+
+
+class Strain(Model):
+    """A class that represents a cannabis strain.
+    ```js
+        {
+            "Id": 1,
+            "Name": "Old-time Moonshine",
+            "TestingStatus": "InHouse",
+            "ThcLevel": 0.1865,
+            "CbdLevel": 0.1075,
+            "IndicaPercentage": 25.0,
+            "SativaPercentage": 75.0
+        }
+    ```
+    """
+
+    def create(self):
+        """Create a strain record in Metrc."""
+        context = self.to_dict()
+        data = clean_dictionary(context, snake_to_camel)
+        self.client.create_strains([data])
+
+    def update(self, **kwargs):
+        """Update the strain given parameters as keyword arguments."""
+        context = self.to_dict()
+        data = update_dict(context, **kwargs)
+        self.client.update_strains([data], license_number=self._license)
+
+    def delete(self):
+        """Delete the strain."""
+        self.client.delete_strain(self.id, license_number=self._license)
+
+
 class Transfer(Model):
-    """A class that represents a cannabis transfer.
+    """A class that represents a cannabis transfer. Metrc documentation states:
+
     Transfers are a key component of the chain of custody process.
-    
     A transfer must be created anytime a package moves from one licensee to
     another, even if the two facilities are located on the same property.
 
     Packages can only be transported from one licensee to another by a licensed
-    Distributor. A Testing Laboratory is allowed to transport test samples for official
-    state testing. Distributors and Testing Laboratories are required to record the
-    actual departure time from the origin facility and the actual arrival time at the
-    destination facility in Metrc real-time.
+    Distributor. A Testing Laboratory is allowed to transport test samples for
+    official state testing. Distributors and Testing Laboratories are required
+    to record the actual departure time from the origin facility and the actual
+    arrival time at the destination facility in Metrc real-time.
 
     A package must be received in its entirety (the system DOES NOT allow
-    receiving a partial package).
-
-    A transfer can be rejected by individual package, or in whole by rejecting all
-    packages.
-
-    A rejected package requires the originating Licensee to receive the package
-    back into inventory.
-
-    A package must exist in order to be selected for transfer. Transfers are done in
-    real time and are inventory dependent.
-
-    When receiving a package, any adjustments to the weight, volume, or count may
-    be reported to the State.
-
-    If there are any questions about a transfer, reject it.
+    receiving a partial package). A transfer can be rejected by individual
+    package, or in whole by rejecting all packages. A rejected package requires
+    the originating Licensee to receive the package back into inventory.
+    A package must exist in order to be selected for transfer. Transfers are
+    done in real time and are inventory dependent. When receiving a package,
+    any adjustments to the weight, volume, or count may be reported to the
+    State. If there are any questions about a transfer, reject it.
 
     A transfer can be modified , or voided, up until the time that the
-    Distributor or Testing Laboratory marks that it has departed the facility. Once the
-    transfer process has begun, the transfer may not be modified except by the Distributor
-    or Testing Laboratory to edit estimated departure and arrival times, or driver and vehicle
-    information (see Edit Transporter Info below).
-
-    When modifying transfers, each of the transfer fields may be modified at the same level
-    of detail as when the transfer was created. Edits may be completed for a variety of
-    reasons including: error correction, changes in destination, changes in product, etc.
-
-    Voiding a transfer can only be completed by the originating business. Voiding a transfer
-    permanently eliminates it and moves the product back into the originator’s inventory.
-    Once a transfer has been voided, it cannot be reinstated and all associated packages
-    will be returned to the transfer originator’s inventory
-
-    Receiving a transfer is the final point of exchange in the chain of custody.
+    Distributor or Testing Laboratory marks that it has departed the facility.
+    Once the transfer process has begun, the transfer may not be modified
+    except by the Distributor or Testing Laboratory to edit estimated departure
+    and arrival times, or driver and vehicle information(see Edit Transporter
+    Info below).
+
+    When modifying transfers, each of the transfer fields may be modified at
+    the same level of detail as when the transfer was created. Edits may be
+    completed for a variety of reasons including: error correction, changes in
+    destination, changes in product, etc.
+
+    Voiding a transfer can only be completed by the originating business.
+    Voiding a transfer permanently eliminates it and moves the product back
+    into the originator’s inventory. Once a transfer has been voided, it cannot
+    be reinstated and all associated packages will be returned to the transfer
+    originator's inventory.
+
+    Receiving a transfer is the final point of exchange in the chain of
+    custody.
+
+    Type `Transfer` is used for all transfers except transfers requiring the
+    use of a `Wholesale Manifest` or `Return` manifest. A `Return` transfer is
+    used only for the transfer of defective manufactured products back to the
+    originating licensee. A `Wholesale Manifest` transfer is used when =
+    transferring products to a Retailer licensee. When a `Wholesale Manifest`
+    is used, the originator is required to record the wholesale price of each
+    package in the transfer. A Microbusiness functioning as a Distributor with
+    a transfer that includes a Retailer licensee, or another Microbusiness
+    licensee functioning as a Retailer, shall follow the process above. It is
+    recommended that Nurseries utilize a `Wholesale Manifest` when transferring
+    seeds or immature plants to a Retailer.
     """
 
     RETURNED_VALUES = {}
 
-    @classmethod
-    def create_from_json(cls, client, json):
-        """Initiate a class instance from a dictionary."""
-        obj = cls(client, json)
-        obj.create()
-        return obj
-
     def create(self):
         """Create a transfer record in Metrc."""
         context = self.to_dict()
         data = clean_nested_dictionary(context, snake_to_camel)
         self.client.create_transfers([data], license_number=self._license)
 
     def update(self, **kwargs):
         """Update the transfer given parameters as keyword arguments."""
         context = self.to_dict().copy()
-        data = update_context(context, **kwargs)
+        data = update_dict(context, **kwargs)
         data = remove_dict_fields(data, self.RETURNED_VALUES.keys())
         data = remove_dict_nulls(data)
         self.client.update_transfers([data], self._license)
 
     def delete(self):
         """Delete the transfer."""
         self.client.delete_transfer(self.id, self._license)
 
 
-
 class TransferTemplate(Model):
-    """A class that represents a cannabis transfer template.
-    Transfer templates can be used for transfers to the same
-    destination licensee utilizing the same:
-
+    """A class that represents a cannabis transfer template. The template can
+    be copied to create other templates. Transfer templates can be used for
+    transfers to the same destination licensee utilizing the
+    same:
         - Planned Route
         - Transporter(s)
         - Driver(s)
         - Vehicle(s)
         - Package
-
-    The template can be copied to create other templates.
     """
 
     RETURNED_VALUES = {}
 
-    @classmethod
-    def create_from_json(cls, client, json):
-        """Initiate a class instance from a dictionary."""
-        obj = cls(client, json)
-        obj.create()
-        return obj
-
     def create(self):
         """Create a transfer template record in Metrc."""
         context = self.to_dict()
         data = clean_nested_dictionary(context, snake_to_camel)
-        self.client.create_transfer_templates([data], license_number=self._license)
+        self.client.create_transfer_templates(
+            [data],
+            license_number=self._license,
+        )
 
     def update(self, **kwargs):
-        """Update the transfer template given parameters as keyword arguments."""
+        """Update the transfer template given parameters as keyword
+        arguments."""
         context = self.to_dict().copy()
-        data = update_context(context, **kwargs)
+        data = update_dict(context, **kwargs)
         data = remove_dict_fields(data, self.RETURNED_VALUES.keys())
         data = remove_dict_nulls(data)
         self.client.update_transfer_templates([data], self._license)
 
     def delete(self):
         """Delete the transfer template."""
         self.client.delete_transfer_template(self.id, self._license)
 
 
 class Transaction(Model):
-    """A class that represents a cannabis sale transaction.
-    When you get a transaction you receive an object as follows.
+    """A class that represents a cannabis sale transaction. When you get a
+    transaction you receive an object as follows.
     ```js
     {
         "SalesDate": "2015-01-08",
         "TotalTransactions": 40,
         "TotalPackages": 40,
         "TotalPrice": 399.6
     }
@@ -1092,123 +1658,46 @@
         "TotalAmount": 9.99
     }
     ```
     """
 
     RETURNED_VALUES = {}
 
-    @classmethod
-    def create_from_json(cls, client, json):
-        """Initiate a class instance from a dictionary."""
-        obj = cls(client, json)
-        obj.create()
-        return obj
-
     def create(self):
         """Create a transaction record in Metrc."""
         context = self.to_dict()
         data = clean_nested_dictionary(context, snake_to_camel)
         self.client.create_transactions([data], license_number=self._license)
 
     def update(self, **kwargs):
         """Update the transaction given parameters as keyword arguments."""
         context = self.to_dict().copy()
-        data = update_context(context, **kwargs)
+        data = update_dict(context, **kwargs)
         data = remove_dict_fields(data, self.RETURNED_VALUES.keys())
         data = remove_dict_nulls(data)
         self.client.update_transactions([data], self._license)
 
 
-
-class Receipt(Model):
-    """A class that represents a cannabis sale receipt.
-    Sales are reported to record the transfer of cannabis
-    products to a consumer, patient or caregiver.
-
-    When you request receipts you receive the following object.
-    ```js
-    {
-        "Id": 1,
-        "ReceiptNumber": null,
-        "SalesDateTime": "2016-01-01T17:35:45.000",
-        "SalesCustomerType": "Consumer",
-        "PatientLicenseNumber": null,
-        "CaregiverLicenseNumber": null,
-        "IdentificationMethod": null,
-        "TotalPackages": 0,
-        "TotalPrice": 0.0,
-        "Transactions": [],
-        "IsFinal": false,
-        "ArchivedDate": null,
-        "RecordedDateTime": "0001-01-01T00:00:00+00:00",
-        "RecordedByUserName": null,
-        "LastModified": "0001-01-01T00:00:00+00:00"
-    }
-    ```
-
-    When you create a receipt, you pass the following object.
-    ```js
-    {
-        "SalesDateTime": "2016-10-04T16:44:53.000",
-        "SalesCustomerType": "Consumer",
-        "PatientLicenseNumber": null,
-        "CaregiverLicenseNumber": null,
-        "IdentificationMethod": null,
-        "Transactions": [
-            {
-                "PackageLabel": "ABCDEF012345670000010331",
-                "Quantity": 1.0,
-                "UnitOfMeasure": "Ounces",
-                "TotalAmount": 9.99
-            }
-        ]
-    }
-    ```
-    """
-
-    @classmethod
-    def create_from_json(cls, client, json):
-        """Initiate a class instance from a dictionary."""
-        obj = cls(client, json)
-        obj.create()
-        return obj
-
-    def create(self):
-        """Create a receipt record in Metrc."""
-        context = self.to_dict()
-        data = clean_nested_dictionary(context, snake_to_camel)
-        self.client.create_receipts([data], license_number=self._license)
-
-    def update(self, **kwargs):
-        """Update the receipt given parameters as keyword arguments."""
-        context = self.to_dict().copy()
-        data = update_context(context, **kwargs)
-        data = remove_dict_nulls(data)
-        self.client.update_receipts([data], self._license)
-
-    def delete(self):
-        """Delete the receipt."""
-        self.client.delete_receipt(self.id, self._license)
-
-
 class Waste(Model):
-    """A class that represents cannabis waste.
-    
-    A harvest batch is created and given a
-    unique Harvest Name when plants
-    or plant material are harvested.
-
-    Plant waste must be recorded within three business days of destruction. In Metrc
-    plant waste can be recorded by Immature Plant Lot, Flowering Plant or by
-    Location.
-    2. Waste can also be recorded by Harvest Batch. See Metrc User Guide for details.
-    3. When recording Flowering Plant waste, the waste from multiple plants can be
-    recorded as a single waste event but the flowering plants contributing to the
-    waste must be individually identified.
-    4. If a plant is no longer viable, the waste must be recorded prior to recording its
-    destruction.
-    5. The reason for the waste must be identified using the Waste Reasons defined by
-    the State of California as listed in Exhibit 38 below. Use of some Waste
-    Reasons may be limited to certain license types, as determined by the State.
+    """A class that represents cannabis waste. Metrc documentation states:
+
+    A harvest batch is created and given a unique Harvest Name when plants or
+    plant material are harvested. [The following regulations need to be met.]
 
+    1. Plant waste must be recorded within three business days of destruction.
+    In Metrc plant waste can be recorded by Immature Plant Lot, Flowering Plant
+    or by Location. Waste can also be recorded by Harvest Batch. See the Metrc
+    User Guide for details.
+
+    2. When recording Flowering Plant waste, the waste from multiple plants can
+    be recorded as a single waste event but the flowering plants contributing
+    to the waste must be individually identified.
+
+    3. If a plant is no longer viable, the waste must be recorded prior to
+    recording its destruction.
+
+    4. The reason for the waste must be identified using the Waste Reasons
+    defined by the State of California as listed in Exhibit 38 below. Use of
+    some Waste Reasons may be limited to certain license types, as determined
+    by the State.
     """
     pass
```

### Comparing `cannlytics-0.0.8/cannlytics/utils/logistics.py` & `cannlytics-0.0.9/cannlytics/utils/logistics.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,84 +1,119 @@
-# -*- coding: utf-8 -*-
 """
-Logistics | Cannlytics
+Logistics Utilities | Cannlytics
+Copyright (c) 2021-2022 Cannlytics and Cannlytics Contributors
 
-Copyright (c) 2021 Cannlytics 
-Author: Keegan Skeate <keegan@cannlytics.com>  
-Created: 1/10/2021  
-
-License GPLv3+: GNU GPL version 3 or later <https://gnu.org/licenses/gpl.html>
-This is free software: you are free to change and redistribute it.
-There is NO WARRANTY, to the extent permitted by law.
+Authors: Keegan Skeate <keegan@cannlytics.com>
+Created: 11/5/2021
+Updated: 12/5/2021
+License: <https://github.com/cannlytics/cannlytics-engine/blob/main/LICENSE>
+
+Description: This script contains functions that are useful for logistics.
 """
-from googlemaps import Client, places
-from firebase_admin import initialize_app, firestore
+# Standard imports.
 from time import sleep
+from typing import List, Optional
 
+# External imports.
+from googlemaps import Client, places
 
-def get_google_maps_api_key():
-    """Get Google Maps API key."""
-    db = firestore.client()
-    admin = db.collection("admin")
-    google = admin.document("google").get()
-    google_data = google.to_dict()
-    return google_data["google_maps_api_key"]
+# Internal imports.
+from ..firebase import initialize_firebase, get_document
 
 
-def geocode_addresses(df):
-    """Geocode addresses in a dataframe."""
-    try:
-        initialize_app()
-    except ValueError:
-        pass
-    api_key = get_google_maps_api_key()
+def get_google_maps_api_key():
+    """Get Google Maps API key.
+    Returns:
+        (str): Returns the Google Maps API key stored
+            in the Firestore database.
+    """
+    # FIXME: Prefer using secret manager to Firestore for secrets.
+    database = initialize_firebase()
+    google_doc = get_document('admin/google', database=database)
+    google_data = google_doc.to_dict()
+    return google_data['google_maps_api_key']
+
+
+def geocode_addresses(df, api_key: Optional[str] = None):
+    """Geocode addresses in a dataframe.
+    Args:
+        df (DataFrame): A DataFrame containing the addresses to geocode.
+    Returns:
+        (DataFrame): Returns the DataFrame with geocoded latitudes and longitudes.
+    """
+    if api_key is None:
+        api_key = get_google_maps_api_key()
     gmaps = Client(key=api_key)
     for index, item in df.iterrows():
-        # FIXME: Handle existing lat and long more elegantly.
+        # TODO: Handle existing lat and long more elegantly.
         # try:
         #     if item.latitude and item.longitude:
         #         continue
         # except:
         #     pass
-        address = f"{item.street}, {item.city}, {item.state} {item.zip}"
+        address = f'{item.street}, {item.city}, {item.state} {item.zip}'
         geocode_result = gmaps.geocode(address)
         if geocode_result:
-            df.at[index, "formatted_address"] = geocode_result[0]["formatted_address"]
-            location = geocode_result[0]["geometry"]["location"]
-            print(item.name, "-->", location)
-            df.at[index, "latitude"] = location["lat"]
-            df.at[index, "longitude"] = location["lng"]
+            df.at[index, 'formatted_address'] = geocode_result[0]['formatted_address']
+            location = geocode_result[0]['geometry']['location']
+            print(item.name, '-->', location)
+            df.at[index, 'latitude'] = location['lat']
+            df.at[index, 'longitude'] = location['lng']
             # TODO: Round latitude and longitude (4-6 decimal places?)
-            for info in geocode_result[0]["address_components"]:
-                key = info["types"][0]
-                if key == "administrative_area_level_2":
-                    df.at[index, "county"] = info["long_name"]
+            for info in geocode_result[0]['address_components']:
+                key = info['types'][0]
+                if key == 'administrative_area_level_2':
+                    df.at[index, 'county'] = info['long_name']
 
-        sleep(2)  # Prevents spamming Google's servers (necessary?)
+        sleep(.2) # Prevents spamming Google's servers (necessary?).
     return df
 
 
-def search_for_address(query, api_key=None, fields=["formatted_address"]):
-    """Search for the address of a given name."""
+def search_for_address(
+        query: str,
+        api_key: Optional[str] = None,
+        fields: Optional[List[str]] = None,
+) -> List[dict]:
+    """Search for the address of a given name.
+    Args:
+        query (str): The text to use to search for an address.
+        api_key (): Optional, None by default.
+        fields (list): Optional, `formatted_address` is included by default.
+    Returns:
+        (list): A list of potential results.
+    """
     if api_key is None:
         api_key = get_google_maps_api_key()
+    if fields is None:
+        fields = ['formatted_address']
     gmaps = Client(key=api_key)
-    place = places.find_place(gmaps, query, "textquery", fields=fields)
-    return place["candidates"]
+    place = places.find_place(gmaps, query, 'textquery', fields=fields)
+    return place['candidates']
 
 
-def get_place_details(query, api_key=None, fields=[]):
-    """Get the place details for a given a name."""
+def get_place_details(
+        query: str,
+        api_key: Optional[str] = None,
+        fields: Optional[List[str]] = None,
+):
+    """Get the place details for a given a name.
+    Args:
+        query (str): The text to use to search for a place.
+        api_key (str): Optional Google Maps API key, None by default.
+        fields (list): Optional fields to retrieve.
+    Returns:
+        (dict): A dictionary of place details.
+    """
     if api_key is None:
         api_key = get_google_maps_api_key()
     if not fields:
         fields = [
-            "formatted_address",
-            "photo",
-            "opening_hours",
-            "website",
+            'formatted_address',
+            'photo',
+            'opening_hours',
+            'website',
         ]
     gmaps = Client(key=api_key)
-    search = places.find_place(gmaps, query, "textquery")
-    place_id = search["candidates"][0]["place_id"]
+    search = places.find_place(gmaps, query, 'textquery')
+    place_id = search['candidates'][0]['place_id']
     place = places.place(gmaps, place_id, fields=fields)
-    return place["result"]
+    return place['result']
```

### Comparing `cannlytics-0.0.8/cannlytics/utils/scraper.py` & `cannlytics-0.0.9/cannlytics/utils/web.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,177 +1,219 @@
-# -*- coding: utf-8 -*-
 """
-Scrape Website Data | Cannlytics
-Copyright © 2021 Cannlytics
-Author: Keegan Skeate <keegan@cannlytics.com>
-Created: 1/10/2021
+Web Utilities | Cannlytics
+Copyright (c) 2021-2022 Cannlytics
 
-License GPLv3+: GNU GPL version 3 or later <https://gnu.org/licenses/gpl.html>
-This is free software: you are free to change and redistribute it.
-There is NO WARRANTY, to the extent permitted by law.
+Authors: Keegan Skeate <keegan@cannlytics.com>
+Created: 1/10/2021
+Updated: 11/6/2021
+License: <https://github.com/cannlytics/cannlytics-engine/blob/main/LICENSE>
 
 Resources:
     https://stackoverflow.com/questions/54416896/how-to-scrape-email-and-phone-numbers-from-a-list-of-websites
     https://hackersandslackers.com/scraping-urls-with-beautifulsoup/
-    
+
 TODO:
     Improve with requests-html - https://github.com/psf/requests-html
     - Get #about
     - Get absolute URLs
     - Search for text (prices/analyses)
         r.html.search('Python is a {} language')[0]
 """
 import re
+from typing import Any, Tuple
 import requests
 from bs4 import BeautifulSoup
 
 
-def get_page_metadata(url):
-    """Scrape target URL for metadata."""
+def format_params(parameters, **kwargs):
+    """Format Metrc request parameters.
+    Returns:
+        (dict): Returns the parameters as a dictionary.
+    """
+    params = {}
+    for param in kwargs:
+        if kwargs[param]:
+            key = parameters[param]
+            params[key] = kwargs[param]
+    return params
+
+
+def get_page_metadata(url: str) -> Tuple:
+    """Scrape target URL for metadata.
+    Args:
+        url (str): The URL to scrape.
+    Returns:
+        (HTTPResponse): The HTTP response.
+        (str): The HTML text.
+        (dict): A dictionary of metadata, including: `description`, `image_url`,
+            `favicon`, and `brand_color`.
+    """
     headers = {
-        "Access-Control-Allow-Origin": "*",
-        "Access-Control-Allow-Methods": "GET",
-        "Access-Control-Allow-Headers": "Content-Type",
-        "Access-Control-Max-Age": "3600",
-        "User-Agent": "Mozilla/5.0 (X11; Ubuntu; Linux x86_64; rv:52.0) Gecko/20100101 Firefox/52.0",
+        'Access-Control-Allow-Origin': '*',
+        'Access-Control-Allow-Methods': 'GET',
+        'Access-Control-Allow-Headers': 'Content-Type',
+        'Access-Control-Max-Age': '3600',
+        'User-Agent': 'Mozilla/5.0 (X11; Ubuntu; Linux x86_64; rv:52.0) Gecko/20100101 Firefox/52.0',
     }
     # Handle URLs without http beginning
-    if not url.startswith("http"):
-        url = "http://" + url
+    if not url.startswith('http'):
+        url = 'http://' + url
     response = requests.get(url, headers=headers)
-    html = BeautifulSoup(response.content, "html.parser")
+    html = BeautifulSoup(response.content, 'html.parser')
     metadata = {
-        "description": get_description(html),
-        "image_url": get_image(html),  # FIXME: Append URL if relative path.
-        "favicon": get_favicon(html, url),
-        "brand_color": get_theme_color(html),
+        'description': get_page_description(html),
+        'image_url': get_page_image(html),  # FIXME: Append URL if relative path.
+        'favicon': get_page_favicon(html, url),
+        'brand_color': get_page_theme_color(html),
     }
     return response, html, metadata
 
 
-def get_description(html):
-    """Scrape page description."""
+def get_page_description(html: str) -> str:
+    """Scrape page description.
+    Args:
+        html (str): A body of HTML text.
+    Returns:
+        (str): A description excerpt from the page.
+    """
     description = None
-    if html.find("meta", property="description"):
-        description = html.find("meta", property="description").get("content")
-    elif html.find("meta", property="og:description"):
-        description = html.find("meta", property="og:description").get("content")
-    elif html.find("meta", property="twitter:description"):
-        description = html.find("meta", property="twitter:description").get("content")
-    elif html.find("p"):
-        description = html.find("p").contents
+    if html.find('meta', property='description'):
+        description = html.find('meta', property='description').get('content')
+    elif html.find('meta', property='og:description'):
+        description = html.find('meta', property='og:description').get('content')
+    elif html.find('meta', property='twitter:description'):
+        description = html.find('meta', property='twitter:description').get('content')
+    elif html.find('p'):
+        description = html.find('p').contents
     if isinstance(description, list):
         try:
             description = description[0]
         except IndexError:
             pass
     return description
 
 
-def get_image(html):
-    """Scrape share image."""
+def get_page_image(html: str) -> str:
+    """Scrape share image.
+    Args:
+        html (str): A body of HTML text.
+    Returns:
+        (str): Returns the first image URL if found.
+    """
     image = None
-    if html.find("meta", property="image"):
-        image = html.find("meta", property="image").get("content")
-    elif html.find("meta", property="og:image"):
-        image = html.find("meta", property="og:image").get("content")
-    elif html.find("meta", property="twitter:image"):
-        image = html.find("meta", property="twitter:image").get("content")
-    elif html.find("img", src=True):
-        image = html.find_all("img")[0].get("src")
+    if html.find('meta', property='image'):
+        image = html.find('meta', property='image').get('content')
+    elif html.find('meta', property='og:image'):
+        image = html.find('meta', property='og:image').get('content')
+    elif html.find('meta', property='twitter:image'):
+        image = html.find('meta', property='twitter:image').get('content')
+    elif html.find('img', src=True):
+        image = html.find_all('img')[0].get('src')
     return image
 
 
-def get_favicon(html, url):
-    """Scrape favicon."""
-    if html.find("link", attrs={"rel": "icon"}):
-        favicon = html.find("link", attrs={"rel": "icon"}).get("href")
-    elif html.find("link", attrs={"rel": "shortcut icon"}):
-        favicon = html.find("link", attrs={"rel": "shortcut icon"}).get("href")
+def get_page_favicon(html: str, url: str) -> str:
+    """Scrape favicon.
+    Args:
+        html (str): A body of HTML text.
+        url (str): The URL of the page.
+    Returns:
+        (str): The URL of any potential favicon.
+    """
+    if html.find('link', attrs={'rel': 'icon'}):
+        favicon = html.find('link', attrs={'rel': 'icon'}).get('href')
+    elif html.find('link', attrs={'rel': 'shortcut icon'}):
+        favicon = html.find('link', attrs={'rel': 'shortcut icon'}).get('href')
     else:
-        favicon = f'{url.rstrip("/")}/favicon.ico'
+        favicon = f"{url.rstrip('/')}/favicon.ico"
     return favicon
 
 
-def get_theme_color(html):
-    """Scrape brand color."""
-    if html.find("meta", property="theme-color"):
-        color = html.find("meta", property="theme-color").get("content")
+def get_page_theme_color(html: str) -> str:
+    """Scrape brand color.
+    Args:
+        html (str): A body of HTML text.
+    Returns:
+        (str): An hex color code if found.
+    """
+    if html.find('meta', property='theme-color'):
+        color = html.find('meta', property='theme-color').get('content')
         return color
-    return None
+    else:
+        return None
 
 
-def get_phone(html, response):
-    """Scrape phone number."""
+def get_page_phone_number(html: str, response: Any) -> str:
+    """Scrape phone number.
+    Args:
+        html (str): A body of HTML text.
+        response (HTTPResponse): An HTTP response.
+    Returns:
+        (str): Returns the first phone number found.
+    """
     try:
-        phone = html.select("a[href*=callto]")[0].text
+        phone = html.select('a[href*=callto]')[0].text
         return phone
     except:
         pass
     try:
         phone = re.findall(
-            r"\(?\b[2-9][0-9]{2}\)?[-][2-9][0-9]{2}[-][0-9]{4}\b", response.text
+            r'\(?\b[2-9][0-9]{2}\)?[-][2-9][0-9]{2}[-][0-9]{4}\b', response.text
         )[0]
         return phone
     except:
         pass
     try:
         phone = re.findall(
-            r"\(?\b[2-9][0-9]{2}\)?[-. ]?[2-9][0-9]{2}[-. ]?[0-9]{4}\b", response.text
+            r'\(?\b[2-9][0-9]{2}\)?[-. ]?[2-9][0-9]{2}[-. ]?[0-9]{4}\b', response.text
         )[-1]
         return phone
     except:
-        print("Phone number not found")
-        phone = ""
+        print('Phone number not found')
+        phone = ''
         return phone
 
 
-def get_email(html, response):
-    """Get email."""
+def get_page_email(html: str, response: Any) -> str:
+    """Get email.
+    Args:
+        html (str): A body of HTML text.
+        response (HTTPResponse): An HTTP response.
+    Returns:
+        (str): Returns the first email found on the page.
+    """
     try:
         email = re.findall(
-            r"([a-zA-Z0-9._-]+@[a-zA-Z0-9._-]+\.[a-zA-Z0-9_-]+)", response.text
+            r'([a-zA-Z0-9._-]+@[a-zA-Z0-9._-]+\.[a-zA-Z0-9_-]+)', response.text
         )[-1]
         return email
     except:
         pass
     try:
-        email = html.select("a[href*=mailto]")[-1].text
+        email = html.select('a[href*=mailto]')[-1].text
     except:
-        print("Email not found")
-        email = ""
+        print('Email not found')
+        email = ''
         return email
 
 
 def find_lab_address():
     """
-    TODO: Tries to find a lab's address from their website, then Google Maps.
+    TODO: Try to find a lab's address from their website, then Google Maps.
     """
-    street, city, state, zipcode = None, None, None, None
-    return street, city, state, zipcode
+    raise NotImplementedError
+    # street, city, state, zipcode = None, None, None, None
+    # return street, city, state, zipcode
 
 
 def find_lab_linkedin():
     """
-    TODO: Tries to find a lab's LinkedIn URL. (Try to find LinkedIn on homepage?)
+    TODO: Tru to find a lab's LinkedIn URL. (Try to find LinkedIn on homepage?)
     """
-    return ""
+    raise NotImplementedError
 
 
 def find_lab_url():
     """
     TODO: Find a lab's website URL. (Google search for name?)
     """
-    return ""
-
-
-def clean_string_columns(df):
-    """Clean string columns in a dataframe."""
-    for column in df.columns:
-        try:
-            df[column] = df[column].str.title()
-            df[column] = df[column].str.replace("Llc", "LLC")
-            df[column] = df[column].str.replace("L.L.C.", "LLC")
-            df[column] = df[column].str.strip()
-        except AttributeError:
-            pass
-    return df
+    raise NotImplementedError
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

