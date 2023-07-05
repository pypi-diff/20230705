# Comparing `tmp/conding-0.1.2.tar.gz` & `tmp/conding-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "conding-0.1.2.tar", last modified: Sun May  7 18:49:48 2023, max compression
+gzip compressed data, was "conding-0.1.3.tar", last modified: Wed Jul  5 19:02:10 2023, max compression
```

## Comparing `conding-0.1.2.tar` & `conding-0.1.3.tar`

### file list

```diff
@@ -1,31 +1,34 @@
-drwxrwxr-x   0 ygg       (1000) ygg       (1000)        0 2023-05-07 18:49:48.656817 conding-0.1.2/
--rw-rw-r--   0 ygg       (1000) ygg       (1000)    11337 2023-01-20 02:50:04.000000 conding-0.1.2/LICENSE
--rw-rw-r--   0 ygg       (1000) ygg       (1000)      111 2023-01-20 02:50:04.000000 conding-0.1.2/MANIFEST.in
--rw-rw-r--   0 ygg       (1000) ygg       (1000)     6612 2023-05-07 18:49:48.656817 conding-0.1.2/PKG-INFO
--rw-rw-r--   0 ygg       (1000) ygg       (1000)     5713 2023-05-03 21:26:11.000000 conding-0.1.2/README.md
-drwxrwxr-x   0 ygg       (1000) ygg       (1000)        0 2023-05-07 18:49:48.652817 conding-0.1.2/conding/
--rw-rw-r--   0 ygg       (1000) ygg       (1000)       22 2023-05-07 18:48:23.000000 conding-0.1.2/conding/__init__.py
--rw-rw-r--   0 ygg       (1000) ygg       (1000)    11523 2023-05-07 18:48:23.000000 conding-0.1.2/conding/_modidx.py
-drwxrwxr-x   0 ygg       (1000) ygg       (1000)        0 2023-05-07 18:49:48.652817 conding-0.1.2/conding/dune/
--rw-rw-r--   0 ygg       (1000) ygg       (1000)        0 2023-05-07 18:48:23.000000 conding-0.1.2/conding/dune/__init__.py
--rw-rw-r--   0 ygg       (1000) ygg       (1000)     1299 2023-05-07 18:48:23.000000 conding-0.1.2/conding/dune/dune.py
--rw-rw-r--   0 ygg       (1000) ygg       (1000)     6323 2023-05-07 18:48:23.000000 conding-0.1.2/conding/dune/tec.py
-drwxrwxr-x   0 ygg       (1000) ygg       (1000)        0 2023-05-07 18:49:48.652817 conding-0.1.2/conding/pamm/
--rw-rw-r--   0 ygg       (1000) ygg       (1000)        0 2023-05-07 18:48:23.000000 conding-0.1.2/conding/pamm/__init__.py
--rw-rw-r--   0 ygg       (1000) ygg       (1000)     3689 2023-05-07 18:48:23.000000 conding-0.1.2/conding/pamm/abc.py
--rw-rw-r--   0 ygg       (1000) ygg       (1000)     6442 2023-05-07 18:48:23.000000 conding-0.1.2/conding/pamm/bancor.py
-drwxrwxr-x   0 ygg       (1000) ygg       (1000)        0 2023-05-07 18:49:48.656817 conding-0.1.2/conding/samm/
--rw-rw-r--   0 ygg       (1000) ygg       (1000)        0 2023-05-07 18:48:23.000000 conding-0.1.2/conding/samm/__init__.py
--rw-rw-r--   0 ygg       (1000) ygg       (1000)     4643 2023-05-07 18:48:23.000000 conding-0.1.2/conding/samm/uniswap.py
-drwxrwxr-x   0 ygg       (1000) ygg       (1000)        0 2023-05-07 18:49:48.652817 conding-0.1.2/conding.egg-info/
--rw-rw-r--   0 ygg       (1000) ygg       (1000)     6612 2023-05-07 18:49:48.000000 conding-0.1.2/conding.egg-info/PKG-INFO
--rw-rw-r--   0 ygg       (1000) ygg       (1000)      506 2023-05-07 18:49:48.000000 conding-0.1.2/conding.egg-info/SOURCES.txt
--rw-rw-r--   0 ygg       (1000) ygg       (1000)        1 2023-05-07 18:49:48.000000 conding-0.1.2/conding.egg-info/dependency_links.txt
--rw-rw-r--   0 ygg       (1000) ygg       (1000)       36 2023-05-07 18:49:48.000000 conding-0.1.2/conding.egg-info/entry_points.txt
--rw-rw-r--   0 ygg       (1000) ygg       (1000)        1 2023-05-07 18:01:48.000000 conding-0.1.2/conding.egg-info/not-zip-safe
--rw-rw-r--   0 ygg       (1000) ygg       (1000)      190 2023-05-07 18:49:48.000000 conding-0.1.2/conding.egg-info/requires.txt
--rw-rw-r--   0 ygg       (1000) ygg       (1000)        8 2023-05-07 18:49:48.000000 conding-0.1.2/conding.egg-info/top_level.txt
--rw-rw-r--   0 ygg       (1000) ygg       (1000)      589 2023-05-07 18:22:21.000000 conding-0.1.2/pyproject.toml
--rw-rw-r--   0 ygg       (1000) ygg       (1000)     1243 2023-05-07 18:49:23.000000 conding-0.1.2/settings.ini
--rw-rw-r--   0 ygg       (1000) ygg       (1000)       38 2023-05-07 18:49:48.656817 conding-0.1.2/setup.cfg
--rw-rw-r--   0 ygg       (1000) ygg       (1000)     2560 2023-01-20 02:50:04.000000 conding-0.1.2/setup.py
+drwxrwxr-x   0 ygg       (1000) ygg       (1000)        0 2023-07-05 19:02:10.275034 conding-0.1.3/
+-rw-rw-r--   0 ygg       (1000) ygg       (1000)    11337 2023-06-15 18:01:34.000000 conding-0.1.3/LICENSE
+-rw-rw-r--   0 ygg       (1000) ygg       (1000)      111 2023-06-15 18:01:34.000000 conding-0.1.3/MANIFEST.in
+-rw-rw-r--   0 ygg       (1000) ygg       (1000)     6612 2023-07-05 19:02:10.275034 conding-0.1.3/PKG-INFO
+-rw-rw-r--   0 ygg       (1000) ygg       (1000)     5713 2023-06-15 18:01:34.000000 conding-0.1.3/README.md
+drwxrwxr-x   0 ygg       (1000) ygg       (1000)        0 2023-07-05 19:02:10.275034 conding-0.1.3/conding/
+-rw-rw-r--   0 ygg       (1000) ygg       (1000)       22 2023-07-05 18:56:24.000000 conding-0.1.3/conding/__init__.py
+-rw-rw-r--   0 ygg       (1000) ygg       (1000)    13801 2023-07-05 18:56:24.000000 conding-0.1.3/conding/_modidx.py
+drwxrwxr-x   0 ygg       (1000) ygg       (1000)        0 2023-07-05 19:02:10.275034 conding-0.1.3/conding/dune/
+-rw-rw-r--   0 ygg       (1000) ygg       (1000)        0 2023-07-05 18:56:24.000000 conding-0.1.3/conding/dune/__init__.py
+-rw-rw-r--   0 ygg       (1000) ygg       (1000)     1299 2023-07-05 18:56:24.000000 conding-0.1.3/conding/dune/dune.py
+-rw-rw-r--   0 ygg       (1000) ygg       (1000)     7440 2023-07-05 18:56:24.000000 conding-0.1.3/conding/dune/tec.py
+drwxrwxr-x   0 ygg       (1000) ygg       (1000)        0 2023-07-05 19:02:10.275034 conding-0.1.3/conding/pamm/
+-rw-rw-r--   0 ygg       (1000) ygg       (1000)        0 2023-07-05 18:56:24.000000 conding-0.1.3/conding/pamm/__init__.py
+-rw-rw-r--   0 ygg       (1000) ygg       (1000)     4182 2023-07-05 18:57:36.000000 conding-0.1.3/conding/pamm/abc.py
+-rw-rw-r--   0 ygg       (1000) ygg       (1000)     6400 2023-07-05 18:56:24.000000 conding-0.1.3/conding/pamm/bancor.py
+drwxrwxr-x   0 ygg       (1000) ygg       (1000)        0 2023-07-05 19:02:10.275034 conding-0.1.3/conding/samm/
+-rw-rw-r--   0 ygg       (1000) ygg       (1000)        0 2023-07-05 18:56:24.000000 conding-0.1.3/conding/samm/__init__.py
+-rw-rw-r--   0 ygg       (1000) ygg       (1000)     4643 2023-07-05 18:56:24.000000 conding-0.1.3/conding/samm/uniswap.py
+drwxrwxr-x   0 ygg       (1000) ygg       (1000)        0 2023-07-05 19:02:10.275034 conding-0.1.3/conding/utils/
+-rw-rw-r--   0 ygg       (1000) ygg       (1000)        0 2023-07-05 18:56:24.000000 conding-0.1.3/conding/utils/__init__.py
+-rw-rw-r--   0 ygg       (1000) ygg       (1000)     2804 2023-07-05 18:56:24.000000 conding-0.1.3/conding/utils/formatted_param.py
+drwxrwxr-x   0 ygg       (1000) ygg       (1000)        0 2023-07-05 19:02:10.275034 conding-0.1.3/conding.egg-info/
+-rw-rw-r--   0 ygg       (1000) ygg       (1000)     6612 2023-07-05 19:02:10.000000 conding-0.1.3/conding.egg-info/PKG-INFO
+-rw-rw-r--   0 ygg       (1000) ygg       (1000)      565 2023-07-05 19:02:10.000000 conding-0.1.3/conding.egg-info/SOURCES.txt
+-rw-rw-r--   0 ygg       (1000) ygg       (1000)        1 2023-07-05 19:02:10.000000 conding-0.1.3/conding.egg-info/dependency_links.txt
+-rw-rw-r--   0 ygg       (1000) ygg       (1000)       36 2023-07-05 19:02:10.000000 conding-0.1.3/conding.egg-info/entry_points.txt
+-rw-rw-r--   0 ygg       (1000) ygg       (1000)        1 2023-07-05 19:01:06.000000 conding-0.1.3/conding.egg-info/not-zip-safe
+-rw-rw-r--   0 ygg       (1000) ygg       (1000)      190 2023-07-05 19:02:10.000000 conding-0.1.3/conding.egg-info/requires.txt
+-rw-rw-r--   0 ygg       (1000) ygg       (1000)        8 2023-07-05 19:02:10.000000 conding-0.1.3/conding.egg-info/top_level.txt
+-rw-rw-r--   0 ygg       (1000) ygg       (1000)      645 2023-07-05 19:01:31.000000 conding-0.1.3/pyproject.toml
+-rw-rw-r--   0 ygg       (1000) ygg       (1000)     1243 2023-07-05 19:02:06.000000 conding-0.1.3/settings.ini
+-rw-rw-r--   0 ygg       (1000) ygg       (1000)       38 2023-07-05 19:02:10.275034 conding-0.1.3/setup.cfg
+-rw-rw-r--   0 ygg       (1000) ygg       (1000)     2560 2023-06-15 18:01:34.000000 conding-0.1.3/setup.py
```

### Comparing `conding-0.1.2/LICENSE` & `conding-0.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `conding-0.1.2/PKG-INFO` & `conding-0.1.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: conding
-Version: 0.1.2
+Version: 0.1.3
 Summary: Python library for analysing and modelling bonding curves. This library is managed using nbdev with application development in python param panel.
 Home-page: https://github.com/bonding-curves/conding
 Author: Shawn Anderson
 Author-email: shawn@longtailfinancial.com
 License: Apache Software License 2.0
 Keywords: nbdev jupyter notebook python
 Classifier: Development Status :: 4 - Beta
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: conding Version: 0.1.2 Summary: Python library for
+Metadata-Version: 2.1 Name: conding Version: 0.1.3 Summary: Python library for
 analysing and modelling bonding curves. This library is managed using nbdev
 with application development in python param panel. Home-page: https://
 github.com/bonding-curves/conding Author: Shawn Anderson Author-email:
 shawn@longtailfinancial.com License: Apache Software License 2.0 Keywords:
 nbdev jupyter notebook python Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers Classifier: Natural Language ::
 English Classifier: Programming Language :: Python :: 3.7 Classifier:
```

### Comparing `conding-0.1.2/README.md` & `conding-0.1.3/README.md`

 * *Files identical despite different names*

### Comparing `conding-0.1.2/conding/_modidx.py` & `conding-0.1.3/conding/_modidx.py`

 * *Files 22% similar despite different names*

```diff
@@ -9,28 +9,32 @@
                                    'conding.dune.dune.DuneWrapper.__init__': ( 'dune/dune.html#dunewrapper.__init__',
                                                                                'conding/dune/dune.py'),
                                    'conding.dune.dune.DuneWrapper.refresh_into_dataframe': ( 'dune/dune.html#dunewrapper.refresh_into_dataframe',
                                                                                              'conding/dune/dune.py')},
             'conding.dune.tec': { 'conding.dune.tec.TECDashboard': ('dune/tec.html#tecdashboard', 'conding/dune/tec.py'),
                                   'conding.dune.tec.TECDashboard.ABCTributes': ( 'dune/tec.html#tecdashboard.abctributes',
                                                                                  'conding/dune/tec.py'),
+                                  'conding.dune.tec.TECDashboard.BondingCurve': ( 'dune/tec.html#tecdashboard.bondingcurve',
+                                                                                  'conding/dune/tec.py'),
                                   'conding.dune.tec.TECDashboard.Conviction': ( 'dune/tec.html#tecdashboard.conviction',
                                                                                 'conding/dune/tec.py'),
                                   'conding.dune.tec.TECDashboard.MarketInformation': ( 'dune/tec.html#tecdashboard.marketinformation',
                                                                                        'conding/dune/tec.py'),
                                   'conding.dune.tec.TECDashboard.Reserves': ('dune/tec.html#tecdashboard.reserves', 'conding/dune/tec.py'),
                                   'conding.dune.tec.TECDashboard.Trades': ('dune/tec.html#tecdashboard.trades', 'conding/dune/tec.py'),
                                   'conding.dune.tec.TECDashboard.TreasuriesInflowsOutflows': ( 'dune/tec.html#tecdashboard.treasuriesinflowsoutflows',
                                                                                                'conding/dune/tec.py'),
                                   'conding.dune.tec.TECDashboard.__init__': ('dune/tec.html#tecdashboard.__init__', 'conding/dune/tec.py')},
             'conding.pamm.abc': { 'conding.pamm.abc.AugmentedBondingCurve': ('pamm/abc.html#augmentedbondingcurve', 'conding/pamm/abc.py'),
                                   'conding.pamm.abc.AugmentedBondingCurve.__init__': ( 'pamm/abc.html#augmentedbondingcurve.__init__',
                                                                                        'conding/pamm/abc.py'),
                                   'conding.pamm.abc.AugmentedBondingCurve._mint': ( 'pamm/abc.html#augmentedbondingcurve._mint',
                                                                                     'conding/pamm/abc.py'),
+                                  'conding.pamm.abc.AugmentedBondingCurve.set_bounds': ( 'pamm/abc.html#augmentedbondingcurve.set_bounds',
+                                                                                         'conding/pamm/abc.py'),
                                   'conding.pamm.abc.AugmentedBondingCurve.total_price_curve': ( 'pamm/abc.html#augmentedbondingcurve.total_price_curve',
                                                                                                 'conding/pamm/abc.py'),
                                   'conding.pamm.abc.AugmentedBondingCurve.update_deposit': ( 'pamm/abc.html#augmentedbondingcurve.update_deposit',
                                                                                              'conding/pamm/abc.py'),
                                   'conding.pamm.abc.AugmentedBondingCurve.view_chart': ( 'pamm/abc.html#augmentedbondingcurve.view_chart',
                                                                                          'conding/pamm/abc.py'),
                                   'conding.pamm.abc.AugmentedBondingCurve.view_total_price_curve': ( 'pamm/abc.html#augmentedbondingcurve.view_total_price_curve',
@@ -90,8 +94,20 @@
                                       'conding.samm.uniswap.Uniswap.view_chart': ( 'samm/1-uniswap-mathv2.html#uniswap.view_chart',
                                                                                    'conding/samm/uniswap.py'),
                                       'conding.samm.uniswap.Uniswap.view_curves': ( 'samm/1-uniswap-mathv2.html#uniswap.view_curves',
                                                                                     'conding/samm/uniswap.py'),
                                       'conding.samm.uniswap.Uniswap.view_points': ( 'samm/1-uniswap-mathv2.html#uniswap.view_points',
                                                                                     'conding/samm/uniswap.py'),
                                       'conding.samm.uniswap.Uniswap.xy_curve': ( 'samm/1-uniswap-mathv2.html#uniswap.xy_curve',
-                                                                                 'conding/samm/uniswap.py')}}}
+                                                                                 'conding/samm/uniswap.py')},
+            'conding.utils.formatted_param': { 'conding.utils.formatted_param.FormattedParam': ( 'utils/formatted_param.html#formattedparam',
+                                                                                                 'conding/utils/formatted_param.py'),
+                                               'conding.utils.formatted_param.FormattedParam.__init__': ( 'utils/formatted_param.html#formattedparam.__init__',
+                                                                                                          'conding/utils/formatted_param.py'),
+                                               'conding.utils.formatted_param.FormattedParam.autostep': ( 'utils/formatted_param.html#formattedparam.autostep',
+                                                                                                          'conding/utils/formatted_param.py'),
+                                               'conding.utils.formatted_param.FormattedParam.autostep_value': ( 'utils/formatted_param.html#formattedparam.autostep_value',
+                                                                                                                'conding/utils/formatted_param.py'),
+                                               'conding.utils.formatted_param.FormattedParam.view': ( 'utils/formatted_param.html#formattedparam.view',
+                                                                                                      'conding/utils/formatted_param.py'),
+                                               'conding.utils.formatted_param.FormattedParam.widgets': ( 'utils/formatted_param.html#formattedparam.widgets',
+                                                                                                         'conding/utils/formatted_param.py')}}}
```

### Comparing `conding-0.1.2/conding/dune/dune.py` & `conding-0.1.3/conding/dune/dune.py`

 * *Files identical despite different names*

### Comparing `conding-0.1.2/conding/dune/tec.py` & `conding-0.1.3/conding/dune/tec.py`

 * *Files 10% similar despite different names*

```diff
@@ -10,20 +10,22 @@
 import numpy as np
 
 # %% ../../nbs/dune/1_tec.ipynb 4
 class TECDashboard(DuneWrapper):
     "Interface to the TEC Dune Analytics dashboard."
     
     def __init__(self):
+        super().__init__()
         self.market_information = self.MarketInformation()
         self.treasury_inflows_outflows = self.TreasuriesInflowsOutflows()
         self.reserves = self.Reserves()
         self.trades = self.Trades()
         self.abc_tributes = self.ABCTributes()
         self.conviction = self.Conviction()
+        self.bonding_curve = self.BondingCurve()
     
     class MarketInformation(DuneWrapper):
     
         def mint_price(self, **params)->pd.DataFrame:
             """NOT WORKING"""
             df = self.refresh_into_dataframe(461108, **params)
             return df
@@ -51,19 +53,19 @@
         def holders_and_supply(self, **params)->pd.Series:
             """Number of TEC Holders and total supply."""
             df = self.refresh_into_dataframe(1898886, **params).iloc[0]
             return df
         
         def total_holders(self, **params)->float:
             """Number of TEC Holders."""
-            return self.holders_and_supply()['total_holders']
+            return self.holders_and_supply(**params)['total_holders']
         
         def supply(self, **params)->float:
             """TEC Supply."""
-            return self.holders_and_supply()['supply']
+            return self.holders_and_supply(**params)['supply']
         
         def holders_over_time(self, **params)->pd.DataFrame:
             """TEC holders over time."""
             df = self.refresh_into_dataframe(1898887, **params)
             return df
         
         def holders_distribution(self, **params)->pd.DataFrame:
@@ -105,25 +107,38 @@
             df = self.refresh_into_dataframe(394987, **params)
             return df
         
     class Reserves(DuneWrapper):
 
         def reserve_pool(self, **params)->pd.Series:
             """Reserve pool information."""
+
+            # Ensure there is an end date in the future to get accurate results.
+            if type(params.get('params')) is list:
+                params['params'] += [{
+                "type": "date",
+                "name": "2. End Date",
+                "value": "2055-05-04 00:00:00",}]
+            else:
+                params['params'] = [{
+                "type": "date",
+                "name": "2. End Date",
+                "value": "2055-05-04 00:00:00",}]
+            
             df = self.refresh_into_dataframe(1752257, **params).iloc[0]
             return df
         
         def total_pool_value(self, **params)->float:
-            return self.reserve_pool()['total_pool_value']
+            return self.reserve_pool(**params)['total_pool_value']
         
         def reserve_pool_value(self, **params)->float:
-            return self.reserve_pool()['reserve_pool_value']
+            return self.reserve_pool(**params)['reserve_pool_value']
         
         def common_pool_value(self, **params)->float:
-            return self.reserve_pool()['common_pool_value']
+            return self.reserve_pool(**params)['common_pool_value']
         
         def commons_pool_balance_over_time(self, **params)->pd.DataFrame:
             """Common pool balance over time."""
             df = self.refresh_into_dataframe(1754471, **params)
             return df
         
         def reserve_balance_over_time(self, **params)->pd.DataFrame:
@@ -156,7 +171,21 @@
             return df
         
     class Conviction(DuneWrapper):
         
         def tec_proposals(self, **params):
             df = self.refresh_into_dataframe(1849767, **params)
             return df
+        
+    class BondingCurve(DuneWrapper):
+        
+        def total_liquidity_over_time_honeyswap(self, **params):
+            df = self.refresh_into_dataframe(2437505, **params)
+            return df
+        
+        def total_liquidity_over_time_honeyswap_aggregated(self, **params):
+            df = self.refresh_into_dataframe(2437591, **params)
+            return df
+        
+        def TEC_total_supply(self, **params):
+            df = self.refresh_into_dataframe(2422062, **params)
+            return df
```

### Comparing `conding-0.1.2/conding/pamm/abc.py` & `conding-0.1.3/conding/pamm/abc.py`

 * *Files 18% similar despite different names*

```diff
@@ -20,14 +20,22 @@
     total_mint_price = pm.Number(constant=True)
     mint_tribute  = pm.Number(constant=True)
     common_pool   = pm.Number(0, constant=True, softbounds=(0,1000), bounds=(0, None))
     
     def __init__(self, **params):
         super().__init__(**params)
         self.update_deposit()
+        self.set_bounds()
+        
+    def set_bounds(self):
+        self.param['supply'].softbounds = (self.supply/2, self.supply*1.5)
+        self.param['reserve_balance'].softbounds = (self.reserve_balance/2, self.reserve_balance*1.5)
+        self.param['common_pool'].softbounds = (self.common_pool/2, self.common_pool*1.5+100)
+        self.param['mint_amount'].step = 1
+        self.param['mint_amount'].softbounds = (-self.supply/5, self.supply/5)
         
     @pm.depends('entry_tribute', 'exit_tribute', 'deposit', watch=True)
     def update_deposit(self):
         with pm.edit_constant(self):
             if self.deposit > 0:
                 self.total_mint_deposit = self.deposit / (1 - self.entry_tribute)
                 self.total_mint_price = self.total_mint_deposit / self.mint_amount
@@ -43,15 +51,15 @@
                 
     def _mint(self):
         with pm.edit_constant(self):
             self.common_pool += self.mint_tribute
         super()._mint()
         
     def total_price_curve(self):
-        supply = np.linspace(*self.param['supply'].softbounds, num=1000)
+        supply = np.linspace(self.param['supply'].softbounds[0],self.param['supply'].softbounds[1]-1, num=1000)
         mint_amount = supply - self.supply
         deposit = self.get_balance_deposit(mint_amount)
         mint_total_price = deposit / (1 - self.entry_tribute) / mint_amount
         burn_total_price = (deposit - deposit * self.exit_tribute) / mint_amount
         total_price = np.where(supply > self.supply, mint_total_price, burn_total_price)
         df = pd.DataFrame({
             'Supply': supply,
```

### Comparing `conding-0.1.2/conding/pamm/bancor.py` & `conding-0.1.3/conding/pamm/bancor.py`

 * *Files 1% similar despite different names*

```diff
@@ -33,15 +33,15 @@
         self.update()
     
     @pm.depends('reserve_balance', 'supply', 'price', 'mint_amount', watch=True)
     def update(self):
         with pm.edit_constant(self):
             self.marketcap = self.price * self.supply
             self.reserve_ratio = self.reserve_balance / self.marketcap
-            self.param['mint_amount'].bounds = [-self.supply+1, self.param['supply'].softbounds[1]-self.supply]
+            self.param['mint_amount'].bounds = [-self.supply+1, None]
             self.n = ((1 / self.reserve_ratio) - 1)
             self.m = self.price / self.supply ** self.n
             if self.mint_amount == 0:
                 self.deposit = 0
                 self.mint_price = self.price
                 self.new_price = self.price
             else:
```

### Comparing `conding-0.1.2/conding/samm/uniswap.py` & `conding-0.1.3/conding/samm/uniswap.py`

 * *Files identical despite different names*

### Comparing `conding-0.1.2/conding.egg-info/PKG-INFO` & `conding-0.1.3/conding.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: conding
-Version: 0.1.2
+Version: 0.1.3
 Summary: Python library for analysing and modelling bonding curves. This library is managed using nbdev with application development in python param panel.
 Home-page: https://github.com/bonding-curves/conding
 Author: Shawn Anderson
 Author-email: shawn@longtailfinancial.com
 License: Apache Software License 2.0
 Keywords: nbdev jupyter notebook python
 Classifier: Development Status :: 4 - Beta
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: conding Version: 0.1.2 Summary: Python library for
+Metadata-Version: 2.1 Name: conding Version: 0.1.3 Summary: Python library for
 analysing and modelling bonding curves. This library is managed using nbdev
 with application development in python param panel. Home-page: https://
 github.com/bonding-curves/conding Author: Shawn Anderson Author-email:
 shawn@longtailfinancial.com License: Apache Software License 2.0 Keywords:
 nbdev jupyter notebook python Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers Classifier: Natural Language ::
 English Classifier: Programming Language :: Python :: 3.7 Classifier:
```

### Comparing `conding-0.1.2/pyproject.toml` & `conding-0.1.3/pyproject.toml`

 * *Files 26% similar despite different names*

```diff
@@ -10,14 +10,17 @@
 pandas = "^1.5.3"
 hvplot = "^0.8.3"
 python-dotenv = "^1.0.0"
 dune-client = "^1.0.0"
 diskcache = "^5.6.1"
 pyparsing = "^3.0.9"
 yfinance = "^0.2.18"
+millify = "^0.1.1"
+icecream = "^2.1.3"
+twine = "^4.0.2"
 
 
 [tool.poetry.group.dev.dependencies]
 nbdev = "^2.3.12"
 jupyterlab = "3.6.0"
 ipython = "^8.12.0"
 icecream = "^2.1.3"
```

### Comparing `conding-0.1.2/settings.ini` & `conding-0.1.3/settings.ini`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 [DEFAULT]
 # All sections below are required unless otherwise specified.
 # See https://github.com/fastai/nbdev/blob/master/settings.ini for examples.
 
 ### Python library ###
 repo = conding
 lib_name = %(repo)s
-version = 0.1.2
+version = 0.1.3
 min_python = 3.7
 license = apache2
 black_formatting = False
 
 ### nbdev ###
 doc_path = _docs
 lib_path = conding
```

### Comparing `conding-0.1.2/setup.py` & `conding-0.1.3/setup.py`

 * *Files identical despite different names*

