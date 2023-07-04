# Comparing `tmp/crypto-screening-1.9.2.tar.gz` & `tmp/crypto-screening-1.9.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "crypto-screening-1.9.2.tar", last modified: Tue Jul  4 23:00:53 2023, max compression
+gzip compressed data, was "crypto-screening-1.9.3.tar", last modified: Tue Jul  4 23:22:18 2023, max compression
```

## Comparing `crypto-screening-1.9.2.tar` & `crypto-screening-1.9.3.tar`

### file list

```diff
@@ -1,43 +1,43 @@
-drwxrwxrwx   0        0        0        0 2023-07-04 23:00:53.228027 crypto-screening-1.9.2/
--rw-rw-rw-   0        0        0       98 2023-07-04 23:00:52.000000 crypto-screening-1.9.2/MANIFEST.in
--rw-rw-rw-   0        0        0     2059 2023-07-04 23:00:53.228027 crypto-screening-1.9.2/PKG-INFO
--rw-rw-rw-   0        0        0     1238 2023-07-01 07:09:50.000000 crypto-screening-1.9.2/README.md
--rw-rw-rw-   0        0        0    12920 2023-06-23 16:52:27.000000 crypto-screening-1.9.2/build.py
-drwxrwxrwx   0        0        0        0 2023-07-04 23:00:53.202028 crypto-screening-1.9.2/crypto_screening/
-drwxrwxrwx   0        0        0        0 2023-07-04 23:00:53.218028 crypto-screening-1.9.2/crypto_screening/collect/
--rw-rw-rw-   0        0        0    17727 2023-06-30 14:15:11.000000 crypto-screening-1.9.2/crypto_screening/collect/assets.py
--rw-rw-rw-   0        0        0     4056 2023-06-27 13:26:48.000000 crypto-screening-1.9.2/crypto_screening/collect/exchanges.py
--rw-rw-rw-   0        0        0    10145 2023-07-04 23:00:38.000000 crypto-screening-1.9.2/crypto_screening/collect/market.py
--rw-rw-rw-   0        0        0    11717 2023-07-04 22:47:33.000000 crypto-screening-1.9.2/crypto_screening/collect/screeners.py
--rw-rw-rw-   0        0        0    18830 2023-07-03 15:11:08.000000 crypto-screening-1.9.2/crypto_screening/collect/symbols.py
--rw-rw-rw-   0        0        0    12514 2023-06-30 09:18:44.000000 crypto-screening-1.9.2/crypto_screening/dataset.py
--rw-rw-rw-   0        0        0      258 2023-06-25 14:21:21.000000 crypto-screening-1.9.2/crypto_screening/exchanges.py
--rw-rw-rw-   0        0        0     5278 2023-07-03 15:17:16.000000 crypto-screening-1.9.2/crypto_screening/interval.py
-drwxrwxrwx   0        0        0        0 2023-07-04 23:00:53.219028 crypto-screening-1.9.2/crypto_screening/market/
-drwxrwxrwx   0        0        0        0 2023-07-04 23:00:53.222028 crypto-screening-1.9.2/crypto_screening/market/foundation/
--rw-rw-rw-   0        0        0    10765 2023-07-04 21:19:28.000000 crypto-screening-1.9.2/crypto_screening/market/foundation/data.py
--rw-rw-rw-   0        0        0      891 2023-07-04 21:20:28.000000 crypto-screening-1.9.2/crypto_screening/market/foundation/protocols.py
--rw-rw-rw-   0        0        0     1352 2023-07-04 21:19:28.000000 crypto-screening-1.9.2/crypto_screening/market/foundation/state.py
--rw-rw-rw-   0        0        0     6969 2023-07-04 21:21:42.000000 crypto-screening-1.9.2/crypto_screening/market/foundation/waiting.py
-drwxrwxrwx   0        0        0        0 2023-07-04 23:00:53.227028 crypto-screening-1.9.2/crypto_screening/market/screeners/
--rw-rw-rw-   0        0        0      294 2023-06-30 10:45:52.000000 crypto-screening-1.9.2/crypto_screening/market/screeners/__init__.py
--rw-rw-rw-   0        0        0    13531 2023-07-04 21:23:28.000000 crypto-screening-1.9.2/crypto_screening/market/screeners/base.py
--rw-rw-rw-   0        0        0     3255 2023-07-03 15:13:24.000000 crypto-screening-1.9.2/crypto_screening/market/screeners/container.py
--rw-rw-rw-   0        0        0    32767 2023-07-04 21:25:29.000000 crypto-screening-1.9.2/crypto_screening/market/screeners/ohlcv.py
--rw-rw-rw-   0        0        0    24982 2023-07-04 21:26:30.000000 crypto-screening-1.9.2/crypto_screening/market/screeners/orderbook.py
--rw-rw-rw-   0        0        0     5390 2023-07-03 15:12:27.000000 crypto-screening-1.9.2/crypto_screening/market/screeners/recorder.py
--rw-rw-rw-   0        0        0     3839 2023-06-30 09:26:54.000000 crypto-screening-1.9.2/crypto_screening/market/waiting.py
--rw-rw-rw-   0        0        0     2382 2023-06-30 14:15:11.000000 crypto-screening-1.9.2/crypto_screening/process.py
--rw-rw-rw-   0        0        0     9969 2023-07-03 15:16:52.000000 crypto-screening-1.9.2/crypto_screening/symbols.py
--rw-rw-rw-   0        0        0     3845 2023-06-27 09:22:00.000000 crypto-screening-1.9.2/crypto_screening/validate.py
-drwxrwxrwx   0        0        0        0 2023-07-04 23:00:53.214027 crypto-screening-1.9.2/crypto_screening.egg-info/
--rw-rw-rw-   0        0        0     2059 2023-07-04 23:00:53.000000 crypto-screening-1.9.2/crypto_screening.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1132 2023-07-04 23:00:53.000000 crypto-screening-1.9.2/crypto_screening.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-04 23:00:53.000000 crypto-screening-1.9.2/crypto_screening.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       94 2023-07-04 23:00:53.000000 crypto-screening-1.9.2/crypto_screening.egg-info/requires.txt
--rw-rw-rw-   0        0        0       17 2023-07-04 23:00:53.000000 crypto-screening-1.9.2/crypto_screening.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      652 2023-07-04 23:00:52.000000 crypto-screening-1.9.2/pyproject.toml
--rw-rw-rw-   0        0        0       99 2023-06-28 09:56:21.000000 crypto-screening-1.9.2/requirements-dev.txt
--rw-rw-rw-   0        0        0       64 2023-06-23 16:55:08.000000 crypto-screening-1.9.2/requirements.txt
--rw-rw-rw-   0        0        0       42 2023-07-04 23:00:53.228027 crypto-screening-1.9.2/setup.cfg
--rw-rw-rw-   0        0        0     1579 2023-07-04 23:00:44.000000 crypto-screening-1.9.2/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-04 23:22:18.736613 crypto-screening-1.9.3/
+-rw-rw-rw-   0        0        0       98 2023-07-04 23:22:17.000000 crypto-screening-1.9.3/MANIFEST.in
+-rw-rw-rw-   0        0        0     2059 2023-07-04 23:22:18.736613 crypto-screening-1.9.3/PKG-INFO
+-rw-rw-rw-   0        0        0     1238 2023-07-01 07:09:50.000000 crypto-screening-1.9.3/README.md
+-rw-rw-rw-   0        0        0    12920 2023-06-23 16:52:27.000000 crypto-screening-1.9.3/build.py
+drwxrwxrwx   0        0        0        0 2023-07-04 23:22:18.640979 crypto-screening-1.9.3/crypto_screening/
+drwxrwxrwx   0        0        0        0 2023-07-04 23:22:18.670949 crypto-screening-1.9.3/crypto_screening/collect/
+-rw-rw-rw-   0        0        0    17727 2023-06-30 14:15:11.000000 crypto-screening-1.9.3/crypto_screening/collect/assets.py
+-rw-rw-rw-   0        0        0     4056 2023-06-27 13:26:48.000000 crypto-screening-1.9.3/crypto_screening/collect/exchanges.py
+-rw-rw-rw-   0        0        0    10145 2023-07-04 23:00:38.000000 crypto-screening-1.9.3/crypto_screening/collect/market.py
+-rw-rw-rw-   0        0        0    11846 2023-07-04 23:21:46.000000 crypto-screening-1.9.3/crypto_screening/collect/screeners.py
+-rw-rw-rw-   0        0        0    18998 2023-07-04 23:21:46.000000 crypto-screening-1.9.3/crypto_screening/collect/symbols.py
+-rw-rw-rw-   0        0        0    12514 2023-06-30 09:18:44.000000 crypto-screening-1.9.3/crypto_screening/dataset.py
+-rw-rw-rw-   0        0        0      258 2023-06-25 14:21:21.000000 crypto-screening-1.9.3/crypto_screening/exchanges.py
+-rw-rw-rw-   0        0        0     5278 2023-07-03 15:17:16.000000 crypto-screening-1.9.3/crypto_screening/interval.py
+drwxrwxrwx   0        0        0        0 2023-07-04 23:22:18.675979 crypto-screening-1.9.3/crypto_screening/market/
+drwxrwxrwx   0        0        0        0 2023-07-04 23:22:18.697948 crypto-screening-1.9.3/crypto_screening/market/foundation/
+-rw-rw-rw-   0        0        0    10765 2023-07-04 21:19:28.000000 crypto-screening-1.9.3/crypto_screening/market/foundation/data.py
+-rw-rw-rw-   0        0        0      891 2023-07-04 21:20:28.000000 crypto-screening-1.9.3/crypto_screening/market/foundation/protocols.py
+-rw-rw-rw-   0        0        0     1352 2023-07-04 21:19:28.000000 crypto-screening-1.9.3/crypto_screening/market/foundation/state.py
+-rw-rw-rw-   0        0        0     6969 2023-07-04 21:21:42.000000 crypto-screening-1.9.3/crypto_screening/market/foundation/waiting.py
+drwxrwxrwx   0        0        0        0 2023-07-04 23:22:18.735623 crypto-screening-1.9.3/crypto_screening/market/screeners/
+-rw-rw-rw-   0        0        0      294 2023-06-30 10:45:52.000000 crypto-screening-1.9.3/crypto_screening/market/screeners/__init__.py
+-rw-rw-rw-   0        0        0    13531 2023-07-04 21:23:28.000000 crypto-screening-1.9.3/crypto_screening/market/screeners/base.py
+-rw-rw-rw-   0        0        0     3255 2023-07-03 15:13:24.000000 crypto-screening-1.9.3/crypto_screening/market/screeners/container.py
+-rw-rw-rw-   0        0        0    32767 2023-07-04 21:25:29.000000 crypto-screening-1.9.3/crypto_screening/market/screeners/ohlcv.py
+-rw-rw-rw-   0        0        0    24982 2023-07-04 21:26:30.000000 crypto-screening-1.9.3/crypto_screening/market/screeners/orderbook.py
+-rw-rw-rw-   0        0        0     5390 2023-07-03 15:12:27.000000 crypto-screening-1.9.3/crypto_screening/market/screeners/recorder.py
+-rw-rw-rw-   0        0        0     3839 2023-06-30 09:26:54.000000 crypto-screening-1.9.3/crypto_screening/market/waiting.py
+-rw-rw-rw-   0        0        0     2382 2023-06-30 14:15:11.000000 crypto-screening-1.9.3/crypto_screening/process.py
+-rw-rw-rw-   0        0        0     9969 2023-07-03 15:16:52.000000 crypto-screening-1.9.3/crypto_screening/symbols.py
+-rw-rw-rw-   0        0        0     3845 2023-06-27 09:22:00.000000 crypto-screening-1.9.3/crypto_screening/validate.py
+drwxrwxrwx   0        0        0        0 2023-07-04 23:22:18.654948 crypto-screening-1.9.3/crypto_screening.egg-info/
+-rw-rw-rw-   0        0        0     2059 2023-07-04 23:22:18.000000 crypto-screening-1.9.3/crypto_screening.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1132 2023-07-04 23:22:18.000000 crypto-screening-1.9.3/crypto_screening.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-04 23:22:18.000000 crypto-screening-1.9.3/crypto_screening.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       94 2023-07-04 23:22:18.000000 crypto-screening-1.9.3/crypto_screening.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       17 2023-07-04 23:22:18.000000 crypto-screening-1.9.3/crypto_screening.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      652 2023-07-04 23:22:17.000000 crypto-screening-1.9.3/pyproject.toml
+-rw-rw-rw-   0        0        0       99 2023-06-28 09:56:21.000000 crypto-screening-1.9.3/requirements-dev.txt
+-rw-rw-rw-   0        0        0       64 2023-06-23 16:55:08.000000 crypto-screening-1.9.3/requirements.txt
+-rw-rw-rw-   0        0        0       42 2023-07-04 23:22:18.736613 crypto-screening-1.9.3/setup.cfg
+-rw-rw-rw-   0        0        0     1579 2023-07-04 23:22:09.000000 crypto-screening-1.9.3/setup.py
```

### Comparing `crypto-screening-1.9.2/PKG-INFO` & `crypto-screening-1.9.3/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: crypto-screening
-Version: 1.9.2
+Version: 1.9.3
 Summary: A software for automatically recording real-time crypto exchanges and pairs OHLCV and Orderbook rates.
 Home-page: https://github.com/Shahaf-F-S/crypto-screening
 Author: Shahaf Frank-Shapir
 Author-email: shahaffrs@gmail.com
 License: MIT
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `crypto-screening-1.9.2/README.md` & `crypto-screening-1.9.3/README.md`

 * *Files identical despite different names*

### Comparing `crypto-screening-1.9.2/build.py` & `crypto-screening-1.9.3/build.py`

 * *Files identical despite different names*

### Comparing `crypto-screening-1.9.2/crypto_screening/collect/assets.py` & `crypto-screening-1.9.3/crypto_screening/collect/assets.py`

 * *Files identical despite different names*

### Comparing `crypto-screening-1.9.2/crypto_screening/collect/exchanges.py` & `crypto-screening-1.9.3/crypto_screening/collect/exchanges.py`

 * *Files identical despite different names*

### Comparing `crypto-screening-1.9.2/crypto_screening/collect/market.py` & `crypto-screening-1.9.3/crypto_screening/collect/market.py`

 * *Files identical despite different names*

### Comparing `crypto-screening-1.9.2/crypto_screening/collect/screeners.py` & `crypto-screening-1.9.3/crypto_screening/collect/screeners.py`

 * *Files 0% similar despite different names*

```diff
@@ -371,16 +371,21 @@
     :param separator: The separator of the assets.
     :param included: The symbols to include.
     :param bases: The bases of the asset pairs.
 
     :return: The data of the exchanges.
     """
 
+    if exchanges is None:
+        exchanges = []
+    # end if
+
     found_exchanges_symbols = exchanges_symbols(
-        exchanges=exchanges, adjust=adjust, separator=separator,
+        exchanges=set(exchanges) | {screener.exchange for screener in screeners},
+        adjust=adjust, separator=separator,
         bases=bases, quotes=quotes, included=included, excluded=excluded
     )
 
     return [
         screener for screener in screeners
         if (
             (screener.exchange in found_exchanges_symbols) and
```

### Comparing `crypto-screening-1.9.2/crypto_screening/collect/symbols.py` & `crypto-screening-1.9.3/crypto_screening/collect/symbols.py`

 * *Files 0% similar despite different names*

```diff
@@ -369,19 +369,25 @@
     :return: The data of the exchanges.
     """
 
     symbols = all_exchange_symbols(
         exchange=exchange, adjust=adjust, separator=separator
     )
 
-    return exclude_symbols(
-        symbols=include_symbols(
+    symbols = (
+        symbols
+        if all(value is None for value in (included, bases, quotes)) else
+        include_symbols(
             symbols=symbols, included=included,
             bases=bases, quotes=quotes, separator=separator
-        ), excluded=excluded, separator=separator, adjust=adjust
+        )
+    )
+
+    return symbols if excluded is None else exclude_symbols(
+        symbols=symbols, excluded=excluded, separator=separator, adjust=adjust
     )
 # end exchange_symbols
 
 def exchanges_symbols(
         exchanges: Optional[Iterable[str]] = None,
         adjust: Optional[bool] = True,
         separator: Optional[str] = None,
```

### Comparing `crypto-screening-1.9.2/crypto_screening/dataset.py` & `crypto-screening-1.9.3/crypto_screening/dataset.py`

 * *Files identical despite different names*

### Comparing `crypto-screening-1.9.2/crypto_screening/interval.py` & `crypto-screening-1.9.3/crypto_screening/interval.py`

 * *Files identical despite different names*

### Comparing `crypto-screening-1.9.2/crypto_screening/market/foundation/data.py` & `crypto-screening-1.9.3/crypto_screening/market/foundation/data.py`

 * *Files identical despite different names*

### Comparing `crypto-screening-1.9.2/crypto_screening/market/foundation/protocols.py` & `crypto-screening-1.9.3/crypto_screening/market/foundation/protocols.py`

 * *Files identical despite different names*

### Comparing `crypto-screening-1.9.2/crypto_screening/market/foundation/state.py` & `crypto-screening-1.9.3/crypto_screening/market/foundation/state.py`

 * *Files identical despite different names*

### Comparing `crypto-screening-1.9.2/crypto_screening/market/foundation/waiting.py` & `crypto-screening-1.9.3/crypto_screening/market/foundation/waiting.py`

 * *Files identical despite different names*

### Comparing `crypto-screening-1.9.2/crypto_screening/market/screeners/base.py` & `crypto-screening-1.9.3/crypto_screening/market/screeners/base.py`

 * *Files identical despite different names*

### Comparing `crypto-screening-1.9.2/crypto_screening/market/screeners/container.py` & `crypto-screening-1.9.3/crypto_screening/market/screeners/container.py`

 * *Files identical despite different names*

### Comparing `crypto-screening-1.9.2/crypto_screening/market/screeners/ohlcv.py` & `crypto-screening-1.9.3/crypto_screening/market/screeners/ohlcv.py`

 * *Files identical despite different names*

### Comparing `crypto-screening-1.9.2/crypto_screening/market/screeners/orderbook.py` & `crypto-screening-1.9.3/crypto_screening/market/screeners/orderbook.py`

 * *Files identical despite different names*

### Comparing `crypto-screening-1.9.2/crypto_screening/market/screeners/recorder.py` & `crypto-screening-1.9.3/crypto_screening/market/screeners/recorder.py`

 * *Files identical despite different names*

### Comparing `crypto-screening-1.9.2/crypto_screening/market/waiting.py` & `crypto-screening-1.9.3/crypto_screening/market/waiting.py`

 * *Files identical despite different names*

### Comparing `crypto-screening-1.9.2/crypto_screening/process.py` & `crypto-screening-1.9.3/crypto_screening/process.py`

 * *Files identical despite different names*

### Comparing `crypto-screening-1.9.2/crypto_screening/symbols.py` & `crypto-screening-1.9.3/crypto_screening/symbols.py`

 * *Files identical despite different names*

### Comparing `crypto-screening-1.9.2/crypto_screening/validate.py` & `crypto-screening-1.9.3/crypto_screening/validate.py`

 * *Files identical despite different names*

### Comparing `crypto-screening-1.9.2/crypto_screening.egg-info/PKG-INFO` & `crypto-screening-1.9.3/crypto_screening.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: crypto-screening
-Version: 1.9.2
+Version: 1.9.3
 Summary: A software for automatically recording real-time crypto exchanges and pairs OHLCV and Orderbook rates.
 Home-page: https://github.com/Shahaf-F-S/crypto-screening
 Author: Shahaf Frank-Shapir
 Author-email: shahaffrs@gmail.com
 License: MIT
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `crypto-screening-1.9.2/crypto_screening.egg-info/SOURCES.txt` & `crypto-screening-1.9.3/crypto_screening.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `crypto-screening-1.9.2/setup.py` & `crypto-screening-1.9.3/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -20,15 +20,15 @@
         exclude=[
             "__pycache__",
             "*.pyc"
         ],
         requirements="requirements.txt",
         dev_requirements="requirements-dev.txt",
         name='crypto-screening',
-        version='1.9.2',
+        version='1.9.3',
         description=(
             "A software for automatically recording "
             "real-time crypto exchanges and pairs "
             "OHLCV and Orderbook rates."
         ),
         license='MIT',
         author="Shahaf Frank-Shapir",
```

