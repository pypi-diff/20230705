# Comparing `tmp/crypto-screening-1.9.1.tar.gz` & `tmp/crypto-screening-1.9.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "crypto-screening-1.9.1.tar", last modified: Tue Jul  4 22:49:00 2023, max compression
+gzip compressed data, was "crypto-screening-1.9.2.tar", last modified: Tue Jul  4 23:00:53 2023, max compression
```

## Comparing `crypto-screening-1.9.1.tar` & `crypto-screening-1.9.2.tar`

### file list

```diff
@@ -1,43 +1,43 @@
-drwxrwxrwx   0        0        0        0 2023-07-04 22:49:00.819798 crypto-screening-1.9.1/
--rw-rw-rw-   0        0        0       98 2023-07-04 22:49:00.000000 crypto-screening-1.9.1/MANIFEST.in
--rw-rw-rw-   0        0        0     2059 2023-07-04 22:49:00.819798 crypto-screening-1.9.1/PKG-INFO
--rw-rw-rw-   0        0        0     1238 2023-07-01 07:09:50.000000 crypto-screening-1.9.1/README.md
--rw-rw-rw-   0        0        0    12920 2023-06-23 16:52:27.000000 crypto-screening-1.9.1/build.py
-drwxrwxrwx   0        0        0        0 2023-07-04 22:49:00.794879 crypto-screening-1.9.1/crypto_screening/
-drwxrwxrwx   0        0        0        0 2023-07-04 22:49:00.810797 crypto-screening-1.9.1/crypto_screening/collect/
--rw-rw-rw-   0        0        0    17727 2023-06-30 14:15:11.000000 crypto-screening-1.9.1/crypto_screening/collect/assets.py
--rw-rw-rw-   0        0        0     4056 2023-06-27 13:26:48.000000 crypto-screening-1.9.1/crypto_screening/collect/exchanges.py
--rw-rw-rw-   0        0        0     9063 2023-07-04 22:48:40.000000 crypto-screening-1.9.1/crypto_screening/collect/market.py
--rw-rw-rw-   0        0        0    11717 2023-07-04 22:47:33.000000 crypto-screening-1.9.1/crypto_screening/collect/screeners.py
--rw-rw-rw-   0        0        0    18830 2023-07-03 15:11:08.000000 crypto-screening-1.9.1/crypto_screening/collect/symbols.py
--rw-rw-rw-   0        0        0    12514 2023-06-30 09:18:44.000000 crypto-screening-1.9.1/crypto_screening/dataset.py
--rw-rw-rw-   0        0        0      258 2023-06-25 14:21:21.000000 crypto-screening-1.9.1/crypto_screening/exchanges.py
--rw-rw-rw-   0        0        0     5278 2023-07-03 15:17:16.000000 crypto-screening-1.9.1/crypto_screening/interval.py
-drwxrwxrwx   0        0        0        0 2023-07-04 22:49:00.811798 crypto-screening-1.9.1/crypto_screening/market/
-drwxrwxrwx   0        0        0        0 2023-07-04 22:49:00.814797 crypto-screening-1.9.1/crypto_screening/market/foundation/
--rw-rw-rw-   0        0        0    10765 2023-07-04 21:19:28.000000 crypto-screening-1.9.1/crypto_screening/market/foundation/data.py
--rw-rw-rw-   0        0        0      891 2023-07-04 21:20:28.000000 crypto-screening-1.9.1/crypto_screening/market/foundation/protocols.py
--rw-rw-rw-   0        0        0     1352 2023-07-04 21:19:28.000000 crypto-screening-1.9.1/crypto_screening/market/foundation/state.py
--rw-rw-rw-   0        0        0     6969 2023-07-04 21:21:42.000000 crypto-screening-1.9.1/crypto_screening/market/foundation/waiting.py
-drwxrwxrwx   0        0        0        0 2023-07-04 22:49:00.818797 crypto-screening-1.9.1/crypto_screening/market/screeners/
--rw-rw-rw-   0        0        0      294 2023-06-30 10:45:52.000000 crypto-screening-1.9.1/crypto_screening/market/screeners/__init__.py
--rw-rw-rw-   0        0        0    13531 2023-07-04 21:23:28.000000 crypto-screening-1.9.1/crypto_screening/market/screeners/base.py
--rw-rw-rw-   0        0        0     3255 2023-07-03 15:13:24.000000 crypto-screening-1.9.1/crypto_screening/market/screeners/container.py
--rw-rw-rw-   0        0        0    32767 2023-07-04 21:25:29.000000 crypto-screening-1.9.1/crypto_screening/market/screeners/ohlcv.py
--rw-rw-rw-   0        0        0    24982 2023-07-04 21:26:30.000000 crypto-screening-1.9.1/crypto_screening/market/screeners/orderbook.py
--rw-rw-rw-   0        0        0     5390 2023-07-03 15:12:27.000000 crypto-screening-1.9.1/crypto_screening/market/screeners/recorder.py
--rw-rw-rw-   0        0        0     3839 2023-06-30 09:26:54.000000 crypto-screening-1.9.1/crypto_screening/market/waiting.py
--rw-rw-rw-   0        0        0     2382 2023-06-30 14:15:11.000000 crypto-screening-1.9.1/crypto_screening/process.py
--rw-rw-rw-   0        0        0     9969 2023-07-03 15:16:52.000000 crypto-screening-1.9.1/crypto_screening/symbols.py
--rw-rw-rw-   0        0        0     3845 2023-06-27 09:22:00.000000 crypto-screening-1.9.1/crypto_screening/validate.py
-drwxrwxrwx   0        0        0        0 2023-07-04 22:49:00.807789 crypto-screening-1.9.1/crypto_screening.egg-info/
--rw-rw-rw-   0        0        0     2059 2023-07-04 22:49:00.000000 crypto-screening-1.9.1/crypto_screening.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1132 2023-07-04 22:49:00.000000 crypto-screening-1.9.1/crypto_screening.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-04 22:49:00.000000 crypto-screening-1.9.1/crypto_screening.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       94 2023-07-04 22:49:00.000000 crypto-screening-1.9.1/crypto_screening.egg-info/requires.txt
--rw-rw-rw-   0        0        0       17 2023-07-04 22:49:00.000000 crypto-screening-1.9.1/crypto_screening.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      652 2023-07-04 22:49:00.000000 crypto-screening-1.9.1/pyproject.toml
--rw-rw-rw-   0        0        0       99 2023-06-28 09:56:21.000000 crypto-screening-1.9.1/requirements-dev.txt
--rw-rw-rw-   0        0        0       64 2023-06-23 16:55:08.000000 crypto-screening-1.9.1/requirements.txt
--rw-rw-rw-   0        0        0       42 2023-07-04 22:49:00.819798 crypto-screening-1.9.1/setup.cfg
--rw-rw-rw-   0        0        0     1579 2023-07-04 22:48:54.000000 crypto-screening-1.9.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-04 23:00:53.228027 crypto-screening-1.9.2/
+-rw-rw-rw-   0        0        0       98 2023-07-04 23:00:52.000000 crypto-screening-1.9.2/MANIFEST.in
+-rw-rw-rw-   0        0        0     2059 2023-07-04 23:00:53.228027 crypto-screening-1.9.2/PKG-INFO
+-rw-rw-rw-   0        0        0     1238 2023-07-01 07:09:50.000000 crypto-screening-1.9.2/README.md
+-rw-rw-rw-   0        0        0    12920 2023-06-23 16:52:27.000000 crypto-screening-1.9.2/build.py
+drwxrwxrwx   0        0        0        0 2023-07-04 23:00:53.202028 crypto-screening-1.9.2/crypto_screening/
+drwxrwxrwx   0        0        0        0 2023-07-04 23:00:53.218028 crypto-screening-1.9.2/crypto_screening/collect/
+-rw-rw-rw-   0        0        0    17727 2023-06-30 14:15:11.000000 crypto-screening-1.9.2/crypto_screening/collect/assets.py
+-rw-rw-rw-   0        0        0     4056 2023-06-27 13:26:48.000000 crypto-screening-1.9.2/crypto_screening/collect/exchanges.py
+-rw-rw-rw-   0        0        0    10145 2023-07-04 23:00:38.000000 crypto-screening-1.9.2/crypto_screening/collect/market.py
+-rw-rw-rw-   0        0        0    11717 2023-07-04 22:47:33.000000 crypto-screening-1.9.2/crypto_screening/collect/screeners.py
+-rw-rw-rw-   0        0        0    18830 2023-07-03 15:11:08.000000 crypto-screening-1.9.2/crypto_screening/collect/symbols.py
+-rw-rw-rw-   0        0        0    12514 2023-06-30 09:18:44.000000 crypto-screening-1.9.2/crypto_screening/dataset.py
+-rw-rw-rw-   0        0        0      258 2023-06-25 14:21:21.000000 crypto-screening-1.9.2/crypto_screening/exchanges.py
+-rw-rw-rw-   0        0        0     5278 2023-07-03 15:17:16.000000 crypto-screening-1.9.2/crypto_screening/interval.py
+drwxrwxrwx   0        0        0        0 2023-07-04 23:00:53.219028 crypto-screening-1.9.2/crypto_screening/market/
+drwxrwxrwx   0        0        0        0 2023-07-04 23:00:53.222028 crypto-screening-1.9.2/crypto_screening/market/foundation/
+-rw-rw-rw-   0        0        0    10765 2023-07-04 21:19:28.000000 crypto-screening-1.9.2/crypto_screening/market/foundation/data.py
+-rw-rw-rw-   0        0        0      891 2023-07-04 21:20:28.000000 crypto-screening-1.9.2/crypto_screening/market/foundation/protocols.py
+-rw-rw-rw-   0        0        0     1352 2023-07-04 21:19:28.000000 crypto-screening-1.9.2/crypto_screening/market/foundation/state.py
+-rw-rw-rw-   0        0        0     6969 2023-07-04 21:21:42.000000 crypto-screening-1.9.2/crypto_screening/market/foundation/waiting.py
+drwxrwxrwx   0        0        0        0 2023-07-04 23:00:53.227028 crypto-screening-1.9.2/crypto_screening/market/screeners/
+-rw-rw-rw-   0        0        0      294 2023-06-30 10:45:52.000000 crypto-screening-1.9.2/crypto_screening/market/screeners/__init__.py
+-rw-rw-rw-   0        0        0    13531 2023-07-04 21:23:28.000000 crypto-screening-1.9.2/crypto_screening/market/screeners/base.py
+-rw-rw-rw-   0        0        0     3255 2023-07-03 15:13:24.000000 crypto-screening-1.9.2/crypto_screening/market/screeners/container.py
+-rw-rw-rw-   0        0        0    32767 2023-07-04 21:25:29.000000 crypto-screening-1.9.2/crypto_screening/market/screeners/ohlcv.py
+-rw-rw-rw-   0        0        0    24982 2023-07-04 21:26:30.000000 crypto-screening-1.9.2/crypto_screening/market/screeners/orderbook.py
+-rw-rw-rw-   0        0        0     5390 2023-07-03 15:12:27.000000 crypto-screening-1.9.2/crypto_screening/market/screeners/recorder.py
+-rw-rw-rw-   0        0        0     3839 2023-06-30 09:26:54.000000 crypto-screening-1.9.2/crypto_screening/market/waiting.py
+-rw-rw-rw-   0        0        0     2382 2023-06-30 14:15:11.000000 crypto-screening-1.9.2/crypto_screening/process.py
+-rw-rw-rw-   0        0        0     9969 2023-07-03 15:16:52.000000 crypto-screening-1.9.2/crypto_screening/symbols.py
+-rw-rw-rw-   0        0        0     3845 2023-06-27 09:22:00.000000 crypto-screening-1.9.2/crypto_screening/validate.py
+drwxrwxrwx   0        0        0        0 2023-07-04 23:00:53.214027 crypto-screening-1.9.2/crypto_screening.egg-info/
+-rw-rw-rw-   0        0        0     2059 2023-07-04 23:00:53.000000 crypto-screening-1.9.2/crypto_screening.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1132 2023-07-04 23:00:53.000000 crypto-screening-1.9.2/crypto_screening.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-04 23:00:53.000000 crypto-screening-1.9.2/crypto_screening.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       94 2023-07-04 23:00:53.000000 crypto-screening-1.9.2/crypto_screening.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       17 2023-07-04 23:00:53.000000 crypto-screening-1.9.2/crypto_screening.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      652 2023-07-04 23:00:52.000000 crypto-screening-1.9.2/pyproject.toml
+-rw-rw-rw-   0        0        0       99 2023-06-28 09:56:21.000000 crypto-screening-1.9.2/requirements-dev.txt
+-rw-rw-rw-   0        0        0       64 2023-06-23 16:55:08.000000 crypto-screening-1.9.2/requirements.txt
+-rw-rw-rw-   0        0        0       42 2023-07-04 23:00:53.228027 crypto-screening-1.9.2/setup.cfg
+-rw-rw-rw-   0        0        0     1579 2023-07-04 23:00:44.000000 crypto-screening-1.9.2/setup.py
```

### Comparing `crypto-screening-1.9.1/PKG-INFO` & `crypto-screening-1.9.2/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: crypto-screening
-Version: 1.9.1
+Version: 1.9.2
 Summary: A software for automatically recording real-time crypto exchanges and pairs OHLCV and Orderbook rates.
 Home-page: https://github.com/Shahaf-F-S/crypto-screening
 Author: Shahaf Frank-Shapir
 Author-email: shahaffrs@gmail.com
 License: MIT
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `crypto-screening-1.9.1/README.md` & `crypto-screening-1.9.2/README.md`

 * *Files identical despite different names*

### Comparing `crypto-screening-1.9.1/build.py` & `crypto-screening-1.9.2/build.py`

 * *Files identical despite different names*

### Comparing `crypto-screening-1.9.1/crypto_screening/collect/assets.py` & `crypto-screening-1.9.2/crypto_screening/collect/assets.py`

 * *Files identical despite different names*

### Comparing `crypto-screening-1.9.1/crypto_screening/collect/exchanges.py` & `crypto-screening-1.9.2/crypto_screening/collect/exchanges.py`

 * *Files identical despite different names*

### Comparing `crypto-screening-1.9.1/crypto_screening/collect/market.py` & `crypto-screening-1.9.2/crypto_screening/collect/market.py`

 * *Files 8% similar despite different names*

```diff
@@ -8,17 +8,17 @@
 from crypto_screening.market.screeners.base import BaseScreener
 from crypto_screening.dataset import BIDS, ASKS
 from crypto_screening.symbols import symbol_to_parts
 
 __all__ = [
     "assets_market_state",
     "AssetsMarketState",
-    "validate_market_state_prices_symbol",
+    "validate_assets_market_state_prices_symbol",
     "assets_market_state",
-    "symbol_market_price",
+    "assets_market_price",
     "is_symbol_in_market_state_prices",
     "SymbolsMarketState",
     "symbols_market_state"
 ]
 
 AssetsPrices = Dict[str, Dict[str, float]]
 SymbolsPrices = Dict[str, float]
@@ -46,15 +46,15 @@
     if quote not in prices[base]:
         return False
     # end if
 
     return True
 # end is_symbol_in_market_state_prices
 
-def validate_market_state_prices_symbol(
+def validate_assets_market_state_prices_symbol(
         symbol: str,
         prices: AssetsPrices,
         separator: Optional[str] = None,
         provider: Optional[Any] = None
 ) -> None:
     """
     Checks if the symbol is in the prices' data.
@@ -82,17 +82,41 @@
             f"quote asset '{quote}' is not found in the quote "
             f"assets of the '{base}' base asset in the bid prices"
             f"{f' of {provider}' if provider is not None else ''}. "
             f"Found quote assets for the '{base}' base asset in "
             f"the bid prices are: {', '.join(prices[base].keys())}"
         )
     # end if
-# end validate_market_state_prices_symbol
+# end validate_assets_market_state_prices_symbol
 
-def symbol_market_price(
+def validate_symbols_market_state_prices_symbol(
+        symbol: str,
+        prices: SymbolsPrices,
+        provider: Optional[Any] = None
+) -> None:
+    """
+    Checks if the symbol is in the prices' data.
+
+    :param symbol: The symbol to search.
+    :param prices: The price data to process.
+    :param provider: The data provider.
+
+    :return: The validation value.
+    """
+
+    if symbol not in prices:
+        raise ValueError(
+            f"symbol '{symbol}' is not found in bid prices of"
+            f"{f' of {provider}' if provider is not None else ''}. "
+            f"Found symbols for bid prices are: {', '.join(prices.keys())}"
+        )
+    # end if
+# end validate_symbols_market_state_prices_symbol
+
+def assets_market_price(
         symbol: str,
         prices: AssetsPrices,
         separator: Optional[str] = None,
         provider: Optional[Any] = None
 ) -> float:
     """
     Checks if the symbol is in the prices' data.
@@ -101,23 +125,45 @@
     :param separator: The separator of the assets.
     :param prices: The price data to process.
     :param provider: The data provider.
 
     :return: The validation value.
     """
 
-    validate_market_state_prices_symbol(
+    validate_assets_market_state_prices_symbol(
         symbol=symbol, prices=prices,
         separator=separator, provider=provider
     )
 
     base, quote = symbol_to_parts(symbol=symbol, separator=separator)
 
     return float(prices[base][quote])
-# end symbol_market_price
+# end assets_market_price
+
+def symbols_market_price(
+        symbol: str,
+        prices: SymbolsPrices,
+        provider: Optional[Any] = None
+) -> float:
+    """
+    Checks if the symbol is in the prices' data.
+
+    :param symbol: The symbol to search.
+    :param prices: The price data to process.
+    :param provider: The data provider.
+
+    :return: The validation value.
+    """
+
+    validate_symbols_market_state_prices_symbol(
+        symbol=symbol, prices=prices, provider=provider
+    )
+
+    return float(prices[symbol])
+# end symbols_market_price
 
 @dataclass(repr=False, slots=True)
 @represent
 class AssetsMarketState:
     """
     A class to represent the current market state.
 
@@ -167,15 +213,15 @@
 
         :param symbol: The symbol to find its bid price.
         :param separator: The separator of the assets.
 
         :return: The bid price for the symbol.
         """
 
-        return symbol_market_price(
+        return assets_market_price(
             symbol=symbol, prices=self.bids,
             separator=separator, provider=self
         )
     # end bid
 
     def ask(self, symbol: str, separator: Optional[str] = None) -> float:
         """
@@ -183,15 +229,15 @@
 
         :param symbol: The symbol to find its ask price.
         :param separator: The separator of the assets.
 
         :return: The ask price for the symbol.
         """
 
-        return symbol_market_price(
+        return assets_market_price(
             symbol=symbol, prices=self.asks,
             separator=separator, provider=self
         )
     # end ask
 # end MarketState
 
 def assets_market_state(
@@ -253,16 +299,16 @@
 
     >>> from crypto_screening.collect.market import AssetsMarketState
     >>>
     >>> state = assets_market_state(["BTC", "ETH", "LTC"], currency="USDT")
     """
 
     screeners: Screeners
-    bids: AssetsPrices
-    asks: AssetsPrices
+    bids: SymbolsPrices
+    asks: SymbolsPrices
 
     __modifiers__: ClassVar[Modifiers] = Modifiers(
         excluded=["screeners", "bids", "asks"]
     )
 
     def __hash__(self) -> int:
         """
@@ -270,43 +316,39 @@
 
         :return: The hash of the object.
         """
 
         return id(self)
     # end __hash__
 
-    def bid(self, symbol: str, separator: Optional[str] = None) -> float:
+    def bid(self, symbol: str) -> float:
         """
         Returns the bid price for the symbol.
 
         :param symbol: The symbol to find its bid price.
-        :param separator: The separator of the assets.
 
         :return: The bid price for the symbol.
         """
 
-        return symbol_market_price(
-            symbol=symbol, prices=self.bids,
-            separator=separator, provider=self
+        return symbols_market_price(
+            symbol=symbol, prices=self.bids, provider=self
         )
     # end bid
 
-    def ask(self, symbol: str, separator: Optional[str] = None) -> float:
+    def ask(self, symbol: str) -> float:
         """
         Returns the ask price for the symbol.
 
         :param symbol: The symbol to find its ask price.
-        :param separator: The separator of the assets.
 
         :return: The ask price for the symbol.
         """
 
-        return symbol_market_price(
-            symbol=symbol, prices=self.asks,
-            separator=separator, provider=self
+        return symbols_market_price(
+            symbol=symbol, prices=self.asks, provider=self
         )
     # end ask
 # end SymbolsMarketState
 
 def symbols_market_state(screeners: Optional[Screeners] = None) -> SymbolsMarketState:
     """
     Fetches the prices and relations between the assets.
```

### Comparing `crypto-screening-1.9.1/crypto_screening/collect/screeners.py` & `crypto-screening-1.9.2/crypto_screening/collect/screeners.py`

 * *Files identical despite different names*

### Comparing `crypto-screening-1.9.1/crypto_screening/collect/symbols.py` & `crypto-screening-1.9.2/crypto_screening/collect/symbols.py`

 * *Files identical despite different names*

### Comparing `crypto-screening-1.9.1/crypto_screening/dataset.py` & `crypto-screening-1.9.2/crypto_screening/dataset.py`

 * *Files identical despite different names*

### Comparing `crypto-screening-1.9.1/crypto_screening/interval.py` & `crypto-screening-1.9.2/crypto_screening/interval.py`

 * *Files identical despite different names*

### Comparing `crypto-screening-1.9.1/crypto_screening/market/foundation/data.py` & `crypto-screening-1.9.2/crypto_screening/market/foundation/data.py`

 * *Files identical despite different names*

### Comparing `crypto-screening-1.9.1/crypto_screening/market/foundation/protocols.py` & `crypto-screening-1.9.2/crypto_screening/market/foundation/protocols.py`

 * *Files identical despite different names*

### Comparing `crypto-screening-1.9.1/crypto_screening/market/foundation/state.py` & `crypto-screening-1.9.2/crypto_screening/market/foundation/state.py`

 * *Files identical despite different names*

### Comparing `crypto-screening-1.9.1/crypto_screening/market/foundation/waiting.py` & `crypto-screening-1.9.2/crypto_screening/market/foundation/waiting.py`

 * *Files identical despite different names*

### Comparing `crypto-screening-1.9.1/crypto_screening/market/screeners/base.py` & `crypto-screening-1.9.2/crypto_screening/market/screeners/base.py`

 * *Files identical despite different names*

### Comparing `crypto-screening-1.9.1/crypto_screening/market/screeners/container.py` & `crypto-screening-1.9.2/crypto_screening/market/screeners/container.py`

 * *Files identical despite different names*

### Comparing `crypto-screening-1.9.1/crypto_screening/market/screeners/ohlcv.py` & `crypto-screening-1.9.2/crypto_screening/market/screeners/ohlcv.py`

 * *Files identical despite different names*

### Comparing `crypto-screening-1.9.1/crypto_screening/market/screeners/orderbook.py` & `crypto-screening-1.9.2/crypto_screening/market/screeners/orderbook.py`

 * *Files identical despite different names*

### Comparing `crypto-screening-1.9.1/crypto_screening/market/screeners/recorder.py` & `crypto-screening-1.9.2/crypto_screening/market/screeners/recorder.py`

 * *Files identical despite different names*

### Comparing `crypto-screening-1.9.1/crypto_screening/market/waiting.py` & `crypto-screening-1.9.2/crypto_screening/market/waiting.py`

 * *Files identical despite different names*

### Comparing `crypto-screening-1.9.1/crypto_screening/process.py` & `crypto-screening-1.9.2/crypto_screening/process.py`

 * *Files identical despite different names*

### Comparing `crypto-screening-1.9.1/crypto_screening/symbols.py` & `crypto-screening-1.9.2/crypto_screening/symbols.py`

 * *Files identical despite different names*

### Comparing `crypto-screening-1.9.1/crypto_screening/validate.py` & `crypto-screening-1.9.2/crypto_screening/validate.py`

 * *Files identical despite different names*

### Comparing `crypto-screening-1.9.1/crypto_screening.egg-info/PKG-INFO` & `crypto-screening-1.9.2/crypto_screening.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: crypto-screening
-Version: 1.9.1
+Version: 1.9.2
 Summary: A software for automatically recording real-time crypto exchanges and pairs OHLCV and Orderbook rates.
 Home-page: https://github.com/Shahaf-F-S/crypto-screening
 Author: Shahaf Frank-Shapir
 Author-email: shahaffrs@gmail.com
 License: MIT
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `crypto-screening-1.9.1/crypto_screening.egg-info/SOURCES.txt` & `crypto-screening-1.9.2/crypto_screening.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `crypto-screening-1.9.1/pyproject.toml` & `crypto-screening-1.9.2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = 'crypto-screening'
-version = '1.9.1'
+version = '1.9.2'
 description = 'A software for automatically recording real-time crypto exchanges and pairs OHLCV and Orderbook rates.'
 classifiers = [
 	'Intended Audience :: Developers',
 	'License :: OSI Approved :: MIT License',
 	'Programming Language :: Python',
 	'Programming Language :: Python :: 3',
 	'Programming Language :: Python :: 3.8',
```

### Comparing `crypto-screening-1.9.1/setup.py` & `crypto-screening-1.9.2/setup.py`

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
-        version='1.9.1',
+        version='1.9.2',
         description=(
             "A software for automatically recording "
             "real-time crypto exchanges and pairs "
             "OHLCV and Orderbook rates."
         ),
         license='MIT',
         author="Shahaf Frank-Shapir",
```

