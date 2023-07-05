# Comparing `tmp/inhandtest-0.0.58.tar.gz` & `tmp/inhandtest-0.0.59.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\inhandtest-0.0.58.tar", last modified: Mon Jul  3 10:26:48 2023, max compression
+gzip compressed data, was "dist\inhandtest-0.0.59.tar", last modified: Wed Jul  5 03:14:22 2023, max compression
```

## Comparing `inhandtest-0.0.58.tar` & `inhandtest-0.0.59.tar`

### file list

```diff
@@ -1,61 +1,61 @@
-drwxrwxrwx   0        0        0        0 2023-07-03 10:26:48.000000 inhandtest-0.0.58/
--rw-rw-rw-   0        0        0       81 2023-04-13 01:59:22.000000 inhandtest-0.0.58/MANIFEST.in
--rw-rw-rw-   0        0        0      593 2023-07-03 10:26:48.000000 inhandtest-0.0.58/PKG-INFO
--rw-rw-rw-   0        0        0    12238 2023-02-27 03:43:37.000000 inhandtest-0.0.58/README.md
-drwxrwxrwx   0        0        0        0 2023-07-03 10:26:48.000000 inhandtest-0.0.58/inhandtest/
--rw-rw-rw-   0        0        0        0 2023-01-31 08:41:58.000000 inhandtest-0.0.58/inhandtest/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-03 10:26:48.000000 inhandtest-0.0.58/inhandtest/base_page/
--rw-rw-rw-   0        0        0      330 2023-05-31 07:35:39.000000 inhandtest-0.0.58/inhandtest/base_page/__init__.py
--rw-rw-rw-   0        0        0    43260 2023-07-03 08:13:32.000000 inhandtest-0.0.58/inhandtest/base_page/_ig_contents_locators.py
--rw-rw-rw-   0        0        0    27868 2023-05-17 02:51:06.000000 inhandtest-0.0.58/inhandtest/base_page/_ir3XX_contents_locators.py
--rw-rw-rw-   0        0        0    64964 2023-05-11 07:07:35.000000 inhandtest-0.0.58/inhandtest/base_page/_vg710_contents_locators.py
--rw-rw-rw-   0        0        0    64740 2023-06-29 08:46:46.000000 inhandtest-0.0.58/inhandtest/base_page/base_page.py
--rw-rw-rw-   0        0        0    25320 2023-06-29 01:54:01.000000 inhandtest-0.0.58/inhandtest/base_page/table_tr.py
--rw-rw-rw-   0        0        0      608 2023-03-31 07:18:06.000000 inhandtest-0.0.58/inhandtest/exception.py
--rw-rw-rw-   0        0        0     3971 2023-06-16 00:48:06.000000 inhandtest-0.0.58/inhandtest/file.py
--rw-rw-rw-   0        0        0    10907 2023-06-15 06:06:07.000000 inhandtest-0.0.58/inhandtest/inmodbus.py
--rw-rw-rw-   0        0        0     4451 2023-06-15 05:47:54.000000 inhandtest-0.0.58/inhandtest/inmongodb.py
--rw-rw-rw-   0        0        0    22542 2023-07-03 10:18:22.000000 inhandtest-0.0.58/inhandtest/inmqtt.py
--rw-rw-rw-   0        0        0    71861 2023-07-03 01:50:04.000000 inhandtest-0.0.58/inhandtest/inrequest.py
--rw-rw-rw-   0        0        0     8389 2023-07-03 08:50:33.000000 inhandtest-0.0.58/inhandtest/inserial.py
--rw-rw-rw-   0        0        0    14831 2023-07-03 08:50:33.000000 inhandtest-0.0.58/inhandtest/insocket.py
--rw-rw-rw-   0        0        0     8481 2023-06-15 06:12:16.000000 inhandtest-0.0.58/inhandtest/inssh.py
--rw-rw-rw-   0        0        0     1569 2023-05-24 09:45:24.000000 inhandtest-0.0.58/inhandtest/ip.py
--rw-rw-rw-   0        0        0     1390 2023-06-15 09:39:25.000000 inhandtest-0.0.58/inhandtest/log.py
--rw-rw-rw-   0        0        0    13757 2023-06-15 05:47:54.000000 inhandtest-0.0.58/inhandtest/mail.py
--rw-rw-rw-   0        0        0      387 2023-06-12 09:08:02.000000 inhandtest-0.0.58/inhandtest/notice_email.html
-drwxrwxrwx   0        0        0        0 2023-07-03 10:26:48.000000 inhandtest-0.0.58/inhandtest/pages/
--rw-rw-rw-   0        0        0      230 2023-05-31 07:29:45.000000 inhandtest-0.0.58/inhandtest/pages/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-03 10:26:48.000000 inhandtest-0.0.58/inhandtest/pages/ingateway/
--rw-rw-rw-   0        0        0      136 2023-05-31 07:30:00.000000 inhandtest-0.0.58/inhandtest/pages/ingateway/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-03 10:26:48.000000 inhandtest-0.0.58/inhandtest/pages/ingateway/edge_computing/
--rw-rw-rw-   0        0        0      134 2023-05-25 07:33:25.000000 inhandtest-0.0.58/inhandtest/pages/ingateway/edge_computing/__init__.py
--rw-rw-rw-   0        0        0    63438 2023-07-03 08:16:21.000000 inhandtest-0.0.58/inhandtest/pages/ingateway/edge_computing/edge_computing_locators.py
--rw-rw-rw-   0        0        0    65044 2023-07-03 07:08:34.000000 inhandtest-0.0.58/inhandtest/pages/ingateway/edge_computing/python_edge_computing.py
--rw-rw-rw-   0        0        0     3195 2023-06-30 06:11:59.000000 inhandtest-0.0.58/inhandtest/pages/ingateway/ingateway.py
--rw-rw-rw-   0        0        0    11128 2023-06-30 03:20:05.000000 inhandtest-0.0.58/inhandtest/pages/ingateway/locale.yml
--rw-rw-rw-   0        0        0      911 2023-06-02 06:30:38.000000 inhandtest-0.0.58/inhandtest/pages/ingateway/locators.py
-drwxrwxrwx   0        0        0        0 2023-07-03 10:26:48.000000 inhandtest-0.0.58/inhandtest/pages/ingateway/network/
--rw-rw-rw-   0        0        0      134 2023-05-15 07:33:50.000000 inhandtest-0.0.58/inhandtest/pages/ingateway/network/__init__.py
--rw-rw-rw-   0        0        0    67807 2023-06-26 05:24:31.000000 inhandtest-0.0.58/inhandtest/pages/ingateway/network/network.py
--rw-rw-rw-   0        0        0    86201 2023-06-26 05:24:31.000000 inhandtest-0.0.58/inhandtest/pages/ingateway/network/network_locators.py
-drwxrwxrwx   0        0        0        0 2023-07-03 10:26:48.000000 inhandtest-0.0.58/inhandtest/pages/ingateway/overview/
--rw-rw-rw-   0        0        0      134 2023-05-15 07:33:50.000000 inhandtest-0.0.58/inhandtest/pages/ingateway/overview/__init__.py
--rw-rw-rw-   0        0        0     6953 2023-06-02 09:29:07.000000 inhandtest-0.0.58/inhandtest/pages/ingateway/overview/overview.py
--rw-rw-rw-   0        0        0     6260 2023-05-18 07:02:23.000000 inhandtest-0.0.58/inhandtest/pages/ingateway/overview/overview_locators.py
-drwxrwxrwx   0        0        0        0 2023-07-03 10:26:48.000000 inhandtest-0.0.58/inhandtest/pages/ingateway/system/
--rw-rw-rw-   0        0        0      133 2023-06-02 06:29:57.000000 inhandtest-0.0.58/inhandtest/pages/ingateway/system/__init__.py
--rw-rw-rw-   0        0        0    28514 2023-06-26 05:24:31.000000 inhandtest-0.0.58/inhandtest/pages/ingateway/system/system.py
--rw-rw-rw-   0        0        0    30656 2023-06-26 05:24:31.000000 inhandtest-0.0.58/inhandtest/pages/ingateway/system/system_locators.py
--rw-rw-rw-   0        0        0     1224 2023-04-28 06:53:30.000000 inhandtest-0.0.58/inhandtest/pytest_email.html
--rw-rw-rw-   0        0        0    34699 2023-06-20 09:30:58.000000 inhandtest-0.0.58/inhandtest/telnet.py
--rw-rw-rw-   0        0        0    28118 2023-07-03 02:25:51.000000 inhandtest-0.0.58/inhandtest/tools.py
-drwxrwxrwx   0        0        0        0 2023-07-03 10:26:48.000000 inhandtest-0.0.58/inhandtest.egg-info/
--rw-rw-rw-   0        0        0      593 2023-07-03 10:26:48.000000 inhandtest-0.0.58/inhandtest.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1656 2023-07-03 10:26:48.000000 inhandtest-0.0.58/inhandtest.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-03 10:26:48.000000 inhandtest-0.0.58/inhandtest.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      123 2023-07-03 10:26:48.000000 inhandtest-0.0.58/inhandtest.egg-info/requires.txt
--rw-rw-rw-   0        0        0       11 2023-07-03 10:26:48.000000 inhandtest-0.0.58/inhandtest.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      147 2023-06-01 10:06:41.000000 inhandtest-0.0.58/requirements.txt
--rw-rw-rw-   0        0        0       42 2023-07-03 10:26:48.000000 inhandtest-0.0.58/setup.cfg
--rw-rw-rw-   0        0        0     1615 2023-07-03 10:26:35.000000 inhandtest-0.0.58/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-05 03:14:22.000000 inhandtest-0.0.59/
+-rw-rw-rw-   0        0        0       81 2023-04-13 01:59:22.000000 inhandtest-0.0.59/MANIFEST.in
+-rw-rw-rw-   0        0        0      593 2023-07-05 03:14:22.000000 inhandtest-0.0.59/PKG-INFO
+-rw-rw-rw-   0        0        0    12238 2023-02-27 03:43:37.000000 inhandtest-0.0.59/README.md
+drwxrwxrwx   0        0        0        0 2023-07-05 03:14:22.000000 inhandtest-0.0.59/inhandtest/
+-rw-rw-rw-   0        0        0        0 2023-01-31 08:41:58.000000 inhandtest-0.0.59/inhandtest/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-05 03:14:22.000000 inhandtest-0.0.59/inhandtest/base_page/
+-rw-rw-rw-   0        0        0      330 2023-05-31 07:35:39.000000 inhandtest-0.0.59/inhandtest/base_page/__init__.py
+-rw-rw-rw-   0        0        0    43260 2023-07-03 08:13:32.000000 inhandtest-0.0.59/inhandtest/base_page/_ig_contents_locators.py
+-rw-rw-rw-   0        0        0    27868 2023-05-17 02:51:06.000000 inhandtest-0.0.59/inhandtest/base_page/_ir3XX_contents_locators.py
+-rw-rw-rw-   0        0        0    64964 2023-05-11 07:07:35.000000 inhandtest-0.0.59/inhandtest/base_page/_vg710_contents_locators.py
+-rw-rw-rw-   0        0        0    64382 2023-07-05 03:09:48.000000 inhandtest-0.0.59/inhandtest/base_page/base_page.py
+-rw-rw-rw-   0        0        0    26127 2023-07-05 03:02:01.000000 inhandtest-0.0.59/inhandtest/base_page/table_tr.py
+-rw-rw-rw-   0        0        0      608 2023-03-31 07:18:06.000000 inhandtest-0.0.59/inhandtest/exception.py
+-rw-rw-rw-   0        0        0     3971 2023-06-16 00:48:06.000000 inhandtest-0.0.59/inhandtest/file.py
+-rw-rw-rw-   0        0        0    10907 2023-06-15 06:06:07.000000 inhandtest-0.0.59/inhandtest/inmodbus.py
+-rw-rw-rw-   0        0        0     4451 2023-06-15 05:47:54.000000 inhandtest-0.0.59/inhandtest/inmongodb.py
+-rw-rw-rw-   0        0        0    22542 2023-07-03 10:18:22.000000 inhandtest-0.0.59/inhandtest/inmqtt.py
+-rw-rw-rw-   0        0        0    71861 2023-07-03 01:50:04.000000 inhandtest-0.0.59/inhandtest/inrequest.py
+-rw-rw-rw-   0        0        0     8389 2023-07-03 08:50:33.000000 inhandtest-0.0.59/inhandtest/inserial.py
+-rw-rw-rw-   0        0        0    14831 2023-07-03 08:50:33.000000 inhandtest-0.0.59/inhandtest/insocket.py
+-rw-rw-rw-   0        0        0     8481 2023-06-15 06:12:16.000000 inhandtest-0.0.59/inhandtest/inssh.py
+-rw-rw-rw-   0        0        0     1569 2023-05-24 09:45:24.000000 inhandtest-0.0.59/inhandtest/ip.py
+-rw-rw-rw-   0        0        0     1390 2023-06-15 09:39:25.000000 inhandtest-0.0.59/inhandtest/log.py
+-rw-rw-rw-   0        0        0    13757 2023-06-15 05:47:54.000000 inhandtest-0.0.59/inhandtest/mail.py
+-rw-rw-rw-   0        0        0      387 2023-06-12 09:08:02.000000 inhandtest-0.0.59/inhandtest/notice_email.html
+drwxrwxrwx   0        0        0        0 2023-07-05 03:14:22.000000 inhandtest-0.0.59/inhandtest/pages/
+-rw-rw-rw-   0        0        0      230 2023-05-31 07:29:45.000000 inhandtest-0.0.59/inhandtest/pages/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-05 03:14:22.000000 inhandtest-0.0.59/inhandtest/pages/ingateway/
+-rw-rw-rw-   0        0        0      136 2023-05-31 07:30:00.000000 inhandtest-0.0.59/inhandtest/pages/ingateway/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-05 03:14:22.000000 inhandtest-0.0.59/inhandtest/pages/ingateway/edge_computing/
+-rw-rw-rw-   0        0        0      134 2023-05-25 07:33:25.000000 inhandtest-0.0.59/inhandtest/pages/ingateway/edge_computing/__init__.py
+-rw-rw-rw-   0        0        0    67491 2023-07-05 02:30:31.000000 inhandtest-0.0.59/inhandtest/pages/ingateway/edge_computing/edge_computing_locators.py
+-rw-rw-rw-   0        0        0    71995 2023-07-05 02:31:02.000000 inhandtest-0.0.59/inhandtest/pages/ingateway/edge_computing/python_edge_computing.py
+-rw-rw-rw-   0        0        0     3247 2023-07-05 03:12:45.000000 inhandtest-0.0.59/inhandtest/pages/ingateway/ingateway.py
+-rw-rw-rw-   0        0        0    11890 2023-07-05 02:55:07.000000 inhandtest-0.0.59/inhandtest/pages/ingateway/locale.yml
+-rw-rw-rw-   0        0        0      911 2023-06-02 06:30:38.000000 inhandtest-0.0.59/inhandtest/pages/ingateway/locators.py
+drwxrwxrwx   0        0        0        0 2023-07-05 03:14:22.000000 inhandtest-0.0.59/inhandtest/pages/ingateway/network/
+-rw-rw-rw-   0        0        0      134 2023-05-15 07:33:50.000000 inhandtest-0.0.59/inhandtest/pages/ingateway/network/__init__.py
+-rw-rw-rw-   0        0        0    68039 2023-07-05 01:05:37.000000 inhandtest-0.0.59/inhandtest/pages/ingateway/network/network.py
+-rw-rw-rw-   0        0        0    86226 2023-07-05 01:05:03.000000 inhandtest-0.0.59/inhandtest/pages/ingateway/network/network_locators.py
+drwxrwxrwx   0        0        0        0 2023-07-05 03:14:22.000000 inhandtest-0.0.59/inhandtest/pages/ingateway/overview/
+-rw-rw-rw-   0        0        0      134 2023-05-15 07:33:50.000000 inhandtest-0.0.59/inhandtest/pages/ingateway/overview/__init__.py
+-rw-rw-rw-   0        0        0     6953 2023-06-02 09:29:07.000000 inhandtest-0.0.59/inhandtest/pages/ingateway/overview/overview.py
+-rw-rw-rw-   0        0        0     6260 2023-05-18 07:02:23.000000 inhandtest-0.0.59/inhandtest/pages/ingateway/overview/overview_locators.py
+drwxrwxrwx   0        0        0        0 2023-07-05 03:14:22.000000 inhandtest-0.0.59/inhandtest/pages/ingateway/system/
+-rw-rw-rw-   0        0        0      133 2023-06-02 06:29:57.000000 inhandtest-0.0.59/inhandtest/pages/ingateway/system/__init__.py
+-rw-rw-rw-   0        0        0    28514 2023-06-26 05:24:31.000000 inhandtest-0.0.59/inhandtest/pages/ingateway/system/system.py
+-rw-rw-rw-   0        0        0    30656 2023-06-26 05:24:31.000000 inhandtest-0.0.59/inhandtest/pages/ingateway/system/system_locators.py
+-rw-rw-rw-   0        0        0     1224 2023-04-28 06:53:30.000000 inhandtest-0.0.59/inhandtest/pytest_email.html
+-rw-rw-rw-   0        0        0    34699 2023-06-20 09:30:58.000000 inhandtest-0.0.59/inhandtest/telnet.py
+-rw-rw-rw-   0        0        0    28122 2023-07-03 10:41:33.000000 inhandtest-0.0.59/inhandtest/tools.py
+drwxrwxrwx   0        0        0        0 2023-07-05 03:14:22.000000 inhandtest-0.0.59/inhandtest.egg-info/
+-rw-rw-rw-   0        0        0      593 2023-07-05 03:14:22.000000 inhandtest-0.0.59/inhandtest.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1656 2023-07-05 03:14:22.000000 inhandtest-0.0.59/inhandtest.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-05 03:14:22.000000 inhandtest-0.0.59/inhandtest.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      123 2023-07-05 03:14:22.000000 inhandtest-0.0.59/inhandtest.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       11 2023-07-05 03:14:22.000000 inhandtest-0.0.59/inhandtest.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      147 2023-06-01 10:06:41.000000 inhandtest-0.0.59/requirements.txt
+-rw-rw-rw-   0        0        0       42 2023-07-05 03:14:22.000000 inhandtest-0.0.59/setup.cfg
+-rw-rw-rw-   0        0        0     1615 2023-07-05 03:14:12.000000 inhandtest-0.0.59/setup.py
```

### Comparing `inhandtest-0.0.58/PKG-INFO` & `inhandtest-0.0.59/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.2
 Name: inhandtest
-Version: 0.0.58
+Version: 0.0.59
 Summary: inhand test tools, so easy
 Home-page: https://inhandnetworks.yuque.com/irhb08/mrpu1r/qgu0imvigkm2xry9?singleDoc# 《inhandtest docs》
 Author: liwei
 Author-email: liwei@inhand.com.cn
 Maintainer: liwei
 Maintainer-email: liwei@inhand.com.cn
 License: UNKNOWN
```

### Comparing `inhandtest-0.0.58/README.md` & `inhandtest-0.0.59/README.md`

 * *Files identical despite different names*

### Comparing `inhandtest-0.0.58/inhandtest/base_page/_ig_contents_locators.py` & `inhandtest-0.0.59/inhandtest/base_page/_ig_contents_locators.py`

 * *Files identical despite different names*

### Comparing `inhandtest-0.0.58/inhandtest/base_page/_ir3XX_contents_locators.py` & `inhandtest-0.0.59/inhandtest/base_page/_ir3XX_contents_locators.py`

 * *Files identical despite different names*

### Comparing `inhandtest-0.0.58/inhandtest/base_page/_vg710_contents_locators.py` & `inhandtest-0.0.59/inhandtest/base_page/_vg710_contents_locators.py`

 * *Files identical despite different names*

### Comparing `inhandtest-0.0.58/inhandtest/base_page/base_page.py` & `inhandtest-0.0.59/inhandtest/base_page/base_page.py`

 * *Files 1% similar despite different names*

```diff
@@ -35,23 +35,25 @@
         :param protocol: 协议
         :param port: 端口
         :param model: 'VG710'|'ER805'|'ER605'|'IR302'|'IG502'|'IG902'|'IR305'|'IR615'
         :param page: 当page为None时，自动打开浏览器及页面，否则使用传入的page
         :param kwargs:
                       browser: 当没有传入page时，可以选择浏览器
                       locale: dict 国际化
+                      bring_to_front: bool 是否将浏览器窗口置顶
         """
         self.page = page
         self.host = host
         self.model = model.upper()
         self.protocol = protocol
         self.port = port
         self.username = username
         self.password = password
         self.language = language
+        self.bring_to_front = kwargs.get('bring_to_front', False)
         self.__browser_type = kwargs.get('browser')
         self.__http_credentials_model = ('VG710',)  # 需要使用http认证的设备, 没有登录页面 只有登录弹窗
         if self.page is None:
             self.__new_page()
         if self.model == 'VG710':
             self.content_locator = VGContentsLocators(self.page, language).tags_menu
         elif self.model in ('IG902', 'IG502'):
@@ -128,15 +130,16 @@
         def goto_router():
             device = "{}://{}:{}".format(self.protocol, self.host, self.port)
             try:
                 self.page.goto(device, timeout=120 * 1000)
             except Exception:
                 logging.exception(f'Open {self.host} device address {device} timeout')
                 raise
-            self.page.bring_to_front()
+            if self.bring_to_front:
+                self.page.bring_to_front()
             self.page.wait_for_timeout(500)
             if self.model in self.__http_credentials_model:
                 logging.info(f'Open {self.host} device address {device} and login')
             else:
                 logging.info(f'Open {self.host} device address {device}')
 
         def _login():
@@ -267,15 +270,16 @@
             for menu_old_ in menu_old_s:
                 locators = locators.get(menu_old_)
             default = locators.get('default')
             menu_new = menu_old + '.' + default if default else menu_old
             return menu_new
 
         if menu:
-            self.page.bring_to_front()
+            if self.bring_to_front:
+                self.page.bring_to_front()
             self.login()
             try:
                 menu = menu.replace(' ', '_').replace('-', '_').lower()
                 menu = default_change(menu, self.content_locator).split('.')
                 access(menu)
             except Exception:
                 logging.exception(f'not support this menu {menu}')
@@ -298,41 +302,50 @@
             locator.clear()
             locator.fill(str(value), force=force)
             locator.blur()  # 鼠标移出输入框
             if log_desc:
                 logging.info(f'Device {self.host} fill {log_desc} {value}')
 
     @allure.step('点击按钮')
-    def click(self, locator: Locator, log_desc=None, dialog_message: str = None, tip_messages: str or list = None,
-              wait_for_time: int = None, tip_messages_timeout=30) -> None:
-        """ 封装公共的点击操作
+    def click(self, locator: Locator or list or tuple, log_desc=None, dialog_message: str = None,
+              tip_messages: str or list = None, wait_for_time: int = None, tip_messages_timeout=30) -> None:
+        """ 封装公共的点击操作 支持多个元素点击, 对点击最后一次的属性做校验
 
         :param locator:  元素定位
         :param log_desc: 功能描述，用英文 如 Static Routing Destination
-        :param dialog_message: str  点击按钮后有dialog弹出，并且期望对信息做验证， 支持模糊匹配
+        :param dialog_message: str  点击按钮后有dialog弹出，并且期望对信息做验证， 支持模糊匹配, 点击最后一个元素
         :param tip_messages: str or list 点击后等待该tip出现 再等待tip消失，如果有多个，使用列表传入
                             tip_messages 是支持模糊匹配
-                            该项校验 页面元素必须停留时间1秒及更多时间，否则不容易检测到导致报错
-        :param wait_for_time: ms  当做完所有操作后是否需要等待时间
+                            该项校验 页面元素必须停留时间1秒及更多时间，否则不容易检测到导致报错， 点击最后一个元素
+        :param wait_for_time: ms  当做完所有操作后是否需要等待时间， 点击最后一个元素
         :param tip_messages_timeout: 默认30秒， 单位秒
         :return:
         """
-
-        if not locator.is_disabled():
-            if dialog_message:
-                self.dialog_massage(locator.click, dialog_message)
-            else:
-                locator.click()
-            if log_desc:
-                logging.info(f'Device {self.host} click {log_desc}')
-            self.tip_messages(tip_messages, tip_messages_timeout)
-            if wait_for_time:
-                self.page.wait_for_timeout(wait_for_time)
+        def last_click(last_locator: Locator):
+            if not last_locator.is_disabled():
+                if dialog_message:
+                    self.dialog_massage(last_locator.click, dialog_message)
+                else:
+                    last_locator.click()
+                if log_desc:
+                    logging.info(f'Device {self.host} click {log_desc}')
+                self.tip_messages(tip_messages, tip_messages_timeout)
+                if wait_for_time:
+                    self.page.wait_for_timeout(wait_for_time)
+            else:
+                logging.warning(f'Device {self.host} click {log_desc} is disabled')
+        if isinstance(locator, (tuple, list)):
+            for locator_ in locator[:-1]:
+                locator_.click()
+            last_click(locator[-1])
+        elif isinstance(locator, Locator):
+            last_click(locator)
         else:
-            logging.warning(f'Device {self.host} click {log_desc} is disabled')
+            logging.exception(f'locator type error {locator}')
+            raise TypeError(f'locator type error {locator}')
 
     @allure.step('勾选框')
     def check(self, locator: Locator, action='check', log_desc=None, tip_messages: str or list = None) -> None:
         """ 封装公共的单选操作
         :param locator:  元素定位
         :param log_desc: 功能描述，用英文 如 Static Routing Destination
         :param action: 'check'|'uncheck'| None | '是' | 'Yes'
@@ -865,23 +878,21 @@
 
         def operation(param, param_locator, value):
             if param_locator.get('type') == 'text':
                 self.fill(param_locator.get('locator'), value, param)
             elif param_locator.get('type') == 'monaco':
                 self.monaco(param_locator.get('locator'), value, param)
             elif param_locator.get('type') == 'select':
-                if param_locator.get('param') and value in param_locator.get('param').keys():
-                    value = param_locator.get('param').get(value)
+                value = replace_str(value, param_locator.get('param'))
                 self.select_option(param_locator.get('locator'), value, param)
             elif param_locator.get('type') == 'select_more':
                 value = replace_str(value, param_locator.get('param'))
                 self.select_more(param_locator.get('locator'), value, param)
             elif param_locator.get('type') == 'select_multi':
-                if param_locator.get('param') and value in param_locator.get('param').keys():
-                    value = param_locator.get('param').get(value)
+                value = replace_str(value, param_locator.get('param'))
                 self.select_multi(param_locator.get('locator'), value, param)
             elif param_locator.get('type') == 'radio_select':
                 if param_locator.get('param') and value in param_locator.get('param').keys():
                     value = param_locator.get('param').get(value)
                 self.radio_select(param_locator.get('locator'), value, param)
             elif param_locator.get('type') == 'radio':
                 if param_locator.get('param') and value in param_locator.get('param').keys():
@@ -896,30 +907,16 @@
                     dialog_message, tip_messages, wait_for_time, tip_messages_timeout = None, None, None, 30
                     if isinstance(value, dict):
                         dialog_message = value.get('dialog_message')
                         tip_messages = value.get('tip_messages')
                         wait_for_time = value.get('wait_for_time')
                         tip_messages_timeout = value.get('tip_messages_timeout') if value.get(
                             'tip_messages_timeout') is not None else 30
-                    if isinstance(param_locator.get('locator'), Locator):
-                        self.click(param_locator.get('locator'), param, dialog_message, tip_messages, wait_for_time,
-                                   tip_messages_timeout)
-                    elif isinstance(param_locator.get('locator'), list) or isinstance(param_locator.get('locator'),
-                                                                                      tuple):  # 二次确认
-                        self.click(param_locator.get('locator')[0], param, dialog_message)
-                        try:
-                            param_locator.get('locator')[1].click(timeout=1 * 1000)
-                        except TimeoutError:
-                            pass
-                        self.tip_messages(tip_messages, tip_messages_timeout)
-                        if wait_for_time:
-                            self.page.wait_for_timeout(wait_for_time)
-                    else:
-                        logging.exception(f'locator {param_locator.get("locator")} is not a Locator or list or tuple')
-                        raise Exception(f'locator {param_locator.get("locator")} is not a Locator or list or tuple')
+                    self.click(param_locator.get('locator'), param, dialog_message, tip_messages, wait_for_time,
+                               tip_messages_timeout)
             elif param_locator.get('type') == 'check':
                 if value:
                     value_, tip_messages = value, None
                     if isinstance(value, dict):
                         value_ = value.get('value')
                         tip_messages = value.get('tip_messages')
                     self.check(param_locator.get('locator'), value_, param, tip_messages)
```

### Comparing `inhandtest-0.0.58/inhandtest/base_page/table_tr.py` & `inhandtest-0.0.59/inhandtest/base_page/table_tr.py`

 * *Files 2% similar despite different names*

```diff
@@ -292,23 +292,38 @@
             add_button = list(filter(lambda x: x[0] == 'add', self.columns))[0][1].get('locator')
         except Exception:
             add_button = self.table_locator.locator('//button').first
         if kwargs.get('is_exists'):
             is_exists = kwargs.pop('is_exists')
             if not self.exist(is_exists, self.locale):
                 add_button.click()
-                agg_in(self.columns, kwargs)
-                logging.debug(f'table resource {kwargs} add success')
+                if not kwargs.get('cancel'):
+                    agg_in(self.columns, kwargs)
+                    logging.debug(f'table resource {kwargs} add success')
+                else:
+                    try:
+                        agg_in(self.columns, kwargs)
+                    except Exception:
+                        raise
+                    finally:
+                        agg_in(self.columns, {'cancel': True})
             else:
                 logging.debug(f'table resource {kwargs} exist')
         else:
             add_button.click()
-            agg_in(self.columns, kwargs)
             if not kwargs.get('cancel'):
+                agg_in(self.columns, kwargs)
                 logging.debug(f'table resource {kwargs} add success')
+            else:
+                try:
+                    agg_in(self.columns, kwargs)
+                except Exception:
+                    raise
+                finally:
+                    agg_in(self.columns, {'cancel': True})
 
     def edit(self, agg_in, old_value, **kwargs) -> None:
         """ 只能编辑匹配到的第一条记录
 
         :param agg_in: function, 导致该方法不能单独使用
         :param old_value: str, 旧值 每列值可按顺序直接连接在一起传入，当然也可以传一列的值
         :param kwargs str, 待添加列 及对应值
@@ -319,17 +334,24 @@
         if exist_tr.count() > 0:
             if exist_tr.first.locator('//i[@class="anticon anticon-form"]').count() == 1:
                 exist_tr.first.locator('//i[@class="anticon anticon-form"]').click()
             else:
                 exist_tr.first.locator('//i[@class="anticon anticon-edit"]').click()
             if ('save' not in list(kwargs.keys())) and ('cancel' not in list(kwargs.keys())):
                 kwargs['save'] = True
-            agg_in(self.columns, kwargs)
             if not kwargs.get('cancel'):
+                agg_in(self.columns, kwargs)
                 logging.debug(f'table resource {kwargs} edit success')
+            else:
+                try:
+                    agg_in(self.columns, kwargs)
+                except Exception:
+                    raise
+                finally:
+                    agg_in(self.columns, {'cancel': True})
         else:
             logging.debug(f'table resource {old_value} not exist')
 
     def delete(self, value: str) -> None:
         """
         :param value str, 待删除列 及对应值 每列值可按顺序直接连接在一起传入，当然也可以传一列的值 自己国际化
         :return:
```

### Comparing `inhandtest-0.0.58/inhandtest/exception.py` & `inhandtest-0.0.59/inhandtest/exception.py`

 * *Files identical despite different names*

### Comparing `inhandtest-0.0.58/inhandtest/file.py` & `inhandtest-0.0.59/inhandtest/file.py`

 * *Files identical despite different names*

### Comparing `inhandtest-0.0.58/inhandtest/inmodbus.py` & `inhandtest-0.0.59/inhandtest/inmodbus.py`

 * *Files identical despite different names*

### Comparing `inhandtest-0.0.58/inhandtest/inmongodb.py` & `inhandtest-0.0.59/inhandtest/inmongodb.py`

 * *Files identical despite different names*

### Comparing `inhandtest-0.0.58/inhandtest/inmqtt.py` & `inhandtest-0.0.59/inhandtest/inmqtt.py`

 * *Files identical despite different names*

### Comparing `inhandtest-0.0.58/inhandtest/inrequest.py` & `inhandtest-0.0.59/inhandtest/inrequest.py`

 * *Files identical despite different names*

### Comparing `inhandtest-0.0.58/inhandtest/inserial.py` & `inhandtest-0.0.59/inhandtest/inserial.py`

 * *Files identical despite different names*

### Comparing `inhandtest-0.0.58/inhandtest/insocket.py` & `inhandtest-0.0.59/inhandtest/insocket.py`

 * *Files identical despite different names*

### Comparing `inhandtest-0.0.58/inhandtest/inssh.py` & `inhandtest-0.0.59/inhandtest/inssh.py`

 * *Files identical despite different names*

### Comparing `inhandtest-0.0.58/inhandtest/ip.py` & `inhandtest-0.0.59/inhandtest/ip.py`

 * *Files identical despite different names*

### Comparing `inhandtest-0.0.58/inhandtest/log.py` & `inhandtest-0.0.59/inhandtest/log.py`

 * *Files identical despite different names*

### Comparing `inhandtest-0.0.58/inhandtest/mail.py` & `inhandtest-0.0.59/inhandtest/mail.py`

 * *Files identical despite different names*

### Comparing `inhandtest-0.0.58/inhandtest/pages/ingateway/edge_computing/edge_computing_locators.py` & `inhandtest-0.0.59/inhandtest/pages/ingateway/edge_computing/edge_computing_locators.py`

 * *Files 2% similar despite different names*

```diff
@@ -176,25 +176,52 @@
 
     @property
     def add_controller_all(self) -> list:
         return [('template_name',
                  {'locator': self.pop_up.locator('.ant-select.ant-select-enabled').first, 'type': 'select'}),
                 ('name', {'locator': self.page.locator('#name'), 'type': 'text'}),
                 ('protocol', {'locator': self.pop_up.locator('.ant-cascader-picker'), 'type': 'select_multi',
-                              'param': {'modbus.modbus tcp': 'Modbus.Modbus Tcp',
+                              'param': {'modbus.modbus tcp': 'Modbus.Modbus Tcp', 'Siemens PLC': self.locale.siemens_plc,
                                         'modbus.modbus rtu': 'Modbus.Modbus Rtu'}}),
+                # opc ua
+                ('servers_url', {'locator': self.pop_up.locator('#endpoint'), 'type': 'text'}),
+
+                # modbus tcp or rtu
                 ('ip_address', {'locator': self.page.locator('#point\.ip'), 'type': 'text'}),
                 ('port', {'locator': self.page.locator('#point\.port'), 'type': 'text'}),
+                # ISO-on-TCP
+                ('mode', {'locator': self.pop_up.locator('#args\.mode'), 'type': 'radio'}),
+                ('rack', {'locator': self.page.locator('#args\.rack'), 'type': 'text'}),
+                ('slot', {'locator': self.page.locator('#args\.slot'), 'type': 'text'}),
+                ('client_tsap', {'locator': self.page.locator('#args\.localTsap'), 'type': 'text'}),
+                ('server_tsap', {'locator': self.page.locator('#args\.remoteTsap'), 'type': 'text'}),
+
                 ('slave', {'locator': self.page.locator('#args\.slaveAddr'), 'type': 'text'}),
                 ('endpoint', {'locator': self.page.locator('#endpoint'), 'type': 'select'}),
                 ('polling_interval', {'locator': self.page.locator('#samplePeriod'), 'type': 'text'}),
                 ('multiple_polling_interval',
                  {'locator': self.page.locator('#enablepollCycle'), 'type': 'switch_button'}),
                 ('polling_interval2', {'locator': self.page.locator('#samplePeriod2'), 'type': 'text',
                                        'relation': [('multiple_polling_interval', 'enable')]}),
+                # opc ua
+                ('auth', {'locator': self.pop_up.locator('#args\.auth'), 'type': 'select',
+                          'param': {'anonymous': self.locale.anonymous,
+                                    'username_password': self.locale.username_password,
+                                    'certificate_auth': self.locale.certificate_auth}}),
+                ('username', {'locator': self.pop_up.locator('#args\.username'), 'type': 'text'}),
+                ('password', {'locator': self.pop_up.locator('#args\.password'), 'type': 'text'}),
+                ('certificate',
+                 {'locator': self.pop_up.locator('.anticon.anticon-upload').nth(0), 'type': 'upload_file'}),
+                ('private_key',
+                 {'locator': self.pop_up.locator('.anticon.anticon-upload').nth(1), 'type': 'upload_file'}),
+                ('security_policy', {'locator': self.pop_up.locator('#args\.securityPolicy'), 'type': 'select',
+                                     'param': {'Automatic detection': self.locale.automatic_detection}}),
+                ('security_mode', {'locator': self.pop_up.locator('#args\.securityMode'), 'type': 'select',
+                                   'param': {'sign': self.locale.sign, 'sign_encrypt': self.locale.sign_encrypt}}),
+                # modbus tcp or rtu
                 ('description', {'locator': self.pop_up.locator('#desc'), 'type': 'text'}),
                 ('advanced_settings', {'locator': self.locale.advanced_settings, 'type': 'expand'}),
                 ('byte_order_16int', {'locator': self.page.locator('#args\.int16Ord'), 'type': 'select',
                                       'relation': [('advanced_settings', 'expand')]}),
                 ('byte_order_32int', {'locator': self.page.locator('#args\.int32Ord'), 'type': 'select',
                                       'relation': [('advanced_settings', 'expand')]}),
                 ('byte_order_32float', {'locator': self.page.locator('#args\.float32Ord'), 'type': 'select',
@@ -365,14 +392,20 @@
             ('time', {'locator': self.page.locator(f'{measure_name}/../../../../td[8]'), 'type': 'text'}),
         ]
         return measures
 
     @property
     def add_measure_all(self):
         return [('name', {'locator': self.pop_up.locator('#name'), 'type': 'text'}),
+                # OPC-UA
+                ('namespace', {'locator': self.pop_up.locator('#index'), 'type': 'text'}),
+                ('address_type', {'locator': self.pop_up.locator('#idType'), 'type': 'select'}),
+                ('identifier', {'locator': self.pop_up.locator('#identifier'), 'type': 'text'}),
+                # ISO-on-TCP
+                ('register_type', {'locator': self.pop_up.locator('#regType'), 'type': 'select'}),
                 ('register_address', [{'locator': self.pop_up.locator(
                     '.antd-pro-components-app-reg-addr-input-index-wrapper >> .ant-input-group-addon'),
                     'type': 'select'},
                     {'locator': self.pop_up.locator(
                         '.antd-pro-components-app-reg-addr-input-index-wrapper >> .ant-input'), 'type': 'text'}]),
                 ('data_type', {'locator': self.pop_up.locator('#dataType'), 'type': 'select',
                                'param': {'bit': self.locale.get('bit'), 'word': self.locale.get('word'),
@@ -386,14 +419,15 @@
                 ('register_bit', {'locator': self.pop_up.locator('#bitIndex'), 'type': 'text'}),
                 ('data_register_bit', {'locator': self.pop_up.locator('#bitIndex'), 'type': 'text'}),
                 ('negative_value', {'locator': self.pop_up.locator('#reverseBit'), 'type': 'switch_button'}),
                 ('size', {'locator': self.pop_up.locator('#len'), 'type': 'text'}),
                 ('encoding_format', {'locator': self.pop_up.locator('#codeType'), 'type': 'select',
                                      'param': {'ascii': 'ASCII', 'utf-8': 'UTF-8', 'utf-16': 'UTF-16',
                                                'utf-16-big': 'UTF-16-BIG', 'gb2312': 'GB2312'}}),
+                ('is_array', {'locator': self.pop_up.locator('#isArr'), 'type': 'switch_button'}),
                 ('read_write', {'locator': self.pop_up.locator('#readWrite'), 'type': 'select',
                                 'param': {'read': 'Read', 'read/write': 'Read/Write', 'write': 'Write'}}),
                 ('mode', {'locator': self.pop_up.locator('#uploadType'), 'type': 'select',
                           'param': {'periodic': 'Periodic', 'onchange': 'Onchange', 'never': 'Never'}}),
                 ('unit', {'locator': self.pop_up.locator('#unit'), 'type': 'text'}),
                 ('description', {'locator': self.pop_up.locator('#desc'), 'type': 'text'}),
                 ('group', {'locator': self.pop_up.locator('#group'), 'type': 'select'}),
@@ -859,30 +893,46 @@
         ]
 
     @property
     def cloud_measuring_point(self) -> list:
         return [
             ('page_number', {'locator': self.pop_up.locator('.ant-pagination-options-size-changer'), 'type': 'select',
                              'param': {'page': f' {self.locale.page_}'}}),
-            ('search', {'locator': self.page.locator('#type'), 'type': 'select',
-                        'param': {'int': self.locale.int, 'float': self.locale.float,
-                                  'bool': self.locale.bool, 'string': self.locale.string}}),
-            ('name', {'locator': self.page.locator('#name'), 'type': 'text'}),
-            ('measuring_point_type', {'locator': self.page.locator('#type'), 'type': 'select',
-                                      'param': {'int': self.locale.int, 'float': self.locale.float,
-                                                'bool': self.locale.bool, 'string': self.locale.string}}),
-            ('unit', {'locator': self.page.locator('#unit'), 'type': 'text'}),
-            ('save', {'locator': self.page.locator('.ant-btn.ant-btn-primary').last,
-                      'type': 'button'}),
-            ('cancel', {'locator': self.page.locator('.ant-btn').last,
-                        'type': 'button'}),
-            ('edit', {'locator': self.page.locator('.anticon.anticon-edit').last,
-                      'type': 'button'}),
-            ('delete', {'locator': self.page.locator('.anticon.anticon-delete').last,
-                        'type': 'button'}),
-            ('delete_confirm', {'locator': self.page.locator('.ant-btn.ant-btn-primary').last,
-                                'type': 'button'}),
+            ('search', [{'locator': self.pop_up.locator('.ant-select.ant-select-enabled').nth(0), 'type': 'select',
+                         'param': {'point_name': self.locale.collection_measuring_point_name,
+                                   'controller_name': self.locale.controller_name,
+                                   'group_name': self.locale.group_name}},
+                        {'locator': self.pop_up.locator('//input[@class="ant-input"]'), 'type': 'text'}]),
+            ('is_search', {'locator': self.pop_up.locator('.anticon.anticon-search'), 'type': 'button'}),
+            ('import', {'locator': self.pop_up.locator('.anticon.anticon-upload'), 'type': 'upload_file'}),
+            ('export', {'locator': self.pop_up.locator('.anticon.anticon-download').first, 'type': 'download_file'}),
+            ('check_all', {'locator': self.pop_up.locator('.ant-checkbox-input').first, 'type': 'check'}),
+            ('mute_bulk', {'locator': self.pop_up.locator('//button[@class="ant-btn"]').first, 'type': 'button'}),
+            ('add_bulk', {'locator': self.pop_up.locator('//button[@class="ant-btn"]').first, 'type': 'button'}),
+            ('bulk_confirm', {'locator': self.page.locator('.ant-popover-content').locator(
+                '.ant-btn.ant-btn-primary.ant-btn-sm'), 'type': 'button',
+                'wait_for': {'type': 'tip_messages', 'messages': self.locale.submit_success}}),
+            ('close', {'locator': self.pop_up.locator('.ant-modal-close-icon'), 'type': 'button'}),
+        ]
+
+    def cloud_measuring_point_table(self, name) -> list:
+        measure_tr = self.pop_up.locator('//tbody[@class="ant-table-tbody"]/tr/td[2]').get_by_text(name,
+                                                                                                   exact=True).locator(
+            '../..')
+        return [
+            ('check', {'locator': measure_tr.locator('.ant-checkbox-input'), 'type': 'button'}),
+            ('mute', {'locator': measure_tr.locator('//td[7]/a'), 'type': 'button'}),
+            ('add', {'locator': measure_tr.locator('//td[7]/a'), 'type': 'button'}),
+            ('confirm',
+             {'locator': self.page.locator('.ant-popover-content').locator('.ant-btn.ant-btn-primary'),
+              'type': 'button', 'wait_for': {'type': 'tip_messages', 'messages': self.locale.submit_success}}),
+            ('name_edit', {'locator': measure_tr.locator('//button'), 'type': 'button'}),
+            ('value', {'locator': self.pop_up.locator('//tbody[@class="ant-table-tbody"]/tr/td').locator(
+                '//input[@class="ant-input"]'),
+                'type': 'text'}),
+            ('submit', {'locator': self.pop_up.locator('//tbody[@class="ant-table-tbody"]/tr/td').locator(
+                '//i[@class="anticon anticon-check"]'), 'type': 'button'}),
         ]
 
 
 class EdgeComputingLocators(PythonEdgeComputingLocators, DockerManagerLocators, DeviceSupervisorLocators):
     pass
```

### Comparing `inhandtest-0.0.58/inhandtest/pages/ingateway/edge_computing/python_edge_computing.py` & `inhandtest-0.0.59/inhandtest/pages/ingateway/edge_computing/python_edge_computing.py`

 * *Files 4% similar despite different names*

```diff
@@ -305,22 +305,35 @@
         """
 
         :param kwargs:
                controller: [(action_type, value, ),]
                            [('add', kwargs)]
                             kwargs:
                                name: 名称
-                               protocol: 'modbus.modbus tcp' | 'modbus.modbus rtu'
+                               protocol: 'modbus.modbus tcp' | 'modbus.modbus rtu'| 'OPC.OPC-UA'|'Siemens Plc.ISO-on-TCP'
+                               servers_url: 服务器地址   OPC-UA
                                ip_address: ip地址
                                port: 端口号
+                               mode: 通讯方式 'Rack/Slot' | 'TSAP'    ISO-on-TCP
+                               rack: 机架号   ISO-on-TCP
+                               slot: 插槽号      ISO-on-TCP
+                               client_tsap:   ISO-on-TCP
+                               server_tsap:  ISO-on-TCP
                                slave: 从站地址
                                endpoint: 通讯方式 'RS485' | 'RS232'
                                polling_interval: 轮询周期 1~864000 s
                                multiple_polling_interval: enable | disable, 轮询周期是否可变
                                polling_interval2: 轮询周期2 1~864000 s
+                               auth: anonymous | username_password| certificate_auth, OPC-UA 验证方式
+                               username: 用户名  OPC-UA
+                               password  : 密码 OPC-UA
+                               certificate: 证书路径 OPC-UA
+                               private_key: 私钥路径 OPC-UA
+                               security_policy: None|Automatic detection|Basic128Rsa15|Basic256|Basic256Sha256|Aes128Sha256RsaOaep 安全策略 OPC-UA
+                               security_mode: None|sign|sign_encrypt 安全模式 OPC-UA
                                description: 描述
                                advanced_settings: 展开高级设置 'expand' | 'close'
                                byte_order_16int: 16位整数字节序 'AB' | 'BA'
                                byte_order_32int: 32位整数字节序 'ABCD' | 'CDAB' | 'DCBA' | 'BADC'
                                byte_order_32float: 32位浮点数字节序 'ABCD' | 'CDAB' | 'DCBA' | 'BADC'
                                byte_order_64int: 同选择框的选项
                                byte_order_64float: 同选择框的选项
@@ -365,24 +378,29 @@
                                     text_messages: 文本信息验证 str or list
                                     tip_messages: 提示信息验证 str or list or dict
                                     cancel: 是否取消  cancel=True
                measure: [(action_type, value, ),]
                         [('add', kwargs)]
                             kwargs:
                                 name: 名称
+                                namespace: 命名空间   OPC-UA
+                                address_type: String|Number   OPC-UA
+                                identifier: 标识符   OPC-UA
+                                register_type:   I|Q|M|DB    ISO-on-TCP
                                 register_address: 寄存器地址 list  ex: ['4X', '40001']
                                 data_type: 数据类型 bit,word,int,dword,dint,float,double,string,bcd16,ulong,long
                                 read_bit_data: enable | disable
                                 register_bit: 位寄存器
                                 data_register_bit: 数据寄存器
                                 negative_value: enable | disable
                                 storage_lwtsdb: enable | disable
                                 decimal_places: 小数位数
                                 size: 数据长度
                                 encoding_format: 编码格式 ascii, utf-8, utf-16, utf-16-big, gb2312
+                                is_array: enable | disable    OPC-UA
                                 read_write: 读写属性 read | write | read/write
                                 mode: periodic | onchange | never
                                 unit: 单位 str
                                 description: 描述
                                 group: 所属组
                                 polling_interval: polling_interval|polling_interval_2
                                 numerical_mapping: 数值映射 enable | disable
@@ -644,26 +662,107 @@
 
 class Cloud(BasePage, IgLocators):
     def __init__(self, host: str, username: str, password: str, protocol='https',
                  port=443, model='IG902', language='en', page=None, locale: dict = None):
         super().__init__(host, username, password, protocol, port, model, language, page, locale=locale)
         IgLocators.__init__(self, page, locale)
 
+    def __measure_point(self, cloud_measure, mute_measure, close=False):
+        """
+
+        :param cloud_measure: [(action_type, value, ),]
+        :param mute_measure: [(action_type, value, ),]
+        :return:
+        """
+        if cloud_measure:
+            self.access_menu('edge_computing.device_supervisor.cloud.mqtt_cloud_service.cloud_measuring_setting.cloud')
+            for ac in cloud_measure:
+                if ac[0] == 'search':
+                    self.agg_in(self.edge_locators.cloud_measuring_point, {"search": ac[1], 'is_search': True})
+                elif ac[0] == 'page_number':
+                    self.agg_in(self.edge_locators.cloud_measuring_point, {"page_number": ac[1]})
+                elif ac[0] in ('import', 'export'):
+                    self.agg_in(self.edge_locators.cloud_measuring_point, {ac[0]: ac[1]})
+                elif ac[0] == 'check':
+                    self.agg_in(self.edge_locators.cloud_measuring_point_table(ac[1]), {'check': ac[2]})
+                elif ac[0] == 'mute':
+                    self.agg_in(self.edge_locators.cloud_measuring_point_table(ac[1]), {'mute': True, 'confirm': True})
+                elif ac[0] == 'check_all':
+                    self.agg_in(self.edge_locators.cloud_measuring_point, {ac[0]: True})
+                elif ac[0] == 'mute_bulk':
+                    self.agg_in(self.edge_locators.cloud_measuring_point, {'check_all': False})  # 先取消选择所有的
+                    all_measure = [ac[1]] if isinstance(ac[1], str) else ac[1]
+                    self.__measure_point(cloud_measure=[('check', x, True) for x in all_measure], mute_measure=None)
+                    self.agg_in(self.edge_locators.cloud_measuring_point, {'mute_bulk': True, 'bulk_confirm': True})
+                elif ac[0] == 'name':
+                    if isinstance(ac[2], str):
+                        value = {'name_edit': True, 'value': ac[2], 'submit': {"wait_for_time": 3 * 1000}}
+                    else:
+                        value = {'name_edit': True}.update(ac[2])
+                    self.agg_in(self.edge_locators.cloud_measuring_point_table(ac[1]), value)
+                else:
+                    pass
+        if mute_measure:
+            self.access_menu('edge_computing.device_supervisor.cloud.mqtt_cloud_service.cloud_measuring_setting.mute')
+            for ac in mute_measure:
+                if ac[0] == 'search':
+                    self.agg_in(self.edge_locators.cloud_measuring_point, {"search": ac[1], 'is_search': True})
+                elif ac[0] == 'page_number':
+                    self.agg_in(self.edge_locators.cloud_measuring_point, {"page_number": ac[1]})
+                elif ac[0] in ('import', 'export'):
+                    self.agg_in(self.edge_locators.cloud_measuring_point, {ac[0]: ac[1]})
+                elif ac[0] == 'check':
+                    self.agg_in(self.edge_locators.cloud_measuring_point_table(ac[1]), {'check': ac[2]})
+                elif ac[0] == 'add':
+                    self.agg_in(self.edge_locators.cloud_measuring_point_table(ac[1]), {'add': True, 'confirm': True})
+                elif ac[0] == 'check_all':
+                    self.agg_in(self.edge_locators.cloud_measuring_point, {ac[0]: True})
+                elif ac[0] == 'add_bulk':
+                    self.agg_in(self.edge_locators.cloud_measuring_point, {'check_all': False})  # 先取消选择所有的
+                    all_measure = [ac[1]] if isinstance(ac[1], str) else ac[1]
+                    self.__measure_point(cloud_measure=None, mute_measure=[('check', x, True) for x in all_measure])
+                    self.agg_in(self.edge_locators.cloud_measuring_point, {'add_bulk': True, 'bulk_confirm': True})
+                else:
+                    pass
+        if (cloud_measure or mute_measure) and close:
+            self.agg_in(self.edge_locators.cloud_measuring_point, {'close': True})
+
     @allure.step('配置Device Supervisor Cloud')
     def config(self, **kwargs):
         """
 
         :param kwargs:
                 enable: bool True | False 是否启用
                 clear_offline_cache: bool True | False 是否清除离线缓存
                 import: str, 导入文件路径
                 import_confirm: bool True | False 是否确认导入, 或者可以写入 确认导入后的提示
                 export: str  or dict   # 导出
                         str: 导出文件夹
                         dict: {"file_path": "./", "file_name": None}
+                cloud_measure: [(action_type, value, ),]
+                    [('page_number', '100page')]  修改每页显示数量
+                    [('search', [$type, name]), ]  # 搜索
+                        type: point_name|controller_name|group_name
+                    [('check', 'test', True), ] or [('check', 'test', False), ]   # 选择与取消选择
+                    [('import', path), ]  # 导入
+                    [('export', path), ]  # 导出
+                    [('check_all', ), ]  # 选择所有
+                    [('mute', 'test',), ]  # 屏蔽
+                    [('mute_bulk', ['test','test1']), ]  # 批量屏蔽
+                    [('name', 'test', 'test1'), ]  # 修改名称
+                mute_measure: [(action_type, value, ),]
+                    [('page_number', '100page')]  修改每页显示数量
+                    [('search', [$type, name]), ]  # 搜索
+                        type: point_name|controller_name|group_name
+                    [('check', 'test', True), ] or [('check', 'test', False), ]   # 选择与取消选择
+                    [('import', path), ]  # 导入
+                    [('export', path), ]  # 导出
+                    [('add_all', ), ]  # 选择所有
+                    [('add', 'test',), ]  # 加入
+                    [('add_bulk', ['test','test1']), ]  # 批量屏蔽
                 cloud_type: mqtt|iSCADA Cloud|alibaba_cloud|AWS IoT|Azure IoT
                 mqtt_server: str
                 mqtt_client_id: str
                 mqtt_auth: True|False
                 mqtt_username: str
                 mqtt_password: str
                 mqtt_last_will: 'expand' | 'collapse'
@@ -744,14 +843,17 @@
                      tip_messages: str or list
                      cancel: True, False
                  [('edit', 'name', kwarg)]
                  多个操作时使用列表 [('add',{}), ('add',{})]
         :return:
         """
         self.access_menu('edge_computing.device_supervisor.cloud')
+        if kwargs.get('cloud_measure') or kwargs.get('mute_measure'):
+            self.agg_in(self.edge_locators.cloud_locator, {'enable': True})
+            self.__measure_point(kwargs.get('cloud_measure'), kwargs.get('mute_measure'), True)
         if kwargs.get('import') and kwargs.get('import_confirm') is None:
             kwargs.update({'import_confirm': True})
         if kwargs.get('clear_offline_cache'):
             kwargs.update({'cache_confirm': True})
         self.agg_in(self.edge_locators.cloud_locator, kwargs)
```

### Comparing `inhandtest-0.0.58/inhandtest/pages/ingateway/ingateway.py` & `inhandtest-0.0.59/inhandtest/pages/ingateway/ingateway.py`

 * *Files 5% similar despite different names*

```diff
@@ -17,38 +17,41 @@
 import os
 
 
 class InGateway(BasePage):
 
     def __init__(self, host: str, super_user: str, super_password: str, page: Page = None, model='IG902',
                  language='en', protocol='https', port=443, username='adm', password='123456', telnet=True,
-                 locale_yaml_path=None):
+                 locale_yaml_path=None, bring_to_front=False):
         """
 
         :param host:   设备主机地址
         :param super_user:  超级用户
         :param super_password: 超级用户密码
         :param page:  playwright page
         :param model:  设备型号  IG902 IG502
         :param language: 语言 en cn
         :param protocol: 协议  http https
         :param port:    端口
         :param username: 用户名
         :param password: 密码
         :param telnet: 是否开启telnet
         :param locale_yaml_path: 语言文件 默认为None
+        :param bring_to_front: 是否将浏览器窗口置顶
         """
 
         if locale_yaml_path:
             in_setting = dynaconf.Dynaconf(
-                settings_files=[os.path.join(os.path.dirname(__file__), 'locale.yml'), locale_yaml_path])
+                settings_files=[os.path.join(os.path.dirname(__file__), 'locale.yml'), locale_yaml_path],
+                merge_enabled=True)
         else:
             in_setting = dynaconf.Dynaconf(
                 settings_files=[os.path.join(os.path.dirname(__file__), 'locale.yml')])
-        super().__init__(host, username, password, protocol, port, model, language, page, locale=in_setting)
+        super().__init__(host, username, password, protocol, port, model, language, page, locale=in_setting,
+                         bring_to_front=bring_to_front)
         if telnet:
             self.telnet = Telnet(model, host, super_user, super_password)
         else:
             self.telnet = None
         if self.language == 'en':
             self.telnet.send_cli(command='language English', type_='user')
         else:
@@ -63,10 +66,9 @@
 
 if __name__ == '__main__':
     from inhandtest.log import enable_log
 
     enable_log(console_level='debug')
     with InGateway('10.5.23.160', 'inhand', '64391099@inhand') as device:
         device.edge.device_supervisor.cloud.config(
-            subscribe=[('add', {'name': 'my_publish',
-                              'topic': '/v122', 'qos': 2, 'entry_function': 'main', 'quick_function': '#import sys'})])
+            cloud_measure=[('export', './'), ])
         device.page.wait_for_timeout(10 * 1000)
```

### Comparing `inhandtest-0.0.58/inhandtest/pages/ingateway/locale.yml` & `inhandtest-0.0.59/inhandtest/pages/ingateway/locale.yml`

 * *Files 3% similar despite different names*

```diff
@@ -154,14 +154,15 @@
   dword: DWORD
   int: INT
   dint: DINT
   float: FLOAT
   double: DOUBLE
   string: STRING
   bcd16: BCD16
+  bcd32: BCD32
   ulong: ULONG
   long: LONG
   ratio_conversion: Ratio Conversion
   offset_and_zoom: Offset And Zoom
   bit_truncation: Bit Truncation
   pt/ct: PT/CT
   value_mapping: Value Mapping
@@ -183,14 +184,24 @@
   last_will: Last-Will and Testament
   'true': True
   'false': False
   unique_certificate_per_device: Unique-certificate-per-device Authentication
   unique_certificate_per_product: Unique-certificate-per-product
   measuring_point: Measuring Point
   alarm_message: Alarm Message
+  collection_measuring_point_name: Collection Measuring Point Name
+  controller_name: Controller Name
+  group_name: Group Name
+  anonymous: Anonymous
+  username_password: Username & Password
+  certificate_auth: Certificate Authentication
+  automatic_detection: Automatic detection
+  sign: Sign
+  sign_encrypt: Sign & Encrypt
+  siemens_plc: Siemens PLC
 cn:
   client: 客户端
   server: 服务器
   ap: 接入端
   connect: 已连接
   disconnect: 未连接
   enable: 启用
@@ -343,14 +354,15 @@
   dword: DWORD(32位无符号整数)
   int: INT(16位有符号整数)
   dint: DINT(32位有符号整数)
   float: FLOAT(单精度浮点数)
   double: DOUBLE(64位浮点数)
   string: STRING(8位字符串)
   bcd16: BCD16(16位BCD码)
+  bcd32: BCD32(32位BCD码)
   ulong: ULONG(64位无符号整数)
   long: LONG(64位有符号整数)
   ratio_conversion: 比例换算
   offset_and_zoom: 偏移及缩放
   bit_truncation: 位截取
   pt/ct: PT/CT
   value_mapping: 数值映射
@@ -372,8 +384,19 @@
   last_will: 遗嘱消息
   'true': 是
   'false': 否
   unique_certificate_per_device: 一机一密
   unique_certificate_per_product: 一型一密
   measuring_point: 测点数据
   alarm_message: 告警数据
+  collection_measuring_point_name: 采集测点名称
+  controller_name: 控制器名称
+  group_name: 分组名称
+  anonymous: 匿名登录
+  username_password: 用户名和密码
+  certificate_auth: 证书认证
+  automatic_detection: 自动检测
+  sign: 签名
+  sign_encryption: 签名和加密
+  siemens_plc: Siemens Plc（西门子）
+
```

### Comparing `inhandtest-0.0.58/inhandtest/pages/ingateway/locators.py` & `inhandtest-0.0.59/inhandtest/pages/ingateway/locators.py`

 * *Files identical despite different names*

### Comparing `inhandtest-0.0.58/inhandtest/pages/ingateway/network/network.py` & `inhandtest-0.0.59/inhandtest/pages/ingateway/network/network.py`

 * *Files 0% similar despite different names*

```diff
@@ -135,14 +135,16 @@
                lcp_interval: 10 ex: lcp_interval=10
                lcp_max_retries: 10 ex: lcp_max_retries=10
                infinitely_dial_retry: enable,disable ex: infinitely_dial_retry="enable"
                debug: enable,disable ex: debug="enable"
                expert_options: 'AT+CPIN?'
                text_messages: str or list or tuple ex: text_messages="Please enter an integer for 1 ~ 604800"
                submit: True or False ex: submit=True  or  submit={'tip_messages': 'cellular_configuration_changed_successful'}
+               confirm: True or False ex: submit=True  or  submit={'tip_messages': 'cellular_configuration_changed_successful'}
+                        拨号参数集配置变更后 在submit后还需要点击confirm才能生效
                reset: True or False ex: reset=True
         :return:
         """
         self.access_menu('network.network_interface.cellular')
         self.agg_in(self.network_locators.cellular_locators, kwargs)
```

### Comparing `inhandtest-0.0.58/inhandtest/pages/ingateway/network/network_locators.py` & `inhandtest-0.0.59/inhandtest/pages/ingateway/network/network_locators.py`

 * *Files 0% similar despite different names*

```diff
@@ -175,17 +175,18 @@
             ('infinitely_dial_retry', {'locator': self.page.locator('#infinitely_dial_retry'), 'type': 'switch_button',
                                        'relation': [('cellular_enable', 'enable'), ('advanced_settings', 'expand')]}),
             ('debug', {'locator': self.page.locator('#debug'), 'type': 'switch_button',
                        'relation': [('cellular_enable', 'enable'), ('advanced_settings', 'expand')]}),
             ('expert_options', {'locator': self.page.locator('#expert_options'), 'type': 'text',
                                 'relation': [('cellular_enable', 'enable'), ('advanced_settings', 'expand')]}),
             ('submit',
-             {'locator': [self.page.locator('//button[@class="ant-btn ant-btn-primary"]', has_text=self.locale.submit),
-                          self.page.locator('.ant-modal-content').locator(
-                              '//button[@class="ant-btn ant-btn-primary"]')],
+             {'locator': self.page.locator('//button[@class="ant-btn ant-btn-primary"]', has_text=self.locale.submit),
+              'type': 'button'}),
+            ('confirm',
+             {'locator': self.page.locator('.ant-modal-content').locator('//button[@class="ant-btn ant-btn-primary"]'),
               'type': 'button'}),
             ('text_messages', {'type': 'text_messages'}),
             ('tip_messages', {'type': 'tip_messages'}),
             ('reset', {'locator': self.page.locator('//button[@class="ant-btn" and @type="reset"]'),
                        'type': 'button'}),
         ]
```

### Comparing `inhandtest-0.0.58/inhandtest/pages/ingateway/overview/overview.py` & `inhandtest-0.0.59/inhandtest/pages/ingateway/overview/overview.py`

 * *Files identical despite different names*

### Comparing `inhandtest-0.0.58/inhandtest/pages/ingateway/overview/overview_locators.py` & `inhandtest-0.0.59/inhandtest/pages/ingateway/overview/overview_locators.py`

 * *Files identical despite different names*

### Comparing `inhandtest-0.0.58/inhandtest/pages/ingateway/system/system.py` & `inhandtest-0.0.59/inhandtest/pages/ingateway/system/system.py`

 * *Files identical despite different names*

### Comparing `inhandtest-0.0.58/inhandtest/pages/ingateway/system/system_locators.py` & `inhandtest-0.0.59/inhandtest/pages/ingateway/system/system_locators.py`

 * *Files identical despite different names*

### Comparing `inhandtest-0.0.58/inhandtest/pytest_email.html` & `inhandtest-0.0.59/inhandtest/pytest_email.html`

 * *Files identical despite different names*

### Comparing `inhandtest-0.0.58/inhandtest/telnet.py` & `inhandtest-0.0.59/inhandtest/telnet.py`

 * *Files identical despite different names*

### Comparing `inhandtest-0.0.58/inhandtest/tools.py` & `inhandtest-0.0.59/inhandtest/tools.py`

 * *Files 0% similar despite different names*

```diff
@@ -12,15 +12,14 @@
 import string
 import subprocess
 import time
 import datetime
 from functools import wraps
 from typing import List
 import pytz
-import winreg
 import requests
 from inhandtest.file import file_hash
 from inhandtest.exception import ResourceNotFoundError
 import logging
 
 
 def loop_inspector(flag='status', timeout=90, interval=5, assertion=True):
@@ -602,14 +601,15 @@
 
 def is_installed(name):
     """
     判断windows系统是否安装了某个软件
     :param name:
     :return: ResourceNotFoundError
     """
+    import winreg
     key = winreg.OpenKey(winreg.HKEY_LOCAL_MACHINE, r"SOFTWARE\Microsoft\Windows\CurrentVersion\Uninstall")
     all_installed = []
     for i in range(0, winreg.QueryInfoKey(key)[0]):
         skey_name = winreg.EnumKey(key, i)
         skey = winreg.OpenKey(key, skey_name)
         try:
             value = winreg.QueryValueEx(skey, 'DisplayName')[0]
```

### Comparing `inhandtest-0.0.58/inhandtest.egg-info/PKG-INFO` & `inhandtest-0.0.59/inhandtest.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.2
 Name: inhandtest
-Version: 0.0.58
+Version: 0.0.59
 Summary: inhand test tools, so easy
 Home-page: https://inhandnetworks.yuque.com/irhb08/mrpu1r/qgu0imvigkm2xry9?singleDoc# 《inhandtest docs》
 Author: liwei
 Author-email: liwei@inhand.com.cn
 Maintainer: liwei
 Maintainer-email: liwei@inhand.com.cn
 License: UNKNOWN
```

### Comparing `inhandtest-0.0.58/inhandtest.egg-info/SOURCES.txt` & `inhandtest-0.0.59/inhandtest.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `inhandtest-0.0.58/setup.py` & `inhandtest-0.0.59/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 
 """
 from distutils.core import setup
 from setuptools import find_packages
 
 setup(
     name='inhandtest',
-    version='0.0.58',
+    version='0.0.59',
     author='liwei',
     author_email='liwei@inhand.com.cn',
     description='inhand test tools, so easy',
     maintainer='liwei',
     maintainer_email='liwei@inhand.com.cn',
     # py_modules=['inhandtest.tools', 'inhandtest.telnet', 'inhandtest.inmodbus', 'inhandtest.inmqtt', 'inhandtest.file',
     #             'inhandtest.inrequest', 'inhandtest.inssh', 'inhandtest.base_page'],
```

