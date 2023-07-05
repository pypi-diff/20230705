# Comparing `tmp/crypto-screening-1.9.8.tar.gz` & `tmp/crypto-screening-2.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "crypto-screening-1.9.8.tar", last modified: Wed Jul  5 09:03:44 2023, max compression
+gzip compressed data, was "crypto-screening-2.0.0.tar", last modified: Wed Jul  5 16:38:00 2023, max compression
```

## Comparing `crypto-screening-1.9.8.tar` & `crypto-screening-2.0.0.tar`

### file list

```diff
@@ -1,43 +1,43 @@
-drwxrwxrwx   0        0        0        0 2023-07-05 09:03:44.108627 crypto-screening-1.9.8/
--rw-rw-rw-   0        0        0       98 2023-07-05 09:03:43.000000 crypto-screening-1.9.8/MANIFEST.in
--rw-rw-rw-   0        0        0     2059 2023-07-05 09:03:44.108627 crypto-screening-1.9.8/PKG-INFO
--rw-rw-rw-   0        0        0     1238 2023-07-01 07:09:50.000000 crypto-screening-1.9.8/README.md
--rw-rw-rw-   0        0        0    12920 2023-06-23 16:52:27.000000 crypto-screening-1.9.8/build.py
-drwxrwxrwx   0        0        0        0 2023-07-05 09:03:44.081021 crypto-screening-1.9.8/crypto_screening/
-drwxrwxrwx   0        0        0        0 2023-07-05 09:03:44.098057 crypto-screening-1.9.8/crypto_screening/collect/
--rw-rw-rw-   0        0        0    17727 2023-06-30 14:15:11.000000 crypto-screening-1.9.8/crypto_screening/collect/assets.py
--rw-rw-rw-   0        0        0     4056 2023-06-27 13:26:48.000000 crypto-screening-1.9.8/crypto_screening/collect/exchanges.py
--rw-rw-rw-   0        0        0    25913 2023-07-05 09:03:35.000000 crypto-screening-1.9.8/crypto_screening/collect/market.py
--rw-rw-rw-   0        0        0    11846 2023-07-04 23:21:46.000000 crypto-screening-1.9.8/crypto_screening/collect/screeners.py
--rw-rw-rw-   0        0        0    18998 2023-07-04 23:21:46.000000 crypto-screening-1.9.8/crypto_screening/collect/symbols.py
--rw-rw-rw-   0        0        0    12514 2023-06-30 09:18:44.000000 crypto-screening-1.9.8/crypto_screening/dataset.py
--rw-rw-rw-   0        0        0      258 2023-06-25 14:21:21.000000 crypto-screening-1.9.8/crypto_screening/exchanges.py
--rw-rw-rw-   0        0        0     5278 2023-07-03 15:17:16.000000 crypto-screening-1.9.8/crypto_screening/interval.py
-drwxrwxrwx   0        0        0        0 2023-07-05 09:03:44.099036 crypto-screening-1.9.8/crypto_screening/market/
-drwxrwxrwx   0        0        0        0 2023-07-05 09:03:44.102064 crypto-screening-1.9.8/crypto_screening/market/foundation/
--rw-rw-rw-   0        0        0    10765 2023-07-04 21:19:28.000000 crypto-screening-1.9.8/crypto_screening/market/foundation/data.py
--rw-rw-rw-   0        0        0      891 2023-07-04 21:20:28.000000 crypto-screening-1.9.8/crypto_screening/market/foundation/protocols.py
--rw-rw-rw-   0        0        0     1352 2023-07-04 21:19:28.000000 crypto-screening-1.9.8/crypto_screening/market/foundation/state.py
--rw-rw-rw-   0        0        0     6969 2023-07-04 21:21:42.000000 crypto-screening-1.9.8/crypto_screening/market/foundation/waiting.py
-drwxrwxrwx   0        0        0        0 2023-07-05 09:03:44.107620 crypto-screening-1.9.8/crypto_screening/market/screeners/
--rw-rw-rw-   0        0        0      294 2023-06-30 10:45:52.000000 crypto-screening-1.9.8/crypto_screening/market/screeners/__init__.py
--rw-rw-rw-   0        0        0    13531 2023-07-04 21:23:28.000000 crypto-screening-1.9.8/crypto_screening/market/screeners/base.py
--rw-rw-rw-   0        0        0     3255 2023-07-03 15:13:24.000000 crypto-screening-1.9.8/crypto_screening/market/screeners/container.py
--rw-rw-rw-   0        0        0    32767 2023-07-04 21:25:29.000000 crypto-screening-1.9.8/crypto_screening/market/screeners/ohlcv.py
--rw-rw-rw-   0        0        0    24982 2023-07-04 21:26:30.000000 crypto-screening-1.9.8/crypto_screening/market/screeners/orderbook.py
--rw-rw-rw-   0        0        0     5390 2023-07-03 15:12:27.000000 crypto-screening-1.9.8/crypto_screening/market/screeners/recorder.py
--rw-rw-rw-   0        0        0     3839 2023-06-30 09:26:54.000000 crypto-screening-1.9.8/crypto_screening/market/waiting.py
--rw-rw-rw-   0        0        0     2382 2023-06-30 14:15:11.000000 crypto-screening-1.9.8/crypto_screening/process.py
--rw-rw-rw-   0        0        0     9969 2023-07-03 15:16:52.000000 crypto-screening-1.9.8/crypto_screening/symbols.py
--rw-rw-rw-   0        0        0     3845 2023-06-27 09:22:00.000000 crypto-screening-1.9.8/crypto_screening/validate.py
-drwxrwxrwx   0        0        0        0 2023-07-05 09:03:44.094067 crypto-screening-1.9.8/crypto_screening.egg-info/
--rw-rw-rw-   0        0        0     2059 2023-07-05 09:03:44.000000 crypto-screening-1.9.8/crypto_screening.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1132 2023-07-05 09:03:44.000000 crypto-screening-1.9.8/crypto_screening.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-05 09:03:44.000000 crypto-screening-1.9.8/crypto_screening.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       94 2023-07-05 09:03:44.000000 crypto-screening-1.9.8/crypto_screening.egg-info/requires.txt
--rw-rw-rw-   0        0        0       17 2023-07-05 09:03:44.000000 crypto-screening-1.9.8/crypto_screening.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      652 2023-07-05 09:03:43.000000 crypto-screening-1.9.8/pyproject.toml
--rw-rw-rw-   0        0        0       99 2023-06-28 09:56:21.000000 crypto-screening-1.9.8/requirements-dev.txt
--rw-rw-rw-   0        0        0       64 2023-06-23 16:55:08.000000 crypto-screening-1.9.8/requirements.txt
--rw-rw-rw-   0        0        0       42 2023-07-05 09:03:44.108627 crypto-screening-1.9.8/setup.cfg
--rw-rw-rw-   0        0        0     1579 2023-07-05 09:03:40.000000 crypto-screening-1.9.8/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-05 16:38:00.771188 crypto-screening-2.0.0/
+-rw-rw-rw-   0        0        0       98 2023-07-05 16:37:58.000000 crypto-screening-2.0.0/MANIFEST.in
+-rw-rw-rw-   0        0        0     2059 2023-07-05 16:38:00.771188 crypto-screening-2.0.0/PKG-INFO
+-rw-rw-rw-   0        0        0     1238 2023-07-01 07:09:50.000000 crypto-screening-2.0.0/README.md
+-rw-rw-rw-   0        0        0    12920 2023-06-23 16:52:27.000000 crypto-screening-2.0.0/build.py
+drwxrwxrwx   0        0        0        0 2023-07-05 16:38:00.664308 crypto-screening-2.0.0/crypto_screening/
+drwxrwxrwx   0        0        0        0 2023-07-05 16:38:00.701373 crypto-screening-2.0.0/crypto_screening/collect/
+-rw-rw-rw-   0        0        0    17727 2023-06-30 14:15:11.000000 crypto-screening-2.0.0/crypto_screening/collect/assets.py
+-rw-rw-rw-   0        0        0     4056 2023-06-27 13:26:48.000000 crypto-screening-2.0.0/crypto_screening/collect/exchanges.py
+-rw-rw-rw-   0        0        0    32354 2023-07-05 16:37:05.000000 crypto-screening-2.0.0/crypto_screening/collect/market.py
+-rw-rw-rw-   0        0        0    11846 2023-07-04 23:21:46.000000 crypto-screening-2.0.0/crypto_screening/collect/screeners.py
+-rw-rw-rw-   0        0        0    18998 2023-07-04 23:21:46.000000 crypto-screening-2.0.0/crypto_screening/collect/symbols.py
+-rw-rw-rw-   0        0        0    12514 2023-06-30 09:18:44.000000 crypto-screening-2.0.0/crypto_screening/dataset.py
+-rw-rw-rw-   0        0        0      258 2023-06-25 14:21:21.000000 crypto-screening-2.0.0/crypto_screening/exchanges.py
+-rw-rw-rw-   0        0        0     5278 2023-07-03 15:17:16.000000 crypto-screening-2.0.0/crypto_screening/interval.py
+drwxrwxrwx   0        0        0        0 2023-07-05 16:38:00.706374 crypto-screening-2.0.0/crypto_screening/market/
+drwxrwxrwx   0        0        0        0 2023-07-05 16:38:00.730043 crypto-screening-2.0.0/crypto_screening/market/foundation/
+-rw-rw-rw-   0        0        0    10765 2023-07-04 21:19:28.000000 crypto-screening-2.0.0/crypto_screening/market/foundation/data.py
+-rw-rw-rw-   0        0        0      891 2023-07-04 21:20:28.000000 crypto-screening-2.0.0/crypto_screening/market/foundation/protocols.py
+-rw-rw-rw-   0        0        0     1352 2023-07-04 21:19:28.000000 crypto-screening-2.0.0/crypto_screening/market/foundation/state.py
+-rw-rw-rw-   0        0        0     6969 2023-07-04 21:21:42.000000 crypto-screening-2.0.0/crypto_screening/market/foundation/waiting.py
+drwxrwxrwx   0        0        0        0 2023-07-05 16:38:00.770218 crypto-screening-2.0.0/crypto_screening/market/screeners/
+-rw-rw-rw-   0        0        0      294 2023-06-30 10:45:52.000000 crypto-screening-2.0.0/crypto_screening/market/screeners/__init__.py
+-rw-rw-rw-   0        0        0    13531 2023-07-04 21:23:28.000000 crypto-screening-2.0.0/crypto_screening/market/screeners/base.py
+-rw-rw-rw-   0        0        0     3255 2023-07-03 15:13:24.000000 crypto-screening-2.0.0/crypto_screening/market/screeners/container.py
+-rw-rw-rw-   0        0        0    32767 2023-07-04 21:25:29.000000 crypto-screening-2.0.0/crypto_screening/market/screeners/ohlcv.py
+-rw-rw-rw-   0        0        0    24982 2023-07-04 21:26:30.000000 crypto-screening-2.0.0/crypto_screening/market/screeners/orderbook.py
+-rw-rw-rw-   0        0        0     5390 2023-07-03 15:12:27.000000 crypto-screening-2.0.0/crypto_screening/market/screeners/recorder.py
+-rw-rw-rw-   0        0        0     3839 2023-06-30 09:26:54.000000 crypto-screening-2.0.0/crypto_screening/market/waiting.py
+-rw-rw-rw-   0        0        0     2382 2023-06-30 14:15:11.000000 crypto-screening-2.0.0/crypto_screening/process.py
+-rw-rw-rw-   0        0        0     9969 2023-07-03 15:16:52.000000 crypto-screening-2.0.0/crypto_screening/symbols.py
+-rw-rw-rw-   0        0        0     3845 2023-06-27 09:22:00.000000 crypto-screening-2.0.0/crypto_screening/validate.py
+drwxrwxrwx   0        0        0        0 2023-07-05 16:38:00.678851 crypto-screening-2.0.0/crypto_screening.egg-info/
+-rw-rw-rw-   0        0        0     2059 2023-07-05 16:38:00.000000 crypto-screening-2.0.0/crypto_screening.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1132 2023-07-05 16:38:00.000000 crypto-screening-2.0.0/crypto_screening.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-05 16:38:00.000000 crypto-screening-2.0.0/crypto_screening.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       94 2023-07-05 16:38:00.000000 crypto-screening-2.0.0/crypto_screening.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       17 2023-07-05 16:38:00.000000 crypto-screening-2.0.0/crypto_screening.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      652 2023-07-05 16:37:58.000000 crypto-screening-2.0.0/pyproject.toml
+-rw-rw-rw-   0        0        0       99 2023-06-28 09:56:21.000000 crypto-screening-2.0.0/requirements-dev.txt
+-rw-rw-rw-   0        0        0       64 2023-06-23 16:55:08.000000 crypto-screening-2.0.0/requirements.txt
+-rw-rw-rw-   0        0        0       42 2023-07-05 16:38:00.771188 crypto-screening-2.0.0/setup.cfg
+-rw-rw-rw-   0        0        0     1579 2023-07-05 16:37:53.000000 crypto-screening-2.0.0/setup.py
```

### Comparing `crypto-screening-1.9.8/PKG-INFO` & `crypto-screening-2.0.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: crypto-screening
-Version: 1.9.8
+Version: 2.0.0
 Summary: A software for automatically recording real-time crypto exchanges and pairs OHLCV and Orderbook rates.
 Home-page: https://github.com/Shahaf-F-S/crypto-screening
 Author: Shahaf Frank-Shapir
 Author-email: shahaffrs@gmail.com
 License: MIT
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `crypto-screening-1.9.8/README.md` & `crypto-screening-2.0.0/README.md`

 * *Files identical despite different names*

### Comparing `crypto-screening-1.9.8/build.py` & `crypto-screening-2.0.0/build.py`

 * *Files identical despite different names*

### Comparing `crypto-screening-1.9.8/crypto_screening/collect/assets.py` & `crypto-screening-2.0.0/crypto_screening/collect/assets.py`

 * *Files identical despite different names*

### Comparing `crypto-screening-1.9.8/crypto_screening/collect/exchanges.py` & `crypto-screening-2.0.0/crypto_screening/collect/exchanges.py`

 * *Files identical despite different names*

### Comparing `crypto-screening-1.9.8/crypto_screening/collect/market.py` & `crypto-screening-2.0.0/crypto_screening/collect/market.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,72 +1,130 @@
 # market.py
 
 from dataclasses import dataclass
+from abc import ABCMeta
 from typing import (
-    Iterable, Dict, Optional, Union, Any, ClassVar, List
+    Iterable, Dict, Optional, Union,
+    Any, ClassVar, List
 )
 
 from represent import represent, Modifiers
 
+import numpy as np
+
 from crypto_screening.market.screeners.base import BaseScreener
 from crypto_screening.dataset import BIDS, ASKS
 from crypto_screening.symbols import symbol_to_parts
 
 __all__ = [
     "assets_market_state",
     "AssetsMarketState",
     "validate_assets_market_state_prices_symbol",
     "assets_market_state",
     "assets_market_price",
-    "is_symbol_in_market_state_prices",
+    "is_symbol_in_assets_market_prices",
     "SymbolsMarketState",
     "symbols_market_state",
     "symbols_market_price_sequence",
     "symbols_market_states",
     "symbols_market_price",
     "merge_assets_market_states",
     "merge_symbols_market_states",
     "assets_market_price_sequence",
     "validate_symbols_market_state_prices_symbol",
     "assets_market_states",
     "AssetsMarketStates",
-    "SymbolsMarketStates"
+    "SymbolsMarketStates",
+    "is_exchange_in_market_prices",
+    "is_symbol_in_symbols_market_prices"
 ]
 
 AssetsPrices = Dict[str, Dict[str, Dict[str, float]]]
 SymbolsPrices = Dict[str, Dict[str, float]]
 AssetsPricesSequence = Dict[str, Dict[str, Dict[str, List[float]]]]
 SymbolsPricesSequence = Dict[str, Dict[str, List[float]]]
-Screeners = Union[Iterable[BaseScreener], Dict[str, BaseScreener]]
 
-def is_symbol_in_market_state_prices(
-        symbol: str, prices: AssetsPrices, separator: Optional[str] = None
+def is_exchange_in_market_prices(
+        exchange: str,
+        prices: Union[
+            AssetsPrices, AssetsPricesSequence,
+            SymbolsPrices, SymbolsPricesSequence
+        ]
+) -> None:
+    """
+    Checks if the exchange is in the prices.
+
+    :param exchange: The exchange name.
+    :param prices: The prices.
+
+    :return: The boolean flag.
+    """
+
+    return exchange not in prices
+# end is_exchange_in_market_prices
+
+def is_symbol_in_assets_market_prices(
+        exchange: str,
+        symbol: str,
+        prices: Union[AssetsPrices, AssetsPricesSequence],
+        separator: Optional[str] = None
 ) -> bool:
     """
     Checks if the symbol is in the prices' data.
 
+    :param exchange: The exchange name.
     :param symbol: The symbol to search.
     :param prices: The price data to process.
     :param separator: The separator of the assets.
 
     :return: The validation value.
     """
 
+    if not is_exchange_in_market_prices(exchange=exchange, prices=prices):
+        return False
+    # end if
+
     base, quote = symbol_to_parts(symbol=symbol, separator=separator)
 
-    if base not in prices:
+    if base not in prices[exchange]:
         return False
     # end if
 
-    if quote not in prices[base]:
+    if quote not in prices[exchange][base]:
         return False
     # end if
 
-    return True
-# end is_symbol_in_market_state_prices
+    return not np.isnan(prices[exchange][base][quote])
+# end is_symbol_in_assets_market_prices
+
+def is_symbol_in_symbols_market_prices(
+        exchange: str,
+        symbol: str,
+        prices: Union[SymbolsPrices, SymbolsPricesSequence]
+) -> bool:
+    """
+    Checks if the symbol is in the prices' data.
+
+    :param exchange: The exchange name.
+    :param symbol: The symbol to search.
+    :param prices: The price data to process.
+
+    :return: The validation value.
+    """
+
+    if not is_exchange_in_market_prices(exchange=exchange, prices=prices):
+        return False
+    # end if
+
+    if symbol not in prices[exchange]:
+        return False
+    # end if
+
+    return not np.isnan(prices[exchange][symbol])
+# end is_symbol_in_assets_market_prices
 
 def validate_assets_market_state_prices_symbol(
         exchange: str,
         symbol: str,
         prices: Union[AssetsPrices, AssetsPricesSequence],
         separator: Optional[str] = None,
         provider: Optional[Any] = None
@@ -93,15 +151,16 @@
         )
     # end if
 
     if base not in prices[exchange]:
         raise ValueError(
             f"base asset '{base}' is not found in '{exchange}' prices of"
             f"{f' of {provider}' if provider is not None else ''}. "
-            f"Found base '{exchange}' assets are: {', '.join(prices[exchange].keys())}"
+            f"Found base '{exchange}' assets are: "
+            f"{', '.join(prices[exchange].keys())}"
         )
     # end if
 
     if quote not in prices[exchange][base]:
         raise ValueError(
             f"quote asset '{quote}' is not found in the quote "
             f"assets of the '{base}' base asset in the prices"
@@ -199,57 +258,147 @@
     )
 
     return float(prices[exchange][symbol])
 # end symbols_market_price
 
 @dataclass(repr=False, slots=True)
 @represent
-class AssetsMarketState:
+class AssetsMarketBase(metaclass=ABCMeta):
     """
     A class to represent the current market state.
 
     This object contains the state of the market, as Close,
     bids and asks prices of specific assets, gathered from the network.
 
     attributes:
 
     - screeners:
         The screener objects to collect the prices of the assets.
+    """
 
-    - prices:
-        The close price of the assets.
+    screeners: Iterable[BaseScreener]
+
+    __modifiers__: ClassVar[Modifiers] = Modifiers(excluded=["screeners"])
+
+    def __hash__(self) -> int:
+        """
+        Returns the hash of the object.
+
+        :return: The hash of the object.
+        """
+
+        return id(self)
+    # end __hash__
+
+    def in_bids_prices(
+            self,
+            exchange: str,
+            symbol: str,
+            separator: Optional[str] = None
+    ) -> bool:
+        """
+        Checks if the symbol is in the prices' data.
+
+        :param exchange: The exchange name.
+        :param symbol: The symbol to search.
+        :param separator: The separator of the assets.
+
+        :return: The validation value.
+        """
+
+        return is_symbol_in_assets_market_prices(
+            exchange=exchange, symbol=symbol,
+            separator=separator, prices=self.bids
+        )
+    # end in_bids_prices
+
+    def in_asks_prices(
+            self,
+            exchange: str,
+            symbol: str,
+            separator: Optional[str] = None
+    ) -> bool:
+        """
+        Checks if the symbol is in the prices' data.
+
+        :param exchange: The exchange name.
+        :param symbol: The symbol to search.
+        :param separator: The separator of the assets.
+
+        :return: The validation value.
+        """
+
+        return is_symbol_in_assets_market_prices(
+            exchange=exchange, symbol=symbol,
+            separator=separator, prices=self.asks
+        )
+    # end in_asks_prices
+
+    def in_prices(
+            self,
+            exchange: str,
+            symbol: str,
+            separator: Optional[str] = None
+    ) -> bool:
+        """
+        Checks if the symbol is in the prices' data.
+
+        :param exchange: The exchange name.
+        :param symbol: The symbol to search.
+        :param separator: The separator of the assets.
+
+        :return: The validation value.
+        """
+
+        return (
+            self.in_bids_prices(
+                exchange=exchange, symbol=symbol,
+                separator=separator
+            )
+            and
+            self.in_asks_prices(
+                exchange=exchange, symbol=symbol,
+                separator=separator
+            )
+        )
+    # end in_prices
+# end AssetsMarketBase
+
+@dataclass(repr=False, slots=True)
+@represent
+class AssetsMarketState(AssetsMarketBase):
+    """
+    A class to represent the current market state.
+
+    This object contains the state of the market, as Close,
+    bids and asks prices of specific assets, gathered from the network.
+
+    attributes:
+
+    - screeners:
+        The screener objects to collect the prices of the assets.
 
     - bids:
         The bids prices of the assets.
 
     - asks:
         The asks prices of the assets.
 
     >>> from crypto_screening.collect.market import AssetsMarketState
     >>>
     >>> state = assets_market_state(["BTC", "ETH", "LTC"], currency="USDT")
     """
 
-    screeners: Screeners
     bids: AssetsPrices
     asks: AssetsPrices
 
     __modifiers__: ClassVar[Modifiers] = Modifiers(
-        excluded=["screeners", "bids", "asks"]
+        **AssetsMarketBase.__modifiers__
     )
-
-    def __hash__(self) -> int:
-        """
-        Returns the hash of the object.
-
-        :return: The hash of the object.
-        """
-
-        return id(self)
-    # end __hash__
+    __modifiers__.excluded.extend(["bids", "asks"])
 
     def bid(self, exchange: str, symbol: str, separator: Optional[str] = None) -> float:
         """
         Returns the bid price for the symbol.
 
         :param exchange: The exchange name.
         :param symbol: The symbol to find its bid price.
@@ -279,15 +428,15 @@
             exchange=exchange, symbol=symbol, prices=self.asks,
             separator=separator, provider=self
         )
     # end ask
 # end MarketState
 
 def assets_market_state(
-        screeners: Optional[Screeners] = None,
+        screeners: Optional[Iterable[BaseScreener]] = None,
         separator: Optional[str] = None,
         adjust: Optional[bool] = True
 ) -> AssetsMarketState:
     """
     Fetches the prices and relations between the assets.
 
     :param screeners: The price screeners.
@@ -306,19 +455,25 @@
         )
 
         if adjust and (len(screener.market) == 0):
             continue
         # end if
 
         try:
-            bids.setdefault(screener.exchange, {}).setdefault(base, {}).setdefault(
-                quote, screener.market[BIDS][-1]
-            )
-            asks.setdefault(screener.exchange, {}).setdefault(base, {}).setdefault(
-                quote, screener.market[ASKS][-1]
+            (
+                bids.
+                setdefault(screener.exchange, {}).
+                setdefault(base, {}).
+                setdefault(quote, screener.market[BIDS][-1])
+            )
+            (
+                asks.
+                setdefault(screener.exchange, {}).
+                setdefault(base, {}).
+                setdefault(quote, screener.market[ASKS][-1])
             )
 
         except IndexError:
             raise ValueError(
                 f"Data of '{screener.exchange}' symbol in "
                 f"'{screener.symbol}' exchange is empty."
                 f"Consider using the 'adjust' parameter as {True}, "
@@ -330,58 +485,133 @@
     return AssetsMarketState(
         screeners=screeners, bids=bids, asks=asks
     )
 # end assets_market_state
 
 @dataclass(repr=False, slots=True)
 @represent
-class SymbolsMarketState:
+class SymbolsMarketBase(metaclass=ABCMeta):
     """
     A class to represent the current market state.
 
     This object contains the state of the market, as Close,
     bids and asks prices of specific assets, gathered from the network.
 
     attributes:
 
     - screeners:
         The screener objects to collect the prices of the assets.
 
-    - prices:
-        The close price of the assets.
-
     - bids:
         The bids prices of the assets.
 
     - asks:
         The asks prices of the assets.
 
     >>> from crypto_screening.collect.market import AssetsMarketState
     >>>
     >>> state = assets_market_state(["BTC", "ETH", "LTC"], currency="USDT")
     """
 
-    screeners: Screeners
-    bids: SymbolsPrices
-    asks: SymbolsPrices
+    screeners: Iterable[BaseScreener]
 
-    __modifiers__: ClassVar[Modifiers] = Modifiers(
-        excluded=["screeners", "bids", "asks"]
-    )
+    __modifiers__: ClassVar[Modifiers] = Modifiers(excluded=["screeners"])
 
     def __hash__(self) -> int:
         """
         Returns the hash of the object.
 
         :return: The hash of the object.
         """
 
         return id(self)
     # end __hash__
 
+    def in_bids_prices(self, exchange: str, symbol: str) -> bool:
+        """
+        Checks if the symbol is in the prices' data.
+
+        :param exchange: The exchange name.
+        :param symbol: The symbol to search.
+
+        :return: The validation value.
+        """
+
+        return is_symbol_in_symbols_market_prices(
+            exchange=exchange, symbol=symbol, prices=self.bids
+        )
+    # end in_bids_prices
+
+    def in_asks_prices(self, exchange: str, symbol: str) -> bool:
+        """
+        Checks if the symbol is in the prices' data.
+
+        :param exchange: The exchange name.
+        :param symbol: The symbol to search.
+
+        :return: The validation value.
+        """
+
+        return is_symbol_in_symbols_market_prices(
+            exchange=exchange, symbol=symbol, prices=self.asks
+        )
+    # end in_asks_prices
+
+    def in_prices(self, exchange: str, symbol: str) -> bool:
+        """
+        Checks if the symbol is in the prices' data.
+
+        :param exchange: The exchange name.
+        :param symbol: The symbol to search.
+
+        :return: The validation value.
+        """
+
+        return (
+            self.in_bids_prices(exchange=exchange, symbol=symbol) and
+            self.in_asks_prices(exchange=exchange, symbol=symbol)
+        )
+    # end in_prices
+
+@dataclass(repr=False, slots=True)
+@represent
+class SymbolsMarketState(SymbolsMarketBase):
+    """
+    A class to represent the current market state.
+
+    This object contains the state of the market, as Close,
+    bids and asks prices of specific assets, gathered from the network.
+
+    attributes:
+
+    - screeners:
+        The screener objects to collect the prices of the assets.
+
+    - prices:
+        The close price of the assets.
+
+    - bids:
+        The bids prices of the assets.
+
+    - asks:
+        The asks prices of the assets.
+
+    >>> from crypto_screening.collect.market import AssetsMarketState
+    >>>
+    >>> state = assets_market_state(["BTC", "ETH", "LTC"], currency="USDT")
+    """
+
+    bids: SymbolsPrices
+    asks: SymbolsPrices
+
+    __modifiers__: ClassVar[Modifiers] = Modifiers(
+        **SymbolsMarketBase.__modifiers__
+    )
+    __modifiers__.excluded.extend(["bids", "asks"])
+
     def bid(self, exchange: str, symbol: str) -> float:
         """
         Returns the bid price for the symbol.
 
         :param exchange: The exchange name.
         :param symbol: The symbol to find its bid price.
 
@@ -408,15 +638,15 @@
             exchange=exchange, symbol=symbol,
             prices=self.asks, provider=self
         )
     # end ask
 # end SymbolsMarketState
 
 def symbols_market_state(
-        screeners: Optional[Screeners] = None,
+        screeners: Optional[Iterable[BaseScreener]] = None,
         adjust: Optional[bool] = True
 ) -> SymbolsMarketState:
     """
     Fetches the prices and relations between the assets.
 
     :param screeners: The price screeners.
     :param adjust: The value to adjust the length of the sequences.
@@ -429,19 +659,23 @@
 
     for screener in screeners:
         if adjust and (len(screener.market) == 0):
             continue
         # end if
 
         try:
-            bids.setdefault(screener.exchange, {}).setdefault(
-                screener.symbol, screener.market[BIDS][-1]
-            )
-            asks.setdefault(screener.exchange, {}).setdefault(
-                screener.symbol, screener.market[ASKS][-1]
+            (
+                bids.
+                setdefault(screener.exchange, {}).
+                setdefault(screener.symbol, screener.market[BIDS][-1])
+            )
+            (
+                asks.
+                setdefault(screener.exchange, {}).
+                setdefault(screener.symbol, screener.market[ASKS][-1])
             )
 
         except IndexError:
             raise ValueError(
                 f"Data of '{screener.exchange}' symbol in "
                 f"'{screener.symbol}' exchange is empty."
                 f"Consider using the 'adjust' parameter as {True}, "
@@ -478,57 +712,44 @@
     )
 
     return [float(value) for value in prices[exchange][symbol]]
 # end symbols_market_price_sequence
 
 @dataclass(repr=False, slots=True)
 @represent
-class AssetsMarketStates:
+class AssetsMarketStates(AssetsMarketBase):
     """
     A class to represent the current market state.
 
     This object contains the state of the market, as Close,
     bids and asks prices of specific assets, gathered from the network.
 
     attributes:
 
     - screeners:
         The screener objects to collect the prices of the assets.
 
-    - prices:
-        The close price of the assets.
-
     - bids:
         The bids prices of the assets.
 
     - asks:
         The asks prices of the assets.
 
     >>> from crypto_screening.collect.market import AssetsMarketState
     >>>
     >>> state = assets_market_state(["BTC", "ETH", "LTC"], currency="USDT")
     """
 
-    screeners: Screeners
     bids: AssetsPricesSequence
     asks: AssetsPricesSequence
 
     __modifiers__: ClassVar[Modifiers] = Modifiers(
-        excluded=["screeners", "bids", "asks"]
+        **AssetsMarketBase.__modifiers__
     )
-
-    def __hash__(self) -> int:
-        """
-        Returns the hash of the object.
-
-        :return: The hash of the object.
-        """
-
-        return id(self)
-    # end __hash__
+    __modifiers__.excluded.extend(["bids", "asks"])
 
     def bid(self, exchange: str, symbol: str, separator: Optional[str] = None) -> List[float]:
         """
         Returns the bid price for the symbol.
 
         :param exchange: The exchange name.
         :param symbol: The symbol to find its bid price.
@@ -587,15 +808,15 @@
 
     base, quote = symbol_to_parts(symbol=symbol, separator=separator)
 
     return [float(value) for value in prices[exchange][base][quote]]
 # end assets_market_price_sequence
 
 def assets_market_states(
-        screeners: Optional[Screeners] = None,
+        screeners: Optional[Iterable[BaseScreener]] = None,
         separator: Optional[str] = None,
         length: Optional[int] = None,
         adjust: Optional[bool] = True
 ) -> AssetsMarketStates:
     """
     Fetches the prices and relations between the assets.
 
@@ -623,39 +844,46 @@
         # end if
 
         base, quote = symbol_to_parts(
             symbol=screener.symbol, separator=separator
         )
 
         try:
-            bids.setdefault(screener.exchange, {}).setdefault(base, {}).setdefault(
-                quote, list(screener.market[BIDS][-length:])
-            )
-            asks.setdefault(screener.exchange, {}).setdefault(base, {}).setdefault(
-                quote, list(screener.market[ASKS][-length:])
+            (
+                bids.
+                setdefault(screener.exchange, {}).
+                setdefault(base, {}).
+                setdefault(quote, list(screener.market[BIDS][-length:]))
+            )
+            (
+                asks.
+                setdefault(screener.exchange, {}).
+                setdefault(base, {}).
+                setdefault(quote, list(screener.market[ASKS][-length:]))
             )
 
         except IndexError:
             raise ValueError(
-                f"Data of '{screener.exchange}' symbol in '{screener.symbol}' exchange "
+                f"Data of '{screener.exchange}' "
+                f"symbol in '{screener.symbol}' exchange "
                 f"is not long enough for the requested length: {length}. "
                 f"Consider using the 'adjust' parameter as {True}, "
                 f"to adjust to the actual length of the data."
             )
         # end try
     # end for
 
     return AssetsMarketStates(
         screeners=screeners, bids=bids, asks=asks
     )
 # end assets_market_state
 
 @dataclass(repr=False, slots=True)
 @represent
-class SymbolsMarketStates:
+class SymbolsMarketStates(SymbolsMarketBase):
     """
     A class to represent the current market state.
 
     This object contains the state of the market, as Close,
     bids and asks prices of specific assets, gathered from the network.
 
     attributes:
@@ -673,31 +901,21 @@
         The asks prices of the assets.
 
     >>> from crypto_screening.collect.market import AssetsMarketState
     >>>
     >>> state = assets_market_state(["BTC", "ETH", "LTC"], currency="USDT")
     """
 
-    screeners: Screeners
     bids: SymbolsPricesSequence
     asks: SymbolsPricesSequence
 
     __modifiers__: ClassVar[Modifiers] = Modifiers(
-        excluded=["screeners", "bids", "asks"]
+        **AssetsMarketBase.__modifiers__
     )
-
-    def __hash__(self) -> int:
-        """
-        Returns the hash of the object.
-
-        :return: The hash of the object.
-        """
-
-        return id(self)
-    # end __hash__
+    __modifiers__.excluded.extend(["bids", "asks"])
 
     def bid(self, exchange: str, symbol: str) -> List[float]:
         """
         Returns the bid price for the symbol.
 
         :param exchange: The exchange name.
         :param symbol: The symbol to find its bid price.
@@ -725,15 +943,15 @@
             exchange=exchange, symbol=symbol,
             prices=self.asks, provider=self
         )
     # end ask
 # end SymbolsMarketStates
 
 def symbols_market_states(
-        screeners: Optional[Screeners] = None,
+        screeners: Optional[Iterable[BaseScreener]] = None,
         length: Optional[int] = None,
         adjust: Optional[bool] = True
 ) -> SymbolsMarketStates:
     """
     Fetches the prices and relations between the assets.
 
     :param screeners: The price screeners.
@@ -755,19 +973,29 @@
             length = len(screener.market)
 
         elif adjust:
             length = min([len(screener.market), length])
         # end if
 
         try:
-            bids.setdefault(screener.exchange, {}).setdefault(
-                screener.symbol, list(screener.market[BIDS][-length:])
-            )
-            asks.setdefault(screener.exchange, {}).setdefault(
-                screener.symbol, list(screener.market[ASKS][-length:])
+            (
+                bids.
+                setdefault(screener.exchange, {}).
+                setdefault(
+                    screener.symbol,
+                    list(screener.market[BIDS][-length:])
+                )
+            )
+            (
+                asks.
+                setdefault(screener.exchange, {}).
+                setdefault(
+                    screener.symbol,
+                    list(screener.market[ASKS][-length:])
+                )
             )
 
         except IndexError:
             raise ValueError(
                 f"Data of '{screener.exchange}' symbol in '{screener.symbol}' exchange "
                 f"is not long enough for the requested length: {length}. "
                 f"Consider using the 'adjust' parameter as {True}, "
```

### Comparing `crypto-screening-1.9.8/crypto_screening/collect/screeners.py` & `crypto-screening-2.0.0/crypto_screening/collect/screeners.py`

 * *Files identical despite different names*

### Comparing `crypto-screening-1.9.8/crypto_screening/collect/symbols.py` & `crypto-screening-2.0.0/crypto_screening/collect/symbols.py`

 * *Files identical despite different names*

### Comparing `crypto-screening-1.9.8/crypto_screening/dataset.py` & `crypto-screening-2.0.0/crypto_screening/dataset.py`

 * *Files identical despite different names*

### Comparing `crypto-screening-1.9.8/crypto_screening/interval.py` & `crypto-screening-2.0.0/crypto_screening/interval.py`

 * *Files identical despite different names*

### Comparing `crypto-screening-1.9.8/crypto_screening/market/foundation/data.py` & `crypto-screening-2.0.0/crypto_screening/market/foundation/data.py`

 * *Files identical despite different names*

### Comparing `crypto-screening-1.9.8/crypto_screening/market/foundation/protocols.py` & `crypto-screening-2.0.0/crypto_screening/market/foundation/protocols.py`

 * *Files identical despite different names*

### Comparing `crypto-screening-1.9.8/crypto_screening/market/foundation/state.py` & `crypto-screening-2.0.0/crypto_screening/market/foundation/state.py`

 * *Files identical despite different names*

### Comparing `crypto-screening-1.9.8/crypto_screening/market/foundation/waiting.py` & `crypto-screening-2.0.0/crypto_screening/market/foundation/waiting.py`

 * *Files identical despite different names*

### Comparing `crypto-screening-1.9.8/crypto_screening/market/screeners/base.py` & `crypto-screening-2.0.0/crypto_screening/market/screeners/base.py`

 * *Files identical despite different names*

### Comparing `crypto-screening-1.9.8/crypto_screening/market/screeners/container.py` & `crypto-screening-2.0.0/crypto_screening/market/screeners/container.py`

 * *Files identical despite different names*

### Comparing `crypto-screening-1.9.8/crypto_screening/market/screeners/ohlcv.py` & `crypto-screening-2.0.0/crypto_screening/market/screeners/ohlcv.py`

 * *Files identical despite different names*

### Comparing `crypto-screening-1.9.8/crypto_screening/market/screeners/orderbook.py` & `crypto-screening-2.0.0/crypto_screening/market/screeners/orderbook.py`

 * *Files identical despite different names*

### Comparing `crypto-screening-1.9.8/crypto_screening/market/screeners/recorder.py` & `crypto-screening-2.0.0/crypto_screening/market/screeners/recorder.py`

 * *Files identical despite different names*

### Comparing `crypto-screening-1.9.8/crypto_screening/market/waiting.py` & `crypto-screening-2.0.0/crypto_screening/market/waiting.py`

 * *Files identical despite different names*

### Comparing `crypto-screening-1.9.8/crypto_screening/process.py` & `crypto-screening-2.0.0/crypto_screening/process.py`

 * *Files identical despite different names*

### Comparing `crypto-screening-1.9.8/crypto_screening/symbols.py` & `crypto-screening-2.0.0/crypto_screening/symbols.py`

 * *Files identical despite different names*

### Comparing `crypto-screening-1.9.8/crypto_screening/validate.py` & `crypto-screening-2.0.0/crypto_screening/validate.py`

 * *Files identical despite different names*

### Comparing `crypto-screening-1.9.8/crypto_screening.egg-info/PKG-INFO` & `crypto-screening-2.0.0/crypto_screening.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: crypto-screening
-Version: 1.9.8
+Version: 2.0.0
 Summary: A software for automatically recording real-time crypto exchanges and pairs OHLCV and Orderbook rates.
 Home-page: https://github.com/Shahaf-F-S/crypto-screening
 Author: Shahaf Frank-Shapir
 Author-email: shahaffrs@gmail.com
 License: MIT
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `crypto-screening-1.9.8/crypto_screening.egg-info/SOURCES.txt` & `crypto-screening-2.0.0/crypto_screening.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `crypto-screening-1.9.8/pyproject.toml` & `crypto-screening-2.0.0/pyproject.toml`

 * *Files 14% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = 'crypto-screening'
-version = '1.9.8'
+version = '2.0.0'
 description = 'A software for automatically recording real-time crypto exchanges and pairs OHLCV and Orderbook rates.'
 classifiers = [
 	'Intended Audience :: Developers',
 	'License :: OSI Approved :: MIT License',
 	'Programming Language :: Python',
 	'Programming Language :: Python :: 3',
 	'Programming Language :: Python :: 3.8',
```

### Comparing `crypto-screening-1.9.8/setup.py` & `crypto-screening-2.0.0/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -20,15 +20,15 @@
         exclude=[
             "__pycache__",
             "*.pyc"
         ],
         requirements="requirements.txt",
         dev_requirements="requirements-dev.txt",
         name='crypto-screening',
-        version='1.9.8',
+        version='2.0.0',
         description=(
             "A software for automatically recording "
             "real-time crypto exchanges and pairs "
             "OHLCV and Orderbook rates."
         ),
         license='MIT',
         author="Shahaf Frank-Shapir",
```

