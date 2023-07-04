# Comparing `tmp/crypto-screening-1.9.0.tar.gz` & `tmp/crypto-screening-1.9.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "crypto-screening-1.9.0.tar", last modified: Tue Jul  4 21:38:57 2023, max compression
+gzip compressed data, was "crypto-screening-1.9.1.tar", last modified: Tue Jul  4 22:49:00 2023, max compression
```

## Comparing `crypto-screening-1.9.0.tar` & `crypto-screening-1.9.1.tar`

### file list

```diff
@@ -1,43 +1,43 @@
-drwxrwxrwx   0        0        0        0 2023-07-04 21:38:57.631830 crypto-screening-1.9.0/
--rw-rw-rw-   0        0        0       98 2023-07-04 21:38:55.000000 crypto-screening-1.9.0/MANIFEST.in
--rw-rw-rw-   0        0        0     2059 2023-07-04 21:38:57.631830 crypto-screening-1.9.0/PKG-INFO
--rw-rw-rw-   0        0        0     1238 2023-07-01 07:09:50.000000 crypto-screening-1.9.0/README.md
--rw-rw-rw-   0        0        0    12920 2023-06-23 16:52:27.000000 crypto-screening-1.9.0/build.py
-drwxrwxrwx   0        0        0        0 2023-07-04 21:38:57.566414 crypto-screening-1.9.0/crypto_screening/
-drwxrwxrwx   0        0        0        0 2023-07-04 21:38:57.604860 crypto-screening-1.9.0/crypto_screening/collect/
--rw-rw-rw-   0        0        0    17727 2023-06-30 14:15:11.000000 crypto-screening-1.9.0/crypto_screening/collect/assets.py
--rw-rw-rw-   0        0        0     4056 2023-06-27 13:26:48.000000 crypto-screening-1.9.0/crypto_screening/collect/exchanges.py
--rw-rw-rw-   0        0        0     8905 2023-07-04 21:38:35.000000 crypto-screening-1.9.0/crypto_screening/collect/market.py
--rw-rw-rw-   0        0        0    10119 2023-06-30 15:31:03.000000 crypto-screening-1.9.0/crypto_screening/collect/screeners.py
--rw-rw-rw-   0        0        0    18830 2023-07-03 15:11:08.000000 crypto-screening-1.9.0/crypto_screening/collect/symbols.py
--rw-rw-rw-   0        0        0    12514 2023-06-30 09:18:44.000000 crypto-screening-1.9.0/crypto_screening/dataset.py
--rw-rw-rw-   0        0        0      258 2023-06-25 14:21:21.000000 crypto-screening-1.9.0/crypto_screening/exchanges.py
--rw-rw-rw-   0        0        0     5278 2023-07-03 15:17:16.000000 crypto-screening-1.9.0/crypto_screening/interval.py
-drwxrwxrwx   0        0        0        0 2023-07-04 21:38:57.609863 crypto-screening-1.9.0/crypto_screening/market/
-drwxrwxrwx   0        0        0        0 2023-07-04 21:38:57.612830 crypto-screening-1.9.0/crypto_screening/market/foundation/
--rw-rw-rw-   0        0        0    10765 2023-07-04 21:19:28.000000 crypto-screening-1.9.0/crypto_screening/market/foundation/data.py
--rw-rw-rw-   0        0        0      891 2023-07-04 21:20:28.000000 crypto-screening-1.9.0/crypto_screening/market/foundation/protocols.py
--rw-rw-rw-   0        0        0     1352 2023-07-04 21:19:28.000000 crypto-screening-1.9.0/crypto_screening/market/foundation/state.py
--rw-rw-rw-   0        0        0     6969 2023-07-04 21:21:42.000000 crypto-screening-1.9.0/crypto_screening/market/foundation/waiting.py
-drwxrwxrwx   0        0        0        0 2023-07-04 21:38:57.630866 crypto-screening-1.9.0/crypto_screening/market/screeners/
--rw-rw-rw-   0        0        0      294 2023-06-30 10:45:52.000000 crypto-screening-1.9.0/crypto_screening/market/screeners/__init__.py
--rw-rw-rw-   0        0        0    13531 2023-07-04 21:23:28.000000 crypto-screening-1.9.0/crypto_screening/market/screeners/base.py
--rw-rw-rw-   0        0        0     3255 2023-07-03 15:13:24.000000 crypto-screening-1.9.0/crypto_screening/market/screeners/container.py
--rw-rw-rw-   0        0        0    32767 2023-07-04 21:25:29.000000 crypto-screening-1.9.0/crypto_screening/market/screeners/ohlcv.py
--rw-rw-rw-   0        0        0    24982 2023-07-04 21:26:30.000000 crypto-screening-1.9.0/crypto_screening/market/screeners/orderbook.py
--rw-rw-rw-   0        0        0     5390 2023-07-03 15:12:27.000000 crypto-screening-1.9.0/crypto_screening/market/screeners/recorder.py
--rw-rw-rw-   0        0        0     3839 2023-06-30 09:26:54.000000 crypto-screening-1.9.0/crypto_screening/market/waiting.py
--rw-rw-rw-   0        0        0     2382 2023-06-30 14:15:11.000000 crypto-screening-1.9.0/crypto_screening/process.py
--rw-rw-rw-   0        0        0     9969 2023-07-03 15:16:52.000000 crypto-screening-1.9.0/crypto_screening/symbols.py
--rw-rw-rw-   0        0        0     3845 2023-06-27 09:22:00.000000 crypto-screening-1.9.0/crypto_screening/validate.py
-drwxrwxrwx   0        0        0        0 2023-07-04 21:38:57.582860 crypto-screening-1.9.0/crypto_screening.egg-info/
--rw-rw-rw-   0        0        0     2059 2023-07-04 21:38:57.000000 crypto-screening-1.9.0/crypto_screening.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1132 2023-07-04 21:38:57.000000 crypto-screening-1.9.0/crypto_screening.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-04 21:38:57.000000 crypto-screening-1.9.0/crypto_screening.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       94 2023-07-04 21:38:57.000000 crypto-screening-1.9.0/crypto_screening.egg-info/requires.txt
--rw-rw-rw-   0        0        0       17 2023-07-04 21:38:57.000000 crypto-screening-1.9.0/crypto_screening.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      652 2023-07-04 21:38:55.000000 crypto-screening-1.9.0/pyproject.toml
--rw-rw-rw-   0        0        0       99 2023-06-28 09:56:21.000000 crypto-screening-1.9.0/requirements-dev.txt
--rw-rw-rw-   0        0        0       64 2023-06-23 16:55:08.000000 crypto-screening-1.9.0/requirements.txt
--rw-rw-rw-   0        0        0       42 2023-07-04 21:38:57.631830 crypto-screening-1.9.0/setup.cfg
--rw-rw-rw-   0        0        0     1579 2023-07-04 21:38:51.000000 crypto-screening-1.9.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-04 22:49:00.819798 crypto-screening-1.9.1/
+-rw-rw-rw-   0        0        0       98 2023-07-04 22:49:00.000000 crypto-screening-1.9.1/MANIFEST.in
+-rw-rw-rw-   0        0        0     2059 2023-07-04 22:49:00.819798 crypto-screening-1.9.1/PKG-INFO
+-rw-rw-rw-   0        0        0     1238 2023-07-01 07:09:50.000000 crypto-screening-1.9.1/README.md
+-rw-rw-rw-   0        0        0    12920 2023-06-23 16:52:27.000000 crypto-screening-1.9.1/build.py
+drwxrwxrwx   0        0        0        0 2023-07-04 22:49:00.794879 crypto-screening-1.9.1/crypto_screening/
+drwxrwxrwx   0        0        0        0 2023-07-04 22:49:00.810797 crypto-screening-1.9.1/crypto_screening/collect/
+-rw-rw-rw-   0        0        0    17727 2023-06-30 14:15:11.000000 crypto-screening-1.9.1/crypto_screening/collect/assets.py
+-rw-rw-rw-   0        0        0     4056 2023-06-27 13:26:48.000000 crypto-screening-1.9.1/crypto_screening/collect/exchanges.py
+-rw-rw-rw-   0        0        0     9063 2023-07-04 22:48:40.000000 crypto-screening-1.9.1/crypto_screening/collect/market.py
+-rw-rw-rw-   0        0        0    11717 2023-07-04 22:47:33.000000 crypto-screening-1.9.1/crypto_screening/collect/screeners.py
+-rw-rw-rw-   0        0        0    18830 2023-07-03 15:11:08.000000 crypto-screening-1.9.1/crypto_screening/collect/symbols.py
+-rw-rw-rw-   0        0        0    12514 2023-06-30 09:18:44.000000 crypto-screening-1.9.1/crypto_screening/dataset.py
+-rw-rw-rw-   0        0        0      258 2023-06-25 14:21:21.000000 crypto-screening-1.9.1/crypto_screening/exchanges.py
+-rw-rw-rw-   0        0        0     5278 2023-07-03 15:17:16.000000 crypto-screening-1.9.1/crypto_screening/interval.py
+drwxrwxrwx   0        0        0        0 2023-07-04 22:49:00.811798 crypto-screening-1.9.1/crypto_screening/market/
+drwxrwxrwx   0        0        0        0 2023-07-04 22:49:00.814797 crypto-screening-1.9.1/crypto_screening/market/foundation/
+-rw-rw-rw-   0        0        0    10765 2023-07-04 21:19:28.000000 crypto-screening-1.9.1/crypto_screening/market/foundation/data.py
+-rw-rw-rw-   0        0        0      891 2023-07-04 21:20:28.000000 crypto-screening-1.9.1/crypto_screening/market/foundation/protocols.py
+-rw-rw-rw-   0        0        0     1352 2023-07-04 21:19:28.000000 crypto-screening-1.9.1/crypto_screening/market/foundation/state.py
+-rw-rw-rw-   0        0        0     6969 2023-07-04 21:21:42.000000 crypto-screening-1.9.1/crypto_screening/market/foundation/waiting.py
+drwxrwxrwx   0        0        0        0 2023-07-04 22:49:00.818797 crypto-screening-1.9.1/crypto_screening/market/screeners/
+-rw-rw-rw-   0        0        0      294 2023-06-30 10:45:52.000000 crypto-screening-1.9.1/crypto_screening/market/screeners/__init__.py
+-rw-rw-rw-   0        0        0    13531 2023-07-04 21:23:28.000000 crypto-screening-1.9.1/crypto_screening/market/screeners/base.py
+-rw-rw-rw-   0        0        0     3255 2023-07-03 15:13:24.000000 crypto-screening-1.9.1/crypto_screening/market/screeners/container.py
+-rw-rw-rw-   0        0        0    32767 2023-07-04 21:25:29.000000 crypto-screening-1.9.1/crypto_screening/market/screeners/ohlcv.py
+-rw-rw-rw-   0        0        0    24982 2023-07-04 21:26:30.000000 crypto-screening-1.9.1/crypto_screening/market/screeners/orderbook.py
+-rw-rw-rw-   0        0        0     5390 2023-07-03 15:12:27.000000 crypto-screening-1.9.1/crypto_screening/market/screeners/recorder.py
+-rw-rw-rw-   0        0        0     3839 2023-06-30 09:26:54.000000 crypto-screening-1.9.1/crypto_screening/market/waiting.py
+-rw-rw-rw-   0        0        0     2382 2023-06-30 14:15:11.000000 crypto-screening-1.9.1/crypto_screening/process.py
+-rw-rw-rw-   0        0        0     9969 2023-07-03 15:16:52.000000 crypto-screening-1.9.1/crypto_screening/symbols.py
+-rw-rw-rw-   0        0        0     3845 2023-06-27 09:22:00.000000 crypto-screening-1.9.1/crypto_screening/validate.py
+drwxrwxrwx   0        0        0        0 2023-07-04 22:49:00.807789 crypto-screening-1.9.1/crypto_screening.egg-info/
+-rw-rw-rw-   0        0        0     2059 2023-07-04 22:49:00.000000 crypto-screening-1.9.1/crypto_screening.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1132 2023-07-04 22:49:00.000000 crypto-screening-1.9.1/crypto_screening.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-04 22:49:00.000000 crypto-screening-1.9.1/crypto_screening.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       94 2023-07-04 22:49:00.000000 crypto-screening-1.9.1/crypto_screening.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       17 2023-07-04 22:49:00.000000 crypto-screening-1.9.1/crypto_screening.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      652 2023-07-04 22:49:00.000000 crypto-screening-1.9.1/pyproject.toml
+-rw-rw-rw-   0        0        0       99 2023-06-28 09:56:21.000000 crypto-screening-1.9.1/requirements-dev.txt
+-rw-rw-rw-   0        0        0       64 2023-06-23 16:55:08.000000 crypto-screening-1.9.1/requirements.txt
+-rw-rw-rw-   0        0        0       42 2023-07-04 22:49:00.819798 crypto-screening-1.9.1/setup.cfg
+-rw-rw-rw-   0        0        0     1579 2023-07-04 22:48:54.000000 crypto-screening-1.9.1/setup.py
```

### Comparing `crypto-screening-1.9.0/PKG-INFO` & `crypto-screening-1.9.1/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: crypto-screening
-Version: 1.9.0
+Version: 1.9.1
 Summary: A software for automatically recording real-time crypto exchanges and pairs OHLCV and Orderbook rates.
 Home-page: https://github.com/Shahaf-F-S/crypto-screening
 Author: Shahaf Frank-Shapir
 Author-email: shahaffrs@gmail.com
 License: MIT
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `crypto-screening-1.9.0/README.md` & `crypto-screening-1.9.1/README.md`

 * *Files identical despite different names*

### Comparing `crypto-screening-1.9.0/build.py` & `crypto-screening-1.9.1/build.py`

 * *Files identical despite different names*

### Comparing `crypto-screening-1.9.0/crypto_screening/collect/assets.py` & `crypto-screening-1.9.1/crypto_screening/collect/assets.py`

 * *Files identical despite different names*

### Comparing `crypto-screening-1.9.0/crypto_screening/collect/exchanges.py` & `crypto-screening-1.9.1/crypto_screening/collect/exchanges.py`

 * *Files identical despite different names*

### Comparing `crypto-screening-1.9.0/crypto_screening/collect/market.py` & `crypto-screening-1.9.1/crypto_screening/collect/market.py`

 * *Files 2% similar despite different names*

```diff
@@ -190,28 +190,34 @@
         return symbol_market_price(
             symbol=symbol, prices=self.asks,
             separator=separator, provider=self
         )
     # end ask
 # end MarketState
 
-def assets_market_state(screeners: Optional[Screeners] = None) -> AssetsMarketState:
+def assets_market_state(
+        screeners: Optional[Screeners] = None,
+        separator: Optional[str] = None
+) -> AssetsMarketState:
     """
     Fetches the prices and relations between the assets.
 
     :param screeners: The price screeners.
+    :param separator: The separator of the assets.
 
     :return: The prices of the assets.
     """
 
     bids = {}
     asks = {}
 
     for screener in screeners:
-        base, quote = symbol_to_parts(screener.symbol)
+        base, quote = symbol_to_parts(
+            symbol=screener.symbol, separator=separator
+        )
 
         bids.setdefault(base, {}).setdefault(
             quote, screener.market[BIDS][-1]
         )
         asks.setdefault(base, {}).setdefault(
             quote, screener.market[ASKS][-1]
         )
```

### Comparing `crypto-screening-1.9.0/crypto_screening/collect/screeners.py` & `crypto-screening-1.9.1/crypto_screening/collect/screeners.py`

 * *Files 5% similar despite different names*

```diff
@@ -4,15 +4,16 @@
 from typing import (
     Optional, Dict, Iterable,
     Set, Union, Tuple, List
 )
 
 from crypto_screening.symbols import symbol_to_pair
 from crypto_screening.collect.symbols import (
-    matching_symbol_pair, MarketSymbolSignature
+    matching_symbol_pair, MarketSymbolSignature,
+    exchanges_symbols
 )
 from crypto_screening.market.screeners.base import (
     BaseScreener, BaseMultiScreener
 )
 
 __all__ = [
     "matching_screener_signatures",
@@ -22,15 +23,16 @@
     "find_screeners",
     "structure_screeners",
     "live_screeners",
     "remove_empty_screeners",
     "screeners_exchanges_symbols",
     "structure_exchanges_symbols_screeners",
     "structure_exchanges_symbols_screener",
-    "gather_screeners"
+    "gather_screeners",
+    "exchanges_symbols_screeners"
 ]
 
 AssetMatches = Iterable[Iterable[str]]
 
 def matching_screener_pair(
         screener1: BaseScreener,
         screener2: BaseScreener, /, *,
@@ -342,8 +344,47 @@
 
         elif isinstance(screener, BaseMultiScreener):
             checked_screeners.extend(screener.screeners)
         # end if
     # end for
 
     return checked_screeners
-# end gather_screeners
+# end gather_screeners
+
+def exchanges_symbols_screeners(
+        screeners: Iterable[BaseScreener],
+        exchanges: Optional[Iterable[str]] = None,
+        adjust: Optional[bool] = True,
+        separator: Optional[str] = None,
+        bases: Optional[Union[Dict[str, Iterable[str]], Iterable[str]]] = None,
+        quotes: Optional[Union[Dict[str, Iterable[str]], Iterable[str]]] = None,
+        included: Optional[Union[Dict[str, Iterable[str]], Iterable[str]]] = None,
+        excluded: Optional[Union[Dict[str, Iterable[str]], Iterable[str]]] = None
+) -> List[BaseScreener]:
+    """
+    Collects the symbols from the exchanges.
+
+    :param screeners: The screeners to collect.
+    :param exchanges: The exchanges.
+    :param quotes: The quotes of the asset pairs.
+    :param excluded: The excluded symbols.
+    :param adjust: The value to adjust the invalid exchanges.
+    :param separator: The separator of the assets.
+    :param included: The symbols to include.
+    :param bases: The bases of the asset pairs.
+
+    :return: The data of the exchanges.
+    """
+
+    found_exchanges_symbols = exchanges_symbols(
+        exchanges=exchanges, adjust=adjust, separator=separator,
+        bases=bases, quotes=quotes, included=included, excluded=excluded
+    )
+
+    return [
+        screener for screener in screeners
+        if (
+            (screener.exchange in found_exchanges_symbols) and
+            (screener.symbol in found_exchanges_symbols[screener.exchange])
+        )
+    ]
+# end exchanges_symbols_screeners
```

### Comparing `crypto-screening-1.9.0/crypto_screening/collect/symbols.py` & `crypto-screening-1.9.1/crypto_screening/collect/symbols.py`

 * *Files identical despite different names*

### Comparing `crypto-screening-1.9.0/crypto_screening/dataset.py` & `crypto-screening-1.9.1/crypto_screening/dataset.py`

 * *Files identical despite different names*

### Comparing `crypto-screening-1.9.0/crypto_screening/interval.py` & `crypto-screening-1.9.1/crypto_screening/interval.py`

 * *Files identical despite different names*

### Comparing `crypto-screening-1.9.0/crypto_screening/market/foundation/data.py` & `crypto-screening-1.9.1/crypto_screening/market/foundation/data.py`

 * *Files identical despite different names*

### Comparing `crypto-screening-1.9.0/crypto_screening/market/foundation/protocols.py` & `crypto-screening-1.9.1/crypto_screening/market/foundation/protocols.py`

 * *Files identical despite different names*

### Comparing `crypto-screening-1.9.0/crypto_screening/market/foundation/state.py` & `crypto-screening-1.9.1/crypto_screening/market/foundation/state.py`

 * *Files identical despite different names*

### Comparing `crypto-screening-1.9.0/crypto_screening/market/foundation/waiting.py` & `crypto-screening-1.9.1/crypto_screening/market/foundation/waiting.py`

 * *Files identical despite different names*

### Comparing `crypto-screening-1.9.0/crypto_screening/market/screeners/base.py` & `crypto-screening-1.9.1/crypto_screening/market/screeners/base.py`

 * *Files identical despite different names*

### Comparing `crypto-screening-1.9.0/crypto_screening/market/screeners/container.py` & `crypto-screening-1.9.1/crypto_screening/market/screeners/container.py`

 * *Files identical despite different names*

### Comparing `crypto-screening-1.9.0/crypto_screening/market/screeners/ohlcv.py` & `crypto-screening-1.9.1/crypto_screening/market/screeners/ohlcv.py`

 * *Files identical despite different names*

### Comparing `crypto-screening-1.9.0/crypto_screening/market/screeners/orderbook.py` & `crypto-screening-1.9.1/crypto_screening/market/screeners/orderbook.py`

 * *Files identical despite different names*

### Comparing `crypto-screening-1.9.0/crypto_screening/market/screeners/recorder.py` & `crypto-screening-1.9.1/crypto_screening/market/screeners/recorder.py`

 * *Files identical despite different names*

### Comparing `crypto-screening-1.9.0/crypto_screening/market/waiting.py` & `crypto-screening-1.9.1/crypto_screening/market/waiting.py`

 * *Files identical despite different names*

### Comparing `crypto-screening-1.9.0/crypto_screening/process.py` & `crypto-screening-1.9.1/crypto_screening/process.py`

 * *Files identical despite different names*

### Comparing `crypto-screening-1.9.0/crypto_screening/symbols.py` & `crypto-screening-1.9.1/crypto_screening/symbols.py`

 * *Files identical despite different names*

### Comparing `crypto-screening-1.9.0/crypto_screening/validate.py` & `crypto-screening-1.9.1/crypto_screening/validate.py`

 * *Files identical despite different names*

### Comparing `crypto-screening-1.9.0/crypto_screening.egg-info/PKG-INFO` & `crypto-screening-1.9.1/crypto_screening.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: crypto-screening
-Version: 1.9.0
+Version: 1.9.1
 Summary: A software for automatically recording real-time crypto exchanges and pairs OHLCV and Orderbook rates.
 Home-page: https://github.com/Shahaf-F-S/crypto-screening
 Author: Shahaf Frank-Shapir
 Author-email: shahaffrs@gmail.com
 License: MIT
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `crypto-screening-1.9.0/crypto_screening.egg-info/SOURCES.txt` & `crypto-screening-1.9.1/crypto_screening.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `crypto-screening-1.9.0/setup.py` & `crypto-screening-1.9.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -20,15 +20,15 @@
         exclude=[
             "__pycache__",
             "*.pyc"
         ],
         requirements="requirements.txt",
         dev_requirements="requirements-dev.txt",
         name='crypto-screening',
-        version='1.9.0',
+        version='1.9.1',
         description=(
             "A software for automatically recording "
             "real-time crypto exchanges and pairs "
             "OHLCV and Orderbook rates."
         ),
         license='MIT',
         author="Shahaf Frank-Shapir",
```

