# Comparing `tmp/KwoksTool-0.0.3.tar.gz` & `tmp/KwoksTool-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "KwoksTool-0.0.3.tar", last modified: Wed Jul  5 02:56:56 2023, max compression
+gzip compressed data, was "KwoksTool-0.0.4.tar", last modified: Wed Jul  5 07:53:07 2023, max compression
```

## Comparing `KwoksTool-0.0.3.tar` & `KwoksTool-0.0.4.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxrwx   0        0        0        0 2023-07-05 02:56:56.174671 KwoksTool-0.0.3/
-drwxrwxrwx   0        0        0        0 2023-07-05 02:56:56.159021 KwoksTool-0.0.3/KwoksTool/
--rw-rw-rw-   0        0        0      997 2023-07-05 02:10:33.000000 KwoksTool-0.0.3/KwoksTool/__init__.py
--rw-rw-rw-   0        0        0       22 2023-07-05 02:56:37.000000 KwoksTool-0.0.3/KwoksTool/_version.py
--rw-rw-rw-   0        0        0    14960 2023-07-05 02:09:26.000000 KwoksTool-0.0.3/KwoksTool/function.py
--rw-rw-rw-   0        0        0      122 2023-07-03 23:35:00.000000 KwoksTool-0.0.3/KwoksTool/info.py
--rw-rw-rw-   0        0        0     1806 2023-07-03 23:35:00.000000 KwoksTool-0.0.3/KwoksTool/model.py
--rw-rw-rw-   0        0        0     3750 2023-07-05 02:52:40.000000 KwoksTool-0.0.3/KwoksTool/spider.py
-drwxrwxrwx   0        0        0        0 2023-07-05 02:56:56.159021 KwoksTool-0.0.3/KwoksTool.egg-info/
--rw-rw-rw-   0        0        0       56 2023-07-05 02:56:56.000000 KwoksTool-0.0.3/KwoksTool.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      269 2023-07-05 02:56:56.000000 KwoksTool-0.0.3/KwoksTool.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-05 02:56:56.000000 KwoksTool-0.0.3/KwoksTool.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       10 2023-07-05 02:56:56.000000 KwoksTool-0.0.3/KwoksTool.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       56 2023-07-05 02:56:56.174671 KwoksTool-0.0.3/PKG-INFO
--rw-rw-rw-   0        0        0       64 2023-07-05 02:56:37.000000 KwoksTool-0.0.3/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-07-05 02:56:56.174671 KwoksTool-0.0.3/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-07-05 07:53:07.156870 KwoksTool-0.0.4/
+drwxrwxrwx   0        0        0        0 2023-07-05 07:53:07.156870 KwoksTool-0.0.4/KwoksTool/
+-rw-rw-rw-   0        0        0      997 2023-07-05 02:58:45.000000 KwoksTool-0.0.4/KwoksTool/__init__.py
+-rw-rw-rw-   0        0        0       22 2023-07-05 07:51:55.000000 KwoksTool-0.0.4/KwoksTool/_version.py
+-rw-rw-rw-   0        0        0    16356 2023-07-05 07:50:20.000000 KwoksTool-0.0.4/KwoksTool/function.py
+-rw-rw-rw-   0        0        0      122 2023-07-05 02:58:45.000000 KwoksTool-0.0.4/KwoksTool/info.py
+-rw-rw-rw-   0        0        0     1806 2023-07-05 02:58:45.000000 KwoksTool-0.0.4/KwoksTool/model.py
+-rw-rw-rw-   0        0        0     3750 2023-07-05 02:58:45.000000 KwoksTool-0.0.4/KwoksTool/spider.py
+drwxrwxrwx   0        0        0        0 2023-07-05 07:53:07.156870 KwoksTool-0.0.4/KwoksTool.egg-info/
+-rw-rw-rw-   0        0        0       56 2023-07-05 07:53:06.000000 KwoksTool-0.0.4/KwoksTool.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      269 2023-07-05 07:53:06.000000 KwoksTool-0.0.4/KwoksTool.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-05 07:53:06.000000 KwoksTool-0.0.4/KwoksTool.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       10 2023-07-05 07:53:06.000000 KwoksTool-0.0.4/KwoksTool.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       56 2023-07-05 07:53:07.156870 KwoksTool-0.0.4/PKG-INFO
+-rw-rw-rw-   0        0        0       64 2023-07-05 07:51:55.000000 KwoksTool-0.0.4/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-07-05 07:53:07.156870 KwoksTool-0.0.4/setup.cfg
```

### Comparing `KwoksTool-0.0.3/KwoksTool/__init__.py` & `KwoksTool-0.0.4/KwoksTool/__init__.py`

 * *Files identical despite different names*

### Comparing `KwoksTool-0.0.3/KwoksTool/function.py` & `KwoksTool-0.0.4/KwoksTool/function.py`

 * *Files 5% similar despite different names*

```diff
@@ -21,15 +21,17 @@
 import os.path
 import sys
 from zipfile import ZipFile
 import zipfile
 import os
 import tushare as ts
 def GetCityNumFromLiepin(place):
-    ip = function.GetIpPool()
+    # place:城市名称，例如GetCityNumFromLiepin('温州')
+    # 返回值:城市代码的数组，例如['300060010', '300060090']
+    ip = GetIpPool()
     ip = ip[random.randint(0, len(ip))]
     print('猎聘网正在查询城市编码')
     case=1
     OutNum=1
     while case==1:
         try:
             sheng = place[:place.find('省')]
@@ -68,37 +70,48 @@
             OutNum=OutNum+1
             if OutNum==10:
                 print('抱歉，城市编码查询失败')
                 case=2
             else:
                 continue
 def GetIpPool():
+    # 直接调用获取代理ip的字典，返回值为字典,例如：[{'https': 'https://175.178.6.6:8118'}, {'https': 'https://123.182.59.80:8089'}]
+    # 可以直接调用
     IpPool = []
     data = pd.read_excel(r'C:\Windows\AgentPool.xlsx')
     data = data.values.T.tolist()
     ip = data[0]
     port = data[1]
     type=data[2]
     for i in range(0, len(ip)):
         list = {}
         list[str(type[i])] = str(type[i])+'://'+str(ip[i]).replace(' ', '')+':'+str(port[i]).replace(' ', '')
         IpPool.append(list)
     return IpPool
-def GetCityNumFromBossZhiPing(city):
-    ip = function.GetIpPool()
+def GetCityNumFromBossZhiPing(city,proxies=False):
+    # city:输入省市县的城市名称，例如：'浙江省宁波市'
+    # proxies:是否使用Ip代理
+    # 返回值：城市代码的数组，例如：['101210400']
+    ip = GetIpPool()
     ip = ip[random.randint(0, len(ip))]
     city=(city.split('省')[1]).split('市')[0]
     print('boss直聘查询说明\n本功能只能通过城市名字查询一个，关键词例如(宁波)，返回结果不是区的字典，只是当前城市代码。\n正在查询Boss的城市代码')
-    res = requests.get('https://www.zhipin.com/wapi/zpCommon/data/cityGroup.json',proxies=ip).json()
+    if proxies is True:
+        res = requests.get('https://www.zhipin.com/wapi/zpCommon/data/cityGroup.json',proxies=ip).json()
+    else:
+        res = requests.get('https://www.zhipin.com/wapi/zpCommon/data/cityGroup.json').json()
     res = str(res['zpData']['cityGroup'])
     res = (res.split(str(city))[0]).split('code\': ')[-1].replace(', \'name\': \'', '')
     res=[str(res)]
     return res
-def GetCityNameFromLiepin(num):
-    ip = function.GetIpPool()
+def GetCityNameFromLiepin(num,proxies=False):
+    # num:城市代码，例如：GetCityNameFromLiepin('300060010',proxies=False)
+    # proxies:是否使用代理ip,防止Ip被封禁
+    # 返回值：城市名称，例如：阿克苏市
+    ip = GetIpPool()
     ip = ip[random.randint(0, len(ip))]
     case = 1
     while case == 1:
         try:
             sheng = num[:num.find('省')]
             shi = num[num.find('省') + 1:num.find('市')]
             url = "https://apidok.liepin.com/api/com.liepin.bd.p.v3.get-all-dq"
@@ -110,24 +123,30 @@
                 "X-Fscp-Fe-Version": "",
                 "X-Fscp-Version": "1.1",
                 "X-Fscp-Std-Info": "{\"client_id\": \"40108\"}",
                 "X-Requested-With": "XMLHttpRequest",
                 "X-Fscp-Trace-Id": "8136730b-00b0-4daa-b975-59728e3c2a5a",
                 "X-XSRF-TOKEN": "1vL6nJjVRCu01PAwwQmdEg"
             }
-            data = requests.post(url, data=data, headers=header, proxies=ip).json()
+            if proxies is True:
+                data = requests.post(url, data=data, headers=header, proxies=ip).json()
+            else:
+                data = requests.post(url, data=data, headers=header).json()
             data = str(data)
             data = data.split('\'sort\': \'' + str(num) + '\'')[1]
             data = data.split('\', \'name\': \'')[1]
             data = data.split('\', \'category\'')[0]
             case = 2
             return data
         except:
             continue
-def YesOrNot(ip,case):
+def YesOrNot(ip,case='yes'):
+    # 检测代理ip能否用于猎聘网的网页爬取中
+    # ip:代理ip
+    # 返回值:打印出代理ip和从服务器返回的值，如果返回值里面涵盖工作内容等信息，说明ip可以使用
     def get():
         jsdata = '''
         function r() {
         var e = 1 > 0 && void 0 !== 32 ? 32 : 32;
         console.assert(e >= 32, "最少需生成32位");
         var t = (new Date).getTime()
           , n = e < 32 ? 32 : e
@@ -170,35 +189,40 @@
             data = requests.post(url, data=data, headers=header)
         res = data
         res.encoding = 'utf-8'
         res=res.json()
         print(ip,res)
     get_data('070030','070030010','数据',0,ip,'温州')
 def CheckIp(ip):
+    # ip:{'http': 'http://39.108.230.16:3128'}
+    # 返回值:可以，不可以,返回值为文本
     try:
         if str(ip)[2:7] != 'https':
             res = requests.get('http://httpbin.org/ip', proxies=ip)
             result = '可以'
         else:
             res = requests.get('https://blog.sina.com.cn/', proxies=ip)
             result = '可以'
     except:
         result = '不行'
     return result
 def IntoZip(dir_):
+    # dir_:需要压缩的文件路径
     with ZipFile(str(dir_) + '.zip', 'w') as z:
         z.write(dir_, arcname=(dn := os.path.basename(dir_)))
         for root, dirs, files in os.walk(dir_):
             for fn in files:
                 z.write(
                     fp := os.path.join(root, fn),
                     arcname=dn + '/' + os.path.relpath(fp, dir_)
                 )
     print('压缩成功，已经压缩到了文件夹:' + str(dir_) + '.zip')
 def ZipOut(dir, out):
+    # dir:解压文件的路径，涵盖文件名
+    # out:解压到
     zf = zipfile.ZipFile(dir)
     os.chdir(out)
     ret = zf.extractall(path=out)  # 解压到指定目录
     print('解压成功')
 def SendEmail(name,password, receivers, text, sub, filepath):
     smtp_server = "smtp.qq.com"  # 发送邮箱服务器
     username = "yongxingkwok@foxmail.com"  # 用于发送邮箱的用户账号
```

### Comparing `KwoksTool-0.0.3/KwoksTool/model.py` & `KwoksTool-0.0.4/KwoksTool/model.py`

 * *Files identical despite different names*

### Comparing `KwoksTool-0.0.3/KwoksTool/spider.py` & `KwoksTool-0.0.4/KwoksTool/spider.py`

 * *Files identical despite different names*

