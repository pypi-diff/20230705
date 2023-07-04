# Comparing `tmp/yabte-0.3.5.tar.gz` & `tmp/yabte-0.3.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "yabte-0.3.5.tar", max compression
+gzip compressed data, was "yabte-0.3.6.tar", max compression
```

## Comparing `yabte-0.3.5.tar` & `yabte-0.3.6.tar`

### file list

```diff
@@ -1,45 +1,47 @@
--rw-r--r--   0        0        0     1072 2023-05-31 21:21:14.945726 yabte-0.3.5/LICENSE
--rw-r--r--   0        0        0     3220 2023-05-31 21:21:14.945726 yabte-0.3.5/README.md
--rw-r--r--   0        0        0     1115 2023-05-31 21:21:14.957726 yabte-0.3.5/pyproject.toml
--rw-r--r--   0        0        0       30 2023-05-31 21:21:14.957726 yabte-0.3.5/yabte/__init__.py
--rw-r--r--   0        0        0      859 2023-05-31 21:21:14.957726 yabte-0.3.5/yabte/backtest/__init__.py
--rw-r--r--   0        0        0      670 2023-05-31 21:21:14.957726 yabte-0.3.5/yabte/backtest/_helpers.py
--rw-r--r--   0        0        0     3123 2023-05-31 21:21:14.957726 yabte-0.3.5/yabte/backtest/asset.py
--rw-r--r--   0        0        0     4004 2023-05-31 21:21:14.957726 yabte-0.3.5/yabte/backtest/book.py
--rw-r--r--   0        0        0    12933 2023-05-31 21:21:14.957726 yabte-0.3.5/yabte/backtest/order.py
--rw-r--r--   0        0        0    11687 2023-05-31 21:21:14.957726 yabte-0.3.5/yabte/backtest/strategy.py
--rw-r--r--   0        0        0     2207 2023-05-31 21:21:14.957726 yabte-0.3.5/yabte/backtest/transaction.py
--rw-r--r--   0        0        0        0 2023-05-31 21:21:14.957726 yabte-0.3.5/yabte/tests/__init__.py
--rw-r--r--   0        0        0      594 2023-05-31 21:21:14.957726 yabte-0.3.5/yabte/tests/_helpers.py
--rw-r--r--   0        0        0     1266 2023-05-31 21:21:14.957726 yabte-0.3.5/yabte/tests/_unittest_numpy_extensions.py
--rw-r--r--   0        0        0   137308 2023-05-31 21:21:14.957726 yabte-0.3.5/yabte/tests/data/nasdaq/AAPL.csv
--rw-r--r--   0        0        0   135665 2023-05-31 21:21:14.961726 yabte-0.3.5/yabte/tests/data/nasdaq/AMZN.csv
--rw-r--r--   0        0        0    90302 2023-05-31 21:21:14.961726 yabte-0.3.5/yabte/tests/data/nasdaq/GOOG.csv
--rw-r--r--   0        0        0   136484 2023-05-31 21:21:14.961726 yabte-0.3.5/yabte/tests/data/nasdaq/INTC.csv
--rw-r--r--   0        0        0   135802 2023-05-31 21:21:14.961726 yabte-0.3.5/yabte/tests/data/nasdaq/META.csv
--rw-r--r--   0        0        0    93835 2023-05-31 21:21:14.961726 yabte-0.3.5/yabte/tests/data/nasdaq/MSFT.csv
--rw-r--r--   0        0        0   130341 2023-05-31 21:21:14.961726 yabte-0.3.5/yabte/tests/data/nasdaq/NFLX.csv
--rw-r--r--   0        0        0   139249 2023-05-31 21:21:14.965726 yabte-0.3.5/yabte/tests/data/nasdaq/TSLA.csv
--rw-r--r--   0        0        0      799 2023-05-31 21:21:14.965726 yabte-0.3.5/yabte/tests/test_notebooks.py
--rw-r--r--   0        0        0     1676 2023-05-31 21:21:14.965726 yabte-0.3.5/yabte/tests/test_portopt.py
--rw-r--r--   0        0        0     4075 2023-05-31 21:21:14.965726 yabte-0.3.5/yabte/tests/test_simulation.py
--rw-r--r--   0        0        0    18624 2023-05-31 21:21:14.965726 yabte-0.3.5/yabte/tests/test_strategy_runner.py
--rw-r--r--   0        0        0     1560 2023-05-31 21:21:14.965726 yabte-0.3.5/yabte/tests/test_utilities.py
--rw-r--r--   0        0        0        0 2023-05-31 21:21:14.965726 yabte-0.3.5/yabte/utilities/__init__.py
--rw-r--r--   0        0        0     1179 2023-05-31 21:21:14.965726 yabte-0.3.5/yabte/utilities/lagrangian.py
--rw-r--r--   0        0        0     2353 2023-05-31 21:21:14.965726 yabte-0.3.5/yabte/utilities/pandas_extension.py
--rw-r--r--   0        0        0        0 2023-05-31 21:21:14.965726 yabte-0.3.5/yabte/utilities/plot/__init__.py
--rw-r--r--   0        0        0        0 2023-05-31 21:21:14.965726 yabte-0.3.5/yabte/utilities/plot/matplotlib/__init__.py
--rw-r--r--   0        0        0     3360 2023-05-31 21:21:14.965726 yabte-0.3.5/yabte/utilities/plot/matplotlib/marker_updater.py
--rw-r--r--   0        0        0     5520 2023-05-31 21:21:14.965726 yabte-0.3.5/yabte/utilities/plot/matplotlib/strategy_runner.py
--rw-r--r--   0        0        0        0 2023-05-31 21:21:14.965726 yabte-0.3.5/yabte/utilities/portopt/__init__.py
--rw-r--r--   0        0        0     2332 2023-05-31 21:21:14.965726 yabte-0.3.5/yabte/utilities/portopt/hierarchical_risk_parity.py
--rw-r--r--   0        0        0      396 2023-05-31 21:21:14.965726 yabte-0.3.5/yabte/utilities/portopt/inverse_volatility.py
--rw-r--r--   0        0        0     1973 2023-05-31 21:21:14.965726 yabte-0.3.5/yabte/utilities/portopt/minimum_variance.py
--rw-r--r--   0        0        0        0 2023-05-31 21:21:14.965726 yabte-0.3.5/yabte/utilities/simulation/__init__.py
--rw-r--r--   0        0        0     1475 2023-05-31 21:21:14.965726 yabte-0.3.5/yabte/utilities/simulation/geometric_brownian_motion.py
--rw-r--r--   0        0        0     2098 2023-05-31 21:21:14.965726 yabte-0.3.5/yabte/utilities/simulation/heston.py
--rw-r--r--   0        0        0     1102 2023-05-31 21:21:14.965726 yabte-0.3.5/yabte/utilities/simulation/weiner.py
--rw-r--r--   0        0        0      397 2023-05-31 21:21:14.965726 yabte-0.3.5/yabte/utilities/strategy_helpers.py
--rw-r--r--   0        0        0     4275 1970-01-01 00:00:00.000000 yabte-0.3.5/setup.py
--rw-r--r--   0        0        0     3916 1970-01-01 00:00:00.000000 yabte-0.3.5/PKG-INFO
+-rw-r--r--   0        0        0     1072 2023-07-04 22:04:05.852069 yabte-0.3.6/LICENSE
+-rw-r--r--   0        0        0     3268 2023-07-04 22:04:05.852069 yabte-0.3.6/README.md
+-rw-r--r--   0        0        0     1134 2023-07-04 22:04:05.860069 yabte-0.3.6/pyproject.toml
+-rw-r--r--   0        0        0       30 2023-07-04 22:04:05.860069 yabte-0.3.6/yabte/__init__.py
+-rw-r--r--   0        0        0      859 2023-07-04 22:04:05.860069 yabte-0.3.6/yabte/backtest/__init__.py
+-rw-r--r--   0        0        0      670 2023-07-04 22:04:05.860069 yabte-0.3.6/yabte/backtest/_helpers.py
+-rw-r--r--   0        0        0     3123 2023-07-04 22:04:05.864069 yabte-0.3.6/yabte/backtest/asset.py
+-rw-r--r--   0        0        0     4004 2023-07-04 22:04:05.864069 yabte-0.3.6/yabte/backtest/book.py
+-rw-r--r--   0        0        0    12925 2023-07-04 22:04:05.864069 yabte-0.3.6/yabte/backtest/order.py
+-rw-r--r--   0        0        0    11675 2023-07-04 22:04:05.864069 yabte-0.3.6/yabte/backtest/strategy.py
+-rw-r--r--   0        0        0     2207 2023-07-04 22:04:05.864069 yabte-0.3.6/yabte/backtest/transaction.py
+-rw-r--r--   0        0        0        0 2023-07-04 22:04:05.864069 yabte-0.3.6/yabte/tests/__init__.py
+-rw-r--r--   0        0        0      594 2023-07-04 22:04:05.864069 yabte-0.3.6/yabte/tests/_helpers.py
+-rw-r--r--   0        0        0     1278 2023-07-04 22:04:05.864069 yabte-0.3.6/yabte/tests/_unittest_numpy_extensions.py
+-rw-r--r--   0        0        0   137308 2023-07-04 22:04:05.864069 yabte-0.3.6/yabte/tests/data/nasdaq/AAPL.csv
+-rw-r--r--   0        0        0   135665 2023-07-04 22:04:05.864069 yabte-0.3.6/yabte/tests/data/nasdaq/AMZN.csv
+-rw-r--r--   0        0        0    90302 2023-07-04 22:04:05.864069 yabte-0.3.6/yabte/tests/data/nasdaq/GOOG.csv
+-rw-r--r--   0        0        0   136484 2023-07-04 22:04:05.864069 yabte-0.3.6/yabte/tests/data/nasdaq/INTC.csv
+-rw-r--r--   0        0        0   135802 2023-07-04 22:04:05.868069 yabte-0.3.6/yabte/tests/data/nasdaq/META.csv
+-rw-r--r--   0        0        0    93835 2023-07-04 22:04:05.868069 yabte-0.3.6/yabte/tests/data/nasdaq/MSFT.csv
+-rw-r--r--   0        0        0   130341 2023-07-04 22:04:05.868069 yabte-0.3.6/yabte/tests/data/nasdaq/NFLX.csv
+-rw-r--r--   0        0        0   139249 2023-07-04 22:04:05.868069 yabte-0.3.6/yabte/tests/data/nasdaq/TSLA.csv
+-rw-r--r--   0        0        0      799 2023-07-04 22:04:05.868069 yabte-0.3.6/yabte/tests/test_notebooks.py
+-rw-r--r--   0        0        0     1676 2023-07-04 22:04:05.868069 yabte-0.3.6/yabte/tests/test_portopt.py
+-rw-r--r--   0        0        0     4075 2023-07-04 22:04:05.868069 yabte-0.3.6/yabte/tests/test_simulation.py
+-rw-r--r--   0        0        0    18624 2023-07-04 22:04:05.868069 yabte-0.3.6/yabte/tests/test_strategy_runner.py
+-rw-r--r--   0        0        0     1560 2023-07-04 22:04:05.868069 yabte-0.3.6/yabte/tests/test_utilities.py
+-rw-r--r--   0        0        0        0 2023-07-04 22:04:05.868069 yabte-0.3.6/yabte/utilities/__init__.py
+-rw-r--r--   0        0        0     1179 2023-07-04 22:04:05.868069 yabte-0.3.6/yabte/utilities/lagrangian.py
+-rw-r--r--   0        0        0     2353 2023-07-04 22:04:05.868069 yabte-0.3.6/yabte/utilities/pandas_extension.py
+-rw-r--r--   0        0        0        0 2023-07-04 22:04:05.868069 yabte-0.3.6/yabte/utilities/plot/__init__.py
+-rw-r--r--   0        0        0        0 2023-07-04 22:04:05.868069 yabte-0.3.6/yabte/utilities/plot/matplotlib/__init__.py
+-rw-r--r--   0        0        0     3360 2023-07-04 22:04:05.868069 yabte-0.3.6/yabte/utilities/plot/matplotlib/marker_updater.py
+-rw-r--r--   0        0        0     5516 2023-07-04 22:04:05.868069 yabte-0.3.6/yabte/utilities/plot/matplotlib/strategy_runner.py
+-rw-r--r--   0        0        0        0 2023-07-04 22:04:05.868069 yabte-0.3.6/yabte/utilities/plot/plotly/__init__.py
+-rw-r--r--   0        0        0     5625 2023-07-04 22:04:05.868069 yabte-0.3.6/yabte/utilities/plot/plotly/strategy_runner.py
+-rw-r--r--   0        0        0        0 2023-07-04 22:04:05.868069 yabte-0.3.6/yabte/utilities/portopt/__init__.py
+-rw-r--r--   0        0        0     2332 2023-07-04 22:04:05.868069 yabte-0.3.6/yabte/utilities/portopt/hierarchical_risk_parity.py
+-rw-r--r--   0        0        0      396 2023-07-04 22:04:05.868069 yabte-0.3.6/yabte/utilities/portopt/inverse_volatility.py
+-rw-r--r--   0        0        0     1973 2023-07-04 22:04:05.868069 yabte-0.3.6/yabte/utilities/portopt/minimum_variance.py
+-rw-r--r--   0        0        0        0 2023-07-04 22:04:05.868069 yabte-0.3.6/yabte/utilities/simulation/__init__.py
+-rw-r--r--   0        0        0     1475 2023-07-04 22:04:05.868069 yabte-0.3.6/yabte/utilities/simulation/geometric_brownian_motion.py
+-rw-r--r--   0        0        0     2098 2023-07-04 22:04:05.868069 yabte-0.3.6/yabte/utilities/simulation/heston.py
+-rw-r--r--   0        0        0     1102 2023-07-04 22:04:05.868069 yabte-0.3.6/yabte/utilities/simulation/weiner.py
+-rw-r--r--   0        0        0      397 2023-07-04 22:04:05.872069 yabte-0.3.6/yabte/utilities/strategy_helpers.py
+-rw-r--r--   0        0        0     4355 1970-01-01 00:00:00.000000 yabte-0.3.6/setup.py
+-rw-r--r--   0        0        0     3964 1970-01-01 00:00:00.000000 yabte-0.3.6/PKG-INFO
```

### Comparing `yabte-0.3.5/LICENSE` & `yabte-0.3.6/LICENSE`

 * *Files identical despite different names*

### Comparing `yabte-0.3.5/README.md` & `yabte-0.3.6/README.md`

 * *Files 5% similar despite different names*

```diff
@@ -107,9 +107,9 @@
 ## Development
 
 Before commit run following format commands in project folder:
 
 ```bash
 poetry run black .
 poetry run isort . --profile black
-poetry run docformatter . --recursive --in-place
+poetry run docformatter . --recursive --in-place --black --exclude _unittest_numpy_extensions.py
 ```
```

### Comparing `yabte-0.3.5/pyproject.toml` & `yabte-0.3.6/pyproject.toml`

 * *Files 15% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "yabte"
-version = "0.3.5"
+version = "0.3.6"
 description = "Yet another backtesting engine"
 authors = ["Blair Azzopardi <blairuk@gmail.com>"]
 license = "MIT"
 readme = "README.md"
 repository = "https://github.com/bsdz/yabte"
 
 [tool.poetry.build]
@@ -35,14 +35,15 @@
 sphinx-rtd-theme = "1.2.0rc4"
 
 [tool.poetry.group.notebooks]
 optional = true
 
 [tool.poetry.group.notebooks.dependencies]
 matplotlib = "^3.6.2"
+plotly = "^5.10.0"
 ipykernel = "^6.20.2"
 pyfeng = "^0.2.5"
 nbconvert = "^7.2.9"
 
 [tool.isort]
 profile = "black"
```

### Comparing `yabte-0.3.5/yabte/backtest/__init__.py` & `yabte-0.3.6/yabte/backtest/__init__.py`

 * *Files identical despite different names*

### Comparing `yabte-0.3.5/yabte/backtest/_helpers.py` & `yabte-0.3.6/yabte/backtest/_helpers.py`

 * *Files identical despite different names*

### Comparing `yabte-0.3.5/yabte/backtest/asset.py` & `yabte-0.3.6/yabte/backtest/asset.py`

 * *Files 2% similar despite different names*

```diff
@@ -61,16 +61,16 @@
         necessary."""
         raise NotImplementedError("The apply methods needs to be implemented.")
 
 
 @mypyc_attr(allow_interpreted_subclasses=True)
 @dataclass(kw_only=True)
 class Asset(AssetBase):
-    """Assets whose price history is represented by High, Low, Open, Close and
-    Volume fields."""
+    """Assets whose price history is represented by High, Low, Open, Close and Volume
+    fields."""
 
     @property
     def fields_available_at_open(self) -> Sequence[str]:
         return ["Open"]
 
     def intraday_traded_price(self, asset_day_data) -> Decimal:
         if pd.notnull(asset_day_data.Low) and pd.notnull(asset_day_data.High):
```

### Comparing `yabte-0.3.5/yabte/backtest/book.py` & `yabte-0.3.6/yabte/backtest/book.py`

 * *Files identical despite different names*

### Comparing `yabte-0.3.5/yabte/backtest/order.py` & `yabte-0.3.6/yabte/backtest/order.py`

 * *Files 1% similar despite different names*

```diff
@@ -70,16 +70,16 @@
 
     priority: int = 0
     """Each day orders are sorted by this field and executed in order."""
 
     key: Optional[str] = None
     """Unique key for this order.
 
-    If a key is set then only the newest order with this key is kept.
-    Older orders with the same key will be removed.
+    If a key is set then only the newest order with this key is kept. Older orders with
+    the same key will be removed.
     """
 
     def __post_init__(self):
         pass
 
     def _book_trades(self, trades):
         # test then book trades, do any post complete tasks
@@ -90,16 +90,15 @@
 
         else:
             self.status = OrderStatus.MANDATE_FAILED
 
     def post_complete(self, trades: List[Trade]):
         """Called after and with trades that have been successfully booked.
 
-        It can append new orders to suborders for execution in the
-        following timestep.
+        It can append new orders to suborders for execution in the following timestep.
         """
         pass
 
     def apply(
         self, ts: pd.Timestamp, day_data: pd.DataFrame, asset_map: Dict[str, Asset]
     ):
         """Applies order to `self.book` for time `ts` using provided `day_data`
@@ -145,16 +144,16 @@
             raise RuntimeError("Unsupported size type")
 
         return asset.round_quantity(quantity), trade_price
 
     def pre_execute_check(
         self, ts: pd.Timestamp, trade_price: Decimal
     ) -> Optional[OrderStatus]:
-        """Called with the current timestep and calculated trade price before
-        the trade is executed.
+        """Called with the current timestep and calculated trade price before the trade
+        is executed.
 
         If it returns `None`, the trade is executed as normal. It can
         return `OrderStatus.CANCELLED` to indicate the trade should be
         cancelled or `OrderStatus.OPEN` to indicate the trade should not
         be executed in the current timestep and processed in the
         following timestep.
         """
```

### Comparing `yabte-0.3.5/yabte/backtest/strategy.py` & `yabte-0.3.6/yabte/backtest/strategy.py`

 * *Files 2% similar despite different names*

```diff
@@ -45,16 +45,15 @@
         ou_sorted = sorted(self.deque, key=lambda o: o.priority, reverse=True)
         self.deque.clear()
         self.deque.extend(ou_sorted)
 
     def remove_duplicate_keys(self) -> List[OrderBase]:
         """Remove older orders with same key.
 
-        Returns a list of orders than were removed with status set to
-        REPLACED.
+        Returns a list of orders than were removed with status set to REPLACED.
         """
         removed = []
         cntr = Counter(o.key for o in self.deque if o.key is not None)
         if any(v > 1 for v in cntr.values()):
             kept = []
             while self.deque:
                 o = self.deque.popleft()
@@ -206,19 +205,19 @@
     Orders are captured in `orders_processed` and `orders_unprocessed`.
     `books` is a list of books and if none provided a single book is
     created called 'Main'. After execution summary book and trade
     histories are captured in `book_history` and `transaction_history`.
     """
 
     data: pd.DataFrame = field()
-    """Dataframe of price data including columns High, Low, Open, Close, Volume
-    for each asset.
+    """Dataframe of price data including columns High, Low, Open, Close, Volume for each
+    asset.
 
-    Both asset name and field make a multiindex column. The index should
-    consist of order pandas timestamps.
+    Both asset name and field make a multiindex column. The index should consist of
+    order pandas timestamps.
     """
 
     assets: List[Asset]
     """Assets available to strategy."""
 
     strat_classes: List[Type[Strategy]]
     """Strategy classes to be called within this runner."""
@@ -228,16 +227,15 @@
 
     strat_params: Dict[str, Any] = field(default_factory=dict)
     """Parameters passed to all strategies."""
 
     books: List[Book] = field(default_factory=list)
     """Books available to strategies.
 
-    If not supplied will be populated with single book named 'Main'
-    denominated in USD.
+    If not supplied will be populated with single book named 'Main' denominated in USD.
     """
 
     @property
     def book_map(self) -> Dict[BookName, Book]:
         """Mapping from book name to book instance."""
         return {book.name: book for book in self.books}
```

### Comparing `yabte-0.3.5/yabte/backtest/transaction.py` & `yabte-0.3.6/yabte/backtest/transaction.py`

 * *Files identical despite different names*

### Comparing `yabte-0.3.5/yabte/tests/_helpers.py` & `yabte-0.3.6/yabte/tests/_helpers.py`

 * *Files identical despite different names*

### Comparing `yabte-0.3.5/yabte/tests/_unittest_numpy_extensions.py` & `yabte-0.3.6/yabte/tests/_unittest_numpy_extensions.py`

 * *Files 10% similar despite different names*

```diff
@@ -2,21 +2,21 @@
 
 import numpy.testing as nptu
 
 __all__ = ["NumpyTestCase"]
 
 
 class NumpyTestCase(unittest.TestCase):
-    """Specialized TestCase which includes numpy test assertion functions and
-    maps them from assert_func_name to self.numpyAssertFuncName.
+    """Specialized TestCase which includes numpy test assertion functions and maps them
+    from assert_func_name to self.numpyAssertFuncName.
 
     class NumpyTest(NumpyTestCase):
-    def test_allclose_example(self):
-        a1 = np.array([1.,2.,3.])
-        self.numpyAssertAllclose(a1, np.array([1.,2.,3.1]))
+        def test_allclose_example(self):
+            a1 = np.array([1.,2.,3.])
+            self.numpyAssertAllclose(a1, np.array([1.,2.,3.1]))
     """
 
 
 def make_test_wrapper(fn):
     def test_wrapper(self, *args, **kwargs):
         try:
             nptu.__dict__[fn](*args, **kwargs)
```

### Comparing `yabte-0.3.5/yabte/tests/data/nasdaq/AAPL.csv` & `yabte-0.3.6/yabte/tests/data/nasdaq/AAPL.csv`

 * *Files identical despite different names*

### Comparing `yabte-0.3.5/yabte/tests/data/nasdaq/AMZN.csv` & `yabte-0.3.6/yabte/tests/data/nasdaq/AMZN.csv`

 * *Files identical despite different names*

### Comparing `yabte-0.3.5/yabte/tests/data/nasdaq/GOOG.csv` & `yabte-0.3.6/yabte/tests/data/nasdaq/GOOG.csv`

 * *Files identical despite different names*

### Comparing `yabte-0.3.5/yabte/tests/data/nasdaq/INTC.csv` & `yabte-0.3.6/yabte/tests/data/nasdaq/INTC.csv`

 * *Files identical despite different names*

### Comparing `yabte-0.3.5/yabte/tests/data/nasdaq/META.csv` & `yabte-0.3.6/yabte/tests/data/nasdaq/META.csv`

 * *Files identical despite different names*

### Comparing `yabte-0.3.5/yabte/tests/data/nasdaq/MSFT.csv` & `yabte-0.3.6/yabte/tests/data/nasdaq/MSFT.csv`

 * *Files identical despite different names*

### Comparing `yabte-0.3.5/yabte/tests/data/nasdaq/NFLX.csv` & `yabte-0.3.6/yabte/tests/data/nasdaq/NFLX.csv`

 * *Files identical despite different names*

### Comparing `yabte-0.3.5/yabte/tests/data/nasdaq/TSLA.csv` & `yabte-0.3.6/yabte/tests/data/nasdaq/TSLA.csv`

 * *Files identical despite different names*

### Comparing `yabte-0.3.5/yabte/tests/test_notebooks.py` & `yabte-0.3.6/yabte/tests/test_notebooks.py`

 * *Files identical despite different names*

### Comparing `yabte-0.3.5/yabte/tests/test_portopt.py` & `yabte-0.3.6/yabte/tests/test_portopt.py`

 * *Files identical despite different names*

### Comparing `yabte-0.3.5/yabte/tests/test_simulation.py` & `yabte-0.3.6/yabte/tests/test_simulation.py`

 * *Files identical despite different names*

### Comparing `yabte-0.3.5/yabte/tests/test_strategy_runner.py` & `yabte-0.3.6/yabte/tests/test_strategy_runner.py`

 * *Files identical despite different names*

### Comparing `yabte-0.3.5/yabte/tests/test_utilities.py` & `yabte-0.3.6/yabte/tests/test_utilities.py`

 * *Files identical despite different names*

### Comparing `yabte-0.3.5/yabte/utilities/lagrangian.py` & `yabte-0.3.6/yabte/utilities/lagrangian.py`

 * *Files identical despite different names*

### Comparing `yabte-0.3.5/yabte/utilities/pandas_extension.py` & `yabte-0.3.6/yabte/utilities/pandas_extension.py`

 * *Files identical despite different names*

### Comparing `yabte-0.3.5/yabte/utilities/plot/matplotlib/marker_updater.py` & `yabte-0.3.6/yabte/utilities/plot/matplotlib/marker_updater.py`

 * *Files identical despite different names*

### Comparing `yabte-0.3.5/yabte/utilities/plot/matplotlib/strategy_runner.py` & `yabte-0.3.6/yabte/utilities/plot/matplotlib/strategy_runner.py`

 * *Files 4% similar despite different names*

```diff
@@ -9,18 +9,17 @@
 from ....backtest import StrategyRunner
 from .marker_updater import MarkerUpdater
 
 
 def plot_strategy_runner(sr: StrategyRunner, settings: dict[str, Any] | None = None):
     """Display the results of a strategy run using matplotlib.
 
-    Plots a grid of charts with each column representing a book and rows
-    representing each asset's price series along with long/short
-    positioning and volumne series. A bottom row shows the value of each
-    book as a price series.
+    Plots a grid of charts with each column representing a book and rows representing
+    each asset's price series along with long/short positioning and volumne series. A
+    bottom row shows the value of each book as a price series.
     """
     default_settings = {
         "candle_body_width": 0.8,
         "candle_wick_width": 0.2,
         "candle_up_color": "green",
         "candle_down_color": "red",
         "date_format": "%d-%b-%Y",
```

### Comparing `yabte-0.3.5/yabte/utilities/portopt/hierarchical_risk_parity.py` & `yabte-0.3.6/yabte/utilities/portopt/hierarchical_risk_parity.py`

 * *Files 5% similar despite different names*

```diff
@@ -53,16 +53,16 @@
             alpha = 1 - cVar0 / (cVar0 + cVar1)
             w[cItems0] *= alpha  # weight 1
             w[cItems1] *= 1 - alpha  # weight 2
     return w
 
 
 def hrp(corr: pd.DataFrame, sigma: np.ndarray) -> np.ndarray:
-    """Calculate weights using hierarchical risk parity and scipy's
-    linkage/to_tree functions."""
+    """Calculate weights using hierarchical risk parity and scipy's linkage/to_tree
+    functions."""
     cov = np.diag(sigma) @ corr @ np.diag(sigma)
     cov.index, cov.columns = corr.index, corr.columns
     rho = corr.values
     D = np.sqrt((1 - rho) / 2)
     I, J = np.triu_indices_from(D, 1)
     link = linkage(np.sqrt(np.sum((D[I] - D[J]) ** 2, axis=1)))
     ix_sorted = to_tree(link, rd=False).pre_order()
```

### Comparing `yabte-0.3.5/yabte/utilities/portopt/minimum_variance.py` & `yabte-0.3.6/yabte/utilities/portopt/minimum_variance.py`

 * *Files 5% similar despite different names*

```diff
@@ -29,16 +29,16 @@
     D = B * C - A * A
     l1 = (C * r - A) / D
     l2 = (B - A * r) / D
     return SigmaInv @ (l1 * mu + l2 * ones)
 
 
 def minimum_variance_numeric(Sigma: np.ndarray, mu: np.ndarray, r: float) -> np.ndarray:
-    """Calculate weights using Lagrangian multipliers and numeric solution
-    (using scipy's root function)."""
+    """Calculate weights using Lagrangian multipliers and numeric solution (using
+    scipy's root function)."""
     m = len(mu)
     ones = np.ones(m)
 
     L = Lagrangian(
         objective=lambda x: x.T @ Sigma @ x / 2,
         constraints=[
             lambda x: r - x.T @ mu,
@@ -48,16 +48,16 @@
     )
     return L.fit()
 
 
 def minimum_variance_numeric_slsqp(
     Sigma: np.ndarray, mu: np.ndarray, r: float
 ) -> np.ndarray:
-    """Calculate weights using Lagrangian multipliers and numeric solution
-    (using scipy's minimize function)."""
+    """Calculate weights using Lagrangian multipliers and numeric solution (using
+    scipy's minimize function)."""
     from scipy.optimize import minimize
 
     m = len(mu)
     ones = np.ones(m)
 
     res = minimize(
         lambda x: x.T @ Sigma @ x / 2,
```

### Comparing `yabte-0.3.5/yabte/utilities/simulation/geometric_brownian_motion.py` & `yabte-0.3.6/yabte/utilities/simulation/geometric_brownian_motion.py`

 * *Files identical despite different names*

### Comparing `yabte-0.3.5/yabte/utilities/simulation/heston.py` & `yabte-0.3.6/yabte/utilities/simulation/heston.py`

 * *Files identical despite different names*

### Comparing `yabte-0.3.5/yabte/utilities/simulation/weiner.py` & `yabte-0.3.6/yabte/utilities/simulation/weiner.py`

 * *Files identical despite different names*

### Comparing `yabte-0.3.5/setup.py` & `yabte-0.3.6/setup.py`

 * *Files 3% similar despite different names*

```diff
@@ -4,31 +4,32 @@
 packages = \
 ['yabte',
  'yabte.backtest',
  'yabte.tests',
  'yabte.utilities',
  'yabte.utilities.plot',
  'yabte.utilities.plot.matplotlib',
+ 'yabte.utilities.plot.plotly',
  'yabte.utilities.portopt',
  'yabte.utilities.simulation']
 
 package_data = \
 {'': ['*'], 'yabte.tests': ['data/nasdaq/*']}
 
 install_requires = \
 ['mypy>=1.3.0,<2.0.0',
  'pandas-stubs>=2.0.0.230412,<3.0.0.0',
  'pandas>=1.5.2,<2.0.0',
  'scipy>=1.10.0,<2.0.0']
 
 setup_kwargs = {
     'name': 'yabte',
-    'version': '0.3.5',
+    'version': '0.3.6',
     'description': 'Yet another backtesting engine',
-    'long_description': '# yabte - Yet Another BackTesting Engine\n\nPython module for backtesting trading strategies.\n\nSupport event driven backtesting, ie `on_open`, `on_close`, etc. Also supports multiple assets.\n\nVery basic statistics like book cash, mtm and total value. Currently, everything else needs to be deferred to a 3rd party module like `empyrical`.\n\nThere are some basic tests but use at your own peril. It\'s not production level code.\n\n## Core dependencies\n\nThe core module uses pandas and scipy.\n\n## Installation\n\n```bash\npip install yatbe\n```\n\n## Usage\n\nBelow is an example usage (the performance of the example strategy won\'t be good).\n\n```python\nimport pandas as pd\n\nfrom yabte.backtest import Strategy, StrategyRunner, Order, Book\nfrom yabte.utilities.plot.matplotlib.strategy_runner import plot_strategy_runner\nfrom yabte.utilities.strategy_helpers import crossover\nfrom yabte.tests._helpers import generate_nasdaq_dataset\n\n\nclass SMAXO(Strategy):\n    def init(self):\n        # enhance data with simple moving averages\n\n        p = self.params\n        days_short = p.get("days_short", 10)\n        days_long = p.get("days_long", 20)\n\n        close_sma_short = (\n            self.data.loc[:, (slice(None), "Close")]\n            .rolling(days_short)\n            .mean()\n            .rename({"Close": "CloseSMAShort"}, axis=1, level=1)\n        )\n        close_sma_long = (\n            self.data.loc[:, (slice(None), "Close")]\n            .rolling(days_long)\n            .mean()\n            .rename({"Close": "CloseSMALong"}, axis=1, level=1)\n        )\n        self.data = pd.concat(\n            [self.data, close_sma_short, close_sma_long], axis=1\n        ).sort_index(axis=1)\n\n    def on_close(self):\n        # create some orders\n\n        for symbol in ["GOOG", "MSFT"]:\n            df = self.data[symbol]\n            ix_2d = df.index[-2:]\n            data = df.loc[ix_2d, ("CloseSMAShort", "CloseSMALong")].dropna()\n            if len(data) == 2:\n                if crossover(data.CloseSMAShort, data.CloseSMALong):\n                    self.orders.append(Order(asset_name=symbol, size=-100))\n                elif crossover(data.CloseSMALong, data.CloseSMAShort):\n                    self.orders.append(Order(asset_name=symbol, size=100))\n\n\n# load some data\nassets, df_combined = generate_nasdaq_dataset()\n\n# create a book with 100000 cash\nbook = Book(name="Main", cash="100000")\n\n# run our strategy\nsr = StrategyRunner(\n    data=df_combined,\n    assets=assets,\n    strat_classes=[SMAXO],\n    books=[book],\n)\nsr.run()\n\n# see the trades or book history\nth = sr.transaction_history\nbch = sr.book_history.loc[:, (slice(None), "cash")]\n\n# plot the trades against book value\nplot_strategy_runner(sr);\n\n```\n\n![Output from code](https://raw.githubusercontent.com/bsdz/yabte/main/readme_image.png)\n\n## Examples\n\nJupyter notebook examples can be found under the [notebooks folder](https://github.com/bsdz/yabte/tree/main/notebooks).\n\n## Documentation\n\nDocumentation can be found on [Read the Docs](https://yabte.readthedocs.io/en/latest/).\n\n\n## Development\n\nBefore commit run following format commands in project folder:\n\n```bash\npoetry run black .\npoetry run isort . --profile black\npoetry run docformatter . --recursive --in-place\n```\n',
+    'long_description': '# yabte - Yet Another BackTesting Engine\n\nPython module for backtesting trading strategies.\n\nSupport event driven backtesting, ie `on_open`, `on_close`, etc. Also supports multiple assets.\n\nVery basic statistics like book cash, mtm and total value. Currently, everything else needs to be deferred to a 3rd party module like `empyrical`.\n\nThere are some basic tests but use at your own peril. It\'s not production level code.\n\n## Core dependencies\n\nThe core module uses pandas and scipy.\n\n## Installation\n\n```bash\npip install yatbe\n```\n\n## Usage\n\nBelow is an example usage (the performance of the example strategy won\'t be good).\n\n```python\nimport pandas as pd\n\nfrom yabte.backtest import Strategy, StrategyRunner, Order, Book\nfrom yabte.utilities.plot.matplotlib.strategy_runner import plot_strategy_runner\nfrom yabte.utilities.strategy_helpers import crossover\nfrom yabte.tests._helpers import generate_nasdaq_dataset\n\n\nclass SMAXO(Strategy):\n    def init(self):\n        # enhance data with simple moving averages\n\n        p = self.params\n        days_short = p.get("days_short", 10)\n        days_long = p.get("days_long", 20)\n\n        close_sma_short = (\n            self.data.loc[:, (slice(None), "Close")]\n            .rolling(days_short)\n            .mean()\n            .rename({"Close": "CloseSMAShort"}, axis=1, level=1)\n        )\n        close_sma_long = (\n            self.data.loc[:, (slice(None), "Close")]\n            .rolling(days_long)\n            .mean()\n            .rename({"Close": "CloseSMALong"}, axis=1, level=1)\n        )\n        self.data = pd.concat(\n            [self.data, close_sma_short, close_sma_long], axis=1\n        ).sort_index(axis=1)\n\n    def on_close(self):\n        # create some orders\n\n        for symbol in ["GOOG", "MSFT"]:\n            df = self.data[symbol]\n            ix_2d = df.index[-2:]\n            data = df.loc[ix_2d, ("CloseSMAShort", "CloseSMALong")].dropna()\n            if len(data) == 2:\n                if crossover(data.CloseSMAShort, data.CloseSMALong):\n                    self.orders.append(Order(asset_name=symbol, size=-100))\n                elif crossover(data.CloseSMALong, data.CloseSMAShort):\n                    self.orders.append(Order(asset_name=symbol, size=100))\n\n\n# load some data\nassets, df_combined = generate_nasdaq_dataset()\n\n# create a book with 100000 cash\nbook = Book(name="Main", cash="100000")\n\n# run our strategy\nsr = StrategyRunner(\n    data=df_combined,\n    assets=assets,\n    strat_classes=[SMAXO],\n    books=[book],\n)\nsr.run()\n\n# see the trades or book history\nth = sr.transaction_history\nbch = sr.book_history.loc[:, (slice(None), "cash")]\n\n# plot the trades against book value\nplot_strategy_runner(sr);\n\n```\n\n![Output from code](https://raw.githubusercontent.com/bsdz/yabte/main/readme_image.png)\n\n## Examples\n\nJupyter notebook examples can be found under the [notebooks folder](https://github.com/bsdz/yabte/tree/main/notebooks).\n\n## Documentation\n\nDocumentation can be found on [Read the Docs](https://yabte.readthedocs.io/en/latest/).\n\n\n## Development\n\nBefore commit run following format commands in project folder:\n\n```bash\npoetry run black .\npoetry run isort . --profile black\npoetry run docformatter . --recursive --in-place --black --exclude _unittest_numpy_extensions.py\n```\n',
     'author': 'Blair Azzopardi',
     'author_email': 'blairuk@gmail.com',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'https://github.com/bsdz/yabte',
     'packages': packages,
     'package_data': package_data,
```

### Comparing `yabte-0.3.5/PKG-INFO` & `yabte-0.3.6/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: yabte
-Version: 0.3.5
+Version: 0.3.6
 Summary: Yet another backtesting engine
 Home-page: https://github.com/bsdz/yabte
 License: MIT
 Author: Blair Azzopardi
 Author-email: blairuk@gmail.com
 Requires-Python: >=3.10,<3.12
 Classifier: License :: OSI Approved :: MIT License
@@ -127,10 +127,10 @@
 ## Development
 
 Before commit run following format commands in project folder:
 
 ```bash
 poetry run black .
 poetry run isort . --profile black
-poetry run docformatter . --recursive --in-place
+poetry run docformatter . --recursive --in-place --black --exclude _unittest_numpy_extensions.py
 ```
```

