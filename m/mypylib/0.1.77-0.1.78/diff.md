# Comparing `tmp/mypylib-0.1.77.tar.gz` & `tmp/mypylib-0.1.78.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mypylib-0.1.77.tar", last modified: Mon Jun 19 13:27:10 2023, max compression
+gzip compressed data, was "mypylib-0.1.78.tar", last modified: Wed Jul  5 13:47:45 2023, max compression
```

## Comparing `mypylib-0.1.77.tar` & `mypylib-0.1.78.tar`

### file list

```diff
@@ -1,35 +1,35 @@
-drwxr-xr-x   0 chenwei-ting   (501) staff       (20)        0 2023-06-19 13:27:10.933024 mypylib-0.1.77/
--rw-r--r--   0 chenwei-ting   (501) staff       (20)      373 2023-06-19 13:27:10.932757 mypylib-0.1.77/PKG-INFO
--rw-r--r--   0 chenwei-ting   (501) staff       (20)     3740 2022-08-12 06:28:20.000000 mypylib-0.1.77/README.md
-drwxr-xr-x   0 chenwei-ting   (501) staff       (20)        0 2023-06-19 13:27:10.929918 mypylib-0.1.77/mypylib/
--rw-r--r--   0 chenwei-ting   (501) staff       (20)     3184 2022-07-20 06:07:23.000000 mypylib-0.1.77/mypylib/MP_shioaji_ticks.py
--rw-r--r--   0 chenwei-ting   (501) staff       (20)    47089 2023-06-19 13:26:14.000000 mypylib-0.1.77/mypylib/__init__.py
--rw-r--r--   0 chenwei-ting   (501) staff       (20)     7105 2022-07-25 06:39:45.000000 mypylib-0.1.77/mypylib/binance_copy_bot.py
--rw-r--r--   0 chenwei-ting   (501) staff       (20)     6342 2022-07-15 14:28:35.000000 mypylib-0.1.77/mypylib/binance_copy_bot_test.py
--rw-r--r--   0 chenwei-ting   (501) staff       (20)     3421 2022-08-01 06:21:06.000000 mypylib-0.1.77/mypylib/chdbif.py
--rw-r--r--   0 chenwei-ting   (501) staff       (20)     1857 2023-06-15 12:43:45.000000 mypylib-0.1.77/mypylib/crawler.py
--rw-r--r--   0 chenwei-ting   (501) staff       (20)     1083 2022-09-13 02:48:34.000000 mypylib-0.1.77/mypylib/crypto.py
--rw-r--r--   0 chenwei-ting   (501) staff       (20)     5093 2022-08-12 06:28:16.000000 mypylib-0.1.77/mypylib/finmind.py
--rw-r--r--   0 chenwei-ting   (501) staff       (20)    87196 2022-06-02 06:59:21.000000 mypylib-0.1.77/mypylib/libexcel.py
--rw-r--r--   0 chenwei-ting   (501) staff       (20)    24435 2023-06-01 04:56:52.000000 mypylib-0.1.77/mypylib/mvp.py
--rw-r--r--   0 chenwei-ting   (501) staff       (20)     1255 2022-06-26 10:52:11.000000 mypylib-0.1.77/mypylib/mytest.py
--rw-r--r--   0 chenwei-ting   (501) staff       (20)     3588 2022-06-12 10:26:49.000000 mypylib-0.1.77/mypylib/option_test.py
--rw-r--r--   0 chenwei-ting   (501) staff       (20)      778 2022-06-02 06:59:21.000000 mypylib-0.1.77/mypylib/shioaji_history_ticks.py
--rw-r--r--   0 chenwei-ting   (501) staff       (20)     2490 2023-04-11 13:54:33.000000 mypylib-0.1.77/mypylib/shioaji_kline.py
--rw-r--r--   0 chenwei-ting   (501) staff       (20)     1312 2022-06-02 06:59:21.000000 mypylib-0.1.77/mypylib/shioaji_ticks.py
--rw-r--r--   0 chenwei-ting   (501) staff       (20)     7649 2023-04-18 13:50:52.000000 mypylib-0.1.77/mypylib/sjtools.py
--rw-r--r--   0 chenwei-ting   (501) staff       (20)     1464 2022-09-05 05:47:59.000000 mypylib-0.1.77/mypylib/tLineNotify.py
--rw-r--r--   0 chenwei-ting   (501) staff       (20)     7735 2023-06-01 04:56:52.000000 mypylib-0.1.77/mypylib/ti.py
-drwxr-xr-x   0 chenwei-ting   (501) staff       (20)        0 2023-06-19 13:27:10.931913 mypylib-0.1.77/mypylib/tmpDevelopment/
--rw-r--r--   0 chenwei-ting   (501) staff       (20)        0 2022-07-16 06:27:26.000000 mypylib-0.1.77/mypylib/tmpDevelopment/__init__.py
--rw-r--r--   0 chenwei-ting   (501) staff       (20)     1074 2022-07-16 07:09:42.000000 mypylib-0.1.77/mypylib/tmpDevelopment/warrant_test.py
--rw-r--r--   0 chenwei-ting   (501) staff       (20)     2543 2023-04-27 13:08:02.000000 mypylib-0.1.77/mypylib/tplaysound.py
--rw-r--r--   0 chenwei-ting   (501) staff       (20)     8466 2023-06-19 13:26:50.000000 mypylib-0.1.77/mypylib/tredis.py
--rw-r--r--   0 chenwei-ting   (501) staff       (20)     8184 2023-04-11 13:54:33.000000 mypylib-0.1.77/mypylib/warrant.py
-drwxr-xr-x   0 chenwei-ting   (501) staff       (20)        0 2023-06-19 13:27:10.931218 mypylib-0.1.77/mypylib.egg-info/
--rw-r--r--   0 chenwei-ting   (501) staff       (20)      373 2023-06-19 13:27:10.000000 mypylib-0.1.77/mypylib.egg-info/PKG-INFO
--rw-r--r--   0 chenwei-ting   (501) staff       (20)      673 2023-06-19 13:27:10.000000 mypylib-0.1.77/mypylib.egg-info/SOURCES.txt
--rw-r--r--   0 chenwei-ting   (501) staff       (20)        1 2023-06-19 13:27:10.000000 mypylib-0.1.77/mypylib.egg-info/dependency_links.txt
--rw-r--r--   0 chenwei-ting   (501) staff       (20)        8 2023-06-19 13:27:10.000000 mypylib-0.1.77/mypylib.egg-info/top_level.txt
--rw-r--r--   0 chenwei-ting   (501) staff       (20)       38 2023-06-19 13:27:10.933115 mypylib-0.1.77/setup.cfg
--rw-r--r--   0 chenwei-ting   (501) staff       (20)      846 2022-06-29 14:27:00.000000 mypylib-0.1.77/setup.py
+drwxr-xr-x   0 chenwei-ting   (501) staff       (20)        0 2023-07-05 13:47:45.767074 mypylib-0.1.78/
+-rw-r--r--   0 chenwei-ting   (501) staff       (20)      373 2023-07-05 13:47:45.766856 mypylib-0.1.78/PKG-INFO
+-rw-r--r--   0 chenwei-ting   (501) staff       (20)     3740 2022-08-12 06:28:20.000000 mypylib-0.1.78/README.md
+drwxr-xr-x   0 chenwei-ting   (501) staff       (20)        0 2023-07-05 13:47:45.764820 mypylib-0.1.78/mypylib/
+-rw-r--r--   0 chenwei-ting   (501) staff       (20)     3184 2022-07-20 06:07:23.000000 mypylib-0.1.78/mypylib/MP_shioaji_ticks.py
+-rw-r--r--   0 chenwei-ting   (501) staff       (20)    47136 2023-07-05 13:45:52.000000 mypylib-0.1.78/mypylib/__init__.py
+-rw-r--r--   0 chenwei-ting   (501) staff       (20)     7105 2022-07-25 06:39:45.000000 mypylib-0.1.78/mypylib/binance_copy_bot.py
+-rw-r--r--   0 chenwei-ting   (501) staff       (20)     6342 2022-07-15 14:28:35.000000 mypylib-0.1.78/mypylib/binance_copy_bot_test.py
+-rw-r--r--   0 chenwei-ting   (501) staff       (20)     3421 2022-08-01 06:21:06.000000 mypylib-0.1.78/mypylib/chdbif.py
+-rw-r--r--   0 chenwei-ting   (501) staff       (20)     2404 2023-07-05 13:44:43.000000 mypylib-0.1.78/mypylib/crawler.py
+-rw-r--r--   0 chenwei-ting   (501) staff       (20)     1083 2022-09-13 02:48:34.000000 mypylib-0.1.78/mypylib/crypto.py
+-rw-r--r--   0 chenwei-ting   (501) staff       (20)     5093 2022-08-12 06:28:16.000000 mypylib-0.1.78/mypylib/finmind.py
+-rw-r--r--   0 chenwei-ting   (501) staff       (20)    87196 2022-06-02 06:59:21.000000 mypylib-0.1.78/mypylib/libexcel.py
+-rw-r--r--   0 chenwei-ting   (501) staff       (20)    24435 2023-06-01 04:56:52.000000 mypylib-0.1.78/mypylib/mvp.py
+-rw-r--r--   0 chenwei-ting   (501) staff       (20)     1255 2022-06-26 10:52:11.000000 mypylib-0.1.78/mypylib/mytest.py
+-rw-r--r--   0 chenwei-ting   (501) staff       (20)     3588 2022-06-12 10:26:49.000000 mypylib-0.1.78/mypylib/option_test.py
+-rw-r--r--   0 chenwei-ting   (501) staff       (20)      778 2022-06-02 06:59:21.000000 mypylib-0.1.78/mypylib/shioaji_history_ticks.py
+-rw-r--r--   0 chenwei-ting   (501) staff       (20)     2490 2023-04-11 13:54:33.000000 mypylib-0.1.78/mypylib/shioaji_kline.py
+-rw-r--r--   0 chenwei-ting   (501) staff       (20)     1312 2022-06-02 06:59:21.000000 mypylib-0.1.78/mypylib/shioaji_ticks.py
+-rw-r--r--   0 chenwei-ting   (501) staff       (20)     7649 2023-04-18 13:50:52.000000 mypylib-0.1.78/mypylib/sjtools.py
+-rw-r--r--   0 chenwei-ting   (501) staff       (20)     1464 2022-09-05 05:47:59.000000 mypylib-0.1.78/mypylib/tLineNotify.py
+-rw-r--r--   0 chenwei-ting   (501) staff       (20)     7735 2023-06-01 04:56:52.000000 mypylib-0.1.78/mypylib/ti.py
+drwxr-xr-x   0 chenwei-ting   (501) staff       (20)        0 2023-07-05 13:47:45.766487 mypylib-0.1.78/mypylib/tmpDevelopment/
+-rw-r--r--   0 chenwei-ting   (501) staff       (20)        0 2022-07-16 06:27:26.000000 mypylib-0.1.78/mypylib/tmpDevelopment/__init__.py
+-rw-r--r--   0 chenwei-ting   (501) staff       (20)     1074 2022-07-16 07:09:42.000000 mypylib-0.1.78/mypylib/tmpDevelopment/warrant_test.py
+-rw-r--r--   0 chenwei-ting   (501) staff       (20)     2543 2023-04-27 13:08:02.000000 mypylib-0.1.78/mypylib/tplaysound.py
+-rw-r--r--   0 chenwei-ting   (501) staff       (20)     8466 2023-06-19 13:26:50.000000 mypylib-0.1.78/mypylib/tredis.py
+-rw-r--r--   0 chenwei-ting   (501) staff       (20)     8217 2023-07-03 23:14:11.000000 mypylib-0.1.78/mypylib/warrant.py
+drwxr-xr-x   0 chenwei-ting   (501) staff       (20)        0 2023-07-05 13:47:45.766006 mypylib-0.1.78/mypylib.egg-info/
+-rw-r--r--   0 chenwei-ting   (501) staff       (20)      373 2023-07-05 13:47:45.000000 mypylib-0.1.78/mypylib.egg-info/PKG-INFO
+-rw-r--r--   0 chenwei-ting   (501) staff       (20)      673 2023-07-05 13:47:45.000000 mypylib-0.1.78/mypylib.egg-info/SOURCES.txt
+-rw-r--r--   0 chenwei-ting   (501) staff       (20)        1 2023-07-05 13:47:45.000000 mypylib-0.1.78/mypylib.egg-info/dependency_links.txt
+-rw-r--r--   0 chenwei-ting   (501) staff       (20)        8 2023-07-05 13:47:45.000000 mypylib-0.1.78/mypylib.egg-info/top_level.txt
+-rw-r--r--   0 chenwei-ting   (501) staff       (20)       38 2023-07-05 13:47:45.767203 mypylib-0.1.78/setup.cfg
+-rw-r--r--   0 chenwei-ting   (501) staff       (20)      846 2022-06-29 14:27:00.000000 mypylib-0.1.78/setup.py
```

### Comparing `mypylib-0.1.77/README.md` & `mypylib-0.1.78/README.md`

 * *Files identical despite different names*

### Comparing `mypylib-0.1.77/mypylib/MP_shioaji_ticks.py` & `mypylib-0.1.78/mypylib/MP_shioaji_ticks.py`

 * *Files identical despite different names*

### Comparing `mypylib-0.1.77/mypylib/__init__.py` & `mypylib-0.1.78/mypylib/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -65,18 +65,19 @@
     '2023/04/18: 0.1.70 Market() 增加 ask bid information',
     '2023/04/27: 0.1.71 tplaysound 減少buffer音量以免很吵',
     '2023/05/10: 0.1.72 改用shioaji API',
     '2023/05/17: 0.1.73 shioaji 1.0 改 Mmvp.py & ti.py',
     '2023/05/22: 0.1.74 mvp() 不繼承 base class。因為shioaji升級的關係。先可以跑再說',
     '2023/06/01: 0.1.75 Apply Carey change',
     '2023/06/15: 0.1.76 Add crawler',
-    '2023/06/19: 0.1.77 Not using stupid Redis connection pool'
+    '2023/06/19: 0.1.77 Not using stupid Redis connection pool',
+    '2023/07/05: 0.1.78 cynes api v1 support'
 }
 
-__version__ = '0.1.77'
+__version__ = '0.1.78'
 
 request_headers = {
     'User-Agent': 'Mozilla/5.0 (Macintosh; Intel Mac OS X 10_10_1) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/39.0.2171.95 Safari/537.36'
 }
 
 path_cronlog = 'cronlog'
```

### Comparing `mypylib-0.1.77/mypylib/binance_copy_bot.py` & `mypylib-0.1.78/mypylib/binance_copy_bot.py`

 * *Files identical despite different names*

### Comparing `mypylib-0.1.77/mypylib/binance_copy_bot_test.py` & `mypylib-0.1.78/mypylib/binance_copy_bot_test.py`

 * *Files identical despite different names*

### Comparing `mypylib-0.1.77/mypylib/chdbif.py` & `mypylib-0.1.78/mypylib/chdbif.py`

 * *Files identical despite different names*

### Comparing `mypylib-0.1.77/mypylib/crawler.py` & `mypylib-0.1.78/mypylib/crawler.py`

 * *Files 20% similar despite different names*

```diff
@@ -18,24 +18,34 @@
 headers = {
     'User-Agent': 'Mozilla/5.0 (Windows NT 10.0; Win64; x64) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/70.0.3538.102 Safari/537.36 Edge/18.18362',
 }
 
 
 class crawler_cnyes:
 
-    def __init__(self, datetime_start: datetime.datetime = datetime.datetime.today(), datetime_end: datetime.datetime = datetime.datetime.today() + datetime.timedelta(days=1)):
-        self.datetime_start = datetime_start
-        self.datetime_end = datetime_end
+    def __init__(self, version=1):
+        self.datetime_start = datetime.datetime.today()
+        self.datetime_end = datetime.datetime.today()
 
         self.list_news = []
+        self.version = version
 
     @logger.catch
-    def fetch(self):
-        url = f'https://news.cnyes.com/api/v3/news/category/tw_stock?startAt={int(self.datetime_start.timestamp())}' \
-              f'&endAt={int(self.datetime_end.timestamp())}&limit=50'
+    def fetch(self,
+              datetime_start: datetime.datetime = datetime.datetime.today().replace(hour=0, minute=0, second=0),
+              datetime_end: datetime.datetime = datetime.datetime.today() + datetime.timedelta(days=1)):
+
+        self.datetime_start = datetime_start
+        self.datetime_end = datetime_end
+
+        if self.version == 1:
+            url = f'https://api.cnyes.com/media/api/v1/newslist/category/tw_stock?startAt={int(self.datetime_start.timestamp())}&endAt={int(self.datetime_end.timestamp())}&limit=30'
+        else:
+            url = f'https://news.cnyes.com/api/v3/news/category/tw_stock?startAt={int(self.datetime_start.timestamp())}' \
+                  f'&endAt={int(self.datetime_end.timestamp())}&limit=100'
         logger.info(url)
         res = requests.get(url, headers)
         ret = json.loads(res.text)
 
         list_news = []
         for x in ret['items']['data']:
             title = x['title']
@@ -56,12 +66,17 @@
 
         return list_news_new
 
 
 if __name__ == '__main__':
 
     cynes = crawler_cnyes()
-    while True:
-        sleep(1)
-        ret = cynes.fetch_new()
-        for x in ret:
-            print(x)
+    if False:
+        while True:
+            sleep(1)
+            ret = cynes.fetch_new()
+            for x in ret:
+                print(x)
+    else:
+        news = cynes.fetch()
+        print(news)
+
```

### Comparing `mypylib-0.1.77/mypylib/crypto.py` & `mypylib-0.1.78/mypylib/crypto.py`

 * *Files identical despite different names*

### Comparing `mypylib-0.1.77/mypylib/finmind.py` & `mypylib-0.1.78/mypylib/finmind.py`

 * *Files identical despite different names*

### Comparing `mypylib-0.1.77/mypylib/libexcel.py` & `mypylib-0.1.78/mypylib/libexcel.py`

 * *Files identical despite different names*

### Comparing `mypylib-0.1.77/mypylib/mvp.py` & `mypylib-0.1.78/mypylib/mvp.py`

 * *Files identical despite different names*

### Comparing `mypylib-0.1.77/mypylib/mytest.py` & `mypylib-0.1.78/mypylib/mytest.py`

 * *Files identical despite different names*

### Comparing `mypylib-0.1.77/mypylib/option_test.py` & `mypylib-0.1.78/mypylib/option_test.py`

 * *Files identical despite different names*

### Comparing `mypylib-0.1.77/mypylib/shioaji_history_ticks.py` & `mypylib-0.1.78/mypylib/shioaji_history_ticks.py`

 * *Files identical despite different names*

### Comparing `mypylib-0.1.77/mypylib/shioaji_kline.py` & `mypylib-0.1.78/mypylib/shioaji_kline.py`

 * *Files identical despite different names*

### Comparing `mypylib-0.1.77/mypylib/shioaji_ticks.py` & `mypylib-0.1.78/mypylib/shioaji_ticks.py`

 * *Files identical despite different names*

### Comparing `mypylib-0.1.77/mypylib/sjtools.py` & `mypylib-0.1.78/mypylib/sjtools.py`

 * *Files identical despite different names*

### Comparing `mypylib-0.1.77/mypylib/tLineNotify.py` & `mypylib-0.1.78/mypylib/tLineNotify.py`

 * *Files identical despite different names*

### Comparing `mypylib-0.1.77/mypylib/ti.py` & `mypylib-0.1.78/mypylib/ti.py`

 * *Files identical despite different names*

### Comparing `mypylib-0.1.77/mypylib/tmpDevelopment/warrant_test.py` & `mypylib-0.1.78/mypylib/tmpDevelopment/warrant_test.py`

 * *Files identical despite different names*

### Comparing `mypylib-0.1.77/mypylib/tplaysound.py` & `mypylib-0.1.78/mypylib/tplaysound.py`

 * *Files identical despite different names*

### Comparing `mypylib-0.1.77/mypylib/tredis.py` & `mypylib-0.1.78/mypylib/tredis.py`

 * *Files identical despite different names*

### Comparing `mypylib-0.1.77/mypylib/warrant.py` & `mypylib-0.1.78/mypylib/warrant.py`

 * *Files 2% similar despite different names*

```diff
@@ -212,7 +212,8 @@
     dict_warrant_to_info, dict_stock_to_warrant = read_warrant_bible('權證達人寶典_NEWVOL_2022-12-21.xls')
     list_new_warrants = get_new_warrant_list()
 
     dict_warrant_to_info, dict_stock_to_warrant = add_new_issued_warrant_to_bible(dict_warrant_to_info,
                                                                                   dict_stock_to_warrant,
                                                                                   list_new_warrants,
                                                                                   date_to_filte)
+    print(dict_stock_to_warrant)
```

### Comparing `mypylib-0.1.77/mypylib.egg-info/SOURCES.txt` & `mypylib-0.1.78/mypylib.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mypylib-0.1.77/setup.py` & `mypylib-0.1.78/setup.py`

 * *Files identical despite different names*

