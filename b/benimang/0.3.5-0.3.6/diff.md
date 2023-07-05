# Comparing `tmp/benimang-0.3.5.tar.gz` & `tmp/benimang-0.3.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "benimang-0.3.5.tar", last modified: Fri Jun 30 02:16:19 2023, max compression
+gzip compressed data, was "benimang-0.3.6.tar", last modified: Wed Jul  5 03:50:26 2023, max compression
```

## Comparing `benimang-0.3.5.tar` & `benimang-0.3.6.tar`

### file list

```diff
@@ -1,41 +1,41 @@
-drwxrwxrwx   0        0        0        0 2023-06-30 02:16:19.860579 benimang-0.3.5/
--rw-rw-rw-   0        0        0       29 2023-05-30 09:18:28.000000 benimang-0.3.5/MANIFEST.in
--rw-rw-rw-   0        0        0      258 2023-06-30 02:16:19.859580 benimang-0.3.5/PKG-INFO
--rw-rw-rw-   0        0        0        0 2023-05-30 09:18:28.000000 benimang-0.3.5/README.md
-drwxrwxrwx   0        0        0        0 2023-06-30 02:16:19.852579 benimang-0.3.5/beni/
--rw-rw-rw-   0        0        0        0 2023-05-30 09:18:28.000000 benimang-0.3.5/beni/__init__.py
--rw-rw-rw-   0        0        0     6350 2023-06-29 02:15:26.000000 benimang-0.3.5/beni/bbyte.py
--rw-rw-rw-   0        0        0     5783 2023-06-29 07:11:14.000000 benimang-0.3.5/beni/bcache.py
--rw-rw-rw-   0        0        0    11460 2023-06-29 07:06:28.000000 benimang-0.3.5/beni/bcmd.py
--rw-rw-rw-   0        0        0     1941 2023-06-09 08:30:18.000000 benimang-0.3.5/beni/bcolor.py
--rw-rw-rw-   0        0        0      436 2023-06-29 07:09:07.000000 benimang-0.3.5/beni/bdefine.py
--rw-rw-rw-   0        0        0     2423 2023-06-26 06:18:37.000000 benimang-0.3.5/beni/bexecute.py
--rw-rw-rw-   0        0        0     1908 2023-06-29 01:45:33.000000 benimang-0.3.5/beni/bfile.py
--rw-rw-rw-   0        0        0     4482 2023-06-30 02:05:52.000000 benimang-0.3.5/beni/bfunc.py
--rw-rw-rw-   0        0        0     1029 2023-06-28 03:38:59.000000 benimang-0.3.5/beni/bhash.py
--rw-rw-rw-   0        0        0     5745 2023-06-26 09:08:25.000000 benimang-0.3.5/beni/bhttp.py
--rw-rw-rw-   0        0        0     2583 2023-06-13 01:57:12.000000 benimang-0.3.5/beni/binput.py
--rw-rw-rw-   0        0        0     5708 2023-06-30 02:08:08.000000 benimang-0.3.5/beni/block.py
--rw-rw-rw-   0        0        0     3989 2023-06-29 01:25:39.000000 benimang-0.3.5/beni/blog.py
--rw-rw-rw-   0        0        0     5790 2023-06-29 01:32:58.000000 benimang-0.3.5/beni/bpath.py
--rw-rw-rw-   0        0        0     2450 2023-06-29 01:26:10.000000 benimang-0.3.5/beni/bplaywright.py
--rw-rw-rw-   0        0        0     1058 2023-06-27 03:17:47.000000 benimang-0.3.5/beni/bprogress.py
--rw-rw-rw-   0        0        0     3373 2023-06-29 01:32:58.000000 benimang-0.3.5/beni/bqiniu.py
--rw-rw-rw-   0        0        0     9866 2023-06-29 01:31:14.000000 benimang-0.3.5/beni/bsqlite.py
--rw-rw-rw-   0        0        0      759 2023-06-29 01:45:35.000000 benimang-0.3.5/beni/bstorage.py
--rw-rw-rw-   0        0        0     1981 2023-06-26 02:57:46.000000 benimang-0.3.5/beni/btable.py
--rw-rw-rw-   0        0        0     4987 2023-06-29 01:28:43.000000 benimang-0.3.5/beni/btask.py
--rw-rw-rw-   0        0        0     1378 2023-06-29 07:10:32.000000 benimang-0.3.5/beni/btime.py
--rw-rw-rw-   0        0        0      324 2023-06-30 02:01:04.000000 benimang-0.3.5/beni/btype.py
--rw-rw-rw-   0        0        0     2392 2023-06-29 02:21:02.000000 benimang-0.3.5/beni/bzip.py
-drwxrwxrwx   0        0        0        0 2023-06-30 02:16:19.857581 benimang-0.3.5/benimang.egg-info/
--rw-rw-rw-   0        0        0      258 2023-06-30 02:16:19.000000 benimang-0.3.5/benimang.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      625 2023-06-30 02:16:19.000000 benimang-0.3.5/benimang.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-30 02:16:19.000000 benimang-0.3.5/benimang.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       40 2023-06-30 02:16:19.000000 benimang-0.3.5/benimang.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       93 2023-06-30 02:16:19.000000 benimang-0.3.5/benimang.egg-info/requires.txt
--rw-rw-rw-   0        0        0        5 2023-06-30 02:16:19.000000 benimang-0.3.5/benimang.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      567 2023-06-30 02:09:09.000000 benimang-0.3.5/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-06-30 02:16:19.860579 benimang-0.3.5/setup.cfg
-drwxrwxrwx   0        0        0        0 2023-06-30 02:16:19.858580 benimang-0.3.5/test/
--rw-rw-rw-   0        0        0      638 2023-05-30 09:18:28.000000 benimang-0.3.5/test/test_sample.py
+drwxrwxrwx   0        0        0        0 2023-07-05 03:50:26.848979 benimang-0.3.6/
+-rw-rw-rw-   0        0        0       29 2023-05-30 09:18:28.000000 benimang-0.3.6/MANIFEST.in
+-rw-rw-rw-   0        0        0      258 2023-07-05 03:50:26.848979 benimang-0.3.6/PKG-INFO
+-rw-rw-rw-   0        0        0        0 2023-05-30 09:18:28.000000 benimang-0.3.6/README.md
+drwxrwxrwx   0        0        0        0 2023-07-05 03:50:26.841978 benimang-0.3.6/beni/
+-rw-rw-rw-   0        0        0        0 2023-05-30 09:18:28.000000 benimang-0.3.6/beni/__init__.py
+-rw-rw-rw-   0        0        0     6350 2023-06-29 02:15:26.000000 benimang-0.3.6/beni/bbyte.py
+-rw-rw-rw-   0        0        0     5789 2023-07-05 03:38:40.000000 benimang-0.3.6/beni/bcache.py
+-rw-rw-rw-   0        0        0    11460 2023-06-29 07:06:28.000000 benimang-0.3.6/beni/bcmd.py
+-rw-rw-rw-   0        0        0     1941 2023-06-09 08:30:18.000000 benimang-0.3.6/beni/bcolor.py
+-rw-rw-rw-   0        0        0      436 2023-06-29 07:09:07.000000 benimang-0.3.6/beni/bdefine.py
+-rw-rw-rw-   0        0        0     2423 2023-06-26 06:18:37.000000 benimang-0.3.6/beni/bexecute.py
+-rw-rw-rw-   0        0        0     1908 2023-06-29 01:45:33.000000 benimang-0.3.6/beni/bfile.py
+-rw-rw-rw-   0        0        0     4482 2023-06-30 02:05:52.000000 benimang-0.3.6/beni/bfunc.py
+-rw-rw-rw-   0        0        0     1029 2023-06-28 03:38:59.000000 benimang-0.3.6/beni/bhash.py
+-rw-rw-rw-   0        0        0     5745 2023-06-26 09:08:25.000000 benimang-0.3.6/beni/bhttp.py
+-rw-rw-rw-   0        0        0     2583 2023-06-13 01:57:12.000000 benimang-0.3.6/beni/binput.py
+-rw-rw-rw-   0        0        0     5708 2023-06-30 02:08:08.000000 benimang-0.3.6/beni/block.py
+-rw-rw-rw-   0        0        0     3989 2023-06-29 01:25:39.000000 benimang-0.3.6/beni/blog.py
+-rw-rw-rw-   0        0        0     5790 2023-06-29 01:32:58.000000 benimang-0.3.6/beni/bpath.py
+-rw-rw-rw-   0        0        0     2450 2023-06-29 01:26:10.000000 benimang-0.3.6/beni/bplaywright.py
+-rw-rw-rw-   0        0        0     1058 2023-06-27 03:17:47.000000 benimang-0.3.6/beni/bprogress.py
+-rw-rw-rw-   0        0        0     3373 2023-06-29 01:32:58.000000 benimang-0.3.6/beni/bqiniu.py
+-rw-rw-rw-   0        0        0     9866 2023-06-29 01:31:14.000000 benimang-0.3.6/beni/bsqlite.py
+-rw-rw-rw-   0        0        0      759 2023-06-29 01:45:35.000000 benimang-0.3.6/beni/bstorage.py
+-rw-rw-rw-   0        0        0     1981 2023-06-26 02:57:46.000000 benimang-0.3.6/beni/btable.py
+-rw-rw-rw-   0        0        0     4987 2023-06-29 01:28:43.000000 benimang-0.3.6/beni/btask.py
+-rw-rw-rw-   0        0        0     1378 2023-06-29 07:10:32.000000 benimang-0.3.6/beni/btime.py
+-rw-rw-rw-   0        0        0      324 2023-06-30 02:01:04.000000 benimang-0.3.6/beni/btype.py
+-rw-rw-rw-   0        0        0     2392 2023-06-29 02:21:02.000000 benimang-0.3.6/beni/bzip.py
+drwxrwxrwx   0        0        0        0 2023-07-05 03:50:26.846980 benimang-0.3.6/benimang.egg-info/
+-rw-rw-rw-   0        0        0      258 2023-07-05 03:50:26.000000 benimang-0.3.6/benimang.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      625 2023-07-05 03:50:26.000000 benimang-0.3.6/benimang.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-05 03:50:26.000000 benimang-0.3.6/benimang.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       40 2023-07-05 03:50:26.000000 benimang-0.3.6/benimang.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       93 2023-07-05 03:50:26.000000 benimang-0.3.6/benimang.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        5 2023-07-05 03:50:26.000000 benimang-0.3.6/benimang.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      567 2023-07-05 03:49:52.000000 benimang-0.3.6/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-07-05 03:50:26.849980 benimang-0.3.6/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-07-05 03:50:26.847978 benimang-0.3.6/test/
+-rw-rw-rw-   0        0        0      638 2023-05-30 09:18:28.000000 benimang-0.3.6/test/test_sample.py
```

### Comparing `benimang-0.3.5/beni/bbyte.py` & `benimang-0.3.6/beni/bbyte.py`

 * *Files identical despite different names*

### Comparing `benimang-0.3.5/beni/bcache.py` & `benimang-0.3.6/beni/bcache.py`

 * *Files 0% similar despite different names*

```diff
@@ -36,15 +36,15 @@
             await bpath.remove(file)
             self._DEADLINE.clear(key)
             return False
 
     async def get(self, key: str):
         file = self._get_file(key)
         if file.is_file():
-            if self._DEADLINE.valid(key):
+            if await self._DEADLINE.valid(key):
                 return pickle.loads(await bfile.read_bytes(file))
             else:
                 await bpath.remove(file)
         else:
             self._DEADLINE.clear(key)
 
     async def clear(self, key: str):
```

### Comparing `benimang-0.3.5/beni/bcmd.py` & `benimang-0.3.6/beni/bcmd.py`

 * *Files identical despite different names*

### Comparing `benimang-0.3.5/beni/bcolor.py` & `benimang-0.3.6/beni/bcolor.py`

 * *Files identical despite different names*

### Comparing `benimang-0.3.5/beni/bexecute.py` & `benimang-0.3.6/beni/bexecute.py`

 * *Files identical despite different names*

### Comparing `benimang-0.3.5/beni/bfile.py` & `benimang-0.3.6/beni/bfile.py`

 * *Files identical despite different names*

### Comparing `benimang-0.3.5/beni/bfunc.py` & `benimang-0.3.6/beni/bfunc.py`

 * *Files identical despite different names*

### Comparing `benimang-0.3.5/beni/bhash.py` & `benimang-0.3.6/beni/bhash.py`

 * *Files identical despite different names*

### Comparing `benimang-0.3.5/beni/bhttp.py` & `benimang-0.3.6/beni/bhttp.py`

 * *Files identical despite different names*

### Comparing `benimang-0.3.5/beni/binput.py` & `benimang-0.3.6/beni/binput.py`

 * *Files identical despite different names*

### Comparing `benimang-0.3.5/beni/block.py` & `benimang-0.3.6/beni/block.py`

 * *Files identical despite different names*

### Comparing `benimang-0.3.5/beni/blog.py` & `benimang-0.3.6/beni/blog.py`

 * *Files identical despite different names*

### Comparing `benimang-0.3.5/beni/bpath.py` & `benimang-0.3.6/beni/bpath.py`

 * *Files identical despite different names*

### Comparing `benimang-0.3.5/beni/bplaywright.py` & `benimang-0.3.6/beni/bplaywright.py`

 * *Files identical despite different names*

### Comparing `benimang-0.3.5/beni/bprogress.py` & `benimang-0.3.6/beni/bprogress.py`

 * *Files identical despite different names*

### Comparing `benimang-0.3.5/beni/bqiniu.py` & `benimang-0.3.6/beni/bqiniu.py`

 * *Files identical despite different names*

### Comparing `benimang-0.3.5/beni/bsqlite.py` & `benimang-0.3.6/beni/bsqlite.py`

 * *Files identical despite different names*

### Comparing `benimang-0.3.5/beni/bstorage.py` & `benimang-0.3.6/beni/bstorage.py`

 * *Files identical despite different names*

### Comparing `benimang-0.3.5/beni/btable.py` & `benimang-0.3.6/beni/btable.py`

 * *Files identical despite different names*

### Comparing `benimang-0.3.5/beni/btask.py` & `benimang-0.3.6/beni/btask.py`

 * *Files identical despite different names*

### Comparing `benimang-0.3.5/beni/btime.py` & `benimang-0.3.6/beni/btime.py`

 * *Files identical despite different names*

### Comparing `benimang-0.3.5/beni/bzip.py` & `benimang-0.3.6/beni/bzip.py`

 * *Files identical despite different names*

### Comparing `benimang-0.3.5/benimang.egg-info/SOURCES.txt` & `benimang-0.3.6/benimang.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `benimang-0.3.5/pyproject.toml` & `benimang-0.3.6/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 # https://peps.python.org/pep-0621/#example
 
 [project]
 name = "benimang"
-version = "0.3.5"
+version = "0.3.6"
 description = "utils library for Beni"
 requires-python = ">=3.10"
 keywords = ["benimang", "beni"]
 authors = [
   {email = "benimang@126.com"},
   {name = "Beni Mang"}
 ]
```

### Comparing `benimang-0.3.5/test/test_sample.py` & `benimang-0.3.6/test/test_sample.py`

 * *Files identical despite different names*

