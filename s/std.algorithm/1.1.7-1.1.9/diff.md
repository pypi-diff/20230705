# Comparing `tmp/std.algorithm-1.1.7.tar.gz` & `tmp/std.algorithm-1.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "std.algorithm-1.1.7.tar", last modified: Tue Jun 13 06:01:09 2023, max compression
+gzip compressed data, was "std.algorithm-1.1.9.tar", last modified: Wed Jul  5 05:20:51 2023, max compression
```

## Comparing `std.algorithm-1.1.7.tar` & `std.algorithm-1.1.9.tar`

### file list

```diff
@@ -1,29 +1,45 @@
-drwxrwxrwx   0        0        0        0 2023-06-13 06:01:09.891359 std.algorithm-1.1.7/
--rw-rw-rw-   0        0        0      324 2023-06-13 06:01:09.891359 std.algorithm-1.1.7/PKG-INFO
--rw-rw-rw-   0        0        0       47 2022-10-13 00:41:19.000000 std.algorithm-1.1.7/README.md
--rw-rw-rw-   0        0        0      312 2023-06-13 06:01:09.892359 std.algorithm-1.1.7/setup.cfg
--rw-rw-rw-   0        0        0      478 2023-03-01 06:13:36.000000 std.algorithm-1.1.7/setup.py
-drwxrwxrwx   0        0        0        0 2023-06-13 06:01:09.881366 std.algorithm-1.1.7/std/
--rw-rw-rw-   0        0        0    14485 2023-06-05 00:56:34.000000 std.algorithm-1.1.7/std/MySQL.py
--rw-rw-rw-   0        0        0    20878 2023-06-09 00:47:00.000000 std.algorithm-1.1.7/std/__init__.py
--rw-rw-rw-   0        0        0     2276 2023-04-19 00:57:44.000000 std.algorithm-1.1.7/std/combinatorics.py
--rw-rw-rw-   0        0        0     2819 2023-05-15 01:39:31.000000 std.algorithm-1.1.7/std/data.py
--rw-rw-rw-   0        0        0      202 2022-10-13 00:41:19.000000 std.algorithm-1.1.7/std/error.py
--rw-rw-rw-   0        0        0     8575 2023-06-13 06:00:00.000000 std.algorithm-1.1.7/std/file.py
--rw-rw-rw-   0        0        0     1754 2023-03-01 06:13:03.000000 std.algorithm-1.1.7/std/http.py
--rw-rw-rw-   0        0        0    39618 2023-05-24 03:29:48.000000 std.algorithm-1.1.7/std/keras.py
-drwxrwxrwx   0        0        0        0 2023-06-13 06:01:09.887362 std.algorithm-1.1.7/std/lib/
--rw-rw-rw-   0        0        0  2220528 2022-10-21 02:36:11.000000 std.algorithm-1.1.7/std/lib/eigen.dll
--rw-rw-rw-   0        0        0    13812 2023-06-13 03:09:24.000000 std.algorithm-1.1.7/std/nlp.py
--rw-rw-rw-   0        0        0       89 2023-03-07 01:03:31.000000 std.algorithm-1.1.7/std/regexp.py
--rw-rw-rw-   0        0        0      740 2022-10-13 00:41:19.000000 std.algorithm-1.1.7/std/search.py
--rw-rw-rw-   0        0        0    19454 2023-03-08 09:05:45.000000 std.algorithm-1.1.7/std/sets.py
--rw-rw-rw-   0        0        0     1162 2022-10-13 00:41:19.000000 std.algorithm-1.1.7/std/tree.py
--rw-rw-rw-   0        0        0      443 2023-03-16 02:15:53.000000 std.algorithm-1.1.7/std/unicode.py
--rw-rw-rw-   0        0        0    35286 2023-02-02 07:42:54.000000 std.algorithm-1.1.7/std/xml.py
-drwxrwxrwx   0        0        0        0 2023-06-13 06:01:09.886362 std.algorithm-1.1.7/std.algorithm.egg-info/
--rw-rw-rw-   0        0        0      324 2023-06-13 06:01:09.000000 std.algorithm-1.1.7/std.algorithm.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      431 2023-06-13 06:01:09.000000 std.algorithm-1.1.7/std.algorithm.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-13 06:01:09.000000 std.algorithm-1.1.7/std.algorithm.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        6 2023-06-13 06:01:09.000000 std.algorithm-1.1.7/std.algorithm.egg-info/requires.txt
--rw-rw-rw-   0        0        0        4 2023-06-13 06:01:09.000000 std.algorithm-1.1.7/std.algorithm.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-07-05 05:20:51.656270 std.algorithm-1.1.9/
+-rw-rw-rw-   0        0        0     1186 2023-07-05 05:20:51.657269 std.algorithm-1.1.9/PKG-INFO
+-rw-rw-rw-   0        0        0      805 2023-07-05 05:15:57.000000 std.algorithm-1.1.9/README.md
+-rw-rw-rw-   0        0        0      312 2023-07-05 05:20:51.658269 std.algorithm-1.1.9/setup.cfg
+-rw-rw-rw-   0        0        0      598 2023-07-05 03:44:38.000000 std.algorithm-1.1.9/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-05 05:20:51.622336 std.algorithm-1.1.9/std/
+-rw-rw-rw-   0        0        0    15074 2023-06-29 01:01:53.000000 std.algorithm-1.1.9/std/MySQL.py
+-rw-rw-rw-   0        0        0    21080 2023-06-24 23:12:40.000000 std.algorithm-1.1.9/std/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-05 05:20:51.588637 std.algorithm-1.1.9/std/assets/
+drwxrwxrwx   0        0        0        0 2023-07-05 05:20:51.588637 std.algorithm-1.1.9/std/assets/cn/
+drwxrwxrwx   0        0        0        0 2023-07-05 05:20:51.628332 std.algorithm-1.1.9/std/assets/cn/segment/
+-rw-rw-rw-   0        0        0  5809716 2022-08-12 09:27:37.000000 std.algorithm-1.1.9/std/assets/cn/segment/vocab.csv
+drwxrwxrwx   0        0        0        0 2023-07-05 05:20:51.590635 std.algorithm-1.1.9/std/assets/jp/
+drwxrwxrwx   0        0        0        0 2023-07-05 05:20:51.637328 std.algorithm-1.1.9/std/assets/jp/segment/
+-rw-rw-rw-   0        0        0   974268 2021-07-12 00:31:55.000000 std.algorithm-1.1.9/std/assets/jp/segment/vocab.csv
+-rw-rw-rw-   0        0        0     2276 2023-04-19 00:57:44.000000 std.algorithm-1.1.9/std/combinatorics.py
+-rw-rw-rw-   0        0        0    16008 2023-07-05 03:38:56.000000 std.algorithm-1.1.9/std/cpp.py
+-rw-rw-rw-   0        0        0     2819 2023-05-15 01:39:31.000000 std.algorithm-1.1.9/std/data.py
+-rw-rw-rw-   0        0        0      202 2022-10-13 00:41:19.000000 std.algorithm-1.1.9/std/error.py
+-rw-rw-rw-   0        0        0     8575 2023-06-13 06:00:00.000000 std.algorithm-1.1.9/std/file.py
+-rw-rw-rw-   0        0        0     1822 2023-06-29 00:59:34.000000 std.algorithm-1.1.9/std/http.py
+-rw-rw-rw-   0        0        0    40303 2023-06-19 00:45:15.000000 std.algorithm-1.1.9/std/keras.py
+drwxrwxrwx   0        0        0        0 2023-07-05 05:20:51.644323 std.algorithm-1.1.9/std/lib/
+-rw-rw-rw-   0        0        0  2220528 2022-10-21 02:36:11.000000 std.algorithm-1.1.9/std/lib/eigen.dll
+-rw-rw-rw-   0        0        0  1821816 2023-07-05 04:59:41.000000 std.algorithm-1.1.9/std/lib/libeigen.so
+drwxrwxrwx   0        0        0        0 2023-07-05 05:20:51.649322 std.algorithm-1.1.9/std/nlp/
+-rw-rw-rw-   0        0        0      976 2023-07-05 03:24:35.000000 std.algorithm-1.1.9/std/nlp/__init__.py
+-rw-rw-rw-   0        0        0    12833 2023-07-05 03:24:56.000000 std.algorithm-1.1.9/std/nlp/ner.py
+drwxrwxrwx   0        0        0        0 2023-07-05 05:20:51.656270 std.algorithm-1.1.9/std/nlp/segment/
+-rw-rw-rw-   0        0        0        0 2023-07-05 03:49:19.000000 std.algorithm-1.1.9/std/nlp/segment/__init__.py
+-rw-rw-rw-   0        0        0     5960 2023-07-05 03:33:09.000000 std.algorithm-1.1.9/std/nlp/segment/cn.py
+-rw-rw-rw-   0        0        0     2896 2022-12-12 01:11:49.000000 std.algorithm-1.1.9/std/nlp/segment/en.py
+-rw-rw-rw-   0        0        0     6731 2023-07-05 03:42:31.000000 std.algorithm-1.1.9/std/nlp/segment/jp.py
+-rw-rw-rw-   0        0        0       89 2023-03-07 01:03:31.000000 std.algorithm-1.1.9/std/regexp.py
+-rw-rw-rw-   0        0        0      740 2022-10-13 00:41:19.000000 std.algorithm-1.1.9/std/search.py
+-rw-rw-rw-   0        0        0    19454 2023-03-08 09:05:45.000000 std.algorithm-1.1.9/std/sets.py
+-rw-rw-rw-   0        0        0     1162 2022-10-13 00:41:19.000000 std.algorithm-1.1.9/std/tree.py
+-rw-rw-rw-   0        0        0      443 2023-03-16 02:15:53.000000 std.algorithm-1.1.9/std/unicode.py
+-rw-rw-rw-   0        0        0    35286 2023-02-02 07:42:54.000000 std.algorithm-1.1.9/std/xml.py
+drwxrwxrwx   0        0        0        0 2023-07-05 05:20:51.627333 std.algorithm-1.1.9/std.algorithm.egg-info/
+-rw-rw-rw-   0        0        0     1186 2023-07-05 05:20:51.000000 std.algorithm-1.1.9/std.algorithm.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      644 2023-07-05 05:20:51.000000 std.algorithm-1.1.9/std.algorithm.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-05 05:20:51.000000 std.algorithm-1.1.9/std.algorithm.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        6 2023-07-05 05:20:51.000000 std.algorithm-1.1.9/std.algorithm.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        4 2023-07-05 05:20:51.000000 std.algorithm-1.1.9/std.algorithm.egg-info/top_level.txt
```

### Comparing `std.algorithm-1.1.7/std/MySQL.py` & `std.algorithm-1.1.9/std/MySQL.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,29 +6,35 @@
         cursor = self.cursor()
         try:
             cursor.execute("CREATE DATABASE {} DEFAULT CHARACTER SET 'utf8'".format(self.DB_NAME))
         except Exception as err:
             print("Failed creating database: {}".format(err))
 
     def __init__(self):
-        user = os.environ.get('MYSQL_USER', 'prod')
-        password = os.environ.get('MYSQL_PASSWORD', 'prod')
-        host = os.environ.get('MYSQL_HOST', '127.0.0.1')
-        database = os.environ.get('MYSQL_DATABASE', 'axiom')
-        charset = os.environ.get('MYSQL_CHARSET', 'utf8')
+        self.user = os.environ.get('MYSQL_USER', 'prod')
+        self.password = os.environ.get('MYSQL_PASSWORD', 'prod')
+        self.host = os.environ.get('MYSQL_HOST', '127.0.0.1')
+        self.database = os.environ.get('MYSQL_DATABASE', 'axiom')
+        self.charset = os.environ.get('MYSQL_CHARSET', 'utf8')
         try:
-            self.conn = mysql.connector.connect(user=user, password=password, host=host, database=database)
+            self.conn = mysql.connector.connect(**self.kwargs)
         except mysql.connector.errors.ProgrammingError as err:
             print(err.msg)
             m = re.compile("Unknown database '(\w+)'").search(err.msg)
             assert m
-            assert m[1] == database
-            self.conn = mysql.connector.connect(user=user, password=password, host=host, database='mysql')
-            self.execute("create database " + database)
-            self.conn = mysql.connector.connect(user=user, password=password, host=host, database=database)
+            assert m[1] == self.database
+            kwargs = self.kwargs
+            kwargs['database'] = 'mysql'
+            self.conn = mysql.connector.connect(**kwargs)
+            self.execute("create database " + self.database)
+            self.conn = mysql.connector.connect(**self.kwargs)
+
+    @property
+    def kwargs(self):
+        return dict(user=self.user, password=self.password, host=self.host, database=self.database, charset=self.charset)
 
     def cursor(self, **kwargs):
         return self.conn.cursor(**kwargs)
 
     @property
     def wait_timeout(self):
         cursor = self.cursor()
@@ -105,21 +111,30 @@
 
     def desc_oracle(self, table):
         return [args for args in self.query("select column_name,data_type,nullable from all_tab_columns where owner='%s' and table_name='%s'" % (self.conn._con._kwargs['user'], table))]
 
     def desc_table(self, table):
         return [*self.query("desc %s" % table)]
 
+    def __enter__(self):
+        if self.conn is None:
+            self.conn = mysql.connector.connect(**self.kwargs)
+        return self
+
+    def __exit__(self, *args):
+        self.conn.close()
+        self.conn = None 
+
 
 class MySQLConnector(Database):
 
     def __init__(self):
         Database.__init__(self)
         
-    def load_data_from_list(self, table, array, step=10000, replace=False, ignore=False, truncate=False):
+    def load_data_from_list(self, table, array, step=10000, replace=False, ignore=True, truncate=False):
         desc = self.desc_table(table)
         
         has_training_field = False
         
         char_length = [256] * len(desc)
         dtype = [None] * len(desc)
         for i, (Field, Type, *_) in enumerate(desc):
@@ -147,14 +162,16 @@
                 
             for i in range(0, len(lines), step):
                 csv = folder + '/%s-%d.csv' % (table, i)
                 with open(csv, 'w', encoding='utf8') as file:
                     for args in lines[i:i + step]: 
                         if isinstance(args, tuple):
                             args = [*args]
+                        elif isinstance(args, dict):
+                            args = [args.get(Field, '') for Field, *_ in desc]
                             
                         for i, arg in enumerate(args):
                             if isinstance(arg, set):
                                 arg = [*arg]
                                                             
                             if isinstance(arg, (list, tuple)):
                                 arg = std.json_encode(arg)
@@ -163,15 +180,17 @@
                                 arg = std.json_encode(arg)[1:-1]
                             elif isinstance(arg, bytes):
                                 if len(arg) > char_length[i]:
                                     print(args)
                                     print('args[%d] exceeds the allowable length %d' % (i, char_length[i]))
                                     arg = arg[:char_length[i]]
                                     
-                                arg = arg.decode()                                
+                                arg = arg.decode()
+                            elif isinstance(arg, dict):
+                                arg = std.json_encode(std.json_encode(arg))[1:-1]
                             else:
                                 arg = str(arg)
                             
                             if not ignore and (len(arg.encode(encoding='utf8')) if dtype[i] == 'text' else len(arg)) > char_length[i]:
                                 if truncate:
                                     print('truncating the data to maximum length:', char_length[i], ", since its length is", len(arg.encode(encoding='utf8')))
                                     arg = arg[:char_length[i]]
```

### Comparing `std.algorithm-1.1.7/std/__init__.py` & `std.algorithm-1.1.9/std/__init__.py`

 * *Files 3% similar despite different names*

```diff
@@ -749,59 +749,68 @@
         args, = args
         for key, value in args:
             obj[key] = value
 
     return obj
 
 
-def array_split(arr, index):
-    if isinstance(index, int):
-        return arr[:index], arr[index:]
+def array_split(self, pivot):
+    if isinstance(pivot, int):
+        return self[:pivot], self[pivot:]
     
-    if isinstance(index, slice):
-        start, stop, step = index.start, index.stop, index.step
+    if isinstance(pivot, slice):
+        start, stop, step = pivot.start, pivot.stop, pivot.step
         if step is None:
             step = 1
 
         if step > 0:
             if start is None:
                 start = 0
             elif start < 0:
-                start += len(arr)
+                start += len(self)
 
             if stop is None:
-                stop = len(arr)
+                stop = len(self)
             elif stop < 0:
-                stop += len(arr)
+                stop += len(self)
 
             if step > 1:
-                rest = (arr[i] for i in {*range(start, stop)} - {*range(start, stop, step)})
-                rest = arr[:start] + type(arr)(rest) + arr[stop:]
+                rest = (self[i] for i in {*range(start, stop)} - {*range(start, stop, step)})
+                rest = self[:start] + type(self)(rest) + self[stop:]
             else:
-                rest = arr[:start] + arr[stop:]
+                rest = self[:start] + self[stop:]
                 
-            return arr[index], rest
+            return self[pivot], rest
         else:
             if start is None:
-                start = len(arr) - 1
+                start = len(self) - 1
             elif start < 0:
-                start += len(arr)
+                start += len(self)
 
             if stop is None:
                 stop = -1
             elif stop < -1:
-                stop += len(arr)
+                stop += len(self)
             
             if step < -1:
-                rest = (arr[i] for i in {*range(start, stop, -1)} - {*range(start, stop, step)})
-                rest = arr[:stop + 1] + type(arr)(rest) + arr[start + 1:]
+                rest = (self[i] for i in {*range(start, stop, -1)} - {*range(start, stop, step)})
+                rest = self[:stop + 1] + type(self)(rest) + self[start + 1:]
             else:
-                rest = arr[:stop + 1] + arr[start + 1:]
+                rest = self[:stop + 1] + self[start + 1:]
 
-            return rest, arr[index] 
+            return rest, self[pivot] 
+
+    former = []
+    latter = []
+    for arg in self:
+        if pivot(arg):
+            former.append(arg)
+        else:
+            latter.append(arg)
+    return former, latter
 
 
 if __name__ == '__main__':
     arr = [*range(10)]
     former, latter = array_split(arr, slice(-2, -8, -2))
     print(former)
     print(latter)
```

### Comparing `std.algorithm-1.1.7/std/combinatorics.py` & `std.algorithm-1.1.9/std/combinatorics.py`

 * *Files identical despite different names*

### Comparing `std.algorithm-1.1.7/std/data.py` & `std.algorithm-1.1.9/std/data.py`

 * *Files identical despite different names*

### Comparing `std.algorithm-1.1.7/std/file.py` & `std.algorithm-1.1.9/std/file.py`

 * *Files identical despite different names*

### Comparing `std.algorithm-1.1.7/std/http.py` & `std.algorithm-1.1.9/std/http.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,18 +1,21 @@
 import json
 import requests
 from json.decoder import JSONDecodeError
 
 def json_post(url, data):
     try:
-        return json.loads(
-            requests.post(
-                url,
-                data=json.dumps(data, ensure_ascii=False).encode(encoding='utf-8'), 
-                headers={"Content-Type": "application/json"}).text)
+        text = requests.post(
+            url,
+            data=json.dumps(data, ensure_ascii=False).encode(encoding='utf-8'), 
+            headers={"Content-Type": "application/json"}).text
+        try:
+            return json.loads(text)
+        except JSONDecodeError:
+            return text
     except Exception as e:
         return e
 
 
 def json_post_curl(url, data):
     data = json.dumps(data, ensure_ascii=False)#.encode(encoding='utf-8')
     return f"curl -H 'Content-Type: application/json' -X POST '{url}' -d'{data}'"
```

### Comparing `std.algorithm-1.1.7/std/keras.py` & `std.algorithm-1.1.9/std/keras.py`

 * *Files 5% similar despite different names*

```diff
@@ -507,14 +507,38 @@
         return EpochRunner(
             StepRunner(
                 model=self.model, 
                 training=False,
                 device=self.device, 
                 **self.metrics))(generator)
 
+    @std.Timer('predict')
+    def predict(self, inputs, **kwargs):
+        batch_size = kwargs.pop('batch_size', len(inputs))
+        
+        device = self.device
+
+        args = {}
+        if self.is_torch:
+            args['torch'] = True
+        else:
+            args['keras'] = True
+
+        args['sort'] = kwargs.get('sort', False)
+        generator = Sequence(inputs,
+                             batch_size=batch_size,
+                             numpify_x=self.numpify_x,
+                             numpify_y=self.numpify_y, **args)
+        
+        return EpochRunner(
+            StepRunner(
+                model=self.model, 
+                training=False,
+                device=self.device)).predict(generator)
+
     def load_weights(self):
         print('\nloading model from', self.modelFile)
         import h5py
         with h5py.File(self.modelFile, 'r') as f:
             self.iostream(self.model, f, mode='r')
             
     @property
@@ -882,67 +906,16 @@
 
 
 class LambdaCallback(Callback):
     r"""
     Create a simple callback on the fly using lambda functions.
     """
 
-    def __init__(
-        self,
-        on_before_accelerator_backend_setup=None,
-        setup=None,
-        on_configure_sharded_model=None,
-        teardown=None,
-        on_init_start=None,
-        on_init_end=None,
-        on_fit_start=None,
-        on_fit_end=None,
-        on_sanity_check_start=None,
-        on_sanity_check_end=None,
-        on_train_batch_start=None,
-        on_train_batch_end=None,
-        on_train_epoch_start=None,
-        on_train_epoch_end=None,
-        on_validation_epoch_start=None,
-        on_validation_epoch_end=None,
-        on_test_epoch_start=None,
-        on_test_epoch_end=None,
-        on_epoch_start=None,
-        on_epoch_end=None,
-        on_batch_start=None,
-        on_validation_batch_start=None,
-        on_validation_batch_end=None,
-        on_test_batch_start=None,
-        on_test_batch_end=None,
-        on_batch_end=None,
-        on_train_start=None,
-        on_train_end=None,
-        on_pretrain_routine_start=None,
-        on_pretrain_routine_end=None,
-        on_validation_start=None,
-        on_validation_end=None,
-        on_test_start=None,
-        on_test_end=None,
-        on_exception=None,
-        on_save_checkpoint=None,
-        on_load_checkpoint=None,
-        on_before_backward=None,
-        on_after_backward=None,
-        on_before_optimizer_step=None,
-        on_before_zero_grad=None,
-        on_predict_start=None,
-        on_predict_end=None,
-        on_predict_batch_start=None,
-        on_predict_batch_end=None,
-        on_predict_epoch_start=None,
-        on_predict_epoch_end=None,
-    ):
-        for k, v in locals().items():
-            if k == "self":
-                continue
+    def __init__(self, **kwargs):
+        for k, v in kwargs.items():
             if v is not None:
                 setattr(self, k, v)
 
 
 class EpochRunner:
 
     def __init__(self, steprunner):
@@ -982,15 +955,17 @@
                     if isinstance(batch, tuple):
                         batch = [*batch]
 
                     for i, data in enumerate(batch):
                         if isinstance(data, (list, tuple)):
                             data = [data.to(self.device) for data in data]
                         else:
-                            data.to(self.device)
+                            if data.dtype == torch.int:
+                                data = data.long()
+                            data = data.to(self.device)
                         batch[i] = data
                 else:
                     ...
 
             time_start = time.time()
 
             current += 1
@@ -1005,24 +980,30 @@
 
                 except Exception as e:
                     print(e)
                     traceback.print_exc()
                     continue
             else:
                 with torch.no_grad():
-                    loss_per_batch, loss_items, accuracy_items = self.steprunner(*batch)
+                    args = self.steprunner(*batch)
+                    if self.steprunner.loss:
+                        loss_per_batch, loss_items, accuracy_items = args
+                    else:
+                        return args
                    
             if self.is_torch:
                 total_loss += loss_per_batch.sum().item()
                 total_count += loss_per_batch.numel()
             
                 for name, val in loss_items.items():
                     loss_dict[name] += val.sum().item()
                     
                 for name, val in accuracy_items.items():
+                    if val.dtype == torch.bool:
+                        val = val.float()
                     accuracy_dict[name] += val.sum().item()
             else:
                 total_loss += tf.reduce_sum(loss_per_batch).numpy()
                 total_count += loss_per_batch._num_elements()
                 
                 for name, val in loss_items.items():
                     loss_dict[name] += tf.reduce_sum(val).numpy()
@@ -1064,14 +1045,45 @@
             total_time += time.time() - time_start
             ETA = (target - current) * total_time / current
             strs[1] = f'ETA: {print_time(ETA)}'
             print(' - '.join(strs))
             
         return history
 
+    def predict(self, dataloader):
+        
+        if self.is_torch:
+            import torch
+        else:
+            import tensorflow as tf
+            
+        history = []
+        for current, batch in enumerate(dataloader):
+            if self.device >= 0: 
+                if self.is_torch:
+                    if isinstance(batch, tuple):
+                        batch = [*batch]
+
+                    for i, data in enumerate(batch):
+                        if isinstance(data, (list, tuple)):
+                            data = [data.to(self.device) for data in data]
+                        else:
+                            if data.dtype == torch.int:
+                                data = data.long()
+                            data = data.to(self.device)
+                        batch[i] = data
+                else:
+                    ...
+
+            with torch.no_grad():
+                args = self.steprunner(*batch)
+                history.append(args)
+                   
+        return torch.vstack(history)
+
     @property
     def is_torch(self):
         return self.steprunner.is_torch
 
     @property
     def device(self):
         return self.steprunner.device
@@ -1102,43 +1114,46 @@
                 
                 traceback.print_exc()
                 raise e
             except Exception as e:
                 traceback.print_exc()
                 raise e
             
-            if isinstance(self.loss, (list, tuple)):
-                loss_dict = {method_name(loss_fn): loss_fn(y_true, y_pred) for loss_fn, y_true, y_pred in zip(self.loss, y_true, y_pred)}
-            else:
-                loss_dict = {method_name(self.loss): self.loss(y_true, y_pred)}
-    
-            loss = sum(loss_dict.values())
-            # backward()
-            if self.optimizer is not None and self.training:
-                loss_mean = torch.mean(loss)
-            
-                if torch.isnan(loss_mean):
-                    print(loss_mean + 'is nan, stop training')
-                    raise Exception('nan error') 
-            
-                if self.accelerator is None:
-                    loss_mean.backward()
+            if self.loss:
+                if isinstance(self.loss, (list, tuple)):
+                    loss_dict = {method_name(loss_fn): loss_fn(y_true, y_pred) for loss_fn, y_true, y_pred in zip(self.loss, y_true, y_pred)}
                 else:
-                    self.accelerator.backward(loss_mean)
+                    loss_dict = {method_name(self.loss): self.loss(y_true, y_pred)}
     
-                self.optimizer.step()
+                loss = sum(loss_dict.values())
+                # backward()
+                if self.optimizer is not None and self.training:
+                    loss_mean = torch.mean(loss)
                 
-                try:
-                    scheduler = self.optimizer.scheduler
-                    if scheduler is not None:
-                        scheduler.step()# Update learning rate schedule
-                except AttributeError:
-                    ...
+                    if torch.isnan(loss_mean):
+                        print(loss_mean + 'is nan, stop training')
+                        raise Exception('nan error') 
+                
+                    if self.accelerator is None:
+                        loss_mean.backward()
+                    else:
+                        self.accelerator.backward(loss_mean)
+        
+                    self.optimizer.step()
                     
-                self.optimizer.zero_grad()
+                    try:
+                        scheduler = self.optimizer.scheduler
+                        if scheduler is not None:
+                            scheduler.step()# Update learning rate schedule
+                    except AttributeError:
+                        ...
+                        
+                    self.optimizer.zero_grad()
+            else:
+                return y_pred
         else:
             import tensorflow as tf
             with tf.GradientTape() as tape:
                 y_pred = self.model(*features) if isinstance(features, list) else self.model(features)
                
                 if isinstance(self.loss, (list, tuple)):
                     loss_dict = {method_name(loss_fn): loss_fn(y_true, y_pred) for loss_fn, y_true, y_pred in zip(self.loss, y_true, y_pred)}
@@ -1152,15 +1167,14 @@
                     
                     if self.accelerator is None:
                         trainable_variables = self.model.trainable_variables
                         self.optimizer.apply_gradients(zip(tape.gradient(loss_mean, trainable_variables), trainable_variables))
                     else:
                         ...
             
-        # accuracy
         if isinstance(self.accuracy, dict):
             step_metrics = {name: metric_fn(y_true, y_pred) for name, metric_fn in self.accuracy.items()}
         elif isinstance(self.accuracy, (list, tuple)):
             step_metrics = {method_name(metric_fn): metric_fn(y_true, y_pred) for metric_fn, y_true, y_pred in zip(self.accuracy, y_true, y_pred)}
         else:
             step_metrics = {method_name(self.accuracy): self.accuracy(y_true, y_pred)}
```

### Comparing `std.algorithm-1.1.7/std/lib/eigen.dll` & `std.algorithm-1.1.9/std/lib/eigen.dll`

 * *Files identical despite different names*

### Comparing `std.algorithm-1.1.7/std/nlp.py` & `std.algorithm-1.1.9/std/nlp/ner.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,9 @@
-# -*- coding: UTF-8 -*-
 from intervaltree import IntervalTree
 
-
 class Entity2Label:
     def __init__(self, label_schema='BILOU', resolve_conflict=True):
         """
         entity to label transformer
         :param label_schema: label schema, only allow 'BILOU', 'BIO' and None.
                             When its value is none, label will be uppercase of entity type(for semi-markov CRF)
         :param resolve_conflict: whether resolve conflict which entity start or end is not in token starts and ends list
@@ -300,53 +298,7 @@
         msg = 'pos tag count and token text count are not equal, token {}, pos tag {}'
         if pos_tag_count != new_token_count:
             raise Exception(msg.format(new_token_count, pos_tag_count))
         else:
             for token, pos_tag in zip(new_tokens, pos_tags):
                 token['pos_tag'] = pos_tag
     return new_tokens
-
-
-import regex as re
-
-def detect_language(text):
-    if re.compile('\p{Han}{2,}').match(text):
-        return 'cn'
-
-    cn = 0
-    en = 0
-
-    for ch in text:
-        if re.compile('\p{Letter}').match(ch):
-            if re.compile('\p{Han}').match(ch):
-                cn += 2
-            else:
-                en += 1    
-
-        elif re.compile('\p{Number}').match(ch):
-            if ord(ch) > 256:
-                cn += 2
-            else:
-                en += 1
-
-        elif re.compile('\p{Punctuation}').match(ch):
-            if ord(ch) > 256:
-                cn += 2
-            else:
-                en += 1
-
-        elif re.compile('\p{Symbol}').match(ch):
-            ...
-        elif re.compile('\p{Separator}').match(ch):
-            ...
-        elif re.compile('\p{Mark}').match(ch):
-            ...
-        else:
-            ...
-            
-    if cn > en:
-        return 'cn'
-
-    if en > cn:
-        return 'en'
-    
-    return 'en'
```

### Comparing `std.algorithm-1.1.7/std/search.py` & `std.algorithm-1.1.9/std/search.py`

 * *Files identical despite different names*

### Comparing `std.algorithm-1.1.7/std/sets.py` & `std.algorithm-1.1.9/std/sets.py`

 * *Files identical despite different names*

### Comparing `std.algorithm-1.1.7/std/tree.py` & `std.algorithm-1.1.9/std/tree.py`

 * *Files identical despite different names*

### Comparing `std.algorithm-1.1.7/std/xml.py` & `std.algorithm-1.1.9/std/xml.py`

 * *Files identical despite different names*

