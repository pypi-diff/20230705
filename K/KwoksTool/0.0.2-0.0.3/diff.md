# Comparing `tmp/KwoksTool-0.0.2.tar.gz` & `tmp/KwoksTool-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "KwoksTool-0.0.2.tar", last modified: Mon Jul  3 08:23:23 2023, max compression
+gzip compressed data, was "KwoksTool-0.0.3.tar", last modified: Wed Jul  5 02:56:56 2023, max compression
```

## Comparing `KwoksTool-0.0.2.tar` & `KwoksTool-0.0.3.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxrwx   0        0        0        0 2023-07-03 08:23:23.181223 KwoksTool-0.0.2/
-drwxrwxrwx   0        0        0        0 2023-07-03 08:23:23.165601 KwoksTool-0.0.2/KwoksTool/
--rw-rw-rw-   0        0        0     1069 2023-07-03 08:22:49.000000 KwoksTool-0.0.2/KwoksTool/__init__.py
--rw-rw-rw-   0        0        0       22 2023-07-03 08:23:08.000000 KwoksTool-0.0.2/KwoksTool/_version.py
--rw-rw-rw-   0        0        0    15838 2023-07-03 07:54:38.000000 KwoksTool-0.0.2/KwoksTool/function.py
--rw-rw-rw-   0        0        0      122 2023-07-03 07:43:06.000000 KwoksTool-0.0.2/KwoksTool/info.py
--rw-rw-rw-   0        0        0     1806 2023-07-03 07:56:39.000000 KwoksTool-0.0.2/KwoksTool/model.py
--rw-rw-rw-   0        0        0      734 2023-07-03 07:50:23.000000 KwoksTool-0.0.2/KwoksTool/spider.py
-drwxrwxrwx   0        0        0        0 2023-07-03 08:23:23.165601 KwoksTool-0.0.2/KwoksTool.egg-info/
--rw-rw-rw-   0        0        0       56 2023-07-03 08:23:23.000000 KwoksTool-0.0.2/KwoksTool.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      269 2023-07-03 08:23:23.000000 KwoksTool-0.0.2/KwoksTool.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-03 08:23:23.000000 KwoksTool-0.0.2/KwoksTool.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       10 2023-07-03 08:23:23.000000 KwoksTool-0.0.2/KwoksTool.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       56 2023-07-03 08:23:23.181223 KwoksTool-0.0.2/PKG-INFO
--rw-rw-rw-   0        0        0       64 2023-07-03 08:23:02.000000 KwoksTool-0.0.2/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-07-03 08:23:23.181223 KwoksTool-0.0.2/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-07-05 02:56:56.174671 KwoksTool-0.0.3/
+drwxrwxrwx   0        0        0        0 2023-07-05 02:56:56.159021 KwoksTool-0.0.3/KwoksTool/
+-rw-rw-rw-   0        0        0      997 2023-07-05 02:10:33.000000 KwoksTool-0.0.3/KwoksTool/__init__.py
+-rw-rw-rw-   0        0        0       22 2023-07-05 02:56:37.000000 KwoksTool-0.0.3/KwoksTool/_version.py
+-rw-rw-rw-   0        0        0    14960 2023-07-05 02:09:26.000000 KwoksTool-0.0.3/KwoksTool/function.py
+-rw-rw-rw-   0        0        0      122 2023-07-03 23:35:00.000000 KwoksTool-0.0.3/KwoksTool/info.py
+-rw-rw-rw-   0        0        0     1806 2023-07-03 23:35:00.000000 KwoksTool-0.0.3/KwoksTool/model.py
+-rw-rw-rw-   0        0        0     3750 2023-07-05 02:52:40.000000 KwoksTool-0.0.3/KwoksTool/spider.py
+drwxrwxrwx   0        0        0        0 2023-07-05 02:56:56.159021 KwoksTool-0.0.3/KwoksTool.egg-info/
+-rw-rw-rw-   0        0        0       56 2023-07-05 02:56:56.000000 KwoksTool-0.0.3/KwoksTool.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      269 2023-07-05 02:56:56.000000 KwoksTool-0.0.3/KwoksTool.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-05 02:56:56.000000 KwoksTool-0.0.3/KwoksTool.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       10 2023-07-05 02:56:56.000000 KwoksTool-0.0.3/KwoksTool.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       56 2023-07-05 02:56:56.174671 KwoksTool-0.0.3/PKG-INFO
+-rw-rw-rw-   0        0        0       64 2023-07-05 02:56:37.000000 KwoksTool-0.0.3/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-07-05 02:56:56.174671 KwoksTool-0.0.3/setup.cfg
```

### Comparing `KwoksTool-0.0.2/KwoksTool/__init__.py` & `KwoksTool-0.0.3/KwoksTool/__init__.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,22 +1,20 @@
 import os
 from KwoksTool.info import (welcome,how)
-from KwoksTool.spider import (Browser)
+from KwoksTool.spider import (Browser,PlateComponentStocks)
 from KwoksTool.function import (GetCityNumFromLiepin,
                                 GetIpPool,
                                 GetCityNumFromBossZhiPing,
                                 GetCityNameFromLiepin,
                                 YesOrNot,
                                 CheckIp,
                                 IntoZip,
                                 ZipOut,
                                 SendEmail,
                                 GetEmail,
                                 ProgressBar,
-                                GetPlateSon,
-                                GetPlateInfo,
                                 MergeTable,
                                 ChoiceColumn)
 from KwoksTool.model import (GetProbMatrix,ToMat)
 if not os.path.exists(
         r'C:\Windows\AgentPool.xlsx'):
     print('注意注意！\n请确保存在\'C:\Windows\AgentPool.xlsx\'的ip代理文件\n否则，ip池功能将无法使用\n继续使用请敲击回车键')
```

### Comparing `KwoksTool-0.0.2/KwoksTool/function.py` & `KwoksTool-0.0.3/KwoksTool/function.py`

 * *Files 3% similar despite different names*

```diff
@@ -284,15 +284,15 @@
         # print("title:", title)
         get_att(msg, dir)
 def ProgressBar(i, sum, printvalue):
     sys.stdout.write('\r')
     sys.stdout.write('{}%|{}{}|{}'.format(int(i / sum * 100), ((int(i / sum * 100))) * '■',
                                           (100 - int(i / sum * 100 + 1)) * '_', '当前打印：' + str(printvalue)))
     sys.stdout.flush()
-def GetPlateSon(num):
+def GetPlateSon1(num):
     if num == '':
         res = requests.get(r'https://hq.stock.sohu.com/pl/pl-1631.html?uid=1681655630543283qgz&548285357286').text
         res = json.loads(
             res.split('PEAK_ODIA(')[1].split(')</script>')[0].replace('\'pllist\',', '').replace('\'', '"'))
         info = ''
         for son in res:
             info = info + son[1] + ':' + son[0] + '、'
@@ -311,36 +311,14 @@
         result2 = []
         for son1 in name:
             result2.append(son1.replace('\'', '').replace('>', '').replace('<', ''))
         result = {}
         result['代码'] = result2
         result['名称'] = result1
         return result
-def GetPlateInfo(PlateInfoName, url,code):
-    def FindCode(codes):
-        result = []
-        pro = ts.pro_api(ApiCode)
-        data = pro.daily(ts_code='')
-        data = data.sort_values(by='ts_code')
-        data = data['ts_code'].T.values.tolist()
-        for i in range(0, len(data)):
-            if data[i][:6] == codes:
-                result.append(data[i])
-        return result
-
-    a =function.GetPlateSon(PlateInfoName)
-    ApiCode=code
-    pro = ts.pro_api(ApiCode)
-    print('正在下载' + str(PlateInfoName) + '板块的股票信息')
-    for i in range(0, len(a['代码'])):
-        code = FindCode(a['代码'][i])
-        for son in code:
-            data = pro.daily(ts_code=son)
-            data.to_csv(r'{}\{}-{}.csv'.format(url, a['名称'][i], a['代码'][i]))
-            function.ProgressBar(i, len(a['代码']), a['名称'][i])
 def MergeTable(data1, data2, on, data1name, data2name):
     data1 = pd.merge(data1, data2, on=on, how='outer')
     for i in range(0, len(list(data1))):
         data1 = data1.rename(
             columns={list(data1)[i]: list(data1)[i].replace('_x', data1name).replace('_y', data2name)})
     return data1
 def ChoiceColumn(date,name):
```

### Comparing `KwoksTool-0.0.2/KwoksTool/model.py` & `KwoksTool-0.0.3/KwoksTool/model.py`

 * *Files identical despite different names*

