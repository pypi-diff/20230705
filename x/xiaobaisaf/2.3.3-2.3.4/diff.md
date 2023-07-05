# Comparing `tmp/xiaobaisaf-2.3.3.tar.gz` & `tmp/xiaobaisaf-2.3.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "xiaobaisaf-2.3.3.tar", last modified: Fri Jun 30 17:18:47 2023, max compression
+gzip compressed data, was "xiaobaisaf-2.3.4.tar", last modified: Wed Jul  5 15:46:09 2023, max compression
```

## Comparing `xiaobaisaf-2.3.3.tar` & `xiaobaisaf-2.3.4.tar`

### file list

```diff
@@ -1,74 +1,75 @@
-drwxrwxrwx   0        0        0        0 2023-06-30 17:18:47.357668 xiaobaisaf-2.3.3/
--rw-rw-rw-   0        0        0    35181 2023-06-27 16:34:34.000000 xiaobaisaf-2.3.3/LICENSE
--rw-rw-rw-   0        0        0    11869 2023-06-30 17:18:47.357668 xiaobaisaf-2.3.3/PKG-INFO
--rw-rw-rw-   0        0        0    11198 2023-06-30 17:16:51.000000 xiaobaisaf-2.3.3/README.md
-drwxrwxrwx   0        0        0        0 2023-06-30 17:18:47.319741 xiaobaisaf-2.3.3/saf/
--rw-rw-rw-   0        0        0     1436 2023-06-27 16:40:21.000000 xiaobaisaf-2.3.3/saf/__init__.py
--rw-rw-rw-   0        0        0      152 2023-06-30 17:16:51.000000 xiaobaisaf-2.3.3/saf/__version__.py
-drwxrwxrwx   0        0        0        0 2023-06-30 17:18:47.320738 xiaobaisaf-2.3.3/saf/data/
--rw-rw-rw-   0        0        0      225 2023-06-27 16:34:35.000000 xiaobaisaf-2.3.3/saf/data/__init__.py
--rw-rw-rw-   0        0        0     2943 2023-06-27 16:34:36.000000 xiaobaisaf-2.3.3/saf/data/config.py
--rw-rw-rw-   0        0        0     4286 2023-06-27 16:34:38.000000 xiaobaisaf-2.3.3/saf/data/favicon.ico
-drwxrwxrwx   0        0        0        0 2023-06-30 17:18:47.320738 xiaobaisaf-2.3.3/saf/example/
--rw-rw-rw-   0        0        0      100 2023-06-27 16:34:37.000000 xiaobaisaf-2.3.3/saf/example/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-30 17:18:47.322732 xiaobaisaf-2.3.3/saf/example/api/
-drwxrwxrwx   0        0        0        0 2023-06-30 17:18:47.323730 xiaobaisaf-2.3.3/saf/example/api/Config/
--rw-rw-rw-   0        0        0      131 2023-06-27 16:34:37.000000 xiaobaisaf-2.3.3/saf/example/api/Config/__init__.py
--rw-rw-rw-   0        0        0     5086 2023-06-27 16:34:37.000000 xiaobaisaf-2.3.3/saf/example/api/Config/config.py
-drwxrwxrwx   0        0        0        0 2023-06-30 17:18:47.324727 xiaobaisaf-2.3.3/saf/example/api/TestCases/
--rw-rw-rw-   0        0        0      129 2023-06-27 16:34:37.000000 xiaobaisaf-2.3.3/saf/example/api/TestCases/__init__.py
--rw-rw-rw-   0        0        0     1438 2023-06-27 16:34:37.000000 xiaobaisaf-2.3.3/saf/example/api/TestCases/test_one_html_case_template.py
-drwxrwxrwx   0        0        0        0 2023-06-30 17:18:47.326722 xiaobaisaf-2.3.3/saf/example/api/Utils/
--rw-rw-rw-   0        0        0     1389 2023-06-28 15:26:03.000000 xiaobaisaf-2.3.3/saf/example/api/Utils/ExcelUtils.py
--rw-rw-rw-   0        0        0     2099 2023-06-27 16:34:37.000000 xiaobaisaf-2.3.3/saf/example/api/Utils/YamlUtils.py
--rw-rw-rw-   0        0        0      308 2023-06-27 16:34:37.000000 xiaobaisaf-2.3.3/saf/example/api/Utils/__init__.py
--rw-rw-rw-   0        0        0     1111 2023-06-28 15:26:03.000000 xiaobaisaf-2.3.3/saf/example/api/Utils/api_client.py
--rw-rw-rw-   0        0        0      285 2023-06-28 15:26:03.000000 xiaobaisaf-2.3.3/saf/example/api/Utils/logger.py
--rw-rw-rw-   0        0        0      129 2023-06-27 16:34:37.000000 xiaobaisaf-2.3.3/saf/example/api/__init__.py
--rw-rw-rw-   0        0        0     1211 2023-06-27 16:34:37.000000 xiaobaisaf-2.3.3/saf/example/api/run.py
--rw-rw-rw-   0        0        0      549 2023-06-27 16:34:37.000000 xiaobaisaf-2.3.3/saf/example/api/send_email_script.py
-drwxrwxrwx   0        0        0        0 2023-06-30 17:18:47.326722 xiaobaisaf-2.3.3/saf/example/web/
-drwxrwxrwx   0        0        0        0 2023-06-30 17:18:47.330711 xiaobaisaf-2.3.3/saf/example/web/Cases/
--rw-rw-rw-   0        0        0      140 2023-06-27 16:34:37.000000 xiaobaisaf-2.3.3/saf/example/web/Cases/__init__.py
--rw-rw-rw-   0        0        0     2441 2023-06-27 16:34:37.000000 xiaobaisaf-2.3.3/saf/example/web/Cases/conftest.py
--rw-rw-rw-   0        0        0      930 2023-06-27 16:34:37.000000 xiaobaisaf-2.3.3/saf/example/web/Cases/test_xiaobai_case_allure.py
--rw-rw-rw-   0        0        0      962 2023-06-27 16:34:37.000000 xiaobaisaf-2.3.3/saf/example/web/Cases/test_xiaobai_case_submitBug.py
--rw-rw-rw-   0        0        0      320 2023-06-27 16:34:37.000000 xiaobaisaf-2.3.3/saf/example/web/Cases/test_xiaobai_case_v1.py
--rw-rw-rw-   0        0        0     1192 2023-06-27 16:34:37.000000 xiaobaisaf-2.3.3/saf/example/web/Cases/test_xiaobai_case_v2.py
--rw-rw-rw-   0        0        0      228 2023-06-27 16:34:37.000000 xiaobaisaf-2.3.3/saf/example/web/Cases/test_xiaobai_case_v3.py
-drwxrwxrwx   0        0        0        0 2023-06-30 17:18:47.331709 xiaobaisaf-2.3.3/saf/example/web/Utils/
--rw-rw-rw-   0        0        0     1389 2023-06-28 15:26:03.000000 xiaobaisaf-2.3.3/saf/example/web/Utils/ExcelUtils.py
--rw-rw-rw-   0        0        0     2099 2023-06-28 15:26:03.000000 xiaobaisaf-2.3.3/saf/example/web/Utils/YamlUtils.py
--rw-rw-rw-   0        0        0      308 2023-06-28 15:26:03.000000 xiaobaisaf-2.3.3/saf/example/web/Utils/__init__.py
--rw-rw-rw-   0        0        0      285 2023-06-28 15:26:03.000000 xiaobaisaf-2.3.3/saf/example/web/Utils/logger.py
--rw-rw-rw-   0        0        0      435 2023-06-27 16:34:37.000000 xiaobaisaf-2.3.3/saf/example/web/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-30 17:18:47.332706 xiaobaisaf-2.3.3/saf/example/web/pageObject/
--rw-rw-rw-   0        0        0      166 2023-06-27 16:34:37.000000 xiaobaisaf-2.3.3/saf/example/web/pageObject/__init__.py
--rw-rw-rw-   0        0        0      152 2023-06-27 16:34:37.000000 xiaobaisaf-2.3.3/saf/example/web/pageObject/register_page_element.py
-drwxrwxrwx   0        0        0        0 2023-06-30 17:18:47.340686 xiaobaisaf-2.3.3/saf/utils/
--rw-rw-rw-   0        0        0     8132 2023-06-27 16:34:36.000000 xiaobaisaf-2.3.3/saf/utils/BugUtils.py
--rw-rw-rw-   0        0        0      134 2023-06-30 17:18:46.000000 xiaobaisaf-2.3.3/saf/utils/Demo.py
--rw-rw-rw-   0        0        0     2076 2023-06-27 16:40:34.000000 xiaobaisaf-2.3.3/saf/utils/MonitorAndroidDeviceGUI.py
--rw-rw-rw-   0        0        0     8917 2023-06-27 16:34:38.000000 xiaobaisaf-2.3.3/saf/utils/MonitorAndroidPackageCLI.py
--rw-rw-rw-   0        0        0    14192 2023-06-27 16:34:38.000000 xiaobaisaf-2.3.3/saf/utils/MonitorAndroidPackageGUI.py
--rw-rw-rw-   0        0        0     7790 2023-06-30 17:18:46.000000 xiaobaisaf-2.3.3/saf/utils/MonitorAndroidPackagePower.py
--rw-rw-rw-   0        0        0     5933 2023-06-27 16:34:38.000000 xiaobaisaf-2.3.3/saf/utils/MonitorDBs.py
--rw-rw-rw-   0        0        0     2099 2023-06-27 16:34:37.000000 xiaobaisaf-2.3.3/saf/utils/YamlUtils.py
--rw-rw-rw-   0        0        0      201 2023-06-27 16:34:35.000000 xiaobaisaf-2.3.3/saf/utils/__init__.py
--rw-rw-rw-   0        0        0     3061 2023-06-27 16:34:38.000000 xiaobaisaf-2.3.3/saf/utils/downloadUtils.py
--rw-rw-rw-   0        0        0     1271 2023-06-27 16:34:36.000000 xiaobaisaf-2.3.3/saf/utils/elementUtils.py
--rw-rw-rw-   0        0        0      660 2023-06-27 16:34:36.000000 xiaobaisaf-2.3.3/saf/utils/imageUtils.py
--rw-rw-rw-   0        0        0     1369 2023-06-27 16:34:36.000000 xiaobaisaf-2.3.3/saf/utils/networkSpeedUtils.py
--rw-rw-rw-   0        0        0      132 2023-06-27 16:40:21.000000 xiaobaisaf-2.3.3/saf/utils/osEnvUtils.py
--rw-rw-rw-   0        0        0     8924 2023-06-27 16:34:37.000000 xiaobaisaf-2.3.3/saf/utils/selenium2POM.py
--rw-rw-rw-   0        0        0     2694 2023-06-27 16:34:36.000000 xiaobaisaf-2.3.3/saf/utils/sendMsgUtils.py
--rw-rw-rw-   0        0        0     2549 2023-06-30 17:16:51.000000 xiaobaisaf-2.3.3/saf/utils/xiaobaicmd.py
--rw-rw-rw-   0        0        0       42 2023-06-30 17:18:47.357668 xiaobaisaf-2.3.3/setup.cfg
--rw-rw-rw-   0        0        0     2450 2023-06-28 17:25:03.000000 xiaobaisaf-2.3.3/setup.py
-drwxrwxrwx   0        0        0        0 2023-06-30 17:18:47.356644 xiaobaisaf-2.3.3/xiaobaisaf.egg-info/
--rw-rw-rw-   0        0        0    11869 2023-06-30 17:18:47.000000 xiaobaisaf-2.3.3/xiaobaisaf.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1811 2023-06-30 17:18:47.000000 xiaobaisaf-2.3.3/xiaobaisaf.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-30 17:18:47.000000 xiaobaisaf-2.3.3/xiaobaisaf.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       57 2023-06-30 17:18:47.000000 xiaobaisaf-2.3.3/xiaobaisaf.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0      154 2023-06-30 17:18:47.000000 xiaobaisaf-2.3.3/xiaobaisaf.egg-info/requires.txt
--rw-rw-rw-   0        0        0        4 2023-06-30 17:18:47.000000 xiaobaisaf-2.3.3/xiaobaisaf.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-07-05 15:46:09.802691 xiaobaisaf-2.3.4/
+-rw-rw-rw-   0        0        0    35181 2023-06-27 16:34:34.000000 xiaobaisaf-2.3.4/LICENSE
+-rw-rw-rw-   0        0        0    11921 2023-07-05 15:46:09.802691 xiaobaisaf-2.3.4/PKG-INFO
+-rw-rw-rw-   0        0        0    11250 2023-07-05 15:45:45.000000 xiaobaisaf-2.3.4/README.md
+drwxrwxrwx   0        0        0        0 2023-07-05 15:46:09.525409 xiaobaisaf-2.3.4/saf/
+-rw-rw-rw-   0        0        0     1436 2023-06-27 16:40:21.000000 xiaobaisaf-2.3.4/saf/__init__.py
+-rw-rw-rw-   0        0        0      152 2023-07-05 15:45:45.000000 xiaobaisaf-2.3.4/saf/__version__.py
+drwxrwxrwx   0        0        0        0 2023-07-05 15:46:09.544359 xiaobaisaf-2.3.4/saf/data/
+-rw-rw-rw-   0        0        0      225 2023-06-27 16:34:35.000000 xiaobaisaf-2.3.4/saf/data/__init__.py
+-rw-rw-rw-   0        0        0     2943 2023-06-27 16:34:36.000000 xiaobaisaf-2.3.4/saf/data/config.py
+-rw-rw-rw-   0        0        0     4286 2023-06-27 16:34:38.000000 xiaobaisaf-2.3.4/saf/data/favicon.ico
+drwxrwxrwx   0        0        0        0 2023-07-05 15:46:09.552337 xiaobaisaf-2.3.4/saf/example/
+-rw-rw-rw-   0        0        0      100 2023-06-27 16:34:37.000000 xiaobaisaf-2.3.4/saf/example/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-05 15:46:09.576274 xiaobaisaf-2.3.4/saf/example/api/
+drwxrwxrwx   0        0        0        0 2023-07-05 15:46:09.590235 xiaobaisaf-2.3.4/saf/example/api/Config/
+-rw-rw-rw-   0        0        0      131 2023-06-27 16:34:37.000000 xiaobaisaf-2.3.4/saf/example/api/Config/__init__.py
+-rw-rw-rw-   0        0        0     5086 2023-06-27 16:34:37.000000 xiaobaisaf-2.3.4/saf/example/api/Config/config.py
+drwxrwxrwx   0        0        0        0 2023-07-05 15:46:09.597218 xiaobaisaf-2.3.4/saf/example/api/TestCases/
+-rw-rw-rw-   0        0        0      129 2023-06-27 16:34:37.000000 xiaobaisaf-2.3.4/saf/example/api/TestCases/__init__.py
+-rw-rw-rw-   0        0        0     1438 2023-06-27 16:34:37.000000 xiaobaisaf-2.3.4/saf/example/api/TestCases/test_one_html_case_template.py
+drwxrwxrwx   0        0        0        0 2023-07-05 15:46:09.630129 xiaobaisaf-2.3.4/saf/example/api/Utils/
+-rw-rw-rw-   0        0        0     1389 2023-06-28 15:26:03.000000 xiaobaisaf-2.3.4/saf/example/api/Utils/ExcelUtils.py
+-rw-rw-rw-   0        0        0     2099 2023-06-27 16:34:37.000000 xiaobaisaf-2.3.4/saf/example/api/Utils/YamlUtils.py
+-rw-rw-rw-   0        0        0      308 2023-06-27 16:34:37.000000 xiaobaisaf-2.3.4/saf/example/api/Utils/__init__.py
+-rw-rw-rw-   0        0        0     1111 2023-06-28 15:26:03.000000 xiaobaisaf-2.3.4/saf/example/api/Utils/api_client.py
+-rw-rw-rw-   0        0        0      285 2023-06-28 15:26:03.000000 xiaobaisaf-2.3.4/saf/example/api/Utils/logger.py
+-rw-rw-rw-   0        0        0      129 2023-06-27 16:34:37.000000 xiaobaisaf-2.3.4/saf/example/api/__init__.py
+-rw-rw-rw-   0        0        0     1211 2023-06-27 16:34:37.000000 xiaobaisaf-2.3.4/saf/example/api/run.py
+-rw-rw-rw-   0        0        0      549 2023-06-27 16:34:37.000000 xiaobaisaf-2.3.4/saf/example/api/send_email_script.py
+drwxrwxrwx   0        0        0        0 2023-07-05 15:46:09.636114 xiaobaisaf-2.3.4/saf/example/web/
+drwxrwxrwx   0        0        0        0 2023-07-05 15:46:09.676028 xiaobaisaf-2.3.4/saf/example/web/Cases/
+-rw-rw-rw-   0        0        0      140 2023-06-27 16:34:37.000000 xiaobaisaf-2.3.4/saf/example/web/Cases/__init__.py
+-rw-rw-rw-   0        0        0     2441 2023-06-27 16:34:37.000000 xiaobaisaf-2.3.4/saf/example/web/Cases/conftest.py
+-rw-rw-rw-   0        0        0      930 2023-06-27 16:34:37.000000 xiaobaisaf-2.3.4/saf/example/web/Cases/test_xiaobai_case_allure.py
+-rw-rw-rw-   0        0        0      962 2023-06-27 16:34:37.000000 xiaobaisaf-2.3.4/saf/example/web/Cases/test_xiaobai_case_submitBug.py
+-rw-rw-rw-   0        0        0      320 2023-06-27 16:34:37.000000 xiaobaisaf-2.3.4/saf/example/web/Cases/test_xiaobai_case_v1.py
+-rw-rw-rw-   0        0        0     1192 2023-06-27 16:34:37.000000 xiaobaisaf-2.3.4/saf/example/web/Cases/test_xiaobai_case_v2.py
+-rw-rw-rw-   0        0        0      228 2023-06-27 16:34:37.000000 xiaobaisaf-2.3.4/saf/example/web/Cases/test_xiaobai_case_v3.py
+drwxrwxrwx   0        0        0        0 2023-07-05 15:46:09.683010 xiaobaisaf-2.3.4/saf/example/web/Utils/
+-rw-rw-rw-   0        0        0     1389 2023-06-28 15:26:03.000000 xiaobaisaf-2.3.4/saf/example/web/Utils/ExcelUtils.py
+-rw-rw-rw-   0        0        0     2099 2023-06-28 15:26:03.000000 xiaobaisaf-2.3.4/saf/example/web/Utils/YamlUtils.py
+-rw-rw-rw-   0        0        0      308 2023-06-28 15:26:03.000000 xiaobaisaf-2.3.4/saf/example/web/Utils/__init__.py
+-rw-rw-rw-   0        0        0      285 2023-06-28 15:26:03.000000 xiaobaisaf-2.3.4/saf/example/web/Utils/logger.py
+-rw-rw-rw-   0        0        0      435 2023-06-27 16:34:37.000000 xiaobaisaf-2.3.4/saf/example/web/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-05 15:46:09.692983 xiaobaisaf-2.3.4/saf/example/web/pageObject/
+-rw-rw-rw-   0        0        0      166 2023-06-27 16:34:37.000000 xiaobaisaf-2.3.4/saf/example/web/pageObject/__init__.py
+-rw-rw-rw-   0        0        0      152 2023-06-27 16:34:37.000000 xiaobaisaf-2.3.4/saf/example/web/pageObject/register_page_element.py
+drwxrwxrwx   0        0        0        0 2023-07-05 15:46:09.785735 xiaobaisaf-2.3.4/saf/utils/
+-rw-rw-rw-   0        0        0     8132 2023-06-27 16:34:36.000000 xiaobaisaf-2.3.4/saf/utils/BugUtils.py
+-rw-rw-rw-   0        0        0      130 2023-07-05 15:07:02.000000 xiaobaisaf-2.3.4/saf/utils/Demo.py
+-rw-rw-rw-   0        0        0     2076 2023-06-27 16:40:34.000000 xiaobaisaf-2.3.4/saf/utils/MonitorAndroidDeviceGUI.py
+-rw-rw-rw-   0        0        0     8917 2023-06-27 16:34:38.000000 xiaobaisaf-2.3.4/saf/utils/MonitorAndroidPackageCLI.py
+-rw-rw-rw-   0        0        0    14196 2023-07-05 15:45:45.000000 xiaobaisaf-2.3.4/saf/utils/MonitorAndroidPackageGUI.py
+-rw-rw-rw-   0        0        0     7790 2023-06-30 17:18:46.000000 xiaobaisaf-2.3.4/saf/utils/MonitorAndroidPackagePower.py
+-rw-rw-rw-   0        0        0     1462 2023-07-05 15:11:29.000000 xiaobaisaf-2.3.4/saf/utils/MonitorCANBus.py
+-rw-rw-rw-   0        0        0     5933 2023-06-27 16:34:38.000000 xiaobaisaf-2.3.4/saf/utils/MonitorDBs.py
+-rw-rw-rw-   0        0        0     2099 2023-06-27 16:34:37.000000 xiaobaisaf-2.3.4/saf/utils/YamlUtils.py
+-rw-rw-rw-   0        0        0      201 2023-06-27 16:34:35.000000 xiaobaisaf-2.3.4/saf/utils/__init__.py
+-rw-rw-rw-   0        0        0     3061 2023-06-27 16:34:38.000000 xiaobaisaf-2.3.4/saf/utils/downloadUtils.py
+-rw-rw-rw-   0        0        0     1271 2023-06-27 16:34:36.000000 xiaobaisaf-2.3.4/saf/utils/elementUtils.py
+-rw-rw-rw-   0        0        0      660 2023-06-27 16:34:36.000000 xiaobaisaf-2.3.4/saf/utils/imageUtils.py
+-rw-rw-rw-   0        0        0     1369 2023-06-27 16:34:36.000000 xiaobaisaf-2.3.4/saf/utils/networkSpeedUtils.py
+-rw-rw-rw-   0        0        0      132 2023-06-27 16:40:21.000000 xiaobaisaf-2.3.4/saf/utils/osEnvUtils.py
+-rw-rw-rw-   0        0        0     8924 2023-06-27 16:34:37.000000 xiaobaisaf-2.3.4/saf/utils/selenium2POM.py
+-rw-rw-rw-   0        0        0     2694 2023-06-27 16:34:36.000000 xiaobaisaf-2.3.4/saf/utils/sendMsgUtils.py
+-rw-rw-rw-   0        0        0     2549 2023-06-30 17:16:51.000000 xiaobaisaf-2.3.4/saf/utils/xiaobaicmd.py
+-rw-rw-rw-   0        0        0       42 2023-07-05 15:46:09.802691 xiaobaisaf-2.3.4/setup.cfg
+-rw-rw-rw-   0        0        0     2450 2023-06-28 17:25:03.000000 xiaobaisaf-2.3.4/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-05 15:46:09.801693 xiaobaisaf-2.3.4/xiaobaisaf.egg-info/
+-rw-rw-rw-   0        0        0    11921 2023-07-05 15:46:09.000000 xiaobaisaf-2.3.4/xiaobaisaf.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1838 2023-07-05 15:46:09.000000 xiaobaisaf-2.3.4/xiaobaisaf.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-05 15:46:09.000000 xiaobaisaf-2.3.4/xiaobaisaf.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       57 2023-07-05 15:46:09.000000 xiaobaisaf-2.3.4/xiaobaisaf.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0      154 2023-07-05 15:46:09.000000 xiaobaisaf-2.3.4/xiaobaisaf.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        4 2023-07-05 15:46:09.000000 xiaobaisaf-2.3.4/xiaobaisaf.egg-info/top_level.txt
```

### Comparing `xiaobaisaf-2.3.3/LICENSE` & `xiaobaisaf-2.3.4/LICENSE`

 * *Files identical despite different names*

### Comparing `xiaobaisaf-2.3.3/PKG-INFO` & `xiaobaisaf-2.3.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: xiaobaisaf
-Version: 2.3.3
+Version: 2.3.4
 Summary: simple_automation_framework(简称：SAF)使用最简单的模式就可以实现需要功能和测试效果，也是xiaobaiauto2的简化版SAF继承了selenium、requests/httpx、appium、loguru、xiaobaiauto2、飞书机器人、钉钉机器人、企业微信机器人（暂时不支持）、禅道提单API
 Home-page: https://gitee.com/xiaobaikeji/simlpe_automation_framework
 Author: xiaobaiTser
 Author-email: 807447312@qq.com
 Keywords: saf test auto automation xiaobai xiaobaiauto2 test framework
 Requires-Python: >=3.6, <3.10
 Description-Content-Type: text/markdown
@@ -334,7 +334,8 @@
 | 2.0     | 新增xiaobaicmd -m命令        |
 | 2.1     | 新增xiaobaicmd --device命令  |
 | 2.2     | 优化xiaobaicmd --device命令  |
 | 2.3     | 新增实时监控Android设备耗电量       |
 | 2.3.1   | fix                      |
 | 2.3.2   | fix                      |
 | 2.3.3   | 新增实时监控Android当前APP的内存使用率 |
+| 2.3.4   | 优化xiaobaicmd -m gui效果展示  |
```

### Comparing `xiaobaisaf-2.3.3/README.md` & `xiaobaisaf-2.3.4/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -321,8 +321,9 @@
 | 1.9     | 新增xiaobaicmd -u命令        |
 | 2.0     | 新增xiaobaicmd -m命令        |
 | 2.1     | 新增xiaobaicmd --device命令  |
 | 2.2     | 优化xiaobaicmd --device命令  |
 | 2.3     | 新增实时监控Android设备耗电量       |
 | 2.3.1   | fix                      |
 | 2.3.2   | fix                      |
-| 2.3.3   | 新增实时监控Android当前APP的内存使用率 |
+| 2.3.3   | 新增实时监控Android当前APP的内存使用率 |
+| 2.3.4   | 优化xiaobaicmd -m gui效果展示  |
```

### Comparing `xiaobaisaf-2.3.3/saf/__init__.py` & `xiaobaisaf-2.3.4/saf/__init__.py`

 * *Files identical despite different names*

### Comparing `xiaobaisaf-2.3.3/saf/data/config.py` & `xiaobaisaf-2.3.4/saf/data/config.py`

 * *Files identical despite different names*

### Comparing `xiaobaisaf-2.3.3/saf/data/favicon.ico` & `xiaobaisaf-2.3.4/saf/data/favicon.ico`

 * *Files identical despite different names*

### Comparing `xiaobaisaf-2.3.3/saf/example/api/Config/config.py` & `xiaobaisaf-2.3.4/saf/example/api/Config/config.py`

 * *Files identical despite different names*

### Comparing `xiaobaisaf-2.3.3/saf/example/api/TestCases/test_one_html_case_template.py` & `xiaobaisaf-2.3.4/saf/example/api/TestCases/test_one_html_case_template.py`

 * *Files identical despite different names*

### Comparing `xiaobaisaf-2.3.3/saf/example/api/Utils/ExcelUtils.py` & `xiaobaisaf-2.3.4/saf/example/api/Utils/ExcelUtils.py`

 * *Files identical despite different names*

### Comparing `xiaobaisaf-2.3.3/saf/example/api/Utils/YamlUtils.py` & `xiaobaisaf-2.3.4/saf/example/api/Utils/YamlUtils.py`

 * *Files identical despite different names*

### Comparing `xiaobaisaf-2.3.3/saf/example/api/Utils/api_client.py` & `xiaobaisaf-2.3.4/saf/example/api/Utils/api_client.py`

 * *Files identical despite different names*

### Comparing `xiaobaisaf-2.3.3/saf/example/api/run.py` & `xiaobaisaf-2.3.4/saf/example/api/run.py`

 * *Files identical despite different names*

### Comparing `xiaobaisaf-2.3.3/saf/example/api/send_email_script.py` & `xiaobaisaf-2.3.4/saf/example/api/send_email_script.py`

 * *Files identical despite different names*

### Comparing `xiaobaisaf-2.3.3/saf/example/web/Cases/conftest.py` & `xiaobaisaf-2.3.4/saf/example/web/Cases/conftest.py`

 * *Files identical despite different names*

### Comparing `xiaobaisaf-2.3.3/saf/example/web/Cases/test_xiaobai_case_allure.py` & `xiaobaisaf-2.3.4/saf/example/web/Cases/test_xiaobai_case_allure.py`

 * *Files identical despite different names*

### Comparing `xiaobaisaf-2.3.3/saf/example/web/Cases/test_xiaobai_case_submitBug.py` & `xiaobaisaf-2.3.4/saf/example/web/Cases/test_xiaobai_case_submitBug.py`

 * *Files identical despite different names*

### Comparing `xiaobaisaf-2.3.3/saf/example/web/Cases/test_xiaobai_case_v2.py` & `xiaobaisaf-2.3.4/saf/example/web/Cases/test_xiaobai_case_v2.py`

 * *Files identical despite different names*

### Comparing `xiaobaisaf-2.3.3/saf/example/web/Utils/ExcelUtils.py` & `xiaobaisaf-2.3.4/saf/example/web/Utils/ExcelUtils.py`

 * *Files identical despite different names*

### Comparing `xiaobaisaf-2.3.3/saf/example/web/Utils/YamlUtils.py` & `xiaobaisaf-2.3.4/saf/example/web/Utils/YamlUtils.py`

 * *Files identical despite different names*

### Comparing `xiaobaisaf-2.3.3/saf/utils/BugUtils.py` & `xiaobaisaf-2.3.4/saf/utils/BugUtils.py`

 * *Files identical despite different names*

### Comparing `xiaobaisaf-2.3.3/saf/utils/MonitorAndroidDeviceGUI.py` & `xiaobaisaf-2.3.4/saf/utils/MonitorAndroidDeviceGUI.py`

 * *Files identical despite different names*

### Comparing `xiaobaisaf-2.3.3/saf/utils/MonitorAndroidPackageCLI.py` & `xiaobaisaf-2.3.4/saf/utils/MonitorAndroidPackageCLI.py`

 * *Files identical despite different names*

### Comparing `xiaobaisaf-2.3.3/saf/utils/MonitorAndroidPackageGUI.py` & `xiaobaisaf-2.3.4/saf/utils/MonitorAndroidPackageGUI.py`

 * *Files 4% similar despite different names*

```diff
@@ -54,14 +54,15 @@
         self.text_box.grid(row=2, column=1)
         self.text_box.insert('1.0', '开始点击你的APP界面吧!')
         self.scrollbar = tk.Scrollbar(self.master, command=self.text_box.yview)
         self.scrollbar.grid(row=2, column=2, sticky="nsew")
         self.text_box.config(yscrollcommand=self.scrollbar.set)
 
     def start_threads(self):
+
         # 启动线程
         self.device_thread = threading.Thread(target=self.update_device)
         self.device_thread.start()
         self.app_thread = threading.Thread(target=self.update_app)
         self.app_thread.start()
         self.text_thread = threading.Thread(target=self.update_text)
         self.text_thread.start()
@@ -156,72 +157,78 @@
         '''
         device = adb.device(device.serial)
         app = device.app_current()
         package_name = getattr(app, 'package')
         activity_name = getattr(app, 'activity')
         print(f'''#! /usr/bin/env python
 
-        from appium import webdriver
+from appium import webdriver
 
-        caps = {{
-            'automationName': 'UiAutomator2',
-            'platformName': 'Android',
-            'platformVersion': {device.shell(['getprop', 'ro.build.version.release']).strip()},
-            'deviceName': {device.serial},
-            'appPackage': {package_name},
-            'appActivity': {activity_name},
-            # 'noReset': True,
-            # 'dontStopAppOnReset': True,
-            'unicodeKeyboard': True,
-            'resetKeyboard': True
-        }}
+caps = {{
+    'automationName': 'UiAutomator2',
+    'platformName': 'Android',
+    'platformVersion': {device.shell(['getprop', 'ro.build.version.release']).strip()},
+    'deviceName': {device.serial},
+    'appPackage': {package_name},
+    'appActivity': {activity_name},
+    # 'noReset': True,
+    # 'allowClearUserData': 'true',
+    # 'fullReset': "false",
+    # 'exported': "true",
+    'unicodeKeyboard': True,
+    'resetKeyboard': True
+}}
 
-        app = webdriver.Remote("http://localhost:4723/wd/hub", caps)
+app = webdriver.Remote("http://127.0.0.1:4723/wd/hub", caps)
 
-        # 下面为定位表达式
+# 下面为定位表达式
         ''')
         deviceName = device.serial
         # 启动getevent命令
         event_cmd = f"adb -s {deviceName} shell getevent -lt /dev/input/event1"
         process = subprocess.Popen(event_cmd, stdout=subprocess.PIPE, shell=True)
         x = 0
         y = 0
         dx = copy.copy(x)
         dy = copy.copy(y)
         sj = ''
         status = [None, None]
         down_time = float(0)
+
+        device = adb.device(device.serial)
+        app = device.app_current()
+        package_name = getattr(app, 'package')
+        activity_name = getattr(app, 'activity')
+        code_header = "#! /usr/bin/env python\n" + \
+                      "\n" + \
+                      "from appium import webdriver\n" + \
+                      "\n" + \
+                      "caps = {\n" + \
+                      "\t'automationName': 'uiautomator2',\n" + \
+                      "\t'platformName': 'Android',\n" + \
+                      f"\t'platformVersion': '{device.shell(['getprop', 'ro.build.version.release']).strip()}',\n" + \
+                      f"\t'deviceName': '{device.serial}',\n" + \
+                      "\t# 'noReset': True,\n" + \
+                      "\t# 'allowClearUserData': 'true',\n" + \
+                      "\t# 'fullReset': \"false\",\n" + \
+                      "\t# 'exported': \"true\",\n" + \
+                      f"\t'appPackage': '{package_name}',\n" + \
+                      f"\t'appActivity': '{activity_name}',\n" + \
+                      "\t'unicodeKeyboard': True,\n" + \
+                      "\t'resetKeyboard': True\n" + \
+                      "}\n" + \
+                      "\n" + \
+                      "app = webdriver.Remote('http://127.0.0.1:4723/wd/hub', caps)\n" + \
+                      "\n" + \
+                      "# 以下内容为您当前触屏事件内容：\n"
+        self.text_box.delete('1.0', 'end')
+        self.text_box.insert('1.0', code_header)
+
         # 解析事件流
         while deviceName == device.serial:
-            device = adb.device(device.serial)
-            app = device.app_current()
-            package_name = getattr(app, 'package')
-            activity_name = getattr(app, 'activity')
-            code_header = "#! /usr/bin/env python\n" +\
-                        "\n" +\
-                        "from appium import webdriver\n" +\
-                        "\n" +\
-                        "caps = {\n" +\
-                            "\t'automationName': 'uiautomator2',\n" +\
-                            "\t'platformName': 'Android',\n" +\
-                            f"\t'platformVersion': '{device.shell(['getprop', 'ro.build.version.release']).strip()}',\n" +\
-                            f"\t'deviceName': '{device.serial}',\n" +\
-                            "\t# 'noReset': True,\n" +\
-                            "\t# 'allowClearUserData': 'true',\n" +\
-                            "\t# 'fullReset': \"false\",\n" +\
-                            "\t# 'exported': \"true\",\n" +\
-                            f"\t'appPackage': '{package_name}',\n" +\
-                            f"\t'appActivity': '{activity_name}',\n" +\
-                            "\t'unicodeKeyboard': True,\n" +\
-                            "\t'resetKeyboard': True\n" +\
-                        "}\n" +\
-                        "\n" +\
-                        "app = webdriver.Remote('http://127.0.0.1:4723/wd/hub', caps)\n" +\
-                        "\n" +\
-                        "# 以下内容为您当前触屏事件内容：\n"
             # 读取一行事件
             line = process.stdout.readline().decode().strip()
             # 获取x坐标
             if 'POSITION_X' in line:
                 parts = line.split()
                 x = int(parts[4], 16)
 
@@ -294,37 +301,37 @@
                             'appActivity': getattr(device.app_current, 'activity'),
                             'action': 'click',
                             'xpath': self.generate_xpath_with_attributes(elements[up_index]),
                             'bounds': [dx, dy, ux, uy],
                             'hold_time': hold_time
                         }
                         elif output_type == 'appium':
-                            sj = f'app.find_element(By.XPATH, value="{self.generate_xpath_with_attributes(elements[up_index])}").click()'
+                            sj = f'app.find_element(By.XPATH, value="{self.generate_xpath_with_attributes(elements[up_index])}").click()\n'
                         else:
-                            sj = '暂不支持此类型'
+                            sj = '暂不支持此类型\n'
                     else:
                         if output_type == 'data':
                             sj = {
                                 'platformName': 'Android',
                                 'platformVersion': device.shell(['getprop', 'ro.build.version.release']).strip(),
                                 'deviceName': device.serial,
                                 'appPackage': getattr(device.app_current, 'package'),
                                 'appActivity': getattr(device.app_current, 'activity'),
                                 'action': 'swipe',
                                 'xpath': None,
                                 'bounds': [dx, dy, ux, uy],
                                 'hold_time': hold_time
                             }
                         elif output_type == 'appium':
-                            sj = f'app.swipe({dx}, {dy}, {ux}, {uy}, {int(hold_time*1000)})'
+                            sj = f'app.swipe({dx}, {dy}, {ux}, {uy}, {int(hold_time*1000)})\n'
                         else:
-                            sj = '暂不支持此类型'
+                            sj = '暂不支持此类型\n'
                     status = [None, None]
-            self.text_box.delete('1.0', 'end')
-            self.text_box.insert('1.0', code_header+sj)
+                    line_count = int(self.text_box.index('end-1c').split('.')[0])
+                    self.text_box.insert(f'{line_count + 1}.0', sj)
             time.sleep(0.1)
         self.monitor_device(device=device.serial)
 
 def gui():
     root = tk.Tk()
     app = App(root)
     root.mainloop()
```

### Comparing `xiaobaisaf-2.3.3/saf/utils/MonitorAndroidPackagePower.py` & `xiaobaisaf-2.3.4/saf/utils/MonitorAndroidPackagePower.py`

 * *Files identical despite different names*

### Comparing `xiaobaisaf-2.3.3/saf/utils/MonitorDBs.py` & `xiaobaisaf-2.3.4/saf/utils/MonitorDBs.py`

 * *Files identical despite different names*

### Comparing `xiaobaisaf-2.3.3/saf/utils/YamlUtils.py` & `xiaobaisaf-2.3.4/saf/utils/YamlUtils.py`

 * *Files identical despite different names*

### Comparing `xiaobaisaf-2.3.3/saf/utils/downloadUtils.py` & `xiaobaisaf-2.3.4/saf/utils/downloadUtils.py`

 * *Files identical despite different names*

### Comparing `xiaobaisaf-2.3.3/saf/utils/elementUtils.py` & `xiaobaisaf-2.3.4/saf/utils/elementUtils.py`

 * *Files identical despite different names*

### Comparing `xiaobaisaf-2.3.3/saf/utils/imageUtils.py` & `xiaobaisaf-2.3.4/saf/utils/imageUtils.py`

 * *Files identical despite different names*

### Comparing `xiaobaisaf-2.3.3/saf/utils/networkSpeedUtils.py` & `xiaobaisaf-2.3.4/saf/utils/networkSpeedUtils.py`

 * *Files identical despite different names*

### Comparing `xiaobaisaf-2.3.3/saf/utils/selenium2POM.py` & `xiaobaisaf-2.3.4/saf/utils/selenium2POM.py`

 * *Files identical despite different names*

### Comparing `xiaobaisaf-2.3.3/saf/utils/sendMsgUtils.py` & `xiaobaisaf-2.3.4/saf/utils/sendMsgUtils.py`

 * *Files identical despite different names*

### Comparing `xiaobaisaf-2.3.3/saf/utils/xiaobaicmd.py` & `xiaobaisaf-2.3.4/saf/utils/xiaobaicmd.py`

 * *Files identical despite different names*

### Comparing `xiaobaisaf-2.3.3/setup.py` & `xiaobaisaf-2.3.4/setup.py`

 * *Files identical despite different names*

### Comparing `xiaobaisaf-2.3.3/xiaobaisaf.egg-info/PKG-INFO` & `xiaobaisaf-2.3.4/xiaobaisaf.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: xiaobaisaf
-Version: 2.3.3
+Version: 2.3.4
 Summary: simple_automation_framework(简称：SAF)使用最简单的模式就可以实现需要功能和测试效果，也是xiaobaiauto2的简化版SAF继承了selenium、requests/httpx、appium、loguru、xiaobaiauto2、飞书机器人、钉钉机器人、企业微信机器人（暂时不支持）、禅道提单API
 Home-page: https://gitee.com/xiaobaikeji/simlpe_automation_framework
 Author: xiaobaiTser
 Author-email: 807447312@qq.com
 Keywords: saf test auto automation xiaobai xiaobaiauto2 test framework
 Requires-Python: >=3.6, <3.10
 Description-Content-Type: text/markdown
@@ -334,7 +334,8 @@
 | 2.0     | 新增xiaobaicmd -m命令        |
 | 2.1     | 新增xiaobaicmd --device命令  |
 | 2.2     | 优化xiaobaicmd --device命令  |
 | 2.3     | 新增实时监控Android设备耗电量       |
 | 2.3.1   | fix                      |
 | 2.3.2   | fix                      |
 | 2.3.3   | 新增实时监控Android当前APP的内存使用率 |
+| 2.3.4   | 优化xiaobaicmd -m gui效果展示  |
```

### Comparing `xiaobaisaf-2.3.3/xiaobaisaf.egg-info/SOURCES.txt` & `xiaobaisaf-2.3.4/xiaobaisaf.egg-info/SOURCES.txt`

 * *Files 0% similar despite different names*

```diff
@@ -35,14 +35,15 @@
 saf/example/web/pageObject/register_page_element.py
 saf/utils/BugUtils.py
 saf/utils/Demo.py
 saf/utils/MonitorAndroidDeviceGUI.py
 saf/utils/MonitorAndroidPackageCLI.py
 saf/utils/MonitorAndroidPackageGUI.py
 saf/utils/MonitorAndroidPackagePower.py
+saf/utils/MonitorCANBus.py
 saf/utils/MonitorDBs.py
 saf/utils/YamlUtils.py
 saf/utils/__init__.py
 saf/utils/downloadUtils.py
 saf/utils/elementUtils.py
 saf/utils/imageUtils.py
 saf/utils/networkSpeedUtils.py
```

