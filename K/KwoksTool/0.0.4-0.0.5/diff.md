# Comparing `tmp/KwoksTool-0.0.4.tar.gz` & `tmp/KwoksTool-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "KwoksTool-0.0.4.tar", last modified: Wed Jul  5 07:53:07 2023, max compression
+gzip compressed data, was "KwoksTool-0.0.5.tar", last modified: Wed Jul  5 12:57:40 2023, max compression
```

## Comparing `KwoksTool-0.0.4.tar` & `KwoksTool-0.0.5.tar`

### file list

```diff
@@ -1,16 +1,18 @@
-drwxrwxrwx   0        0        0        0 2023-07-05 07:53:07.156870 KwoksTool-0.0.4/
-drwxrwxrwx   0        0        0        0 2023-07-05 07:53:07.156870 KwoksTool-0.0.4/KwoksTool/
--rw-rw-rw-   0        0        0      997 2023-07-05 02:58:45.000000 KwoksTool-0.0.4/KwoksTool/__init__.py
--rw-rw-rw-   0        0        0       22 2023-07-05 07:51:55.000000 KwoksTool-0.0.4/KwoksTool/_version.py
--rw-rw-rw-   0        0        0    16356 2023-07-05 07:50:20.000000 KwoksTool-0.0.4/KwoksTool/function.py
--rw-rw-rw-   0        0        0      122 2023-07-05 02:58:45.000000 KwoksTool-0.0.4/KwoksTool/info.py
--rw-rw-rw-   0        0        0     1806 2023-07-05 02:58:45.000000 KwoksTool-0.0.4/KwoksTool/model.py
--rw-rw-rw-   0        0        0     3750 2023-07-05 02:58:45.000000 KwoksTool-0.0.4/KwoksTool/spider.py
-drwxrwxrwx   0        0        0        0 2023-07-05 07:53:07.156870 KwoksTool-0.0.4/KwoksTool.egg-info/
--rw-rw-rw-   0        0        0       56 2023-07-05 07:53:06.000000 KwoksTool-0.0.4/KwoksTool.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      269 2023-07-05 07:53:06.000000 KwoksTool-0.0.4/KwoksTool.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-05 07:53:06.000000 KwoksTool-0.0.4/KwoksTool.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       10 2023-07-05 07:53:06.000000 KwoksTool-0.0.4/KwoksTool.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       56 2023-07-05 07:53:07.156870 KwoksTool-0.0.4/PKG-INFO
--rw-rw-rw-   0        0        0       64 2023-07-05 07:51:55.000000 KwoksTool-0.0.4/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-07-05 07:53:07.156870 KwoksTool-0.0.4/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-07-05 12:57:40.988531 KwoksTool-0.0.5/
+drwxrwxrwx   0        0        0        0 2023-07-05 12:57:40.972932 KwoksTool-0.0.5/KwoksTool/
+-rw-rw-rw-   0        0        0      807 2023-07-05 12:56:26.000000 KwoksTool-0.0.5/KwoksTool/__init__.py
+-rw-rw-rw-   0        0        0       22 2023-07-05 12:57:17.000000 KwoksTool-0.0.5/KwoksTool/_version.py
+-rw-rw-rw-   0        0        0    15701 2023-07-05 12:56:58.000000 KwoksTool-0.0.5/KwoksTool/function.py
+-rw-rw-rw-   0        0        0      122 2023-07-05 12:54:44.000000 KwoksTool-0.0.5/KwoksTool/info.py
+-rw-rw-rw-   0        0        0     1806 2023-07-05 12:54:44.000000 KwoksTool-0.0.5/KwoksTool/model.py
+drwxrwxrwx   0        0        0        0 2023-07-05 12:57:40.972932 KwoksTool-0.0.5/KwoksTool/source/
+-rw-rw-rw-   0        0        0   199365 2023-07-05 10:25:10.000000 KwoksTool-0.0.5/KwoksTool/source/IpPool.py
+-rw-rw-rw-   0        0        0     3750 2023-07-05 12:54:44.000000 KwoksTool-0.0.5/KwoksTool/spider.py
+drwxrwxrwx   0        0        0        0 2023-07-05 12:57:40.972932 KwoksTool-0.0.5/KwoksTool.egg-info/
+-rw-rw-rw-   0        0        0       56 2023-07-05 12:57:40.000000 KwoksTool-0.0.5/KwoksTool.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      296 2023-07-05 12:57:40.000000 KwoksTool-0.0.5/KwoksTool.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-05 12:57:40.000000 KwoksTool-0.0.5/KwoksTool.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       10 2023-07-05 12:57:40.000000 KwoksTool-0.0.5/KwoksTool.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       56 2023-07-05 12:57:40.972932 KwoksTool-0.0.5/PKG-INFO
+-rw-rw-rw-   0        0        0       64 2023-07-05 12:53:12.000000 KwoksTool-0.0.5/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-07-05 12:57:40.988531 KwoksTool-0.0.5/setup.cfg
```

### Comparing `KwoksTool-0.0.4/KwoksTool/function.py` & `KwoksTool-0.0.5/KwoksTool/function.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,13 @@
 import pandas as pd
 import requests
 import random
-from selenium import webdriver
-from selenium.webdriver.chrome.service import Service
+from KwoksTool.source.IpPool import GetIpPool
 import email
 import imaplib
-import numpy as np
 import re
 from email.header import decode_header
 import execjs
 import json
 import mimetypes
 import smtplib   # 发送邮件模块
 from email import encoders
@@ -19,15 +17,14 @@
 import  datetime
 from email.utils import formataddr
 import os.path
 import sys
 from zipfile import ZipFile
 import zipfile
 import os
-import tushare as ts
 def GetCityNumFromLiepin(place):
     # place:城市名称，例如GetCityNumFromLiepin('温州')
     # 返回值:城市代码的数组，例如['300060010', '300060090']
     ip = GetIpPool()
     ip = ip[random.randint(0, len(ip))]
     print('猎聘网正在查询城市编码')
     case=1
@@ -69,28 +66,14 @@
         except:
             OutNum=OutNum+1
             if OutNum==10:
                 print('抱歉，城市编码查询失败')
                 case=2
             else:
                 continue
-def GetIpPool():
-    # 直接调用获取代理ip的字典，返回值为字典,例如：[{'https': 'https://175.178.6.6:8118'}, {'https': 'https://123.182.59.80:8089'}]
-    # 可以直接调用
-    IpPool = []
-    data = pd.read_excel(r'C:\Windows\AgentPool.xlsx')
-    data = data.values.T.tolist()
-    ip = data[0]
-    port = data[1]
-    type=data[2]
-    for i in range(0, len(ip)):
-        list = {}
-        list[str(type[i])] = str(type[i])+'://'+str(ip[i]).replace(' ', '')+':'+str(port[i]).replace(' ', '')
-        IpPool.append(list)
-    return IpPool
 def GetCityNumFromBossZhiPing(city,proxies=False):
     # city:输入省市县的城市名称，例如：'浙江省宁波市'
     # proxies:是否使用Ip代理
     # 返回值：城市代码的数组，例如：['101210400']
     ip = GetIpPool()
     ip = ip[random.randint(0, len(ip))]
     city=(city.split('省')[1]).split('市')[0]
```

### Comparing `KwoksTool-0.0.4/KwoksTool/model.py` & `KwoksTool-0.0.5/KwoksTool/model.py`

 * *Files identical despite different names*

### Comparing `KwoksTool-0.0.4/KwoksTool/spider.py` & `KwoksTool-0.0.5/KwoksTool/spider.py`

 * *Files identical despite different names*

